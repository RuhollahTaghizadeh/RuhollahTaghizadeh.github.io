---
title: Dust Pollution and Shapley Values
author: Ruhollah Taghizadeh
date: "2021-04-24T00:00:00Z"
slug: Dust Prediction and Shapley Values
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
  url:  https://www.sciencedirect.com/science/article/pii/S1470160X21009523
subtitle: 'Determining the contribution of environmental factors in controlling dust pollution during cold and warm months of western Iran using different data mining algorithms and game theory'
summary: 'The specific objectives of this study were (1) to assess the usefulness of the DNN for predicting dust events in comparison to MLR, GP, XGB, and RF; (2) to examine the interpretability of DNN models using Shapley values; and (3) to determine the contribution of environmental factors in controlling dust events during the cold and warm months of western Iran. We observed that the DNN model was most effective in predicting DSI.'

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
The specific objectives of this study were (1) to assess the usefulness of the DNN for predicting dust events in comparison to MLR, GP, XGB, and RF; (2) to examine the interpretability of DNN models using Shapley values; and (3) to determine the contribution of environmental factors in controlling dust events during the cold and warm months of western Iran.

## Study area

Our study area is western Iran. Seasonal variations in wind erosion events in the region are notable. Most of these events occur in the summer when strong Shamal winds blow and little rain falls.

![](fig1.png)

## Methods

The workflow used to carry out this study is summarized in the figure. 

![](fig2.png)

## Dust storm index (DSI)

The DSI is an indicator that is used in monitoring wind erosion from local- to global-scales. The index is calculated based on synoptic records that are assigned for dust events.

![](fig3.png)

## Efficiency of ML models for CMDSI and WMDSI prediction

The observed and predicted values of the DSI using the MLR, GP, XGB, RF, and DNN for the cold and warm months of the study period are shown. Overall, our findings showed that DNN was an effective modelling approach for western Iran—regardless of the season.

![](fig4.png)

## Contribution of explanatory variables

Identifying and prioritizing the factors that control dust events is important in reducing their adverse impacts in different regions. After identifying that DNN was the most accurate model in predicting CMDSI and WMDSI, the importance of predictive variables, relative to each other, was determined using game theory. In the method, Shapley values, which compute the importance of a predictor by measuring how much the performance of a model changes with and without the predictor. The variable importance results for CMDSI and WMDSI are shown. In the y-axis, the predictors were sorted according to the Shapley values whereby higher values represent greater importance.

![](fig5.png)

## Conclusion

A methodology framework was proposed for identifying the environmental controls of dust pollution in western Iran using game theory and different machine-learning models. Here, we observed that the DNN model was most effective in predicting DSI in the cold and warm months of western Iran when compared to the MLR, GPR, XGB, and RF models. The major findings of our study were summarized as follows:
•Using multicollinearity analysis, wind speed, precipitation, palmer drought severity index, NDVI, NDSI, surface pressure, soil heat flux, and potential evapotranspiration were selected as the set of non-correlated predictors of CMDSI and WMDSI.
•he DNN models had the highest accuracy when compared to the other machine learners when predicting CMDSI and WMDSI. In comparison, MLR consistently had the lowest accuracy. Hence, we recommend its use for areas with similar environmental conditions. However, future studies should evaluate its effectiveness for areas with different environmental conditions to confirm the generalizability of DNN for other areas.
•Game theory was useful in identifying the most important environmental controls dust events during the cold and warm months in western Iran. Using this technique, wind speed and soil heat flux were identified as the main factors controlling dust events in the cold months while wind speed and precipitation were the main controls during the warm months of the study period.
•Examining the effectiveness of different machine-learning models for predicting dust storms and identifying the factors affecting these events can increase our understanding of the mechanism of dust events across arid regions of the world. The lake of long-term data for all synoptic stations located in the study area and the short duration of data from some stations are considered as limitations of the present study.