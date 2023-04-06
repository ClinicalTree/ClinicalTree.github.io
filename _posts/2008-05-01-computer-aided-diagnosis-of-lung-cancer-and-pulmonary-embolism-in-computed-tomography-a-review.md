---
title: Computer-Aided Diagnosis of Lung Cancer and Pulmonary Embolism in Computed Tomography—A Review
author: [Heang-Ping Chan PhD,Lubomir Hadjiiski PhD,Chuan Zhou PhD,Berkman Sahiner PhD]
date: 2008-05-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 15, Issue 5 SOURCE CL_S_AcademicRadiologyVolume15Issue5 1}]
tags: [Journals,General Radiology]
---
Computer-aided detection (CADe) and computer-aided diagnosis (CADx) have been important areas of research in the last two decades. Significant progress has been made in the area of breast cancer detection, and CAD techniques are being developed in many other areas. Recent advances in multidetector row computed tomography have made it an increasingly common modality for imaging of lung diseases. A thoracic examination using thin-section computed tomography contains hundreds of images. Detection of lung cancer and pulmonary embolism on computed tomographic (CT) examinations are demanding tasks for radiologists because they have to search for abnormalities in a large number of images, and the lesions can be subtle. If successfully developed, CAD can be a useful second opinion to radiologists in thoracic CT interpretation. In this review, we summarize the studies that have been reported in these areas, discuss some challenges in the development of CAD, and identify areas that deserve particular attention in future research.

Computer-aided detection (CADe) and computer-aided diagnosis (CADx) have been important areas of research in the last two decades. Because of the high prevalence of breast cancer and challenges in interpretation of mammograms, most of the early work on CAD (CADe or CADx) was devoted to detection and characterization of masses and microcalcifications on mammograms. However, in the last decade, numerous studies on the development of CAD techniques have been reported for other diseases and imaging modalities. Lung cancer is the leading cause of cancer death in both men and women. The interpretation of thoracic computed tomographic (CT) scans for lung nodules is a demanding task for radiologists, and the risks of false-negative detection and benign nodules being recommended for biopsy are high. There is a potential for improvement if CADe and CADx are available for lung nodules in CT scans. A different, but related area is the detection of pulmonary embolism (PE) in CT pulmonary angiography (CTPA). PE is a common, potentially fatal condition in all age groups associated with significant morbidity and mortality in untreated patients, and radiologists may benefit from CADe because of the complexity of the pulmonary vascular structures and the large number of vessels to be inspected for PE in each case. In this review, we will focus our discussion on CADe and CADx of lung nodules and CADe of PE on CT examinations.

## Challenges in lung cancer detection on CT examinations

In the United States, it is estimated that there will be 160,390 deaths from lung cancer and that 213,380 new cases will be diagnosed in 2007 ( ). Lung cancer remains the leading cause of cancer death for men since the 1950s and for women since 1987. The overall prognosis of lung cancer is very poor. The 5-year survival rate is only about 16% for all stages combined ( ). However, if detected and resected at its earliest stage (stage I), the 5-year survival rate can reach 70% ( ).

Unfortunately, previous studies failed to show a significant reduction in mortality by screening with chest radiography (CXR) ( ) despite the improvement in stage distribution, resectability, survival, and fatality in lung cancer. Lung cancer screening was therefore not recommended in clinical practice. Interest in screening was revived when computed tomography was shown to have higher sensitivity in detecting small, early stage lung cancer than CXR. The Early Lung Cancer Action Project (ELCAP) investigated the usefulness of annual low dose CT screening for lung cancer in a high-risk population and found that low-dose computed tomography can detect four times more malignant lung nodules than CXR, and six times more stage I malignant nodules, which potentially are more curable ( ). More recently, the International ELCAP (I-ELCAP) study showed that the 10-year survival of patients with stage I lung cancer detected on CT screening and who underwent surgical resection within 1 month reached 92%, and concluded that CT screening can detect lung cancer that is curable ( ). However, another multicenter study found that, in comparison with the predictions from a model, there were a threefold increase in cancer detection and 10-fold increase in lung resection, but no decline in diagnoses of advanced lung cancer or mortality rate ( ). A 30-site randomized controlled study (National Lung Screening Trial), sponsored by the National Cancer Institute, has enrolled about 50,000 participants to compare the effect of screening using helical computed tomography or chest x-rays on the mortality rate of lung cancer patients. The results of the study will not be available until about 2010.

Although there is controversy over whether CT screening may reduce lung cancer mortality, there is consensus that computed tomography allows the detection of more and smaller lung nodules than CXR. In the National Emphysema Treatment Trial, 25.6% of the 446 emphysema patients were found to have noncalcified nodules ( ). In ELCAP, 23.3% of the patients were found to have noncalcified nodules by computed tomography, which represented a threefold increase in sensitivity than CXRs ( ). This increase in sensitivity comes at the price of an increased workload for radiologists. A major potential difficulty in using helical computed tomography for screening is the dramatic increase in the number of images that need to be interpreted for each case. Another potential difficulty is the additional resources that will be needed for clinical management of the expected screening detected nodules. Different criteria are being used by physicians to manage lung nodules in current clinical practice ( ). Many nodules are recommended to be followed up. However, the rate of the screening detected nodules being resected is still high at about 20–40% ( ). A study of 426 patients who underwent video-assisted thoracoscopic surgery ( ) indicated that 42.5% of these cases were benign. Keagy et al ( ) found that 40% of their patients with benign nodules were subjected to thoracotomy for presumed malignant disease. It is therefore important to establish, if possible, more reliable criteria to estimate the likelihood of malignancy of the lung nodules based on image information without resorting to invasive procedures, thereby reducing the potential patient morbidity and additional health care costs associated with lung cancer screening. 2-\[  18 F\]fluoro-2-deoxy-D-glucose–enhanced positron emission tomographic scans ( ) have been found to provide high sensitivity and good specificity for differentiating nodules as malignant and benign, but the procedure will involve radioactivity, relatively high costs, and may not be available in many medical facilities. The I-ELCAP study ( ) demonstrated that, with workup protocols that mainly used repeated CT scans to estimate nodule growth, the negative biopsy rate could be as low as 8% in the patient cohort. However, short-term follow-up with repeated computed tomography will further increase radiologists' workload.

Although computed tomography has a much higher sensitivity than CXR, missed cancers are not uncommon in CT interpretation ( ). The main causes for missed cancers include detection errors and characterization errors. Detection errors can be attributed to factors such as oversight or failure to detect the lesion among other structures. Characterization errors may be attributed to the difficulty in differentiating malignant lesions from benign nodules. The latter can also cause a radiologist to overestimate the likelihood of malignancy and recommend biopsy for benign lesions. Double reading may reduce missed diagnoses, but it doubles the demand on radiologists' time. Some criteria have been suggested to estimate the likelihood of malignancy of solitary pulmonary nodules ( ). Computer-assisted classification of malignant and benign lung nodules has been attempted and promising results have been reported ( ). Gurney et al ( ) used Bayesian analysis and an artificial neural network ( ) to classify radiographic and clinical features and achieved a higher accuracy than subjective classification by radiologists. However, these computer classifiers used radiologist-identified image features, the extraction of which are both time consuming and subject to inter- and intra-observer variations. Subtle change in nodule volume, especially when the nodule is small, is difficult to discern visually on CT images.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Computerized detection of lung nodules

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Studies on the Development of CADe Systems for Detection of Lung Nodules in Thoracic Computed Tomography Examinations


References No. of Cases (No. of Exams) Section Thickness/Interval Nodule Sizes Total No. of Nodules Sensitivity FP Rate Giger et al, 1994 ( ) 8 10 mm 3–18 mm 2–21/case 94% 1.25/case Kanazawa et al, 1998 ( ) 450 (Screening in Japan) 10 mm \> 4 mm? 230 90% not reported Armato et al, 2001 ( ) 43 7–10 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


171 70% 1.5/section Ko et al, 2001 ( ) 8 (16 exams)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


>3 mm 295 91% 2.3/case Brown et al, 2001 ( ) 17 5–10 mm 5–30 mm 36 86% 11/case Lee et al, 2001 ( ) 20 10 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


98 72%

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Armato et al, 2002 ( ) 31 (38 LD exams) 10 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


50 80%

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Wormanns et al, 2002 ( ) 85 (88 LD exams) 5 mm 5–16 mm 68 38% 5.8/case Gurcan et al, 2002 ( ) 34 5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


63 84% 1.74/slice Armato et al, 2003 ( ) 38 5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


82

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Suzuki et al, 2003 ( ) 63 (LD) 10 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


71 80.3%

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Brown et al, 2003 ( ) 15 0.5–1 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


79

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


15/case (2 cm of thorax) Zhao et al, 2003 ( )

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


2–7 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Goo et al, 2003 ( ) 50 7–8 mm ≥5 mm 26 65% 8/case Paik et al, 2004 ( ) 8 Not reported ≥6 mm Not reported 90% 5.6/case Lee et al, 2004 ( ) 15 1–1.25 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


309

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


28.8/case Arimura et al, 2004 ( ) 106 10 mm 6–26 mm 131 81% 0.28/section McCulloch et al, 2004 ( ) 50 (LD) 2.5 mm 5.0–17.1 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


70% 8.3/case Awai et al, 2004 ( ) 82 7.5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


78 80%

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Ge et al, 2005 ( ) 56 (82 exams) 1–2.5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


116 80% 0.34/section Bae et al, 2005 ( ) 20 1 mm 3–27 mm 164 95.1% 6.9/case Rubin et al, 2005 ( ) 20 1.25/0.6 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


195

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Lin et al, 2005 ( ) 29 10 mm 10–30 mm 393 89.3% 0.21/section Kim et al, 2005 ( ) 10

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


≥3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Li et al, 2005 ( ) 38 (LD, missed cancers) 10 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


87% 3/case Armato et al, 2005 ( ) 393 (LD) 10 mm 3–30 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Kim et al, 2005 ( ) 14 1–5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


>29 GGO 89.7% 0.89/section Brown et al, 2005 ( ) 8 (LD) 1.25 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


22 86.4% 2.64 FPs/case (40 sections/case, 5 cm of thorax) Marten et al, 2005 ( ) (ICAD) 20 0.75 mm/0.6 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


135 76.3% 0.55/case Marten et al, 2005 ( ) (ICAD) 20

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


135  ⁎

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Peldschus et al, 2005 ( ) (R2 system) 100 1.25–3 mm Not reported 160 Reference radiologists checked CADe marks only 1.25/case Roy et al, 2006 ( ) 38 5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


82 70% 0.28/section or 0.03/section Boroczky et al, 2006 ( ) 25 (38 scans) 1.3 mm >3.5 mm 52 100% (no loss of TP in FP classification) –56.4% (FP reduction) Sahiner et al, 2006 ( ) 27 1–2.5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


80%

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Sahiner et al, 2007 ( ) 48 (30 positive, 18 negative) 1.5–3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


70 79% 4.9/case Wang et al, 2007 ( ) 12 3 mm 4–20 mm 47 100% 1.75/case Sahiner et al, 2007 ( ) 85 (52 positive, 33 negative) 1.5–3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


118 78% 5.5/case

LD, low-dose computed tomography; GGO, ground-glass opacity; R2, CADe system by R2 Technologies; ICAD, CADe system by Siemens Medical Solutions; CADe, computer-aided detection; TP, true positive; FP, false positive.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Effect of CADe on radiologists' detection of lung nodules

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Observer Performance Studies for Evaluation of the Effects of CADe on Radiologists' Detection of Lung Nodules in Thoracic Computed Tomography Examinations


References No. of Exams Section Thickness/Interval Nodule Sizes Total No. of Nodules No. of Observers Reading without CAD Reading with CAD_P_ Value Awai et al, 2004 ( ) 50 (36 pos, 14 neg) 7.5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


56

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Marten et al, 2004 ( ) (ICAD) 18 0.75/0.6 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


96 (89 solid, 2 mixed, 5 calcified) 4 rad, 2 read with CAD

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Marten et al, 2005 ( ) (ICAD) 20

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


135  ⁎  2

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Li et al, 2005 ( ) 27 (17 pos, 10 neg) (LD) 10 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


18 (6 GGO 10 mixed 1 solid)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Brown et al, 2005 ( ) 8 (6 pos, 2 neg) (LD) (5 cm of thorax) 1.25 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


22

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Rubin et al, 2005 ( ) (Simulation) 20 (19 pos, 1 neg) 1.25/0.6 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


195 3

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


< .05 Das et al, 2006 ( ) (R2, NEV) 25 (23 pos, 2 neg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


116 3

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Yuan et al, 2006 ( ) (Simulation) 150 (134 pos, 16 neg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


628 1

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Predicted sens increase 21.2% — Sahiner et al, 2007 ( ) 48 (30 pos, 18 neg) 1.5–3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


70 4

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


.03 Sahiner et al, 2007 ( ) 85 (52 pos, 33 neg) 1.5–3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


118 6

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


LD, low-dose computed tomography; pos, positive; neg, negative; rad, radiologists; resid, residents; AFROC, alternative free response receiver-operating characteristic; JAFROC, jackknife FROC; FOM, figure of merit; R2, CADe system by R2 Technologies; NEV, CADe system by Siemens Medical Solutions; ICAD, CADe system by Siemens Medical Solutions.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Computerized characterization of lung nodules

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Studies on the Development of CADx Systems for Characterization of Malignant and Benign Lung Nodules on Thoracic Computed Tomography Examinations


References No. of Exams Section Thickness/Interval Nodule Sizes Total No. of Nodules Malignant Benign_A  z_ Accuracy Sensitivity Specificity Henschke et al, 1997 ( ) Not reported 5 mm <30 mm 28 14 14 ∼0.79 (from graph) 89% (25/28) 100% 79% Kawata et al, 1998 ( ) 62 1 mm 6–25 mm 62 47 15 Not reported McNitt-Gray et al, 1999 ( ) 31 ≤3 mm 5–30 mm 31 17 14 Not reported 90.3% (28/31) 88.2% 92.9% McNitt-Gray et al, 1999 ( ) 32 ≤3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


32 19 13 0.992–1.0 90.6–100% 89.5–100% 92.3–100% Matsuki et al, 2002 ( ) 155 2 mm <30 mm 155 99 56 0.951 Lo et al, 2003 ( ) 48 Thin-section CT Not reported 48 24 24 0.89 Armato et al, 2003 ( ) 393 (LD) 10 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


0.79 Aoyama et al, 2003 ( ) 415 (LD) 10 mm <30 mm 489 76 413 0.846 Kawata et al, 2004 ( ) 174 0.5 mm Not reported 174 98 76 Not reported Li et al, 2004 ( ) 228 1 mm 3–20 mm 244 61 183 0.937 Suzuki et al, 2005 ( ) 415 (LD) 10 mm <30 mm 489 76 413 0.882 100% 48% Shah et al, 2005 ( ) 81 ≤3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


81 48 33 0.92 Shah et al, 2005 ( ) 54 not reported

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


54 33 21 81% 91% 67% Shah et al,. 2005 ( ) 35 pre-, post-contrast enhanced ≤3 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


35 19 16 0.69–0.92 Mori et al, 2005 ( ) 62 pre-, post-contrast enhanced 2 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


62 35 27

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Awai et al, 2006 ( ) 33 1–1.25 mm <30 mm 33 18 15 0.795 73% 72% 75% Way et al, 2006 ( ) 58 1.25–5 mm

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


96 44 52 0.83 Way et al, 2007 ( ) 152 1–7.5 mm 3–36 mm 256 124 132 0.86 Hadjiiski et al, 2007 ( ) 43 0.625–3 mm 2–30 mm 103 39 64 0.85

LD, low-dose computed tomography.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Effect of CADx on radiologists' characterization of lung nodules

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Observer Performance Studies for Evaluation of the Effects of CADx for Characterization of Malignant and Benign Lung Nodules in Thoracic Computed Tomography Examinations


References No. of Exams Section Thickness/Interval Nodule Sizes Total No. of Nodules Malignant Benign_A  z_ CAD System No. of Observers_A  z_ without CAD_A  z_ with CAD_P_ Value Matsuki et al, 2002 ( ) 50 2 mm <30 mm 50 25 25 0.951

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


56 1 mm 6–20 mm 56 28 28 0.831

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


0.785 0.853 .016 Shah et al, 2005 ( ) 28 Not reported

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


28 15 13

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


0.75 0.81 .02 Awai et al, 2006 ( ) 33 1–1.25 mm <30 mm 33 18 15 0.795

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Way et al, 2007 ( ) 152 1–7.5 mm 3–36 mm 256 124 132 0.86 6 thoracic rad 0.82 0.84 < .01

CADx, computer-aided diagnosis; Rad, radiologists; resid, residents.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Challenges in pulmonary embolism detection on CTPA examinations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Computerized detection of pulmonary embolism

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Studies on the Development of CADe Systems for Detection of Pulmonary Embolism in Computed Tomography Examinations


References No. of Cases No. of Positive Cases Section Thickness Presence of Artifacts and Lung Disease PE Location Total No. of PEi Sensitivity FP Rate Masutani et al, 2002 ( ) 19 11 1.5 mm No Not reported 21 (>10 mm  3  ) 85% 2.6/case Das et al, 2003 ( ) (R2) 33 33 0.75–1.25 mm Not reported Segmental and subseg 306 (186 seg, 120 subseg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


4/case Zhou et al, 2005 ( ) 14 14 1.25 mm 8 cases with extensive lung disease Proximal to subseg and subseg 163 (94 prox-subseg, 69 subseg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


14.4/case Digumarthy et al, 2006 ( ) (R2) 39 33 Not reported No Arteries ≥4 mm 270 92% 2.8/case Jeudy et al, 2006 ( ) (R2) 22 22 Not reported Not reported Segmental and subseg 251 (188 seg, 63 subseg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


1.8/case Das et al, 2006 ( ) (Siemens) 45 29 1 mm Not reported

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


213 82% median 3/case Zhou et al, 2007 ( ) 43 43 1.25 mm Yes Proximal to subseg, and subseg 435 (263 prox-subseg, 172 subseg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


24/case Schoepf et al, 2007 ( ) (R2) 36 23 1.25 mm 21 cases with lung disease Segmental and subseg

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


4.8/case Maizlin et al, 2007 ( ) (R2) 104 15 1.25 mm Lung disease not reported, severe motion cases excluded Central, segmental, subseg 45 (32 central, seg, 13 subseg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


0.93/case Buhmann et al, 2007 ( ) (Siemens) 40 18 1 mm 5 with motion artifacts, lung disease not reported Central and peripheral 212 (65 central, 147 peripheral)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


3.85/case Engelke et al, 2007 ( ) (Siemens) 56 56 0.6 mm Nonanalyzable arteries excluded Mediastinal, lobar, segmental, subsegmental 1116  ⁎  (72 mediastinal, 133 lobar, 465 seg, 455 subseg)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


4.1/case

CADe, computer-aided detection; PE, pulmonary embolism; PEi, pulmonary emboli; FP, false positive; seg, segmental arteries; subseg, subsegmental arteries; prox, proximal; R2, CADe system by R2 Technologies; Siemens, Siemens CADe system.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. American Cancer Society: Cancer facts & figures 2007. www.cancer.org/downloads/STT/CAFF2007PWSecured.pdf.

- 2\. Flehinger B.J., Kimmel M., Melamed M.R.: Survival from early lung cancer: implications for screening. Chest 1992; 101: pp. 1013-1018.


- 3\. Nesbitt J.C., Putnam J.B., Walsh G.L., et. al.: Survival in early-stage lung cancer. Ann Thorac Surg 1995; 60: pp. 466-472.


- 4\. Shah R., Sabanathan S., Richardson J., et. al.: Results of surgical treatment of stage I and II lung cancer. J Cardiovasc Surg 1996; 37: pp. 169-172.


- 5\. Frost J.K., Ball W.C., Levin M.L., et. al.: Early lung cancer detection: results of the initial (prevalence) radiologic and cytologic screening in the Johns Hopkins study. Am Rev Respir Dis 1984; 130: pp. 549-554.


- 6\. Melamed M.R., Flehinger B.J., Zaman M.B., et. al.: Screening for early lung cancer. Chest 1984; 86: pp. 44-53.


- 7\. Fontana R.S., Sanderson D.R., Woolner L.B., et. al.: Lung cancer screening: the Mayo program. J Occup Med 1986; 28: pp. 746-750.


- 8\. Kubík A.K., Parkin D.M., Zatloukal P.: Czech study on lung cancer screening: post-trial follow-up of lung cancer deaths up to year 15 since enrollment. Cancer 2000; 89: pp. 2363-2368.


- 9\. Henschke C.I., McCauley D.I., Yankelevitz D.F., et. al.: Early Lung Cancer Action Project: overall design and findings from baseline screening. Lancet 1999; 354: pp. 99-105.


- 10\. The International Early Lung Cancer Action Program Investigators: Survival of patients with stage I lung cancer detected on CT screening. N Engl J Med 2006; 355: pp. 1763-1771.


- 11\. Bach P.B., Jett J.R., Pastorino U., et. al.: Computed tomography screening and lung cancer outcomes. JAMA 2007; 297: pp. 953-961.


- 12\. Adusumilli S., Kazerooni E.A., Ojo T.C.: Screening CT for lung cancer: a study of emphysema patients being evaluated for lung volume reduction surgery. Radiology 1998; 209: pp. 222-223.


- 13\. Swensen S.J., Jett J.R., Payne W.S., et. al.: An integrated approach to evaluation of the solitary pulmonary nodule. Mayo Clinic Proc 1990; 65: pp. 173-186.


- 14\. Midthun D.E., Swensen S.J., Jett J.R.: Clinical strategies for solitary pulmonary nodule. Annu Rev Med 1992; 43: pp. 195-208.


- 15\. Ginsberg M.S., Griff S.K., Go B.D., et. al.: Pulmonary nodules resected at video-assisted thoracoscopic surgery: etiology in 426 patients. Radiology 1999; 213: pp. 277-282.


- 16\. Keagy B.A., Starek P.J.K., Murray G.F., et. al.: Major pulmonary resection for suspected but unconfirmed malignancy. Ann Thorac Surg 1984; 38: pp. 314-316.


- 17\. Dewan N.A., Shehan C.J., Reeb S.D., et. al.: Likelihood of malignancy in a solitary pulmonary nodule: Comparison of bayesian analysis and results of FDG-PET scan. Chest 1997; 112: pp. 416-422.


- 18\. Gurney J.W.: Missed lung cancer at CT: imaging findings in nine patients. Radiology 1996; 199: pp. 117-122.


- 19\. Davis S.D.: Through the “Retrospectoscope”: a glimpse of missed lung cancer at CT. Radiology 1996; 199: pp. 23-24.


- 20\. Kakinuma R., Ohmatsu H., Kaneko M., et. al.: Detection failures in spiral CT screening for lung cancer: analysis of CT findings. Radiology 1999; 212: pp. 61-66.


- 21\. White C.S., Salis A.I., Meyer C.A.: Missed lung cancer on chest radiography and computed tomography: imaging and medicolegal issues. J Thorac Imag 1999; 14: pp. 63-68.


- 22\. Proto A.V., Thomas S.R.: Pulmonary nodules studied by computed tomography. Radiology 1985; 156: pp. 149-153.


- 23\. Siegelman S.S., Khouri N.F., Leo F.P., et. al.: Solitary pulmonary nodules: CT assessment. Radiology 1986; 160: pp. 307-312.


- 24\. Swensen S.J., Silverstein M.D.: The probability of malignancy in the solitary pulmonary nodule. Arch Intern Med 1997; 157: pp. 849-855.


- 25\. Gurney J.W.: Determining the likelihood of malignancy in solitary pulmonary nodules with bayesian analysis—Part I. Radiology 1993; 186: pp. 405-413.


- 26\. Erasmus J.J., Connolly J.E., McAdams H.P., et. al.: Solitary pulmonary nodules: part I Morphological evaluation for differentiation of benign and malignant lesions. RadioGraphics 2000; 20: pp. 43-58.


- 27\. Erasmus J.J., Connolly J.E., McAdams H.P., Roggli V.L.: Solitary pulmonary nodules: part II Evaluation of the indeterminate nodule. RadioGraphics 2000; 20: pp. 59-66.


- 28\. Templeton A.W., Jansen C., Lehr J.L., et. al.: Solitary pulmonary lesions: computer aided differential diagnosis and evaluation of mathematical methods. Radiology 1967; 89: pp. 605-613.


- 29\. Wojtowicz J., Pietraszkiewicz L., Grala B.: A trial of differential diagnosis of solitary pulmonary foci on the basis of bayes's equation with the use of electronic digital computers. Pol Rev Radiol Nucl Med 1970; 34: 694-691


- 30\. Rotte K.H., Meiske W.: Results of computer-aided diagnosis of peripheral bronchial carcinoma. Radiology 1977; 125: pp. 583-586.


- 31\. Edwards F., Schaefer P.S., Callahan S., et. al.: Bayesian statistical theory in the preoperative diagnosis of pulmonary lesions. Chest 1987; 92: pp. 888-891.


- 32\. Edwards F.H., Schaefer P.S., Cohen A.J., et. al.: Use of artificial intelligence for the preoperative diagnosis of pulmonary lesions. Ann Thorac Surg 1989; 48: pp. 556-559.


- 33\. Gurney J.W.: Determining the likelihood of malignancy in solitary pulmonary nodules with bayesian analysis—Part II. Radiology 1993; 186: pp. 415-422.


- 34\. Gurney J.W.: Solitary pulmonary nodules: determining the likelihood of malignancy with neural network analysis. Radiology 1993; 196: pp. 823-829.


- 35\. Ballard D., Sklansky J.: A ladder-structured decision tree for recognizing tumors in chest radiographs. IEEE Trans Computers 1976; 25: pp. 503-513.


- 36\. Sankar P.V., Sklansky J.: A gestalt-guided heuristic boundary follower for x-ray images of lung nodules. IEEE Trans Pattern Anal Machine Intell 1982; 4: pp. 326-331.


- 37\. Lampeter W.A., Wandtke J.C.: Computerized search of chest radiographs for nodules. Invest Radiol 1986; 21: pp. 384-390.


- 38\. Giger M.L., Doi K., MacMahon H.: Image feature analysis and computer aided diagnosis in digital radiography. Med Phys 1988; 15: pp. 158-166.


- 39\. Giger M.L., Ahn N., Doi K., et. al.: Computerized detection of pulmonary nodules in digital chest images—use of morphological filters in reducing false-positive detections. Med Phys 1990; 17: pp. 861-865.


- 40\. Matsumoto T., Yoshimura H., Doi K.: Image feature analysis of false-positive diagnoses produced by automatic detection of lung nodules. Invest Radiol 1992; 27: pp. 587-597.


- 41\. Lo S.C., Lou S.L., Lin J.S., et. al.: Artificial convolution neural network techniques and applications to lung nodule detection. IEEE Trans Med Imag 1995; 14: pp. 711-718.


- 42\. Xu X.W., Doi K., Kobayashi T., et. al.: Development of an improved CAD scheme for automated detection of lung nodules in digital chest images. Med Phys 1997; 24: pp. 1395-1403.


- 43\. Vittitoe N.F., Baker J.A., Floyd C.E.: Fractal texture analysis in computer-aided diagnosis of solitary pulmonary nodules. Acad Radiol 1997; 4: pp. 96-101.


- 44\. Mao F., Qian W., Gaviria J., et. al.: Fragmentary window filtering for multiscale lung nodule detection: preliminary study. Acad Radiol 1998; 5: pp. 306-311.


- 45\. Carreira M.J., Cabello D., Penedo M.G., et. al.: Computer-aided diagnoses: automatic detection of lung nodules. Med Phys 1998; 25: pp. 1998-2006.


- 46\. Penedo M.G., Carreira M.J., Mosquera A., et. al.: Computer-aided diagnosis: a neural-network-based approach to lung nodule detection. IEEE Trans Med Imag 1998; 17: pp. 872-880.


- 47\. Suzuki K., Shiraishi J., Abe H., et. al.: False-positive reduction in computer-aided diagnostic scheme for detecting nodules in chest radiographs by means of massive training artificial neural network. Acad Radiol 2005; 12: pp. 191-201.


- 48\. Shiraishi J., Li F., Doi K.: Computer-aided diagnosis for improved detection of lung nodules by use of PA and lateral chest radiographs. Acad Radiol 2007; 14: pp. 28-37.


- 49\. Kobayashi T., Xu X.-W., MacMahon H., et. al.: Effect of a computer-aided diagnosis scheme on radiologists' performance in detection of lung nodules on radiographs. Radiology 1996; 199: pp. 843-848.


- 50\. MacMahon H., Engelmann R., Behlen F.M., et. al.: Computer-aided diagnosis of pulmonary nodules: Results of a large-scale observer test. Radiology 1999; 213: pp. 723-726.


- 51\. Osicka T., Freedman M.T., Lo S.C.B., et. al.: Computer aided detection of lung cancer on chest radiographs: differences in the interpretation time of radiologists showing vs not showing improvement with CAD. Proc SPIE 2003; 5034: pp. 483-494.


- 52\. Kakeda S., Moriya J., Sato H., et. al.: Improved detection of lung nodules with aid of computerized detection method: evaluation of a commercial computer-aided diagnosis system. Am J Roentgenol 2004; 182: pp. 505-510.


- 53\. Shiraishi J., Abe H., Li F., et. al.: Computer-aided diagnosis for the detection and classification of lung cancers on chest radiographs: ROC analysis of radiologists' performance. Acad Radiol 2006; 13: pp. 995-1003.


- 54\. Sakai S., Soeda H., Takahashi N., et. al.: Computer-aided nodule detection on digital chest radiography: validation test on consecutive t1 cases of resectable lung cancer. J Digital Imaging 2006; 19: pp. 376-382.


- 55\. Chan H.P., Sahiner B., Wagner R.F., et. al.: Classifier design for computer-aided diagnosis: effects of finite sample size on the mean performance of classical and neural network classifiers. Med Phys 1999; 26: pp. 2654-2668.


- 56\. Armato S.G., McLennan G., McNitt-Gray M.F., et. al.: Lung image database consortium: developing a resource for the medical imaging research community. Radiology 2004; 232: pp. 739-748.


- 57\. Awai K., Murao K., Ozawa A., et. al.: Pulmonary nodules at chest CT: effect of computer-aided diagnosis on radiologists' detection performance. Radiology 2004; 230: pp. 347-352.


- 58\. Marten K., Seyfarth T., Auer F., et. al.: Computer-assisted detection of pulmonary nodules: performance evaluation of an expert knowledge-based detection system in consensus reading with experienced and inexperienced chest radiologists. Euro Radiol 2004; 14: pp. 1930-1938.


- 59\. Marten K., Grillhösl A., Seyfarth T., et. al.: Computer-assisted detection of pulmonary nodules: evaluation of diagnostic performance using an expert knowledge-based detection system with variable reconstruction slice thickness settings. Euro Radiol 2005; 15: pp. 203-212.


- 60\. Li F., Arimura H., Suzuki K., et. al.: Computer-aided detection of peripheral lung cancers missed at CT: ROC analyses without and with localization. Radiology 2005; 237: pp. 684-690.


- 61\. Brown M.S., Goldin J.G., Rogers S., et. al.: Computer-aided lung nodule detection in CT results of large-scale observer test. Acad Radiol 2005; 12: pp. 681-686.


- 62\. Rubin G.D., Lyo J.K., Paik D.S., et. al.: Pulmonary nodules on multi-detector row CT scans: performance comparison of radiologists and computer-aided detection. Radiology 2005; 234: pp. 274-283.


- 63\. Das M., Muhlenbruch G., Mahnken A.H., et. al.: Small pulmonary nodules: effect of two computer-aided detection systems on radiologist performance. Radiology 2006; 241: pp. 564-571.


- 64\. Yuan R., Vos P.M., Cooperberg P.L.: Computer-aided detection in screening CT for pulmonary nodules. AJR Am J Roentgenol 2006; 186: pp. 1280-1287.


- 65\. Sahiner B., Chan H.-P., Cascade P.N., et. al.: Effect of CAD on radiologists' detection of lung nodules on thoracic CT scans: analysis of an observer performance study by nodule size. RSNA Program Book 2007; pp. 265-266.


- 66\. Henschke C.I., Yankelevitz D.F., Mateescu I., et. al.: Neural networks for the analysis of small pulmonary nodules. Clin Imaging 1997; 21: pp. 390-399.


- 67\. Kawata Y., Niki N., Ohmatsu H., et. al.: Quantitative surface characterization of pulmonary nodules based on thin-section CT images. IEEE Trans Nuclear Science 1998; 45: pp. 2132-2138.


- 68\.  Kawata Y, Niki N, Ohmatsu H, et al. Pulmonary nodule classification based on nodule retrieval from 3-d thoracic CT image database. In: Medical Image Computing and Computer-Assisted Intervention - MICCAI 2004, Part 2, Proceedings 2004; 838–846.


- 69\. McNitt-Gray M.F., Hart E.M., Wyckoff N., et. al.: A pattern classification approach to characterizing solitary pulmonary nodules imaged on high resolution CT: preliminary results. Med Phys 1999; 26: pp. 880-888.


- 70\. McNitt-Gray M.F., Wyckoff N., Sayre J.W., et. al.: The effects of co-occurrence matrix based texture parameters on the classification of solitary pulmonary nodules images on computed tomography. Comp Med Imag Graphics 1999; 23: pp. 339-348.


- 71\. Matsuki Y., Nakamura K., Watanabe H., et. al.: Usefulness of an artificial neural network for differentiating benign from malignant pulmonary nodules on high-resolution CT: evaluation with receiver operating characteristic analysis. AJR Am J Roentgenol 2002; 178: pp. 657-663.


- 72\. Lo S.C.B., Hsu L.Y., Freedman M.T., et. al.: Classification of lung nodules in diagnostic CT: an approach based on 3-D vascular features, nodule density distributions, and shape features. Proc SPIE 2003; 5032: pp. 183-189.


- 73\. Armato S.G., Altman M.B., Wilkie J.: Automated lung nodule classification following automated nodule detection on CT: a serial approach. Med Phys 2003; 30: pp. 1188-1197.


- 74\. Aoyama M., Li Q., Katsuragawa S., et. al.: Computerized scheme for determination of the likelihood measure of malignancy for pulmonary nodules on low-dose CT images. Med Phys 2003; 30: pp. 387-394.


- 75\. Suzuki K., Li F., Sone S., et. al.: Computer-aided diagnostic scheme for distinction between benign and malignant nodules in thoracic low-dose CT by use of massive training artificial neural network. IEEE Trans Med Imag 2005; 24: pp. 1138-1150.


- 76\. Li F., Aoyama M., Shiraishi J., et. al.: Radiologists' performance for differentiating benign from malignant lung nodules on high-resolution CT using computer-estimated likelihood of malignancy. AJR Am J Roentgenol 2004; 183: pp. 1209-1215.


- 77\. Li F., Li Q., Engelmann R., et. al.: Improving radiologists' recommendations with computer-aided diagnosis for management of small nodules detected by CT. Acad Radiol 2006; 13: pp. 943-950.


- 78\. Shah S.K., McNitt-Gray M.F., Rogers S.R., et. al.: Computer-aided diagnosis of the solitary pulmonary nodule. Acad Radiol 2005; 12: pp. 570-575.


- 79\. Shah S.K., McNitt-Gray M.F., De Zoysa K.R., et. al.: Solitary pulmonary nodule diagnosis on CT results of an observer study. Acad Radiol 2005; 12: pp. 496-501.


- 80\. Shah S.K., McNitt-Gray M.F., Rogers S.R., et. al.: Computer aided characterization of the solitary pulmonary nodule using volumetric and contrast enhancement features. Acad Radiol 2005; 12: pp. 1310-1319.


- 81\. Mori K., Niki N., Kondo T., et. al.: Development of a novel computer-aided diagnosis system for automatic discrimination of malignant from benign solitary pulmonary nodules on thin-section dynamic computed tomography. J Comp Assist Tomogr 2005; 29: pp. 215-222.


- 82\. Awai K., Murao K., Ozawa A., et. al.: Pulmonary nodules: estimation of malignancy at thin-section helical CT—effect of computer-aided diagnosis on performance of radiologists. Radiology 2006; 239: pp. 276-284.


- 83\. Way T.W., Hadjiiski L.M., Sahiner B., et. al.: Computer-aided diagnosis of pulmonary nodules on CT scans: segmentation and classification using 3D active contours. Med Phys 2006; 33: pp. 2323-2337.


- 84\. Way T.W., Chan H.P., Stojanovska-Nojkova J., et. al.: Effect of computer-aided diagnosis (CAD) on radiologists' characterization of lung nodules on CT: an ROC study. RSNA Program Book 2007; 2007: pp. 267.


- 85\. Hadjiiski L.M., Way T., Sahiner B., et. al.: Computer-aided diagnosis for interval change analysis of lung nodule features in serial CT examinations. Proc SPIE 2007; 6514: pp. 111-117.


- 86\. Dalen J., Alpert J.: Natural history of pulmonary embolism. Progr Cardiovasc Dis 1975; 17: pp. 257-270.


- 87\. Price D.: Thoughts on immediate care-pulmonary embolism. Anaesthesia 1976; 31: pp. 925-932.


- 88\. Remy-Jardin M., Remy J., Wattinne L., et. al.: Central pulmonary thromboembolism: diagnosis with spiral volumetric CT with the single-breath-hold technique-comparison with pulmonary angiography. Radiology 1992; 185: pp. 381-387.


- 89\. McCollough C., Zink F.: Performance evaluation of a multi-slice CT system. Med Phys 1999; 26: pp. 2223-2230.


- 90\. Rubin G.D., Paik D.S., Johnston P.C., et. al.: Measurements of the aorta and its branches with helical CT. Radiology 1998; 206: pp. 823-829.


- 91\. Stein P.: Reassessment of pulmonary angiography for the diagnosis of pulmonary embolism: relation of interpreter agreement to the order of the involved pulmonary arterial branch. Radiology 1999; 210: pp. 689-691.


- 92\. Ghaye B.: Peripheral pulmonary arteries: how far in the lung does multi-detector row spiral CT allow analysis?. Radiology 2001; 219: pp. 629-636.


- 93\. Raptopoulos V., Boiselle P.: Multi-detector row spiral CT pulmonary angiography: comparison with single-detector row spiral CT. Radiology 2001; 221: pp. 606-613.


- 94\. Schoepf U.J., Holzknecht N., Helmberger T.K., et. al.: Subsegmental pulmonary emboli: improved detection with thin-collimation multi-detector row spiral CT. Radiology 2002; 222: pp. 483-490.


- 95\. Diffin D., Leyendecker J., Johnson S., et. al.: Effect of anatomic distribution of pulmonary emboli on interobserver agreement in the interpretation of pulmonary angiography. Am J Roentgenol 1998; 171: pp. 1085-1089.


- 96\. Stein P.D., Fowler S.E., Goodman L.R., et. al.: Multidetector computed tomography for acute pulmonary embolism. N Engl J Me 2006; 354: pp. 2317-2327.


- 97\. Goodman L., Curtin J., Mewissen M.: Detection of pulmonary embolism in patients with unsolved clinical and scintigraphic diagnosis: helical CT versus angiography. AJR Am J Roentgenol 1995; 164: pp. 1369-1374.


- 98\. Drucker E., Rivitz S., Shepard J.: Acute pulmonary embolism: assessment of helical CT for diagnosis. Radiology 1998; 209: pp. 235-241.


- 99\. Perrier A., Howarth N., Didier D., et. al.: Performance of helical computed tomography in unselected outpatients with suspected pulmonary embolism. Ann Intern Med 2001; 135: pp. 88-97.


- 100\. Schoepf U.J., Goldhaber S.Z., Costello P.: Spiral computed tomography for acute pulmonary embolism. Circulation 2004; 109: pp. 2160-2167.


- 101\. Schoepf U.J., Costello P.: CT angiography for diagnosis of pulmonary embolism: state of the art. Radiology 2004; 230: pp. 329-337.


- 102\. Hull R., Raskob G., Ginsberg J., et. al.: A noninvasive strategy for the treatment of patients with suspected pulmonary embolism. Arch Intern Med 1994; 154: pp. 289-297.


- 103\. Oser R., Zuckerman D., Gutierrez F., Brink J.: Anatomic distribution of pulmonary emboli at pulmonary angiography: implications for cross sectional imaging. Radiology 1996; 199: pp. 31-35.


- 104\. Patriquin L., Khorasani R., Polak J.: Correlation of diagnostic imaging and subsequent autopsy findings in patients with pulmonary embolism. Am J Respir Crit Care Med 1998; 171: pp. 347-349.


- 105\. Wu A.S., Pezzullo J.A., Cronan H.J., et. al.: CT pulmonary angiography: quantification of pulmonary embolus as a predictor of patient outcome—initial experience. Radiology 2004; 230: pp. 831-835.


- 106\. Bankier A., Janata K., Fleischmann D., et. al.: Severity assessment of acute pulmonary embolism with spiral CT: evaluation of two modified angiographic scores and comparison with clinical data. J Thorac Imaging 1997; 12: pp. 150-158.


- 107\. Qanadli S.D., Hajjam M.E., Vieillard-Baron A., et. al.: New CT index to quantify arterial obstruction in pulmonary embolism: comparison with angiographic index and echocardiography. AJR Am J Roentgenol 2001; 176: pp. 1415-1420.


- 108\. Mastora I., Remy-Jardin M., P M., et. al.: Severity of acute pulmonary embolism: evaluation of a new spiral CT angiographic score in correlation with echocardiographic data. Eur Radiol 2003; 13: pp. 29-35.


- 109\. Wood K., Visani L., De Rosa M.: Major pulmonary embolism: review of a pathophysiologic approach to the golden hour of hemodynamically signification pulmonary embolism. Chest 2002; 121: pp. 877-905.


- 110\. Araoz P.A., Gotway M.B., Trowbridge R.L., et. al.: Helical CT pulmonary angiography predictors of in-hospital morbidity and mortality in patients with acute pulmonary embolism. J Thorac Imaging 2003; 18: pp. 207-216.


- 111\. Coche E., Verschuren F., Keyeux A., et. al.: Diagnosis of acute pulmonary embolism in outpatients: comparison of thin-collimation multi–detector row spiral CT and planar ventilation-perfusion scintigraphy. Radiology 2003; 229: pp. 757-765.


- 112\. Patel S., Kazerooni E., Cascade P.: Pulmonary embolism: optimization of small pulmonary artery visualization at multi-detector row CT. Radiology 2003; 227: pp. 455-460.


- 113\. Sostman H.D., Stein P.D., Gottschalk A., et. al.: Results of the NIH/NHLBI PIOPED II study: is spiral CT the best and only test for suspected pulmonary embolism?. RSNA Program Book 2004; pp. 55.


- 114\. Ko J.P., Naidich D.P.: Computer-aided diagnosis and the evaluation of lung disease. J Thorac Imaging 2004; 19: pp. 136-155.


- 115\. Masutani Y., MacMahon H., Doi K.: Computerized detection of pulmonary embolism in spiral CT angiography based on volumetric image analysis. IEEE Trans Med Imag 2002; 21: pp. 1517-1523.


- 116\. Das M., Schneider A.C., Schoepf U.O., et. al.: Computer-aided diagnosis of peripheral pulmonary emboli. RSNA Program Book 2003; pp. 351-352.


- 117\. Digumarthy S., Kagay C., Legasto A., et. al.: Computer-aided detection (CAD) of acute pulmonary emboli: evaluation in patients without significant pulmonary disease. RSNA Program Book 2006; pp. 255.


- 118\. Jeudy J., Flukinger T., White C.: Evaluation of pulmonary embolism using an automated computer-aided detection tool. RSNA Program Book 2006; pp. 255.


- 119\. Schoepf U.J., Schneider A.C., Das M., et. al.: Pulmonary embolism: computer-aided detection at multidetector row spiral computed tomography. J Thorac Imag 2007; 22: pp. 319-323.


- 120\. Maizlin Z.V., Vos P.M., Godoy M.B., et. al.: Computer-aided detection of pulmonary embolism on CT angiography: initial experience. J Thorac Imag 2007; 22: pp. 324-329.


- 121\. Das M., Salganicoff M., Bakai A., Mühlenbruch G., Günther R.W., Wildberger J.: Computer-aided detection of pulmonary embolism: Assessment of sensitivity with regard to vessel segments.RSNA Program Book 2006.2006.RSNAChicago, IL:pp. 487.


- 122\. Buhmann S., Herzog P., Liang J., et. al.: Clinical evaluation of a computer-aided diagnosis (CAD) prototype for the detection of pulmonary embolism. Acad Radiol 2007; 14: pp. 651-658.


- 123\. Engelke C., Schmidt S., Bakai A., et. al.: Computer-assisted detection of pulmonary embolism: performance evaluation in consensus with experienced and inexperienced chest radiologists. Euro Radiol 2008; 18: pp. 298-307.


- 124\. Zhou C., Chan H.P., Patel S., et. al.: Preliminary investigation of computer-aided detection of pulmonary embolism in 3D computed tomographic pulmonary angiography (CTPA) images. Acad Radiol 2005; 12: pp. 782-792.


- 125\. Zhou C., Hadjiiski L.M., Sahiner B., et. al.: Computerized detection of pulmonary embolism in 3D computed tomographic (CT) images: vessel tracking and segmentation techniques. Proc SPIE 2003; 5032: pp. 1613-1620.


- 126\.  Zhou C, Hadjiiski LM, Patel S, et al. Computerized detection of pulmonary embolism in 3D computed tomographic (CT) images. RSNA 2003, Chicago, November 30–December 5, 2003; 51.


- 127\.  Zhou C, Chan H-P, Patel S, et al. Computerized detection of pulmonary embolism in 16-slice computed tomographic pulmonary angiography (CTPA) images. RSNA 2004, November 28–December 3, Chicago, 2004; 350.


- 128\. Zhou C., Chan H.P., Hadjiiski L.M., et. al.: Automated detection of pulmonary embolism (PE) in computed tomographic pulmonary angiographic (CTPA) images: multiscale hierarchical expectation-maximization segmentation of vessels and PEs. Proc SPIE 2007; 6514: pp. 2F1-2F8.


- 129\. Kim K.G., Goo J.M., Kim J.H., et. al.: Computer-aided diagnosis of localized ground-glass opacity in the lung at CT: initial experience. Radiology 2005; 237: pp. 657-661.


- 130\. Giger M.L., Bae K.T., MacMahon H.: Computerized detection of pulmonary nodules in computed tomography images. Invest Radiol 1994; 29: pp. 459-465.


- 131\. Kanazawa K., Kawata Y., Niki N., et. al.: Computer-aided diagnosis for pulmonary nodules based on helical CT images. Comp Med Imag Graphics 1998; 22: pp. 157-167.


- 132\. Armato S.G., Giger M.L., MacMahon H.: Automated detection of lung nodules in CT scans: preliminary results. Med Phys 2001; 28: pp. 1552-1561.


- 133\. Ko J.P., Betke M.: Chest CT: automated nodule detection and assessment of change over time-preliminary experience. Radiology 2001; 218: pp. 267-273.


- 134\. Brown M.S., McNitt-Gray M.F., Goldin J.G., et. al.: Patient-specific models for lung nodule detection and surveillance in CT images. IEEE Trans Med Imag 2001; 20: pp. 1242-1250.


- 135\. Lee Y., Hara T., Fujita H., et. al.: Automated detection of pulmonary nodules in helical CT images based on an improved template-matching technique. IEEE Trans Med Imag 2001; 20: pp. 595-604.


- 136\. Armato S., Li F., Giger M., et. al.: Lung cancer: performance of automated lung nodule detection applied to cancers missed in a CT screening program. Radiology 2002; 225: pp. 685-692.


- 137\. Wormanns D., Fiebich M., Saidi M., et. al.: Automatic detection of pulmonary nodules at spiral CT: clinical application of a computer-aided diagnosis system. Euro Radiol 2002; 12: pp. 1052-1057.


- 138\. Gurcan M.N., Sahiner B., Petrick N., et. al.: Lung nodule detection on thoracic computed tomography images: preliminary evaluation of a computer-aided diagnosis system. Med Phys 2002; 29: pp. 2552-2558.


- 139\. Suzuki K., Armato S.G., Li F., et. al.: Massive training artificial neural network (mtann) for reduction of false positives in computerized detection of lung nodules in low-dose computed tomography. Med Phys 2003; 30: pp. 1602-1617.


- 140\. Brown M.S., Goldin J.G., Suh R.D., et. al.: Lung micronodules: automated method for detection at thin-section CT—initial experience. Radiology 2003; 226: pp. 256-262.


- 141\. Zhao B.S., Gamsu G., Ginsburg M.S., et. al.: Automatic detection of small lung nodules on CT utilizing a local density maximum algorithm. J Appl Clin Med Phys 2003; 4: pp. 248-260.


- 142\. Goo J.M., Lee J.W., Lee H.J., et. al.: Automated lung nodule detection at low-dose CT: preliminary experience. Korean J Radiol 2003; 4: pp. 211-216.


- 143\. Paik D.S., Beaulieu C.F., Rubin G.D., et. al.: Surface normal overlap: a computer-aided detection algorithm with application to colonic polyps and lung nodules in helical CT. IEEE Trans Med Imag 2004; 23: pp. 661-675.


- 144\. Lee J.W., Goo J.M., Lee H.J., et. al.: The potential contribution of a computer-aided detection system for lung nodule detection in multidetector row computed tomography. Invest Radiol 2004; 39: pp. 649-655.


- 145\. Arimura H., Katsuragawa S., Suzuki K., et. al.: Computerized scheme for automated detection of lung nodules in low-dose computed tomography images for lung cancer screening. Acad Radiol 2004; 11: pp. 617-629.


- 146\. McCulloch C.C., Kaucic R.A., Mendonca P.R.S., et. al.: Model-based detection of lung nodules in computed tomography exams—thoracic computer-aided diagnosis. Acad Radiol 2004; 11: pp. 258-266.


- 147\. Ge Z., Sahiner B., Chan H.P., et. al.: Computer aided detection of lung nodules: False positive reduction using a 3D gradient field method and 3D ellipsoid fitting. Med Phys 2005; 32: pp. 2443-2454.


- 148\. Bae K.T., Kim J.-S., Na Y.-H., Kim K.G., Kim J.-H.: Pulmonary nodules: automated detection on CT images with morphologic matching algorithm—preliminary results. Radiology 2005; 236: pp. 286-293.


- 149\. Lin D.T., Yan C.R., Chen W.T.: Autonomous detection of pulmonary nodules on CT images with a neural network-based fuzzy system. Comp Med Imag Graphics 2005; 29: pp. 447-458.


- 150\. Kim J.-S., Kim J.-H., Cho G., et. al.: Automated detection of pulmonary nodules on CT images: effect of section thickness and reconstruction interval—initial results. Radiology 2005; 236: pp. 295-299.


- 151\. Armato S.G., Roy A.S., MacMahon H., et. al.: Evaluation of automated lung nodule detection on low-dose computed tomography scans from a lung cancer screening program. Acad Radiol 2005; 12: pp. 337-346.


- 152\. Marten K., Engelke C., Seyfarth T., et. al.: Computer-aided detection of pulmonary nodules: influence of nodule characteristics on detection performance. Clin Radiol 2005; 60: pp. 196-206.


- 153\. Peldschus K., Herzog P., Wood S.A., et. al.: Computer-aided diagnosis as a second reader—spectrum of findings in CT studies of the chest interpreted as normal. Chest 2005; 128: pp. 1517-1523.


- 154\. Roy A.S., Samuel G. Armato, Wilson A., et. al.: Automated detection of lung nodules in CT scans: false-positive reduction with the radial-gradient index. Med Phys 2006; 33: pp. 1133-1140.


- 155\. Boeroezky L., Zhao L.Y., Lee K.P.: Feature subset selection for improving the performance of false positive reduction in lung nodule CAD. IEEE Trans Inform Technol Biomed 2006; 10: pp. 504-511.


- 156\. Sahiner B., Hadjiiski L.M., Chan H.P., et. al.: Computerized lung nodule detection on screening CT scans: performance on juxta-pleural and internal nodules. Proc SPIE 2006; 6144: pp. 5S1-5S6.


- 157\. Sahiner B., Hadjiiski L.M., Chan H.P., et. al.: Effect of CAD on radiologists' detection of lung nodules on thoracic CT scans: observer performance study. Proc SPIE 2007; 6515: pp. 1D1-1D7.


- 158\. Wang P., DeNunzio A., Okunieff P., et. al.: Lung metastases detection in CT images using 3D template matching. Med Phys 2007; 34: pp. 915-922.