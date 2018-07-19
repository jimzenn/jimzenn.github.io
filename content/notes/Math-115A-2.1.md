---
title: "Linear Transformation"
date: 2018-07-11T11:03:48 + 08:00
author: "Jim Zenn"
volumes: ["MATH 115A"]
layout: "note"
issue: 2.1


---

Linear transformations (linear maps) and their basic properties, identity transformation, zero transformation, kernel (null space), range (image), theorem 2.1, nullity, rank.

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\br}{\\}$

    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\C}{\mathbb{C}}$
    $\newcommand{\P}{\mathbb{P}}$
    $\newcommand{\F}{\mathbb{F}}$
    $\newcommand{\L}{\mathcal{L}}$
    $\newcommand{\B}{\beta}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{otherwise}}$
    $\newcommand{\if}{\text{if}}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{|#1|}$
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
    $\newcommand{\t}[1]{\text{#1}}$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\rank}[1]{\text{rank}(#1)}$

    $\newcommand{\Vcw}[2]{\begin{pmatrix} #1 \br #2 \end{pmatrix}}$
    $\newcommand{\Vce}[3]{\begin{pmatrix} #1 \br #2 \br #3 \end{pmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \end{pmatrix}}$
    $\newcommand{\Vct}[5]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{pmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{pmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{pmatrix}}$

    $\newcommand{\Mqw}[2]{\begin{bmatrix} #1 & #2 \end{bmatrix}}$
    $\newcommand{\Mqe}[3]{\begin{bmatrix} #1 & #2 & #3 \end{bmatrix}}$
    $\newcommand{\Mqr}[4]{\begin{bmatrix} #1 & #2 & #3 & #4 \end{bmatrix}}$
    $\newcommand{\Mqt}[5]{\begin{bmatrix} #1 & #2 & #3 & #4 & #5 \end{bmatrix}}$

    $\newcommand{\Mwq}[2]{\begin{bmatrix} #1 \br #2 \end{bmatrix}}$
    $\newcommand{\Meq}[3]{\begin{bmatrix} #1 \br #2 \br #3 \end{bmatrix}}$
    $\newcommand{\Mrq}[4]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \end{bmatrix}}$
    $\newcommand{\Mtq}[5]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{bmatrix}}$

    $\newcommand{\Mqw}[2]{\begin{bmatrix} #1 & #2 \end{bmatrix}}$
    $\newcommand{\Mwq}[2]{\begin{bmatrix} #1 \br #2 \end{bmatrix}}$
    $\newcommand{\Mww}[4]{\begin{bmatrix} #1 & #2 \br #3 & #4 \end{bmatrix}}$
    $\newcommand{\Mqe}[3]{\begin{bmatrix} #1 & #2 & #3 \end{bmatrix}}$
    $\newcommand{\Meq}[3]{\begin{bmatrix} #1 \br #2 \br #3 \end{bmatrix}}$
    $\newcommand{\Mwe}[6]{\begin{bmatrix} #1 & #2 & #3\br #4 & #5 & #6 \end{bmatrix}}$
    $\newcommand{\Mew}[6]{\begin{bmatrix} #1 & #2 \br #3 & #4 \br #5 & #6 \end{bmatrix}}$
    $\newcommand{\Mee}[9]{\begin{bmatrix} #1 & #2 & #3 \br #4 & #5 & #6 \br #7 & #8 & #9 \end{bmatrix}}$
  {{< /raw >}}
</div>

{{% definition name="" %}}

$V/F$,$W$is a vector space over field$F$.

A **linear transformation** (or **linear map**) $T:V \to W$ is a function which satisfies the following properties:

1. $T(v\_1 + v\_2) = T(v\_1) + (v\_2), \forall v\_1, v\_2 \in V.$
2. $T(cv) = cT(v), \forall v \in V, c \in F.$

{{% /definition %}}

{{% example name="" %}}
$T: \R^3 \to \R^2, T(a\_1, a\_2, a\_3) = (2a\_1-a\_3, a\_2 - a\_1).$

$v\_1 = (a\_1, a\_2, a\_3), v\_2 = (b\_1, b\_2, b\_3).$

$\begin{align\*}
  &T((a\_1, a\_2, a\_3)  + (b\_1, b\_2, b\_3)) \br
  &=T(a\_1 + b\_1, a\_2 + b\_2, a\_3 + b\_3) \br
  &=(2(a\_1 + b\_1) - (a\_3 + b\_3), (a\_2 + b\_2) - (a\_1 + b\_1))
\end{align*}$

$T(c(a\_1, a\_2, a\_3)) = T((ca\_1, ca\_2, ca\_3)) = (c(2a-a\_3), c(a\_2 - a\_1))$

$T((a\_1, a\_2, a\_3)) = (2a\_1-a\_3, a\_2 - a\_1)$

$T((b\_1, b\_2, b\_3)) = (2b\_1-b\_3, b\_2 - b\_1)$

$\begin{align\*}
  &T((a\_1, a\_2, a\_3)) + T((b\_1, b\_2, b\_3)) \br
  &= (2a\_1-a\_3, a\_2 - a\_1) + (2b\_1-b\_3, b\_2 - b\_1) \br
  &= ...
\end{align*}$


{{% /example %}}

{{% example name="reflection about x-axis" %}}

$T: \R^2 \to \R^2, T ((a,b)) = (a, -b)$

{{% /example %}}

{{% example name="Rotation" %}}

$T: \R^2 \to \R^2, T(P)=P'. P=(a,b).$

$T(P) = (a\cos \theta - b \sin \theta, a \sin \theta + b \cos \theta)$

{{% /example %}}

{{% properties name="Basic properties of linear transformation" %}}

1. If $T: V \to W$ a linear transformation,

  - $T(0) = 0$

  - $T(v\_1 - v\_2) = T(v\_1) - T(v\_2)$

2. $T: V \to W$is a linear transportation$\iff T(cv\_1 + v\_2) = c T(v\_1) + T(v\_2), \forall v\_1, v\_2 \in V, \forall c \in F$

{{% proof index="1" name="" %}}

$T(0) = T(0 + 0) = T(0) + T(0) \implies T(0) + 0 = T(0) + T(0)$

By cancellation law, $0 = T(0)$.

$T(v\_1 - v\_2) = T(v\_1 + (-v\_2))$.

{{% /proof %}}

{{% /properties %}}

{{% example name="" %}}

$\R^2 \to \R^2$.

$T(x, y) = T(x + y, x-y + 1)$ is not a linear transformation.

$T(x, y) = (x, \abs{y})$ is not a linear transformation.

{{% /example %}}

{{% example name="" %}}

$T: M\_{m \times n}( \R ) \to M\_{n \times m} ( \R)$.

$T(A) = A^t$ is a linear transformation.

{{% /example %}}

{{% example name="" %}}
$T: \P\_n(x) \to \P\_{n-1}(x)$.

$T(f(x)) = f'(x)$ is a linear transformation.

$\begin{align\*}
T(cf(x) + g(x)) &= (cf(x) + g(x))' \br
&= cf'(x) g'(x) \br
&= cT(f(x)) + T(g(x))
\end{align*}$

{{% /example %}}

{{% example name="" %}}

$T:\R^2 \to \R^3$.

$T(a\_1, a\_2) = (a\_1, a\_2, 0)$

{{% /example %}}

{{% definition name="Identity transformation" %}}

$I: V \to V. I(v) = v, \forall v \in V$.

{{% /definition %}}

{{% definition name="zero transformation" %}}

$T: V \to W. T(x) = 0, \forall x \in V$.

{{% proof index="" name="" %}}
$T(cx + y) = 0$.
$T(cx) + T(y) = 0 + 0 = 0$.
{{% /proof %}}

{{% /definition %}}


{{% definition name="kernel (null space), range (image)" %}}

$T: V \to W$ is a linear transformation.

The **kernel** (or **null space**) of $T$ denoted by $N(T)$, and is defined as:

$$N(T) = \set{v \in V \mid T(v) = 0}$$

The **range** (or **image**) of $T$ is denoted by $R(T)$, and is defined as:

$$R(T)= \set{T(x) \in W \mid x \in V}$$

{{% /definition %}}


{{% theorem name="$N(T) \leq V$" index="2.1" %}}

$T: V \to W$ is a linear transformation.

$N(T)$ is a subspace of $V$, and $R(T)$ is a subspace of $W$.

{{% proof index="" name="$N(T) \leq V$" %}}

$x, y \in N(T)$, then $T(x) = 0, T(y) = 0$, need to show that $x + y \in N(T)$.

$T(x + y) = T(x) + T(y) = 0 + 0 = 0$

$\therefore x + y \in N(T)$.

$x \in N(T) \implies T(x) = 0, c \in F$.

$T(cx) = cT(x) = c0 = 0$

$\therefore cx \in N(T)$.

$N(T)$ is a subspace of $V$.

{{% /proof %}}

{{% proof index="" name="$R(T) \leq W$" %}}

$w\_1, w\_2 \in R(T) \implies \exists x\_1, x\_2 \in V, s.t.$

$T(x\_1) = w\_1, T(x\_2) = w\_2$.

$w\_1 + w\_2 = T(x\_1) + T(x\_2) = T(x\_1 + x\_2)$.

$\therefore (w\_1 + w\_2) \in R(T)$.

$w \in R(T) \implies \exists x \in V s.t. T(x) = w$.

$cw = cT(x) = T(cx)$.

$\therefore cw \in R(T)$.

{{% /proof %}}

{{% /theorem %}}

{{% definition name="Nullity, Rank" %}}

$T:V \to W$ is a linear transformation.

The dimension of the null space $N(T)$ is called the **nullity** of $T$ and is denoted by $\nullity{T}$.

$$\nullity{T} := \dim{N(T)}$$

The dimension of the image $R(T)$ is called the **rank** of $T$ and is denoted by $\rank{T}$.

$$\rank{T} := \dim{R(T)}$$

{{% /definition %}}

{{% example name="$A\_{m \times n}$" %}}

$T: \R^n \to \R^m$. $T(x) = Ax, \forall x \in \R^n$.

$\begin{align\*}
T(cx + y) &= A(cx + y) \br
&= A(cx) + Ay \br
&= cAx + Ay \br
&= cT(x) + T(y)
\end{align*}$

$\rank{A} = \rank{T}$.

{{% /example %}}


{{% theorem name="" index="2.2" %}}

$T:V \to W$ is a linear transformation.

If $\B = \set{ x\_1, x\_2, ..., x\_{n}}$ is a basis of $V\_1$, then $R(T) = \spa{ T(x\_1), T(x\_2), ... T(x\_n) }$.

{{% /theorem %}}


{{% theorem name="Rank-nullity Theorem" index="2.3" %}}

Let $T: V \in W$ be a linear transformation.

If $V$ is a finite-dimensional vector space, then

$$\begin{align\*}
\dim V &= \rank{T} + \nullity{T} \br
&=\dim R(T) + \dim N(T)
\end{align*}$$

{{% proof index="" name="" %}}
Let $\dim N(T) = k, N(T) \leq V$.

Let $\B = \set{ x\_1, x\_2, ..., x\_{k} }$ be a basis of $N(T)$,

Since $N(T) \leq V$, $\B$ can be extended to a basis of $V$ , saying $\gamma  = \B \cup \set{ y\_1, y\_2, ..., y\_{ n-k } }$, where $n = \dim V$.

$\gamma = \set{ x\_1, ..., x\_k, y\_1, ..., y\_{n-k} }$is a basis of $V$.

Need to prove $\set{ T(v\_{k + 1}), T(v\_{k + 2}), ..., T(v\_{n}) }$ is a basis for $R(T)$.


Let $w in R(T)$

Then $\exists x \in v s.t. T(x) = w$

Since $\beta$ is a basis of $V \exists c\_1, c\_2, ..., c\_{n} \in F s.t. x = \sum\ c\_ix\_i$

Then $T(x) = T( \sum\_{ i=1 }^{n} c\_ix\_i) = \sum\_{ i=1 }^{n} c\_i T(x\_i)$
$i.e. \sum\_{ i=1 }^{n} c\_i T(x\_i)$

Then $R(T) = \spa{ T(x\_i), ..., T(x\_k), T(y\_1), ... , T(y\_{1-k}) } = \spa{ T(y\_1), ..., T(y\_{n-k}) }$

Need to prove this set is acutally linearly independent.

Consider the equation, $a\_1T(y\_1) + ... + a\_{n-k}T(y\_{n-k}) = 0$

$\implies T( a\_1y\_1 + a\_2y\_2 + ... + a\_{ n-k } y\_{ n-k } = 0 )$

$\implies \sum\_{ i=1 }^{ n- } a\_iy\_i \in N(T)$

Since $\beta = \set{ x\_1, x\_2, ..., x\_{k} }$is a basis of$N(T), \exists b\_1, b\_2, ..., b\_{k} \in F$

s.t. $\sum\_{ i=1 }^{ n-k } a\_iy\_i = b\_1x\_1 + b\_2x\_2 + ... + b\_{k} x\_{k}$

$-b\_1x\_1  -b\_2x\_2  ...  -b\_{k} x\_{k}  + a\_1y\_1 + a\_2y\_2 + ... + a\_{ n-k } y\_{ n-k }= 0$(*)

since $\set{x\_1, x\_2, ..., x\_{k}, y\_1, y\_2, ..., y\_{ n-k } }$ is a basis of V, it is a linearly independentset, in particular, for equation (\*) we get

$-b\_1 = -b\_2 = -b\_k = a\_1 =a\_2 =...= a\_{n-k} = 0$

$\therefore$from (i) we see that$T(y\_1) ... T(y\_{n-k}) is a linearly independent set $

In particular, it forms a basis of $R(T)$.

$\therefore \rank{T} = \dim R(T) = n-k$
recall that $\nullity{T} = \dim N(T) = k and \dim V = n$

and $\dim V = n$

$\therefore \rank{T} + \nullity{T} = \dim V$

{{% /proof %}}

{{% /theorem %}}

{{% theorem name="" index="" %}}

$T: V \to W$ linear transformation.

$T \text{ is one to one}  \iff N(T) = \set{0}$

{{% /theorem %}}

{{% remarks name="" %}}

Null space always contains at least one vector, namely, the null vector 0. $0 \in N(T)$

{{% /remarks %}}


f: X \to Y

f is called a one-to-one or injective if $\forall x\_1, x\_2, \in X$and$ x\_1 \neq x\_2 \implies f(x\_1) \neq f(x\_2)$equivalently, S one-to-one, if$\forall x\_1, x\_2 \in X,$

$f(x\_1)=f(x\_2) \implies x\_1 = x\_2$

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
