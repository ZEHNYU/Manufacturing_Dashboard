# 📊 WIP History – Power BI Report

This report provides detailed visibility into the historical work-in-progress (WIP) records and repair data across manufacturing process stations. It includes interactive filtering and a **drill-through-enabled** layout for tracking unit-level movements and rework actions.

![WIP History Screenshot](screenshot_WIP_History.png)

---

## 📌 Overview

The **WIP History** dashboard helps users analyze current and historical WIP by PB_NO, WO, BOM, and SFC station. It is designed to support high-volume assembly and diagnostic workflows.

It consists of two key pages:

1. **WIP History** – A summary view showing target quantity, shipping/NPI output, and repair activity by station.
2. **WIP Detail** – A drill-through page that shows unit-level travel logs with entry timestamps per station.

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| 🔘 Button Navigation | Switch between "WIP History" and "WIP Detail" views |
| 🔄 Drill-Through | From WIP summary to SN-level station time tracking |
| 📊 KPI Cards | Display target quantity, shipping output, NPI out |
| 📋 Data Tables | Show PB/WO-level WIP records and repair summaries |
| 📈 Timeline Gantt | Visual timeline of in-station timestamps for each SN |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `R_SN_DETAIL_T` | Full SN movement history by station |
| `R_REPAIR_T` | Repair logs with station, action code, and result |
| `C_ROUTE_CONTROL_T` | Process route control and expected step sequence |
| `BridgeTable_2` | Bridge table for filtering and drill-through connections |

---

## 🛠️ Technical Highlights

- **Drill-through enabled** for tracing each unit’s process flow
- Timeline chart showing in-station duration with visual range
- Rich filtering by PB_NO, BOM, WO, and station
- Dynamic aggregation of SN counts per rework/station/step

---

## 📈 Example Use Cases

- Investigate WIP accumulation at specific stations
- Analyze rework patterns and reasons across product batches
- Identify delays in production flow using in-station timestamps

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `WIP_History_07242025.pbix` | Power BI report file |
| `screenshot_WIP_History.png` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | DAX function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
