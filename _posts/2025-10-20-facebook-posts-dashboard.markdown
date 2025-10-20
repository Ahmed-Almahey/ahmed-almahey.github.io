---
layout: posts
title: "Power BI — Facebook Posts Performance Dashboard"
date: 2025-10-20 07:30:00 +0200
tags: [Power BI]
author_profile: true
author: Ahmed Almahey
categories: [work]
highlight_home: true
header:
  overlay_image: "/assets/images/Screenshot 2025-10-20 065912.png"
  teaser: "/assets/images/Screenshot 2025-10-20 065912.png"
description: "Interactive Power BI dashboard built using Facebook Graph API — tracking post activity, engagement, and publishing trends with DAX measures and calculation groups."
---

**Power BI — Facebook Posts Performance Dashboard**

I built this project to explore **social media data analytics** using Power BI and Facebook’s **Graph API**.  
The main idea was to understand how post frequency and engagement evolve over time, and how data from social media platforms can be **transformed into actionable business insights**.

---

###  Project Inspiration

Social media pages generate a continuous stream of data — likes, comments, shares, and post reach — but that data is often scattered across different endpoints.  
I wanted to automate and visualize this process to simulate what a **social media manager or marketing analyst** might use to monitor performance.  

This dashboard aims to answer questions like:
- How active is my page over time?  
- Are we posting more or less than before?  
- What kind of posts generate higher activity?

---

### ⚙️ Data Source & Preparation

- **Data Source:** [Facebook Graph API](https://graph.facebook.com/)  
- **Platform:** [Meta for Developers](https://developers.facebook.com/)  
- **Connectivity Mode:** Import  
- **API Connection:** Personal Facebook App  

The data was pulled directly from my Facebook Page using Graph API endpoints for posts.  

Data preparation steps:
- Renamed queries and columns  
- Changed data types for consistency  
- Extracted **hashtags** and **links** from text fields  
- Added a **Post URL** column to allow click-through access from the report  

---

###  Data Modeling

After cleaning, I created key measures and used **calculation groups** to handle comparisons and trends:
- `# Posts`
- `# Posts Previous Month`
- `# Posts Running Total`

These measures enabled me to analyze post volume trends month-over-month and track cumulative activity across time.

---

###  Dashboard Visuals

The report focuses on simplicity and insight clarity.  
Main visuals include:

- **# Posts (Card)** — KPI summary  
- **# Posts by Date (Line Chart)** — trend analysis  
- **Post Details Table** — each post with a clickable URL icon  
- **Matrix View:** Month vs. Posts, Previous Month, and Running Total  

Each element was designed to provide a quick, clear view of how the page’s content strategy evolves over time.

{% include figure image_path="/assets/images/Screenshot 2025-10-20 065912.png" alt="Facebook Power BI Dashboard Overview" %}
{% include figure image_path="/assets/images/Screenshot 2025-10-20 070016.png" alt="Facebook Power BI Post Details View" %}

---

### 📱 Mobile Optimization

I designed a **mobile layout** for quick access on smaller screens — ideal for marketing teams or managers tracking daily content performance on the go.

---

###  Design & Layout

- Used **consistent, professional color palettes** suitable for a business dashboard  
- Added **interactive tooltips** and icons for clarity  
- Focused on minimal text and strong visual storytelling  

---

### 🔗 GitHub Repository

You can explore the `.pbix` file and data preparation steps here:  
👉 [https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/Facebook-Posts-Dashboard](https://github.com/Ahmed-Almahey/PowerBI_Projects/tree/main/Facebook-Posts-Dashboard)

---

###  What I Learned

This project helped me understand:
- How to connect **Power BI with REST APIs (Facebook Graph API)**  
- Using **calculation groups** for dynamic time-based metrics  
- The importance of **mobile-friendly Power BI design**

It also deepened my ability to turn **unstructured social data** into structured insights — a key skill for any **data professional in digital analytics**.

---

###  Looking Ahead

This project opened up ideas for future integrations — such as combining **Facebook + Instagram + Twitter APIs** into one unified social analytics dashboard.  
It’s also a foundation for automating **content performance reports** for marketing teams.

---

### 🏁 Summary

This Power BI dashboard proves that **social media analytics** doesn’t have to stay on the platform — it can be modeled, measured, and visualized like any business dataset.  
It’s a step toward building **data-driven marketing intelligence** tools that are both functional and visually insightful.

---
