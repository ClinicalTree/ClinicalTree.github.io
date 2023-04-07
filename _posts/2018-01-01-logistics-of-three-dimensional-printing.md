---
title: Logistics of Three-dimensional Printing
author: [CL_AT_TarynHodgdonMD,CL_AT_RamanDanradMD,CL_AT_MidhirJPatelMD,CL_AT_StacyESmithMD,CL_AT_MichaelLRichardsonMD,CL_AT_DavidHBallardMD,CL_AT_SayedAliMD,CL_AT_AnthonyPaulTraceMDPhD,CL_AT_CarolynnMDeBenedectisMD,CL_AT_MatthewEZygmontMD,CL_AT_LeonLenchikMD,CL_AT_SummerJDeckerPhD]
date: 2018-01-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 25, Issue 1]
tags: [Journals,General Radiology]
---
The Association of University Radiologists Radiology Research Alliance Task Force on three-dimensional (3D) printing presents a review of the logistic considerations for establishing a clinical service using this new technology, specifically focused on implications for radiology. Specific topics include printer selection for 3D printing, software selection, creating a 3D model for printing, providing a 3D printing service, research directions, and opportunities for radiologists to be involved in 3D printing. A thorough understanding of the technology and its capabilities is necessary as the field of 3D printing continues to grow. Radiologists are in the unique position to guide this emerging technology and its use in the clinical arena.

## Introduction

Producing three-dimensional (3D) physical prototypes from digital models became popular in the late 1990s . Over the past decade, the heath-care sector has shown increased interest in this technology for clinical use. Radiology has a long-standing history of acquiring and maintaining volumetric anatomic data. This precedent leaves our specialty at an advantage to unlock the true potential of medical 3D printing for mainstream use.

The process of creating 3D models from digital data can be categorized into four major steps: image acquisition, image segmentation, creation of a 3D model, and transfer of model data to a 3D printer . Image acquisition is most commonly in the form of computed tomography (CT), due to rapid acquisition and relative ease of image post-processing for 3D printing . The volumetric data are analyzed to ensure that there are no gaps in anatomy during acquisition . Volumetric data from CT, magnetic resonance imaging (MRI), or ultrasound images are rendered in digital imaging and communication in medicine (DICOM) format. DICOM data cannot be 3D printed, and thus image data require conversion using specialized software into one of several output file types amenable for 3D printing. The most common of these is Standard Tessellation Language or STereoLithography (STL) format, which helps 3D printers to define objects by surfaces that enclose a region of space . These surfaces are defined as collections of triangles called facets.

Segmentation is the process of extracting region of interest (ROI)-specific data and refining the STL representation of the selected anatomy . This step requires specialized software to ensure model integrity, preferably with software programs that are approved by the Food and Drug Administration (FDA) . Parts of segmentation can be automated or manual, which can serve as a challenge for radiologists who may be unfamiliar with the application software.

After segmentation, acquired STL data are sent to another program for creation of a 3D model . Open-source and commercially available computer-aided design or computer-aided manufacturing software packages include many post-processing techniques, such as smoothing and wrapping, that must be used to ensure printability of a 3D model (  Table 1 ). Lastly, the completed STL file is transferred to a 3D printer for production. The various steps of creating a 3D model are illustrated in  Figure 1 .

TABLE 1


Examples of Various Free Software Platforms Available for the Creation of 3D-printed Models


CURA Beginner Slicer software to prepare STL files for 3D printing Free PC, Mac, Linux CRAFTWARE Beginner Slicer software to prepare STL files for 3D printing Free PC, Mac OSIRIX Intermediate To create 3D model and prepare STL file Osirix lite (32 bit) is free. Mac only Osirix MD (64 bit) costs about $600 USD HOROS Intermediate To create 3D model and prepare STL file 64-bit Free, donation to user group requested Mac only NETFABB Intermediate Slicer to prepare STL files for 3D printing Basic free, professional edition paid PC, Mac, Linux REPETIER Intermediate-advanced Slicer software to prepare STL files for 3D printing Free PC, Mac, Linux 3-D TOOL Intermediate To view and check STL files Free PC MESHFIX Intermediate Check STL files Free PC SLIC3R Professional Slicer software to prepare STL files for 3D printing Free PC, Mac, Linux BLENDER Professional Edit STL files for 3D printing Free PC, Mac

PC, personal computer; STL, Standard Tessellation Language or STereoLithography; 3D, three-dimensional.


![Figure 1, Flowchart demonstrating the workflow for printing of a 3D model. After acquiring the images, DICOM files are initially segmented to extract the anatomy of interest. An STL file is created and post-processed with CAD software. Support scaffolds can also be created to hold the model parts in place. The completed STL file is then sent to the 3D printer for printing. CAD, computer-aided software; DICOM, digital imaging and communication in medicine; STL, Standard Tessellation Language or STereoLithography; 3D, three-dimensional.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/LogisticsofThreedimensionalPrinting/0_1s20S1076633217303604.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Printer Selection for 3D Printing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Material Extrusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Powder Bed Fusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Vat Photopolymerization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Material Jetting

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Binder Jetting

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Sheet Lamination

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Directed Energy Deposition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Software Selection for 3D Printing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Creating a 3D Model for Printing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


![Figure 2, Example demonstrating how the software package ( Mimics Innovation Suite) can be used to segment the bones of the skull from source CT head images to generate a 3D model. CT, computed tomography; 3D, three-dimensional.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/LogisticsofThreedimensionalPrinting/1_1s20S1076633217303604.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 5.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


  - [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - (a)
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - (b)
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - (c)
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - (d)
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - (e)
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - (f)
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - (g)
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 6.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 7.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, (a) 3D-Printed model of a skull created after using post-processing and 3D printing software, PreForm , to convert the model into an STL file and designing support structures for the model to be used during the printing process. The skulls pictured were printed on (b) Stratasys and (c) ZCorp printers, respectively. STL, Standard Tessellation Language or STereoLithography; 3D, three-dimensional.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/LogisticsofThreedimensionalPrinting/2_1s20S1076633217303604.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Providing a 3D Printing Service

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Entry-level Use

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Educational Use

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, 3D-Printed model of a complex acetabular fracture. By providing greater anatomic detail and tactile information about the fracture type, these models can help to determine treatment options (surgical vs nonsurgical) and to plan adequate fracture reduction preoperatively. The model pictured was printed on a Stratasys Objet500 Connex3 printer using jetting of VeroWhite material.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/LogisticsofThreedimensionalPrinting/3_1s20S1076633217303604.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Clinical Use

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Research Directions in 3D Printing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## General Directions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, 3D-Printed tracheal model with fabricated tracheal stents of a 58-year-old man with long-standing respiratory symptoms due to tracheobronchomalacia. (a) and (b) Computed tomography (CT) of the chest with inspiration (a) and expiration (b) revealing greater than 50% collapse in the carina and left mainstem bronchus. (c) CT DICOM data used to segment the trachea and create an STL file (3D Slicer version 4.6, www.slicer.org ). (d) and (e) 3D-rendered models and (f) 3D-printed stent. The final model was used in the treatment of this patient. DICOM, digital imaging and communication in medicine; STL, Standard Tessellation Language or STereoLithography; 3D, three-dimensional.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/LogisticsofThreedimensionalPrinting/4_1s20S1076633217303604.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials Research

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Other Research Opportunities

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Mitsouras D., Liacouras P., Imanzadeh A., et. al.: Medical 3D printing for the radiologist. Radiographics 2015; 35: pp. 1965-1988. PubMed PMID; : 26562233 Epub 2015/11/13; PMCID: PMC4671424


- 2\. Marro A., Bandukwala T., Mak W.: Three-dimensional printing and medical imaging: a review of the methods and applications. Curr Probl Diagn Radiol 2016; 45: pp. 2-9. PubMed PMID; : 26298798 Epub 2015/08/25


- 3\. Mishra S.: Application of 3D printing in medicine. Indian Heart J 2016; 68: pp. 108-109. PubMed PMID; : 26896278 Epub 2016/02/21; PMCID: PMC4759482


- 4\. Rybicki F.J., Otero H.J., Steigner M.L., et. al.: Initial evaluation of coronary images from 320-detector row computed tomography. Int J Cardiovasc Imaging 2008; 24: pp. 535-546. PubMed PMID; : 18368512 Epub 2008/03/28


- 5\. Christensen A., Rybicki F.J.: Maintaining safety and efficacy for 3D printing in medicine. 3D Print Med 2017; 3: pp. 1.


- 6\. Prima M.: Additively manufactured medical products—the FDA perspective. 3D Print Med 2015; 2:


- 7\. Kim G.B., Lee S., Kim H., et. al.: Three-dimensional printing: basic principles and applications in medicine and radiology. Korean J Radiol 2016; 17: pp. 182-197. PubMed PMID; : 26957903 Epub 2016/03/10; PMCID: PMC4781757


- 8\. Friedman T., Michalski M., Goodman T.R., et. al.: 3D printing from diagnostic images: a radiologist's primer with an emphasis on musculoskeletal imaging—putting the 3D printing of pathology into the hands of every physician. Skeletal Radiol 2016; 45: pp. 307-321. PubMed PMID; : 26592802 Epub 2015/11/26


- 9\. Matsumoto J.S., Morris J.M., Foley T.A., et. al.: Three-dimensional physical modeling: applications and experience at Mayo Clinic. Radiographics 2015; 35: pp. 1989-2006. PubMed PMID; : 26562234 Epub 2015/11/13


- 10\. Anastasiou A., Tsirmpas C., Rompas A., et. al.: 3D printing: basic concepts mathematics and technologies. 13th IEEE International Conference on BioInformatics and BioEngineering; 2013 10–13 Nov2013.


- 11\. Wojtyla S., Klama P., Baran T.: Is 3D printing safe? Analysis of the thermal treatment of thermoplastics: ABS, PLA, PET, and nylon. J Occup Environ Hyg 2017; 14: pp. D80-D85. PubMed PMID; : 28165927 Epub 2017/02/07


- 12\. Kakizawa H., Toyota N., Akiyama Y., et. al.: A three-dimensional laminated paper model of the scaphoid from computed tomography. Acta Radiol (Stockholm, Sweden: 1987) 2007; 48: pp. 80-88. PubMed PMID; : 17325931 Epub 2007/02/28


- 13\. Leng S., McGee K., Morris J., et. al.: Anatomic modeling using 3D printing: quality assurance and optimization. 3D Print Med 2017; 3: pp. 6.


- 14\. Bortolotto C., Eshja E., Peroni C., et. al.: 3D printing of CT dataset: validation of an open source and consumer-available workflow. J Digit Imaging 2016; 29: pp. 14-21. PubMed PMID; : 26175139 Epub 2015/07/16; PMCID: PMC4722024


- 15\. Ford J.M., Decker S.J.: Computed tomography slice thickness and its effects on three-dimensional reconstruction of anatomical structures. J Forensic Radiol Imaging 2016; 4: pp. 43-46.


- 16\. Marcus R.P., Morris J.M., Matsumoto J.M., et. al.: Implementation of iterative metal artifact reduction in the pre-planning-procedure of three-dimensional physical modeling. 3D Print Med 2017; 3: pp. 5.


- 17\. Poornima B., Sumathi A.: Image registration techniques for satellite and medical images: a survey. Int J Sci Eng Res 2013; 4: pp. 2090-2101.


- 18\. Oberg E.J., Franklin D., Horton H.L., et. al.: Machinery's handbook.25th ed.1996.Industrial PressNew York, NY, USA


- 19\. AlAli A.B., Griffin M.F., Butler P.E.: Three-dimensional printing surgical applications. Eplasty 2015; 15: pp. e37. PubMed PMID; : 26301002 Epub 2015/08/25; PMCID: PMC4539849


- 20\. Preece D., Williams S.B., Lam R., et. al.: Let's get physical”: advantages of a physical model over 3D computer models and textbooks in learning imaging anatomy. Anat Sci Educ 2013; 6: pp. 216-224. PubMed PMID; : 23349117 Epub 2013/01/26


- 21\. Brown G.A., Firoozbakhsh K., DeCoster T.A., et. al.: Rapid prototyping: the future of trauma surgery?. J Bone Joint Surg Am 2003; 85: pp. 49-55. PubMed PMID; : 14652393 Epub 2003/12/04


- 22\. Esses S.J., Berman P., Bloom A.I., et. al.: Clinical applications of physical 3D models derived from MDCT data and created by rapid prototyping. AJR Am J Roentgenol 2011; 196: pp. W683-W688. PubMed PMID; : 21606254 Epub 2011/05/25


- 23\. Frame M., Huntley J.S.: Rapid prototyping in orthopaedic surgery: a user's guide. ScientificWorldJournal 2012; 2012: pp. 838575. PubMed PMID; : 22666160 Epub 2012/06/06; PMCID: PMC3361341


- 24\. Malik H.H., Darwood A.R., Shaunak S., et. al.: Three-dimensional printing in surgery: a review of current surgical applications. J Surg Res 2015; 199: pp. 512-522. PubMed PMID; : 26255224 Epub 2015/08/10


- 25\. Martelli N., Serrano C., van den Brink H., et. al.: Advantages and disadvantages of 3-dimensional printing in surgery: a systematic review. Surgery 2016; 159: pp. 1485-1500. PubMed PMID; : 26832986 Epub 2016/02/03


- 26\. Murray D.J., Edwards G., Mainprize J.G., et. al.: Advanced technology in the management of fibrous dysplasia. J Plast Reconstr Aesthet Surg 2008; 61: pp. 906-916. PubMed PMID; : 18339597 Epub 2008/03/15


- 27\. Zheng Y.X., Yu D.F., Zhao J.G., et. al.: 3D printout models vs. 3D-rendered images: which is better for preoperative planning?. J Surg Educ 2016; 73: pp. 518-523. PubMed PMID; : 26861582 Epub 2016/02/11


- 28\. He Y., Xue G.H., Fu J.Z.: Fabrication of low cost soft tissue prostheses with the desktop 3D printer. Sci Rep 2014; 4: pp. 6973. PubMed PMID; : 25427880 Epub 2014/11/28; PMCID: PMC4245596


- 29\. Ibrahim A.M., Jose R.R., Rabie A.N., et. al.: Three-dimensional printing in developing countries. Plast Reconstr Surg Glob Open 2015; 3: pp. e443. PubMed PMID; : 26301132 Epub 2015/08/25; PMCID: PMC4527617


- 30\. Naftulin J.S., Kimchi E.Y., Cash S.S.: Streamlined, inexpensive 3D printing of the brain and skull. PLoS ONE 2015; 10: PubMed PMID; : 26295459 e0136198; Epub 2015/08/22; PMCID: PMC4546422


- 31\. Cheng Y.L., Chen S.J.: Manufacturing of cardiac models through rapid prototyping technology for surgery planning. Mater Sci Forum 2006; 505–507: pp. 1063-1068. doi:10.4028/www.scientific.net/MSF.505-507.1063


- 32\. Zopf D.A., Hollister S.J., Nelson M.E., et. al.: Bioresorbable airway splint created with a three-dimensional printer. N Engl J Med 2013; 368: pp. 2043-2045. PubMed PMID; : 23697530 Epub 2013/05/24


- 33\. US Food and Drug Administration : CDRH May 10, 2016, Document no. 1400002. Technical considerations for additive manufactured devices. Draft Guidance for Industry and Food and Drug Administration Staff2016.


- 34\. US Food and Drug Administration : CDRH fiscal year 2015 (FY 2015) proposed guidance development and focused retrospective review of final guidance.2015.


- 35\. Morrison R.J., Kashlan K.N., Flanangan C.L., et. al.: Regulatory considerations in the design and manufacturing of implantable 3D-printed medical devices. Clin Transl Sci 2015; 8: pp. 594-600. PubMed PMID; : 26243449 Epub 2015/08/06; PMCID: PMC4626249


- 36\. Fan H., Fu J., Li X., et. al.: Implantation of customized 3-D printed titanium prosthesis in limb salvage surgery: a case series and review of the literature. World J Surg Oncol 2015; 13: pp. 308. PubMed PMID; : 26537339 Epub 2015/11/06; PMCID: PMC4632365


- 37\. Hong S.B., Eliaz N., Leisk G.G., et. al.: A new Ti-5Ag alloy for customized prostheses by three-dimensional printing (3DP). J Dent Res 2001; 80: pp. 860-863. PubMed PMID; : 11379885 Epub 2001/05/31


- 38\. Ng C.S.: Recent and future developments in chest wall reconstruction. Semin Thorac Cardiovasc Surg 2015; 27: pp. 234-239. PubMed PMID; : 26686454 Epub 2015/12/22


- 39\. Banks J.: Adding value in additive manufacturing: researchers in the United Kingdom and Europe look to 3D printing for customization. IEEE Pulse 2013; 4: pp. 22-26. PubMed PMID; : 24233187 Epub 2013/11/16


- 40\. Chia H.N., Wu B.M.: Recent advances in 3D printing of biomaterials. J Biol Engrg 2015; 9: pp. 4. PubMed PMID; : 25866560 Epub 2015/04/14; PMCID: PMC4392469


- 41\. Rankin T.M., Giovinco N.A., Cucher D.J., et. al.: Three-dimensional printing surgical instruments: are we there yet?. J Surg Res 2014; 189: pp. 193-197. PubMed PMID; : 24721602 Epub 2014/04/12; PMCID: PMC4460996


- 42\. Arora A., Datarkar A.N., Borle R.M., et. al.: Custom-made implant for maxillofacial defects using rapid prototype models. J Oral Maxillofac Surg 2013; 71: pp. e104-e110. PubMed PMID; : 23351764 Epub 2013/01/29


- 43\. Grant G.T., Taft R.M., Wheeler S.T.: Practical application of polyurethane and Velcro in maxillofacial prosthetics. J Prosthet Dent 2001; 85: pp. 281-283. PubMed PMID; : 11264936 Epub 2001/03/27


- 44\. Harrysson O.L., Hosni Y.A., Nayfeh J.F.: Custom-designed orthopedic implants evaluated using finite element analysis of patient-specific computed tomography data: femoral-component case study. BMC Musculoskelet Disord 2007; 8: pp. 91. PubMed PMID; : 17854508 Epub 2007/09/15; PMCID: PMC2100040


- 45\. Woodfield T.B., Guggenheim M., von Rechenberg B., et. al.: Rapid prototyping of anatomically shaped, tissue-engineered implants for restoring congruent articulating surfaces in small joints. Cell Prolif 2009; 42: pp. 485-497. PubMed PMID; : 19486014 Epub 2009/06/03


- 46\. Yoo S.-J., Thabit O., Kim E.K., et. al.: 3D printing in medicine of congenital heart diseases. 3D Print Med 2016; 2: pp. 3.


- 47\. Bizzotto N., Tami I., Santucci A., et. al.: 3D printed replica of articular fractures for surgical planning and patient consent: a two years multi-centric experience. 3D Print Med 2016; 2: pp. 2.


- 48\. Tabakovic S.Z., Konstantinovic V.S., Radosavljevic R., et. al.: Application of computer-aided designing and rapid prototyping technologies in reconstruction of blowout fractures of the orbital floor. J Craniofac Surg 2015; 26: pp. 1558-1563. PubMed PMID; : 26125649 Epub 2015/07/01


- 49\. Zhou L.B., Shang H.T., He L.S., et. al.: Accurate reconstruction of discontinuous mandible using a reverse engineering/computer-aided design/rapid prototyping technique: a preliminary clinical study. J Oral Maxillofac Surg 2010; 68: pp. 2115-2121. PubMed PMID; : 20542365 Epub 2010/06/15


- 50\. Lee J.Y., Choi B., Wu B., et. al.: Customized biomimetic scaffolds created by indirect three-dimensional printing for tissue engineering. Biofabrication 2013; 5: pp. 045003. PubMed PMID; : 24060622 Epub 2013/09/26; PMCID: PMC3852984


- 51\. Makitie A.A., Korpela J., Elomaa L., et. al.: Novel additive manufactured scaffolds for tissue engineered trachea research. Acta Otolaryngol 2013; 133: pp. 412-417. PubMed PMID; : 23394221 Epub 2013/02/12


- 52\. Mannoor M.S., Jiang Z., James T., et. al.: 3D printed bionic ears. Nano Lett 2013; 13: pp. 2634-2639. PubMed PMID; : 23635097 Epub 2013/05/03; PMCID: PMC3925752


- 53\. Wang X., Yan Y., Zhang R.: Rapid prototyping as a tool for manufacturing bioartificial livers. Trends Biotechnol 2007; 25: pp. 505-513. PubMed PMID; : 17949840 Epub 2007/10/24


- 54\. Giannopoulos A.A., Mitsouras D., Yoo S.J., et. al.: Applications of 3D printing in cardiovascular diseases. Nat Rev Cardiol 2016; 13: pp. 701-718. PubMed PMID; : 27786234 Epub 2016/11/05


- 55\. Ripley B., Kelil T., Cheezum M.K., et. al.: 3D printing based on cardiac CT assists anatomic visualization prior to transcatheter aortic valve replacement. J Cardiovasc Comput Tomogr 2016; 10: pp. 28-36. PubMed PMID; : 26732862 Epub 2016/01/07


- 56\. Markert M., Weber S., Lueth T.C.: A beating heart model 3D printed from specific patient data. Conf Proc IEEE Eng Med Biol Soc 2007; 2007: pp. 4472-4475. PubMed PMID; : 18002998 Epub 2007/11/16


- 57\. Gao B., Yang Q., Zhao X., et. al.: 4D Bioprinting for biomedical applications. Trends Biotechnol 2016; 34: pp. 746-756. PubMed PMID; : 27056447 Epub 2016/04/09


- 58\. Li Y.C., Zhang Y.S., Akpek A., et. al.: 4D Bioprinting: the next-generation technology for biofabrication enabled by stimuli-responsive materials. Biofabrication 2016; 9: pp. 012001. PubMed PMID; : 27910820 Epub 2016/12/03


- 59\. Kunz M., Ma B., Rudan J.F., et. al.: Image-guided distal radius osteotomy using patient-specific instrument guides. J Hand Surg Am 2013; 38: pp. 1618-1624. PubMed PMID; : 23890500 Epub 2013/07/31


- 60\. Biglino G., Verschueren P., Zegels R., et. al.: Rapid prototyping compliant arterial phantoms for in-vitro studies and device testing. J Cardiovasc Magn Reson 2013; 15: pp. 2. PubMed PMID; : 23324211 Epub 2013/01/18.; PMCID: PMC3564729


- 61\. Canstein C., Cachot P., Faust A., et. al.: 3D MR flow analysis in realistic rapid-prototyping model systems of the thoracic aorta: comparison with in vivo data and computational fluid dynamics in identical vessel geometries. Magn Reson Med 2008; 59: pp. 535-546. PubMed PMID; : 18306406 Epub 2008/02/29


- 62\. Cao P., Duhamel Y., Olympe G., et. al.: A new production method of elastic silicone carotid phantom based on MRI acquisition using rapid prototyping technique. Conf Proc IEEE Eng Med Biol Soc 2013; 2013: pp. 5331-5334. PubMed PMID; : 24110940 Epub 2013/10/11


- 63\. Ionita C.N., Mokin M., Varble N., et. al.: Challenges and limitations of patient-specific vascular phantom fabrication using 3D polyjet printing. Proc SPIE Int Soc Opt Eng 2014; 9038: pp. 90380m. PubMed PMID; : 25300886 Epub 2014/10/11; PMCID: PMC4188370


- 64\. Markl M., Schumacher R., Kuffer J., et. al.: Rapid vessel prototyping: vascular modeling using 3t magnetic resonance angiography and rapid prototyping technology. Magma (New York, NY) 2005; 18: pp. 288-292. PubMed PMID; : 16369802 Epub 2005/12/22


- 65\. Steigner M.L., Mitsouras D., Whitmore A.G., et. al.: Iodinated contrast opacification gradients in normal coronary arteries imaged with prospectively ECG-gated single heart beat 320-detector row computed tomography. Circ Cardiovasc Imaging 2010; 3: pp. 179-186. PubMed PMID; : 20044512 Epub 2010/01/02; PMCID: PMC3063948


- 66\. Lindegaard J.C., Madsen M.L., Traberg A., et. al.: Individualised 3D printed vaginal template for MRI guided brachytherapy in locally advanced cervical cancer. Radiother Oncol 2016; 118: pp. 173-175. PubMed PMID; : 26743833 Epub 2016/01/09


- 67\. Mitsouras D., Lee T.C., Liacouras P., et. al.: Three-dimensional printing of MRI-visible phantoms and MR image-guided therapy simulation. Magn Reson Med 2017; 77: pp. 613-622. PubMed PMID; : 26864335 Epub 2016/02/13; PMCID: PMC5108690


- 68\. Morrison R.J., Hollister S.J., Niedner M.F., et. al.: Mitigation of tracheobronchomalacia with 3D-printed personalized medical devices in pediatric patients. Sci Transl Med 2015; 7: pp. 285ra64. PubMed PMID; : 25925683 Epub 2015/05/01; PMCID: PMC4495899


- 69\. Paydarfar J.A., Wu X., Halter R.J.: MRI- and CT-compatible polymer laryngoscope: a step toward image-guided transoral surgery. Otolaryngol Head Neck Surg 2016; 155: pp. 364-366. PubMed PMID; : 27221570 Epub 2016/05/26


- 70\. Ripley B., Levin D., Kelil T., et. al.: 3D printing from MRI data: harnessing strengths and minimizing weaknesses. J Magn Reson Imaging 2017; 45: pp. 635-645. PubMed PMID; : 27875009 Epub 2016/11/23


- 71\. Ebert L.C., Thali M.J., Ross S.: Getting in touch—3D printing in forensic imaging. Forensic Sci Int 2011; 211: pp. e1-e6. PubMed PMID; : 21602004 Epub 2011/05/24


- 72\. Schievano S., Sebire N.J., Robertson N.J., et. al.: Reconstruction of fetal and infant anatomy using rapid prototyping of post-mortem MR images. Insights Imaging 2010; 1: pp. 281-286. PubMed PMID; : 22347922 Epub 2010/09/01; PMCID: PMC3259363


- 73\. Kaisar M.A., Sajja R.K., Prasad S., et. al.: New experimental models of the blood-brain barrier for CNS drug discovery. Expert Opin Drug Discov 2017; 12: pp. 89-103. PubMed PMID; : 27782770 Epub 2016/10/27


- 74\. D'Urso P.S., Barker T.M., Earwaker W.J., et. al.: Stereolithographic biomodelling in cranio-maxillofacial surgery: a prospective trial. J Craniomaxillofac Surg 1999; 27: pp. 30-37. PubMed PMID; : 10188125 Epub 1999/04/03


- 75\. Muller A., Krishnan K.G., Uhl E., et. al.: The application of rapid prototyping techniques in cranial reconstruction and preoperative planning in neurosurgery. J Craniofac Surg 2003; 14: pp. 899-914. PubMed PMID; : 14600634 Epub 2003/11/06