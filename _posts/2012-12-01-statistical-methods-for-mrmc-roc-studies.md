---
title: Statistical Methods for MRMC ROC Studies
author: [Annie Skaron MSc,Kang Li PhD,Xiao-Hua Zhou PhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 12 SOURCE CL_S_AcademicRadiologyVolume19Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

In radiology, multireader, multicase (MRMC) receiver-operating characteristic studies are commonly used to evaluate the accuracy of diagnostic imaging systems. The special feature of an MRMC receiver-operating characteristic study requires that the same set of patients’ images be examined by the same set of doctors. One main difficulty of analyzing MRMC data is a complicated correlation structure. Four commonly used methods are available for dealing with this complicated correlation structure. The authors conducted an extensive simulation study to assess the performance of these methods in finite sample sizes. They summarize the relative strengths and weaknesses of these methods and make recommendations on the use of these methods.

## Materials and Methods

A comprehensive simulation study was conducted to assess finite-sample performance of these methods with continuous data. The use of these methods for magnetic resonance imaging to predict extracapsular extension of prostate gland tumors is also illustrated.

## Results

The results indicate that when test outcomes are continuous, all four methods perform well for estimating the difference in areas under the curves for two diagnostic tests. On the basis of these results, it seems that any of these approaches is appropriate for analyzing an MRMC data set with continuous or pseudocontinuous data.

## Conclusions

The Dorfman-Berbaum-Metz method is the most practical analysis method to implement in a wide variety of scenarios. Also, in MRMC studies, radiologists should be encouraged to use the entire rating scale rather than tending toward a binary “diseased” or “not diseased” decision.

Receiver-operating characteristic (ROC) analysis is commonly used to assess and compare the accuracy of diagnostic tests . In diagnostic radiology, the measured outcome of a test is often a numerical rating that quantifies the likelihood that a reader believes that an image indicates the presence of a particular condition.

An ROC curve shows how the true-positive and false-positive rates vary as the threshold for classifying an image as positive or negative changes . The area under the ROC curve (AUC) is commonly used as a summary measure to describe the accuracy of an imaging modality. Other ROC summary measures, such as sensitivity at a given specificity and partial AUC, can also be used, but here we consider mostly the full AUC.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Estimated AUC and 95% CIs of the Two Tests for the Prostate Cancer Data


Method Smooth (CI) Direct (CI) Smooth–Direct (CI)_F__P_ DBM 0.627 (0.550 to 0.703) 0.552 (0.482 to 0.622) 0.075 (−0.017 to 0.167) 3.395 .097 OR 0.627 (0.551 to 0.703) 0.552 (0.482 to 0.622) 0.075 (−0.017 to 0.166) 3.417 .105 MM 0.776 (0.705 to 0.870) 0.911 (0.870 to 0.941) −0.134 (−0.197 to −0.072) — — BWC (BCA) 0.627 0.552 0.075 (−0.022 to 0.174) — — BWC (percentile) 0.627 0.552 0.075 (−0.025 to 0.174) — —

AUC, area under the curve; BCA, bias-corrected and accelerated; BWC, Beiden-Wagner-Campbell; CI, confidence interval; DBM, Dorfman-Berbaum-Metz; OR, Obuchowski-Rockette; MM, marginal model.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Xijk=μt+Tit+Rj+Ckt+(TR)ij+(TC)ikt+(RC)jkt+ϵijkt,
X

i

j

k

=

μ

t

+

T

i

t

+

R

j

+

C

k

t

+

(

T

R

)

i

j

+

(

T

C

)

i

k

t

+

(

R

C

)

j

k

t

+

ϵ

i

j

k

t

,


where _t_ = _I_ ( _k_ \> _c_ 0 ) is the indicator of disease, μ _t_ is the population mean, _T__it_ is the fixed effect of test _i_ , _R__j_ is the random effect of reader _j_ , _C__kt_ is the random effect of subject _k_ , ( _TR_ ) _ij_ , ( _TC_ ) _ikt_ , and ( _RC_ ) _jkt_ are the corresponding two-way interactions, and ϵ _ijkt_ is the random error.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


AUC and Parameter Values for Continuous Test Outcomes


AUC Setting_A_ 1 _A_ 2  μ  1 _T_ 21  Normal random effects, interactions, and errors 1 0.702 0.702 0.75 0 2 0.702 0.892 0.75 1 3 0.856 0.856 1.5 0 4 0.856 0.962 1.5 1 Normal random effects and interactions, χ  2  errors 1 0.714 0.714 0.75 0 2 0.714 0.904 0.75 1 3 0.869 0.869 1.5 0 4 0.869 0.966 1.5 1 χ  2  random effects, interactions, and errors 1 0.714 0.714 0.2 0 2 0.714 0.899 0.2 1 3 0.869 0.869 0.9 0 4 0.869 0.951 0.9 1.25

AUC, area under the curve.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Variations of the analysis methods used

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation results

## Confidence Interval Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Ninety-five percent confidence interval coverage of the four methods.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalMethodsforMRMCROCStudies/0_1s20S1076633212004722.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## DBM and OR methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## SZ method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## BWC Bootstrap

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## Methods for the Analysis of MRMC Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## DBM Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Yijk=μ=Ti+Rj+Ck+(TR)ij+(TC)ik+(RC)jk+(TRC)ijk+ϵijk,
Y

i

j

k

=

μ

=

T

i

+

R

j

+

C

k

+

(

T

R

)

i

j

+

(

T

C

)

i

k

+

(

R

C

)

j

k

+

(

T

R

C

)

i

j

k

+

ϵ

i

j

k

,


where μ is the population mean, _T__i_ is the fixed effect of treatment _i_ , _R__j_ is the random effect of reader _j_ , and _C__k_ is the random effect of case _k_ . The terms in parentheses denote the corresponding interactions, and ϵ _ijk_ is the random error term. The random variables are assumed to be independent and normally distributed with mean zero and variances σ2R
σ

R

2
, σ2C
σ

C

2
, σ2TR
σ

T

R

2
, σ2TC
σ

T

C

2
, σ2RC
σ

R

C

2
, σ2TRC
σ

T

R

C

2
, and σ2ϵ
σ

ϵ

2
for _R__j_ , _C__k_ , ( _TR_ ) _ij_ , ( _TC_ ) _ik_ , ( _RC_ ) _jk_ , ( _TRC_ ) _ijk_ , and ϵ _ijk_ , respectively. The DBM method uses conventional ANOVA techniques based on pseudovalues to estimate treatment AUCs and test for a treatment effect.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FDBM=MS(T)MS(T)+MS(T×R)−MS(T×R×C).
F

DBM

=

MS

(

T

)

MS

(

T

)

+

MS

(

T

×

R

)

−

MS

(

T

×

R

×

C

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

dfDBM=\[MS(T×R)+MS(T×C)−MS(T×R×C)\]2MS(T×R)2/\[(I−1)(J−1)\]
d

f

DBM

=

\[

MS

(

T

×

R

)

+

MS

(

T

×

C

)

−

MS

(

T

×

R

×

C

)

\]

2

MS

(

T

×

R

)

2

/

\[

(

I

−

1

)

(

J

−

1

)

\]


is the denominator degrees of freedom proposed by Hillis . Equations for 95% confidence intervals for single-test mean accuracies, and the difference in a pair of test mean accuracies, are included in Skaron and Zhou .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## OR Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Aij=μ+Ti+Rj+(TR)ij+ϵij,
A

i

j

=

μ

+

T

i

+

R

j

+

(

T

R

)

i

j

+

ϵ

i

j

,


_i_ = 1,…, _I_ , _j_ = 1,…, _J_ , where _A__ij_ is the AUC (or other accuracy measure) for test _i_ and reader _j_ , _T__i_ is the fixed effect of test _i_ , _R__j_ is the random effect of reader _j_ , ( _TR_ ) _ij_ is the random treatment-by-reader interaction, and ϵ _ij_ is the error. The random effect _R__j_ and random interaction ( _TR_ ) _ij_ are assumed to be mutually independent normal random variables with means equal to zero and variances σ2R
σ

R

2
and σ2TR
σ

T

R

2
, respectively. Here σ2R
σ

R

2
represents the variation in reader ability and σ2TR
σ

T

R

2
the interaction between reader and imaging modality. The error term ϵ _ij_ is assumed to be normally distributed with mean zero and variance σ2ϵ
σ

ϵ

2
; σ2ϵ
σ

ϵ

2
represents both the variability due to the patient sample and the within-reader variation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Cov(ϵij,ϵi′j′′)=⎧⎩⎨⎪⎪Cov1Cov2Cov3i≠i′,j=j′i=i′,j≠j′i≠i′,j≠j′.
Cov

(

ϵ

i

j

,

ϵ

i

′

j

″

)

=

{

Cov

1

i

≠

i

′

,

j

=

j

′

Cov

2

i

=

i

′

,

j

≠

j

′

Cov

3

i

≠

i

′

,

j

≠

j

′

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FOR=MS(T)MS(T×R)+J(Cov2ˆ−Cov3ˆ),
F

O

R

=

M

S

(

T

)

M

S

(

T

×

R

)

+

J

(

Cov

2

ˆ

−

Cov

3

ˆ

)

,


where Cov2ˆ
Cov

2

ˆ
and Cov3ˆ
Cov

3

ˆ
are consistent estimators of Cov2 and Cov3. Cov2ˆ
Cov

2

ˆ
and Cov3ˆ
Cov

3

ˆ
can be obtained from the data. Conditional on the reader and treatment-by-reader effects, it follows from the ANOVA model (equation  A4 ) that Cov1, Cov2, and Cov3 are the same as the corresponding covariances of the AUC’s \[9\]. For example, Cov1 = cov(ϵ _ij_ , ϵ _i_ ′ _j_ ) = Cov( _A__ij_ , _A__i_ ′ _j_ R , _TR_ ). Thus, Cov2 and Cov3 can be estimated from the AUC estimates using any method that treats readers as fixed and cases as random. These estimates are used to calculate the modified _F_ statistic. DeLong et al described a nonparametric method for estimating the covariance between all pairs of reader-treatment AUC accuracy estimates that treats cases as random and readers as fixed. Obuchowski and Rockette suggested averaging all corresponding pairs of between-reader covariances obtained from DeLong et al’s method for estimates of Cov2 and Cov3 when nonparametric AUC estimates are used.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

df={E\[MS(T×R)\]+J(Cov2−Cov3)}2{E\[MS(T×R)\]}2/\[(I−1)(J−1)\],
d

f

=

{

E

\[

MS

(

T

×

R

)

\]

+

J

(

Cov

2

−

Cov

3

)

}

2

{

E

\[

MS

(

T

×

R

)

\]

}

2

/

\[

(

I

−

1

)

(

J

−

1

)

\]

,

which leads to less conservative inference than the originally proposed ( _I_ − 1)( _J_ − 1). In practice, estimates of Cov2 and Cov3 are used to obtain an estimate of _df_ .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Components of Variance Bootstrap Method (BWC)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Aijk=μ+Ti+Rj+Ck+(TR)ij+(TC)ik+(RC)jk+ϵijk,
A

i

j

k

=

μ

+

T

i

+

R

j

+

C

k

+

(

T

R

)

i

j

+

(

T

C

)

i

k

+

(

R

C

)

j

k

+

ϵ

i

j

k

,


where μ is the population mean, _T__i_ is the contribution of treatment _i_ to the overall AUC, _R__j_ is the random effect of reader _j_ , and _C__k_ is the random effect of case _k_ . The terms in parentheses denote the corresponding interactions, and ϵ _ijk_ is the random error term. The random variables are assumed to be independent with mean zero and variances σ2R
σ

R

2
, σ2C
σ

C

2
, σ2TR
σ

T

R

2
, σ2TC
σ

T

C

2
, σ2RC
σ

R

C

2
, and σ2ϵ
σ

ϵ

2
for _R__j_ , _C__k_ , ( _TR_ ) _ij_ , ( _TC_ ) _ik_ , ( _RC_ ) _jk_ , and ϵ _ijk_ , respectively. Using the BWC bootstrap method, it is not necessary to assume the random variables are normally distributed.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

var(ARC\|T−ARC\|T′)=2(σ2TR+σ2TC+σ2ϵ)
var

(

A

R

C

\|

T

−

A

R

C

\|

T

′

)

=

2

(

σ

T

R

2

+

σ

T

C

2

+

σ

ϵ

2

)


and obtain a bootstrap confidence interval for the difference in treatment accuracies using the BCA bootstrap . In a similar way, one can obtain a confidence interval for a single test accuracy. For each bootstrap sample, one would choose a random sample of _J_ readers and _K_ cases, and the bootstrap data set would be made up of the ratings for the same _K_ cases for each sampled reader as in the original data set in which readers rate the same set of cases.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Marginal Model Method (SZ)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Aijks=E(ϕijks∣∣Zi,Qj,V1k,V0s)=P(Xijs<Xijk∣∣Zi,Qj,V1k,V0s),
A

i

j

k

s

=

E

(

ϕ

i

j

k

s

\|

Z

i

,

Q

j

,

V

k

1

,

V

s

0

)

=

P

(

X

i

j

s

<

X

i

j

k

\|

Z

i

,

Q

j

,

V

k

1

,

V

s

0

)

,


where ϕ _ijks_ is the indicator that _X__ijs_ < _X__ijk_ . Then the marginal regression model for _A__ijks_ is given by


Aijks=g(βT1Zi+βT2Qj+βT3V0k+βT4V0s),
A

i

j

k

s

=

g

(

β

1

T

Z

i

+

β

2

T

Q

j

+

β

3

T

V

k

0

+

β

4

T

V

s

0

)

,


where β=(βT1,βT2,βT3,βT4)T
β

=

(

β

1

T

,

β

2

T

,

β

3

T

,

β

4

T

)

T
is the vector of regression parameters and _g_ (·) is a monotone link function. The data set used to fit the marginal model is {(ϕijks,Zi,Qj,V1k,V0s):i=1,…I;j=1,…J;s=1,…c0;k=c0+1,…K}
{

(

ϕ

i

j

k

s

,

Z

i

,

Q

j

,

V

k

1

,

V

s

0

)

:

i

=

1

,

…

I

;

j

=

1

,

…

J

;

s

=

1

,

…

c

0

;

k

=

c

0

+

1

,

…

K

}
. The authors obtained a consistent estimator for the AUC; the regression parameter estimate βˆ
β

ˆ
is the same as that from a generalized estimating equation with working independence. Standard errors for the marginal model cannot be obtained using classical methods, because the “observations” ϕ _ijks_ are not independent. Song and Zhou showed that the ϕ _ijks_ are “sparsely correlated” according to the definition given by Lumley and Hambett under three different assumptions about the correlation structure:


- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Song and Zhou obtained a consistent sandwich estimator of the variance of βˆ
β

ˆ
under each of these assumptions. To make use of the asymptotic normality, the number of nondiseased cases and the number of diseased cases need to be large under assumption 1. Under assumption 2, the number of readers must also be large, and under assumption 3, the number of tests and readers must also be large.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Zhou X.H., Obuchowski N.A., McClish D.K.: Statistical Methods in Diagnostic Medicine.2nd ed.2011.John WileyNew York


- 2\. Pesce L.L., Horsch K., Drukker K., Metz C.E.: Semiparametric estimation of the relationship between roc operating points and the test-result scale: application to the proper binormal model. Acad Radiol 2011; 18: pp. 1537-1548.


- 3\. Pesce L.L., Metz C.E., Berbaum K.S.: On the convexity of roc curves estimated from radiological test results. Acad Radiol 2010; 17: pp. 960-968.


- 4\. Dorfman D.D., Berbaum K.S., Metz C.E.: Receiver operating characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 5\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of diagnostic accuracy for multiple readers and multiple tests: an ANOVA approach with dependent observations. Comm Stat Sim Comput 1995; 24: pp. 285-308.


- 6\. Beiden S., Wagner R., Campbell G.: Components-of-variance models and multiple bootstrap experiments: an alternative method for random-effects, receiver operating characteristic analysis. Acad Radiol 2000; 7: pp. 341-349.


- 7\. Song X., Zhou X.-H.: A marginal model approach for analysis of multi-reader multi-test receiver operating characteristic (ROC) data. Biostatistics 2005; 6: pp. 303-312.


- 8\. Roe C., Metz C.E.: Variance-component modelling of receiver operating characteristic index estimates. Acad Radiol 1997; 4: pp. 587-600.


- 9\. DeLong E., DeLong D., Clarke-Pearson D.: Comparing the areas under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-845.


- 10\. Hillis S.L., Obuchowski N.A., Berbaum K.S.: Power estimation for multireader roc methods an updated and unified approach. Acad Radiol 2011; 18: pp. 129-142.


- 11\. Hillis S.: A comparison of denominator degrees of freedom methods for multiple observer roc analysis. Stat Med 2007; 26: pp. 596-619.


- 12\. Skaron A., Zhou X.: Statistical methods for MRMC ROC studies. University of Washington Biostatistics Working Paper Series.2012.University of WashingtonSeattle


- 13\. Hillis S.L., Obuchowski N.A., Schartz K.M., Berbaum K.S.: A comparison of the Dorfman-Berbaum-Metz and Obuchowski-Rockette methods for receiver operating characteristic (ROC) data. Stat Med 2005; 24: pp. 1579-1607.


- 14\. Hillis S., Berbaum K., Metz C.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader roc study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 15\. Efron B., Tibshirani R.J.: An Introduction to the Bootstrap.1993.Chapman & HallNew York


- 16\. Lumley T., Hamblett N.: Asymptotics for marginal generalized linear models with sparse correlations. University of Washington Biostatistics Working Paper Series, Paper 207.2003.University of WashingtonSeattle