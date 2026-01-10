---
layout: page
title: Deep Learning for Spatial Prediction
description: Uses deep models to learn spatial patterns from gridded covariates, improving soil predictions.
img: assets/img/deep_learning.png
importance: 2
category: Digital Soil Mapping
related_publications: true
---

This project investigates deep learning—particularly convolutional neural networks (CNNs)—as a next-step approach for digital soil mapping when covariates are available as gridded layers. Soils exhibit spatial structure shaped by geomorphology, hydrology, climate, and management, and these influences appear as patterns in stacked terrain and remote-sensing layers. CNNs are designed to learn spatial features (textures, gradients, multi-scale motifs) directly from such inputs, reducing reliance on hand-crafted feature engineering and enabling models to use neighborhood context around each location. The workflow links soil observations to covariate “image stacks” (e.g., DEM derivatives and satellite-derived bands/indices), trains deep models with regularization to avoid overfitting, and evaluates generalization with spatially structured validation so results reflect real mapping scenarios. Beyond performance, the project emphasizes model understanding through practical explainability tools (feature attributions, saliency-style summaries) and reliability through confidence/uncertainty indicators where feasible. The outputs are high-resolution soil property maps (or class probability maps) that can better capture complex spatial patterns, supporting applications such as soil carbon monitoring, salinity assessment, and precision land management.
---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/deep_learning.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Graphical abstract summarizing the workflow and key results.
</div>


---


