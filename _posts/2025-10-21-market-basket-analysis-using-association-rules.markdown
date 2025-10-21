---
layout: posts
title: "Market Basket Analysis Using Association Rules"
date: 2025-10-21 7:55:00 +0200
tags: [Python]
author_profile: true
author: Ahmed Almahey
categories: [work]
header:
  overlay_image: "/assets/images/Screenshot 2025-10-21 105156.png"
  teaser: "/assets/images/Screenshot 2025-10-21 105156.png"
description: "Python-based Market Basket Analysis using Apriori algorithm to uncover frequent itemsets and association rules from Egyptian grocery transactions."
---

##  Project Overview
This project focuses on **Market Basket Analysis**, a fundamental **data mining** technique used to uncover patterns and associations between items in transactional datasets.  
Using **Python** and the **Apriori algorithm**, the goal was to analyze purchasing behavior within an **Egyptian supermarket dataset**, identifying commonly co-purchased products and actionable shopping insights.

![Market Basket Analysis Project Screenshot](/assets/images/Screenshot 2025-10-21 105156.png)

---

##  Dataset
**Dataset:** `Egyptian_Grocery_Transactions.xlsx`  
The dataset contains **grocery transactions** from a typical Egyptian store.  
Each record lists items purchased together — including local Egyptian foods like *baladi bread, ful, and taameya*.  
These patterns help uncover which products are frequently bought together.

---

##  Objective
Apply **market basket analysis** techniques to:
- Discover meaningful **item associations**  
- Identify **frequent itemsets**  
- Derive **association rules** with confidence and lift metrics  
- Visualize top relationships using charts and graphs  

---

##  Tasks Summary

1. **Load and Preprocess the Dataset**
   - Split transactions into item lists  
   - Use `TransactionEncoder` for one-hot encoding  

2. **Generate Frequent Itemsets**
   - Implement **Apriori algorithm**  
   - Set `min_support = 0.1` and sort by support  

3. **Generate Association Rules**
   - Use `metric='confidence'` and `min_threshold=0.3`  
   - Analyze rules using **confidence** and **lift**  
   - Identify at least **2 strong rules** and **2 weak rules**  

4. **Bonus**
   - Visualize rules using bar charts or network graphs  

---

##  Deliverables
- A clean, well-commented **Jupyter Notebook** (`.ipynb`)  
- A concise **summary of insights** from the analysis  

---

##  Key Skills Demonstrated
- Data preprocessing and transformation  
- Use of **Apriori** and **association rule mining** in Python  
- Practical understanding of **confidence**, **lift**, and **support**  
- Visualizing relationships through **data visualization tools**  
- Data storytelling and result interpretation  

---

##  Repository
Explore the full code and notebook here:  
 [GitHub Repository](https://github.com/Ahmed-Almahey/data_mining/tree/main)
