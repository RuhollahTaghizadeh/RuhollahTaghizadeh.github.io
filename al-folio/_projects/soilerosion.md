---
layout: page
title: Soil Erosion
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





## Papers (selected)

### Paper 1 — **Erosion-SAM**
[DOI](https://doi.org/10.1016/j.catena.2025.108954)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p38.png" title="Paper 1 GA" class="img-fluid rounded z-depth-1" %}

<br><br>

---

### Paper 2 — **Erosion Evidence from Soil 13C Patchiness and 15N Uniformity**
[DOI](https://doi.org/10.1016/j.agee.2023.108616)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p39.png" title="Paper 2 GA" class="img-fluid rounded z-depth-1" %}

<br><br>

---

### Paper 3 — **Soil Erosion Mapping**
[DOI](https://doi.org/10.3390/soilsystems3030043)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p40.png" title="Paper 3 GA" class="img-fluid rounded z-depth-1" %}

<br>


------------------------------------------------------------------------



