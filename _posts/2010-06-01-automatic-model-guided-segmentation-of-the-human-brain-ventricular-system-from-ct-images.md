---
title: Automatic Model-guided Segmentation of the Human Brain Ventricular System From CT Images
author: [Jimin Liu PhD,Su Huang MS,Volkau Ihar PhD,Wojciech Ambrosius MD,Looi Chow Lee BS,Wieslaw L. Nowinski PhD]
date: 2010-06-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 17, Issue 6 SOURCE CL_S_AcademicRadiologyVolume17Issue6 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Accurate segmentation of the brain ventricular system on computed tomographic (CT) imaging is useful in neurodiagnosis and neurosurgery. Manual segmentation is time consuming, usually not reproducible, and subjective. Because of image noise, low contrast between soft tissues, large interslice distance, large shape, and size variations of the ventricular system, no automatic method is presently available. The authors propose a model-guided method for the automated segmentation of the ventricular system.

## Materials and Methods

Fifty CT scans of patients with strokes at different sites were collected for this study. Given a brain CT image, its ventricular system was segmented in five steps: (1) a predefined volumetric model was registered (or deformed) onto the image; (2) according to the deformed model, eight regions of interest were automatically specified; (3) the intensity threshold of cerebrospinal fluid was calculated in a region of interest and used to segment all regions of cerebrospinal fluid from the entire brain volume; (4) each ventricle was segmented in its specified region of interest; and (5) intraventricular calcification regions were identified to refine the ventricular segmentation.

## Results

Compared to ground truths provided by experts, the segmentation results of this method achieved an average overlap ratio of 85% for the entire ventricular system. On a desktop personal computer with a dual-core central processing unit running at 2.13 GHz, about 10 seconds were required to analyze each data set.

## Conclusion

Experiments with clinical CT images showed that the proposed method can generate acceptable results in the presence of image noise, large shape, and size variations of the ventricular system, and therefore it is potentially useful for the quantitative interpretation of CT images in neurodiagnosis and neurosurgery.

Because of its relatively short scanning time and low cost, computed tomographic (CT) imaging is widely used in neurosurgery and neurodiagnosis . To better analyze brain CT scans, segmentation of the ventricular system may be of importance for several reasons. First, the ventricular system is useful for the diagnosis of human brain abnormality: ventricular enlargement can be associated with some diseases, such as schizophrenia, ventriculitis, and meningitis. Second, information about the position, shape, and size of the ventricular system is helpful for locating ventricular hemorrhages and staging and treatment evaluation of brain stroke . Because the intensity of the ischemic region on a CT scan is usually between the cerebrospinal fluid (CSF) and gray matter (GM), and can even be overlapped with CSF regions, the accurate segmentation of the ventricular system is useful for ischemic region localization. Third, the segmented ventricular system can be used as an important anatomic landmark to guide the registration of a brain atlas such as the Talairach and Tournoux (TT) atlas with CT scans and thus to increase registration accuracy.

A number of methods have been developed for the extraction of the ventricular system from magnetic resonance images, for example, intensity-based methods such as thresholding and region growing , model-based methods such as atlas warping , geometric and parametric model deformation , and knowledge-based methods . However, no method is presently available for the automatic segmentation of the ventricular system from CT scans. This is due mainly to the following difficulties.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633210X00058/S1076633210001285/gr1.jpg?Signature=DA0cPtF8Gr-NaHx%7EcIPP9clUe%7EvGVsYyMCALKmdIObv-eqBpjjqDg-YiPXwbJuPQmOtj1TwETlHmLsWKyGeufOmLTJqVi4jkWkV51U1eN39WdZD7DA8tnPB0YUDZsKB1m273VJtPxGvLg7lWaHPE%7EvqT50cRKt6Or8OUa0sQQSU_&Expires=1669557693&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Histogram enhancement for cerebrospinal fluid (CSF) segmentation: **(a)** histogram of the whole computed tomographic scan; **(b)** histogram of whole brain tissue inside the brain skull: it is not suitable to segment the CSF in the brain, because the CSF peak is not distinguishable; and **(c)** local histogram calculated in the vicinity of the ventricular system: its CSF peak is enhanced and visible and is used to find the threshold of the CSF using Gaussian function fitting. GM, gray matter; WM, white matter.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633210X00058/S1076633210001285/gr2.jpg?Signature=ZSs6ctH9oW3UBtzHg1F0THq7tu5pOaBdlsErMadR-102XbSa99lxySo7zzLPkTperqdWe-KgFqEwnsXDNJ3-gcKMvsElu5Gb4nWkTPagUDot0Q4rmpDVgXvuxI801TjKbaUyBOZ0K-ygZv9Ih7zrzmQGBzJkWC2RU5ywSBXr0vw_&Expires=1669557693&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 2


Illustration of original images and segmentation results of subjects with different morphometric and pathologic features. The first row shows the original images of four subjects. The second row shows their segmentation results. The third row displays the three-dimensional models built from the segmentation results of the entire ventricles. **(a)** Subject with a large ischemic region adjacent to right ventricle. **(b)** Subject with very small ventricles. **(c)** Subject with serious intraventricular calcification. **(d)** Subject with very large ventricles.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633210X00058/S1076633210001285/gr3.jpg?Signature=btjrth8q3bglSDBlSmwqw1CS86qDB8m6CqJIyjD72ZZE2vzIq5w8RkigkSCQuCFrNtDw2kQN3ruWF6J4R43MLIX7Pn74poRpP9vnVkEpqUhSV8hF7VbkM-TyC1uL5hic90xPy0Mfi%7ECr9Uqm0uT47IF88AakfTz2oTF6wjhGB4k_&Expires=1669557693&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 3


Illustration of ventricular leakage problems: the third ventricle has a wide common boundary (region A1) with the lateral ventricle and leaks to the subarachnoid cavity at its posterior-inferior part (region A2); the lateral ventricle (region A3) leaks to the basal cistern through the region (A4) on its inferior neighboring slice.


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

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Construction of the ROI Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, The model is composed of five subvolumes from three-dimensional Talairach and Tournoux brain atlas: V 1 and V 2 are the left and right lateral ventricles, respectively, and V 3 and V 4 are the third and fourth ventricles, respectively. V 5 is the minimal nonventricular ellipsoid that passes the three landmark points (anterior commissure: P1; the middle point of the poster centerline intersect points [18] of the left and right lateral ventricles: P2; and the superior point of the fourth ventricle: P3) and contacts the two lateral ventricles.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticModelguidedSegmentationoftheHumanBrainVentricularSystemFromCTImages/0_1s20S1076633210001285.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Registration of ROI Model to Image

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Illustration of the automatic ventricular segmentation procedure: (a) an original slice; (b) the brain is extracted using morphologic analysis; (c) the middle sagittal plane (MSP) is extracted according to the local symmetry of brain anatomy; (d) a region-of-interest model is registered to the image according to the brain-bounding box and the MSP; (e) the cerebrospinal fluid (CSF) region is segmented; (f) CSF noise is removed using morphologic opening and closing operators; (g) CSF regions are separated into three parts (left, right, and middle); (h) the main parts of the lateral ventricles are identified using connected component analysis); (i) the remaining parts of two lateral ventricles are found using boundary patch–based region growing; (j) expansion of lateral ventricles in the middle sagittal slab and nonventricular ellipsoid; (k) the third and fourth ventricles are found; and (l) calcification regions are identified.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticModelguidedSegmentationoftheHumanBrainVentricularSystemFromCTImages/1_1s20S1076633210001285.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Generation of ROI in Image

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Ω0=V0∪Ω(V′5,−d1),
Ω

0

=

V

0

∪

Ω

(

V

5

′

,

−

d

1

)

,


Ωi=Ω(V′i,d2)−Ω0fori=1,2;Ωi=Ω(V′i,d2)fori=3,4,
Ω

i

=

Ω

(

V

i

′

,

d

2

)

−

Ω

0

for

i

=

1

,

2

;

Ω

i

=

Ω

(

V

i

′

,

d

2

)

for

i

=

3

,

4

,


Ω5=V10−Ω0;Ω6=V20−Ω0,
Ω

5

=

V

0

1

−

Ω

0

;

Ω

6

=

V

0

2

−

Ω

0

,


and


Ω7=Ω(V′1∪V′2,d2),
Ω

7

=

Ω

(

V

1

′

∪

V

2

′

,

d

2

)

,


where _d_ 1 and _d_ 2 are given constants with their values empirically set to 4 and 6 mm, respectively. Region Ω  0 is used to avoid the leakage of the two lateral ventricles, region Ω  7 is used to calculate the CSF intensity threshold, and regions Ω  1 to Ω  6 are used for the segmentation of four ventricles.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Calculation of the CSF Threshold

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

f(x)=∑2i=1hiexp\[(x−μi)2/(2σ21)\],
f

(

x

)

=

∑

i

=

1

2

h

i

exp

\[

(

x

−

μ

i

)

2

/

(

2

σ

1

2

)

\]

,


where _x_ is the intensity value, μ the mean, σ the standard deviation, and _h_ the height of the Gaussian function.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Segmentation of the Ventricular System

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Identification of Intraventricular Calcification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Comparison Between Our Ventricular Segmentation Results and Ground Truth on Images With Different Representative Features


Left Ventricle Right Ventricle Third Ventricle Fourth Ventricle Four Ventricles Subject DSC FP FN DSC FP FN DSC FP FN DSC FP FN DSC FP FN 1 82.1 0.3 30.1 70.4 36.5 15.0 60.1 23.2 47.0 74.2 23.3 27.2 74.1 21.6 22.5 2 87.2 4.6 19.1 84.4 2.0 25.6 47.0 83.9 12.8 57.7 82.7 5.6 78.3 14.1 20.2 3 78.6 0.5 35.0 85.6 14.3 14.4 74.4 29.8 23.1 70.6 41.3 23.0 82.2 10.1 23.2 4 96.1 2.2 7.4 96.4 0.8 6.9 92.0 13.1 8.6 96.4 6.5 6.9 96.3 1.3 7.1 5 92.1 0.4 14.3 90.1 0.2 17.8 51.7 32.1 54.4 46.3 20.8 63.6 90.1 1.1 17.1 6 83.7 3.2 25.7 80.2 0.8 32.5 80.2 17.7 21.2 73.1 19.1 31.4 80.9 5.4 28.5 7 92.5 0.8 13.2 92.2 1.1 13.5 78.9 35.7 11.7 80.7 5.9 28.4 91.5 2.7 13.4 8 82.1 31.5 8.4 78.7 37.6 4.2 66.2 72.2 14.7 31.3 79.3 48.1 78.9 36.8 7.6 9 75.7 32.0 13.6 74.2 41.3 10.8 49.6 89.5 31.1 51.8 76.6 3.3 72.1 40.1 13.1 10 81.2 8.9 25.6 81.5 7.3 26.2 74.9 19.2 28.6 88.7 1.8 18.9 81.0 9.0 25.9 11 81.2 8.6 25.8 79.1 7.8 29.5 69.9 22.6 34.2 79.9 34.1 10.9 79.4 10.7 27.1 12 86.8 6.9 18.0 86.3 7.3 18.6 75.2 49.1 10.2 83.8 11.5 19.6 85.8 9.3 17.9 13 63.9 19.1 44.1 77.3 23.6 22.1 63.7 85.7 13.2 77.2 37.5 13.7 71.1 27.1 29.8 14 89.0 4.2 16.4 90.2 2.5 15.8 76.1 9.3 32.9 66.0 10.6 45.5 88.5 3.8 17.5

DSC, Dice similarity coefficient; FP, false-positive ratio; FN, false-negative ratio.


Table 2


Performance Statistics of Our Method on the Entire Data Set ( _n_ = 50)


Left Ventricle Right Ventricle Third Ventricle Fourth Ventricle Four Venticles DSC FP FN DSC FP FN DSC FP FN DSC FP FN DSC FP FN Mean 85.0 6.1 16.2 85.8 8.37 17.2 67.5 41.8 27.8 58.8 42.9 38.6 84.8 10.1 18.0 Standard deviation 7.8 9.5 10.3 6.8 15.5 7.8 18.3 38.1 19.9 29.7 49.6 31.5 7.1 12.8 7.5

DSC, Dice similarity coefficient; FP, false-positive ratio; FN, false-negative ratio.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

## Statistical Versus Structural Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Shape-based Interpolation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Shape-based interpolation of ventricular system: (a) a ventricular system segmented from a computed tomographic image and (b) interpolation of the ventricular system using shape-based interpolation (17).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticModelguidedSegmentationoftheHumanBrainVentricularSystemFromCTImages/2_1s20S1076633210001285.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Limitations and Further Improvement

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## _boundary Patch–based Region-Growing Procedure_

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

∂i,k+1=∪p∈∂i,k{q\|q∈N26(p),q∈Ω}−\[K∪(∪ni=1∂i,k)\](k=0,1,2,…),
∂

i

,

k

+

1

=

∪

p

∈

∂

i

,

k

{

q

\|

q

∈

N

26

(

p

)

,

q

∈

Ω

}

−

\[

K

∪

(

∪

i

=

1

n

∂

i

,

k

)

\]

(

k

=

0

,

1

,

2

,

…

)

,


where _N_ 26 ( **p** ) represents all the 26 neighbors of the voxel **p** . The procedure of generating ∂ _i_ , _k_ +1 from ∂ _i_ , _k_ continues either until ∂i,ki+1
∂

i

,

k

i

+

1
is empty or the number of voxels in ∂i,ki+1
∂

i

,

k

i

+

1
is more than twice the number of voxels in the previous step ∂i,ki
∂

i

,

k

i
(ie, # ∂i,ki+1
∂

i

,

k

i

+

1
\> 2 × # ∂i,ki
∂

i

,

k

i
). The last stopping condition is used to avoid leakage.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

X=∪ni=1(∪kij=0∂i,j)∪K.
X

=

∪

i

=

1

n

(

∪

j

=

0

k

i

∂

i

,

j

)

∪

K

.


The region X is regarded as the result of the region-growing procedure. For the ventricular segmentation, the candidate region Ω is the related CSF region.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Hu X., Jiang X., Zhou X., et. al.: Risks of intracranial hemorrhage in patients with Parkinson's disease receiving deep brain stimulation and ablation. Parkinsonism Relat Disord 2010; 16: pp. 96-100.


- 2\. Liu F., Qian J., Lu Y.: Computer-assisted stereotactic neurosurgery with framework neurosurgery navigation. Clin Neurol Neurosurg 2008; 110: pp. 696-700.


- 3\. Nowinski W.L., Qian G., Prakash K.N.B., et. al.: Stroke Suite: CAD systems for acute ischemic stroke, hemorrhagic stroke, and stroke in ER. Med Imaging Informatics 2008; 4987: pp. 377-386.


- 4\. Talairach J., Tournoux P.: Coplanar stereotactic atlas of the human brain.1988.ThiemeStuttgart, Germany


- 5\. Worth A.J., Makris N., Patti M.R., et. al.: Precise segmentation of the lateral ventricles and caudate nucleus in MR brain images using anatomically driven histograms. IEEE Trans Med Imaging 1998; 17: pp. 303-310.


- 6\. Schnack H.G., Hulshoff P.H.E., Baare W.F.C., Viergever M.A., Kahn R.S.: Automatic segmentation of the ventricular system from MR images of the human brain. Neuroimage 2001; 14: pp. 95-104.


- 7\. Sonka M., Tadikonda S.K., Collins S.M.: Knowledge-based interpretation of MR brain images. IEEE Trans Med Imaging 1996; 15: pp. 443-452.


- 8\. Xia Y., Hu Q., Aziz A., Nowinski W.L.: A knowledge-driven algorithm for a rapid and automatic extraction of the human cerebral ventricular system for MR meuroimages. Neuroimage 2004; 21: pp. 269-282.


- 9\. Holden M., Schnable J.A., Hill D.L.G.: Quantifying small changes in brain ventricular volume using non-rigid registration. Lecture Notes Comput Sci 2010; 2208: pp. 49-56.


- 10\. Baillard C., Hellier P., Barillot C.: Segmentation of 3D brain structures using level sets and dense registration. IEEE Workshop Math Methods Biomed Image Anal 2000; pp. 94-101.


- 11\. Kaus M.R., Warfield S.K., Nabavi A., Black P.M., Jolesz F.A., Kikinis R.: Automated segmentation of MR images of brain tumors. Radiology 2001; 218: pp. 586-591.


- 12\. Shen D., Herskovits E.H., Davatzikos C.: An adaptive-focus statistical shape model for segmentation and shape modeling of 3-D brain structure. IEEE Trans Med Imaging 2001; 20: pp. 257-270.


- 13\. Liu J., Huang S., Nowinski W.L.: Automatic segmentation of the human brain ventricles in MR images by knowledge-based region growing and trimming. Neuroinformatics 2009; 7: pp. 131-146.


- 14\. Han X., Fischl B.: Atlas renormalization for improved brain MR image segmentation across scanner platforms. IEEE Trans Med Imaging 2007; 26: pp. 479-486.


- 15\. Showalter C., Clymer B.D., Richmond B., Powell K.: Three-dimensional texture analysis of cancellous bone cores evaluated at clinical CT resolutions. Osteoporosis Int 2006; 17: pp. 259-266.


- 16\. Al-Kadi O.S., Watson D.: Texture analysis of aggressive and nonaggressive lung tumor CE CT images. IEEE Trans Biomed Eng 2008; 55: pp. 1822-1830.


- 17\. Liu J., Nowinski W.L.: A hybrid approach to shape-based interpolation of stereotactic atlases of the human brain. Neuroinformatics 2006; 4: pp. 177-198.


- 18\. Liu J., Gao W., Huang S., Nowinski W.L.: A model-based, semi-global segmentation approach for automatic 3D point landmark localization in neuroimages. IEEE Trans Med Imag 2008; 27: pp. 1034-1044.


- 19\. Mangin J.F., Frouin V., Bloch I., Regis J., Lopez-Krahe J.: From 3D magnetic resonance images to structural representations of the cortex topography using topology preserving deformations. J Math Imag Vision 1995; 5: pp. 297-318.


- 20\. Volkau I., Bhanu Prakash K.N., Anand A., Aziz A., Nowinski W.L.: Extraction of the midsagittal plane from morphological neuroimages using the Kullback-Leibler's measure. Med Image Anal 2006; 10: pp. 863-874.


- 21\. Maurer C.R., Qi J.R., Raghavan V.: A linear time algorithm for computing exact Euclidean distance transforms of binary images in arbitrary dimensions. IEEE Trans PAMI 2003; 25: pp. 265-270.


- 22\. Gonzalez R.C., Woods R.E.: Digital Image Processing.1993.Addison-WesleyBoston


- 23\. Liu J., Huang S., Aziz A., Nowinski W.L.: Three dimensional digital atlas of the orbit constructed from multi-modal radiological images. Int J Comput Assist Radiol Surg 2007; 1: pp. 275-283.


- 24\. Liu J., Huang S., Nowinski W.L.: A hybrid approach for segmentation of anatomic structures in medical images. Int J Comput Assist Radiol Surg 2008; 3: pp. 213-219.


- 25\. Nowinski W.L., Qian G., Prakash K.N.B., Hu Q., Aziz A.: Fast Talairach transformation for magnetic resonance neuroimages. J Comput Assist Tomogr 2006; 30: pp. 629-641.