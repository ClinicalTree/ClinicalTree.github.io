---
title: Automated Patient Identity Recognition by Analysis of Chest Radiograph Features
author: [CL_AT_EFongKaoPhD,CL_AT_WeiChenLinMD,CL_AT_TweiShiunJawMD,CL_AT_GinChungLiuMD,CL_AT_JainShingWuPhD,CL_AT_ChungNanLeePhD]
date: 2013-08-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 20, Issue 8]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to develop a computerized scheme for automated identity recognition based on chest radiograph features.

## Materials and Methods

The proposed method was evaluated on a database consisting of 1000 pairs of posteroanterior chest radiographs. The method was based on six features: length of the lung field, size of the heart, area of the body, and widths of the upper, middle, and lower thoracic cage. The values for the six features were determined from a chest image, and absolute differences in feature values between the two images (feature errors) were used as indices of image similarity. The performance of the proposed method was evaluated by receiver operating characteristic (ROC) analysis. The discriminant performance was evaluated as the area Az under the ROC curve.

## Results

The discriminant performance Az of the feature errors for lung field length, heart size, body area, upper cage width, middle cage width, and lower cage width were 0.794 ± 0.005, 0.737 ± 0.007, 0.820 ± 0.008, 0.860 ± 0.005, 0.894 ± 0.006, and 0.873 ± 0.006, respectively. The combination of the six feature errors obtained an Az value of 0.963 ± 0.002.

## Conclusion

The results indicate that combining the six features yields a high discriminant performance in recognizing patient identity. The method has potential usefulness for automated identity recognition to ensure that chest radiographs are associated with the correct patient.

Patient identity recognition is an important procedure when radiographic examinations are performed. Taking a radiograph with a wrong patient sometimes happens due to the heavy workload of radiologic technologists in examination rooms. Minimizing such errors is an important issue. Among all radiographic examinations, chest examinations are performed most frequently. It is helpful to alert radiologic technologists when a chest examination performed with a wrong patient occurs. The examination can be repeated on the spot, and the further problems can be prevented. This is especially worthwhile for outpatients who leave the hospital after seeing a physician.

The major works related to patient identification using chest radiographs have been performed by Morishita et al, including the first automated patient recognition method based on image-matching technique . The proposed method determined the similarity between two images by calculating correlation values between two chest images. The authors further brought up an idea about automated patient recognition using biological fingerprints in chest radiographs . The biological fingerprints included thoracic field, cardiac shadow, lung apex, superior mediastinum, right lung, and right lower lung in the study. After determining the correlation value between two subimages of each biological fingerprint, the discriminant performance of each biological fingerprint was analyzed. In another prospective study, the authors evaluated the effectiveness of a method based on image-matching technique in a clinical environment .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Image Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Features Used to Recognize Patient Identity

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Top of Thoracic Cage

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

V(y)=∑Xleft\_lungx=Xright\_lungI(x,y)
V

(

y

)

=

∑

x

=

X

r

i

g

h

t

\_

l

u

n

g

X

l

e

f

t

\_

l

u

n

g

I

(

x

,

y

)


![Figure 1, (a) Determining the top of the thoracic cage in a chest radiograph. (b) The P (x) is the horizontal projection profile of the image. (c) The V(y) is the vertical projection profile obtained by summing the pixel values of the image along the x direction between X right_lung and X left_lung .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/0_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Length of Lung Field

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Llunglength=\|Ybottom−Ytop\|
L

l

u

n

g

l

e

n

g

t

h

=

\|

Y

b

o

t

t

o

m

−

Y

t

o

p

\|


![Figure 2, (a) Determining the bottom of the lung field in a chest radiograph. (b) The v(y) is the vertical profile at X right_lung . (c) The v′(y) is the first derivative of v(y) . The bottom of the lung field is determined by finding the minimum from v′(y) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/1_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Size of Heart

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, (a) Determining heart size in a chest radiograph. (b) The V(y) is the vertical projection profile obtained by summing the pixel values of the image between ( X right_lung + X center )/2 and X left_lung along the x direction. (c) The h(x) is the horizontal profile at Y widest . The size of the heart is determined from h(x) by threshold.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/2_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Area of Body

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Abodyarea=Nbody×pixelsize
A

b

o

d

y

a

r

e

a

=

N

b

o

d

y

×

p

i

x

e

l

s

i

z

e


![Figure 4, (a) Histogram of chest image in Figure 1 a. (b) Binary image obtained by thresholding the chest image using G threshold .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/3_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Width of Thoracic Cage

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, (a) Widths of upper, middle, and lower thoracic cage. (b) A typical horizontal profile used for determining the thoracic cage widths.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/4_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation Method

## Errors of feature values

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Errlunglength=∣∣Llunglength(A)−Llunglength(B)∣∣
E

r

r

l

u

n

g

l

e

n

g

t

h

=

\|

L

l

u

n

g

l

e

n

g

t

h

(

A

)

−

L

l

u

n

g

l

e

n

g

t

h

(

B

)

\|


Errheartsize=∣∣Lheartsize(A)−Lheartsize(B)∣∣
E

r

r

h

e

a

r

t

s

i

z

e

=

\|

L

h

e

a

r

t

s

i

z

e

(

A

)

−

L

h

e

a

r

t

s

i

z

e

(

B

)

\|


Errbodyarea=∣∣Abodyarea(A)−Abodyarea(B)∣∣
E

r

r

b

o

d

y

a

r

e

a

=

\|

A

b

o

d

y

a

r

e

a

(

A

)

−

A

b

o

d

y

a

r

e

a

(

B

)

\|


Erruppercage=∣∣Luppercage(A)−Luppercage(B)∣∣
E

r

r

u

p

p

e

r

c

a

g

e

=

\|

L

u

p

p

e

r

c

a

g

e

(

A

)

−

L

u

p

p

e

r

c

a

g

e

(

B

)

\|


Errmiddlecage=∣∣Lmiddlecage(A)−Lmiddlecage(B)∣∣
E

r

r

m

i

d

d

l

e

c

a

g

e

=

\|

L

m

i

d

d

l

e

c

a

g

e

(

A

)

−

L

m

i

d

d

l

e

c

a

g

e

(

B

)

\|


Errlowercage=∣∣Llowercage(A)−Llowercage(B)∣∣
E

r

r

l

o

w

e

r

c

a

g

e

=

\|

L

l

o

w

e

r

c

a

g

e

(

A

)

−

L

l

o

w

e

r

c

a

g

e

(

B

)

\|


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Combination of Six Feature Errors

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, (a) Schematic representation of the distributions of feature error for the same and different identities. (b) Similarity value in terms of feature error.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/5_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

S={(Meandifferent−Err)/Meandifferent0ifErr≤MeandifferentifErr>Meandifferent
S

=

{

(

M

e

a

n

d

i

f

f

e

r

e

n

t

−

E

r

r

)

/

M

e

a

n

d

i

f

f

e

r

e

n

t

i

f

E

r

r

≤

M

e

a

n

d

i

f

f

e

r

e

n

t

0

i

f

E

r

r

>

M

e

a

n

d

i

f

f

e

r

e

n

t


where _Err_ is feature error and where _Mean__differen_ t is the average of feature error for different identities.  Figure 6 b schematically presents similarity value in terms of feature error. Using Equation 10, each feature error can be transformed into a value between 0 and 1. This general idea can be applied to all six feature errors, and S values were obtained for each set of feature errors ( _S__lung length_ , _S__heart size_ , _S__body area_ , _S__upper cage_ , _S__middle cage_ , and _S__lower cage_ ). The combination of the six feature errors can be represented by a similarity score calculated using Equation 11.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Scoresimilarity=Slunglength+Sheartsize+Sbodyarea+Suppercage+Smiddlecage+Slowercage
S

c

o

r

e

s

i

m

i

l

a

r

i

t

y

=

S

l

u

n

g

l

e

n

g

t

h

+

S

h

e

a

r

t

s

i

z

e

+

S

b

o

d

y

a

r

e

a

+

S

u

p

p

e

r

c

a

g

e

+

S

m

i

d

d

l

e

c

a

g

e

+

S

l

o

w

e

r

c

a

g

e


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discriminant Performance Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Feature error distributions for (a) lung field length, (b) heart size, (c) body area, (d) upper thoracic cage width, (e) middle thoracic cage width, and (f) lower thoracic cage width.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/6_1s20S1076633213002183.jpg)

Table 1


Means and Standard Deviations of Feature Errors for the Same and Different Identities


Same Identity ( _n_ = 1000) Different Identities ( _n_ = 999,000)_Err__Lung length_ (cm) 1.10 ± 1.66 3.05 ± 2.46_Err__heart size_ (cm) 0.98 ± 1.48 2.02 ± 1.84_Err__body area_ (cm  2  ) 11.88 ± 15.34 51.17 ± 45.51_Err__upper cage_ (cm) 0.40 ± 0.50 1.78 ± 1.48_Err__middle cage_ (cm) 0.39 ± 0.52 2.25 ± 1.78_Err__lower cage_ (cm) 0.57 ± 0.70 2.83 ± 2.18

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, Distributions of Score similarity for the same and different identities.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/7_1s20S1076633213002183.jpg)

Table 2


Means and Standard Deviations of _Score__similarity_ for the Same and Different Identities


Same Identity ( _n_ = 1000) Different Identities ( _n_ = 999,000)_Score__similarity_ 4.53 ± 0.84 1.90 ± 1.18

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Discriminant Performance of Similarity Score and Feature Errors


Az ( _n_ = 10)_Score__similarity_ 0.963 ± 0.002_Err__Lung length_ 0.794 ± 0.005_Err__heart size_ 0.737 ± 0.007_Err__body area_ 0.820 ± 0.008_Err__upper cage_ 0.860 ± 0.005_Err__middle cage_ 0.894 ± 0.006_Err__lower cage_ 0.873 ± 0.006

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Low Score similarity values for two images for the same patient identity resulted from (a) insufficient inhalation, (b) gross opacity abnormalities, and (c) incorrect identification of the top of the thoracic cage.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/8_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Example of chest images for two different patient identities that obtained a high Score similarity value.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedPatientIdentityRecognitionbyAnalysisofChestRadiographFeatures/9_1s20S1076633213002183.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Morishita J., Katsuragawa S., Kondo K., et. al.: An automated patient recognition method based on an image-matching technique using previous chest radiographs in the picture archiving and communication system environment. Med Phys 2001; 28: pp. 1093-1097.


- 2\. Morishita J., Katsuragawa S., Sasaki Y., et. al.: Potential usefulness of biological fingerprints in chest radiographs for automated patient recognition and identification. Acad Radiol 2004; 11: pp. 309-315.


- 3\. Morishita J., Watanabe H., Katsuragawa S., et. al.: Investigation of misfiled cases in the PACS environment and a solution to prevent filing errors for chest radiographs. Acad Radiol 2005; 12: pp. 97-103.


- 4\. Kao E.F., Lee C., Hsu J.S., et. al.: Projection profile analysis for automated detection of abnormalities in chest radiographs. Med Phys 2006; 33: pp. 118-123.


- 5\. Kao E.F., Kuo Y.T., Hsu J.S., et. al.: Zone-based analysis for automated detection of abnormalities in chest radiographs. Med Phys 2011; 38: pp. 4241-4250.


- 6\. Hanley J.A., McNeil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 7\. Metz C.E.: Basic principles of ROC analysis. Semin Nucl Med 1978; 8: pp. 283-298.


- 8\. Bontrager K.L.: Textbook of Radiographic Positioning and Related Anatomy.2001.MosbySt. Louis, MO