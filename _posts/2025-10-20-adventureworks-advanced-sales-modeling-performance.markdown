---
layout: posts
title: "Power BI — AdventureWorks Advanced Sales Modeling & Performance Dashboard"
date: 2025-10-20 06:10:00 +0200
tags: [Power BI]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: true
header:
  overlay_image: "/assets/images/Screenshot 2025-10-20 190419.png"
  teaser: "/assets/images/Screenshot 2025-10-20 190419.png"
description: "An advanced Power BI dashboard for AdventureWorks sales performance — featuring complex DAX modeling, hierarchy design, and relationship management for real-world business analysis."
---

**Power BI — AdventureWorks Advanced Sales Modeling & Performance Dashboard**

This project was inspired by a simple goal — to push my Power BI modeling skills beyond standard reporting and simulate a **real enterprise BI scenario**.  
AdventureWorks provided the perfect dataset for building a **multi-dimensional analytical model** that mirrors real-world retail sales environments.

I wanted to understand how professional data teams handle **large relational models**, complex **date relationships**, and optimize **DAX calculations** for high performance.

---

###  Project Objective

The purpose of this project was to design a **robust analytical dashboard** that allows business users to track sales trends, monitor regional performance, and evaluate product profitability efficiently — all through a clean, interactive Power BI experience.  

It aims to answer questions like:
- How do sales vary by order date, due date, and ship date?  
- Which products and territories drive the most revenue?  
- What are the most profitable shipping methods and salespeople?  

---

###  Data Source & Preparation

- **Data Source:** [AdventureWorks Sample Database (Microsoft Docs)](https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms)  
- **Connectivity Mode:** Import (to make file sharing easier — no need for SQL connection setup)  
- Original connectivity was **DirectQuery**, but switched to Import for portability.  
- Extracted and cleaned multiple tables:  
  - `Sales.SalesOrderHeader`, `Sales.SalesOrderDetail`, `Sales.vSalesPerson`,  
    `Sales.SalesTerritory`, `Purchasing.ShipMethod`,  
    `Production.Product`, `Production.ProductSubcategory`, `Production.ProductCategory`  

**Data Preparation Steps:**
- Renamed tables and columns for consistency  
- Removed unused columns for model efficiency  
- Merged product-related tables (`Product`, `Subcategory`, `Category`) using Power Query (M language)  
- Added calculated **Status** field using logic from `ufnGetSalesOrderStatusText()`  
- Created **Dates** table in Power Query  
- Fixed TotalDue, Tax, and Freight values via DAX and Power Query transformations  

---

###  Data Modeling

The model follows a **Star Schema**, optimized for clear relationships and flexible analysis.  

**Features:**
- Defined **Product Hierarchy** → Category → Subcategory → Product  
- Built **role-playing date dimensions** (OrderDate, ShipDate, DueDate) using `USERELATIONSHIP()`  
- Created a dedicated **DAX Measures Table** containing all KPIs  

**Key Measures:**
- `# Orders`  
- `Total SubTotal`  
- `Total Tax`  
- `Total Freight`  
- `Total Due`  
- `# Quantity`  

---

###  Visuals & Insights

The dashboard includes a full analytical flow across multiple views:

- **Cards:** KPIs for Orders, SubTotal, Tax, Freight, and Due  
- **Time Analysis:** Orders by OrderDate, ShipDate, and DueDate  
- **Sales Breakdown:** Orders by Status and ShipMethod  
- **Product Insights:** Quantity by Category → SubCategory → Product  
- **Regional Analysis:** Orders vs. TotalDue by Territory  
- **Top 10 Salespersons:** ranked by Orders or Total Amount  
- **Advanced Features:**  
  - Drill Down  
  - Drill Through  
  - Tooltip Pages  

{% include figure image_path="/assets/images/Screenshot 2025-10-20 190419.png" alt="AdventureWorks Power BI Dashboard Overview" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-20 120652.png" alt="AdventureWorks Data Modeling" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-20 190442.png" alt="Power BI Sales Visualizations" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-20 190501.png" alt="Power BI Product Insights" %}

---

###  What I Learned

This project challenged me to think like a **data modeler, not just a report designer**.  
I learned how to:
- Manage complex date relationships and inactive relationships  
- Build scalable star schemas  
- Optimize DAX performance  
- Maintain consistency across visuals and KPIs  

It taught me how **data modeling choices** affect dashboard responsiveness, accuracy, and user experience — lessons that directly apply to enterprise-level BI development.

---

###  Future Impact

By completing this project, I strengthened my ability to deliver **production-ready dashboards**.  
In a future analytics role, this experience helps me:
- Design efficient data models from relational sources  
- Implement reusable DAX logic for any business domain  
- Communicate insights effectively through well-structured visuals  

---

### 🔗 Project Files

- **GitHub Repository:**  
  [https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/AdventureWorks_Advanced_Sales_Modeling_Performance.pbix](https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/AdventureWorks_Advanced_Sales_Modeling_Performance.pbix)

---

###  References

- [AdventureWorks Sample Database Documentation](https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms)  
- [RADACAD — USERELATIONSHIP and Role-Playing Dimensions in Power BI](https://radacad.com/userelationship-or-role-playing-dimension-dealing-with-inactive-relationships-in-power-bi)

---

