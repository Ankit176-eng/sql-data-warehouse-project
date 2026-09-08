# sql-data-warehouse-project

## 📌 Project Overview

This project demonstrates the development of an **end-to-end SQL Data Warehouse** using a **Bronze, Silver, and Gold layered architecture**.

The project covers **ETL, data cleaning, transformation, data modeling, and analytics** to convert raw business data into meaningful and analysis-ready information.

---

## 🎯 Project Objectives

* Build an end-to-end SQL Data Warehouse
* Implement **Bronze, Silver, and Gold layers**
* Perform **ETL (Extract, Transform, Load)**
* Clean and transform raw data
* Create a structured **data model**
* Develop analytical views for reporting
* Generate business insights using SQL

---

## 🏗️ Data Warehouse Architecture

```text
                ┌─────────────────┐
                │   Source Data   │
                │ CSV / Raw Files  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │  Bronze Layer   │
                │   Raw Data      │
                └────────┬────────┘
                         │
                    ETL / Cleaning
                         │
                         ▼
                ┌─────────────────┐
                │  Silver Layer   │
                │ Cleaned Data    │
                └────────┬────────┘
                         │
                Transformation
                         │
                         ▼
                ┌─────────────────┐
                │   Gold Layer    │
                │ Business Ready  │
                │     Data        │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │    Analytics    │
                │ Reports / BI    │
                └─────────────────┘
```

---

## 🥉 Bronze Layer

The Bronze layer stores **raw data** directly from the source systems.

### Activities

* Load raw CSV/source data
* Preserve original data
* Basic validation
* Track data loading process

---

## 🥈 Silver Layer

The Silver layer contains **cleaned and transformed data**.

### Activities

* Remove duplicate records
* Handle NULL values
* Standardize data formats
* Clean incorrect values
* Convert data types
* Apply business rules
* Integrate multiple source tables

---

## 🥇 Gold Layer

The Gold layer contains **business-ready analytical data**.

### Activities

* Create fact tables
* Create dimension tables
* Apply business logic
* Create analytical views
* Prepare data for reporting and BI tools

---

## 🔄 ETL Process

### Extract

Data is extracted from source files/systems.

### Transform

Data is cleaned, validated, standardized, and transformed using SQL.

### Load

The transformed data is loaded into the appropriate Data Warehouse layers.

```text
Extract → Transform → Load
   ↓          ↓          ↓
Source → Cleaning → Data Warehouse
```

---

## 🧩 Data Modeling

The Gold layer follows a **dimensional data modeling approach**.

### Fact Tables

Store measurable business transactions such as:

* Sales
* Quantity
* Revenue
* Orders

### Dimension Tables

Store descriptive information such as:

* Customers
* Products
* Dates
* Locations

### Example Star Schema

```text
              Dim_Customer
                   │
                   │
Dim_Product ─── Fact_Sales ─── Dim_Date
                   │
                   │
              Dim_Location
```

---

## 📊 Analytics

SQL is used to answer important business questions, such as:

* What is the total sales revenue?
* Which products generate the highest revenue?
* Which customers generate the most sales?
* What are the monthly sales trends?
* Which categories perform best?
* What are the top-performing regions?
* What is the average order value?
* How are sales changing over time?

---

## 🛠️ Technologies Used

* **SQL**
* **SQL Server**
* **ETL**
* **Data Warehousing**
* **Data Modeling**
* **Dimensional Modeling**
* **Data Analytics**
* **Git & GitHub**
* **Power BI** *(if used for reporting)*

---

## 📁 Project Structure

```text
sql-data-warehouse-project/
│
├── datasets/
│   └── raw_data.csv
│
├── scripts/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── docs/
│   ├── data_model.png
│   └── architecture.png
│
├── tests/
│
├── README.md
└── LICENSE
```

---

## 🔍 Key Skills Demonstrated

* SQL Querying
* Joins
* CTEs
* Subqueries
* Window Functions
* Stored Procedures
* Views
* Data Cleaning
* ETL Development
* Data Transformation
* Data Modeling
* Star Schema
* Fact & Dimension Tables
* Data Warehouse Architecture
* Business Analytics

---

## 🚀 Project Outcome

The project transforms raw source data into a **structured, clean, and analysis-ready Data Warehouse**, enabling efficient SQL-based analytics and business reporting.

---

## 👨‍💻 Author

**Ankit Kumar Swain**

**Skills:** SQL | Power BI | Excel | Python | Data Analytics

---



