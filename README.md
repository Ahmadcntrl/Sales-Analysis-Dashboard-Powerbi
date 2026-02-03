# 📊 Sales Performance & Return Analysis Dashboard
## 📝 Project Overview
This repository contains a comprehensive Power BI solution designed to track retail performance, monitor budget achievement, and analyze product return risks. The project transforms raw transactional data into actionable insights, focusing on high-growth categories and operational efficiency.

## 🏗️ Data Architecture (Star Schema)
The model is built on a robust star schema to ensure scalability and filter efficiency.

## Fact Tables
- Sales Data: The core transactional table containing Sales, Profit, Quantity, and Cost metrics.

- Budget: Contains Adjusted_target values mapped by Date and Category to enable Variance Analysis.

- Item Return: A specialized fact table tracking return status (Yes/No) linked via Order_ID.

## Dimension Tables
- Dim_product: Contains product hierarchies including Category, Sub-Category, and Product Name.

- Dim_customer: Enables segmentation by customer name, ID, and business segments.

- Dim_territory: Facilitates regional analysis across Country, Region, State, and City.

- DimCalendar: A dedicated time dimension supporting Time Intelligence functions.

- Dim_category: A normalized table for high-level category grouping.

## 📈 Key Business Insights
### 1. Financial Performance
- Revenue & Profit: The business generated $113M in Total Sales with an 87.56% Profit Margin.

- Growth Trend: Sales grew from $19M in 2018 to $44M in 2020, achieving a 51.24% growth rate.

- Target Achievement: The organization surpassed its $63M target by achieving $91M in Net Sales, representing a 144.46% achievement rate.

### 2. Category & Regional Drivers
- Dominant Category: Stationary & Office Items is the primary revenue driver, contributing $55M to net sales.

- Regional Strength: The West Region leads in sales within the Stationary category.

### 3. Operational Risk (Returns)
- Return Metrics: The overall Return Rate is 19.22%, with 1,284 total return orders.

- High-Risk Products: Items like Crayola Colored Pencils show a critical 75% return rate.

### 🛠️ Technical Implementation Details
- DAX Measures: Used for calculations including Achievement %, Return Rate %, and Sales Previous Period.

- Decomposition Tree: Implemented to drill down into the root causes of return amounts.

- Time Intelligence: Leveraged the DimCalendar to compare performance against historical data.

- Interactive UI: Custom sidebar navigation and dynamic filtering by Year, Region, and Category.

### 🚀 How to Use
- Clone the Repository: git clone https://github.com/Ahmadcntrl/Sales-Analysis-Dashboard-Powerbi.git

- Open the .pbix File: Requires Power BI Desktop.

- Interact: Use the sidebar to toggle between Sales Analysis, Item Return Analysis, and Comparison Analysis pages.
