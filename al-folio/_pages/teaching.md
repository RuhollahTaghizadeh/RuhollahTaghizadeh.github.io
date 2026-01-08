---
layout: page
title: teaching
permalink: /teaching/
description: Materials for courses and workshops I taught.
nav: true
nav_order: 6
display_categories: [Courses, Workshops]
horizontal: false
---

<div class="projects">
  {% for category in page.display_categories %}
    <a id="{{ category | slugify }}" href="#{{ category | slugify }}">
      <h2 class="category">{{ category }}</h2>
    </a>

    {% assign categorized_teaching = site.teaching | where: "category", category %}
    {% assign sorted_teaching = categorized_teaching | sort: "importance" %}

    <div class="row row-cols-1 row-cols-md-3">
      {% for teaching in sorted_teaching %}
        {% include teaching.liquid %}
      {% endfor %}
    </div>
  {% endfor %}
</div>
