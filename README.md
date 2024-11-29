## to do

<br>
<br>
<br>
<br>
<br>

#### Use this somewhere in the future sections
regression analysis
Excel's Data Analysis tool
- Use Excel's Forecast.Linear or Forecast.ETS functions for basic predictive modeling.

- Build a simple linear regression model to predict sales:
- X-axis: Time (e.g., months).
- Y-axis: Sales (total sales or per product).


#### marketing channels
- clean up findings
- write recommendation

#### refund rates
- rewrite findings to be more beneficial for stakeholders
- clean up recommendation

#### purchasing platform
- rewrite findings to be more beneficial for stakeholders
- clean up recommendation

#### Time to deliver
- are there any trends
- shipping times
- trends with refunds vs non-refunds?

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

- **Findings:** The direct marketing channel has the highest number of loyalty participants: 32.9K signups (39% signup rate). The email marketing channel has the highest average signup rate: 58% signup rate (~10.8K signups). The affiliate marketing channel has the lowest average signup rate: 16% signup rate (~500 signups). Based on this information, more money should be spent on the email marketing channel and less spent on the affiliate marketing channel. Money should continue to be spent on the direct marketing channel even though the signup rate isn't the highest because the number of signups are still very high.

The direct marketing channel has been the most successful for the number of orders each year. However, the affiliate marketing channel has steadily had the highest average order value each year and should be pursued further. Email marketing channel has consistently had the lowest number of orders and average order value, so less marketing should be spent here.

Need to identify the marketing channels for 85 unknown and 1387 blank customers.

Due to this concerning recent trend in the loyalty program, DotDash should cut affiliate channel marketing efforts and focus efforts on reaching customers through the direct and email channels. These channels have led to the most signups and have a significant signup rate:

Direct Marketing Channel: 40% signup rate | 23.5K signups
Email Marketing Channel: 59% signup rate | 8K signups

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

#### Purchasing Platform

- **Findings:** Both the mobile app and the website saw a significant increase in total sales and orders in 2020. This is inline with the other data. One other significant point is that the mobile app had a 165% increase in orders in 2021 and the website had a decrease of 11%. This increase in mobile app orders came from the Samsung Charging Cable Pack (351% increase) and the Samsung Webcam (128% increase).
- **Recommendation:** This suggests that it might be worth focusing the mobile app on smaller purchases whereas the website should focus on larger purchases.

<img width="410" alt="Purchasing Platform" src="https://github.com/user-attachments/assets/dedbe4e3-e4b7-4dee-958e-913dc6691d51">

<img width="501" alt="Mobile App" src="https://github.com/user-attachments/assets/a4d961ad-6a5b-4ee4-a052-4f069a3f6ff5">


#### Operational Effectiveness

The general average time to ship (3 days) and deliver (14 days) across all regions has remained extremely consistent since 2019. However, without proper benchmarks it is unclear whether these figures fare well against competitors.
Loyalty members do not appear to receive faster delivery times, with time to deliver being equal with non-members (14 days).







## ERD
The entity relation diagram (ERD) can be found [here](https://github.com/JordanCWard/elist_analysis/blob/main/Elist_ERD.png).

# About the Data
Include file about data cleaning here
Include workbook for more analysis here
