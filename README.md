# 👨🏻‍💻Customer Behavior Data Analyst Project
This project represents a complete, industry standard, end-to-end data analytics workflow, designed to mirror the real responsibilities of professional analysts in modern business environments. The project encompasses all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.

## 1. Project Overview
The goal of this project is to simulate a corporate-grade end-to-end data analytics workflow, demonstrating the ability to translate raw data into strategic business intelligence by:

✅ Data Preparation,Modeling & Exploratory Data Analysis (Python): Clean and transform the raw dataset for analysis.

✅ Data Analysis (SQL): Simulate business transactions, and run queries to extract insights on customer segments, loyalty, and purchase drivers.

✅ Visualization & Insights (Power BI): Build an interactive dashboard that highlights key patterns and trends, enabling stakeholders to make data-driven decisions.

✅ Report: Write a clear project report summarizing your key findings and business recommendations. 

## 2. Technical Stack

This project leverages industry-standard tools for each phase of the analysis:

| Phase | Tools/Techniques | Purpose |
| :--- | :--- | :--- |
| **Data Cleaning & Preparation** | Python (Pandas) | Data consistency (snake casing), feature engineering, and robust missing value imputation. |
| **Advanced Analysis & Storage** | SQL (PostgreSQL/MySQL/MSSQL Server) | Deep data analysis using complex queries (e.g., subqueries, window functions) to answer specific business questions. |
| **Visualization & Reporting** | Power BI | Creating a sleek, interactive dashboard for tracking KPIs and facilitating business decisions. |
| **Documentation & Showcase** | Project Report and GitHub | Official documentation and public portfolio showcase. |

## 3. Key Methodology Highlights

The project focused on using smart, professional techniques to extract trustworthy insights from the customer shopping behavior data set:

### A. Data Manipulation (Python)

*   **Smart Imputation:** Missing `review_rating` values were imputed using the **median review rating within each item category** to avoid introducing bias and respect natural differences between categories (e.g., clothing vs. footwear).
*   **Data Consistency:** All column names were converted to **snake casing** (lowercase with underscores) for easier referencing in both Python and SQL.
*   **Feature Engineering:** Created `age_group` by splitting customers into four equal-sized groups using `pd.qcut`, and converted textual `frequency_of_purchases` (e.g., 'weekly') into a numeric column (`purchase_frequency_days`) for easier analysis.
*   **Redundancy Check:** Confirmed that `discount_applied` and `promo_code_used` carried identical information, and the redundant `promo_code_used` column was dropped.

### B. Deep Analysis (SQL)

Advanced SQL queries were used to answer crucial business questions regarding revenue and loyalty, including:

*   **Customer Segmentation:** Segmenting customers into **New** (1 previous purchase), **Returning** (2-10 previous purchases), and **Loyal** (more than 10 previous purchases).
*   **Product Ranking:** Identifying the top three most purchased products within each category using the **`ROW_NUMBER()` window function**.
*   **Discount Effectiveness:** Identifying customers who used a discount but still spent more than the overall average purchase amount.
*   **Subscription Value:** Comparing the total customer count, average spend, and total revenue between subscribers and non-subscribers to evaluate the program's success.
*   **Revenue Drivers:** Determining that **Young Adults drive the most revenue** compared to other segmented age groups (middle-aged, adult, senior).

### C. Visualization (Power BI)

An interactive dashboard was built featuring Key Performance Indicators (KPIs) like total customers, average purchase amount, and average review rating. Visualizations include charts displaying Revenue and Sales split by Category and Age Group, alongside slicers for dynamic filtering by Subscription Status, Gender, and Shipping Type.

## 4. Deliverables

This repository contains all necessary files for replication and review:

*   Python scripts/Jupyter Notebooks (data cleaning and feature engineering).
*   SQL Scripts (advanced business analysis queries).
*   Power BI file (`.pbix`).
*   Project Report .
