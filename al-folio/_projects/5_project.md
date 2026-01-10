---
layout: page
title: Machine Learning in Archaeology
description: Systematic Review
img: assets/img/24.png
importance: 4
category: 
related_publications: true
---

Machine learning (ML) is rapidly reshaping archaeological research, but the field is scattered across many subdomains (remote sensing, artefact studies, predictive modelling, taphonomy), often using inconsistent data standards and evaluation practices.  
This review consolidates the evidence base and highlights where ML is effective today—and where methodological gaps still limit reliability and interpretability.

The paper synthesizes **135 peer-reviewed studies (1997–2022)** and extracts structured information about **tasks, data sources, algorithms, validation strategies, and research trends**, providing a roadmap for more reproducible and transparent archaeological ML.

### What we did
- Performed a **systematic literature review** of **135 journal articles** covering ML applications in archaeology (1997–2022).
- Categorized studies by **problem type**, including:
  - **automatic structure detection** (e.g., features in imagery/point clouds),
  - **artefact classification** (shape, texture, typology),
  - **archaeological predictive modelling** (site likelihood),
  - **taphonomy / preservation assessment**,
  - **architectural classification & reconstruction**.
- Summarized algorithm usage patterns (e.g., **ANNs, ensembles**, and other supervised methods).
- Synthesized reported **data modalities** (satellite/UAV imagery, LiDAR/photogrammetry, geophysics, lab/imaging data, tabular predictors).
- Compiled common **validation practices** and recurring weaknesses (e.g., small sample sizes, limited external validation, class imbalance, interpretability gaps).

### Key findings
- Publications show a **strong rise after ~2019**, indicating a recent acceleration of ML adoption in archaeology.
- **Supervised learning dominates** across applications, especially for detection and classification tasks.
- Reported use is concentrated around **neural networks and ensemble learning**, reflecting their flexibility with high-dimensional data (imagery/3D).
- Many studies rely on **limited geographic transfer testing**, meaning models may not generalize well across landscapes, sensors, or archaeological contexts.
- The review emphasizes the need for **better benchmarking, uncertainty reporting, and explainability** to support trustworthy archaeological interpretation.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/24.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Systematic review workflow and taxonomy of ML applications in archaeology: tasks → data types → algorithms → validation patterns → research roadmap.
</div>

---

## Why it matters
This review helps the community move from “cool demos” toward **robust, reusable ML in archaeology** by:
1) clarifying what tasks ML is most used for today,  
2) identifying common methodological pitfalls (generalization + validation), and  
3) motivating **transparent, explainable, and benchmarked** workflows for future studies.

> Paper: *Machine Learning Applications in Archaeological Practices: A Review* (Journal of Computer Applications in Archaeology, 2025).
