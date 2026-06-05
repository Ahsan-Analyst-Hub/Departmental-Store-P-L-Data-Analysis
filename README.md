# Departmental Store P&L Data Analysis
<img width="1376" height="768" alt="Image" src="https://github.com/user-attachments/assets/8e109456-7150-4040-90e9-c969f94778fd" />


## Project Overview

The **Departmental Store P&L Data Analysis** is a Power BI business intelligence project designed to transform raw transactional data into actionable insights. The project focuses on analyzing sales performance, profitability, customer behavior, product performance, promotional effectiveness, and regional sales trends across multiple product categories.

Using Power BI, Power Query, and data modeling techniques, an interactive dashboard was developed to enable stakeholders to monitor key business metrics and make data-driven decisions.

---

## Business Problem

Department stores generate large volumes of transactional data from various product categories, customers, and promotional campaigns. Without proper analysis, it becomes difficult to:

* Identify top and underperforming products.
* Monitor sales and profit trends over time.
* Evaluate the effectiveness of promotions and discounts.
* Compare business performance across different periods.
* Understand customer purchasing behavior.
* Analyze regional sales distribution.
* Track key operational and financial metrics.

This project addresses these challenges through a comprehensive Power BI dashboard.

---

## Dataset Information

The project uses four datasets:

### 1. DimCustomers

Contains customer-related information including customer identifiers and demographic details.

### 2. DimProduct

Contains product information such as:

* Product ID
* Product Name
* Product Category
* Product Price

### 3. DimPromotions

Contains promotional campaign details including:

* Promotion ID
* Promotion Name / Ad Type / Coupon code
* Discount Information

### 4. Fact Sheet

Transactional dataset containing:

* Customer References
* Product References
* Promotion References
* Order Details
* Unit Price
* Sales
* Profit
* Quantity Sold
* Offers
* Dates
  
---

## Product Categories Analyzed

The department store operates across the following categories:

* Electronics
* Footwear
* Clothing
* Home Appliances
* Accessories
* Kitchenware
* Bags
* Personal Care

---

## Project Objectives

The dashboard was designed to answer the following business questions:

### A)Product Performance Analysis

* Identify Top 5 Products by Sales
* Identify Bottom 5 Products by Sales
* Identify Top 5 Products by Profit
* Identify Bottom 5 Products by Profit
* Identify Top 5 Products by Quantity Sold
* Identify Bottom 5 Products by Quantity Sold

### B)Sales Trend Analysis

Analyze sales performance across:

* Daily Trends
* Monthly Trends
* Quarterly Trends
* Annual Trends

### C)Profitability Analysis

* Analyze the relationship between Sales and Profit.
* Identify high-revenue but low-profit products.
* Evaluate profitability across product categories.

### D)Comparative Period Analysis

Compare:

* Sales
* Profit
* Quantity Sold

Between any two periods selected by the user through interactive filters.

### E)Discount Analysis

Determine:

* Average Discount Offered by Discount Category.
* Impact of promotions on sales performance.

### E)Order Analysis

Track:

* Total Number of Orders.
* Detailed order-level metrics.

### F)Geographic Analysis

Analyze:

* Sales by City.
* Regional business performance.

---

## Data Analysis Process

### 1. Data Cleaning

Data was cleaned and transformed to ensure:

* Data consistency
* Removal of duplicate records
* Correct data types
* Handling of missing values
* Improved reporting accuracy

### 2. Exploratory Data Analysis (EDA)

EDA was performed using **Power Query Editor**.

Activities included:

* Data profiling
* Creating additional analytical columns
* Merging and enriching transactional data using dimension tables
* Validating business logic
* Preparing datasets for reporting

### 3. Data Modeling
<img width="634" height="331" alt="Image" src="https://github.com/user-attachments/assets/0c7c984a-4b83-4e27-80e0-9948a3120b4b" />

A **Star Schema** model was implemented.

#### Dimension Tables

* DimCustomers
* DimProduct
* DimPromotions

#### Fact Table

* Fact Sheet

Relationships were created using:

* One-to-Many Cardinality
* Dimension-to-Fact Model Design

This structure improves performance, scalability, and reporting efficiency.

---

## Dashboard Features

### KPI Monitoring

The dashboard provides visibility into:

* Total Sales
* Total Profit
* Total Orders
* Total Quantity Sold
* Net Sales
* Total Discount

### Interactive Filtering

Users can dynamically filter data using:

* Product
* Date
* Customer ID
* Promotion Category

### Product Insights

* Top/Bottom Product Analysis
* Product Category Performance
* Quantity Sold Analysis

### Sales & Profit Insights

* Sales vs Profit Relationship Analysis
* Time-Series Trend Analysis
* Comparative Performance Analysis

### Regional Insights

* City-wise Sales Distribution
* Geographic Performance Comparison

### Order-Level Reporting

Detailed order analysis including:

* Sales
* Profit
* Discount
* Net Sales
* Product Details
* Customer Information
* Promotion Information

---

## Tools & Technologies Used

| Tool                  | Purpose                               |
| --------------------- | ------------------------------------- |
| Power BI              | Dashboard Development & Visualization |
| Power Query           | Data Cleaning & Transformation        |
| DAX                   | KPI and Measure Creation              |
| Data Modeling         | Star Schema Implementation            |
| Microsoft Excel / CSV | Data Source                           |

---

## Data Model

Star Schema Architecture:

```text
DimCustomers
       |
       |
       |
Fact Sheet -------- DimProduct
       |
       |
       |
DimPromotions
```

Relationships:

* One-to-Many from each Dimension Table to Fact Sheet.
* Optimized for analytical reporting and dashboard performance.

---

## Key Insights Generated

The dashboard enables stakeholders to:

* Identify best-selling and underperforming products.
* Monitor profitability trends.
* Evaluate promotional effectiveness.
* Compare business performance across custom time periods.
* Analyze customer purchasing patterns.
* Understand regional sales distribution.
* Support strategic decision-making using data-driven insights.

---

## Dashboard Outcomes

The final Power BI dashboard delivers:

✔ Interactive Reporting

✔ Dynamic Filtering

✔ Product Performance Analysis

✔ Profitability Monitoring

✔ Trend Analysis

✔ Promotion Effectiveness Tracking

✔ Regional Sales Analysis

✔ Executive-Level KPI Monitoring

---
## Dashboard Screenshorts
<img width="631" height="363" alt="Image" src="https://github.com/user-attachments/assets/840738e9-9124-4061-b007-ec251fe3ce89" />

---
<img width="630" height="365" alt="Image" src="https://github.com/user-attachments/assets/6d2c58fa-7ecd-4d25-bcf0-becd0053dce6" />

---
<img width="634" height="365" alt="Image" src="https://github.com/user-attachments/assets/c3f5c7f5-278c-4357-a0f5-4f35d83b787d" />

---
<img width="632" height="365" alt="Image" src="https://github.com/user-attachments/assets/a2709136-1bfa-46ee-89bb-fdf7fe59075b" />

---
<img width="631" height="365" alt="Image" src="https://github.com/user-attachments/assets/e4aad608-71f0-44d5-9713-803ce1c83803" />

---

## Repository Structure

```text
Departmental-Store-PnL-Analysis/
│
├── Dataset (Department Store Data - RAW)/
│   ├── DimCustomers.xlsx
│   ├── DimProduct.xlsx
│   ├── DimPromotions.xlsx
│   └── FactSheet.xlsx
├── Dataset (Department Store Data - EDA)/
│   ├── DimCustomers.csv
│   ├── DimProduct.csv
│   ├── DimPromotions.csv
│   └── FactSheet.csv
│
├── PowerBI/
│   └── Departmental Store P&L Data Analysis.pbix
│
├── Dashboard/
│   └── Departmental Store P&L Data Analysis.PDF
│   └── Screenshots.png 
│
└── README.md
```

---

## Author

**Ahsan ul haq**

Business Intelligence | Power BI | Data Analytics | Data Visualization

This project demonstrates end-to-end data analysis skills including data preparation, exploratory analysis, data modeling, KPI development, and dashboard design using Power BI.
