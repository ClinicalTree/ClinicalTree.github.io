---
title: Estimating the Area Under ROC Curve When the Fitted Binormal Curves Demonstrate Improper Shape
author: [CL_AT_AndriyIBosPhD,CL_AT_BenGuoMS,CL_AT_DavidGurScD]
date: 2017-02-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 24, Issue 2]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The “binormal” model is the most frequently used tool for parametric receiver operating characteristic (ROC) analysis. The binormal ROC curves can have “improper” (non-concave) shapes that are unrealistic in many practical applications, and several tools (eg, PROPROC) have been developed to address this problem. However, due to the general robustness of binormal ROCs, the improperness of the fitted curves might carry little consequence for inferences about _global_ summary indices, such as the area under the ROC curve (AUC). In this work, we investigate the effect of _severe_ improperness of fitted binormal ROC curves on the reliability of AUC estimates when the data arise from an actually proper curve.

## Materials and Methods

We designed theoretically proper ROC scenarios that induce _severely_ improper shape of fitted binormal curves in the presence of well-distributed empirical ROC points. The binormal curves were fitted using maximum likelihood approach. Using simulations, we estimated the frequency of severely improper fitted curves, bias of the estimated AUC, and coverage of 95% confidence intervals (CIs). In  Appendix S1 , we provide additional information on percentiles of the distribution of AUC estimates and bias when estimating partial AUCs. We also compared the results to a reference standard provided by empirical estimates obtained from continuous data.

## Results

We observed up to 96% of severely improper curves depending on the scenario in question. The bias in the binormal AUC estimates was very small and the coverage of the CIs was close to nominal, whereas the estimates of partial AUC were biased upward in the high specificity range and downward in the low specificity range. Compared to a non-parametric approach, the binormal model led to slightly more variable AUC estimates, but at the same time to CIs with more appropriate coverage.

## Conclusions

The improper shape of the fitted binormal curve, by itself, ie, in the presence of a sufficient number of well-distributed points, does not imply unreliable AUC-based inferences.

## Introduction

Assessing diagnostic performance is an important problem in many fields, particularly in the development of medical diagnostic systems, biomarkers, and predictive models. A basic concept in evaluating diagnostic performance is the accuracy of classification of subjects with a known binary true status (eg, “diseased”/“non-diseased”). Typically, diagnostic results are either binary (eg, “negative”/“positive” with respect to the “disease”) or have a form of an ordinal “rating” (eg, perceived likelihood of the presence of the “disease”). The most widely used methodology for assessing performance in this type of diagnostic tasks is the receiver operating characteristic (ROC) analysis .

The basic quantities in ROC analysis are “sensitivity” (or true positive fraction, _TPF_ ) and “specificity” (or complement of the false positive fraction, 1- _FPF_ ), which are defined as the probabilities of correct classification of diseased and non-diseased subjects into “positive” and “negative” groups, correspondingly. When diagnostic results are ordinal, classification into “positive” and “negative” groups is performed by comparing the diagnostic rating to a given threshold. The ROC curve describes pairs of “ _sensitivity_ ” (or _TPF_ ) and “ _1-specificity_ ” (or _FPF_ ) values, computed for all positive thresholds and is conventionally plotted in (FPF, TPF) coordinates . The ROC curve is a fundamental tool in ROC analysis, and it is used to determine various summary indices of diagnostic performance .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X∼N(0,1)andY∼N(ab,1b2)and
X

∼

N

(

0

,

1

)

and

Y

∼

N

(

a

b

,

1

b

2

)

and


ROC(fpf)=Φ(a+bΦ−1(fpf)),
R

O

C

(

f

p

f

)

=

Φ

(

a

+

b

Φ

−

1

(

f

p

f

)

)

,


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Binormal ROC curves with an AUC of 0.8 and different degrees of improperness (corresponding to “b” of 1, 0.53, and 0.3, respectively). AUC, area under the ROC curve; ROC, receiver operating characteristic.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstimatingtheAreaUnderROCCurveWhentheFittedBinormalCurvesDemonstrateImproperShape/0_1s20S1076633216303348.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

dROC(p)dp∣∣p=fpf=bexp\[12{(1−b)Φ−1(1−fpf)+a}×{(1+b)Φ−1(1−fpf)−a}\].
dROC

(

p

)

d

p

\|

p

=

f

p

f

=

b

e

x

p

\[

1

2

{

(

1

−

b

)

Φ

−

1

(

1

−

f

p

f

)

+

a

}

×

{

(

1

+

b

)

Φ

−

1

(

1

−

f

p

f

)

−

a

}

\]

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X∼GAM(1,κ)andY∼GAM(β,κ)
X

∼

G

A

M

(

1

,

κ

)

and

Y

∼

G

A

M

(

β

,

κ

)


ROC(fpf)=1−Gκ{1βG−1κ(1−fpf)}
R

O

C

(

f

p

f

)

=

1

−

G

κ

{

1

β

G

κ

−

1

(

1

−

f

p

f

)

}


AUC=1−HF(2κ,2κ)(1β)
A

U

C

=

1

−

H

F

(

2

κ

,

2

κ

)

(

1

β

)


where _H  F(u,v)_ is the cumulative density function (c.d.f.) for the F-distribution with degrees of freedom _u_ and _v_ , and G  κ is the c.d.f. for gamma distribution with scale parameter “1” and shape parameter κ. Similar to the binormal model, the bigamma ROC curves can be conveniently parameterized in terms of AUC and the shape parameter κ.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Bigamma ROC curves with an AUC of 0.8 and different magnitudes of initial slope (corresponding to κ of 1, 0.33, and 0.1). AUC, area under the ROC curve; ROC, receiver operating characteristic.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstimatingtheAreaUnderROCCurveWhentheFittedBinormalCurvesDemonstrateImproperShape/1_1s20S1076633216303348.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

rˆ=aˆ1−bˆ
r

^

=

a

^

1

−

b

^


with \| _r_ \| ≤ 2 indicating a “noticeably improper” ROC curve. Although “noticeable improperness” of the fitted ROC curves is likely to affect at least some inferences under the binormal model, we believe its impact on the statistical inference depends on the summary index of interest, and in the presence of well-distributed empirical ROC points may have little impact on estimating overall indices, such as the AUC.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X∼χ2(1,θ)andY∼λ×χ2(1,λθ)
X

∼

χ

2

(

1

,

θ

)

and

Y

∼

λ

×

χ

2

(

1

,

λ

θ

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Frequency of Scenarios Resulting in “Noticeably Improper” (\| _r_ \| < 2) Fitted ROC for the 10,000 Bigamma Datasets Generated for Each Scenario


Sample Size Number of Categories True AUC κ = 0.1  (Highly Non-binormal) κ = 0.33  κ = 3  (Binormal-like) 100:100 10 0.6 0.82 0.59 0.29 0.7 0.90 0.65 0.10 0.8 0.90 0.65 0.02 0.9 0.80 0.61 0.03 50:50 10 0.6 0.73 0.58 0.41 0.7 0.82 0.61 0.18 0.8 0.81 0.61 0.09 0.9 0.74 0.59 0.08 100:100 5 0.6 0.82 0.60 0.32 0.7 0.95 0.74 0.13 0.8 0.96 0.79 0.07 0.9 0.93 0.99 0.11 50:50 5 0.6 0.75 0.61 0.45 0.7 0.87 0.68 0.22 0.8 0.90 0.72 0.16 0.9 0.78 0.94 0.30

AUC, area under the ROC curve; ROC, receiver operating characteristic.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Average of Binormal AUC and Monte Carlo Standard Deviation (STD) for Both Binormal and Empirical AUCs Based on 10,000 Datasets Generated for Each Scenario


Sample Size Number of Categories True AUC κ = 0.1  (Highly Non-binormal) κ = 0.33  κ = 3  (Binormal-like) Monte Carlo Estimates for AUC for the Fitted Binormal ROC STD of Empirical AUC  \\*  for Continuous Data Monte Carlo Estimates for AUC for the Fitted Binormal ROC STD of Empirical AUC  \\*  for Continuous Data Monte Carlo Estimates for AUC for the Fitted Binormal ROC STD of Empirical AUC  \\*  for Continuous Data AUC STD AUC STD AUC STD 100:100 10 0.6 0.61 0.040 0.040 0.61 0.042 0.040 0.61 0.044 0.040 0.7 0.71 0.036 0.037 0.70 0.036 0.037 0.70 0.038 0.037 0.8 0.81 0.032 0.032 0.80 0.032 0.032 0.80 0.032 0.031 0.9 0.89 0.029 0.025 0.89 0.028 0.024 0.90 0.024 0.022 50:50 10 0.6 0.61 0.055 0.056 0.61 0.058 0.057 0.61 0.060 0.056 0.7 0.71 0.051 0.053 0.71 0.052 0.052 0.70 0.053 0.052 0.8 0.81 0.045 0.046 0.80 0.046 0.045 0.80 0.045 0.044 0.9 0.89 0.041 0.035 0.89 0.039 0.033 0.90 0.034 0.031 100:100 5 0.6 0.60 0.041 0.040 0.60 0.041 0.040 0.60 0.041 0.040 0.7 0.70 0.039 0.037 0.70 0.039 0.037 0.70 0.039 0.037 0.8 0.79 0.038 0.032 0.79 0.037 0.032 0.80 0.035 0.031 0.9 0.87 0.040 0.025 0.85 0.039 0.024 0.89 0.033 0.022 50:50 5 0.6 0.60 0.058 0.056 0.60 0.059 0.057 0.60 0.058 0.056 0.7 0.70 0.055 0.053 0.70 0.056 0.052 0.70 0.056 0.052 0.8 0.79 0.055 0.046 0.79 0.053 0.045 0.80 0.050 0.044 0.9 0.89 0.058 0.035 0.85 0.056 0.033 0.88 0.050 0.031

AUC, area under the ROC curve; ROC, receiver operating characteristic.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Estimated Coverage of the 95% CIs Based on Binormal and Empirical AUC, and the Relative Bias of the Estimated Variance of the Binormal AUC for the10,000 Bigamma Datasets Generated for Each Scenario


Sample Size Number of Categories True Bigamma AUC κ = 0.1 (Highly Non-binormal) κ = 0.33 κ = 3 (Binormal-like) Relative Bias of the Estimated Variance Estimated Coverage of a Binormal 95% CI # Estimated Coverage of a Non-parametric 95% CI for Continuous Data Relative Bias of the Estimated Variance Estimated Coverage of a Binormal 95% CI # Estimated Coverage of a Non-parametric 95% CI for Continuous Data Relative Bias of the Estimated Variance Estimated Coverage of a Binormal 95% CI # Estimated Coverage of a Non-parametric 95% CI for Continuous Data 100:100 10 0.6 0.00 94.7% 10,000 94.9% −0.09 94.1% 10,000 94.9% −0.14 94.2% 10,000 94.8% 0.7 0.08 95.5% 10,000 94.9% 0.05 96.1% 10,000 94.8% −0.02 95.6% 10,000 94.3% 0.8 0.10 96.0% 10,000 94.2% 0.05 96.3% 10,000 94.6% −0.04 95.6% 9996 94.6% 0.9 0.00 96.2% 9998 93.8% 0.01 96.2% 10,000 93.4% 0.49 95.6% 9981 93.6% 50:50 10 0.6 0.03 95.1% 10,000 94.8% −0.06 94.6% 10,000 94.4% −0.09 94.8% 9999 94.9% 0.7 0.07 95.3% 10,000 94.6% 0.01 95.1% 10,000 94.4% −0.02 95.0% 10,000 94.6% 0.8 0.08 94.9% 10,000 93.7% 0.03 95.2% 10,000 93.8% 0.00 94.9% 9998 93.4% 0.9 0.07 94.8% 9869 91.8% 0.05 95.4% 9948 91.7% 0.09 94.8% 9992 92.2% 100:100 5 0.6 0.02 97.1% 10,000 94.9% 0.00 96.9% 10,000 94.9% 0.00 96.8% 10,000 94.8% 0.7 0.03 97.1% 10,000 94.9% 0.04 97.5% 10,000 94.8% −0.01 97.0% 10,000 94.3% 0.8 0.02 97.8% 9993 94.2% 0.01 97.6% 10,000 94.6% 0.01 96.9% 10,000 94.6% 0.9 153.69 99.7% 8994 93.8% 89.56 100.0% 9167 93.4% 3.34 97.1% 9960 93.6% 50:50 5 0.6 0.02 96.9% 10,000 94.8% −0.01 96.5% 10,000 94.4% 0.01 96.9% 10,000 94.9% 0.7 0.03 97.1% 10,000 94.6% 0.00 96.7% 10,000 94.4% −0.03 96.3% 10,000 94.6% 0.8 0.13 96.7% 9957 93.7% 0.06 96.9% 9996 93.8% 0.02 96.4% 10,000 93.4% 0.9 129.61 98.2% 8368 91.8% 86.16 99.9% 9104 91.7% 18.33 96.5% 9820 92.2%

AUC, area under the ROC curve; CI, confidence interval; ROC, receiver operating characteristic.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Frequency of Scenarios Resulting in “Noticeably Improper” (\| _r_ \| < 2) Fitted ROC Curves, Binormal AUC (Est. Bias), Its Empirical Standard Deviation (Emp. Std), and Relative Bias of the Estimated AUC Variance (R.B. var) for the 10,000 Bi-Chi-Squared Datasets Generated for Each Scenario  \\*

True AUC of the Underlying Bi-chi-squared Curve θ = 0.1 (Somewhat Non-binormal) θ = 0.33 θ = 3 (Binormal-like) Proportion of Improper Fitted Binormal ROC Curves Proportion of Improper Fitted Binormal ROC Curves Proportion of Improper Fitted Binormal ROC Curves 0.6 0.44 0.39 0.24 0.7 0.42 0.34 0.18 0.8 0.24 0.08 0.00 0.9 0.11 0.01 0.00

Est. AUC Emp. Std. Est. AUC Emp. Std. Est. AUC Emp. Std. 0.6 0.60 0.014 0.60 0.013 0.60 0.013 0.7 0.71 0.012 0.70 0.012 0.70 0.012 0.8 0.80 0.010 0.80 0.010 0.80 0.011 0.9 0.90 0.008 0.90 0.008 0.90 0.008

R.B. Var Est. Cover. R.B. Var Est. Cover. R.B. var Est. Cover. 0.6 −0.13 94.0% −0.10 94.6% −0.09 95.1% 0.7 0.00 96.0% −0.01 96.0% −0.06 95.7% 0.8 0.03 96.5% 0.01 96.5% −0.12 96.2% 0.9 0.04 94.8% 0.03 95.6% −0.02 95.9%

AUC, area under the ROC curve; ROC, receiver operating characteristic.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The empirical ROC curve and fitted ROC curves for the data analyzed in the Example section (LR-binormal ROC curve is the proper-binormal ROC [16 21] ). ROC, receiver operating characteristic.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstimatingtheAreaUnderROCCurveWhentheFittedBinormalCurvesDemonstrateImproperShape/2_1s20S1076633216303348.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


The Empirical AUC and the Areas Under the Fitted ROC Curve for the Data Analyzed in the Example Section


Type AUC Standard Deviation (STD) of the estimated AUC 95% Confidence Interval Lower Limit Upper Limit Empirical 0.77 0.032 0.71 0.83 Binormal  \\*  0.78 0.032 0.71  \\*  0.85  \\*  LR-binormal  †  0.81 0.022 0.76 0.86

AUC, area under the ROC curve; CI, confidence interval; ROC, receiver operating characteristic.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

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

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Supplementary Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Appendix S1

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Egan J.P.: Signal detection theory and ROC analysis.1975.Academic PressNew York


- 2\. Pepe M.S.: The statistical evaluation of medical tests for classification and prediction.2004.Oxford University PressOxford, United Kingdom


- 3\. Zhou X.H., Obuchowski N.A., McClish D.K.: Statistical methods in diagnostic medicine.2nd ed.2011.John Wiley & Sons, Inc.New York


- 4\. Hajian-Tilaki K.O., Hanley J.A., Joseph L., et. al.: A comparison of parametric and nonparametric approaches to ROC analysis of quantitative diagnostic tests. Med Decis Making 1997; 17: pp. 94-102.


- 5\. Constantine K., Karson M., Tse S.K.: Estimation of P(Y<X) in the gamma case. Commun Stat B Simul Comput 1986; 15: pp. 365-388.


- 6\. DeLong E.R., DeLong D.M., Clarke-Pearson D.L.: Comparing the area under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-845.


- 7\. Obuchowski N.A., Lieber M.L.: Confidence intervals for the receiver operating characteristic area in studies with small samples. Acad Radiol 1998; 5: pp. 561-571.


- 8\. Dorfman D.D., Alf E.: Maximum likelihood estimation of parameters of signal detection theory and determination of confidence intervals – rating-method data. J Math Psychol 1969; 6: pp. 487-496.


- 9\. Hanley J.A.: The robustness of the “binormal” assumptions used in fitting ROC curves. Med Decis Making 1988; 8: pp. 197-203.


- 10\. Walsh S.J.: Limitations to the robustness of binormal ROC curves: effects of model misspecification and location of decision threshold on bias, precision, size and power. Stat Med 1999; 16: pp. 669-679.


- 11\. Gönen M.: Analyzing receiver operating characteristic curves with SAS®.2007.SAS InstituteCary, NC


- 12\. Obuchowski N.A., McClish D.K.: Sample size determination for diagnostic accuracy studies involving binormal ROC curve indices. Stat Med 1997; 16: pp. 1529-1542.


- 13\. Hintze J.: PASS 12. Kaysville, UT: NCSS, LLC \[computer software\]; Available at www.ncss.com Accessed November 12, 2016


- 14\. Fawcett T.: An introduction to ROC analysis. Pattern Recognit Lett 2006; 27: pp. 861-874.


- 15\. Wagner R.F., Metz C.E., Campbell G.: Assessment of medical imaging systems and computer aids: a tutorial review. Acad Radiol 2007; 14: pp. 723-748.


- 16\. Pan X., Metz C.E.: The “proper” binormal model: parametric receiver operating characteristic curve estimation with degenerate data. Acad Radiol 1997; 4: pp. 380-389.


- 17\.  Metz ROC software. University of Chicago \[computer software\]; Available at http://metz-roc.uchicago.edu/MetzROC/software Accessed November 12, 2016


- 18\. Dorfman D.D., Berbaum K.S., Metz C.E., et. al.: Proper receiver operating characteristic analysis: the bigamma model. Acad Radiol 1997; 4: pp. 138-149.


- 19\. Hillis S.L., Berbaum K.S.: Using the mean-to-sigma ratio as a measure of the improperness of binormal ROC curves. Acad Radiol 2011; 18: pp. 143-154.


- 20\. Huang Y., Pepe M.S.: A parametric ROC model-based approach for evaluating the predictiveness of continuous markers in case-control studies. Biometrics 2009; 65: pp. 1133-1144.


- 21\. Hillis S.L.: Equivalence of binormal likelihood-ratio and bi-chi-squared ROC curve models. Stat Med 2016; 35: pp. 2031-2057.


- 22\. Herron J.M., Bender T.M., Campbell W.L., et. al.: Effects of luminance and resolution on observer performance with chest radiographs. Radiology 2000; 215: pp. 169-174.


- 23\. Hillis S.L., Schartz K.M., Berbaum K.S.: OR/DBM MRMC for SAS (Version 3.0) \[computer software\]. Available at http://perception.radiology.uiowa.edu Accessed November 12, 2016


- 24\. McClish D.: Analyzing a portion of the ROC curve. Med Decis Making 1989; 9: pp. 190-195.


- 25\. Jiang Y., Metz C.E., Nishikawa R.M.: A receiver operating characteristic partial area index for highly sensitive diagnostic tests. Radiology 1996; 201: pp. 745-750.


- 26\. Ma H., Bandos A.I., Rockette H.E., et. al.: On use of partial area under the ROC curve for evaluation of diagnostic performance. Stat Med 2013; 32: pp. 3449-3458.


- 27\. Pisano E.D., Gatsonis C., Yaffe M., et. al.: Diagnostic performance of digital versus film mammography for breast-cancer screening. N Engl J Med 2005; 353: pp. 1773-1783.