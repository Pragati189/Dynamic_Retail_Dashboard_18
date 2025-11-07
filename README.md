# Dynamic Retail Dashboard
An interactive retail dashboard crafted in Excel—merging pivot tables, slicers, and charts to track KPIs like sales, stock, and regional performance. Designed for clarity and control, it turns spreadsheets into a strategic insights engine. 
## Overview
A dynamic retail dashboard in Excel is an interactive visual tool that tracks and analyzes key retail metrics—like sales, inventory, and customer behavior—using formulas, charts, slicers, and pivot tables. It allows users to filter data by region, product category, time period, and more.
## Datasets Used
### 1. Orders Table
The Orders table contains details of customer orders, including product, shipping, and financial metrics.
#### Sample Data:
### 📦 Sample Retail Orders Table

| Row ID | Order ID | Order Date | Ship Date | Ship Mode | Customer Name | Segment | Region | Category | Sub-Category | Product Name | Sales | Quantity | Discount | Profit |
|--------|----------|------------|-----------|-----------|----------------|---------|--------|----------|--------------|---------------|--------|----------|----------|--------|
| 1      | CA-2016-152156 | 11/08/2016 | 11/11/2016 | Second Class | Claire Gute | Consumer | West | Furniture | Bookcases | Bush Somerset Collection Bookcase | 261.96 | 2 | 0.0 | 41.91 |
| 2      | CA-2016-152156 | 11/08/2016 | 11/11/2016 | Second Class | Claire Gute | Consumer | West | Furniture | Chairs | Hon Deluxe Fabric Upholstered Chairs | 731.94 | 3 | 0.0 | 219.58 |
| 3      | CA-2016-138688 | 06/12/2016 | 06/16/2016 | Second Class | Darrin Van Huff | Corporate | West | Office Supplies | Labels | Self-Adhesive Address Labels | 14.62 | 2 | 0.0 | 6.87 |
### 2. Returns Table
Tracks orders that have been returned along with the associated markets.
#### Sample Data:
| BIS | Return Date | Product Code |
|-----|-------------|--------------|
| Yes | 02-Mar-2020 | AAMAM        |
| Yes | 03-Mar-2020 | AAPAM        |
| Yes | 04-Mar-2020 | AAPMC        |
| Yes | 05-Mar-2020 | AAPNC        |
| Yes | 06-Mar-2020 | AAPOC        |
| Yes | 07-Mar-2020 | AAPPC        |
| Yes | 08-Mar-2020 | AAPQC        |
| Yes | 09-Mar-2020 | AAPRC        |
| Yes | 10-Mar-2020 | AAPSC        |
### 3. People Table
Contains details about sales representatives and their respective regions.
#### Sample Data:
| Person         | Region     |
|----------------|------------|
| Anna           | America    |
| Chuck Williams | South      |
| Clay Mendez    | West       |
| Greg Collins   | East       |
| Julia Alvarez  | America    |
| Guleon Roberts | Caribbean  |
### KPI Table
The KPI table consolidates the most essential performance metrics for the retail analysis. These KPIs allow the dashboard to provide actionable insights by comparing important aspects of sales performance.
KPI	NAME	Symbol
Sum of Sales	Total Sales	📈
Sum of Profit	Total Profit	💰
Sum of Quantity	Total Qty	📦
Count of Order ID	No. of Orders	🛒
Sum of Profit Margin	Profit Margin	🔍

<img width="357" height="145" alt="image" src="https://github.com/user-attachments/assets/3d5189ca-b268-4e3a-8203-0b8e894a7dab" 

## Problem Statements Solved with Steps
### 1. Key Performance Indicators (KPIs)
**Objective:** Calculate and display Total Sales, Total Profits, Total Quantity, Number of Orders, and Profit Margin dynamically.
##### Steps:
  1. Import the Orders Table into Excel using Power Query.
  2. Create calculated columns for:
     + Profit Margin = Profit/Sales
     + Total Orders = Count of Order ID
  3. Use Excel formulas to calculate:
       + Total Sales = =SUM(Sales)
       + Total Profit = =SUM(Profit)
       + Total Quantity = =SUM(Quantity)
  4. Build a dynamic KPI table and use symbols to enhance visual appeal.
<img width="627" height="94" alt="Screenshot 2025-11-07 150459" src="https://github.com/user-attachments/assets/662713c9-595c-4405-a2a3-39aa4f649ff7" />

### 2. Sales and Profit Analysis
**Objective:** Visualize sales and profit trends to identify patterns.
##### Steps:
  1. Create a Pivot Table with **Order Date** grouped by Year and Month.
  2. Add **Sales** and **Profit** as values.
  3. Create a Line Chart to display trnds for Sales and Profit.
  4. Apply slicers to filter by category, market, or region dynamically.
### 3. Category -Wise Profit
**Objective:** Analyse profitability across product categories.
##### Steps:
   1. Create a Pivot Table using Category as rows and Profit as values.
   2. Sort the table in descending order of Profit.
   3. Create a Bar Chart to visualize category-wise profit.
   4. Add slicer for interactivity.
### 4. Segment-Wise Sales Share(%)
**Objective:** Display the proportion of sales for each customer segment.
##### Steps: 
   1. Create a Pivot Table with Segment as rows and Sales as values
   2. Calculate percentage share using =Sales/Total Sales*100.
   3. Create a Pie Chart or Donut Chart to display the Sales share.
   4. Add lables to show percentage value dynamically.
### 5. Sales by Country
**Objective:** Analyse Sales performance by country.
##### Steps:
   1. Create a Pivot Table with Country as rows and sales as values.
   2. Sort the table in descending order of Sales.
   3. Use Conditional Formatting or a Heatmap to highlight top performing countrues.
### 6. Top 5 Subcategories
**Objective:** Identify the top 5 performing subcategories.
##### Steps: 
   1. Create a Pivot Table with Sub-category as rows and Sales as values.
   2.  Sort the table in descending order of Sales.
   3.  Filter to display the top 5 subcategories.
   4.  Use a Column Chart to visualize results.
### Dynamic Features
The dashboard includes:
  1. **Dynamic Charts:** Update in real-time based on slicer inputs.
  2. **Power Query Integration:**  Automates data cleaning and transformation.
  3. **KPI Table:** Highlights critical metrics at a glance.
### New Steps for Extensions
Additional insights to enhance the dashboard:
  1. **Return Analysis:** Investigate return rate by market or product category.
  2. **Top and Bottom Customers:** Identify most and least profitable customers.
  3. **Market Analysis:** Compare performance across different markets.
  4. **Product Analysis:** Evaluate individual product contributions.
### Significance
This dashboard empowers retail businesses to:
  + Track performance through KPIs.
  + Understand category, segment, and geographic trends.
  + Make data-driven decisions to optimize operations.
### Visuals
This repository includes:
  + Visual examples for each solved problem statemnent.
  + Snapshots of the final dashboard with all components.










