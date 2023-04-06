---
title: Statistical Power Considerations for a Utility Endpoint in Observer Performance Studie s
author: [Craig K. Abbey PhD,Frank W. Samuelson PhD,Bron D. Gallas PhD]
date: 2013-07-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 20, Issue 7 SOURCE CL_S_AcademicRadiologyVolume20Issue7 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The purpose of this investigation is to compare the statistical power of the most common measure of performance for observer performance studies, area under the ROC curve (AUC), to an expected utility (EU) endpoint.

## Materials and Methods

We have modified a well-known simulation procedure developed by Roe and Metz for statistical power analysis in receiver operating characteristic (ROC) studies. Starting from a set of baseline simulations, we investigate the effects of three parameters that describe properties of the observers (iso-utility slope, unequal variance, and tendency to favor more aggressive or conservative actions) and three parameters that affect experimental design (number of readers, number of cases, and fraction of positive cases).

## Results

The EU endpoint generally has good statistical power relative to AUC in our simulations. Of 396 total conditions simulated, EU had higher statistical power in 377 cases (95%). In 246 of these cases, EU power was 5 percentage points or more higher than AUC. In simulation runs evaluating the effect of the number of readers and cases on the baseline simulations, EU measure had equivalent power to AUC with fewer readers (9% to 28%) or fewer cases (18% to 41%).

## Conclusion

These simulation studies provide further motivation for considering EU in studies of screening mammography technology and they motivate investigations of utility in other diagnostic tasks.

Decisions have consequences. This truism is particularly applicable to medical decisions that affect the health and well-being of patients as well as the financial cost of care to payers. In this context, diagnostic medical imaging technology can be categorized as providing support for medical decision-making. It is widely recognized that the evaluation of diagnostic medical imaging technology should represent its effect on decision-making performance in addition to physical measurements of fundamental imaging characteristics (noise, resolution, contrast). The medical imaging community generally expects that proponents of new techniques will use some measure of observer performance as an endpoint of validation studies. For example, the United States Food and Drug Administration routinely asks manufacturers of medical imaging technology to provide reasonable assurance that a device is effective through observer performance metrics .

In many cases of interest, technology can be assessed in the framework of a binary task. In such cases, receiver operating characteristic (ROC) analysis is a well-established method to characterize the effect of technology on diagnostic ability . The ROC curve plots the tradeoff between the true-positive fraction (TPF also referred to as sensitivity) and the false positive fraction (FPF, also 1 - Specificity). However, to be useful for quantitative comparisons, a summary value must be extracted from the ROC curve as a figure of merit indicating the level of performance. In the field of medical imaging, that number has most commonly been the area under the ROC curve (AUC) . AUC has an intuitive interpretation as the average sensitivity over all possible specificities as well as the probability that a randomly chosen example from the population with disease will be detected over a randomly chosen example from the normal (nondiseased) population . But AUC does not account for the prevalence of disease or the consequences of decisions, which both factor heavily in clinical decisions.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## A Roe and Metz Type Simulation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## AUC and Utility Endpoints

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

EU=Max(FPF,TPF)∈ROC(TPF−βFPF),
EU

=

Max

(

F

P

F

,

T

P

F

)

∈

R

O

C

(

TPF

−

β

FPF

)

,


where (FPF,TPF)∈ROC
(

FPF

,

TPF

)

∈

ROC
indicates all points on the ROC curve. The quantity, TPF− _β_ FPF, can be thought of as the _y_ intercept of a line with slope _β_ that passes through the point (FPF, TPF). It can also be considered a FPF “corrected” sensitivity, where _β_ scales the penalty associated with the given false-positive rate. In either case, the figure of merit consists of maximizing this value over all possible points on the ROC curve. Because the maximal value is found when the line is tangent to a smooth ROC curve, _β_ is often referred to as the ROC slope. Utility theory suggests that this value should be determined by the four possible outcome utilities and by the prevalence of disease. In this case, lines of slope _β_ may be considered iso-utility lines, and the _y_ intercept can be related to the total utility of the decision process.  Figure 1 shows graphically how EU endpoints are derived from hypothetical ROC data.

![Figure 1, A comparison of two hypothetical systems. Observed categorical data are used to fit receiver operating characteristic (ROC) curves from which figures of merit for performance are obtained. Area under the ROC curve (AUC) is one such figure of merit (AUC = 0.84 for modality 1 and 0.90 for modality 2). The expected utility (EU) measure is obtained from the y -intercept of an iso-utility line tangent to each curve (EU 1 = 0.55 for modality 1 and EU 2 = 0.70 for modality 2).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalPowerConsiderationsforaUtilityEndpointinObserverPerformanceStudies/0_1s20S1076633213001153.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Scope of Studies

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Default Simulation Parameters


Effect Label or Parameter Default Roe and Metz variance structure LL, LH, HL, and HH See reference  Level of performance Low, mid, and high AUC = 0.70, 0.86, or 0.96 Iso-utility slope_β_ 1.03  ∗  Categorization bias_B_ 1 Mean-to-sigma ratio_r_ 4 Fraction of positive cases_F__C_ 0.5 Number of cases_N__C_ 200 Number of readers_N__R_ 8

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Power as a function of modality differences. Observed statistical power is plotted from the modified Roe and Metz simulation with high-high components of variance structure and mid-level difficulty. Two modalities are assumed, with the difference in modality effects leading to increased power in detecting the better modality ( Δt=t2,1−t1,1 Δt=t2,1−t1,1 , where t i ,1 is the abnormal modality term from Eq 1 ). Power for both expected utility (EU) (iso-utility slope of 1.03) and area under the curve (AUC) endpoints are plotted. The reference point where AUC achieves 80% power is shown as well ( dashed vertical line ). Note that both endpoints are near the nominal rejection rate of 5% when Δt=0 Δt=0 . Near 80% power, the EU endpoint is uniformly higher than AUC.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalPowerConsiderationsforaUtilityEndpointinObserverPerformanceStudies/1_1s20S1076633213001153.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Power as a function of observer effects. Observed power in the high-high variance structure of the modified RM simulation is shown for parameters that describe the observer. The slope parameter, b , used to compute expected utility (EU) (a) only affects utility, leaving all area under the curve (AUC) power at the targeted level of 80%. The effect of unequal variance (b) as implemented in the mean-to-sigma ratio and categorization disposition (c) both remain relatively constant across parameter values. The legend in (b) also applies to (c) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalPowerConsiderationsforaUtilityEndpointinObserverPerformanceStudies/2_1s20S1076633213001153.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Power as a function of experimental design effects. Observed power in the modified Roe and Metz simulations (high-high variance structure) is shown as a function of experimental design parameters. These include the number of readers (a) , the number of cases (b) and the relative number of positive cases (c) . The legend applies to all plots. FPF, false positive fraction; TPF, true positive fraction.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalPowerConsiderationsforaUtilityEndpointinObserverPerformanceStudies/3_1s20S1076633213001153.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation Model and Components of Variance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Xi,j,k,t=μt+τi,t+Rj,t+Ck,t+(τR)i,j,t+(τC)i,k,t+(RC)j,k,t+Ei,j,k,t.
X

i

,

j

,

k

,

t

=

μ

t

+

τ

i

,

t

+

R

j

,

t

+

C

k

,

t

+

(

τ

R

)

i

,

j

,

t

+

(

τ

C

)

i

,

k

,

t

+

(

R

C

)

j

,

k

,

t

+

E

i

,

j

,

k

,

t

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Unequal Variance Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Var(Xi,j,k,t\|t)=w2i,t(σ2R+σ2C+σ2τR+σ2τC+σ2RC+σ2E),
Var

(

X

i

,

j

,

k

,

t

\|

t

)

=

w

i

,

t

2

(

σ

R

2

+

σ

C

2

+

σ

τ

R

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

E

2

)

,


where _w__i_ , _t_ ( _t_ = 0,1) is a positive truth-dependent weight for each modality that applies to all random effects. The weights are constrained to achieve an MSR of 4 and a combined magnitude of w2i,0+w2i,1=2
w

i

,

0

2

+

w

i

,

1

2

=

2
, which can be made consistent with the original RM model by setting _w__i_ ,0 = _w__i_ ,1 = 1\. Based on Equation  A1 , difference in means in a given modality ( _i_ ) and averaged across readers can be written


Δmi=μ1+τi,1.
Δ

m

i

=

μ

1

+

τ

i

,

1

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δσi=(wi,1−wi,0)σ2C+σ2τC+σ2RC+σ2E−−−−−−−−−−−−−−−−−√.
Δ

σ

i

=

(

w

i

,

1

−

w

i

,

0

)

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

E

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δσi=wi,1−wi,0.
Δ

σ

i

=

w

i

,

1

−

w

i

,

0

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

wi,0=−Δmi2r+1−(Δmi2r)2−−−−−−−−−−√.wi,1=wi,0+Δmir
w

i

,

0

=

−

Δ

m

i

2

r

+

1

−

(

Δ

m

i

2

r

)

2

.

w

i

,

1

=

w

i

,

0

+

Δ

m

i

r


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Generating Discrete Ratings

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

−∞=ci,0<ci,1<ci,2<⋯<ci,N−1<ci,N=∞,
−

∞

=

c

i

,

0

<

c

i

,

1

<

c

i

,

2

<

⋯

<

c

i

,

N

−

1

<

c

i

,

N

=

∞

,


in which only the central _N_ −1 categorical boundaries ( _c__i_ , _n_ , _n_ = 1,…, _N_ −1) need to be determined. Once these have been set (as described next), the rating data are determined from the decision variables to be


Ri,j,k,t=∑Nn=1nI(Xi,j,k,t;ci,n−1,ci,n),
R

i

,

j

,

k

,

t

=

∑

n

=

1

N

n

I

(

X

i

,

j

,

k

,

t

;

c

i

,

n

−

1

,

c

i

,

n

)

,


where the indicator function _I_ is defined as


I(X;cLow,cHigh)={10ifcLow<X≤cHighOtherwise.
I

(

X

;

c

Low

,

c

High

)

=

{

1

if

c

Low

<

X

≤

c

High

0

Otherwise

.


The indicator functions in Equation  A8 cause the elements of the sum to be zero except for the “bin” that contains the decision variable, and the index element ensures that the correct rating value is assigned.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Pi(c)=(1−FC)Φ(cwi,0)+FCΦ(c−Δmiwi,1),
P

i

(

c

)

=

(

1

−

F

C

)

Φ

(

c

w

i

,

0

)

+

F

C

Φ

(

c

−

Δ

m

i

w

i

,

1

)

,


where Φ is the cumulative normal distribution function (note this also assumes the remaining components of variance sum to one). We determine categorical thresholds by solving


Pi(ci,n)=(nN)B
P

i

(

c

i

,

n

)

=

(

n

N

)

B


for _c__i_ , _n_ , which can be accomplished numerically to arbitrary precision. The exponent, _B_ , is a positive categorization disposition parameter that controls where the thresholds appear on an ROC curve. We will consider the thresholds to be at baseline when _B_ = 1\. In this case, decision variables are equally spread among the categorical scores. Higher values of _B_ lead to reduced categorization thresholds, which assigns more decision variables to higher scores. This moves the categorical operating points towards the upper right corner of the ROC curve. Conversely, lower values of _B_ increase the categorization thresholds, which then move the observed operating points toward the lower left corner of the ROC curve. Effects of categorization disposition are shown in  Figure A1 .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Figures of Merit

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TPF=aFPF+(1−a)(1−Φ\[cFPF−u\]),
TPF

=

a

FPF

+

(

1

−

a

)

(

1

−

Φ

\[

c

FPF

−

u

\]

)

,


where _c_ FPF is the criterion associated with a given FPF value (ie,cFPF=Φ−1\[1−FPF\])
(

ie

,

c

FPF

=

Φ

−

1

\[

1

−FPF

\]

)
. The AUC is readily computed from the CBM parameters as


AUC=a2+(1−a)Φ(u2√).
AUC

=

a

2

+

(

1

−

a

)

Φ

(

u

2

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FPFOOP=1−Φ\[1uln(β−a1−a)−12u\],
FP

F

OOP

=

1

−

Φ

\[

1

u

ln

(

β

−

a

1

−

a

)

−

1

2

u

\]

,


if _β_ \> _a_ , and _a_ < 1\. The TPF at the optimal operating point, TPF  OOP , is obtained by evaluating Equation  A12 at FPF  OOP . If _β_ ≤ _a_ , then the optimum point of the ROC curve is (FPF  OOP , TPF  OOP ) = (1,1). If _a_ = 1 or _u_ = 0 (in either case performance is at chance), then (FPF  OOP , TPF  OOP ) = (0,0) if _β >_ 1, and (FPF  OOP , TPF  OOP ) = (1,1) if _β <_ 1\. The expected utility figure of merit, EU, is then


EU=TPFOOP−βFPFOOP.
EU

=

TP

F

OOP

−

β

FP

F

OOP

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Power Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure A1, Effects of the threshold bias parameter. Simulation of a single reader in a single modality is shown. A set of decision variables generated according to Equation A1 was discretized to a 7-point rating using different values of the categorization disposition parameter, B . As this parameter is increased ( a . to c .), the operating points of the categorical data move from the lower left region of the curve toward the upper right . The theoretical curve describing the decision variables is also plotted. The different categorization thresholds lead to some variation in the estimated receiver operating characteristic (ROC) curves.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/StatisticalPowerConsiderationsforaUtilityEndpointinObserverPerformanceStudies/4_1s20S1076633213001153.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Gallas B.D., Chan H.P., D'Orsi C.J., et. al.: Evaluating imaging and computer-aided detection and diagnosis devices at the FDA. Acad Radiol 2012; 19: pp. 463-477.


- 2\. Metz C.E.: Basic principles of ROC analysis. Semin Nucl Med 1978; 8: pp. 283-298.


- 3\. Metz C.E.: ROC analysis in medical imaging: a tutorial review of the literature. Radiol Phys Technol 2008; 1: pp. 2-12.


- 4\. Obuchowski N.A.: ROC analysis. AJR Am J Roentgenol 2005; 184: pp. 364-372.


- 5\. Swets J.A., Pickett R.M.: Evaluation of diagnostic systems: methods from signal detection theory.1982.Academic PressNew York


- 6\. Bamber D.: The area above the ordinal dominance graph and the area below the receiver operating characteristic graph. J Math Psychol 1975; 12: pp. 387-415.


- 7\. Hanley J.A., McNeil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 8\. Metz C.E.: ROC methodology in radiologic imaging. Invest Radiol 1986; 21: pp. 720-733.


- 9\. Hanley J.A.: Receiver operating characteristic (ROC) methodology: the state of the art. Crit Rev Diagnostic Imaging 1989; 29: pp. 307.


- 10\. Green D.M., Swets J.A.: Signal detection theory and psychophysics.1966.WileyNew York


- 11\. Peterson W., Birdsall T., Fox W.: The theory of signal detectability. IRE Professional Group on Information Theory 1954; 4: pp. 171-212.


- 12\. Tanner W.P., Swets J.A.: A decision-making theory of visual detection. Psychol Rev 1954; 61: pp. 401-409.


- 13\. Pauker S.G., Kassirer J.P.: Therapeutic decision making: a cost-benefit analysis. N Engl J Med 1975; 293: pp. 229-234.


- 14\. Hilden J.: The area under the ROC curve and its competitors. Med Decis Making 1991; 11: pp. 95-101.


- 15\. Moons K.G., Stijnen T., Michel B.C., et. al.: Application of treatment thresholds to diagnostic-test evaluation: an alternative to the comparison of areas under receiver operating characteristic curves. Med Decis Making 1997; 17: pp. 447-454.


- 16\. Schisterman E.F., Perkins N.J., Liu A., et. al.: Optimal cut-point and its corresponding Youden Index to discriminate individuals using pooled blood samples. Epidemiology 2005; 16: pp. 73-81.


- 17\. Schwartz W.B., Gorry G.A., Kassirer J.P., et. al.: Decision analysis and clinical judgment. Am J Med 1973; 55: pp. 459-472.


- 18\. Lusted L.B.: Introduction to medical decision making.1968.C ThomasSpringfield, IL


- 19\. Weinstein M.C., Fineberg H.V., Elstein A.S., et. al.: Clinical decision analysis.1980.SaundersPhiladelphia, PA


- 20\. Sunshine J.: Contributed comment. Acad Radiol 1995; 2: pp. S72-S74.


- 21\. Halpern E.J., Albert M., Krieger A.M., et. al.: Comparison of receiver operating characteristic curves on the basis of optimal operating points. Acad Radiol 1996; 3: pp. 245-253.


- 22\. Wagner R.F., Beam C.A., Beiden S.V.: Reader variability in mammography and its implications for expected utility over the population of readers and cases. Med Decis Making 2004; 24: pp. 561-572.


- 23\. Abbey C.K., Eckstein M.P., Boone J.M.: An equivalent relative utility metric for evaluating screening mammography. Med Decis Making 2010; 30: pp. 113-122.


- 24\.  Abbey CK, Eckstein MP, Boone JM. Estimating the relative utility of screening mammography. In Press: Medical Decision Making.


- 25\. Roe C.A., Metz C.E.: Dorfman-Berbaum-Metz method for statistical analysis of multireader, multimodality receiver operating characteristic data: validation with computer simulation. Acad Radiol 1997; 4: pp. 298-303.


- 26\. Dorfman D.D., Berbaum K.S., Metz C.E.: Receiver operating characteristic rating analysis. Generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 27\. Roe C.A., Metz C.E.: Variance-component modeling in the analysis of receiver operating characteristic index estimates. Acad Radiol 1997; 4: pp. 587-600.


- 28\. Beiden S.V., Wagner R.F., Campbell G., et. al.: Components-of-variance models for random-effects ROC analysis: the case of unequal variance structures across modalities. Acad Radiol 2001; 8: pp. 605-615.


- 29\. Metz C.E., Kronman H.B.: Statistical significance tests for binormal ROC curves. J Math Psychol 1980; 22: pp. 218-243.


- 30\. Swets J.A.: Form of empirical ROCs in discrimination and diagnostic tasks: implications for theory and measurement of performance. Psychol Bull 1986; 99: pp. 181-198.


- 31\. Hillis S.L.: Simulation of unequal-variance binormal multireader ROC decision data: an extension of the Roe and Metz simulation model. Acad Radiol 2012; 19: pp. 1518-1528.


- 32\. Hillis S.L., Berbaum K.S.: Using the mean-to-sigma ratio as a measure of the improperness of binormal ROC curves. Acad Radiol 2011; 18: pp. 143-154.


- 33\. Dorfman D.D., Berbaum K.S.: A contaminated binormal model for ROC data: part III. Initial evaluation with detection ROC data. Acad Radiol 2000; 7: pp. 438-447.


- 34\. Dorfman D.D., Berbaum K.S.: A contaminated binormal model for ROC data: Part II. A formal model. Acad Radiol 2000; 7: pp. 427-437.


- 35\. Dorfman D.D., Berbaum K.S., Brandser E.A.: A contaminated binormal model for ROC data: part I. Some interesting examples of binormal degeneracy. Acad Radiol 2000; 7: pp. 420-426.


- 36\. Hillis S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.