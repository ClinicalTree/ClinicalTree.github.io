---
title: Tree-structured Subgroup Analysis of Receiver Operating Characteristic Curves for Diagnostic Tests
author: [Caixia Li PhD,Claus-C. Glüer PhD,Richard Eastell MD,Dieter Felsenberg MD,David M. Reid MD,Christian Roux MD,Ying Lu PhD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 12 SOURCE CL_S_AcademicRadiologyVolume19Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Multiple diagnostic tests are often available for a disease. Their diagnostic accuracy may depend on the characteristics of testing subjects. The investigators propose a new tree-structured data-mining method that identifies subgroups and their corresponding diagnostic tests to achieve the maximum area under the receiver-operating characteristic curve.

## Materials and Methods

The Osteoporosis and Ultrasound Study is a prospectively designed, population-based European multicenter observational study to evaluate state-of-the-art diagnostic methods for assessing osteoporosis. A total 2837 women underwent dual x-ray absorptiometry (DXA) and quantitative ultrasound (QUS). Prevalent vertebral fractures were determined by a centralized radiology laboratory on the basis of radiographs. The data-mining algorithm includes three steps: defining the criteria for node splitting and selection of the best diagnostic test on the basis of the area under the curve, using a random forest to estimate the probability of DXA being the preferred diagnostic method for each participant, and building a single regression tree to describe subgroups for which either DXA or QUS is the more accurate test or for which the two tests are equivalent.

## Results

For participants with weights ≤54.5 kg, QUS had a higher area under the curve in identifying prevalent vertebral fracture. For participants whose weights were >58.5 kg and whose heights were ≤167.5 cm, DXA was better, and for the remaining participants, DXA and QUS had comparable accuracy and could be used interchangeably.

## Conclusions

The proposed tree-structured subgroup analysis successfully defines subgroups and their best diagnostic tests. The method can be used to develop optimal diagnostic strategies in personalized medicine.

Multiple diagnostic tests are commonly available for the same disease. Their diagnostic accuracy may depend on the characteristics of the testing subjects. For example, bone mineral density (BMD) measured by dual x-ray absorptiometry (DXA) and the speed of sound (SOS) by quantitative ultrasound (QUS) devices are continuous diagnostic markers for osteoporosis. Compared to DXA, QUS has the advantages of low cost, portability, and absence of radiation exposure, but it may be less accurate. A recent prospective multicenter epidemiologic study pointed out that age may influence the choice of quantitative bone assessment techniques in elderly women. In the era of personalized medicine, proper methods are needed to find subgroups with their corresponding optimal diagnostic strategies.

The area under the receiver-operating characteristic (ROC) curve (AUC) is a measure of diagnostic accuracy . A higher AUC reflects higher diagnostic accuracy. Differences between AUCs depend not only on the tests themselves but also on the population tested. A recent regression approach to ROC analysis detects the interactions between diagnostic performance and covariates and assesses diagnostic utility after adjusting for covariate effects. Because of possible complex interactions, particularly when the number of covariates is large, modeling on the basis of regression approaches may make it difficult to answer the question of who should undergo which test. Ciampi et al proposed a tree-structured subgroup analysis for survival data on the basis of a Cox model with interaction terms to find subgroups of patients for whom one treatment is preferable to the other. Negassa et al investigated a model selection in tree-structured subgroup analysis on the basis of Ciampi et al's work. These tree-based methods demonstrated efficiency to handle large numbers of covariates and identify operational subgroups of patients.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Description of the Study Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Summary Statistics of Diagnostic Measurements and Covariates


Nonfractured Subjects ( _n_ 0  = 1951) Fractured Subjects ( _n_ 1  = 371) Diagnostic test Hip BMD (DXA) 878.85 ± 140.03 802.11 ± 149.59 SOS (QUS) 1546.33 ± 10.53 1541.98 ± 10.29 Continuous covariates Age (y) 66.42 ± 6.86 69.18 ± 7.10 Height (cm) 160.64 ± 6.31 159.61 ± 6.30 Weight (kg) 68.71 ± 12.38 67.72 ± 12.41 BMI (kg/m  2  ) 26.61 ± 4.51 26.56 ± 4.42

BMD, bone mineral density; BMI, body mass index; DXA, dual x-ray absorptiometry; QUS, quantitative ultrasound; SOS, speed of sound.


Data are expressed as mean ± standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Description of Recursive Partitioning Tree Algorithm and Random Forest

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Tr0≻Tr1≻Tr2≻⋯≻Trl=Root
Tr

0

≻

Tr

1

≻

Tr

2

≻

⋯

≻

Tr

l

=

Root


is identified that represents the optimal choices of trees at different size. Here, Tr  0 is the largest tree, and Tr _l_ is the smallest tree that has everyone in it. The validation data are used to determine which one of these subtrees has the best utility value in an independently collected data set. The use of validation data is to ensure that the final tree does not overly fit the training data because the splitting step is data dependent.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Description of Subgroup Analysis Algorithm

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Selection of Noninferiority Margin

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Correlations between the preference score v and the predicted preference score (vˆ) (vˆ) ( dashed line ) or the inferiority statistic st ( solid line ) for the Osteoporosis and Ultrasound Study data.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TreestructuredSubgroupAnalysisofReceiverOperatingCharacteristicCurvesforDiagnosticTests/0_1s20S1076633212004746.jpg)

![Figure 2, The selected regression tree for preference score prediction. DXA, dual x-ray absorptiometry; QUS, quantitative ultrasound.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TreestructuredSubgroupAnalysisofReceiverOperatingCharacteristicCurvesforDiagnosticTests/1_1s20S1076633212004746.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Area under the curve (AUC) differences, standard error (SE), and predicted preference score in four terminal nodes of the final tree. The center coordinates of the box for node h are (vˆ,Δˆ) (vˆ,Δˆ) in h , the height and width are proportional to n 0 ( h ) and n 1 ( h ), the area of the box is weight in the weighted stratified AUC calculation, and the vertical line across the box is the interval (Δˆ−SE,Δˆ+SE) (Δˆ−SE,Δˆ+SE) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TreestructuredSubgroupAnalysisofReceiverOperatingCharacteristicCurvesforDiagnosticTests/2_1s20S1076633212004746.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Summary Statistics of the Terminal Nodes, Decision Groups, and Combinations in the Final Tree


Node _h_ Node Information Sample Size Preference Score  ∗  AUCs AUC Difference_st__n__h_ = ( _n__h_ 0  , _n__h_ 1  )vˆ
v

ˆ
± SEˆ=(ˆ1,ˆ2)
ˆ

=

(

ˆ

1

,

ˆ

2

)
Δˆ±SE
Δ

ˆ

±

SE
QUS-preferred subgroup (node 1) (220, 34) 0.286 ± 0.006 (0.637, 0.726) −0.089 ± 0.057 −2.037 1 Weight <54.5 kg (220, 34) 0.286 ± 0.006 (0.637, 0.726) −0.089 ± 0.057 −2.037 No-preference subgroup (nodes 2 and 3 combined) (469, 92) 0.500 ± 0.003 (0.624, 0.639) −0.015 ± 0.030 −1.484 2 54.5 kg ≤ weight <58.5 kg (183, 54) 0.456 ± 0.007 (0.656, 0.678) −0.022 ± 0.042 −1.195 3 Weight ≥58.5 kg, height ≥167.5 cm (286, 38) 0.532 ± 0.005 (0.595, 0.603) −0.008 ± 0.043 −0.924 DXA-preferred subgroup (node 4) (1262, 245) 0.748 ± 0.002 (0.664, 0.600) 0.064 ± 0.021 1.699 4 Weight ≥58.5 kg, height <167.5 cm (1262, 245) 0.748 ± 0.002 (0.664, 0.600) 0.064 ± 0.021 1.699 Total (nodes 1–4 combined) (1951, 371) 0.484 ± 0.004 (0.653, 0.623) 0.030 ± 0.016 0.013

AUC, area under the receiver-operating characteristic curve; DXA, dual x-ray absorptiometry; QUS, quantitative ultrasound; SE, standard error.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Weighted receiver-operating characteristic curves for three decision subgroups. DXA, dual x-ray absorptiometry; QUS, quantitative ultrasound.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TreestructuredSubgroupAnalysisofReceiverOperatingCharacteristicCurvesforDiagnosticTests/3_1s20S1076633212004746.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A

## Criterion for Splitting and Diagnostic Test Selection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

d(h)=T1I(ˆ1−ˆ2>δ)+T2I(ˆ1−ˆ2≤δ),
d

(

h

)

=

T

1

I

(

ˆ

1

−

ˆ

2

>

δ

)

+

T

2

I

(

ˆ

1

−

ˆ

2

≤

δ

)

,


where _I_ ( _E_ ) is the binary indication function of event _E_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

g(s,h\|δ)=w(h(L)s)\[ˆd(h(L)s)(h(L)s)−ˆd(h)(h(L)s)\]+w(h(R)s)\[ˆd(h(R)s)(h(R)s)−ˆd(h)(h(R)s)\]+w(h(L)s){I\[d(h(L)s)=T2\]−I\[d(h)=T2\]}δ+w(h(R)s){I\[d(h(R)s)=T2\]−I\[d(h)=T2\]}δ
g

(

s

,

h

\|

δ

)

=

w

(

h

s

(

L

)

)

\[

ˆ

d

(

h

s

(

L

)

)

(

h

s

(

L

)

)

−

ˆ

d

(

h

)

(

h

s

(

L

)

)

\]

+

w

(

h

s

(

R

)

)

\[

ˆ

d

(

h

s

(

R

)

)

(

h

s

(

R

)

)

−

ˆ

d

(

h

)

(

h

s

(

R

)

)

\]

+

w

(

h

s

(

L

)

)

{

I

\[

d

(

h

s

(

L

)

)

=

T

2

\]

−

I

\[

d

(

h

)

=

T

2

\]

}

δ

+

w

(

h

s

(

R

)

)

{

I

\[

d

(

h

s

(

R

)

)

=

T

2

\]

−

I

\[

d

(

h

)

=

T

2

\]

}

δ


where w(h(L)s)
w

(

h

s

(

L

)

)
and w(h(R)s)
w

(

h

s

(

R

)

)
are weights on daughter nodes h(L)s
h

s

(

L

)
and h(R)s
h

s

(

R

)
, given by


w(h(L)s)=n0(h(L)s)n1(h(L)s)n0(h(L)s)n1(h(L)s)+n0(h(R)s)n1(h(R)s)
w

(

h

s

(

L

)

)

=

n

0

(

h

s

(

L

)

)

n

1

(

h

s

(

L

)

)

n

0

(

h

s

(

L

)

)

n

1

(

h

s

(

L

)

)

+

n

0

(

h

s

(

R

)

)

n

1

(

h

s

(

R

)

)


and


w(h(R)s)=n0(h(R)s)n1(h(R)s)n0(h(L)s)n1(h(L)s)+n0(h(R)s)n1(h(R)s).
w

(

h

s

(

R

)

)

=

n

0

(

h

s

(

R

)

)

n

1

(

h

s

(

R

)

)

n

0

(

h

s

(

L

)

)

n

1

(

h

s

(

L

)

)

+

n

0

(

h

s

(

R

)

)

n

1

(

h

s

(

R

)

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

sh=argmaxs{g(s,h\|δ)vaˆr\[g(s,h\|δ)\]√∣∣∣g(s,h\|δ)>0},
s

h

=

arg

max

s

{

g

(

s

,

h

\|

δ

)

v

a

ˆ

r

\[

g

(

s

,

h

\|

δ

)

\]

\|

g

(

s

,

h

\|

δ

)

>

0

}

,


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix B

## Construction of the Random Forest

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix C

## Construction of Final Regression Decision Tree

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Schott A.M., Koupa B.K., Hans D., et. al.: Should age influence the choice of quantitative bone assessment technique in elderly women? The EPIDOS study. Osteoporos Int 2004; 15: pp. 196-203.


- 2\. Metz C.E.: Basic principles of ROC analysis. Semin Nucl Med 1978; 8: pp. 283-298.


- 3\. Samuelson F., Gallas B.D., Myers K.J., et. al.: The importance of ROC data. Acad Radiol 2011; 18: pp. 257-258.


- 4\. Pepe M.S.: Three approaches to regression analysis of receiver operating characteristic curves for continuous test results. Biometrics 1998; 54: pp. 124-135.


- 5\. Ciampi A., Negassa A., Lou Z.: Tree-structured subgroup analysis for censored survival data and the Cox model. J Clin Epidemiol 1995; 48: pp. 675-689.


- 6\. Negassa A., Ciampi A., Abrahamowicz M., et. al.: Tree-structured subgroup analysis for censored survival data: validation of computationally inexpensive model selection criteria. Stat Comput 2005; 15: pp. 231-239.


- 7\. Glüer C.C., Eastell R., Reid D.M., et. al.: Association of five quantitative ultrasound devices and bone densitometry with osteoporotic vertebral fractures in a population-based sample: the OPUS study. J Bone Miner Res 2004; 19: pp. 782-793.


- 8\. Breiman L., Friedman J.H., Olshen R.A., et. al.: Classification and Regression Trees.1984.Chapman & HallNew York


- 9\. Breiman L.: Bagging predictors. Mach Learn 1996; 24: pp. 123-140.


- 10\. Metz C.E.: ROC methodology in radiologic imaging. Invest Radiol 1986; 21: pp. 720-733.


- 11\. Metz C.E., Herman B.A., Shen J.-H.: Maximum-likelihood estimation of ROC curves from continuously-distributed data. Stat Med 1998; 17: pp. 1033-1053.


- 12\.  Metz CE. ROCFIT. Available at:  http://metz-roc.uchicago.edu  . Accessed August 3, 2012.


- 13\. Pesce L.L., Horsch K., Drukker K., et. al.: Semiparametric estimation of the relationship between ROC operating points and the test-result scale: application to the proper binormal model. Acad Radiol 2011; 18: pp. 1537-1548.


- 14\. Delong E.R., Delong D.M., Clarke-Pearson D.L.: Comparing the areas under a receive operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 15\. Jin H., Lu Y.: A procedure for determining whether a simple combination of diagnostic tests may be non-inferior to the theoretical optimum combination. Med Decis Making 2008; 28: pp. 909-916.


- 16\.  Study of Osteoporotic Fractures. Available at:  http://sof.ucsf.edu/Interface/  . Accessed August 3, 2012.


- 17\. Cummings S.R., Black D.M., Nevitt M.C., et. al.: The Study of Osteoporotic Fractures Research Group. Bone density at various sites for prediction of hip fractures. Lancet 1993; 341: pp. 72-75.


- 18\. Lu Y., Black D., Mathur A.K., et. al.: Study of hip fracture risk using tree structured survival analysis. J Miner Stoffwechs 2003; 10: pp. 11-16.


- 19\. Jin H., Lu Y., Harris S.T., et. al.: Classification algorithm for hip fracture prediction based on recursive partitioning methods. Med Decis Making 2004; 24: pp. 386-398.


- 20\. Jin H., Lu Y., Stone K., et. al.: Alternative tree structured survival analysis based on variance of survival time. Med Decis Making 2004; 24: pp. 670-680.


- 21\. Liu H., Lan Y., Xu X., et. al.: Fissures segmentation using surface features: content-based retrieval for mammographic mass using ensemble classifier. Acad Radiol 2011; 18: pp. 1475-1484.


- 22\. Paquerault S., Hardy P.T., et. al.: Investigation of optimal use of computer-aided detection systems: the role of the “machine” in decision making process. Acad Radiol 2010; 17: pp. 1112-1121.


- 23\. Tromp A.M., Smit J.H., Deeg D.J.H., et. al.: Quantitative ultrasound measurements of the tibia and calcaneus in comparison with DXA measurements at various skeletal sites. Osteoporos Int 1999; 9: pp. 230-235.


- 24\. Hans D., Schott A.M., Arlot M.E., et. al.: Influence of anthropometric parameters on ultrasound measurements of oscalcis. Osteoporos Int 1995; 5: pp. 371-376.


- 25\. Glüer C.C.: International Quantitative Ultrasound Consensus Group. Quantitative ultrasound techniques for the assessment of osteoporosis: expert agreement on current status. J Bone Miner Res 1997; 12: pp. 1280-1288.