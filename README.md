Vendor Invoice Risk Detection & Freight Cost Analytics
Overview-

This project analyzes vendor invoice and purchase order data to understand transaction patterns and identify potentially risky invoices. The analysis combines SQL-based feature engineering, exploratory data analysis (EDA), and machine learning to generate insights and build predictive models.The dataset is stored in a SQLite database and processed using Python. The project also includes a small Streamlit application that allows users to interact with the trained models.

Project Goal-

The goal of this project is to use data analytics techniques to:
-analyze vendor invoice and purchase order data
-identify patterns that may indicate invoice anomalies
-predict freight costs associated with invoices
-flag invoices that may require manual verification

This helps demonstrate how data analytics can support financial monitoring and operational decision-making.

Components of this project -

1)Exploratory Data Analysis (EDA)

Exploratory analysis was performed to better understand the dataset and identify useful relationships.

Key analysis included:
-Handling missing values
-distribution of invoice and freight values
-comparison between invoice value and purchase order value
-correlation analysis between features
-examination of payment and receiving delays
Visualizations were created using libraries Matplotlib and Seaborn to better interpret patterns in the data.

2)Data Processing & Feature Engineering

Data is extracted from a SQLite database containing two main tables:
-vendor_invoice
-purchases

Using SQL joins and aggregations, additional analytical features were created, including:
-total purchase value
-total item quantity
-number of brands per purchase order
-receiving delays
-time difference between purchase order, invoice, and payment

These features provide useful context for understanding invoice behavior.

3)Predictive Models

Two machine learning tasks were implemented:

-Freight Cost Prediction
A regression model predicts freight cost based on invoice and purchase features.

Models evaluated:
Linear Regression
Decision Tree
Random Forest

-Invoice Risk Detection

A classification model identifies invoices that may require manual review.
A Random Forest classifier with hyperparameter tuning was used and evaluated using metrics such as accuracy and F1 score.

4)Streamlit Application

The project includes an interactive dashboard where users can:

enter invoice details

estimate freight cost

check whether an invoice may require manual review

 **Final Result **

The project produces two trained models:

Freight prediction model for estimating shipping cost

Invoice risk classification model for identifying suspicious invoices

These models are saved and integrated into a Streamlit dashboard, allowing users to input invoice details and obtain predictions in real time.

PROJECT STRUCTURE

data/                   → SQLite database  
freight_cost_prediction/ → freight prediction pipeline  
invoice_flagging/       → invoice risk detection pipeline  
inference/              → prediction scripts  
models/                 → saved trained models  
notebooks/              → exploratory data analysis and experimentation  
app.py                  → Streamlit dashboard

Skills Demonstrated

-SQL data extraction and feature engineering
-exploratory data analysis and visualization
-machine learning model development
-model evaluation and tuning
-building a simple data application using Streamlit

Author
Anurag Krishna
Python Developer | Data Analytics & Machine Learning
