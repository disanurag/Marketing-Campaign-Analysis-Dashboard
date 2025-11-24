#  Marketing Campaign Analysis Dashboard

A Power BI dashboard to analyze and compare marketing campaign performance across regions and platforms. It helps marketing teams make data-driven decisions by tracking spend, conversions, revenue, and ROI.

---

##  Objective

To evaluate the effectiveness of marketing campaigns and identify high-ROI strategies by analyzing metrics like impressions, clicks, conversions, spend, revenue, and ROI.

---

##  Dataset Overview

- `Marketing_Campaign_Performance.csv`: Impressions, clicks, conversions, revenue, spend  
- `Marketing_Campaign_Details.csv`: Campaign names, types, platforms  
- `Region_Performance.csv`: Regional mapping and performance metrics  

---

##  Steps Followed

###  Data Preparation

- Imported 3 CSV files into Power BI  
- Renamed columns, removed nulls/duplicates  
- Corrected data types for numerical and categorical fields  

###  Data Modeling

- Built relationships:
  - Campaign Name (One-to-Many)
  - Region (One-to-Many)
- Enabled cross-filtering between tables  

---

##  DAX Measures Created

- **Total Impressions / Clicks / Conversions** – To track reach and engagement  
- **Total Revenue** – Overall earnings  
- **Total Spend** – Total marketing spend  
- **Total ROI** – Profitability  

```dax
Total ROI = (Total Revenue - Total Spend) / Total Spend * 100
```

- **Average ROI** – Benchmark for comparison  
- **Best Campaign** – Auto-selects campaign with highest ROI  

---

##  Visualizations & Insights

| Visualization         | Insight                                                |
|-----------------------|--------------------------------------------------------|
|  Stacked Column     | Spend vs Revenue by Region – spot high vs low ROI areas |
|  Combo Chart        | Spend vs Avg ROI per Campaign – detect cost-efficient campaigns |
|  Bar Chart          | ROI% by Campaign – rank top and poor performers        |
|  Pie Chart          | Campaign Type Distribution – understand marketing mix  |
|  Gauge Chart        | Total ROI vs Average ROI – overall performance check   |
|  KPI Cards          | Revenue, Spend, ROI, Best Campaign – key metrics at a glance |
|  Slicers           | Region & Campaign Type – for interactive filtering     |

---

##  Key Benefits

- See complete campaign performance in one place  
- Identify and scale high-ROI strategies  
- Optimize spend across platforms and regions  
- Interact and filter data as needed  

---

##  Limitations

- Static data – no real-time updates  
- Doesn’t include customer feedback or sentiment  
- Accuracy depends on source data quality  

---

##  Conclusion

This dashboard empowers marketing teams to **measure**, **compare**, and **optimize** their campaigns by visualizing the most important KPIs and ROI metrics.
