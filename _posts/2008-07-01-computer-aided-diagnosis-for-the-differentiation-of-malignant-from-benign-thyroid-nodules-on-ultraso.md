---
title: Computer-Aided Diagnosis for the Differentiation of Malignant from Benign Thyroid Nodules on Ultrasonography
author: [CL_AT_KyoungJaLimMD,CL_AT_ChulSoonChoiMD,CL_AT_DaeYoungYoonMD,CL_AT_SukKiChangMD,CL_AT_KwangKiKimPhD,CL_AT_HeonHanMD,CL_AT_SamSooKimMD,CL_AT_JiwonLeeMD,CL_AT_YongHwanJeonMD]
date: 2008-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 15, Issue 7]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We sought to evaluate the diagnostic performance of an artificial neural network (ANN) and binary logistic regression (BLR) in differentiating malignant from benign thyroid nodules on ultrasonography.

## Materials and Methods

Two experienced radiologists, who were unaware of the histopathological diagnosis, analyzed ultrasonographic (US) features of 109 pathologically proven thyroid lesions (49 malignant and 60 benign) in 96 patients. Each radiologist was asked to evaluate US findings and categorize nodules into one of the two groups (malignant vs. benign) in each case. The following 8 US parameters were assessed for each nodule: size, shape, margin, echogenicity, cystic change, microcalcification, macrocalcification, and halo sign. Statistically significant US findings were obtained with backward stepwise logistic regression and were used for training and testing of the ANN and the BLR. The performance of the ANN and BLR was compared to that of the radiologists using receiver-operating characteristic (ROC) analysis.

## Results

Statistically significant US findings were size, margin, echogenicity, cystic change, and macrocalcification of the nodules. The area under the ROC curve ( _A  z_ ) values of ANN and BLR were 0.9492 ± 0.0195 and 0.9046 ± 0.0289, respectively. The _A  z_ value was 0.8300 ± 0.0359 for reader 1 and 0.7600 ± 0.0409 for reader 2. The _A  z_ values for ANN and BLR were significantly higher than those for both radiologists (all _p_ < .05).

## Conclusion

The performance of the ANN and the BLR was better than that of the radiologists in the distinction of benign and malignant thyroid nodules.

The widespread application of high-resolution ultrasonography has led to the discovery of small thyroid nodules with increasing frequency ( ). Although most thyroid nodules are benign, approximately 4% to 14% of such nodules are malignant ( ). Many studies have been published in which the ability to predict the histology of a thyroid nodule on the basis of ultrasonographic (US) findings has been assessed ( ). Several US features have been proposed as possible markers of malignancy, including the presence of fine or coarse calcifications, hypoechogenicity, irregular margins, absence of a halo, predominantly solid composition, a shape more tall than wide, and internal vascular flow ( ). However, differential diagnosis of thyroid nodules is often difficult and requires much experience and knowledge because of the considerable overlap in the appearance of benign and malignant thyroid nodules ( ).

In the past few decades, a number of computer-aided diagnosis (CAD) algorithms have been developed and implemented for accurate diagnosis of diseases, including artificial neural network (ANN), binary logistic regression (BLR), support vector machines, and the Bayesian approach ( ). These algorithms have recently been applied to the differential diagnosis of ovarian masses, pulmonary nodules, interstitial lung disease, pediatric lung lesions, and breast masses and shown to be potentially powerful tools ( ). However, to our knowledge, the usefulness of CAD has not been reported in the differential diagnosis of thyroid nodules on US images.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## US Examinations and Image Interpretation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ANN Procedure

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## BLR Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Q=11+e−z
Q

=

1

1

+

e

−

z


where _e_ is the base of natural logarithms and _Z_ is the linear combination calculated as _Z_ = _α_ \+ _β  1  x  1_ \+ _β  2  x  2_ \+ · · · \+ _β  n  x  n_ , in which α is the intercept, _β  n_ are coefficients estimated from the data, and _x  n_ are the predictor variables included in the model (  Table 1 ). If _Q_ was greater than 0.5, the case was classified as malignant. In our study, _x  n_ were US findings of thyroid nodules and we selected significant predictors for thyroid malignancy.

Table 1


Statistical Results for the Variables Related to US Features of Thyroid Nodules


Variables Estimates (β) Standard Error_p_ -Value Intercept  ⁎  3.759 2.476 .129 Size 0.694 0.401 .015 Shape −0.226 0.520 .666 Margin −1.216 0.418 .004 Echogenicity 1.021 0.402 .011 Cystic change −0.039 0.385 .027 Microcalcification −1.255 0.802 .118 Macrocalcification −1.465 0.761 .014 Halo −0.735 0.495 .137

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Receiver-operating characteristic (ROC) curves of artificial neural network and binary logistic regression. ROC curves show that the performance of the ANN ( A z value, 0.9492 ± 0.0195; 95% confidence interval, 0.8983−0.9774) ( a ) and BLR ( A z value, 0.9046 ± 0.0289; 95% confidence interval, 0.8350−0.9498) ( b ) was better than that of the two experienced radiologists ( A z value, 0.83 ± 0.0359; and A z value, 0.76 ± 0.0409 for radiologists 1 and 2, respectively) (all p < .05). A z value, area under ROC curve. Std. Err, standard error, 95% Conf, 95% confidence interval.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputerAidedDiagnosisfortheDifferentiationofMalignantfromBenignThyroidNodulesonUltrasonography/0_1s20S107663320800041X.jpg)

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

## Refernces

- 1\. Kim E.K., Park C.S., Chung W.Y., et. al.: Incidentally found thyroid nodules in women with no previous thyroid disease: Its significance. In: J Korean Radiol Soc 2002; pp. 449-453.


- 2\. Marqusee E., Benson C.B., Frates M.C., et. al.: Usefulness of ultrasonography in the management of nodular thyroid disease. Ann Intern Med 2000; 133: pp. 696-700.


- 3\. Mazzaferri E.L.: Management of a solitary thyroid nodule. N Engl J Med 1993; 328: pp. 553-559.


- 4\. Hegedus L.: Thyroid ultrasound. Endocrinol Metab Clin North Am 2001; 30: pp. 339-360.


- 5\. Pacini F., Schlumberger M., Dralle H., et. al.: European consensus for the management of patients with differentiated thyroid carcinoma of the follicular epithelium. Eur J Endocrinol 2006; 154: pp. 787-803.


- 6\. Frates M.C., Benson C.B., Doubilet P.M., et. al.: Can color Doppler sonography aid in the prediction of malignancy of thyroid nodules?. J Ultrasound Med 2003; 22: pp. 127-131. quiz 132–124


- 7\. Kim E.K., Park C.S., Chung W.Y., et. al.: New sonographic criteria for recommending fine-needle aspiration biopsy of nonpalpable solid nodules of the thyroid. AJR Am J Roentgenol 2002; 178: pp. 687-691.


- 8\. Papini E., Guglielmi R., Bianchini A., et. al.: Risk of malignancy in nonpalpable thyroid nodules: Predictive value of ultrasound and color-Doppler features. J Clin Endocrinol Metab 2002; 87: pp. 1941-1946.


- 9\. Ashizawa K., MacMahon H., Ishida T., et. al.: Effect of an artificial neural network on radiologists' performance in the differential diagnosis of interstitial lung disease using chest radiographs. AJR Am J Roentgenol 1999; 172: pp. 1311-1315.


- 10\. Biagiotti R., Desii C., Vanzi E., et. al.: Predicting ovarian malignancy: Application of artificial neural networks to transvaginal and color Doppler flow US. Radiology 1999; 210: pp. 399-403.


- 11\. Brem R.F., Hoffmeister J.W., Zisman G., et. al.: A computer-aided detection system for the evaluation of breast cancer by mammographic appearance and lesion size. AJR Am J Roentgenol 2005; 184: pp. 893-896.


- 12\. Chang R.F., Wu W.J., Moon W.K., et. al.: Improvement in breast tumor discrimination by support vector machines and speckle-emphasis texture analysis. Ultrasound Med Biol 2003; 29: pp. 679-686.


- 13\. Gross G.W., Boone J.M., Greco-Hunt V., et. al.: Neural networks in radiologic diagnosis. Invest Radiol 1990; 25: pp. 1017-1023.


- 14\. Kim S.H., Lee J.M., Kim J.H., et. al.: Appropriateness of a donor liver with respect to macrosteatosis: Application of artificial neural networks to US images—Initial experience. Radiology 2005; 234: pp. 793-803.


- 15\. Kobayashi T., Xu X.W., MacMahon H., et. al.: Effect of a computer-aided diagnosis scheme on radiologists' performance in detection of lung nodules on radiographs. Radiology 1996; 199: pp. 843-848.


- 16\. Warren Burhenne L.J., Wood S.A., D'Orsi C.J., et. al.: Potential contribution of computer-aided detection to the sensitivity of screening mammography. Radiology 2000; 215: pp. 554-562.


- 17\. Metz C.E.: ROC methodology in radiologic imaging. Invest Radiol 1986; 21: pp. 720-733.


- 18\. Frates M.C., Benson C.B., Charboneau J.W., et. al.: Management of thyroid nodules detected at US: Society of Radiologists in Ultrasound consensus conference statement. Radiology 2005; 237: pp. 794-800.


- 19\. Wu Y., Giger M.L., Doi K., et. al.: Artificial neural networks in mammography: Application to decision making in the diagnosis of breast cancer. Radiology 1993; 187: pp. 81-87.


- 20\. Abe H., Ashizawa K., Katsuragawa S., et. al.: Use of an artificial neural network to determine the diagnostic value of specific clinical and radiologic parameters in the diagnosis of interstitial lung disease on chest radiographs. Acad Radiol 2002; 9: pp. 13-17.


- 21\. Fukushima A., Ashizawa K., Yamaguchi T., et. al.: Application of an artificial neural network to high-resolution CT: Usefulness in differential diagnosis of diffuse lung disease. AJR Am J Roentgenol 2004; 183: pp. 297-305.


- 22\. Nakamura K., Yoshida H., Engelmann R., et. al.: Computerized analysis of the likelihood of malignancy in solitary pulmonary nodules with use of artificial neural networks. Radiology 2000; 214: pp. 823-830.


- 23\. Matsuki Y., Nakamura K., Watanabe H., et. al.: Usefulness of an artificial neural network for differentiating benign from malignant pulmonary nodules on high-resolution CT: Evaluation with receiver operating characteristic analysis. AJR Am J Roentgenol 2002; 178: pp. 657-663.