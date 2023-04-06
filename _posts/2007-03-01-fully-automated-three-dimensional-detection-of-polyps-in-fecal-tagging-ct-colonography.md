---
title: Fully Automated Three-Dimensional Detection of Polyps in Fecal-Tagging CT Colonography
author: [Janne Näppi PhD,Hiroyuki Yoshida PhD]
date: 2007-03-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 3 SOURCE CL_S_AcademicRadiologyVolume14Issue3 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The presence of opacified materials presents several technical challenges for automated detection of polyps in fecal-tagging computed tomography colonography ( _ft_ CTC), such as pseudo-enhancement and the distortion of the density, size, and shape of the observed lesions. We developed a fully automated computer-aided detection (CAD) scheme that addresses these issues in automated detection of polyps in _ft_ CTC.

## Materials and Methods

Pseudo-enhancement was minimized by use of an adaptive density correction (ADC) method. The presence of tagging was minimized by use of an adaptive density mapping (ADM) method. We also developed a new method for automated extraction of the colonic wall within air-filled and tagged regions. The ADC and ADM parameters were optimized by use of an anthropomorphic phantom. The CAD scheme was evaluated with 32+32 cases from two types of clinical _ft_ CTC databases. The cases in database I had full cathartic cleansing and 40 polyps ≥6 mm, and the cases in database II had reduced cathartic cleansing and 44 polyps ≥6 mm. The by-polyp detection performance of the CAD scheme was evaluated by use of a leave-one-patient-out method with five features, and the results were compared with those of a conventional CAD scheme by use of free-response receiver operating characteristic curves.

## Results

The CAD scheme detected 95% and 86% of the polyps ≥6 mm with 3.6 and 4.2 false positives per scan on average in databases I and II, respectively. For polyps ≥10 mm, the detection sensitivity was 94% in database I (with one missed hyperplastic polyp) and 100% in database II at the same false-positive rate. The detection sensitivity of the new CAD scheme was approximately 20% higher than that of the conventional CAD scheme.

## Conclusions

The results show that the CAD scheme developed in this study resolves the technical challenges introduced by fecal tagging, is applicable to a variety of colon preparation regimens, and provides a performance superior to that of conventional CAD schemes.

_Colorectal cancer_ is one of the three leading causes of cancer-related mortalities in the United States. Approximately 148,000 new cases and 55,000 deaths from colon cancer were estimated to occur in 2006 ( ). Screening can reduce colon cancer by facilitating the detection and removal of precancerous polyps. _Colonoscopy_ is considered to have the highest diagnostic performance for screening of colon cancer, but it also has a high cost, risk of complications, and problems with patient compliance ( ).

Minimally invasive _computed tomography colonography_ (CTC, also known as _virtual colonoscopy_ ) can potentially yield a high diagnostic performance in the detection of clinically significant polyps ( ). As with colonoscopy, proper bowel preparation is necessary with CTC for confident detection of colorectal lesions. Residual materials and poor distension can reduce the sensitivity of CTC by obscuring polyps, and solid fecal materials can reduce the specificity of CTC by imitating polyps. The presence of fecal materials can be minimized by use of cathartic cleansing of the colon. However, cathartic cleansing is also a major barrier for patient compliance ( ).

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Detection of Polyps

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ADC Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, An overview of the fecal-tagging computer-aided detection scheme.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/0_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

υI(p)=υˆI(p)+υI(p)PEH,
υ

I

(

p

)

=

υ

^

I

(

p

)

+

υ

I

(

p

)

PEH

,


where the additive term _v  I_ ( _p_ )  PEH represents the effect of PEH at _p_ . We estimate this term by modeling of the PEH as an iterative additive Gaussian effect as follows: Each voxel _q_ with a high value of CT attenuation distributes residual pseudo-enhancement “energy” _r_ 0 ( _q_ ) to its neighboring voxels _p_ according to a Gaussian function. This distributed energy is redistributed iteratively according to


rn(p)=∑qrn−1(q)2π√σ2(rn−1(q))exp(−12∣∣D(p,q)σ2(rn−1(q))∣∣2),
r

n

(

p

)

=

∑

q

r

n

−

1

(

q

)

2

π

σ

2

(

r

n

−

1

(

q

)

)

exp

⁡

(

−

1

2

\|

D

(

p

,

q

)

σ

2

(

r

n

−

1

(

q

)

)

\|

2

)

,


where _σ  2_ ( _r  n−1_ ( _q_ )) represents the Gaussian spread of the distributed residual energy at _q_ at iteration _n_ − 1, and _D_ ( _p, q_ ) is the Euclidean distance between _p_ and _q_ . At each iteration, the residual energy that was distributed during previous iteration is redistributed according to  Eq 2 . The iteration terminates when the redistributable energy becomes negligible. Then, the PEH is minimized by


υˆI(p)=υI(p)−υI(p)PEH≈υI(p)−∑Ni=0ri(p),
υ

^

I

(

p

)

=

υ

I

(

p

)

−

υ

I

(

p

)

PEH

≈

υ

I

(

p

)

−

∑

i

=

0

N

r

i

(

p

)

,


where _N_ is the number of iterations. An advantage of ADC is that it uses only the output data of a CT scanner, and thus it can be applied retrospectively to any CTC cases. After the application of the ADC, we can assume that CT attenuations ≤ _t  T_ ( _t  T_ ≈100 HU) represent untagged materials such as soft tissue and air, whereas higher CT attenuations indicate tagged materials.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ADM Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

υ˙I=⎧⎩⎨⎪⎪⎪⎪υItT−(1000+tT)υI−tTtU−tT−1000υI≤tT,tT<υI<tU,υI≥tU.
υ

˙

I

=

{

υ

I

υ

I

≤

t

T

,

t

T

−

(

1000

+

t

T

)

υ

I

−

t

T

t

U

−

t

T

t

T

<

υ

I

<

t

U

,

−

1000

υ

I

≥

t

U

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Example of the application of the adaptive density mapping (ADM) method in the correction of the measured shape of a polyp covered by opacified fluid. (a) Axial view of the polyp with a –200 ± 800 Hounsfield units lung display window setting. (b) The vertical bar indicates the continuous mapping of five discrete local surface example shapes into shape index values. (c) Visualization of the values of the shape index within the extracted region of the colonic wall in (a) . The shapes indicated by the shape index values are mostly opposite to the visually perceived soft-tissue shapes. (d) Visualization of the shape index values in the same region after the application of the ADM method. The indicated shapes now match the visually perceived shapes.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/1_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, (a) Left: A polyp located within the surface layer of tagged fluid (in the original computed tomography [CT] data). Middle: Effect of the application of Eq 4 . Right: The white region indicates the interface between air and tagged regions identified by the application of the gradient interface analysis method. (b) Left: The white region indicates an initially detected region (in the CT data interpolated to isotropic resolution). Right: The white region indicates the region of a polyp candidate extracted by conditional morphologic dilation (18).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/2_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

υTI(n)(p)={10ifυI(p)≥n,otherwise.
υ

T

I

(

n

)

(

p

)

=

{

1

if

υ

I

(

p

)

≥

n

,

0

otherwise

.


Let _NT__I_ ( _n_ ) ( _p_ ) denote the negation of _T__I_ ( _n_ ) ( _p_ ): if υ _T__I_ ( _n_ )  ( _p_ ) = _m_ ( _m_ = 0,1), then υ _NT__I_ ( _n_ )  ( _p_ ) = 1 – _m_ . Let parameter _t  A_ denote the highest CT attenuation that represents air ( _t  A_ ≈ –700 HU). Then, the region of air is represented by A = _NT_ _I_ ( _t  A_ ), the tagged region is represented by _T_ = _T  I_ ( _t  T_ ), and the soft-tissue region is represented by S = _NT  I_ ( _t  T_ ) ∩ _T  I_ ( _t  A_ ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Line samples of three different interface types in the phantom data with 300 HU tagging during the (a) first and (b) second step of the gradient interface analysis method. The data were preprocessed by the ADC method. In (a) , CT attenuations >100 HU have been clipped to 100 HU. The contrast between soft tissue and tagging is much lower than that between the other interfaces. In (b) , CT attenuations >100 HU have been clipped to 800 HU. The contrast between air and soft tissue is much lower than that between air and tagging. Based on these data, the three interfaces may be differentiated as explained in the text. Abbreviations: HU = Hounsfield unit; A ¦ S = air and soft tissue; A ¦ T = air and tagging; S ¦ T = soft tissue and tagging.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/3_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

υ′′(p)={tT+700υI(p)ifυI(p)≥tT,otherwise.
υ

″

(

p

)

=

{

t

T

+

700

if

υ

I

(

p

)

≥

t

T

,

υ

I

(

p

)

otherwise

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

A\|T=T∇I'(t∇I')∩T∇I′′(t∇I′′),
A

\|

T

=

T

∇

I

′

(

t

∇

I

′

)

∩

T

∇

I

″

(

t

∇

I

″

)

,


A\|S=T∇I'(t∇I')\T∇I′′(t∇I′′),
A

\|

S

=

T

∇

I

′

(

t

∇

I

′

)

\

T

∇

I

″

(

t

∇

I

″

)

,


S\|T=T∇I′′(t∇I′′)\T∇I'(t∇I').
S

\|

T

=

T

∇

I

″

(

t

∇

I

″

)

\

T

∇

I

′

(

t

∇

I

′

)

.


where _t_ ∇ _I_ ″ is set to exceed the highest contrast of the CT attenuation within the interfaces _A_ ¦ _S_ and _S_ ¦ _T_ . Thus we have obtained the region of the interface _A_ ¦ _T_ which is then excluded from the detection of polyp candidates as explained previously.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Colonic Lumen Tracking Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

D(Pe2r,Pe1k)+D(Pe2k,Pe1d)<D(Pe2r,Pe1l)+D(Pe2l,Pe1d)
D

(

P

r

e

2

,

P

k

e

1

)

+

D

(

P

k

e

2

,

P

d

e

1

)

<

D

(

P

r

e

2

,

P

l

e

1

)

+

D

(

P

l

e

2

,

P

d

e

1

)


and


D(Pe2k,Pe1d)<D(Pe2r,Pe1d).
D

(

P

k

e

2

,

P

d

e

1

)

<

D

(

P

r

e

2

,

P

d

e

1

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Illustration of the colonic lumen tracking method; see text for additional explanation. (a) Input computed tomography (CT) images are stacked into a volume. (b) Labeling of the voxels. (c) Cut-plane views of the conversion of the CT volume into binary volume. (d) Visualization of a piece of tracked path entering and exiting tagged fluid within the colonic lumen. (e) All tracked abdominal lumen paths. (f) Three initially established landmarks and the tracking of their corresponding primary segments. (g) Lumen tracking in sigmoid colon. The end point of the rectal segment that is indicated by large white sphere can be connected to one of the four indicated candidate connections. (h) Further lumen tracking in sigmoid colon. (i) Completed lumen path with adjusted landmark locations. (j) Result of the region-growing steps. (k) Result of the final shape-based interpolation step.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/4_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Parameter Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Examples of line samples of 11 polyps that were covered by low-density (300 Hounsfield units [HU]; solid lines) and moderate-density (600 HU; dotted lines) tagging. The line samples were calculated after the application of the adaptive density correction method.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/5_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation of CAD Performance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, (a) In database I, the full cathartic preparation eliminated most residual materials. The remaining residual materials were clearly tagged because of the large dose of high-density tagging agent. This simplifies the detection of abnormalities such as the polyp seen at the center of the image. (b) In database II, the reduced cathartic preparation could leave residual materials that imitate polyps in the colon. If tagged, these materials could be identified confidently. However, because of the experimental nature of the data, some of the cases included poorly tagged or untagged fecal materials that could be confused with true abnormalities.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/6_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Leave-one-patient-out detection performance on database I for the 40 polyps ≥6 mm. The thick and thin solid lines indicate the performance of the fecal-tagging computer-aided detection ( ft CAD) and ft CADb schemes, respectively, and the dotted line indicates the performance of the n CAD scheme.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/7_1s20S1076633206006738.jpg)

![Figure 9, Leave-one-patient-out detection performance on database II for the 44 polyps ≥6 mm. The thick and thin solid lines indicate the performance of the fecal-tagging computer-aided detection ( ft CAD) and ft CADb schemes, respectively, and the dotted line indicates the performance of the n CAD scheme.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/8_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Comparison of typical false-positive and false-negative detections of the CTC cases without fecal tagging ( n CAD) and fecal-tagging computer-aided detection ( ft CAD) schemes. (a) The n CAD scheme missed this polyp covered by tagged fluid, whereas the ft CAD scheme detected the polyp correctly. (b) The n CAD scheme detected this stool (arrow) incorrectly as a flat lesion based upon its shape. The ft CAD scheme identified the lesion correctly as an FP based on the fecal tagging. (c) An example of untagged stool (indicated by arrow) that was detected incorrectly as a polyp by both CAD schemes.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/9_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 11, Examples of false-positive (FP) fecal-tagging computer-aided detection (CAD) detections in database I. (a) Thickened fold (indicated by arrow). Folds are the single major source of FP detections in cathartically cleansed cases. (b) Polypoid pattern (indicated by arrow) on an ileocecal valve. Up to 10% of CAD detections tend to be generated by ileocecal valves. (c) An example of untagged residual material detected by CAD. Such lesions are not common in cathartically cleansed fecal-tagging cases.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/10_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 12, Examples of false-positive (FP) fecal-tagging computer-aided detection (FP ft CAD) detections in database II. (a) Small fold imitating a polyp (arrow). The top figure shows the lesion in lung display window, and the bottom figure shows the lesion in soft-tissue display window setting. (b) Poorly tagged feces with polypoid appearance (arrow). Folds and poorly tagged feces are the two major sources of FP detections in reduced and noncathartic colon preparations. (c) Ileocecal valve with a masslike appearance. The arrow indicates a polypoid pattern that was detected by CAD.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/FullyAutomatedThreeDimensionalDetectionofPolypsinFecalTaggingCTColonography/11_1s20S1076633206006738.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Jemal A., Siegel R., Ward E., et. al.: Cancer statistics, 2006. CA Cancer J Clin 2006; 56: pp. 106-130.


- 2\. Glick S.: Background and significance.Dachman A.Atlas of virtual colonoscopy.2003.Springer-VerlagNew York:pp. 5-9.


- 3\. Pickhardt P., Choi J., Hwang I., et. al.: Computed tomographic virtual colonoscopy to screen for colorectal neoplasia in asymptomatic adults. N Engl J Med 2003; 349: pp. 2191-2200.


- 4\. Gluecker T., Johnson C., Harmsen W., et. al.: Colorectal cancer screening with CT colonography, colonoscopy, and double-contrast barium enema examination: prospective assessment of patient perceptions and preferences. Radiology 2003; 227: pp. 378-384.


- 5\. Lefere P., Gryspeerdt S., Dewyspelaere J., et. al.: Dietary fecal tagging as a cleansing method before CT colonography: initial results - polyp detection and patient acceptance. Radiology 2002; 24: pp. 393-403.


- 6\. Zalis M., Perumpillichira J., Del Frate C., et. al.: CT colonography: digital subtraction bowel cleansing with mucosal reconstruction—initial observations. Radiology 2003; 226: pp. 911-917.


- 7\. Iannaccone R., Laghi A., Magniapane F., et. al.: Computed tomographic colonography without cathartic preparation for the detection of colorectal polyps. Gastroenterology 2004; 127: pp. 1300-1311.


- 8\. Lefere P., Gryspeerdt S.: 2006.SpringerBerlin, Germany


- 9\. Yoshida H.: The future: computer-aided detection.Lefere P.Gryspeerdt S.2006.SpringerBerlin, Germany:pp. 137-152.


- 10\. Yoshida H., Näppi J.: Three-dimensional computer-aided diagnosis scheme for detection of colonic polyps. IEEE Trans Med Imaging 2001; 20: pp. 1261-1274.


- 11\. Yoshida H., Dachman A.: CAD techniques, challenges and controversies in computed tomographic colonography. Abdom Imaging 2004; 30: pp. 26-41.


- 12\. Frimmel H., Näppi J., Yoshida H.: Centerline-based colon segmentation for CT colonography. Med Phys 2005; 32: pp. 2665-2672.


- 13\. Summers R., Franaszek M., Miller M.: Computer-aided detection of polyps on oral contrast-enhanced CT colonography. AJR Am J Roentgenol 2005; 184: pp. 105-108.


- 14\. Summers R., Yao J., Pickhardt P., et. al.: Computed tomographic virtual colonoscopy computer-aided polyp detection in a screening population. Gastroenterology 2005; 2005: pp. 1832-1844.


- 15\. Zalis M., Yoshida H., Näppi J., et. al.: Evaluation of false positive detections in combined computer aided polyp detection and minimal preparation/digital subtraction CT colonography (CTC). Proc RSNA 2004; pp. 578.


- 16\. Näppi J., Frimmel H., Dachman A., et. al.: A new high-performance CAD scheme for the detection of polyps in CT colonography.Fitzpatrick J.Sonka M.SPIE medical imaging 2004.2004.SPIE PressBellingham WA, USA:pp. 839-848.


- 17\. Yoshida H., Näppi J., MacEneaney P., et. al.: Computer-aided diagnosis scheme for detection of polyps at CT colonography. Radiographics 2002; 22: pp. 963-979.


- 18\. Näppi J., Yoshida H.: Feature-guided analysis for reduction of false positives in CAD of polyps for CT colonography. Med Phys 2003; 30: pp. 1592-1601.


- 19\. Lefere P., Gryspeerdt S., Marrannes J., et. al.: CT colonography after fecal tagging with reduced cathartic cleansing and a reduced volume of barium. AJR Am J Roentgenol 2005; 184: pp. 1836-1842.


- 20\. Näppi J., Okamura A., Frimmel H., et. al.: Region-based supine-prone correspondence for the reduction of false-positive CAD polyp candidates in CT colonography. Acad Radiol 2005; 12: pp. 695-707.


- 21\. Kupinski M., Edwards D., Giger M., et. al.: Ideal observer approximation using Bayesian classification neural networks. IEEE Trans Med Imaging 2001; 20: pp. 886-899.


- 22\. Näppi J., Yoshida H.: Automated detection of polyps in CT colonography: evaluation of volumetric features for reduction of false positives. Acad Radiol 2002; 9: pp. 386-397.


- 23\.  Näppi J, Yoshida H. Adaptive correction of CT attenuation for computer-aided detection of polyps in fecal-tagging CT colonography. Submitted.


- 24\. Näppi J., Yoshida H.: Adaptive normalization of fecal-tagging CT colonography images for computer-aided detection of polyps. Int J Comp Assisted Radiol Surg 2006; 1: pp. 371-372.


- 25\. Näppi J., MacEneaney P., Dachman A., et. al.: Knowledge-guided automated segmentation of colon for computer-aided detection of polyps in CT colonography. J Comput Assist Tomogr 2002; 26: pp. 493-504.


- 26\. Frimmel H., Näppi J., Yoshida H.: Fast and robust computation of colon centerline in CT colonography. Med Phys 2004; 31: pp. 3046-3056.


- 27\. Sethian J.: 1999.Cambridge University PressCambridge, MA


- 28\. Zalis M., Perumpillichira J., Kim J., et. al.: Polyp size at CT colonography after electronic subtraction cleansing in an anthropomorphic colon phantom. Radiology 2005; 236: pp. 118-124.


- 29\. Callstrom M., Johnson C., Fletcher J., et. al.: CT colonography without cathartic preparation: feasibility study. Radiology 2001; 219: pp. 693-698.


- 30\. Bunch P., Hamilton J., Sanderson G., et. al.: A free-response approach to the measurement and characterization of radiographic-observer performance. J Appl Photogr Eng 1978; 4: pp. 166-171.


- 31\. Metz C.: Evaluation of CAD methods.Doi K. et. al.Computer-Aided diagnosis in medical imaging.1999.Elsevier ScienceAmsterdam, The Netherlands:pp. 543-544.


- 32\. Näppi J., Zalis M., Cai W., et. al.: CAD in minimal-preparation CT colonography: technical feasibility. Proc RSNA 2005; pp. 440.


- 33\. Tourassi G., Floyd C.: The effect of data sampling on the performance evaluation of artificial neural networks in medical diagnosis. Med Decis Making 1997; 17: pp. 186-192.