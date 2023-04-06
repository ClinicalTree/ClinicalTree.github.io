---
title: Interactive Deformation Registration of Endorectal Prostate MRI Using ITK Thin Plate Splines
author: [M. Rex Cheung MD PhD,Karthik Krishnan MS]
date: 2009-03-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 16, Issue 3 SOURCE CL_S_AcademicRadiologyVolume16Issue3 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Magnetic resonance imaging with an endorectal coil allows high-resolution imaging of prostate cancer and the surrounding normal organs. These anatomic details can be used to direct radiotherapy. However, organ deformation introduced by the endorectal coil makes it difficult to register magnetic resonance images for treatment planning. In this study, plug-ins for the volume visualization software VolView were implemented on the basis of algorithms from the National Library of Medicine's Insight Segmentation and Registration Toolkit (ITK).

## Materials and Methods

Magnetic resonance images of a phantom simulating human pelvic structures were obtained with and without the endorectal coil balloon inflated. The prostate not deformed by the endorectal balloon was registered to the deformed prostate using an ITK thin plate spline (TPS). This plug-in allows the use of crop planes to limit the deformable registration in the region of interest around the prostate. These crop planes restricted the support of the TPS to the area around the prostate, where most of the deformation occurred. The region outside the crop planes was anchored by grid points.

## Results

The TPS was more accurate in registering the local deformation of the prostate compared with a TPS variant, the elastic body spline. The TPS was also applied to register an in vivo T  2 -weighted endorectal magnetic resonance image. The intraprostatic tumor was accurately registered. This could potentially guide the boosting of intraprostatic targets. The source and target landmarks were placed graphically. This TPS plug-in allows the registration to be undone. The landmarks could be added, removed, and adjusted in real time and in three dimensions between repeated registrations.

## Conclusion

This interactive TPS plug-in allows a user to obtain a high level of accuracy satisfactory to a specific application efficiently. Because it is open-source software, the imaging community will be able to validate and improve the algorithm.

Magnetic resonance imaging (MRI) enhanced by an endorectal coil provides anatomic details of both prostate tumor and the surrounding normal tissues . Incorporating information from MRI studies into radiotherapy treatment may enable the direction of radiation to boost resistant areas, without increasing the dose to surrounding tissues. Various image registration methods have recently been studied to incorporate MRI information for radiation treatment planning and monitoring . Because the information needed for radiation treatment planning is concentrated in and around the prostate, the thin plate spline (TPS) approach appears to be an efficient and accurate way to perform deformable registration . Here, we report our implementation and assessment of plug-ins based on algorithms available in the open source Insight Segmentation and Registration Toolkit (ITK; National Library of Medicine, Bethesda, MD). In particular, we adapted a physics-based ITK TPS plug-in to run interactively in the volume visualization software VolView version 2.0 (Kitware, Inc, Clifton Park, NY) . The interactive nature of the plug-in allows landmarks to be added, removed, and adjusted in real time between repeated registrations. We evaluated the accuracy of the TPS in registering the local deformation of the prostate compared with a TPS variant, the elastic body spline (EBS). To illustrate potential clinical utility, we also applied the TPS to register an in vivo T  2 -weighted endorectal magnetic resonance image. The intraprostatic tumor was accurately registered. This could potentially guide the boosting of intraprostatic targets.

## Materials and methods

## Magnetic Resonance Images

A deformable pelvic phantom was custom made for our image registration study. Our earlier studies have been reported . Pertinent to this study, the magnetic resonance numbers for the prostate, seminal vesicles, bladder, and rectal wall were specified to simulate those of humans. The phantom was made of tissue-substitute materials by blending epoxy resins, urethanes, water-based polymers, and other proprietary materials (CIRS, Inc, Norfolk, VA). The University of Texas M.D. Anderson Cancer Center's institutional review board approved this retrospective study.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Registration Work Flow

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Adaptation of the ITK TPS as a VolView Plug-In

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

μ∇2u→(x→)+(μ+λ)∇\[∇∙u→(x→)\]=f→(x→),
μ

∇

2

u

→

(

x

→

)

+

(

μ

+

λ

)

∇

\[

∇

•

u

→

(

x

→

)

\]

=

f

→

(

x

→

)

,


where u→(x→)
u

→

(

x

→

)
is the displacement from the original position x→
x

→
; ∇2
∇

2
and ∇
∇
are the Lapacian and gradient operators, respectively; the force field f→(x→)=c→r(x→)
f

→

(

x

→

)

=

c

→

r

(

x

→

)
; position vector r→(x→)=∣∣x→∣∣=\[x21+x22+x23\]1/2
r

→

(

x

→

)

=

\|

x

→

\|

=

\[

x

1

2

+

x

2

2

+

x

3

2

\]

1

/

2
; μ and λ are the coefficients that describe the physical properties of the materials; and ∇∙u→(x→)
∇

•

u

→

(

x

→

)
is the divergence of u→(x→)
u

→

(

x

→

)
. The solution to Equation  1 given the force field is


u→(x→)=G(x→)c→,
u

→

(

x

→

)

=

G

(

x

→

)

c

→

,


where


G(x→)=\[αr(x→)I−3x→x→T\]r(x→).
G

(

x

→

)

=

\[

α

r

(

x

→

)

I

−

3

x

→

x

→

T

\]

r

(

x

→

)

.


The Poisson ratio υ = λ/\[2(λ + μ)\], α = 12(1 − υ) − 1, and _I_ is the identity matrix. The form of G(x→)
G

(

x

→

)
for the ITK TPS implementation used in this study is as follows:


G(x→)=Ir(x→).
G

(

x

→

)

=

I

r

(

x

→

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Variants of the TPS

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

G(x)=r(x)2log\[r(x)\]×I;
G

(

x

)

=

r

(

x

)

2

log

\[

r

(

x

)

\]

×

I

;


the EBS,


G(x)={\[12×(1−v)−1\]r\[x\]2×I−3xxT}×r(x),
G

(

x

)

=

{

\[

12

×

(

1

−

v

)

−

1

\]

r

\[

x

\]

2

×

I

−

3

x

x

T

}

×

r

(

x

)

,


where ν is the Poisson ratio; the elastic body reciprocal spline,


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

G(x)={\[8×(1−v)−1\]r\[x\]×I−3xxT/r(x)};
G

(

x

)

=

{

\[

8

×

(

1

−

v

)

−

1

\]

r

\[

x

\]

×

I

−

3

x

x

T

/

r

(

x

)

}

;


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

G(x)=r(x)3×I.
G

(

x

)

=

r

(

x

)

3

×

I

.


These variants are based on variants plugged into the solution of _G_ ( _x_ ) . In this study, we investigated the accuracy of the TPS and the ITK EBS for the deformable registration of endorectal magnetic resonance images of the prostate.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Landmark Placement

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## TPS Deformable Manual Alignment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, (a) Slice slowing landmark pairs placed by the user to construct the thin plate spline (TPS) transform. The red landmarks were placed on the endorectal magnetic resonance image. The green landmarks were placed on the planning image. The planning image was deformed using the resulting TPS transform and overlaid on the endorectal image to show the accuracy of the registration. If the results are dissatisfactory, a user can adjust the landmark pairs and rerun the registration to obtain the overlay again. (b) Deformation field resulting from the TPS transform. The segmentation of the planning image was warped using the inverse field and overlaid on a slice of the balloon-deflated image. The maximum deformation of 7.5 mm occurred at the prostate-rectum interface.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InteractiveDeformationRegistrationofEndorectalProstateMRIUsingITKThinPlateSplines/0_1s20S1076633208005692.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, The deformed grid as a result of the thin plate spline. Target landmarks are shown in red . Source landmarks are shown in green .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InteractiveDeformationRegistrationofEndorectalProstateMRIUsingITKThinPlateSplines/1_1s20S1076633208005692.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison of TPS Variants

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The deformed grid as a result of the elastic body spline. Target landmarks are shown in red . Source landmarks are shown in green .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InteractiveDeformationRegistrationofEndorectalProstateMRIUsingITKThinPlateSplines/2_1s20S1076633208005692.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, (a) Thin plate spline and (b) elastic body spline kernels obtained by displacing one of the landmark correspondence pairs.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InteractiveDeformationRegistrationofEndorectalProstateMRIUsingITKThinPlateSplines/3_1s20S1076633208005692.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Example

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Axial image from a T 2 -weighted prostate magnetic resonance imaging study with an endorectal probe (a) and without the probe (b) . (c) Thin plate spline registration of the image in (a) . Source ( green ) and target ( red ) landmarks are shown.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InteractiveDeformationRegistrationofEndorectalProstateMRIUsingITKThinPlateSplines/4_1s20S1076633208005692.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, (a) Checkerboard display of the registered magnetic resonance image and the target image. (b) Prostate and tumor contours prior to and after registration, overlaid on the target image. The green contours correspond to the initial positions of the prostate (thick contour) and the tumor (thin contour) prior to registration. The blue contours correspond to expected positions of the prostate (thick contour) and the tumor (thin contour) after registration.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/InteractiveDeformationRegistrationofEndorectalProstateMRIUsingITKThinPlateSplines/5_1s20S1076633208005692.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Future Work

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Villeirs G.M., Verstraete K.L., De Neve W.J., De Meerleer G.O.: Magnetic resonance imaging anatomy of the prostate and periprostatic area: a guide for radiotherapists. Radiother Oncol 2005; 76: pp. 99-106.


- 2\. McLaughlin P.W., Troyer S., Berri S., et. al.: Functional anatomy of the prostate: implications for treatment planning. Int J Radiat Oncol Biol Phys 2005; 63: pp. 479-491.


- 3\. Dean D., Herbener T.E.: Cross-sectional human anatomy.2000.Lippincott Williams & WilkinsPhiladelphia, PA 191


- 4\. van Lin E.N., Futterer J.J., Heijmink S.W., et. al.: IMRT boost dose planning on dominant intraprostatic lesions: gold marker-based three-dimensional fusion of CT with dynamic contrast-enhanced and 1H-spectroscopic MRI. Int J Radiat Oncol Biol Phys 2006; 65: pp. 291-303.


- 5\. Alterovitz R., Goldberg K., Pouliot J., et. al.: Registration of MR prostate images with biomechanical modeling and nonlinear parameter estimation. Med Phys 2006; 33: pp. 446-454.


- 6\. Hensel J.M., Ménard C., Chung P.W., et. al.: Development of multiorgan finite element-based prostate deformation model enabling registration of endorectal coil magnetic resonance imaging for radiotherapy planning. Int J Radiat Oncol Biol Phys 2007; 68: pp. 1522-1528.


- 7\. Schreibmann E., Xing L.: Narrow band deformable registration of prostate magnetic resonance imaging, magnetic resonance spectroscopic imaging, and computed tomography studies. Int J Radiat Oncol Biol Phys 2005; 62: pp. 595-605.


- 8\. Zhong H., Peters T., Siebers J.V.: FEM-based evaluation of deformable image registration for radiation therapy. Phys Med Biol 2007; 52: pp. 4721-4738.


- 9\. Davis M.H., Khotanzad A., Flamig D.P., Harms S.E.: A physics-based coordinate transformation for 3-D image matching. IEEE Trans Med Imaging 1997; 16: pp. 317-328.


- 10\. Bookstein F.L.: Principal warps: thin-plate splines and the decomposition of deformations. IEEE Trans Pattern Anal Mach Intell 1989; 11: pp. 567-585.


- 11\. Lian J., Xing L., Hunjan S., et. al.: Mapping of the prostate in endorectal coil-based MRI/MRSI and CT: a deformable registration and validation study. Med Phys 2004; 31: pp. 3087-3094.


- 12\. Fei B., Duerk J.L., Sodee D.B., Wilson D.L.: Semiautomatic nonrigid registration for the prostate and pelvic MR volumes. Acad Radiol 2005; 12: pp. 815-824.


- 13\. Schaly B., Bauman G.S., Battista J.J., Van Dyk J.: Validation of contour-driven thin-plate splines for tracking fraction-to-fraction changes in anatomy and radiation therapy dose mapping. Phys Med Biol 2005; 50: pp. 459-475.


- 14\. Martin K., Ibáñez L., Avila L., Barré S., Kaspersen J.H.: Integrating segmentation methods from the Insight Toolkit into a visualization application. Med Image Anal 2005; 9: pp. 579-593.


- 15\. Wang H., Dong L., Lii M.F., et. al.: Implementation and validation of a three-dimensional deformable registration algorithm for targeted prostate cancer radiotherapy. Int J Radiat Oncol Biol Phys 2005; 61: pp. 725-735.


- 16\. Prata S.: C++ primer plus.5th ed.2005.SamsIndianapolis, IN


- 17\. Sprengel R., Rohr D., Stiehl H.: Thin-plate spline approximation for image registration.1996.Presented at: 18th International Conference of the IEEE Engineering in Medicine and Biology Society


- 18\. Horn B.K.P.: Closed-form solution of absolute orientation using unit quaternions. J Optical Soc Am 1987; 4: pp. 629-642.


- 19\. Cheung R., Tucker S.L., Lee A.K., et. al.: Dose-response characteristics of low- and intermediate-risk prostate cancer treated with external beam radiotherapy. Int J Radiat Oncol Biol Phys 2005; 61: pp. 993-1002.


- 20\. Cheung R., Tucker S.L., Dong L., Kuban D.: Dose-response for biochemical control among high-risk prostate cancer patients after external beam radiotherapy. Int J Radiat Oncol Biol Phys 2003; 56: pp. 1234-1240.


- 21\. Cheung R., Tucker S.L., Ye J.S., et. al.: Characterization of rectal normal tissue complication probability after high-dose external beam radiotherapy for prostate cancer. Int J Radiat Oncol Biol Phys 2004; 58: pp. 1513-1519.


- 22\. Cheung R., Tucker S.L., Dong L., et. al.: Identification of the bladder dose and volume factors to control late urinary toxicity after external beam radiotherapy for prostate cancer. Int J Radiat Oncol Biol Phys 2007; 67: pp. 1059-1065.


- 23\. Pickett B., Kurhanewicz j, Coakley F., Shinohara K., Fein B., Roach M.I.: Use of MRI and spectroscopy in evaluation of external beam radiotherapy for prostate cancer. Int J Radiat Oncol Biol Phys 2004; 60: pp. 1047-1055.


- 24\. Li C., Liengsawangwong R., Choi H., Cheung R.: Using a priori structural information from magnetic resonance imaging to investigate the feasibility of prostate diffuse optical tomography and spectroscopy: a simulation study. Med Phys 2007; 34: pp. 266-274.


- 25\. Yushkevich P.A., Piven J., Cody H., Ho S., Gee J.C., Gerig G.: User-guided active contour segmentation of anatomical structures: significantly improved efficiency and reliability. Neuroimage 2006; 31: pp. 1116-1128.