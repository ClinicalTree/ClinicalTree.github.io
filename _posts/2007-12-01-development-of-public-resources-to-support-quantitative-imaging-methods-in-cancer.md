---
title: Development of Public Resources to Support Quantitative Imaging Methods in Cancer
author: [Laurence P. Clarke,Barbara Croft]
date: 2007-12-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 12 SOURCE CL_S_AcademicRadiologyVolume14Issue12 1}]
tags: [Journals,General Radiology]
---
Recent advances in high-resolution, multi-detector X-ray-CT have resulted in this imaging modality being used in lung cancer screening by some proponents because of its potential to detect lung cancer as a nodule within the lung. This detection, coupled with timely intervention, may potentially reduce lung cancer mortality. To study the morbidity end-point implications more closely, the NCI along with other research groups are engaged in a number of lung cancer screening trials. Coincident with these lung cancer-screening trials, it has been recognized that computer-assisted diagnosis (CAD) methods might serve as useful aides to radiologists for image interpretation, potentially improving the sensitivity and specificity for both the detection and characterization tasks. However, methods or related image data sets needed to optimize and assess the performance of CAD techniques prior to their inclusion in the clinical trial setting, and later in clinical practice, have not been readily available.

In response to this significant unmet need, the NCI issued the Lung Image Database Consortium (LIDC) RFA in 2000 with the goal of developing a validated lung image database, with related meta-data, as a public resource \[ \]. This database would serve as an agreed upon environment to facilitate the task of benchmarking the performance of CAD tools, (i.e., permitting the comparison of CAD results with expert radiologists’ annotations and image mark up of lung nodules). To populate the database, representative X-ray CT data from the NCI and other lung cancer screening programs are being collected, validated and hosted on NCI’s imaging archive NCIA; see  ncia.nci.nih.gov/ . Five academic institutions were funded through this open competition RFA in late 2001, and together are governed by a steering committee with representation from NCI program staff, FDA (CDRH) and NIST scientists. The primary goal of the steering committee is to help ensure that the resource is broadly recognized by both the academic and industry communities:  http://imaging.cancer.gov/reportsandpublications/reportsandpresentations/firstdataset

The targeted date for completion of this LIDC resource that will contain 400 annotated CT images is early in 2008. An extension of this lung database using both projection X-ray (e.g., CXR) and X-ray CT is underway through an associated public private partnership, organized by the Foundation of NIH. This database will contain 600 CT images annotated by expert radiologists, with 300 of these having an associated and annotated digital CXR. This extension of the LIDC database is now referred to as the Image Database Resource Initiative (IDRI), and will be publicly available in 2009:  http://www.fnih.org/partners/research\_environment/IDRI.shtml

An image database designed as a _reference standard_ to evaluate the relative performance of clinical decision tools for cancer screening/diagnosis objectively has never been developed prior to this effort. Several academic centers and industrial groups have developed image databases in house to optimize and validate their own software tools, such as for breast cancer screening using X-ray mammography. However, these databases were not populated by different research centers and then used as a resource to compare the performance of a wide range of algorithm designs.

The development of this public resource posed many scientific and logistical problems. For example, implementing this reference standard required a consensus for all procedures used to generate this resource. Examples of consensus requirements for the lung database include: (a) minimum technical requirements for imaging protocol across different CT platforms, (b) CT quality control methods and image display systems, (c) criteria for inclusion and exclusion of cases, (d) image annotation methods, and (e) spatial truth estimates based on expert observers \[ \]. The most critical performance requirement during database development was to minimize any bias that might occur in the creation of this reference resource that would favor any particular software tool or method. The CAD algorithms often use unique mathematical operational criteria and optimization parameters to improve performance, and the database must be impartial to any possible CAD methods. Similarly, creating a web -accessible resource to query this database and to train and test software tools against sub-sets of images and image mark up, posed several new informational technology challenges in the areas of informatics and statistics, many of which have yet to be fully resolved.

Three publications in this issue of Academic Radiology are highlighted by this editorial \[ \]. They are unique in their scope, because they report research efforts that reflect a well-articulated consensus process across the five academic sites of LIDC with federal agency scientific oversight. The work reported by Sam Armato et al., \[ \] and Michael McNittGray et al., \[ \] each demonstrate the complexity for defining both the presence of nodules or non-nodules of varying size, and the characterization of nodules within the CT lung volume as being non-cancerous or cancerous. This process required the creation of a lung nodule library to visually define what a lung nodule is with current CT scanning methodology, and to train already experienced chest radiologists to characterize lung nodules and their spatial extent based on a consistent set of instructions. In addition, methods to define the boundary of nodules proved to be very challenging, requiring probability maps to be generated, reflecting the spatial variance of radiologist’s assessment of nodule boundaries \[ \]. The work reported by McNitt-Gray et al., outlines a two-stage method for identifying and characterizing lung nodules, a multi-step “process model” for annotation and image mark up methods, that avoids a forced reader consensus, and describes some of the technical challenges in implementing this unique approach. In addition, quality assurance methods were implemented to ensure the integrity of the annotations and the “truth” they represent, as reported elsewhere by Armato et al \[ \]. Finally, the work reported in this issue of Academic Radiology by Anthony Reeves et al., \[ \] reflects the type of analysis that is critically required to characterize this resource and to compare the performance of different algorithms. Thus one goal is to encourage sharing of results to help drive a consensus on how to evaluate increasingly complex computer methods, including related statistical tools.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Clarke L.P., Croft B.Y., Staab E., et. al.: National Cancer Institute initiative: Lung image database resource for imaging research. Academic Radiology 2001; 8: pp. 447-450.


- 2\. Armato S.G., McLennan G., McNitt-Gray M.F., et. al.: Lung Image Database Consortium: Developing a resource for the medical imaging research community. Radiology 2004; 232: pp. 739-748.


- 3\. Armato S.G., Roberts R.Y., McNitt-Gray M.F., et. al.: The Lung Image Database Consortium (LIDC): Ensuring the integrity of expert-defined “truth”. Academic Radiology 2007; 14: pp. 1455-1463.


- 4\. McNitt-Gray M.F., Armato S.G., Meyer C.R., et. al.: The Lung Image Database Consortium (LIDC) Data Collection Process for Nodule Detection and Annotation. Academic Radiology 2007; 14: pp. 1464-1474.


- 5\. Reeves A.P., Biancardi A.M., Apanasovich T.V.: The Lung Image Database Consortium (LIDC): A comparison of different size metrics for pulmonary nodule measurements. Academic Radiology 2007; 14: pp. 1475-1485.


- 6\. Meyer C.R., TD Johnson, G McLennan, et. al.: Evaluation of lung MDCT nodule annotations across radiologists and methods. Acad Radiol 2006; 13: pp. 1254-1265.


- 7\. Armato S.G., Roberts R.Y., McLennan G., et. al.: The Lung Image Database Consortium (LIDC): A quality assurance model for the collection of expert-defined “truth” in lung-nodule-based image analysis studies. SPIE Proceedings 2007; 6514: (in press)


- 8\. Therasse P., Arbuck S.G., Eisenhauer E.A., et. al.: New guidelines to evaluate the response to treatment in solid tumors. J Natl Cancer Inst 2000; 92: pp. 205-216. Feb 2


- 9\.  Doot R K, Saletore Y., Mankoff, D. A. and Kinahan. P. E et al., Reproducibility of Quantifying Tracer Uptake with PET/CT for Evaluation of Response to Therapy “Presented at 2007 IEEE Nuclear Science Symposium (NSS) and Medical Imaging Conference (MIC), Honolulu, Hawaii October 28 to November 3.”


- 10\. Kinahan P.E., Christian P.E., Karp J.S., Divgi C., Zubal G., Pappas V., McEwan A.J.: A calibration phantom for multi-center PET/CT studies of assessing response to therapy. Journal of Nuclear Medicine 2007; 48: pp. 194P. vol., supplement 2, pp. (abstract)