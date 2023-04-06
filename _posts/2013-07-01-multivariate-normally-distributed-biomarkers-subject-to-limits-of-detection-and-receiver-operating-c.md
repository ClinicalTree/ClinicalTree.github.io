---
title: Multivariate Normally Distributed Biomarkers Subject to Limits of Detection and Receiver Operating Characteristic Curve Inference
author: [Neil J. Perkins PhD,Enrique F. Schisterman PhD,Albert Vexler PhD]
date: 2013-07-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 20, Issue 7 SOURCE CL_S_AcademicRadiologyVolume20Issue7 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Biomarkers are of ever-increasing importance to clinical practice and epidemiologic research. Multiple biomarkers are often measured per patient. Measurement of true biomarker levels is limited by laboratory precision, specifically measuring relatively low, or high, biomarker levels resulting in undetectable levels below, or above, a limit of detection (LOD). Ignoring these missing observations or replacing them with a constant are methods commonly used although they have been shown to lead to biased estimates of several parameters of interest, including the area under the receiver operating characteristic (ROC) curve and regression coefficients.

## Materials and Methods

We developed asymptotically consistent, efficient estimators, via maximum likelihood techniques, for the mean vector and covariance matrix of multivariate normally distributed biomarkers affected by LOD. We also developed an approximation for the Fisher information and covariance matrix for our maximum likelihood estimations (MLEs). We apply these results to an ROC curve setting, generating an MLE for the area under the curve for the best linear combination of multiple biomarkers and accompanying confidence interval.

## Results

Point and confidence interval estimates are scrutinized by simulation study, with bias and root mean square error and coverage probability, respectively, displaying behavior consistent with MLEs. An example using three polychlorinated biphenyls to classify women with and without endometriosis illustrates how the underlying distribution of multiple biomarkers with LOD can be assessed and display increased discriminatory ability over naïve methods.

## Conclusions

Properly addressing LODs can lead to optimal biomarker combinations with increased discriminatory ability that may have been ignored because of measurement obstacles.

The use of biomarkers, including medical images, is becoming increasingly common in the diagnosis and prognosis of individuals with a given disease in clinical settings and epidemiologic research. Combining various sources of biologic information quantitatively, through diagnostic indices for example, allows a concrete way to collapse blood, imaging, and other biomarker information. The receiver operating characteristic (ROC) curve is a tool frequently used to assess the usefulness of biomarkers as diagnostic tools . Some biomarkers, often emerging ones, are difficult to measure and/or are measured with less than optimally refined laboratory methods, making it difficult to assess any potential clinical usefulness. Specifically, limits of quantifiable biomarker levels are introduced by the sensitivity of the measurement instrument or process, which often leads to censored measurements at either the lower or upper end of the biomarker spectrum. The points at which this censoring occurs are called the limit of detection (LOD) and point of saturation, respectively . However, scientists remain interested in the biomarkers' potential relations, causations, and discriminatory ability for adverse outcomes and disease despite this measurement-induced error of censoring. For instance, polychlorinated biphenyl (PCB) levels are a group of compounds that have been linked with several adverse outcomes but their correlated nature and measurements being affected by LODs have hindered their study.

Consider _p_ biomarkers that are of interest in a particular population, where each individuals has true values for each, denoted by W−→=(W1,…,Wp)T
W

→

=

(

W

1

,

…

,

W

p

)

T
. Now suppose laboratory measurements, Z→
Z

→
, for each of those same biomarkers are affected by LODs d→=(d1,…,dp)T
d

→

=

(

d

1

,

…

,

d

p

)

T
. One way to write this component-wise transformation of W−→
W

→
is

Zl={Wl;Wl≥dl.;Wl<dl,
Z

l

=

{

W

l

;

W

l

≥

d

l

.

;

W

l

<

d

l

,


where for a fixed _d__l_ , _l_ = 1, … , _p_ , the _l_ th biomarker level is either quantified above _d__l_ or censored below _d__l_ . Clearly, estimating the underlying distribution or parameters and testing hypothesis intended for W−→
W

→
but using Z→
Z

→
, a mix of continuous and ordinal data, requires special consideration.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Left-Censored Multivariate Normal Likelihood

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Lk(μ→,Σ;Z→(1),Z→(2))∝g(1)(w→(1);μ→(1),Σ11)×Λ(2\|1)(d→(2);μ→(Q),ΣQ).
L

k

(

μ

→

,

Σ

;

Z

→

(

1

)

,

Z

→

(

2

)

)

∝

g

(

1

)

(

w

→

(

1

)

;

μ

→

(

1

)

,

Σ

11

)

×

Λ

(

2

\|

1

)

(

d

→

(

2

)

;

μ

→

(

Q

)

,

Σ

Q

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

L(μ→,Σ;Z)=∏nYj=1L(μ→,Σ;Z→j)∝∏Q→(Z→j)=(1,1,…,1)Tg(w→j;μ→,Σ)×⋯×∏Q→(Z→j)=(1,0,…,1,1,0)Tg(1)(w→(1)j;μ→(1),Σ11)×Λ(2\|1)(d→(2);μ→(Q),ΣQ)×⋯×∏Q→(Z→j)=(0,0,…,0,0)TΛ(d→;μ→,Σ)
L

(

μ

→

,

Σ

;

Z

)

=

∏

j

=

1

n

Y

L

(

μ

→

,

Σ

;

Z

→

j

)

∝

∏

Q

→

(

Z

→

j

)

=

(

1

,

1

,

…

,

1

)

T

g

(

w

→

j

;

μ

→

,

Σ

)

×

⋯

×

∏

Q

→

(

Z

→

j

)

=

(

1

,

0

,

…

,

1

,

1

,

0

)

T

g

(

1

)

(

w

→

j

(

1

)

;

μ

→

(

1

)

,

Σ

11

)

×

Λ

(

2

\|

1

)

(

d

→

(

2

)

;

μ

→

(

Q

)

,

Σ

Q

)

×

⋯

×

∏

Q

→

(

Z

→

j

)

=

(

0

,

0

,

…

,

0

,

0

)

T

Λ

(

d

→

;

μ

→

,

Σ

)


Maximizing Equation  1 with respect to each element of μ→
μ

→
and ∑
∑
results in MLEs μ→ˆ
μ

→

ˆ
and Σˆ
Σ

ˆ
. This must be performed numerically due to the complexity of the likelihood for which a closed-form solution does not exist for even the univariate case. The details of this development are found in the  Appendix .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ROC Curve and the AUC

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

β→T0∝(μ→X−μ→Y)T(ΣX+ΣY)−1,
β

→

0

T

∝

(

μ

→

X

−

μ

→

Y

)

T

(

Σ

X

+

Σ

Y

)

−

1

,


leading to


AUC0=P(U>V)=Φ((μ⇀X−μ⇀Y)T(ΣX+ΣY)−1(μ⇀X−μ⇀Y)−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−√),
A

U

C

0

=

P

(

U

>

V

)

=

Φ

(

(

μ

⇀

X

−

μ

⇀

Y

)

T

(

Σ

X

+

Σ

Y

)

−

1

(

μ

⇀

X

−

μ

⇀

Y

)

)

,


which is “best” with respect to maximizing AUC over all real β→T
β

→

T
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Relative bias and root mean square error of maximum likelihood estimates of various levels of AUC 0 (0.6 triangles, 0.8 squares) based on simulated multivariate normally distributed data. Censoring denotes limit of detection set at each quartile of the marginal distributions. Sample sizes 50, 100, and 200 correspond to increasing character size. AUC 0 is the area under the ROC curve for the best linear combination.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultivariateNormallyDistributedBiomarkersSubjecttoLimitsofDetectionandReceiverOperatingCharacteristicCurveInference/0_1s20S1076633213001724.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, QQ normal plots of the log transformed biomarker levels of polychlorinated biphenyls (PCBs) 180, 153, and 188 for women with endometriosis (cases) and without (controls). Horizontal points correspond to data below the limit of detection that are indistinguishable from each other.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultivariateNormallyDistributedBiomarkersSubjecttoLimitsofDetectionandReceiverOperatingCharacteristicCurveInference/1_1s20S1076633213001724.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

μ⇀ˆX=(−3.68,−1.81,−2.23)μ⇀ˆY=(−3.72,−1.89,−2.51)ΣˆX=⎡⎣⎢0.300.160.140.160.340.260.140.260.23⎤⎦⎥ΣˆY=⎡⎣⎢0.220.150.220.150.150.250.220.250.45⎤⎦⎥.
μ

⇀

ˆ

X

=

(

−

3.68

,

−

1.81

,

−

2.23

)

μ

⇀

ˆ

Y

=

(

−

3.72

,

−

1.89

,

−

2.51

)

Σ

ˆ

X

=

\[

0.30

0.16

0.14

0.16

0.34

0.26

0.14

0.26

0.23

\]

Σ

ˆ

Y

=

\[

0.22

0.15

0.22

0.15

0.15

0.25

0.22

0.25

0.45

\]

.


While these mean and covariance estimates are informative on their own, we substitute them into Equation 3 and get the BLC β→ˆT0=(0.164,−1.496,1.598)
β

→

ˆ

0

T

=

(

0.164

,

−

1.496

,

1.598

)
. We could now apply these coefficients and generate a parametric ROC curve for the BLC, which we compare to a similar curve for PCB 180 in  Figure 3 . It is obvious in  Figure 3 that the estimated BLC ROC curve (solid) is completely and substantially higher than that of estimated PCB 180 (dashed) and implies a potential increase in discrimination. We can quantify this using the AUˆC0
A

U

ˆ

C

0
by simply using Equation 4 to see what might be achieved using all three biomarkers jointly for separating women with and without endometriosis. Combining PCBs 188, 153, and 180 in this manner yields AUˆC0=0.731
A

U

ˆ

C

0

=

0.731
, an increase in estimated discriminatory ability from any single biomarker. Using Equations  A2 and A5 , we can also generate a 95% CI of 0.677 to 0.779. While these estimates show a potential benefit of using three biomarkers over one, ROC analysis is a process in which superiority of one biomarker over another for practical purposes needs to be validated with independent data before a recommendation can be made.

![Figure 3, Binormal parametric receiver operating characteristic curves for log polychlorinated biphenyl (PCB) 180 (dashed) and the best linear combination of log PCBs 180, 153, and 188.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultivariateNormallyDistributedBiomarkersSubjecttoLimitsofDetectionandReceiverOperatingCharacteristicCurveInference/2_1s20S1076633213001724.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## Multivariate Normal Likelihood with Left Censoring

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

g(W−→;μ→,Σ)=1(2π)p/2\|Σ\|1/2exp{−12(W−→−μ→)TΣ−1(W−→−μ→)},
g

(

W

→

;

μ

→

,

Σ

)

=

1

(

2

π

)

p

/

2

\|

Σ

\|

1

/

2

exp

{

−

1

2

(

W

→

−

μ

→

)

T

Σ

−

1

(

W

→

−

μ

→

)

}

,


where the covariance matrix ∑
∑
consists of variance, ∑ll=σll
∑

l

l

=

σ

l

l
, and covariance terms, Σll′=σll′
Σ

l

l

′

=

σ

l

l

′
, l≠l′
l

≠

l

′
. Again, suppose that biomarker measurements Z→
Z

→
are observed. The first part necessary for creating a likelihood function for a sample matrix **Z** with which we can estimate μ→
μ

→
and ∑
∑
is for those Z→
Z

→
with Q→(Z→)=(1,1,1,…,1)
Q

→

(

Z

→

)

=

(

1

,

1

,

1

,

…

,

1

)
, where the likelihood function is the standard result L(μ→,Σ;Z→)=L1(μ→,Σ;w1,w2…,wp)=g(w→;μ→,Σ)
L

(

μ

→

,

Σ

;

Z

→

)

=

L

1

(

μ

→

,

Σ

;

w

1

,

w

2

…

,

w

p

)

=

g

(

w

→

;

μ

→

,

Σ

)
. Second, we skip to the other extreme for those Z→
Z

→
with Q→(Z→)=(0,0,0,…,0)
Q

→

(

Z

→

)

=

(

0

,

0

,

0

,

…

,

0

)
, where the likelihood function corresponds to the probability


L(μ→,Σ;Z→)=L2p(μ→,Σ;w1<d1,w2<d2,…,wp<dp)=∫−∞d1∫−∞d2⋯∫−∞dpg(w→;μ→,Σ)dwp⋯dw2dw1=Λ(d→;μ→,Σ)
L

(

μ

→

,

Σ

;

Z

→

)

=

L

2

p

(

μ

→

,

Σ

;

w

1

<

d

1

,

w

2

<

d

2

,

…

,

w

p

<

d

p

)

=

∫

−

∞

d

1

∫

−

∞

d

2

⋯

∫

−

∞

d

p

g

(

w

→

;

μ

→

,

Σ

)

d

w

p

⋯

d

w

2

d

w

1

=

Λ

(

d

→

;

μ

→

,

Σ

)


Henceforth, Λ(d→;μ→,Σ)
Λ

(

d

→

;

μ

→

,

Σ

)
will denote the probability that all of an individual's biomarker levels are below the LODs for a given μ→
μ

→
and ∑
∑
. For the likelihoods of all the cases of Q→(Z→)
Q

→

(

Z

→

)
in between, Lk(μ→,Σ;Z→)
L

k

(

μ

→

,

Σ

;

Z

→

)
, _k_ = 2,3, … , 2 _p_ – 1 (ie, those Z→
Z

→
composed of both quantified and censored levels), we will extend ideas from explicit results for _P_ = 2 to the general _p_ case here . In that work, the bivariate normal case with Q→(Z→)=(1,0)
Q

→

(

Z

→

)

=

(

1

,

0

)
or (0,1) was shown to lead to a likelihood that is the product of a marginal distribution for the biomarker that is observed and a conditional distribution for the biomarker measured below the LOD. We will rely on the same rationale here but allow the observed and unobserved to be vectors of biomarkers with marginal and conditional distributions that can themselves be multivariate.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

CZ→=⎡⎣⎢⎢⎢⎢⎢⎢0001010000010000000100100⎤⎦⎥⎥⎥⎥⎥⎥⎛⎝⎜⎜⎜⎜⎜⎜.w2w3.w5⎞⎠⎟⎟⎟⎟⎟⎟=⎛⎝⎜⎜⎜⎜⎜⎜w2w3w5..⎞⎠⎟⎟⎟⎟⎟⎟=⎛⎝⎜Z→(1)Z→(2)⎞⎠⎟
C

Z

→

=

\[

0

1

0

0

0

0

0

1

0

0

0

0

0

0

1

1

0

0

0

0

0

0

0

1

0

\]

(

.

w

2

w

3

.

w

5

)

=

(

w

2

w

3

w

5

.

.

)

=

(

Z

→

(

1

)

Z

→

(

2

)

)


A consequence of this reordering is that CZ→∼Np(Cμ→,CΣCT)
C

Z

→

∼

N

p

(

C

μ

→

,

C

Σ

C

T

)
and that Cμ→=(μ→(1),μ→(2))T
C

μ

→

=

(

μ

→

(

1

)

,

μ

→

(

2

)

)

T
and CΣCT=\[Σ11Σ21Σ12Σ22\]
C

Σ

C

T

=

\[

Σ

11

Σ

12

Σ

21

Σ

22

\]
can be similarly partitioned, where Σab
Σ

ab
can be a matrix, vector, or scalar depending on the partition. The resultant multivariate normal density is then factored into a marginal density, g(1)(W−→(1);μ→(1),Σ11)
g

(

1

)

(

W

→

(

1

)

;

μ

→

(

1

)

,

Σ

11

)
, and a conditional density, g(2\|1)(W−→(2);μ→(Q),ΣQ)
g

(

2

\|

1

)

(

W

→

(

2

)

;

μ

→

(

Q

)

,

Σ

Q

)
, with μ→(Q)=μ→(2)+Σ21Σ−111(W−→(1)−μ→(1))
μ

→

(

Q

)

=

μ

→

(

2

)

+

Σ

21

Σ

11

−

1

(

W

→

(

1

)

−

μ

→

(

1

)

)
and ΣQ=Σ22−Σ21Σ−111Σ12
Σ

Q

=

Σ

22

−

Σ

21

Σ

11

−

1

Σ

12
. Since the observations in Z→(2)
Z

→

(

2

)
are unobserved but below the LODs, the likelihood for the _k_ th unique Q→(Z→)
Q

→

(

Z

→

)
, _k_ = 2,3, … , 2 _p_ – 1 is


Lk(μ→,Σ;Z→(1),Z→(2))∝g(1)(w→(1);μ→(1),Σ11)×∫−∞d→(2)g(2\|1)(w→(2);μ→(Q),ΣQ)dw→(2)=g(1)(w→(1);μ→(1),Σ11)×Λ(2\|1)(d→(2);μ→(Q),ΣQ)
L

k

(

μ

→

,

Σ

;

Z

→

(

1

)

,

Z

→

(

2

)

)

∝

g

(

1

)

(

w

→

(

1

)

;

μ

→

(

1

)

,

Σ

11

)

×

∫

−

∞

d

→

(

2

)

g

(

2

\|

1

)

(

w

→

(

2

)

;

μ

→

(

Q

)

,

Σ

Q

)

d

w

→

(

2

)

=

g

(

1

)

(

w

→

(

1

)

;

μ

→

(

1

)

,

Σ

11

)

×

Λ

(

2

\|

1

)

(

d

→

(

2

)

;

μ

→

(

Q

)

,

Σ

Q

)


Therefore, for a random sample **Z** of independent identically distributed _p_ -dimensional vectors Z→j
Z

→

j
, _j_ = 1, … , _n_ , following a multivariate normal distribution, the likelihood has the form


L(μ→,Σ;Z)=∏nYj=1L(μ→,Σ;Z→j)∝∏Q→(Z→j)=(1,1,…,1)Tg(w→j;μ→,Σ)×⋯×∏Q→(Z→j)=(1,0,…,1,1,0)Tg(1)(w→(1)j;μ→(1),Σ11)×Λ(2\|1)(d→(2);μ→(Q),ΣQ)×⋯×∏Q→(Z→j)=(0,0,…,0,0)TΛ(d→;μ→,Σ)
L

(

μ

→

,

Σ

;

Z

)

=

∏

j

=

1

n

Y

L

(

μ

→

,

Σ

;

Z

→

j

)

∝

∏

Q

→

(

Z

→

j

)

=

(

1

,

1

,

…

,

1

)

T

g

(

w

→

j

;

μ

→

,

Σ

)

×

⋯

×

∏

Q

→

(

Z

→

j

)

=

(

1

,

0

,

…

,

1

,

1

,

0

)

T

g

(

1

)

(

w

→

j

(

1

)

;

μ

→

(

1

)

,

Σ

11

)

×

Λ

(

2

\|

1

)

(

d

→

(

2

)

;

μ

→

(

Q

)

,

Σ

Q

)

×

⋯

×

∏

Q

→

(

Z

→

j

)

=

(

0

,

0

,

…

,

0

,

0

)

T

Λ

(

d

→

;

μ

→

,

Σ

)


Maximizing Equation  A1 with respect to each element of μ→
μ

→
and Σ
Σ
results in MLEs μ→ˆ
μ

→

ˆ
and Σˆ
Σ

ˆ
. This must be performed numerically due to the complexity of the likelihood for which a closed form solution does not exist for even the univariate case. Also of note is that for the explicit _P_ = 2 case, Equation  A1 reduces to the likelihood of Lyles et al . However, out of necessity, we maintain matrix notation rather than the explicit expansion displayed there.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Fisher Information Matrix

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Cov(θ→ˆ)=Cov(μ→ˆ,Σˆ)=\[I\]−1=⎡⎣⎢⎢⎢I1,1⋮Ip(p+1),1⋯⋱⋯I1,p(p+1)⋮Ip(p+1),p(p+1)⎤⎦⎥⎥⎥,
C

o

v

(

θ

→

ˆ

)

=

C

o

v

(

μ

→

ˆ

,

Σ

ˆ

)

=

\[

I

\]

−

1

=

\[

I

1

,

1

⋯

I

1

,

p

(

p

+

1

)

⋮

⋱

⋮

I

p

(

p

+

1

)

,

1

⋯

I

p

(

p

+

1

)

,

p

(

p

+

1

)

\]

,


where ( _P_ ≥ 2) and each Iab=limn→∞−1nE⎡⎣⎢∂2log(L(θ→;z→)∂θa∂θb⎤⎦⎥
I

a

b

=

lim

n

→

∞

−

1

n

E

\[

∂

2

log

(

L

(

θ

→

;

z

→

)

∂

θ

a

∂

θ

b

\]
. Please note that the rows and columns of Equation  A2 correspond to θ→=(μ→,Σ)T=(μ1,…,μp,σ11,σ12,…,σpp)T
θ

→

=

(

μ

→

,

Σ

)

T

=

(

μ

1

,

…

,

μ

p

,

σ

11

,

σ

12

,

…

,

σ

p

p

)

T
, a vector where the elements of **Σ** are listed out as a vector and concatenated with μ→
μ

→
. The development of the _I__ab_ , based on the partial derivatives of the log likelihood in Equation  A1 , was done with respect to the subvectors and matrices in μ→=(μ→(1),μ→(2))T
μ

→

=

(

μ

→

(

1

)

,

μ

→

(

2

)

)

T
and Σ=\[Σ11Σ21Σ12Σ22\]
Σ

=

\[

Σ

11

Σ

12

Σ

21

Σ

22

\]
in order to facilitate for the general _p_ dimensionality of our data. The expected values of elements _I__ab_ are explicitly evaluated where possible and are approximated otherwise.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimated AUC for a BLC with CI

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

β→T0∝(μ→X−μ→Y)T(ΣX+ΣY)(−1),
β

→

0

T

∝

(

μ

→

X

−

μ

→

Y

)

T

(

Σ

X

+

Σ

Y

)

(

−

1

)

,


leading to


AUC0=P(U>V)=Φ((μ→X−μ→Y)T(ΣX+ΣY)−1(μ⇀X−μ⇀Y)−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−√),
A

U

C

0

=

P

(

U

>

V

)

=

Φ

(

(

μ

→

X

−

μ

→

Y

)

T

(

Σ

X

+

Σ

Y

)

−

1

(

μ

⇀

X

−

μ

⇀

Y

)

)

,


which is “best” with respect to maximizing AUC over all real β→T
β

→

T
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σ2δ=λ−1(∂δ∂θ→X)T(Cov(θ→Xˆ))(∂δ∂θ→X)+(1−λ)−1(∂δ∂θ→Y)T(Cov(θ→Yˆ))(∂δ∂θ→Y),
σ

δ

2

=

λ

−

1

(

∂

δ

∂

θ

→

X

)

T

(

C

o

v

(

θ

→

X

ˆ

)

)

(

∂

δ

∂

θ

→

X

)

+

(

1

−

λ

)

−

1

(

∂

δ

∂

θ

→

Y

)

T

(

C

o

v

(

θ

→

Y

ˆ

)

)

(

∂

δ

∂

θ

→

Y

)

,


with θ→=(μ→,Σ)T
θ

→

=

(

μ

→

,

Σ

)

T
have the form described in Materials and Methods, and (∂δ∂θ→)ij=∂δ∂θ→ij
(

∂

δ

∂

θ

→

)

i

j

=

∂

δ

∂

θ

→

i

j
being the _ij__th_ element of (∂δ∂θ→)
(

∂

δ

∂

θ

→

)
, the partial derivative of δ with respect to the vectorized parameters. A 1 – _α_ level CI for AUˆC0
A

U

ˆ

C

0
can subsequently be calculated by Φ(δˆ±zα/2σ2δ√N√)
Φ

(

δ

ˆ

±

z

α

/

2

σ

δ

2

N

)
. Given μ→ˆX,μ→ˆY,ΣˆX
μ

→

ˆ

X

,

μ

→

ˆ

Y

,

Σ

ˆ

X
, and ΣˆY
Σ

ˆ

Y
based on **Z**_x_ and **Z**_Y_ , we use this technique to calculate an approximately 1 – _α_ level CI for AUˆC0
A

U

ˆ

C

0
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Metz C.E.: Basic principles of ROC analysis. Semin Nucl Med 1978; 8: pp. 283-298.


- 2\. Wagner R.F., Beiden S.V., Metz C.E.: Continuous versus categorical data for ROC analysis: some quantitative considerations. Acad Radiol 2001; 8: pp. 328-334.


- 3\. Pepe M.S.: The statistical evaluation of medical tests for classification and prediction.2003.Oxford University PressNew York


- 4\. Zhou X.H., Obuchowski N.A., McClish D.K.: Statistical methods in diagnostic medicine.2002.Wiley & Sons InterscienceNew York


- 5\. Browne R.W., Whitcomb B.W.: Procedures for determination of detection limits: application to high-performance liquid chromatography analysis of fat-soluble vitamins in human serum. Epidemiology 2010; 21: pp. S4-S9.


- 6\. Hornung R.W., Reed L.D.: Estimation of average concentration in the presence of nondetectable values. Appl Occup Environ Hyg 1990; 5: pp. 46-51.


- 7\. Haas C.H., Scheff P.A.: Estimation of averages in truncated samples. Environ Sci Technol 1990; 24: pp. 912-919.


- 8\. Lyles R.H., Williams J.K., Chuachoowong R.: Correlating two viral load assays with known detection limits. Biometrics 2001; 57: pp. 1238-1244.


- 9\. Schisterman E.F., Little R.J.: Opening the black box of biomarker measurement error. Epidemiology 2010; 21: pp. S1-S3.


- 10\. Singh A., Nocerino J.: Robust estimation of mean and variance using environmental data sets with below detection limit observations. Chemometr Intelligent Lab Syst 2002; 60: pp. 69-86.


- 11\. Perkins N.J., Schisterman E.F., Vexler A.: Receiver operating characteristic curve inference from a sample with a limit of detection. Am J Epidemiol 2007; 165: pp. 325-333.


- 12\. Gupta A.K.: Estimation of the mean and standard deviation of a normal population from a censored sample. Biometrika 1952; 39: pp. 260-273.


- 13\. Harter H.L., Moore A.H.: Asymptotic variances and covariances of maximum-likelihood estimators, from censored samples, of the parameters of Weibull and gamma populations. Ann Math Stat 1967; 38: pp. 557-570.


- 14\. Vexler A., Liu A., Eliseeva E., et. al.: Maximum likelihood ratio tests for comparing the discriminatory ability of biomarkers subject to limit of detection. Biometrics 2008; 64: pp. 895-903.


- 15\. Perkins N.J., Schisterman E.F., Vexler A.: ROC curve inference for best linear combination of two biomarkers subject to limits of detection. Biometr J 2011; 53: pp. 464-476.


- 16\. Su J.Q., Liu J.S.: Linear combinations of multiple diagnostic markers. J Am Stat Assoc 1993; 88: pp. 1350-1355.


- 17\. Reiser B., Faraggi D.: Confidence intervales for the generalized ROC criterion. Biometrics 1997; 53: pp. 192-202.


- 18\. Louis G., Weiner J.M., Whitcomb B.W., et. al.: Environmental PCB exposure and risk of endometriosis. Hum Reprod 2005; 20: pp. 279-285.


- 19\. Cooke P.S., Sato T., Buchanan D.L.: Disruption of steroid hormone signaling by PCBs.Robertson L.W.Hansen L.G.PCBs: recent advances in environmental toxicology and health effects.2001.The University Press of KentuckyLexington:pp. 257-263.


- 20\. Molodianovitch K., Faraggi D., Reiser B.: Comparing the areas under two correlated ROC curves: parametric and non-parametric approaches. Biometr J 2006; 48: pp. 745-757.


- 21\. Pesce L.L., Metz C.E., Berbaum K.S.: On the convexity of ROC curves estimated from radiological test results. Acad Radiol 2010; 17: pp. 960-968.


- 22\. Pesce L.L., Horsch K., Drukker K., et. al.: Semiparametric estimation of the relationship between ROC operating points and the test-result scale: application to the proper binormal model. Acad Radiol 2011; 18: pp. 1537-1548.


- 23\. Samuelson F., Gallas B.D., Myers K.J., et. al.: The importance of ROC data. Acad Radiol 2011; 18: pp. 257-258. author reply 259–261


- 24\. Alemayehu D., Zou K.H.: Applications of ROC analysis in medical research: recent developments and future directions. Acad Radiol 2012; 19: pp. 1457-1464.


- 25\. Hillis S.L., Metz C.E.: An analytic expression for the binormal partial area under the ROC curve. Acad Radiol 2012; 19: pp. 1491-1498.