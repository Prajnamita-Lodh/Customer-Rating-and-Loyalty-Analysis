# Customer Rating and Loyalty-Analysis
Developed Power BI dashboard to track customer satisfaction, repeat purchase behavior, and loyalty patterns. Analyzed geographic purchase trends, satisfaction scores, and returning customer data to uncover retention drivers and regional engagement insights for leading U.S. retail chain OmniRetail throughout 2024.

## [View the Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNTU0NGMzODktZjQzZC00ZThhLTkwZjYtYjg1MWNiMjVkZmI5IiwidCI6IjQ2NTRiNmYxLTBlNDctNDU3OS1hOGExLTAyZmU5ZDk0M2M3YiIsImMiOjl9)
<img width="720" height="1280" alt="Image" src="https://github.com/user-attachments/assets/4cb637e4-f8b6-49b2-933d-78b418f2e01f" />

## Introductiion:
Customer satisfaction is the heartbeat of long-term success in retail — especially in a hybrid model like OmniRetail, where online and in-store experiences must align seamlessly.

This dashboard explores feedback collected throughout 2024 across OmniRetail’s customer touchpoints. By analyzing satisfaction scores alongside purchase behavior, support history, and demographic data, we gain a holistic view of customer sentiment and loyalty drivers.

From pinpointing service gaps to uncovering regional patterns and experience trends, the insights here aim to guide strategic decisions that enhance retention, drive repeat purchases, and elevate the overall customer experience.

## Problem Statement:
*Your mission is to create an analytical report that identifies the key factors influencing customer satisfaction and loyalty across different regions, customer demographics, and support experiences.*
#### *Key questions to guide your analysis:*

*a) What are the main factors contributing to high vs. low satisfaction scores?*

*b) Are certain customer segments (by age, gender, group) more loyal than others?*

*c)  Locations (cities or states) report consistently high or low satisfaction scores?*

*d) Does contacting customer support negatively impact satisfaction?*

*e) How do factors like “Price” or “Product Variety” influence customer loyalty?*

*f) Do repeat purchasers report higher satisfaction compared to one-time buyers?*

*g) Are there regional clusters of highly loyal or dissatisfied customers based on location data?*

*h) What is the relationship between loyalty level and satisfaction score?*

*i) Do specific demographic groups favor certain satisfaction factors (e.g., Packaging vs. Price)?*


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

- Female customers (66) outnumber males (54), Female-to-male ratio is 0.82; indicating stronger engagement from women.

- Customers aged 50–59 are the highest contributors, so they should be the focus of retention efforts.
- Senior citizens (60–69) are the least active, showing limited interaction with support or shopping.
- 46.67% of users contacted the Contract Support Team; 58.93% of them were female—females prefer guided assistance.
- 40% are repeat customers with "Good" average satisfaction score (5.13); retention strategy is working. “Customer service” is the top satisfaction driver; this area must continue to be a core focus.
- 57.5% of customers made the purchase successfully converts to sales.
- Only 31% of users show high loyalty; loyalty-building initiatives need to be prioritized. Females aged 50–59 show the highest low loyalty rate - targeted loyalty programs required. Females aged 30–39 show the highest loyalty—this group can be used for advocacy and referral campaigns.

#### Bottom Line: Support quality is driving purchases and satisfaction, especially among females—but loyalty is weak in key age groups. It is suggested to double down on service consistency and launch targeted loyalty campaigns by age and gender.

### Regional Insights:

- Phoenix has the most repeated customer overall, while Texas (TX) leads among states. Consider targeting Phoenix and TX for customer loyalty programs or retention initiatives, as their repeat behavior indicates engagement.

- Los Angeles and Chicago top the chart for highly loyal customer distribution by city; Texas (TX) ranks highest by state. These cities/states are key loyalty hubs—offering exclusive benefits or faster service in these areas could further strengthen customer ties.

- Chicago customers have the highest satisfaction (avg. 6.36, rated "Good"), making it the most satisfied city. Illinois (IL) leads as the state with the most satisfied users. Maintain the service quality in Chicago and Illinois while using their service models to replicate success in lower-performing regions.

#### Bottom Line: Texas (TX) stood out with exceptional overall performance. Phoenix, Chicago, Los Angeles, Texas, and Illinois are strategic focus areas for loyalty, retention, and satisfaction-driven initiatives.


## Step Followed

- Step 1 : Load data into Power BI Desktop, the dataset is a .xlsx file.

- Step 2 : Open Power Query Editor & in the View tab under the Data Preview section, check "column distribution", "column quality," & "column profile" options.

- Step 3 : Also, since by default, the profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".

- Step 4 : It was observed that in none of the columns, errors & empty values were present.

- Step 5 : To establish a more informative and insightful dashboard, a few columns are added in Power Query to this dataset.

     *A.* To segment customers based on their engagement frequency, a new column Customer Classification Group was created using a conditional logic applied to the existing Group column. 
     Here is the condition -
     - If the value in the Group column is A, then the output is High frequency Shopper.
    - If the value is B, then the output is Medium frequency Shopper.
    - If the value is C, then the output is New frequency Shopper.

    <img width="878" height="278" alt="Image" src="https://github.com/user-attachments/assets/3e784b1c-a140-4c99-95cc-0de30d62810e" />

    *B.* In the raw dataset, city and state information were combined into a single column, separated by a period (.) delimiter.To make the data more structured and analysis-ready, I used the Split Column by Delimiter feature in Power Query. As a result, two separate columns — City and State — were created. 

    <img width="334" height="425" alt="Image" src="https://github.com/user-attachments/assets/02ebd7c8-f954-4bbd-ab03-638cbea4d49a" />

    *C.* To estimate the Birth Year of each customer, a new calculated column was created using the reference year 2024. 

        Birth Year = 2024 - [Age]

    <img width="441" height="185" alt="Image" src="https://github.com/user-attachments/assets/523a4ca5-cc1f-493a-b9a5-24f78d25184c" />

    *D.* To segment customers based on their generation, a new column, Generation, was created using a conditional logic applied to the existing Birth Year column. Here is the condition –
  - If the value in the Birth Year column is 1964, then the output is Baby Boomer.
  - If the value is less than or equal to 1965, then the output is Generation X.
  - If the value is 1980, then the output is Millennials.
  - If the value is less than or equal to 1994, then the output is Millennials.
  - If the value is greater than or equal to 1995, then the output is Millennials.

    <img width="837" height="366" alt="Image" src="https://github.com/user-attachments/assets/d6bdedad-b1fc-490e-9d3b-f8a2f6f5c2cc" />

  *E.* To segment customers based on their Satisfaction Score, a new column, Satisfaction Status, was created using conditional logic applied to the existing Satisfaction Score column. Here is the condition –
    
    - If the Satisfaction Score is between 1 and 2.99, then the output is Very Poor.
    - If the score is between 3 and 4.99, then the output is Average.
    - If the score is between 5 and 6.99, then the output is Good.
    - If the score is between 7 and 8.99, then the output is Very Good.
    - If the score is between 9 and 10, then the output is Excellent.

- Step 6 : Applied the transformation in Power Query and closed it to load the data into Power BI for building the Customer Satisfaction Dashboard.

### Page Set up:

- Step 7 : To organise the report, at first text box is inseted in the report to write the TITLE of the page. Name the report as "Customer Insight".

- Step 8 : In the report view, under the insert tab, using image option, company's logo was added to the report design area at the left corner. Also added the "Home" action button for navigation. Here is visual outcome:

  <img width="411" height="164" alt="Image" src="https://github.com/user-attachments/assets/1349f9b1-54df-4c69-9a39-da7cad1aaee9" />

- Step 9 : "Filter" button is included to allow users to slice the data dynamically, and a "Reset" action button is added to clear all applied filters at once.

   <img width="105" height="138" alt="Image" src="https://github.com/user-attachments/assets/498b67b2-6b00-4473-bb82-8b0cbf9917ce" />

- Step 10 : In order to navigate the report add the another three "Action" button as "Customer Satisfaction", "Loyalty Level", and "Customer Demography" horizontally.

   <img width="432" height="226" alt="Image" src="https://github.com/user-attachments/assets/31d2dad8-ed4a-4707-9bef-effc1d53746b" />

- Step 11 : Make the duplicate of the page for three times to create the separate Canvas for each part.

### Creating Measure Table:
To develop a dynamic Power BI report on Customer Satisfaction and Loyalty dashboard, I created a dedicated Measure Table to organize and centralize all the key DAX measures at one place. For creating a new Measures table, the following DAX expression was written;

    MeasuresTable = 
    SELECTCOLUMNS(
          FILTER(
            { (1) },
            FALSE()
          ),
        "Measure", [Value]
    )

#### *Step 12 : Used DAX expression in Measures Table*

1. To calculate *"Average Satisfaction Score"*:

        Average Satisfaction Score = AVERAGE(Data[Satisfaction_Score])

2. To count the *"Total Customer"*:

       Total Customer = COUNTROWS(Data)

3. To count the customer on the basis of the customer:

        A.  Male Customer = 
            CALCULATE
                (COUNTROWS(Data), Data[Gender] = "Male")

        B.  Female Customer = 
            CALCULATE
                (COUNTROWS(Data), Data[Gender] = "Female")

        C. Male and Female Ratio = 
            DIVIDE([Male Customer], [Female Customer])

4. To count the *"High Loyalty Customer"*:

        High Loyalty Customer (%) = DIVIDE(CALCULATE(COUNTROWS(Data), Data[Loyalty_Level] = "High"), [Total Customer])

5. To count the *"Support Contact Rate"*:

        Support Contact Rate = DIVIDE(CALCULATE(COUNTROWS(FILTER(Data, Data[Support_Contacted]="Yes"))),[Total Customer])

6. To calculate the *"Satisfaction Status"*:

        Satisfaction Status = SWITCH( TRUE(),
            [Average Satisfaction Score] >= 1 && [Average Satisfaction Score] <= 2.99, "Very Poor",
            [Average Satisfaction Score] >= 3 && [Average Satisfaction Score] <= 4.99, "Average",
            [Average Satisfaction Score] >= 5 && [Average Satisfaction Score] <= 6.99, "Good",
            [Average Satisfaction Score] >= 7 && [Average Satisfaction Score] <= 8.99, "Very Good",
            [Average Satisfaction Score] >= 9 && [Average Satisfaction Score] <= 10, "Excellent", 
            "Unknown")

7. To create the dynamic *"Satisfaction Status Color"*:

        Satisfaction Status Color Indication = 
            SWITCH(
            TRUE(),
        [Satisfaction Status] = "Very Poor" , "#FF3B2D", // Red
        [Satisfaction Status] = "Average" , "#FFAF28", // Orange
        [Satisfaction Status] = "Good" , "#F5E100", // Yellow
        [Satisfaction Status] = "Very Good" , "#ACE552", // Green
        [Satisfaction Status] = "Excellent" , "#77D046", // Dark Green
        "#616569")

8. To calculate *"% of Repeat Customer"*:

       % of Repeat Customer = 
          DIVIDE(CALCULATE(COUNTROWS(Data), Data[Customer Classification Group]= "High-frequency shopper"), [Total Customer],0)



   
## Recommendations for Business Improvement Based on Customer Satisfaction Insights

- #### Smaller Packs, Bigger Impact:

    Analysis shows that customers are price-sensitive and expect a wider variety of flavors, sizes, and product types. To improve satisfaction and drive sales, it is recommended to launch smaller, budget-friendly product packs and ensure consistent availability of products across multiple price points.

- #### Unhappy Customers, Untapped Insights

    Around 52% of customers rated their satisfaction between 1 and 5, and notably, 25% gave the lowest scores (1 or 2) in the CSAT survey. This indicates a significant portion of dissatisfied customers. However, it’s observed that customers who interacted with support team, to give higher satisfaction ratings. To improve overall satisfaction and reduce negative feedback, it’s recommended to proactively reach out to low-scoring customers to understand their concerns, address service gaps, and refine support processes accordingly to drive business growth.

- #### Support Drives Repeat Business:

    The Support team plays a critical role in enhancing customer satisfaction and loyalty. Analysis shows that nearly 50% of customers who made a purchase also contacted the support team, highlighting how essential support interactions are in the overall customer journey. Among these, 39% were repeat customers, indicating that positive support experiences are strongly linked to repeat business. To strengthen this impact, it is recommended to assign additional resources to the support function—this could include staffing, training, or process improvements—to ensure faster response times, better issue resolution, and ultimately, greater customer satisfaction and business success.

- #### Young Buyers, Big Potential:

    The 20–29 age group demonstrates high potential to drive business success, with 69.23% of customers in this group having contacted support, resulting in a 53.58% purchase rate and a 46% loyalty level. This highlights that support interactions play a key role in building customer loyalty. However, the overall customer count in this age segment remains low. To strengthen performance in this area, it is recommended to launch targeted digital marketing campaigns and offer exclusive discounts (both online and in-store) to attract more customers from this age group and increase their purchase activity.

- #### Mid-Age Shoppers, Strongest Spenders:

    The 40–49 age group shows the highest purchase rate at 64.52%, making them a key revenue-driving segment. To capitalize on this, it's recommended to offer targeted promotional codes to this group to encourage continued purchases. Additionally, introducing a loyalty program can help convert one-time buyers into repeat customers, boosting retention and long-term revenue growth for the store.

- #### San Antonio Needs a Local Touch: 

    Focus on San Antonio for improvement, as it shows the lowest satisfaction score and repeat customer rate—consider cultural sensitivity as a factor, and collaborate with local partners to apply successful strategies used in top-performing cities like Chicago.

- #### Arizona: Low Buzz, High Opportunity:

    The dashboard reveals that customer volume in Arizona is low, and those who do purchase report lower satisfaction levels. To address this, a customer loyalty program can be introduced to encourage repeat engagement. Additionally, expanding the support team’s outreach efforts in this region can help directly resolve issues, improve customer experience, and build trust with the brand.

- #### New York: Great Start, Weak Follow-Up:

    Despite a healthy volume of first-time customers in New York, the repeat purchase rate is low. To improve customer retention, it's recommended to implement a “discount on next purchase” scheme. This incentive can nudge first-time buyers to return, increasing customer lifetime value and strengthening brand loyalty in a competitive market.

  ## Snapshot of Customer Satisfaction Performance::

<img width="955" height="534" alt="Image" src="https://github.com/user-attachments/assets/aece5972-0ca2-4903-85b6-edd1e5b377ef" />

## Snapshot of Customer Demographics:

<img width="955" height="537" alt="Image" src="https://github.com/user-attachments/assets/e3091540-d5f9-4dce-87b8-294c9d89e434" />

## Snapshot of Regional Insights:

<img width="953" height="536" alt="Image" src="https://github.com/user-attachments/assets/c8a4fb1d-ef6c-422d-88b0-260959558296" />


<img width="956" height="536" alt="Image" src="https://github.com/user-attachments/assets/262902a5-c869-43a5-83ff-4b9d4bfd5f60" />
