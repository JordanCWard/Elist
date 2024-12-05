## to do

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

108124 total orders so this is a very small amount of data
18 orders have negative value from -697 to -3 days for ship - purchase
23 orders have values 25 to 1297 days for ship - purchase
rest are 1 to 3

108124 total orders so this is a very small amount of data
17 orders have values from -694 to -16 days for deliver - purchase
23 orders have values from 29 to 1300 days for deliver - purchase
rest are 5 to 10

the issue is with the purchase date because deliver - ship has values from 2 to 9

look at refund section for purchase date stuff

Continue below, data has been created
file is called regression analysis
green columns are cleaned and ready to analyze, red need fixing, yellow might need fixing?
there's an issue in the ship - purchase column, is it also in deliver - purchase column and deliver - ship column? data should be noted in the report below somewhere
negative values should be removed from data, doesn't make sense, should be noted though as part of data cleaning

Transform categorical variables to numbers then run correlation analysis, such as email = 1, direct = 2, etc
Use the Data Analysis Toolpak (enable it via File > Options > Add-ins):
Go to Data > Data Analysis > Correlation.
Select your data range and get a matrix of correlations.

#### Use this somewhere in the future sections
regression analysis
Excel's Data Analysis tool
- Use Excel's Forecast.Linear or Forecast.ETS functions for basic predictive modeling.

- Build a simple linear regression model to predict sales:
- X-axis: Time (e.g., months).
- Y-axis: Sales (total sales or per product).

#### operational effectiveness
- add more info about effectiveness
- write recommendation

#### graphs/tables
- include various types
- don't repeat too often
- standardize colors, fonts, borders
- put them before or after info?

#### make sure that graphs are the best chosen for what the data is showing

#### rewrite current list of topics/titles better

#### fix sizing of headers

#### clean up excel file



<br>
<br>



# <p align="center"> Elist Sales Analysis </p>

### Overview

Elist, established in 2018, is an e-commerce business specializing in popular electronics. Initially focused on the local market, Elist has grown to serve customers worldwide. Their products are available for purchase through both their website and mobile app. To engage their audience, they utilize various marketing strategies such as email marketing, SEO tactics, and affiliate programs. Among their top-selling items are electronics from major brands like Apple, Samsung, and ThinkPad.

The company has vast amounts of data on its (fill in topics). This data, previously underutilised, is now being thoroughly analysed to uncover critical insights aimed at enhancing their commercial performance. The project provides insights and recommendations on the following key areas:

### Current list of topics
- Sales Trends: Focused on ____ (Focused on Revenue, Orders Placed, and Average Order Value (AOV).)
- Product Performance: Focused on ____ (An analysis of different product lines and their market impact.)
- Global Reach: Focused on ____
- Loyalty Program: Focused on ____ (Loyalty Programme Performance - Assessment of the loyalty programme's effectiveness and its future.)
- Marketing Channels: Focused on ____ (Marketing Channel Effectiveness - Analysis of various marketing channels and their return on investment.)
- Purchasing Platform: Focused on ____
- Refund Rates: Focused on ____
- Operational Effectiveness: Focused on ____ (Evaluation of logistics and operational efficiency.)

- The SQL queries performed to uncover these general insights are found here.

- Targeted SQL queries relating to these categories can also be found here.

- Tableau dashboard can be found here.





### <p align="center"> Deep-Dive Insights </p>

### Sales Trends

- Remove Sales by Month and Growth Rates?

<img width="500" alt="Seasonality" src="https://github.com/user-attachments/assets/e47024fc-952f-498e-a384-5f110f9b5650">
<img width="388" alt="Sales by Month and Growth Rates" src="https://github.com/user-attachments/assets/64ae9d32-2163-47e4-9987-9c3986daca0f">
<img width="500" alt="Total Sales - 3 Month Moving Average" src="https://github.com/user-attachments/assets/e6ed8f17-b0c1-4d31-a090-7ef80e5b588b">
<img width="216" alt="Sales by Year" src="https://github.com/user-attachments/assets/905af2c4-9424-47ce-8048-c1644e0c5d20">

#### Findings:
- **Revenue and Order Trends:** Between 2019 and 2022, Elist generated over $28 million in revenue from more than 100,000 orders, with an average order value (AOV) of $260. The peak year was 2020, which saw the highest revenue ($10.2 million) and AOV ($300), likely due to increased pandemic-related spending. In contrast, 2021 recorded the highest number of orders (36,000).
- **Seasonal Sales Patterns:** Elist experiences a holiday sales surge, with growth rates of 18% in November and 23% in December. This is followed by significant declines in January (-10%) and February (-25%), with a rebound of 18% in March. October sees potential sales stagnation as consumers may wait for holiday deals or shop elsewhere.
- **Consumer Behavior Insights:** The sales pattern aligns with typical electronics seasonality, with holiday promotions influencing consumer purchasing decisions. October’s lower activity highlights a potential opportunity to better engage customers before the holiday season.

#### Recommendations:
- **Maximize November and December Promotions:** Expand marketing campaigns starting in early November to capitalize on the surge in sales growth (18% in November and 23% in December). Highlight exclusive deals, limited-time offers, and bundle packages to drive urgency and boost AOV.
- **Retain Post-Holiday Shoppers:** Offer “New Year” incentives in January to mitigate the 10% sales decline, such as discount codes for future purchases or post-holiday clearance sales.
- **Optimize for March Rebound:** Prepare a focused campaign to harness the 18% sales rebound in March, potentially targeting customers who paused spending after the holiday season. Promote spring deals or “fresh start” themes tied to new product launches or upgrades.
- **Investigate Drop-off Causes:** Conduct customer surveys and study competitor trends to understand consumer behavior in October and other slower months. Test incentives (e.g., early-bird discounts, pre-holiday bundles) to encourage purchases before the “deal season” begins in November.


### Product Performance

<img width="500" alt="Product Sales Graph" src="https://github.com/user-attachments/assets/53c4f5dd-2e01-4219-9175-327cf63a8235">
<img width="500" alt="Product Sales Table" src="https://github.com/user-attachments/assets/75100b5a-31e7-4fb0-887e-f29a724896d1">

#### Findings:
- **Popular Products by Order Volume:** Apple AirPods are Elist's most popular product, accounting for 45% of all orders (48,000+ units).
- **Top Revenue Generator:** The 27-inch 4K Gaming Monitor is Elist's highest revenue-generating product, contributing nearly $10 million (35% of total sales).
- **Key Revenue Drivers:** Four products—Gaming Monitor, Apple AirPods, MacBook Air, and ThinkPad Laptops—together account for 96% of Elist's total revenue.
- **Samsung Charging Cable Pack:** This product constitutes 20% of orders but contributes only 2% of total sales, indicating room for optimization.

#### Recommendations:
- **Expand Product Catalog:** To diversify revenue streams, Elist should consider adding more products in the same categories as its top performers, focusing on in-class alternatives.
- **Optimize Samsung Charging Cable Pack Strategy:** Increase profitability by exploring price adjustments or introducing a bundled version of the product to capture additional value.


### Global Reach

<img width="350" alt="Sales by Location" src="https://github.com/user-attachments/assets/9d40231b-97f8-42b2-b947-093f20e18e8c">
<img width="337" alt="Average Order Value by Location" src="https://github.com/user-attachments/assets/cdf35e3f-4fa7-4159-b17c-1f041267f8db">
<img width="400" alt="Average Order Value by Location (map)" src="https://github.com/user-attachments/assets/e58c7eca-8323-4c51-90d5-7ab1222932ca">

#### Findings:
- **Global Reach:** Elist customers placed orders from 195 countries, with the United States contributing 47% of total sales.
- **Concentration of Sales:** The top 12 countries account for 80% of Elist's total sales, highlighting the importance of maintaining a strong presence in these markets.
- **High-AOV Countries:** After filtering for countries with 100 or more orders, 12 countries show an average order value (AOV) above $300. These countries represent 8% of total orders and 10% of total sales.

#### Recommendations:
- **Prioritize Top Markets:** Continue to focus on the top 12 countries driving 80% of sales, ensuring a strong presence and tailored strategies to maintain momentum, particularly in capturing retained value from 2020.
- **Explore High-AOV Markets:** Develop targeted efforts to penetrate the 12 high-AOV countries, leveraging consumer preferences for premium products to drive significant sales growth.
- **Market Analysis for Expansion:** Conduct in-depth analysis to identify similarities among countries, using these insights to pinpoint new market opportunities and refine global expansion strategies.


#### Loyalty Program

<img width="400" alt="Loyalty Program Comparison" src="https://github.com/user-attachments/assets/f43730e3-d160-435b-b393-a25c0ddb9bb9">
<img width="400" alt="Loyalty vs Non-Loyalty Orders" src="https://github.com/user-attachments/assets/4431eae5-a2ef-4f1e-9c53-9015b7379c1f">
<img width="400" alt="Loyalty vs Non-Loyalty Sales Forecast" src="https://github.com/user-attachments/assets/c2753bc7-ab27-4424-a6e6-49a148a16780">

#### Findings:
- **Loyalty Program Adoption and Performance:** The loyalty program, introduced in 2019, saw significant customer adoption beginning in early 2021. Since then, loyalty customers have consistently outperformed non-loyalty customers in sales and order count, a trend that has continued through 2022.
- **Higher AOV for Loyalty Customers:** In addition to higher order volumes, loyalty customers now have a greater average order value (AOV) compared to non-loyalty customers. This indicates that loyalty members are making not only more frequent purchases but also higher-value purchases.
- **Forecasted Growth for Loyalty Sales:** Based on current trends, loyalty sales are expected to continue outpacing non-loyalty sales in the foreseeable future, highlighting the growing effectiveness of the program.

#### Recommendations:
- **Sustain and Expand the Loyalty Program:** Continue to invest in and refine the loyalty program to maintain its positive trajectory and further boost loyalty customer engagement and revenue.
- **Increase Focus on Loyalty Customer Growth:** Prioritize initiatives that encourage more customers to join the loyalty program, leveraging its demonstrated ability to drive higher sales and order values.
- **Monitor and Enhance Effectiveness:** Regularly analyze the differences between loyalty and non-loyalty customer behaviors to identify opportunities for targeted improvements in program offerings and incentives.



#### Marketing Channels

<img width="500" alt="Marketing Channels" src="https://github.com/user-attachments/assets/29e9d65c-0c5b-49b1-ab13-c7c04253750a">
<img width="500" alt="Loyalty + Channel" src="https://github.com/user-attachments/assets/ad06dcd7-ef4a-459e-966c-849b7015ec01">

#### Findings:
- **Key Channels:** The **direct channel** is the most successful at acquiring customers (~84K) and generating loyalty signups (~32.9K) but has a moderate conversion rate to loyalty members (39%). The **email channel** ranks second in customer acquisition (~19K) and has the highest loyalty conversion rate (58%). 
- **Other Channels:** Despite its low number of orders (2,900) and low loyalty member conversion rate (16%), the **affiliate channel** achieves the highest average order value. The **social media channel** has a low number of orders (1,293) but demonstrates strong loyalty conversion performance (50%), second only to email marketing.
- **Data Gaps:** Marketing channels are unidentified for 85 "unknown" and 1,387 "blank" customers.

#### Recommendations:
- **Direct Channel:** Focus marketing efforts on promoting products to further leverage its large customer base. Deprioritize loyalty program marketing due to its relatively lower success in converting customers to loyalty members.
- **Email Channel:** Emphasize acquiring more customers while leveraging its high loyalty conversion rate to grow loyalty program participation.
- **Affiliate Channel:** Shift focus toward customer acquisition, capitalizing on its high average order value. Deprioritize loyalty program efforts for this channel due to its low loyalty conversion performance.
- **Social Media Channel:** Concentrate marketing efforts on acquiring more loyalty members, leveraging its strong loyalty conversion rate. Consider strategies to increase overall order volume for improved channel performance.


#### Refund Rates

<img width="500" alt="AOV and Refund Rate - Bar Graph" src="https://github.com/user-attachments/assets/6a04c540-c496-4361-8f10-631bfa304124">
<img width="500" alt="AOV and Refund Rate - Scatter Plot" src="https://github.com/user-attachments/assets/f00b746c-3551-4532-b713-b34082254550">
<img width="254" alt="Highest Refund Rate 5+ Orders" src="https://github.com/user-attachments/assets/4aad9df8-1088-4584-9f96-5c6517b47eb5">
<img width="254" alt="Highest Refund Rate 100+ Orders" src="https://github.com/user-attachments/assets/5a1620ec-811b-424f-a0ad-a5e3d7c532a0">

#### Findings:
- **High Refund Rates for Specific Laptops:** The ThinkPad Laptop has the highest refund rate at 12%, followed closely by the MacBook Air Laptop at 11%.
- **Correlation Between Average Order Value and Refund Rates:** A strong correlation (R-squared = 0.8843) exists, suggesting that higher-priced items are more likely to have higher refund rates.
- **Country-Specific Refund Trends:** Five countries with five or more orders have refund rates of at least 20%, despite their low order volumes. Eight countries with 100 or more orders have refund rates of at least 7%, indicating potential systemic issues.

#### Recommendations:
- **Investigate High Refund Rates for Laptops:** Conduct an in-depth analysis of the ThinkPad Laptop and MacBook Air Laptop to determine the root causes of their high refund rates. Implement targeted improvements to reduce refunds.
- **Monitor and Manage High-Value Product Refund Trends:** Develop strategies for mitigating refunds on high-priced items, such as better customer education, enhanced product descriptions, or stricter quality control. Regularly review the relationship between average order value and refund rates to ensure acceptable levels.
- **Address Country-Specific Refund Issues:** Analyze the countries with small order volumes and high refund rates to identify and address unique regional factors. For the countries with over 100 orders and refund rates of 7% or more, implement localized measures to reduce refund rates, such as improved logistics, better customer support, or tailored return policies.



#### Purchasing Platform

<img width="410" alt="Purchasing Platform" src="https://github.com/user-attachments/assets/a2d675c6-f169-4e95-bb5e-e59164b47479">
<img width="501" alt="Mobile App" src="https://github.com/user-attachments/assets/3cdc1095-a95b-4bba-aeaf-9abeead4a61b">

#### Findings:
- **Mobile App Performance:** Sales and order growth spiked in 2020 (114% increase in sales, 237% increase in orders) but slowed in 2021 (42% sales growth, 165% order growth) and declined significantly in 2022 (41% drop in sales, 39% drop in orders). The average order value (AOV) decreased steadily from $111 in 2019 to $36 in 2022, reflecting a shift toward smaller item purchases such as the Samsung Charging Cable Pack (351% growth in 2021) and the Samsung Webcam (128% growth in 2021).
- **Website Performance:** Total sales surged in 2020 (164% growth) but declined by 11% in 2021 and 46% in 2022, with order growth patterns varying. The website's AOV has generally increased, from $237 in 2019 to $294 in 2022, with fluctuations in between. Customers primarily use the website for purchasing higher-value items.
- **Customer Preferences:** Customers tend to purchase lower-value items on the mobile app and higher-value items on the website.

#### Recommendations:
- **Mobile App Strategy:** Focus marketing efforts on smaller, lower-value items that align with customer purchase behavior. Expand promotions and optimize the app for smaller, high-demand products to capitalize on this trend.
- **Website Strategy:** Emphasize high-value items in marketing campaigns to leverage the website’s alignment with these purchases. Ensure the website experience supports customers looking for premium or expensive items.
- **Cross-Channel Opportunity:** Use cross-promotion to encourage customers who browse on the app to complete higher-value purchases on the website. Consider encouraging mobile app users to explore higher-value items by promoting exclusive deals or bundles.


#### Shipping Times

<img width="410" alt="Delivery Metrics" src="https://github.com/user-attachments/assets/793e68cb-d825-43ca-ab14-6f7dad1f0e63">
<img width="239" alt="Refund Metrics" src="https://github.com/user-attachments/assets/fadb310a-e1e9-464c-bd30-5fcff29751f4">
<img width="254" alt="Most Days to Deliver" src="https://github.com/user-attachments/assets/5352bb06-e245-42f9-8206-51d17881856d">

#### Findings:
- **Refunds and Shipping/Delivery Times:** Analysis shows no discernible patterns linking refunds to shipping or delivery times. Refunds are independent of these factors, which is a positive outcome for the process.
- **Outliers in Shipping and Delivery Times:** Qatar and Taiwan exhibit unusually high days to ship and deliver, as illustrated in the scatter plot. In addition to Taiwan, seven other countries with 100 or more orders have average delivery times exceeding 8 days.

#### Recommendations:
- **Investigate Outliers:** Analyze the specific reasons for the extended shipping and delivery times in Qatar and Taiwan. Develop strategies to reduce these durations, such as identifying logistical bottlenecks or partnering with more efficient carriers.
- **Optimize Delivery Times for High-Order Countries:** For the countries with over 100 orders and delivery times averaging more than 8 days, conduct a deeper analysis to understand delays. Implement measures to streamline processes and improve delivery speed in these regions.













#### Operational Effectiveness

The general average time to ship (3 days) and deliver (14 days) across all regions has remained extremely consistent since 2019. However, without proper benchmarks it is unclear whether these figures fare well against competitors.
Loyalty members do not appear to receive faster delivery times, with time to deliver being equal with non-members (14 days).







## ERD
The entity relation diagram (ERD) can be found [here](https://github.com/JordanCWard/elist_analysis/blob/main/Elist_ERD.png).

# About the Data
Include file about data cleaning here
Include workbook for more analysis here
