---
title: Improved Estimation of Coronary Plaque and Luminal Attenuation Using a Vendor-specific Model-based Iterative Reconstruction Algorithm in Contrast-enhanced CT Coronary Angiography
author: [CL_AT_YoshinoriFunamaPhD,CL_AT_DaisukeUtsunomiyaMD,CL_AT_KenichiroHirataMD,CL_AT_KatsuyukiTaguchiPhD,CL_AT_TakeshiNakauraMD,CL_AT_SeitaroOdaMD,CL_AT_MasafumiKidohMD,CL_AT_HideakiYukiMD,CL_AT_YasuyukiYamashitaMD]
date: 2017-09-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 24, Issue 9]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

To investigate the stabilities of plaque attenuation and coronary lumen for different plaque types, stenotic degrees, lumen densities, and reconstruction methods using coronary vessel phantoms and the visualization of coronary plaques in clinical patients through coronary computed tomography (CT) angiography.

## Materials and Methods

We performed 320-detector volume scanning of vessel tubes with stenosis and a tube without stenosis using three types of plaque CT numbers. The stenotic degrees were 50% and 75%. Images were reconstructed with filtered back projection (FBP) and two types of iterative reconstructions (AIDR3D and FIRST \[forward-projected model-based iterative reconstruction solution\]), with stenotic CT number of approximately 40, 80, and 150 HU (Hounsfield unit), respectively. In each case, the tubing of the coronary vessel was filled with diluted contrast material and distilled water to reach the target lumen CT numbers of approximately 350 HU and 450 HU, and 0 HU, respectively. Peak lumen and plaque CT numbers were measured to calculate the lumen–plaque contrast. In addition, we retrospectively evaluated the image quality with regard to coronary arterial lumen and the plaque in 10 clinical patients on a 4-point scale.

## Results

At 50% stenosis, the plaque CT number with contrast enhancement increased for FBP and AIDR3D, and the difference in the plaque CT number with and without contrast enhancement was 15–44 HU for FBP and 10–31 HU for AIDR3D. However, the plaque CT number for FIRST had a smaller variation and the difference with and without contrast enhancement was −12 to 8 HU. The visual evaluation score for the vessel lumen was 2.8 ± 0.6, 3.5 ± 0.5, and 3.7 ± 0.5 for FBP, AIDR3D, and FIRST, respectively.

## Conclusions

The FIRST method controls the increase in plaque density and the lumen–plaque contrast. Consequently, it improves the visualization of coronary plaques in coronary CT angiography.

## Introduction

Coronary computed tomography angiography (CTA) with electrocardiogram (ECG) gating is an accurate noninvasive method to evaluate coronary artery disease . Potential applications of coronary CTA require high visualization of coronary arteries while maintaining radiation dose . In addition, coronary CTA raises concerns regarding evaluations of coronary stenosis and coronary plaque. Previous studies have associated high-risk plaque characteristics (e.g., positive remodeling, low CT number plaque, napkin ring, sign, and spotty calcium), as characterized by coronary CTA, with culprit lesions of the acute coronary syndrome . Therefore, diagnostic accuracy relies on knowledge of the plaque burden and high-risk plaque features. Regarding coronary plaque, CT number of coronary plaque varies with the increasing contrast enhancement of coronary lumen owing to partial volume effects, beam hardening, and plaque vascularity . Noncontrast CTA and dual-phase coronary CTA from noncontrast (first phase) and contrast enhancement (second phase) were previously applied to achieve accurate CT number of the coronary plaque .

Recently, an algorithm called “forward-projected model-based iterative reconstruction solution” (FIRST) was developed as an iterative method for image reconstructions . Unlike AIDR3D , FIRST is an iterative reconstruction algorithm that models system optics, such as the detector element aperture, and improves image quality by iteratively minimizing a penalty-based cost function. FIRST can potentially improve the spatial resolution and CT number because it employs a more accurate model of X-ray physics (considering partial volume effects, beam hardening, etc.) than the former iterative method does, as well as an improved filtered back projection (FBP) method.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Phantom Study

## Phantom

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ECG-gated Single-heartbeat CTA

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Peak CT Number and Plaque CT Number

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

d-lumenCTnum\[HU\]=p-lumenCTnumw​/​ostenosis−p-lumenCTnumw​/stenosis
d

 -

lumen

C

T

n

u

m

\[

H

U

\]

=

p

 -

lumen

C

T

n

u

m

w

​

/

​

o

stenosis

−

p

 -

lumen

C

T

n

u

m

w

​

/

stenosis


d-plaqueCTnum\[HU\]=plaqueCTnumw​/​ostenosis−plaqueCTnumw​/stenosis.
d

 -

plaque

C

T

n

u

m

\[

H

U

\]

=

plaque

C

T

n

u

m

w

​

/

​

o

stenosis

−

plaque

C

T

n

u

m

w

​

/

stenosis

.


![Figure 1, Multiplanar reformation images with plaque on noncontrast enhancement (a) and contrast enhancement (b) ; CT voxel attenuation profile across the 50% and 75% plaques.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovedEstimationofCoronaryPlaqueandLuminalAttenuationUsingaVendorspecificModelbasedIterativeReconstructionAlgorithminContrastenhancedCTCoronaryAngiography/0_1s20S1076633217301150.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Study

## Patients

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantitative Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

CNRvessel=(CTnumberoflumen−CTnumberofperivascularfat)/imagenoise
C

N

R

vessel

=

(

C

T

number

o

f

lumen

−

C

T

number

o

f

perivascular

f

a

t

)

/

image

noise


CNRplaque=(CTnumberofplaque−CTnumberofperivascularfat)/imagenoise
C

N

R

plaque

=

(

C

T

number

o

f

plaque

−

C

T

number

o

f

perivascular

f

a

t

)

/

image

noise


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Qualitative Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Phantom Study

## Lumen CT Number

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 1


Lumen CT Number with and without Stenosis for FBP, AIDR3D, and FIRST


Lumen CT Number without Stenosis (HU) Stenosis Plaque Type S-plaque (HU) I-plaque (HU) C-plaque (HU) FBP 370.5 331.8 325 338.8 451.7 386.1 401.3 383.7 AIDR3D 370.4 50% 328.2 362.5 335.2 453.6 377.2 384.5 377.2 FIRST 387.9 371.9 378.4 386.6 464.7 444.7 441 449.6 FBP 370.5 214.5 229.8 230 451.7 255.4 276.3 282.3 AIDR3D 370.4 75% 210 218.9 219.2 453.6 253.2 273.2 280.9 FIRST 387.9 266.6 270.6 273.4 464.7 314 322.1 343.3

CT, computed tomography; FBP, filtered back projection; FIRST, forward-projected model-based iterative reconstruction solution; HU, Hounsfield unit. C-plaque, calcified plaque; I-plaque, intermediate plaque; S-plaque, soft plaque.


![Figure 2, Difference in peak CT numbers with and without stenosis for FBP, AIDR3D, and FIRST at different plaque types and lumen densities, calculated from peak lumen CT number without stenosis–peak lumen CT number with stenosis [HU]. ( a ) and ( b ) represent the cases with 50% and 75% stenoses, respectively. CT, computed tomography; FBP, filtered back projection; FIRST, forward-projected model-based iterative reconstruction solution; HU, Hounsfield unit. C-plaque, calcified plaque; I-plaque, intermediate plaque; S-plaque, soft plaque.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovedEstimationofCoronaryPlaqueandLuminalAttenuationUsingaVendorspecificModelbasedIterativeReconstructionAlgorithminContrastenhancedCTCoronaryAngiography/1_1s20S1076633217301150.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Plaque CT Number

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 2


Plaque CT Number with and without Contrast Enhancement at 50% and 75% Stenoses for FBP, AIDR3D, and FIRST


Stenosis Plaque Type Plaque CT Number without Contrast Enhancement (HU) Plaque CT Number with Contrast Enhancement (HU) Low Lumen Density High Lumen Density 50% FBP S-plaque 48.2 80.2 92.4 I-plaque 87.4 104.5 106.8 C-plaque 152.2 173 167.6 AIDR3D S-plaque 49.5 80 66 I-plaque 89.4 103.7 99.6 C-plaque 151.2 171.6 171.6 FIRST S-plaque 50.1 50.2 40.2 I-plaque 87.8 86.5 75.9 C-plaque 148.5 153 156.1 75% FBP S-plaque 50.1 47.7 57.7 I-plaque 90.2 92.3 103 C-plaque 158.2 169.6 167.6 AIDR3D S-plaque 50.6 45.4 61.3 I-plaque 91.6 96.3 102.1 C-plaque 149.7 167.3 148.9 FIRST S-plaque 49.8 34.5 41.9 I-plaque 86.8 82.2 84.3 C-plaque 150.3 148.5 154.2

CT, computed tomography; FBP, filtered back projection; FIRST, forward-projected model-based iterative reconstruction solution; HU, Hounsfield unit. C-plaque, calcified plaque; I-plaque, intermediate plaque; S-plaque, soft plaque.


![Figure 3, Difference in plaque CT numbers with and without contrast enhancement for FBP, AIDR3D, and FIRST at different plaque types and lumen densities, calculated from plaque CT number without stenosis–plaque CT number with stenosis [HU]. ( a ) and ( b ) represent the cases with 50% and 75% stenoses, respectively. CT, computed tomography; FBP, filtered back projection; FIRST, forward-projected model-based iterative reconstruction solution; HU, Hounsfield unit. C-plaque, calcified plaque; I-plaque, intermediate plaque; S-plaque, soft plaque.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovedEstimationofCoronaryPlaqueandLuminalAttenuationUsingaVendorspecificModelbasedIterativeReconstructionAlgorithminContrastenhancedCTCoronaryAngiography/2_1s20S1076633217301150.jpg)

![Figure 4, Profile curve for high lumen density including 75% stenosis of soft plaque with MPR images obtained at FBP, AIDR3D, and FIRST. The FIRST image gives a narrower profile curve than the other images. CT, computed tomography; FBP, filtered back projection; FIRST, forward-projected model-based iterative reconstruction solution; HU, Hounsfield unit; MPR, multiplanar reformation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovedEstimationofCoronaryPlaqueandLuminalAttenuationUsingaVendorspecificModelbasedIterativeReconstructionAlgorithminContrastenhancedCTCoronaryAngiography/3_1s20S1076633217301150.jpg)

TABLE 3


Ratio of Lumen-plaque Contrast in Each Method to That of FBP


Stenosis Plaque Type Low Lumen Density High Lumen Density FBP AIDR3D FIRST FBP AIDR3D FIRST 50% S-plaque 1.0 1.0 1.3 1.0 1.1 1.4 I-plaque 1.0 1.2 1.3 1.0 1.0 1.2 C-plaque 1.0 1.0 1.4 1.0 1.0 1.4 75% S-plaque 1.0 1.0 1.4 1.0 1.0 1.4 I-plaque 1.0 0.9 1.4 1.0 1.0 1.4 C-plaque 1.0 0.9 1.6 1.0 1.2 1.6

FBP, filtered back projection; FIRST, forward-projected model-based iterative reconstruction solution. C-plaque, calcified plaque; I-plaque, intermediate plaque; S-plaque, soft plaque.


Lumen-plaque contrast is calculated from subtraction of plaque CT (computed tomography) number from peak lumen CT number.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Study

## Quantitative Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Qualitative Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, A 66-year-old man with chest pain. Noncalcified plaque is shown in the proximal right coronary artery (arrow). Clear margins of vessel lumen and plaque with less image noise are demonstrated on the FIRST image. FBP, filtered back projection; FIRST, forward-projected model-based iterative reconstruction solution.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImprovedEstimationofCoronaryPlaqueandLuminalAttenuationUsingaVendorspecificModelbasedIterativeReconstructionAlgorithminContrastenhancedCTCoronaryAngiography/4_1s20S1076633217301150.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

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

- 1\. Oncel D., Oncel G., Tastan A., et. al.: Evaluation of coronary stent patency and in-stent restenosis with dual-source CT coronary angiography without heart rate control. AJR Am J Roentgenol 2008; 191: pp. 56-63.


- 2\. Mollet N.R., Cademartiri F., van Mieghem C.A., et. al.: High-resolution spiral computed tomography coronary angiography in patients referred for diagnostic conventional coronary angiography. Circulation 2005; 112: pp. 2318-2323.


- 3\. Leschka S., Alkadhi H., Plass A., et. al.: Accuracy of MSCT coronary angiography with 64-slice technology: first experience. Eur Heart J 2005; 26: pp. 1482-1487.


- 4\. Miller J.M., Rochitte C.E., Dewey M., et. al.: Diagnostic performance of coronary angiography by 64-row CT. N Engl J Med 2008; 359: pp. 2324-2336.


- 5\. Chen M.Y., Shanbhag S.M., Arai A.E.: Submillisievert median radiation dose for coronary angiography with a second-generation 320-detector row CT scanner in 107 consecutive patients. Radiology 2013; 267: pp. 76-85.


- 6\. Cury R.C., Abbara S., Achenbach S., et. al.: CAD-RADS(TM) Coronary Artery Disease—Reporting and Data System. An expert consensus document of the Society of Cardiovascular Computed Tomography (SCCT), the American College of Radiology (ACR) and the North American Society for Cardiovascular Imaging (NASCI). Endorsed by the American College of Cardiology. J Cardiovasc Comput Tomogr 2016; 10: pp. 269-281.


- 7\. Utsunomiya D., Fukunaga T., Oda S., et. al.: Multidetector computed tomography evaluation of coronary plaque morphology in patients with stable angina. Heart Vessels 2011; 26: pp. 392-398.


- 8\. Ferencik M., Mayrhofer T., Puchner S.B., et. al.: Computed tomography-based high-risk coronary plaque score to predict acute coronary syndrome among patients with acute chest pain—results from the ROMICAT II trial. J Cardiovasc Comput Tomogr 2015; 9: pp. 538-545.


- 9\. Fuchs T.A., Fiechter M., Gebhard C., et. al.: CT coronary angiography: impact of adapted statistical iterative reconstruction (ASIR) on coronary stenosis and plaque composition analysis. Int J Cardiovasc Imaging 2013; 29: pp. 719-724.


- 10\. Precht H., Kitslaar P.H., Broersen A., et. al.: Influence of Adaptive Statistical Iterative Reconstruction on coronary plaque analysis in coronary computed tomography angiography. J Cardiovasc Comput Tomogr 2016; 10: pp. 507-516.


- 11\. Puchner S.B., Ferencik M., Karolyi M., et. al.: The effect of iterative image reconstruction algorithms on the feasibility of automated plaque assessment in coronary CT angiography. Int J Cardiovasc Imaging 2013; 29: pp. 1879-1888.


- 12\. Puchner S.B., Ferencik M., Maurovich-Horvat P., et. al.: Iterative image reconstruction algorithms in coronary CT angiography improve the detection of lipid-core plaque—a comparison with histology. Eur Radiol 2015; 25: pp. 15-23.


- 13\. Dalager M.G., Bottcher M., Andersen G., et. al.: Impact of luminal density on plaque classification by CT coronary angiography. Int J Cardiovasc Imaging 2011; 27: pp. 593-600.


- 14\. Yoshioka K., Tanaka R., Muranaka K., et. al.: Subtraction coronary CT angiography using second-generation 320-detector row CT. Int J Cardiovasc Imaging 2015; 31: pp. 51-58.


- 15\. Kidoh M., Utsunomiya D., Oda S., et. al.: Evaluation of the effect of intracoronary attenuation on coronary plaque measurements using a dual-phase coronary CT angiography technique on a 320-row CT scanner—in vivo validation study. Acad Radiol 2016; 23: pp. 315-320.


- 16\. Kidoh M., Utsunomiya D., Oda S., et. al.: Optimized subtraction coronary CT angiography protocol for clinical use with short breath-holding time-initial experience. Acad Radiol 2015; 22: pp. 117-120.


- 17\. Nishiyama Y., Tada K., Nishiyama Y., et. al.: Effect of the forward-projected model-based iterative reconstruction solution algorithm on image quality and radiation dose in pediatric cardiac computed tomography. Pediatr Radiol 2016; 46: pp. 1663-1670.


- 18\. Yasaka K., Kamiya K., Irie R., et. al.: Metal artefact reduction for patients with metallic dental fillings in helical neck computed tomography: comparison of adaptive iterative dose reduction 3D (AIDR 3D), forward-projected model-based iterative reconstruction solution (FIRST) and AIDR 3D with single-energy metal artefact reduction (SEMAR). Dentomaxillofac Radiol 2016; 45: pp. 20160114.


- 19\. Gervaise A., Osemont B., Lecocq S., et. al.: CT image quality improvement using Adaptive Iterative Dose Reduction with wide-volume acquisition on 320-detector CT. Eur Radiol 2012; 22: pp. 295-301.


- 20\. Chen M.Y., Steigner M.L., Leung S.W., et. al.: Simulated 50% radiation dose reduction in coronary CT angiography using adaptive iterative dose reduction in three-dimensions (AIDR3D). Int J Cardiovasc Imaging 2013; 29: pp. 1167-1175.


- 21\. Einstein A.J., Elliston C.D., Arai A.E., et. al.: Radiation dose from single-heartbeat coronary CT angiography performed with a 320-detector row volume scanner. Radiology 2010; 254: pp. 698-706.


- 22\. Nikolic B., Khosa F., Lin P.J., et. al.: Absorbed radiation dose in radiosensitive organs during coronary CT angiography using 320-MDCT: effect of maximum tube voltage and heart rate variations. AJR Am J Roentgenol 2010; 195: pp. 1347-1354.


- 23\. Qin J., Liu L.Y., Fang Y., et. al.: 320-detector CT coronary angiography with prospective and retrospective electrocardiogram gating in a single heartbeat: comparison of image quality and radiation dose. Br J Radiol 2012; 85: pp. 945-951.


- 24\. Kitagawa K., George R.T., Arbab-Zadeh A., et. al.: Characterization and correction of beam-hardening artifacts during dynamic volume CT assessment of myocardial perfusion. Radiology 2010; 256: pp. 111-118.


- 25\. Leipsic J., Abbara S., Achenbach S., et. al.: SCCT guidelines for the interpretation and reporting of coronary CT angiography: a report of the Society of Cardiovascular Computed Tomography Guidelines Committee. J Cardiovasc Comput Tomogr 2014; 8: pp. 342-358.


- 26\. Husarik D.B., Marin D., Samei E., et. al.: Radiation dose reduction in abdominal computed tomography during the late hepatic arterial phase using a model-based iterative reconstruction algorithm: how low can we go?. Invest Radiol 2012; 47: pp. 468-474.


- 27\. Scheffel H., Stolzmann P., Schlett C.L., et. al.: Coronary artery plaques: cardiac CT with model-based and adaptive-statistical iterative reconstruction technique. Eur J Radiol 2012; 81: pp. e363-e369.


- 28\. Funama Y., Taguchi K., Utsunomiya D., et. al.: Image quality assessment of an iterative reconstruction algorithm applied to abdominal CT imaging. Phys Med 2014; 30: pp. 527-534.


- 29\. Leipsic J., Labounty T.M., Heilbron B., et. al.: Adaptive statistical iterative reconstruction: assessment of image noise and image quality in coronary CT angiography. AJR Am J Roentgenol 2010; 195: pp. 649-654.


- 30\. Cademartiri F., Mollet N.R., Runza G., et. al.: Influence of intracoronary attenuation on coronary plaque measurements using multislice computed tomography: observations in an ex vivo model of coronary computed tomography angiography. Eur Radiol 2005; 15: pp. 1426-1431.


- 31\. Hoffmann U., Bamberg F., Chae C.U., et. al.: Coronary computed tomography angiography for early triage of patients with acute chest pain: the ROMICAT (Rule Out Myocardial Infarction using Computer Assisted Tomography) trial. J Am Coll Cardiol 2009; 53: pp. 1642-1650.


- 32\. Yamamoto H., Kitagawa T., Ohashi N., et. al.: Noncalcified atherosclerotic lesions with vulnerable characteristics detected by coronary CT angiography and future coronary events. J Cardiovasc Comput Tomogr 2013; 7: pp. 192-199.