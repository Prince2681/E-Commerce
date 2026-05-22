# E-Commerce Sales and Profit Analysis — Python EDA Project

An end-to-end Exploratory Data Analysis project on a retail superstore dataset uncovering sales trends, profitability patterns, customer behavior, and operational insights using Python and interactive Plotly visualizations.

* * *

# Overview

This project performs a complete Exploratory Data Analysis (EDA) workflow on a retail e-commerce dataset using Python. The analysis simulates a real-world business analytics scenario where raw transactional data is transformed into actionable insights for business decision-making.

The project includes:

* Data Cleaning and Transformation
* Exploratory Data Analysis
* Feature Engineering
* Time-Series Analysis
* Profitability Analysis
* Customer Segment Analysis
* Interactive Data Visualization

Unlike traditional static reports, all visualizations are built using Plotly, enabling interactive exploration through hover analysis, zooming, filtering, and legend toggling.

* * *

# Problem Statement

Modern e-commerce businesses generate large volumes of transactional data daily. Without structured analytics, identifying sales trends, profitability gaps, customer purchasing behavior, and operational inefficiencies becomes difficult.

This project was built to answer the following business questions:

1. Which months generated the highest and lowest sales?
2. Which product categories contribute the most revenue?
3. Which sub-categories underperform despite generating strong sales?
4. How does profit vary across different months?
5. Which categories and sub-categories are most profitable?
6. Which customer segments generate the highest sales and profit?
7. How efficiently are sales converted into profit?

* * *

# Dataset Information

**Dataset:** Sample - Superstore**Domain:** Retail / E-Commerce Analytics

The dataset contains over 9,000 retail transactions across different categories, customer segments, and geographic locations.

| Column | Description |
| --- | --- |
| Order Date | Date the order was placed |
| Ship Date | Date the order was shipped |
| Customer Name | Name of customer |
| Segment | Consumer, Corporate, or Home Office |
| Category | Main product category |
| Sub-Category | Product sub-category |
| Product Name | Product description |
| Sales | Revenue generated |
| Profit | Profit earned from transaction |
| Quantity | Units sold |
| Discount | Discount applied |
| Region / State / City | Geographical information |

* * *

# Tools and Technologies

| Tool / Library | Purpose |
| --- | --- |
| Python 3.x | Core programming language |
| Pandas | Data cleaning and transformation |
| Plotly Express | Interactive visualizations |
| Plotly Graph Objects | Customized business charts |
| Jupyter Notebook | Development and analysis environment |

* * *

# Project Workflow

## Step 1 — Data Loading and Profiling

* Loaded dataset using `pd.read_csv()`
* Performed initial profiling using:
  * `.head()`
  * `.info()`
  * `.describe()`
* Checked dataset dimensions and null values

* * *

## Step 2 — Data Cleaning

* Converted `Order Date` and `Ship Date` into datetime format
* Validated datatype conversions
* Prepared dataset for time-series analysis

* * *

## Step 3 — Feature Engineering

Derived additional features from the raw order date:

* Order Month
* Order Year
* Day of Week

These engineered features enabled trend and seasonality analysis.

* * *

## Step 4 — Exploratory Data Analysis

| Analysis Type | Method Used |
| --- | --- |
| Monthly Sales Trend | `groupby(Order Month)` + `sum(Sales)` |
| Sales by Category | `groupby(Category)` + `sum(Sales)` |
| Sales by Sub-Category | `groupby(Sub-Category)` + `sum(Sales)` |
| Monthly Profit Trend | `groupby(Order Month)` + `sum(Profit)` |
| Profit by Category | `groupby(Category)` + `sum(Profit)` |
| Profit by Sub-Category | `groupby(Sub-Category)` + `sum(Profit)` |
| Segment Analysis | `groupby(Segment)` + aggregation |
| Sales-to-Profit Ratio | Derived analytical metric |

* * *

# Interactive Visualizations

The project contains multiple interactive business charts:

* Monthly Sales Trend Line Chart
* Monthly Profit Trend Line Chart
* Category-wise Sales Donut Chart
* Category-wise Profit Donut Chart
* Sub-Category Sales Bar Chart
* Sub-Category Profit Bar Chart
* Segment-wise Sales vs Profit Grouped Bar Chart
* Sales-to-Profit Ratio Analysis Table

All charts support interactive exploration using Plotly.

* * *

# Key Business Insights

## 1. Strong Seasonal Sales Pattern

Sales showed clear seasonality, with some months generating significantly higher revenue than others.

### Business Impact

* Enables seasonal inventory planning
* Improves demand forecasting
* Helps optimize marketing campaigns

* * *

## 2. Technology Category Generated Highest Revenue

Technology emerged as the highest revenue-generating category while also maintaining strong profitability margins.

### Observation

Technology products demonstrated better margin efficiency compared to Furniture products.

* * *

## 3. Certain Sub-Categories Generated Losses

Some sub-categories recorded negative profits despite generating substantial sales.

### Root Cause

Heavy discounting reduced profitability.

### Business Risk

High sales without profit optimization can negatively impact long-term sustainability.

* * *

## 4. Consumer Segment Drove Maximum Sales

The Consumer segment contributed the highest sales volume among all customer segments.

However, higher sales did not always translate into higher profit efficiency.

* * *

## 5. Feature Engineering Revealed Hidden Trends

Extracting month and weekday information from order dates uncovered important trends invisible in the raw transactional data.

This demonstrates the importance of feature engineering in business analytics.

* * *

# Business Recommendations

Based on the analysis, the following recommendations can improve operational efficiency and profitability:

* Reduce excessive discounting in loss-making sub-categories
* Increase inventory preparation during peak sales periods
* Invest more in high-margin Technology products
* Improve pricing strategies for low-profit products
* Monitor sub-categories with strong sales but poor profitability
* Build forecasting models for proactive business planning

* * *

# Quantified Results

* Technology contributed the highest share of total sales revenue
* Consumer segment generated the largest portion of overall sales
* Several sub-categories recorded negative total profit
* Monthly sales and profit demonstrated strong seasonality
* Sales-to-Profit Ratio analysis identified profitability inefficiencies across customer segments

* * *

# Repository Structure

    ecommerce-sales-profit-analysis/
    │
    ├── Ecommerce.ipynb
    ├── Sample - Superstore.csv
    ├── README.md
    │
    ├── images/
    │   ├── monthly_sales.png
    │   ├── sales_category.png
    │   ├── profit_subcategory.png
    │   └── segment_analysis.png

* * *

# How to Run This Project

## Step 1 — Clone Repository

    git clone https://github.com/Prince2681/ecommerce-sales-profit-analysis.git

* * *

## Step 2 — Navigate to Project Directory

    cd ecommerce-sales-profit-analysis

* * *

## Step 3 — Install Dependencies

    pip install pandas plotly notebook

* * *

## Step 4 — Launch Jupyter Notebook

    jupyter notebook Ecommerce.ipynb

* * *

# Results and Conclusion

This project successfully demonstrates a complete end-to-end Exploratory Data Analysis workflow using Python and Plotly.

The analysis uncovered:

* Seasonal sales patterns
* Category-level profitability gaps
* Loss-making product segments
* Customer segment purchasing behavior
* Operational inefficiencies

The project also demonstrates industry-relevant analytical skills including:

* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Interactive Dashboarding
* Business Insight Generation
* Analytical Storytelling

* * *

# Future Improvements

Future enhancements for this project include:

* Building Machine Learning forecasting models
* Customer segmentation using RFM analysis
* Deploying an interactive Streamlit dashboard
* Integrating SQL-based analytical workflows
* Creating Power BI dashboards
* Performing discount optimization analysis

* * *

# Skills Demonstrated

* Python Programming
* Pandas Data Analysis
* Exploratory Data Analysis (EDA)
* Data Cleaning and Transformation
* Feature Engineering
* Business Analytics
* Interactive Data Visualization
* Analytical Thinking
* Data Storytelling

* * *

# Author

## Ankit Saini

Data Analytics | Python | SQL | Exploratory Data Analysis | Data Visualization

📧 Email: princesaini2681@gmail.com💼 LinkedIn: linkedin.com/in/ankit-saini-6aaba781

* * *

#
