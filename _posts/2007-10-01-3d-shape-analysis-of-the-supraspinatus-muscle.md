---
title: 3D Shape Analysis of the Supraspinatus Muscle
author: [CL_AT_AaronDWardMSc,CL_AT_GhassanHamarnehPhD,CL_AT_ReemAshryMD,CL_AT_MarkESchweitzerMD]
date: 2007-10-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 14, Issue 10]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Rotator cuff disorders are prevalent and can cause pain and reduced range of motion and strength. Accurate, noninvasive diagnosis of rotator cuff disorders is therefore important. In this work, we study the relationship between several three-dimensional (3D) shape measurements of the supraspinatus and its pathologic conditions. The objective is to explore the utility of 3D shape descriptors in distinguishing supraspinatus pathologies, leading to computer-aided diagnosis of rotator cuff disorders.

## Materials and Methods

We acquired magnetic resonance images of the shoulder from 73 patients, separated into five pathology groups: normal ( ), tear ( ), tear and atrophy ( ), tear and retraction ( ), and tear and atrophy and retraction ( ). We segmented the 3D surface of the supraspinatus from each magnetic resonance image, and computed 11 3D shape characteristics for each. We performed an analysis of variance (ANOVA) test for each measurement to test the null hypothesis that the means of the pathology groups were equal. The most promising of the measurements, as determined by the ANOVA test, were used to train a support vector machine classifier to automatically assign new supraspinata to the correct pathology groups.

## Results

The ANOVA test results rejected the null hypothesis ( _p_ < .0045) for 7 of our 11 measurements. Highlights of the results from the support vector machine classifier were 79% accuracy in distinguishing normals from abnormals, and 82% accuracy in distinguishing atrophy from retraction, our main clinical motivation. These scores were tabulated based on leave-one-out cross-validation.

## Conclusion

From the results, we draw the conclusion that 3D shape analysis may be helpful in the diagnosis of rotator cuff disorders, but further investigation is required to develop a 3D shape descriptor that yields ideal pathology group separation. The results of this study suggest several promising avenues of future research to meet this goal.

The rotator cuff comprises several muscles and tendons that stabilize the shoulder, including the supraspinatus (  Fig 1 ). Disorders of the rotator cuff are prevalent; incidence of disorder has been found to be 34% of asymptomatic individuals in a study where diagnosis was performed on magnetic resonance images (MRI) ( ), and 30% of individuals older than 60 years of age in a cadaveric study ( ). Symptoms of rotator cuff disorder can be debilitating, including pain, weakness, and limited range of motion, especially for overhead work ( ). Disorders of the supraspinatus muscle may involve tearing, which can lead to muscle retraction, atrophy, or both ( ). It is important to be able to distinguish between retraction and atrophy because retraction is a condition that is repairable by pulling the muscle forward in surgery, whereas atrophy is a condition uncorrectable by surgery. Because both of these conditions result in a reduction of the apparent size of the muscle and therefore are difficult to distinguish by size alone, we are motivated to investigate the utility of analyzing the 3D shape of the supraspinatus to discover shape characterizations that may assist the physician in distinguishing between these groups.

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633207X00916/S1076633207003376/gr1.jpg?Signature=S4PCmZv3EJK20vIPqg3CxGR6sB-zvXlKevuCDnXmTXpjM5Ie4dBco42CK72TJ4KsHAjvaVnHehZWyiN8umJUotJhh%7EZOwG9JZ4swWevUxBVeMix9Dex4s2dy4FLMUqMR3kZGdpouKt93PabiC2H%7ELA5f2Pn3JRmNNnhPGePFS5U_&Expires=1669520221&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Diagram of shoulder anatomy indicating the location of the supraspinatus (posterior view). Adapted from Grey’s Anatomy ( ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Description of the Pathology Groups


Abbreviation Number of Patients Pathology Group Normal: No pathology N 14 Abnormal: T, TA, TR, TAR A 59 Abnormal subgroups Tear: Full/partial tear T 20 Tear + atrophy TA 13 Tear + retraction TR 15 Tear + atrophy + retraction TAR 11

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Computational pipeline used in this study. Slice-by-slice segmentation of the supraspinatus from magnetic resonance images leads to a set of sparse surface points, which are interpolated to create a surface in three dimensions (3D). Each muscle is assigned to a pathology group by an expert, and 3D shape measures are computed for each group. Group difference significance is then assessed using analysis of variance testing and training and evaluation of a machine learning algorithm for automated diagnosis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DShapeAnalysisoftheSupraspinatusMuscle/0_1s20S1076633207003376.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Supraspinatus muscle surface segmentation. Contours resulting from expert segmentation of the supraspinatus are shown, rendered (as dark bands) using physical space coordinates. Large spaces between contours are due to the low out-of-plane resolution of the data. Note that contours appear non-parallel because of perspective projection. Also shown is the result of three-dimensional interpolation of the contours, yielding a dense set of points lying on the surface of the supraspinatus, rendered as a surface. The coloring of this surface is according to the mean curvature calculated at each point; higher curvature corresponds to lighter coloring. This surface has been made translucent so that the contours can be clearly seen surrounding the muscle.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DShapeAnalysisoftheSupraspinatusMuscle/1_1s20S1076633207003376.jpg)

![Figure 4, Sample supraspinatus surfaces. Each row shows three samples for each pathology group. (a–c) Normal. (d–f) Tear. (g–i) Tear and atrophy. (j–l) Tear and retraction. (m–o) Tear and atrophy and retraction. The surfaces are shaded according to the computed mean curvature at each point; lighter shading corresponds to higher curvature values.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DShapeAnalysisoftheSupraspinatusMuscle/2_1s20S1076633207003376.jpg)

![Figure 5, Supraspinatus surface, in context. Four views, from different angles, of the same segmented supraspinatus, in context of the magnetic resonance image from which it was segmented. (a) The semitransparent sagittal slices viewed face-on, with the supraspinatus rendered as a hollow region. (b) Image (a) rotated slightly for a different perspective. (c) A view from the side of the shoulder. (d) A view from the top of the shoulder.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DShapeAnalysisoftheSupraspinatusMuscle/3_1s20S1076633207003376.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Descriptions of the measurements taken, with their associated measurement numbers used in this article


Number Description of Measurement 1 Eigenvalue ratio λ  1  /λ  2  2 Eigenvalue ratio λ  1  /λ  3  3 Eigenvalue ratio λ  2  /λ  3  4 Mean of distances to centroid (cm) 5 Standard deviation of distances to centroid (cm) 6 3D moment _J_ 1  7 3D moment _J_ 2  8 3D moment _J_ 3  9 Surface area (cm  2  ) 10 Volume (cm  3  ) 11 Surface area/volume (1/cm)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Ratios of Eigenvalues (Three Measures)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Illustration of the meaning of the relationship of the eigenvalues (resulting from principal components analysis [ 20 ] on shape surface points) to each other. (a) PCA on a set of two-dimensional points: Eigenvalues λ 1 and λ 2 represent the lengths of the vectors along the directions of greatest and second-greatest variation in the data points, respectively. (b) When PCA is done on a set of points lying on a sphere-like shape, eigenvalues tend to be equal. (c) When PCA is done on a set of points lying on a cylinder-like shape, λ 1 tends to be much larger than λ 2 and λ 3 , both of which tend to be equal. (d) PCA on a set of points lying on a disk-like shape yields λ 1 approximately equal to λ 2 , both of which being much larger than λ 3 .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DShapeAnalysisoftheSupraspinatusMuscle/4_1s20S1076633207003376.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Mean and Standard Deviation of Distances to Centroid (Two Measures)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## 3D Moment Invariants (Three Measures)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

J1=μ200+μ020+μ002
J

1

=

μ

200

+

μ

020

+

μ

002


J2=μ200μ020+μ200μ002+μ020μ002−μ2110−μ2101−μ2011
J

2

=

μ

200

μ

020

+

μ

200

μ

002

+

μ

020

μ

002

−

μ

110

2

−

μ

101

2

−

μ

011

2


J3=μ200μ020μ002+2μ110μ101μ011−μ002μ2110−μ020μ2101−μ200μ2011,
J

3

=

μ

200

μ

020

μ

002

+

2

μ

110

μ

101

μ

011

−

μ

002

μ

110

2

−

μ

020

μ

101

2

−

μ

200

μ

011

2

,


where _μ  pqr_ is given by


μpqr=∑x∑y∑z(x−x¯)p(y−y¯)q(z−z¯)rf(x,y,z),
μ

p

q

r

=

∑

x

∑

y

∑

z

(

x

−

x

¯

)

p

(

y

−

y

¯

)

q

(

z

−

z

¯

)

r

f

(

x

,

y

,

z

),


_f_ is given by


f(x,y,z)={1if(x,y,z)isasurfacepoint0otherwise
f

(

x

,

y

,

z

)

=

{

1

if

(

x

,

y

,

z

)

is

a

surface

point

0

otherwise


x¯
x

¯
, y¯
y

¯
, z¯
z

¯
are given by


x¯=m100/m000
x

¯

=

m

100

/

m

000


y¯=m010/m000
y

¯

=

m

010

/

m

000


z¯=m001/m000,
z

¯

=

m

001

/

m

000

,


and _m  pqr_ is given by


mpqr=∑x∑y∑zxpyqzrf(x,y,z).
m

p

q

r

=

∑

x

∑

y

∑

z

x

p

y

q

z

r

f

(

x

,

y

,

z

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Surface Area, Volume, and Their Ratios (Three Measures)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, A plot showing two features, f1 and f2, in 2D feature space. Black points correspond to one group, and red points to another (please see electronic version). The points are projected onto the f1 and f2 axes to illustrate that the group separability is very poor for either of these features taken separately. However, a classifier based on a quadratic decision curve is able to achieve perfect class separation when both features are considered together.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DShapeAnalysisoftheSupraspinatusMuscle/5_1s20S1076633207003376.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Mean ± standard deviation values of each of the measurements for each of the groups


N T TA TR TAR 1 2.4 ± 1.2 2.6 ± 0.90 4.0 ± 2.4 3.5 ± 1.4 3.0 ± 2.1 2 5.7 ± 2.5 6.7 ± 2.3 10 ± 5.7 7.6 ± 2.6 7.4 ± 3.3 3 2.5 ± 0.60 2.6 ± 0.69 2.7 ± 0.75 2.5 ± 0.85 3.0 ± 1.5 4 2.0 ± 0.44 1.8 ± 0.32 1.8 ± 0.34 1.6 ± 0.29 1.6 ± 0.22 5 0.65 ± 0.22 0.66 ± 0.13 0.66 ± 0.11 0.56 ± 0.13 0.6 ± 0.17 6 10.2 × 10  5  ± 9.1 × 10  4  8.7 × 10  4  ± 5.2 × 10  4  6.5 × 10  4  ± 4.2 × 10  2  4.5 × 10  4  ± 2.8 × 10  4  3.7 × 10  4  ± 2.2 × 10  4  7 5.3 × 10  9  ± 6.4 × 10  9  2.7 × 10  9  ± 2.8 × 10  9  1.5 × 10  9  ± 1.9 × 10  9  6.8 × 10  8  ± 7.3 × 10  8  4.6 × 10  8  ± 5.5 × 10  8  8 7.6 × 10  13  ± 1.1 × 10  14  2.6 × 10  13  ± 3.7 × 10  13  1.3 × 10  13  ± 2.2 × 10  13  3.2 × 10  12  ± 4.5 × 10  12  1.7 × 10  12  ± 2.8 × 10  12  9 60 ± 24 49 ± 18 45 ± 22 34 ± 7.6 34 ± 12 10 23 ± 13 15 ± 8.3 15 ± 10 9.1 ± 2.8 7.1 ± 4.7 11 2.8 ± 0.56 3.5 ± 0.80 4.8 ± 1.7 4.1 ± 1.3 5.1 ± 0.89

Please refer to  Tables 1 and 2  for the meanings of the column and row labels, respectively.


Table 4


_p_ Values resulting from a one-way analysis of variance test for each measurement, testing the null hypothesis that the means of the measurements of all of the pathology groups are the same


_p_ Value Mean of distances to centroid (cm) .0039 3D moment _J  1_ .0014 3D moment _J  2_ .0018 3D moment _J  3_ .0027 Surface area (cm  2  ) .0010 Volume (cm  3  ) .000041 Surface area/volume (1/cm) .0000034

Only _p_ values leading to rejection of the null hypothesis ( _p_ < .0045) are shown.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Box plots showing the separability of the pathology groups using the mean of distances to centroid (top), three-dimensional moment J 1 (middle), and ratio of surface area to volume (bottom). The bottom and top of each displayed box plot indicate the first ( Q 1) and third ( Q 3) quartiles of the measurements, respectively. The line in the middle of the box shows the median. The whiskers emanating from the box show the largest and smallest nonoutliers. The + symbols show outliers (defined as being smaller than Q 1 − P or larger than Q 3 + P where P = 1.5 × Q, Q = Q1 − Q3).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DShapeAnalysisoftheSupraspinatusMuscle/6_1s20S1076633207003376.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Automated Classification Results


N T TA TR A 0.79 T 0.70 TA 0.81 0.72 TR 0.79 0.44 0.82 TAR 0.76 0.73 0.50 0.73

Each cell shows the accuracy (1 being perfect accuracy) of a support vector machine trained to distinguish the pathology groups corresponding to the row and column of that cell. Leave-one-out cross-validation was performed, with the results averaged over all rounds. The support vector machine was trained using shape features corresponding to the three smallest _p_ values: surface area, volume, and the surface area to volume ratio. See  Table 1  for abbreviations.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Sher J.S., Uribe J.W., Posada A., et. al.: Abnormal findings on magnetic resonance images of asymptomatic shoulders. J Bone Joint Surg 1995; 77: pp. 10-15.


- 2\. Lehman C., Cuomo F., Kummer F.J., et. al.: The incidence of full thickness rotator cuff tears in a large cadaveric population. Bulle Hosp Joint Dis 1995; 54: pp. 30-31.


- 3\. Ellman H., Hanker G., Bayer M.: Repair of the rotator cuff. J Bone Joint Surg 1986; 68: pp. 1136-1144.


- 4\. Fuchs S., Chylarecki C., Langenbrinck A.: Incidence and symptoms of clinically manifest rotator cuff lesions. A Int J Sports Med 1999; 20: pp. 201-205.


- 5\. Gartsman G.M., Khan M., Hammerman S.M.: Arthroscopic repair of full thickness tears of the rotator cuff. J Bone Joint Surg Am 1998; 80: pp. 832-840.


- 6\. Halder A.M., O’Driscoll S.W., Heers G., et. al.: Biomechanical comparison of effects of supraspinatus tendon detachments, tendon defects, and muscle retractions. J Bone Joint Surg 2002; 84-A: pp. 780-785.


- 7\. Itoi E., Hsu H.-C., Carmichael S.W., et. al.: Morphology of the torn rotator cuff. J Anat 1995; 186: pp. 429-434.


- 8\. Robertson P.L., Schweitzer M.E., Mitchell D.G., et. al.: Rotator cuff disorders: Interobserver and intraobserver variation in diagnosis with MR imaging. Radiology 1995; 194: pp. 831-835.


- 9\. Thomazeau H., Rolland Y., Lucas C., et. al.: Atrophy of the supraspinatus belly. Acta Orthop Scand 1996; 67: pp. 264-268.


- 10\. Gray H.: Anatomy of the human body.1918.Lea and FebigerPhiladelphia, Pa:


- 11\. Fuchs B., Weishaupt D., Zanetti M., et. al.: Fatty degeneration of the muscles of the rotator cuff: Assessment by computed tomography versus magnetic resonance imaging. J Shoulder Elbow Surg 1999; 8: pp. 599-605.


- 12\. Zanetti M., Gerber C., Hodler J.: Quantitative assessment of the muscles of the rotator cuff with magnetic resonance imaging. Investig Radiol 1998; 33: pp. 163-170.


- 13\. Bachmann G.F., Melzer C., Heinrichs C.M., et. al.: Diagnosis of rotator cuff lesions: comparison of US and MRI on 38 joint specimens. Eur Radiol 1997; 7: pp. 192-197.


- 14\. Quinn S.F., Sheley R.C., Demlow T.A., et. al.: Rotator cuff tendon tears: Evaluation with fat-suppressed MR imaging with arthroscopic correlation in 100 patients. Radiology 1995; 195: pp. 497-500.


- 15\. Swen W.A.A., Jacobs J.W.G., Algra P.R., et. al.: Sonography and magnetic resonance imaging equivalent for the assessment of full-thickness rotator cuff tears. Arthritis Rheum 1999; 42: pp. 2231-2238.


- 16\. Zlatkin M., Iannotti J., Roberts M., et. al.: Rotator cuff tears: Diagnostic performance of MR imaging. Radiology 1989; 172: pp. 223-229.


- 17\. Mortensen M.E.: Geometric modeling.1985.John Wiley & Sons, IncNew York


- 18\. Lehtinen J.T., Tingart M.J., Apreleva M., et. al.: Practical assessment of rotator cuff muscle volumes using shoulder MI. Acta Orthop Scand 2003; 74: pp. 722-729.


- 19\. Turk G., O’Brien J.F.: Shape transformation using variational implicit functions. Proc ACM SIGGRAPH 1999; pp. 335-342.


- 20\. Jolliffe I.T.: Principal components analysis.1986.Springer-VerlagNew York


- 21\. Sadjadi F.A., Hall E.L.: Three-dimensional moment invariants. IEEE PAMI 1980; 2: pp. 127-136.


- 22\. Lorensen W.E., Cline H.E.: Marching cubes: A high resolution 3D surface construction algorithm.1987.ACM PressNew York:


- 23\. Abdi H.: Bonferroni and Sidak corrections for multiple comparisons.Salkind N.J.Encyclopedia of measurement and statistics.2007.SageThousand Oaks, Calif:


- 24\. Fradkin D., Muchnik I.: Support vector machines for classification.Abello J.Carmode G.Discrete methods in epidemiology.2006.pp. 13-20.