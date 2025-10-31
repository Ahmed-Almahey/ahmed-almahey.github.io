---
layout: posts
title: "SSRS — Student Data & BI Reports"
date: 2025-10-21 14:00:00 +0200
tags: [BI TOOLS (SSIS, SSAS, SSRS)]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: true
header:
  overlay_image: "/assets/images/Students_data.png"
  teaser: "/assets/images/Students_data.png"
description: "Building dynamic, interactive SSRS reports for real-world student data and sales insights."
---

**SSRS — Student Data & BI Reports**

In business, reports aren’t just data — they’re decisions made visible.  
This project brings that philosophy to life by using **SQL Server Reporting Services (SSRS)** to transform raw student and sales data into interactive, insightful visual reports.

---

### 🎯 Business Problem & Goal

Every organization, from education to enterprise, needs to **turn data into clarity**.  
The goal here was to design a series of SSRS reports that allow users — such as school administrators or business managers — to quickly extract insights, filter data, and present it in a professional format (PDF, charts, and dashboards).

These reports simulate real-world BI reporting scenarios across education and sales domains.

---

###  What I Built

1. **Tabular Student Report**
   - Added headers and footers with dynamic expressions (user name, execution time)
   - Embedded institutional logo for branding consistency  
   - Conditional formatting to highlight students aged above 23  
   - Displayed total student count in the last row  
   - Enabled **interactive sorting** on student age  
   - Exported reports as **PDF**

2. **Topic & Courses Report**
   - Used the wizard to display topics with related courses  
   - Ensured each topic appears on a **separate page**  
   - Added built-in pagination (“Page X of Y”)

3. **Sales Matrix Report**
   - Designed a **matrix layout** that aggregates quantities per ProductID and Salesman  
   - Built directly from SQL queries to simulate enterprise sales reports

4. **Chart Visualization**
   - Converted the matrix report into a **visual dashboard** using SSRS charts  
   - Showed key trends for faster, data-driven decisions

5. **Student Grades Indicator**
   - Designed a report with **color-coded grade indicators**  
     - Red (0–50), Yellow (51–60), Green (61–100)

6. **Parameterized Reports**
   - Used **stored procedures** with parameters (`Age1`, `Age2`, `Dept_ID`)  
   - Displayed parameter selections dynamically in report headers  
   - Allowed multiple department selections via dropdowns

7. **Advanced Scenarios**
   - Demonstrated **linked reports**  
   - Integrated SSRS with **SQL Server Analysis Services (SSAS)** cubes for multi-dimensional data  
   - Enabled filtering by year from OLAP data sources

---

### 🖼 Project Preview

{% include figure image_path="/assets/images/Students_data.png" alt="SSRS Student Data Report" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-31 132647.png" alt="SSRS Tabular Report Preview" %}
{% include figure image_path="/assets/images/Q3_Matrix.png" alt="SSRS Matrix Report" %}

---

###  What I Learned

This project refined my understanding of:
- Designing **dynamic and interactive BI reports**
- Applying **expressions, parameters, and conditional formatting** effectively
- Integrating SSRS with **SQL Server and Analysis Services**
- Thinking about reporting not only as a technical task but as a **communication tool for business stakeholders**

---

###  Impact on My Work

Building this SSRS project enhanced my ability to:
- Structure BI solutions end-to-end (SSIS → SSAS → SSRS)  
- Communicate insights visually for non-technical audiences  
- Approach future BI projects with a **business-first mindset**

---

### 🔗 Project Resources

- **GitHub Repo:** [SQL Server BI Tools — SSRS](https://github.com/Ahmed-Almahey/SQL-Server-BI-Tools/tree/main/SSRS)

---

###  Reflection

This project was more than a technical exercise — it was an exercise in *clarity*.  
It taught me how structured reports can bridge the gap between data and decision-making, a lesson I’ve carried into every BI solution since.

