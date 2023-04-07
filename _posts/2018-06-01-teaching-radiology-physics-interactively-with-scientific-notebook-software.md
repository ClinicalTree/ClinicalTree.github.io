---
title: Teaching Radiology Physics Interactively with Scientific Notebook Software
author: [CL_AT_MichaelLRichardsonMD,CL_AT_BehrangAminiMDPhD]
date: 2018-06-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 25, Issue 6]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

The goal of this study is to demonstrate how the teaching of radiology physics can be enhanced with the use of interactive scientific notebook software.

## Methods

We used the scientific notebook software known as Project Jupyter, which is free, open-source, and available for the Macintosh, Windows, and Linux operating systems.

## Results

We have created a scientific notebook that demonstrates multiple interactive teaching modules we have written for our residents using the Jupyter notebook system.

## Conclusions

Scientific notebook software allows educators to create teaching modules in a form that combines text, graphics, images, data, interactive calculations, and image analysis within a single document. These notebooks can be used to build interactive teaching modules, which can help explain complex topics in imaging physics to residents.

## Introduction

The American Board of Radiology (ABR) Core Examination assesses knowledge of physics as part of its overall testing in clinical radiology. Physics questions are integrated into each category of this examination . Topics emphasized include image quality, artifacts, radiation dose, and patient safety for each modality or subspecialty organ system. Radiology residencies therefore include instruction in physics as part of the residency curriculum. However, imparting an adequate understanding of imaging physics remains a challenging task.

Zhang et al. showed that a hands-on exposure to clinically oriented physics was not only well received by radiology residents but also improved their understanding of the material. It occurred to us that such physical hands-on experiences could be supplemented or possibly even replaced by suitable simulations.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Using Jupyter

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Nuclear Medicine

## Module 1. Simple Radioactive Decay

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

A(t)=A0e−λt​,
A

(

t

)

=

A

0

e

−

λ

t

​

,


where _A_ 0 is the initial activity, _t_ is time, and _λ_ is the decay constant—the probability that a radioatom will decay per unit time . This decay constant is related to the isotope's half-life (t12)
(

t

1

2

)
—the time when 50% of the radioatoms present will have decayed—as shown in Equation  2 :


t12=ln(2)λ.
t

1

2

=

l

n

(

2

)

λ

.


Half-life has direct implications in nuclear medicine imaging, radiation therapy, and radiation safety. For example, the half-life can make it relatively simple to calculate how much of a radioisotope will be left after a given time. For example, technetium-99m (  99m Tc) has a half-life of about 6 hours. Therefore, after 24 hours, the remaining amount of  99m Tc will be 1/2 × 1/2 × 1/2 × 1/2 or 1/16 of the original amount.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Jupyter interactive widget for simple radioactive decay.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/0_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Module 2. Technetium Generator Simulation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

99Mo→λA99mTc→λB99Tc
99

M

o

→

λ

A

99

m

T

c

→

λ

B

99

T

c


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

parent→λAdaughter→λBgranddaughter
parent

→

λ

A

daughter

→

λ

B

granddaughter


can be expressed by the Bateman equation (Eq.  5 ) :


Aparent=λdaughterλdaughter−λparentAparent(0)(e−λparentt−e−λdaughtert).
A

parent

=

λ

daughter

λ

daughter

−

λ

parent

A

parent

(

0

)

(

e

−

λ

parent

t

−

e

−

λ

daughter

t

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Parent-daughter isotope activity widget.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/1_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Secular equilibrium

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Transient equilibrium

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Ultrasound

## Module 3. Sound Interference Patterns

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Interference pattern formed by a 15-Hz and a 17-Hz sound.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/2_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Jupyter widget that allows the user to interactively change the frequencies of two sound waves and see and hear the resulting interference pattern.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/3_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Module 4. Doppler Shift Simulation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, A train crossing with an observer some distance back from the tracks.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/4_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

fobs=forig×cc+Vsource,
f

o

b

s

=

f

orig

×

c

c

+

V

source

,


where _f  orig_ is the original frequency, _f  obs_ is the observed frequency, _c_ is the velocity of sound in a medium, and _V  source_ is the speed of the source.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Vradial=Vsource×cosθ,
V

radial

=

V

source

×

cos

θ

,


where _θ_ is the angle between the source's forward direction of travel and the line of sight from the source to the observer.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Doppler shift of each of the frequency components of an Amtrak P5a horn as a function of its position relative to a crossing. Each component is plotted in a different color. For purposes of this plot, the train is traveling from left to right at 27 m/s, and the observer is located 50 m away from the tracks. (Color version of figure is available online.)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/5_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Magnetic Resonance Imaging

## Module 5: T2 vs T2\*

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Mxy(t)=M0e−tT2
M

x

y

(

t

)

=

M

0

e

−

t

T

2


![Figure 7, Decay of transverse magnetization.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/6_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

1T2\*=1T2+1T2i.
1

T

2

\*

=

1

T

2

+

1

T

2

i

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, T2* vs T2 as a function of the percent change in relative field inhomogeneity.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/7_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Module 6: Magic Angle Effect in a Tendon

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Magic angle effect in a simulated ankle tendon.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/8_1s20S107663321830059X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Module 7: MR Contrast Optimization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Intensity=H⋅e−TET2(1−2e−(TR−3τ)T1+2e−(TR−τ)T1−e−TRT1),
Intensity

=

H

⋅

e

−

T

E

T

2

(

1

−

2

e

−

(

T

R

−

3

τ

)

T

1

+

2

e

−

(

T

R

−

τ

)

T

1

−

e

−

T

R

T

1

)

,


where _H_ is the local hydrogen density, T1 is the longitudinal magnetic relaxation constant, T2 is the transverse magnetic relaxation constant, TR is the pulse repetition time, TE is the echo delay, and _τ_ is the time between the first 90° radiofrequency pulse and the first 180° radiofrequency pulse in the spin-echo pulse train.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

contrast=Intensitytumor−Intensitybackground
contrast

=

Intensit

y

tumor

−

Intensit

y

background


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

TABLE 1


Measured Values of Tissue Parameters From the Literature


Tissue H T1 (ms) T2 (ms) Normal fat 1170–1580 214–242 46–58 Normal marrow 1280–1410 210–246 51–60 Normal muscle 1000 456–520 28–40 Fibrosarcoma 1180 991 71 Giant cell tumor 950 965 68 Osteogenic sarcoma 1360–1990 991–1213 58–62

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Magnetic resonance contrast widget. TE, echo delay time; TR, repetition time.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/9_1s20S107663321830059X.jpg)

![Figure 11, Magnetic resonance contrast plot for fibrosarcoma vs normal fat using tissue values from Table 1 . TE, echo delay time; TR, repetition time.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/10_1s20S107663321830059X.jpg)

![Figure 12, Magnetic resonance contrast plot for fibrosarcoma vs normal muscle using tissue values from Table 1 . TE, echo delay time; TR, repetition time.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/TeachingRadiologyPhysicsInteractivelywithScientificNotebookSoftware/11_1s20S107663321830059X.jpg)

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

- 1\. American Board of Radiology : Core exam. Available at https://www.theabr.org/diagnostic-radiology/initial-certification/core-exam#exam-categories

- 2\. Zhang J., Hardy P.A., DiSantis D.J., et. al.: Hands-on physics education of residents in diagnostic radiology. Acad Radiol 2017; 24: pp. 677-681.


- 3\. Shen H.: Interactive notebooks: sharing the code. Nature 2014; 515: pp. 151-152.


- 4\. Van Noorden R.: My digital toolbox: Ecologist Ethan White on interactive notebooks. Nature 2014; Available at http://www.nature.com/news/my-digital-toolbox-ecologist-ethan-white-on-interactive-notebooks-1.16015

- 5\. Osipov D.: The rise of data science notebooks. Available at https://www.datanami.com/2016/05/04/rise-data-science-notebooks/

- 6\. Wolfram Language and System Documentation Center : Using a notebook interface. Available at https://reference.wolfram.com/language/tutorial/UsingANotebookInterface.html

- 7\. Maplesoft : Maplesoft - Software for Mathematics, Online Learning, Engineering. Available at http://www.maplesoft.com

- 8\. Matlab : MathWorks - Makers of MATLAB and Simulink. Available at https://www.mathworks.com

- 9\. Project Jupyter : Project Jupyter Home. Available at http://jupyter.org

- 10\. RStudio Team : Integrated development environment for R.2015.RStudio, Inc.Boston, MA Available at http://www.rstudio.com/

- 11\. Pérez F., Granger B.E.: IPython: a system for interactive scientific computing. Comput Sci Eng 2007; 9: pp. 21-29. Available at http://ipython.org

- 12\. Richardson M.L., Amini B.: Scientific notebook software: applications for radiology. Curr Probl Diagn Radiol 2017; epub ahead of print


- 13\. van der Walt S., Schönberger J.L., Nunez-Iglesias J., et. al.: Scikit-image: image processing in Python. Peer J 2014; 2: pp. e453. https://doi.org/10.7717/peerj.453

- 14\. van der Walt S., Colbert S.C., Varoquaux G.: The NumPy array: a structure for efficient numerical computation. Comput Sci Eng 2011; 13: pp. 22-30.


- 15\. Gruber J.: Markdown: Syntax. Available at https://daringfireball.net/projects/markdown/syntax

- 16\. GitHub contributors : Writing on GitHub/Basic writing and formatting syntax. Available at https://help.github.com/articles/basic-writing-and-formatting-syntax/

- 17\. Mittelbach F., Goossens M.: The LaTeX companion.2nd ed.2004.Addison-WesleyBoston, MA


- 18\. Groch M.W.: Radioactive decay. Radiographics 1998; 18: pp. 1247-1256.


- 19\. Wikipedia : Doppler effect—Wikipedia, the free encyclopedia. Available at https://en.wikipedia.org/w/index.php?title=Doppler\_effect&oldid=831208270

- 20\. Chappell K.E., Robson M.D., Stonebridge-Foster A., et. al.: Magic angle effects in MR neurography. AJNR Am J Neuroradiol 2004; 25: pp. 431-440.


- 21\. Pérez F., Granger B.E., Hunter J.D.: Python: an ecosystem for scientific computing. Comput Sci Eng 2011; 13: pp. 13-21.


- 22\. Erickson S.J., Cox I.H., Hyde J.S., et. al.: Effect of tendon orientation on MR imaging signal intensity: a manifestation of the “magic angle” phenomenon. Radiology 1991; 181: pp. 389-392.


- 23\. Hayes C.W., Parellada J.A.: The magic angle effect in musculoskeletal MR imaging. Top Magn Reson Imaging 1996; 8: pp. 51-56.


- 24\. Marshall H., Howarth C., Larkman D.J., et. al.: Contrast-enhanced magic-angle MR imaging of the Achilles tendon. AJR Am J Roentgenol 2002; 179: pp. 187-192.


- 25\. Oatridge A., Herlihy A., Thomas R.W., et. al.: Magic angle imaging of the Achilles tendon in patients with chronic tendinopathy. Clin Radiol 2003; 58: pp. 384-388.


- 26\. Richardson M.L., Amparo E.G., Gillespy T., et. al.: Theoretical considerations for optimizing intensity differences between primary musculoskeletal tumors and normal tissue with spin-echo magnetic resonance imaging. Invest Radiol 1985; 20: pp. 492-497.


- 27\. Mitchell M.R., Conturo T.E., Gruber T.J., et. al.: AUR memorial award. Two computer models for selection of optimal magnetic resonance imaging (MRI) pulse sequence timing. Invest Radiol 1984; 19: pp. 350-360.


- 28\. AAPM Subcommittee of Physics Education of Physics : Diagnostic radiology physics curriculum. Available at http://www.aapm.org/education/documents/Curriculum.pdf

- 29\. Jacobs C.T., Gorman G.J., Rees H.E., et. al.: Experiences with efficient methodologies for teaching computer programming to geoscientists. J Geosci Educ 2016; 64: pp. 183-198.


- 30\. Milas J.: Jupyter in the classroom. Available at https://deephorizons.github.io/2016/06/06/jupyter-in-the-classroom/

- 31\. Jones B., Beazley D.: Python cookbook—recipes for mastering Python 3.3rd ed.2013.O'ReillySebastopol, CA Available at http://shop.oreilly.com/product/0636920027072.do

- 32\. Chang W.: Cookbook for R.. Available at http://www.cookbook-r.com

- 33\. Teetor P.: R cookbook. O'Reilly. Available at http://shop.oreilly.com/product/9780596809164.do

- 34\. Stack Overflow Contributors : Stack overflow. Available at https://stackoverflow.com