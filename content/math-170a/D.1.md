---
title: "Discussion"
date: 2018-06-25T9:03:48+08:00
volumes: ["D"]
layout: "note"
issue: 1

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
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
    $\newcommand{\t}[1]{\text{ #1 }}$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
    $\newcommand{\inv}[1]{{#1}^{-1}}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\rank}[1]{\text{rank}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$


    $\newcommand{\Vcw}[2]{\begin{pmatrix} #1 \br #2 \end{pmatrix}}$
    $\newcommand{\Vce}[3]{\begin{pmatrix} #1 \br #2 \br #3 \end{pmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \end{pmatrix}}$
    $\newcommand{\Vct}[5]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{pmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{pmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{pmatrix}}$

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

Proposition $ A, B\_1, B\_2 ... $ all subsets of $\Omega$

Show $A\cup(\cap B\_n)= \cap (A\cup B\_n)$

(For example $\Omega=\mathbb{R}, B\_n=[0, \frac{1}{n}], then \cap [0, \frac{1}{n}]=\{0\}$)

Let $\omega \in A \cup (\cap B\_n),$ we have two cases:

case 1: $\omega \in A$, Then $\omega \in A \cup B\_n \forall n$ , so $\omega \in (A\cup B\_n)$

case 2: $\omega \in B\_n$, so $\forall n, \omega \in B\_n$. This implies $\omega \in A \cup B\_n, \forall n$, thus $\omega \in (A\cup B\_n)$

So we conclude that,



Question A,B,C be sets, are the following two properties equivalent?

1. $A\cap B \cap C = \emptyset$

2. $A\cap B \neq \emptyset$ and $A \cap C = \emptyset$ and $B \cap C = \emptyset$(i.e. A, B, C are pairwise disjoint)

$(1) \not\implies (2), (2) \implies (1)$



{{% example name="Monty Hall Problem" %}}

There are three doors. One has a new car, the other two have goats. You select the door you think the car is behind. Of the two unselected doors, at least one has a goat. Monty will open the unselected door with a goat. Next, he asks if you want to swap doors. Should you swap?


<strong>YES</strong>. you should swap.

Let $C$ be choosing the door with a car, let $G\_1$ and $G\_2$ be choosing one of the doors with a goat.

<strong>Case 1: swap.</strong>


Now let's consider the sample space $\Omega$.

$$\Omega = \set{ CG, G\_1C, G\_2C }$$

Since the player has no knowledge about the three doors, the first choice must be random. Therefore, all three doors have the same probability to be chosen,

$$P(CG) = P(G\_1C) = P(G\_2C)$$

The probability of the player winning a car in the end is:

$$P(\text{win})=P(\set{G\_1C, G\_2C}) = \frac23$$

In other words, if you swap, you win the game if and only if you select the wrong door at the beginning.

<strong>Case 2: don't swap.</strong>

Let's consider the sample space $\Omega$.

$$\Omega = \set{ CC, G\_1G\_1, G\_2G\_2 }$$

$$P(CC) = P(G\_1G\_1) = P(G\_2G\_2)$$

$$P(\text{win})=P(\set{CC}) = \frac13$$

So with the swap you have 2/3 chance of winning, but without swap you only have 1/3 chance.

In other words, if you do not swap, you win the game if and only if you select the correct door at the beginning.

{{% /example %}}


{{% example name="Monty Hall Problem, but the Host Does Not Know" %}}

Now, lets say the host does not know where the car is as well. After you pick a door, Monty will randomly pick an unselected doors. If the door reveals a car, the game stops. You lose. If the door reveals a goat, you are given a chance to swap. Should you swap?

Let $C$ be choosing the door with a car, let $G\_1$ and $G\_2$ be choosing one of the doors with a goat.

<strong>Case 1: swap.</strong>

Now let's consider the sample space $\Omega$.

$$\Omega = \set{ G\_1C, G\_2C, CG, G\_1G\_2, G\_2G\_1 }$$

we seek $P(\set{G\_1C, G\_2C})$


Since the player has no knowledge about the three doors, the first choice must be random. Therefore, all three doors have the same probability to be chosen,

$$P(CG) = P(G\_1C) = P(G\_2C)$$

The probability of the player winning a car in the end is:

$$P(\text{win})=P(\set{G\_1C, G\_2C}) = \frac23$$

<strong>Case 2: don't swap.</strong> If you do not swap then you win the game if and only if you select the correct door at the beginning.

Now let's consider the sample space $\Omega$*.

$$\Omega = \set{ CC, G\_1G\_1, G\_2G\_2 }$$

Since the player has no knowledge about the three doors, the first choice must be random. Therefore, all three doors have the same probability to be chosen,

$$P(CC) = P(G\_1G\_1) = P(G\_2G\_2)$$

$$P(\text{win})=P(\set{CC}) = \frac13$$

So with the swap you have 2/3 chance of winning, but without swap you only have 1/3 chance.

{{% /example %}}




A four-sided die is rolled repeatedly, until the first time an even number is rolled. What is the sample space?

> ?$\Omega=\{1, 2, 3, 4, 5\}$
>
> ?$\Omega=\{(i, j), i\in\{1, 2, 3, ...\}, j\in\{2, 4\}\}$
>
> ? $\Omega=\{2, 4\}$
