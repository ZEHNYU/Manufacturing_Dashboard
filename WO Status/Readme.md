# 📊 SJ WOs Status – Power BI Report

This report is designed to track the Work Order (WO) status for the San Jose site. It provides a high-level summary and trend analysis of order releases (REL) and technical completions (TECO) by month and week.

![SJ WOs Status Overview](screenshot.png)

---

## 📌 Overview

The **SJ WOs Status** dashboard gives stakeholders a quick view of order movement throughout the year. It is divided into two primary visuals:

1. **WOs Status by Created Month** – Aggregates WOs into monthly bins, broken down by status: `REL` (Released) and `TECO` (Technically Completed).
2. **Weekly Closed Progress** – Shows the count of WOs completed (TECO) each week for real-time operational visibility.

It supports slicing by business unit (QT, RW, MP) using toggle buttons at the top of the report.

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| 📅 Matrix Table | Displays monthly totals of `REL`, `TECO`, and grand total |
| 📊 Clustered Column Chart | Monthly status breakdown (REL vs. TECO) |
| 📈 Line/Bar Chart | Weekly TECO progress to track closure pace |
| 🔘 Business Unit Slicer | Supports dynamic filtering by business line (QT, RW, MP) |
| 🔢 KPI Card | Current number of open work orders |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `DateTable` | Standard calendar reference table |
| `QT`, `RW`, `MP` | WO data from each business line with status and creation/completion dates |

---

## 🛠️ Technical Highlights

- Dynamic DAX measures to calculate status count over time
- Time intelligence functions for YTD and monthly aggregation
- Parameterized navigation with bookmark toggles (for QT/RW/MP tabs)
- Report structured for scalability across multiple business units

---

## 📈 Example Use Cases

- Track backlog of open work orders across months
- Compare REL vs. TECO trends to evaluate team performance
- Identify bottlenecks or delayed completions by week

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `SJ_WOs_Status_04172025.pbix` | Power BI report file |
| `screenshot_SJ_WOs_Status.png` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | DAX function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
