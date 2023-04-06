---
title: Automated T2-mapping of the Menisci From Magnetic Resonance Images in Patients with Acute Knee Injury
author: [Anthony Paproki PhD,Craig Engstrom PhD,Mark Strudwick PhD,Katharine J. Wilson MSc,Rachel K. Surowiec MSc,Charles Ho PhD,Stuart Crozier PhD,Jurgen Fripp PhD]
date: 2017-10-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 24, Issue 10 SOURCE CL_S_AcademicRadiologyVolume24Issue10 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

This study aimed to evaluate the accuracy of an automated method for segmentation and T2 mapping of the medial meniscus (MM) and lateral meniscus (LM) in clinical magnetic resonance images from patients with acute knee injury.

## Materials and Methods

Eighty patients scheduled for surgery of an anterior cruciate ligament or meniscal injury underwent magnetic resonance imaging of the knee (multiplanar two-dimensional \[2D\] turbo spin echo \[TSE\] or three-dimensional \[3D\]-TSE examinations, T2 mapping). Each meniscus was automatically segmented from the 2D-TSE (composite volume) or 3D-TSE images, auto-partitioned into anterior, mid, and posterior regions, and co-registered onto the T2 maps. The Dice similarity index (spatial overlap) was calculated between automated and manual segmentations of 2D-TSE (15 patients), 3D-TSE (16 patients), and corresponding T2 maps (31 patients). Pearson and intraclass correlation coefficients (ICC) were calculated between automated and manual T2 values. T2 values were compared (Wilcoxon rank sum tests) between torn and non-torn menisci for the subset of patients with both manual and automated segmentations to compare statistical outcomes of both methods.

## Results

The Dice similarity index values for the 2D-TSE, 3D-TSE, and T2 map volumes, respectively, were 76.4%, 84.3%, and 75.2% for the MM and 76.4%, 85.1%, and 76.1% for the LM. There were strong correlations between automated and manual T2 values (r  MM = 0.95, ICC  MM = 0.94; r  LM = 0.97, ICC  LM = 0.97). For both the manual and the automated methods, T2 values were significantly higher in torn than in non-torn MM for the full meniscus and its subregions ( _P_ < .05). Non-torn LM had higher T2 values than non-torn MM ( _P_ < .05).

## Conclusions

The present automated method offers a promising alternative to manual T2 mapping analyses of the menisci and a considerable advance for integration into clinical workflows.

## Introduction

Meniscal degeneration, by altering normal knee function and loading mechanisms, has been identified as a strong determinant within the multifactorial etiology of knee osteoarthritis (OA) , and overall healthy and properly functioning menisci are paramount to the long-term health of the knee joint . These cartilaginous structures can be altered acutely via trauma or chronically through degenerative processes commonly found in knee OA or secondary to anterior cruciate ligament (ACL) injuries . Direct injuries often result in visible morphological alterations; however, such changes may not be obvious in the early stages of degenerative processes where biochemical alterations occur first . In both cases, quantitative magnetic resonance (MR) imaging of the meniscus could be useful for accurate diagnosis, surgery planning and follow-up, and for the early detection of degeneration not resulting in macroscopic tissue damage .

The acquisition of multiple multiplanar two-dimensional (2D) turbo spin echo (TSE) MR images is the standard clinical MR protocol for noninvasive assessment of the menisci. In research studies, three-dimensional \[3D\]-TSE and T2 mapping MR imaging have been shown to provide enhanced morphological and biochemical assessment of soft tissue structures including the menisci . In both cases, the identification of the menisci volume in the images remains challenging and a major obstacle to clinical integration of quantitative MR imaging. Subjective manual or semiautomated segmentations are currently the primary means to analyze the structures in the MR images. These methods are time- and expertise-intensive and associated with variable intra-rater and inter-rater reliability for subsequent measurements , hence limiting their utility in clinical workflows.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

## Study Population

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## MR Imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 1


Acquisition Parameters for Each MR Sequence


2D-TSE ( _n_ = 37) 3D-TSE ( _n_ = 43) T2 Map ( _n_ = 80) Plane SAG-COR-AX SAG SAG TR (ms) 5590 1200 2570ss TE(s) (ms) 40 45 13.8/27.6/41.4/55.2/69/82.8/96.6 Flip angle (°) 120 120 180 In plane (mm) 0.188 × 0.188 0.586 × 0.586 0.546 × 0.546 Thickness (mm) 3 0.699 2 Slice gap (mm) 0–0.3 — 2.0 FOV (mm) 120 150 140 Number of slices 30–33 176 25 Bandwidth (Hz/Px) 260 425 300 Acq. time (min) 1:54-3:13 5:35 6:55 Number of images 1 1 7

2D, two-dimensional; 3D, three-dimensional; FOV, field of view; MR, magnetic resonance; TE, echo time; TR, repetition time; TSE, turbo spin echo.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Manual Image Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Automated Image Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Flow diagram illustrating the segmentation and T2 analysis pipeline.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedT2mappingoftheMenisciFromMagneticResonanceImagesinPatientswithAcuteKneeInjury/0_1s20S1076633217302088.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## MR Image Preprocessing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Illustration of the preprocessing performed for the 2D-TSE MRI. (a) Initial sagittal MRI visualized in the coronal plane (0.19 × 0.19 × 3.3 mm). (b) Example of standard resolution up-sampling using b-spline interpolation (0.31 × 0.31 × 0.69 mm). (c) Composite image resulting from the super-resolution scheme used to improve the spatial resolution and tissue delineation of the meniscus in the MR image (0.31 × 0.31 × 0.69 mm). 2D, two-dimensional; MRI, magnetic resonance imaging; TSE, turbo spin echo.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedT2mappingoftheMenisciFromMagneticResonanceImagesinPatientswithAcuteKneeInjury/1_1s20S1076633217302088.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Meniscus Partitioning

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Co-registration to T2 maps

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quality Control

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analyses

## Segmentation Validation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

DSI(A,M)=100∗2\|A∩M\|\|A\|+\|M\|
D

S

I

(

A

,

M

)

=

100

∗

2

\|

A

∩

M

\|

\|

A

\|

+

\|

M

\|


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## T2 Map Analyses

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Segmentation Performance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 2


Validation of the Accuracy of the Method Using the DSI, Mean Absolute Surface Distance (MASD) Between Automated and Manual Surfaces and Pearson (r  T2  ), and Intraclass (ICC  T2  ) Correlations between the T2 Means Estimated From the Automated (\*.A) and Manual Segmentations (\*.M)


_N_ DSI (%) MASD (mm) T2.M (ms) T2.A (ms) r  T2  ; ICC  T2  2D-TSE MRI MM 15 76.4 ± 7.87 0.46 ± 0.31 26.7 ± 2.48 25.9 ± 2.91 0.95;0.93 LM 15 76.4 ± 11.9 0.49 ± 0.51 30.4 ± 1.89 30.3 ± 2.07 0.89;0.89 3D-TSE MRI MM 16 84.3 ± 9.02 0.36 ± 0.28 29.3 ± 4.29 28.8 ± 4.81 0.95;0.95 LM 16 85.1 ± 10.5 0.33 ± 0.33 32.1 ± 3.33 32.2 ± 3.47 0.99;0.99 T2 map MRI MM 31 75.2 ± 7.8 0.50 ± 0.34 28 ± 3.82 27.4 ± 4.31 0.95;0.94 LM 31 76.1 ± 10.6 0.45 ± 0.45 31.2 ± 3.05 31.1 ± 3.18 0.97;0.97

2D, two-dimensional; 3D, three-dimensional; DSI, Dice similarity index; ICC, intraclass correlation coefficient; LM, lateral meniscus; MM, medial meniscus; MR, magnetic resonance; TSE, turbo spin echo.


For the 2D-TSE and 3D-TSE MR images, the T2 statistics, r  T2  , and ICC  T2  values were estimated from the co-registrations of the 2D-TSE and 3D-TSE MR images onto the T2 maps, respectively. For the T2 maps, the statistics were inclusive of both.


![Figure 3, Example of automated versus manual segmentation of the menisci for a patient imaged with (a) 3D-TSE and T2 mapping MRI (MM.DSI 3DTSE = 90%, MM.DSI T2 = 81%, LM.DSI 3DTSE = 84%, LM.DSI T2 = 85%) and for a patient imaged with (b) 2D-TSE and T2 mapping MRI (MM.DSI TSE = 79%, MM.DSI T2 = 74%, LM.DSI TSE = 74%, LM.DSI T2 = 75%). The manual segmentations and automated segmentations are displayed on the top and bottom rows, respectively. 2D, two-dimensional; 3D, three-dimensional; DSI, Dice similarity index; LM, lateral meniscus; MM, medial meniscus; MRI, magnetic resonance imaging; TSE, turbo spin echo.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedT2mappingoftheMenisciFromMagneticResonanceImagesinPatientswithAcuteKneeInjury/2_1s20S1076633217302088.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Correlation ( left ) and Bland-Altman ( right ) analyses comparing the T2 values estimated from the automated (T2.A) and manual (T2.M) segmentations.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedT2mappingoftheMenisciFromMagneticResonanceImagesinPatientswithAcuteKneeInjury/3_1s20S1076633217302088.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantitative Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, T2 analyses of the subset of patient MR images that were manually segmented. In the plots, values suffixed with *.M and *.A are the values estimated from the manual segmentations ( blue ) and automated segmentations ( orange ), respectively. (a) and (b) Regional analysis of the MM and LM. Ant.M, Mid.M, and Post.M describe the T2 statistics estimated from the manual segmentations, whereas Ant.A, Mid.A, and Post.A describe those estimated from the automated segmentations. (c) and (d) Comparison of the MM and LM T2 values between the tear group and the no-tear group. LM, lateral meniscus; MM, medial meniscus; MR, magnetic resonance. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedT2mappingoftheMenisciFromMagneticResonanceImagesinPatientswithAcuteKneeInjury/4_1s20S1076633217302088.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, ( Top ) Automated T2 mapping obtained for a patient with no reported injury of the MM. ( Bottom ) Automated T2 mapping obtained for a patient with a bucket-handle tear appearing in the mid-compartment of the MM. MM, medial meniscus.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedT2mappingoftheMenisciFromMagneticResonanceImagesinPatientswithAcuteKneeInjury/5_1s20S1076633217302088.jpg)

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Source of Funding

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Supplementary Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Appendix S1

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Englund M., Lohmander L.S.: Risk factors for symptomatic knee osteoarthritis fifteen to twenty-two years after meniscectomy. Arthritis Rheum 2004; 50: pp. 2811-2819.


- 2\. Englund M.: Effect of meniscal damage on the development of frequent knee pain, aching, or stiffness. Arthritis Rheum 2007; 56: pp. 4048-4054.


- 3\. Hunter D.J., Zhang Y.Q., Niu J.B., et. al.: The association of meniscal pathologic changes with cartilage loss in symptomatic knee osteoarthritis. Arthritis Rheum 2006; 54: pp. 795-801.


- 4\. Lee J.-J., Choi Y.-J., Shin K.-Y., et. al.: Medial meniscal tears in anterior cruciate ligament-deficient knees: effects of posterior tibial slope on medial meniscal tear. Knee Surg Relat Res 2011; 23: pp. 227-230.


- 5\. Zarins Z.A., Bolbos R.I., Pialat J.B., et. al.: Cartilage and meniscus assessment using T1rho and T2 measurements in healthy subjects and patients with osteoarthritis. Osteoarthritis Cartilage 2010; 18: pp. 1408-1416.


- 6\. Juras V., Apprich S., Zbýň Š., et. al.: Quantitative MRI analysis of menisci using biexponential T 2\* fitting with a variable echo time sequence. Magn Reson Med 2014; 71: pp. 1015-1023.


- 7\. Rauscher I., Stahl R., Cheng J., et. al.: Meniscal measurements of T1rho and T2 at MR imaging in healthy subjects and patients with osteoarthritis. Radiology 2008; 249: pp. 591-600.


- 8\. Chu C.R., Williams A.A., West R.V., et. al.: Quantitative magnetic resonance imaging UTE-T2\* mapping of cartilage and meniscus healing after anatomic anterior cruciate ligament reconstruction. Am J Sports Med 2014; 42: pp. 1847-1856.


- 9\. Nemec S.F., Marlovits S., Trattnig S., et. al.: High-resolution magnetic resonance imaging and conventional magnetic resonance imaging on a standard field-strength magnetic resonance system compared to arthroscopy in patients with suspected meniscal tears. Acad Radiol 2008; 15: pp. 928-933.


- 10\. Mayerhoefer M.E.M., Welsch G.G.H., Riegler G., et. al.: Feasibility of texture analysis for the assessment of biochemical changes in meniscal tissue on T1 maps calculated from delayed gadolinium-enhanced magnetic resonance imaging of cartilage data: comparison with conventional relaxation time measurements. Invest Radiol 2010; 45: pp. 543-547.


- 11\. Krishnan N.: Delayed gadolinium-enhanced magnetic resonance imaging of the meniscus: an index of meniscal tissue degeneration?. Arthritis Rheum 2007; 56: pp. 1507-1511.


- 12\. Glaser C., D'Anastasi M., Theisen D., et. al.: Understanding 3D TSE sequences: advantages, disadvantages, and application in MSK imaging. Semin Musculoskelet Radiol 2015; 19: pp. 321-327.


- 13\. Klocke N.F., Amendola A., Thedens D.R., et. al.: Comparison of T1rho, dGEMRIC, and quantitative T2 MRI in preoperative ACL rupture patients. Acad Radiol 2013; 20: pp. 99-107.


- 14\. Wang L., Regatte R.R.: Quantitative mapping of human cartilage at 3.0T. Acad Radiol 2014; 21: pp. 463-471.


- 15\. Baum T., Joseph G.B., Karampinos D.C., et. al.: Cartilage and meniscal T2 relaxation time as non-invasive biomarker for knee osteoarthritis and cartilage repair procedures. Osteoarthritis Cartilage 2013; 21: pp. 1474-1484.


- 16\. Liu F., Samsonov A., Wilson J.J., et. al.: Rapid in vivo multicomponent T2 mapping of human knee menisci. J Magn Reson Imaging 2015; 42: pp. 1321-1328.


- 17\. Chang E.Y., Du J., Bae W.C., et. al.: Qualitative and quantitative ultrashort echo time imaging of musculoskeletal tissues. Semin Musculoskelet Radiol 2015; 19: pp. 375-386.


- 18\. Siorpaes K., Wenger A., Bloecker K., et. al.: Interobserver reproducibility of quantitative meniscus analysis using coronal multiplanar DESS and IWTSE MR imaging. Magn Reson Med 2012; 67: pp. 1419-1426.


- 19\. Tamez-Pena J.: Unsupervised statistical segmentation of multispectral volumetric MRI images. Med Imaging'99 Int Soc Opt Photonics 1999; 3661: pp. 300-311.


- 20\. Sasaki T., Hata Y., Ando Y., et. al.: Fuzzy rule-based approach to segment the menisci regions from MR images. Med Imaging'99 1999; pp. 258-265.


- 21\. Fripp J., Bourgeat P., Engstrom C., et. al.: Automated segmentation of the menisci from MR images.Biomed imaging from nano to macro, 2009 ISBI'09 IEEE Int Symp.2009.pp. 510-513.


- 22\. Zhang K., Lu W., Marziliano P.: The unified extreme learning machines and discriminative random fields for automatic knee cartilage and meniscus segmentation from multi-contrast MR images. Mach Vis Appl 2013; 24: pp. 1459-1472.


- 23\. Paproki A., Engstrom C., Chandra S.S., et. al.: Automated segmentation and analysis of normal and osteoarthritic knee menisci from magnetic resonance images—data from the Osteoarthritis Initiative. Osteoarthritis Cartilage 2014; 22: pp. 1259-1270.


- 24\. Welsch G.H., Zak L., Mamisch T.C., et. al.: Advanced morphological 3D magnetic resonance observation of cartilage repair tissue (MOCART) scoring using a new isotropic 3D proton-density, turbo spin echo sequence with variable flip angle distribution (PD-SPACE) compared to an isotropic 3D steady-state. J Magn Reson Imaging 2011; 33: pp. 180-188.


- 25\. Yushkevich P.A., Piven J., Hazlett H.C., et. al.: User-guided 3D active contour segmentation of anatomical structures: significantly improved efficiency and reliability. Neuroimage 2006; 31: pp. 1116-1128.


- 26\. Ibanez L., Schroeder W., Ng L.: The ITK software guide second edition updated for ITK version 2.4. Available at: http://www.itk

- 27\. Rivest-Hénault D., Dowson N., Greer P.B., et. al.: Robust inverse-consistent affine CT-MR registration in MRI-assisted and MRI-alone prostate radiation therapy. Med Image Anal 2015; 23: pp. 56-69.


- 28\. Cootes T., Taylor C., Cooper D.: Active shape models—their training and application. Comput Vis 1995; 61: pp. 38-59.


- 29\. Fripp J., Lucas E., Engstrom C.: Automated morphological knee cartilage analysis of 3D MRI at 3T.2013.pp. 146-156.


- 30\. Peterfy C.G., Schneider E., Nevitt M.: The osteoarthritis initiative: report on the design rationale for the magnetic resonance imaging protocol for the knee. Osteoarthritis Cartilage 2008; 16: pp. 1433-1441.


- 31\. Bourgeat P., Dore V., Villemagne V.L., et. al.: MilxXplore: a web-based system to explore large imaging datasets. J Am Med Inform Assoc 2013; 20: pp. 1046-1052.


- 32\. Benjamini Y., Hochberg Y.: Controlling the false discovery rate: a practical and powerful approach to multiple testing. J R Stat Soc Ser B 1995; 57: pp. 289-300.


- 33\. Abrams G.D., Frank R.M., Gupta A.K., et. al.: Trends in meniscus repair and meniscectomy in the United States, 2005–2011. Am J Sports Med 2013; 41: pp. 2333-2339.


- 34\. Nicholas S.J., Golant A., Schachter A.K., et. al.: A new surgical technique for arthroscopic repair of the meniscus root tear. Knee Surg Sports Traumatol Arthrosc 2009; 17: pp. 1433-1436.


- 35\. Swanson M.S.: Semi-automated segmentation to assess the lateral meniscus in normal and osteoarthritic knees. Osteoarthritis Cartilage 2010; 18: pp. 344-353.