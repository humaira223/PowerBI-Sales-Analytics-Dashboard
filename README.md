Interactive Power BI sales analytics dashboard with star-schema data modeling, DAX measures, time intelligence, drillthrough and interactive reporting.
# Sales Performance & Executive Dashboard — Power BI

## Project Overview

This project is an interactive Power BI sales analytics dashboard created as part of a data analytics / business intelligence project.

The objective is to transform raw sales data into a structured analytical model and an interactive multi-page dashboard that helps users explore sales performance across time, customers, products, geography, and other available business dimensions.

> **Project status:** Dashboard and core data-model/DAX work completed up to the current stage. Advanced analysis and final documentation requirements will be completed in the next phase.

---

## Business Objective

The dashboard is designed to help stakeholders:

- Monitor overall sales performance.
- Analyze sales trends over time.
- Compare customer and product performance.
- Explore geographic sales performance.
- Identify high-performing products and customers.
- Analyze sales using interactive filters and drillthrough.
- Compare current sales with previous periods using time-intelligence measures.

---

## Dataset

The project uses a sales dataset containing order, customer, product, date, geography, and sales information.

The available dataset was used as provided. No unsupported values were fabricated.

Some assignment requirements refer to fields such as **Profit, Discount, and Quantity**. These fields are not available in the actual source dataset used for this project, so those analyses have not been fabricated and will be treated as dataset limitations in the final documentation.

---

## Data Model

A star-schema approach was implemented.

### Fact Table

**Fact_Orders**

Contains transactional/order-level information used for sales analysis.

### Dimension Tables

- **Dim_Date**
- **Dim_Customer**
- **Dim_Product**
- **Dim_Geography**

The model uses dimension-to-fact relationships, with the fact table containing the corresponding foreign keys.

Foreign-key fields that are primarily required for relationships were hidden from the report field list where appropriate.

---

## Dashboard Pages

The current report contains five dashboard pages.

### 1. Executive Dashboard

Provides a high-level overview of the business and acts as the main entry point to the report.

Includes:

- KPI cards
- Year slicer
- Reset Filters button
- Page navigation
- Sales visualizations
- Interactive filtering

The Year slicer is connected to the relevant report pages so that selecting a year updates the related visuals.

---

### 2. Sales Performance

Focuses on sales performance and trends.

Includes:

- Clustered column charts
- Clustered bar charts
- Matrix
- Stacked column chart
- Line chart
- Bar/Line view bookmark functionality

The page supports comparison of sales performance across relevant business dimensions and time.

---

### 3. Customer Analysis

Focuses on customer-related sales analysis.

Includes:

- Customer-focused charts
- KPI cards
- Interactive filtering

---

### 4. Product Detail

Provides detailed product-level analysis.

Includes:

- KPI cards
- Line chart
- Product detail analysis
- Drillthrough functionality
- Back button

The Product Detail page can be reached through drillthrough from relevant product analysis visuals.

The Back button returns the user to the page from which the drillthrough was initiated.

---

### 5. Profitability & Discounts

Contains the final analytical dashboard page with:

- Three KPI cards
- Clustered bar charts
- Matrix

The page name is retained from the assignment structure. However, profitability/discount-specific calculations that require unavailable source columns have not been fabricated.

---

## DAX Measures Implemented So Far

The following core measures have been implemented and tested:

### Total Sales

Calculates total sales.

### Total Orders

Calculates total order count.

### Average Order Value

Calculates the average sales value per order.

### Sales LY

Calculates sales for the previous-year period.

### Sales YTD

Calculates year-to-date sales.

### Sales MTD

Calculates month-to-date sales.

### Sales YoY%

Calculates year-over-year sales growth.

### Sales MoM%

Calculates month-over-month sales growth.

### Sales Running Total

Calculates cumulative sales over the selected date context.

### Sales Rank by Product

Ranks products according to their sales performance.

### % of Total Sales

Calculates a product's contribution to the selected total sales context.

All implemented measures were tested within the Power BI report, including filter responsiveness for the time-intelligence measures.

---

## Interactivity

The report currently includes:

- Year slicer
- Slicer filtering across relevant report pages
- Reset Filters functionality
- Page navigation
- Drillthrough
- Dynamic Back button
- Bookmark-based Bar/Line view
- Cross-filtering between visuals
- Conditional formatting
- Interactive KPI cards and charts

---

## Data Quality & Modeling Work

During development, the following data/modeling tasks were performed:

- Raw data was cleaned and structured.
- Dimension tables were created.
- Duplicate dimension records were addressed.
- Relationships were established between fact and dimension tables.
- Date modeling was implemented.
- Foreign-key fields were hidden where appropriate.
- Visuals were connected to the analytical model.
- Time-intelligence measures were tested against year filters.

---

## Design & Formatting

The dashboard was formatted consistently across the five pages.

Work included:

- Theme colors
- Canvas sizing
- KPI card formatting
- Chart formatting
- Matrix formatting
- Conditional formatting
- Headers
- Navigation elements
- Button formatting
- Alignment and spacing
- Readability improvements

---

## Current Project Status

### Completed

- Data preparation
- Star-schema data model
- Relationships
- Core DAX measures
- Time-intelligence measures
- Five dashboard pages
- Dashboard formatting
- Interactive slicers
- Reset Filters
- Navigation
- Drillthrough
- Back navigation
- Bookmark interaction
- Conditional formatting
- Initial validation/testing

### Planned Next Phase

The remaining assignment work will be completed after this project snapshot, including applicable advanced analysis, custom tooltip functionality, final validation, business insights, documentation, and portfolio/publishing tasks.

Requirements that depend on unavailable dataset fields will be explicitly documented as **not applicable due to source-data limitations** rather than being fabricated.

---

## Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Data Modeling
- Star Schema
- Interactive Data Visualization

---

## Project Files

The repository is intended to contain:

```text
Sales-PowerBI-Dashboard/
│
├── README.md
├── Sales_Dashboard.pbix
└── screenshots/
```

Additional documentation and screenshots can be added as the project is finalized.

---

## Author

**Data Analytics / Data Science Portfolio Project**

This project demonstrates practical experience with:

- Power BI
- Data modeling
- DAX
- Business intelligence
- Interactive dashboards
- Sales analytics
- Data visualization
