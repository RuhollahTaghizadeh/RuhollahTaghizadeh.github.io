---
layout: page
title: Spatial Prediction of Soils
description: Maps soil properties from samples using covariates and spatial validation, producing high-resolution predictions with confidence.
img: assets/img/spatial_soil.png
importance: 1
category: Digital Soil Mapping
related_publications: true
---

This project converts point-based soil observations into continuous, high-resolution maps that capture soil variability more realistically than traditional polygon mapping. It integrates soil measurements (e.g., SOC, texture, pH, salinity-related indicators, CaCO₃, CEC, and hydraulic properties) with environmental covariates (terrain, climate, land cover, geology, and remote sensing) to train machine-learning models that learn nonlinear soil–landscape relationships. Performance is evaluated using spatially informed validation to ensure realistic generalization, and outputs can include uncertainty/confidence layers to highlight where predictions are reliable and where additional sampling is most valuable.

**Main focus**
- Robust and scalable spatial prediction of multiple soil properties.
- High-resolution soil maps for management and environmental applications.
- Reliability-aware outputs (confidence/uncertainty) for trustworthy decisions.

**Objectives**
1. Integrate multi-source covariates with soil observations to build prediction-ready datasets.
2. Train and evaluate ML models using spatially structured validation to avoid optimistic bias.
3. Produce prediction maps (and optional confidence layers) that support decision-making and sampling design.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
{% include figure.liquid loading="eager" path="assets/img/spatial_soil.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------
