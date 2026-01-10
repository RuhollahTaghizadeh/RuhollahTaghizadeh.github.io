---
layout: page
title: Land Suitability with Machine Learning
description: Learns suitability patterns from soil and environmental constraints, producing spatial suitability maps and key limiting factors.
img: assets/img/landsuitability_map.png
importance: 1
category: Land Degradation & Soil Quality
related_publications: true
---

This project produces land suitability maps using machine learning to capture complex interactions among soil, terrain, and climate constraints. We combine soil and environmental covariates (e.g., texture/soil limitations, SOC, salinity risk, pH/carbonates, slope, climate variables) to predict suitability classes or continuous scores. Spatially informed validation ensures realistic generalization for mapping. Outputs include suitability maps, key limiting-factor summaries, and optional confidence layers for planning and management.

**Main focus**
- Data-driven land suitability mapping beyond fixed threshold/rule methods.
- Identify limiting factors that drive low suitability and management needs.
- Produce decision-ready suitability maps with realistic validation.

**Objectives**
1. Compile suitability targets and constraint covariates for modelling.
2. Train ML models and evaluate with spatially robust validation.
3. Deliver suitability maps + limiting-factor summaries for land-use decisions.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
{% include figure.liquid loading="eager" path="assets/img/landsuitability_map.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------
