---
title: Soil Spectroscopy
author: Ruhollah Taghizadeh
date: "2021-06-24T00:00:00Z"
slug: Predicting weathering indices
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
  url:  https://www.sciencedirect.com/science/article/abs/pii/S0341816221002952
subtitle: 'Predicting weathering indices in soils using FTIR spectra and random forest models'
summary: 'The main goals of this work were to assess the suitability of different indices to determine soil weathering, and to predict weathering indices using Fourier Transform Mid-infrared (FTIR) spectroscopy and Random Forest models. The important spectral bands for prediction were those related to the presence of smectitic clays, which indicates that weathering is related to the alteration of primary minerals and the neoformation of smectites.'

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
Although there are some examples relating FTIR spectra and WI through PLSR, the potential use of RF to estimate the variability of soil weathering indices from a limited number of samples has not been investigated. Thus, the main goal of this paper was to evaluate the intensity of weathering and alteration of soils in the Miandoab county, West Azerbaijan, Iran, using different weathering indices and to examine the suitability of FTIR spectroscopy and RF model for predicting different weathering indices as a rapid and inexpensive technique.

## Study area

The study area is situated in Miandoab county, West Azerbaijan Province, Iran, and covers approximately 5000 ha

![](fig1.png)

## Spectral model development for weathering indices

A chemometric model was applied to detect relations between the weathering indices and FTIR spectra, and to recognize the most relevant spectral bands for this purpose. The process consisted on fitting a RF model with weathering indices as dependent variables and spectral data as predictors. 

## Weathering indices

All twelve profiles were quite similar in terms of weathering despite the fact that they belong to different soil groups. The CIA and CIW indices had the same pattern, and resembled closely each other in all profiles.

![](fig2.png)

## FTIR spectra

FTIR spectra are good predictors of soil composition, since both inorganic and organic soil components have a distinctive signature in the MIR region of the spectra.

![](fig3.png)

## Modeling weathering indices using FTIR data

Transmission MIR spectra of the soil samples were used as predictors of the weathering indices using RF models. Result indicates the prediction accuracy of the RF models on calibration and validation data for all the indices. From the results obtained with the validation set, it can be observed that not all the models had the same performance.

![](fig4.png)

In addition to the capability to predict the weathering indices using spectral data, the RF models identified the most important spectral bands for the estimation of each weathering index. 

![](fig5.png)

## Conclusion

The main goal of this study was to analyze the weathering conditions of the most representative soils of West Azerbaijan, Northern Iran, using chemical indices, and to demonstrate the suitability of FTIR spectra and RF to predict these weathering indices and to identify the major soil components related to soil weathering. The results showed that the soils in the study area are at an early stage of development and fairly homogeneous in terms of weathering. From all the indices, CIA, CIW, MIA and V were the most suitable to evaluate the weathering intensity, and the combination of FTIR spectra and RF models allowed their prediction with high accuracy. In addition to the predictions, the RF models provided valuable information on the most important weathering processes these indices were describing, which are related to the alteration of K-bearing minerals and the relative increase of smectites in these soils.
