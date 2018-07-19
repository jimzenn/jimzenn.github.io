---
title: "Probability Mass Function"
date: 2018-07-11T10:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 2.2


---

Probability mass function, binomial random variable

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

{{% example name="Roulette" %}}

[1|2|3|4| ... |36|0|00] <br>
1, 3, ..., 35 are red (odd) <br>
2, 4, ..., 36 are black (even) <br>
0, 00 are green. <br>
Payout on red or black is $1:1$ i.e. if you bet \$1 and win, you win \$1. <br>
Payout on $a \neq (1, ..., 36)$ is $1:35$ i.e. if you bet \$1 and win you win \$35.

Let $X$ be the outcome of a roll.

$X(\set{0})= 37, X(\set{00})=38$

A bet is a function of $X$.

{{% /example %}}

e.g. 1: bet \$10 on red.

$G(X) = \begin{cases}
10 , \if x = 1,3,...,35 \br
-10 , \otherwise
\end{cases}$

2: bet \$10 on 2.

$W(X) = \begin{cases}
350, \if x = 2 \br
-10, \otherwise
\end{cases}$

We assume it's a fair wheel, i.e.

$P(X=k) = \begin{cases}
\frac{1}{ 38 }, \if 1, 2, ..., 38 \br
0, \otherwise
\end{cases}$

Let's compute the expected.

Let's compute the expected outcome of each of these bets.

1. let $Y = g(X)$,
 recall by definition, $E[Z]= \sum\_{z}P(Z=z)$
 also recall theorem E[g(X)] = \sum\_{x} g(x)P(X=x)
$E[y] = E[g(X)] = \sum\_{x} g(x)P(X=x) = 10 \sum\_{ x=1,3,...,35 } \frac{1}{ 38 } + (-10) \sum\_{ x = 2,4, ..., 36,37,38 } \frac{1}{ 38 }$

$ E[h(X)] = \sum\_{x} h(x)P(X=x) = \sum\_{ x=2 } 350 \cdot \frac{1}{ 38 } + \sum\_{ x \in \set{ 1, 38 } }  (-10) \frac{1}{ 38 }$

try calculating variance and standard deviation.

{{% properties name="Key properties of $E[X]$" %}}

1. $E[X+Y] = E[X] + E[Y]$
2. if $a \in R$, then $E[aX] = aE[X]$
3. if $a \in R$, then $E[a] = a$

I summarize (2) - (3) as $E[aX + c] = aE[X] + c$

for variance,
$var(aX + c) = a^2 var(X)$

{{% /properties %}}

{{% definition name="Varience" %}}

$var(X) = E[(X-E[X])^2]$

equivalently, $var(X) = E [X^2 -2XE[X] + (E[X])^2]$
$=E[X^2] - 2E[X]E[X] + E[X]^2 = E[X^2] -2E[X]^2$

{{% /definition %}}

One experiment, $2$ random variable $s$.

{{% definition name="Joint PMF" %}}
The joint probability mass function of two discrete random variable $X,Y$ associated to one experiment is $P_{X,Y}(x,y) = P(X=x, Y=y)$.

{{% /definition %}}

{{% example name="" %}}
magnetic board, some parts are stronger than others, I throw a metallic object.

I record the probability of objects landing on the each of the squares.


|     | 0 | 1 |
|-----|---|---|
|**1**|1/2|1/8|
|**0**|1/8|1/4|

Let X be the horizontal grid value,
y = the vertical grid value.

$P(X=1)= P(X=1) = \frac18 + \frac14 = \frac38$

How to find $P_X, P_Y$?

In general, say $X, Y$ have joint PMF $ P_{X, Y}$ we can find $P_X$, and $P_Y$(called **marginals**) as follow:
$P\_X(x) = P(X=x) = P( \cup\_y (X=x \cap Y = y) ) = \sum\_{y} p\_{X,Y}(x,y)$

Similarly,
$P\_Y(y) = P_{X,Y}(x,y)$


$P_X(1) = \sum\_{y} P\_{1,Y} = P(X=1, Y=0) + P(X=1, Y=1) = \frac{1}{4} + \frac{1}{8} = \frac{3}{8}$

$P_X(0) = \sum\_{y} P\_{0,Y} = P(X=0, Y=0) + P(X=0, Y=1) = \frac{1}{8} + \frac{1}{2} = \frac{5}{8}$

$P_Y(1) = \sum\_{x} P\_{X,1} = P(X=0, Y=1) + P(X=1, Y=1) = \frac{1}{2} + \frac{1}{8} = \frac{5}{8}$

$P_Y(0) = \sum\_{x} P\_{X,0} = P(X=0, Y=0) + P(X=1, Y=0) = \frac{1}{8} + \frac{1}{4} = \frac{3}{8}$

{{% /example %}}


{{% example name="" %}}

Another example, with same marginals but different probability for each grid.

|     | 0 | 1 |
|-----|---|---|
|**1**|25/64|15/64|
|**0**|15/64|9/64|

$P_X(1) = \sum\_{y} P\_{1,Y} = P(X=1, Y=0) + P(X=1, Y=1) = \frac{3}{8}$

$P_X(0) = \sum\_{y} P\_{0,Y} = P(X=0, Y=0) + P(X=0, Y=1) = \frac{5}{8}$

$P_Y(1) = \sum\_{x} P\_{X,1} = P(X=0, Y=1) + P(X=1, Y=1) = \frac{5}{8}$

$P_Y(0) = \sum\_{x} P\_{X,0} = P(X=0, Y=0) + P(X=1, Y=0) = \frac{3}{8}$

{{% /example %}}


{{% theorem name="" index="" %}}
Let $g: \R \times \R \to \R$
i.e. g is a real-valued function of 2 variables. Let X, Y have joint PMF, $P_{X,Y}$.

$$E[g(X,Y)] = \sum\_{ x,y } g(x,y) P\_{X,Y}(x, y)$$

{{% /theorem %}}

{{% example name="" %}}

Let $X$ be binomial random variable, with parameters $n$, $p$ i.e. $X$ is number of $H$ in $n$ tosses of a coin.

Let random variable $X_i$ take the value $1$ if the $i$th toss is $H$, and $0$ if the $i$th toss is $T$.

Note: $X = \sum\_{ i=1 }^{n} X_i$

So $E[X] = \sum\_{ i=1 }^{n} E[X_i]$

$\forall i, E[X\_i] = \sum\_{x}Xp\_X\_1(x) = 10 p + 0(1-p) =p $

so $E[X] = np$

summaries:

if $X$ binomial with parameters $n, p$. New $E[X]= np$.

note: if $p=1/2, E[X] = \frac{n}{2}$
{{% /example %}}

{{% definition name="" %}}

Let X be number of typos in a book with n letters, where each letter is wrong is p. and the typos are independent. i.e. X binomial.

$P(X=k) = \binom{n}{k} p^k (1-p)^{n-k}, k = \set{ 0, 1, 2, ..., {n} }$

Let $\lambda = np$ fact $k \in \set{ 0, ..., n }$

for $n$ large, $p \in [0, 1]$

$e^{-\lambda} \frac{ \lambda^k }{ k! } \approx \binom{n}{k} p^k (1-p)^{n-k}$

Let $y$ be random variable with probability mass function.

$p_y(k) = e^{-\lambda} \frac{ \lambda^k }{ k! }, k= 0,1,2,...$

y is called **Poisson** with parameter $\lambda > 0$.

check

$\sum\_{ k=0 }^{ \infty } p_y(k) = \sum\_{ k=0 }^{ \infty } e^{-\lambda} \frac{ \lambda^k }{ k! } =  e^{-\lambda} \sum\_{ k=0 }^{ \infty } \frac{ \lambda^k }{ k! } = e^{-\lambda} e^\lambda = 1$

{{% /definition %}}

