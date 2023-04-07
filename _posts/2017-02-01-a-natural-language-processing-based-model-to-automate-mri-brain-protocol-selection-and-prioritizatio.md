---
title: A Natural Language Processing-based Model to Automate MRI Brain Protocol Selection and Prioritization
author: [CL_AT_AndrewDBrownMDMBA,CL_AT_ThomasRMarottaMD]
date: 2017-02-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 24, Issue 2]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Incorrect imaging protocol selection can contribute to increased healthcare cost and waste. To help healthcare providers improve the quality and safety of medical imaging services, we developed and evaluated three natural language processing (NLP) models to determine whether NLP techniques could be employed to aid in clinical decision support for protocoling and prioritization of magnetic resonance imaging (MRI) brain examinations.

## Materials and Methods

To test the feasibility of using an NLP model to support clinical decision making for MRI brain examinations, we designed three different medical imaging prediction tasks, each with a unique outcome: selecting an examination protocol, evaluating the need for contrast administration, and determining priority. We created three models for each prediction task, each using a different classification algorithm—random forest, support vector machine, or k-nearest neighbor—to predict outcomes based on the narrative clinical indications and demographic data associated with 13,982 MRI brain examinations performed from January 1, 2013 to June 30, 2015. Test datasets were used to calculate the accuracy, sensitivity and specificity, predictive values, and the area under the curve.

## Results

Our optimal results show an accuracy of 82.9%, 83.0%, and 88.2% for the protocol selection, contrast administration, and prioritization tasks, respectively, demonstrating that predictive algorithms can be used to aid in clinical decision support for examination protocoling.

## Conclusions

NLP models developed from the narrative clinical information provided by referring clinicians and demographic data are feasible methods to predict the protocol and priority of MRI brain examinations.

## Introduction

In recent years, much has been written about the use of clinical decision support tools to reduce the rates of inappropriate imaging examinations . However, even if an appropriate test is ordered, suboptimal imaging protocols can contribute to the waste of healthcare resources. Incorrect imaging protocols can contribute to increased healthcare costs , especially when imaging procedures must be repeated due to suboptimal examination results. In addition, optimizing protocol management has the potential to improve both safety and the patient's experience. For example, optimized computed tomography protocols tailored to an individual patient's specific diagnosis and demographic information can be performed with lower radiation doses, whereas optimized magnetic resonance imaging (MRI) protocols permit fast scanning—both of which contribute to a better overall patient experience .

To ensure the correct imaging protocols are chosen, some institutions assign radiologists the task of evaluating imaging requisitions before studies are approved. Requisitions contain the clinical histories of patients in the form of unstructured narratives written by referring clinicians, in addition to patient demographic information. However, the process of reviewing each requisition can be time-consuming, cumbersome, and prone to error . For example, studies may be delayed due to incomplete requisitions or the time required for clerical staff to locate radiologists to protocol studies. Automating the process of reviewing requisitions and selecting appropriate protocols through machine learning methods could provide an unbiased quantitative solution that reduces the time and cost associated with manual protocol selection while also creating an opportunity for personalized imaging.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Source

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Study Design

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Preparation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Data preparation and term-document matrix. In the pre-processing step, the clinical history contained in magnetic resonance imaging (MRI) requisitions was converted to lower case, and stopwords—words of little predictive power—were removed. Numbers and punctuation were then removed and, if applicable, each word was converted to its radical form. The processed sentences produce what is referred to as a term-document matrix, with each word representing a separate column and each row representing an MRI requisition.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ANaturalLanguageProcessingbasedModeltoAutomateMRIBrainProtocolSelectionandPrioritization/0_1s20S1076633216303270.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Prediction Models

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation and Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 1


Five Most Common Examination Protocols and Their Frequencies in Our Dataset (13,982 Imaging Studies)


Examination Protocols Frequency Fast brain 5320 Multiple sclerosis 2560 Sella 1800 Circle of Willis 1343 Internal acoustic canal 884

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 2


Dataset Characteristics for Protocol Selection, Contrast Administration, and Examination Prioritization Dataset


Dataset for Protocol Selection and Contrast Administration Models Characteristics Overall (13,982) Training (11,185) Testing (2797) Age \[mean (SD)\] 50.5(16.3) 50.6(16.3) 50.0(16.2) Female 60.4% 60.4% 61.9% Stat 10.4% 10.7% 9.4% Outpatient 79.5% 79.3% 80.7% No. of words  \\*  \[mean (SD)\] 5.6(3.4) 5.6(3.4) 5.6(3.4) Gadolinium 62.8% 62.8% 62.7%

Dataset for Prioritization Model Characteristics Overall (10,101) Training (8081) Testing (2019) Age \[mean (SD)\] 50.6(16.4) 50.0(16.3) 50.0(16.4) Female 60.7% 60.4% 61.9% Stat 10.5% 10.5% 10.5% Outpatient 79.3% 79.5% 79.0% No. of words  \\*  \[mean (SD)\] 5.6(3.3) 5.6(3.4) 5.6(3.3) Completed <24 hours 20.0% 20.0% 19.4%

SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 3


Performance Measures of Machine Learning Models to Predict Protocol Selection, Contrast Administration, and Examination Prioritization From Narrative Clinical Indications


Accuracy (%) Sensitivity (%) Specificity (%) PPV (%) NPV (%) Protocol model RF 82.9 82.9 96.5 82.2 96.3 KNN 77.2 77.2 97.1 75.8 94.3 SVM 81.4 81.4 92.9 83.2 97.2 Contrast model RF 83.0 76.7 86.8 77.5 86.2 KNN 74.4 66.7 79.0 65.4 80.0 SVM 81.2 74.9 85.0 74.8 85.1 Examination priority model RF 88.2 70.7 92.4 69.2 92.9 KNN 86.5 57.4 93.6 68.2 90.1 SVM 88.2 73.7 91.7 68.2 93.5

KNN, k-nearest neighbor algorithm; NPV, negative predictive value; PPV, positive predictive value; RF, random forest algorithm; SVM, support vector machine.


![Figure 2, Receiver operating characteristic curves of the performance of the random forest (RF), k-nearest neighbor (kNN), and support vector machine (SVM) models on Task 2, contrast administration. Area under the curve: RF—0.888; KNN—0.815; and SVM—0.875.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ANaturalLanguageProcessingbasedModeltoAutomateMRIBrainProtocolSelectionandPrioritization/1_1s20S1076633216303270.jpg)

![Figure 3, Receiver operating characteristic curves of the performance of random forest (RF), k-nearest neighbor (kNN), and support vector machine (SVM) models on Task 3, examination prioritization. Area under the curve: RF—0.863; KNN—0.847; and SVM—0.830.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ANaturalLanguageProcessingbasedModeltoAutomateMRIBrainProtocolSelectionandPrioritization/2_1s20S1076633216303270.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 4


Five Most Important Random Forest Variables in Protocol Selection, Contrast Administration, and Prioritization Prediction Tasks


Protocol Model Contrast Model Examination Priority Model Variable Importance Score Variable Importance Score Variable Importance Score Sclerosis  \\*  100 Neurosurgery  ‡  100 Outpatient  ‡  100 Aneurysm  \\*  82 Age  †  59 Inpatient  ‡  78 Pituitary  \\*  74 Follow-up  \\*  30 Stat order  ‡  65 Multiple  \\*  72 Endocrinology  ‡  28 Family  ‡  32 Endocrinology  ‡  57 Aneurysm  \\*  27 Age  †  32

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Bairstow P.J., Persaud J., Mendelson R., et. al.: Reducing inappropriate diagnostic practice through education and decision support. Int J Qual Health Care 2010; 22: pp. 194-200.


- 2\. Garg A.X., Adhikari N.K.J., McDonald H., et. al.: Effects of computerized clinical decision support systems on practitioner performance and patient outcomes: a systematic review. JAMA 2005; 293: pp. 1223-1238.


- 3\. Blackmore C.C., Castro A.: Improving the quality of imaging in the emergency department. Acad Emerg Med 2015; 22: pp. 1385-1392.


- 4\. Munn Z., Jordan Z.: The patient experience of high technology medical imaging: a systematic review of the qualitative evidence. Radiography 2011; 17: pp. 323-331.


- 5\. Boland G.W., Duszak R., Kalra M.: Protocol design and optimization. J Am Coll Radiol 2014; 11: pp. 440-441.


- 6\. Bell J.: Machine learning: hands-on for developers and technical professionals.2014.John Wiley & SonsIndianapolis, INpp. 1-15.


- 7\. Norrie J.: Mortality prediction in ICU: a methodological advance. Lancet Respir Med 2015; 3: pp. 5-6.


- 8\. Gultepe E., Green J.P., Nguyen H., et. al.: From vital signs to clinical outcomes for patients with sepsis: a machine learning basis for a clinical decision support system. J Am Med Inform Assoc 2014; 21: pp. 315-325.


- 9\. Berikol G.B., Yildiz O., Özcan I.T.: Diagnosis of acute coronary syndrome with a support vector machine. J Med Syst 2016; 40: pp. 1-8.


- 10\. R Core Team : R: a language and environment for statistical computing.2015.R Foundation for Statistical ComputingVienna, Austria


- 11\. Breiman L.: Random forests. Mach Learn 2001; 45: pp. 5-32.


- 12\. Cortes C., Vapnik V.: Support-vector networks. Mach Learn 1995; 20: pp. 273-297.


- 13\. Altman N.S.: An introduction to kernel and nearest-neighbor nonparametric regression. Am Stat 1992; 46: pp. 175-185.


- 14\. Chowdhury G.G.: Natural language processing. Annu Rev Inform Sci 2003; 37: pp. 51-89.


- 15\. Leaman R., Khare R., Lu Z.: Challenges in clinical natural language processing for automated disorder normalization. J Biomed Inform 2015; 57: pp. 28-37.


- 16\. Langley P., Sage S.: Scaling to domains with many irrelevant features.1997.MIT PressCambridge, MA:pp. 17-29.


- 17\. Pascual D.G.: Information theory-based techniques.Artificial intelligence tools: decision support systems in condition monitoring and diagnosis.2015.CRC PressBoca Raton, FL:pp. 428-429.


- 18\. Caruana R., Niculescu-Mizil A.: An empirical comparison of supervised learning algorithms.William CohenAndrew MooreProceedings of the 23rd International Conference on Machine Learning (ICML‘06).2006.ACMNew York, NY:pp. 161-168.


- 19\. Shi T., Horvath S.: Unsupervised learning with random forest predictors. J Comput Graph Stat 2006; 15: pp. 118-138.