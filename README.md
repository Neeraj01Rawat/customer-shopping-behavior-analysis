# Customer Shopping Behavior Analysis

## Project Overview

This project analyzes customer shopping behavior using **Python, SQL, and Power BI**. The goal is to uncover insights related to customer demographics, purchasing patterns, subscription behavior, discounts, and product performance.

## Tools Used

* **Python**: Data cleaning, preprocessing, and feature engineering
* **MySQL**: Data storage and business analysis queries
* **Power BI**: Interactive dashboard and visualization
* **Pandas & SQLAlchemy**: Data manipulation and MySQL integration

## Dataset

The dataset contains customer shopping information, including:

* Customer demographics (Age, Gender, Location)
* Purchase details (Category, Item Purchased, Purchase Amount)
* Subscription status
* Discount and promo code usage
* Shipping type
* Review ratings
* Previous purchase history

## Python Data Processing

In Python, the following preprocessing steps were performed:

* Standardized column names
* Renamed `purchase_amount_(usd)` to `purchase_amount`
* Handled missing `review_rating` values using category-wise median imputation
* Created an `age_group` feature using `pd.qcut()`
* Converted purchase frequency into numerical days
* Removed redundant columns after validation
* Loaded the cleaned dataset into MySQL using SQLAlchemy

## SQL Business Analysis

Key SQL analyses performed include:

* Total revenue by gender
* Customers spending above average with discounts
* Top 5 products by average review rating
* Average purchase amount by shipping type
* Subscriber vs non-subscriber spending comparison
* Products with the highest discount purchase percentage
* Customer segmentation (New, Returning, Loyal)
* Top products within each category
* Repeat buyer subscription analysis
* Revenue contribution by age group

## Power BI Dashboard

The interactive Power BI dashboard includes:

* **KPI Cards**: Average Purchase Amount, Average Review Rating, Total Customers, Total Locations
* **Donut Chart**: Subscription status distribution
* **Bar Charts**: Revenue by Category, Orders by Category
* **Horizontal Bar Charts**: Revenue by Age Group, Orders by Age Group
* **Slicers**: Subscription Status, Gender, Category, and Shipping Type

## Dashboard Preview

![Customer Behavior Dashboard](images/dashboard_screenshot.png)

## Key Insights

* Clothing category generated the highest revenue.
* Young Adult customers contributed the highest revenue among age groups.
* A significant portion of customers were non-subscribers.
* Discount usage influenced purchasing behavior across multiple categories.
* Repeat buyers showed notable subscription engagement.

## Repository Structure

```text
customer-shopping-behavior-analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── python/
│   └── customer_behavior_analysis.ipynb
│
├── sql/
│   └── customer_behavior_queries.sql
│
├── powerbi/
│   └── Customer_Behavior_Dashboard.pbix
│
├── images/
│   └── dashboard_screenshot.png
│
└── README.md
```

## Author

**Neeraj Rawat**

This project was created as part of my Data Analyst portfolio to demonstrate end-to-end data analysis using Python, SQL, and Power BI.
