# POWER BI CAPSTONE PROJECT

## Retail Sales & Profitability Analysis

**Dataset:** FreshChoice_PowerBI.xlsx  
**Role:** Business Intelligence / Data Analyst

---

## Business Scenario:

You have been hired as a **Data Analyst** for a supermarket chain called **FreshChoice Mart**, operating multiple stores across Kenya.

Management wants a **Power BI dashboard** that helps them:

* Monitor **sales and profitability**
* Track **performance vs targets**
* Understand **store, product, and time-based trends**
* Make **data-driven decisions**

You are required to build an **end-to-end Power BI solution**.

---

## Dataset Description

You are provided with an Excel file containing **5 sheets**:

1. **Sales** – Transaction-level data (2,500 records)
2. **Products** – Product master data
3. **Stores** – Store and location information
4. **Calendar** – Date table (2023–2024)
5. **Targets** – Monthly sales & profit targets per store

---

## Project Objectives

By the end of this project, you should be able to:

* Clean and transform data using **Power Query**
* Build a proper **Star Schema data model**
* Create **DAX measures** for business KPIs
* Design **interactive dashboards**
* Answer real **business questions**

---

## PROJECT TASKS (STEP BY STEP)

---

## TASK 1: Load & Clean Data (Power Query)

1. Open **Power BI Desktop**
2. Import the Excel file
3. Load all sheets:
   * Sales
   * Products
   * Stores
   * Calendar
   * Targets
4. In **Power Query**, perform the following:
   * Confirm correct data types (Date, Text, Decimal, Whole Number)
   * Remove any unnecessary columns
   * Rename columns for clarity (user-friendly names)
   * Ensure no duplicate primary keys

**Deliverable:** Cleaned data loaded into Power BI with no errors.

---

## TASK 2: Data Modeling (Model View)

Create the following relationships:

| From Table | Column       | To Table | Column     | Relationship |
| ---------- | ------------ | -------- | ---------- | ------------ |
| Sales      | Product_ID   | Products | Product_ID | Many to One  |
| Sales      | Store_ID     | Stores   | Store_ID   | Many to One  |
| Sales      | Invoice_Date | Calendar | Date       | Many to One  |
| Targets    | Store_ID     | Stores   | Store_ID   | Many to One  |

Ensure:

* **Single direction filtering**
* **Star schema design**
* No circular relationships

**Deliverable:** A clean, optimized data model.

---

## TASK 3: Create Core DAX Measures

Create a **Measures table** and add the following measures:

### Sales & Profit Measures

* Total Sales
* Total Quantity
* Total Cost
* Total Profit
* Profit Margin %

### Time Intelligence Measures

* Sales Last Year
* Sales Growth %

### Target Performance Measures

* Monthly Sales Target
* Monthly Profit Target
* Sales vs Target %
* Profit vs Target %

**Deliverable:** All measures working correctly across filters.

---

## TASK 4: Build Report Pages

---

### Page 1: Executive Overview

**Visuals Required:**

* KPI Cards:
  * Total Sales
  * Total Profit
  * Profit Margin %
  * Sales vs Target %
* Line Chart:
  * Monthly Sales Trend
* Bar Chart:
  * Sales by Store
* Slicers:
  * Year
  * Month
  * Store
  * Category

**Purpose:** High-level performance view for executives

---

### Page 2: Store Performance

**Visuals Required:**

* Bar Chart: Sales by Store
* Bar Chart: Profit by Store
* Table:
  * Store Name
  * Total Sales
  * Total Profit
  * Profit Margin %
  * Sales vs Target %
* Conditional formatting:
  * Red if Sales vs Target < 90%
  * Green if > 100%

**Purpose:** Identify top and underperforming stores

---

### Page 3: Product & Category Analysis

**Visuals Required:**

* Tree Map or Bar Chart: Sales by Category
* Top 10 Products by Sales
* Top 10 Products by Profit
* Matrix:
  * Category to Product hierarchy
  * Measures: Sales, Profit, Margin %

**Purpose:** Product profitability insights

---

### Page 4: Time Analysis

**Visuals Required:**

* Line Chart: Sales by Month
* Column Chart: Sales by Quarter
* Bar Chart: Sales by Day of Week
* Slicer: Year

**Purpose:** Seasonality and trend analysis

---

## TASK 5: Interactivity & UX

* Enable **drill-down** on time visuals
* Use **tooltips** to show:
  * Profit
  * Margin %
* Ensure slicers affect all visuals
* Use consistent colors and titles

**Deliverable:** A professional, easy-to-use dashboard.

---

## TASK 6: Insights & Recommendations (Written)

Create a **1-2 page analysis** answering:

1. Which store performs best overall and why?
2. Which category generates the highest profit margin?
3. Are there stores consistently missing targets?
4. Any seasonal sales patterns?
5. Which products sell a lot but generate low profit?

**Deliverable:** Written insights with data-backed conclusions.

---

## Final Deliverables Checklist

* Power BI (.pbix) file
* Clean data model
* DAX measures
* 4 report pages
* Written business insights

---

## Skills Demonstrated

* Power Query (ETL)
* Data Modeling
* DAX
* Business Analytics
* Dashboard Design
* Real-world decision support
