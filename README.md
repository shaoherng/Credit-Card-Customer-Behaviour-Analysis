# Credit-Card-Customer-Behaviour-Analysis

## Type of views in Power BI
1. Customer Segmentation
2. Credit Risk Assessment
3. Customer Attrition and Retention

### Customer Segmentation
1

### Credit Risk Assessment
1. Credit limit
2. Total Revolving balance
3. Average utilization ratio
4. Number of months in the bank
5. Card category
6. Income category
7. Total transaction amount
8. Total transaction count
9. Total credit utilization ratio = total revolving balance / credit limit
10. Total spending amount to income ratio = (total transaction amount / income category midpoint) * 100
11. Impact of demographics on credit risk (slicer on age, education level, marital status)
12. Proportion of attrited customers in high credit risk
    
### Customer Attrition and Retention
1. Attrition rate
2. Everything else

### Dashboard Design
![image](https://github.com/user-attachments/assets/285e2913-1587-4582-aa7f-7a0a690c7888)
![image](https://github.com/user-attachments/assets/b7eae210-c07c-4f65-88e6-4df70214c46d)

The dataset appears to be related to bank customers and includes various customer attributes such as age, gender, marital status, education, income category, and credit-related features, along with indicators for customer attrition ("churn"). Here are the key columns:

- **CLIENTNUM**: A unique identifier for each customer.
- **Attrition_Flag**: Indicates whether the customer is an "Existing Customer" or an "Attrited Customer."
- **Customer_Age**: The age of the customer.
- **Gender**: Gender of the customer.
- **Dependent_count**: Number of dependents.
- **Education_Level**: Educational background.
- **Marital_Status**: Marital status of the customer.
- **Income_Category**: Customer's income range.
- **Card_Category**: The category of the credit card the customer uses.
- **Months_on_book**: Number of months the customer has been with the bank.
- **Credit_Limit**: The total credit limit available to the customer.
- **Total_Revolving_Bal**: The customer's total revolving balance.
- **Avg_Open_To_Buy**: Average available credit for the customer.
- **Total_Trans_Amt**: Total transaction amount.
- **Total_Trans_Ct**: Total transaction count.
- **Avg_Utilization_Ratio**: The ratio of the credit used by the customer relative to their credit limit.

Given this dataset, we can generate insights related to:

1. **Attrition Patterns**: Analyze the factors that correlate with customer churn, such as age, income category, card category, or transaction activity.
2. **Customer Segmentation**: We can group customers based on attributes like income, credit usage, or transaction behavior to identify different customer segments.
3. **Credit and Spending Behavior**: Explore relationships between credit limit, revolving balances, and transaction activity.
4. **Customer Demographics**: Insights based on demographic characteristics like gender, education, and marital status.
  
I will now start by analyzing some of these patterns, particularly focusing on customer attrition and demographic factors.

From the summary and data inspection, we can derive the following key points:

1. **Customer Demographics**:
   - The average customer age is around 46 years, with ages ranging from 26 to 73.
   - Gender distribution: More than half (around 53%) of the customers are female.
   - Marital status: About 46% of the customers are married.
   - Education: The most common education level is "Graduate" (around 31%).
   - Income: The most common income category is "Less than $40K" (about 35%).

2. **Attrition**:
   - About 16% (1,627 out of 10,127) of the customers are labeled as "Attrited Customer," with the rest being "Existing Customers."

3. **Financial Behavior**:
   - The average credit limit is around $8,000, with some customers having limits as high as $34,000.
   - Many customers have a low revolving balance, with some customers having zero balance.
   - The average utilization ratio is around 0.27, indicating that most customers are using less than a third of their available credit.

4. **Transaction Activity**:
   - The total transaction amounts and transaction counts vary significantly, with the average customer making 60 transactions per year and spending a significant amount.

Since there are no missing values in the dataset, we can now dive into more detailed analyses, such as understanding the factors affecting customer attrition. Let's begin by looking at the differences between existing and attrited customers.

The comparison between **Attrited Customers** and **Existing Customers** shows some notable differences in key financial behaviors:

1. **Customer Age**: Attrited customers are slightly older on average (46.66 years) compared to existing customers (46.26 years), though the difference is minimal.

2. **Credit Limit**: Attrited customers tend to have lower average credit limits (\$8,136) compared to existing customers (\$8,727).

3. **Revolving Balance**: Attrited customers have a significantly lower average total revolving balance (\$673) compared to existing customers (\$1,257), which could suggest that they are using less of their available credit before leaving.

4. **Transaction Amount and Count**: Attrited customers tend to have lower transaction amounts (\$3,095) and fewer transactions (44 transactions on average) compared to existing customers, who have higher transaction amounts (\$4,655) and 69 transactions per year on average. This indicates that attrited customers are less engaged with their accounts.

5. **Utilization Ratio**: Attrited customers have a lower average credit utilization ratio (16%) compared to existing customers (29%), meaning they use less of their available credit.

These differences suggest that **attrited customers generally have lower engagement** in terms of credit usage and transaction activity, which could be key indicators of potential attrition. Further analysis could be done to identify specific thresholds for these metrics that might help predict future attrition.
