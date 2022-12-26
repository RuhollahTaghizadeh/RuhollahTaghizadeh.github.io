---
title: Convolutional Neural Networks 
author: Ruhollah Taghizadeh
date: "2020-11-24T00:00:00Z"
slug: Multi Task CNNs for Soil Mapping
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
  url:  https://www.sciencedirect.com/science/article/abs/pii/S0016706119312777
subtitle: 'Multi-task convolutional neural networks outperformed random forest for mapping soil particle size fractions in central Iran'
summary: 'Although conventional machine learning algorithms, such as random forest, have been extensively used in digital soil mapping to predict the PSF, less research examined the potential of state-of-the-art deep learning approaches for such processing. Convolutional neural networks are able to incorporate contextual information about the landscape, which is of great use for digital soil mapping analysis.'
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
Accordingly, the main objectives of this study are to (i) propose a CNN architecture and modelling framework that allows predicting the spatial distribution of PSFs in soils of central Iran, three-dimensionally for various soil depths, (ii) compare the CNN with one of the current state-of-the-art RF algorithm, (iii) and to analyse the effect of CNN patch sizes on the prediction error. It should be noted the comparison between RF and CNN models in the previous studies has been done by using auxiliary data “as-is” for RF while letting CNN essentially search for the best feature space by looking in the respective neighborhoods. Therefore, it might not be totally true to state that CNN is better than RF when the RF models have not been given all the information that they can use. In the current study, we tried to effectively reproduce the auxiliary data (i.e. feature-engineered auxiliary data) using simple smoothing (mean) filters with different neighbourhood sizes (radii of 1, 3, 5, 7, 9, 15, 21, and 29 pixels). It enables a fairer comparison between RF and CNN models.

## Methods

we proposed a patch-based, multi-task CNN architecture, specifically designed for DSM analysis, to predict PSF at six standard depths. The capability of the proposed CNN method was evaluated by comparing it to a well-known, conventional ML algorithm (i.e. Random Forest).

![](fig1.png)

## Convolutional neural networks

CNNs consists of two parts: the first part consists of convolutional filtering for extracting features hierarchically and the second is a fully-connected layer to calculate the output value from multiple input values composed of fully-connected layers of neurons. Ordinary artificial neural networks (ANNs) only consist of the second part; therefore, the feature extraction step is the main distinction between CNNs and ordinary ANNs. Feature extraction by convolutional filtering attempts to extract characteristic information from auxiliary data in the spatial sense. In image analysis or pattern recognition, these can, for example, be for a face of a person or for a cat. In our case, it may be a particular shape of the terrain surface; for example, a peak or a steep slope that is relevant for describing the distribution of soil properties. Feature extraction by convolutional filtering consists of different steps that can be repeated several times and includes convolution and pooling. The aim is to extract the most relevant features and the multiple representations of the spatial scales from the entire auxiliary data set.

## Accuracy assessment

The results demonstrated that CNN was advantageous in characterizing a relationship between the target and auxiliary data in all depths for clay, sand, and silt content predictions even when the RF and RF* models were insufficient (i.e. for deeper soil layers). The higher accuracy of CNN models is potentially explained by the fact that CNNs incorporate contextual information into their prediction scheme, which is of great use for DSM analysis. Importantly, the results revealed that CNN is advantageous for DSM analysis in the subsoil where the conventional methods either fail or have the poor capability.

![](fig2.png)

## Spatial distribution of soil particle size fractions

The predicted soil texture maps indicated the soils in the central part of the region are light-textured from top to depth due to the lack of moisture to develop and wind-eroded light-textured deposits mostly cover the lowlands of that region. The eastern parts from North to South are mostly covered by gypsiferous soils in uplands and wind deposits in lowlands and, therefore, are sandy-textured in the top and relatively clay-textured in depth. The soils in the western and southern parts of the study area have been experiencing a relatively favorable climate condition, which contributed to developing soils with clay texture in plains and in sloping piedmonts compared to soils in the eastern or northern parts of the study area.

![](fig3.png)


## Conclusion

For all soil depths, the proposed CNN architecture consistently outperformed the RF model for predicting PSF. This highlighted the importance of including contextual information for soil studies and explained the better performance of CNN compared to RF. Even the use of feature-engineered auxiliary data could not enable the RF* models to reach the performance of CNN. This is because the latter approach relies on the exclusive use of local characteristics (e.g., spectral information and elevation) within its prediction scheme so that important complex characteristics on a catena or regional scale are not reflected in the subsequent data-mining algorithm.
