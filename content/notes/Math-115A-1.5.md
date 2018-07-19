---
title: "Linear Dependence and Linear Independence"
date: 2018-07-03T11:03:48+08:00
author: "Jim Zenn"
volumes: ["MATH 115A"]
layout: "note"
issue: 1.5


---

Linear dependence, linear independence.

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\C}{\mathbb{C}}$
    $\newcommand{\P}{\mathbb{P}}$
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

{{% definition name="linearly dependent" %}}
Let $V$ be a vector space over field $F$. A subset $S \subseteq V$ is called **linearly dependent** if there <u>exist</u> a finite number of distinct vectors $u_1, u_2, ..., u_n \in S$ and $a_1, a_2,..., a_n \in F$, <u>not all zero</u> such that

$$a_1v_1 + a_2v_2 + ... + a_nv_n = 0$$

{{% /definition %}}

{{% example name="$\R^2$" %}}

Prove that $S= \set{(1,0), (0,1), (2,-3)}$ is linearly dependent.

{{% proof name="" %}}
We just need to find <u>one</u> not all zero coefficient solution.

$-2(1,0) + 3(0,1) +1(2,-3) = (0,0)$

$\therefore S$ is linearly dependent.

{{% /proof %}}

{{% /example %}}

{{% definition name="linearly independent" %}}
Let $V$ be a vector space over $F$, a subset of $S\subseteq V$.

$S$ is called **linearly independent** if it is NOT linearly dependent.

Equivalently, $S$ is called **linearly independent** if for <u>every finite</u> subset of vector $v_1, v_2, ..., v_n \in S$ the only solution of the equation (in $a_i$) $$a_1v_1 + a_2v_2 + ... + a_nv_n = 0$$
is
$$a_1=a_2=...=a_n=0$$

{{% /definition %}}

{{% note name="" %}}

1\. $V/F$, $\set{\emptyset}$ is linearly independent.

{{% proof name="by contradiction" %}}

Assume that $\emptyset$ is linear dependent.

$v_1, v_2, ..., v_n \in \emptyset$ and $a_1,a_2, ..., a_n \in F$ such that at least one of the $a_i$s is non-zero and $a_1v_1 + a_2v_2 + ... + a_nv_n = 0$.

However, since there is no $v \in \emptyset$, there doesn't exist a $a$ that is non-zero.

Therefore, the empty set is linearly independent.

{{% /proof %}}

2\. $V/F, \set{v}\ (v \neq 0)$ is linearly independent.


3\. if $0 \in S$, $S$ is linearly dependent. (In particular, $\set{0}$ is linearly dependent.)

{{% proof name="by contradiction" %}}
Assume that it is linearly dependent:

$\exists a \in F, a\neq 0.$ s.t. $$av=0$$

$\because a\in F$ and $a\neq 0$, $\therefore a^{-1} \in F$.

$$a^{-1}(av)= a^{-1}0 \implies v = 0$$

This is a contradiction to $v\neq 0$.

{{% /proof %}}

{{% /note %}}


{{% example name="$\R^2$" %}}
$S=\set{(1,0),(0,1)}$ is linearly independent.

{{% proof name="" %}}
$a(1,0) + b(0,1) = (0,0)$

$\implies (a,b) = (0,0)$

$a= 0, b=0$

$\therefore S$ is linearly independent.
{{% /proof %}}
{{% /example %}}

{{% example name="$\R^2$" %}}
$S=\set{(1,1),(3,-3)}$ is linearly independent.

{{% proof name="" %}}
$a(1,1) + b(2,-3) = (0,0)$

$(a+2b,a-3b) = (0,0)$

$$
\begin{align\*}
a+2b=0 \br
a-3b=0
\end{align*}
$$

$\implies (a,b) = (0,0)$

$a= 0, b=0$

$T$ is linearly independent.
{{% /proof %}}
{{% /example %}}

{{% theorem name="" index="1.6" %}}
$V/F$, $S_1, S_2 \subseteq V$.

If $S_1$ is linearly dependent and $S_2\supseteq S_1$, then $S_2$ is also linearly dependent.

If $S_1$ is linearly independent and $S_2 \subseteq S_1$, then $S_2$ is also linearly independent.

{{% /theorem %}}

{{% theorem name="" index="1.7" %}}
$V/F, S \subseteq V, v \in V,$ $S$ is linearly independent.

$S \cup \set{v}$ is linearly dependent
$\iff v \in \spa{S}$.

{{% proof name="" %}}

$\impliedby$

$v\in \spa{S}$.

$\therefore \exists v_1, v_2, ..., v_n \in S$ and $a_1, a_2, ..., a_n \in F$ s.t. $$v=a_1v_1 + a_2v_2 + ... + a_nv_n$$

$a_1v_1+a_2v_2 + ... a_nv_n + (-1)v = 0$

$S\cup \set{v}$ is linearly dependent.

$\implies$

$S \cup \set{v}$ is linearly dependent.

$\therefore$ for $v_1, v_2, ..., v_n, v \in S\cup \set{v}, \exists a_1, a_2, ..., a_n \in F$ s.t.

$$a_1v_1+a_2v_2 + ... + a_nv_n + av = 0$$
at least one of $a_1, a_2, ... ,a_n, a$ is non-zero.

Claim $a \neq 0$.

If $a = 0$, then we have
$a_1v_1 + a_2v_2 + ... + a_nv_n = 0$.

Since $S$ is linearly independent $\set{v_1, v_2, ..., v_n} \subseteq S$ is also linearly independent.

From theorem we get $a_1=a_2=a_3= ... = a_n = 0= a$

This is a contradiction to the condition $a_1, a_2, ..., a_n, a$ not all zero

$\therefore a \neq 0$

$a_1v_1+a_2v_2 + ... + a_nv_n + av = 0$
$av = -a_1v_1 -a_2v_2 - ... -a_nv_n$
$v = -\frac{a_1}{a}v_1 -\frac{a_2}{a}v_2 - ... -\frac{a_n}{a}a_nv_n$

$\therefore v \in \spa{S}$.

{{% /proof %}}

{{% /theorem %}}

{{% example name="" %}}
$V=\R, F=\R$

$S=\set{1}$

$x\in V = \R$

$\forall r \in \R, S=\set{r}$ is a generating set.

{{% /example %}}

{{% example name="" %}}
$V=\C, F=\C$

$S = {z} \subset V = \C, z \neq z$

$w \in V = \C$

$w = \frac w z \cdot z$

{{% /example %}}

{{% example name="" %}}
$V=\C, F=\R$

$s = {1, z}, z\neq 0$

$w\in V = \C$

NOTTRUE! $w = \frac w z \cdot z$

{{% /example %}}
