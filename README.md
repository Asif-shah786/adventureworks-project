# AdventureWorks Sales & Customer Analytics Dashboard

An end-to-end Power BI business intelligence project built to analyse sales performance, profitability, product trends, returns, regional performance, and customer behaviour for AdventureWorks.

> **Note:** This is a portfolio case study created using the Microsoft AdventureWorks sample dataset. The company and business scenario are fictional.

## Dashboard Preview

Below is the main executive dashboard from the AdventureWorks Power BI report.

<p align="center">
  <img src="https://github.com/user-attachments/assets/faa0ad7b-7700-4461-8da1-25f735bec754"
       alt="AdventureWorks Executive Dashboard"
       width="1000">
</p>

## Live report

[Open the interactive Power BI report](https://app.powerbi.com/reportEmbed?reportId=095ad57b-fad9-4de4-8344-08d5c6cb239e&autoAuth=true&ctid=65b52940-f4b6-41bd-833d-3033ecbcf6e1)

> The current link may require Microsoft sign-in. Before adding it to your CV, test it in a private/incognito browser where you are not signed in. For unrestricted recruiter access, replace it with a **Publish to web (public)** URL.

## Business objective

The dashboard was developed to help decision-makers:

- Track sales, revenue, profit, orders, customers, and return rate
- Compare performance across regions and time periods
- Identify high-performing and underperforming products
- Analyse product return patterns in the context of sales volume
- Explore customer value, demographics, and purchasing behaviour

## What I built

- Connected and transformed raw CSV files using **Power Query**
- Cleaned data types, handled inconsistent values, and prepared lookup tables
- Combined yearly transaction files into a consolidated sales table
- Built a relational model using fact and dimension tables
- Configured one-to-many relationships and appropriate filter flow
- Created calculated columns and reusable measures using **DAX**
- Designed interactive report pages with KPI cards, charts, slicers, drill-downs, bookmarks, and tooltips
- Published the finished report to Power BI Service

## Report pages

Update these descriptions so they exactly match your report.

### 1. Executive Dashboard
High-level view of revenue, profit, orders, customers, returns, and performance over time.

### 2. Product Analysis
Product and category performance, sales trends, profitability, and return behaviour.

### 3. Customer Analysis
Customer segmentation, purchasing patterns, high-value customers, and revenue per customer.

### 4. Regional Analysis
Sales and profitability by country, territory, and region.

## Table View

Typical tables include:

- **Sales Data** — order-level sales transactions
- **Returns Data** — returned product quantities
- **Product Lookup** — product attributes
- **Product Category Lookup**
- **Product Subcategory Lookup**
- **Customer Lookup**
- **Territory Lookup**
- **Calendar Lookup**

## Data Model

Built using a **star schema** with fact and dimension tables, one-to-many relationships, and reusable DAX measures.

<p align="center">
  <img src="https://github.com/user-attachments/assets/fb0ae0a1-98d1-4bc2-837d-ef2001baf6a9"
       alt="AdventureWorks Data Model"
       width="1100">
</p>

## Repository structure

```text
adventureworks-project/
├── README.md
├── assets/
│   ├── executive-dashboard.png
│   ├── product-analysis.png
│   ├── customer-analysis.png
│   └── data-model.png
├── docs/
│   ├── DAX_MEASURES.md
│   ├── PROJECT_NOTES.md
│   └── DATA_DICTIONARY.md
├── report/
│   └── AdventureWorks-Report.pbix
└── data/
    └── README.md
```

## Data source and attribution

This project uses the Microsoft AdventureWorks sample data for learning and portfolio demonstration. The dashboard design, transformations, calculations, analysis, and presentation in this repository represent my own implementation.

The project was developed while following structured Power BI training material. The repository is intended to showcase my completed work and analytical understanding, not reproduce or redistribute the training content.
