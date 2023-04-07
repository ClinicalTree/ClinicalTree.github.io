---
title: Integration of a Zero-footprint Cloud-based Picture Archiving and Communication System with Customizable Forms for Radiology Research and Education
author: [CL_AT_JasonHostetterMD,CL_AT_NishanthKhannaMD,CL_AT_JacobCMellMD]
date: 2018-06-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 25, Issue 6]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The purpose of this study was to integrate web-based forms with a zero-footprint cloud-based Picture Archiving and Communication Systems (PACS) to create a tool of potential benefit to radiology research and education.

## Materials and Methods

Web-based forms were created with a front-end and back-end architecture utilizing common programming languages including Vue.js, Node.js and MongoDB, and integrated into an existing zero-footprint cloud-based PACS.

## Results

The web-based forms application can be accessed in any modern internet browser on desktop or mobile devices and allows the creation of customizable forms consisting of a variety of questions types. Each form can be linked to an individual DICOM examination or a collection of DICOM examinations.

## Conclusions

Several uses are demonstrated through a series of case studies, including implementation of a research platform for multi-reader multi-case (MRMC) studies and other imaging research, and creation of an online Objective Structure Clinical Examination (OSCE) and an educational case file.

## Introduction

Cloud-based picture archiving and communication systems (PACSs) have been widely available for the past several years. The National Institute of Standards and Technology broadly defines cloud computing as a “model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources” . Such a rapidly elastic framework offers several advantages to a PACS implementation, including offloading of server considerations to the cloud provider with resultant reliable and maintenance-free performance, and ensuring broad compatibility across computing platforms and handheld devices.

The functionality of a cloud-based PACS can potentially be further enhanced by integrating web forms to allow easily customizable data collection linked to each DICOM (Digital Imaging and Communications in Medicine) examination. Web forms are commonly used in research, education, and administration. However, the integration of images into web-based forms such as Google Forms (Google Inc., Mountain View, MA) or SurveyMonkey (San Mateo, CA) is relatively primitive, and to our knowledge, there is no online form provider that supports the DICOM standard and allows standard PACS functionality. Combining a zero-footprint PACS with web-based forms may offer unique benefits to several research and educational tasks. Additionally, universal compatibility among desktop and handheld devices could facilitate studies or educational tasks tailored for mobile computing and more general applications.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Integration of Forms with Cloud-based PACS

## Cloud-based PACS

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 1


DICOM Tags That Are Anonymized


DICOM Tag Name of DICOM Tag 0008,0030–0033 Study, series, acquisition, content time 0008,0050 Accession number 0008,0080–1010 Institution name, address, referrer, station name 0008,1040–1070 Institution department, physician of record, operator's name 0010,0010–2154 Patient's name, ID, issuer of patient ID, birth date, sex, other patient's ID, patient's age, patient's size and weight, ethnic group, pregnancy status, telephone number, religious preference, military rank, branch of service 0020,3404 Modifying device manufacturer 0020,4000 Image comments 0028,4000 Image presentation comments All tags starting with the following group numbers are removed: 0019, 0029, 0031–0033, 0035, 0038, 0043, 0045, 0049, 0051, 0053, 0060, 0070, 0073, 4008 All private, nonstandard tags are removed (any group number starting with an odd number)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Integration of Web Forms

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Schematic demonstrating the “front-end” and “back-end” components of the cloud-based picture archiving and communication system (PACS) with integrated web forms.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IntegrationofaZerofootprintCloudbasedPictureArchivingandCommunicationSystemwithCustomizableFormsforRadiologyResearchandEducation/0_1s20S1076633218300710.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Studies

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Study: MRMC Research Study Evaluating a New Imaging Technique

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Flowchart demonstrating the workflow to perform a multireader, multicase (MRMC) study using the cloud-based picture archiving and communication system (PACS) with web forms. DICOM, Digital Imaging and Communications in Medicine.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IntegrationofaZerofootprintCloudbasedPictureArchivingandCommunicationSystemwithCustomizableFormsforRadiologyResearchandEducation/1_1s20S1076633218300710.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Screenshot demonstrating the user interface shown to the reader in a multireader, multicase study.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IntegrationofaZerofootprintCloudbasedPictureArchivingandCommunicationSystemwithCustomizableFormsforRadiologyResearchandEducation/2_1s20S1076633218300710.jpg)

![Figure 4, Example display of results from a hypothetical three-case study. The reader's response is shown in the “response” column and the time elapsed per case is displayed in the rightmost column.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IntegrationofaZerofootprintCloudbasedPictureArchivingandCommunicationSystemwithCustomizableFormsforRadiologyResearchandEducation/3_1s20S1076633218300710.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Study: Multireader Research Study Evaluating Imaging Features of a Specific Disease Process

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Screenshot demonstrating the user interface shown to the reader in a research study where imaging features of a certain disease process are shown to multiple readers. This screenshot also demonstrates that the relative width of the picture archiving and communication system (PACS) pane and the forms pane is freely adjustable, as the forms pane has been expanded.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IntegrationofaZerofootprintCloudbasedPictureArchivingandCommunicationSystemwithCustomizableFormsforRadiologyResearchandEducation/4_1s20S1076633218300710.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Study: Educational Assessment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Screenshot showing an example educational assessment.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IntegrationofaZerofootprintCloudbasedPictureArchivingandCommunicationSystemwithCustomizableFormsforRadiologyResearchandEducation/5_1s20S1076633218300710.jpg)

![Figure 7, Screenshot showing explanation of the correct answer of an educational assessment.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IntegrationofaZerofootprintCloudbasedPictureArchivingandCommunicationSystemwithCustomizableFormsforRadiologyResearchandEducation/6_1s20S1076633218300710.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Study: Online Teaching File

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Limitations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Mell P., Grance T.: The NIST definition of cloud computing recommendations of the National Institute of Standards and Technology. NIST Spec Publ 2011; 145: pp. 7.


- 2\. Skaron A., Li K., Zhou X.H.: Statistical methods for MRMC ROC studies. Acad Radiol 2012; 19: pp. 1499-1507.


- 3\. Dendumrongsup T., Plumb A.A., Halligan S., et. al.: Multi-reader multi-case studies using the area under the receiver operator characteristic curve as a measure of diagnostic accuracy: systematic review with a focus on quality of data reporting. PLoS ONE 2014; 9: pp. 1-20.


- 4\. Tagliafico A.S., Calabrese M., Bignotti B., et. al.: Accuracy and reading time for six strategies using digital breast tomosynthesis in women with mammographically negative dense breasts. Eur Radiol 2017; 27: pp. 5179-5184.


- 5\. Kim Y.S., Chang J.M., Yi A., et. al.: Interpretation of digital breast tomosynthesis: preliminary study on comparison with picture archiving and communication system (PACS) and dedicated workstation. Br J Radiol 2017; 90: 20170182


- 6\. Sakamoto R., Yakami M., Fujimoto K., et. al.: Temporal subtraction of serial CT images with large deformation diffeomorphic metric mapping in the identification of bone metastases. Radiology 2017; 285: 161942


- 7\. Toth D.F., Töpker M., Mayerhöfer M.E., et. al.: Rapid detection of bone metastasis at thoracoabdominal CT: accuracy and efficiency of a new visualization algorithm. Radiology 2013; 270: pp. 130789.


- 8\. Dong T., Zahn C., Saguil A., et. al.: The associations between clerkship Objective Structured Clinical Examination (OSCE) grades and subsequent performance. Teach Learn Med 2017; 29: pp. 1-6.


- 9\. You E.: Vue.js. Available at: https://vuejs.org

- 10\. Klein K.A., Neal C.H.: Simulation in radiology education: thinking outside the phantom. Acad Radiol 2016; 23: pp. 908-910.


- 11\. Chetlen A.L., Mendiratta-Lala M., Probyn L., et. al.: Conventional medical education and the history of simulation in radiology. Acad Radiol 2015; 22: pp. 1252-1267.


- 12\. Hafey C.: Cornerstone \[Internet\]. Available at: https://github.com/cornerstonejs

- 13\. Mendelson D.S., Erickson B.J., Choy G.: Image sharing: evolving solutions in the age of interoperability. J Am Coll Radiol 2014; 11: pp. 1260-1269.


- 14\. Lee W.J., Yang C.Y., Liu K.L., et. al.: Establishing a web-based DICOM teaching file authoring tool using open-source public software. J Digit Imaging 2005; 18: pp. 169-175.


- 15\. Bastião Silva L.A., Costa C., Oliveira J.L.: A PACS archive architecture supported on cloud services. Int J Comput Assist Radiol Surg 2012; 7: pp. 349-358.


- 16\. Balkman J.D., Loehfelm T.W.: A cloud-based multimodality case file for mobile devices. Radiographics 2014; 34: pp. 863-872.


- 17\. Balkman J.D., Awan O.A.: A platform-independent plugin for navigating online radiology cases. J Digit Imaging 2016; 29: pp. 321-324.


- 18\. Monteiro E., Costa C., Oliveira J.L.: A de-identification pipeline for ultrasound medical images in DICOM format. J Med Syst 2017; 41: pp. 89.


- 19\. Wagner R.F., Beiden S.V., Campbell G., et. al.: Assessment of medical imaging and computer-assist systems: lessons from recent experience. Acad Radiol 2002; 9: pp. 1264-1277.


- 20\. Wagner R.F., Metz C.E., Campbell G.: Assessment of medical imaging systems and computer aids: a tutorial review. Acad Radiol 2007; 14: pp. 723-748.


- 21\. Archie K.A., Marcus D.S.: DicomBrowser: software for viewing and modifying DICOM metadata. J Digit Imaging 2012; 25: pp. 635-645.


- 22\. Epstein R.M.: Medical education—assessment in medical education. N Engl J Med 2007; 356: pp. 387-396.


- 23\. Ganguli S., Pedrosa I., Yam C.S., et. al.: Part I: preparing first-year radiology residents and assessing their readiness for on-call responsibilities. Acad Radiol 2006; 13: pp. 764-769.


- 24\. Yam C.S., Kruskal J., Pedrosa I., et. al.: Part II: preparing and assessing first-year radiology resident on-call readiness technical implementation. Acad Radiol 2006; 13: pp. 770-773.


- 25\. Towbin A.J., Paterson B., Chang P.J.: A computer-based radiology simulator as a learning tool to help prepare first-year residents for being on call. Acad Radiol 2007; 14: pp. 1271-1283.


- 26\. Yang G.L., Aziz A., Narayanaswami B., et. al.: Informatics in radiology (infoRAD): multimedia extension of medical imaging resource center teaching files. Radiographics 2005; 25: pp. 1699-1708.


- 27\. Siegel E., Reiner B.: The Radiological Society of North America's medical image resource center: an update. J Digit Imaging 2001; 14: pp. 77-79.


- 28\. Lim C.C.T., Yang G.L., Nowinski W.L., et. al.: Medical image resource center-making electronic teaching files from PACS. J Digit Imaging 2003; 16: pp. 331-336.


- 29\. Mongkolwat P., Bhalodia P., Makori A., et. al.: Informatics in radiology (infoRAD): integrating MIRC-compliant semiautomated teaching files into PACS work flow. Radiographics 2005; 25: pp. 543-548.


- 30\. Tellis W.M., Andriole K.P.: Implementing a MIRC query interface for a database driven teaching file. J Digit Imaging 2003; 16: pp. 180-184.


- 31\. Welte F.J., Kim S.C., Doshi D.J., et. al.: Incorporation of a formalized emergency radiology curriculum to facilitate population of a MIRC-based digital teaching file. J Digit Imaging 2010; 23: pp. 226-237.


- 32\. Gentili A., Chung C.B., Hughes T.: Informatics in radiology: use of the MIRC DICOM service for clinical trials to automatically create teaching file cases from PACS. Radiographics 2007; 27: pp. 269-275.