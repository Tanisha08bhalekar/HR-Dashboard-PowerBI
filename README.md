# 📊 HR Analytics Dashboard

Hey everyone! 👋

A lot of you have been curious about HR dashboards — so here’s mine!  
I used **Power BI**, **Python**, and some **SQL** to turn raw HR data into something clear, visual, and insightful. Whether you’re in HR or data, I hope this gives a quick view into the kind of analysis that supports people-first decisions.

---

## 🔍 Dashboard Summary

| Metric                | Value        |
|------------------------|--------------|
| 👥 Total Employees      | 50           |
| 👋 Resigned Employees   | 8            |
| 🎂 Average Age          | 29.6 years   |
| 👩 Female Percentage     | 46%          |
| 🏢 Most Common Division  | Operations   |

---

## 💡 What This Dashboard Shows

- ✅ Key KPIs in one glance (Total employees, attrition, gender balance)
- 📉 Resignation trends over time
- 👩‍💼 Gender distribution and diversity breakdown
- 📊 Age distribution across workforce
- 🏢 Department-wise headcount summary
- 📌 Designed to fit **carousel layout** for LinkedIn or presentations

---

### 🛠️ Tools & Features

- Power BI: DAX formulas, KPI cards, slicers, clustered column charts
- Python: Data wrangling, cleaning
- SQL: Aggregations, filtering, grouping
- Storytelling: Carousel-ready layout, professional color palette


---

## 🧠 Sample SQL Queries Used

```sql
-- Total Active vs Resigned
SELECT 
  CASE 
    WHEN resignation_date IS NULL THEN 'Active' 
    ELSE 'Resigned' 
  END AS Status,
  COUNT(*) AS Count
FROM employees
GROUP BY Status;

-- Average Age
SELECT AVG(age) AS AvgAge FROM employees;

-- Gender Ratio
SELECT gender, COUNT(*) AS Count
FROM employees
GROUP BY gender;

---

### 💬 Always learning — open to feedback!
If you have ideas or want to collaborate, feel free to reach out.


