---
title: Use of a Machine-learning Method for Predicting Highly Cited Articles Within General Radiology Journals
author: [Andrew B. Rosenkrantz MD MPA,Ankur M. Doshi MD,Luke A. Ginocchio,Yindalon Aphinyanaphongs MD PhD]
date: 2016-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 23, Issue 12 SOURCE CL_S_AcademicRadiologyVolume23Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

This study aimed to assess the performance of a text classification machine-learning model in predicting highly cited articles within the recent radiological literature and to identify the model's most influential article features.

## Materials and Methods

We downloaded from PubMed the title, abstract, and medical subject heading terms for 10,065 articles published in 25 general radiology journals in 2012 and 2013. Three machine-learning models were applied to predict the top 10% of included articles in terms of the number of citations to the article in 2014 (reflecting the 2-year time window in conventional impact factor calculations). The model having the highest area under the curve was selected to derive a list of article features (words) predicting high citation volume, which was iteratively reduced to identify the smallest possible core feature list maintaining predictive power. Overall themes were qualitatively assigned to the core features.

## Results

The regularized logistic regression (Bayesian binary regression) model had highest performance, achieving an area under the curve of 0.814 in predicting articles in the top 10% of citation volume. We reduced the initial 14,083 features to 210 features that maintain predictivity. These features corresponded with topics relating to various imaging techniques (eg, diffusion-weighted magnetic resonance imaging, hyperpolarized magnetic resonance imaging, dual-energy computed tomography, computed tomography reconstruction algorithms, tomosynthesis, elastography, and computer-aided diagnosis), particular pathologies (prostate cancer; thyroid nodules; hepatic adenoma, hepatocellular carcinoma, non-alcoholic fatty liver disease), and other topics (radiation dose, electroporation, education, general oncology, gadolinium, statistics).

## Conclusions

Machine learning can be successfully applied to create specific feature-based models for predicting articles likely to achieve high influence within the radiological literature.

## Introduction

Identification of articles having the greatest impact, as measured through future citations, has been a topic of interest within the radiological literature. Three recent studies have explored the most highly cited radiological articles from a broad historical perspective, evaluating a large number of journals over an extended time frame . At least three additional articles have explored the most highly cited radiological articles within a specific journal of subspecialty area . Such investigations seek to provide insights that will be helpful for researchers in shaping their studies, for journal editors and reviewers in selecting high-impact journal content, and for radiologists in appreciating the topics of greatest interest in the field . However, all of these earlier studies used essentially the same approach in their analyses: manually evaluating the content of solely the 100 most highly cited articles relevant to the question at hand. Although providing useful information from a historical perspective, this approach draws conclusions regarding the imaging literature based on only an extremely small fraction of available published articles. Moreover, a simple manual coding of features of the most highly cited articles, although easy to perform, risks leading to incorrect information regarding those features that in fact have the greatest influence in predicting a high-citation volume. In addition, the manual approach does not provide any numerical estimate of the actual overall performance of the identified features in predicting citation volume. Finally, the approach fails to provide any quantitative method for evaluating the likelihood of a given article to be highly cited. Such ability would be valuable for investigators aiming to maximize the impact of their research and for editors and reviewers aiming to enhance a journal's status.

Machine learning provides an alternate approach for performing a sophisticated evaluation of citation frequency based on a broad spectrum of article features. This approach generates computational models for predicting citation volume based on text analysis of the article's title and abstract in combination with other article meta-data, using a very large number of articles . This comprehensive scheme can identify trends that would be difficult for human observers to otherwise detect. Perhaps more important in comparison to the historical approaches of the earlier cited radiological studies, the actual predictive performance of a machine-learning model can be quantified, and the model can be applied prospectively to predict future citations at the time of an article's publication, if not even earlier . As an example, a machine-learning tool to automatically predict citations could be used to efficiently and reliably aid the initial triage and assessment of submitted manuscripts.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## Corpus Construction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


List of Included Radiological Journals and Associated 2014 Impact Factors, Ranked in Order of Descending Number of Articles in the Top 10% of All Articles in the Analysis


Journal 20014 Impact Factor  \\*  Number of Included Articles From 2012 or 2013 Number of Included Articles in Top 10% in Terms of Citations to Articles in 2014_Radiology_ 6.867 998 387_European Radiology_ 4.014 746 200_American Journal of Roentgenology_ 2.731 1320 178_European Journal of Radiology_ 2.369 1363 178_Investigative Radiology_ 4.437 220 75_British Journal of Radiology_ 1.984 575 65_RadioGraphics_ 2.602 312 45_Clinical Radiology_ 1.759 506 42_Academic Radiology_ 1.751 469 36_Journal of the American College of Radiology_ 2.836 518 31_Radiologic Clinics of North America_ 1.984 139 21_Acta Radiologica_ 1.603 382 19_Korean Journal of Radiology_ 1.571 292 13_Diagnostic and Interventional Radiology_ 1.436 178 11_Japanese Journal of Radiology_ 0.837 255 9_Radiologia Medica_ 1.343 221 8_Rofo_ 1.402 283 8_Clinical Imaging_ 0.810 379 6_BMC Medical Imaging_ 1.312 80 3_Surgical and Radiologic Anatomy_ 1.047 289 3_Seminars in Roentgenology_ 0.705 81 1_Canadian Association of Radiologists Journal_ 0.519 129 0_Iranian Journal of Radiology_ 0.366 86 0_Radiologe_ 0.425 244 0

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Preprocessing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Experimental Design

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Machine-learning Algorithms

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Performance Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Feature Assessment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Area Under the Curve (AUC) of Investigated Machine-learning Algorithms for Prediction of an Article's Presence Among the Top 10% of Cited Articles


Model AUC bbr 0.814 svm\_linear 0.811 naïve\_bayes 0.676

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


General Themes Ascribed to the Maximally Reduced List of 210 Core Features That Were Identified by the Highest Performing Machine-learning Model  \\*  ,  †

Theme Core Features Article meta-data Journal of publication_Radiology_ \[Journal\]_Eur Radiol_ \[Journal\]_Radiologe_ \[Journal\]_Clin Imaging_ \[Journal\]_Invest Radiol_ \[Journal\]_Surg Radiol Anat_ \[Journal\]_Acta Radiol_ \[Journal\]_Can Assoc Radiol J_ \[Journal\]_J Am Coll Radiol_ \[Journal\]_Rofo_ \[Journal\]_Jpn J Radiol_ \[Journal\] Publication type Case Reports\[Publication Type\] Research Support, Non-U.S. Gov't\[Publication Type\] Journal Article\[Publication Type\] Letter\[Publication Type\] Comment\[Publication Type\] Research Support, N.I.H., Extramural\[Publication Type\] English Abstract\[Publication Type\] case case\[Title\] Basic imaging modality CT ct\[Title\] ct MRI mr mr\[Title\] weighted magnetic resonance weighted\[Title\] multiparametric t2 Magnetic Resonance Imaging:methods\[MeSH\] mh\_Magnetic Resonance Imaging PET pet pet\[Title\] positron Positron-Emission Tomography\[MeSH\] emission Fluoroscopy Fluoroscopy\[MeSH\] Advanced imaging technique Diffusion-weighted MRI diffusion Diffusion Magnetic Resonance Imaging\[MeSH\] mh\_Diffusion Magnetic Resonance Imaging diffusion\[Title\] Diffusion Magnetic Resonance Imaging:methods\[MeSH\] dwi dw adc kurtosis apparent coefficient Hyperpolarized MRI hyperpolarized hyperpolarized\[Title\] CT reconstruction technique iterative\[Title\] iterative filtered energy\[Title\] fbp asir projection mbir adaptive diagnostic Radiation Dosage\[MeSH\] safire sinogram\[Title\] Dual-energy CT energy dect dual\[Title\] dual Tomosynthesis tomosynthesis\[Title\] tomosynthesis Elastography elastography mh\_Elasticity Imaging Techniques Elasticity Imaging Techniques\[MeSH\] shear wave\[Title\] shear\[Title\] wave elastography\[Title\] Elasticity Imaging Techniques:methods\[MeSH\] Computer-aided diagnosis Image Interpretation, Computer-Assisted\[MeSH\] Radiographic Image Interpretation, Computer-Assisted\[MeSH\] Radiographic Image Interpretation, Computer-Assisted:methods\[MeSH\] mh\_Radiographic Image Interpretation, Computer-Assisted Organ-based feature Prostate cancer prostate\[Title\] Prostatic Neoplasms:pathology\[MeSH\] Prostatic Neoplasms\[MeSH\] mh\_Prostatic Neoplasms prostate Prostatectomy\[MeSH\] Prostatic Neoplasms:surgery\[MeSH\] Prostatic Neoplasms:diagnosis\[MeSH\] mh\_Prostate Prostate\[MeSH\] Prostate-Specific Antigen\[MeSH\] mh\_Prostate-Specific Antigen Prostate:pathology\[MeSH\] gleason Prostate:blood supply\[MeSH\] Thyroid nodules Thyroid Nodule\[MeSH\] mh\_Thyroid Nodule Liver lesions  \\*  mh\_Liver Neoplasms Liver Neoplasms\[MeSH\] Adenoma, Liver Cell:diagnosis\[MeSH\] liver\[Title\] hepatocellular\[Title\] hepatocellular liver mh\_Adenoma, Liver Cell Adenoma, Liver Cell\[MeSH\] mh\_Carcinoma, Hepatocellular Carcinoma, Hepatocellular\[MeSH\] Liver Neoplasms:diagnosis\[MeSH\] hcc Nonalcoholic fatty liver disease nafld Non-alcoholic Fatty Liver Disease\[MeSH\] Other General oncology cancer cancer\[Title\] Neoplasm Staging\[MeSH\] metastases locally locally\[Title\] Radiation dose Education education\[MeSH\] Radiology:education\[MeSH\] Gadolinium Gadolinium DTPA\[MeSH\] Gadolinium DTPA:diagnostic use\[MeSH\] gadoxetic\[Title\] gadoxetic mh\_Gadolinium DTPA Electroporation Electroporation:methods\[MeSH\] mh\_Electroporation Statistics Sensitivity and Specificity\[MeSH\] Statistics, Nonparametric\[MeSH\] ROC Curve\[MeSH\] Reproducibility of Results\[MeSH\] Predictive Value of Tests\[MeSH\] Linear Models\[MeSH\] Chi-Square Distribution\[MeSH\] Proportional Hazards Models\[MeSH\] Analysis of Variance\[MeSH\] Logistic Models\[MeSH\] Area Under Curve\[MeSH\] statistical Study design Prospective Studies\[MeSH\] Survival Analysis\[MeSH\] Comparative Study\[Publication Type\] comparison\[Title\] multicenter trial\[Title\] prospective\[Title\] prognostic\[Title\]

CT, computed tomography; MRI, magnetic resonance imaging; PET, positron emission tomography.


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

## References

- 1\. Brinjikji W., Klunder A., Kallmes D.F.: The 100 most-cited articles in the imaging literature. Radiology 2013; 269: pp. 272-276.


- 2\. Yoon D.Y., Yun E.J., Ku Y.J., et. al.: Citation classics in radiology journals: the 100 top-cited articles, 1945–2012. AJR Am J Roentgenol 2013; 201: pp. 471-481.


- 3\. Pagni M., Khan N.R., Cohen H.L., et. al.: Highly cited works in radiology: the top 100 cited articles in radiologic journals. Acad Radiol 2014; 21: pp. 1056-1066.


- 4\. Dolan R.S., Hanna T.N., Warraich G.J., et. al.: The top 100 articles in the radiology of trauma: a bibliometric analysis. Emerg Radiol 2015; 22: pp. 667-675.


- 5\. Bui-Mansfield L.T.: Top 100 cited AJR articles at the AJR's Centennial. AJR Am J Roentgenol 2006; 186: pp. 3-6.


- 6\. Siegelman S.S.: The cat's meow: the most frequently cited papers in Radiology 1955–1986. Radiology 1988; 168: pp. 414-420.


- 7\. Fu L.D., Aliferis C.: Models for predicting and explaining citation count of biomedical articles. AMIA Annu Symp Proc 2008; pp. 222-226.


- 8\. Lokker C., McKibbon K.A., McKinlay R.J., et. al.: Prediction of citation counts for clinical articles at two years using data available within three weeks of publication: retrospective cohort study. BMJ 2008; 336: pp. 655-657. http://www.bmj.com/content/336/7645/655

- 9\. Castillo C., Donato D., Gionis A.: String Processing and Information Retrieval (SPIRE).Estimating the number of citations using author reputation.2007.pp. 107-117.


- 10\. Thomson Reuters : InCites Journal Citation Reports. Available at http://about.jcr.incites.thomsonreuters.com/ Accessed January 23, 2016


- 11\. Rosenkrantz A.B., Ayoola A.: The Impact Factor of Radiological Journals: Associations with Journal Content and Other Characteristics Over a Recent 12-Year Period. Acad Radiol 2016; 23: pp. 661-668.


- 12\. Durieux V., Gevenois P.A.: Bibliometric indicators: quality measurements of scientific publication. Radiology 2010; 255: pp. 342-351.


- 13\. Thomson Reuters : Web of Science. Available at webofscience.com Accessed January 23, 2016


- 14\. Garfield E.: Citation indexes for science; a new dimension in documentation through association of ideas. Science 1955; 122: pp. 108-111.


- 15\. National Center for Biotechnology Information : U.S. National Library of Medicine. PubMed. Available at http://www.ncbi.nlm.nih.gov/pubmed Accessed January 23, 2015


- 16\. U.S. National Library of Medicine : Publication Characteristics (Publication Types)—Scope Notes. Available at https://www.nlm.nih.gov/mesh/pubtypes.html Accessed January 23, 2016


- 17\. Aphinyanaphongs Y., Fu L.D., Li Z., et. al.: A comprehensive empirical comparison of modern supervised classification and feature selection methods for text categorization. J Assn Inf Sci Tech 2014; 65: pp. 1964-1987.


- 18\. Aphinyanaphongs Y., Lulejian A., Brown D.P., et. al.: Text classification for automatic detection of E-cigarette use and use for smoking cessation from twitter: a feasibility pilot. Pac Symp Biocomput 2016; 21: pp. 480-491.


- 19\. Kibriya A.M., Frank E., Pfahringer B., et. al.: AI 2004: advances in artificial intelligence.Multinomial naive Bayes for text categorization revisited.2004.Springer Berlin Heidelbergpp. 488-499.


- 20\. McCallum A.K.: Mallet: MAchine Learning for LanguagE Toolkit. Available at http://mallet.cs.umass.edu Accessed September 14, 2016


- 21\. Joachims T.: Text categorization with support vector machines: learning with many relevant features.Nédellec C.Rouveirol C.Machine learning: ECML-98.1998.Springer Berlin HeidelbergBerlin, Heidelberg:pp. 137-142.


- 22\. Genkin A., Lewis D.D., Madigan D.: Large-scale Bayesian logistic regression for text categorization. Technometrics 2007; 49: pp. 291-304.


- 23\. Barentsz J.O., Richenberg J., Clements R., et. al.: ESUR prostate MR guidelines 2012. Eur Radiol 2012; 22: pp. 746-757.


- 24\. Rosenkrantz A.B., Kim S., Lim R.P., et. al.: Prostate cancer localization using multiparametric MR imaging: comparison of Prostate Imaging Reporting and Data System (PI-RADS) and Likert scales. Radiology 2013; 269: pp. 482-492.


- 25\. Cheng S.P., Lee J.J., Lin J.L., et. al.: Characterization of thyroid nodules using the proposed thyroid imaging reporting and data system (TI-RADS). Head Neck 2013; 35: pp. 541-547.


- 26\. Russ G., Royer B., Bigorgne C., et. al.: Prospective evaluation of thyroid imaging reporting and data system on 4550 nodules with and without elastography. Eur J Endocrinol 2013; 168: pp. 649-655.


- 27\. Purysko A.S., Remer E.M., Coppa C.P., et. al.: LI-RADS: a case-based review of the new categorization of liver findings in patients with end-stage liver disease. Radiographics 2012; 32: pp. 1977-1995.


- 28\. Davenport M.S., Khalatbari S., Liu P.S., et. al.: Repeatability of diagnostic features and scoring systems for hepatocellular carcinoma by using MR imaging. Radiology 2014; 272: pp. 132-142.


- 29\. Rosenkrantz A.B., Ayoola A.: The impact factor of radiological journals: associations with journal content and other characteristics over a recent 12-year period. Acad Radiol 2016; 23: pp. 661-668.