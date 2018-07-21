---
title: "Conditional Probability"
date: 2018-06-28T9:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 1.3


---

Conditional probability.

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
    $\newcommand{\head}{\text{H}}$
    $\newcommand{\tail}{\text{T}}$
  {{< /raw >}}
</div>


Toss a fair coin 3 times:

1. Probability that we get more $\head$ than $\tail$?
2. Given that the 1st one is $\head$, probability of getting more $\head$ than $\tail$?

$$
\begin{align\*}
\Omega & = \set{A_1 A_2 A_3| A_1 A_2 A_3 \in \set{\head, \tail}} \br
       & = \set{\text{HHH, HHT, HTH, HTT, TTT,TTH, THT, THH}}
\end{align\*}
$$

1. $P(\text{more H than T})=P(\text{HHH, HHT, HTH, THH})= \frac 12 $
2. $P(\text{given 1st is H, more H than T})=P(\text{HHH, HHT, HTH})= \frac 34 $

More generally, we are given a sample space $\Omega$, a probility law $P$, suppose $B \subseteq \Omega, P(B) > 0, P(B) > 0.$

In our example, let $A =\set{\text{more H than T}}, B = \set{\text{1st one is H}}$. We found, by counting $|B|=4$, and $|A\cap B| = 3$. Note $\frac{3}{4}=\frac{P(A\cap B)}{P(B)}$.


{{% definition name="Conditional Probability" %}}

We denote the <strong>conditional probability of $A$ given $B$</strong> by $P(A|B)$.

$$P(A|B)=\frac{P(A\cap B)}{P(B)}$$

{{% /definition %}}

{{% example name="Roll a Fair Die" %}}

Roll a fair die. Suppose we know the outcome is  even. What is the probability that outcome is 6?

$$\Omega = \set{1, 2, 3, 4, 5, 6}, A = \set{6}, B=\set{2,4,6}$$
$P(A|B)=\frac{P(A\cap B)}{P(B)}=\frac{P(\set{6})}{P(B)}= \frac{\frac16}{\frac36}=\frac13$

Note: If $P(B) = 0$, then $P(A\cap B) = 0, $ since $P(A\cap B) \subset P(B)$

So in this case, $P(A\cap B) = P(A|B) P(B)​$ since both are zero.

So $P(A\cap B) = P(A|B)P(B), \forall A, B \subset \Omega$.

{{% /example %}}

For $B$ with $P(B)>0, P(X|B)$ is a probability law on $\Omega$.

{{% proof %}}

1. possitivity: $P(A|B) =\frac{P(A\cap B)}{P(B)}\geq 0,  \forall A$
2. addtivity: let $A, C$ be disjoint, $P((A\cup C)| B)=\frac{P((A\cup C)\cap B)}{P(B)}=\frac{P((A\cap B)\cup (C\cap B)}{P(B)} = \frac{P(A\cap B)+ P(C \cap B)}{P(B)}=P(A|B)+P(A|C)$
3. normalization??

{{% /proof %}}


{{% example name="Fair 4-sided die " %}}

We roll a fair, 4 sided die twice. let $x$ denote result of 1st roll, let $y$ denote result of 2nd roll. Let $B$ be the event $B=\set{(x,y)\in\Omega|\text{min}(x,y)=2}$. Determine $P(A_n| B)$, where for $n = \set{1, 2, 3, 4}$, $A_n$ is the event $A_n=\set{max(x,y) = n}$.

$B=\set{(2,2),(2,3),(3,2),(2,4),(4,2)}, P(B)=\frac5{16}$

$P(A_1|B)=\frac{P(A_1\cap B))}{P(B)}=\frac{0}{P(B)}=0$

$P(A_2|B)=\frac{P(A_2\cap B))}{P(B)}=\frac{1/ 16}{5/ 16}=1/ 5$

$P(A_3|B)=\frac{P(A_3\cap B))}{P(B)}=\frac{2/ 16}{5/ 16}=2/ 5$

$P(A_4|B)=\frac{P(A_4\cap B))}{P(B)}=\frac{2/ 16}{5/ 16}=2/ 5$

{{% /example %}}



