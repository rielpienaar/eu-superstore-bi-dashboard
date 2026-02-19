# KPI Definitions

This document defines the key performance indicators (KPIs) used in the EU Superstore Executive Dashboard to ensure consistent interpretation across analyses.

---

## Sales
**Definition:** Total revenue generated from product sales.  
**Calculation:** SUM(Sales)  
**Grain:** Transaction level aggregated to selected filter context  
**Format:** GBP (£)  
**Notes:** Includes all completed orders within the selected time period.

---

## Profit
**Definition:** Net profit generated from product sales after costs.  
**Calculation:** SUM(Profit)  
**Grain:** Transaction level aggregated to selected filter context  
**Format:** GBP (£)  
**Notes:** Negative values indicate loss-making transactions or products.

---

## Median Basket Size
**Definition:** Median revenue per order (customer transaction value).  
**Calculation:** MEDIAN(Sales per Order ID)  
**Grain:** Order level  
**Format:** GBP (£)  
**Business Meaning:** Represents the typical customer spend per transaction, less sensitive to extreme values than average basket size.

---

## Total Customers
**Definition:** Number of unique customers who placed orders.  
**Calculation:** COUNTD(Customer ID)  
**Grain:** Customer level  
**Notes:** A customer is counted once regardless of number of orders.

---

## Year-over-Year (YoY) Change
**Definition:** Percentage change in a KPI compared to the previous year.  
**Calculation:**  
(Current Year KPI − Previous Year KPI) / Previous Year KPI  
**Format:** Percentage (%)  
**Notes:** Calculated for Sales, Profit, Median Basket Size, and Customers.

---

## Sales by Category
**Definition:** Total sales aggregated by product category.  
**Calculation:** SUM(Sales) by Category  
**Grain:** Category level  
**Purpose:** Identifies revenue contribution by major product groups.

---

## Sales by Country
**Definition:** Total sales aggregated by customer country.  
**Calculation:** SUM(Sales) by Country  
**Grain:** Country level  
**Purpose:** Supports geographic performance analysis.

---

## Top Sub-Categories
**Definition:** Highest-revenue product sub-categories.  
**Calculation:** SUM(Sales) by Sub-Category  
**Grain:** Sub-Category level  
**Purpose:** Identifies product-level revenue drivers.

---

## Profit Margin (Category)
**Definition:** Profitability ratio for each product category.  
**Calculation:** SUM(Profit) / SUM(Sales)  
**Format:** Percentage (%)  
**Purpose:** Evaluates category profitability and cost efficiency.
