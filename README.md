## 📊 HR Dashboard Overview

An interactive HR analytics dashboard built using **Power BI**, **Python**, and **SQL**, providing insights like:

- 👩‍💼 Total Employees: 50
- 👋 Total Resigned: 8
- 🎂 Average Age: 29.6 years
- 👩 Female Percentage: 46%
- 📈 Resignation Trends (Year-wise)
- 👥 Active vs Resigned Employees
- 📍 Department-level Employee Distribution

> Built with a focus on data clarity and HR decision-making needs.

| Metric               | Value        |
|----------------------|--------------|
| Total Employees      | 50           |
| Resigned Employees   | 8            |
| Average Age          | 29.6 years   |
| Female %             | 46%          |
| Top Department       | Operations   |

## 🛠 Tools
- Power BI for visualization
- SQL for data prep
- Excel as data source

### 🧠 Sample SQL Queries Used

```sql
-- Count Active vs Resigned
SELECT 
  CASE 
    WHEN resignation_date IS NULL THEN 'Active' 
    ELSE 'Resigned' 
  END AS Status,
  COUNT(*) AS Count
FROM employees
GROUP BY Status;


