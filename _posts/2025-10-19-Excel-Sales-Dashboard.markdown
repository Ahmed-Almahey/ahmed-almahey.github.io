---
layout: posts
title: "Excel Sales Dashboard — Last Month Analysis"
date: 2025-10-19 05:36:00 +0200
tags: [Excel]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: true
header:
  overlay_image: "/assets/images/Screenshot 2025-10-19 073647.png"
  teaser: "/assets/images/Screenshot 2025-10-19 073647.png"
description: "End-to-end Excel sales dashboard using Power Query, star schema, and time intelligence to compare last vs previous month."
---

**Excel Sales Dashboard — Last Month Analysis**

Businesses need month-over-month insights to track revenue trends and performance.  
I built this Excel dashboard using Power Query, Data Modeling, and PivotTables to compare **Last Month vs Previous Month** sales and reveal key drivers.

---

### Data Preparation & Modeling

- Loaded **masterdata.xlsx** as a workbook and created connections for Employees, Products, Customers  
- Cleaned and transformed **salesdata.txt** and added a calculated column: `Sales = Qty × Unit Price`  
- Built a **Date Table** with Month, Month Name, Month Flags (Last / Previous)  
- Created a **star schema model** linking Fact Sales to all dimension tables  

{% include figure image_path="/assets/images/Screenshot 2025-10-19 080341.png" alt="Data Model" %}

---

### Dashboard Insights

The dashboard includes:

- **Month-over-Month Sales** comparison with % change  
- **Top 3 Sales Managers** (Last Month)  
- **Sales by Product Category** with MoM % change  
- **Top 5 Customers** and **Top 5 Employees** (interactive with slicers)  
- **Sales Trend by Month** (formatted in millions with currency)

This simulates a realistic business reporting scenario using Excel as a lightweight BI solution.

---


### 🖼 Dashboard Preview

{% include figure image_path="/assets/images/Screenshot 2025-10-19 073647.png" alt="Excel Sales Dashboard — Last Month Analysis" %}


### 🔗 Demo & Project Files

- **GitHub Repo:**  
  [https://github.com/Ahmed-Almahey/Excel-Projects/tree/main/Last%20Month%20Dashboard](https://github.com/Ahmed-Almahey/Excel-Projects/tree/main/Last%20Month%20Dashboard)

- **LinkedIn Demo (Video):**  
  [Watch on LinkedIn](https://www.linkedin.com/posts/ahmed-almahey_dataanalytics-exceldashboard-powerquery-activity-7379421872494460929-9ANJ?utm_source=share&utm_medium=member_desktop&rcm=ACoAACc9-lYBwv4AGqqF7Pyk4h-OiyXQ8haYNow)

---