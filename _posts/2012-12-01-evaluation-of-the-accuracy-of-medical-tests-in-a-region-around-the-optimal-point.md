---
title: Evaluation of the Accuracy of Medical Tests in a Region around the Optimal Point
author: [CL_AT_DonnaKatzmanMcClishPhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 12]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The accuracy of medical tests is often assessed using the area under the entire receiver-operating characteristic (ROC) curve. However, this includes values that might be of no clinical importance. Evaluation of a portion of the curve, or a single point, requires identifying a range of clinical interest, which may not be obvious. The author suggests evaluating the accuracy of medical tests in the vicinity of the optimal point.

## Materials and Methods

Assuming binormality, the author estimated the optimal threshold as the value that maximizes the generalized Youden index. The confidence interval around the optimal point defined a region of clinical interest; the accuracy of the medical test was assessed using the partial area index (PAI) and standardized partial area (sPA). Bootstrapping was used to estimate variances and construct confidence intervals. Coverage probabilities for the PAI and sPA were assessed, as was the size of the test to compare measures. An example using biomechanical measures from radiographic images of the pelvis and lumbar spine to detect disk hernia and spondylolisthesis is presented.

## Results

Coverage probabilities of confidence intervals for the partial area measures were good. The size of the test to compare partial area measures was appropriate. Values of PAI and sPA varied with the cost/prevalence ratio. In the example, the biomechanical measures were not found to have significantly different accuracy around the optimal point.

## Conclusions

The PAI and sPA associated with the optimal point were found to be reasonable and useful measures of accuracy.

Receiver-operating characteristic (ROC) curves are often used in medicine to evaluate the accuracy of medical tests . Using an ROC curve, the accuracy of a medical test can be assessed in a number of ways. A popular measure is the area under the entire ROC curve (AUC). However, this includes false-positive rates (FPRs) that might be of no practical or clinical importance. At the other extreme, one could look at a single point on an ROC curve: the sensitivity or true-positive rate (TPR) at a specific FPR value or threshold. This would require knowing, a priori, a single, appropriate FPR value. A compromise would be to look at the area under a portion of the curve of interest . Again, this would require identifying a range of FPRs of clinical interest. It may not be obvious what a priori single FPR/threshold or range of FPR/threshold values should be chosen.

A good choice of an a priori point to represent the accuracy of a medical test would be the optimal point on an ROC curve. This is the point associated with the best threshold for clinicians to use to dichotomize test results to diagnose disease. Recognizing that there is some uncertainty surrounding the optimal point, rather than simply assessing a medical test at a single optimal point, it would be preferable to consider the AUC in a region near the optimal point. More specifically, this region could be defined by the confidence interval (CI) around the optimal point, that is, the (partial) AUC between the bounds of the CI.

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

GYI(c)=sensitivity(c)+R×specificity(c)−G,
GYI

(

c

)

=

sensitivity

(

c

)

+

R

×

specificity

(

c

)

−

G

,


where _G_ is a constant with respect to _c_ , _R_ = \[(1− _p_ )/ _p_ \]\[( _C_ TN − _C_ FP )/( _C_ TP − _C_ FN )\], _p_ is the prevalence of disease, and _C_ TN , _C_ FP , _C_ TP , and _C_ FN represent the costs of true-negative, false-positive, true-positive, and false-negative findings, respectively .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

PAI=pAUC/Amn,
PAI

=

pAUC

/

Amn

,


and


sPA=12(1+pAUC−AmnAmx−Amn),
sPA

=

1

2

(

1

+

pAUC

−

A

mn

A

mx

−

A

mn

)

,


where _A_ mn = FPR  U −FPR  L is the minimum value for the partial area, and the maximum value is _A_ mx = (FPR  U −FPR  L )(FPR  U \+ FPR  L )/2\. Although the PAI is more commonly used, the sPA should be more useful to the researcher in terms of interpretation, as its value reflects the same scale as the total area.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Z=A∗1−A∗2Var(A∗1−A∗2)√,
Z

=

A

1

∗

−

A

2

∗

Var

(

A

1

∗

−

A

2

∗

)

,


where A∗i
A

i

∗
is the PAI or sPA for the _i_ th medical test ( _i_ = 1, 2). Variance of the difference was estimated by bootstrapping the differences. To show that the statistical test is valid, it was checked that when the partial area measures were not different, the _Z_ -test statistic would exceed 1.96 only approximately 5% of the time (called the size of the test).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Effect of area under the receiver-operating characteristic curve (AUC) and binormal parameter b on the value of the partial area index (PAI) and the standardized partial area (sPA) at the optimal point ( R = 1).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationoftheAccuracyofMedicalTestsinaRegionaroundtheOptimalPoint/0_1s20S1076633212004667.jpg)

![Figure 2, Effect of area under the receiver-operating characteristic curve (AUC) and sample size ( n ) on the coverage probabilities of the confidence interval around the partial area index (PAI) and the standardized partial area (sPA) at the optimal point ( R = 1).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationoftheAccuracyofMedicalTestsinaRegionaroundtheOptimalPoint/1_1s20S1076633212004667.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Effect of area under the receiver-operating characteristic curve (AUC), sample size (n), and binormal parameter b on the size of the test to compare two partial area index (PAI) or standardized partial area (sPA) values at the optimal point ( R = 1).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationoftheAccuracyofMedicalTestsinaRegionaroundtheOptimalPoint/2_1s20S1076633212004667.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Effect of area under the receiver-operating characteristic curve (AUC) and R on the value of the partial area index (PAI) and the standardized partial area (sPA) at the optimal point ( b = 1, n = 100).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationoftheAccuracyofMedicalTestsinaRegionaroundtheOptimalPoint/3_1s20S1076633212004667.jpg)

![Figure 5, Effect of area under the receiver-operating characteristic curve (AUC) and R on the coverage probabilities of the confidence interval around the partial area index (PAI) and the standardized partial area (sPA) at the optimal point ( b = 1, n = 100).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationoftheAccuracyofMedicalTestsinaRegionaroundtheOptimalPoint/4_1s20S1076633212004667.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

x∗=xλ−1λ,λ≠0orx∗=log(x),λ=0.
x

∗

=

x

λ

−

1

λ

,

λ

≠

0

or

x

∗

=

log

(

x

)

,

λ

=

0.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Analysis of Accuracy of Biomechanical Pelvic and Lumbar Measures around the Optimal Point


Measure Pelvic Incidence Lumbar Lordosis Angleμˆ∗D
μ

ˆ

D

∗
7.262 12.714σˆ∗D
σ

ˆ

D

∗
0.797 2.688μˆ∗H
μ

ˆ

H

∗
6.670 11.069σˆ∗H
σ

ˆ

H

∗
0.625 1.846 AUC 0.720 0.693 R = 0.5 c\* (original units) 44.2 32.3 Optimal point (FPR, TPR) (0.715, 0.883) (0.822,0.894) PAI (95% CI) 0.877 (0.859–0.897) 0.880 (0.860–0.897) sPA (95% CI) 0.791 (0.709–0.866) 0.709 (0.560–0.837) R = 1.0 c\* (original units) 56.5 48.2 Optimal point (FPR, TPR) (0.318, 0.645) (0.328, 0.620) PAI (95% CI) 0.654 (0.604–0.688) 0.621 (0.582–0.660) sPA (95% CI) 0.739 (0.689–0.789) 0.717 (0.664–0.769) R = 2.0 c\* (original units) 71.2 67.4 Optimal point (FPR, TPR) (0.065, 0.328) (0.035, 0.263) PAI (95% CI) 0.354 (0.252–0.459) 0.314 (0.230–0.402) sPA (95% CI) 0.649 (0.594–0.704) 0.634 (0.589–0.683)

AUC, area under the receiver-operating characteristic curve; CI, confidence interval; FPR, false-positive rate; μˆ∗
μ

ˆ

∗
, estimated mean of the transformed data; PAI, partial area index; σˆ∗
σ

ˆ

∗
, estimated standard deviation of the transformed data; sPA, standardized partial area; TPR, true-positive rate.


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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A

## Formulas for the Optimal Threshold

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

c∗=μHσ2D−μDσ2H+σHσD(μD−μH)2+2(σ2D−σ2H)\[ln(RσH/σD)\]√σ2D−σ2H
c

∗

=

μ

H

σ

D

2

−

μ

D

σ

H

2

+

σ

H

σ

D

(

μ

D

−

μ

H

)

2

+

2

(

σ

D

2

−

σ

H

2

)

\[

ln

(

R

σ

H

/

σ

D

)

\]

σ

D

2

−

σ

H

2


when σ  H ≠ σ  D and


c∗=σ2ln(R)μD−μH+μD+μH2
c

∗

=

σ

2

ln

(

R

)

μ

D

−

μ

H

+

μ

D

+

μ

H

2


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix B

## Partial Area Around the Optimal Point

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pAUC=∫FPRLFPRUΦ\[a+bΦ−1(x)\]dx,
pAUC

=

∫

FPR

L

FPR

U

Φ

\[

a

+

b

Φ

−

1

(

x

)

\]

d

x

,


where “ _a_ ” and “ _b_ ” are the usual binormal parameters, defined as _a_ = (μ  D − μ  H )/σ  D and _b_ = σ  H /σ  D , and Φ represents the cumulative normal distribution function and Φ  −1 is its inverse. For the pAUC corresponding to the confidence interval of the optimal point, the limits of integration would be the bounds of the confidence interval:


(FPRL,FPRU)={1−Φ\[(c∗−zα/2Var(c∗)−−−−−−−√−μH)/σH\],1−Φ\[(c∗+zα/2Var(c∗)−−−−−−−√−μH)/σH\]}.
(

FPR

L

,

FPR

U

)

=

{

1

−

Φ

\[

(

c

∗

−

z

α

/

2

Var

(

c

∗

)

−

μ

H

)

/

σ

H

\]

,

1

−

Φ

\[

(

c

∗

+

z

α

/

2

Var

(

c

∗

)

−

μ

H

)

/

σ

H

\]

}

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Metz C.E.: Basic principles of ROC analysis. Semin Nucl Med 1978; 8: pp. 283-298.


- 2\. Zweig M.H., Campbell G.: Receiver-operating characteristic plots: a fundamental evaluation tool of clinical medicine. Clin Chem 1993; 39: pp. 561-577.


- 3\. Greiner M., Pfieffer D., Smith R.D.: Principles and practical applications of the receiver- operating characteristic analysis for diagnostic tests. Prev Vet Med 2000; 45: pp. 23-41.


- 4\. McClish D.K.: Analyzing a portion of the ROC curve. Med Decis Making 1989; 9: pp. 190-195.


- 5\. Jiang Y., Metz C.E., Nishidawa R.M.: A receiver operating characteristic partial area index for highly sensitive diagnostic tests. Radiology 1996; 201: pp. 745-750.


- 6\. Wieand S., Gail M.H., James B.R., et. al.: A family of nonparametric statistics for comparing diagnostic markers with paired or unpaired data. Biometrika 1989; 76: pp. 585-592.


- 7\. Dwyer A.J.: In pursuit of a piece of the ROC. Radiology 1997; 202: pp. 621-625.


- 8\. Thompson M.L., Zucchini W.: On the statistical analysis of ROC curves. Stat Med 1989; 8: pp. 1277-1290.


- 9\. Halpern E.J., Albert M., Krieger A.M., et. al.: Comparison of receiver operating characteristic curves on the basis of optimal operating points. Acad Radiol 1996; 3: pp. 245-253.


- 10\. Jund J., Rabilloud M., Wallon M., et. al.: Methods to estimate the optimal threshold for normally or log-normally distributed biological tests. Med Decis Making 2005; 25: pp. 406-515.


- 11\. Skaltsa K., Jover L., Carrasco J.L.: Estimation of the diagnostic threshold accounting for decision costs and sampling uncertainty. Biometr J 2010; 52: pp. 676-697.


- 12\. Remally A.T., Sampson M.L., DeLeo J.M., et. al.: Prevalence-value-accuracy plots: a new method for comparing diagnostic tests based on misclassification costs. Clin Chem 1999; 45: pp. 934-941.


- 13\. Cantor S.B., Sun C.C., Tortolero-Luna G., et. al.: A comparison of C/B ratios using receiver operating characteristic curve analysis. J Clin Epidemiol 1999; 52: pp. 885-892.


- 14\. Fluss R., Faraggi D., Reiser B.: Estimation of the Youden index and its associated cutoff point. Biom J 2005; 47: pp. 458-472.


- 15\. Schisterman E.F., Perkins N.J.: Confidence intervals for the Youden index and corresponding optimal cut-point. Commun Stat Simul Comput 2007; 36: pp. 549-563.


- 16\.  Frank A, Asuncion A. UCI Machine Learning Repository. Available at:  http://archive.ics.uci.edu/ml  . Accessed September 27, 2012.


- 17\. Somoza E., Mossman D.: “Biological markers” and psychiatric diagnosis: risk-benefit balancing using ROC analysis. Biol Psychiatry 1991; 29: pp. 811-826.


- 18\. Berthonnaud E., Dimnet J., Roussouly P., et. al.: Analysis of the sagittal balance of the spine and pelvis using shape and orientation parameters. J Spinal Disord Tech 2005; 18: pp. 40-47.


- 19\. Somoza E., Mossman D.: Comparing and optimizing diagnostic tests: an information-theoretical approach. Med Decis Making 1992; 12: pp. 179-188.


- 20\. Faraggi D., Reiser B.: Estimation of the area under the ROC curve. Stat Med 2002; 21: pp. 3093-3106.


- 21\. Dodd L.E., Pepe M.S.: Partial AUC estimation and regression. Biometrics 2003; 59: pp. 614-623.


- 22\. He Y., Escobar M.: Nonparametric statistical inference method for partial areas under receiver operating characteristic curves with application to genomic studies. Stat Med 2008; 27: pp. 361-376.


- 23\. Zhang D.D., Zhou X.H., Freeman D.H., et. al.: A non-parametric method for the comparison of partial areas under ROC curves and its application to large health care data sets. Stat Med 2002; 21: pp. 701-715.


- 24\. Zou K.H., Hall W.J., Shapiro D.E.: Smooth non-parametric receiver operating characteristic (ROC) curves for continuous diagnostic tests. Stat Med 1997; 16: pp. 2143-2156.


- 25\. Baker S.G.: Identifying combinations of cancer markers for further study as triggers of early intervention. Biometrics 2000; 56: pp. 1082-1087.


- 26\. Perkins N.J., Schisterman E.F.: The inconsistency of “optimal” cutpoints obtained using two criteria based on the receiver operating characteristic curve. Am J Epidemiol 2006; 163: pp. 670-675.