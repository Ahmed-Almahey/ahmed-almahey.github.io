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
description: "End-to-end Power BI report built on the AdventureWorks dataset — modeling sales data with star schema, role-playing dates, and interaction-ready analytical visuals."
---

**Power BI — AdventureWorks Sales & Product Report**

I built this project to simulate how a BI team would analyze retail performance using a real-world dataset.  
The goal was not just to visualize numbers — but to model the data correctly, manage relationships, and design a dashboard that supports operational and managerial decisions.

---

###  Project Objective

Help decision makers answer questions like:
- How do orders trend across OrderDate, ShipDate, and DueDate?
- Which territories and products contribute most to revenue?
- How do categories drill down to individual products?
- How do regional sales evolve over years?

---

###  Data Modeling & Engineering

- Built a **Star Schema** from curated AdventureWorks views  
- Created **DimDates in DAX** with Year/Month/Day attributes  
- Defined **Product & Date hierarchies** for drill navigation  
- Used `USERELATIONSHIP()` for **role-playing date tables**
- Built a **dedicated DAX Measures Table** containing:
  - `# Orders`
  - `Total SubTotal`
  - `Total Tax`
  - `Total Freight`
  - `Total Due`
  - `Max Qty per Product`

---

###  Report Features & Visuals

The report includes industry-grade BI features:

- **Matrix view** — Territories × Years (Total & Canada Sales)
- **Line charts using inactive dates** (Order/Ship/Due)
- **Drill Down & Drill Through** navigation  
- **Bookmarks** to toggle between chart states  
- **Synced slicers** across pages  
- **Q&A visual** for natural-language exploration  
- Clean layout with business-focused titles and consistent formatting

{% include figure image_path="/assets/images/Screenshot 2025-10-20 064701.png" alt="AdventureWorks Power BI Report — Overview" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-20 064929.png" alt="AdventureWorks Data Model" %}

---

###  Project Files

- **GitHub Repository:**  
  https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/adventureworks-report

- **Data Source:**  
  https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms

---

###  Key Learnings

This project solidified my skills in:
- Building scalable, business-ready star schemas  
- Handling inactive relationships with `USERELATIONSHIP()`  
- Organizing KPIs via dedicated Measures Tables  
- Designing dashboards for interactive business analysis — not static reports

These patterns are transferable to any enterprise BI project involving sales, logistics, finance, or operations.

