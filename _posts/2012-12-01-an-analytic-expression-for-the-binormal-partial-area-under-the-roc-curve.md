---
title: An Analytic Expression for the Binormal Partial Area under the ROC Curve
author: [Stephen L. Hillis PhD,Charles E. Metz PhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 12 SOURCE CL_S_AcademicRadiologyVolume19Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The partial area under the receiver operating characteristic (ROC) curve (pAUC) is a useful summary measure for diagnostic studies. Unlike most summary measures that are functions of the ROC curve, researchers have not been aware of an analytic expression available for computing the pAUC for an ROC curve based on a latent binormal model. Instead, the pAUC has been computed using numerical integration or a rational polynomial approximation. Our purpose is to provide analytic expressions for the two forms of pAUC.

## Materials and Methods

We discuss the two fundamentally different types of pAUC. We present analytic expressions for both types, provide corresponding proofs, and illustrate their application with an example comparing the performances of spin echo and cine magnetic resonance imaging for detecting thoracic aortic dissection.

## Results

We provide an example of using the pAUC as the outcome in a multireader multicase analysis. We find that using the pAUC results in a more significant finding.

## Conclusions

We have provided analytic expressions for both types of pAUC, making it easier to compute the pAUCs corresponding to binormal ROC curves.

## Introduction

In diagnostic radiology, receiver operating characteristic (ROC) curves are commonly used to quantify the accuracy with which a reader (typically a radiologist) can discriminate between images from nondiseased (or normal) and diseased (or abnormal) cases. Although the ROC curve concisely describes the tradeoffs between sensitivity and specificity, typically accuracy is summarized by a summary index that is a function of the ROC curve. Commonly used summary indices include the area under the ROC curve (AUC), the partial area under the ROC curve (pAUC), sensitivity for a given specificity, and specificity for a given sensitivity. See Zou et al for a concise introduction to ROC analysis.

A common method for estimating the ROC curve is likelihood estimation under the assumption of a latent binormal model ; alternatively, a generalized linear model approach can also be used based on the binormal model assumption. Under the latent binormal model assumption the ROC curve can be described by two parameters. Except for the pAUC, analytic expressions have been routinely employed for expressing the indices previously mentioned as a function of the binormal ROC curve parameters. It is generally believed that the pAUC, assuming a latent binormal model, cannot be expressed as an analytic expression. For example, Pepe states: “Unfortunately, a simple analytic expression does not exist for the pAUC summary measure. It must be calculated using numerical integration or a rational polynomial approximation.” Similarly, Zhou et al state: “This partial area as it is known, is evaluated by numerical integration (McClish, 1989).” Although these methods can be programmed, having a simple expression for the pAUC would be much more convenient.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Two Different pAUCs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Partial areas under the receiver operating characteristic curve (pAUC). FPF, false-positive fraction; TPF, true-positive fraction.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnalyticExpressionfortheBinormalPartialAreaundertheROCCurve/0_1s20S1076633212004771.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Analytic Expressions for the pAUCs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Binormal model assumptions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results for pAUCFPF(0,FPF0)  pAUC    FPF    (    0    ,    FPF    0    )

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(0,FPF0)=FBVN(μ1+σ2√,Φ−1(FPF0);−1/1+σ2−−−−−√)
pAUC

FPF

(

0

,

FPF

0

)

=

F

BVN

(

μ

1

+

σ

2

,

Φ

−

1

(

FPF

0

)

;

−

1

/

1

+

σ

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(0,FPF0)=FBVN(a1+b2√,Φ−1(FPF0);−b/1+b2−−−−−√)
pAUC

FPF

(

0

,

FPF

0

)

=

F

BVN

(

a

1

+

b

2

,

Φ

−

1

(

FPF

0

)

;

−

b

/

1

+

b

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results for pAUCTPF(TPF0,1)  pAUC    TPF    (    TPF    0    ,    1    )

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCTPF(TPF0,1)=FBVN(μ1+σ2√,Φ−1(1−TPF0);−σ/1+σ2−−−−−√)
pAUC

TPF

(

TPF

0

,

1

)

=

F

BVN

(

μ

1

+

σ

2

,

Φ

−

1

(

1

−

TPF

0

)

;

−

σ

/

1

+

σ

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(TPF0,1)=FBVN(a1+b2√,Φ−1(1−TPF0);−1/1+b2−−−−−√)
pAUC

FPF

(

TPF

0

,

1

)

=

F

BVN

(

a

1

+

b

2

,

Φ

−

1

(

1

−

TPF

0

)

;

−

1

/

1

+

b

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimation and Inference for pAUC

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example Data Set

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Binormal receiver operating characteristic curve (ROC) curves for Van Dyke et al (20) data by reader. FPF, false-positive fractions; TPF, true-positive fractions.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnalyticExpressionfortheBinormalPartialAreaundertheROCCurve/1_1s20S1076633212004771.jpg)

Table 1


Binormal Parameter Estimates and Corresponding Summary Indices for Spin-Echo and Cine MRI Multireader Data


Modality Reader_a__b_ AUCpAUCFPF
pAUC

FPF
pAUCTPF
pAUC

TPF
(0,0.2) (0,0.1) (0.8,1) (0.9,1) Cine 1 1.7022 0.5368 0.93 (0.03) 0.82 (0.07) 0.77 (0.10) 0.69 (0.17) 0.49 (0.30) 2 1.4033 0.5607 0.89 (0.06) 0.73 (0.07) 0.66 (0.09) 0.52 (0.27) 0.31 (0.34) 3 1.7408 0.6346 0.93 (0.02) 0.79 (0.07) 0.73 (0.09) 0.68 (0.08) 0.51 (0.10) 4 1.9255 0.2015 0.97 (0.02) 0.95 (0.03) 0.94 (0.03) 0.85 (0.12) 0.70 (0.24) 5 1.0630 0.4635 0.83 (0.05) 0.66 (0.08) 0.60 (0.09) 0.32 (0.17) 0.12 (0.14) Spin echo 1 1.8501 0.5030 0.95 (0.02) 0.87 (0.04) 0.83 (0.05) 0.76 (0.12) 0.58 (0.21) 2 1.6552 0.4473 0.93 (0.02) 0.84 (0.05) 0.80 (0.06) 0.68 (0.10) 0.46 (0.14) 3 1.6220 0.4878 0.93 (0.03) 0.82 (0.06) 0.77 (0.07) 0.66 (0.15) 0.44 (0.23) 4 7.1233 0.8806 1.00 (0.00) 1.00 (0.00) 1.00 (0.00) 1.00 (0.00) 1.00 (0.00) 5 1.7329 0.4221 0.94 (0.03) 0.87 (0.05) 0.84 (0.06) 0.73 (0.13) 0.52 (0.22)

pAUCFPF
pAUC

FPF
, area under the ROC curve within the stated false-positive fraction interval; pAUCTPF
pAUC

TPF
, area to the right of the ROC curve within the stated TPF interval; ROC, receiver operating characteristic.


pAUCs have been normalized by dividing by the length of the defining interval. Standard errors, computed using the jackknife, are shown in parentheses.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


ROC Summary Measure Estimates for Spin-Echo and CINE MRI Data Assuming a Latent Binormal Model


Type of Estimator Specific Estimator Estimates_P_ Value Cine Spin-echo AUC AUC 0.911 0.952 .1413pAUCFPF
pAUC

FPF
pAUCFPF(0.0,0.2)
pAUC

FPF

(

0.0

,

0.2

)
0.790 0.880 .0600pAUCFPF(0.0,0.1)
pAUC

FPF

(

0.0

,

0.1

)
0.740 0.848 .0399pAUCFPF(0.0,0.05)
pAUC

FPF

(

0.0

,

0.05

)
0.691 0.817 .0278 Sens at fixed spec Sens (spec = 0.80) 0.863 0.925 .1265 Sens (spec = 0.90) 0.811 0.894 .0778 Sens (spec = 0.95) 0.760 0.862 .0491pAUCTPF
pAUC

TPF
pAUCTPF(0.8,1.0)
pAUC

TPF

(

0.8

,

1.0

)
0.613 0.765 .1426pAUCTPF(0.9,1.0)
pAUC

TPF

(

0.9

,

1.0

)
0.427 0.599 .1534pAUCTPF(0.95,1.0)
pAUC

TPF

(

0.95

,

1.0

)
0.251 0.430 .2277

AUC, area under the ROC curve; pAUCFPF
pAUC

FPF
, area under the ROC curve within the stated false-positive fraction interval; pAUCTPF
pAUC

TPF
, area to the right of the ROC curve within the stated TPF interval; ROC, receiver operating characteristic; sens at fixed spec, sensitivity for the stated specificity; spec, specificity.


_P_ value is for H  0  : the pAUC means are equal for cine and spin-echo magnetic resonance imaging.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A

## Derivation of Equations  1–4  in Results for the pAUCFPF(0,FPF0)  pAUC    FPF    (    0    ,    FPF    0    )   Section

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A1

## Derivation of pAUCFPF(0,FPF0)  pAUC    FPF    (    0    ,    FPF    0    )   Results (Eq  1 and 2  )

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUC(0,FPF0)=Pr\[Y>X,X>S−1X(FPF0)\]
pAUC

(

0

,

FPF

0

)

=

Pr

\[

Y

>

X

,

X

>

S

X

−

1

(

FPF

0

)

\]


where SX
S

X
, defined by SX(x)=Pr(X>x)
S

X

(

x

)

=

Pr

(

X

>

x

)
, is the complement of the cumulative distribution function of _X_ . This is a general result that holds even if the conditional distributions are not normal. Noting that S−1X(FPF0)=ξ0
S

X

−

1

(

FPF

0

)

=

ξ

0
, where FPF0=Pr(X>ξ0)
FPF

0

=

Pr

(

X

>

ξ

0

)
, it follows from Equation  A1 that


pAUCFPF(0,FPF0)=Pr\[Y−X>0,X>ξ0\]
pAUC

FPF

(

0

,

FPF

0

)

=

Pr

\[

Y

−

X

>

0

,

X

>

ξ

0

\]


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(0,FPF0)=Pr\[Y−X>0,X>ξ0\]=Pr\[Y−X−μ1+σ2√>−μ1+σ2√,X>ξ0\]=Pr\[Z>−μ1+σ2√,X>ξ0\]
pAUC

FPF

(

0

,

FPF

0

)

=

Pr

\[

Y

−

X

>

0

,

X

>

ξ

0

\]

=

Pr

\[

Y

−

X

−

μ

1

+

σ

2

>

−

μ

1

+

σ

2

,

X

>

ξ

0

\]

=

Pr

\[

Z

>

−

μ

1

+

σ

2

,

X

>

ξ

0

\]


where Z=(Y−X−μ)/1+σ2−−−−−√
Z

=

(

Y

−

X

−

μ

)

/

1

+

σ

2
. It is easy to show that Z∼N(0,1)
Z

∼

N

(

0

,

1

)
and corr(Z,X)=−1/1+σ2−−−−−√
corr

(

Z

,

X

)

=

−

1

/

1

+

σ

2
. To show the correlation result, note that _X_ and _Y_ are independent and that corr(Z,X)=cov(Z,X)
corr

(

Z

,

X

)

=

cov

(

Z

,

X

)
because both _Z_ and _X_ have unit standard deviation. Thus corr(Z,W)=cov(Z,W)=(1+σ2−−−−−√)−1cov(Y−X,X)=(1+σ2−−−−−√)−1cov(−X,X)=−(1+σ2−−−−−√)−1var(X)=−(1+σ2−−−−−√)−1
corr

(

Z

,

W

)

=

cov

(

Z

,

W

)

=

(

1

+

σ

2

)

−

1

cov

(

Y

−

X

,

X

)

=

(

1

+

σ

2

)

−

1

cov

(

−

X

,

X

)

=

−

(

1

+

σ

2

)

−

1

var

(

X

)

=

−

(

1

+

σ

2

)

−

1
. It follows that (Z,X)
(

Z

,

X

)
has a standardized bivariate normal distribution with correlation −1/1+σ2−−−−−√
−

1

/

1

+

σ

2
. Thus


pAUCFPF(0,FPF0)=Pr\[Z>−μ1+σ2√,X>ξ0\]
pAUC

FPF

(

0

,

FPF

0

)

=

Pr

\[

Z

>

−

μ

1

+

σ

2

,

X

>

ξ

0

\]


where FBVN(z,x;ρ)
F

BVN

(

z

,

x

;

ρ

)
is the standardized bivariate normal distribution function with correlation _ρ_ as discussed in the Results for pAUCFPF(0,FPF0)
pAUC

FPF

(

0

,

FPF

0

)
section. Because FBVN(z,x;ρ)=Pr(Z<x,X<x)=Pr(Z>−z,X>−x)
F

BVN

(

z

,

x

;

ρ

)

=

Pr

(

Z

<

x

,

X

<

x

)

=

Pr

(

Z

>

−

z

,

X

>

−

x

)
, it follows from Equation  A4 that


pAUCFPF(0,FPF0)=FBVN(μ1+σ2√,−ξ0;−1/1+σ2−−−−−√)
pAUC

FPF

(

0

,

FPF

0

)

=

F

BVN

(

μ

1

+

σ

2

,

−

ξ

0

;

−

1

/

1

+

σ

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(0,FPF0)=FBVN(μ1+σ2√,Φ−1(FPF0);−1/1+σ2−−−−−√)
pAUC

FPF

(

0

,

FPF

0

)

=

F

BVN

(

μ

1

+

σ

2

,

Φ

−

1

(

FPF

0

)

;

−

1

/

1

+

σ

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(0,FPF0)=FBVN(a1+b2√,Φ−1(FPF0);−b/1+b2−−−−−√)
pAUC

FPF

(

0

,

FPF

0

)

=

F

BVN

(

a

1

+

b

2

,

Φ

−

1

(

FPF

0

)

;

−

b

/

1

+

b

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A2

## Derivation of pAUCTPF(TPF0,0)  p    A    U    C    TPF    (    TPF    0    ,    0    )   Results (Eq 3 and 4) in the Results for pAUCFPF(0,FPF0)  pAUC    FPF    (    0    ,    FPF    0    )   Section

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FPF′=1−TPF andTPF′=1−FPF
FPF

′

=

1

−

TPF and

TPF

′

=

1

−

FPF


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FPF′(ξ)=1−TPF(ξ)=1−Pr(Y≥ξ)=Pr(Y≤−ξ)=Pr(−Y≥ξ)TPF′(ξ)=1−FPF(ξ)=1−Pr(X≥ξ)=Pr(X≤−ξ)=Pr(−X≥ξ)
FPF

′

(

ξ

)

=

1

−

TPF

(

ξ

)

=

1

−

Pr

(

Y

≥

ξ

)

=

Pr

(

Y

≤

−

ξ

)

=

Pr

(

−

Y

≥

ξ

)

TPF

′

(

ξ

)

=

1

−

FPF

(

ξ

)

=

1

−

Pr

(

X

≥

ξ

)

=

Pr

(

X

≤

−

ξ

)

=

Pr

(

−

X

≥

ξ

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X′=−YandY′=−X
X

′

=

−

Y

and

Y

′

=

−

X


we have


FPF′(ξ)=Pr(X′≥ξ)and TPF′(ξ)=Pr(Y′≥ξ)
FPF

′

(

ξ

)

=

Pr

(

X

′

≥

ξ

)

and TPF

′

(

ξ

)

=

Pr

(

Y

′

≥

ξ

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X˜=X′+μσandY˜=Y′+μσ
X

˜

=

X

′

+

μ

σ

and

Y

˜

=

Y

′

+

μ

σ


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X˜∼N(0,1),Y˜∼N(μσ,1σ2)
X

˜

∼

N

(

0

,

1

)

,

Y

˜

∼

N

(

μ

σ

,

1

σ

2

)


and the standard binormal parameters for the (X˜,Y˜)
(

X

˜

,

Y

˜

)
binormal distribution are


a=μandb=σ
a

=

μ

and

b

=

σ


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(1−TPF0,0)=FBVN(μ1+σ2√,Φ−1(1−TPF0);−σ/1+σ2−−−−−√)
pAUC

FPF

(

1

−

TPF

0

,

0

)

=

F

BVN

(

μ

1

+

σ

2

,

Φ

−

1

(

1

−

TPF

0

)

;

−

σ

/

1

+

σ

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUCFPF(TPF0,0)=FBVN(a1+b2√,Φ−1(1−TPF0);−1/1+b2−−−−−√)
pAUC

FPF

(

TPF

0

,

0

)

=

F

BVN

(

a

1

+

b

2

,

Φ

−

1

(

1

−

TPF

0

)

;

−

1

/

1

+

b

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure A1, Receiver operating characteristic (ROC) curve and partial areas under the ROC curve (pAUC TPF (0.8, 1) shaded area in ROC space (a) and after transformation (b) to the coordinate system defined by FPF′ = 1 − TPF on the x-axis and TPF′ = 1 − FPF on the y-axis. In the original ROC space (a) the nondiseased and diseased decision variables X and Y define the ROC curve; in the transformed ROC space (b) the ROC curve is defined by nondiseased and diseased decision variables X′ = −Y and Y′ = −X, with the shaded area equal to pAUC FPF (0, 0.2).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnalyticExpressionfortheBinormalPartialAreaundertheROCCurve/2_1s20S1076633212004771.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Zou K.H., O'Malley A.J., Mauri L.: Receiver-operating characteristic analysis for evaluating diagnostic tests and predictive models. Circulation 2007; 115: pp. 654-657.


- 2\. Dorfman D.D., Alf E.: Maximum likelihood estimation of parameters of signal-detection theory and determination of confidence intervals—rating method data. J Math Psychol 1969; 6: pp. 487-496.


- 3\. Dorfman D.D.: RSCORE II.Swets J.A.Pickett R.M.Evaluation of diagnostic systems: methods from signal detection theory.1982.Academic PressSan Diego, CA:pp. 212-232.


- 4\. Dorfman D.D., Berbaum K.S.: Degeneracy and discrete receiver operating characteristic rating data. Acad Radiol 1995; 2: pp. 907-915.


- 5\. Metz C.E., Herman B.A., Shen J.H.: Maximum likelihood estimation of receiver operating characteristic (ROC) curves from continuously-distributed data. Stat Med 1998; 17: pp. 1033-1053.


- 6\. Pepe M.S.: An interpretation for the ROC curve and inference using GLM procedures. Biometrics 2000; 56: pp. 352-359.


- 7\. Alonzo T.A., Pepe M.S.: Distribution-free ROC analysis using binary regression techniques. Biostatistics 2002; 3: pp. 421-432.


- 8\. Pepe M.: The statistical evaluation of medical tests for classification and prediction.2003.Oxford University PressNew York


- 9\. Zhou X.-H., Obuchowski N.A., McClish D.K.: Statistical methods in diagnostic medicine.2011.WileyNew Jersey


- 10\. Pan X.C., Metz C.E.: The “proper” binormal model: parametric receiver operating characteristic curve estimation with degenerate data. Acad Radiol 1997; 4: pp. 380-389.


- 11\. Thompson M.L., Zucchini W.: On the statistical analysis of ROC curves. Stat Med 1989; 8: pp. 1277-1290.


- 12\. McClish D.K.: Analyzing a portion of the ROC curve. Med Decision Making 1989; 9: pp. 190-195.


- 13\. Jiang Y.L., Metz C.E., Nishikawa R.M.: A receiver operating: characteristic partial area index for highly sensitive diagnostic tests. Radiology 1996; 201: pp. 745-750.


- 14\. Walter S.D.: The partial area under the summary ROC curve. Stat Med 2005; 24: pp. 2025-2040.


- 15\. Obuchowski N.A., McClish D.K.: Sample size determination for diagnostic accuracy studies involving binormal ROC curve indices. Stat Med 1997; 16: pp. 1529-1542.


- 16\. Shao J., Dongsheng T.: The jackknife and bootstrap.1995.Springer-VerlagNew York


- 17\. Efron B., Tibshirani R.J.: An introduction to the bootstrap.1993.Chapman and HallNew York


- 18\. Dorfman D.D., Berbaum K.S., Metz C.E.: Receiver operating characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 19\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of the diagnostic accuracy for multiple diagnostic tests: an ANOVA approach with dependent observations. Commun Stat Simulation Comp 1995; 24: pp. 285-308.


- 20\.  Van Dyke CW, White RD, Obuchowski NA, et al. Cine MRI in the diagnosis of thoracic aortic dissection. 79th RSNA Meetings, Chicago, IL, November 28–December 3, 1993.


- 21\. Dorfman D.D., Berbaum K.S., Lenth R.V., et. al.: Monte Carlo validation of a multireader method for receiver operating characteristic discrete rating data: factorial experimental design. Acad Radiol 1998; 5: pp. 591-602.


- 22\. Hillis S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 23\. Hillis S.L.: A comparison of denominator degrees of freedom methods for multiple observer ROC analysis. Stat Med 2007; 26: pp. 596-619.


- 24\.  SAS for Windows, version 9.3, copyright (c) 2002–2010 by SAS Institute Inc., Cary, NC.


- 25\.  Hillis SL, Schartz KM, Berbaum KS. OR/DBM MRMC procedure for SAS 3.0 (computer software). Available for download from  http://perception.radiology.uiowa.edu  . Accessed December 29, 2011.


- 26\. Berbaum K.S., Schartz K.M., Hillis S.L.: OR/DBM MRMC (version 2.4) (computer software).2012.The University of IowaIowa City, IA Available from http://perception.radiology.uiowa.edu

- 27\. Hanley J.A.: Receiver operating characteristic (ROC) methodology—the state of the art. Crit Rev Diagnostic Imaging 1989; 29: pp. 307-335.


- 28\. Dodd L.E., Pepe M.S.: Partial AUC estimation and regression. Biometrics 2003; 59: pp. 614-623.