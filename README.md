# Retail Sales Analysis | PostgreSQL

**SQL-based transaction, customer and sales performance analysis**

## Project overview
This project analyses retail transaction data from 2022–2023 to understand category contribution, customer purchasing patterns, monthly average transaction value and time-of-day activity. PostgreSQL queries are used to clean, explore and analyse the data, then translate the results into practical retail questions and recommendations.

## Business problem
Retail decision-makers need a consistent view of what drives sales, which categories contribute most, who is purchasing and when transaction activity is strongest. This project creates that view from transaction-level records to support more informed merchandising, customer engagement and store-operations reviews.

## Dataset
- **Source:** `Dataset_Retail_Sales.csv`
- **Raw size:** 2,000 rows × 11 columns
- **Period:** 1 January 2022 – 31 December 2023
- **Categories:** Beauty, Clothing, Electronics
- **Fields:** transaction ID, sale date, sale time, customer ID, gender, age, category, quantity, price per unit, COGS and total sale.
- **Cleaned analysis set:** 1,987 complete transactions; 155 distinct customers.

## Tools and SQL concepts
- PostgreSQL
- SQL data definition and filtering
- NULL checks and data cleaning
- `COUNT`, `COUNT(DISTINCT)`, `SUM`, `AVG`, `GROUP BY`, `ORDER BY`
- Date extraction and monthly grouping
- `CASE` expressions for shift segmentation
- Common Table Expressions (CTEs)
- Window function: `RANK()`

## Workflow
1. Inspected the dataset schema, date range and missing values.
2. Checked data quality and removed incomplete records for the analysis set.
3. Explored transaction volume, customer count and category values.
4. Wrote SQL queries to answer ten retail business questions.
5. Compared category, gender, customer, monthly and shift-level patterns.
6. Interpreted findings and documented practical recommendations and limitations.

## Key findings
- **908,230** total sales across **1,987** complete transactions.
- **155** distinct customers in the cleaned dataset.
- Category sales were closely balanced: Electronics **311,445**, Clothing **309,995**, Beauty **286,790**.
- Clothing had the highest transaction count (**698**); Electronics generated the highest category sales (**311,445**).
- Beauty had the highest average transaction value (**469.38**).
- Evening was the busiest shift with **1,062 transactions** (about **53.4%**).
- Highest average transaction value by year: **July 2022 (541.34)** and **February 2023 (535.53)**.
- Top customer by cumulative sales: customer ID **3**, with **38,440**.

## Business value
The analysis establishes a baseline for category planning, customer analysis and shift-level operational reviews. It highlights the need to assess category margin and inventory alongside sales, investigate monthly peaks using revenue and order volume, and review evening staffing against transaction demand.

## Repository files
- Dataset_Retail_Sales.csv
- Code_Retail_Sales.Sql
-Retail_Sales_Analysis_Project_Report

## Keywords
Retail Analytics, Sales Analysis, PostgreSQL, SQL, Data Cleaning, Exploratory Data Analysis, Customer Segmentation, Revenue Analysis, Category Performance, Monthly Sales Trends, Window Functions, Business Intelligence, Data-Driven Decision Making.
