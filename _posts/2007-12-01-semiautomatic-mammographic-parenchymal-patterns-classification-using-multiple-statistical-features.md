---
title: Semiautomatic Mammographic Parenchymal Patterns Classification Using Multiple Statistical Features
author: [CL_AT_CyrilCastellaMSc,CL_AT_KarenKinkelMD,CL_AT_MiguelPEcksteinPhD,CL_AT_PierreEdouardSottasPhD,CL_AT_FrancisRVerdunPhD,CL_AT_FranoisOBochudPhD]
date: 2007-12-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 14, Issue 12]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Our project was to investigate a complete methodology for the semiautomatic assessment of digital mammograms according to their density, an indicator known to be correlated to breast cancer risk. The BI-RADS four-grade density scale is usually employed by radiologists for reporting breast density, but it allows for a certain degree of subjective input, and an objective qualification of density has therefore often been reported hard to assess. The goal of this study was to design an objective technique for determining breast BI-RADS density.

## Materials and Methods

The proposed semiautomatic method makes use of complementary pattern recognition techniques to describe manually selected regions of interest (ROIs) in the breast with 36 statistical features. Three different classifiers based on a linear discriminant analysis or Bayesian theories were designed and tested on a database consisting of 1408 ROIs from 88 patients, using a leave-one-ROI-out technique. Classifications in optimal feature subspaces with lower dimensionality and reduction to a two-class problem were studied as well.

## Results

Comparison with a reference established by the classifications of three radiologists shows excellent performance of the classifiers, even though extremely dense breasts continue to remain more difficult to classify accurately. For the two best classifiers, the exact agreement percentages are 76% and above, and weighted κ values are 0.78 and 0.83. Furthermore, classification in lower dimensional spaces and two-class problems give excellent results.

## Conclusion

The proposed semiautomatic classifiers method provides an objective and reproducible method for characterizing breast density, especially for the two-class case. It represents a simple and valuable tool that could be used in screening programs, training, education, or for optimizing image processing in diagnostic tasks.

While the etiology of breast cancer remains unclear, many studies have demonstrated a correlation between cancer risk and factors such as age, breastfeeding and pregnancy history, family history of breast cancer, hormonal treatments, genetic factors, and breast density ( ). Breast density as a factor of risk was first investigated by Wolfe ( ), who defined a four-grade density scale on the basis of the patterns and textures observed on mammograms. Later, the BI-RADS (Breast Imaging Reporting Data System) density scale was developed by the American College of Radiology to standardize mammography reporting terminology and assessment and recommendation categories ( ). The BI-RADS density classification was created to inform referring physicians about the decline in sensitivity of mammography with increasing breast density. BI-RADS defines breast density 1 as almost entirely fatty, density 2 as scattered fibroglandular tissue, density 3 as heterogeneously dense tissue and density 4 as extremely dense tissues. It was not intended to serve as a method of measuring breast density percentage, although as per Wolfe’s scale ( ), correlations with this more objective factor do exist ( ). In clinical American and European conditions, the breast density of a given patient is typically evaluated and reported by a radiologist using BI-RADS on the basis of the simultaneous display of two mammograms per breast.

However, one of the difficulties for correctly assessing breast density is that the BI-RADS density scale definitions are rather subjective. A certain interpretational freedom prevents perfect interobserver and even intraobserver reproducibility ( ). On the other hand, numerous pattern recognition and classification techniques have been developed and can be directly applied to this task ( ). This is why different statistical approaches have been explored in the last few years in order to develop an objective classifier of mammograms according to Wolfe or the BI-RADS scale. These techniques have made use of various pattern recognition parameters to statistically describe the whole breast or part of it: fractal dimension ( ), gray level histogram properties ( ), moments ( ), gray level variations matrices ( ), or maximum response filters ( ). These descriptions have been combined with several general classification algorithms: Bayesian classification ( ), linear discriminant analysis (LDA) ( ), nearest neighbor rules ( ), neural networks, and textons ( ).

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Mammogram Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Selection of Regions of Interest

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Digital mammogram and corresponding manually defined regions of interest.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticMammographicParenchymalPatternsClassificationUsingMultipleStatisticalFeatures/0_1s20S1076633207004059.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Description

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Summary of the Texture Analysis Methods and the Corresponding Features


Analysis Method Statistical Features Gray level histogram standard deviation skewness kurtosis balance Gray level co-occurrence matrices energy entropy cmax contrast homogeneity Primitives matrices short primitive emphasis long primitive emphasis gray level uniformity primitive length uniformity Fractal analysis fractal dimension Neighbourhood gray-tone difference matrix

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


The 18 parameters in this table were computed for two scales as described in the text, making a total of 36 features.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Definition of Gold Standard From Radiologists’ Ratings

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classification Algorithms

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classic Bayesian classifier based on Mahalanobis distance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ψk(v)=1(2π)NdetKk√⋅exp\[−12(v−μk)TK−1k(v−μk)\],
ψ

k

(

v

)

=

1

(

2

π

)

N

det

⁡

K

k

⋅

exp

⁡

\[

−

1

2

(

v

−

μ

k

)

T

K

k

−

1

(

v

−

μ

k

)

\]

,


where μ  k represents the mean vector of class _k_ and K  k is the covariance matrix of vectors in class _k_ :


μk=1nk∑vi∈Skvi
μ

k

=

1

n

k

∑

v

i

∈

S

k

v

i


Kk=1nk−1∑vi∈Sk(vi−μk)T(vi−μk)
K

k

=

1

n

k

−

1

∑

v

i

∈

S

k

(

v

i

−

μ

k

)

T

(

v

i

−

μ

k

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

p(k∣∣v)=p(v\|k)p(k)p(v)=ψk(v)pa(k)∑kψk(v)pa(k)
p

(

k

\|

v

)

=

p

(

v

\|

k

)

p

(

k

)

p

(

v

)

=

ψ

k

(

v

)

p

a

(

k

)

∑

k

ψ

k

(

v

)

p

a

(

k

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

cR=∑4k=1k⋅p(k\|v),
c

R

=

∑

k

=

1

4

k

⋅

p

(

k

\|

v

)

,


with c  R being rounded to the nearest integer value to obtain the class attributed to the tested sample vector v.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

pa(k)=14,
p

a

(

k

)

=

1

4

,


which represents the most conservative a priori assumption.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Naïve Bayesian classifier

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ψk(vn,k)=1(2π)N√exp\[−12vTn,kvn,k\],
ψ

k

(

v

n

,

k

)

=

1

(

2

π

)

N

exp

⁡

\[

−

1

2

v

n

,

k

T

v

n

,

k

\]

,


where v has been normalized in the same way as training samples of class _k_ to obtain the normalized vector v _n,k_ . The four a posteriori probabilities p( _k_ \|v) were then computed with Equation  4 , and the attributed class with Equation  5 .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

12π√∫−∞pj,kne−t2/2dt=pj,kpj,kmax,
1

2

π

∫

−

∞

p

n

j

,

k

e

−

t

2

/

2

d

t

=

p

j

,

k

p

max

⁡

j

,

k

,


where _p  j,k  max_ is the highest value in the original distribution of feature _j_ in class _k_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Linear discriminant analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ψk(v)=1(2π)NdetKo√⋅exp\[−12(v−μk)TK−1o(v−μk)\]
ψ

k

(

v

)

=

1

(

2

π

)

N

det

⁡

K

o

⋅

exp

⁡

\[

−

1

2

(

v

−

μ

k

)

T

K

o

−

1

(

v

−

μ

k

)

\]


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Averaging the individual ROIs classifications

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reduction of the features’ space size and number of classes

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation of the performance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

κ=po−pe1−pe,
κ

=

p

o

−

p

e

1

−

p

e

,


where _p  o_ is the observed agreement proportion and _p  e_ the agreement expected by chance alone. Both are calculated from the confusion matrix and the quadratic weights matrix, and the values of κ stand between −1 and 1 (the minimum value actually depends on _p  e_ but is always between −1 and 0). Benchmarks by Landis and Koch ( ) (adjusted by Fleiss et al. \[41\] for taking the weighting process into account) are commonly used: κ values below 0.4 reflect poor agreement, between 0.4 and 0.6 moderate agreement, while it is substantial between 0.6 and 0.75 and excellent above 0.75. Weighted κ is particularly well adapted to multiclass tasks and when the classes are rather subjectively defined, which is the case for the BI-RADS density scale. The weighting process indeed differentiates between serious (more than one BI-RADS class difference) and slight disagreement (immediate neighbor class choice), and has been chosen as an evaluation parameter in numerous previous works on mammogram classification ( ). Although much more sensitive to differences in class prevalence, the exact agreement proportion was also computed to be able to compare the performance with results from other studies ( ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Radiologist Classifications Compared to the Gold Standard Classification Defined in Text


Radiologist # 1 Radiologist # 2 Radiologist # 3 Kappa 0.81 ± 0.07 0.88 ± 0.07 0.91 ± 0.08 Exact agreement 77% 89% 89%

Standard error for weighted κ was computed according to the formula given by Fleiss et al. ( ).


![Figure 2, Repartition of the 176 breast pairs among BI-RADS density classes. The separation line in the gold standard column indicates the proportion of cases per consensus level: 3/3 (lower part of the column) or 2/3 (upper part).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticMammographicParenchymalPatternsClassificationUsingMultipleStatisticalFeatures/1_1s20S1076633207004059.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


(a) Confusion Matrix Obtained for the Bayesian Classifier Based on Mahalanobis Distance. Results are Averaged Over Mammogram Pairs from the Same View. (b) Same for LDA Classifier


(a) Gold Standard Bayesian Classifier Density 1 Density 2 Density 3 Density 4 Density 1 14 3 0 0 Density 2 5 30 6 1 Density 3 0 14 86 3 Density 4 0 0 10 4

(b) Gold Standard LDA Classifier Density 1 Density 2 Density 3 Density 4 Density 1 16 3 0 0 Density 2 3 31 4 1 Density 3 0 13 95 3 Density 4 0 0 3 4

Table 4


Weighted κ Values Obtained with the Different Averaging Processes and Classifiers. Exact Agreement is Given in Parenthesis


Individual ROI Classification Average per Mammogram (4 ROIs) Average per View Type (8 ROIs) Naïve Bayesian 0.50 ± 0.02 (39%) 0.65 ± 0.05 (55%) 0.68 ± 0.07 (60%) Mahalanobis Bayesian 0.58 ± 0.03 (53%) 0.73 ± 0.05 (69%) 0.78 ± 0.07 (76%) LDA 0.71 ± 0.03 (70%) 0.81 ± 0.05 (80%) 0.83 ± 0.08 (83%)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, ( a ) Weighted κ value as a function of the features space dimensionality. Lines at 0.6 and 0.75 represent the limits for substantial and excellent agreement. ( b ) Corresponding percentage agreement.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticMammographicParenchymalPatternsClassificationUsingMultipleStatisticalFeatures/2_1s20S1076633207004059.jpg)

![Figure 4, Partition of the optimal bidimensional feature subspace. ( a ) LDA leads to linear borders. ( b ) For Bayesian classifier based on Mahalanobis distance, the borders are conics. For visibility reasons, only 40 to 50 randomly chosen ROIs per density class are shown.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticMammographicParenchymalPatternsClassificationUsingMultipleStatisticalFeatures/3_1s20S1076633207004059.jpg)

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## Definition of the statistical parameters

## Parameters Computed From the Gray Level Histogram

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

mean≡x¯=1N∑ixi
mean

≡

x

¯

=

1

N

∑

i

x

i


standarddev.≡σ=1N−1√(∑i(xi−x¯)2)1/2
standard

dev

.

≡

σ

=

1

N

−

1

(

∑

i

(

x

i

−

x

¯

)

2

)

1

/

2


skewness=1Nσ3∑i(xi−x¯)3
skewness

=

1

N

σ

3

∑

i

(

x

i

−

x

¯

)

3


kurtosis=1Nσ4∑i(xi−x¯)4−3
kurtosis

=

1

N

σ

4

∑

i

(

x

i

−

x

¯

)

4

−

3


balance=x70−x¯x¯−x30,
balance

=

x

70

−

x

¯

x

¯

−

x

30

,


where the summations are performed over the N pixels of the ROI, and _x  p_ is the gray level yielding to _p_ th percentile of the gray level distribution ( ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Gray Level Co-occurrence Matrices (GLCM)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

energy(C)=∑i,jC2i,j
energy

(

C

)

=

∑

i

,

j

C

i

,

j

2


entropy(C)=−∑i,jCi,jlogCi,j
entropy

(

C

)

=

−

∑

i

,

j

C

i

,

j

log

⁡

C

i

,

j


cmax(C)=maxi,jCi,j
c

max

(

C

)

=

max

⁡

i

,

j

C

i

,

j


contrast(C)=∑i,j\|i−j\|2Ci,j
contrast

(

C

)

=

∑

i

,

j

\|

i

−

j

\|

2

C

i

,

j


homogeneity(C)=∑i,jCi,j1+\|i−j\|
homogeneity

(

C

)

=

∑

i

,

j

C

i

,

j

1

+

\|

i

−

j

\|


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Primitives Matrix (PM)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

spe=1Btot∑a∑rBa,rr2
spe

=

1

B

t

o

t

∑

a

∑

r

B

a

,

r

r

2


lpe=1Btot∑a∑rBa,rr2
lpe

=

1

B

t

o

t

∑

a

∑

r

B

a

,

r

r

2


glu=1Btot∑a(∑rBa,r)2
glu

=

1

B

t

o

t

∑

a

(

∑

r

B

a

,

r

)

2


plu=1Btot∑r(∑aBa,r)2,
plu

=

1

B

t

o

t

∑

r

(

∑

a

B

a

,

r

)

2

,


where **B**_tot_ is the sum of the elements of the primitives matrix **B** : Btot=∑a∑rBa,r.
B

t

o

t

=

∑

a

∑

r

B

a

,

r

.
Note that **B** could be defined for several directions, but we limited our investigations to one ( ), corresponding to a scan of the image along direction \[1,0\].


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Fractal Dimension

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

L(ε)=λε1−D
L

(

ε

)

=

λ

ε

1

−

D


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

A(ε)=λε2−D
A

(

ε

)

=

λ

ε

2

−

D


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Neighborhood Gray-Tone Difference Matrix (NGTDM)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

A¯¯¯xk,l=1W−1\[∑dm=−d∑dn=−dxk+m,l+n\],(m,n)≠(0,0),
A

¯

x

k

,

l

=

1

W

−

1

\[

∑

m

=

−

d

d

∑

n

=

−

d

d

x

k

+

m

,

l

+

n

\]

,

(

m

,

n

)

≠

(

0

,

0

)

,


where d = 3 is the neighbouring size and W = (2d+1)  2 . Denoting { _X  i_ } the set of all pixels with value _i_ in the ROI, the _i_ th entry of the NGTDM is given by:


s(i)=∑x∈Xi∣∣i−A¯¯¯x∣∣
s

(

i

)

=

∑

x

∈

X

i

\|

i

−

A

¯

x

\|


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

coarseness=\[ε+∑imaxi=0pis(i)\]−1
c

o

a

r

s

e

n

e

s

s

=

\[

ε

+

∑

i

=

0

i

max

⁡

p

i

s

(

i

)

\]

−

1


contrast′=\[1Ng(Ng−1)∑imaxi=0∑jmaxj=0pipj(i−j)2\]⋅\[1n2∑imaxi=0s(i)\]
contrast

′

=

\[

1

N

g

(

N

g

−

1

)

∑

i

=

0

i

max

⁡

∑

j

=

0

j

max

⁡

p

i

p

j

(

i

−

j

)

2

\]

·

\[

1

n

2

∑

i

=

0

i

max

⁡

s

(

i

)

\]


complexity=∑imaxi=0∑jmaxj=0\|i−j\|\[pis(i)+pjs(j)\]n2(pi+pj),pi>0,pj>0
complexity

=

∑

i

=

0

i

max

⁡

∑

j

=

0

j

max

⁡

\|

i

−

j

\|

\[

p

i

s

(

i

)

+

p

j

s

(

j

)

\]

n

2

(

p

i

+

p

j

)

,

p

i

>

0

,

p

j

>

0


strength=∑imaxi=0∑jmaxj=0(pi+pj)(i−j)2ε+∑imaxi=0s(i),pi>0,pj>0,
strength

=

∑

i

=

0

i

max

⁡

∑

j

=

0

j

max

⁡

(

p

i

+

p

j

)

(

i

−

j

)

2

ε

+

∑

i

=

0

i

max

⁡

s

(

i

)

,

p

i

>

0

,

p

j

>

0

,


where pi=\|Xi\|/∑imaxi=0\|Xi\|
p

i

=

\|

X

i

\|

/

∑

i

=

0

i

max

⁡

\|

X

i

\|
is the probability of occurrence of gray level _i_ in the ROI, _i_ max the highest gray level and _N  g_ the number of different gray levels effectively present in the ROI and ε a small number (10  −12 in our case) to prevent coarseness and strength becoming infinite. The feature representing the contrast given by Equation  30 is called here _contrast′_ , to make a distinction with the contrast derived from the primitives matrices (see Equation  19 ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Fitzgibbons P.L., Page D.L., Weaver D., et. al.: Prognostic factors in breast cancer. Arch Pathol Lab Med 2000; 124: pp. 966-978.


- 2\. Ziv E., Smith-Bindman R., Kerlikowske K.: Mammographic breast density and family history of breast cancer. J Natl Cancer Inst 2003; 95: pp. 556-558.


- 3\. Colditz G.A., Hankison S.E., Hunter D.J., et. al.: The use of estrogens and progestins and the risk of breast cancer in postmenopausal women. N Engl J Med 1995; 332: pp. 1589-1593.


- 4\. Kelsey J.L., Gammon M.D., John E.M.: Reproductive factors and breast cancer. Epidemiol Rev 1993; 15: pp. 36-47.


- 5\. Boyd N.F., Byng J.W., Long R.A., et. al.: Quantitative classification of mammographic densities and breast cancer risk: Results from the Canadian National Breast Screening study. J Natl Cancer Inst 1995; 87: pp. 670-675.


- 6\. van Gils C.H., Hendriks J.H., Holland R., et. al.: Changes in mammographic breast density and concomitant changes in breast cancer risk. Eur J Cancer Prev 1999; 8: pp. 509-515.


- 7\. Heine J.J., Malhotra P.: Mammographic tissue, breast cancer risk, serial image analysis, and digital mammography: Part 1. Acad Radiol 2001; 9: pp. 298-316.


- 8\. Wolfe J.N.: Breast patterns as an index of risk for developing breast cancer. AJR Am J Roentgenol 1976; 126: pp. 1130-1137.


- 9\. American College of Radiology (ACR) 2004: ACR Practice Guideline for the performance of screening mammography.2004.


- 10\. Harvey J.A., Bovbjerg V.E.: Quantitative assessment of mammographic breast density: relationship with breast cancer risk. Radiology 2004; 230: pp. 29-41.


- 11\. Brisson J., Diorio C., Mâsse B.: Wolfe’s parenchymal pattern and percentage of the breast with mammographic densities: Redundant or complementary classifications?. Cancer Epidemiol Biomark Prevent 2003; 12: pp. 728-732.


- 12\. Perconti P., Loew M.: Analysis of parenchymal patterns using conspicuous spatial frequency features in mammograms applied to the BI-RADS density rating scheme.2006.


- 13\. Kerlikowske K., Grady D., Barclay J., et. al.: Variability and accuracy in mammographic interpretation using the American College of Radiology Breast Imaging Reporting and Data System. J Natl Cancer Inst 1998; 90: pp. 1801-1809.


- 14\. Berg W.A., Campassi C., Langenberg P., Sexton M.J.: Breast Imaging Reporting and Data System: Inter- and intraobserver variability in feature analysis and final assessment. AJR Am J Roentgenol 2000; 174: pp. 1769-1777.


- 15\. Huo Z., Giger M.L., Wolverton D.E., Zhong W., Cumming S., Olopade O.I.: Computerized analysis of mammographic parenchymal patterns for breast cancer assessment: Feature selection. Med Phys 2000; 27: pp. 4-12.


- 16\. Caldwell C.B., Stappelton S.J., Holdsworth D.W., et. al.: Characterisation of mammographic parenchymal pattern by fractal dimension. Phys Med Biol 1990; 35: pp. 235-247.


- 17\. Byng J.W., Boyd N.F., Fishel E., Jong R.A., Yaffe M.J.: Automated analysis of mammographic densities. Phys Med Biol 1996; 41: pp. 909-923.


- 18\. Bovis K., Singh S.: Classification of mammographic breast density using a combined classifier paradigm. Proceedings of the 4th International Workshop on Digital Mammography 2002; pp. 177-180.


- 19\. Zhou C., Chan H.P., Petrick N., et. al.: Computerized image analysis: Estimation of breast density on mammograms. Med Phys 2001; 28: pp. 1056-1569.


- 20\. Tahoces P.G., Correa J., Souto M., Gómez L., Vidal J.J.: Computer-aided diagnosis: The classification of mammographic breast parenchymal patterns. Phys Med Biol 1995; 40: pp. 103-117.


- 21\. Karssemeijer N.: Automated classification of parenchymal patterns in mammograms. Phys Med Biol 1998; 43: pp. 365-378.


- 22\. Petroudi S., Kadir T., Brady M.: Automatic classification of mammographic parenchymal patterns: A statistical approach. Proc IEEE Int Conf Eng Med Biol 2003; pp. 798-801.


- 23\. Vedantham S., Karellas A., Suryanarayanan S., et. al.: Full breast digital mammography with an amorphous silicon-based flat panel detector: Physical characteristics of a clinical prototype. Med Phys 2000; 27: pp. 558-567.


- 24\. Burgess A.: On the noise variance of a digital mammography system. Med Phys 2004; 31: pp. 1987-1995.


- 25\. Muller S.: Full-field digital mammography designed as a complete system. Eur J Radiol 1999; 31: pp. 25-34.


- 26\. Hemdal B., Andersson I., Grahn A., et. al.: Can the average glandular dose in routine digital mammography screening be reduced?. Radiat Protect Dosimetry 2005; 114: pp. 383-388.


- 27\. Li H., Giger M.L., Olopade O.I., Margolis A., Lan L., Chinander M.R.: Computerized texture analysis of mammographic parenchymal patterns of digitized mammograms. Acad Radiol 2005; 12: pp. 863-873.


- 28\. Sonka M., Hlavak V., Boyle R.: Image processing.2nd ed.1999.Brooks/ColePacific Grove, CA


- 29\. Tuceryan M., Jain A.K.: Texture analysis.Chen C.H.Pau L.F.Wang P.The Handbook of Pattern Recognition and Computer Vision.1998.World Scientific PublishingRiver Edge, NJ:


- 30\. Haralick R.M., Shanmugam K., Dinstein I.: Textural features for image classification. IEEE Trans Syst Manage Cybern 1973; 3: pp. 610-662.


- 31\. Lundhal T., Ohley W.J., Kunklinski W.S., Williams D.O., Gewirtz H., Most A.S.: Analysis and interpolation of angiographic images by use of fractals. Proceedings of IEEE Conference on Computers in Cardiology 1985; pp. 355-358.


- 32\. Amadasun M., King R.: Textural features corresponding to textural properties. IEEE Trans Syst Manage Cybern 1989; 19: pp. 1264-1274.


- 33\. Fukunaga K.: Introduction to Statistical Pattern Recognition.2nd ed.1990.Academic PressSan Diego, CA


- 34\. Chabat F., Guang-Zhong Y., Mansell D.M.: Obstructive lung diseases: Texture classification for differentiation at CT. Radiology 2003; 228: pp. 871-877.


- 35\. Friedman N., Geiger D., Goldszmidt M.: Bayesian network classifier. Machine Learning 1997; 29: pp. 131-163.


- 36\. Domingos P., Pazzani M.J.: On the optimality of the simple Bayesian classifier under zero-one loss. Machine Learning 1997; 29: pp. 103-130.


- 37\. 2004.MathWorksNatick, MA


- 38\. Nasri M., El Hitmy M.: Algorithme génétique et Critère de la Trace pour l’Optimisation du vecteur Attribut: Application à la Classification Supervisée des Images de Textures.2002.


- 39\. Yeom S., Javidi B.: Three-dimensional distortion-tolerant object recognition using integral imaging. Optics Express 2004; 12: pp. 5795-5809.


- 40\. Barrett H.H., Myers K.J.: Foundations of Image Science.2004.WileyHoboken, NJ


- 41\. Fleiss J.L., Levin B., Paik M.C.: Statistical Rates and Proportions.3rd ed.2003.WileyHoboken, NJ


- 42\. Ker M.: Issues in the use of kappa. Invest Radiol 1991; 26: pp. 78-83.


- 43\. Kundel H.L.: Measurement of Observer Agreement. Radiology 2003; 228: pp. 303-308.


- 44\. Kraemer H.C.: Extension of the kappa coefficient. Biometrics 1980; 36: pp. 207-216.


- 45\. Kraemer H.C., Periyakoil V.S., Noda A.: Kappa coefficients in medical research.D’Agostino R.B.2004.WileyHoboken, NJ:


- 46\. Landis J.R., Koch G.G.: The measurement of observer agreement for categorical data. Biometrics 1973; 33: pp. 671-679.


- 47\. Petroudi S., Brady M.: Proceedings of the 8th International Workshop on Digital Mammography.Proceedings of the 8th International Workshop on Digital Mammography.2006.SpringerBerlin/Heidelberg:pp. 609-615.


- 48\. Mandelbrot B.B.: The Fractal Geometry of Nature.1982.WH FreemanSan Francisco, CA