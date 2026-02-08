# 🗽 NYC Yellow Taxi Trip Analysis (2023)

[![Python](https://img.shields.io/badge/python-3.x-blue)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)
[![Platform](https://img.shields.io/badge/Platform-Colab-red)](https://colab.research.google.com/)

---

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Description](#dataset-description)
- [Tools and Libraries](#tools-and-libraries)
- [Analysis Workflow](#analysis-workflow)
- [Key Insights](#key-insights)
- [How to Run](#how-to-run)
- [Future Scope](#future-scope)
- [Author](#author)

---

## 📘 Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on NYC Yellow Taxi Trip data for 2023. The analysis aims to uncover patterns in passenger behavior, fare structures, trip demand, and revenue trends.  

The insights can help optimize taxi operations, improve pricing strategies, and enhance service quality.

---

## 🎯 Objectives
- Clean and preprocess raw trip data.
- Handle missing, zero, and negative values.
- Analyze fare components (fare, tip, surcharge, tolls).
- Study trip characteristics (distance, duration, passenger count).
- Explore temporal trends (hourly, daily, monthly patterns).
- Investigate geographical patterns using pickup and drop-off zones.
- Visualize correlations and relationships between variables.
- Derive actionable insights to improve taxi operations.

---

## 🧩 Dataset Description
- **Source:** NYC Taxi & Limousine Commission (TLC) trip record data.
- **Sample Fields:**
  - `VendorID`, `passenger_count`, `trip_distance`, `RatecodeID`
  - `PULocationID`, `DOLocationID`, `payment_type`
  - `fare_amount`, `extra`, `mta_tax`, `tip_amount`, `tolls_amount`
  - `improvement_surcharge`, `total_amount`, `congestion_surcharge`, `airport_fee`
  - `pickup_datetime`, `dropoff_datetime`
- **Volume:** ~300,000 rows sampled for analysis.

---

## 🧮 Tools & Libraries
| Purpose             | Libraries/Tools              |
|--------------------|------------------------------|
| Data Manipulation  | pandas, numpy               |
| Data Cleaning      | pandas, datetime            |
| Visualization      | matplotlib, seaborn, plotly |
| Environment        | Jupyter Notebook (Python 3.x)|

---

## ⚙️ Analysis Workflow
### 1. Data Overview
- Loaded and inspected the dataset.
- Checked column types, missing values, and duplicates.

### 2. Data Cleaning
- Removed duplicates.
- Handled missing, zero, or negative values.
- Converted datetime columns and extracted new features (`hour`, `weekday`, `month`).

### 3. Feature Engineering
- Created features: `trip_duration`, `pickup_hour`, `tip_percentage`, `distance_category`.

### 4. Exploratory Analysis
- Passenger count and trip distance distributions.
- Fare, tip, and surcharge patterns.
- Temporal trends (hourly, daily, monthly, quarterly).
- Geographical trends using pickup/drop-off zones.

### 5. Statistical Insights
- Correlation analysis between numerical features.
- Detection and handling of outliers.
- Summary statistics and distribution patterns.

### 6. Visualization
- Bar charts, histograms, scatter plots, line plots, heatmaps, pie charts.
- Color-coded maps for zone-wise trip activity.

---

## 📊 Key Insights
- Most trips involve 1–2 passengers with short distances (<5 miles).  
- Trip demand peaks between **3 PM – 7 PM**, with 6 PM being the busiest hour.  
- Nighttime trips generate higher revenue per mile due to tips and surcharges.  
- Tips are higher for shorter trips and solo passengers.  
- Surcharges vary by pickup zone and time, with extra charges common between 12–6 AM.  
- Vendor 2 generally charges more per mile, particularly for shorter trips.  

---
## 📈 Future Scope
- Geospatial visualization using **Folium** or **GeoPandas**  
- Statistical hypothesis testing on fare and tip variations  
- Predictive modeling: fare estimation and demand forecasting  
- Automated report generation in Python  

---

## 👤 Author
**Pratiksha Wagaj**  
Data Analyst | NYC Taxi EDA Project  
[GitHub Repository](https://github.com/wagajpratiksha/EDA_NYC_Taxi_Analysis)
