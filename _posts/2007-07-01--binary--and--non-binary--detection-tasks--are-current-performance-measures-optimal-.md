---
title: “Binary” and “Non-Binary” Detection Tasks: Are Current Performance Measures Optimal?
author: [David Gur ScD,Howard E. Rockette PhD,Andriy I. Bos PhD]
date: 2007-07-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 7 SOURCE CL_S_AcademicRadiologyVolume14Issue7 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We have observed that a very large fraction of responses for several detection tasks during the performance of observer studies are in the extreme ranges of lower than 11% or higher than 89% regardless of the actual presence or absence of the abnormality in question or its subjectively rated “subtleness.” This observation raises questions regarding the validity and appropriateness of using multicategory rating scales for such detection tasks. Monte Carlo simulation of binary and multicategory ratings for these tasks demonstrate that the use of the former (binary) often results in a less biased and more precise summary index and hence may lead to a higher statistical power for determining differences between modalities.

Observer performance studies have become a widely accepted method of assessing and comparing performance levels of imaging systems and practices when the observer is considered an integral part of the diagnostic system ( ). Many of these studies focus primarily on detection, namely the presence or absence of an abnormality in question, and interpretation tasks, namely the likelihood that if the abnormality is present it is either benign or malignant. In the majority of the “detection” studies a categorical (ordinal) rating scale is implemented to allow observers to rate their relative confidence or suspicion level (probability) that a given predefined abnormality is either present or absent (depicted on the images or not) in the examination being rated ( ). Both receiver operating characteristic (ROC) and free-response ROC (FROC) type ratings and analyses have been used for the purpose of estimating performance curves and for computing summary indices of performance, such as the area under the ROC curve (AUC), and to compare different technologies and practices ( ). Our experience has been that observers often state and behave as if there are at least two distinct types of detection tasks. The one detection task is related to the very well-defined and clearly described abnormality in which high-frequency information (eg, the identification of sharp lines) often is pivotal to the detection task. These abnormalities include, but are not limited to, pneumothorax, rib fracture, the presence of foreign bodies, and some types of interstitial disease. The second type of detection task includes abnormalities that are “less defined” in terms of their appearance on the images and, although these obviously include high-frequency information that may be extremely important for the diagnosis (interpretation), the actual detection is often related to the general shape and contrast distribution of the region of interest. These abnormalities include, but are not limited to, masses, asymmetry, some types of interstitial disease, and occasionally developing or improving subtle alveolar infiltrates.

When a potential abnormality is identified there may be some ambiguity as to whether or not the suspected finding constitutes an actual abnormality depicted on the image or a variation of normal tissue pattern possibly masked by overlapping tissue. The observer then typically uses more deliberately additional background information in the surrounding area and possibly in other comparison images, such as prior examinations, a contralateral view, or a different projection image during the decision making as to whether or not the observed region may represent a true abnormality rather than a variation of negative (“normal”) depiction. In this case, the use of a probability-based rating scale to indicate the confidence level of the observer as to whether or not the abnormality is truly present is clearly reasonable and a quite natural approach. However, in the detection of the well-defined abnormality, the initial identification of the region does not naturally result in a “suspicion level” but rather as a binary observation (namely “I know I see ….”), and once detected, there is little and often no doubt in the observer’s mind about the specific finding. This detection task is primarily a binary event and the outcome for the actually positive subjects is typically a definite “detection” or a complete “miss” rather than a probability based observation. Whether right or wrong, the observer “knows” immediately that he or she “sees” the abnormality in question (eg, pneumothorax, a cluster of microcalcifications) and there is rarely a need for any additional comparative information to confirm the observation. Imposing a confidence level–based rating scale in these well-defined instances is largely a study design issue, and even when observers provide a distribution of confidence ratings, it may be more representative of the subtleness of the depicted abnormality rather than the confidence that the observer actually “saw” or did not “see” it. When the observer detects the abnormality (“sees it”), his or her confidence level is typically extremely high (eg, >89%) and if the abnormality is not detected (“seen”), the confidence level is typically very low (eg, <11%, or a “complete miss”). The question remains whether artificially inducing and later “magnifying” the rating differences, if any, by using a multicategorical scale for the purpose of a performance analysis is a valid (or optimal) approach and more important perhaps, whether the results of these studies are limited in terms of their generalizability to the clinical environment.

In a review of several of our own studies, we note that in the detection of well-defined abnormalities, with the exception of but a few situations, the fraction of cases rated in the two extremes (eg, probabilities <11% or >89%) is very high (typically >90%); as a result, most of the ROC curve represents an extrapolation from few poorly placed data points. An example of the fraction of “extreme” ratings for different abnormalities is presented in  Table 1 . As important perhaps, the number of “complete misses,” namely percent of cases with the abnormality present being rated as not present (ie, likelihood score <11%) and vice versa, is substantially larger when rating well-defined abnormalities. In all of the studies we reviewed, a similar pattern was observed and regardless of the individual’s rating pattern (readers are generally more or less decisive) as well as the subtleness of the cases, the rating distributions for well-defined abnormalities were always “narrower” than that for masses, nodules, or interstitial disease. In general, the tendency to rate very confidently that the abnormality in question is “not present” in negative cases is even stronger than the ratings of positive cases as definitely present ( ).

Table 1


Illustration of the Fraction (%) of Cases Rated by Seven Observers  ⁎

Reader Abnormality Interstitial Disease Nodule Pneumothorax Rib Fracture 1 91% 79% 99% 94% 2 70% 66% 92% 92% 3 64% 86% 95% 95% 4 89% 70% 96% 93% 5 34% 31% 97% 54% 6 34% 29% 89% 83% 7 89% 84% 95% 100% Average 67% 64% 95% 87%

⁎ In an observer performance study with rating scores greater than 89% or less than 11% for four different abnormalities: interstitial disease, nodule, pneumothorax, and rib fracture. Note that, with the exception of one reader (#5) for the presence or absence of rib fracture, the decisiveness in detecting pneumothorax and rib fractures is extremely high and is higher than for the detection of interstitial disease or nodules for all readers. Despite observer training that includes a specific request to distribute the ratings over a wide range, the complete performance curves for the “well-defined” abnormalities, in particular at higher false-positive fractions, are largely determined by a very small fraction of the cases.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

binaryX∼Bin(1,px)Y∼Bin(1,py)multicategoryX∗\|X=0∼F(t)X∗\|X=1∼G(t)Y∗\|Y=0∼F(t)Y∗\|Y=1∼G(t)
b

i

n

a

r

y

m

u

l

t

i

c

a

t

e

g

o

r

y

X

∼

B

i

n

(

1

,

p

x

)

X

∗

\|

X

=

0

∼

F

(

t

)

X

∗

\|

X

=

1

∼

G

(

t

)

Y

∼

B

i

n

(

1

,

p

y

)

Y

∗

\|

Y

=

0

∼

F

(

t

)

Y

∗

\|

Y

=

1

∼

G

(

t

)


where _p  x_ and _p  y_ correspond to the true values of the 1-specificity and sensitivity, respectively, under binary response scale. Also, because we assume that higher ratings are indicative of an assumed presence of the abnormality, we constrain the distribution _G_ to be “to the right” of the distribution _F_ ; in other words ∫G(t)dF(t)>0
∫

G

(

t

)

d

F

(

t

)

>

0
. The true AUCs for binary and multicategory scales can then be written as follows:


Abinary=py+1−px2Acontinuous=py+1−px2+\[∫G(t)dF(t)\]×\[px−py\]
A

b

i

n

a

r

y

=

p

y

+

1

−

p

x

2

A

c

o

n

t

i

n

u

o

u

s

=

p

y

+

1

−

p

x

2

+

\[

∫

G

(

t

)

d

F

(

t

)

\]

×

\[

p

x

−

p

y

\]


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Monte Carlo Estimates of Variance and Bias of the Nonparametric Estimators of AUC (Binary and Continuous Scales) for “Well-Defined” Abnormalities.


True AUC for Binary Scale (A = TPF/2+1/2-FPF/2) 0.70 0.80 0.90 AUC Estimator AUC Estimator AUC Estimator Scale Scale Scale Overlap FPF (pX) Binary Continuous Binary Continuous Binary Continuous Variance Moderate 0.00 0.00151 0.00373 0.00150 0.00302 0.00102 0.00208 0.05 0.00182 0.00369 0.00172 0.00305 0.00112 0.00209 0.10 0.00209 0.00356 0.00187 0.00298 0.00113 0.00213 0.30 0.00262 0.00370 0.00185 0.00301 — — 0.50 0.00212 0.00368 — — — — Negligible 0.00 0.00148 0.00340 0.00148 0.00273 0.00100 0.00152 0.05 0.00188 0.00356 0.00170 0.00271 0.00107 0.00150 0.10 0.00211 0.00348 0.00187 0.00270 0.00113 0.00153 0.30 0.00263 0.00350 0.00190 0.00276 — — 0.50 0.00212 0.00353 — — — — Bias Moderate 0.00 0.00028 −0.03050 −0.00029 −0.04783 −0.00002 −0.06251 0.05 −0.00047 −0.03266 0.00056 −0.04721 0.00044 −0.06264 0.10 0.00000 −0.03166 0.00030 −0.04639 0.00013 −0.06296 0.30 0.00069 −0.03136 −0.00077 −0.04809 — — 0.50 0.00013 −0.03172 — — — — Negligible 0.00 −0.00003 −0.00101 0.00074 −0.00001 –0.00010 −0.00211 0.05 −0.00036 −0.00178 0.00027 −0.00045 –0.00048 −0.00233 0.10 −0.00055 −0.00127 −0.00026 −0.00199 –0.00018 −0.00169 0.30 0.00007 −0.00094 −0.00077 −0.00183 — — 0.50 0.00064 0.00035 — — — —

Estimates are based on 10,000 simulations for 40 actually positive and 40 actually negative examinations for each combination of the parameters. Continuous ratings (multicategory responses) for the examinations diagnosed as negative and positive in the binary scale are normally distributed with the same standard deviation and distances of 2 and 4 standard deviations between the applicable distributions and are termed “moderate” and “negligible” overlap, respectively.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Hadjiiski L., Chan H.P., Sahiner B., et. al.: Improvement in radiologists’ characterization of malignant and benign breast masses on serial mammograms with computer-aided diagnosis: an ROC study. Radiology 2004; 233: pp. 255-265.


- 2\. Shiraishi J., Abe H., Li F., et. al.: Computer-aided diagnosis for the detection and classification of lung cancers on chest radiographs ROC analysis of radiologists’ performance. Acad Radiol 2006; 13: pp. 995-1003.


- 3\. Horsch K., Giger M.L., Vyborny C.J., et. al.: Classification of breast lesions with multimodality computer-aided diagnosis: observer study results on an independent clinical data set. Radiology 2006; 240: pp. 357-368.


- 4\. Herron J.M., Bender T., Campbell W.L., et. al.: Effects of luminance and resolution on observer performance. Radiology 2000; 215: pp. 169-174.


- 5\. Gur D., Rockette H.E., Armfield D.R., et. al.: Prevalence effect in a laboratory environment. Radiology 2003; 228: pp. 10-14.


- 6\. Egan J.P., Schulman A.l., Greenberg G.Z.: Operating characteristics determined by binary decisions and by ratings. J Acoust Soc Am 1959; 31: pp. 768-773.


- 7\. Rockette H.E., Gur D., Metz C.E.: The use of continuous and discrete confidence judgments in ROC studies. Invest Radiol 1992; 27: pp. 169-172.


- 8\. Beiden S.V., Wagner R.F., Doi K., et. al.: Independent versus sequential reading in ROC studies of computer-assist modalities: analysis of components of variance. Acad Radiol 2002; 9: pp. 1036-1043.


- 9\. Jiang Y., Nishikawa R.M., Schmidt R.A., Metz C.E.: Comparison of independent double readings and computer-aided diagnosis (CAD) for the diagnosis of breast calcifications. Acad Radiol 2006; 13: pp. 84-94.


- 10\. Chakraborty D.P.: Maximum likelihood analysis of free-response receiver operating characteristic analyses. Med Phys 1989; 16: pp. 561-568.


- 11\. Chakraborty D.P., Berbaum K.S.: Observer studies involving detection and localization: modeling, analysis and validation. Med Phys 2004; 31: pp. 2313-2330.


- 12\. Chakraborty D.P.: A search model and figure of merit for observer data acquired according to the free-response paradigm. Phys Med Biol 2006; 51: pp. 3449-3462.


- 13\. Gur D., King J.L., Rockette H.E., et. al.: Practical issues of experimental ROC analysis. Invest Radiol 1990; 25: pp. 583-586.


- 14\. Dorfman D.D., Berbaum K.S., Brandser E.A.: A contaminated binormal model for ROC data: part I. Acad Radiol 2000; 7: pp. 420-426.


- 15\. Dorfman D.D., Berbaum K.S.: A contaminated binormal model for ROC data: part II. Acad Radiol 2000; 7: pp. 427-437.


- 16\. Dorfman D.D., Berbaum K.S.: A contaminated binormal model for ROC data: part III. Acad Radiol 2000; 7: pp. 438-447.


- 17\. Wagner R.F., Beiden S.V., Metz C.E.: Continuous versus categorical data for ROC analysis: some quantitative considerations. Acad Radiol 2001; 8: pp. 328-334.


- 18\. Coffin M., Sukhatme S.: Receiver operating characteristic studies and measurement error. Biometrics 1997; 53: pp. 823-837.


- 19\. Faraggi D.: The effect of random measurement error on receiver operating characteristic (ROC) curves. Stat Med 2000; 19: pp. 61-70.


- 20\.  Wagner RF. US Food and Drug Administration. Computer-aided diagnosis and the general bioinformatics problem. Presented at the SPIE Medical Imaging meeting San Diego (February 2007). Proc SPIE 6514:S3.