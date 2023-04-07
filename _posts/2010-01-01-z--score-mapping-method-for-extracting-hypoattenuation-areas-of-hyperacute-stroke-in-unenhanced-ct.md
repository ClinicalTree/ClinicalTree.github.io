---
title: Z -score Mapping Method for Extracting Hypoattenuation Areas of Hyperacute Stroke in Unenhanced CT
author: [CL_AT_NoriyukiTakahashiMS,CL_AT_DuYihTsaiPhD,CL_AT_YongbumLeePhD,CL_AT_ToshibumiKinoshitaMDPhD,CL_AT_KiyoshiIshiiMD]
date: 2010-01-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 17, Issue 1]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The purpose of this study was to develop a _z_ -score mapping method on the basis of a voxel-by-voxel analysis to visualize hypoattenuation areas of hyperacute stroke on unenhanced computed tomographic (CT) images.

## Materials and Methods

The algorithm of the developed method consisted of five main steps: anatomic standardization, the construction of a normal reference database, calculation of the _z_ scores, the elimination of false-positive areas, and the extraction of hypoattenuation areas. The obtained _z_ -score map was then superimposed on the original CT images for identifying hypoattenuation areas of hyperacute stroke on the unenhanced CT images. The method was applied to 21 patients with infarctions of the middle cerebral artery territory <3 hours after symptom onset. The performance of the method was evaluated using receiver-operating characteristic analysis.

## Results

Hypoattenuation regions could be significantly distinguished from normal regions by _z_ -score values ( _P_ < .0001). The area under the receiver-operating characteristic curve for distinction between 68 hypoattenuation regions and 142 normal regions was 0.834.

## Conclusions

The developed method has the potential to accurately indicate high–signal intensity areas corresponding to hypoattenuation areas on CT images in the hyperacute stage of stroke.

Currently, unenhanced computed tomographic (CT) imaging still serves as an initial neuroimaging examination in the diagnosis of acute ischemic stroke because of its accessibility and speed, although diffusion-weighted magnetic resonance (MR) imaging in acute ischemic stroke has been supported . Identifying hypoattenuation of ischemic brain parenchyma is important in the interpretation of acute stroke on CT images. Hypoattenuation is a subtle attenuation change (in Hounsfield units \[HU\]) of ischemic brain tissue. In recent years, tissue plasminogen activator thrombolysis has been approved by the US Food and Drug Administration as an effective treatment for acute stroke <3 hours after symptom onset. Patients with large areas of ischemic lesions would incur a high risk for fatal hemorrhagic complications after thrombolysis. To avoid the risk, unenhanced CT imaging plays an important role in rapidly selecting patients. Thus, quantifying the extent of areas of ischemic lesions is mandatory to select patients for thrombolysis with low risk for hemorrhage. A quantitative CT scoring system, the Alberta Stroke Program Early CT Score (ASPECTS) , is often used to help interpreters in quantifying the extent of ischemic lesions of acute stroke in the territory of the middle cerebral artery (MCA). When evaluating the extent of ischemic areas using the ASPECTS method, the extent of the regions of ischemic lesions (hypoattenuation or brain swelling) is quantified by counting the number of lesions among 10 predefined regions. However, the sensitivity for the detection of acute stroke was <50% on unenhanced CT images , even when the ASPECTS system was used.

The presence of hypoattenuation is an important CT finding of acute ischemic stroke. The detectability of hypoattenuation within a few hours of symptom onset largely depends on the skill and experiences of the reader, because of difficulty in the detection of subtle attenuation changes of ischemic brain tissue . Therefore, improvement in the detection of parenchymal hypoattenuation on unenhanced CT images would be desirable. To cope with this issue, we have developed an adaptive smoothing filter to reduce image noise . The results showed that the proposed filter had potential usefulness in the improvement of detection . However, the method was effective for detecting only the presence of hypoattenuation. The extent of hypoattenuation was difficult to identify with this method. Maldjian et al reported an automated segmentation method for identifying hypoattenuation of acute ischemia. In their report, histograms of voxel density distributions in the lentiform nucleus and insula were in comparison to those of the contralateral side on the brain image. The method, however, was limited to analyzing only two of the 10 regions in ASPECTS (ie, the lentiform nucleus and insula).

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Flowchart illustrating the process of generating a z -score map for the extraction of hypoattenuation regions on unenhanced computed tomographic (CT) images. MCA, middle cerebral artery.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/0_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Patient Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Ten Alberta Stroke Program Early CT Score (ASPECTS)–defined regions in the middle cerebral artery territory for the performance evaluation on unenhanced computed tomographic images. These regions include the lentiform nucleus (L), insula (I), caudate nucleus (C), internal capsule (IC), anterior inferior frontal lobe (M1), temporal lobe (M2), inferior parietal and posterior temporal lobe (M3), anterior superior frontal lobe (M4), precentral and superior frontal lobe (M5), and superior parietal lobe (M6).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/1_1s20S1076633209004097.jpg)

![Figure 3, Histogram of hypoattenuation regions identified by two neuroradiologists from 21 patients. The selected locations were based on the Alberta Stroke Program Early CT Score method. C, caudate nucleus; I, insula; IC, internal capsule; L, lentiform nucleus; M1, anterior inferior frontal lobe; M2, temporal lobe; M3, inferior parietal and posterior temporal lobe; M4, anterior superior frontal lobe; M5, precentral and superior frontal lobe; M6, superior parietal lobe.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/2_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Normalization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Normal Reference Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Examples showing images obtained with the normalized computed tomographic database composed of 28 normal subjects. (a) Sample images of the mean data set. Voxel value is indicated by a grayscale bar (right) . (b) Sample images of the standard deviation data set. Standard deviation value is indicated by a grayscale bar (right) . HU, Hounsfield units.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/3_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Calculation of _z_ Score

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

zscore(x,y,z)=\[Cmean(x,y,z)− input(x,y,z)\]/NSD(x,y,z),
z

score

(

x

,

y

,

z

)

=

\[

C

mean

(

x

,

y

,

z

)

− input

(

x

,

y

,

z

)

\]

/

N

SD

(

x

,

y

,

z

)

,


where _C_ mean( _x_ , _y_ , _z_ ) and _N_ SD( _x_ , _y_ , _z_ ) represent the mean and SD, respectively of the normal reference data at the coordinate of ( _x_ , _y_ , _z_ ). Input  ( _x_ , _y_ , _z_ ) is the value of spatially normalized patient data set at the same coordinate system. It is desirable that the _z_ score in the area of normal brain parenchyma be nearly equal to zero. However, attenuation coefficients of the brain parenchyma on unenhanced CT images usually fluctuate because of variation in skull vault thickness. In this study, an offset was used to remove this variation during the calculation of _z_ scores. The offset was the difference between an input CT value and the reference CT value. The determination of the offset was follows. First, two volumes of interest (VOIs) were determined from the mean data set. The two VOIs (size, 107 voxels), the right and left VOIs, were set at the right lentiform nucleus and the left lentiform nucleus, respectively. Second, the following measurements were made: the average value of the mean data set for the right VOI ( _A_ R ) and that for the left VOI ( _A_ L ) and the average value of the each input CT data set for the right VOI ( _I_ R ) and that for the left VOI ( _I_ L ). When measuring _I_ R and _I_ L , the VOIs were automatically set to each case of the input data. The offset value, _V_ off , was defined as


Voff={AR−IRAL−ILwhenIR≥ILwhenIR<IL.
V

of

f

=

{

A

R

−

I

R

A

L

−

I

L

when

I

R

≥

I

L

when

I

R

<

I

L

.


It is evident in equation  2 that the higher value of _I_ R and _I_ L was adopted for offsetting the input CT data set. The reason was that the VOI with the lower value relative to the contralateral VOI might include parenchymal hypoattenuation of acute stroke. After performing offsetting, the _z_ score of each voxel of the input CT data was calculated using equation  1 .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Elimination of Cerebrospinal Fluid (CSF) Area

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, (a) Binary-mask image used in the elimination of cerebrospinal fluid areas. (b) A z -score image before elimination. (c) A z -score image after the elimination of cerebrospinal fluid areas.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/4_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Determination of the MCA Territory

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Display of _z_ -score Maps

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Performance Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Imaging findings in patient 1. (a) Z -score maps corresponding to the unenhanced images of (b) ; z scores are indicated by a color bar (right) . (b) Unenhanced computed tomographic (CT) images. (c) Follow-up CT images. High– z score areas shown in colors in (a) correspond to three hypoattenuation regions (caudate nucleus, lentiform nucleus, and inferior parietal and posterior temporal lobe white arrows in b ). Ischemic lesions ( black arrows in c ) corresponding to the high– z score areas are identified.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/5_1s20S1076633209004097.jpg)

![Figure 7, Imaging findings in patient 2. (a) Z -score maps corresponding to the unenhanced images shown in (b) ; z scores are indicated by a color bar (right) . (b) Unenhanced computed tomographic (CT) images. (c) Follow-up CT images. High– z score areas shown in colors in (a) correspond to two hypoattenuation regions (lentiform nucleus and precentral and superior frontal lobe; white arrows in b ). Ischemic lesions ( black arrows in c ) corresponding to the high– z score areas are identified.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/6_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Distribution of the absolute difference of z score (ADZ) values for the regions of hypoattenuation and normality.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/7_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Receiver-operating characteristic curve for distinction between hypoattenuation regions and normal regions.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/8_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Comparison of median absolute difference of z score (ADZ) values between hypoattenuation regions and normal regions at each location. Hatched bars and shaded bars represent the values for regions without and with hypoattenuation, respectively. C, caudate nucleus; I, insula; IC, internal capsule; L, lentiform nucleus; M1, anterior inferior frontal lobe; M2, temporal lobe; M3, inferior parietal and posterior temporal lobe; M4, anterior superior frontal lobe; M5, precentral and superior frontal lobe; M6, superior parietal lobe.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ZscoreMappingMethodforExtractingHypoattenuationAreasofHyperacuteStrokeinUnenhancedCT/9_1s20S1076633209004097.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Adams H., Adams R., del Zoppo G.: Guidelines for the early management of patients with ischemic stroke: 2005 guidelines update a scientific statement from the Stroke Council of the American Heart Association/American Stroke Association. Stroke 2005; 36: pp. 916-923.


- 2\. Adams J.H.P., Adams R.J., Brott T., et. al.: Guidelines for the early management of patients with ischemic stroke: a scientific statement from the Stroke Council of the American Stroke Association. Stroke 2003; 34: pp. 1056-1083.


- 3\. Balbel P.A., Demchuk A.M., Zhang J., et. al.: Validity and reliability of a quantitative computed tomography score in predicting outcome of hyperacute stroke before thrombolytic therapy. Lancet 2000; 355: pp. 1670-1674.


- 4\. Camargo E.C.S., Furie K.L., Singhal A.B., et. al.: Acute brain infarct: detection and delineation with CT angiographic source images versus nonenhanced CT scans. Radiology 2007; 244: pp. 541-548.


- 5\. Schriger D.L., Karafut M., Starkman S., et. al.: Cranial computed tomography interpretation in acute stroke: physician accuracy in determining eligibility for thrombolytic therapy. JAMA 1998; 279: pp. 1293-1297.


- 6\. Wardlaw J.M., Mielke O.: Early signs of brain infarction at CT: observer reliability and outcome after thrombolytic treatment—systematic review. Radiology 2005; 235: pp. 444-453.


- 7\. Takahashi N., Lee Y., Tsai D.Y., et. al.: A novel noise reduction filter for improving visibility of early CT signs of hyperacute stroke: evaluation of the filter's performance—preliminary clinical experience. Radiat Med 2007; 25: pp. 247-254.


- 8\. Lee Y., Takahashi N., Tsai D.Y., et. al.: Adaptive partial median filter for early CT signs of acute cerebral infarction. Int J Comp Assisted Radiol Surg 2007; 2: pp. 105-115.


- 9\. Takahashi N., Lee Y., Tsai D.Y., et. al.: Improvement of detection of hypoattenuation in acute ischemic stroke in unenhanced CT using an adaptive smoothing Filter. Acta Radiologica 2008; 49: pp. 816-826.


- 10\. Maldjian J.A., Chalela J., Kasner S.E., et. al.: Automated CT segmentation and analysis for acute middle cerebral artery stroke. AJNR Am J Neuroradiol 2001; 22: pp. 1050-1055.


- 11\. Minoshima S., Frey K.A.A., Koeppe R.A., et. al.: A diagnostic approach in Alzheimer's disease using three-dimensional stereotactic surface projections of fluorine-18-FDG PET. J Nucl Med 1995; 36: pp. 1238-1248.


- 12\. Matsuda H., Mizunuma S., Nagao T., et. al.: Automated discrimination between very early Alzheimer disease and controls using an easy Z-score imaging system for multicenter brain perfusion single-photon emission tomography. AJNR Am J Neuroradiol 2007; 28: pp. 731-736.


- 13\. Friston K.J., Ashburner J., Frith C.D., et. al.: Spatial registration and normalization of images. Hum Brain Mapp 1995; 3: pp. 165-189.


- 14\. Ashburner J., Friston K.J.: Nonlinear spatial normalization using basis functions. Hum Brain Mapp 1999; 7: pp. 254-266.