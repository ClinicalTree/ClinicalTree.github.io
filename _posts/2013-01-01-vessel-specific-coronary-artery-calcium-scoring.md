---
title: Vessel Specific Coronary Artery Calcium Scoring
author: [CL_AT_RahilShahzadMSc,CL_AT_TheovanWalsumPhD,CL_AT_MichielSchaapPhD,CL_AT_AlexiaRossiMD,CL_AT_StefanKleinPhD,CL_AT_AnnickCWeustinkMDPhD,CL_AT_PimJdeFeyterMDPhD,CL_AT_LucasJvanVlietPhD,CL_AT_WiroJNiessenPhD]
date: 2013-01-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 20, Issue 1]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to automatically detect and quantify calcium lesions for the whole heart as well as per coronary artery on non-contrast-enhanced cardiac computed tomographic images.

## Materials and Methods

Imaging data from 366 patients were randomly selected from patients who underwent computed tomographic calcium scoring assessments between July 2004 and May 2009 at Erasmum MC, Rotterdam. These data included data sets with 1.5-mm and 3.0-mm slice spacing reconstructions and were acquired using four different scanners. The scores of manual observers, who annotated the data using commercially available software, served as ground truth. An automatic method for detecting and quantifying calcifications for each of the four main coronary arteries and the whole heart was trained on 209 data sets and tested on 157 data sets. Statistical testing included determining Pearson's correlation coefficients and Bland-Altman analysis to compare performance between the system and ground truth. Wilcoxon's signed-rank test was used to compare the interobserver variability to the system's performance.

## Results

Automatic detection of calcified objects was achieved with sensitivity of 81.2% per calcified object in the 1.5-mm data set and sensitivity of 86.6% per calcified object in the 3.0-mm data set. The system made an average of 2.5 errors per patient in the 1.5-mm data set and 2.2 errors in the 3.0-mm data set. Pearson's correlation coefficients of 0.97 ( _P_ < .001) for both 1.5-mm and 3.0-mm scans with respect to the calcium volume score of the whole heart were found. The average _R_ values over Agatston, mass, and volume scores for each of the arteries (left circumflex coronary artery, right coronary artery, and left main and left anterior descending coronary arteries) were 0.93, 0.96, and 0.99, respectively, for the 1.5-mm scans. Similarly, for 3.0-mm scans, _R_ values were 0.94, 0.94, and 0.99, respectively. Risk category assignment was correct in 95% and 89% of the data sets in the 1.5-mm and 3-mm scans.

## Conclusions

An automatic vessel-specific coronary artery calcium scoring system was developed, and its feasibility for calcium scoring in individual vessels and risk category classification has been demonstrated.

Coronary artery disease is one of the leading causes of mortality worldwide . Many clinical studies have shown that the amount of calcium in coronary artery plaques correlates with the risk for future cardiovascular events .

Calcium scoring is routinely performed on low-dose, non-contrast-enhanced computed tomographic (CT) scans by manually annotating all calcium objects present in the main vessels of the coronary artery tree: the left main (LM), left circumflex, left anterior descending (LAD), and right coronary arteries. Subsequently, on the basis of all selected objects per patient, the Agatston , mass , or volume score is determined. Recently, it has been suggested that vessel-specific calcium scoring or rather risk assessment on the basis of individual vessels is more informative compared to whole-heart calcium scoring . Similar findings have been reported in other large population studies. Williams et al observed that the mortality rate of the patients they followed increased proportionally with the rise in the number of calcified lesions, and they also observed that all patients who had Agatston scores ≥ 1000 in the LM died during follow-up. Mohlenkamp et al observed that LM disease was an independent predictor of hard events. Vessel-specific scores also facilitate in better understanding calcium progression in longitudinal studies. Budoff and Raggi found that calcium increases by approximately 20% to 30% each year. The Multi-Ethnic Study of Atherosclerosis investigated the relationship between calcium scores at baseline and stenosis in individual vessels. It reported a positive correlation between calcium scores and vessel-specific scores in the individual artery beds.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Data Description

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Details of the Data Sets


Variable Value Data sets Total 366 Women 86 (23.5%) Men 280 (76.5%) Age, women (y) 57 (28–83) Age, men (y) 57 (21–84) Scanner type  ∗  Definition (3.0-mm scans) 132 (36.1%) Sensation 64 205 (56%) Definition Flash 16 (4.4%) Definition AS+ 13 (3.5%)

Data are expressed as number (percentage) or as mean (range).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Schematic diagram showing the distribution of data sets used for designing, training, and testing of the calcium scoring system. CT, computed tomographic.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/VesselSpecificCoronaryArteryCalciumScoring/0_1s20S1076633212004266.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## System Overview

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, An illustration showing the work flow of the system. ( Top left ) Non-contrast-enhanced computed tomographic (CT) image of a patient that needs to be analyzed. ( Bottom left ) Ten contrast-enhanced CT angiographic images used as atlases to compute the coronary artery position estimate features. Using a registration step, the CT angiographic atlas features are mapped onto the CT image. The detected calcium objects are then labeled using the position estimates as shown by the image on the right ( red objects are assigned to the left anterior descending coronary artery and the yellow object to the left circumflex coronary artery).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/VesselSpecificCoronaryArteryCalciumScoring/1_1s20S1076633212004266.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Candidate Detection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classifier

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Features

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Feature Description


Feature Description Number of Features Volume of object (mm  3  ) 1 Intensity of object: maximum and average 2 Position: _x_ , _y_ , and _z_ coordinates in image space and mean space 6 Intensity of voxel at the maximum intensity point after Gaussian filtering at five different scales 5 Intensity of voxel at the maximum intensity point after first-order Gaussian derivatives in _x_ , _y_ , and _z_ directions at five different scales 15 Intensity of voxel at the maximum intensity point after second-order Gaussian derivatives were computed in _xx_ , _yy_ , _zz_ , _xy_ , _yz_ , and _zx_ direction at five different scales 30 Coronary artery position likelihood estimate 1 Shape 2

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Object-based features

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Multi-scale image derivatives

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Coronary artery location estimate

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Position-based features

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Feature Selection and Classifier Selection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Calcium Scores

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Risk Categorization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reference Standard

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Overall Performance of the System for Calcium Object Detection

## 1.5-mm scans

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 3.0-mm scans

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Performance of the System on the Patient Calcium Scores

## 1.5-mm scans

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Results of Bland-Altman Analysis of Agatston, Mass, and Volume scores for the Individual Arteries and Correlation between Automatic and Manual Scores for Each of the Arteries after Discarding the Outliers (as Depicted in  Figure 4  )


Calcium Quantification (Score) Bias 95% Limits of Agreement Correlation ( _R_ ) 3.0-mm scans LCX Agatston 14 −93 to 122 0.94 Mass (mg) 3 −18 to 24 0.94 Volume (mm  3  ) 10 −84 to 104 0.93 RCA Agatston −14 −211 to 184 0.93 Mass (mg) −3 −45 to 39 0.94 Volume (mm  3  ) −14 −272 to 143 0.93 LM + LAD Agatston 11 −56 to 78 0.99 Mass (mg) 3 −12 to 17 0.99 Volume (mm  3  ) 1 −41 to 39 0.99 1.5-mm scans LCX Agatston −8 −243 to 227 0.96 Mass (mg) −2 −60 to 56 0.93 Volume (mm  3  ) −6 −187 to 175 0.96 RCA Agatston −4 −175 to 167 0.98 Mass (mg) −1 −43 to 42 0.96 Volume (mm  3  ) −4 −137 to 128 0.98 LM + LAD Agatston −5 −113 to 103 0.99 Mass (mg) −1 −23 to 21 0.99 Volume (mm  3  ) −6 −89 to 77 0.99

LAD, left anterior descending coronary artery; LCX, left circumflex coronary artery; LM, left main coronary artery; RCA, right coronary artery.


Table 4


Confusion Matrix for Assigning a Risk Percentile by the Automatic and Manual Scores for 3.0-mm and 1.5-mm Scans


3.0-mm Slice Spacing Scans 1.5-mm Slice Spacing Scans Automatic/Manual 10% 25% 50% 75% 90% Automatic/Manual 10% 25% 50% 75% 90% 10% 17 0 0 0 0 10% 15 0 0 0 0 25% 1 5 0 0 0 25% 0 13 0 0 0 50% 1 0 9 1 0 50% 1 0 22 1 0 75% 0 0 1 8 1 75% 0 1 1 22 0 90% 0 0 0 1 11 90% 0 0 0 1 24

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 3.0-mm scans

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Scatterplot of calcium volume obtained with automatic and manual methods. The largest errors are labeled and described below. (a) For 1.5-mm scans, (1) and (3) denote calcified mitral valves that were mistaken for calcium in the left circumflex coronary artery (LCX), (2) denotes an aortic calcification at the ostium was mistaken for calcium in the right coronary artery (RCA), (4) denotes a calcium object at the distal part of the RCA that was missed, and (5) denotes an aortic calcification at the ostium that was mistaken for calcium in the left main coronary artery (LM). (b) For 3.0-mm scans, (1) a few calcium objects in the RCA were missed, (2) a calcified mitral valve was mistaken for calcium in the LCX, (3) a calcified object in the distal part of the RCA was missed, and (4) and (5) indicate a few objects that were missed in the LCX.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/VesselSpecificCoronaryArteryCalciumScoring/2_1s20S1076633212004266.jpg)

![Figure 4, Scatterplot of automatic and manual volume scores for each of the arteries on the 1.5-mm scans: (a) left circumflex coronary artery (LCX), (b) right coronary artery (RCA), and (c) left main coronary artery (LM) and left anterior descending coronary artery (LAD). We discarded five outliers ( red ) in computing the correlation for assessing the accuracy of the automatic vessel labeling.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/VesselSpecificCoronaryArteryCalciumScoring/3_1s20S1076633212004266.jpg)

![Figure 5, Axial slices showing cases in which the automatic method misclassified calcium objects: false-positives ( left ) and false-negatives ( right ). ( Top left ) A 1.5-mm scan from an 84-year-old man with an aortic calcification at the ostium. ( Bottom left ) A 1.5-mm scan from a 57-year-old man with a calcified valve. ( Top right ) A 3.0-mm scan from a 46-year-old woman with a lesion in the left circumflex coronary artery (LCX). ( Bottom right ) A 3.0-mm scan from a 50-year-old man with a lesion in the LCX very close to the mitral valve.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/VesselSpecificCoronaryArteryCalciumScoring/4_1s20S1076633212004266.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Method Performance in Left-dominant and Balanced Subjects

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Interobserver Variability

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Coronary Artery Calcium Scores of the Automated System (A) and Observers O1 and O2 (Median), Pearson's Correlation Coefficient ( _R_ ), _Z_ Statistics Using Wilcoxon's Signed-rank test, and Bland-Altman Limits of Agreement for Interobserver and the System with Respect to the Observers


Score Median (Range)_R_ ∗ _Z_ Statistic Bland-Altman A O1 O2 Interobserver A-O1 A-O2 Interobserver  ∗  A-O1 A-O2 Interobserver A-O1 A-O2 Volume 204 (0 to 1700) 214 (0 to 1769) 224 (0 to 1727) 0.98 0.97 0.95 −4.4 −1.7 −2.1 −157 to 145 −220 to 198 −247 to 217 Mass 38 (0 to 378) 39 (0 to 389) 41 (0 to 382) 0.98 0.96 0.94 −3.9 −1.0 −1.8 −36 to 37 −48 to 49 −56 to 58 Agatston 216 (0 to 2117) 215 (0 to 2177) 217 (0 to 2136) 0.98 0.97 0.96 −3.5 −1.2 −1.7 −194 to 202 −243 to 237 −274 to 277

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

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

- 1\. World Health Organization : Cardiovascular diseases. Fact Sheet 317.2011.World Health OrganizationGeneva, Switzerland


- 2\. Budoff M.J., Gul K.M.: Expert review on coronary calcium. Vasc Health Risk Manage 2008; 4: pp. 315-324.


- 3\. Kondos G.T., Hoff J.A., Sevrukov A., et. al.: Coronary artery calcium and cardiac events electron-beam tomography coronary artery calcium and cardiac events: a 37-month follow-up of 5,635 initially asymptomatic low to intermediate risk adults. Circulation 2003; 107: pp. 2571-2576.


- 4\. Raggi P.: Coronary-calcium screening to improve risk stratification in primary prevention. J Louis State Medl Soc 2002; 154: pp. 314-318.


- 5\. Vliegenthart R., Oudkerk M., Hofman A., et. al.: Coronary calcification improves cardiovascular risk prediction in the elderly. Circulation 2005; 112: pp. 572-577.


- 6\. Elias-Smale S.E., Proenca R.V., Koller M.T., et. al.: Coronary calcium score improves classification of coronary heart disease risk in the elderly: the Rotterdam study. J Am Coll Cardiol 2010; 56: pp. 1407-1414.


- 7\. Detrano R., Guerci A.D., Carr J.J., et. al.: Coronary calcium as a predictor of coronary events in four racial or ethnic groups. N Engl J Med 2008; 358: pp. 1336-1345.


- 8\. Agatston A., Janowitz W., Hildner F., et. al.: Quantification of coronary artery calcium using ultrafast computed tomography. J Am Coll Cardiol 1990; 15: pp. 827-832.


- 9\. Callister T., Cooil B., Raya S., et. al.: Coronary artery disease: improved reproducibility of calcium scoring with an electronbeam CT volumetric method. Radiology 1998; 208: pp. 807-814.


- 10\. Hong C., Becker C.R., Schoepf U.J., et. al.: Coronary artery calcium: absolute quantification in nonenhanced and contrast-enhanced multi–detector row CT studies. Radiology 2002; 223: pp. 474-480.


- 11\. Qian Z., Anderson H., Marvasty I., et. al.: Lesion- and vessel-specific coronary artery calcium scores are superior to whole-heart Agatston and volume scores in the diagnosis of obstructive coronary artery disease. J Cardiovasc Comput Tomogr 2010; 4: pp. 391-399.


- 12\. Williams M., Shaw L.J., Raggi P., et. al.: Prognostic value of number and site of calcified coronary lesions compared with the total score. J Am Coll Cardiol Cardiovasc Imaging 2008; 1: pp. 61-69.


- 13\. Mohlenkamp S., Lehmann N., Schmermund A., et. al.: Prognostic value of extensive coronary calcium quantities in symptomatic males—a 5-year follow-up study. Eur Heart J 2003; 24: pp. 845-854.


- 14\. Budoff M.J., Raggi P.: Coronary artery disease progression assessed by electron-beam computed tomography. Am J Cardiol 2001; 88: pp. 46-50.


- 15\. Rosen B.D., Fernandes V., McClelland R.L., et. al.: Relationship between baseline coronary calcium score and demonstration of coronary artery stenoses during follow-up: MESA (Multi-Ethnic Study of Atherosclerosis). J Am Coll Cardiol Cardiovasc Imaging 2009; 2: pp. 1175-1183.


- 16\. Isgum I., Rutten A., Prokop M., et. al.: Detection of coronary calcifications from computed tomography scans for automated risk assessment of coronary artery disease. Med Phys 2007; 34: pp. 1450-1461.


- 17\. Shahzad R., Schaap M., van Walsum T., et. al.: A patient specific coronary artery density estimate. Proc IEEE Int Symp Biomed Imaging Nano Macro 2010; pp. 9-12.


- 18\. Theodoridis S., Koutroumbas K.: Pattern Recognition.2009.Academic PressSan Diego, CA


- 19\. Frangi A., Niessen W.J., Vincken K., et. al.: Multiscale vessel enhancement filtering. Med Image Comput Comput Assist Interv 1998; 1496: pp. 130-137.


- 20\. Pham D.L., Xu C., Prince J.L.: Current methods in medical image segmentation. Annu Rev Biomed Eng 2000; 2: pp. 315-337.


- 21\. Klein S., Staring M., Murphy K., et. al.: ElastiX: a toolbox for intensity-based medical image registration. IEEE Trans Med Imaging 2010; 29: pp. 196-205.


- 22\. Ohnesorge B., Flohr T., Fischbach R., et. al.: Reproducibility of coronary calcium quantification in repeat examinations with retrospectively ECG-gated multisection spiral CT. Eur Radiol 2002; 12: pp. 1532-1540.


- 23\. Oudkerk M., Stillman A.E., Halliburton S.S., et. al.: Coronary artery calcium screening: current status and recommendations from the European Society of Cardiac Radiology and North American Society for Cardiovascular Imaging. Int J Cardiovasc Imaging 2008; 24: pp. 645-671.


- 24\. Polonsky T.S., McClelland R.L., Jorgensen N.W., et. al.: Coronary artery calcium score and risk classification for coronary heart disease prediction. JAMA 2010; 303: pp. 1610-1616.


- 25\. Hoff J.A., Chomka E.V., Krainik A.J., et. al.: Age and gender distributions of coronary artery calcium detected by electron beam tomography in 35,246 adults. Am J Cardiol 2001; 87: pp. 1335-1339.


- 26\. Bland J.M., Altman D.G.: Statistical methods for assessing agreement between two methods of clinical measurement. Lancet 1986; 1: pp. 307-310.


- 27\. Cademartiri F., Grutta L.L., Malago R., et. al.: Prevalence of anatomical variants and coronary anomalies in 543 consecutive patients studied with 64-slice CT coronary angiography. Eur Radiol 2008; 18: pp. 781-791.


- 28\. Budoff M.J., Shaw L.J., Liu S.T., et. al.: Long-term prognosis associated with coronary calcification: observations from a registry of 25,253 patients. J Am Coll Cardiol 2007; 49: pp. 1860-1870.