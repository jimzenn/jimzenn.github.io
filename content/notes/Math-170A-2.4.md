---
title: "Covarience"
date: 2018-07-18T10:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 2.3

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
    $\newcommand{\B}{\beta}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{{#1}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
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

Recall

$X, Y $ are independent means for any $x, y$,
$P(X=x, Y=y) = P(X=x)P(Y=y) $
We saw that if $X,Y$ are independent.

Then $E\[XY\] = E\[X\]E\[Y\]$
$var(X+Y) = var(X)+ var(Y)$

{{% definition name="conditional independence" %}}
Let $A \subset \Omega , P(A) > 0, X, Y$ are conditionally independent given A, meaning

$$ P(X=x, Y=y|A) = P(X=x|A)P(Y=y|A), \forall x, y$$

{{% /definition %}}

{{% definition name="covariance" %}}

The covariance of $X,Y$ is $cov(X,Y) = E[(X-E[X])(Y-E[Y])]$.

{{% note name="" %}}
measures if X and Y are around the mean at the same time.

Notice if $X, Y$ are independent, then $cov(X,Y) = E[XY - XE[Y] - YE[X] + E[X]E[Y]] = 0$

{{% /note %}}

{{% /definition %}}

{{% example name="" %}}

Two RVs $X,Y$ with $E[XY] = E[X]E[Y]$ and $cov(X,Y) = 0$, but $X,Y$ not independent. Let $X$ take value $1, 2,-1, -2$, each with probability $\frac{1}{4}$. Note $E[X] = 0, E[Y] = 0$.

Let $Y=X^2$, $Y$ takes value 1,4 with probability $\frac{1}{2}$.

$E[y] = 1 \cdot \frac{1}{2} + 4 \cdot \frac{1}{2} = 2.5 $

$X \cdot Y = X \cdot X^2 = X^3$

So $E[XY] = E[X^3] = 0 = E[X]E[Y]$

$cov(X,Y) = E[(X-0)(Y-2.5)] = E[XY-2.5X] = 0$

To prove $X$ and $Y$ are not independent, we try to find a value of $X$ and a value of $Y$ s.t.

$P( \set{ X=1 } \cap \set{ Y=1 } ) = P( \set{ X=1 } ) = \frac{1}{4}$, since $\set{ Y=1 } \supset \set{ X=1 }$

$ P(X=1) P(Y=1) = \frac{1}{4} \frac{1}{2} = \frac{1}{8}$

So $X,Y $ aren't independent.

{{% /example %}}

{{% example name="" %}}

Let $X\_i, i = 1, 2, ..., n$be independent random variables, with the same probability mass function. (e.g. $ X_i $is Bernoulli represents $i$th toss of same coin.) We call $S\_n = \frac{ X\_1, X\_2, ..., X\_{n} }{n}$ the sample mean.

$E[S_n] = \frac{ E[X\_1] + ... + E[X\_n] }{n} = E[X\_1] $

$var(S\_n) = \frac{ var(X\_1) + ... + var(X\_n) }{ n^2 } = \frac{ n var(X\_1) }{ n^2 } = \frac{ var(X\_1) }{n}$

{{% note name="" %}}
$var(S\_n) \to 0 $as $n \to \infty$

This suggests that tossing coin many times will allow to determine the chance of a toss being $\head $.
{{% /note %}}

{{% /example %}}

{{% example name="St. Petersburg Paradox (Bernoulli, 1738)" %}}

Casino offers a game, you can toss a fair coin until you get $\tail $, and at that point you win $\$2^{ \text{ number of tosses } }$. How much would you pay to play this game?

{{% note name="" %}}

let $X$ be gain, note number of tosses is a geometric random variable with parameter $\frac{1}{2}. $

$P(Y=k) = \frac{1}{2}^{k-1} \cdot \frac{1}{2} = \frac{1}{2}^k, k = 1, 2, ...$

$X = 2^y$ i.e. $X = g(Y)$, where $g(y) = 2^y$

$E[X] = E[g(y)] = \sum\_{y} g(y)P(Y=y) = \sum\_{ y=1 }^{ \infty } 2^y \frac{1}{2}^y = \sum\_{ y=1 }^{ \infty } 1 = \infty$

What?

Resolution of paradox:

Expected value <u>doesn't necessarily</u> describe a random variable.

{{% /note %}}

{{% /example %}}

{{% example name="" %}}

An oak sheds $N$ seeds where $N$ is binomial with parameter $n, p $.
Each seed takes root with probability $\gamma$independent of others. Let $S$ be resulting number of new trees.

1. $P(S|N)$
2. $P(S,N)$
3. $P(S)$

$P(S=i|N=j)$ given that $i$ seeds dropped, what is the probability that $j$ new trees took root?

Note: $P(S=i|N=j) = 0, \if j > i.$

i.e. the chance of $j$ successes in $i$ trials. i.e. Binomial with parameter $i, j$.

$P(S=j, N=i) = P(S=j, N=i) = P(S=j | N = i)P(N=i) $

$\because B\text{ is a binomial with probability} n, p , P(N=i) = \binom{n}{i} p^i (1-p)^n-i$

$P(S-j, N=i) = \binom{i}{j} \gamma^j (1-\gamma)^{i-j} \binom{n}{i}p(1-p)^{n-j}, 0 \leq j \leq i \leq n$

$P(S=j) = \sum\_{ i=0 }^{n} P(S=j, N=i) = \binom{n}{j}(\gamma p)^j (1- \gamma p)^{n-j}$

i.e. Binomial with parameter $n, p $. We can see this also via: name each seed $i$ becomes a tree if and only if it drops and takes root. Thus, occrs with probability $\gamma p$. Thus,

$$S= \sum\_{ i=1 }^{n} X_i$$

{{% /example %}}



