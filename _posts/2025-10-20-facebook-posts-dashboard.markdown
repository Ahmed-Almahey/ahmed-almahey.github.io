---
layout: posts
title: "Facebook Posts Dashboard — Power BI Graph API Integration"
date: 2025-10-20 06:45:00 +0200
tags: [PowerBI]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: true
header:
  overlay_image: "/assets/images/Screenshot 2025-10-20 065912.png"
  teaser: "/assets/images/Screenshot 2025-10-20 065912.png"
description: "Power BI dashboard connected to Facebook Graph API to analyze and visualize post performance metrics over time."
---

**Facebook Posts Dashboard — Power BI Graph API Integration**

Social media insights are key to understanding engagement trends and audience behavior.  
This Power BI project connects directly to the **Facebook Graph API**, fetching post data in real-time to visualize publishing patterns, hashtags, and performance metrics.

---

### Data Source & Preparation

- **Data Source:** Facebook Graph API (Personal Account or Page Posts)  
  - [Graph API Documentation](https://developers.facebook.com/docs/graph-api)  
  - [Facebook Developer Portal](https://developers.facebook.com/)

- Created a **Facebook App** to authenticate and connect to post data  
- Renamed query names and standardized column headers  
- Changed data types where needed for clean modeling  
- Extracted **links** and **hashtags** from post content  
- Added a **Post URL** column for interactivity

---

### Data Modeling

- Designed a **star schema** optimized for time-based insights  
- Created **calculation groups** for dynamic metrics:
  - `# Posts`
  - `# Posts Previous Month`
  - `# Posts Running Total`
- Built relationships and date hierarchies for month-over-month tracking

---

### Visualizations

The dashboard includes:

- **# Posts Card** with dynamic monthly counts  
- **Posts by Date** time series  
- **Post Details Table** (with clickable Post URLs shown as icons)  
- **Matrix** showing Month, # Posts, # Posts Previous Month, and # Posts Running Total  

A **mobile layout** was also designed for on-the-go analysis.  
Color themes, titles, and layouts were optimized for readability and storytelling.

{% include figure image_path="/assets/images/Screenshot 2025-10-20 065912.png" alt="Facebook Posts Dashboard" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-20 070016.png" alt="Power BI Facebook Integration" %}

---

###  Key Learning & Deployment

This project demonstrates the power of **API connectivity** in Power BI, showing how to integrate external web data for automated reporting.

Finally, the report was **published to Power BI Report Server** for secure sharing and management within an enterprise environment.

---

### 🔗 Project Files

- **GitHub Repo:**  
  [https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/Facebook-Posts-Dashboard](https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/Facebook-Posts-Dashboard)
