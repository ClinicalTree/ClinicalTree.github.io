---
title: An Interactive Web-Based Tool for Detecting Verification (Work-up) Bias in Studies of the Efficacy of Diagnostic Imaging
author: [CL_AT_MichaelLRichardsonMD,CL_AT_JonelleMPetscavageMDMPH]
date: 2010-12-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 17, Issue 12]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Diagnostic tests are validated by comparison against a “gold standard” reference test. When the reference test is invasive or expensive, it may not be applied to all patients. This results in biased estimates of the sensitivity and specificity of the diagnostic test. This type of bias is called “verification bias” and is a common problem in imaging research. The purpose of this study was to create an interactive web-based tool to help detect the presence of prevalence of verification bias in data.

## Materials and Methods

The web-based tool was written using well-documented and freely available open-source software (HTML, Apache, Ruby, and R). Our calculator is currently hosted on a Mac OS X server, but should run with minor changes on most other platforms.

## Results

Our program applies user-supplied study data to generate a global sensitivity analysis plot containing noncorrected and corrected values of sensitivity and specificity and 95% confidence intervals for these estimates. Interpretation of the global sensitivity analysis (GSA) plot is relatively simple. Because the characteristic GSA “butterfly” plot contains all possible values of sensitivity and specificity, any indices lying outside of this butterfly are therefore incompatible with the data, confirming that they are biased.

## Conclusions

Our online calculator makes it easy for investigators to use global sensitivity analysis to demonstrate the presence of significant verification bias and to estimate bias-corrected values of sensitivity and specificity.

Sensitivity and specificity are key indices of the efficacy of a diagnostic test. Clinicians consider these indices when choosing one diagnostic imaging test over another. However, sensitivity and specificity can be biased when research does not correct for verification bias . Verification bias, also known as “workup bias” or “posttest referral bias,” occurs when patients receiving the test of interest are not equally likely to undergo a reference standard test to verify their diagnosis and only those receiving the “gold standard” test are included in the statistical analysis . Failure to verify all patients may occur when the reference test is invasive, expensive, or refused by patients.

Additional forms of verification bias occur when an inappropriate reference standard is used or when patients are verified using different reference standards in the same study . Ultimately, these different forms of verification bias will falsely elevate estimates of sensitivity and falsely deflate estimates of specificity. The false estimates may result in a clinician choosing an exam that is not the most accurate for patient diagnosis. This in turn may alter one’s decision to treat, to order more tests, or to discharge a patient. For examinations such as computed tomography or fluoroscopy, this can result in unnecessary patient radiation exposure.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 6.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Resulting global sensitivity analysis plot for the input values shown in Figure 1 .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnInteractiveWebBasedToolforDetectingVerificationWorkupBiasinStudiesoftheEfficacyofDiagnosticImaging/0_1s20S1076633210004241.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


![Figure 1, Initial web page for global sensitivity analysis calculator with sample input values.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnInteractiveWebBasedToolforDetectingVerificationWorkupBiasinStudiesoftheEfficacyofDiagnosticImaging/1_1s20S1076633210004241.jpg)

![Figure 2, Flowchart of global sensitivity analysis calculator.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AnInteractiveWebBasedToolforDetectingVerificationWorkupBiasinStudiesoftheEfficacyofDiagnosticImaging/2_1s20S1076633210004241.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

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

## Supplementary data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Appendix 1 to 3

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Zhou X.H., Obuchowski N.A., Obuchowski D.M.: Statistical Methods in Diagnostic Medicine.2002.Wiley & SonsNew York


- 2\. Sica G.T.: Bias in research studies. Radiology 2006; 238: pp. 780-789.


- 3\. Begg C.B.: Biases in the assessment of diagnostic tests. Stat Med 1987; 6: pp. 411-423.


- 4\. Revesz G., Kundel H.L., Bonitatibus M.: The effect of verification on the assessment of imaging techniques. Investig Radiol 1983; 18: pp. 194-198.


- 5\. Kosinski A.S., Barnhart H.X.: A global sensitivity analysis of performance of a medical diagnostic test when verification bias is present. Stat Med 2003; 22: pp. 2711-2721.


- 6\. Whiting P., Rutjes A.W.S., Reitsma J.B., et. al.: Sources of variation and bias in studies of diagnostic accuracy: a systematic review. Ann Intern Med 2004; 140: pp. 189-202.


- 7\. Bates A.S., Margolis P.A., Evans A.T.: Verification bias in pediatric studies evaluating diagnostic tests. J Pediatr 1993; 122: pp. 585-590.


- 8\. Cronin A.M., Vickers A.J.: Statistical methods to correct for verification bias in diagnostic studies are inadequate when there are few false negatives: a simulation study. BMC Med Res Methodol 2008; 8: pp. 75.


- 9\. Mallett S., Deeks J.J., Halligan S., et. al.: Systematic reviews of diagnostic tests in cancer: review of methods and reporting. BMJ 2006; 333: pp. 413.


- 10\. Begg C.B., Greenes R.A.: Assessment of diagnostic tests when disease verification is subject to selection bias. Biometrics 1983; 39: pp. 207-215.


- 11\. Diamond G.A.: Reverend Bayes’ silent majority. An alternative factor affecting sensitivity and specificity of exercise electrocardiography. Am J Cardiol 1986; 57: pp. 1175-1180.


- 12\. Rubin D.B., Schenker N.: Logit-based interval estimation for binomial data using the Jeffreys prior. Sociol Methodol 1987; 17: pp. 131-144.


- 13\. Harel O., Zhou X-H.: Multiple imputation for correcting verification bias. Stat Med 2006; 25: pp. 3769-3786.


- 14\. Punglia R.S., D’Amico A.V., Catalona W.J., et. al.: Effect of verification bias on screening for prostate cancer by measurement of prostate-specific antigen. N Engl J Med 2003; 349: pp. 335-342.


- 15\. Nishikawa H., Imanaka Y., Sekimoto M., et. al.: Influence of verification bias on the assessment of MRI in the diagnosis of meniscal tear. AJR Am J Roentgenol 2009; 193: pp. 1596-1602.