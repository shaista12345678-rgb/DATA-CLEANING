# DATA-CLEANING
This project focuses on building a robust data-cleaning and preprocessing pipeline for a messy customer orders dataset (Messy_data.csv). The primary goal is to transform raw, inconsistent data into a structured, structured, and analysis-ready format.

Key Pipeline Steps:
Data Inspection & Deduplication: Analyzed dataset structure, identified missing values, and successfully removed 5 duplicate records.
Text Standardization: Standardized textual fields (CustomerName, City, Product, and OrderStatus) by stripping leading/trailing whitespaces and converting them into uniform Title Case.
Numeric Conversions: Converted Quantity, UnitPrice, and CustomerAge columns into numerical types, safely handling non-numeric inconsistencies.
Imputation of Missing Values: Filled missing entries strategically using averages (means) for numeric features like UnitPrice, Quantity, CustomerAge, and OrderDate, while filling categorical gaps with 'Unknown' values.
Outlier Mitigation: Calculated Interquartile Range (IQR) boundaries for UnitPrice to pinpoint extreme outliers (such as values up to 999,999.00) and capped them safely using clipping techniques.
Feature Engineering: Created a new feature Total_Price by multiplying the clean Quantity and UnitPrice columns.
Export: Saved and automatically downloaded the fully processed dataset as a clean, standardized CSV file (cleaned_data.csv).
