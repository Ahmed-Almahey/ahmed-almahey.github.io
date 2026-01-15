---
title: "My Work"
layout: archive
category: work
author: Ahmed Almahey
author_profile: true
classes: page--mywork
---

Over Time, I’ve combined my background in mathematics and statistics with my passion for data and technology.  
Here you’ll find a collection of my work in data analysis, BI development, and visualization — each project reflecting my focus on turning numbers into meaningful insights.

---

<div class="tags-navigation">
 <a href="#BI" class="tag-btn">End-to-End BI Projects</a>
  <a href="#powerbi" class="tag-btn">Power BI</a>
  <a href="#python" class="tag-btn">Python</a>
  <a href="#tableau" class="tag-btn">Tableau</a>
  <a href="#excel" class="tag-btn">Excel</a>
  <a href="#sql" class="tag-btn">SQL</a>
   <a href="#BITOOLS" class="tag-btn">BI TOOLS (SSIS, SSAS, SSRS)</a>
  <a href="#DWH" class="tag-btn">Data Warehouse</a>
  <a href="#mongodb" class="tag-btn">MongoDB</a>
</div>

---

## End-to-End BI Projects {#BI}
<div class="entries-grid entries-grid--mywork">
{% for post in site.categories.work %}
  {% if post.tags contains "End-to-End" %}
    {% include archive-single.html type="grid" %}
  {% endif %}
{% endfor %}
</div>

---

## 🟦 Power BI Projects {#powerbi}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "Power BI" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

---

## 🐍 Python Projects {#python}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "Python" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

---

## 📊 Tableau Projects {#tableau}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "Tableau" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

---

## 📈 Excel Projects {#excel}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "Excel" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

---

## 🗄️ BI Tools (SSIS, SSRS, SSAS) Projects {#BITOOLS}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "BI TOOLS" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

---

## 🗄️ SQL Projects {#sql}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "SQL" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

---
## 🗄️ Data Warehouse Projects {#DWH}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "Data Warehouse" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

---


## 🍃 MongoDB Projects {#mongodb}
<div class="entries-grid entries-grid--mywork">
  {% for post in site.categories.work %}
    {% if post.tags contains "MongoDB" %}
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>

