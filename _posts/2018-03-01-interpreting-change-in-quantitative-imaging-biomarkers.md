---
title: Interpreting Change in Quantitative Imaging Biomarkers
author: [Nancy A. Obuchowski PhD]
date: 2018-03-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 25, Issue 3 SOURCE CL_S_AcademicRadiologyVolume25Issue3 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Quantitative imaging biomarkers (QIBs) are becoming increasingly adopted into clinical practice to monitor changes in patients' conditions. The repeatability coefficient (RC) is the clinical cut-point used to discern between changes in a biomarker's measurements due to measurement error and changes that exceed measurement error, thus indicating real change in the patient. Imaging biomarkers have characteristics that make them difficult for estimating the repeatability coefficient, including nonconstant error, non-Gaussian distributions, and measurement error that must be estimated from small studies.

## Methods

We conducted a Monte Carlo simulation study to investigate how well three statistical methods for estimating the repeatability coefficient perform under five settings common for QIBs.

## Results

When the measurement error is constant and replicates are normally distributed, all of the statistical methods perform well. When the measurement error is proportional to the true value, approaches that use the log transformation or coefficient of variation perform similarly. For other common settings, none of the methods for estimating the repeatability coefficient perform adequately.

## Conclusion

Many of the common approaches to estimating the repeatability coefficient perform well for only limited scenarios. The optimal approach depends strongly on the pattern of the within-subject variability; thus, a precision profile is critical in evaluating the technical performance of QIBs. Asymmetric bounds for detecting regression vs progression can be implemented and should be used when clinically appropriate.

## Introduction

As quantitative imaging biomarkers (QIBs) become increasingly adopted into clinical practice for diagnosis, prognosis, and disease monitoring, it is critical that clinicians be able to interpret them properly. Clinicians must be able to discern between changes in a biomarker's measurements that are expected because of measurement error by the imaging system and changes that exceed measurement error and thus indicate a real change in the patient.

Studies of the technical performance of QIBs, particularly studies of their repeatability, are used to help radiologists interpret change. Organizations such as the Quantitative Imaging Biomarker Alliance (QIBA) conduct groundwork studies to estimate biomarkers' performance. They also perform meta-analyses to summarize biomarkers' performance over multiple published studies . From these studies of repeatability, investigators calculate a cut-point, or threshold, for discerning when a measured change is attributable to measurement error vs when the measured change should be interpreted as a real change in the patient, with some stated degree of confidence . For illustration, when measuring the change in volume of a pulmonary lesion from baseline, a measured change <25% might be considered purely measurement error, whereas a measured change exceeding 25% might be considered a real change, with 95% confidence .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## Defining Change

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Three Definitions of Change in QIBs  \\*

Difference from baseline

dˆ=(Yit−Yib)
d

^

=

(

Y

i

t

−

Y

i

b

)


Percentage change from baseline

%dˆb=(Yit−Yib)/Yib×100
%

d

^

b

=

(

Y

i

t

−

Y

i

b

)

/

Y

i

b

×

100


Percentage difference

%dˆmean=(Yit−Yib)(Yib+Yit)/2×100
%

d

^

mean

=

(

Y

i

t

−

Y

i

b

)

(

Y

i

b

+

Y

i

t

)

/

2

×

100


QIBs, quantitative imaging biomarkers.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods for Estimating Cut-Points From Technical Performance Studies

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Yik=βo+β1Xik+ϵik​,
Y

i

k

=

β

o

+

β

1

X

i

k

+

ϵ

i

k

​

,


where _β  o_ is the fixed bias, _β_ 1 is the proportional bias, and ϵik
ϵ

i

k
is the measurement error. It is often assumed that the measurement error is constant and follows a normal distribution, ϵik~N(0,σ2)
ϵ

i

k

~

N

(

0

,

σ

2

)
. We vary these assumptions in our Monte Carlo simulation study to consider scenarios typical in imaging. The measurement error, _σ_ 2 , is often referred to as the within-subject variance. Its square root is referred to as the within-subject standard deviation (wSD) .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σˆ2=∑Ni=1{Yi1−Yi2}2/2N,
σ

^

2

=

∑

i

=

1

N

{

Y

i

1

−

Y

i

2

}

2

/

2

N

,


where _Y  ik_ denotes the biomarker measurement for the _k_ th replicate on the _i_ th subject. Assuming constant within-subject variance and normality, the cut-point associated with 95% confidence is then


RCˆ=1.96×2σˆ2−−−√,
R

C

^

=

1.96

×

2

σ

^

2

,


where RC is the repeatability coefficient, or the least significant difference between two repeat measurements taken under identical conditions . Changes in the biomarker that exceed +RC or are less than −RC are considered real changes (not as a result of just measurement error), with 95% confidence. Specifically, measured differences <−RC are considered true regression, whereas measured differences >+RC are considered true progression. We refer to this simple approach as Approach 1 (see first row of  Table 2 ).

Table 2


Three Approaches to Discerning Measurement Error From Real Change


“The observed change in QIB is attributable to measurement error.” “The observed change in the QIB represents true change in the patient, with 95% confidence.” Approach 1

−RCˆ<dˆ<+RCˆ
−

R

C

^

<

d

^

<

+

R

C

^


dˆ<−RCˆordˆ>+RCˆ
d

^

<

−

R

C

^

o

r

d

^

>

+

R

C

^


Approach 2A

−%RCˆ<%dˆb<+%RCˆ
−

%

R

C

^

<

%

d

^

b

<

+

%

R

C

^


%dˆb<−%RCˆor%dˆb>+%RCˆ
%

d

^

b

<

−

%

R

C

^

o

r

%

d

^

b

>

+

%

R

C

^


Approach 2B

−%RCˆ<%dˆmean<+%RCˆ
−

%

R

C

^

<

%

d

^

mean

<

+

%

R

C

^


%dˆmean<−%RCˆor%dˆmean>+%RCˆ
%

d

^

mean

<

−

%

R

C

^

o

r

%

d

^

mean

>

+

%

R

C

^


Approach 3A

RClnlower<%dˆb<RClnupper
R

C

lnlower

<

%

d

^

b

<

R

C

lnupper


%dˆb<RClnloweror%dˆb>RClnupper
%

d

^

b

<

R

C

lnlower

or

%

d

^

b

>

R

C

lnupper


Approach 3B

%RClnlower<%dˆmean<%RClnupper
%

R

C

lnlower

<

%

d

^

mean

<

%

R

C

lnupper


%dˆmean<%RClnloweror%dˆmean>%RClnupper
%

d

^

mean

<

%

R

C

lnlower

or

%

d

^

mean

>

%

R

C

lnupper


QIB, quantitative imaging biomarker.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Illustration of lower and upper bounds of RC based on three statistical approaches. The green range is based on Approach 1 where the difference between two measurements (ie, dˆ d^ ) is quantified in the original units of the biomarker (mm 3 used here for illustration). Measurement error is distinguished from real change based on estimates of the wSD. The red and blue ranges are based on statistical Approaches 2 and 3, respectively, where the percent change from baseline (ie, dˆb d^b ) or the percent difference in the two measurements (ie, dˆmean d^mean ) is quantified. Measurement error is distinguished from real change based on estimates of either the wCV (leading to a symmetric range) or the wSD after log transformation (leading to an asymmetric range). RC, repeatability coefficient; wCV, within-subject coefficient of variation; wSD, within-subject standard deviation. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InterpretingChangeinQuantitativeImagingBiomarkers/0_1s20S1076633217304191.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

wCVˆ2=∑Ni=1{(Yi1−Yi2)2/(2Y¯¯¯2i)}/N.
w

C

V

^

2

=

∑

i

=

1

N

{

(

Y

i

1

−

Y

i

2

)

2

/

(

2

Y

¯

i

2

)

}

/

N

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

%RCˆ=1.96×2wCVˆ2−−−−−−√
%

R

C

^

=

1.96

×

2

w

C

V

^

2


and the symmetric cut-points are defined as Approach 2 in  Table 2 . Note that _%RC_ could be used to define a cut-point for the percentage change from baseline ( %dˆb
%

d

^

b
) or for the percentage difference ( %dˆmean
%

d

^

mean
). These are presented as Approaches 2A and 2B in  Table 2 , respectively.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σˆ2ln=∑Ni=1{ln(Yi1)−ln(Yi2)}2/2N.
σ

^

ln

2

=

∑

i

=

1

N

{

ln

(

Y

i

1

)

−

ln

(

Y

i

2

)

}

2

/

2

N

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

RCˆln=1.96×2σˆ2ln−−−−√.
R

C

^

ln

=

1.96

×

2

σ

^

ln

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

RClnlower=(exp(−RCˆln)−1)andRClnupper=(exp(+RCˆln)−1).
R

C

ln

lower

=

(

exp

(

−

R

C

^

ln

)

−

1

)

and

R

C

ln

upper

=

(

exp

(

+

R

C

^

ln

)

−

1

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## QIB Repeatability Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Assessment of the Distribution of Intra-Subject Repeated Measurements


QIB Setting No. of Observations Distribution for Intra-Subject Replicates Magnetic resonance imaging T1 values Phantom study with replicate scans of each target 15 replicates per target Close to normally distributed except for targets at low T1 values where there's clustering at the minimum values Ultrasound shear wave speed Phantom study with replicate scans of each target 10 replicates per target Close to normally distributed Magnetic resonance elastography values Clinical study with 1 scan per subject, evaluated by multiple algorithms 10 replicates per subject Close to normally distributed except for subjects with low values where there is clustering at these low values Computed tomography acetabular angle Clinical study with 1 scan per patient, interpreted by multiple readers 4 replicates per subject Close to normally distributed

QIB, quantitative imaging biomarker.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Monte Carlo Simulation Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Five Scenarios for Monte Carlo Simulation


Scenario Description Distribution of True Value of Biomarker  \\*  Distribution of Replicate Measurements within Subject  †  1 QIB with constant wSD and normally distributed replicates_X_ ~ _N_ (100, 100) ε ~ _N_ (0,100) 2 QIB with constant wSD and log-normally distributed replicates_X_ ~ _N_ (100, 100) ε = exp( _Z_ ), where _Z_ ~ _N_ (0,10) 3 QIB with clustering at one extreme  ‡ _X_ ~ _N_ (10, 100) ε ~ _N_ (0,100), but values less than zero were set to zero 4 QIB with constant wCV and normally distributed replicates_X_ ~ _N_ (20, 10) ε ~ _N_ (0,σ  2  ), with σ increasing with true biomarker value: σ=(0.1)×(X)
σ

=

(

0.1

)

×

(

X

)
5 QIB where wSD is larger for both small and large values of QIB  § _X_ ~ _N_ (20, 10) ε ~ _N_ (0,σ  2  ), with σ  2  = 100 for _X_ < 17 or >23; otherwise σ  2  = 20 and values less than zero were set to zero

QIB, quantitative imaging biomarker; wCV, within-subject coefficient of variation; wSD, within-subject standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

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


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Coverage of the RC range when no true change in the subject has occurred. The different statistical methods for calculating RC described in the section Defining Change are illustrated in green (Approach 1), shades of red (Approaches 2A and 2B), and shades of blue (Approaches 3A and 3B). The nominal coverage is 95%. The repeatability metrics were estimated from technical performance studies of N = 35. The five scenarios are as follows: 1 = constant wSD with normally distributed replicates; 2 = constant wSD with log-normally distributed replicates; 3 = clustering of values at one extreme where the imaging system is unable to measure; 4 = constant wCV with normally distributed replicates; and 5 = wSD “sweet spot” in the mid-range with large wSD at both extremes. RC, repeatability coefficient; wCV, within-subject coefficient of variation; wSD, within-subject standard deviation. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InterpretingChangeinQuantitativeImagingBiomarkers/1_1s20S1076633217304191.jpg)

![Figure 3, Coverage of the RC range when no true change in the subject has occurred. RC was estimated from technical performance studies with N = 100. The different statistical methods for estimating RC described in the section Defining Change are illustrated in green , shades of red , and shades of blue , respectively. The nominal coverage is 95%. RC, repeatability coefficient. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InterpretingChangeinQuantitativeImagingBiomarkers/2_1s20S1076633217304191.jpg)

![Figure 4, Proportion of subjects falling outside the RC range when a true increase in the biomarker has occurred. RC was estimated from technical performance studies with N = 35. The different statistical methods for estimating RC are illustrated in green , shades of red , and shades of blue , respectively. RC, repeatability coefficient. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InterpretingChangeinQuantitativeImagingBiomarkers/3_1s20S1076633217304191.jpg)

![Figure 5, Proportion of subjects falling outside the RC range when a true decrease in the biomarker has occurred. RC was estimated from technical performance studies with N = 35. The different statistical methods for estimating RC are illustrated in green , shades of red , and shades of blue , respectively. Note that for Scenario 3, Approach 3a demonstrated power slightly over 50%. RC, repeatability coefficient. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InterpretingChangeinQuantitativeImagingBiomarkers/4_1s20S1076633217304191.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Scenario 1: Constant wSD and Normally Distributed Replicates

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Scenario 2: Constant wSD and Log-Normally Distributed Replicates

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Scenario 3: Clustering of Values at One Extreme

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Scenario 4: Constant wCV and Normally Distributed Replicates

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Scenario 5: “Sweet-Spot” with High wSD at Each End and Normally Distributed Replicates

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

RCˆlower=Za×2σˆ2−−−√RCˆupper=Zb×2σˆ2−−−√.
R

C

^

lower

=

Z

a

×

2

σ

^

2

R

C

^

upper

=

Z

b

×

2

σ

^

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σˆ2i=bo+b1(Y¯¯¯i),
σ

^

i

2

=

b

o

+

b

1

(

Y

¯

i

)

,


where the estimated within-subject variance of subject _i_ is a function of the mean of the measurements from subject _i_ . A quadratic term could also be added and tested using ordinary least squares regression. The estimated regression coefficients, bˆo
b

^

o
and bˆ1
b

^

1
, are then used to define dynamic cut-points, that is, cut-points that vary with a future subject's baseline measurement. For example, for the _i_ th future subject, the cut-point associated with 95% confidence is then


RCˆdynamic=1.96×2(bˆo+bˆ1Yib)−−−−−−−−−−−√,
R

C

^

dynamic

=

1.96

×

2

(

b

^

o

+

b

^

1

Y

i

b

)

,


where bˆo
b

^

o
and bˆ1
b

^

1
are estimated from a technical performance study of a biomarker's repeatability, _Y  ib_ is the baseline measurement for future subject _i_ . When we evaluated this approach in our Monte Carlo simulation study with _N_ = 35, this model approach did not have nominal coverage, with coverage of only 89%–92%. With a larger sample size ( _N_ = 100), the coverage improved somewhat but it did not reach the nominal level. Thus, this sort of approach might be extremely useful for QIBs but much larger technical performance studies than are typically performed now would be needed.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Radiological Society of North America (RSNA) : Quantitative Imaging Biomarkers Alliance. Available at: www.rsna.org/QIBA/ Accessed November 20, 2017


- 2\. Sullivan D.C., Obuchowski N.A., Kessler L.G., et. al.: Metrology standards for quantitative imaging biomarkers. Radiology 2015; 277: pp. 813-825.


- 3\. Raunig D., McShane L.M., Pennello G., et. al.: Quantitative imaging biomarkers: a review of statistical methods for technical performance assessment. Stat Methods Med Res 2015; 24: pp. 27-67.


- 4\. Obuchowski N.A., Reeves A.P., Huang E.P., et. al.: Quantitative imaging biomarkers: a review of statistical methods for computer algorithm comparisons. Stat Methods Med Res 2015; 24: pp. 68-106.


- 5\. Barnhart H.X., Barboriak D.P.: Applications of the repeatability of quantitative imaging biomarkers: a review of statistical analysis of repeat data sets. Transl Oncol 2009; 2: pp. 231-235.


- 6\. QIBA : CT Tumor Volumetry for Advanced Disease. Available at: http://qibawiki.rsna.org/index.php/Profiles Accessed November 20, 2017


- 7\. Obuchowski N.A., Bullen J.: Quantitative imaging biomarkers: effect of sample size and bias on confidence interval coverage. Stat Methods Med Res 2017; In press


- 8\. Bland J.M., Altman D.G.: Measuring agreement in method comparison studies. Stat Methods Med Res 1999; 8: pp. 135-160.


- 9\. Weber W.A., Gatsonis C.A., Mozley P.D., et. al.: Repeatability of  18  F-FDG PET/CT in advanced non-small cell lung cancer: prospective assessment in 2 multicenter trials. J Nucl Med 2015; 56: pp. 1137-1143.


- 10\. Winfield J.M., Tunariu N., Rata M., et. al.: Extracranial soft-tissue tumors: repeatability of apparent diffusion coefficient estimates from diffusion-weighted MR imaging. Radiology 2017; 284: pp. 88-99.


- 11\. Obuchowski N.A., Barnhart H.X., Buckler A.J., et. al.: Statistical issues in the comparison of quantitative imaging biomarker algorithms using pulmonary nodule volume as an example. Stat Methods Med Res 2015; 24: pp. 107-140.


- 12\. Lodge M.: Repeatability of SUV in oncologic  18  F-FDG PET. J Nucl Med 2017; 58: pp. 523-532.