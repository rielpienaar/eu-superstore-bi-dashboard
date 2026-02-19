# Data Dictionary

This document describes the fields used in the EU Superstore dataset and dashboard model.

---

## Order ID
**Type:** String  
**Description:** Unique identifier for each transaction/order.  
**Grain:** Order level  
**Example:** ES-2019-152156  

---

## Order Date
**Type:** Date  
**Description:** Date when the order was placed.  
**Grain:** Order level  
**Use:** Time-series analysis, YoY comparisons, trend analysis.

---

## Customer ID
**Type:** String  
**Description:** Unique identifier for each customer.  
**Grain:** Customer level  
**Use:** Customer counts and behavioural metrics.

---

## Country
**Type:** String  
**Description:** Customer country where the order was placed or delivered.  
**Grain:** Order level  
**Use:** Geographic analysis and map visualisation.

---

## Region
**Type:** String  
**Description:** Sales region grouping multiple countries.  
**Grain:** Order level  
**Use:** Regional performance filtering and aggregation.

---

## Category
**Type:** String  
**Description:** High-level product classification.  
**Values:** Furniture, Office Supplies, Technology  
**Grain:** Product level  
**Use:** Category performance analysis.

---

## Sub-Category
**Type:** String  
**Description:** Detailed product classification within category.  
**Examples:** Phones, Chairs, Copiers, Storage  
**Grain:** Product level  
**Use:** Product-level performance ranking.

---

## Sales
**Type:** Decimal (GBP)  
**Description:** Revenue generated from the transaction.  
**Grain:** Order line level  
**Aggregation:** SUM  
**Use:** Revenue KPIs and category/country analysis.

---

## Profit
**Type:** Decimal (GBP)  
**Description:** Net profit from the transaction after costs.  
**Grain:** Order line level  
**Aggregation:** SUM  
**Use:** Profit KPIs and margin analysis.

---

## Derived Fields (Dashboard)

### Sales per Order
**Calculation:** SUM(Sales) per Order ID  
**Purpose:** Basket size analysis.

### Year
**Calculation:** YEAR(Order Date)  
**Purpose:** Time filtering and YoY analysis.

### YoY Metrics
**Calculation:** KPI compared to previous year  
**Purpose:** Growth indicators.
