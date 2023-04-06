---
title: Registration-Based Metrics of Lung Function to Describe COPD
author: [Robert H. Brown MD MPH]
date: 2013-05-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 20, Issue 5 SOURCE CL_S_AcademicRadiologyVolume20Issue5 1}]
tags: [Journals,General Radiology]
---
We have a very complex organ (the lung), and on it is superimposed a very complicated disease, chronic obstructive pulmonary disease (COPD). How can we devise a simple value that gives us greater insight into this heterogeneous disease in this complex organ? How can we better assess COPD in patients? More important, how can we better determine the extent that ever-worsening COPD has on the lives of our patients? The pulmonary component of COPD is characterized by airflow limitation that is not fully reversible. The airflow limitation is usually progressive and associated with an abnormal inflammatory response of the lungs to noxious particles or gases , the most common of which is cigarette smoke. COPD is classically assessed by pulmonary function testing. Spirometry is a pulmonary function test (PFT) to determine the diagnosis and evaluate the severity of the disease. The ratio of the post-bronchodilator forced expiratory volume in 1 second divided by the forced vital capacity (FEV  1 /FVC) <0.70 is the classic cut-off for a diagnosis of COPD . As the FEV  1 /FVC ratio decreases, the severity of the disease increases. The generally accepted categorization of COPD severity classifies patients into four stages according to the Global Initiative for Chronic Obstructive Lung Disease (GOLD) classification . Can we devise a better way to assess the disease based on the directly viewed changes in the lungs in vivo?

With the advent of computed tomographic (CT) scanning more than four decades earlier, the ability to examine the lung parenchyma has improved with each new generation of faster and greater resolution CT machines. Now, one can directly assess the parenchyma in both health and disease states . Thus, we have a window into the lungs to assess the destruction wrought by (predominantly) cigarette smoke on the lungs that leads to COPD. Emphysema, the extent and progression of which historically we could measure only with the use of limited pathological specimens at autopsy, can now be easily measured in vivo. We can assess the amount of parenchymal destruction and compare it to the decrease in lung function in COPD. Other methods have been used to improve our ability to correlate the anatomic changes seen in the lungs using high-resolution CT with the physiological changes of disease. Several investigators have proposed various methods to improve our analysis of the CT data to better correlate with the spirometric data .

In the current issue of _Academic Radiology_ , Bodduluri et al use image registration to provide additional information about lung function changes in COPD subjects. Their study uses a combination of density and texture feature sets and compares that to a biomechanical feature set from the registration of inspiratory and expiratory scans to evaluate the severity of COPD, with the presumption that this method will provide greater accuracy. They tested this through the use of a machine-learning framework to evaluate the performance of the obtained feature sets. They found that many of their CT-derived features were highly correlated with spirometry measurements as well as a health-related quality of life questionnaire. However, it was not clear whether these CT features would translate into a better understanding of the extent, progression, or response to therapy of the disease compared to the information described by the spirometry and/or the health questionnaire. Are we simply trading one value (spirometry) for another (CT-based image features)? How can we attain a simpler valuation that gives us greater insight into the disease? With a very complex organ and a very complicated disease, is it possible to derive a simple answer?

One important step in developing a better measure of lung disease is the use of image registration of inspiratory and expiratory scans, as presented by Bodduluri et al . This should lead to better quantification of the changes in the lung with disease progression and should be lauded. The lung is a dynamic organ in constant motion. Using image registration in their analyses thus considers the dynamic nature of the lung. These authors examined whether their feature sets could determine which CT scans were from individuals with COPD, compared to the data from spirometry and the health questionnaire. The biomechanical feature set showed higher correlations with FEV  1 percent predicted but not with FEV  1 /FVC, the latter being the classic spirometric measure of COPD. Combining all three feature sets produced the best correlations with the spirometric measures and the health-related quality of life questionnaire. However, surprisingly, the combination of all three did not have the highest area under the curve on the receiver operating characteristic analysis.

Another aspect of these investigators' study was the use of a machine-learning framework to evaluate the performance of the obtained biomechanical feature set compared to density- and texture-based feature sets, with the goal of using their feature sets to determine the presence and severity of disease (COPD vs non-COPD) (GOLD stages 0–4). They showed that the biomechanical features were more effective in recognizing COPD severity than the density and texture feature sets.

This work has all the makings of a method that would combine all the complicated variables into a simple measure, but we are not quite there yet. We never quite get a sense of which feature set is most important, or what is the best combination of feature sets, in discriminating disease from nondisease.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Rabe K.F., Hurd S., Anzueto A., et. al.: Global strategy for the diagnosis, management, and prevention of chronic obstructive pulmonary disease: GOLD executive summary. Am J Respir Crit Care Med 2007; 176: pp. 532-555.


- 2\. Barr R.G., Berkowitz E.A., Bigazzi F., et. al.: A combined pulmonary-radiology workshop for visual evaluation of COPD: study design, chest CT findings and concordance with quantitative evaluation. COPD 2012; 9: pp. 151-159.


- 3\. Diaz A.A., Bartholmai B., San Jose Estepar R., et. al.: Relationship of emphysema and airway disease assessed by CT to exercise capacity in COPD. Respir Med 2010; 104: pp. 1145-1151.


- 4\. Diaz A.A., Come C.E., Ross J.C., et. al.: Association between airway caliber changes with lung inflation and emphysema assessed by volumetric CT scan in subjects with COPD. Chest 2012; 141: pp. 736-744.


- 5\. Diaz A.A., Han M.K., Come C.E., et. al.: The effect of emphysema on computed tomographic measures of airway dimensions in smokers. Chest 2012 Oct 8; \[Epub ahead of print\]


- 6\. Diaz A.A., Valim C., Yamashiro T., et. al.: Airway count and emphysema assessed by chest CT imaging predicts clinical outcome in smokers. Chest 2012; 138: pp. 880-887.


- 7\. Estepar R.S., Washko G.G., Silverman E.K., et. al.: Accurate airway wall estimation using phase congruency. Med Image Comput Comput Assist Interv 2006; 9: pp. 125-134.


- 8\. Foreman M.G., Zhang L., Murphy J., et. al.: Early-onset chronic obstructive pulmonary disease is associated with female sex, maternal factors, and African American race in the COPDGene Study. Am J Respir Crit Care Med 2011; 184: pp. 414-420.


- 9\. Gevenois P.A., de Maertelaer V., De Vuyst P., et. al.: Comparison of computed density and macroscopic morphometry in pulmonary emphysema. Am J Respir Crit Care Med 1995; 152: pp. 653-657.


- 10\. Gould G.A., MacNee W., McLean A., et. al.: CT measurements of lung density in life can quantitate distal airspace enlargement–an essential defining feature of human emphysema. Am Rev Respir Dis 1988; 137: pp. 380-392.


- 11\. Gould G.A., Redpath A.T., Ryan M., et. al.: Lung CT density correlates with measurements of airflow limitation and the diffusing capacity. Eur Respir J 1991; 4: pp. 141-146.


- 12\. Han M.K., Agusti A., Calverley P.M., et. al.: Chronic obstructive pulmonary disease phenotypes: the future of COPD. Am J Respir Crit Care Med 2010; 182: pp. 598-604.


- 13\. Han M.K., Kazerooni E.A., Lynch D.A., et. al.: Chronic obstructive pulmonary disease exacerbations in the COPDGene Study: associated radiologic phenotypes. Radiology 2011; 261: pp. 274-282.


- 14\. Hersh C.P., Washko G.R., Jacobson F.L., et. al.: Interobserver variability in the determination of upper lobe-predominant emphysema. Chest 2007; 131: pp. 424-431.


- 15\. Kim W.J., Silverman E.K., Hoffman E., et. al.: CT metrics of airway disease and emphysema in severe COPD. Chest 2009; 136: pp. 396-404.


- 16\. McDonough J.E., Yuan R., Suzuki M., et. al.: Small-airway obstruction and emphysema in chronic obstructive pulmonary disease. N Engl J Med 2011; 365: pp. 1567-1575.


- 17\. Ross J.C., Estepar R.S., Diaz A., et. al.: Lung extraction, lobe segmentation and hierarchical region assessment for quantitative analysis on high resolution computed tomography images. Med Image Comput Comput Assist Interv 2009; 12: pp. 690-698.


- 18\. Ross J.C., San Jose Estepar R., Kindlmann G., et. al.: Automatic lung lobe segmentation using particles, thin plate splines, and maximum a posteriori estimation. Med Image Comput Comput Assist Interv 2010; 13: pp. 163-171.


- 19\. San Jose Estepar R., Reilly J.J., Silverman E.K., et. al.: Three-dimensional airway measurements and algorithms. Proc Am Thorac Soc 2008; 5: pp. 905-909.


- 20\. Washko G.R., Dransfield M.T., Estepar R.S., et. al.: Airway wall attenuation: a biomarker of airway disease in subjects with COPD. J Appl Physiol 2009; 107: pp. 185-191.


- 21\. Washko G.R., Hunninghake G.M., Fernandez I.E., et. al.: Lung volumes and emphysema in smokers with interstitial lung abnormalities. N Engl J Med 2011; 364: pp. 897-906.


- 22\. Washko G.R., Lynch D.A., Matsuoka S., et. al.: Identification of early interstitial lung disease in smokers from the COPDGene Study. Acad Radiol 2010; 17: pp. 48-53.


- 23\. Yamashiro T., Matsuoka S., Bartholmai B.J., et. al.: Collapsibility of lung volume by paired inspiratory and expiratory CT scans: correlations with lung function and mean lung density. Acad Radiol 2010; 17: pp. 489-495.


- 24\. Yamashiro T., Matsuoka S., Estepar R.S., et. al.: Kurtosis and skewness of density histograms on inspiratory and expiratory CT scans in smokers. COPD 2011; 8: pp. 13-20.


- 25\. Yamashiro T., Matsuoka S., Estepar R.S., et. al.: Quantitative airway assessment on computed tomography in patients with alpha1-antitrypsin deficiency. COPD 2009; 6: pp. 468-477.


- 26\. Sorensen L., Nielsen M., Lo P., et. al.: Texture-based analysis of COPD: a data-driven approach. IEEE Trans Med Imaging 2012; 31: pp. 70-78.


- 27\. Uppaluri R., Hoffman E.A., Sonka M., et. al.: Computer recognition of regional lung disease patterns. Am J Respir Crit Care Med 1999; 160: pp. 648-654.


- 28\. Uppaluri R., Hoffman E.A., Sonka M., et. al.: Interstitial lung disease: a quantitative study using the adaptive multiple feature method. Am J Respir Crit Care Med 1999; 159: pp. 519-525.


- 29\. Bodduluri S., Newell J., Hoffman A., et. al.: Registration based lung mechanical analysis of chronic obstructive pulmonary disease (COPD) using a supervised machine learning framework. Acad Radiol 2013; 20: pp. 527-536.


- 30\. Adams D.: The Hitchhiker's Guide to the Galaxy.1995.Random House Publishing GroupNew York City, NY