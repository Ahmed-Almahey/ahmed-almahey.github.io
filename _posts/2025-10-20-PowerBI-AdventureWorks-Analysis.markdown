---
layout: posts
title: "Power BI — AdventureWorks Sales & Product Analysis"
date: 2025-10-20 02:30:00 +0200
tags: [Power BI]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: true
header:
  overlay_image: "/assets/images/Screenshot 2025-10-20 055557.png"
  teaser: "/assets/images/Screenshot 2025-10-20 055557.png"
description: "End-to-end Power BI report analyzing AdventureWorks sales and product performance using star schema modeling, DAX measures, and interactive visuals."
---

**Power BI — AdventureWorks Sales & Product Analysis**

In this project, I built a comprehensive **sales and product performance report** using **Power BI** for the AdventureWorks dataset.  
The goal was to create a dynamic and visually engaging BI dashboard that helps stakeholders explore sales trends, regional performance, and product insights interactively.

---

###  Data Modeling & Preparation

- Imported the **Sales.xlsx** file as the primary data source.  
- Designed a **Star Schema** model linking fact and dimension tables for optimized relationships.  
- Implemented a **Product Hierarchy** (Category → Subcategory → Product) to support drill-down analysis.  
- Created a dedicated **DAX Measures Table** for better organization of KPIs.

---

###  DAX Measures Created

- `# Orders`
- `# Order Details`
- `Total SubTotal`
- `Total Tax`
- `Total Freight`
- `Total Due`

These measures formed the foundation for all visualizations, enabling accurate aggregation and comparison across dimensions.

---

### Visualizations & Insights

The dashboard includes a range of interactive visuals and KPIs:

- **Cards:** `# Orders`, `# Order Details`, `Total SubTotal`, `Total Tax`, `Total Freight`, `Total Due`
- **Charts:**  
  - Orders by Order Date  
  - Orders by Status  
  - Order Quantity by Category → Subcategory → Product  
  - Orders vs. Total Due by Territory  
- **Additional Features:**  
  - Tooltip pages for context-aware insights  
  - Drill-down capability for hierarchical analysis  
  - Clean layout with consistent colors and meaningful chart titles  

---

### 🖼 Dashboard Preview

{% include figure image_path="/assets/images/Screenshot 2025-10-20 055557.png" alt="Power BI Dashboard — Overview" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-20 055716.png" alt="Power BI Dashboard — Detailed Insights" %}

---

### 🔗 Project Repository

- **GitHub Repo:**  
  [https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/AdvendureWorks_Sales%26Product_Analysis](https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/AdvendureWorks_Sales%26Product_Analysis)

---
