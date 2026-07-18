# HR-Workforce-Analytics-Dashboard
# 📊 HR Workforce Analytics Dashboard

An interactive Excel dashboard analyzing employee attrition, satisfaction, and compensation trends across an organization of **1,470 employees**. Built entirely in Excel using PivotTables, PivotCharts, and dynamic KPI cards — no external BI tool required.

![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Dashboard](https://img.shields.io/badge/Type-Data%20Analytics%20Dashboard-blue)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📌 Overview

This project transforms a raw HR dataset into a decision-ready dashboard for HR and business leaders. It answers key workforce questions:

- Where is attrition concentrated (department, age, gender, marital status)?
- Does overtime correlate with employees leaving?
- How does compensation vary by job role?
- How satisfied and balanced (work/life) are employees across departments?

The workbook is structured as a mini data pipeline: **Raw Data → KPI Calculations → Pivot Tables → Visual Dashboard**.

---

## 🗂️ Workbook Structure

| Sheet | Purpose |
|---|---|
| **Raw Data** | 1,470 employee records, 38 columns (demographics, compensation, satisfaction, tenure, and engineered fields like `Age_Group`, `Income_Group`, `Attrition_Flag`) |
| **KPI** | Core headline metrics calculated with formulas referencing the raw dataset |
| **Pivot_Table** | 10 PivotTables breaking down attrition and compensation by different dimensions |
| **Dashboard** | Visual summary combining KPI cards with 6 charts (bar, column, and doughnut) sourced from the pivot data |

---

## 📈 Key Metrics (KPI Cards)

| Metric | Value |
|---|---|
| Total Employees | 1,470 |
| Attrition Count | 237 |
| Attrition Rate | 16.1% |
| Average Monthly Salary | ~$6,503 |
| Average Job Satisfaction | 2.7 / 4 |
| Average Work-Life Balance | 2.76 / 4 |

---

## 📊 Dashboard Visuals

1. **Attrition by Department** — Bar chart (R&D has the highest raw attrition count, driven by headcount size)
2. **Attrition by Gender** — Doughnut chart
3. **Attrition by Age Group** — Bar chart (26–35 age group has the highest attrition)
4. **Attrition by Overtime** — Column chart (employees working overtime show a notably higher share of attrition)
5. **Avg Salary by Job Role** — Bar chart (Managers and Research Directors earn the most; Sales Representatives the least)
6. **Employee Count by Department** — Doughnut chart (R&D is the largest department by headcount)

---

## 🔍 PivotTable Breakdown

The `Pivot_Table` sheet includes 10 tables covering:

1. Attrition by Department
2. Attrition by Gender
3. Attrition by Age Group
4. Attrition by Overtime
5. Average Salary by Job Role
6. Employee Count by Department
7. Attrition by Marital Status
8. Attrition by Education Field
9. Job Satisfaction by Department
10. Work-Life Balance by Department

---

## 💡 Notable Insights

- **Overtime is a strong attrition signal**: employees working overtime attrite at a disproportionately higher rate relative to their share of headcount.
- **Single employees** show the highest attrition count among marital status groups, followed by married and divorced employees.
- **Younger employees (18–35)** account for the majority of attrition — over two-thirds of all departures.
- **Compensation follows a clear hierarchy**: leadership/director-level roles (Manager, Research Director) earn 2–5x more than entry-level technical/sales roles.
- **Job satisfaction and work-life balance are fairly consistent across departments** (~2.6–2.9 out of 4), suggesting attrition is driven more by role, tenure, and overtime than department-level culture differences.

---

## 🛠️ Tech / Tools Used

- Microsoft Excel (PivotTables, PivotCharts, formulas)
- Dataset: IBM HR Analytics Employee Attrition dataset (1,470 records, 35 original attributes + 3 engineered fields)

---

## 🚀 How to Use

1. Download `HR_Workforce_Dashboard.xlsx`
2. Open in Excel (charts and pivots are fully interactive — click into any PivotTable to filter/drill down)
3. Use the `Dashboard` sheet for an at-a-glance executive view
4. Explore `Raw Data` for the underlying records

---

## 📬 Future Improvements

- Add slicers for interactive filtering directly on the Dashboard
- Build a Power BI / Tableau version for web-based interactivity
- Add predictive attrition scoring using logistic regression in Python
