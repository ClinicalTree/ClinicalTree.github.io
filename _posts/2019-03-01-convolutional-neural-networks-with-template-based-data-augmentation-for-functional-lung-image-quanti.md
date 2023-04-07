---
title: Convolutional Neural Networks with Template-Based Data Augmentation for Functional Lung Image Quantification
author: [CL_AT_NicholasJTustisonDSc,CL_AT_BrianBAvants,CL_AT_ZixuanLin,CL_AT_XueFeng,CL_AT_NicholasCullen,CL_AT_JaimeFMata,CL_AT_LuciaFlors,CL_AT_JamesCGee,CL_AT_TalissaAAltes,CL_AT_IIIMuglerJohnP,CL_AT_KunQing]
date: 2019-03-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 26, Issue 3]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We propose an automated segmentation pipeline based on deep learning for proton lung MRI segmentation and ventilation-based quantification which improves on our previously reported methodologies in terms of computational efficiency while demonstrating accuracy and robustness. The large data requirement for the proposed framework is made possible by a novel template-based data augmentation strategy. Supporting this work is the open-source _ANTsRNet_ —a growing repository of well-known deep learning architectures first introduced here.

## Materials and Methods

Deep convolutional neural network (CNN) models were constructed and trained using a custom multilabel Dice metric loss function and a novel template-based data augmentation strategy. Training (including template generation and data augmentation) employed 205 proton MR images and 73 functional lung MRI. Evaluation was performed using data sets of size 63 and 40 images, respectively.

## Results

Accuracy for CNN-based proton lung MRI segmentation (in terms of Dice overlap) was left lung: 0.93 ± 0.03, right lung: 0.94 ± 0.02, and whole lung: 0.94 ± 0.02. Although slightly less accurate than our previously reported joint label fusion approach (left lung: 0.95 ± 0.02, right lung: 0.96 ± 0.01, and whole lung: 0.96 ± 0.01), processing time is <1 second per subject for the proposed approach versus ∼30 minutes per subject using joint label fusion. Accuracy for quantifying ventilation defects was determined based on a consensus labeling where average accuracy (Dice multilabel overlap of ventilation defect regions plus normal region) was 0.94 for the CNN method; 0.92 for our previously reported method; and 0.90, 0.92, and 0.94 for expert readers.

## Conclusion

The proposed framework yields accurate automated quantification in near real time. CNNs drastically reduce processing time after offline model construction and demonstrate significant future potential for facilitating quantitative analysis of functional lung MRI.

## INTRODUCTION

Probing lung function under a variety of conditions and/or pathologies has been significantly facilitated by the use of hyperpolarized gas imaging and corresponding quantitative image analysis methodologies. Such developments have provided direction and opportunity for current and future research trends . Computational techniques targeting these imaging technologies permit spatial quantification of localized ventilation with potential for increased reproducibility, resolution, and robustness over traditional spirometry and radiological readings , .

One of the most frequently used image-based biomarkers for the study of pulmonary development and disease is based on the quantification of regions of limited ventilation, also known as _ventilation defects_ . These features have been shown to be particularly salient in a clinical context. For example, ventilation defect volume to total lung volume ratio has been shown to outperform other image-based features in discriminating asthmatics versus nonasthmatics . Ventilation defects have also demonstrated discriminative capabilities in chronic obstructive pulmonary disease and asthma . These findings, along with related research, have motivated the development of multiple automated and semiautomated segmentation algorithms which have been proposed in the literature (eg, ) and are currently used in a variety of clinical research investigations (eg, ).

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## MATERIALS AND METHODS

## Image Acquisition

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Image Processing and Analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Illustration of the proposed workflow. Training the U-net models for both proton and ventilation imaging includes template-based data augmentation. This offline training is computationally intensive but is only performed once. Subsequent individual subject preprocessing includes MR denoising and bias correction. The proton mask determined from the proton U-net model is included as a separate channel (in deep learning software parlance) for ventilation image processing. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/0_1s20S1076633218303878.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Previous Approaches From Our Group for Lung and Ventilation-Based Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Preprocessing

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Side-by-side image comparison showing the effects of preprocessing on the proton (top) and ventilation (bottom) MRI. (a) Uncorrected image showing MR field inhomogeneity and noise. (b) Corresponding corrected image in which the bias effects have been ameliorated.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/1_1s20S1076633218303878.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## U-Net Architecture for Structural/Functional Lung Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, The modified U-net architecture for both structural and functional lung segmentation (although certain parameters, specifically the number of filters per convolution layer, are specific to the functional case). Network layers are represented as boxes with arrows designating connections between layers. The main parameter value for each layer is provided above the corresponding box. Each layer of the descending (or “encoding”) branch of the network is characterized by two convolutional layers. Modification of the original architecture includes an intermediate dropout layer for regularization (dropout rate = 0.2). A max pooling operation produces the feature map for the next series. The ascending (or “decoding”) branch is similarly characterized. A convolutional transpose operation is used to upsample the feature map following a convolution → dropout → convolution layer series until the final convolutional operation which yields the segmentation probability maps. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/2_1s20S1076633218303878.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Template-Based Data Augmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Snew=Ssource(φ−1target(φsource))
S

n

e

w

=

S

s

o

u

r

c

e

(

φ

t

a

r

g

e

t

−

1

(

φ

s

o

u

r

c

e

)

)


![Figure 4, Template-based data augmentation for the proton (left) and ventilation (right) U-net model generation. For both cases, a template is created, or selected, to generate the transforms to and from the template. The derived deformable, invertible transform for the k th subject, S k to the template, T , is denoted by φ k : S k ↔ T . These subject-specific mappings are used during model training (but not the template itself). Data augmentation occurs by randomly choosing a reference subject and a target subject during batch processing. In the illustration above, the sample mapping of Subject 1 to the space of Subject 2, represented by the green curved arrow, is defined as φ−12(φ1) φ2−1(φ1) . (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/3_1s20S1076633218303878.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ANTsRNet

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Current ANTsRNet Capabilities Comprising Architectures for Applications in Image Segmentation, Image Classification, Object Localization, and Image Super-Resolution. Self-Contained Examples with Data are also Provided to Demonstrate Usage for Each of the Architectures. Although the Majority of Neural Network Architectures are Originally Described for 2-D Images, we Generalized the Work to 3-D Implementations Where Possible


**ANTsRNet****Image Segmentation** U-net  (2-D) Extends fully convolutional neural networks by including an upsampling decoding path with skip connections linking corresponding encoding/decoding layers. V-net  (3-D) 3-D extension of U-net which incorporates a customized Dice loss function.**Image Classification** AlexNet  (2-D, 3-D) Convolutional neural network that precipitated renewed interest in neural networks. VGG16/VGG19  (2-D, 3-D) Also known as “OxfordNet.” VGG architectures are much deeper than AlexNet. Two popular styles are implemented. GoogLeNet  (2-D) A 22-layer network formed from _inception blocks_ meant to reduce the number of parameters relative to other architectures. ResNet  (2-D, 3-D) Characterized by specialized _residualized blocks_ (and skip connections. ResNeXt  (2-D, 3-D) A variant of ResNet distinguished by a hyperparameter called _cardinality_ defining the number of independent paths. DenseNet  (2-D, 3-D) Based on the observation that performance is typically enhanced with shorter connections between the layers and the input.**Object Localization** SSD  (2-D, 3-D) The Multibox Single-Shot Detection (SSD) algorithm for determining bounding boxes around objects of interest. SSD7  (2-D, 3-D) Lightweight SSD variant which increases speed by slightly sacrificing accuracy. Training size requirements are smaller.**Image super-resolution** SRCNN  (2-D, 3-D) Image super-resolution using CNNs.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Processing Specifics

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)




[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)




[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)




[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)




[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    - -
      [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)




[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## RESULTS

## Proton MRI Lung Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

we applied it to the evaluation data consisting of the same 62 proton MRI used in . We performed a direct comparison with the JLF method of with an adopted modification that we currently use in our studies. Instead of using the entire atlas set (which would require a large number of pairwise image registrations), we align the center of the image to be segmented with each atlas image and compute a neighborhood cross-correlation similarity metric . We then select the 10 atlas images that are most similar for use in the JLF scheme. The resulting performance numbers (in terms of Dice overlap) are similar to what we obtained previously and are given in  Figure 5 along with the Dice overlap numbers from the CNN-based approach.

![Figure 5, The Dice overlap coefficient for the left and right lungs (and their combination) between the updated latter requires significantly less computation time. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/4_1s20S1076633218303878.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Ventilation MRI Lung Segmentation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, The Dice overlap coefficient for total, normal lung, and ventilation defect regions for segmentation of the functional evaluation data set. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/5_1s20S1076633218303878.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## DISCUSSION

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Problematic case showing potential issues with the JLF approach (left) for proton lung segmentation where a difficult pairwise image registration caused segmentation failure. In contrast, by learning features directly, the U-net approach (right) avoids possible registration difficulties. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/6_1s20S1076633218303878.jpg)

![Figure 8, Ventilation segmentation comparison between a human reader and the two computational approaches. Notice the effects of the partial voluming at the apex of the lungs, indicated by the yellow arrow, which are labeled as ventilation defect by the Atropos approach whereas U-net and the human reader correctly label this region. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/ConvolutionalNeuralNetworkswithTemplateBasedDataAugmentationforFunctionalLungImageQuantification/7_1s20S1076633218303878.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ACKNOWLEDGMENTS

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## REFERENCES

- 1\. Liu Z, Araki T, Okajima Y, et. al.: Pulmonary hyperpolarized noble gas MRI: recent advances and perspectives in clinical application. Eur J Radiol 2014; 83: pp. 1282-1291.


- 2\. Roos JE, McAdams HP, Kaushik SS, et. al.: Hyperpolarized gas MR imaging: technique and applications. Magn Reson Imaging Clin N Am 2015; 23: pp. 217-229.


- 3\. Adamson EB, Ludwig KD, Mummy DG, et. al.: Magnetic resonance imaging with hyperpolarized agents: methods and applications. Phys Med Biol 2017; 62: pp. R81-R123.


- 4\. Svenningsen S, Kirby M, Starr D, et. al.: What are ventilation defects in asthma?. Thorax 2014; 69: pp. 63-71.


- 5\. Tustison NJ, Altes TA, Song G, et. al.: Feature analysis of hyperpolarized helium-3 pulmonary MRI: a study of asthmatics versus nonasthmatics. Magn Reson Med 2010; 63: pp. 1448-1455.


- 6\. Kirby M, Pike D, Coxson HO, et. al.: Hyperpolarized (3) He ventilation defects used to predict pulmonary exacerbations in mild to moderate chronic obstructive pulmonary disease. Radiology 2014; 273: pp. 887-896.


- 7\. Altes TA, Mugler JP, Ruppert K, et. al.: Clinical correlates of lung ventilation defects in asthmatic children. J Allergy Clin Immunol 2016; 137: pp. 789-796. e7


- 8\. Tustison NJ, Avants BB, Flors L, et. al.: Ventilation-based segmentation of the lungs using hyperpolarized (3) He MRI. J Magn Reson Imaging 2011; 34: pp. 831-841.


- 9\. Kirby M, Heydarian M, Svenningsen S, et. al.: Hyperpolarized 3He magnetic resonance functional imaging semiautomated segmentation. Acad Radiol 2012; 19: pp. 141-152.


- 10\. He M, Kaushik SS, Robertson SH, et. al.: Extending semiautomatic ventilation defect analysis for hyperpolarized (129)Xe ventilation MRI. Acad Radiol 2014; 21: pp. 1530-1541.


- 11\. Zha W, Niles DJ, Kruger SJ, et. al.: Semiautomated ventilation defect quantification in exercise-induced bronchoconstriction using hyperpolarized helium-3 magnetic resonance imaging: a repeatability study. Acad Radiol 2016; 23: pp. 1104-1114.


- 12\. Hughes PJC, Horn FC, Collier GJ, et. al.: Spatial fuzzy c-means thresholding for semiautomated calculation of percentage lung ventilated volume from hyperpolarized gas and 1 H MRI. J Magn Reson Imaging 2018; 47: pp. 640-646.


- 13\. Trivedi A, Hall C, Hoffman EA, et. al.: Using imaging as a biomarker for asthma. J Allergy Clin Immunol 2017; 139: pp. 1-10.


- 14\. LeCun Y, Bengio Y, Hinton G: Deep learning. Nature 2015; 521: pp. 436-444.


- 15\. Russakovsky O, Deng J, Su H, et. al.: ImageNet large scale visual recognition challenge. Int J Comput Vis 2015; 115: pp. 211-252.


- 16\. Krizhevsky A, Sutskever I, Hinton GE: ImageNet classification with deep convolutional neural networks.Proceedings of the 25th international conference on neural information processing systems - volume 1.2012.pp. 1097-1105. Available at http://dl.acm.org/citation.cfm? id=2999134.2999257


- 17\. Simonyan K, Zisserman A: Very deep convolutional networks for large-scale image recognition. CoRR 2014; abs/1409.1556 2014. Available at: http://arxiv.org/abs/1409.1556

- 18\. Szegedy C, Vanhoucke V, Ioffe S, et. al.: Rethinking the inception architecture for computer vision. CoRR 2015; abs/1512.00567 2015. Available at: http://arxiv.org/abs/1512.00567

- 19\. LeCun Y, Bottou L, Bengio Y, et. al.: Gradient-based learning applied to document recognition. Proc IEEE 1998; 86: pp. 2278-2324.


- 20\. Fukushima K: Neocognitron: a self-organizing neural network model for a mechanism of pattern recognition unaffected by shift in position. Biol Cybern 1980; 36: pp. 193-202.


- 21\. Hubel DH, Wiesel TN: Receptive fields, binocular interaction and functional architecture in the cat's visual cortex. J Physiol 1962; 160: pp. 106-154.


- 22\. Litjens G, Kooi T, Bejnordi BE, et. al.: A survey on deep learning in medical image analysis. Med Image Anal 2017; 42: pp. 60-88.


- 23\. Ronneberger O, Fischer P, Brox T: U-net: convolutional networks for biomedical image segmentation. Proc Int Conf Med Image Comput Comput-Assist Interv 2015; 9351: pp. 234-241.


- 24\. Tustison Nicholas J., Qing Kun, Wang Chengbo, Altes Talissa A, Mugler III John P: Atlas-based estimation of lung and lobar anatomy in proton MRI. Magn Reson Med Jul 2016; 76: pp. 315-320.


- 25\. Taylor L, Nitschke G: Improving deep learning using generic data augmentation. CoRR 2017; abs/1708.06020, 2017. Available at: http://arxiv.org/abs/1708.06020

- 26\. Tustison NJ, Avants BB: Explicit B-spline regularization in diffeomorphic image registration. Front Neuroinform 2013; 7: pp. 39.


- 27\. Avants BB, Tustison NJ, Song G, et. al.: A reproducible evaluation of ANTs similarity metric performance in brain image registration. Neuroimage 2011; 54: pp. 2033-2044.


- 28\.  Available at:  https://github.com/stnava/ANTsR

- 29\.  Available at:  https://github.com/ntustison/DeepVentNet

- 30\. Altes TA, Johnson M, Fidler M, et. al.: Use of hyperpolarized helium-3 MRI to assess response to ivacaftor treatment in patients with cystic fibrosis. J Cyst Fibros 2017; 16: pp. 267-274.


- 31\. Tustison NJ, Avants BB, Cook PA, et. al.: N4ITK: improved N3 bias correction. IEEE Trans Med Imaging 2010; 29: pp. 1310-1320.


- 32\. Qing K, Altes TA, Tustison NJ, et. al.: Rapid acquisition of helium-3 and proton three-dimensional image sets of the human lung in a single breath-hold using compressed sensing. Magn Reson Med 2015; 74: pp. 1110-1115.


- 33\. Wang H, Suh JW, Das SR, et. al.: Multi-Atlas Segmentation with Joint Label Fusion. IEEE Trans Pattern Anal Machine Intell March 2013; 35: pp. 611-623.


- 34\.  Available at:  https://github.com/ntustison/LungAndLobeEstimationExample

- 35\.  Available at:  https://github.com/ntustison/LungVentilationSegmentationExample

- 36\. Manjón JV, Coupé P, Martí-Bonmatí L, et. al.: Adaptive non-local means denoising of MR images with spatially varying noise levels. J Magn Reson Imaging 2010; 31: pp. 192-203.


- 37\. Shelhamer E, Long J, Darrell T: Fully convolutional networks for semantic segmentation. IEEE Trans Pattern Anal Mach Intell 2017; 39: pp. 640-651.


- 38\. Srivastava N, Hinton G, Krizhevsky A, et. al.: Dropout: a simple way to prevent neural networks from overfitting. J Machine Learn Res 2014; 15: pp. 1929-1958.


- 39\.  Available at:  https://github.com/ANTsX/ANTsRNet

- 40\. Avants BB, Yushkevich P, Pluta J, et. al.: The optimal template effect in hippocampus studies of diseased populations. Neuroimage 2010; 49: pp. 2457-2466.


- 41\. Yang X, Kwitt R, Styner M, et. al.: Quicksilver: fast predictive image registration—a deep learning approach. Neuroimage 2017; 158: pp. 378-396.


- 42\.  Available at:  https://doi.org/10.6084/m9.figshare.4964915.v1  .


- 43\. Cullen NC, Avants BB: Convolutional neural networks for rapid and simultaneous brain extraction and tissue segmentation. Brain Morphometry 2018; 136: pp. 13-36.


- 44\. Nair V, Hinton GE: Rectified linear units improve restricted Boltzmann machines.Proceedings of the 27th international conference on machine learning.2010.


- 45\. Warfield SK, Zou KH, Wells WM: Simultaneous truth and performance level estimation (STAPLE): an algorithm for the validation of image segmentation. IEEE Trans Med Imaging 2004; 23: pp. 903-921.


- 46\. Wong SC, Gatt A, Stamatescu V, et. al.: Understanding data augmentation for classification: when to warp?. CoRR 2016; abs/1609.08764, 2016


- 47\. Milletari F, Navab N, Ahmadi S: V-net: fully convolutional neural networks for volumetric medical image segmentation. CoRR 2016; abs/1606.04797, 2016. Available at: http://arxiv.org/abs/1606.04797

- 48\. He K, Zhang X, Ren S, et. al.: Deep residual learning for image recognition. CoRR 2015; abs/1512.03385, 2015. Available at: http://arxiv.org/abs/1512.03385

- 49\. Xie S, Girshick RB, Dollár P, et. al.: Aggregated residual transformations for deep neural networks. CoRR 2016; abs/1611.05431, 2016. Available at: http://arxiv.org/abs/1611.05431

- 50\. Huang G, Liu Z, Weinberger KQ: Densely connected convolutional networks. CoRR 2016; abs/1608.06993, 2016 Available at :http://arxiv.org/abs/1608.06993

- 51\. Liu W, Anguelov D, Erhan D, et. al.: SSD: single shot multibox detector. CoRR 2015; abs/1512.02325, 2015. Available at: http://arxiv.org/abs/1512.02325

- 52\.  Available at:  https://github.com/pierluigiferrari/ssd\_keras

- 53\. Dong C, Loy CC, He K, et. al.: Image super-resolution using deep convolutional networks. IEEE Trans Pattern Anal Mach Intell 2016; 38: pp. 295-307.