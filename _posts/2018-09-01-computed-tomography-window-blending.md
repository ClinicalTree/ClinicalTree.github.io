---
title: Computed Tomography Window Blending
author: [CL_AT_JacobCMellMD,CL_AT_JeremyRWortmanMD,CL_AT_TatianaCRochaMD,CL_AT_LesRFolioDOMPH,CL_AT_KatherinePAndriolePhD,CL_AT_BhartiKhuranaMD]
date: 2018-09-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 25, Issue 9]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

This study aims to demonstrate the feasibility of processing computed tomography (CT) images with a custom window blending algorithm that combines soft-tissue, bone, and lung window settings into a single image; to compare the time for interpretation of chest CT for thoracic trauma with window blending and conventional window settings; and to assess diagnostic performance of both techniques.

## Materials and Methods

Adobe Photoshop was scripted to process axial DICOM images from retrospective contrast-enhanced chest CTs performed for trauma with a window-blending algorithm. Two emergency radiologists independently interpreted the axial images from 103 chest CTs with both blended and conventional windows. Interpretation time and diagnostic performance were compared with Wilcoxon signed-rank test and McNemar test, respectively. Agreement with Nexus CT Chest injury severity was assessed with the weighted kappa statistic.

## Results

A total of 13,295 images were processed without error. Interpretation was faster with window blending, resulting in a 20.3% time saving ( _P_ < .001), with no difference in diagnostic performance, within the power of the study to detect a difference in sensitivity of 5% as determined by post hoc power analysis. The sensitivity of the window-blended cases was 82.7%, compared to 81.6% for conventional windows. The specificity of the window-blended cases was 93.1%, compared to 90.5% for conventional windows. All injuries of major clinical significance (per Nexus CT Chest criteria) were correctly identified in all reading sessions, and all negative cases were correctly classified. All readers demonstrated near-perfect agreement with injury severity classification with both window settings.

## Conclusions

In this pilot study utilizing retrospective data, window blending allows faster preliminary interpretation of axial chest CT performed for trauma, with no significant difference in diagnostic performance compared to conventional window settings. Future studies would be required to assess the utility of window blending in clinical practice.

## Introduction

Rapid and accurate interpretation of computed tomography (CT) images is an essential component of managing acutely traumatized patients based on the “golden hour in shock” principle that calls for immediate recognition and treatment of life-threatening injuries. The CT findings of code-trauma patients are interpreted and verbally communicated in a real-time fashion while the patient is still on the CT table as soon as the first axial reconstructions are available. This immediate interpretation allows the trauma surgeon to plan surgical intervention or transfer the patient to the intensive care unit or a major trauma center within minutes of image acquisition, as has been previously described in mass casualty incidents and in combat . Because the dynamic range acquired by CT is greater than can be displayed on an 8-bit or 10-bit clinical workstation monitor , each examination must be thoroughly reviewed in at least three distinct window and level settings optimized for soft tissue, lung, and bone to optimally visualize critical injuries that may only be evident in a specific window setting. In high-acuity situations or mass casualty incidents where multiple CT scanners may be operating simultaneously, a technique to eliminate the need for adjustment of window and level settings has the potential to expedite the image review process and streamline patient throughput during the “golden hour.”

Through image processing techniques, the wide dynamic range of CT can be compressed to a reduced number of grayscale shades to allow simultaneous display of the full range of medically useful information in a single pass, without needing to change window or level settings. Several methods have previously been described to achieve this goal including window blending , companding , nonlinear CT windows , histogram equalization , and adaptive histogram equalization . None of these methods have achieved widespread clinical use, and many suffer from various artifacts and unfamiliar modification in relative attenuation of the fundamental radiographic densities.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Selection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Abbreviated List of Findings Determining Classification by Nexus CT Chest Criteria


Major clinical significance Pneumothorax or hemothorax, requiring chest tube Aortic or great vessel injury Multiple rib fractures, requiring surgical intervention or epidural nerve block Thoracic spine or scapular fracture, requiring surgical intervention Pulmonary contusion, requiring mechanical ventilation for respiratory failure Esophageal, tracheal, or bronchial injury, requiring surgical intervention Minor clinical significance Pneumothorax or hemothorax, not requiring evacuation procedure but observed as an inpatient Multiple rib fractures, not requiring surgical intervention or epidural nerve block Sternal, thoracic spine, or scapular fracture, not requiring surgical intervention Esophageal, tracheal, or bronchial injury, not requiring surgical intervention No clinical significance Hemothorax, pneumothorax, pneumomediastinum, pulmonary contusion/laceration, not requiring intervention or inpatient observation

CT, computed tomography.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Flowchart demonstrating the test cohort, selected from all trauma chest computed tomography (CT) interpreted at this institution between July 1, 2015, and January 31, 2017.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputedTomographyWindowBlending/0_1s20S1076633218300205.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CT Scanning

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Processing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reading Sessions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Standard of Reference

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Study Group

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Feasibility of Image Processing and Interpretation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, A 28-year-old male patient who underwent contrast-enhanced chest computed tomography (CT) after motorcycle accident, negative for traumatic injury. (a) Window-blended axial image through the midthorax. Note that the pulmonary vascular, pulmonary parenchyma, vascular structures, soft tissues, and osseous trabecular detail can be visualized. However, the interface between the cortex and the medullary space of the osseous structures including the ribs, vertebral body, sternum, and scapulae is more sharply delineated on the conventional bone windows. (b-d) Same CT slice in conventional window settings, in soft tissue (b) , bone (c) , and lung (d) window settings.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputedTomographyWindowBlending/1_1s20S1076633218300205.jpg)

![Figure 3, A 26-year-old male patient who underwent contrast-enhanced chest computed tomography (CT) after gunshot wound to the right posterior thorax, with findings of major clinical significance (pneumothorax requiring chest tube). (a) Window-blended axial image through the midthorax. There is pulverized bone and bullet fragments in the posterior right chest wall (white arrow) , and a large right pneumothorax (asterisk) . A right-sided chest tube is partially visualized (white arrowhead) . There are scattered foci of subcutaneous emphysema (black arrowheads) . Note the subtle right transverse process fracture (black arrow) . (b-d) Same CT slice in conventional window settings, in soft tissue (b) , bone (c) , and lung (d) window settings.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputedTomographyWindowBlending/2_1s20S1076633218300205.jpg)

![Figure 4, A 53-year-old female patient who underwent chest computed tomography (CT) after fall from four stories, with findings of major clinical significance (aortic injury). (a) Window-blended axial image through the midthorax. There is a transection of the descending thoracic aorta (black arrows) with a large mediastinal hematoma (asterisk) and a small left hemothorax (white arrow) . (b-d) Same CT slice in conventional window settings, in soft tissue (b) , bone (c) , and lung (d) window settings.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputedTomographyWindowBlending/3_1s20S1076633218300205.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Time for Interpretation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Average Time in Seconds to Interpret Each Examination ( _n_ = 103) in Blended and Conventional Windows, with Subgroup Analyses for Examinations of Major Clinical Significance, Minor Clinical Significance, and Negative for Intrathoracic Trauma


Reader Blended Conventional_P_ C-B (B/C %) Time (SD) \[Range\] Time (SD) \[Range\] All examinations ( _n_ = 103) Reader 1 91.9 s (44.4) \[39–258\] 109.3 s (49.8) \[42–279\] <.001  \\*  17.4 s (84.1%) Reader 2 135.2 s (31.5) \[80–234\] 179.6 s (54.1) \[106–356\] <.001  \\*  44.4 s (75.3%) Examinations of major clinical significance ( _n_ = 20) Reader 1 149.7 s (50.6) \[66–258\] 162.4 s (50.6) \[71–279\] .306 12.7 s (92.2%) Reader 2 164.4 s (33.0) \[100–234\] 238.5 s (57.8) \[132–356\] <.001  \\*  74.1 s (68.9%) Examinations of minor clinical significance ( _n_ = 36) Reader 1 89.5 s (27.1) \[52–144\] 114.6 s (39.9) \[63–256\] .0012  \\*  25.1 s (78.1%) Reader 2 137.0 s (33.3) \[80–221\] 182.8 s (48.9) \[111–330\] <.001  \\*  45.8 s (72.6%) Examinations negative for intrathoracic trauma ( _n_ = 42) Reader 1 63.8 s (21.3) \[39–118\] 75.2 s (20.3) \[42–137\] .0078  \\*  11.4 s (84.8%) Reader 2 118.1 s (16.5) \[90–155\] 146.5 s (24.5) \[106–200\] <.001  \\*  28.4 s (80.6%)

C-B, absolute time difference (in seconds) between conventional and blended windows; B/C, blended/conventional time ratio.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison of Diagnostic Performance: Statistical Significance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Pooled and Per-reader Global Sensitivity and Specificity (with 95% Confidence Interval) of 231 Findings, and _P_ value From McNemar Test Comparing Blended to Conventional Window Settings


Reader Sensitivity (95% Confidence Interval) Specificity (95% Confidence Interval) Blended Conventional_P_ Blended Conventional_P_ Pooled 382/462

82.7% (79–86%) 377/462

81.6% (78–85%) .074 108/116

93.1% (87–97%) 105/116

90.5% (84–95%) .248 Reader 1 190/231

82.3% (77–87%) 189/231

81.8% (76–87%) 1.0 53/58

91.4% (81–97%) 54/58

93.1% (83–98%) 1.0 Reader 2 192/231

83.1% (78–88%) 188/231

81.4% (76–86%) .387 55/58

94.8% (86–99%) 51/58

87.9% (77–95%) .133

Table 4


Sensitivity and False Positives for Rib Fractures (Determined on a Per-case basis) with Blended and Conventional Windows


Sensitivity Reader 1 Reader 2 Blended Conventional_P_ Blended Conventional_P_ Rib fracture—per case (45) 35/45 (77.8%) 37/45 (82.2%) .68 38/45 (84.4%) 35/45 (77.8%) .51

_P_ values were calculated with McNemar test.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison of Diagnostic Performance: Clinical Significance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Type and Number of Findings Determining Classification by Nexus CT Chest Criteria, in the 20 Included Cases of Major Clinical Significance


Finding Determining Major Clinical Significance by Nexus CT Chest Criteria Number of Instances Pneumothorax, requiring chest tube placement 10 Aortic or great vessel injury 6 (5 aortic; 1 subclavian) Contusion, requiring mechanical ventilation 4 (3/4 also with pneumothorax requiring chest tube) Hemothorax, requiring chest tube placement 2 Multiple rib fractures, requiring epidural nerve block 1

CT, computed tomography.


Total number of findings is greater than 20, as 3 cases had 2 findings indicating major clinical significance. Accuracy was 100% for all readers in all window settings for these findings. These findings were confirmed by operative reports (four cases of aortic injury), cardiology follow-up notes (one case of a stable aortic injury treated conservatively), cardiology follow-up notes and follow-up CT angiogram (subclavian pseudoaneurysm treated conservatively), and procedure notes or follow-up imaging for the remainder of the findings.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, A 46-year-old male patient who underwent chest computed tomography (CT) after motorcycle accident, with findings of minor clinical significance by reference standard. Chest CT portion of the examination was misclassified as negative for traumatic injury by a single reader with window blending. (a) Window-blended axial image through the midthorax. There is a mildly displaced left-sided rib fracture (white arrow) , and a tiny focus of pneumothorax more posteriorly (black arrow) ; same findings magnified in inset. (b-d) Same CT slice in conventional window settings, in soft tissue (b) , bone (c) , and lung (d) window settings. These findings were treated conservatively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ComputedTomographyWindowBlending/4_1s20S1076633218300205.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Impact and Future Directions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Limitations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Lerner E.B., Moscati R.M.: The golden hour: scientific fact or medical “urban legend”?. Acad Emerg Med 2001; 8: pp. 758-760.


- 2\. Bolster F., Linnau K., Mitchell S., et. al.: Emergency radiology and mass casualty incidents—report of a mass casualty incident at a level 1 trauma center. Emerg Radiol 2017; 24: pp. 47-53.


- 3\. Berger F.H., Korner M., Bernstein M.P., et. al.: Emergency imaging after a mass casualty incident: role of the radiology department during training for and activation of a disaster management plan. Br J Radiol 2016; 89: pp. 20150984.


- 4\. Brunner J., Rocha T.C., Chudgar A.A., et. al.: The Boston Marathon bombing: after-action review of the Brigham and Women's Hospital emergency radiology response. Radiology 2014; 273: pp. 78-87.


- 5\. Folio L.R.: Combat radiology: diagnostic imaging of blast and ballistic injuries.2010.SpringerNew York


- 6\. Kimpe T., Tuytschaever T.: Increasing the number of gray shades in medical display systems—how much is enough?. J Digit Imaging 2007; 20: pp. 422-432.


- 7\. Gabriel Peterson P., Pak S.K., Nguyen B., et. al.: Extreme compression for extreme conditions: pilot study to identify optimal compression of CT images using MPEG-4 video compression. J Digit Imaging 2012; 25: pp. 764-770.


- 8\. Whitworth S., Folio L., Nguyen B.: Universal trauma CT window for rapid preliminary interpretation. Emerg Radiol 2009; 16: pp. 502-503.


- 9\. Cohen-Duwek H., Spitzer H., Weitzen R., et. al.: A biologically-based algorithm for companding computerized tomography (CT) images. Comput Biol Med 2011; 41: pp. 367-379.


- 10\. Gomori J.M., Steiner I.: Non-linear CT windows. Comput Radiol 1987; 11: pp. 21-27.


- 11\. Lehr J.L., Capek P.: Histogram equalization of CT images. Radiology 1985; 154: pp. 163-169.


- 12\. Fayad L.M., Jin Y., Laine A.F., et. al.: Technical developments chest CT window settings with multiscale adaptive histogram equalization: pilot study. Radiology 2002; 223: pp. 845-852.


- 13\. Rodriguez R.M., Langdorf M.I., Nishijima D., et. al.: Derivation and validation of two decision instruments for selective chest CT in blunt trauma: a multicenter prospective observational study (NEXUS Chest CT). PLoS Med 2015; 12: e1001883


- 14\. Sodickson A., Opraseuth J., Ledbetter S.: Outside imaging in emergency department transfer patients: CD import reduces rates of subsequent imaging utilization. Radiology 2011; 260: pp. 408-413.


- 15\. Mandell J.C., Khurana B., Folio L.R., et. al.: Clinical Applications of a CT Window Blending Algorithm: RADIO (Relative Attenuation-Dependent Image Overlay). J Digit Imaging 2017; 30: pp. 358-368.


- 16\. Archie K.A., Marcus D.S.: DicomBrowser: software for viewing and modifying DICOM metadata. J Digit Imaging 2012; 25: pp. 635-645.


- 17\. Landis J.R., Koch G.G.: The measurement of observer agreement for categorical data. Biometrics 1977; 33: pp. 159-174.


- 18\. Hajian-Tilaki K.: Sample size estimation in diagnostic test studies of biomedical informatics. J Biomed Inform 2014; 48: pp. 193-204.


- 19\. Ringl H., Lazar M., Töpker M., et. al.: The ribs unfolded—a CT visualization algorithm for fast detection of rib fractures: effect on sensitivity and specificity in trauma patients. Eur Radiol 2015; 25: pp. 1865-1874.


- 20\. Toth D.F., Töpker M., Mayerhöfer M.E., et. al.: Rapid detection of bone metastasis at thoracoabdominal CT: accuracy and efficiency of a new visualization algorithm. Radiology 2013; 270: pp. 130789.


- 21\. Bongers M.N., Bier G., Ditt H., et. al.: Improved CT detection of acute herpes simplex virus type 1 encephalitis based on a frequency-selective nonlinear blending: comparison with MRI. Am J Roentgenol 2016; 207: pp. 1082-1088.


- 22\. Bongers M.N., Bier G., Kloth C., et. al.: Improved delineation of pulmonary embolism and venous thrombosis through frequency selective nonlinear blending in computed tomography. Invest Radiol 2017; 52: pp. 240-244.


- 23\. Singh A.K., Ditkofsky N.G., York J.D., et. al.: Blast injuries: from improvised explosive device blasts to the Boston Marathon bombing. Radiographics 2016; 36: pp. 295-307.


- 24\. Wyen H., Lefering R., Maegele M., et. al.: The golden hour of shock—how time is running out: prehospital time intervals in Germany—a multivariate analysis of 15,103 patients from the TraumaRegister DGU(R). Emerg Med J 2013; 30: pp. 1048-1055.


- 25\. Jeong Y.J., Lee K.S., Yoon Y.C., et. al.: Evaluation of small pulmonary arteries by 16-slice multidetector computed tomography: optimum slab thickness in condensing transaxial images converted into maximum intensity projection images. J Comput Assist Tomogr 2004; 28: pp. 195-203.


- 26\. Valencia R., Denecke T., Lehmkuhl L., et. al.: Value of axial and coronal maximum intensity projection (MIP) images in the detection of pulmonary nodules by multislice spiral CT: comparison with axial 1-mm and 5-mm slices. Eur Radiol 2006; 16: pp. 325-332.