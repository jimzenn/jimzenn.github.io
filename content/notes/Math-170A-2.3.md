---
title: "Probability Mass Function"
date: 2018-07-16T10:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 2.3


---

Probability mass function.

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
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

{{% definition name="Conditional Expectation" %}}

The conditional expectation of $X$ given $A$ with $P(A) > 0$ is

$E[X|A] = \sum\_{x} x p_{X|A}(x) = \sum\_{x} x P(X=x|A)$

Conditional expectation enjoys the properties of expectation we're seen:

1. linearity
2. Theorem:$E[g(X) | A] = \sum\_{x} g(x)P_{X|A}(x)$

We can condition one random variable on another.

{{% /definition %}}

{{% definition name="" %}}

Let $X, Y$ be random variable the conditional probability mass function of $X$ given $Y$ is

$P_{X|Y}(x|y) = P(X=x|Y=y)$

The expectation for X given Y is

$E[X|Y=y] = \sum\_{x} xP_{X|Y}(x|y) = \sum\_{x} x P(X=x|Y=y)$

{{% /definition %}}

{{% theorem name="Total Expectation Theorem" index="" %}}

Let $B \subset \Omega, P(B) > 0$

1\. $E[X] = E[X|B]P(B) + E[X|B^c]P(B^c)$

{{% proof index="" name="" %}}

$$
\begin{align\*}
E[X] &= \sum\_{x} xP(X=x)\\\\\
 &= \sum\_{x} xP(X=x|B)P(B) + P(X=x|B^c)P(B^c)\\\\\
 &= P(B)\sum\_{x} xP(X=x|B) + P(B^c) \sum\_{x} xP(X=x|B^c)
\end{align*}
$$

{{% /proof %}}

2\. If $ A\_1, A\_2, ..., A\_{n}$ partitions $\Omega, E[X] = \sum\_{ i=1 }^{n} E[X|A_i]P(A_i)$

3\. If $Y$ is a discrete random variable with range $\set{ y\_1, y\_2, ..., y\_{n} }$

$E[X] = \sum\_{ i=1 }^{n} E[X|Y=y]P(Y=y)$


Recall let $X$ be a geometric random variable with parameter $P$ recall:

$P_X(k) = (1-p)^{k-1} \cdot p$, for $k = 1,2, ...$

By conditioning on whether or not the first trial is successful.

$E[X] = E[X | X=1]P(X=1) + E[X|X > 1]P(X>1)$

1st trial failed "start over". The expected number of trials till success (once you've started over) is $E(X)$.

$E[X|X>1] = 1 + E[X]$

$$
\begin{align\*}
E[X] &= p + (1+E[X])(1-p) \\\\\\
&= p + 1 - p + (1-p)E[X] \\\\\\
p \cdot E[X] &= 1 \\\\\\
E[X] &= \frac{1}{p} \\\\\\
\end{align*}
$$

Using a similar technique, can find

$var(X) = \frac{ 1-p }{ p^2 }$

Summary: if $X$ generates random variable with parameter $p$, then $E[X] = \frac1p$ and $var(X)= \frac{ 1-p }{p}$

4\. Let $ A\_1, A\_2, ..., A\_{n}$ partition $\Omega$, Let $B \subset \Omega$, let $B \subset  \Omega$ s.t. $P(A \cap B) > 0$ for all $i$.

$E[X|A] = \sum\_{ i=1 }^{n} E[X|A_i \cap B]P(A_i|B)$

{{% proof index="" name="" %}}

$$
\begin{align\*}
& \sum\_{n}^{ i=1 }  \sum\_{x}^{  } P(X=x | A_i \cap B)P(A_i | B) \\\\\
&= \sum\_{ i=1 }^{n}  \sum\_{x} x \frac{ P(X=x \cap A \cap B) }{ P(A_i \cap B) } \cdot \frac{ P(A_i \cap B) }{ P(B) } \\\\\
&= \sum\_{x}^{  } \sum\_{ i=1 }^{n} x \frac{ P(X=x \cap A_i \cap B) }{ P(B) } \\\\\
&= \sum\_{x}^{  } \frac{x}{ P(B) } \sum\_{ i=1 }^{n} P(X=x \cap A_i \cap B) \\\\\
&= \sum\_{x}^{  } \frac{x}{ P(B) } P(X=x \cap B) \\\\\
&= \sum\_{x}^{  } xP(X=x |B) = E[X|B]
\end{align*}
$$
{{% /proof %}}

{{% /theorem %}}

Let $X, Y$ be discrete random variables, how are $P\_{X,Y}, P\_{X|Y}, P_{Y|X}, P_X, P_Y$.

$P_{X|Y}(x|y) = P(X=x | Y=y) = \frac{ P( \set{ X = x } \cap \set{ Y = y }) }{ P(Y=y) }$

Recall $A, B \subset \Omega$ are independent means $P(A \cap B) = P(A)P(B).$

{{% definition name="" %}}

1\. Random variable $X$ is independent of $A \subset \Omega, X = x$ and $A$ are independent for all $x$.

2\. $P(X=x, Y=y) = P(X=x)P(Y=y)$ for all $x, y$.

Equivalently, $P_{X,Y}(x,y) = P_X(x)P_Y(y)$ for all $x, y$.

In this case, $P_{X|Y}(x|y) = P_X(x)$ for all $x, y$.

{{% /definition %}}

{{% theorem name="" index="" %}}

If $X, Y$ are independent, then

$E[XY]  = E[X] E[Y]$

{{% example name="" %}}

Let $X_i$ be outcome of $i$th toss of a 6-sided dice.

$E[X_iX_2X_3] = E[X_1]E[X_2]E[X_3]=(3.5)^3$

{{% /example %}}

{{% proof index="" name="" %}}

$$
\begin{align\*}
E[XY] &= \sum\_{x}^{  } \sum\_{y}^{  } P(X=x, Y=y) \\\\\
&=\sum\_{x}^{y} x y P(X=x)P(Y=y) \\\\\
&= \sum\_{x}^{  } x P(X=x) \sum\_{y}^{  } yP(Y=y) \\\\
&=E[X] E[Y]
\end{align*}
$$

{{% /proof %}}

{{% /theorem %}}

{{% theorem name="" index="" %}}

If $X, Y$ are independent, then

$$
\begin{align\*}
var(X+Y) &= E[(X+Y)^2] - (E[X + Y])^2 \\\\\
&= E[X^2 +2XY + Y^2] - (E[X] + E[Y])^2 \\\\\
&= E[X^2] + 2E[X]E[Y] + E[Y^2] - (E[x]^2 + 2E[X]E[Y] + E[Y]^2) \\\\\
&= (E[X^2] - E[x]^2) + (E[Y^2] - E[Y]^2) \\\\\
&= var(X) + var(Y)
\end{align*}
$$

{{% /theorem %}}

{{% theorem name="" index="" %}}
Let $X$ be binomial with parameters $n_1p$

Recall: $X = \sum\_{ i=1 }^{x} y_i,$ where $y_i$ Bernoulli with parameter $p$.

i.e. $P(Y=1) = p, P(Y=0) = 1-p$

$E[X] = \sum\_{ i=1 }^{n} E[Y_i] = np$

since the $y_i$s are independent.

$$
\begin{align\*}
var(X) &= \sum\_{ i=1 }^{n} var(y_i) \\\\\
&= n[E[y_1^2] - E[y_1]]^2 \\\\\
&= n[1^2p + 0(1-p) - p^2] \\\\\
&= n(p-p^2)
\end{align*}
$$



{{% /theorem %}}
