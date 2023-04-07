---
title: An Anthropomorphic Breast Model for Breast Imaging Simulation and Optimization
author: [CL_AT_BaiyuChenBE,CL_AT_JamieShoreyPhD,CL_AT_RobertSSaundersPhD,CL_AT_SamuelRichardPhD,CL_AT_JohnThompsonMS,CL_AT_LorenWNoltePhD,CL_AT_EhsanSameiPhD]
date: 2011-05-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 18, Issue 5]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Optimization studies for x-ray−based breast imaging systems using computer simulation can greatly benefit from a phantom capable of modeling varying anatomical variability across different patients. This study aimed to develop a three-dimensional phantom model with realistic and randomizable anatomical features.

## Materials and Methods

A voxelized breast model was developed consisting of an outer layer of skin and subcutaneous fat, a mixture of glandular and adipose, stochastically generated ductal trees, masses, and microcalcifications. Randomized realization of the breast morphology provided a range of patient models. Compression models were included to represent the breast under various compression levels along different orientations. A Monte Carlo (MC) simulation code was adapted to simulate x-ray based imaging systems for the breast phantom. Simulated projections of the phantom at different angles were generated and reconstructed with iterative methods, simulating mammography, breast tomosynthesis, and computed tomography (CT) systems. Phantom dose maps were further generated for dosimetric evaluation.

## Results

Region of interest comparisons of simulated and real mammograms showed strong similarities in terms of appearance and features. Noise-power spectra of simulated mammographic images demonstrated that the phantom provided target properties for anatomical backgrounds. Reconstructed tomosynthesis and CT images and dose maps provided corresponding data from a single breast enabling optimization studies. Dosimetry result provided insight into the dose distribution difference between modalities and compression levels.

## Conclusion

The anthropomorphic breast phantom, combined with the MC simulation platform, generated a realistic model for a breast imaging system. The developed platform is expected to provide a versatile and powerful framework for optimizing volumetric breast imaging systems.

Breast imaging performance is highly affected by the spatial heterogeneity of the breast structure . Furthermore, breast density varies substantially across patients of different ages . As a result, optimizing breast imaging systems across a variety of cases requires the capability of modeling the heterogeneity and variability across patients. In recent years, a number of anthropomorphic breast models have been developed for breast-related research, including physical and computerized phantoms . Physical phantoms were employed for empirical performance measurements , whereas computerized phantoms were voxelized and embedded into computerized simulations . Computerized phantoms have shown advantages in optimization research because of their low cost, ability to imitate subtle tissue structures, and ability to represent varying physical properties. These phantoms are generally characterized into two categories: those based on data from computed tomography (CT) or magnetic resonance imaging (MRI) scans , and those defined by analytical descriptions of human anatomy . Phantoms based on CT or MRI data are highly realistic, because they are built from patient data; however, they are inherently limited by the employed scanning technique (eg, finite resolution, noise pattern, artifact). Furthermore, these phantoms are not representative of the whole population, because each phantom is built from one specific patient. In contrast, phantoms based on mathematical methods are not restricted by the imaging technique. While being not as realistic, they offer a larger flexibility of parameter, enabling breast models representative of large segments of the population. Furthermore, recent studies to improve on the realism of these phantoms have included advanced mathematical concepts such as fractal structure and self-similar structure implemented to model realistic breast structures .

Based on prior research, this work focuses on developing a mathematical breast phantom with compression models, which includes skin, adipose tissue, glandular tissue, ducts, microcalcifications, and masses . The phantom presented here improves on prior work in several ways with more realistic skin boundary definition, more accurate anatomical background structure, improved ductal connections and distribution, increased number of growing features in the stochastic mass definition, added microcalcifications, and the development of a deformation algorithm that compresses the breast along various orientations into various thicknesses objects. This project further includes dedicated Monte Carlo (MC) projection simulation and iterative image reconstruction software for simulating and optimizing breast imaging modalities.

## Materials and methods

## Breast Phantom Construction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Schematic representation of each component of the breast phantom.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/0_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Skin

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Background Texture

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

P(f)=1fβ,
P

(

f

)

=

1

f

β

,


where _f_ denotes spatial frequency and the _β_ factor denotes the Hausdorff dimension of a fractal structure . Previous research suggested that mammograms possess a mean _β_ value of 2.83 with a standard deviation of 0.35 , and that the _β_ value in a two-dimensional mammographic projection corresponds to the _β_ value in the three-dimensional (3D) volume . Thus, the 3D texture in this work employed a _β_ values randomly selected between 2.13 and 3.53 (ie, _β_ =2.83 ± 2\*0.35).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

H(u,v,w)=⎧⎩⎨⎪⎪01(u2+v2+w2√)β2u=v=w=0otherwise,
H

(

u

,

v

,

w

)

=

{

0

u

=

v

=

w

=

0

1

(

u

2

+

v

2

+

w

2

)

β

2

o

t

h

e

r

w

i

s

e

,


where (u,v,w)∈\[(−U,−V,−W),(U,V,W)\],
(

u

,

v

,

w

)

∈

\[

(

−

U

,

−

V

,

−

W

)

,

(

U

,

V

,

W

)

\]

,
and U, V, and W correspond to the Nyquist frequencies in the orthogonal direction (ie, 12Δx,12Δy,12Δz,
1

2

Δ

x

,

1

2

Δ

y

,

1

2

Δ

z

,
with Δx,Δy,Δz
Δ

x

,

Δ

y

,

Δ

z
characterizing the voxel size in three dimensions). The filtered volume representing the designed inverse power law distribution was converted to spatial domain by inverse Fourier transform, and thresholded by assigning each voxel to either a glandular or an adipose tissue value to produce the desired glandular tissue density. This thresholded matrix, however, had glandular and adipose tissue scattered and discontinued within the volume. To better imitate the pattern of background tissues, an additional smoothing process was performed to expand both the glandular and adipose region to be continuous.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Adipose and glandular tissue mixtures with different β values. The tissues tend to cluster with increasing β values.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/1_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Ductal Network

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The basic unit of the ductal network, defined by a cylindrical segment and a spherical junction. The subscript n denotes the level number of each segment.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/2_1s20S1076633210006306.jpg)

![Figure 4, The new direction of the progeny duct is calculated at the branching point using the old direction, polar angle increment d , and azimuthal angle increment dφ .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/3_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Parameters Used in the Ductal System Simulation for a Reasonable Visual Pattern


Parameter Symbol Value Radius of level 0_r_ 0  1 mm Length of level 0_l_ 0  5 mm Probability of a smaller progeny_p_ 1  32% Probability of bifurcation_p_ 2  28% Probability of no new progeny_p_ 3  40% Scaling factor between radii_a_ 0.8 Factor between radius and length_b_ 8 Lower limitation of segment length_q_ 1  % 40% Upper limitation of segment length_q_ 2  % 100% Polar angle of the new branch ± (37.5° ± 10°) Azimuthal angle of the new branch_φ_ ± (15° ± 5°)

![Figure 5, A ductal network simulated with three-dimensional branching algorithm.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/4_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Microcalcification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Breast Masses

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, The sigmoid distribution that decides the percentage of mass tissue in each concentric shell.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/5_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, (a) A single mass with a stochastic stellate pattern composed of a dense center and a gradually fading boundary. (b) In total six lesions are distributed in the craniocaudal mid-plane of the phantom, continually invading into normal tissues. Other structures, such as ducts, skin, adipose, and glandular tissue, are also presented.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/6_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Compression Models

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

(rR)6+(zT/2)2=1,wherer2=x2+y2,y>0.
(

r

R

)

6

+

(

z

T

/

2

)

2

=

1

,

where

r

2

=

x

2

+

y

2

,

y

>

0.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

x'=1α√x,y'=1α√y,z'=αz.
x

′

=

1

α

x

,

y

′

=

1

α

y

,

z

′

=

α

z

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, A phantom with different compression levels of (a) 4 cm, (b) 5 cm, (c) 6 cm, and (d) 7 cm. The 4-cm phantom served as the base of this set from which all the other phantoms were deformed.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/7_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

(xR')2+(yR')2+(zR')2=1,y>0.
(

x

R

′

)

2

+

(

y

R

′

)

2

+

(

z

R

′

)

2

=

1

,

y

>

0.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

(x'R)2+(y'R)2+(\|z'\|T/2)2.75=1,y'>0.
(

x

′

R

)

2

+

(

y

′

R

)

2

+

(

\|

z

′

\|

T

/

2

)

2.75

=

1

,

y

′

>

0.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

(xR')2=(x'R)2,(yR')2=(y'R)2,(zR')2=(\|z'\|T/2)2.75.
(

x

R

′

)

2

=

(

x

′

R

)

2

,

(

y

R

′

)

2

=

(

y

′

R

)

2

,

(

z

R

′

)

2

=

(

\|

z

′

\|

T

/

2

)

2.75

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, (b) A craniocaudal compressed phantom and (c) a mediolateral oblique compressed phantom. Both of them were deformed from (a) an uncompressed hemisphere breast phantom.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/8_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Phantom and System Validation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Geometry of the Monte Carlo simulation for breast imaging systems. A moving x-ray source with a synchronized selenium detector was modeled to image the phantom from different angles and emulate different breast imaging modalities: mammography (mammo), tomosynthesis (tomo), and breast computed tomography (BCT).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/9_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Dosimetric Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

D=dϵdm=dϵρdV,
D

=

d

ϵ

d

m

=

d

ϵ

ρ

d

V

,


where dϵ
d

ϵ
denotes the local deposited energy, _dm_ denotes the mass of the voxel, ρ
ρ
denotes the density of the material in the voxel, and _dV_ denoted the volume of the voxel. A 3D dose map representing the dose distribution in the breast phantom was generated after calculating the deposited dose in each voxel.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Mammographic Simulations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 11, One of the six masses ( solid box ) and microcalcification clusters ( dashed boxes ) observed in the simulated mammogram of a 4 cm, 60% density, 0.17-mm resolution phantom.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/10_1s20S1076633210006306.jpg)

![Figure 12, Synthetic mammograms of five randomly generated 4-cm-thick, 60%-dense phantoms with β values of (a) 2.13, (b) 2.48, (c) 2.83, (d) 3.18, (e) 3.53. Images were generated for a 28 kVp W anode beam and a direct flat-panel detector with parameters as specified in Methods.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/11_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 13, A region of interest (ROI) comparison of synthetic mammograms with real mammograms from Digital Database for Screening Mammography (DDSM) database. Five of them are ROIs from synthetic mammograms with a β value of (1) 2.83, (4) 2.13, (7) 2.48, (13) 3.53, (15) 3.18. The rest of the images are ROIs from real mammograms chosen from DDSM database.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/12_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 14, A collection of simulated mammograms of the same 0.51-mm resolution phantoms under different compression thickness: (a) 4 cm, (b) 5 cm, (c) 6 cm, and (d) 7 cm. The radius of the projected phantom decreases as the thickness increases to maintain breast volume. The internal pattern of the background mixture is also reformed accordingly. Some ring artifacts are visible at the outer periphery, due to the large voxel size that is less capable of depicting the large curvature.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/13_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## β value Validation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 15, The measured logarithmic NPS as a function of logarithmic spatial frequency. The slopes of the fitted lines represent the estimated β factors.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/14_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Volumetric Imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 16, (a) Synthetic mammogram is compared to slices taken from (b, c) tomosynthesis and (d, e) breast computed tomography reconstructions, showing (b, c) microcalcifications and (d, e) lesions.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/15_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Dosimetry

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 17, Lateral and front views of (a) 4-cm breast phantom and three-dimensional dose maps after (b) a mammography scan, (c) a tomosynthesis scan, and (d) a computed tomography scan. The color-bar represents the logarithmic deposited dose in the unit of mGy.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/16_1s20S1076633210006306.jpg)

![Figure 18, Lateral and front views of three-dimensional dose maps after tomosynthesis scans of a (a) 4-cm phantom, (b) 5-cm phantom, (c) 6-cm phantom, and (d) 7-cm phantom. The color-bar represents the logarithmic deposited dose in the unit of mGy.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAnthropomorphicBreastModelforBreastImagingSimulationandOptimization/17_1s20S1076633210006306.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Samei E., Eyler W., Baron L.: Effects of anatomical structure on signal detection. Handbook of Medical Imaging.2000.SPIE PressBellingham, WA


- 2\. Tamimi R.M., Cox D., Kraft P., et. al.: Breast cancer susceptibility loci and mammographic density. Breast Cancer Res 2008; 10: pp. R66.


- 3\. Armstrong K., Eisen A., Weber B.: Assessing the risk of breast cancer. N Engl J Med 2000; 342: pp. 564-571.


- 4\. Caldwell C.B., Yaffe M.J.: Development of an anthropomorphic breast phantom. Med Phys 1990; 17: pp. 273-280.


- 5\. Cinti M.N., Pani R., Garibaldi F., et. al.: Custom breast phantom for an accurate tumor SNR analysis. IEEE Trans Nucl Sci 2004; 51: pp. 198-204.


- 6\. Hoeschen C., Fill U., Zankl M., et. al.: A high-resolution voxel phantom of the breast for dose calculations in mammography. Radiat Prot Dosimetry 2005; 114: pp. 406-409.


- 7\. Zastrow E., Davis S.K., Lazebnik M., et. al.: Development of anatomically realistic numerical breast phantoms with accurate dielectric properties for modeling microwave interactions with the human breast. IEEE Trans Biomed Eng 2008; 55: pp. 2792-2800.


- 8\. Bliznakova K., Bliznakov Z., Bravou V., et. al.: A three-dimensional breast software phantom for mammography simulation. Phys Med Biol 2003; 48: pp. 3699-3719.


- 9\. Nappi J., Dean P.B., Nevalainen O., et. al.: Algorithmic 3D simulation of breast calcifications for digital mammography. Comput Methods Programs Biomed 2001; 66: pp. 115-124.


- 10\. Bakic P.R., Albert M., Brzakovic D., et. al.: Mammogram synthesis using a 3D simulation. II. Evaluation of synthetic mammogram texture. Med Phys 2002; 29: pp. 2140-2151.


- 11\. Bakic P.R., Albert M., Brzakovic D., et. al.: Mammogram synthesis using a 3D simulation. I. Breast tissue model and image acquisition simulation. Med Phys 2002; 29: pp. 2131-2139.


- 12\. Bakic P.R., Albert M., Brzakovic D., et. al.: Mammogram synthesis using a three-dimensional simulation. III. Modeling and evaluation of the breast ductal network. Med Phys 2003; 30: pp. 1914-1925.


- 13\.  Shorey JM. Stochastic simulations for the detection of objects in three dimensional volumes: applications in medical imaging and ocean acoustics. 2007.


- 14\. Egan R.L.: Breast embryology, anatomy and physiology. Breast imaging: diagnosis and morphology of breast diseases.1988.SaundersPhiladelphia, PA 30–58


- 15\. Burgess A.E., Jacobson F.L., Judy P.F.: Human observer detection experiments with mammograms and power-law noise. Med Phys 2001; 28: pp. 419-437.


- 16\. Gong X., Glick S.J., Liu B., et. al.: A computer simulation study comparing lesion detection accuracy with digital mammography, breast tomosynthesis, and cone-beam CT breast imaging. Med Phys 2006; 33: pp. 1041-1052.


- 17\. Bargeron C.B., Hutchins G.M., Moore G.W., et. al.: Distribution of the geometric parameters of human aortic bifurcations. Arteriosclerosis 1986; 6: pp. 109-113.


- 18\. Zamir M., Chee H.: Branching characteristics of human coronary arteries. Can J Physiol Pharmacol 1986; 64: pp. 661-668.


- 19\. Raabe O.G., Yeh H.C., Schum G.M., et. al.: Tracheobronchial geometry: human, dog, rat, hamster.1976.Lovelace Foundation Report LF-53 Lovelace FoundationAlbuquerque, NM


- 20\. Burgess A.E., Chakraborty S.: Producing lesions for hybrid mammograms: Extracted tumours and simulated microcalcifications. Proc SPIE Int Soc Optical Eng 1999; 3663: pp. 316-322.


- 21\. Saunders R.S., Samei E., Lo J.Y., et. al.: Can compression be reduced for breast tomosynthesis? Monte Carlo study on mass and microcalcification conspicuity in tomosynthesis. Radiology 2009; 251: pp. 673-682.


- 22\. Chawla A.S., Lo J.Y., Baker J.A., et. al.: Optimized image acquisition for breast tomosynthesis in projection and reconstruction space. Med Phys 2009; 36: pp. 4859-4869.


- 23\. Erdogan H., Fessler J.A.: Ordered subsets algorithms for transmission tomography. Phys Med Biol 1999; 44: pp. 2835-2851.


- 24\. Samei E., Flynn M.J.: An experimental comparison of detector performance for direct and indirect digital radiography systems. Med Phys 2003; 30: pp. 608-622.


- 25\. Saunders R.S., Samei E.: The effect of breast compression on mass conspicuity in digital mammography. Med Phys 2008; 35: pp. 4464-4473.