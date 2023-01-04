---
title: Multisensor Remote Sensing Data 
author: Ruhollah Taghizadeh
date: "2022-10-24T00:00:00Z"
slug: Digital Soil Texture Mapping and Spatial Transferability of Machine Learning Models
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
  url:  https://www.mdpi.com/2072-4292/14/23/5909
subtitle: 'Digital Soil Texture Mapping and Spatial Transferability of Machine Learning Models Using Sentinel-1, Sentinel-2, and Terrain-Derived Covariates'
summary: 'This study examined the capability of ML models in estimating soil texture fractions using different combinations of remotely sensed data from Sentinel-1, Sentinel-2, and terrain-derived covariates across two regions in Germany. We tested the predictive power of three different ML models: the random forest, the support vector machine, and extreme gradient boosting coupled with the remote sensing data covariates.'
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

## Video Abstract
<center>

{{< youtube FADH_3RAzoc >}}

</center>

## Motivation
<style>
body {
text-align: justify}
</style>
Machine learning (ML) models are more efficient than traditional statistical models when multisource datasets are applied. However, findings indicate that the prediction results from different models might vary substantially when the same data source is applied. Therefore, when dealing with multisource datasets in areas offering meaningful intrinsic and extrinsic heterogeneity, it is necessary to assess different models’ abilities to select the best-performing model with the highest accuracy and the lowest uncertainty. Thus, an approach that simultaneously uses multisensor RS data combined with environmental covariates may allow soil texture estimates with a better accuracy at a higher spatial resolution.

## Methods

This study examined the potential effects of RS imagery (S1 and S2) and terrain-derived covariates (TDC) in estimating soil texture fractions (clay, silt, and sand contents) across two contrasting agroecological regions, Kraichgau and the Swabian Alb, in Southwest Germany. In this context, the aims of the present study were (1) to evaluate the performance of ML algorithms, including the random forest—RF, the support vector machine—SVM, and extreme gradient boosting—XGB, in mapping soil texture fractions using S1 and S2 data individually and combined with terrain-derived covariates; (2) to explore the most effective covariates to estimate soil texture fractions; and (3) to evaluate the transferability of predictive models outside of the initial training region in predicting soil texture fractions.

![](fig1.png)

## Sentinel 1

S1 allows full polarimetric imaging, i.e., horizontal transmit and receive (HH), horizontal transmit and vertical receive (HV), vertical transmit and horizontal receive (VH), and vertical transmit and receive (VV), at a resolution of 5–20 m every 12 days. This study used dual-polarized SAR level-1 ground range detected products (VH, VV) in ‘IW’ mode as the original data was at a resolution of 10 m. Multiploidization SAR allows a better understanding of soil surface properties compared only to the backscatter coefficients of a single polarization. Several preprocessing algorithms, including radiometric and geometric correction, speckle filtering, and thermal noise removal, were applied to each SAR image to draw out the backscatter coefficient at any polarization mode. These allow reducing error propagation in the following processes and analyses. 

## Sentinel 2

S2 is a space-borne multispectral spectral imager with a five-day revisit time, which started its mission first in June 2015 as part of the “Copernicus” program. The S2 image comprises 13 spectral bands in the optical domain (VNIR/SWIR) at spatial resolutions of 10, 20, and 60 m. After excluding B1 (Coastal Aerosol), the remaining 11 bands (i.e., B2 (490 nm), B3 (560 nm), B4 (665 nm), B5 (705 nm), B6 (740 nm), B7 (783 nm), B8 (842 nm), B9 (945 nm), B10 (1375 nm), B11 (1610 nm), and B12 (2190 nm)) were extracted for further use.

## Summary of data

Given that the clay content of the field observation in the entire SA region was over 40%, the soils would typically be classified as clay and silty clay textures. There was a wide range of soil texture classes in the SA region, which included 9 out of the 12 possible texture classes. However, the dominant texture classes across both regions were silt loam (27%), silty clay (25%), silty clay loam (22%), and clay (17%). The remaining 10 percent of measured samples represented other soil texture types.

![](fig2.png)

## Variable importance for computational models

The relative importance of predictor covariates differed both by region and by model type. The selected predictors were ordered in the selection process by their influence or by the order in which they were contributed. For example, S2 and TDC explained 17.5% and 82.5% of the sand variation in the SA region, respectively.

![](fig3.png)

## Mapping of soil texture classes

The best model was applied to create the spatial prediction map of soi ltexture fractions, later, the texture classes for both regions. 

![](fig4.png)

![](fig5.png)

## Conclusion

This paper examined the capability of satellite imagery (S1 and S2) and terrain-derived covariates (TDC) in estimating soil texture fractions and evaluated the spatial transferability of three machine learning models. Due to the complexity of the influential factors of soil properties (e.g., intrinsic and extrinsic) across the study regions, model performance was not consistent, even for different models in the same area.