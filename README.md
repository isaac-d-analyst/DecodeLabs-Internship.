# DecodeLabs Data Analytics Internship
### Isaac Okolie | SkillAhead Solutions Ltd | 2026

---

## 👤 About Me

**Isaac Okolie** — Computer Science Graduate, Data Analyst & Data Analytics Tutor @ **SkillAhead Solutions Ltd** based in Nigeria-
and accredited by the **Institute of Analytics (IoA), United Kingdom.**

This repository documents my complete internship work at DecodeLabs

---

## 🏢 About the Internship

| Property | Detail |
|----------|--------|
| Program | DecodeLabs Data Analytics Internship |
| Powered by | SkillAhead Solutions Ltd |
| Accreditation | Institute of Analytics (IoA), UK |
| Year | 2026 |
| Focus | End-to-end data analytics using real business datasets |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Data cleaning, EDA, pivot tables, charts |
| Power Query (M Language) | Data transformation and shaping |
| MySQL | SQL querying and data analysis |
| Microsoft Power BI | Data visualization and dashboard design |
| DAX | Measures and calculated columns |

---

## 📁 Repository Structure

```
DecodeLabs-Internship/
│
├── README.md
├── DecodeLabs_Internship_Complete_Report.pdf
│
├── Project-1-Data-Cleaning/
│   ├── project_1_cleaned.xlsx
│   ├── CR_DOC.xlsx
│   └── README.md
│
├── Project-2-EDA/
│   ├── project_2_EDA.xlsx
│   └── README.md
│
├── Project-3-SQL-Analysis/
│   ├── project_3_queries.sql
│   ├── project_3_dataset.csv
│   ├── DecodeLabs_Project3_SQL_Report.pdf
│   └── README.md
│
└── Project-4-Data-Visualization/
    ├── project_4_dashboard.pbix
    ├── DecodeLabs_Project4_Visualization_Report.pdf
    ├── screenshots/
    │   ├── page1_revenue_drivers.png
    │   └── page2_revenue_leakage.png
    └── README.md
```

---

## 📊 Dataset Overview

All 4 projects were built on the same e-commerce sales dataset:

| Property | Detail |
|----------|--------|
| Total Orders | 1,200 |
| Total Customers | 1,189 |
| Total Products | 7 |
| Total Revenue | $1,264,762 |
| Analysis Period | 2023 – 2025 |

**Key Fields:**
OrderID, CustomerID, Product, Quantity, UnitPrice, TotalPrice,
PaymentMethod, ReferralSource, CouponCode, OrderStatus, Date

---

## 🔍 Project 1 — Data Integrity & Cleaning Audit

📂 [View Folder](https://github.com/isaac-d-analyst/Task-1-Isaac_Okoile) &nbsp;|&nbsp; 🛠️ Excel & Power Query

**Objective:** Audit and clean the raw dataset before any analysis begins.

**Key Work:**
- Found and resolved 309 missing CouponCode values
- Confirmed OrderID has zero duplicates (1,000 distinct = 1,000 unique)
- Converted Date column from numeric format using Locale settings
- Applied IQR method to detect outliers in UnitPrice and TotalPrice
- Investigated 8 TotalPrice outliers — confirmed valid, retained

**Change Log:**
| Change ID | Description | Impact | Status |
|-----------|-------------|--------|--------|
| CR001 | Replaced 309 null CouponCode values with "No Coupon" | 309 records preserved | Resolved |
| CR002 | Converted Date column from numeric to date format | All rows reformatted | Resolved |
| CR003 | Flagged UnitPrice outliers via IQR — Upper Fence $1,024.83 | 0 outliers detected | Verified |
| CR004 | Investigated 8 TotalPrice outliers — retained as valid | 0 records removed | Resolved |

---

## 📈 Project 2 — Exploratory Data Analysis (EDA)

📂 [View Folder](https://github.com/isaac-d-analyst/Task-2-Isaac_Okoile) &nbsp;|&nbsp; 🛠️ Excel & Power Query

**Objective:** Explore patterns, detect outliers, and measure variable relationships.

**Key Findings:**
| Finding | Value |
|---------|-------|
| Total Revenue | $1,264,762 |
| Average Order Value | $1,053.97 |
| UnitPrice → TotalPrice Correlation | 0.72 (Strong Positive) |
| TotalPrice Outliers | 8 found (all valid — high cart volumes) |
| Combined Cancellation + Return Rate | 41.4% |
| Monthly Revenue Trend | Consistent downward trend since mid-2024 |

**Workbook Sheets:**

| Sheet | Contents |
|-------|---------|
| PROJECT DATA | Clean dataset — 1,200 rows |
| CR DOC | Full change log |
| OUTLIERS FX | IQR calculations for UnitPrice & TotalPrice |
| EDA SUMMARIES | Pivot tables, means, medians, correlations |
| REVENUE CHART | Monthly revenue trend line chart |
| VISUALS | 6 charts covering all key business dimensions |

---

## 🗄️ Project 3 — SQL for Data Analysis

📂 [View Folder](https://github.com/isaac-d-analyst/Task-3-Isaac_Okoile) &nbsp;|&nbsp; 🛠️ MySQL

**Objective:** Extract actionable business insights using structured SQL queries.

**18 Queries Across 6 Categories:**

| Category | Queries | Key Result |
|----------|---------|-----------|
| Data Inspection | 1–3 | 1,200 records confirmed |
| Data Cleaning | 4–5 | 309 CouponCode nulls resolved |
| Revenue Analysis | 6–7 | $1,264,738 total revenue |
| Customer & Product | 8–10 | 1,189 unique customers |
| Fulfillment Analysis | 11–15 | $519,658 total revenue at risk |
| Behavior & Trends | 16–18 | Channel and trend patterns identified |

**Key Financial Results:**
| Metric | Value |
|--------|-------|
| Total Revenue | $1,264,738 |
| Average Order Value | $1,053.95 |
| Revenue Lost to Returns | $243,268 |
| Revenue Lost to Cancellations | $276,390 |
| Combined Revenue at Risk | $519,658 |

---

## 📊 Project 4 — Data Visualization & Storytelling

📂 [View Folder](https://github.com/isaac-d-analyst/Task-4-Isaac_Okoile) &nbsp;|&nbsp; 🛠️ Power BI

**Objective:** Build a 2-page Power BI dashboard communicating revenue insights clearly.

**Design Principles:**
- One Page, One Message
- Reduce Visual Clutter
- Tell a Story

**Dashboard Pages:**

| Page | Business Question | Key Finding |
|------|-----------------|------------|
| Page 1 — Revenue Drivers | What is driving revenue? | Instagram leads at $275,285 |
| Page 2 — Revenue Leakage | How much is being lost? | $519,674 lost to cancellations & returns |

**Revenue by Referral Source:**
| Source | Revenue |
|--------|---------|
| Instagram | $275,285 |
| Email | $261,809 |
| Google | $250,441 |
| Facebook | $250,411 |
| Referral | $226,816 |

---

## 💡 Key Business Insights Across All Projects

1. Total revenue of **$1,264,762** generated across 2023–2025
2. **Instagram** is the top-performing acquisition channel at **$275,285**
3. **Chair, Printer, and Laptop** are the top 3 revenue-generating products
4. **41.4%** of all orders cancelled or returned — the biggest operational challenge
5. Over **$519,000** in revenue was lost and is potentially recoverable
6. Revenue shows a **consistent downward trend** since mid-2024
7. UnitPrice is the strongest driver of TotalPrice (**r = 0.72**)
8. All 5 payment methods are near-equally distributed
9. 309 missing CouponCode records were resolved without any data loss
10. TotalPrice outliers were valid high-volume orders — not errors

---

## ✅ Skills Demonstrated

| Skill | Evidence |
|-------|---------|
| Data Cleaning & Auditing | Resolved 309 missing values; IQR outlier detection |
| Exploratory Data Analysis | Stats, distribution, and correlation analysis |
| SQL & Database Management | 18 queries across 6 categories in MySQL |
| Data Visualization | 7 Excel charts + 2-page Power BI dashboard |
| Business Communication | 4 formal reports with insights and recommendations |
| Documentation | Change logs, README files, reports for all 4 projects |
| Storytelling with Data | Every visual designed to answer a business question |

---

## 📬 Connect With Me

**Isaac Okolie**
Data Analyst & Data Analytics Tutor | Nigeria

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://linkedin.com/ebube-isaac-okolie)
---

*DecodeLabs Internship | SkillAhead Solutions Ltd | Accredited by Institute of Analytics, UK*
