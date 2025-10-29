# 🚗 Demand Planning Simulation
**Impact Analysis of Fremont Production Disruption on Lead Time, Cost & Customer Fulfillment**

---

## 🔍 Project Overview

This project simulates how global electric vehicle production is allocated across three U.S. demand regions — **East Coast (EC), Central (CC), West Coast (WC)** — under two operational scenarios:

| Scenario | Description |
|---------|-------------|
| ✅ Baseline | All plants produce normally |
| ⚠️ Fremont Incident | Fremont capacity reduced by **20%** |

The objective is to understand how a **critical plant disruption** affects:
 
✅ Logistics lead-times  
✅ Cost to serve  
✅ Regional supply alignment  
✅ Vulnerable product-mix segments

---

## 🎯 Key Business Questions

1️⃣ How does production loss at Fremont impact customers?  
2️⃣ What cost penalties emerge from rerouting production overseas?  
3️⃣ Which model-trim-color combinations are most at risk?  
4️⃣ How are we allocating products to customers? 

---

## 🧠 Methodology

| Stage | What We Built |
|------|---------------|
| Data Simulation | 93 days of plant-level production across multiple SKUs |
| Demand Modeling | Weekly customer preference by model × trim × color |
| Transit Mapping | Shipping lead time + cost by lane |
| Allocation Engine | Greedy nearest-first allocator to minimize delays |
| Scenario Outputs | Allocation, backlog, and KPI comparison |
| Analytics Dashboard | Visuals in Excel |

📌 Core logic: Vehicles are allocated from the **nearest plant with available supply**  

---

### 🛠 Tools & Technologies

| Category | Tools Used | Purpose |
|---------|------------|--------|
| Programming & Scripting | Python (Pandas, NumPy) | Data simulation, allocation engine, scenario modeling |
| Data Visualization | Excel (PivotCharts, Conditional Formatting), Tableau-ready outputs | Dashboard design & insights |
| Data Engineering | CSV structured datasets, transformation workflows | Connecting production → demand → allocation |
| Modeling Techniques | Greedy nearest-first allocator, SKU-level aggregation | Minimize lead time & shipping cost while serving demand |
| Database | SQL Database Creation | Storing all simulated data in one place |



---

## 🗺 Dashboard Snapshot

<img width="927" height="596" alt="Dashboard_Snapshot" src="https://github.com/user-attachments/assets/515f90de-8b84-465f-9e40-3075833dd36d" />

[Dashboard.xlsx](https://github.com/user-attachments/files/23215218/Dashboard.xlsx)


---

## 📁 Repository Structure

    .
    ├── notebooks
    │   ├── 01_synthetic_data2.ipynb
    │   └── 02_Allocator2.ipynb
    │ 
    ├── data
    │   └── colors.csv
    │   └── models.csv
    │   └── trims.csv
    │   └── transit_time.csv
    │   └── regional_demand.csv
    │   └── vehicle_production.csv
    │   └── regions.csv
    │   └── plants.csv
    │ 
    ├── result
    │   └── allocation_result2.csv
    │ 
    ├── dashboard
    │   └── Dashboard.xlsx
    │   └── Dashboard_Snapshot.png
    │ 
    ├── README.md

---
