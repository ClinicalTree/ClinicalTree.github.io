---
title: Design and Implementation of Handheld and Desktop Software for the Structured Reporting of Hepatic Masses Using the LI-RADS Schema
author: [Toshimasa J. Clark MD,Michael F. McNeeley MD,Jeffrey H. Maki MD PhD]
date: 2014-04-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 21, Issue 4 SOURCE CL_S_AcademicRadiologyVolume21Issue4 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The Liver Imaging Reporting and Data System (LI-RADS) can enhance communication between radiologists and clinicians if applied consistently. We identified an institutional need to improve liver imaging report standardization and developed handheld and desktop software to serve this purpose.

## Materials and Methods

We developed two complementary applications that implement the LI-RADS schema. A mobile application for iOS devices written in the Objective-C language allows for rapid characterization of hepatic observations under a variety of circumstances. A desktop application written in the Java language allows for comprehensive observation characterization and standardized report text generation. We chose the applications' languages and feature sets based on the computing resources of target platforms, anticipated usage scenarios, and ease of application installation, deployment, and updating.

## Results

Our primary results are the publication of the core source code implementing the LI-RADS algorithm and the availability of the applications for use worldwide via our website,  http://www.liradsapp.com/ . The Java application is free open-source software that can be integrated into nearly any vendor's reporting system. The iOS application is distributed through Apple's iTunes App Store. Observation categorizations of both programs have been manually validated to be correct. The iOS application has been used to characterize liver tumors during multidisciplinary conferences of our institution, and several faculty members, fellows, and residents have adopted the generated text of Java application into their diagnostic reports.

## Conclusions

Although these two applications were developed for the specific reporting requirements of our liver tumor service, we intend to apply this development model to other diseases as well. Through semiautomated structured report generation and observation characterization, we aim to improve patient care while increasing radiologist efficiency.

The radiology report is an essential part of the medical record, encompassing several roles. Although its primary function is to communicate important findings and to guide clinical decision-making, the radiology report is also an informational resource for medicolegal, research-related, and financial inquiries . Nonetheless, the conventional approach to radiology reporting has included few constraints on lexical or editorial choices. Consequently, radiology reports are highly inconsistent in terms of their accuracy, completeness, and clarity .

The adoption of uniform subspecialty lexicons and report formats may improve the usability of radiology reports. Perhaps, the most successful effort has been the Breast Imaging Reporting and Data System (BI-RADS), which was developed by the American College of Radiology (ACR) to reduce variability in the assessment, reporting, and management of findings in breast tissue . Its initial implementation led to substantial improvements in the clarity and consistency of mammography reports , thereby prompting the Food and Drug Administration (FDA) to mandate its adoption by breast imagers nationwide. Furthermore, by facilitating the usage of clinical data embedded in mammography reports, the BI-RADS schema has enhanced clinical research and quality assurance initiatives within the field of breast imaging .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/gr1.jpg?Signature=LqTZdE47Ana32lK8FZAVmbZWSxvxw7YnYsrram7MXoC26gZDXL1Kbn3qZCN%7EhdUgwTeAiw77BoPmwboSHeaeF1dZzL9sRPpV5Guo5xJH4k%7ExOwfkR%7EKuxNCU6jEucYQF69UDqx46YeiT5AbmwCtd3ZDB-LpHeQtr70WDOLMOByw_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


LI-RADS v2013.1 observation categorization flowchart. HCC, hepatocellular carcinoma; LI-RADS, Liver Imaging Reporting and Data System. (LR1, LR2, LR3, LR4, and LR5 represent LI-RADS categories).


Reprinted with permission of the American College of Radiology. No other representation of this material is authorized without expressed, written permission from the American College of Radiology.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Java application interface. HCC, hepatocellular carcinoma; LI-RADS, Liver Imaging Reporting and Data System; RFA, radiofrequency ablation; Y90, Yttrium-90; TACE, transcatheter arterial chemoembolization.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DesignandImplementationofHandheldandDesktopSoftwarefortheStructuredReportingofHepaticMassesUsingtheLIRADSSchema/0_1s20S107663321300593X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, iOS application – new lesion interface. DWI, diffusion-weighted imaging; HCC, hepatocellular carcinoma; PTLD, Post-transplant lymphoproliferative disorder.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DesignandImplementationofHandheldandDesktopSoftwarefortheStructuredReportingofHepaticMassesUsingtheLIRADSSchema/1_1s20S107663321300593X.jpg)

![Figure 4, iOS application – lesion list interface. LI-RADS, Liver Imaging Reporting and Data System.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DesignandImplementationofHandheldandDesktopSoftwarefortheStructuredReportingofHepaticMassesUsingtheLIRADSSchema/2_1s20S107663321300593X.jpg)

![Figure 5, iOS application – lesion details interface. LI-RADS, Liver Imaging Reporting and Data System.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DesignandImplementationofHandheldandDesktopSoftwarefortheStructuredReportingofHepaticMassesUsingtheLIRADSSchema/3_1s20S107663321300593X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

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

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix 1

## Java lesion characterization function

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/fx1a.jpg?Signature=A6yr3L5SUXsOrH64x1HOYCdWrg%7EwMT%7EYn6e03GLio9Uj3os37LYvJ%7ExgU6JHesQRkLiSkRTZaiH73LTRHuHXZZki6ICiZBLC24ThmEXT3lnN7bv17TUIsfN9CWa1NgLKhvPKu8jUdmPbSa-s9BFHelQsi9eTQZB0a9N-BUWc39k_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/fx1b.jpg?Signature=R2MewfOxNBul30SxU1OGghc6cfsnH4Dk9ek2oJxIs4fkz7Kt20Oybj3SnWhs21GEFNXc-HhE2ZW6mcYSHD%7ENCVLhl5vJ3AMk1RU43sRMFtjmtT7qa6DxwFrFmKwLKjGdFcvLwGqXjAoYBje0aVa20NL1b0ciWvK521178tk4xYw_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix 2

## Objective-C lesion characterization method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/fx2a.jpg?Signature=AqnUNteO2QPhCfGzhGVQz9n0dgD5KRs5HqrCjJUm87soVcxqKAPisMku11q8V9smbZlS5CywsAFr5RGvUHgOy3sfRsZuL5OjWbiCxMgCPJ7cqOKmhn7jdOjO40oMqqCwSZcMPo0ljsp-j1nkaScTxhc4h7ijsnv%7E2XpQU9XZajk_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/fx2b.jpg?Signature=Ej5DJq1qSq8ct9IrFASoB7YLzj4hK9EGQKEEscBZ1dCHjz5Ln6nEE377DuKoc9H2kpRg7KrtDBAsXphHfw1rLVJ1NJ-0LLdd4nXOmW6KC1DVz6D-tY26wYphjkG1HaRfyvHlVxPMxB0bfO6jGMNpT3pEQvpBUSZRYw8AnPS6Xws_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix 3

## Proposed Java function implementing API for use with CAD software

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/fx3a.jpg?Signature=gtnzL4nZLdNOJeLDJp0ueRQRhOunwkE0elSpnUl9vTP0ZLlXbQiqeovCAnFaGDKbf4EepVp8f1m4P737OJjuhdmAoOXFh5DRwIbCaUjf%7Ebvxm1iPvf3pyer6GAJoyFG4r5o7MTKoBucm5S8uelBDC6X0kvss9JwShXux1fTg2VE_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/fx3b.jpg?Signature=dkRkYEoc%7Ei3vbQwEgYKJMHVEJPPh2RJXtErLYtsiz2f7PoGEV2sQ-YkzU9UAjzVYC2igX4wcjGpYg2b1fT5Vm8MrvbMCweM%7E%7ER8QSgo1%7EeF14-D0qfl4kBjqCMgMK9tyyecFNeMDrWpLJIgPMuivl7WOK9yibBy0g7T7B06iPfI_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix 4

## Sample generated report text from Java application

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00157/S107663321300593X/fx4.jpg?Signature=da1GmvBYBmyOYF25xe4RNa0NFUnQjwlqhaNJX8LlBE955LimsQwOLV7fuoXTp7V1HGcXCsnX5xn4ptLU85d55qg3e%7EWcfftu1wby%7EK9Pddmbd0s-4kAXjolI9pIhOZ9Z4QvS%7E93H4%7EGaWvQoeC5MjGh5Sp2RJGR-xnwWKgwxUzc_&Expires=1669580541&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Duszak R., Nossal M., Schofield L., et. al.: Physician documentation deficiencies in abdominal ultrasound reports: frequency, characteristics, and financial impact. J Am Coll Radiol 2012; 9: pp. 403-408.


- 2\. Thorwarth W.T.: Get paid for what you do: dictation patterns and impact on billing accuracy. J Am Coll Radiol 2005; 2: pp. 665-669.


- 3\. Lucey L.L., Kushner D.C., American College of Radiology: The ACR guideline on communication: to be or not to be, that is the question. J Am Coll Radiol 2010; 7: pp. 109-114.


- 4\. Duszak R.: Dictating for dollars (and compliance, too). J Am Coll Radiol 2004; 1: pp. 874-875.


- 5\. Johnson A.J., Chen M.Y., Zapadka M.E., et. al.: Radiology report clarity: a cohort study of structured reporting compared with conventional dictation. J Am Coll Radiol 2010; 7: pp. 501-506.


- 6\. Robinson P.J.: Radiology's Achilles' heel: error and variation in the interpretation of the Rontgen image. Br J Radiol 1997; 70: pp. 1085-1098.


- 7\. Khorasani R., Bates D.W., Teeger S., et. al.: Is terminology used effectively to convey diagnostic certainty in radiology reports?. Acad Radiol 2003; 10: pp. 685-688.


- 8\. Kong A., Barnett G.O., Mosteller F., et. al.: How medical professionals evaluate expressions of probability. N Engl J Med 1986; 315: pp. 740-744.


- 9\. American College of Radiology: . Breast Imaging–Reporting and Data System (BI-RADS).4th ed.2003.American College of RadiologyReston, VA


- 10\. Lazarus E., Mainiero M.B., Schepps B., et. al.: BI-RADS lexicon for US and mammography: interobserver variability and positive predictive value. Radiology 2006; 239: pp. 385-391.


- 11\. Taplin S.H., Ichikawa L.E., Kerlikowske K., et. al.: Concordance of breast imaging reporting and data system assessments and management recommendations in screening mammography. Radiology 2002; 222: pp. 529-535.


- 12\. Geller B.M., Barlow W.E., Ballard-Barbash R., et. al.: Use of the American College of Radiology BI-RADS to report on the mammographic evaluation of women with signs and symptoms of breast disease. Radiology 2002; 222: pp. 536-542.


- 13\. Burnside E.S., Sickles E.A., Bassett L.W., et. al.: The ACR BI-RADS experience: learning from history. J Am Coll Radiol 2009; 6: pp. 851-860.


- 14\. Purysko A.S., Remer E.M., Coppa C.P., et. al.: LI-RADS: a case-based review of the new categorization of liver findings in patients with end-stage liver disease. Radiographics 2012; 32: pp. 1977-1995.


- 15\.  American College of Radiology. Quality and safety resources: Liver Imaging–Reporting and Data System. Available at:  http://www.acr.org/Quality-Safety/Resources/LIRADS  . Accessed August 22, 2013.;


- 16\. Tang A., Cruite I., Sirlin C.B.: Toward a standardized system for hepatocellular carcinoma diagnosis using computed tomography and MRI. Exp Rev Gastroenterol Hepatol 2013; 7: pp. 269-279.


- 17\. Freeman R.B., Mithoefer A., Ruthazer R., et. al.: Optimizing staging for hepatocellular carcinoma before liver transplantation: a retrospective analysis of the UNOS/OPTN database. Liver Transpl 2006; 12: pp. 1504-1511.


- 18\. Hertl M., Cosimi A.B.: Liver transplantation for malignancy. Oncologist 2005; 10: pp. 269-281.