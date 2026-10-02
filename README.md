# TASK-1-SALES-DASHBOARD-
# 📊 Sales Data Analysis using Python & Power BI

## 📌 Project Overview

This project focuses on analyzing sales data to understand sales performance, revenue trends, customer behavior, product performance, regional performance, sales channels, discounts, and the impact of sessions attributed to sales.

The project uses **Python for data cleaning, exploratory data analysis (EDA), grouping, aggregation, and visualization**, followed by **Power BI for interactive dashboard development**.

---

## 🔴 Problem Statement

Businesses generate large amounts of sales data, but raw data alone does not provide clear information about business performance.

The main problem addressed in this project is:

> **How can sales data be analyzed to identify revenue trends, high-performing products and regions, customer behavior, sales channel performance, discount patterns, and other factors that influence overall sales performance?**

The analysis aims to transform raw sales data into meaningful business insights that can help in understanding sales performance and supporting data-driven decision-making.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Analyze overall sales and revenue performance.
* Identify the highest and lowest performing regions.
* Analyze revenue by product.
* Compare different sales channels.
* Understand customer-type performance.
* Analyze monthly revenue trends.
* Examine units sold and unit price.
* Analyze the effect of discounts on revenue.
* Study the relationship between attributed sessions and revenue.
* Identify important patterns and trends in the sales data.
* Create meaningful visualizations using Python.
* Build an interactive Power BI dashboard.
* Convert raw sales data into useful business insights.

---

## 📂 Dataset

The dataset contains sales transaction-level information.

### Dataset Columns

| Column                | Description                        |
| --------------------- | ---------------------------------- |
| `Order_id`            | Unique order identifier            |
| `Order_date`          | Date on which the order was placed |
| `Region`              | Region where the sale occurred     |
| `Product`             | Product sold                       |
| `Channel`             | Sales channel used                 |
| `Customer_type`       | Type/category of customer          |
| `Units`               | Number of units sold               |
| `Unit_price`          | Price per unit                     |
| `Discount_pct`        | Discount percentage applied        |
| `Revenue`             | Revenue generated from the order   |
| `Sessions_attributed` | Sessions attributed to the order   |
| `Month`               | Month associated with the order    |

---

# 🛠️ Tools & Technologies

### Python

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

### Power BI

* Power Query
* Data Transformation
* Data Visualization
* Interactive Dashboard
* KPI Cards
* Charts and Filters

### Other Tools

* GitHub
* Microsoft Excel

---

# 🔄 Project Workflow

```text
Raw Sales Data
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Grouping & Aggregation
      ↓
Visualization
      ↓
Business Insights
      ↓
Power BI Dashboard
      ↓
Conclusion
```

---

# 🧹 Data Cleaning & Preparation

The dataset was examined before performing the analysis.

The data preparation process included:

* Checking the dataset structure.
* Checking data types.
* Identifying missing/null values.
* Checking duplicate records.
* Converting date columns into appropriate date formats.
* Creating/using month information for monthly analysis.
* Checking numerical columns.
* Reviewing unusual or inconsistent values.
* Preparing the dataset for analysis and visualization.

---

# 📊 Exploratory Data Analysis

The analysis was performed using Python.

## 1. Revenue by Region

Revenue was grouped by `Region` to understand which regions generated higher and lower revenue.

```python
region_revenue = df.groupby("Region")["Revenue"].sum().sort_values()
print(region_revenue)
```

## 2. Monthly Revenue

Monthly revenue was analyzed to identify sales trends over time.

```python
monthly_revenue = df.groupby("Month")["Revenue"].sum().sort_values()
print(monthly_revenue)
```

## 3. Revenue by Product

Revenue was grouped by product to compare product-level performance.

```python
product_revenue = df.groupby("Product")["Revenue"].sum().sort_values()
print(product_revenue)
```

## 4. Revenue by Sales Channel

Revenue was analyzed across different sales channels to understand channel performance.

```python
channel_revenue = df.groupby("Channel")["Revenue"].sum().sort_values()
print(channel_revenue)
```

## 5. Revenue by Customer Type

Customer types were compared based on revenue contribution.

```python
customer_revenue = df.groupby("Customer_type")["Revenue"].sum().sort_values()
print(customer_revenue)
```

## 6. Revenue by Sessions Attributed

The relationship between attributed sessions and revenue was explored.

```python
session_revenue = df.groupby("Sessions_attributed")["Revenue"].sum().sort_values()
print(session_revenue)
```

## 7. Discount Analysis

Discount percentages were analyzed to understand their relationship with sales and revenue.

## 8. Units and Price Analysis

The number of units sold and unit prices were analyzed to understand sales volume and pricing patterns.

---

# 📈 Visualizations

The project includes visualizations to make the analysis easier to understand.

Examples include:

* 📊 Revenue by Region
* 📊 Revenue by Product
* 📊 Revenue by Channel
* 📊 Revenue by Customer Type
* 📈 Monthly Revenue Trend
* 📊 Units Sold Analysis
* 📊 Discount Analysis
* 📊 Sessions vs Revenue Analysis

Python visualization libraries such as **Matplotlib and Seaborn** were used.

---

# 💼 Business Questions

The project attempts to answer the following business questions:

1. Which region generates the highest revenue?
2. Which region generates the lowest revenue?
3. Which products generate the most revenue?
4. Which products have lower sales performance?
5. Which sales channel contributes the most revenue?
6. Which customer type generates the highest revenue?
7. How does revenue change across months?
8. How many units are being sold?
9. How does unit price vary across products?
10. How do discounts affect revenue?
11. Which levels of attributed sessions are associated with higher revenue?
12. Which areas of the business require further attention?
13. What patterns can be identified from the sales data?
14. How can the analysis support better business decisions?

---

# 📊 Power BI Dashboard

The cleaned sales data was also used to create an interactive **Power BI dashboard**.

The dashboard focuses on:

* Total Revenue
* Total Orders
* Total Units
* Average Unit Price
* Average Discount
* Revenue by Region
* Revenue by Product
* Revenue by Channel
* Revenue by Customer Type
* Monthly Revenue Trends
* Interactive filters and slicers

The Power BI dashboard provides a visual overview of business performance and allows users to explore different dimensions of the sales data.

---

# 🔍 Key Insights

The analysis helps identify:

* Revenue differences between regions.
* High-performing and low-performing products.
* Differences in sales channel performance.
* Revenue contribution from different customer types.
* Monthly sales patterns.
* Sales volume and pricing patterns.
* Discount patterns.
* The relationship between attributed sessions and revenue.

These insights can help businesses better understand their sales performance and identify areas that may require further investigation.

---

# 🧠 Skills Demonstrated

This project demonstrates practical skills in:

* Python for Data Analysis
* Pandas
* NumPy
* Data Cleaning
* Exploratory Data Analysis (EDA)
* `groupby()` and aggregation
* Data filtering
* Descriptive analysis
* Matplotlib
* Seaborn
* Business problem solving
* Business insights generation
* Power BI
* Dashboard development
* Data visualization
* GitHub project documentation

---

# 📁 Project Structure

```text
Sales-Data-Analysis/
│
├── Sales_Data_Analysis.ipynb
├── sales_data.csv
├── PowerBI_Dashboard.pbix
├── README.md
│
└── images/
    └── dashboard.png
```

---

# ✅ Conclusion

This project demonstrates how raw sales data can be transformed into meaningful business information using Python and Power BI.

Python was used for data preparation, exploratory data analysis, grouping, aggregation, and visualization. Different business dimensions such as region, product, channel, customer type, month, units, discounts, and sessions were analyzed to understand sales performance.

Power BI was then used to present the analysis through an interactive dashboard.

Overall, the project demonstrates the practical application of **Data Analysis, Exploratory Data Analysis, Data Visualization, and Business Intelligence** to support data-driven decision-making.

---

# 🚀 Future Improvements

The project can be further improved by:

* Adding advanced DAX measures in Power BI.
* Creating additional KPI metrics.
* Performing correlation analysis.
* Adding forecasting for future revenue.
* Conducting deeper discount and profitability analysis.
* Adding more interactive dashboard features.
* Automating the data-refresh process.
* Adding advanced statistical analysis.

---

# 👨‍💻 Author

**Gumma Venkata Naveen**

BBA Student | Aspiring Data Analyst

### Skills

`Python` `SQL` `Excel` `Power BI` `Pandas` `NumPy` `Matplotlib`

---

## ⭐ Project Purpose

This project was created as a practical **Data Analyst portfolio project** to demonstrate the complete process of converting raw sales data into meaningful business insights using **Python and Power BI**.
