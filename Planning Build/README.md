# 📊 Planning Build – Power BI Report

This report provides a centralized view of product build readiness, integrating calendar-based build scheduling, material shortage analysis, and project milestone tracking for various PB (Product Build) IDs.

![Planning Build Screenshot](screenshot_Planning_Build.png)

---

## 📌 Overview

The **Planning Build** dashboard is designed for program managers and planners to manage build schedules and material readiness for prototype and pilot builds. It consists of two fully implemented pages:

1. **PBR Build Info** – A calendar-based build planning view with filters and status breakdowns.
2. **Planning PBR Info** – A shortage tracking interface showing SMT/Mechanical shortfall per PB_NO and associated color code risks.

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| 📅 Calendar View | Monthly/Weekly/Daily layout showing PB_ID per build date |
| 📋 Build Table | PB-level info including Project ID, RSD, QTPM, Planner |
| 🧮 Shortage Breakdown | Real-time SMT and Mechanical shortage by type |
| 🟡 ColorCode Analysis | Visual alert using `G / Y / R / Pending Review / Consign` categories |
| 🔍 Filters | Interactive controls by Build Status, PB_NO, and material type |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `PBR Build Information` | Master PB-level metadata: Project ID, RSD, Planner, Status |
| `ShortageInfo` | Material shortage data including PartNo and ColorCode flags |
| DAX Measures | Computed shortage counts, build status summaries, filters by status/date |

---

## 🛠️ Technical Highlights

- Integrated **calendar UI** built using custom matrix with dynamic formatting
- Color-coded shortfall visualization across SMT & Mechanical groups
- Flexible filtering by planner, project, date, and PB status
- Easy drill path to view builds affected by `can't match RSD` or missing CTB

---

## 📈 Example Use Cases

- Identify PBs lacking sufficient SMT or mechanical parts before RSD
- Filter quick-turn builds awaiting approval
- Cross-check planner ownership and build timeline in a single view

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `Planning_Build_07282025.pbix` | Power BI report file |
| `screenshot_Planning_Build.png` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | DAX function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
