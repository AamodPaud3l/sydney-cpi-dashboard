# Sydney Cost of Living – CPI Dashboard (Power BI)

## Overview
This project analyses **Sydney’s Consumer Price Index (CPI)** to understand cost-of-living trends, identify inflation drivers, and explore how individual CPI categories behave over time.

The dashboard is intentionally designed to separate:
- **Snapshot KPIs** (latest available data), and
- **Exploratory analysis** (historical trends and category-level deep dives).

This approach helps avoid ambiguity while still allowing flexible exploration.

---

## Key questions answered
- What is the current level of inflation in Sydney?
- Which CPI categories are driving inflation in a given month?
- Is inflation pressure accelerating or easing?
- Is inflation broad-based or concentrated across categories?
- How does a specific category compare to overall CPI?
- Is a category’s price movement stable or volatile?

---

## Dashboard structure

### 1. Overview page
- Latest CPI price index (base = 100)
- Annual (YoY) and monthly (MoM) inflation
- Inflation momentum indicator (accelerating / easing / stable)
- Top 10 CPI categories by annual inflation (YoY) for a selected month
- Searchable category table to explore **any** CPI category and drill through

---

### 2. Category deep dive
- Latest price index, YoY and MoM for the selected category
- Long-term price index trend
- Difference vs overall CPI
- 12-month rolling price volatility
- Contextual KPI tooltips when hovering over the trend chart

---

## Design decisions
- KPIs are fixed to the **latest available month** to provide a clear snapshot.
- Exploratory visuals (Top 10 chart, category table) allow **month-by-month analysis** without affecting headline KPIs.
- Drill-through is used for focused, category-level investigation.
- Volatility is calculated over a rolling 12-month window to reflect **typical price stability**, not single-month noise.
- Colour usage reflects inflation context (rising prices highlighted cautiously rather than aggressively).

---

## Tools & techniques
- Power BI Desktop
- DAX measures
- Dimensional data model (Date and Category dimensions)
- Drill-through navigation
- Report-page tooltips for contextual insights

---

## Data source
- **Australian Bureau of Statistics (ABS)** – Consumer Price Index (CPI), [Link](https://www.abs.gov.au/statistics/economy/price-indexes-and-inflation/consumer-price-index-australia/nov-2025)

---

## How to view
1. Download the `.pbix` file from this repository  
2. Open it using **Power BI Desktop (free)**  

---

## Screenshots
Screenshots of the Overview and Category Deep Dive pages are available in the `/screenshots` folder.
