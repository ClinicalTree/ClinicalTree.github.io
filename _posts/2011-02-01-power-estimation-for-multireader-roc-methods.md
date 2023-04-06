---
title: Power Estimation for Multireader ROC Methods
author: [Stephen L. Hillis PhD,Nancy A. Obuchowski PhD,Kevin S. Berbaum PhD]
date: 2011-02-01 00:00:00 +0700 +07
categories: [{Academic Radiology, Volume 18, Issue 2 SOURCE CL_S_AcademicRadiologyVolume18Issue2 1}]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We describe a step-by-step procedure for estimating power and sample size for planned multireader receiver operating characteristic (ROC) studies that will be analyzed using either the Dorfman-Berbaum-Metz (DBM) or Obuchowski-Rockette (OR) method. This procedure updates previous approaches by incorporating recent methodological developments and unifies the approaches by allowing inputs to be conjectured parameter values or outputs from either a DBM or OR pilot-study analysis.

## Materials and Methods

Power computations are described in a step-by-step procedure and the theoretical basis for the procedure is described. Updates include using the currently recommended denominator degrees of freedom, accounting for different pilot and planned study normal-to-abnormal case ratios, and a new method for computing the OR test-by-reader variance component.

## Results

Using a real dataset we illustrate how to compute the power for two planned studies, one having the same normal-to-abnormal case ratio as the pilot study and the other having a different ratio. In a simulation study, we show that the proposed procedure gives mean power estimates close to the true power.

## Conclusions

Application of the updated procedure is straightforward. It is important that pilot data be comparable to the planned study with respect to the modalities, reader expertise, and case selection. Variability of the power estimates warrants further investigation.

Receiver operating characteristic (ROC) curve analysis is a well-established method for evaluating and comparing the performance of diagnostic tests for radiological imaging studies. Throughout we assume that rating data have been collected using the study design where multiple readers (typically radiologists) assign disease-severity or disease-likelihood ratings, using one or more tests, to the same images using either a discrete (eg, 1, 2, 3, 4, 5) or a quasi-continuous (eg, 0–100%) scale. From these ratings, ROC curves and corresponding accuracy estimates are computed for each reader and each test to assess how well a test performs or to compare the performance of tests. In such studies, there is variability between cases and between readers. Thus it is important that results generalize to both the corresponding case and reader populations; methods that accomplish this goal are commonly referred to as multireader multicase methods.

Two popular multireader multicase methods are those proposed by Dorfman, Berbaum, and Metz (DBM) and by Obuchowski and Rockette (OR) . For the OR method, power computation using conjectured parameter estimates is discussed by Obuchowski and Zhou et al ; for the DBM method power computation based on pilot-study estimates or conjectured parameter values is discussed by Hillis and Berbaum . Since the publication of these articles, it has been shown that both the DBM and OR methods can be improved by using a common denominator degrees of freedom, ddf  H , for the _F_ statistic for testing for equality of tests. When both methods use ddf  H , the DBM method can be viewed as an implementation of the OR method using jackknife covariance estimates, with both methods yielding the same conclusions. Furthermore, previous work shows that if the OR method is not based on jackknife covariance estimates, then _quasi pseudovalues_ can be generated that give the same results when analyzed by the DBM method. Thus we can consider the DBM and OR procedures to be equivalent. These developments in the DBM procedure and its relationship with the OR procedure are summarized elsewhere .

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Materials and methods

## Design and Notation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The DBM Procedure

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FDBM=MS(T)YMS(T∗R)Y+H\[MS(T∗C)Y−MS(T∗R∗C)Y\]
F

DBM

=

MS

(

T

)

Y

MS

(

T

∗

R

)

Y

+

H

\[

MS

(

T

∗

C

)

Y

−

MS

(

T

∗

R

∗

C

)

Y

\]


where the function _H_ (⋅) is defined by


H(x)={x0ifx>0ifx≤0
H

(

x

)

=

{

x

if

x

>

0

0

if

x

≤

0


Equation  1 is recommended by Hillis et al and differs slightly from the original DBM formulation in that less data-based model reduction is allowed. Hillis and Berbaum used Equation  1 in their power algorithm; although they used raw instead of normalized pseudovalues, the use of normalized pseudovalues does not alter their algorithm. Hillis showed that the DBM method has improved performance if the following denominator degrees of freedom for _F_ DBM is used:


ddfH={MS(T∗R)Y+H\[MS(T∗C)Y−MS(T∗R∗C)Y\]}2\[MS(T∗R)Y\]2/\[(t−1)(r−1)\]
dd

f

H

=

{

MS

(

T

∗

R

)

Y

+

H

\[

MS

(

T

∗

C

)

Y

−

MS

(

T

∗

R

∗

C

)

Y

\]

}

2

\[

MS

(

T

∗

R

)

Y

\]

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


The updated power procedure that we will present incorporates Equation  2 , which was not used by Hillis and Berbaum because it had not yet been proposed. We note that since it was proposed in 2007 by Hillis , ddf  H has been incorporated into freely available DBM analysis software .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The OR Procedure

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ˆij=μ+τi+Rj+(TR)ij+ϵij
ˆ

i

j

=

μ

+

τ

i

+

R

j

+

(

T

R

)

i

j

+

ϵ

i

j


_i_ = 1,…, _t_ , _j_ = 1,…, _r_ , where τi
τ

i
denotes the fixed effect of test _i_ , _R  j_ denotes the random effect of reader _j_ , ( _TR_ ) _ij_ denotes the random test × reader interaction, and _ϵ  ij_ is the error term. The _R  j_ and ( _TR_ ) _ij_ are assumed to be mutually independent and normally distributed with zero means and respective variances σ2R
σ

R

2
, reflecting differences in reader ability, and σ2TR
σ

T

R

2
, reflecting test-by-reader interaction. The _ϵ  ij_ are assumed to be normally distributed with zero mean and variance σ2ϵ
σ

ϵ

2
, which represents variability attributable to cases and within-reader variability that describes how a reader interprets the same image in different ways on different occasions. The _ϵ  ij_ are independent of the _R  j_ and ( _TR_ ) _ij_ . Equicovariance of the errors between readers and tests is assumed, resulting in three possible covariances:


Cov(ϵij,ϵi′j′)=⎧⎩⎨⎪⎪⎪⎪⎪⎪⎪⎪⎪⎪⎪⎪Cov1i≠i′,j=j′(different tests,samereader)Cov2i≠i′,j=j′(same test,differentreaders)Cov3i≠i′,j=j′(different tests, different readers)
Cov

(

ϵ

i

j

,

ϵ

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

different tests

,

same

reader

)

Cov

2

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

same test

,

different

readers

)

Cov

3

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

different tests, different readers

)


It follows from model that σ2ϵ
σ

ϵ

2
, Cov  1 , Cov  2 , and Cov  3 are also the variance and corresponding covariances of the AUC estimates, conditional on the reader and test × reader effects. Based on clinical considerations Obuchowski and Rockette suggest the following ordering for the covariances:


Cov1≥Cov2≥Cov3≥0.
Co

v

1

≥

Co

v

2

≥

Co

v

3

≥

0.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

FOR=MS(T)ˆijMS(T∗R)ˆij+H\[r(Covˆ2−Covˆ3)\]
F

OR

=

MS

(

T

)

ˆ

i

j

MS

(

T

∗

R

)

ˆ

i

j

+

H

\[

r

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]


where MS(T)ˆij
MS

(

T

)

ˆ

i

j
and MS (T∗R)ˆij
(

T

∗

R

)

ˆ

i

j
are the two-way ANOVA test and test-by-reader mean squares; these mean squares are based on the AUC outcomes, in contrast to the DBM mean squares that are based on the case-level pseudovalues. The quantities Covˆ2
Cov

ˆ

2
and Covˆ3
Cov

ˆ

3
denote estimates for Cov  2 and Cov  3 , respectively. Note that Equation  5 incorporates the constraint given by Equation  4 by setting Covˆ2−Covˆ3
Cov

ˆ

2

−

Cov

ˆ

3
to zero if it is negative.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

df2={E\[MS(T∗R)ˆij\]+r(Cov2−Cov3)}2\[E\[MS(T∗R)ˆij\]\]2(t−1)(r−1)
d

f

2

=

{

E

\[

MS

(

T

∗

R

)

ˆ

i

j

\]

+

r

(

Co

v

2

−

Co

v

3

)

}

2

\[

E

\[

MS

(

T

∗

R

)

ˆ

i

j

\]

\]

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


and suggests estimating df  2 by


ddfH={MS(T∗R)ˆij+H\[r(Covˆ2−Covˆ3)\]}2\[MS(T∗R)ˆij\]2(t−1)(r−1)
dd

f

H

=

{

MS

(

T

∗

R

)

ˆ

i

j

+

H

\[

r

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]

}

2

\[

MS

(

T

∗

R

)

ˆ

i

j

\]

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


Note that the estimate ddf  H replaces the parameters in df  2 by estimates; in particular, the expected test × reader mean square, E\[MS(T∗R)ˆij\]
E

\[

MS

(

T

∗

R

)

ˆ

i

j

\]
, is replaced by the observed mean square, MS (T∗R)ˆij
(

T

∗

R

)

ˆ

i

j
, and _r_ (Cov  2 − Cov  3 ) is replaced by H\[r(Covˆ2−Covˆ3)\]
H

\[

r

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]
, which incorporates the model covariance constraints given by Equation  4 . He also shows that ddf  H results in improved performance compared to the denominator degrees of freedom, ddf  0 originally proposed by Obuchowski and Rockette . A 100(1− _α_ )% confidence interval for _i_ − _i_ ′ , _i_ ≠ _i_ ′, is given by ˆi⋅−ˆi'⋅±ta/2;ddfH2rMSdenOR−−−−−−−−−−√
ˆ

i

⋅

−

ˆ

i

′

⋅

±

t

a

/

2

;

dd

f

H

2

r

MSde

n

OR
, where MSden  OR is the denominator of the right-hand-side of Equation  5 .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δ=r∑ti=1(i−⋅)2σ2TR+σ2ϵ−Cov1+(r−1)(Cov2−Cov3)
Δ

=

r

∑

i

=

1

t

(

i

−

⋅

)

2

σ

T

R

2

+

σ

ϵ

2

−

Co

v

1

+

(

r

−

1

)

(

Co

v

2

−

Co

v

3

)


and i=μ+τi
i

=

μ

+

τ

i
is the expected accuracy measure for test _i_ . This result is stated by Obuchowski and a detailed proof is provided elsewhere .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## OR and DBM Relationships

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


OR Outputs in Terms of DBM Mean Squares from a Pilot Study


Adapted and reprinted, with permission, from Hillis et al .


OR Output Equivalent Function of DBM Mean SquaresMS(T)ˆij
MS

(

T

)

ˆ

i

j
=1c∗MS(T)
=

1

c

∗

MS

(

T

)
MS(R)ˆij
MS

(

R

)

ˆ

i

j
=1c∗MS(T)
=

1

c

∗

MS

(

T

)
MS(T∗R)ˆij
MS

(

T

∗

R

)

ˆ

i

j
=1c∗MS(T∗R)
=

1

c

∗

MS

(

T

∗

R

)
σˆ2ϵ
σ

ˆ

ϵ

2
=1t∗r∗c∗\[MS(C)−(t∗−1)MS(T∗C)+(r∗−1)MS(R∗C)+(t∗−1)(r∗−1)MS(T∗R∗C)\]
=

1

t

∗

r

∗

c

∗

\[

MS

(

C

)

−

(

t

∗

−

1

)

MS

(

T

∗

C

)

+

(

r

∗

−

1

)

MS

(

R

∗

C

)

+

(

t

∗

−

1

)

(

r

∗

−

1

)

MS

(

T

∗

R

∗

C

)

\]
Covˆ1
Cov

ˆ

1
=1t∗r∗c∗\[MS(C)−MS(T∗C)+(r∗−1)MS(R∗C)−MS(T∗R∗C)\]
=

1

t

∗

r

∗

c

∗

\[

MS

(

C

)

−

MS

(

T

∗

C

)

+

(

r

∗

−

1

)

MS

(

R

∗

C

)

−

MS

(

T

∗

R

∗

C

)

\]
Covˆ2
Cov

ˆ

2
=1t∗r∗c∗\[MS(C)−MS(R∗C)+(t∗−1)MS(T∗C)−MS(T∗R∗C)\]
=

1

t

∗

r

∗

c

∗

\[

MS

(

C

)

−

MS

(

R

∗

C

)

+

(

t

∗

−

1

)

MS

(

T

∗

C

)

−

MS

(

T

∗

R

∗

C

)

\]
Covˆ3
Cov

ˆ

3
=1t∗r∗c∗\[MS(C)−MS(T∗C)−MS(R∗C)+MS(T∗R∗C)\]
=

1

t

∗

r

∗

c

∗

\[

MS

(

C

)

−

MS

(

T

∗

C

)

−

MS

(

R

∗

C

)

+

MS

(

T

∗

R

∗

C

)

\]


DBM, Dorfman-Berbaum-Metz; OR, Obuchowski-Rockette.


The number of tests, readers, and cases in the study are denoted by _t_ ∗  , _r_ ∗  , and _c_ ∗  , respectively.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## OR method in terms of correlations and the σ2c  σ    c    2  **,**σ2w  σ    w    2   parameterization

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Updated and Unified OR/DBM Power Computation Procedure

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


  - a.
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

    σˆ2TR=MS¯¯¯¯¯(T∗R)−σˆ2ϵ+Covˆ1+H(Covˆ2−Covˆ3)
     σ

     ˆ

     T

     R

     2

     =

     MS

     ¯

     (

     T

     ∗

     R

     )

     −

     σ

     ˆ

     ϵ

     2

     +

     Cov

     ˆ

     1

     +

     H

     (

     Cov

     ˆ

     2

     −

     Cov

     ˆ

     3

     )

     If σˆ2TR<0
     σ

     ˆ

     T

     R

     2

     <

     0
      then set σˆ2TR
     σ

     ˆ

     T

     R

     2
      equal to zero or to a positive conjectured value for the remaining steps (see _What to do if Section_ ) for further discussion of this point.
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - b.
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

  - c.
    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)




    Table 2





    Relationships Between OR and DBM Variance Component and Covariance Parameters





    Adapted and reprinted, with permission, from Hillis et al ( ,  Table III  ).




    OR Parameter  Equivalent Function of DBM Variance Components σ2R
    σ

    R

    2
    =σ2R
    =

    σ

    R

    2
    σ2TR
    σ

    T

    R

    2
    =σ2TR
    =

    σ

    T

    R

    2
    σ2ϵ
    σ

    ϵ

    2
    =(σ2C+σ2TC+σ2RC+σ2TRC+σ2ϵ)/c
    =

    (

    σ

    C

    2

    +

    σ

    T

    C

    2

    +

    σ

    R

    C

    2

    +

    σ

    T

    R

    C

    2

    +

    σ

    ϵ

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
    Cov  2 =(σ2C+σ2TC)/c
    =

    (

    σ

    C

    2

    +

    σ

    T

    C

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





    DBM, Dorfman-Berbaum-Metz; OR, Obuchowski-Rockette.





    Notes: _c_ is the number of cases; see reference for definitions of the DBM variance components.




    [Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δˆ=r2d2σˆ2TR+c∗c{σˆ2ϵ−Covˆ1+(r−1)H(Covˆ2−Covˆ3)}
Δ

ˆ

=

r

2

d

2

σ

ˆ

TR

2

+

c

∗

c

{

σ

ˆ

ϵ

2

−

Cov

ˆ

1

+

(

r

−

1

)

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

}

and

dfˆ2=\[σˆ2TR+c∗c(σˆ2ϵ−Covˆ1+(r−1)H\[Covˆ2−Covˆ3\])\]2{σˆ2TR+(c∗c)\[σˆ2ϵ−Covˆ1−H(Covˆ2−Covˆ3)\]}2r−1
df

ˆ

2

=

\[

σ

ˆ

T

R

2

+

c

∗

c

(

σ

ˆ

ϵ

2

−

Cov

ˆ

1

+

(

r

−

1

)

H

\[

Cov

ˆ

2

−

Cov

ˆ

3

\]

)

\]

2

{

σ

ˆ

T

R

2

+

(

c

∗

c

)

\[

σ

ˆ

ϵ

2

−

Cov

ˆ

1

−

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]

}

2

r

−

1

Here Δˆ
Δ

ˆ
    is the estimated noncentrality parameter and dfˆ2
df

ˆ

2
    is the estimated denominator degrees of freedom for the distribution of _F_ OR  (Eq.  5  ). These formulas were derived for _t_ = 2 tests. It is easy to show that dfˆ2
df

ˆ

2
    has the same value as ddf  H  (Eq.  7  ) for _c_ = _c_ ∗  .
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

power=Pr(F1,dfˆ2;Δˆ>F1−α;1,dfˆ2)
power

=

Pr

(

F

1

,

df

ˆ

2

;

Δ

ˆ

>

F

1

−

α

;

1

,

df

ˆ

2

)

treating dfˆ2
df

ˆ

2
    and Δˆ
Δ

ˆ
    as fixed.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Other Considerations

## Accounting for different pilot and planned study normal-to-abnormal case ratios

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

ηij=μ+τi+Rj+TRij
η

i

j

=

μ

+

τ

i

+

R

j

+

T

R

i

j


From Equation  3 , it follows that for given test _i_ and fixed reader _j_ , ηij=E(ˆij)
η

i

j

=

E

(

ˆ

i

j

)
; this is the expected or mean AUC across the population of cases. Thus _η  ij_ is the latent or true AUC for test _i_ and reader _j_ , which can be loosely interpreted as the AUC that would result if reader _j_ read a very large number of cases. It follows that σ2TR
σ

T

R

2
can be interpreted as the interaction variance component for the _η  ij_ , and hence the value of this parameter does not depend on the ratio or numbers of normals and abnormals in the sample. We note that alternatively estimating σ2TR
σ

T

R

2
using Equation  9 from each of the 10 generated datasets would not be valid, because Equation  9 assumes that both readers and cases are random units but our generated datasets only treated cases as random.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Comparison with earlier results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## What to do if σˆ2TR<0  σ    ˆ    T    R    2    <    0

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

(ηij−ηi'j)−(ηij'−ηi'j')∼N(0,4σ2TR)
(

η

i

j

−

η

i

′

j

)

−

(

η

i

j

′

−

η

i

′

j

′

)

∼

N

(

0

,

4

σ

T

R

2

)


For example, if reader 1 has latent AUC values of 0.95 and 0.90 for tests 1 and 2, respectively, and reader 2 has corresponding latent AUC values of 0.93 and 0.91, then _η_ 11 − _η_ 21 − ( _η_ 12 − _η_ 22 ) = (0.95 - 0.90) − (0.93 - 0.91) = 0.05 − 0.02 = 0.03. The quantity _η  ij_ − _η  i_ ′ _j_ − ( _η  ij_ ′ − _η  i_ ′ _j_ ′ ) can be interpreted as the difference of the two intrareader latent AUC differences for randomly selected readers _j_ and _j_ ′. Thus σ2TR
σ

T

R

2
is equal to one-fourth of the variance of the difference of the intrareader latent AUC differences for two randomly chosen readers.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

l≥(1.96)var(ηij−ηi'j−ηij'+ηi'j')−−−−−−−−−−−−−−−−−−−−√=(1.96)(2σTR)
l

≥

(

1.96

)

var

(

η

i

j

−

η

i

′

j

−

η

i

j

′

+

η

i

′

j

′

)

=

(

1.96

)

(

2

σ

T

R

)


ie,


σTR≤l3.92andσ2TR≤(l3.92)2
σ

TR

≤

l

3.92

and

σ

TR

2

≤

(

l

3.92

)

2


For _l_ = .06, we have σTR≤.063.92=.01531
σ

T

R

≤

.06

3.92

=

.01531
, or equivalently σ2TR≤.015312=.00023
σ

T

R

2

≤

.01531

2

=

.00023
. Thus if σˆ2TR<0
σ

ˆ

T

R

2

<

0
, it would be reasonable to set σˆ2TR=.00023
σ

ˆ

T

R

2

=

.00023
in step 2 if _l_ = .06 seems like a reasonable 95% bound.  Table 3 presents values of σ2TR
σ

T

R

2
corresponding to various values of _l_ .

Table 3


Relationship between OR Test-by-reader Interaction Variance Component σ2TR
σ

T

R

2
and 95% Probability Upper Bound _l_ on the Absolute Difference of Intrareader Latent AUCs Differences  ∗

_l_σ2TR
σ

T

R

2
0.01 0.00001 0.02 0.00003 0.03 0.00006 0.04 0.00010 0.05 0.00016 0.06 0.00023 0.07 0.00032 0.08 0.00042 0.09 0.00053 0.1 0.00065

AUC, area under the curve; OR, Obuchowski-Rockette.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## One-sided tests

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Example: Spin echo versus Cine MRI for Detection of Aortic Dissection

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Situation 1: Similar normal-to-abnormal ratios

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 4


Obuchowski-Rockette Analysis of Van Dyke et al Data


(a) PROPROC AUC Estimates for Cine and Spin-echo MRI Test Reader Cine Spin-echo 1 .934 .952 2 .891 .926 3 .908 .930 4 .977 1.000 5 .841 .943 Mean: .910 .950 Notes: H  0  = test AUCs are equal; _t_ = 2 tests; _r_ = 5 readers.

(b) ANOVA Table Based on PROPROC AUCs Source df Mean Square T 1 0.004003382 R 4 0.002834705 T∗R 4 0.000622731

(c) Jackknife Covariance Matrix Corresponding to PROPROC AUC Estimates C1 C2 C3 C4 C5 S1 S2 S3 S4 S5 C1 9.54 C2 7.47 20.35 C3 8.73 6.64 61.78 C4 2.24 2.65 1.70 1.48 C5 5.48 12.26 3.11 2.00 18.07 S1 3.93 4.26 3.67 0.37 2.62 5.19 S2 3.28 5.50 3.26 1.07 4.70 2.46 4.94 S3 4.74 5.59 5.53 1.23 4.40 5.03 3.95 8.03 S4 0.00 0.00 0.00 0.00 0.00 0.00 0.00 0.00 0.00 S5 0.85 0.35 3.82 0.07 2.63 0.40 2.98 2.19 0.00 10.00 Notes: C1-C5 = readers 1–5, cine; S1-S5 = readers 1–5, spin echo. Values have been multiplied by 10  4  .

(d) Covariance Estimatesσˆ2ϵ=.001393652
σ

ˆ

ϵ

2

=

.001393652
; Covˆ1=.000351859
Cov

ˆ

1

=

.000351859
; Covˆ2=.000346505
Cov

ˆ

2

=

.000346505
; Covˆ3=.000221453
Cov

ˆ

3

=

.000221453


(e) Correlation Estimates ( ri=Covˆi/σˆ2ϵ
r

i

=

Cov

ˆ

i

/

σ

ˆ

ϵ

2
)_r_ 1  = 0.25247; _r_ 2  = 0.24863; _r_ 3  = 0.15890

(f)F=MS(T)MS(T∗R)+H\[r(Covˆ2−Covˆ3),0\]=.004003382.000622731+5(.000346505−.000221453)=3.21
F

=

MS

(

T

)

MS

(

T

∗

R

)

+

H

\[

r

(

Cov

ˆ

2

−

Cov

ˆ

3

)

,

0

\]

=

.004003382

.000622731

+

5

(

.000346505

−

.000221453

)

=

3.21


(g)ddfH={MS(T∗R)+H\[r(Covˆ2−Covˆ3),0\]}2\[MS(T∗R)\]2/\[(t−1)(r−1)\]=16.065
ddf

H

=

{

MS

(

T

∗

R

)

+

H

\[

r

(

Cov

ˆ

2

−

Cov

ˆ

3

)

,

0

\]

}

2

\[

MS

(

T

∗

R

)

\]

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

=

16.065


(h)_P_ value = Pr( _F_ 1;16.065  >3.21) = .092

(i)95%CIfor2−1:.04±t.025;16.06525MSdenOR−−−−−−−−−√=(−0.0073,0.0921)
95

%

CI

for

2

−

1

:

.04

±

t

.

025

;

16.065

2

5

MSde

n

O

R

=

(

−

0.0073

,

0.0921

)


ANOVA, analysis of variance; AUC, area under the curve; MRI, magnetic resonance imaging.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 1.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 2.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 3.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

dfˆ2={σˆ2TR+c∗c\[σˆ2ϵ−Covˆ1+(r−1)H(Covˆ2−Covˆ3)\]}2{σˆ2TR+(c∗c)\[σˆ2ϵ−Covˆ1−H(Covˆ2−Covˆ3)\]}2r−1={0+114240\[0.001394−0.000352\]+\[4(0.000347−0.000221)\]}2{0+114240\[0.001394−0.000352−(0.000347−0.000221)\]}24=30.6
df

ˆ

2

=

{

σ

ˆ

T

R

2

+

c

∗

c

\[

σ

ˆ

ϵ

2

−

Cov

ˆ

1

+

(

r

−

1

)

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]

}

2

{

σ

ˆ

T

R

2

+

(

c

∗

c

)

\[

σ

ˆ

ϵ

2

−

Cov

ˆ

1

−

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]

}

2

r

−

1

=

{

0

+

114

240

\[

0.001394

−

0.000352

\]

+

\[

4

(

0.000347

−

0.000221

)

\]

}

2

{

0

+

114

240

\[

0.001394

−

0.000352

−

(

0.000347

−

0.000221

)

\]

}

2

4

=

30.6


Δˆ=r2d2σˆ2TR+c∗c\[σˆ2ϵ−Covˆ1+(r−1)H(Covˆ2−Covˆ3)\]=82(.05)20+114240\[0.001394−0.000352\]+\[4(0.000347−0.000221)\]=10.98
Δ

ˆ

=

r

2

d

2

σ

ˆ

T

R

2

+

c

∗

c

\[

σ

ˆ

ϵ

2

−

Cov

ˆ

1

+

(

r

−

1

)

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]

=

8

2

(

.05

)

2

0

+

114

240

\[

0.001394

−

0.000352

\]

+

\[

4

(

0.000347

−

0.000221

)

\]

=

10.98


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

- 4.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

power=Pr(F1,dfˆ2;Δˆ>F1−α;1,dfˆ2)=Pr(F1,30.6;10.98>F.95;1,30.6)=.89
power

=

Pr

(

F

1

,

df

ˆ

2

;

Δ

ˆ

>

F

1

−

α

;

1

,

df

ˆ

2

)

=

Pr

(

F

1

,

30.6

;

10.98

>

F

.95

;

1

,

30.6

)

=

.89

Recall that this estimate was computed assuming no test × reader interaction, because we have set σˆ2TR=0
σ

ˆ

T

R

2

=

0
    . A more conservative approach would be, for example, to set σ2TR=.0001
σ

T

R

2

=

.0001
    corresponding to the belief that a 95% upper bound on the absolute difference of two intrareader AUC differences is given by _l_ = 0.04. Using this approach, the power is 0.86.
[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 5


Combinations of Cases and Readers having 0.80 Power to Detect a 0.05 AUC Difference Between Spin-echo and Cine MRI Based on the Van Dyke et al Data


Normal/abnormal Ratio = 69/45 = 1.53 Normal/abnormal Ratio = 1σˆ2TR=0
σ

ˆ

T

R

2

=

0
σˆ2TR=.0001
σ

ˆ

T

R

2

=

.0001
σˆ2TR=0
σ

ˆ

T

R

2

=

0
σˆ2TR=.0001
σ

ˆ

T

R

2

=

.0001
Readers Cases Power Cases Power Cases Power Cases Power 3 559 0.800 1898 0.800 374 0.800 1282 0.800 4 343 0.800 491 0.800 229 0.800 328 0.800 5 266 0.801 330 0.801 177 0.801 220 0.801 6 225 0.800 263 0.800 150 0.801 176 0.802 7 200 0.800 227 0.801 133 0.800 151 0.801 8 183 0.800 203 0.801 122 0.801 135 0.801 9 171 0.801 187 0.802 114 0.802 124 0.801 10 162 0.802 174 0.800 108 0.803 116 0.802 11 154 0.800 165 0.801 103 0.803 110 0.803 12 148 0.800 158 0.802 99 0.803 105 0.803 13 143 0.800 151 0.800 95 0.801 101 0.803 14 139 0.801 146 0.800 93 0.804 97 0.801 15 136 0.802 142 0.801 90 0.801 94 0.800

AUC, area under the curve; MRI, magnetic resonance imaging.


The pilot-study estimate of σˆ2TR
σ

ˆ

T

R

2
was negative. The left-hand-side results are for a planned study that has the same normal-to-abnormal ratio as the pilot study; the right-hand-side results are for a planned study that has equal numbers of normal and abnormal cases.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Situation 2: Different normal-to-abnormal ratios

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 6


OR Variance Component Estimates from 10 Randomly Generated Van Dyke Datasets having 69 Normal and 69 Abnormal Images


Sampleσˆ2ϵ
σ

ˆ

ϵ

2
Covˆ1
Cov

ˆ

1
Covˆ2
Cov

ˆ

2
Covˆ3
Cov

ˆ

3
1 0.000512 0.000204 0.000181 0.000125 2 0.000416 0.000019 0.000112 0.000073 3 0.001173 0.000118 0.000169 0.000138 4 0.001121 0.000078 0.000129 0.000074 5 0.000545 0.000153 0.000242 0.000106 6 0.000629 0.000316 0.000224 0.000189 7 0.000634 0.000155 0.000225 0.000107 8 0.001117 0.000135 0.000204 0.000116 9 0.000608 0.000176 0.000222 0.000145 10 0.000470 0.000130 0.000136 0.000089 Mean 0.000723 0.000148 0.000184 0.000116

OR, Obuchowski-Rockette.


Each dataset contains 69 resampled abnormal images combined with the original 69 normal images.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Power computation based on DBM analysis

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 7


DBM Analysis of Van Dyke et al Data


(a) ANOVA Table Based on Normalized Jackknife AUC Pseudovalues Source df SS MS T 1 0.45638557 0.45638557 R 4 1.29262569 0.32315642 T∗R 4 0.28396550 0.07099138 C 113 51.75139760 0.45797697 T∗C 113 19.86406163 0.17578816 R∗C 452 60.67694615 0.13424103 T∗R∗C 452 47.23783039 0.10450847 C, case; MS, mean square; R, reader; SS, sum of squares; T, test. Notes: H  0  = test AUCs are equal; _t_ = 2 tests; _r_ = 5 readers. (b) F=MS(T)MS(T∗R)+H\[MS(T∗C)−MS(T∗R∗C),0\]=0.456385570.07099138+0.17578816−0.10450847=3.21
F

=

MS

(

T

)

MS

(

T

∗

R

)

+

H

\[

MS

(

T

∗

C

)

−

MS

(

T

∗

R

∗

C

)

,

0

\]

=

0.45638557

0.07099138

+

0.17578816

−

0.10450847

=

3.21
(c) ddf  H ={MS(T∗R)+H\[MS(T∗C)−MS(T∗R∗C)\]}2\[MS(T∗R)\]2/\[(t−1)(r−1)\]=16.065
=

{

MS

(

T

∗

R

)

+

H

\[

MS

(

T

∗

C

)

−

MS

(

T

∗

R

∗

C

)

\]

}

2

\[

MS

(

T

∗

R

)

\]

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

=

16.065
(d) _P_ value = Pr( _F_ 4;16.065  >3.21) = .092

ANOVA, analysis of variance; AUC, area under the curve; DBM, Dorfman-Berbaum-Metz.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Simulation Study

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 8


Simulation Study Results: Mean Parameter Estimates Based on the 4000 Simulated Samples for Each Combination of Reader and Case Sample Sizes


Mean Parameter Estimates_r__c_ AUC  2 −AUC1
−

AU

C

1
Powerσ2TR
σ

T

R

2
σ2ϵ
σ

ϵ

2
Cov  1  Cov  2  Cov  3 _r_ 1 _r_ 2 _r_ 3  3 50 0.066 0.189 1.330 2.350 0.873 1.116 0.475 0.358 0.461 0.189 3 100 0.066 0.276 1.282 1.123 0.427 0.549 0.234 0.372 0.480 0.200 3 200 0.066 0.343 1.294 0.547 0.210 0.270 0.115 0.378 0.488 0.204 5 50 0.065 0.256 1.251 2.335 0.861 1.106 0.469 0.357 0.461 0.190 5 100 0.066 0.407 1.257 1.126 0.426 0.551 0.233 0.372 0.482 0.200 5 200 0.066 0.525 1.250 0.549 0.211 0.271 0.115 0.381 0.490 0.206 10 50 0.066 0.355 1.196 2.349 0.867 1.112 0.470 0.360 0.462 0.191 10 100 0.066 0.571 1.260 1.119 0.423 0.543 0.229 0.373 0.479 0.200 10 200 0.066 0.781 1.257 0.550 0.212 0.272 0.115 0.382 0.491 0.207

Notes: AUC  2  –AUC  1  is the mean difference of the test 1 and test 2 empirical AUC estimates; _r_ = number of readers; _c_ = number of cases; σ2TR
σ

T

R

2
, σ2ϵ
σ

ϵ

2
, Cov  1  , Cov  2  , and Cov  3  values are multiplied by 1000.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 9


Simulation Results: Power Estimates for 10 Readers, 200 Cases, and Effect Size (AUC Difference) = .066


Power Estimated From_r__c_ Actual Power Reliable Estimates Sample Estimates P25 P75 P75 −P25 3 50 0.781 0.729 0.773 0.639 0.955 .316 3 100 0.781 0.742 0.776 0.658 0.935 .277 3 200 0.781 0.745 0.772 0.653 0.918 .265 5 50 0.781 0.742 0.768 0.635 0.930 .295 5 100 0.781 0.744 0.766 0.655 0.906 .251 5 200 0.781 0.751 0.767 0.666 0.892 .226 10 50 0.781 0.749 0.765 0.649 0.903 .254 10 100 0.781 0.747 0.760 0.662 0.868 .206 10 200 0.781 0.749 0.760 0.675 0.856 .181 Mean 0.744 0.767 .252

AUC, area under the curve.


The “Actual power” estimate 0.781 is from the last line of  Table 8  ; the “Reliable estimates” column contains power estimates based on the mean parameter estimates from  Table 8  ; the “Sample estimates” column contains the mean of the sample power estimates across the 4000 simulated samples; P25 and P75 are the 25th and 75th percentiles of the sample power estimates; _r_ = number of readers; _c_ = number of cases.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discussion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgment

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Supplementary data

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Appendix

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix A

## Power derivation for the or procedure

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Δ=r2(1−2)2σ2TR+σ2ϵ−Cov1+(r−1)(Cov2−Cov3)
Δ

=

r

2

(

1

−

2

)

2

σ

T

R

2

+

σ

ϵ

2

−

Co

v

1

+

(

r

−

1

)

(

Co

v

2

−

Co

v

3

)


and


df2=\[E(MS(T∗R))+r(Cov2−Cov3)\]2\[E(MS(T∗R))\]2r−1
d

f

2

=

\[

E

(

MS

(

T

∗

R

)

)

+

r

(

Co

v

2

−

Co

v

3

)

\]

2

\[

E

(

MS

(

T

∗

R

)

)

\]

2

r

−

1


It is shown in reference (8) that


E(MS(T∗R))=σ2TR+σ2ϵ−Cov1−(Cov2−Cov3)
E

(

MS

(

T

∗

R

)

)

=

σ

T

R

2

+

σ

ϵ

2

−

Co

v

1

−

(

Co

v

2

−

Co

v

3

)


It follows from Equations  13-14 that


σ2TR=E(MS(T∗R))−σ2ϵ+Cov1+(Cov2−Cov3)
σ

T

R

2

=

E

(

MS

(

T

∗

R

)

)

−

σ

ϵ

2

+

Co

v

1

+

(

Co

v

2

−

Co

v

3

)


and


df2=\[σ2TR+σ2ϵ−Cov1+(r−1)(Cov2−Cov3)\]2\[σ2TR+σ2ϵ−Cov1−(Cov2−Cov3)\]2r−1
d

f

2

=

\[

σ

T

R

2

+

σ

ϵ

2

−

Co

v

1

+

(

r

−

1

)

(

Co

v

2

−

Co

v

3

)

\]

2

\[

σ

T

R

2

+

σ

ϵ

2

−

Co

v

1

−

(

Co

v

2

−

Co

v

3

)

\]

2

r

−

1


Let _r_ ∗ and _c_ ∗ denote reader and case pilot-study sample sizes from which covariance parameter estimates are obtained and _r_ and _c_ the corresponding sample sizes for which we want to compute power. Based on Equations  12, 15, and 16 we use the following estimates that incorporate the constraint Cov ≥ Cov  3 :


σˆ2TR=MS(T∗R)−σ2ϵ+Covˆ1+H(Covˆ2−Covˆ3)
σ

ˆ

T

R

2

=

MS

(

T

∗

R

)

−

σ

ϵ

2

+

Cov

ˆ

1

+

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)


Δˆ=r2(1−2)2σˆ2TR+c∗c{σˆ2ϵ−Covˆ1+(r−1)H(Covˆ2−Covˆ3)}
Δ

ˆ

=

r

2

(

1

−

2

)

2

σ

ˆ

T

R

2

+

c

∗

c

{

σ

ˆ

ϵ

2

−

Cov

ˆ

1

+

(

r

−

1

)

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

}


and


dfˆ2={σˆ2TR+c∗c\[σˆϵ−Covˆ1+(r−1)H(Covˆ2−Covˆ3)\]}2{σˆ2TR+(c∗c)\[σˆ2ϵ−Covˆ1−H(Covˆ2−Covˆ3)\]}2r−1
df

ˆ

2

=

{

σ

ˆ

T

R

2

+

c

∗

c

\[

σ

ˆ

ϵ

−

Cov

ˆ

1

+

(

r

−

1

)

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]

}

2

{

σ

ˆ

T

R

2

+

(

c

∗

c

)

\[

σ

ˆ

ϵ

2

−

Cov

ˆ

1

−

H

(

Cov

ˆ

2

−

Cov

ˆ

3

)

\]

}

2

r

−

1


In deriving these estimates we make the reasonable assumption that σ2ϵ
σ

ϵ

2
, Cov  1 , Cov  2 , and Cov  3 are inversely proportional to the number of cases for a specified normal-to-abnormal case ratio. Note that if Covˆ2−Covˆ3≤0
Cov

ˆ

2

−

Cov

ˆ

3

≤

0
, then


dfˆ2=\[σˆ2TR+(c∗c)(σˆ2ϵ−Covˆ1)\]2\[σˆ2TR+(c∗c)(σˆ2ϵ−Covˆ1)\]2r−1=r−1
df

ˆ

2

=

\[

σ

ˆ

T

R

2

+

(

c

∗

c

)

(

σ

ˆ

ϵ

2

−

Cov

ˆ

1

)

\]

2

\[

σ

ˆ

T

R

2

+

(

c

∗

c

)

(

σ

ˆ

ϵ

2

−

Cov

ˆ

1

)

\]

2

r

−

1

=

r

−

1


with _r_ − 1 being the lower bound on the denominator degrees of freedom.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

power=Pr(F1,dfˆ2;Δˆ>F1−α;1,dfˆ2)
power

=

Pr

(

F

1

,

df

ˆ

2

;

Δ

ˆ

>

F

1

−

α

;

1

,

df

ˆ

2

)


for a two-sided test with significance level _α_ , treating dfˆ2
df

ˆ

2
, and Δˆ
Δ

ˆ
as constants.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Appendix B

## Determination of the parameter estimated by the previously used estimate of σ2TR  σ    T    R    2   for the or procedure

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

σˆ2TR\_O=(σˆ21+σˆ22)2\[1−ρˆ\]
σ

ˆ

T

R

\_

O

2

=

(

σ

ˆ

1

2

+

σ

ˆ

2

2

)

2

\[

1

−

ρ

ˆ

\]


where σˆ21
σ

ˆ

1

2
and σˆ22
σ

ˆ

2

2
are the sample variances of the AUCs across readers for tests 1 and 2, respectively, and ρˆ
ρ

ˆ
is the within-reader correlation coefficient for the paired data (ˆ1j,ˆ2j),j=1,…,r
(

ˆ

1

j

,

ˆ

2

j

)

,

j

=

1

,

…

,

r
; ie,


σˆ2i=∑rj=1(ˆij−ˆi⋅)2r−1,i=1,2
σ

ˆ

i

2

=

∑

j

=

1

r

(

ˆ

i

j

−

ˆ

i

⋅

)

2

r

−

1

,

i

=

1

,

2


and


ρˆ=∑rj=1(ˆ1j−ˆ1⋅)(ˆ2j−ˆ2⋅)/(r−1)σˆ21√σˆ22√
ρ

ˆ

=

∑

j

=

1

r

(

ˆ

1

j

−

ˆ

1

⋅

)

(

ˆ

2

j

−

ˆ

2

⋅

)

/

(

r

−

1

)

σ

ˆ

1

2

σ

ˆ

2

2


From the OR model (Eq.  3 ) it follows that var (ˆij)=σ2R+σ2TR+σ2ϵ
(

ˆ

i

j

)

=

σ

R

2

+

σ

T

R

2

+

σ

ϵ

2
and covj≠j'(ˆij,ˆij')=Cov2
cov

j

≠

j

′

(

ˆ

i

j

,

ˆ

i

j

′

)

=

Co

v

2
; it follows that


E\[∑rj=1(ˆ1j−ˆ1⋅)2r−1\]=var(ˆij)−Cov2
E

\[

∑

j

=

1

r

(

ˆ

1

j

−

ˆ

1

⋅

)

2

r

−

1

\]

=

var

(

ˆ

i

j

)

−

Co

v

2


ie,


E(σˆ2i)=σ2R+σ2TR+σ2ϵ−Cov2
E

(

σ

ˆ

i

2

)

=

σ

R

2

+

σ

T

R

2

+

σ

ϵ

2

−

Co

v

2


Furthermore, we show at the end of this section that


∑rj=1(ˆ1j−ˆ1⋅)(ˆ2j−ˆ2⋅)r−1=\[MS(R)−MS(T∗R)\]t
∑

j

=

1

r

(

ˆ

1

j

−

ˆ

1

⋅

)

(

ˆ

2

j

−

ˆ

2

⋅

)

r

−

1

=

\[

MS

(

R

)

−

MS

(

T

∗

R

)

\]

t


where MS ( _R_ ) and MS ( _T_ ∗ _R_ ) are the reader and test × reader mean squares resulting from fitting the OR model to the pilot data.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

E\[MS(R)−MS(T∗R)\]/t=σ2R+Cov1−Cov3
E

\[

MS

(

R

)

−

MS

(

T

∗

R

)

\]

/

t

=

σ

R

2

+

Co

v

1

−

Co

v

3


From Equations  20 and 21 , it follows that


E\[∑rj=1(ˆ1j−ˆ1A⋅)(ˆ2j−ˆ2A⋅)r−1\]=σ2R+Cov1−Cov3
E

\[

∑

j

=

1

r

(

ˆ

1

j

−

ˆ

1

A

⋅

)

(

ˆ

2

j

−

ˆ

2

A

⋅

)

r

−

1

\]

=

σ

R

2

+

Co

v

1

−

Co

v

3


Replacing estimates by their expected value in Equation  17 using Equations  18, 19 , and  22 shows that σˆ2TR\_O
σ

ˆ

T

R

\_

O

2
estimates the following parameter:


\[σ2R+σ2TR+σ2ϵ−Cov2\]\[1−(σ2R+Cov1−Cov3)σ2R+σ2TR+σ2ϵ−Cov2\]=σ2TR+σ2ϵ−Cov1−(Cov2−Cov3)
\[

σ

R

2

+

σ

T

R

2

+

σ

ϵ

2

−

Co

v

2

\]

\[

1

−

(

σ

R

2

+

Co

v

1

−

Co

v

3

)

σ

R

2

+

σ

T

R

2

+

σ

ϵ

2

−

Co

v

2

\]

=

σ

T

R

2

+

σ

ϵ

2

−

Co

v

1

−

(

Co

v

2

−

Co

v

3

)


The relationship var ( _ϵ_ 11 − _ϵ_ 12 − _ϵ_ 21 \+ _ϵ_ 22 )≥0 implies that σ2ϵ−Cov1−(Cov2−Cov3)
σ

ϵ

2

−

Co

v

1

−

(

Co

v

2

−

Co

v

3

)
≥ 0.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

MS(R)−MS(TR)=t∑rj=1(ˆ.j−ˆ..)r−12−∑ti=1∑rj=1(ˆij−ˆi.−ˆ.j+ˆ..)2(t−1)(r−1)=\[(t∑rj=1ˆ2.j−trˆ2..)−(∑ti=1∑rj=1ˆ2ij−r∑ti=1ˆ2i.−t∑rj=1ˆ2.j+trˆ2..)\]r−1
MS

(

R

)

−

MS

(

T

R

)

=

t

∑

j

=

1

r

(

ˆ

.

j

−

ˆ

..

)

r

−

1

2

−

∑

i

=

1

t

∑

j

=

1

r

(

ˆ

i

j

−

ˆ

i

.

−

ˆ

.

j

+

ˆ

..

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

=

\[

(

t

∑

j

=

1

r

ˆ

.

j

2

−

t

r

ˆ

..

2

)

−

(

∑

i

=

1

t

∑

j

=

1

r

ˆ

i

j

2

−

r

∑

i

=

1

t

ˆ

i

.

2

−

t

∑

j

=

1

r

ˆ

.

j

2

+

t

r

ˆ

..

2

)

\]

r

−

1


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case 1

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

MS(R)−MS(TR)t=1t(t∑rj=1ˆ2.j)−(∑ti=1∑rj=1ˆ2ij−t∑rj=1ˆ2.j)r−1=1t(2t∑rj=1ˆ2.j)−(∑ti=1∑rj=1ˆ2ij)r−1=1t(2t∑rj=1(ˆ1j+ˆ2jt)2)−(∑ti=1∑rj=1ˆ2ij)r−1=1t\[2t(∑ti=1∑rj=1ˆ2ij+2∑rj=1ˆ1jˆ2j)−(∑ti=1∑rj=1ˆ2ij)\]r−1
MS

(

R

)

−

MS

(

T

R

)

t

=

1

t

(

t

∑

j

=

1

r

ˆ

.

j

2

)

−

(

∑

i

=

1

t

∑

j

=

1

r

ˆ

i

j

2

−

t

∑

j

=

1

r

ˆ

.

j

2

)

r

−

1

=

1

t

(

2

t

∑

j

=

1

r

ˆ

.

j

2

)

−

(

∑

i

=

1

t

∑

j

=

1

r

ˆ

i

j

2

)

r

−

1

=

1

t

(

2

t

∑

j

=

1

r

(

ˆ

1

j

+

ˆ

2

j

t

)

2

)

−

(

∑

i

=

1

t

∑

j

=

1

r

ˆ

i

j

2

)

r

−

1

=

1

t

\[

2

t

(

∑

i

=

1

t

∑

j

=

1

r

ˆ

i

j

2

+

2

∑

j

=

1

r

ˆ

1

j

ˆ

2

j

)

−

(

∑

i

=

1

t

∑

j

=

1

r

ˆ

i

j

2

)

\]

r

−

1


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

MS(R)−MS(T∗R)t=∑rj=1ˆ1jˆ2jr−1
MS

(

R

)

−

MS

(

T

∗

R

)

t

=

∑

j

=

1

r

ˆ

1

j

ˆ

2

j

r

−

1


and thus Equation  21 holds for the ˆij
ˆ

i

j
.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Case 2

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Dorfman D.D., Berbaum K.S., Metz C.E.: Receiver operating characteristic rating analysis: generalization to the population of readers and patients with the jackknife method. Invest Radiol 1992; 27: pp. 723-731.


- 2\. Dorfman D.D., Berbaum K.S., Lenth R.V., et. al.: Monte Carlo validation of a multireader method for receiver operating characteristic discrete rating data: factorial experimental design. Acad Radiol 1998; 5: pp. 591-602.


- 3\. Obuchowski N.A., Rockette H.E.: Hypothesis testing of the diagnostic accuracy for multiple diagnostic tests: an ANOVA approach with dependent observations. Commun Stat Simulation Computation 1995; 24: pp. 285-308.


- 4\. Obuchowski N.A.: Multi-reader multi-modality ROC studies: hypothesis testing and sample size estimation using an ANOVA approach with dependent observations. With rejoinder. Acad Radiol 1995; 2: pp. S22-S29.


- 5\. Obuchowski N.A., McClish D.K.: Sample size determination for diagnostic accuracy studies involving binormal ROC curve indices. Stat Med 1997; 16: pp. 1529-1542.


- 6\. Zhou X.-H., Obuchowski N.A., McClish D.K.: Statistical methods in diagnostic medicine.2002.WileyNew York


- 7\. Hillis S.L., Berbaum K.S.: Power estimation for the Dorfman-Berbaum-Metz method. Acad Radiol 2004; 11: pp. 1260-1273.


- 8\. Hillis S.L.: A comparison of denominator degrees of freedom methods for multiple observer ROC analysis. Stat Med 2007; 26: pp. 596-619.


- 9\. Hillis S.L., Obuchowski N.A., Schartz K.M., et. al.: A comparison of the Dorfman-Berbaum-Metz and Obuchowski-Rockette Methods for receiver operating characteristic (ROC) data. Stat Med 2005; 24: pp. 1579-1607.


- 10\. Hillis S.L., Berbaum K.S., Metz C.E.: Recent developments in the Dorfman-Berbaum-Metz procedure for multireader ROC study analysis. Acad Radiol 2008; 15: pp. 647-661.


- 11\. Quenoille M.H.: Approximate tests of correlation in time series. J Royal Stat Soc Series B 1949; 11: pp. 68-84.


- 12\. Quenoille M.H.: Notes on bias in estimation. Biometrika 1956; 43: pp. 353-360.


- 13\. Tukey J.W.: Bias and confidence in not quite large samples (abstract). Ann Math Stat 1958; 29: pp. 614.


- 14\.  Berbaum KS, Schartz KM, Pesce LL, et al. DBM MRMC 2.2 (computer software). Available for download from  http://perception.radiology.uiowa.edu  . Accessed August 1, 2009.


- 15\.  Berbaum KS, Metz CE, Pesce LL, et al. DBM MRMC 2.1 User’s Guide (software manual). Available for download from  http://perception.radiology.uiowa.edu  . Accessed August 1, 2009.


- 16\.  Hillis SL, Schartz KM, Pesce LL, et al. DBM MRMC procedure for SAS (computer software). Available for download from  http://perception.radiology.uiowa.edu  . Accessed August 1, 2009.


- 17\. DeLong E.R., DeLong D.M., Clarke-Pearson D.L.: Comparing the areas under two or more correlated receiver operating characteristic curves: a nonparametric approach. Biometrics 1988; 44: pp. 837-844.


- 18\. Hanley J.A., McNeil B.J.: The meaning and use of the area under a receiver operating characteristic (ROC) curve. Radiology 1982; 143: pp. 29-36.


- 19\. Obuchowski N.A.: Computing sample size for receiver operating characteristic studies. Invest Radiol 1994; 29: pp. 238-243.


- 20\.  Hillis SL, Berbaum KS. MRMC sample size program user’s guide (software manual). Available for download from  http://perception.radiology.uiowa.edu  . Accessed August 1, 2009.


- 21\.  Van Dyke CW, White RD, Obuchowski NA, et al. Cine MRI in the diagnosis of thoracic aortic dissection. 79th RSNA Meetings, Chicago, IL, November 28–December 3, 1993.


- 22\. Pan X.C., Metz C.E.: The “proper” binormal model: parametric receiver operating characteristic curve estimation with degenerate data. Acad Radiol 1997; 4: pp. 380-389.


- 23\. Metz C.E., Pan X.C.: “Proper” binormal ROC curves: theory and maximum-likelihood estimation. J Math Psychol 1999; 43: pp. 1-33.


- 24\.  SAS for Windows, Version 9.2, copyright 2002–2008 by SAS Institute Inc, Cary, NC.


- 25\. Roe C.A., Metz C.E.: Dorfman-Berbaum-Metz method for statistical analysis of multireader, multimodality receiver operating characteristic data: validation with computer simulation. Acad Radiol 1997; 4: pp. 298-303.


- 26\. Chakraborty D.P.: Prediction accuracy of a sample-size estimation method for ROC Studies. Acad Radiol 2010; 17: pp. 628-638.