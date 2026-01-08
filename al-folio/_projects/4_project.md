---
layout: page
title: SOC from Sentinel-2 Time Series
description: Temporal SWIR for accurate soil organic carbon mapping
img: assets/img/23.png
importance: 1
category: Soil Sensing & Remote Observation
related_publications: true
---

Soil Organic Carbon (SOC) is a key indicator for soil fertility, food security, and climate mitigation, but **lab-based SOC measurements are slow, expensive, and hard to scale**.  
Most remote-sensing approaches rely on **single-date imagery**, which often fails to capture SOC’s complex and condition-dependent spectral response—typically limiting accuracy.

This study introduces a **time-series feature engineering workflow** for SOC estimation using only **Sentinel-2 imagery**, centered on **Band 11 (SWIR, ~1610 nm)**—a spectral region sensitive to SOC-related absorption features.

### What we did
- Collected **91 topsoil samples (0–10 cm)** in summer 2019 (Sanandaj, Iran) and analyzed SOC using **Walkley–Black**.
- Built Sentinel-2 predictors exclusively from imagery:
  - A **synthetic median composite** (summer 2019) of Sentinel-2 surface reflectance + spectral indices.
  - A **B11 time series** (20 acquisitions during the sampling period).
- Extracted high-level temporal features from the **B11 time series** using:
  - **PCA** (first 5 principal components)
  - **ICA** (independent components + kurtosis-based component selection)
- Trained and compared four ML models (**RF, GBRT, XGBoost, LightGBM**) under four scenarios:
  - **S#1:** single-time features only  
  - **S#2:** S#1 + **Genetic Algorithm (GA)** feature selection  
  - **S#3:** single-time + **B11 time-series PCA/ICA features**  
  - **S#4:** S#3 + **GA feature selection** (best pipeline)

### Key findings
- Adding **time-series B11 PCA/ICA features** improved accuracy by about **+0.11 R²** (S#3 vs S#1).
- Applying **GA feature selection** added about **+0.05 R²** (S#4 vs S#3).
- Best performance was achieved with **XGBoost in S#4**: **R² = 0.891** (10-fold CV).
- Permutation importance indicated **PCA-derived temporal features** were the most informative group, outperforming raw spectral bands and indices.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/23.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Pipeline for SOC estimation using Sentinel-2 only: B11 time-series → PCA/ICA temporal features → GA feature selection → boosted ML models.
</div>

---

## Why it matters
This work shows that **high-accuracy SOC mapping is possible using only multispectral Sentinel-2 data** by:
1) targeting an SOC-sensitive SWIR band (**B11**),  
2) exploiting the **temporal dimension** (time series instead of a single image), and  
3) using **feature extraction + selection** to produce compact, powerful predictors.

> Paper: *Estimating soil organic carbon using time series Band 11 (SWIR) of multispectral Sentinel-2 satellite images and machine learning algorithms* (Remote Sensing Applications: Society and Environment, 2025).
