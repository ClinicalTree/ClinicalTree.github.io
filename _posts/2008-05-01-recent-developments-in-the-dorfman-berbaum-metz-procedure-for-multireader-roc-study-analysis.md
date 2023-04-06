---
title: Recent Developments in the Dorfman-Berbaum-Metz Procedure for Multireader ROC Study Analysis
author: [Stephen L. Hillis PhD,Kevin S. Berbaum PhD,Charles E. Metz PhD]
date: 2008-05-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 15, Issue 5 SOURCE CL_S_AcademicRadiologyVolume15Issue5 1}]
tags: [Journals,General Radiology]
---
## Rationale and objectives

The Dorfman-Berbaum-Metz (DBM) method has been one of the most popular methods for analyzing multireader receiver-operating characteristic (ROC) studies since it was proposed in 1992. Despite its popularity, the original procedure has several drawbacks: it is limited to jackknife accuracy estimates, it is substantially conservative, and it is not based on a satisfactory conceptual or theoretical model. Recently, solutions to these problems have been presented in three papers. Our purpose is to summarize and provide an overview of these recent developments.

## Materials and Methods

We present and discuss the recently proposed solutions for the various drawbacks of the original DBM method.

## Results

We compare the solutions in a simulation study and find that they result in improved performance for the DBM procedure. We also compare the solutions using two real data studies and find that the modified DBM procedure that incorporates these solutions yields more significant results and clearer interpretations of the variance component parameters than the original DBM procedure.

## Conclusions

We recommend using the modified DBM procedure that incorporates the recent developments.

There are several different statistical methods for analyzing multireader receiver-operating characteristic (ROC) studies, with the Dorfman-Berbaum-Metz (DBM) method ( ) being one of the most frequently used methods. The DBM method involves an analysis of variance (ANOVA) of pseudovalues computed with the Quenouille-Tukey jackknife ( ). The basic data for the analysis are pseudovalues corresponding to test-reader ROC accuracy measures, such as the area under the ROC curve (AUC), computed by jackknifing cases separately for each test-reader combination. Throughout we use the term _test_ to refer to a diagnostic test, modality, or treatment. A mixed-effects ANOVA is performed on the pseudovalues to test the null hypothesis that the average accuracy of readers is the same for all of the diagnostic tests studied. Accuracy can be characterized using any accuracy measure, such as sensitivity, specificity, area under the ROC curve, partial area under the ROC curve, sensitivity at a fixed specificity, or specificity at a fixed sensitivity. Furthermore, these measures of accuracy can be estimated parametrically, semi-parametrically or nonparametrically; the DBM method accuracy estimates are the corresponding jackknife estimates.

Although the DBM method may be the most frequently used analysis method for multireader ROC studies since it was proposed in 1992, having been used in over 100 published studies ( ), the original procedure has several drawbacks: it requires that the analysis be based on jackknife accuracy estimates, it is substantially conservative, and it is not based on a satisfactory conceptual or theoretical model. Recently, solutions to these problems were presented in three papers ( ). We summarize these recent developments and compare the solutions in a simulation study and in two examples.

## Materials and methods

## Original DBM Method

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Yijk=cˆij−(c−1)ˆij(k)
Y

i

j

k

=

c

^

i

j

−

(

c

−

1

)

^

i

j

(

k

)


where _c_ denotes the number of cases, ˆij
^

i

j
denotes the AUC estimate based on all of the data for the _i_ th test and _j_ th reader, and ˆij(k)
^

i

j

(

k

)
denotes the AUC estimate based on the same data but with data for the _k_ th case removed. Thus, in effect, _Y__ijk_ represents the contribution of the _k_ th case to the accuracy estimate for the _i_ th test and _j_ th reader, ˆij
^

i

j
. Then using the _Y__ijk_ as the data to be evaluated by conventional statistical analysis, the DBM procedure tests for a test effect using a fully crossed three-factor ANOVA with test treated as a fixed factor and reader and case as random factors. A “jackknife estimate” of AUC for the _i_ th test and _j_ th reader is given by the mean of the corresponding pseudovalues:


Y¯¯¯ij⋅=1c∑ck=1Yijk.
Y

¯

ij

⋅

=

1

c

∑

k

=

1

c

Y

i

j

k

.


We refer to ˆij
^

i

j
as the _original_ AUC estimate, Y¯¯¯ij⋅
Y

¯

ij

⋅
as the _jackknife_ AUC estimate, and the _Y__ijk_ as the _raw pseudovalues_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Yijk=μ+τi+Rj+Ck+(τR)ij+(τC)ik+(RC)jk+(τRC)ijk+εijk,
Y

i

j

k

=

μ

+

τ

i

+

R

j

+

C

k

+

(

τ

R

)

i

j

+

(

τ

C

)

i

k

+

(

R

C

)

j

k

+

(

τ

R

C

)

i

j

k

+

ε

i

j

k

,


i=1,…,t;j=1,…,r;k=1,…,c;
i

=

1

,

…

,

t

;

j

=

1

,

…

,

r

;

k

=

1

,

…

,

c

;
where τ _i_ denotes the fixed effect of test _i_ , _R__j_ denotes the random effect of reader _j_ , _C__k_ denotes the random effect of case _k_ , the multiple symbols in parentheses denote interactions, and ε _ijk_ is the error term. The interaction terms are all random effects. The random effects are assumed to be mutually independent and normally distributed with zero means and respective variances σ _R_ 2 , σ _C_ 2 , σ  τ _R_ 2 , σ  τ _C_ 2 , σ _RC_ 2 , σ  τ _RC_ 2 and σ _ε_ 2 . Because there are no replications, σ  τ _RC_ 2 and σ _ε_ 2 are inseparable. The DBM _F_ statistic for testing for a test effect is the conventional mixed-model ANOVA _F_ statistic based on the pseudovalues. Letting MS(T), MS(T\*R), MS(T\*C), and MS(T\*R\*C) denote the mean squares corresponding to the test, test × reader, test × case, and test × reader × case effects, respectively, the _F_ statistic for testing for a test effect for the model is given by


F=MS(T)MS(T\*R)+MS(T\*C)−MS(T\*R\*C)
F

=

MS

(

T

)

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)


Under the null hypothesis of no test effect, _F_ has an approximate _F_ df  1  ,  df  2  distribution, where df  1 = _t_ − 1 and df  2 is the Satterthwaite ( ) degrees of freedom approximation given by


df2=\[MS(T\*R)+MS(T\*C)−MS(T\*R\*C)\]2MS(T\*R)2(t−1)(r−1)+MS(T\*C)2(t−1)(c−1)+MS(T\*R\*C)2(t−1)(r−1)(c−1).
df

2

=

\[

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

\]

2

MS

(

T\*R

)

2

(

t

−

1

)

(

r

−

1

)

+

MS

(

T\*C

)

2

(

t

−

1

)

(

c

−

1

)

+

MS

(

T\*R\*C

)

2

(

t

−

1

)

(

r

−

1

)

(

c

−

1

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σˆ2τR=1c\[MS(T\*R)−MS(T\*R\*C)\]σˆ2τC=1r\[MS(T\*C)−MS(T\*R\*C)\].
σ

^

τ

R

2

=

1

c

\[

MS

(

T\*R

)

−

MS

(

T\*R\*C

)

\]

σ

^

τ

C

2

=

1

r

\[

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

\]

.


Taking into account possible model simplification, the _F_ statistic and ddf for the original DBM method are given by


Forig=⎧⎩⎨⎪⎪⎪⎪⎪⎪⎪⎪⎪⎪MS(T)MS(T\*R)+MS(T\*C)−MS(T\*R\*C)MS(T)/MS(T\*R)MS(T)/MS(T\*C)MS(T)/MS(T\*R\*C)
F

orig

=

{

MS

(

T

)

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

MS

(

T

)

/

MS

(

T\*R

)

MS

(

T

)

/

MS

(

T\*C

)

MS

(

T

)

/

MS

(

T\*R\*C

)


σˆ2τR>0,σˆ2τR>0,σˆ2τR≤0,σˆ2τR≤0,σˆ2τCσˆ2τCσˆ2τCσˆ2τC>0≤0>0≤0
σ

^

τ

R

2

⁢

>

0

,

σ

^

τ

C

2

>

0

σ

^

τ

R

2

⁢

⁢

>

0

,

σ

^

τ

C

2

≤

0

σ

^

τ

R

2

⁢

≤

0

,

σ

^

τ

C

2

>

0

σ

^

τ

R

2

⁢

≤

0

,

σ

^

τ

C

2

≤

0


and


ddforig=⎧⎩⎨⎪⎪⎪⎪⎪⎪⎪⎪⎪⎪Equation4(t−1)(r−1)(t−1)(c−1)(t−1)(r−1)(c−1)σˆ2τR>0,σˆ2τC>0σˆ2τR>0,σˆ2τC≤0σˆ2τR≤0,σˆ2τC>0σˆ2τR≤0,σˆ2τC≤0.
ddf

orig

=

{

Equation

4

σ

^

τ

R

2

>

0

,

σ

^

τ

C

2

>

0

(

t

−

1

)

(

r

−

1

)

σ

^

τ

R

2

>

0

,

σ

^

τ

C

2

≤

0

(

t

−

1

)

(

c

−

1

)

σ

^

τ

R

2

≤

0

,

σ

^

τ

C

2

>

0

(

t

−

1

)

(

r

−

1

)

(

c

−

1

)

σ

^

τ

R

2

≤

0

,

σ

^

τ

C

2

≤

0

.


The numerator degrees of freedom for _F_ in Equation  6 is _t_ − 1\. We refer to this approach, using _F_ orig and ddf  orig , as _original DBM_ . Note that the conditions in Equations  6 and 7 can also be written in terms of the mean squares; eg, σˆ2τR>0,σˆ2τC>0
σ

^

τ

R

2

>

0

,

σ

^

τ

C

2

>

0
is equivalent to MS(T\*R) > MS(T\*R\*C), MS(T\*C) > MS(T\*R\*C).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FDBM=⎧⎩⎨MS(T)MS(T\*R)+MS(T\*C)−MS(T\*R\*C)MS(T)/MS(T\*R)σˆ2τC>0σˆ2τC≤0.
F

DBM

=

{

MS

(

T

)

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

σ

^

τ

C

2

>

0

MS

(

T

)

/

MS

(

T\*R

)

σ

^

τ

C

2

≤

0

.


Because σˆ2τC≤0
σ

^

τ

C

2

≤

0
is equivalent to MS(T\*C) − MS(T\*R\*C) ≤ 0, this _F_ statistic can be succinctly written in the following form that takes model simplification into account:


FDBM=MS(T)MS(T\*R)+max\[MS(T\*C)−MS(T\*R\*C),0\].
F

DBM

=

MS

(

T

)

MS

(

T\*R

)

+

max

⁡

\[

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

,

0

\]

.


The corresponding conventional ANOVA ddf is given by


ddfD={Equation4(t−1)(r−1)σˆ2τC>0σˆ2τC≤0.
ddf

D

=

{

Equation

4

σ

^

τ

C

2

>

0

(

t

−

1

)

(

r

−

1

)

σ

^

τ

C

2

≤

0

.


Thus, new model simplification uses _F_ DBM and ddf  D .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ddfH=⎧⎩⎨⎪⎪{MS(T\*R)+MS(T\*C)−MS(T\*R\*C)}2MS(T\*R)2/\[(t−1)(r−1)\](t−1)(r−1)σˆ2τC>0σˆ2τC≤0
ddf

H

=

{

{

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

}

2

MS

(

T\*R

)

2

/

\[

(

t

−

1

)

(

r

−

1

)

\]

σ

^

τ

C

2

>

0

(

t

−

1

)

(

r

−

1

)

σ

^

τ

C

2

≤

0


Equation  11 can be written more compactly in the form


ddfH={MS(T\*R)+max\[MS(T\*C)−MS(T\*R\*C),0\]}2MS(T\*R)2(t−1)(r−1).
ddf

H

=

{

MS

(

T\*R

)

+

max

⁡

\[

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

,

0

\]

}

2

MS

(

T\*R

)

2

(

t

−

1

)

(

r

−

1

)

.


The quantity ddf  H is derived by assuming that new model simplification is used—that is, it is to be used with _F_ DBM (Eq.  9 ). We refer to this approach, using _F_ DBM and ddf  H , as _new model simplification plus ddf  H_ .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Summary of the Different DBM Approaches


a) Original DBM F  orig  ddf  orig  ConditionMS(T)MS(T\*R)+MS(T\*C)−MS(T\*R\*C)
MS

(

T

)

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)
Equation  4 σˆ2τR>0,σˆ2τC>0
σ

^

τ

R

2

>

0

,

σ

^

τ

C

2

>

0
MS(T)/MS(T\*R) ( _t_ − 1) ( _r_ − 1)σˆ2τR>0,σˆ2τC≤0
σ

^

τ

R

2

>

0

,

σ

^

τ

C

2

≤

0
MS(T)/MS(T\*C) ( _t_ − 1) ( _c_ − 1)σˆ2τR≤0,σˆ2τC>0
σ

^

τ

R

2

≤

0

,

σ

^

τ

C

2

>

0
MS(T)/MS(T\*R\*C) ( _t_ − 1) ( _r_ − 1) ( _c_ − 1)σˆ2τR≤0,σˆ2τC≤0
σ

^

τ

R

2

≤

0

,

σ

^

τ

C

2

≤

0
b) New model simplificationFDBM=MS(T)MS(T\*R)+max\[MS(T\*C)−MS(T\*R\*C),0\]
F

DBM

=

MS

(

T

)

MS

(

T\*R

)

+

max

⁡

\[

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

,

0

\]
ddfD={Equation4σˆ2τC>0(t−1)(r−1)σˆ2τC≤0
ddf

D

=

{

Equation

4

σ

^

τ

C

2

>

0

(

t

−

1

)

(

r

−

1

)

σ

^

τ

C

2

≤

0
c) New model simplification plus ddf  H FDBM=MS(T)MS(T\*R)+max\[MS(T\*C)−MS(T\*R\*C),0\]
F

DBM

=

MS

(

T

)

MS

(

T\*R

)

+

max

⁡

\[

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

,

0

\]
(same as in (b))ddfH={MS(T\*R)+max\[MS(T\*C)−MS(T\*R\*C),0\]}2MS(T\*R)2(t−1)(r−1)
ddf

H

=

{

MS

(

T\*R

)

+

max

⁡

\[

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

,

0

\]

}

2

MS

(

T\*R

)

2

(

t

−

1

)

(

r

−

1

)


These approaches can be used with raw, normalized, or quasi pseudovalues. See  Table 6  for computational formulas for σˆ2τR
σ

^

τR

2
and σˆ2τC
σ

^

τ

C

2
.


Table 2


Relationships Between the DBM _F_ Statistics and Between the DBM Denominator Degrees of Freedom


σ2τR
σ

τ

R

2
σ2τC
σ

τ

C

2
_F_ Relationship Ddf Relationship >0 >0Forig=FDBM
F

orig

=

F

DBM
ddforig=ddfD<ddfH
ddf

orig

=

ddf

D

<

ddf

H
≤0 >0Forig≤FDBM
F

orig

≤

F

DBM
(equality iff σ2τR=0
σ

τ

R

2

=

0
)ddfD<ddforig,ddfD<ddfH
ddf

D

<

ddf

orig

,

ddf

D

<

ddf

H
>0 ≤0Forig=FDBM
F

orig

=

F

DBM
ddforig=ddfD=ddfH
ddf

orig

=

ddf

D

=

ddf

H
≤0 ≤0Forig≤FDBM
F

orig

≤

F

DBM
(equality iff σ2τR=0
σ

τ

R

2

=

0
)ddfD=ddfH<ddforig
ddf

D

=

ddf

H

<

ddf

orig


These relationships are derived in  Appendix A  . Iff: if and only if.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ˆij=μ˜+τ˜i+Rj+(τR)ij+εij,
^

i

j

=

μ

˜

+

τ

˜

i

+

R

j

+

(

τ

R

)

i

j

+

ε

i

j

,


i=1,…,t;j=1,…,r;
i

=

1

,

…

,

t

;

j

=

1

,

…

,

r

;
where ˆij
^

i

j
is the AUC estimate (or other accuracy estimate) for the _i_ th test and _j_ th reader, τ˜i
τ

˜

i
denotes the fixed effect of test _i, R__j_ denotes the random effect of reader _j_ , (τR)ij
(

τ

R

)

i

j
denotes the random test × reader interaction, and ε _ij_ is the error term having mean zero and variance σ˜2ε
σ

˜

ε

2
. The random effects _R__j_ and (τR)ij
(

τ

R

)

i

j
are assumed independent and normally distributed with zero means and variances σ˜2R
σ

˜

R

2
and σ˜2τR
σ

˜

τ

R

2
, respectively, and are assumed independent of the ε _ij_ . We use the tilde symbol “∼” to distinguish OR model parameters from analogous DBM model parameters. Because the same cases are read by each reader using each test, the error terms are not assumed to be independent. Instead, equi-covariance of the errors between readers and tests is assumed, resulting in three possible covariances given by


Cov⎛⎝⎜εij,εi′j′⎞⎠⎟=⎧⎩⎨⎪⎪Cov1Cov2Cov3i≠i′,j=j′(different test, same reader)i=i′,j≠j′(same test, different reader)i≠i′,j≠j′(different test, different reader).
Cov

(

ε

i

j

,

ε

i

′

j

′

)

=

{

Cov

1

i

≠

i

′

,

j

=

j

′

(

different test, same reader

)

Cov

2

i

=

i

′

,

j

≠

j

′

(

same test, different reader

)

Cov

3

i

≠

i

′

,

j

≠

j

′

(

different test, different reader

)

.


Obuchowski and Rockette ( ) suggest the following ordering: Cov  1 ≥ Cov  2 ≥ Cov  3 . Conditional on the reader and test × reader effects (that is, treating readers as fixed), it follows from Equation  13 that Cov  1 , Cov  2 , and Cov  3 are also the corresponding covariances of the AUC estimates; for example, Cov  2 is the covariance between the AUCs for two fixed readers using the same test, whereas Cov  3 is the covariance between the AUCs for two fixed readers using different modalities.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FOR=MS(T)ˆijMS(T\*R)ˆij+max\[r(Covˆ2−Covˆ3),0\],
F

OR

=

MS

(

T

)

^

i

j

MS

(

T\*R

)

^

i

j

+

max

⁡

\[

r

(

Cov

^

2

−

Cov

^

3

)

,

0

\]

,


where MS(T)ˆij
MS

(

T

)

^

i

j
and MS(T\*R)ˆij
MS

(

T\*R

)

^

i

j
are the test and test × reader mean squares corresponding to the OR model, and where Covˆ2
Cov

^

2
and Covˆ3
Cov

^

3
are covariance estimates; the subscript “ ˆij
^

i

j
” is used here to indicate that the mean squares are computed from the AUCs rather than the pseudovalues. The quantities Covˆ2
Cov

^

2
and Covˆ3
Cov

^

3
are estimated by averaging corresponding covariance estimates for pairs of AUCs, estimated using covariance estimation methods that treat readers as fixed. For example,


Covˆ2=2tr(r−1)∑ti=1∑j<j'Covˆ(ˆij,ˆij'),
Cov

^

2

=

2

t

r

(

r

−

1

)

∑

i

=

1

t

∑

j

<

j

′

Cov

^

(

^

i

j

,

^

i

j

′

)

,


where Covˆ(ˆij,ˆij')
Cov

^

(

^

i

j

,

^

i

j

′

)
is an estimate of the covariance between AUCs for fixed readers _j_ and _j_ ′ using test _i_ , estimated using a fixed reader method such as bootstrapping or jackknifing.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ddfH={MS(T\*R)+max\[r(Covˆ2−Covˆ3),0\]}2MS(T\*R)2(t−1)(r−1).
ddf

H

=

{

MS

(

T\*R

)

+

max

⁡

\[

r

(

Cov

^

2

−

Cov

^

3

)

,

0

\]

}

2

MS

(

T\*R

)

2

(

t

−

1

)

(

r

−

1

)

.


Under any of the conditions described above that result in _F_ DBM = _F_ OR , the same value for ddf  H is obtained using either Equation  12 or 16 , and there is a one-to-one correspondence between the DBM and OR computed quantities, as shown in  Table 4 .

Table 3


Conditions That Result in _F_ DBM  = _F_ OR  as Defined by Equations  9 and 15

(1) Normalized pseudovalues are used with DBM and σ˜ˆ2ε
σ

˜

^

ε

2
, Covˆ1
Cov

^

1
, Covˆ2
Cov

^

2
and Covˆ3
Cov

^

3
are jackknife variance and covariance estimates._or_ (2) Raw pseudovalues are used with DBM, σ˜ˆ2ε
σ

˜

^

ε

2
, Covˆ1
Cov

^

1
, Covˆ2
Cov

^

2
and Covˆ3
Cov

^

3
are jackknife variance and covariance estimates, and ˆij
^

i

j
are jackknife accuracy estimates._or_ (3) Quasi pseudovalues are used with DBM.

Note: Any one of the above conditions results in _F_ DBM  = _F_ OR  .


Table 4


Relationship Between DBM and OR Computed Quantities


OR Computed Quantity Equivalent Function of DBM Computed QuantitiesMS(T)ˆij
MS(T)

^

i

j
=1cMS(T)
=

1

c

MS(T)
MS(R)ˆij
MS(R)

^

i

j
=1cMS(R)
=

1

c

MS(R)
MS(T\*R)ˆij
MS(T\*R)

^

i

j
=1cMS(T\*R)
=

1

c

MS(T\*R)
σ˜ˆ2ε
σ

˜

^

ε

2
=1trc\[MS(C)+(t−1)MS(T\*C)+(r−1)MS(R\*C)+(t−1)(r−1)MS(T\*R\*C)\]
=

1

t

r

c

\[

MS(C)

+

(

t

−

1

)

MS(T\*C)

+

(

r

−

1

)

MS(R\*C)

+

(

t

−

1

)

(

r

−

1

)

MS(T\*R\*C)\]
Cov1ˆ
Cov

1

^
=1trc{MS(C)−MS(T\*C)+(r−1)\[MS(R\*C)−MS(T\*R\*C)\]}
=

1

t

r

c

{MS(C)

−

MS(T\*C)

+

(

r

−

1

)

\[MS(R\*C)

−

MS(T\*R\*C)\]}
Cov2ˆ
Cov

2

^
=1trc{MS(C)−MS(R\*C)+(t−1)\[MS(T\*C)−MS(T\*R\*C)\]}
=

1

t

r

c

{

MS(C)

−

MS(R\*C)

+

(

t

−

1

)

\[

MS(T\*C)

−

MS(T\*R\*C)\]}
Cov3ˆ
Cov

3

^
=1trc\[MS(C)−MS(T\*C)−MS(R\*C)+MS(T\*R\*C)\]
=

1

t

r

c

\[

MS(C)

−

MS(T\*C)

−

MS(R\*C)

+

MS(T\*R\*C)\]
DBM Computed Quantity Equivalent Function of OR Computed Quantities MS(T)=cMS(T)ˆij
=

c

MS(T)

^

i

j
MS(R)=cMS(R)ˆij
=

c

MS(R)

^

i

j
MS(T\*R)=cMS(T\*R)ˆij
=

c

MS(T\*R)

^

i

j
MS(C)=c\[σ˜ˆ2ε−(t−1)Covˆ1+(r−1)Covˆ2+(t−1)(r−1)Covˆ3)\]
=

c

\[

σ

˜

^

ε

2

−

(

t

−

1

)

Cov

^

1

+

(

r

−

1

)

Cov

^

2

+

(

t

−

1

)

(

r

−

1

)

Cov

^

3

)

\]
MS(T\*C)=c\[σ˜ˆ2ε−Covˆ1+(r−1)(Covˆ2−Covˆ3)\]
=

c

\[

σ

˜

^

ε

2

−

Cov

^

1

+

(

r

−

1

)

(

Cov

^

2

−

Cov

^

3

)

\]
MS(R\*C)=c\[σ˜ˆ2ε+(t−1)Covˆ1−Covˆ2−(t−1)Covˆ3)\]
=

c

\[

σ

˜

^

ε

2

+

(

t

−

1

)

Cov

^

1

−

Cov

^

2

−

(

t

−

1

)

Cov

^

3

)

\]
MS(T\*R\*C)=c\[σ˜ˆ2ε−Covˆ1−Covˆ2+Covˆ3\]
=

c

\[

σ

˜

^

ε

2

−

Cov

^

1

−

Cov

^

2

+

Cov

^

3

\]


These relationships assume one of the three conditions given in  Table 3  .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Relationship Between DBM and OR Model Parameters


OR Model Parameter Equivalent Function of DBM Model Parametersμ˜
μ

˜
= μτ˜i
τ

˜

i
= τ _i_σ˜2R
σ

˜

R

2
= σ _R_ 2 σ˜2τR
σ

˜

τ

R

2
= σ  τ _R_ 2 σ˜2ε
σ

˜

ε

2
=(σ2C+σ2τC+σ2RC+σ2τRC+σ2ε)/c
=

(

σ

C

2

+

σ

τ

C

2

+

σ

R

C

2

+

σ

τ

R

C

2

+

σ

ε

2

)

/

c
Cov  1 =(σ2C+σ2RC)/c
=

(

σ

C

2

+

σ

R

C

2

)

/

c
Cov  2 =(σ2C+σ2τc)/c
=

(

σ

C

2

+

σ

τ

c

2

)

/

c
Cov  3 =σ2C/c
=

σ

C

2

/

c
DBM Model Parameter Equivalent Function of OR Model Parameters μ=μ˜
=

μ

˜
τ _i_=τ˜i
=

τ

˜

i
σ _R_ 2 =σ˜2R
=

σ

˜

R

2
σ  τ _R_ 2 =σ˜2τR
=

σ

˜

τ

R

2
σ _C_ 2 =cCov3
=

c

Cov

3
σ  τ _C_ 2 =c(Cov2−Cov3)
=

c

(

Cov

2

−

Cov

3

)
σ _RC_ 2 =c(Cov1−Cov3)
=

c

(

Cov

1

−

Cov

3

)
σ  τ _RC_ 2  \+ σ  ε  2 =c(σ˜2ε−Cov1−Cov2+Cov3)
=

c

(

σ

˜

ε

2

−

Cov

1

−

Cov

2

+

Cov

3

)


These relationships assume that the constraints for the OR model parameters are those implied by the DBM model: σ2ε≥Cov1+Cov2−Cov3
σ

ε

2

≥

Cov

1

+

Cov

2

−

Cov

3
, Cov1≥Cov3
Cov

1

≥

Cov

3
, Cov2≥Cov3
Cov

2

≥

Cov

3
, and Cov3≥0
Cov

3

≥

0
. They also assume the same linear constraint for the τi
τ

i
(eg, Στi=0
Σ

τ

i

=

0
) for both models and that either (1) normalized or quasi pseudovalues are used; or (2) if raw pseudovalues are used, then the OR model outcome is the jackknife accuracy estimate.


Adapted and reprinted, with permission, from Hillis et al. ( ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 6


ANOVA Estimates for DBM Variance Components


DBM Model Parameter Estimate σ _R_ 2 1tc\[MS(R)−MS(T\*R)−MS(R\*C)+MS(T\*R\*C)\]
1

t

c

\[

MS

(

R

)

−

MS

(

T\*R

)

−

MS

(

R\*C

)

+

MS

(

T\*R\*C

)

\]
σ _C_ 2 1tr\[MS(C)−MS(T\*C)−MS(R\*C)+MS(T\*R\*C)\]
1

t

r

\[

MS

(

C

)

−

MS

(

T\*C

)

−

MS

(

R\*C

)

+

MS

(

T\*R\*C

)

\]
σ  τ _R_ 2 1c\[MS(T\*R)−MS(T\*R\*C)\]
1

c

\[

MS

(

T\*R

)

−

MS

(

T\*R\*C

)

\]
σ  τ _C_ 2 1r\[MS(T\*C)−MS(T\*R\*C)\]
1

r

\[

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

\]
σ _RC_ 2 1t\[MS(R\*C)−MS(T\*R\*C)\]
1

t

\[

MS

(

R\*C

)

−

MS

(

T\*R\*C

)

\]
σ  τ _RC_ 2  \+ σ  ε  2  MS(T\*R\*C)

These estimates, except for the last, can be negative.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

## Simulation Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 7


Semi-parametric Estimation Results of the Simulation Study for Discrete Rating Data


Type I Error Rates Approach Pseudovalues_N_ Mean Min Max Range SD CI Width Mean Original Raw 144 0.036 0.009 0.063 0.054 0.0124 0.196 Normalized 144 0.036 0.011 0.062 0.052 0.0111 0.188 New Raw 144 0.042 0.011 0.070 0.060 0.0123 4.05E+121 Normalized 144 0.043 0.017 0.067 0.050 0.0108 2.74E+121 New plus ddf  H  Raw 144 0.049 0.016 0.075 0.060 0.0124 0.192 Normalized 144 0.051 0.025 0.077 0.052 0.0105 0.184

Original, original DBM; New, new model simplification; New plus ddf  H  , new model simplification plus ddf  H  ; Min, minimum; Max, maximum; SD, standard deviation; CI width, width of a 95% confidence interval for the difference of the AUC estimates.


Table 8


Nonparametric Estimation Results of the Simulation Study for Discrete Rating Data


Type I Error Rates Approach_N_ Mean Min Max Range SD CI Width Mean Original 144 0.041 0.014 0.069 0.055 0.0098 0.177 New 144 0.046 0.024 0.072 0.049 0.0100 4.55E+121 New plus ddf  H  144 0.053 0.029 0.079 0.050 0.0097 0.174

No distinction is made between raw and normalized pseudovalues since the trapezoid estimate is the same for either type of pseudovalues. Original, original DBM; new, new model simplification; new plus ddf  H  , new model simplification plus ddf  H  ; min, minimum; max, maximum; SD, standard deviation; CI width, width of a 95% confidence interval for the difference of the AUC estimates.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 9


DBM Procedure Analyses for Van Dyke et al. (20) Data for Semi-parametric and Corresponding Jackknife AUC Estimates


Test 1 (CINE) 2 (Spin Echo) Reader (j)ˆ1j
^

1

j
(semiparametric)_Y_ 1 _j_ (jackknife)ˆ2j
^

2

j
(semiparametric)_Y_ 2 _j._ (jackknife) 1 0.933 0.947 0.951 0.950 2 0.890 0.909 0.935 0.933 3 0.929 0.929 0.928 0.928 4 0.970 0.981 1.000 0.999 5 0.833 0.836 0.945 0.943ˆ1⋅=.911
^

1

⋅

=

.911
Y1⋅⋅=.920
Y

1

⋅

⋅

=

.920
ˆ2⋅=.952
^

2

⋅

=

.952
Y2⋅⋅=.951
Y

2

⋅

⋅

=

.951


ANOVA Table Source ddf Raw Pseudovalue Mean Square Normalized Pseudovalue Mean Square T 1 0.264166 0.468996 R 4 0.315637 0.297310 C 113 0.392538 0.392538 T × R 4 0.112560 0.108062 T × C 113 0.143095 0.143095 R × C 452 0.098771 0.098771 T × R × C 452 0.072068 0.072068

T, tests; R, readers; C, cases.


Raw pseudovalues results:


a) Original DBM: _F_ orig  = 1.439, ddf  orig  = 10.03, _p_ = 0.2579


b) New model simplification: _F_ DBM  = 1.439, ddf  D  = 10.03, _p_ = 0.2579


c) New model simplification plus ddf  H  : _F_ DBM  = 1.439, ddf  H  = 10.64, _p_ = 0.2563


Normalized pseudovalues results:


a) Original DBM: _F_ orig  = 2.619, ddf  orig  = 10.31, _p_ = 0.1358


b) New model simplification: _F_ DBM  = 2.619, ddf  D  = 10.31, _p_ = 0.1358


c) New model simplification plus ddf  H  : _F_ DBM  = 2.619, ddf  H  = 10.99, _p_ = 0.1339


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 10


Variance Component Estimates for Van Dyke et al. ( ) Data Based on Normalized Pseudovalues


DBM OR Variance Component Estimate Variance Component Estimate σ _R_ 2  0.000713σ˜2R
σ

˜

R

2
0.000713 σ  τ _R_ 2  0.000316σ˜2τR
σ

˜

τ

R

2
0.000316 σ _C_ 2  0.022274 Cov  1  0.000313 σ  τ _C_ 2  0.014205 Cov  2  0.000320 σ _RC_ 2  0.013351 Cov  3  0.000195 σ  τ _RC_ 2  \+ σ  ε  2  0.072068σ˜2ε
σ

˜

ε

2
0.001069

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 11


DBM Procedure Analyses for Franken et al. ( ) Data for ANOVA Table


Source ddf Raw Pseudovalue Mean Square Normalized Pseudovalue Mean Square T 1 0.063574 0.066606 R 3 0.088782 0.097686 C 99 0.547734 0.547734 T×R 3 0.007781 0.007494 T×C 99 0.078071 0.078071 R×C 297 0.127582 0.127582 T×R×C 297 0.083643 0.083643

T, tests; R, readers; C, cases.


Raw pseudovalues results:


a) Original DBM: _F_ orig  = 0.760, ddf  orig  = 297, _p_ = 0.3840


b) New model simplification: _F_ DBM  = 8.171, ddf  D  = 3, _p_ = 0.0647


c) New model simplification plus ddf  H  : _F_ DBM  = 8.171, ddf  H  = 3, _p_ = 0.0647


Normalized pseudovalues results:


a) Original DBM: _F_ orig  = 0.796, ddf  orig  = 297, _p_ = 0.3729


b) New model simplification: _F_ DBM  = 8.888, ddf  D  = 3, _p_ = 0.0585


c) New model simplification plus ddf  H  : _F_ DBM  = 8.888, ddf  H  = 3, _p_ = 0.0585


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ddfD=(t−1)(r−1)=ddfH.
ddf

D

=

(

t

−

1

)

(

r

−

1

)

=

ddf

H

.


Thus, ddf  D < ddf  H if σˆ2τC>0
σ

^

τ

C

2

>

0
and ddf  D = ddf  H if σˆ2τC≤0
σ

^

τ

C

2

≤

0
. These relationships hold regardless of the value of σˆ2τR
σ

^

τ

R

2
. Now we consider each of the four situations separately for the other relationships.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Forig=FDBM=MS(T)MS(T\*R)+MS(T\*C)−MS(T\*R\*C)
F

orig

=

F

DBM

=

MS

(

T

)

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)


ddforig=ddfD=\[MS(T\*R)+MS(T\*C)−MS(T\*R\*C)\]2MS(T\*R)2(t−1)(r−1)+MS(T\*C)2(t−1)(c−1)+MS(T\*R\*C)(t−1)(r−1)(c−1).
ddf

orig

=

ddf

D

=

\[

MS

(

T\*R

)

+

MS

(

T\*C

)

−

MS

(

T\*R\*C

)

\]

2

MS

(

T\*R

)

2

(

t

−

1

)

(

r

−

1

)

+

MS

(

T\*C

)

2

(

t

−

1

)

(

c

−

1

)

+

MS

(

T\*R\*C

)

(

t

−

1

)

(

r

−

1

)

(

c

−

1

)

.


_Situation 2:_σˆ2τR≤0,σˆ2τC>0
σ

^

τ

R

2

≤

0

,

σ

^

τ

C

2

>

0
. From Equation  5 , we have cσˆ2τR=MS(T\*R)−MS(T\*R\*C)
c

σ

^

τ

R

2

=

MS

(

T\*R

)

−

MS

(

T\*R\*C

)
. Hence
![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633208X00042/S1076633208000068/fx2.gif?Signature=ZnWcKWVjvIzDJv7kDn6JJAfCwiu5iv07tPeT3gXvZrmdz67P%7EbxbUi1PlCFHkKYfR3CIPvXUxHWfonYem8gL3tvn8BoIamfkZiVQYh%7EumfOmIZRpwLdm9mh03%7EVnGrmYyzGgOOHgCHK-ohuAc%7E3KpXNGE5MANZz35BoFuLC-dNo_&Expires=1669525249&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ) with Forig=FDBM
F

o

r

i

g

=

F

D

B

M
if and only if σˆ2τR=0
σ

^

τ

R

2

=

0
. Also,
![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633208X00042/S1076633208000068/fx3.gif?Signature=bbdlZTEqv9obdAkZGH7E%7EFOpQIc1jp8kPi36Wu32lb4%7ESHKGtx%7EWPTzvEQXLuGi8kGedUSBUYMftjfDpM0PIrl2K6DtuZ49pa0aoPYMsB7Z6STe3Qw5f54MKYxY2j7SIub9Fo8CffUKqSJazYze51p2wimkSeg1XIzyuQLIIViY_&Expires=1669525249&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ) That is, ddfD<ddforig
ddf

D

<

ddf

orig
. In the proof we have utilized the relationship MS(T\*R)−MS(T\*R\*C)+MS(T\*C)>0
MS

(

T\*R

)

−

MS

(

T\*R\*C

)

+

MS

(

T\*C

)

>

0
, because from Equation  5 we have MS(T\*C)−MS(T\*R\*C)=rσˆ2τC>0
MS

(

T\*C

)

−

MS

(

T\*R\*C

)

=

r

σ

^

τ

C

2

>

0
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Forig=FDBM=MS(T)MS(T\*R)
F

orig

=

F

DBM

=

MS

(

T

)

MS

(

T\*R

)


ddforig=ddfD=(t−1)(r−1)
ddf

orig

=

ddf

D

=

(

t

−

1

)

(

r

−

1

)


_Situation 4:_σˆ2τR≤0,σˆ2τC≤0
σ

^

τ

R

2

≤

0

,

σ

^

τ

C

2

≤

0
. From Equation  5 , it follows that MS(T\*R)≤MS(T\*R\*C)
MS

(

T\*R

)

≤

MS

(

T\*R\*C

)
, with equality if and only if σˆ2τR=0
σ

^

τ

R

2

=

0
. Thus,


Forig=MS(T)MS(T\*R\*C)≤MS(T)MS(T\*R)=FDBM,
F

orig

=

MS

(

T

)

MS

(

T\*R\*C

)

≤

MS

(

T

)

MS

(

T\*R

)

=

F

DBM

,


with equality if and only if σˆ2τR=0
σ

^

τ

R

2

=

0
. Also,


ddforig=(t−1)(r−1)(c−1)>(t−1)(r−1)=ddfDBM.
ddf

orig

=

(

t

−

1

)

(

r

−

1

)

(

c

−

1

)

>

(

t

−

1

)

(

r

−

1

)

=

ddf

DBM

.


Note that we require the assumption that _c_ \> 2 for this last relationship.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix B

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Corr(AUCˆij,AUCˆi'j')=Cov(AUCˆij,AUCˆi'j')Var(AUCˆij)Var(AUCˆi'j')√
Corr

(

AUC

^

i

j

,

AUC

^

i

′

j

′

)

=

Cov

(

AUC

^

i

j

,

AUC

^

i

′

j

′

)

Var

(

AUC

^

i

j

)

Var

(

AUC

^

i

′

j

′

)


where Cov(AUCˆij,AUCˆi′j′)
Cov

(

AUC

^

i

j

,

AUC

^

i

′

j

′

)
is the covariance. To find the covariance and variances, we write AUCˆij
AUC

^

i

j
and AUCˆi′j′
AUC

^

i

′

j

′
as functions of random and fixed effects using the OR model (Eq. ). It follows from well known statistical properties that the variance for each AUC estimate is the sum of the OR model variance components corresponding to the random effects, and Cov(AUCˆij,AUCˆi′j′)
Cov

(

AUC

^

i

j

,

AUC

^

i

′

j

′

)
is the sum of the variance components corresponding to the reader or test × reader random effects that the AUC estimates have in common (ie, they have the same subscript values for each AUC estimate), plus the covariance between the error terms.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ρBR=Corr(AUCˆij,AUCˆij')=Cov(AUCˆij,AUCˆij')Var(AUCˆij)Var(AUCˆij')√
ρ

B

R

=

Corr

(

AUC

^

i

j

,

AUC

^

ij

′

)

=

Cov

(

AUC

^

i

j

,

AUC

^

ij

′

)

Var

(

AUC

^

i

j

)

Var

(

AUC

^

ij

′

)


where _j_ ≠ _j_ ′. From Equation  13 , with AUCˆij
AUC

^

i

j
taking the place of ˆij
^

i

j
, we have


AUCˆij=μ˜+τ˜i+Rj+(τR)ij+εijAUCˆij′=μ˜+τ˜i+Rj′+(τR)ij′+εij′.
AUC

^

i

j

=

μ

˜

+

τ

˜

i

+

R

j

+

(

τ

R

)

i

j

+

ε

i

j

AUC

^

i

j

′

=

μ

˜

+

τ

˜

i

+

R

j

′

+

(

τ

R

)

i

j

′

+

ε

i

j

′

.


Each AUC estimate has the same variance, equal to the sum of all of the variance components corresponding to the random effects; that is,


Var(AUCijˆ)=Var(AUCij'ˆ)=σ˜2R+σ˜2τR+σ˜2e.
Var

(

AUC

i

j

^

)

=

Var

(

AUC

ij

′

^

)

=

σ

˜

R

2

+

σ

˜

τ

R

2

+

σ

˜

e

2

.


Examination of Equation  18 shows that the AUCs do not have any reader or test × reader random effects in common because _j_ ≠ _j_ ′. Thus, the covariance is equal to Cov  2 , the covariance between the error terms for different readers using the same test:


Cov(AUCijˆ,AUCij'ˆ)=Cov2.
Cov

(

AUC

i

j

^

,

AUC

ij

′

^

)

=

Cov

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ρBR=Cov2σ˜2R+σ˜2τR+σ˜2e.
ρ

BR

=

Cov

2

σ

˜

R

2

+

σ

˜

τ

R

2

+

σ

˜

e

2

.


Now we derive the between-reader correlation between AUC estimates for two different readers using the same test, but this time _treating readers as fixed_ . In this case, the correlation is a measure of the association between the deviation of one reader's AUC estimate from that reader's underlying AUC, due to case variation and reader error, with the deviation of the other reader's AUC estimate from that reader's underlying AUC. In contrast, ρBR
ρ

B

R
is a measure of association between deviations of _randomly chosen_ readers' AUC estimates from the _reader population_ AUC.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ρBR\|readers=Corr(AUCˆij,AUCˆij'∣∣Ri(τR)ij,(τR)ij')=Cov(AUCˆij,AUCˆij'∣∣Ri(τR)ij,(τR)ij')Var(AUCˆij∣∣Ri,(τR)ij,(τR)ij')Var(AUCˆij'∣∣Ri,(τR)ij,(τR)ij')√
ρ

BR

\|

readers

=

Corr

(

AUC

^

ij

,

AUC

^

ij

′

\|

R

i

(

τ

R

)

i

j

,

(

τ

R

)

ij

′

)

=

Cov

(

AUC

^

i

j

,

AUC

^

ij

′

\|

R

i

(

τ

R

)

i

j

,

(

τ

R

)

ij

′

)

Var

(

AUC

^

i

j

\|

R

i

,

(

τR

)

i

j

,

(

τ

R

)

ij

′

)

Var

(

AUC

^

i

j

′

\|

R

i

,

(

τ

R

)

i

j

,

(

τ

R

)

i

j

′

)


When we condition on the reader and test × reader random effects, the only random effects in Equations  18 are the error terms. Thus, each AUC has the same variance, equal to σ˜2ε
σ

˜

ε

2
:


Var(AUCˆij∣∣∣Ri,(τR)ij,(τR)ij')= Var(AUCˆij'∣∣∣Ri,(τR)ij,(τR)ij')=σ˜2ε.
Var

(

AUC

^

i

j

\|

R

i

,

(

τ

R

)

i

j

,

(

τ

R

)

i

j

′

)

= Var

(

AUC

^

ij

′

\|

R

i

,

(

τ

R

)

i

j

,

(

τ

R

)

i

j

′

)

=

σ

˜

ε

2

.


Similarly, the covariance is equal to Cov  2 , the covariance between the error terms:


Cov(AUCˆij,AUCˆij'∣∣Ri,(τR)ij,(τR)ij')=Cov2
Cov

(

A

U

C

^

i

j

,

A

U

C

^

ij

′

\|

R

i

,

(

τ

R

)

i

j

,

(

τ

R

)

ij

′

)

=

Cov

2


It follows from Equations  20, 21, and 22 that


ρBR\|readers=Cov2σ˜2ε.
ρ

B

R

\|

r

e

a

d

e

r

s

=

Cov

2

σ

˜

ε

2

.


These correlations can be written in terms of the DBM model parameters using the relationships in  Table 5 . For example, since Cov2=(σ2C+σ2τC)
Cov

2

=

(

σ

C

2

+

σ

τ

C

2

)
and σ˜2ε=σ2C+σ2τC+σ2RC+σ2tRC+σ2ε
σ

˜

ε

2

=

σ

C

2

+

σ

τ

C

2

+

σ

R

C

2

+

σ

t

R

C

2

+

σ

ε

2
, where σ _C_ 2 , σ  τ _C_ 2 , σ _RC_ 2 , σ  τ _RC_ 2 and σ  ε 2 denote the DBM model variance components, then ρBR\|readers=(σ2C+σ2τC)/(σ2C+σ2τC+σ2RC+σ2τRC+σ2ε)
ρ

B

R

\|

r

e

a

d

e

r

s

=

(

σ

C

2

+

σ

τ

C

2

)

/

(

σ

C

2

+

σ

τ

C

2

+

σ

R

C

2

+

σ

τ

R

C

2

+

σ

ε

2

)
in terms of the DBM variance components. This last expression is also given in Equation  4 of Roe and Metz ( ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Dorfman D.D., Berbaum K.S., Metz C.E.: Receiver operating characteristic rating analysis: Generalization to the population of readers and patients with the jackknife method. Investig Radiol 1992; 27: pp. 723-731.


- 2\. Roe C.A., Metz C.E.: Dorfman-Berbaum-Metz method for statistical analysis of multireader, multimodality receiver operating characteristic data: Validation with computer simulation. Acad Radiol 1997; 4: pp. 298-303.


- 3\. Dorfman D.D., Berbaum K.S., Lenth R.V., Chen Y.F., Donaghy B.A.: Monte Carlo validation of a multireader method for receiver operating characteristic discrete rating data: Factorial experimental design. Acad Radiol 1998; 5: pp. 591-602.


- 4\. Quenoille M.H.: Approximate tests of correlation in time series. J R Stat Soc Ser B 1949; 11: pp. 68-84.


- 5\. Quenoille M.H.: Notes on bias in estimation. Biometrika 1956; 43: pp. 353-360.


- 6\. Tukey J.W.: Bias and confidence in not quite large samples. Ann Math Stat 1958; 29: pp. 614. (abstract)


- 7\. Berbaum K.S.: God, like the devil, is in the details. Acad Radiol 2006; 13: pp. 1311-1316.


- 8\. Hillis S.L., Obuchowski N.A., Schartz K.M., Berbaum K.S.: A comparison of the Dorfman-Berbaum-Metz and Obuchowski-Rockette Methods for receiver operating characteristic (ROC) data. Stat Med 2005; 24: pp. 1579-1607.


- 9\. Hillis S.L., Berbaum K.S.: Monte Carlo validation of the Dorfman-Berbaum-Metz method using normalized pseudovalues and less data-based model simplification. Acad Radiol 2005; 12: pp. 1534-1542.


- 10\. Hillis S.L.: A comparison of denominator degrees of freedom methods for multiple observer ROC analysis. Stat Med 2007; 26: pp. 596-619.


- 11\. Satterthwaite F.E.: Synthesis of variance. Psychometrika 1941; 6: pp. 309-316.


- 12\. Satterthwaite F.E.: An approximate distribution of estimates of variance components. Biometric Bull 1946; 2: pp. 110-114.


- 13\. Hanley J.A., Mcneil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 14\. Hillis S.L., Berbaum K.S.: Power estimation for the Dorfman-Berbaum-Metz method. Acad Radiol 2004; 11: pp. 1260-1273.


- 15\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of diagnostic accuracy for multiple readers and multiple tests: An ANOVA approach with dependent observations. Commun Stat Simul Comput 1995; 24: pp. 285-308.


- 16\. Obuchowski N.A.: Multireader, multimodality receiver operating characteristic curve studies: Hypothesis testing and sample size estimation using an analysis of variance approach with dependent observations. Acad Radiol 1995; 2: pp. S22-S29.


- 17\. Dorfman D.D., Alf E.: Maximum likelihood estimation of parameters of signal-detection theory and determination of confidence intervals: Rating method data. J Math Psychol 1969; 6: pp. 487-496.


- 18\. Dorfman D.D.: RSCORE II.Swets J.A.Pickett R.M.Evaluation of Diagnostic Systems: Methods From Signal Detection Theory.1982.Academic PressSan Diego, CA:pp. 212-232.


- 19\.  The SAS System for Windows, Version 9.1.2002.SAS InstituteCary, NC


- 20\.  Van Dyke CW, White RD, Obuchowski NA, Geisinger MA, Lorig RJ, Meziane MA. Cine MRI in the diagnosis of thoracic aortic dissection. Presented at the 79th RSNA Meeting, Chicago, IL, 1993.


- 21\. Franken E.A., Berbaum K.S., Marley S.M., Smith W.L., Sato Y., Kao S.C., Milam S.G.: Evaluation of a digital workstation for interpreting neonatal examinations: A receiver operating characteristic study. Invest Radiol 1992; 27: pp. 732-737.


- 22\. Berbaum K.S., Schartz K.M., Pesce L.L., Hillis S.L.: DBM MRMC 2.1 (computer software).2006. http://perception.radiology.uiowa.edu

- 23\. Berbaum K.S., Metz C.E., Pesce L.L., Schartz K.M.: DBM MRMC 2.1 User's Guide (software manual).2006. http://perception.radiology.uiowa.edu

- 24\. Hillis S.L., Schartz K.M., Pesce L.L., Berbaum K.S.: DBM MRMC 2.1 for SAS (computer software).2007. http://perception.radiology.uiowa.edu