# JSE Executive Valuation Dashboard
### Shoprite Holdings Ltd (SHP.JO) — Equity Valuation Platform

## Project Overview
A production-grade financial analytics dashboard built with 
SQL, Power Query (M), DAX, and Power BI Desktop. Replaces 
manual Excel-based equity valuation with a live, automated 
platform.

## Live Features
- **Live JSE Price Feed** — Yahoo Finance API (SHP.JO)
- **Interactive DCF Engine** — WACC slider updates 
  implied share price in real time
- **5-Year Forecast Model** — Implied Share Price R147.27
- **Sensitivity Heatmap** — WACC vs Growth rate matrix
- **Bull/Base/Bear Scenarios** — One-click scenario switching
- **Reverse DCF** — Implied market growth rate calculation
- **Margin of Safety** — Live vs implied price comparison

## Technology Stack
| Layer | Technology | Purpose |
|-------|-----------|---------|
| 1 | SQL Server | Schema design, normalised fact tables |
| 2 | Power Query (M) | ETL pipeline, data cleaning |
| 3 | DAX | 28 financial measures, DCF engine |
| 4 | Power BI Desktop | 7-page executive dashboard |

## Key Results (FY2025)
- Implied Share Price: **R147.27** (DCF at WACC=12%)
- Live Market Price: **R263.36** (Yahoo Finance)
- Margin of Safety: **-44.1%**
- Return on Equity: **24.5%**
- Revenue: **R256,682m**

## Dashboard Pages
1. Cover Page
2. P&L Overview
3. Valuation Engine
4. Scenario Analysis
5. Sensitivity Heatmap
6. Balance Sheet
7. Executive Summary

## Data Source
Shoprite Holdings FY2025 Audited Annual Financial Statements
