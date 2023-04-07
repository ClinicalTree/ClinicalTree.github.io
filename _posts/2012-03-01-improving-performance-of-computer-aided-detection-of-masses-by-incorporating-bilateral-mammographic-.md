---
title: Improving Performance of Computer-aided Detection of Masses by Incorporating Bilateral Mammographic Density Asymmetry An Assessment
author: [CL_AT_XingweiWangPhD,CL_AT_LihuaLiPhD,CL_AT_WeidongXuPhD,CL_AT_WeiLiuPhD,CL_AT_DrorLedermanPhD,CL_AT_BinZhengPhD]
date: 2012-03-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 3]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Bilateral mammographic density asymmetry is a promising indicator in assessing risk of having or developing breast cancer. This study aims to assess the performance improvement of a computer-aided detection (CAD) scheme in detecting masses by incorporating bilateral mammographic density asymmetrical information.

## Materials and Methods

A testing dataset containing 2400 full-field digital mammograms (FFDM) acquired from 600 examination cases was established. Among them, 300 were positive cases with verified cancer associated with malignant masses and 300 were negative cases. Two computerized schemes were applied to process images of each case. The first single-image based CAD scheme detected suspicious mass regions and the second scheme computed average and difference of mammographic tissue density depicted between the left and right breast. A fusion method based on rotation of the CAD scoring projection reference axis was then applied to combine CAD-generated mass detection scores and either the computed average or difference (asymmetry) of bilateral mammographic density scores. The CAD performance levels with and without incorporating mammographic density information were evaluated and compared using a free-response receiver operating characteristic type data analysis method.

## Results

CAD achieved a case-based mass detection sensitivity of 0.74 and a region-based sensitivity of 0.56 at a false-positive rate of 0.25 per image. By fusing the CAD and bilateral mammographic density asymmetry scores, the case-based and region-based sensitivity levels of the CAD scheme were increased to 0.84 and 0.69, respectively, at the same false-positive rate. Fusion with average mammographic density only slightly increased CAD sensitivity to 0.75 (case-based) and 0.57 (region-based).

## Conclusions

This study indicated that 1) bilateral mammographic density asymmetry was a stronger indicator of the case depicting suspicious masses than the average density computed from two breasts and 2) fusion between the conventional CAD scores and bilateral mammographic density asymmetry information could substantially increase CAD performance in mass detection.

Breast cancer is one of the leading cancers in women older than age 40 worldwide and scientific evidence has shown the breast cancer screening resulted in the early cancer detection and reduced patients’ mortality and morbidity rates . Although mammography is a most cost-effective and widely used imaging modality for breast cancer screening for the last several decades, interpreting mammograms to achieve high accuracy in terms of cancer detection and recall rates is a difficult and time-consuming task because of the large variability of breast abnormalities, overlapping dense fibroglandular tissue, and low cancer prevalence in the screening environment . As a result, a large number of computer-aided detection (CAD) schemes of mammograms have been developed to detect microcalcification clusters and masses in the last two decades and the commercialized CAD systems have also be routinely used to assist radiologists in interpreting mammograms in the clinical practice to date . Although there is no universal agreement of whether using current CAD systems as “a second reader” actually helped improve radiologists’ performance in the screening environment , improving CAD performance alone is important and has scientific merit . Current CAD schemes are able to detect microcalcification clusters with high sensitivity and low false-positive detection rates, which helps improve radiologists’ efficiency in interpreting mammograms and detect more cancers that are associated with microcalcifications . However, current CAD schemes have relatively lower performance in mass detection , which may reduce the overall performance level of radiologists as measured by the areas under receiver operating characteristic (ROC) curves . Previous studies have also found high correlation of mass detection results between radiologists and CAD schemes , which could substantially reduce the clinical utility of using CAD as “the second reader.” Hence, improving CAD sensitivity while maintaining or reducing the false-positive rates remains a challenge in developing CAD schemes of mammographic masses.

Because mammographic tissue density is one of the strongest known breast cancer risk indicator to date , several research groups have attempted to improve CAD performance in mass detection by taking mammographic density information into account in CAD decision-making . Because of considerable inter- and intraobserver variability, subjectively rating mammographic density using Breast Imaging Reporting and Data System (BIRADS) is often unreliable . Hence, a number of computerized schemes have been developed and tested to segment fibroglandular tissue and compute mammographic density. The results were proved to highly correlate to radiologists’ subjective assessment . As a result, one recent study reported that incorporating automatically computed mammographic density information into CAD schemes enabled CAD to achieve higher performance than incorporating CAD with manually (subjectively) assessed mammographic density . In our previous studies, we have pursued a new approach to extract and use mammographic density information. Based on the scientific evidence of that bilateral breast tissue pattern asymmetry is an important phenotype related to the abnormal biological processes that may increase the risk of developing breast cancer and our observation that radiologists routinely examined regional breast tissue density asymmetry depicted on bilateral mammograms of the left and right breast when identifying and/or classifying suspicious lesions, we demonstrated in our previous studies that computerized bilateral mammographic tissue density asymmetry was also an useful indicator in assessing the risk of developing breast cancer . Hence, in this study, we investigated the feasibility of improving CAD performance in mass detection by incorporating bilateral mammographic density asymmetry information, in particular enabling CAD scheme detecting more subtle masses without increasing false-positive rates. The details of our experimental procedures and results are presented in the following sections.

## Materials and methods

## Testing Image Dataset

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Distribution of breast density Breast Imaging Reporting and Data System ratings in the testing dataset.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/0_1s20S1076633211005137.jpg)

Table 1


Distribution of 314 Verified Malignant Masses in the Testing Dataset


Mass Type Not Specified Smoothed Irregular Spiculated Focal Asymmetry Mass Number 26 7 179 80 22 Percentage 8.3 2.2 57.0 25.5 7.0

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CAD Scheme of Mass Detection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, An example of applying our computer-aided detection scheme to both craniocaudal (CC) and mediolateral (MLO) view images of a testing case in which a true-positive mass is cued on both CC and MLO view images.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/1_1s20S1076633211005137.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Computing Mammographic Tissue Density and its Bilateral Asymmetry

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Fusion of CAD Scores and Mammographic Density Information

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Illustration of fusion between computer-aided detection (CAD) scores and bilateral mammographic density asymmetry scores by rotating the CAD scoring projection (reference) axis. In the figure, 300 true-positive mass regions (o) and 300 CAD-detected false-positive regions (Δ) are presented, which represent one region with the maximum CAD-generated detection score per case. For the cases without a detected suspicious region, a sign (Δ or o) is added in the position of CAD score = 0. The dashed line represents the original CAD scoring axis; the solid line represents the rotated new CAD scoring projection axis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/2_1s20S1076633211005137.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Comparison of two histograms of normalized average (a) and asymmetry (b) of bilateral mammographic density scores between 300 positive and 300 negative cases.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/3_1s20S1076633211005137.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, The trend of computer-aided detection (CAD) cueing sensitivity and minimum CAD cueing score (threshold) as the increase of CAD scoring projection (reference) axis rotation slopes when fusion of CAD scores and the bilateral mammographic density asymmetry scores. The false-positive rate is 0.25 per image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/4_1s20S1076633211005137.jpg)

![Figure 6, Comparison of two case-based free-response receiver operating characteristic curves representing the original computer-aided detection (CAD) performance (S = 0.0) and CAD performance after incorporating the bilateral mammographic density asymmetry information with a rotation slope of S = 0.6.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/5_1s20S1076633211005137.jpg)

![Figure 7, Comparison of two region-based FROC curves representing the original computer-aided detection (CAD) performance (S = 0.0) and CAD performance after incorporating the bilateral mammographic density asymmetry information with a rotation slope of S = 0.6.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/6_1s20S1076633211005137.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, The trend of computer-aided detection (CAD) cueing sensitivity and minimum CAD cueing score (threshold) as the increase of CAD scoring projection (reference) axis rotation slopes when fusion of CAD scores and the average mammographic density scores. The false-positive rate is 0.25 per image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovingPerformanceofComputeraidedDetectionofMassesbyIncorporatingBilateralMammographicDensityAsymmetryAnAssessment/7_1s20S1076633211005137.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Jemal A., Siegel R., Xu J., et. al.: Cancer statistics, 2010. CA Cancer J Clin 2010; 60: pp. 277-300.


- 2\. Smith R.A., Cokkindes V., Brooks D., et. al.: Cancer screening in the United States, 2011. CA Cancer J Clin 2011; 61: pp. 8-30.


- 3\. Birdwell R.L., Ikeda D.M., O’Shaughnessy K.D.: Mammographic characteristics of 115 missed cancers later detected with screening mammography and the potential utility of computer-aided detection. Radiology 2001; 219: pp. 192-202.


- 4\. Sickles E.A., Wolverton D.E., Dee K.E.: Performance parameters for screening and diagnostic mammography: specialist and general radiologists. Radiology 2002; 224: pp. 861-869.


- 5\. Nishikawa R.M.: Current status and future directions of computer-aided diagnosis in mammography. Comput Med Imaging Graph 2007; 31: pp. 224-235.


- 6\. Nishikawa R.M., Kallergi M.: Computer-aided detection, in its present form, is not an effective aid for screening mammography (Point/Counterpoint). Med Phys 2006; 33: pp. 811-814.


- 7\. Fenton J.J., Taplin S.H., Carney P.A., et. al.: Influence of computer-aided detection on performance of screening mammography. N Engl J Med 2007; 356: pp. 1399-1409.


- 8\. Karssemeijer N., Bluekens A.M., Beijerinck D., et. al.: Breast cancer screening results 5 years after introduction of digital mammography in a population-based screening program. Radiology 2009; 253: pp. 353-358.


- 9\. Zheng B., Ganott M.A., Britton C.A., et. al.: Soft-copy mammographic readings with different computer-assisted diagnosis cuing environments: preliminary findings. Radiology 2001; 221: pp. 633-640.


- 10\. Freer T.M., Ulissey M.J.: Screening mammography with computer-aided detection: prospective study of 12,860 patients in a community breast center. Radiology 2001; 220: pp. 781-786.


- 11\. Gur D., Stalder J.S., Hardesty L.A., et. al.: Computer-aided detection performance in mammographic examination of masses: assessment. Radiology 2004; 233: pp. 418-423.


- 12\. Zheng B., Wang X., Lederman D., et. al.: Computer-aided detection: the effect of training databases on detection of subtle breast masses. Acad Radiol 2010; 17: pp. 1401-1408.


- 13\. Boyd N., Martin I., Stone J., et. al.: Mammographic densities as a marker of human breast cancer risk and their use in chemoprevention. Curr Oncol Rep 2001; 3: pp. 314-321.


- 14\. Amir E., Freedman O.C., Seruga B., et. al.: Assessing women at high risk of breast cancer: a review of risk assessment models. J Natl Cancer Inst 2010; 102: pp. 680-691.


- 15\. Freixenet J., Oliver A., Marti R., et. al.: Eigendetection of masses considering false positive reduction and breast density information. Med Phys 2008; 35: pp. 1840-1853.


- 16\. Bueno G., Vallez N., Esteve P., et. al.: Automatic breast parenchymal density classification integrated into a CADe system. Int J Comput Assist Radiol Surg 2011; 6: pp. 309-318.


- 17\. Berg W.A., Campassi C., Langenberg P., et. al.: Breast imaging reporting and data system: inter- and intra-observer variability in feature analysis and final assessment. Am J Roentgenol 2000; 174: pp. 1769-1777.


- 18\. Taboces P.G., Correa J., Souto M., et. al.: Computer-assisted diagnosis: the classification of mammographic breast parenchymal patterns. Phys Med Biol 1995; 40: pp. 103-117.


- 19\. Zhou C., Chan H.P., Petrick N., et. al.: Computerized image analysis: estimation of breast density on mammograms. Med Phys 2001; 28: pp. 1056-1069.


- 20\. Chang Y.H., Wang X.H., Hardesty L.A., et. al.: Computerized assessment of tissue composition on digitized mammograms. Acad Radiol 2002; 9: pp. 898-905.


- 21\. Oliver A., Llado X., Freixenet J., et. al.: Influence of using manual or automatic breast density information in a mass detection CAD System. Acad Radiol 2010; 17: pp. 877-883.


- 22\. Scutt D., Lancaster G.A., Manning J.T.: Breast asymmetry and predisposition to breast cancer. Breast Cancer Res 2006; 8: pp. R14.


- 23\. Wang X., Lederman D., Tan J., et. al.: Computerized detection of breast tissue asymmetry depicted on bilateral mammograms: a preliminary study of breast risk stratification. Acad Radiol 2010; 17: pp. 1234-1241.


- 24\. Wang X., Lederman D., Tan J., et. al.: Computerized prediction of risk for developing breast cancer based on bilateral mammographic breast tissue asymmetry. Med Eng Phys 2011; 33: pp. 934-942.


- 25\.  Zheng B, Sumkin JH, Zuley M, et al. Computer-aided detection of breast masses depicted on full-field digital mammograms: a performance assessment. Br J Radiol. In press.


- 26\. Gur D., Stalder J., Hardesty L.A., et. al.: CAD performance on sequentially ascertained mammographic examinations of masses: an assessment. Radiology 2004; 233: pp. 418-423.


- 27\. Zheng B., Leader J.K., Abrams G.S., et. al.: Multiview-based computer-aided detection scheme for breast masses. Med Phys 2006; 33: pp. 3135-3143.


- 28\. Metz C.E., Herman B.A., Shen J.: Maximum likelihood estimation of receiver operating characteristic (ROC) curves from continuously distributed data. Stat Med 1998; 17: pp. 1033-1053.


- 29\. Zheng B., Shah R., Wallace L., et. al.: Computer-aided detection in mammography: an assessment of performance on current and prior images. Acad Radiol 2002; 9: pp. 1245-1250.


- 30\. Yoon H.J., Zheng B., Sahiner B., et. al.: Evaluating computer aided detection algorithms. Med Phys 2007; 34: pp. 2024-2038.


- 31\. Gail M.H., Mai P.L.: Comparing breast cancer risk assessment models. J Natl Cancer Inst 2010; 102: pp. 665-668.


- 32\. Yin F.F., Giger M.L., Doi K., et. al.: Computerized detection of masses in digital mammograms: analysis of bilateral subtraction images. Med Phys 1991; 18: pp. 955-963.


- 33\. Zheng B., Chang Y.H., Gur D.: Computerized detection of masses from digitized mammograms: comparison of single-image segmentation and bilateral-image subtraction. Acad Radiol 1995; 2: pp. 1056-1061.