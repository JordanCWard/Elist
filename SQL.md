
Order counts, sales, and AOV for Macbooks sold in North America for each quarter across all years.

``` sql
SELECT 
  DATE_TRUNC(purchase_ts, quarter) AS quarter, 
  COUNT(
    DISTINCT(orders.id)
  ) AS order_count, 
  SUM(usd_price) AS sales, 
  AVG(usd_price) AS aov 
FROM 
  core.orders 
  LEFT JOIN core.customers ON orders.customer_id = customers.id 
  LEFT JOIN core.geo_lookup ON customers.country_code = geo_lookup.country_code 
WHERE 
  product_name = 'Macbook Air Laptop' 
  AND region = 'NA' 
GROUP BY 
  1 
ORDER BY 
  quarter ASC;
```

Number of Macbooks ordered in USD each month in 2019 through 2020, sorted oldest to most recent.

``` sql
SELECT 
  date_trunc(purchase_ts, month) AS order_month, 
  COUNT(
    product_name = 'Macbook Air Laptop'
  ) AS Macbook_orders 
FROM 
  core.orders 
WHERE 
  currency = 'USD' 
  AND purchase_ts BETWEEN '2019-01-01' 
  AND '2020-12-31' 
GROUP BY 
  order_month 
ORDER BY 
  order_month ASC;

```

All unique combinations of product IDs and product names of Apple and Bose products.

``` sql
SELECT 
  distinct(product_id), 
  product_name 
FROM 
  core.orders 
WHERE 
  product_name LIKE 'Apple%' 
  OR product_name LIKE 'Mac%' 
  OR product_name LIKE 'bose%' 
order by 
  2;
```

Region with longest time to deliver (products purchased on mobile OR products purchased in 2022 on the website).

``` sql
SELECT 
  geo_lookup.region, 
  AVG(
    DATE_DIFF(
      order_status.delivery_ts, order_status.purchase_ts, 
      day
    )
  ) time_to_deliver 
FROM 
  core.orders 
  LEFT JOIN core.customers ON orders.customer_id = customers.id 
  LEFT JOIN core.geo_lookup ON customers.country_code = geo_lookup.country_code 
  LEFT JOIN core.order_status ON orders.id = order_status.order_id 
WHERE 
  purchase_platform = "website" 
  AND extract(
    year 
    from 
      orders.purchase_ts
  ) = 2022 
  OR purchase_platform = "mobile app" 
GROUP BY 
  1 
ORDER BY 
  2 DESC;
```

For orders in 2020: purchase month, shipping month, time to ship (in days), and product name.

``` sql
SELECT 
  date_trunc(order_status.purchase_ts, month) as purchase_month, 
  date_trunc(ship_ts, month) as shipping_month, 
  date_diff(
    ship_ts, order_status.purchase_ts, 
    day
  ) as time_to_ship, 
  product_name 
FROM 
  core.order_status 
  LEFT Join core.orders ON order_status.order_id = orders.id 
Where 
  extract(
    year 
    from 
      order_status.purchase_ts
  ) = 2020;
```

Refund rate and refund count for each product.

``` sql
SELECT 
  CASE WHEN product_name = '27in"" 4k gaming monitor' THEN '27in 4K gaming monitor' ELSE product_name END AS product_clean, 
  SUM(
    CASE WHEN refund_ts IS NOT NULL THEN 1 ELSE 0 END
  ) AS refunds, 
  AVG(
    CASE WHEN refund_ts IS NOT NULL THEN 1 ELSE 0 END
  ) AS refund_rate 
FROM 
  core.orders 
  LEFT JOIN core.order_status ON orders.id = order_status.order_id 
GROUP BY 
  1 
ORDER BY 
  3 DESC;
```

Most popular product within each region.

``` sql
WITH sales_by_product AS (
  SELECT 
    count(product_id) AS total_orders, 
    CASE WHEN product_name = '27in"" 4k gaming monitor' THEN '27in 4K gaming monitor' ELSE product_name END AS product_clean, 
    region 
  FROM 
    core.orders 
    LEFT JOIN core.customers ON orders.customer_id = customers.id 
    LEFT JOIN core.geo_lookup ON customers.country_code = geo_lookup.country_code 
  GROUP BY 
    product_name, 
    region 
  ORDER BY 
    total_orders DESC
) 
SELECT 
  *, 
  ROW_NUMBER() OVER (
    PARTITION BY region 
    ORDER BY 
      total_orders DESC
  ) AS order_ranking 
FROM 
  sales_by_product QUALIFY ROW_NUMBER() OVER (
    PARTITION BY region 
    ORDER BY 
      total_orders DESC
  ) = 1;
```

Average time to make a purchase after creating an account, loyalty customers vs. non-loyalty customers).

``` sql
SELECT 
  AVG(
    DATE_DIFF(
      orders.purchase_ts, created_on, day
    )
  ) AS time_to_purchase, 
  loyalty_program 
FROM 
  core.customers 
  LEFT JOIN core.orders ON customers.id = orders.customer_id 
GROUP BY 
  2;
```
