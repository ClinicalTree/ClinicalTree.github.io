---
title: Reproducibility of Four-dimensional Computed Tomography-based Lung Ventilation Imaging
author: [CL_AT_TokihiroYamamotoPhD,CL_AT_SvenKabusPhD,CL_AT_JensvonBergPhD,CL_AT_CristianLorenzPhD,CL_AT_MelodyPChungBS,CL_AT_JulianCHongMS,CL_AT_BillyWLooMDPhD,CL_AT_PaulJKeallPhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 12]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

A novel ventilation imaging method based on four-dimensional (4D) computed tomography (CT) has been applied to the field of radiation oncology. Understanding its reproducibility is a prerequisite for clinical applications. The purpose of this study was to quantify the reproducibility of 4D CT ventilation imaging over different days and the same session.

## Materials and Methods

Two ventilation images were created from repeat 4D CT scans acquired over the average time frames of 15 days for 6 lung cancer patients and 5 minutes for another 6 patients. The reproducibility was quantified using the voxel-based Spearman rank correlation coefficients for all lung voxels and Dice similarity coefficients (DSC) for the spatial overlap of segmented high-, moderate-, and low-functional lung volumes. Furthermore, the relationship between the variation in abdominal motion range as a measure of the depth of breathing and variation in ventilation was evaluated using linear regression.

## Results

The voxel-based correlation between the two ventilation images was moderate on average (0.50 ± 0.15). The DSCs were also moderate for the high- (0.60 ± 0.08), moderate- (0.46 ± 0.06), and low-functional lung (0.58 ± 0.09). No patients demonstrated strong correlations. The relationship between the motion range variation and ventilation variation was found to be moderate and significant.

## Conclusions

We investigated the reproducibility of 4D CT ventilation imaging over the time frames of 15 days and 5 minutes and found that it was only moderately reproducible. Respiratory variation during 4D CT scans was found to deteriorate the reproducibility. Improvement of 4D CT imaging is necessary to increase the reproducibility of 4D CT ventilation imaging.

In recent years, there have been significant advances in molecular and functional imaging as applied to the field of radiation oncology. The most important applications include treatment planning, especially for dose painting (ie, boosting dose to active tumor subregions) and functional avoidance (ie, sparing dose from high-functional subregions of normal tissues) . The other important application is the assessment of tumor response to treatment and radiation-induced normal tissue injury . In lung cancer radiotherapy, lung ventilation or perfusion imaging with single photon emission computed tomography (SPECT) and magnetic resonance (MR) have been used in such applications. However, SPECT and MR imaging suffer from drawbacks such as low resolution, high cost, long scan time, and limited availability.

Lung ventilation images can be created by a novel technique based on four-dimensional (4D) computed tomography (CT) . The 4D CT-derived ventilation can be considered “free” information for lung cancer radiotherapy patients, because 4D CT scans are currently in routine use for treatment planning purposes at many centers (42.3%) and ventilation computation involves only image processing and analysis. Moreover, 4D CT ventilation imaging has higher resolution, lower cost, shorter scan time, and/or higher availability compared to SPECT or MR imaging. In the literature, there have been several applications of 4D CT ventilation imaging to functional avoidance and assessment of radiation-induced ventilation changes . Four-dimensional CT ventilation images have been found to vary widely with deformable image registration (DIR) algorithms and ventilation metrics , indicating the need for careful validation. Nevertheless, little validation has been performed to date. Several investigators evaluated the physiologic accuracy of 4D CT ventilation imaging by comparing with xenon CT ventilation imaging for animal subjects and found reasonable correlations . Major drawbacks of these studies include limited axial coverage (∼3 cm). Castillo et al and Yamamoto et al compared 4D CT and SPECT ventilation images for thoracic cancer patients. Although they observed some regional agreements, the correlations were low overall, which was at least in part due to central airway depositions of the SPECT radiotracer (ie, technetium-99m-labeled diethylenetriamine pentaacetate) aerosols. Positive data on human subjects include significantly lower 4D CT ventilation in emphysematous regions (ie, known low-signal regions) than in nonemphysematous regions (ie, known high-signal regions) for 12 lung cancer patients as demonstrated by Yamamoto et al . More recently, Castillo et al compared 4D CT ventilation and SPECT perfusion images for 10 lung cancer patients and demonstrated strong correlations in functional defect regions distal to airway obstruction because of gross tumor . These results indicate the potential for a high physiologic accuracy of 4D CT ventilation imaging. Given the lack of data showing strong correlations with ground truth ventilation imaging for human subjects, however, further studies are necessary. In addition, the reproducibility should also be investigated, which is particularly important for longitudinal studies such as the assessment of radiation-induced ventilation changes. Recently, Du et al investigated the reproducibility of 4D CT ventilation imaging using repeat 4D CT scans acquired over less than 10 minutes for three anesthetized, mechanically ventilated sheep and nine lung cancer patients . They found high reproducibility for sheep, but relatively poor reproducibility for patients.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Material and methods

## Patients

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 4D CT Ventilation Imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

J(x,y,z)=∣∣∣∣∣∣∣1+∂ux(x,y,z)∂x∂uy(x,y,z)∂x∂uz(x,y,z)∂x∂ux(x,y,z)∂y1+∂uy(x,y,z)∂y∂uz(x,y,z)∂y∂ux(x,y,z)∂z∂uy(x,y,z)∂z1+∂uz(x,y,z)∂z∣∣∣∣∣∣∣,
J

(

x

,

y

,

z

)

=

\|

1

+

∂

u

x

(

x

,

y

,

z

)

∂

x

∂

u

x

(

x

,

y

,

z

)

∂

y

∂

u

x

(

x

,

y

,

z

)

∂

z

∂

u

y

(

x

,

y

,

z

)

∂

x

1

+

∂

u

y

(

x

,

y

,

z

)

∂

y

∂

u

y

(

x

,

y

,

z

)

∂

z

∂

u

z

(

x

,

y

,

z

)

∂

x

∂

u

z

(

x

,

y

,

z

)

∂

y

1

+

∂

u

z

(

x

,

y

,

z

)

∂

z

\|

,


which represents the differential contraction or expansion at point (x,y,z)
(

x

,

y

,

z

)
. The volume of each exhale voxel deformed into the inhale phase (Volvoxelin)
(

Vol

in

voxel

)
can be estimated by


Volvoxelin(x,y,z)=Volvoxelex(x,y,z)⋅J(x,y,z),
Vol

in

voxel

(

x

,

y

,

z

)

=

Vol

ex

voxel

(

x

,

y

,

z

)

⋅

J

(

x

,

y

,

z

)

,


where Volvoxelex
Vol

ex

voxel
is the exhale voxel volume. In this study, the ventilation metric (V)
(

V

)
was defined as exhale-to-inhale volume change and can be expressed as


V(x,y,z)=Volvoxelin(x,y,z)−Volvoxelex(x,y,z)=Volvoxelex⋅{J(x,y,z)−1}.
V

(

x

,

y

,

z

)

=

Vol

in

voxel

(

x

,

y

,

z

)

−

Vol

ex

voxel

(

x

,

y

,

z

)

=

Vol

ex

voxel

⋅

{

J

(

x

,

y

,

z

)

−

1

}

.


A value of zero corresponds to local volume preservation. A negative value represents local contraction, and a positive value represents local expansion. Thus 4D CT ventilation images at the peak-exhale phase were created for the first (V1st)
(

V

1

st

)
and second (V2nd)
(

V

2

nd

)
scans. Further details on each step of 4D CT ventilation imaging have been described elsewhere .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantification of the Tidal Volume

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Volair(x,y,z)=−HU(x,y,z)1000Volvoxel(x,y,z),
Vol

air

(

x

,

y

,

z

)

=

−

HU

(

x

,

y

,

z

)

1000

Vol

voxel

(

x

,

y

,

z

)

,


where HU
HU
is the Hounsfield unit value . Note that the air and tissue densities were assumed to be −1000 and 0 HU, respectively. Second, the air volume in the peak-exhale lung was subtracted from that of the peak-inhale lung to determine a tidal volume.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantification of the Reproducibility of 4D CT Ventilation Imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


DSC=2⋅FLV1st∩FLV2ndFLV1st+FLV2nd,
D

S

C

=

2

⋅

F

L

V

1

st

∩

F

L

V

2

nd

F

L

V

1

st

+

F

L

V

2

nd

,


where FLV
F

L

V
is the segmented high-, moderate-, or low-functional lung volume.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

V(x,y,z)=Volvoxelex{J(x,y,z)−1}V¯¯¯.
V

(

x

,

y

,

z

)

=

Vol

ex

voxel

{

J

(

x

,

y

,

z

)

−

1

}

V

¯

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Regression Analysis for the Relationship between the Abdominal Motion Range Variation and 4D CT Ventilation Variation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ΔV(x,y,z)=V2nd(x,y,z)−V1st(x,y,z).
Δ

V

(

x

,

y

,

z

)

=

V

2

nd

(

x

,

y

,

z

)

−

V

1

st

(

x

,

y

,

z

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δm(x,y,z)=m2nd(x,y,z)m2nd¯¯¯¯¯¯¯−m1st(x,y,z)m1st¯¯¯¯¯¯¯.
Δ

m

(

x

,

y

,

z

)

=

m

2

nd

(

x

,

y

,

z

)

m

2

nd

¯

−

m

1

st

(

x

,

y

,

z

)

m

1

st

¯

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Vm(x,y,z)=V(x,y,z)m(x,y,z).
V

m

(

x

,

y

,

z

)

=

V

(

x

,

y

,

z

)

m

(

x

,

y

,

z

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Patients

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Characteristics of Patients and Repeat 4D CT Scans for 12 Patients


Patient Scan Gender Age (y) Histology and Stage Time Frame AV Biofeedback Used? Arm Position Immobilization Device Used? Peak-exhale Lung (Air) Volume (cm  3  ) Peak-inhale Lung (Air) Volume (cm  3  ) Tidal Volume (cm  3  ) Average Abdominal Motion Range (cm)**Different-day cohort** 1 First Male 78 NSCLC, stage I 13 days Yes Up Yes 4742 (3898) 5439 (4546) 648 1.25 Second Yes Down No 3863 (2912) 4936 (3706) 794 1.28 2 First Male 66 NSCLC, stage III 12 days Yes Up Yes 3681 (2889) 4055 (3241) 352 1.02 Second Yes Down No 3615 (1955) 4349 (2367) 412 1.37 3 First Male 62 NSCLC, stage III 9 days No Up Yes 5896 (4727) 6386 (5176) 449 0.64 Second No Down No 5537 (3897) 6532 (4481) 584 1.04 4 First Male 82 NSCLC, stage IV 8 days Yes Up Yes 7812 (6694) 8130 (6983) 289 0.43 Second Yes Up Yes 8436 (4993) 9021 (5492) 499 0.51 5 First Male 67 NSCLC, stage IV 30 days Yes Up Yes 5021 (4019) 5735 (4710) 691 0.97 Second Yes Up Yes 4748 (3307) 5655 (4108) 800 0.97 6 First Male 77 NSCLC, stage II 15 days No Up Yes 6622 (5663) 7126 (6142) 479 0.95 Second No Down No 6145 (4771) 6624 (5211) 441 0.95**Same-session Cohort** 1 First Male 60 NSCLC, stage IV 5 min No Down Yes 3470 (2579) 3712 (2869) 290 0.65 Second Yes Down Yes 3508 (2579) 3837 (2853) 275 0.64 2 First Female 74 NSCLC, stage I 6 min Yes Down Yes 2837 (1887) 3430 (2445) 558 0.66 Second No Down Yes 2645 (1765) 3356 (2369) 604 0.65 3 First Male 61 NSCLC, stage I 5 min No Up Yes 4382 (3448) 4711 (3719) 272 0.59 Second Yes Up Yes 4564 (3404) 4971 (3705) 301 0.57 4 First Female 57 Metastatic tumor 5 min Yes Up Yes 1418 (854) 2004 (1397) 543 0.95 Second No Up Yes 1375 (822) 1786 (1240) 418 0.62 5 First Male 59 NSCLC, stage III 5 min No Up Yes 4257 (3428) 4860 (3993) 566 0.74 Second Yes Up Yes 4839 (3343) 5020 (3859) 516 0.36 6 First Female 67 NSCLC, stage III 4 min No Up Yes 2467 (1884) 2879 (2266) 382 0.66 Second Yes Up Yes 2575 (1823) 2953 (2187) 364 0.70

4D, four-dimensional; AV, audiovisual; CT, computed tomography; NSCLC, non–small-cell lung cancer.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reproducibility of 4D CT Ventilation Imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Comparison of the first and second peak-exhale four-dimensional (4D) computed tomography (CT) and ventilation images at different coronal levels for patient 1 of the same-session cohort, showing the highest correlation in that cohort with the voxel-based Spearman correlation coefficient of 0.75. Note that ventilation is normalized by the overall mean value and that the second 4D CT and ventilation images are propagated to the domain of the first scan.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ReproducibilityofFourdimensionalComputedTomographybasedLungVentilationImaging/0_1s20S1076633212003844.jpg)

![Figure 2, Comparison of the 1st and 2nd peak-exhale four-dimensional (4D) computed tomography (CT) and ventilation images at different coronal levels for patient 6 of the different-day cohort, showing the lowest correlation in that cohort with the voxel-based Spearman correlation coefficient of 0.36. Note that ventilation is normalized by the overall mean value and that the second 4D CT and ventilation images are propagated to the domain of the first scan.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ReproducibilityofFourdimensionalComputedTomographybasedLungVentilationImaging/1_1s20S1076633212003844.jpg)

Table 2


Voxel-based Spearman Correlation Coefficients (All Voxels within the Lung) and Dice Similarity Coefficients (Segmented Functional Lung Volumes) between the First and Second Four-dimensional Computed Tomography Ventilation Images for 12 Patients


Patient Voxel-based Correlation Dice Similarity Coefficient High Moderate Low**Different-day cohort** 1 0.50 0.57 0.43 0.56 2 0.65 0.66 0.44 0.65 3 0.38 0.56 0.40 0.47 4 0.45 0.56 0.46 0.56 5 0.53 0.60 0.44 0.54 6 0.36 0.54 0.44 0.53 Mean ± SD 0.48 ± 0.11 0.58 ± 0.05 0.44 ± 0.02 0.55 ± 0.06**Same-session cohort** 1 0.75 0.72 0.59 0.76 2 0.66 0.64 0.47 0.67 3 0.42 0.60 0.49 0.57 4 0.69 0.74 0.54 0.67 5 0.34 0.49 0.38 0.52 6 0.31 0.51 0.46 0.51 Mean ± SD 0.53 ± 0.20 0.62 ± 0.11 0.49 ± 0.07 0.62 ± 0.10**All patients** Mean ± SD 0.50 ± 0.15 0.60 ± 0.08 0.46 ± 0.06 0.58 ± 0.09

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Relationship between the Abdominal Motion Range Variation and 4D CT Ventilation Variation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Comparison of the abdominal motion range images of the first scan, second scan, and variation between the two scans for patient 1 of the same-session cohort and patient 6 of the different-day cohort. The standard deviation of motion range variation of patient 1 of the same-session cohort was 0.21, which was markedly smaller than 0.41 of patient 6 of the different-day cohort. Note that motion range is normalized by the overall mean value and that the second motion range images are propagated to the domain of the first scan.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ReproducibilityofFourdimensionalComputedTomographybasedLungVentilationImaging/2_1s20S1076633212003844.jpg)

![Figure 4, Standard deviations of abdominal motion range variations versus voxel-based Spearman correlation coefficients between the first and second four-dimensional (4D) computed tomography (CT) ventilation images for 12 patients, showing a moderate, significant linear relationship ( r 2 = 0.55, P < .01). The line of best fit is also shown.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ReproducibilityofFourdimensionalComputedTomographybasedLungVentilationImaging/3_1s20S1076633212003844.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, (a) Comparison of the images of abdominal motion range variation and four-dimensional (4D) computed tomography (CT) ventilation variation at different coronal levels for patient 2 of the different-day cohort, showing the strongest linear relationship ( r 2 = 0.90, P < .01). (b) Abdominal motion range variation versus 4D CT ventilation variation for the same patient. Points represent the average ventilation variations within motion range variation bins. Error bars represent the standard deviations.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ReproducibilityofFourdimensionalComputedTomographybasedLungVentilationImaging/4_1s20S1076633212003844.jpg)

![Figure 6, (a) Comparison of the images of abdominal motion range variation and four-dimensional (4D) computed tomography (CT) ventilation variation at different coronal levels for patient 6 of the different-day cohort, showing the weakest linear relationship ( r 2 = 0.01, P = .83). (b) Abdominal motion range variation versus 4D CT ventilation variation for the same patient. Points represent the average ventilation variations within motion range variation bins. Error bars represent the standard deviations.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ReproducibilityofFourdimensionalComputedTomographybasedLungVentilationImaging/5_1s20S1076633212003844.jpg)

Table 3


Slopes, _r_ 2  , and _P_ Values of the Linear Regression Models for the Relationship between the Abdominal Motion Range Variation and Four-dimensional Computed Tomography Ventilation Variation for 12 Patients


Patient Slope_r_ 2 _P_ Value**Different-day cohort** 1 0.88 0.81 <.01 2 0.70 0.90 <.01 3 0.48 0.29 .06 4 0.30 0.23 .03 5 0.55 0.35 .30 6 −0.04 0.01 .83**Same-session cohort** 1 0.33 0.07 .44 2 1.11 0.85 <.01 3 0.17 0.02 .65 4 1.03 0.83 <.01 5 0.35 0.28 <.01 6 0.46 0.41 .01**All patients** 0.26 0.42 <.01

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Comparison of the images of the first and second abdominal motion range, and four-dimensional (4D) computed tomography (CT) ventilation without and with motion range-based linear normalization for patient 1 of the different-day cohort, showing the largest improvement in the voxel-based correlation between the two ventilation images from 0.50 to 0.56. Motion range-based normalization increased or decreased regional ventilation as denoted by white arrows in the first ventilation image and resulted in better agreements with the second ventilation image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ReproducibilityofFourdimensionalComputedTomographybasedLungVentilationImaging/6_1s20S1076633212003844.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Ling C.C., Humm J., Larson S., et. al.: Towards multidimensional radiotherapy (MD-CRT): biological imaging and biological conformality. Int J Radiat Oncol Biol Phys 2000; 47: pp. 551-560.


- 2\. Brahme A.: Biologically optimized 3-dimensional in vivo predictive assay-based radiation therapy using positron emission tomography-computerized tomography imaging. Acta Oncol 2003; 42: pp. 123-136.


- 3\. Bentzen S.M.: Theragnostic imaging for radiation oncology: dose-painting by numbers. Lancet Oncol 2005; 6: pp. 112-117.


- 4\. Marks L.B., Spencer D.P., Bentel G.C., et. al.: The utility of SPECT lung perfusion scans in minimizing and assessing the physiologic consequences of thoracic irradiation. Int J Radiat Oncol Biol Phys 1993; 26: pp. 659-668.


- 5\. Ireland R.H., Bragg C.M., McJury M., et. al.: Feasibility of image registration and intensity-modulated radiotherapy planning with hyperpolarized helium-3 magnetic resonance imaging for non-small-cell lung cancer. Int J Radiat Oncol Biol Phys 2007; 68: pp. 273-281.


- 6\. Yaremko B.P., Guerrero T.M., Noyola-Martinez J., et. al.: Reduction of normal lung irradiation in locally advanced non-small-cell lung cancer patients, using ventilation images for functional avoidance. Int J Radiat Oncol Biol Phys 2007; 68: pp. 562-571.


- 7\. Chen K., Chen X.: Positron emission tomography imaging of cancer biology: current status and future prospects. Semin Oncol 2011; 38: pp. 70-86.


- 8\. Boersma L.J., Damen E.M., de Boer R.W., et. al.: A new method to determine dose-effect relations for local lung-function changes using correlated SPECT and CT data. Radiother Oncol 1993; 29: pp. 110-116.


- 9\. Usenius T., Usenius J.P., Tenhunen M., et. al.: Radiation-induced changes in human brain metabolites as studied by 1H nuclear magnetic resonance spectroscopy in vivo. Int J Radiat Oncol Biol Phys 1995; 33: pp. 719-724.


- 10\. Munden R.F., Erasmus J.J., Smythe W.R., et. al.: Radiation injury to the liver after intensity-modulated radiation therapy in patients with mesothelioma: an unusual CT appearance. AJR Am J Roentgenol 2005; 184: pp. 1091-1095.


- 11\. Seppenwoolde Y., Muller S.H., Theuws J.C., et. al.: Radiation dose-effect relations and local recovery in perfusion for patients with non-small-cell lung cancer. Int J Radiat Oncol Biol Phys 2000; 47: pp. 681-690.


- 12\. Seppenwoolde Y., Engelsman M., De Jaeger K., et. al.: Optimizing radiation treatment plans for lung cancer using lung perfusion information. Radiother Oncol 2002; 63: pp. 165-177.


- 13\. Das S.K., Miften M.M., Zhou S., et. al.: Feasibility of optimizing the dose distribution in lung tumors using fluorine-18-fluorodeoxyglucose positron emission tomography and single photon emission computed tomography guided dose prescriptions. Med Phys 2004; 31: pp. 1452-1461.


- 14\. Christian J.A., Partridge M., Nioutsikou E., et. al.: The incorporation of SPECT functional lung imaging into inverse radiotherapy planning for non-small cell lung cancer. Radiother Oncol 2005; 77: pp. 271-277.


- 15\. McGuire S.M., Zhou S., Marks L.B., et. al.: A methodology for using SPECT to reduce intensity-modulated radiation therapy (IMRT) dose to functioning lung. Int J Radiat Oncol Biol Phys 2006; 66: pp. 1543-1552.


- 16\. Lavrenkov K., Christian J.A., Partridge M., et. al.: A potential to reduce pulmonary toxicity: the use of perfusion SPECT with IMRT for functional lung avoidance in radiotherapy of non-small cell lung cancer. Radiother Oncol 2007; 83: pp. 156-162.


- 17\. Shioyama Y., Jang S.Y., Liu H.H., et. al.: Preserving functional lung using perfusion imaging and intensity-modulated radiation therapy for advanced-stage non-small cell lung cancer. Int J Radiat Oncol Biol Phys 2007; 68: pp. 1349-1358.


- 18\. Gayed I.W., Chang J., Kim E.E., et. al.: Lung perfusion imaging can risk stratify lung cancer patients for the development of pulmonary complications after chemoradiation. J Thorac Oncol 2008; 3: pp. 858-864.


- 19\. Zhang J., Ma J., Zhou S., et. al.: Radiation-induced reductions in regional lung perfusion: 0.1–12 year data from a prospective clinical study. Int J Radiat Oncol Biol Phys 2010; 76: pp. 425-432.


- 20\. Ward E.R., Hedlund L.W., Kurylo W.C., et. al.: Proton and hyperpolarized helium magnetic resonance imaging of radiation-induced lung injury in rats. Int J Radiat Oncol Biol Phys 2004; 58: pp. 1562-1569.


- 21\. Cai J., Mata J.F., Orton M.D., et. al.: A rabbit irradiation platform for outcome assessment of lung stereotactic radiosurgery. Int J Radiat Oncol Biol Phys 2009; 73: pp. 1588-1595.


- 22\. Ireland R.H., Din O.S., Swinscoe J.A., et. al.: Detection of radiation-induced lung injury in non-small cell lung cancer patients using hyperpolarized helium-3 magnetic resonance imaging. Radiother Oncol 2010; 97: pp. 244-248.


- 23\. Allen A.M., Albert M., Caglar H.B., et. al.: Can hyperpolarized helium MRI add to radiation planning and follow-up in lung cancer?. J Appl Clin Med Phys 2011; 12: pp. 3357.


- 24\. Guerrero T., Sanders K., Noyola-Martinez J., et. al.: Quantification of regional ventilation from treatment planning CT. Int J Radiat Oncol Biol Phys 2005; 62: pp. 630-634.


- 25\. Simpson D.R., Lawson J.D., Nath S.K., et. al.: Utilization of advanced imaging technologies for target delineation in radiation oncology. J Am Coll Radiol 2009; 6: pp. 876-883.


- 26\. Yamamoto T., Kabus S., von Berg J., et. al.: Impact of four-dimensional computed tomography pulmonary ventilation imaging-based functional avoidance for lung cancer radiotherapy. Int J Radiat Oncol Biol Phys 2011; 79: pp. 279-288.


- 27\. Ding K., Bayouth J.E., Buatti J.M., et. al.: 4DCT-based measurement of changes in pulmonary function following a course of radiation therapy. Med Phys 2010; 37: pp. 1261-1272.


- 28\. Vinogradskiy Y.Y., Castillo R., Castillo E., et. al.: Use of weekly 4DCT-based ventilation maps to quantify changes in lung function for patients undergoing radiation therapy. Med Phys 2012; 39: pp. 289-298.


- 29\. Yamamoto T., Kabus S., Klinder T., et. al.: Four-dimensional computed tomography pulmonary ventilation images vary with deformable image registration algorithms and metrics. Med Phys 2011; 38: pp. 1348-1358.


- 30\. Fuld M.K., Easley R.B., Saba O.I., et. al.: CT-measured regional specific volume change reflects regional ventilation in supine sheep. J Appl Physiol 2008; 104: pp. 1177-1184.


- 31\. Reinhardt J.M., Ding K., Cao K., et. al.: Registration-based estimates of local lung tissue expansion compared to xenon CT measures of specific ventilation. Med Image Anal 2008; 12: pp. 752-763.


- 32\.  Ding K, Cao K, Amelon RE, et al. Comparison of intensity- and Jacobian-based estimates of lung regional ventilation. Proc. of the Third International Workshop on Pulmonary Image Analysis, MICCAI 2010:49–60.


- 33\. Castillo R., Castillo E., Martinez J., et. al.: Ventilation from four-dimensional computed tomography: density versus Jacobian methods. Phys Med Biol 2010; 55: pp. 4661-4685.


- 34\.  Yamamoto T, Kabus S, von Berg J, et al. Evaluation of four-dimensional (4D) computed tomography (CT) pulmonary ventilation imaging by comparison with single photon emission computed tomography (SPECT) scans for a lung cancer patient. Proc. of the Third International Workshop on Pulmonary Image Analysis, MICCAI. 2010; 117–128.


- 35\. Yamamoto T., Kabus S., Klinder T., et. al.: Investigation of four-dimensional computed tomography-based pulmonary ventilation imaging in patients with emphysematous lung regions. Phys Med Biol 2011; 56: pp. 2279-2298.


- 36\. Castillo R., Castillo E., McCurdy M., et. al.: Spatial correspondence of 4D CT ventilation and SPECT pulmonary perfusion defects in patients with malignant airway stenosis. Phys Med Biol 2012; 57: pp. 1855-1871.


- 37\. Du K., Bayouth J.E., Cao K., et. al.: Reproducibility of registration-based measures of lung tissue expansion. Med Phys 2012; 39: pp. 1595-1608.


- 38\. Rietzel E., Pan T., Chen G.T.: Four-dimensional computed tomography: image formation and clinical protocol. Med Phys 2005; 32: pp. 874-889.


- 39\.  Kabus S, Lorenz C. Fast elastic image registration. Proc Med Image Analysis Clinic - A Grand Challenge, MICCAI. 2010; 81–89.


- 40\.  Kabus S, Klinder T, Murphy K, et al. Evaluation of 4D-CT Lung Registration. In: Yang GZ, Hawkes DJ, Rueckert D, et al, eds. Proc MICCAI. London, UK; 2009; 747–754.


- 41\.  Kabus S, von Berg J, Yamamoto T, et al. Lung ventilation estimation based on 4D-CT imaging. Proc First International Workshop on Pulmonary Image Analysis, MICCAI; 2008; 73–81.


- 42\. Guerrero T., Sanders K., Castillo E., et. al.: Dynamic ventilation imaging from four-dimensional computed tomography. Phys Med Biol 2006; 51: pp. 777-791.


- 43\. Hoffman E.A., Ritman E.L.: Effect of body orientation on regional lung expansion in dog and sloth. J Appl Physiol 1985; 59: pp. 481-491.


- 44\. Dice L.R.: Measures of the amount of ecologic association between species. Ecology 1945; 26: pp. 297-302.


- 45\. Zou K.H., Tuncali K., Silverman S.G.: Correlation and simple linear regression. Radiology 2003; 227: pp. 617-622.


- 46\. Landis J.R., Koch G.G.: The measurement of observer agreement for categorical data. Biometrics 1977; 33: pp. 159-174.


- 47\. Zou K.H., Warfield S.K., Bharatha A., et. al.: Statistical validation of image segmentation quality based on a spatial overlap index. Acad Radiol 2004; 11: pp. 178-189.


- 48\. Mathew L., Evans A., Ouriadov A., et. al.: Hyperpolarized 3He magnetic resonance imaging of chronic obstructive pulmonary disease: reproducibility at 3.0 tesla. Acad Radiol 2008; 15: pp. 1298-1311.


- 49\. Parraga G., Mathew L., Etemad-Rezai R., et. al.: Hyperpolarized 3He magnetic resonance imaging of ventilation defects in healthy elderly volunteers: initial findings at 3.0 Tesla. Acad Radiol 2008; 15: pp. 776-785.


- 50\. Woodhouse N., Wild J.M., van Beek E.J., et. al.: Assessment of hyperpolarized 3He lung MRI for regional evaluation of interventional therapy: a pilot study in pediatric cystic fibrosis. J Magn Reson Imaging 2009; 30: pp. 981-988.


- 51\. Amis T.C., Crawford A.B., Davison A., et. al.: Distribution of inhaled 99mtechnetium labelled ultrafine carbon particle aerosol (Technegas) in human lungs. Eur Respir J 1990; 3: pp. 679-685.


- 52\. Yamamoto T., Langner U., Loo B.W., et. al.: Retrospective analysis of artifacts in four-dimensional CT images of 50 abdominal and thoracic radiotherapy patients. Int J Radiat Oncol Biol Phys 2008; 72: pp. 1250-1258.


- 53\. Iwasawa T., Yoshiike Y., Saito K., et. al.: Paradoxical motion of the hemidiaphragm in patients with emphysema. J Thorac Imaging 2000; 15: pp. 191-195.


- 54\. Iwasawa T., Kagei S., Gotoh T., et. al.: Magnetic resonance analysis of abnormal diaphragmatic motion in patients with emphysema. Eur Respir J 2002; 19: pp. 225-231.


- 55\. Vedam S.S., Kini V.R., Keall P.J., et. al.: Quantifying the predictability of diaphragm motion during respiration with a noninvasive external marker. Med Phys 2003; 30: pp. 505-513.


- 56\. Ahn S., Yi B., Suh Y., et. al.: A feasibility study on the prediction of tumour location in the lung from skin motion. Br J Radiol 2004; 77: pp. 588-596.


- 57\. Hoisak J.D., Sixel K.E., Tirona R., et. al.: Correlation of lung tumor motion with external surrogate indicators of respiration. Int J Radiat Oncol Biol Phys 2004; 60: pp. 1298-1306.


- 58\. Couser J.I., Martinez F.J., Celli B.R.: Respiratory response and ventilatory muscle recruitment during arm elevation in normal subjects. Chest 1992; 101: pp. 336-340.


- 59\. Kini V.R., Vedam S.S., Keall P.J., et. al.: Patient training in respiratory-gated radiotherapy. Med Dosim 2003; 28: pp. 7-11.


- 60\. George R., Chung T.D., Vedam S.S., et. al.: Audio-visual biofeedback for respiratory-gated radiotherapy: impact of audio instruction and audio-visual biofeedback on respiratory-gated radiotherapy. Int J Radiat Oncol Biol Phys 2006; 65: pp. 924-933.


- 61\. Venkat R.B., Sawant A., Suh Y., et. al.: Development and preliminary evaluation of a prototype audiovisual biofeedback device incorporating a patient-specific guiding waveform. Phys Med Biol 2008; 53: pp. N197-N208.


- 62\. Keall P.J., Vedam S.S., George R., et. al.: Respiratory regularity gated 4D CT acquisition: concepts and proof of principle. Australas Phys Eng Sci Med 2007; 30: pp. 211-220.


- 63\. Langner U.W., Keall P.J.: Prospective displacement and velocity-based cine 4D CT. Med Phys 2008; 35: pp. 4501-4512.


- 64\. Langner U.W., Keall P.J.: Quantification of artifact reduction with real-time cine four-dimensional computed tomography acquisition methods. Int J Radiat Oncol Biol Phys 2010; 76: pp. 1242-1250.


- 65\. Hein P.A., Romano V.C., Lembcke A., et. al.: Initial experience with a chest pain protocol using 320-slice volume MDCT. Eur Radiol 2009; 19: pp. 1148-1155.