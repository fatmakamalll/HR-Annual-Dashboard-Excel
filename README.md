# 📊 HR Annual Dashboard — Excel Data Analysis Project

> **Week 6 Assignment** | Human Resources Workforce & Salary Analytics Dashboard  
> Built entirely in Microsoft Excel using formulas, pivot tables, named ranges, and dashboard design.

---

## 📌 Project Overview

This project is a complete **HR Analytics Dashboard** built in Excel, designed to analyze employee data across multiple dimensions including salary, department, work type, country, gender, and experience. The workbook contains **300 employee records** and transforms raw HR data into meaningful summaries and visual insights.

The project demonstrates proficiency in:
- Excel data cleaning and standardization
- Formula-driven salary calculations (tax, bonus, net salary)
- Pivot table analysis and summarization
- Named ranges for dynamic referencing
- Dashboard design and KPI reporting

---

## 📁 File Structure

```
fatmaYusfReport2-week6_assignment.xlsx
├── Basic        → Raw employee data + salary calculations
├── Range        → Named ranges applied to the same dataset
├── Pivot        → Pivot table summaries and aggregations
└── Report 2     → Final HR Annual Dashboard (KPIs + visuals)
```

---

## 🗂️ Sheet-by-Sheet Breakdown

### 1️⃣ `Basic` — Employee Master Data & Salary Calculations

This is the **main data sheet** containing all 300 employee records with the following columns:

| Column | Description |
|---|---|
| `ID` | Unique employee identifier (1001–1300) |
| `First Name` / `Last Name` | Employee name (raw, with spacing issues) |
| `Full Name` | Cleaned full name (PROPER function applied) |
| `Gender` | Male / Female |
| `Phone` | Egyptian-format phone numbers |
| `Country` | Egypt, Saudi Arabia, Iraq, Sudan, Syria |
| `Work Type` | Full Time / Contract / Half-Time / Hourly |
| `Department` | Engineering, Marketing, IT, Manufacturing, Sales, Account Management, Quality Control, Product Development, Creative |
| `MonyTransfere` | Payment method: Hawala / Debt Card / Master Card / Western Union |
| `Email` | Format: `firstname.lastname@email.com` |
| `Hire Day / Month / Year` | Date components |
| `Hiring Date` | Full hiring date (assembled from components) |
| `Current Date` | Date of calculation (2026-02-18) |
| `Experience Year` | Calculated years since hire |
| `Salary` | Base salary (range: 742 – 7,478) |
| `Tax 10%` | Tax deduction = Salary × 10% |
| `Bonus 3%` | Bonus addition = Salary × 3% |
| `Net Salary` | Net = Salary − Tax + Bonus |
| `Salary Status` | "Over" if Net ≥ 6,000 / "Normal" if Net < 6,000 |
| `Extra Bonus` | Tiered bonus % based on salary bracket (2% / 5% / 8% / 10%) |

**Side summary table (on the right):**
| Metric | Value |
|---|---|
| Total Net Salary | 1,242,807.36 |
| Average Net Salary | 4,142.69 |
| Count of Employees | 300 |
| Max Salary | 7,478 |
| Min Salary | 742 |

**Extra Bonus Tiers:**
| Salary Range | Bonus % |
|---|---|
| < 1,000 | 10% |
| 1,000 – 2,999 | 8% |
| 3,000 – 5,999 | 5% |
| ≥ 6,000 | 2% |

---

### 2️⃣ `Range` — Named Ranges Version

This sheet is a **duplicate of the Basic sheet** with the same data and calculations, but uses **Excel Named Ranges** to make formulas more readable and maintainable. The structure, columns, and summary statistics are identical to the Basic sheet.

---

### 3️⃣ `Pivot` — Pivot Table Summaries

This sheet contains multiple pivot-style summary tables derived from the employee data:

**Overall KPIs:**
- Total Employees: **300**
- Total Net Salary: **1,242,807.36**
- Average Experience: **19.15 years**

**Employees by Country:**
| Country | Count |
|---|---|
| Egypt | 99 |
| Saudi Arabia | 72 |
| Sudan | 61 |
| Iraq | 53 |
| Syria | 15 |

**Employees by Department × Work Type:**
Breakdown of Contract / Full Time / Half-Time / Hourly headcount across all 9 departments.

**Employees by Gender:**
| Gender | Count |
|---|---|
| Male | 185 |
| Female | 115 |

**Employees by Payment Method:**
| Method | Count |
|---|---|
| Debt Card | 111 |
| Hawala | 92 |
| Western Union | 53 |
| Master Card | 44 |

**Employees by Extra Bonus Tier:**
| Bonus % | Count |
|---|---|
| 5% (3,000–5,999) | 150 |
| 8% (1,000–2,999) | 84 |
| 2% (≥ 6,000) | 52 |
| 10% (< 1,000) | 14 |

**Hiring Trends by Year (1990–2023):**
Year-by-year breakdown showing total IDs and sum of net salaries per hire cohort.

---

### 4️⃣ `Report 2` — HR Annual Dashboard

The final **executive dashboard** sheet displaying:
- **Title:** HR Annual Dashboard
- **Total Salaries:** 1,242,807.36
- **Count of Employees:** 300
- **Average Experience Years:** ~19.15

This sheet serves as the visual summary layer of the workbook, likely containing charts and formatted KPI cards powered by the data in the other sheets.

---

## 📊 Key Insights

- **Egypt dominates the workforce** with 99 employees (33% of total)
- **Males outnumber females** — 185 vs 115 (62% vs 38%)
- **Full Time is the most common** work arrangement
- **Marketing and Engineering** are the largest departments
- **Most employees (50%)** fall in the 5% bonus tier (salary 3,000–5,999)
- **Salary range** is wide: from 742 to 7,478 — avg net ~4,143
- **Average experience** is ~19 years, indicating a senior workforce

---

## 🛠️ Excel Skills Demonstrated

- `PROPER()`, `TRIM()` — name cleaning
- `DATE()`, `DATEDIF()` — date construction and experience calculation
- `IF()`, `IFS()`, `NESTED IF` — salary status and bonus tiers
- `SUM()`, `AVERAGE()`, `COUNT()`, `MAX()`, `MIN()` — aggregation
- `VLOOKUP` / `IFS` — bonus percentage lookup
- **Pivot Tables** — multi-dimensional data summarization
- **Named Ranges** — formula readability
- **Dashboard layout** — KPI cards and visual organization

---

## 📋 Dataset Summary

| Attribute | Details |
|---|---|
| Total Records | 300 employees |
| ID Range | 1001 – 1300 |
| Countries | Egypt, Saudi Arabia, Iraq, Sudan, Syria |
| Departments | 9 departments |
| Work Types | Full Time, Contract, Half-Time, Hourly |
| Salary Range | 742 – 7,478 |
| Hire Year Range | 1990 – 2023 |
| Reference Date | February 18, 2026 |

---

## 👩‍💻 Author

**Fatma Yusuf**  
Week 6 Assignment — Excel Data Analysis & Dashboard Design  
📅 Submitted: 2026

---

## 📄 License

This project is submitted as an academic assignment. Data is synthetic/generated for educational purposes.
