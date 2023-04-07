---
title: Automatic Left Ventricle Segmentation in Cardiac MRI Using Topological Stable-State Thresholding and Region Restricted Dynamic Programming
author: [CL_AT_HongLiuPhD,CL_AT_HuaifeiHuPhD,CL_AT_XiangyangXuPhD,CL_AT_EnminSongPhD]
date: 2012-06-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 6]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Segmentation of the left ventricle (LV) is very important in the assessment of cardiac functional parameters. The aim of this study is to develop a novel and robust algorithm which can improve the accuracy of automatic LV segmentation on short-axis cardiac magnetic resonance images (MRI).

## Materials and Methods

The database used in this study consists of 45 cases obtained from the Sunnybrook Health Sciences Centre. The 45 cases contain 12 ischemic heart failures, 12 non-ischemic heart failures, 12 LV hypertrophies, and 9 normal cases. Three key techniques are developed in this segmentation algorithm: 1) topological stable-state thresholding method is proposed to refine the endocardial contour, 2) an edge map with non-maxima gradient suppression approach, and 3) a region-restricted technique that is proposed to improve the dynamic programming to derive the epicardial boundary.

## Results

The validation experiments were performed on a pool of data sets of 45 cases. For both endo- and epicardial contours of our results, percentage of good contours is about 91%, the average perpendicular distance is about 2 mm, and the overlapping dice metric is about 0.91. The regression and determination coefficient for the experts and our proposed method on the ejection fraction is 1.05 and 0.9048, respectively; they are 0.98 and 0.8221 for LV mass.

## Conclusions

An automatic method using topological stable-state thresholding and region restricted dynamic programming has been proposed to segment left ventricle in short-axis cardiac MRI. Evaluation results indicate that the proposed segmentation method can improve the accuracy and robust of left ventricle segmentation. The proposed segmentation approach shows the better performance and has great potential in improving the accuracy of computer-aided diagnosis systems in cardiovascular diseases.

Cardiovascular diseases are the leading cause of death in Western countries . The quantification of myocardial mass and systolic function is routinely performed in the clinical setting to diagnose and treat a variety of cardiac pathologies. Cine magnetic resonance (MR) images of the cardiac left ventricle (LV), using the short-axis view, is commonly employed for the assessment of stroke volume, ejection fraction, and myocardial mass as well as regional function parameters such as wall motion and wall thickening. To perform these quantification tasks, the LV needs to be segmented well.

Manual segmentation of LV is a time-consuming and tedious task, with poor reproducibility, and inter- and intra-observer variability resulting from inaccuracies in tracing complex myocardial structures such as papillary and trabecular muscles. It is therefore desirable to use algorithms that are accurate and require as little user interaction as possible. In recent years, quite a number of methods have been proposed for automated LV segmentation. These methods can be classified into two categories: 1) deformable models and 2) image-based techniques. A complete review of recent literature describing cardiac segmentation techniques is given in previous work .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Materials

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The Framework of the Segmentation Algorithm

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Workflow of the proposed segmentation method.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticLeftVentricleSegmentationinCardiacMRIUsingTopologicalStableStateThresholdingandRegionRestrictedDynamicProgramming/0_1s20S1076633212001006.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ROI and LV Location

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Extract the Endocardial Contour

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Analysis change of the blood area with a different threshold: (a) area of blood pool, (b) change rate of the blood pool area.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticLeftVentricleSegmentationinCardiacMRIUsingTopologicalStableStateThresholdingandRegionRestrictedDynamicProgramming/1_1s20S1076633212001006.jpg)

![Figure 3, Blood pool detection with different threshold: (a) gray image, (b) binary image with Otsu threshold value, (c) binary image with Th1, (d) binary image with Th1-5. The top connected white region in the binary image is the detected blood pool.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticLeftVentricleSegmentationinCardiacMRIUsingTopologicalStableStateThresholdingandRegionRestrictedDynamicProgramming/2_1s20S1076633212001006.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Calculate the Epicardial Contour

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Construct a Region-restricted Mask

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Definition of Cost Function

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

g(i,j)={01Localmaximalpoint(i,j)andmask(i,j)=0other
g

(

i

,

j

)

=

{

0

L

o

c

a

l

max

i

m

a

l

p

o

int

(

i

,

j

)

a

n

d

m

a

s

k

(

i

,

j

)

=

0

1

o

t

h

e

r


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

C(i,1)={∞g(i,1)mask(i,1)=1other
C

(

i

,

1

)

=

{

∞

m

a

s

k

(

i

,

1

)

=

1

g

(

i

,

1

)

o

t

h

e

r


C⎛⎝⎜i,j⎞⎠⎟=⎧⎩⎨⎪⎪∞,min−5≤k≤5Ck(i,j),mask(i,j)=1otherwiseCk(i,j)=C(i+k,j−1)+exp(\|k\|∗0.5)+λ∗g(i,j)for2≤j≤N;1≤i+k≤M
C

(

i

,

j

)

=

{

∞

,

m

a

s

k

(

i

,

j

)

=

1

min

−

5

≤

k

≤

5

C

k

(

i

,

j

)

,

o

t

h

e

r

w

i

s

e

C

k

(

i

,

j

)

=

C

(

i

+

k

,

j

−

1

)

+

exp

(

\|

k

\|

∗

0.5

)

+

λ

∗

g

(

i

,

j

)

f

o

r

2

≤

j

≤

N

;

1

≤

i

+

k

≤

M


where λ
λ
is the weighting factor of the image feature _g_ ( _i_ , _j_ ). At the beginning of the column-by-column procession, we start from the second column and go to the last column N for cost map construction; the cost in current column is computed from the cost in its previous column. In this construction, small values indicate higher likely edge locations. Therefore, the row position r in the last column N with the minimum value in the cost map _C_ (\*, _N_ ) is searched, which specifies the point ( _r_ , _N_ ) of the epicardial contour in last column. Then with a column-by-column backward search from column N to 1 start from the point ( _r_ , _N_ ), the complete coordinates of the epicardial contour can be obtained, which is the optimal solution corresponding to the global minimum of the optimizing function.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Smooth Endo- and Epicardial Contours

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ρ∗=IFFT(H∗FFT(ρ))
ρ

∗

=

I

F

F

T

(

H

∗

F

F

T

(

ρ

)

)


where ρ
ρ
are the corresponding distances of the edge points to its center, ρ={ρ1,ρ2,…,ρn}
ρ

=

{

ρ

1

,

ρ

2

,

…

,

ρ

n

}
. H is an ideal low pass filter and IFFT is the inverse FFT.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Segmentation Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

LVM=(VEDepi−VEDend)∗1.05
L

V

M

=

(

V

e

p

i

E

D

−

V

e

n

d

E

D

)

∗

1.05


EF=(VEDend−VESend)VEDend∗100%
E

F

=

(

V

e

n

d

E

D

−

V

e

n

d

E

S

)

V

e

n

d

E

D

∗

100

%


Where VEDend
V

e

n

d

E

D
and VEDepi
V

e

p

i

E

D
represents endo- and epicardial volume in the end-diastole (ED) phase respectively; VESend
V

e

n

d

E

S
represents endocardial volume in the end-systole (ES) phase.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Results of 45 Cases

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Results on 45 Cases


Group Studies Good (%) Distance (mm) Overlap EF (%) LVM (g) Endo Epi Endo Epi Endo Epi Auto Expert Auto Expert HF-I 12 Mean 94.24 91.57 2.22 2.07 0.91 0.95 28 25.61 126.11 132.52 SD 5.82 13 0.38 0.51 0.03 0.01 13.95 10.18 39.77 34.09 HF-NI 12 Mean 86.94 88.63 2.43 2.11 0.9 0.94 31.42 28.86 135.7 128.47 SD 7.95 9.39 0.36 0.29 0.02 0.01 14.68 14.53 31.79 25.97 HYP 12 Mean 88.21 89.28 2.58 2.48 0.85 0.92 67.69 60.93 101.74 103.76 SD 10.33 8.31 0.35 0.53 0.02 0.02 7.80 10.09 60.92 57.07 Normal 9 Mean 96.68 94.60 2.16 2.07 0.87 0.93 64.29 58.26 87.15 86.53 SD 4.32 10.92 0.34 0.51 0.03 0.02 6.19 7.73 25.76 27.74 All 45 Mean 91.17 90.78 2.36 2.19 0.88 0.94 46.75 42.42 114.38 114.57 SD 8.52 10.68 0.39 0.49 0.03 0.02 21.61 19.67 45.32 41.79 Overall 45 Mean 90.98 2.28 0.91 SD 9.60 0.44 0.03

Distance, average perpendicular distance; EF, ejection fraction; endo, endocardial contour; epi, epicardial contour; good, percentage of good contours; HF-I, heart failure with ischemic; HF-NI, heart failure without ischemic; HYP, hypertrophy; LVM, left ventricle mass; overlap, overlapping dice metric; SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Regression and Bland-Altman Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Regression curve and Bland-Altman plot for the ejection fraction and left ventricle mass: (a) Linear regression for ejection fraction (EF), (b) Bland-Altman plots of EF, (c) linear regression for left ventricular (LV) mass, (d) Bland-Altman plots of LV mass.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticLeftVentricleSegmentationinCardiacMRIUsingTopologicalStableStateThresholdingandRegionRestrictedDynamicProgramming/3_1s20S1076633212001006.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparisons

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Compare Contour Accuracy between Huang's and Our Results


Result

Contours Good (%) Distance (mm) Overlap Huang's Our Huang's Our Huang's Our Endo Epi Endo Epi Endo Epi Endo Epi Endo Epi Endo Epi All Mean 79.2 83.9 91.17 90.78 2.16 2.22 2.36 2.19 0.89 0.93 0.88 0.94 SD 19 16.8 8.52 10.68 0.46 0.43 0.39 0.49 0.04 0.02 0.03 0.02 Overall 81.5 ± 18.0 90.98 ± 9.60 2.19 ± 0.44 2.28 ± 0.44 0.91 ± 0.03 0.91 ± 0.03

Endo, endocardial contour; epi, epicardial contour; SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Segmentation of an example case (SC-HF-I-05) by our method. The names below the image data are from the data source. The image with the last three odd number of its name is from the end-systole (ES) phase, whereas that with the last three even number of its name comes from the end-diastole (ED) phase. The dashed white curves indicate our contours; whereas the solid white ones are the ground truth. The epicardial contour is not drawn by experts in the ES phase (cropped for better viewing).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticLeftVentricleSegmentationinCardiacMRIUsingTopologicalStableStateThresholdingandRegionRestrictedDynamicProgramming/4_1s20S1076633212001006.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Endocardial contours of a slice image (IM-0001-0100) from case SC-HF-I-05. The dashed white curve is obtained using topological stable-state thresholding technique, whereas the solid gray one is derived without using this thresholding method. The solid white curve is the ground truth.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticLeftVentricleSegmentationinCardiacMRIUsingTopologicalStableStateThresholdingandRegionRestrictedDynamicProgramming/5_1s20S1076633212001006.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Compare Endocardial Contour Accuracy for the Utility of Topological Stable-state Thresholding


Method Good (%) Distance (mm) Overlap A B A B A B All Mean 57.95 91.17 3.29 2.36 0.84 0.88 SD 23.70 8.52 0.68 0.39 0.06 0.03

A, not using topological stable thresholding; B, adopting topological stable thresholding; SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Epicardial contours of two slice image from case SC-HF-I-05 before and after using non-maxima gradient suppression or region restricted technique in dynamic programming: (a) contours of slice image (IM-0001-0160) with and without non-maxima gradient suppression technique, but using the region-restricted method, (b) contours of slice image (IM-0001-0200) with and without region restricted technique, but adopting the non-maxima method. The solid gray curve is obtained with using only one of the two techniques, whereas the dashed white one using the two techniques. The solid white curve is the ground truth.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticLeftVentricleSegmentationinCardiacMRIUsingTopologicalStableStateThresholdingandRegionRestrictedDynamicProgramming/6_1s20S1076633212001006.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Compare Epicardial Contour Accuracy to Show the Advantages of Non-maxima Gradient Suppression and Region-restricted Technique


Method Good (%) Distance (mm) Overlap C D E C D E C D E All Mean 73.42 81.85 90.78 2.61 2.24 2.19 0.93 0.94 0.94 SD 16.41 15.58 10.68 0.5 0.51 0.49 0.02 0.02 0.02

C, not using non-maxima gradient suppression, but adopting region restricted technique; D, adopting non-maxima gradient suppression, but not using region restricted technique; E, using both non-maxima gradient suppression and region-restricted techniques; SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Allender S., Scarborough P., Peto V., et. al.: European cardiovascular disease statistics.2008.European Heart NetworkBrussels


- 2\. Lloyd-Jones D., Adams R.J., Brown T.M., et. al.: Heart disease and stroke statistics—2010 update. Circulation 2010; 121: pp. e46-e215.


- 3\. Petitjean C., Dacher J.N.: A review of segmentation methods in short axis cardiac MR images. Med Image Anal 2011; 15: pp. 169-184.


- 4\. Kaus M.R., Berg J., Weese J., et. al.: Automated segmentation of the left ventricle in cardiac MRI. Med Image Anal 2004; 8: pp. 245-254.


- 5\. Pednekar A., Kurkure U., Muthupillai R., et. al.: Automated left ventricular segmentation in cardiac MRI. IEEE Trans Biomed Engineering 2006; 53: pp. 1425-1428.


- 6\. Chen T., Babb J., Kellman P., et. al.: Semiautomated segmentation of myocardial contours for fast strain analysis in cine displacement-encoded MRI. IEEE Trans Med Imaging 2008; 27: pp. 1084-1094.


- 7\. Lee H.Y., Codella N.C.F., Cham M.D., et. al.: Automatic left ventricle segmentation using iterative thresholding and an active contour model with adaptation on short-axis cardiac MRI. IEEE Trans Biomed Engineering 2010; 57: pp. 905-913.


- 8\. Pluempitiwiriyawej C., Moura J.M.F., Wu Y.J.L., et. al.: STACS: new active contour scheme for cardiac MR image segmentation. IEEE Trans Med Imaging 2005; 24: pp. 593-603.


- 9\. Lu Y., Radau P., Connelly K., et. al.: Segmentation of left ventricle in cardiac cine MRI: An automatic image-driven method. Functional Imaging and Modeling of the Heart 2009; 5528: pp. 339-347.


- 10\. Huang S., Liu J., Lee L.C., et. al.: An image-based comprehensive approach for automatic segmentation of left ventricle from cardiac short axis cine mr images. J Digit Imaging 2011; 24: pp. 598-608.


- 11\. Otsu N.: A threshold selection method from gray-level histograms. Automatica 1975; 11: pp. 285-296.


- 12\. Xu X., Xu S., Jin L., et. al.: Characteristic analysis of Otsu threshold and its applications. Pattern Recognition Lett 2011; 32: pp. 956-961.


- 13\. Yeh J., Fu J., Wu C., et. al.: Myocardial border detection by branch-and-bound dynamic programming in magnetic resonance images. Computer Meth Prog Biomed 2005; 79: pp. 19-29.


- 14\. Üzümcü M., van der Geest R.J., Swingen C., et. al.: Time continuous tracking and segmentation of cardiovascular magnetic resonance images using multidimensional dynamic programming. Investig Radiol 2006; 41: pp. 52.


- 15\. Mainali P., Yang Q., Lafruit G., et. al.: Robust low complexity corner detector. Circuits and Systems for Video Technology, IEEE Transactions on 2011; 21: pp. 435-445.


- 16\.  Xu XY, Xu SZ, Jin LH, et al. Using PSO to improve dynamic programming based algorithm for breast mass segmentation. In: Kenli L, ed. Proceedings 2010 IEEE Fifth International Conference on Bio-Inspired Computing: Theories and Applications. Institute of Electrical and Electronics Engineerings, Inc; 2010. p. 485-488.


- 17\. Lynch M., Ghita O., Whelan P.F.: Automatic segmentation of the left ventricle cavity and myocardium in MRI data. Comput Biol Med 2006; 36: pp. 389-407.


- 18\. Pikaz A., Averbuch A.: Digital image thresholding, based on topological stable-state. Pattern Recognition 1996; 29: pp. 829-843.


- 19\.  The data source and evaluation software. Available at:  http://sourceforge.net/projects/cardiac-mr/files/  . Accessed July 18, 2011.


- 20\. Chuang M.L., Gona P., Hautvast G.L.T.F., et. al.: Impact of left ventricular trabeculations and papillary muscles on measures of cavity volume and ejection fraction. Journal of Cardiovascular Magnetic Resonance 2011; 13: pp. 1-2.


- 21\. Lynch M., Ghita O., Whelan P.F.: Segmentation of the left ventricle of the heart in 3-D+ t MRI data using an optimized nonrigid temporal model. IEEE Trans Med Imaging 2008; 27: pp. 195-203.