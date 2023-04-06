---
title: Computer-Aided Mass Detection Based on Ipsilateral Multiview Mammograms
author: [Wei Qian PhD,Dansheng Song MSc,Minshan Lei MSc,Ravi Sankar PhD,Edward Eikman MD]
date: 2007-05-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 5 SOURCE CL_S_AcademicRadiologyVolume14Issue5 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Recent reports on advances in computer-aided detection (CAD) indicate that current schemes miss early-stage breast cancers and result in a relatively large false-positive detection rate in order to achieve a high sensitivity rate for mass detection. This paper is inspired by the interpretation procedure from mammographers. The abnormal diagnosis can be derived from multiple views but is not available through single-view image analysis.

## Materials and Methods

A new multiview CAD system for early-stage breast cancer detection, which is based on modifying the optimized CAD algorithms from our prior single-view CAD system for constructing an adaptive ipsilateral multiview concurrent CAD system, is presented in this paper. The selection and design for the training and testing ipsilateral multiview mammogram databases are described here.

## Results

The performance evaluation of the developed ipsilateral multiview CAD system using free-response receiver operating characteristic analysis and computerized receiver operating characteristic experiments are presented. The results indicated that the proposed multiview CAD system is significantly superior to the single-view CAD systems based on statistically standard _P_ -values.

## Conclusion

This paper addresses a very important and timely project. It is related to two main problems regarding the development of breast cancer detection and diagnosis: early-stage detection and diagnosis of breast cancer with digital mammogram, and overall improvement of CAD system performance for clinical implementation. In order to improve the efficacy, accuracy, and efficiency of the current CAD scheme, an entirely new class of CAD method is required. This paper is unique in that a comprehensive and state-of-the-art approach is proposed for the CAD scheme of digital mammography. From the design aspect of the CAD scheme, the proposed ipsilateral multiview CAD method is innovative and quite different from current single-view CAD methods.

Breast cancer is the second leading cause of cancer death among women in the United States. The number of new cases of breast cancer is about 180,000 every year with an estimated number of 44,000 deaths annually. There is considerable evidence that early-stage diagnosis and treatment can significantly improve the survival rate of breast cancer patients. Mammography faces the difficulty of detecting very subtle signs in the extremely complex images ( ). Missed cancers will cause a delay in diagnosis and treatment and allow early-stage breast cancer develop to an advanced stage with severe implications for survival rates. False-positive (FP) screening mammograms will lead to unnecessary emotional stress in the patient, additional imaging studies with mammography, ultrasound, or MRI, and/or costly invasive procedures such as image-guided fine needle aspiration for cytologic evaluation, core biopsy, or needle localized breast biopsy.

The computer-aided diagnosis (CAD) on mammography (screen film and digital) has been a highly studied topic by a large number of research investigators, including our research team, over the past decade. The use of current CAD methods for mass detection, as applied to _retrospective_ case analysis, has been widely reported with a sensitivity of about 80–90% and an average FP detection rate of two to four per image ( ). CAD methods using retrospective case studies have proved to be useful for the reduction of the variability of reading mammograms when used as a second opinion strategy. For _prospective case analysis_ , the performance reported dropped significantly to less than 70% sensitivity with a similar FP detection rate ( ). But despite this performance reduction, it is proved to be useful for detection of missed interval cancers. In past years, despite considerable effort by many researchers on the study of CAD schemes, none of these efforts has been able to reach the acceptable levels of both detection sensitivity and FP rate for clinical requirements ( ). The main drawback of these CAD methods can be attributed to the single-view mammogram that lacks full analysis of breast image information. Therefore, a new, fully automatic and highly efficient multiview method was developed, and it is described in this paper.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## Design of Ipsilateral Multiview CAD System

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Flowchart of proposed ipsilateral multi-view CAD for mass detection.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedMassDetectionBasedonIpsilateralMultiviewMammograms/0_1s20S1076633207000207.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Preprocessing module

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Segmentation module

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Flow chart of Fuzzy C-means clustering algorithm.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedMassDetectionBasedonIpsilateralMultiviewMammograms/1_1s20S1076633207000207.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Feature Extraction and Concurrent Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Concurrent feature extraction and analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Schematic of spatial feature matching in multi-view images.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedMassDetectionBasedonIpsilateralMultiviewMammograms/2_1s20S1076633207000207.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Shape analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Mass margin analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Mass density analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Multiview concurrent feature selection using genetic algorithms

## Rationale

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## GA approach

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Multiview concurrent feature matching

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classification for mass detection using neural network

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Description of Datasets for the Study


Number of Normal Cases Number of Abnormal Cases Mass Size Description Testing databases Dataset 1 100 100 ≥1 mm and <5 mm BI-RADSTM 3, 4, 5 Dataset 2 100 100 ≥5 mm and <10 mm BI-RADSTM 3, 4, 5 Dataset 3 100 100 ≥10 mm and <20 mm BI-RADSTM 4, 5 Dataset 4 100 100 ≥20 mm BI-RADSTM 4, 5

American College of Radiology (ACR) Breast Imaging Reporting and Data System (BI-RADSTM), BI-RADSTM 3, 4, 5 are defined in ACR 1998.


Table 2


Results for Showing the Advantage of the Multiview CAD System Compared to Single-View CAD System


Methods Multiview CAD System Single-View CAD System Dataset 1 TP: 86% TP: 81% FP: 1.2/image FP: 1.5/image Dataset 2 TP: 90% TP: 85% FP: 1.0/image FP: 1.1/image Dataset 3 TP: 93% TP: 89% FP: 0.8/image FP: 1.0/image Dataset 4 TP: 95% TP: 90% FP: 0.5/image FP: 0.8/image

Datasets 1, 2, 3, and 4 are given in  Table 1  .


![Figure 4, Representative comparison between ipsilateral multiview CAD system and single-view CAD system. a and b are two views of ipsilateral raw mammograms, c and d are the detection results using single-view CAD method in different views, and e and f are the results using ipsilateral multi-view CAD method.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedMassDetectionBasedonIpsilateralMultiviewMammograms/3_1s20S1076633207000207.jpg)

![Figure 5, FROC curves showing the comparison of the detection performances for very tiny breast masses and MCCs. The results are based on the datasets 1, 2 in Table I , total 400 images, 200 normals and 200 abnormals with tiny masses and MCCs.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedMassDetectionBasedonIpsilateralMultiviewMammograms/4_1s20S1076633207000207.jpg)

![Figure 6, ROC curves showing the comparison of the detection performances for tiny breast masses and MCCs. The curves showing the advantage of multi-view CAD system compared to single-view CAD systems. The results are based on the datasets 1, 2 in Table I , total 400 images, 200 normals and 200 abnormals with tiny masses and MCCs.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedMassDetectionBasedonIpsilateralMultiviewMammograms/5_1s20S1076633207000207.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

P-value=2.15×102between a and b (P-value<.05, the difference is statistically significant)
P

 -value

=

2.15

×

10

2

between a and b (

P

 -value

<

.05

, the difference is statistically significant)


where a is multiview CAD system (Az = 0.91591) and b is single-view CAD system (Az = 0.85096).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Beam C.A., Layde P.M., Sullivan D.C.: Variability in the interpretation of screening mammograms by US radiologists: Findings from a national sample. Arch Intern Med 1996; 156: pp. 209-213.


- 2\. Petrick N., Chan H.P., Sahiner B., Wei D.: An adaptive density-weighted contrast enhancement filter for mammographic breast mass detection. IEEE Trans Med Imaging 1996; 15:


- 3\. Mendez A.J., Tahoces P.G., et. al.: Computer-aided diagnosis: Automatic detection of malignant masses in digitized mammograms. Med Physics 1998; 25: june


- 4\. Polakowski W.E., Cournoyer D.A., Rogers S.K., et. al.: Computer-aided breast cancer detection and diagnosis of masses using difference of Gaussians and derivative-based feature saliency. IEEE Trans Med Imaging 1997; 16:


- 5\. Giger M.L.: 1998.University Park Hotel at MITCambridge, MA


- 6\. Nishikawa R.M., Giger M.L., Schmidt R.A., et. al.: 1998.University of Nijmegenthe Netherlands June 7–0


- 7\. Sahiner B., Chan H.P., Wei D., Petrick N., Helvie M.A., Adler D.D., Goodsitt M.M.: Image feature selection by a genetic algorithm: Application to classification of mass and normal tissue. Med Physics 1996; 23: October


- 8\. Qian W., Clarke L.P., Li H.D., Kallergi M., Clark R.A., Silbiger M.L.: Digital mammography: m-channel quadrature mirror filters for microcalcification extraction. Comput Med Imaging Graphics 1994; 18: pp. 301-314.


- 9\. Qian W., Clarke L.P., Kallergi M., Clark R.A.: Tree-structured nonlinear filters in digital mammography. IEEE Trans Med Imaging 1994; 13: pp. 25-36.


- 10\. Qian W., Sun X., Song D., Clark R.A.: Digital mammography: Wavelet transform and kalman filtering neural network in mass segmentation and detection. Acad Radiol 2001; pp. 1074-1082. August


- 11\. Qian W., Clarke L.P., Li H.D., Kallergi M.: (abstract)1994. Proceedings of SNM 41st Annual Meeting, Orlando, Fla, June 5–8


- 12\. Qian W., Clarke L.P., Kallergi M., et. al.: 1994. Proceedings of ANNIE, November


- 13\. Qian W., Kallergi M., Clarke L.P., Li H.D., Clark R.A., Silbiger M.L.: Tree-structured nonlinear filter and wavelet transform for microcalcification segmentation in digital mammography. Med Phys 1995; pp. 1247-1254.


- 14\. Qian W., Clarke L.P., Kallergi M., Zheng B., Clark R.A.: Wavelet transform for computer assisted diagnosis (CAD) for digital mammography. IEEE Eng Med Biol 1995; 14: pp. 561-569.


- 15\. Qian W., Clarke L.P.: 1995. Presented at AAPM Annual Meeting, Boston, MA, August


- 16\. Qian W., Clarke L.P.: A restoration algorithm for P-32 and Y-90 remsstrahlung emission nuclear imaging: A wavelet-based neural network approach. Med Phys 1996; 23: pp. 1309-1323.


- 17\. Qian W., Clarke L.P.: Wavelet-based neural network with fuzzy-logic adaptivity for nuclear image restoration. Proc IEEE 1996; pp. 1458-1473. Special Issue


- 18\. Qian W., Clarke L.P., Kallergi M.: A restoration algorithm for P-32 and Y-90 bremsstrahlung emission nuclear imaging: A wavelet-neural network approach. Med Phys 1996; 23: pp. 1309-1323.


- 19\. Qian W., Land L., Clarke L.P.: Digital mammography: Wavelet based CAD method for mass detection. Proc SPIE Med Imaging 1997;


- 20\. Qian W., Lihua L., Clarke L.P.: Image feature extraction for mass detection using digital mammography: Influence of wavelet analysis. Med Phys 1999; 26: pp. 402-408.


- 21\. Qian W., Lihua L., Clarke L., Clark R.A.: Digital mammography: Comparison of adaptive and non-adaptive CAD methods for mass detection. Acad Radiol 1999; pp. 471-480.


- 22\. Qian W.: A novel hybrid filter architecture for image enhancement in medical imaging.Handbook of Medical Image Processing.2000.Academic PressNew York:


- 23\. Qian W., Sheybani E., Sankar R., et. al.: 2000. Presented at the International Workshop in Digital Mammography, June 11–14, Toronto, Canada


- 24\. Qian W., Sun X., Liu H., Clark R.: 2000. Presented at Wavelet Application in Signal and Image Processing VIII, SPIE International Symposium on Optical Science and Technology, July 30–August 4, San Diego, CA.


- 25\.  Qian W, Liu H, Li L, Clark R. A novel CAD method for mass detection in digital mammography. Presented at IEEE International Conference on Multimedia and Expo, July 30–August 2, New York.


- 26\. Qian W., Ravi S., Xiaoshan S., Xuejun S., Clark R.: Standardization for image characteristics in telemammography using genetic and nonlinear algorithms. Comput Biol Med 2005; 35: pp. 183-196.


- 27\. Luo P., Qian W., Romilly P.: CAD-aided mammogram training. Acad Radiol 2005; 12: pp. 1039-1048.


- 28\. Qian W., Zhukov T.A., Song M., Tockman M.S.: Computerized analysis of cellular features and biomarkers for cytologic diagnosis of early lung cancer. J Analyt Quant Cytol Histol 2006; 10: pp. 18-28.


- 29\. Albayrak S., Amasyali F.: 2003. Presented at the International XII, Turkish Symposium on Artificial Intelligence and Neural Networks, TAINN


- 30\. Chuang K.S., Tzeng H.L., Chen S., Wu J., Chen T.J.: Fuzzy C-means clustering with spatial information for image segmentation. Comput Med Imaging Graphics 1995; 30: pp. 9-15.


- 31\. Wu Y., Giger M.L., Doi K., Vyborny C.J., Schmidt R.A., Metz C.: Artificial neural networks in mammography: Application to decision making in diagnosis of breast cancer. Radiology 1993; 187: pp. 81-87.


- 32\. Brzakovic D., Luo M., Brzakovic P.: An approach to automated detection of tumors in mammograms. IEEE Trans Med Imaging 1990; 9: pp. 233-241.


- 33\. Burdett C.J., Longbotham H.D., Desai M., Richardson W.B., Stoll J.F.: Nonlinear indicator of malignancy. Proc SPIE 1993; 1905: pp. 853-860.


- 34\. Parr T., Astley S., Boggis C.: The detection of stellate lesions in digital mammograms.Gale A.G. et. al.Digital Mammography.1994.Elsevier Science BVLondon:


- 35\. Li L., Qian W., Clarke L.P.: X-ray medical image processing using directional wavelet transform. Proc IEEE Int Conf ASSP 1996; pp. 4.


- 36\. Claridge E., Richter J.H.: Characterization of mammographic lesions.Gale A.G. et. al.Digital Mammography.1994.Elsevier Science BVLondon:


- 37\. Kassemeijer N.: Recognition of stellate lesions in digital mammograms.Gale A.G. et. al.Digital Mammography.1994.Elsevier Science BVLondon:


- 38\. Kilday J., Palmieri F., Fox M.D.: Classifying mammographic lesions using computerized image analysis. IEEE Trans Med Imaging 1993; 12:


- 39\. Giger M.L., Lu P., Huo Z., et. al.: CAD in digital mammography: Computerized detection and classification of masses.Gale A.G. et. al.Digital Mammography.1994.Elsevier Science BVLondon:


- 40\. Giger M.L.: Computer-aided diagnosis, RSNA syllabus: A categorical course in physics.Haus A.G.Yaffe M.J.Technical Aspects of Breast Imaging.1993.pp. 283-298.


- 41\. Lo J.Y., Baker J.A., Kornguth P.J., Floyd C.E.: Computer-aided diagnosis of breast cancer: Artificial neural network approach for optimized merging of mammographic features. Acad Radiol 1995; 2: pp. 841-850.


- 42\. Velthuizen R.P., Hall L.O., Clarke L.P.: An initial investigation of feature extraction with genetic algorithms for fuzzy clustering. Biomed Eng J 1996; November


- 43\. Chan H.P., Lo S.C., Sahiner B., Lam K.L., Helvie M.A.: Computer-aided detection of mammographic microcalcifications: Pattern recognition with an artificial neural network. Med Phys 1995; 22: pp. 1555-1567.


- 44\. Dawan A.P., Chitre Y., Kaiser-Bonasso C., Moskowitz M.: Analysis of mammogaphic microcalcifications using gray-level image structure features. IEEE Trans Med Imaging 1996; 15:


- 45\. Li H.D., Kallergi M., Clarke L.P., Jain V.K., Clark R.A.: Markov random field for tumor detection in digital mammography. IEEE Trans Med Imaging 1995; 14: pp. 565-576.


- 46\. Sun X., Qian W., Song D., Clark R.A.: 2001. Presented at the IEEE Computer Society Conference on Computer Vision and Pattern Recognition, Kauai, Hawaii, December 9–14