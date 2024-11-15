# <p align="center"> Elist Sales Analysis </p>

### Overview

Elist, established in 2018, is an e-commerce business specializing in popular electronics. Initially focused on the local market, Elist has grown to serve customers worldwide. Their products are available for purchase through both their website and mobile app. To engage their audience, they utilize various marketing strategies such as email marketing, SEO tactics, and affiliate programs. Among their top-selling items are electronics from major brands like Apple, Samsung, and ThinkPad.

The company has vast amounts of data on its (fill in topics). This data, previously underutilised, is now being thoroughly analysed to uncover critical insights aimed at enhancing their commercial performance. The project provides insights and recommendations on the following key areas:

### Current list of topics
- Product Performance
- Global Reach
- Loyalty Program
- Marketing Channels
- Refund Rates
- Purchase Platform

### Should I include these topics? Exclude some topics?
- Sales Trends - Focused on Revenue, Orders Placed, and Average Order Value (AOV).
- Product Performance - An analysis of different product lines and their market impact.
- Loyalty Programme Performance - Assessment of the loyalty programme's effectiveness and its future.
- Operational Effectiveness - Evaluation of logistics and operational efficiency.
- Marketing Channel Effectiveness - Analysis of various marketing channels and their return on investment.

### The SQL queries performed to uncover these general insights are found here.

### Targeted SQL queries relating to these categories can also be found here.

### Tableau dashboard can be found here.


<br>
<br>

### <p align="center"> Deep-Dive Insights </p>

#### Product Performance

- **Findings:**

Apple Airpods are Elist's most popular product by order count, comprising 45% of all orders (48K+). The 27in 4K Gaming Monitor is Elist's top revenue generating product, generating almost $10M (35% of total sales). The Gaming Monitor, Apple Airpods, the Macbook Air and ThinkPad Laptops generate 96% of revenue. Elitch should prioritize the marketing of these 4 products over the rest of its current catalog to maintain market presence.

Of importance to note, Elist sees a significant percentage of orders of the Samsung Charging Cable Pack (20%). This product generates 2% of total sales and an opportunity to capture more value by either increasing the price or offering a bundle version of this product exists.

Product Performance
96% of current sales come from products in these categories:
Wireless In-Ear Headphones
High-End Gaming Monitors
Lighterweight Laptops
DotDash should expand its product catalog to offer similar, in-class products. Doing so will improve sales performance and brand reach.

- **Yearly summary:** From 2019 to 2022, average number of sales per year was 27K, with average yearly sale revenue of $7M and average order value of $254. 2021 saw the highest number of sales (36K), but 2020 had on average the most expensive sales (AOV of $300).
- **Growth rates:** 2020 had by far the highest growth rate, with more than double the number of sales and the total sales revenue than 2019. On average, 2020 sales were also 31% more expensive than 2019 sales. While 2021 exhibited positive growth in the number of sales, total sales revenue went down, as people purchased items that were an average of 15% less expensive than in 2021.


- **Recommendation:** ghjghh
  

<img width="500" alt="Product Sales Graph" src="https://github.com/user-attachments/assets/53c4f5dd-2e01-4219-9175-327cf63a8235">
<img width="500" alt="Product Sales Table" src="https://github.com/user-attachments/assets/75100b5a-31e7-4fb0-887e-f29a724896d1">


#### Seasonality

- **Findings:** Elist experiences a holiday sales surge each year in sales growth rate in November (18%) and December (23%), with a decrease following in January (-10%) and February (-25%) and a rebound in March (18%). While Elist's sales trend follows common seasonality for companies selling electronics, these figures offer insights into consumer behavior. For example, the ‘best’ deals in consumers' eyes start to run through the holiday season so customers in October may be waiting for ‘deal season’ to start in November or are finding deals elsewhere. October requires more insight analysis into whether something can be done to improve sales.

Average order value (AOV) and percentage of total sales have little to note since all months are very similar.

- **Recommendation:** 


<img width="500" alt="Seasonality" src="https://github.com/user-attachments/assets/e47024fc-952f-498e-a384-5f110f9b5650">
<img width="500" alt="Seasonality" src="https://github.com/user-attachments/assets/29957c3b-ee26-452a-b163-983c28180cc0">



#### Global Reach

- **Findings:**
Elist had customers place orders from 195 countries. The US drives by far the most sales with 47% of total sales. If we expand further, the top 12 countries drive 80% of total sales (shown below). Maintaining strong presences in these countires should be a top priority, especially as Elist angles to maintain some of the excess value captured from 2020. Further, it would serve Elist well to identify similarities between countries because this analysis can be used to identify new market opportunities.

After filtering for countries with 100 or more orders, there are 12 countries with an average order value above $300. Thus suggesting experimentation with efforts to increase brand reach within these countries may drive future sales growth.

Global Presence
Knowing 85% orders and sales come from 17 countries, DotDash should concentrate marketing efforts on maintaining market penetration in these countries in the short-term. To create growth opportunities over the longer term, DotDash should create a project to identify 'similar' countries, to its top performers.

It is also in DotDash's best interest to prioritize experimenting in the APAC region. Even though this region accounts for 12% of sales, it has the highest AOV. Pairing that with an understanding that consumer tendencies in this region are to purchase higher-priced "status symbols", efforts to penetrate this market should provide a significant boost in sales.

- **Recommendation:** ghjghh


<img width="350" alt="Sales by Location" src="https://github.com/user-attachments/assets/9d40231b-97f8-42b2-b947-093f20e18e8c">
<img width="206" alt="Average Order Value by Location" src="https://github.com/user-attachments/assets/47e8fdad-a042-431e-9140-3c4c33841ad5">
<img width="1000" alt="Average Order Value by Location (map)" src="https://github.com/user-attachments/assets/e58c7eca-8323-4c51-90d5-7ab1222932ca">


#### Loyalty Program

<img width="800" alt="Loyalty Program Comparison" src="https://github.com/user-attachments/assets/f43730e3-d160-435b-b393-a25c0ddb9bb9">

- **Findings:**
The loyalty program seems to serve as another viable avenue to maintain some of the value captured in 2020's boom. After it's rollout in 2019, significant customer adoption did not occur until the beginning of 2021. Sales and order count from loyalty customers exceeded that of non-loyalty customers in 2021. This trend has continued through 2022 with the AOV of loyalty customers now also exceeding that of non-loyalty customers.

From Sep through Dec ‘22, non-loyalty customer sales, aov and order count has surpassed the metrics of loyalty customers. This is the first time since Dec ‘20 order count of non-loyalty customers has exceeded that of loyalty customers.

Until these most recent micro trends, there has been evidence to support the loyalty program as a key way to maintaining captured value, given DotDash's overall sales have been declining since ‘20.

Due to this concerning recent trend in the loyalty program, DotDash should cut affiliate channel marketing efforts and focus efforts on reaching customers through the direct and email channels. These channels have led to the most signups and have a significant signup rate:

Direct Marketing Channel: 40% signup rate | 23.5K signups
Email Marketing Channel: 59% signup rate | 8K signups

During 2019 and 2020, loyalty program customers made fewer purchases than non-loyalty program customers, and their purchases were less expensive than non-loyalty customers. However, in more recent years (2021-2022), loyalty customers not only made more purchases than non-loyalty customers, but also purchased about $30 more on average in 2022.

- **Recommendation:** Considering the fact that in recent years, loyalty customers are not only making more purchases but also more expensive purchases than non-loyalty customers, we would recommend continuing with the loyalty program.


  
#### Marketing Channels

- **Findings:** The direct marketing channel has the highest number of loyalty participants: 32.9K signups (39% signup rate). The email marketing channel has the highest average signup rate: 58% signup rate (~10.8K signups). The affiliate marketing channel has the lowest average signup rate: 16% signup rate (~500 signups). Based on this information, more money should be spent on the email marketing channel and less spent on the affiliate marketing channel. Money should continue to be spent on the direct marketing channel even though the signup rate isn't the highest because the number of signups are still very high.

The direct marketing channel has been the most successful for the number of orders each year. However, the affiliate marketing channel has steadily had the highest average order value each year and should be pursued further. Email marketing channel has consistently had the lowest number of orders and average order value, so less marketing should be spent here.

Need to identify the marketing channels for 85 unknown and 1387 blank customers.

- **Recommendation:** 
Prioritize marketing incentives on high-performing items like the Apple AirPods Headphones and 27in 4K Gaming Monitor.
Work with the products team to investigate the poor product performance of the Bose Soundsport Headphones and identify a replacement.
Incentivize email marketing channels to increase customer loyalty signup rate.
Continue the loyalty program and work with data analyst teams to monitor yearly growth and revenue.
Work with the products team to investigate the high refund rates of the ThinkPad Laptop and Macbook Air Laptop while improving product descriptions and photos.

<img width="500" alt="Marketing Channels" src="https://github.com/user-attachments/assets/29e9d65c-0c5b-49b1-ab13-c7c04253750a">
<img width="500" alt="Loyalty + Channel" src="https://github.com/user-attachments/assets/ad06dcd7-ef4a-459e-966c-849b7015ec01">






#### Refund Rates

- **Findings:** The ThinkPad Laptop (12%) and Macbook Air Laptop (11%) have the highest refund rates, while the Apple Airpods Headphones (2,636) and 27in 4K Gaming Monitor (1,444) have the highest number of refunds.
- **Recommendation:** This isn't cause for concern because there's a strong trend between average order value and refund rate that shows when the average order value increases, the refund rate also increases. Therefore, higher number of refunds are a natural consequence of higher price.

<img width="500" alt="AOV and Refund Rate - Bar Graph" src="https://github.com/user-attachments/assets/6a04c540-c496-4361-8f10-631bfa304124">
<img width="500" alt="AOV and Refund Rate - Scatter Plot" src="https://github.com/user-attachments/assets/41c769b3-0d9a-432d-a191-1f6dad1ed290">



<br>
<br>

#### Purchase Platform

- **Findings:** Both the mobile app and the website saw a significant increase in total sales and orders in 2020. This is inline with the other data. One other significant point is that the mobile app had a 165% increase in orders in 2021 and the website had a decrease of 11%. This increase in mobile app orders came from the Samsung Charging Cable Pack (351% increase) and the Samsung Webcam (128% increase).
- **Recommendation:** This suggests that it might be worth focusing the mobile app on smaller purchases whereas the website should focus on larger purchases.

<img width="410" alt="Purchasing Platform" src="https://github.com/user-attachments/assets/dedbe4e3-e4b7-4dee-958e-913dc6691d51">

<img width="501" alt="Mobile App" src="https://github.com/user-attachments/assets/a4d961ad-6a5b-4ee4-a052-4f069a3f6ff5">












## ERD
The entity relation diagram (ERD) can be found [here](https://github.com/JordanCWard/elist_analysis/blob/main/Elist_ERD.png).

# About the Data
Include file about data cleaning here
Include workbook for more analysis here
