# Shoprite Holdings JSE Executive Valuation Dashboard
### Power BI · DAX · M · Live Market Intelligence · FY2025
 
---
 
## Overview
 
A fully dynamic equity valuation platform built in Power BI for Shoprite Holdings Ltd (SHP.JO), JSE-listed. The dashboard ingests audited FY2025 financials, calculates a live DCF valuation, and recalculates the entire model in real time as assumptions change — replacing a manual, multi-day analyst workflow with an interactive, single-platform solution.
 
**Current Valuation Signal: OVERVALUED**
- Implied Share Price: R144.91 (Base scenario)
- Live JSE Price: R263.36
- Margin of Safety: -44.1%
- WACC: 12.56%
 
---
 
## The Problem
 
JSE equity analysts typically spend 2–3 days per company manually extracting data from SENS PDFs, rebuilding Excel DCF models, and recalculating sensitivity tables each reporting cycle. There is no live market price integration, no instant scenario switching, and no single executive view.
 
## The Solution
 
A 7-page Power BI platform that:
- Calculates WACC dynamically from 5 interactive input sliders
- Discounts projected free cash flows in real time as assumptions change
- Runs a reverse DCF to calculate the growth rate implied by the live market price
- Colour-codes a 5×5 sensitivity heatmap against the live JSE price
- Switches instantly between Bull, Base, and Bear scenarios via bookmarks
 
---
 
## Dashboard Pages
 
| Page | Description |
|---|---|
| Cover | Branded entry point with live valuation signal |
| P&L Overview | Revenue, margins, and 3-year trend chart |
| Valuation Engine | Live DCF · WACC sliders · Reverse DCF · Heatmap |
| Scenario Analysis | Bull / Base / Bear implied price comparison |
| Sensitivity Heatmap | 5×5 WACC vs Terminal Growth colour-coded matrix |
| Balance Sheet | Equity, debt, ROE, leverage, capital structure chart |
| Executive Summary | All key outputs on one print-ready page |
 
---
 
## Key Outputs — FY2025 Base Scenario
 
| Metric | Value |
|---|---|
| Revenue | R256,682m |
| EBIT Margin | 5.8% |
| Return on Equity | 24.5% |
| Free Cash Flow | R3,619m |
| Enterprise Value | R96,779m |
| Implied Share Price | R144.91 |
| Live JSE Price | R263.36 |
| Margin of Safety | -44.1% |
| Implied Market Growth Rate | 6.0% |
 
---
 
## Scenario Summary
 
| Scenario | Implied Price | vs JSE |
|---|---|---|
| Bull | R203.63 | -22.7% |
| Base | R146.60 | -44.3% |
| Bear | R110.56 | -58.0% |
 
---
 
## Technology Stack
 
| Layer | Tool | Detail |
|---|---|---|
| Data Source | Shoprite FY2025 AFS | Audited financials |
| Market Feed | Yahoo Finance | SHP.JO live price |
| ETL | Power Query (M) | 4-layer pipeline |
| Data Model | Star schema | Fact + Dimension tables |
| Calculations | DAX | 30+ measures |
| Visualisation | Power BI | 7-page dashboard |
 
---
 
## Dynamic WACC Engine
 
The WACC recalculates in real time from 5 interactive parameters:
 
| Input | Range | Default |
|---|---|---|
| Risk-Free Rate (RSA 10yr) | 7% – 12% | 8.82% |
| Beta | 0.50 – 1.50 | 0.85 |
| Equity Risk Premium | 4% – 10% | 8.0% |
| Cost of Debt | 8% – 15% | 11.0% |
| Terminal Growth Rate | 3% – 9% | 6.0% |
 
Every downstream output — PV of FCF, Terminal Value, Enterprise Value, Implied Share Price, Margin of Safety — cascades from WACC_Dynamic automatically.
 
---
 
## Sensitivity Heatmap
 
The 5×5 matrix shows implied share price at every combination of WACC (8%–16%) and Terminal Growth Rate (1%–5%), colour-coded against the live JSE price:
 
- Deep red → Heavily overvalued (MoS < -30%)
- Light red → Slight premium (MoS -5% to -30%)
- Light green → Fair value (MoS ±5%)
- Deep green → Undervalued (MoS > +5%)
 
The active cell (matching current slider values) is highlighted with a red border.
 
---
 
## Data Sources
 
- **Shoprite Holdings FY2025 Annual Financial Statements** — audited, sourced from JSE SENS
- **Yahoo Finance API** — SHP.JO live market price via Power Query web connector
- **Historical data** — FY2023, FY2024, FY2025
 
---
 
## Author
 
Built by **Saun Sibanyoni** · [@shawnanalytics](https://github.com/shawnanalytics)
Portfolio: [github.com/shawnanalytics/finance-valuation-portfolio](https://github.com/shawnanalytics/finance-valuation-portfolio)
 
