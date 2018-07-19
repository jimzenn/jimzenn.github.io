---
title: "Linear Trans"
date: 2018-07-18T11:03:48+08:00
author: "Jim Zenn"
volumes: ["MATH 115A"]
layout: "note"
issue: 2.3


---

Linear transformation, range, kernel (null space), range (image),

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\br}{\\}$

    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$ $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\C}{\mathbb{C}}$
    $\newcommand{\P}{\mathbb{P}}$
    $\newcommand{\F}{\mathbb{F}}$
    $\newcommand{\L}{\mathcal{L}}$
    $\newcommand{\B}{\beta}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{|#1|}$
    $\newcommand{\inv}[1]{#1^{-1}}$
    $\newcommand{\t#1}{\text}[1]$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$

    $\newcommand{\Vcw}[2]{\begin{pmatrix} #1 \br #2 \end{pmatrix}}$
    $\newcommand{\Vce}[3]{\begin{pmatrix} #1 \br #2 \br #3 \end{pmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \end{pmatrix}}$
    $\newcommand{\Vct}[5]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{pmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{pmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{pmatrix}}$

    $\newcommand{\vcw}[2]{\begin{matrix} #1 \br #2 \end{matrix}}$
    $\newcommand{\vce}[3]{\begin{matrix} #1 \br #2 \br #3 \end{matrix}}$
    $\newcommand{\vcr}[4]{\begin{matrix} #1 \br #2 \br #3 \br #4 \end{matrix}}$
    $\newcommand{\vct}[5]{\begin{matrix} #1 \br #2 \br #3 \br #4 \br #5 \end{matrix}}$
    $\newcommand{\vcy}[6]{\begin{matrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{matrix}}$
    $\newcommand{\vcu}[7]{\begin{matrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{matrix}}$

    $\newcommand{\Mqw}[2]{\begin{bmatrix}#1 & #2 \end{bmatrix}}$
    $\newcommand{\Mqe}[3]{\begin{bmatrix}#1 & #2 & #3 \end{bmatrix}}$
    $\newcommand{\Mqr}[4]{\begin{bmatrix}#1 & #2 & #3 & #4 \end{bmatrix}}$
    $\newcommand{\Mqt}[5]{\begin{bmatrix}#1 & #2 & #3 & #4 & #5 \end{bmatrix}}$

    $\newcommand{\Mwq}[2]{\begin{bmatrix}#1 \br #2 \end{bmatrix}}$
    $\newcommand{\Meq}[3]{\begin{bmatrix}#1 \br #2 \br #3 \end{bmatrix}}$
    $\newcommand{\Mrq}[4]{\begin{bmatrix}#1 \br #2 \br #3 \br #4 \end{bmatrix}}$
    $\newcommand{\Mtq}[5]{\begin{bmatrix}#1 \br #2 \br #3 \br #4 \br #5 \end{bmatrix}}$

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

Let $T: V \to W$and $U: V \to W$ be two linear maps.

Then $T+U: V \to W$and $cT: V \to W$for a scalar $c \in F $are also linear maps.

defined as:
$\begin{align\*}
&(T + U)(v) = T(v) + U(v), \forall u \in V \br
&(cT)(v) = cT(v), \forall u \in V \br
&(T+U)(av+w) = a(T+U)(v) + (T+U)(w)
\end{align*}$
{{% /definition %}}

{{% theorem name="" index="" %}}

Let $\L(V,W)$be the set of all linear transformations from $V \to W$.

Then $\L(V, W)$is a vector space over $F$. Under the addition and scalar multiplication defined before.

{{% proof index="" name="" %}}

exercise. Verify the 8 axioms.

{{% /proof %}}

{{% /theorem %}}

Later we will show that if $\dim V = n $and $\dim W = m $. Then $\L(V, W) M\_{m \times n}(\F)$

$V/F, W/F, \L(V,W)$, choose $W =F, \L(V,F) = {T:V \to F}, V = V*$ **Dual space** of V.

$\R^{2*} = \set{ T: \R^2 \to R }$
$T(x, y) = x$
$T(x, y) = 0$
$T(x, y) = ax+by$
$T(x, y) = T(xe\_1 + ye\_2) = xT(e\_1)+yT(e\_2)$

{{% theorem name="" index="" %}}
$T: V \to W, U:V \to W$

Let $\B$ and $\gamma$ be two ordered basis of $V$and $W$, respectively.

Then:

1. $[T+U]^\gamma\_\beta = [T]^\gamma\_\beta + [U]^\gamma\_\beta $
2. $c \in F, [cT]^\gamma\_\beta = c[T]^\gamma\_\beta$

{{% proof index="" name="" %}}
Let $\dim V = n, \dim W = m$.
$\beta = \set{ v\_1, v\_2, ..., v\_{n} }, \gamma = \set{ w\_1, w\_2, ..., w\_{m} }$

$T(v\_j) = \sum\_{ i=1 }^{m} a\_{ij}w\_i$

$[T]^\gamma\_\beta = {\Mrq{ ... a\_{1j} ... }{ ... a\_{2j} ... }{... a\_{3j} ...  }{... a\_{4j} ... }} = (a\_{ij})\_{m \times n}$

$\cup (v\_j) = \sum\_{ i=1 }^{m} b\_{ij}w\_i$
$[v]^\gamma\_\beta = (b\_{ij})\_{m \times n}$

$\begin{align\*}
  (T+U)(v\_j) &= T(v\_j) + U(v\_j) \br
  &= \sum\_{ i=1 }^{m} a\_{ij}w\_i + \sum\_{ i=1 }^{w} b\_{ij}w\_i
  &= \sum\_{ i=1 }^{m} (a\_{ij} + b\_{ij})w\_i
\end{align*}$

$\therefore,$

$\begin{align\*}
[T+U]^\gamma\_\beta &= (a\_{ij} + b\_{ij})\_{m \times n} \br
&= [T]^\gamma\_\beta + [U]^\gamma\_\beta
\end{align*}$

{{% /proof %}}

{{% /theorem %}}

{{% theorem name="" index="" %}}

$T:V \to W, U: W \to Z$

$V, W, Z$ are vector space over $F$

Then $U \circ T = UT:V \to Z$ is also a linear transformation.

{{% proof index="" name="" %}}

$x, y \in V, a \in F$

$\begin{align\*}
UT(ax+y) &= U(T(ax+y)) \br
&=(aT(x) +T(y)) \br
&=aU(T(x)) +U(T(y)) \br
&=a(UT)(x) + (UT)(y)
\end{align*}$

{{% /proof %}}

{{% /theorem %}}

{{% theorem name="" index="" %}}

Let $T, U\_1, U\_2 \in \L(V)$

Then the following holds

1. $T(U\_1 + U\_2) = TU\_1 + TU\_2$
2. $(U\_1 + U\_2)T = U\_1T + U\_2T$
3. $T(U\_1U\_2) = (TU\_1)U\_2$
4. $TI = IT = T$, where $I$ is the identity linear transformation.
5. $a(U\_1U\_2) = (aU\_1)U\_2 = U\_1(aU\_2), \forall a \in F$

{{% proof index="(1)" name="" %}}
$\begin{align\*}
&(T(U\_1 + U\_2)(x)) \br
&=T((U\_1+U\_2)(x)) \br
&=T(U\_1(x)+U\_2(x)) \br
&=T(U\_1(x))+T(U\_2(x)) \br
&=(TU\_1)(x)+(TU\_2)(x) \forall x \in V
\end{align*}$

$\therefore T \circ (U\_1 + U\_2) = TU\_1 + TU\_2$

{{% note name="" %}}

This is special to linear transformation and does not apply to general functions.

e.g. $f(x) = x^2, g\_1(x) = x^3, g\_2(x)=x^4$

{{% /note %}}

{{% /proof %}}

{{% /theorem %}}

{{% example name="multiplication why" %}}

$T: V \to W, U: W \to Z / F$

$\alpha = \set{ v\_1, v\_2, ..., v\_{n} },
\beta = \set{ w\_1, w\_2, ..., w\_{m} },
\gamma = \set{ z\_1, z\_2, ..., z\_{p} }$

and they are the ordered basis of $V, W, Z$ respectively.

$[T]^\beta\_\alpha, [U]^\gamma\_\beta, [UT]^\gamma\_\alpha$


Let $A = [U]^\gamma\_\beta$ and $B=[T]^\beta\_\alpha$.

Let $A = (a\_{ij})\_{p \times m}$ and $B = (b\_{ij})\_{m \times n}$.

We want to compute the matrix of $UT$.

We define the product of $A$ and $B$ denoted by $AB$ as the new matrix obtained from the matrix representation of $UT$ with respect to  ordered basis $\alpha$ and $\gamma$

We define $AB:= [UT]^\gamma\_\alpha$

$UT(v\_j) = \sum\_{ i=1 }^{v} (\cdot)\_{ij}z\_i$

Let $A=[U]^\gamma\_\beta$ and $B=[T]^\beta\_\alpha$

Let  $A = (a\_{ij})\_{p\times m}, U(w\_j) = \sum\_{ i=1 }^{p}a\_{ij}z\_i$(1)
and $B=(b\_{ij})\_{m \times n}$

We want to complete the matrix of $UT$


$T(v\_j) = \sum\_{ i=1 }^{m} b\_{ij} w\_i$(2)

$\begin{align\*}
&(UT)(v\_j)=U(T(v\_j)) \br
&= U( \sum\_{ i=1 }^{m}b\_{ij}w\_i ) \br
&= \sum\_{ i=1 }^{m}b\_{ij}U(w\_i) \br
&= \sum\_{ k=1 }^{m}b\_{kj}U(w\_k) \br
&= \sum\_{ k=1 }^{m}b\_{kj}( \sum\_{ i=1 }^{p} a\_{ik} z\_i ) \text{  (using 1) }\br
&= \sum\_{ i=1 }^{p} (\sum\_{ k=1 }^{m} a\_{ik}b\_{kj})z\_i
\end{align*}$

{{% /example %}}

{{% theorem name="" index="" %}}

$T:V \to W, U: W \to Z$

$\alpha, \beta, \gamma$ are ordered basis of $V, W$ and $Z$ respectively,
Then $[UT]^\gamma\_\alpha = [U]^\gamma\_\beta + [T]^\beta\_\alpha$

{{% proof index="" name="" %}}

Follws from the previous computation

{{% /proof %}}

{{% /theorem %}}

# 2.4

{{% definition name="" %}}

A linear transformation $T: V \to W$ is called invertible if

$\exists$ a function $U: W \to V$ s.t. $TU = I\_W$ and $UT = I\_V$.

{{% /definition %}}

{{% remarks name="" %}}

1. $T$ is invertible $\iff T$ is bijective
2. Let $T\_1: V \to W, T\_2: W \to V$ are both invertible, then $T\_2T\_1$ is also invertible and $(T\_2T\_1)^{-1} = (T\_1)^{-1}(T\_2)^{-1}$
3. If $T: V \to V/F$ is invertible, then $(T^{-1})^{-1} = T$
4. A linear transformation $T:V \to W$ is invertible $\iff$ $N(T) = {0}$ and $R(T)= W$

{{% /remarks %}}

{{% theorem name="" index="" %}}

If $T:V \to W$ is an invertible linear transformation, and $T^{-1}: W \to V$  is its inverse, then $T^{-1}$ is also linear.

{{% proof index="" name="" %}}
$w\_1, w\_2 \in W, a \in F$

$\inv{T}(aw\_1 + w\_2) = $

$\because T: V \to W$ is invertible, $T$ is bijective, in particle, subjective.

$\therefore v\_1, v\_2 \in V$ s.t.

$T(v\_1)= w\_1  \implies aw\_1 = aT(v\_1) = T(av\_1)$
$T(v\_2)= w\_2  \implies aw\_1 +w\_2 = T(av\_1) + T(v\_2) = T(av\_1 + v\_2)$

$\inv{T}(aw\_1 + w\_2) = \inv{T}(T (av\_1 + v\_2) = av\_1 + v\_2$

$\because T$ is bijective and $T(u\_1) = w\_1$ and $T(v\_2) = w\_2$

We have $v\_1 = \inv{T}(w\_1)$, $v\_2 = \inv{T}(w\_2)$

{{% /proof %}}

{{% /theorem %}}


