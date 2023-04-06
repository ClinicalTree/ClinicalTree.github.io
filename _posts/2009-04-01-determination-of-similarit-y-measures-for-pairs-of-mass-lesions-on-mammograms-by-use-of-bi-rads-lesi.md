---
title: Determination of Similarit y Measures for Pairs of Mass Lesions on Mammograms by Use of BI-RADS Lesion Descriptors and Image Features
author: [Chisako Muramatsu PhD,Qiang Li PhD,Robert A. Schmidt MD,Junji Shiraishi PhD,Kunio Doi PhD]
date: 2009-04-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 16, Issue 4 SOURCE CL_S_AcademicRadiologyVolume16Issue4 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

To determine similarity measures for selection of pathology-known similar images that would be useful for radiologists as a reference guide in the diagnosis of new breast lesions on mammograms.

## Materials and Methods

The images were obtained from the Digital Database for Screening Mammography developed by the University of South Florida. For determination and evaluation of similarity measures, the “gold standard” of similarities for 300 pairs of masses was determined by 10 breast radiologists. For determining similarity measures that would agree with radiologists' similarity determination, an artificial neural network (ANN) was trained with the radiologists' subjective similarity ratings and the image features. The image features were determined subjectively using the Breast Imaging Reporting and Data System (BI-RADS) lesion descriptors and objectively by computerized image analysis. The similarity measures determined by the ANN were compared to the gold standard and evaluated in terms of the correlation coefficient.

## Results

The similarity measures determined using the BI-RADS descriptors only were not as useful as those determined by use of the image features only. When the BI-RADS margin ratings were combined with the image features, the correlation coefficient between the subjective ratings and the objective measures improved slightly ( _r_ = 0.76) compared to those based on the image features alone ( _r_ = 0.74).

## Conclusions

The inclusion of the BI-RADS margin descriptors may be useful for determination of similarity measures, especially when it is difficult to obtain the manual outlines of the masses and if the BI-RADS descriptors were provided consistently by radiologists.

Breast cancer is the most frequently diagnosed cancer in women in the United States . To achieve a decrease in the cancer mortality rate, early detection of cancer lesions is important. Mammography is considered a useful screening method for early detection in the general population. However, it can be difficult to diagnose breast cancer on mammograms; sometimes cancers might be missed, and usually many patients with benign lesions are sent for biopsy . Computer-aided diagnosis, in which radiologists make a diagnosis by taking into consideration the outputs from the computer analysis of medical images, has been demonstrated to improve radiologists' diagnostic accuracy in the classification of breast lesions . With such a computer-aided diagnosis, the likelihood of malignancy of the lesion is presented to radiologists.

It has been suggested that the presentation of images similar to that of a new unknown lesion would be helpful for distinction between benign and malignant lesions because radiologists learn their diagnostic skills by observing many cases in clinical practice, review courses, and textbooks . Studies have shown the potential usefulness of similar images for classification of breast masses and lung diseases . For similar images to be useful, we believe that images must be similar from the point of view of the diagnosing radiologists. However, in most previous studies, the similar images were selected based only on objective image features and, to our knowledge, there were only a few studies in which computed similarities were evaluated based on the radiologists' subjective similarities. Moreover, the number of studies on investigation of subjective similarity for image pairs by radiologists is limited . In this study, subjective similarity ratings for pairs of masses were determined by breast radiologists, and the average similarity ratings were employed as the “gold standard” for determination and evaluation of objective similarity measures. By training an artificial neural network (ANN) with radiologists' subjective similarity ratings as teacher and the image features as input data, it may be possible to determine similarity measures that would agree with radiologists' similarity ratings for unknown pairs.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Image Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Distributions of the fractions of masses in each of the Breast Imaging Reporting and Data System (BI-RADS) (a) shape categories and (b) margin categories for 1568 masses in the database and 350 masses used in the 300 pairs.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeterminationofSimilarityMeasuresforPairsofMassLesionsonMammogramsbyUseofBIRADSLesionDescriptorsandImageFeatures/0_1s20S107663320800634X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Subjective Similarity Ratings by Breast Radiologists

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Objective Similarity Measures

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Relationship between the subjective similarity ratings and the objective similarity measure using the six image features and the Breast Imaging Reporting and Data System (BI-RADS) margin ratings.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeterminationofSimilarityMeasuresforPairsofMassLesionsonMammogramsbyUseofBIRADSLesionDescriptorsandImageFeatures/1_1s20S107663320800634X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Relationship between the difference in the Breast Imaging Reporting and Data System (BI-RADS) margin ratings for the pairs and the output of the artificial neural network (ANN) trained with the BI-RADS margin ratings.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeterminationofSimilarityMeasuresforPairsofMassLesionsonMammogramsbyUseofBIRADSLesionDescriptorsandImageFeatures/2_1s20S107663320800634X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Three pairs of masses (a-c) for which the inclusion of the Breast Imaging Reporting and Data System (BI-RADS) margin ratings was useful and three pairs of masses (d-f) for which the inclusion of the BI-RADS margin ratings was not useful in addition to the computed image features. The BI-RADS descriptors given for left and right masses are, respectively: (a) microlobulated and microlobulated, (b) spiculated and spiculated, (c) obscured and ill-defined, (d) ill-defined and spiculated, (e) obscured and spiculated, and (f) ill-defined and obscured.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeterminationofSimilarityMeasuresforPairsofMassLesionsonMammogramsbyUseofBIRADSLesionDescriptorsandImageFeatures/3_1s20S107663320800634X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\.  American Cancer Society. Cancer facts and figures 2008. Available at:  http://www.cancer.org/docroot/STT/content/STT\_1x\_Cancer\_Facts\_and\_Figures\_2008.asp?from=fast  . Accessed August 6, 2008.


- 2\. Hall F.M., Storella J.M., Silverstone D.Z., et. al.: Nonpalpable breast lesions: recommendations for biopsy based on suspicion of carcinoma at mammography. Radiology 1988; 167: pp. 353-358.


- 3\. Kopans D.B., Moore R.H., McCarthy K.A., et. al.: Positive predictive value of breast biopsy performed as a result of mammography: there is no abrupt change at age 50 years. Radiology 1996; 200: pp. 357-360.


- 4\. Sickles E.A., Miglioretti D.L., Ballard-Barbash R., et. al.: Performance benchmarks for diagnostic mammography. Radiology 2005; 235: pp. 775-790.


- 5\. Chan H.P., Sahiner B., Roubidoux M.A., et. al.: Improvement of radiologists' characterization of mammographic masses by using computer-aided diagnosis: an ROC study. Radiology 1999; 212: pp. 817-827.


- 6\. Huo Z., Giger M.L., Vyborny C.J., et. al.: Breast cancer: effectiveness of computer-aided diagnosis-observer study with independent database of mammograms. Radiology 2002; 224: pp. 560-568.


- 7\. Jiang Y., Nishikawa R.M., Schmidt R.A., et. al.: Improving breast cancer diagnosis with computer-aided diagnosis. Acad Radiol 1999; 6: pp. 22-33.


- 8\. Doi K.: Current status and future potential of computer-aided diagnosis in medical imaging. Br J Radiol 2005; 78: pp. S3-S19.


- 9\. Doi K.: Computer-aided diagnosis in medical imaging: historical review, current status and future potential. Comput Med Imaging Graph 2007; 31: pp. 198-211.


- 10\. Muramatsu C.: Investigation of similarity measures for selection of similar images in computer-aided diagnosis of breast lesions on mammograms. PhD dissertation, The University of Chicago, Chicago, IL. Ann Arbor, MI: ProQuest/UMI 2008;


- 11\. Horsch K., Giger M.L., Vyborny C.J., et. al.: Classification of breast lesions with multimodality computer-aided diagnosis: observer study results on an independent clinical data set. Radiology 2006; 240: pp. 357-368.


- 12\. Li Q., Li F., Shiraishi J., et. al.: Investigation of new psychophysical measures for evaluation of similar images on thoracic CT for distinction between benign and malignant nodules. Med Phys 2003; 30: pp. 2584-2593.


- 13\. Qi H., Snyder W.E.: Content-based image retrieval in picture archiving and communications systems. J Digit Imaging 1998; 11: pp. 65-73.


- 14\. Sklansky J., Tao E.Y., Bazargan M., et. al.: Computer-aided case-based diagnosis of mammographic regions of interest containing microcalcifications. Acad Radiol 2000; 7: pp. 395-405.


- 15\. Giger M.L., Huo Z., Vyborny C.J., et. al.: Intelligent CAD workstation for breast imaging using similarity to known lesions and multiple visual prompt aids. Proc SPIE 2002; 4684: pp. 768-773.


- 16\. Aisen A.M., Broderick L.S., Winer-Muram H., et. al.: Automated storage and retrieval of thin-section CT images to assist diagnosis: system description and preliminary assessment. Radiology 2003; 228: pp. 265-270.


- 17\. Kawata Y., Niki N., Ohmatsu , et. al.: Example-based assisting approach for pulmonary nodule classification in three-dimensional thoracic computed tomography images. Acad Radiol 2003; 10: pp. 1402-1415.


- 18\. Muramatsu C., Li Q., Suzuki K., et. al.: Investigation of psychophysical measure for evaluation of similar images for mammographic masses: preliminary results. Med Phys 2005; 32: pp. 2295-2304.


- 19\. Nishikawa R.M., Yang Y., Huo D., et. al.: Observers' ability to judge the similarity of clustered calcifications on mammograms. Proc SPIE 2004; 5372: pp. 192-198.


- 20\. Muramatsu C., Li Q., Schmidt R.A., et. al.: Experimental determination of subjective similarity for pairs of clustered microcalcifications on mammograms: observer study results. Med Phys 2006; 33: pp. 3460-3468.


- 21\. Muramatsu C., Li Q., Schmidt R.A.: Determination of subjective similarity for pairs of masses and pairs of clustered microcalcifications on mammograms: comparison of similarity ranking scores and absolute similarity ratings. Med Phys 2007; 34: pp. 2890-2895.


- 22\. Zheng B., Lu A., Hardesty L.A., et. al.: A method to improve visual similarity of breast masses for an interactive computer-aided diagnosis environment. Med Phys 2006; 33: pp. 111-117.


- 23\. Kumazawa S., Muramatsu C., Li Q., et. al.: An investigation of radiologists' perception of lesion similarity: observations with paired breast masses on mammograms and paired lung nodules on CT images. Acad Radiol 2008; 15: pp. 887-894.


- 24\.  American College of Radiology.4th ed.2003.American College of RadiologyReston, VA


- 25\. Baker J.A., Kornguth P.J., Lo J.Y., et. al.: Breast cancer: prediction with artificial neural network based on BI-RADS standardized lexicon. Radiology 1995; 196: pp. 817-822.


- 26\. Heath M., Bowyer K., Kopans D., et. al.: The digital database for screening mammography.Yaffe M.J.Proceedings of the fifth international workshop on digital mammography.1998.Kluwer Academic PublishersDordrecht, Holland:pp. 212-218.


- 27\. Aoyama M., Li Q., Katsuragawa S., et. al.: Computerized scheme for determination of the likelihood measure of malignancy for pulmonary nodules on low-dose CT images. Med Phys 2003; 30: pp. 387-394.


- 28\. Huo Z., Giger M.L., Vyborny C.J., et. al.: Analysis of spiculation in the computerized classification of mammographic masses. Med Phys 1995; 22: pp. 1569-1579.