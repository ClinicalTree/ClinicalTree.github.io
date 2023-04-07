---
title: Benefit of Overlapping Reconstruction for Improving the Quantitative Assessment of CT Lung Nodule Volume
author: [CL_AT_MariosAGavrielidesPhD,CL_AT_RongpingZengPhD,CL_AT_KyleJMyersPhD,CL_AT_BerkmanSahinerPhD,CL_AT_NicholasPetrickPhD]
date: 2013-02-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 20, Issue 2]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to quantify the effect of overlapping reconstruction on the precision and accuracy of lung nodule volume estimates in a phantom computed tomographic (CT) study.

## Materials and Methods

An anthropomorphic phantom was used with a vasculature insert on which synthetic lung nodules were attached. Repeated scans of the phantom were acquired using a 64-slice CT scanner. Overlapping and contiguous reconstructions were performed for a range of CT imaging parameters (exposure, slice thickness, pitch, reconstruction kernel) and a range of nodule characteristics (size, density). Nodule volume was estimated with a previously developed matched-filter algorithm.

## Results

Absolute percentage bias across all nodule sizes ( _n_ = 2880) was significantly lower when overlapping reconstruction was used, with an absolute percentage bias of 6.6% (95% confidence interval \[CI\], 6.4–6.9), compared to 13.2% (95% CI, 12.7–13.8) for contiguous reconstruction. Overlapping reconstruction also showed a precision benefit, with a lower standard percentage error of 7.1% (95% CI, 6.9–7.2) compared with 15.3% (95% CI, 14.9–15.7) for contiguous reconstructions across all nodules. Both effects were more pronounced for the smaller, subcentimeter nodules.

## Conclusions

These results support the use of overlapping reconstruction to improve the quantitative assessment of nodule size with CT imaging.

The application of lung nodule volume estimation with computed tomographic (CT) imaging is being examined as a more accurate and consistent measure of size change and disease progression compared to the widely used Response Evaluation Criteria in Solid Tumors (RECIST) . The RECIST are based on one-dimensional in-plane measures that are simple and easy to perform but assume that tumor size change can be completely described by a change in the largest in-plane dimension. A true change in volume can be characterized by a change in a one-dimensional measurement only for tumors that are spherical in shape. Volumetric (three-dimensional \[3D\]) measures, in theory, measure the full extent of a lesion and thus may provide an earlier determination of change and an improved quantitative assessment of lesion response to treatment compared with one-dimensional RECIST measures.

The precision and accuracy of CT volume estimates can be affected by a number of factors, including image acquisition and reconstruction parameters, nodule characteristics such as size and density, as well as the software tools used in the estimation process . A factor that has been underexamined is the effect of the reconstruction overlap and its interaction with imaging parameters and nodule characteristics in the context of volumetric assessment of lung nodule size with CT imaging. The reconstruction overlap is an operator-defined parameter, typically involving a choice between overlapping and contiguous reconstruction. Overlapping reconstruction is defined here as a reconstruction interval smaller than the slice thickness, expressed as a percentage of slice thickness. In contrast, contiguous reconstruction involves reconstructing the data using an interval equal to slice thickness (ie, 0% overlap). The ability to retrospectively (without increased x-ray dose to the patient) reconstruct an arbitrary number of overlapping axial images at small increments is a unique feature of helical CT technology. Overlapping reconstruction increases the probability that a lesion is centered in a CT section, which in turn maximizes object contrast . In a theoretical study, Wang and Vannier showed that longitudinal resolution (described by the Fourier transform of the slice sensitivity profile) improved with decreasing reconstruction interval, reaching a pitch-dependent plateau above which no more improvement was possible. Practically, the choice in selecting the reconstruction overlap involves a trade-off between a possible improvement in image quality for a given task through the use of overlapping reconstruction and an increase in the number of slice images in need of processing and review.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Anthropomorphic Phantom and Synthetic Lung Nodules

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Imaging Parameters

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Volume Estimation Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Analysis of Significant Effects

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Analysis of Bias and Variance

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

APNE=100×∣∣Vest−VtrueVtrue∣∣,
APNE

=

100

×

\|

V

est

−

V

true

V

true

\|

,


where _V_ est is the estimated nodule volume obtained with the matched-filter, and _V_ true is the reference standard (true nodule volume). The reference standard was derived from material density information provided by the two manufacturers of the nodules and weight measures performed using a precision scale. Absolute error was used because an underestimate in size was considered to be equal to an overestimate of the same magnitude. Our analysis estimated the absolute percent bias (APB) and the standard deviation of APNE (SPE). APB and SPE were defined as


APB=⟨APNE⟩=100×⟨∣∣Vest−VtrueVtrue∣∣⟩
APB

=

〈

APNE

〉

=

100

×

〈

\|

V

est

−

V

true

V

true

\|

〉


and


SPE=stdev(APNE).
SPE

=

stdev

(

APNE

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Analysis of Significant Effects Using ANOVA

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Results of _n_ -way Analysis of Variance


Source Sum of Squares_df_ Mean Square_F_ Prob > _F_ NodSize 10,097.3 3 3365.8 66.0 .0000  ∗  NodHU 1569.3 1 1569.3 30.8 .0000  ∗  Exposure 166.7 2 83.3 1.6 .1962 Pitch 7.0 1 7.0 0.1 .7120 SliceThn 5806.8 2 2903.4 56.9 .0000  ∗  RecKernel 534.9 1 534.9 10.5 .0013  ∗  ReconOverlap 6652.5 1 6652.5 130.4 .0000  ∗  NodSize × NodHU 554.1 3 184.7 3.6 .0131  ∗  NodSize × Exposure 346.8 6 57.8 1.1 .3416 NodSize × Pitch 159.5 3 53.2 1.0 .3734 NodSize × SliceThn 22,277.1 6 3712.9 72.8 .0000  ∗  NodSize × RecKernel 1619.9 3 540.0 10.6 .0000  ∗  NodSize × ReconOverlap 4439.6 3 1479.9 29.0 .0000  ∗  NodHU × Exposure 293.5 2 146.8 2.9 .0572 NodHU × Pitch 79.8 1 79.8 1.6 .2115 NodHU × SliceThn 139.2 2 69.6 1.4 .2565 NodHU × RecKernel 3.6 1 3.6 0.1 .7897 NodHU × ReconOverlap 50.2 1 50.2 1.0 .3215 Exposure × Pitch 33.3 2 16.6 0.3 .7217 Exposure × SliceThn 102.0 4 25.5 0.5 .7359 Exposure × RecKernel 193.3 2 96.7 1.9 .1514 Exposure × ReconOverlap 335.6 2 167.8 3.3 .0381  ∗  Pitch × SliceThn 48.1 2 24.1 0.5 .6241 Pitch × RecKernel 11.3 1 11.3 0.2 .6384 Pitch × ReconOverlap 22.9 1 22.9 0.4 .5028 SliceThn × RecKernel 128.5 2 64.2 1.3 .2848 SliceThn × ReconOverlap 1505.9 2 752.9 14.8 .0000  ∗  RecKernel × ReconOverlap 96.1 1 96.1 1.9 .1706 Error 26,220.4 514 51.0 Total 83,495.3 575

NodHU, nodule density; NodSize, nodule size; RecKernel, reconstruction kernel; ReconOverlap, reconstruction overlap; SliceThn, slice thickness.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Effect of Reconstruction Overlap as a Function of Nodule Size

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Nodule Volume Estimates Derived from Overlapping and Contiguous Reconstruction as a Function of Nodule Size


Nodule Size Overlapping Contiguous APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) All sizes ( _n_ = 2880) 6.7 (6.4–6.9) 7.1 (6.9–7.2) 13.2 (12.7–13.8) 15.3 (14.9–15.7) 5 mm ( _n_ = 720) 9.1 (8.2–9.9) 12.1 (11.5–12.8) 25.1 (23.3–26.9) 24.6 (23.4–26.0) 8 mm ( _n_ = 720) 5.0 (4.8–5.3) 3.6 (3.4–3.8) 9.5 (8.9–10.1) 8.4 (8.0–8.9) 10 mm ( _n_ = 720) 6.1 (5.9–6.3) 3.1 (3.0–3.3) 11.4 (11.0–11.9) 6.3 (5.9–6.6) 20 mm ( _n_ = 720) 6.3 (6.0–6.7)  ∗  4.6 (4.4–4.9)  ∗  6.8 (6.5–7.1)  ∗  4.2 (4.0–4.4)  ∗

APB, average percentage bias; CI, confidence interval; SPE, standard deviation of absolute percentage normalized error.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Slice across a 20-mm nodule showing multiple vessel attachments ( arrows ).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/BenefitofOverlappingReconstructionforImprovingtheQuantitativeAssessmentofCTLungNoduleVolume/0_1s20S1076633212004709.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Effect of Reconstruction Overlap as a Function of Slice Thickness

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Nodule Volume Estimates Derived from Overlapping and Contiguous Reconstruction as a Function of Slice Thickness


Slice Thickness Overlapping Contiguous APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) 0.75 mm 5.6 (5.3–5.9) 4.4 (4.2–4.6) 10.1 (9.7–10.5) 6.4 (6.1–5.7) 1.5 mm 5.4 (5.1–5.6) 3.9 (3.8–4.1) 9.7 (9.0–10.3) 9.6 (9.2–10.0) 3.0 mm 8.9 (8.2–9.6) 10.4 (9.9–10.8) 19.9 (18.5–21.3) 22.3 (21.4–23.4)

APB, average percentage bias; CI, confidence interval; SPE, standard deviation of absolute percentage normalized error.


All paired differences were statistically significant ( _P_ < .05).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Nodule Volume Estimates Derived from Overlapping and Contiguous Reconstruction as a Function of Nodule Size and Slice Thickness


Nodule Size Slice Thickness 0.75 mm 1.5 mm 3.0 mm Overlapping Contiguous Overlapping Contiguous Overlapping Contiguous APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) 5 mm ( _n_ = 240) 4.7 (4.4–2.0) 2.6 (2.4–2.8) 9.5 (8.2–20.7) 9.6 (8.8–20.6) 3.8 (3.1–2.4) 5.0 (4.6–2.5) 11.6 (9.8–23.3) 13.9 (12.7–25.2) 18.7 (16.6–20.8) 16.4 (15.1–28.0) 54.3 (52.2–26.3) 16.0 (14.7–27.6) 8 mm ( _n_ = 240) 6.1 (5.6–2.6) 3.8 (3.5–2.2) 9.7 (8.7–20.6) 7.6 (7.0–2.3) 4.0 (3.6–2.4) 3.1 (2.8–2.4) 6.9 (6.4–2.5) 4.2 (3.9–2.6) 5.0 (4.6–2.5) 3.5 (3.2–2.9) 11.9 (10.5–23.4) 11.1 (10.2–22.2) 10 mm ( _n_ = 240) 6.3 (5.8–2.8) 4.2 (3.8–2.6)  ∗  9.4 (9.0–2.8) 3.0 (3.8–2.6)  ∗  6.5 (6.2–2.7) 2.1 (2.0–2.3) 16.5 (15.5–27.5) 7.9 (7.3–2.7) 5.5 (5.2–2.8) 2.6 (2.4–2.9) 8.4 (8.1–2.7) 2.7 (2.4–2.9) 20 mm ( _n_ = 240) 5.4 (4.6–2.1) 6.1 (5.6–2.6) 11.9 (11.7–22.0) 0.9 (0.8–2.9) 7.3 (6.8–2.7) 3.8 (3.5–2.1) 3.6 (3.5–2.8) 1.1 (1.0–2.3) 6.4 (5.9–2.8) 3.4 (3.2–2.8)  ∗  4.9 (4.5–2.3) 3.2 (3.0–2.6)  ∗

APB, average percentage bias; CI, confidence interval; SPE, standard deviation of absolute percentage normalized error.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Nodule Volume Estimates Derived from Overlapping and Contiguous Reconstruction for Scans Reconstructed with Equivalent Slice Increment


Nodule Size Equivalent Slice Increment = 0.75 mm Equivalent Slice Increment = 1.5 mm 1.5 mm Overlapping 0.75 mm Contiguous 3.0 mm Overlapping 1.5 mm Contiguous APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) 5 3.8 (3.1–4.4) 5.0 (4.1–5.5) 9.5 (8.1–10.7) 9.6 (8.1–10.6) 18.7 (16.1–20.8)  ∗  16.4 (15.1–18.0)  ∗  11.6 (9.1–13.3)  ∗  13.9 (12.1–15.2)  ∗  8 4.0 (3.1–4.4) 3.1 (2.1–3.4) 9.7 (8.1–10.6) 7.6 (7.1–8.3) 5.0 (4.1–5.5) 3.5 (3.1–3.9) 6.9 (6.1–7.5) 4.2 (3.1–4.6) 10 6.5 (6.1–6.7) 2.1 (2.1–2.3) 9.4 (9.1–9.8) 3.0 (2.1–3.3) 5.5 (5.1–5.8) 2.6 (2.1–2.9) 16.5 (15.1–17.5) 7.9 (7.1–8.7) 20 7.7 (6.1–7.7) 3.8 (3.1–4.1) 11.9 (11.1–12.0) 0.9 (0.1–0.9) 6.4 (5.1–6.8)  ∗  3.4 (3.1–3.8)  ∗  3.6 (3.1–3.8)  ∗  1.1 (1.1–1.3)  ∗

APB, average percentage bias; CI, confidence interval; SPE, standard deviation of absolute percentage normalized error.


Refer to text for an example.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Effect of Reconstruction Overlap as a Function of Other Parameters

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 6


Nodule Volume Estimates Derived from Overlapping and Contiguous Reconstruction as a Function of Image Acquisition Protocol and Nodule Density


Imaging/Nodule Parameter Overlapping Contiguous APB (95% CI) SPE (95% CI) APB (95% CI) SPE (95% CI) Reconstruction kernel B40f ( _n_ = 1440) 7.1 (6.7–7.5) 7.7 (7.5–8.0) 14.6 (13.7–15.5) 17.3 (16.6–17.9) B60f ( _n_ = 1440) 6.2 (5.9–6.5) 6.3 (6.1–6.5) 11.9 (11.2–12.5) 12.8 (12.4–13.3) Exposure 25 mAs ( _n_ = 960) 6.5 (6.0–6.9) 7.0 (6.7–7.3) 14.9 (13.9–16.0) 16.6 (15.9–17.4) 100 mAs ( _n_ = 960) 6.1 (5.7–6.4) 5.6 (5.4–5.9) 12.8 (11.9–13.7) 14.6 (13.9–15.2) 200 mAs ( _n_ = 960) 7.3 (6.8–7.9) 8.3 (8.0–8.7) 11.9 (11.0–12.8) 14.4 (13.8–15.1) Nodule density −630 HU ( _n_ = 1440) 7.8 (7.3–8.2) 8.9 (8.6–9.3) 15.3 (14.7–16.0) 13.4 (12.9–13.9) 100 HU ( _n_ = 1440) 5.5 (5.3–5.7) 4.2 (4.0–4.3) 11.1 (10.2–11.9) 16.7 (16.1–17.3) Pitch 0.9 ( _n_ = 1440) 6.5 (6.1–6.9) 7.7 (7.4–8.0) 13.5 (12.7–14.3) 15.5 (14.9–16.1) 1.2 ( _n_ = 1440) 6.8 (6.4–7.1) 6.4 (6.2–6.6) 12.9 (12.2–13.7) 15.0 (14.5–15.6)

APB, average percentage bias; CI, confidence interval; HU, Hounsfield units; SPE, standard deviation of absolute percentage normalized error.


All paired differences were statistically significant ( _P_ < .05).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Therasse P., Arbuck S.G., Eisenhauer E.A., et. al.: New guidelines to evaluate the response to treatment in solid tumors. J Natl Cancer Inst 2000; 92: pp. 205-216.


- 2\. Eisenhauer E.A., Therasse P., Bogaerts J., et. al.: New response evaluation criteria in solid tumours: revised RECIST guideline (version 1.1). Eur J Cancer 2009; 45: pp. 228-247.


- 3\. Gavrielides M.A., Kinnard L.M., Myers K.J., et. al.: Non-calcified lung nodules: volumetric assessment with thoracic CT. Radiology 2009; 251: pp. 26-37.


- 4\. McNitt-Gray M.F., Bidaut L.M., Armato S.G., et. al.: CT assessment of response to therapy: tumor volume change measurement, truth data and error. Translat Oncol 2009; 2: pp. 216-222.


- 5\. Meyer C.R., Armato S.G., Fenimore C.P., et. al.: Quantitative imaging to assess tumor response to therapy: common themes of measurement, truth data, and error sources. Translat Oncol 2009; 2: pp. 198-210.


- 6\. Leung A.N.: Spiral CT of the thorax in daily practice: optimization of technique. J Thorac Imaging 1997; 12: pp. 2-10.


- 7\. Kalender W.A., Polacin A., Süss C.: A comparison of conventional and spiral CT: an experimental study on the detection of spherical lesions. J Comput Assist Tomogr 1994; 18: pp. 167-176.


- 8\. Wang G., Vannier M.W.: Longitudinal resolution in volumetric x-ray computerized tomography-analytical comparison between conventional and helical computerized tomography. Med Phys 1994; 21: pp. 429-433.


- 9\. Urban B.A., Fishman E.K., Kuhlman J.E., et. al.: Detection of focal hepatic lesions with spiral CT: comparison of 4-and 8-mm interscan spacing. AJR Am J Roentgenol 1993; 160: pp. 783.


- 10\. Diederich S., Lentschig M.G., Winter F., et. al.: Detection of pulmonary nodules with overlapping vs non-overlapping image reconstruction at spiral CT. Eur Radiol 1999; 9: pp. 281-286.


- 11\. Buckley J.A., Scott W.W., Siegelman S.S., et. al.: Pulmonary nodules: effect of increased data sampling on detection with spiral CT and confidence in diagnosis. Radiology 1995; 196: pp. 395-400.


- 12\. Kim J.S., Kim J.H., Cho G., et. al.: Automated detection of pulmonary nodules on CT images: effect of section thickness and reconstruction interval—initial results. Radiology 2005; 236: pp. 295-299.


- 13\. Honda O., Sumikawa H., Johkoh T., et. al.: Computer-assisted lung nodule volumetry from multi-detector row CT: influence of image reconstruction parameters. Eur J Radiol 2007; 62: pp. 106-113.


- 14\. Ravenel J.G., Leue W.M., Nietert P.J., et. al.: Pulmonary nodule volume: effects of reconstruction parameters on automated measurements—a phantom study. Radiology 2008; 247: pp. 400-408.


- 15\. Goo J.M., Tongdee T., Tongdee R., et. al.: Volumetric measurement of synthetic lung nodules with multi-detector row CT: effect of various image reconstruction parameters and segmentation thresholds on measurement accuracy. Radiology 2005; 235: pp. 850-856.


- 16\. Xu D.M., van Klaveren R.J., de Bock G.H., et. al.: Limited value of shape, margin and CT density in the discrimination between benign and malignant screen detected solid pulmonary nodules of the NELSON trial. Eur J Radiol 2008; 68: pp. 347-352.


- 17\. Gavrielides M.A., Zeng R., Kinnard L.M., et. al.: Information-theoretic approach for analyzing bias and variance in lung nodule size estimation. IEEE Trans Med Imaging 2010; 29: pp. 1795-1807.


- 18\. Winer-Muram H.T., Jennings S.G., Meyer C.A., et. al.: Effect of varying CT section width on volumetric measurement of lung tumors and application of compensatory equations. Radiology 2003; 229: pp. 184-194.


- 19\. Wang G., Brink J.A., Vannier M.W.: Theoretical FWTM values in helical CT. Med Phys 1994; 21: pp. 753.


- 20\. Kasales C.J., Hopper K.D., Ariola D.N., et. al.: Reconstructed helical CT scans: improvement in z-axis resolution compared with overlapped and nonoverlapped conventional CT scans. AJR Am J Roentgenol 1995; 164: pp. 1281.


- 21\. Kostis W.J., Reeves A.P., Yankelevitz D.F., et. al.: Three-dimensional segmentation and growth-rate estimation of small pulmonary nodules in helical CT images. IEEE Trans Med Imaging 2003; 22: pp. 1259-1274.


- 22\. Gavrielides M.A., Kinnard L.M., Myers K.J., et. al.: A resource for the assessment of lung nodule size estimation methods: database of thoracic CT scans of an anthropomorphic phantom. Opt Express 2010; 18: pp. 15244-15255.