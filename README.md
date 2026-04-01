# VCU Lightpole Infrastructure Dashboard
![Lightpole Dashboard](assets/Lightpoleinfra.jpeg)

## 📊 Overview
This project analyzes and visualizes campus light infrastructure data across two time periods (2016 vs 2025) using ArcGIS. The goal was to clean and integrate inconsistent datasets and build an interactive dashboard to support infrastructure insights and comparisons.

---

## 🎯 Problem
The original 2016 dataset contained inconsistencies such as duplicate identifiers and misaligned records, making it difficult to accurately compare against newer survey data from 2025.

There was no centralized way to:
- Compare light infrastructure across time
- Identify changes in asset counts
- Visualize spatial distribution of lighting assets

---

## 🛠️ Data Engineering Process
Significant effort was spent cleaning and structuring the data before visualization:

- Filtered 2016 dataset to include only VCU-owned light poles
- Resolved duplicate records (389 rows vs 112 unique poles)
- Standardized schema across 2016 and 2025 datasets
- Unified datasets into a consistent structure for comparison
- Assigned consistent Pole_ID values across all records
- Created clean latitude/longitude fields for mapping

---

## 📍 Dashboard Features
- Interactive campus map of light pole locations
- Time-based comparison between 2016 and 2025 datasets
- KPI summaries of total poles by campus and year
- Filtering by campus (MCV vs MPC)
- Visual comparison of infrastructure changes over time

---

## 🧰 Tools Used
- ArcGIS Dashboards
- Python (pandas for data cleaning and transformation)
- CSV data processing
- Excel (supporting transformations)

---

## ⚠️ Challenges & Solutions
**Challenge:** Duplicate and inconsistent identifiers in 2016 dataset  
**Solution:** Rebuilt unique Pole_ID system based on cleaned data  

**Challenge:** Aligning datasets across different formats and schemas  
**Solution:** Standardized column structures and merged datasets  

**Challenge:** Time-based visualization limitations in ArcGIS  
**Solution:** Structured data to support timeline-based filtering and comparison  

---

## 📈 Key Takeaways
- Data cleaning and structure are critical before visualization
- Real-world datasets require significant preprocessing
- Geospatial dashboards depend heavily on accurate coordinate data
- Comparing historical vs current data requires consistent schema design

---

## 🚀 Future Improvements
- Add automated data pipeline for updates
- Integrate additional infrastructure datasets
- Enhance time-series visualization capabilities
- Deploy dashboard for broader stakeholder access
