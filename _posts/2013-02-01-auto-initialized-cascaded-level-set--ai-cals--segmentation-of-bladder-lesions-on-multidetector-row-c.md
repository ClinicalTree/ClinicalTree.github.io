---
title: Auto-Initialized Cascaded Level Set (AI-CALS) Segmentation of Bladder Lesions on Multidetector Row CT Urography
author: [CL_AT_LubomirHadjiiskiPhD,CL_AT_HeangPingChanPhD,CL_AT_ElaineMCaoiliMD,CL_AT_RichardHCohanMD,CL_AT_JunWeiPhD,CL_AT_ChuanZhouPhD]
date: 2013-02-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 20, Issue 2]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

To develop a computerized system for segmentation of bladder lesions on computed tomography urography (CTU) scans for detection and characterization of bladder cancer.

## Materials and Methods

We have developed an auto-initialized cascaded level set method to perform bladder lesion segmentation. The segmentation performance was evaluated on a preliminary dataset including 28 CTU scans from 28 patients collected retrospectively with institutional review board approval. The bladders were partially filled with intravenous contrast material. The lesions were located fully or partially within the contrast-enhanced area or in the non–contrast-enhanced area of the bladder. An experienced abdominal radiologist marked 28 lesions (14 malignant and 14 benign) with bounding boxes that served as input to the automated segmentation system and assigned a difficulty rating on a scale of 1 to 5 (5 = most subtle) to each lesion. The contours from automated segmentation were compared to three-dimensional contours manually drawn by the radiologist. Three performance metric measures were used for comparison. In addition, the automated segmentation quality was assessed by an expert panel of two experienced radiologists, who provided quality ratings of the contours on a scale from 1 to 10 (10 = excellent).

## Results

The average volume intersection ratio, the average absolute volume error, and the average distance measure were 67.2 ± 16.9%, 27.3 ± 26.9%, and 2.89 ± 1.69 mm, respectively. Of the 28 segmentations, 18 were given quality ratings of 8 or above. The average rating was 7.9 ± 1.5. The average quality ratings for lesions with difficulty ratings of 1, 2, 3, and 4 were 8.8 ± 0.9, 7.9 ± 1.8, 7.4 ± 0.9, and 6.6 ± 1.5, respectively.

## Conclusion

Our preliminary study demonstrates the feasibility of using the three-dimensional level set method for segmenting bladder lesions in CTU scans.

## Introduction

Bladder cancer is a common type of cancer that can cause substantial morbidity and mortality among both men and women. Bladder cancer causes 14,880 deaths per year in the United States . Early detection of bladder cancers is very important. The survival rate for patients whose cancers were detected and treated early is high . Early diagnosis and treatment of these lesions can improve the morbidity, mortality, and their attendant costs compared to diagnosis at a later stage when muscularis mucosa invasion and/or regional or distant metastases have developed. However, at the present time, only 75% of cancers are detected in the early localized stage.

Multidetector row computed tomography (MDCT) urography is a very promising new imaging modality for evaluation of patients with known or suspected urothelial neoplasms . It offers the distinct advantage of providing essentially complete imaging of the urinary tract and of the remainder of the abdomen and pelvis in a single study. With MDCT urography, it is expected that the need for other imaging studies (such as intravenous urography, ultrasonography, or magnetic resonance imaging) will be substantially reduced. Computed tomography urography (CTU), therefore, may spare the patient the considerable effort of undergoing a potentially large number of alternative imaging studies and also reduce health care costs.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Computed tomography urography slice showing bladder with a bladder lesion ( white arrow ). This lesion contains a thin rim of peripheral calcification.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/0_1s20S1076633212004680.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Level Set Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Block diagram of the autoinitialized cascaded level set (AI-CALS) method. 3D, three dimensional.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/1_1s20S1076633212004680.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

x∈C˜:{\|I(x)−μ\|≤3.0σ,I(x)>−400HU},
x

∈

C

˜

:

{

\|

I

(

x

)

−

μ

\|

≤

3.0

σ

,

I

(

x

)

>

−

400

H

U

}

,


where _I_ ( _x_ ) is the voxel value. A morphological dilation filter, 3D flood fill algorithm, and morphological erosion filter are applied to C˜
C

˜
to connect neighboring components and extract an initial segmentation surface _C_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Dataset

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Distribution of the difficulty ratings for the conspicuity of the lesions in the dataset (1 = most obvious, 5 = most subtle). No case was rated as 5 in this pilot dataset.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/2_1s20S1076633212004680.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

AVDIST(G,U)=12(∑x∈Gmin{d(x,y):y∈U}NG+∑y∈Umin{d(x,y):x∈G}NU),
A

V

D

I

S

T

(

G

,

U

)

=

1

2

(

∑

x

∈

G

min

{

d

(

x

,

y

)

:

y

∈

U

}

N

G

+

∑

y

∈

U

min

{

d

(

x

,

y

)

:

x

∈

G

}

N

U

)

,


where _G_ is the gold standard 3D surface contour marked by the radiologist and _U_ is the 3D contour being evaluated. _N  G_ and _N  U_ denote the number of points (voxels) on _G_ and _U_ , respectively. The function _d_ is the Euclidean distance. For a given voxel along the contour _G_ , the distance to the closest point along the contour _U_ is determined. The minimum distances for all points in _G_ are averaged. This process is repeated by switching the roles of _G_ and _U_ . The two average minimum distances are then averaged.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

R3D=VG∩VUVG,
R

3

D

=

V

G

∩

V

U

V

G

,


where _V__G_ is the volume enclosed by the gold standard contour _G_ and _V__U_ is the volume enclosed by the contour _U_ . A value of 1 indicates that _V__U_ completely overlap with _V__G_ , whereas a value of 0 implies _V__U_ and _V__G_ are disjoint.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

E3D=VG−VUVG,
E

3

D

=

V

G

−

V

U

V

G

,


where negative error indicates oversegmentation and vice versa. Because the over- and undersegmentation tend to mask the actual deviations from the gold standard when the average is taken, the absolute (unsigned) errors \| _E__3D_ \| is also calculated.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Histogram of the volume intersection ratio measure. The average was 67.2%.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/3_1s20S1076633212004680.jpg)

![Figure 5, Histogram of the average distance measure. The average was 2.89 mm.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/4_1s20S1076633212004680.jpg)

![Figure 6, Histogram of the volume error. The average was 4.9%.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/5_1s20S1076633212004680.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Histogram for the radiologists' quality ratings of the AI-CALS segmented contours.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/6_1s20S1076633212004680.jpg)

![Figure 8, Radiologists' quality ratings for the AI-CALS segmented lesions grouped by radiologists' lesion difficulty ratings.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/7_1s20S1076633212004680.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Segmentation of bladder lesions with difficulty rating of 1: (a,c,e) the original images; (b,d,f) the corresponding AI-CALS segmentations ( black contours ) and radiologist hand outlines ( white contours ). The segmentation quality for (b,d,f) was 10, 8, and 7, respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/8_1s20S1076633212004680.jpg)

![Figure 10, Segmentation of bladder lesions with difficulty rating of 2: (a,c,e) the original images; (b,d,f) the corresponding AI-CALS segmentations ( black contours ) and radiologist hand outlines ( white contours ). The segmentation quality for (b,d,f) was 10, 8, and 5, respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/9_1s20S1076633212004680.jpg)

![Figure 11, Segmentation of bladder lesions with difficulty rating of 3: (a,c,e) the original images; (b,d,f) the corresponding AI-CALS segmentations ( black contours ) and radiologist hand outlines ( white contours ). The segmentation quality for (b,d,f) was 8, 8, and 6 respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/10_1s20S1076633212004680.jpg)

![Figure 12, Segmentation of bladder lesions with difficulty rating of 4: (a,c,e) the original images; (b,d,f) the corresponding AI-CALS segmentations ( black contours ) and radiologist hand outlines ( white contours ). The segmentation quality for (b,d,f) was 9, 6, and 5, respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutoInitializedCascadedLevelSetAICALSSegmentationofBladderLesionsonMultidetectorRowCTUrography/11_1s20S1076633212004680.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\.  American Cancer Society.  www.cancer.org  2012\. Cancer Facts & Figures 2012.


- 2\. McCarthy C.L., Cowan N.C.: Multidetector CT urography (MD-CTU) for urothelial imaging. Radiology 2002; 225: pp. 237.


- 3\. Noroozian M., Cohan R.H., Caoili E.M., et. al.: Multislice CT urography: state of the art. Br J Radiol 2004; 77: pp. S74-S86.


- 4\. Akbar S.A., Mortele K.J., Baeyens K., et. al.: Multidetector CT urography: Techniques, clinical applications, and pitfalls. Semin Ultrasound CT MRI 2004; 25: pp. 41-54.


- 5\. Liu W.C., Mortele K.J., Silverman S.G.: Incidental extraurinary findings at MDCT urography in patients with hematuria: prevalence and impact on imaging costs. AJR Am J Roentgenol 2005; 185: pp. 1051-1056.


- 6\. Caoili E.M., Cohan R.H., Korobkin M., et. al.: Urinary tract abnormalities: initial experience with multi-detector row CT urography. Radiology 2002; 222: pp. 353-360.


- 7\. Sudakoff G.S., Dunn D.P., Guralnick M.L., et. al.: Multidetector computerized tomography urography as the primary imaging modality for detecting urinary tract neoplasms in patients with asymptomatic hematuria. J Urol 2008; 179: pp. 862-867.


- 8\. Park S.B., Kim J.K., Lee H.J., et. al.: Hematuria: portal venous phase multi detector row CT of the bladder—a prospective study. Radiology 2007; 245: pp. 798-805.


- 9\. Li L., Wang Z., Li X., et. al.: A new partial volume segmentation approach to extract bladder wall for computer aided detection in virtual cystoscopy. Proc SPIE 2004; 5369: pp. 199-206.


- 10\. Duan C., Liang Z., Bao S., et. al.: A coupled level set framework for bladder wall segmentation with application to MR cystography. IEEE Trans Med Imaging 2010; 29: pp. 903-915.


- 11\. Duan C.J., Yuan K.H., Liu F.H., et. al.: Volume-based features for detection of bladder wall abnormal regions via MR cystography. IEEE Trans Biomed Engin 2011; 58: pp. 2506-2512.


- 12\. Duan C.J., Yuan K.H., Liu F.H., et. al.: An adaptive window-setting scheme for segmentation of bladder tumor surface via MR cystography. IEEE Trans Inform Technol Biomed 2012; 16: pp. 720-729.


- 13\.  Hadjiiski L, Chan H-P, Caoili E, et al. Segmentation of malignant and benign bladder lesions on multidetector row CT urography using 3D level set. Presented at: Radiological Society of North America 2010 Scientific Assembly and Annual Meeting. Chicago, IL, November 28–December 3, 2010.


- 14\. Street E., Hadjiiski L., Sahiner B., et. al.: Automated volume analysis of head and neck lesions on CT scans using 3D level set segmentation. Med Phys 2007; 34: pp. 4399-4408.


- 15\. Sahiner B., Petrick N., Chan H.P., et. al.: Computer-aided characterization of mammographic masses: accuracy of mass segmentation and its effects on characterization. IEEE Trans Med Imaging 2001; 20: pp. 1275-1284.


- 16\. Way T.W., Hadjiiski L.M., Sahiner B., et. al.: Computer-aided diagnosis of pulmonary nodules on CT scans: segmentation and classification using 3D active contours. Med Phys 2006; 33: pp. 2323-2337.