---
layout: posts
title: "Customer Segmentation using Unsupervised Machine Learning"
date: 2025-10-20 01:36:00 +0200
tags: [Python]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: true
header:
  overlay_image: "/assets/images/1747404460297.png"
  teaser: "/assets/images/1747404460297.png"
description: "Customer segmentation using K-Means clustering to identify distinct customer groups and support data-driven marketing strategies."
---

**Customer Segmentation using Unsupervised Machine Learning**

Businesses often struggle to tailor their marketing efforts because not all customers behave the same way.  
This project uses **unsupervised machine learning** to segment customers based on their **spending behavior, age, and income**, helping businesses **understand their audience and personalize their marketing** more effectively.

---

###  Data Understanding & Preparation

Before applying machine learning, I conducted a full **Exploratory Data Analysis (EDA)** and data preprocessing phase:

- Loaded mall customer dataset containing **Customer ID, Gender, Age, Annual Income, and Spending Score**.  
- Handled missing values and ensured correct data types.  
- Standardized features using normalization for accurate clustering.  
- Visualized variable distributions and relationships to understand spending patterns across demographics.

---

###  Model Implementation

To identify meaningful customer groups, I implemented **K-Means Clustering**, following these steps:

- Used the **Elbow Method** and **Silhouette Score** to determine the optimal number of clusters.  
- Trained the K-Means model on standardized data.  
- Assigned each customer to a specific cluster label.  
- Visualized cluster distributions using scatter plots to interpret group characteristics.

{% include figure image_path="/assets/images/1747404460297.png" alt="K-Means Cluster Visualization" %}
{% include figure image_path="/assets/images/1747404460606.png" alt="Elbow Method Chart" %}
{% include figure image_path="/assets/images/1747404461129.png" alt="Customer Distribution by Cluster" %}

---

###  Insights & Business Impact

After clustering, distinct customer segments were revealed:

- **Cluster 1:** Young customers with high income and high spending — *potential luxury buyers*.  
- **Cluster 2:** Mid-age, moderate spenders — *steady customers with potential for upselling*.  
- **Cluster 3:** High-income but low-spending — *price-sensitive group needing re-engagement*.  
- **Cluster 4:** Low-income, high-spending — *value-driven impulsive buyers*.

By identifying these segments, businesses can now:
- Design **targeted campaigns** tailored to each group’s preferences.  
- Optimize **product recommendations** and **promotional offers**.  
- Allocate **marketing budgets** more efficiently.

---

### Tools & Technologies Used

- **Python**, **pandas**, **NumPy**, **scikit-learn**, **matplotlib**, **seaborn**  
- **K-Means Clustering**, **EDA**, **Feature Scaling**, **Visualization**

---

### 🔗 GitHub Repository

[View the Full Project on GitHub](https://github.com/Ahmed-Almahey/Customer-Segmentation-data-mining)
