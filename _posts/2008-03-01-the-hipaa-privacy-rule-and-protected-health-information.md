---
title: The HIPAA Privacy Rule and Protected Health Information
author: [CL_AT_DavidTFetzerBS,CL_AT_OClarkWestMD]
date: 2008-03-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 15, Issue 3]
tags: [Journals,General Radiology]
---
Much of the medical imaging community now uses the Digital Imaging and Communication in Medicine (DICOM) format, developed by the American College of Radiology and the National Electrical Manufacturers Association as a standard system for viewing, archiving, retrieving, and transferring images ( ). Benefits stem from the fact that a single standard provides physicians practicing within a variety of fields, for different institutions, and working with various technologies the ability to readily share images ( ). As the DICOM image format was integrated into clinical practice, it was subsequently integrated into clinical research and teaching databases.

The DICOM format is a multipart document that contains two layers: the header, typically hidden from view, and the viewable image. Most problematic from the standpoint of patient confidentiality is the identifying information saved in the DICOM header ( ). Such information may include patient name, date and time of the exam, participating physicians (ordering, reading), and so on. Image dimensions, pixel spacing, slice thickness, scan time, and other scanning protocols are also saved in the header. Each variable is stored under a standardized data group and element number. An example would be 0010,0030, where the group number, in this case 0010, is the assigned location for much of the patient’s personal information, and the element number, 0030, contains the patient’s date of birth. Other examples are the group-element numbers 0010,0010 as the assigned location for the patient name, and 0018,0050 as the assigned location for the slice thickness.

## Health insurance portability and accountability act and protected health information—who does the privacy rule affect?

The Health Insurance Portability and Accountability Act of 1996 (HIPAA) is a statute intended to ensure the portability of health insurance information. The Privacy Rule, published in August 2002 as part of the implementation of HIPAA, is a comprehensive federal protection of the privacy of personal health information ( ). Protected health information (PHI) is defined as “individually identifiable health information that is transmitted or maintained in any form or medium by a covered entity or its business associates, excluding certain education and employment records” ( ).  Figure 1 provides the items that constitute PHI. This list does not apply to any randomized study code or other identification assigned to each record that is in no way derived from or related to the protected information about that individual ( ). Researchers are subject to HIPAA Privacy Rule regulations if they are part of or work for a covered entity, provide heath care to subjects as part of their research, or work at a hybrid institution, such as a university that provides heath care as well as participates in research ( ).

![Figure 1, Identifiers considered Health Insurance Portability and Accountability Act protected health information. *Direct identifiers that must be excluded from a limited data set.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheHIPAAPrivacyRuleandProtectedHealthInformation/0_1s20S1076633207006848.jpg)

## PHI and the DICOM header—what in the header is considered PHI?

Much of the information stored in the DICOM header falls under the umbrella of PHI and thus is subject to the rules and regulations of HIPAA. Many data elements such as patient name and medical record number are explicit identifiers. Other elements may be PHI under specific circumstances (eg, in a rural imaging center, exam date recorded on radiographs that reveal the presence of a rare pathologic finding would in and of itself be considered an identifier to that patient). We feel the data elements listed in  Fig 2 have the potential to be identifiers and thus may fall under HIPAA PHI regulations. We recommend the removal of these elements if not required for research purposes ( ). Because the information included in each DICOM header is dependent on the imaging modality, the specific imaging device, and the institution operating the equipment, researchers may only have to concern themselves with a limited number of the listed data elements.

![Figure 2, Digital Imaging and Communication in Medicine (DICOM) data groups and elements that may constitute protected health information. Classification of some elements as protected health information identifiers may be dependent on incidence of pathology at a certain institution or geographic area. SOP: service-object pair; UID: unique identifier.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheHIPAAPrivacyRuleandProtectedHealthInformation/1_1s20S1076633207006848.jpg)

## DICOM and PHI—why should researchers care?

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## De-Identifying DICOM headers—scrubbing a dataset containing PHI

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Radiological Society of North America: DICOM: The Value and Importance of an Imaging Standard. http://www.rsna.org/Technology/DICOM/index.cfm Accessed July 15, 2005


- 2\. Radiological Society of North America: DICOM: the value and importance of an imaging standard. http://www.rsna.org/Technology/DICOM/intro/index.cfm Accessed July 15, 2005


- 3\. Kallepalli V.N., Ehikioya S.A., Camorlinga S., et. al.: Security middleware infrastructure for DICOM images in health information systems. J Digital Imaging 2003; 16: pp. 356-364.


- 4\. National Electrical Manufacturers Association: Digital Imaging and Communications in Medicine (DICOM)—part 1: introduction and overview. http://medical.nema.org/dicom/2004.html Accessed July 15, 2005


- 5\.  Health Insurance Portability and Accountability Act, P.L. 104–191, 110 Stat 2023 (1996).


- 6\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 CFR § 160–164).


- 7\. Department of Health and Human Services: Protecting personal health information in research: understanding the HIPAA privacy rule (NIH Publication #03-5388). http://privacyruleandresearch.nih.gov/pr\_02.asp Accessed July 14, 2005


- 8\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.514(b)).


- 9\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.501).


- 10\. Gunn P.P., Fremont A.M., Bottrell M., et. al.: The Health Insurance Portability and Accountability Act Privacy Rule—a practical guide for researchers. Med Care 2004; 42: pp. 321-327.


- 11\. National Electrical Manufacturers Association: Digital Imaging and Communication in Medicine (DICOM) part 6: data dictionary. http://medical.nema.org/dicom/2003/03\_06PU.PDF Accessed July 18, 2005


- 12\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.508(a)).


- 13\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.508(c)).


- 14\. Department of Health and Human Services: OCR HIPAA privacy - research. http://www.hhs.gov/ocr/hipaa/guidelines/research.pdf Accessed July 13, 2005


- 15\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.514(b)).


- 16\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.514(e)).


- 17\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.512(i)(1)(i)).


- 18\. Toms A., Kasmai B., Williams S., et. al.: Building an anonymized catalogued radiology museum in PACS: a feasibility study. Br J Radiol 2006; 79: pp. 666-671.


- 19\.  67 Federal Register 53182 (August 14, 2002) (codified at 45 § CFR 164.502(b)).


- 20\. Roach W.H., Hoban R.C.T., Broccolo B.M., et. al.: Medical records and the law.1994.Aspen Publishers, IncGaithersburg, MD