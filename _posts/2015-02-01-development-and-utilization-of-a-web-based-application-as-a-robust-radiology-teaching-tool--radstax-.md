---
title: Development and Utilization of a Web-Based Application as a Robust Radiology Teaching Tool (RadStax) for Medical Student Anatomy Teaching
author: [Philip G. Colucci BFA,Petro Kosty MD,William R. Shrauner BS,Elizabeth Arleo MD,Michele Fuortes MD PhD,Andrew S. Griffin MD,Yun-Han Huang BS,Krishna Juluru MD,Apostolos John Tsiouris MD]
date: 2015-02-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 22, Issue 2 SOURCE CL_S_AcademicRadiologyVolume22Issue2 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The primary role of radiology in the preclinical setting is the use of imaging to improve students' understanding of anatomy. Many currently available Web-based anatomy programs include either suboptimal or overwhelming levels of detail for medical students. Our objective was to develop a user-friendly software program that anatomy instructors can completely tailor to match the desired level of detail for their curriculum, meets the unique needs of the first- and the second-year medical students, and is compatible with most Internet browsers and tablets.

## Materials and Methods

RadStax is a Web-based application developed using free, open-source, ubiquitous software. RadStax was first introduced as an interactive resource for independent study and later incorporated into lectures. First- and second-year medical students were surveyed for quantitative feedback regarding their experience.

## Results

RadStax was successfully introduced into our medical school curriculum. It allows the creation of learning modules with labeled multiplanar (MPR) image sets, basic anatomic information, and a self-assessment feature. The program received overwhelmingly positive feedback from students. Of 115 students surveyed, 87.0% found it highly effective as a study tool and 85.2% reported high user satisfaction with the program.

## Conclusions

RadStax is a novel application for instructors wishing to create an atlas of labeled MPR radiologic studies tailored to meet the specific needs their curriculum. Simple and focused, it provides an interactive experience for students similar to the practice of radiologists. This program is a robust anatomy teaching tool that effectively aids in educating the preclinical medical student.

For many medical students, their first exposure to the field of radiology occurs in gross anatomy and related courses. The quality of this experience has long-term impact on medical students' competence in and opinions about radiology . The instructor's goal in this setting is not to teach clinical radiology but rather to use imaging to demonstrate anatomy and provide students with the basics of interpretation . Although a didactic approach is often necessary to disseminate key information within a limited time frame, clinical correlates and interactive experiences are preferred by students and are thought to improve their understanding of anatomy . Digital technology can help create more interactive experiences in medical education , as evidenced by the increasing use of the iPad (Apple Inc., Cupertino, CA); however, there is often an underutilization of this technology in radiology courses . Although there are many applications and online radiology resources already available, such as E-anatomy (IMAIOS, Montpellier, France) or the Medical Resource Imaging Center (MIRC; RSNA, Oak Brook, IL), none is optimized for preclinical medical education . Lack of time and resources is a significant limitation for faculty who seek to provide the most rewarding educational experience possible .

After reviewing the currently available resources, we identified key characteristics of an ideal teaching tool that can be tailored to meet the specific needs of the preclinical anatomy or radiology instructor. The ideal resource would include 1) a fast and intuitive way to create labels for all anatomy of interest; 2) the incorporation of basic information about each labeled region of interest; 3) the ability to view all three planes of imaging simultaneously; 4) a guide bar for localization to facilitate three-dimensional (3D) understanding; 5) a search function; 6) the ability to be easily incorporated into lectures; 7) availability for independent study; and 8) a means for self-assessment. Therefore, the purpose of our endeavor was to develop a free, user-friendly, Web-based program for instructors to create an institution-specific tool compatible with both Web browsers and the iPad, which is becoming ubiquitous in the classroom.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633214X00024/S107663321400378X/gr1.jpg?Signature=UWC0Gs09ILVhoOVIeycGJWFeMER09qNo01sz8W6v4Yjb%7EmHqrlV3a619dbLsQAWKYZJhcYXpFvO8-SqlgEumYC2FjJIl4lJs6X1h2uRN7vuXsV7qNKi09ZzXwrzjUhe000TnX2LmOudLeN-9nFiBdBet7PkH57izePITeCq4BO4_&Expires=1669584539&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Screenshot of RadStax, an interactive Web-based program for viewing imaging studies that allows 1) a fast and intuitive way to create labels for all anatomy of interest; 2) the incorporation of basic information about each labeled region of interest; 3) the ability to view all three planes of imaging simultaneously; 4) a guide bar for localization to facilitate 3D understanding; 5) a search function; 6) the ability to be easily incorporated into lectures; 7) availability for independent study; and 8) a means for self-assessment.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## Technical Development

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)




Table 1





Sample Spreadsheet




Set Name  Formal Name  Common Names  Structure Description  Vascular  Basilar artery  BA, vessel, artery  Origin: confluence of vertebral artery at the junction of the pons and medulla oblongata branches: anterior inferior cerebellar artery and pontine arteries

Terminal branches: superior cerebellar artery and posterior cerebral artery  Viscera  Common bile duct  CBD, Vater  Origin: the common bile duct is formed from the confluence of the cystic duct and common hepatic duct

Drains to: joins the main pancreatic duct to form the ampulla of Vater  Bone  Coracoid process  CP  Superior to the glenoid cavity, this anterolateral projection of the scapula gives rise to the attachment of three muscles: coracobrachialis, short head of the biceps, and pectoralis minor.  Nerve  Facial nerve  FN, CN VII, nerve, inner ear  Arises from the pons. Controls muscles of facial expression, conveys taste from anterior 2/3 tongue. Supplies preganglionic parasympathetic fibers to submandibular and lacrimal glands  Muscle  Flexor hallucis longus  FHL  Proximal attachment: the inferior two-thirds of the posterior surface of the fibula and the inferior part of the interosseous membrane

Distal attachment: the base of the distal phalanx of the great toe  Level  Functional segment 1  FS1, liver, portal vein, hepatic, division, divisions, FS, FD1, FD  The caudate lobe found in the posterior part of the liver  Gland  Pituitary gland  PGl, hypophysis  Rests in the hypophysial fossa. Composed of the anterior pituitary and posterior pituitary  Space  Rectouterine pouch  RuP, Douglas  Separates the body of the uterus and the supravaginal cervix from the sigmoid colon  Connective tissue  Thecal sac  ThSac  A membrane of dura mater that surrounds the spinal cord and cauda equina and is filled with cerebrospinal fluid




Sample of the information entered into a spreadsheet and then converted into XML format. The columns “Set Name” and “Common Names” were created with a future version in mind, which will provide a text search function.




[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Screenshot of the RadStax developer program. The studies load similarly; however, there are “STRUCTURE” and “ROI” tabs that allow for an intuitive and user-friendly way to create labels. The “STRUCTURE” tab allows for creation of new labels or selection of pre-populated data imported from the spreadsheet. These structures may then be edited or deleted directly within the program. The “ROI” tab will automatically generate coordinates after the developer selects the desired label type and clicks on the structure's location in the main viewer. ROI, region of interest.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DevelopmentandUtilizationofaWebBasedApplicationasaRobustRadiologyTeachingToolRadStaxforMedicalStudentAnatomyTeaching/0_1s20S107663321400378X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Program Implementation and Assessment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Survey of First- and Second-Year Medical Students Who Used RadStax


First-Year Students; _N_ = 55 Second-Year Students; _N_ = 60 Combined percentage; _N_ = 115 How helpful was it to see all three planes of imaging simultaneously (with a guide in the other two windows)? 8.42/10 8.20/10 83.1 How helpful was it to be able to scroll through all three planes of imaging simultaneously? 8.37/10 8.11/10 82.4 How helpful was it to have the label follow structures while scrolling through the main window? 9.25/10 9.71/10 94.8 How useful was the quiz function? 7.08/10 8.07/10 75.8 How useful were the descriptions associated with labeled structures? 6.73/10 7.47/10 71.0 How helpful was it to have multiple modalities of the same study? 8.45/10 8.27/10 83.6 Overall, did you find RadStax to be an EFFECTIVE study resource? 8.47/10 8.47/10 84.7 Overall, did you find RadStax to be an EFFICIENT study resource? 7.73/10 8.16/10 79.5 Overall, how satisfied were you with RadStax? 7.93/10 8.42/10 81.8

Medical students were asked to participate in a voluntary and anonymous electronic survey. Subjects responded on a 10-point scale ranging from (1) “Not helpful / Did not use” to (10) “Extremely helpful.” The data mean is displayed.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Technical Product

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Screenshot demonstrating the use of magnetic resonance, 3D localization capabilities, and full-screen mode. In addition to being able to scroll through all three viewers, clicking on the main viewer automatically loads the appropriate slices in the other two viewers allowing for 3D localization (a) . Full-screen mode provides the maximum viewer size and is indicated in the top left corner (b) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DevelopmentandUtilizationofaWebBasedApplicationasaRobustRadiologyTeachingToolRadStaxforMedicalStudentAnatomyTeaching/1_1s20S107663321400378X.jpg)

![Figure 4, Screenshot of the use of plain films and quiz mode. Clicking on the “Quiz” button automatically closes the navigation window and randomly generates numbers for each label (a) . Clicking on the “Key” button opens the navigation window and displays the answer key under the Index drop-down menu (b) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DevelopmentandUtilizationofaWebBasedApplicationasaRobustRadiologyTeachingToolRadStaxforMedicalStudentAnatomyTeaching/2_1s20S107663321400378X.jpg)

![Figure 5, Screenshot of labels in axial, coronal, and sagittal views. Labels are only displayed in the main viewer. Clicking on the “Axial,” “Coronal,” and “Sagittal” buttons will load the desired series of images and their labels ( a , b , and c ; respectively).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DevelopmentandUtilizationofaWebBasedApplicationasaRobustRadiologyTeachingToolRadStaxforMedicalStudentAnatomyTeaching/3_1s20S107663321400378X.jpg)

![Figure 6, Screenshot of labels toggled on (a) and off (b) . Instead of altering the Joint Photographic Experts Group images, the labels are displayed in an overlay fashion using an Extensible Markup Language file. This feature is especially beneficial when regions of interest are very small or in close proximity.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DevelopmentandUtilizationofaWebBasedApplicationasaRobustRadiologyTeachingToolRadStaxforMedicalStudentAnatomyTeaching/4_1s20S107663321400378X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Implementation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Survey Results

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

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Branstetter B.F., Humphrey A.L., Schumann J.B.: The long-term impact of preclinical education on medical students' opinions about radiology. Acad Radiol 2008; 15: pp. 1331-1339.


- 2\. Feigin D.S., Magid D., Smirniotopoulos J.G., et. al.: Learning and retaining normal radiographic chest anatomy: does preclinical exposure improve student performance?. Acad Radiol 2007; 14: pp. 1137-1142.


- 3\. Bloomfield J.: Radiology–focus of the medical curriculum?. AAJR Am J Roentgenol 1982; 138: pp. 980-981.


- 4\. Erinjeri J.P., Bhalla S.: Redefining radiology education for first-year medical students: shifting from a passive to an active case-based approach. Acad Radiol 2006; 13: pp. 789-796.


- 5\. Zou L., King A., Soman S., et. al.: Medical students' preferences in radiology education a comparison between the Socratic and didactic methods utilizing powerpoint features in radiology education. Acad Radiol 2011; 18: pp. 253-256. Epub 2010 Nov 13


- 6\. Phillips A.W., Smith S.G., Straus C.M.: The role of radiology in preclinical anatomy: a critical review of the past, present, and future. Acad Radiol 2013; 20: pp. 297-304.e1.


- 7\. Phillips A.W., Smith S.G., Ross C.F., et. al.: Improved understanding of human anatomy through self-guided radiological anatomy modules. Acad Radiol 2012; 19: pp. 902-907. Epub 2012 Apr 24


- 8\. Roubidoux M.A., Chapman C.M., Piontek M.E.: Development and evaluation of an interactive Web-based breast imaging game for medical students. Acad Radiol 2002; 9: pp. 1169-1178.


- 9\. Durfee S.M., Jain S., Shaffer K.: Incorporating electronic media into medical student education: a survey of AMSER members on computer and web use in radiology courses. Alliance of Medical Student Educators in Radiology. Acad Radiol 2003; 10: pp. 205-210.


- 10\. Marker D., Juluru K., Long C., et. al.: Strategic improvements for gross anatomy Web-based teaching. Anat Res Int 2012; 2012: pp. 146262. Epub 2011 Dec 14


- 11\.  Dashevsky B, Gorovoy M, Weadock W, Juluru K. Radiology teaching files: an assessment of their role and desired features based on a national survey. \[ahead of print\]


- 12\. Lewis P.J., Chen J.Y., Lin D.J., et. al.: Radiology ExamWeb: development and implementation of a national web-based examination system for medical students in radiology. Acad Radiol 2013; 20: pp. 290-296.