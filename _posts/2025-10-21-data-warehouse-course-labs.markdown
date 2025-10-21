---
layout: posts
title: "Data Warehouse — Dimensional Modeling & OLAP Design"
date: 2025-10-21 01:36:00 +0200
tags: [Data Warehouse]
author_profile: true
author: Ahmed Almahey
categories: [work]
header:
  overlay_image: "/assets/images/data-warehouse-landing-page.png"
  teaser: "/assets/images/data-warehouse-landing-page.png"
description: "A collection of Data Warehouse design and modeling tasks completed during the ITI course, covering star schema design, dimensional modeling, and OLTP-to-OLAP transformation."
---

**Data Warehouse — Dimensional Modeling & OLAP Design**

This work represents a series of **Data Warehouse modeling and design exercises** completed during the ITI program, focused on understanding and implementing data warehousing concepts such as **dimensional modeling, star schema design, and OLTP-to-OLAP transformation**.

The goal of these tasks was to apply theoretical knowledge in a hands-on way — converting normalized databases into analytical models, and designing warehouse structures optimized for reporting and business intelligence.

---

###  Objectives
- Learn the **principles of dimensional modeling** and schema design.
- Apply **ETL thinking** to transform transactional (OLTP) systems into analytical (OLAP) structures.
- Design **fact and dimension tables** with clearly defined relationships, keys, and measures.
- Understand the **business logic behind aggregation and drill-down** analysis.

---

###  Key Exercises & Case Studies

1. **Hospital Visits Data Warehouse**  
   Designed a star schema with `Time`, `Doctor`, and `Patient` dimensions, and measures `Count` and `Charge`.  
   Focused on understanding the relationship between service activity and revenue.

2. **University Academic Performance Warehouse**  
   Created a schema with `Student`, `Course`, `Semester`, and `Instructor` dimensions, tracking measures like `Count` and `Average Grade`.  
   Practiced modeling across hierarchical levels for academic analytics.

3. **Sports Ticketing Warehouse**  
   Modeled data for `Date`, `Spectator`, `Location`, and `Game` dimensions, analyzing ticket counts and charge rates by audience segment.

4. **Furniture Sales Warehouse**  
   Designed a star schema analyzing sales by product attributes (`Type`, `Category`, `Material`) and customer geography (`City`, `Region`, `State`).  
   Measures included `Quantity`, `Income`, and `Discount`.

5–7. **OLTP to OLAP Conversion Tasks**  
   Converted normalized 3NF relational models into dimensional models.  
   Defined **fact tables, dimension hierarchies**, and **surrogate keys**, ensuring scalability and analytical efficiency.

---

### 🧱 OLTP to Data Warehouse Transformation

One major component involved transforming a **Sales OLTP database** into a **Data Warehouse schema**, optimizing it for analysis.  
Below is a sample of the original OLTP design used in conversion:

![OLTP Schema Preview](/assets/images/Screenshot 2025-10-21 100244.png)



![Data Warehouse Schema Preview](/assets/images/Screenshot 2025-10-21 100746.png)

The challenge was restructuring it to support **analytical querying**, focusing on aggregations like total sales, revenue per region, and product category performance.

---

### 🔗 Repository
- **GitHub Repository:**  
  [https://github.com/Ahmed-Almahey/Data-Warehouse](https://github.com/Ahmed-Almahey/Data-Warehouse)

---

###  Key Learnings
This set of labs strengthened my understanding of:
- **Dimensional modeling and schema optimization**
- **Fact/dimension relationships and key design**
- **Analytical thinking for business data**
- **Bridging OLTP systems with OLAP environments**

These foundations shaped how I now approach building **data-driven systems** — ensuring that every database design supports both **efficient transactions** and **meaningful insights**.

---
