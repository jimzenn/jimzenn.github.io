---
title: "Linear Transformation"
date: 2018-07-11T11:03:48+08:00
author: "Jim Zenn"
volumes: ["MATH 115A"]
layout: "note"
issue: 2.1


---

Linear transformation, range, kernel (null space), range (image),

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\C}{\mathbb{C}}$
    $\newcommand{\P}{\mathbb{P}}$
    $\newcommand{\F}{\mathbb{F}}$
    $\newcommand{\B}{\beta}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{|#1|}$
    $\newcommand{\t#1}{\text}[1]$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
  {{< /raw >}}
</div>

{{% definition name="" %}}

$V/F$, $W$ is a vector space over field $F$.

A linear transformation or linear map $T:V \to W$ is a function which satisfies the following properties.

1. $T(v_1+v_2) = T(v_1) + (v_2), \forall v_1, v_2 \in V.$
2. $T(cv) = cT(v), \forall v \in V, c \in F.$

{{% /definition %}}

{{% example name="" %}}
$T: \R^3 \to \R^2$

$T(a_1, a_2, a_3) = (2a_1-a_3, a_2 - a_1)$

$T((a_1, a_2, a_3)  + (b_1, b_2, b_3))$
$=T(a_1 + b_1, a_2 + b_2, a_3 + b_3)$
$=(2(a_1 + b_1) - (a_3 + b_3), (a_2 + b_2) - (a_1 + b_1))$

$T(c(a_1, a_2, a_3)) = T((ca_1, ca_2, ca_3)) = (c(2a-a_3), c(a_2 - a_1))$

$T((a_1, a_2, a_3)) = (2a_1-a_3, a_2 - a_1)$
$T((b_1, b_2, b_3)) = (2b_1-b_3, b_2 - b_1)$
$T((a_1, a_2, a_3)) + T((b_1, b_2, b_3))$
$= (2a_1-a_3, a_2 - a_1) + (2b_1-b_3, b_2 - b_1) = ...$

{{% /example %}}

{{% example name="reflection about x-axis" %}}

$T: \R^2 \to \R^2$

$T(a,b) = (a, -b)$

{{% /example %}}

{{% example name="Rotation" %}}

$T: \R^2 \to \R^2$

$T(P)=P'$

$P=(a,b)$

$T((a,b)) = (a\cos \theta - b \sin \theta, a \sin \theta + b \cos \theta)$

{{% /example %}}

{{% properties name="Basic properties of linear transformation" %}}

1. If $T: V \to W$ a lin trans <br>
then (1) T(0) = 0 <br>
and (2) T(v_1 - v_2) = T(v_1) - T(v_2)
2. $T:: V \to W$ is a linear transportation $\iff T(cv_1 + v_2) = c T(v_1) + T(v_2), \forall v_1, v_2 \in V, \forall c \in F$

{{% proof index="" name="" %}}

(1) $T(0) = T(0 + 0) = T(0) + T(0) \implies T(0) + 0 = T(0) + T(0)

By cancellation law 0 = T(0)

(2) T(v_1 - v_2) = T(v_1 + (-v_2))

{{% /proof %}}

{{% /properties %}}

{{% examples name="" %}}

$\R^2 \to \R^2$

$T(x, y) = T(x + y, x-y + 1)$ not a linear transformation.

$T(x, y) = (x, \abs{y})$ not a linear transformation.

{{% /examples %}}

{{% example name="" %}}

$T: M_{m \times n}( \R ) \to M_{n \times m} ( \R)$

$T(A) = A^t$ is a lintrans

{{% /example %}}

{{% example name="" %}}
$T: \P_n(x) \to \P_{n-1}(x)$

$T(f(x)) = f'(x)$

$T(cf(x) + g(x)) = (cf(x) + g(x))' = cf'(x) g'(x) = cT(f(x)) + T(g(x))$

{{% /example %}}

{{% example name="" %}}

$T:\R^2 \to \R^3$

$T(a_1, a_2) = (a_1, a_2, 0)$

{{% /example %}}

{{% remarks name="Identity transformation" %}}

$I: V \to V$
$I(x) = x, \forall v \in V$

{{% /remarks %}}

{{% remarks name="zero transformation" %}}

$T: V \to W$

$T(x) = 0 \forall x \in V$

$T(cx +y) = 0$

$T(cx ) + T(y) = 0 + 0 = 0$

{{% /remarks %}}


{{% definition name="" %}}

$ T: V \to W $ be a linear transformation.
The kernel or null space of T denoted by $N(T)$ is defined as $N(T) = { x \in V : T(x) = 0 }$

The range or image of T is denoted by $R(T)$ is defined as $R(T)= {T(x) : x \in V}
$
{{% /definition %}}


{{% theorem name="" index="" %}}

$T: V \to W$ lin trans

then $N(T)$ is a subspace of $V$, and R(T) is a subspace of $W$.

{{% proof index="" name="" %}}
$x, y \in N(T), i.e. T(x) = 0, T(y) = 0$ <br>
need to show that $x + y \in N(T)$.

$T(x + y) = T(x) + T(y) = 0 + 0 = 0$

$x+y \in N(T)$

$x \in N(T) \implies T(x) = 0$
$c \in F$
$cx \in N(T)$

$T(cx) = cT(x) = c0 = 0$

$\implies x \in N(T) $


...................
$w_1, w_2 \in R(T)$

$\implies \exists x_1, x_2 \in V, s.t.$
$T(x_1) = w_1$
$T(x_2) = w_2$

$w_1+ w_2 =T(x_1) + T(x_2) = T(x_1 + x_2)$

$\implies (w_1 + w_2) \in R(T)$

$w \in R(T) \implies \exists x \in V s.t. T(x) = w$

$cw \in R(T)$

$cw= cT(x) = T(cx)$

$cw \in R(T)$

{{% /proof %}}

{{% /theorem %}}

{{% definition name="nullity and rank" %}}

$T:V \to W$ lin trans

The dimension of the null space N(T) is called the Nullity of $T$

It is denoted by nullity(T).


The dimension of image space R(T) is called the rank of T.
It is denoted by rank(T).

{{% /definition %}}

{{% example name="$A_{m \times n}$" %}}

$T: \R^n \to \R^m$

$T(x) = Ax, \forall x \in \R^n$

$T(cx+ y) = A(cx+y) = A(cx) + Ay = cAx + Ay = cT(x) + T(y)$

$rank(A) = rank(T)$

{{% /example %}}

{{% theorem name="Rank-nullity Theorem" index="" %}}

Let $T: V \in W$ lin trans

$\dim V$ is FINITE

Then $rank(T) + nullity(T) = \dim V$

$\dim R(T) + \dim N(T) = \dim V$

{{% proof index="" name="" %}}
Let $\dim N(T) = \R$
$N(T) \leq V$

let $\B = \set{ x\_1, x\_2, ..., x\_{r} }$ be a basis of $N(T)$

Since $N(T) \leq V$, $\B$ can be extended to a basis of $V$, saying $\gamma  = \B \cup \set{ y\_1, y\_2, ..., y\_{ n-k } } when h = \dim V$

$i.e.  \gamma = \set{ x_1, ..., x_k, y_1, ..., y_{n-k} }$ is a basis of $V$.

$T: V \to W$, R(T)

{{% /proof %}}

{{% /theorem %}}

{{% theorem name="" index="" %}}
$T:V \to W$

If $\B = \set{ x\_1, x\_2, ..., x\_{n}}$ is a basis of $V_1$ then $R(T) = \spa{ T(x_1), T(x_2), ... T(x_n) }$

let $w in R(T)$

Then $\exists x \in v s.t. T(x) = w$

since $\beta$ is a bsis of $V \exists c\_1, c\_2, ..., c\_{n} \in F s.t. x = \sum\_{  }^{  } c_ix_i$

Then $T(x) = T( \sum\_{ i=1 }^{n} c_ix_i) = \sum\_{ i=1 }^{n} c_i T(x_i)$
$i.e. \sum\_{ i=1 }^{n} c_i T(x_i)$

Then $R(T) = \spa{ T(x_i), ..., T(x_k), T(y_1), ... , T(y_{1-k}) } = \spa{ T(y_1), ..., T(y_{n-k}) }$

Need to prove this set is acutally linearly independent.

Consider the equation, $a_1T(y_1)+ ... + a_{n-k}T(y_{n-k}) = 0$

$\implies T( a\_1y\_1 + a\_2y\_2 + ... + a\_{ n-k } y\_{ n-k } = 0 )$

$\implies \sum\_{ i=1 }^{ n- } a_iy_i \in N(T)$

Since $\beta = \set{ x\_1, x\_2, ..., x\_{k} }$ is a basis of $N(T), \exists b\_1, b\_2, ..., b\_{k} \in F$

s.t. $\sum\_{ i=1 }^{ n-k } a_iy_i = b\_1x\_1 + b\_2x\_2 + ... + b\_{k} x\_{k}$

$-b\_1x\_1  -b\_2x\_2  ...  -b\_{k} x\_{k}  + a\_1y\_1 + a\_2y\_2 + ... + a\_{ n-k } y\_{ n-k }= 0$(*)

since $\set{x\_1, x\_2, ..., x\_{k}, y\_1, y\_2, ..., y\_{ n-k } }$ is a basis of V, it is a linearly independentset, in particular, for equation (\*) we get

$-b_1 = -b_2 = -b_k = a_1 =a_2 =...= a_{n-k} = 0$

$\therefore$ from (i) we see that$T(y_1) ... T(y_{n-k}) is a linearly independent set $

In particular, it forms a basis of $R(T)$.

$\therefore rank(T) = \dim R(T) = n-k$
recall that $nullity(T) = \dim N(T) = k and \dim V = n$

and $\dim V = n$

$\therefore rank(T) + nullity(T) = \dim V$

{{% /theorem %}}

{{% theorem name="" index="" %}}

$T: V \to W$ linearly transformation.

$T \text{ is one to one}  \iff N(T) = \set{0}$

{{% /theorem %}}

{{% remarks name="" %}}

Null space always contains at least one vector, namely, the null vector 0. $0 \in N(T)$

{{% /remarks %}}


f: X \to Y

f is called a one-to-one or injective if $\forall x_1, x_2, \in X$ and $ x_1 \neq x_2 \implies f(x_1) \neq f(x_2)$ equivalently, S one-to-one, if $\forall x_1, x_2 \in X,$

$f(x_1)=f(x_2) \implies x_1 = x_2$

equivalently f \in every y \in in ???


there exists  exactly one  pa??? x \in X s.t. f(x) = y

{{% proof index="" name="" %}}

Assume that T is one-to-one let $x\in N(T), \implies T(x) = 0 =T(0)$

since T is one-to-one, x = 0

=================

Assume that N(T) = \set{0}

let $x, y \in V, s.t. T(x) = T(y)$

$$
\implies T(x) - T(y) =0
\implies T(x-y) =0

\implies x-y \in N(T) = \set{0}
\implies x-y = 0

\implies x = y

$$

{{% /proof %}}

{{% definition name="" %}}

Let V be a vector space over F.

{{% /definition %}}