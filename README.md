## <div align='center'> <h1> BANK CUSTOMER CHURN ANALYSIS </div>

**Tool Used: Excel, Power BI**

**[Dataset Used](https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn)**

**Power BI Dashboard: [Click to view](https://github.com/Weefred/Bank_Customer_Churn_Analysis/blob/main/Bank_customer_churn_dashboard.png)**

**Power BI Dashboard: [Click to interact](https://app.powerbi.com/view?r=eyJrIjoiZTgwNWZlMWEtMGVkMC00MmE0LWEyZTctMGE0NzBkMWRlOGMzIiwidCI6IjI3MGRhZWVlLTdkMWYtNDQwZC1hMDYxLTQzOWMzMGFhYjUwMSJ9)**

## About this project

This project focuses on analyzing bank customer churn to identify key factors contributing to customer attrition. By examining various customer attributes, the analysis aims to uncover patterns and trends that lead to churn. The insights derived from this project will help the bank develop targeted strategies to enhance customer engagement, improve satisfaction, and ultimately reduce churn rates. 

![imange](https://github.com/Weefred/Bank_Customer_Churn_Analysis/blob/main/Bank_customer_churn_dashboard.png)

## Business Problem

The bank is experiencing a high rate of customer churn, with a significant portion of its clientele leaving for competitors. This attrition negatively impacts revenue and growth.

## Applied Steps

1.	**Extract**: The dataset for this project was sourced from Kaggle. It consists of 18 columns and 10,001 rows. The data was imported into Power Query Editor for cleaning and transformation.

2.	**Data Cleaning**: The data was checked for duplicates, missing values etc.

3.	**Transformation**: The appropriate data types were used, and the following new columns were created using conditional columns to make for better analysis:

- Credit Score Category
- Age group
- Tenure with bank 

Three new measures ‘Total Customers’, ’Churned’ and ‘Stayed’ were created to find out the total number of customers the bank has, number of those who have left and those still with the bank, using the formula.

                    Total Customers = COUNTROWS('Customer-Churn-Records') 

                    Churned = COUNTROWS(FILTER('Customer-Churn-Records', 'Customer-Churn-Records'[Has Exited]  ="Yes"))
 
                    Stayed = COUNTROWS(FILTER('Customer-Churn-Records', 'Customer-Churn-Records'[Has Exited]  ="No"))

4.	**Data Visualization**: Data was loaded into Power BI to create interactive dashboards and generate insights.
 
## Insights

1.	Customers with lower credit scores are more likely to churn possibly due to limited access to financial products, financial instability etc.

2.	Clients with credit cards have a higher churn rate compared to those who do not. Potential factors could include dissatisfaction with credit card terms, fees etc.

3.	Non-active customers have a higher churn rate. This suggests that they may feel disconnected or undervalued. 

4.	Customers from Germany and France exhibit the highest churn rate while those from Spain have the lowest.

5.	Customers who have spent 6-8 years with the bank have the highest churn rate. This suggests that mid-tenure customers may experience diminishing satisfaction or unmet expectations over time.

## Recommendations

1.	For customers with lower credit scores, offer services such as financial counseling, loyalty programs and credit score improvement incentives such as reduced interest rates for those that show positive financial behaviors.

2.	Improve credit card offerings and offer better customer support to retain customers with credit cards.

3.	To retain non-active customers, consider engagement campaigns, regular communication and feedback, bundle offers etc.

4.	Study the CRM strategies used in Spain and implement similar techniques in Germany and France to enhance customer retention.

5.	Implement enhanced loyalty programs for long and mid-term customers including special offers and benefits. 

6.	Implement regular feedback mechanisms to capture and address any issues or concerns early.
