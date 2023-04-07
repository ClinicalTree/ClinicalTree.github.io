---
title: HIPAA Privacy and DICOM Anonymization for Research
author: [CL_AT_DavidAvrinMDPhD]
date: 2008-03-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 15, Issue 3]
tags: [Journals,General Radiology]
---
Fetzer and West ( ) have provided us, in this issue, with a superb relatively nontechnical summary of privacy issues in any medical research arena, which includes images from a Picture Archival and Communication System (PACS). Their well-developed premise is that confidentiality is an important principle of the clinical patient record, and that the same protection is required in the research environment and to a slightly lesser extent in the education environment.

Digital Imaging and Communication in Medicine (DICOM) has provided the ability for relatively easy interinstitution sharing of medical imaging data, which powers large-scale studies: witness cancer Biomedical Informatics Grid (caBIG) of the National Cancer Institute (NCI).

The three key issues that the authors elaborate upon are: 1) every image from PACS in DICOM format contains a data “header” that includes sensitive and identifying protected health information (PHI) in addition to the technical information describing the imaging study; 2) software is available for anonymizing or de-identifying these digital images while maintaining a secure unique “key” for tracing back to the specific patient when necessary; and 3) that de-identifying DICOM data can be more difficult than it appears at first glance; significant problems can remain if one is not vigilant.

Some of the “scrubbing” software tools that the authors review are configurable. This is important because occasionally DICOM data elements are misused or inappropriately stored in the header. Occasionally, they are deliberately “mapped” to another element for device/system communication compatibility. Another issue that arises is the occurrence of DICOM private tags for vendor or site modification and use.

Usually, today, the PHI that we see at a workstation is an “overlay” of data derived from the header that projects upon, but is separate from, the image. However, some older devices, particularly ultrasound, “burn” the PHI demographics into the image data itself, and therefore are inseparable from the image. As the authors point out, such PHI can be removed with image editing tools such as Photoshop™ (Adobe Systems, Inc., San Jose, CA), following careful procedures. However, placing a black block over such PHI in PowerPoint™ (Microsoft Corp., Redmond, WA), can be readily removed and is therefore insufficient.

One final conundrum they present, worthy of further thought, is that a three-dimensional volume of computed tomographic or magnetic resonance data of the head inherently contains a soft-tissue image of facial detail; essentially a sculptured rendition of the patient’s facial appearance. Although no suggestions have come forth yet on how to deal with this, it is being explored by the Biomedical Informatics Research Network (BIRN).

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reference

- 1\. Fetzer D.T., Clark O.C.: The HIPAA privacy rule and protected health information: implications in research involving DICOM image databases. Acad Radiol 2008; 15: pp. 390-395.