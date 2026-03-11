# Jenson-USA-SQL-Data-Analysis-Project
Project Overview

This project is an end-to-end SQL Data Analysis case study on the Jenson USA retail database, focusing on analyzing customer behavior, product performance, store sales, and staff productivity.

The objective of this project is to transform raw transactional retail data into meaningful business insights using MySQL analytical queries.

The workflow includes:

Retail sales data exploration

Multi-table relational analysis

Advanced SQL querying

Performance and sales trend analysis

Business insight generation

Business Problem

Retail businesses generate large volumes of transactional data across customers, products, stores, and employees. However, without structured analysis, it becomes difficult to extract actionable insights.

As a Data Analyst, the goal of this project was to answer key business questions such as:

Which stores generate the highest sales volume?

Which products contribute the most revenue?

Who are the most valuable customers?

Which staff members perform above or below average?

Are there products that remain unsold in the inventory?

The insights derived from this analysis can help improve sales strategy, inventory planning, employee performance monitoring, and customer engagement.

Dataset

Dataset Source:

Jenson USA Retail Database

Dataset Link:
https://drive.google.com/drive/folders/1feFkClnYME7Be3kjmz-TD2PV1uVkXNAN

Tables Used

The project analyzes multiple relational tables including:

customers

orders

order_items

products

categories

stores

staff

These tables were combined using SQL joins to generate cross-functional business insights.

Project Execution & Methodology
A. Store Sales Analysis

The first step was to evaluate store performance by calculating the total number of products sold by each store.

Joined stores, orders, and order_items tables

Calculated total quantity sold

Ranked stores by sales performance

Business Purpose:

Identify high-performing locations

Understand store-level demand patterns

B. Product Sales Trend Analysis

To analyze product demand over time, cumulative sales were calculated using window functions.

Partitioned sales by product

Ordered transactions by date

Calculated running totals of quantities sold

Business Purpose:

Identify long-term product demand

Track growth patterns in sales

C. Category-Level Revenue Analysis

Products were analyzed to determine which product generated the highest revenue within each category.

Calculated revenue using quantity × price

Ranked products using ROW_NUMBER()

Selected top-performing product per category

Business Purpose:

Identify top revenue drivers

Support category-based marketing strategies

D. Customer Spending Analysis

Customer purchasing behavior was analyzed to identify the highest spending customer.

Joined customers, orders, and order_items

Calculated total purchase value

Ranked customers by total spending

Business Purpose:

Identify VIP customers

Support loyalty and retention strategies

E. Premium Product Identification

To understand the premium offerings in the product catalog, the highest priced product in each category was identified.

Partitioned products by category

Selected maximum price per category

Business Purpose:

Identify high-end product offerings

Support pricing and product positioning analysis

F. Customer Purchase Behavior by Store

Customer activity across store locations was analyzed.

Counted total orders per customer per store

Analyzed shopping distribution across locations

Business Purpose:

Understand store-level customer engagement

Identify loyal customers at specific locations

G. Staff Performance Analysis

Employee productivity was analyzed by identifying:

Staff members who have no recorded sales

Staff members whose sales exceed the average performance

Business Purpose:

Detect underperforming staff

Recognize high-performing employees

H. Product Demand Analysis

To identify best-selling products:

Total quantity sold was calculated

Products were ranked by sales volume

Top 3 best-selling products were identified

Business Purpose:

Identify products with highest demand

Support inventory planning

I. Pricing Distribution Analysis

The median product price was calculated to understand the central price range of products.

Business Purpose:

Understand pricing distribution

Identify the mid-point of the product price range

J. Inventory Performance Analysis

Products that have never been ordered were identified using NOT EXISTS.

Business Purpose:

Detect slow-moving or inactive inventory

Support product discontinuation or promotion decisions

K. Customer Category Coverage Analysis

Customers who have purchased products from every category were identified.

Business Purpose:

Identify highly engaged customers

Understand diverse purchasing behavior

SQL Techniques & Concepts Used

The project demonstrates practical use of several SQL concepts used in real-world data analytics.

Data Retrieval

SELECT statements for extracting relevant columns

Table Relationships

INNER JOIN

LEFT JOIN

Aggregation and Grouping

GROUP BY for summarizing data

Aggregate Functions

COUNT()

SUM()

AVG()

Advanced SQL

Window Functions

ROW_NUMBER()

Common Table Expressions (CTE)

Subqueries

EXISTS / NOT EXISTS

Statistical Computation

Median price calculation using window logic

Technologies & Skills

Database: MySQL

Query Language: SQL

Data Analysis: Aggregations and window functions

Database Concepts: Relational modeling and joins

Analytical Skills:

Business data interpretation

Customer behavior analysis

Sales trend analysis

Staff performance evaluation

Inventory analysis

Key Insights & Impact

The analysis revealed several meaningful business insights:

Certain stores significantly outperform others in total sales.

A small number of products drive a large portion of total sales.

Some customers contribute disproportionately to total revenue.

Several products have never been ordered, indicating inventory inefficiencies.

Staff sales performance varies significantly across employees.

These insights can help businesses improve:

Sales strategy

Inventory management

Customer engagement

Staff performance monitoring

Product marketing decisions

Challenges Faced

Understanding relationships between multiple database tables.

Writing optimized SQL queries across multiple joins.

Implementing median calculations using SQL.

Handling complex queries using subqueries and CTEs.

Future Enhancements

Build an interactive Power BI dashboard on top of the SQL analysis.

Implement sales forecasting models for product demand prediction.

Add customer segmentation analysis.

Create automated data pipelines for continuous reporting.Project Overview

This project is an end-to-end SQL Data Analysis case study on the Jenson USA retail database, focusing on analyzing customer behavior, product performance, store sales, and staff productivity.

The objective of this project is to transform raw transactional retail data into meaningful business insights using MySQL analytical queries.

The workflow includes:

Retail sales data exploration

Multi-table relational analysis

Advanced SQL querying

Performance and sales trend analysis

Business insight generation

Business Problem

Retail businesses generate large volumes of transactional data across customers, products, stores, and employees. However, without structured analysis, it becomes difficult to extract actionable insights.

As a Data Analyst, the goal of this project was to answer key business questions such as:

Which stores generate the highest sales volume?

Which products contribute the most revenue?

Who are the most valuable customers?

Which staff members perform above or below average?

Are there products that remain unsold in the inventory?

The insights derived from this analysis can help improve sales strategy, inventory planning, employee performance monitoring, and customer engagement.

Dataset

Dataset Source:

Jenson USA Retail Database

Dataset Link:
https://drive.google.com/drive/folders/1feFkClnYME7Be3kjmz-TD2PV1uVkXNAN

Tables Used

The project analyzes multiple relational tables including:

customers

orders

order_items

products

categories

stores

staff

These tables were combined using SQL joins to generate cross-functional business insights.

Project Execution & Methodology
A. Store Sales Analysis

The first step was to evaluate store performance by calculating the total number of products sold by each store.

Joined stores, orders, and order_items tables

Calculated total quantity sold

Ranked stores by sales performance

Business Purpose:

Identify high-performing locations

Understand store-level demand patterns

B. Product Sales Trend Analysis

To analyze product demand over time, cumulative sales were calculated using window functions.

Partitioned sales by product

Ordered transactions by date

Calculated running totals of quantities sold

Business Purpose:

Identify long-term product demand

Track growth patterns in sales

C. Category-Level Revenue Analysis

Products were analyzed to determine which product generated the highest revenue within each category.

Calculated revenue using quantity × price

Ranked products using ROW_NUMBER()

Selected top-performing product per category

Business Purpose:

Identify top revenue drivers

Support category-based marketing strategies

D. Customer Spending Analysis

Customer purchasing behavior was analyzed to identify the highest spending customer.

Joined customers, orders, and order_items

Calculated total purchase value

Ranked customers by total spending

Business Purpose:

Identify VIP customers

Support loyalty and retention strategies

E. Premium Product Identification

To understand the premium offerings in the product catalog, the highest priced product in each category was identified.

Partitioned products by category

Selected maximum price per category

Business Purpose:

Identify high-end product offerings

Support pricing and product positioning analysis

F. Customer Purchase Behavior by Store

Customer activity across store locations was analyzed.

Counted total orders per customer per store

Analyzed shopping distribution across locations

Business Purpose:

Understand store-level customer engagement

Identify loyal customers at specific locations

G. Staff Performance Analysis

Employee productivity was analyzed by identifying:

Staff members who have no recorded sales

Staff members whose sales exceed the average performance

Business Purpose:

Detect underperforming staff

Recognize high-performing employees

H. Product Demand Analysis

To identify best-selling products:

Total quantity sold was calculated

Products were ranked by sales volume

Top 3 best-selling products were identified

Business Purpose:

Identify products with highest demand

Support inventory planning

I. Pricing Distribution Analysis

The median product price was calculated to understand the central price range of products.

Business Purpose:

Understand pricing distribution

Identify the mid-point of the product price range

J. Inventory Performance Analysis

Products that have never been ordered were identified using NOT EXISTS.

Business Purpose:

Detect slow-moving or inactive inventory

Support product discontinuation or promotion decisions

K. Customer Category Coverage Analysis

Customers who have purchased products from every category were identified.

Business Purpose:

Identify highly engaged customers

Understand diverse purchasing behavior

SQL Techniques & Concepts Used

The project demonstrates practical use of several SQL concepts used in real-world data analytics.

Data Retrieval

SELECT statements for extracting relevant columns

Table Relationships

INNER JOIN

LEFT JOIN

Aggregation and Grouping

GROUP BY for summarizing data

Aggregate Functions

COUNT()

SUM()

AVG()

Advanced SQL

Window Functions

ROW_NUMBER()

Common Table Expressions (CTE)

Subqueries

EXISTS / NOT EXISTS

Statistical Computation

Median price calculation using window logic

Technologies & Skills

Database: MySQL

Query Language: SQL

Data Analysis: Aggregations and window functions

Database Concepts: Relational modeling and joins

Analytical Skills:

Business data interpretation

Customer behavior analysis

Sales trend analysis

Staff performance evaluation

Inventory analysis

Key Insights & Impact

The analysis revealed several meaningful business insights:

Certain stores significantly outperform others in total sales.

A small number of products drive a large portion of total sales.

Some customers contribute disproportionately to total revenue.

Several products have never been ordered, indicating inventory inefficiencies.

Staff sales performance varies significantly across employees.

These insights can help businesses improve:

Sales strategy

Inventory management

Customer engagement

Staff performance monitoring

Product marketing decisions

Challenges Faced

Understanding relationships between multiple database tables.

Writing optimized SQL queries across multiple joins.

Implementing median calculations using SQL.

Handling complex queries using subqueries and CTEs.

Future Enhancements

Build an interactive Power BI dashboard on top of the SQL analysis.

Implement sales forecasting models for product demand prediction.

Add customer segmentation analysis.

Create automated data pipelines for continuous reporting.
