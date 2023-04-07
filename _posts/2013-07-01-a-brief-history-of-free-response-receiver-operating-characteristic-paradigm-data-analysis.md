---
title: A Brief History of Free-Response Receiver Operating Characteristic Paradigm Data Analysis
author: [CL_AT_DevPChakrabortyPhD]
date: 2013-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 20, Issue 7]
tags: [Journals,General Radiology]
---
In the receiver operating characteristic paradigm the observer assigns a single rating to each image and the location of the perceived abnormality, if any, is ignored. In the free-response receiver operating characteristic paradigm the observer is free to mark and rate as many suspicious regions as are considered clinically reportable. Credit for a correct localization is given only if a mark is sufficiently close to an actual lesion; otherwise, the observer's mark is scored as a location-level false positive. Until fairly recently there existed no accepted method for analyzing the resulting relatively unstructured data containing random numbers of mark-rating pairs per image. This report reviews the history of work in this field, which has now spanned more than five decades. It introduces terminology used to describe the paradigm, proposed measures of performance (figures of merit), ways of visualizing the data (operating characteristics), and software for analyzing free-response receiver operating characteristic studies.

The term “free-response” was coined by Egan in 1961 in connection with studies involving the detection of brief audio tone(s) against a white-noise background . The tone(s) could occur at any instant within an active listening interval (eg, while an indicator light was on), and the listener's task was to respond by pressing a button at any instant(s) when a tone(s) was perceived. The listener was uncertain how many true tones, if any, could occur in the active interval and when they might occur. Therefore, the number of responses per active interval could be zero or greater and was a priori unpredictable. With two-dimensional space replacing time, the acoustic study is analogous to a common task in medical imaging, namely, prior to interpreting an image for possible breast cancer, the mammographer does not know a priori how many lesions (ie, cancers) are present, if any, and where they are located. Consequently the image must be searched for regions that appear suspicious for cancer. If the level of suspicion of a particular suspicious region exceeds the minimum clinical reporting threshold, the mammographer reports it (at our institution, they digitally outline and annotate the suspicious region). Conceptually, a screening report consists of the locations of regions that exceed the threshold and the corresponding levels of suspicion \[reported as a Breast Imaging Reporting and Data System rating \]. This type of information defines the free-response paradigm as it applies to medical imaging. At its essence free-response is a search paradigm.

The free-response receiver operating characteristic (FROC) curve was introduced, also in the auditory domain, by Miller as a way of visualizing performance in the free-response task . The importance of the free-response paradigm for radiology applications was first recognized by Bunch et al . Their report describes several ambiguities that arise when the ROC method is applied to a localization task (the interested reader is referred to Table I in their report). A well-known one is the ambiguity when a location-level false positive and a location-level false negative occur on the same image. The two mistakes effectively “cancel” each other in ROC analysis and the image is scored as a “perfect” image-level true positive. In other words, the radiologist was right–a cancer containing image was diagnosed abnormal—but for the wrong reason–an incorrect lesion location was reported.

Bunch et al conducted the first imaging FROC experiment. Under certain assumptions, appropriate to their data, they showed that it was possible to derive ROC operating points from FROC operating points and they also anticipated the alternative FROC (AFROC) curve. The author and colleagues at the University of Alabama at Birmingham were the first to apply the free-response paradigm to a clinical problem, that of comparing a prototype digital chest imaging device to a conventional analog device in a lesion localization task . The method was soon applied in a second study to evaluate a prototype dual-energy chest imaging system by the same manufacturer.

In an FROC study, the number of marks on an image can be zero or more and must be regarded as a modality, reader- and image-dependent random variable. The randomness in the number of marks, in addition to the usual sources of randomness of the ratings due to image sampling and reader sampling, is the main reason why analysis of FROC data has been a challenge. Work in this area has now spanned more than five decades. This report traces the history of developments in free-response analysis.

## FROC data: Mark-Rating pairs

The mark is the location of the suspicious region and the rating is the confidence level that the region contains a lesion. The data analyst decides whether a mark is close enough to a real lesion to qualify as lesion localization (LL)—a location-level “true positive”—and otherwise the mark is classified as non-lesion localization (NL)—a location-level “false positive.” The quotes are intended to emphasize the confusion that can arise if one uses terminology developed for image-level ROC studies to location-level paradigms. What constitutes “close enough” (ie, the proximity criterion or “acceptance radius”) is a clinical decision that should be made based on the application . Two physicians do not need to agree on the exact center of a lesion in order to appropriately assess and treat it. The proximity criterion should be similar for all modalities under comparison as otherwise there would be a bias favoring the modality with the more lenient criterion .

## Data analysis

## Operating Characteristics and Figures-of-Merit

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The FROC curve and associated FOMs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The AFROC curve and associated FOM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimating FPF from FROC data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimating the FOM: Parametric Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Estimating the FOM: Nonparametric Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Other FROC FOMs

## The Λ  Λ   FOM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The EFROC FOM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Should One Count NLs on Both Normal and Abnormal Images?

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## JAFROC software

## FOMs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Significance Testing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Validation Studies

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Egan J.P., Greenburg G.Z., Schulman A.I.: Operating characteristics, signal detectability and the method of free response. J Acoust Soc Am 1961; 33: pp. 993-1007.


- 2\. D'Orsi C.J., Mendelson E.B., Ikeda D.M., et. al.: Breast Imaging Reporting and Data System: ACR BI-RADS – Breast Imaging Atlas.2003.American College of RadiologyReston, VA


- 3\. Miller H.: The FROC curve: a representation of the observer's performance for the method of free response. J Acoust Soc Am 1969; 46: pp. 1473-1476.


- 4\. Bunch P.C., Hamilton J.F., Sanderson G.K., et. al.: A free-response approach to the measurement and characterization of radiographic-observer performance. J Appl Photogr Eng 1978; 4: pp. 166-171.


- 5\. Chakraborty D.P., Breatnach E.S., Yester M.V., et. al.: Digital and conventional chest imaging: a modified ROC study of observer performance using simulated nodules. Radiology 1986; 158: pp. 35-39.


- 6\. Niklason L.T., Hickey N.M., Chakraborty D.P., et. al.: Simulated pulmonary nodules: detection with dual-energy digital versus conventional radiography. Radiology 1986; 160: pp. 589-593.


- 7\. Kallergi M., Carney G.M., Gaviria J.: Evaluating the performance of detection algorithms in digital mammography. Med Phys 1999; 26: pp. 267-275.


- 8\. Chakraborty D.P., Yoon H.J., Mello-Thoms C.: Spatial localization accuracy of radiologists in free-response studies: inferring perceptual FROC curves from mark-rating data. Acad Radiol 2007; 14: pp. 4-18.


- 9\. Haygood T.M., Ryan J., Brennan P.C., et. al.: On the choice of acceptance radius in free-response observer performance studies. Br J Radiol 2013; 86:


- 10\. Chakraborty D.P., Winter L.H.L.: Free-response methodology: alternate analysis and a new observer-performance experiment. Radiology 1990; 174: pp. 873-881.


- 11\. Chakraborty D.P.: Maximum likelihood analysis of free-response receiver operating characteristic (FROC) data. Med Phys 1989; 16: pp. 561-568.


- 12\. Swensson R.G.: Unified measurement of observer performance in detecting and localizing target objects on images. Med Phys 1996; 23: pp. 1709-1725.


- 13\. Chakraborty D.P.: ROC curves predicted by a model of visual search. Phys Med Biol 2006; 51: pp. 3463-3482.


- 14\. Chakraborty D.P.: A search model and figure of merit for observer data acquired according to the free-response paradigm. Phys Med Biol 2006; 51: pp. 3449-3462.


- 15\. Chakraborty D.P.: New developments in observer performance methodology in medical imaging. Semin Nucl Med 2011; 41: pp. 401-418.


- 16\. Metz C.E.: Evaluation of digital mammography by ROC analysis.Doi K.Digital mammography '96.1996.Elsevier ScienceAmsterdam, the Netherlands:pp. 61-68.


- 17\. Berbaum K.S., Franken E.A., Dorfman D.D., et. al.: Satisfaction of search in diagnostic radiology. Invest Radiol 1990; 25: pp. 133-140.


- 18\. Samuelson F.W., Petrick N.: Comparing image detection algorithms using resampling.2006.IEEE International Symposium on Biomedical Imaging: From Nano to MicroArlington, VA, USA 1312–1315


- 19\. Samuelson F.W., Petrick N., Paquerault S.: Advantages and examples of resampling for CAD evaluation.2007.2007 4th IEEE International Symposium on Biomedical Imaging: From Nano to MacroWashington, DC, USA 492–495


- 20\. Bandos A.I., Rockette H.E., Song T., et. al.: Area under the free-response ROC curve (FROC) and a related summary index. Biometrics 2008; 65: pp. 247-256.


- 21\. Gur D., Bandos A.I., Rockette H.E., et. al.: Localized detection and classification of abnormalities on FFDM and tomosynthesis examinations rated under an FROC paradigm. AJR Am J Roentgenol 2011; 196: pp. 737-741.


- 22\. Popescu L.M.: Nonparametric signal detectability evaluation using an exponential transformation of the FROC curve. Med Phys 2011; 38: pp. 5690-5702.


- 23\. Chakraborty D.P., Berbaum K.S.: Observer studies involving detection and localization: modeling, analysis and validation. Med Phys 2004; 31: pp. 2313-2330.


- 24\. Song T., Bandos A.I., Rockette H.E., et. al.: On comparing methods for discriminating between actually negative and actually positive subjects with FROC type data. Med Phys 2008; 35: pp. 1547-1558.


- 25\. Dorfman D.D., Berbaum K.S., Metz C.E.: ROC characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 26\. Hillis S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 27\. Beiden S.V., Wagner R.F., Campbell G.: Components-of variance models and multiple-bootstrap experiments: an alternative method for random-effects, receiver operating characteristic analysis. Acad Radiol 2000; 7: pp. 341-349.


- 28\. Hillis S.L., Obuchowski N.A., Schartz K.M., et. al.: A comparison of the Dorfman-Berbaum-Metz and Obuchowski-Rockette methods for receiver operating characteristic (ROC) data. Stat Med 2005; 24: pp. 1579-1607.


- 29\. Chakraborty D.P.: Validation and statistical power comparison of methods for analyzing free-response observer performance studies. Acad Radiol 2008; 15: pp. 1554-1566.


- 30\. Chakraborty D.P.: Recent developments in free-response methodology.Samei E.Krupinski E.The handbook of medical image perception and techniques.2010.Cambridge University PressCambridge, UK:pp. 216-239.


- 31\. Hillis S.L., Berbaum K.S.: Power estimation for the Dorfman-Berbaum-Metz method. Acad Radiol 2004; 11: pp. 1260-1273.


- 32\. Hillis S.L., Berbaum K.S.: Recent developments in the Dorfman-Berbaum-Metz (DBM) procedure for multi-reader ROC study analysis.2005.Medical Image Perception Society (MIPS) Conference XIWindermere, UK


- 33\. Hillis S.L., Berbaum K.S.: Monte Carlo validation of the Dorfman-Berbaum-Metz method using normalized pseudovalues and less data-based model simplification. Acad Radiol 2005; 12: pp. 1534-1541.


- 34\. Hillis S.L.: A comparison of denominator degrees of freedom methods for multiple observer ROC studies. Stat Med 2007; 26: pp. 596-619.


- 35\. Hillis S.: Multireader ROC analysis.Samei E.Krupinski E.The handbook of medical image perception and techniques.2010.Cambridge University PressCambridge, UK:pp. 204-215.


- 36\. Edwards D.C., Kupinski M.A., Metz C.E., et. al.: Maximum likelihood fitting of FROC curves under an initial-detection-and-candidate-analysis model. Med Phys 2002; 29: pp. 2861-2870.


- 37\. Chakraborty D.P.: Recent developments in imaging system assessment methodology, FROC analysis and the search model. Nucl Instr and Meth A: Accelerators, Spectrometers, Detectors and Associated Equipment 2011; 648: pp. S297-S301.


- 38\. Chakraborty D.P., Yoon H.-J., Mello-Thoms C.: Inverse dependence of search and classification performances in lesion localization tasks. Proc SPIE 2012; 8318: pp. 83180H.


- 39\. Starr S.J., Metz C.E., Lusted L.B., et. al.: Visual detection and localization of radiographic images. Radiology 1975; 116: pp. 533-538.


- 40\. Starr S.J., Metz C.E., Lusted L.B.: Comments on generalization of receiver operating characteristic analysis to detection and localization tasks. Phys Med Biol 1977; 22: pp. 376-379.


- 41\. Swensson R.G., Judy P.F.: Detection of noisy visual targets: models for the effects of spatial uncertainty and signal-to-noise ratio. Percept Psychophys 1981; 29: pp. 521-534.


- 42\. Obuchowski N.A., Lieber M.L., Powell K.A.: data analysis for detection and localization of multiple abnormalities with application to mammography. Acad Radiol 2000; 7: pp. 516-525.


- 43\. Rutter C.M.: Bootstrap estimation of diagnostic accuracy with patient-clustered data. Acad Radiol 2000; 7: pp. 413-419.