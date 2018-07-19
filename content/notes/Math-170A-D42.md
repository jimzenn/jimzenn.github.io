---
title: "Disucission"
date: 2018-07-17T10:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: D4


---

Discrete random variable.

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\br}{\\}$
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
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
  {{< /raw >}}
</div>


{{% example name="" %}}

Let $X$ be uniform on $\set{ a, a+1, ..., b }, a < b integers$, compute $E[X|c \leq X \leq d]$, where $a \leq < d \leq b$.

$\begin{align\*}
  &E[X| c \leq X \leq d] \br
  &= \sum\_{ k=a }^{b} k P(X=k | c \leq X \leq d) \br
  &= \sum\_{ k=c }^{d} k P(X=k | c \leq X \leq d)
\end{align*}$

$\begin{align\*}
  P(X=k | c \leq X \leq d) \br
  &= \frac{ P(X=k, c \leq X \leq d) }{ P( c \leq X \leq d ) } \br
  &= \frac{ P(X =k) }{ P( c \leq X \leq d ) } \br
  &= \frac{ \frac{1}{ b - a + 1 } }{ \frac{ d -c + 1 }{ b - a +1 }} \br
  &= \frac{1}{ d-c+1 }
\end{align*}$

{{% /example %}}

{{% example name="2" %}}

The number of hours worked in a month by Oscar in a uniform random variable on $\set{ 0,1 ,2, ..., 100 }$. He makes \$1 per hour, but once he has worked 50 hours, he makes \$2 per hour for each addition hour. <br>
If he works more than 75 hours, he has a 50% chance of winning a \$30 prize.<br>
Find the expected value of his pay.


$W = $ k hours work W is uniform  on $\set{ 0, 1, 2, ..., 100 }$

$P( \text{ pay }) = \begin{cases}
             W , 0 \leq W \leq 50  \br
             50+2(W-50) , 51 \leq W \leq 75 \br
             2W - 50 + 30, 76 \leq W \leq 100 \text{ w/ prize } \br
             2W - 50 , 76 \leq W \leq 100 \text{ w/o prize } \br
         \end{cases}$

$\begin{align\*}
  &E[P] =   \br
  &E[P| 0 \leq W \leq 50] P( 0 \leq W \leq 50 ) \br
  &+ E[P| 51 \leq W \leq 75] P( 51 \leq W \leq 75 ) \br
  &+ E[P| 76 \leq W \leq 100 \text{ w/ prize}] P( 76 \leq W \leq 100 \text{ w/ prize} ) \br
  &+ E[P| 76 \leq W \leq 100 \text{ w/o prize}] P( 76 \leq W \leq 100 \text{ w/o prize} ) \br
\end{align*}$

{{% /example %}}


{{% example name="3" %}}
Roll 3 fair 6-sided die. <br>
$X_i = \text{ outcome of roll } i$ <br>
$Y = min(X_1, X_2, X_3)$ <br>
$Z = max(X_1, X_2, X_3)$ <br>

{{% remarks name="technique" %}}

$\begin{align\*}
P(Y \geq k) &= P(min(X_1, X_2, X_3) \geq k) \br
&= P(X_1 \geq k, X_2 \geq k, X_3 \geq k) \br
&= P(X_1 \geq k) P(X \geq k) P(X_3 \geq k) \br
&= P(X_1 \geq k)^3
\end{align*}$

$\begin{align\*}
P(Y = k) &= P(Y \geq k) - P(Y \geq k+1) \br
&= \left\(\frac{ 7-k }{6}\right\)^3 - \left\(\frac{ 7-(k+1) }{6}\right\)^3 \br
\end{align*}$

{{% /remarks %}}


$\begin{align\*}
P(Z \leq k) &= P( max(X_1, X_2, X_3) \leq k ) \br
&=P(X_1 \leq k, X_2 \leq k, X_3 \leq k) \br
&=P(X_1 \leq k)^3 \br
&= \frac{k}{6}^3
\end{align*}$

$P(Z=k) = P(Z \leq k) - P(Z \leq k-1) = \left\( \frac{k}{6} \right\)^3 - \left\( \frac{ k - 1 }{6} \right\)^3$


{{% /example %}}

{{% example name="5" %}}

A class has 150 students.
25 are graduate students.
125 are undergraduates.
<br>
A graduate student has prop p of getting an A.
An undergraduate student has prop q of getting an A.
<br>
Find the expected value of $X$ = number os students who get A's.

method 1: $E[X] = \sum\k P(X=k)$

method 2:

X_1, X_2, ..., X_{125}
Y_1, ..., Y_{25}

$P_{X_i} (k) =
\begin{cases}
q, k = 1 \br
1-q, k = 0
0 \text{ otherwise }
\end{cases}$

$P_{Y_i} (k) =
\begin{cases}
p, k = 1 \br
1-p, k = 0
0 \text{ otherwise }
\end{cases}$

$X_i =
\begin{cases}
1, \text{ if undergrad gets an A } \br
0 \text{ otherwise }
\end{cases}$

$Y_i =
\begin{cases}
1, \text{ if grad student gets an A } \br
0 \text{ otherwise }
\end{cases}$

$X = (X_1 + ... + X_{125}) + (Y_1 + ... + Y_{25})$

$E[X] = E[X_1] + ... + E[X_{125}] + E[Y_1] + ... E[Y_{25}] = 125q + 25p$

{{% /example %}}

{{% example name="" %}}

n couples will be seated uniformly at random at a circular table $w/ 2n$ chairs
Let $X$ = number of couples who are seated next to each other.

Find $E[X]$.

$X_i =
\begin{cases}
1, \text{ if couple }i \text{ is seated next to each other } \br
0 \text{ otherwise }
\end{cases}$


Notice that $ X\_1, X\_2, ..., X\_{n}$ are NOT independent.

$E[X] &= E[X_1] + ... + E[X_n] \br
&= n E[X_i] \br
&= n P(couple 1 sits next to each other) \br
&= n( \frac{2}{ n-1 } ) \br
&= \frac{ 2n }{ n-1 }$


{{% /example %}}

