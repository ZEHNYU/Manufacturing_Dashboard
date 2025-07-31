# 🏭 Manufacturing Dashboard ｜ Power BI Portfolio

This repository showcases a collection of real-world Power BI reports designed to optimize **factory production tracking**, **work-in-progress (WIP) visibility**, and **planning readiness**.

These dashboards were built to support day-to-day operations across the shop floor, from build scheduling to SN-level traceability and shipping analysis.

---

## 📦 Included Reports & Use Cases

| Module | Description | Typical Usage |
|--------|-------------|----------------|
| **Planning Build** | Calendar-based PB tracking and material readiness overview | For PMs and planners to coordinate build schedules and manage shortages |
| **WO Status** | Monthly & weekly WO release/closure trends | For executives and planners to evaluate backlog and release pacing |
| **WIP Tracking** | Real-time WIP by station with filterable views | For floor managers to monitor production flow |
| **WIP History** | Historical WIP and repair record with drill-through | For QA and engineering to trace issues and repair cycles |
| **WIP Daily report** | WO aging and unstarted SN status | For exception management and delayed order follow-up |
| **SN_Tracking** | Serial-level process tracking with error flagging | For debugging SN issues and validating completion flow |
| **Shipping** | Outbound SN status and shipment tracking | For logistics to confirm outbound accuracy |
| **Bone-pile** | Bottleneck analysis by station and duration aging | For engineering to identify where SNs get stuck and for how long |

---

## 💡 Key Features

- ✅ **Drill-through** from summary to SN-level details
- 📅 Calendar layout with dynamic Build Status tags
- 📊 SN aging, delay, and process time distribution analysis
- 🚚 Outbound vs. unshipped SN verification
- ⚠️ Material shortage visualization with ColorCode logic (G/Y/R/Pending/Consign)
- 🔄 Real-time WIP snapshots with DAX-driven filtering

---

## 🛠️ Technologies Used

- **Power BI Desktop**
- DAX (for time intelligence, filters, KPIs)
- Oracle/ SQL Server/OneLake/Dataverse as data sources
- Power BI Service (for report deployment)
- GitHub (for version control and portfolio showcase)

---

## 👨‍💼 Author

> Created by Allen Wu ｜ allen0307ai@gmail.com  
> Focused on manufacturing analytics, cost control, and automation with Power BI

---

## 📁 Folder Structure

Each folder contains:

- `*.pbix` – Power BI report file  
- `screenshot_().png` – Report UI image  
- `README.md` – Module-level description  
- `Dax code` – DAX logic or KPIs (optional)  
- `Sample data` – Simulated or masked data (optional)

---

## 📍 When to Use These Reports?

These dashboards were created and used in real factory environments, best suited for:

- NPI or pilot line build tracking
- High-mix, low-volume manufacturing
- Daily WIP/Shipping/Repair/Shortage sync meetings
- Exception-based SN tracing
- Factory floor efficiency improvements

---

> For collaboration or discussion, reach out via email.
