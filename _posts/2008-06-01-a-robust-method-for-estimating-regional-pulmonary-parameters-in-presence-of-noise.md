---
title: A Robust Method for Estimating Regional Pulmonary Parameters in Presence of Noise
author: [CL_AT_RichardAGuyerBA,CL_AT_MichaelDHellmanBS,CL_AT_KiarashEmamiMS,CL_AT_StephenKadlecekPhD,CL_AT_RobertVCadmanPhD,CL_AT_JiangshengYuMS,CL_AT_VahidVadhatMS,CL_AT_MasaruIshiiMDPhD,CL_AT_JohnMacDuffieWoodburnMS,CL_AT_MichelleLawBA,CL_AT_RahimRRiziPhD]
date: 2008-06-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 15, Issue 6]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Estimation of regional lung function parameters from hyperpolarized gas magnetic resonance images can be very sensitive to presence of noise. Clustering pixels and averaging over the resulting groups is an effective method for reducing the effects of noise in these images, commonly performed by grouping proximal pixels together, thus creating large groups called “bins.” This method has several drawbacks, primarily that it can group dissimilar pixels together, and it degrades spatial resolution. This study presents an improved approach to simplifying data via principal component analysis (PCA) when noise level prohibits a pixel-by-pixel treatment of data, by clustering them based on similarity to one another rather than spatial proximity. The application to this technique is demonstrated in measurements of regional lung oxygen tension using hyperpolarized  3 He magnetic resonance imaging (MRI).

## Materials and Methods

A synthetic dataset was generated from an experimental set of oxygen tension measurements by treating the experimentally derived parameters as “true” values, and then solving backwards to generate “noiseless” images. Artificial noise was added to the synthetic data, and both traditional binning and PCA-based clustering were performed. For both methods, the root-mean-square (RMS) error between each pixel's “estimated” and “true” parameters was computed and the resulting effects were compared.

## Results

At high signal-to-noise ratios (SNRs), clustering did not enhance accuracy. Clustering did, however, improve parameter estimations for moderate SNR values (below 100). For SNR values between 100 and 20, the PCA-based K-means clustering analysis yielded greater accuracy than Cartesian binning. In extreme cases (SNR < 5), Cartesian binning can be more accurate.

## Conclusions

The reliability of parameters estimation in imaging-based regional functional measurements can be improved in the presence of noise by utilizing principal component analysis-based clustering without sacrificing spatial resolution compared to Cartesian binning. Results suggest that this approach has a great potential for robust grouping of pixels in hyperpolarized  3 He MRI maps of lung oxygen tension.

Pulmonary disorders such as emphysema, asthma, and acute respiratory distress syndrome are among the most common illnesses in the world; asthma alone is estimated to afflict 150 million people globally and costs the Untied States over $6 billion each year ( ). Emphysema may impact over 3% of the United States population, which is more than 9 million people ( ). Because the lung is a large and heterogeneous organ, these conditions can be difficult to diagnose clinically. It is thus important to develop sensitive radiologic techniques for regional measurement of lung function to assist physicians in diagnosing such diseases.

Functional lung imaging using hyperpolarized gas magnetic resonance imaging (HP gas MRI) allows various pulmonary parameters to be assessed regionally (3). This method is safe and does not deliver ionizing radiation to patients. Patients inhale hyperpolarized helium-3 (  3 He) or xenon-129 (  129 Xe), and images of the airspaces are subsequently acquired. Signal intensity in each region of the lungs is directly related to the degree of polarization of the gas and the amount of gas that is present in that region. The images can be postprocessed to reveal physiologic information. HP gas MRI allows researchers to rigorously assess a wide range of pulmonary parameters, such as regional ventilation ( ), the regional alveolar partial pressure of oxygen (P  A O  2 ) ( ), and the apparent diffusion coefficient (ADC) of gasses, which is linked to the size of the alveoli and structure of small airway ( ), turning them into powerful tools for diagnosing and studying lung diseases.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Theory

## Measurement of Regional Oxygen Tension

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ΓO2=PAO2ξ,
Γ

O

2

=

P

A

O

2

ξ

,


where _ξ_ = 2.6 bar · s at body temperature. The decay rate, however, is different for each region, and is a function of local P  A O  2 and ODR. Theoretically, this relation is given by the following equation for the _n_ -th image in the sequence ( ):


S(n)=S(0)⋅exp\[M⋅n⋅ln(cos(α))−1ξ(PAO2⋅t(n)−12ODR⋅t2(n))\],
S

(

n

)

=

S

(

0

)

·

e

xp

\[

M

·

n

·

ln

⁡

(

cos

⁡

(

α

)

)

−

1

ξ

(

P

A

O

2

·

t

(

n

)

−

1

2

ODR

·

t

2

(

n

)

)

\]

,


where _S_ (0) indicates the original signal intensity in each region. In general the interscan time delay _t_ ( _n_ ) can be an arbitrary function of the image number _n_ . In the case of equally spaced images, _t_ ( _n_ ) = τ · _n_ , where τ is the time interval between each pair of images. The form of Equation  2 follows from the common approximation that uptake of oxygen into the blood stream can be expressed as a linear function:


PAO2(t)=PAO2(0)−ODR⋅t
P

A

O

2

(

t

)

=

P

A

O

2

(

0

)

−

O

DR

·

t


where P  A O  2 (0) denotes oxygen partial pressure at the beginning of the breathhold ( _t_ = 0). If two images are obtained with no—or negligible with respect to Γ  O2 —interscan time delay in each slice at the beginning of the image series, they can be used to fairly accurately calculate the flip angle in each region of the lung by analyzing the signal decay induced by RF pulse. Subsequent images are obtained at longer time intervals, and are used to calculate signal decay caused by oxygen. The time evolution of P  A O  2 ( _t_ ) and ODR( _t_ ) values at acquisition times can therefore be obtained in this manner from a single series of images acquired during one single breathhold ( ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Formation of the Data Space

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Principal Component Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

B=X−u⋅h
B

=

X

−

u

⋅

h


where _h_ is a 1 × N vector of all ones. Next, the covariance matrix _C_ is computed and its unit eigenvectors _V__n_ (1 ≤ _n_ ≤ A) are determined, as are their corresponding eigenvalues _l__n_ . _C_ is given by:


C=1A−1B⋅B\*,
C

=

1

A

−

1

B

·

B

\*

,


where \* represents the conjugate transpose operation. The eigenvectors are sorted in decreasing order of eigenvalues _l_ . By theorem, these unit eigenvectors are orthogonal to one another, and they define a space identical to the data space ( ). The eigenvector corresponding to the highest eigenvalue is the first principal component, and the following eigenvectors represent the remaining principal components in decreasing order of eigenvalues. Also, the eigenvalue of the _n_ -th principal component tells us what proportion _P_ of the variation in the data it describes, as given by the identity:


P=λnλ1+⋅⋅⋅+λN.
P

=

λ

n

λ

1

+

⋅

⋅

⋅

+

λ

N

.


We assume that projecting all our data points into the two-dimensional space defined by the first two principal components effectively eliminates variation in the data due to insignificant variables, although this property cannot be universally assumed. The desired result is a lower dimension data space in which noise effects has been reduced. Clustering points in this reduced data space can theoretically allow parameters estimations to be performed with less uncertainty in presence of noise.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Clustering—Cartesian Binning and K-means

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

v=∑ki=1∑xj∈Si∣∣xj−μi\|2,
v

=

∑

i

=

1

k

∑

x

j

∈

S

i

\|

x

j

−

μ

i

\|

2

,


where each _S__i_ is a cluster with the centroid _μ__i_ . Objects are moved between clusters until _v_ is minimized. The theoretical result is a set of clusters that are as compact and separated as possible.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Helium-3 Polarization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Animal Preparation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Oxygen Tension Measurement Experiment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Imaging Protocol

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Synthetic Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

SNR=1NS2−N2,−−−−−−−−√
S

N

R

=

1

N

S

2

−

N

2

,


where _S_ is the signal intensity of the pixel, and _N_ is the bias-corrected noise level in the image ( ):


N=2π⋅Nˆ.−−−−−−√
N

=

2

π

·

N

^

.


The unbalanced noise, Nˆ
N

^
, is estimated by averaging the intensity of a group of pixels in an area of the image in which no MR signal is present, away from the actual lung tissue. Pixels not exceeding an SNR = 3 in the first image of the series were excluded in the synthetic dataset. The synthetic data was only generated for a single slice near the middle of the lung that contained the trachea.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Principal Component Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Data Clustering

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Noise Simulations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison of Clustering Techniques

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Experimental Data and Synthetic Images

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, A time-series of 3He lung images acquired in a healthy rabbit during a breathhold. The signal decay, largely caused by collisions with oxygen molecules, is analyzed to yield the concentration (P A O 2 ) and uptake rate (ODR) of oxygen into the bloodstream.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ARobustMethodforEstimatingRegionalPulmonaryParametersinPresenceofNoise/0_1s20S1076633208001785.jpg)

![Figure 2, The last in a series of eight images used to test the relative merits of principal-component analysis and clustering. (a) The synthetic “noise-free” image derived from experimental data. (b–d) The same image with Rician noise added to achieve an SNR of 100:1 (b) , 10:1 (c) , and 3:1 (d) , respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ARobustMethodforEstimatingRegionalPulmonaryParametersinPresenceofNoise/1_1s20S1076633208001785.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Principal Component Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Relative magnitudes of the information (variance) explained by each of the eight principal components (PCs) in the data space. Note that the first two PCs contain virtually all of the information in the dataset analyzed in this study, allowing significant simplification of the data space by omitting the other six components.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ARobustMethodforEstimatingRegionalPulmonaryParametersinPresenceofNoise/2_1s20S1076633208001785.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Oxygen Parameter Estimation in the Synthetic Dataset

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, P A O 2 values for the “true” noiseless case derived from the synthetic dataset (a) , and three estimations at an SNR of 20:1 (b–d) . Frame (b) displays the estimation in an unfiltered and unclustered case on a pixel-by-pixel basis, frame (c) displays the results when forming 2 × 2 spatial bins, and frame (d) displays the results of K-means clustering in a PCA/EVD-simplified data space with 192 clusters. A visual inspection shows that the PCA-based method is most similar to the true case. Loss of spatial information increases as the bin size increases beyond the minimal binning shown here. The remaining frames (e–h) depict the corresponding effect of filtering schemes on the derived oxygen uptake rate (ODR). The unlabeled, black and white image to the left depicts the first image in the series with its simulated noise.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ARobustMethodforEstimatingRegionalPulmonaryParametersinPresenceofNoise/3_1s20S1076633208001785.jpg)

![Figure 5, P A O 2 values derived as shown in Figure 4 , but with 16 × 16 Cartesian binning. This results in six unmasked bins. For comparison, a PCA/EVD-simplified dataset is shown using the same number of clusters. In both cases, significant physiologically relevant information is lost through the simplification, but anatomic detail remains in the latter case. (a) This depicts fit to the “noise-free” dataset, and (b–d) are unfiltered, spatially binned, and PCA/EVD-simplified images, respectively.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ARobustMethodforEstimatingRegionalPulmonaryParametersinPresenceofNoise/4_1s20S1076633208001785.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Evolution of root-mean-square (RMS) error between “true” P A O 2 values and estimated values of the entire oxygen map in the lung, generated from 50 random noise level simulations in each case. The RMS error evolution for the unfiltered case ( dotted ), Cartesian binning ( dashed ), and PCA-based K-means clustering ( solid ) is shown. Frames (a–f) are for estimations performed with 192, 58, 17, 6, 4, and 1 clusters, respectively. Error bars were too small to aid visual analysis. Units on the y -axis are in millibars.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ARobustMethodforEstimatingRegionalPulmonaryParametersinPresenceofNoise/5_1s20S1076633208001785.jpg)

![Figure 7, Evolution of root-mean-square (RMS) error between “true” oxygen uptake rate (ODR) values and estimated values of the entire oxygen map in the lung, generated from 50 random noise level simulations in each case. The RMS error evolution for the unfiltered case ( dotted ), Cartesian binning ( dashed ), and PCA-based K-means clustering ( solid ) is shown. Frames (a–f) are for estimations performed with 192, 58, 17, 6, 4, and 1 clusters, respectively. Error bars were too small to aid visual analysis. Units on the y -axis are in millibars per second.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ARobustMethodforEstimatingRegionalPulmonaryParametersinPresenceofNoise/6_1s20S1076633208001785.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

## Principal Component Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Oxygen Parameter Estimation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Number of Clusters

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Potential Clinical Applications

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Study Limitations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Cookson W.: The alliance of genes and environment in asthma and allergy. Nature 1999; 402: pp. B5-B11.


- 2\. Boutin-Forzano S., Moreau D., Kalaboka S., et. al.: Reported prevalence and co-morbidity of asthma, chronic bronchitis and emphysema: a pan-European estimation. Int J Tuberc Lung Dis 2007; 11: pp. 695-702.


- 3\. Ishii M., Fischer M.C., Emami K., et. al.: Hyperpolarized  3  He MR imaging of pulmonary function. Radiol Clin North Am 2005; 43: pp. 235-246.


- 4\. Deninger A.J., Månsson S., Petersson J.S., et. al.: Quantitative measurement of regional lung ventilation using  3  He MRI. Magn Reson Med 2002; 48: pp. 223-232.


- 5\. Deninger A.J., Eberle B., Ebert M., et. al.: Quantification of regional intrapulmonary oxygen partial pressure evolution during apnea by (3)He MRI. J Magn Reson 1999; 141: pp. 207-216.


- 6\. Fain S.B., Panth S.R., Evans M.D., et. al.: Early emphysematous changes in asymptomatic smokers: detection with  3  He MR imaging. Radiology 2006; 239: pp. 875-883.


- 7\. Fischer M.C., Spector Z.Z., Ishii M., et. al.: Single-acquisition sequence for the measurement of oxygen partial pressure by hyperpolarized gas MRI. Magn Reson Med 2004; 52: pp. 766-773.


- 8\. Fischer M.C., Kadlecek S., Yu J., et. al.: Measurements of regional alveolar oxygen pressure using hyperpolarized  3  He MRI. Acad Radiol 2005; 12: pp. 1430-1439.


- 9\. Shiga M., Takigawa I., Mamitsuka H.: Annotating gene function by combining expression data with a modular gene network. Bioinformatics 2007; 23: pp. i468-i478.


- 10\. Banada P.P., Guo S., Bayraktar B., et. al.: Optical forward-scattering for detection of Listeria monocytogenes and other Listeria species. Biosense Bioelectron 2007; 22: pp. 1664-1671.


- 11\. Wang Z., Wang J., Calhoun V., et. al.: Strategies for reducing large fMRI data sets for independent component analysis. Magn Reson Imaging 2006; 24: pp. 591-596.


- 12\. Goutte C., Hansen L.K., Liptrot M.G., et. al.: Feature-space clustering for fMRI meta-analysis. Hum Brain Mapp 2001; 13: pp. 165-183.


- 13\. Goutte C., Toft P., Rostrup E., et. al.: On clustering fMRI time series. Neuroimage 1999; 9: pp. 298-310.


- 14\. Kimura Y., Hsu H., Toyama H., et. al.: Improved signal-to-noise ratio in parametric images by cluster analysis. Neuroimage 1999; 9: pp. 554-561.


- 15\. Kimura Y., Senda M., Alpert N.M.: Fast formation of statistically reliable FDG parametric images based on clustering and principal components. Phys Med Biol 2002; 47: pp. 455-468.


- 16\. Layfield D., Venegas J.G.: Enhanced parameter estimation from noisy PET data: Part I–methodology. Acad Radiol 2005; 12: pp. 1440-1447.


- 17\. Yu J., Ishii M., Kadlecek S., et. al.: Multiple regression method for pulmonary apparent diffusion coefficient measurement by hyperpolarized  3  He MRI. J Magn Reson Imaging 2007; 25: pp. 982-991.


- 18\.  MATLAB Statistics Toolbox, User's Guide, 5th Ed. Natick, MA: MathWorks, 2004.


- 19\. Lay D.: Linear Algebra and its Applications.2003.Addison WesleyNew York, NY


- 20\. Ding C., Xe H.: K-means clustering via principal component analysis. Proc Int'l Conf Machine Learning 2004; pp. 225-232.


- 21\. Gudbjartsson H., Patz S.: The Rician distribution of noisy MRI data. Magn Reson Med 1995; 34: pp. 910-914.


- 22\. Venegas J.G., Winkler T., Musch G., et. al.: Self-Organized Patchiness in Asthma as a Prelude to Catastrophic Shifts. Nature 2005; 434: pp. 777-782.


- 23\. Roberts D.A., Rizi R.R., Lipson D.A., et. al.: Detection and localization of pulmonary air leaks using laser-polarized (3)He MRI. Magn Reson Med 2000; 44: pp. 379-382.