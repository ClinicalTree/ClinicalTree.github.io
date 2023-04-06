---
title: Simple and Efficient Method for Region of Interest Value Extraction from Picture Archiving and Communication System Viewer with Optical Character Recognition Software and Macro Program
author: [Young Han Lee MD PhD,Eun Hae Park MD,Jin-Suck Suh MD PhD]
date: 2015-01-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 22, Issue 1 SOURCE CL_S_AcademicRadiologyVolume22Issue1 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The objectives are: 1) to introduce a simple and efficient method for extracting region of interest (ROI) values from a Picture Archiving and Communication System (PACS) viewer using optical character recognition (OCR) software and a macro program, and 2) to evaluate the accuracy of this method with a PACS workstation.

## Materials and Methods

This module was designed to extract the ROI values on the images of the PACS, and created as a development tool by using open-source OCR software and an open-source macro program. The principal processes are as follows: (1) capture a region of the ROI values as a graphic file for OCR, (2) recognize the text from the captured image by OCR software, (3) perform error-correction, (4) extract the values including area, average, standard deviation, max, and min values from the text, (5) reformat the values into temporary strings with tabs, and (6) paste the temporary strings into the spreadsheet. This principal process was repeated for the number of ROIs. The accuracy of this module was evaluated on 1040 recognitions from 280 randomly selected ROIs of the magnetic resonance images. The input times of ROIs were compared between conventional manual method and this extraction module-assisted input method.

## Results

The module for extracting ROI values operated successfully using the OCR and macro programs. The values of the area, average, standard deviation, maximum, and minimum could be recognized and error-corrected with AutoHotkey-coded module. The average input times using the conventional method and the proposed module-assisted method were 34.97 seconds and 7.87 seconds, respectively.

## Conclusions

A simple and efficient method for ROI value extraction was developed with open-source OCR and a macro program. Accurate inputs of various numbers from ROIs can be extracted with this module. The proposed module could be applied to the next generation of PACS or existing PACS that have not yet been upgraded.

## Key points:

- 1.
Optical character recognition applications are helpful in radiologic reading environments.

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633213X00248/S1076633214002475/gr1.jpg?Signature=DAISdBiZKX5NMbh5QmCob8Cf7mBj1Sm41UhpV12WyQtE0wwbk3TeHu5YyOfbEKG7PvlWZqa3urAwbeGHWMTUHYtOcZKZ06On9xnX8%7EYo6IpDWRYWY5rG3XPbj1WUWCQ246GQ1A-vXrQ7AlPBbDuYd1F63L79rCflvLd2rqfD-AA_&Expires=1669584078&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Screenshots of the Picture Archiving and Communicating System (PACS). **(a)** Region of interest (ROI) values are displayed on the PACS screen. In large images, the ROI values are overlaid with the background signal. **(b)** By zooming out, the ROI values are displayed with no background. SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Hardware and Software

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Main Module for ROI Extraction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (1)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (2)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, OCR of the ROI values. (a) Captured image of the ROI values, (b) unprocessed raw text after OCR, and (c) error correction and space removal of the raw text. OCR, optical character recognition; ROI, region of interest; SD, standard deviation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SimpleandEfficientMethodforRegionofInterestValueExtractionfromPictureArchivingandCommunicationSystemViewerwithOpticalCharacterRecognitionSoftwareandMacroProgram/0_1s20S1076633214002475.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (3)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (4)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (5)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


![Figure 2, Flowchart of the ROI extracting module. OCR, optical character recognition; PACS, Picture Archiving and Communicating System; ROI, region of interest.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SimpleandEfficientMethodforRegionofInterestValueExtractionfromPictureArchivingandCommunicationSystemViewerwithOpticalCharacterRecognitionSoftwareandMacroProgram/1_1s20S1076633214002475.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- (6)
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Spreadsheet. The extracted region of interest values are successfully inserted in a spreadsheet with proper cell separation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SimpleandEfficientMethodforRegionofInterestValueExtractionfromPictureArchivingandCommunicationSystemViewerwithOpticalCharacterRecognitionSoftwareandMacroProgram/2_1s20S1076633214002475.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Accuracy Evaluation and Comparison

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

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

## References

- 1\.  Optical character recognition. Wikipedia. Available at:  http://en.wikipedia.org/wiki/Optical\_character\_recognition  . Accessed August 24, 2013.


- 2\. Cook T.S., Zimmerman S., Maidment A.D., et. al.: Automated extraction of radiation dose information for CT examinations. J Am Coll Radiol 2010; 7: pp. 871-877.


- 3\. Li X., Zhang D., Liu B.: Automated extraction of radiation dose information from CT dose report images. AJR Am J Roentgenol 2011; 196: pp. W781-W783.


- 4\. Lee Y.H., Song H.T., Suh J.S.: Quantitative computed tomography (QCT) as a radiology reporting tool by using optical character recognition (OCR) and macro program. J Digit Imaging 2012; 25: pp. 815-818.


- 5\.  AutoHotkey Web site. Available at  http://www.autohotkey.com  . Accessed August 24, 2013.


- 6\. Robson M.D., Gatehouse P.D., Bydder M., et. al.: Magnetic resonance: an introduction to ultrashort TE (UTE) imaging. J Comput Assist Tomogr 2003; 27: pp. 825-846. AutoHotkey Web site. Available at:  http://www.autohotkey.com  . Accessed August 24, 2013.


- 7\.  GOCR Web site. Available at:  http://jocr.sourceforge.net/api  . Accessed August 24, 2013.


- 8\. Goyal N., Jain N., Rachapalli V.: Ergonomics in radiology. Clin Radiol 2009; 64: pp. 119-126.


- 9\. Harisinghani M.G., Blake M.A., Saksena M., et. al.: Importance and effects of altered workplace ergonomics in modern radiology suites. Radiographics 2004; 24: pp. 615-627.