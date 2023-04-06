---
title: Three-Dimensional Isotropic Wavelets for Post-Acquisitional Extraction of Latent Images of Atherosclerotic Plaque Components from Micro-Computed Tomography of Human Coronary Arteries
author: [S. David Gertz MD PhD,Bernhard G. Bodmann PhD,Deborah Vela MD,Manos Papadakis PhD,Ibrahim Aboshady MD,Paul Cherukuri PhD,Simon Alexer PhD,Donald J. Kouri PhD,Shikha Baid,Alex A. Gittens,Gregory W. Gladish MD,Jodie L. Conyers PhD,Dianna D. Cody PhD,Lilach Gavish MSc,Reza M. Mazraeshahi MD,Wayne T. Wilner PhD,Lorraine Frazier DSN MS RN NP,Mohammad Madjid MD,Alireza Zarrabi MD,Serhiy Lukovenkov MD,Amany Ahmed MD,James T. Willerson MD,S. Ward Casscells MD]
date: 2007-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 12 SOURCE CL_S_AcademicRadiologyVolume14Issue12 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The capability of wavelet transforms to separate signals into frequency bands is the basis for its use in image compression and storage, data management and transmission, and, recently, extraction of latent images of tissue components from noisy medical images. Analysis of temporal variations of radiofrequency backscatter of intravascular ultrasound with one-dimensional wavelets can detect lipid-laden plaque in coronary arteries with a sensitivity and specificity of >80%. In this study we evaluate the capability of a novel, 3-dimensional isotropic wavelet analysis to perform high resolution, non-directionally biased, statistically reliable, non-invasive discrimination between components of human coronary atherosclerotic plaques in micro-CT.

## Materials and Methods

Coronary artery segments (5–15 mm) were excised at necropsy from 18 individuals with advanced coronary atherosclerosis. Specimens were imaged using a GE Locus SP ex vivo micro-CT scanner and processed for histological correlation (833 sections). The isotropic wavelet constructs were applied to the entire volume of CT data of each arterial segment to distinguish tissue textures of varying scales and intensities. Voxels were classified and plaque characterization achieved by comparing the relative magnitudes of these wavelet constituents to that of several reference plaque tissue components.

## Results

Processing of micro-CT images via these isotropic wavelet algorithms permitted 3-D, color-coded, high resolution, digital discrimination between lumen, calcific deposits, lipid-rich deposits, and fibromuscular tissue providing detail not possible with conventional thresholding based on Hounsfield intensity units. Using the isotropic wavelets (with histology as the gold standard), lipid-rich pools approaching the size of the filter for the isotropic wavelet algorithm (0.25 mm \[250 microns\] in length) were identified with 81% sensitivity and 86% specificity. Calcific deposits, fibromuscular tissue, and lumen equal to or larger than the wavelet filter size were detected without error (100% sensitivity and specificity).

## Conclusion

Isotropic wavelet analysis permits high resolution, multi-dimensional identification of coronary atherosclerotic plaque components in micro-CT with sensitivity and specificity similar to that achieved with data obtained invasively (from IVUS in vivo) using one-dimensional wavelets. Further studies are necessary to test the applicability of this technology to clinical, multi-detector scanners.

## Introduction

The principal pathologic process underlying most acute myocardial infarctions (AMI) is the rupture of an atherosclerotic plaque ( ). The thin-cap fibroatheroma and superficial erosions are the principal histopathological precursors to plaque rupture and acute coronary occlusion in approximately 70% and 25% of cases respectively ( ). Necropsy studies of patients dying after a first, fatal AMI have shown that the luminal cross-sectional-area narrowing by plaque at the site of plaque rupture is less than 75% (equivalent to a 50% reduction in luminal diameter) in approximately one-third of cases ( ). This degree of narrowing is significantly less than the 70% to 80% diameter reduction necessary to reduce coronary flow sufficiently to cause symptoms ( ). Consequently, such patients are not likely to experience pain at rest, or even on exercise, prior to the fatal event, and, hence, will not present to their physician for evaluation. Moreover, even if angiography were to be performed, the search for the most severely narrowed segments of coronary arteries would not necessarily identify the site of origin of these coronary catastrophes ( ).

Multi-detector CT can assess the thickness of the atherosclerotic wall of the major epicardial coronary arteries with acceptable reliability and can readily identify calcific deposits. However, further plaque characterization such as lipid-rich pools and fibrous tissue, a prerequisite for the identification of most atherosclerotic lesions prone to rupture (vulnerable lesions), is not yet a workable reality, even with the 64-detector machines in their current configuration ( ). In fact, pools of lipid-rich pultaceous debris can be mistaken for fibrous tissue approximately 50% of the time even in ex-vivo CT studies ( ). In the current study we test the capability of a recently developed isotropic wavelet analysis algorithm for discrimination of plaque components in CT data.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Comparison of traditional wavelets with isotropic wavelets. Left , Spatial intensity profile of traditional three-dimensional wavelets of filter length 24 (generated with MatLab 7.3, The MathWorks, 2006) obtained from the product of one-dimensional symlets (symmetric wavelets). Right , Spatial intensity profile of three-dimensional isotropic wavelets of filter size 23x23x23. Each image (right and left) shows three mutually orthogonal slices of the intensity profile of a superposition of two wavelets that differ in size by a scale of two (smaller one in the top right portion of each image; larger one centered at the intersection of the planes). In each slice, neutral gray depicts a zero intensity level, lighter than neutral gray corresponds to a positive intensity value, and darkest gray represents negative intensity values. Note that the intensity distribution of the traditional wavelets (left) is a checkerboard pattern aligned along the coordinate axes; whereas the isotropic wavelets (right) do not exhibit preferred directions and hence reduce errors of feature detection that result from image-orientation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ThreeDimensionalIsotropicWaveletsforPostAcquisitionalExtractionofLatentImagesofAtheroscleroticPlaqueComponentsfromMicroComputedTomographyofHumanCoronaryArteries/0_1s20S1076633207003418.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Baseline Clinical Characteristics (n = 18)


Age range 54–80 years Sex 11 men History of: Coronary Artery Disease 14 Diabetes Mellitus 13 Hypertension 12 Chronic Renal Failure 12 Dyslipidemia 10 Obesity 9 Congestive Heart Failure 9 Chronic Obstructive Pulmonary Disease 8 Left Ventricular Hypertrophy 8 Peripheral Artery Disease 6 Abdominal Aortic Aneurysm 2 Smoking 2 Causes of Death Acute Myocardial Infarction  ⁎  4 Congestive Heart Failure 3 Stroke 1 Multisystem Failure 6 Renal Failure 4 Complications of Coronary Artery Bypass Surgery (pneumothorax) 1 Constrictive Pericarditis 1 Liver transplant rejection 1 Pulmonary Embolus following Deep Vein Thrombosis 1 Prostate cancer/cardiac arrest 1 Abdominal Aortic Aneurysm, Post-operative complications 1 Gastrointestinal Bleeding 1

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Measurement and Classification of Lipid-Rich Pools


Sample Dimensions (H×W×L)\* mm Volume (mm  3  ) True Positive False Positive False Negative Sensitivity Specificity 1_none in sample_ 2_none in sample_ 3 0.2×0.6×0.9 0.108 • 1 1 4 0.31×0.6×0.4 0.0744 • 1 1 0.54×0.75×0.36 0.1458 • 0.48×1.93×1.8 1.6675 • 5 0.93×5.6×4.77 24.8421 • 1 0.5 • 6 0.38×0.57×1.17 0.2534 • 1 1 7 0.41×1.3×0.63 0.3358 • 1 1 8_none in sample_ 9_none in sample_ 10_none in sample_ 11 0.71×1.28×0.36 0.3272 • 0 0 0.86×2.13×1.35 2.4729 • 0.44×1.23×0.72 0.3897 • 12 0.44×1.6×1.71 1.2038 • 0.67 1 0.54×1.45×1.17 0.9161 • 0.87×2.13×0.81 1.5010 • 13 0.21×0.96×0.9 0.1814 • 0 0 0.29×0.33×0.9 0.08613 • 0.16×0.3×0.18 0.00864 • 14 0.52×0.93×0.54 0.2611 • 1 1 0.41x0.8x0.54 0.1771 • 0.9×2.46×1.53 3.4627 • 15 0.3×0.52×0.45 0.0702 • 1 1 16 1.29×2.23×0.9 2.5890 • 1 1 17 • 0 0 18 0.31×0.51×1.26 0.1992 • 1 1 Average 0.8058 0.86364

Table 3


Measurement and Classification of Calcific Deposits


Sample Dimensions (H×W×L)\* mm Volume (mm  3  ) True Positive False Positive False Negative Sensitivity Specificity 1 0.09×0.48×0.36 0.01555 • 1 1 1.18×1.57×2.07 3.83488 • 2 3.2×0.52×3.69 6.14016 • 1 1 3 1.35×2.27×2.52 7.72254 • 1 1 0.2×0.65×0.36 0.04680 • 4 0.2×0.66×0.4 0.05280 • 1 1 0.52×1.74×0.63 0.57002 • 5 0.33×5.6×4.59 8.48232 • 6 0.22×0.55×0.9 0.10890 • 1 1 7 0.41×1.3×1.8 0.95940 • 1 1 8 0.21×0.77×0.99 0.16008 • 1 1 0.85×2.3×3.78 7.38990 • 9_none in sample_ 10 0.91×1.84×0.45 0.75348 • 1 1 11 0.71×1.28×0.36 0.32717 • 1 1 1×2.24×2.97 6.65280 • 0.47×1.54×1.35 0.97713 • 12 0.22×0.9×0.54 0.10692 • 1 1 0.36×0.58×0.72 0.15034 • 1.38×1.84×1.98 5.02762 • 0.34×0.4×0.45 0.06120 • 0.61×1.31×1.44 1.15070 • 0.54×1.45×1.17 0.91611 • 13 0.63×1.36×0.72 0.61690 • 1 1 14 0.16×0.5×0.63 0.05040 • 1 1 1.11×1.89×4.23 8.87412 • 15 0.64×0.63×1.17 0.47174 • 1 1 0.1×0.34×0.36 0.01224 • 16 1.02×2.5×3.51 8.95050 • 1 1 17 1.76×2.45×5.76 24.83712 • 1 1 18 0.46×0.73×0.45 0.15111 • 1 1 0.34×0.61×0.81 0.16799 •

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Post-acquisitional analysis of micro-CT images of two human coronary arteries excised at necropsy ( top and bottom ) using 3-dimensional, isotropic, non-directionally biased wavelets. Left (top and bottom): H and E stained histologic sections of human coronary arteries both of which are at the sites of large lipid-rich pools (asterisk) containing numerous cholesterol clefts and, particularly in the bottom frame, remnants of calcific deposits (dark blue granular material) along the periphery of the lipid pool. Middle: (top and bottom): Original, unprocessed micro-CT scans; showing relatively dark, relatively radiolucent areas (asterisk) corresponding to the lipid pools seen on histology. Right (top and bottom): Images processed with isotropic wavelets for selective identification of lipid-rich pools confirmed by histology but seen with difficulty in the unprocessed CT images. The lipid pool in the bottom artery is surrounded by calcific deposits which produce a very bright semicircular crown. The oblique line seen in the lipid pool is an artifact incurred during the initial scanning process.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ThreeDimensionalIsotropicWaveletsforPostAcquisitionalExtractionofLatentImagesofAtheroscleroticPlaqueComponentsfromMicroComputedTomographyofHumanCoronaryArteries/1_1s20S1076633207003418.jpg)

![Figure 3, Post-acquisitional analysis of micro- CT image of a human coronary artery excised at necropsy using color coded, isotropic wavelets showing calcific deposits (blue) intimately associated with previously undetected lipid-rich core. Top: partially decalcified histologic section showing residual calcific deposits within the plaque associated with lipid-rich pultaceous debris (arrow). (H&E stain). Middle: Original, unprocessed micro-CT image; Bottom: micro-CT image after color-coded, isotropic wavelet analysis. Yellow = lipid-rich tissue; blue = calcific deposits; L = lumen.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ThreeDimensionalIsotropicWaveletsforPostAcquisitionalExtractionofLatentImagesofAtheroscleroticPlaqueComponentsfromMicroComputedTomographyofHumanCoronaryArteries/2_1s20S1076633207003418.jpg)

![Figure 4, Color-coded, 3-dimensional, isotropic wavelet analysis of micro-CT scan of human coronary artery excised at necropsy showing calcium-lipid complex. Top: Original micro-CT in 3-slice view. Middle: Conventional threshold-based rendering. Bottom: isotropic wavelet-based tissue segmentation of the original micro-CT data depicted on top. Calcific deposits visible in original (top)(white) and in threshold based rendering (middle)(blue) are seen in the isotropic wavelet transform (bottom)(blue) to be intimately associated with lipid-rich core (yellow). The Lipid-rich core seen in the isotropic wavelet transform is not visible in the original or in the threshold based rendering. Red = lumen. Images are at .028mm isotropic voxel size.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ThreeDimensionalIsotropicWaveletsforPostAcquisitionalExtractionofLatentImagesofAtheroscleroticPlaqueComponentsfromMicroComputedTomographyofHumanCoronaryArteries/3_1s20S1076633207003418.jpg)

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

## Acknowledgements

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Chapman I.: Morphogenesis of occluding coronary artery thrombosis. Arch Pathol 1965; 80: pp. 256-261.


- 2\. Friedman M., Van den Bovenkamp G.J.: The pathogenesis of a coronary thrombus. Am J Pathol 1966; 48: pp. 19-44.


- 3\. Ridolfi R.L., Hutchins G.M.: The relationship between coronary artery lesions and myocardial infarcts: Ulceration of atherosclerotic plaques precipitating coronary thrombosis. Am Heart J 1977; 93: pp. 468-486.


- 4\. Horie T., Sekiguchi M., Hirosawa K.: Coronary thrombosis in pathogenesis of acute myocardial infarction. Br Heart J 1978; 40: pp. 153-161.


- 5\. Falk E.: Plaque rupture with severe pre-existing stenosis precipitating coronary thrombosis. Br Heart J 1983; 50: pp. 127-134.


- 6\. Ambrose J.A., Winters S.L., Stern A., Eng A., Teichholz L.E., Gorlin R., Fuster V.: Angiographic morphology and the pathogenesis of unstable angina pectoris. J Am Coll Cardiol 1985; 5: pp. 609-616.


- 7\. Fuster V., Badimon L., Cohen M., et. al.: Insights into the pathogenesis of acute ischemic syndromes. Circulation 1988; 77: pp. 1213-1220.


- 8\. Alpert J.S.: The pathophysiology of acute myocardial infarction. Cardiology 1989; 76: pp. 85-95.


- 9\. Davies M.J., Bland J.M., Hangartner J.R., et. al.: Factors influencing the presence or absence of acute coronary artery thrombi in sudden ischaemic death. Eur Heart J 1989; 10: pp. 203-208.


- 10\. Falk E.: Morphologic features of unstable atherothrombotic plaques underlying acute coronary syndromes. Am J Cardiol 1989; 63: pp. 114E-120E.


- 11\. Gertz S.D., Kragel A.H., Kalan J.M., et. al., The TIMI Investigators: Comparison of coronary and myocardial morphologic findings in patients with and without thrombolytic therapy during fatal first acute myocardial infarction. Am J Cardiol 1990; 66: pp. 904-909.


- 12\. Gertz S.D., Roberts W.C.: Hemodynamic shear force in rupture of coronary arterial atherosclerotic plaques. Am J Cardiol 1990; 66: pp. 1368-1372.


- 13\. Kragel A.H., Gertz S.D., Roberts W.C.: Morphologic comparison of frequency and types of acute lesions in the major epicardial coronary arteries in unstable angina pectoris, sudden coronary death and acute myocardial infarction. J Am Coll Cardiol 1991; 18: pp. 801-808.


- 14\. Virmani R., Kolodgie F.D., Burke A.P., et. al.: Lessons from sudden coronary death: a comprehensive morphological classification scheme for atherosclerotic lesions. Arterioscler Thromb Vasc Biol 2000; 20: pp. 1262-1275.


- 15\. Kolodgie F.D., Burke A.P., Farb A., et. al.: The thin-cap fibroatheroma: a type of vulnerable plaque: the major precursor lesion to acute coronary syndromes. Curr Opin Cardiol 2001; 16: pp. 285-292.


- 16\. Virmani R., Burke A.P., Kolodgie F.D., Farb A.: Pathology of the thin-cap fibroatheroma: a type of vulnerable plaque. J Interv Cardiol 2003; 16: pp. 267-272.


- 17\. Kolodgie F.D., Virmani R., Burke A.P., et. al.: Pathologic assessment of the vulnerable human coronary plaque. Heart 2004; 90: pp. 1385-1391.


- 18\. McMahon M.M., Brown B.G., Cukingnan R., et. al.: Quantitative coronary angiography: measurement of the “critical” stenosis in patients with unstable angina and single-vessel disease without collaterals. Circulation 1979; 60: pp. 106-113.


- 19\. Castillo M.: From the vulnerable plaque to the vulnerable patient: Imaging and clinical implications. Acad Radiol 2006; 13: pp. 1177-1179.


- 20\. Schoenhagen P., Halliburton S.S., Stillman A.E., et. al.: Noninvasive imaging of coronary arteries: current and future role of multi-detector row CT. Radiology 2004; 232: pp. 7-17.


- 21\. Schoepf U.J., Becker C.R., Ohnesorge B.M., et. al.: CT of coronary artery disease. Radiology 2004; 232: pp. 18-37.


- 22\. Schoenhagen P., Stillman A.E., Halliburton S.S., et. al.: Non-invasive coronary angiography with multi-detector computed tomography: comparison to conventional X-ray angiography. Int J Cardiovasc Imaging 2005; 21: pp. 63-72.


- 23\. Schroeder S., Kuettner A., Wojak T., et. al.: Non-invasive evaluation of atherosclerosis with contrast enhanced 16 slice spiral computed tomography: results of ex vivo investigations. Heart 2004; 90: pp. 1471-1475.


- 24\. Hubbard B.B.: Second ed1998. A.K Peters, Wellesley, Massachusetts


- 25\. Wang J.Z.: Wavelets and imaging informatics: a review of the literature. J Biomed Inform 2001; 34: pp. 129-141.


- 26\. Skodras A.C., Ebrahimi T.: The JPEG2000 still image coding: An overview. IEEE Trans Consum Elect 2000; 46: pp. 1103-1127.


- 27\. Adams M.D., Ward R.: Wavelet Transforms in the JPEG-2000 Standard.Proceedings of the IEEE Pacific Rim Conference on Communications, Computers and Signal Processing.2001.pp. 160-163. Victoria, BC, Canada.  http://www.ece.ubc.ca/∼mdadams/papers/pacrim2001.pdf

- 28\. Santa-Cruz D., Ebrahimi T., Askelof J., et. al.: JPEG 2000 still image coding versus other standards.2000. Proc. SPIE July; 4115.  http://www.jpeg.org/public/wg1n1816.pdf

- 29\. Elzinga J., Feenstra K., Aboufadel F.: 2001.Grand Valley State UniversityAllendale, MI December 4.  http://www.gvsu.edu/math/wavelets/student\_work/EF/

- 30\. Frankewitsch T., Sohnlein S., Muller M., Prokosch H.U.: Computed Quality Assessment of MPEG4-compressed DICOM Video Data. Stud Health Technol Inform 2005; 116: pp. 447-452.


- 31\. Nachtergaele L., Vanhoof B., Peon M., et. al.: Implementation of a scalable MPEG-4 wavelet-based visual texture compression system.1999.pp. 333-336. Proc. 36th Design Automation Conf., New Orleans, LA, June.  http://delivery.acm.org/10.1145/310000/309948/p333-nachtergaele.pdf?key1=309948&key2=7872764311&coll=GUIDE&dl=GUIDE&CFID=63076545&CFTOKEN=74798681

- 32\. Segal N.: 2001. Streaming Media World, June 19.  http://streamingmediaworld.com/video/docs/MPEG4/

- 33\. Turkheimer F.E., Brett M., Aston J.A.: Statistical modeling of positron emission tomography images in wavelet space. J. Cereb. Blood Flow Metab 2000; 20: pp. 1610-1618.


- 34\. Turkheimer F.E., Aston J.A., Banati R.B., et. al.: A linear wavelet filter for parametric imaging with dynamic PET. Med. Imaging 2003; 22: pp. 289-301.


- 35\. Bullmore E., Fadili J., Breakspear M.: Wavelets and statistical analysis of functional magnetic resonance images of the human brain. Stat Methods Med. Res 2003; 12: pp. 375-399.


- 36\. Bullmore E., Fadili J., Maxim V., et. al.: Wavelets and functional magnetic resonance imaging of the human brain. Neuroimage 2004; 23: pp. S234-S249.


- 37\. Haase H., Junger M.: An expert system for cutaneous blood flow in melanocytic skin lesions. Clin Hemorheol Microcirc 2004; 30: pp. 253-262.


- 38\. Kavitha A., Ramakrishnan S.: Analysis on the erythrocyte shape changes using wavelet transforms. Clin Hemorheol Microcirc 2005; 33: pp. 327-335.


- 39\. Lucier B.J., Kallergi M., Qian W., et. al.: Wavelet compression and segmentation of digital mammograms. J Digit Imaging 1994; 7: pp. 27-38.


- 40\. Wang T.C., Karayiannis N.B.: Detection of microcalcifications in digital mammograms using wavelets. IEEE Trans Med Imaging 1998; 17: pp. 498-509.


- 41\. Swiniarski R., Swiniarska A.: Comparison of feature extraction and selection methods in mammogram recognition. Ann NY Acad Sc 2002; 980: pp. 116-124.


- 42\. Hwang H.G., Choi H.J., Lee B.I.: Multi-resolution wavelet-transformed image analysis of histological sections of breast carcinomas. Cell Oncol 2005; 27: pp. 237-244.


- 43\. Murashige A., Hiro T., Fujii T., et. al.: Detection of Lipid-laden atherosclerotic plaque by wavelet analysis of radiofrequency intravascular ultrasound signals. J Am Coll Cardiol 2005; 45: pp. 1954-1960.


- 44\. Papadakis M.A., Gogoshin G., Kakadiaris I., et. al.: Non-separable radial frame multiresolution analysis in multidimensions. Numer Funct Anal Optim 2003; 24: pp. 907-928.


- 45\.  Papadakis MA, Gogoshin G, Kakadiaris I, et al. Non-separable radial frame multiresolution analysis in multidimensions and the isotropic fast wavelet transform. In: Laine A, Aldroubi M, Unser M, eds. SPIE Proceedings. Nov. 14, 2003; 2003; Vol. 5207: Wavelets: Applications in Signal and Image Processing X, pp 631–42.


- 46\. Bodmann B.G., Papadakis M., Kouri D., et. al.: Frame isotropic multiresolution analysis for Micro-CT scans of coronary arteries.Papadakis M.Laine A.F.Unser M.2005. 59141O-1-12


- 47\. Stary H.C., Chandler A.B., Dinsmore R.E.: A definition of advanced types of atherosclerotic lesions and a histological classification of atherosclerosis. Art Thromb Vasc Biol 1995; 15: pp. 1512-1531.


- 48\. Feldkamp L.A., Davis L.C., Kress J.W.: Practical cone-beam algorithm. J Opt Soc Am. A: Optics and Image Science 1984; 1: pp. 612-619.


- 49\. McCullagh P., Nelder J.A.: Generalized linear models.1989.Chapman and HallLondon


- 50\. Gertz S.D., Cherukuri P., Bodmann B.G., et. al.: Usefulness of multidetector computed tomography for noninvasive evaluation of coronary arteries in asymptomatic patients. Am J Cardiol 2006; 97: pp. 287-293.


- 51\. Virmani R., Burke A.P., Kolodgie F.D., Farb A.: Vulnerable plaque: the pathology of unstable coronary lesions. J Interv Cardiol 2002; 15: pp. 439-446.


- 52\. Virmani R., Burke A.P., Farb A., Kolodgie F.D.: Pathology of the vulnerable plaque. J Am Coll Cardiol 2006; 47: pp. C13-C18.


- 53\. Ehara S., Kobayashi Y., Yoshiyama M.: Spotty calcification typifies the culprit plaque in patients with acute myocardial infarction: an intravascular ultrasound study. Circulation 2004; 10: pp. 3424-3429.


- 54\. Burke A.P., Weber D., Kolodgie F.D., et. al.: Pathophysiology of calcium deposition in coronary arteries. Herz 2001; 26: pp. 239-244.


- 55\. Naghavi M., Libby P., Falk E., et. al.: From vulnerable plaque to vulnerable patient: a call for new definitions and risk assessment strategies: Part II. Circulation 2003; 108: pp. 1772-1778.