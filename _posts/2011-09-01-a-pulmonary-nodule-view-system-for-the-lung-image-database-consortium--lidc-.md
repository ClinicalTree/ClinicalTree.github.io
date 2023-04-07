---
title: A Pulmonary Nodule View System for the Lung Image Database Consortium (LIDC)
author: [CL_AT_HongliLinPhD,CL_AT_ZhenchengChenPhD,CL_AT_WeishengWangMD]
date: 2011-09-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 18, Issue 9]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to develop a pulmonary nodule viewing system to visualize and retrieve data from the Lung Image Database Consortium.

## Materials and Methods

The pulmonary nodule viewing system, developed using Microsoft C++ and the .NET 2.0 Framework, is composed of a clinical information integrator, a nodule viewer, a search engine, and a data model.

## Results

A pulmonary nodule viewing system using Lung Image Database Consortium data for computer-aided diagnosis research and training purpose was developed.

## Conclusions

The pulmonary nodule viewing system can be used to build a pulmonary nodule database for computer-aided diagnosis research and medical education. It can also be used to view and retrieve large data sets efficiently.

In the continuing battle against lung cancer, computed tomographic (CT) scanning has been found to increase the detection rate of pulmonary nodules . Much work has been done to develop computer-aided detection and diagnosis (CAD) systems for pulmonary nodules on CT imaging . Training and testing systems have also been considered to educate residents and fellows in lung cancer image interpretation . Reference databases with large numbers of cases containing representative types of nodules are vital for the development of robust CAD systems and training systems. However, these databases are very expensive to create. At present, there are only a limited number of public available databases to support research in CAD. The National Cancer Institute’s Lung Image Database Consortium (LIDC) is one of these. The development of the LIDC has led to a large amount of research based on the image sets that are provided to users. Meyer et al investigated the effects of radiologist agreement on the development of a “ground truth” and the subsequent impact on CAD performance. Reeves et al compared volumes computed using their research system with those derived from the LIDC archive. LIDC data have also been used to train and validate CAD algorithms , as well as to develop a pulmonary nodule image retrieval system .

However, there are still some barriers that prevent LIDC data from being used efficiently. First, the LIDC data lack a unified data model. At present, the data are composed of Digital Imaging and Communications in Medicine (DICOM) images, annotation files, a nodule size report, and a diagnosis report. The annotation files are in extensible markup language (XML) format. The nodule size report and the diagnosis data report are Excel spreadsheets (Microsoft Corporation, Redmond, WA). As a result, it is difficult to access this valuable resource efficiently, because of the lack of a unified data view.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Summary of Subjective Assessment Ratings and Associated Descriptive Terms of Nodule Characteristics Provided by Lung Image Database Consortium Radiologists


Characteristic Description Ratings and Terms Calcification Calcification appearance in the nodule

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

- 6.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Internal structure Internal composition of the nodule (soft tissue, fluid, fat, air)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Subtlety Difficulty in detection (refers to the contrast between the lung and its surroundings)

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


Lobulation Whether a lobular shape is apparent from the margin or not

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Margin How well defined the margins of the nodule are

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Sphericity The three-dimensional shape of the nodule in terms of its roundness

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Malignancy Likelihood of malignancy of the nodule

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


Texture Internal texture of the nodule

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


Spiculation Degree to which the nodule has spicules, spikelike structures, along its border

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Entity relational diagram.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APulmonaryNoduleViewSystemfortheLungImageDatabaseConsortiumLIDC/0_1s20S1076633211002042.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Information Integrator

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Nodule Viewer

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Search Engine

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Nodule search window.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APulmonaryNoduleViewSystemfortheLungImageDatabaseConsortiumLIDC/1_1s20S1076633211002042.jpg)

![Figure 3, Search result window.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APulmonaryNoduleViewSystemfortheLungImageDatabaseConsortiumLIDC/2_1s20S1076633211002042.jpg)

![Figure 4, Nodule viewer.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APulmonaryNoduleViewSystemfortheLungImageDatabaseConsortiumLIDC/3_1s20S1076633211002042.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Henschke C.I., McCauley D.I., Yankelevitz D.F., et. al.: Early lung cancer action project: overall design and findings from baseline screening. Lancet 1999; 354: pp. 99-105.


- 2\. Temesguen M., Russell C.H., Steven K.R.: A new computationally efficient CAD system for pulmonary nodule detection in CT imagery. Med Image Anal 2010; 14: pp. 390-406.


- 3\. Daw T.L., Yan C.R., Chen W.T.: Autonomous detection of pulmonary nodules on CT images with a neural network-based fuzzy system. Comput Med Imaging Graph 2005; 29: pp. 447-458.


- 4\. Way T., Chan H.P., Hadjiiski L., et. al.: Computer-aided diagnosis of lung nodules on CT scans. Acad Radiol 2010; 17: pp. 323-332.


- 5\. Retico A., Delogu P., Fantacci M.E., et. al.: Lung nodule detection in low-dose and thin-slice computed tomography. Comput Biol Med 2008; 38: pp. 525-534.


- 6\. Tabakov S., Roberts V.C., Jonsson B.A., et. al.: W. Med Eng Phys 2005; 27: pp. 591-598.


- 7\. Lison T., Günther S., Ogurol Y., et. al.: VISION2003: virtual learning units for medical training and education. Int J Med Inform 2004; 73: pp. 165-172.


- 8\. Armato S.G., McLennan G., McNitt-Gray M.F., et. al., Lung Image Database Consortium Research Group: Lung Image Database Consortium: developing a resource for the medical imaging research community. Radiology 2004; 232: pp. 739-748.


- 9\. Meyer C.R., Johnson T.D., McLennan G., et. al.: Evaluation of lung MDCT nodule annotation across radiologists and methods. Acad Radiol 2006; 13: pp. 1254-1265.


- 10\. Reeves A.P., Biancardi A.M., Apanasovich T.V., et. al.: The Lung Image Database Consortium (LIDC): a comparison of different size metrics for pulmonary nodule measurements. Acad Radiol 2007; 14: pp. 1475-1485.


- 11\. Lam M., Disney T., Raicu D.S., et. al.: BRISC—an open source pulmonary nodule image retrieval framework. J Digit Imaging 2007; 20: pp. 63-71.


- 12\. McNitt-Gray M.F., Armato S.G., Meyer C.R., et. al.: The Lung Database Consortium (LIDC) data collection process for nodule detection and annotation. Acad Radiol 2007; 14: pp. 1464-1474.