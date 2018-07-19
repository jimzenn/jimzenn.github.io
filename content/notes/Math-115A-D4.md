---
title: "Discussion"
date: 2018-07-17T11:03:48+08:00
author: "Jim Zenn"
volumes: ["MATH 115A"]
layout: "note"
issue: D4

---

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\br}{\}$

    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\C}{\mathbb{C}}$
    $\newcommand{\P}{\mathbb{P}}$
    $\newcommand{\F}{\mathbb{F}}$
    $\newcommand{\B}{\beta}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{{#1}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{|#1|}$
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
    $\newcommand{\t#1}{\text}[1]$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$

    $\newcommand{\Vcw}[2]{\begin{pmatrix} #1 \br #2 \end{pmatrix}}$
    $\newcommand{\Vce}[3]{\begin{pmatrix} #1 \br #2 \br #3 \end{pmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \end{pmatrix}}$
    $\newcommand{\Vct}[5]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{pmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{pmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{pmatrix}}$

    $\newcommand{\Mqw}[2]{\begin{bmatrix}#1 & #2 \end{bmatrix}}$
    $\newcommand{\Mqe}[3]{\begin{bmatrix}#1 & #2 & #3 \end{bmatrix}}$
    $\newcommand{\Mqr}[4]{\begin{bmatrix}#1 & #2 & #3 & #4 \end{bmatrix}}$
    $\newcommand{\Mqt}[5]{\begin{bmatrix}#1 & #2 & #3 & #4 & #5 \end{bmatrix}}$

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

{{% example name="midterm 4b" %}}

$\set{ W\_i| W\_i \leq V, i \in I }$

Collection of infinite many dinstinct subspaces of V.

$W\_i \cap W\_j = \set{0}$ for $i \neq j, I$ infinite indexing set.

$\cup\_{i \in I} W\_i$ is NOT a subspace of $V\_i$.

Counter example.

$W\_i = { (x,y) | y = ix, i \in R }$


{{% /example %}}

{{% example name="HW 3 2.1.14" %}}

$V, W$ vector space, $T: V \to W linear$

(a) T one-to-one $\iff$ T carries independent subsets of $V$ onto linearly independent subsets of $W$.
note Do not assume $S$ is finite.

$T\_i$ one-to-one  if $T\_x = T\_y$ implies $x = y$.

$T\_i$ onto if
for each $z \in W$ there is $x$ in $V$ s.t. $T\_x = z$.

1. $T one-to-one \iff N(T) = {0}$
2. $T onto \iff R(T) = W$

{{% /example %}}

{{% example name="2.1.37" %}}

$T:V \to W$ T not a linear transformation, additive if T(x+y) = T(x) + T(y).

$V, W$ vector space over P.

Then any additive function T is a linear transformation.

we have to prove $T(x) = cTx \forall c \in R, x \in V$.

{{% proof index="step 1" name="" %}}

(\*) true for any $c \in N$

$c = 1$ trivial $ T(1x) = 1Tx $

$ c=2,  T(2x) = T(x + x) = Tx + Tx = 2Tx$

induction, assume (\*) is true for some $ n \in N\_1 $

$T(nx) = nTx$

$T((n+1) x) = T(nx + x) = T(nx) + Tx$

$nTx +Tx = (n+1) Tx$

By induction it is true $\forall c \in N$

{{% /proof %}}

{{% proof index="step 2" name="" %}}

$ T(0) = T (0) = T(0) + T(0)$
$\implies T(0) = 0$

$T(0x) = T(0) = 0 = 0 \cdot T(x)$, true for $c = 0$

$0 = T(o) = T(x+(-x)) = T(x) + T(-x)$

$\implies T(-x) = - T(x)$

if $c \in Z, c < 0$ then $-c \in N$


$T(cx) = -T((-c) x) = -(-c) T(x) = cT(x)$(step 1)

$(\*) is true for c \in Z$

{{% /proof %}}

{{% proof index="step 3" name="" %}}

$c \in \R, c = \frac{p}{q} p \in Z q \in N$

$T(px) = pT(x) $(step 2)

$T(q \frac{p}{q} x ) = q \cdot T( \frac{p}{q} x )$(step 2)

$c = \frac{p}{q} p \in Z, q \in N$

$pT(x) = qT( \frac{p}{q}x ) \implies T( \frac{p}{q} x ) = \frac{p}{q}T(x)$

{{% /proof %}}

{{% /example %}}

{{% example name="2.2.16" %}}

$V, W$ vector space, $\dim V = \dim V$,
$T: V \to W$ linear,
Show that there exists ordered basis $\B, \gamma$ for $V, W$ s.t. $[T]^\gamma\_\beta$ is a diagonal matrix.

Recall

$\B = \set{ v\_1, v\_2, ..., v\_{n} } , \gamma = \set{ w\_1, w\_2, ..., w\_{m} }$

$T(v\_i) = \sum\_{ i=1 }^{m} a\_{ij} W\_i$

$A= (a\_{ij}) = [T]^\gamma\_\beta$

{{% proof index="step 1" name="" %}}
let $k = \dim R(T) \leq n
find a basis \set{ w\_1, w\_2, ..., w\_{k} } of $R(T)$

{{% /proof %}}

{{% proof index="step 2" name="" %}}

For each  $i \leq i \leq k$

there is $V\_i \in V$ s.t. $TV\_i = W\_i$ since $W \in R(T)$.

{{% /proof %}}

{{% proof index="step 3" name="" %}}

check \set{ V\_1, V\_2, ..., V\_{k} } is linearly independent. ( use the fact that $\set{ w\_1, w\_2, ..., w\_{k} }$  is linear independent)

{{% /proof %}}

{{% proof index="step 4" name="" %}}

$n = dimV = \dim N(T) + \dim R(T)$

$\implies N(T) = n - k$


choose basis of $N(T) \leq V, \set{ V\_{k+1}, ..., V\_n }$

{{% /proof %}}

{{% proof index="step 5" name="" %}}

Define $\beta = \set{ v\_1, v\_2, ..., v\_{n} }$

check this is a basis of $V$.

enough to prove that $ V\_1, V\_2, ..., V\_{n} is linearly independent. Why? $

{{% /proof %}}

{{% proof index="step 6" name="" %}}

Use replacement theorem to extend $\set{ w\_1, w\_2, ..., w\_{k} }$ to a basis $\set{ w\_1, w\_2, ..., w\_{n} }$ of $W$.

{{% /proof %}}

{{% proof index="step 7" name="" %}}

define $\gamma = \set{ w\_1, w\_2, ..., w\_{n} }$

prove that $ [T]^\gamma\_\beta $ is diagonal.

{{% /proof %}}

{{% /example %}}


{{% example name="2.2.13 extra" %}}
$V, W$ is $T, U: V \to W$
$T, U $ nonzero linear transformation,
If $R(T) \cap R(U) = \set{0}$ prove:
$\set{ T, U }$ is a linearly independent subset of $L(V, W)$


Note $L(V, W)$ is the collection of all linear transformation from $V$ to $W$.

{{% proof index="" name="" %}}
Assume $ aT + bU = 0 $ for some $a,b$

This means $aT(x) + bU(x) = 0, \forall x \in V$

To prove independent, we have to prove that $a = b = 0 $
suppose not, without loss of generality, assume $a \neq 0$

If $b = 0$, then $aT=0 \to T =0$ contradiction.

(T, V are non-zero maps).

so $a, b \neq 0$.

{{% /proof %}}

T is a non-zero map

so $\exists v \in V s.t. T(v) \neq 0$

$a T(v) + bU(v) = 0$

$\implies U(v) = - \frac{a}{b} T(v)$

if $T(v) = W, w \in range(T)$

$Range(T)$ is subspace, $- \frac{a}{b} w \in Range(T) $

$U(v) = - \frac{a}{b} w \in Range(V)$

{{% /example %}}
