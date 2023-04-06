---
title: Capricorn–A Web-Based Automatic Case Log and Volume Analytics for Diagnostic Radiology Residents
author: [Po-Hao Chen MD MBA,Yin Jie Chen MD,Tessa S. Cook MD PhD]
date: 2015-10-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 22, Issue 10 SOURCE CL_S_AcademicRadiologyVolume22Issue10 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

On-service clinical learning is a mainstay of radiology education. However, an accurate and timely case log is difficult to keep, especially in the absence of software tools tailored to resident education. Furthermore, volume-related feedback from the residency program sometimes occurs months after a rotation ends, limiting the opportunity for meaningful intervention.

## Materials and Methods

We surveyed the residents of a single academic institution to evaluate the current state of and the existing need for tracking interpretation volume. Using the results of the survey, we created an open-source automated case log software. Finally, we evaluated the effect of the software tool on the residency in a 1-month, postimplementation survey.

## Results

Before implementation of the system, 89% of respondents stated that volume is an important component of training, but 71% stated that volume data was inconvenient to obtain. Although the residency program provides semiannual reviews, 90% preferred reviewing interpretation volumes at least once monthly. After implementation, 95% of the respondents stated that the software is convenient to access, 75% found it useful, and 88% stated they would use the software at least once a month. The included analytics module, which benchmarks the user using historical aggregate average volumes, is the most often used feature of the software. Server log demonstrates that, on average, residents use the system approximately twice a week.

## Conclusions

An automated case log software system may fulfill a previously unmet need in diagnostic radiology training, making accurate and timely review of volume-related performance analytics a convenient process.

The theory of implicit learning in the acquisition of tacit knowledge has been implicated in many areas of behavioral research, including in medicine and radiology . It posits that knowledge obtained over time and from practice is distinct from, and therefore irreplaceable, by explicit learning such as reading textbooks and attending didactic lectures. In diagnostic radiology, clinical teaching by independently interpreting an imaging study first and then reviewing findings with an experienced staff radiologist is the primary mode of implicit learning. The importance of tacit knowledge acquisition in radiology makes the volume of studies interpreted one of the important metrics for the success of a radiology resident.

Recognizing that on-service clinical learning is key to competence in radiology, standards for minimal volume of interpretation, and performance are sometimes set as thresholds necessary for accreditation. For instance, the Accreditation Council of Graduate Medical Education (ACGME) requires satisfaction of minimal volume requirements for a set of 11 radiology examination categories . To ensure the clinical competency of their practitioners, subspecialty organizations such as the American Heart Association/American College of Cardiology Foundation also set minimum volumes required as milestones for standardized levels of training . In addition, the satisfaction of some requirements is a function of both volume and timing. For example, the Mammography Quality Standards Act requires an initial experience of 240 mammographic interpretations within a 6-month interval no earlier than 2 years before completion of residency .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## Study Population

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Analytic Software Creation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Initial features offered when a resident logs into the system. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CapricornAWebBasedAutomaticCaseLogandVolumeAnalyticsforDiagnosticRadiologyResidents/0_1s20S1076633215002792.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Survey Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Sample Question From Preimplementation and Postrelease Anonymous Surveys


Preimplementation Survey 1\. How important is the volume of studies you interpret as a component of your education? Very unimportant Somewhat unimportant Neither important nor unimportant Somewhat important Very important 2\. Currently, how convenient is it for you to track the number of studies you have interpreted using existing tools? Very inconvenient Somewhat inconvenient Neither convenient or inconvenient Somewhat convenient Very convenient 3\. Estimate how many studies an average radiology resident will have interpreted during 4 years of residency for the different modalities and subspecialties? \*The residents then had an opportunity to try out a demo of the system before answering the following questions. 4\. Please rate your experience with the Capricorn demonstration (1 = lowest to 5 = highest) in “convenience,” “usefulness,” and “functionality.” 5\. If Capricorn becomes available to you, how often would you expect to use it? Never Less than once a month Once a month 2–3 Times a month Once a week 2–3 Times a week Daily 1 Month postrelease survey 1\. Please rate your experience with Capricorn (1 = lowest to 5 = highest) in “convenience,” “usefulness,” and “functionality.” 2\. How important do you consider volume of studies interpreted in your residency education? Very unimportant Somewhat unimportant Neither important nor unimportant Somewhat important Very important 3\. How often have you used Capricorn since its release last month? Never At least once a month At least once every 2 weeks At least once a week Daily 4\. What have you used Capricorn for? (check all that apply) To review my volume for various rotations To review my volume for various modalities To review my volume on call To assess my volume over time To obtain my list of performed procedures To compare myself to historical averages To find a particular study I have not used Capricorn

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Database Validation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## User Interface

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Browsing through interpreted computed tomography (CT) examinations over a 1-year period. (A) The overview window displays CTs interpreted across all rotations during this period. (B) The user clicks on the legends on the right to isolate body CT examinations to review more closely. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CapricornAWebBasedAutomaticCaseLogandVolumeAnalyticsforDiagnosticRadiologyResidents/1_1s20S1076633215002792.jpg)

![Figure 3, A detailed case log that comprises the overview display is elicited by clicking on the graph from Figure 2 . The user has the option of exporting this list to a spreadsheet or reviewing the dictated reports for individual cases (not shown) by clicking on the accession number. Note that a deidentified case log is displayed as an example, and accession numbers and patient names are fictitious. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CapricornAWebBasedAutomaticCaseLogandVolumeAnalyticsforDiagnosticRadiologyResidents/2_1s20S1076633215002792.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, The “cumulative view” shows screening and diagnostic mammography interpreted over the last 2 years of a fictional resident's training in assessing compliance with the requirements of the Mammography Quality Standards Act (8) . (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CapricornAWebBasedAutomaticCaseLogandVolumeAnalyticsforDiagnosticRadiologyResidents/3_1s20S1076633215002792.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, The interactive analytics module allows the user to adjust the anatomy, modality, and parameters of the analytical statistics using control panels (not shown). (A) The resident's number of chest radiograph interpreted is compared to the “average” resident using historical mean with confidence interval currently set to 25%–75%. (B) The cumulative count has been separated into a year-by-year analysis. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CapricornAWebBasedAutomaticCaseLogandVolumeAnalyticsforDiagnosticRadiologyResidents/4_1s20S1076633215002792.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Survey Responses

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Results From Preimplementation and 1-Month Postrelease Surveys


Preimplementation, % (n) 1 Month Postrelease, % (n) Response rate 68.3 (28) 39 (16) Importance of volume (“somewhat important” or “very important”) 89.3 (25) 100 (16) Ease of tracking volume before Capricorn (“somewhat inconvenient” or “very inconvenient”) 71.4 (20) Rating of Capricorn (4 or 5 with 5 = highest) n = 19 respondents for below questions n = 16 total respondents for below questions Capricorn convenience 57.9 (11) 94.8 (15) Capricorn usefulness 63.2 (12) 75 (12) Capricorn functionality 68.4 (13) 87.5 (14) Use Capricorn at least once monthly 89.5 (17) 87.5 (14)

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

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Degonda N., Mondadori C.R.A., Bosshardt S., et. al.: Implicit associative learning engages the hippocampus and interacts with explicit associative learning. Neuron 2005; 46: pp. 505-520.


- 2\. Siegert R.J., Taylor K.D., Weatherall M., et. al.: Is implicit sequence learning impaired in Parkinson’s disease? A meta-analysis. Neuropsychology 2006; 20: pp. 490-495.


- 3\. Barb A.S., Shyu C.-R., Sethi Y.P.: Knowledge representation and sharing using visual semantic modeling for diagnostic medical image databases. IEEE Trans Inf Technol Biomed Publ IEEE Eng Med Biol Soc 2005; 9: pp. 538-553.


- 4\. Heiberg Engel P.J.: Tacit knowledge and visual expertise in medical diagnostic reasoning: implications for medical education. Med Teach 2008; 30: pp. e184-e188.


- 5\. Henry S.G.: Polanyi’s tacit knowing and the relevance of epistemology to clinical medicine. J Eval Clin Pract 2010; 16: pp. 292-297.


- 6\.  Accreditation Council for Graduate Medical Education. Case Log Categories and Required Minimum Numbers - Review Committee for Diagnostic Radiology. Available at:  https://www.acgme.org/acgmeweb/Portals/0/PFAssets/ProgramResources/420\_DR\_Case\_Log\_Minimums.pdf  . Accessed July 1, 2014.


- 7\. Budoff M.J., Cohen M.C., Garcia M.J., et. al.: ACCF/AHA clinical competence statement on cardiac imaging with computed tomography and magnetic resonance. Circulation 2005; 112: pp. 598-617.


- 8\. Compliance Guidance: The mammography quality standards act final regulations: preparing for MQSA inspections \[Internet\].2001.U.S. Food and Drug Administration \[cited 2014 Jul 4\]. Available at: http://www.fda.gov/MedicalDevices/DeviceRegulationandGuidance/GuidanceDocuments/ucm094420.htm

- 9\. Bhargava P., Lackey A.E., Dhand S., et. al.: Radiology education 2.0–on the cusp of change: part 1. Tablet computers, online curriculums, remote meeting tools and audience response systems. Acad Radiol 2013; 20: pp. 364-372.


- 10\. Tellis W.M., Andriole K.P.: Implementing a MIRC query interface for a database driven teaching file. J Digit Imaging 2003; 16: pp. 180-184.


- 11\. Rowe S.P., Siddiqui A., Bonekamp D.: The key image and case log application: new radiology software for teaching file creation and case logging that incorporates elements of a social network. Acad Radiol 2014; 21: pp. 916-930.


- 12\. dos-Santos M., Fujino A.: Interactive radiology teaching file system: the development of a MIRC-compliant and user-centered e-learning resource. Conf Proc Annu Int Conf IEEE Eng Med Biol Soc IEEE Eng Med Biol Soc Annu Conf 2012; 2012: pp. 5871-5874.