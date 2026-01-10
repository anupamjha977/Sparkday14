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


## 📂 Notebook File
`spark day 2.ipynb`

---
