---
title: "Theorems of Vector Spaces; Field"
date: 2018-06-25T11:03:48+08:00
author: "Jim Zenn"
volumes: ["MATH 115A"]
layout: "note"
issue: 1.2


---

Theorem 1.1: cancellation law for vector addition, theorem 1.2, null vector's uniqueness, fields.

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\C}{\mathbb{C}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\union}{\cup}$  
    $\newcommand{\intercept}{\cap}$  
    $\newcommand{\abs}[1]{|#1|}$  
    $\newcommand{\t#1}{\text}[1]$  
  {{< /raw >}}
</div>

{{% theorem name="Cancellation Law for Vector Addition" index="1.1" %}}

$x,y,z \in V$, if $x + z = y+z$, then $x= y$.

{{% proof %}}

$\exists v \in V $ s.t. $z+v = 0$   (VS4)

$
\begin{align\*}
x &= x+0 \\\\\\ 
 &= x + (z+ v) \\\\\\ 
&= (x+ z) + v \\\\\\
&= (y + z) + v \\\\\\
&= y + (z + v) \\\\\\ 
&= y + 0 = y
\end{align*}
$

{{% /proof %}}

{{% /theorem %}}


{{% corollary index="1" %}}

The **zero vector** (or **null vector**) $0$ described in VS3 is <u>unique</u>.

i.e. if $0, 0'$ both satisfy (VS3) then $0=0'$.

i.e. $\forall x \in V, x + 0=x, x + 0'=x$, then $0=0'$.

{{% proof %}}

let $x = 0, y = 0' $

$0 + x = x \implies 0 + 0 = 0$

$0 + y = y \implies 0 + 0' = 0$

$\therefore 0 + 0 = 0 + 0'$

$0 = 0'$ (cancellation law)

{{% /proof %}}

{{% proof %}}

$0=0+0'=0'+0=0'$, so $0=0'$

{{% /proof %}}

{{% /corollary %}}


{{% corollary index="2" %}}

The **addtictive inverse** (vector) described in VS4 is <u>unique</u>.

The additive inverse of $x$ can be denoted by $-x$.

{{% /corollary %}}

{{% theorem name="" index="1.2" %}} 
In any vector space $V$, the following statements are true:

1. $\forall x \in V, 0 \in F, 0x = 0.$
2. $\forall a \in F, \forall x \in V, (-a) x = -(ax) = a(-x).$
3. $\forall a \in F, 0 \in V, a0=0$.

<small>Please be careful what is the symbol '0' is referring to. When $0 \in F$, it is a scalar; when $0 \in V$, it is a vector.</small>

{{% /theorem %}}

{{% definition name="Field" %}} 

A **field** $F$ is a set on which two operations **addition** $+$ and **multiplication** $\cdot$ are defined so that following conditions are satisfied

1. $a+b=b+a$ , $a\cdot b= b\cdot a$
<br> (commutativity of addition and multiplication)
2. $(a+b)+c=a+(b+c), (a\cdot b)\cdot c = a\cdot (b\cdot c)$
<br> (associativity of addition and multiplication)
3. $ \exists 0 \in F, 1\in F$ s.t. $\forall a, 0+a=a, 1\cdot a = a$
<br> (existence of identity elements for addition and multiplication)
4. $a\in F, \exists c \in F$ s.t. $a+c=0$<br>
$b \in F, b \neq 0, \exists d \in F$ s.t. $b\cdot d = 1$
<br> (existence of inversion for addition and multipliation)
1. $a \cdot (b+c) = a\cdot b + a\cdot c$
<br> (distributivity of multiplication over addition)


<small>
The elements $x + y$ and $x \cdot y$ are called the **sum** and **product**, respectively of $x$ and $y$. 
<br>
The elements $0$ and $1$ are called **identity elements** for addition and multiplication, respectively. 
<br>
The elements  elements $c$ and $d$ referred to in (F 4) are called an **additive inverse** for $a$ and a **multiplicative inverse** for $b$, respectively.
</small>

{{% /definition %}}

{{% examples name="" %}} 

$\R$ is a field.
$\C$ is a field.
$\Q$ is a fkeld.

$\Z$ is NOT a field.  (F4)

{{% /examples %}}

{{% corollary name="" index="" %}} 
Every field is a vector space over itself.
{{% /corollary %}}

{{% examples name="" %}} 
$\C$ is a vector space over $\C$.

$\C$ is also a vector space over $\R$, $\R \subset \C$.

$\R$ is also a vector space over $\Q$, $\Q \subset \R$.
{{% /examples %}}

{{% example name="$F_2$, a field of characteristic 2" %}}
$F = \set{0, 1}.$<br>
addition is defined as xor, i.e.:<br>
$0 + 0 = 0$,
$0 + 1 = 1$.<br>
multiplication is defined as:<br>
$0 \cdot 1 = 0$,
$1 \cdot 1 = 1$.
{{% /example %}}

{{% example name="the prime field" %}} 
$\forall$ prime number $p$, $F_p = \set{0, 1, 2, ..., p - 1}$

> ... The sum, the difference and the product are computed by taking the remainder by p of the integer result. The multiplicative inverse of an element may be computed by using the extended Euclidean algorithm ...

{{% /example %}}