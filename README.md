# 📊 Marketing Campaign Analysis Dashboard

A Power BI dashboard to analyze and compare marketing campaign performance across regions and platforms. It helps marketing teams make data-driven decisions by tracking spend, conversions, revenue, and ROI.

---

## 🎯 Objective

To evaluate the effectiveness of marketing campaigns and identify high-ROI strategies by analyzing metrics like impressions, clicks, conversions, spend, revenue, and ROI.

---

## 📁 Dataset Overview

- `Marketing_Campaign_Performance.csv`: Impressions, clicks, conversions, revenue, spend
- `Marketing_Campaign_Details.csv`: Campaign names, types, platforms
- `Region_Performance.csv`: Regional mapping and performance metrics

---

## ⚙️ Steps Followed

### ✅ Data Preparation
- Imported 3 CSV files into Power BI
- Renamed columns, removed nulls/duplicates
- Corrected data types for numerical and categorical fields

### ✅ Data Modeling
- Built relationships:
  - Campaign Name (One-to-Many)
  - Region (One-to-Many)
- Enabled cross-filtering between tables

### ✅ DAX Measures
- **Total Impressions / Clicks / Conversions** – Track reach and engagement
- **Total Revenue** – Overall earnings
- **Total Spend** – Total budget used
- **Total ROI** – Profitability  
  ```dax
  Total ROI = (Total Revenue - Total Spend) / Total Spend * 100
  ```
  Average ROI – Benchmark to compare individual campaigns
  Best Campaign – Auto-select campaign with highest ROI
  
📊 Visualizations & Insights
Visualization	Insight
📊 Stacked Column Chart	Spend vs Revenue by Region – spot high vs low ROI areas
📈 Combo Chart	Spend vs Avg ROI per Campaign – detect cost-efficient campaigns
📉 Bar Chart	ROI% by Campaign – rank top and poor performers
🥧 Pie Chart	Campaign Type Distribution – understand marketing mix
🧭 Gauge Chart	Total ROI vs Average ROI – overall performance check
🧾 KPI Cards	Revenue, Spend, ROI, Best Campaign – key metrics at a glance
🎛️ Slicers	Region & Campaign Type – interactive filtering for deep dive
