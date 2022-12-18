# Sales_Analysis
Sales-Insights-Analysis-Project
## Abstract
In this project I will be conducting a basic sales analysis using MySQL and Power BI.

## Introduction
This project will show how you can download data from MySQL, perform preliminary data analysis, extract, transform and load data into Power BI.

Next, we will build 2 different dashboards on Power BI showing the revenue and profit of various sales.

At the end of the project, we will visualize the revenue and profit trends for various years starting from 2017 to 2020.

## Purpose
To unlock sales insights that are not visible to the sales team in order to enable decision support and automate them in order to reduce the time spent in data gathering.

## Stakeholders
The results obtained in this project can be used by various stakeholders such as

* Sales director
* Marketing team
* Customer service team
* Data and analytics team
* IT
 
## Objective
An automated dashboard providing quick and latest sales in order to support data driven decision making.

## Code and Resources used
MySQL workbench Version:8.0
Power BI
Data Source: 

## Insights
After a quick data exploration in MySQL, here are some initial findings:

* The database contains 5 tables: customers, date, markets, products, and transactions.
* There are 17 markets, 279 products, and 38 customers.
* The observation period is from OCT 2017 to JUN 2020.
* The total revenue in 2020 was ₹ 142.22 M, 57.7% less than 2019, which was ₹ 336.02 M.
* Most of the transactions data are in INR(₹) currency, but we have 2 records in US($) currency.
* And we got some garbage values in sales amount and market column. We’re going to deal with it in the ETL process.

## ETL(Extract, Transform, Load)
Once I knew the basic features of the data I had to work with, I Imported the MySQL database into Power BI to do the necessary transformations and make a simple, reliable, and helpful dashboard.

### Data Modeling Step
We have one main table and four other tables having one shared column with the main table. So we will connect the other tables to the main table using the shared columns.
* Main Table: transactions

# Filtering, Cleaning and Adding New Columns
* The company is serving only in India, So “Paris” and “New York” in the market table are garbage values, so filtering them out.
* The “currency” column (in transactions table) have 2 USD currency values, So created a new column called “Sales”, where all the sales_amount is in INR Currency.

## Dashboards
The three dashboards shows all the main information about the company sales.
https://github.com/Ashfia23/Sales_Analysis_using_PowerBI/blob/main/Sales_Dashboard_Report.pdf

## Final Report
Based on the dashbaords insights, I have made some conclusions and recommendation that Sales Marketing team should/can consider making a sales strategy.

### Conclusions
* Sales were rapidly decreasing in 2020 compared to 2019 by around 57.7%.
* Highest revenue generated from Markets such as Delhi NCR, Mumbai, Ahmedabad, Bhopal, Nagpur, and so on.
* Highest quantities sold in the Market such as Delhi NCR, Mumbai, Nagpur, Kochi, Ahmedabad, and so on.
* Majority of the sales were takes place in the month of January followed by November and March.

### Recommendation
* Make a new sales strategy for lucknow since its showing lowest revenue and negative profit margin and if possible so as for Surat and Bhubhaneshwar also.
* try to increase sales quantity in Patna, Surat and Kanpur since they have lowest sales quantity.
* start target campagin for Prod047 and Prod061 since they two are the most profitable and most selling products.
* try to give special benefits to Electronics and Excel stores as they are most profitable customers.
* make campgain strategy for mid year as they are showing high sales among other months.
