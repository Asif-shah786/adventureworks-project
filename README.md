# AdventureWorks Sales & Customer Analytics Dashboard

An end-to-end Power BI business intelligence project built to analyse sales performance, profitability, product trends, returns, regional performance, and customer behaviour for AdventureWorks.

> **Note:** This is a portfolio case study created using the Microsoft AdventureWorks sample dataset. The company and business scenario are fictional.

## Dashboard preview

Add your strongest dashboard screenshot here:

```markdown
![Executive Dashboard](assets/executive-dashboard.png)
```

### Live report

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

## Data model

The model uses a relational structure with transaction-level fact tables and descriptive lookup tables.

Typical tables include:

- **Sales Data** — order-level sales transactions
- **Returns Data** — returned product quantities
- **Product Lookup** — product attributes
- **Product Category Lookup**
- **Product Subcategory Lookup**
- **Customer Lookup**
- **Territory Lookup**
- **Calendar Lookup**

Add a screenshot of your actual model:

```markdown
![Data Model](assets/data-model.png)
```

## Example DAX measures

Add only the measures that exist in your report. A separate template is available in [`docs/DAX_MEASURES.md`](docs/DAX_MEASURES.md).

Examples of portfolio-relevant measures:

```DAX
Total Revenue =
SUMX(
    'Sales Data',
    'Sales Data'[Order Quantity] * RELATED('Product Lookup'[Product Price])
)

Total Profit =
[Total Revenue] - [Total Cost]

Return Rate =
DIVIDE([Quantity Returned], [Quantity Sold], 0)

Revenue per Customer =
DIVIDE([Total Revenue], [Total Customers], 0)
```

## Key insights

Replace these prompts with findings from your own dashboard:

- Which product category generated the most revenue and profit?
- Which regions performed above or below average?
- Did increasing return volume reflect a worsening return rate, or simply higher sales?
- Which customers or segments contributed the most value?
- Which months showed the strongest or weakest performance?

A good insight should include a finding, context, and business implication.

**Example format:**

> Bike returns increased in absolute volume, but the return rate remained relatively stable because bike sales increased at a similar pace. This suggests growth in returns was driven primarily by higher sales volume rather than deteriorating product quality.

## Tools and skills demonstrated

- Power BI Desktop
- Power BI Service
- Power Query
- DAX
- Data cleaning and transformation
- Relational data modelling
- Star/snowflake schema concepts
- KPI design
- Data visualisation
- Business analysis
- Insight communication

## Repository structure

```text
adventureworks-power-bi-dashboard/
├── README.md
├── index.html
├── .gitignore
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

## How to explore the project

1. Review the dashboard screenshots in `assets/`
2. Open the live Power BI report using the link above
3. Review the project methodology and measures in `docs/`
4. Download the `.pbix` file from `report/` if included

## Data source and attribution

This project uses the Microsoft AdventureWorks sample data for learning and portfolio demonstration. The dashboard design, transformations, calculations, analysis, and presentation in this repository represent my own implementation.

The project was developed while following structured Power BI training material. The repository is intended to showcase my completed work and analytical understanding, not reproduce or redistribute the training content.
