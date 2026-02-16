# 📊 COVID-19 Data Exploration & Analysis (SQL)

## 📌 Project Overview

This project focuses on performing in-depth exploratory data analysis (EDA) on global COVID-19 data using **SQL in Azure Data Studio**.  

The objective of this analysis is to extract meaningful insights from real-world pandemic data by writing structured SQL queries that examine infection rates, mortality rates, population impact, and geographic trends.

This project demonstrates my ability to:
- Write complex SQL queries
- Perform aggregations and calculations
- Use joins, CTEs, and window functions
- Analyze large datasets efficiently
- Translate raw data into actionable insights

---

## 🛠 Tools Used

- **Azure Data Studio**
- **SQL Server**
- **COVID-19 dataset (CSV format)**

---

## 📂 Dataset Description

The dataset contains global COVID-19 statistics including:

- Location (Country/Region)
- Date
- Total Cases
- New Cases
- Total Deaths
- New Deaths
- Population
- Total Vaccinations (if included)

The dataset allows for time-series analysis as well as cross-country comparisons.

---

## 🧠 Analysis Objectives

The primary analytical goals of this project were to:

1. Calculate death percentages by country  
2. Compare total cases relative to population  
3. Identify countries with the highest infection rates  
4. Determine countries with the highest mortality counts  
5. Analyze global trends over time  
6. Examine continent-level summaries  
7. Utilize window functions to calculate rolling totals  

---

## 🧾 Key SQL Techniques Demonstrated

### ✔ Aggregations
- SUM()
- AVG()
- MAX()
- GROUP BY

### ✔ Filtering & Data Cleaning
- WHERE clauses
- Handling NULL values
- Data type conversions

### ✔ Joins
- INNER JOIN between deaths and vaccination datasets

### ✔ Common Table Expressions (CTEs)
Used to simplify complex queries and improve readability.

### ✔ Window Functions
- Rolling totals
- Partitioned calculations using:
  ```sql
  SUM(new_cases) OVER (PARTITION BY location ORDER BY date)
