---
title: dr-ROC, Summary ROC Meta-Analysis Software, Version 2.0
author: [John D. Carew PhD]
date: 2007-06-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 6 SOURCE CL_S_AcademicRadiologyVolume14Issue6 1}]
tags: [Journals,General Radiology]
---
Summary ROC Meta-Analysis Software, dr-ROC, is a highly specialized Microsoft Excel workbook file for meta-analysis of diagnostic tests. This software is best suited for a statistically minded investigator who aims to assess the utility of a diagnostic test from a collection of reports on the test’s sensitivity and specificity. Typically, these reports would come from a literature review. The standard version of the software is limited to 25 or fewer studies. A version that handles up to 100 studies is available, free of charge, to licensees who contact the publisher. Key strengths of dr-ROC include an easy-to-use complete, self-contained solution for meta-analysis and automatic generation of publication quality graphics. A previous version of the software was recently reviewed ( ).

The statistical methodology of dr-ROC is based on the summary receiver operating characteristic (ROC) approach to meta-analysis ( ). Users of the software need to have a good understanding of this method, including assumptions, interpretation of results, and how to appropriately choose the software options. The software manual does not include a tutorial. Additionally, some terms and variables are not clearly defined or not defined at all. A glossary would be helpful. The publisher will provide, on request, a “Lesson Plan and Student Guide.” This document is essentially an outline of topics for a course in meta-analysis of diagnostic tests. Not included is training on the statistical aspects of meta-analysis.

Data input to dr-ROC is performed in the first page of the Excel workbook. Results from each independent study are reported in a single row. The results include the numbers of true positives (TPs), false negatives (FNs), false positives (FPs), and true negatives (TNs). One can also assign a quality score to each study and provide user-specified weights. Other weighting options are none (default), inverse variance, and the total number of subjects in each study. To accommodate studies where TPs, FNs, FPs, or TNs have values of 0, a “continuity correction” is applied. This involves adding 0.5 to each of the TPs, FNs, FPs, and TNs. These and other options are specified with pop-up menus that appear on the “Input” worksheet. Computations are started by pressing “Go.” For the eight example studies included with the software, the calculations and graphs were generated in a few seconds.

Numeric output appears in the “Results” and “Table” worksheets. This includes mean threshold, analysis parameters, regression parameters (for fitting the ROC curve), area under the ROC curve, and several other parameters. One convenient feature of the “Results” worksheet is that 95% confidence intervals are included for all estimated quantities. Intermediate calculations that are used to produce what is included on the “Results” sheet are available as described in the manual. The “Table” worksheet summarizes the results from all studies used in the meta-analysis as well as the estimated sensitivity, specificity, positive predictive value, and negative predictive value (all at mean threshold) from the meta-analysis. One can paste the table into a publication or report.

The automatically generated graphs are very nice and easily customizable. Included plots are “raw data,” “summary ROC,” “logit” (the linear regression line), “forest,” “pre-post,” “different methods” (fixed/random effects), and “sensitivity/specificity.” All plot options are specified through check boxes next to each graph. The process of updating plots after changing the options seemed a little sluggish. The “sensitivity/specificity” plots had some formatting issues where the study name did not line up with the corresponding point on the graph.

Overall, dr-ROC is a convenient solution to performing a meta-analysis of a diagnostic test that is best suited for users who have expertise in the summary ROC methodology. The chief strengths are the easy data input and graphics. The user manual has room for improvement, particularly in terms of clarity, a glossary, and a tutorial.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Parvin C.A.: dr-ROC software. Clin Chem 2006; 52: pp. 543-544.


- 2\. Moses L.E., Shapiro D., Littenberg B.: Combining independent studies of a diagnostic test into a summary ROC curve: Data analytic approaches and some additional considerations. Stat Med 1993; 12: pp. 1293-1316.


- 3\. Littenberg B., Moses L.E.: Estimating diagnostic accuracy from multiple conflicting reports: A new meta-analytic method. Med Decis Making 1993; 13: pp. 313-321.