---
title: Shape-based Assessment of Vertebral Fracture Risk in Postmenopausal Women Using Discriminative Shape Alignment
author: [CL_AT_AlessroCrimiPhD,CL_AT_MarcoLoogPhD,CL_AT_MarleendeBruijnePhD,CL_AT_MadsNielsenPhD,CL_AT_MartinLillholmPhD]
date: 2012-04-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 4]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Risk assessment of future osteoporotic vertebral fractures is currently based mainly on risk factors, such as bone mineral density, age, prior fragility fractures, and smoking. It can be argued that an osteoporotic vertebral fracture is not exclusively an abrupt event but the result of a decaying process. To evaluate fracture risk, a shape-based classifier, identifying possible small prefracture deformities, may be constructed.

## Materials and Methods

During a longitudinal case-control study, a large population of postmenopausal women, fracture free at baseline, were followed. The 22 women who sustained at least one lumbar fracture on follow-up represented the case group. The control group comprised 91 women who maintained skeletal integrity and matched the case group according to the standard osteoporosis risk factors. On radiographs, a radiologist and two technicians independently performed manual annotations of the vertebrae, and fracture prediction using shape features extracted from the baseline annotations was performed. This was implemented using posterior probabilities from a standard linear classifier.

## Results

The classifier tested on the study population quantified vertebral fracture risk, giving statistically significant results for the radiologist annotations (area under the curve, 0.71 ± 0.013; odds ratio, 4.9; 95% confidence interval, 2.94–8.05).

## Conclusions

The shape-based classifier provided meaningful information for the prediction of vertebral fractures. The approach was tested on case and control groups matched for osteoporosis risk factors. Therefore, the method can be considered an additional biomarker, which combined with traditional risk factors can improve population selection (eg, in clinical trials), identifying patients with high fracture risk.

Osteoporosis is a disease characterized by decreases in the density and quality of bone, potentially leading to fractures. Vertebral fractures are the most common type of osteoporotic fractures , and they may occur in the absence of trauma or after minimal trauma. In this case, they are also called fragility fractures. Moreover, the presence of vertebral fractures increases the risk for hip fractures and additional vertebral fractures . A growing percentage of elderly people develop osteoporosis and experience osteoporotic fractures, and consequently, the related burden sustained by the medical system is heavy and increasing rapidly . The total cost in 2000 in Europe has been estimated to €31.7 billion, and it is foreseen to grow to €76 billion by 2050 , while the estimated expense in the United States in 2005 was $19 billion . Therefore, the early assessment of fracture risk is crucial for reducing the number of fractures through appropriate treatments, improving the quality of life of patients, and reducing costs to the health system.

Several clinical factors can provide information on fracture risk. These include bone mineral density (BMD), age, prior fragility fractures, smoking, the use of corticosteroids, excessive consumption of alcohol, and rheumatoid arthritis . The World Health Organization has formalized the analysis of such risk factors in the FRAX tool , which gives a probability of hip fracture over a 10-year period and a probability of major osteoporotic fracture (located in the spine, forearm, hip, or shoulder) over a 10-year period as well. The FRAX tool is available as a Web-based service and in a paper version with guided charts .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633211X00156/S1076633211006192/gr1.jpg?Signature=SCz5KXZ7zR5lP%7EVEZuCPS3xPBXtsjYDZpek7DdoBUImSufvGf3AoveFjRIE9twunuwEeCeTWznDPYB6Th7U7QNX4Lrlu2Vqg%7E8Tx1qyKlAbdDp5MhBRMI3nDgDlRLur1gZXamLd4fm0uu1f5OI82c5wP6u8eD22YOcSdsVNJHtg_&Expires=1669568802&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


On the left **(a)** , overlay of the lumbar region in an x-ray image (case baseline) and its six-point annotation, given by the _stars_ . On the right **(b)** , the spine shape that can be obtained from the concatenation of the two-dimensional landmarks. The annotations were performed considering coherently the lowest endplate of the vertebrae. The contrast in the reproduction above is most likely too low to clearly visualize all the lower boundaries. For the experiments reported in this study, a spine shape was used as the collection of these landmarks without any interpolation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633211X00156/S1076633211006192/gr2.jpg?Signature=Ob3c5jnOxaAC2tkQteeMjq-ilhQ2Z9L1yhOgnxkem8aMjQDNuaDBLqy8KxzRFPHPW1ylWuRPkzKOVoEAZNRrB7hQ1gOu7xITfJSsNF8nRky1LOFrUMjxidh-JQ2Gi3bzYElwy7HkPBwipv0ZSPnUbE9f3wnMTjcSCJdYknYDq40_&Expires=1669568802&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 2


**(a)** Example of baseline vertebra that had fractured by follow-up and **(b)** example of baseline vertebra that had not fractured by follow-up. **(c,d)** Follow-up radiographs of the same vertebrae depicted, respectively, in **(a)** and **(b)** .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

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

## Shape alignment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

dGPA(xi,xj)=∥Wixi−xj∥2,
d

GPA

(

x

i

,

x

j

)

=

‖

W

i

x

i

−

x

j

‖

2

,


where **_W_****_i_** is a similarity transformation matrix, which can be found either by using a closed-form solution or in an iterative fashion , and _x  i_ and _x  j_ are specific shapes.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Point distribution model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Σ=VΛVT,
Σ

=

V

Λ

V

T

,


where **_V_** = \[ **_v_** 1 \|…\| **_v_**_q_ \] is the column matrix of eigenvectors, and **Λ** = diag\[(λ  1 ,…, λ _q_ )\] is the diagonal matrix of corresponding eigenvalues . These eigenvectors and eigenvalues can be used to represent the shapes into the new coordinate system as


Y=Λ−1−−−√VTX.
Y

=

Λ

−

1

V

T

X

.


This equation represents the linear transformation principal components analysis is performing on the data **_X_** to yield the transformed **_Y_** .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

x˜=Vdiag\[(λ1−−√,…λs−−√,0,…,0)\]y+μ,
x

˜

=

V

diag

\[

(

λ

1

,

…

λ

s

,

0

,

…

,

0

)

\]

y

+

μ

,


where x˜
x

˜
is the approximation of **_x_** using this model, **_y_** is the column vector in **_Y_** corresponding to the column vector in **_X_** , and diag\[(λ1−−√,…,λs−−√,0,…,0)\]
diag

\[

(

λ

1

,

…

,

λ

s

,

0

,

…

,

0

)

\]
is the diagonal matrix containing a subset of eigenvalues. The optimal number of used components, _s_ , represents a pivotal parameter that needs to be estimated. We describe in the section “Experiments” how this selection was performed in our experiments.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Linear discriminant classifier

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Pcase(x˜\|μcase,Σ).
P

case

(

x

˜

\|

μ

case

,

Σ

)

.


By normalizing the score as P¯¯¯case=Pcase/(Pcase+Pcontrol)
P

¯

case

=

P

case

/

(

P

case

+

P

control

)
, the probability of fracture risk is in the interval between 0 and 1, where values close to 1 represent high risk for vertebra fracture and those close to 0 represent low risk.  Figure 3 depicts, from left to right, some spine shapes ordered from low to high fracture risk as defined by the described probability. The picture illustrates how difficult it is to see the slight differences in the vertebra shapes and spine curvature without accurate measurements.

![Figure 3, Examples of baseline spine shape, ordered from left to right accordingly to their probability of belonging to the case group on the basis of our fracture risk score. For the experiments reported in this study, the spine shapes were used as the collection of the landmarks without any interpolation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ShapebasedAssessmentofVertebralFractureRiskinPostmenopausalWomenUsingDiscriminativeShapeAlignment/0_1s20S1076633211006192.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discriminative shape alignment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

∑Ni=1(aTxi−ki)2,
∑

i

=

1

N

(

a

T

x

i

−

k

i

)

2

,


where **_a_****_T_** is the discriminative linear regression vector.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

z′i=zizHim.
z

i

′

=

z

i

z

i

H

m

.


Here, zHi
z

i

H
represents the Hermitian of the shape vector. To use this alignment in conjunction with the minimization of equation  6 , the complex vectors must be converted to real values, yielding the expression:


∑Ni=1(aTZiμref−ki)2,
∑

i

=

1

N

(

a

T

Z

i

μ

ref

−

k

i

)

2

,


where Zi=(Re(zizHi)Im(zizHi)−Im(zizHi)Re(zizHi))
Z

i

=

(

Re

(

z

i

z

i

H

)

−

Im

(

z

i

z

i

H

)

Im

(

z

i

z

i

H

)

Re

(

z

i

z

i

H

)

)
. The algorithm is initiated with the mean shape as the **μ  ref** and iteratively updates the reference shape in conjunction with the projection vector **_a_****_T_** . Equation  8 cannot be solved in closed form, because it represents an intertwined linear regression problem .


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


Here, **_F_** is the multidimensional matrix containing all the **_Z  i_** matrices of all the shapes multiplied by **μ  ref** , **_K_** is the vector containing all the labels _k  i_ , and _r_ is a regularization parameter that controlled the degree of regularization.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Experiments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Pseudocode for BNLO algorithm using the DSA version

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


  - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


    - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


      - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

      - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


        - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


          - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

          - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

          - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

        - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

      - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Biologic Data Used to Match the Case and Control Groups


Variable Cases ( _n_ = 22) Controls ( _n_ = 91)_P_ ∗  Age (y) 64.7 (66.9 ± 5.4) 65.4 (66.6 ± 5.9) .98 Height (cm) 162 (163 ± 4.6) 161 (161 ± 6.0) .21 Weight (kg) 64.5 (68.3 ± 11.7) 65.4 (65.4 ± 8.4) .53 Body mass index (kg/m  2  ) 24.8 (25.5 ± 4.0) 24.6 (25.0 ± 3.2) .72 Spine bone mineral density (g/cm  2  ) 0.79 (0.81 ± 0.14) 0.84 (0.86 ± 0.14) .20

Data are expressed as median (mean ± standard deviation).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Receiver-operating characteristic curves obtained using the balanced nested leave-out algorithm and (a) the generalized Procrustes analysis alignment, (b) the discriminative shape alignment. The curves are constructed using all the scores without averaging the scores with respect to the same test shape. The same random samples were used for both versions of the algorithm.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ShapebasedAssessmentofVertebralFractureRiskinPostmenopausalWomenUsingDiscriminativeShapeAlignment/1_1s20S1076633211006192.jpg)

Table 2


AUCs, _P_ Values, and ORs Obtained Using the GPA Alignment


Data Set AUC_P_ OR (95% CI) P.P. 0.72 ± 0.009 .017 5.85 (3.52–9.71) J.P. 0.54 ± 0.089 .352 1.04 (0.62–1.66) A.O. 0.53 ± 0.061 .384 1.03 (0.60–1.45)

AUC, area under the receiver-operating characteristic curve; CI, confidence interval; GPA, generalized Procrustes analysis; OR, odds ratio.


Reported results are mean values with respect to the same test shape for 10 iterations using 1000 samples of the balanced nested leave-out cross-validation protocol. The reported _P_ values were obtained comparing the scores to chance using the DeLong test.


Table 3


AUCs, _P_ Values, and ORs Obtained Using the DSA


Data Set AUC_P_ OR (95% CI) P.P. 0.71 ± 0.013 .019 4.87 (2.94–8.05) J.P. 0.62 ± 0.025 .043 2.04 (1.21–3.36) A.O. 0.60 ± 0.046 .047 1.92 (1.06–2.87)

AUC, area under the receiver-operating characteristic curve; CI, confidence interval; DSA, discriminative shape alignment; OR, odds ratio.


Reported results are mean values with respect to the same test shape for 10 iterations using 1000 samples of the balanced nested leave-out cross-validation protocol. The reported _P_ values were obtained comparing the scores to chance using the DeLong test.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Szulc P., Delmas P.: Vertebral fracture initiative resource document.2005.International Osteoporosis Foundation ReportNyon, Switzerland


- 2\. Black D., Arden N., Palermo L.: Prevalent vertebral deformities predict hip fractures and new vertebral deformities but not wrist fractures. J Bone Miner Res 1999; 14: pp. 821-828.


- 3\. Melton L.J., Atkinson E.J., Cooper C.: Vertebral fractures predict subsequent fractures. Osteoporos Int 1999; 10: pp. 214-221.


- 4\. Kanis J., Borgstrom F., Laet C.D., et. al.: Assessment of fracture risk. Osteoporos Int 2005; 16: pp. 581-589.


- 5\. Burge R., Dawson-Hughes B., Solomon D., et. al.: Incidence and economic burden of osteoporosis-related fractures in the united states. J Bone Miner Res 2007; 22: pp. 465-475.


- 6\. Laet C.D., Oden A., Johnell O., et. al.: The impact of the use of multiple risk factors on case finding strategies: a mathematical framework. Osteoporos Int 2005; 16: pp. 313-318.


- 7\.  World Health Organization Collaborating Centre for Metabolic Bone Diseases, University of Sheffield. FRAX®: WHO Fracture Risk Assessment Tool. Available at:  http://www.shef.ac.uk/frax  . Accessed January 13, 2012.


- 8\. Genant H.K., Wu C., van Kuijk C., et. al.: Vertebral fracture assessment using a semiquantitative technique. J Bone Miner Res 1993; 8: pp. 1137-1148.


- 9\. Eastell R., Cedel S.L., Wahner H.W., et. al.: Classification of vertebral fractures. J Bone Miner Res 1991; 6: pp. 207-215.


- 10\. McCloskey E.V., Spector T.D., Eyres K.S., et. al.: The assessment of vertebral deformity: a method for use in population studies and clinical trials. Osteoporos Int 1994; 4: pp. 138-147.


- 11\. Hurxthal L.M.: Measurement of vertebral heights. AJR Am J Roentgenol 1968; 103: pp. 635-644.


- 12\. Genant H.K., Jergas M., Palermo L., et. al.: Comparison of semi-quantitative visual and quantitative morphometric assessment of prevalent and incident vertebral fractures. J Bone Miner Res 1996; 11: pp. 984-996.


- 13\. Jiang G., Eastell R., Barrington N., et. al.: Comparison of methods for the visual identification of prevalent vertebral fracture in osteoporosis. Osteoporos Int 2004; 15: pp. 887-896.


- 14\.  Aouache M, Hussain A, Samad S, et al. Active shape modeling of medical images for vertebral fracture computer assisted assessment system. Available at:  http://ieeexplore.ieee.org/xpl/freeabs\_all.jsp?arnumber=4451397  . Accessed January 13, 2012.


- 15\. de Bruijne M., Lund M.T., Tanko L.B., et. al.: Quantitative vertebral morphometry using neighbor-conditional shape models. Med Image Anal 2007; 11: pp. 503-512.


- 16\. de Bruijne M., Pettersen P., Tanko L., et. al.: Vertebral fracture classification. Proc SPIE Med Imaging 2007; 6512: pp. 651219.


- 17\. Roberts M., Cootes T., Pacheco E., et. al.: Quantitative vertebral fracture detection on DXA images using shape and appearance models. Acad Radiol 2007; 14: pp. 1166-1178.


- 18\. Roberts M., Pacheco E., Mohamkumar R., et. al.: Detection of vertebral fractures in DXA VFA images using statistical models of appearance and a semi-automatic segmentation. Osteoporos Int 2010; 21: pp. 2037-2046.


- 19\. Diacinti D., Pisani D., Barone-Adesi F., et. al.: A new predictive index for vertebral fractures: The sum of the anterior vertebral body heights. Bone 2010; 46: pp. 768-773.


- 20\. Lillholm M., Ghosh A., de Bruijne M., et. al.: Vertebral fracture risk (VFR) score for fracture prediction in postmenopausal women. Osteoporos Int 2011; 22: pp. 2119-2128.


- 21\. Loog M., Bruijne M.: Discriminative shape alignment. Proc 21st Int Conf Inform Proc Med Imaging 2009; 12: pp. 459-466.


- 22\. Pettersen P.C., de Bruijne M., Chen J., et. al.: A computer-based measure of irregularity in vertebral alignment is a BMD-independent predictor of fracture risk in postmenopausal women. Osteoporos Int 2007; 18: pp. 1525-1530.


- 23\. Ruyssen-Witrand A., Gossec L., Kolta S., et. al.: Vertebral dimensions as risk factor of vertebral fracture in osteoporotic patients: a systematic literature review. Osteoporos Int 2007; 18: pp. 1271-1278.


- 24\. Baker-LePain J., Luker K., Lynch J., et. al.: Active shape modeling of the hip in the prediction of incident hip fracture. J Bone Miner Res 2011; 26: pp. 468-474.


- 25\. Gregory J., Stewart A., Undrill P., et. al.: Bone shape, structure and density as determinants of osteoporotic hip fracture: a pilot study investigating the combination of risk factors. Invest Radiol 2005; 40: pp. 591-597.


- 26\. Bouxsein M., Karasik D.: Bone geometry and skeletal fragility. Curr Osteoporos Rep 2006; 4: pp. 49-56.


- 27\. Bagger Y.Z., Tanko L.B., Alexandersen P., et. al.: The long-term predictive value of bone mineral density measurements for fracture risk is independent of the site of measurement and the age at diagnosis: results from the prospective epidemiological risk factors study. Osteoporos Int 2006; 17: pp. 471-477.


- 28\. Bookstein F.L.: Shape and the information in medical images: a decade of morphometric synthesis. Comput Vis Image Understand 1997; 66: pp. 97-118.


- 29\. Goodall C.: Procrustes methods in the statistical analysis of shape. J R Stat Soc 1991; 53: pp. 285-339.


- 30\. Dryden I., Mardia K.: Statistical shape analysis.1998.John WileyNew York


- 31\. Bookstein F.L.: Landmark methods for forms without landmarks: localizing group differences in outline shape. Med Image Anal 1997; 1: pp. 225-243.


- 32\. Jolliffe I.T.: Principal component analysis.2002.SpringerNew York


- 33\. Cootes T.F., Taylor C.J., Cooper D.H., et. al.: Active shape models-their training and application. J Comput Vis Image Understand 1995; 61: pp. 38-59.


- 34\. Bellman R.E.: Dynamic programming.2003.Courier DoverMineola, NY


- 35\. Duda R.O., Hart P.E.: Pattern recognition and scene analysis.1973.John WileyNew York


- 36\. Hastie T., Tibshirani R., Friedman J.: The elements of statistical learning.2003.SpringerNew York


- 37\. Tikhonov A.N., Arsenin A.N.: Solution of ill-posed problems.1977.Winston & SonsWashington, DC


- 38\. Hastie T., Buja A., Tibshirani R.: Penalized discriminant analysis. Ann Stat 1995; 1: pp. 73-102.


- 39\. Hoerl A., Kennard R.W.: Ridge regression: biased estimation for nonorthogonal problems. Technometrics 2000; 42: pp. 80-86.


- 40\. DeLong E., DeLong D., Clarke-Pearson D.: Comparing the areas under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-845.


- 41\. Zebaze R.M.D., Maalouf G., Seeman N.M.E.: Loss of regularity in the curvature of the thoracolumbar spine: a measure of structural failure. J Bone Miner Res 2004; 19: pp. 1099-1104.


- 42\. McCance L., Huether S.E.: Pathophysiology: the biologic basis for disease in adults and children.2009.MosbySt. Louis, MO