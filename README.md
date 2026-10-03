# Confectionery Sales & Operations Analytics Dashboard

An interactive Power BI analytics dashboard designed to monitor FMCG sales performance, supply chain status, regional distribution, and profitability metrics across multiple zones.

## Author
* **Chiranjivi Kamble**[cite: 1]

---

## Dashboard Overview

This solution provides comprehensive visibility into wholesale and retail confectionery operations, helping stakeholders track revenue trends, order fulfillment bottlenecks, and regional demand patterns.

### Key Performance Indicators (KPIs)
* **Total Net Revenue:** ₹6.37M[cite: 1]
* **Total Gross Sales:** ₹3.30M[cite: 2]
* **Total Gross Profit:** ₹1.18M[cite: 2]
* **Profit Margin:** 37.32%[cite: 2]
* **Total Orders:** 2,050[cite: 1]
* **Total Units Sold:** 39,627[cite: 1]
* **YoY Sales Growth:** -0.75%[cite: 1]
* **Wholesale Contribution:** 34.60%[cite: 2]

---

## Data Transformation & Power Query

Before building the data model and visuals, raw data underwent rigorous cleaning and transformation using **Power Query (M Language)**:
* **Data Cleansing:** Handled missing values, standardized text formatting, and removed duplicate or erroneous records.
* **Type Conversion & Schema Shaping:** Ensured appropriate data types (Dates, Numeric, Text) and structured relational tables following a clean Star Schema design.
* **Custom Columns & Conditional Logic:** Created conditional columns for order categorization, delivery status mapping, and financial metric calculations to streamline DAX measure writing.

---

## Visualizations & Features

1. **Sales & Revenue Analysis:**
   * Category-wise breakdown (Candy, Toffee, Lollipops, Eclairs, Gums & Mints).
   * Year-over-Year trend comparisons across months.
   * Net revenue distribution by store types (Wholesaler, Kirana Retail, Supermarket, Sweet & Candy Shop, etc.).

2. **Geographical Distribution:**
   * Zone-wise and District-wise performance matrices (Western Zone, Vidarbha Zone, North/South Maharashtra, etc.).
   * Interactive India map visualization tracking active billed stores and regional delivery success rates.

3. **Operations & Fulfillment Pipeline:**
   * Order status tracking (Delivered/Successful, Cancelled, Pending).
   * Delay reasons pipeline (Delivery Route Postponed, Retailer Delayed Payment, Stock-Outs, Overdue Credit).
   * Delivery success rate versus cancellation metrics.

---

## Dashboard Screenshots

### Page 1: Sales & Regional Performance
![Sales Overview](Screenshot%202026-10-02-182724.png)[cite: 3]

### Page 2: Operations & Delay Analysis
![Operations Overview](Screenshot%202026-10-02-182648.png)[cite: 2]

---

## Tech Stack & Tools
* **Power Query (M):** ETL, data cleaning, and transformation.
* **Power BI Desktop:** Data modeling, DAX measures, and interactive UI design.
* **Excel / Data Model:** Source data management and relational schema structure (`Fact_Sales_Orders`, `Dim_Product`, `Dim_Geography`, `Dim_Customers`, `Dim_Sales_Team`).

```
