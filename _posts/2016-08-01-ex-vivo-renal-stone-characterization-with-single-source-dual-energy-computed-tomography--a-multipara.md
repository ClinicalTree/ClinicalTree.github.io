---
title: Ex Vivo Renal Stone Characterization with Single-Source Dual-Energy Computed Tomography: A Multiparametric Approach
author: [J. Scott Kriegshauser MD,Alvin C. Silva MD,Robert G. Paden MS,Miao He PhD,Mitchell R. Humphreys MD,Steven I. Zell MD,Yinlin Fu PhD,Teresa Wu PhD]
date: 2016-08-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 23, Issue 8 SOURCE CL_S_AcademicRadiologyVolume23Issue8 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We aimed to investigate a multiparametric approach using single-source dual-energy computed tomography (ssDECT) for the characterization of renal stones.

## Materials and Methods

ssDECT scans were performed at 80 and 140 kVp on 32 ex vivo kidney stones of 3–10 mm in a phantom. True composition was determined by infrared spectroscopy to be uric acid (UA; _n_ = 14), struvite ( _n_ = 7), cystine ( _n_ = 7), or calcium oxalate monohydrate ( _n_ = 4). Measurements were obtained for up to 52 variables, including mean density at 11 monochromatic keV levels, effective Z, and multiple material basis pairs. The data were analyzed with five multiparametric algorithms. After omitting 8 stones smaller than 5 mm, the remaining 24-stone dataset was similarly analyzed. Both stone datasets were also analyzed with a subset of 14 commonly used variables in the same fashion.

## Results

For the 32-stone dataset, the best method for distinguishing UA from non-UA stones was 97% accurate, and for distinguishing the non-UA subtypes was 72% accurate. For the 24-stone dataset, the best method for distinguishing UA from non-UA stones was 100% accurate, and for distinguishing the non-UA subtypes was 75% accurate.

## Conclusion

Multiparametric ssDECT methods can distinguish UA from non-UA stones of 5 mm or larger with 100% accuracy. The best model to distinguish the non-UA renal stone subtypes was 75% accurate. Further refinement of this multiparametric approach may increase the diagnostic accuracy of separating non-UA subtypes and assist in the development of a clinical paradigm for in vivo use.

## Introduction

Urinary stones are increasing in prevalence and can be associated with morbidities ranging from pain and obstruction to renal failure and sepsis . Management of urinary calculi is influenced not only by the size, number, and location of stones, but also by their underlying chemical composition .

Conventional computed tomography (CT) has been used to evaluate the size, number, and location of stones. When using Hounsfield unit (HU) analysis at a single energy level, however, CT has limited specificity in determining the underlying chemical composition because considerable overlap in HU values has been reported for different urinary stone compositions . The recent commercial availability of dual-energy CT (DECT) has allowed for further characterization of the chemical composition of stones by exploiting the ability to acquire and measure data at both 140 kV and 80 kV simultaneously . Single-source DECT (ssDECT) scanners use a fast kV–switch single X-ray source, which flips rapidly between high and low energies during the scan .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Variables Used


Variables_N_ Paired Materials  \\*  52-Variable set Mean 40–140 keV  †  11 NA Mean effective Z 1 NA CaOx pairs 4 Water, cystine, struvite, UA NaUrate pairs 3 Calcium, HAP, water Calcium pairs 6 Iodine, NaUrate, water, struvite, cystine, UA Struvite pairs 5 CaOx, calcium, water, cystine, UA Iodine pairs 3 Calcium, water, UA Cystine pairs 5 CaOx, calcium, water, struvite, UA HAP pair 1 NaUrate UA pairs 6 CaOx, calcium, iodine, water, cystine, struvite Water pairs 7 CaOx, calcium, iodine, NaUrate, cystine, struvite, UA 14-Variable set Mean 40–140 keV  †  11 NA Mean effective Z 1 NA Iodine pair 1 Water Water pair 1 Iodine

CaOx, calcium oxalate; HAP, hydroxyapatite; NA, not applicable; NaUrate, sodium urate; UA, uric acid.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Image representation of material pair decomposition. ( a–c ) Images of a 5-mm struvite stone viewed as a 70-keV monochromatic image ( a ), calcium (uric acid) basis pair ( b ), and uric acid (calcium) basis pair ( c ). Components of the struvite stone are projected into both basis dimensions. ( d–f ) Images of 4-mm and 6-mm uric acid stones viewed as a 70-keV monochromatic image ( d ), calcium (uric acid) basis pair ( e ), and uric acid (calcium) basis pair ( f ). Components of uric acid stones are fully projected into the uric acid basis for complete separation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ExVivoRenalStoneCharacterizationwithSingleSourceDualEnergyComputedTomographyAMultiparametricApproach/0_1s20S1076633216300083.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Decision Models


Name and Description Parameters ANN (Artificial Neural Network):

A classifier that uses back-propagation to classify instances. Similar to human brain structure, an ANN comprises an interconnected network of nodes and directed links. L (learning rate): 0.3

M (momentum): 0.2

N (number of epochs): 500

V (percentage size of validation set): 0

S (seed for random number generator): 0

E (threshold for number of consecutive errors): 20

H (comma-separated numbers for nodes on each layer): derived number, which is the average of the numbers of attributes and classes SVM (Support Vector Machine):

A classification method that can effectively perform nonlinear classification by first mapping the input data into high-dimensional feature space and then using an optimum linear hyperplane to separate two sets of data in the feature space. This optimum hyperplane is constructed by maximizing the margin of the two sets. C (complexity constant): 1

L (tolerance parameter): 0.001

P (epsilon for round-off error): 1.0 × 10  −12

N (whether to 0 = normalize/1 = standardize/2 = neither): 0

V (number of folds for the internal cross-validation): −1 (default setting using training data)

W (random number seed): 1

K (kernel to use): weka.classifiers.functions.supportVector.PolyKernel C4.5 (Decision Tree):

A classification algorithm that constructs decision trees in a top-down, recursive, divide-and-conquer manner. In a decision tree, every leaf node has an assigned class label. Attribute test conditions are used to separate records having different characteristics in the nonterminal nodes, which consist of the root node and other internal nodes. Decision trees, especially smaller-sized trees, are relatively easy to interpret. C (confidence threshold for pruning): 0.25

M (minimum number of instances per leaf): 2 RandomTree:

A classification algorithm that constructs multiple decision trees randomly. To construct each tree, the algorithm randomly picks a remaining (not used in previous nodes) feature at each node expansion. Each tree outputs a class probability distribution. The final class distribution is the average of outputs from multiple trees. K (number of attributes to randomly investigate): 0

M (minimum number of instances per leaf): 1

S (seed for random number generator): 1 NBTree (Naïve Bayes Tree):

A classifier for generating a decision tree with Naïve Bayes classifiers at the leaves. The Naïve Bayes classifier is based on the Bayes rule of conditional probability. None

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 3


Accuracy Distinguishing UA from Non-UA Stones  \\*

32-Stone Dataset 24-Stone Dataset Method 52 Variables 14 Variables 52 Variables 14 Variables ANN 97%(31) 97%(31) 100%(24) 100%(24) SVM 97%(31) 97%(31) 100%(24) 100%(24) C4.5 91%(29) 94%(30) 96%(23) 96%(23) RandomTree 94%(30) 97%(31) 100%(24) 100%(24) NBTree 97%(31) 94%(30) 100%(24) 100%(24)

ANN, Artificial Neural Network; C4.5, Decision Tree; NBTree, Naïve Bayes Tree; SVM, Support Vector Machine; UA, uric acid.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Box plot of the multiparametric accuracies for the five methods in distinguishing uric acid (UA) from non-UA stones. Note the limited scale of the y -axes (75%–100%). ( a ) 52 variables on 32-stone dataset ( best value ): Artificial Neural Network (ANN) ( 0.97 ), Support Vector Machine (SVM) ( 0.97 ), Decision Tree (C4.5) ( 0.91 ), RandomTree ( 0.94 ), and Naïve Bayes Tree (NBTree) ( 0.97 ). ( b ) 14 variables on 32-stone dataset: ANN ( 0.97 ), SVM ( 0.97 ), C4.5 ( 0.94 ), RandomTree ( 0.97 ), and NBTree ( 0.94 ). ( c ) 52 variables on 24-stone dataset: ANN ( 1 ), SVM ( 1 ), C4.5 ( 0.96 ), RandomTree ( 1 ), and NBTree ( 1 ). ( d ) 14 variables on 24-stone dataset: ANN ( 1 ), SVM ( 1 ), C4.5 ( 0.96 ), RandomTree ( 1 ), and NBTree ( 1 ). RandomTree is the recommended model for its perfomance and ease of clinical interpretation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ExVivoRenalStoneCharacterizationwithSingleSourceDualEnergyComputedTomographyAMultiparametricApproach/1_1s20S1076633216300083.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Accuracy Distinguishing Non-UA Stone Subtypes  \\*

18-Stone Dataset 12-Stone Dataset Method 52 Variables 14 Variables 52 Variables 14 Variables ANN 50%(9) 50%(9) 42%(5) 50%(6) SVM 44%(8) 44%(8) 42%(5) 42%(5) C4.5 33%(6) 39%(7) 33%(4) 33%(4) RandomTree 56%(10) 44%(8) 75%(9) 67%(8) NBTree 72%(13) 61%(11) 17%(2) 17%(2)

ANN, Artificial Neural Network; C4.5, Decision Tree; NBTree, Naïve Bayes Tree; SVM, Support Vector Machine; UA, uric acid.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Box plot of the multiparametric accuracies for the five methods in distinguishing non-uric acid stone subtypes. ( a ) 52 variables on 18-stone dataset ( best value ): Artificial Neural Network (ANN) ( 0.5 ), Support Vector Machine (SVM) ( 0.44 ), Decision Tree (C4.5) ( 0.33 ), RandomTree ( 0.56 ), and Naïve Bayes Tree (NBTree) ( 0.72 ). ( b ) 14 variables on 18-stone dataset: ANN ( 0.50 ), SVM ( 0.44 ), C4.5 ( 0.39 ), RandomTree ( 0.44 ), and NBTree ( 0.61 ). ( c ) 52 variables on 12-stone dataset: ANN ( 0.42 ), SVM ( 0.42 ), C4.5 ( 0.33 ), RandomTree ( 0.75 ), and NBTree ( 0.17 ). ( d ) 14 variables on 12-stone dataset: ANN ( 0.50 ), SVM ( 0.42 ), C4.5 ( 0.33 ), RandomTree ( 0.67 ), and NBTree ( 0.17 ). RandomTree is the recommended model for its perfomance and ease of clinical interpretation.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ExVivoRenalStoneCharacterizationwithSingleSourceDualEnergyComputedTomographyAMultiparametricApproach/2_1s20S1076633216300083.jpg)

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

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Stamatelou K.K., Francis M.E., Jones C.A., et. al.: Time trends in reported prevalence of kidney stones in the United States: 1976–1994. Kidney Int 2003; 63: pp. 1817-1823.


- 2\. Curhan G.C.: Epidemiology of stone disease. Urol Clin North Am 2007; 34: pp. 287-293.


- 3\. Romero V., Akpinar H., Assimos D.G.: Kidney stones: a global picture of prevalence, incidence, and associated risk factors. Rev Urol 2010; 12: pp. e86-e96.


- 4\. Pak C.Y., Poindexter J.R., Adams-Huet B., et. al.: Predictive value of kidney stone composition in the detection of metabolic abnormalities. Am J Med 2003; 115: pp. 26-32.


- 5\. Sakhaee K., Maalouf N.M., Sinnott B.: Clinical review: kidney stones 2012: pathogenesis, diagnosis, and management. J Clin Endocrinol Metab 2012; 97: pp. 1847-1860. Epub 2012 Mar 30


- 6\. Patel S.R., Haleblian G., Zabbo A., et. al.: Hounsfield units on computed tomography predict calcium stone subtype composition. Urol Int 2009; 83: pp. 175-180. Epub 2009 Sep 10


- 7\. Mostafavi M.R., Ernst R.D., Saltzman B.: Accurate determination of chemical composition of urinary calculi by spiral computerized tomography. J Urol 1998; 159: pp. 673-675.


- 8\. el-Assmy A., Abou-el-Ghar M.E., el-Nahas A.R., et. al.: Multidetector computed tomography: role in determination of urinary stones composition and disintegration with extracorporeal shock wave lithotripsy: an in vitro study. Urology 2011; 77: pp. 286-290. Epub 2010 Aug 16


- 9\. Coursey C.A., Nelson R.C., Boll D.T., et. al.: Dual-energy multidetector CT: how does it work, what can it tell us, and when can we use it in abdominopelvic imaging?. Radiographics 2010; 30: pp. 1037-1055.


- 10\. Ascenti G., Siragusa C., Racchiusa S., et. al.: Stone-targeted dual-energy CT: a new diagnostic approach to urinary calculosis. AJR Am J Roentgenol 2010; 195: pp. 953-958.


- 11\. Hidas G., Eliahou R., Duvdevani M., et. al.: Determination of renal stone composition with dual-energy CT: in vivo analysis and comparison with X-ray diffraction. Radiology 2010; 257: pp. 394-401. Epub 2010 Aug 31


- 12\. Manglaviti G., Tresoldi S., Guerrer C.S., et. al.: In vivo evaluation of the chemical composition of urinary stones using dual-energy CT. AJR Am J Roentgenol 2011; 197: pp. W76-W83.


- 13\. Stolzmann P., Kozomara M., Chuck N., et. al.: In vivo identification of uric acid stones with dual-energy CT: diagnostic performance evaluation in patients. Abdom Imaging 2010; 35: pp. 629-635. Epub 2009 Sep 2


- 14\. Thomas C., Patschan O., Ketelsen D., et. al.: Dual-energy CT for the characterization of urinary calculi: in vitro and in vivo evaluation of a low-dose scanning protocol. Eur Radiol 2009; 19: pp. 1553-1559. Epub 2009 Feb 10


- 15\. Zilberman D.E., Ferrandino M.N., Preminger G.M., et. al.: In vivo determination of urinary stone composition using dual energy computerized tomography with advanced post-acquisition processing. J Urol 2010; 184: pp. 2354-2359. Epub 2010 Oct 16


- 16\. Graser A., Johnson T.R., Bader M., et. al.: Dual energy CT characterization of urinary calculi: initial in vitro and clinical experience. Invest Radiol 2008; 43: pp. 112-119.


- 17\. Kulkarni N.M., Eisner B.H., Pinho D.F., et. al.: Determination of renal stone composition in phantom and patients using single-source dual-energy computed tomography. J Comput Assist Tomogr 2013; 37: pp. 37-45.


- 18\. Boll D.T., Patil N.A., Paulson E.K., et. al.: Renal stone assessment with dual-energy multidetector CT and advanced postprocessing techniques: improved characterization of renal stone composition: pilot study. Radiology 2009; 250: pp. 813-820.


- 19\. Primak A.N., Fletcher J.G., Vrtiska T.J., et. al.: Noninvasive differentiation of uric acid versus non-uric acid kidney stones using dual-energy CT. Acad Radiol 2007; 14: pp. 1441-1447.


- 20\. Qu M., Ramirez-Giraldo J.C., Leng S., et. al.: Dual-energy dual-source CT with additional spectral filtration can improve the differentiation of non-uric acid renal stones: an ex vivo phantom study. AJR Am J Roentgenol 2011; 196: pp. 1279-1287.


- 21\. Stolzmann P., Leschka S., Scheffel H., et. al.: Characterization of urinary stones with dual-energy CT: improved differentiation using a tin filter. Invest Radiol 2010; 45: pp. 1-6.


- 22\. Stolzmann P., Scheffel H., Rentsch K., et. al.: Dual-energy computed tomography for the differentiation of uric acid stones: ex vivo performance evaluation. Urol Res 2008; 36: pp. 133-138. Epub 2008 Jun 11


- 23\. Thomas C., Krauss B., Ketelsen D., et. al.: Differentiation of urinary calculi with dual energy CT: effect of spectral shaping by high energy tin filtration. Invest Radiol 2010; 45: pp. 393-398.


- 24\. Hartman R., Kawashima A., Takahashi N., et. al.: Applications of dual-energy CT in urologic imaging: an update. Radiol Clin North Am 2012; 50: pp. 191-205. Epub 2012 Mar 7


- 25\. Li X., Zhao R., Liu B., et. al.: Gemstone spectral imaging dual-energy computed tomography: a novel technique to determine urinary stone composition. Urology 2013; 81: pp. 727-730. Epub 2013 Feb 26


- 26\. Wisenbaugh E.S., Paden R.G., Silva A.C., et. al.: Dual-energy vs conventional computed tomography in determining stone composition. Urology 2014; 83: pp. 1243-1247. Epub 2014 Feb 16


- 27\. Silva A.C., Morse B.G., Hara A.K., et. al.: Dual-energy (spectral) CT: applications in abdominal imaging. Radiographics 2011; 31: pp. 1031-1046.


- 28\. Goodsitt M.M., Christodoulou E.G., Larson S.C.: Accuracies of the synthesized monochromatic CT numbers and effective atomic numbers obtained with a rapid kVp switching dual energy CT scanner. Med Phys 2011; 38: pp. 2222-2232.


- 29\. Berger M.J., Hubbell J.H., Seltzer S.M., et. al.: XCOM: photon cross sections database: NIST Standard reference database 8 (XGAM) \[Internet\]. Available at: http://www.nist.gov/pml/data/xcom/ Accessed October 21, 2014


- 30\. Hall M., Frank E., Holmes G., et. al.: The WEKA data mining software: an update. SIGKDD Explorations Newsletter \[Internet\]. 2009;11(1):10–18; Available at: http://www.cms.waikato.ac.nz/~ml/publications/2009/weka\_update.pdf Accessed October 21, 2014


- 31\. Eliahou R., Hidas G., Duvdevani M., et. al.: Determination of renal stone composition with dual-energy computed tomography: an emerging application. Semin Ultrasound CT MR 2010; 31: pp. 315-320.


- 32\. Schubert G.: Stone analysis. Urol Res 2006; 34: pp. 146-150. Epub 2006 Feb 14


- 33\. Lieske J.C., Pena de la Vega L.S., Slezak J.M., et. al.: Renal stone epidemiology in Rochester, Minnesota: an update. Kidney Int 2006; 69: pp. 760-764.


- 34\. Qu M., Yu L., Cardona D.G., et. al.: Radiation dose reduction in dual-energy CT: does it affect the accuracy of urinary stone characterization?. AJR Am J Roentgenol 2015; 205: pp. W172-W176.