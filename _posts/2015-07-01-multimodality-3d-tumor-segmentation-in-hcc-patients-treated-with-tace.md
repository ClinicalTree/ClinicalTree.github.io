---
title: Multimodality 3D Tumor Segmentation in HCC Patients Treated with TACE
author: [CL_AT_ZhijunWangMDPhD,CL_AT_JuliusChapiroMD,CL_AT_RdigerSchernthanerMD,CL_AT_RafaelDuranMD,CL_AT_RongxinChenMDPhD,CL_AT_JeanFranoisGeschwindMD,CL_AT_MingDeLinPhD]
date: 2015-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 22, Issue 7]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

To validate the concordance of a semiautomated multimodality lesion segmentation technique between contrast-enhanced magnetic resonance imaging (CE-MRI), cone-beam computed tomography (CBCT), and multidetector CT (MDCT) in patients with hepatocellular carcinoma (HCC) treated with transarterial chemoembolization (TACE).

## Materials and Methods

This retrospective analysis included 45 patients with unresectable HCC who underwent baseline CE-MRI within 1 month before the treatment, intraprocedural CBCT during conventional TACE, and MDCT within 24 hours after TACE. Fourteen patients were excluded because of atypical lesion morphology, portal vein invasion, or small lesion size which precluded sufficient lesion visualization. Thirty-one patients with a total of 40 target lesions were included into the analysis. A tumor segmentation software, based on non-Euclidean geometry and theory of radial basis functions, was used to allow for the segmentation of target lesions in 3D on all three modalities. The algorithm created image-based masks located in a 3D region whose center and size were defined by the user, yielding the nomenclature “semiautomatic”. On the basis of that, tumor volumes on all three modalities were calculated and compared using a linear regression model ( _R_ 2 values). Residual plots were used to analyze drift and variance of the values.

## Results

The mean value of tumor volumes was 18.72 ± 19.13 cm  3 (range, 0.41–59.16 cm  3 ) on CE-MRI, 21.26 ± 21.99 cm  3 (range, 0.62–86.82 cm  3 ) on CBCT, and 19.88 ± 20.88 cm  3 (range, 0.45–75.24 cm  3 ) on MDCT. The average volumes of the tumor were not significantly different between CE-MRI and DP-CBCT, DP-CBCT and MDCT, MDCT and CE-MRI ( _P_ = .577, .770, and .794, respectively). A strong correlation between volumes on CE-MRI and CBCT, CBCT and MDCT, MDCT and CE-MRI was observed ( _R_ 2 = 0.974, 0.992 and 0.983, respectively). When plotting the residuals, no drift was observed for all methods showing deviations of no >10% of absolute volumes (in cm  3 ).

## Conclusions

A semiautomated 3D segmentation of HCC lesions treated with TACE provides high volumetric concordance across all tested imaging modalities.

Locoregional therapies (ie, conventional transarterial chemoembolization \[cTACE\]) represent the mainstay of therapy for patients with unresectable primary and some secondary liver malignancies. Because treatment recommendations are usually based on measurements made on cross-sectional imaging, accurate and workflow-efficient evaluation of tumor size on baseline imaging and radiologic tumor response assessment on follow-up imaging constitute important aspects of the therapeutic concept . There are three accepted methods to assess tumor response to TACE: Response Evaluation Criteria in Solid Tumor \[RECIST\], European Association for the Study of the Liver \[EASL\] guidelines, and modified RECIST \[mRECIST\]. The diameter-based RECIST is used to measure changes in overall tumor size. The bidimensional EASL is used to measure the area of enhancement, and the more recently introduced unidimensional mRECIST measures the maximal diameter of tumor enhancement . The advent of workflow-efficient and clinically practicable segmentation-based 3D quantification of tumor volumes has been confirmed as technically feasible, highly reproducible, and reader independent. However, no evidence exists until today for the intermodality concordance between these systems. Before their full clinical introduction, these methods must be shown as accurate and reproducible across all cross-sectional imaging modalities. The purpose of our study was thus to validate the concordance of a semiautomated multimodality lesion segmentation technique on contrast-enhanced magnetic resonance imaging (CE-MRI), C-arm cone-beam computed tomography (CBCT), and multidetector CT (MDCT) in patients with hepatocellular carcinoma (HCC) treated with TACE.

## Material and methods

## Patient Study Selection

This was a single-institution retrospective study. Health Insurance Portability and Accountability Act compliant and institutional review board approved the study. All patients were provided with informed consent before cTACE in the study. Diagnosis of HCC was confirmed by liver biopsy or the lesion presented with typical features on dynamic contrast-enhanced CT or MR cross-sectional imaging (hypervascularity in the arterial phase and washout in the venous phase) and an α-fetoprotein level of ≥200 ng/mL. Patients with unresectable HCC were evaluated and treated with cTACE after discussion at the multidisciplinary liver tumor conference. Eligibility criteria for cTACE were as follows: focal or multifocal unresectable HCC; Child-Pugh classification A or B; Eastern Cooperative Oncology Group performance status was 0 or 1, and no contraindication to contrast medium. Patients with tumor burden of >70% presence of extrahepatic disease or complete tumor occlusion of the portal vein were excluded. The eligibility criteria for assessment of the treated target lesions included all patients 1) with dynamic CE-MRI within 4 weeks before cTACE, intraprocedural dual-phase CBCT (DP-CBCT), and MDCT 24 hours after cTACE; 2) with well visualized target lesion in all the three modalities; 3) with clear border between tumor and liver tissue. Targeted lesions that were not visualized well (ie, atypical lesion morphology like that found in infiltrative disease) or with insufficient imaging on any modality were excluded from our study.

## Preprocedural CE-MRI Technique

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Intraprocedural Dual-Phase CBCT Technique

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Transcatheter Arterial Chemoembolization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## MDCT Technique

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Semiautomatic Tumor Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Three-dimensional semiautomatic segmentation of the HCC tumor on a representative case. Tumor at a representative axial slice level was visualized well on CE-MRI, DP-CBCT, and MDCT (a,b,c) . Three-dimensional segmentation volume rendering on the same slice (d,e,f) . The tumor volumes on CE-MRI, CBCT, and MDCT were 3.85, 4.47, and 3.97 cm 3 , respectively. CE-MRI, contrast-enhanced magnetic resonance imaging; DP-CBCT, dual-phase cone-beam computed tomography; HCC, hepatocellular carcinoma; MDCT, multidetector CT.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/Multimodality3DTumorSegmentationinHCCPatientsTreatedwithTACE/0_1s20S1076633215001063.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Patient Demographics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Tumor Volume on Preprocedural CE-MRI, DP-CBCT, and MDCT

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Tumor Volume Comparison on Three Modalities


Variable Tumor Volume (cm  3  )_P_ Value CE-MRI and CBCT 18.72 ± 19.13 21.26 ± 21.99 0.577 CBCT and MDCT 21.26 ± 21.99 19.88 ± 20.88 0.770 MDCT and CE-MRI 19.88 ± 20.88 18.72 ± 19.13 0.794

Data were expressed as means ± standard deviations.


![Figure 2, Comparison of tumor volumes between CE-MR, DP-CBCT, and MDCT. (a1,b1,c1) The correlation of CE-MRI and DP-CBCT, DP-CBCT and MDCT, and MDCT and CE-MRI. (a2,b2,c2) The residual plots between CE-MRI, DP-CBCT, and MDCT. CE-MRI, contrast-enhanced magnetic resonance imaging; DP-CBCT, dual-phase cone-beam computed tomography; HCC, hepatocellular carcinoma; MDCT, multidetector CT.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/Multimodality3DTumorSegmentationinHCCPatientsTreatedwithTACE/1_1s20S1076633215001063.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Bruix J., Sherman M., Practice Guidelines Committee AAftSoLD: Management of hepatocellular carcinoma. Hepatology 2005; 42: pp. 1208-1236.


- 2\. Gonzalez-Guindalini F.D., Botelho M.P., Harmath C.B., et. al.: Assessment of liver tumor response to therapy: role of quantitative imaging. Radiographics : a review publication of the Radiological Society of North America, Inc 2013; 33: pp. 1781-1800.


- 3\. Vossen J.A., Buijs M., Kamel I.R.: Assessment of tumor response on MR imaging after locoregional therapy. Techniques in vascular and interventional radiology 2006; 9: pp. 125-132.


- 4\. Kamel I.R., Liapi E., Reyes D.K., et. al.: Unresectable hepatocellular carcinoma: serial early vascular and cellular changes after transarterial chemoembolization as detected with MR imaging. Radiology 2009; 250: pp. 466-473.


- 5\. Therasse P., Arbuck S.G., Eisenhauer E.A., et. al.: New guidelines to evaluate the response to treatment in solid tumors. European Organization for Research and Treatment of Cancer, National Cancer Institute of the United States, National Cancer Institute of Canada. Journal of the National Cancer Institute 2000; 92: pp. 205-216.


- 6\. Loffroy R., Lin M., Rao P., et. al.: Comparing the detectability of hepatocellular carcinoma by C-arm dual-phase cone-beam computed tomography during hepatic arteriography with conventional contrast-enhanced magnetic resonance imaging. Cardiovascular and interventional radiology 2012; 35: pp. 97-104.


- 7\. Loffroy R., Lin M., Yenokyan G., et. al.: Intraprocedural C-arm dual-phase cone-beam CT: can it be used to predict short-term response to TACE with drug-eluting beads in patients with hepatocellular carcinoma?. Radiology 2013; 266: pp. 636-648.


- 8\. Chapiro J., Lin M., Duran R., et. al.: Assessing tumor response after loco-regional liver cancer therapies: the role of 3D MRI. Expert Review of Anticancer Therapy 2014; 15: pp. 199-205.


- 9\. Pellerin O., Lin M., Bhagat N., et. al.: Comparison of semi-automatic volumetric VX2 hepatic tumor segmentation from cone beam CT and multi-detector CT with histology in rabbit models. Academic radiology 2013; 20: pp. 115-121.


- 10\. Tacher V., Lin M., Chao M., et. al.: Semiautomatic volumetric tumor segmentation for hepatocellular carcinoma: comparison between C-arm cone beam computed tomography and MRI. Academic radiology 2013; 20: pp. 446-452.


- 11\. Lin M., Pellerin O., Bhagat N., et. al.: Quantitative and volumetric European Association for the Study of the Liver and Response Evaluation Criteria in Solid Tumors measurements: feasibility of a semiautomated software method to assess tumor response after transcatheter arterial chemoembolization. Journal of vascular and interventional radiology: JVIR 2012; 23: pp. 1629-1637.


- 12\. Prasad S.R., Jhaveri K.S., Saini S., et. al.: CT tumor measurement for therapeutic response assessment: comparison of unidimensional, bidimensional, and volumetric techniques initial observations. Radiology 2002; 225: pp. 416-419.


- 13\. Sohaib S.A., Turner B., Hanson J.A., et. al.: CT assessment of tumour response to treatment: comparison of linear, cross-sectional and volumetric measures of tumour size. The British journal of radiology 2000; 73: pp. 1178-1184.


- 14\. Bonekamp S., Halappa V.G., Geschwind J.F., et. al.: Unresectable hepatocellular carcinoma: MR imaging after intraarterial therapy. Part II. Response stratification using volumetric functional criteria after intraarterial therapy. Radiology 2013; 268: pp. 431-439.


- 15\. Bonekamp S., Li Z., Geschwind J.F., et. al.: Unresectable hepatocellular carcinoma: MR imaging after intraarterial therapy. Part I. Identification and validation of volumetric functional response criteria. Radiology 2013; 268: pp. 420-430.


- 16\. Chapiro J., Wood L., Lin M., et. al.: Radiologic-pathologic analysis of contrast-enhanced and diffusion-weighted MR imaging in patients with HCC after TACE: diagnostic accuracy of 3D quantitative image analysis. Radiology 2014; 273: pp. 746-758.


- 17\. Mahr A., Levegrun S., Bahner M.L., et. al.: Usability of semiautomatic segmentation algorithms for tumor volume determination. Investigative radiology 1999; 34: pp. 143-150.


- 18\. Ray S., Hagge R., Gillen M., et. al.: Comparison of two-dimensional and three-dimensional iterative watershed segmentation methods in hepatic tumor volumetrics. Medical physics 2008; 35: pp. 5869-5881.


- 19\. Yim P.J., Vora A.V., Raghavan D., et. al.: Volumetric analysis of liver metastases in computed tomography with the fuzzy C-means algorithm. Journal of computer assisted tomography 2006; 30: pp. 212-220.


- 20\. Zhao B., Schwartz L.H., Jiang L., et. al.: Shape-constraint region growing for delineation of hepatic metastases on contrast-enhanced computed tomograph scans. Investigative radiology 2006; 41: pp. 753-762.


- 21\. Hermoye L., Laamari-Azjal I., Cao Z., et. al.: Liver segmentation in living liver transplant donors: comparison of semiautomatic and manual methods. Radiology 2005; 234: pp. 171-178.