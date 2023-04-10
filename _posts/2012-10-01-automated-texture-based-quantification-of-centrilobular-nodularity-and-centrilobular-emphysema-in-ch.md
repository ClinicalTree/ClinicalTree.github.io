---
title: Automated Texture-based Quantification of Centrilobular Nodularity and Centrilobular Emphysema in Chest CT Images
author: [CL_AT_ShoshanaBGinsburgMS,CL_AT_DavidALynchMB,CL_AT_RussellPBowlerMDPhD,CL_AT_JoyceDSchroederMD]
date: 2012-10-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 10]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Characterization of smoking-related lung disease typically consists of visual assessment of chest computed tomographic (CT) images for the presence and extent of emphysema and centrilobular nodularity (CN). Quantitative analysis of emphysema and CN may improve the accuracy, reproducibility, and efficiency of chest CT scoring. The purpose of this study was to develop a fully automated texture-based system for the detection and quantification of centrilobular emphysema (CLE) and CN in chest CT images.

## Materials and Methods

A novel approach was used to prepare regions of interest (ROIs) within the lung parenchyma for representation by texture features associated with the gray-level run-length and gray-level gap-length methods. These texture features were used to train a multiple logistic regression classifier to discriminate between normal lung tissue, CN or “smoker's lung,” and CLE. This classifier was trained and evaluated on 24 and 71 chest CT scans, respectively.

## Results

During training, the classifier correctly classified 89% of ROIs depicting normal lung tissue, 74% of ROIs depicting CN, and 95% of ROIs manifesting CLE. When the performance of the classifier in quantifying extent of CN and CLE was evaluated on 71 chest CT scans, 65% of ROIs in smokers without CLE were classified as CN, compared to 31% in nonsmokers ( _P_ < .001) and 28% in smokers with CLE ( _P_ < .001).

## Conclusions

The texture-based framework described herein facilitates successful discrimination among normal lung tissue, CN, and CLE and can be used for the automated quantification of smoking-related lung disease.

Chronic obstructive pulmonary disease (COPD), the third leading cause of death in the United States , is a chronic lung disease strongly associated with smoking. COPD comprises both large-airway and small-airway disease and emphysema, which is characterized by the progressive destruction of alveolar walls in lung tissue. Emphysema is visible on computed tomographic (CT) images as areas with low attenuation values similar to the density of air. Centrilobular nodularity (CN) or respiratory bronchiolitis (“smoker's lung”), which is thought to be the earliest manifestation of smoking-related lung injury, manifests as multiple centrilobular nodules <3 mm in size centered in the pulmonary lobule . The presence and extent of emphysema and CN are typically assessed by radiologists for the characterization of smoking-related lung disease.

Currently, the reference standard for the evaluation of disease extent on CT imaging is visual examination. However, visual assessment of CT images for quantifying and staging COPD is limited by high interobserver variability . For instance, at the Genetic Epidemiology of COPD (COPDGene) Study CT Imaging Workshop that took place in February 2010, 51 pulmonologists and radiologists reviewed 395 CT scans, each of which was evaluated by nine to 11 reviewers. Average κ values for the detection of CN and the quantification of centrilobular emphysema (CLE) by readers were 0.12 and 0.33, respectively . These poor κ values suggest that the visual detection and quantification of CN and CLE are limited by readers' subjectivity. A second limitation of visual assessment is the time and expense involved. Especially in large-scale projects such as the COPDGene Study (10,500 subjects from 21 different academic centers), visual evaluation of thousands of scans can be prohibitively time consuming and costly.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Data Description

## Study population

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Description of Subjects From the COPDGene Study Cohort Used in This Study


Variable Nonsmokers, No Emphysema Smokers, No Emphysema Smokers, Centrilobular Emphysema Training (n = 12) Evaluation (n = 25) Training (n = 12) Evaluation (n = 24) Training (n = 12) Evaluation (n = 22) Subject data Men/women 3/9 7/18 6/6 15/9 7/5 9/13 Age at enrollment (y) 61.2 ± 7.2 61.5 ± 8.0 60.2 ± 11.2 59.6 ± 7.8 64.2 ± 10.0 67.5 ± 7.6 BMI (kg/m  2  ) 25.5 ± 3.1 28.6 ± 5.8 30.0 ± 5.3 32.9 ± 5.9 29.7 ± 7.4 26.0 ± 5.2 Smoking history Start age (y) NA NA 16.0 ± 2.0 17.0 ± 14.7 17.6 ± 7.5 17.7 ± 3.8 Current smokers (yes/no) NA NA 5/7 6/18 6/6 4/18 Stop age (y) NA NA 42.0 49.0 55.3 58.9 Cigarettes/day NA NA 21.1 ± 11.9 27.7 ± 14.7 30.3 ± 15.1 26.1 ± 10.7 ATS pack-years NA NA 31.7 ± 15.6 46.2 ± 29.8 58.3 ± 26.4 54.1 ± 25.1 CT scanner Siemens/GE 11 (2)/1 21 (4)/4 9 (2)/3 (2) 18 (3)/6 (2) 9 (2)/3 (2) 19 (3)/3 (2) Number of study centers 5 6 5 9 6 7 VIDA image processing Total lung capacity (mL) 5445 ± 852 5125 ± 1046 6103 ± 1371 5600 ± 1217 6453 ± 1738 5866 ± 1148 % LAA  ∗  1.1 ± 1.1 1.3 ± 0.9 4.4 ± 3.2 3.5 ± 4.0 10.1 ± 5.1 17.6 ± 8.4 % air trapping  †  4.6 ± 3.1 10.0 ± 6.3 16.4 ± 13.6 11.5 ± 7.1 26.1 ± 11.4 41.4 ± 16.8

ATS, American Thoracic Society; BMI, body mass index; COPDGene, Genetic Epidemiology of COPD; CT, computed tomographic; LAA, low-attenuation area; NA, not applicable.


Data are expressed as mean ± standard deviation or as numbers.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image processing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Radiologist assessment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Overview of Methodology

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Summary of proposed method for quantification of centrilobular emphysema and centrilobular nodularity. ROI, region of interest.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedTexturebasedQuantificationofCentrilobularNodularityandCentrilobularEmphysemainChestCTImages/0_1s20S1076633212003121.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ROI Preprocessing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Bij=Ih−8IlIh−Il+7Ih−IlAij
B

i

j

=

I

h

−

8

I

l

I

h

−

I

l

+

7

I

h

−

I

l

A

i

j


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Representative regions of interest from (a) a scan of a normal subject with no emphysema, (f) a scan of a smoker with no emphysema, and (k) a scan of a subject with centrilobular emphysema binned between −1024 and −950 Hounsfield units (HU) (column 2), between −1024 and −856 HU (column 3), between −950 and −856 HU (column 4), and between the minimum and maximum gray levels in the parenchyma (column 5).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedTexturebasedQuantificationofCentrilobularNodularityandCentrilobularEmphysemainChestCTImages/1_1s20S1076633212003121.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Texture Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## GLRL method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Gray-level Run-length and Gap-length Features Used for Texture Analysis


Run-length Features Formula Gap-length Features Formula Average run length∑Nli=1∑Nrj=1jRij∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

l

∑

j

=

1

N

r

j

R

i

j

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Average gap length∑Nli=1∑Ngj=1jGij∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

l

∑

j

=

1

N

g

j

G

i

j

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Average gray level∑Nli=1∑Nrj=1iRij∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

l

∑

j

=

1

N

r

i

R

i

j

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Average gray level∑Nli=1∑Ngj=1iGij∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

l

∑

j

=

1

N

g

i

G

i

j

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Short run emphasis∑Nli=1∑Nrj=1Rij/j2∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j

/

j

2

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Short gap emphasis∑Nli=1∑Ngj=1Gij/j2∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j

/

j

2

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Long run emphasis∑Nli=1∑Nrj=1j2Rij∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

l

∑

j

=

1

N

r

j

2

R

i

j

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Long gap emphasis∑Nli=1∑Ngj=1j2Gij∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

l

∑

j

=

1

N

g

j

2

G

i

j

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Bright color emphasis∑Nli=1∑Nrj=1i2Rij∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

l

∑

j

=

1

N

r

i

2

R

i

j

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Bright color emphasis∑Nli=1∑Ngj=1i2Gij∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

l

∑

j

=

1

N

g

i

2

G

i

j

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Dark color emphasis∑Nli=1∑Nrj=1Rij/i2∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j

/

i

2

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Dark color emphasis∑Nli=1∑Ngj=1Gij/i2∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j

/

i

2

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Gray-level nonuniformity∑Nli=1(∑Nrj=1Rij)2(∑Nli=1∑Nrj=1Rij)2
∑

i

=

1

N

l

(

∑

j

=

1

N

r

R

i

j

)

2

(

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j

)

2
Gray level nonuniformity∑Nli=1(∑Ngj=1Gij)2(∑Nli=1∑Ngj=1Gij)2
∑

i

=

1

N

l

(

∑

j

=

1

N

g

G

i

j

)

2

(

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j

)

2
Run-length nonuniformity∑Nri=1(∑Nlj=1Rij)2(∑Nli=1∑Nrj=1Rij)2
∑

i

=

1

N

r

(

∑

j

=

1

N

l

R

i

j

)

2

(

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j

)

2
Gap-length nonuniformity∑Ngi=1(∑Nlj=1Gij)2(∑Nli=1∑Ngj=1Gij)2
∑

i

=

1

N

g

(

∑

j

=

1

N

l

G

i

j

)

2

(

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j

)

2
Gray-level distribution∑Nli=1(∑Nrj=1Rij)2∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

l

(

∑

j

=

1

N

r

R

i

j

)

2

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Gray-level distribution∑Nli=1(∑Ngj=1Gij)2∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

l

(

∑

j

=

1

N

g

G

i

j

)

2

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Run-length distribution∑Nri=1(∑Nlj=1Rij)2∑Nli=1∑Nrj=1Rij
∑

i

=

1

N

r

(

∑

j

=

1

N

l

R

i

j

)

2

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Gap-length distribution∑Ngi=1(∑Nlj=1Gij)2∑Nli=1∑Ngj=1Gij
∑

i

=

1

N

g

(

∑

j

=

1

N

l

G

i

j

)

2

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j
Run percentage1n∑Nli=1∑Nrj=1Rij
1

n

∑

i

=

1

N

l

∑

j

=

1

N

r

R

i

j
Gap percentage1n∑Nli=1∑Ngj=1Gij
1

n

∑

i

=

1

N

l

∑

j

=

1

N

g

G

i

j


_R_ and _G_ are the run-length and gap-length matrices, respectively; _N_ r  and _N_ g  represent the numbers of run and gap lengths considered, respectively; _N_ l  is the number of gray levels in the binned image; and _n_ is the number of pixels in the image or region of interest.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## GLGL method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Experiments

## Phase 1: Training

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Phase 2: Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Phase 1: Training

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Average Confusion Matrices Associated with Each of the Four Windowing Strategies Evaluated during the Training Phase


Range Classified as NNE SNE CLE −1024 to −950 HU True class NNE 86.2% 13.3% 0.5% SNE 30.0% 65.0% 5.0% CLE 2.8% 4.6% 92.7% −1024 to −856 HU True class NNE 85.7% 13.8% 4.6% SNE 27.1% 67.9% 5.0% CLE 1.8% 9.2% 89.0% −950 to −856 HU True class NNE 89.4% 10.6% 0.0% SNE 22.9% 74.3% 2.9% CLE 0.0% 5.5% 94.5% Minimum to maximum True class NNE 84.3% 14.3% 1.4% SNE 34.3% 57.1% 8.6% CLE 3.7% 11.0% 85.3%

CLE, centrilobular emphysema; HU, Hounsfield units; NNE, normal subjects with no emphysema; SNE, smokers with no emphysema.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Phase 2: Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Results of classification are shown in three dimensions for (a) a scan of a normal subject with no emphysema, (b) a scan of a smoker with no emphysema, and (c) a scan of a subject with centrilobular emphysema (CLE). Regions of interest (ROIs) colored blue were classified as normal lung, green ROIs were found to contain centrilobular nodularity, and red ROIs were found to manifest CLE.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedTexturebasedQuantificationofCentrilobularNodularityandCentrilobularEmphysemainChestCTImages/2_1s20S1076633212003121.jpg)

![Figure 4, Percentage of regions of interest classified as normal lung (blue) , centrilobular nodularity or “smoker's lung” (green) , and centrilobular emphysema (CLE) (red) for (a) 25 normal subjects with no emphysema, (b) 24 smokers with no emphysema, and (c) 22 subjects with CLE. Gold, Global Initiative for Chronic Obstructive Lung Disease.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedTexturebasedQuantificationofCentrilobularNodularityandCentrilobularEmphysemainChestCTImages/3_1s20S1076633212003121.jpg)

Table 4


Average Number and Percentage of Lung Regions of Interest Classified as Normal Lung Tissue, Manifesting CN, and Manifesting CLE for Computed Tomographic Scans in the Evaluation Data Set Belonging to NNE, SNE, and CLE Classes


Class Normal CN CLE_n_ %_n_ %_n_ % NNE 9407 ± 5693 65.8 ± 32.8 3098 ± 2749 30.9 ± 32.9 459 ± 470 3.3 ± 3.0 SNE 3624 ± 3280 30.2 ± 27.5 7208 ± 3612 64.6 ± 28.0 762 ± 1097 5.2 ± 5.8 CLE 3209 ± 3389 20.0 ± 16.4 3958 ± 2179 27.5 ± 14.9 7358 ± 3802 51.9 ± 28.9_P_ <.001 <.001 <.001

CLE, centrilobular emphysema; CN, centrilobular nodularity; NNE, normal subjects with no emphysema; SNE, smokers with no emphysema.


Data are expressed as mean ± standard deviations.


The probabilities of the null hypotheses that NNE, SNE, and CLE scans contain the same percentages of normal lung, CN, and CLE are listed in the bottom row.


![Figure 5, Percentage emphysema obtained using the texture-based method is correlated with (a) percentage low-attenuation area (LAA) computed by the density mask technique and (b) chronic obstructive pulmonary disease (COPD) Global Initiative for Chronic Obstructive Lung Disease (GOLD) stage. Black data points represent scans of normal subjects with no emphysema (NNE); cyan represents scans of smokers with no emphysema (SNE); and blue , green , and red represent GOLD stages 1, 2, and 3, respectively. The differences in percentage emphysema computed using the texture-based method were statistically significant ( P < .001) by analysis of variance. SNE scans were not statistically significantly different from NNE scans, but GOLD stages 1, 2, and 3 were statistically significantly different from both NNE and SNE classes ( P < .05).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedTexturebasedQuantificationofCentrilobularNodularityandCentrilobularEmphysemainChestCTImages/4_1s20S1076633212003121.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Kochanek K.D., Xu J., Murphy S.L., et. al.: Deaths: preliminary data for 2009. Natl Vit Stat Rep 2001; 59: pp. 1-51.


- 2\. Hansell D.M., Bankier A.A., MacMahon H., et. al.: Fleischner society: glossary of terms for thoracic imaging. Radiology 2008; 246: pp. 697-722.


- 3\. Remy-Jardin M., Edme J.L., Boulenguez C., et. al.: Longitudinal follow-up study of smoker's lung with thin-section CT in correlation with pulmonary function tests. Radiology 2002; 222: pp. 261-270.


- 4\. Heyneman L.E., Ward S., Lynch D.A., et. al.: Respiratory bronchiolitis, respiratory bronchiolitis–associated interstitial lung disease, and desquamative interstitial pneumonia: different entities or part of the spectrum of the same disease process. AJR Am J Roentgenol 1999; 173: pp. 1617-1622.


- 5\. Hersh C.P., Washko G.R., Jacobson F.L., et. al.: Interobserver variability in the determination of upper lobe-predominant emphysema. Chest 2007; 131: pp. 424-431.


- 6\. Lynch D.A., Murphy J.R., Crapo J.D., et. al.: A combined pulmonary-radiology workshop for visual evaluation of COPD: study design, chest CT findings and concordance with quantitative evaluation. J Chron Obstruct Pulmon Dis 2012; 9: pp. 151-159.


- 7\. Blechschmidt R.A., Werthschutzky R., Lorcher U.: Automated CT image evaluation of the lung: a morphology-based concept. IEEE Trans Med Imaging 2001; 20: pp. 434-442.


- 8\. Guo J., Reinhardt J.M., Kitaoka H., et. al.: Integrated system for CT-based assessment of parenchymal lung disease. Proc IEEE Int Sympos Biomed Imaging 2002; pp. 871-874.


- 9\. Keller B.M., Reeves A.P., Apanasovich T.V., et. al.: Quantitative assessment of emphysema from whole lung CT scans: comparison with visual grading. Proc SPIE 2009; pp. 7260. 726008


- 10\. Mishima M., Hirai T., Itoh H., et. al.: Complexity of terminal airspace geometry assessed by lung computed tomography in normal subjects and patients with chronic obstructive pulmonary disease. Proc Natl Acad Sci U S A 1999; 96: pp. 8829-8834.


- 11\. Nakano Y., Muro S., Sakai H., et. al.: Computed tomographic measurements of airway dimensions and emphysema in smokers. Am J Respirat Crit Care Med 2000; 162: pp. 1102-1108.


- 12\. Nakano Y., Sakai H., Muro S., et. al.: Comparison of low attenuation areas on computed tomographic scans between inner and outer segments of the lung in patients with chronic obstructive pulmonary disease: incidence and contribution to lung function. Thorax 1999; 54: pp. 384-389.


- 13\. Stavngaard T., Shaker S.B., Bach K.S., et. al.: Quantitative assessment of regional emphysema distribution in patients with chronic obstructive pulmonary disease (COPD). Acta Radiol 2006; 9: pp. 914-921.


- 14\. Boedeker K.L., McNitt-Gray M.F., Rogers S.R., et. al.: Emphysema: effect of reconstruction algorithm on CT imaging measures. Radiology 2004; 232: pp. 295-301.


- 15\. Kemerink G.J., Kruize H.H., Lamers R.J.S., et. al.: CT lung densitometry: dependence of CT number histograms on sample volume and consequences for scan protocol comparability. J Comput Assist Tomogr 1997; 21: pp. 948-954.


- 16\. Kemerink G.J., Lamers R.J.S., Pellis B.J., et. al.: On segmentation of lung parenchyma in quantitative computed tomography of the lung. Med Phys 1997; 25: pp. 2432-2439.


- 17\. Sluimer I., Prokop M., Hartmann I., et. al.: Automated classification of hyperlucency, fibrosis, ground glass, solid, and focal lesions in high-resolution CT of the lung. Med Phys 2006; 33: pp. 2610-2620.


- 18\. Gietema H.A., Muller N.L., Fauerbach P.V.N., et. al.: Quantifying the extent of emphysema: factors associated with radiologists' estimations and quantitative indices of emphysema severity using the ECLIPSE cohort. Acad Radiol 2011; 18: pp. 661-671.


- 19\. Sluimer I., van Waes P.F., Viergever M.A., et. al.: Computer-aided diagnosis in high resolution CT of the lungs. Med Phys 2003; 30: pp. 3081-3090.


- 20\. Uppaluri R., Hoffman E.A., Sonka M., et. al.: Computer recognition of regional lung disease patterns. Am J Respirat Crit Care Med 1999; 160: pp. 648-654.


- 21\. Zavaletta V.A., Bartholmai B.J., Robb R.A.: High resolution multidetector CT-aided tissue analysis and quantification of lung fibrosis. Acad Radiol 2007; 14: pp. 772-787.


- 22\. Chabat F., Yang G., Hansell D.M.: Obstructive lung diseases: texture classification for differentiation at CT. Radiology 2003; 228: pp. 871-877.


- 23\. Kim N., Seo J.B., Lee Y., et. al.: Development of an automatic classification system for differentiation of obstructive lung disease using HRCT. J Digit Imaging 2009; 22: pp. 136-148.


- 24\. Uppaluri R., McLennan G., Sonka M., et. al.: Interstitial lung disease: a quantitative study using the adaptive multiple feature method. Am J Respirat Crit Care Med 1999; 159: pp. 519-525.


- 25\. Xu Y., Sonka M., McLennan G., et. al.: MDCT-based 3-D texture classification of emphysema and early smoking related lung pathologies. IEEE Trans Med Imaging 2006; 25: pp. 464-475.


- 26\. Park Y.S., Seo J.B., Kim N., et. al.: Texture-based quantification of pulmonary emphysema on high-resolution computed tomography: comparison with density-based quantification and correlation with pulmonary function tests. Invest Radiol 2008; 43: pp. 395-402.


- 27\. Prasad M., Sowmya A., Wilson P.: Multi-level classification of emphysema in HRCT lung images. Pattern Anal Appl 2009; 12: pp. 9-20.


- 28\. Sorensen L., Shaker S.B., de Bruijne M.: Quantitative analysis of pulmonary emphysema using local binary patterns. IEEE Trans Med Imaging 2010; 29: pp. 559-569.


- 29\. Uppaluri R., Mitsa T., Sonka M., et. al.: Quantification of pulmonary emphysema from lung computed tomography images. Am J Respirat Crit Care Med 1997; 156: pp. 248-254.


- 30\. Regan E.A., Hokanson J.E., Murphy J.R., et. al.: Genetic epidemiology of COPD (COPDGene) study design. J Chron Obstruct Pulmon Dis 2010; 7: pp. 32-43.


- 31\. Han M.K., Kazerooni E.A., Lynch D.A., et. al.: Chronic obstructive pulmonary disease exacerbations in the COPDGene study: associated radiologic phenotypes. Radiology 2011; 261: pp. 274-282.


- 32\. Calverley P.M.A.: The GOLD classification has advanced understanding of COPD. Am J Respirat Crit Care Med 2004; 170: pp. 211-212.


- 33\. Genevois P.A., Vuyst P.D., de Maertelaer V., et. al.: Comparison of computed density and microscopic morphometry in pulmonary emphysema. Am J Respirat Crit Care Med 1996; 154: pp. 187-192.


- 34\. Coxson H.O., Rogers R.M., Whittall K.P., et. al.: A quantification of the lung surface area in emphysema using computed tomography. Am J Respirat Crit Care Med 1999; 159: pp. 851-856.


- 35\. Loh H., Leu J., Luo R.C.: The analysis of natural textures using run length features. IEEE Trans Indust Electron 1988; 35: pp. 323-328.


- 36\. Xinli W., Albregtsen F., Foyn B.: Texture features from gray level gap length matrix. IAPR Workshop Mach Vision Appl 1994; pp. 375-378.


- 37\. Hastie T., Tibshirani R., Friedman J.: The elements of statistical learning: data mining, inference, and prediction.2001.SpringerNew York