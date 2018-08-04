---
title: "Discussion"
date: 2018-07-31T11:03:48+08:00
menuTitle: "Linear Algebra"
volumes: ["D"]
layout: "note"
issue: 6

---

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
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{| #1 |}$
    $\newcommand{\norm}[1]{\left\lVert#1\right\rVert}$
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
    $\newcommand{\t}[1]{\text{ #1 }}$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
    $\newcommand{\d}{\text d}$
    $\newcommand{\limu}[2]{\underset{#1 \to #2}\lim}$
    $\newcommand{\inv}[1]{{#1}^{-1}}$
    $\newcommand{\inner}[2]{\langle #1, #2 \rangle}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\rank}[1]{\text{rank}(#1)}$
    $\newcommand{\tr}[1]{\text{tr}(#1)}$
    $\newcommand{\Re}[1]{\text{Re}(#1)}$
    $\newcommand{\Im}[1]{\text{Im}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$

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

{{% example name="6.1.19a" %}}
$\norm{ x \pm y } ^2 = \norm{ x }^2 \pm 2\Re {\inner{ x }{ y }} + \norm{ y }^2 $

$z = x + iy \in \C, x, y \in \R $

$\overline{ z } = x - iy $

$z + \overline{  z } = 2x = 2 \Re{z} $

$\begin{align\*}
\norm{ x+y }^2 &= \inner{ x+y }{ x+y } = \inner{ x }{ x } + \inner{ y }{ x } + \inner{ x }{ y } + \inner{ y }{ y } \br
&= \norm{ x }^2 + \inner{ y }{ x } + \inner{ x }{ y } + \norm{ y }^2 \br
&= \norm{ x }^2 + \overline{ \inner{ x }{ y }} + \inner{ x }{ y }+ \norm{ y }^2 \br
&= 2 \Re{\inner{ x }{ y }}
\end{align\*}$

$\norm{ x-y }^2 = \norm{ x }^2 - 2 \Re \inner{ x }{ y } + \norm{ y }^2 $

{{% /example %}}

{{% example name="6.1.19b" %}}

$\abs{ a } \leq b \iff -b \leq a \leq b$

It is sufficient to show $- \norm{ x - y } \leq \norm{ x } - \norm{ y } \leq \norm{ x - y } $

using (1) $\norm{ y } \leq \norm{ x } + \norm{ x - y } $
(2) $\norm{ x } \leq \norm{ y } + \norm{ x - y } $

$\norm{ y } \leq \norm{ x } + \norm{ x - y } = \norm{ y - x } $

$y = x + (y - x) $

$\iff \norm{ x + (y-x)} \leq \norm{ x } + \norm{ y-x } $

{{% /example %}}

{{% example name="" %}}

$V = P\_2(\R) = \set{ a\_0 + a\_1x + a\_2x^2 \mid a\_0, a\_1, a\_2 \in R }$

$f, g \in P\_2(\R)$

$\inner{ f }{ g } := \int\_{ 0 }^{ 1 } f(t)g(t) \d t $

Find an orthonormal basis of $P\_2(\R) $

{{% /example %}}

{{% example name="" %}}

$V = \R^3, standard inner product $

$\inner{(a\_1, a\_2, a\_3)}{(b\_1, b\_2, b\_3)  = a\_1b\_1 + a\_2b\_2 +  a\_{ 3 }b\_{ 3 }} $

$S = \set{(1,2,3), (4, 5,6), (7,8,9)} $

{{% /example %}}

{{% example name="" %}}

$W$ is finite-dimensional vector space, $U, V $ are subspaces of  $W $.
Define $U+V = \set{ u+v | u \in U, v \in V } $

(a) $\dim(U+V) \leq \dim U + \dim V$
(you can just assume $U + V$ is a subspace)

{{% proof index="" name="" %}}

$W $ is finite-dimensional vector space $\implies$ finite dimensional vector space.

Let $\dim U = n, \dim V = m $

$\beta = \set{ u\_1, u\_2, ..., u\_{ n }}, \gamma = \set{ v\_1, v\_2, ..., v\_{ m }} $ bases


for any $u+v \in U+V $

$\exists a\_1, a\_2, ..., a\_{ n }, b\_1, b\_2, ..., b\_{ m } s.t. $

$u = a\_1u\_1 + \_2u\_2 + ... + \_{ n }u\_{ n } $

$v = b\_1v\_1 + \_2v\_2 + ... + \_{ m }v\_{ m } $

$u+v = a\_1u\_1 + a\_2u\_2 + ... + a\_{ n }u\_{ n } + b\_1v\_1 + b\_2v\_2 + ... + b\_{ m }v\_{ m } $

$U + V \subseteq \spa{ \set{ u\_1, u\_2, ..., u\_{ n }, v\_1, v\_2, ..., v\_{ m }}}$

$\implies \dim (U+V) \leq n + m = \dim V + \dim V' $

{{% /proof %}}


(b) Let $U, V $ subspaces of $\R^5 $. $\dim U, \dim V = 3 $.

Prove that $U \cap V $ contains non-zero elements

{{% proof index="" name="" %}}

Suppose not $U \cap V = \set{ 0 } $

What is the $\dim U + V $

{{% lemma name="" index="" %}}

If $U \cap V = \set{  0 }$, then $\dim U + \dim V = \dim (U + V) $

{{% /lemma %}}

Let $\dim U = n, \dim V = m $

$\beta = \set{ u\_1, u\_2, ..., u\_{ n }}, \gamma = \set{ v\_1, v\_2, ..., v\_{ m }} $

in (a) we proved  that $U + V \subseteq \spa{ \beta \cup \gamma } $

To prove $\dim (U + V) = n + m$, it is sufficient to show that  $\beta \cup \gamma $ is linearly independent

Suppose $a\_1u\_1 + a\_2u\_2 + ... + a\_{ n }u\_{ n } + b\_1v\_1 + b\_2v\_2 + ... + b\_{ m }v\_{ m } = 0 $

$w = a\_1u\_1 + a\_2u\_2 + ... + a\_{ n }u\_{ n } = (-b\_1)v\_1 + (-b\_2)v\_2 + ... + (-b\_{ m })v\_{ m } $

$a\_1u\_1 + a\_2u\_2 + ... + a\_{ n }u\_{ n }= 0 \implies a\_1 = a\_2 = ... = a\_n = 0$

$b\_1v\_1 + \_2v\_2 + ... + b\_{ m }v\_{ m } = 0 \implies b\_1 = b\_2 = ... = b\_m = 0 $

so $a\_1u\_1 + a\_2u\_2 + ... + b\_{ m }b\_{ m } = 0 \implies a\_1 = a\_2 = ... = b\_m = 0$

Thus $\beta \cup \gamma $ is linearly independent.

(c\) Suppose not $U \cap V = \set{  0 } $

By (b) $\dim(U + V) = \dim U + \dim V = 3 + 3 = 6 $

$U + V \leq W, \dim W = 5, 6 = \dim (U + V) \leq \dim W = 5 $

Contradiction.

{{% /proof %}}

{{% /example %}}

{{% example name="" %}}

$V$ is a real valued  vector space. $T: V \to V $ linear transformation.

$T^2 = T $

(a) R(T) \cap N(T) = \set{ 0 }
(b) R(T) + N(T) = V

{{% proof index="(a)" name="" %}}

Suppose $V \in R(T) \cap N(T)$

$v \in R(T), \exists w \in V s.t. V = T(W) $

$v \in N(T) \implies T(v)  = 0$

$0 = T(v)  = T(T(w)) = T^2w = Tw = v$

{{% /proof %}}

{{% proof index="(b)" name="" %}}

$R(T) + N(T) = V $

Enough to show, for each $v \in V$

$\exists u \in R(T), w \in N(T), s.t. $

$v = u + w $

$T^2 v = Tv \implies T(Tv -v) = 0 $

$\implies Tv - v \in N(T) $

$\implies v - Tv \in N(T) $

$v = (v - Tv) + Tv $

{{% /proof %}}

{{% /example %}}

{{% example name="" %}}

$T: V \to W $ linear transformation. $v\_1, \_2, ..., \_{ n } \in V $.

$N(T) \subseteq \spa{ \set{ v\_1, v\_2, ..., v\_{ n }}}$

$W = \spa{ \set{ Tv\_1, Tv\_2, ..., Tv\_{ n }}} $

Then $\spa{ v\_1, v\_2, ..., v\_{ n }} = V  $

{{% proof index="" name="" %}}
For each $v \in V $

we want to prove that $v \in \spa{ v\_1, v\_2, ..., v\_{ n }} $

$Tv \in W = \spa{  \set{ Tv\_1, Tv\_2, ..., Tv\_{ n }}} $

$\exists a\_1, a\_2, ..., a\_{ n } \in F s.t. $

$Tv = a\_1Tv\_1 + a\_2Tv\_2 + ... + a\_{ n }Tv\_{ n } $

$\because T$ is linear

$T(v - a\_1Tv\_1 - a\_2Tv\_2 - ... - a\_{ n }Tv\_{ n }) = 0$

$v - a\_1Tv\_1 - a\_2Tv\_2 - ... - a\_{ n }Tv\_{ n } \in N(T) \subseteq \spa{ v\_1, v\_2, ..., v\_{ n }}  $

$\exists b\_1, b\_2, ..., b\_{ n } s.t. v - a\_1Tv\_1 - a\_2Tv\_2 - ... - a\_{ n }Tv\_{ n } = b\_1v\_1 + b\_2v\_2 + ... + b\_{ n }v\_{ n } $

$v = (a\_1 + b\_1)\_1v\_1 + (a\_2 + b\_2)\_2v\_2 + ... + (a\_n + b\_n)\_{ n }v\_{ n } \in \spa{ v\_1, v\_2, ..., v\_{ n }}$

{{% /proof %}}

{{% /example %}}

{{% example name="" %}}

$T: \R^3 \to \R^3, T(a,b,c) = (a + b, b+c, 0)$

1. $T $ is linear transformation
2. $N(T), R(T) = ? $
3. $nullity ? rank? $ verify the dimension theorem
4. $\beta = \set{(1, 0, 0), (1, 1, 0), (1, 1, 1)} $

{{% /example %}}
