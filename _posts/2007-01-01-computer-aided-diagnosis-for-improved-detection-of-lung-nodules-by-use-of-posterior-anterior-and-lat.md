---
title: Computer-Aided Diagnosis for Improved Detection of Lung Nodules by Use of Posterior-Anterior and Lateral Chest Radiographs
author: [Junji Shiraishi PhD,Feng Li MD PhD,Kunio Doi PhD]
date: 2007-01-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 1 SOURCE CL_S_AcademicRadiologyVolume14Issue1 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We developed a computerized scheme for detection of lung nodules in the lateral views of chest radiographs, in order to improve the overall performance in combination with the computer-aided diagnostic (CAD) scheme for posterior-anterior (PA) views.

## Materials and Methods

We used 106 pairs of PA and lateral views of chest radiographs (122 lung nodules) for development of the CAD scheme. In the CAD scheme for lateral views, initial candidates of lung nodules were identified by use of a nodule enhancement filter based on the edge gradients. Thirty-four image features extracted from the original and the nodule-enhanced images were used for the rule-based scheme and for artificial neural networks (ANNs) for removal of some false-positive candidates. The computer performance was evaluated with a leave-one-case-out test method for ANNs. For PA views, we used the existing CAD scheme, which was trained with one-half of 924 chest images and then tested with the remaining images.

## Results

When the CAD scheme was applied only to PA views, the sensitivity in the detection of lung nodules was 70.5%, with 4.9 false positives per image. Although the performance of the computerized scheme for lateral views was relatively low (60.7% sensitivity with 1.7 false positives per image), the overall sensitivity (86.9%) was improved (6.6 false positives per two views), because 20 (16.4%) of the 122 nodules were detected only on lateral views.

## Conclusions

The CAD scheme by use of lateral-view images has the potential to improve the overall performance for detection of lung nodules on chest radiographs when combined with a conventional CAD scheme for standard PA views.

Lung cancer is the most common cause of cancer death in the United States ( ). Treatment for advanced lung cancer is unsatisfactory at present; however, treatment for early-stage lung cancer would be much more effective for improving the 5-year-survival rate ( ). Chest radiography and computed tomography (CT) have been used for the early detection of lung nodules. Currently, the effectiveness of lung cancer screening methods by use of chest radiography and CT is being examined in the National Lung Screening Trial (NLST) ( ). Despite differences in opinion about the effectiveness of screening by use of chest radiography ( ), chest radiography has been the most common radiologic examination in the world. Therefore, when chest radiographs are available, it would be useful to apply them for the early detection of lung nodules.

Computer-aided diagnosis (CAD) for the detection of lung nodules on chest images has been developed ( ) and has become available for clinical practice ( ). However, CAD methods used only posterior-anterior (PA) views of chest images, even if both PA and lateral views for the same patient were available. In fact, lateral views of chest images were commonly obtained together with PA views in many medical centers and clinical institutions. Even though different opinions have been expressed about the necessity of obtaining PA and lateral views in the past ( ), it is reasonable to use a lateral view in supporting the performance of a CAD scheme for the detection of lung nodules, and thus in assisting radiologists’ decision-making, if a lateral view together with a PA view has already been obtained.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


The number of lung nodules in each subtlety group and in each nodule size group for 121 and 118 lung nodules on PA and lateral views, respectively


Degree of subtlety Effective diameter of lung nodules \[mm\] 5–10 10–15 15–20 20–25 25–30 30–40 Total Extremely subtle PA 0 0 0 0 0 0 0 (0.0%) Lat 0 1 0 0 0 0 1 (0.8%) Very subtle PA 0 2 6 2 5 1 16 (13.2%) Lat 0 8 8 9 1 0 26 (22.0%) Subtle PA 2 14 12 12 7 6 53 (43.8%) Lat 1 6 13 12 7 2 41 (34.7%) Relatively obvious PA 0 6 9 9 8 4 36 (29.8%) Lat 1 0 5 14 16 7 43 (36.4%) Obvious PA 0 0 2 5 6 3 16 (13.2%) Lat 0 0 1 1 4 1 7 (5.9%) Total PA 2 (1.7%) 22 (18.2%) 29 (24.0%) 28 (23.1%) 26 (21.5%) 14 (11.6%) 121 Lat 2 (1.7%) 15 (12.7%) 27 (22.9%) 36 (30.5%) 28 (23.7%) 10 (8.5%) 118

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CAD Scheme for Detection of Lung Nodules on PA Views

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CAD Scheme for Detection of Lung Nodules on Lateral Views

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Overall computerized scheme for the detection of lung nodules on chest lateral views.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedDiagnosisforImprovedDetectionofLungNodulesbyUseofPosteriorAnteriorandLateralChestRadiographs/0_1s20S1076633206005599.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 1

## Segmentation of lung fields

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Example of density-adjusted chest lateral views without and with a contour of segmented lung field, a binary image of a roughly segmented chest region, and a histogram of pixel values on density-adjusted image of which the pixel value range between the upper 20% and 90% of the area under the histogram was used for segmenting the chest region.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedDiagnosisforImprovedDetectionofLungNodulesbyUseofPosteriorAnteriorandLateralChestRadiographs/1_1s20S1076633206005599.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Examples of chest lateral views with contours of automatically estimated segmented lung field.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedDiagnosisforImprovedDetectionofLungNodulesbyUseofPosteriorAnteriorandLateralChestRadiographs/2_1s20S1076633206005599.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 2

## Lung nodule detection and image feature extraction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Example of original chest lateral image including one lung nodule (arrow), and nodule-enhanced image obtained by use of the ARG filtering technique.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedDiagnosisforImprovedDetectionofLungNodulesbyUseofPosteriorAnteriorandLateralChestRadiographs/3_1s20S1076633206005599.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 3

## Rule-based test and ANNs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, FROC curves for the detection of 122 lung nodules (106 cases) obtained with CAD schemes for PA and lateral views and for the combination of two CAD schemes.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedDiagnosisforImprovedDetectionofLungNodulesbyUseofPosteriorAnteriorandLateralChestRadiographs/4_1s20S1076633206005599.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Number of identified lung nodules and sensitivities for 122 lung nodules, the number of false positives (FPs) per image for each of 106 PA and lateral views, and the number of FPs per case for 106 pairs


PA only PA and lateral Lateral only Overall No. of nodules correctly identified by CAD 32 54 20 106 Sensitivity 26.2% 44.3% 16.4% 86.9% No. of false positives 4.9/image 1.7/image 6.6/case

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Examples of PA and lateral views with a lung nodule, true location of lung nodules ( dashed circles ), and the computer output for lung nodule candidates ( arrowheads ) obtained with each CAD scheme for PA and lateral views. ( a ) A subtle lung nodule in the right middle lobe was identified correctly by both CAD schemes. One false-positive mark on the PA view cued a large vessel in the hilum and another false-positive mark in the center of the lateral view seemed to be paired. ( b ) A small and very subtle lung nodule located just above the right diaphragm was correctly identified by CAD on the PA view, but not on the lateral view, because the nodule was hidden by the overlap of the right and left diaphragm. ( c ) Relatively large, but very subtle lung nodules located in the right mediastinum region were not identified by CAD on PA views, but could be recognized by radiologists and were correctly identified by CAD on lateral views, with one false positive for each lateral view.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedDiagnosisforImprovedDetectionofLungNodulesbyUseofPosteriorAnteriorandLateralChestRadiographs/5_1s20S1076633206005599.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion and conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Jemal A., Murray T., Ward E., et. al.: Cancer statistics, 2005. CA Cancer J Clin 2005; 55: pp. 10-30.


- 2\. Ginsberg R.J., Rubinstein L.V., Lung Cancer Study Group: Randomized trial of lobectomy versus limited resection for T1 N0 non-small cell lung cancer. Ann Thorac Surg 1995; 60: pp. 615-622. discussion 622−613


- 3\.  National Lung Screening Trial. Available at  http://www.cancer.gov/nlst  . Accessed September 6, 2006.


- 4\. Fontana R.S., Sanderson D.R., Woolner L.B., et. al.: Screening for lung cancer. Cancer 1991; 67: pp. 1155-1164.


- 5\. Warner E.E., Mulshine J.L.: Lung cancer screening with spiral CT: Toward a working strategy. Oncology (Williston Park) 2004; 18: pp. 564-575. discussion 578, 583−564, 587


- 6\. Oken M.M., Marcus P.M., Hu P., et. al.: Baseline chest radiograph for lung cancer detection in the randomized Prostate, Lung, Colorectal and Ovarian Cancer Screening Trial. J Natl Cancer Inst 2005; 97: pp. 1832-1839.


- 7\. Byers T., Barrera E., Fontham E.T., et. al.: A midpoint assessment of the American Cancer Society challenge goal to halve the U.S. cancer mortality rates between the years 1990 and 2015. Cancer 2006; 107: pp. 396-405.


- 8\. Xu X.W., Doi K., Kobayashi T., MacMahon H., Giger M.L.: Development of an improved CAD scheme for automated detection of lung nodules in digital chest images. Med Phys 1997; 24: pp. 1395-1403.


- 9\. Shiraishi J., Li Q., Suzuki K., Engelmann R., Doi K.: Computer-aided diagnostic scheme for the detection of lung nodules on chest radiographs: Localized search method based on anatomical classification. Med Phys 2006; 33: pp. 2642-2653.


- 10\. Freedman M., Lo S., Osicka T., et. al.: Computer-aided detection of lung cancer on chest radiographs: Effect of machine CAD false-positive locations on radiologists’ behavior. Proc SPIE Med Imaging Image Proc 2002; 4684: pp. 1311-1319.


- 11\. Kakeda S., Moriya J., Sato H., et. al.: Improved detection of lung nodules on chest radiographs using a commercial computer-aided diagnosis system. AJR Am J Roentgenol 2004; 182: pp. 505-510.


- 12\. Sakai S., Soeda H., Takahashi N., et. al.: Computer-aided nodule detection on digital chest radiography: Validation test on consecutive T1 cases of resectable lung cancer. J Digit Imaging 2006; \[E-pub\]


- 13\. Austin J.H., Romney B.M., Goldsmith L.S.: Missed bronchogenic carcinoma: Radiographic findings in 27 patients with a potentially resectable lesion evident in retrospect. Radiology 1992; 182: pp. 115-122.


- 14\. Forrest J.V., Sagel S.S.: The lateral radiograph for early diagnosis of lung cancer. Radiology 1979; 131: pp. 309-310.


- 15\. Muhm J.R., Miller W.E., Fontana R.S., Sanderson D.R., Uhlenhopp M.A.: Lung cancer detected during a screening program using four-month chest radiographs. Radiology 1983; 148: pp. 609-615.


- 16\. Quekel L.G., Kessels A.G., Goei R., van Engelshoven J.M.: Miss rate of lung cancer on the chest radiograph in clinical practice. Chest 1999; 115: pp. 720-724.


- 17\. Stitik F.P., Tockman M.S.: Radiographic screening in the early detection of lung cancer. Radiol Clin North Am 1978; 16: pp. 347-366.


- 18\. Tala E.: Carcinoma of the lung. Acta Radiol Diagn (Stockh) 1967; 268: pp. 261.


- 19\. Katsuragawa S., Doi K., MacMahon H.: Image feature analysis and computer-aided diagnosis in digital radiography: Detection and characterization of interstitial lung disease in digital chest radiographs. Med Phys 1988; 15: pp. 311-319.


- 20\. Chakraborty D.P.: Maximum likelihood analysis of free-response receiver operating characteristic (FROC) data. Med Phys 1989; 16: pp. 561-568.


- 21\. Chan H.P., Sahiner B., Wagner R.F., Petrick N.: Classifier design for computer-aided diagnosis: effects of finite sample size on the mean performance of classical and neural network classifiers. Med Phys 1999; 26: pp. 2654-2668.


- 22\. Shiraishi J., Abe H., Engelmann R., Doi K.: Effect of the number of cases in image database on the performance of computer-aided diagnosis (CAD) for the detection of pulmonary nodules in chest radiographs. Proc SPIE Med Imaging Image Proc 2003; 5032: pp. 177-182.


- 23\. Armato S.G., Giger M.L., Ashizawa K., MacMahon H.: Automated lung segmentation in digital lateral chest radiographs. Med Phys 1998; 25: pp. 1507-1520.