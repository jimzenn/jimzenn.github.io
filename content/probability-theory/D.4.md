---
title: "Disucission: Midterm Review"
date: 2018-07-17T10:03:48+08:00
volumes: ["D"]
layout: "note"
issue: 4
draft: true


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
    $\newcommand{\rank}[1]{\text{rank }#1}$
    $\newcommand{\tr}[1]{\text{tr}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$
    $\newcommand{\Re}[1]{\text{Re}(#1)}$
    $\newcommand{\Im}[1]{\text{Im}(#1)}$


    $\newcommand{\Vcw}[2]{\begin{bmatrix} #1 \br #2 \end{bmatrix}}$
    $\newcommand{\Vce}[3]{\begin{bmatrix} #1 \br #2 \br #3 \end{bmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \end{bmatrix}}$
    $\newcommand{\Vct}[5]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{bmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{bmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{bmatrix}}$

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

{{% example name="1c" %}}

Two fair six-sided dice are rolled. Find the probability that the sum of the outcome is 11.

$\Omega = \set{(i, j) | i,j \in \set{ 1,2,...,6 }}$

$P(\text{ sum = 11 }) = P(\set{(5,6), (6,5)}) = \frac{2}{ 36 } = \frac{1}{ 18 }$

{{% /example %}}

{{% example name="1c, with extra sauce" %}}

Roll 3 fair six-sided dice. Let X = sum of the outcomes. Find P(X=11).

Let $X\_i = $ outcome of roll $i, i = 1,2,3$.

$X= X\_1 + X\_2 + X\_3$

$$
\begin{align\*}
P(\text{ X = 11 })
&= P(\text{ X\_1 + X\_2 + X\_3 = 11 }) \br
&= \sum\_{ k=2 }^{ 10 }P(X\_1 + X\_2 = k)P(X\_3 = 11-k | x\_1 + x\_2 = k) \br
&= \sum\_{ k=5 }^{ 10 } P(X\_1 + X\_2 =k)P(X\_3 = 11 - k) \br
\end{align*}
$$

{{% /example %}}

{{% example name="1f" %}}

$6$ sheets of paper, labeled with #s from $1$ through $6$. Draw two simultaneously (without replacement). Find the probability that the sum of the umbers is $11$.

$\Omega = \set{(i,) | i \neq j, i,j \in \set{ 1,2,...,6 }}$

$P(\text{ um = 11 }) = \frac{1}{ \binom{6}{2}}$

{{% /example %}}

{{% example name="2" %}}

Let X be discrete uniform on \set{ -3, -2,  -1, 0, 1, 2, 3 } <br>
a) Find the PMF of X

$P(X=k) = \begin{cases}
               \frac{1}{7} \text{ if } k \in \set{ -3, -2, -1, 0, 1, 2, 3 }
               0 \text{ otherwise }
            \end{cases}
$
b) $E[X] = \frac{1}{7} (-3 -2 -1 +0 + 1 + 2+ 3)$


{{% /example %}}

{{% remarks name="What should you check?" %}}

1. Is every probability between 0 and 1?
2. do all probabilities add up to one?

{{% /remarks %}}


{{% example name="3c" %}}
10 balls, numbered $0, 1, ..., 9$.
You keep drawing without replacement, until you draw the 0 ball.
For $k = 1, 2, 3, ..., 10$, find the probability that you need k draws to get the $0$. $X = $ number of balls drawn until you get the ball $0$.

$P(X = k) = \frac{ \binom{9}{ k-1 } (k-1)! \cdot 1 }{ \binom{ 10 }{k} k! } = \frac{1}{ 10 }$

{{% /example %}}

{{% example name="4d" %}}

Candidate is qualified with probability $q$; <br>
qualified candidate answers correctly with probability $p$; <br>
unqualified answers incorrectly with probability $p$; <br>
answers to different questions are independent.<br>
Company gives a candidate $15$ questions. Will hire if candidate answers all correctly. A candidate is selected at random, given, the test and is hired. Find probability that the candidate is qualified.

H = candidate hired, Q = candidate is qualified.

$P(Q|H) = \frac{ P(H |Q) P(Q)}{ P(H)} = \frac{ P(H|Q) P(Q)}{ P(H|Q) P(Q) + P(H|Q^c) P(Q^c)}= \frac{ p^{15} \cdot q }{ p^{15} \cdot q + (1-p)^{15} \cdot (1-q)}$

{{% /example %}}

{{% example name="" %}}

Let $X$ be uniform on $\set{ a, a+1, ..., b }, a < b integers$, compute $E[X|c \leq X \leq d]$, where $a \leq < d \leq b$.

$\begin{align\*}
  &E[X| c \leq X \leq d] \br
  &= \sum\_{ k=a }^{b} k P(X=k | c \leq X \leq d) \br
  &= \sum\_{ k=c }^{d} k P(X=k | c \leq X \leq d)
\end{align*}$

$\begin{align\*}
  P(X=k | c \leq X \leq d) \br
  &= \frac{ P(X=k, c \leq X \leq d)}{ P(c \leq X \leq d)} \br
  &= \frac{ P(X =k)}{ P(c \leq X \leq d)} \br
  &= \frac{ \frac{1}{ b - a + 1 }}{ \frac{ d -c + 1 }{ b - a +1 }} \br
  &= \frac{1}{ d-c+1 }
\end{align*}$

{{% /example %}}

{{% example name="2" %}}

The number of hours worked in a month by Oscar in a uniform random variable on $\set{ 0,1 ,2, ..., 100 }$. He makes \$1 per hour, but once he has worked 50 hours, he makes \$2 per hour for each addition hour. <br>
If he works more than 75 hours, he has a 50% chance of winning a \$30 prize.<br>
Find the expected value of his pay.


$W = $ k hours work W is uniform  on $\set{ 0, 1, 2, ..., 100 }$

$P(\text{ pay }) = \begin{cases}
             W , 0 \leq W \leq 50  \br
             50+2(W-50) , 51 \leq W \leq 75 \br
             2W - 50 + 30, 76 \leq W \leq 100 \text{ w/ prize } \br
             2W - 50 , 76 \leq W \leq 100 \text{ w/o prize } \br
         \end{cases}$

$\begin{align\*}
  &E[P] =   \br
  &E[P| 0 \leq W \leq 50] P(0 \leq W \leq 50) \br
  &+ E[P| 51 \leq W \leq 75] P(51 \leq W \leq 75) \br
  &+ E[P| 76 \leq W \leq 100 \text{ w/ prize}] P(76 \leq W \leq 100 \text{ w/ prize}) \br
  &+ E[P| 76 \leq W \leq 100 \text{ w/o prize}] P(76 \leq W \leq 100 \text{ w/o prize}) \br
\end{align*}$

{{% /example %}}


{{% example name="3" %}}
Roll 3 fair 6-sided die. <br>
$X\_i = \text{ outcome of roll } i$ <br>
$Y = min(X\_1, X\_2, X\_3)$ <br>
$Z = max(X\_1, X\_2, X\_3)$ <br>

{{% remarks name="technique" %}}

$\begin{align\*}
P(Y \geq k) &= P(min(X\_1, X\_2, X\_3) \geq k) \br
&= P(X\_1 \geq k, X\_2 \geq k, X\_3 \geq k) \br
&= P(X\_1 \geq k) P(X \geq k) P(X\_3 \geq k) \br
&= P(X\_1 \geq k)^3
\end{align*}$

$\begin{align\*}
P(Y = k) &= P(Y \geq k) - P(Y \geq k+1) \br
&= \left\(\frac{ 7-k }{6}\right\)^3 - \left\(\frac{ 7-(k+1)}{6}\right\)^3 \br
\end{align*}$

{{% /remarks %}}


$\begin{align\*}
P(Z \leq k) &= P(max(X\_1, X\_2, X\_3) \leq k) \br
&=P(X\_1 \leq k, X\_2 \leq k, X\_3 \leq k) \br
&=P(X\_1 \leq k)^3 \br
&= \frac{k}{6}^3
\end{align*}$

$P(Z=k) = P(Z \leq k) - P(Z \leq k-1) = \left\(\frac{k}{6} \right\)^3 - \left\(\frac{ k - 1 }{6} \right\)^3$


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

X\_1, X\_2, ..., X\_{125}
Y\_1, ..., Y\_{25}

$P\_{X\_i} (k) =
\begin{cases}
q, k = 1 \br
1-q, k = 0
0 \text{ otherwise }
\end{cases}$

$P\_{Y\_i} (k) =
\begin{cases}
p, k = 1 \br
1-p, k = 0
0 \text{ otherwise }
\end{cases}$

$X\_i =
\begin{cases}
1, \text{ if undergrad gets an A } \br
0 \text{ otherwise }
\end{cases}$

$Y\_i =
\begin{cases}
1, \text{ if grad student gets an A } \br
0 \text{ otherwise }
\end{cases}$

$X = (X\_1 + ... + X\_{125}) + (Y\_1 + ... + Y\_{25})$

$E[X] = E[X\_1] + ... + E[X\_{125}] + E[Y\_1] + ... E[Y\_{25}] = 125q + 25p$

{{% /example %}}

{{% example name="" %}}

n couples will be seated uniformly at random at a circular table $w/ 2n$ chairs
Let $X$ = number of couples who are seated next to each other.

Find $E[X]$.

$X\_i =
\begin{cases}
1, \text{ if couple }i \text{ is seated next to each other } \br
0 \text{ otherwise }
\end{cases}$


Notice that $ X\_1, X\_2, ..., X\_{n}$ are NOT independent.

$E[X] &= E[X\_1] + ... + E[X\_n] \br
&= n E[X\_i] \br
&= n P(couple 1 sits next to each other) \br
&= n(\frac{2}{ n-1 }) \br
&= \frac{ 2n }{ n-1 }$


{{% /example %}}

