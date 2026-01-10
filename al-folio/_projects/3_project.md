---
layout: page
title: Erosion-SAM
description: Segment Anything Model for water-erosion segmentation
img: assets/img/22.png
importance: 3
category: 
related_publications: true
---

Soil erosion by water removes fertile topsoil and causes major economic losses, but **training data for erosion mapping is scarce** and manual interpretation of orthophotos is slow.  
In this project, we introduce **Erosion-SAM**: a **fine-tuned Segment Anything Model (SAM)** for **automatic pixel-level segmentation** of erosion and deposition features in **20 cm** aerial orthophotos.

### What we did
- Built a labeled dataset of **405 agricultural fields** (grassland, vegetated cropland, bare cropland) with expert **manual erosion/deposition masks**.
- Fine-tuned **SAM (ViT-B)** by adapting the **mask decoder** (transfer learning) to erosion patterns.
- Compared two preprocessing strategies (**resizing vs. cropping**) and tested an enhanced workflow that uses **minimal point prompts** at inference.

### Key findings
- All fine-tuned models **outperformed the original SAM**, which tended to **overestimate erosion** (many false positives).
- The best results came from **resizing + user point prompts**, especially in **grassland** *(recall 0.90, precision 0.82, Dice 0.86, IoU 0.75)*.
- Predicted field-scale erosion severity ratios matched ground truth strongly, with **R² up to 0.93** for the prompt-enhanced resizing workflow.

---

## Graphical abstract
<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/22.png" title="Graphical abstract" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Erosion-SAM workflow: fine-tune SAM for pixel-level erosion/deposition segmentation from high-resolution orthophotos.
</div>

---

## Why it matters
Erosion-SAM enables **scalable, consistent erosion monitoring** at high spatial and temporal resolution, producing training data for ML-based erosion models and supporting practical applications like **risk assessment, land management, and insurance solutions**.

> Paper: *Erosion-SAM: Semantic segmentation of soil erosion by water* (Catena, 2025).
