---
title: A Comparative Study of HRCT Image Metrics and PFT Values for Characterization of ILD and COPD
author: [CL_AT_GangSongMS,CL_AT_EduardoMortaniBarbosaMD,CL_AT_NicholasTustisonDSc,CL_AT_WarrenBGefterMD,CL_AT_MarylKreiderMDMSCE,CL_AT_JamesCGeePhD,CL_AT_DrewATorigianMDMA]
date: 2012-07-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 7]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The aim of this study was to compare the performance of various image-based metrics computed from thoracic high-resolution computed tomography (HRCT) with data from pulmonary function testing (PFT) in characterizing interstitial lung disease (ILD) and chronic obstructive pulmonary disease (COPD).

## Materials and Methods

Fourteen patients with ILD and 11 with COPD had undergone both PFT and HRCT within 3 days. For each patient, 93 image-based metrics were computed, and their relationships with the 21 clinically used PFT parameters were analyzed using a minimal-redundancy-maximal-relevance statistical framework. The first 20 features were selected among the total of 114 mixed image metrics and PFT values in the characterization of ILD and COPD.

## Results

Among the best-performing 20 features, 14 were image metrics, derived from attenuation histograms and texture descriptions. The highest relevance value computed from PFT parameters was 0.47, and the highest from image metrics was 0.52, given the theoretical bound as \[0, 0.69\]. The ILD or COPD classifier using the first four features achieved a 1.92% error rate.

## Conclusions

Some image metrics are not only as good discriminators as PFT for the characterization of ILD and COPD but are also not redundant when PFT values are provided. Image metrics of attenuation histogram statistics and texture descriptions may be valuable for further investigation in computer-assisted diagnosis.

Chronic lung disease constitutes a major worldwide public health care problem and is the fourth leading cause of morbidity and mortality in the United States . On the basis of clinical, imaging, and pathologic characteristics, most types of chronic lung disease can be grouped into two basic categories: interstitial lung disease (ILD) and chronic obstructive pulmonary disease (COPD). ILD is a heterogeneous group of diseases in which the hallmark is chronic, progressive, predominantly interstitial inflammation with varying degrees of fibrosis of the lung parenchyma, often leading to reduced lung volume, decreased lung compliance, and restrictive physiology. COPD is characterized by chronic airflow limitation due to airway inflammation and lung parenchymal destruction that is not fully reversible and is usually progressive.

The diagnosis, differentiation, and classification of the severity of ILD and COPD rely on clinical assessment, thoracic imaging (using computed tomography and chest radiography), and pulmonary function testing (PFT). PFT is a noninvasive method of assessing the integrated mechanical function of the lung, chest wall, and respiratory muscles. It is the current reference standard for pulmonary functional assessment. Using PFT, the heterogeneous group of ILDs typically exhibit a restrictive physiology pattern, whereas COPD typically manifests an obstructive physiology pattern.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Statistics of Patients with ILD ( _n_ = 14)


Variable Value Gender Female 8 Male 6 Age (y) Mean 56.1 Standard deviation 12.0 Median 56 Degree of PFT restriction Normal 3 Mild 3 Moderate 4 Severe 2 Moderately severe 1 Very severe 1

ILD, interstitial lung disease; PFT, pulmonary function testing.


Table 2


Statistics of Patients with COPD ( _n_ = 11)


Variable Value Gender Female 6 Male 5 Age (y) Mean 53.1 Standard deviation 7.7 Median 54 Degree of PFT restriction Normal 0 Mild 3 Moderate 1 Severe 3 Very severe 4

COPD, chronic obstructive pulmonary disease; PFT, pulmonary function testing.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Pipeline of the proposed feature selection analysis. COPD, chronic obstructive pulmonary disease; ILD, interstitial lung disease; mRMR, minimal-redundancy-maximal-relevance; PFT, pulmonary function testing; SVM, support vector machine.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AComparativeStudyofHRCTImageMetricsandPFTValuesforCharacterizationofILDandCOPD/0_1s20S1076633212001493.jpg)

Table 3


Computed Image Metrics and Their Relevance to the Disease Types


Number Metric Type (Reference) G1 G2 G3 Attenuation histogram indices 1 Lung region volume  0.325 0.276 0.073 2 Relative volume  <-910  0.439 0.454 0.071 3 Attenuation mean  0.416 0.407 0.181 4 Attenuation variance  0.171 0.197 0.181 5 Sum  0.295 0.353 0.005 6 Attenuation skewness  0.276 0.159 0.026 7 Attenuation kurtosis  0.392 0.201 0.079 8 Attenuation gray level entropy  0.021 0.121 0.005 9 5% attenuation value  0.47 0.527 0.353 10 95% attenuation value  0.463 0.22 0.006 11 5% attenuation mean  0.488 0.416 0.036 12 95% attenuation mean  0.055 0.065 0.071 Co-occurrence matrix indices 13 Energy  0.019 0.05 0.05 14 Entropy  0.159 0.215 0.159 15 Correlation  0.003 0.001 0.002 16 Inverse difference moment  0.021 0.121 0.025 17 Inertia  0.003 0.022 0.005 18 Cluster shade  0.083 0.021 0.074 19 Cluster prominence  0.113 0.074 0.104 20 Haralick's correlation  0.034 0.034 0.001 Run-length matrix indices 21 Short run emphasis  0.049 0.002 0.002 22 Long run emphasis  0.074 0.002 0.002 23 Gray level nonuniformity  0.243 0.316 0.007 24 Run-length nonuniformity  0.325 0.353 0.006 25 Run percentage  0.157 0.101 0.101 26 Low gray level run emphasis  0.285 0.157 0.113 27 High gray level run emphasis  0.005 0.114 0.005 28 Short run low gray level emphasis  0.285 0.157 0.058 29 Short run high gray level emphasis  0.005 0.114 0.005 30 Long run low gray level emphasis  0.285 0.157 0.113 31 Long run high gray level emphasis  0.005 0.114 0.005

G1 denotes the metrics computed from the expiratory images and G2 those from the inspiratory images. Metrics of G3 were generated by subtracting G1 from G2. Within each of G1, G2, and G3, the metrics were indexed from 1 to 31. The values in the last three columns are the relevance values to the disease types of interstitial lung disease and chronic obstructive pulmonary disease.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## PFT Parameters and Image Metrics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


All 21 PFT Values (First and Third Rows) and Corresponding Relevance Values (Second and Fourth Rows) to the Disease Types


PFT FVC FEV  1  FEV  1  /FVC FEF max FEF 25–75% FEF50 FIF50 MVV SVC IC ERV Relevance 0.088 0.026 0.47 0.357 0.218 0.307 0.021 0.251 0.197 0.083 0.146 PFT TGV RV (Pleth) TLC (Pleth) RV/TLC DLCO unc DLCO cor DL/VA VA Raw sGaw Relevance 0.268 0.268 0.35 0.218 0.041 0.15 0.066 0.269 0.101 0.074

DLCOcor, corrected carbon monoxide diffusion; DLCOunc, uncorrected carbon monoxide diffusion; DL/VA, carbon monoxide diffusion corrected for alveolar volume; ERV, expiratory reserve volume; FEF25–75%, forced expiratory flow at 25% and 75% of forced vital capacity; FEF50, forced expiratory flow at 50% of forced vital capacity; FEV  1  , forced expiratory volume in 1 second; FIF50, forced expiratory flow at 50% of forced vital capacity; IC, inspiratory capacity; FVC, forced vital capacity; max, maximum; MVV, maximum voluntary ventilation; PFT, pulmonary function testing; Raw, airway resistance; RV (Pleth), residual volume on plethysmography; sGaw, specific airway conductance; SVC, slow vital capacity; TGV, thoracic gas volume; TLC (Pleth), total lung capacity on plethysmography; VA, alveolar volume.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Feature Selection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

I(zi,c)=∬p(zi,c)logp(zi,c)p(zi)p(c)dzidc.
I

(

z

i

,

c

)

=

∬

p

(

z

i

,

c

)

log

p

(

z

i

,

c

)

p

(

z

i

)

p

(

c

)

d

z

i

d

c

.


The relevance measure _I_ ( _z__i_ , _c_ ) shows the amount of information that knowing the feature _z__i_ can provide to classify the disease type _c_ . This relevance value is always nonnegative. If two variables _z__i_ and _c_ are independent, which means that _z__i_ provides no information in predicting _c_ , their relevance is zero. If the value of _z__i_ is totally determined by _c_ , _z__i_ and _c_ are not independent, and their relevance becomes the entropy of _c_ , which is a measure of the uncertainty associated with _c_ . Also, the maximal relevance is bounded by the greater of the entropies of _z__i_ and _c_ . Note that the maximum entropy for all possible binary distributions is obtained from the uniform distribution as log(2). This gives the upper bound for _I_ ( _z__i_ , _c_ ) as log(2) = 0.69.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

S=argmaxS⫅Z{∑zi∈SI(zi,c)−1∥S∥∑zi,zj∈SI(zi,zj)}.
S

=

arg

max

S

⫅

Z

{

∑

z

i

∈

S

I

(

z

i

,

c

)

−

1

‖

S

‖

∑

z

i

,

z

j

∈

S

I

(

z

i

,

z

j

)

}

.


The first term in equation  1 maximizes the total relevance of the selected features with the corresponding disease types; the second term minimizes the total redundancy of all pairs of the selected features. The framework in Peng et al gives a heuristic way to optimize equation  1 . We use the online toolbox to compute the relevance weights and select features.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classification with SVMs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

w⋅x−b{≥0forthepositiveclass<0forthenegativeclass.
w

⋅

x

−

b

{

≥

0

for

the

positive

class

<

0

for

the

negative

class

.


The parameters **w** and _b_ are learned from the training samples to maximize the margins between hyperplanes that separates data points of two classes. An example of a linear SVM using two features is illustrated in two dimensions in  Figure 2 a. In this two-dimensional case, the two features for each data point are its _x_ and _y_ coordinates, and the separating plane is a straight line. Note that the linear SVM is unable to classify all the data points correctly using a straight line.

![Figure 2, Illustration of support vector machines (SVMs) on a synthetic two-dimensional data set. Each data point has its x and y coordinates as two features. Type I points are marked with red dots and type II points with blue crosses . SVM hyperplanes are shown in green . Note that type I points cannot be separated from type II points by any straight lines. (a) The linear kernel SVM misclassifies several points, marked with circles. (b) The radial basis function kernel SVM classifies all the points with a curve as classification hyperplane.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AComparativeStudyofHRCTImageMetricsandPFTValuesforCharacterizationofILDandCOPD/1_1s20S1076633212001493.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Experiment Setup

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Relevance (mutual information) of image metrics to different disease types. The x axis has the image metrics index listed in Table 3 . Red bars are for metrics from G1, the expiratory (exp) images; blue bars for G2, the inspiratory (insp) images; and green bars for G3, the difference of G1 to G2.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AComparativeStudyofHRCTImageMetricsandPFTValuesforCharacterizationofILDandCOPD/2_1s20S1076633212001493.jpg)

![Figure 4, Relevance (mutual information) of pulmonary function testing (PFT) values to different disease types. The x axis lists all 21 PFT values in Table 4 . Note that the range of the y axis is similar to the range from those image metrics in Figure 3. DLCOcor, corrected carbon monoxide diffusion; DLCOunc, uncorrected carbon monoxide diffusion; DL/VA, carbon monoxide diffusion corrected for alveolar volume; ERV, expiratory reserve volume; FEF, forced expiratory flow; FEF25–75%, forced expiratory flow at 25% and 75% of forced vital capacity; FEF50, forced expiratory flow at 50% of forced vital capacity; FEV 1 , forced expiratory volume in 1 second; FIF50, forced inspiratory flow at 50% of forced vital capacity; FVC, forced vital capacity; IC, inspiratory capacity; max, maximum; MVV, maximum voluntary ventilation; Raw, airway resistance; RV (Pleth), residual volume on plethysmography; sGaw, specific airway conductance; SVC, slow vital capacity; TGV, thoracic gas volume; TLC (Pleth), total lung capacity on plethysmography; VA, alveolar volume.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AComparativeStudyofHRCTImageMetricsandPFTValuesforCharacterizationofILDandCOPD/3_1s20S1076633212001493.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Classifying interstitial lung disease and chronic obstructive pulmonary disease using the first k = 1 to 20 selected features with (a) the linear support vector machine (SVM) and (b) the radial basis function SVM, using maximum relevance (MaxRel) or minimal-redundancy-maximal-relevance (mRMR) on pulmonary function testing (PFT) values, image metrics, or both PFT values and image metrics. For each curve, the x axis is the number of selected features for training and testing with SVMs; the y axis is the average error rate from leave-one-out tests. One subject is excluded when learning SVM parameters, and that subject is used to test the accuracy of the trained SVM.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AComparativeStudyofHRCTImageMetricsandPFTValuesforCharacterizationofILDandCOPD/4_1s20S1076633212001493.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


The First 20 Selected Features from mRMR on Both PFT Values and Image Metrics


Rank Feature 1 G1: attenuation mean 2 G1: lung region volume 3 G1: sum 4 FEV  1  /FVC 5 G1: run length nonuniformity 6 TGV 7 G1: 95% attenuation value 8 FEF max 9 FEF50 10 G1: relative volume  <-950  11 G3: mean 12 FEF25–75% 13 RV (Pleth) 14 G2: mean 15 G2: run length nonuniformity 16 FEF  1  17 G1: 5% attenuation mean 18 G2: 95% attenuation mean 19 G2: sum 20 G2: relative volume  <-950

FEF, forced expiratory flow; FEF  1  , forced expiratory flow in 1 second; FEF25–75%, forced expiratory flow at 25% and 75% of forced vital capacity; FEV  1  , forced expiratory volume in 1 second; FVC, forced vital capacity; max, maximum; mRMR, minimal-redundancy-maximal-relevance; PFT, pulmonary function testing; RV (Pleth), residual volume on plethysmography; TGV, thoracic gas volume.


Note these features include both PFT values and image metrics. The image metrics includes both the first-order statistical measurements obtainable from the attenuation histogram and other more sophisticated metrics of texture descriptions. G1 denotes the metrics computed from the expiratory images and G2 those from the inspiratory images. Metrics of G3 were generated by subtracting G1 from G2.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Receiver-operating characteristic curves for using different values to separate interstitial lung disease and chronic obstructive pulmonary disease. The green curve uses the ratio of forced expiratory volume in 1 second (FEV 1 ) to forced vital capacity (FVC). The red curve uses the radial basis function support vector machine (SVM) scores computed from the first 10 features selected by minimal-redundancy-maximal-relevance. SVMs are trained and tested using the leave-one-out strategy. FPR, false-positive rate; TPR, true-positive rate.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AComparativeStudyofHRCTImageMetricsandPFTValuesforCharacterizationofILDandCOPD/5_1s20S1076633212001493.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Xu J., Kochanek K., Murphy S., et. al.: Deaths: final data for 2007. Natl Vital Stat Rep 2010; 58: pp. 1-134.


- 2\. Müller N.L., Staples C.A., Miller R.R., et. al.: “Density mask.” An objective method to quantitate emphysema using computed tomography. Chest 1988; 94: pp. 782-787.


- 3\. Gevenois P.A., De Vuyst P., Sy M., et. al.: Pulmonary emphysema: quantitative CT during expiration. Radiology 1996; 199: pp. 825-829.


- 4\. Lamers R.J., Kemerink G.J., Drent M., et. al.: Reproducibility of spirometrically controlled CT lung densitometry in a clinical setting. Eur Respir J 1998; 11: pp. 942-945.


- 5\. Xu Y., Sonka M., McLennan G., et. al.: MDCT-based 3-D texture classification of emphysema and early smoking related lung pathologies. IEEE Trans Med Imaging 2006; 25: pp. 464-475.


- 6\. Zaporozhan J., Ley S., Eberhardt R., et. al.: Paired inspiratory/expiratory volumetric thin-slice CT scan for emphysema analysis: comparison of different quantitative evaluations and pulmonary function test. Chest 2005; 128: pp. 3212-3220.


- 7\. Coxson H.O., Rogers R.M., Whittall K.P., et. al.: A quantification of the lung surface area in emphysema using computed tomography. Am J Respir Crit Care Med 1999; 159: pp. 851-856.


- 8\. Stavngaard T., Shaker S.B., Bach K.S., et. al.: Quantitative assessment of regional emphysema distribution in patients with chronic obstructive pulmonary disease (COPD). Acta Radiol 2006; 47: pp. 914-921.


- 9\. Madani A., Zanen J., de Maertelaer V., et. al.: Pulmonary emphysema: objective quantification at multi-detector row CT—comparison with macroscopic and microscopic morphometry. Radiology 2006; 238: pp. 1036-1043.


- 10\. Temizoz O., Etlik O., Sakarya M.E., et. al.: Detection and quantification of the parenchymal abnormalities in emphysema using pulmo-CT. Comput Med Imaging Graph 2007; 31: pp. 542-548.


- 11\. Washko G.R., Criner G.J., Mohsenifar Z., et. al.: Computed tomographic-based quantification of emphysema and correlation to pulmonary function and mechanics. COPD 2008; 5: pp. 177-186.


- 12\. Park Y.S., Seo J.B., Kim N., et. al.: Texture-based quantification of pulmonary emphysema on high-resolution computed tomography: comparison with density-based quantification and correlation with pulmonary function test. Invest Radiol 2008; 43: pp. 395-402.


- 13\. Song G., Barbosa E., Tustison N., et. al.: Computational analysis of HRCT images for characterization and differentiation of ILD and COPD.IEEE International Symposium on Biomedical Imaging: From Nano to Macro 2009.2009.IEEEPiscataway, NJ:pp. 999-1002.


- 14\. Vapnik V.: The Nature of Statistical Learning Theory.2nd ed.1999.SpringerNew York


- 15\. Peng H., Long F., Ding C.: Feature selection based on mutual information: criteria of max-dependency, max-relevance, and min-redundancy. IEEE Trans Pattern Anal Mach Intell 2005; 27: pp. 1226-1238.


- 16\. Haralick R.M., Shanmugam K., Dinstein I.: Textural features for image classification. IEEE Trans Syst Man Cybern 1973; 3: pp. 610-621.


- 17\. Dasarathy B.V., Holder E.B.: Image characterizations based on joint gray level-run length distributions. Pattern Recogn Lett 1991; 12: pp. 497-502.


- 18\. Hu S., Hoffman E.A., Reinhardt J.M.: Automatic lung segmentation for accurate quantitation of volumetric X-ray CT images. IEEE Trans Med Imaging 2001; 20: pp. 490-498.


- 19\.  Peng H. mRMR (minimum redundancy maximum relevance feature selection). Available from:  http://penglab.janelia.org/proj/mRMR/  . Accessed December 21, 2011.


- 20\. Schlkopf B., Smola A.J.: Learning with Kernels: Support Vector Machines, Regularization, Optimization, and Beyond.2001.MIT PressCambridge, MA