---
title: Semi-Automatic Segmentation Software for Quantitative Clinical Brain Glioblastoma Evaluation
author: [CL_AT_YingZhuMS,CL_AT_GeoffreySYoungMD,CL_AT_ZhongXuePhD,CL_AT_RaymondYHuangMDPhD,CL_AT_HuiYouMD,CL_AT_KianSetayeshMS,CL_AT_HirotoHatabuMDPhD,CL_AT_FeiCaoPhD,CL_AT_StephenTWongPhD]
date: 2012-08-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 8]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Quantitative measurement provides essential information about disease progression and treatment response in patients with glioblastoma multiforme (GBM). The goal of this article is to present and validate a software pipeline for semi-automatic GBM segmentation, called AFINITI (Assisted Follow-up in NeuroImaging of Therapeutic Intervention), using clinical data from GBM patients.

## Materials and Methods

Our software adopts the current state-of-the-art tumor segmentation algorithms and combines them into one clinically usable pipeline. Both the advantages of the traditional voxel-based and the deformable shape-based segmentation are embedded into the software pipeline. The former provides an automatic tumor segmentation scheme based on T1- and T2-weighted magnetic resonance (MR) brain data, and the latter refines the segmentation results with minimal manual input.

## Results

Twenty-six clinical MR brain images of GBM patients were processed and compared with manual results. The results can be visualized using the embedded graphic user interface.

## Conclusion

Validation results using clinical GBM data showed high correlation between the AFINITI results and manual annotation. Compared to the voxel-wise segmentation, AFINITI yielded more accurate results in segmenting the enhanced GBM from multimodality MR imaging data. The proposed pipeline could be used as additional information to interpret MR brain images in neuroradiology.

## Introduction

Despite the best available standard therapies, including surgery, radiation, and chemotherapy, the survival in patients diagnosed with glioblastoma multiforme (GBM) remains dismal at 14 months . Newer therapeutic strategies aiming at targeting specific molecules are being developed and tested in clinical trials . Temozolomide chemoradiation has significantly prolonged survival but produces pseudoprogression that is difficult or impossible to distinguish from recurrence in 30%–50% of patients . In addition, antiangiogenic therapies have been used in combination with conventional chemotherapy in patients with recurrent GBM, demonstrating radiographic response rates of 35%–50% . These agents improve significantly patient quality of life but alter the pattern of recurrence by a potent effect on tumor permeability, suppressing enhancement within a solid tumor with a resulting increase in the frequency of infiltrative recurrence .

These therapy-induced alterations in the natural history and imaging appearance of treated GBM have made imaging follow-up by conventional magnetic resonance imaging (MRI) difficult, which motivates widespread ongoing research to discover additional imaging biomarkers and has led to a revision in response criteria. Although the most commonly used imaging criteria for evaluating treatment response are still based on measurement of enhancing tumor (the Macdonald Criteria) , the increase in infiltrative recurrence and the difficulty in distinguishing recurrence from progression has led to proposal of a new criteria for tumor response that includes abnormality on T2-weighted or fluid-attenuated inversion recovery images as additional markers for progression (the RANO criteria) . The RANO criteria also recommends the use of volumetric measurements of enhancing tumor because reliance on cross product diameters is problematic and highly operator dependent in cases of irregularly shaped tumor, multifocal tumor, or tumor with cystic or necrotic components. Recently, volumetric measures were found comparable or superior to linear diameter measures as indicators of tumor evaluation.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## Patients and Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The AFINITI Software Pipeline

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Brain tumor segmentation pipeline

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Brain tumor segmentation pipeline.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/0_1s20S1076633212001808.jpg)

![Figure 2, Registration-based skull stripping method. (a) Original image to be processed; (b) the template image; (c) the segmented brain region of the template image; (d) overlapping the brain region onto the original image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/1_1s20S1076633212001808.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Automatic segmentation step

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Some examples of tumor segmentation results after FAST. (a,c) Input images. (b,d) FAST segmentation results.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/2_1s20S1076633212001808.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Illustration of the combined T1 and T2 segmentation. (a) T2 image registered onto T1 image; (b) overlaying the segmentation result from T1 image onto T2 image; (c) thresholding T2 image ( blue shows the region of interest filtered out ); by adjusting the threshold, we can eliminate the enhanced big vessels close to the tumor; (d) after applying T2 thresholding, the majority of false-positive spots were removed; (e) other isolated spots are removed using morphological operations.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/3_1s20S1076633212001808.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Interactive processing step

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Representative segmentation results. Images (a,b) are original; (c,d) are the corresponding segmentation results.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/4_1s20S1076633212001808.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Detailed AFINITI Segmentation Results (mL)


AFINITI Results Manual Results Intersection Union Intersection/AFINITI (%) Intersection/Union (Jaccard Index; %) 6.57 7.26 6.16 7.67 93.7 80.2 20.63 27.60 16.47 31.76 79.8 51.9 28.95 41.32 24.38 45.88 84.2 53.1 2.52 4.27 2.49 4.30 98.6 57.8 53.91 81.80 51.81 83.91 96.1 61.8 22.84 28.03 22.72 28.14 99.5 80.7 10.35 19.65 10.26 19.74 99.1 52.0 21.54 20.79 17.00 25.33 78.9 67.1 4.63 13.96 4.30 14.29 92.8 30.1 6.49 21.09 6.45 21.13 99.4 30.2 1.22 2.27 1.18 2.32 96.5 51.1 3.73 6.62 3.71 6.64 99.5 55.9 40.71 58.44 40.67 58.49 99.9 69.5 8.19 17.13 7.71 17.61 94.2 43.8 35.61 45.60 34.22 46.99 96.1 72.8 15.24 19.99 14.79 20.44 97.1 72.4 12.49 14.74 12.08 15.15 96.8 79.8 7.59 20.48 7.54 20.53 99.3 36.7 1.36 2.34 1.31 2.39 96.6 54.9 10.14 16.04 8.10 18.08 79.9 44.8 17.98 43.75 15.90 45.83 88.4 34.7 64.66 90.07 64.16 90.56 99.2 70.8 1.42 3.13 1.40 3.15 98.5 44.5 39.76 51.85 35.93 55.68 90.4 64.5 9.24 25.32 6.86 27.70 74.3 24.8 14.90 44.10 13.91 45.09 93.3 30.8

AFINITI, Assisted Follow-up in NeuroImaging of Therapeutic Intervention.


![Figure 6, Correlation of the segmentation results.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/5_1s20S1076633212001808.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Difference between manual and semi-automatic segmentations: (a) original image; (b) manual segmentation; (c) semi-automatic segmentation; (d) difference between manual segmentation ( background white shape ) and semi-automatic segmentation ( highlighted red shape ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/6_1s20S1076633212001808.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Detailed Voxel-based Segmentation Results (mL)


FAST Results Manual Results Intersection Union Intersection/FAST (%) Intersection/Union (Jaccard Index; %) 6.60 7.26 6.16 7.69 93.4 80.1 61.03 27.60 17.04 71.58 27.9 23.8 80.03 41.32 27.39 93.96 34.2 29.2 2.52 4.27 2.49 4.30 98.6 57.8 73.75 81.80 54.34 101.21 73.7 53.7 23.16 28.03 23.03 28.16 99.4 81.8 10.91 19.65 10.72 19.83 98.3 54.1 27.81 20.79 17.20 31.39 61.9 54.8 10.19 13.96 5.70 18.45 55.9 30.9 7.01 21.09 6.54 21.57 93.2 30.3 1.26 2.27 1.21 2.32 96.1 52.0 3.73 6.62 3.71 6.64 99.5 55.9 40.93 58.44 40.86 58.51 99.8 69.8 10.75 17.13 8.19 19.70 76.2 41.6 37.40 45.60 35.71 47.29 95.5 75.5 17.59 19.99 15.50 22.08 88.1 70.2 12.55 14.74 12.14 15.15 96.7 80.1 7.59 20.48 7.54 20.53 99.3 36.7 1.38 2.34 1.33 2.39 96.7 55.8 15.32 16.04 9.03 22.34 58.9 40.4 18.34 43.75 16.11 45.99 87.8 35.0 65.10 90.07 64.51 90.65 99.1 71.2 1.48 3.13 1.46 3.15 98.4 46.2 85.36 51.85 40.13 97.08 47.0 41.3 0.01 25.32 0.00 25.33 0.0 0.0 9.48 44.10 9.42 44.15 99.4 21.3

AFINITI, Assisted Follow-up in NeuroImaging of Therapeutic Intervention.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Bland-Altman plots of the volume measures between Assisted Follow-up in NeuroImaging of Therapeutic Intervention (AFINITI) and manual results, and between FAST and manual results, respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiAutomaticSegmentationSoftwareforQuantitativeClinicalBrainGlioblastomaEvaluation/7_1s20S1076633212001808.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Stupp R., Mason W.P., van den Bent M.J., et. al.: Radiotherapy plus concomitant and adjuvant temozolomide for glioblastoma. N Engl J Med 2005; 352: pp. 987-996.


- 2\. Van Meir E.G., Hadjipanayis C.G., Norden A.D., et. al.: Exciting new advances in neuro-oncology: the avenue to a cure for malignant glioma. CA Cancer J Clin 2010; 60: pp. 166-193.


- 3\. Topkan E., Topuk S., Oymak E., et. al.: Pseudoprogression in patients with glioblastoma multiforme after concurrent radiotherapy and temozolomide. Am J Clin Oncol 2011 Mar 10; 60: \[Epub ahead of print\]


- 4\. Pope W.B., Lai A., Nghiemphu P., et. al.: MRI in patients with high-grade gliomas treated with bevacizumab and chemotherapy. Neurology 2006; 66: pp. 1258-1260.


- 5\. Vredenburgh J.J., Desjardins A., Herndon J.E., et. al.: Phase II trial of bevacizumab and irinotecan in recurrent malignant glioma. Clin Cancer Res 2007; 13: pp. 1253-1259.


- 6\. Vredenburgh J.J., Desjardins A., Herndon J.E., et. al.: Bevacizumab plus irinotecan in recurrent glioblastoma multiforme. J Clin Oncol 2007; 25: pp. 4722-4729.


- 7\. Norden A.D., Young G.S., Setayesh K., et. al.: Bevacizumab for recurrent malignant gliomas: efficacy, toxicity, and patterns of recurrence. Neurology 2008; 70: pp. 779-787.


- 8\. Macdonald D.R., Cascino T.L., Schold S.C., et. al.: Response criteria for phase II studies of supratentorial malignant glioma. J Clin Oncol 1990; 8: pp. 1277-1280.


- 9\. Wen P.Y., Macdonald D.R., Reardon D.A., et. al.: Updated response assessment criteria for high-grade gliomas: response assessment in neuro-oncology working group. J Clin Oncol 2010; 28: pp. 1963-1972.


- 10\. Galanis E., Buckner J.C., Maurer M.J., et. al.: Validation of neuroradiologic response assessment in gliomas: measurement by RECIST, two-dimensional, computer-assisted tumor area, and computer-assisted tumor volume methods. Neuro Oncol 2006; 8: pp. 156-165.


- 11\. Sorensen A.G., Patel S., Harmath C., et. al.: Comparison of diameter and perimeter methods for tumor volume calculation. J Clin Oncol 2001; 19: pp. 551-557.


- 12\. Gladwish A., Koh E., Hoisak J., et. al.: Evaluation of early imaging response criteria in glioblastoma multiform. Radiat Oncol 2011; 6: pp. 1-7.


- 13\. Ellingson B.M., Cloughesy T.F., Lai A., et. al.: Quantitative volumetric analysis of conventional MRI response in recurrent glioblastoma treated with bevacizumab. Neuro Oncol 2011; 13: pp. 401-409.


- 14\. Corso J.J., Sharon E., Dube S., et. al.: Efficient multilevel brain tumor segmentation with integrated bayesian model classification. IEEE Trans Med Imaging 2008; 27: pp. 629-640.


- 15\. Vaidyanathan M., Clarke L.P., Hall L.O., et. al.: Monitoring brain tumor response to therapy using MRI segmentation. Magn Res Imaging 1997; 15: pp. 323-334.


- 16\. Vaidyanathan M., Clarke L.P., Velthuizen R.P., et. al.: Comparison of supervised MRI segmentation methods for tumor volume determination during therapy. Magnet Res Imaging 1995; 13: pp. 719-728.


- 17\. Fletcher-Heath L.M., Hall L.O., Goldgof D.B., et. al.: Automatic segmentation of non-enhancing brain tumors in magnetic resonance images. Artificial Intell Med 2001; 21: pp. 43-63.


- 18\. Phillips W.E., Velthuizen R.P., Phuphanich S., et. al.: Application of fuzzy c-means segmentation technique for tissue differentiation in MR images of a hemorrhagic glioblastoma multiforme. Magn Res Imaging 1995; 13: pp. 277-290.


- 19\. Moonis G., Liu J., Udupa J.K., et. al.: Estimation of tumor volume with fuzzy-connectedness segmentation of MR images. AJNR Am J Neuroradiol 2002; 23: pp. 356-363.


- 20\. Emblem K.E., Nedregaard B., Hald J.K., et. al.: Automatic glioma characterization from dynamic susceptibility contrast imaging: brain tumor segmentation using knowledge-based fuzzy clustering. J Magn Res Imaging 2009; 30: pp. 1-10.


- 21\. Clark M.C., Hall L.O., Goldgof D.B., et. al.: Automatic tumor segmentation using knowledge-based techniques. IEEE Trans Med Imaging 1998; 17: pp. 187-201.


- 22\. Prastawa M., Bullitt E., Ho S., et. al.: A brain tumor segmentation framework based on outlier detection. Med Image Anal 2004; 8: pp. 275-283.


- 23\. Prastawa M., Bullitt E., Moon N., et. al.: Automatic brain tumor segmentation by subject specific modification of atlas priors. Acad Radiol 2003; 10: pp. 1341-1348.


- 24\. Kaus M.R., Warfield S.K., Nabavi A., et. al.: Automated segmentation of MR images of brain tumors. Radiology 2001; 218: pp. 586-591.


- 25\. Warfield S.K., Kaus M., Jolesz F.A., et. al.: Adaptive, template moderated, spatially varying statistical classification. Med Image Anal 2000; 4: pp. 43-55.


- 26\. Kass M., Witkin A., Terzopoulos D.: Snakes: active contour models. Int J Computer Vision 1988; pp. 321-331.


- 27\. Rivest-Henault D., Cheriet M.: Unsupervised MRI segmentation of brain tissues using a local linear model and level set. Mag Res Imaging 2011; 29: pp. 243-259.


- 28\. Wang L., Chen Y., Pan X., et. al.: Level set segmentation of brain magnetic resonance images based on local Gaussian distribution fitting energy. J Neurosci Methods 2010; 188: pp. 316-325.


- 29\. Chen Y., Zhang J., Macione J.: An improved level set method for brain MR images segmentation and bias correction. Comp Med Imaging Graph 2009; 33: pp. 510-519.


- 30\. Hu S., Collins D.L.: Joint level-set shape modeling and appearance modeling for brain structure segmentation. NeuroImage 2007; 36: pp. 672-683.


- 31\. Cheng L., Yang J., Fan X., et. al.: A generalized level set formulation of the Mumford-Shah functional for brain MR image segmentation. Inf Process Med Imaging 2005; 19: pp. 418-430.


- 32\. Vese L.A., Chan T.F.: A multiphase level set framework for image segmentation using the Mumford and Shah model. Int J Comp Vision 2002; 50: pp. 271-293.


- 33\. Cheng L.S., Fan X., Yang J., et. al.: A generalized level set formulation of the Mumford-Shah functional with shape prior for medical image segmentation. Proc Comp Vision Biomed Image Appl 2005; 3765: pp. 61-71.


- 34\. Dydenko I., Jamal F., Bernard O., et. al.: A level set framework with a shape and motion prior for segmentation and region tracking in echocardiography. Med Image Anal 2006; 10: pp. 162-177.


- 35\. Rousson M., Cremers D.: Efficient kernel density estimation of shape and intensity priors for level set segmentation. Med Image Comput Comput Assist Interv 2005; 8: pp. 757-764.


- 36\. Smith S.M., Jenkinson M., Woolrich M.W., et. al.: Advances in functional and structural MR image analysis and implementation as FSL. NeuroImage 2004; 23: pp. S208-S219.


- 37\. Woolrich M.W., Jbabdi S., Patenaude B., et. al.: Bayesian analysis of neuroimaging data in FSL. NeuroImage 2009; 45: pp. S173-S186.


- 38\. Yushkevich P.A., Piven J., Hazlett H.C., et. al.: User-guided 3D active contour segmentation of anatomical structures: significantly improved efficiency and reliability. NeuroImage 2006; 31: pp. 1116-1128.


- 39\. Zhang Y., Brady M., Smith S.: Segmentation of brain MR images through a hidden Markov random field model and the expectation-maximization algorithm. IEEE Trans Med Imaging 2001; 20: pp. 45-57.


- 40\. Xue X., Xue Z., Cao F., et. al.: PICE: prior information constrained evolution for 3-D and 4-D brain tumor segmentation. IEEE Int Symp Biomed Imaging 2010; pp. 840-843.