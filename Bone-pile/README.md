# 📊 Bone-pile – Power BI Report

This report provides visibility into serial numbers (SNs) that are stuck or delayed in production. It focuses on identifying bottlenecks by station and SFC group through duration analysis and SN count aggregation.

![Bone-pile Screenshot](screenshot_Bonepile.png)

---

## 📌 Overview

The **Bone-pile** dashboard tracks units that have been idle in specific stations for extended periods. It is designed to help engineers and planners identify:
- High-concentration stations
- Average aging by station
- Serial numbers that require intervention or escalation

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| 📊 Combo Chart | Displays SN count and average duration by station |
| 📋 SN Table | Detailed view of delayed serial numbers including station, time, and duration |
| 📈 KPIs | Total count of SNs and average delay duration |
| 🎯 Filters | Multi-select by SFC Group and PB_NO for targeted analysis |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `r_wip_tracking_t` | Contains in-station timestamps and station metadata |
| DAX Measures | Includes average duration and filtered SN count per station |

---

## 🛠️ Technical Highlights

- Tracks production stagnation points using `IN_STATION_TIME` and `Duration`
- Combines bar and line charts for visual correlation
- Highlights process inefficiencies and WIP accumulation risks
- Filters allow drilling into specific SFC groups or products

---

## 📈 Example Use Cases

- Detect bottlenecks in assembly, test, or repair stations
- Prioritize units with excessive idle time for resolution
- Compare WIP delay trends across departments or shifts

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `Bonepile_04032025.pbix` | Power BI report file |
| `screenshot_Bonepile.png` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | DAX function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
