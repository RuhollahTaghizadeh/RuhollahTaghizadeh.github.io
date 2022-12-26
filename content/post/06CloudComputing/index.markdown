---
title: Big Geospatial Data Analysis
author: Ruhollah Taghizadeh
date: "2021-01-24T00:00:00Z"
slug: High resolution middle eastern soil attributes
categories: 
tags: []
external_link: ""
image:
  caption: 
  focal_point: Smart
links:
- icon: photo-video
  icon_pack: fa
  name: DOI
  url:  https://www.sciencedirect.com/science/article/abs/pii/S0016706120326458
subtitle: 'High resolution middle eastern soil attributes mapping via open data and cloud computing'
summary: 'There are no detailed soil maps covering a large extension of the Middle East region, especially for calcium carbonate content. Thus, we used topsoil data for mapping near 3,338,000 square km of the Middle East. We used covariates obtained from RS data and random forest algorithm. After training RF we used the optimal ones for making spatial predictions of topsoil attributes and associated uncertainties at 30 m resolution.'

authors: 
  - admin
lastmod: '2022-08-17T13:21:49-07:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---
{{< toc >}} 

## Motivation
<style>
body {
text-align: justify}
</style>
At the moment, there are no detailed maps covering a large extension of the Middle East region using bare topsoil reflectance or traditional environmental controllers—e.g. geological maps, climate data, and relief attributes. Indeed, there is no work that mapped calcium carbonates from middle eastern soils, and the available maps for clay, silt, sand, organic matter, and pH present coarser resolution than the proposed in this study. Thus, we aimed to map soil attributes at 0–20 cm depth with 30 m spatial resolution in a part of the Middle East region using remote sensing data and RF algorithm and provide spatial uncertainties.

## Methods

The DSM framework was implemented in this study.

![](fig1.png)

## Importance of covariates

Although several covariates had a low linear correlation with soil observations, they were all relatively important for DSM of topsoil attributes, ranging from 4% to 98%. Annual precipitation, the annual range of temperature, and elevation were the most important covariates (greater than31%) driving the spatial variability of topsoil attributes in the Middle East region

![](fig2.png)

## Performance of spatial models

In overall, the R2 values of the predictions of topsoil attributes from the testing set ranged from 0.40 to 0.66, indicating that the models explained around 40–66% of the variation present in topsoil attributes.

## Mapping of soil properties

Despite considerable local spatial variation on soil attributes patterns, we observed that from northwest to southeast clay, silt and OC content gradually decreased while the amount of sand, CaCO3, and pH increased in the topsoil. This occurred across a precipitation gradient, as suggested by the correlation between soil observations and annual precipitation.

![](fig3.png)

## Conclusion

The DSM framework implemented in this study—e.g. the use of cloud computing freely available in GEE for covariates obtaining, bootstrapping and results assessment— overcame some limitations related to computing infrastructure for large-extent applications. In fact, the excellent quality of the soil dataset—measurements, spatial location and distribution—, the strength of covariates—high explanatory power—that accurately represented soil spatial patterns, and the RF’s consistency, were crucial to the success of this work.