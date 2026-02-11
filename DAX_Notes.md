# DAX Notes — Sales Performance Dashboard

This dashboard focuses on category-level and regional sales performance analysis using time-based comparisons.

---

## 1️⃣ Base Aggregation Measures

### Total Sales

```DAX
Total_Sales =
CALCULATE(SUM(Orders[Sales]))
```

Calculates overall sales revenue.

---

## 2️⃣ Time Intelligence Measures

### Current Year Sales (YTD)

```DAX
Current_year_sales =
CALCULATE(
    SUM(Orders[Sales]),
    DATESYTD(Orders[Order Date])
)
```

Calculates Year-To-Date sales dynamically.

---

### Previous Year Sales

```DAX
Previous_year_sales =
CALCULATE(
    SUM(Orders[Sales]),
    YEAR(Orders[Order Date]) = 2021
)
```

Calculates sales for the previous year (static comparison baseline).

---

### Sales Growth %

```DAX
Sales_growth =
DIVIDE(
    ([Current_year_sales] - [Previous_year_sales]),
    [Previous_year_sales]
)
```

Calculates year-over-year growth percentage.

---

## 3️⃣ Category Logic

### Category Switch (Dynamic Labeling)

```DAX
Category_Switch =
VAR cate = SELECTEDVALUE(Orders[Category])
VAR _type =
    SWITCH(
        TRUE(),
        cate = "Office Supplies", "Digital Watch",
        cate = "Furniture", "Analog Watch",
        cate = "Technology", "Other"
    )
RETURN _type
```

Maps product categories to display types for visual customization.

---

## 4️⃣ UI / Display Measures

### Growth Card Label

```DAX
Growth_Card = "Growth By Year"
```

Static text used for KPI card title.

---

### Get Last Refresh Date

```DAX
Getdate =
VALUES('Last Rfresh Date'[Last Refresh Date])
```

Displays dataset refresh timestamp.

---

### Color Gradient Control

```DAX
colorGradient = 60
```

Used for conditional formatting in visuals.

---
