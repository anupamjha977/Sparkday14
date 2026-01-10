# Spark Day 2 — README

## 📌 Overview
This notebook covers **Spark Day 2 learning** with hands-on practice on **reading CSV files** and applying core **PySpark DataFrame transformations** in Databricks.

The notebook is designed for transformation practice and includes commonly used functions required in real-world data engineering pipelines.

---

## ✅ Topics Covered

### 1) Reading CSV Files in Spark
- How to load CSV into Spark DataFrame
- Understanding reader options:
  - header
  - inferSchema
  - delimiter/separator
  - schema enforcement
  - handling null/blank values
- Data exploration after reading:
  - display()
  - show()
  - printSchema()

---

### 2) Column Transformations (`col`)
- Using `col()` to reference DataFrame columns
- Creating derived columns using calculations
- Best practices for clean column expressions

---

### 3) Filtering Data (`filter`)
- Filtering rows based on conditions
- Multiple condition filtering using:
  - `&` (AND)
  - `|` (OR)
  - `~` (NOT)
- Filtering NULL values using:
  - `isNull()`
  - `isNotNull()`

---

### 4) Conditional Logic (`when`)
- Creating new columns using if-else logic
- Handling NULL/blank strings and replacing them
- Use cases:
  - categorizing age group
  - creating flags/indicators
  - assigning default values like `XXXX`

---

### 5) Aggregations (`groupBy + agg`)
- Grouping data state-wise / city-wise
- Aggregation functions:
  - sum
  - avg
  - max
  - count
- Order results using `orderBy`

---

### 6) Spark SQL Expressions (`expr`)
- Writing SQL-like formulas inside PySpark
- Using expressions for:
  - arithmetic formulas
  - `CASE WHEN`
  - clean and compact transformations

---

### 7) Sales Calculation Logic
The notebook includes formula-based sales calculations:

- **Gross Amount** = quantity * unit_price  
- **Discount Amount** = gross_amount * discount_pct/100  
- **Tax Amount** = (gross_amount - discount_amount) * tax_pct/100  
- ✅ **Total Sale** = gross_amount - discount_amount + tax_amount  

This is used further to compute:
- Total sale by state
- Sorting highest revenue state

---

## 🧪 Practice Exercises Included
- Find null / blank customer names
- Clean customer_name by replacing missing values
- Compute total sales columns
- Group and rank outputs (state revenue analysis)
- Use `dense_rank` / ranking patterns

---

## ⭐ Expected Outcome
By completing this notebook, you will be confident in:
- Reading CSV files in Spark correctly
- Cleaning and transforming raw data
- Writing PySpark transformations used in Medallion pipelines
- Creating aggregated reporting outputs (Gold layer style)

---

## 📂 Notebook File
`spark day 2.ipynb`

---
