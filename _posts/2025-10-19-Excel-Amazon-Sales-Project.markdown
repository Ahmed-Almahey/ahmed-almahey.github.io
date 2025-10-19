---
layout: posts
title: "Excel Amazon Sales Project — Data Cleaning & Revenue Logic"
date: 2025-10-19 12:53:00 +0200
tags: [Excel]
author_profile: true
author: Ahmed Almahey
categories: [work]
header:
  overlay_image: "/assets/images/Screenshot 2025-10-19 125344.png"
  teaser: "/assets/images/Screenshot 2025-10-19 125344.png"
description: "An Excel-based Amazon Sales Project focused on data cleaning, consistency, and building accurate revenue logic for business-ready analysis."
---

**Excel Amazon Sales Project — Data Cleaning & Revenue Logic**

This project focused on preparing and validating Amazon sales data to ensure accurate revenue analysis.  
The goal was to design a clean dataset with consistent values, logical rules, and business-ready insights.

---

###  Data Cleaning Process

- Removed blank rows and duplicate records across the dataset.  
- Standardized inconsistent text values (e.g., variations of “Cancelled,” “Pending,” etc.).  
- Created a **Flagged Helper Column** to identify anomalies:
  - `OK` → valid records.  
  - `Anomaly` → flagged when Quantity = 0 with a non-zero Amount or both Quantity and Amount = 0.  
- Cleaned and standardized categorical fields such as **Status**, **Category**, and **Style**.  
- Adjusted **data types** to ensure smooth transformations and reliable calculations.

---

###  Revenue Logic & Business Rules

To ensure financial accuracy, I established clear inclusion/exclusion criteria:

- **Excluded:** Cancelled, Returned, Damaged/Lost, and Pending orders.  
- **Included:** Delivered, Shipped, and In Transit orders — considered valid revenue because many are prepaid.  
- **Flagged anomalies:**  
  - Quantity = 0 and Amount > 0 (or both 0) → excluded.  
- **Special cases:**  
  - If `Quantity > 0` but `Amount = 0` and status is Shipped/In Transit/Delivered → retained (represents promotions or free items).  
  - If status = Cancelled/Returned/Damaged → retained only if logically consistent (e.g., zero refunds).  

This logic ensures that every metric reflects **real and auditable business activity**.

---

###  Key Learnings

Through this project, I strengthened my ability to:
- Build **robust data-cleaning pipelines** inside Excel.  
- Design **flag-based validation systems** for anomaly detection.  
- Apply **business logic directly in the data layer** before visualization.  

This process makes future analyses more accurate and repeatable — essential for scalable reporting in e-commerce contexts.

---

### 🖼 Dashboard Preview

{% include figure image_path="/assets/images/Screenshot 2025-10-19 125344.png" alt="Excel Amazon Sales Project — Data Cleaning & Revenue Logic" %}

---

### 🔗 Project Files

- **GitHub Repo:**  
  [https://github.com/Ahmed-Almahey/Excel-Projects/tree/main/Amazon%20Sales%20Project](https://github.com/Ahmed-Almahey/Excel-Projects/tree/main/Amazon%20Sales%20Project)

