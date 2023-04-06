---
title: A Practical Approach for Inexpensive Searches of Radiology Report Databases
author: [Benoit Desjardins MD PhD,R. Curtis Hamilton BSME]
date: 2007-06-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 6 SOURCE CL_S_AcademicRadiologyVolume14Issue6 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We present a method to perform full text searches of radiology reports for the large number of departments that do not have this ability as part of their radiology or hospital information system.

## Materials and Methods

A tool written in Microsoft Access (front-end) has been designed to search a server (back-end) containing the indexed backup weekly copy of the full relational database extracted from a radiology information system (RIS). This front end-/back-end approach has been implemented in a large academic radiology department, and is used for teaching, research and administrative purposes.

## Results

The weekly second backup of the 80 GB, 4 million record RIS database takes 2 hours. Further indexing of the exported radiology reports takes 6 hours. Individual searches of the indexed database typically take less than 1 minute on the indexed database and 30–60 minutes on the nonindexed database. Guidelines to properly address privacy and institutional review board issues are closely followed by all users.

## Conclusions

This method has potential to improve teaching, research, and administrative programs within radiology departments that cannot afford more expensive technology.

Modern radiology departments make extensive use of information technology. Basic computer workstations with displays are used to review images, and are part of a Picture and communication archiving system (PACS) that distributes the images throughout a department or an institution. Dictation of radiology reports is commonly performed with voice recognition software that minimizes the need for transcriptionists and reduces the time from exam completion to availability of the final report ( ). A large computer infrastructure, the radiology information system (RIS) contains all the patient and radiology exam information, including final radiology reports and administrative information, such as billing. All these systems are interrelated to produce an efficient modern work environment. Many of the administrative and clinical needs of a modern radiology department are addressed by these systems. However, these systems often fail to address some specific information technology needs of the radiologists, particularly related to teaching, quality assurance and research. Sometimes these needs are met by a larger hospital information system, but often they are not.

## RIS

A RIS is used to store, manipulate and distribute information about the patients, their radiologic exams, and the resulting images. A RIS usually contains information about patient registration, tracking, scheduling and billing, information about radiology reports including the text of the reports themselves, and information about tracking of images. The images themselves are usually not stored in the RIS but on the PACS. The RIS usually has a health level 7 interface with the PACS to associate reports with images and quickly retrieve prior reports when a radiologist interprets images on the PACS.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Three tables in a relational database. The column headers are indicated for each table. The tables are linked through specific unique identifiers, patient identification (ID), exam ID, and internal ID number of the report text.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APracticalApproachforInexpensiveSearchesofRadiologyReportDatabases/0_1s20S1076633207001250.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## SQL

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Purpose

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Material and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Back-End Server

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Front-End Client

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Back-End Server

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Front-End Client

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, The basic RadQuery interface, a form in Microsoft Access. The top part contains the entry of search terms and restrictions. The bottom part displays the list of reports found by the search (bottom left), the text of the reports (bottom right), patient information (middle left), and report information (middle right).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APracticalApproachforInexpensiveSearchesofRadiologyReportDatabases/1_1s20S1076633207001250.jpg)

![Figure 3, Sample search terms and restrictions. A pulled down menu of all the radiologists in the radiology information system database is also illustrated.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APracticalApproachforInexpensiveSearchesofRadiologyReportDatabases/2_1s20S1076633207001250.jpg)

![Figure 4, This illustrates the results of a database search using RadQuery. The list of reports found by the search is illustrated at the bottom left. The user can then select any report and the text of the report is displayed in the bottom right panel, which is scrollable. The results can be saved in a text file or an Excel file. The unrestricted mode is illustrated, containing Personal Health Information (PHI).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APracticalApproachforInexpensiveSearchesofRadiologyReportDatabases/3_1s20S1076633207001250.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Search Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Search Contexts

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Security, Privacy, and IRB Issues

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, This illustrates the dialog box displayed when the user selects the unrestricted mode. The purpose of the search must be entered by the user. If the purpose is research, the system requests entry of a specific privacy review board key issued by the institutional review board to unlock the unrestricted mode.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/APracticalApproachforInexpensiveSearchesofRadiologyReportDatabases/4_1s20S1076633207001250.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Limitations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Marquez L.O.: Improving medical imaging report turnaround times. Radiol Manage 2005; 27: pp. 34-37.


- 2\. Codd E.F.: A relational model of data for large shared data banks. CACM 1970; 13: pp. 377-387.


- 3\. Chamberlin D.D., Boyce R.F.: SEQUEL: a structured English query language.1974.pp. 249-264. Proceedings of the 1974 ACM SIGFIDET workshop on Data description, access and control. Ann Arbor, Michigan


- 4\. Viescas J.L.: 2003.Microsoft PressRedmond, WA


- 5\.  US Code of Federal Regulations, Title 45, Volume 1 Part 164 Subpart E (revised October 1, 2005): Privacy of individually identifiable health information (45CFR164).


- 6\.  US Code of Federal Regulations, Title 45, Volume 1 Part 46 Subpart A (Revised October 1, 2005): Basic HHS Policy for protection of human research subjects (45CFR46).


- 7\. Chew F.S.: Evaluation of clinical experience in a radiology residency program with quantitative profiling: rationale, methods, and application. Acad Radiol 1999; 6: pp. 102-111.


- 8\. Lee S.I., Chew F.S.: Radiology in the emergency department: technique for quantitative description of use and results. Am J Roentgenol 1998; 171: pp. 559-564.