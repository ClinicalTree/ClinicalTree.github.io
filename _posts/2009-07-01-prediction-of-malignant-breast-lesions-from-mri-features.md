---
title: Prediction of Malignant Breast Lesions from MRI Features
author: [CL_AT_ChristineEMcLarenPhD,CL_AT_WenPinChenMS,CL_AT_KeNieMS,CL_AT_MinYingSuPhD]
date: 2009-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 16, Issue 7]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Dynamic contrast-enhanced magnetic resonance imaging is a clinical imaging modality for the detection and diagnosis of breast lesions. Analytic methods were compared for diagnostic feature selection and the performance of lesion classification to differentiate between malignant and benign lesions in patients.

## Materials and Methods

The study included 43 malignant and 28 benign histologically proved lesions. Eight morphologic parameters, 10 gray-level co-occurrence matrix texture features, and 14 Laws texture features were obtained using automated lesion segmentation and quantitative feature extraction. Artificial neural network (ANN) and logistic regression analysis were compared for the selection of the best predictors of malignant lesions among the normalized features.

## Results

Using ANN, the final four selected features were compactness, energy, homogeneity, and Law\_LS, with an area under the receiver-operating characteristic curve (AUC) of 0.82 and accuracy of 0.76. The diagnostic performance of these four features computed on the basis of logistic regression yielded an AUC of 0.80 (95% confidence interval \[CI\], 0.688–0.905), similar to that of ANN. The analysis also showed that the odds of a malignant lesion decreased by 48% (95% CI, 25%–92%) for every increase of 1 standard deviation in the Law\_LS feature, adjusted for differences in compactness, energy, and homogeneity. Using logistic regression with _z_ -score transformation, a model composed of compactness, normalized radial length entropy, and gray-level sum average was selected, and it had the highest overall accuracy, 0.75, among all models, with an AUC of 0.77 (95% CI, 0.660–0.880). When logistic modeling of transformations using the Box-Cox method was performed, the most parsimonious model with predictors compactness and Law\_LS had an AUC of 0.79 (95% CI, 0.672–0.898).

## Conclusion

The diagnostic performance of models selected by ANN and logistic regression was similar. The analytic methods were found to be roughly equivalent in terms of predictive ability when a small number of variables were chosen. The robust ANN methodology uses a sophisticated nonlinear model, while logistic regression analysis provides insightful information to enhance the interpretation of the model features.

Dynamic contrast-enhanced magnetic resonance imaging (MRI) is a clinical imaging modality for the detection and diagnosis of breast lesions. Computer algorithms have been used for automated lesion segmentation , with statistical analysis techniques applied to select an optimal set of features to achieve the highest diagnostic accuracy . Breast MRI has demonstrated high sensitivity (>95%), with specificity of approximately 67% reported by meta analysis . To address the challenge of accuracy and efficiency in the interpretation of breast MRI, a computer-aided diagnosis (CAD) system that can automatically analyze lesion features to differentiate between malignant and benign lesions would be very useful.

The general approach of breast CAD to predict a dichotomous outcome, malignant versus benign, involves applying computer algorithms for tumor characterization and then developing models using techniques including linear discriminate analysis , logistic regression analysis , and artificial neural networks (ANNs) for classifying a lesion as either malignant or benign. Because of inherent differences in these techniques, it is of interest to compare the diagnostic performance of analytic methods. In a review of 28 studies comparing ANN with other statistical approaches, Sargent found that ANN outperformed regression analysis in 36% of cases, ANN was outperformed by regression analysis in 14% of cases, and similar results were obtained in 50% of cases. The advantages of ANN for predicting a dichotomous outcome include a requirement of less formal statistical training, an ability to implicitly detect complex nonlinear relationships between dependent and predictor variables, consideration of all possible interactions between predictor variables, and the availability of multiple training algorithms. Disadvantages include the “black box” nature of the ANN procedure, a greater computational burden, the tendency for overfitting, and the empirical nature of model development . Logistic regression is superior for examining possible causal relationships between independent and dependent variables and understanding the effects of predictors on outcome variables . In summary, there is no universal approach to select models for data classification; the evaluation of tasks on a case-by-case basis is necessary.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Malignant and Benign Lesion Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ANN for Diagnostic Feature Selection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Logistic Regression Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

logit(p)=loge(p1−p).
logit

(

p

)

=

log

e

(

p

1

−

p

)

.


The logistic regression model enables the prediction of the probability of a malignant breast lesion in relation to _m_ lesion features, from an equation of the form


loge(p1−p)=β0+β1x1+β2x2+β3x3+⋯+βmxm,
log

e

(

p

1

−

p

)

=

β

0

+

β

1

x

1

+

β

2

x

2

+

β

3

x

3

+

⋯

+

β

m

x

m

,


where β  0 is the intercept term, and β  1 , β  2 , β  3 ,…, β _m_ are the coefficients in the model associated with the _m_ lesion features. It is assumed that the lesion features are linearly related to the log odds of the response. For a continuous lesion feature, the odds ratio for malignant versus benign lesions can be estimated as the exponentiation of the associated coefficient in the model .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation of ANN Models Using Logistic Regression

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Logistic Regression Analysis for Diagnostic Feature Selection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## ANN Diagnostic Feature Selection and Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Diagnostic Evaluation of Models Selected Using the ANN Technique


Model Imaging Descriptors  ¶  Method Accuracy  ∗  (%) Sensitivity  †  (%) Specificity  ‡  (%) PPV  §  NPV  \|\|  Estimated AUC 95% CI A Morphology (three selected from eight): volume, NRL entropy, compactness ANN 77 88 61 0.78 0.77 0.80 Logistic regression 76 93 50 0.74 0.82 0.80 0.686–0.912 B GLCM (three selected from 10): energy, gray-level sum average, homogeneity ANN 73 84 57 0.75 0.70 0.81 Logistic regression 68 86 39 0.69 0.65 0.77 0.660–0.880 C Laws (only one selected from 14): Law\_LS ANN 65 84 36 0.67 0.59 0.70 Logistic regression 65 86 32 0.66 0.60 0.70 0.573–0.819 D Combining all seven selected features: volume, NRL entropy, compactness, energy, gray-level sum average, homogeneity, Law\_LS ANN 79 81 75 0.83 0.72 0.87 Logistic regression 80 86 71 0.82 0.77 0.86 0.772–0.949 E Final (four selected from seven): compactness, energy, homogeneity, Law\_LS ANN 76 84 64 0.78 0.72 0.82 Logistic regression 72 86 50 0.73 0.70 0.80 0.688–0.905

ANN, artificial neural network; AUC, area under the receiver-operating characteristic curve; CI, confidence interval; GLCM, gray-level co-occurrence matrix; NPV, negative predictive value; NRL, normalized radial length; PPV, positive predictive value. For each model, the corresponding logistic regression equation also was applied to data from the full cohort ( _n_ = 71; 43 malignant, 28 benign).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, The dashed line represents the receiver-operating characteristic (ROC) curve for artificial neural network modeling of z scores ( Table 1 , model E: compactness, energy, homogeneity, and Law_LS; area under the ROC curve [AUC] = 0.82). The solid line represents the ROC curve for the four features as assessed by logistic regression ( Table 1 , model E, AUC = 0.80).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/PredictionofMalignantBreastLesionsfromMRIFeatures/0_1s20S1076633209001342.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

logit(p)=0.69+1.69compactness−0.61energy+0.24homogeneity−0.73Law\_LS.
logit

(

p

)

=

0.69

+

1.69

compactness

−

0.61

energy

+

0.24

homogeneity

−

0.73

Law

\_

LS

.


Law\_LS was the most predictive variable in the model (Wald statistic, _P_ = .028). The _P_ value of the Hosmer-Lemeshow test was .76, indicating a reasonably good fit of the model to the data. However, the adjusted _R_ 2 value for the model was 0.30, indicating that only 30% of the total variation in values could be explained by the predictor features in the model . The estimated odds ratio for Law\_LS was calculated as the exponentiation of the associated estimated coefficient, exp(−0.73) = 0.48. Thus the odds of a malignant lesion decreased by 48% (95% CI, 25%–92%) for every increase of 1 SD in the Law\_LS feature, adjusted for differences in compactness, energy, and homogeneity. For example, comparing a lesion with Law\_LS of 0.19, 1 SD above the mean of 0.13 for the set of 71 lesions, to a lesion with Law\_LS of 0.25, 2 SDs above the mean, the odds of the second lesion being malignant are about half those of the first lesion, assuming they have similar values for compactness, energy, and homogeneity.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Diagnostic Feature Selection Using Logistic Regression Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Diagnostic Evaluation of Models Selected Using Logistic Regression of Feature _z_ Scores With Fourfold Cross-Validation and Applied to Data From the Full Cohort ( _n_ = 71; 43 Malignant, 28 Benign)


Training Cohort Model With Highest AUC for Corresponding Validation Cohort  #  Likelihood Ratio χ  2 _P_ Accuracy  ∗  (%) Sensitivity  †  (%) Specificity  ‡  (%) PPV  §  NPV  \|\|  Estimated AUC  ¶  95% CI 1 Compactness, NRL entropy, energy 13.54 0.0036 73 95 39 0.71 0.85 0.75 0.626–0.879 2 Compactness, NRL entropy, gray-level sum average 17.86 0.0005 75 91 50 0.74 0.78 0.77 0.660–0.880 3, 4 Compactness, NRL entropy, Law\_LW 19.16 0.0003 72 86 50 0.73 0.70 0.80 0.690–0.908

AUC, area under the receiver-operating characteristic curve; CI, confidence interval; NPV, negative predictive value; NRL, normalized radial length; PPV, positive predictive value.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

logit(p)=0.66+1.28compactness−0.66NRLentropy+0.72gray-levelsum average.
logit

(

p

)

=

0.66

+

1.28

compactness

−

0.66

NRL

entropy

+

0.72

gray-level

sum average

.


Gray-level sum average was the most predictive variable in the model (Wald statistic, _P_ = .016). For this variable, the estimated odd ratio was exp(0.72) = 2.1 (95% CI, 1.14–3.68); thus, the odds of a malignant lesion increased by 2.1 for every increase of 1 SD in the gray-level sum average feature, adjusted for differences in compactness and NRL entropy. For example, comparing a lesion with gray-level sum average of 27.6, the mean for the 71 lesions, to a lesion with feature value of 34.2, 1 SD above the mean, the odds of the second lesion being malignant are over twice that of the first lesion, assuming they have similar values for compactness and NRL entropy.

![Figure 2, The solid line represents the receiver-operating characteristic (ROC) curve for logistic regression modeling of z scores for compactness, normalized radial length entropy, and gray-level sum average (area under the ROC curve [AUC] = 0.77; 95% CI, 0.660–0.880). The dashed line represents logistic regression model of Box-Cox-transformed values for compactness and Law_LS (AUC = 0.79; 95% CI, 0.672–0.898).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/PredictionofMalignantBreastLesionsfromMRIFeatures/1_1s20S1076633209001342.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

logit(p)=−5.650+0.666(ln compactness)−266.50\[(Law\_LS0.1)−1\]/(1/0.1).
logit

(

p

)

=

−

5.650

+

0.666

(

ln compactness

)

−

266.50

\[

(

Law

\_

LS

0.1

)

−

1

\]

/

(

1

/

0.1

)

.


For the natural log of compactness, the estimated odds ratio was exp(0.666) = 1.9, indicating that the odds of a malignant lesion increased by 1.9 (95% CI, 1.20–3.56) for every increase of 1 unit in the natural log of the morphologic feature compactness, adjusted for differences in the Laws feature Law\_LS. For example, comparing a lesion with natural log of compactness of 3.0, 1 SD above the mean of 1.6 for the set of 71 lesions, to that of a lesion with natural log of compactness of 4.5, 2 SDs above the mean, the second lesion would be nearly twice as likely to be malignant as the first lesion, assuming equal values for Law\_LS.


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

## References

- 1\. Chen W., Giger M.L., Bick U.: A fuzzy c-means (FCM)-based approach for computerized segmentation of breast lesions in dynamic contrast-enhanced MR images. Acad Radiol 2006; 13: pp. 63-72.


- 2\. Chen W., Giger M.L., Bick U., et. al.: Automatic identification and classification of characteristic kinetic curves of breast lesions on DCE-MRI. Med Phys 2006; 33: pp. 2878-2887.


- 3\. Chen W., Giger M.L., Lan L., et. al.: Computerized interpretation of breast MRI: investigation of enhancement-variance dynamics. Med Phys 2004; 31: pp. 1076-1082.


- 4\. Liney G.P., Sreenivas M., Gibbs P., et. al.: Breast lesion analysis of shape technique: semiautomated vs. manual morphological description. J Magn Reson Imaging 2006; 23: pp. 493-498.


- 5\. Meinel L.A., Stolpen A.H., Berbaum K.S., et. al.: Breast MRI lesion classification: improved performance of human readers with a backpropagation neural network computer-aided diagnosis (CAD) system. J Magn Reson Imaging 2007; 25: pp. 89-95.


- 6\. Esserman L., Hylton N., Yassa L., et. al.: Utility of magnetic resonance imaging in the management of breast cancer: evidence for improved preoperative staging. J Clin Oncol 1999; 17: pp. 110-119.


- 7\. Fischer U., Kopka L., Grabbe E.: Breast carcinoma: effect of preoperative contrast-enhanced MR imaging on the therapeutic approach. Radiology 1999; 213: pp. 881-888.


- 8\. Mumtaz H., Hall-Craggs M.A., Davidson T., et. al.: Staging of symptomatic primary breast cancer with MR imaging. AJR Am J Roentgenol 1997; 169: pp. 417-424.


- 9\. Rieber A., Schirrmeister H., Gabelmann A., et. al.: Pre-operative staging of invasive breast cancer with MR mammography and/or PET: boon or bunk?. Br J Radiol 2002; 75: pp. 789-798.


- 10\. Schelfout K., Van Goethem M., Kersschot E., et. al.: Contrast-enhanced MR imaging of breast lesions and effect on treatment. Eur J Surg Oncol 2004; 30: pp. 501-507.


- 11\. Zhang Y., Fukatsu H., Naganawa S., et. al.: The role of contrast-enhanced MR mammography for determining candidates for breast conservation surgery. Breast Cancer 2002; 9: pp. 231-239.


- 12\. Gilhuijs K.G., Giger M.L., Bick U.: Computerized analysis of breast lesions in three dimensions using dynamic magnetic-resonance imaging. Med Phys 1998; 25: pp. 1647-1654.


- 13\. Chou Y.H., Tiu C.M., Hung G.S., et. al.: Stepwise logistic regression analysis of tumor contour features for breast ultrasound diagnosis. Ultrasound Med Biol 2001; 27: pp. 1493-1498.


- 14\. Chan H.P., Sahiner B., Petrick N., et. al.: Computerized classification of malignant and benign microcalcifications on mammograms: texture analysis using an artificial neural network. Phys Med Biol 1997; 42: pp. 549-567.


- 15\. Sargent D.J.: Comparison of artificial neural networks with other statistical approaches. Cancer 2001; 91: pp. 1636-1642.


- 16\. Tu J.V.: Advantages and disadvantages of using artificial neural networks versus logistic regression for predicting medical outcomes. J Clin Epidemiol 1996; 49: pp. 1225-1231.


- 17\. Song J.H., Venkatesh S.S., Conant E.A., et. al.: Comparative analysis of logistic regression and artificial neural network for computer-aided diagnosis of beast masses. Acad Radiol 2005; 12: pp. 487-495.


- 18\. Nie K., Chen J.-H., Yu H.J., et. al.: Quantitative analysis of lesion morphology and texture features for diagnostic prediction in breast MRI. Acad Radiol 2008; 15: pp. 1513-1525.


- 19\. Haralick R.M., Shanmugam K., Dinstein I.: Textural features for image classification. IEEE Trans Syst Man Cybern 1973; SMC-3: 610–621


- 20\. Laws K.I.: Rapid texture identification.Image processing for missile guidance.1980.Society of Photo-Optical Instrumentation EngineersSan Diego, CA:pp. 376-380.


- 21\. Altman D.G.: Practical statistics for medical research.1991.Chapman & HallLondon


- 22\. DeLong E.R., DeLong D.M., Clarke-Pearson D.L.: Comparing the areas under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-845.


- 23\. Puri M.L., Sen P.K.: Nonparametric methods in multivariate analysis.1971.John WileyNew York


- 24\. Neter J., Kutner M., Nachtsheim C., et. al.: Applied linear statistical models.1996.WCB McGraw-HillNew York


- 25\. Harrell F.E., Cadiff R.M., Pryor D.B., et. al.: Evaluating the yield of medical tests. JAMA 1982; 247: pp. 2543-2546.


- 26\. Spitz M.R., Hong W.K., Amos C.I., et. al.: A risk model for prediction of lung cancer. J Natl Cancer Inst 2007; 99: pp. 715-726.


- 27\. Hosmer D.W., Lemeshow S.: Applied logistic regression.1989.John WileyNew York


- 28\. Nagelkerke N.J.D.: A note on a general definition of the coefficient of determination. Biometrika 1991; 78: pp. 691-692.


- 29\. Nilsson J., Ohlsson M., Thulin L., et. al.: Risk factor identification and mortality prediction in cardiac surgery using artificial neural networks. J Thorac Cardiovasc Surg 2006; 132: pp. 12-19.


- 30\. Clermont G., Angus D.C., DiRusso S.M., et. al.: Predicting hospital mortality for patients in the intensive care unit: a comparison of artificial neural networks with logistic regression models. Crit Care Med 2001; 29: pp. 291-296.


- 31\. Delen D., Walker G., Kadam A.: Predicting breast cancer survivability: a comparison of three data mining methods. Artif Intell Med 2005; 34: pp. 113-127.


- 32\. Jaimes F., Farbiarz J., Alvarez D., et. al.: Comparison between logistic regression and neural networks to predict death in patients with suspected sepsis in the emergency room. Crit Care 2005; 9: pp. R150-R156.


- 33\. Lundin M., Lundin J., Burke H.B., et. al.: Artificial neural networks applied to survival prediction in breast cancer. Oncology 1999; 57: pp. 281-286.


- 34\. Kohavi R.: A study of cross-validation and bootstrap for accuracy estimation and model selection.Proceedings of the Fourteenth International Joint Conference on Artificial Intelligence.1995.Morgan KaufmannSan Mateo, CA:pp. 1137-1143.


- 35\. Terrin N., Schmid C.H., Griffith J.L., et. al.: External validity of predictive models: a comparison of logistic regression, classification trees, and neural networks. J Clin Epidemiol 2003; 56: pp. 721-729.


- 36\. Efron B.: Estimating the error rate of a prediction rule: improvement on cross-validation. J Am Stat Assoc 1983; 78: pp. 316-331.


- 37\. Breiman L., Spector P.: Submodel selection and evaluation in regression. The X-random case. Int Stat Rev 1992; 60: pp. 291-319.


- 38\. Martens H., Næs T.: Multivariate calibration.1989.WileyChichester, UK


- 39\. Næs T., Mevik B.-H.: Understanding the collinearity problem in regression and discriminant analysis. J Chemometr 2001; 15: pp. 413-426.


- 40\. Weisberg S.: Applied linear regression.1985.John WileyNew York