# 📊 WIP Tracking – Power BI Report

This report is part of the **Manufacturing Dashboard**, specifically designed to monitor the real-time status of **Work Orders (WO)** across different process stations. It provides visibility into where each unit currently is, how many are in each station, and the distribution across shifts.

![WIP Tracking Overview](screenshot.png)

---

## 📌 Overview

In high-mix, high-volume manufacturing environments like semiconductor and electronics assembly, having visibility into WIP (Work-In-Progress) is essential. This Power BI report enables teams to:

- View SN (Serial Number) count by WO, station, and shift
- Monitor daily/weekly/monthly WIP trends
- Filter by product number (PB_NO), BOM, WO, or station
- Identify bottlenecks or abnormal work-in-process flow

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| 📅 Date Picker | Filter by Day, Week, Month, or custom range |
| 🔍 Multi-layer Filters | Select PB_NO, WO, SFC Station, and BOM |
| 📋 Data Table | Display current WIP count grouped by WO and Station |
| 🏷️ Shift Label | Automatically classifies Day and Swing shifts |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `R_WIP_TRACKING_T` | Main dataset including WO, SFC station, SN count, and shift |
| `C_ROUTE_CONTROL_T` | Reference table for SFC process route and station definitions |

---

## 🛠️ Technical Highlights

- **Hybrid storage mode** for faster performance and scalable deployment
- DAX-driven time filtering and aggregation
- Drill-through-ready layout for future enhancements
- Built-in support for identifying shift-based trends and anomalies

---

## 📈 Example Use Cases

- Compare WIP levels across day and night shifts
- Identify work order build-up at specific stations
- Final-stage WIP validation before outbound shipping

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `WIP_Tracking_07242025.pbix` | Power BI report file |
| `screenshot_()` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | Dax function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
