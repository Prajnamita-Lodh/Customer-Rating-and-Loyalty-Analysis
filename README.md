# Customer-Rating-and-Loyalty-Analysis
Developed Power BI dashboard to track customer satisfaction, repeat purchase behavior, and loyalty patterns. Analyzed geographic purchase trends, satisfaction scores, and returning customer data to uncover retention drivers and regional engagement insights for leading U.S. retail chain OmniRetail throughout 2024.

## [View the Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNTU0NGMzODktZjQzZC00ZThhLTkwZjYtYjg1MWNiMjVkZmI5IiwidCI6IjQ2NTRiNmYxLTBlNDctNDU3OS1hOGExLTAyZmU5ZDk0M2M3YiIsImMiOjl9)

## Introductiion:
Customer satisfaction is the heartbeat of long-term success in retail — especially in a hybrid model like OmniRetail, where online and in-store experiences must align seamlessly.

This dashboard explores feedback collected throughout 2024 across OmniRetail’s customer touchpoints. By analyzing satisfaction scores alongside purchase behavior, support history, and demographic data, we gain a holistic view of customer sentiment and loyalty drivers.

From pinpointing service gaps to uncovering regional patterns and experience trends, the insights here aim to guide strategic decisions that enhance retention, drive repeat purchases, and elevate the overall customer experience.

## Problem Statement:
*Your mission is to create an analytical report that identifies the key factors influencing customer satisfaction and loyalty across different regions, customer demographics, and support experiences.*
#### *Key questions to guide your analysis:*

*What are the main factors contributing to high vs. low satisfaction scores?*
*Are certain customer segments (by age, gender, group) more loyal than others?*
*Which locations (cities or states) report consistently high or low satisfaction scores?*
*Does contacting customer support negatively impact satisfaction?*
*How do factors like “Price” or “Product Variety” influence customer loyalty?*
*Do repeat purchasers report higher satisfaction compared to one-time buyers?*
*Are there regional clusters of highly loyal or dissatisfied customers based on location data?*
*What is the relationship between loyalty level and satisfaction score?*
*Do specific demographic groups favor certain satisfaction factors (e.g., Packaging vs. Price)?*


## Files Included:

### Customer Satisfaction Dataset .xlsx:
Contains raw data with details on customer satisfaction, loyalty level, customer demography, etc.

### Customer Satisfaction Report .pbix:
Power BI report file with interactive dashboards and visualizations on satisfaction performance, regional insights, and customer demographics based on the dataset.

## Data Dictionary
| Column Name        | Description                                                                                  |
|--------------------|----------------------------------------------------------------------------------------------|
| Customer_ID        | Unique customer identifier (for internal use only)                                           |
| Group              | Customer classification: A, B, or C:<br>• Group A: High-frequency shoppers<br>• Group B: Moderate-frequency<br>• Group C: New or low-frequency |
| Satisfaction_Score | Customer’s rating of their experience (1 = very poor, 10 = excellent)                        |
| Age and Gender     | Demographic attributes                                                                       |
| Location           | City and State (e.g., Austin.TX), with Latitude and Longitude for geographic mapping         |
| Purchase_History   | Indicates if the customer has made purchases (Yes/No)                                        |
| Support_Contacted  | Whether the customer interacted with support                                                 |
| Loyalty_Level      | OmniRetail’s internal rating: Low / Medium / High loyalty                                    |
| Satisfaction_Factor| The main reason influencing the satisfaction score (e.g., Price, Product Variety, Packaging) |



## IT Helpdesk Support Dashboard Output
The Satisfaction Dashboard is built using responses from 120 customers and analyzes key satisfaction factors.
It offers actionable insights based on demographics, repeat behavior, purchase patterns, and loyalty trends.

### Customer Satisfaction Performance:
- The average customer satisfaction score is 5.35. Customer service needs attention to improve it.

- 13.33% of customers rated satisfaction as 1. This is the biggest red flag, as a large portion is not satisfied. A total of 25% of customers rated 1 and 2, which is "Very Poor". The shop needs to improve all satisfaction factors to raise the ratings.

- Customers love the "Packaging of products", as it is the highest-rated factor. On average, customers rated it 7.00, which is "Very Good". Price and product variant are the lowest-rated factors.

- High loyalty customers have an average satisfaction score of 5.65. Medium loyalty customers have 4.47, and low loyalty customers have 5.84. Attention should be given to medium-level customers, as dissatisfaction may be the reason for their Medium loyalty.

- San Antiano has the lowest customer count and the lowest average satisfaction score. This area needs additional strategy and support to grow.

#### Bottom line: The shop must focus on service improvement, pricing, and offerings to boost satisfaction—especially for medium-loyalty customers and weaker-performing regions like San Antiano.

### Customer Demographics:

1. Female customers (66) outnumber males (54), Female-to-male ratio is 0.82; indicating stronger engagement from women.

2. Customers aged 50–59 are the highest contributors, so they should be the focus of retention efforts.
3. Senior citizens (60–69) are the least active, showing limited interaction with support or shopping.
4. 46.67% of users contacted the Contract Support Team; 58.93% of them were female—females prefer guided assistance.
5. 40% are repeat customers with "Good" average satisfaction score (5.13); retention strategy is working. “Customer service” is the top satisfaction driver; this area must continue to be a core focus.
6. 57.5% of customers made the purchase successfully converts to sales.
7. Only 31% of users show high loyalty; loyalty-building initiatives need to be prioritized. Females aged 50–59 show the highest low loyalty rate - targeted loyalty programs required. Females aged 30–39 show the highest loyalty—this group can be used for advocacy and referral campaigns.

#### Bottom Line: Support quality is driving purchases and satisfaction, especially among females—but loyalty is weak in key age groups. It is suggested to double down on service consistency and launch targeted loyalty campaigns by age and gender.

### Regional Insights:

- Phoenix has the most repeated customer overall, while Texas (TX) leads among states. Consider targeting Phoenix and TX for customer loyalty programs or retention initiatives, as their repeat behavior indicates engagement.

- Los Angeles and Chicago top the chart for highly loyal customer distribution by city; Texas (TX) ranks highest by state. These cities/states are key loyalty hubs—offering exclusive benefits or faster service in these areas could further strengthen customer ties.

- Chicago customers have the highest satisfaction (avg. 6.36, rated "Good"), making it the most satisfied city. Illinois (IL) leads as the state with the most satisfied users. Maintain the service quality in Chicago and Illinois while using their service models to replicate success in lower-performing regions.

#### Bottom Line: Texas (TX) stood out with exceptional overall performance. Phoenix, Chicago, Los Angeles, Texas, and Illinois are strategic focus areas for loyalty, retention, and satisfaction-driven initiatives.




