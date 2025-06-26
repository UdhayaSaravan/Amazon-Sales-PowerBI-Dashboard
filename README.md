#  Amazon Sales Analysis Dashboard – Power BI Project

##  Project Overview

This Power BI project visualizes Amazon sales data using interactive visuals and DAX measures to derive actionable business insights. The dashboard is divided into two pages, each focusing on key aspects such as product performance, customer behavior, sales trends, and category comparisons.

---

## 📁 Dataset Used

The dataset contains the following fields:

- `orderId`
- `date`
- `product`
- `category`
- `price`
- `quantity`
- `total sales`
- `customer name`
- `customer location`
- `payment method`
- `status`

> ✅ Source: Cleaned and structured Amazon sales data for 2025 (simulated).

---

## 📊 Dashboard Pages & Visuals

### 🔹 **Page 1: Sales Overview**

Focus: Product performance, sales distribution, and payment insights.

**Visuals Used:**
- 📊 **Clustered Column Chart** – Total Sales
- 📊 **Clustered Column Chart** – Total Orders
- 📊 **Clustered Column Chart** – Avg Order Value
- 📊 **Clustered Bar Chart** – Total Sales by product
- 📈 **Line Chart** – Total Sales by Month
- 📎 **Pie Chart** – Total Sales by Category
- 🔘 **Slicer** – Interactive filtering by Category / Month

---

### 🔹 **Page 2: Advanced Insights**

Focus: Time-based analysis and ranking performance by product/category.

**Visuals Used:**
- 📊 **Stacked Column Chart** – Total Orders by Payment Method
- 📋 **Tables** – Customer Name vs Total Sales and Orders
- 🏁 **Ribbon Chart** – Total Sales by Day
- 📈 **Line Chart** – Total Sales by Year,Quarter and Month
- 📊 **Clustered Bar Chart** – Total Quantity Sold by Weekday
- 🔘 **Slicer** – Interactive time or category filte

---

## 🧠 Key DAX Measures & Calculated Columns

```DAX
Total Sales = SUM('amazon_sales_data_2025'[total sales])

Total Orders = DISTINCTCOUNT('amazon_sales_data_2025'[orderId])

Average Order Value = [Total Sales] / [Total Orders]

MonthYear = FORMAT('amazon_sales_data_2025'[date], "MMM YYYY")

Weekday = FORMAT('amazon_sales_data_2025'[date], "dddd")

---


## 📷 Dashboard Previews

Below are screenshots from the Power BI dashboard illustrating interactive visuals and insights.

### 🔹 Page 1: Sales Overview
![Sales Overview](E:\Data Analytics projects\pro1 page1.png)

### 🔹 Page 2: Advanced Insights
![Advanced Insights](E:\Data Analytics projects\pro1 page2.png)

