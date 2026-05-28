# Superstore Sales & Delivery Performance Dashboard

This project was created as the final project of the Tableau module.  
The goal was to analyze sales, profit, profitability, and delivery performance using the Superstore Sales dataset.

The project focuses on building interactive Tableau dashboards that help users understand business performance across time, product categories, shipping methods, customer segments, and U.S. states.

## Project Overview

The analysis was built around three main business questions:

1. How did sales and profit change over time?
2. Which product categories, sub-categories, and shipping methods are more or less profitable?
3. How does delivery performance vary by shipping method, delivery duration, and state?

## Dataset

The project uses the **Sample Superstore** dataset.

Main fields used in the analysis:

- Order Date
- Ship Date
- Ship Mode
- Segment
- Category
- Sub-Category
- State
- Sales
- Profit
- Order ID

## Dashboards and Visualizations

### 1. Sales and Profit Time Series

A monthly time series was created for the years 2020–2023.  
Sales and profit were visualized together using a dual-axis chart with a shared scale.

Interactive filters were added for:

- Ship Mode
- Segment

Both filters were configured with an Apply button to give users more control over the dashboard view.

### 2. Profitability Analysis by Category and Shipping Method

This analysis compares profitability across product categories, sub-categories, and shipping methods.

A calculated field was created to measure relative profit percentage:

```text
Profit Ratio = SUM(Profit) / SUM(Sales)
