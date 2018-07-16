---
title: "Discussion"
date: 2018-06-25T9:03:48+08:00
author: "Tyler Arant"
volumes: ["MATH 170A"]
layout: "note"
issue: D1
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
  {{< /raw >}}
</div>


Proposition $ A, B_1, B_2 ... $ all subsets of $ \Omega$

Show $A\cup(\cap B_n)= \cap (A\cup B_n)$

(For example $\Omega=\mathbb{R}, B_n=[0, \frac{1}{n}], then \cap [0, \frac{1}{n}]=\{0\}$)

Let $\omega \in A \cup (\cap B_n),$ we have two cases:

case 1: $\omega \in A$, Then $\omega \in A \cup B_n \forall n$ , so $\omega \in (A\cup B_n)$

case 2: $\omega \in B_n$, so $\forall n, \omega \in B_n$. This implies $\omega \in A \cup B_n, \forall n$, thus $\omega \in (A\cup B_n)$

So we conclude that,



Question A,B,C be sets, are the following two properties equivalent?

1. $A\cap B \cap C = \emptyset$

2. $A\cap B \neq \emptyset$ and $A \cap C = \emptyset$ and $B \cap C = \emptyset$ (i.e. A, B, C are pairwise disjoint)

$(1) \not\implies (2), (2) \implies (1)$



{{% example name="Monty Hall Problem" %}}

There are three doors. One has a new car, the other two have goats. You select the door you think the car is behind. Of the two unselected doors, at least one has a goat. Monty will open the unselected door with a goat. Next, he asks if you want to swap doors. Should you swap?


<strong>YES</strong>. you should swap.

Let $C$ be choosing the door with a car, let $G_1$ and $G_2$ be choosing one of the doors with a goat.

<strong>Case 1: swap.</strong>


Now let's consider the sample space $\Omega$.

$$\Omega = \set{ CG, G_1C, G_2C }$$

Since the player has no knowledge about the three doors, the first choice must be random. Therefore, all three doors have the same probability to be chosen,

$$P(CG) = P(G_1C) = P(G_2C)$$

The probability of the player winning a car in the end is:

$$P(\text{win})=P(\set{G_1C, G_2C}) = \frac23$$

In other words, if you swap, you win the game if and only if you select the wrong door at the beginning.

<strong>Case 2: don't swap.</strong> 

Let's consider the sample space $\Omega$.

$$\Omega = \set{ CC, G_1G_1, G_2G_2 }$$

$$P(CC) = P(G_1G_1) = P(G_2G_2)$$

$$P(\text{win})=P(\set{CC}) = \frac13$$

So with the swap you have 2/3 chance of winning, but without swap you only have 1/3 chance.

In other words, if you do not swap, you win the game if and only if you select the correct door at the beginning.

{{% /example %}}


{{% example name="Monty Hall Problem, but the Host Does Not Know" %}}

Now, lets say the host does not know where the car is as well. After you pick a door, Monty will randomly pick an unselected doors. If the door reveals a car, the game stops. You lose. If the door reveals a goat, you are given a chance to swap. Should you swap?

Let $C$ be choosing the door with a car, let $G_1$ and $G_2$ be choosing one of the doors with a goat.

<strong>Case 1: swap.</strong> 

Now let's consider the sample space $\Omega$.

$$\Omega = \set{ G_1C, G_2C, CG, G_1G_2, G_2G_1 }$$

we seek $P(\set{G_1C, G_2C})$


Since the player has no knowledge about the three doors, the first choice must be random. Therefore, all three doors have the same probability to be chosen,

$$P(CG) = P(G_1C) = P(G_2C)$$

The probability of the player winning a car in the end is:

$$P(\text{win})=P(\set{G_1C, G_2C}) = \frac23$$

<strong>Case 2: don't swap.</strong> If you do not swap then you win the game if and only if you select the correct door at the beginning.

Now let's consider the sample space $\Omega$*.

$$\Omega = \set{ CC, G_1G_1, G_2G_2 }$$

Since the player has no knowledge about the three doors, the first choice must be random. Therefore, all three doors have the same probability to be chosen,

$$P(CC) = P(G_1G_1) = P(G_2G_2)$$

$$P(\text{win})=P(\set{CC}) = \frac13$$

So with the swap you have 2/3 chance of winning, but without swap you only have 1/3 chance.

{{% /example %}}




A four-sided die is rolled repeatedly, until the first time an even number is rolled. What is the sample space?

> ?$\Omega=\{1, 2, 3, 4, 5\}$
>
> ?$\Omega=\{(i, j), i\in\{1, 2, 3, ...\}, j\in\{2, 4\}\}$
>
> ? $\Omega=\{2, 4\}$