---
title: Evaluation of Hepatic Tumor Response to Yttrium-90 Radioembolization Therapy Using Texture Signatures Generated from Contrast-enhanced CT Images
author: [Rebekah H. Gensure BS,David J. Foran PhD,Vincent M. Lee MD,Vyacheslav M. Gendel MD,Salma K. Jabbour MD,Darren R. Carpizo MD PhD,John L. Nosher MD,Lin Yang PhD]
date: 2012-10-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 10 SOURCE CL_S_AcademicRadiologyVolume19Issue10 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to explore the use of texture features generated from liver computed tomographic (CT) datasets as potential image-based indicators of patient response to radioembolization (RE) with yttrium-90 (  90 Y) resin microspheres, an emerging locoregional therapy for advanced-stage liver cancer.

## Materials and Methods

Overall posttherapy survival and percent change in serologic tumor marker at 3 months posttherapy represent the primary clinical outcomes in this study. Thirty advanced-stage liver cancer cases (primary and metastatic) treated with RE over a 3-year period were included. Texture signatures for tumor regions, which were delineated to reveal boundaries with normal regions, were computed from pretreatment contrast-enhanced liver CT studies and evaluated for their ability to classify patient serologic response and survival.

## Results

A series of systematic leave-one-out cross-validation studies using soft-margin support vector machine (SVM) classifiers showed hepatic tumor texton and local binary pattern (LBP) signatures both achieve high accuracy (96%) in discriminating subjects in terms of their serologic response. The image-based indicators were also accurate in classifying subjects by survival status (80% and 93% accuracy for texton and LBP signatures, respectively).

## Conclusions

Hepatic texture signatures generated from tumor regions on pretreatment triphasic CT studies were highly accurate in differentiating among subjects in terms of serologic response and survival. These image-based computational markers show promise as potential predictive tools in candidate evaluation for locoregional therapy such as RE.

Radioembolization with yttrium-90 (  90 Y) microspheres (  90 Y-RE) is an effective locoregional treatment for primary and metastatic cancers of the liver. This therapy is generally reserved for patients with advanced-stage liver cancer that is deemed not surgically resectable or that has failed to respond to standard chemotherapy . Significant clinical benefit has been reported with radioembolization in both primary and metastatic cancers of the liver , but it has also been observed that a subpopulation of patients undergoing radioembolization may exhibit disease progression. This disparity in response is currently not well understood.

Previous work has evaluated the influence of potentially indicative clinical features in colorectal cancer liver metastases such as tumor size, grade, and carcinoembryonic antigen level and found that these factors alone do not predict response to  90 Y-RE . One recent investigation identified several independent clinical factors including the presence of cancer-related symptoms, high hepatic tumor burden, and elevated bilirubin that may correlate with prognosis . Another study developed a complex dosimetric model to predict metabolic response (expected changes on positron emission tomography) . This model suggests a fairly accurate way of estimating response of individual tumors, but does not necessarily generalize to overall patient response. Given the high costs and potential risks associated with this therapy, there is a growing need to develop a set of robust prognostic tools to predict patient response to radioembolization.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## CT Volume Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Radioembolization Therapy

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Response Outcomes

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Semiautomated Hepatic Tumor Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Texture Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Representative liver computed tomography axial slice showing tumor on arterial phase ( left ) and corresponding texture representations ( right ) using several scales of filter responses within the LM filter bank.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationofHepaticTumorResponsetoYttrium90RadioembolizationTherapyUsingTextureSignaturesGeneratedfromContrastenhancedCTImages/0_1s20S1076633212003042.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Schematic showing how tumor volume is divided into orthogonal anatomical planes for texture analysis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationofHepaticTumorResponsetoYttrium90RadioembolizationTherapyUsingTextureSignaturesGeneratedfromContrastenhancedCTImages/1_1s20S1076633212003042.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Supervised Learning Experiments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Support vector machine classification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Dimensionality reduction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

xˆi=T(xi)+ui,i=1,2,⋯,n
x

ˆ

i

=

T

(

x

i

)

+

u

i

,

i

=

1

,

2

,

⋯

,

n


where ui∈Rd
u

i

∈

ℝ

d
represents the sampling noise and xˆi∈Rd'
x

ˆ

i

∈

ℝ

d

'
represents the feature vector xi
x

i
in the low-dimensional subspace. Depending on the nature of the dataset, the mapping _T_ can be obtained by traditional linear techniques, such as principal component analysis (PCA), or by nonlinear techniques, such as isometric feature mapping (ISOMAP) and locally linear embedding (LLE) . In this liver cohort, because we do not know a priori the nature of the underlying manifold from which we are sampling, we explore both linear and nonlinear dimensionality reduction approaches. PCA is a method in which the mapping TPCA
T

P

C

A
represents linear combinations of the input vectors constructed to maximize the variance captured along each component in the reduced subspace. The ISOMAP technique calculates a graph based on geodesic distances between points and then applies multidimensional scaling to the graph distances to obtain the low-dimensional mapping TISOMAP
T

I

S

O

M

A

P
. LLE reconstructs the high-dimensional input points as linear combinations of their neighbors, thus preserving the local geodesic distance.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Patient Characteristics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Baseline Patient Characteristics


Demographics Total ( n=30
n

=

30
) Age≥65
≥

65
9 (30%)<65
<

65
21 (70%) Gender Male 16 (53%) Female 14 (47%) Primary diagnosis Colorectal 21 (70%) Breast 3 (10%) Neuroendocrine 1 (3%) Hepatocellular 1 (3%) Melanoma 1 (3%) Other 3 (10%) Treatment cycles 2 (bilobar) 20 (67%) 1 (whole liver) 10 (33%)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Dimensionality Reduction and Classification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Error rate estimation for three different dimensionality reduction techniques as a function of number of reduced dimensions in distinguishing subjects by serologic response using texton signatures.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/EvaluationofHepaticTumorResponsetoYttrium90RadioembolizationTherapyUsingTextureSignaturesGeneratedfromContrastenhancedCTImages/2_1s20S1076633212003042.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Texture Signature Performance in Survival Classification (n = 30)


Texture Signature DR Method Accuracy (%) Sensitivity (%) Specificity (%) Texton PCA 66.7 33.3 93.3 ISOMAP 80.0 66.7 93.3 LLE 70.0 53.3 86.7 LBP PCA 93.3 86.7 100 ISOMAP 93.3 86.7 100 LLE 76.7 73.3 80.0

DR, dimensionality reduction; ISOMAP, isometric feature mapping; LBP, local binary pattern; LLE, locally linear embedding; PCA, principal component analysis.


Table 3


Texture Signature Performance in Serologic Response Classification (n = 30)


Texture Signature DR Method Accuracy (%) Sensitivity (%) Specificity (%) Texton PCA 96.7 100 93.3 ISOMAP 96.7 93.3 100 LLE 76.7 80.0 73.3 LBP PCA 96.7 100 93.3 ISOMAP 86.7 86.7 86.7 LLE 73.3 86.7 60.0

DR, dimensionality reduction; ISOMAP, isometric feature mapping; LBP, local binary pattern; LLE, locally linear embedding; PCA, principal component analysis.


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

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Stubbs R.S., Wickremesekera S.K.: Selective internal radiation therapy (SIRT): a new modality for treating patients with colorectal liver metastases. HPB 2004; 6: pp. 133-139.


- 2\. Miller F.H., Keppke A.L., Reddy D., et. al.: Response of liver metastases after treatment with yttrium-90 microspheres: role of size, necrosis, and PET. AJR Am J Roentgenol 2007; 188: pp. 776-783.


- 3\. Dunfee B.L., Riaz A., Lewandowski R.J., et. al.: Yttrium-90 radioembolization for liver malignancies: prognostic factors associated with survival. J Vasc Intervent Radiol 2010; 21: pp. 90-95.


- 4\. Flamen P., Vanderlinden B., Delatte P., et. al.: Multimodality imaging can predict the metabolic response of unresectable colorectal liver metastases to radioembolization therapy with Yttrium-90 labeled resin microspheres. Phys Med Biol 2008; 53: pp. 6591-6603.


- 5\. Tuzel O., Yang L., Meer P., et. al.: Classification of hematologic malignancies using texton signatures. Pattern Anal Applications 2007; 10: pp. 277-290.


- 6\. Huang Y.L., Chen J.H., Shen W.C.: Diagnosis of hepatic tumors with texture analysis in nonenhanced computed tomography images. Acad Radiol 2006; 13: pp. 713-720.


- 7\. Alic L., van Vliet M., van Dijke C.F., et. al.: Heterogeneity in DCE-MRI parametric maps: a biomarker for treatment response?. Phys Med Biol 2001; 56: pp. 1601-1616.


- 8\. Miles K.A., Ganeshan B., Griffiths M.R., et. al.: Colorectal cancer: texture analysis of portal phase hepatic CT images as a potential marker of survival. Radiology 2009; 250: pp. 444-452.


- 9\. Salem R., Lewandowski R.J., Gates V.L., et. al.: Research reporting standards for radioembolization of hepatic malignancies. J Vasc Interventional Radiol 2011; 22: pp. 265-278.


- 10\. Nosher J.L., Ohman-Strickland P.A., Jabbour S., et. al.: Changes in liver and spleen volumes and liver function after radioembolization with yttrium-90 resin microspheres. J Vasc Interventional Radiol 2011; 22: pp. 1706-1713.


- 11\. Salem R., Thurston K.G.: Radioembolization with 90Yttrium microspheres: a state-of-the-art brachytherapy treatment for primary and secondary liver malignancies. Part 1: technical and methodologic considerations. J Vasc Interventional Radiol 2006; 17: pp. 1251-1278.


- 12\.  McAuliffe MJ, Lalonde FM, McGarry D, et al. Medical image processing, analysis and visualization in clinical research. IEEE Sym Computer-Based Med Systems 2001; 381–386.


- 13\.  Fang Q, Boas BA. Tetrahedral mesh generation from volumetric binary and grayscale images. IEEE Int Symp Biomed Imaging. ISBI '09. 2009; 1142–1145.


- 14\.  MATLAB, version 7.12.0 (R2011a). The MathWorks Inc., Natick, MA, 2011.


- 15\. Ganeshan B., Miles K.A., Young R.C.D., et. al.: Hepatic enhancement in colorectal cancer: texture analysis correlates with hepatic hemodynamics and patient survival. Acad Radiol 2007; 14: pp. 1520-1530.


- 16\. Sørensen L., Shaker S.B., de Bruijne M.: Texture classification in lung CT using local binary patterns. Medical Image Comp Computer-Assisted Intervention. MICCAI 2008; 11: pp. 934-941.


- 17\. Fuchs T.J., Wild P.J., Moch H., et. al.: Computational pathology analysis of tissue microarrays predicts survival of renal clear cell carcinoma patients. Med Image Comp Computer-Assisted Intervention. MICCAI 2008; 11: pp. 1-8.


- 18\. Qureshi H., Sertel O., Rajpoot N., et. al.: Adaptive discriminant wavelet packet transform and local binary patterns for meningioma subtype classification. Med Image Comp Computer-Assisted Intervention. MICCAI 2008; 11: pp. 196-204.


- 19\. Gangeh M.J., Sørensen L., Shaker S.B., et. al.: A texton-based approach for the classification of lung parenchyma in CT images. Med Image Comp Computer-Assisted Intervention. MICCAI 2010; 13: pp. 595-602.


- 20\. Leung T., Malik J.: Representing and recognizing the visual appearance of materials using three-dimensional textons. Int J Comp Vision 2001; 43: pp. 29-44.


- 21\. Goh V., Ganeshan B., Nathan P., et. al.: Assessment of response to tyrosine kinase inhibitors in metastatic renal cell cancer: CT texture as a predictive biomarker. Radiology 2011; 261: pp. 165-171.


- 22\. Ojala T., Pietikainen M., Harwood D.: A comparative study of texture measures with classification based on featured distributions. Pattern Recognit 1996; 29: pp. 51-59.


- 23\. Ojala T., Pietikainen M., Maenpaa T.: Multiresolution gray-scale and rotation invariant texture classification with local binary patterns. IEEE Trans Pattern Anal Machine Intell 2002; 24: pp. 971-987.


- 24\. Tesar L., Shimizu A., Smutek D., et. al.: Medical image analysis of 3D CT images based on extension of Haralick texture features. Comp Med Imaging Graphics 2008; 32: pp. 513-520.


- 25\. Joachims T.: Making large-scale SVM learning practical.1999.MIT PressCambridge, MA 169–184


- 26\. Tenenbaum J.B., de Silva V., Langford J.C.: A global geometric framework for nonlinear dimensionality reduction. Science 2000; 290: pp. 2319-2323.


- 27\. Roweis S.T., Saul L.K.: Nonlinear dimensionality reduction by locally linear embedding. Science 2000; 290: pp. 2323-2326.


- 28\. Coldwell D., Sangro B., Salem R., et. al.: Radioembolization in the treatment of unresectable liver tumors: experience across a range of primary cancers. Am J Clin Oncol 2012; 35: pp. 167-177.


- 29\. Yang L., Meer P., Foran D.J.: Multiple class segmentation using a unified framework over mean-shift patches. IEEE Comp Soc Conf Comp Vision Pattern Recognit (CVPR) 2007; pp. 1-8.


- 30\. Heeger D., Bergen J.: Pyramid-based texture analysis/synthesis. IEEE Intl Conf Image Processing (ICIP) 1995; 3: pp. 648-651.


- 31\. Boppudi S., Wickremesekera S.K., Nowitz M.: Evaluation of the role of CT in the assessment of response to selective internal radiation therapy in patients with colorectal liver metastases. Australas Radiol 2006; 50: pp. 570-577.