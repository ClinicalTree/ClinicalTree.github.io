---
title: 3D Registration of mpMRI for Assessment of Prostate Cancer Focal Therapy
author: [Clément Orczyk MSc MD,Andrew B. Rosenkrantz MD,Artem Mikheev MSc,Arnauld Villers MD PhD,Myriam Bernaudin PhD,Samir S. Taneja MD,Samuel Valable PhD,Henry Rusinek PhD]
date: 2017-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 24, Issue 12 SOURCE CL_S_AcademicRadiologyVolume24Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

This study aimed to assess a novel method of three-dimensional (3D) co-registration of prostate magnetic resonance imaging (MRI) examinations performed before and after prostate cancer focal therapy.

## Materials and Methods

We developed a software platform for automatic 3D deformable co-registration of prostate MRI at different time points and applied this method to 10 patients who underwent focal ablative therapy. MRI examinations were performed preoperatively, as well as 1 week and 6 months post treatment. Rigid registration served as reference for assessing co-registration accuracy and precision.

## Results

Segmentation of preoperative and postoperative prostate revealed a significant postoperative volume decrease of the gland that averaged 6.49 cc ( _P_ = .017). Applying deformable transformation based on mutual information from 120 pairs of MRI slices, we refined by 2.9 mm (max. 6.25 mm) the alignment of the ablation zone, segmented from contrast-enhanced images on the 1-week postoperative examination, to the 6-month postoperative T2-weighted images. This represented a 500% improvement over the rigid approach ( _P_ = .001), corrected by volume. The dissimilarity by Dice index of the mapped ablation zone using deformable transformation vs rigid control was significantly ( _P_ = .04) higher at the ablation site than in the whole gland.

## Conclusions

Our findings illustrate our method's ability to correct for deformation at the ablation site. The preliminary analysis suggests that deformable transformation computed from mutual information of preoperative and follow-up MRI is accurate in co-registration of MRI examinations performed before and after focal therapy. The ability to localize the previously ablated tissue in 3D space may improve targeting for image-guided follow-up biopsy within focal therapy protocols.

## Introduction

Contemporary methods of multiparametric magnetic resonance imaging (mpMRI) of the prostate have greatly improved the ability of radiologists and urologists to detect prostate cancer . mpMRI allows physicians to diagnose clinically significant cancer in its early stage, to plan prostatectomy and radiation therapy, and to detect local recurrence.

Combined with the trend of earlier detection, noninvasive prostate cancer therapies are gaining interest. Focal therapies (FT) aim to combine oncologic benefit with preserved continence and erectile function. The use of this tissue-preservation approach is evolving, and FT are being applied to more aggressive disease than when initially proposed . Clinical FT trials depend on mpMRI for tumor localization, treatment planning, and posttreatment follow-up .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

## Patients

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Timeline of treatment and imaging examinations.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/0_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Image analysis workflow.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/1_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Co-registration Framework

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (1)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (2)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The dialog box defines the registration process.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/2_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimating Transformations Within Examination and Across Examinations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Error Analysis and Segmentation of Prostate Gland and Ablation Zone

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Illustrative case of affine registration between pretreatment (a) and posttreatment (photodynamic therapy) T2-weighted (T2W) volumes (c) . Panel (b) shows delayed dynamic contrast-enhanced (DCE) image of the treated area, with ablated gland shown as nonenhancing region. The bottom panel displays a postoperative T2W image overlayed with the corresponding preoperative image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/3_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Schematic illustration of various measures assessed in the current study. (a) Analysis of errors in whole-gland definition for rigid transform model M 2 vs M 2 ″; (b) analysis of errors for affine transform model M 2 vs M 2 ′; and (c) analysis of errors in defining AZ (AZ 2′ -AZ 2″ ) vs (M 2 ′-M 2 ″).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/4_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (1)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (2)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (3)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Volumetric Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 1


Distribution of Prostate Volumes Estimated from T2W Images Acquired Before and After Ablation (Late Control) and Distribution of Volume of Ablated Zone (AZ)


Prostate Volume From T2W Images Ablated Volume (cc) From DCE MRI Initial Volume (cc) Postablation Volume (cc) Difference D (cc) Median 51.64 46.73 6.70 7.88 Mean 46.49 39.99 6.50 13.82 SD 23.67 20.25 7.05 13.67 Min 8.42 6.80 −3.60 1.07 Max 87.16 65.52 21.64 37.35

DCE, dynamic contrast-enhanced; SD, standard deviation; T2W, T2-weighted.


![Figure 6, Comparison between median preoperative and 6-month postoperative volumes of the prostate (orange bars). Comparison between median volume generated with rigid and nonrigid transforms (blue bars) shows that nonrigid transformation compensates better for volume loss due to focal therapy. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/5_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Analysis of Image Co-registration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Demonstration of high central processing unit core usage on a 12-core computer achieved during registration.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/6_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 2


Comparison of Volumes Between Original T2WI and Their Transform Using Rigid and Deformable Methods


Transformed Volumes Rigid Preop Transform Volume (cc) Deformable Preop Transform Volume (cc) Median 50.71 48.22 Mean 45.41 43.23 SD 22.81 21.17 Min 7.99 7.17 Max 81.02 73.67

SD, standard deviation; T2W, T2-weighted image.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 3


Alignment Between Whole Gland Obtained by Mapping From Preoperative to Postoperative T2W Image and Whole Gland Traced Directly on Postoperative Image: Comparison Between Rigid and Affine Co-registrations


Rigid Registration _Tr_ Affine Registration _Ta_ Hausdorff Distance (mm) Median 7.73 7.29 Mean 8.14 6.91 Max 9.46 9.98 Min 5.31 4.64 SD 1.45 1.60_P_ value_P_ = .20

Dice Index Mean 0.82 0.84 Median 0.85 0.85 Max 0.91 0.92 Min 0.68 0.72 SD 0.08 0.06_P_ value_P_ = .10

SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Analysis of AZ

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 4


Compensation of the Local Deformation by Affine Algorithm: Comparison Between Mapping Accuracy of the Location of the Ablated Zone and the Whole Gland, Referring to Measures Shown in  Figure 5c

_Ta_ (AZ) vs _Tr_ (AZ)_Ta_ (M) vs _Tr_ (M) Hausdorff Distance (mm) Median 1.99 3.83 Mean 2.99 3.84 Max 6.25 7.05 Min 1.10 1.10 SD 2.10 2.21

Normalized Hausdorff distance (mm/mL) Mean 0.72 0.15 Median 0.22 0.09 Max 1.09 0.55 Min 0.05 0.03 SD 0.57 0.17_P_ value_**P**_ **=** **.0019**

Dice Index Mean 0.87 0.93 Median 0.87 0.92 Max 0.96 0.98 Min 0.59 0.88 SD 0.11 0.04_P_ value_**P**_ **=** **.046**

SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Postsurgical changes for a representative case involving dynamic phototherapy on the left lobe. (a,b) Three-dimensional (3D) rendering before and after treatment. Changes in shape and volume loss are observed in the left part of the gland. The pretreatment view shows in red the lesion 10 mm in axial diameter, Gleason 6 (3 + 3). The posttreatment view displays in yellow the location of the ablated zone. This yellow area needs to be sampled to rule out cancer at follow-up biopsy. The green line segment is the needle path for transperineal targeted biopsy. (c) Preoperative T2-weighted (T2W) image. (d) Preoperative apparent diffusion coefficient (ADC) map. (e) Preoperative dynamic contrast-enhanced (DCE) image through the cancer focus (white arrow). (f) Late postoperative T2W image. (g) Postoperative ADC map. (h) DCE image at the same level. Changes in shape and magnetic resonance imaging (MRI) signal are discernible at the site of ablation on the left side of the gland. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/7_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

## The Role of Image Registration in Prostate Cancer Pathway

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Challenge for Image Registration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Posttreatment Volume Loss

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Co-registration Accuracy

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Limitations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Implications

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Graphical summary of implementation of three-dimensional (3D) registration of multiparametric magnetic resonance imaging (mpMRI) into focal therapy of prostate cancer pathway. Overlays of the prostate segmentation are presented on the extreme right MRI image with the green line as the postablation segmentation, the blue the preoperative registered prostate using the nonrigid transformation, and the orange using the rigid registration. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/3DRegistrationofmpMRIforAssessmentofProstateCancerFocalTherapy/8_1s20S107663321730301X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Dickinson L., Ahmed H.U., Allen C., et. al.: Magnetic resonance imaging for the detection, localisation, and characterisation of prostate cancer: recommendations from a European consensus meeting. Eur Urol 2011; 59: pp. 477-494.


- 2\. Orczyk C., Emberton M., Ahmed H.U.: What tumours should we treat with focal therapy based on risk category, grade, size and location?. Curr Opin Urol 2015; 25: pp. 212-219.


- 3\. Donaldson I.A., Alonzi R., Barratt D., et. al.: Focal therapy: patients, interventions, and outcomes—a report from a consensus meeting. Eur Urol 2015; 67: pp. 771-777.


- 4\. Oto A., Sethi I., Karczmar G., et. al.: MR imaging-guided focal laser ablation for prostate cancer: phase I trial. Radiology 2013; 267: pp. 932-940.


- 5\. van den Bos W., Muller B.G., Ahmed H., et. al.: Focal therapy in prostate cancer: international multidisciplinary consensus on trial design. Eur Urol 2014; 65: pp. 1078-1083.


- 6\. Le Nobin J., Orczyk C., Deng F.-M., et. al.: Prostate tumour volumes: evaluation of the agreement between magnetic resonance imaging and histology using novel co-registration software: prostate tumour volume: co-registration between MRI and pathology. BJU Int 2014; 114: pp. E105-E112.


- 7\. Le Nobin J., Rosenkrantz A.B., Villers A., et. al.: Image guided focal therapy for magnetic resonance imaging visible prostate cancer: defining a 3-dimensional treatment margin based on magnetic resonance imaging histology co-registration analysis. J Urol 2015; 194: pp. 364-370.


- 8\. Muller B.G., van den Bos W., Brausi M., et. al.: Follow-up modalities in focal therapy for prostate cancer: results from a Delphi consensus project. World J Urol 2015; 33: pp. 1503-1509. Available at http://link.springer.com/10.1007/s00345-014-1475-2

- 9\. Rosenkrantz A.B., Taneja S.S.: Targeted prostate biopsy: opportunities and challenges in the era of multiparametric prostate magnetic resonance imaging. J Urol 2012; 188: pp. 1072-1073.


- 10\. Wysock J.S., Rosenkrantz A.B., Huang W.C., et. al.: A prospective, blinded comparison of magnetic resonance (MR) imaging-ultrasound fusion and visual estimation in the performance of MR-targeted prostate biopsy: the PROFUS trial. Eur Urol 2014; 66: pp. 343-351.


- 11\. Lindner U., Lawrentschuk N., Weersink R.A., et. al.: Focal laser ablation for prostate cancer followed by radical prostatectomy: validation of focal therapy and imaging accuracy. Eur Urol 2010; 57: pp. 1111-1114.


- 12\. Huang Z., Haider M.A., Kraft S., et. al.: Magnetic resonance imaging correlated with the histopathological effect of Pd-bacteriopheophorbide (Tookad) photodynamic therapy on the normal canine prostate gland. Lasers Surg Med 2006; 38: pp. 672-681.


- 13\. Bratan F., Melodelima C., Souchon R., et. al.: How accurate is multiparametric MR imaging in evaluation of prostate cancer volume?. Radiology 2014; 140524


- 14\. Rouvière O., Gelet A., Crouzet S., et. al.: Prostate focused ultrasound focal therapy—imaging for the future. Nat Rev Clin Oncol 2012; 9: pp. 721-727.


- 15\. Fei B., Wheaton A., Lee Z., et. al.: Automatic MR volume registration and its evaluation for the pelvis and prostate. Phys Med Biol 2002; 47: pp. 823-838.


- 16\. Wu X., Dibiase S.J., Gullapalli R., et. al.: Deformable image registration for the use of magnetic resonance spectroscopy in prostate treatment planning. Int J Radiat Oncol Biol Phys 2004; 58: pp. 1577-1583.


- 17\. Marami B., Sirouspour S., Ghoul S., et. al.: Elastic registration of prostate MR images based on estimation of deformation states. Med Image Anal 2015; 21: pp. 87-103.


- 18\. Toth R., Sperling D., Madabhushi A.: Quantifying post-laser ablation prostate therapy changes on MRI via a domain-specific biomechanical model: preliminary findings. PLoS ONE 2016; 11: pp. e0150016.


- 19\. Orczyk C., Rusinek H., Rosenkrantz A.B., et. al.: Preliminary experience with a novel method of three-dimensional co-registration of prostate cancer digital histology and in vivo multiparametric MRI. Clin Radiol 2013; 68: pp. e652-e658.


- 20\. Taneja S.S., Bennett J., Coleman J., et. al.: Final results of a phase I/II multicenter trial of WST11 (TOOKAD® Soluble) vascular-targeted photodynamic therapy (VTP) for hemiablation of the prostate in men with unilateral low risk prostate cancer conducted in the United States. J Urol 2016; 196: pp. 1096-1104.


- 21\. Lagarias J., Reeds J., Wright M., et. al.: Convergence properties of the Nelder–Mead simplex method in low dimensions. SIAM J Optim 1998; 9: pp. 112-147.


- 22\. Hajnal J.V., Saeed N., Oatridge A., et. al.: Detection of subtle brain changes using subvoxel registration and subtraction of serial MR images. J Comput Assist Tomogr 1995; 19: pp. 677-691.


- 23\. Lemieux L., Wieshmann U.C., Moran N.F., et. al.: The detection and significance of subtle changes in mixed-signal brain lesions by serial MRI scan matching and spatial normalization. Med Image Anal 1998; 2: pp. 227-242.


- 24\. Woods R.P., Grafton S.T., Holmes C.J., et. al.: Automated image registration: I. General methods and intrasubject, intramodality validation. J Comput Assist Tomogr 1998; 22: pp. 139-152.


- 25\. Woods R.P., Grafton S.T., Watson J.D., et. al.: Automated image registration: II. Intersubject validation of linear and nonlinear models. J Comput Assist Tomogr 1998; 22: pp. 153-165.


- 26\. Collignon A., Maes F., Delaere D., et. al.: Automated multi-modality image registration based on information theory.Bizais.1995.


- 27\. Maes F., Collignon A., Vandermeulen D., et. al.: Multimodality image registration by maximization of mutual information. IEEE Trans Med Imaging 1997; 16: pp. 187-198.


- 28\. Viola P., Wells W.M.: Alignment by maximization of mutual information.Fifth international conference on computer vision, 1995. Proceedings.1995.pp. 16-23.


- 29\. Wells W.M., Viola P., Atsumi H., et. al.: Multi-modal volume registration by maximization of mutual information. Med Image Anal 1996; 1: pp. 35-51.


- 30\. James A.P., Dasarathy B.V.: Medical image fusion: a survey of the state of the art. Inf Fusion 2014; 19: pp. 4-19.


- 31\. Park B., Mikheev A., Zaim Wadghiri Y., et. al.: Optimal target VOI size for accurate 4D coregistration of DCE-MRI2016. Available at http://dx.doi.org/10.1117/12.2214675 97881P–97881P–8


- 32\. Gibson E., Crukley C., Gaed M., et. al.: Registration of prostate histology images to ex vivo MR images via strand-shaped fiducials. J Magn Reson Imaging 2012; 36: pp. 1402-1412.


- 33\. Patel P., Chappelow J., Tomaszewski J., et. al.: Spatially weighted mutual information (SWMI) for registration of digitally reconstructed ex vivo whole mount histology and in vivo prostate MRI.IEEE.2011.pp. 6269-6272. Available at http://ieeexplore.ieee.org.ezproxy.med.nyu.edu/xpls/abs\_all.jsp?arnumber=6091547&tag=1

- 34\. Hawkes D.J., Barratt D., Blackall J.M., et. al.: Tissue deformation and shape models in image-guided interventions: a discussion paper. Med Image Anal 2005; 9: pp. 163-175.


- 35\. Hu Y., Carter T., Ahmed H., et. al.: Modelling prostate motion for data fusion during image-guided interventions. IEEE Trans Med Imaging 2011; 30: pp. 1887-1900. Available at http://www.ncbi.nlm.nih.gov/pubmed/21632296

- 36\. Hu Y., Morgan D., Ahmed H.U., et. al.: A statistical motion model based on biomechanical simulations for data fusion during image-guided prostate interventions. Med Image Comput Comput Assist Interv 2008; 11: pp. 737-744.


- 37\. Mitra J., Kato Z., Martí R., et. al.: A spline-based non-linear diffeomorphism for multimodal prostate registration. Med Image Anal 2012; 16: pp. 1259-1279.


- 38\. Rouvière O., Glas L., Girouin N., et. al.: Prostate cancer ablation with transrectal high-intensity focused ultrasound: assessment of tissue destruction with contrast-enhanced US. Radiology 2011; 259: pp. 583-591.


- 39\. Barret E., Harvey-Bryan K.-A., Sanchez-Salas R., et. al.: How to diagnose and treat focal therapy failure and recurrence?. Curr Opin Urol 2014; 24: pp. 241-246.


- 40\. Muller B.G., van den Bos W., Pinto P.A., et. al.: Imaging modalities in focal therapy: patient selection, treatment guidance, and follow-up. Curr Opin Urol 2014; 24: pp. 218-224.


- 41\. Muller B.G., Fütterer J.J., Gupta R.T., et. al.: The role of magnetic resonance imaging (MRI) in focal therapy for prostate cancer: recommendations from a consensus panel: role of MRI in focal therapy for prostate cancer. BJU Int 2014; 113: pp. 218-227.


- 42\. De Visschere P.J., De Meerleer G.O., Fütterer J.J., et. al.: Role of MRI in follow-up after focal therapy for prostate carcinoma. AJR Am J Roentgenol 2010; 194: pp. 1427-1433.


- 43\. Del Vescovo R., Pisanti F., Russo V., et. al.: Dynamic contrast-enhanced MR evaluation of prostate cancer before and after endorectal high-intensity focused ultrasound. Radiol Med 2013; 118: pp. 851-862.


- 44\. Ven W.J.M., Hulsbergen-van de Kaa C.A., Hambrock T., et. al.: Simulated required accuracy of image registration tools for targeting high-grade cancer components with prostate biopsies. Eur Radiol 2012; 23: pp. 1401-1407.


- 45\. Shah T.T., Kasivisvanathan V., Jameson C., et. al.: Histological outcomes after focal high-intensity focused ultrasound and cryotherapy. World J Urol 2015; pp. 1-10.


- 46\. Chappelow J., Madabhushi A.: Multi-attribute combined mutual information (MACMI): an image registration framework for leveraging multiple data channels.2010 IEEE international symposium on biomedical imaging: from nano to macro.2010.IEEEpp. 376-379.


- 47\. Fei B., Lee Z., Boll D.T., et. al.: Image registration and fusion for interventional MRI guided thermal ablation of the prostate cancer.Medical image computing and computer-assisted intervention—MICCAI 2003.2003.SpringerBerlin, Heidelberg:pp. 364-372. Available at https://link.springer.com/chapter/10.1007/978-3-540-39903-2\_45

- 48\. Gerig G., Fishbaugh J., Sadeghi N.: Longitudinal modeling of appearance and shape and its potential for clinical use. Med Image Anal 2016; 33: pp. 114-121.


- 49\. Mozer P., Baumann M., Chevreau G., et. al.: Mapping of transrectal ultrasonographic prostate biopsies: quality control and learning curve assessment by image processing. J Ultrasound Med 2009; 28: pp. 455-460.


- 50\. Engelhard K., Kühn R., Osten A., et. al.: Impact of magnetic resonance imaging-guided prostate biopsy in the supine position on the detection of significant prostate cancer in an inhomogeneous patient cohort. Scand J Urol 2016; 50: pp. 110-115.


- 51\. Ukimura O., Gross M.E., de Castro Abreu A.L., et. al.: A novel technique using three-dimensionally documented biopsy mapping allows precise re-visiting of prostate cancer foci with serial surveillance of cell cycle progression gene panel: re-visiting biopsy from known prostate cancer. Prostate 2015; 75: pp. 863-871.


- 52\. Ghai S., Trachtenberg J.: Prostate cancer: a consensus on trial design for focal therapy. Nat Rev Urol 2014; 11: pp. 190-192.


- 53\. Natarajan S., Raman S., Priester A.M., et. al.: Focal laser ablation of prostate cancer: phase I clinical trial. J Urol 2016; 196: pp. 68-75.


- 54\. Lencioni R., de Baere T., Martin R.C., et. al.: Image-guided ablation of malignant liver tumors: recommendations for clinical validation of novel thermal and non-thermal technologies—a western perspective. Liver Cancer 2015; 4: pp. 208-214.


- 55\. Singla N., Gahan J.: New technologies in tumor ablation. Curr Opin Urol 2016; 26: pp. 248-253.