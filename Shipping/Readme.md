# 📊 Shipped Tracking – Power BI Report

This report monitors the shipment status of serial numbers (SNs) across the production floor. It allows users to track total shipment progress, identify unshipped SNs, and filter by BOM, PB_NO, and production tags.

![Shipped Tracking Screenshot](screenshot_Shipped_Tracking.png)

---

## 📌 Overview

The **Shipped Tracking** dashboard provides near real-time tracking of outgoing shipments and pending units. The key KPIs include:

- **Target Quantity** – Planned output quantity
- **Shipped SN** – Actual serials sent to shipping
- **Balance** – Units that remain unshipped

It also contains a breakdown of:
- SNs already shipped (with DN/SHIPNO info)
- SNs that haven’t shipped (with last scanned station & time)

---

## 🧩 Key Report Features

| Component | Description |
|----------|-------------|
| 📈 KPI Cards | Target vs. actual shipped quantity with balance |
| 🗂️ BOM & PB_NO Filters | Multi-select slicers for product-level review |
| 📋 Shipped SN Table | Full log of shipped SNs with DN and Ship No. |
| 🚫 Unshipped SN Table | Shows SNs still stuck in production or packing |
| 📅 Date Range Slicer | Filter report scope by in-station date |

---

## 🗂️ Data Tables

| Table Name | Description |
|------------|-------------|
| `R_DATAFEED_SENDING_T` | Shipment feed table with SNs and shipping metadata |
| `R_WIP_TRACKING_T` | Remaining WIP not yet shipped |
| DAX Measures | Custom logic for balance, filters, and dynamic totals |

---

## 🛠️ Technical Highlights

- Tracks SN movement across shipping lifecycle with DN/SHIPNO
- Highlights SNs that passed through all process steps but not shipped
- Dynamic filtering using MP Tag, PB_NO, BOM, and date
- Supports proactive backlog detection for shipping team

---

## 📈 Example Use Cases

- Monitor shipping progress vs. production goals
- Identify bottleneck SNs awaiting shipment
- Drill into unshipped units by BOM, station, or work order

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `Shipping_07242025.pbix` | Power BI report file |
| `screenshot_Shipped_Tracking.png` | Report UI screenshot |
| `README.md` | This documentation file |
| `Dax code` | DAX function |
| `Sample data` | Sample data |

---

> Created by Allen Wu ｜ allen0307ai@gmail.com
