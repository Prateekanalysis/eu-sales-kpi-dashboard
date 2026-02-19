# EU Sales Performance & Executive KPI Dashboard (Python + Excel + Power BI-style)

An end-to-end business KPI project for executive reporting: data generation → cleaning → KPI engineering → Excel management pack → dashboard-ready tables for Power BI.

## Business questions

- What are the revenue and profit trends over time?
- Which countries/categories drive growth?
- Where are margins weak or negative?
- Which products/customers contribute most to profit?


## KPIs

- Revenue (Sales)
- Profit
- Profit margin %
- Orders
- Customers
- Average order value (AOV)
- MoM & YoY growth (Sales/Profit)


## Folder structure

```text
01-eu-sales-kpi-dashboard/
├── data/
│   ├── raw/
│   └── clean/
├── excel-dashboard/
├── powerbi-dashboard/
├── reports/
├── src/
└── README.md
```

## How to run

1) Generate realistic sales data:
```bash
python src/00_generate_sales_data.py
```
2) Clean + engineer KPIs:
```bash
python src/01_clean_build_kpis.py
```
3) Create the Excel management pack:
```bash
python src/02_build_excel_pack.py
```
4) Open the Excel file in `excel-dashboard/` and take screenshots.
5) Optional: Load `data/clean/fact_sales_kpis.csv` into Power BI and build a one-page dashboard.


## Power BI page layout (recommended)

**KPI cards:** Revenue, Profit, Margin %, Orders, Customers

**Charts:**
- Line: Sales by Month (with YoY)
- Bar: Profit by Category/Subcategory
- Map: Sales/Profit by Country
- Table: Top 10 products by Profit and Margin

**Slicers:** Year, Country, Category, Segment

## Resume bullets (copy/paste)

- Built an executive KPI dashboard (Excel + Power BI-style) tracking revenue, profit, margin and growth across EU regions.
- Cleaned and engineered KPIs in Python (Pandas), delivering stakeholder-ready insights on profitability drivers and underperforming segments.

