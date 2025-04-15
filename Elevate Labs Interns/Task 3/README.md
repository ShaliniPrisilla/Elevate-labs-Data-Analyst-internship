
# 📊 Amazon Sales Report SQL Project

This project focuses on analyzing an Amazon sales dataset using SQL. It involves data cleaning, transformation, normalization into separate tables, and executing insightful queries for business analysis.

---

## 🗂️ Dataset Overview

The original dataset is stored in a table named `amazon sale report`, which contains order, product, and shipping information.

---

## 🔧 Step-by-Step Process

### ✅ 1. Table Renaming
```sql
RENAME TABLE `amazon sale report` TO amazon_sales_report;
```

### 📋 2. View Table Columns
```sql
SELECT COLUMN_NAME
FROM INFORMATION_SCHEMA.COLUMNS
WHERE TABLE_NAME = 'amazon_sales_report';
```

---

## 🏗️ Data Modeling

### Created Normalized Tables:
```sql
-- Orders Table
CREATE TABLE orders (
    order_id VARCHAR(50),
    order_date DATE,
    status VARCHAR(50),
    fulfilment VARCHAR(50),
    sales_channel VARCHAR(50),
    amount DECIMAL(10,2),
    currency VARCHAR(10),
    b2b BOOLEAN,
    fulfilled_by VARCHAR(50),
    sku VARCHAR(100)
);

-- Products Table
CREATE TABLE products (
    sku VARCHAR(100),
    style VARCHAR(100),
    category VARCHAR(100),
    size VARCHAR(50),
    asin VARCHAR(20)
);

-- Shipping Table
CREATE TABLE shipping (
    order_id VARCHAR(50),
    ship_service_level VARCHAR(50),
    courier_status VARCHAR(50),
    ship_city VARCHAR(100),
    ship_state VARCHAR(100),
    ship_postal_code VARCHAR(20),
    ship_country VARCHAR(50)
);
```

---

## 📥 Data Insertion from `amazon_sales_report`
```sql
-- Insert into Orders
INSERT INTO orders (...)

-- Insert into Products
INSERT INTO products (...)

-- Insert into Shipping
INSERT INTO shipping (...)
```

---

## 🔍 Queries & Analysis

### 🎯 Basic Queries
```sql
-- Orders with INR currency
SELECT order_id, sku, ship_city, amount, currency
FROM amazon_sales_report
WHERE currency = 'INR'
ORDER BY amount DESC
LIMIT 10;
```

### 📊 Grouping & Aggregation
```sql
-- Orders by Status
SELECT status, COUNT(*) AS total_orders
FROM amazon_sales_report
GROUP BY status
ORDER BY total_orders DESC;
```

### 🤝 Joins
```sql
-- INNER JOIN: orders + products + shipping
-- LEFT JOIN / RIGHT JOIN
-- FULL OUTER JOIN using UNION
```

### 📈 Subqueries & Aggregate Insights
```sql
-- Orders above average amount
-- Top courier status order filter
-- Total sales in INR
-- Average amount by fulfilment
```

---

## 👁️ Views

```sql
-- High Value INR Orders
CREATE VIEW high_value_inr_orders AS (...)

-- Total Sales by City
CREATE VIEW total_sales_by_city AS (...)
```

---

## 🚀 Indexing
```sql
CREATE INDEX idx_order_id ON orders(order_id);
```

---

## 🔎 Sample Query with Index
```sql
SELECT *
FROM orders o
JOIN shipping s ON o.order_id = s.order_id
WHERE o.order_id = '171-0022303-3275527';
```

---

## 📌 Summary

This SQL project demonstrates:
- Data normalization and schema design
- Comprehensive querying techniques (joins, subqueries, views)
- Aggregations and filtering for business insights
- Optimization via indexing

---

## 📁 Files

- `amazon_sales_report.sql` – Original data import and table creation
- `queries.sql` – All queries used for analysis
- `README.md` – Project overview (this file)

