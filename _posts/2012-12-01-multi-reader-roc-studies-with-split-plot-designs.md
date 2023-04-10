---
title: Multi-reader ROC Studies with Split-plot Designs
author: [CL_AT_NancyAObuchowskiPhD,CL_AT_BronDGallasPhD,CL_AT_StephenLHillisPhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 12]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Multireader imaging trials often use a factorial design, in which study patients undergo testing with all imaging modalities and readers interpret the results of all tests for all patients. A drawback of this design is the large number of interpretations required of each reader. Split-plot designs have been proposed as an alternative, in which one or a subset of readers interprets all images of a sample of patients, while other readers interpret the images of other samples of patients. In this paper, the authors compare three methods of analysis for the split-plot design.

## Materials and Methods

Three statistical methods are presented: the Obuchowski-Rockette method modified for the split-plot design, a newly proposed marginal-mean analysis-of-variance approach, and an extension of the three-sample _U_ -statistic method. A simulation study using the Roe-Metz model was performed to compare the type I error rate, power, and confidence interval coverage of the three test statistics.

## Results

The type I error rates for all three methods are close to the nominal level but tend to be slightly conservative. The statistical power is nearly identical for the three methods. The coverage of 95% confidence intervals falls close to the nominal coverage for small and large sample sizes.

## Conclusions

The split-plot multireader, multicase study design can be statistically efficient compared to the factorial design, reducing the number of interpretations required per reader. Three methods of analysis, shown to have nominal type I error rates, similar power, and nominal confidence interval coverage, are available for this study design.

In imaging clinical trials, investigators often compare the accuracy of clinicians' diagnostic interpretations of different imaging modalities, assessing the sensitivity, specificity, and/or receiver-operating characteristic (ROC) indices of the modalities . In estimating the accuracy of mammography for detecting breast cancer, for example, mammograms are interpreted by trained radiologists who read the images to determine if suspicious lesions are present. It is well known that there is variability among readers in their visual, cognitive, and perceptual abilities ; similarly, there is variability among patients in their anatomy, comorbidities, and manifestation of disease. Thus, samples of both readers and patients are integral components in characterizing diagnostic test accuracy. The average accuracy of the readers is typically used as the measure of a test's accuracy. There has been a great deal of methodology development for the estimation and comparison of diagnostic tests' accuracy from multiple-reader studies .

Multireader imaging trials often use a factorial, or fully crossed, design, in which study patients undergo testing with all imaging modalities being compared, and study readers interpret the results of all of the tests for all patients. The rationale is that because both patients and readers introduce variability to the measurement of diagnostic accuracy, for comparing modalities, variability from these sources can be reduced if study patients undergo all modalities and if study readers interpret all of the test results.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## MRMC Split-plot Study Design

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Layout of Fully Crossed Multireader, Multicase Study Design


Reader 1 Reader 2… Reader _J_ Test 1 Test 2 Test 1 Test 2 Test 1 Test 2 Patient 1 X  111  X  211  X  121  X  221  X  1 _J_ 1  X  2 _J_ 1  Patient 2 X  112  X  212  X  122  X  222  X  1 _J_ 2  X  2 _J_ 2  Patient 3 X  113  X  213  X  123  X  223  X  1 _J_ 3  X  2 _J_ 3  … Patient _N_ T  X  11 _N_ X  21 _N_ X  12 _N_ X  22 _N_ X  1 _JN_ X  2 _JN_

_X__ijk_ denotes the test score assigned by the _j_ th reader to the _k_ th patient imaged with modality _i_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Layout of Split-plot Multireader, Multicase Study Design with Three Blocks


Block 1 Block 2 Block 3 Reader 1 Reader 2_X_ 1111  , _X_ 2111 _X_ 1211  , _X_ 2211 _X_ 1121  , _X_ 2121 _X_ 1221  , _X_ 2221 _X_ 1131  , _X_ 2131 _X_ 1231  , _X_ 2231  Reader 3 Reader 4_X_ 1342  , _X_ 2342 _X_ 1442  , _X_ 2442 _X_ 1352  , _X_ 2352 _X_ 1452  , _X_ 2452 _X_ 1362  , _X_ 2362 _X_ 1462  , _X_ 2462  Reader 5 Reader 6_X_ 1573  , _X_ 2573 _X_ 1673  , _X_ 2673 _X_ 1583  , _X_ 2583 _X_ 1683  , _X_ 2683 _X_ 1593  , _X_ 2593 _X_ 1693  , _X_ 2693

In a split-plot reader design with _G_ blocks, _J_ readers are randomized to a block and _N_ T  patients are randomized to a block such that in each block, there are _J_ / _G_ readers and _N_ T  / _G_ patients. In the three-block split-plot design illustrated here, _J_ = 6 and _N_ T  = 9; thus, two readers are randomized to each of the three blocks and three patients are randomized to each of the three blocks. _X__ijkg_ denotes the test score assigned by the _j_ th reader to the _k_ th patient imaged with modality _i_ in block _g_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Resources Needed for Different Study Designs


Study Design Number of Readers ( _J_ ) Number of Patients  ∗  Total Number of Image Interpretations Number of Image Interpretations per Reader Statistical Efficiency  †  Two-block split-plot 6 (3/block) 120 (30 + 30) 720 120 1.0 Three-block split-plot 9 (3/block) 120 (20 + 20) 720 80 1.2 Four-block split-plot 12 (3/block) 120 (15 + 15) 720 60 1.33 Fully paired A 6 60 (30 + 30) 720 120 0.83 Fully paired B 6 120 (60 + 60) 1440 240 1.16 Unpaired reader 12 120 (60 + 60) 1440 120 0.90

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## OR Test Statistic Modified for Split-plot Design

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ˆij=τi+Rj+(τR)ij+ϵij
ˆ

i

j

=

τ

i

+

R

j

+

(

τ

R

)

i

j

+

ϵ

i

j


where τi
τ

i
is the fixed effect of the _i_ th modality, _R__j_ is the random reader effect, and (τR)ij
(

τ

R

)

i

j
is the random effect due to the interaction of modality and reader. The error term in equation  1 is assumed to have a multivariate normal distribution with mean zero and covariance matrix defined as follows:


E(ϵij,ϵi′j′)=σ2ccov1=σ2cρ1cov2=σ2cρ2cov3=σ2cρ3ifi=i′andj=j′ifi≠i′andj=j′ifi=i′andj≠j′ifi≠i′andj≠j′,
E

(

ϵ

i

j

,

ϵ

i

′

j

′

)

=

σ

c

2

if

i

=

i

′

and

j

=

j

′

cov

1

=

σ

c

2

ρ

1

if

i

≠

i

′

and

j

=

j

′

cov

2

=

σ

c

2

ρ

2

if

i

=

i

′

and

j

≠

j

′

cov

3

=

σ

c

2

ρ

3

if

i

≠

i

′

and

j

≠

j

′

,


where ρ  1 denotes the correlation between errors corresponding to a reader reading the results of the same patients from different tests, ρ  2 denotes the correlation between different readers interpreting the same test, and ρ  3 denotes the correlation between different readers interpreting different tests.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

H0:τ1=τ2,HA:τ1≠τ2.
H

0

:

τ

1

=

τ

2

,

H

A

:

τ

1

≠

τ

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

F∗=MS(T)/{MS(T×R)+max\[J×ϕˆ,0\]},
F

∗

=

MS

(

T

)

/

{

MS

(

T

×

R

)

+

max

\[

J

×

ϕ

ˆ

,

0

\]

}

,


where MS is the mean square. Details of the calculation of the MS terms are given in the  Appendix .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ddf={MS(T×R)+max\[J×(coˆv2−coˆv3),0\]}2/{MS(T×R)2/\[(I−1)(J−1)\]}.
d

d

f

=

{

MS

(

T

×

R

)

+

max

\[

J

×

(

c

o

ˆ

v

2

−

c

o

ˆ

v

3

)

,

0

\]

}

2

/

{

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

}

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Marginal-mean ANOVA Test Statistic for Split-plot Design

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

F=MS(T)MS\[T×R(G)\]+max\[r(coˆv2−coˆv3),0\],
F

=

MS

(

T

)

MS

\[

T

×

R

(

G

)

\]

+

max

\[

r

(

c

o

ˆ

v

2

−

c

o

ˆ

v

3

)

,

0

\]

,


where


MS\[T×R(G)\]=∑Gg=1∑Ii=1∑rj=1(Yijg−Yi⋅g−Y⋅jg+Y⋅⋅g)2/\[G(I−1)(J−1)\],
MS

\[

T

×

R

(

G

)

\]

=

∑

g

=

1

G

∑

i

=

1

I

∑

j

=

1

r

(

Y

i

j

g

−

Y

i

·

g

−

Y

·

j

g

+

Y

·

·

g

)

2

/

\[

G

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


and cov  2 and cov  3 are computed as the averages of the corresponding estimated covariances within reader blocks; these covariances can be estimated using the same methods discussed previously for the OR statistic.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

F=MS(T)MS\[T×R(G)\]+max\[J−1J−GJϕˆ,0\].
F

=

MS

(

T

)

MS

\[

T

×

R

(

G

)

\]

+

max

\[

J

−

1

J

−

G

J

ϕ

ˆ

,

0

\]

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ddf={MS\[T×R(G)\]+max\[r(cov2−cov3),0\]}2{MS\[T×R(G)\]}2G(I−1)(r−1).
d

d

f

=

{

MS

\[

T

×

R

(

G

)

\]

+

max

\[

r

(

cov

2

−

cov

3

)

,

0

\]

}

2

{

MS

\[

T

×

R

(

G

)

\]

}

2

G

(

I

−

1

)

(

r

−

1

)

.


_F_ is compared to a central _F_ distribution with degrees of freedom ( _I_ −1) and _ddf_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Three-sample _U_ -statistic Test for Split-plot Design

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

cov(ˆi⋅,ˆi′⋅)=(αii′N0+α2ii′N1+α3ii′N0N1)+(α4ii′J)+(α4ii′N0J+α5ii′N1J+α6ii′N0N1J),
cov

(

ˆ

i

·

,

ˆ

i

′

·

)

=

(

α

i

i

′

N

0

+

α

2

i

i

′

N

1

+

α

3

i

i

′

N

0

N

1

)

+

(

α

4

i

i

′

J

)

+

(

α

4

i

i

′

N

0

J

+

α

5

i

i

′

N

1

J

+

α

6

i

i

′

N

0

N

1

J

)

,


where _J_ is the number of readers, _N_ 0 is the number of nondiseased cases, _N_ 1 is the number of diseased cases, and each αii′
α

i

i

′
is a variance when _i_ = i′
i

′
and a covariance when _i_ ≠ i′
i

′
. Gallas and Brown generalized the variance derivation and estimation in equation  8 to treat study designs that are not fully crossed by using scaling factors for the α values. This generalization is exactly what is used for the split-plot study designs examined here. Further details of Gallas's prior work are summarized in the  Appendix .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

T=ˆ1−ˆ2VˆUΔ√,
T

=

ˆ

1

−

ˆ

2

V

ˆ

U

Δ

,


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

df=(VˆUΔ)2(s2BR)2/(NR−1)3+(s2B0)2/(N0−1)3+(s2B1)2/(N1−1)3,
d

f

=

(

V

ˆ

U

Δ

)

2

(

s

B

R

2

)

2

/

(

N

R

−

1

)

3

+

(

s

B

0

2

)

2

/

(

N

0

−

1

)

3

+

(

s

B

1

2

)

2

/

(

N

1

−

1

)

3

,


where


s2BR=αˆB4ii+αˆB4i′i′−2αˆB4ii′,
s

B

R

2

=

α

ˆ

B

4

i

i

+

α

ˆ

B

4

i

′

i

′

−

2

α

ˆ

B

4

i

i

′

,


s2B0=αˆB1ii+αˆB1i′i′−2αˆB1ii′,
s

B

0

2

=

α

ˆ

B

1

i

i

+

α

ˆ

B

1

i

′

i

′

−

2

α

ˆ

B

1

i

i

′

,


and


s2B1=αˆB2ii+αˆB2i′i′−2αˆB2ii′
s

B

1

2

=

α

ˆ

B

2

i

i

+

α

ˆ

B

2

i

′

i

′

−

2

α

ˆ

B

2

i

i

′


are ideal bootstrap (method of moments) estimates of the components of variance for the three random effects : readers, nondiseased cases, and diseased cases. We can also refer to these as the nonparametric maximum likelihood estimates and relate them to the mean squares of a four-way ANOVA.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Parameter Values for Simulated Test Scores


Parameter Test Values Intercept For nondiseased patients, μ  0  = 0\. For diseased patients, μ  1  = 1.53. Fixed modality effect Under the null hypothesis, τit
τ

it
= 0 for i = 1 and 2 and t = 0 and 1. Under the alternative hypothesis, τi0
τ

i0
= 0 for i = 1 and 2, and τ11
τ

11
= 0 and τ21
τ

21
= 0.25. Random effect due to reader _j_ Two values of σ2r
σ

r

2
were tested, 0.011 and 0.056, to represent small and large interreader variability. Random effect due to case _k_σ2C
σ

C

2
was set to 0.1. Random effect due to modality × reader Two values of σ2τR
σ

τ

R

2
were tested, 0.03 and 0.06. Random effect due to modality × caseσ2τC
σ

τ

C

2
was set to 0.1. Random effect due to reader × caseσ2RC
σ

R

C

2
was set to 0.2. Random effect due to pure errorσ2τRC
σ

τ

R

C

2
was set to 0.2.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Type I error rates of three methods: marginal-mean analysis-of-variance (mm ANOVA) test statistic (equation 5 ) plotted with circles , modified Obuchowski-Rockette (OR) test statistic (equation 3 ) plotted with squares , and three-sample U -statistic (equation 9 ) plotted with diamonds . The nominal type I error rate was .05.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultireaderROCStudieswithSplitplotDesigns/0_1s20S1076633212004837.jpg)

![Figure 2, Coverage of 95% confidence intervals (CIs) of three methods: marginal-mean analysis-of-variance (mm ANOVA) test statistic ( circles ), modified Obuchowski-Rockette (OR) test statistic ( squares ), and three-sample U -statistic ( diamonds ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultireaderROCStudieswithSplitplotDesigns/1_1s20S1076633212004837.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example: CAD of Breast Cancer

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Summary of Results of Three Methods for Breast Cancer Example


Method Test Statistic ( _P_ ) Estimated Difference (Standard Error) 95% Confidence Interval for Difference Marginal-mean analysis of variance_F_ = 3.12 (.0786) 0.0076 (0.00431) −0.0009 to 0.0161 Modified Obuchowski-Rockette_F_ = 3.37 (.0678) 0.0076 (0.00415) −0.0005 to 0.0159 Three-sample U-statistic_F_ = 3.55 (.0644) 0.0076 (0.00404) −0.0005 to 0.0157

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 6


Layout of Four-block Split-plot Design Simultaneously Evaluating Four CAD Systems


Reader Block 1 Reader Block 2 Reader Block 3 Reader Block 4 Patient block 1 Unaided vs CAD 1 Unaided vs CAD 2 Unaided vs CAD 3 Unaided vs CAD 4 Patient block 2 Unaided vs CAD 4 Unaided vs CAD 1 Unaided vs CAD 2 Unaided vs CAD 3 Patient block 3 Unaided vs CAD 3 Unaided vs CAD 4 Unaided vs CAD 1 Unaided vs CAD 2 Patient block 4 Unaided vs CAD 2 Unaided vs CAD 3 Unaided vs CAD 4 Unaided vs CAD 1

CAD, computer-aided diagnosis.


Each reader block contained nine readers. Each patient block contained 25 patients with cancer and 25 patients without cancer.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## Calculation of Mean Square Terms for OR Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

MS(T)=J∑i(ˆi⋅−ˆ⋅⋅)2/(I−1),
MS

(

T

)

=

J

∑

i

(

ˆ

i

·

−

ˆ

·

·

)

2

/

(

I

−

1

)

,


and


MS(T×R)={1/(J−1)(I−1)}∑i∑j(ˆij−ˆi⋅−ˆ⋅j+ˆ⋅⋅)2.
MS

(

T

×

R

)

=

{

1

/

(

J

−

1

)

(

I

−

1

)

}

∑

i

∑

j

(

ˆ

i

j

−

ˆ

i

·

−

ˆ

·

j

+

ˆ

·

·

)

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ˆi⋅=∑jˆij/J,
ˆ

i

·

=

∑

j

ˆ

i

j

/

J

,


ˆ⋅j=∑iˆij/I,
ˆ

·

j

=

∑

i

ˆ

i

j

/

I

,


and


ˆ⋅⋅=∑i∑jˆij/I×J,
ˆ

·

·

=

∑

i

∑

j

ˆ

i

j

/

I

×

J

,


where _i_ = 1,…, _I_ , and _j_ = 1,…, _J_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Rationale for Marginal-mean Model Approach

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Yijg=μ+τi+γg+Rj(g)+(τγ)ig+(τR)ij(g)+ϵijg,
Y

i

j

g

=

μ

+

τ

i

+

γ

g

+

R

j

(

g

)

+

(

τ

γ

)

i

g

+

(

τ

R

)

i

j

(

g

)

+

ϵ

i

j

g

,


where _g_ = 1,…, _G_ , _i_ = 1,…, _t_ , _j_ = 1,…, _r_ , where _G_ is the number of blocks, _t_ is the number of tests, _r_ is the number of readers in each block, τi
τ

i
denotes the fixed effect of test, γg
γ

g
denotes the fixed effect of block, and (τγ)ig
(

τ

γ

)

i

g
denotes the fixed test-by-block interaction. Rj(g)
R

j

(

g

)
and (τR)ij(g)
(

τ

R

)

i

j

(

g

)
are random reader and test-by-reader effects, nested within block; they are mutually independent and normally distributed with zero means and respective variances σ2R(G)
σ

R

(

G

)

2
and σ2τR(G)
σ

τ

R

(

G

)

2
, where the subscript _R_ ( _G_ ) is read “reader nested within group,” and so on. The ϵijg
ϵ

i

j

g
are normally distributed with zero mean and variance σ2ϵ
σ

ϵ

2
. The ϵijg
ϵ

i

j

g
are independent of the Rj(g)
R

j

(

g

)
and (τR)ij(g)
(

τ

R

)

i

j

(

g

)
. The covariances are defined by cov1≡cov(ϵijg,ϵi′jg)
cov

1

≡

cov

(

ϵ

i

j

g

,

ϵ

i

′

j

g

)
, cov2≡cov(ϵijg,ϵij′g)
cov

2

≡

cov

(

ϵ

i

j

g

,

ϵ

i

j

′

g

)
, and cov2≡cov(ϵijg,ϵi′g)
cov

2

≡

cov

(

ϵ

i

j

g

,

ϵ

i

′

g

)
, where i≠i′
i

≠

i

′
, j≠j′
j

≠

j

′
, and are subject to these constraints: cov  1 ≥ cov  3 , cov  2 ≥ cov  3 , and cov  3 ≥ 0\. Thus this is a three-way split-plot ANOVA with correlated errors, with test and block crossed and reader nested within block. Thus, readers are the whole plots, test is the split-plot factor, and block is the whole-plot factor.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Background Work for the Three-sample _U_ -sample Approach

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Xijkt=μt+τit+Rjt+Ckt+(τR)ijt+(τC)ikt+(RC)jkt+(τRC)ijkt+Eijkt,
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

j

t

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

,


where _X__ijkt_ is the test score assigned by the _j_ th reader to the _k_ th case with truth state _t_ ( _t_ = 0 for nondiseased patients and _t_ = 1 for diseased patients) imaged with modality _i_ . Every effect on the right-hand side depends on the truth state _t_ : μ _t_ is an intercept term; τit
τ

i

t
is the fixed effect due to the _i_ th modality; _R__jt_ is the random effect due to the _j_ th reader; _C__kt_ is the random effect due to the _k_ th case; (τR)ijt
(

τ

R

)

i

j

t
is the random effect due to the interaction between modality and reader; (τC)ikt
(

τ

C

)

i

k

t
is the random effect due to the interaction between modality and case; ( _RC_ ) _jkt_ is the random effect due to the interaction between reader and case; (τRC)ijkt
(

τ

R

C

)

i

j

k

t
is the random effect due to the three-way interaction between modality, reader, and patient; and _E__ijkt_ is the pure random error term.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Parameter Estimates from Breast Cancer CAD Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table A1


Estimates of Variance from Three-sample _U_ -statistic Method


Components of Variance Corresponding to Equation  8  Without CAD With CAD Covariance α  1  : nondiseased cases 0.005446 0.005281 0.005388 α  2  : diseased cases 0.037868 0.038301 0.037542 α  3  : nondiseased and diseased cases 0.002588 0.002841 0.002678 α  4  : readers 0.001130 0.000880 0.001053 α  5  : nondiseased cases and readers 0.015376 0.016371 0.015150 α  6  : diseased cases and readers 0.036952 0.034328 0.032539 α  7  : nondiseased cases and diseased cases and readers 0.024778 0.025958 0.023680

CAD, computer-aided diagnosis.


Table A2


Estimates of Variance from ANOVA


Variance Component Estimates from ANOVA Reader  ∗  0.001661 Treatment × reader  ∗  −0.000026 Error  †  0.003888 cov  1  †  0.003709 (r = 0.954) cov  2  ‡  0.001798 (r = 0.463) cov  3  ‡  0.001775 (r = 0.457)

ANOVA, analysis of variance.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Metz C.E.: Basic principles of ROC analysis. Semin Nucl Med 1978; 8: pp. 283-298.


- 2\. Zweig M.H., Campbell G.: Receiver operating characteristic plots: a fundamental evaluation tool in clinical medicine. Clin Chem 1993; 39: pp. 561-577.


- 3\. Pepe M.S.: The Statistical Evaluation of Medical Tests for Classification and Prediction.2004.Oxford University PressNew York


- 4\. Zhou X.H., Obuchowski N.A., McClish D.L.: Statistical Methods in Diagnostic Medicine.2nd ed.2011.John WileyHoboken, NJ


- 5\. Wagner R.F., Metz C.E., Campbell G.: Assessment of medical imaging systems and computer aids: a tutorial review. Acad Radiol 2007; 14: pp. 723-748.


- 6\. Beam C.A., Layde P.M., Sullivan D.C.: Variability in the interpretation of screening mammograms by US radiologists: findings from a national sample. Arch Intern Med 1996; 156: pp. 209-213.


- 7\. Chakraborty D.P.: Analysis of location specific observer performance data: validated extensions of the jackknife free-response (JAFROC) method. Acad Radiol 2006; 13: pp. 1187-1193.


- 8\. Dorfman D.D., Berbaum K.S., Metz C.E.: ROC rating analysis: generalization to the population of readers and cases with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 9\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of the diagnostic accuracy for multiple diagnostic tests: an ANOVA approach with dependent observations. Commun Stat Simul Comput 1995; 24: pp. 285-308.


- 10\. Beiden S.V., Wagner R.F., Campbell G.: Components-of-variance models and multiple-bootstrap experiments: an alternative method for random-effects, receiver operating characteristic analysis. Acad Radiol 2000; 7: pp. 341-349.


- 11\. Beiden S.V., Wagner R.F., Campbell G., et. al.: Components-of-variance models for random-effects ROC analysis: the case of unequal variance structures across modalities. Acad Radiol 2001; 8: pp. 605-615.


- 12\. Beiden S.V., Wagner R.F., Campbell G., et. al.: Analysis of uncertainties in estimates of components of variance in multivariate ROC analysis. Acad Radiol 2001; 8: pp. 616-622.


- 13\. Obuchowski N.A., Beiden S.V., Berbaum K.S., et. al.: Multireader, multicase receiver operating characteristic analysis: an empirical comparison of five methods. Acad Radiol 2004; 11: pp. 980-995.


- 14\. Hillis S.L.: A comparison of denominator degrees of freedom methods for multiple observer ROC analysis. Stat Med 2007; 26: pp. 596-619.


- 15\. Gallas B.D.: One-shot estimate of MRMC variance: AUC. Acad Radiol 2006; 13: pp. 353-362.


- 16\. Bandos A.I., Rockette H.E., Gur D.: A permutation test for comparing ROC curves in multireader studies. Acad Radiol 2006; 13: pp. 414-420.


- 17\. Obuchowski N.A.: Multi-reader ROC studies: a comparison of study designs. Acad Radiol 1995; 2: pp. 709-716.


- 18\. Obuchowski N.A.: Reducing the number of reader interpretations in MRMC studies. Acad Radiol 2009; 16: pp. 209-217.


- 19\. Gallas B.D., Pennello G.A., Myers K.J.: Multireader multicase variance analysis for binary data. J Opt Soc Am A Opt Image Sci Vis 2007; 24: pp. B70-B80.


- 20\. Gallas B.D., Brown D.G.: Reader studies for validation of CAD systems. Neural Networks 2008; 21: pp. 387-397.


- 21\.  Hillis SL. A marginal-mean ANOVA approach for analyzing multi-reader radiological imaging data. Unpublished manuscript submitted for review.


- 22\. Bhat B.R.: On the distribution of certain quadratic forms in normal variates. J R Stat Soc B 1962; 24: pp. 148-151.


- 23\. DeLong E., DeLong D., Clarke-Pearson D.: Comparing areas under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-845.


- 24\. Gallas B.D., Bandos A., Samuelson F., et. al.: A framework for random-effects ROC analysis: biases with the bootstrap and other variance estimators. Commun Stat A Theory 2009; 38: pp. 2586-2603.


- 25\. Barrett H.H., Kupinski M.A., Clarkson E.: Probabilistic foundations of the MRMC method. Proc SPIE 2005; 5749: pp. 21-31.


- 26\. Clarkson E., Kupinski M.A., Barrett H.H.: A probabilistic model for the MRMC method. Part 1. Theoretical development. Acad Radiol 2006; 13: pp. 1410-1421.


- 27\. Roe C.A., Metz C.E.: Variance-component modeling in the analysis of receiver operating characteristic index estimates. Acad Radiol 1997; 4: pp. 587-600.


- 28\. Dorfman D.D., Berbaum K.S., Lenth R.V., et. al.: Monte Carlo validation of a multireader method for receiver operating characteristic discrete rating data: factorial experimental design. Acad Radiol 1998; 5: pp. 9-19.


- 29\. Hillis S.L., Obuchowski N.A., Berbaum K.S.: Power estimation for multireader ROC methods an updated and unified approach. Acad Radiol 2011; 18: pp. 129-142.