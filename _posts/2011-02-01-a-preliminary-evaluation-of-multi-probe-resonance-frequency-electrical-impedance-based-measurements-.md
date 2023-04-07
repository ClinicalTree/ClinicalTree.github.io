---
title: A Preliminary Evaluation of Multi-probe Resonance-frequency Electrical Impedance Based Measurements of the Breast
author: [CL_AT_BinZhengPhD,CL_AT_DrorLedermanPhD,CL_AT_JulesHSumkinDO,CL_AT_MargaritaLZuleyMD,CL_AT_MichelleZGrussBSMTASCP,CL_AT_LindaSLovyRTRMCTRDMSBR,CL_AT_DavidGurScD]
date: 2011-02-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 18, Issue 2]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to preliminarily assess the performance of a new, resonance-frequency electrical impedance spectroscopy (REIS) system in identifying young women who were recommended to undergo breast biopsy following imaging.

## Materials and Methods

A seven-probe REIS system was designed and assembled and is currently being prospectively tested. During examination, contact is made with the nipple and six concentric points on the breast skin. Signal sweeps are performed, and outputs ranging from 200 to 800 kHz at 5-kHz intervals are recorded. An initial set of 140 patients, including 56 who eventually had biopsies, 63 who had negative results on screening mammography, and 21 recalled for additional imaging but later determined to have negative results, was used. An initial set of 35 features, 33 representing impedance signal differences between breasts and two representing participant age and average breast density, was assembled and reduced by a genetic algorithm to 14. The performance of an artificial neural network–based classifier was assessed using a case-based leave-one-out method.

## Results

The substantially greater asymmetry between signals of mirror-matched regions ascertained from biopsy (“positive”) compared to nonbiopsy (“negative”) cases resulted in an artificial neural network classifier performance (area under the curve) of 0.830 ± 0.023. At 90% specificity, this classifier, optimized for “recommendation for biopsy” rather than “cancer,” detected 30 REIS-positive cases (54%), including six of nine (67%) actual cancer cases and six of nine women (67%) recommended for surgical excision of high-risk lesions.

## Conclusions

Asymmetry in impedance measurements between bilateral breasts may provide valuable discriminatory information regarding the presence of highly suspicious imaging-based findings.

The early detection of breast cancers in younger women (aged < 50 years) is a mammographically difficult and time-consuming task, primarily because of the low prevalence of disease and denser breast tissue (on average) that results in lower detection sensitivity and specificity . In recent years, a number of alternative and/or improved approaches have been investigated for this purpose. Full-field digital mammography, whole breast ultrasound, and magnetic resonance imaging are frequently used for this purpose . Other newer technologies, such as digital breast tomosynthesis and breast cone-beam computed tomography, are also being investigated . These new breast imaging modalities have demonstrated the ability to achieve improved detection performance in specific groups of women compared to film and/or digital mammography , resulting for example in the recent recommendation for periodic breast magnetic resonance imaging examinations in women at high risk as an adjunct to mammography . Often these technologies result in the detection of different cancers; hence, the information obtained is complementary to mammography . However, all of these imaging modalities have well-understood advantages and disadvantages, in particular when, and if, applied to a substantial fraction of the screened population with no known risk factors.

Despite these advances and the fact that mortality from breast cancer is decreasing, there is a serious continuing controversy about the efficacy of current screening practices in the United States . As related to women who are of prescreening age and those not complying with screening recommendations at an older age, there has been an interest in developing an inexpensive, non-radiation-based examination tool that is simple to use and interpret, which could be used during annual examinations at physicians’ offices in conjunction with the clinical breast examination. The underlying concept is that with the use of this new examination tool, any abnormalities in these women would be detected at an early time (and potentially at an earlier stage). Because of low cancer prevalence among younger women (aged < 50 years), there may be an important role for tools that could stratify these women into two groups, the majority of those who are at “average risk” and but a small fraction of those (eg, ≤10%) who are at significantly higher than average risk for having or developing breast cancer. Hence, women who do not participate in periodic imaging-based screening because of their age, or their personal choice, and are found to be “positive” on the basis of the stratification-type examination should be recommended to seek imaging-based evaluation because they were determined to belong to a “defined high-risk group” . This approach is therefore based on a “rule-in” concept rather than a “rule-out” one. Namely, such a stratification tool is in no way a competitor of imaging-based surveillance. Under this paradigm, every additional cancer that would be ultimately detected as a result of the practice, and the imaging that would follow, will likely be detected substantially earlier. As important perhaps, a stratification-type examination (tool) with these operational characteristics could become extremely important for individualized screening recommendations if annual imaging-based examinations, in particular at an earlier age (<50 years), is ultimately deemed to no longer be the standard of practice.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## The Multiprobe REIS System

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, The multiprobe resonance-frequency electrical impedance spectroscopy system installed in our clinical breast imaging facility.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APreliminaryEvaluationofMultiprobeResonancefrequencyElectricalImpedanceBasedMeasurementsoftheBreast/0_1s20S1076633210005283.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The REIS Examination

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acquired Output Signals

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, An example of three recorded breast electrical impedance spectroscopy (EIS) output signal sweeps for a single-probe channel.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APreliminaryEvaluationofMultiprobeResonancefrequencyElectricalImpedanceBasedMeasurementsoftheBreast/1_1s20S1076633210005283.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Study Participants

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The Initial Feature Pool

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Six sets of magnitude signal sweeps acquired from the right (a) and left (b) breasts of a 48-year-old participant with a biopsy-verified breast cancer.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APreliminaryEvaluationofMultiprobeResonancefrequencyElectricalImpedanceBasedMeasurementsoftheBreast/2_1s20S1076633210005283.jpg)

![Figure 4, Six sets of magnitude signal sweeps acquired from the right (a) and left (b) breasts of a 38-year-old woman whose mammograms were rated “negative” during the screening mammography examination that followed the resonance-frequency electrical impedance spectroscopy examination.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APreliminaryEvaluationofMultiprobeResonancefrequencyElectricalImpedanceBasedMeasurementsoftheBreast/3_1s20S1076633210005283.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

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


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Number of Occurrences by Orientation (Location) of the Mirror-matched Probe Pair (of Six Pairs) That Showed Maximum Resonance Frequency Differences Between Two Breasts


Probe pair position on the left and right breasts (o’clock) 12 and 12 2 and 10 4 and 8 6 and 6 8 and 4 10 and 2 Number of cases 34 27 18 19 10 32

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Optimization and Performance Assessment of the Machine Learning Classifier

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Experimental artificial neural network scoring (output) data and the fitted receiver-operating characteristic (ROC) curve for classifying 56 biopsy (positive) and 84 nonbiopsy (negative) cases. The area under the ROC curve is 0.830 ± 0.023.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APreliminaryEvaluationofMultiprobeResonancefrequencyElectricalImpedanceBasedMeasurementsoftheBreast/4_1s20S1076633210005283.jpg)

Table 2


ANN Overall Classification Performance Levels Measured by Areas Under the Receiver-operating Characteristic Curves and Associated Standard Deviations as a Function of the Number of ANN Training Iterations


Number of Iterations 500 1000 1500 2000 3000 Training 0.873 ± 0.021 0.893 ± 0.017 0.901 ± 0.018 0.909 ± 0.018 0.922 ± 0.017 Testing 0.826 ± 0.025 0.830 ± 0.023 0.804 ± 0.026 0.783 ± 0.030 0.778 ± 0.031

ANN, artificial neural network.


Table 3


Detection Performance of the Classifier by Biopsy Outcome, Type of Abnormality, and Density BI-RADS Category at Three Specificity Levels


Specificity 95% 90% 80% Biopsy result All 56 biopsy cases 22 (39%) 30 (54%) 41 (73%) Nine cancer cases 2 (22%) 6 (67%) 7 (78%) Nine high-risk cases 6 (67%) 6 (67%) 7 (78%) 38 benign biopsy cases 14 (37%) 18 (47%) 27 (71%) Abnormality 37 cases depicting only masses 14 (38%) 17 (46%) 25 (68%) Eight cases depicting calcifications only 4 (50%) 6 (75%) 6 (75%) 11 cases depicting both abnormalities 4 (36%) 7 (64%) 10 (91%) Breast density 12 BI-RADS category 2 cases 3 (25%) 5 (42%) 9 (75%) 36 BI-RADS category 3 cases 16 (44%) 20 (56%) 27 (75%) Eight BI-RADS category 4 cases 3 (38%) 5 (63%) 5 (63%)

BI-RADS, breast imaging reporting and data system.


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

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Smith R.A.: Breast cancer screening among women younger than age 50: a current assessment of the issues. CA Cancer J Clin 2000; 50: pp. 312-336.


- 2\. Pisano E.D., Gatsonis C., Hendrick E., et. al.: Diagnostic performance of digital versus film mammography for breast cancer screening. N Engl J Med 2005; 353: pp. 1773-1783.


- 3\. Fenton J.J., Egger J., Carney P.A., et. al.: Reality check: perceived versus actual performance of community mammographers. AJR Am J Roentgenol 2006; 187: pp. 42-46.


- 4\. Berg B.A., Gutierrez L., NessAiver M.S., et. al.: Diagnostic accuracy of mammography, clinical examination, US, and MR imaging in preoperative assessment of breast cancer. Radiology 2004; 233: pp. 830-849.


- 5\. Poplack S.P., Tosteson T.D., Kogel C.A., et. al.: Digital breast tomosynthesis: initial experience in 98 women with abnormal digital screening mammography. AJR Am J Roentgenol 2007; 189: pp. 616-623.


- 6\. Yang K., Kwan A.L., Huang S.Y., et. al.: Noise power properties of a cone-beam CT system for breast cancer detection. Med Phys 2008; 35: pp. 5317-5327.


- 7\. Warner E., Plewes D.B., Hill K.A., et. al.: Surveillance of BRCA1 and BRCA2 mutation carriers with magnetic resonance imaging, ultrasound, mammography, and clinical breast examination. JAMA 2004; 292: pp. 1317-1325.


- 8\. Kriege M., Brekelmans C.T., Boetes C., et. al.: Efficacy of MRI and mammography for breast-cancer screening in women with a familial or genetic predisposition. N Engl J Med 2004; 351: pp. 427-437.


- 9\. Gur D., Abrams G.S., Chough D.M., et. al.: Digital breast tomosynthesis: observer performance study. AJR Am J Roentgenol 2009; 193: pp. 586-591.


- 10\. Saslow D., Boetes C., Burke W., et. al.: American cancer society guidelines for breast screening with MRI as an adjunct to mammography. CA Cancer J Clin 2007; 57: pp. 168-185.


- 11\. Berlin L., Hall F.M.: More mammography muddle: emotions, politics, science, costs and polarization. Radiology 2010; 255: pp. 311-316.


- 12\. US Preventive Services Task Force: Screening for breast cancer: U.S. Preventive Services Task Force recommendation statement. Ann Intern Med 2009; 151: pp. 716-726.


- 13\. Stojadinovic A., Nissan A., Shriver C.D.: Electrical impedance scanning as a new breast cancer risk stratification tool for young women. J Surg Oncol 2008; 97: pp. 112-120.


- 14\. Chaundhary S.S., Mishra R.K., Swarup A., et. al.: Dielectric properties of breast carcinoma and surrounding tissues. IEEE Trans Biomed Eng 1988; 35: pp. 257-263.


- 15\. Pipemo G., Frei G., Moshitzky M.: Breast cancer screening by impedance measurement. Med Biol Eng 1990; 2: pp. 111-117.


- 16\. Malich A., Fritsch T., Anderson R., et. al.: Electrical impedance scanning for classifying suspicious breast lesions: first results. Eur Radiol 2000; 10: pp. 1555-1561.


- 17\. Kerner T.E., Paulsen K.D., Hartov A., et. al.: Electrical impedance spectroscopy of the breast: clinical imaging results in 26 subjects. IEEE Trans Med Imaging 2002; 21: pp. 638-645.


- 18\. Glickman Y.A., Filo O., Nachaliel U., et. al.: Novel EIS postprocessing algorithm for breast cancer diagnosis. IEEE Trans Med Imaging 2002; 21: pp. 710-712.


- 19\. Sumkin J.H., Stojadinovic A., Huerbin M., et. al.: Impedance measurements for early detection of breast cancer in younger women: a preliminary assessment. Proc SPIE 2003; 5034: pp. 197-203.


- 20\. Poplack S.P., Paulsen K.D., Hartov A., et. al.: Electromagnetic breast imaging: average tissue property values in women with negative clinical findings. Radiology 2004; 231: pp. 571-580.


- 21\. Stojadinovic A., Nissan A., Gallimidi Z., et. al.: Electrical impedance scanning for the early detection of breast cancer in young women: preliminary results of a multicenter prospective clinical trial. J Clin Oncol 2005; 23: pp. 2703-2715.


- 22\. Stojadinovic A., Moskovitz O., Gallimidi Z., et. al.: Prospective study of electrical impedance scanning for identifying young women at risk for breast cancer. Breast Cancer Res Treat 2006; 97: pp. 179-189.


- 23\. Fricke H., Morse S.: The electric capacity of tumors of the breast. J Cancer Res 1926; 16: pp. 310-376.


- 24\. Hope T.A., Iles S.E.: Technology review: the use of electrical impedance scanning in the detection of breast cancer. Breast Cancer Res 2004; 6: pp. 69-74.


- 25\. Sumkin J.H., Zheng B., Gruss M., et. al.: Assembling a prototype resonance electrical impedance spectroscopy system for breast tissue signal detection: preliminary assessment. Proc SPIE 2008; 6917: pp. 691716.


- 26\. Zheng B., Zuley M.L., Sumkin J.H., et. al.: Detection of breast abnormalities using a prototype resonance electrical impedance spectroscopy system: a preliminary study. Med Phys 2008; 35: pp. 3041-3048.


- 27\. Gur D., Zheng B., Dhurjaty S., et. al.: Developing and testing a multi-probe resonance electrical impedance spectroscopy system for detecting breast abnormalities. Proc SPIE 2009; 7263: pp. 72631F.


- 28\. Zheng B., Chang Y.H., Wang X.H., et. al.: Feature selection for computerized mass detection in digitized mammograms by using a genetic algorithm. Acad Radiol 1999; 6: pp. 327-332.


- 29\. Zheng B., Chang Y.H., Good W.F., et. al.: Performance gain in computer-assisted detection schemes by averaging scores generated from artificial neural networks with adaptive filtering. Med Phys 2001; 28: pp. 2302-2308.


- 30\. Zheng B., Lu A., Hardesty L.A., et. al.: A method to improve visual similarity of breast masses for an interactive computer-aided diagnosis environment. Med Phys 2006; 33: pp. 111-117.


- 31\. Kantrowitz M.: Prime time freeware for AI, issue 1-1: selected materials from the Carnegie Mellon University, Artificial Intelligence Repository.1994.Prime Time FreewareSunnyvale, CA