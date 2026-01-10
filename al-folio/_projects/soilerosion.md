---
layout: page
title: Soil Erosion with Machine & Deep Learning
description: Detects erosion and deposition features from imagery using ML/CNN segmentation, producing high-resolution hotspot maps.
img: assets/img/erosion-map.png
importance: 1
category: Land Degradation & Soil Quality
related_publications: true
---

This project uses machine learning and deep learning to detect and map soil erosion and deposition features from high-resolution imagery. CNN-based segmentation learns erosion signatures (e.g., rills, channels, depositional patterns) directly from images, while covariates such as terrain derivatives add process context. Models are evaluated across space and time to ensure robustness under real conditions. Outputs include high-resolution erosion hotspot maps that support targeted conservation planning.

**Main focus**
- Automated detection of erosion/deposition features from imagery.
- High-resolution hotspot mapping for monitoring and intervention targeting.
- Robust evaluation to ensure generalization across landscapes and dates.

**Objectives**
1. Build labeled/annotated erosion datasets from UAV/satellite imagery.
2. Train ML/CNN segmentation models with spatially realistic validation.
3. Produce erosion/deposition maps to prioritize soil conservation actions.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
{% include figure.liquid loading="eager" path="assets/img/erosion-map.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------
