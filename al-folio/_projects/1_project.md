---
layout: page
title: Precision Irrigation
description: Multi-depth soil water content maps for precision irrigation
img: assets/img/soilmoisture_kerry.png
importance: 1
category: Soil Sensing & Remote Observation
related_publications: true
---

Accurate **root-zone soil volumetric water content (VWC)** maps (0–120 cm) are critical for **variable-rate irrigation (VRI)**, especially in drought-prone regions.  
In this project, we used **Random Forests** with **UAV reflectance**, **terrain attributes**, and **yield monitor data** to map VWC at **four depths** (0–30, 30–60, 60–90, 90–120 cm) at **field scale (5 m grid)**.

### What we did
- Trained RF models using dense covariates (UAV indices, DEM derivatives, yield, distance/scaling features).
- Produced **multi-depth VWC maps** for multiple seasons.
- Quantified uncertainty via cross-validation and a **jack-knife** experiment to find the “good enough” sample size.

### Key findings 
- RF predicted VWC well (typically ~**1–3% RMSE**), with performance varying by **depth and season**.
- **Terrain + scaling factors** were usually more informative than crop reflectance, except after unusually hot periods.
- Sampling could often be reduced to about **50–60 points** (from >100) while keeping errors around **2–3%**.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/soilmoisture_kerry.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Graphical abstract summarizing the workflow and key results.
</div>


---

## Why it matters
This workflow shows how **dense digital data** can support **practical VRI decisions** by providing **root-zone moisture context**, not just surface patterns—while also highlighting that **some field sampling remains necessary** for reliable calibration.

> Paper: *Mapping Soil Volumetric Water Content at Multiple Depths for Variable Rate Irrigation Using UAV and Yield Monitor Data With Random Forests* (Soil Use and Management, 2025).
