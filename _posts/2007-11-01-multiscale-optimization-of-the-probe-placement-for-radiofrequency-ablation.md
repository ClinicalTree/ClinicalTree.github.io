---
title: Multiscale Optimization of the Probe Placement for Radiofrequency Ablation
author: [CL_AT_IngaAltrogge,CL_AT_TobiasPreusser,CL_AT_TimKrger,CL_AT_ChristofBskens,CL_AT_PhilippeLPereira,CL_AT_DiethardSchmidt,CL_AT_HeinzOttoPeitgen]
date: 2007-11-01 00:00:00 +0700 +07
categories: [Academic Radiology, Volume 14, Issue 11]
tags: [Journals,General Radiology]
---
## Rationale and Objectives

We present a model for the optimal placement of mono- and bipolar probes in radiofrequency (RF) ablation. The model is based on a system of partial differential equations that describe the electric potential of the probe and the steady state of the induced heat distribution.

## Materials and Methods

To optimize the probe placement we minimize a temperature-based objective function under the constraining system of partial differential equations. Further, the extension of the resulting optimality system for the use of multiple coupled RF probes is discussed. We choose a multiscale gradient descent approach to solve the optimality system.

## Results

This article describes the discretization and implementation of the approach with finite elements on three-dimensional hexahedral grids.

## Conclusion

Applications of the optimization to artificial test scenarios as well as a comparison to a real RF ablation show the usefulness of the approach.

During the last decade, local and minimally invasive techniques have become a promising treatment of tumor diseases. Especially in situations in which a surgical resection or chemotherapy is not possible because of the extent of the tumor or the general state of the patient, thermotherapies such as radiofrequency (RF) ablation offer an alternative and less invasive form of treatment.

In this work, we consider the RF ablation of hepatic tumors with mono- or bipolar systems (see  Fig 1 ): A probe, which is connected to an electric generator, is placed inside the malignant tissue, so that an electric current flows through the body and heats the tissue near the probe up to temperatures of more than 60°C.

![](https://d1niluoi1dd30v.cloudfront.net/10766332/S1076633207X00928/S1076633207004448/gr1.jpg?Signature=L%7EPr7sspoYQogxZ8o6R2TpfBOPypq98jl7gcp8e5u%7EJaGCamB-gQDoMEVJ7lc8gepJebA1pJp4gMzcA2s4z3deDaSnxjLSSdQFyVPW2gLr2-uF4ftYXViSZ9XAP45AgQbl3ppLmUlf1v2oORtcf%7EodMtYkxsGcHtbKU54xZiO7w_&Expires=1669521929&Key-Pair-Id=APKAICLNFGBCWWYGVIZQ)Open full size image

Figure 1


Schematic sketch of a bipolar RF ablation.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## A model for the simulation of RF ablation

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 2, Schematic setting of the considered configuration. Note that Ω+∪Ω−=Ω±⊂Ωpr Ω+∪Ω−=Ω±⊂Ωpr , where all these sets depend on x¯ x¯ and a¯ a¯ .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/0_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

−div(σ∇)=0inΩ\Ω¯¯¯±
−

div

(

σ

∇

)

=

0

in

Ω

\

Ω

¯

±


with appropriate boundary conditions (see below), models the electric potential _ϕ_ : Ω → R of the RF probe. Here, _σ_ ∈ ℝ is the electric conductivity of the tissue. For the electrostatic equation, we consider the boundary conditions


=±1onΩ¯¯¯+andΩ¯¯¯−,
=

±

1

on

Ω

¯

+

and

Ω

¯

−

,


n⋅∇=n⋅(x¯−x)\|x¯−x\|2onΓout,
n

⋅

∇

=

n

⋅

(

x

¯

−

x

)

\|

x

¯

−

x

\|

2

on

Γ

out

,


where _n_ denotes the outer normal on Γ  out . Equation  2a fixes the potential on the electrodes, and the Robin boundary condition in Eq  2b is based on the assumption that on the boundary (far from the probe) the potential behaves approximately as induced by a point load at the barycenter x¯
x

¯
of the probe.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 3, Equivalent circuit diagram for the calculation of the scaling factor that is needed to convert the unscaled power P into the effective heat source Q rf .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/1_1s20S1076633207004448.jpg)

![Figure 4, The characteristic curve of the generator shows the dependence of the effective power P eff on the impedance R of the tissue, whereas R I and P setup are fixed (here: R I = 80Ω, P setup = 200 W).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/2_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

R=U2PtotalwithPtotal=∫Ωσ\|∇\|2dx,
R

=

U

2

P

total

with

P

total

=

∫

Ω

σ

\|

∇

\|

2

d

x

,


where _U_ is the difference of the potential _ϕ_ on the two electrodes ( _U_ = 2V for bipolar probes and _U_ = 1V for monopolar probes) (see Eq  2a ). According to the equivalent circuit diagram shown in  Fig 2 , the effective power of the generator is now given by


Peff=4PsetupRRI(R+RI)2,
P

eff

=

4

P

setup

R

R

I

(

R

+

R

I

)

2

,


where _R_ I is the inner resistance of the generator and _P_ setup is the value set up at the generator’s control unit. Finally, the heat source is given by


Qrf=PeffPtotalσ\|∇\|2.
Q

rf

=

P

eff

P

total

σ

\|

∇

\|

2

.


The spatial distribution of heat T : Ω → ℝ is modeled by the steady state of the so-called bioheat-transfer equation


−div(λ∇T)=Qrf+QperfinΩ.
−

div

(

λ

∇

T

)

=

Q

rf

+

Q

perf

in

Ω

.


Here, _λ_ ∈ ℝ is the thermal conductivity of the tissue. The right hand side of Eq  3 consists of the source (heating) _Q_ rf from the electric current and the sink (cooling) _Q_ perf from the vascular system. We assume that there is no heating on the outer boundary of Ω and thus consider the Dirichlet boundary condition


T=TbodyonΓout.
T

=

T

body

on

Γ

out

.


Finally, the term modeling the cooling effects of the blood perfusion _Q_ perf is a variant of the approach of Pennes ( ):


Qperf=−v(T−Tbody),
Q

perf

=

−

v

(

T

−

T

body

)

,


where


v=v(x)={vvesselρm,Bcm,B,vcapρm,Bcm,B,x∈Ωv,else.
v

=

v

(

x

)

=

{

v

vessel

ρ

m,B

c

m,B

,

x

∈

Ω

v

,

v

cap

ρ

m,B

c

m,B

,

else

.


Thus the coefficient _v_ depends on the relative blood circulation rate vvessel\[s−1\]
v

vessel

\[

s

−

1

\]
of vessels and vcap\[s−1\]
v

cap

\[

s

−

1

\]
of capillaries respectively, as well as on the blood density _ρ_ m,B \[k _g_ /m\] and the heat capacity cm,B\[J/kgK\]
c

m,B

\[

J

/

k

g

K

\]
of blood. Here we assume that the whole tissue is pervaded by capillary vessels and thus is exposed to their cooling influence.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

−σΔ=0inΩ/Ω¯¯¯±,
−

σΔ

=

0

in

Ω

/

Ω

¯

±

,


−λΔT+vT=Qrf+vTbodyinΩ
−

λΔT

+

vT

=

Q

rf

+

v

T

body

in

Ω


with boundary conditions Eq  2a, 2b, and 4 . Here _H_ 1 = _H_ 1,2 denotes the Sobolev space of functions having weak derivatives ( ). Note that the two equations are coupled through the term _Q_ rf on the right hand side of the steady state heat equation in Eq  5b .


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Objective functions

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

f(T)=ω12∥T−Tbody∥2L2(Ω\Ωtu)+ω22∥T−Tcrit∥2L2(Ωtu)
f

(

T

)

=

ω

1

2

∥

T

−

T

body

∥

L

2

(

Ω

\

Ω

tu

)

2

+

ω

2

2

∥

T

−

T

crit

∥

L

2

(

Ω

tu

)

2


with ω  1 and ω  2 being suitable weights, so that the above requirements are met. Here, _L_ 2 (Ω) is the space of square integrable functions on Ω and ∥∥v∥2L2=(v,v)
∥

v

∥

L

2

2

=

(

v

,

v

)
is the norm on _L_ 2 where ( _v,w_ ) = ∫  Ω _vwdx_ denotes the scalar poduct.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

f(T)=∫Ωtue−T(x)dx.
f

(

T

)

=

∫

Ω

tu

e

−

T

(

x

)

d

x

.


By using the exponential function, we aim at an equal heat distribution inside the tumor. The lowest temperature inside the tumor is penalized most (see black curve in  Fig 5 ), so that configurations with only a small sufficiently hot volume inside the tumor lead to a higher value of the objective function than a uniform tumor heating.

![Figure 5, Different curves of exponential functions without additional weighting (black) or with a weighting factor in the argument (gray). The steep slope leads to a high penalty for low temperatures.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/3_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

f(T)=∫Ωtue−αT(x)dx.
f

(

T

)

=

∫

Ω

tu

e

−

α

T

(

x

)

d

x

.


This allows for a modification of the grade of penalization of a non-uniform temperature distribution inside the tumor (lower penalization for _α_ < 1; stronger penalization for _α_ \> 1; see gray curves in  Fig 4 ).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

f(T)=eTmin∫Ωtue−T(x)dx=∫ΩtueTmin−T(x)dx,
f

(

T

)

=

e

T

min

⁡

∫

Ω

tu

e

−

T

(

x

)

d

x

=

∫

Ω

tu

e

T

min

⁡

−

T

(

x

)

d

x

,


where _T_ min is the minimal temperature of the current iteration step. This modification guarantees that the argument of the exponential function does not become too large. The analog modification for the objective function ( ) is straightforward.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Optimizing the probe placement

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Qrf=Q(u),Q:U→L2(Ω),T=T(Qrf),T:L2(Ω)→H1(Ω)
Q

rf

=

Q

(

u

)

,

Q

:

U

→

L

2

(

Ω

)

,

T

=

T

(

Q

rf

)

,

T

:

L

2

(

Ω

)

→

H

1

(

Ω

)


To optimize the probe location, we are looking for _u_ ∈ _U_ such that F:U→R,u↦F(u):=f
F

:

U

→

ℝ

,

u

↦

F

(

u

)

:=

f
· T
T
· Q
Q
( _u_ ) becomes minimal.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

U˜=Ω×(R3\{0})⊃U,
U

˜

=

Ω

×

(

ℝ

3

\

{

0

}

)

⊃

U

,


and introduce the projection


P:U˜→U,(x¯,a¯)↦(x¯,a¯/\|a¯\|).
P

:

U

˜

→

U

,

(

x

¯

,

a

¯

)

↦

(

x

¯

,

a

¯

/

\|

a

¯

\|

)

.


Now we set


Q(x¯,a¯)=(Q⋅P)(x¯,a¯)=Q(x¯,a¯/\|a¯\|),
Q

(

x

¯

,

a

¯

)

=

(

Q

⋅

P

)

(

x

¯

,

a

¯

)

=

Q

(

x

¯

,

a

¯

/

\|

a

¯

\|

)

,


(ie, Q
Q
does not depend on the length of a¯
a

¯
).


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Initial value

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Descent direction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step size

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Stopping criterion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Descent Direction

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

∂ujF(u)=f′(T⋅Q(u))\[T′(Q(u))\[∂ujQ(u)\]\]=T′(Q(u))\*\[f′(T⋅Q(u))\]\[∂ujQ(u)\]
∂

u

j

F

(

u

)

=

f

′

(

T

⋅

Q

(

u

)

)

\[

T

′

(

Q

(

u

)

)

\[

∂

u

j

Q

(

u

)

\]

\]

=

T

′

(

Q

(

u

)

)

\*

\[

f

′

(

T

⋅

Q

(

u

)

)

\]

\[

∂

u

j

Q

(

u

)

\]


where ′ denotes the Frechet derivative, \* denotes the adjoint operator, and brackets \[ · \] denote the application of linear operators. For the calculation of ∂ujQ(u)
∂

u

j

Q

(

u

)
, we use a numerical approximation by central differences, whereas we determine _f′_ analytically as


f′(T)\[w\]=−(αe−αT,w)L2(Ωtu).
f

′

(

T

)

\[

w

\]

=

−

(

α

e

−

α

T

,

w

)

L

2

(

Ω

tu

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

T′(Qrf)\*\[f′(T)\]\[w\]=(p,w)L2(Ω),
T

′

(

Q

rf

)

\*

\[

f

′

(

T

)

\]

\[

w

\]

=

(

p

,

w

)

L

2

(

Ω

)

,


where _p_ ∈ _H_ 1 (Ω) is the solution to the adjoint problem of Eq  5b with boundary condition (Eq  4 ):


−λΔp+vp=−αe−αTp=0inΩ,onΓout.
−

λ

Δ

p

+

v

p

=

−

α

e

−

α

T

in

Ω

,

p

=

0

on

Γ

out

.


The advantage of the above application of the chain-rule Eq  8 over a numerical approximation of ∂ujF(u)
∂

u

j

F

(

u

)
is the reduction of the numerical effort. Our approach needs evaluations of the potential equation only (everything else is done analytically), whereas a full numerical differentiation would involve the coupled system (Eq  5a, 5b ) and thus be at least about twice as expensive.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Step Size

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

s0∣∣v0∣∣=12diam(Ω),i.e.s0=diam(Ω)2\|v0\|.
s

0

\|

v

0

\|

=

1

2

diam

(

Ω

)

,

i.e.

s

0

=

diam

(

Ω

)

2

\|

v

0

\|

.


In the following iteration steps _n_ \> 0 we start with a step size that fulfills


\|vn\|sn=2∣∣vn−1∣∣sn−1,i.e.sn=2∣∣vn−1∣∣\|vn\|sn−1.
\|

v

n

\|

s

n

=

2

\|

v

n

−

1

\|

s

n

−

1

,

i.e.

s

n

=

2

\|

v

n

−

1

\|

\|

v

n

\|

s

n

−

1

.


After having chosen an initial value for the step size _s  n_ , we bisect _s  n_ until the new iterate un+1=P(un+snvn)
u

n

+

1

=

P

(

u

n

+

s

n

v

n

)
fulfills _u__n_ +1 ∈ _U_ and F( _u__n_ +1 ) < F ( _u__n_ ). If these conditions are not matched after a certain number of bisections, the step size _s  n_ is set to zero and the algorithm stops.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Stopping Criterion

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

∣∣x¯n+1−x¯n∣∣<1and∣∣a¯n+1−a¯n∣∣<2.
\|

x

¯

n

+

1

−

x

¯

n

\|

<

1

and

\|

a

¯

n

+

1

−

a

¯

n

\|

<

2

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Optimization of Multiple Coupled Probes

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

U={(x¯,a¯,r¯)∈Ω×S2×S2:r¯⊥a¯}.
U

=

{

(

x

¯

,

a

¯

,

r

¯

)

∈

Ω

×

S

2

×

S

2

:

r

¯

⊥

a

¯

}

.


Again, for easier handling of the gradient with respect to the optimization variable, we replace _U_ with the open set


U˜={(x¯,a¯,r¯)∈Ω×R3×R3:r¯∦a¯}
U

˜

=

{

(

x

¯

,

a

¯

,

r

¯

)

∈

Ω

×

ℝ

3

×

ℝ

3

:

r

¯

∦

a

¯

}


and use the projection


P:U˜→U,(x¯,a¯,r¯)↦(x¯,a¯\|a¯\|,\|a¯\|2r¯−(r¯,a¯)a¯\|\|a¯\|2r¯−(r¯,a¯)a¯∣∣).
P

:

U

˜

→

U

,

(

x

¯

,

a

¯

,

r

¯

)

↦

(

x

¯

,

a

¯

\|

a

¯

\|

,

\|

a

¯

\|

2

r

¯

−

(

r

¯

,

a

¯

)

a

¯

\|

\|

a

¯

\|

2

r

¯

−

(

r

¯

,

a

¯

)

a

¯

\|

)

.


![Figure 6, A probe cluster and its parameters.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/4_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Discretization with finite elements

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Reduction to a Linear System of Equations

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

λ(∇T,∇v)L2(Ω)+v(T,v)L2(Ω)=(Qrf+vTbody,v)L2(Ω)∀v∈H10(Ω).
λ

(

∇

T

,

∇

v

)

L

2

(

Ω

)

+

v

(

T

,

v

)

L

2

(

Ω

)

=

(

Q

rf

+

v

T

body

,

v

)

L

2

(

Ω

)

⁢

∀

v

∈

H

0

1

(

Ω

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Vhl=span{ψli\|i=1,…,nl},
V

l

h

=

span

{

ψ

i

l

\|

i

=

1

,

…

,

n

l

}

,


where ψli
ψ

i

l
is given by the requirements that ψli
ψ

i

l
is trilinear on each grid cell of G _l_ and ψli(xj)=δij
ψ

i

l

(

x

j

)

=

δ

i

j
for all nodes xi∈Nl
x

i

⁢

∈

N

l
. Here δ _ij_ is the Kronecker symbol. Then every function w∈Vhl
w

⁢

∈

V

l

h
is determined by its nodal values _w  i_ at the vertices _x  i_ ∈ N _l_ :


w(x)=∑nli=1wiψli(x).
w

(

x

)

=

∑

i

=

1

n

l

w

i

ψ

i

l

(

x

)

.


Because the weak form (Eq  11 ) is linear in the test function _v_ , it suffices to test this equation with all the basis functions of Vhl
V

l

h
(ie _v_ = ψil
ψ

l

i
for _j_ = 1, …, _n  l_ ). This leads to a system of equations in the nodal values _t  i_ of the temperature _T_ . Denoting the vector of nodal values with _t_ = ( _t  i_ ) _i_ and the right hand side with _r_ = ( _r  i_ ) _i_ , we have to solve


(λL+M)t=rwithri=(Qrf+vTbody,ψli)L2(Ω),
(

λL

+

M

)

t

=

r

⁢

with

⁢

r

i

=

(

Q

rf

+

v

T

body

,

ψ

i

l

)

L

2

(

Ω

)

,


where _L_ = ( _L  ij_ ) _ij_ is the so called _stiffness matrix_ and M = ( _M  ij_ ) _ij_ the so called _mass matrix_ defined by


Lij=(∇ψli,∇ψlj)L2(Ω)andMij=(vψli,ψlj)L2(Ω).
L

i

j

=

(

∇

ψ

i

l

,

∇

ψ

j

l

)

L

2

(

Ω

)

and

M

i

j

=

(

v

ψ

i

l

,

ψ

j

l

)

L

2

(

Ω

)

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Numerical Integration

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

∫Ωtue−αT(x)dx=∑E∈Gl∫EχLtu(x)e−αT(x)dx≈∑E∈Gl\|E\|8∑xi∈E∩Nl(χLtue−αT)(xi).
∫

Ω

tu

e

−

α

T

(

x

)

d

x

=

∑

E

∈

G

l

∫

E

χ

t

u

L

(

x

)

e

−

α

T

(

x

)

d

x

≈

∑

E

∈

G

l

\|

E

\|

8

∑

x

i

∈

E

∩

N

l

(

χ

tu

L

e

−

α

T

)

(

x

i

)

.


For the integration of the mass matrix _M_ and the right hand side _r_ , we use _lumped masses_ ( ), which corresponds to a quadrature in which the coefficient _v_ and the heat source _Q_ rf are evaluated at the midpoints of elements only.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## A Multiscale Optimization Approach

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Rll+1:Vhl+1→Vhl
R

l

+

1

l

⁢

:

V

l

+

1

h

→

V

l

h


for l = 0, …, _L_ − 1, which transports finite element functions to the next coarser level. A straightforward approach would use the trivial restriction that directly multiplies the nodal values of a fine-grid function with the coarse-grid basis function. However, this leads to unsatisfactory results, because on coarse grids it does not preserve details of the tumor, which have important influence on the choice of the optimal probe positioning. Therefore we propose to use the classical restriction of multigrid approaches for the solution of PDEs ( ). We set Rll+1=(Pll+1)T
R

l

+

1

l

=

(

P

l

+

1

l

)

T
where Pll+1
P

l

+

1

l
is the trilinear interpolation from grid G _l_ to grid G _l_ +1 involving the weights {1/8,1/4,1/2,1}. So we set


χltu=Rll+1χl+1tu,χlv=Rll+1χl+1v.
χ

tu

l

=

R

l

+

1

l

χ

tu

l

+

1

,

χ

v

l

=

R

l

+

1

l

χ

v

l

+

1

.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 7, Intersection of the probe with a slice of the grid orthogonal to the probe. Here, h i is the minimal voxel size of the grid G l , so the diameter of the probe must be at least hl2–√ hl2 .](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/5_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 8, (Left) The progression of the objective function value is shown for the multiscale optimization algorithm (•) and the standard algorithm (+). In contrast to the standard algorithm the multiscale optimization finds a slightly better minimum with a smaller number of iterations on the finest grid. (Right) The progression of the objective function value is shown for the definition of a coarse grid tumor and vascular domains that involve a thresholding.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/6_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

χltu(xj)={10if(Rll+1χl+1)(xj)≥1/2else,
χ

tu

l

(

x

j

)

=

{

1

i

f

(

R

l

+

1

l

χ

l

+

1

)

(

x

j

)

≥

1

/

2

0

else,


and analog for χlv
χ

v

l
. The progression of the corresponding objective function value is shown in the right graph of  Fig 7 . Because here the mass of the tumor and the vessels is not conserved on the coarse levels, the values of the objective function increase at the transition stages.


[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 9, Optimization of the probe’s placement for an artificial example with an ellipsoid-shaped tumor (dark gray), a linear vessel (black), and a monopolar probe (white-gray). The transparent layer is the corresponding 60°C isosurface of the temperature. (A) Steps 0 (start), 2, 5, and 20 of the first preoptimization (coarsest grid). (B) Steps 0 and 11 of the second preoptimization. (C) Steps 0 and 3 (end) of the main optimization. (Color images are available at www.cevis.uni-bremen.de/∼tim/ .)](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/7_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## The Optimization Algorithm

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

Table 1


Algorithm 1—Multi-scale optimization of the probe location


1:_l_ ← _l_ 0  ▷Start with level _l_ 0  2: Initialize u¯.
u

¯

.
3:**while** _l_ ≤ _L_ **do** 4:_u_ 0  ← u¯
u

¯
▷ Initialization 5:_n_ ← 0 6:**repeat** ▷ Compute descent direction 7:_v  n_ ← −∇ _u__F_ ( _u  n_ ) 8:**if** _n_ = 0 **then** ▷ Initialize step size 9:_s_ 0  = (2\| _v_ 0  \|)  −1  diam(Ω) 10:**else** 11:_s  n_ = 2\| _v__n_ −1  \|(\| _v  n_ \|)  −1 _s__n_ −1  12:**end if** 13:_m_ ← 0 ▷ Reset counter ▷ Determine step size 14:_u__n_ +1  ← _P_ ( _u  n_ \+ _s  n  v  n_ ) 15:**while** _F_ ( _u__n_ +1  ) \> _F_ ( _u  n_ ) or _u__n_ +1  ∉ _U_ **do** 16:_m_ ← _m_ \+ 1 ▷ Increase counter 17:**if** _m_ = _m_ max **then** 18: STOP. 19:**end** **if** 20:_s  n_ ← _s  n_ /2 ▷ Bisect step size 21:_u__n_ +1  ← _P_ ( _u  n_ \+ _s  n  v  n_ ) 22:**end** **while** 23:**until u _n_ +1  − _u  n_ \| ≤ θ** 24:u¯
u

¯
← _u__n_ +1  25:_l_ ← _l_ \+ 1 ▷ Proceed to next level 26:**end while**

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Numerical results

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 10, Optimization for an example based on patient data with segmented tumor and surrounding vascular system. Here we have a fixed cluster of three monopolar probes with the corresponding 60°C isosurface of the temperature. (A) Steps 0 (start), 2, 5, and 11 of the first preoptimization (coarsest grid). (B) Steps 0 and 3 of the second preoptimization. (C) Steps 0 and 2 (end) of the main optimization.](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/8_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

![Figure 11, Comparison of the computed optimal probe placement (left) with the probe placement chosen by the responsible physician (right).](https://storage.googleapis.com/dl.dentistrykey.com/clinical/MultiscaleOptimizationoftheProbePlacementforRadiofrequencyAblation/9_1s20S1076633207004448.jpg)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Conclusions and future work

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## Acknowledgments

[Get Radiology Tree app to read full this article<](https://clinicalpub.com/app)

## References

- 1\. Stein T.: Untersuchungen zur Dosimetrie der hochfrequenzstrominduzierten interstitiellen Thermotherapie in bipolarer Technik, vol 22.2000.Müller and Berlien Fortschritte in der Lasermedizin


- 2\. Tungjitkusolum S., Staelin S.T., Haemmerich D., et. al.: Three-dimensional finite-element analyses for radio-frequency hepatic tumor ablation. IEEE Trans Biomed Eng 2002; 49: pp. 3-9.


- 3\. Welp C., Siebers S., Ermert H., et. al.: Investigation of the influence of blood flow rate on large vessel cooling in hepatic radiofrequency ablation. Biomed Tech 2006; 51: pp. 337-346.


- 4\. Deuflhard P., Weiser M., Seebaß M.: A new nonlinear elliptic multilevel FEM applied to regional hyperthermia. Comp Vis Sci 2000; 3: pp. 115-120.


- 5\.  Roggan A. Dosimetrie thermischer Laseranwendungen in der Medizin 1997; 16 (Fortschritte in der Lasermedizin, Müller and Berlien, 1997.


- 6\. Jain M.K., Wolf P.D.: A three-dimensional finite element model of radiofrequency ablation with blood flow and its experimental validation. Ann Biomed Eng 2000; 28: pp. 1075-1084.


- 7\. Preusser T., Weihusen A., Peitgen H.O.: On the modelling of perfusion in the simulation of RF-ablation. SimVis 2005; pp. 259-269.


- 8\. Tröltzsch F.: Optimale Steuerung partieller Differentialgleichungen.2005.ViewegWiesbaden


- 9\. Geiger C., Kanzow C.: Theorie und Numerik restringierter rungsaufgaben.2002.SpringerBerlin


- 10\. Khalil-Bustany I.S., Diederich C.J., Polak E., et. al.: Minmax optimization-based inverse treatment planning for interstitial thermal therapy. Int J Hypertherm 1998; 14: pp. 347-366.


- 11\. Gaenzler T., Volkwein S., Weiser M.: SQP methods for parametric identification problems arising in hyperthermia. Optimization Methods Software 2006; 6: pp. 869-887.


- 12\. Villard C., Soler L., Gangi A.: Radiofrequency ablation of hepatic tumors: simulation, planning, and contribution of virtual reality and haptics. Comp Meth Biomech Biomed Eng 2005; 8: pp. 215-227.


- 13\. Bourquain H., Schenk A., et. al.: Hepavision2: a software assistant for preoperative planning in living-related liver transplantation and oncologic liver surgery. CARS 2002; pp. 341-346.


- 14\. Pennes H.H.: Analysis of tissue and arterial blood temperatures in a resting forearm. J Appl Physiol 1948; 1: pp. 93-122.


- 15\. Altrogge I., Kröger T., Preusser T., et. al.: Towards optimization of probe placement for radio-frequency ablation. LNCS 2006; 4190: pp. 486-493.


- 16\. Braess D.: Finite Elemente, ed 3.2003.SpringerBerlin:


- 17\. Preusser T., Rumpf M.: An adaptive finite element method for large scale image processing.1999.pp. 223-234.


- 18\. Thomee V.: Galerkin-finite element methods for parabolic problems.1984.SpringerNew York


- 19\. Hackbusch W.: Multi-grid methods and applications, Vol. 4 of Springer Series in Computational Mathematics.1985.SpringerBerlin