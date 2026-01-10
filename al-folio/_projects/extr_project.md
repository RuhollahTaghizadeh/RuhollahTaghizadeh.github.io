---
layout: page
title: Transferability & Extrapolation in Spatial Prediction
description: Tests model generalization across regions and scales, mapping where predictions extrapolate and where uncertainty increases.
img: assets/img/extra_polation.png
importance: 1
category: Digital Soil Mapping
related_publications: true
---

This project focuses on whether spatial prediction models remain reliable when applied beyond their training conditions—across new regions, different scales, or novel covariate combinations. In soil mapping, samples are often clustered and landscapes vary widely, so models can look accurate under random splits yet fail in true extrapolation settings. We address this by using spatially robust evaluation designs (blocked/clustered cross-validation, region holdouts) and by running experiments that vary sampling density, sample size, and spatial extent to mimic real deployment. A core component is diagnosing the “applicability domain”: identifying where target locations fall within the covariate space supported by training data versus where they are out-of-distribution. These diagnostics are paired with strategies to improve generalization, such as careful covariate selection, simplifying overly complex models, using ensembles to stabilize predictions, and leveraging semi-supervised ideas when appropriate. Outputs include prediction maps plus extrapolation-risk or similarity layers that communicate where predictions are supported and where uncertainty should be higher. This helps users prioritize new sampling, interpret maps cautiously in novel areas, and design workflows that are more dependable for operational mapping.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
```         
{% include figure.liquid loading="eager" path="assets/img/extra_polation.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
```
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------

