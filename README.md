## to do


#### graphs/tables\
- once I've decided all the ones to use, put them in one sheet in excel then use theme to change all of them
- include various types
- don't repeat too often
- standardize colors, fonts, borders
- put them before or after info?
- remove gridlines

#### make sure that graphs are the best chosen for what the data is showing

#### rewrite current list of topics/titles better

#### fix sizing of headers

#### clean up excel file







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

#### Findings:

<img width="350" alt="Sales by Year" src="https://github.com/user-attachments/assets/905af2c4-9424-47ce-8048-c1644e0c5d20">

- **Revenue and Order Trends:** Between 2019 and 2022, $28 million in revenue was generated from more than 100,000 orders, with an average order value (AOV) of $260. The peak year was 2020, which saw the highest revenue ($10.2 million) and AOV ($300), likely due to increased pandemic-related spending. In contrast, 2021 recorded the highest number of orders (36,000).

<img width="500" alt="Seasonality" src="https://github.com/user-attachments/assets/e47024fc-952f-498e-a384-5f110f9b5650">

- **Seasonal Sales Patterns:** There is a holiday sales surge, with growth rates of 18% in November and 23% in December. This is followed by significant declines in January (-10%) and February (-25%), with a rebound of 18% in March. October sees potential sales stagnation as consumers may wait for holiday deals or shop elsewhere.
- **Consumer Behavior Insights:** The sales pattern aligns with typical electronics seasonality, with holiday promotions influencing consumer purchasing decisions. October’s lower activity highlights a potential opportunity to better engage customers before the holiday season.

#### Recommendations:
- **Maximize November and December Promotions:** Expand marketing campaigns starting in early November to capitalize on the surge in sales growth (18% in November and 23% in December). Highlight exclusive deals, limited-time offers, and bundle packages to drive urgency and boost AOV.
- **Retain Post-Holiday Shoppers:** Offer “New Year” incentives in January to mitigate the 10% sales decline, such as discount codes for future purchases or post-holiday clearance sales.
- **Optimize for March Rebound:** Prepare a focused campaign to harness the 18% sales rebound in March, potentially targeting customers who paused spending after the holiday season. Promote spring deals or “fresh start” themes tied to new product launches or upgrades.
- **Investigate Drop-off Causes:** Conduct customer surveys and study competitor trends to understand consumer behavior in October and other slower months. Test incentives (e.g., early-bird discounts, pre-holiday bundles) to encourage purchases before the “deal season” begins in November.


### Product Performance

#### Findings:

<img width="500" alt="Product Performance" src=https://github.com/user-attachments/assets/643e8dc7-8056-4bd5-a47a-02d70804d3ff>

- **Top Revenue Generator:** The 27-inch 4K Gaming Monitor is the highest revenue-generating product, contributing nearly $10 million (35% of total sales).
- **Popular Products by Order Volume:** Apple AirPods are the most popular product, accounting for 45% of all orders (48,000+ units).

<img width="343" alt="Product Performance Table" src="https://github.com/user-attachments/assets/5e2c905f-1f9c-4c04-96df-d8aa4f638344">

- **Key Revenue Drivers:** Four products—the 27-inch 4K Gaming Monitor, Apple AirPods, MacBook Air, and ThinkPad Laptops—together account for 96% of total revenue.
- **Samsung Charging Cable Pack:** This product constitutes 20% of orders but contributes only 2% of total sales, indicating room for optimization.

#### Recommendations:
- **Expand Product Catalog:** To diversify revenue streams, consider adding more products in the same categories as the top performers, focusing on in-class alternatives.
- **Optimize Samsung Charging Cable Pack Strategy:** Increase profitability by exploring price adjustments or introducing a bundled version of the product to capture additional value.


### Global Reach

#### Findings:

<img width="350" alt="Sales by Location" src="https://github.com/user-attachments/assets/9d40231b-97f8-42b2-b947-093f20e18e8c">

- **Global Reach:** Customers placed orders from 195 countries, with the United States contributing 47% of total sales.
- **Concentration of Sales:** The top 12 countries account for 80% of total sales, highlighting the importance of maintaining a strong presence in these markets.

<img width="400" alt="AOV over 300" src="https://github.com/user-attachments/assets/f69bec02-4c2c-4446-bf73-987dc0424f15">

- **High-AOV Countries:** After filtering for countries with 100 or more orders, 12 countries have an AOV above $300. These countries represent 8% of total orders and 10% of total sales.

#### Recommendations:
- **Prioritize Top Markets:** Continue to focus on the top 12 countries driving 80% of sales, ensuring a strong presence and tailored strategies to maintain momentum, particularly in capturing retained value from 2020.
- **Explore High-AOV Markets:** Develop targeted efforts to penetrate the 12 high-AOV countries, leveraging consumer preferences for premium products to drive significant sales growth.
- **Market Analysis for Expansion:** Conduct in-depth analysis to identify similarities among countries, using these insights to pinpoint new market opportunities and refine global expansion strategies.


#### Loyalty Program

#### Findings:
<img width="650" alt="Loyalty Program Comparison" src="https://github.com/user-attachments/assets/f43730e3-d160-435b-b393-a25c0ddb9bb9">

- **Loyalty Program Adoption and Performance:** The loyalty program, introduced in 2019, saw significant customer adoption beginning in early 2021. Since then, loyalty customers have consistently outperformed non-loyalty customers in sales and order count, a trend that has continued through 2022.
- **Higher AOV for Loyalty Customers:** In addition to higher order volumes, loyalty customers now have a greater average order value (AOV) compared to non-loyalty customers. This indicates that loyalty members are making not only more frequent purchases but also higher-value purchases.

<img width="500" alt="Loyalty vs Non-Loyalty Sales Forecast" src="https://github.com/user-attachments/assets/c2753bc7-ab27-4424-a6e6-49a148a16780">

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
- **Other Channels:** Despite its low number of orders (2,900) and low loyalty member conversion rate (16%), the **affiliate channel** achieves the highest AOV. The **social media channel** has a low number of orders (1,293) but demonstrates strong loyalty conversion performance (50%), second only to email marketing.
- **Data Gaps:** Marketing channels are unidentified for 85 "unknown" and 1,387 "blank" customers.

#### Recommendations:
- **Direct Channel:** Focus marketing efforts on promoting products to further leverage its large customer base. Deprioritize loyalty program marketing due to its relatively lower success in converting customers to loyalty members.
- **Email Channel:** Emphasize acquiring more customers while leveraging its high loyalty conversion rate to grow loyalty program participation.
- **Affiliate Channel:** Shift focus toward customer acquisition, capitalizing on its high AOV. Deprioritize loyalty program efforts for this channel due to its low loyalty conversion performance.
- **Social Media Channel:** Concentrate marketing efforts on acquiring more loyalty members, leveraging its strong loyalty conversion rate. Consider strategies to increase overall order volume for improved channel performance.


#### Refund Rates

<img width="500" alt="AOV and Refund Rate - Bar Graph" src="https://github.com/user-attachments/assets/6a04c540-c496-4361-8f10-631bfa304124">
<img width="500" alt="AOV and Refund Rate - Scatter Plot" src="https://github.com/user-attachments/assets/f00b746c-3551-4532-b713-b34082254550">
<img width="206" alt="Highest Refund Rate 10+ Orders" src="https://github.com/user-attachments/assets/8e4399ed-f49d-4eab-9de0-e71468456354">
<img width="215" alt="Highest Refund Rate 100+ Orders" src="https://github.com/user-attachments/assets/784cac26-8065-4933-90bd-8116275663bc">


#### Findings:
- **High Refund Rates for Specific Laptops:** The ThinkPad Laptop has the highest refund rate at 12%, followed closely by the MacBook Air Laptop at 11%.
- **Correlation Between AOV and Refund Rates:** A strong correlation (R-squared = 0.8843) exists, suggesting that higher-priced items are more likely to have higher refund rates.
- **Country-Specific Refund Trends:** Five countries with five or more orders have refund rates of at least 20%, despite their low order volumes. Eight countries with 100 or more orders have refund rates of at least 7%, indicating potential systemic issues.

#### Recommendations:
- **Investigate High Refund Rates for Laptops:** Conduct an in-depth analysis of the ThinkPad Laptop and MacBook Air Laptop to determine the root causes of their high refund rates. Implement targeted improvements to reduce refunds.
- **Monitor and Manage High-Value Product Refund Trends:** Develop strategies for mitigating refunds on high-priced items, such as better customer education, enhanced product descriptions, or stricter quality control. Regularly review the relationship between AOV and refund rates to ensure acceptable levels.
- **Address Country-Specific Refund Issues:** Analyze the countries with small order volumes and high refund rates to identify and address unique regional factors. For the countries with over 100 orders and refund rates of 7% or more, implement localized measures to reduce refund rates, such as improved logistics, better customer support, or tailored return policies.



#### Purchasing Platform

<img width="410" alt="Purchasing Platform" src="https://github.com/user-attachments/assets/a2d675c6-f169-4e95-bb5e-e59164b47479">
<img width="501" alt="Mobile App" src="https://github.com/user-attachments/assets/3cdc1095-a95b-4bba-aeaf-9abeead4a61b">

#### Findings:
- **Mobile App Performance:** Sales and order growth spiked in 2020 (114% increase in sales, 237% increase in orders) but slowed in 2021 (42% sales growth, 165% order growth) and declined significantly in 2022 (41% drop in sales, 39% drop in orders). The AOV decreased steadily from $111 in 2019 to $36 in 2022, reflecting a shift toward smaller item purchases such as the Samsung Charging Cable Pack (351% growth in 2021) and the Samsung Webcam (128% growth in 2021).
- **Website Performance:** Total sales surged in 2020 (164% growth) but declined by 11% in 2021 and 46% in 2022, with order growth patterns varying. The website's AOV has generally increased, from $237 in 2019 to $294 in 2022, with fluctuations in between. Customers primarily use the website for purchasing higher-value items.
- **Customer Preferences:** Customers tend to purchase lower-value items on the mobile app and higher-value items on the website.

#### Recommendations:
- **Mobile App Strategy:** Focus marketing efforts on smaller, lower-value items that align with customer purchase behavior. Expand promotions and optimize the app for smaller, high-demand products to capitalize on this trend.
- **Website Strategy:** Emphasize high-value items in marketing campaigns to leverage the website’s alignment with these purchases. Ensure the website experience supports customers looking for premium or expensive items.
- **Cross-Channel Opportunity:** Use cross-promotion to encourage customers who browse on the app to complete higher-value purchases on the website. Consider encouraging mobile app users to explore higher-value items by promoting exclusive deals or bundles.





#### Shipping Times

<img width="198" alt="Shipping Logistics" src="https://github.com/user-attachments/assets/3ab16e75-b982-4367-ab31-89c9b2743bf0">
<img width="220" alt="Refund Metrics" src="https://github.com/user-attachments/assets/bb0af87c-c328-4ae1-b5ce-4121d821f16e">

#### Findings:
- **Outliers in Orders:** Out of 108,124 orders, 41 outliers were identified. 18 orders have shipping dates that precede the purchase date. 23 orders exhibit abnormally long shipping times, ranging from 25 to 1297 days. These outliers represent a small fraction of the dataset and warrant separate analysis to uncover potential data quality issues, specifically related to the purchase date column.
- **Shipping and Delivery Times** After excluding the 41 outliers, shipping times range from 1 to 3 days with an average of 2 days and delivery times range from 5 to 10 days with an average of 7.5 days.
- **Refund Analysis:** The refund rate shows no correlation with shipping or delivery times, indicating that customers are not requesting refunds due to delays in shipping or delivery.

#### Recommendations:
- **Addressing Outliers:** Investigate the purchase date column for the 18 orders with shipping dates preceding purchase dates to identify and correct data entry or system errors. Analyze the 23 orders with extended shipping times to determine their root cause and assess if system improvements are necessary.
- **Data Quality Improvements:** Implement validation checks to prevent shipping dates from being earlier than purchase dates in future data entries. Set acceptable thresholds for shipping durations and develop alert systems to flag unusually long shipping times.
- **Ongoing Monitoring:** Continue monitoring the refund process to ensure it remains independent of shipping and delivery performance. Periodically review and audit the data for consistency and accuracy to maintain its reliability.





## ERD
The entity relation diagram (ERD) can be found [here](https://github.com/JordanCWard/elist_analysis/blob/main/Elist_ERD.png).

# About the Data
Include file about data cleaning here
Include workbook for more analysis here
