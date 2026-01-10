---
layout: page
title: Land Suitability Mapping
description: Integrating TOPSIS and Random Forest
img: assets/img/27.png
importance: 4
category: 
related_publications: true
---

Land suitability assessment is central to sustainable crop planning because it links **soil**, **terrain**, **climate**, and management constraints to expected productivity.  
This study evaluates wheat suitability in the **Gavshan region (western Iran)** by combining **advanced multi-criteria decision-making (MCDM)** with **machine learning (ML)**—and validates suitability scores against **measured wheat yield**.

### What we did
- **Field campaign:** 70 soil profiles selected using a **geomorphology map** and stratified random sampling; profiles described and lab-analyzed.
- **Criteria:** multiple diagnostic attributes were screened; **8 key attributes** were selected for wheat suitability following Sys-style land evaluation.
- **Weighting:** criteria weights derived objectively using **Shannon’s entropy**.
- **MCDM suitability scoring:** compared three methods:
  - **TOPSIS**
  - **Grey Relational Analysis (GRA)**
  - **Simple Additive Weighting (SAW)**
- **Validation with yield:** wheat yield measured at each profile (1 m² harvest) and correlated with suitability scores.
- **Spatial mapping (DSM):** suitability scores were spatially predicted using **Random Forest** with environmental covariates:
  - terrain derivatives (10 m DEM),
  - Landsat 8 bands/indices (30 m),
  - geomorphology classes,
  resampled to a common 30 m grid.
- **Spatial diagnostics:** spatial autocorrelation used to confirm spatial agreement between key criteria, suitability maps, and yield.

### Key findings
- **Most influential criteria** (entropy weights):
  - **Slope** (highest)
  - **Organic carbon (OC)**
  - **Cation exchange capacity (CEC)**
- **Agreement with yield (correlation):**
  - **TOPSIS:** 0.74 (best)
  - **GRA:** 0.72
  - **SAW:** 0.57
- **RF mapping performance (test set):**
  - Models achieved strong predictive skill (R² up to ~0.88 depending on the MCDM target surface).
- **Spatial interpretation:**
  - High suitability zones concentrated mainly in the **central part** of the study area, associated with:
    - gentle slopes (< ~5%),
    - higher CEC and OC,
    - higher observed yields.
  - TOPSIS and GRA classified **larger areas as “good”** than SAW, which tended to assign more “moderate/weak” suitability.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/27.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Workflow: soil profiles + yield → entropy-weighted MCDM (TOPSIS/GRA/SAW) → validation vs. yield → Random Forest DSM using DEM + Landsat + geomorphology → suitability maps + spatial autocorrelation diagnostics.
</div>

---

## Why it matters
This work shows that combining **MCDM** (transparent, decision-oriented suitability scoring) with **ML-based spatial modeling** (pattern learning from complex covariates) can produce **more reliable, mappable suitability surfaces** for crop plannin
