# Sales Analytics Dashboard — Power BI

## Project Overview

An interactive Power BI Sales Analytics Dashboard built to analyze sales performance across customers, products, geography, and time.

The project focuses on transforming raw sales data into a structured data model and presenting the results through an interactive multi-page Power BI report.

---

## Dashboard Pages

### 1. Executive Dashboard
Provides a high-level overview of sales performance with KPI cards, sales visuals, year filtering, reset filters, and navigation.

### 2. Sales Performance
Analyzes sales performance using multiple charts, a matrix, and interactive Bar/Line view bookmarks.

### 3. Customer Analysis
Provides customer-focused sales analysis using charts and KPI cards.

### 4. Product Detail
Provides product-level analysis with KPI cards, a line chart, and drillthrough functionality.

### 5. Profitability & Discounts
Provides additional sales analysis through KPI cards, clustered bar charts, and a matrix.

---

## Data Model

The report uses a star-schema structure with:

- Fact_Orders
- Dim_Date
- Dim_Customer
- Dim_Product
- Dim_Geography

Relationships were created between the fact table and the relevant dimension tables.

---

## DAX Measures

The dashboard currently includes the following measures:

- Total Sales
- Total Orders
- Average Order Value
- Sales LY
- Sales YTD
- Sales MTD
- Sales YoY%
- Sales MoM%
- Sales Running Total
- Sales Rank by Product
- % of Total Sales

---

## Interactivity

The dashboard includes:

- Year slicer
- Reset Filters button
- Page navigation
- Drillthrough
- Back button
- Bookmark-based Bar/Line view
- Cross-filtering
- Conditional formatting

---

## Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Data Modeling
- Star Schema
- Data Visualization

---

## Project Structure

```text
PowerBI-Sales-Analytics-Dashboard/
│
├── README.md
├── Sales_Dashboard.pbix
│
└── screenshots/
    ├── executive-dashboard.png
    ├── sales-performance.png
    ├── customer-analysis.png
    ├── product-details.png
    └── sales-overview.png

## Dashboard Preview

### Executive Dashboard

![Executive Dashboard](screenshots/executive-dashboard.png)

### Sales Performance

![Sales Performance](screenshots/sales-performance.png)

### Customer Analysis

![Customer Analysis](screenshots/customer-analysis.png)

### Product Detail

![Product Detail](screenshots/product-detail.png)

### Sales Overview

![Sales Overview](screenshots/sales-overview.png)
```

---

## Project Status

The current version contains the completed dashboard pages, data model, core DAX measures, interactive features, and dashboard formatting completed so far.
