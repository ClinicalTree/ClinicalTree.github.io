---
title: Multimodality Non-rigid Image Registration for Planning, Targeting and Monitoring During CT-Guided Percutaneous Liver Tumor Cryoablation
author: [Haytham Elhawary PhD,Sota Oguro MD,Kemal Tuncali MD,Paul R. Morrison MS,Servet Tatli MD,Paul B. Shyn MD,Stuart G. Silverman MD,Nobuhiko Hata PhD]
date: 2010-11-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 17, Issue 11 SOURCE CL_S_AcademicRadiologyVolume17Issue11 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to develop non-rigid image registration between preprocedure contrast-enhanced magnetic resonance (MR) images and intraprocedure unenhanced computed tomographic (CT) images, to enhance tumor visualization and localization during CT imaging–guided liver tumor cryoablation procedures.

## Materials and Methods

A non-rigid registration technique was evaluated with different preprocessing steps and algorithm parameters and compared to a standard rigid registration approach. The Dice similarity coefficient, target registration error, 95th-percentile Hausdorff distance, and total registration time (minutes) were compared using a two-sided Student's _t_ test. The entire registration method was then applied during five CT imaging–guided liver cryoablation cases with the intraprocedural CT data transmitted directly from the CT scanner, with both accuracy and registration time evaluated.

## Results

Selected optimal parameters for registration were a section thickness of 5 mm, cropping the field of view to 66% of its original size, manual segmentation of the liver, B-spline control grid of 5 × 5 × 5, and spatial sampling of 50,000 pixels. A mean 95th-percentile Hausdorff distance of 3.3 mm (a 2.5 times improvement compared to rigid registration, _P_ < .05), a mean Dice similarity coefficient of 0.97 (a 13% increase), and a mean target registration error of 4.1 mm (a 2.7 times reduction) were measured. During the cryoablation procedure, registration between the preprocedure MR and the planning intraprocedure CT imaging took a mean time of 10.6 minutes, MR to targeting CT image took 4 minutes, and MR to monitoring CT imaging took 4.3 minutes. Mean registration accuracy was <3.4 mm.

## Conclusions

Non-rigid registration allowed improved visualization of the tumor during interventional planning, targeting, and evaluation of tumor coverage by the ice ball. Future work is focused on reducing segmentation time to make the method more clinically acceptable.

Computed tomographic (CT) imaging is used to guide percutaneous liver tumor cryoablation and has proven particularly useful when the tumor is not visible with ultrasound . CT can be used to plan the interventional approach, to facilitate the safe placement of the ablation applicators in the tumor, and to monitor the ablation effects in the case of cryoablation .

Despite the benefits of CT imaging, there can be challenges related to the lack of soft tissue contrast for liver tumors on unenhanced CT images, especially for small or poorly marginated tumors and when there are contraindications to the use of intravenous contrast material . The tumor selected for ablation and the adjacent structures at risk for injury during the procedure may be invisible or poorly visible . Suboptimal visibility can lead to improper applicator placement, resulting in inadequate ablation beyond the tumor margins or thermal injury to adjacent structures . To overcome this problem, interventional radiologists often rely on preprocedure contrast-enhanced CT imaging or magnetic resonance (MR) imaging (MRI) that depicts tumor margins and surrounding structures, including vascular anatomy. The radiologist then performs a mental correlation of the preprocedure and intraprocedure images to estimate tumor location, tumor boundaries, and adjacent anatomic structures. This can be challenging because the liver position, shape, and relation to extrahepatic structures may differ significantly between two exams.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Patient Population

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Non-rigid and Rigid Registration Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Registration Assessment Metrics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Optimization of Registration Between Preprocedural MR and Intraprocedural CT Images

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## First Optimization Stage

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Experiments Performed to Evaluate the Effects of Different Parameters and Preprocessing Steps on the Accuracy and Time of the Non-rigid Registration Method Between Preprocedure Contrast-enhanced MR and Intraprocedure Unenhanced CT Images


Parameter Set Section Thickness (mm) FOV Size Segmentation Liver Volume 1 (reference) 5 66% Yes >75% 2 3 66% Yes >75% 3 7.5 66% Yes >75% 4 5 100% Yes >75% 5 5 Liver Yes >75% 6 5 66% No >75% 7 5 66% Every 2 slices >75% 8 5 66% Yes 50%–75%

CT, computed tomographic; FOV, field of view; MR, magnetic resonance.


Parameter set 1 acts as a reference set of parameters, and the other sets are defined by modifying a single parameter value from the reference set.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Second Optimization Stage

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Experiments Performed to Evaluate the Effects of Different Algorithmic Parameters on the Accuracy and Time of the Non-rigid Registration Method Between Preprocedure Contrast-enhanced MR and Intraprocedure Unenhanced CT Images


Parameter Set Number of Control Points per Direction Sampling Pixels 1 (reference) 5 50,000 2 4 50,000 3 3 50,000 4 4 20,000 5 3 20,000 6 4 2000

CT, computed tomographic; MR, magnetic resonance.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison with Rigid Registration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Registration of Intraprocedural CT Images

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Registration between the preprocedure magnetic resonance (MR) image (MRI) and intraprocedure planning computed tomographic (CT) image results in a transformation matrix, T1, which was used to deform the preprocedure MR image on to the intraprocedure planning CT image. To register the preprocedure MR image to both the intraprocedure targeting and monitoring CT images, we registered the planning CT image to the targeting CT image, and the resulting transformation matrix, T2, was combined with T1 to deform the preprocedure MR image onto the targeting CT image. The same process can be applied to the monitoring CT image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultimodalityNonrigidImageRegistrationforPlanningTargetingandMonitoringDuringCTGuidedPercutaneousLiverTumorCryoablation/0_1s20S1076633210003090.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Registration During CT Imaging–guided Liver Tumor Ablation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Registration for Preprocedural MR to Intraprocedural CT Images

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, The graph indicates for each set of parameters ( Table 1 ) the average time taken to perform the entire registration as well as the average 95% Hausdorff distance (HD) as an indicator of accuracy. FOV, field of view; seg, segmentation; ST, section thickness.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultimodalityNonrigidImageRegistrationforPlanningTargetingandMonitoringDuringCTGuidedPercutaneousLiverTumorCryoablation/1_1s20S1076633210003090.jpg)

![Figure 3, The graph indicates for each set of design parameters related with the registration algorithm ( Table 2 ), the average computation time taken to perform the non-rigid registration, as well as the average 95% Hausdorff distance (HD) as an indicator of accuracy.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultimodalityNonrigidImageRegistrationforPlanningTargetingandMonitoringDuringCTGuidedPercutaneousLiverTumorCryoablation/2_1s20S1076633210003090.jpg)

![Figure 4, (a) Preprocedure contrast-enhanced magnetic resonance (MR) image shows 3-cm liver tumor (arrow). (b) Intraprocedure unenhanced computed tomographic (CT) image does not show the tumor. (c) Registration and fusion of the two images shows the MR-depicted tumor overlaid on the intraprocedural CT image.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultimodalityNonrigidImageRegistrationforPlanningTargetingandMonitoringDuringCTGuidedPercutaneousLiverTumorCryoablation/3_1s20S1076633210003090.jpg)

![Figure 5, Validation results for both rigid and non-rigid registration (reg) performed on nine patient images. The 95% Hausdorff distance, the Dice similarity coefficient, and the target registration error were measured in each case, showing a considerable improvement in all three metrics when using non-rigid registration compared to a rigid algorithm.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultimodalityNonrigidImageRegistrationforPlanningTargetingandMonitoringDuringCTGuidedPercutaneousLiverTumorCryoablation/4_1s20S1076633210003090.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Registration of Intraprocedural CT Images

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Average 95% HD, DSC, and Total Registration Time Measured for the Two Liver Registration Methods for Five Patient Data Sets


Method 1 Method 2 Registered Images 95% HD (mm) DSC Time (min) 95% HD (mm) DSC Time (min) MR to planning CT images 3.29 0.97 19.2 3.29 0.97 19.2 MR to targeting CT images 3.9 0.94 10.2 3.5 0.96 4.6 MR to monitoring CT images 3.9 0.93 10.4 4 0.96 4.3

CT, computed tomographic; DSC, Dice similarity coefficient; HD, Hausdorff distance; MR, magnetic resonance.


Method 1 was a direct registration of preprocedure MR to intraprocedure CT images, while method 2 used the transformation obtained from CT-to-CT registration to deform and register the MR image.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Registration During CT Imaging–guided Liver Tumor Ablation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, (a) Preprocedure, contrast-enhanced axial magnetic resonance (MR) image obtained with patient in supine position shows tumor (arrow) as hypointense region. (b) Intraprocedure computed tomographic (CT) image for interventional planning obtained with the patient in a left posterior oblique position. (c) Registered and fused image shows liver tumor (arrow) from registered MR image overlaid on planning CT image. (d) Targeting CT image shows cryoablation applicators (arrows) in position, overlaid with segmented tumor from the registered MR image. (e) CT image shows the ice ball as hypointense area around the tumor (white arrows) overlaid with segmented tumor from registered MR image. (f) Three-dimensional representation of liver, tumor, ice ball, and cryoablation applicators to evaluate tumor coverage and margins.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultimodalityNonrigidImageRegistrationforPlanningTargetingandMonitoringDuringCTGuidedPercutaneousLiverTumorCryoablation/5_1s20S1076633210003090.jpg)

![Figure 7, The average time for registration and 95% Hausdorff distance (HD) measured for non-rigid registration performed during computed tomographic (CT) imaging–guided percutaneous liver tumor ablation. Registration was performed for preprocedure magnetic resonance (MR) and intraprocedure planning CT images, for MR and targeting CT images, and for MR and monitoring CT images acquired during the intervention. A standard deviation is also expressed around the average for each measured metric.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultimodalityNonrigidImageRegistrationforPlanningTargetingandMonitoringDuringCTGuidedPercutaneousLiverTumorCryoablation/6_1s20S1076633210003090.jpg)

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

## References

- 1\. Antoch G., Kuehl H., Vogt F.M., et. al.: Value of CT volume imaging for optimal placement of radiofrequency ablation probes in liver lesions. J Vasc Interv Radiol 2002; 13: pp. 1155-1161.


- 2\. Jakobs T.F., Hoffmann R.T., Schrader A., et. al.: CT-guided radiofrequency ablation in patients with hepatic metastases from breast cancer. Cardiovasc Intervent Radiol 2009; 32: pp. 38-46.


- 3\. Kuehl H., Stattaus J., Forsting M., et. al.: Transhepatic CT-guided radiofrequency ablation of adrenal metastases from hepatocellular carcinoma. Cardiovasc Intervent Radiol 2008; 31: pp. 1210-1214.


- 4\. Ohmoto K., Mimura N., Iguchi Y., et. al.: CT-guided percutaneous ethanol injection therapy for ultrasonically invisible hepatocellular carcinoma. Hepatogastroenterology 2002; 49: pp. 297-299.


- 5\. Sato M., Watanabe Y., Tokui K., et. al.: CT-guided treatment of ultrasonically invisible hepatocellular carcinoma. Am J Gastroenterol 2000; 95: pp. 2102-2106.


- 6\. Shankar S., Bhargava P., Habib F., et. al.: Transpulmonary CT-guided radiofrequency ablation of liver metastasis. Cardiovasc Intervent Radiol 2005; 28: pp. 481-484.


- 7\. Shankar S., Tuncali K., vanSonnenberg E., et. al.: Myoglobinemia after CT-guided radiofrequency ablation of a hepatic metastasis. AJR Am J Roentgenol 2002; 178: pp. 359-361.


- 8\. Park B.J., Byun J.H., Jin Y.H., et. al.: CT-guided radiofrequency ablation for hepatocellular carcinomas that were undetectable at US: therapeutic effectiveness and safety. J Vasc Interv Radiol 2009; 20: pp. 490-499.


- 9\. Silverman S.G., Tuncali K., Morrison P.R.: MR imaging-guided percutaneous tumor ablation. Acad Radiol 2005; 12: pp. 1100-1109.


- 10\. Clasen S., Pereira P.L.: Magnetic resonance guidance for radiofrequency ablation of liver tumors. J Magn Reson Imaging 2008; 27: pp. 421-433.


- 11\. Lu D.S., Raman S.S., Vodopich D.J., et. al.: Effect of vessel size on creation of hepatic radiofrequency lesions in pigs: assessment of the “heat sink” effect. AJR Am J Roentgenol 2002; 178: pp. 47-51.


- 12\. Goldberg S.N., Hahn P.F., Tanabe K.K., et. al.: Percutaneous radiofrequency tissue ablation: does perfusion-mediated tissue cooling limit coagulation necrosis?. J Vasc Interv Radiol 1998; 9: pp. 101-111.


- 13\. Mahnken A.H., Buecker A., Spuentrup E., et. al.: MR-guided radiofrequency ablation of hepatic malignancies at 1.5 T: initial results. J Magn Reson Imaging 2004; 19: pp. 342-348.


- 14\. Livraghi T., Solbiati L., Meloni M.F., et. al.: Treatment of focal liver tumors with percutaneous radio-frequency ablation: complications encountered in a multicenter study. Radiology 2003; 226: pp. 441-451.


- 15\. Crum W.R., Hartkens T., Hill D.L.G.: Non-rigid image registration: theory and practice. Br J Radiol 2004; 77: pp. S140-S153.


- 16\. Hill D.L.G., Batchelor P.G., Holden M., et. al.: Medical image registration. Phys Med Biol 2001; 46: pp. R1-R45.


- 17\. Carrillo A., Duerk J.L., Lewin J.S., et. al.: Semiautomatic 3-D image registration as applied to interventional MRI liver cancer treatment. IEEE Trans Med Imaging 2000; 19: pp. 175-185.


- 18\. Wilson D.L., Carrillo A., Zheng L., et. al.: Evaluation of 3D image registration as applied to MR-guided thermal treatment of liver cancer. J Magn Reson Imaging 1998; 8: pp. 77-84.


- 19\. Penney G.P., Blackall J.M., Hamady M.S., et. al.: Registration of freehand 3D ultrasound and magnetic resonance liver images. Med Image Anal 2004; 8: pp. 81-91.


- 20\. Archip N., Tatli S., Morrison P., et. al.: non-rigid registration of pre-procedural MR images with intra-procedural unenhanced CT images for improved targeting of tumors during liver radiofrequency ablations. Med Image Comput Computer-Assist Interv 2007; pp. 969-977.


- 21\.  Niculescu G, Forand DJ, Nosher J. Non-rigid registration of the liver in consecutive CT studies for assessment of tumor response to radiofrequency ablation. Presented at: Engineering in Medicine and Biology Society: 29th Annual International Conference of the IEEE; 2007.


- 22\.  Yen-Wei C, Katsumi T, Rui X, et-al. Semiautomatic non-rigid 3-D image registration for MR-guided liver cancer surgery. Presented at: 15th IEEE International Conference on Image Processing; 2008.


- 23\. Lange T., Wenckebach T.H., Lamecker H., et. al.: Registration of different phases of contrast-enhanced CT/MRI data for computer-assisted liver surgery planning: Evaluation of state-of-the-art methods. Int J Med Robot Comput Assist Surg 2005; 1: pp. 6-20.


- 24\. Rohlfing T., Maurer C.R., O'Dell W.G., et. al.: Modeling liver motion and deformation during the respiratory cycle using intensity-based nonrigid registration of gated MR images. Med Phys 2004; 31: pp. 427-432.


- 25\. Archip N., Clatz O., Whalen S., et. al.: Non-rigid alignment of pre-operative MRI, fMRI, and DT-MRI with intra-operative MRI for enhanced visualization and navigation in image-guided neurosurgery. Neuroimage 2007; 35: pp. 609-624.


- 26\. Rueckert D., Sonoda L.I., Hayes C., et. al.: Nonrigid registration using free-form deformations: application to breast MR images. IEEE Trans Med Imaging 1999; 18: pp. 712-721.


- 27\. Wells W., Viola P., Atsumi H., et. al.: Multi-modal volume registration by maximization of mutual information. Med Image Anal 1996; 1: pp. 35-51.


- 28\. Gering D.T., Nabavi A., Kikinis R., et. al.: An integrated visualization system for surgical planning and guidance using image fusion and an open MR. J Magn Reson Imaging 2001; 13: pp. 967-975.


- 29\. Hausdorff F.: Set Theory.2nd ed.1962.Chelsea Publication CompanyLondon


- 30\. Canny J.: A computational approach to edge detection. IEEE Trans Patt Anal Mach Intell 1986; 8: pp. 679-698.


- 31\. Bharatha A., Hirose M., Hata N., et. al.: Evaluation of three-dimensional finite element-based deformable registration of pre- and intraoperative prostate imaging. Med Phys 2001; 28: pp. 2551-2560.


- 32\. Zou K.H., Warfield S.K., Bharatha A., et. al.: Statistical validation of image segmentation quality based on a spatial overlap index: scientific reports. Acad Radiol 2004; 11: pp. 178-189.


- 33\.  Morten B-N, Claus G. Fast fluid registration of medical images. Presented at: 4th International Conference on Visualization in Biomedical Computing; 1996.


- 34\. Studholme C., Hill D.L.G., Hawkes D.J.: An overlap invariant entropy measure of 3D medical image alignment. Patt Recog 1999; 32: pp. 71-86.


- 35\. Thirion J.P.: Image matching as a diffusion process: an analogy with Maxwell's demons. Med Image Anal 1998; 2: pp. 243-260.


- 36\. Lange T., Eulenstein S., Hunerbein M., et. al.: Vessel-based non-rigid registration of MR/CT and 3D ultrasound for navigation in liver surgery. Comput Aided Surg 2003; 8: pp. 228-240.


- 37\. Heimann T., van Ginneken B., Styner M.A., et. al.: Comparison and evaluation of methods for liver segmentation from CT datasets. IEEE Trans Med Imaging 2009; 28: pp. 1251-1265.


- 38\.  Gholipour A, Kehtarnavaz ND. Computationally efficient mutual information estimation for non-rigid image registration. Presented at: IEEE International Conference of Image Processing; 2008.


- 39\. Klein S., Staring M., Pluim J.P.W.: Evaluation of optimization methods for nonrigid medical image registration using mutual information and B-splines. IEEE Trans Image Process 2007; 16: pp. 2879-2890.


- 40\. Maes F., Vandermeulen D., Suetens P.: Comparative evaluation of multiresolution optimization strategies for multimodality image registration by maximization of mutual information. Med Image Anal 1999; 3: pp. 373-386.