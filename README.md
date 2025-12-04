# SQL_finance_analytics
📊 Financial Analytics Using SQL — Portfolio Project
📌 Overview

This project performs end-to-end financial analytics using SQL.
It includes customer-level sales analysis, product analytics, gross price calculations, fiscal year logic, stored procedures, and market-level performance classification.

All SQL scripts in this project were written as part of my Data Analytics learning journey to practice real-world financial analysis, similar to what analysts do in startups and business teams.

🎯 Key Objectives
✔ Customer-Level Analysis

Identify customers (e.g., Croma India)

Pull sales transactions for selected fiscal years

Join with product and pricing tables

Generate customer revenue and gross sales insights

✔ Fiscal Year Automation

Created a reusable get_fiscal_year() SQL function

Automatically converts calendar date → fiscal year (April–March)

✔ Stored Procedures

This project includes multiple stored procedures:

1️⃣ get_monthly_gross_sales_for_customer()

Generates monthly gross sales for any customer or multiple customers.

2️⃣ get_market_badge()

Classifies a market as:

Gold → Total sold quantity > 5 million

Silver → Otherwise

This logic helps understand market performance category automatically.

🛠 Tools & Technologies

SQL

MySQL

Joins, CTEs, Functions, Stored Procedures

GitHub for version control

📂 Files Included
File	Description
project1_finance_analytics.sql	Full SQL analysis including joins, fiscal year function, stored procedures, and financial metrics
🔍 Detailed Analysis Performed
1. Customer Identification
SELECT * 
FROM dim_customer 
WHERE customer LIKE "%croma%" AND market = "india";

2. Sales Transactions for a Fiscal Year

Uses fiscal year logic (April–March) to filter sales.

3. Fiscal Year Function

Created a function:

get_fiscal_year(date)


Helps ensure fiscal-year-based reporting in all queries.

4. Product & Pricing Join

Joined product and price tables to compute:

Sold Quantity

Gross Price

Total Gross Sales

5. Monthly Gross Sales Report

Aggregated report for:

A single customer

Multiple customers

All fiscal years

6. Market Badge Classification

Stored procedure:

Computes total sold quantity for a market

Assigns Gold / Silver category

🧠 Concepts Demonstrated

SQL Functions

Stored Procedures

Joins (INNER JOIN)

Date manipulation

Aggregations & KPIs

Financial Calculations (Revenue, Gross Sales)

Performance classification logic

🚀 How to Use

Clone the repository

Import the database schema

Run the SQL functions & procedures

Execute reports for any customer or market

📈 Example Output KPIs

Monthly Gross Sales

Market Category (Gold/Silver)

Total Sold Quantity

Fiscal-Year Revenue

🙌 About Me

I’m learning SQL, Python, Excel, and Power BI to become a Data Analyst.
This financial analytics project showcases my SQL skills and real-world problem-solving abilities.
