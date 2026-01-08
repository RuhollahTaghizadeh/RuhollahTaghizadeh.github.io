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

<!-- pages/teaching.md -->
<div class="projects">
{% if page.display_categories %}
  <!-- Display categorized teaching items -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>

  {% assign categorized_items = site.teaching | where: "category", category %}
  {% assign sorted_items = categorized_items | sort: "importance" %}

  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for item in sorted_items %}
      {% include teaching_horizontal.liquid item=item %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for item in sorted_items %}
      {% include teaching.liquid item=item %}
    {% endfor %}
  </div>
  {% endif %}

  {% endfor %}
{% else %}

  <!-- Display teaching items without categories -->
  {% assign sorted_items = site.teaching | sort: "importance" %}

  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for item in sorted_items %}
      {% include teaching_horizontal.liquid item=item %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for item in sorted_items %}
      {% include teaching.liquid item=item %}
    {% endfor %}
  </div>
  {% endif %}

{% endif %}
</div>
