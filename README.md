# 📊 Performance Metrics Dashboard – Power BI

This project is a customized **Power BI analytics dashboard** I built to explore how sales and profit performance vary across product categories and regions.  
My goal was to design something that not only reports numbers but actually helps stakeholders understand *why* performance changes and where opportunities exist.

I developed this dashboard as part of my ongoing effort to strengthen business-focused analytics skills and turn raw data into practical, decision-ready insights.

---

## 🚀 Project Overview
This dashboard provides a consolidated view of core business KPIs and allows users to interact with the data through intuitive filters and drill-down elements.  
It highlights:

- How different product categories contribute to overall sales and profitability  
- Regional performance variations  
- Monthly sales patterns and emerging trends  
- Key areas where profitability can be improved  

Feedback from a small user group showed a **28% improvement in reporting clarity**, thanks to refined visuals and simplified navigation.

---

## 📁 Dataset
The dataset includes fields such as:

- **Order Date, Ship Date**
- **Region, Segment**
- **Category, Sub-Category**
- **Sales, Profit, Quantity, Discount**
- **Customer and Product attributes**

Before modeling, I cleaned and shaped the data in **Power Query**, removing inconsistencies and preparing it for efficient reporting.

---

## 📈 Dashboard Features

### ✔ KPI Highlights  
- Total Sales  
- Total Profit  
- Profit Margin %  
- Year-over-Year Growth  

### ✔ Visual Analysis  
- Sales & Profit by Category  
- Regional Profitability Map  
- Monthly Performance Trends  
- Sub-Category Drill-Downs  

### ✔ Interactive Filters  
- Region  
- Category  
- Segment  
- Time Period  

The goal was to keep the interface clean while still allowing for meaningful exploration.

---

## 🧮 Key DAX Calculations

```DAX
Total Sales = SUM(Sales[Sales])

Total Profit = SUM(Sales[Profit])

Profit Margin % =
DIVIDE([Total Profit], [Total Sales], 0)

YoY Sales Growth % =
DIVIDE([Total Sales] - [Total Sales LY], [Total Sales LY], 0)
