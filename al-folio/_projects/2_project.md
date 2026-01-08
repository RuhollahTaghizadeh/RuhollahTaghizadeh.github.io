---
layout: page
title: Explainable SOC Mapping
description: Learning-based explanations for SOC models
img: assets/img/21.png
importance: 2
category: Digital Soil Mapping
related_publications: true
---

Machine-learning models can predict **soil organic carbon (SOC)**, but their decisions are often hard to interpret.  
In this project, we mapped SOC across **Germany (250 m)** using **LUCAS** samples and **Google Earth Engine** covariates, then applied a **learning-based post-hoc explanation model** to reveal what different ML models rely on.

### What we did
- Trained multiple SOC models (**Random Forest, Gradient Boosting, DeepForest, Neural Network, Ridge**).
- Used **HLS (Landsat–Sentinel)** imagery plus **soil, climate, vegetation, and topography** predictors from GEE.
- Learned feature importance via an explainer that measures prediction-error change when inputs are masked.

### Key findings 
- **Tree-based models** mainly relied on **topography** (e.g., elevation and terrain derivatives).
- **Neural networks and linear models** relied more on **soil chemistry**, especially **pH** (and related soil-property layers).
- Interpretations are **model-dependent**, so explainability needs an expert-guided workflow.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/21.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Learning-based post-hoc explanations of SOC mapping models across Germany.
</div>

---

## Why it matters
Explainable SOC mapping helps connect predictions to real soil processes and supports more transparent, defensible decisions for carbon policy and land management.

> Paper: *Towards Explainable AI: Interpreting Soil Organic Carbon Prediction Models Using a Learning-Based Explanation Method* (European Journal of Soil Science, 2025).