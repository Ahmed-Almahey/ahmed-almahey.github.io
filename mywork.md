---
title: "My Work"
layout: archive
author: Ahmed Almahey
author_profile: true
---

Over the years, I’ve combined my background in mathematics and statistics with my passion for data and technology.  
Here you’ll find a collection of my work in data analysis, BI development, and visualization — each project reflecting my focus on turning numbers into meaningful insights.

<hr>

{% assign work_posts = site.posts | where_exp: "post", "post.categories contains 'work'" %}
{% if work_posts.size > 0 %}
  <div class="entries-grid">
  {% for post in work_posts %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
  </div>
{% else %}
  <p>No projects found in the <strong>work</strong> category yet.</p>
{% endif %}
