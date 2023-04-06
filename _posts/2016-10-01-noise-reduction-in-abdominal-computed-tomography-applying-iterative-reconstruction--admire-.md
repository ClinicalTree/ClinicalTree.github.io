---
title: Noise Reduction in Abdominal Computed Tomography Applying Iterative Reconstruction (ADMIRE)
author: [Frank Schaller,Martin Sedlmair,Rainer Raupach,Michael Uder,Michael Lell]
date: 2016-10-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 23, Issue 10 SOURCE CL_S_AcademicRadiologyVolume23Issue10 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The study aimed to compare image quality of filtered back projection (FBP) and iterative reconstruction (advanced modeled iterative reconstruction, ADMIRE) in contrast-enhanced computed tomography (CT) of the abdomen, and to assess the differences of reconstructions according to these methods. It also aimed to investigate the potential for noise reduction of ADMIRE for different reconstructed slice thicknesses.

## Materials and Methods

CT data of the abdomen and pelvis were acquired using a 128-slice single-source CT system using automated kV selection and tube current adaption based on patients' anatomy. Raw data sets from patients scanned at 100 kV were selected, and images were reconstructed with slice thicknesses of 1 mm, 3 mm, and 5 mm, both with FBP and ADMIRE. Filter strength F1, F3, and F5 of the ADMIRE algorithm and the corresponding reconstruction kernels were used. In total, 58 raw data sets from 17 patients were used to reconstruct from the same raw data FBP and ADMIRE images, representing identical body regions. Identical regions of interest were placed at the same position of up to four images and image noise was measured. Differences of reconstructed images and detail preservation were tested using an image subtraction technique, and subjective image quality was assessed using a 5-point Likert scale.

## Results

On average, for 1-mm slice thickness, noise reduction was 9.15% ± 2.4% with filter strength level F1, 30.2% ± 3.4% with F3, and 54.4% ± 7.0% with F5 as compared to FBP. For a slice thickness of 3 mm, noise reduction was 8.5% ± 3.7% with F1, 28.6% ± 3.9% with F3, and 52.2% ± 9.1% with F5. For 5 mm, the corresponding values are 8.9% ± 2.7%, 31.4% ± 2.8%, and 52.7% ± 7.7%. On subtraction images, edge information of tissue classes with a high attenuation gradient was found, but structures with small differences in attenuation were not detectable on subtraction images, confirming that no relevant details were lost in the iterative reconstruction process.

## Conclusions

ADMIRE is able to reduce image noise considerably (up to 50%) without any obvious negative impact on lesion depiction as assessed visually. Noise reduction of ADMIRE seems to be independent of slice thickness.

## Introduction

Dose reduction is a permanent challenge in clinical computed tomography (CT). Despite the fact that radiation dose of a single CT examination is far too low to induce deterministic tissue damage, there is increasing concern about the statistical risk of cancer induction , and cell experiments could demonstrate that there is a strong correlation between radiation exposure and DNA double-strand breaks in lymphocytes . The cumulative effects of x-ray exposure from repeated CT examinations are of further concern. The reason why alertness of medical scientists, both physicians and physicists, is focused on CT is twofold: First, the benefit of CT in clinical diagnosis is outstanding, and therefore the number of examinations is steadily rising; and second, the radiation exposure is usually much higher than with conventional x-ray examinations . To get a rough idea of the order of radiation exposure of a CT examination, the average environmental exposure per year from natural sources is often referenced. Natural background radiation, mainly cosmological radiation and radioactive materials (eg, radon), is in the order of 4 mSv per year, whereas a single CT examination of the abdomen and pelvis at 120 kV is associated with about 8–11 mSv. Although the frequency of CT is about 7% of all medical x-ray examinations, it accounts for 60% of the collective effective dose .

The European Commission founded the European ALARA (As Low As Reasonably Achievable) Network in 1996 in order to support and coordinate research on imaging optimization and radiation protection. There is a large variety of dose reduction measures, starting from very basic ones (critical review of the indication, selection of the most appropriate imaging modality, and restriction to the relevant body region) to more advanced ones concerning the data acquisition process (automated exposure control, on-line tube current modulation, attenuation-based kV selection, prefiltering and spectral shaping, and dynamic collimation) and advanced image reconstruction techniques (3D adaptive filtering and iterative reconstruction \[IR\]) . Only recently, IR, which has been implemented in nuclear medicine for a long time, gained importance in diagnostic CT. IR avoids some of the drawbacks of filtered back projection (FBP) and is superior regarding artifacts and noise at the cost of high computational demands .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, A 78-year-old patient with colorectal cancer and multiple liver metastases. Images are reconstructed with a slice thickness of 1 mm: (a) FBP, (b) ADMIRE F1, (c) ADMIRE F3, and (d) ADMIRE F5. Noise reduction is 11% (F1), 34% (F3), and 60% (F5) compared to FBP; CNRs (contrast-to-noise ratios) are 2.1 (FBP), 2.4 (F1), 3.2 (F3), and 5.3 (F5). FBP, filtered back projection.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/NoiseReductioninAbdominalComputedTomographyApplyingIterativeReconstructionADMIRE/0_1s20S1076633216300952.jpg)

![Figure 2, A 78-year-old patient with colorectal cancer and multiple liver metastases (same patient as in Fig 1 ). Images are reconstructed with a slice thickness of 5 mm: (a) FBP, (b) ADMIRE F1, (c) ADMIRE F3, and (d) ADMIRE F5. Noise reduction is 11% (F1), 34% (F3), and 59% (F5) compared to FBP; CNRs are 4.4 (FBP), 5.0 (F1), 6.7 (F3), and 10.6 (F5). FBP, filtered back projection.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/NoiseReductioninAbdominalComputedTomographyApplyingIterativeReconstructionADMIRE/1_1s20S1076633216300952.jpg)

Table 1


Noise Ratios q for Different Filter Strengths and Slice Thicknesses


F1T1 F1T3 F1T5 F3T1 F3T3 F3T5 F5T1 F5T3 F5T5 Third quartile 0.9153 0.9349 0.9226 0.7021 0.7245 0.7040 0.4781 0.5080 0.4945 Median 0.9014 0.9090 0.9045 0.6853 0.7103 0.6877 0.4405 0.4544 0.4609 Mean

SD 0.9085

0.024 0.9149

0.037 0.9106

0.027 0.6976

0.034 0.7139

0.039 0.6858

0.028 0.4561

0.070 0.4781

0.091 0.4725

0.077 First quartile 0.8923 0.8918 0.8900 0.6789 0.6865 0.6589 0.4150 0.4272 0.4161

SD, standard deviation.


![Figure 3, Boxplots of the noise ratios q = σ ADMIRE /σ FBP for the various F-T-categories. Categories are a combination of filter strengths F1, F3, and F5 and slice thicknesses T1, T3, and T5 (in mm).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/NoiseReductioninAbdominalComputedTomographyApplyingIterativeReconstructionADMIRE/2_1s20S1076633216300952.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Subtraction images to demonstrate the effects of the iterative reconstruction algorithm (window: C0/W100 HU): (a) ADMIRE F1 – FBP; (b) ADMIRE F3 – FBP; and (c) ADMIRE F5 – FBP. In the large regions of interest, which include both the metastasis and normal liver tissue, the mean attenuation coefficient µ is close to 0 in all subtraction images, whereas the extracted noise σ increases at higher filter strengths. ROI measurements: (a) µ = 0.035 HU, σ = 3.01 HU; (b) µ = 0.139 HU, σ = 9.02 HU; and (c) µ = 0.140 HU, σ = 16.02 HU. FBP, filtered back projection; ROI, region of interest.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/NoiseReductioninAbdominalComputedTomographyApplyingIterativeReconstructionADMIRE/3_1s20S1076633216300952.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## Iterative Reconstruction Algorithm ADMIRE

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Algorithm scheme of ADMIRE.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/NoiseReductioninAbdominalComputedTomographyApplyingIterativeReconstructionADMIRE/4_1s20S1076633216300952.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Brenner D.J., Shuryak I., Einstein A.J.: Impact of reduced patient life expectancy on potential cancer risks from radiologic imaging. Radiology 2011; 261: pp. 193-198.


- 2\. Kuefner M.A., Grudzenski S., Hamann J., et. al.: Effect of CT scan protocols on x-ray-induced DNA double-strand breaks in blood lymphocytes of patients undergoing coronary CT angiography. Eur Radiol 2010; 20: pp. 2917-2924.


- 3\. Brenner D.J., Hall E.J.: Computed tomography—an increasing source of radiation exposure. N Engl J Med 2007; 357: pp. 2277-2284.


- 4\. RadiologyInfo.org : Radiation dose in x-ray and CT-exams. Available at http://www.radiologyinfo.org/en/pdf/sfty\_xray.pdf

- 5\. May M.S., Wuest W., Lell M.M., et. al.: Aktuelle strategien zur dosisreduktion in der computertomographie. Radiologe 2012; 52: pp. 905-913.


- 6\. Ehman E.C., Yu L., Manduca A., et. al.: Methods for clinical evaluation of noise reduction techniques in abdominopelvic CT 1. Radiographics 2014; 34: pp. 849-862.


- 7\. Pontana F., Pagniez J., Flohr T., et. al.: Chest computed tomography using iterative reconstruction vs filtered back projection (part 1): evaluation of image noise reduction in 32 patients. Eur Radiol 2011; 21: pp. 627-635.


- 8\. Beister M., Kolditz D., Kalender W.A.: Iterative reconstruction methods in X-ray CT. Phys Med 2012; 28: pp. 94-108.


- 9\. Pickhardt P.J., Lubner M.G., Kim D.H., et. al.: Abdominal CT with model-based iterative reconstruction (MBIR): initial results of a prospective trial comparing ultralow-dose with standard-dose imaging. AJR Am J Roentgenol 2012; 199: pp. 1266-1274.


- 10\. Yamada Y., Jinzaki M., Niijima Y., et. al.: CT dose reduction for visceral adipose tissue measurement: effects of model-based and adaptive statistical iterative reconstructions and filtered back projection. AJR Am J Roentgenol 2015; 204: pp. W677-W683.


- 11\. Lell M., Wildberger J., Alkhadi H., et. al.: Evolution in computed tomography: the battle for speed and dose. Invest Radiol 2015; 50: pp. 629-644.


- 12\. Lim H.-J., Chung M.J., Shin K.E., et. al.: Model Based Iterative Reconstruction in Chest CT: influence to the low-contrast high spatial frequency lung abnormalities in diffuse interstitial lung disease. In: Radiological Society of North America 2013 Scientific Assembly and Annual Meeting; Available at http://www.researchgate.net/publication/266094460\_Model\_Based\_Iterative\_Reconstruction\_in\_Chest\_CT\_Influence\_to\_the\_Low-contrast\_High\_Spatial\_Frequency\_Lung\_Abnormalities\_in\_Diffuse\_Interstitial\_Lung\_Disease Accessed November 16, 2015


- 13\. Chang W., Lee J.M., Lee K., et. al.: Assessment of a model-based, iterative reconstruction algorithm (MBIR) regarding image quality and dose reduction in liver computed tomography. Invest Radiol 2013; 48: pp. 598-606.


- 14\. Husarik D.B., Marin D., Samei E., et. al.: Radiation dose reduction in abdominal computed tomography during the late hepatic arterial phase using a model-based iterative reconstruction algorithm. Invest Radiol 2012; 47: pp. 468-474.


- 15\. Solomon J., Wilson J., Samei E.: Characteristic image quality of a third generation dual-source MDCT scanner: noise, resolution, and detectability. Med Phys 2015; 42: pp. 4941-4953.


- 16\. Schindera S.T., Odedra D., Raza S.A., et. al.: Iterative reconstruction algorithm for CT: can radiation dose be decreased while low-contrast detectability is preserved?. Radiology 2013; 269: pp. 511-518.


- 17\. Saiprasad G., Peskin A., Siegel E., et. al.: Evaluation of low-contrast detectability of iterative reconstruction across multiple institutions, CT scanner manufacturers and radiation exposure levels. Radiology 2015; 19: pp. 1412.


- 18\. Patino M., Fuentes J., Singh S., et. al.: Iterative reconstruction techniques in abdominopelvic CT: technical concepts and clinical implementation. AJR Am J Roentgenol 2015; 205: pp. W19-W31.


- 19\. Hell M., Bittner D., Schuhbaeck A., et. al.: Prospectively ECG-triggered high-pitch coronary angiography with third-generation dual-source CT at 70 kVp tube voltage: feasibility, image quality, radiation dose, and effect of iterative reconstruction. J Cardiovasc Comput Tomogr 2014; 8: pp. 418-425.


- 20\. Deseive S., Chen M., Korosglou G., et. al.: Prospective randomized trial on radiation dose estimates of CT angiography applying iterative image reconstruction: the PROTECTION V Study. JACC Cardiovasc Imaging 2015; 8: pp. 888-896. pii:S1936-878X(15)00299-S


- 21\. Willemink M., Takx R., de Jong P., et. al.: The impact of CT radiation dose reduction and iterative reconstruction algorithms from four different vendors on coronary calcium scoring. Eur Radiol 2014; 24: pp. 2201-2212.


- 22\. Gordic S., Desbiolles L., Sedlmair M., et. al.: Optimizing radiation dose by using advanced modelled iterative reconstruction in high-pitch coronary CT angiography. Eur Radiol 2015; 26: pp. 459-468.


- 23\. Solomon J., Mileto A., Ramirez-Giraldo J.S.E.: Diagnostic performance of an advanced modeled iterative reconstruction algorithm for low-contrast detectability with a third-generation dual-source multidetector CT scanner: potential for radiation dose reduction in a multireader study. Radiology 2015; 275: pp. 735-745.


- 24\. Thibault J.-B., Sauer K.D., Bouman C.A., et. al.: A three-dimensional statistical approach to improved image quality for multislice helical CT. Med Phys 2007; 34: pp. 4526-4544.


- 25\. Clinthorne N.H., Chiao P.C., Rogers W.L., et. al.: Preconditioning methods for improved convergence rates in iterative reconstructions. IEEE Trans Med Imaging 1993; 12: pp. 78-83.


- 26\. Bruder H., Raupach R., Sunnegardh J., et. al.: Adaptive iterative reconstruction. Phys Med Imaging 2011; 7961: 79610J-1–79610J-12