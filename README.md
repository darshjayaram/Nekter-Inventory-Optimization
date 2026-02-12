# Nekter Juice Bar Inventory Optimization System

## Overview
This project is designed to help Nekter Juice Bar’s Fremont branch reduce food waste, optimize orders, and save costs. 
Using historical sales data, ingredient recipes, and sales records, the system predicts daily ingredient demand and recommends precise order quantities. 
It combines SQL for data storage, Python for data processing and modeling, and machine learning (XGBoost) for accurate prediction.


## Key Objectives
- Forecast daily ingredient demand based on historical sales and recipes
- Convert menu items sold into ingredient usage
- Optimize order quantities using safety stock and lead time formulas
- Track inventory levels and calculate potential waste
- Provide actionable recommendations for branch management
- Quantify the amount of money and food saved


## Repo Structure
- data
    - raw – original sales and inventory files
    - processed – cleaned data ready for modeling
    - waste_logs – records of food waste
- sql
    - create_tables.sql – creates the database tables
    - insert_data.sql – inserts sample or test data
    - queries.sql – SQL queries used for analysis
- notebooks
    - 01_data_exploration.ipynb – exploring the sales and ingredient data
    - 02_feature_engineering.ipynb – creating new features like day of week and rolling averages
    - 03_modeling.ipynb – training and testing the machine learning models
- scripts
    - data_prep.py – cleans and prepares the data
    - feature_engineering.py – builds the features for the model
    - train_model.py – trains the XGBoost model
    - predict_orders.py – calculates how much of each ingredient to order
- reports
    - order_recommendations.xlsx – final order suggestions
    - waste_analysis.csv – waste and savings analysis