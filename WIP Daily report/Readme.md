# 📊 WIP Daily Report – Power BI Report

This report provides daily visibility into aging work orders and unfinished serial numbers. It enables production and engineering teams to monitor delayed WIP, aging trends, and SN-level blocking issues across stations.

![WIP Daily Report Screenshot](screenshot_WIP_Daily.png)

---

## 📌 Overview

The **WIP Daily Report** is used to detect overdue WIP across the shop floor and highlight serial numbers that have not yet completed their process. It contains two key sections:

1. **WO Aging Table** – Displays open work orders with their calculated aging, quantity breakdowns, and last station timestamp.
2. **SN Haven't Finished** – Lists unfinished SNs with their last known station or "Not put into production" status.

This page is highly filterable by:
- Year / Month
- MO Number
- WIP Aging Range (e.g., >120, >90, >60)

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| 📘 Aging Column | Dynamically calculated using DAX between create date and today |
| 📊 Balance Calculation | Derived from `TARGET - SHIPPING - NPT_OUT` |
| 🧮 WIP Range Buckets | Categorized by >120, >90, >60 days aging |
| 🔎 SN Drill Table | Displays SNs with incomplete routes or no entry into production |
| 🗂️ Multiple Slicers | Allows MO number and aging filters for faster debugging |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `R_MO_BASE_T` | Base WO data including target quantity, dates, and PB mapping |
| `R_WIP_TRACKING_T` | WIP movement tracking and quantity summary |
| Calculated Columns | DAX measures for `Aging`, `Balance`, `WIP Bucket` |

---

## 🛠️ Technical Highlights

- Aging logic using `DATEDIFF(TODAY(), CREATE_DATE, DAY)`
- Multi-level WIP range grouping with transparent SN validation
- Real-time WIP balance updates based on shipping/NPT output
- Visibility into bottlenecked SNs and production hold issues

---

## 📈 Example Use Cases

- Prioritize aging WOs stuck in production
- Detect units that never entered the line despite issued orders
- Trigger escalation or re-planning based on WIP bottlenecks

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `WIP_Daily_Report_05142025.pbix` | Power BI report file |
| `screenshot_WIP_Daily.png` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | DAX function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
