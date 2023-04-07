---
title: Looking Back at Prospective Studies
author: [CL_AT_CarolynMRutterPhD]
date: 2008-11-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 15, Issue 11]
tags: [Journals,General Radiology]
---
Gur's perspective article raises important points about analytic methods and the clinical inferences drawn from retrospective statistical analyses of prospective studies. Specifically, he associates three problems with the scientific methods of retrospective analyses: (1) using the parametric receiver-operating characteristic (ROC) curve and the area under the ROC curve (AUC) as a performance measure, (2) using Bonferroni adjustments to account for multiple comparisons, and (3) failing to evaluate the variability of results across sites and observers. Gur demonstrates these problems with a case study: a recent paper analyzing the Digital Mammographic Imaging Screening Trial (DMIST) ( ). The issues he raises are not specific to either retrospective study designs or secondary exploratory analyses of large studies but are important issues to consider in many design settings. I address each of these issues in the following and relate them to the information provided by DMIST papers.

## Problems with the ROC curve

The receiver-operating characteristic (ROC) curve plots the true-positive (TP) rate (sensitivity) on the y-axis against the false-positive (FP) rate (1 − specificity) on the x-axis to demonstrate the inherent trade-off between TP and FP rates ( ). The TP and FP rates increase together as test criteria are relaxed to allow more individuals to test positive. The area under the ROC curve (AUC) describes the average TP rate over the full, but often unobserved, range of FP rates (ie, 0 to 1). Because the AUC is based on the ROC curve over the entire FP range, a large fraction of the AUC can be based on FP regions that observed data do not support.

Many have criticized the use of the AUC as a summary measure and suggested the partial AUC (pAUC) as an alternative summary ( ), as does Gur. I agree that there are problems with the AUC, but I am not convinced that the pAUC offers an adequate solution for ordinal tests. The pAUC, which (when rescaled) represents the average TP rate over a selected range of FP values, has problems of its own. Most notably, using the pAUC requires selecting the corresponding FP range before observing the data. In addition, the pAUC does not account for differences in the observed FP range across tests being compared, leaving this criticism of AUC statistics unresolved. Because of these problems, the pAUC is not widely used for ordinal test outcomes. Instead, authors often make comparisons between tests using AUC statistics that capture the overall accuracy and supplement this overall comparison with (TP, FP) pairs that describe accuracy for selected test criteria. This was the approach taken in the DMIST paper ( ). Ideally, ROC curves would be presented, along with operating points, though space limitations sometimes preclude the inclusion of these graphs. In cases in which clinically relevant test criteria can be defined, it may make sense to design studies using TP and FP rates as primary outcomes and AUC statistics as secondary outcomes. The Breast Imaging Reporting and Data System (American College of Radiology, Reston, VA, 2003) ratings may offer such an example if ratings are dichotomized into those that indicate the need for additional imaging or surgical workup and those that do not.

Gur also points out that parametric ROC curves may have a “hook”: that is, estimated TP values that are less than FP values for some FP values near 1. This is a problem with parametric modeling approaches but not for nonparametric modeling approaches. Nonparametric models for ROC curves can be used either as the primary analytic approach or to explore potential problems with the parametric ROC curves. The DMIST paper reports the results from parametric ROC curve models that account for the paired study design ( ) and report using nonparametric analysis ( ) to corroborate their findings.

Finally, Gur suggests that the DMIST authors should have focused solely on comparing sensitivities. Problems with focusing solely on sensitivity and not acknowledging the inherent trade-off between sensitivity and specificity are well known and well documented in the diagnostic testing literature. This trade-off is the motivation for using ROC curve analysis. When examining screening tests, is especially important to account for the FP rates, given that the vast majority of people screened will not have the condition of interest. Post hoc comparisons, carried out only after large differences are observed can be misleading, because these tests are conditional on observed differences.

## Problems with adjustments for multiple comparisons

Gur points out problems using the Bonferroni correction for multiple tests. To place the multiple-comparison problem in context, first consider a single statistical test. The probability of a type I error—that is, rejecting the null hypothesis (eg, that there is no difference between digital and film mammography) when it is true—is set to a fixed value, α, and this is referred to as the α level of the test. Now consider _m_ independent tests, each performed with a type I error equal to α. In the literature on multiple testing, this may be referred to as a “family” of tests. The goal of adjusting for multiple tests is to control the overall probability of rejecting at least one of the tests in the family when all of the null hypotheses are true. For these _m_ independent tests, this family-wise error rate is 1 − (1 − α) _m_ . If α = .05 and _m_ = 25, the probability of a statistically significant finding when all of the null hypotheses are true rises to .72. Put another way, if we conducted 25 independent significance tests at the .05 level, where in each case the null hypothesis was true (ie, no differences existed), we would expect to reject at least one of the null hypotheses simply by chance. The Bonferroni adjustment is based on the Bonferroni inequality, which tells us that when all of the null hypotheses are true, the probability of rejecting at least one is less than or equal to _m_ α, and the correction is made by dividing the desired family-wise error rate by the number of tests. The Bonferroni approximation works well for families of independent statistical tests. The advantage of this approach is its simplicity and, therefore, transparency. The cost is power. The test can be conservative when the tests within the family are not independent, as is the case when the outcomes included in the family of tests are correlated.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reporting results from multisite studies

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Pisano E.D., Hendrick R.E., Yaffe M.J., et. al.: Diagnostic accuracy of digital versus film mammography: exploratory analysis of selected population subgroups in DMIST. Radiology 2008; 246: pp. 376-383.


- 2\. Obuchowski N.A.: Receiver operating characteristic curves and their use in radiology. Radiology 2003; 229: pp. 3-8.


- 3\. Hanley J.A., McNeil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 4\. Baker S.G.: The central role of receiver operating characteristic (ROC) curves in evaluating tests for the early detection of cancer. J Natl Cancer Inst 2003; 95: pp. 511-515.


- 5\. Dodd L.E., Pepe M.S.: Partial AUC estimation and regression. Biometrics 2003; 59: pp. 614-623.


- 6\. McClish D.K.: Analyzing a portion of the ROC curve. Med Decis Making 1989; 9: pp. 190-195.


- 7\. Thompson M.L., Zucchini W.: On the statistical analysis of ROC curves. Stat Med 1989; 8: pp. 1277-1290.


- 8\. Jiang Y., Metz C.E., Nishikawa R.M.: A receiver operating characteristic partial area index for highly sensitive diagnostic tests. Radiology 1996; 201: pp. 745-750.


- 9\. Baker S.G., Pinsky P.: A proposed design and analysis for comparing digital and analog mammography: special ROC methods for cancer screening. J Am Stat Assoc 2001; 96: pp. 421-428.


- 10\. Metz C., Wang P., Kronman H.: A new approach for testing the significance of differences between ROC curves measures from correlated data.Deconinck F.Information processing in medical imaging.1984.NijhoffThe Hague, The Netherlands:pp. 432-445.


- 11\. Zhou X.H., Obuchowski N.A., McClish D.: Statistical methods in diagnostic medicine.2002.John WileyNew York


- 12\. DeLong E.R., DeLong D.M., Clarke-Pearson D.L.: Comparing the areas under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-845.


- 13\. Toledano A.Y., Gatsonis C.: Generalized estimating equations for ordinal categorical data: arbitrary patterns of missing responses and missingness in a key covariate. Biometrics 1999; 55: pp. 488-496.


- 14\. Greenland S.: Multiple comparisons and association selection in general epidemiology. Int J Epidemiol 2008; 37: pp. 430-434.


- 15\.  Rothman KJ. No adjustments are needed for multiple comparisons. Epidemiology; 1:43–46.


- 16\. Greenland S., Robins J.M.: Empirical-Bayes adjustments for multiple comparisons are sometimes useful. Epidemiology 1991; 2: pp. 244-251.


- 17\. Poole C.: Multiple comparisons?. No problem! Epidemiology 1991; 2: pp. 241-243.


- 18\. Savitz D.A., Olshan A.F.: Multiple comparisons and related issues in the interpretation of epidemiologic data. Am J Epidemiol 1995; 142: pp. 904-908.


- 19\. Manor O., Peritz E.: Re: “Multiple comparisons and related issues in the interpretation of epidemiologic data.”. Am J Epidemiol 1997; 145: pp. 84-85.


- 20\. Thompson J.R.: Invited commentary: re: “Multiple comparisons and related issues in the interpretation of epidemiologic data.”. Am J Epidemiol 1998; 147: pp. 801-806.


- 21\. Goodman S.N.: Multiple comparisons, explained. Am J Epidemiol 1998; 147: pp. 807-812.


- 22\. Savitz D.A., Olshan A.F.: Describing data requires no adjustment for multiple comparisons: a reply from Savitz and Olshan. Am J Epidemiol 1998; 147: pp. 813-814.


- 23\. Benjamini Y., Hochberg Y.: Controlling the false discovery rate: a practical and powerful approach to multiple testing. J R Stat Soc Ser B 1995; 57: pp. 289-300.


- 24\. Goodman S.: Commentary: the p-value, devalued. Int J Epidemiol 2003; 32: pp. 699-702.


- 25\. Pisano E.D., Gatsonis C.A., Yaffe M.J., et. al.: American College of Radiology Imaging Network Digital Mammographic Imaging Screening Trial: objectives and methodology. Radiology 2005; 236: pp. 404-412.


- 26\. Elmore J.G., Miglioretti D.L., Reisch L.M., et. al.: Screening mammograms by community radiologists: variability in false-positive rates. J Natl Cancer Inst 2002; 94: pp. 1373-1380.