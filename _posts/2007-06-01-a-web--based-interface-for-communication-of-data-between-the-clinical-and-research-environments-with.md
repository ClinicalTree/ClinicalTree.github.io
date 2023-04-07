---
title: A Web -Based Interface for Communication of Data Between the Clinical and Research Environments without Revealing Identifying Information
author: [CL_AT_PeytonHBlPhD,CL_AT_GaryELaderachBS,CL_AT_CharlesRMeyerPhD]
date: 2007-06-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 14, Issue 6]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Recent health care policies and regulations have affected the manner in which patient data—especially protected health information (PHI)—are handled in both the clinical and research settings. Specifically, it is now more challenging to obtain de-identified PHI from the clinic for use in research while adhering to the requirements of this new environment.

## Materials and Methods

To meet this challenge, we have devised a novel web-based interface that facilitates the communication of data (eg, biopsy results) between the clinic and research environments without revealing PHI to the research team or associated research identifiers to the clinical collaborators. At the heart of the scheme is a web application that coordinates message passing between the researchers (in general, the requesters of de-identified PHI) and clinical collaborators (who have access to PHI) by use of a protocol that protects confidentiality.

## Results

We describe the design requirements of this communication scheme and present implementation details of the web application and its associated database.

## Conclusions

We conclude that this scheme provides a useful communication mechanism that facilitates clinical research while maintaining confidentiality of patient data.

Recent years have seen significant changes in the management of patient data in the medical setting. These changes have been heavily influenced and, in some cases, dictated by regulations such as the rather broad mandates of the Department of Health and Human Services. Specifically, certain provisions of Health Insurance Portability and Accountability Act, as detailed in Department of Health and Human Services 45 CFR Parts 160 to 164 ( )—notably, the Privacy Rule and the Security Rule ( )—have greatly affected the manner in which medical staff and medical centers operate with respect to both clinical practice and research. Further, privacy practices in some hospitals and medical centers are influenced by policies of The Joint Commission (formerly the Joint Commission on Accreditation of Healthcare Organizations). On a local level, clinical research facilities are influenced by local institutional review boards (IRB). All of these are concerned with the proper handling of protected health information (PHI), which is any information about health and health care that can be linked to an individual. Confidentiality of PHI must be maintained for both legal and ethical reasons, and the adherence to appropriate standards is mandatory for facilities that receive federal funding. Clearly, a new set of procedures is needed to facilitate research while protecting PHI in this new environment.

As an example of PHI, consider the results obtained from a radiologic examination. Images from these exams are commonly made available in DICOM format (Digital Imaging and Communications in Medicine \[ \]). This widely used set of standards specifies not only the encoding and storage of image data, but also specifies how meta-data relating to the patient, the imaging equipment, the imaging exam, etc., are to be stored along with the image data. The meta-data (the DICOM attributes, often referred to collectively as the “DICOM header”) are integral with the image data and thus cannot be lost or separated from it, a clear advantage to researchers. However, even though the DICOM standard has been a boon to researchers, it comes with a price: In the current environment of confidentiality practices, the information stored in the meta-data—much of it PHI—must be dealt with properly.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Deidentifying DICOM images

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, This flowchart illustrates how the “patient ID” attribute is processed when a DICOM image is received by our lab. This attribute holds the patient’s hospital ID when the image file leaves the PACS in the hospital. However, by the time the image file is written to the disk array in our lab, this value of this attribute has been changed to the so-called research ID. Note that the database table that stores the correspondence between the hospital and research IDs stores the patient ID in encrypted form.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AWebBasedInterfaceforCommunicationofDataBetweentheClinicalandResearchEnvironmentswithoutRevealingIdentifyingInformation/0_1s20S1076633207001365.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 1

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 2

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 3

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Web-CAP system description

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Flowchart of Web-CAP showing the life cycle of a request for information as initiated by the researcher. Type-in boxes indicate information that is entered by the users. For simplicity, the messages are shown in abbreviated form; in practice, the messages include additional identifying information. (a) The creation of the request message by the researcher and its storage in the database. (b) The retrieval of the request by the clinical collaborator and the creation of a response message. (c) The storage of the response message in the database and the subsequent retrieval and viewing of it by the researcher. The Web-CAP application and the database are central to the process, acting in tandem as an interface between the clinical and research sides. Note how the identifier field name and content change depending on the location of the message: “patient ID” on the clinical side and “research ID” on the research side.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AWebBasedInterfaceforCommunicationofDataBetweentheClinicalandResearchEnvironmentswithoutRevealingIdentifyingInformation/1_1s20S1076633207001365.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 1

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 2

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 3

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 4

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 5

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 6

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 7

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 8

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 9

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 10

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step 11

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Implementation and use

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\.  US Department of Health and Human Services. Standards for privacy of individually identifiable health information. 45 CFR Parts 160 through 164. Available online at  http://www.dhhs.gov/ocr/hipaa/guidelines/Introduction.rtf  . Accessed October 4, 2006.


- 2\.  US Department of Health and Human Services. National Institutes of Health. HIPAA privacy rule and its impacts on research. Available online from  http://privacyruleandresearch.nih.gov/healthservicesprivacy.asp  . Retrieved October 5, 2006.


- 3\.  National Electrical Manufacturers Association. Digital imaging and communications in medicine. DICOM Homepage. Available online at  http://medical.nema.org/dicom/  . Accessed October 6, 2006.


- 4\.  US Department of Health and Human Services. National Institutes of Health. National Cancer Institute. Lung Image Database Consortium. Available online at  http://imaging.cancer.gov/programsandresources/InformationSystems/LIDC  . Accessed January 9, 2007.


- 5\.  Mallinckrodt Institute of Radiology. MIR DICOM Central Test Node Software. Available online at  http://wuerlim.wustl.edu/DICOM/ctn.html  . Accessed October 11, 2006.


- 6\.  MySQL AB. Accessed October 11, 2006. Available online at  http://www.mysql.com/products/  .


- 7\. National Electrical Manufacturers Association: Rosslyn, Virginia Digital imaging and communications in medicine (DICOM), Part 5: Data structures and encoding 2006; 38:


- 8\. National Electrical Manufacturers Association: Rosslyn, Virginia Digital imaging and communications in medicine (DICOM), Part 3: Information object definitions 2006; 255:


- 9\. Gupta D., Saul M., Gilbertson J.: Evaluation of a deidentification (De-Id) software engine to share pathology reports and clinical documents for research. Am J Clin Pathol 2004; 121: pp. 176-186.