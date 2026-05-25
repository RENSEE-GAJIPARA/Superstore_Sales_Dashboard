# 📊 Superstore Business Insights Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Data%20Analytics-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed%20✅-brightgreen?style=for-the-badge)

> **Interactive Power BI Dashboard** — Analysis of Sales, Profit, Customers & Regional Performance  
> 🏫 *Red & White Skill Education | Power BI · Practical Report 1 (PR 1)*

---

## 📌 Dashboard Overview

This Power BI project is built on the **Sample Superstore Sales Dataset** (Kaggle) and delivers a fully interactive business intelligence dashboard. It enables stakeholders to explore sales trends, profitability by category, top customers, regional performance, and monthly revenue patterns — all through dynamic slicers and cross-filtering visuals.

**Key Metrics at a Glance:**

| Metric | Value |
|---|---|
| 💰 Total Profit | 226.10K |
| 🛒 Total Sales | 1,867.55K |
| 📦 Total Quantity | 31K |
| 🏷️ Average Discount | 0.16 |

---

## 📁 Dataset Used

| Field | Detail |
|---|---|
| **Dataset Name** | Sample Superstore Sales Dataset |
| **Source** | Kaggle |
| **URL** | [Superstore Dataset – Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) |
| **Format** | CSV / Excel (.xlsx) |
| **Rows** | ~9,994 rows |
| **Key Columns** | Order Date, Ship Date, Ship Mode, Segment, Country, City, State, Region, Category, Sub-Category, Product Name, Sales, Quantity, Discount, Profit |

---

## 🔧 Power Query Steps

The following data transformation steps were applied in **Power Query Editor** before loading into the data model:

| # | Step | Details |
|---|---|---|
| 1 | **Connect to Data** | Loaded CSV via Home → Get Data → CSV |
| 2 | **Rename Columns** | Renamed `Sub-Category` → `Sub Category`, and 2 other columns for readability |
| 3 | **Change Data Types** | Order Date → Date · Sales → Decimal · Quantity → Whole Number · Discount → Decimal · Profit → Decimal |
| 4 | **Remove Nulls** | Checked and removed rows with null values in Sales and Profit columns |
| 5 | **Filter Rows** | Kept only `Consumer` and `Corporate` segments; removed `Home Office` |
| 6 | **Split Column** | Split `Order ID` by delimiter `-` to extract the order region code |
| 7 | **Remove Unnecessary Columns** | Removed: Row ID, Country (single-country dataset), Postal Code |
| 8 | **Column Profiling** | Enabled Column Quality, Column Distribution & Column Profile from View tab |
| 9 | **Close & Apply** | Applied all transformations and loaded the clean data into the model |

---

## 📈 Visuals Used

| Visual | Title | Purpose |
|---|---|---|
| 🃏 Card (×4) | Total Sales · Total Profit · Total Quantity · Avg Discount | KPI summary at a glance |
| 🍩 Donut Chart | Profit by Categories | Shows profit share — Technology (50.85%), Office Supplies (42.71%), Furniture (6.45%) |
| 📊 Bar Chart | Sales by Category | Compares sales across Technology (653K), Furniture (620K), Office Supplies (595K) |
| 📊 Bar Chart | Top 10 Customers by Sales | Ranks highest-value customers (Tamara Chand leads at 19.05K) |
| 📉 Line Chart | Monthly Trend | Visualizes monthly sales patterns across the full year |

---

## 🎛️ Slicers

Three interactive slicers are configured in a tile/button layout, allowing users to dynamically filter all visuals simultaneously:

| Slicer | Field | Options |
|---|---|---|
| **Select Category** | Category | Select All · Furniture · Office Supplies · Technology |
| **Select ShipMode** | Ship Mode | First Class · Second Class · Same Day · Standard Class |
| **Select Region** | Region | Central · South · East · West |

Cross-filtering is enabled across all visual pairs so that selecting any slicer value or clicking a chart element updates the entire dashboard in real time.

---

## 🖼️ Screenshots

### Full Dashboard

<img width="1284" height="740" alt="Dashboard" src="https://github.com/user-attachments/assets/0c03169b-df09-4e09-b20e-51ad3d3823cc" />


> *Full interactive dashboard view with all KPI cards, category charts, customer rankings, and monthly trend line.*

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Primary development environment for data modelling and report building |
| **Power Query Editor** | ETL — data cleaning, transformation, and shaping |
| **DAX (Data Analysis Expressions)** | Measures for KPIs (Total Sales, Total Profit, Avg Discount, Total Quantity) |
| **Microsoft Excel / CSV** | Source data format for the Superstore dataset |
| **GitHub** | Version control and project repository hosting |

---

## 📂 Repository Structure

```
📁 SuperStore-PowerBI-PR1/
├── 📄 SuperStore_Sales.pbix       # Power BI project file
├── 📄 Sample_Superstore.csv       # Source dataset
├── 🎥 PR1_RenseeGajipara.mp4      # Explanation video — full project walkthrough (face + screen)
├── 📄 README.md                   # Project documentation
└── 📁 Screenshots/
    └── 🖼️ Dashboard.png           # Full dashboard screenshot
```

---

## 📝 Notes & Insights

- **Technology dominates profitability** — contributing over 50% of total profit despite near-equal sales across all three categories.
- **Furniture lags in profit margins** — with only 6.45% of profit share, despite being the second-highest in sales volume, suggesting high discounting or cost inefficiencies.
- **Sales peak in Q4** — the Monthly Trend chart clearly shows a sharp sales surge in November and December, indicating strong seasonal demand.
- **Top customers are highly concentrated** — the gap between Tamara Chand (19.05K) and the 10th customer (Greg Tran at 11.82K) highlights significant customer value disparity worth strategic attention.
- **Standard Class is the dominant shipping mode** — reflected in the dataset composition, with Same Day delivery being the least utilized.

---

> *"Shaping Skills for Scaling Higher" — Red & White Skill Education*

---

![Made with Power BI](https://img.shields.io/badge/Made%20with-Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Dataset](https://img.shields.io/badge/Dataset-Superstore%20Sales-blue?style=flat-square&logo=databricks&logoColor=white)
![Visuals](https://img.shields.io/badge/Visuals-5%20Chart%20Types-purple?style=flat-square&logo=chartdotjs&logoColor=white)
![Rows](https://img.shields.io/badge/Data%20Rows-9%2C994-orange?style=flat-square&logo=files&logoColor=white)
![License](https://img.shields.io/badge/License-Educational%20Use-lightgrey?style=flat-square)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square&logo=github)

---

## 👨‍💻 Author

<div align="center">

![Author](https://img.shields.io/badge/👨‍💻%20Author-RENSEE%20GAJIPARA-white?style=for-the-badge&labelColor=6C3483&color=A569BD)
![Institute](https://img.shields.io/badge/🏫%20Institute-Red%20%26%20White%20Skill%20Education-white?style=for-the-badge&labelColor=1A5276&color=2E86C1)
![Project](https://img.shields.io/badge/📘%20Project-Power%20BI%20·%20PR%201-white?style=for-the-badge&labelColor=117A65&color=1ABC9C)

</div>
