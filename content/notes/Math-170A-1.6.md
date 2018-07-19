---
title: "Counting"
date: 2018-07-05T9:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 1.6


---

Counting, permutations, combinations, binomial formula

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

{{% definition name="Counting" %}}
Number of ways to select $k$ objects from a collection of n objects.

- if order matters: "permutation"
- of order doesn't matter: "combination"

{{% /definition %}}


Recall: $m != m(m-1)(m-2) ... 3 \cdot 2 \cdot 1$
Convention: $0!=1$

{{% definition name="Permutation" %}}

Let $k, n$ be integers, $k \leq n$. We have $n$ distince objects, we wish to count number of ways to pick $k$ of these and arrange them in a sequence.
i.e. number of sequences of length $k$ made up of the $n$ objects.

$$
\begin{align\*}
total &= n(n-1)(n-2)...n-(k-1) \br
&=\frac{n(n-1) ... (n-k+1)(n-k) ... 2 \cdot 1}{(n-k)(n-k-1)...2\cdot 1} \br
&=\frac{n!}{(n-k)!}
\end{align*}
$$

In particular, if $k = n$, number of ways to arrange n objects is $n!$.
{{% /definition %}}

{{% definition name="Combinations" %}}
Let $\binom{n}{k}$ denote number of ways to form a $k$-elements subset from $n$ objects.

$\binom{n}{k}$ is called **binomial coefficient**.

$\binom{n}{k} = \frac{n!}{k!(n-k)!}$

or

$n! = \binom{n}{k}k!(n-k)!$

{{% /definition %}}

{{% example name="Toss a coin $n$ times" %}}
$\Omega=\set{(x_1, ..., x_n)| x_i\in\set{\head, \tail}}$

We have $\binom{n}{k} =$ number of distince outcomes in $\Omega$ (i.e. n-toss sequences) that contains exactly $k$ heads.

{{% /example %}}

{{% theorem name="Binomial Formula" %}}
$$\sum_{k=1}^n\binom{n}{k}p^k(1-p)^{n-k} = 1$$


{{% proof name="" %}}
For $0 \leq p \leq 1$, and for $0 \leq p \leq 1$.

Say we have a coin that  comes up $\head$ with probability $p$. We toss it $n$ times, the tosses are independent (as usual). Let $A_k$ be the event that $\head$ compes up exactly $k$ times.

$\abs{A_k} = \binom{n}{k}$

$$
\begin{align\*}
P(A_k) &=\binom{n}{k} \underset{k\text{ times i.e. # heads}}{p ... p}\cdot\underset{n-k\text{ times i.e. # tails}}{(1-p)...(1-p)} \br
&=\binom{n}{k} p^k(1-p)^{n-k}\br
\end{align*}
$$

{{% /proof %}}

{{% /theorem %}}

{{% example name="Draw 7 cards" %}}
Draw 7 cards (w/o replacement) from standard 52 card deck.
Let $A$ be the event you get exactly 3 aces.
Let $B$ be the event you get exactly 2 kings.

$P(A\cup B) = P(A) + P(B) - P(A\cap B)$

Number of ways to choose 7 cards: $\binom{52}{7}$

let's find $P(A)$:
Think of deck as "aces" and "non-aces". <br>
7 cards = exactly 3 aces (out of 4) + 4 other cards. <br>
so total number ways is $\binom{4}{3}\binom{48}{4}$.
$P(A) = \frac{\abs{A}}{\abs{\Omega}} = \frac{\binom{4}{3}\binom{48}{4}}{\binom{52}{7}}$

Similarly,
$P(B) = \frac{\abs{A}}{\abs{\Omega}} = \frac{\binom{4}{2}\binom{48}{5}}{\binom{52}{7}}$

$P(A\cap B) = \frac{\abs{A}}{\abs{\Omega}} = \frac{\binom{4}{3}\binom{4}{2}\binom{44}{2}}{\binom{52}{7}}$

{{% /example %}}
