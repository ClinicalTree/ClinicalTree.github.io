---
title: Application of Threshol d-bias Independent Analysis to Eye-tracking and FROC Data
author: [CL_AT_DevPChakrabortyPhD,CL_AT_HongJunYoonPhD,CL_AT_ClaudiaMelloThomsMSPhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 12]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Studies of medical image interpretation have focused on either assessing radiologists' performance using, for example, the receiver operating characteristic (ROC) paradigm, or assessing the interpretive process by analyzing their eye-tracking (ET) data. Analysis of ET data has not benefited from threshold-bias independent figures of merit (FOMs) analogous to the area under the receiver operating characteristic (ROC) curve. The aim was to demonstrate the feasibility of such FOMs and to measure the agreement between FOMs derived from free-response ROC (FROC) and ET data.

## Methods

Eight expert breast radiologists interpreted a case set of 120 two-view mammograms while eye-position data and FROC data were continuously collected during the interpretation interval. Regions that attract prolonged (>800 ms) visual attention were considered to be virtual marks, and ratings based on the dwell and approach-rate (inverse of time-to-hit) were assigned to them. The virtual ratings were used to define threshold-bias independent FOMs in a manner analogous to the area under the trapezoidal alternative FROC (AFROC) curve (0 = worst, 1 = best). Agreement at the case level (0.5 = chance, 1 = perfect) was measured using the jackknife and 95% confidence intervals (CI) for the FOMs and agreement were estimated using the bootstrap.

## Results

The AFROC mark-ratings' FOM was largest at 0.734 (CI 0.65–0.81) followed by the dwell at 0.460 (0.34–0.59) and then by the approach-rate FOM 0.336 (0.25–0.46). The differences between the FROC mark-ratings' FOM and the perceptual FOMs were significant ( _P_ < .05). All pairwise agreements were significantly better then chance: ratings vs. dwell 0.707 (0.63–0.88), dwell vs. approach-rate 0.703 (0.60–0.79) and rating vs. approach-rate 0.606 (0.53–0.68). The ratings vs. approach-rate agreement was significantly smaller than the dwell vs. approach-rate agreement ( _P_ = .008).

## Conclusions

Leveraging current methods developed for analyzing observer performance data could complement current ways of analyzing ET data and lead to new insights.

## Introduction

Observer performance measurements in radiology involve collecting ratings, usually one per image as in the receiver operating characteristic (ROC) paradigm , or one per perceived suspicious region as in the free-response receiver operating characteristic (FROC) paradigm . The rating, which could be an integer or continuous variable, represents a decision about how confident the observer is in the presence of abnormality in the image (for ROC) or at the location of the perceived suspicious region (for FROC). The analysis of observer performance data, to which Professor Charles E. Metz has made seminal contributions, uses a figure of merit (FOM), such as the area under the ROC curve (AUC), which rewards/penalizes correct/incorrect decisions in a manner commensurate with their ratings . For example, in the ROC paradigm, high-rated abnormal images and low-rated normal images are rewarded more than intermediate-rated images; and low-rated abnormal images and high-rated normal images are penalized more than intermediate-rated images. Likewise, a FROC FOM rewards high-rated lesions and unmarked normal images while penalizing high rated marks on normal images. In either paradigm, the FOM depends on reader skill and on the difficulty of the cases but is independent of threshold-bias inherent in an observer's usage of the rating scale.

Threshold-bias can be thought of as how conservative or liberal the observer is in using the rating scale: a conservative observer tends to be more reluctant to give high ratings, whereas the liberal observer is less reluctant. Two observers may use the ratings scale quite differently, yet in ROC analysis they could yield identical AUCs. ROC analysis eliminates threshold-bias by measuring the differential ability of the ratings to correctly classify diseased and nondiseased images. Threshold-bias independence is an important advantage of ROC/FROC area-based FOMs over sensitivity-specificity analysis . As an example, consider the study conducted to evaluate the effectiveness of screening mammography by estimating the variability in radiologists' ability to detect breast cancer. Fifty accredited mammography centers were randomly sampled from across the United States. One hundred eight radiologists from these centers gave blinded interpretation to the same set of 79 randomly selected screening mammograms. Ground truth for these women had been established either by biopsy or by 2-year follow-up. The observed range of sensitivity was at least 40% and the range of false positive fraction was at least 45%. The study shows that a large part of the variability in sensitivity and specificity is due to the radiologists' variable thresholds for reporting disease. Once this is accounted for, the variability of the AUC measure, representing the intrinsic variability in diagnostic abilities of the mammographers, is only 11%.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Selection of Observers, Cases, and Ground Truth

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## FROC and ET Data Collection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Schematic of the data collection and processing to obtain real and virtual marks: the radiologists interpreted the images using a two-monitor workstation. Concurrently, and for the duration of the interpretation, an ASL eye-position tracking system determined the line-of-gaze. The ASL fixation and clustering algorithms are described in the text. The proximity criterion, defined as 2.5° of visual angle, is the maximum distance between a lesion center and a mark for the mark to be considered an LL (correct localization). Nonlesion localizations are all other marks. ASL, Applied Sciences Laboratory; NL, non-lesion localization; LL, lesion localization.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ApplicationofThresholdbiasIndependentAnalysistoEyetrackingandFROCData/0_1s20S1076633212004643.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Study Protocol

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Eye-position Data Clustering

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Example of (a) small clusters in yellow ; (b) big-clusters, before threshold, in green ; and (c) big clusters, after applying the 800 ms threshold, in blue . The green diamond symbol marks the location where search started, whereas the red cross symbol indicates the locations marked by the radiologist as containing a malignant lesion. The small yellow dots mark the raw eye-position data. The red circles mark the true locations of the lesions in the two views.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ApplicationofThresholdbiasIndependentAnalysistoEyetrackingandFROCData/1_1s20S1076633212004643.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Measures of Visual Attention

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Generalized Ratings, FOM, Agreement, and Confidence Intervals

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Summary of the Average Numbers of Physical FROC NL and LL Marks per Image and Virtual ET NL and LL Marks for Individual Readers Split between NOR and ABN Cases


Reader Physical FROC Marks Virtual ET Marks NL LL NL LL NOR ABN NOR ABN 1 0.607 0.305 0.831 3.557 2.695 0.864 2 1.098 1.034 0.695 5.852 4.898 0.695 3 0.574 0.881 0.627 4.738 5.475 0.797 4 0.541 0.797 0.678 3.475 2.831 0.831 5 2.311 3.237 0.814 6.230 7.000 0.831 6 0.770 1.017 0.780 2.328 2.814 0.627 7 1.082 1.017 0.678 2.820 2.831 0.593 8 0.230 0.542 0.627 0.672 0.797 0.644 Average 0.902 1.104 0.716 3.709 3.667 0.735

ABN, abnormal; ET, eye tracking; FROC, free-response receiver operating characteristic; LL, lesion localizations; NL, nonlesion localizations; NOR, normal.


On normal images only NL marks are possible but on abnormal images both NL and LL marks are possible. The final row lists the averages of the corresponding columns.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Summary of the Average Ratings, Dwells, and Approach-rates per Image for the Individual Readers, Split between NOR and ABN Cases, and between NLs and LLs


Reader Rating R Dwell D (s) Approach-rate A (s  −1  ) NL LL NL LL NL LL NOR ABN NOR ABN NOR ABN 1 1.649 2.833 2.918 2.131 2.109 4.701 0.684 0.725 0.907 2 1.851 2.164 3.073 3.524 3.481 5.334 0.488 0.525 1.186 3 1.657 2.212 3.324 2.338 2.463 4.210 0.581 0.414 1.106 4 1.242 2.085 3.275 2.435 3.230 6.699 0.675 0.470 1.270 5 1.291 2.199 3.104 3.464 3.799 8.251 0.541 0.394 1.054 6 3.277 3.933 4.130 2.617 2.863 5.626 0.697 0.581 0.903 7 1.742 3.100 3.600 3.499 3.331 3.638 0.780 0.894 0.835 8 1.500 2.625 3.459 2.464 3.569 6.193 0.894 0.870 1.664 Average 1.776 2.644 3.361 2.842 3.286 6.276 0.796 0.690 1.185

ABN, abnormal; ET, eye tracking; FROC, free-response receiver operating characteristic; LL, lesion localizations; NL, nonlesion localizations; NOR, normal.


The final row lists the averages of the corresponding columns.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


FOM Values


Reader Rating Dwell Approach-rateR
R
D
D
A
A
1 0.806 0.577 0.263 2 0.632 0.221 0.220 3 0.723 0.433 0.303 4 0.753 0.551 0.408 5 0.703 0.445 0.249 6 0.795 0.498 0.364 7 0.692 0.280 0.244 8 0.764 0.678 0.635 Average (95% CI) 0.734 (0.65–0.81) 0.460 (0.34–0.59) 0.336 (0.25–0.46)

FOM, figure of merit; FROC, free-response receiver operating characteristic.


The ratings FOM was largest, followed by the dwell, and then by the approach rate. The differences between the FROC mark ratings FOM and the perceptual FOMs were significant ( _P_ < .05). The last row lists the average over all readers and the bootstrap 95% confidence interval.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Agreements Values


Reader Rating vs. Dwell Dwell vs. Approach-rate Rating vs. Approach-rateΓRD
Γ

R

D
ΓDA
Γ

D

A
ΓRA
Γ

R

A
1 0.808 0.583 0.592 2 0.550 0.683 0.533 3 0.683 0.675 0.592 4 0.817 0.692 0.608 5 0.617 0.558 0.542 6 0.708 0.733 0.608 7 0.675 0.717 0.575 8 0.800 0.983 0.800 Average (95% CI) 0.707 (0.63, 0.88) 0.703 (0.60, 0.79) 0.606 (0.53, 0.68)

All pairwise agreements were significantly better then chance. The ratings vs. approach-rate agreement was significantly smaller than the dwell vs. approach-rate agreement ( _P_ = .008). The last row lists the average over all readers and the bootstrap 95% confidence interval (CI).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix 1

## Figures of Merit Derived from FROC and Eye-tracking Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Notation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Figures-of-merit

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X,j=1NNNA∑NNk1=1∑NAk2=1ψ(maxl1(xjk11l11),maxl2(xjk22l22))
X

,

j

=

1

N

N

N

A

∑

k

1

=

1

N

N

∑

k

2

=

1

N

A

ψ

(

m

a

x

l

1

(

x

j

k

1

1

l

1

1

)

,

m

a

x

l

2

(

x

j

k

2

2

l

2

2

)

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix 2

## Measuring Agreement between Pairs of Figures-of-merit

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

∗k=K−(K−1)(k)
k

∗

=

K

−

(

K

−

1

)

(

k

)


Here K=NN+NA
K

=

N

N

+

N

A
is the total number of cases,  is the figure of merit using all cases, (k)
(

k

)
is the figure of merit when case _k_ is removed (jackknifed) from the analysis and _k_ runs from 1 to _K_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δ∗k=∗k−∗∙
Δ

k

∗

=

k

∗

−

•

∗


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ΓXX'=∑Jj=1∑Kk=1ψ(0,Δ∗X,jkΔ∗X',jk)JK
Γ

X

X

'

=

∑

j

=

1

J

∑

k

=

1

K

ψ

(

0

,

Δ

X

,

j

k

∗

Δ

X

'

,

j

k

∗

)

J

K


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ΓXX',j=∑Kk=1ψ(0,Δ∗X,jkΔ∗X',jk)K
Γ

X

X

'

,

j

=

∑

k

=

1

K

ψ

(

0

,

Δ

X

,

j

k

∗

Δ

X

'

,

j

k

∗

)

K


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Confidence Intervals for Figures of Merit and Agreement

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Metz C.E.: Basic principles of ROC analysis. Semin Nucl Med 1978; 8: pp. 283-298.


- 2\. Metz C.E.: ROC methodology in radiologic imaging. Investig Radiol 1986; 21: pp. 720-733.


- 3\. Bunch P.C., Hamilton J.F., Sanderson G.K., et. al.: A free-response approach to the measurement and characterization of radiographic-observer performance. J Appl Photogr Eng 1978; 4: pp. 166-171.


- 4\. Chakraborty D.P.: New developments in observer performance methodology in medical imaging. Semin Nucl Med 2011; 41: pp. 401-418.


- 5\. Chakraborty D.P., Berbaum K.S.: Observer studies involving detection and localization: Modeling, analysis and validation. Med Phys 2004; 31: pp. 2313-2330.


- 6\. Begg C.B.: Biases in the assessment of diagnostic tests. Stat Med 1987; 6: pp. 411-423.


- 7\. Beam C.A., Layde P.M., Sullivan D.C.: Variability in the interpretation of screening mammograms by US radiologists. Findings from a national sample. Arch Intern Med 1996; 156: pp. 209-213.


- 8\. Krupinski E.A., Nodine C.F.: Gaze duration predicts the locations of missed lesions in mammography.Gale A.G.Astley S.M.Dance D.R. et. al.Digital mammography: proceedings of the 2nd International Workshop on Digital Mammography.1994.Elsevier Science B.V.Amsterdam, The Netherlands:pp. 399-403.


- 9\. Kundel H.L., Nodine C.F., Krupinski E.A.: Computer-displayed eye position as a visual aid to pulmonary nodule interpretation. Investig Radiol 1990; 25: pp. 890-896.


- 10\. Nodine C., Mello-Thoms C., Kundel H., et. al.: Time course of perception and decision making during mammographic interpretation. AJR Am J Roentgenol 2002; 179: pp. 917-923.


- 11\. Nodine C.F.: Recording and analyzing eye-position data using a microcomputer workstation. Behav Res Methods Instruments Computers 1992; 24: pp. 475-485.


- 12\. Hillstrom A.: Repetition effects in visual search. Percept Psychophys 2000; 2: pp. 800-817.


- 13\. Kundel H.L., Nodine C.F., Carmody D.: Visual scanning, pattern recognition and decision-making in pulmonary nodule detection. Invest Radiol 1978; 13: pp. 175-181.


- 14\. Kundel H.L., Nodine C.F., Krupinski E.A., et. al.: Using gaze-tracking data and mixture distribution analysis to support a holistic model for the detection of cancers on mammograms. Acad Radiol 2008; 15: pp. 881-886.


- 15\. Mello-Thoms C., Hardesty L.A., Sumkin J.H., et. al.: Effects of lesion conspicuity on visual search in mammogram reading. Acad Radiol 2005; 12: pp. 830-840.


- 16\. Hanley J.A.: The robustness of the “binormal” assumptions used in fitting ROC curves. Med Decis Making 1988; 8: pp. 197-203.


- 17\. Chakraborty D.P.: ROC Curves predicted by a model of visual search. Phys Med Biol 2006; 51: pp. 3463-3482.


- 18\. Chakraborty D.P.: A search model and figure of merit for observer data acquired according to the free-response paradigm. Phys Med Biol 2006; 51: pp. 3449-3462.


- 19\. Yoon H.J., Zheng B., Sahiner B., et. al.: Evaluating computer-aided detection algorithms. Med Phys 2007; 34: pp. 2024-2038.


- 20\. Hanley J.A., Hajian-Tilaki K.O.: Sampling variability of nonparametric estimates of the areas under receiver operating characteristic curves: an update. Acad Radiol 1997; 4: pp. 49-58.


- 21\. Chakraborty D.P., Hagood T.M., Ryan J., et. al.: Quantifying the clinical relevance of a laboratory observer performance paradigm. Br J Radiol 2012; 85: pp. 1287-1302.


- 22\. Chakraborty D.P.: Measuring agreement between ratings interpretations and binary clinical interpretations of images: a simulation study of methods for quantifying the clinical relevance of an observer performance paradigm. Phys Med Biol 2012; 57: pp. 2873-2904.