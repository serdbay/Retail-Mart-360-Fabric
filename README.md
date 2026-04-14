# Retail-Mart-360-Fabric
# 🛒 RetailMart360 — MS Fabric Analytics Platform

![Microsoft Fabric](https://img.shields.io/badge/Microsoft%20Fabric-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apache-spark&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta%20Lake-00ADD8?style=for-the-badge&logo=delta&logoColor=white)

## 📌 Project Overview
End-to-end analytics platform for a multinational retail company migrating from legacy Excel systems to Microsoft Fabric. Built as part of the MS Fabric Elite Architect Bootcamp.

**Sector:** Retail | **Dataset:** Kaggle Real Retail Sales Data | **Scale:** 10M+ revenue, 19 countries

---

## 🏗️ Architecture
Raw Data (CSV)
↓
[Bronze Layer] — Raw ingestion, no transformation
↓
[Silver Layer] — Cleaned, deduplicated, typed
↓
[Gold Layer] — Star Schema, aggregations, rankings
↓
[Power BI] — Interactive Dashboard

## ⚙️ Tech Stack
- **Platform:** Microsoft Fabric (Lakehouse, Notebooks, Pipelines)
- **Processing:** PySpark, Delta Lake
- **Modeling:** Star Schema, SCD Type 1 & 2
- **Analytics:** DAX, Power BI
- **Orchestration:** Fabric Data Pipeline
- **Version Control:** GitHub

---

## 📊 Data Model (Star Schema)

| Table | Type | Description |
|-------|------|-------------|
| fact_sales | Fact | Core sales transactions |
| dim_customer | Dimension | Customer master data (SCD Type 2) |
| dim_product | Dimension | Product catalog |
| dim_geography | Dimension | 19 countries, cleaned & deduplicated |
| dim_date | Dimension | Date hierarchy |
| dim_store | Dimension | Store information |

---

## 🔧 Key Features

### Data Engineering
- ✅ Medallion Architecture (Bronze → Silver → Gold)
- ✅ SCD Type 1 & 2 implementation
- ✅ Window Functions (RANK, LAG, MoM Change)
- ✅ Data Quality Framework (5 validation rules)
- ✅ Incremental Load with Watermark Pattern
- ✅ Delta Lake Optimization (OPTIMIZE, VACUUM, Z-ORDER)
- ✅ Automated Pipeline with error notifications

### Analytics & BI
- ✅ Advanced DAX (MTD, YTD, SAMEPERIODLASTYEAR)
- ✅ Country ranking & trend analysis
- ✅ Month-over-Month change tracking
- ✅ Interactive Power BI Dashboard

---

## 📈 Business Metrics
- **Total Revenue:** $10.03M
- **Total Orders:** 307
- **Avg Revenue:** $32.68K
- **Top Market:** USA ($3.6M)
- **Countries:** 19 across EMEA, APAC, NA

---

## 🚀 Pipeline Architecture
star_schema_notebook
↓
scd_notebook
↓
data_quality_notebook
↓
optimization_notebook
↓
error_notification_notebook

---

## 📁 Project Structure
retail-mart-360-fabric/
├── notebooks/
│   ├── star_schema_notebook.ipynb
│   ├── scd_notebook.ipynb
│   ├── data_quality_notebook.ipynb
│   └── optimization_notebook.ipynb
├── docs/
│   └── architecture_diagram.png
└── README.md

---

## 🎯 Skills Demonstrated
`Microsoft Fabric` `PySpark` `Delta Lake` `Star Schema` `SCD` `DAX` `Power BI` `Data Pipeline` `Data Quality` `Medallion Architecture` `Incremental Load` `Git`
