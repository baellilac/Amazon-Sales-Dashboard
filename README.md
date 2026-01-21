# Amazon Sales Analytics Dashboard

Interactive Power BI dashboard analyzing US-based Amazon e-commerce sales data (~113K orders).

## Overview

This comprehensive Power BI dashboard provides in-depth analytics for Amazon e-commerce sales, tracking Year-to-Date (YTD) performance against prior year metrics. The dashboard enables identification of top and bottom performers across categories, states, regions, and shipping methods, delivering actionable business insights for strategic decision-making.

**Key Business Insight Example**: The dashboard reveals declining Office Supplies sales (-1.22% YoY) despite profit gains (+4.5%), highlighting opportunities for strategic optimization.

## Purpose

- Track **Year-to-Date (YTD) performance** versus prior year
- Identify **top and bottom performers** by:
  - Category
  - State
  - Region
  - Shipping method
- Derive actionable **business insights** for strategic planning
- Monitor **profitability trends** alongside sales volume
- Analyze **geographic performance** across US markets

## Tech Stack

- **Power BI Desktop** (latest version)
- **DAX** - Advanced calculations using:
  - `TOTALYTD` for year-to-date aggregations
  - `SAMEPERIODLASTYEAR` for prior year comparisons
  - `FORMAT` for KPI formatting (e.g., "#107.2K")
- **Power Query** - Data cleaning and modeling
- **SQL Server** - Primary data import (with CSV fallback option)
- **Date table** - Custom date dimension for time intelligence functions

## Data Sources

- **Modified Kaggle e-commerce dataset**:
  - **Orders table** (~113K rows) containing:
    - Customer ID
    - Category
    - Sales amount
    - Profit
    - Quantity
    - State/Region
    - Shipping method
  - **US States table** with latitude/longitude coordinates for geographic mapping

## Key Features & Insights

###  KPI Banner
Dynamic year-to-date metrics with prior year comparisons:
- **YTD Sales** - Total sales performance
- **YTD Profit** - Profitability tracking
- **YTD Quantity** - Units sold
- **YTD Margin** - Profit margin percentage
- **YoY Growth** - Year-over-year growth with conditional formatting (green for positive, red for negative)
- **Monthly trends** - Visual trend indicators
- **Icon indicators** - Quick visual status indicators

###  Sales by Category Matrix
Comprehensive category performance analysis:
- **YTD vs. PYTD Sales** - Current year versus prior year totals (displayed in millions)
- **YoY Percentage Change** - Growth or decline by category
- **Trend Icons** - Visual indicators for performance direction
- **Insight Example**: Office Supplies showing -1.22% YoY decline in sales volume

###  Sales by State
Geographic performance visualization:
- **Bubble Map** - Interactive US map visualization
- **Bubble Size** - Proportional to sales volume
- **Color Coding** - Differentiated by region
- State-level performance at a glance

###  Top/Bottom Products
Product performance rankings:
- **Top Products** - Ranked by YTD sales performance
- **Bottom Products** - Identifying underperforming items
- Helps prioritize inventory and marketing efforts

###  Sales by Region/Shipping
Performance analysis by:
- **Sales by Region** - Bar charts showing regional performance
- **Sales by Shipping Method** - Optimization opportunities for logistics
- Comparative analysis across different dimensions

###  Interactivity Features

- **Slicers**:
  - Customer segment filtering
  - Category selection
- **Filters**:
  - State-level filtering
  - Region-based filtering
- **Cross-filtering**: Click any visual to filter related visuals
- **Drill-through capabilities** for detailed analysis

## Business Impact

The dashboard enables strategic decision-making through:

- **Performance Optimization**: Identify declining categories (e.g., Office Supplies) and develop targeted strategies
- **Profit Analysis**: Understand profit gains (+4.5%) even when sales decline (-1.22%), revealing margin improvements
- **Seasonal Strategies**: Identify low-performing periods (e.g., December) and create targeted offers or campaigns
- **Category Focus**: Prioritize high-profit categories despite volume drops
- **Geographic Expansion**: Identify top-performing states and regions for growth opportunities
- **Logistics Optimization**: Analyze shipping method performance for cost reduction

## Key Metrics Tracked

### Year-to-Date Metrics
- Total Sales (YTD)
- Total Profit (YTD)
- Total Quantity (YTD)
- Profit Margin (YTD)

### Comparative Metrics
- Year-over-Year (YoY) Growth Percentage
- Prior Year-to-Date (PYTD) Comparisons
- Month-over-Month Trends

### Performance Indicators
- Category Performance Rankings
- Regional Performance Metrics
- State-Level Sales Distribution
- Shipping Method Efficiency


**Dataset**: ~113K orders from US-based Amazon e-commerce sales  



