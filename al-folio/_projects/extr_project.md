---
layout: page
title: Extrapolation
description: Tests model generalization across regions and scales, mapping where predictions extrapolate and where uncertainty increases.
img: assets/img/extra_polation.png
importance: 1
category: Digital Soil Mapping
related_publications: true
---

This project focuses on whether spatial prediction models remain reliable when applied beyond their training conditions—across new regions, scales, and covariate combinations. We use spatially robust validation designs (blocked CV, region holdouts) and diagnose where models extrapolate outside the training “applicability domain.” Outputs include prediction maps plus extrapolation-risk or similarity layers that show where results are well supported and where uncertainty should be higher. The aim is more trustworthy soil mapping under real deployment scenarios.

**Main focus**
- Improve generalization of soil models across space, scale, and data shifts.
- Detect and communicate extrapolation risk and applicability domain limits.
- Support safer use of maps in unsampled or novel environments.

**Objectives**
1. Test model transfer with spatial validation and region-based holdouts.
2. Map covariate coverage and identify out-of-distribution prediction zones.
3. Deliver prediction + extrapolation-risk layers to guide interpretation/sampling.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
{% include figure.liquid loading="eager" path="assets/img/extra_polation.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------




## Papers (selected)

### Paper 1 — **Covariate Transferability for Cropland SOC Prediction**
[DOI](https://doi.org/10.3390/rs15040876)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p13.png" title="Paper 1 GA" class="img-fluid rounded z-depth-1" %}

<br><br>

---

### Paper 2 — **Model Transferability Using Sentinel and Terrain Covariates**
[DOI](https://doi.org/10.3390/rs14235909)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p14.png" title="Paper 2 GA" class="img-fluid rounded z-depth-1" %}

<br><br>

---

### Paper 3 — **Semi-Supervised Learning for Spatial Extrapolation**
[DOI](https://doi.org/10.1016/j.geoderma.2022.116094)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p15.png" title="Paper 3 GA" class="img-fluid rounded z-depth-1" %}

<br>


------------------------------------------------------------------------
