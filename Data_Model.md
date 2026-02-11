# Data Model — Sales Dashboard

## Model Structure

This dashboard uses a simplified model with:

* 1 Fact Table (Orders)
* 1 Supporting Table (Last Refresh Date)

---

## Fact Table: Orders

Contains transactional sales records.

Key Columns:

* Order Date
* Category
* Region
* Sales

Used to calculate:

* Revenue
* Growth
* Category performance
* Regional performance

---

## Supporting Table

### Last Refresh Date

Used to dynamically show dataset refresh timestamp.

---

## Modeling Approach

* Single-table aggregation model
* Time intelligence via DATESYTD
* Static previous year comparison
* Category-based filtering logic
* Conditional formatting controls


