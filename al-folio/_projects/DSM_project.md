---
layout: page
title: Spatial Prediction of Soils
description: Maps soil properties from samples using covariates and spatial validation, producing high-resolution predictions with confidence.
img: assets/img/spatial_soil.png
importance: 1
category: Digital Soil Mapping
related_publications: true
---

This project converts point-based soil measurements into continuous, high-resolution maps that better represent real landscape variability than traditional polygon soil maps. We compile soil observations for key variables (e.g., soil organic carbon, texture fractions, pH, salinity-related indicators, calcium carbonate, cation exchange capacity, and hydraulic properties) and link them to environmental covariates that capture soil-forming factors and processes, including terrain derivatives, climate layers, land cover/vegetation proxies, geology/parent material, and remote-sensing predictors such as multispectral indices and bare-soil composites. Using machine learning, we model nonlinear relationships and interactions between covariates and soil properties, then evaluate performance with spatially informed validation strategies to reduce overly optimistic accuracy estimates caused by spatial autocorrelation. The deliverables are prediction surfaces suitable for field-to-regional applications, often accompanied by uncertainty or confidence layers that communicate where estimates are robust and where extrapolation risk is higher. These products support decision-making in precision agriculture (management zones, variable-rate inputs), soil health monitoring, land suitability assessments, and environmental modelling, while also guiding efficient sampling by identifying areas where additional observations would most improve map reliability.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/spatial_soil.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Graphical abstract summarizing the workflow and key results.
</div>


---

