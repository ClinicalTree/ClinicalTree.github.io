---
title: Can CT and MR Shape and Textural Features Differentiate Benign Versus Malignant Pleural Lesions?
author: [CL_AT_ElenaPenaMD,CL_AT_MacArinzeOjiakuMD,CL_AT_JoaoRInacioMD,CL_AT_AshishGuptaMD,CL_AT_DBlairMacdonaldMDFRCPC,CL_AT_WaelShabanaMDPhD,CL_AT_JeanMSeelyMDFRCPC,CL_AT_FrankJRybickiMDPhD,CL_AT_CaroleDennieMDFRCPC,CL_AT_RebeccaEThornhillPhD]
date: 2017-10-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 24, Issue 10]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The study aimed to identify a radiomic approach based on CT and or magnetic resonance (MR) features (shape and texture) that may help differentiate benign versus malignant pleural lesions, and to assess if the radiomic model may improve confidence and accuracy of radiologists with different subspecialty backgrounds.

## Materials and Methods

Twenty-nine patients with pleural lesions studied on both contrast-enhanced CT and MR imaging were reviewed retrospectively. Three texture and three shape features were extracted. Combinations of features were used to generate logistic regression models using histopathology as outcome. Two thoracic and two abdominal radiologists evaluated their degree of confidence in malignancy. Diagnostic accuracy of radiologists was determined using contingency tables. Cohen's kappa coefficient was used to assess inter-reader agreement. Using optimal threshold criteria, sensitivity, specificity, and accuracy of each feature and combination of features were obtained and compared to the accuracy and confidence of radiologists.

## Results

The CT model that best discriminated malignant from benign lesions revealed an AUC  CT = 0.92 ± 0.05 ( _P_ < 0.0001). The most discriminative MR model showed an AUC  MR = 0.87 ± 0.09 ( _P_ < 0.0001). The CT model was compared to the diagnostic confidence of all radiologists and the model outperformed both abdominal radiologists ( _P_ < 0.002), whereas the top discriminative MR model outperformed one of the abdominal radiologists ( _P_ = 0.02). The most discriminative MR model was more accurate than one abdominal ( _P_ = 0.04) and one thoracic radiologist ( _P_ = 0.02).

## Conclusion

Quantitative textural and shape analysis may help distinguish malignant from benign lesions. A radiomics-based approach may increase diagnostic confidence of abdominal radiologists on CT and MR and may potentially improve radiologists' accuracy in the assessment of pleural lesions characterized by MR.

## Introduction

Pleural disease has a wide variety of etiologies, ranging from benign inflammatory and infectious processes to aggressive malignancy . The most common pleural malignancy is metastatic adenocarcinoma. The second most common is malignant pleural mesothelioma (MPM) , a tumor strongly associated with asbestos exposure. MPM portends a poor prognosis, has a median survival rate of 9–17 months, and may be fatal in a few months if untreated .

Although a definitive diagnosis of malignant pleural disease often relies on tissue histopathology, it is challenging to differentiate MPM from benign reactive mesothelial cells . Several invasive procedures may be required to obtain sufficient tissue , and a large panel of immunohistochemical markers is often required to establish the correct diagnosis. Thus, imaging and in particular computed tomography (CT) plays a major role for both diagnosis and follow-up of pleural lesions . Radiologists currently use conventional visual assessment of morphologic findings to distinguish benign from malignant pleural disease. However, benign pleural reaction may resemble malignancy, as the pleura can react to disparate pathologic processes in a similar way, namely thickening and effusions .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

## Study Population

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Imaging Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Slice Selection, Segmentation, and Imaging Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Examples of segmentations of nodular (a, b) and smooth (c, d) pleural lesions on CT and MR. Axial contrast-enhanced CT (a) and MR images (b) showing the segmentation ( yellow lines ) of a nodular pleural lesion involving the left anterior mediastinal pleura. Core biopsies of the lesion were diagnostic of mesothelioma. Axial contrast-enhanced CT (b) and MR (d) images show the segmentation ( yellow lines ) of the smooth pleural thickening along the right posterior costal pleura. Core biopsies revealed fibrous pleural thickening without malignant features. Additionally, the lesion was stable on follow-up imaging for 3 years, indicating benignity. CT, computed tomography; MR, magnetic resonance. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CanCTandMRShapeandTexturalFeaturesDifferentiateBenignVersusMalignantPleuralLesions/0_1s20S1076633217301332.jpg)

![Figure 2, Representative contrast-enhanced CT (a) and MR images (d) demonstrating an enhancing lobulated pleural lesion of an 88-year-old male. Pleuroscopy revealed mesothelioma with both epithelioid and sarcomatoid elements. The selected areas depicted in (a) and (d) demonstrate the lesion chosen for segmentation ( b and e , respectively). The rectangular areas in (a) and (d) are magnified 400% (b) and 600% (e) , respectively, to better depict the segmentation. (c, f) Show screen captures of the software program utilized to extract the shape and textural features (MaZda) of the segmented lesion. CT, computed tomography; MR, magnetic resonance.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CanCTandMRShapeandTexturalFeaturesDifferentiateBenignVersusMalignantPleuralLesions/1_1s20S1076633217301332.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Subjective Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantitative Texture and Shape Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Mean=1Np∑ijg(i,j)
M

e

a

n

=

1

N

p

∑

i

j

g

(

i

,

j

)


where _g_ ( _i, j_ ) indicates the gray-level intensity of pixel ( _i, j_ ), and _N  p_ the number of pixels.


f8=−∑2Ngi=1px+y(i)log{px+y(i)},wherepx+y(k)=∑Ngi=1i+j=k∑Ngj=1P(i,j),k=2,3,…2Ng
f

8

=

−

∑

i

=

1

2

N

g

p

x

+

y

(

i

)

log

{

p

x

+

y

(

i

)

}

,

where

p

x

+

y

(

k

)

=

∑

i

=

1

i

+

j

=

k

N

g

∑

j

=

1

N

g

P

(

i

,

j

)

,

k

=

2

,

3

,

…

2

N

g


f9=∑Ngi=1∑Ngj=1P(i,j)log(P(i,j))
f

9

=

∑

i

=

1

N

g

∑

j

=

1

N

g

P

(

i

,

j

)

log

(

P

(

i

,

j

)

)


where _N  g_ represents the number of distinct gray levels, _g  i_ , and indicates the _ith_ gray-level value ( _i_ = 1, 2, …, _N_ ); _P(i, j)_ indicates the joint probability of two pixels having particular co-occurring values _i, j_ = 1, 2, …, _N  g_ ; and µ  x , µ  y , σ  x , and σ  y indicate means and standard deviations of the row and column sums of the co-occurrence matrix , .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Rc=2A/π√∑D/π
R

c

=

2

A

/

π

∑

D

/

π


where _A_ indicates the area of the lesion (number of pixels) and _D_ denotes the contour profile diameter.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Patient Demographics, Diagnosis, and Pleural Lesion Characteristics


Patients Benign Lesions Malignant Lesions_n_ 12 17 Gender (M/F) 8/4 16/1 Age (mean ± SD) 67 ± 16 73 ± 10 Lesion diagnosis ( _N_ ) Benign (12) Malignant (17) Etiology ( _n_ , diagnosis) 5 chronic inflammation

2 pleural plaques

1 solitary fibrous tumor

4 benign (stable over 2 years on imaging studies) 12 mesothelioma

8 epithelioid

3 biphasic

1 sarcomatoid 5 metastasis

4 adenocarcinoma (2 in the lungs, 1 in the breast, 1 in the salivary gland)

1 pleomorphic undifferentiated sarcoma Involvement of mediastinal pleura, _n_ (%) 0 (0%) 9 (53%)_P_ = 0.003 Pleural thickening >1 cm 6 (50%) 15 (88%)_P_ = 0.04 Nodular contour, _n_ (%) 3 (25%) 15 (88%)_P_ = 0.001 Circumferential pleural thickening, _n_ (%) 0 (0%) 15 (88%)_P_ < 0.0001

F, female; M, male; SD, standard deviation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Comparison of receiver operating characteristic curves for thoracic radiologists 1 and 2 and abdominal radiologists 1 and 2 for identification of malignant lesions on CT and MR. The thoracic radiologists' AUC CT (SE) was 0.91 (0.07) and 0.92 (0.03) ( P < .0001), and the AUC MR (SE) was 0.96 (0.03) and 0.79 (0.07), both significantly different from AUC = 0.5 ( P < .0001). The abdominal radiologists' AUC CT was 0.51 (0.09) and 0.56 (0.11), and the AUC MR was 0.53 (0.10) and 0.61 (0.10), and they were not significantly different from AUC = 0.5 ( P > 0.05). AUC, area under the curve; CT, computed tomography; MR, magnetic resonance; SE, standard error.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CanCTandMRShapeandTexturalFeaturesDifferentiateBenignVersusMalignantPleuralLesions/2_1s20S1076633217301332.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Box and whisker plots depicting medians, interquartile ranges, and extrema for each of the texture features (a) mean, (b) f 8 , and (c) f 9 , and shape features (d) S1, (e) N i , and (f) R c for both benign and malignant pleural lesions. On CT, the median values of f 8 (sum entropy) and S1 (a feature related to maximum thickness of the contour skeleton) were significantly lower in benign compared to malignant lesions ( P < 0.002 and P = 0.03, respectively). Additionally, on MR, the median values of N i (a feature related to the number of skeleton branches) demonstrated significant differences comparing benign to malignant lesions ( P = 0.02). CT, computed tomography; MR, magnetic resonance.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CanCTandMRShapeandTexturalFeaturesDifferentiateBenignVersusMalignantPleuralLesions/3_1s20S1076633217301332.jpg)

![Figure 5, Individual receiving operating characteristic curves of textural features (a) mean, (b) f 8 , and (c) f 9 , and shape features (d) S1, (e) N i , and (f) R c on CT and MR for identification of malignant lesions. The features most capable of delineating malignant from benign lesions on CT images were f 8 (AUC CT = 0.75 ± 0.10) and S1 (AUC CT = 0.74 ± 0.11), both ( P < 0.05). On MR, the descriptors mean, N i , and S1 reached significance, with AUC MR = 0.70 ± 0.10, AUC MR = 0.76 ± 0.10, and AUC MR = 0.71 ± 0.11 ( P < 0.05), respectively. AUC, area under the curve; CT, computed tomography; MR, magnetic resonance.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/CanCTandMRShapeandTexturalFeaturesDifferentiateBenignVersusMalignantPleuralLesions/4_1s20S1076633217301332.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Receiver Operating Characteristics for Combinations of CT or MR Features


Model CT MRI AUC (SE)  \\* _P_ Criterion Se (%) Sp (%) AUC (SE)  \\* _P_ Criterion Se (%) Sp (%) Shape: S1 + R  c  + N  i  0.78 (0.09) 0.001 >0.63 71 83 0.75 (0.10) 0.01 >0.39 88 67 Shape: S1 + R  c  0.69 (0.10) 0.07 >0.69 47 92 0.68 (0.11) 0.10 >0.50 82 67 Texture: f  8  +  f  9  + mean 0.86 (0.07) <0.0001 >0.48 82 83 0.72 (0.10) 0.02 >0.74 41 100 Texture: f  8  + mean 0.84 (0.08) <0.0001 >0.58 82 83 0.70 (0.10) 0.06 >0.33 100 33 Shape and texture: S1 + R  c  + f  8  + mean 0.92 (0.05) <0.0001 >0.35 94 75 0.76 (0.09) 0.005 >0.67 53 92 Shape and texture: S1 + f  8  + mean 0.85 (0.07) <0.0001 >0.52 82 83 0.70 (0.10) 0.048 >0.32 100 33 Shape and texture: R  c  + f  8  + mean 0.86 (0.08) <0.0001 >0.45 88 75 0.77 (0.09) 0.004 >0.50 71 75 Shape and texture: S1 + R  c  + f  8  0.87 (0.07) <0.0001 >0.42 100 75 0.68 (0.11) 0.09 >0.56 71 75 Shape and texture: S1 + R  c  + mean 0.75 (0.10) 0.01 >0.53 71 75 0.76 (0.09) 0.005 >0.39 94 50 Shape and texture: S1 + f  8  0.76 (0.10) 0.01 >0.53 82 67 0.64 (0.11) 0.23 >0.57 71 67 Shape and texture: S1 + mean 0.73 (0.11) 0.03 >0.56 76 75 0.72 (0.10) 0.03 >0.56 65 75 Shape and texture: R  c  + f  8  0.86 (0.08) <0.0001 >0.57 82 83 0.65 (0.11) 0.18 >0.51 76 67 Shape and texture: R  c  + mean 0.77 (0.10) 0.01 >0.70 59 92 0.76 (0.09) 0.005 >0.39 94 50 PC-1 0.67 (0.11) 0.11 ≤-1.81 71 75 0.69 (0.10) 0.06 >16.93 41 100 PC-2 0.63 (0.12) 0.28 >-8.27 94 42 0.76 (0.11) 0.01 >-2.28 76 75 PC-3 0.52 (0.11) 0.90 ≤-2.20 47 67 0.75 (0.10) 0.01 ≤0.41 71 83 PC-1 + PC-2 0.71 (0.11) 0.07 >0.54 82 75 0.77 (0.10) 0.01 >0.43 100 58 PC-1 + PC-2 + PC-3 0.71 (0.11) 0.06 >0.55 76 75 0.87 (0.09) 0.0001 >0.45 100 83

AUC, area under the curve; CT, computed tomography; MR, magnetic resonance; MRI, magnetic resonance imaging; Se, sensitivity; Sp, specificity.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Difference in AUC (95% CI) Between CT Shape and Textural Features and Subjective Visual Assessment (Confidence)


Reader CT Models MRI Models S1 + R  c  + f  8  + Mean R  c  + f  8  + Mean PC-1 + PC-2 + PC-3 S1 + R  c  + f  8  + Mean R  c  + f  8  + Mean PC-1 + PC-2 + PC-3 Thoracic radiologist 1 0.01 \[−0.15 to 0.17\]; 0.90 0.05 \[−0.15 to 0.25\]; 0.64 −0.20 \[−0.06 to 0.47\]; 0.14 −0.21 \[0.04 to 0.37\]; 0.01 −0.20 \[0.03 to 0.36\]; 0.02 −0.09 \[−0.09 to 0.28\]; 0.33 Thoracic radiologist 2 0.00 \[−0.16 to 0.17\]; 0.95 0.05 \[−0.15 to 0.25\]; 0.60 −0.21 \[−0.06 to 0.47\]; 0.13 −0.04 \[−0.20 to 0.27\]; 0.76 −0.03 \[−0.20 to 0.26\]; 0.82 0.08 \[−0.14 to 0.30\]; 0.50 Abdominal radiologist 1 0.41 \[0.17 to 0.66\]; 0.001 0.35 \[0.06 to 0.64\]; 0.02 0.20 \[−0.09 to 0.50\]; 0.18 0.23 \[−0.05 to 0.50\]; 0.10 0.24 \[−0.03 to 0.50\]; 0.08 0.34 \[0.05 to 0.62\]; 0.02 Abdominal radiologist 2 0.36 \[0.13 to 0.60\]; 0.002 0.30 \[0.05 to 0.56\]; 0.02 0.15 \[−0.18 to 0.48\]; 0.37 0.14 \[−0.15 to 0.43\]; 0.34 0.15 \[−0.12 to 0.42\]; 0.27 0.26 \[−0.04 to 0.56\]; 0.10

AUC, area under the curve; CI, confidence interval; CT, computed tomography; MRI, magnetic resonance imaging; PC, principal components.


Values indicate difference in AUC between shape and texture model and radiologist readers \[95% CI\]; _P_ value.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Difference in Accuracy Between Shape and Textural Models and Subjective Diagnosis (Benign vs Malignant)


Reader CT Models MRI Models S1 + R  c  + f  8  + Mean R  c  + f  8  + Mean PC-1 + PC-2 + PC-3 S1 + R  c  + f  8  + Mean R  c  + f  8  + Mean PC-1 + PC-2 + PC-3 Thoracic radiologist 1 3.5% \[−12.2 to 15.4\]; 1.00 −6.9% \[−11.5 to 18.9\]; 0.69 −17.2% \[−6.2 to 29.3\]; 0.18 −17.2% \[−6.2 to 29.3\]; 0.18 −20.7% \[1.7 to 20.7\]; 0.03 −6.9% \[−8.4 to 13.6\]; 0.63 Thoracic radiologist 2 13.8% \[−8.3 to 25.8\]; 0.29 −10.3% \[−12.5 to 26.4\]; 0.51 0.0% \[−26.0 to 26.0\]; 1.00 −3.5% \[−26.0 to 31.7\]; 1.00 −0.0% \[−23.9 to 23.9\]; 1.00 27.6% \[3.8 to 34.3\]; 0.02 Abdominal radiologist 1 13.8% \[−8.3 to 25.8\]; 0.29 10.3% \[−10.1 to 22.4\]; 0.45 0.0% \[−18.9 to 18.9\]; 1.00 3.5% \[−22.3 to 27.6\]; 1.00 6.9% \[−16.4 to 26.1\]; 0.75 20.7% \[−1.5 to 27.4\]; 0.07 Abdominal radiologist 2 13.8% \[−10.5 to 29.9\]; 0.34 10.3% \[−10.1 to 22.4\]; 0.45 0.0% \[−15.8 to 15.8\]; 1.00 0.0% \[−18.9 to 18.9\]; 1.00 3.5% \[−17.9 to 22.5\]; 1.00 24.1% \[1.1 to 30.9\]; 0.04

CI, confidence interval; CT, computed tomography; PC, principal components.


Values indicate difference in % accuracy between shape and texture model and binary diagnosis by radiologist readers \[95% CI\]; _P_ value.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Leff A., Hopewell P.C., Costello J.: Pleural effusion from malignancy. Ann Intern Med 1978; 88: pp. 532-537.


- 2\. Bonomo L., Feragalli B., Sacco R., et. al.: Malignant pleural disease. Eur J Radiol 2000; 34: pp. 98-118.


- 3\. Tsao A.S., Wistuba I., Roth J.A., Kindler H.L.: Malignant pleural mesothelioma. J Clin Oncol 2009; 27: pp. 2081-2090.


- 4\. Roggli V.L., Kolbeck J., Sanfilippo F., Shelburne J.D.: Pathology of human mesothelioma. Etiologic and diagnostic considerations. Pathol Annu 1987; 22: pp. 91-131.


- 5\. Wang Z.J., Reddy G.P., Gotway M.B., et. al.: Malignant pleural mesothelioma: evaluation with CT, MR imaging, and PET. Radiographics 2004; 24: pp. 105-119.


- 6\. Aisner J.: Current approach to malignant mesothelioma of the pleura. Chest 1995; 107: pp. 332S-344S.


- 7\. Nickell L.T., Lichtenberger J.P., Khorashadi L., et. al.: Multimodality imaging for characterization, classification, and staging of malignant pleural mesothelioma. Radiographics 2014; 34: pp. 1692-1706.


- 8\. Leung A.N., Muller N.L., Miller R.R.: CT in differential diagnosis of diffuse pleural disease. AJR Am J Roentgenol 1990; 154: pp. 487-492.


- 9\. Knuuttila A., Kivisaari A., Kivisaari M., et. al.: Evaluation of pleural disease using MR and CT. With special reference to malignant pleural mesothelioma. Acta Radiol 2001; 42: pp. 502-507.


- 10\. Hierholzer J., Luo L., Bittner R.C., et. al.: MRI and CT in the differential diagnosis of pleural disease. Chest 2000; 118: pp. 604-609.


- 11\. Benamore R.E., O'Doherty M.J., Entwisle J.J.: Use of imaging in the management of malignant pleural mesothelioma. Clin Radiol 2005; 60: pp. 1237-1247.


- 12\. Gillies R.J., Kinahan P.E., Hricak H.: Radiomics: images are more than pictures, they are data. Radiology 2016; 278: pp. 563-577.


- 13\. Kido S., Kuriyama K., Higashiyama M., et. al.: Fractal analysis of small peripheral pulmonary nodules in thin-section CT: evaluation of the lung-nodule interfaces. J Comput Assist Tomogr 2002; 26: pp. 573-578.


- 14\. Dennie C., Thornhill R., Sethi-Virmani V., et. al.: Role of quantitative computed tomography texture analysis in the differentiation of primary lung cancer and granulomatous nodules. Quant Imaging Med Surg 2016; 6: pp. 6-15.


- 15\. Gibbs P., Turnbull L.W.: Textural analysis of contrast-enhanced MR images of the breast. Magn Reson Med 2003; 50: pp. 92-98.


- 16\. Ahmed A., Gibbs P., Pickles M., Turnbull L.: Texture analysis in assessment and prediction of chemotherapy response in breast cancer. J Magn Reson Imaging 2013; 38: pp. 89-101.


- 17\. Simon I., Snow P.B., Marks L.S., et. al.: Neural network prediction of prostate tissue composition based on magnetic resonance imaging analysis. A pilot study. Anal Quant Cytol Histol 2000; 22: pp. 445-452.


- 18\. Wibmer A., Hricak H., Gondo T., et. al.: Haralick texture analysis of prostate MRI: utility for differentiating non-cancerous prostate from prostate cancer and differentiating prostate cancers with different Gleason scores. Eur Radiol 2015; 25: pp. 2840-2850.


- 19\. Ganeshan B., Miles K.A., Young R.C.D., et. al.: Texture analysis in non-contrast enhanced CT: impact of malignancy on texture in apparently disease-free areas of the liver. Eur J Radiol 2009; 70: pp. 101-110.


- 20\. Thornhill R.E., Golfam M., Sheikh A., et. al.: Differentiation of lipoma from liposarcoma on MRI using texture and shape analysis. Acad Radiol 2014; 21: pp. 1185-1194.


- 21\. Bayanati H., Thornhill E., Souza C.A., et. al.: Quantitative CT texture and shape analysis: can it differentiate benign and malignant mediastinal lymph nodes in patients with primary lung cancer?. Eur Radiol 2015; 25: pp. 480-487.


- 22\. Andersen M.B., Harders S.W., Ganeshan B., et. al.: CT texture analysis can help differentiate between malignant and benign lymph nodes in the mediastinum in patients suspected for lung cancer. Acta Radiol 2016; 57: pp. 669-676.


- 23\. Hodgdon T., McInnes M.D., Schieda N., et. al.: Can quantitative CT texture analysis be used to differentiate fat-poor renal angiomyolipoma from renal cell carcinoma on unenhanced CT images?. Radiology 2015; 276: pp. 787-796.


- 24\. Schieda N., Thornhill R.E., Al-Subhi M., et. al.: Diagnosis of sarcomatoid renal cell carcinoma with CT: evaluation by qualitative imaging features and texture analysis. AJR Am J Roentgenol 2015; 204: pp. 1013-1023.


- 25\. Collewet G., Strzelecki M., Mariette F.: Influence of MRI acquisition protocols and image intensity normalization methods on texture classification. Magn Reson Imaging 2004; 22: pp. 81-91.


- 26\. Haralick R.M., Shanmugam K., Dinstein I.: Textural features for image classification. IEEE Trans Syst Man Cybern 1973; 3: pp. 610-621.


- 27\. DeLong E.R., DeLong D.M., Clarke-Pearson D.L.: Comparing the areas under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-845.


- 28\. Davnall F., Yip C.S., Ljunggvist G., et. al.: Assessment of tumor heterogeneity: an emerging imaging tool for clinical practice?. Insights Imaging 2012; 3: pp. 573-589.


- 29\. O'Connor J.P., Rose C.J., Waterton J.C., et. al.: Imaging intratumor heterogeneity: role in therapy response, resistance, and clinical outcome. Clin Cancer Res 2015; 21: pp. 249-257.


- 30\. Sureka B., Thukral B.B., Mittal M.K., et. al.: Radiological review of pleural tumors. Indian J Radiol Imaging 2013; 23: pp. 313-320.


- 31\. Ganeshan B., Panayiotou E., Burnand K., et. al.: Tumour heterogeneity in non-small cell lung carcinoma assessed by CT texture analysis: a potential marker of survival. Eur Radiol 2012; 22: pp. 796-802.


- 32\. Li H., Zhu Y., Burnside E.S., et. al.: MR imaging radiomics signatures for predicting the risk of breast cancer recurrence as given by research versions of MammaPrint, Oncotype DX, and PAM50 gene assays. Radiology 2016; 281: pp. 382-391.


- 33\. Wang H., Guo X.H., Jia Z.W., et. al.: Multilevel binomial logistic prediction model for malignant pulmonary nodules based on texture features of CT image. Eur J Radiol 2010; 74: pp. 124-129.


- 34\. Way T.W., Sahiner B., Chan H.P., et. al.: Computer-aided diagnosis of pulmonary nodules on CT scans: improvement of classification performance with nodule surface features. Med Phys 2009; 36: pp. 3086-3098.


- 35\. Kassner A., Thornhill R.E.: Texture analysis: a review of neurologic MR imaging applications. AJNR Am J Neuroradiol 2010; 31: pp. 809-816.


- 36\. Jordanov M., Bregman J., Montgomery K., Heidel M.: Curbside radiology consults: how does the time allotted for review, level of training, and subspecialization affect interpretation accuracy?. Clin Imaging 2015; 39: pp. 497-503.


- 37\. Yip S.S., Aerts H.J.: Applications and limitations of radiomics. Phys Med Biol 2016; 61: pp. R150-R166.


- 38\. Ravanelli M., Farina D., Morassi M., et. al.: Texture analysis of advanced non-small cell lung cancer (NSCLC) on contrast-enhanced computed tomography: prediction of the response to the first-line chemotherapy. Eur Radiol 2013; 23: pp. 3450-3455.