---
title: Comparison of the Quantitative CT Imaging Biomarkers of Idiopathic Pulmonary Fibrosis at Baseline and Early Change with an Interval of 7 Months
author: [CL_AT_HyunJKimMSPhD,CL_AT_MatthewSBrownPhD,CL_AT_DanielChongMS,CL_AT_DavidWGjertsonPhD,CL_AT_PeiyunLuMS,CL_AT_HakJKimMS,CL_AT_HeidiCoyBS,CL_AT_JonathanGGoldinMDPhD]
date: 2015-01-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 22, Issue 1]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Median survival of patients with idiopathic pulmonary fibrosis (IPF) is 2–5 years. Sensitive imaging metrics can play a role in detecting early changes in therapeutic development. The aim of the present study was to compare known computed tomography (CT) histogram kurtosis and a classifier-based quantitative score to assess baseline severity and change over time in patients with IPF.

## Materials and Methods

A total of 57 patients with at least baseline and paired follow-up scans were selected from an imaging database of standardized CT scans obtained from patients with IPF. CT histogram measurement of kurtosis and quantitative lung fibrosis (QLF) and quantitative interstitial lung disease (QILD) scores from a classification algorithm were calculated. Spearman rank correlations were used to assess associations between baseline severity and changes for all CT-derived measures compared to forced vital capacity (FVC) and carbon monoxide diffusion capacity (DL  CO ) (percent predicted).

## Results

At baseline, mean (±SD) of kurtosis was 2.43 (±1.83). Mean (±SD) values of QLF and QILD scores were 20.7% (±13.4) and 43.3% (±20.0), respectively. All baseline histogram indices and QLF and QILD scores were correlated well with baseline FVC and DL  CO . When assessing associations with changes in FVC and DL  CO over time, only QLF score was statistically significant (ρ = −0.57; _P_ < .0001 for FVC and ρ = −0.34; _P_ = .025 for DL  CO ), whereas kurtosis was not.

## Conclusions

Classifier-model-derived scores (QLF and QILD), based on a set of texture features, are associated with baseline disease extent and are also a sensitive measure of change over time. A QLF score can be used for measuring the extent of disease severity and longitudinal changes.

Idiopathic pulmonary fibrosis (IPF) is a rare and ultimately fatal lung disease of unknown cause with a median survival of 2–5 years . Although several studies have identified risk factors and histopathologic features, the natural history of IPF is poorly understood and the rate of progression for a given patient can be unpredictable. Disease progression ranges from very rapid to remaining stable over several years and may be punctuated by acute worsening . Diagnosing IPF can also be challenging as distinct from other diffuse lung diseases . High-resolution computed tomography (HRCT) plays an indispensable role in the diagnosis of IPF. Predicating the presence of a classically subpleural, basilar distribution of interstitial abnormalities, or other known causes of interstitial lung disease, the HRCT features obviate the need for surgical biopsy . Evidence of classic visual feature of IPF on thoracic CT is often used as inclusion criteria in clinical trials. Guidelines have been developed for assigning a confidence to a diagnosis of IPF on CT . There are currently very limited treatment options for patients diagnosed with IPF. Important to the success of IPF clinical trials are the inclusion of correctly characterized patients and the demonstration of clinically meaningful benefits .

Development of a sensitive surrogate measure for IPF has become increasingly urgent, as the understanding of underlying pathophysiology of IPF has led to several potential, new antifibrotic therapies . In measuring treatment outcomes, a change in forced vital capacity (FVC) has been most often used. The progression is normally defined as 10% drop in FVC. The implication of progression in FVC differs in patients with moderate and severe IPF. Other outcomes have included the 6-minute walk test, carbon monoxide diffusion capacity (DL  CO ), and quality of life instruments . More recently the Food and Drug Administration suggested that mortality as an ideal endpoint be used in pivotal clinical trials . The usage of survival requires large study populations and long trials making this economically and logistically challenging. Overall survival as an outcome need to consider systematic biases at clinical centers, socioeconomic status, and censoring because of lung transplant if a patient is eligible . Development and evaluation of the HRCT method, whose measurement is sensitive to the early localized changes, is important to assess or confirm the effect of therapy on patients with IPF.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Patient Selection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CT Scanning Protocol

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantitative CT Image Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CT Histogram Features

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Kurtosis=(x−x¯)4\[∑(x−x¯)2\]2−3,
Kurtosis

=

(

x

−

x

¯

)

4

\[

∑

(

x

−

x

¯

)

2

\]

2

−

3

,


where _x_ indicates CT density ranging from −1024 to +200 HU and x¯
x

¯
is the mean Hounsfield unit value from the CT attenuation histogram.

![Figure 1, Two patients with mild and severe IPF (FVC 65%, and 47%, respectively): kurtosis measures are 5.00 and 0.41 in subjects with mild and severe IPF, respectively. Corresponding skewness measures are 1.48 and 0.80. FVC, forced vital capacity; IPF, idiopathic pulmonary fibrosis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComparisonoftheQuantitativeCTImagingBiomarkersofIdiopathicPulmonaryFibrosisatBaselineandEarlyChangewithanIntervalof7Months/0_1s20S1076633214003110.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantitative CT Scores from Texture Classification Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

QLFscore(%)=voxelsclassifiedasreticularpatternstotalsamples×100,
QLF

score

(

%

)

=

v

o

x

e

l

s

c

l

a

s

s

i

f

i

e

d

a

s

r

e

t

i

c

u

l

a

r

p

a

t

t

e

r

n

s

t

o

t

a

l

s

a

m

p

l

e

s

×

100

,


QLFvolume(L)=(QLFscore/100)×segmentedlungorlobarvolume(L),
QLF

volume

(

L

)

=

(

Q

L

F

s

c

o

r

e

/

100

)

×

s

e

g

m

e

n

t

e

d

l

u

n

g

o

r

l

o

b

a

r

v

o

l

u

m

e

(

L

)

,


QILDscore(%)=voxelsclassifiedasabnomalpatternstotalsamples×100,
QILD

score

(

%

)

=

v

o

x

e

l

s

c

l

a

s

s

i

f

i

e

d

a

s

a

b

n

o

m

a

l

p

a

t

t

e

r

n

s

t

o

t

a

l

s

a

m

p

l

e

s

×

100

,


QILDvolume(L)=(QILDscore/100)×segmentedlungorlobarvolume(L).
QILD

volume

(

L

)

=

(

Q

I

L

D

s

c

o

r

e

/

100

)

×

s

e

g

m

e

n

t

e

d

l

u

n

g

o

r

l

o

b

a

r

v

o

l

u

m

e

(

L

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Descriptive Summary Statistics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Characteristics of Idiopathic Pulmonary Fibrosis Subjects


Variables Baseline ( _N_ = 57) Follow-Up ( _N_ = 57)_P_ value Mean (SD) Median (IQR) Mean (SD) Median (IQR) Pulmonary function tests TLC volume  ∗  (L) 4.11 (0.96) 4.13 (0.87) 3.93 (1.01) 4.04 (1.42) .2190 RV volume  ∗  (L) 1.50 (0.69) 1.44 (0.81) 1.36 (0.52) 1.31 (0.81) .9523 FVC (% pred) 65.18 (12.44) 66.40 (18.80) 62.79 (14.05) 63.60 (18.40) .0001  †  FEV  1  (% pred) 71.34 (13.03) 72.60 (18.30) 68.28 (14.82) 69.00 (20.70) <.0001 DL  CO  ∗  (% pred) 49.67 (14.19) 47.00 (15.70) 45.18 (13.53) 44.50 (17.50) <.0001 CT histogram indexes Kurtosis 2.81 (1.83) 2.38 (2.44) 2.26 (1.77) 1.83 (1.93) <.0001  †  Mean −768.28 (53.62) −772.87 (63.88) −756.40 (62.82) −757.91 (79.06) .0329  †  Variance 44,299.30 (15,065.58) 42,578.12 (21,196.77) 44,299.30 (15,065.58) 42,578.12 (21,196.77) .1626 Skewness 1.58 (0.42) 1.59 (0.53) 1.47 (0.43) 1.46 (0.53) <.0001 Entropy 6.37 (0.24) 6.33 (0.29) 6.39 (0.27) 6.36 (0.31) .1741 Median −829.32 (50.63) −832.00 (62.00) −819.67 (56.90) −817.00 (58.00) .0811 Quantitative CT texture scores QLF score (%) 17.63 (10.10) 17.00 (13.00) 20.37 (11.99) 18.00 (14.00) <.0001  †  Ground glass score (%) 17.53 (7.44) 16.00 (11.00) 17.25 (7.30) 17.00 (10.00) .6435 QILD score (%) 39.02 (17.22) 38.00 (21.00) 41.33 (17.86) 39.00 (23.00) .0453 QLF volume (L) 0.63 (0.39) 0.56 (0.31) 0.71 (0.41) 0.64 (0.35) .0002 Ground glass volume (L) 0.63 (0.23) 0.61 (0.35) 0.61 (0.25) 0.61 (0.33) .6590 QILD volume (L) 1.39 (0.63) 1.30 (0.55) 1.46 (0.65) 1.31 (0.64) .0521  †

CT, computed tomography; TLC, total lung capacity; RV, residual volume. DL  CO  , carbon monoxide diffusion capacity; FEV, forced expiratory volume in 1 second; FVC, forced vital capacity; IQR, interquartile range; QLF, quantitative lung fibrosis; QILD, quantitative interstitial lung disease; SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, (a) Baseline CT scan: FVC is 54.4% and CT TLC volume is 3.51 L; (b) follow-up CT scan: FVC is 53.5%, DL CO decreased by 8.6%, and CT volume is 3.34 L; (c) baseline classification overlay for QLF score at whole lung of 15% in blue and red and QILD of 43% (not overlaid); (d) follow-up classification overlay for QLF score of 22% in blue and red and QILD of 52% (not overlaid); (e) baseline histogram with kurtosis of 2.24; (f) follow-up kurtosis of 2.51, which is greater than baseline (indicating improvement which is not consistent with FVC and QLF). CT, computed tomography; DL CO , carbon monoxide diffusion capacity; FVC, forced vital capacity; QILD, quantitative interstitial lung disease; QLF, quantitative lung fibrosis. For interpretation of the references to color in this figure legend, the reader is referred to the web version of this article.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComparisonoftheQuantitativeCTImagingBiomarkersofIdiopathicPulmonaryFibrosisatBaselineandEarlyChangewithanIntervalof7Months/1_1s20S1076633214003110.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Associations

## Whole Lung

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Association at Baseline at Whole Lung


Baseline Percent Predicted FVC (%), _N_ = 57 Percent Predicted FEV  1  (%), _N_ = 57 Percent Predicted DL  CO  (%), _N_ = 51 CT histogram indexes Kurtosis 0.56 ( _P_ < .0001) 0.49 ( _P_ = .0001) 0.44 ( _P_ = .0014) Mean −0.60 ( _P < .0001_ ) −0.45 ( _P_ = .0005) −0.36 ( _P_ = .0094) Variance −0.55 ( _P_ < .0001) −0.56 ( _P_ < .0001) −0.31 ( _P_ = .0264) Skewness 0.50 ( _P_ < .0001) 0.43 ( _P_ = .0007) 0.07 ( _P_ = .003) Entropy −0.54 ( _P_ < .0001) −0.51 ( _P_ < .0001) −0.44 ( _P_ = .0013) Median −0.22 ( _P_ = .107) −0.17 ( _P_ = .197) −0.2544 ( _P_ = .072) Quantitative CT texture scores QLF score (%) −0.59 ( _P_ < .0001) −0.51 ( _P_ < .0001) −0.46 ( _P_ = .0007) Ground glass (%) −0.36 ( _P_ = .0053) −0.20 ( _P_ = .1270) −0.28 ( _P_ = .0431) QILD score (%) −0.58 ( _P_ < .0001) −0.50 ( _P_ = .0001) −0.45 ( _P_ = .0009) QLF volume (L) −0.44 ( _P_ = .0006) − _0.38 (P = .0033)_ −0.35 ( _P_ = .0123) Ground glass (L) −0.04 ( _P_ = .75) 0.059 ( _P_ = .66) 0.04 ( _P_ = .78) QILD volume (L) −0.30 ( _P_ = .021) −0.25 ( _P_ = .064) −0.22 ( _P_ = .117)

CT, computed tomography; DL  CO  , carbon monoxide diffusion capacity; FEV, forced expiratory volume in 1 second; FVC, forced vital capacity; QLF, quantitative lung fibrosis; QILD, quantitative interstitial lung disease.


![Figure 3, Association with PFT of kurtosis and QLF at baseline for whole lung. DL CO , carbon monoxide diffusion capacity; FEV, forced expiratory volume in 1 second; FVC, forced vital capacity; QLF, quantitative lung fibrosis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComparisonoftheQuantitativeCTImagingBiomarkersofIdiopathicPulmonaryFibrosisatBaselineandEarlyChangewithanIntervalof7Months/2_1s20S1076633214003110.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Association in the Change Assessment for Whole Lung


Changes Percent Predicted FVC (%), _N_ = 57, ρ ( _P_ value) Percent Predicted FEV  1  (%), _N_ = 57, ρ ( _P_ value) DL  CO  (%), _N_ = 43, ρ ( _P_ value) CT histogram indexes Kurtosis 0.26 ( _P_ = .0513) 0.0719 ( _P_ = .60) −0.1626 ( _P_ = .30) Mean −0.54 ( _P_ < .0001) −0.4442 ( _P_ = .0005) −0.2384 ( _P_ = .12) Variance −0.22 ( _P_ = .1061) −0.2077 ( _P_ = .1211) −0.2505 ( _P_ = .11) Skewness 0.41 ( _P_ = .0017) 0.2116 ( _P_ = .1140) 0.0414 ( _P_ = .79) Entropy −0.36 ( _P_ = .0055) −0.3195 ( _P_ = .0154) −0.2605 ( _P_ = .0916) Median −0.52 ( _P_ < .0001) −0.4099 ( _P_ = .0015) −0.2459 ( _P_ = .11) Quantitative CT texture scores QLF score (%)_−0.57 (P < .0001)_ −0.49 ( _P_ = .0001) −0.34 ( _P_ = .0251) Ground glass (%) −0.31 ( _P_ = .0185) −0.26 ( _P_ = .0512) −0.034 ( _P_ = .83) QILD score (%) −0.45 ( _P_ = .0004) −0.39 ( _P_ = .0030) −0.21 ( _P_ = .17) QLF volume (L)_−0.51_ ( _P_ < .0001) −0.44 ( _P_ = .0005) −0.37 ( _P_ = .0149) Ground glass (L) −0.19 ( _P_ = .15) −0.14 ( _P_ = .32) 0.018 ( _P_ = .91) QILD volume (L) −0.38 ( _P_ = .0033) −0.34 ( _P_ = .0103) −0.27 ( _P_ = .0753)

CT, computed tomography; DL  CO  , carbon monoxide diffusion capacity; FEV, forced expiratory volume in 1 second; FVC, forced vital capacity; QLF, quantitative lung fibrosis; QILD, quantitative interstitial lung disease.


![Figure 4, Association with changes in PFT of kurtosis and QLF for whole lung. DL CO , carbon monoxide diffusion capacity; FEV, forced expiratory volume in 1 second; FVC, forced vital capacity; QLF, quantitative lung fibrosis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComparisonoftheQuantitativeCTImagingBiomarkersofIdiopathicPulmonaryFibrosisatBaselineandEarlyChangewithanIntervalof7Months/3_1s20S1076633214003110.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Lobes

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Association in Each Lobe and Lung


Parenchymal Regions Baseline ( _N_ = 57) Changes ( _N_ = 57) QLF Score vs. Percent Predicted FVC (%), ρ ( _P_ value) Kurtosis vs. Percent Predicted FVC (%), ρ ( _P_ value) Skewness vs. Percent Predicted FVC (%), ρ ( _P_ value) QLF Score vs. Percent Predicted FVC (%), ρ ( _P_ value) Kurtosis vs. Percent Predicted FVC (%), ρ ( _P_ value) Skewness vs. Percent Predicted FVC (%), ρ ( _P_ value) Right upper lobe −0.48 ( _P_ = .0002) 0.41 ( _P_ = .0015) 0.37 ( _P_ = .0041) −0.53 ( _P_ < .0001) 0.36 ( _P_ = .0062) 0.37 ( _P_ = .0045) Right middle lobe −0.52 ( _P_ < .0001) 0.49 ( _P_ = .0001) 0.46 ( _P_ = .0003) −0.40 ( _P_ = .0023) 0.21 ( _P_ = .12) 0.22 ( _P_ = .0993) Right lower lobe −0.41 ( _P_ = .0013) 0.44 ( _P_ = .0005) 0.39 ( _P_ = .0027) −0.54 ( _P_ < .0001) 0.19 ( _P_ = .17) 0.34 ( _P_ = .0108) Left upper lobe −0.60 ( _P_ < .0001) 0.53 ( _P_ < .0001) 0.48 ( _P_ = .0001) −0.56 ( _P_ < .0001) 0.26 ( _P_ = .0479) 0.38 ( _P_ = .0036) Left lower lobe −0.55 ( _P_ < .0001) 0.55 ( _P_ < .0001) 0.49 ( _P_ = .0001) −0.53 ( _P_ < .001) 0.34 ( _P_ = .0089) 0.48 ( _P_ = .0002) Right lung −0.54 ( _P_ < .0001) 0.52 ( _P_ < .0001) 0.47 ( _P_ = .0002) −0.55 ( _P_ < .0001) 0.23 ( _P_ = .0908) 0.34 ( _P_ = .0095) Left lung −0.60 ( _P_ < .0001) 0.54 ( _P_ < .0001) 0.48 ( _P_ = .0001) −0.54 ( _P_ < .0001) 0.29 ( _P_ = .0275) 0.44 ( _P_ = .0006)

FVC, forced vital capacity; QLF, quantitative lung fibrosis.


![Figure 5, (a) Association with FVC of kurtosis at baseline for each lobe and lung. (b) Association with FVC of QLF at baseline for each lobe and lung. FVC, forced vital capacity; RUL, right upper lobe; RML, right middle lobe; RLL, right lower lobe; LUL, left upper lobe; LLL, left lower lobe.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComparisonoftheQuantitativeCTImagingBiomarkersofIdiopathicPulmonaryFibrosisatBaselineandEarlyChangewithanIntervalof7Months/4_1s20S1076633214003110.jpg)

![Figure 6, (a) Association with changes in FVC of kurtosis for each lobe and lung. (b) Association with changes in FVC of QLF for each lobe and lung. FVC, forced vital capacity; LLL, left lower lobe; LUL, left upper lobe; QLF, quantitative lung fibrosis; RLL, right lower lobe; RML, right middle lobe; RUL, right upper lobe.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComparisonoftheQuantitativeCTImagingBiomarkersofIdiopathicPulmonaryFibrosisatBaselineandEarlyChangewithanIntervalof7Months/5_1s20S1076633214003110.jpg)

Table 5


Association in Each Lobe and Lung


Parenchymal Regions Baseline ( _N_ = 51) Changes ( _N_ = 43) QLF Score vs. Percent Predicted DL  CO  (%), ρ ( _P_ value) Kurtosis vs. Percent Predicted DL  CO  (%), ρ ( _P_ value) Skewness vs. Percent Predicted DL  CO  (%), ρ ( _P_ value) QLF Score vs. Percent Predicted DL  CO  (%), ρ ( _P_ value) Kurtosis vs. Percent Predicted DL  CO  (%), ρ ( _P_ value) Skewness vs. Percent Predicted DL  CO  (%), ρ ( _P_ value) Right upper lobe −0.37 ( _P_ = .0078) 0.36 ( _P_ = .0097) 0.30 ( _P_ = .0302) −0.31 ( _P_ = .0462) 0.04 ( _P_ = .80) 0.074 ( _P_ = .64) Right middle lobe −0.39 ( _P_ = .0049) 0.35 ( _P_ = .0116) 0.30 ( _P_ = .0331) −0.17 ( _P_ = .27) −0.13 ( _P_ = .41) −0.10 ( _P_ = .50) Right lower lobe −0.38 ( _P_ = .0057) 0.43 ( _P_ = .0019) 0.35 ( _P_ = .0117) −0.24 ( _P_ = .12) −0.15 ( _P_ = .33) −0.034 ( _P_ = .83) Left upper lobe −0.43 ( _P_ = .0016) 0.39 ( _P_ = .0050) 0.32 ( _P_ = .0200) −0.30 ( _P_ = .0537) 0.004 ( _P_ = .98) 0.17 ( _P_ = .27) Left lower lobe −0.49 ( _P_ = .0002) 0.45 ( _P_ = .0008) 0.39 ( _P_ = .0044) −0.33 ( _P_ = .0294) −0.0168 ( _P_ = .92) 0.19 ( _P_ = .22) Right lung −0.43 ( _P_ = .0016) 0.42 ( _P_ = .0022) 0.38 ( _P_ = .0055) −0.27 ( _P_ = .079) 0.20 ( _P_ = .21) −0.0439 ( _P_ = .78) Left lung −0.48 ( _P_ = .0004) 0.43 ( _P_ = .0016) 0.38 ( _P_ = .0056) −0.32 ( _P_ = .034) −0.078 ( _P_ = .62) 0.25 ( _P_ = .11)

DL  CO  , carbon monoxide diffusion capacity; QLF, quantitative lung fibrosis.


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

## References

- 1\. Schwartz D.A., Helmers R.A., Galvin J.R., et. al.: Determinants of survival in idiopathic pulmonary fibrosis. Am J Respir Crit Care Med 1994; 149: pp. 450-454.


- 2\. Raghu G., Weycker D., Edelsberg J., et. al.: Incidence and prevalence of idiopathic pulmonary fibrosis. Am J Respir Crit Care Med 2006; 74: pp. 810-816.


- 3\. Olson A.L., Swigris J.: Idiopathic pulmonary fibrosis: diagnosis and epidemiology. Clin Chest Med 2012; 33: pp. 41-50.


- 4\. GarcÃa-Sancho C., BuendÃa-RoldÃn I., FernÃndez-Plata M.R., et. al.: Familial pulmonary fibrosis is the strongest risk factor for idiopathic pulmonary fibrosis. Respir Med 2001; 105: pp. 1902-1907.


- 5\. King T.E., Schwarz M.I., Brown K., et. al.: Idiopathic pulmonary fibrosis: relationship between histopathologic features and mortality. Am J Respir Crit Care Med 2001; 164: pp. 1025-1032.


- 6\. Ley B., Ryerson C.J., Vittinghoff E., et. al.: A multidimensional index and staging system for idiopathic pulmonary fibrosis. Ann Intern Med 2012; 156: pp. 684-691.


- 7\. du Bois R.M., Weycker D., Albera C., et. al.: Ascertainment of individual risk of mortality for patients with idiopathic pulmonary fibrosis. Am J Respir Crit Care Med 2011; 184: pp. 459-466.


- 8\. Wells A.U., Desai S.R., Rubens M.B., et. al.: Idiopathic pulmonary fibrosis: a composite physiologic index derived from disease extent observed by computed tomography. Am J Respir Crit Care Med 2003; 167: pp. 962-969.


- 9\. Latsi P.I., du Bois R.M., Nicholson A.G., et. al.: Fibrotic idiopathic interstitial pneumonia: the prognostic value of longitudinal functional trends. Am J Respir Crit Care Med 2003; 168: pp. 531-537.


- 10\. Raghu G., Collard H.R., Egan J., et. al.: An official ATS/ERS/JRS/ALAT statement: idiopathic pulmonary fibrosis: evidence-based guidelines for diagnosis and management. Am J Respir Crit Care Med 2011; 183: pp. 788-824.


- 11\. Hodnett P.A., Naidich D.P.: Fibrosing interstitial lung disease. A practical high-resolution computed tomography-based approach to diagnosis and management and a review of the literature. Am J Respir Crit Care Med 2013; 188: pp. 141-149.


- 12\. Raghu G., Collard H.R., Anstrom K.J., et. al.: Idiopathic pulmonary fibrosis: clinically meaningful primary endpoints in phase 3 clinical trials. Am J Respir Crit Care Med 2012; 185: pp. 1044-1048.


- 13\. Cottin V.: Interstitial lung disease. Eur Respir Rev 2013; 22: pp. 26-32.


- 14\. Woodcock H.V., Molyneaux P.L., Maher T.M.: Reducing lung function decline in patients with idiopathic pulmonary fibrosis: potential of nintedanib. Drug Des Devel Ther 2013; 7: pp. 503-510.


- 15\. Adamali H.I., Maher T.M.: Current and novel drug therapies for idiopathic pulmonary fibrosis. Drug Des Devel Ther 2012; 6: pp. 261-272.


- 16\. Loomis-King H., Flaherty K.R., Moore B.B.: Pathogenesis, current treatment and future direction for idiopathic pulmonary fibrosis. Curr Opin Pharmacol 2013; 13: pp. 377-385.


- 17\. O'Connell O.J., Kennedy M.P., Henry M.T.: Idiopathic pulmonary fibrosis: treatment update. Adv Ther 2011; 28: pp. 986-999.


- 18\. Mahendran S., Sethi T.: Treatments in idiopathic pulmonary fibrosis: time for a more targeted approach?. QJM 2012; 105: pp. 929-934.


- 19\. Maher T.M.: PROFILEing idiopathic pulmonary fibrosis: rethinking biomarker discovery. Eur Respir Rev 2013; 22: pp. 148-152.


- 20\. US Food and Drug Administration (FDA): Title of Advisory Committee document.2010.FDAMaryland Available at: http://www.fda.gov/downloads/AdvisoryCommittees/CommitteesMeetingMaterials/Drugs/Pulmonary-AllergyDrugsAdvisoryCommittee/UCM203081.pdf Accessed April 18, 2014


- 21\. Kotloff R.M., Thabut G.: Lung Transplantation. Am J Respir Crit Care Med 2011; 184: pp. 159-171.


- 22\. Best A.C., Lynch A.M., Bozic C.M., et. al.: Quantitative CT indexes in idiopathic pulmonary fibrosis: relationship with physiologic impairment. Radiology 2003; 228: pp. 407-414.


- 23\. Lynch D.A.: Quantitative CT of fibrotic interstitial lung disease. Chest 2007; 131: pp. 643-644.


- 24\. Camiciottoli G., Orlandi I., Bartolucci M., et. al.: Lung CT densitometry in systemic sclerosis: correlation with lung function, exercise testing, and quality of life. Chest 2007; 131: pp. 672-681.


- 25\. Best A.C., Meng J., Lynch A.M., et. al.: Idiopathic pulmonary fibrosis: physiologic tests, quantitative CT indexes, and CT visual scores as predictors of mortality. Radiology 2008; 246: pp. 935-940.


- 26\. Uppaluri R., Hoffman E.A., Sonka M., et. al.: Computer recognition of regional lung disease patterns. Am J Respir Crit Care Med 1999; 160: pp. 648-654.


- 27\. Chabat F., Yang G.Z., Hansell D.M.: Obstructive lung diseases: texture classification for differentiation at CT. Radiology 2003; 228: pp. 871-877.


- 28\. Zavaletta V.A., Bartholmai B.J., Robb R.A.: High resolution multidetector CT-aided tissue analysis and quantification of lung fibrosis. Acad Radiol 2007; 14: pp. 772-787.


- 29\. Kim H.G., Tashkin D.P., Clements P.J., et. al.: A computer-aided diagnosis system for quantitative scoring of extent of lung fibrosis in scleroderma patients. Clin Exp Rheumatol 2010; 28: pp. S26-S35.


- 30\. Kim H.J., Li G., Gjertson D., et. al.: Classification of parenchymal abnormality in scleroderma lung using a novel approach to denoise images collected via a multicenter study. Acad Radiol 2008; 15: pp. 1004-1016.


- 31\. Maldonado F., Moua T., Rajagopalan S., et. al.: Automated quantification of radiologic patterns predicts survival in idiopathic pulmonary fibrosis. Eur Respir J 2013; 43: pp. 204-212.


- 32\. Bartholmai B.J., Raghunath S., Karwoski R.A., et. al.: Quantitative computed tomography imaging of interstitial lung diseases. J Thorac Imaging 2013; 28: pp. 298-307.


- 33\. Kim H.J., Brown M.S., Elashoff R., et. al.: Quantitative texture-based assessment of one-year changes in fibrotic reticular patterns on HRCT in scleroderma lung disease treated with oral cyclophosphamide. Eur Radiol 2011; 21: pp. 2455-2465.


- 34\. Brown M.S., Kim H.J., Abtin F., et. al.: Reproducibility of lung and lobar volume measurements using computed tomography. Acad Radiol 2010; 17: pp. 316-322.


- 35\. Cramer D.: Fundamental statistics for social research.1st ed.1997.RoutledgeNew York NYpp. 89-90.


- 36\. Biomarkers Definitions Working Group: Biomarkers and surrogate endpoints: preferred definitions and conceptual framework. Clin Pharmacol Ther 2001; 69: pp. 89-95.


- 37\. Temple R.J.: A regulatory authority's opinion about surrogate endpoints.Nimmo W.S.Tucker G.T.Clinical measurement in drug evaluation.1995.John WileyNew York:pp. 1-22.


- 38\. Fan J., Li J.: Variable selection via nonconcave penalized likelihood and its oracle properties. J Am Stat Assoc 2001; 96: pp. 1348-1360.


- 39\. Vapnik V.N.: The nature of statistical learning theory.2nd ed.1999.SpringerNew York, NYpp. 138-160.


- 40\. Gay S.E., Kazerooni E.A., Toews G.B., et. al.: Idiopathic pulmonary fibrosis: predicting response to therapy and survival. Am J Respir Crit Care Med 1998; 157: pp. 1063-1072.


- 41\. Tashkin D.P., Elashoff R., Clements P.J., et. al.: Cyclophosphamide versus placebo in scleroderma lung disease. N Engl J Med 2006; 354: pp. 2655-2666.


- 42\. du Bois R.M., Weycker D., Albera C., et. al.: Forced vital capacity in patients with idiopathic pulmonary fibrosis: test properties and minimal clinically important difference. Am J Respir Crit Care Med 2011; 184: pp. 1382-1389.


- 43\. Wells A.U.: Forced vital capacity as a primary end point in idiopathic pulmonary fibrosis treatment trials: making a silk purse from a sow's ear. Thorax 2013; 68: pp. 309-310.