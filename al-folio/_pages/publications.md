---
layout: page
permalink: /publications/
title: publications
description: "<span style='color:#c00000;'>List not exhaustive — see <a href='https://scholar.google.com/citations?user=IDHEr08AAAAJ' target='_blank' rel='noopener' style='color:#1a73e8; text-decoration:underline; font-weight:600;'>Google Scholar</a>.</span>"
nav: true
nav_order: 2
---

<!-- Bibsearch Feature -->
{% include bib_search.liquid %}

<!-- Your custom content -->
## Research topics
<p>
  <img src="{{ '/assets/img/PedometricsResearch.png' | relative_url }}"
       alt="Research topics word cloud"
       style="max-width:900px;width:100%;height:auto;border-radius:10px;box-shadow:0 6px 18px rgba(0,0,0,0.08);">
</p>

<p class="small text-muted">
  Keywords represent recurring themes across my work (not exhaustive).
</p>

<hr>

<div class="publications">
{% bibliography %}
</div>
