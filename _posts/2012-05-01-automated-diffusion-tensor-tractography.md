---
title: Automated Diffusion Tensor Tractography
author: [CL_AT_PaoloGPNuciforaMDPhD,CL_AT_XiaoyingWuMS,CL_AT_EliasRMelhemMDPhD,CL_AT_RaquelEGurMDPhD,CL_AT_RubenCGurPhD,CL_AT_RaginiVermaPhD]
date: 2012-05-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 19, Issue 5]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Diffusion tensor tractography offers a unique perspective of white matter anatomy, but proper delineation of white matter tracts of interest generally requires the active involvement of an expert neuroanatomist. The investigators describe the implementation of an automated tractographic method requiring no user input and compare its results to those from user-driven tractography.

## Materials and Methods

Fourteen healthy volunteers underwent diffusion tensor imaging at 3 T. Images were registered to a standard template, and predefined seed regions containing tract termini were transformed into subject space for use in unsupervised probabilistic tractography. The output was compared to the results of user-driven tractography performed on the same subjects.

## Results

After the selection of suitable smoothing kernels and thresholds, the results of automated tractography closely approximated those of user-driven tractography. The main bodies of the cingulum, inferior fronto-occipital fasciculus, and inferior longitudinal fasciculus were depicted equally well by both methods. Discrepancies mainly arose at the periphery of these tracts, where anatomic uncertainty tends to be greatest.

## Conclusions

Automated tractography can be used to depict white matter anatomy without need for user intervention, particularly if the main body of the tract is of greatest interest.

Diffusion tensor tractography is a recently developed imaging modality that can demonstrate the anatomy of white matter tracts in vivo . It is based on the observation that the diffusion of water in the brain occurs preferentially in directions parallel to axon bundles, which can be measured with an appropriate set of directionally encoded diffusion-weighted images . Because axons extend over multiple voxels, white matter tracts can be parceled as regions of directionally coherent diffusion tensors.

Tractography has found growing use in several clinical settings. However, several factors have constrained the use of tractography in routine practice. Among these is the operator dependence of its output. Typically, tractographic results are produced through an interactive process that relies on an experienced user to identify a “seed,” a likely location of each white matter tract. Tractography fibers are then inspected by the user and rejected if they do not conform to known white matter tract anatomy. Obtaining accurate and reproducible depictions of white matter can be time consuming, and user-introduced bias may complicate a population-based analysis . Semiautomated methods have been proposed to reduce operator dependence by using information in the neighborhood of a minimal seed region to improve seed reproducibility .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

## Image Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## User-driven Tractography

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Automated Tractography

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Summary of method used to obtained automated tractographic results. Diffusion tensor imaging data were registered to a standard atlas to import predefined labels into subject space. The labels were converted to seed regions located at the termini of white matter tracts of interest. Unsupervised probabilistic tractography was used to generate probability maps of where each tract was likely to exist.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedDiffusionTensorTractography/0_1s20S1076633212000372.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

J(A,B)=\|A∩B\|\|A∪B\|.
J

(

A

,

B

)

=

\|

A

∩

B

\|

\|

A

∪

B

\|

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison of Tractographic Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Tractography of the cingulum ( top ), inferior fronto-occipital fasciculus ( middle ), and inferior longitudinal fasciculus ( bottom ) of one of the subjects in the training set. User-driven tractographic fibers ( left ) are compared to maximum intensity projections of automated tractographic results ( right ). The automated tractographic results are color coded to indicate their probability values. Tractographic results are superimposed on b = 0 s 2 /mm diffusion-weighted images.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedDiffusionTensorTractography/1_1s20S1076633212000372.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Jaccard similarity coefficients between automated and user-driven tractography using various postprocessing criteria. Twelve automated tractographic maps contributed from four randomly selected subjects were used to improve the consistency between these two methods. Automated tractographic maps were subjected to Gaussian smoothing kernels of varying sizes and subjected to a range of thresholds. User-driven tractographic results were held as a reference. The maximal Jaccard coefficient was achieved with a smoothing kernel of 3 mm and a threshold of 0.02.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedDiffusionTensorTractography/2_1s20S1076633212000372.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Qualitative comparison of automated tractography to user-driven tractography. Maximum intensity projections of the cingulum ( top ), inferior fronto-occipital fasciculus ( middle ), and inferior longitudinal fasciculus ( bottom ) are shown from a representative subject. Voxels recognized by both methods as belonging to the tract of interest are shown in red. Voxels recognized only by user-driven tractography are shown in green. Voxels recognized only by automated tractography are shown in blue. For all three white matter tracts, the main body of the tract was recognized by both methods.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/AutomatedDiffusionTensorTractography/3_1s20S1076633212000372.jpg)

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

## Conclusions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Conturo T.E., Lori N.F., Cull T.S., et. al.: Tracking neuronal fiber pathways in the living human brain. Proc Natl Acad Sci U S A 1999; 96: pp. 10422-10427.


- 2\. Le Bihan D., Mangin J.F., Poupon C., et. al.: Diffusion tensor imaging: concepts and applications. J Magn Reson Imaging 2001; 13: pp. 534-546.


- 3\. Stieltjes B., Kaufmann W.E., van Zijl P.C., et. al.: Diffusion tensor imaging and axonal tracking in the human brainstem. Neuroimage 2001; 14: pp. 723-735.


- 4\. Ciccarelli O., Parker G.J., Toosy A.T., et. al.: From diffusion tractography to quantitative white matter tract measures: a reproducibility study. Neuroimage 2003; 18: pp. 348-359.


- 5\. Wakana S., Caprihan A., Panzenboeck M.M., et. al.: Reproducibility of quantitative tractography methods applied to cerebral white matter. Neuroimage 2007; 36: pp. 630-644.


- 6\. Nucifora P.G., Verma R., Melhem E.R., et. al.: Leftward asymmetry in relative fiber density of the arcuate fasciculus. Neuroreport 2005; 16: pp. 791-794.


- 7\. Byrnes T.J., Barrick T.R., Bell B.A., et. al.: Semiautomatic tractography: motor pathway segmentation in patients with intracranial vascular malformations. J Neurosurg 2009; 111: pp. 132-140.


- 8\. O'Donnell L.J., Kubicki M., Shenton M.E., et. al.: A method for clustering white matter fiber tracts. AJNR Am J Neuroradiol 2006; 27: pp. 1032-1036.


- 9\. Hagler D.J., Ahmadi M.E., Kuperman J., et. al.: Automated white-matter tractography using a probabilistic diffusion tensor atlas: application to temporal lobe epilepsy. Hum Brain Mapp 2008; 30: pp. 1535-1547.


- 10\. Thottakara P., Lazar M., Johnson S.C., et. al.: Application of Brodmann's area templates for ROI selection in white matter tractography studies. Neuroimage 2006; 29: pp. 868-878.


- 11\.  Nucifora PG, Melhem ER, Loughead JW, et al. Tract-specific effects of schizophrenia demonstrated with quantitative MR diffusion tractography. Presented at: 15th Scientific Meeting, International Society for Magnetic Resonance in Medicine; 2007.


- 12\. Lawes I.N., Barrick T.R., Murugam V., et. al.: Atlas-based segmentation of white matter tracts of the human brain using diffusion tensor tractography and comparison with classical dissection. Neuroimage 2008; 39: pp. 62-79.


- 13\. Park H.J., Kim J.J., Lee S.K., et. al.: Corpus callosal connection mapping using cortical gray matter parcellation and DT-MRI. Hum Brain Mapp 2008; 29: pp. 503-516.


- 14\.  Yendiki A, Stevens A, Augustinack J, et al. Fully automated probabilistic white-matter tractography with anatomical priors: application to Huntington's disease. Presented at: 17th Scientific Meeting, International Society for Magnetic Resonance in Medicine; 2009.


- 15\.  Kolbe S, Bajraszewski C, Chapman C, et al. Optic radiation abnormalities after optic neuritis. Presented at: 17th Scientific Meeting, International Society for Magnetic Resonance in Medicine; 2009.


- 16\. Gutman D.A., Holtzheimer P.E., Behrens T.E., et. al.: A tractography analysis of two deep brain stimulation white matter targets for depression. Biol Psychiatry 2009; 65: pp. 276-282.


- 17\. Behrens T.E.J., Johansen-Berg H., Woolrich M.W., et. al.: Non-invasive mapping of connections between human thalamus and cortex using diffusion imaging. Nature Neurosci 2003; 6: pp. 750-757.


- 18\. Whitford T.J., Kubicki M., Ghorashi S., et. al.: Predicting inter-hemispheric transfer time from the diffusion properties of the corpus callosum in healthy individuals and schizophrenia patients: a combined ERP and DTI study. Neuroimage 2011; 54: pp. 2318-2329.


- 19\. Mori S., Crain B.J., Chacko V.P., et. al.: Three-dimensional tracking of axonal projections in the brain by magnetic resonance imaging. Ann Neurol 1999; 45: pp. 265-269.


- 20\. Masutani Y., Aoki S., Abe O., et. al.: MR diffusion tensor imaging: recent advance and new techniques for diffusion tensor visualization. Eur J Radiol 2003; 46: pp. 53-66.


- 21\. Catani M., Thiebaut de Schotten M.: A diffusion tensor imaging tractography atlas for virtual in vivo dissections. Cortex 2008; 44: pp. 1105-1132.


- 22\. Wakana S., Jiang H., Nagae-Poetscher L.M., et. al.: Fiber tract-based atlas of human white matter anatomy. Radiology 2004; 230: pp. 77-87.


- 23\.  Nucifora PGP, Wu X, Melhem ER, et al. Automated generation of diffusion tensor tractography maps. Presented at: 46th Annual Meeting of the American Society of Neuroradiology; 2008.


- 24\. Shen D., Davatzikos C.: HAMMER: hierarchical attribute matching mechanism for elastic registration. IEEE Trans Med Imaging 2002; 21: pp. 1421-1439.


- 25\. Tzourio-Mazoyer N., Landeau B., Papathanassiou D., et. al.: Automated anatomical labeling of activations in SPM using a macroscopic anatomical parcellation of the MNI MRI single-subject brain. Neuroimage 2002; 15: pp. 273-289.


- 26\. Mori S., van Zijl P.C.: Fiber tracking: principles and strategies—a technical review. NMR Biomed 2002; 15: pp. 468-480.


- 27\. Zhang W., Olivi A., Hertig S.J., et. al.: Automated fiber tracking of human brain white matter using diffusion tensor imaging. Neuroimage 2008; 42: pp. 771-777.


- 28\. Zhang Y., Zhang J., Oishi K., et. al.: Atlas-guided tract reconstruction for automated and comprehensive examination of the white matter anatomy. Neuroimage 2010; 52: pp. 1289-1301.


- 29\. Hua K., Zhang J., Wakana S., et. al.: Tract probability maps in stereotaxic spaces: analyses of white matter anatomy and tract-specific quantification. Neuroimage 2008; 39: pp. 336-347.


- 30\. Reich D.S., Ozturk A., Calabresi P.A., et. al.: Automated vs. conventional tractography in multiple sclerosis: variability and correlation with disability. Neuroimage 2010; 49: pp. 3047-3056.


- 31\. Behrens T.E., Johansen-Berg H.: Relating connectional architecture to grey matter function using diffusion imaging. Philos Trans R Soc Lond B Biol Sci 2005; 360: pp. 903-911.


- 32\. Cook P.A., Zhang H., Avants B.B., et. al.: An automated approach to connectivity-based partitioning of brain structures. Med Image Computing Computer Assist Interv 2005; 8: pp. 164-171.


- 33\. Clatworthy P., Williams G., Acosta-Cabronero J., et. al.: Probabilistic tractography of the optic radiations—an automated method and anatomical validation. Neuroimage 2010; 49: pp. 2001-2012.


- 34\. Kubicki M., Westin C.F., Nestor P.G., et. al.: Cingulate fasciculus integrity disruption in schizophrenia: a magnetic resonance diffusion tensor imaging study. Biol Psychiatry 2003; 54: pp. 1171-1180.


- 35\. Concha L., Gross D.W., Beaulieu C.: Diffusion tensor tractography of the limbic system. AJNR Am J Neuroradiol 2005; 26: pp. 2267-2274.


- 36\. Lee C.E., Danielian L.E., Thomasson D., et. al.: Normal regional fractional anisotropy and apparent diffusion coefficient of the brain measured on a 3 T MR scanner. Neuroradiology 2008; 51: pp. 3-9.


- 37\. O'Donnell L.J., Westin C.F., Golby A.J.: Tract-based morphometry for white matter group analysis. Neuroimage 2009; 45: pp. 832-844.


- 38\. Morris D.M., Embleton K.V., Parker G.J.: Probabilistic fibre tracking: differentiation of connections from chance events. Neuroimage 2008; 42: pp. 1329-1339.