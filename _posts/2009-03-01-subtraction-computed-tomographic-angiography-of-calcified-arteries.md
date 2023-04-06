---
title: Subtraction Computed Tomographic Angiography of Calcified Arteries
author: [Peter J. Yim PhD,John L. Nosher MD,Anthony Burgos MD,Ihab Haddadin MD]
date: 2009-03-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 16, Issue 3 SOURCE CL_S_AcademicRadiologyVolume16Issue3 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The technique of subtraction computed tomographic angiography (sCTA) has been proposed for the evaluation of atherosclerotic disease to address limitations in CTA in highly calcified arteries. However, sCTA has not gained acceptance in clinical practice, in part, due to image artifacts caused by patient motion that occur between the acquisition of the two component images. The purpose of this study was to evaluate the effectiveness of computational image co-registration to obtain sCTA.

## Materials and Methods

The study was conducted using a semi-automated implementation of the mutual information (MI) registration algorithm. The results of sCTA were evaluated quantitatively in a phantom representing a calcified artery. Technical success of sCTA was evaluated in 14 calcified arterial segments in two patients. An observer study was carried out to determine interobserver agreement in the interpretation of sCTA. Qualitative observations were made between sCTA and CTA.

## Results

Computation time for performing the co-registration for each 2-cm calcification is less than 1 second. The necessary user interaction required minimal expertise. Measurements of the degree of stenosis in the calcified artery phantom agreed to within 8 ± 4% of gold-standard measurements. Technical success was demonstrated in all calcifications. Strong interobserver agreement was obtained for the detection of hemodynamically significant stenoses (κ = 0.86). Several apparent pitfalls in the interpretation of CTA in calcified arteries were noted that could potentially be obviated by sCTA.

## Conclusions

The study supports the use of a straight-forward implementation of the MI algorithm and provides preliminary evidence validating the use of sCTA in the setting of atherosclerotic disease of the lower extremities.

The accuracy of the computed tomographic angiographic (CTA) examination may be degraded by the presence of calcified plaque. Detection and quantification of such calcification may have value in the diagnosis and therapy planning of this disease ( ); however, in relation to the primary criteria of disease severity (the degree of stenosis), such calcifications are simply a nuisance. Calcifications appear in CTA as small objects with a high computed tomographic density that can sometimes approach that of bone. In the cross-sectional view, the lumenal region of the calcified artery may appear distinctive as a region with intermediate intensity surrounded either partially or completely by a high-intensity region corresponding to the calcification. Thus, common radiologic practice for assessing calcified arteries in CTA is to review the cross-sectional images. However, even with this approach, recent studies suggest that detection of hemodynamically significant stenoses in the presence of calcified plaque can be inaccurate. For example, in the study of Willmann et al ( ), the presence of calcification tended to cause an overestimation of the degree of stenosis. In their study of 39 consecutive patients with 35 hemodynamically significant stenoses, overestimation of stenosis occurred in 26 vessel segments. In 20 of the cases in which the stenosis was overestimated, the primary cause of overestimation of stenosis was the presence of calcification. Ouwendink et al ( ) found that wall calcifications in CTA often limited the diagnostic value of CTA and were a statistically significant predictor of when a patient would need additional imaging studies.

In the study presented here, we elaborate on a promising new approach to computed tomographic angiography involving, in essence, digital subtraction of the non-contrast computed tomography from the computed tomography angiography. Our study addresses practical considerations that arise for implementation of this technique including, most importantly, the need to correct for patient motion that occurs between the acquisition of the noncontrast CT (ncCT) and the computed tomographic angiography. A computational image registration algorithm plays a large role in this respect. The study also involves robust validation of the methodology including a study using a realistic phantom as well as observations from a clinical study.

## Materials and methods

## Patients

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Calcified-artery Phantom

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Schematic of the calcified artery phantom. The phantom represents the relevant four elements of the imaging field: lumen (L), calcification (C), vessel wall (VW), and extravascular space (EVS). The phantom was constructed with two stenoses of varying stenosis length (SL) and stenosis diameter (SD).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SubtractionComputedTomographicAngiographyofCalcifiedArteries/0_1s20S1076633208004029.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Acquisition: Vascular Phantom

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Acquisition: Clinical Cases

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Registration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Image regions included in co-registration of noncontrast computed tomography and the computed tomographic angiography. The regions are based on a series of two or more points along the calcified artery identified by the user. A box is then constructed, such as a pair of consecutive points (P1, P2), such that those points are located at the diametrically opposite corners. The box is then extended outwards by 0.5 and 1.0 cm to form image subvolumes in computed tomographic angiography (SVCTA) and in noncontrast computed tomogaphy (SVNCCT).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SubtractionComputedTomographicAngiographyofCalcifiedArteries/1_1s20S1076633208004029.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Analysis: Vascular Phantom

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Observer Study: Clinical Cases

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Subtraction computed tomographic angiography of calcified artery phantom. The images represent the results of simulation of the computed tomographic angiography ( a,e ), the noncontrast computed tomography ( b,f ), and the subtraction computed tomographic angiography ( c,g ). Reference images ( d,h ) were obtained from imaging of the phantom without calcification material present.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SubtractionComputedTomographicAngiographyofCalcifiedArteries/2_1s20S1076633208004029.jpg)

Table 1


Results from the Phantom Study: Measurements from Subtracted Computed Tomograpic Angiography (sCTA) Compared with Gold Standard (GS) Measurements


GS Stenosis (%) sCTA Stenosis (%) Absolute Error (%) Model #1 32 27 5 Model #2 49 60 11 Mean ± SD — — 8 ± 4

SD, standard deviation.


![Figure 4, Effect of transformation error in the initialization of the image registration on the accuracy of the image transformation following registration. Only the translational component of the image transformation is represented in the error. The true image transformation was estimated as that obtained from a best guess initialization followed by mutual information registration.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SubtractionComputedTomographicAngiographyofCalcifiedArteries/3_1s20S1076633208004029.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Subtraction computed tomographic angiography in the territory of the superficial femoral artery. Subtraction computed tomographic angiography ( c ) obtained from computed tomographic angiography ( a ) and noncontrast computed tomography ( b ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SubtractionComputedTomographicAngiographyofCalcifiedArteries/4_1s20S1076633208004029.jpg)

Table 2


Breakdown of Outcomes from Interobserver Agreement Study for the Detection of Stenosis


Negative Positive Total Negative 6 0 6 Positive 1 5 6 Total 7 5 12 segments

Negative, number of arterial segments in which stenoses was not detected; Positive, number of arterial segments in which stenosis was detected.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Types of calcified arterial segments in which computed tomographic angiography is likely to be misinterpreted. One such type is where the calcification is highly inhomogenous as shown in the computed tomographic angiogram ( b ) and noncontrast computed tomography ( c ) and whose position is indicated by the top line in ( a ). Another type is where the calcification concentrically surrounds the lumen as shown in the computed tomographic angiogram ( d ) and the noncontrast computed tomography ( e ) and whose position is indicated by the bottom line in ( a ). In the first type of arterial segment, the degree of stenosis may be underestimated in computed tomographic angiography. In the second type of arterial segment, total occlusion may be suspected based on reading of the computed tomographic angiogram.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SubtractionComputedTomographicAngiographyofCalcifiedArteries/5_1s20S1076633208004029.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Study Limitations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Rutten A., Isgum I., Prokop M.: Coronary calcification: effect of small variation of scan starting position on Agatston, volume, and mass scores. Radiology 2008; 246: pp. 90-98..


- 2\. Suzuki M., Ozaki Y., Komura S., Nakanishi A.: Intracranial carotid calcification on CT images as an indicator of atheromatous plaque: analysis of high-resolution CTA images using a 64-multidetector scanner. Radiat Med 2007; 25: pp. 378-385.


- 3\. Maldonado T.S.: What are current preprocedure imaging requirements for carotid artery stenting and carotid endarterectomy: have magnetic resonance angiography and computed tomographic angiography made a difference?. Semin Vasc Surg 2007; 20: pp. 205-215.


- 4\. Willmann J.K., Baumert B., Schertler T., et. al.: Aortoiliac and lower extremity arteries assessed with 16-detector row CT angiography: prospective comparison with digital subtraction angiography. Radiology 2005; 236: pp. 1083-1093.


- 5\. Ouwendijk R., Kock M.C., van Dijk L.C., van Sambeek M.R., Stijnen T., Hunink M.G.: Vessel wall calcifications at multi-detector row CT angiography in patients with peripheral arterial disease: effect on clinical utility and clinical predictors. Radiology 2006; 241: pp. 603-608.


- 6\. Pluim J.P., Maintz J.B., Viergever M.A.: Mutual-information-based registration of medical images: a survey. IEEE Trans Med Imaging 2003; 22: pp. 986-1004.


- 7\. Poletti P.A., Rosset A., Didier D., Bachmann P., Verdun F.R., et. al.: Subtraction CT angiography of the lower limbs: a new technique for the evaluation of acute arterial occlusion. ASR Am J Roentgenol 2004; 183: pp. 1445-1448.


- 8\. Kwon S.M., Kim Y.S., Kim T., Ra J.B.: Novel digital subtraction CT angiography based on 3D registration and refinement. SPIE Med Imaging 2004; 5370: pp. 1156-1165.


- 9\. Loeckx D., Drisis S., Maes F., Vandermeulen D., Marchal G., Suetens P.: Removal of plaque and stent artifacts in subtraction CT angiography using nonrigid registration and a volume penalty. Conf Proc IEEE Eng Med Biol Soc 2005; 4: pp. 4294-4297.


- 10\. Vogel W.V., Schinagl D.A., Van Dalen J.A., Kaanders J.H., Oyen W.J.: Validated image fusion of dedicated PET and CT for external beam radiation therapy in the head and neck area. Q J Nucl Med Mol Imaging 2008; 52: pp. 74-83.


- 11\. Bani-Hashemi A.R., Krishnan A., Samaddar S.: Warped matching for digital subtraction of CT-angiography studies. Proceedings SPIE 1996; 2710: pp. 428-437.


- 12\. Yim P.J., Nosher J.L.: Subtraction computed tomographic angiography: use of pre-contrast images for calcification removal. Proceedings SPIE 2006; 6143: pp. 805-811.


- 13\. van Straten M., Venema H.W., Streekstra G.J., Reekers J.A., den Heeten G.J., Grimbergen C.A.: Removal of arterial wall calcifications in CT angiography by local subtraction. Med Phys 2003; 30: pp. 761-770.