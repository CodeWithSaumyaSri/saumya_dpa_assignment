Hotel Booking Data Analysis
Data preparation, exploratory data analysis (EDA), visualization, and feature engineering on the Hotel Booking Demand dataset using Python.
This project was completed for the M.Tech CSE (Artificial Intelligence) course Data Preparation and Analysis. It examines booking patterns, cancellations, guest and stay characteristics, and pricing trends across City and Resort Hotels.
Dataset

Name: Hotel Booking Demand
Raw data: 119,390 records and 32 columns
After cleaning: 87,395 records
Includes: Booking status, arrival dates, stay duration, guest counts, room details, lead time, Average Daily Rate (ADR), meal plans, and booking channels

Objectives

Inspect the dataset’s structure and quality.
Clean missing values, duplicates, data types, and outliers.
Explore numerical and categorical data and their relationships.
Create static and interactive visualizations.
Engineer useful features and summarize key insights.

Workflow

Data inspection: Reviewed dimensions, columns, types, descriptive statistics, missing values, and duplicates.
NumPy analysis: Used array operations and calculated statistical measures for ADR and lead time.
Data cleaning:
Standardized column names to lowercase with underscores.
Converted date-related columns to integer types.
Filled missing children values with 0 and missing country values with Unknown.
Retained missing agent and company values.
Removed 31,994 duplicate rows and one record with a negative ADR.


Outlier analysis: Flagged 2,490 ADR outliers using the IQR method (upper bound: 227.00). Created a 99th-percentile capped ADR column (261.41) to support visualization without removing records.
EDA and visualization: Examined distributions, cancellation rates, hotel-level comparisons, categorical data, and monthly arrival trends.

Key Findings

Overall cancellation rate: 27.49%
City Hotels: 30.04%
Resort Hotels: 23.48%


Bookings by hotel type: 53,428 City Hotel; 33,967 Resort Hotel
ADR: Mean 106.34; median 98.10
Lead time: Mean 79.89 days; median 49 days
Leading market segment: Online TA (51,618 bookings)
Leading distribution channel: TA/TO (69,141 bookings)
Most common meal type: BB (Bed & Breakfast; 67,977 bookings)

Libraries

NumPy
Pandas
Matplotlib
Plotly
