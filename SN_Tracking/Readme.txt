# 📊 SN Tracking – Power BI Report

This report enables detailed tracking of individual Serial Numbers (SNs) through the production process. It highlights their current station, process duration, error status, and history of failed units, helping manufacturing and engineering teams manage exceptions and flow efficiency.

![SN Tracking Screenshot](screenshot_SN_Tracking.png)

---

## 📌 Overview

The **SN Tracking** dashboard allows users to trace each SN from the first process step through to its current location. It includes filtering by PB_NO and SN, and identifies failed units that are currently offline or stuck in specific stations.

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| ⏱️ Day Duration | Displays total days SNs have remained active in production |
| 🏁 Latest Station | Shows where the most recent activity occurred |
| 🕒 Time Range | Highlights earliest and latest IN_STATION_TIME |
| 📋 SN Table | Lists real-time SN status, including station and timestamp |
| ⚠️ Off-line SN Table | Displays SNs that are in ERROR state or dropped out of flow |
| 📊 Pie Chart | Visual breakdown of `PASS` vs `ERROR` statuses across all SNs |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `R_SN_DETAIL_T` | Serial-level process record with timestamps and stations |
| `R_WIP_TRACKING_T` | Live WIP snapshot with current station and balance |
| DAX Measures | Duration, error classification, latest station logic |

---

## 🛠️ Technical Highlights

- Tracks **real-time WIP movement** and **error rates** at SN level
- Filters allow PB_NO and SN focus with high interactivity
- Custom DAX to compute `Day Duration` between first and last scan
- Off-line table isolates all SNs marked with `Error_Status = ERROR`

---

## 📈 Example Use Cases

- Diagnose units stuck in test, repair, or final assembly stations
- Identify trend of failures at specific SFC stations
- Audit units with abnormal time gaps or missing process scans

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `SN_Tracking_07242025.pbix` | Power BI report file |
| `screenshot_SN_Tracking.png` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | DAX function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
