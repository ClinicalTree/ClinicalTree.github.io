---
title: Experiences With a Prototype Tracking and Verification System Implemented Within an Imaging Center
author: [CL_AT_BingGuoMD,CL_AT_JorgeDocumetMS,CL_AT_JasperLeeBS,CL_AT_BrentLiuPhD,CL_AT_NelsonKingPhD,CL_AT_RasuShresthaMD,CL_AT_KevinWangBS,CL_AT_HKHuangDSc,CL_AT_EdwardGGrantMD]
date: 2007-03-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 14, Issue 3]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Most health care facilities currently struggle with protecting medical data privacy, misidentification of patients, and long patient waiting times. This article demonstrates a novel system for a clinical environment using wireless tracking and facial biometric technologies to automatically monitor and identify staff and patients to address these problems.

## Materials and Methods

The design of the location tracking and verification system (LTVS) was based on a workflow study which was performed to observe the physical location and movement of patient and staff at the Healthcare Consultation Center II (HCC II) running hospital information systems, radiology information systems, picture archive and communication systems, and a voice recognition system. Based on the results from this workflow study, the LTVS was designed using a wireless real-time location system and a facial biometric system integrated with the radiology information system. The LTVS was tested for its functionality in a laboratory environment, then evaluated at HCC II.

## Results

Experimental results in the laboratory and clinical environments demonstrated that patient and staff real-time location information and identity verification can be obtained from LTVS. Warning messages can immediately be sent to alert staff when patient’s waiting time is over a predefined limit, and unauthorized access to a security area can be audited. Additionally, patient misidentification can be prevented during the course of examinations.

## Conclusions

The system enabled health care providers to streamline the patient workflow, protect against erroneous examinations and create a security zone to prevent, and audit unauthorized access to patient health care data required by the Health Insurance Portability and Accountability Act mandate.

With the explosion in the number of digital imaging and medical records, more and more medical data are managed and stored electronically in different medical information systems, for example, hospital information systems (HIS), radiology information systems (RIS), and picture archive and communication systems (PACS). To protect the privacy of personal health information, HIPAA privacy rules regarding national standards were effected on April 14, 2001, and complianced on April 14, 2003 ( ). Great care should be taken to protect patient confidentiality to meet partial HIPAA requirements. Moreover, in an ever-increasingly complex and dynamic clinical environment, misidentification of patients is also a common problem in health facilities ( ). In the United States, the Joint Commission on Accreditation of Healthcare Organizations processed root cause analysis information on 126 cases of wrong site surgery between 1998 and 2001. Seventy-six percent of cases involved surgery on the wrong body part or site, 13% surgery on the wrong patient, and 11% the wrong surgical procedure. The Joint Commission on Accreditation of Healthcare Organizations has identified the factor that human error such as misuse of Addressograph labels, mishearing, misspelling, and misfiling may lead to misidentification. In addition, patient experience with long waiting time for scheduled appointment is another widespread problem within health care. Visitors to US hospital emergency departments wait an average of 222 minutes, or 3.7 hours, before being seen by a provider, according to a new state-by-state study released by Press Ganey Associates, _USA Today_ reports ( ). The study, which examines wait times at emergency departments across the nation, is based on 1.5 million patient questionnaires filled out in 2005. Most health care facilities struggle with protecting medical data privacy, misidentification of patients, and long patient waiting times.

To address these issues, a location tracking and verification system (LTVS) was designed and developed using wireless technology for tracking the location of patients ( ) and facial biometric technology for automatically identifying staff and patients ( ). By integrating these two technologies, the LTVS system provided a simple yet systematic solution to monitor and automatically identify staff and patients to streamline the patient workflow, protect against erroneous examinations, and create a security zone to prevent and audit unauthorized access to patient health care data for partial compliance of the HIPAA mandate.

## Materials and methods

## Clinical Workflow Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, The General outpatient tracking location workflow at the Healthcare Consultant Center II, University of Southern California, Los Angeles, CA.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ExperiencesWithaPrototypeTrackingandVerificationSystemImplementedWithinanImagingCenter/0_1s20S1076633206007173.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## LTVS Development

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, System architecture shows the location tracking and verification system (LTVS) server that consists of a web server application that runs the LTVS web-based graphical user interface. The system design and implementation were developed in-house. (a) Facial biometrics verification module with cameras. (b) Wireless location tracking module with tags. Perl = Practical Extraction and Report Language; FRS = Facial Biometric Recognition System; API = Application Programming Interface.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ExperiencesWithaPrototypeTrackingandVerificationSystemImplementedWithinanImagingCenter/1_1s20S1076633206007173.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Hardware and Software Components of the LTVS


Hardware Software Dedicated LTVS Server (PC Workstation, Dell Dimension 3000) LTVS GUI web application WiFi tracking devices: Web server (Apache) Wireless Access Points (D-Link Xtreme G router) LTVS tracking API Ekahau WiFi tags PostGreSQL database Client workstations (PC Workstation, Dell Dimension 3000) Ekahau WiFi positioning engine Logitech USB video cameras LTVS facial verification Application programming interface (Neven Vision) Image-capturing software

Note.—LTVS = Location Tracking and Verification System.


System design and implementation were completed in-house.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Laboratory Testing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Testing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The “Report Page” provides multiple choices for querying the report from the database (see left column, arrow). For example, in the figure, the graphical user interface display a window of patients John Doe, with radiology information systems identification number, tracking device number, location, event time, event date, and system message saying “Patient waiting longer than 30 minutes.”](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ExperiencesWithaPrototypeTrackingandVerificationSystemImplementedWithinanImagingCenter/2_1s20S1076633206007173.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Technical Features of the Location Tracking and Verification System to Address Given Clinical Issues


Clinical Issues System Technical Features Lost patients in the department Real-time identification of the movement of patients Patient waiting too long Provide a warning to the department personnel if a particular patient has been in one location (eg, waiting room) beyond the time limit Patient misidentification Patient identity can be verified biometrically through facial recognition at the exam site Security for protection and privacy of patient information System creates an information security zone in a given subunit. Verifies biometrically access rights to vital clinical information for authorization by the health care provider

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Patient Registration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Tag Assignment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Patient Tracking

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Information Security

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Patient Safety

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## User Interface Examples

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, The graphical user interface showing a window of the floor plan of the clinical evaluation site, University of Southern California Healthcare Consultation Center II. This example depicts that patient John Doe 1, Staff 2, and Staff 3 each had been assigned a tracking tag. Their names, tag accession number, status, and physical location are shown in event list table above the floor plan.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ExperiencesWithaPrototypeTrackingandVerificationSystemImplementedWithinanImagingCenter/3_1s20S1076633206007173.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Evaluation Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Fifteen Sample Cases with Tracking Status Including X-Ray and Computed Tomography from Location Tracking and Verification System at Healthcare Consultation Center II During the Testing in Two Given Days


Case Number Date Enter Department Start Procedure Waiting Time (Minutes) X-ray 1 November 7, 2005 8:38 am 8:54 am 16 X-ray 2 November 7, 2005 9:00 am 9:13 am 13 X-ray 3 November 7, 2005 9:39 am 9:48 am 9 X-ray 4 November 7, 2005 9:43 am 10:03 am 20 X-ray 5 November 7, 2005 10:05 am 10:28 am 23 X-ray 6 November 8, 2005 9:08 am 9:37 am 29 X-ray 7 November 8, 2005 10:50 am 11:02 am 12 X-ray 8 November 8, 2005 11:04 am 11:27 am 23 X-ray 9 November 8, 2005 1:02 pm 1:17 pm 15 X-ray 10 November 8, 2005 1:21 pm 1:34 pm 13 CT-1 November 8, 2005 8:44 am 9:52 am 68  ⁎  CT-2 November 8, 2005 10:05 am 10:43 am 38  ⁎  CT-3 November 8, 2005 10:49 am 11:43 am 54  ⁎  CT-4 November 8, 2005 1:06 pm 1:48 pm 42  ⁎  CT-5 November 8, 2005 2:29 pm 3:19 pm 50  ⁎

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

## Benefits of LTVS

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Privacy Concerns

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Cost Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Cost of the Location Tracking and Verification System Evaluated at Healthcare Consultation Center II Including Cost of Hardware and Software (Excluding Design, Development, and Implementation Costs)


Item Quantity Unit Cost Subtotal Hardware Wireless access points 6 $35 $210 Active tags 15 $80 $1,200 FRS cameras 6 $80 $480 Server (computer) 1 $700 $700 Software Web server (Apache) Free Database (PostGreSQL) Free Facial recognition SDK $5,000 license fees per year Wireless location tracking $5,000 for 15 tags Total $12,590

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Alternative Identification Devices

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\.  US Department of Health and Human Services. HIPAA. Available online at:  http://www.hhs.gov/ocr/hipaa/bkgrndhtml  . Accessed December 23, 2006.


- 2\. Thomas P., Evans C.: An identity crisis?. Clin Risk 2004; 10: pp. 18-22.


- 3\.  Joint Commission on Accreditation of Healthcare Organizations. Available online at:  http://www.saferhealthcare.org.uk/IHI/Topics/PatientIdentification/Whatweknow/Whatweknowoverview.htm  . Accessed December 23, 2006.


- 4\.  Ekahau Inc. Available online at:  http://www.ekahau.com/?id=4200  . Accessed December 23, 2006.


- 5\.  NevenVision. Available online at:  http://www.hrsltd.com/products/face\_recognition/index.htm

- 6\. Vissers J.M.H.: Patient flow-based allocation of inpatient resources: a case study. Eur J Oper Res 1998; 105: pp. 356-370.


- 7\. Bing G., Jorge D., Jasper L., et. al.: A tracking and verification system implemented in a clinical environment for partial HIPAA compliance. Proc SPIE 2006; 6145: pp. 184-191.


- 8\.  Bing G, Jorge D, Nelson K. Patient tracking and facial biometrics integrated in a clinical environment for HIPAA security compliance, Presented at the 91st Scientific Assembly and Annual Meeting of RSNA (Inforad exhibit), Sun. Nov 7-Fri, Dec 02, 2005, Chicago, IL.