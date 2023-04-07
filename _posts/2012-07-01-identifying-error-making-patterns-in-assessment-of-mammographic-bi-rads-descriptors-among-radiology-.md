---
title: Identifying Error-making Patterns in Assessment of Mammographic BI-RADS Descriptors among Radiology Residents Using Statistical Pattern Recognition
author: [CL_AT_MaciejAMazurowskiPhD,CL_AT_HuimanXBarnhartPhD,CL_AT_JayABakerMD,CL_AT_GeorgiaDTourassiPhD]
date: 2012-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 7]
tags: [Journals,General Radiology]
---
## Rationale and Objective

The objective of this study is to test the hypothesis that there are patterns in erroneous assessment of BI-RADS features among radiology trainees when interpreting mammographic masses and that these patterns can be captured in individualized statistical user models. Identifying these patterns could be useful in personalizing and adapting educational material to complement the individual weaknesses of each trainee during his or her mammography education.

## Materials and Methods

Reading data of 33 mammographic cases containing masses was used. The cases were individually described by 10 radiology residents using four BI-RADS features: mass shape, mass margin, mass density and parenchyma density. For each resident, an individual model was automatically constructed that predicts likelihood (HIGH or LOW) of erroneously assigning each BI-RADS descriptor by the resident. Error was defined as deviation of the resident's assessment from the expert assessments. We evaluated the predictive performance of the models using leave-one-out crossvalidation.

## Results

The user models were able to predict which assessments have higher likelihood of error. The proportion of actual errors to the number of situations in which these errors could potentially occur was significantly higher ( _P_ < .05) when user-model assigned HIGH likelihood of error than when LOW likelihood of error was assigned for three of the four BI-RADS features. Overall, the difference between the HIGH and LOW likelihood of error groups was statistically significant ( _P_ < .0001) combining all four features.

## Conclusion

Error making in BI-RADS descriptor assessment appears to follow patterns that can be captured with statistical pattern recognition-based user models.

Over the years, mammography has proven to be an effective tool for breast cancer screening. When combined with adjuvant therapy, mammography can notably reduce the rate of death from breast cancer . However, the diagnostic interpretation of mammograms is a challenging task for radiologists, and substantial inter-observer variability in performance has been reported . As a potential solution to this problem, it has been shown that specialized training can significantly contribute to improving the radiologists' performance . Most of the training in interpretation of mammograms takes place in the radiology residency years through lectures, interaction with expert breast imagers and supervised analysis of mammograms. However, computerized training tools hold promise to significantly contribute to the traditional approach to radiology education .

In our recent study we proposed the general framework for a new adaptive computer-aided radiology training system. The system addresses the common drawback of existing online training tools: their “one-size-fits-all” approach. Online training tools available today present the same material to all trainees independent of their individual needs, strengths, and weaknesses.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Database

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Error in BI-RADS Feature Assessment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## User Models

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

p(T)(V=v\|R≠v)≥p(Overall)(V=v\|R≠v)
p

(

T

)

(

V

=

v

\|

R

≠

v

)

≥

p

(

O

v

e

r

a

l

l

)

(

V

=

v

\|

R

≠

v

)


group(T)(v)=HIGH
group

(

T

)

(

v

)

=

HIGH


**ELSE**

group(T)(v)=LOW
group

(

T

)

(

v

)

=

LOW


**END**

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

p(Overall)(v)=∑10T=1p(T)(V=v\|R≠v)10
p

(

O

v

e

r

a

l

l

)

(

v

)

=

∑

T

=

1

10

p

(

T

)

(

V

=

v

\|

R

≠

v

)

10


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Diagram illustrating construction of one rule in a user model: the analyzed BI-RADS descriptor is “shape” and the analyzed value of the descriptor is “oval”. In this illustration, assessments of 8 example cases were made. Green boxes represent correct assessments of the descriptor. Red boxes represent erroneous assessments of the descriptor. Bold outline represents cases for each the descriptors assigned by experts did not include “oval”.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IdentifyingErrormakingPatternsinAssessmentofMammographicBIRADSDescriptorsamongRadiologyResidentsUsingStatisticalPatternRecognition/0_1s20S1076633212000517.jpg)

![Figure 2, An example user model. For each descriptor value, the likelihood of error is as follows: dark red = very high likelihood of error, light red = high likelihood of error, green = low likelihood of error.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IdentifyingErrormakingPatternsinAssessmentofMammographicBIRADSDescriptorsamongRadiologyResidentsUsingStatisticalPatternRecognition/1_1s20S1076633212000517.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Experimental Design and Statistical Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

∑Nv=1p(V=v\|R≠v)⋅wi∑Nv=1wi=∑Nv=1(n(V=v\|R≠v)n(R≠v)⋅wi)∑Nv=1wi
∑

v

=

1

N

p

(

V

=

v

\|

R

≠

v

)

·

w

i

∑

v

=

1

N

w

i

=

∑

v

=

1

N

(

n

(

V

=

v

\|

R

≠

v

)

n

(

R

≠

v

)

·

w

i

)

∑

v

=

1

N

w

i


where


wi=n(R≠v)
w

i

=

n

(

R

≠

v

)


and


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Overall percentages of error among (a) the residents and (b) the BI-RADS features. Percentage of error for a resident is defined as the total number of errors made in individual assessments of all features divided by the total number of such assessments and multiplied by 100. Percentage of error for a feature is defined as the total number of times the error was made by the residents while assigning the feature divided by the total number of times a value was assigned to the feature and multiplied by 100.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/IdentifyingErrormakingPatternsinAssessmentofMammographicBIRADSDescriptorsamongRadiologyResidentsUsingStatisticalPatternRecognition/2_1s20S1076633212000517.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Fitted Percents of Errors (95% Confidence Interval from GEE Models) Made by the Residents in the Two Groups Determined by the Predicted Likelihood of Error along with the Corresponding p-values. For Each Feature (e.g. Mass Margin), the Presented Values are Proportions of Errors of a Certain Type (e.g. Erroneously Assigning Value “Spiculated”) to the Number of Opportunities of Making Such Error (Situations when the True Descriptor is not “Spiculated”) Averaged across All Possible Values of that Feature and Pooled across All Residents. A Weighted Average was Used with Weights for Each Type of Error Equal the Total Number of Situations when Such Type of Error Could Potentially be Made. The Values are Multiplied by 100 to Express the Percent Values.


Predicted Likelihood of Error HIGH LOW_P_ -value (HIGH vs. LOW) BI-RADS Feature**Mass margin** 9.30 (5.79 14.62) 6.49 (4.53 9.21) 0.1251**Mass shape** 9.16 (6.21 13.33) 2.37 (1.13 4.90) 0.0030**Mass density** 15.22 (10.45 21.64) 0.33 (0.08 1.25) 0.0003**Parenchyma density** 8.99 (5.08 15.43) 2.28 (1.38 3.75) 0.0116**Overall** 10.09 (8.13 12.45) 2.82 (2.19 3.61) < 0.0001

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

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

## References

- 1\. Berry D.A., Cronin K.A., Plevritis S.K., et. al.: Effect of screening and adjuvant therapy on mortality from breast cancer. N Engl J Med Oct 2005; 353: pp. 1784-1792.


- 2\. Elmore J.G., Wells C.K., Lee C.H., et. al.: Variability in radiologists' interpretations of mammograms. N Engl J Med Dec 1994; 331: pp. 1493-1499.


- 3\. Linver M.N., Paster S.B., Rosenberg R.D., et. al.: Improvement in mammography interpretation skills in a community radiology practice after dedicated teaching courses: 2-year medical audit of 38,633 cases. Radiology Jul 1992; 184: pp. 39-43.


- 4\. Leung J.W.T., Margolin F.R., Dee K.E., et. al.: Performance parameters for screening and diagnostic mammography in a community practice: are there differences between specialists and general radiologists?. AJR Am J Roentgenol Jan 2007; 188: pp. 236-241.


- 5\. Scarsbrook A.F., Graham R.N.J., Perriss R.W.: Radiology education: a glimpse into the future. Clin Radiol Aug 2006; 61: pp. 640-648.


- 6\. Mazurowski M.A., Baker J.A., Barnhart H.X., et. al.: Individualized computer-aided education in mammography based on user modeling: concept and preliminary experiments. Med Phys Mar 2010; 37: pp. 1152-1160.


- 7\. 1998.American College of Radiology


- 8\. Berg W.A., D'Orsi C.J., Jackson V.P., et. al.: Does training in the Breast Imaging Reporting and Data System (BI-RADS) improve biopsy recommendations or feature analysis agreement with experienced breast imagers at mammography?. Radiology Sep 2002; 224: pp. 871-880.


- 9\. Rich E.: Users are individuals:- individualizing user models. Int. J. Man-Machine Studies 1983; 18: pp. 199-214.


- 10\. Fisher G.: User Modeling in Human–Computer Interaction. User Modeling and User-Adapted Interaction 2001; 11: pp. 65-86.


- 11\. Webb G.I., Pazzani M.J., Billsus D.: Machine Learning for User Modeling. User Modeling and User-Adapted Interaction 2001; 11: pp. 19-29.


- 12\. Brusilovsky P., Millan E.: User Models for Adaptive Hypermedia and Adaptive Educational Systems. The Adaptive Web, LNCS 2007; 4321: pp. 3-53.


- 13\. Zukerman I., Albrecht D.W.: Predictive Statistical Models for User Modeling. User Modeling and User-Adapted Interaction 2001; 11: pp. 5-18.


- 14\.  Sun S, Taylor P, Wilkinson L, et al. An Ontology to Support Adaptive Training for Breast Radiologists 2008:257–264.


- 15\. Sun S., Taylor P., Wilkinson L., et. al.: Individualised Training to Address Variability of Radiologists' Performance. SPIE Medical Imaging 2008; Vol 6917: 69170G. Available at: http://spie.org/x648.html?product\_id=770296

- 16\. Yap M.H., Gale A.G., Scott H.J.: Generic Infrastructure for Medical Informatics (GIMI): The Development of a Mammographic Training System. Proceedings of the International Workshop on Digital Mammography 2008; pp. 577-584.


- 17\. Yap M.H., Gale A.G.: Individualized grid-enabled mammographic training system. Proceedings of SPIE: Medical Imaging 2009; Vol 7264: 72640V. Available at: http://www.springerlink.com/content/k6647728104t4537/

- 18\.  Mazurowski MA, Tourassi GD. Modeling error in assessment of mammographic image features for improved computer-aided mammography training: initial experience. Paper presented at: SPIE Medical Imaging (in press) 2011.


- 19\. Singh S., Maxwell J., Baker J.A., et. al.: Computer-aided Classification of Breast Masses: Performance and Interobserver Variability of Expert Radiologists versus Residents. Radiology 2011; 258: pp. 73-80.


- 20\. Baker J.A., Kornguth P.J., Floyd C.E.: Breast imaging reporting and data system standardized mammography lexicon: observer variability in lesion description. AJR Am J Roentgenol Apr 1996; 166: pp. 773-778.