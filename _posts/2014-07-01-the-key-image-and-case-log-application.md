---
title: The Key Image and Case Log Application
author: [CL_AT_StevenPRoweMDPhD,CL_AT_AdeelSiddiquiMD,CL_AT_DavidBonekampMDPhD]
date: 2014-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 21, Issue 7]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

To create novel radiology key image software that is easy to use for novice users, incorporates elements adapted from social networking Web sites, facilitates resident and fellow education, and can serve as the engine for departmental sharing of interesting cases and follow-up studies.

## Materials and Methods

Using open-source programming languages and software, radiology key image software (the key image and case log application, KICLA) was developed. This system uses a lightweight interface with the institutional picture archiving and communications systems and enables the storage of key images, image series, and cine clips. It was designed to operate with minimal disruption to the radiologists' daily workflow. Many features of the user interface have been inspired by social networking Web sites, including image organization into private or public folders, flexible sharing with other users, and integration of departmental teaching files into the system. We also review the performance, usage, and acceptance of this novel system.

## Results

KICLA was implemented at our institution and achieved widespread popularity among radiologists. A large number of key images have been transmitted to the system since it became available. After this early experience period, the most commonly encountered radiologic modalities are represented. A survey distributed to users revealed that most of the respondents found the system easy to use (89%) and fast at allowing them to record interesting cases (100%). Hundred percent of respondents also stated that they would recommend a system such as KICLA to their colleagues.

## Conclusions

The system described herein represents a significant upgrade to the Digital Imaging and Communications in Medicine teaching file paradigm with efforts made to maximize its ease of use and inclusion of characteristics inspired by social networking Web sites that allow the system additional functionality such as individual case logging.

As picture archiving and communications systems (PACS) and the Internet have become commonplace in the modern practice of radiology, digital teaching files have naturally begun to replace old hard copy teaching files. The advantages of digital teaching files versus hard copy teaching files are numerous, including ease of submitting and accessing interesting cases, the lack of a space-occupying physical file, and the digital preservation of the case images. Furthermore, as the volumes of studies encountered by radiologists have increased markedly in recent years, a means of efficiently logging cases for reasons other than teaching, such as follow-up and quality control, has also become highly desirable. Generally, PACS are not optimized for either teaching file creation or case logging.

Although the system we describe in this report has capabilities not traditionally encompassed by digital teaching files (including personal case logging), one of the central goals of the system has been to provide a platform for the departmental sharing of interesting cases. Thus, previously reported digital teaching files remain an important point of comparison . The inherent efficiency of creating a digital teaching file based on key images as opposed to entire studies has been noted by a number of authors . Kamauu et al. noted the importance of PACS vendor neutrality in the development of a standard digital teaching file format. Ease of use and minimal disruption of the radiologists workflow have been addressed in the literature . The Radiological Society of North America's (RSNA) Medical Imaging Resource Center (MIRC) open-source software has endeavored to provide the current standard for the construction of digital teaching files and is involved in the ongoing development of a widely accepted digital teaching file format. Thus, MIRC compliance is of high importance for digital teaching files .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Key Image and Case Log Application Design Criteria


Minimal interference with clinical workflow Reduction of necessary interaction to as little as a single mouse click, with more complex processes occurring hidden from the user Social network functionality Automated case sorting Video generation Ability to retrieve case data to personal archives Compliance with all clinical information security requirements at our institution Easy to use and customizable Implementation carried out with freely available programming languages and software libraries

Table 2


Ideal Features of a Digital Imaging and Communications in Medicine Digital Teaching File


General characteristics Constructed using open-source software PACS vendor neutral with lightweight connection between the teaching file system and the institutional PACS Key image format with option to submit entire image series or cine clip as appropriate Teaching file system maintained on an institutional server with password protection Front end characteristics Minimal/no stored patient protected health information Minimal user computer knowledge required to submit cases (ie, conversion of images and clips to JPEG/MPEG format, parsing of cases into the appropriate area of the teaching file, etc. all handled automatically by the teaching file system) Annotation of cases can be carried out at the discretion of the submitting radiologist Minimal workflow disruption to submit a case Back end characteristics Viewable from any computer with Web access. Minimal user computer knowledge required to browse cases (ie, pleasing visual layout with intuitive on-screen buttons and text boxes) Organized into public (teaching cases) and private (follow-up cases) areas Flexible search function allowing the user to search by diagnosis, organ system, modality, submitting radiologist, and so forth

JPEG, Joint Photographic Experts Group; MPEG, Moving Picture Experts Group; PACS, picture archiving and communications systems.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Technical Aspects and Implementation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Front End

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Simplified schematic representation of KICLA architecture with image paths indicated by red arrows and with additional information flow represented by blue arrows . AJAX, Asynchronous JavaScript and XML; DCMTK, Digital Imaging and Communications in Medicine ToolKit; JPEG, Joint Photographic Experts Group; KICLA, key image and case log application; MySQL, My Structured Query Language; PACS, picture archiving and communications system; PERL, Practical Extraction and Report Language. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheKeyImageandCaseLogApplication/0_1s20S1076633214001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Screen capture image of the main front end window. A thumbnail representation of the key image is included as are text fields for annotation of the image, an option to select an assigned attending for the case, and a button allowing for retrieval of the entire image series as a video clip.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheKeyImageandCaseLogApplication/1_1s20S1076633214001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Back End

## Home Screen and Case Browser

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Screen capture image of the home screen of the back end. Thumbnail representations of the user's most recently submitted cases are prominently displayed. Additionally, a “Search” text field is available as are access points to the user's key image and case log application groups and to the “teaching file” folder that includes images that have been shared with all users. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheKeyImageandCaseLogApplication/2_1s20S1076633214001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Screen capture image of the teaching file (TF) folder that includes all publicly shared cases and is accessible from the user's home folder. Filter functions ( thick red arrow ) are displayed in the left upper aspect of the TF screen with the option to sort cases by specific groups, sections, or users. “Like” buttons are also provided for each case ( thin red arrow ). (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheKeyImageandCaseLogApplication/3_1s20S1076633214001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Viewing Module

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Screen capture image of an individual case viewing window demonstrating the display of all relevant key images submitted for the case, including images from prior studies. From this screen, a user is able to e-mail the case to themselves or to other users. The thick red arrow in the figure indicates the pink frame surrounding a submitted video file. Additionally, a text field for commenting on the case is provided with the option for the comment to be publicly displayed or sent only to the submitting user ( thin red arrow ). (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheKeyImageandCaseLogApplication/4_1s20S1076633214001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Social Network Functionality, Groups

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Radiologist Usage Analysis and User Survey

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Teaching File Usage

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Monthly usage as determined by the number of key images submitted each month. Key image and case log application became available in November 2011, and there has been a sustained average of more than 1000 images submitted per month since February 2012. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TheKeyImageandCaseLogApplication/5_1s20S1076633214001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Radiologist KICLA User Survey Responses

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Selected Key Image and Case Log Application (KICLA) User Survey Questionnaire Responses


Question Answer Number of Responses (Percentage) How frequently have you used KICLA? Daily multiple times 3 (16) Daily to several times per week 9 (47) About once every 1–2 weeks 5 (26) Infrequently 2 (11) An app like KICLA (which is a pilot project) has the potential to convince me to use it to manage the following percentage of cases that I want to record during my clinical workflow 91%–100% 14 (74) 50%–90% 3 (16) 15%–49% 1 (5) 0%–14% 1 (5) With your previously established method (before using KICLA), what percentage of cases did/do you record just by number without ever getting images for them? 76%–100% 7 (37) 51%–75% 2 (11) 26%–50% 2 (11) 0%–25% 8 (42) Which of the following basic and advanced features do you use often enough to feel comfortable? The “Teaching File Share” button 15 (79) The “Like” button 4 (21) The statistics view 8 (42) Video export to PowerPoint 7 (37) Viewing videos using the Flowplayer (embedded Web viewing using flash) 8 (42) Scrolling through images of a video sequence 9 (47) Creating folders and organizing cases into folders 10 (53) Search function 10 (53) Self-created user groups 1 (5) The comment feature (private) 2 (11) The comment feature (public) 1 (5) Motivations for using KICLA Clinical follow-up 17 (89) Quality control of my own work 9 (47) Peer review of my cases 2 (11) Self-review of my cases 9 (47) Teaching others by sharing cases 11 (58) Review of shared cases for learning 9 (47) Teaching others by aggregating cases for later preparation of presentations 14 (74)

Table 4


Survey Questionnaire Responses Comparing Experiences before and after Key Image and Case Log Application (KICLA) Use


Question Answer Number of Responses (Percentage) Before Using KICLA Using KICLA How much time did it take to record a case? 0–29 seconds 4 (21) 15 (79) 30 seconds–2 minutes 8 (42) 4 (21) 2–5 minutes 6 (32) 0 (0) 5–10 minutes 1 (5) 0 (0) What percentage of follow up cases were you able to record? 91%–100% 3 (16) 10 (53) 50%–90% 2 (11) 8 (42) 15%–49% 10 (53) 0 (0) 0%–14% 4 (21) 1 (5)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Bhargava P., Dhand S., Lackey A.E., et. al.: Radiology education 2.0—on the cusp of change: part 2. eBooks; file sharing and synchronization tools; websites/teaching files; reference management tools and note taking applications. Acad Radiol 2013; 20: pp. 373-381.


- 2\. dos-Santos M., Fujino A.: Interactive radiology teaching file system: the development of a MIRC-compliant and user-centered e-learning resource. Conf Proc IEEE Eng Med Biol Soc 2012; 2012: pp. 5871-5874.


- 3\. Ernst R.D., Baumgartner B.R., Tamm E.P., et. al.: Development of a teaching file by using a DICOM database. Radiographics 2002; 22: pp. 217-221.


- 4\. Gentili A., Chung C.B., Hughes T.: Informatics in radiology: use of the MIRC DICOM service for clinical trials to automatically create teaching file cases from PACS. Radiographics 2007; 27: pp. 269-275.


- 5\. Herderson B., Camorlinga S., DeGagne J.C.: A cost-effective web-based teaching file system. J Digit Imaging 2004; 17: pp. 87-91.


- 6\. Kamauu A.W., DuVall S.L., Liimatta A.P., et. al.: Translating the IHE teaching file and clinical trial export (TCE) profile document templates into functional DICOM structured report objects. J Digit Imaging 2008; 21: pp. 390-407.


- 7\. Kamauu A.W., DuVall S.L., Robison R.J., et. al.: Informatics in radiology (infoRAD): vendor-neutral case input into a server-based digital teaching file system. Radiographics 2006; 26: pp. 1877-1885.


- 8\. Kamauu A.W., DuVall S.L., Wiggins R.H., et. al.: Using applet-servlet communication for optimizing window, level and crop for DICOM to JPEG conversion. J Digit Imaging 2008; 21: pp. 348-354.


- 9\. Lee W.J., Yang C.Y., Liu K.L., et. al.: Establishing a Web-based DICOM teaching file authoring tool using open-source public software. J Digit Imaging 2005; 18: pp. 169-175.


- 10\. Rojas C.A., Jawad H., Chung J.H.: The new era of radiology teaching files. AJR Am J Roentgenol 2012; 198: pp. 773-776.


- 11\. Rosset A., Muller H., Martins M., et. al.: Casimage project: a digital teaching files authoring environment. J Thorac Imaging 2004; 19: pp. 103-108.


- 12\. Rosset A., Ratib O., Geissbuhler A., et. al.: Integration of a multimedia teaching and reference database in a PACS environment. Radiographics 2002; 22: pp. 1567-1577.


- 13\. Toms A.P., Kasmai B., Williams S., et. al.: Building an anonymized catalogued radiology museum in PACS: a feasibility study. Br J Radiol 2006; 79: pp. 666-671.


- 14\. Wilkinson L.E., Gledhill S.R.: An integrated approach to a teaching file linked to PACS. J Digit Imaging 2008; 20: pp. 402-410.


- 15\. Zaidel M., Hopper K., Iyriboz T.: Interactive web-based radiology teaching file. J Digit Imaging 1999; 12: pp. 203-204.


- 16\.  Radiological Society of North America. Available at:  http://www.rsna.org/MIRC.aspx  . Accessed May 1, 2013.


- 17\.  Ubuntu. Available at:  http://www.ubuntu.com  . Accessed August 1, 2011.


- 18\.  Virtual Machine Ware. Available at:  http://www.vmware.com  . Accessed August 1, 2011.


- 19\.  Practical Extraction and Report Language. Available at:  http://www.perl.org  . Accessed August 1, 2011.


- 20\.  JavaScript Object Notation. Available at:  http://www.json.com  . Accessed August 1, 2011.


- 21\.  My Structured Query Language. Available at:  http://www.mysql.com  . Accessed September 15, 2011.


- 22\.  Joint Photographics Expert Group. Available at:  http://www.jpeg.org  . Accessed August 15, 2011.


- 23\.  Fast Forward Moving Picture Experts Group. Available at:  http://www.ffmpeg.org  . Accessed September 15, 2011.


- 24\.  Motion Picture Experts Group. Available at:  http://mpeg.chiariglione.org  . Accessed August 1, 2011.


- 25\.  Image Magick. Available at:  http://imagemagick.org  . Accessed August 1, 2011.


- 26\.  Flow Player. Available at:  http://flowplayer.org  . Accessed August 15, 2011.


- 27\.  IHE Key Image Note. Available at:  http://wiki.ihe.net/index.php?title=Key\_Image\_Note  . Accessed November 20, 2013.


- 28\. Asch D.A., Jedrziewski M.K., Christakis N.A.: Response rates to mail surveys published in medical journals. J Clin Epidemiol 1997; 50: pp. 1129-1136.