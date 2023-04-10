---
title: Motion Correction of Multi-b-value Diffusion-weighted Imaging in the Liver
author: [CL_AT_YousefMazaheriPhD,CL_AT_RichardKGDoMDPhD,CL_AT_AmitaShuklaDavePhD,CL_AT_JosephODeasyPhD,CL_AT_YonggangLuPhD,CL_AT_OguzAkinMD]
date: 2012-12-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 12]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Motion artifacts are a significant source of error in the acquisition and quantification of parameters from multi-b-value diffusion-weighted imaging (DWI). The objective of this article is to present a reliable method to reduce motion-related artifacts during free-breathing at higher b-values when signal levels are low.

## Materials and Methods

Twelve patients referred for magnetic resonance imaging of the liver underwent a clinical magnetic resonance imaging examination of the abdominal region that included DWI. Conventional single-shot spin-echo echo planar imaging acquisitions of the liver during free breathing were repeated in a “time-resolved” manner during a single acquisition to obtain data for multi-b-value analysis, alternating between low and high b-values. Image registration using a normalized mutual information similarity measure was used to correct for spatial misalignment of diffusion-weighted volumes caused by motion. Registration error was estimated indirectly by comparing the normalized root-mean-square error (NRMSE) values of data fitted to the biexponential intra-voxel incoherent motion model before and after motion correction. Regions of interest (ROIs) were selected in the liver close to the surface of the liver and close to internal structures such as large bile ducts and blood vessels.

## Results

For the 12 patient datasets, the mean NRMSE value for the motion-corrected ROIs (0.38 ± 0.16) was significantly lower than the mean NRMSE values for the non–motion-corrected ROIs (0.41 ± 0.13) ( _P_ < .05). In cases where there was substantial respiratory motion during the acquisition, visual inspection verified that the algorithm markedly improved alignment of the liver contours between frames.

## Conclusions

The proposed method addresses motion-related artifacts to increase robustness in multi-b-value acquisitions.

In biological tissues, microscopic motion detected by diffusion-weighted imaging (DWI) includes both diffusion of water molecules, influenced by the structural components of the tissue, and microcirculation of blood in the capillary network (perfusion). When the diffusion sensitivity parameter, referred to as the b-value, is low, microperfusion causes rapid signal decay. To separate microperfusion effects from tissue diffusion in DWI studies, Le Bihan proposed the intravoxel incoherent motion (IVIM) biexponential model .

Several studies have applied an IVIM non-monoexponential model to characterize diffusion in tumors of the body . Application of the IVIM model, however, has been hindered by the presence of bulk motion and physiologic motions such as respiration. DWI is sensitive to both molecular displacement and the mean length of blood perfusion within the capillary network, both of which are of the order of tens of microns . However, body motion can produce displacements of the order of several millimeters, causing severe artifacts that interfere with calculation of DWI parameters.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Biexponential Model for Diffusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

s(b)=S(0)⋅\[(1−f)⋅exp(−b⋅D)+f⋅exp(−b⋅D∗)\]
s

(

b

)

=

S

(

0

)

⋅

\[

(

1

−

f

)

⋅

exp

(

−

b

⋅

D

)

+

f

⋅

exp

(

−

b

⋅

D

∗

)

\]


where _D_ is the slow component of diffusion which describes true diffusion of extravascular water molecules, _D\*_ is the perfusion coefficient, _f_ is the perfusion fraction, and S(b)
S

(

b

)
and S(0)
S

(

0

)
are the signal measured in each individual voxel in the DWI with diffusion sensitivity of _b_ and 0, respectively. To estimate diffusion parameters with this model, diffusion signal is measured for a large number of b-values, ranging from very low (<200 s/mm  2 ) to high (>200 s/mm  2 ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Magnetic Resonance Imaging Data Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Motion Correction of Multi-b-value DWI

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Schematic diagram of the motion correction of multi-b-value diffusion-weighted imaging technique. (a) The data are acquired during two phases. Phase 1: Image frames are acquired without diffusion-weighted gradients (b = 0) to minimize T 1 -weighting because of incomplete recovery of longitudinal magnetization at shorter TRs. Phase 2: Image frames are acquired with non-zero b-values. High (H 1 , H 2 , H 3 , …) and low (L 1 , L 2 , L 3 , …) b-values are interleaved. This is to allow spatial transformation parameters for low-signal high-b–value images to be approximated using the spatial transformation parameters from adjacent low b-value frames. (b) Three b = 0 frames are acquired (Phase 1) followed by four blocks of b-values (4 × 9, total of 36) (Phase 2). In total, 39 frames are acquired.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MotionCorrectionofMultibvalueDiffusionweightedImagingintheLiver/0_1s20S1076633212003832.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Phase 1

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Phase 2

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Registration: Three-dimensional Affine Transformation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

NMI(X,Y)=H(X)+H(Y)H(X,Y)
N

M

I

(

X

,

Y

)

=

H

(

X

)

+

H

(

Y

)

H

(

X

,

Y

)


where X is the reference (or source image) and Y is the target image. The quantities (and H(Y)
H

(

Y

)
) are the standard entropy definition entropy functions given by:


H(X)=−∑ip(i)⋅logp(i)
H

(

X

)

=

−

∑

i

p

(

i

)

⋅

log

p

(

i

)


where p(i)
p

(

i

)
is the marginal probability distribution and H(X,Y)
H

(

X

,

Y

)
is the joint distribution function given by:


H(X,Y)=∑ijp(i,j)⋅logp(i,j)p(i)⋅p(j)
H

(

X

,

Y

)

=

∑

i

j

p

(

i

,

j

)

⋅

log

p

(

i

,

j

)

p

(

i

)

⋅

p

(

j

)


where p(i,j)
p

(

i

,

j

)
represents the probability estimated using the (i,j)
(

i

,

j

)
joint histogram bin of the image pixel values of the reference and source image. The joint probability density functions describe the probability that a pair of values, one from each image in the comparison, occurs at the same spatial location. When two image volumes are matched, their mutual information is maximized. Affine transformation in three dimensions was used to register DW images in each acquisition. Three-dimensional (3D) affine transformation describes a global space warping with 12 degrees of freedom. The 3D affine transformation of a point x=(x,y,z)T
x

=

(

x

,

y

,

z

)

T
can be written as :


A(x)=A⋅x+T
A

(

x

)

=

A

⋅

x

+

T


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

A=R(,,ψ)⎡⎣⎢1SyxSzxSxy1SyzSxzSyz1⎤⎦⎥⎡⎣⎢Sx000Sy000Sz⎤⎦⎥
A

=

R

(

,

,

ψ

)

\[

1

S

x

y

S

x

z

S

y

x

1

S

y

z

S

z

x

S

y

z

1

\]

\[

S

x

0

0

0

S

y

0

0

0

S

z

\]


where R(,,ψ)
R

(

,

,

ψ

)
is a 3 × 3 rotation matrix, given by:


R(,,ψ)=⎡⎣⎢1000cos−sin0−sincos⎤⎦⎥×⎡⎣⎢cos0−sin010sin0cos⎤⎦⎥⎡⎣⎢cosψsinψ0−sinψcosψ0001⎤⎦⎥
R

(

,

,

ψ

)

=

\[

1

0

0

0

cos

−

sin

0

−

sin

cos

\]

×

\[

cos

0

sin

0

1

0

−

sin

0

cos

\]

\[

cos

ψ

−

sin

ψ

0

sin

ψ

cos

ψ

0

0

0

1

\]


and {Sx,Sy,Sz}
{

S

x

,

S

y

,

S

z

}
are scale factors in three orthogonal directions, and {Sxy,Sxz,Syz,Syx,Szx,Szy}
{

S

x

y

,

S

x

z

,

S

y

z

,

S

y

x

,

S

z

x

,

S

z

y

}
are 3D shear parameters in the XY, XZ, YZ, YX, ZX, and ZY directions.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

NRMSE=1xdata,max−xdata,min∑Ni=1(xdata,i−xmod,i)2N−−−−−−−−−−−−−√
N

R

M

S

E

=

1

x

d

a

t

a

,

m

a

x

−

x

d

a

t

a

,

m

i

n

∑

i

=

1

N

(

x

d

a

t

a

,

i

−

x

m

o

d

,

i

)

2

N


where xdata,i
x

d

a

t

a

,

i
is the (pre- or post-registered) data and xmod,i
x

m

o

d

,

i
is the (pre- or postregistered) biexponential fit, and _N_ is the number of voxels in the ROI. NRMSE is expressed as a percentage, where lower values indicate less residual variance. The NRMSE of each ROI for each patient was calculated and was regarded as an indirect measure of the ability of the registration algorithm to correct for motion. The nonparametric Wilcoxon signed-rank test was used to test statistical significance between pre- and postregistered NRMSEs. A _P_ value of .05 or less was defined as significant.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Images obtained using motion correction of multi-b-value diffusion-weighted imaging. (a) Images obtained with diffusion sensitivity parameters 200, 400, and 800 s/mm 2 . (b) Scatter plots corresponding ( from left to right ) to the images shown in (a) . By comparing the plots, we can detect if the mutual information or pixel distance can be used as a similarity measure. Reduced signal can limit the accuracy of motion correction. We used the criteria sum(abs(HX-HY))<0.5 , where HX and HY are the normalized standard entropy of the source and target images. For the plots, the sum(abs(HX-HY)) values corresponding to b-values 200, 400 and 800 s/mm 2 were 0.34, 0.45, and 0.74, respectively, suggesting that b-values >400 s/mm 2 result in images with low signal and contrast.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MotionCorrectionofMultibvalueDiffusionweightedImagingintheLiver/1_1s20S1076633212003832.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Plot of three-dimensional affine transformation parameters for the 39 frames acquired during an abdominal exam. (a) Translational parameters (translate X, translate Y, and translate Z), (b) Shear parameters (shear XY, shear XZ, and shear YX) and (c) (shear YZ, shear ZX, and shear ZY). Motion parameters were estimated during acquisition of high-signal low b-value images ( colored markers represent target frames ), which can then be interpolated to the adjacent high b-value images that lack sufficient signal for reliable motion estimation ( black markers represent interpolated frames ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MotionCorrectionofMultibvalueDiffusionweightedImagingintheLiver/2_1s20S1076633212003832.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Regions of interest (ROIs) placed on a diffusion-weighted image (b = 0) of the liver (a) . Plots of mean signal intensity and the biexponential fit for the ROIs pre- (b) and postregistration (c) . The biexponential parameters D *, D , and f were extracted. The preregistration fitted parameters were D * = 0.04 mm 2 /s, D = 1.3 × 10 −3 mm 2 /s, and f = 0.17 for blue ROI, and D * = 0.014 mm 2 /s, D = 1.2 × 10 −3 mm 2 /s, and f = 0.27 for green ROI. The postregistration fitted parameters were D * = 0.04 mm 2 /s, D = 1.0 × 10 −3 mm 2 /s, and f = 0.25 for blue ROI, and D * = 0.063 mm 2 /s, D = 0.9 × 10 −3 mm 2 /s, and f = 0.44 for green ROI.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MotionCorrectionofMultibvalueDiffusionweightedImagingintheLiver/3_1s20S1076633212003832.jpg)

Table 1


The Mean NRMSE of Data Fitted to the Biexponential IVIM Model Value before Motion Correction and after Motion Correction for the 12 Patient Datasets


Subject NRMSE before Motion Correction NRMSE after Motion Correction 1 0.61 0.59 2 0.65 0.64 3 0.43 0.44 4 0.35 0.36 5 0.61 0.60 6 0.32 0.16 7 0.34 0.27 8 0.27 0.27 9 0.36 0.35 10 0.35 0.33 11 0.40 0.37 12 0.28 0.17 Average ± SD 0.41 ± 0.13 0.38 ± 0.16

IVIM, intra-voxel incoherent motion; NRMSE, normalized root-mean-square error; SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Registration of target image to the reference image. (a) Reference image (frame 1, b = 0 s/mm 2 ). For comparison, the contour of the liver ( blue ) from frame 1 is copied in its original location in each subsequent frame. (b) Pre- ( left ) and postregistration images of the same slice from frame 29 (b = 70 s/mm 2 ). In the preregistered image, the liver and the contour do not match. Postregistration, there is an improvement in the alignment of the liver edge and the contour copied from frame 1. (c) Similarly, for frame 36 (b = 150 s/mm 2 ), the liver edge in the preregistered image ( left ) does not match the contour. The alignment is improved in the postregistration image ( right ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MotionCorrectionofMultibvalueDiffusionweightedImagingintheLiver/4_1s20S1076633212003832.jpg)

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Le Bihan D., Turner R., MacFall J.R.: Effects of intravoxel incoherent motions (IVIM) in steady-state free precession (SSFP) imaging: application to molecular diffusion imaging. Magn Reson Med 1989; 10: pp. 324-337.


- 2\. Le Bihan D., Breton E., Lallemand D., et. al.: MR imaging of intravoxel incoherent motions: application to diffusion and perfusion in neurologic disorders. Radiology 1986; 161: pp. 401-407.


- 3\. Le Bihan D., Breton E., Lallemand D., et. al.: Separation of diffusion and perfusion in intravoxel incoherent motion MR imaging. Radiology 1988; 168: pp. 497-505.


- 4\. Yamada I., Aung W., Himeno Y., et. al.: Diffusion coefficients in abdominal organs and hepatic lesions: evaluation with intravoxel incoherent motion echo-planar MR imaging. Radiology 1999; 210: pp. 617-623.


- 5\. Luciani A., Vignaud A., Cavet M., et. al.: Liver cirrhosis: intravoxel incoherent motion MR imaging—pilot study. Radiology 2008; 249: pp. 891-899.


- 6\. Patel J., Sigmund E.E., Rusinek H., et. al.: Diagnosis of cirrhosis with intravoxel incoherent motion diffusion MRI and dynamic contrast-enhanced MRI alone and in combination: preliminary experience. J Magn Reson Imaging 2010; 31: pp. 589-600.


- 7\. Sigmund E.E., Cho G.Y., Kim S., et. al.: Intravoxel incoherent motion imaging of tumor microenvironment in locally advanced breast cancer. Magn Reson Med 2011; 65: pp. 1437-1447.


- 8\. Lemke A., Laun F.B., Klauss M., et. al.: Differentiation of pancreas carcinoma from healthy pancreatic tissue using multiple b-values: comparison of apparent diffusion coefficient and intravoxel incoherent motion derived parameters. Invest Radiol 2009; 44: pp. 769-775.


- 9\. Riches S.F., Hawtin K., Charles-Edwards E.M., et. al.: Diffusion-weighted imaging of the prostate and rectal wall: comparison of biexponential and monoexponential modelled diffusion and associated perfusion coefficients. NMR Biomed 2009; 22: pp. 318-325.


- 10\. Chandarana H., Lee V.S., Hecht E., et. al.: Comparison of biexponential and monoexponential model of diffusion weighted imaging in evaluation of renal lesions: preliminary experience. Investigative Radiology 2011; 46: pp. 285-291.


- 11\. Pawlik G., Rackl A., Bing R.J.: Quantitative capillary topography and blood flow in the cerebral cortex of cats: an in vivo microscopic study. Brain Res 1981; 208: pp. 35-58.


- 12\. Chow L.C., Bammer R., Moseley M.E., et. al.: Single breath-hold diffusion-weighted imaging of the abdomen. J Magn Reson Imaging 2003; 18: pp. 377-382.


- 13\. Taouli B., Sandberg A., Stemmer A., et. al.: Diffusion-weighted imaging of the liver: comparison of navigator triggered and breathhold acquisitions. J Magn Reson Imaging 2009; 30: pp. 561-568.


- 14\. Taouli B., Koh D.M.: Diffusion-weighted MR imaging of the liver. Radiology 2010; 254: pp. 47-66.


- 15\. Koh D.M., Collins D.J.: Diffusion-weighted MRI in the body: applications and challenges in oncology. AJR Am J Roentgenol 2007; 188: pp. 1622-1635.


- 16\. Kandpal H., Sharma R., Madhusudhan K.S., et. al.: Respiratory-triggered versus breath-hold diffusion-weighted MRI of liver lesions: comparison of image quality and apparent diffusion coefficient values. AJR Am J Roentgenol 2009; 192: pp. 915-922.


- 17\. Kim D.H., Chung S., Vigneron D.B., et. al.: Diffusion-weighted imaging of the fetal brain in vivo. Magn Reson Med 2008; 59: pp. 216-220.


- 18\. Rohde G.K., Barnett A.S., Basser P.J., et. al.: Comprehensive approach for correction of motion and distortion in diffusion-weighted MRI. Magn Reson Med 2004; 51: pp. 103-114.


- 19\. Shechter G., Resar J.R., McVeigh E.R.: Displacement and velocity of the coronary arteries: cardiac and respiratory motion. IEEE Trans Med Imaging 2006; 25: pp. 369-375.


- 20\. Andersson J.L., Skare S.: A model-based method for retrospective correction of geometric distortions in diffusion-weighted EPI. NeuroImage 2002; 16: pp. 177-199.


- 21\. Wilson D.L., Carrillo A., Zheng L., et. al.: Evaluation of 3D image registration as applied to MR-guided thermal treatment of liver cancer. J Magn Reson Imaging 1998; 8: pp. 77-84.


- 22\. Rohlfing T., Maurer C.R., O'Dell W.G., et. al.: Modeling liver motion and deformation during the respiratory cycle using intensity-based nonrigid registration of gated MR images. Med Phys 2004; 31: pp. 427-432.


- 23\. Nasu K., Kuroki Y., Sekiguchi R., et. al.: Measurement of the apparent diffusion coefficient in the liver: is it a reliable index for hepatic disease diagnosis?. Radiat Med 2006; 24: pp. 438-444.


- 24\. Murtz P., Flacke S., Traber F., et. al.: Abdomen: diffusion-weighted MR imaging with pulse-triggered single-shot sequences. Radiology 2002; 224: pp. 258-264.


- 25\. Skare S., Andersson J.L.: On the effects of gating in diffusion imaging of the brain using single shot EPI. Magnetic Res Imaging 2001; 19: pp. 1125-1128.


- 26\. Kwee T.C., Takahara T., Niwa T., et. al.: Influence of cardiac motion on diffusion-weighted magnetic resonance imaging of the liver. Magma 2009; 22: pp. 319-325.


- 27\. Butts K., de Crespigny A., Pauly J.M., et. al.: Diffusion-weighted interleaved echo-planar imaging with a pair of orthogonal navigator echoes. Magn Reson Med 1996; 35: pp. 763-770.


- 28\. Zur Y., Stokar S., Bendel P.: An analysis of fast imaging sequences with steady-state transverse magnetization refocusing. Magn Reson Med 1988; 6: pp. 175-193.


- 29\. Stanisz G.J., Odrobina E.E., Pun J., et. al.: T1, T2 relaxation and magnetization transfer in tissue at 3T. Magn Reson Med 2005; 54: pp. 507-512.


- 30\. Jezzard P., Balaban R.S.: Correction for geometric distortion in echo planar images from B0 field variations. Magn Reson Med 1995; 34: pp. 65-73.


- 31\. Taouli B., Vilgrain V., Dumont E., et. al.: Evaluation of liver diffusion isotropy and characterization of focal hepatic lesions with two single-shot echo-planar MR imaging sequences: prospective study in 66 patients. Radiology 2003; 226: pp. 71-78.