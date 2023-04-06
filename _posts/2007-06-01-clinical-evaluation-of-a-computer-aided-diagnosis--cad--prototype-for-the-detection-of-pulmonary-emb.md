---
title: Clinical Evaluation of a Computer-Aided Diagnosis (CAD) Prototype for the Detection of Pulmonary Embolism
author: [Sonja Buhmann MD,Peter Herzog MD,Jin Liang PhD,Mathias Wolf PhD,Marcos Salganicoff PhD,Chlodwig Kirchhoff MD,Maximilian Reiser MD PhD,Christoph H. Becker MD]
date: 2007-06-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 6 SOURCE CL_S_AcademicRadiologyVolume14Issue6 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

To evaluate the performance of a prototype computer-aided diagnosis (CAD) tool using artificial intelligence techniques for the detection of pulmonary embolism (PE) and the possible benefit for general radiologists.

## Materials and Methods

Forty multidetector row computed tomography datasets (16/64- channel scanner) using 100 kVp, 100 mAs effective/slice, and 1-mm axial reformats in a low-frequency reconstruction kernel were evaluated. A total of 80 mL iodinated contrast material was injected at a flow rate of 5 mL/seconds. Primarily, six general radiologists marked any PE using a commercially available lung evaluation software with simultaneous, automatic processing by CAD in the background. An expert panel consisting of two chest radiologists analyzed all PE marks from the readers and CAD, also searching for additional finding primarily missed by both, forming the ground truth.

## Results

The ground truth consisted of 212 emboli. Of these, 65 (31%) were centrally and 147 (69%) were peripherally located. The readers detected 157/212 emboli (74%) leading to a sensitivity of 97% (63/65) for central and 70% (103/147) for peripheral emboli with 9 false-positive findings. CAD detected 168/212 emboli (79%), reaching a sensitivity of 74% for central (48/65) and 82%(120/147) for peripheral emboli. A total of 154 CAD candidates were considered as false positives, yielding an average of 3.85 false positives/case.

## Conclusions

The CAD software showed a sensitivity comparable to that of the general radiologists, but with more false positives. CAD detection of findings incremental to the radiologists suggests benefit when used as a second reader. Future versions of CAD have the potential to further increase clinical benefit by improving sensitivity and reducing false marks.

Suspected acute pulmonary embolism (PE), a potentially life-threatening condition, in most cases resulting from underlying venous thromboembolic disease, presents a common problem in emergency units especially at night or at the weekends. Consequently, emergency medicine specialists often feel compelled to order a plasma D-dimer in patients with dyspnea or pleuritic chest pain, even when the clinician recognizes a very low pretest probability. Overtesting for PE has long been recognized as a significant problem in the process of ruling out pulmonary embolism ( ). However, early and accurate diagnosis is the key to survival of these patients. But in particular, plasma D-dimer test frequently result in false positive results demanding expensive and time consuming radiologic imaging ( ). However, the diagnosis remains problematic because very often clinical signs and symptoms are mimicked by other diseases. The former method of choice in terms of ventilation-perfusion scintigraphy is insensitive and nonspecific ( ).

Recently, spiral computed tomography (CT) contrast angiography has been established as the examination method of choice for investigating patients with suspected PE, mainly because of the high acquisition speed of multidetector row CT (MDCT) systems. But the accuracy of CT contrast angiography is uncertain, resulting in sensitivities as low as 70% ( ).

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Material and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## PE CAD Algorithm Description

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, The figure presents the first findings of both evaluating entities, separated for central and peripheral located candidate pulmonary embolism.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ClinicalEvaluationofaComputerAidedDiagnosisCADPrototypefortheDetectionofPulmonaryEmbolism/0_1s20S1076633207001249.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


The Measured HUs in the Different Vascular Regions of the Lung to Evaluate Image Quality of the Acquired Computed Tomography-Pulmonary Angiography Datasets


Pulmonary trunk SI (HU) 496.2 ± 81.5 Right pulmonary art (HU) 495.9 ± 90.1 Left pulmonary art (HU) 500.3 ± 89.9 Peripheral art (HU) 472.4 ± 18.6 SI paraspinal muscle (HU) 53.4 ± 24.1 Background noise (HU) 8.1 ± 7.4 Signal-noise ratio 36.0 ± 13.7 Contrast-noise ratio 31.7 ± 12.7

SI: Signal intensity; HU: Hounsfield units.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, This diagram presents the complete number of findings of the expert panel and the confirmed emboli found by both the human readers and computer-aided diagnosis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ClinicalEvaluationofaComputerAidedDiagnosisCADPrototypefortheDetectionofPulmonaryEmbolism/1_1s20S1076633207001249.jpg)

![Figure 3, False-positive findings of human readers and computer-aided diagnosis.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ClinicalEvaluationofaComputerAidedDiagnosisCADPrototypefortheDetectionofPulmonaryEmbolism/2_1s20S1076633207001249.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, True-positive finding of the computer-aided diagnosis prototype with embolus in the right upper lobe artery, correctly marked by a red marker box.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ClinicalEvaluationofaComputerAidedDiagnosisCADPrototypefortheDetectionofPulmonaryEmbolism/3_1s20S1076633207001249.jpg)

![Figure 5, Pulmonary embolism in the periphery of the right lower lobe that was missed by the human readers and detected by the computer-aided diagnosis (CAD) prototype, thus considered as false-negative finding of the human reader correctly identified by CAD.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ClinicalEvaluationofaComputerAidedDiagnosisCADPrototypefortheDetectionofPulmonaryEmbolism/4_1s20S1076633207001249.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Robin E.D.: Overdiagnosis and overtreatment of pulmonary embolism: the emperor may have no clothes. Ann Intern Med 1977; 87: pp. 775-781.


- 2\. Goldstein N.M., Kollef M.H., Ward S., et. al.: The impact of the introduction of the rapid d-dimer assay on the diagnostic evaluation of suspected pulmonary embolism. Arch Intern Med 2001; 161: pp. 567-571.


- 3\. Anderson D.R., Wells P.S.: Improvements in the diagnostic approach for patients with suspected pulmonary embolism. Thromb Haemost 1999; 82: pp. 878-886.


- 4\. Kruip M.J.H.A., Leclerq M.G.L., van der Heul C., et. al.: Diagnostic strategies for excluding pulmonary embolism in clinical outcome studies: a systematic review. Ann Intern Med 2003; 138: pp. 941-951.


- 5\. Perrier A., Howarth N., Didier D., et. al.: Performance of helical computed tomography in unselected outpatients with suspected pulmonary embolism. Ann Intern Med 2001; 135: pp. 88-97.


- 6\. Rathburn S.W., Raskob G.E., Whitsett T.L.: Sensitivity and specificity of helical computed tomography in the diagnosis of pulmonary embolism: a systematic review. Ann Intern Med 2000; 132: pp. 227-232.


- 7\. Goodman L.R., Curtin J.J., Mewissen M.W., et. al.: Detection of pulmonary embolism in patients with unresolved clinical and scintigraphic diagnosis: helical versus angiography. AJR Am J Roentgenol 1995; 164: pp. 1369-1374.


- 8\. Kim K.I., Mueller N.L., Mayo J.R.: Clinically suspected pulmonary embolism: utility of spiral CT. Radiology 1999; 210: pp. 693-697.


- 9\. Remy-Jardin M., Remy J., Baghaie F., et. al.: Clinical value of thin collimation in the diagnostic work up of pulmonary embolism. AJR Am J Roentgenol 2000; 175: pp. 407-411.


- 10\. PIOPED Investigators: Value of ventilation/perfusion scan in acute pulmonary embolism: results of the prospective investigation of pulmonary embolism diagnosis. JAMA 1990; 263: pp. 2753-2759.


- 11\. Remy-Jardin M., Jardin J., Deschildre F., et. al.: Diagnosis of pulmonary embolism with spiral CT: comparison with pulmonary angiography and scintigraphy. Radiology 1996; 200: pp. 699-706.


- 12\. Garg K., Welsh G.H., Feyerabend A.J., et. al.: Pulmonary embolism: diagnosis of with spiral CT and ventilation-perfusion scanning—correlation with pulmonary angiographic results and clinical outcome. Radiology 1998; 208: pp. 201-208.


- 13\. Drucker E.A., Rivitz S.M., Shepard J.A., et. al.: Acute pulmonary embolism: assessment of helical CT for diagnosis. Radiology 1998; 209: pp. 235-241.


- 14\. Masutani Y., MacMahon H., Doi K.: Computerized detection of pulmonary embolism in spiral CT angiography based on volumetric image analysis. IEEE Trans Med Imaging 2002; 21: pp. 1517-1523.


- 15\. Wittram C., Maher M.M., Yoo A.J., et. al.: CT angiography of pulmonary embolism: diagnostic criteria and causes of misdiagnosis. RadioGraphics 2004; 24: pp. 1219-1238.


- 16\. Fairfield J.: 1990.pp. 712-716. IEEE Proceedings of 10th International Conference on Pattern Recognition. Atlantic City


- 17\. Stein P.D., Athanasoulis C., Alavi A., et. al.: Complications and validity of pulmonary angiography in acute pulmonary embolism. Circulation 1992; 85: pp. 462-468.


- 18\. Diffin D., Leyendecker J.R., Johnson S.P., et. al.: Effect of anatomic distribution of pulmonary emboli on interobserver agreement in the interpretation of pulmonary angiography. AJR Am J Roentgenol 1998; 171: pp. 1085-1089.


- 19\. Stein P.D., Henry J.W., Gottschalk A.: Reassessment of pulmonary angiography for the diagnosis of pulmonary embolism. Radiology 1999; 210: pp. 689-691.


- 20\. Meaney J., Weg J.G., Chenevert T.L., et. al.: Diagnosis of pulmonary embolism with magnetic resonance angiography. N Engl J Med 1997; 336: pp. 1422-1427.


- 21\. Roberts D.A., Gefter W.B., Hirsch J.A., et. al.: Pulmonary perfusion: respiratory-triggered three-dimensional MR imaging with arterial spin-tagging-preliminary results in healthy volunteers. Radiology 1999; 212: pp. 890-895.


- 22\. van Erkel A.R., van Rossum A.B., Bloem J.L., et. al.: Spiral CT angiography for suspected pulmonary embolism: a cost-effectiveness analysis. Radiology 1996; 201: pp. 29-36.


- 23\. Stanford W., Reiners T.J., Thompson B.H., et. al.: Contrast-enhanced thin slice ultrafast computed tomography for the detection of small pulmonary emboli. Invest Radiol 1993; 29: pp. 184-187.


- 24\. Geraghty J., Stanford W., Landas S.K., et. al.: Ultrafast computed tomography in experimental pulmonary embolism. Invest Radiol 1991; 27: pp. 60-63.


- 25\. Remy-Jardin M., Remy J., Artaud D., et. al.: Peripheral pulmonary arteries: optimization of the spiral CT acquisition protocol. Radiology 1997; 204: pp. 157-163.


- 26\. Schoepf J., Holzknecht N., Helmberger T.K., et. al.: Subsegmental pulmonary emboli: improved detection with thin-collimation multi-detector row spiral CT. Radiology 2002; 222: pp. 483-490.


- 27\. Zhou C., Chan H.P., Patei S., et. al.: Preliminary investigation of computer-aided detection of pulmonary embolism in three-dimensional computed tomography pulmonary angiography images. Acad Radiol 2005; 12: pp. 782-792.


- 28\. Masutani Y., MacMahon H., Doi K.: Computerized detection of pulmonary embolism in spiral CT angiography based on volumetric image analysis. IEEE Trans Med Imaging 2002; 12: pp. 1517-1523.


- 29\. Schoepf U.J., Schneider A.C., Das M., et. al.: 2003.