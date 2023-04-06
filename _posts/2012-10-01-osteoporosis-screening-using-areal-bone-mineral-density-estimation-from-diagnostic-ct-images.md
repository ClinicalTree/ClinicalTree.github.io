---
title: Osteoporosis Screening Using Areal Bone Mineral Density Estimation from Diagnostic CT Images
author: [Wei-Liang Tay BEng,Chee-Kong Chui PhD,Sim-Heng Ong PhD,Alvin Choong-Meng Ng MBBS MMed MRCP (UK)]
date: 2012-10-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 10 SOURCE CL_S_AcademicRadiologyVolume19Issue10 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

A reliable and cost-effective method for osteoporosis screening is important in addressing the increase in osteoporotic fractures due to aging populations. Diagnostic computed tomographic (dCT) images may contain densitometric information useful for osteoporosis screening. The aim of this study was to investigate the relationship between areal bone mineral density (aBMD) and volumetric information on dCT imaging and its suitability for building an osteopenia screening system. The goal of this system is to estimate aBMD and predict bone disease condition on the basis of dCT images of the lumbar spine.

## Materials and Methods

Dual-energy x-ray absorptiometry (DXA) aBMD and computed tomographic (CT) images were obtained from 44 male patients (mean age, 60 years). An aBMD from CT images (aBMD  CT ) was computed from the CT volume using established relationships of Hounsfield units to bone density and used to estimate DXA-derived aBMD (aBMD  DxA ). Estimated aBMD  CT was then applied to diagnose osteopenia of the lumbar spine using statistical methods.

## Results

For the estimation of aBMD  DxA from aBMD  CT , the proposed approach yielded a high correlation factor of _r_ = 0.852, with a root mean square error of 0.0884 g/cm  2 . The correlation was strongest when every slice in the dCT volume and both trabecular and cortical bone components were used. The classifier achieved an overall classification accuracy of 80.1% and an area under the receiver-operating characteristic curve of 0.894.

## Conclusions

This clinical study demonstrates that aBMD  DxA can be determined from routine CT data. Estimated aBMD  DxA can be extended to form a dCT imaging–based opportunistic screening system for the detection and management of osteopenia.

Osteoporosis is a skeletal disease characterized by low bone mass and microarchitectural deterioration of bone tissue, with consequent increases in bone fragility and susceptibility to fracture. The progression of osteoporosis is often gradual, with few obvious symptoms before bone fracture . Therefore, osteoporosis must be detected and treated early to avoid fragility fractures. The main methods of diagnosing osteoporosis are the use of bone mineral density (BMD) values measured by dual-energy x-ray absorptiometry (DXA) and quantitative computed tomographic (QCT) imaging. Unfortunately, the frequency of bone screening among the population is still low. One way to improve screening rates is to exploit the densitometric information contained in diagnostic computed tomographic (dCT) images performed for other medical reasons, such as presurgical planning or diagnosis of diseases. Opportunistic osteoporosis screening using routine computed tomographic (CT) images allows physicians to receive early notification of potential bone loss and the opportunity to prescribe measures for early treatment or management.

QCT imaging can be distinguished from dCT imaging in that it is a dedicated CT technique to determine BMD. QCT imaging also requires the use of calibration, whereas dCT imaging may be used in the absence of calibration for diagnosis or presurgical planning. Although dCT imaging is performed more frequently because of the generality of its application, bone assessments cannot currently be made on the basis of dCT scans, because the absence of calibration phantoms means that dCT BMD values are less reliable than QCT BMD values. Diagnostic CT imaging is also often performed with the use of an intravenous contrast agent, which further affects BMD measurements.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Overview

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Overview of the three-stage areal bone mineral density (aBMD) prediction and osteopenia screening system, performing perform preprocessing, aBMD prediction, and osteopenia classification tasks. CT, computed tomographic; DXA, dual-energy x-ray absorptiometry; HU, Hounsfield units.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/OsteoporosisScreeningUsingArealBoneMineralDensityEstimationfromDiagnosticCTImages/0_1s20S1076633212003248.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Vertebral Body Segmentation and HU Correction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Vertebra localization and segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Vertebral body segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Two examples of vertebral body segmentation. (a) includes the detected rib bones for context, while (b) contains only the extracted region of interest. In each image, the red outer boundary is the extracted region of interest for the vertebra, the red x is the guess for the vertebral body centroid, and the blue o is the centroid of the spinal canal. The green line is the line connecting the two centroids, and the red square and the blue lines are the detected cutoff point and cutoff lines, respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/OsteoporosisScreeningUsingArealBoneMineralDensityEstimationfromDiagnosticCTImages/1_1s20S1076633212003248.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Intensity correction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


HUoffset=+40−μmuscle,
HU

offset

=

+

40

−

μ

muscle

,


is then added to each voxel of the segmented vertebral body.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Generation of aBMD  CT  from Routine CT Images

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ρ=1.112×HU+47kg/m3.
ρ

=

1.112

×

HU

+

47

kg

/

m

3

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

BMCCT=∑ρ×Sy×S2x.
BMC

CT

=

∑

ρ

×

S

y

×

S

x

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Abone=Apixel×Sy×Sx.
A

bone

=

A

pixel

×

S

y

×

S

x

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

aBMDCT=BMCCTAbone.
aBMD

CT

=

BMC

CT

A

bone

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Regression of aBMD  DxA  from aBMD  CT

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

aBMDCT=k1×aBMDDXA+k2,
aBMD

CT

=

k

1

×

aBMD

DXA

+

k

2

,


where k1
k

1
and k2
k

2
are the scaling and offset constants, respectively. This assumption of linearity is supported by experimental data provided in the “Results” section. The values of the constants can be directly obtained by linear least squares regression, but the results will be adversely affected by the presence of large outliers due to infrequent but large errors in the estimation of vertebral area and bone mineral content. Random sample consensus (RANSAC) is used instead to obtain a robust estimation of the linear transformation parameters. The RANSAC procedure randomly selects pairs of points to construct linear models, and the available data are fitted to the tentative model. Points lying far away are treated as outliers, and the model is considered a potential candidate only if there are fewer than a preset number of outliers. For a valid candidate, the inlier points are collectively used to generate a regression fit. This process is continued for several iterations to yield a number of potential candidate models, which are evaluated on the basis of the standard deviation of the inlier points from the regression fit. The model with the minimum standard deviation is adopted as the best-fitting model.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classification of Osteopenia from aBMD  CT

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Experiments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Subjects and imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Correlation between DXA and HU with volumetric information

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimation of aBMD  DxA  and aBMD  CT

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Impact of segmentation of cortical and trabecular bone

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation of aBMD  CT  osteopenia classifier

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison of aBMD  CT  and vBMD  CT  for aBMD  DxA  regression and osteopenia classification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Evidence of Correlation between aBMD  DxA  and HU

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Correlation Coefficients Using Different Slice Sampling Schemes


Top, Middle, and Bottom Slices, r  2  (r) Entire Volume, r  2  (r) Mean without RANSAC 0.286 (0.535) 0.478 (0.691) Mean with RANSAC 0.465 (0.682) 0.647 (0.804)

RANSAC, random sample consensus.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimating aBMD  DxA  from aBMD  CT

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

aBMDDXA=0.866×aBMDCT+0.194g/cm2.
aBMD

DXA

=

0.866

×

aBMD

CT

+

0.194

g

/

cm

2

.


![Figure 3, Bland-Altman plot of areal bone mineral density derived from dual-energy x-ray absorptiometry (aBMD DxA ) and from computed tomographic images (aBMD CT ). aBMD CT systematically underestimates aBMD DXA . SD, standard deviation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/OsteoporosisScreeningUsingArealBoneMineralDensityEstimationfromDiagnosticCTImages/2_1s20S1076633212003248.jpg)

![Figure 4, Regression plot of areal bone mineral density derived from dual-energy x-ray absorptiometry (aBMD DxA ) versus that derived from computed tomographic images (aBMD CT ). Four of 155 samples were rejected by random sample consensus.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/OsteoporosisScreeningUsingArealBoneMineralDensityEstimationfromDiagnosticCTImages/3_1s20S1076633212003248.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Impact of Different Bone Tissues on DXA Correlation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Correlation of aBMD  DxA  by Computing aBMD  CT  from Different Bone Tissues


Bone Tissue Used r  2  (r) Cortical bone 0.479 (0.692) Trabecular bone 0.655 (0.809) Both cortical and trabecular bone 0.726 (0.852)

aBMD  CT  , areal bone mineral density derived from computed tomographic images; aBMD  DxA  , areal bone mineral density derived from dual-energy x-ray absorptiometry.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Osteopenia Classification on the Basis of T Score

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Receiver-operating characteristic curve for a linear classifier using areal bone mineral density derived from computed tomographic images (aBMD CT ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/OsteoporosisScreeningUsingArealBoneMineralDensityEstimationfromDiagnosticCTImages/4_1s20S1076633212003248.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## vBMD and aBMD for Prediction and Classification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Comparison between Volumetric and Areal Bone Mineral Density


Method r  2  (r) RMSE (g/cm  2  ) AUC vBMD  CT  0.808 (0.653) 0.104 0.871 aBMD  CT  0.852 (0.726) 0.0884 0.894 Difference −5.16% (−10.1%) 17.6% −2.57%

aBMD  CT  , areal bone mineral density derived from computed tomographic images; AUC, area under the receiver-operating characteristic curve; RMSE, root mean square error; vBMD  CT  , volumetric bone mineral density derived from computed tomographic images.


The difference was obtained by subtracting the areal from the volumetric bone mineral density results.


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

## References

- 1\.  Consensus development conference: diagnosis, prophylaxis, and treatment of osteoporosis. Am J Med 1993; 94: pp. 646-650.


- 2\. NIH Consensus Development Panel on Osteoporosis Prevention, Diagnosis, and Therapy: Osteoporosis prevention, diagnosis, and therapy. JAMA 2001; 285: pp. 785-795.


- 3\. Revilla M., Cardenas J.L., Hernndez E.R., et. al.: Correlation of total-body bone mineral content determined by dual-energy x-ray absorptiometry with bone mineral density determined by peripheral quantitative computed tomography. Acad Radiol 1995; 2: pp. 1062-1066.


- 4\. Schreiber J., Anderson P., Humberto G., et. al.: Hounsfield units for assessing bone mineral density and strength: a tool for osteoporosis management. J Bone Joint Surg 2011; 93: pp. 1057-1063.


- 5\. Boden S., Goodenough D., Stockham C., et. al.: Precise measurement of vertebral bone density using computed tomography without the use of an external reference phantom. J Digit Imaging 1989; 2: pp. 31-38.


- 6\. Link T., Koppers B., Licht T., et. al.: In vitro and in vivo spiral CT to determine bone mineral density: initial experience in patients at risk for osteoporosis. Radiology 2004; 231: pp. 805-811.


- 7\. Teoh S., Chui C.: Bone material properties and fracture analysis: needle insertion for spinal surgery. J Mech Behav Biomed Mater 2008; 1: pp. 115-139.


- 8\. Rho J., Hobatho M., Ashman R.: Relations of mechanical properties to density and CT numbers in human bone. Med Eng Phys 1995; 17: pp. 347-355.


- 9\. Baum T., Carballido-Gamio J., Huber M., et. al.: Automated 3D trabecular bone structure analysis of the proximal femur—prediction of biomechanical strength by CT and DXA. Osteoporos Int 2010; 21: pp. 1553-1564.


- 10\. Bauer J., Henning T., Mueller D., et. al.: Volumetric quantitative CT of the spine and hip derived from contrast-enhanced MDCT: conversion factors. AJR Am J Roentgenol 2007; 188: pp. 1294-1301.


- 11\. Habashy A.H., Yan X., Brown J.K., et. al.: Estimation of bone mineral density in children from diagnostic CT images: a comparison of methods with and without an internal calibration standard. Bone 2011; 48: pp. 1087-1094.


- 12\. Pickhardt P., Lee L., del Rio A., et. al.: Simultaneous screening for osteoporosis at CT colonography: bone mineral density assessment using MDCT attenuation techniques compared against the DXA reference standard. J Bone Miner Res 2011; 26: pp. 2194-2203.


- 13\. Gudmundsdottir H., Jonsdottir B., Kristinsson S., et. al.: Vertebral bone density in Icelandic women using quantitative computed tomography without an external reference phantom. Osteoporos Int 1993; 3: pp. 84-89.


- 14\. Mueller D., Kutscherenko A., Bartel H., et. al.: Phantom-less QCT BMD system as screening tool for osteoporosis without additional radiation. Eur J Radiol 2010; 79: pp. 375-381.


- 15\. Hui S., Weir V., Brown K., et. al.: Assessing the clinical utility of quantitative computed tomography with a routinely used diagnostic computed tomography scanner in a cancer center. J Clin Densitom 2011; 14: pp. 41-46.


- 16\. Li W., Kornak J., Harris T., et. al.: Identify fracture-critical regions inside the proximal femur using statistical parametric mapping. Bone 2009; 44: pp. 596-602.


- 17\. Valentinitsch A., Patsch J., Mueller D., et. al.: Texture analysis in quantitative osteoporosis assessment: characterizing microarchitecture.Biomedical Imaging: From Nano to Macro: 2010 IEEE International Symposium.2010.IEEEPiscataway, NJ:pp. 1361-1364.


- 18\.  Tay W-L, Chui C-K, Ong S-H, et al. Detection of osteopenia from routine CT images. Presented at: 7th Asian Conference on Computer-Aided Surgery; Bangkok, Thailand; August 26–27, 2011.


- 19\. Lewiecki E., Watts N.: Assessing response to osteoporosis therapy. Osteoporos Int 2008; 19: pp. 1363-1368.


- 20\. Lotz J., Cheal E., Hayes W.: Fracture prediction for the proximal femur using finite element models: part I—linear analysis. J Biomech Eng 1991; 113: pp. 353.


- 21\. Marshall D., Johnell O., Wedel H.: Meta-analysis of how well measures of bone mineral density predict occurrence of osteoporotic fractures. BMJ 1996; 312: pp. 1254.


- 22\. World Health Organization: Assessment of Fracture Risk and Its Application to Screening for Postmenopausal Osteoporosis.1994.World Health OrganizationGeneva, Switzerland


- 23\. Boykov Y., Veksler O.: Graph cuts in vision and graphics: theories and applications.Handbook of Mathematical Models in Computer Vision.2006.Springer-VerlagBerlin, Germany:pp. 79-96.


- 24\. Li Y., Sun J., Tang C., et. al.: Lazy snapping. ACM Trans Graph 2004; 23: pp. 303-308.


- 25\. Reynolds D.: Gaussian mixture models.Li S.Z.Encyclopedia of Biometric Recognition.2008.Springer-VerlagNew York:


- 26\. Hounsfield G.: Computed medical imaging. Med Phys 1980; 7: pp. 283.


- 27\. Fischler M., Bolles R.: Random sample consensus: a paradigm for model fitting with applications to image analysis and automated cartography. Comm ACM 1981; 24: pp. 381-395.


- 28\. Zweig M., Campbell G.: Receiver-operating characteristic (ROC) plots: a fundamental evaluation tool in clinical medicine. Clin Chem 1993; 39: pp. 561-577.


- 29\. Faulkner K.G., Orwoll E.: Implications in the use of T-scores for the diagnosis of osteoporosis in men. J Clin Densitom 2002; 5: pp. 87-93.


- 30\. Zhang J., Yan C., Chui C., et. al.: Accurate measurement of bone mineral density using clinical CT imaging with single energy beam spectral intensity correction. IEEE Trans Med Imaging 2010; 29: pp. 1382-1389.


- 31\. Svendsen O., Hassager C., Skødt V., et. al.: Impact of soft tissue on in vivo accuracy of bone mineral measurements in the spine, hip, and forearm: a human cadaver study. J Bone Miner Res 1995; 10: pp. 868-873.


- 32\. Carrino J., Ohno-Machado L.: Development of radiology prediction models using feature analysis. Acad Radiol 2005; 12: pp. 415-421.