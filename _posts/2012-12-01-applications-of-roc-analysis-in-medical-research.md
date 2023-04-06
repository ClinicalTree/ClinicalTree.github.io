---
title: Applications of ROC Analysis in Medical Research
author: [Demissie Alemayehu PhD,Kelly H. Zou PhD PStat]
date: 2012-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 19, Issue 12 SOURCE CL_S_AcademicRadiologyVolume19Issue12 1}]
tags: [Journals,General Radiology]
---
With the growing focus on comparative effectiveness research and personalized medicine, receiver-operating characteristic analysis can continue to play an important role in health care decision making. Specific applications of receiver-operating characteristic analysis include predictive model assessment and validation, biomarker diagnostics, responder analysis in patient-reported outcomes, and comparison of alternative treatment options. The authors present a survey of the potential applications of the method and briefly review several relevant extensions. Given the level of attention paid to biomarker validation, personalized medicine and comparative effectiveness research, it is highly likely that the receiver-operating characteristic analysis will remain an important visual and analytic tool for medical research and evidence-based medicine in the foreseeable future.

The receiver-operating characteristic (ROC) curve is a visual tool for assessing the accuracy of a classifier or predictor. As a measure and display of classification accuracy, the ROC curve has several appealing features relative to other competing measures. Some of these desirable features include the incorporation of sensitivity (ie, true-positive fraction \[TPF\]) and specificity (ie, true-negative fraction \[TNF\]) into a single performance metric, an ROC point. Such a performance metric does not depend on the disease prevalence as it does for other metrics (eg, measures of test accuracy). This property is advantageous to either rule in or rule out diseases, particularly when dealing with rare events in medical research. A highly sensitive test is particularly useful to rule out disease, while a highly specific test is particularly useful to rule in disease .

The history of ROC analysis dates back to World War II, when it first found application in the assessment of the accuracy of prediction of enemy aircraft on the basis of radar signals. The original purpose was to assess classification accuracy to differentiate good “signals” from bad “noises.” In subsequent years, the ROC methodology was fully integrated in the theory of signal detection, and the concept was later popularized in such diverse fields as psychophysics to quantify the association between physical stimuli and their sensory effects , medical imaging , radiologists' performance , machine learning , and medical informatics , as well as finance, sociology, and beyond .

Since the early 1980s, there have been increasing applications of the procedure in medical research.  Figure 1 displays the growth in the number of peer-reviewed articles according to a PubMed search using search string “receiver operating characteristic” in the period between January 1, 1981, and December 31, 2010 . This systematic search was conducted on August 10, 2012. Furthermore, the topic has been the subject of comprehensive monographs and review articles , focusing on a variety of topics that include sample size and power considerations for study designs .

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633211X00235/S1076633212004734/gr1.jpg?Signature=iTxVqgOYiF1bwHMF5OCi0jL8yLp1PrYQ6bcQ0d3P2-bNL0lQSs8DjVlnnaXnMyHF8EuIq8xO1yuj6zNWU04FIkgZ7FZf2cbBvtXorN-8DLKS8YkssOooAlvEO-RTPewh8lv%7EBvf57SzN8hn%7EgD-Mlk0lbghtkZRssD-Gktn8dLU_&Expires=1669572623&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Number of publications using receiver-operating characteristic analysis from 1981 to 2010 according to a systematic search in PubMed.


The use of ROC curves in evidence-based medicine ranged from the evaluation of screening and diagnostic tests to the assessment of performance of models for the identification of subgroups of patients at differential risks for specific outcomes . In clinical practice, physicians routinely rely on the accuracy of diagnostic testing to provide effective care to their patients. For example, in cardiology, serum markers are used to screen for myocardial necrosis, while cardiac imaging tests are customarily used to diagnose various cardiovascular complications . In other applications, when interest lies in estimating expected outcomes (eg, mortality or adverse events) as a function of patient risk factors, one often resorts to predictive models. In all of these cases, ROC analysis can play a central role.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Basic concepts of receiver-operating characteristic analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Cross-tabulation of a Binary Diagnosis (Dx) on the Basis of a Continuous Test Outcome ( _T_ ) Dichotomized according to an Arbitrary Cutoff Threshold ( _c_ ) Versus a Binary Reference Standard (RS)


Dx RS Total Count Healthy (RS = 0) Diseased (RS = 1) Negative if { _T_ ≤ _c_ }_A_ = #{TN}_B_ = #{FN}_A_ \+ _B_ = #{ _T_ ≤ _c_ } Positive if { _T_ \> _c_ }_C_ = #{FP}_D_ = #{TP}_C_ \+ _D_ = #{ _T_ \> _c_ } Total count_A_ \+ _C_ = _m__B_ \+ _D_ = _n__N_ = _A_ \+ _B_ \+ _C_ \+ _D_ = _m_ \+ _n_

FN, false-negative; FNF, false-negative fraction; FP, false-positive; FPF, false-positive fraction; TN, true-negative; TNF, true-negative fraction; TP, true-positive; TPF, true-positive fraction.


Specificity = TNF = #{TN}/ _m_ = _A_ /( _A_ \+ _C_ ); sensitivity = TPF = #{TP}/ _n_ = _D_ /( _B_ \+ _D_ ); FPF = 1−specificity; FNF = 1−sensitivity; disease prevalence = _n_ / _N_ , where _N_ = _m_ \+ _n_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Hypothetical receiver-operating characteristic curves to differentiate between two classes (eg, healthy vs diseased), determined by a binary reference standard.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ApplicationsofROCAnalysisinMedicalResearch/0_1s20S1076633212004734.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

AUC=Φ(α/1+β2−−−−−√),
AUC

=

Φ

(

α

/

1

+

β

2

)

,


where Φ is the CDF of a standard normal random variable, _N_ (0,1).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Applications of receiver-operating characteristic analysis in medical research

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Biomarker Diagnostics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classification and Predictive Model Assessment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Responder Analysis and CDF Plot

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

(YR,0,YR,1)∼BN\[(5,8)(10.50.51)\];
(

Y

R

,

0

,

Y

R

,

1

)

∼

BN

\[

(

5

,

8

)

(

1

0.5

0.5

1

)

\]

;


(YNR,0,YNR,1)∼BN\[(5,5)(10.30.31)\].
(

Y

NR

,

0

,

Y

NR

,

1

)

∼

BN

\[

(

5

,

5

)

(

1

0.3

0.3

1

)

\]

.


![Figure 3, Hypothetical cumulative distribution function plots (a) and corresponding receiver-operating characteristic curve (b) to differentiate between responders and nonresponders. AUC, area under the curve.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ApplicationsofROCAnalysisinMedicalResearch/1_1s20S1076633212004734.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Treatment Comparison

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ROC software programs

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Bianchi M.T., Alexander B.M.: Evidence based diagnosis: does the language reflect the theory?. BMJ 2006; 333: pp. 442-445.


- 2\. Swets J.A., Pickett R.M.: Evaluation of Diagnostic Systems: Methods From Signal Detection Theory.1982.Academic PressNew York


- 3\. Metz C.E.: ROC methodology in radiologic imaging. Invest Radiol 1986; 21: pp. 720-733.


- 4\. Metz C.E., Wagner R.F., Doi K., et. al.: Toward consensus on quantitative assessment of medical imaging systems. Med Phys 1995; 22: pp. 1057-1061.


- 5\. Dofrman D.D., Berbaum K.S., Lenth R.V.: Multireader, multicase receiver operating characteristic methodology: a bootstrap analysis. Acad Radiol 1995; 2: pp. 626-633.


- 6\. Metz C.E.: Receiver operating characteristic analysis: a tool for the quantitative evaluation of observer performance and imaging systems. J Am Coll Radiol 2006; 3: pp. 413-422.


- 7\. Metz C.E.: ROC analysis in medical imaging: a tutorial review of the literature. Radiol Phys Technol 2008; 1: pp. 2-12.


- 8\. Kashani H., Varon C.A., Paul N.S., et. al.: Diagnostic performance of a prototype dual-energy chest imaging system ROC analysis. Acad Radiol 2010; 17: pp. 298-308.


- 9\. Aoki T., Oda N., Yamashita Y., et. al.: Usefulness of computerized method for lung nodule detection in digital chest radiographs using temporal subtraction images. Acad Radiol 2011; 18: pp. 1000-1005.


- 10\. Foerster B.R., Dwamena B.A., Petrou M., et. al.: Diagnostic accuracy using diffusion tensor imaging in the diagnosis of ALS: a meta-analysis. Acad Radiol 2012; 19: pp. 1075-1086.


- 11\. Larson T.C., Holiday D.B., Antao V.C., et. al.: Comparison of digital with film radiographs for the classification of pneumoconiotic pleural abnormalities. Acad Radiol 2012; 19: pp. 131-140.


- 12\. Matsubara R., Kawano S., Chikui T., et. al.: Clinical significance of combined assessment of the maximum standardized uptake value of F-18 FDG PET with nodal size in the diagnosis of cervical lymph node metastasis of oral squamous cell carcinoma. Acad Radiol 2012; 19: pp. 708-717.


- 13\. Obuchowski N.A.: Multireader, multimodality receiver operating characteristic curve studies: hypothesis testing and sample size estimation using an analysis of variance approach with dependent observations. Acad Radiol 1995; 2: pp. S22-S29.


- 14\. Obuchowski N.A.: Multireader receiver operating characteristic studies: a comparison of study designs. Acad Radiol 1995; 2: pp. 709-716.


- 15\. Obuchowski N.A., Beiden S.V., Berbaum K.S., et. al.: Multireader, multicase receiver operating characteristic analysis: an empirical comparison of five methods. Acad Radiol 2004; 11: pp. 980-995.


- 16\. Miglioretti D.L., Haneuse S.J., Anderson M.L.: Statistical approaches for modeling radiologists' interpretive performance. Acad Radiol 2009; 16: pp. 227-238.


- 17\. Cole E.B., Toledano A.Y., Lundqvist M., et. al.: Comparison of radiologist performance with photon-counting full-field digital mammography to conventional full-field digital mammography. Acad Radiol 2012; 19: pp. 916-922.


- 18\. Spackman K.A.: Signal detection theory: valuable tools for evaluating inductive learning.Proceedings of the Sixth International Workshop on Machine Learning.1989.Morgan KaufmannSan Mateo, CA:


- 19\. Paquerault S., Hardy P.T., Wersto N., et. al.: Investigation of optimal use of computer-aided detection systems: the role of the “machine” in decision making process. Acad Radiol 2010; 17: pp. 1112-1121.


- 20\. Lasko T.A., Bhagwat J.G., Zou K.H., et. al.: The use of receiver operating characteristic curves in biomedical informatics. J Biomed Inform 2005; 38: pp. 404-415.


- 21\. Chen H., Xu Y., Ma Y., et. al.: Neural network ensemble-based computer-aided diagnosis for differentiation of lung nodules on CT images: clinical evaluation. Acad Radiol 2010; 17: pp. 595-602.


- 22\. Krzanowski W.J., Hand D.J.: ROC Curves for Continuous Data.2009.Chapman & Hall/CRC PressBoca Raton, FL


- 23\.  National Library of Medicine. PubMed.gov. Available at:  http://www.ncbi.nlm.nih.gov/pubmed  . Accessed August 10, 2012.


- 24\. Zhou X.H., Obuchowski N.A., McClish D.K.: Statistical Methods in Diagnostic Medicine.2002.John WileyNew York


- 25\. Pepe M.S.: The Statistical Evaluation of Medical Tests for Classification and Prediction.2003.Oxford University PressOxford, UK


- 26\. Gönen M.: Analyzing Receiver Operating Characteristic Curves with SAS  ® .2007.SAS Institute IncCary, NC


- 27\. Zou K.H., Liu A., Bandos A.I., et. al.: Statistical Evaluation of Diagnostic Performance: Topics in ROC Analysis.2011.Chapman & Hall/CRC PressBoca Raton, FL


- 28\. Zweig M.H., Campbell G.: Receiver-operating characteristic (ROC) plots: a fundamental evaluation tool in clinical medicine. Clin Chem 1993; 39: pp. 561-577.


- 29\. Zhou X.H.: Correcting for verification bias in studies of a diagnostic test's accuracy. Stat Methods Med Res 1998; 7: pp. 337-353.


- 30\. Shapiro D.E.: The interpretation of diagnostic tests. Stat Methods Med Res 1999; 8: pp. 113-134.


- 31\. Obuchowski N.A., Lieber M.L., Wians F.H.: ROC curves in clinical chemistry: uses, misuses, and possible solutions. Clin Chem 2004; 50: pp. 1118-1125.


- 32\. Eng J.: Receiver operating characteristic analysis: a primer. Acad Radiol 2005; 12: pp. 909-916.


- 33\. Weinstein S., Obuchowski N.A., Lieber M.L.: Clinical evaluation of diagnostic tests. AJR Am J Roentgenol 2005; 184: pp. 14-19.


- 34\. Zou K.H., O'Malley A.J., Mauri L.: Receiver-operating characteristic analysis for evaluating diagnostic tests and predictive models. Circulation 2007; 115: pp. 654-657.


- 35\. Wagner R.F., Metz C.E., Campbell G.: Assessment of medical imaging systems and computer aids: a tutorial review. Acad Radiol 2007; 14: pp. 723-748.


- 36\. Mallett S., Halligan S., Thompson M., et. al.: Interpreting diagnostic accuracy studies for patient care. BMJ 2012; 345: pp. e3999.


- 37\. Obuchowski N.A.: Sample size calculations in studies of test accuracy. Stat Methods Med Res 1998; 7: pp. 371-392.


- 38\. Eng J.: Sample size estimation: a glimpse beyond simple formulas. Radiology 2004; 230: pp. 606-612.


- 39\. Chakraborty D.P.: Prediction accuracy of a sample-size estimation method for ROC studies. Acad Radiol 2010; 17: pp. 628-638.


- 40\. Chakraborty D.P.: How many readers and cases does one need to conduct an ROC study?. Acad Radiol 2011; 18: pp. 127-128.


- 41\. Hillis S.L., Obuchowski N.A., Berbaum K.S.: Power estimation for multireader ROC methods an updated and unified approach. Acad Radiol 2011; 18: pp. 129-142.


- 42\. Friedman C.A., Sandow S.: Model performance measures for expected utility maximizing investors. Int J Theoretical Appl Finance 2003; 6: pp. 355-401.


- 43\. Adams J.E., Sicard G.A., Allen B.T., et. al.: Diagnosis of perioperative myocardial infarction with measurement of cardiac troponin I. N Engl J Med 1994; 330: pp. 670-674.


- 44\.  Institute of Medicine. Initial national priorities for comparative effectiveness research. Available at:  http://www.iom.edu/Reports/2009/ComparativeEffectivenessResearchPriorities.aspx  . Accessed September 17, 2012.


- 45\. Leeflang M.M., Deeks J.J., Gatsonis C., et. al.: Systematic reviews of diagnostic test accuracy. Ann Intern Med 2008; 149: pp. 889-897.


- 46\. Virgili G., Conti A.A., Murro V., et. al.: Systematic reviews of diagnostic test accuracy and the Cochrane collaboration. Intern Emerg Med 2009; 4: pp. 255-258.


- 47\. Faraggi D.: The effect of random measurement error on receiver operating characteristic (ROC) curves. Stat Med 2000; 19: pp. 61-70.


- 48\. Zhou X.H., Harezlak J.: Comparison of bandwidth selection methods for kernel smoothing of ROC curves. Stat Med 2002; 21: pp. 2045-2055.


- 49\. Dorfman D.D., Alf E.: Maximum likelihood estimation of parameters of signal detection theory—a direct solution. Psychometrika 1968; 33: pp. 117-124.


- 50\. Metz C.E., Herman B.A., Shen J.H.: Maximum likelihood estimation of receiver operating characteristic (ROC) curves from continuously-distributed data. Stat Med 1998; 17: pp. 1033-1053.


- 51\. Pesce L.L., Horsch K., Drukker K., et. al.: Semiparametric estimation of the relationship between ROC operating points and the test-result scale: application to the proper binormal model. Acad Radiol 2011; 18: pp. 1537-1548.


- 52\. Zou K.H., Warfield S.K., Fielding J.R., et. al.: Statistical validation based on parametric receiver operating characteristic analysis of continuous classification data. Acad Radiol 2003; 10: pp. 1359-1368.


- 53\. Dorfman D.D., Berbaum K.S., Metz C.E., et. al.: Proper receiver operating characteristic analysis: the bigamma model. Acad Radiol 1997; 4: pp. 138-149.


- 54\. Zou K.H., Wells W.M., Kikinis R., et. al.: Three validation metrics for automated probabilistic image segmentation of brain tumours. Stat Med 2004; 23: pp. 1259-1282.


- 55\. Hanley J.A., McNeil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 56\. Hanley J.A., McNeil B.J.: A method of comparing the areas under receiver operating characteristic curves derived from the same cases. Radiology 1983; 148: pp. 839-843.


- 57\. Bamber D.: The area above the ordinal dominance graph and the area below the receiver operating graph. J Math Psychol 1975; 12: pp. 387-415.


- 58\. Wan S., Zhang B.: Smooth semiparametric receiver operating characteristic curves for continuous diagnostic tests. Stat Med 2007; 26: pp. 2565-2586.


- 59\. Wieand S., Gail M.H., James B.R., et. al.: A family of nonparametric statistics for comparing diagnostic markers with paired or unpaired data. Biometrika 1989; 76: pp. 585-592.


- 60\. Wagner R.F., Beiden S.V., Campbell G., et. al.: Assessment of medical imaging and computer-assist systems: lessons from recent experience. Acad Radiol 2002; 9: pp. 1264-1277.


- 61\. Hillis S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 62\. Yuan Y., Giger M.L., Li H., et. al.: Multimodality computer-aided breast cancer diagnosis with FFDM and DCE-MRI. Acad Radiol 2010; 17: pp. 1158-1167.


- 63\. Chen W., Petrick N.A., Sahiner B.: Hypothesis testing in noninferiority and equivalence MRMC ROC studies. Acad Radiol 2012; 19: pp. 1158-1165.


- 64\. Dorfman D.D., Berbaum K.S., Metz C.E.: Receiver operating characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 65\. Dorfman D.D., Berbaum K.S., Lenth R.V., et. al.: Monte Carlo validation of a multireader method for receiver operating characteristic discrete rating data: factorial experimental design. Acad Radiol 1998; 5: pp. 591-602.


- 66\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of the diagnostic accuracy for multiple diagnostic tests: an ANOVA approach with dependent observations. Commun Stat Simul Computation 1995; 24: pp. 285-308.


- 67\. Beiden S.V., Wagner R.F., Campbell G.: Components-of-variance models and multiple-bootstrap experiments: an alternative method for random-effects, receiver operating characteristic analysis. Acad Radiol 2000; 7: pp. 341-349.


- 68\. Song H.H.: Analysis of correlated ROC areas in diagnostic testing. Biometrics 1997; 53: pp. 370-382.


- 69\. Ishwaran H., Gatsonis C.A.: A general class of hierarchical ordinal regression models with applications to correlated ROC analysis. Can J Stat 2000; 28: pp. 731-750.


- 70\. Bandos A.I., Rockette H.E., Song T., et. al.: Area under the free-response ROC curve (FROC) and a related summary index. Biometrics 2009; 65: pp. 247-256.


- 71\. Chakraborty D.P.: Clinical relevance of the ROC and free-response paradigms for comparing imaging system efficacies. Radiat Prot Dosimetry 2010; 139: pp. 37-41.


- 72\. Chakraborty D.P.: New developments in observer performance methodology in medical imaging. Semin Nucl Med 2011; 41: pp. 401-418.


- 73\. Katz R.: Biomarkers and surrogate markers: an FDA perspective. NeuroRx 2004; 1: pp. 189-195.


- 74\. Hylton N.: Dynamic contrast-enhanced magnetic resonance imaging as an imaging biomarker. J Clin Oncol 2006; 24: pp. 3293-3298.


- 75\. Lee J.W., Devanarayan V., Barrett Y.C., et. al.: Fit-for-purpose method development and validation for successful biomarker measurement. Pharm Res 2006; 23: pp. 312-328.


- 76\. Su J., Liu J.S.: Linear combinations of multiple diagnostic markers. J Am Stat Assoc 1993; 88: pp. 1350-1355.


- 77\. Liu C., Liu A., Halabi S.: A min-max combination of biomarkers to improve diagnostic accuracy. Stat Med 2011; 30: pp. 2005-2014.


- 78\. Greving J.P., Schonewille W.J., Wijman C.A., et. al.: BASICS Study Group. Predicting outcome after acute basilar artery occlusion based on admission characteristics. Neurology 2012; 78: pp. 1058-1063.


- 79\. Talos I.F., Zou K.H., Ohno-Machado L., et. al.: Supratentorial low-grade glioma resectability: statistical predictive analysis based on anatomic MR features and tumor characteristics. Radiology 2006; 239: pp. 506-513.


- 80\. Hollenbeak C.S., Chirumbole M., Novinger B., et. al.: Predictive models for diabetes patients in Medicaid. Popul Health Manag 2011; 14: pp. 239-242.


- 81\. O'Malley A.J., Zou K.H.: Bayesian multivariate hierarchical transformation models for ROC analysis. Stat Med 2006; 25: pp. 459-479.


- 82\. Mundry R., Nunn C.L.: Stepwise model fitting and statistical inference: turning noise into signal pollution. Am Nat 2009; 173: pp. 119-123.


- 83\. Farrar J.T., Dworkin R.H., Max M.B.: Use of the cumulative proportion of responders analysis graph to present pain data over a range of cut-off points: making clinical trial data more understandable. J Pain Symptom Manage 2006; 31: pp. 369-377.


- 84\. Farrar J.T., Young J.P., LaMoreaux L., et. al.: Clinical importance of changes in chronic pain intensity measured on an 11-point numerical pain rating scale. Pain 2001; 94: pp. 149-158.


- 85\. de Vet H.C., Ostelo R.W., Terwee C.B., et. al.: Minimally important change determined by a visual method integrating an anchor-based and a distribution-based approach. Qual Life Res 2007; 16: pp. 131-142.


- 86\.  US Food and Drug Administration. Guidance for industry: patient-reported outcome measures: use in medical product development to support labeling claims. Available at:  http://www.fda.gov/downloads/Drugs/GuidanceComplianceRegulatoryInformation/Guidances/UCM193282.pdf  . Accessed September 28, 2012.


- 87\. Speight J., Barendse S.M.: FDA guidance on patient reported outcomes. BMJ 2010; 340: pp. c2921.


- 88\. Fluss R., Faraggi D., Reiser B.: Estimation of the Youden index and its associated cutoff point. Biom J 2005; 47: pp. 458-472.


- 89\. O'Malley A.J., Zou K.H., Fielding J.R., et. al.: Bayesian regression methodology for estimating a receiver operating characteristic curve with two radiologic applications: prostate biopsy and spiral CT of ureteral stones. Acad Radiol 2001; 8: pp. 713-725.


- 90\. Perkins N.J., Schisterman E.F.: The inconsistency of “optimal” cutpoints obtained using two criteria based on the receiver operating characteristic curve. Am J Epidemiol 2006; 163: pp. 670-675.


- 91\. Brumback L.C., Pepe M.S., Alonzo T.A.: Using the ROC curve for gauging treatment effect in clinical trials. Stat Med 2006; 25: pp. 575-590.


- 92\. Rutter C.M., Gatsonis C.A.: Regression methods for meta-analysis of diagnostic test data. Acad Radiol 1995; 2: pp. S48-S56.


- 93\.  University of Chicago, Department of Radiology. Metz ROC software at the University of Chicago. Available at:  http://metz-roc.uchicago.edu/MetzROC  . Accessed September 17, 2012.


- 94\.  University of Iowa, Medical Perception Library. DBM MRMC. Available at:  http://perception.radiology.uiowa.edu/Software/ReceiverOperatingCharacteristicROC/DBMMRMC/tabid/116/Default.aspx  . Accessed September 17, 2012.


- 95\.  Eng J. ROC analysis: Web-based calculator for ROC curves. Available at:  http://www.jrocfit.org  . Accessed September 17 2012.


- 96\.  SAS Institute Inc. Plot ROC curve with labeled points for a binary-response model. Available at:  http://support.sas.com/kb/25/018.html  . Accessed September 17, 2012.


- 97\.  SAS Institute. %macro roc. Available at:  http://support.sas.com/kb/25/addl/fusion\_25017\_6\_roc.sas.txt  . Accessed September 17, 2012.


- 98\.  Gönen M. Analyzing receiver operating characteristic curves with SAS. Available at:  http://www.mskcc.org/sites/www.mskcc.org/files/node/11749/documents/sas-code-macros.txt  . Accessed September 17, 2012.


- 99\.  Robin X, Turck N, Hainard A, et al. Package “pROC.” Available at:  http://cran.r-project.org/web/packages/pROC/pROC.pdf  . Accessed September 17, 2012.


- 100\.  Lauss M. Package “rocc.” Available at:  http://cran.r-project.org/web/packages/rocc/rocc.pdf  . Accessed September 17, 2012.


- 101\.  Wheeler B. Package “rocplus.” Available at:  http://cran.r-project.org/web/packages/rocplus/rocplus.pdf  . Accessed September 17, 2012.


- 102\.  Sing T, Sander O, Beerenwinkel N, et al. ROCR: visualizing the performance of scoring classifiers. Available at:  http://cran.r-project.org/web/packages/ROCR/index.html  . Accessed September 17, 2012.


- 103\.  Heagerty PJ, Saha P. survivalROC: time-dependent ROC curve estimation from censored survival data. Available at:  http://cran.r-project.org/web/packages/survivalROC/index.html  . Accessed September 17, 2012.


- 104\.  Lopez-Raton M, Rodriguez-Alvarez MX. Package “OptimalCutpoints.” Available at:  http://cran.r-project.org/web/packages/OptimalCutpoints/OptimalCutpoints.pdf  . Accessed September 17, 2012.


- 105\.  Pepe Lab, Fred Hutchison Cancer Research Center. Software. Available at:  http://labs.fhcrc.org/pepe/dabs/software.html  . Accessed September 17, 2012.


- 106\.  Cleveland Clinic, Department of Quantitative Health Sciences. Research activities: ROC analysis. Available at:  http://www.bio.ri.ccf.org/html/rocanalysis.html  . Accessed September 17, 2012.


- 107\. Rutter C.M., Gatsonis C.A.: A hierarchical regression approach to meta-analysis of diagnostic test accuracy evaluations. Stat Med 2001; 20: pp. 2865-2884.


- 108\. Obuchowski N.A.: Estimating and comparing diagnostic tests' accuracy when the gold standard is not binary. Acad Radiol 2005; 12: pp. 1198-1204.


- 109\. Obuchowski N.A.: An ROC-type measure of diagnostic accuracy when the gold standard is continuous-scale. Stat Med 2006; 25: pp. 481-493.


- 110\. Talos I.F., Mian A.Z., Zou K.H., et. al.: Magnetic resonance and the human brain: anatomy, function and metabolism. Cell Mol Life Sci 2006; 63: pp. 1106-1124.


- 111\. Warfield S.K., Zou K.H., Wells W.M.: Simultaneous truth and performance level estimation (STAPLE): an algorithm for the validation of image segmentation. IEEE Trans Med Imaging 2004; 23: pp. 903-921.


- 112\. Warfield S.K., Zou K.H., Wells W.M.: Validation of image segmentation by estimating rater bias and variance. Philos Transact A Math Phys Eng Sci 2008; 366: pp. 2361-2375.


- 113\. Phelps C.E., Hutson A.: Estimating diagnostic test accuracy using a “fuzzy gold standard.”. Med Decis Making 1995; 15: pp. 44-57.