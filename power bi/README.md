# Finance Dashboard – Power BI

A one-page, dark-themed **Power BI dashboard** that tracks revenue, cost, profit, discounts and units sold across customer segments, countries and products.

> The dashboard page in the report is named **"Q9 - Finance Dashboard"**.

## Overview

The dashboard answers questions such as:

- How much did we sell, what did it cost, and how much profit did we make?
- Which segments, countries and products drive sales and profit?
- How do sales, COGS and profit change month by month?
- Where do discounts go, and which segments lose money?

## Dataset

The dashboard uses one table, `financials`:

| Item | Detail |
|------|--------|
| Rows | 700 |
| Period | Sep 2013 – Dec 2014 (monthly dates, 16 months) |
| Segments | Government, Small Business, Enterprise, Midmarket, Channel Partners |
| Countries | United States of America, Canada, France, Germany, Mexico |
| Products | Paseo, VTT, Amarilla, Velo, Montana, Carretera |
| Key columns | Units Sold, Manufacturing Price, Sale Price, Gross Sales, Discounts, Sales, COGS, Profit, Date |

There are no missing values or duplicate rows in this table.

## Dashboard contents

**Header:** title ("FINANCE DASHBOARD – Revenue | Cost | Profitability | Performance") and a button that links to https://www.excelr.com/.

**Slicers (5):** Year, Quarter, Month, Segment, Country. They filter every visual on the page.

**KPI cards:** Total Sales, Total COGS, Total Profit, Total Quantity, Average Discount.

**Visuals**

| Visual | Type |
|--------|------|
| Sales, COGS and Profit trend by month | Line chart |
| Sales by Segment | Bar chart |
| Profit by Segment | Donut chart |
| Sales by Country | Map |
| Profit by Country & Year | Ribbon chart |
| Top 5 Product by Sales | Bar chart |
| Top 5 Product by Profit | Bar chart |
| Quantity by Segment | Column chart |
| Discount by Segment | Column chart |
| Profit Analysis by Year, Segment & Country | Decomposition tree |

## Key figures

| KPI | Value |
|-----|-------|
| Total sales | 118.73M |
| Total COGS | 101.83M |
| Total profit | 16.89M (14.2% of sales) |
| Units sold | 1,125,806 |
| Average discount per record | 13,150 |

## Findings

**Segments**

| Segment | Sales | Profit | Profit as % of sales |
|---------|-------|--------|----------------------|
| Government | 52.50M | 11.39M | 21.7% |
| Small Business | 42.43M | 4.14M | 9.8% |
| Enterprise | 19.61M | -0.61M | -3.1% |
| Midmarket | 2.38M | 0.66M | 27.7% |
| Channel Partners | 1.80M | 1.32M | 73.1% |

- **Government is the biggest earner:** it brings in about 44% of sales and about 67% of profit.
- **Enterprise is the only segment losing money.** All 58 loss-making records in the data belong to Enterprise (about -0.78M in total).
- **Small Business has the highest discounts** (3.51M in total), and its margin is under 10%.
- **Channel Partners has the highest margin** (73.1%) but is the smallest segment by sales.

**Countries** – Sales are fairly even, from 20.95M (Mexico) to 25.03M (USA). Profit is not: France (3.78M) and Germany (3.68M) lead, while the USA has the highest sales but the lowest margin (12.0%).

**Products** – Paseo is first in both sales (33.01M) and profit (4.80M). The top 5 products by sales and by profit are the same five (Paseo, VTT, Amarilla, Velo, Montana). Carretera is last on both. Velo has the lowest margin (12.6%).

**Time** – December 2014 is the most profitable month (2.03M) and November 2014 the least (0.60M).

## Notes

- The data covers only Sep–Dec 2013 for 2013, but all of 2014, so year-over-year comparisons are not like-for-like.
- "Average Discount" is the average discount amount per record, not a percentage.

## How to use

1. Download `Finance_Dashboard.pbix`.
2. Open it in **Power BI Desktop** (free, Windows). The file cannot be previewed on GitHub.
3. Use the slicers at the top to filter, and click a chart element to cross-filter the other visuals.

## Repository structure

```
├── Finance_Dashboard.pbix
└── README.md
```

## Author

**Ambati Sarath**
[LinkedIn](https://www.linkedin.com/in/ambatisarath/)
