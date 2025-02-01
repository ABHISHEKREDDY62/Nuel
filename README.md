# Retail Stores Sales Analysis

## Overview

This project focuses on analyzing sales and customer behavior across multiple retail stores to derive actionable insights, identify key trends, and make data-driven recommendations. The analysis covers various aspects such as sales trends, geographical performance, product categories, customer segmentation, and the impact of external factors like holidays.

## Table of Contents

1. [Problem Definition](#problem-definition)  
2. [Dataset Information](#dataset-information)  
3. [Project Workflow](#project-workflow)  
4. [Key Insights](#key-insights)  
5. [Advanced Analysis](#advanced-analysis)  
6. [Tools and Libraries](#tools-and-libraries)  
7. [Recommendations](#recommendations)  
8. [How to Run the Project](#how-to-run-the-project)  

---

## Problem Definition

The goal of this project is to analyze sales and customer behavior across multiple stores and provide actionable insights to improve sales, customer engagement, and product placement strategies.

### Key Objectives:

- Identify sales trends.  
- Highlight top and low-performing product categories.  
- Assess the impact of external factors like holidays and location.  
- Segment customers based on purchasing behavior.  
- Provide recommendations for optimizing sales and product placements.  

---

## Dataset Information

- **Source:** Kaggle  
- **Dataset:** [Different_stores_dataset.csv](https://www.kaggle.com/datasets/kzmontage/sales-from-different-stores?select=Different_stores_dataset.csv) 
- **Size:** 99,457 rows with essential columns such as `date`, `product category`, `quantity`, `price`, `customer demographics`, and `location` etc.  


### Holiday Data Integration

A custom dataset containing U.S. public holidays in 2016 was merged with the main dataset to analyze the impact of holidays on sales.  

---

## Project Workflow

1. **Data Collection:** Collected the retail dataset and external holiday data.  
2. **Data Cleaning:** Handled missing values, removed duplicates, and corrected region-state mapping.  
3. **Feature Engineering:** Created new features like `invoice_month`, `profit_per_unit`, and `invoice_value` to analyze profitability and seasonality.  
4. **Exploratory Data Analysis (EDA):** Visualized key trends, regional performance, customer demographics, and category-wise insights.  
5. **Regression Analysis:** Built Linear Regression and Random Forest models to identify key drivers of sales.  
6. **Customer Segmentation:** Used K-Means clustering to group customers based on demographics and spending behavior.  
7. **Sales Forecasting:** Implemented ARIMA, SARIMAX and Exponential Smoothing models to predict future sales.  

---

## Key Insights

### 1. Sales Trends  

- Sales peak in **November** and towards the **end of each month**.  
- Holiday periods show a significant increase in sales, with an **average transaction value being $53 higher on holidays** compared to non-holiday days.  

### 2. Regional Performance  

- **Top Performing Region:** **West**  
- **Lowest Performing Region:** **Central**  
- **Top Performing State:** **California**  
- **Lowest Performing State:** **Kentucky**
- **Top Performing Mall:** **Mall of Istanbul** (highest sales & profit).  
- **Lowest Performing Malls:**  
  - **By Sales:** **Metropol AVM**  
  - **By Profit:** **Istinye Park**  

### 3. Product Category Performance  

- **Best-Selling Category:** **Clothing** (Consistently highest in both profit and sales).  
- **Lowest-Selling Category:** **Books** (by sales) and **Food & Beverages** (by profit).  
- **Holiday Best Seller:** **Technology**  
- **Holiday Lowest Performer:** **Food & Beverages**  

### 4. Customer Behavior  

- **Majority of purchases are made by females.**  
- Customers aged **20-50** are responsible for the highest purchase volumes.  
- Sales at the **end of the month** are higher compared to the start.  

### 5. Payment Preferences  

- **Most preferred payment method:** **Cash**  
- **Credit cards are preferred over debit cards by sales, but debit cards yield higher profit margins.**  

---

## Advanced Analysis

### Predictive Modeling  

- **Regression Models:**  
  - **Random Forest Regressor** identified top features influencing invoice value.  
  - **Key drivers:** `selling_price_per_unit`, `invoice_profit`, `cost_price_per_unit`.  
- **Time Series Forecasting:**  
  - **SARIMAX** performed better than ARIMA and Exponential Smoothing in capturing seasonality.  



 

---

## Tools and Libraries  

The project was developed using the following libraries:  

- **Python Libraries:**  
  - `pandas`, `numpy` – Data manipulation  
  - `matplotlib`, `seaborn`, `plotly` – Visualization  
  - `scikit-learn` – Machine learning models  
  - `statsmodels` – Time series forecasting   

---
