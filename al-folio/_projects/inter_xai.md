---
layout: page
title: Interpretable & Explainable AI in Soil Science
description: Explains why models predict patterns by highlighting key drivers and local effects.
img: assets/img/inter_xai.png
importance: 3
category: Digital Soil Mapping
related_publications: true
---

This project makes machine learning for soil science more transparent by adding interpretability and explainability throughout the modelling pipeline. High-performing models (ensembles and deep learning) can be difficult to trust if they cannot communicate which variables drive predictions or whether learned relationships align with soil–landscape understanding. Here, we pair predictive mapping with explainable AI methods that deliver global explanations (overall importance of terrain, climate, land cover, geology, and remote-sensing variables) and local explanations (why a specific location is predicted high or low). These explanations help connect model outputs to plausible processes—such as erosion–deposition effects on SOC, topographic controls on moisture and salinity accumulation, or carbonate and parent material influences on pH—and they support clearer scientific interpretation rather than “maps only.” The project also checks explanation stability under spatial validation, reducing the risk of reporting spurious drivers caused by sampling bias or spatial autocorrelation. Deliverables include prediction maps, uncertainty/confidence layers when possible, and explanation products (importance summaries, effect plots, driver maps) designed for communication to researchers and stakeholders. Ultimately, the project supports responsible AI adoption by improving transparency, comparability, and decision confidence in soil modelling.

------------------------------------------------------------------------

## Graphical abstract

:::: {.row .justify-content-sm-center}
::: {.col-sm-10 .mt-3 .mt-md-0}
```         
{% include figure.liquid loading="eager" path="assets/img/inter_xai.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
```
:::
::::

::: caption
Graphical abstract summarizing the workflow and key results.
:::

------------------------------------------------------------------------

