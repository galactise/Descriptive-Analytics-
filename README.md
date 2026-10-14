# Descriptive-Analytics-
Descriptive Analytics
# Lenskart Daily Transaction Analytics: Descriptive Report

A descriptive analytics report on **30 days of e-commerce eyewear and vision-care transactions**, built on a **synthetic dataset** that mirrors real Lenskart-style order patterns. It answers *what happened, who transacted, and how much value moved*, and closes with a roadmap toward predictive analytics.

**Author:** Adarsh Patel
**Programme:** BCA (Data Science & AI), School of Computer Applications, Babu Banaras Das University

📄 **Report:** [Lenskart_Transaction_Descriptive_Analytics_Report.pdf](Lenskart_Transaction_Descriptive_Analytics_Report.pdf)

---

## Dataset at a glance

| Item | Detail |
|------|--------|
| Period | 30 days (2026-07-31 to 2026-08-29) |
| Structure | 60 stores × 10 categories × 8 regions |
| Orders | ~1.38 million (simulated) |
| Gross transaction value | ~INR 252 crore |
| Data quality | Zero missing cells, schema and arithmetic validated |

> The data is **synthetic and illustrative**. A real platform's order feed is not publicly available.

## Headline KPIs

| Metric | Value |
|--------|-------|
| Total orders | 1.38M |
| Gross transaction value | INR 252 Cr |
| Average order value (AOV) | INR 1,821 |
| Average order success rate | 97.4% |
| Stores in the inventory reorder zone | 9 of 60 |
| Top category by value (Eyeglasses, Prescription) | 25.9% share |

## Report contents

| Section | Topic | What it shows |
|---------|-------|---------------|
| 1 | Top categories | Value vs. volume leaders across 10 categories |
| 2 | Weekly trends | Value and order build-up across weeks, partial-week caveat |
| 3 | AOV distribution | Binned spread, quartiles and IQR of store-day AOV |
| 4 | Channel tiers | App, Offline Store, Website and Marketplace comparison |
| 5 | Customer segments | Regular, Gold, Premium/Designer and Corporate/Bulk contribution |
| 6 | Regional demand | 8 regions and 4 macro-clusters |
| 7 | Revenue concentration | Region × Category top combinations, Pareto effect |
| 8 | Payment rails | UPI, cards, EMI, COD, wallets and more |
| 9 | Success rate | Distribution and 7-day rolling reliability |
| 10 | Inventory risk | Store reserve status: adequate, low or critical |
| 11 | Correlation analysis | Order count vs. value vs. success rate (Pearson r) |
| 12 | Limitations | Scope, assumptions and governance |
| 13 | Descriptive → Predictive | Candidate ML models and features |
| 14 | Executive scorecard | One-page summary of key metrics |

## Key findings

- **Value is concentrated.** Prescription Eyeglasses and Sunglasses make up about 32% of orders but about 43.7% of value.
- **Value and volume leaders differ.** Designer/Luxury Eyewear has about 25K orders but ~INR 29 Cr in value (AOV ≈ INR 11,744).
- **Channel mix.** App leads on orders (36.3%) but has a low ticket size. Offline stores have the highest AOV (INR 2,324).
- **Segments.** Regular customers give the largest value share (43.1%). Premium/Designer has the highest AOV (INR 3,699).
- **Payments.** UPI leads on both order count and value. Credit Card and EMI skew toward higher-value orders.
- **Reliability.** Success rate is tightly clustered around 97.4% with no meaningful drift.
- **Correlation.** Order count and value are moderately correlated (r ≈ +0.65). Success rate is nearly independent of volume and ticket size.

## Tools and concepts

- Descriptive statistics: mean, median, quartiles, IQR, Pearson correlation
- Aggregation, share analysis and binned distributions
- Visualization: bar charts, line trends, donut chart, histograms
- Reference stack: Python (Pandas), SQL, Excel Pivot Tables, Power BI / Tableau, Kafka / Kinesis

## Limitations

- Synthetic data, not a real platform's volume
- Week 5 is a partial week (2 days) and should not be read as a demand drop
- No customer-level, return or refund data
- Findings are descriptive and non-causal
- Figures are nominal INR, with no adjustment for discounts or inflation

## Next steps (roadmap)

Demand forecasting (ARIMA, Prophet, LSTM), fraud and anomaly detection, success-rate early warning, and customer cohort and retention modeling.

## Repository structure

# RetailPulse: IBM Cognos Analytics Practical Record

A set of six hands-on practicals built in **IBM Cognos Analytics** using the fictional **RetailPulse** retail dataset. They cover the full reporting workflow, from a first list report to an interactive customer dashboard.

**Author:** Adarsh Patel 
**Programme:** BCA (Data Science & AI), School of Computer Applications, Babu Banaras Das University

---

## Practicals

| # | Title | Topic | Key skills |
|---|-------|-------|-----------|
| 1 | [First RetailPulse Report](Practical_1_First_Report.pdf) | Intro to Cognos Reporting | Package selection, list template, run and save |
| 2 | [Grouped Sales List Report](Practical_2_Grouped_List_Report.pdf) | List reports | Grouping (Region > Store), currency format, alignment, totals, page header |
| 3 | [Filter Sales by Region and Date](Practical_3_Filters.pdf) | Filters | Simple and advanced detail filters, AND logic, prompted filter |
| 4 | [Region × Product Crosstab](Practical_4_Region_Product_Crosstab.pdf) | Crosstab reports | Rows/columns/measures, nested measures, row and column totals |
| 5 | [Sales Prompt Report](Practical_5_Prompt_Report.pdf) | Prompt pages | Value, date-range and cascading prompts, linked filters, defaults |
| 6 | [Customer Insights Dashboard](Practical_6_Customer_Insights_Dashboard.pdf) | Dashboards | KPI card, line and bar charts, cross-filtering Region selector |

## What each practical covers

1. **First Report:** Connect to the *RetailPulse Sales* package and build a basic three-column list report (Region, Product Category, Sales Amount).
2. **Grouped List Report:** Group rows by Region and Store Name, format Sales Amount as currency, right-align numbers, add group and overall totals, and add a title and run date to the page header.
3. **Filters:** Scope the report to one region and the current quarter using a combined filter, then turn the Region filter into a reusable prompt.
4. **Crosstab:** Summarize Sales Amount and Quantity across Region and Product Category with grand totals that reconcile with the Practical 2 list report ($2,494,250 and 19,345 units).
5. **Prompt Report:** Build a prompt page with a Region prompt, a date-range prompt and a Store prompt that cascades from Region, each linked to a report filter, with default selections and a Finish button.
6. **Dashboard:** Using the *RetailPulse Customers* data module, assemble an Active Customers KPI card, a New vs Returning monthly trend line, a Loyalty Segment bar chart and a Region filter that cross-filters all widgets.

## Tools and data

- IBM Cognos Analytics (Reporting and Dashboards)
- *RetailPulse Sales* package (Practicals 1–5)
- *RetailPulse Customers* data module (Practical 6)

> All figures shown in the practical records are illustrative sample data.

## Repository structure

# RetailPulse: Power BI Practical Record (Practicals 7-10)

Four hands-on practicals in **Microsoft Power BI** using a sample **RetailPulse** retail dataset. They cover the full BI workflow: importing and cleaning data, modeling and DAX, time intelligence and performance tuning, then interactive dashboards, row-level security and Power Platform integration.

**Author:** Adarsh Patel
**Programme:** BCA (Data Science & AI), School of Computer Applications, Babu Banaras Das University

---

## Practicals

| # | Title | Key skills |
|---|-------|-----------|
| 7 | [Import and Transform RetailPulse Data](Practical_7_Import_Transform_RetailPulse.pdf) | Power BI interface, Power Query, data types, cleaning, conditional column, M code |
| 8 | [Model, Calculate and Publish a Sales Report](Practical_8_Model_Calculate_Publish_RetailPulse.pdf) | Star-schema relationships, basic DAX, calculated column, visuals, publishing |
| 9 | [Time Intelligence and Advanced DAX](Practical_9_Time_Intelligence_DAX_RetailPulse.pdf) | Date table, TOTALYTD, SAMEPERIODLASTYEAR, variables, ALL, Performance Analyzer |
| 10 | [Interactive Dashboard, RLS and Power Platform](Practical_10_Dashboard_RLS_PowerPlatform_RetailPulse.pdf) | Slicers, drill-through, bookmarks, row-level security, Power Automate, Power Apps |

## What each practical covers

### Practical 7: Import and Transform
- Explore Report, Table and Model views, the ribbon and the Data, Visualizations and Filters panes
- Load the Sales, Product and Store tables from an Excel workbook
- Set data types, remove blank rows (3) and duplicates (4), replace null quantities (5) with 0
- Add a **Sale Size** conditional column (Large if Sales Amount ≥ 1000): 46 Large, 104 Standard
- Review the Applied Steps and the equivalent Power Query (M) code

### Practical 8: Model, Calculate and Publish
- One-to-many, single-direction relationships: `Product → Sales ← Store`
- Measures: `Total Sales`, `Total Quantity`, `Average Order Value` (using `DIVIDE`)
- Calculated column: `Sales per Unit`
- Report page with a card, category bar chart, monthly line chart and Region slicer
- Publish to the Power BI service and share the report

### Practical 9: Time Intelligence and Advanced DAX
- Build a `CALENDAR` date table and mark it as the date table
- Measures: `Sales YTD`, `Sales LY`, `YoY Growth %` (with `VAR`/`RETURN`) and `Region Share %` (with `ALL`)
- Matrix of Year > Month with YTD, last-year and growth values
- Use **Performance Analyzer** to compare visual load times before and after optimization (e.g. Matrix 640 ms → 410 ms)

### Practical 10: Dashboard, RLS and Power Platform
- Slicers, a drill-through **Store Detail** page and bookmark buttons (chart view / table view)
- **Row-Level Security** roles: North Manager and South Manager, tested with *View as*
- Publish, assign users and pin a card to a dashboard
- Data alert triggering a **Power Automate** flow (email / Teams message)
- **Power Apps** visual showing details of the drilled-through store

## Dataset

Sample RetailPulse data: **150 sales orders, 8 products, 8 stores, 4 regions, Jan 2024 - Dec 2025**.

| Metric | Value |
|--------|-------|
| Total Sales | 139,794.72 |
| Total Quantity | 435 |
| Average Order Value | 931.96 |
| Top region by sales | East (34.1%) |

> All figures are generated from sample data and are illustrative.

## Core concepts

- **Power Query:** Applied Steps, data types, cleaning, M language
- **Data modeling:** star schema, cardinality, cross-filter direction
- **DAX:** measures vs. calculated columns, `CALCULATE`, `DIVIDE`, `ALL`, variables, time intelligence
- **Performance:** Performance Analyzer, reducing columns and visuals
- **Security and integration:** static RLS vs. dynamic RLS, Power Automate, Power Apps

## Tools

Power BI Desktop, Power BI Service, Power Query Editor, DAX, Power Automate, Power Apps, Excel (data source)

## Repository structure
