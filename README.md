Customer Shopping Behaviour Analysis

An end-to-end data analysis project exploring shopping behaviour across 3,900 customers, covering the full pipeline from raw data to insights — data cleaning, SQL-based business analysis, and an interactive dashboard.

Project Overview

This project analyses customer transaction data to understand purchasing patterns, revenue drivers, and customer segments. The workflow spans three stages:

Data Cleaning & Feature Engineering — Python (pandas)
Business Analysis — SQL (PostgreSQL)
Visualization — Interactive Excel Dashboard
Dataset
File: customer_shopping_behavior.csv
Size: 3,900 records, 18 raw attributes
Attributes include: Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount, Review Rating, Subscription Status, Shipping Type, Discount Applied, Previous Purchases, Frequency of Purchases, and more.
Tech Stack
Stage	Tool
Data cleaning & feature engineering	Python (pandas)
Database & analysis	PostgreSQL (SQL)
Visualization	Excel Dashboard
Repository Contents
├── customer_shopping_behavior.csv        # Raw dataset
├── customer_shopping_behavior.ipynb      # Data cleaning & PostgreSQL load (Python)
├── sql_queries.sql                       # 10 business-question SQL queries
├── dashboard.xlsx                        # Interactive Excel dashboard
└── Customer_Shopping_Behaviour_Report    # Full project report (.docx)
Data Cleaning & Feature Engineering

Performed in Python using pandas:

Imputed missing Review Rating values using the category-wise median.
Standardized column names (lowercase, underscores).
Dropped promo_code_used (identical to discount_applied).
Engineered age_group (quartile-based bucket) and purchase_frequency_days.
Loaded the cleaned dataset into PostgreSQL via SQLAlchemy.
SQL Analysis

Ten business questions answered using SQL on PostgreSQL, including:

Revenue by gender
High-spending discount users
Top-rated products
Shipping type comparison
Subscriber vs. non-subscriber spend
Most-discounted products
Customer loyalty segmentation (New / Returning / Loyal)
Top products per category
Repeat buyers vs. subscription likelihood
Revenue contribution by age group

Full query set available in sql_queries.sql.

Dashboard

An interactive Excel dashboard with KPI cards, revenue/sales breakdowns by category and age group, and slicers for Subscription Status, Gender, Category, and Shipping Type.

Report

A detailed project report (data used, code, SQL queries with results, dashboard walkthrough) is available in the repo as a Word document.
