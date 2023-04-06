---
title: An Automatic Method for Renal Cortex Segmentation on CT Images
author: [Xinjian Chen PhD,Ronald M. Summers MD PhD,Monique Cho MD,Ulas Bagci PhD,Jianhua Yao PhD]
date: 2012-05-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 5 SOURCE CL_S_AcademicRadiologyVolume19Issue5 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aims of this study were to develop and validate an automated method to segment the renal cortex on contrast-enhanced abdominal computed tomographic images from kidney donors and to track cortex volume change after donation.

## Materials and Methods

A three-dimensional fully automated renal cortex segmentation method was developed and validated on 37 arterial phase computed tomographic data sets (27 patients, 10 of whom underwent two computed tomographic scans before and after nephrectomy) using leave-one-out strategy. Two expert interpreters manually segmented the cortex slice by slice, and linear regression analysis and Bland-Altman plots were used to compare automated and manual segmentation. The true-positive and false-positive volume fractions were also calculated to evaluate the accuracy of the proposed method. Cortex volume changes in 10 subjects were also calculated.

## Results

The linear regression analysis results showed that the automated and manual segmentation methods had strong correlations, with Pearson's correlations of 0.9529, 0.9309, 0.9283, and 0.9124 between intraobserver variation, interobserver variation, automated and user 1, and automated and user 2, respectively ( _P_ < .001 for all analyses). The Bland-Altman plots for cortex segmentation also showed that the automated and manual methods had agreeable segmentation. The mean volume increase of the cortex for the 10 subjects was 35.1 ± 13.2% ( _P_ < .01 by paired _t_ test). The overall true-positive and false-positive volume fractions for cortex segmentation were 90.15 ± 3.11% and 0.85 ± 0.05%. With the proposed automated method, the time for cortex segmentation was reduced from 20 minutes for manual segmentation to 2 minutes.

## Conclusions

The proposed method was accurate and efficient and can replace the current subjective and time-consuming manual procedure. The computer measurement confirms the volume of renal cortex increases after kidney donation.

The renal cortex, the outer kidney layer consisting of renal corpuscles and convoluted tubules, has distinct morphology and function from the inner renal medulla. Because glomerular filtration, an important clinical assessment of renal function, is the main function of the renal cortex, there has been considerable interest in accurately assessing renal cortex size and volume. The current method for renal cortex segmentation in clinics, however, is mainly operated manually , which is subjective and tedious. There have been several prior investigations of renal cortex segmentation on computed tomographic (CT) and magnetic resonance images, including both semiautomatic and fully automatic methods. However, most of these studies considered the renal cortex and renal column as one tissue type, although they are anatomically different. In this paper, we propose a method to precisely and automatically segment the renal cortex. To the best of our knowledge, this study is the first work that aims to automatically separate the renal cortex and renal column in renal segmentation.

In kidney transplantation, the ability to accurately and reliably measure renal volume may give clinicians a better understanding of the aftereffects of kidney donation and therefore improve the kidney donor selection process. Limited but available data suggest that larger renal volume is associated with better renal graft function in recipients 1 year after transplantation . A few studies have estimated kidney volume change after donation by using image findings (such as computed tomography, magnetic resonance imaging, and ultrasound). In this investigation, we also tracked cortex volume change for the remaining kidneys of the donors. As for the volume change in the renal cortex, to the best of our knowledge, we are the first group to measure change after donation.

## Materials and methods

## Donors

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## CT Imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Manual Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Automatic Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Flowchart of the proposed cortex segmentation system. AAM, active appearance model; GC, graph cut; LW, live wire; OAAM, oriented active appearance model; 3D, three-dimensional.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAutomaticMethodforRenalCortexSegmentationonCTImages/0_1s20S1076633212000402.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Model building and training

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Landmark specification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## AAM construction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

M=(M1,M2,…,Mn).
M

=

(

M

1

,

M

2

,

…

,

M

n

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Parameter estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Kidney initialization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Localization of top and bottom slices

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## OAAM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


  - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Etotal=α1×EAAM+α2×ELW.
E

total

=

α

1

×

E

AAM

+

α

2

×

E

LW

.


- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 6.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 7.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 8.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Renal cortex segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Shape-constrained GC

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

En(f)=∑p∈PRp(fp)+∑p∈P,q∈NpBp,q(fp,fq),
En

(

f

)

=

∑

p

∈

P

R

p

(

f

p

)

+

∑

p

∈

P

,

q

∈

N

p

B

p

,

q

(

f

p

,

f

q

)

,


where _N__p_ is the set of pixels in the neighborhood of _p_ , _R__p_ ( _f__p_ ) is the cost of assigning label fp∈L
f

p

∈

L
to _p_ , and _B__p_ , _q_ ( _f__p_ , _f__q_ ) is the cost of assigning labels _f__p_ , fp∈L
f

p

∈

L
to _p_ and _q_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

En(f)=∑p∈P\[α×Dp(fp)+β×Sp(fp,xo)\]+∑p∈P,q∈Npγ×Bp,q(fp,fq),
En

(

f

)

=

∑

p

∈

P

\[

α

×

D

p

(

f

p

)

+

β

×

S

p

(

f

p

,

x

o

)

\]

+

∑

p

∈

P

,

q

∈

N

p

γ

×

B

p

,

q

(

f

p

,

f

q

)

,


where α, β, and γ are the weights for the data term, shape term _S__p_ , and boundary term, respectively, satisfying α + β + γ = 1. These components are defined as follows:


Dp(fp)={−lnP(Ip\|O)iffp=objectlabel−lnP(Ip\|B)iffp=backgroundlabel,
D

p

(

f

p

)

=

{

−

ln

P

(

I

p

\|

O

)

if

f

p

=

object

label

−

ln

P

(

I

p

\|

B

)

if

f

p

=

background

label

,


Bp,q(fp,fq)=exp\[−(Ip−Iq)22σ2\]×1d(p,q)×δ(fp,fq),
B

p

,

q

(

f

p

,

f

q

)

=

exp

\[

−

(

I

p

−

I

q

)

2

2

σ

2

\]

×

1

d

(

p

,

q

)

×

δ

(

f

p

,

f

q

)

,


and


δ(fp,fq)={10iffp≠fqotherwise,
δ

(

f

p

,

f

q

)

=

{

1

if

f

p

≠

f

q

0

otherwise

,


where _I__p_ is the intensity of pixel _p_ ; object label is the label of the object (foreground); _P_ ( _I__p_ O ) and _P_ ( _I__p_ B ) are the probability of intensity of pixel _p_ belonging to object and background, respectively, which are estimated from object and background intensity histograms during the training phase (details given below); _d_ ( _p_ , _q_ ) is the Euclidian distance between pixels _p_ and _q_ ; and σ is the standard deviation of the intensity differences of neighboring voxels along the boundary.

Sp(fp,xo)=1−exp\[−dfp(p,xo)ro\]
S

p

(

f

p

,

x

o

)

=

1

−

exp

\[

−

d

f

p

(

p

,

x

o

)

r

o

\]

and

dfp(p,xo)={d(p,xo)d(p,x¯o)iffp=sourcelabelotherwise,
d

f

p

(

p

,

x

o

)

=

{

d

(

p

,

x

o

)

if

f

p

=

source

label

d

(

p

,

x

¯

o

)

otherwise

,

where _d_ ( _p_ , **x**_O_ ) is the distance from pixel _p_ to the set of pixels that constitute the interior of the current shape **x**_o_ of object _O_ (note that if _p_ is in the interior of **x**_o_ , then _d_ \[ _p_ , **x**_O_ \] = 0); d(p,x¯o)
d

(

p

,

x

¯

o

)
is the distance from voxel _p_ to the complementary of the shape _x__o_ ; and _r__O_ is the radius of the sphere that roughly encloses **x**_o_ . The linear time method of reference was used in this study for computing this distance.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Renal Cortex Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analyses and Segmentation Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TPVF=\|CTP\|\|Ctd\|,
TPVF

=

\|

C

TP

\|

\|

C

td

\|

,


and


FPVF=\|CFP\|\|Ud−Ctd\|,
FPVF

=

\|

C

FP

\|

\|

U

d

−

C

td

\|

,


where _C_ TP is the set of voxels in the true-positive delineation, _C_ td is the set of voxels in the ground truth, _C_ FP is the set of voxels falsely identified, _U_ d is assumed to be a binary scene with all voxels in the scene domain, and \|·\| denotes volume.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Correlations between Manual and Automatic Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Linear regression analysis and Bland-Altman plots for intraobserver and interobserver assessment of manual segmentation results.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAutomaticMethodforRenalCortexSegmentationonCTImages/1_1s20S1076633212000402.jpg)

![Figure 3, Linear regression analysis and Bland-Altman plots for automated and manual segmentation results.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAutomaticMethodforRenalCortexSegmentationonCTImages/2_1s20S1076633212000402.jpg)

![Figure 4, Examples of segmentation results for cortex segmentation. The top and bottom rows show the corresponding slices before and after nephrectomy, respectively. (a) One slice image before nephrectomy, (b) user 1's segmentation results on (a) , (c) user 2's segmentation results on (a) , (d) automated segmentation results on (a) , (e) corresponding slice image after nephrectomy of (a) , (f) user 1's segmentation results on (e) , (g) user 2's segmentation results on (e) , and (h) automated segmentation results on (e) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAutomaticMethodforRenalCortexSegmentationonCTImages/3_1s20S1076633212000402.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Accuracy of Localization of Top and Bottom Slices

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Segmentation Accuracy Measurement

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Experimental results of kidney and cortex segmentation on one slice by the proposed method. (a) Original slice image, (b) initialization results, (c) kidney segmentation results, (d) cortex segmentation results, and (e) three-dimensional visualization of cortex segmentation results.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAutomaticMethodforRenalCortexSegmentationonCTImages/4_1s20S1076633212000402.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Operation Time Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Running Time in the Segmentation Procedures


Procedure Time (s) Automatic segmentation Step 1: initialization 40 ± 5 Step 2: kidney segmentation 35 ± 6 Step 3: cortex segmentation 30 ± 3 Total Kidney segmentation (step 1 + step 2) 75 ± 7 Cortex segmentation (step 1 + step 2 + step 3) 105 ± 8 Manual segmentation: user 1 Kidney segmentation 435 ± 45 Cortex segmentation 1152 ± 60 Manual segmentation: user 2 Kidney segmentation 486 ± 35 Cortex segmentation 1209 ± 50

Data are expressed as mean ± standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Volume Change before and after Donation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Renal cortex volume change by user 1, user 2, and automated segmentation results.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnAutomaticMethodforRenalCortexSegmentationonCTImages/5_1s20S1076633212000402.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Lee V.S., Rusinek H., Noz M.E., et. al.: Dynamic three-dimensional MR renography for the measurement of single kidney function: initial experience. Radiology 2003; 227: pp. 289-294.


- 2\. Van den Dool S.W., Wasser M.N., de Fijter J.W., et. al.: Functional renal volume: quantitative analysis at gadolinium-enhanced MR angiography-feasibility study in healthy potential kidney donors. Radiology 2005; 236: pp. 189-195.


- 3\. Holden A., Smith A., Dukes P., et. al.: Assessment of 100 live potential renal donors for laparoscopic nephrectomy with multi-detector row helical CT. Radiology 2005; 237: pp. 973-980.


- 4\. Halpern E.J., Mitchell D.G., Wechsler R.J., et. al.: Preoperative evaluation of living renal donors: comparison of CT angiography and MR angiography. Radiology 2000; 216: pp. 434-439.


- 5\. Sahani D.V., Rastogi N., Greenfield A.C., et. al.: Multi-detector row CT in evaluation of 94 living renal donors by readers with varied experience. Radiology 2005; 235: pp. 905-910.


- 6\. Low R.N., Martinez A.G., Steinberg S.M., et. al.: Potential renal transplant donors: evaluation with gadolinium-enhanced MR angiography and MR urography. Radiology 1998; 207: pp. 165-172.


- 7\. Shen W., Kassim A.A., Koh H.K., et. al.: Segmentation of kidney cortex in MRI studies: a constrained morphological 3D h-maxima transform approach. Int J Med Eng Inform 2009; 1: pp. 330-341.


- 8\.  Chevaillier B, Ponvianne Y, Collette JL, et al. Functional semi-automated segmentation of renal DCE-MRI sequences. In: Proceedings of the International Conference on Acoustics, Speech, and Signal Processing; 2008:525–528.


- 9\. Lin D.T., Lei D.T., Hung S.W.: Computer-aided kidney segmentation on abdominal CT images. IEEE Trans Inform Technol Biomed 2006; 10: pp. 59-65.


- 10\. Li X., Chen X., Yao J., et. al.: Renal cortex segmentation using optimal surface search with novel graph construction. Lecture Notes Comput Sci 2011; 6893: pp. 387-394.


- 11\. de Priester J.A., Kessels A.G., Giele E.L., et. al.: MR renography by semiautomated image analysis: performance in renal transplant recipients. J Magn Reson Imaging 2001; 14: pp. 134-140.


- 12\. Shim H., Chang S., Tao C., et. al.: Semiautomated segmentation of kidney from high-resolution multidetector computed tomography images using a graph-cuts technique. J Comput Assist Tomogr 2009; 33: pp. 893-901.


- 13\.  Ali AM, Farag AA, El-Baz AS. Graph cuts framework for kidney segmentation with prior shape constraints. In: Proceedings of the International Conference on Medical Image Computing and Computer Assisted Intervention; 2007:384–392.


- 14\. Tang Y., Jackson H.A., De Filippo R.E., et. al.: Automatic renal segmentation applied in pediatric MR urography. Int J Intel Inform Process 2010; 1: pp. 12-19.


- 15\. Hugen C.M., Polcari A.J., Farooq A.V., et. al.: Size does matter: donor renal volume predicts recipient function following live donor renal transplantation. J Urol 2011; 185: pp. 605-609.


- 16\. Jeon H.G., Lee S.R., Joo D.J., et. al.: Predictors of kidney volume change and delayed kidney function recovery after donor nephrectomy. J Urol 2010; 184: pp. 1057-1063.


- 17\. Boykov Y., Kolmogorov V.: An experimental comparison of min-cut/max-flow algorithms. IEEE Trans Patt Anal Machine Intel 2004; 26: pp. 1124-1137.


- 18\. Kolmogorov V., Zabih R.: What energy functions can be minimized via graph cuts?. IEEE Trans Patt Anal Machine Intel 2004; 26: pp. 147-159.


- 19\. Cootes T., Edwards G., Taylor C.: Active appearance models. IEEE Trans Patt Anal Machine Intel 2001; 23: pp. 681-685.


- 20\. Mitchell S.C., Lelieveldt B.P.F., van der Geest R.J., et. al.: Multistage hybrid active appearance model matching: segmentation of left and right ventricles in cardiac MR images. IEEE Trans Med Imaging 2001; 20: pp. 415-423.


- 21\.  Chen X, Yao J, Zhuge Y, et al. 3D automatic image segmentation based on Graph Cut-Oriented Active Appearance Models. ICIP; 2010. p. 3653–3656.


- 22\. Falcao A.X., Udupa J.K., Samarasekera S., et. al.: User-steered image segmentation paradigms: live wire and live lane. Graph Models Image Process 1998; 60: pp. 233-260.


- 23\. Chen X., Udupa J.K., Alavi A., et. al.: Automatic anatomy recognition via multi-object oriented active shape models. Med Phys 2010; 37: pp. 6390-6401.


- 24\. Ciesielski K.C., Chen X., Udupa J.K., et. al.: Linear time algorithms for exact distance transform. J Math Imaging Vision 2011; 39: pp. 193-209.


- 25\. Udupa J.K., Leblanc V.R., Zhuge Y., et. al.: A framework for evaluating image segmentation algorithms. Comput Medl Imaging Graphics 2006; 30: pp. 75-87.


- 26\. Cox D.R., Hinkley D.V.: Theoretical Statistics.1974.Chapman & HallNew York


- 27\. Bland J.M., Altman D.G.: Statistical methods for assessing agreement between two methods of clinical measurement. Lancet 1986; 1: pp. 307-310.


- 28\. Bland J.M., Altman D.G.: Measuring agreement in method comparison studies. Stat Methods Med Res 1999; 8: pp. 135-160.