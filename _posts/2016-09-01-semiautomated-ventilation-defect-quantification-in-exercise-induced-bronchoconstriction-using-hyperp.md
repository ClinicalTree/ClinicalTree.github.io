---
title: Semiautomated Ventilation Defect Quantification in Exercise-induced Bronchoconstriction Using Hyperpolarized Helium-3 Magnetic Resonance Imaging
author: [CL_AT_WeiZhaPhD,CL_AT_DavidJNilesPhD,CL_AT_StanleyJKrugerPhD,CL_AT_BernardJDardzinskiPhD,CL_AT_RobertVCadmanPhD,CL_AT_DavidGMummyMS,CL_AT_ScottKNagleMDPhD,CL_AT_SeanBFainPhD]
date: 2016-09-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 23, Issue 9]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

This study aimed to compare the performance of a semiautomated ventilation defect segmentation approach, adaptive _K_ -means, with manual segmentation of hyperpolarized helium-3 magnetic resonance imaging in subjects with exercise-induced bronchoconstriction (EIB).

## Materials and Methods

Six subjects with EIB underwent hyperpolarized helium-3 magnetic resonance imaging and spirometry tests at baseline, post exercise, and recovery over two separate visits. Ventilation defects were analyzed by two methods. First, two independent readers manually segmented ventilation defects. Second, defects were quantified by an adaptive _K_ -means method that corrected for coil sensitivity, applied a vesselness filter to estimate pulmonary vasculature, and segmented defects adaptively based on the overall low-intensity signals in the lungs. These two methods were then compared in four aspects: (1) ventilation defect percent (VDP) measurements, (2) correlation between spirometric measures and measured VDP, (3) regional VDP variations pre- and post exercise challenge, and (4) Dice coefficient for spatial agreement.

## Results

The adaptive _K_ -means method was ~5 times faster, and the measured VDP bias was under 2%. The correlation between predicted forced expiratory volume in 1 second over forced vital capacity and VDP measured by adaptive _K_ -means ( _ρ_ = −0.64, _P_ <  0.0001) and by the manual method ( _ρ_ = −0.63, _P_ <  0.0001) yielded almost identical 95% confidence intervals. Neither method of measuring VDP indicated apical/basal or anterior dependence in this small study cohort.

## Conclusions

Compared to the manual method, the adaptive _K_ -means method provided faster, reproducible, comparable measures of VDP in EIB and may be applied to a variety of lung diseases.

## Introduction

Over the past decade, hyperpolarized helium-3 magnetic resonance imaging (HP  3 He MRI) has been used extensively in research for evaluating ventilation and defect in asthma , cystic fibrosis (CF) , and chronic obstructive pulmonary disease (COPD) . Quantitative assessment of ventilation and its regional distribution is critical to the application and advance of HP gas MRI in clinical research. The ventilation defect quantification from HP gas MRI has been advanced from subjective defect scores to semiquantitative measures and quantitative defect volume measures . The commonly used quantitative metric is ventilation defect percent (VDP) . Thedefect quantification from gas images contains two main steps: (1) lung cavity segmentation and (2) defect measurements within the lung cavity. Although the manual defect segmentation demonstrated good interreader agreement , it is tedious, time-consuming, and subjective. For automated lung cavity segmentation, Ray et al. proposed merging active contours using the properties of fluid flow to segment the lung in each slice to obtain the total lung cavity volume. Tustison et al. proposed a shape model–based lung segmentation, which requires offline preprocessing to obtain the unbiased shape template. Guo et al. proposed to co-segment the lung cavity jointly from three-dimensional (3D) proton and  3 He MRI pairs. For quantitative measures of defect from  3 He MRI within the lung cavity, Tustison et al. used Atropos to partition the lungs into ventilated and unventilated regions with optimal parameter settings. The hierarchical _K_ -means method showed good spatial agreement relative to manual segmentation on subjects with COPD and CF and low spatial agreement on asthmatic subjects. Moreover, the histogram-based linear binning method proposed for defect quantification on  129 Xe images has not been assessed for  3 He images. Therefore, there is still a demand for a reliable, automated defect quantification method that is generally applicable for various lung conditions.

Three major confounding factors have made the defect quantification a difficult problem, especially in less-defected lungs. First, because of the inherent low-intensity presence on  3 He image, pulmonary vasculature regions are likely to be misclassified as ventilation defects in computer-aided detection. Second, the intensity inhomogeneity due to the nonuniform coil sensitivities can jeopardize the accuracy of intensity-based segmentation algorithms. Third, highly defected lungs tend to have smaller signal-intensity variations, whereas less-defected lungs tend to have more subtle signal heterogeneity requiring refined subclassification. In particular, asthmatic lungs are known to have spatially heterogeneous patterns of ventilation . This makes quantitative defect measurement, especially in mild asthma, a more challenging problem than in CF or COPD, where the ventilation defect is often persistent and focal. Therefore, a robust and reproducible defect quantification method for evaluating longitudinal progression and treatment response is of particular importance in asthma.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

## Human Subjects

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Spirometry

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 3  He Polarization and Image Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Overview of the Defect Segmentation Pipeline

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, The workflow of the adaptive K -means defect quantification: the registered proton image (a) was transformed to obtain a vessel-enhanced proton image (b) . The vesselness filter was then applied to estimate the pulmonary vasculature (c) . A retrospective coil sensitivity map was estimated from the raw helium-3 ( 3 He) image (d) to obtain the intensity-corrected 3 He image (e) . The adaptive K- means clustering was applied for the initial ventilation defect segmentation (f) with the defects contoured in green and yellow for the right and left lungs, respectively. A morphometric correction step was used to correct the vessels and partial volume effect for the final ventilation map (g) . Clusters 1 and 4 represent ventilation defects (blue) and highly ventilated regions (red).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/0_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Landmark-based Image Registration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Vasculature Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Estimation of the vascular mask. The pulmonary vasculature is not conspicuous in the registered proton images (a and e) and became more distinct on the contrast-enhanced proton images (b and f) . The vessel-like object map estimated by the vesselness filter was thresholded to obtain the binary vascular mask (c and g) with the edge of the lung outlined in white solid lines. The vessels present as low-intensity pixels on the sensitivity-corrected helium-3 ( 3 He) image in subject 1 (d) and a vessel is seen to merge into a large defect in subject 2 (h) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/1_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

T(x)=⎧⎩⎨⎪⎪⌈μ¯¯s+(x−μi)s1−μ¯sp1−μi⌉,⌈μ¯¯s+(x−μi)s2−μ¯sp2−μi⌉,ifp1≤x≤μiifμi≤x≤p2
T

(

x

)

=

{

⌈

μ

¯

s

+

(

x

−

μ

i

)

s

1

−

μ

¯

s

p

1

−

μ

i

⌉

,

if

p

1

≤

x

≤

μ

i

⌈

μ

¯

s

+

(

x

−

μ

i

)

s

2

−

μ

¯

s

p

2

−

μ

i

⌉

,

if

μ

i

≤

x

≤

p

2


where ⌈⌉
⌈

⌉
denotes the ceiling operation that rounds up to the nearest integer, _p  1_ and _p  2_ denote the minimum and maximum intensity values in the lungs, and _s  1_ and _s  2_ were chosen as 1 and 512 respectively. This transformation highlights those relatively low-intensity pixels below the _µ  i_ value. Consequently, the vascular structures on the contrast-enhanced proton images (  Fig 2b and f ) were more distinct relative to the raw proton images (  Fig 2a and e ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

V(RA​,RB)=exp(−RA/(2α2))⋅(1−exp(−RB/(2β2))),
V

(

R

A

​

,

R

B

)

=

exp

(

−

R

A

/

(

2

α

2

)

)

⋅

(

1

−

exp

(

−

R

B

/

(

2

β

2

)

)

)

,


where RA=(λ2/λ1)2
R

A

=

(

λ

2

/

λ

1

)

2
and RB=λ21+λ22
R

B

=

λ

1

2

+

λ

2

2
. Parameters _α_ and _β_ were selected as 0.5 and 15 respectively. A threshold <0.15 was applied on _V_ ( _R  A_ , _R  B_ ) to obtain the binary vasculature mask. The estimated vasculature masks (  Fig 2c and g ) were aligned with low-intensity vascular pixels in the corresponding  3 He (  Fig 2d and h ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Coil Sensitivity Correction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Coil sensitivity estimation. The first column displays the raw helium-3 ( 3 He) image. The middle column shows the estimated sensitivity map within the lungs, and the third column shows the intensity-corrected 3 He image. All images are plotted with the same grayscale window/level.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/2_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Adaptive _K_ -Means Clustering

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

PL=Voxel count in the first binSum of all lung voxels×100%.
P

L

=

Voxel count in the first bin

Sum of all lung voxels

×

100

%

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Defect cluster=⎧⎩⎨⎪⎪A.First two subclusters withK=5,B.First three subclusters withK=4,C.First cluster withK=4,PL<4%4%≤PL<10%PL≥10%
Defect cluster

=

{

A

.

First two subclusters with

K

=

5

,

P

L

<

4

%

B

.

First three subclusters with

K

=

4

,

4

%

≤

P

L

<

10

%

C

.

First cluster with

K

=

4

,

P

L

≥

10

%


![Figure 4, The adaptive clustering on ventilation defect based on the percent low-intensity signal P L . The P L value was calculated from the histogram of all lung voxels and used to adaptively determine the defect cluster with three options (A, B, or C) based on the extent of ventilation defect volume after two rounds of K -means clustering.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/3_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Morphometric Correction of Partial Volume Effect

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Manual Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

D=2⋅\|S∩M\|\|S\|+\|M\|.
D

=

2

⋅

\|

S

∩

M

\|

\|

S

\|

+

\|

M

\|

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Manual Versus Semiautomated Measurements

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, The segmented defects overlaid on the helium-3 ( 3 He) images obtained by the adaptive K -means, manual segmentation, and hierarchical K -means methods in the same subject at visit 1. The adaptive K -means results (defects shown as green and yellow contoured regions in the right and left lungs, respectively) on Row 1 effectively masked out the low-intensity, tubular-shaped vessels (white arrows) at baseline (a) , post challenge (b) , and recovery (c) similar to the manually segmented defects on Row 2 (d, e, and f) . However, the adaptive K -means showed discrepancies on the size and location of small defects. The hierarchical K -means included low-intensity voxels along the lung periphery due to partial volume effect at baseline (g) and vessels (g and i) . The large defects (h) detected by the hierarchical K -means appeared in a more scatter pattern and smaller compared to the manual (e) and adaptive K -means methods (b) likely due to the lack of intensity correction.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/4_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Bland-Altman plots for pairwise comparison between manual readers, adaptive K -means, and hierarchical K -means. The biases in ventilation defect percent (VDP) between adaptive K -means and two readers (a and b) were 1.12% and 1.34% respectively. The bias between the two manual readers (c) was 0.22%. The hierarchical K -means yielded a significant bias 6.1% (d) compared to Reader 1, which was mainly due to the over-segmentation at baseline and recovery. When vasculature was not removed in the adaptive K -means (e) , the bias of 2.2% was still insignificant. The VDP measurements are plotted separately at baseline (black circle), post challenge (dark-gray square), and recovery (light-gray diamond). The upper and lower bounds (dashed lines) were adjusted for repeated measures.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/5_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 1


Percent Change in Ventilation Defect Percent (ΔVDP) From Baseline to Post Challenge at Two Separate Visits Measured by Manual and Adaptive _K_ -means Methods


Subject Manual Adaptive _K_ -means ΔVDP Visit1 (%) ΔVDP Visit2 (%) ΔVDP Visit1 (%) ΔVDP Visit2 (%) 1 14.27 19.98 19.52 19.60 2 7.66 4.15 4.47 3.33 3 0.23 0.80 0.40 −0.61 4 8.57 15.34 3.58 13.20 5 0 1.02 −2.32 −2.49 6 14.69 14.45 16.85 22.06

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 2


Average Ventilation Defect Percent for Exercise Challenge Protocol in Subjects with EIB at Each of Two Visits


Visit Manual Adaptive _K-_ means Baseline Post Challenge Recovery Baseline Post Challenge Recovery Visit1 1.11 ± 1.12% 8.68 ± 7.41% 1.94 ± 1.47% 2.78 ± 1.63% 9.86 ± 8.21% 2.94 ± 2.67% Visit2 0.70 ± 0.81% 9.99 ± 8.97% 1.82 ± 1.36% 1.84 ± 1.50% 11.02 ± 9.77% 2.48 ± 2.90%

EIB, exercise-induced bronchoconstriction.


Values are mean ± standard deviation. Ventilation defect percent (%) was calculated as 100% × defect volumes/total lung volumes.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Correlation to Spirometric Measures

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 3


Spearman Correlation Between Whole Lung VDP and Spirometric Measures


FEV1/FVC %P FEV1%P_ρ__P_ value 95% CI_ρ__P_ value 95% CI Manual −0.63 <0.0001 \[−0.80, −0.38\] −0.54 0.00071 \[−0.75, −0.25\] Adaptive _K_ -means −0.64 <0.0001 \[−0.83, −0.38\] −0.40 0.016 \[−0.66, −0.049\]

CI, confidence interval; FEV1 %P, percent predicted forced expiratory volume in 1 second; FEV1/FVC %P, percent predicted FEV1 over forced vital capacity; VDP, ventilation defect percent.


A _P_ < 0.05 was considered significantly correlated.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Regional Variations in VDP

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Boxplots of the regional ventilation defect percent (VDP) at baseline, post challenge, and recovery using the two measurement methods. Despite qualitative trends, no significant differences in apical/basal regional dependence were observed by manual (a) and adaptive K -means (b) . Similarly, no significant differences in anterior/posterior dependence were observed by manual (c) and adaptive K -means (d) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/6_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Dice Coefficient

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 4


Dice Coefficients (Mean ± Standard Deviation) for Manual and Semiautomated Segmentation


Methods Ventilation Volume Defect Volume Reader 2 – Reader 1 0.99 ± 0.015 0.56 ± 0.31 Adaptive _K_ -means – Reader 1 0.98 ± 0.027 0.28 ± 0.24 Adaptive _K_ -means – Reader 2 0.97 ± 0.033 0.25 ± 0.21 Hierarchical _K_ -means – Reader 1 0.95 ± 0.013 0.16 ± 0.18 Adaptive _K_ -means 2 – Adaptive _K_ -means 1 1.00 ± 0.00033 0.99 ± 0.022

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Bar graph of the mean Dice coefficient between Reader 1 and adaptive K -means at various whole lung ventilation defect percent (VDP) values by manual segmentation. The measured VDP was categorized into six bins with values from 0% to more than 10%. The error bars represent the standard deviation of the Dice coefficient within each measured VDP bin. The spatial agreement between the two methods improved in more diseased lungs, where the whole lung VDP is higher.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomatedVentilationDefectQuantificationinExerciseinducedBronchoconstrictionUsingHyperpolarizedHelium3MagneticResonanceImaging/7_1s20S1076633216300733.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Fain S.B., Gonzalez-Fernandez G., Peterson E.T., et. al.: Evaluation of structure-function relationships in asthma using multidetector CT and hyperpolarized He-3 MRI. Acad Radiol 2008; 15: pp. 753-762.


- 2\. Niles D.J., Kruger S.J., Dardzinski B.J., et. al.: Exercise-induced bronchoconstriction: reproducibility of hyperpolarized 3He MR imaging. Radiology 2013; 266: pp. 618-625.


- 3\. de Lange E.E., Altes T.A., Patrie J.T., et. al.: Changes in regional airflow obstruction over time in the lungs of patients with asthma: evaluation with 3He MR imaging. Radiology 2009; 250: pp. 567-575.


- 4\. Altes T.A., Powers P.L., Knight-Scott J., et. al.: Hyperpolarized 3He MR lung ventilation imaging in asthmatics: preliminary findings. J Magn Reson Imaging 2001; 13: pp. 378-384.


- 5\. Sun Y., O'Sullivan B.P., Roche J.P., et. al.: Using hyperpolarized 3He MRI to evaluate treatment efficacy in cystic fibrosis patients. J Magn Reson Imaging 2011; 34: pp. 1206-1211.


- 6\. Bannier E., Cieslar K., Mosbah K., et. al.: Hyperpolarized 3He MR for sensitive imaging of ventilation function and treatment efficiency in young cystic fibrosis patients with normal lung function. Radiology 2010; 255: pp. 225-232.


- 7\. van Beek E.J.R., Hill C., Woodhouse N., et. al.: Assessment of lung disease in children with cystic fibrosis using hyperpolarized 3-Helium MRI: comparison with Shwachman score, Chrispin-Norman score and spirometry. Eur Radiol 2007; 17: pp. 1018-1024.


- 8\. Woodhouse N., Wild J.M., Paley M.N.J., et. al.: Combined helium-3/proton magnetic resonance imaging measurement of ventilated lung volumes in smokers compared to never-smokers. J Magn Reson Imaging 2005; 21: pp. 365-369.


- 9\. Mathew L., Kirby M., Etemad-Rezai R., et. al.: Hyperpolarized 3He magnetic resonance imaging: preliminary evaluation of phenotyping potential in chronic obstructive pulmonary disease. Eur J Radiol 2011; 79: pp. 140-146.


- 10\. Kirby M., Heydarian M., Svenningsen S., et. al.: Hyperpolarized 3He magnetic resonance functional imaging semiautomated segmentation. Acad Radiol 2012; 19: pp. 141-152.


- 11\. Panth S.R., Fain S.B., Holmes J.H., et. al.: Assessment of lung ventilation, gas trapping and pulmonary perfusion in patients with asthma during inhaled corticosteroid withdrawal.Proceedings of the 12th Annual Meeting of ISMRM.2004. Kyoto, Japan


- 12\. Donnelly L.F., Macfall J.R., Mcadams H.P., et. al.: Cystic fibrosis: combined hyperpolarised 3He-enchanced and conventional proton MR imaging in the lung—preliminary observations. Radiology 1999; 212: pp. 885-889.


- 13\. Tustison N.J., Avants B.B., Flors L., et. al.: Ventilation-based segmentation of the lungs using hyperpolarized (3)He MRI. J Magn Reson Imaging 2011; 34: pp. 831-841.


- 14\. He M., Kaushik S.S., Robertson S.H., et. al.: Extending semiautomatic ventilation defect analysis for hyperpolarized 129Xe ventilation MRI. Acad Radiol 2014; 21: pp. 1530-1541.


- 15\. Kruger S.J., Niles D.J., Dardzinski B., et. al.: Hyperpolarized Helium-3 MRI of exercise-induced bronchoconstriction during challenge and therapy. J Magn Reson Imaging 2014; 39: pp. 1230-1237.


- 16\. Guo F., Yuan J., Rajchl M., et. al.: Globally optimal co-segmentation of three-dimensional pulmonary 1H and hyperpolarized 3He MRI with spatial consistence prior. Med Image Anal 2015; 23: pp. 43-55.


- 17\. Pike D., Kirby M., Guo F., et. al.: Ventilation heterogeneity in ex-smokers without airflow limitation. Acad Radiol 2015; 22: pp. 1068-1078.


- 18\. Ray N., Acton S.T., Altes T., et. al.: Merging parametric active contours within homogeneous image regions for MRI-based lung segmentation. IEEE Trans Med Imaging 2003; 22: pp. 189-199.


- 19\. Frangi A.F., Member S., Niessen W.J., et. al.: Model-based quantitation of 3-D magnetic resonance angiographic images. IEEE Trans Med Imaging 1999; 18: pp. 946-956.


- 20\. Tustison N.J., Avants B.B., Cook P.A., et. al.: N4ITK: improved N3 bias correction. IEEE Trans Med Imaging 2010; 29: pp. 1310-1320.


- 21\. Parsons J.P., Hallstrand T.S., Mastronarde J.G., et. al.: An official American Thoracic Society clinical practice guideline: exercise-induced bronchoconstriction. Am J Respir Crit Care Med 2013; 187: pp. 1016-1027.


- 22\. Hankinson J.L., Odencrantz J.R., Fedan K.B.: Spirometric reference values from a sample of the general U.S. population. Am J Respir Crit Care Med 1999; 159: pp. 179-187.


- 23\. Möller H.E., Chen X.J., Saam B., et. al.: MRI of the lungs using hyperpolarized noble gases. Magn Reson Med 2002; 47: pp. 1029-1051.


- 24\. Kirby M., Wheatley A., McCormack D.G., et. al.: Development and application of methods to quantify spatial and temporal hyperpolarized 3He MRI ventilation dynamics: preliminary results in chronic obstructive pulmonary disease. SPIE 2010; pp. 762605-762609.


- 25\. Udupa J.K.: On standardizing the MR image intensity scale. Magn Reson Med 1999; 42: pp. 1072-1081.


- 26\. Otsu N.: A threshold selection method from gray-level histograms. IEEE Trans Syst Man Cybern 1979; 9: pp. 62-66.


- 27\. Bland J.M., Altman D.G.: Agreement between methods of measurement with multiple observations per individual. J Biopharm Stat 2007; 17: pp. 571-582.


- 28\. Haukoos J.S., Lewis R.J.: Advanced statistics: bootstrapping confidence intervals for statistics with “difficult” distributions. Acad Emerg Med 2005; 12: pp. 360-365.


- 29\. R Development Core Team : R: A language and environment for statistical computing.2012.R Foundation for Statistical ComputingVienna, Austria Available online at http://www.R-project.org/

- 30\. Virgincar R.S., Cleveland Z.I., Kaushik S.S., et. al.: Quantitative analysis of hyperpolarized (129) Xe ventilation imaging in healthy volunteers and subjects with chronic obstructive pulmonary disease. NMR Biomed 2013; 26: pp. 425-435.


- 31\. Avants B.B., Tustison N.J., Song G., et. al.: A reproducible evaluation of ANTs similarity metric performance in brain image registration. Neuroimage 2011; 54: pp. 2033-2044.


- 32\. Rueckert D., Sonoda L.I., Hayes C., et. al.: Nonrigid registration using free-form deformations: application to breast MR images. IEEE Trans Med Imaging 1999; 18: pp. 712-721.