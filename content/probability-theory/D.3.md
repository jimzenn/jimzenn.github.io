---
title: "Disucission"
date: 2018-07-10T10:03:48+08:00
volumes: ["D"]
layout: "note"
type: "notes"
issue: 3
draft: true


---


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

{{% example name="counting" %}}
(a) a couple is to be seated at a round table with $n \geq 3$ chairs uniformly at random.

What is the probability that the couple is seated next to each other?


$\b{P}(A)=\frac{\text{number of ways to pick 2 chairs next to each other}}{\text{number of ways to pick 2 chairs}}$

Seat person 1 first (they can sit anywhere doesn't matter since table is round) Then, when seating person 2, there are n-1 chairs left, and we want them to end up in one of the 2 chairs next to person 1.
So $\b{P}(A) = \frac{2}{n-1}$

(b) Repeat put (a), but with a rectangular table with the chairs all on one side.

$\b{P}(A) = \frac{\text{number of ways to select 2 chairs next to each other}}{\text{number of ways to select 2 chairs}}$

{{% /example %}}

{{% example name="deck of cards" %}}
A deck of 52 standard standard playing cards is shuffled. What is the probability that the 13th card dealt from top is the first king to be dealt with.

Way 1: multiplication rule
$\b{P}(A)=\frac{48}{52}\frac{47}{51} \frac{46}{50}... \frac{37}{41} \frac{4}{40}$

Way 2:
$\b{P}(A)= \frac{ \text{number of ways to deal 13 cards, first 12 not kings,  then a king}}{ \text{number of ways to deal 13 cards}}$
$= \frac{ \binom{48}{12} \cdot 12! \cdot 4 }{ \binom{52}{13} 13!}$


{{% /example %}}

{{% example name="Urn" %}}
an urn contains m red balls and n white balls.
(a) We draw 2 balls randomly and simultaneously. Describe the sample space and find the probability of drawings balls of different colors.

$\Omega = \set{RR, RW,WW}$

$\b{P}(RW) = \frac{ \binom{m}{1} }{ \binom{n}{1}}$

(b) Suppose we draw with replacement.

$\b{P}( \text{different colors}) = \frac{m}{m+n} \frac{n}{m+n} + \frac{n}{n+m} + \frac{m}{n+m}$

{{% /example %}}

{{% example name="original" %}}
Howmany unique words can be arranged from "original".

$ \binom{8}{2} \binom{6}{1} \binom{5}{1} \binom{4}{1} \binom{3}{1} \binom{2}{1} \binom{1}{1}$

{{% /example %}}

{{% example name="missisippi" %}}
How many unique words can be arranged from "original".

$ \binom{11}{4} \binom{7}{4} \binom{3}{2} \binom{1}{1}$

{{% /example %}}

{{% example name="" %}}
The math department offers 8 lower division subjects $ \set{ L\_1, L\_2, ..., L\_8 }$ and 10 upper division subjects $ \set{ u\_1, u\_2, ..., u\_10 }$ a valid curricullum consists of exactly 4 lower div's and 3 upper div's.

(a) How many valid curricula are there?

$ \binom{8}{4} \binom{10}{3}$

(b) Suppose now that $L_1$ is a prerequisite for $ \set{ u\_1, u\_2, ..., u\_5 }$, $L_2, L_3$ are prereq's for $ \set{ u\_6, u\_2, ..., u\_10 }$ How many valid curricula?

$ \binom{5}{3} \binom{5}{3} + 3 \binom{5}{2} \binom{5}{3} + 5 \binom{10}{3}$

{{% /example %}}

$X$ is uniform on $ \set{1, 2, ..., 1000}$

$ \b{P}( \text{divisible by 2 or 3} ) = \b{P}( \text{2 divides X} ) \b{P}( \text{3 divides X} ) - \b{P}( \text{6 divides X} )$

Random variables

RV's are functions from a single space $ \Omega $ to $ \R $

{{% example name="toss a fair coin twice" %}}

Let X be the number of H's.

$ \Omega = \set{HH, HT, TH, TT}$

$X(HH) =2, X(HT) =X(TH) = 1, X(TT) = 0$

{{% /example %}}

{{% example name="" %}}

Let X be a RV with Probability mass function (PMF)

(b) compute $E[X] = \sum_k k \cdot \b{P}(X=k)$

\(c) Find the PMF of $Y = X^2$

p_Y(y) = \b{P}(Y = y)


(d) compute $E[Y]$

$E[Y] = 0 \b{P}(Y=0) + 1 \b{P}(Y=1)  +4 \b{P}(Y=4)$ = 0 + \frac{1}{5} + 4 \cdot \frac{4}{5} = \frac{17}{5}$

$E[Y]= E[X^2] = \sum_{k \in \set{-2, -1, 0, 1, 2}} K^2 \b{P}(X=k)$


{{% /example %}}


{{% example name="" %}}

X discrete R.V. which is uniform on the integers in the range $[a, b]$ where a, b are integers with $a <0 < b$ X uniform m $ \set{a, a+1, a+2, ..., -1, -, 1, ...}$   (size=-a+b+1).
(a) Find the PMF of $y = max \set{0, X}$. $y \in \set{0, 1,2,..., b}$.

if $k =1,2,..., b, \b{P}(y=k) = \b{P}(max \set{0, x} = k) = \b{P}(X=k) = \frac{1}{-a+b+1}$

$\b{P}(Y =0)=\b{P}(max \set{0,x} 0 = 0)= \b{P}(X \in \set{a + a+1, ..., -1, 0}) = \frac{-a+1}{-a+b+1}$
{{% /example %}}

{{% example name="" %}}
Player A and B play a series of chess games in which the first player to win a game wins the series. After 10 successive draws the series is called a draw.<br>
Each game is won by player A with prob 0.4, won by player B with probability 0.3, and is a draw with probability 0.3.

(a) What is the probability that A wins the series?

W 0.4
DW 0.3 * 0.4
DDW 0.3^2 * 0.4
DDDW 0.3^3 * 0.4
...
DDDDDDDDDW 0.3^9 * 0.4

\b{P}(A wins series) = \sum_(i=0)^9 (.3)^i (.4)

(b) What is the probability mass function of the $X = \text{number of games played}$

$\b{P}(X=1)= .3 + .4 = .7$
$\b{P}(X=2)= .3 (.3 + .4) =.21$
$\b{P}(X=k)= .3^{k-1} (.3 + .4) (k = 1, 2, ..., 9)$

$\b{P}(X=10)= (.3)^{10} +(.3)^9 \times .7$

(c) Find $E[X]$
E[X] = \sum_1^{10}{ k \cdot 3^{k-1} \cdot .7} + 10 \cdot .3

{{% /example %}}


