# Retail Sales SQL Analysis

## Project Overview

This project uses SQL to analyze a mock retail sales database. The goal of the project is to answer common business questions related to sales performance, product revenue, customer behavior, and regional trends.

The database was created in SQLite using DB Browser for SQLite. It contains customer, product, order, and order item data. SQL queries were used to summarize revenue, identify top-performing products, compare sales by state, analyze monthly sales trends, and find repeat customers.

## Tools Used

- SQLite
- DB Browser for SQLite
- SQL
- GitHub

## Database Structure

The database contains four tables:

### customers

Contains customer information such as customer ID, name, age, gender, state, and signup date.

### products

Contains product information such as product ID, product name, category, and unit price.

### orders

Contains order-level information such as order ID, customer ID, order date, and state.

### order_items

Contains item-level order details such as product ID, quantity purchased, and unit price.

## Entity Relationship Overview

The tables are connected using primary and foreign keys:

- `customers.customer_id` connects to `orders.customer_id`
- `orders.order_id` connects to `order_items.order_id`
- `products.product_id` connects to `order_items.product_id`

This structure allows sales data to be analyzed across customers, products, orders, and locations.

## Business Questions Answered

This project answers the following questions:

1. What is the total revenue?
2. How many total orders were placed?
3. What is the average order value?
4. Which product categories generated the most revenue?
5. Which states generated the most revenue?
6. Which products were the top revenue drivers?
7. How did revenue change by month?
8. Which customers spent the most?
9. Which customers placed multiple orders?
10. How do products rank by total revenue?

## SQL Skills Demonstrated

This project demonstrates the following SQL skills:

- Creating relational database tables
- Using primary keys and foreign keys
- Inserting data into tables
- Querying tables with `SELECT`
- Filtering and sorting results
- Joining multiple tables
- Aggregating data with `SUM`, `COUNT`, and `AVG`
- Grouping results with `GROUP BY`
- Filtering grouped results with `HAVING`
- Using date functions
- Using window functions such as `RANK()`

## Project Files

```text
retail-sales-sql-analysis/
│
├── README.md
├── retail_sales_project.db
│
└── sql/
    ├── 01_table_setup.sql
    ├── 02_insert_data.sql
    ├── 03_table_checks.sql
    ├── 04_sql_checks.sql
    └── 05_analysis_queries.sql
