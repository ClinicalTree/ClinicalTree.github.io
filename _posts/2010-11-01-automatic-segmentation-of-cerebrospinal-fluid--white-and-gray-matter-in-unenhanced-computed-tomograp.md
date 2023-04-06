---
title: Automatic Segmentation of Cerebrospinal Fluid, White and Gray Matter in Unenhanced Computed Tomography Images
author: [Varsha Gupta PhD,Wojciech Ambrosius MD PhD,Guoyu Qian MSc,Anna Blazejewska MSc,Radoslaw Kazmierski MD PhD DSc,Andrzej Urbanik MD PhD DSc,Wieslaw L. Nowinski PhD DSc]
date: 2010-11-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 17, Issue 11 SOURCE CL_S_AcademicRadiologyVolume17Issue11 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Although segmentation algorithms for cerebrospinal fluid (CSF), white matter (WM), and gray matter (GM) on unenhanced computed tomographic (CT) images exist, there is no complete research in this area. To take into account poor image contrast and intensity variability on CT scans, the aim of this study was to derive and validate a novel, automatic, adaptive, and robust algorithm.

## Materials and Methods

Unenhanced CT scans of normal subjects from two different centers were used. The algorithm developed uses adaptive thresholding, connectivity, and domain knowledge and is based on heuristics on the shape of CT histogram. The slope of the intensity histogram corresponding to the three-dimensional largest connected region in a variable CSF intensity range is tracked to determine the critical intensity, which serves as an initial classifier of CSF-WM. Thresholds of CSF, WM, and GM are then optimally derived to minimize classification overlap. Multiple, null, and erroneous classifications are resolved by applying domain knowledge.

## Results

The ground-truth regions with the minimal partial volume effect were used to evaluate segmentation results using the statistical markers. Average sensitivity, Dice index, and specificity, respectively, for the first center were 95.7%, 97.0%, and 98.6% for CSF; 96.1%, 97.3%, and 98.8% for WM; and 95.2%, 94.3%, and 92.8% for GM. The results were consistent for the second data center.

## Conclusions

The algorithm automatically identifies CSF, WM, and GM on unenhanced CT images with high accuracy, is robust to data from different scanners, does not require any parameter setting, and takes about 5 minutes in MATLAB to process a 512 × 512 × 30 scan. The algorithm has potential use in research and clinical applications.

Although segmentation algorithms for unenhanced computed tomographic (CT) images of the brain exist, there is still a need for an accurate and robust solution. Some of the associated reasons are low contrast between different tissues (cerebrospinal fluid \[CSF\], white matter \[WM\], and gray matter \[GM\]), diffuse tissue boundaries, artifacts due to the partial volume, inhomogeneity in images, and lack of validation due to difficulty in achieving the accurate ground truth (GT), among others . Intensity variations may further occur because of different scanner parameters combined with signal attenuations (due to different skull thickness) or beam hardening artifacts. Therefore, hard-coded threshold values for CT imaging of different tissues can lead to substantial errors in CT segmentation. Furthermore, pathologic conditions may also be responsible for the loss of GM and WM contrast on CT images (eg, in comatose patients after cardiac arrest ).

In the literature, only a few methods for CSF, WM, and GM segmentation of CT scans have been reported. The method of Lee et al is based on _k_ -means and expectation maximization clustering, which basically clusters the intensities into _k_ clusters. The intensity belongs to the cluster with the nearest mean. The performance of clustering algorithms, however, is sensitive to the choice of initial parameters . Also, the focus of Lee et al's study was only on CSF, skull, parenchyma, and calcification, not on the segmentation of WM and GM. Another approach by Hu and Xie is an automatic segmentation method based on a combination of pattern recognition, fuzzy theory, anatomy, fractal dimensions, and parameter thresholds. Although this algorithm was validated on 10 CT images (986 slices), there was no quantitative measure of the performance. The algorithm classifies CSF, WM, and GM but does not handle their diffuse boundaries. In general, a shape-based or texture-based analysis can perform well only when image quality is good. A genetic algorithm to locate the boundary of an organ in medical images was proposed by Heydarian et al . However, their method has limitations when an organ is composed of different tissue types (eg, the brain). Although genetic algorithms are a possible solution to medical image segmentation, there can be issues with parameter initialization, convergence criteria, and computation time . Segmentation methods based only on intensity thresholds, such as that of DeLeo et al , can have limitations due to the partial volume effect. Another fully automatic algorithm, by Ruttimann et al , focuses only on the segmentation of CSF regions.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Outline of algorithm for segmentation of cerebrospinal fluid (CSF), white matter (WM), and gray matter (GM).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/0_1s20S1076633210003107.jpg)

![Figure 2, Flowchart illustrating the details of each step of cerebrospinal fluid (CSF), white matter (WM), and gray matter (GM) segmentation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/1_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimation of the Initial Criterion of CSF-WM Classification: Critical Intensity

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

![Figure 3, Shape change of histogram by an increase in the upper range of intensity. A1 is the original slice in the range 0 to 70, and A2 is the corresponding histogram. B1, C1, D1, E1, and F1 are the largest connected components of image A1 after thresholding in the intensity range 0 to i , where i = 18, 22, 26, 30, and 34, and B2, C2, D2, E2, and F2 are the corresponding histograms. The significance of difference between the maximum height of histogram and the height of the end bin is highlighted. D2 has the maximum significance of difference.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/2_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimation of CSF Parameters

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Estimate of cerebrospinal fluid (CSF) parameters from the premaximum region of the histogram. Assuming that the CSF distribution is Gaussian, the bin with the maximum height, Mc , can be considered as the mean of CSF, CSFmean. The bin closest to the half of the maximum height is F . The standard deviation of CSF, CSFstd, is (Mc−F)/2log2−−−−−√ (Mc−F)/2log2 .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/3_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, A plot of significance, S _ i , and the mean cerebrospinal fluid (CSF) intensity derived from the CSF histogram maximum (as illustrated in Fig 4 ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/4_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## WM and GM parameters

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Fine-tuning of the white matter (WM) and gray matter (GM) parameters using Gaussian functions. I _c is the critical intensity, Mp is the position of maximum height of parenchyma histogram, and M _g = Mp + ( Mp − I _c) is the limit of intensity for which the initial GM parameters are estimated.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/5_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Intensity Thresholds

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Spatial errors

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, An illustration of multiple and unclassified voxels (left) resolved through voting (right). CSF, cerebrospinal fluid; GM, gray matter; WM, white matter.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/6_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Domain knowledge

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Correction of white matter (WM) identified as cerebrospinal fluid (CSF) or gray matter (GM) lying close to the brain-skull boundary (b) . If voxel intensity is greater than mean WM, then it is a GM voxel. If voxel intensity is less than or equal to mean WM, then it is a CSF voxel (c) . Original image is displayed in (a) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/7_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Overlap of GT Regions with Segmented Volume

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Illustration of results produced by the algorithm and the selection of different types of ground truth regions. A1, B1, C1, and D1 are the original unenhanced computed tomographic images, and A2, B2, C2, and D2 represent the corresponding segmented images with the ground truth regions overlaid. CSF, cerebrospinal fluid; GM, gray matter; WM, white matter.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/8_1s20S1076633210003107.jpg)

Table 1


Sensitivity, Dice Index , and Specificity of Ground Truth Comparison


Class Sensitivity (%) Dice Index (%) Specificity (%) Data from Poznań (70 data sets) CSF 95.7 97.0 98.6 WM 96.1 97.3 98.8 GM 95.2 94.3 92.8 Data from Kraków (14 data sets) CSF 95.2 96.1 98.5 WM 96.1 97.2 98.3 GM 95.9 94.7 93.3

CSF, cerebrospinal fluid; GM, gray matter; WM, white matter.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison of Mean Intensity of CSF, WM, and GM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Comparison of the mean intensity of cerebrospinal fluid (CSF), white matter (WM), and gray matter (GM) as calculated from the ground truth regions and estimated by the algorithm. The coefficients of determination for CSF, WM, and GM were 0.91, 0.84, and 0.89, respectively. The scans are from two different centers.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticSegmentationofCerebrospinalFluidWhiteandGrayMatterinUnenhancedComputedTomographyImages/9_1s20S1076633210003107.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Pham D.L., Xu C., Prince J.L.: Current methods in medical image segmentation. Annu Rev Biomed Eng 2000; 2: pp. 315-337.


- 2\. Torbey M.T., Selim M., Knorr J., et. al.: Quantitative analysis of the loss of distinction between gray and white matter in comatose patients after cardiac arrest. Stroke 2000; 31: pp. 2163-2167.


- 3\. Lee T.H., Fauzi M.F.A., Komiya R.: Segmentation of CT brain images using K-means and EM clustering. Proc Comput Graph Imaging Visualiz Modern Techn Appl 2008; pp. 339-344.


- 4\. Davenport J.W., Bezdek J.C., Hathaway R.J.: Parameters estimation for finite mixture distributions. Comput Math Appl 1988; 15: pp. 810-828.


- 5\. Hu Y., Xie M.: Automatic segmentation of brain CT image based on multiplicate features and decision tree. Proc Int Conf Commun Circuit Syst 2007; pp. 837-840.


- 6\. Heydarian M., Noseworthy M.D., Kamath M.V., et. al.: Optimizing the level set algorithm for detecting object edges in MR and CT images. IEEE Trans Nucl Sci 2009; 56: pp. 156-166.


- 7\. Maulik U.: Medical image segmentation using genetic algorithms. IEEE Trans Inform Technol Biomed 2009; 13: pp. 166-173.


- 8\. DeLeo J.M., Schwarz M., Creasy H., et. al.: Computer assisted categorization of brain computerized tomography pixels into cerebrospinal fluid, white matter and gray matter. Comput Biomed Res 1985; 18: pp. 79-88.


- 9\. Ruttimann U.E., Joyce E.M., Rio D.E., et. al.: Fully automated segmentation of cerebrospinal fluid in computed tomography. Psychiatry Res Neuroimaging 1993; 50: pp. 101-119.


- 10\. Klauschen F., Goldman A., Barra V., et. al.: Evaluation of automated brain MR image segmentation and volumetry methods. Hum Brain Mapping 2009; 30: pp. 1310-1327.


- 11\. Hacker H., Artmann H.: The calculation of CSF spaces in CT. Neuroradiology 1978; 16: pp. 190-192.


- 12\. Zimmerman R.A., Gibby W.A., Raymond F.: Neuroimaging: Clinical and Physical Principles.1999.SpringerNew York


- 13\. Mandel J.: The Statistical Analysis of Experimental Data.1984.Courier Dover PublicationsNew York


- 14\. Bevington P.R.: Data Reduction and Error Analysis for the Physical Sciences.1969.McGraw-HillNew York


- 15\. Zou K.H., Warfield S.K., Bharatha A., et. al.: Statistical validation of image segmentation quality based on spatial overlap index. Acad Radiol 2004; 11: pp. 178-189.


- 16\. Nowinski W.L., Qian G., Bhanu Prakash K.N., et. al.: Stroke suite: CAD systems for acute ischemic stroke, hemorrhagic stroke, and stroke in ER. Med Imaging Informat Lect Notes Comput Sci 2008; 4987: pp. 377-386.