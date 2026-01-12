---
layout: page
title: Neural Networks for Soil Mapping
description: Uses CNN/deep models to learn spatial patterns from gridded covariates, improving soil predictions with confidence layers.
img: assets/img/deep_learning.png
importance: 1
category: Digital Soil Mapping
related_publications: true
---

This project applies deep learning (especially CNNs) to spatial prediction of soil properties from stacked gridded covariates such as terrain derivatives and remote-sensing layers. CNNs learn multiscale spatial patterns and neighborhood context directly from these layers, helping capture complex soil–landscape relationships that may be missed by hand-crafted features. Models are trained with regularization and evaluated with spatially structured validation to ensure realistic generalization to new areas. Deliverables include high-resolution soil prediction maps and, where feasible, confidence/uncertainty information to communicate reliability.

**Main focus**
- Learn spatial patterns from gridded covariates using CNN-based models.
- Improve mapping performance for complex, nonlinear soil relationships.
- Provide reliable outputs through spatial validation and confidence layers.

**Objectives**
1. Build covariate “image stacks” that preserve spatial context for deep learning.
2. Train CNN/deep models with spatial validation to test real-world generalization.
3. Produce soil maps (and confidence layers) that support applied soil decisions.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
{% include figure.liquid loading="eager" path="assets/img/deep_learning.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------



## Papers (selected)

### Paper 1 — **Multi-Task CNN Soil Texture Mapping**
[DOI](https://doi.org/10.1016/j.geoderma.2020.114552)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p4.png" title="Paper 1 GA" class="img-fluid rounded z-depth-1" %}

<br><br>

---

### Paper 2 — **Bio-Inspired ANN Hybrid for Soil Texture Fraction Mapping**
[DOI](https://doi.org/10.3390/rs13051025)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p5.png" title="Paper 2 GA" class="img-fluid rounded z-depth-1" %}

<br><br>

---

### Paper 3 — **Uncertainty Quantification in ANN-Based Mapping of Soils**
[DOI](https://doi.org/10.5194/egusphere-egu23-15495)

<br>

{% include figure.liquid loading="lazy" path="assets/img/p6.png" title="Paper 3 GA" class="img-fluid rounded z-depth-1" %}

<br>


------------------------------------------------------------------------