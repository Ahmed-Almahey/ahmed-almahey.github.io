---
layout: posts
title: "Airlines Delay Analysis"
date: 2025-10-16 08:24:00 +0200
tags: [Power BI]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: false
header:
  overlay_image: "/assets/images/Screenshot 2025-10-16 083436.png"
  teaser: "/assets/images/Screenshot 2025-10-16 083436.png"
  caption: "Photo credit: [Unsplash: Myriam Jessier](https://unsplash.com/@mjessier)"
description: "Analysis of airline delays using Power BI and statistical techniques."
---
✈️ **Airlines Delay Analysis — Power BI Project**

This project was built to answer a real business question:  
*Where and why do flight delays happen — and how can airlines act on the insights?*

I approached the problem as if designing an internal BI report for airline operations teams.  
The goal was not only to visualize delay KPIs, but to **engineer a model that supports accurate time, geography, and carrier-level analysis**.

---

🖼 Dashboard Previews {% include figure image_path="/assets/images/Screenshot 2025-10-16 083436.png" alt="Airline Delay Power BI Dashboard" %} {% include figure image_path="/assets/images/Screenshot 2025-10-16 185128.png" alt="Airline Delay Visualization" %} {% include figure image_path="/assets/images/Screenshot 2025-10-16 185856.png" alt="Airline Delay Analysis Charts" %}

---

### Project Objective
To design a dashboard that helps aviation stakeholders:
- Understand which **delay types** are most impactful
- Identify **airlines and regions** most responsible for delays
- Detect **time-based patterns** in operational performance
- Guide decisions in scheduling, staffing, and route optimization

---

### Modeling & Technical Work

- Built a **Star Schema** to separate facts from dimensions
- Created a **Date Dimension** in DAX for time-series intelligence
- Created a **Location Dimension** to unify Origin and Destination analysis
- Resolved a **many-to-many relationship** scenario with proper modeling techniques
- Built a dedicated **DAX Measures Table** with KPIs such as:  
  - Total Delays by Type  
  - Average Arrival / Departure Delay  
  - Delays per Flight  
  - Weather-based Delay Metrics  

---

### Visuals & Insights Delivered

- **Map visual** to show geographic clusters of delays  
- **Bar charts** by airline and delay categories  
- **Time trend lines** to detect seasonal or operational patterns  
- **Scatter plot** relating delay to flight distance  

These visuals reveal which airlines suffer most from carrier errors, which regions are weather-vulnerable, and how delays evolve over time.

---

### What I Learned & Why It Matters

This project reinforced habits of **thinking like a modeler, not just a report builder**:
- Model complexity directly affects accuracy and insights
- Role-playing dimensions and relationships determine what questions can be answered
- A reusable modeling approach makes future BI projects faster and more reliable

These lessons now influence how I build every new Power BI project going forward.

---

### 🔗 Project Files

- **GitHub Repo:**  
  [https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/Airlines-Delay-Dashboard](https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/Airlines-Delay-Dashboard)
