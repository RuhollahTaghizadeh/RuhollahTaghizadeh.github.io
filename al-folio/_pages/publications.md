---
layout: page
permalink: /publications/
title: publications
description: "<span style='color:#c00000;'>List not exhaustive — see <a href='https://scholar.google.com/citations?user=IDHEr08AAAAJ' target='_blank' rel='noopener' style='color:#1a73e8; text-decoration:underline; font-weight:600;'>Google Scholar</a>.</span>"
nav: true
nav_order: 2
---

{% include bib_search.liquid %}

<p style="margin: 0 0 12px 0;">
  <img src="{{ '/assets/img/PedometricsResearch.png' | relative_url }}"
       alt="PedometricsResearch"
       style="width:420px; max-width:100%; height:auto; border-radius:8px;">
</p>

<div class="publications">
{% bibliography %}
</div>
