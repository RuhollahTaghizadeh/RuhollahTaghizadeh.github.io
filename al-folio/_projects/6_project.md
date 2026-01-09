---
layout: page
title: Pedodiversity
description: Spatial scale flips the pedodiversity–elevation relationship
img: assets/img/25.png
importance: 4
category: Land Degradation and Soil Quality Assessment
related_publications: true
---

Pedodiversity (soil diversity) is shaped by soil-forming factors such as climate, vegetation, and relief—yet **its relationship with elevation is often reported inconsistently** (positive in some studies, negative in others). A major reason is **spatial scale**: changing spatial extent and resolution can fundamentally change the observed relationship.

In this study, we show that the **pedodiversity–elevation relationship in semi-arid Botswana is strongly scale-dependent**, even **changing sign** from negative (national) to positive (local).

### What we did
- Compiled **~2060 soil class observations** across Botswana (AfSIS + BRIMP legacy data).
- Mapped soil classes at **90 m** using **Random Forest** within a **SCORPAN** DSM framework.
  - Model validation: **nested cross-validation**
  - Accuracy: **OA = 56.2 ± 3.3%**, **Kappa = 39.7 ± 4.6%**
- Converted the soil class map into a continuous **pedodiversity surface** using **Rao’s quadratic entropy (RaO’s Q)** with a moving window.
- Assessed pedodiversity–elevation relationships across:
  - **Spatial extents:** national (Botswana), **Central district**, **Southern district**
  - **Spatial resolutions:** **90 m, 900 m, 9000 m, 90,000 m**
- Modelled relationships with interpretable statistics:
  - **GLM** (Gaussian)
  - **GWR** (local structure/correlation)
  - Verified patterns with **Spearman correlation**

### Key findings
- **National scale:** pedodiversity vs elevation shows a **negative linear trend** (higher elevation → lower pedodiversity).
- **Local scale (Southern district):** the relationship becomes **positive** (higher elevation → higher pedodiversity).
- **Resolution matters a lot:** the strength of the relationship changes markedly with aggregation.
  - Reported **R² ranges** (GLM) show major scale effects:
    - National: **~0.0005–0.017**
    - Central: **~0.007–0.015**
    - Southern: **~0.061–0.65**
- Coarser resolutions can **inflate apparent relationships** via spatial averaging and may produce **overly optimistic conclusions**, especially at small extents.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/25.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Workflow: RF soil class mapping (90 m) → RaO’s Q pedodiversity → multi-scale aggregation (extent × resolution) → GLM/GWR to quantify scale-dependent pedodiversity–elevation relationships.
</div>

---

## Why it matters
This paper shows that **scale is not a technical detail—it can change the scientific conclusion**. For dryland soil management and conservation, it implies:
1) interpret pedodiversity–environment relationships **only at the scale they’re intended for**,  
2) avoid transferring national-scale conclusions directly to local planning, and  
3) choose resolutions that match the decision context (coarse grids can mislead).

> Paper: *Spatial scale drives pedodiversity-elevation relationship in Botswana* (Geomatica, 2024). DOI: 10.1016/j.geomat.2024.100037
