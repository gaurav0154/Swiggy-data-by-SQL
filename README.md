# 🍔 Swiggy Sales Analysis (PostgreSQL Data Warehouse Project)

## 📌 Project Overview

This project focuses on transforming a large and unstructured food delivery dataset into a **clean, scalable, and analytics-ready data warehouse** using PostgreSQL.

The core idea was to simulate a real-world business scenario where raw data is messy and not directly usable. Through **data cleaning, normalization, and dimensional modeling (Star Schema)**, the dataset was converted into a powerful system capable of generating meaningful business insights.

---

## 🎯 Project Objective

* Clean and validate messy raw delivery data
* Remove duplicates and handle missing values
* Build a **Star Schema Data Model**
* Enable fast and efficient analytical queries
* Generate business insights to improve:

  * Sales 📈
  * Delivery efficiency 🚚
  * Customer satisfaction ⭐

---

## 💼 Business Problems Solved

* Which locations generate the highest revenue?
* When are peak order times?
* What are the most popular dishes and cuisines?
* Which restaurants are underperforming?
* How do customer ratings impact business performance?

---

## 🛠️ Tools & Technologies

* PostgreSQL
* SQL (Advanced Queries)
* Data Warehousing Concepts
* Git & GitHub

---

## 🧹 Data Cleaning & Validation

### ✅ Null Value Checks

Checked missing values in critical fields:

* State, City, Order Date
* Restaurant Name, Location
* Category, Dish Name
* Price, Rating, Rating Count

### ✅ Duplicate Detection & Removal

* Identified duplicate rows using `GROUP BY`
* Removed duplicates using `ROW_NUMBER()` and CTE

### ✅ Data Quality Improvements

* Ensured consistency
* Improved reliability of analytics

---

## 🏗️ Data Modeling (Star Schema)

To optimize performance and scalability, a **Star Schema** was implemented.

### 📊 Dimension Tables

* `dim_date` → Date attributes (Year, Month, Quarter, Week)
* `dim_location` → State, City, Location
* `dim_restaurant` → Restaurant names
* `dim_category` → Cuisine types
* `dim_dish` → Dish names

### ⭐ Fact Table

* `fact_swiggy_orders`

  * Price
  * Rating
  * Rating Count
  * Foreign keys linking all dimensions

### 🚀 Benefits

* Faster query performance
* Reduced redundancy
* Easy BI/dashboard integration
* Scalable architecture

---

## 📈 KPI Development

### 🔹 Basic KPIs

* Total Orders
* Total Revenue (INR Millions)
* Average Dish Price
* Average Rating

### 🔹 Advanced Business Analysis

#### 📅 Date Analysis

* Monthly trends
* Quarterly trends
* Yearly growth
* Day-of-week ordering patterns

#### 📍 Location Analysis

* Top cities by orders
* Revenue by state

#### 🍽️ Food Performance

* Top restaurants
* Popular cuisines
* Most ordered dishes
* Category performance (Orders + Ratings)

#### 💰 Customer Spending Insights

Order distribution across price ranges:

* Under 100
* 100–199
* 200–299
* 300–499
* 500+

#### ⭐ Ratings Analysis

* Distribution of ratings (1–5)

---

## 🔍 Key Insights

* Certain cities dominate order volume and revenue
* Peak orders occur on specific days and months
* Mid-range pricing (₹100–₹300) drives maximum orders
* High-rated restaurants contribute significantly to repeat orders
* Some restaurants underperform due to low ratings

---

## 💡 Business Recommendations

* Focus marketing on high-growth cities
* Optimize pricing strategies for mid-range customers
* Improve quality for low-rated restaurants
* Promote top-performing dishes
* Plan delivery resources for peak times

---

## ⚡ SQL Concepts Used

* CTEs (Common Table Expressions)
* Window Functions (`ROW_NUMBER()`)
* Aggregations (`COUNT`, `SUM`, `AVG`)
* Joins (Fact-Dimension relationships)
* Date Functions (`EXTRACT`, `TO_CHAR`)
* Conditional Logic (`CASE WHEN`)

---

## 🚀 How to Run This Project

1. Install PostgreSQL
2. Create database
3. Import raw dataset into `swiggy_data`
4. Run data cleaning queries
5. Create dimension & fact tables
6. Insert transformed data
7. Run KPI queries

---

## 📁 Project Structure

```
📦 swiggy-sales-analysis
 ┣ 📜 Swiggy solutions.sql
 ┣ 📜 swiggy_data.csv
 ┗ 📜 README.md
```

---

## 🧠 What I Learned

* End-to-end data pipeline development
* Real-world data cleaning challenges
* Data warehousing & star schema design
* Writing optimized SQL queries for analytics
* Converting raw data into actionable insights

---

## 📬 Contact

* LinkedIn: (https://www.linkedin.com/in/gaurav-joshi-335165217)
* GitHub: (https://github.com/gaurav0154/Swiggy-data-by-SQL)

---

## ⭐ Support

If you found this project helpful, give it a ⭐ and share your feedback!

---

🔥 *This project demonstrates strong SQL, data cleaning, and data warehousing skills—making it highly valuable for Data Analyst and Data Engineer roles.*
