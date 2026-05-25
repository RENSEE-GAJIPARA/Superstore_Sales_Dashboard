# 📊 Superstore Business Insights Dashboard

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

![Superstore Business Insights Dashboard](D:\Power%20BI\pr1\Screenshots\Dashboard.png)

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

## ✅ Submission Checklist

- [x] `.pbix` file — all 13 tasks completed
- [x] Power Query: 9 transformation steps applied
- [x] 4 KPI Cards + Bar Charts + Donut Chart + Line Chart (all formatted)
- [x] 3 Slicers — Region, Category, Ship Mode (Tile style)
- [x] Filter panel configured (Page-level & Visual-level)
- [x] Cross-filtering enabled across 3+ visual pairs
- [x] Professional dark theme applied consistently
- [x] Dashboard layout aligned with consistent spacing
- [x] GitHub repository: public with all project files
- [x] README.md: complete with screenshots and documentation
- [x] 3+ meaningful commits with descriptive messages

---

## 👨‍💻 Author

**RENSEE GAJIPARA**  
🏫 Red & White Skill Education  
📘 Power BI — Practical Report 1 (PR 1)  

---

## 📝 Notes & Insights

- **Technology dominates profitability** — contributing over 50% of total profit despite near-equal sales across all three categories.
- **Furniture lags in profit margins** — with only 6.45% of profit share, despite being the second-highest in sales volume, suggesting high discounting or cost inefficiencies.
- **Sales peak in Q4** — the Monthly Trend chart clearly shows a sharp sales surge in November and December, indicating strong seasonal demand.
- **Top customers are highly concentrated** — the gap between Tamara Chand (19.05K) and the 10th customer (Greg Tran at 11.82K) highlights significant customer value disparity worth strategic attention.
- **Standard Class is the dominant shipping mode** — reflected in the dataset composition, with Same Day delivery being the least utilized.

---

> *"Shaping Skills for Scaling Higher" — Red & White Skill Education*
