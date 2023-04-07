---
title: Automated Method for Identification of Patients With Alzheimer’s Disease Based on Three-dimensional MR Images
author: [CL_AT_HidetakaArimuraPhD,CL_AT_TakashiYoshiuraMDPhD,CL_AT_SeijiKumazawaPhD,CL_AT_KazuhiroTanakaMDPhD,CL_AT_HiroshiKogaMDPhD,CL_AT_FutoshiMiharaMDPhD,CL_AT_HiroshiHondaMDPhD,CL_AT_ShujiSakaiMDPhD,CL_AT_FukaiToyofukuPhD,CL_AT_YoshiharuHigashidaPhD]
date: 2008-03-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 15, Issue 3]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

An automated method for identification of patients with cerebral atrophy due to Alzheimer’s disease (AD) was developed based on three-dimensional (3D) T1-weighted magnetic resonance (MR) images.

## Materials and Methods

Our proposed method consisted of determination of atrophic image features and identification of AD patients. The atrophic image features included white matter and gray matter volumes, cerebrospinal fluid (CSF) volume, and cerebral cortical thickness determined based on a level set method. The cortical thickness was measured with normal vectors on a voxel-by-voxel basis, which were determined by differentiating a level set function. The CSF spaces within cerebral sulci and lateral ventricles (LVs) were extracted by wrapping the brain tightly in a propagating surface determined with a level set method. Identification of AD cases was performed using a support vector machine (SVM) classifier, which was trained by the atrophic image features of AD and non-AD cases, and then an unknown case was classified into either AD or non-AD group based on an SVM model. We applied our proposed method to MR images of the whole brains obtained from 54 cases, including 29 clinically diagnosed AD cases (age range, 52−82 years; mean age, 70 years) and 25 non-AD cases (age range, 49−78 years; mean age, 62 years).

## Results

As a result, the area under a receiver operating characteristic (ROC) curve ( _Az_ value) obtained by our computerized method was 0.909 based on a leave-one-out test in identification of AD cases among 54 cases.

## Conclusion

This preliminary result showed that our method may be promising for detecting AD patients.

Alzheimer’s disease (AD) is a dementing disorder and one of the major public health problems in countries with greater longevity, such as Japan, where the average citizen lived for 82 years in 2004 ( ). AD is a progressive neurodegenerative disorder of hitherto unknown etiology leading progressively to severe incapacity and death ( ). AD is associated with the atrophy of gray matter in the cerebral cortex, which leads to a volume decrease of the cerebral cortex or a volume increase of cerebrospinal fluid (CSF) in cerebral sulci and lateral ventricles (LVs), which can be measured in magnetic resonance (MR) images. In order to provide appropriate care for AD patients, it is very important to quantitatively evaluate the degree of the atrophy in the cerebral cortex at the early stage of AD. Neuroradiologists attempt to estimate the degree of atrophy by capturing atrophic image features on MR images, but it is very difficult and time consuming in routine clinical practice. Therefore, a number of automated methods for segmentation of gray matter and white matter regions ( ), measurement of the cortical thickness ( ), and volumetric measurement of the CSF in cerebral sulci and LVs ( ) have been studied so that the progression of cerebral atrophy can be monitored. However, such image features have not been employed for identification of AD patients.

In recent years, a whole-brain unbiased objective technique, known as voxel-based morphometry (VBM), has been developed for characterizing differences in the local composition of brain tissue using MR images and can objectively map gray matter loss on a voxel-by-voxel basis ( ). The VBM is achieved by spatially normalizing all brains to the same standardized brain acquired from many normal subjects, segmenting the normalized brain into gray and white matter, smoothing the gray and white matter images, and then finally performing a statistical analysis to localize significant differences between two or more experimental groups. On the other hand, the computer-aided diagnosis (CAD) methods based on a pattern recognition technique using image features have been developed and may be promising for detection of abnormalities in the field of neuroradiology ( ). Therefore, such CAD approaches should be studied for detection of AD patients. To our knowledge, no studies have ever tried to develop CAD systems based on pattern recognition techniques with the atrophic image features, which would be automatically determined. For the purpose, we have developed two automated methods for measurement of the cortical thickness ( ) and for volumetric measurement of CSF regions in cerebral sulci and LVs ( ). In this study, we attempted to develop an automated method for identification of patients with cerebral atrophy due to AD based on a novel pattern recognition technique using 3D MR images.

## Materials and methods

## Subjects and MRI Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Overall Algorithm

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Fig 1, Overall algorithm for identification of patients with the cerebral atrophy due to Alzheimer’s disease based on MR images.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/0_1s20S1076633207006307.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Determination of Atrophic Image Features

## Volumes of White Matter and Gray Matter Regions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ψn+1=ψn−ΔtF∣∣∇ψ∣∣,
ψ

n

+

1

=

ψ

n

−

Δ

t

F

\|

∇

ψ

\|

,


The new zero level set ψ = 0 moves depending on the speed function _F_ . In this study, the speed function _F_ was given by


F=am(ν−ρκ),
F

=

a

m

(

ν

−

ρ

κ

)

,


where


m=11+\|∇{Gσ⊗I(x,y,z)}\|,
m

=

1

1

+

\|

∇

{

G

σ

⊗

I

(

x

,

y

,

z

)

}

\|

,


_a_ , ν, and ρ are constants, κ is the mean curvature, _G  σ_ is the Gaussian function with a standard deviation of _σ_ , _I_ (x,y,z) is the original image to be processed, and ⊗ means convolution. The constants _a_ and ν function as accelerator and inflation terms, and the curvature _κ_ gives influence on the smoothness of the front. The values _a, v, ρ_ , and _σ_ were set as 1.1, 1.0, 0.5, and 1.1, respectively, which were empirically determined. The value _m_ plays a key role on more accurate segmentation, because the speed function _F_ would decrease and the level set function ψ would hardly change if the moving front approaches an edge of an object. Consequently, we can expect that the zero level set would be at the boundary of a desired object, i.e., the brain surface. Therefore, by monitoring the speed function, the boundary can be determined automatically.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Fig 2, Segmentation of four regions for determination of atrophic image features for an AD patient: ( a ) a brain region and a white matter region in sagittal planes, ( b ) CSF regions in sulci in a coronal plane, and ( c ) CSF regions in LVs in an axial plane.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/1_1s20S1076633207006307.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Volumes of CSF regions in cerebral sulci and lateral ventricles

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

F=−exp(−α∇{Gσ⊗I(x,y,z)}),
F

=

−

exp

⁡

(

−

α

∇

{

G

σ

⊗

I

(

x

,

y

,

z

)

}

)

,


where _α_ is the constant, which was set as α = 3.0 for this study. If the speed _F_ at a center voxel in a region of interest (ROI) with 3 × 3 × 3 would be slower than a threshold speed—i.e., the propagating surface approaches an edge of a brain, the speeds _F_ for 26 neighbors were controlled for wrapping the brain in the propagating surface tightly by the following equation:


Fs=F{1−exp(−βd)},
F

s

=

F

{

1

−

exp

⁡

(

−

β

d

)

}

,


where _Fs_ is the controlled speed determined by Equation  5 , _d_ is the distance between a voxel and a center of the ROI, and _β_ is the constant, which was set as 0.5 for this study. Consequently, the propagating surface would not intrude sulci and stop at around edge of the brain.

![Fig 3, ( a ) Illustration of a sphere with a radius of the maximum distance between the centroid of the segmented brain and the brain surface, which was embedded as a zero level set at the centroid of the segmented brain. ( b ) Illustration of a lateral ventricle (LV) model used for extracting LV regions.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/2_1s20S1076633207006307.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Cerebral cortical thickness

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Fig 4, Labeling of 32 subregions in a divided brain region for measurement of cortical thickness: ( a ) upper region (Nos.1−16) and ( b ) lower region (Nos. 17−32).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/3_1s20S1076633207006307.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

n=∇ψ
n

=

∇

ψ


A normal vector for measuring of the cortical thickness is shown by solid line with an arrow in  Figure 5 . The cortical thickness was measured from the absolute value of the vector **T** obtained by extending the normal vector from the white matter surface to the cortical gray matter surface (brain surface) by using the following equation:


T=v0+tn,
T

=

v

0

+

t

n

,


where _v_ 0 is the voxel on the white matter surface and _t_ is the parameter for this linear Equation  7 . Mean cortical thicknesses were measured in the 32 subregions of a brain.

![Fig 5, Illustration of a method for measurement of the cortical thickness based on a normal vector on the white matter surface. The cortical thickness was measured from the absolute value of the vector T obtained by extending the normal vector from the white matter surface to the cortical gray matter surface (brain surface).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/4_1s20S1076633207006307.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Identification of AD Patients Based on Support Vector Machine

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_G=∣∣μp−μn∣∣σp+σn,_
_G_

_=_

_\|_

_μ_

_p_

_−_

_μ_

_n_

_\|_

_σ_

_p_

_+_

_σ_

_n_

_,_

_where  μ  p  and  μ  n  are the mean cortical thicknesses in a subregion for positive (AD) and negative (non-AD) case groups, respectively, and  σ  p  and  σ  n  are the standard deviations of the cortical thicknesses for positive and negative case groups, respectively. Because the Golub statistic can be interpreted as the degree of separation between the two classes, mean cortical thickness in the effective subregion, which indicated Golub statistic greater than a threshold value, was selected for an input of the SVM. In this study, the threshold value was empirically set as 0.6._

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)__## Performance Evaluation Method_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)__## Results_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_![Fig 6, Atrophic image features: ( a ) relationship between white matter volume and volume ratio of white matter region to whole brain, ( b ) relationship between gray matter volume and volume ratio of gray matter region to whole brain, and ( c ) relationship in CSF volume ratio to whole brain in sulci and LVs.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/5_1s20S1076633207006307.jpg)_

_![Fig 7, Relationship in mean cortical thickness for the upper subregion No. 6 and lower subregion No. 22, which roughly correspond to a part of parietal lobe and temporal lobe, respectively. The subregion numbers correspond to the numbers shown in Figure 4 .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/6_1s20S1076633207006307.jpg)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_![Fig 8, ROC curve obtained by using the SVM classifier for distinction between AD and non-AD cases.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/7_1s20S1076633207006307.jpg)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_## Discussion_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_## Conclusions_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_## Acknowledgments_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_## Appendix_

_## Method for Division of a Brain Into Small Subregions_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_![Fig A1, Illustration of a method for division of a brain region into small subregions. The maximum widths of a brain in x and y directions, Bwx and Bwy ,were determined for each brain region. The brain region was divided into 4 × 4 regions, i.e., 16 subregions as shown in a , and then the maximum width in z direction, Bwz , was determined in a sagittal plane, as shown in b , at the first quarter ( Bwx /4) of the brain in the x direction indicated by a white dotted line in a . The brain region was split into upper and lower regions at the sagittal plane as shown in b .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedMethodforIdentificationofPatientsWithAlzheimersDiseaseBasedonThreedimensionalMRImages/8_1s20S1076633207006307.jpg)_

_[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)_

_## References_

_- 1\. World Health Organization: The World Health Report 2006: Working Together for Health. http://www.who.int/whr/2006/en/index.html_

_- 2\. Jellinger K.A.: Alzheimer 100: Highlights in the history of Alzheimer research. J Neural Transm 2006; 113: pp. 1603-1623._


_- 3\. Xu C., Pham D.L., Rettmann M.E., et. al.: Reconstruction of the human cerebral cortex from magnetic resonance images. IEEE Trans Med Imaging 1999; 18: pp. 467-480._


_- 4\. Kovacevic N., Lobaugh N.J., Bronskill M.J., et. al.: A robust method for extraction and automatic segmentation of brain images. NeuroImage 2002; 17: pp. 1087-1100._


_- 5\. Goldenberg R., Kimmel R., Rivlin E., et. al.: Cortex segmentation: A fast variational geometric approach. IEEE Trans Med Imaging 2002; 21: pp. 1544-1551._


_- 6\. Zeng X., Staib L.H., Schultz R.T., et. al.: Segmentation and measurement of the cortex from 3D MR images using coupled surfaces propagation. IEEE Trans Med Imaging 1999; 18: pp. 100-101._


_- 7\. MacDonald D., Kabani N., Avis D., et. al.: Automated 3D extraction of inner and outer surfaces of cerebral cortex from MRI. NeuroImage 2000; 12: pp. 340-356._


_- 8\. Fischl B., Dale A.M.: Measuring the thickness of the human cerebral cortex from magnetic resonance images. PNAS 2000; 97: pp. 11050-11055._


_- 9\. Jones S.E., Buchbinder B.R., Aharon I.: Three-dimensional mapping of cortical thickness using Laplace’s equation. Hum Brain Mapp 2000; 11: pp. 12-32._


_- 10\. Thacker N.A., Varma A.R., Bathgate D.: Dementing disorders: Volumetric measurement of cerebrospinal fluid to distinguish normal from pathologic findings—Feasibility study. Radiology 2002; 224: pp. 278-285._


_- 11\. Barra V., Frenoux E., Boire J.-Y.: Automatic volumetric measurement of lateral ventricles on magnetic resonance images with correction of partial volume effects. J Magn Reson Imaging 2002; 15: pp. 16-22._


_- 12\. Ashburner J., Friston K.J.: Voxel-based morphometry: The methods. NeuroImage 2000; 11: pp. 805-821._


_- 13\. Hirata Y., Matsuda H., Nemoto K., et. al.: Voxel-based morphometry to discriminate early Alzheimer’s disease from controls. Neurosci Lett 2005; 382: pp. 269-274._


_- 14\. Arimura H., Li Q., Korogi Y., et. al.: Automated computerized scheme for detection of unruptured intracranial aneurysms in three-dimensional MRA. Acad Radiol 2004; 11: pp. 1093-1104._


_- 15\.  Arimura H, Li Q, Korogi Y, et al. Computerized detection of intracranial aneurysms for 3D MR angiography: Feature extraction of small protrusions based on a shape-based difference image technique. Med Phys 33:394–401._


_- 16\. Arimura H., Yoshiura T., Kumazawa S., et. al.: Computerized method for automated measurement of thickness of cerebral cortex for 3D MR images. SPIE Proc 2006; 6144: pp. 1239-1246._


_- 17\. Arimura H., Yoshiura T., Kumazawa S., et. al.: Automated volumetric measurement of cerebrospinal fluid in sulci and lateral ventricles based on 3D MR images. IFMBE Proc 2006; 14: pp. 2184-2187._


_- 18\. Sethian J.A.: Level Set Methods and Fast Marching Methods: Evolving Interfaces in Computational Geometry, Fluid Mechanics, Computer Vision, and Materials Science.1999.Cambridge University PressCambridge_


_- 19\. Malladi R., Sethian J.A., Vemuri B.C.: Shape modeling with front propagation: A level set approach. IEEE Trans Pattern Anal Mach Intell 1995; 17: pp. 158-175._


_- 20\. Deng J., Tsui H.T.: A fast level set method for segmentation of low contrast noisy biomedical images. Pattern Recogn Lett 2002; 23: pp. 161-169._


_- 21\. Vapnik V.N.: The Nature of Statistical Learning Theory: Statistics for Engineering and Information Science.2nd ed.1999.Springer-VerlagNew York_


_- 22\. Cristianini N., Shawe-Taylor J.: An Introduction to Support Vector Machines and Other Kernel-Based Learning Methods.2000.Cambridge University PressCambridge_


_- 23\. Joachims T.: _SVM  light_ . Cornell University. http://svmlight.joachims.org/_

_- 24\.  Campadelli P, Casiraghi E, Artioli D. A fully automated method for lung nodule detection from postero-anterior chest radiographs. IEEE Trans Med Imaging 25:1588–1603._


_- 25\. Golub T.R., Slonim D.K., Tamayo P., et. al.: Molecular classification of cancer: Class discovery and class prediction by gene expression monitoring. Science 1999; 286: pp. 531-537._


_- 26\. Jain A.K., Duin R.P.W., Jianchang M.: Statistical pattern recognition: a review. IEEE Trans Pattern Anal Mach Intell 2000; 22: pp. 4-37._


_- 27\. Metz C.E.: ROC Software ROCKIT. http://xray.bsd.uchicago.edu/krl/roc\_soft6.htm_

_- 28\. Matsumae M., Kikinis R., Mórocz L., et. al.: Intracranial compartment volumes in patients with enlarged ventricles assessed by magnetic resonance-based image processing. J Neurosurg 1996; 84: pp. 972-981._


_- 29\. Jorm A.F., Korten E., Henderson A.S.: The prevalence of dementia: A quantitative integration of the literature. Acta Psychiat Scand 1987; 76: pp. 465-479._


_- 30\. Mölsä P.K., Matilla R.J., Rinne U.K.: Epidemiology of dementia in a Finnish population. Acta Neurol Scand 1982; 65: pp. 541-552._


_- 31\. Yamada T., Kadekaru H., Matsumoto S., et. al.: Prevalence of dementia in the older Japanese-Brazilian population. Psychiatry Clin Neurosci 2002; 56: pp. 71-75._