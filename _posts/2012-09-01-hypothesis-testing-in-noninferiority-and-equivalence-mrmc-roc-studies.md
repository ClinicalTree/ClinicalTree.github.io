---
title: Hypothesis Testing in Noninferiority and Equivalence MRMC ROC Studies
author: [CL_AT_WeijieChenPhD,CL_AT_NicholasAPetrickPhD,CL_AT_BerkmanSahinerPhD]
date: 2012-09-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 9]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Conventional multireader multicase receiver operating characteristic (MRMC ROC) methodologies use hypothesis testing to test differences in diagnostic accuracies among several imaging modalities. The general MRMC-ROC analysis framework is designed to show that one modality is statistically different among a set of competing modalities (ie, the superiority setting). In practice, one may wish to show that the diagnostic accuracy of a modality is noninferior or equivalent, in a statistical sense, to that of another modality instead of showing its superiority (a higher bar). The purpose of this article is to investigate the appropriate adjustments to the conventional MRMC ROC hypothesis testing methodology for the design and analysis of noninferiority and equivalence hypothesis tests.

## Materials and Methods

We present three methodological adjustments to the updated and unified Obuchowski-Rockette (OR)/Dorfman-Berbaum-Metz (DBM) MRMC ROC method for use in statistical noninferiority/equivalence testing: 1) the appropriate statement of the null and alternative hypotheses; 2) a method for analyzing the experimental data; and 3) a method for sizing MRMC noninferiority/equivalence studies. We provide a clinical example to further illustrate the analysis of and sizing/power calculation for noninferiority MRMC ROC studies and give some insights on the interplay of effect size, noninferiority margin parameter, and sample sizes.

## Results

We provide detailed analysis and sizing computation procedures for a noninferiority MRMC ROC study using our method adjusted from the updated and unified OR/DBM MRMC method. Likewise, we show that an equivalence hypothesis test is identical to performing two simultaneous noninferiority tests (ie, either modality is noninferior to the other).

## Conclusion

Conventional MRMC ROC methodology developed for superiority studies can and should be adjusted appropriately for the design and analysis of a noninferiority/equivalence hypothesis testing. In addition, the confidence interval of the difference in diagnostic accuracies is important information and should generally accompany the statistical analysis and any conclusions drawn from the hypothesis testing.

Multireader multicase receiver operating characteristic (MRMC ROC) analysis is a popular approach to evaluating and comparing the diagnostic accuracy of medical imaging modalities . A commonly used statistical tool for comparing the diagnostic accuracy of two or more imaging modalities is hypothesis testing. Methods of hypothesis testing in MRMC ROC studies have been investigated extensively, for example, the DBM (Dorfman-Berbaum-Metz) method and the OR (Obuchowski-Rockette) method . These methods have been further updated and compared and, more recently, the DBM and the OR methods are unified for the analysis and power estimation of multireader ROC studies . In these methods, the null and alternative hypotheses are generally defined as follows: under the null hypothesis (denoted as H  0 ), the diagnostic accuracies (eg, areas under the ROC curve, or AUC) of all the modalities are equal; under the alternative hypothesis (denoted as H  1 ), they are not all equal (ie, at least one is significantly different from the others). The goal of the study is to reject the null hypothesis and demonstrate there is a difference or superiority, the success of which can be claimed by obtaining a _P_ value (Type I error rate) that is less than a prespecified significance level α (eg, 0.05).

Although superiority of diagnostic accuracy is often the driving force for scientific innovation, meeting this high bar is not always necessary for accepting a new technology into clinical practice. For example, when a new imaging modality offers lower or equivalent radiation dose to the patient than does the conventional modality and has similar diagnostic accuracy (ie, noninferior performance), it would be appropriate for use in the clinic. Another example could be demonstrating that a computer-aided diagnosis (CAD) system works equally well on images obtained from multiple image acquisition systems where equivalent performance among the various imaging systems would provide evidence of the robustness of the CAD system across different image acquisition systems.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Statement of Hypotheses

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Illustration of the null and alternative hypotheses in equivalence and noninferiority tests.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/HypothesisTestinginNoninferiorityandEquivalenceMRMCROCStudies/0_1s20S1076633212002310.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Statements of the Hypotheses in Four Types of Hypothesis Testing Settings


Two-sided One-sided Nonequivalence Superiority H  0  :  e  −  c  = 0 H  0  :  e  −  c  = 0 H  1  :  e  −  c  ≠ 0 H  1  :  e  −  c  \> 0 Equivalence Noninferiority H  0  : \|  e  −  c  \| = δ H  0  :  e  −  c  = −δ H  1  : \|  e  −  c  \| < δ H  1  :  e  −  c  \> −δ

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Analysis of Data for Noninferiority Tests

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

t=ˆe∙−ˆc∙+δsˆ,
t

=

^

e

•

−

^

c

•

+

δ

s

^

,


where ˆi∙
^

i

•
is the estimated average reader AUC for modality _i_ ( _i_ = _e,c_ ) and the dot symbol represents an average over readers, sˆ
s

^
is the estimated standard deviation (SD) of ˆe∙−ˆc∙+δ
^

e

•

−

^

c

•

+

δ
,


sˆ=2JMS(T∗R)+2H(coˆv2−coˆv3)−−−−−−−−−−−−−−−−−−−−−−−−−−√,
s

^

=

2

J

M

S

(

T

∗

R

)

+

2

H

(

c

o

^

v

2

−

c

o

^

v

3

)

,


where the function H is defined as H(x) = x if x > 0 and 0 otherwise, coˆv2
c

o

^

v

2
is the estimated covariance in diagnostic accuracies of different readers in the same modality, coˆv3
c

o

^

v

3
is the estimated covariance in diagnostic accuracies of different readers in different modalities, and MS(T\*R) is the two-way ANOVA test-by-reader mean squares in the OR model,


MS(T∗R)=12(J−1)∑Jj=1\[(ˆej−ˆcj)−(ˆe∙−ˆc∙)\]2.
M

S

(

T

∗

R

)

=

1

2

(

J

−

1

)

∑

j

=

1

J

\[

(

^

e

j

−

^

c

j

)

−

(

^

e

•

−

^

c

•

)

\]

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

dˆf0={MS(T∗R)+H(J(coˆv2−coˆv3))}2(MS(T∗R))2/(J−1).
d

^

f

0

=

{

M

S

(

T

∗

R

)

+

H

(

J

(

c

o

^

v

2

−

c

o

^

v

3

)

)

}

2

(

M

S

(

T

∗

R

)

)

2

/

(

J

−

1

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

\[ˆe∙−ˆc∙−sˆtα/2,df0,ˆe∙−ˆc∙+sˆtα/2,df0\].
\[

^

e

•

−

^

c

•

−

s

^

t

α

/

2

,

d

f

0

,

^

e

•

−

^

c

•

+

s

^

t

α

/

2

,

d

f

0

\]

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Sizing/Power Calculation for Noninferiority Tests

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


λˆ=d+δ2{σˆ2TR+c∗c\[σˆ2ϵ−coˆv1+(J−1)H(coˆv2−coˆv3)\]}/J√,
λ

^

=

d

+

δ

2

{

σ

^

T

R

2

+

c

∗

c

\[

σ

^

ϵ

2

−

c

o

^

v

1

+

(

J

−

1

)

H

(

c

o

^

v

2

−

c

o

^

v

3

)

\]

}

/

J

,


dˆf1={σˆ2TR+c∗c\[σˆ2ϵ−coˆv1+(J−1)H(coˆv2−coˆv3)\]}2{σˆ2TR+c∗c\[σˆ2ϵ−coˆv1−H(coˆv2−coˆv3)\]}2J−1,
d

^

f

1

=

{

σ

^

T

R

2

+

c

∗

c

\[

σ

^

ϵ

2

−

c

o

^

v

1

+

(

J

−

1

)

H

(

c

o

^

v

2

−

c

o

^

v

3

)

\]

}

2

{

σ

^

T

R

2

+

c

∗

c

\[

σ

^

ϵ

2

−

c

o

^

v

1

−

H

(

c

o

^

v

2

−

c

o

^

v

3

)

\]

}

2

J

−

1

,


where c  ∗ is the case sample size in the pilot study, c and J are the case sample size and the reader sample size, respectively, for the planned study, σˆ2∈
σ

^

∈

2
is the sum of case variability and the within-reader variability, and the test-reader interaction variance is estimated as


σˆ2TR=MS(T∗R)−σˆ2ϵ+coˆv1+H(coˆv2−coˆv3).
σ

^

T

R

2

=

M

S

(

T

∗

R

)

−

σ

^

ϵ

2

+

c

o

^

v

1

+

H

(

c

o

^

v

2

−

c

o

^

v

3

)

.


- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Illustration of the distributions of the test statistic under the null and alternative hypotheses.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/HypothesisTestinginNoninferiorityandEquivalenceMRMCROCStudies/1_1s20S1076633212002310.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Power=1−F(tc;df1,λ\|H1),
Power

=

1

−

F

(

t

c

;

df

1

,

λ

\|

H

1

)

,


where F(t; df  1 , _λ\|H__1_ ) is the distribution function of the test statistic t under the alternative hypothesis H  1 and t  c = F  −1 (1-α/2;df  0 \|H  0 ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Equivalence Tests

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Example

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Combinations of Number of Cases and Number Readers for 80% Power in Establishing Noninferiority of Spin-echo MRI as Compared to Cine MRI, Based on the Van Dyke et al Data


Noninferiority Margin δ = 0.01 Noninferiority Margin δ = 0.02σˆ2TR=0
σ

^

T

R

2

=

0
σˆ2TR=0.0001
σ

^

T

R

2

=

0.0001
σˆ2TR=0
σ

^

T

R

2

=

0
σˆ2TR=0.0001
σ

^

T

R

2

=

0.0001
Readers Cases Power Cases Power Cases Power Cases Power 3 559 0.8005 1898 0.8000 388 0.8003 710 0.8002 4 343 0.8004 491 0.8004 238 0.8001 300 0.8002 5 266 0.8014 330 0.8007 185 0.8020 213 0.8005 6 225 0.8004 263 0.8002 157 0.8023 174 0.8011 7 200 0.8002 227 0.8014 139 0.8005 151 0.8002 8 183 0.8001 203 0.8008 128 0.8029 137 0.8022 9 171 0.8008 187 0.8018 119 0.8016 126 0.8008 10 162 0.8017 174 0.8002 113 0.8035 118 0.8002 11 154 0.8003 165 0.8010 107 0.8005 112 0.8004 12 148 0.8002 158 0.8021 103 0.8011 108 0.8033 13 143 0.8001 152 0.8024 100 0.8028 104 0.8033 14 139 0.8005 146 0.8001 97 0.8024 100 0.8008 15 136 0.8021 142 0.8009 94 0.8003 97 0.8001

MRI, magnetic resonance imaging.


The abnormal to normal case ratio in the planned study is assumed to be the same as that in the Van Dyke data (ie, 45/69 = 0.652). The effect size d is 0.04 as measured in the Van Dyke study.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

H0:e−(c−δ)=0
H

0

:

e

−

(

c

−

δ

)

=

0


H1:e−(c−δ)>0,
H

1

:

e

−

(

c

−

δ

)

>

0

,


and comparing to the superiority test (  Table 1 ), we see immediately that to show _e_ is noninferior to _c_ appears isomorphic with showing _e_ is superior to _c_ − _δ_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Wagner R.F., Metz C.E., Campbell G.: Assessment of medical imaging systems and computer aids: a tutorial review. Acad Radiol 2007; 14: pp. 723-748.


- 2\. Dorfman D.D., Berbaum K.S., Metz C.E.: Receiver operating characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 3\. Hillis S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 4\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of the diagnostic accuracy for multiple diagnostic tests: an ANOVA approach with dependent observations. Commun Stat Simulation Comput 1995; 24: pp. 285-308.


- 5\.  Obuchowski NA. Multi-reader multi-modality ROC studies: hypothesis testing and sample size estimation using an ANOVA approach with dependent observations. With rejoinder. Acad Radiol 1995; 2(Suppl 1):S22–S29.


- 6\. Hillis S.L., Obuchowski N.A., Schartz K.M., et. al.: A comparison of the Dorfman-Berbaum-Metz and Obuchowski-Rockette methods for receiver operating characteristic (ROC) data. Stat Med 2005; 24: pp. 1579-1607.


- 7\. Hillis S.L.: A comparison of denominator degrees of freedom methods for multiple observer ROC analysis. Stat Med 2007; 26: pp. 596-619.


- 8\. Hills S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 9\. Hillis S.L., Obuchowski N.A., Berbaum K.S.: Power estimation for multireader ROC methods: an updated and unified approach. Acad Radiol 2011; 18: pp. 129-142.


- 10\. Blackwelder W.C.: “Proving the null hypothesis” in clinical trials. Controlled Clin Trials 1982; 3: pp. 345-353.


- 11\. Metz C.E.: Quantification of failure to demonstrate statistical significance: the usefulness of confidence intervals. Invest Radiol 1993; 28: pp. 59-63.


- 12\. Fisher R.A.: The Design of Experiments.1935.Oliver and BoydLondon


- 13\. Liu J.-P., Ma M.-C., Wu C.-Y., et. al.: Tests of equivalence and non-inferiority for diagnostic accuracy based on the paired areas under ROC curves. Stat Med 2006; 25: pp. 1219-1238.


- 14\. Li C.-R., Liao C.-T., Liu J.-P.: A non-inferiority test for diagnostic accuracy based on the paired partial areas under ROC curves. Stat Med 2008; 27: pp. 1762-1776.


- 15\. Lu Y., Jin H., Genant H.K.: On the non-inferiority of a diagnostic test based on paired observations. Stat Med 2003; 22: pp. 3029-3044.


- 16\. Lui K.J., Zhou X.H.: Testing non-inferiority (and equivalence) between two diagnostic procedures in paired-sample ordinal data. Stat Med 2004; 23: pp. 545-559.


- 17\.  Van Dyke CW, White RD, Obuchowski NA, et al. Cine MRI in the diagnosis of thoracic aortic dissection. 79th RSNA Meetings, Chicago, IL; 1993.


- 18\. Pan X.C., Metz C.E.: The “proper” binormal model: parametric receiver operating characteristic curve estimation with degenerate data. Acad Radiol 1997; 4: pp. 380-389.


- 19\. Metz C.E., Pan X.C.: “Proper” binormal ROC curves: theory and maximum likelihood estimation. J Math Psychol 1999; 43: pp. 1-33.


- 20\. Gennaro G., Toledano A., di Maggio C., et. al.: Digital breast tomosynthesis versus digital mammography: a clinical performance study. Eur Radiol 2010; 20: pp. 1545-1553.


- 21\. Hanley J.A., McNeil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 22\. Gallas B.D., Brown D.G.: Reader studies for validation of CAD systems. Neural Networks 2008; 21: pp. 387-397.


- 23\. Obuchowski N.A.: Reducing the number of reader interpretations in MRMC studies. Acad Radiol 2009; 16: pp. 209-217.