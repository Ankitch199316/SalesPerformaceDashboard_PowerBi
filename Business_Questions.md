# Business Questions — Sales Performance Dashboard

This dashboard focuses on analyzing category and regional sales performance across time.

---

## 1️⃣ Sales Performance

### Q1: What is total sales?

**Measure Used:**

* `Total_Sales`

---

### Q2: What are current year sales (YTD)?

**Measure Used:**

* `Current_year_sales`

---

### Q3: How did sales perform compared to last year?

**Measures Used:**

* `Previous_year_sales`
* `Sales_growth`

---

### Q4: What is the growth percentage?

**Measure Used:**

* `Sales_growth`

---

## 2️⃣ Category Analysis

### Q5: Which product category drives the most revenue?

**Logic Used:**

* `Total_Sales` grouped by Category
* `Category_Switch` for visual mapping

---

### Q6: How do categories perform month-over-month?

**Logic Used:**

* Line chart grouped by Category
* Aggregation using SUM(Orders[Sales])

---

## 3️⃣ Regional Analysis

### Q7: Which region generates highest sales?

**Logic Used:**

* SUM(Orders[Sales]) grouped by Region

---

### Q8: How does sales vary across regions?

**Logic Used:**

* Stacked column visual by Region

---

## 4️⃣ Dashboard Metadata

### Q9: When was the dataset last refreshed?

**Measure Used:**

* `Getdate`

---

