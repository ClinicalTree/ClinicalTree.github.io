---
title: Automated Tissue Segmentation in Breast MRI
author: [Dania Daye MD PhD]
date: 2015-02-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 22, Issue 2 SOURCE CL_S_AcademicRadiologyVolume22Issue2 1}]
tags: [Journals,General Radiology]
---
Estimating a woman's risk of breast cancer is becoming increasingly important in clinical practice. As new strategies for breast cancer prevention and risk reduction become available , it is essential to provide accurate methods for longitudinally quantifying a woman's cancer risk in response to various preventative interventions. Current approaches to estimate breast cancer risk still face many limitations. For instance, the Gail model, National Cancer Institute's breast cancer risk assessment tool for the general population, has limited accuracy at the individual level . Over the last few decades, a number of studies suggested that it may be possible to improve risk prediction by supplementing information about risk with imaging features, namely breast density .

Breast density is a known independent risk factor of breast cancer . Breast density reflects the relative amount of fibroglandular tissue to adipose tissue in the breast. As breast density increases, so does a woman's risk of breast cancer. For instance, a woman with breast density >75% has four to five times the risk of developing breast cancer compared to a woman of the same age with low breast density . Similarly, longitudinal increases or decreases in breast density on imaging have been associated with changes in a woman's risk of developing breast cancer . Breast density changes serve as a surrogate biomarker for response to breast cancer preventive interventions, such as the use of aromatase inhibitors, increased physical activity, and weight loss . Accurately quantifying changes in breast density can thus have significant clinical implications by allowing clinicians to personalize treatment decisions and preventative interventions based on a woman's individual risk of breast cancer and perceived treatment response in a given period.

To date, most breast density quantification techniques have been developed for mammographic imaging. However, breast magnetic resonance (MR) imaging (MRI) is emerging as an important tool for breast cancer screening and risk assessment. Guidelines from the National Comprehensive Cancer Network and the American Cancer Society recommend regular breast MRIs for breast cancer surveillance in women at high risk of developing breast cancer . Despite the increasing use of MRI, few automated methods for breast tissue segmentation and density quantification are available. Breast tissue segmentation in MR images is an especially laborious and clinically impractical process. It often requires radiologists to trace the boundaries of the breast, adipose tissue, and parenchymal tissue on multiple slices in an image stack. Automated algorithms that accurately segment breast tissue are needed and hold significant clinical utility.

In the article by Rosado-Toro et al. in this issue of _Academic Radiology_ , the authors introduce k-means++ and dynamic programming (KDP), a novel automated segmentation algorithm that performs similarly to expert manual readers in isolating breast tissue from registered fat and water MR images, independent of the subject's breast density. Their algorithm, which implements k-means++ clustering and dynamic programming, takes advantage of contrast differences between different anatomic structures in the breast in MR fat and water images.

The KDP algorithm implements a three-step approach to segment the breast tissue. A k-means++ algorithm first clusters the pixels in the water images based on the signal intensity. Three clusters are defined as follows: 1) fibroglandular tissue (high signal intensity), 2) adipose tissue and pectoral muscle (intermediate signal intensity), and 3) background (low signal intensity). The pectoral muscle boundary is then delineated using dynamic programming by finding the minimum cost path through the fat images. Finally, the remaining chest tissue is removed using either the fixed sternum removal (FSR) approach or the morphologic sternum removal (MSR) approach. FSR removes a fixed 29-column region centered within the sternum, whereas MSR removes the tissue based on morphologic opening on the breast segmentation mask.

The authors compare the performance of the KDP algorithm to that of two recently described automated segmentation algorithms and three expert manual tracers using 266 MRI images from 14 female subjects. The recently described automated algorithms based on clustering and local gradient analysis (CLG) and Hessian-based sheetness filter (HSF) were adapted for segmenting breast tissue from MR fat and water images. The authors used the Dice metric and row-wise differences between the automated and manually traced pectoral muscle boundary to characterize the performance of the KDP algorithm. Statistical significance was assessed using the Welch two-sample _t_ test and the cumulative distribution function (cdf).

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Li J., Humphreys K., Eriksson L., et. al.: Mammographic density reduction is a prognostic marker of response to adjuvant tamoxifen therapy in postmenopausal patients with breast cancer. J Clin Oncol 2013; 31: pp. 2249-2256.


- 2\. Cuzick J., Warwick J., Pinney E., et. al.: Tamoxifen-induced reduction in mammographic density and breast cancer risk reduction: a nested case-control study. J Natl Cancer Inst 2011; 103: pp. 744-752.


- 3\. McTiernan A., Martin C.F., Peck J.D., et. al.: Estrogen-plus-progestin use and mammographic density in postmenopausal women: Women's Health Initiative randomized trial. J Natl Cancer Inst 2005; 97: pp. 1366-1376.


- 4\. Rockhill B., Spiegelman D., Byrne C., et. al.: Validation of the Gail et al. model of breast cancer risk prediction and implications for chemoprevention. J Natl Cancer Inst 2001; 93: pp. 358-366.


- 5\. Tice J.A., Cummings S.R., Smith-Bindman R., et. al.: Using clinical factors and mammographic breast density to estimate breast cancer risk: development and validation of a new predictive model. Ann Intern Med 2008; 148: pp. 337-347.


- 6\. Boyd N.F., Martin L.J., Yaffe M.J., et. al.: Mammographic density and breast cancer risk: current understanding and future prospects. Breast Cancer Res 2011; 13: pp. 223.


- 7\. McCormack V.A., dos Santos Silva I.: Breast density and parenchymal patterns as markers of breast cancer risk: a meta-analysis. Cancer Epidemiol Biomarkers Prev 2006; 15: pp. 1159-1169.


- 8\. Boyd N.F., Guo H., Martin L.J., et. al.: Mammographic density and the risk and detection of breast cancer. N Engl J Med 2007; 356: pp. 227-236.


- 9\. Warner E., Lockwood G., Tritchler D., et. al.: The risk of breast cancer associated with mammographic parenchymal patterns: a meta-analysis of the published literature to examine the effect of method of classification. Cancer Detect Prev 1992; 16: pp. 67-72.


- 10\. Kerlikowske K., Ichikawa L., Miglioretti D.L., et. al.: Longitudinal measurement of clinical mammographic breast density to improve estimation of breast cancer risk. J Natl Cancer Inst 2007; 99: pp. 386-395.


- 11\.  National Comprehensive Cancer Network (NCCN). NCCN Clinical practice guidelines in oncology. Available at:  http://www.nccn.org/professionals/physician\_gls/f\_guidelines.asp  . 2014.


- 12\. Saslow D., Boetes C., Burke W., et. al.: American Cancer Society guidelines for breast screening with MRI as an adjunct to mammography. CA Cancer Journal Clin 2007; 57: pp. 75-89.


- 13\. Rosado-Toro J., Barr T., Galons J.P., et. al.: Automated breast segmentation of fat and water MR images using dynamic programming. Acad Radiol 2015; 22: pp. 139-148.


- 14\. Giannini V., Vignati A., Morra L., et. al.: A fully automatic algorithm for segmentation of the breasts in DCE-MR images. Conf Proc IEEE Eng Med Biol Soc 2010; 2010: pp. 3146-3149.


- 15\. Wang L., Platel B., Ivanovskaya T., et. al.: Fully automatic breast segmentation in 3D breast MRI. Biomedical Imaging (ISBI), 2012 9th IEEE International Symposium 2012; pp. 1024-1027.