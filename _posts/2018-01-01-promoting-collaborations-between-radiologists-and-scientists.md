---
title: Promoting Collaborations Between Radiologists and Scientists
author: [CL_AT_JohnPaulJYuMDPhD,CL_AT_BradleyMSpielerMD,CL_AT_TiffanyLChanMD,CL_AT_ElizabethMJohnsonMD,CL_AT_VikasGulaniMDPhD,CL_AT_KimLSlerMD,CL_AT_PonnadaANarayanaPhDMSc,CL_AT_WinnieAMarMD,CL_AT_JamesMBrianMD,CL_AT_ChinKNgPhD,CL_AT_PeterAHardyPhD]
date: 2018-01-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 25, Issue 1]
tags: [Journals,General Radiology]
---
Radiology as a discipline thrives on the dynamic interplay between technological and clinical advances. Progress in almost all facets of the imaging sciences is highly dependent on complex tools sourced from physics, engineering, biology, and the clinical sciences to obtain, process, and view imaging studies. The application of these tools, however, requires broad and deep medical knowledge about disease pathophysiology and its relationship with medical imaging. This relationship between clinical medicine and imaging technology, nurtured and fostered over the past 75 years, has cultivated extraordinarily rich collaborative opportunities between basic scientists, engineers, and physicians. In this review, we attempt to provide a framework to identify both currently successful collaborative ventures and future opportunities for scientific partnership. This invited review is a product of a special working group within the Association of University Radiologists-Radiology Research Alliance.

## Introduction

Radiology as a discipline thrives on the dynamic interplay between technological and clinical advances. Progress in almost all facets of the imaging sciences is highly dependent on complex tools sourced from physics, engineering, biology, and the clinical sciences to obtain, process, and view imaging studies. The application of these tools, however, requires broad and deep medical knowledge about disease pathophysiology and its relationship with medical imaging. This relationship between clinical medicine and imaging technology, nurtured and fostered over the past 75 years, has cultivated extraordinarily rich collaborative opportunities between basic scientists, engineers, and physicians both within academia and between academic scientists and imaging equipment scientists and manufacturers. In this review, we attempt to provide a framework to identify both currently successful collaborative ventures and future opportunities for scientific partnership within the academic environment. The multidisciplinary nature of these interactions also naturally presents challenges and roadblocks, which we have outlined along with potential solutions. This review is organized by disciplines within the imaging sciences that are strongly positioned for collaborative efforts: medical physics (between physical scientists or engineers and clinicians), biological science, medical informatics (computer-aided diagnosis \[CAD\] and machine learning \[ML\]), and finally, medical education in hopes of spurring future ideas, discussions, and relationships that can further enrich the imaging sciences.

## Medical Physics Collaborations

## Overview

The introduction and implementation of X-rays, nuclear magnetic resonance, ultrasound, and radioisotope tagging and detection techniques into the medical arena by physicists—coupled with dramatic gains in computational capacity and memory—have revolutionized medical imaging. Traditionally, medical imaging research has been conceptualized along two different domains. In the first, imaging scientists sought to both develop and refine technologies to image the human body with higher spatial resolution and increased signal-to-noise ratios. In the second, clinical imaging research in radiology was devoted toward describing new imaging findings and understanding the correlation of these findings with disease pathophysiology . The major interest in medical imaging research over the past decade has been focused on technical advances in computed tomography (CT) and high-field magnetic resonance imaging (MRI) as well as the optimization of the balance between image quality and patient safety . More recently, medical imaging research has evolved into a dynamic, multiparametric, multimodal, and interdisciplinary field that seeks to noninvasively study the intact human body. These include significant advances in numerous areas of imaging research, from the development of unique radiopharmaceuticals and technical advances in positron emission tomography (PET) imaging to digital breast tomosynthesis. These and other innovations have provided unique and valuable information about tissue composition, morphology, and function. Specifically, efforts within the imaging science community, coupled with easier and greater availability of computational resources, have resulted in the development of advanced image-analysis methods and processing algorithms that can be applied to enhance images and to extract novel quantitative data .

## Case Examples

## MRI Texture Features as Biomarkers to Predict the Methylguanine Methyltransferase ( _MGMT_ ) Methylation Status in Glioblastomas

Glioblastoma multiforme (GBM) is a malignant primary brain tumor with a median survival of 14 months . Current treatment paradigms comprise an initial surgical resection and debulking followed by radiation therapy and temozolomide chemotherapy, with longitudinal studies demonstrating an increase in median survival of approximately 3 months as compared to radiotherapy alone . Oncological evaluation of GBM also incorporates the evaluation of several well-defined molecular genetic biomarkers to provide both prognostic evaluation and treatment planning. One such molecular genetic biomarker is the methylation status of the promoter region of the _MGMT_ gene. Methylation of the promoter region of _MGMT_ ( _MGMT_ methylation) gene suppresses transcriptional activity with a concomitant decreased downstream DNA repair activity and is associated with longer survival. As a complement to molecular testing, recent work has sought to identify magnetic resonance texture features that can classify regions of the tumor as either methylated or unmethylated . In collaboration with medical physicists, recent studies have calculated both co-occurrence and run length texture features with support vector machines (SVMs) and random forest classifiers used to predict the _MGMT_ methylation status. The best classification system combines the SVM classifier with four co-occurrence-based texture features (correlation, energy, entropy, and local intensity) originating from T2-weighted images, yielding a sensitivity of 0.803 and a specificity of 0.813 . These results suggest that SVM and texture features from magnetic resonance images can be used to predict the _MGMT_ methylation status in preoperative GBM tumors, providing a noninvasive imaging correlate for this important biomarker.

## Technical Feasibility Proof for High-resolution Low-dose Photon-counting CT of the Breast

Prompted by collaborations with medical physicists, a 2016 study performed by Kalender et al. investigated a new method for CT imaging of the breast . Historically, CT has shown little utility for evaluating breast tissue when compared to mammography secondary to a limited spatial resolution and a higher radiation dose. Despite the success of digital mammography, limitations still remain in the early detection of breast cancer, particularly in patients with dense breasts. The novel CT approach described in the present study for a dedicated breast CT scanner with a photon-counting detector (pcBCT) aims to provide high spatial resolution (better than 100 µm) combined with low average glandular dose (levels of 5 mGy or less). The detector uses cadmium telluride (CdTe) crystals to count photons. The advantage of using CdTe is that it has the ability to directly convert X-ray photon energy into electric charge. This unique property of CdTe avoids the deterioration of spatial resolution caused by the need of scintillating crystals to first generate light photons. The results showed that pcBCT scanners offer much higher spatial resolution than other breast CT scanners and breast tomosynthesis. Microcalcifications were better detected using pcBCT compared to digital mammography and breast tomosynthesis. The pcBCT technique offers high-dose efficiency at 5-mGy average glandular dose for the reliable detection of calcification and soft-tissue delineation.

## Diffusion MRI Analysis in Osteosarcoma Xenotransplants Predicts Response to Anticheckpoint Therapy

A relatively novel treatment for osteosarcoma combines a Wee-1 cell cycle checkpoint inhibitor (MK1775) with gemcitabine. The combination was found to increase DNA damage of malignant cells and to induce apoptotic cell death. Foroutan et al. developed a novel approach for evaluating the response to treatment using texture analysis . Prior studies showed that apparent diffusion coefficient (ADC) values could be used to determine lesion cellularity and changes in cellularity before and after treatment. In the present study, diffusion MRI was used to evaluate the response of osteosarcoma to gemcitabine and MK1775 by quantifying tumor volume and assessing ADC properties within tumors. Results showed that increases in ADC parameters correlated with a significant inhibition of tumor growth following treatment. Immunohistochemical analysis of the treated tissue confirmed cell damage and apoptosis. ADC therefore has a potential role as an imaging biomarker for measuring treatment response in the sarcoma patient population.

## Opportunities for Collaboration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Challenges and Solutions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Biological Science Collaborations

## Overview

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Examples

## Quantitative Imaging and Radiomics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Radiogenomics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Opportunities for Collaboration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Challenges and Solutions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Informatics Collaborations

## Overview

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Examples

## PACS

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CAD

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Machine Learning

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Opportunities for Collaboration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Challenges and Solutions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Educational Collaborations

## Overview

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case Examples

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Opportunities for Collaboration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Challenges and Solutions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Hillman B.J.: The past 25 years in medical imaging research: a memoir. Radiology 2000; 214: pp. 11-14.


- 2\. Gore J.C.: Biomedical imaging: current and future trends. Available at: http://medicalphysicsweb.org/cws/article/opinion/60791

- 3\. Johnson D.R., O'Neill B.P.: Glioblastoma survival in the United States before and during the temozolomide era. J Neurooncol 2012; 107: pp. 359-364.


- 4\. Stupp R., Mason W.P., van den Bent M.J., et. al.: Radiotherapy plus concomitant and adjuvant temozolomide for glioblastoma. NEJM 2005; 352: pp. 987-996.


- 5\. Korfiatis P., Kline T.L., Coufalova L., et. al.: MRI texture features as biomarkers to predict MGMT methylation status in glioblastomas. Med Phys 2016; 43: pp. 2835-2844.


- 6\. Kalender W.A., Kolditz D., Stieding C., et. al.: Technical feasibility proof for high-resolution low-dose photon-counting CT of the breast. Eur Radiol 2016; 27: pp. 1081-1086.


- 7\. Foroutan P., Kreahling J.M., Morse D.L., et. al.: Diffusion MRI and novel texture analysis in osteosarcoma xenotransplants predicts response to anti-checkpoint therapy. PLoS ONE 2013; 8: pp. 1-10.


- 8\. Mackay R.I., Burnet N.G., Green S., et. al.: Radiotherapy physics research in the UK: challenges and proposed solutions. British Journal of Radiology 2012; 85: pp. 1354-1362.


- 9\. Lewiss R.E., Chan W., Sheng A.Y., et. al.: Research priorities in the utilization and interpretation of diagnostic imaging: education, assessment, and competency. Acad Emerg Med 2015; 22: pp. 1447-1454.


- 10\. Majithia A., Bhat D.L.: Editorial commentary: bringing precision medicine to intervention: virtually a reality. Trends Cardiovasc Med 2016; 26: pp. 474-476.


- 11\. Huang Y., Liu Z., He L., et. al.: Radiomics signature: a potential biomarker for the prediction of disease-free survival in early-stage (I or II) non-small cell lung cancer. Radiology 2016; 281: pp. 947-957.


- 12\. Jaffe C.: Imaging and genomics: is there a synergy?. Radiology 2012; 264: pp. 329-331.


- 13\. National Research Council (US) Committee on A Framework for Developing a New Taxonomy of Disease : Toward precision medicine: building a knowledge network for biomedical research and a new taxonomy of disease.2011.National Academies PressWashington (DC)


- 14\. Mirnezami R., Nicholson J., Darzi A.: Preparing for precision medicine. N Engl J Med 2012; 366: pp. 489-491.


- 15\. Canonica G., Bachert C., Hellings P., et. al.: Allergen Immunotherapy (AIT): a prototype of precision medicine. World Allergy Organ J. 2015; 8: pp. 31.


- 16\. Comabella M., Sastre-Garriga J., Montalban X.: Precision medicine in multiple sclerosis: biomarkers for diagnosis, prognosis, and treatment response. Curr Opin Neurol 2016; 29: pp. 254-262.


- 17\. Dugas C., Schussler J.M.: Advanced technology in interventional cardiology: a roadmap for the future of precision coronary interventions. Trends Cardiovasc Med 2016; 26: pp. 466-473.


- 18\. Golan D., Staun-Ram E., Miller A.: Shifting paradigms in multiple sclerosis: from disease-specific, through population-specific toward patient-specific. Curr Opin Neurol 2016; 29: pp. 354-361.


- 19\. Xing X., Liang D., Huang Y., et. al.: The application of proteomics in different aspects of hepatocellular carcinoma research. J Proteomics 2016; 145: pp. 70-80.


- 20\. Gillies R.J., Kinahan P.E., Hricak H.: Radiomics: images are more than pictures, they are data. Radiology 2016; 278: pp. 563-577.


- 21\. Gutman D., Cooper L.A.D., Hwang S.N., et. al.: MR imaging predictors of molecular profile and survival: multi-institutional study of the TCGA glioblastoma data set. Radiology 2013; 267: pp. 560-569.


- 22\. Mazurowski M., Zhang J., Peters K.B., et. al.: Computer-extracted MR imaging features are associated with survival in glioblastoma patients. J Neurooncol 2014; 120: pp. 483-488.


- 23\. Mazurowski M., Zhang J., Grimm L.J., et. al.: Radiogenomic analysis of breast cancer: luminal B molecular subtype is associated with enhancement dynamics at MR imaging. Radiology 2014; 273: pp. 365-372.


- 24\. Henzler T., Fink C.: Functional computed tomography in oncology and cardiovascular imaging: a key player in the era of precision medicine and radiogenomics. Eur J Radiol 2015; 84: pp. 2345-2346.


- 25\. Zinn P., Singh S.K., Kotrotsou A., et. al.: Clinically applicable and biologically validated MRI radiomic test method predicts glioblastoma genomic landscape and survival. Neurosurgery 2016; 63: pp. 156-157.


- 26\. Nakamura K., Imafuku N., Nishida T., et. al.: Measurement of the minimum apparent diffusion coefficient (ADCmin) of the primary tumor and CA125 are predictive of disease recurrence for patients with endometrial cancer. Gynecol Oncol 2012; 124: pp. 335-339.


- 27\. Schlett C., Hendel T., Weckbach S., et. al.: Population-based imaging and radiomics: rationale and perspective of the German national cohort MRI study. Rofo 2016; 188: pp. 652-661.


- 28\. Garzón B., Emblem K.E., Mouridsen K., et. al.: Multiparametric analysis of magnetic resonance images for glioma grading and patient survival time prediction. Acta Radiol 2011; 52: pp. 1052-1060.


- 29\. Li H., Zhu Y., Burnside E.S., et. al.: MR imaging radiomics signatures for predicting the risk of breast cancer recurrence as given by research versions of MammaPrint, Oncotype DX, and PAM50 gene assays. Radiology 2016; pp. 152110.


- 30\. Hawkins S., Wang H., Liu Y., et. al.: Predicting malignant nodules from screening CTs. J Thorac Oncol 2016; 11: pp. 2120-2128.


- 31\. Holdsworth C., Badawi R.D., Manola J.B., et. al.: CT and PET: early prognostic indicators of response to imatinib mesylate in patients with gastrointestinal stromal tumor. AJR Am J Roentgenol 2007; 189: pp. W324-W330.


- 32\. Zinn P., Mahajan B., Sathyan P., et. al.: Radiogenomic mapping of edema/cellular invasion MRI-phenotypes in glioblastoma multiforme. PLoS ONE 2011; 6: e25451


- 33\. Gillies R., Kinahan P.E., Hricak H.: Radiomics: images are more than pictures, they are data. Radiology 2016; 278: pp. 563-577.


- 34\. Kuo M., Jamshidi N.: Behind the numbers: decoding molecular phenotypes with radiogenomics—guiding principles and technical considerations. Radiology 2014; 270: pp. 320-325.


- 35\. Mazurowski M.: Radiogenomics: what it is and why it is important?. J Am Coll Radiol 2015; 12: pp. 862-866.


- 36\. Ellingson B.: Radiogenomics and imaging phenotypes in glioblastoma: novel observations and correlation with molecular characteristics. Curr Neurol Neurosci Rep 2015; 15: pp. 506.


- 37\. Herold C., Lewin J.S., Wibmer A.G., et. al.: Imaging in the age of precision medicine: summary of the Proceedings of the 10th Biannual Symposium of the International Society for Strategic Studies in Radiology. Radiology 2016; 279: pp. 226-238.


- 38\. Rutman A., Kuo M.D.: Radiogenomics: creating a link between molecular diagnostics and diagnostic imaging. Eur J Radiol 2009; 70: pp. 232-241.


- 39\. Panth K., Leijenaar R.T., Carvalho S., et. al.: Is there a causal relationship between genetic changes and radiomics-based image features? An in vivo preclinical experiment with doxycycline inducible GADD34 tumor cells. Radiother Oncol 2015; 116: pp. 462-466.


- 40\. Thrall J.: Moreton lecture: imaging in the age of precision medicine. J Am Coll Radiol 2015; 12: pp. 1106-1111.


- 41\. Collins F.S., Varmus H.: A new initiative on precision medicine. N Engl J Med 2015; 372: pp. 793-795.


- 42\. Kumar V., Gua Y., Basu S., et. al.: Radiomics: the process and the challenges. Magn Reson Imaging 2012; 30: pp. 1234-1248.


- 43\. Eisenhauer E., Therasse P., Bogaerts J., et. al.: New response evaluation criteria in solid tumours: revised RECIST guideline (version 1.1). Eur J Cancer 2009; 45: pp. 228-247.


- 44\. Therasse P., Arbuck S.G., Eisenhauer E.A., et. al.: New guidelines to evaluate the response to treatment in solid tumors: European Organization for Research and Treatment of Cancer, National Cancer Institute of the United States, National Cancer Institute of Canada. J Natl Cancer Inst 2000; 92: pp. 205-216.


- 45\. Yip S., Aerts H.J.: Applications and limitations of radiomics. Phys Med Biol 2016; 61: pp. R150-R166.


- 46\. Lambin P., Rios-Velazquez E., Leijenaar R., et. al.: Radiomics: extracting more information from medical images using advanced feature analysis. Eur J Cancer 2012; 48: pp. 441-446.


- 47\. Datta S., Narayana P.A.: A comprehensive approach to the segmentation of multichannel three-dimensional MR brain images in multiple sclerosis. Neuroimage Clin 2013; 2: pp. 184-196.


- 48\. Mansoor A., Bagci U., Foster B., et. al.: Segmentation and image analysis of abnormal lungs at CT: current approaches, challenges, and future trends. Radiographics 2015; 35: pp. 1056-1076.


- 49\. Despotović I., Goossens B., Philips W.: MRI segmentation of the human brain: challenges, methods, and applications. Comput Math Methods Med 2015; 2015: pp. 450341.


- 50\. Wang L., Chitiboi T., Meine H., et. al.: Principles and methods for automatic and semi-automatic tissue segmentation in MRI data. MAGMA 2016; 29: pp. 95-110.


- 51\. Sudarshan V., Mookiah M.R., Acharya U.R., et. al.: Application of wavelet techniques for cancer diagnosis using ultrasound images: a review. Comput Biol Med 2016; 69: pp. 97-111.


- 52\. Hatt M., Tixier F., Pierce L., et. al.: Characterization of PET/CT images using texture analysis: the past, the present… any future?. Eur J Nucl Med Mol Imaging 2016; 44: pp. 151-165.


- 53\. Boone J.: Radiological interpretation 2020: toward quantitative image assessment. Med Phys 2007; 34: pp. 4173-4179.


- 54\. Branstetter B.F.: Basics of imaging informatics. Part 1. Radiology 2007; 243: pp. 656-667.


- 55\. Schafer J.F., Gatidis S., Schmidt H., et. al.: Simultaneous whole-body PET/MR imaging in comparison to PET/CT in pediatric oncology: initial results. Radiology 2014; 273: pp. 220-231.


- 56\. Yu J.P., Kansagra A.P., Thaker A., et. al.: Building for tomorrow today: opportunities and directions in radiology resident research. Acad Radiol 2015; 22: pp. 50-57.


- 57\. van Ginneken B., Schaefer-Prokop C.M., Prokop M.: Computer-aided diagnosis: how to move from the laboratory to the clinic. Radiology 2011; 261: pp. 719-732.


- 58\. Giger M.L., Chan H.P., Boone J.: Anniversary paper: history and status of CAD and quantitative image analysis: the role of Medical Physics and AAPM. Med Phys 2008; 35: pp. 5799-5820.


- 59\. Wallis M.G., Walsh M.T., Lee J.R.: A review of false negative mammography in a symptomatic population. Clin Radiol 1991; 44: pp. 13-15.


- 60\. Birdwell R.L., Ikeda D.M., O'Shaughnessy K.F., et. al.: Mammographic characteristics of 115 missed cancers later detected with screening mammography and the potential utility of computer-aided detection. Radiology 2001; 219: pp. 192-202.


- 61\. Lai S.M., Li X., Biscof W.F.: On techniques for detecting circumscribed masses in mammograms. IEEE Trans Med Imaging 1989; 8: pp. 377-386.


- 62\. Chan H.P., Doi K., Galhotra S., et. al.: Image feature analysis and computer-aided diagnosis in digital radiography. I. Automated detection of microcalcifications in mammography. Med Phys 1987; 14: pp. 538-548.


- 63\. Doi K., Huang H.K.: Computer-aided diagnosis (CAD) and image-guided decision support. Comp Med Imag Graph 2007; 31: pp. 3.


- 64\. Chan H.P., Doi K., Vyborny C.J., et. al.: Improvement in radiologists' detection of clustered microcalcifications on mammograms. The potential of computer-aided diagnosis. Invest Radiol 1990; 25: pp. 1102-1110.


- 65\. Birdwell R.L., Bandodkar P., Ikeda D.M.: Computer-aided detection with screening mammography in a university hospital setting. Radiology 2005; 236: pp. 451-457.


- 66\. Morton M.J., Whaley D.H., Brandt K.R., et. al.: Screening mammograms: interpretation with computer-aided detection—prospective evaluation. Radiology 2006; 239: pp. 375-383.


- 67\. Wang S., Summers R.M.: Machine learning and radiology. Med Image Anal 2012; 16: pp. 933-951.


- 68\. Bauce M., Capuani S., Di Domenico G., et. al.: The GAP Project—GPU for Real-time Applications in High Energy Physics and Medical Imaging. 2014 19th IEEE-NPSS Real Time Conference (Rt)2014.


- 69\. Bryan R.N.: Look Ahead—Machine Learning in Radiology. RSNA.org: RSNA.2016. Noted radiologist Nick Bryan, M.D., Ph.D. discusses the role of Machine Learning (ML) in the radiology practice of tomorrow


- 70\. Summers R.M.: Road maps for advancement of radiologic computer-aided detection in the 21st century. Radiology 2003; 229: pp. 11-13.


- 71\. Summers R.M.: Progress in fully automated abdominal CT interpretation. AJR Am J Roentgenol 2016; 207: pp. 67-79.


- 72\. Raghupathi W., Raghupathi V.: Big data analytics in healthcare: promise and potential. Health information science and systems 2014; 2: pp. 3.


- 73\. Poot J.D., Hartman M.S., Daffner R.H.: Understanding the US medical school requirements and medical students' attitudes about radiology rotations. Acad Radiol 2012; 19: pp. 369-373.


- 74\. Branstetter B.F., Faix L.E., Humphrey A.L., et. al.: Preclinical medical student training in radiology: the effect of early exposure. AJR Am J Roentgenol 2007; 188: pp. W9-W14.


- 75\. Heptonstall N.B., Ali T., Mankad K.: Integrating radiology and anatomy teaching in medical education in the UK—the evidence, current trends, and future scope. Acad Radiol 2016; 23: pp. 521-526.


- 76\. McLachlan J.C., Bligh J., Bradley P., et. al.: Teaching anatomy without cadavers. Med Educ 2004; 38: pp. 418-424.


- 77\. Miles K.A.: Diagnostic imaging in undergraduate medical education: an expanding role. Clin Radiol 2005; 60: pp. 742-745.


- 78\. Pujol S., Baldwin M., Nassiri J., et. al.: Using 3D modeling techniques to enhance teaching of difficult anatomical concepts. Acad Radiol 2016; 23: pp. 507-516.


- 79\. Kong X., Nie L., Zhang H., et. al.: Do three-dimensional visualization and three-dimensional printing improve hepatic segment anatomy teaching? A randomized controlled study. Journal of surgical education 2016; 73: pp. 264-269.


- 80\. Lufler R.S., Zumwalt A.C., Romney C.A., et. al.: Incorporating radiology into medical gross anatomy: does the use of cadaver CT scans improve students' academic performance in anatomy?. Anat Sci Educ 2010; 3: pp. 56-63.


- 81\. Bell F.E., Wilson L.B., Hoppmann R.A.: Using ultrasound to teach medical students cardiac physiology. Adv Physiol Educ 2015; 39: pp. 392-396.


- 82\. Morgan H., Zeller J., Hughes D.T., et. al.: Applied clinical anatomy: the successful integration of anatomy into specialty-specific senior electives. Surgical and radiologic anatomy : SRA. 2016; 39: pp. 95-101.


- 83\. Torres A., Staskiewicz G.J., Lisiecka J., et. al.: Bridging the gap between basic and clinical sciences: a description of a radiological anatomy course. Anat Sci Educ 2016; 9: pp. 295-303.


- 84\. Eisenstein A., Vaisman L., Johnston-Cox H., et. al.: Integration of basic science and clinical medicine: the innovative approach of the cadaver biopsy project at the Boston University School of Medicine. Acad Med 2014; 89: pp. 50-53.