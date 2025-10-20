---
layout: posts
title: "Power BI — AdventureWorks Sales & Product Report"
date: 2025-10-20 02:55:00 +0200
tags: [Power BI]
author_profile: true
author: Ahmed Almahey
categories: [work]
header:
  overlay_image: "/assets/images/Screenshot 2025-10-20 064701.png"
  teaser: "/assets/images/Screenshot 2025-10-20 064701.png"
description: "End-to-end Power BI report built on the AdventureWorks dataset — analyzing sales performance, product hierarchies, and order efficiency using DAX and interactive visuals."
---

**Power BI — AdventureWorks Sales & Product Report**

AdventureWorks is one of Microsoft’s classic sample datasets, and it represents a full retail sales operation.  
I built this project to simulate a **real business intelligence workflow** — connecting data from multiple sources, modeling it efficiently, and designing an interactive report that helps managers track **sales performance, delivery efficiency, and profitability**.

---

###  Data Source & Preparation

- **Data Source:** [AdventureWorks Sample Database](https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms)  
- **Connectivity Mode:** Import  
- Extracted data from key views:  
  - `vw_DimProducts`, `vw_DimSalesPersons`, `vw_DimShipMethods`, `vw_DimStatuses`, `vw_DimTerritories`, `vw_FactOrderDetails`  
- Built **DimDates (DAX table)** with Year, Month, Day, Month Name, and Day Name for flexible time analysis  
- Cleaned and validated relationships to ensure reliable aggregations  

---

###  Data Modeling

The report uses a **Star Schema**, designed for high-performance analysis:  
- Fact table: `vw_FactOrderDetails`  
- Dimension tables: Products, Territories, Ship Methods, Statuses, Dates  
- Created **Product** and **Date hierarchies** for intuitive drill-down  
- Implemented **role-playing dimensions** using `USERELATIONSHIP()` to analyze metrics by Order Date, Ship Date, and Due Date  

{% include figure image_path="/assets/images/Screenshot 2025-10-20 064929.png" alt="AdventureWorks Data Model" %}

---

###  Key Measures (DAX)

Created a dedicated **DAX Measures Table** for all KPIs:

- `# Orders`
- `Total SubTotal`
- `Total Tax`
- `Total Freight`
- `Total Due`
- `Max Qty per Product`

These measures enable flexible, consistent calculations across multiple visuals.

---

###  Report Visuals & Features

The Power BI report includes:

- **Overview Page**: KPIs for Orders, Tax, Freight, and Due amounts  
- **Category & Territory Analysis**:  
  - Orders by Status and Order Date  
  - Order Quantity by Category → Subcategory → Product  
  - Orders vs. Total Due by Territory  
- **Matrix Chart**: Rows = Territories, Columns = Years, Values = Total & Canada Sales  
- **Drill Down / Drill Through** for interactive exploration  
- **Bookmarks** to toggle between charts  
- **Synced Slicers** across pages for consistent filtering  
- **Q&A Visual** for natural language queries  

---

### Design & Layout

- Used a **clean, meaningful color palette** with clear contrast  
- All visuals are labeled with **business-focused titles**  
- Ensured a balanced, professional layout suitable for executive dashboards  

---

### 🖼 Dashboard Preview

{% include figure image_path="/assets/images/Screenshot 2025-10-20 064701.png" alt="AdventureWorks Power BI Report — Overview" %}

---

### 🔗 Demo & Project Files

- **GitHub Repository:**  
  [https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/adventureworks-report](https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/adventureworks-report)

---

###  Key Learnings

This project deepened my understanding of **data modeling best practices**, **DAX optimization**, and **user-centered dashboard design**.  
It demonstrates how Power BI can turn complex operational data into **actionable insights** that support strategic decisions.

---
