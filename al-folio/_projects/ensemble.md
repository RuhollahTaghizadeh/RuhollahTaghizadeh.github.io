---
layout: page
title: Ensemble & Super Learning for DSM
description: Combines multiple ML models (stacking/averaging) to reduce errors and improve stability of soil maps and uncertainty.
img: assets/img/ensemble_dsm.png
importance: 1
category: Digital Soil Mapping
related_publications: true
---

This project improves digital soil mapping by combining multiple models instead of relying on a single algorithm. We train diverse base learners and fuse them using model averaging or Super Learner (stacking) to reduce variance and stabilize predictions across regions, properties, and sampling designs. Evaluation uses spatially informed validation to ensure realistic performance and to avoid optimistic bias. Outputs include improved soil maps and, where feasible, uncertainty indicators based on ensemble spread.

**Main focus**
- Reduce single-model risk by combining complementary learners.
- Improve robustness and stability of soil predictions across settings.
- Provide reliability signals using ensemble-based uncertainty summaries.

**Objectives**
1. Train a diverse set of base models for key soil properties.
2. Combine models via stacking/averaging under spatially robust validation.
3. Deliver improved prediction maps plus uncertainty from ensemble behavior.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
{% include figure.liquid loading="eager" path="assets/img/ensemble_dsm.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------
