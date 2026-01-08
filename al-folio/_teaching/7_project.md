---
layout: page
title: SOC Mapping in Germany
description: Ensemble ML to map MAOM and POM
img: assets/img/26.png
importance: 4
category: Digital Soil Mapping
related_publications: true
---

Soil organic matter (SOM) quality—often described through **mineral-associated organic matter (MAOM)**, **particulate organic matter (POM)**, and the **C/N ratio**—controls key soil functions like nutrient cycling, aggregation, and long-term carbon stabilization.  
Yet, these components are typically modeled **separately**, ignoring their **interdependencies**, which can limit interpretation and potentially bias conclusions.

This study delivers **national-scale maps** of **C/N ratio, MAOM, and POM** for German agricultural **topsoils (0–10 cm)** using **ensemble machine learning**, and introduces a **modified regressor chain** to explicitly capture and interpret **nonlinear interactions** between SOM components.

### What we did
- Focused on **German agricultural mineral topsoils (0–10 cm)** from the **German Agricultural Soil Inventory** (≈ **3104 sites** on an ~8 km grid).
- Response variables:
  - **C/N ratio** (from measured SOC and total N via dry combustion).
  - **MAOM and POM** fractions estimated nationally using **NIR spectroscopy** calibrated with density fractionation reference samples.
- Built predictors under **SCORPAN**, harmonized to a **25 m grid** (INSPIRE standard), including:
  - **Soil & parent material** (soil type, pedo-climatic region, hydrological unit, soilscapes)
  - **Climate** (DWD long-term grids)
  - **Land use/cover** (official land use + **Landsat 8** bands + NDVI/NDMI/NDWI composites)
  - **Relief** (EU-DEM derivatives: slope, curvatures, TWI, etc.)
- Trained **three base learners** and combined them via **ensemble averaging**:
  - **RF**, **BRT**, **SVR**
- Used **nested cross-validation** (spatially stratified folds) for tuning + unbiased evaluation.
- Proposed a **modified regressor chain** (hybrid of regressor chains + stacked single-target) to study **MAOM–POM–C/N** dependencies without order-induced bias.
- Interpreted models with **grouped permutation importance** (GPFI/GOPFI), **ALE/PDP**, and **SHAP**.

### Key findings
- Predictive performance (MAPE):
  - **C/N ratio:** **8.2%** (high accuracy)
  - **MAOM:** **14.8%** (good accuracy)
  - **POM:** **28.6%** (reasonable; hardest target, especially for extremes)
- **Soil & parent material** plus **land use/cover** dominated explained variation:
  - ~**75%** of variance explained for **MAOM & POM**
  - ~**50%** for **C/N**
- Spatial patterns:
  - **Northern Germany** tends to show **higher C/N and POM** and **lower MAOM**, consistent with regional soil-texture/soilscape contrasts.
  - Highest uncertainty clustered where extremes occur (notably parts of the northwest).
- The **modified regressor chain** revealed a **nonlinear C/N–SOM relationship**, consistent with **variable decomposition dynamics** and SOM quality differences across regions.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/26.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Workflow: SCORPAN predictors (25 m) → RF/BRT/SVR ensemble models → national maps of C/N, MAOM, POM + uncertainty → modified regressor chain to interpret MAOM–POM–C/N interdependencies.
</div>

---

## Why it matters
This work advances national soil carbon monitoring by:
1) producing **high-resolution (25 m)** maps of SOM quality indicators across Germany,  
2) combining strong prediction with **model-agnostic interpretation**, and  
3) providing an **interpretable multi-target framework** (modified regressor chain) to study **how SOM fractions and C/N co-vary**—instead of treating them as isolated targets.

> Paper: *Spatial Prediction of Organic Matter Quality in German Agricultural Topsoils* (Agriculture, 2024). DOI: 10.3390/agriculture14081298
