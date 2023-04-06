---
title: Automatic and Rapid Identification of Infarct Slices and Hemisphere in DWI Scans
author: [Varsha Gupta PhD,Bhanu Prakash KN PhD,Wieslaw L. Nowinski PhD DSc]
date: 2008-01-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 15, Issue 1 SOURCE CL_S_AcademicRadiologyVolume15Issue1 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Accurate, free of observer’s bias, and fast identification of acute infarct is critical in visual and automatic processing of stroke images. An automatic and rapid algorithm has been developed to identify the infarct slices and the hemisphere in diffusion-weighted imaging (DWI) scans.

## Materials and Methods

Thirty-six DWI scans were acquired from five centers with the slice thickness of 4–14 mm. We also derive images from the original scans to assess the accuracy of the algorithm by using a wide range of infarct size and number of artifacts per unit area. Based on the difference in percentile characteristics of intensity normalized (infarct/noninfarct) images, two parameters are defined: R _s_ for infarct slice identification and R _h_ for infarct hemisphere identification. Using the identified infarct slices the infarct hemisphere is subsequently determined.

## Results

The average sensitivity and specificity for slice and hemisphere identification were 98.1%, 51.4% and 91.7%, 91.7%, respectively. The processing time is ∼3–5 seconds on Matlab platform and on VC++ it is predicted ∼10 milliseconds. Based on simulation study, we can infer that the algorithm produces accurate results in most of the situations although the sensitivity goes down by ∼15% when the infarct size is small (<2–3% of image area) and the artifacts per unit area are large.

## Conclusions

The proposed algorithm applied as a preprocessor can be useful to: 1) estimate location (hemisphere) and extent of infarct (number and location of slices), 2) reduce time and labor of infarct volume study, 3) cross-check visual interpretation, 4) form a part of an infarct segmentation module, and 5) improve localization of the midsagittal plane.

Diffusion-weighted Imaging (DWI) is used to evaluate infarct in acute ischemic stroke patients. Automatic and rapid identification of infarcts in DWI images is important both in visual scan reading and automatic image processing as it reduces time and increases confidence. More importantly, as a recent study ( ) shows, infarct location is fundamentally linked to neurologic deficits. Several automatic or semiautomatic segmentation techniques are proposed to reduce the total time of infarct segmentation compared with manual processing of data, which may have errors and observer’s bias. A semiautomatic method ( ) was developed to determine infarct volume by diffusion tensor magnetic resonance imaging. Another study ( ) proposed an unsupervised segmentation method using multiscale statistical classification and partial volume voxel reclassification in the case of diffusion tensor magnetic resonance images. A method based on the probabilistic neural network for selecting infarct slices and an adaptive (two-level) Gaussian mixture model for infarct segmentation was suggested by Bhanu Prakash et al ( ).

In this article, an automatic framework to detect the infarct slices and hemisphere is presented. We propose a conceptually simple and fast approach that utilizes the difference in image intensity distribution for infarct (hyperintense) and normal tissue (isointense). The difference in intensity percentile characteristics in isointense and hyperintense regions is used to define two parameters: 1) slice parameter R  s to quantify the difference in infarct/noninfarct slices and 2) hemisphere parameter R  h to identify the infarct hemisphere. The proposed method is applied to 36 DWI scans obtained from five different sources. The accuracy is assessed using images derived from combinations of infarcts of different sizes and normal tissue region containing different artifact densities (number of artifacts per unit area). The algorithm can be useful to: 1) estimate location (hemisphere) and extent of infarct (number and location of slices), 2) reduce time and labor of infarct volume study, 3) cross-check visual interpretation, 4) form a part of an infarct segmentation module ( ), and 5) improve localization of the midsagittal plane ( ). It can be applied as a preprocessor in a stroke computer-assisted diagnosis system ( ).

## Materials and methods

## Data Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Description

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Algorithm

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Stage 1: Identification of infarct slices

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Flowchart diagram to explain summary of slice identification procedure.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/0_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Concept of the algorithm

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, An example of (a) diffusion-weighted image and (b) its histogram.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/1_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, (a) Synthetic image with a distribution of isointense pixels and its histogram, A/B = 1.2 and (b) synthetic image with a few isointense pixels replaced by hyperintense pixels and its histogram A/B = 0.8.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/2_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Normalization of image

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Inorm=f\*I−IminImax−Imin
I

n

o

r

m

=

f

\*

I

−

I

min

⁡

I

max

⁡

−

I

min

⁡


where _I_ max and _I_ min are the maximum and minimum intensity on a given slice and f is the normalization parameter. In our study, we selected f = 1 so that the maximum intensity is 1 and the minimum intensity is 0. The histograms of all the images have been plotted with 256 bins.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reference point and slice parameter R _s_

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, (a) Percentiles of intensity of a real noninfarct slice and (b) percentiles of intensity of a real infarct slice.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/3_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Rs=(1P50)(Pa+20−PaPb+20−Pb)
R

s

=

(

1

P

50

)

(

P

a

+

20

−

P

a

P

b

+

20

−

P

b

)


where P _a_ are percentiles in a slice above P  50 and P _b_ are percentiles below P  50 .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## R  s  for different bands

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

NormalizedRs=(Rs−min\[Rs\])/(max\[Rs\]−min\[Rs\])
Normalized

R

s

=

(

R

s

−

min

\[

R

s

\]

)

/

(

max

\[

R

s

\]

−

min

\[

R

s

\]

)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Occurrence of peaks and flat region

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Plot of normalized R s for a volume in different B1-B4 bands the flat region corresponding to the predicted infarct is limited by the peak regions.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/4_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Final width of flat region=\[max (width of flat region in B1−B4)\]
Final width of flat region

=

\[

max (width of flat region in B1

−

B4

)

\]


In the example discussed (  Fig 5 ), the extrema of flat region for B1 is at 12 and 28, for B2 at 12 and 28, for B3 at 12 and 28 and for B4 at 11 and 28. The maximum width corresponds to B4 (28 − 11 = 17), so we take the final extrema of flat region as 11 to 28.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Hypothesis of flat region and infarct slices

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Stage 2: Localization of Infarct Hemisphere

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Flowchart of a summary of hemisphere identification procedure.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/5_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, (a) Midsagittal plane dividing the image into left and right hemisphere, (b) plot of histogram and percentiles for an infarct hemisphere, and (c) plot of histogram and percentiles for noninfarct hemisphere. Note the density of percentiles is different to that observed in slice identification. This is because of different intensity range for both the hemispheres. The infarct hemisphere intensity distribution has both iso- and hyperintense, whereas normal hemisphere has only isointense pixel intensities.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/6_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Selection of reference point (r  i  )

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Percentile characteristics and hemisphere parameter R  h

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Rh=P50(Pa+20−PaPb+20−Pb)
R

h

=

P

50

(

P

a

+

20

−

P

a

P

b

+

20

−

P

b

)


Also a higher value of _P_ 50 is observed in case of the infarct hemisphere. Multiplying by _P_ 50 enhances the difference of Hemisphere parameter between the infarct (noninfarct) hemispheres.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## R  h  for infarct and noninfarct hemisphere

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Synthetic Data Creation for Accuracy Estimation

## Slice identification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, (a) An example of synthetic noninfarct slice created from original infarct slice and (b) example of synthetic images with combination of different foreground (infarct types) on the same background.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/7_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Hemisphere identification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Slice Identification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, (a) Comparison of ground truth slices, algorithm-identified infarct slices, and whole volume, and (b) results of sensitivity, specificity, and Dice statistical index for the slice identification procedure.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/8_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 6
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 7
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Hemisphere Identification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Results of Hemisphere Identification


Case GT AR 1 L L 2 R R 3 L R 4 R R 5 R R 6 R R 7 L L 8 L L 9 R R 10 L L 11 L L 12 L L 13 L L 14 R R 15 R R 16 R R 17 R R 18 R R 19 R R 20 L L 21 R R 22 R R 23 L L 24 L L 25 R R 26 R R 27 R R 28 L L 29 L R 30 R R 31 L L 32 L L 33 R L 34 R R 35 L L 36 L L

GT: ground truth, AR: Algorithm result, L: Left hemisphere, R: Right Hemisphere.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Accuracy of the Algorithm

## Slice identification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, (a) Area under receiver operating characteristic curves (AUC) corresponding to normalized R s determined for real cases with different artifact densities. AUC decreases by about 15% when the artifact density increases. (b) Sensitivity of hemisphere identification decreases by ∼10%–20% when artifact density goes from low to high.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/9_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Hemisphere identification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 11, Illustration of sensitivity of slice parameter as compared with a median or ratio of difference of percentiles (see A/B in Fig 3 ) alone. Infarct slices are 13 to 29 in this example.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/10_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Infarct Slice Detection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Infarct Hemisphere Detection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Limitations and Further Improvements

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 12, Multistep postprocessing of diffusion-weighted images.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/11_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Potential

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## Testing for Peak Location

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Location of Flat Region

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

if slope>−0.01, extrema=x\_i else consider \[x\_i+1:x\_i+3\]
if slope

>

−

0.01

, extrema

=

x\_i else consider \[x\_i+1:x\_i+3\]


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure A, Different shapes of peaks and flat regions.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomaticandRapidIdentificationofInfarctSlicesandHemisphereinDWIScans/12_1s20S1076633207004527.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Menezes N.M., Ay H., Wang Zhu M., et. al.: The real estate factor: quantifying the impact of infarct location on stroke severity. Stroke 2007; 38: pp. 194-197.


- 2\. Martel A.L., Allder S.J., Delay G.S., et. al.: Measurement of infarct volume in infarct patients using adaptive segmentation of diffusion weighted MR images. MICCAI 1999; 1679: pp. 22-31.


- 3\. Li W., Li E., et. al.: Robust unsupervised segmentation of infarct lesion from diffusion tensor MR images using multiscale statistical classification and partial volume voxel reclassification. Neuroimage 2004; 23: pp. 1507-1518. J Tan


- 4\. Bhanu Prakash K.N., Gupta V., Bilello M., et. al.: Identification, segmentation and image property study of acute infarcts in diffusion-weighted images by using a probabilistic neural network and adaptive gaussian mixture model. Acad Radiol 2006; 13: pp. 1474-1484.


- 5\.  Bhanu Prakash KN, Gupta V, Nowinski WL. Segmenting infarct in diffusion weighted imaging volumes. PCT/SG2006/000292, filed 3 October 2006.


- 6\. Nowinski W.L., Bhanu Prakash K.N., Volkau I., et. al.: Rapid and automatic calculation of the midsagittal plane in magnetic resonance diffusion and perfusion images. Acad Radiol 2006; 13: pp. 652-663.


- 7\. Nowinski W.L., Qian G., Bhanu Prakash K.N., et. al.: A CAD system for stroke MR and CT.2006.pp. 789. 92 Radiological Society of North America Scientific Assembly and Annual Meeting Program 2006, Chicago, IL: 25 November–1 December


- 8\. Bezdec J.C.: Pattern recognition with fuzzy objective function algorithms.1981.Plenum PressNew York


- 9\.  Weisstein EW. Gaussian function. Available online from MathWorld:  http://mathworld.wolfram.com/GaussianFunction.html

- 10\. Gibbons J.D.: Nonparametric statistical inference.ed 21985.M. Dekker


- 11\. Mann H.B., Whitney D.R.: On a test of whether one of 2 random variables is stochastically larger than the other. Annals of Mathematical Statistics 1947; 18: pp. 50-60.


- 12\. Linn S.: A new conceptual approach to teaching the interpretation of clinical tests. J Stat Educ 2004; 12: Available online from:  www.amstat.org/publications/jse/v12n3/linn.html

- 13\. Zou K.H., Warfield S.K., Bharatha A., et. al.: Statistical validation of image segmentation quality based on spatial overlap index. Acad Radiol 2004; 11: pp. 178-189.


- 14\. Kinnard L.M., Lo S.C.B., Duckett E., et. al.: Mass segmentation of dense breasts on digitized mammograms: Analysis of probability-based function. Medical Imaging 2005; 5747: pp. 1813-1823. Image Processing. Proceedings of the SPIE 2005


- 15\. Hanley J.A., McNeil B.J.: The meaning and use of area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 16\. Moritani T., Ekholm S., Westesson P.L.: Diffusion weighted MR imaging of the brain.2005.Springer-VerlagBerlin


- 17\. Bammer R., Markl M., Barnett A., et. al.: Analysis and generalized correction of the effect of spatial gradient field distortions in diffusion-weighted imaging. Magnet Reson Med 2003; 20: pp. 560-569.


- 18\. Nowinski W.L., Qian G., Bhanu Prakash K.N., et. al.: Analysis of ischemic stroke MR images by means of brain atlases of anatomy and blood supply territories. Acad Radiol 2006; 13: pp. 1025-1034.


- 19\. Nowinski W.L., Thirunavuukarasuu A.: The Cerefy clinical brain atlas on CD-ROM.2004.ThiemeNew York