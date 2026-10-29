# Excel Sales Analytics: AtliQ Hardwares

An Excel-based sales and profitability analysis for **AtliQ Hardwares**, a consumer hardware and peripherals company. The project turns raw sales data into a set of pivot-table reports covering revenue, gross margin, market performance against target, products, and customers across **FY2019 to FY2021**.

The reports in this repository are PDF exports of the Excel pivot-table reports.

\---

## Business Questions Answered

* How did net sales and gross margin change from FY2019 to FY2021?
* Which divisions, markets, products and customers drive revenue?
* Which markets missed their FY2021 target, and by how much?
* How does gross margin vary by sub-zone, quarter and market?
* How did products launched in 2021 perform?
* What are the seasonal patterns across fiscal months?

\---

## Repository Structure

```
Excel-Sales-Analytics/
├── README.md
└── reports/
    ├── Division\_Report.pdf
    ├── GM\_\_by\_Qtrs-\_Subzone.pdf
    ├── Market\_perfomance\_vs\_Target.pdf
    ├── New\_Products\_2021.pdf
    ├── P\_L\_Performance\_by\_Months.pdf
    ├── P\_L\_Statement\_by\_Fiscal\_Year.pdf
    ├── P\_L\_Statement\_by\_Markets.pdf
    ├── Top\_5\_Countries.pdf
    ├── Top\_10\_Net\_Sales\_Product.pdf
    ├── Top5\_N\_bottom5.pdf
    └── Customer\_Performance\_Report.pdf
```

\---

## Reports Overview

|#|Report|What it shows|
|-|-|-|
|1|[Division Report](reports/Division_Report.pdf)|Net sales by division (N\&S, P\&A, PC), 2020 vs 2021 with growth %|
|2|[GM% by Quarter and Sub-zone](reports/GM__by_Qtrs-_Subzone.pdf)|Gross margin % by quarter for each sub-zone (ANZ, India, NA, NE, ROA, SE), FY2019 to FY2021|
|3|[Market Performance vs Target](reports/Market_perfomance_vs_Target.pdf)|Net sales by country for 2019 to 2021, plus the gap to the 2021 target in value and %|
|4|[New Products 2021](reports/New_Products_2021.pdf)|Net sales of the 16 products launched in 2021|
|5|[P\&L by Fiscal Months](reports/P_L_Performance_by_Months.pdf)|Monthly net sales, COGS, gross margin and GM% for each fiscal year, plus YoY net sales comparison|
|6|[P\&L by Fiscal Year](reports/P_L_Statement_by_Fiscal_Year.pdf)|Annual net sales, COGS, gross margin and GM%, with 21 vs 20 change|
|7|[P\&L by Markets](reports/P_L_Statement_by_Markets.pdf)|FY2021 net sales, COGS, gross margin and GM% for every market|
|8|[Top 5 Countries](reports/Top_5_Countries.pdf)|Five largest countries by net sales in 2021|
|9|[Top 10 Products by Net Sales](reports/Top_10_Net_Sales_Product.pdf)|Ten products with the highest net sales and their 2020 to 2021 growth|
|10|[Top 5 and Bottom 5 Products](reports/Top5_N_bottom5.pdf)|Best and worst products by quantity sold|
|11|[Customer Performance](reports/Customer_Performance_Report.pdf)|Net sales by customer for 2019 to 2021 with 21 vs 20 comparison|

> The fiscal year runs \*\*September to August\*\* (Q1 = Sep to Nov, Q2 = Dec to Feb, and so on, as laid out in the monthly P\&L report).

\---

## Key Findings

**Growth and profitability**

* Net sales grew from **87.5M (FY19)** to **196.7M (FY20)** to **598.9M (FY21)**, up 124.8% and then 204.5% year on year.
* Gross margin value grew from 36.2M to 218.2M, but **GM% declined every year: 41.4% → 37.3% → 36.4%**. Growth came with thinner margins.

**Divisions**

* **P\&A** is the largest division at 338.4M in FY21, about 56% of net sales.
* **PC** grew fastest (+313.7%); **N\&S** grew slowest (+84.4%).

**Markets**

* The **top 5 countries (India, USA, South Korea, Canada, UK)** account for 367.2M, roughly 61% of FY21 net sales. India alone contributes 161.3M (about 27%).
* **All 23 markets finished below their 2021 target**, with an overall shortfall of 54.9M (-8.4%). The largest gaps in value were USA (-10.2M) and India (-9.6M); the worst in percentage terms was Poland (-15.3%).
* FY21 gross margin is highest in New Zealand (48.2%), Japan (46.5%) and the UK (45.1%), and lowest in Germany (26.2%), Norway (29.5%), Austria and Italy (30.1% each). India, the largest market, sits at 32.0%.

**Sub-zones**

* India's GM% dropped from 42.4% in FY19 to 32.2% in FY20 and stayed near 32% in FY21.
* ANZ fell from 42.8% (FY20) to 38.3% (FY21).

**Seasonality**

* Q2 (Dec to Feb) is the peak. December 2021 reached the highest monthly net sales at 78.1M.
* March 2020 net sales dropped to 2.1M, down 67.1% on March 2019.

**Products and customers**

* The 16 products launched in 2021 generated **176.2M (about 29% of FY21 net sales)**. Leaders: AQ Qwerty (22.0M), AQ Trigger (20.7M) and AQ Gen Y (19.5M).
* **Amazon** is the largest customer at 82.1M, followed by AtliQ Exclusive (61.1M) and Atliq e Store (53.0M). These three make up about 33% of FY21 net sales.

\---

## Data Notes and Caveats

* **Currency labelling is inconsistent.** The same totals (87.5M, 196.7M, 598.9M) appear as INR in some reports and USD in others. Confirm the correct currency against the source data before quoting absolute values.
* **The "21 vs 20" column is defined differently across reports.** Division, P\&L and product reports show growth % (new minus old, divided by old). The Customer Performance report shows 2021 as a % of 2020 (its total is 304.5% versus 204.5% growth).
* Very high growth % for small-base items (for example Nova, Integration Stores, AQ Mx NB) reflects tiny 2020 values, not necessarily large absolute gains.
* Several reports use filters set to "All" (region, market, division, customer). Where a report shows blanks for a year, no sales were recorded in that period.

\---

## Tools and Techniques

* **Microsoft Excel**: pivot tables, calculated fields, conditional formatting (heat maps, data bars)
* Fiscal-calendar handling, YoY comparisons and variance-to-target analysis
* Report layout for management-style P\&L views

\---

## How to Use This Repository

1. Clone or download the repo.
2. Open any PDF in the `reports/` folder.
3. Read the report together with the filters shown at the top of each page.

```bash
git clone https://github.com/Rutvik84/Excel-Sales-Analytics.git
```

\---

## Data Source

AtliQ Hardwares is a company dataset.

\---

## Author

**Rutvik**
MBA (Business Analytics)
GitHub: [Rutvik84](https://github.com/Rutvik84)
LinkedIn: *https://www.linkedin.com/in/rutvik-savkare-51a3bb195/*

