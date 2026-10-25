# Blinkit Sales Analysis Dashboard | Power BI

An interactive Power BI dashboard for exploring Blinkit sales performance across outlet types, outlet sizes, locations, item categories, and fat content.

![Blinkit Sales Analysis Dashboard](dashboard-preview.png)

## Project Overview

This project presents a sales-performance dashboard built in Microsoft Power BI. It brings key business metrics and several breakdowns into one view to help users compare sales across outlet tiers, outlet sizes, outlet types, and item categories.

> **Note:** The figures below are transcribed from the dashboard screenshot. They describe the displayed report and have not been independently validated against the underlying dataset.

## Key Performance Indicators

| KPI | Value shown | What it represents |
|---|---:|---|
| Total Sales | **$1.20M** | Total sales value displayed in the report |
| Average Sales | **$141** | Average sales value per item/transaction displayed in the report (confirm the exact definition in Power BI) |
| No. of Items | **9K** | Number of items displayed in the report (rounded; the outlet-type table adds up to about 8.5K) |
| Average Rating | **4.0** | Average customer rating displayed in the report |

## Dashboard Sections

### 1. Outlet Establishment
An area/line chart showing total sales by outlet establishment year, from $205K (2018) down to $78K (2011). The years on the x-axis are ordered by sales value rather than chronologically (2018, 2017, 2016, 2014, 2022, 2015, 2012, 2020, 2011), so the line should not be read as a time trend.

### 2. Fat Content
A doughnut chart splitting the $1.20M total sales between:
- Low Fat: **$776.32K**
- Regular: **$425.36K**

### 3. Fat by Outlet
A clustered bar chart comparing Low Fat and Regular item sales across outlet location tiers:

| Tier | Low Fat | Regular |
|---|---:|---:|
| Tier 3 | $0.31M | $0.17M |
| Tier 2 | $0.25M | $0.14M |
| Tier 1 | $0.22M | $0.12M |

### 4. Item Type
A horizontal bar chart ranking item categories by total sales. Top categories shown: Fruits and Vegetables and Snack Foods (about $0.18M each), followed by Household ($0.14M), Frozen Foods ($0.12M), and Dairy. The list continues down to Breakfast (about $0.02M). Some category labels are truncated in the screenshot.

### 5. Outlet Size
A doughnut chart comparing sales by outlet size:
- Medium: **$507.90K**
- Small: **$444.79K**
- High: **$248.99K**

### 6. Outlet Location
A funnel chart showing sales by location tier:
- Tier 3: **$472.13K** (100%)
- Tier 2: **$393.15K**
- Tier 1: **$336.40K** (71.3% of Tier 3)

### 7. Outlet Type Summary Table
A table with conditional formatting comparing outlet types:

| Outlet Type | Total Sales | No. of Items | Avg Sales | Avg Rating | Item Visibility |
|---|---:|---:|---:|---:|---:|
| Grocery Store | $151.94K | 1083 | $140 | 4.0 | 0.10 |
| Supermarket Type1 | $787.55K | 5577 | $141 | 4.0 | 0.06 |
| Supermarket Type2 | $131.48K | 928 | $142 | 4.0 | 0.06 |
| Supermarket Type3 | $130.71K | 935 | $140 | 4.0 | 0.06 |

## Filters and Interactivity

The screenshot shows:
- An **Outlet Location Type** dropdown filter (currently set to "All")
- Metric toggle buttons above the Fat Content and Item Type charts: **Total Sales**, **Avg Sales**, **No of Items**, and **Avg Rating**

These controls allow users to narrow the report to a location type and switch the metric shown in the charts, assuming the original Power BI report has the interactions configured.

## Tools

- **Microsoft Power BI**: dashboard design and data visualization
- **GitHub**: project documentation and version control

Add other tools here if you used them (for example, Excel, SQL, Power Query, DAX, or Python).

## Repository Contents

```text
blinkit-sales-analysis/
├── README.md
├── dashboard-preview.png
└── Blinkit-Sales-Analysis.pbix   # optional: add your Power BI file
```

The `.pbix` file is optional, but include it if you want visitors to inspect or interact with the report in Power BI Desktop. Only add files you have permission to share.

## How to View the Project

1. Open `dashboard-preview.png` in this repository to see the dashboard screenshot.
2. If the `.pbix` file is included, download it.
3. Open the `.pbix` file using **Microsoft Power BI Desktop**.
4. If Power BI asks for a data source or credentials, reconnect the data source using your own authorized access.

A screenshot is a static preview; it does not preserve Power BI filters, tooltips, or interactivity.

## Insights to Explore

Based on the visuals shown, a viewer can investigate:
- Which outlet type drives most of the sales (Supermarket Type1 shows about $787.55K of the $1.20M total).
- How Low Fat items compare with Regular items (Low Fat is roughly 65% of total sales in the chart).
- Which location tier and outlet size contribute the most sales (Tier 3 and Medium outlets lead in the screenshot).
- Which item categories lead in sales.
- Whether average sales and ratings differ at all between outlet types (they look almost identical: $140 to $142 and 4.0).
- Whether the location filter changes the rankings.

Avoid treating these as final business conclusions until you verify the source data, definitions, and report calculations.

## Data and Metric Notes

- Confirm whether the sales figures are in USD or INR and document the currency in the report.
- The "No of Items" card shows 9K, while the outlet-type table adds up to 8,523. Confirm whether the card is just rounded or uses a different calculation.
- The Outlet Establishment chart is sorted by sales value, not by year. If you want a true timeline, sort the axis by year.
- Document the source dataset, refresh date, and any data-cleaning steps if known.

## Suggested GitHub Repository Details

- **Repository name:** `blinkit-sales-analysis`
- **Short description:** `Power BI dashboard analyzing Blinkit sales, average sales, ratings, outlet types, locations, and item categories.`
- **Topics:** `power-bi`, `data-analytics`, `sales-analysis`, `data-visualization`, `business-intelligence`, `dashboard`, `blinkit`
- **Visibility:** Public if you want to showcase it in a portfolio and are allowed to share all included files; otherwise choose Private.

## Future Improvements

- Add the original `.pbix` file if it can be shared.
- Document the dataset source and a data dictionary.
- Add definitions for each KPI and explain any DAX measures.
- Sort the Outlet Establishment chart by year for a clear timeline.
- Widen the Item Type labels so category names are not truncated.
- Add a short section with verified findings after checking the underlying data.

## Author

**Your Name**  
Add your GitHub profile or portfolio link here.

---

*This README describes the dashboard based on the supplied screenshot. Update the tools, data-source details, calculations, and author information to match your actual project before publishing.*
