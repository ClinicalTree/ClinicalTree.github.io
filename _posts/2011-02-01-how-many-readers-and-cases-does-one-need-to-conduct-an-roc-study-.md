---
title: How Many Readers and Cases does One Need to Conduct an ROC Study?
author: [CL_AT_DevPChakrabortyPhD]
date: 2011-02-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 18, Issue 2]
tags: [Journals,General Radiology]
---
This issue includes an article on sample size estimation for receiver operating characteristic (ROC) studies. ROC studies are widely used to assess medical imaging systems and several such studies have appeared in this journal. Sample size estimation is an important consideration when planning an ROC study. It is well known that underpowered studies represent a waste of resources, besides subjecting patients to unnecessary procedures in a study of doubtful scientific value. Funding agencies and institutional review boards usually require the applicant to show that a contemplated study has adequate power. However, in spite of these exhortations, it is probably true that the majority of published ROC studies are underpowered. The problem is not unique to our field, because underpowering is but one reason why a study cannot be replicated . As academic radiologists, we take pride in being especially receptive to methodology issues that affect our discipline.

In a typical ROC study, a representative sample of radiologist observers interpret a representative sample of cases in the two modalities being compared. A figure of merit (eg, area under the ROC curve), is calculated for each observer–modality combination. For each modality, the figures of merit are averaged over all readers, and the difference is calculated—this is the observed effect size. The statistical analysis assigns a _P_ value that chance could have accounted for the observed effect size. If the _P_ value is less than 5%, then the study has “succeeded” and the new modality may become clinically accepted. However, what does one do if the observed effect size is not significant? Assuming that the observed effect size is “encouraging,” the next step is to estimate the numbers of readers and cases for a new study in order to have a reasonable chance of obtaining a significant finding.

Sample size estimation amounts essentially to estimating the variability of the observed effect size. The challenge is that when one calculates a figure of merit, as in the area under the ROC curve, there is a large data reduction. For example, a study with six readers, 200 cases and two modalities yields only 12 numbers, the figures of merit of each of the six readers in the two modalities. The Dorfman, Berbaum, and Metz (DBM) approach depends on the construct of the jackknife pseudovalue. Now, instead of only 12 numbers, one has 12 × 200 (ie, 2400 pseudovalues to analyze, a statistician’s dream!). However, the pseudovalue based DBM method is not entirely satisfying. Most obviously, DBM analysis assumes that the pseudovalues are normally distributed and independent, which they are not. A more satisfying approach by Obuchowski and Rockette is based on the figure of merit—not the pseudovalues. Hillis et al demonstrated an equivalence between the DBM and Obuchowski-Rockette (OR) methods. This meant that whether or not one believed in the DBM pseudovalue-based method, the procedure could be regarded as a procedure that “worked” in the sense that it yielded the same results as the more firmly grounded OR method.

So what remains to be done? Consensus on what is a clinically relevant effect size is lacking. Because it enters the relevant statistic as the square, the effect size has a major influence on the sample size estimate. If one overestimates the effect size then the study could be significantly underpowered. To quote previous work , “My experience and those of colleagues suggest that investigators tend to make the (potentially serious) error of choosing too large of a value. They see that a difference in ROC areas of 0.01 requires a large sample size, whereas a difference of 0.10 leads to a much smaller sample size. Thus, they naively choose the latter.”

Often the only estimate one has of effect size is that observed in the pilot study. However, as noted by Kraemer et al , because the (small) pilot study effect size is an inaccurate estimate of the true effect size, there are two results of this strategy. The true effect size will be understated and the main study may be aborted, even when the true effect size is clinically significant, or the true effect size will be overstated, thereby underestimating the sample size for the main study and under powering the study. Clearly, reliance on the observed effect size is not enough. An alternate approach is: “I don’t know the true effect size—only God does—but I will plan the study so that it can detect a clinically relevant effect size.” Methodology for determining the clinically relevant effect size is needed. Here are some free ideas: the relative cost of the new modality, the change in patient throughput, the costs and benefits of the various decision outcomes, legal considerations, and disease prevalence, all of these factors are expected to impact clinically relevant effect size. For example, if the new modality has broad applicability but is otherwise similar to an existing modality, then a smaller effect size may be considered clinically relevant. If the new modality is applicable to a disease with low prevalence, a so-called “orphan disease,” or the new modality is more expensive, then a larger effect size may be needed before one can justify using the new modality.

A neglected issue, in my opinion, is the units in which effect size is quoted. Commonly, effect size is quoted in area under the ROC curve (AUC) units. In AUC units, changes of ROC areas from 0.95 to 0.96 and from 0.99 to 1.0 are equivalent 1% effect sizes. Because unit AUC represents perfect performance, the improvement from 0.99 to 1.0 represents an infinite improvement (ie, an infinite effect size). A better approach would seem to be to quote effect size in detectability parameter (d′) units.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Hillis S.L., Obuchowski N.A., Berbaum K.S.: Power estimation for multireader ROC methods: an updated and unified approach. Acad Radiol 2011; 18: pp. 129-142.


- 2\. Ioannidis J.P.A.: Why Most Published Research Findings Are False. PLoS Med 2005; 2: pp. e124.


- 3\. Dorfman D.D., Berbaum K.S., Metz C.E.: ROC characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 4\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of the diagnostic accuracy for multiple diagnostic tests: an ANOVA approach with dependent observations. Commun Stat Simulation Computation 1995; 24: pp. 285-308.


- 5\. Hillis S.L., Obuchowski N.A., Schartz K.M., et. al.: A comparison of the Dorfman-Berbaum-Metz and Obuchowski-Rockette methods for receiver operating characteristic (ROC) data. Stat Med 2005; 24: pp. 1579-1607.


- 6\. Obuchowski N.: Determining sample size for roc studies: what is reasonable for the expected difference in tests in ROC areas?. Acad Radiol 2003; 10: pp. 1327-1328.


- 7\. Kreaemer H.C., Mintz J., Noda A., et. al.: Caution regarding the use of pilot studies to guide power calculations for study proposals. Arch Gen Psychiatry 2006; 63: pp. 484-489.


- 8\.  Berbaum KS, Metz CE, Pesce LL, et al. DBM MRMC User's Guide, DBM-MRMC 2.1 Beta Version 2. Available at:  http://www-radiology.uchicago.edu/cgi-bin/roc\_software.cgi  and from  http://perception.radiology.uiowa.edu  . Accessed December 28, 2009.


- 9\. Roe C.A., Metz C.E.: Dorfman-Berbaum-Metz method for statistical analysis of multireader, multimodality receiver operating characteristic data: validation with computer simulation. Acad Radiol 1997; 4: pp. 298-303.


- 10\. Dorfman D.D., Berbaum K.S., Lenth R.V., et. al.: Monte Carlo validation of a multireader method for receiver operating characteristic discrete rating data: factorial experimental design. Acad Radiol 1998; 5: pp. 591-602.


- 11\. Hillis S.L., Berbaum K.S.: Monte Carlo validation of the Dorfman-Berbaum-Metz method using normalized pseudovalues and less data-based model simplification. Acad Radiol 2005; 12: pp. 1534-1541.