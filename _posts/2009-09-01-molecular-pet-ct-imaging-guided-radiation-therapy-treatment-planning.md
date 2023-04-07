---
title: Molecular PET/CT Imaging-Guided Radiation Therapy Treatment Planning
author: [CL_AT_HabibZaidiPhDPD,CL_AT_HansjrgVeesMD,CL_AT_MichaelWissmeyerMD]
date: 2009-09-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 16, Issue 9]
tags: [Journals,General Radiology]
---
The role of positron emission tomography (PET) during the past decade has evolved rapidly from that of a pure research tool to a methodology of enormous clinical potential.  18 F-fluorodeoxyglucose (FDG)-PET is currently the most widely used probe in the diagnosis, staging, assessment of tumor response to treatment, and radiation therapy planning because metabolic changes generally precede the more conventionally measured parameter of change in tumor size. Data accumulated rapidly during the last decade, thus validating the efficacy of FDG imaging and many other tracers in a wide variety of malignant tumors with sensitivities and specificities often in the high 90 percentile range. As a result, PET/computed tomography (CT) had a significant impact on the management of patients because it obviated the need for further evaluation, guided further diagnostic procedures, and assisted in planning therapy for a considerable number of patients. On the other hand, the progress in radiation therapy technology has been enormous during the last two decades, now offering the possibility to plan highly conformal radiation dose distributions through the use of sophisticated beam targeting techniques such as intensity-modulated radiation therapy (IMRT) using tomotherapy, volumetric modulated arc therapy, and many other promising technologies for sculpted three-dimensional (3D) dose distribution. The foundation of molecular imaging-guided radiation therapy lies in the use of advanced imaging technology for improved definition of tumor target volumes, thus relating the absorbed dose information to image-based patient representations. This review documents technological advancements in the field concentrating on the conceptual role of molecular PET/CT imaging in radiation therapy treatment planning and related image processing issues with special emphasis on segmentation of medical images for the purpose of defining target volumes. There is still much more work to be done and many of the techniques reviewed are themselves not yet widely implemented in clinical settings.

Advances in genomics, proteomics, and biomedical technology are changing the practice of medicine in a profound way . The role of positron emission tomography (PET) during the past decade has evolved rapidly from that of a pure research tool to a methodology of enormous clinical potential .  18 F-fluorodesoxyglucose (FDG)-PET is widely used in the diagnosis, staging, and assessment of tumor response to therapy, since metabolic changes generally precede the more conventionally measured parameter of change in tumor size. Data accumulated rapidly during the last decade to validate the efficacy of FDG-PET imaging in a wide variety of malignant tumors with sensitivities and specificities often in the high 90 percentile range. Although molecular PET/CT imaging is an obvious choice, the design of specific clinical protocols is still under development. The tracers or combinations of tracers to be used (eg, for imaging metabolism, hypoxia, and cell proliferation), when and how the imaging should be done after therapy, the selection of optimal acquisition and processing protocols, and robust algorithms for accurately performing quantitative or semiquantitative analysis of data are still undetermined. Moreover, each tumor-therapy combination may need to be independently optimized and validated. There have been multiple studies that have demonstrated the role of PET/CT especially for oncologic applications . It should be emphasized that much worthwhile research was carried out. However, there are still many open questions offering many opportunities for future research.

Dual-modality techniques offer a critical advantage over separate computed tomography (CT) and PET scanning in correlating functional and anatomical images without moving the patient (other than table translation). Different designs of combined PET/CT scanners were developed for diagnostic purposes in clinical oncology and have been commercially available since the beginning of this century . This technique thereby produces anatomical and functional images with the patient in the same position and during a single procedure, which simplifies the image registration and fusion processes . In seeking to achieve accurate registration of the anatomical and functional data, dual-modality imaging offers several potential advantages over conventional imaging techniques. First, the PET and x-ray CT images are supplementary and complementary. PET images can identify areas of disease that are not apparent on the CT images alone . The latter provide an anatomical context that interpreters use to differentiate normal radiotracer uptake from that indicating disease and to help localize disease sites within the body. Second, the low noise x-ray CT data can be used to generate a patient-specific map of attenuation coefficients and other a priori anatomical data, which in turn are used to correct the PET emission data for errors from photon attenuation , scattered radiation , and other physical degrading factors such as partial volume effect . In these ways, the CT images can be used to improve both the visual quality and the quantitative accuracy of the correlated radiotracer data .

In parallel, radiation therapy (RT) has gone through a series of revolutions in the last two decades, now offering the possibility to produce highly conformal radiation dose distribution by using techniques such as intensity-modulated radiation therapy (IMRT) using tomotherapy, volumetric modulated arc therapy, and many other RT units for dose painting. The improved dose conformity and steep dose gradients have necessitated enhanced patient localization and beam targeting techniques for radiotherapy treatments . Components affecting the reproducibility of target position during and between subsequent fractions of RT include the displacement of internal organs between fractions and internal organ motion within a fraction. Image-guided radiation therapy (IGRT) uses advanced imaging technology to better define the tumor target and is the key to reducing and ultimately eliminating the uncertainties .

In general, anatomical cross-sectional images (CT and magnetic resonance imaging \[MRI\]) are used to delineate the treatment volumes, and radiation treatment portals are designed to entirely cover the planning treatment volume and deliver a uniform dose distribution to it. The ability of IMRT to deliver nonuniform dose patterns by design has raised the question of how to “dose paint” and “dose sculpt” . In this regard, it was suggested that molecular imaging using PET/CT may be of additional value even if the issue is still controversial . PET allows a more correct delineation of gross tumor volume (GTV) and planning target volume. It should, however, be emphasized that much scientific research and clinical studies are needed before this potential can be realized. The recent enthusiasm in the use PET/CT-guided RT treatment planning is stimulated by the commercial availability of advanced imaging technologies and their incorporation in treatment planning software offering the possibility to integrate data from different departments and even from different hospitals into RT treatment planning . One of the main difficulties encountered by radiation oncologists is the delineation of the treatment volume from noisy PET data . Identification of lesion boundaries in general is not a trivial problem as whole-body images exhibit inhomogeneity . Another challenge for the industry is to provide an easy, open, and vendor-independent platform for incorporating the PET/CT information in a DICOM-compatible format into the RT dose planning software.

This review documents technological advancements in the field focusing on the conceptual role of molecular PET/CT imaging in RT treatment planning and related image processing issues with special emphasis on segmentation of PET images for the purpose of defining target volumes.

## Progress in RT technology

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

## Advances in anatomolecular PET/CT imaging instrumentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Progress in new cancer-specific PET probes

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Molecular PET/CT IGRT treatment planning

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Current Evidence of FDG-PET/CT Utilization in Target Volume Definition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Photograph of the Biograph 16 HI-REZ PET/CT scanner (Siemens Medical Systems, Erlangen, Germany) installed at Geneva University Hospital and used routinely for radiation therapy simulation and positron emission tomography/computed tomography–based treatment planning. The scanner is equipped with a flat-panel tabletop and external room lasers. The 70 cm large diameter bore allows most patients to be imaged in the treatment position with the use of suitable immobilization devices.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MolecularPETCTImagingGuidedRadiationTherapyTreatmentPlanning/0_1s20S1076633209001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Summary of Recent Contributions Assessing the Impact of PET/CT on Target Volume Definition in FDG Avid Malignancies


Localization Reference_n_ Reference Modality GTV Delineation Method Impact of PET on GTV Other Important Findings Head and neck 18 CT and MRI Manually: CT and MRI Significant reduction of target volumes (up to 18%) Significant reduction of mean dose to ipsilateral (31%) and contralateral (11%) parotids Automated: PET 38 CT Manually: CT and PET/CT Significant change of GTV, no significant change of PTV 22 CT Manually: CT, PET and fused PET/CT Significant change of GTV Change of TNM stage in 22% 20 CT Manually: CT and fused PET/CT No significant differences between GTV CT and GTV PET/CT Significantly higher interobserver agreement for GTV PET/CT when compared to GTV CT 16 CT Manually on CT and fused PET/CT Higher interobserver variability for GTV PET/CT than GTV CT 25 CT CT: manually Significantly higher interobserver concordance for GTV PET/CT than for GTV CT PET/CT: manually based on halo phenomenon Esophageal cancer 21 CT Manually: PET and CT Median 38% of GTV-PET not covered by GTV-CT Clinical stage altered in 8/21 patients (38%); change of intent (curative -> palliative) in 5/21 patients (24%) 16 CT Manually: CT and PET/CT Smaller GTV in 62.5% 25 CT, EUS Manually: CT and PET/CT GTV PET < GTV CT EUS detected significantly more patients with locoregional lymphadenopathy 10 CT Manually: CT and PET/CT NA Reduced intra- and interobserver variability when adding the PET information NSCLC 19 CT Halo phenomenon Up to 25% GTV modification in 10/19 patients. (52%) Interobserver variability significantly improved (up to 84%) by adding the PET information 52 Pathologic specimen; CT NA NA Better correlation between real tumor volume and PET/CT than PET or CT alone 21 CT Manually Significant changes of CTV in 55% Major GTV changes based on inclusion or exclusion of lymph nodes 21 CT Manually Significant changes of GTV in 67% Significant dose escalation possible while respecting dose constraints for organs at risk 33 CT Manually and automated (source to background ratio) GTV PET/CT smaller than GTV CT Reduced interobserver variability using automatic GTV delineation; PET/CT best correlated with pathology 21 CT Manually: CT and fused PET/CT Significant change in 39% TNM staging modified in 48%; Change of treatment modality (curative -> palliative) in 14% Breast cancer (tumor bed) 12 CT Manually: CT and PET PTV PET greater than PTV CT (median volume ratio: 1.16) Inadequate coverage of PET/CT based GTV by CT PTV in 9/12 patients (75%) Breast cancer (axilla) 15 CT Manually: CT and PET Increase of axillary dose in 11/13 patients (85%) when adding PET information Cervical cancer 51 CT Manually: CT and PET/CT Discordant CTV between PET and CT in 37% of patients According to PET more extensive nodal involvement in 27% of patients 11 Intracavitary brachytherapy planning Manually: PET Significantly better dose coverage of the tumor without significant dose increase to bladder and rectum Hodgkin lymphoma 30 CT Manually: CT and PET Increase of target volumes of 8–87% in 7/30 patients (23%); decrease of target volume of 18 and 30% in 2/30 patients (7%) Rectal cancer 20 CT Manually: CT and PET/CT Mean GTV PET/CT < GTV CT; PTV altered by PET/CT in 17% Change of treatment fields and patient management in 26% 25 CT Manually: fused PET/CT PET/CT-GTV significantly greater (mean 25.4%) than CT-GTV Clinical stage or treatment purpose altered in 4/25 patients (24%)

PET, positron emission tomography; CT, computed tomography; FDG, fluorodeoxyglucose; GTV, gross tumor volume; MRI, magnetic resonance imaging; EUS, endoscopic ultrasound: GTV, gross tumor volume; CTV, clinical target volume.


The number of patients ( _n_ ) enrolled in the study protocol, impact of PET on GTV delineation and other important findings are also given.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Head-and-neck Tumors

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Patient with stage IIA Hodgkin lymphoma. The gross tumor volumes delineated on the positron emission tomography/computed tomography (PET/CT) scan is shown in green color. PET revealed an additional 7 mm paratracheal lymph node (arrow) that was missed on CT.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MolecularPETCTImagingGuidedRadiationTherapyTreatmentPlanning/1_1s20S1076633209001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Lung Cancer

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Patient with cervical lymph node metastases of squamous cell carcinoma from an unknown primary tumor. The gross tumor volume delineated on the positron emission tomography/computed tomography scan (red color) revealed the primary tumor located on the base of tongue (arrow) that was not identified on diagnostic magnetic resonance imaging, computed tomography, and panendoscopy.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MolecularPETCTImagingGuidedRadiationTherapyTreatmentPlanning/2_1s20S1076633209001445.jpg)

![Figure 4, Patient with poorly differentiated carcinoma of the left lung. Fused positron emission tomography/computed tomography (CT) images detected two additional 18 F-fluorodeoxyglucose positive mediastinal lymph nodes of 6 mm. The diagnostic CT scan performed on the same day did not classify these lymph nodes as suspicious.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MolecularPETCTImagingGuidedRadiationTherapyTreatmentPlanning/3_1s20S1076633209001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Esophageal Cancer

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Gynecological Tumors

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Rectal Cancer

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Lymphoma

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Sagittal and axial positron emission tomography/computed tomography (PET/CT) images of a patient with non–small-cell lung cancer of the right upper lobe. PET/CT allowed excluding associated atelectasis that was impossible using a diagnostic quality CT alone.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MolecularPETCTImagingGuidedRadiationTherapyTreatmentPlanning/4_1s20S1076633209001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Breast Cancer

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Other Tumors

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Novel Promising Probes beyond FDG for of PET-guided Target Volume Delineation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 2


Summary of Recent Contributions assessing the Impact of non-FDG PET Tracers for Target Volume Definition in Radiotherapy


Target Tracer Localization Reference_n_ Reference Method(s) Results Complementary Findings Hypoxia 18  F-MISO Head and neck 10 FDG PET/CT, CT, MRI Dose escalation to hypoxic tissue feasible in all cases (84–105 Gy) without exceeding normal tissue tolerance Various levels of hypoxia demonstrated by heterogeneous 18F-MISO distribution 18  F-FAZA Head and neck 18 CT Median GTV/FAZA represented 10.8% (0.7–52%) of the GTV/CT in the primary and 8.3% (2.2–51.3%) in the lymph nodes. No significant correlation between GTV/FAZA and GTV/CT for the primary, significant correlation for the lymph nodes. Different patterns of hypoxia influenced dose painting. 60  Cu-ATSM Cervical cancer 14 FDG PET, clinical follow-up ATSM uptake significant predictor of progression free and overall survival Frequency of locoregional nodal metastases significantly higher in hypoxic tumors; FDG uptake did not correlate with tumor hypoxia Amino acid metabolism 11  C-Methionine Meningioma 32 CT, MRI Methionine PET beneficial in 29/32 patients (91%) due to identification of small tumor portions not identified by CT or MRI. Mean GTV enlargement due to PET: 9.4 ± 10.7% Meningioma 10 CT, MRI Significant decrease of interobserver variability of GTV when adding the PET information ( _r_ = 0.855 ≥ 0.988) PET information helpful in GTV delineation in sinus cavernosus, orbit and skull base areas 18  F-FET Malignant glioma 45 MRI FET PET sensitivity 100%, specificity 92.9%; MRI sensitivity 93.5%, specificity 50% Concordance between FET PET and MRI in 37 cases, discordance in 8 cases ( _P_ < .01) Malignant glioma 24 Pathology ( _n_ = 9); clinical follow-up Time course and pattern of serial FET PET acquisitions correlate well with success of intracavitary radioimmunotherapy Threshold of 2.4 (tumor/background ratio) allows for discrimination between recurrence and inflammation (sensitivity 88%, specificity 100%) Malignant glioma 18 PET, MRI The majority of GTVs defined on various PET-based segmentation techniques were usually smaller than GTV  MRI  (67% of cases) PET detected frequently tumours that are not visible on MRI and added substantially tumour extension outside the GTV  MRI  in 6 patients (33% of cases) Cell membranes/fatty acid metabolism 18  F-Fluorocholine Prostate cancer 10 CT Comparable results for target volumes derived from CT and PET. Optimal concordance for lateral and craniocaudal dimensions was achieved when using a signal threshold of 23.0 ± 2.6%, for anterior-posterior dimensions when applying a threshold of 49.5 ± 4.6% 3-dimensional conformal treatment planning on Fluorocholine PET and CT alone delivered comparable doses to the rectal wall Somatostatin receptors 68  Ga-DOTA-TOC Meningioma 26 CT, MRI Significant modification of PTV based on DOTA-TOC PET in 19/26 patients (73%). Compared to CT PTVs alone, trimodal outlined PTVs decreased in 9/26 patients (35%) and increased in 10/26 patients (38%) DOTA-TOC PET delivered additional information on tumor extension in all patients. In one patient, only DOTA-TOC PET was able to detect the lesion

ATSM, diacetyl-bis(N4-methylthiosemicarbazone); PET, positron emission tomography; CT, computed tomography; FDG, fluorodeoxyglucose; GTV, gross tumor volume; MRI, magnetic resonance imaging.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Markers of Tumor Hypoxia

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Amino Acids

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Example of a patient with a glioblastoma (World Health Organization IV) in the left temporal and frontal areas. The contrast enhanced T2-weighted magnetic resonance images and the 18 F-fluoro-ethyl-tyrosine positron emission tomography show substantially different gross tumor volume extension on the two modalities (black color) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MolecularPETCTImagingGuidedRadiationTherapyTreatmentPlanning/5_1s20S1076633209001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Cell Membranes/Fatty Acid Metabolism

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Patient with biochemically recurrent prostate cancer 6 years after initial radiotherapy. 18 F-choline positron emission tomography/computed tomography (PET/CT) showed a recurrent tumor in the left posterior lobe. This tumor was confirmed by bilateral endorectal biopsy of the prostate. The gross tumor volume delineated for partial reirradiation of the prostate by intensity-modulated radiotherapy is shown (red color) .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MolecularPETCTImagingGuidedRadiationTherapyTreatmentPlanning/6_1s20S1076633209001445.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Proliferation Markers

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Tracers for Neuroendocrine Tumors

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## PET/CT-guided delineation of target volumes

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Validation and Comparison of Techniques

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Challenges and future directions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Cherry S.R.: In vivo molecular and genomic imaging: new challenges for imaging physics. Phys Med Biol 2004; 49: pp. R13-R48.


- 2\. Zaidi H., Alavi A.: Current trends in PET and combined (PET/CT and PET/MR) systems design. PET Clin 2007; 2: pp. 109-123.


- 3\. von Schulthess G.K., Steinert H.C., Hany T.F.: Integrated PET/CT: current applications and future directions. Radiology 2006; 238: pp. 405-422.


- 4\. Juweid M.E., Cheson B.D.: Positron-emission tomography and assessment of cancer therapy. N Engl J Med 2006; 354: pp. 496-507.


- 5\. Blodgett T.M., Meltzer C.C., Townsend D.W.: PET/CT: form and function. Radiology 2007; 242: pp. 360-385.


- 6\. Czernin J., Allen-Auerbach M., Schelbert H.R.: Improvements in cancer staging with PET/CT: literature-based evidence as of september 2006. J Nucl Med 2007; 48: pp. 78S-88S.


- 7\. Townsend D.W.: Positron emission tomography/computed tomography. Sem Nucl Med 2008; 38: pp. 152-166.


- 8\. Hasegawa B., Zaidi H.: Dual-modality imaging: more than the sum of its components.Zaidi H.Quantitative analysis in nuclear medicine imaging.2006.SpringerNew York:pp. 35-81.


- 9\. Goerres G.W., von Schulthess G.K., Steinert H.C.: Why most PET of lung and head-and-neck cancer will be PET/CT. J Nucl Med 2004; 45: pp. 66S-71S.


- 10\. Zaidi H., Montandon M.-L., Alavi A.: Advances in attenuation correction techniques in PET. PET Clin 2007; 2: pp. 191-217.


- 11\. Zaidi H., Montandon M.-L.: Scatter compensation techniques in PET. PET Clin 2007; 2: pp. 219-234.


- 12\. Soret M., Bacharach S.L., Buvat I.: Partial-volume effect in PET tumor imaging. J Nucl Med 2007; 48: pp. 932-945.


- 13\.  Zaidi H, El Naqa I. PET-guided delineation of radiation therapy treatment volumes: a review of image segmentation techniques. Med Image Anal. In press.


- 14\. Bortfeld T.: IMRT: a review and preview. Phys Med Biol 2006; 51: pp. R363-R379.


- 15\. Ling C.C., Yorke E., Fuks Z.: From IMRT to IGRT: frontierland or neverland?. Radiother Oncol 2006; 78: pp. 119-122.


- 16\. Bentzen S.M.: Theragnostic imaging for radiation oncology: dose-painting by numbers. Lancet Oncol 2005; 6: pp. 112-117.


- 17\. Bentzen S.M.: Dose painting and theragnostic imaging: towards the prescription, planning and delivery of biologically targeted dose distributions in external beam radiation oncology. Cancer Treat Res 2008; 139: pp. 41-62.


- 18\. Chapman J.D., Bradley J.D., Eary J.F., et. al.: Molecular (functional) imaging for radiotherapy applications: an RTOG symposium. Int J Radiat Oncol Biol Phys 2003; 55: pp. 294-301.


- 19\. Grosu A.L., Wiedenmann N., Molls M.: Biological imaging in radiation oncology. Z Med Phys 2005; 15: pp. 141-145.


- 20\. Messa C., Di Muzio N., Picchio M., et. al.: PET/CT and radiotherapy. Q J Nucl Med Mol Imaging 2006; 50: pp. 4-14.


- 21\. Gregoire V., Haustermans K., Geets X., et. al.: PET-based treatment planning in radiotherapy: a new standard?. J Nucl Med 2007; 48: pp. 68S-77S.


- 22\. Lecchi M., Fossati P., Elisei F., et. al.: Current concepts on imaging in radiotherapy. Eur J Nucl Med Mol Imaging 2008; 35: pp. 821-837.


- 23\. Mah D., Chen C.C.: Image guidance in radiation oncology treatment planning: the role of imaging technologies on the planning process. Sem Nucl Med 2008; 38: pp. 114-118.


- 24\. Xing L., Wessels B.: The value of PET/CT is being over-sold as a clinical tool in radiation oncology. Med Phys 2005; 32: pp. 1457-1459.


- 25\. Pan T., Chen L., Orton C.G.: PET/CT will become standard practice for radiotherapy simulation and planning. Med Phys 2008; 35: pp. 3825-3827.


- 26\. Ollers M., Bosmans G., van Baardwijk A., et. al.: The integration of PET-CT scans from different hospitals into radiotherapy treatment planning. Radiother Oncol 2008; 87: pp. 142-146.


- 27\. Aristophanous M., Penney B.C., Pelizzari C.A.: The development and testing of a digital PET phantom for the evaluation of tumor volume segmentation techniques. Med Phys 2008; 35: pp. 3331-3342.


- 28\. Bernier J., Hall E.J., Giaccia A.: Radiation oncology: a century of achievements. Nat Rev Cancer 2004; 4: pp. 737-747.


- 29\. Webb S., Evans P.M.: Innovative techniques in radiation therapy: editorial, overview, and crystal ball gaze to the future. Semin Radiat Oncol 2006; 16: pp. 193-198.


- 30\. Perez C.A., Purdy J.A., Harms W., et. al.: Three-dimensional treatment planning and conformal radiation therapy: preliminary evaluation. Radiother Oncol 1995; 36: pp. 32-43.


- 31\. Stroom J.C., Korevaar G.A., Koper P.C., et. al.: Multiple two-dimensional versus three-dimensional PTV definition in treatment planning for conformal radiotherapy. Radiother Oncol 1998; 47: pp. 297-302.


- 32\. Dobbs H.J., Parker R.P.: The respective roles of the simulator and computed tomography in radiotherapy planning: a review. Clin Radiol 1984; 35: pp. 433-439.


- 33\. Lu R., Radke R.J., Happersett L., et. al.: Reduced-order parameter optimization for simplifying prostate IMRT planning. Phys Med Biol 2007; 52: pp. 849-870.


- 34\. Chang B.K., Timmerman R.D.: Stereotactic body radiation therapy: a comprehensive review. Am J Clin Oncol 2007; 30: pp. 637-644.


- 35\. Pan T., Lee T.Y., Rietzel E., et. al.: 4D-CT imaging of a volume influenced by respiratory motion on multi-slice CT. Med Phys 2004; 31: pp. 333-340.


- 36\. Rietzel E., Pan T., Chen G.T.: Four-dimensional computed tomography: image formation and clinical protocol. Med Phys 2005; 32: pp. 874-889.


- 37\. Keall P., Vedam S., George R., et. al.: The clinical implementation of respiratory-gated intensity-modulated radiotherapy. Med Dosim 2006; 31: pp. 152-162.


- 38\. Li X.A., Keall P.J.: Respiratory gating for radiation therapy is not ready for prime time. Med Phys 2007; 34: pp. 867-870.


- 39\. Li G., Citrin D., Camphausen K., et. al.: Advances in 4D medical imaging and 4D radiation therapy. Technol Cancer Res Treat 2008; 7: pp. 67-82.


- 40\. Erdi Y.E., Nehmeh S.A., Pan T., et. al.: The CT motion quantitation of lung lesions and its impact on PET-measured SUVs. J Nucl Med 2004; 45: pp. 1287-1292.


- 41\. Nehmeh S.A., Erdi Y.E., Pan T., et. al.: Four-dimensional (4D) PET/CT imaging of the thorax. Med Phys 2004; 31: pp. 3179-3186.


- 42\. Nehmeh S.A., Erdi Y.E., Pan T., Yorke E., et. al.: Quantitation of respiratory motion during 4D-PET/CT acquisition. Med Phys 2004; 31: pp. 1333-1338.


- 43\. Lamare F., Ledesma Carbayo M.J., Cresson T., et. al.: List-mode-based reconstruction for respiratory motion correction in PET using non-rigid body transformations. Phys Med Biol 2007; 52: pp. 5187-5204.


- 44\. Li T., Thorndyke B., Schreibmann E., et. al.: Model-based image reconstruction for four-dimensional PET. Med Phys 2006; 33: pp. 1288-1298.


- 45\. Nehmeh S.A., Erdi Y.E.: Respiratory motion in positron emission tomography/computed tomography: a review. Sem Nucl Med 2008; 38: pp. 167-176.


- 46\. Dawood M., Buther F., Jiang X., et. al.: Respiratory motion correction in 3-D PET data with advanced optical flow algorithms. IEEE Trans Med Imaging 2008; 27: pp. 1164-1175.


- 47\. Papathanassiou D., Becker S., Amir R., et. al.: Respiratory motion artefact in the liver dome on FDG PET/CT: comparison of attenuation correction with CT and a caesium external source. Eur J Nucl Med Mol Imaging 2005; 32: pp. 1422-1428.


- 48\. Osman M.M., Cohade C., Nakamoto Y., et. al.: Clinically significant inaccurate localization of lesions with PET/CT: frequency in 300 patients. J Nucl Med 2003; 44: pp. 240-243.


- 49\. Pan T., Mawlawi O., Nehmeh S.A., et. al.: Attenuation correction of PET images with respiration-averaged CT images in PET/CT. J Nucl Med 2005; 46: pp. 1481-1487.


- 50\. Xing L., Thorndyke B., Schreibmann E., et. al.: Overview of image-guided radiation therapy. Med Dosim 2006; 31: pp. 91-112.


- 51\. Shirato H., Shimizu S., Kitamura K., et. al.: Organ motion in image-guided radiotherapy: lessons from real-time tumor-tracking radiotherapy. Int J Clin Oncol 2007; 12: pp. 8-16.


- 52\. Xing L., Siebers J., Keall P.: Computational challenges for image-guided radiation therapy: framework and current research. Semin Rad Oncol 2007; 7: pp. 245-257.


- 53\. Fenwick J.D., Tome W.A., Soisson E.T., et. al.: Tomotherapy and other innovative IMRT delivery systems. Semin Radiat Oncol 2006; 16: pp. 199-208.


- 54\. Mackie T.R.: History of tomotherapy. Phys Med Biol 2006; 51: pp. R427-R453.


- 55\. Otto K.: Volumetric modulated arc therapy: IMRT in a single gantry arc. Med Phys 2008; 35: pp. 310-317.


- 56\. Cozzi L., Dinshaw K.A., Shrivastava S.K., et. al.: A treatment planning study comparing volumetric arc modulation with RapidArc and fixed field IMRT for cervix uteri radiotherapy. Radiother Oncol 2008; 89: pp. 180-191.


- 57\. Ling C.C., Zhang P., Archambault Y., et. al.: Commissioning and quality assurance of RapidArc radiotherapy delivery system. Int J Radiat Oncol Biol Phys 2008; 72: pp. 575-581.


- 58\. Brahme A.: Recent advances in light ion radiation therapy. Int J Radiat Oncol Biol Phys 2004; 58: pp. 603-616.


- 59\. Amaldi U.: Future trends in cancer therapy with particle accelerators. Z Med Phys 2004; 14: pp. 7-16.


- 60\. Brada M., Pijls-Johannesma M., De Ruysscher D.: Proton therapy in clinical practice: current clinical evidence. J Clin Oncol 2007; 25: pp. 965-970.


- 61\. Jakel O., Karger C.P., Debus J.: The future of heavy ion radiotherapy. Med Phys 2008; 35: pp. 5653-5663.


- 62\. Yoneoka Y., Tsumanuma I., Fukuda M., et. al.: Cranial base chordoma–long term outcome and review of the literature. Acta Neurochir (Wien) 2008; 150: pp. 773-778. discussion 778


- 63\. Pommier P., Liebsch N.J., Deschler D.G., et. al.: Proton beam radiation therapy for skull base adenoid cystic carcinoma. Arch Otolaryngol Head Neck Surg 2006; 132: pp. 1242-1249.


- 64\.  Delaney TF, Liebsch NJ, Pedlow FX, et al. Phase II study of high-dose photon/proton radiotherapy in the management of spine sarcomas. Int J Radiat Oncol Biol Phys. In press.


- 65\. Habrand J.L., Schneider R., Alapetite C., et. al.: Proton therapy in pediatric skull base and cervical canal low-grade bone malignancies. Int J Radiat Oncol Biol Phys 2008; 71: pp. 672-675.


- 66\. Rutz H.P., Weber D.C., Goitein G., et. al.: Postoperative spot-scanning proton radiation therapy for chordoma and chondrosarcoma in children and adolescents: initial experience at Paul Scherrer Institute. Int J Radiat Oncol Biol Phys 2008; 71: pp. 220-225.


- 67\. Combs S.E., Nikoghosyan A., Jaekel O., et. al.: Carbon ion radiotherapy for pediatric patients and young adults treated for tumors of the skull base. Cancer 2009; 115: pp. 1348-1355.


- 68\. Bennett G.W., Archambeau J.O., Archambeau B.E., et. al.: Visualization and transport of positron emission from proton activation in vivo. Science 1978; 200: pp. 1151-1153.


- 69\. Pawelke J., Byars L., Enghardt W., et. al.: The investigation of different cameras for in-beam PET imaging. Phys Med Biol 1996; 41: pp. 279-296.


- 70\. Crespo P., Shakirin G., Enghardt W.: On the detector arrangement for in-beam PET for hadron therapy monitoring. Phys Med Biol 2006; 51: pp. 2143-2163.


- 71\. Attanasi F., Belcari N., Del Guerra A., et. al.: Comparison of two dedicated ‘in beam’ PET systems via simultaneous imaging of (12)C-induced beta(+)-activity. Phys Med Biol 2009; 54: pp. N29-N35.


- 72\. Nassalski A., Kapusta M., Batsch T., et. al.: Comparative study of scintillators for PET/CT detectors. IEEE Trans Nucl Sci 2007; 54: pp. 3-10.


- 73\. Parodi K., Paganetti H., Cascio E., et. al.: PET/CT imaging for treatment verification after proton therapy: a study with plastic phantoms and metallic implants. Med Phys 2007; 34: pp. 419-435.


- 74\. Kirkby C., Stanescu T., Rathee S., et. al.: Patient dosimetry for hybrid MRI-radiotherapy systems. Med Phys 2008; 35: pp. 1019-1027.


- 75\. Hasegawa B.H., Gingold E.L., Reilly S.M., et. al.: Description of a simultaneous emission-transmission CT system. Proc SPIE 1990; 1231: pp. 50-60.


- 76\. Beyer T., Townsend D., Brun T., et. al.: A combined PET/CT scanner for clinical oncology. J Nucl Med 2000; 41: pp. 1369-1379.


- 77\. Townsend D., Kinahan P., Beyer T.: Attenuation correction for a combined 3D PET/CT scanner. Phys Medica 1996; 12: pp. 43-48.


- 78\. Kluetz P.G., Meltzer C.C., Villemagne V.L., et. al.: Combined PET/CT imaging in oncology. Impact on patient management. Clin Positron Imaging 2000; 3: pp. 223-230.


- 79\. Muehllehner G., Karp J.S.: Positron emission tomography. Phys Med Biol 2006; 51: pp. R117-R137.


- 80\. Zaidi H.: Recent developments and future trends in nuclear medicine instrumentation. Z Med Phys 2006; 16: pp. 5-17.


- 81\.  Thompson CJ. Instrumentation for positron emission mammography. PET Clin 2006; 1: pp. 33-38.


- 82\. Weinberg I.N.: Applications for positron emission mammography. Phys Med 2006; 21: pp. 132-137.


- 83\. Huber J.S., Choong W.S., Moses W.W., et. al.: Initial results of a positron tomograph for prostate imaging. IEEE Trans Nucl Sci 2006; 53: pp. 2653-2659.


- 84\. Surti S., Kuhn A., Werner M.E., et. al.: Performance of Philips Gemini TF PET/CT scanner with special consideration for its time-of-flight imaging capabilities. J Nucl Med 2007; 48: pp. 471-480.


- 85\. Karp J.S., Surti S., Daube-Witherspoon M.E., et. al.: Benefit of time-of-flight in PET: experimental and clinical results. J Nucl Med 2008; 49: pp. 462-470.


- 86\. Brenner D.J., Hall E.J.: Computed tomography-an increasing source of radiation exposure. N Engl J Med 2007; 357: pp. 2277-2784.


- 87\. Mori S., Endo M., Tsunoo T., et. al.: Physical performance evaluation of a 256-slice CT-scanner for four-dimensional imaging. Med Phys 2004; 31: pp. 1348-1356.


- 88\. Klingebiel R., Siebert E., Diekmann S., et. al.: 4-D Imaging in cerebrovascular disorders by using 320-slice CT: feasibility and preliminary clinical experience. Acad Radiol 2009; 16: pp. 123-129.


- 89\. Kalender W.A.: X-ray computed tomography. Phys Med Biol 2006; 51: pp. R29-R43.


- 90\. Boone J.M.: Multidetector CT: opportunities, challenges, and concerns associated with scanners with 64 or more detector rows. Radiology 2006; 241: pp. 334-337.


- 91\. Steinert H.C., von Schulthess G.K.: Initial clinical experience using a new integrated in-line PET/CT system. Br J Radiol 2002; 73: pp. S36-S38.


- 92\. Zaidi H.: Is radionuclide transmission scanning obsolete for dual-modality PET/CT systems?. Eur J Nucl Med Mol Imaging 2007; 34: pp. 815-818.


- 93\. Alavi A., Mavi A., Basu S., Fischman A.: Is PET-CT the only option?. Eur J Nuc Med Mol Imaging 2007; 34: pp. 819-821.


- 94\. Gambhir S., Czernin J., Schwimmer J., et. al.: A tabulated summary of the FDG PET literature. J Nucl Med 2001; 45: pp. 1S-93S.


- 95\. Lardinois D., Weder W., Hany T.F., et. al.: Staging of non-small-cell lung cancer with integrated positron-emission tomography and computed tomography. N Engl J Med 2003; 348: pp. 2500-2507.


- 96\. Bar-Shalom R., Yefemov N., Guralnik L., et. al.: Clinical performance of PET/CT in evaluation of cancer: additional value for diagnostic imaging and patient management. J Nucl Med 2003; 44: pp. 1200-1209.


- 97\. Cohade C., Wahl R.L.: Applications of positron emission tomography/computed tomography image fusion in clinical positron emission tomography—clinical use, interpretation, methods, diagnostic improvements. Semin Nucl Med 2003; 33: pp. 228-237.


- 98\. Cherry S.R.: Multimodality in vivo imaging systems: twice the power or double the trouble?. Annu Rev Biomed Eng 2006; 8: pp. 35-62.


- 99\. Zaidi H., Mawlawi O.: Simultaneous PET/MR will replace PET/CT as the molecular multimodality imaging platform of choice. Med Phys 2007; 34: pp. 1525-1528.


- 100\. Pichler B.J., Wehrl H.F., Kolb A., et. al.: Positron emission tomography/magnetic resonance imaging: the next generation of multimodality imaging?. Sem Nucl Med 2008; 38: pp. 199-208.


- 101\. Schlemmer H.P., Pichler B.J., Schmand M., et. al.: Simultaneous MR/PET imaging of the human brain: feasibility study. Radiology 2008; 248: pp. 1028-1035.


- 102\. Zaidi H., Montandon M.-L., Slosman D.O.: Magnetic resonance imaging-guided attenuation and scatter corrections in three-dimensional brain positron emission tomography. Med Phys 2003; 30: pp. 937-948.


- 103\. Zaidi H.: Is MRI-guided attenuation correction a viable option for dual-modality PET/MR imaging?. Radiology 2007; 244: pp. 639-642.


- 104\. Hofmann M., Steinke F., Scheel V., et. al.: MRI-based attenuation correction for PET/MRI: a novel approach combining pattern recognition and Atlas registration. J Nucl Med 2008; 49: pp. 1875-1883.


- 105\. Gaa J., Rummeny E.J., Seemann M.D.: Whole-body imaging with PET/MRI. Eur J Med Res 2004; 30: pp. 309-312.


- 106\. Seemann M.D.: Whole-body PET/MRI: the future in oncological imaging. Technol Cancer Res Treat 2005; 4: pp. 577-582.


- 107\.  Schlemmer HP, Pichler BJ, Krieg R, et al. An integrated MR/PET system: prospective applications. Abdom Imaging. In press.


- 108\. Hicks R.J., Lau E.W.: PET/MRI: a different spin from under the rim. Eur J Nucl Med Mol Imaging 2009; 36: pp. 10-14.


- 109\. Payne G.S., Leach M.O.: Applications of magnetic resonance spectroscopy in radiotherapy treatment planning. Br J Radiol 2006; 79: pp. S16-S26.


- 110\. Torigian D.A., Huang S.S., Houseni M., et. al.: Functional imaging of cancer with emphasis on molecular techniques. CA Cancer J Clin 2007; 57: pp. 206-224.


- 111\. Schoder H., Ong S.C.: Fundamentals of molecular imaging: rationale and applications with relevance for radiation oncology. Semin Nucl Med 2008; 38: pp. 119-128.


- 112\. Kumar R., Dhanpathi H., Basu S., et. al.: Oncologic PET tracers beyond \[(18)F\]FDG and the novel quantitative approaches in PET imaging. Q J Nucl Med Mol Imaging 2008; 52: pp. 50-65.


- 113\. Fowler J.S., Ding Y.S., Volkow N.D.: Radiotracers for positron emission tomography imaging. Semin Nucl Med 2003; 33: pp. 14-27.


- 114\. Weber W.A., Figlin R.: Monitoring cancer treatment with PET/CT: does it make a difference?. J Nucl Med 2007; 48: pp. 36S-44S.


- 115\. Evans S.M., Fraker D., Hahn S.M., et. al.: EF5 binding and clinical outcome in human soft tissue sarcomas. Int J Radiat Oncol Biol Phys 2006; 64: pp. 922-927.


- 116\. Grosu A.L., Souvatzoglou M., Roper B., et. al.: Hypoxia imaging with FAZA-PET and theoretical considerations with regard to dose painting for individualization of radiotherapy in patients with head and neck cancer. Int J Radiat Oncol Biol Phys 2007; 69: pp. 541-551.


- 117\. Wong T.Z., Lacy J.L., Petry N.A., et. al.: PET of hypoxia and perfusion with 62Cu-ATSM and 62Cu-PTSM using a 62Zn/62Cu generator. AJR Am J Roentgenol 2008; 190: pp. 427-432.


- 118\. Nehmeh S.A., Lee N.Y., Schroder H., et. al.: Reproducibility of intratumor distribution of (18)F-fluoromisonidazole in head and neck cancer. Int J Radiat Oncol Biol Phys 2008; 70: pp. 235-242.


- 119\. Rajendran J.G., Hendrickson K.R., Spence A.M., et. al.: Hypoxia imaging-directed radiation treatment planning. Eur J Nucl Med Mol Imaging 2006; 33: pp. 44-53.


- 120\. Mankoff D., Shields A., Krohn K.: PET imaging of cellular proliferation. Radiol Clin North Am 2005; 43: pp. 153-167.


- 121\. Fischman A.: Role of \[18F\]-dopa-PET imaging in assessing movement disorders. Radiol Clin North Am 2005; 43: pp. 93-106.


- 122\. Jager P.L., Chirakal R., Marriott C.J., et. al.: 6-L-18F-Fluorodihydroxyphenylalanine PET in neuroendocrine tumors: Basic aspects and emerging clinical applications. J Nucl Med 2008; 49: pp. 573-586.


- 123\. Nanni C., Fanti S., Rubello D.: 18F-DOPA PET and PET/CT. J Nucl Med 2007; 48: pp. 1577-1579.


- 124\. Belvisi L., Bernardi A., Colombo M., et. al.: Targeting integrins: insights into structure and activity of cyclic RGD pentapeptide mimics containing azabicycloalkane amino acids. Bioorg Med Chem 2006; 14: pp. 169-180.


- 125\. Beer A.J., Grosu A.L., Carlsen J., et. al.: \[18F\]Galacto-RGD positron emission tomography for imaging of {alpha}v{beta}3 expression on the neovasculature in patients with squamous cell carcinoma of the head and neck. Clin Cancer Res 2007; 13: pp. 6610-6616.


- 126\. Couturier O., Luxen A., Chatal J.F., et. al.: Fluorinated tracers for imaging cancer with positron emission tomography. Eur J Nucl Med Mol Imaging 2004; 31: pp. 1182-1206.


- 127\. Blankenberg F., Katsikis P., Tait J., et. al.: In vivo detection and imaging of phosphatidylserine expression during programmed cell death. Proc Natl Acad Sci U S A 1998; 95: pp. 6349-6354.


- 128\. Rahn A.N., Baum R.P., Adamietz I.A., et. al.: (Value of 18F fluorodeoxyglucose positron emission tomography in radiotherapy planning of head-neck tumors). Strahlenther Onkol 1998; 174: pp. 358-364.


- 129\. Gross M.W., Weber W.A., Feldmann H.J., et. al.: The value of F-18-fluorodeoxyglucose PET for the 3-D radiation treatment planning of malignant gliomas. Int J Radiat Oncol Biol Phys 1998; 41: pp. 989-995.


- 130\. Kiffer J.D., Berlangieri S.U., Scott A.M., et. al.: The contribution of 18F-fluoro-2-deoxy-glucose positron emission tomographic imaging to radiotherapy planning in lung cancer. Lung Cancer 1998; 19: pp. 167-177.


- 131\. Scarfone C., Jaszczak R.J., Gilland D.R., et. al.: Quantitative pulmonary single photon emission computed tomography for radiotherapy applications. Med Phys 1999; 26: pp. 1579-1588.


- 132\. Munley M.T., Marks L.B., Scarfone C., et. al.: Multimodality nuclear medicine imaging in three-dimensional radiation treatment planning for lung cancer: challenges and prospects. Lung Cancer 1999; 23: pp. 105-114.


- 133\. Nestle U., Walter K., Schmidt S., et. al.: 18F-deoxyglucose positron emission tomography (FDG-PET) for the planning of radiotherapy in lung cancer: high impact in patients with atelectasis. Int J Radiat Oncol Biol Phys 1999; 44: pp. 593-597.


- 134\. Vanuytsel L.J., Vansteenkiste J.F., Stroobants S.G., et. al.: The impact of 18F-fluoro-2-deoxy–glucose positron emission tomography (FDG-PET) lymph node staging on the radiation treatment volumes in patients with non-small cell lung cancer. Radiother Oncol 2000; 55: pp. 317-324.


- 135\. Levivier M., Wikier D., Goldman S., et. al.: Integration of the metabolic data of positron emission tomography in the dosimetry planning of radiosurgery with the gamma knife: early experience with brain tumors. Technical note. J Neurosurg 2000; 93: pp. 233-238.


- 136\. Ling C., Humm J., Larson S., et. al.: Towards multidimensional radiotherapy (MD-CRT): biological imaging and biological conformality. Int J Radiat Oncol Biol Phys 2000; 47: pp. 551-560.


- 137\. Scarfone C., Lavely W.C., Cmelak A.J., et. al.: Prospective feasibility trial of radiotherapy target definition for head and neck cancer using 3-dimensional PET and CT imaging. J Nucl Med 2004; 45: pp. 543-552.


- 138\. Paulino A.C., Thorstad W.L., Fox T.: Role of fusion in radiotherapy treatment planning. Semin Nucl Med 2003; 33: pp. 238-243.


- 139\. Yap J.T., Carney J.P., Hall N.C., Townsend D.W.: Image-guided cancer therapy using PET/CT. Cancer J 2004; 10: pp. 221-233.


- 140\. Brunetti J., Caggiano A., Rosenbluth B., et. al.: Technical aspects of positron emission tomography/computed tomography fusion planning. Sem Nucl Med 2008; 38: pp. 129-136.


- 141\. Greco C., Rosenzweig K., Cascini G.L., et. al.: Current status of PET/CT for tumour volume definition in radiotherapy treatment planning for non-small cell lung cancer (NSCLC). Lung Cancer 2007; 57: pp. 125-134.


- 142\. Stroom J., Blaauwgeers H., van Baardwijk A., et. al.: Feasibility of pathology-correlated lung imaging for accurate target definition of lung tumors. Int J Radiat Oncol Biol Phys 2007; 69: pp. 267-275.


- 143\. Mah K., Caldwell C.B., Ung Y.C., et. al.: The impact of (18)FDG-PET on target and critical organs in CT-based treatment planning of patients with poorly defined non-small-cell lung carcinoma: a prospective study. Int J Radiat Oncol Biol Phys 2002; 52: pp. 339-350.


- 144\. Caldwell C.B., Mah K., Skinner M., et. al.: Can PET provide the 3D extent of tumor motion for individualized internal target volumes? A phantom study of the limitations of CT and the promise of PET. Int J Radiat Oncol Biol Phys 2003; 55: pp. 1381-1393.


- 145\. Bradley J., Thorstad W.L., Mutic S., et. al.: Impact of FDG-PET on radiation therapy volume delineation in non-small-cell lung cancer. Int J Radiat Oncol Biol Phys 2004; 59: pp. 78-86.


- 146\. Nestle U., Kremp S., Grosu A.L.: Practical integration of \[18F\]-FDG-PET and PET-CT in the planning of radiotherapy for non-small cell lung cancer (NSCLC): the technical basis, ICRU-target volumes, problems, perspectives. Radiother Oncol 2006; 81: pp. 209-225.


- 147\. Levy R.P.: PET-CT: evolving role in 3-D radiation therapy. Technol Cancer Res Treat 2006; 5: pp. 101-107.


- 148\. Grosu A.L., Weber W.A., Astner S.T., et. al.: 11C-methionine PET improves the target volume delineation of meningiomas treated with stereotactic fractionated radiotherapy. Int J Radiat Oncol Biol Phys 2006; 66: pp. 339-344.


- 149\. Macapinlac H.A.: Clinical applications of positron emission tomography/computed tomography treatment planning. Semin Nucl Med 2008; 38: pp. 137-140.


- 150\. Dizendorf E.V., Baumert B.G., von Schulthess G.K., et. al.: Impact of whole-body 18F-FDG PET on staging and managing patients for radiation therapy. J Nucl Med 2003; 44: pp. 24-29.


- 151\. Czernin J., Phelps M.E.: Positron emission tomography scanning: current and future applications. Annu Rev Med 2002; 53: pp. 89-112.


- 152\.  Lammering G, De Haas D, De Ruysscher D, et al. First report on the use of a dedicated combined CT-PET simulator in rectal cancer patients \[abstract\]. Radiother Oncol 2004; ESTRO 23:S441.


- 153\. Weder W., Schmid R.A., Bruchhaus H., et. al.: C. Detection of extrathoracic metastases by positron emission tomography in lung cancer. Ann Thorac Surg 1998; 66: pp. 886-892. discussion 892–893


- 154\. Kalff V., Hicks R.J., MacManus M.P., et. al.: Clinical impact of (18)F fluorodeoxyglucose positron emission tomography in patients with non-small-cell lung cancer: a prospective study. J Clin Oncol 2001; 19: pp. 111-118.


- 155\. van Baardwijk A., Bosmans G., Boersma L., et. al.: PET-CT-based auto-contouring in non-small-cell lung cancer correlates with pathology and reduces interobserver variability in the delineation of the primary tumor and involved nodal volumes. Int J Radiat Oncol Biol Phys 2007; 68: pp. 771-778.


- 156\. Caldwell C.B., Mah K., Ung Y.C., et. al.: Observer variation in contouring gross tumor volume in patients with poorly defined non-small-cell lung tumors on CT: the impact of 18FDG-hybrid PET fusion. Int J Radiat Oncol Biol Phys 2001; 51: pp. 923-931.


- 157\. Fox J.L., Rengan R., O'Meara W., et. al.: Does registration of PET and planning CT images decrease interobserver and intraobserver variation in delineating tumor volumes for non-small-cell lung cancer?. Int J Radiat Oncol Biol Phys 2005; 62: pp. 70-75.


- 158\. Ciernik I.F., Dizendorf E., Baumert B.G., et. al.: Radiation treatment planning with an integrated positron emission and computer tomography (PET/CT): a feasibility study. Int J Radiat Oncol Biol Phys 2003; 57: pp. 853-863.


- 159\. Deniaud-Alexandre E., Touboul E., Lerouge D., et. al.: Impact of computed tomography and 18F-deoxyglucose coincidence detection emission tomography image fusion for optimization of conformal radiotherapy in non-small-cell lung cancer. Int J Radiat Oncol Biol Phys 2005; 63: pp. 1432-1441.


- 160\. Ashamalla H., Rafla S., Parikh K., et. al.: The contribution of integrated PET/CT to the evolving definition of treatment volumes in radiation treatment planning in lung cancer. Int J Radiat Oncol Biol Phys 2005; 63: pp. 1016-1023.


- 161\. Hong R., Halama J., Bova D., et. al.: Correlation of PET standard uptake value and CT window-level thresholds for target delineation in CT-based radiation treatment planning. Int J Radiat Oncol Biol Phys 2007; 67: pp. 720-726.


- 162\. Paulino A.C., Koshy M., Howell R., et. al.: Comparison of CT- and FDG-PET-defined gross tumor volume in intensity-modulated radiotherapy for head-and-neck cancer. Int J Radiat Oncol Biol Phys 2005; 61: pp. 1385-1392.


- 163\. Schwartz D.L., Ford E.C., Rajendran J., et. al.: FDG-PET/CT-guided intensity modulated head and neck radiotherapy: a pilot investigation. Head Neck 2005; 27: pp. 478-487.


- 164\. Geets X., Daisne J.F., Tomsej M., et. al.: Impact of the type of imaging modality on target volumes delineation and dose distribution in pharyngo-laryngeal squamous cell carcinoma: comparison between pre- and per-treatment studies. Radiother Oncol 2006; 78: pp. 291-297.


- 165\. Daisne J.F., Duprez T., Weynand B., et. al.: Tumor volume in pharyngolaryngeal squamous cell carcinoma: comparison at CT, MR imaging, and FDG PET and validation with surgical specimen. Radiology 2004; 233: pp. 93-100.


- 166\. Burri R.J., Rangaswamy B., Kostakoglu L., et. al.: Correlation of positron emission tomography standard uptake value and pathologic specimen size in cancer of the head and neck. Int J Radiat Oncol Biol Phys 2008; 71: 682–628


- 167\. van Baardwijk A., Baumert B.G., Bosmans G., et. al.: The current status of FDG-PET in tumour volume definition in radiotherapy treatment planning. Cancer Treat Rev 2006; 32: pp. 245-260.


- 168\. Vernon M.R., Maheshwari M., Schultz C.J., et. al.: Clinical outcomes of patients receiving integrated PET/CT-guided radiotherapy for head and neck carcinoma. Int J Radiat Oncol Biol Phys 2008; 70: pp. 678-684.


- 169\. Weng E., Tran L., Rege S., et. al.: Accuracy and clinical impact of mediastinal lymph node staging with FDG-PET imaging in potentially resectable lung cancer. Am J Clin Oncol 2000; 23: pp. 47-52.


- 170\. De Ruysscher D., Wanders S., Minken A., et. al.: Effects of radiotherapy planning with a dedicated combined PET-CT-simulator of patients with non-small cell lung cancer on dose limiting normal tissues and radiation dose-escalation: a planning study. Radiother Oncol 2005; 77: pp. 5-10.


- 171\. Messa C., Ceresoli G.L., Rizzo G., et. al.: Feasibility of \[18F\]FDG-PET and coregistered CT on clinical target volume definition of advanced non-small cell lung cancer. Q J Nucl Med Mol Imaging 2005; 49: pp. 259-266.


- 172\. Luketich J.D., Friedman D.M., Meltzer C.C., et. al.: The role of positron emission tomography in evaluating mediastinal lymph node metastases in non-small-cell lung cancer. Clin Lung Cancer 2001; 2: pp. 229-233.


- 173\. Everitt S., Schneider-Kolsky M., Yuen K., et. al.: Dose escalation of radical radiation therapy in non-small-cell lung cancer using positron emission tomography/computed tomography-defined target volumes: are class solutions obsolete?. J Med Imaging Radiat Oncol 2008; 52: pp. 168-177.


- 174\. Klopp A.H., Chang J.Y., Tucker S.L., et. al.: Intrathoracic patterns of failure for non-small-cell lung cancer with positron-emission tomography/computed tomography-defined target delineation. Int J Radiat Oncol Biol Phys 2007; 69: pp. 1409-1416.


- 175\. De Ruysscher D., Wanders S., van Haren E., et. al.: Selective mediastinal node irradiation based on FDG-PET scan data in patients with non-small-cell lung cancer: a prospective clinical study. Int J Radiat Oncol Biol Phys 2005; 62: pp. 988-994.


- 176\. Neicu T., Berbeco R., Wolfgang J., et. al.: Synchronized moving aperture radiation therapy (SMART): improvement of breathing pattern reproducibility using respiratory coaching. Phys Med Biol 2006; 51: pp. 617-636.


- 177\. Yaremko B., Riauka T., Robinson D., et. al.: Thresholding in PET images of static and moving targets. Phys Med Biol 2005; 50: pp. 5969-5982.


- 178\. Nestle U., Kremp S., Schaefer-Schuler A., et. al.: Comparison of different methods for delineation of 18F-FDG PET-positive tissue for target volume definition in radiotherapy of patients with non-Small cell lung cancer. J Nucl Med 2005; 6: pp. 1342-1348.


- 179\. Belhassen S., Llina Fuentes C.S., Dekker A., et. al.: Comparative methods for 18F-FDG PET-based delineation of target volumes in non-small-cell lung cancer \[abstract\]. J Nucl Med 2009; 50: In press


- 180\. van Westreenen H.L., Westerterp M., Bossuyt P.M.M., et. al.: Systematic review of the staging performance of 18F-Fluorodeoxyglucose positron emission tomography in esophageal cancer. J Clin Oncol 2004; 22: pp. 3805-3812.


- 181\. Vrieze O., Haustermans K., De Wever W., et. al.: Is there a role for FGD-PET in radiotherapy planning in esophageal carcinoma?. Radiother Oncol 2004; 73: pp. 269-275.


- 182\. Vinjamuri S., Ray S.: Added value of PET and PET-CT in oesophageal cancer: a review of current practice. Nucl Med Commun 2008; 29: pp. 4-10.


- 183\. van Vliet E.P., Heijenbrok-Kal M.H., Hunink M.G., et. al.: Staging investigations for oesophageal cancer: a meta-analysis. Br J Cancer 2008; 98: pp. 547-557.


- 184\. Bruzzi J.F., Munden R.F., Truong M.T., Marom E.M., Sabloff B.S., Gladish G.W., et. al.: PET/CT of esophageal cancer: its role in clinical management. Radiographics 2007; 27: pp. 1635-1652.


- 185\. Narayan K., Hicks R.J., Jobling T., et. al.: A comparison of MRI and PET scanning in surgically staged loco-regionally advanced cervical cancer: potential impact on treatment. Int J Gynecol Cancer 2001; 11: pp. 263-271.


- 186\. Khan N., Oriuchi N., Yoshizaki A., et. al.: Diagnostic accuracy of FDG PET imaging for the detection of recurrent or metastatic gynecologic cancer. Ann Nucl Med 2005; 19: pp. 137-145.


- 187\. Grisaru D., Almog B., Levine C., et. al.: The diagnostic accuracy of 18F-fluorodeoxyglucose PET/CT in patients with gynecological malignancies. Gynecol Oncol 2004; 94: pp. 680-684.


- 188\. Nakamoto Y., Saga T., Fujii S.: Positron emission tomography application for gynecologic tumors. Int J Gynecol Cancer 2005; 15: pp. 701-709.


- 189\. Esthappan J., Mutic S., Malyapa R.S., et. al.: Treatment planning guidelines regarding the use of CT/PET-guided IMRT for cervical carcinoma with positive paraaortic lymph nodes. Int J Radiat Oncol Biol Phys 2004; 58: pp. 1289-1297.


- 190\. Mutic S., Grigsby P.W., Low D.A., et. al.: PET-guided three-dimensional treatment planning of intracavitary gynecologic implants. Int J Radiat Oncol Biol Phys 2002; 52: pp. 1104-1110.


- 191\. Mutic S., Malyapa R.S., Grigsby P.W., et. al.: PET-guided IMRT for cervical carcinoma with positive para-aortic lymph nodes—a dose-escalation treatment planning study. Int J Radiat Oncol Biol Phys 2003; 55: pp. 28-35.


- 192\. Kantorova I., Lipska L., Belohlavek O., et. al.: Routine (18)F-FDG PET preoperative staging of colorectal cancer: comparison with conventional staging and its impact on treatment decision making. J Nucl Med 2003; 44: pp. 1784-1788.


- 193\. Anderson C., Koshy M., Staley C., et. al.: PET-CT fusion in radiation management of patients with anorectal tumors. Int J Radiat Oncol Biol Phys 2007; 69: pp. 155-162.


- 194\. Podoloff D.A., Macapinlac H.A.: PET and PET/CT in management of the lymphomas. Radiol Clin North Am 2007; 45: pp. 689-696.


- 195\. Juweid M.E., Stroobants S., Hoekstra O.S., et. al.: Use of positron emission tomography for response assessment of lymphoma: consensus of the imaging subcommittee of International harmonization project in lymphoma. J Clin Oncol 2007; 25: pp. 571-578.


- 196\. Lee Y.K., Cook G., Flower M.A., et. al.: Addition of 18F-FDG-PET scans to radiotherapy planning of thoracic lymphoma. Radiother Oncol 2004; 73: pp. 277-283.


- 197\. Girinsky T., Ghalibafian M., Bonniaud G., et. al.: Is FDG-PET scan in patients with early stage Hodgkin lymphoma of any value in the implementation of the involved-node radiotherapy concept and dose painting?. Radiother Oncol 2007; 85: pp. 178-186.


- 198\. Hutchings M., Loft A., Hansen M., et. al.: Clinical impact of FDG-PET/CT in the planning of radiotherapy for early-stage Hodgkin lymphoma. Eur J Haematol 2007; 78: pp. 206-212.


- 199\. Veronesi U., De Cicco C., Galimberti V., et. al.: A comparative study on the value of FDG-PET and sentinel node biopsy to identify occult axillary metastases. Ann Oncol 2007; 18: pp. 473-478.


- 200\. Barranger E., Grahek D., Antoine M., et. al.: Evaluation of fluorodeoxyglucose positron emission tomography in the detection of axillary lymph node metastases in patients with early-stage breast cancer. Ann Surg Oncol 2003; 10: pp. 622-627.


- 201\. Zornoza G., Garcia-Velloso M.J., Sola J., et. al.: 18F-FDG PET complemented with sentinel lymph node biopsy in the detection of axillary involvement in breast cancer. Eur J Surg Oncol 2004; 30: pp. 15-19.


- 202\. Lovrics P.J., Chen V., Coates G., et. al.: A prospective evaluation of positron emission tomography scanning, sentinel lymph node biopsy, and standard axillary dissection for axillary staging in patients with early stage breast cancer. Ann Surg Oncol 2004; 11: pp. 846-853.


- 203\. Cardillo A., De Cicco C., Paganelli G., et. al.: Role of fluorodeoxyglucose positron emission tomography in the staging of patients with breast cancer candidated to surgery. Ann Oncol 2007; 18: pp. 394-395.


- 204\. Gil-Rendo A., Zornoza G., Garcia-Velloso M.J., et. al.: Fluorodeoxyglucose positron emission tomography with sentinel lymph node biopsy for evaluation of axillary involvement in breast cancer. Br J Surg 2006; 93: pp. 707-712.


- 205\. Mavi A., Urhan M., Yu J.Q., et. al.: Dual time point 18F-FDG PET imaging detects breast cancer with high sensitivity and correlates well with histologic subtypes. J Nucl Med 2006; 47: pp. 1440-1446.


- 206\. Heusner T.A., Freudenberg L.S., Kuehl H., et. al.: Whole-body PET/CT-mammography for staging breast cancer: initial results. Br J Radiol 2008; 81: pp. 743-748.


- 207\. Heusner T.A., Kuemmel S., Umutlu L., et. al.: Breast cancer staging in a single session: whole-body PET/CT mammography. J Nucl Med 2008; 49: pp. 1215-1222.


- 208\. Bral S., Vinh-Hung V., Everaert H., et. al.: The use of molecular imaging to evaluate radiation fields in the adjuvant setting of breast cancer: a feasibility study. Strahlenther Onkol 2008; 184: pp. 100-104.


- 209\. Doshi N.K., Silverman R.W., Shao Y., et. al.: maxPET, a dedicated mammary and axillary region PET imaging system for breast cancer. IEEE Trans Nucl Sci 2001; 48: pp. 811-815.


- 210\. Levin C.S., Foudray A.M., Habte F.: Impact of high energy resolution detectors on the performance of a PET system dedicated to breast cancer imaging. Phys Med 2006; 21(Suppl 1): pp. 28-34.


- 211\. Abreu M.C., et. al.: Clear-PEM: a PET imaging system dedicated to breast cancer diagnostics. Nucl Instr Meth A 2007; 571: pp. 81-84.


- 212\. Surti S., Karp J.S.: Design considerations for a limited angle, dedicated breast, TOF PET scanner. Phys Med Biol 2008; 53: pp. 2911-2921.


- 213\. Murthy K., Aznar M., Thompson C.J., et. al.: Results of preliminary clinical trials of the positron emission mammography system PEM-I: a dedicated breast imaging system producing glucose metabolic images using FDG. J Nucl Med 2000; 41: pp. 1851-1858.


- 214\. Rosen E.L., Turkington T.G., Soo M.S., et. al.: Detection of primary breast carcinoma with a dedicated, large-field-of-view FDG PET mammography device: initial experience. Radiology 2005; 234: pp. 527-534.


- 215\. Raylman R.R., Majewski S., Smith M.F., et. al.: The positron emission mammography/tomography breast imaging and biopsy system (PEM/PET): design, construction and phantom-based measurements. Phys Med Biol 2008; 53: pp. 637-653.


- 216\. Zangheri B., Messa C., Picchio M., et. al.: PET/CT and breast cancer. Eur J Nuc Med Mol Imaging 2004; 31: pp. S135-S142.


- 217\. Lindfors K.K., Boone J.M., Nelson T.R., et. al.: Dedicated breast CT: initial clinical experience. Radiology 2008; 246: pp. 725-733.


- 218\. Liang H., Yang Y., Yang K., et. al.: A microPET/CT system for in vivo small animal imaging. Phys Med Biol 2007; 52: pp. 3881-3894.


- 219\. Grosu A.L., Piert M., Weber W.A., et. al.: Positron emission tomography for radiation treatment planning. Strahlenther Onkol 2005; 181: pp. 483-499.


- 220\. Koch C.J., Evans S.M.: Non-invasive PET and SPECT imaging of tissue hypoxia using isotopically labeled 2-nitroimidazoles. Adv Exp Med Biol 2003; 510: pp. 285-292.


- 221\. Beck R., Roper B., Carlsen J.M., et. al.: Pretreatment 18F-FAZA PET predicts success of hypoxia-directed radiochemotherapy using tirapazamine. J Nucl Med 2007; 48: pp. 973-980.


- 222\. Sorger D., Patt M., Kumar P., et. al.: \[18F\]Fluoroazomycinarabinofuranoside (18FAZA) and \[18F\]Fluoromisonidazole (18FMISO): a comparative study of their selective uptake in hypoxic cells and PET imaging in experimental rat tumors. Nucl Med Biol 2003; 30: pp. 317-326.


- 223\. Tanaka T., Furukawa T., Fujieda S., et. al.: Double-tracer autoradiography with Cu-ATSM/FDG and immunohistochemical interpretation in four different mouse implanted tumor models. Nucl Med Biol 2006; 33: pp. 743-750.


- 224\. Rischin D., Hicks R.J., Fisher R., et. al.: Prognostic significance of \[18F\]-misonidazole positron emission tomography-detected tumor hypoxia in patients with advanced head and neck cancer randomly assigned to chemoradiation with or without tirapazamine: a substudy of Trans-Tasman Radiation Oncology Group Study 98.02. J Clin Oncol 2006; 24: pp. 2098-2104.


- 225\. Thorwarth D., Eschmann S.M., Scheiderbauer J., et. al.: Kinetic analysis of dynamic 18F-fluoromisonidazole PET correlates with radiation treatment outcome in head-and-neck cancer. BMC Cancer 2005; 5: pp. 152.


- 226\. Lee N.Y., Mechalakos J.G., Nehmeh S., et. al.: Fluorine-18-labeled fluoromisonidazole positron emission and computed tomography-guided intensity-modulated radiotherapy for head and neck cancer: a feasibility study. Int J Radiat Oncol Biol Phys 2008; 70: pp. 2-13.


- 227\. Lin Z., Mechalakos J., Nehmeh S., et. al.: The influence of changes in tumor hypoxia on dose-painting treatment plans based on (18)F-FMISO positron emission tomography. Int J Radiat Oncol Biol Phys 2008; 70: pp. 1219-1228.


- 228\. Eschmann S.M., Paulsen F., Reimold M., et. al.: Prognostic impact of hypoxia imaging with 18F-misonidazole PET in non-small cell lung cancer and head and neck cancer before radiotherapy. J Nucl Med 2005; 46: pp. 253-260.


- 229\. Lawrentschuk N., Poon A.M., Foo S.S., et. al.: Assessing regional hypoxia in human renal tumours using 18F-fluoromisonidazole positron emission tomography. BJU Int 2005; 96: pp. 540-546.


- 230\. Rajendran J.G., Wilson D.C., Conrad E.U., et. al.: \[(18)F\]FMISO and \[(18)F\]FDG PET imaging in soft tissue sarcomas: correlation of hypoxia, metabolism and VEGF expression. Eur J Nucl Med Mol Imaging 2003; 30: pp. 695-704.


- 231\. Eschmann S.M., Paulsen F., Bedeshem C., et. al.: Hypoxia-imaging with (18)F-Misonidazole and PET: changes of kinetics during radiotherapy of head-and-neck cancer. Radiother Oncol 2007; 83: pp. 406-410.


- 232\. Dolbier W.R., Li A.R., Koch C.J., et. al.: \[18F\]-EF5, a marker for PET detection of hypoxia: synthesis of precursor and a new fluorination procedure. Appl Radiat Isot 2001; 54: pp. 73-80.


- 233\. Komar G., Seppanen M., Eskola O., et. al.: 18F-EF5: a new PET tracer for imaging hypoxia in head and neck cancer. J Nucl Med 2008; 49: pp. 1944-1951.


- 234\. Evans S., Hahn S., Judy K., et. al.: 18F EF5 PET imaging with imunohistochemical validation in patients with brain lesions \[abstract\]. Int J Rad Oncol Biol Phys 2006; 66: pp. S248.


- 235\. Reinhardt M.J., Kubota K., Yamada S., et. al.: Assessment of cancer recurrence in residual tumors after fractionated radiotherapy: a comparison of fluorodeoxyglucose. L-methionine and thymidine. J Nucl Med 1997; 38: pp. 280-287.


- 236\. Grosu A.L., Weber W.A., Riedel E., et. al.: L-(methyl-11C) methionine positron emission tomography for target delineation in resected high-grade gliomas before radiotherapy. Int J Radiat Oncol Biol Phys 2005; 63: pp. 64-74.


- 237\. Terakawa Y., Tsuyuguchi N., Iwai Y., et. al.: Diagnostic accuracy of 11C-methionine PET for differentiation of recurrent brain tumors from radiation necrosis after radiotherapy. J Nucl Med 2008; 49: pp. 694-699.


- 238\. Singhal T., Narayanan T.K., Jain V., et. al.: 11C-L-methionine positron emission tomography in the clinical management of cerebral gliomas. Mol Imaging Biol 2008; 10: pp. 1-18.


- 239\. Nariai T., Tanaka Y., Wakimoto H., et. al.: Usefulness of L-\[methyl-11C\] methionine-positron emission tomography as a biological monitoring tool in the treatment of glioma. J Neurosurg 2005; 103: pp. 498-507.


- 240\. Rachinger W., Goetz C., Popperl G., et. al.: Positron emission tomography with O-(2-\[18F\]fluoroethyl)-l-tyrosine versus magnetic resonance imaging in the diagnosis of recurrent gliomas. Neurosurgery 2005; 57: pp. 505-511.


- 241\. Astner S.T., Dobrei-Ciuchendea M., Essler M., et. al.: Effect of (11)C-methionine-positron emission tomography on gross tumor volume delineation in stereotactic radiotherapy of skull base meningiomas. Int J Radiat Oncol Biol Phys 2008; 72: pp. 1161-1167.


- 242\. Grosu A.L., Lachner R., Wiedenmann N., et. al.: Validation of a method for automatic image fusion (BrainLAB System) of CT data and 11C-methionine-PET data for stereotactic radiotherapy using a LINAC: first clinical experience. Int J Radiat Oncol Biol Phys 2003; 56: pp. 1450-1463.


- 243\. Grosu A.L., Weber W.A., Franz M., et. al.: Reirradiation of recurrent high-grade gliomas using amino acid PET (SPECT)/CT/MRI image fusion to determine gross tumor volume for stereotactic fractionated radiotherapy. Int J Radiat Oncol Biol Phys 2005; 63: pp. 511-519.


- 244\. Plotkin M., Gneveckow U., Meier-Hauff K., et. al.: 18F-FET PET for planning of thermotherapy using magnetic nanoparticles in recurrent glioblastoma. Int J Hyperthermia 2006; 22: pp. 319-325.


- 245\. Levivier M., Massager N., Wikler D., et. al.: Integration of functional imaging in radiosurgery: the example of PET scan. Prog Neurol Surg 2007; 20: pp. 68-81.


- 246\. Mahasittiwat P., Mizoe J.E., Hasegawa A., et. al.: l-\[METHYL-(11)C\] methionine positron emission tomography for target delineation in malignant gliomas: impact on results of carbon ion radiotherapy. Int J Radiat Oncol Biol Phys 2008; 70: pp. 515-522.


- 247\. Miwa K., Matsuo M., Shinoda J., et. al.: Simultaneous integrated boost technique by helical tomotherapy for the treatment of glioblastoma multiforme with (11)C-methionine PET: report of three cases. J Neurooncol 2008; 87: pp. 333-339.


- 248\. Tang B.N., Levivier M., Heureux M., et. al.: 11C-methionine PET for the diagnosis and management of recurrent pituitary adenomas. Eur J Nucl Med Mol Imaging 2006; 33: pp. 169-178.


- 249\. Vees H., Senthamizhchelvan S., Miralbell R., et. al.: Assessment of various strategies for 18F-FET PET-guided delineation of target volumes in high-grade glioma patients. Eur J Nucl Med Mol Imaging 2009; 36: pp. 182-193.


- 250\. Weber D.C., Zilli T., Buchegger F., et. al.: \[(18)F\]Fluoroethyltyrosine- positron emission tomography-guided radiotherapy for high-grade glioma. Radiat Oncol 2008; 3: pp. 44.


- 251\. de Jong I.J., Pruim J., Elsinga P.H., et. al.: 11C-choline positron emission tomography for the evaluation after treatment of localized prostate cancer. Eur Urol 2003; 44: pp. 32-38. discussion 38–39


- 252\. Heinisch M., Dirisamer A., Loidl W., et. al.: Positron emission tomography/computed tomography with F-18-fluorocholine for restaging of prostate cancer patients: meaningful at PSA < 5 ng/ml?. Mol Imaging Biol 2006; 8: pp. 43-48.


- 253\. Picchio M., Messa C., Landoni C., et. al.: Value of \[11C\]choline-positron emission tomography for re-staging prostate cancer: a comparison with \[18F\]fluorodeoxyglucose-positron emission tomography. J Urol 2003; 169: pp. 1337-1340.


- 254\. Reske S.N., Blumstein N.M., Glatting G.: \[(11)C\]choline PET/CT imaging in occult local relapse of prostate cancer after radical prostatectomy. Eur J Nucl Med Mol Imaging 2008; 35: pp. 9-17.


- 255\. Vees H., Buchegger F., Albrecht S., et. al.: 18F-choline and/or 11C-acetate positron emission tomography: detection of residual or progressive subclinical disease at very low prostate-specific antigen values (<1 ng/mL) after radical prostatectomy. BJU Int 2007; 99: pp. 1415-1420.


- 256\. Steiner C., Vees H., Zaidi H., et. al.: Three-phase 18F-fluorocholine PET/CT in the evaluation of prostate cancer recurrence. Nuklearmedizin 2009; 48: pp. 1-9.


- 257\. Ciernik I.F., Brown D.W., Schmid D., et. al.: 3D-segmentation of the 18F-choline PET signal for target volume definition in radiation therapy of the prostate. Technol Cancer Res Treat 2007; 6: pp. 23-30.


- 258\. Picozzi P., Rizzo G., Landoni C., et. al.: A simplified method to integrate metabolic images in stereotactic procedures using a PET/CT scanner. Stereotact Funct Neurosurg 2005; 83: pp. 208-212.


- 259\. Rickhey M., Bogner L.: Application of the inverse Monte Carlo treatment planning system IKO for an inhomogeneous dose prescription in the sense of dose painting. Z Med Phys 2006; 16: pp. 307-312.


- 260\. Sugiyama M., Sakahara H., Sato K., et. al.: Evaluation of 3'-deoxy-3'-18F-fluorothymidine for monitoring tumor response to radiotherapy and photodynamic therapy in mice. J Nucl Med 2004; 45: pp. 1754-1758.


- 261\. Gabriel M., Decristoforo C., Kendler D., et. al.: 68Ga-DOTA-Tyr3-octreotide PET in neuroendocrine tumors: comparison with somatostatin receptor scintigraphy and CT. J Nucl Med 2007; 48: pp. 508-518.


- 262\. Milker-Zabel S., Zabel-du Bois A., Henze M., et. al.: Improved target volume definition for fractionated stereotactic radiotherapy in patients with intracranial meningiomas by correlation of CT, MRI, and \[68Ga\]-DOTATOC-PET. Int J Radiat Oncol Biol Phys 2006; 65: pp. 222-227.


- 263\. Austin-Seymour M., Chen G.T., Rosenman J., et. al.: Tumor and target delineation: current research and future challenges. Int J Radiat Oncol Biol Phys 1995; 33: pp. 1041-1052.


- 264\. Van Hoe L., Haven F., Bellon E., et. al.: Factors influencing the accuracy of volume measurements in spiral CT: a phantom study. J Comput Assist Tomogr 1997; 21: pp. 332-338.


- 265\. Bowden P., Fisher R., Mac Manus M., et. al.: Measurement of lung tumor volumes using three-dimensional computer planning software. Int J Radiat Oncol Biol Phys 2002; 53: pp. 566-573.


- 266\. Senan S., Chapet O., Lagerwaard F.J., et. al.: Defining target volumes for non-small cell lung carcinoma. Semin Radiat Oncol 2004; 14: pp. 308-314.


- 267\. Chaney E., Ibbott G., Hendee W.R.: Methods for image segmentation should be standardized and calibrated. Med Phys 2005; 32: pp. 3507-3510.


- 268\. Evans P.M.: Anatomical imaging for radiotherapy. Phys Med Biol 2008; 53: pp. R151-R191.


- 269\. Rasch C., Barillot I., Remeijer P., et. al.: Definition of the prostate in CT and MRI: a multi-observer study. Int J Rad Oncol Biol Phys 1999; 43: pp. 57-66.


- 270\. Khoo V.S., Adams E.J., Saran F., et. al.: A comparison of clinical target volumes determined by CT and MRI for the radiotherapy planning of base of skull meningiomas. Int J Rad Oncol Biol Phys 2000; 46: pp. 1309-1317.


- 271\. Lee Y.K., Bollet M., Charles-Edwards G., et. al.: Radiotherapy treatment planning of prostate cancer using magnetic resonance imaging alone. Radiother Oncol 2003; 66: pp. 203-216.


- 272\. Chen L., Price J., Robert A., et. al.: MRI-based treatment planning for radiotherapy: Dosimetric verification for prostate IMRT. Int J Rad Oncol Biol Phys 2004; 60: pp. 636-647.


- 273\. Schinagl D.A., Kaanders J.H., Oyen W.J.: From anatomical to biological target volumes: the role of PET in radiation treatment planning. Cancer Imaging 2006; 6: pp. S107-S116.


- 274\. Ashamalla H., Guirgius A., Bieniek E., et. al.: The impact of positron emission tomography/computed tomography in edge delineation of gross tumor volume for head and neck cancers. Int J Radiat Oncol Biol Phys 2007; 68: pp. 388-395.


- 275\. Newbold K., Partridge M., Cook G., et. al.: Advanced imaging applied to radiotherapy planning in head and neck cancer: a clinical review. Br J Radiol 2006; 79: pp. 554-561.


- 276\. Lavrenkov K., Partridge M., Cook G., et. al.: Positron emission tomography for target volume definition in the treatment of non-small cell lung cancer. Radiother Oncol 2005; 77: pp. 1-4.


- 277\. Ford E.C., Kinahan P.E., Hanlon L., et. al.: Tumor delineation using PET in head and neck cancers: Threshold contouring and lesion volumes. Med Phys 2006; 33: pp. 4280-4288.


- 278\. Ahn P.H., Garg M.K.: Positron emission tomography/computed tomography for target delineation in head and neck cancers. Sem Nucl Med 2008; 38: pp. 141-148.


- 279\. Zaidi H.: Medical image segmentation: Quo Vadis. Comput Meth Prog Biomed 2006; 84: pp. 63-67.


- 280\. Boudraa A., Zaidi H.: Image segmentation techniques in nuclear medicine imaging.Zaidi H.Quantitative analysis of nuclear medicine images.2006.SpringerNew York:pp. 308-357.


- 281\. Erdi Y., Mawlawi O., Larson S., et. al.: Segmentation of lung lesion volume by adaptive positron emission tomography image thresholding. Radioimmunodetection and radioimmunotherapy of cancer.1997.American Cancer SocietyPrinceton, NJ 2505–2509


- 282\. Daisne J.F., Sibomana M., Bol A., et. al.: Tri-dimensional automatic segmentation of PET volumes based on measured source-to-background ratios: influence of reconstruction algorithms. Radiother Oncol 2003; 69: pp. 247-250.


- 283\. Drever L., Roa W., McEwan A., et. al.: Iterative threshold segmentation for PET target volume delineation. Med Phys 2007; 34: pp. 1253-1265.


- 284\. Schinagl D.A., Vogel W.V., Hoffmann A.L., et. al.: Comparison of five segmentation tools for 18F-fluoro-deoxy-glucose-positron emission tomography-based target volume definition in head and neck cancer. Int J Radiat Oncol Biol Phys 2007; 69: pp. 1282-1289.


- 285\. Hatt M., Lamare F., Boussion N., et. al.: Fuzzy hidden Markov chains segmentation for volume determination and quantitation in PET. Phys Med Biol 2007; 52: pp. 3467-3491.


- 286\. Montgomery D., Amira A., Zaidi H.: Fully automated segmentation of oncological PET volumes using a combined multiscale and statistical model. Med Phys 2007; 34: pp. 722-736.


- 287\. Drever L., Robinson D.M., McEwan A., et. al.: A local contrast based approach to threshold segmentation for PET target volume delineation. Med Phys 2006; 33: pp. 1583-1594.


- 288\. Biehl K.J., Kong F.M., Dehdashti F., et. al.: 18F-FDG PET definition of gross tumor volume for radiotherapy of non-small cell lung cancer: is a single standardized uptake value threshold approach appropriate?. J Nucl Med 2006; 47: pp. 1808-1812.


- 289\. Jentzen W., Freudenberg L., Eising E.G., et. al.: Segmentation of PET volumes by iterative image thresholding. J Nucl Med 2007; 48: pp. 108-114.


- 290\. Ciernik I.F., Huser M., Burger C., et. al.: Automated functional image-guided radiation treatment planning for rectal cancer. Int J Radiat Oncol Biol Phys 2005; 62: pp. 893-900.


- 291\. Davis J.B., Reiner B., Huser M., et. al.: Assessment of (18)F PET signals for automatic target volume definition in radiotherapy treatment planning. Radiother Oncol 2006; 80: pp. 43-50.


- 292\. Wong C.Y., Mahajan P., Yan D.: Dynamic threshold for radiation target volume by PET/CT. J Nucl Med 2007; 48: pp. 849. author reply 847


- 293\. van Dalen J.A., Hoffmann A.L., Dicken V., et. al.: A novel iterative method for lesion delineation and volumetric quantification with FDG PET. Nucl Med Commun 2007; 28: pp. 485-493.


- 294\. Aristophanous M., Penney B.C., Martel M.K., et. al.: A Gaussian mixture model for definition of lung tumor volumes in positron emission tomography. Med Phys 2007; 34: pp. 4223-4235.


- 295\. Schaefer A., Kremp S., Hellwig D., et. al.: A contrast-oriented algorithm for FDG-PET-based delineation of tumour volumes for the radiotherapy of lung cancer: derivation from phantom measurements and validation in patient data. Eur J Nucl Med Mol Imaging 2008; 35: pp. 1989-1999.


- 296\. Breen S.L., Publicover J., De Silva S., et. al.: Intraobserver and interobserver variability in GTV delineation on FDG-PET-CT images of head and neck cancers. Int J Radiat Oncol Biol Phys 2007; 68: pp. 763-770.


- 297\. Bosmans G., van Baardwijk A., Dekker A., et. al.: Intra-patient variability of tumor volume and tumor motion during conventionally fractionated radiotherapy for locally advanced non-small-cell lung cancer: a prospective clinical study. Int J Radiat Oncol Biol Phys 2006; 66: pp. 748-753.


- 298\. Coleman R.E., Delbeke D., Guiberteau M.J., et. al.: Concurrent PET/CT with an integrated imaging system: intersociety dialogue from the joint working group of the American College of Radiology, the Society of Nuclear Medicine, and the Society of Computed Body Tomography and Magnetic Resonance. J Nucl Med 2005; 46: pp. 1225-1239.


- 299\. Bischof Delaloye A., Carrio I., Cuocolo A., et. al.: White paper of the European Association of Nuclear Medicine (EANM) and the European Society of Radiology (ESR) on multimodality imaging. Eur J Nuc Med Mol Imaging 2007; 34: pp. 1147-1151.


- 300\. Graves E.E., Quon A., Loo B.W.: RT\_Image: an open-source tool for investigating PET in radiation oncology. Technol Cancer Res Treat 2007; 6: pp. 111-121.


- 301\. Jannin P., Fitzpatrick J.M., Hawkes D.J., et. al.: Validation of medical image processing in image-guided therapy. IEEE Trans Med Imaging 2002; 21: pp. 1445-1449.


- 302\. Tomei S., Reilhac A., Visvikis D., et. al.: Development of a database of realistic simulated whole body 18F-FDG images for lymphoma. Proc IEEE Nuclear Science Symposium and Medical Imaging Conference. Dresden.2008.IEEEGermany 4958–4963


- 303\. Mamede M., El Fakhri G., Abreu-e-Lima P., et. al.: Pre-operative estimation of esophageal tumor metabolic length in FDG-PET images with surgical pathology confirmation. Ann Nucl Med 2007; 21: pp. 553-562.


- 304\. Geets X., Lee J., Bol A., et. al.: A gradient-based method for segmenting FDG-PET images: methodology and validation. Eur J Nuc Med Mol Imaging 2007; 34: pp. 1427-1438.


- 305\. Venel Y., Garhi H., de Muret A., et. al.: Comparaison de six méthodes de segmentation du volume tumoral sur la 18F-FDG TEP-TDM avec le volume de référence anatomopathologique dans les cancers bronchopulmonaires non à petites cellules. Médecine Nucléaire 2008; 32: pp. 339-353.


- 306\. Drever L.A., Roa W., McEwan A., et. al.: Comparison of three image segmentation techniques for target volume delineation in positron emission tomography. J Appl Clin Med Phys 2007; 8: pp. 93-109.


- 307\. Visser E.P., Philippens M.E.P., Kienhorst L., et. al.: Comparison of tumor volumes derived from glucose metabolic rate maps and SUV maps in dynamic 18F-FDG PET. J Nucl Med 2008; 49: pp. 892-898.


- 308\. Aerts H.J., Bosmans G., van Baardwijk A.A., et. al.: Stability of (18)F-Deoxyglucose uptake locations within tumor during radiotherapy for NSCLC: a prospective study. Int J Radiat Oncol Biol Phys 2008; 71: pp. 1402-1407.


- 309\. Qiao F., Pan T., Clark J., et. al.: Joint model of motion and anatomy for PET image reconstruction. Med Phys 2007; 34: 426–439


- 310\. Lamare F., Cresson T., Savean J., et. al.: Respiratory motion correction for PET oncology applications using affine transformation of list mode data. Phys Med Biol 2007; 52: pp. 121-140.


- 311\. Rahmim A., Dinelle K., Cheng J.-C., et. al.: Accurate event-driven motion compensation in high-resolution PET incorporating scattered and random events. IEEE Trans Med Imaging 2008; 27: pp. 1018-1033.


- 312\.  Boutchko R, Reutter B, Gullberg G, et al. Correlating motion of internal organs with the displacements of fiducial markers during respiration. IEEE Nuclear Science Symposium & Medical Imaging Conference. 19–25 October 2008, Dresden, Germany; 2008, 3641–3642.


- 313\.  McQuaid S, Lambrou T, Hutton B. Statistical shape modeling of the diaphragm for application to Rb-82 cardiac PET-CT studies. IEEE Nuclear Science Symposium & Medical Imaging Conference. 19–25 October 2008, Dresden, Germany; 2008, 3651–3655.


- 314\.  Dey J, Segars W, Pretorius P, et al. Estimation and correction of irregular respiratory motion of the heart in presence of partial angle effects due to amplitude binning in SPECT. IEEE Nuclear Science Symposium & Medical Imaging Conference. 19–25 October 2008, Dresden, Germany; 2008, 3656–3662.


- 315\.  Bond S, Kadir T, Hamill J, et al. Automatic registration of cardiac PET/CT for attenuation correction. IEEE Nuclear Science Symposium & Medical Imaging Conference. 19–25 October 2008, Dresden, Germany; 2008, 5512–5517.


- 316\.  Chen S, Tsui B. Accuracy analysis of image-based respiratory motion estimation and compensation in respiratory gated PET reconstruction. IEEE Nuclear Science Symposium & Medical Imaging Conference. 19–25 October 2008, Dresden, Germany; 2008, 4292–4295.


- 317\. Lucignani G.: Respiratory and cardiac motion correction with 4D PET imaging: shooting at moving targets. Eur J Nucl Med Mol Imaging 2009; 36: pp. 315-319.


- 318\. Rahmim A., Rousset O., Zaidi H.: Strategies for motion tracking and correction in PET. PET Clin 2007; 2: pp. 251-266.


- 319\. Guido A., Fuccio L., Rombi B., et. al.: Combined (18)F-FDG-PET/CT imaging in radiotherapy target delineation for head-and-neck cancer. Int J Radiat Oncol Biol Phys 2009; 73: pp. 759-763.


- 320\. Deantonio L., Beldi D., Gambaro G., et. al.: FDG-PET/CT imaging for staging and radiotherapy treatment planning of head and neck carcinoma. Radiat Oncol 2008; 3: pp. 29.


- 321\. Murakami R., Uozumi H., Hirai T., et. al.: Impact of FDG-PET/CT fused imaging on tumor volume assessment of head-and-neck squamous cell carcinoma: intermethod and interobserver variations. Acta Radiol 2008; 49: pp. 693-699.


- 322\. Riegel A.C., Berson A.M., Destian S., et. al.: Variability of gross tumor volume delineation in head-and-neck cancer using CT and PET/CT fusion. Int J Radiat Oncol Biol Phys 2006; 65: pp. 726-732.


- 323\. Leong T., Everitt C., Yuen K., et. al.: A prospective study to evaluate the impact of FDG-PET on CT-based radiotherapy treatment planning for oesophageal cancer. Radiother Oncol 2006; 78: pp. 254-261.


- 324\. Gondi V., Bradley K., Mehta M., et. al.: Impact of hybrid fluorodeoxyglucose positron-emission tomography/computed tomography on radiotherapy planning in esophageal and non-small-cell lung cancer. Int J Radiat Oncol Biol Phys 2007; 67: pp. 187-195.


- 325\. Konski A., Doss M., Milestone B., et. al.: The integration of 18-fluoro-deoxy-glucose positron emission tomography and endoscopic ultrasound in the treatment-planning process for esophageal carcinoma. Int J Radiat Oncol Biol Phys 2005; 61: pp. 1123-1128.


- 326\. Vesprini D., Ung Y., Dinniwell R., et. al.: Improving observer variability in target delineation for gastro-oesophageal cancer - the role of (18F)fluoro-2-deoxy-d-glucose positron emission tomography/computed tomography. Clin Oncol (R Coll Radiol) 2008; 20: pp. 631-638.


- 327\.  Yu HM, Liu YF, Hou M, et al. Evaluation of gross tumor size using CT, (18)F-FDG PET, integrated (18)F-FDG PET/CT and pathological analysis in non-small cell lung cancer. Eur J Radiol. In press.


- 328\. van Der Wel A., Nijsten S., Hochstenbag M., et. al.: Increased therapeutic ratio by 18FDG-PET CT planning in patients with clinical CT stage N2-N3M0 non-small-cell lung cancer: a modeling study. Int J Radiat Oncol Biol Phys 2005; 61: pp. 649-655.


- 329\. Ceresoli G.L., Cattaneo G.M., Castellone P., et. al.: Role of computed tomography and \[(18F\]) fluorodeoxyglucose positron emission tomography image fusion in conformal radiotherapy of non-small cell lung cancer: a comparison with standard techniques with and without elective nodal irradiation. Tumori 2007; 93: pp. 88-96.


- 330\. Ford E.C., Lavely W.C., Frassica D.A., et. al.: Comparison of FDG-PET/CT and CT for delineation of lumpectomy cavity for partial breast irradiation. Int J Radiat Oncol Biol Phys 2008; 71: pp. 595-602.


- 331\. Dolezelova H., Slampa P., Ondrova B., et. al.: The impact of PET with 18FDG in radiotherapy treatment planning and in the prediction in patients with cervix carcinoma: results of pilot study. Neoplasma 2008; 55: pp. 437-441.


- 332\. Lin L.L., Mutic S., Low D.A., et. al.: Adaptive brachytherapy treatment planning for cervical cancer using FDG-PET. Int J Rad Oncol Biol Phys 2007; 67: pp. 91-96.


- 333\. Bassi M.C., Turri L., Sacchetti G., et. al.: FDG-PET/CT imaging for staging and target volume delineation in preoperative conformal radiotherapy of rectal cancer. Int J Radiat Oncol Biol Phys 2008; 70: pp. 1423-1426.


- 334\. Dehdashti F., Grigsby P.W., Mintun M.A., et. al.: Assessing tumor hypoxia in cervical cancer by positron emission tomography with 60Cu-ATSM: relationship to therapeutic response-a preliminary report. Int J Radiat Oncol Biol Phys 2003; 55: pp. 1233-1238.


- 335\. Popperl G., Gotz C., Rachinger W., et. al.: Serial O-(2-\[(18)F\]fluoroethyl)-L-tyrosine PET for monitoring the effects of intracavitary radioimmunotherapy in patients with malignant glioma. Eur J Nucl Med Mol Imaging 2006; 33: pp. 792-800.