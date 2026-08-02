# Business Intelligence Dashboard — Superstore Sales Analysis

Interactive BI dashboard built in **Microsoft Excel** to analyze sales performance across regions, product categories, and time. Built using formula-driven KPIs (SUMIFS/COUNTIFS) and live charts — no hardcoded values, so every number recalculates automatically if the underlying data changes.

## Problem
Analyze 4 years of retail order data to answer: which regions, categories, and customer segments drive the most revenue, and how does revenue trend over time?

## Data Source
[Superstore Sales Dataset](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting) — Kaggle, 9,800 order line items across 4,922 unique orders, spanning FY2015–FY2018.

## Approach
- Imported and cleaned raw order-level data (converted date fields, added helper columns for month grouping and unique-order detection)
- Built KPI cards for Total Revenue, Unique Orders, Line Items, and Average Order Value using `SUMIFS` / `COUNTIFS` formulas
- Broke down revenue by Region, Category, Segment, and Sub-Category using summary tables
- Built a 48-month revenue trend table to surface seasonality
- Visualized everything with 4 native Excel charts (bar, pie, horizontal bar, line)

## Key Insights
- Total revenue across the dataset: **$2,261,536**
- **West** region leads revenue (**$710,220**), followed by East; **South** is lowest
- **Technology** is the top-performing category (**$827,456**), ahead of Furniture and Office Supplies
- **Phones** and **Chairs** are the top two sub-categories by revenue
- **Consumer** segment drives over half of total revenue ($1.15M of $2.26M)

## Tools Used
Microsoft Excel (formulas, PivotTable-style aggregation, native charts), data sourced and cleaned from a public Kaggle dataset.

## Zoho Analytics Dashboard (Companion Build)

To complement the Excel workbook and demonstrate cloud BI tooling, the same dataset and KPIs were rebuilt as an interactive dashboard in Zoho Analytics.

![Zoho Analytics Dashboard](Zoho_Dashboard_Screenshot.png)

**Live interactive dashboard:** https://analytics.zoho.in/open-view/554171000000007006

Same 4 KPIs (Total Revenue, Unique Orders, Line Items, Avg Order Value) and same 4 charts (Revenue by Region, Revenue by Category, Revenue by Sub-Category, Monthly Revenue Trend), cross-validated to match the Excel workbook's figures exactly.

## Files
- `Superstore_BI_Dashboard.xlsx` — the dashboard (Dashboard tab + Raw Data tab)
- `data/train.csv` — source dataset

## Notes
This project uses a widely-used public training dataset for demonstrating BI/dashboard skills (dates reflect the original dataset's 2015–2018 range). Project built: August 2026.
