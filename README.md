# 📊 Sales Performance Dashboard – Power BI

## 📌 Project Overview

This project presents a Sales Performance Dashboard built using the Sample Superstore dataset.

The dashboard analyzes category-level and regional sales trends, year-over-year growth, and monthly performance using DAX time intelligence functions.

It is designed to provide quick visibility into revenue performance and growth trends across product categories and regions.

---

## 🎯 Business Objectives

The dashboard answers the following key questions:

* What is total sales revenue?
* How is current year sales performing (YTD)?
* What is the year-over-year growth rate?
* Which product category generates the highest revenue?
* How do categories perform month-over-month?
* Which region drives the most sales?
* When was the dataset last refreshed?

Detailed breakdown available in:
➡ `Business_Questions.md`

---

### Dashboard Screenshot
<img width="1003" height="562" alt="Screenshot 2026-02-11 at 11 29 20 AM" src="https://github.com/user-attachments/assets/d6a95c71-e19f-4b2e-bd58-2ebeaafd48fd" />


---

## 📊 Key KPIs Implemented

* Total Sales
* Current Year Sales (YTD)
* Previous Year Sales
* Sales Growth %
* Category-Level Sales
* Regional Sales Comparison
* Last Refresh Date

---

## 🧠 DAX Measures Used

This dashboard uses custom DAX measures including:

* YTD calculations using `DATESYTD`
* Year-over-Year growth calculation
* Category-based switching logic
* Conditional formatting controls
* Static and dynamic KPI card measures

Full DAX documentation available in:
➡ `DAX_Notes.md`

---

## 🏗 Data Model

The model uses a simplified structure:

* **Orders** (Fact Table)
* **Last Refresh Date** (Supporting Table)

The Orders table contains transaction-level data including:

* Order Date
* Category
* Region
* Sales

Time intelligence is implemented directly on the Order Date column.

Model documentation available in:
➡ `Data_Model.md`

---

## 🛠 Tools & Techniques

* Power BI Desktop
* DAX Time Intelligence
* Year-over-Year Growth Analysis
* Category and Region Segmentation
* KPI Card Design
* Conditional Formatting

---

## 📁 Repository Structure

```
Sales-Performance-Dashboard/
│
├── README.md
├── DAX_Notes.md
├── Business_Questions.md
├── Data_Model.md
├── Screenshots/
└── Data/
```

---

## 🚀 Project Positioning

This project demonstrates:

* Sales trend analysis
* Time-based KPI modeling
* Revenue growth calculation
* Category segmentation analysis
* Clean dashboard design with strong visual hierarchy

It highlights core Power BI capabilities in building structured sales reporting dashboards.

---
