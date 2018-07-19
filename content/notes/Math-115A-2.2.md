---
title: "The Matrix Representation of a Linear Transformation"
date: 2018-07-16T11:03:48+08:00
author: "Jim Zenn"
volumes: ["MATH 115A"]
layout: "note"
issue: 2.2


---

Linear transformation, range, kernel (null space), range (image),

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

{{% theorem name="" index="" %}}
<u>Finite-dimensional</u> and $\dim V = \dim W = n$, then the following are all equivalent.

1. $T$ is one-to-one
2. $T$ is onto
3. $rank{T} = \dim V$

{{% proof index="" name="" %}}
(i) \implies (ii)

Assume $T$ is one-to-one.

$\implies N(T) = {0}$

$\implies nullity(T) = \dim N(T) = 0$

Now by the rank-nullity theorem, $nullity(T) + rank(T) = \dim V$

$\implies rank(T) = \dim V$

$\dim R(T) = \dim W$

$\because \dim V = \dim W$

$\therefore R(T) \subseteq W$

We have, $R(T)  = W$

FC. $range(T) = W$ T is onto

(ii) \implies (iii)

Assume that T is onto,
i.e. $R(T) = W$

i.e. $rank(T) = \dim W = \dim V$

(iii) \implies (i)

Assume that $rank(T) = \dim V$

$nullity(T) + rank(T) = \dim V$

{{% /proof %}}

{{% /theorem %}}

{{% theorem name="" index="" %}}

Let $V$ and $W$ be two vector space over field F. Let $\dim V = n $(not infinity) and $\set{ x\_1, x\_2, ..., x\_{n} }$ is a basis of $ V_0 $ Let $\set{ w\_1, w\_2, ..., w\_{n} }$ be a set of <u>any vectors</u> in $W$. Then there exists a <u>unique</u> linearly transformation $T: V \to W$ s.t. $T(x_i) = w_i, \forall i = 1,2, ..., n$.

Analysis:

$\B = \set{ x\_1, x\_2, ..., x\_{n} } \subset V \to W \supset \gamma = \set{ w\_1, w\_2, ..., w\_{n} }$

$Want to define: T: V \to W,$ s.t. $T(x_1) = w_1, T(x_2) = w_2, T(x_3) = w_3$

T: $\B \subseteq V \to \gamma \subseteq W$

You want to extend $T$ to $V \to W$

* Define a linearly transformation $\R^3$ to $\R^2$ whose image is the line $y = x$ in $\R^2$.

$y = x$

$w = \spa{ \set{ (1, 1) } }$

$T: \R^3 \to \R^2$

$\B = \set{ e\_1, e\_2, e\_{3} }$

Define $T(e_1) = T(e_2) = T(e_3)$


$R(T) = \spa{ T(e_1), T(e_2) T(e_3) } = \spa{ (1, 1) }$

$t(a, b, c) = t( a\_1e\_1 + a\_2e\_2 + a\_{3} e\_{3} )$

$= aT(e_1) + bT(e_2) + c_T(e_3) = (a+b+c)(1,1)$

{{% proof index="" name="" %}}

Since $x \in V$ be an arbitrary vector. We need to know $T(x)=?$.

Since $\set{ x\_1, x\_2, ..., x\_{n} }$ is a basis,

$\exists$ unique scalars $a\_1, a\_2, ..., a\_{n}$ s.t. $x = \sum\_{ i=1 }^{n} a_i x_i$

We define $T(x)$ as $T(x) := \sum\_{ i=1 }^{n} a_i w_i$(\*)

$T$ is linearly transformation.

{{% proof index="" name="" %}}

$x, y \in, c \in F$

$\because \set{ x\_1, x\_2, ..., x\_{n} }$ is a basis of $V\exists a\_1, a\_2, ..., a\_{n}$ and $b\_1, b\_2, ..., b\_{n} \in F$, s.t.

$x = \sum\_{  }^{  } a_i x_i$
$x+y = \sum\_{  }^{  } b_i x_i$

by definition
$T(x+y) = \sum\_{ i=1 }^{n}(a_i + b_i) w_i$
$= c \sum\_{ i=1 }^{n} a_i w_i + \sum\_{ i=1 }^{n} b_iw_i$

so $T$ is a linearly transformation.

need to choose $T(x_i) = w_i \forall i$

$x_i = 0x\_1 + 0x\_2 + ... + 0 x\_{ i-1 } + 1x_i + a\_1x\_i+1 + a\_2x\_i+2 + ... + a\_{n} x\_{n}$.

by definition (\*), $T(x_i) = 0w\_1 + 0w\_2 + ... + 0 w\_{ i-1 } + 1w_i + 0w\_i+1 + 0w\_i+2 + ... + 0 w\_{n}$

Remark: Defining T from basis to entire V is called extending T linearly.

{{% /proof %}}

{{% proof index="" name="uniquness" %}}

Assume that: there is another linearly transformation $U: V \to W$ s.t. $U(n_i) = w_i, v_i = 1,2, ..., n$.

We need to show that $U(x) = T(x) \forall x in V$

since $\set{ x\_1, x\_2, ..., x\_{n} }$ is a basis of V,

$\exists c\_1, c\_2, ..., c\_{n} \in F$ s.t. $x = \sum\_{ i=1 }^{n} c_ix_i$

Then $U(x)  = U( \sum\_{ i=1 }^{n} c_ix_i ) = \sum\_{ i=1 }^{n} U(x_i) = \sum\_{ i=1 }^{n} c_iw_i = T( \sum\_{ i=1 }^{n} c_ix_i ) = T(x)$

{{% /proof %}}

{{% /proof %}}

{{% /theorem %}}

{{% corollary name="" index="" %}}

$\dim V = n$

let $\set{ x_i, ..., x_N }$ be a basis of $V$.

and  $\set{ w\_1, w\_2, ..., w\_{n} }$ any subset in $W$.

If $T: V \to W$ and $U:V \to W$ and  two linearly transformation s.t.

$T(x_i) = w_i$ and $U(x_i) = w_i \forall i = 1, ..., n$

i.e. $T(x_i) = U(x_i), \forall i = 1, ..., n$

Then $T(x) = U(x) \forall x \in V$

i.e. $T$ and $U$ are the same linearly transformation.

{{% remarks name="" %}}

If two linearly transformation from $V$\to $W$ coincide on a basis of V, then they coincide everywhere else.

{{% /remarks %}}

{{% proof index="" name="" %}}

It follows from the uniqueness of the previous theorem.

{{% /proof %}}

{{% /corollary %}}

Find a linearly transformation from $\R^3$ to $\R^2$ s.t. $T(1, 0, 0) = (-1, 5)$ and $T(1,1, 0) = (2,3)$

$\set{ (1, 0, 0) , (1,1, 0), (0, 0, 1)}$ is a basis of $\R^3$

choose $T((0, 0, 1))$ to any vector for example $T((0,0,1)) = (0, 0, 0)$.

$(x, y , z) \in R^3$


$T(x,y,z) = $
$(x,y,z) = (x-y) e_1 + ye + ze_3$
$= (x-y)(1, 0, 0) + y (1, 1, 0) + z(0, 0, 1)$
$T(x, y, z) = (x-y)(-1,5) +y(2,3) + 2(0, 0)$
$=(-x + y+2y, 5x -5y + 3y) = (-x+3y, 5x-2y)$


An **ordered basis** of V is a basis of V with preassigned order on the vectors.

e.g. $\set{ 1st vec, 2nd vec }$


{{% example name="$\R^2 $" %}}

$\B = \set{ e_1, e_2 }$ is called the standard ordered basis of $\R^2$

$\gamma = \set{ e_1, e_2 }$ is a different ordered basis than $\B$

{{% /example %}}

{{% definition name="" %}}

Let $\B$ = \set{ u\_1, u\_2, ..., u\_{n} } be an ordered basis of a finite-dimensional vector space, V/F. For an arbitrary vector. $x \in V, \exists unique scalars a\_1, a\_2, ..., a\_{n} \in F$ s.t. x= a\_1u\_1 + a\_2u\_2 + ... + a\_{n} u\_{n}.

Then the column vectors ( a\_1, a\_2, ..., a\_{n} )  \in F^n is called the coodinate of x with respect to the ordered basis $\B$ and write $[x]\_\B = ( a\_1, a\_2, ..., a\_{n} )$
{{% /definition %}}

{{% example name="$\P_2(x)/ \R$" %}}

$\B = \set{ 1, x, x^2 }$ is an ordered basis

$f(x) = -5x^2 + x - \frac{1}{2} = -\frac{1}{2} \cdot 1 + 1 \cdot x - 5 \cdot x^2$

$[f(x)]_\B = (- \frac{1}{2}\ 1\ -5)$

{{% /example %}}

{{% definition name="" %}}

Let $T: V \to W  dim V = n$ and $dim W = m$

Let $\B = \set{ x\_1, x\_2, ..., x\_{n} }$ and $\gamma = \set{ w\_1, w\_2, ..., w\_{m} }$ are ordered basis of $V$ and $W$ respectively.

Now choose $x_j \in \B$ and consider $T(x_j)$ since $\gamma$ is a basis of $W \exists $ scalars $ a\_1j, a\_2j, ..., a\_{ mj } \in F$ s.t. $T(x_j) = a\_1jw\_1 + a\_2jjw\_2 + ... + a\_{ mj } jw\_{m}= \sum\_{ i=1 }^{m} a_{ij}w_i$

$[T(x_j)]\_\gamma = ( a\_1j, a\_2j, ..., a\_{ mj } )$

Let A be a matrix s.t. its columns are the coodinates vector $[T(x_1)]_\gamma, [T(x_2)]_\gamma, [T(x_3)]_\gamma$


i.e. A = ( ah... so hard )


This matrix $A$ is called the matrix representation fo $T$ with regard to the ordered basis \B and \Gamma.

{{% /definition %}}

{{% example name="$T: \R^3 \to \R^2$" %}}

$T(x, y, z) = (2x-y, x+z)$

$\B = \set{ e_1, e_2, e_3)$, and $\gamma = \set{ e_1, e_2 }$

$T(e_1) = (2, 1) = 2e_1' +1 e_1'$
$T(e_2) = (-1, 0) = -1e_1' + 0e_1'$
$T(e_3) = (0, 1) = -0e_1' + 1e_1'$

{{% /example %}}

{{% example name="" %}}

$\B' = \set{ (1,-1, 0), (1,0, 3), (1,1,-2) }$

T(x, y, z) = (2x-y, x + z) = \set{ e_1, e_2 } = \set{ (1,0), (0,1) }

T(e_1'') = (3,1)  = 3e_1' + 1e_2'
T(e_2'') = (2,4)  = 2e_1' + 4e_2'
T(e_3'') = (1,-1) = 1e_1' + 1e_2'


{{% /example %}}

