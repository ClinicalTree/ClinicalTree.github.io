---
title: Semiautomatic Segmentation of Vertebrae in Lateral X-rays Using a Conditional Shape Model
author: [J. Eugenio Iglesias MSc,Marleen de Bruijne PhD]
date: 2007-10-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 14, Issue 10 SOURCE CL_S_AcademicRadiologyVolume14Issue10 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

Manual annotation of the full contour of the vertebrae in lateral x-rays for subsequent morphometry is time-consuming. The standard six-point morphometry is commonly used instead. It has been shown that the information from the complete contour improves the quality of the study. In this article, the six landmarks are given and the vertebrae are segmented taking advantage of that information. The result is a semiautomatic system in which the full contour is found with high precision, and that only requires a radiologist to mark six points per vertebra.

## Materials and Methods

A shape model was built for both the six landmarks and the full contours of the vertebrae L1, L2, L3, and L4 of 142 patients. The distribution of the principal components of the full contour was then modeled as a Gaussian conditional distribution depending on the principal components of the six landmarks. The conditional mean was used as initialization for active shape model optimization, and the conditional variance was used to constrain the solution to plausible shapes.

## Results

The achieved point-to-line error was 0.48 mm, and 95% of the points were located within 1.36 mm of the annotated contour. The accuracy is superior to those of previously published studies, at the expense of requiring the six points to be marked. Fractures and osteophytes are well approximated by the model, although they are sometimes oversmoothed.

## Conclusions

The proposed method provides hence a richer description than the six points, and can be used as input for shape-based morphometry to detect and quantify vertebral deformation more accurately.

Osteoporosis is a disease of bone in which the bone mineral density is reduced, bone microarchitecture is disrupted, and the amount and variety of noncollagenous proteins in bone is altered ( ). Bones affected by the disease are more likely to fracture. Osteoporosis is defined by the World Health Organization as either a bone mineral density 2.5 standard deviations below peak bone mass (20-year-old, sex-matched healthy person average) as measured by dual x-ray absorptiometry (DXA), or any fragility fracture. Because of its hormonal component, more women, particularly after menopause, suffer from this disease than men.

Osteoporotic fractures are those that occur under slight amount of stress that would not normally lead to fractures in nonosteoporotic people. Typical fractures occur in the vertebral column, hip, and wrist. Vertebral fractures are the most common ones. They occur in younger patients and they are a good indicator for the risk of future spine and hip fractures. These two are the most serious cases, leading to limited mobility and possibly disability. Hip fracture, in particular, usually requires major surgery, which has important associated risks, such as deep vein thrombosis and pulmonary embolism. Although osteoporosis patients have an increased mortality rate because of the complications of fractures, most patients die with the disease rather than of it.

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Available Data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 1, Six initial landmarks (stars), contour with and selected points (asterisks). Note that the six landmarks are not exactly on the contour.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticSegmentationofVertebraeinLateralXraysUsingaConditionalShapeModel/0_1s20S107663320700308X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Methods

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


  - a
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - b
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - c
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


  - a
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - b
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - c
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - d
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Landmark Placement

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Alignment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

x=\[x1,x2,…,xN,y1,y2,…,yN\]t
x

=

\[

x

1

,

x

2

,

…

,

x

N

,

y

1

,

y

2

,

…

,

y

N

\]

t


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## PDM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

x≈x¯+Pb
x

≈

x

¯

+

Pb


where _b_ can be calculated for a certain shape:


b=Pt(x−x¯)
b

=

P

t

(

x

−

x

¯

)


and the approximation error vector is:


e=x−x¯−Pb=x−x¯−P(Pt(x−x¯))
e

=

x

−

x

¯

−

Pb

=

x

−

x

¯

−

P

(

P

t

(

x

−

x

¯

)

)


where **b** is a column vector of _k_ components, representing the projection of the shape onto the space of the model. Across the training set, the mean of this vector will be zero, and the covariance **C** will be a diagonal matrix including the _k_ eigenvalues _λ  i_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

d=btC−b1−−−−−−√=∑ki=1(b2iλi)−−−−−−−−−√
d

=

b

t

C

−

b

1

=

∑

i

=

1

k

(

b

i

2

λ

i

)


If the condition _d_ < _d  max_ is not true, the _b_ vector can be modified:


b′=b(dmax/d)
b

′

=

b

⁢

(

d

m

a

x

/

d

)


Because the number of fractures in the dataset is low compared with the number of healthy ones, their influence on the model was increased by giving them a higher weight when building it. Two different weights were given to normal and fractured vertebrae when calculating the mean and the variance of the shapes, so that their total contributions were equal. Because 504 healthy and 64 fractured vertebrae were available, the weights were


Wh=12Nheal=0.5504
W

h

=

1

2

N

h

e

a

l

=

0.5

504


Wf=12Nfrac=0.564
W

f

=

1

2

N

f

r

a

c

=

0.5

64


x¯′=∑Nheali=1whxi+∑Nfracj=1wfxj
x

¯

′

=

∑

i

=

1

N

h

e

a

l

w

h

x

i

+

∑

j

=

1

N

f

r

a

c

w

f

x

j


C′=Nheal+NfracNheal+Nfrac−1{∑Nheali=1wh(xi−x¯′)(xi−x¯′)t+∑Nfracj=1wf(xj−x¯′)(xj−x¯′)t}
C

′

=

N

h

e

a

l

+

N

f

r

a

c

N

h

e

a

l

+

N

f

r

a

c

−

1

{

∑

i

=

1

N

h

e

a

l

w

h

(

x

i

−

x

¯

′

)

(

x

i

−

x

¯

′

)

t

+

∑

j

=

1

N

f

r

a

c

w

f

(

x

j

−

x

¯

′

)

(

x

j

−

x

¯

′

)

t

}


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conditional Model

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

P(F\|L)=N(bcond,Ccond)bcond=μF+∑FL∑−1LL(L−μL)Ccond=∑FF−∑FL∑−1LL∑LF
P

(

F

\|

L

)

=

N

(

b

c

o

n

d

,

C

c

o

n

d

)

b

c

o

n

d

=

μ

F

+

∑

F

L

∑

L

L

−

1

(

L

−

μ

L

)

C

c

o

n

d

=

∑

F

F

−

∑

F

L

∑

L

L

−

1

∑

L

F


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Initialization (dotted line) and real solution (solid line). The six landmarks are also marked.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticSegmentationofVertebraeinLateralXraysUsingaConditionalShapeModel/1_1s20S107663320700308X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## ASM

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

fi(t)=(pi(t)−p¯i)tS−1p,i(pi(t)−p¯i)
f

i

(

t

)

=

(

p

i

(

t

)

−

p

¯

i

)

t

S

p

,

i

−

1

(

p

i

(

t

)

−

p

¯

i

)


where **p** ̶  i is the average of the profiles of length 2 _T  t_ \+ 1 around the points in the training cases, and _S  p,i_ is a diagonal matrix including the (independent) variances of each element in the profile. The function _f  i  (t)_ will just be defined in the interval \[− _T  p  , T  p_ \]. Therefore _T  p_ defines how far from the current point location the search for the contour is performed. If _t  m_ minimizes _f  i  (t)_ , the shift 0.66 _t  m_ is chosen to make the algorithm evolve in a smoother way.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

(PtWs)dx=(PtWsP)db
(

P

t

W

s

)

dx

=

(

P

t

W

s

P

)

db


where _W  S_ is a diagonal matrix with weights that measure the importance of each point in the fitting. The weights depend on the magnitude of the displacement ( ) and on the goodness of the fit:


w′i=12+\|dXi\|21fi(tm)
w

′

i

=

1

2

+

\|

d

X

i

\|

2

1

f

i

(

t

m

)


wi=w′i∑67l=1w′i
w

i

=

w

′

i

∑

l

=

1

67

w

′

i


The idea behind the first term of the weight (2+\|dXi\|2)−1
(

2

+

\|

d

X

i

\|

2

)

−

1
is to prevent the shape model from fitting distant points that might be wrong, as least-squares is not robust against outliers. The second term ( _f  i_ ( _t  m_ ))  −1 gives higher priority to fitting those points that are probably located on the right contour.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

btC−1b=∑ki=1(b2iλi)
b

t

C

−

1

b

=

∑

i

=

1

k

(

b

i

2

λ

i

)


does not hold any longer (even though it would be possible to diagonalize _**C** cond_ and then use this simplification).


b′i+1=bi+db
b

′

i+1

=

b

i

+

db


d=(b′i+1−bcond)tC−1cond(b′i+1−bcond)−−−−−−−−−−−−−−−−−−−−−−−−−−−√
d

=

(

b

′

i

+

1

−

b

c

o

n

d

)

t

C

c

o

n

d

−

1

(

b

′

i

+

1

−

b

c

o

n

d

)


and then


bi+1={b′i+1,bcond+(b′i+1−bcond)(dmax/d),ifd≤dmaxifd>dmax
b

i

+

1

=

{

b

′

i

+

1

,

if

d

≤

d

max

⁡

b

c

o

n

d

+

(

b

′

i

+

1

−

b

c

o

n

d

)

(

d

max

⁡

/

d

)

,

if

d

>

d

max

⁡


Therefore _d  max_ is the parameter that controls how free the algorithm is to fit the contour to the edges in the image. A large value allows the result to move around the principal component space, which can lead to implausible solutions if the edges are not clear in the image. A small value makes the algorithm rely mostly on the model, leading to more conservative solutions, closer to the mean of the distribution. This can prevent the algorithm from finding the correct solution, especially in abnormal cases with fractures or osteophytes, in which the real contour is relatively far from the initialization in the principal component space (  Fig 3 ).

![Figure 3, Influence of maximum allowed Mahalanobis distance on the result. In (a) the shape model is unable to fit the contour to the osteophyte. In (b) , the threshold has been increased by 1.5 and the contour approximates the osteophyte better. The shape model tends to oversmooth the osteophytes.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticSegmentationofVertebraeinLateralXraysUsingaConditionalShapeModel/2_1s20S107663320700308X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Parameter Setting

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 5, Some samples from the leave-one-out experiments. For each pair, the image on the left represents the ground truth, while the one on the right represents the output of the algorithm. (a) Oversmoothing in fractured vertebra (0.85 mm mean point-to-line error), (b) wrong edge captured (0.83 mm), (c) well-segmented fracture (0.51 mm), and (d) typical, normal, well-segmented vertebra (0.33 mm).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticSegmentationofVertebraeinLateralXraysUsingaConditionalShapeModel/3_1s20S107663320700308X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Evaluation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 4, Distance to real contour: histogram and cumulative distribution function.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticSegmentationofVertebraeinLateralXraysUsingaConditionalShapeModel/4_1s20S107663320700308X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Comparison of the Results from This Study and From the Literature


Authors Modality Error Measure Results Zamora et al X-rays Point-to-point average ≤6.4 mm (50% of cases) Smyth et al DXA Point-to-line RMS ≤1.23 in 95% of healthy ≤2.24 mm in 92% of fractures de Bruijne et al X-rays Point-to-line average 1.4 mm (healthy and fractures) Roberts et al DXA Point-to-line average 0.70 mm in healthy, 1.23 mm in fractures Roberts et al X-rays Point-to-line average 0.64 mm in healthy, 1.06 mm in fractures Roberts et al DXA Point-to-line average 0.69 mm in healthy, 0.96 mm in fractures This study X-rays Point-to-line average 0.47 mm in healthy, 0.54 mm in fractures

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 6, Error depending on the point number. The points corresponding to the six landmarks are marked with a star. The distance from the manually placed landmarks to the true contour are marked with crosses.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/SemiautomaticSegmentationofVertebraeinLateralXraysUsingaConditionalShapeModel/5_1s20S107663320700308X.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Genant H.K., Guglielmi G., Jergas M.: Bone densitometry and osteoporosis.1997.SpringerBerlin


- 2\. Black D.M., Palermo L., Nevitt M.C., et. al.: Comparison of methods for defining prevalent vertebral deformities: the Study of Osteoporotic Fractures. J Bone Miner Res 1995; 10: pp. 890-902.


- 3\. Genant H.K., Wu C.Y., van Kuijk C., et. al.: Vertebral fracture assessment using a semiquantitative technique. J Bone Miner Res 1993; 8: pp. 1137-1148.


- 4\. McCloskey E.V., Spector T.D., Eyres K.S., et. al.: The assessment of vertebral deformity: a method for use in population studies and clinical trials. Osteoporos Int 1993; 3: pp. 138-147.


- 5\. Ferrar L., Jiang G., Admas J., et. al.: Identification of vertebral fractures: an update. Osteoporos Int 2005; 16: pp. 717-728.


- 6\. Smyth P., Taylor C., Adams J.: Vertebral shape: automatic measurement with active shape models. Radiology 1999; 211: pp. 571-578.


- 7\. Zamora G., Sari-Sarrafa H., Long R.: Hierarchical segmentation of vertebrae from X-ray images.Sonka M.Fitzpatrick M.Medical Imaging: Image Process.2003.Proc SPIE, SPIE Presspp. 631-642. 5302


- 8\. de Bruijne M., Nielsen M.: Image segmentation by shape particle filtering.Kittler J.Petrou M.Nixon M.ICPR, IEEE Computer Society Press.2004.pp. 722-725. (III)


- 9\. de Bruijne M., Lund M.T., Pettersen P.C., et. al.: Quantitative vertebral morphometry using neighbor-conditional shape models.Larsen R.Nielsen M.Sporring J.2006.pp. 1-8. MICCAI. Volume 4190 of LNCS, Springer


- 10\. Roberts M.G., Cootes T.F., Adams J.E.: Vertebral shape: automatic measurement with dynamically sequenced active appearance models.Duncan J.Gerig G.2005.pp. 733-740. MICAAI. Volume 3750 of LNCS, Springer


- 11\. Roberts M.G., Cootes T.F., Adams J.E.: Automatic segmentation of lumbar vertebrae on digitised radiographs using linked active appearance models. Proc Med Image Understanding Analysis 2006; 1: pp. 120-124.


- 12\. Roberts M.G., Cootes T.F., Adams J.E.: Improving the segmentation accuracy of fractured vertebrae with dynamically sequenced active appearance models.2006.pp. 1-8.


- 13\. Goodall C.R.: Procrustes methods in the statistical analysis of shape. J R Stat Soc 1991; 53: pp. 285-339.


- 14\. Cootes T., Taylor C., Cooper D., et. al.: Active shape models—their training and application. Comput Vis Image Underst 1995; 61: pp. 38-59.


- 15\. Cootes T., Taylor C., Lanitis D.H., et. al.: Building and using flexible models incorporating grey-level information. Proce Fourth Int Conf Computer Vision 1993; pp. 242-246.


- 16\. Long L.R., Antani S., Lee D.J., et. al.: Biomedical information from a national collection of spine x-rays: film to content-based retrieval. Proceedings of the SPIE 2003; 5033: pp. 70-84.


- 17\. Davies R.H., Twining C.J., Cooter T.F., et. al.: A minimum description length approach to statistical shape modeling. IEEE Trans Med Imaging 2002; 21: pp. 525-537.


- 18\. Thodberg H.H.: Minimum description length shape and appearance models. Proc Inf Process Med Imaging 2003; 18: pp. 51-62.