---
title: Statistical Methods for Predicting Mo rtality in Patients Diagnosed with Acute Pulmonary Embolism
author: [Layla Parast PhD,Bryan Cai,Arash Bedayat MD,Kanako K. Kumamaru MD PhD,Elizabeth George MBBS,Karin E. Dill MD,Frank J. Rybicki MD PhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 12 SOURCE CL_S_AcademicRadiologyVolume19Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Risk stratification in pulmonary embolism (PE) guides patient management. The purpose of this study was to develop and test novel mortality risk prediction models for subjects with acute PE diagnosed using computed tomographic pulmonary angiography in a large cohort with comprehensive clinical data.

## Materials and Methods

Retrospective analyses of 1596 consecutive subjects diagnosed with acute PE from a single, large, urban teaching hospital included two modern statistical methods to predict survival in patients with acute PE. Landmark analysis was used for 90-day mortality. Adaptive least absolute shrinkage and selection operator (aLASSO), a penalization method, was used to select variables important for prediction and to estimate model coefficients. Receiver-operating characteristic analysis was used to evaluate the resulting prediction rules.

## Results

Using 30-day all-cause mortality outcome, three of the 16 clinical risk factors (the presence of a known malignancy, coronary artery disease, and increased age) were associated with high risk, while subjects treated with anticoagulation had lower risk. For 90-day landmark mortality, subjects with recent operations had a lower risk for death. Both prediction rules developed using aLASSO performed well compared to standard logistic regression.

## Conclusions

The aLASSO regression approach combined with landmark analysis provides a novel tool for large patient populations and can be applied for clinical risk stratification among subjects diagnosed with acute PE. After positive results on computed tomographic pulmonary angiography, the presence of a known malignancy, coronary artery disease, and advanced age increase 30-day mortality. Additional risk stratification can be simplified with these methods, and future work will place imaging-based prediction of mortality in perspective with other clinical data.

Acute pulmonary embolism (PE) is a common, life-threatening disease that has a variable clinical course; for example, some patients rapidly develop cardiogenic shock leading to death, while others present with only mild dyspnea . Therefore, risk stratification is essential to determine the most appropriate treatment, including those patients who would benefit from more aggressive therapies (eg, thrombolysis or thrombectomy) and those for whom outpatient treatment is appropriate. Several studies have suggested objective clinical factors that predict early death after PE, such as cancer, increasing age, heart failure, and chronic obstructive pulmonary disease . The PE severity index or simplified PE severity index is designed to stratify patients into five risk classes using clinical factors and identifies patients at low risk for short-term mortality . Most, if not all, prognostic studies have used either 30-day or 90-day mortality, as well as in-hospital mortality, as clinical end points.

It has been shown that right ventricular (RV) dysfunction is important for prognosis, because mortality from acute PE is mainly from acute right-heart failure . With respect to imaging, echocardiography is often used to evaluate RV dysfunction. However, considerable effort has focused on using computed tomographic pulmonary angiographic (CTPA) findings to detect RV strain . The rationale is that CTPA images are readily available because computed tomography (  Fig 1 ) is generally used to confirm the clinical suspicion of PE . The most commonly used metric is RV enlargement as measured by the RV/left ventricular diameter ratio . However, following studies that used PE-specific death to assess the efficacy of inferior vena cava filter placement , the work of Grifoni et al introduced so-called PE-related mortality. Although clear decision rules to determine patients who died from PE have not been published to our knowledge, it is likely that prediction rules that use more targeted mortality data will have better receiver-operating characteristic (ROC) performance than similar data using all-cause mortality. In this study, we did not consider the RV/left ventricular diameter ratio as a potential predictor, and only all-cause mortality information is available.

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633211X00235/S1076633212004758/gr1.jpg?Signature=GeLY%7E1mZiVub8W4QxttzoIrkRRoTN3C8gXj%7E-6o25ddc5lOHr%7Ex8Y40T3yqBWvP40k%7EoGvM9PDyRMmgk7w4oXMJkyE7dCWpYkHLXxYiXvh3sm3qJfpgNweOrN%7E9ybsMn-lOrXFiJz0nCI3H4fkfv%7Esrpexxt6MuJ1Iuz4VyXeuM_&Expires=1669572645&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


A 67-year-old woman with a history of endometrial cancer presented with shortness of breath and hypoxia. Computed tomographic pulmonary angiography showed extensive pulmonary emboli filling defects in the left pulmonary arteries **(a)** . Axial images chosen at the maximum right ventricular **(b)** and left ventricular **(c)** diameters reveal an enlarged ratio of right ventricular to left ventricular size. The patient died 11 days later from acute pulmonary embolism.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Study Population

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Measurements and Outcomes

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Variable Selection and Statistical Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

logP(Y=1\|x)P(Y=0\|x)=x′β,
log

P

(

Y

=

1

\|

x

)

P

(

Y

=

0

\|

x

)

=

x

′

β

,


where _x_ and β denote vectors of the predictors and the unknown coefficients, respectively . The coefficient vector β = (β  1 ,…, β _p_ ) is estimated by solving a set of nonlinear equations that satisfy the maximum likelihood criterion. In particular, the standard logistic regression estimates β as the maximizer of the log-likelihood function, _ℓ__n_ (β), denoted by βˆ
β

ˆ
. This approach uses all available variables to fit the data, whether the variables are significant or not. In a high-dimensional setting in which the number of predictors _p_ is large relative to the number of observations _n_ , the problem of overfitting can be a serious issue and lead to unstable and poor performing models . An effective alternative approach, LASSO, is to shrink regression coefficients by imposing a penalization on the _ℓ_ 1 -norm of the coefficients to obtain a sparse and more interpretable model . The favorable performance of logistic regression with this type of penalization has been extensively studied . The aLASSO estimator uses a weighted penalization approach and is the solution to a penalized minimization problem, as described in detail in the  Appendix . The estimated coefficients are denoted by βˆ(λ)
β

ˆ

(

λ

)
, where λ > 0 is the penalty parameter. This weighted penalization leads to a sparse model with the selection of important variables by setting βˆ(λ)=0
β

ˆ

(

λ

)

=

0
for variables not selected. This yields a model that is more interpretable and has better performance for future predictions.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Landmark Analysis and Risk Prediction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation Using ROC Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Sens30(c)=P\[pˆi(30)>c\|Yi(30)=1\]
Sens

30

(

c

)

=

P

\[

p

ˆ

i

(

30

)

>

c

\|

Y

i

(

30

)

=

1

\]


and


Spec30(c)=P\[pˆi(30)≤c\|Yi(30)=0\].
Spec

30

(

c

)

=

P

\[

p

ˆ

i

(

30

)

≤

c

\|

Y

i

(

30

)

=

0

\]

.


One may summarize the trade-offs between the sensitivity and specificity using the ROC curve, ROC30(u)=Sens30{Spec−130(1−u)}
ROC

30

(

u

)

=

Sens

30

{

Spec

30

−

1

(

1

−

u

)

}
and the area under the ROC curve (AUC), AUC30=∫ROC30(u)du
AUC

30

=

∫

ROC

30

(

u

)

d

u
, can be used as an overall accuracy measure. With such a prediction rule, one may also consider the positive predictive value (PPV) and negative predictive value (NPV) functions, defined as


PPV30(c)=P\[Yi(30)=1\|pˆi(30)>c\]
PPV

30

(

c

)

=

P

\[

Y

i

(

30

)

=

1

\|

p

ˆ

i

(

30

)

>

c

\]


and


NPV30(c)=P\[Yi(30)=0\|pˆi(30)≤c\].
NPV

30

(

c

)

=

P

\[

Y

i

(

30

)

=

0

\|

p

ˆ

i

(

30

)

≤

c

\]

.


Similarly, when predicting 90-day landmark mortality, for any given risk score, pˆi(90\|30)
p

ˆ

i

(

90

\|

30

)
, and cutoff value, c∗
c

∗
, the discrimination accuracy of pˆi(90\|30)
p

ˆ

i

(

90

\|

30

)
for classifying Yi(90\|30)
Y

i

(

90

\|

30

)
can be summarized by the functions


Sens90\|30(c∗)=P\[pˆi(90\|30)>c\|Yi(90\|30)=1\],
Sens

90

\|

30

(

c

∗

)

=

P

\[

p

ˆ

i

(

90

\|

30

)

>

c

\|

Y

i

(

90

\|

30

)

=

1

\]

,


Spec90\|30(c∗)=P\[pˆi(90\|30)≤c∗\|Yi(90\|30)=0\],
Spec

90

\|

30

(

c

∗

)

=

P

\[

p

ˆ

i

(

90

\|

30

)

≤

c

∗

\|

Y

i

(

90

\|

30

)

=

0

\]

,


PPV90\|30(c∗)=P\[Yi(90\|30)=1\|pˆi(90\|30)>c∗\],
PPV

90

\|

30

(

c

∗

)

=

P

\[

Y

i

(

90

\|

30

)

=

1

\|

p

ˆ

i

(

90

\|

30

)

>

c

∗

\]

,


and


NPV90\|30(c∗)=P\[Yi(90\|30)=0\|pˆi(90\|30)≤c∗\]
NPV

90

\|

30

(

c

∗

)

=

P

\[

Y

i

(

90

\|

30

)

=

0

\|

p

ˆ

i

(

90

\|

30

)

≤

c

∗

\]


and ROC curve ROC90\|30(u)=Sens90\|30{Spec−190\|30(1−u)}
ROC

90

\|

30

(

u

)

=

Sens

90

\|

30

{

Spec

90

\|

30

−

1

(

1

−

u

)

}
with corresponding AUC, AUC90\|30=∫ROC90\|30(u)du
AUC

90

\|

30

=

∫

ROC

90

\|

30

(

u

)

d

u
. Note that the possible cutoff values, _c_ and c∗
c

∗
, range from 0 to 1 and represent the various decision thresholds that could be considered. In settings with a limited number of decision thresholds, as is common in studies of radiologic devices, ROC analysis should be approached with care .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Sensˆ30(c)=∑iI\[pˆi(30)>c\]Yi(30)∑iYi(30),
Sens

ˆ

30

(

c

)

=

∑

i

I

\[

p

ˆ

i

(

30

)

>

c

\]

Y

i

(

30

)

∑

i

Y

i

(

30

)

,


where _I_ ( _x_ ) is the indicator function, which is equal to 1 if _x_ is true and 0 otherwise, and AUC  30 is estimated by


AUCˆ30=∑i∑jI{pˆi(30)>pˆj(30)∣∣Yi(30)=1,Yj(30)=0}∑i∑jYi(30)\[1−Yj(30)\].
AUC

ˆ

30

=

∑

i

∑

j

I

{

p

ˆ

i

(

30

)

>

p

ˆ

j

(

30

)

\|

Y

i

(

30

)

=

1

,

Y

j

(

30

)

=

0

}

∑

i

∑

j

Y

i

(

30

)

\[

1

−

Y

j

(

30

)

\]

.


Similarly, Sens90\|30(c\*)
Sens

90

\|

30

(

c

\*

)
is estimated by


Sensˆ30,90(c∗)=∑i∈Ω30I\[pˆi(90\|30)>c∗\]Yi(90\|30)∑i∈Ω30Yi(90\|30),
Sens

ˆ

30

,

90

(

c

∗

)

=

∑

i

∈

Ω

30

I

\[

p

ˆ

i

(

90

\|

30

)

>

c

∗

\]

Y

i

(

90

\|

30

)

∑

i

∈

Ω

30

Y

i

(

90

\|

30

)

,


and AUC90\|30
AUC

90

\|

30
is estimated by


AUCˆ90\|30=∑i∈Ω30∑j∈Ω30I{pˆi(90\|30)>pˆj(90\|30)∣∣Yi(90\|30)=1,Yj(90\|30)=0}∑i∈Ω30∑j∈Ω30Yi(90\|30)\[1−Yj(90\|30)\].
AUC

ˆ

90

\|

30

=

∑

i

∈

Ω

30

∑

j

∈

Ω

30

I

{

p

ˆ

i

(

90

\|

30

)

>

p

ˆ

j

(

90

\|

30

)

\|

Y

i

(

90

\|

30

)

=

1

,

Y

j

(

90

\|

30

)

=

0

}

∑

i

∈

Ω

30

∑

j

∈

Ω

30

Y

i

(

90

\|

30

)

\[

1

−

Y

j

(

90

\|

30

)

\]

.


Spec  30 ( _c_ ), PPV  30 ( _c_ ), NPV  30 ( _c_ ), Spec90\|30(c\*)
Spec

90

\|

30

(

c

\*

)
, PPV90\|30(c\*)
PPV

90

\|

30

(

c

\*

)
, and NPV90\|30(c\*)
NPV

90

\|

30

(

c

\*

)
can be similarly estimated. To compensate for potential model overfitting, fivefold cross-validation was performed to estimate all accuracy measures. Apparent estimates were all calculated to demonstrate the potential for overfitting. SE estimates were obtained using the bootstrap with 200 bootstrap samples taken . An alternative approach that may be considered for selecting important variables and estimating corresponding coefficients that combines penalization techniques and ROC concepts is to minimize a surrogate loss function, as proposed by Zhao et al .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Demographics and Clinical Characteristics of Subjects Diagnosed with Acute PE by CT Pulmonary Angiography


All Subjects Subjects with _T_ L _i_ \> 30 Days Variable ( _n_ = 1596) ( _n_ = 1408) Men 714 (44.7%) 635 (45.1%) Age (y) 57.8 ± 16.7 57.0 ± 16.9 Cancer 835 (52.3%) 671 (47.7%) Recent operation 608 (38.1%) 554 (39.3%) Atrial fibrillation 103 (6.5%) 88 (6.2%) Diabetes 237 (14.8%) 210 (14.9%) Hypertension 648 (40.6%) 575 (40.8%) CHF 83 (5.2%) 72 (5.1%) CAD 203 (12.7%) 167 (11.9%) PAD 49 (3.1%) 41 (2.9%) Coagulopathies 70 (4.4%) 66 (4.7%) Stroke 70 (4.4%) 63 (4.5%) CRI 48 (3.0%) 43 (3.1%) IVC filter 105 (6.6%) 95 (6.7%) Lung disease 214 (13.4%) 189 (13.4%) Anticoagulants  ∗  1483 (92.9%) 1326 (94.2%)

CAD, coronary artery disease; CHF, congestive heart failure; CRI, chronic renal insufficiency; CT, computed tomographic; IVC, inferior vena cava; PAD, peripheral artery disease; PE, pulmonary embolism.


Data are expressed as number (percentage) or as mean ± standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Estimates of β(λ) and β  30  (λ  30  ) with Corresponding SEs Obtained Using Bootstrap


30-Day Mortality 90-Day Landmark Mortality Variable β(λ) SE_P_ β  30  (λ  30  ) SE_P_ Cancer 1.967 0.241 <.001 1.722 0.256 <.001 Anticoagulants  ∗  −1.219 0.283 <.001 −0.855 0.392 .029 Age 0.026 0.007 <.001 0.017 0.007 .021 CAD 0.590 0.281 .036 −0.463 0.423 .274 Hypertension −0.361 0.197 .067 −0.235 0.242 .332 Recent operation −0.344 0.207 .096 −0.842 0.237 <.001 IVC filter −0.773 0.524 .140 0.586 0.367 .110 Male gender −0.201 0.172 .242 0 Stroke −0.331 1.190 .781 0.749 0.487 .124 Atrial fibrillation 0 0 Diabetes 0 0 CHF 0 0 PAD 0 0 Coagulopathies 0 −1.233 6.894 .858 CRI 0 0 Lung disease 0 0.442 0.363 .224

CAD, coronary artery disease; CHF, congestive heart failure; CRI, chronic renal insufficiency; CT, computed tomographic; IVC, inferior vena cava; PAD, peripheral artery disease; SE, standard error.


A coefficient of zero indicates that the variable was not chosen to be in the respective model.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Apparent and cross-validated receiver-operating characteristic (ROC) curves for 30-day mortality predictions using standard logistical model and adaptive least absolute shrinkage and selection operator (Lasso).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalMethodsforPredictingMortalityinPatientsDiagnosedwithAcutePulmonaryEmbolism/0_1s20S1076633212004758.jpg)

![Figure 3, Apparent and cross-validated receiver-operating characteristic (ROC) curves for 90-day landmark mortality predictions using standard logistical model and adaptive least absolute shrinkage and selection operator (Lasso).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalMethodsforPredictingMortalityinPatientsDiagnosedwithAcutePulmonaryEmbolism/1_1s20S1076633212004758.jpg)

Table 3


Receiver-operating Characteristic Analysis for Prediction Models for 30-Day Mortality and 90-Day Landmark Mortality with Apparent Estimates, Cross-validated Estimates, and Standard Error Estimates Using the Bootstrap


Standard Logistic aLASSO Variable AP CV SE AP CV SE 30-day mortality AUC 0.771 0.73 0.017 0.771 0.741 0.017 Sensitivity 0.494 0.413 0.039 0.489 0.455 0.041 PPV 0.397 0.356 0.026 0.395 0.378 0.026 NPV 0.930 0.920 0.007 0.930 0.925 0.008 90-day landmark mortality AUC 0.781 0.735 0.019 0.778 0.753 0.020 Sensitivity 0.518 0.439 0.052 0.509 0.447 0.056 PPV 0.335 0.300 0.030 0.331 0.303 0.032 NPV 0.950 0.943 0.007 0.949 0.944 0.007

AP, apparent estimate; AUC, area under the receiver-operating characteristic curve; CV, cross-validated estimate; NPV, negative predictive value; PPV, positive predictive value; SE, standard error estimate.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

βˆ=argmaxβℓn(β)=argmaxβ∑ni=1\[Yiβ′Xi−log{1+exp(β′Xi)}\].
β

ˆ

=

arg

max

β

ℓ

n

(

β

)

=

arg

max

β

∑

i

=

1

n

\[

Y

i

β

′

X

i

−

log

{

1

+

exp

(

β

′

X

i

)

}

\]

.


The aLASSO estimator uses a weighted penalization approach and is the solution to the following penalized minimization problem:


βˆ(λ)=argminβ{−ℓn(β)+λ∑pj=1wj\|βj\|},
β

ˆ

(

λ

)

=

arg

min

β

{

−

ℓ

n

(

β

)

+

λ

∑

j

=

1

p

w

j

\|

β

j

\|

}

,


where λ > 0 is the penalty parameter and _w_ = ( _w_ 1 ,…, _w__p_ ) is a vector of weights. In our analysis, the weights vector is chosen to be w=1∣∣∣βˆ(LR)∣∣∣
w

=

1

\|

β

ˆ

(

LR

)

\|
, where βˆ(LR)
β

ˆ

(

LR

)
is the standard logistic regression estimator of β. The value of the penalty parameter λ is chosen on the basis of a modified Bayesian information criterion with the penalty factor log( _n_ ) replaced by min{log(n),(∑iYi)0.1}
min

{

log

(

n

)

,

(

∑

i

Y

i

)

0.1

}
. This factor was chosen to account for the rarity of the event and decrease the model size penalty in finite samples.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

βˆ30(λ30)=argminβ30{−ℓn(β30)+λ30∑pj=1wj\|β30,j\|},
β

ˆ

30

(

λ

30

)

=

arg

min

β

30

{

−

ℓ

n

(

β

30

)

+

λ

30

∑

j

=

1

p

w

j

\|

β

30

,

j

\|

}

,


where


ℓn30(β30)=∑n30i=1\[Yi(90\|30)β′30Xi−log{1+exp(β′30Xi)}\],
ℓ

n

30

(

β

30

)

=

∑

i

=

1

n

30

\[

Y

i

(

90

\|

30

)

β

′

30

X

i

−

log

{

1

+

exp

(

β

′

30

X

i

)

}

\]

,


where β  30 is the unknown coefficient vector among Ω30
Ω

30
, and λ  30 is the penalty parameter.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Carson J., Kelley M., Duff A., et. al.: The clinical course of pulmonary embolism. N Engl J Med 1992; 326: pp. 1240-1245.


- 2\. Tapson V.: Acute pulmonary embolism. N Engl J Med 2008; 358: pp. 1037-1052.


- 3\. Goldhaber S., Visani L., De Rosa M.: Acute pulmonary embolism: clinical outcomes in the International Cooperative Pulmonary Embolism Registry (ICOPER). Lancet 1999; 353: pp. 1386-1389.


- 4\. Aujesky D., Perrier A., Roy P., et. al.: Validation of a clinical prognostic model to identify low-risk patients with pulmonary embolism. J Intern Med 2007; 261: pp. 597-604.


- 5\. Wicki J., Perrier A., Perneger T., et. al.: Predicting adverse outcome in patients with acute pulmonary embolism: a risk score. Thromb Haemost 2000; 84: pp. 548-552.


- 6\. Wood K.: Major pulmonary embolism. Chest 2002; 121: pp. 877-905.


- 7\. Ghaye B., Ghuysen A., Bruyere P., et. al.: Can CT pulmonary angiography allow assessment of severity and prognosis in patients presenting with pulmonary embolism? What the radiologist needs to know. Radiographics 2006; 26: pp. 23-39.


- 8\. Henzler T., Krissak R., Reichert M., et. al.: Volumetric analysis of pulmonary CTA for the assessment of right ventricular dysfunction in patients with acute pulmonary embolism. Acad Radiol 2010; 17: pp. 309-315.


- 9\. Quiroz R., Kucher N., Schoepf U., et. al.: Right ventricular enlargement on chest computed tomography. Circulation 2004; 109: pp. 2401-2404.


- 10\. Schoepf U., Kucher N., Kipfmueller F., et. al.: Right ventricular enlargement on chest computed tomography. Circulation 2004; 110: pp. 3276-3280.


- 11\. Hunsaker A., Lu M., Goldhaber S., et. al.: Imaging in acute pulmonary embolism with special clinical scenarios. Circ Cardiovasc Imaging 2010; 3: pp. 491-500.


- 12\. Lu M., Demehri S., Cai T., et. al.: Axial and reformatted four-chamber right ventricle–to–left ventricle diameter ratios on pulmonary ct angiography as predictors of death after acute pulmonary embolism. AJR Am J Roentgenol 2012; 198: pp. 1353-1360.


- 13\. Lu M., Ersoy H., Whitmore A., et. al.: Reformatted four-chamber and short-axis views of the heart using thin section (≤ 2 mm) MDCT images. Acad Radiol 2007; 14: pp. 1108-1112.


- 14\. Alexander J., Yuhas J., Piotrowski J.: Is the increasing use of prophylactic percutaneous IVC filters justified?. Am J Surg 1994; 168: pp. 102-106.


- 15\. Ferris E., McCowan T., Carver D., et. al.: Percutaneous inferior vena caval filters: follow-up of seven designs in 320 patients. Radiology 1993; 188: pp. 851-856.


- 16\. Grifoni S., Olivotto I., Cecchini P., et. al.: Short-term clinical outcome of patients with acute pulmonary embolism, normal blood pressure, and echocardiographic right ventricular dysfunction. Circulation 2000; 101: pp. 2817-2822.


- 17\. Van Houwelingen H.: Dynamic prediction by landmarking in event history analysis. Scand J Stat 2007; 34: pp. 70-85.


- 18\. Anderson J., Cain K., Gelber R.: Analysis of survival by tumor response. J Clin Oncol 1983; 1: pp. 710.


- 19\.  Parast L, Cai T. Landmark prediction of survival. Harvard University Biostatistics Working Paper Series 123. Available at:  http://www.bepress.com/harvardbiostat/paper123/  . Accessed September 27, 2012.


- 20\. Fan J., Li R.: Variable selection via nonconcave penalized likelihood and its oracle properties. J Am Stat Assoc 2001; 96: pp. 1348-1360.


- 21\. Binder H., Porzelius C., Schumacher M.: An overview of techniques for linking high-dimensional molecular data to time-to-event endpoints by risk prediction models. Biometr J 2011; 53: pp. 170-189.


- 22\. Metz C., Goodenough D., Rossmann K.: Evaluation of receiver operating characteristic curve data in terms of information theory, with applications in radiography. Radiology 1973; 109: pp. 297-303.


- 23\. Dorfman D., Berbaum K., Metz C.: ROC rating analysis: generalization to the population of readers and cases with the jackknife method. Invest Radiol 1992; 27: pp. 1099.


- 24\. Jiang Y., Nishikawa R., Schmidt R., et. al.: Improving breast cancer diagnosis with computer-aided diagnosis. Acad Radiol 1999; 6: pp. 22-33.


- 25\. Kobayashi T., Xu X., MacMahon H., et. al.: Effect of a computer-aided diagnosis scheme on radiologists' performance in detection of lung nodules on radiographs. Radiology 1996; 199: pp. 843-848.


- 26\. Giger M., Doi K., MacMahon H., et. al.: Pulmonary nodules: computer-aided detection in digital chest images. Radiographics 1990; 10: pp. 41-51.


- 27\. Metz C.: Basic principles of ROC analysis. Semin Nucl Medicine 1978; 8: pp. 283-298.


- 28\. Metz C.: Some practical issues of experimental design and data analysis in radiological ROC studies. Invest Radiol 1989; 24: pp. 234-245.


- 29\. Metz C.: ROC methodology in radiologic imaging. Invest Radiol 1986; 21: pp. 720-733.


- 30\. Metz C., Herman B., Roe C.: Statistical comparison of two ROC-curve estimates obtained from partially-paired datasets. Med Decis Making 1998; 18: pp. 110-121.


- 31\. Metz C., Herman B., Shen J.: Maximum likelihood estimation of receiver operating characteristic (ROC) curves from continuously-distributed data. Stat Med 1998; 17: pp. 1033-1053.


- 32\. Wagner R., Beiden S., Metz C.: Continuous versus categorical data for ROC analysis: some quantitative considerations. Acad Radiol 2001; 8: pp. 328-334.


- 33\. Zou H.: The adaptive LASSO and its oracle properties. J Am Stat Assoc 2006; 101: pp. 1418-1429.


- 34\. McCullagh P., Nelder J.: Generalized Linear Models.1989.Chapman & Hall/CRCNew York


- 35\. Tibshirani R.: Regression shrinkage and selection via the LASSO. J R Stat Soc Ser B Stat Methodol 1996; pp. 267-288.


- 36\. Park M., Hastie T.: L1-regularization path algorithm for generalized linear models. J R Stat Soc Ser B Stat Methodol 2007; 69: pp. 659-677.


- 37\. Yuan M., Lin Y.: Model selection and estimation in regression with grouped variables. J R Stat Soc Ser B Stat Methodol 2006; 68: pp. 49-67.


- 38\. Yuan M., Joseph V., Zou H.: Structured variable selection and estimation. Ann Appl Stat 2009; 3: pp. 1738-1757.


- 39\. Efron B., Tibshirani R.: An Introduction to the Bootstrap, Vol 57.1993.Chapman & Hall/CRCNew York


- 40\. Swets J.A., Pickett R.M.: Evaluation of Diagnostic Systems: Methods From Signal Detection Theory.1982.Academic PressNew York


- 41\. Hanley H.A.: Receiver operating characteristic (ROC) methodology: the state of the art. Clin Rev Diagn Imaging 1989; 29: pp. 307-335.


- 42\. Begg C.B.: Advances in statistical methodology for diagnostic medicine in the 1980's. Stat Med 1991; 10: pp. 1887-1895.


- 43\. Samuelson F., Gallas B., Myers K., et. al.: The importance of ROC data. Acad Radiol 2011; 18: pp. 257.


- 44\. Zhao X., Dai W., Li Y., et. al.: AUC-based biomarker ensemble with an application on gene scores predicting low bone mineral density. Bioinformatics 2011; 27: pp. 3050-3055.


- 45\.  Vedovati M, Becattini C, Agnelli G, et al. Multidetector computed tomography for acute pulmonary embolism: embolic burden and clinical outcome. Chest. In press.


- 46\. Stein P., Matta F., Janjua M., et. al.: Outcome in stable patients with acute pulmonary embolism who had right ventricular enlargement and/or elevated levels of troponin I. Am J Cardiol 2010; 106: pp. 558-563.