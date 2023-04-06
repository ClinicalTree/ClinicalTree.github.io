---
title: Simulation of Unequal-Variance Binormal Multireader ROC Decision Data
author: [Stephen L. Hillis PhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 12 SOURCE CL_S_AcademicRadiologyVolume19Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Roe and Metz (RM) proposed a model for simulating multireader multicase (MRMC) data collected from a factorial study design in which readers read the same cases in all modalities. However, a major weakness of the RM model is that it generates data according to an equal-variance binormal model for each reader. This article extends the RM model by allowing the diseased and nondiseased decision-variable distributions to have unequal variances for each reader.

## Materials and Methods

I show how to modify the RM model so that it generates data according to an unequal-variance binormal model for each reader. In doing so, I preserve other important characteristics of the original simulation input values. The mean-to-sigma ratio, which describes the relationship between the means and variances of the diseased and nondiseased decision-variable distributions, is constrained to have a value that is representative of many data sets. This last point is illustrated with an example comparing the performances of spin echo and cine magnetic resonance imaging for detecting thoracic aortic dissection.

## Results

A simulation study is performed to assess the performance of the MRMC methods proposed by Dorfman, Berbaum, and Metz and by Obuchowski and Rockette using the proposed unequal variance extension of the RM model. The methods show either excellent or acceptable performance when there are at least five readers and at least 25 normal and 25 abnormal cases.

## Conclusions

The proposed extension of the RM simulation model generates data that are more similar to data collected from radiological studies.

## Introduction

Roe and Metz (RM) proposed a model for the purpose of simulating multireader (MRMC) data that emulate confidence-of-disease data collected from the typical factorial study design where each case (ie, patient) undergoes each of several diagnostic tests (or modalities) and the resulting images are interpreted once by each reader. Studies that have used this model have been published previously . To account for the MRMC study design, the RM model generates data according to an equal-variance binormal model for which the separation of the diseased and nondiseased decision-variable distributions varies across modality-reader combinations. However, it is generally recognized that for real data the decision variable distributions for diseased and nondiseased cases will often have different variances, with the diseased distribution typically having the larger variance . Thus this equal-variance assumption is an important limitation of the RM model. The purpose of this article is to extend the RM model by allowing the diseased and nondiseased decision-variable distributions to have unequal variances for each reader, while keeping intact other important characteristics of the original RM simulation structures.

## Materials and methods

## Original RM Model Formulation

Let Xijkt
X

i

j

k

t
denote the value of the RM-model decision variable for test _i_ , reader _j_ , case _k_ , and truth _t_ ( _t_ = − for a nondiseased case image, + for a diseased case image); ie, Xijkt
X

i

j

k

t
represents the reader’s degree of confidence that the image is abnormal. The RM decision model, using the notation of RM , is given by

Xijkt=μt+τit+Rij+Ckt+(τR)ijt+(τC)ikt+(RC)jkt+(τRC)ijkt+Eijkt
X

i

j

k

t

=

μ

t

+

τ

i

t

+

R

i

j

+

C

k

t

+

(

τ

R

)

i

j

t

+

(

τ

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

(

τ

R

C

)

i

j

k

t

+

E

i

j

k

t


Without loss of generality they set


μ−=0
μ

−

=

0


and


τi−=0for alli
τ

i

−

=

0

for all

i


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σ2ϵ=σ2τRC+σ2E
σ

ϵ

2

=

σ

τ

R

C

2

+

σ

E

2


In their simulations RM set σ2τRC=0
σ

τ

R

C

2

=

0
, which is equivalent to omitting (τRC)ijkt
(

τ

R

C

)

i

j

k

t
from Equation  1 , resulting in σ2ϵ
σ

ϵ

2
representing only the pure error in the model.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Creating the Unequal-Variance RM Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σ2=σ2C+σ2τC+σ2RC+σ2ϵ
σ

2

=

σ

C

2

+

σ

τ

C

2

+

σ

R

C

2

+

σ

ϵ

2


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σ2C(+)=1b2σ2C(−),σ2τC(+)=1b2σ2τC(−),σ2RC(+)=1b2σ2RC(−),σ2ϵ(+)=1b2σ2ϵ(−)
σ

C

(

+

)

2

=

1

b

2

σ

C

(

−

)

2

,

σ

τ

C

(

+

)

2

=

1

b

2

σ

τ

C

(

−

)

2

,

σ

R

C

(

+

)

2

=

1

b

2

σ

R

C

(

−

)

2

,

σ

ϵ

(

+

)

2

=

1

b

2

σ

ϵ

(

−

)

2


for some b>0
b

>

0
. In Equation  5 the value of truth state _t_ is in parentheses.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σ2\_=σ2C(−)+σ2τC(−)+σ2RC(−)+σ2ϵ(−)
σ

\_

2

=

σ

C

(

−

)

2

+

σ

τ

C

(

−

)

2

+

σ

R

C

(

−

)

2

+

σ

ϵ

(

−

)

2


and


σ2+=σ2C(+)+σ2τC(+)+σ2RC(+)+σ2ϵ(+)
σ

+

2

=

σ

C

(

+

)

2

+

σ

τ

C

(

+

)

2

+

σ

R

C

(

+

)

2

+

σ

ϵ

(

+

)

2


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

b=σ−σ+
b

=

σ

−

σ

+


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Selecting Inputs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Null Simulation Parameter Values Used by Roe and Metz


This table is reprinted and adapted with permission from Roe and Metz .


Structureμ+
μ

+
AUC Correlations Variance ComponentsρWR
ρ

WR
ρBR
ρ

BR
σ2C
σ

C

2
σ2τC
σ

τ

C

2
σ2RC
σ

R

C

2
σ2ϵ
σ

ϵ

2
σ2R
σ

R

2
σ2τR
σ

τ

R

2
HL 0.75 0.702 0.8 0.6 0.3 0.3 0.2 0.2 0.0055 0.0055 HL 1.50 0.856 0.8 0.6 0.3 0.3 0.2 0.2 0.0055 0.0055 HL 2.50 0.961 0.8 0.6 0.3 0.3 0.2 0.2 0.0055 0.0055 LL 0.75 0.702 0.4 0.2 0.1 0.1 0.2 0.6 0.0055 0.0055 LL 1.50 0.856 0.4 0.2 0.1 0.1 0.2 0.6 0.0055 0.0055 LL 2.50 0.961 0.4 0.2 0.1 0.1 0.2 0.6 0.0055 0.0055 HH 0.75 0.702 0.8 0.6 0.3 0.3 0.2 0.2 0.011 0.011 HH 1.50 0.856 0.8 0.6 0.3 0.3 0.2 0.2 0.030 0.030 HH 2.50 0.961 0.8 0.6 0.3 0.3 0.2 0.2 0.056 0.056 LH 0.75 0.702 0.4 0.2 0.1 0.1 0.2 0.6 0.011 0.011 LH 1.50 0.856 0.4 0.2 0.1 0.1 0.2 0.6 0.030 0.030 LH 2.50 0.961 0.4 0.2 0.1 0.1 0.2 0.6 0.056 0.056

AUC, area under the curve; HH, high data correlation, low reader variance; HL, high data correlation, low reader variance; LH, low data correlation, high reader variance; LL, low data correlation, low reader variance.


For these null simulations μ−=τi−=τi+=0
μ

−

=

τ

i

−

=

τ

i

+

=

0
for all _i_ . Thus μ+
μ

+
is the median separation of the normal and abnormal decision variable distributions across readers. This table contains slight corrections (eg, AUC = 0.961 instead of 0.962) from previous work so that AUC corresponds to μ+
μ

+
. In previous work , A _z_ is used instead of AUC. All other notation is the same as in previous work .


Table 2


Null Simulation Parameter Values for Unequal-Variance Roe and Metz Model Simulations with the Median Mean-to-Sigma Ratio Set to 4.5, Based on Values from Table 1


Structure AUCμ+
μ

+
_b_ Correlations Variance Components Normal Cases Abnormal CasesρWR
ρ

WR
ρBR
ρ

BR
σ2C(−)
σ

C

(

−

)

2
σ2τC(−)
σ

τ

C

(

−

)

2
σ2RC(−)
σ

R

C

(

−

)

2
σ2ϵ(−)
σ

ϵ

(

−

)

2
σ2C(+)
σ

C

(

+

)

2
σ2τC(+)
σ

τ

C

(

+

)

2
σ2RC(+)
σ

R

C

(

+

)

2
σ2ϵ(+)
σ

ϵ

(

+

)

2
σ2R
σ

R

2
σ2τR
σ

τ

R

2
r.025
r

.025
HL 0.702 0.821 0.846 0.8 0.6 0.3 0.3 0.2 0.2 0.42 0.42 0.28 0.28 0.0066 0.0066 2.76 HL 0.856 1.831 0.711 0.8 0.6 0.3 0.3 0.2 0.2 0.59 0.59 0.40 0.40 0.0082 0.0082 3.63 HL 0.961 3.661 0.551 0.8 0.6 0.3 0.3 0.2 0.2 0.99 0.99 0.66 0.66 0.0118 0.0118 3.98 LL 0.702 0.821 0.846 0.4 0.2 0.1 0.1 0.2 0.6 0.14 0.14 0.28 0.84 0.0066 0.0066 2.76 LL 0.856 1.831 0.711 0.4 0.2 0.1 0.1 0.2 0.6 0.20 0.20 0.40 1.19 0.0082 0.0082 3.63 LL 0.961 3.661 0.551 0.4 0.2 0.1 0.1 0.2 0.6 0.33 0.33 0.66 1.97 0.0118 0.0118 3.98 HH 0.702 0.821 0.846 0.8 0.6 0.3 0.3 0.2 0.2 0.42 0.42 0.28 0.28 0.0132 0.0132 2.03 HH 0.856 1.831 0.711 0.8 0.6 0.3 0.3 0.2 0.2 0.59 0.59 0.40 0.40 0.0447 0.0447 2.46 HH 0.961 3.661 0.551 0.8 0.6 0.3 0.3 0.2 0.2 0.99 0.99 0.66 0.66 0.1201 0.1201 2.83 LH 0.702 0.821 0.846 0.4 0.2 0.1 0.1 0.2 0.6 0.14 0.14 0.28 0.84 0.0132 0.0132 2.03 LH 0.856 1.831 0.711 0.4 0.2 0.1 0.1 0.2 0.6 0.20 0.20 0.40 1.19 0.0447 0.0447 2.46 LH 0.961 3.661 0.551 0.4 0.2 0.1 0.1 0.2 0.6 0.33 0.33 0.66 1.97 0.1201 0.1201 2.83

AUC, area under the curve; HH, high data correlation, low reader variance; HL, high data correlation, low reader variance; LH, low data correlation, high reader variance; LL, low data correlation, low reader variance.


For these null simulations μ−=τi−=τi+=0
μ

−

=

τ

i

−

=

τ

i

+

=

0
for all _i_ ; μ+
μ

+
is the median separation of the normal and abnormal decision variable distributions across readers; AUC is the median AUC across readers; the median mean-to-sigma ratio across readers for each test is given by r=μ+/(σ+−σ\_)
r

=

μ

+

/

(

σ

+

−

σ

\_

)
, where σ\_=σ2C(−)+σ2τC(−)+σ2RC(−)+σ2ϵ(−)−−−−−−−−−−−−−−−−−−−−−−−−√
σ

\_

=

σ

C

(

−

)

2

+

σ

τ

C

(

−

)

2

+

σ

R

C

(

−

)

2

+

σ

ϵ

(

−

)

2
and σ+=σ−/b
σ

+

=

σ

−

/

b
; variance components involving case for the abnormal cases were computed by multiplying the corresponding variance components for the normal cases by b−2
b

−

2
; more precise values of _b_ are 0.84566, 0.71082, and 0.55140; structure is defined as in  Table 1  ; r.025
r

.025
is the 2.5th percentile of the distribution of the mean-to-sigma ratio across readers.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example Illustrating Unequal-Variance Binormal Parameters

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Latent-Binormal Model Parameter Estimates for Van Dyke et al Data


Modality Readerμ2
μ

2
σ2
σ

2
_r_ Cine 1 3.17 1.86 3.67 2 2.50 1.78 3.19 3 2.74 1.58 4.76 4 9.56 4.96 2.41 5 2.29 2.16 1.98 Spin echo 1 3.68 1.99 3.72 2 3.70 2.24 2.99 3 3.32 2.05 3.17 4 6.93 1.21 33.19 5 4.11 2.37 3.00

The mean and standard deviation of the latent nondiseased decision-variable distribution are set to zero and one, respectively; μ2
μ

2
and σ2
σ

2
are the estimated mean and standard deviation for the latent diseased decision-variable distribution; r=μ2/(σ2−1)
r

=

μ

2

/

(

σ

2

−

1

)
is the estimated mean-to-sigma ratio.


![Figure 1, Binormal receiver operating characteristic curves for Van Dyke et al (17) data by reader. FPF, false-positive fraction; TPF, true-positive fraction.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SimulationofUnequalVarianceBinormalMultireaderROCDecisionData/0_1s20S1076633212004825.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Plots of trapezoid and semiparametric (latent binormal) AUC empirical type I error rates (alpha = 0.05) versus correlation-and-variance structure and sample size for testing the null hypothesis of equal modality AUCs. Case sample sizes are indicated by 25+/25−, 50+/50−, and 100+/100−, where “+” indicates a diseased case and “−” indicates a nondiseased case. AUC, area under the curve; HH, high data correlation, low reader variance; HL, high data correlation, low reader variance; LH, low data correlation, high reader variance; LL, low data correlation, low reader variance.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SimulationofUnequalVarianceBinormalMultireaderROCDecisionData/1_1s20S1076633212004825.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A

## Derivation of steps for selecting input values for the unequal-variance ROE and Metz model

## Notation and Results for the Unequal-Variance Roe and Metz Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X(kt)ij=Xijkt
X

i

j

(

k

t

)

=

X

i

j

k

t


For test _i_ and reader _j_ , the model can be written in the form


X(kt)ij=μ(ij)t+ϵ(ij)kt
X

i

j

(

k

t

)

=

μ

t

(

i

j

)

+

ϵ

k

t

(

i

j

)


where


μ(ij)t=μt+τit+Rjt+τRijt
μ

t

(

i

j

)

=

μ

t

+

τ

i

t

+

R

j

t

+

τ

R

i

j

t


and


ϵ(ij)kt=Ckt+(τC)ikt+(RC)jkt+τRCijkt+Eijkt
ϵ

k

t

(

i

j

)

=

C

k

t

+

(

τ

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

τ

R

C

i

j

k

t

+

E

i

j

k

t


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ϵ(ij)kt∼N(0,σ2t),t=−,+
ϵ

k

t

(

i

j

)

∼

N

(

0

,

σ

t

2

)

,

t

=

−

,

+


where


σ2−=σ2C(−)+σ2τC(−)+σ2RC(−)+σ2ϵ(−)
σ

−

2

=

σ

C

(

−

)

2

+

σ

τ

C

(

−

)

2

+

σ

R

C

(

−

)

2

+

σ

ϵ

(

−

)

2


σ2+=σ2−b2
σ

+

2

=

σ

−

2

b

2


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

μ(ij)+−μ(ij)−=μ++τi++Rj+−Rj−+τRij+−τRij−
μ

+

(

i

j

)

−

μ

−

(

i

j

)

=

μ

+

+

τ

i

+

+

R

j

+

−

R

j

−

+

τ

R

i

j

+

−

τ

R

i

j

−


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

μ(ij)+−μ(ij)−∼N(μ++τi+,2σ2R+2σ2τR)
μ

+

(

i

j

)

−

μ

−

(

i

j

)

∼

N

(

μ

+

+

τ

i

+

,

2

σ

R

2

+

2

σ

τ

R

2

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

E(μ(ij)+−μ(ij)−)=med(μ(ij)+−μ(ij)−)=μ++τi+
E

(

μ

+

(

i

j

)

−

μ

−

(

i

j

)

)

=

med

(

μ

+

(

i

j

)

−

μ

−

(

i

j

)

)

=

μ

+

+

τ

i

+


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

AUC=Φ(μ++τi+σ2−+σ2+√)
AUC

=

Φ

(

μ

+

+

τ

i

+

σ

−

2

+

σ

+

2

)


where denotes the standard normal cumulative distribution function.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Avoiding Visibly Improper Receiver Operating Characteristics Curves

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

r=μ2−μ1σ2−σ1
r

=

μ

2

−

μ

1

σ

2

−

σ

1


Equivalently,


r=a1−b
r

=

a

1

−

b


where _a_ and _b_ denote the usual parameters of the binormal model: a=(μ2−μ1)/σ2
a

=

(

μ

2

−

μ

1

)

/

σ

2
and b=σ1/σ2
b

=

σ

1

/

σ

2
. If σ1=σ2
σ

1

=

σ

2
I define r=∞
r

=

∞
if μ2>μ1
μ

2

>

μ

1
, r=−∞
r

=

−

∞
if μ2<μ1
μ

2

<

μ

1
, and _r_ to be undefined if μ2=μ1
μ

2

=

μ

1
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

r=ΔmΔσ
r

=

Δ

m

Δ

σ


The mean-to-sigma ratio was first introduced by Swets et al , who noticed that it seemed to be approximately constant for a variety of experiments. Some support for this conclusion was provided by later analyses . For example, Green and Swets note that r≈4
r

≈

4
describes the relationship between the latent means and standard deviations for many studies. Hillis and Berbaum classify the improperness of a binormal ROC curve as visibly indiscernible if \|r\|≥3
\|

r

\|

≥

3
, noticeable if \|r\|≤2
\|

r

\|

≤

2
, and slight if 2<\|r\|<3
2

<

\|

r

\|

<

3
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δm=−b˜+b˜2−4a˜c˜√2a˜
Δ

m

=

−

b

˜

+

b

˜

2

−

4

a

˜

c

˜

2

a

˜


and


b=rΔmσ1+r
b

=

r

Δ

m

σ

1

+

r


where


c=Φ−1(AUC),a˜=r2−c2,b˜=−2c2rσ21,c˜=−2c2r2σ21
c

=

Φ

−

1

(

AUC

)

,

a

˜

=

r

2

−

c

2

,

b

˜

=

−

2

c

2

r

σ

1

2

,

c

˜

=

−

2

c

2

r

2

σ

1

2


In the next section I derive the unequal-variance RM model parameters by first starting with the median AUC value and variance components for the nondiseased decision-variable distribution and then, setting r=4.5
r

=

4.5
, compute the corresponding values of Δm
Δ

m
and _b_ that will be used to generate the simulated data. To ensure that the latent ROC curves are rarely noticeably improper, I then verify that the 2.5th percentile of the mean-to-sigma ratio distribution exceeds 2.0, which implies that less that 2.5% of the latent mean-to-sigma ratios will be visually noticeable, using the Hillis and Berbaum classification.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Input Values for the Unequal-Variance Simulation Model

## Preliminaries

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

τ1+=0
τ

1

+

=

0


Under the constraints given by Equations  2, 3, and A13 , the null hypothesis of equal test AUCs is given by


H0:τ2+=0
H

0

:

τ

2

+

=

0


Under the null hypothesis, it follows from Equation  A7 that μ+
μ

+
is the separation between the normal and abnormal distributions for a typical reader (ie, μ+
μ

+
is the median separation across the reader population), with the corresponding median AUC given by Equation  A8 with τi+=0
τ

i

+

=

0
and σ2+replaced byσ2−
σ

+

2

replaced by

σ

−

2
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ρWR=σ2C+σ2τC+σ2RCσ2C+σ2τC+σ2RC+σ2ϵ
ρ

WR

=

σ

C

2

+

σ

τ

C

2

+

σ

R

C

2

σ

C

2

+

σ

τ

C

2

+

σ

R

C

2

+

σ

ϵ

2


and


ρBR=σ2C+σ2τCσ2C+σ2τC+σ2RC+σ2ϵ
ρ

BR

=

σ

C

2

+

σ

τ

C

2

σ

C

2

+

σ

τ

C

2

+

σ

R

C

2

+

σ

ϵ

2


The reader is referred to Roe and Metz for details about the correlations. Because these correlations are for the same case, allowing the variance components in Equations  A15 and A16 to depend on truth, as specified by Equation  5 , will not change the values of these two correlations. The “structure” label in  Table 1 describes combinations of values of the two correlations with reader and test-by-reader variance component values.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

{Φ\[μ+−1.962(σ2R+σ2τR)√2σ2−√\],Φ\[μ++1.962(σ2R+σ2τR)√2σ2−√\]}
{

Φ

\[

μ

+

−

1.96

2

(

σ

R

2

+

σ

τ

R

2

)

2

σ

−

2

\]

,

Φ

\[

μ

+

+

1.96

2

(

σ

R

2

+

σ

τ

R

2

)

2

σ

−

2

\]

}


where σ2−
σ

−

2
is given by Equation  A4 . From  Table 1 we see that Roe and Metz set σ2−=1
σ

−

2

=

1
and use σ2R+σ2τR=0.022
σ

R

2

+

σ

τ

R

2

=

0.022
, 0.060, and 0.112 for μ+=0.75
μ

+

=

0.75
, 1.50, and 2.50, respectively. It follows from Equation  A17 that 95% of the latent AUCs will fall between 0.87 and 0.99 for the high ( μ+=2.50
μ

+

=

2.50
, median AUC = 0.961) ROC curves, between 0.72 and 0.94 for the intermediate ( μ+=1.50
μ

+

=

1.50
, median AUC = 0.856) ROC curves, and between 0.59 and 0.79 for the low ( μ+=0.75
μ

+

=

0.75
, median AUC = 0.702) ROC curves. (I note that Roe and Metz report similar but slightly different ranges, but because they do not give the formula they used it is not possible to know if the slight differences are due to miscalculation or a slightly different formula.)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

{Φ\[μ+−1.962(σ2R+σ2τR)√σ2−+σ2+√\],Φ\[μ++1.962(σ2R+σ2τR)√σ2−+σ2+√\]}
{

Φ

\[

μ

+

−

1.96

2

(

σ

R

2

+

σ

τ

R

2

)

σ

−

2

+

σ

+

2

\]

,

Φ

\[

μ

+

+

1.96

2

(

σ

R

2

+

σ

τ

R

2

)

σ

−

2

+

σ

+

2

\]

}


which is equivalent to


{Φ\[μ+−1.962(σ2R+σ2τR)√σ2\_(1+b−2)√\],Φ\[μ++1.962(σ2R+σ2τR)√σ2−(1+b−2)√\]}
{

Φ

\[

μ

+

−

1.96

2

(

σ

R

2

+

σ

τ

R

2

)

σ

\_

2

(

1

+

b

−

2

)

\]

,

Φ

\[

μ

+

+

1.96

2

(

σ

R

2

+

σ

τ

R

2

)

σ

−

2

(

1

+

b

−

2

)

\]

}


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σ2R+σ2τR=.5\[μ+−Φ−1(lower bound)σ2−(1+b−2)√(1.96)\]2
σ

R

2

+

σ

τ

R

2

=

.5

\[

μ

+

−

Φ

−

1

(

lower bound

)

σ

−

2

(

1

+

b

−

2

)

(

1.96

)

\]

2


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Algorithm for computing input values

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


σ2R+σ2τR=.5\[μ+−Φ−1(lower limit)σ2−(1+b−2)√(1.96)\]2
σ

R

2

+

σ

τ

R

2

=

.5

\[

μ

+

−

Φ

−

1

(

lower limit

)

σ

−

2

(

1

+

b

−

2

)

(

1.96

)

\]

2


where “lower limit” is set equal to the lower interval limit defined by Equation  A17 for the RM model. Specifically, for “high reader variance” structures (second letter is “H”) lower limit is given by 0.59469, 0.71293, and 0.86689 for median AUC = 0.702, 0.856, and 0.961, respectively, and for “low reader variance” structures (second letter is “L”) lower limit given by 0.62732, 0.80375, and 0.94088 for median AUC = 0.702, 0.856, and 0.961, respectively. Values of μ+
μ

+
and _b_ were determined in step 2 and σ2−
σ

−

2
is given by Equation  A4 ; thus σ2−=1
σ

−

2

=

1
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Distribution intervals for mean-to-sigma ratio

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

rij=μ(ij)+−μ(ij)−σ+−σ−
r

i

j

=

μ

+

(

i

j

)

−

μ

−

(

i

j

)

σ

+

−

σ

−


where μ(ij)+
μ

+

(

i

j

)
and μ(ij)−
μ

−

(

i

j

)
are defined by Equation  A2 , μ(ij)+−μ(ij)−
μ

+

(

i

j

)

−

μ

−

(

i

j

)
is the latent separation between the diseased and nondiseased distributions, and σ+
σ

+
and σ−
σ

−
are defined by Equations  A4 and A5 . It follows from Equations  A6, A13, and A14 that for null simulations


rij∼N(μ+σ−(1/b−1),2σ2R+2σ2τRσ2−(1/b−1)2)
r

i

j

∼

N

(

μ

+

σ

−

(

1

/

b

−

1

)

,

2

σ

R

2

+

2

σ

τ

R

2

σ

−

2

(

1

/

b

−

1

)

2

)


and hence the 2.5th percentile for the mean-to-sigma ratio distribution is given by 2.5th pct(mean−to−sigma ratio)=μ+−1.962σ2R+2σ2τR√σ−(1/b−1)
2.5

th pct

(

mean

−

to

−

sigma ratio

)

=

μ

+

−

1.96

2

σ

R

2

+

2

σ

τ

R

2

σ

−

(

1

/

b

−

1

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Nonnull simulation values

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

AUC+d=Φ(μ++τ2+σ2−+σ2+√)
AUC

+

d

=

Φ

(

μ

+

+

τ

2

+

σ

−

2

+

σ

+

2

)


where σ−=σ2C(−)+σ2τC(−)+σ2RC(−)+σ2ϵ(−)−−−−−−−−−−−−−−−−−−−−−−−−√
σ

−

=

σ

C

(

−

)

2

+

σ

τ

C

(

−

)

2

+

σ

R

C

(

−

)

2

+

σ

ϵ

(

−

)

2
and σ+=σ−/b
σ

+

=

σ

−

/

b
. For simplicity I suggest not changing any of the variance component parameter values. Although the median mean-to-sigma ratio will be higher than 4.5 for readers under test 2, the increase usually will not be great because effect sizes of interest are typically relatively small.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix B

## Derivation of Equations  A10–A12

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

r=μ2−μ1σ2−σ1=ΔmΔσ
r

=

μ

2

−

μ

1

σ

2

−

σ

1

=

Δ

m

Δ

σ


and define


b=σ1σ2
b

=

σ

1

σ

2


From the relationship


AUC=Φ(Δmσ21+σ22√)
AUC

=

Φ

(

Δ

m

σ

1

2

+

σ

2

2

)


it follows that


Δm=Φ−1(AUC)σ21+σ22−−−−−−√
Δ

m

=

Φ

−

1

(

AUC

)

σ

1

2

+

σ

2

2


Define


c=Φ−1(AUC)
c

=

Φ

−

1

(

AUC

)


From Equations  B1–B5 , we have


Δm=cσ21+(σ1+Δσ)2−−−−−−−−−−−−−√=cσ21+(σ1+Δmr)2−−−−−−−−−−−−−−√
Δ

m

=

c

σ

1

2

+

(

σ

1

+

Δ

σ

)

2

=

c

σ

1

2

+

(

σ

1

+

Δ

m

r

)

2


Solving for Δm
Δ

m
yields the following quadratic equation in Δm
Δ

m
:


a˜(Δm)2+b˜(Δm)+c˜=0
a

˜

(

Δ

m

)

2

+

b

˜

(

Δ

m

)

+

c

˜

=

0


where


a˜=r2−c2,b˜=−2c2rσ21,c˜=−2c2r2σ21
a

˜

=

r

2

−

c

2

,

b

˜

=

−

2

c

2

r

σ

1

2

,

c

˜

=

−

2

c

2

r

2

σ

1

2


Assuming μ2≥μ1
μ

2

≥

μ

1
, the solution for Δm
Δ

m
in terms of _r_ and AUC, using the quadratic formula, is given by


Δm=−b˜+b˜2−4a˜c˜√2a˜
Δ

m

=

−

b

˜

+

b

˜

2

−

4

a

˜

c

˜

2

a

˜


I can then solve for _b_ using the relationship


b=rΔmσ1+r
b

=

r

Δ

m

σ

1

+

r


which follows from Equations  B1 and B2 .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Supplementary data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Appendix C

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Roe C.A., Metz C.E.: Dorfman-Berbaum-Metz method for statistical analysis of multireader, multimodality receiver operating characteristic data: validation with computer simulation. Acad Radiol 1997; 4: pp. 298-303.


- 2\. Dorfman D.D., Berbaum K.S., Lenth R.V., et. al.: Monte Carlo validation of a multireader method for receiver operating characteristic discrete rating data: factorial experimental design. Acad Radiol 1998; 5: pp. 591-602.


- 3\. Beiden S.V., Wagner R.F., Campbell G.: Components-of-variance models and multiple-bootstrap experiments: an alternative method for random-effects, receiver operating characteristic analysis. Acad Radiol 2000; 7: pp. 341-349.


- 4\. Beiden S.V., Wagner R.F., Campbell G., et. al.: Analysis of uncertainties in estimates of components of variance in multivariate ROC analysis. Acad Radiol 2001; 8: pp. 616-622.


- 5\. Wagner R.F., Beiden S.V., Metz C.E.: Continuous versus categorical data for ROC analysis: some quantitative considerations. Acad Radiol 2001; 8: pp. 328-334.


- 6\. Song X., Zhou X.H.: A marginal model approach for analysis of multi-reader multi-test receiver operating characteristic (ROC) data. Biostatistics 2005; 6: pp. 303-312.


- 7\. Hillis S.L., Berbaum K.S.: Monte Carlo validation of the Dorfman-Berbaum-Metz method using normalized pseudovalues and less data-based model simplification. Acad Radiol 2005; 12: pp. 1534-1541.


- 8\. Hillis S.L.: A comparison of denominator degrees of freedom methods for multiple observer ROC analysis. Stat Med 2007; 26: pp. 596-619.


- 9\. Hillis S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 10\. Hillis S.L., Obuchowski N.A., Berbaum K.S.: Power estimation for multireader ROC methods an updated and unified approach. Acad Radiol 2011; 18: pp. 129-142.


- 11\. Chakraborty D.P.: Prediction accuracy of a sample-size estimation method for ROC studies. Acad Radiol 2010; 17: pp. 628-638.


- 12\. Pepe M.: The statistical evaluation of medical tests for classification and prediction.2003.Oxford University PressNew York


- 13\. Swets J.A., Tanner W.P., Birdsall T.G.: Decision processes in perception. Psychol Rev 1961; 68: pp. 301-340.


- 14\. Green D.M., Swets J.A.: Signal detection theory and psychophysics.1988.Peninsula PublishingLos Altos, CA (Original work: Green DM, Swets JA. Signal detection theory and psychophysics. New York: Wiley, 1966.)


- 15\. Egan J.P.: Signal detection theory and ROC analysis.1974.Academic PressNew York


- 16\. Hillis S.L., Berbaum K.S.: Using the mean-to-sigma ratio as a measure of the improperness of binormal ROC curves. Acad Radiol 2011; 18: pp. 143-154.


- 17\.  Van Dyke CW, White RD, Obuchowski NA, et al. Cine MRI in the diagnosis of thoracic aortic dissection. 79th RSNA Meetings, Chicago, IL, November 28–December 3, 1993.


- 18\. Dorfman D.D., Alf E.: Maximum likelihood estimation of parameters of signal-detection theory and determination of confidence intervals–rating method data. J Math Psychol 1969; 6: pp. 487-496.


- 19\. Dorfman D.D.: RSCORE II.Swets J.A.Pickett R.M.Evaluation of diagnostic systems: methods from signal detection theory.1982.Academic PressSan Diego, Calif:pp. 212-232.


- 20\. Dorfman D.D., Berbaum K.S.: Degeneracy and discrete receiver operating characteristic rating data. Acad Radiol 1995; 2: pp. 907-915.


- 21\. Hanley J.A., McNeil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 22\.  Dorfman DD, Berbaum KS, Metz CE. Receiver operating characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 992; 27:723–731.


- 23\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of the diagnostic accuracy for multiple diagnostic tests: an ANOVA approach with dependent observations. Commun Stat Simul Comput 1995; 24: pp. 285-308.


- 24\. Quenoille M.H.: Approximate tests of correlation in time series. J Royal Stat Soc Series B 1949; 11: pp. 68-84.


- 25\. Quenoille M.H.: Notes on bias in estimation. Biometrika 1956; 43: pp. 353-360.


- 26\. Tukey J.W.: Bias and confidence in not quite large samples \[abstract\]. Ann Math Stat 1958; 29: pp. 614.


- 27\.  SAS for Windows, version 9.3, copyright 2002–2010 by SAS Institute Inc., Cary, NC.


- 28\. Swets J.A.: Form of empirical ROCS in discrimination and diagnostic tasks: implications for theory and measurement of performance. Psychol Bull 1986; 99: pp. 181-198.


- 29\. Swets J.A.: Indices of discrimination or diagnostic accuracy: their ROCs and implied models. Psychol Bull 1986; 99: pp. 100-117.