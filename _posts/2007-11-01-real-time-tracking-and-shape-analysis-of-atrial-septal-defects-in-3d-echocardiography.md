---
title: Real-Time Tracking and Shape Analysis of Atrial Septal Defects in 3D Echocardiography
author: [Marius George Linguraru,Alexre Kabla,Gerald R. Marx,Pedro J. del Nido,Robert D. Howe]
date: 2007-11-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 11 SOURCE CL_S_AcademicRadiologyVolume14Issue11 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Real-time cardiac ultrasound (US) allows monitoring the heart motion during intracardiac beating heart procedures. Our application assists pediatric atrial septal defect (ASD) closure techniques using real-time 3D US guidance and rigid instruments. ASD tracking is also an important tool for facilitating systematic clinical studies of the dynamic behavior of the intra-atrial communication. One major image processing challenge is associated with the required processing of information at high frame rate, especially given the low image quality.

## Materials and Methods

We present an optimization scheme for a block flow technique, which combines the probability-based velocity computation for an entire block (a 3D volume centered on the ASD) with cyclic template matching. The adapted similarity imposes constraints both locally (from frame to frame) to conserve energy, and globally (from a reference template) to minimize cumulative errors. The algorithm is optimized for fast and reliable results. For tests, we use three intra-operational 4D ultrasound sequences of clinical infant beating hearts with ASD.

## Results

Computing velocity at the block level with an optimized scheme, our technique tracks ASD motion at a frequency of 60 frames/s on clinical 4D datasets. Results are stable and accurate for changes in resolution and block size. In particular, we show robust real-time tracking and preliminary segmentation results of the ASD shape, size and orientation as a function of time.

## Conclusions

We present an optimized block flow technique for real-time tracking of ASD to assist in minimally invasive beating heart surgery. Our method proposes the standard use of references for processing repetitive data. This paper represents, to our knowledge, the first study on the dynamic morphology of ASD that takes into account the angular effect introduced by the slanted position of the intra-atrial communication with respect to the US probe.

Real-time cardiac ultrasound (US) allows monitoring the heart motion during intracardiac beating heart procedures. Among the congenital heart malformations, secundum-type atrial septal defects (ASD) have been reported to account for up to 15% of cases ( ). ASD represent openings in the septum between the atria, which decrease the efficiency of heart pumping. Although the surgical intervention for ASD closure is well established and has excellent prognosis, it is performed under cardiopulmonary bypass, which has widely acknowledged harmful effects. Minimally invasive, image-guided beating-heart ASD closure will avoid using cardiopulmonary bypass and improve the patient rehabilitation.

There are two alternatives for minimally invasive ASD closure procedures: one using a catheter-based closure, usually under contrast-enhanced fluoroscopy ( ), and another using rigid instruments through the chest wall to place a patch over the ASD, demonstrated in animals ( ). Although clinically available, the catheter-based procedure has major disadvantages: it can be used only on a fraction of ASD ( ), it excludes procedures on small children ( ), and the delivered x-ray dose is usually high. Animal and pediatric studies showed the feasibility of ASD closures using rigid instruments and highlighted their limitations ( ). A major challenge to successful beating-heart surgical interventions remains the reliable visualization of structures within the heart ( ). Our application shows the position and morphology of ASD in real-time to support the development of US-guided intracardiac interventions using rigid instruments.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633207X00928/S1076633207004011/gr1.jpg?Signature=fTpwVrwA0nO4qwawQPi46QIezecJe44M%7EKAuowre9a55-A%7E3gpU8rfKDOn0CkryzlmWEYdUm3ofiX7-xrMdz60zaCIE-g6wsxIyYMYVvWF5Q0OVWHh8x39JrX%7Ebj%7EMygttJsyXRrvdAHlIq6EAry%7EcpBoZmMW1Dl3iTmgjh3Ugw_&Expires=1669521893&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Three-dimensional (3D) ultrasound (US) image of an atrial septal defect (ASD). The US probe is placed on the exterior wall of the right atrium and pointed towards the left atrium. The image on the left shows the entire 3D US volume, whereas on the right we present a magnified view of the ASD. The round patch must cover the entire ASD surface.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Block Flow

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ref¯¯¯¯¯=ref/μref;
r

e

f

¯

=

r

e

f

/

μ

r

e

f

;


absref¯¯¯¯¯¯¯¯¯¯=absref/μabsref;
a

b

s

r

e

f

¯

=

a

b

s

r

e

f

/

μ

a

b

s

r

e

f

;


tar¯¯¯¯¯=tar/μtar;
t

a

r

¯

=

t

a

r

/

μ

t

a

r

;


newref¯¯¯¯¯¯¯¯¯¯¯=(ref¯¯¯¯¯+absref¯¯¯¯¯¯¯¯¯¯)/2;
n

e

w

r

e

f

¯

=

(

r

e

f

¯

+

a

b

s

r

e

f

¯

)

/

2

;


The velocity or displacement of the block _V  b_ is computed as a probability distribution function _R_ , where _n_ is the number of voxels in the 3D block, _τ_ a normalizing weight, and _md_ the maximum displacement or search space ( ). The similarity between frames and between current frame and template is computed from adapted maximum likelihood ( ). The energy function _E_ accounts for both the Rayleigh distribution of the noise model and logarithmic compression in US images ( ).


E(newref¯¯¯¯¯¯¯¯¯¯¯,tar¯¯¯¯¯)=1n∑i\[lnnewref¯¯¯¯¯¯¯¯¯¯¯i−lntar¯¯¯¯¯i−ln(e2(lnnewref¯¯¯¯¯¯¯¯¯¯¯i−lntari¯¯¯¯¯¯)+1)\];
E

(

n

e

w

r

e

f

¯

,

t

a

r

¯

)

=

1

n

∑

i

\[

ln

n

e

w

r

e

f

¯

i

−

ln

t

a

r

¯

i

−

ln

⁡

(

e

2

(

ln

n

e

w

r

e

f

¯

i

−

ln

t

a

r

i

¯

)

+

1

)

\]

;


R(u,v,w)=1τ(exp(−E(newref¯¯¯¯¯¯¯¯¯¯¯,tar¯¯¯¯¯)−max(E(newref¯¯¯¯¯¯¯¯¯¯¯,tar¯¯¯¯¯))2md3)−1);
R

(

u

,

v

,

w

)

=

1

τ

(

exp

⁡

(

−

E

(

n

e

w

r

e

f

¯

,

t

a

r

¯

)

−

max

⁢

⁡

(

E

(

n

e

w

r

e

f

¯

,

t

a

r

¯

)

)

2

m

d

3

)

−

1

)

;


Vb=(∑u,v,wR(u,v,w)u,∑u,v,wR(u,v,w)v,∑u,v,wR(u,v,w)w);
V

b

=

(

∑

u

,

v

,

w

R

(

u

,

v

,

w

)

u

,

⁢

∑

u

,

v

,

w

R

(

u

,

v

,

w

)

v

,

∑

u

,

v

,

w

R

(

u

,

v

,

w

)

w

)

;


Minimizing the energy _E_ is equivalent to minimizing the maximum error in similarity between the target block _tar_ and _newref_ , which embeds information from both _ref_ and _absref_ . _E_ becomes a value of dual match and obstructs velocities _u_ , _v_ and _w_ to grow in the directions of blocks that are not similar to both the previous frame and the absolute reference.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

abserr=E(absref¯¯¯¯¯¯¯¯¯¯,tar¯¯¯¯¯);
a

b

s

e

rr

=

E

(

a

b

s

r

e

f

¯

,

t

a

r

¯

)

;


conserr=E(ref¯¯¯¯¯,tar¯¯¯¯¯);
c

o

n

s

e

r

r

=

E

(

r

e

f

¯

,

t

a

r

¯

)

;


Both error measures should vary with the heart motion and the change in shape of ASD. For a correct tracking, the errors would become minimal at the same moment of the heart cycle. The errors are in percentage and normalized between 0 and 100, in which an error of 0 corresponds to the perfect match.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Optimization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

E(newref¯¯¯¯¯¯¯¯¯¯¯,tar¯¯¯¯¯)=1n∑if(lnnewref¯¯¯¯¯¯¯¯¯¯¯itari¯¯¯¯¯¯);
E

(

n

e

w

r

e

f

¯

,

t

a

r

¯

)

=

1

n

∑

i

f

(

ln

⁡

n

e

w

r

e

f

¯

i

t

a

r

i

¯

)

;


with


f(x)=x−ln(e2x+1);
f

(

x

)

=

x

−

ln

⁡

(

e

2

x

+

1

)

;


The repetitive evaluations of the logarithmic and exponential functions represent the most time-consuming operations. This process can be accelerated using the following scheme: _f_ is an even function of _x_ and is asymptotically equal _to f_ ( _x_ ) _∼\- x_ \| for large values of \| _x_ \|; the relative error ( _f_ ( _x_ )+\| _x_ \|)/\| _x_ \| is lower than 1% for \| _x_ \|>2\. Therefore we precomputed and stored the values of _f_ for _x_ ∈(0;2) and used the asymptotical expression for larger values, which ensures that arbitrarily large values of _x_ would be accurately taken into account.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Atrial septal defect (ASD) segmentation: (a) a two-dimensional slice of the three-dimensional image in (x,z) coordinates, normal to the ASD; the frame represents the typical block size and location used for the segmentation; (b) the neighborhood of ASD is extracted using the tracking information; a family of vertical slices defined by the angle θ between the normal to the plane and the x axis are used to detect the boundary of the hole; (c) a typical vertical section after thresholding; the computed location of the hole boundary allows the reconstruction of the ASD shape parameterized by the angle θ.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/0_1s20S1076633207004011.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Tracking

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Tracking results in three-dimensional (3D) volume. From left to right, the columns show the entire US volume with the 3D block delineated at frames 1, 25, and 50.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/1_1s20S1076633207004011.jpg)

![Figure 4, Clinical atrial septal defect tracking. From left to right and top to bottom, the columns show three-dimensional blocks visualized from right atrium to left atrium every two frames between frames 1 and 15, corresponding to one heart cycle (the frame number is marked on the upper left corner).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/2_1s20S1076633207004011.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, The evolution in time of the absolute and conservation errors in clinical experiments. Although data are ungated, each error measure has two synchronized peaks, which are temporally related to each other, as shown by the two arrows.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/3_1s20S1076633207004011.jpg)

![Figure 6, The three-dimensional motion of the block for a typical clinical case for one heart cycle. Temporal frames start at dark shades of gray and end at light gray. At the end of the heart cycle, the block is found at the same position as at the start.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/4_1s20S1076633207004011.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Stability and Efficiency

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Vertical motion of the atrial septal defect for different block sizes and different resolutions. Data are obtained over 20 repetitions of a unique full heart cycle in order to test the stability of tracking.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/5_1s20S1076633207004011.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ASD Segmentation and Dynamic Morphology

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, The four-dimensional segmentation of a typical atrial septal defect (ASD) case during one heart cycle: (a) the ASD contour is shown from top view at three different times, corresponding to the smallest, intermediate, and maximal size; (b) the ASD contour is shown from side view at the same times as in (a) ; (c) the plot of the evolution of the ASD surface area as a function of time during a heart cycle; (d) the plot of the evolution of the ASD tilt angle as a function of time during a heart cycle.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/6_1s20S1076633207004011.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, The four-dimensional atrial septal defect dynamic morphology during one heart cycle. Temporal frames start at dark shades of gray and end at light gray.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/RealTimeTrackingandShapeAnalysisofAtrialSeptalDefectsin3DEchocardiography/7_1s20S1076633207004011.jpg)

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

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Barron J.L., Fleet D.J., Beauchemin S.: Performance of optical flow techniques. Int J Comp Vision 1994; 12: pp. 43-77.


- 2\. Faella H.J., Sciegata A.M., Alonso J.L., et. al.: ASD closure with the Amplatzer device. J Intervent Cardiol 2003; 16: pp. 393-397.


- 3\. Papadopoulou D.I., Yakoumakis E.N., Makri T.K., et. al.: Assessment of patient radiation roses during transcatheter closure of ventricular and atrial septal defects with Amplatzer devices. Catheter Cardiovasc Interventions 2005; 65: pp. 434-441.


- 4\. Suematsu Y., Martinez J.F., Wolf B.K., et. al.: Three-dimensional echo-guided beating heart surgery without cardiopulmonary bypass: atrial septal defect closure in a swine model. J Thoracic Cardiovasc Surg 2005; 130: pp. 1348-1357.


- 5\. Podnar T., Martanovi P., Gavora P., et. al.: Morphological variations of secundum-type atrial septal defects: feasibility for percutaneous closure using amplatzer septal occluders. Catheter Cardiovasc Interventions 2001; 53: pp. 386-391.


- 6\. Patel A., Cao Q.L., Koenig P.R., et. al.: Intracardiac echocardiography to guide closure of atrial septal defects in children less than 15 kilograms. Catheter Cardiovasc Interventions 2006; 68: pp. 287-291.


- 7\. Downing S.W., Herzog W.R., McElroy M.C., et. al.: Feasibility of off-pump ASD closure using real-time 3-D echocardiography. Heart Surg Forum 2002; 5: pp. 96-99.


- 8\. Cannon J.W., Stoll J.A., Salgo I.S., et. al.: Real time 3-dimensional ultrasound for guiding surgical tasks. Comp Aided Surg 2003; 8: pp. 82-90.


- 9\. Suematsu Y., Marx G.R., Stoll J.A., et. al.: Three-dimensional echocardiography-guided beating-heart surgery without cardiopulmonary bypass: a feasibility study. J Thoracic Cardiovasc Surg 2004; 128: pp. 579-587.


- 10\. Handke M., Schäfer D., Müller G., et. al.: Dynamic changes of atrial septal defect area: new insights by three-dimensional volume-rendered echocardiography with high temporal resolution. Eur J Echocardiogr 2001; 2: pp. 46-51.


- 11\. Maeno Y.V., Benson L.N., McLaughlin P.R., et. al.: Dynamic morphology of the secundum atrial defect evaluated by three dimensional septal transesophageal echocardiography. Heart 2000; 83: pp. 673-677.


- 12\. Fenster A., Downey D.B., Cardinal H.N.: Three-dimensional ultrasound imaging. Phys Med Biol 2001; 46: pp. R67-R99.


- 13\. Duan Q., Angelini E.C., Herz S.L., et. al.: Evaluation of optical flow algorithms for tracking endocardial surfaces on three-dimensional ultrasound data. SPIE Int Symp Med Imaging 2005; 5750: pp. 159-169.


- 14\. Singh A., Allen P.: Image-flow computation: an estimation-theoretic framework and a unified perspective. CVGIP Image Understanding 1992; 65: pp. 152-177.


- 15\. Boukerroui D., Noble J.A., Brady M.: Velocity estimation in ultrasound images: a block matching approach. Inform Process Med Imaging (IPMI) 2003; 2732: pp. 586-598.


- 16\. Cohen B., Dinstein I.: New maximum likelihood motion estimation schemes for noisy ultrasound images. Pattn Recognit 2002; 35: pp. 455-463.


- 17\. Paragios N.: A level set approach for shape-driven segmentation and tracking of the left ventricle. IEEE Trans Med Imaging 2003; 22: pp. 773-786.


- 18\. Chen X., Xie H., Erkamp R., et. al.: O’Donnell: 3-D correlation-based speckle tracking. Ultrason Imaging 2005; 27: pp. 21-36.


- 19\. Montagnat J., Sermesant M., Delingette H., et. al.: Ayache: anisotropic filtering for model-based segmentation of 4D cylindrical echocardiographic images. Patt Recognit Lett 2003; 24: pp. 815-828.


- 20\. Papademetris X., Sinusas A.J., Dione D.P., et. al.: Estimation of 3D left ventricular deformation from echocardiography. Med Image Anal 2001; 5: pp. 17-28.


- 21\. Morsy A.A., von Ramm O.T.: FLASH correlation: a new method for 3-D ultrasound tissue motion tracking and blood velocity estimation. IEEE Trans Ultrasonics Ferroelectrics Freq Contr 1999; 46: pp. 728-736.


- 22\. Ourselin S., Roche A., Prima S., et. al.: Block matching: a general framework to improve robustness of rigid registration of medical images.2000.SpringerNew York:pp. 557-566.


- 23\. Novotny P.M., Stoll J.A., Vasilyev N.V., et. al.: GPU Based real-time instrument tracking with three dimensional ultrasound.2006.SpringerNew York:pp. 58-65.


- 24\. Thijssen J.M.: Ultrasonic speckle formation, analysis and processing applied to tissue characterization. Patt Recognit Lett 2003; 24: pp. 659-675.


- 25\.  Noble JA, Boukerroui D. Ultrasound image segmentation: a survey. IEEE Trans Med Imaging 2066; 25:987–1010.


- 26\. Deriche R.: Using Canny’s criteria to derive a recursively implemented optimal edge detector. Int J Comp Vision 1987; 1: pp. 167-187.


- 27\. Linguraru M.G., Vasilyev N.V., del Nido P.J., et. al.: Atrial septal defect tracking in 3D cardiac ultrasound.2006.SpringerNew York:pp. 596-603.


- 28\. Linguraru M.G., Howe R.D.: Texture-based segmentation of instruments in 3D ultrasound.Reinhardt J.M.Pluim J.P.W.2006. 61443J1–61443JI9


- 29\. Roche A., Malandain G., Ayache N.: Unifying maximum likelihood approaches in medical image registration. Int J Imaging Syst Technol Special 2000; 11: pp. 71-80.