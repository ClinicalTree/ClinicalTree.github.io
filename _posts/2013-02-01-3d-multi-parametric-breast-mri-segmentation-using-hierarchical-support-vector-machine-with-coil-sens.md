---
title: 3D Multi-parametric Breast MRI Segmentation Using Hierarchical Support Vector Machine with Coil Sensitivity Correction
author: [CL_AT_YiWangMS,CL_AT_GlenMorrellMDPhD,CL_AT_MartaEHeibrunMDMS,CL_AT_AllisonPaynePhD,CL_AT_DennisLParkerPhD]
date: 2013-02-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 20, Issue 2]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The goal of the study is to develop a technique to achieve accurate volumetric breast tissue segmentation using magnetic resonance imaging (MRI) data. This segmentation can be useful to aid in the diagnosis of breast cancers and to assess breast cancer risk based on breast density. Tissue segmentation is also essential for development of acoustic and thermal models used in magnetic resonance guided high-intensity focused ultrasound treatment of breast lesions.

## Materials and Methods

In addition to commonly used T1-, T2-, and proton density–weighted images, three-point Dixon water- and fat-only images were also included as part of the multiparametric inputs to a tissue segmentation algorithm using a hierarchical support vector machine (SVM). The effectiveness of a variety of preprocessing schemes was evaluated through two in vivo datasets. The performance of the hierarchical SVM was investigated and compared to the conventional classification algorithms—conventional SVM and fuzzy C-mean (FCM).

## Results

The need for co-registration, zero-filled interpolation, coil sensitivity correction, and optimal SNR reconstruction before the final stage classification was demonstrated. The overlap ratios of the hierarchical SVM, conventional SVM and FCM were 93.25%–94.08%, 81.68–92.28%, and 75.96%–91.02%, respectively. Classification outputs from in vivo experiments showed that the presented methodology is consistent and outperforms other algorithms.

## Conclusion

The presented hierarchical SVM-based technique showed promising results in automatically segmenting breast tissues into fat, fibroglandular tissue, skin, and lesions. The results provide evidence that both the multiparametric breast MRI inputs and the preprocessing procedures contribute to the high accuracy of tissue classification.

## Introduction

Breast magnetic resonance imaging (MRI) has become a very useful imaging modality for breast cancer screening and diagnosis . It has been shown that 17%–34 % of cancer foci visible on breast MRI are not detected by mammography . Not only does breast MRI offer higher sensitivity for detection of breast cancer than x-ray mammography, ultrasound, clinical examination, or any combination of these, it also has a superior ability to delineate fatty and fibroglandular tissue .

Although lesions can be detected by visual inspection of breast MRI images, including dynamic contrast-enhanced (DCE) studies, there is evidence that quantitative measurements of different structures in the breast with and without contrast can assist not only in the detection of abnormal tissues, but also in the discrimination between fibroadenomas, cysts, and various types of malignancies . In an attempt to improve the performance of breast computer-aided diagnosis systems that are designed to supplement visual inspection and interpretation of breast MRI, methods for fully and semiautomatic segmentation of lesion mass based on DCE-MRIs have been developed . Efforts have also been made to discriminate between benign and malignant lesions using quantitative morphological and feature analyses . In addition to automatic lesion detection and discrimination, breast tissue segmentation could also be used to determine the percentage of fibroglandular tissue present in the breast, which is directly linked to breast parenchymal patterns , where the parenchymal pattern characterization parameters are taken as risk factors of developing breast cancer .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Subjects and Image Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Preprocessing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Co-registration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ZFI

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Three-point Dixon reconstruction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Skin extraction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Coil sensitivity estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Optimal SNR reconstruction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Iopt(r)=R(r)Ψ−1ST(r)S(r)Ψ−1ST(r)
I

o

p

t

(

r

)

=

R

(

r

)

Ψ

−

1

S

T

(

r

)

S

(

r

)

Ψ

−

1

S

T

(

r

)


where r denotes the position in the image space; R(r)=\[R1(r),R2(r),...,RL(r)\]
R

(

r

)

=

\[

R

1

(

r

)

,

R

2

(

r

)

,

...

,

R

L

(

r

)

\]
is the row vector of coil images; S(r)=\[S1(r),S2(r),...,SL(r)\]
S

(

r

)

=

\[

S

1

(

r

)

,

S

2

(

r

)

,

...

,

S

L

(

r

)

\]
is the row vector of coil sensitivities estimated from above step; and Ψ
Ψ
is an _L_ by _L_ matrix that describes the coupling and noise correlations between the coil elements. The noise matrix was assumed to be an identity matrix in the actual calculation for simplicity, and it was shown by Roemer et al that there was only a 10% SNR loss when assuming there is no noise correlation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Tissue Segmentation Using Hierarchical SVM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Schematic structure of hierarchical support vector machine (SVM) process with corresponding input feature and output segmented tissue type. PD-w, proton density weighted; T1w, T1-weighted; T2w, T2-weighted; TPD, three-point Dixon.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/0_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, (a) An example sagittal slice from the multiparametric input of a subject with confirmed fibroadenoma ( circled ). Contrasts displayed from left to right: T1, fat-suppressed T2, proton density (PD), three-point Dixon fat-only, and water-only images. (b) Region of interest–based image intensities from fatty tissue, fibroglandular tissue, skin, fibroadenoma, and background are plotted in a three-dimensional feature space composed of T1, T2, and PD contrast.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/1_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The central slice of T1-weighted images from dataset 1–4 is displayed in (a – d) , respectively. The axes units are in mm. The four datasets in this study represent a wide range of breast volumes, shapes, and densities.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/2_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Segmentation output (a) without and (b) with co-registration. Fatty tissue, fibroglandular tissue, skin, and fibroadenoma are presented in dark blue , light blue , yellow , and red , respectively. The misclassification appears on the border of the fibroglandular tissue island ( light blue ) and the surrounding fatty tissue ( dark blue ) drops considerably after co-registration, as pointed by the arrow .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/3_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Skin extraction using (a) three-point Dixon water-only image, (b) Canny filtering output, and (c) final skin pixels extracted from the water-only image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/4_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Coil sensitivity correction on an example proton density–weighted sagittal image of a healthy subject. (a) Original image, (b) estimated coil sensitivity, and (c) optimal signal-to-noise ratio reconstructed image with coil sensitivity correction.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/5_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Line plot of histograms of image intensity before and after coil sensitivity correction, based on the example from Figure 6. PD-w, proton density–weighted.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/6_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Lateral projection through the three-dimensional volumetric segmentation output of the hierarchical support vector machine algorithm for the subject with confirmed fibroadenoma. Fatty tissue, fibroglandular tissue, skin, and fibroadenoma are presented in blue , green , yellow , and red , respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/7_1s20S1076633212004783.jpg)

![Figure 9, Segmentation output of (a) hierarchical support vector machine (SVM), (b) conventional SVM, and (c) fuzzy c-mean from the subject with a confirmed fibroadenoma. Fatty tissue, fibroglandular tissue, skin, and fibroadenoma are presented in dark blue , light blue , green , and red , respectively. The corresponding multiparametric input was shown in Figure 2 .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/8_1s20S1076633212004783.jpg)

Table 1


Overlap Ratios of Various Algorithms with Radiologist's Manual Classification as Ground Truth


Overlap Ratio h-SVM (Sagittal), % h-SVM (Axial), % c-SVM, % FCM, % h-SVM without CSC, % h-SVM without ZFI, % h-SVM without Co-registration, % Dataset 1 90.94 90.47 86.97 75.96 82.09 90.69 88.81 Dataset 2 94.08 93.92 90.30 80.58 83.42 94.50 93.67 Dataset 3 93.90 93.90 81.68 91.02 95.45 94.41 95.38 Dataset 4 93.25 92.79 92.28 80.06 81.39 92.76 81.12

Hierarchical support vector machine (h-SVM) offers highest overlap ratio than the conventional SVM (c-SVM) and the FCM algorithm. Three preprocessing steps: coil sensitivity correction (CSC), zero-filled interpolation (ZFI), and co-registration are also evaluated.


![Figure 10, Bar diagram illustration of the overlap ratios from hierarchical support vector machine (SVM) along sagittal and axial directions, conventional SVM, and fuzzy c-mean algorithms for four datasets, according to Table 1 . The overlap ratios are calculated by comparing the performance of the methods to manual segmentation by radiologist. Consistently higher overlap ratios from the hierarchical SVM along both directions indicate the superior performance and stability of the hierarchical SVM than other algorithms.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DMultiparametricBreastMRISegmentationUsingHierarchicalSupportVectorMachinewithCoilSensitivityCorrection/9_1s20S1076633212004783.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2a


Individual Tissue Type Analysis of Dataset 1 Segmentation: Correctly Classified, Incorrectly Classified, and Overlap Ratios of Hierarchical SVM for Individual Tissue Type, Comparing to the Manual Classification from Radiologist 1


Hierarchical SVM Fat Fibroglandular Skin Lesion Air Overlap Ratio, % Radiologist Fat**3877** 165 45 4 116 92.16 Fibroglandular 222**467** 17 2 1 65.87 Skin 8 37**180** 2 91 56.60 Lesion 0 8 0**8** 0 50.00 Air 6 30 14 0**3401** 98.55

The bold face indicates the number of pixels that are correctly identified using radiologist as the ground truth for each tissue type.


Table 2b


Individual Tissue Type Analysis of Dataset 1 Segmentation: Correctly Classified, Incorrectly Classified, and Overlap Ratios of Hierarchical SVM for Individual Tissue Type, Comparing to the Manual Classification from Radiologist 2


Hierarchical SVM Fat Fibroglandular Skin Lesion Air Overlap Ratio (%) Radiologist Fat**3483** 122 22 0 112 93.15 Fibroglandular 445**467** 211 1 0 50.00 Skin 73 40**200** 2 15 46.51 Lesion 0 1 0**7** 0 87.50 Air 19 33 14 0**3378** 98.08

SVM, support vector machine.


The bold face indicates the number of pixels that are correctly identified using radiologist as the ground truth for each tissue type.


Table 3


Correctly Classified, Incorrectly Classified, and Overlap Ratios of Hierarchical SVM in Sagittal Orientation for Each Individual Tissue Type in Dataset 2


Hierarchical SVM Fat Fibroglandular Skin Air Overlap Ratio, % Radiologist Fat**3279** 180 33 45 92.71 Fibroglandular 142**632** 9 3 80.41 Skin 6 83**143** 56 49.65 Air 2 7 12**5443** 99.62

SVM, support vector machine.


The bold face indicates the number of pixels that are correctly identified using radiologist as the ground truth for each tissue type.


Table 4


Correctly Classified, Incorrectly Classified, and Overlap Ratios of Hierarchical SVM in Sagittal Orientation for Individual Tissue Type in Dataset 3


Hierarchical SVM Fat Fibroglandular Skin Air Overlap Ratio, % Radiologist Fat**3006** 40 0 28 97.79 Fibroglandular 115**379** 0 2 76.41 Skin 27 85**110** 39 42.15 Air 123 4 2**4046** 96.91

SVM, support vector machine.


The bold face indicates the number of pixels that are correctly identified using radiologist as the ground truth for each tissue type.


Table 5


Correctly Classified, Incorrectly Classified, and Overlap Ratios of Hierarchical SVM in Sagittal Orientation for Individual Tissue Type in Dataset 4


Hierarchical SVM Fat Fibroglandular Skin Air Overlap Ratio, % Radiologist Fat**1223** 52 12 180 83.37 Fibroglandular 26**1340** 1 57 94.10 Skin 9 78**145** 38 53.70 Air 3 22 29**4517** 98.82

SVM, support vector machine.


The bold face indicates the number of pixels that are correctly identified using radiologist as the ground truth for each tissue type.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 6


Overlap Ratios of Hierarchical SVM at Two Orientations (Sagittal and Axial) for Individual Tissue Type


Sagittal SVM Fat Fibroglandular Skin Lesion Air Total Points Overlap Ratio, % Axial SVM Fat**4,532,681** 156,116 3,926 967 19,280 4,712,970 96.17 Fibroglandular 50,442**1,027,900** 0 1,178 7,192 1,086,712 94.59 Skin 1,629 0**268,830** 252 1,330 272,041 98.82 Lesion 18 994 110**4,123** 18 5,263 78.34 Air 6,807 8,440 52 0**5,482,907** 5,498,206 99.72

SVM, support vector machine.


The bold face indicates the number of pixels that are correctly identified using radiologist as the ground truth for each tissue type.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Sinha S., Sinha U.: Recent advances in breast MRI and MRS. NMR Biomed 2009; 22: pp. 3-16.


- 2\. Weatherall P.T., Evans G.F., Metzger G.J., et. al.: MRI vs. histologic measurement of breast cancer following chemotherapy: comparison with x-ray mammography and palpation. J Magn Reson Imaging 2001; 13: pp. 868-875.


- 3\. Lee N.A., Rusinek H., Weinreb J., et. al.: Fatty and fibroglandular tissue volumes in the breasts of women 20–83 years old: comparison of X-ray mammography and computer-assisted MR imaging. AJR Am J Roentgenol 1997; 168: pp. 501-506.


- 4\. Bhooshan N., Giger M.L., Jansen S.A., et. al.: Cancerous breast lesions on dynamic contrast-enhanced MR images: computerized characterization for image-based prognostic markers. Radiology 2010; 254: pp. 680-690.


- 5\. Ertas G., Gulcur H.O., Osman O., et. al.: Breast MR segmentation and lesion detection with cellular neural networks and 3D template matching. Comput Biol Med 2008; 38: pp. 116-126.


- 6\. Ertas G., Gulcur H.O., Tunaci M.: Improved lesion detection in MR mammography: three-dimensional segmentation, moving voxel sampling, and normalized maximum intensity-time ratio entropy. Acad Radiol 2007; 14: pp. 151-161.


- 7\. Gilhuijs K.G., Giger M.L., Bick U.: Computerized analysis of breast lesions in three dimensions using dynamic magnetic-resonance imaging. Med Phys 1998; 25: pp. 1647-1654.


- 8\. Nie K., Chen J.H., Yu H.J., et. al.: Quantitative analysis of lesion morphology and texture features for diagnostic prediction in breast MRI. Acad Radiol 2008; 15: pp. 1513-1525.


- 9\. Nie K., Chen J.H., Chan S., et. al.: Development of a quantitative method for analysis of breast density based on three-dimensional breast MRI. Med Phys 2008; 35: pp. 5253-5262.


- 10\. Lin M., Chan S., Chen J.H., et. al.: A new bias field correction method combining N3 and FCM for improved segmentation of breast density on MRI. Med Phys 2011; 38: pp. 5-14.


- 11\. Kuroda K., Oshio K., Mulkern R.V., et. al.: Optimization of chemical shift selective suppression of fat. Magn Reson Med 1998; 40: pp. 505-510.


- 12\. Jacobs M.A., Barker P.B., Bluemke D.A., et. al.: Benign and malignant breast lesions: diagnosis with multiparametric MR imaging. Radiology 2003; 229: pp. 225-232.


- 13\.  Wang CM, Mai XX, Lin GC, et al. Classification for breast MRI using support vector machine. Proceedings of the 2008 IEEE 8th International Conference on Computer and Information Technology 2008:362–367.


- 14\. Heywang S.H., Bassermann R., Fenzl G., et. al.: MRI of the breast—histopathologic correlation. Eur J Radiol 1987; 7: pp. 175-182.


- 15\. Meyer C.R., Bland P.H., Pipe J.: Retrospective correction of intensity inhomogeneities in MRI. IEEE Trans Med Imaging 1995; 14: pp. 36-41.


- 16\. Guillemaud R., Brady M.: Estimating the bias field of MR images. IEEE Trans Med Imaging 1997; 16: pp. 238-251.


- 17\. Brey W.W., Narayana P.A.: Correction for intensity falloff in surface coil magnetic resonance imaging. Med Phys 1988; 15: pp. 241-245.


- 18\. McVeigh E.R., Bronskill M.J., Henkelman R.M.: Phase and sensitivity of receiver coils in magnetic resonance imaging. Med Phys 1986; 13: pp. 806-814.


- 19\. Bezdek J.C.: Pattern recognition with fuzzy objective function algorithms.1981.Plenum PressNew York


- 20\. Chen W., Giger M.L., Bick U.: A fuzzy c-means (FCM)-based approach for computerized segmentation of breast lesions in dynamic contrast-enhanced MR images. Acad Radiol 2006; 13: pp. 63-72.


- 21\. Barck K.H., Willis B., Ross J., et. al.: Viable tumor tissue detection in murine metastatic breast cancer by whole-body MRI and multispectral analysis. Magn Reson Med 2009; 62: pp. 1423-1430.


- 22\. Yang S.C., Wang C.M., Hsu H.H., et. al.: Contrast enhancement and tissues classification of breast MRI using Kalman filter-based linear mixing method. Comput Med Imaging Graph 2009; 33: pp. 187-196.


- 23\. Chung P.C., Wang C.M., Yang S.H., et. al.: Tissues classification for breast MRI contrast enhancement using spectral signature detection approach. IEEE International Conference on Systems, Man and Cybernetics 2006; 5: pp. 3917-3921.


- 24\. Du Y.P., Parker D.L., Davis W.L., et. al.: Reduction of partial-volume artifacts with zero-filled interpolation in three-dimensional MR angiography. J Magn Reson Imaging 1994; 4: pp. 733-741.


- 25\. Glover G.H., Schneider E.: Three-point Dixon technique for true water/fat decomposition with B0 inhomogeneity correction. Magn Reson Med 1991; 18: pp. 371-383.


- 26\. Bernstein M.A., King K.F., Zhou Z.J.: Handbook of MRI pulse sequences.2004.Academic PressBoston


- 27\. Moon-Ho Song S., Napel S., Pelc N.J., et. al.: Phase unwrapping of MR phase images using Poisson equation. IEEE Trans Image Process 1995; 4: pp. 667-676.


- 28\. Nie K., Chang D., Chen J.H., et. al.: Impact of skin removal on quantitative measurement of breast density using MRI. Med Phys 2010; 37: pp. 227-233.


- 29\. Canny J.: A computational approach to edge detection. IEEE Trans Pattern Anal Mach Intell 1986; 8: pp. 679-698.


- 30\. Vemuri P., Kholmovski E.G., Parker D.L., et. al.: Coil sensitivity estimation for optimal SNR reconstruction and intensity inhomogeneity correction in phased array MR imaging. Inf Process Med Imaging 2005; 19: pp. 603-614.


- 31\. Roemer P.B., Edelstein W.A., Hayes C.E., et. al.: The NMR phased array. Magn Reson Med 1990; 16: pp. 192-225.


- 32\. Cortes C., Vapnik V.: Support-vector networks. Machine Learning 1995; 20: pp. 273-297.


- 33\. Chang C.C., Lin C.J.: LIBSVM: a library for support vector machine. ACM Trans Intell Syst Technol 2011; 2: pp. 1-27.


- 34\. Casasent D., Wang Y.C.: A hierarchical classifier using new support vector machines for automatic target recognition. Neural Netw 2005; 18: pp. 541-548.