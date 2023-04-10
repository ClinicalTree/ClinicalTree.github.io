---
title: Establishing a Normative Atlas of the Human Lung
author: [CL_AT_BaojunLiPhD,CL_AT_GaryEChristensenPhD,CL_AT_EricAHoffmanPhD,CL_AT_GeoffreyMcLennanMD,CL_AT_JosephMReinhardtPhD]
date: 2012-11-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 11]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

To establish the range of normal for quantitative computed tomography (CT)-based measures of lung structure and function, we seek to develop methods for matching pulmonary structures across individuals and establishing a normative human lung atlas.

## Materials and Methods

In our previous work, we have presented a three-dimensional (3D) image registration method suitable for pulmonary atlas construction based on CT datasets. The method has been applied to a population of normative lungs in multiple experiments and, in each instance, has resulted in significant reductions in registration errors. This study is a continuation to our previous work by presenting a method for synthesizing a computerized human lung atlas from previously registered and matched 3D pulmonary CT datasets from a population of normative subjects. Our method consists of defining the origin of the atlas coordinate system; defining the nomenclature and labels for anatomical structures within the atlas system; computing the average transformation based on the displacement fields to register individual subject to the common template subject; constructing the atlas by deforming the template with the average transformation; and calculating shape variations within the population.

## Results

The feasibility of pulmonary atlas construction was evaluated using CT datasets from 20 normal volunteers. Substantial reductions in shape variability were demonstrated. In addition, the constructed atlas depends only slightly on a specific subject being selected as the template. These results indicate the framework is a robust and valid method for pulmonary atlas construction based on CT scans. The atlas consists of a grayscale CT dataset of the template, a labeled mask dataset of the template (ie, lungs, lobes, and lobar fissures are labeled with different gray levels), a data set representing the population's average shape, datasets representing the population's shape variations (ie, the magnitude of standard deviation), a data structure to contain the labels and coordinates of major airway branchpoints, and the labels of the mask dataset, and a reference coordinate system for each lung.

## Conclusion

A computerized human lung atlas representing by the average shape of a population of twenty normal subjects was constructed and visualized. The atlas provides a basis for establishing regional ranges of normative values for structural and functional measures of the human lung. In the future, we plan to use the computerized human lung atlas to help detect and quantify early signs of lung pathology.

To reduce lung cancer–associated mortality, many computed tomography (CT)-based new therapeutic interventions for lung disease have emerged. As one takes advantage of new methods for CT-based assessment of regional ventilation and perfusion , it becomes necessary to detect age- and gender-based normative values for CT-based measures of lung structure and function. Therefore, there is a need to establish methods by which lung structure can be compared from person to person (inter-subject) . A computerized atlas (or standard structural model) that defines a normal range of pulmonary variation can greatly facilitate the understanding of subject-invariant structure-function relationships. It can also provide standard, quantitative, and sensitive measures of chronic structural change from aging or disease.

In our previous work , we presented an semiautomatic method for inter-subject registration and warping of volumetric CT datasets. Our method consists of the following steps. First, in all subjects, the lungs, lobes, and airways are segmented based on image gray level information and three-dimensional (3D) connectivity of tissues. Next, the airways are further processed by skeletonization technique to extract a set of reproducible airway branchpoints to be used as anatomical landmarks in the registration process. The airway branchpoints are labelled and matched across subjects by an automatic airway tree matching and labeling algorithm . Third, image registration in general requires all images to be in the same coordinate system. This is achieved by a combination of rigid alignment, isotropic scaling, padding, and downsampling. This step results in the segmented lungs, lobes, and matched airway branchpoints, all in the coordinate system of the template image. Finally, a landmark and intensity-based consistent image registration technique is used to register a template image volume with the remaining lung volumes in the population. Results from clinical studies showed that our proposed method was able to reduce the average landmark registration error and average relative volume overlap error from 10.5 mm and 0.70 before registration to 0.4 mm and 0.11, respectively, after registration. The results indicate the method is suitable for pulmonary atlas construction based on CT datasets.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Image Acquisition

## Participants

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

## Selecting a template

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, A topological model of human airway tree developed in this research. Details concerning this model was discussed in our previous work (6 7) . ant., anterior; BronInt., bronchus intermedius; lat., lateral; LB, left segmental bronchus; LMB, left mainstem branchus; med., medial; post., posterior; RB, right segmental bronchus; RLL, right lower lobe bronchus; TriLBB, trifurcation lower lobe bronchus; TriRLL, trifurcation right lower lobe bronchus; TriRUL, trifurcation right upper lobe bronchus.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/0_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CT scan protocol

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Two transverse slices of a three-dimensional pulmonary computed tomography image from subject 9 from Table 1 .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/1_1s20S1076633212003819.jpg)

Table 1


Demographics for the 20 Subjects Used in This Study for Atlas Construction


Subject Number Age (y) Gender Weight (kg) Height (cm) 1 20 M 99.8 174 2 22 M 81 177 3 60 F 72 162 4 25 M 79 182 5 25 M 84 187.9 6 24 F 63.3 170 7 37 F 79.5 167.6 8 21 F 70.4 172.4 9  ∗  22 F 60 165 10 20 F 54 162.5 11 22 F 65.7 184.5 12 25 M 91.8 187.9 13 29 M 80 172.2 14 46 F 61.3 155 15 20 F 69 172 16 21 F 67.7 167 17 24 F 63.6 177.5 18 43 F 53 161.3 19 23 F 70.45 180 20 40 M 109 185

F, female; M, male.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Atlas Coordinate Systems

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Labeling the Template Dataset and Atlas Nomenclature

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


The Suggested Allocation of Labels for the Template Dataset


Label (Gray Level) Nomenclature (Anatomy) Label (Gray Level) Nomenclature (Anatomy) 0 Background 1 Lung 2 Lung left 3 Lung right 4 Lung left upper lobe 5 Lung left lower lobe 6 Lung right upper lobe 7 Lung right middle lobe 8 Lung right lower lobe 9 Lung LB1 + LB2 sub-lobe 10 Lung LB3 sub-lobe 11 Lung LB4 sub-lobe 12 Lung LB5 sub-lobe 13 Lung LB6 sub-lobe 14 Lung LB7 + LB8 sub-lobe 15 Lung LB9 sub-lobe 16 Lung LB10 sub-lobe 17 Lung LBA sub-lobe 18 Lung RB1 sub-lobe 19 Lung RB2 sub-lobe 20 Lung RB3 sub-lobe 21 Lung RB4 sub-lobe 22 Lung RB5 sub-lobe 23 Lung RB6 sub-lobe 24 Lung RB7 sub-lobe 25 Lung RB8 sub-lobe 26 Lung RB9 sub-lobe 27 Lung RB10 sub-lobe 28 Lung RBA sub-lobe 29 Airway trachea 30 Airway LMB 31 Airway RMB 32 Airway LUL 33 Airway LLB6 34 Airway RUL 35 Airway BronInt 36 Airway LB1 + 2 37 Airway LB3 38 Airway LB4 + 5 39 Airway LB6 40 Airway LLB 41 Airway RB1 42 Airway RB2 43 Airway RB3 44 Airway RB4 + 5 45 Airway RB6 46 Airway RLL7 47 Airway LB1 48 Airway LB2 49 Airway LB4 50 Airway LB8 51 Airway LB9 52 Airway LB10 53 Airway RB4 54 Airway RB5 55 Airway RLL 56 Airway RB7 57 Airway RB8 58 Airway RB9 59 Airway RB10 60–80 Reserved 81 Right horizontal fissure 82 Right oblique fissure 83 Left oblique fissure 84–255 Not used

BronInt, bronchus intermedius; LB, left segmental bronchus; LBA, left apical segmental bronchus; LLB, left lower lobe bronchus; LMB, left mainstem bronchus; LUL, left upper lobe bronchus; RB, right segmental bronchus; RLL, right lower lobe bronchus; RMB, right mainstem bronchus; RUL, right upper lobe bronchus.


There are totally 256 (2  8  ) labels available for an 8-bit gray-level image.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


A Sample of a Label LUT That Maps the Old Labels from Individual Segmentation Routines to the Labels in  Table 2

Nomenclature Old Label (Gray Level) → New Label (Gray Level) Background 0 → 0 Lung left 20 → 2 Lung right 30 → 3 Airway LMB 5 → 31 Airway RMB 4 → 32 Airway LUL 8 → 33 Airway LLB6 9 → 34 Airway RUL 7 → 35 Airway BronInt 6 → 36 Airway LB1 + 2 26 → 37 Airway LB1 + 2 49 → 37 Airway LB3 27 → 38 Airway LB4 + 5 15 → 39 Airway LB6 16 → 40 Airway LLB 17 → 41 Airway RB1 12 → 42 Airway RB2 25 → 43 Airway RB3 24 → 44 Airway RB4 + 5 10 → 45 Airway … … → … Airway RLL7 20 → 47 Airway … … → … Airway RB8 68 → 58 Airway RB9 69 → 59 Airway RB10 100 → 60

BronInt, bronchus intermedius; LB, left segmental bronchus; LLB, left lower lobe bronchus; LMB, left mainstem bronchus; LUL, left upper lobe bronchus; RB, right segmental bronchus; RLL, right lower lobe bronchus; RMB, right mainstem bronchus; RUL, right upper lobe bronchus.


Note that the actual look-up table is determined by the labeling conventions of the segmentation algorithms.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Computing the Average Shape

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

g¯=1N∑Ni=1g(i),
g

¯

=

1

N

∑

i

=

1

N

g

(

i

)

,


and is applied to the template _T_ to synthesize the average shape of the population as


T¯¯¯=T(h¯)=T(g¯−1).
T

¯

=

T

(

h

¯

)

=

T

(

g

¯

−

1

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The procedure to build an image-based average shape for a homogeneous population.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/2_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

L¯¯¯=MT(h¯)=MT(g¯−1),
L

¯

=

M

T

(

h

¯

)

=

M

T

(

g

¯

−

1

)

,


where _L_ represents the upper and lower lobar atlas and MT
M

T
is the lobar mask subimage of the template. By this means, the upper and lower lobar atlas for each lung is calculated at the same time. Alternatively, the upper and lower lobar atlases can be constructed separated. A detailed discussion on this matter can be found in the Discussion section.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Computing the Population Shape Variations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

w(i,j)(x)=g(i,j)(x)−x
w

(

i

,

j

)

(

x

)

=

g

(

i

,

j

)

(

x

)

−

x


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

DAD(i,j)=1vol(M)∫M∣∣w(i,j)(x)∣∣dx
D

A

D

(

i

,

j

)

=

1

vol

(

ℳ

)

∫

ℳ

\|

w

(

i

,

j

)

(

x

)

\|

d

x


where vol(M)=∫M1⋅dx
v

o

l

(

ℳ

)

=

∫

ℳ

1

·

d

x
is the volume of the region of interest. The average displacement distance between image T(i)
T

(

i

)
and the population of images T(j)
T

(

j

)
for j=1,…,N
j

=

1

,

…

,

N
within the region of interest is defined as the average of the pairwise average displacement distances. The average displacement distance between a dataset and the population is given by


DADPOP(i)=1N∑Nj=1DAD(i,j).
D

A

D

P

O

P

(

i

)

=

1

N

∑

j

=

1

N

D

A

D

(

i

,

j

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

V(i)(x)=1N−1∑Nj=1∣∣g(i,j)(x)−g(i,i¯)(x)∣∣2dx.
V

(

i

)

(

x

)

=

1

N

−

1

∑

j

=

1

N

\|

g

(

i

,

j

)

(

x

)

−

g

(

i

,

i

¯

)

(

x

)

\|

2

d

x

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

DDV(i)=1vol(M)∫MV(i)(x)dx
D

D

V

(

i

)

=

1

vol

(

ℳ

)

∫

ℳ

V

(

i

)

(

x

)

d

x


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, The three orthogonal views of the gray-level computed tomography dataset of the template, the most representative subject of the population sampled.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/3_1s20S1076633212003819.jpg)

![Figure 5, The volume renderings of the labeled mask. User may click the structure of interest in the computed tomography dataset and get the corresponding anatomic label from the labeled mask, or vice versa. LB, left segmental bronchus; LLL, left lower lobe; LMSB, left mainstem bronchus; LUL, left upper lobe; RB, right segmental bronchus; RML, right middle lobe; RMSB, right mainstem bronchus; RUL, right upper lobe; RLL, right lower lobe.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/4_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, The surface renderings of the calculated mean shape of the population. The different anatomies have been color-coded. It can be seen in the figure that this image-based atlas carries structural information such as the average location of the oblique lobar fissures. LLL, left lower lobe; LUL, left upper lobe; RLL, right lower lobe; RML, right middle lobe; RUL, right upper lobe.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/5_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, The standard deviation displacements (with respect to end right mainstem bronchus or end left mainstem bronchus) color-coded on the right lung ( top row ) and the left lung ( bottom row ). The standard deviation displacement is the indication of the shape variations in the population. The color bars indicate the scale of variations (unit: mm). LLL, left lower lobe; LUL, left upper lobe; RLL, right lower lobe; RML, right middle lobe; RUL, right upper lobe.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/6_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Computed lung atlases (averages + shape variations) from 20 subjects, using 3 different subjects as the template. ( Top row ) Subject 9 as the template. ( Middle row ) Subject 19 as the template. ( Bottom row ) Subject 11 as the template. For each atlas, the left column represents the right lung and the right column represents the left lung. Examination of the average shapes and shape variations suggests that the proposed atlas construction method depends only slightly on a specific subject being selected as the template.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/7_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, The shape variability among a set of ( n = 6) subjects involved in this study is demonstrated by overlapping contours from axial computed tomography (CT) images. The top row shows the shape variation among the subjects; the bottom row corresponds to the transformed CT datasets after transforming individual subject with respect to a common template subject (subject 9). Only 6 subjects were displayed here to avoid overcrowding the figure. The columns represent three axial image slices randomly chosen near the apex ( a and d ), the body ( b and e ), and the diaphragm ( c and f ). Significant reduction in registration errors can be seen with reduced variability.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/8_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Construction of Lobar Atlas

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Lobe slippage

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Performance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Slice comparison of two typical slices from the right upper lobe atlases. The atlases were generated by applying two different approaches to six pulmonary computed tomography datasets. (a,b) The current approach. (c,d) The alternative approach. The volume difference between the two atlases is only 2.6%.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/9_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Computational expenses

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Lobe overlapping

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 11, Overlapping regions around the lobar fissure can be seen in this synthesized dataset by combining the right upper lobe atlas and the right lower lobe atlas. These two atlases were constructed separately from six pulmonary computed tomography datasets. (a) Coronal view. (b) Transverse view.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EstablishingaNormativeAtlasoftheHumanLung/10_1s20S1076633212003819.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The Impact of the Origin on the Shape Variation Measure

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Tajik J.K., Chon D., Won C., et. al.: Hoffman. Subsecond multisection CT of regional pulmonary ventilation. Acad Radiol 2002; 9: pp. 130-146.


- 2\. Tajik J.K., Tran B.Q., Hoffman E.A.: CT-based assessment of regional pulmonary blood flow parameters: an update. Proc SPIE Conf Med Imaging 1999; 3660: pp. 181-187.


- 3\. Kreck T.C., Krueger M.A., Altemeier W.A., et. al.: Determination of regional ventilation and perfusion in the lung using xenon and computed tomography. J Appl Physiol 2001; 91: pp. 1741-1749.


- 4\. Marcucci C., Nyhan D., Simon B.A.: Distribution of pulmonary ventilation using Xe-enhanced computed tomography in prone and supine dogs. J Appl Physiol 2001; 90: pp. 421-430.


- 5\. Hoffman E.A.: Advances in physiologic lung assessment via electron beam computed tomography. Med Technol Symp 1998; pp. 96-108.


- 6\. Li B., Christensen G.E., Dill J., et. al.: 3-d inter-subject warping and registration of pulmonary CT images for a human lung model. Proc SPIE Conf Med Imaging 2002; 4683: pp. 324-335.


- 7\. Li B., Christensen G.E., Hoffman E.A., et. al.: Establishing a normative atlas of the human lung: Intersubject warping and registration of volumetric CT images. Acad Radiol 2003; 10: pp. 255-265.


- 8\. Li B., Christensen G.E., Hoffman E.A., et. al.: Pulmonary CT image registration and warping for tracking tissue deformation during respiratory cycle through 3D consistent image registration. Med Phys 2008; 35: pp. 5575-5583.


- 9\. Tschirren J., Palagyi K., Reinhardt J.M., et. al.: Segmentation, skeletonization, and branchpoint matching—a fully automated quantitative evaluation of human intrathoracic airway trees. Lecture Notes Comp Sci 2002; 2489: pp. 12-19.


- 10\. Johnson H.J., Christensen G.E.: Consistent landmark and intensity-based image registration. IEEE Trans Med Imaging 2002; 21: pp. 450-461.


- 11\.  Guo J, Reinhardt JM, Won C-H, et al. Human lung atlas: establishment of a comprehensive software environment for the assessment of pulmonary anatomy and physiology via multi-slice sub-second spiral CT. Proc Radiol Soc North Am Annual Meeting: Chicago, IL; 2001.


- 12\.  Guo J, Reinhardt JM, Kitaoka H, et al. Integrated system for CT-based assessment of parenchymal lung disease. 2002 International Symposium on Biomedical Imaging, Washington, DC, July 2002:871–874.


- 13\.  Thompson B, Lee W, Wilson J. Electronic Textbook of Lung Anatomy. Available at:  //medpro.smiletrain.org/library/images/vh096.htm  . 1993.


- 14\. Mazziotta J., Toga A., Evans A., et. al.: A four-dimensional probabilistic atlas of the human brain. J Am Med Info Assoc 2001; 8: pp. 401-430.


- 15\.  Thompson PM, Mega M, Woods R, et al. A probabilistic atlas of the human brain in Alzheimer's disease: emerging pattern of variability, asymmetry and degeneration. Proc 5th International Conference on Functional Mapping of the Human Brain, Dusseldorf, Germany; June 1999.


- 16\. Thompson P., Toga A.: A framework for computational anatomy. Comp Visualization Sci 2002; 5: pp. 13-34.


- 17\.  M. Miller M, A. Banerjee A, G. E. Christensen GE, et al. Statistical methods in computational anatomy. Stat Methods Med Res 1997; 6:267–299.


- 18\. Christensen G.E., Johnson H.J., Haller J.W., et. al.: Synthesizing average 3D anatomical shapes using deformable templates. Medical Imaging 1999. Proc SPIE 1999; 3661: pp. 574-582.


- 19\. Johnson H.J., Christensen G.E., Marsh J.L., et. al.: Validation of probabilistic anatomical shape atlases. Medical Imaging 2000: Image Processing. Proc SPIE 2000; 3979: pp. 687-697.


- 20\. Zhang L., Reinhardt J.M.: Detection of lung lobar fissures using fuzzy logic. Proc SPIE Conf Med Imaging 1999; 3660: pp. 188-199.


- 21\.  Zhang L, Reinhardt JM, McLennan G, et al. Lung lobe segmentation for quantitative assessment of pulmonary anatomy and physiology in volumetric X-ray CT images. Proc Radiol Soc North Am Annual Meeting: Chicago, IL; 2002.


- 22\.  Christensen GE, Johnson H, Blake C, et al. GEC Lab Software Reference Manual (v1.7). Department Elect. Eng., The University of Iowa, Iowa City, IA. October 2002.