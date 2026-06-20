# 🚚 Zomato Delivery Operations Analytics

## 📌 Project Overview

This project analyzes Zomato delivery operations data to identify the key factors affecting delivery performance and customer experience.

Using Python-based data analysis techniques, the project explores the impact of traffic conditions, weather, rider ratings, festivals, delivery distance, and multiple deliveries on delivery time.

The project also includes feature engineering, outlier handling, business insights, and recommendations for improving operational efficiency.

---

## 🎯 Objectives

* Analyze delivery operations data
* Identify factors affecting delivery time
* Engineer new features from geographical coordinates
* Detect and handle data quality issues
* Generate actionable business insights
* Prepare data for delivery time prediction models

---

## 📊 Dataset Information

Dataset: Zomato Delivery Operations Analytics

### Dataset Summary

| Metric          | Value            |
| --------------- | ---------------- |
| Records         | 45,584           |
| Features        | 20               |
| Target Variable | Time_taken (min) |

### Key Features

* Delivery Person Age
* Delivery Person Ratings
* Weather Conditions
* Road Traffic Density
* Vehicle Condition
* Type of Order
* Type of Vehicle
* Multiple Deliveries
* Festival
* City
* Restaurant Coordinates
* Delivery Coordinates
* Time Taken (min)

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 📂 Project Workflow

### 1. Data Understanding

* Dataset exploration
* Data type inspection
* Missing value analysis
* Statistical summary

### 2. Data Cleaning

* Missing value treatment
* Duplicate removal
* Data type conversion
* Handling invalid records

### 3. Feature Engineering

A new feature named **Distance_km** was created using restaurant and delivery coordinates.

The Haversine Formula was used to calculate geographical distance between two locations.

### 4. Outlier Detection

During analysis, several coordinate anomalies generated unrealistic distances exceeding 19,000 km.

A percentile-based approach was used to remove these outliers before conducting further analysis.

### 5. Exploratory Data Analysis

Business-focused analysis was performed on:

* Traffic Density
* Weather Conditions
* Festivals
* Multiple Deliveries
* Rider Ratings
* Delivery Distance

---

## 📈 Key Findings

### 🚦 Traffic Density Impact

| Traffic Condition | Avg Delivery Time |
| ----------------- | ----------------- |
| Low               | 21.27 min         |
| Medium            | 26.71 min         |
| High              | 27.23 min         |
| Jam               | 31.18 min         |

**Insight:** Delivery time increased by approximately 46% under jam traffic conditions.

---

### 📦 Multiple Deliveries Impact

| Multiple Deliveries | Avg Delivery Time |
| ------------------- | ----------------- |
| 0                   | 22.87 min         |
| 1                   | 26.86 min         |
| 2                   | 40.44 min         |
| 3                   | 47.81 min         |

**Insight:** Delivery time more than doubled when riders handled three deliveries simultaneously.

---

### 🎉 Festival Impact

| Festival | Avg Delivery Time |
| -------- | ----------------- |
| No       | 25.99 min         |
| Yes      | 45.51 min         |

**Insight:** Festival periods increased average delivery time by approximately 75%.

---

### 🌦️ Weather Impact

| Weather | Avg Delivery Time |
| ------- | ----------------- |
| Sunny   | 21.85 min         |
| Fog     | 28.93 min         |

**Insight:** Adverse weather conditions significantly increased delivery time.

---

### ⭐ Rider Ratings

Correlation between rider ratings and delivery time:

```text
-0.344
```

**Insight:** Higher-rated riders generally completed deliveries faster.

---

### 📍 Delivery Distance

Correlation between delivery distance and delivery time:

```text
0.322
```

**Insight:** Longer delivery distances moderately increased delivery duration.

---

## 🏆 Major Business Insights

### Most Influential Factors Affecting Delivery Time

| Rank | Factor              |
| ---- | ------------------- |
| 1    | Multiple Deliveries |
| 2    | Festival            |
| 3    | Traffic Density     |
| 4    | Rider Ratings       |
| 5    | Delivery Distance   |
| 6    | Weather Conditions  |

---

## 💡 Business Recommendations

* Limit excessive batch deliveries during peak hours.
* Increase rider availability during festivals.
* Use dynamic routing under heavy traffic conditions.
* Incorporate weather conditions into ETA calculations.
* Improve training and monitoring for low-rated riders.
* Optimize assignment of long-distance deliveries.

---

## 📸 Visualizations

The project includes:

* Distribution Plots
* Bar Charts
* Box Plots
* Scatter Plots
* Correlation Heatmaps
* Operational Performance Analysis

---

## 📁 Repository Structure

```text
Zomato-Delivery-Analytics/
│
├── data/
│   └── zomato.csv
│
├── notebooks/
│   └── zomato_analysis.ipynb
│
├── visualizations/
│
├── report/
│   └── project_report.pdf
│
├── README.md
│
└── requirements.txt
```

---

## 🚀 Future Enhancements

* Delivery Time Prediction using Machine Learning
* Random Forest Regressor
* Feature Importance Analysis
* Interactive Dashboard using Power BI
* Real-Time ETA Prediction
* Route Optimization Analysis

