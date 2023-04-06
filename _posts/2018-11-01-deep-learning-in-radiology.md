---
title: Deep Learning in Radiology
author: [Morgan P. McBee MD,Omer A. Awan MD MPH CIIP,Andrew T. Colucci MD,Comeron W. Ghobadi MD,Nadja Kadom MD,Akash P. Kansagra MD MS,Srini Tridapani MD PhD MSEE MSCR MBA,William F. Auffermann MD PhD]
date: 2018-11-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 25, Issue 11 SOURCE CL_S_AcademicRadiologyVolume25Issue11 1}]
tags: [Journals,General Radiology]
---
As radiology is inherently a data-driven specialty, it is especially conducive to utilizing data processing techniques. One such technique, deep learning (DL), has become a remarkably powerful tool for image processing in recent years. In this work, the Association of University Radiologists Radiology Research Alliance Task Force on Deep Learning provides an overview of DL for the radiologist. This article aims to present an overview of DL in a manner that is understandable to radiologists; to examine past, present, and future applications; as well as to evaluate how radiologists may benefit from this remarkable new tool. We describe several areas within radiology in which DL techniques are having the most significant impact: lesion or disease detection, classification, quantification, and segmentation. The legal and ethical hurdles to implementation are also discussed. By taking advantage of this powerful tool, radiologists can become increasingly more accurate in their interpretations with fewer errors and spend more time to focus on patient care.

## Introduction

Recent rapid advances in computer hardware and software now allow computers to perform an increasing number of tasks that have historically not been possible . The technologies that can in some ways mimic the decision-making abilities of humans are known by several names, depending on the nature of the algorithms used. One of the more sophisticated sets of algorithms is often referred to as deep learning (DL). DL has made great advances in recent years, now performing tasks that only humans could perform just a few years ago. Some may perceive DL algorithms as a threat to medicine and radiology. However, DL is like any other tool, intrinsically neither good nor evil, but rather dependent on the application. In this work, the Association of University Radiologists Radiology Research Alliance Task Force on Deep Learning provides an overview of DL for the radiologist. The goal of this task force was to examine developments in DL and how they will influence the current and future practice of radiology. This article seeks to present an overview of DL in a manner that is understandable to radiologists; to examine past, present, and future applications; and to evaluate how radiologists may benefit from this remarkable new tool. Additional resources providing greater depth of coverage are included for the interested reader.

## Evolution of Artificial Intelligence and Machine Learning

Most people's knowledge of artificial intelligence (AI) is derived from science fiction movies. AI is defined as “the capacity of computers or other machines to exhibit or simulate intelligent behavior” and is now a thriving field and the focus of a great amount of research and investment. Early on, the focus of AI was to address problems that were difficult for humans but relatively straight forward for computers to solve. Such problems include abstract and formal mathematical problems, such as adjusting the window and the level of a radiographic image on a viewing workstation. Additionally, the early attempts of AI were based on rigid predefined rules, but this approach was largely unsuccessful .

An advance in AI was the advent of machine learning (ML), which is the ability of an AI system to extract information from raw data and to learn from experience. This avoids the need for “human operators to formally specify all of the knowledge that the computer needs” . For example, an ML algorithm introduced in 1990 utilized logistic regression to determine whether or not cesarean section was appropriate .

Broadly speaking, ML comprises a set of algorithms that aim to allow computers to receive an assortment of input data and to generate complex inferences that are based on potentially obscure relationships between inputs. For example, ML algorithms may play an important role in combining financial data (such as company and industry earnings reports) and nonfinancial data (including information of geopolitical events and weather patterns) to generate nuanced recommendations about whether to buy or sell an equity stock position.

## What Is Deep Learning?

DL has received a great deal of attention lately both in the consumer world and throughout the medical community, whereas ML algorithms have been a focus of research for many years. There has been a renewed interest in DL algorithms lately since they reduced the top-5 error by 10% in 2012 at the ImageNet Large Scale Visual Recognition Challenge . Top-5 error is defined as “the fraction of test images for which the correct label is not among the five labels considered most probable by the model.” Every year since then, DL models have dominated the challenges, significantly reducing the top-5 error, and in 2015, human performance was surpassed by DL algorithms.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Basic representation of an artificial neural network with neurons similar to those within a brain. The left layer of the neural network is called the input layer and contains neurons that encode the values of the input pixels. The rightmost layer is called the output layer , which contains the output neurons. The middle contains “n” number of hidden layers , which perform mathematical transformations or convolutions of the data. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeepLearninginRadiology/0_1s20S1076633218301041.jpg)

![Figure 2, A representative example of how increasing the number of layers ( x axis) increases the test accuracy ( y axis).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeepLearninginRadiology/1_1s20S1076633218301041.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, A curve showing the convergence of accuracy for a machine learning algorithm for chest radiograph data as a function of the number of iterations (epochs).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeepLearninginRadiology/2_1s20S1076633218301041.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Current Advances in Deep Learning Outside of Medicine

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Gaming

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Chess

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Go

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Language

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Imaging

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Deep Learning in Medicine

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Current Applications in Radiology

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Lesion or Disease Detection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Classification

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Differences between classification using conventional algorithms and deep learning algorithms. Note that Σ indicates combination of data inputs.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeepLearninginRadiology/3_1s20S1076633218301041.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Quantification

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


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, A representative example of chest and lung segmentation. (a) Original computed tomography image of the chest in lung windows. (b) Region of the image corresponding to the lungs. (c) Segmented image with the chest wall and the mediastinum removed and the lungs isolated.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/DeepLearninginRadiology/4_1s20S1076633218301041.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Speech Recognition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Current Limitations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Future Applications

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Schmidhuber J.: Deep learning in neural networks: An overview. Neural Netw 2015; 61: pp. 85-117.


- 2\. Dictionary OE : Artificial intelligence, n. Oxford University Press; Available at: http://www.oed.com

- 3\. Goodfellow I., Bengio Y., Courville A.: Deep learning.2016.MIT Press


- 4\. Mor-Yosef S., Samueloff A., Modan B., et. al.: Ranking the risk factors for cesarean: logistic regression analysis of a nationwide study. Obstet Gynecol 1990; 75: pp. 944-947.


- 5\. Krizhevsky A., Sutskever I., Hinton G.E.: ImageNet classification with deep convolutional neural networks. Lake Tahoe, Nevada, Curran Associates Inc2012.


- 6\. Moeskops P., Viergever M.A., Mendrik A.M., et. al.: Automatic segmentation of MR brain images with a convolutional neural network. IEEE Trans Med Imaging 2016; 35: pp. 1252-1261.


- 7\. Tajbakhsh N., Shin J.Y., Gurudu S.R., et. al.: Convolutional neural networks for medical image analysis: full training or fine tuning?. IEEE Trans Med Imaging 2017;


- 8\. Bar Y., Diamant I., Wolf L., et. al.: Chest pathology detection using deep learning with non-medical training. In 2015 IEEE 12th International Symposium on Biomedical Imaging (ISBI)2015.pp. 294-297.


- 9\. Huynh B.Q., Li H., Giger M.L.: Digital mammographic tumor classification using transfer learning from deep convolutional neural networks. J Med Imaging (Bellingham) 2016; 3: pp. 034501.


- 10\. Goodfellow I., Bengio Y., Courville A.: Deep learning.2016.The MIT PressCambridge, MA


- 11\. Campbell M., Hoane A.J., Hsu F.-H.: Deep blue. Artif Intell 2002; 134: pp. 57-83.


- 12\.  Deep learning machine teaches itself chess in 72 hours, plays at international master level. Available at: https://www.technologyreview.com/s/541276/deep-learning-machine-teaches-itself-chess-in-72-hours-plays-at-international-master/#comments

- 13\. Koch C.: How the computer beat the Go master. Nature America, Inc2016.


- 14\. Gibney E.: Go players react to computer defeat.2016.


- 15\. Perez S.: Google's smarter, A.I.-powered translation system expands to more languages. AOL Inc2017.


- 16\. French K.: Your New Best Friend: AI Chatbot. Futurism.. Available at: https://futurism.com/ai-chatbot-meaningful-conversation/

- 17\. Coldewey D.: This neural network “hallucinates” the right colors into black and white pictures. TechCrunch2016.


- 18\. Sebastiani F.: Classification of text, automatic.Brown K.Encyclopedia of language & linguistics.2006.ElsevierOxford:


- 19\. Gulshan V., Peng L., Coram M., et. al.: Development and validation of a deep learning algorithm for detection of diabetic retinopathy in retinal fundus photographs. JAMA 2016; 316: pp. 2402-2410.


- 20\. Esteva A., Kuprel B., Novoa R.A., et. al.: Dermatologist-level classification of skin cancer with deep neural networks. Nature 2017; 542: pp. 115-118.


- 21\. Liu Y., Gadepalli K., Norouzi M., et. al.: Detecting cancer metastases on gigapixel pathology images. arXiv2017.


- 22\. Bar Y., Diamant I., Wolf L., et. al.: Deep learning with non-medical training used for chest pathology identification. In SPIE Medical Imaging2015. SPIE, 9414, 7


- 23\. Lakhani P., Sundaram B.: Deep learning at chest radiography: automated classification of pulmonary tuberculosis by using convolutional neural networks. Radiology 2017; 284: pp. 162326.


- 24\. Cheng J.Z., Ni D., Chou Y.H., et. al.: Computer-aided diagnosis with deep learning architecture: applications to breast lesions in us images and pulmonary nodules in CT scans. Sci Rep 2016; 6: pp. 24454.


- 25\. Kooi T., Litjens G., van Ginneken B., et. al.: Large scale deep learning for computer aided detection of mammographic lesions. Med Image Anal 2017; 35: pp. 303-312.


- 26\. Wang J., Yang X., Cai H., et. al.: Discrimination of breast cancer with microcalcifications on mammography by deep learning. Sci Rep 2016; 6: pp. 27327.


- 27\. Hua K.L., Hsu C.H., Hidayati S.C., et. al.: Computer-aided classification of lung nodules on computed tomography images via deep learning technique. Onco Targets Ther 2015; 8: pp. 2015-2022.


- 28\. Rajkomar A., Lingam S., Taylor A.G., et. al.: High-throughput classification of radiographs using deep convolutional neural networks. J Digit Imaging 2016; pp. 1-7.


- 29\. Wang C., Elazab A., Wu J., et. al.: Lung nodule classification using deep feature fusion in chest radiography. Comput Med Imaging Graph 2017; 57: pp. 10-18.


- 30\. van Ginneken B.: Fifty years of computer analysis in chest imaging: rule-based, machine learning, deep learning. Radiol Phys Technol 2017; 10: pp. 23-32.


- 31\. Armato S.G., Altman M.B., Wilkie J., et. al.: Automated lung nodule classification following automated nodule detection on CT: a serial approach. Med Phys 2003; 30: pp. 1188-1197.


- 32\. Dou Q., Chen H., Yu L., et. al.: Multilevel contextual 3-D CNNs for false positive reduction in pulmonary nodule detection. IEEE Trans Biomed Eng 2017; 64: pp. 1558-1567.


- 33\. Nibali A., He Z., Wollersheim D.: Pulmonary nodule classification with deep residual networks. Int J Comput Assist Radiol Surg 2017; LID


- 34\. Ciompi F., Chung K., van Riel S.J., et. al.: Towards automatic pulmonary nodule management in lung cancer screening with deep learning. Sci Rep 2017;


- 35\. Kim N., Seo J.B., Lee Y., et. al.: Development of an automatic classification system for differentiation of obstructive lung disease using HRCT. J Digit Imaging 2009; 22: pp. 136-148.


- 36\. Anthimopoulos M., Christodoulidis S., Ebner L., et. al.: Lung pattern classification for interstitial lung diseases using a deep convolutional neural network. IEEE Trans Med Imaging 2017; 35: pp. 1207-1216.


- 37\. Lakhani P.: Deep convolutional neural networks for endotracheal tube position and x-ray image classification: challenges and opportunities. J Digit Imaging 2017; LID


- 38\. Wang J., Kato F., Yamashita H., et. al.: Automatic estimation of volumetric breast density using artificial neural network-based calibration of full-field digital mammography: feasibility on Japanese women with and without breast cancer. J Digit Imaging 2016; pp. 1-13.


- 39\. Lee H., Tajmir S., Lee J., et. al.: Fully automated deep learning system for bone age assessment. J Digit Imaging 2017; pp. 1-15.


- 40\. Cheng P.M., Malhi H.S.: Transfer learning with convolutional neural networks for classification of abdominal ultrasound images. J Digit Imaging 2016; pp. 1-10.


- 41\. Cha K.H., Hadjiiski L.M., Chan H.-P., et. al.: Bladder cancer treatment response assessment using deep learning in CT with transfer learning. In SPIE Medical Imaging2017. SPIE, 10134, 6


- 42\. Chen Y., Dhar R., Heitsch L., et. al.: Automated quantification of cerebral edema following hemispheric infarction: application of a machine-learning algorithm to evaluate CSF shifts on serial head CTs. Neuroimage Clin 2016; 12: pp. 673-680.


- 43\. Haralick R.M., Shanmugam K., Dinstein I.H.: Textural features for image classification. IEEE Trans Syst Man Cybern 1973; 3: pp. 610-621.


- 44\. Galloway M.M.: Texture analysis using gray level run lengths. Comput Graph Image Process 1975; 4: pp. 172-179.


- 45\. Tixier F., Le Rest C.C., Hatt M., et. al.: Intratumor heterogeneity characterized by textural features on baseline 18F-FDG PET images predicts response to concomitant radiochemotherapy in esophageal cancer. J Nucl Med 2011; 52: pp. 369-378.


- 46\. Coroller T.P., Grossmann P., Hou Y., et. al.: CT-based radiomic signature predicts distant metastasis in lung adenocarcinoma. Radiother Oncol 2015; 114: pp. 345-350.


- 47\. Akkus Z., Galimzianova A., Hoogi A., et. al.: Deep learning for brain MRI segmentation: state of the art and future directions. J Digit Imaging 2017; LID


- 48\. Gaonkar B., Hovda D., Martin N., et. al.: Deep learning in the small sample size setting: cascaded feed forward neural networks for medical image segmentation. In SPIE Medical Imaging2016. SPIE, 9785, 8


- 49\. Cheng R., Roth H.R., Lu L., et. al.: Active appearance model and deep learning for more accurate prostate segmentation on MRI. In SPIE Medical Imaging2016. SPIE, 9784, 9


- 50\. Hammana I., Lepanto L., Poder T., et. al.: Speech recognition in the radiology department: a systematic review. Health Inf Manag 2015; 44: pp. 4-10.


- 51\. Deng L., Li X.: Machine learning paradigms for speech recognition: an overview. IEEE Trans Audio Speech Lang Process 2013; 21: pp. 1060-1089.


- 52\. Launchbury J.: A DARPA perspective on artificial intelligence.2017.


- 53\. Moosavi-Dezfooli S.-M., Fawzi A., Fawzi O., et. al.: Universal adversarial perturbations.2016.


- 54\. Summers R.M.: Progress in fully automated abdominal CT interpretation. AJR Am J Roentgenol 2016; 207: pp. 67-79.


- 55\. Wang S., Summers R.M.: Machine learning and radiology. Med Image Anal 2012; 16: pp. 933-951.


- 56\. Mikolas P., Melicher T., Skoch A., et. al.: Connectivity of the anterior insula differentiates participants with first-episode schizophrenia spectrum disorders from controls: a machine-learning study. Psychol Med 2016; 46: pp. 2695-2704.


- 57\. Collij L.E., Heeman F., Kuijer J.P.A., et. al.: Application of machine learning to arterial spin labeling in mild cognitive impairment and Alzheimer disease. Radiology 2016; 281: pp. 865-875.


- 58\. Bryan R.N.: Machine learning applied to Alzheimer disease. Radiology 2016; 281: pp. 665-668.


- 59\. Motwani M., Dey D., Berman D.S., et. al.: Machine learning for prediction of all-cause mortality in patients with suspected coronary artery disease: a 5-year multicentre prospective registry analysis. Eur Heart J 2016; 38: pp. 500-507. ehw188


- 60\. Gaonkar B., Macyszyn L., Bilello M., et. al.: Automated tumor volumetry using computer-aided image segmentation. Acad Radiol 2015; 22: pp. 653-661.