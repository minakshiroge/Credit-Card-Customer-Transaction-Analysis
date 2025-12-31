# Credit-Card-Customer-Transaction-Analysis
This project includes Credit Card analysis, dashboards and insights using Power BI.

## Project Objective
This project analyzes credit card customer demographics and transaction behavior to generate actionable business insights.  The analysis focuses on revenue trends, customer segmentation, card performance

# Key Insights
WoW change:
•	Revenue increased by 28.8%,
•	Total Transaction Amt & Count increased by xx% & xx%
•	Customer count increased by xx%
Overview YTD:
•	Overall revenue is 55M
•	Total interest is 8M
•	Total transaction amount is 45M
•	Male customers are contributing more in revenue 31M, female 26M
•	Blue & Silver credit card are contributing to 93% of overall transactions
•	TX, NY & CA is contributing to 68%
•	Overall Activation rate is 57.5%
•	Overall Delinquent rate is 6.09%


# Recommendations to Improve Credit Card Transactions
Promote digital and chip-based payments to increase transaction efficiency.
Use customer segmentation (age, income, card category) to offer targeted promotions.
Introduce early-activation and category-based offers to boost transaction frequency and revenue.

# Dataset Overview
1️⃣ Customer Table (10,109 rows)
- Client_Num
- Customer_Age
- Gender
- Dependent_Count
- Education_Level
- Marital_Status
- State_cd
- Zipcode
- Car_Owner
- House_Owner
- Personal_Loan
- Contact
- Customer_Job
- Income
- Cust_Satisfaction_Score

2️⃣ Credit Card Table (10,109 rows)
- Client_Num
- Card_Category
- Annual_Fees
- Activation_30_Days
- Customer_Acq_Cost
- Week_Start_Date
- Week_Num
- Qtr
- Current_Year
- Credit_Limit
- Total_Revolving_Bal
- Total_Trans_Amt
- Total_Trans_Count
- Avg_Utilization_Ratio
- Use_Chip
- Exp_Type
- Interest_Earned
- Delinquent_Acc

# Project Workflow 
🔹 Step 1: Data Extraction using SQL

- Imported raw customer and credit card data into SQL database
- Performed:
- Data validation
- Null value checks
- Data type verification

Ensured Client_Num is consistent in both tables for joining
Tools Used: SQL

🔹 Step 2: Data Export from SQL

- Exported cleaned tables from SQL as CSV files
- Files used:
- customer.csv
- credit_card.csv

These files were then imported into Power BI

🔹 Step 3: Data Loading in Power BI

- Loaded both CSV files into Power BI
- Verified row count (10,109 rows in each table)
- Checked column data types and formatting

🔹 Step 4: Data Modeling

- Created relationship between tables:
- Client_Num → Primary Key
- Relationship Type:
- One-to-Many
- Data Model Design:
- Customer table → Dimension table
- Credit Card table → Fact table

🔹 Step 5: Calculated Columns (Power BI)
Customer Table

- Age_Group (Created age buckets for demographic analysis)
- Income_Group (Segmented customers based on income ranges)
These columns help in customer segmentation and slicing dashboards.

🔹 Step 6: DAX Measures Created

Revenue Analysis

- Current_week_revenue
- Previous_week_revenue
- WoW_revenue (Week-over-Week revenue change)

Transaction Metrics

- Total_Trans_Amt
- Total_Trans_Count
- Total_Revolving_Bal

These measures enable trend analysis, KPI tracking.

🔹 Step 7: Power BI Dashboard & Visuals
KPI Cards

- Total Revenue
- Total Transaction Amount
- Total Transaction Count
- Total Interest
- Income
- Customer satisfiction Score
  
Charts & Visuals

Line Chart: Week-over-Week Revenue Trend

- Bar Chart: Revenue by Card Category
- Bar Chart: Delinquent Accounts by Card Category
- Bar Chart: Customer Count by Income Group
- Bar Chart : Transaction Count by Use Chip

Filters & Slicers

- Gender
- Education Level
- Card Category
- Quarter
- Week Start Date
- Use Chip

These slicers make the dashboard fully interactive.
