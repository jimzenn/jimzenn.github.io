---
title: "Discussion"
date: 2018-07-03T9:03:48+08:00
author: "Tyler Arant"
volumes: ["MATH 170A"]
layout: "note"
issue: D2


---

Properties of prababilistic laws, conditional probability, tests, and indipendence.

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

{{% example name="" %}}
$\Omega$ is a sample space, $A, B \subset \Omega$ are events. We know $P(A)=0.55$, $P(B^c)=0.35$, and $P(A\cup B) = 0.75$.

$P(B) = 1-P(B^c)=1-0.35=0.65$

$P(A\cup B) = P(A)+P(B)-P(A\cap B)$

$0.75 = 0.55+0.65-P(A\cap B)$

{{% /example %}}

{{% example name="Magical 4-sided die" %}}

A magical 4-sided die is rolled twice. Let $S$ be the sum of the two rolls.
We are told that the probability that $S=k$ is proportional to $k$ , for $k = 2,3,4,5,6,7,8$.<br>
Moreover, all possible ways to give sum k are equally likely.<br>
1.construct an appropriate probibility model. <br>
2.Find the probability that doubles are rolled.

There is a fixed constant $c$ s.t. $P(k)= ck$ for $k = 2, ..., 8$ How to find $c$?

because all these events forms a partition of the sample space,

(a)

$$
\begin{align\*}
P(\Omega) &= P(s=2) + P(2=3) + ... + P(s=8) \\\\\\
1 &= 2c+3c+... +8c \\\\\\
1 &= 35c \\\\\\
c &= \frac1{35}
\end{align*}
$$

$P(s=k) = \frac k {35} for k = 2,3,4, ..., 8$

(b)

$P(\text{Double 1s}) = P(s=2) = \frac 2{35}$

$P(s=4) = {(2,2), (1,3), (3, 1)}$

given all possible ways to give sum $k$ are equally likely,

$P(\text{Double 2s}) = \frac13 P(s=4) = \frac13 \frac 4{35}$

$P(\text{Double 3s}) = \frac13 P(s=6) = \frac13 \frac 6{35}$

$P(\text{Double 4s}) = P(s=8) = \frac 8{35}$

$P(\text{rolling doubles})= ...$

{{% /example %}}

{{% example name="Conditional probability" %}}

we roll 2 fair six-sided die.

**GRID DIAGRAM**

(a) find the probability that doubles were rolled.

$\Omega=\set{(i, j) | i,j = 1,2,...6}$
$P(\text{roll doubles}))= \frac16$

(b) Given that the sum of the rolls is 4 or less, find the conditional probability that doubles were rolled.

Let $S$ be the sum, $D =$ event that doubles were rolled.

$P(D|S \leq 4) = \frac{P(D\cap (S\leq 4))}{P(S\leq 4)}$

\(c) Find the probability that at least one die lands 6.

let A be the event that at least on die lands 6.

$P(A) = P(\text{first roll is 6}) + P(\text{second roll is 6}) - P(\text{both land 6})=\frac{11}{36}$

(d) Give that you do not roll doubles, find the conditional probability that at least one die lands 6.
let D be the event you roll doubles.

$P(A|D^c)=\frac{P(A\cap D^c)}{P(D^c)} = \frac{\frac{11}{36}-\frac{1}{36}}{1-\frac{6}{36}}=\frac13$

{{% /example %}}

{{% example name="Tests" %}}

A new test has been developed for determining whether a student is overstressed. The test is $95\%$ accurate if the student is not overstressed; and $85\%$ if the student is.<br>
We know that $99.5\%$ of students are overstressed. Given that a particular student tests negative, what is the probability that the test is accurate?

![Test Problem Partition](/images/test-problems.png)

$N = P(\text{test negative})$,<br>
$A = P(\text{test accurate})$,<br>
$B = P(\text{student is overstressed})$

$P(A|N) = \frac{P(A\cap N)}{P(N)} = \frac{P(A\cap N)}{P(N|B)P(B)+P(N|B^c)P(B^c)} = \frac{0.005\times 0.95}{0.005\times 0.95+0.995\times 0.15} = $

{{% /example %}}

{{% example name="Independence" %}}
A source  transmits a signal through a noisy channel. each simbol is a $0$ or a $1$ with probabilities $p$ and $1-p$, and is recieved incorrectly with probabilities $\epsilon_0$ and $\epsilon_1$ respectively. Transmissions and errors all independent.

(a) What is the probabilities that the $k$th symbol is accurately received. (call it event A)

$z = k$th transmitted symbol is 0

$$
\begin{align\*}
P(A) &= P(A|z)P(z) + P(A|z^c)P(z^c) \\\\\\
&=(1-\epsilon)p + (1-\epsilon)(1-p)
\end{align*}
$$

(b) Given that the k^th symbol was received accurately, what's the probability that the $k$th symbol submitted was a zero.

$$
P(Z|A) = \frac{P(A|Z)P(Z)}{P(A)} = \frac{(1-\epsilon_0)p}{(1\epsilon_0)p + (1-\epsilon_0)(1-p)}
$$

\(c) What's the probability that 1011 is correctly received.

$P(\text{1 is correctly received}) = 1\epsilon_1$<br>
$P(\text{0 is correctly received}) = 1\epsilon_0$

$$
\begin{align\*}
&P(\text{1011 correctly received}) \\\\\\
&= P(\text{1 is correctly received})^3P(\text{0 is correctly received}) \\\\\\\
&= (1-\epsilon_1)^3(1-\epsilon)
\end{align*}
$$

(d) suppose each symbol is transmitted 3 times, and the received symbol is decided by majority rule.
What is the probability that a zero is correctly recieved.

\begin{align\*}
P(\text{zero received}) &= P(000) + P(100) + P(010) + P(001) \\\\\\
&= (1-\epsilon_0)^3 + 3\epsilon_0(1-\epsilon_0)^2
\end{align*}

{{% /example %}}

{{% example name="" %}}
Let $A$ and $B$ be events with $A\subset B$. Can $A$ and $B$ be independent?

Yes, if $B = \Omega$, then

$P(A\cap \Omega) = P(A) - P(A) \cdot 1 = P(A) \cdot P(\Omega)$
{{% /example %}}

{{% example name="" %}}
We know that $A$ and $B$ are independent, and that $A$ and $C$ are independent. Does it follow that $A$ and $B\cup C$ are independent?

No, it does not follow.

A = {HH, TH}
B = {HH, HT}
C = {HH, TT}

$P(A) = P(B) = P\(C) = \frac12, P(B\cup C) = \frac34$

$P(A\cap(B\cup C)) = P(HH) = \frac14 \neq \frac13 \frac34 = P(A)P(B\cup C)$

But,
$P(A\cap B) = P(HH) = \frac14 = \frac12 \frac12 = P(A)P(B)$

and similarly for A and C.

{{% /example %}}

{{% example name="" %}}
Suppose $A,B, C$ are mutually independent, show that A and $B\cup C$ are independent (contrast this with previous example, we have a stronger hypothesis here!)

{{% definition name="Mutually independent" %}}

$A, B, C$ are mutually independent if<br>
1.The pairs$(A,B),(A,C),(B,C)$ all independent
2.$P(A\cap B\cap C) = P(A)P(B)P\(C)$

{{% /definition %}}

$P(A\cap(B\cup C))$<br>
$= P((A\cap B) \cup (A\cap C))$<br>
$= P(A\cap B)+P(A\cap) - P(A\cap B \cap C)$<br>
$= P(A)(P(B) + P\(C) -P(B)P\(C))$<br>
$= P(A)(P(B) + P\(C) - P(B\cap C))$

{{% /example %}}
