---
title: Influence of Using Manual or Automatic Breast Density Information in a Mass Detection CAD System
author: [CL_AT_ArnauOliverPhD,CL_AT_XavierLladPhD,CL_AT_JordiFreixenetPhD,CL_AT_RobertMartPhD,CL_AT_ElsaPrezMD,CL_AT_JosepPontPhD,CL_AT_ReyerZwiggelaarProfessor]
date: 2010-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 17, Issue 7]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The goal of this article is to analyze and compare the performance of a developed mass computer-aided detection (CAD) system that takes breast density information into account when using manual or automatic breast density annotations in the training step. The advantages of considering this breast density information will be highlighted.

## Materials and Methods

The image database used in this article is 92 mediolateral oblique (MLO) and 92 craniocaudal (CC) mammograms obtained by a full-field digital mammographic unit. All mammograms contain at least one mass. The evaluation of the experiments is performed using free receiver operating characteristic analysis for evaluating the detection performance and pixel-based receiver operating characteristic analysis for evaluating the segmentation accuracy. In addition, the performance of the automatic breast density classifier is shown using confusion matrices.

## Results

When the breast density information is not considered and at a specificity of two false positives per image, the sensitivity obtained by the CAD system is 0.747 for the CC views and 0.853 for the MLO views. Considering the breast density information, the sensitivity for CC and MLO mammograms increases to 0.800 and 0.893, respectively, using manual classification, and 0.827 and 0.907, respectively, using automatic estimation. The same trend is observed when evaluating the CAD segmentation accuracy for detected masses in terms of area under the curve values: without considering breast density, these are 0.920 ± 0.057 and 0.917 ± 0.072; using manual classification, 0.934 ± 0.039 and 0.932 ± 0.046; and using automatic estimation, 0.947 ± 0.038 and 0.946 ± 0.045 for CC and MLO views, respectively.

## Conclusions

The experiments showed improved results when breast density information was taken into account. Moreover, the results obtained when using automatic breast density estimation outperformed those based on the manual annotations provided by expert radiologists. In this sense, the experiments showed that breast density information can be beneficial for CAD systems, and this information can be estimated robustly by an automatic procedure, which reduces the inter- and intra-class variability of the radiologists.

Between 1 in 8 and 1 in 12 women will develop breast cancer during their lifetime . There is no guaranteed way to prevent breast cancer at this time . Therefore, efforts are still focused on the detection of abnormalities at an early stage, because it has been shown to be correlated with improved survival rates . In this sense, the widespread adoption of mammography screening , as well as improvements made in breast cancer treatment, has resulted in decreases of breast cancer mortality among women of all ages .

However, it is also well-known that expert radiologists can miss a significant proportion of abnormalities . Typical reasons are that either the missed abnormality presents a distracting morphology, is located at the edge of glandular tissue, is obscured by overlying tissue, or is only seen in one view . In addition, a large number of mammographic abnormalities turn out to be benign after biopsy .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Summary of the Mammograms used in this Work, Detailing the BIRADS Distribution of the Mammograms and the Size of the Masses


Number BIRADS Number Size Mammograms BIRADS-I BIRADS-II BIRADS-III BIRADS-IV Masses Ultra-tiny Tiny Small Medium Large Extra-large Both views 80 40 16 18 6 98 46 24 7 8 8 5 Only CC 12 5 3 3 2 17 7 4 3 2 1 0 Only MLO 12 4 4 2 2 15 6 3 2 2 2 0

BIRADS, Breast Imaging Reporting and Data System; MLO, mediolateral oblique; CC, craniocaudal. Ultra-tiny, <1.0 cm  2  ; tiny, 1.0–2.0 cm  2  ; small, 2.0–3.0 cm  2  ; medium, 3.0– 4.0 cm  2  ; large, 4.0– 7.5 cm  2  ; extra-large ≥7.5 cm  2  .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, The top row shows four mammograms of increasing Breast Imaging Reporting and Data System category; the bottom row shows the same mammograms after the preprocessing step.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InfluenceofUsingManualorAutomaticBreastDensityInformationinaMassDetectionCADSystem/0_1s20S1076633210002345.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Eigendetection of Masses

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Layout of the computer-aided detection (CAD) system (top center flow diagram), depicting graphically the main steps with details in the specific boxes. The bottom right corner shows the results of the CAD system after breast density estimation and false-positive reduction. Note, however, that in the second mammogram, a false-positive appears. PCA, Principal Components Analysis; ROI, region of interest; 2D, two-dimensional.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InfluenceofUsingManualorAutomaticBreastDensityInformationinaMassDetectionCADSystem/1_1s20S1076633210002345.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Breast Density Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Manual Annotations versus Breast Density Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Density Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Confusion Matrix for Breast Density Estimation


Automatic Estimation CC (73.9%) MLO (83.7%) BIRADS-I BIRADS-II BIRADS-III BIRADS-IV BIRADS-I BIRADS-II BIRADS-III BIRADS-IV Manual Annotations BIRADS-I 36 4 3 2 42 0 2 0 BIRADS-II 6 11 2 0 5 12 2 1 BIRADS-III 2 1 15 2 0 2 17 1 BIRADS-IV 0 0 2 6 0 1 1 6

BIRADS, Breast Imaging Reporting and Data System; MLO, mediolateral oblique; CC, craniocaudal.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CAD System Performance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Comparison of the CAD System Performance (in Terms of _A  z_ ) when the Density Information is Not Used and when This Information is Used According to Manual Annotations and Automatic Breast Density Estimation


No Density Manual Annotations Automatic Estimation CC 0.77 ± 0.13 0.78 ± 0.15 0.79 ± 0.14 MLO 0.81 ± 0.12 0.82 ± 0.13 0.84 ± 0.13

CAD, computer-aided detection; MLO, mediolateral oblique; CC, craniocaudal.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


FROC Analysis of the CAD System when the Density Information is Not Used and When This Information is Used According to Manual Annotations and Automatic Breast Density Estimation


No Density Manual Annotations Automatic Estimation Sensitivity_A  z_ Sensitivity_A  z_ Sensitivity_A  z_ FPI = 0 CC 0.341 0.919 ± 0.065 0.400 0.937 ± 0.041 0.424 0.954 ± 0.037 MLO 0.341 0.924 ± 0.074 0.400 0.943 ± 0.040 0.400 0.951 ± 0.041 FPI = 1 CC 0.624 0.925 ± 0.053 0.659 0.935 ± 0.038 0.671 0.949 ± 0.065 MLO 0.682 0.921 ± 0.070 0.729 0.934 ± 0.046 0.765 0.947 ± 0.045 FPI = 2 CC 0.747 0.920 ± 0.057 0.800 0.934 ± 0.039 0.827 0.947 ± 0.038 MLO 0.853 0.917 ± 0.072 0.893 0.932 ± 0.046 0.907 0.946 ± 0.045

FROC, free receiver operating characteristic; CAD, computer-aided diagnosis; A _z_ , area under the curve; FPI, false positives per image.


The comparison details for different specificities and sensitivities the segmentation accuracy (in terms of _A  z_ ).


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

- 1\.  American Cancer Society. Breast cancer: facts and figures. Atlanta (GA): 2007-08, ACS.


- 2\.  Eurostat. Health statistics atlas on mortality in the European Union. Luxembourg: Office for Official Publications of the European Union 2002;


- 3\. Sener S.F., Winchester D.J., Winchester D.P., et. al.: Survival rates for breast cancers detected in a community service screening mammogram program. Am J Surg 2006; 191: pp. 406-409.


- 4\. Thurfjell E.L., Lernevall K.A., Taube A.A.S.: Benefit of independent double reading in a population-based mammography screening program. Radiology 1994; 191: pp. 241-244.


- 5\. Hendee W.R., Beam C., Hendrick E.: Proposition: all mammograms should be double-read. Med Phys 1999; 26: pp. 115-118.


- 6\. Sickles E.A.: Breast cancer screening outcomes in women ages 40-49: clinical experience with service screening using modern mammography. J Natl Cancer Inst Monogr 1997; 22: pp. 99-104.


- 7\. Bray F., McCarron P., Parkin D.M.: The changing global patterns of female breast cancer incidence and mortality. Breast Cancer Res 2004; 6: pp. 229-239.


- 8\. Bird R.E., Wallace T.W., Yankaskas B.C.: Analysis of cancers missed at screening mammography. Radiology 1992; 184: pp. 613-617.


- 9\. Birdwell R.L., Ikeda D.M., O'Shaughnessy K.D., et. al.: Mammographic characteristics of 115 missed cancers later detected with screening mammography and the potential utility of computer-aided detection. Radiology 2001; 219: pp. 192-202.


- 10\. Basset L.W., Gold R.H.: Breast cancer detection: mammograms and other methods in breast imaging.1987.Grune & StrattonNew York


- 11\. Hall F.M., Storella J.M., Siverstond D.Z., et. al.: Nonpalpable breast lesions: recommendations for biopsy based on suspicion of carcinoma at mammography. Radiology 1988; 167: pp. 353-358.


- 12\. Kuzmiak C.M., Millnamow G.A., Qaqish B., et. al.: Comparison of full-field digital mammography to screen-film mammography with respect to diagnostic accuracy of lesion characterization in breast tissue biopsy specimens. Acad Radiol 2002; 9: pp. 1378-1382.


- 13\.  R2 ImageChecker. Available online at:  http://www.r2tech.com  . Accessed June 6, 2009.


- 14\.  iCAD Second Look. Available online at:  http://www.icadmed.com  . Accessed June 6, 2009.


- 15\. Ho W.T., Lam P.W.T.: Clinical performance of computer-assisted detection (CAD) system in detecting carcinoma in breasts of different densities. Clin Radiol 2003; 58: pp. 133-136.


- 16\. Obenauer S., Sohns C., Werner C., et. al.: Impact of breast density on computer-aided detection in full-field digital mammography. J Digit Imaging 2006; 19: pp. 258-263.


- 17\. Brem R.F., Hoffmeister J.W., Rapelyea J.A., et. al.: Impact of breast density on computer-aided detection for breast cancer. Am J Roentgenol 2005; 184: pp. 439-444.


- 18\. Wolfe J.N.: Risk for breast cancer development determined by mammographic parenchymal pattern. Cancer 1976; 37: pp. 2486-2492.


- 19\. Boyd N.F., Byng J.W., Jong R.A., et. al.: Quantitative classification of mammographic densities and breast cancer risk: results from the Canadian national breast screening study. J Natl Cancer Inst 1995; 87: pp. 670-675.


- 20\. McCormack V.A., dos Santos Silva I.: Breast density and parenchymal patterns as markers of breast cancer risk: a meta-analysis. Cancer Epidem Biomarkers Prev 2006; 15: pp. 1159-1169.


- 21\. Freixenet J., Oliver A., Lladó X., et. al.: Eigendetection of masses considering false positive reduction and breast density information. Med Phys 2008; 35: pp. 1840-1853.


- 22\. Tourassi G.D., Harrawood B., Singh S., et. al.: Evaluation of information-theoretic similarity measures for content-based retrieval and detection of masses in mammograms. Med Phys 2007; 34: pp. 140-150.


- 23\. Varela C., Tahoces P.G., Méndez A.J., et. al.: Computerized detection of breast masses in digitized mammograms. Comp Biol Med 2007; 37: pp. 214-226.


- 24\. Lladó X., Oliver A., Freixenet J., et. al.: A textural approach for mass false positive reduction in mammography. Comp Med Imag Graph 2009; 33: pp. 415-422.


- 25\. Oliver A., Freixenet J., Martí R., et. al.: A novel breast tissue density classification methodology. IEEE Trans Inform Technol Biomed 2008; 12: pp. 55-65.


- 26\. Quinlan J.R.: Bagging, boosting, and C4.5. Nat Conf Artif Intell 1996; pp. 725-730.


- 27\. Metz C.E.: Evaluation of digital mammography by ROC analysis. Int Work Dig Mammogr 1996; pp. 61-68.


- 28\. Lai S.M., Li X., Bischof W.F.: On techniques for detecting circumscribed masses in mammograms. IEEE Trans Med Imag 1989; 8: pp. 377-386.


- 29\. Kegelmeyer W.P., Pruneda J.M., Bourland P.D., et. al.: Computer-aided mammographic screening for spiculated lesions. Radiology 1994; 191: pp. 331-337.


- 30\. Chakraborty D.P.: Validation and statistical power comparison of methods for analyzing free-response observer performance studies. Acad Radiol 2008; 15: pp. 1554-1566.


- 31\. Chakraborty D.P., Berbaum K.S.: Observer studies involving detection and localization: modeling, analysis, and validation. Med Phys 2004; 31: pp. 2313-2330.