# SQL Data Analysis Project

This project contains SQL scripts and sample datasets for performing data analysis on three different domains:

1. **HR Data (`hrdata`)**
2. **Car Sales Data (`car_info`)**
3. **Call Center Performance Data (`call_center`)**

Each dataset includes `CREATE TABLE`, `INSERT INTO`, and analysis queries written in MySQL.

---

## 📁 Contents

### 1. HR Data

- **File:** `hrdata.sql`
- **Table:** `hrdata`
- **Purpose:** To analyze employee attrition, job satisfaction, education background, department-wise attrition, and more.
- **Key Queries:**
  - Average job satisfaction by department
  - Attrition rate by education field
  - Count of active employees

---

### 2. Car Sales Data

- **File:** `car_info.sql`
- **Table:** `car_info`
- **Purpose:** Analyze second-hand car sales data to understand pricing trends, mileage patterns, and market behavior.
- **Key Queries:**
  - Average selling price by fuel type
  - Car models with decreasing price trend year-over-year
  - Cumulative and exponential moving averages of prices
  - Cars priced within ±10% of average price

---

### 3. Call Center Data

- **File:** `call_center.sql`
- **Table:** `call_center`
- **Purpose:** Analyze call volume, CSAT scores, and call duration trends in a multi-city call center operation.
- **Data Cleaning:**
  - Converted `call_timestamp` to proper date format
  - Replaced empty CSAT scores with `NULL`
- **Key Queries:**
  - CSAT score statistics
  - Call volume by day of the week
  - Call durations by response time
  - Distribution of sentiments and cities

---

## 🚀 How to Use

1. **Set up MySQL Server**
2. Run each SQL script (`.sql` file) in your preferred SQL client (e.g., MySQL Workbench, DBeaver).
3. Analyze the data using the provided SELECT queries or write your own.

---

## 🛠️ Technologies Used

- MySQL 8+
- SQL (DDL, DML, Window Functions, CTEs, Subqueries)

---

## 📌 Note

Make sure SQL Safe Updates is disabled before running some `UPDATE` statements:

```sql
SET SQL_SAFE_UPDATES = 0;
-- Run your UPDATEs
SET SQL_SAFE_UPDATES = 1;
