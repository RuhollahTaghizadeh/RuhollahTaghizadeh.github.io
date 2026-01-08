---
title: "Spatial Pedology and Geomorphology"
category: "Courses"
importance: 1
description: "Master’s-level course introducing digital soil mapping workflows and machine-learning methods for spatial prediction of soil properties."
---

**Level:** Master’s  
**Institution:** University of Tübingen  
**Department:** Geosciences (Soil Science & Geomorphology)  
**My contribution:** Digital Soil Mapping (DSM) module (lectures + practical sessions)

## Overview
This course introduces students to spatial approaches in pedology and geomorphology, with a dedicated module on **Digital Soil Mapping (DSM)**. My teaching focuses on how modern statistical learning and geospatial workflows can be used to produce reproducible, interpretable, and uncertainty-aware soil maps. The module combines **theoretical foundations** with **hands-on training** using **R** and point-based soil observations.

## Learning objectives
By the end of the DSM module, students will be able to:
- understand the **DSM workflow** from problem definition to map production and reporting
- explain core **machine-learning concepts** relevant to environmental modelling (bias–variance trade-off, overfitting, validation)
- implement and compare common modelling approaches for DSM, including:
  - **Decision Trees** and **Random Forest**
  - basic **geostatistical concepts** and spatial structure in residuals
- prepare and engineer covariates for spatial prediction (terrain, remote sensing, climate/land use where available)
- evaluate model performance using appropriate strategies (e.g., cross-validation and spatial considerations)
- produce **soil property maps** and communicate **prediction uncertainty** in a transparent way

## Teaching format
The module is structured in two complementary parts:

### 1) Theoretical sessions
Topics include:
- DSM concepts and the role of environmental covariates (e.g., SCORPAN-inspired thinking)
- supervised learning for spatial prediction: regression and model generalization
- model interpretation: variable importance and response patterns (intro level)
- spatial dependence and why it matters in validation and uncertainty assessment
- uncertainty quantification and good practice in reporting DSM results

### 2) Practical sessions (R-based)
Students work with point-based soil datasets and covariates to:
- clean and explore soil observations (EDA, outliers, transformations where needed)
- build predictive models (baseline models → Random Forest / tree-based approaches)
- validate models and compare alternatives using robust performance metrics
- generate prediction grids and create maps
- summarize uncertainty and limitations, and document a reproducible workflow

## Key topics (DSM module)
- Digital Soil Mapping workflow (from data to map)
- Machine learning fundamentals for environmental prediction
- Decision Trees, Random Forest, and model tuning (intro)
- Geostatistical concepts (spatial autocorrelation, residual structure)
- Model evaluation and spatial validation considerations
- Uncertainty quantification and communication

## Tools
- **R** (data handling, modelling, validation, mapping)
- Common spatial packages (depending on course setup): `sf`, `terra/raster`, `caret`/`mlr3`, visualization tools

---
If you are a student in this course and need access to scripts, data links, or assignment instructions, please contact me.
