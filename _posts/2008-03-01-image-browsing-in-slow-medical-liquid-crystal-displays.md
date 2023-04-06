---
title: Image Browsing in Slow Medical Liquid Crystal Displays
author: [Hongye Liang PhD,Subok Park PhD,Bron D. Gallas PhD,Kyle J. Myers PhD,Aldo Badano PhD]
date: 2008-03-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 15, Issue 3 SOURCE CL_S_AcademicRadiologyVolume15Issue3 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Statistics show that radiologists are reading more studies than ever before, creating the challenge of interpreting an increasing number of images without compromising diagnostic performance. Stack-mode image display has the potential to allow radiologists to browse large three-dimensional (3D) datasets at refresh rates as high as 30 images/second. In this framework, the slow temporal response of liquid crystal displays (LCDs) can compromise the image quality when the images are browsed in a fast sequence.

## Materials and Methods

In this article, we report on the effect of the LCD response time at different image browsing speeds based on the performance of a contrast-sensitive channelized-hoteling observer. A stack of simulated 3D clustered lumpy background images with a designer nodule to be detected is used. The effect of different browsing speeds is calculated with LCD temporal response measurements from our previous work. The image set is then analyzed by the model observer, which has been shown to predict human detection performance in Gaussian and non-Gaussian lumpy backgrounds. This methodology allows us to quantify the effect of slow temporal response of medical liquid crystal displays on the performance of the anthropomorphic observers.

## Results

We find that the slow temporal response of the display device greatly affects lesion contrast and observer performance. A detectability decrease of more than 40% could be caused by the slow response of the display.

## Conclusions

After validation with human observers, this methodology can be applied to more realistic background data with the goal of providing recommendations for the browsing speed of large volumetric image datasets (from computed tomography, magnetic resonance, or tomosynthesis) when read in stack-mode.

The high-fidelity display of medical images helps radiologists make correct diagnoses. Active-matrix liquid crystal displays (LCDs) are taking the place of traditional cathode-ray tube (CRT) displays and hard-copy films in most medical diagnostic imaging modalities. The image quality of LCD monitors has been significantly improved over the last few years. High-performance LCDs are considered to have comparable or better performance than CRTs in displaying static images for all aspects of display performances except noise and viewing angle ( ). However, LCDs can be inferior to CRTs at displaying moving scenes due to their slow response and the hold-type addressing scheme used in their pixel addressing methods ( ).

With the increasing number of computed tomography (CT) images to be interpreted per day, the ability of showing a fast sequence of images in stack-mode has been described as a preferred choice for a medical display. When using stack-mode browsing, slices are stacked on top of each other in the display memory buffer. At a given point, only one image is visible on the screen with the images being browsed back and forth at high image refresh rates under the control of the radiologist. When a high browsing speed is used, the radiologist perceives a three-dimensional (3D) volumetric image instead of a series of separate slices. The refresh rate could reach 30 images per second (ie, the duration for each specific image on the screen is only 33 milliseconds) depending on the application and equipment used ( ). Further increase of browsing speed with the advancement of technology is expected.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633208X00960/S1076633207006277/gr1.jpg?Signature=eD1K8d4aeWQaeo4tNMNCgx98dqUxMgjONjSkYE2XAGMX9A%7EV2MvlZ8AtN6s8niTYVob1XvSOAgz%7EBWQqTZn2Pr1X136TxuNZ-j5wPT86b5Px9f3JwRHc1q1rCfx3w3VxM98efz6k4Xvrpy4oLsz8Q5Af4pYqYw%7EJ8tYteyiCWmY_&Expires=1669524286&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Luminance change for a dynamic scene. _L  0  (i, j, n)_ indicates the target luminance of pixel ( _i, j_ ) at frame _n_ , corresponding to a gray level _g  0  (i, j, n)_ . At frame _n + 1_ , the target gray level is _g  0  (i, j, n + 1)_ (target luminance level _L  0  (i, j, n + 1)_ ). Because of slow temporal response, the achieved luminance at frame _n + 1_ is _L(i, j, n + 1)_ . The profile of luminance change from frame _n_ to _n + 1_ may take different forms, as indicated by the dashed lines, depending on different liquid crystal display technologies and different gray level transitions.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Measurements

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation of Temporal Effects

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, The three-dimensional CLBs can be generated with different spatial frequencies and contrasts by using different numbers and distributions of clusters, blobs, and different blob sizes. K is the number of clusters, N k is the number of blobs, and L x , L y are the dimensions of the blobs. The images are normalized to a maximum gray level of 225. (a) K = 50, N k = 10, L x = 2, L y = 1. (b) K = 50, N k = 10, L x = 3, L y = 2. (c) K = 50, N k = 10, L x = 4, L y = 2. (d) K = 100, N k = 10, L x = 2, L y = 1. (e) K = 100, N k = 10, L x = 3, L y = 2. (f) K = 100, N k = 10, L x = 4, L y = 2 (g) K = 200, N k = 10, L x = 2, L y = 1 (h) K = 200, N k = 10, L x = 3, L y = 2. (i) K = 200, N k = 10, L x = 4, L y = 2.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/0_1s20S1076633207006277.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

g(r)=∑Kk=1∑Nkn=1b(1akn(r−rk−rkn),Rθkn)
g

(

r

)

=

∑

k

=

1

K

∑

n

=

1

N

k

b

(

1

a

k

n

(

r

−

r

k

−

r

k

n

)

,

R

θ

k

n

)


where _r  k_ represents position of the k _th_ cluster, _a  kn_ represents scale of the n _th_ blob within the k _th_ cluster, θ _kn_ is rotation angle of the n _th_ blob within the k _th_ cluster, and _b(r,R  θ  )_ is blob profile rotated at angle θ. To represent the power-law characteristics of the background, asymmetrical exponential blobs are used with characteristic length _L  x_ and _L  y_ in _x_ and _y_ directions. The details can be found elsewhere ( ). In this work, blobs and clusters are randomly distributed in a 3D cube to simulate 3D breast CT or tomosynthesis slices. Fifty independent 3D CLBs are generated for the temporal effect calculation. The mean number of clusters was set to be 160, and the mean number of blobs per cluster was set to be 20. The designer nodule is used as a signal to be detected ( ) and added to the center slice.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

L(n)=L(n−1)+ΔL(g0(n),C−1(L(n−1)))\*P(g0(n),C−1(L(n−1)))
L

(

n

)

=

L

(

n

−

1

)

+

Δ

L

(

g

0

(

n

)

,

C

−

1

(

L

(

n

−

1

)

)

)

\*

P

(

g

0

(

n

)

,

C

−

1

(

L

(

n

−

1

)

)

)


where _g  0  (n)_ is the target gray level of pixel ( _i, j_ ) at time index n, _L(n − 1)_ is the achieved luminance level at the end of frame _n−1_ . The achieved gray level corresponding to an arbitrary screen luminance is calculated using the luminance response function of the device ( _L = C(g)_ ). Because actual luminance values are mapped to a floating-point representation of the gray scale, we define _C  −1  (L)_ as its nearest integer value. Δ _L(\*)_ is the theoretical increase in luminance given by the grayscale calibration of the display device for the corresponding gray levels, and denotes the element-wise multiplication of matrix elements. For the next time index or frame, a similar equation can be written:


L(n+1)=L(n)+ΔL(g0(n+1),C−1(L(n)))\*P(g0(n+1),C−1(L(n)))
L

(

n

+

1

)

=

L

(

n

)

+

Δ

L

(

g

0

(

n

+

1

)

,

C

−

1

(

L

(

n

)

)

)

\*

P

(

g

0

(

n

+

1

)

,

C

−

1

(

L

(

n

)

)

)


The change of luminance at pixel ( _i,j_ ) is illustrated in  Fig 3 . Note that the luminance level depends not only on the temporal characteristics of the display device, but also on the history of the pixel luminance. The calculations assume that luminance is constant in a frame time, shown as the horizontal thick lines in the graph. In reality it will take some time for the luminance to change from frame _n −1_ to _n_ . The luminance may take different tracks depending on different transitions and display technology, as illustrated in  Fig 1 for transition at frame _n_ . We also consider the linear case to compare with the constant luminance case. The linear approximation assumes that the integrated luminance is a good estimate for the perceived luminance. Alternatively, a constant luminance model can also be used. By running the CLB slices through such an LCD temporal response model, images that represent actual displayed values on LCDs can be calculated.  Figure 4 shows an example of our method to simulate temporal response effects on medical images.

![Figure 3, Pixel luminance change at different frames. L(n − 1) is the achieved luminance of pixel ( i, j ) at frame n − 1 , corresponding to a gray level g(n − 1) , which can be obtained from the display luminance curve ( L(n) = C(g(n)) ). At frame n , the target gray level is g 0 (n) (target luminance level L 0 (n) ). Because of slow temporal response, the achieved luminance at frame n is L(n) . In some cases, the luminance at the end of a frame is taken as the perceived luminance. If the luminance transition within a frame is considered, the perceived luminance can be approximated to be the average luminance in the frame as shown by ̄L .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/1_1s20S1076633207006277.jpg)

![Figure 4, Example of a clustered lumpy background used in the study, with 3D extension of clustered lumpy background (15) and designer mass (16). The central slice with the signal corresponding to a fast (left) and a slow (right) response device are shown.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/2_1s20S1076633207006277.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

LC=Ls−LbLb
L

C

=

L

s

−

L

b

L

b


where _L  s_ is the average luminance of the signal and _L  b_ is the average luminance of the background in the region adjacent to the signal. However, this metric doesn’t always correlate with detectability. To further quantify the effects of temporal response, a computational observer was used to estimate detectability under different browsing speeds.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Temporal response measurements corresponding to different devices ( (a) 1 million and (b) 5 million pixels) used in the study to simulate the effect of the different display temporal characteristics on target detection. Contour lines indicate the response time for different regions in the plots.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/3_1s20S1076633207006277.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Luminance achieved after one, two, three, and four frames expressed as a percentage of the desired transition to the target luminance for display 1 million pixel color display: after one frame (a) , two frames (b) , three frames (c) , and four frames (d) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/4_1s20S1076633207006277.jpg)

![Figure 7, Luminance achieved after one, two, three, and four frames expressed as a percentage of the desired transition to the target luminance for display 5 million pixel monochromatic display: after one frame (a) , two frames (b) , three frames (c) , and four frames (d) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/5_1s20S1076633207006277.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Reduction in contrast (a) and in detectability (b) , expressed as the area under the receiver operating characteristic curve, for 1 million pixel and 5 million pixel displays with a constant luminance model.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/6_1s20S1076633207006277.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Reduction in contrast (a) and in detectability (b) , expressed as the area under the receiver operating characteristic curve, for 1 million pixel and 5 million pixel displays, with a linear luminance transition model.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ImageBrowsinginSlowMedicalLiquidCrystalDisplays/7_1s20S1076633207006277.jpg)

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

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix

## Computational model observer

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

C(l¯)=1C0csf(μ,l¯)
C

(

l

¯

)

=

1

C

0

c

s

f

(

μ

,

l

¯

)


where μ is the frequency of the signal to be detected, _̄l_ is the mean luminance in a field of view (FOV) of an image, and _csf(.)_ is the contrast sensitivity model of the human visual system. Then we use _C(̄l)_ to determine if a pixel luminance is above the threshold:


lk−l¯l¯<C(l¯)→lk=l¯
l

k

−

l

¯

l

¯

<

C

(

l

¯

)

→

l

k

=

l

¯


where _l  k_ is the luminance of the k _th_ pixel in the image. If the given relation is satisfied, the luminance of the kth pixel in the image is replaced by the mean luminance of the field of view; if not, the luminance of the k _th_ pixel is left unchanged. Finally, the CHO with difference-of-Gaussian channels was applied to the resulting image. We fixed _C_ at a value for which the csCHO matches human performance in one of the experiment conditions. Then we calculated the csCHO performance for the other experiments. csCHO has been shown to well predict human performance in detection tasks using lumpy backgrounds. More details on the performance of the csCHO will be presented in a separate article ( ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Badano A.: AAPM/RSNA tutorial on equipment selection: PACS equipment overview: display systems. Radiographics 2004; 24: pp. 879-889.


- 2\. Tsukuda T.: TFT/LCD: liquid crystal displays addressed by thin film transistors.1996.Gordon and Breach Science PublishersAmsterdam, The Netherlands


- 3\. Kurita T., Saito A., Yuyama I.: Consideration on perceived MTF of hold type display for moving images. Proc Int Display Workshop’98 1998; pp. 823-826.


- 4\. Miseli J.: Motion artifacts. Proc SID 2004; pp. 86-89.


- 5\. Mathie A.G., Strickland N.H.: Interpretation of CT scans with PACS image display in stack mode. Radiology 1997; 203: pp. 207-209.


- 6\. Reiner B.I., Siegel E.L., Hooper F.J., et. al.: Radiologists productivity in the interpretation of CT scans: a comparison of PACS with conventional film. AJR Am J Roentgenol 2001; 176: pp. 861-864.


- 7\. den Boer W.: Active Matrix liquid crystal displays: fundamentals and applications.2005.ElsevierBurlington, MA


- 8\. Nakamura H., Crain J., Sekiya K.: Optimized active-matrix drives for liquid crystal displays. J Appl Phys 2001; 90: pp. 2122-2127.


- 9\. Barrett H.H., Myers K.J.: Foundations of image science.2004.WileyHoboken, NJ


- 10\. Park S., Gallas B.D., Badano A., et. al.: Efficiency of the human observer for detecting a gaussian signal at a known location in non-gaussian distributed lumpy backgrounds. J Optical Soc Am A Optics Image Sci Vision 2007; 24: pp. 911-921.


- 11\. Myers K.J., Barrett H.H.: Addition of a channel mechanism to the ideal-observer model. J Opt Soc Am A 1987; 4: pp. 2447-2457.


- 12\. Abbey C.K., Barrett H.H.: Human- and model-observer performance in ramp-spectrum noise: effects of regularization and object variability. J Opt Soc Am A 2001; 18: pp. 473-487.


- 13\. Gallas D.B., Barrett H.H.: Validating the use of channels to estimate the ideal linear observer. J Opt Soc Am A 2003; 20: pp. 1725-1738.


- 14\. Liang H., Badano A.: Precision of gray level response time measurements of medical liquid crystal display. Rev Scient Instr 2006; 77: pp. 065104.


- 15\. Bochud F.O., Abbey C.K., Eckstein M.P.: Statistical texture synthesis of mammographic images with clustered lumpy backgrounds. Optic Exp 1999; 4: pp. 33-43.


- 16\. Burgess E.A., Jacobson F.L., Judy P.F.: Human observer detection experiments with mammograms and power-law noise. Med Phys 2001; 28: pp. 419-437.


- 17\. Barten P.G.J.: Contrast sensitivity of the human eye and its effects on image quality.1999.SPIE PressBellingham, WA


- 18\. Eckstein M.P., Whiting J.S., Thomas J.P.: Role of knowledge in human visual temporal integration in spatiotemporal noise. J Opt Soc Am A 1996; 13: pp. 1960-1968.


- 19\. Bartlett N.R.: Thresholds as dependent on some energy relations and characteristics of the subject.Graham C.H.Vision and visual perception.1965.WileyNew York:pp. 154-184.


- 20\. Liang H., Badano A.: Temporal response of medical liquid crystal displays. Med Phys 2007; 34: pp. 639-646.


- 21\.  Park S, Badano A, Gallas BD, et al. A contrast-sensitive channelized observer. IEEE Trans Med Imaging. In press.