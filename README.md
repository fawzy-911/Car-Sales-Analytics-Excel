# Car Sales Analytics Dashboard | Microsoft Excel

**From raw car sales records to an interactive sales dashboard.**

This project explores a car sales dataset with Microsoft Excel and turns it into a visual report for investigating sales value, vehicle demand, company performance, dealer performance, and customer and vehicle characteristics.

![Car Sales Analytics Dashboard](images/dashboard-preview.png)

## At a Glance

| Project detail | Description |
|---|---|
| **Project type** | Sales data analysis and dashboarding |
| **Tool** | Microsoft Excel |
| **Dataset size** | 23,906 records · 17 columns |
| **Period covered** | January 2022 – December 2023 |
| **Main techniques** | PivotTables, charts, KPI summaries, interactive filters |
| **Workbook sheets** | `Car Sales Data`, `Pivot tables`, `Dashboard`, `Summary` |

## Business Objective

The objective is to make a large set of sales records easier to explore and interpret. Instead of reading rows one by one, users can compare companies and dealers, inspect popular vehicle types, and filter the dashboard to investigate a selected period or group.

## Business Questions

The dashboard is designed to help explore questions such as:

- Which car companies contribute the most sales value?
- Which companies sell the highest number of cars?
- How does sales performance vary between dealers?
- Which models appear most frequently in the sales data?
- Which body styles, transmission types, engine types, and colors are most common?
- How do the results change when the date or other dashboard filters are adjusted?

## Key Metrics

The dashboard highlights four headline KPIs:

- **Total Sales** — the total value of car sales.
- **Total Cars Sold** — the number of car records included in the analysis.
- **Average Car Price** — the average recorded vehicle price.
- **Average Customer Income** — the average annual income recorded for customers.

These KPIs are complemented by charts for company sales, cars sold by company, dealer performance, top models, body style, transmission type, engine type, and car color.

## What the Dashboard Contains

| Dashboard visual | What it helps investigate |
|---|---|
| **Sales by Company** | Compares sales value across car companies |
| **Cars Sold by Company** | Compares the number of cars recorded for each company |
| **Dealer Performance** | Compares sales value across dealers |
| **Top Models Sold** | Highlights models with higher recorded sales counts |
| **Body Style Distribution** | Compares SUV, Hatchback, Sedan, Passenger, and Hardtop categories |
| **Transmission Type Distribution** | Compares automatic and manual transmission records |
| **Engine Type Distribution** | Shows the distribution of engine types |
| **Car Color Popularity** | Compares the colors shown in the dashboard |
| **Date timeline and slicers** | Let users filter the dashboard and explore different subsets of the data |

## Data & Workbook Structure

The `Car Sales Data` worksheet contains **23,906 records and 17 columns**, including:

- **Sales and time:** `Date`, `Price ($)`, `Car_id`
- **Customer attributes:** `Customer Name`, `Gender`, `Annual Income`
- **Vehicle attributes:** `Company`, `Model`, `Engine`, `Transmission`, `Color`, `Body Style`
- **Dealer attributes:** `Dealer_Name`, `Dealer_No`, `Dealer_Region`
- **Additional field:** `Car-Income_Per`

The workbook is organized into four worksheets:

1. **Car Sales Data** — the source records.
2. **Pivot tables** — supporting PivotTables and charts used for aggregation.
3. **Dashboard** — the main visual report.
4. **Summary** — KPI labels and formulas linked to PivotTable results.

## Initial Data Observations

A basic check of the source worksheet shows:

- The dataset contains **23,906 records** spanning **2022–2023**.
- There are **30 distinct car-company names** in the source data.
- **SUV** is the most frequent body-style category in the source records (**6,374 records**), followed by **Hatchback** (**6,128 records**).
- The source data contains **12,571 Auto** and **11,335 Manual** transmission records.

These are descriptive counts from the raw worksheet, not causal explanations or recommendations. They should be interpreted in the context of the dataset and validated alongside the final dashboard calculations.

## Excel Skills Demonstrated

- Structuring and reviewing a tabular dataset
- Summarizing records with **PivotTables**
- Presenting comparisons with charts
- Building a dashboard from supporting summaries
- Displaying KPI values through linked summary formulas such as `GETPIVOTDATA`
- Adding a date timeline and slicers for interactive filtering

## How to Explore the Project

1. Download `Car_Sales_Analytics.xlsx` from this repository.
2. Open the workbook in Microsoft Excel.
3. Select the **Dashboard** worksheet.
4. Use the date timeline and slicers to filter the report.
5. Compare the KPI cards and charts, then investigate the patterns behind the selected results.
6. If you modify the source data, verify the PivotTable source ranges and select **Data → Refresh All**.

## Validation Note

The current dashboard screenshot shows **5,920** for `Total Cars Sold` and **166,337,116** for `Total Sales`. However, the source worksheet contains **23,906 records**, and the sum of the `Price ($)` column in that source data is **671,525,465**.

The displayed KPI values therefore do not currently reconcile with the full source worksheet. Before presenting those dashboard KPIs as final results, check the PivotTable source ranges, refresh the PivotTables, and verify the formulas and filters. The source-data observations above are calculated separately from the raw worksheet.

## Repository Contents

```text
Car-Sales-Analytics-Excel/
├── README.md
├── Car_Sales_Analytics.xlsx
└── images/
    └── dashboard-preview.png
```

## Project Summary

This project demonstrates how Microsoft Excel can be used to summarize sales data and present it in a filterable dashboard. The next step toward a publication-ready analysis is to reconcile the KPI calculations with the complete source dataset, then document any validated business insights and recommendations.

---

**Tools:** Microsoft Excel · PivotTables · Charts · `GETPIVOTDATA` · Slicers · Timeline
