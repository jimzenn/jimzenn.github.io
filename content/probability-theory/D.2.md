---
title: "Discussion"
date: 2018-07-03T9:03:48+08:00
volumes: ["D"]
layout: "note"
type: "notes"
issue: 2
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
    $\newcommand{\dist}[1]{\text{dist}(#1)}$
    $\newcommand{\max}[1]{\text{max}(#1)}$
    $\newcommand{\min}[1]{\text{min}(#1)}$
    $\newcommand{\supr}[1]{\text{sup}(#1)}$
    $\newcommand{\infi}[1]{\text{inf}(#1)}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
    $\newcommand{\proj}{\text{proj}}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{\left| #1 \right|}$
    $\newcommand{\norm}[1]{\left\lVert#1\right\rVert}$
    $\newcommand{\pare}[1]{\left(#1\right)}$
    $\newcommand{\t}[1]{\text{ #1 }}$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
    $\newcommand{\d}{\text d}$
    $\newcommand{\limu}[2]{\underset{#1 \to #2}\lim}$
    $\newcommand{\inv}[1]{{#1}^{-1}}$
    $\newcommand{\inner}[2]{\langle #1, #2 \rangle}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\rank}[1]{\text{rank }#1}$
    $\newcommand{\var}[1]{\text{var}(#1)}$
    $\newcommand{\tr}[1]{\text{tr}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$
    $\newcommand{\ceil}[1]{\lceil#1\rceil}$
    $\newcommand{\floor}[1]{\lfloor#1\rfloor}$
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

{{% example name="" %}}
$\Omega$ is a sample space, $A, B \subset \Omega$ are events. We know $\b{P}(A)=0.55$, $\b{P}(B^c)=0.35$, and $\b{P}(A\cup B) = 0.75$.

$\b{P}(B) = 1-\b{P}(B^c)=1-0.35=0.65$

$\b{P}(A\cup B) = \b{P}(A)+\b{P}(B)-\b{P}(A\cap B)$

$0.75 = 0.55+0.65-\b{P}(A\cap B)$

{{% /example %}}

{{% example name="Magical 4-sided die" %}}

A magical 4-sided die is rolled twice. Let $S$ be the sum of the two rolls.
We are told that the probability that $S=k$ is proportional to $k$ , for $k = 2,3,4,5,6,7,8$.<br>
Moreover, all possible ways to give sum k are equally likely.<br>
1.construct an appropriate probibility model. <br>
2.Find the probability that doubles are rolled.

There is a fixed constant $c$ s.t. $\b{P}(k)= ck$ for $k = 2, ..., 8$ How to find $c$?

because all these events forms a partition of the sample space,

(a)

$$
\begin{align\*}
\b{P}(\Omega) &= \b{P}(s=2) + \b{P}(2=3) + ... + \b{P}(s=8) \br
1 &= 2c+3c+... +8c \br
1 &= 35c \br
c &= \frac1{35}
\end{align*}
$$

$\b{P}(s=k) = \frac k {35} for k = 2,3,4, ..., 8$

(b)

$\b{P}(\text{Double 1s}) = \b{P}(s=2) = \frac 2{35}$

$\b{P}(s=4) = {(2,2), (1,3), (3, 1)}$

given all possible ways to give sum $k$ are equally likely,

$\b{P}(\text{Double 2s}) = \frac13 \b{P}(s=4) = \frac13 \frac 4{35}$

$\b{P}(\text{Double 3s}) = \frac13 \b{P}(s=6) = \frac13 \frac 6{35}$

$\b{P}(\text{Double 4s}) = \b{P}(s=8) = \frac 8{35}$

$\b{P}(\text{rolling doubles})= ...$

{{% /example %}}

{{% example name="Conditional probability" %}}

we roll 2 fair six-sided die.

**GRID DIAGRAM**

(a) find the probability that doubles were rolled.

$\Omega=\set{(i, j) | i,j = 1,2,...6}$
$\b{P}(\text{roll doubles}))= \frac16$

(b) Given that the sum of the rolls is 4 or less, find the conditional probability that doubles were rolled.

Let $S$ be the sum, $D =$ event that doubles were rolled.

$\b{P}(D|S \leq 4) = \frac{\b{P}(D\cap (S\leq 4))}{\b{P}(S\leq 4)}$

(c\) Find the probability that at least one die lands 6.

let A be the event that at least on die lands 6.

$\b{P}(A) = \b{P}(\text{first roll is 6}) + \b{P}(\text{second roll is 6}) - \b{P}(\text{both land 6})=\frac{11}{36}$

(d) Give that you do not roll doubles, find the conditional probability that at least one die lands 6.
let D be the event you roll doubles.

$\b{P}(A|D^c)=\frac{\b{P}(A\cap D^c)}{\b{P}(D^c)} = \frac{\frac{11}{36}-\frac{1}{36}}{1-\frac{6}{36}}=\frac13$

{{% /example %}}

{{% example name="Tests" %}}

A new test has been developed for determining whether a student is overstressed. The test is $95\%$ accurate if the student is not overstressed; and $85\%$ if the student is.<br>
We know that $99.5\%$ of students are overstressed. Given that a particular student tests negative, what is the probability that the test is accurate?

![Test Problem Partition](/images/test-problems.png)

$N = \b{P}(\text{test negative})$,<br>
$A = \b{P}(\text{test accurate})$,<br>
$B = \b{P}(\text{student is overstressed})$

$\b{P}(A|N) = \frac{\b{P}(A\cap N)}{\b{P}(N)} = \frac{\b{P}(A\cap N)}{\b{P}(N|B)\b{P}(B)+\b{P}(N|B^c)\b{P}(B^c)} = \frac{0.005\times 0.95}{0.005\times 0.95+0.995\times 0.15} = $

{{% /example %}}

{{% example name="Independence" %}}
A source  transmits a signal through a noisy channel. each simbol is a $0$ or a $1$ with probabilities $p$ and $1-p$, and is recieved incorrectly with probabilities $\epsilon\_0$ and $\epsilon\_1$ respectively. Transmissions and errors all independent.

(a) What is the probabilities that the $k$th symbol is accurately received. (call it event A)

$z = k$th transmitted symbol is 0

$$
\begin{align\*}
\b{P}(A) &= \b{P}(A|z)\b{P}(z) + \b{P}(A|z^c)\b{P}(z^c) \br
&=(1-\epsilon)p + (1-\epsilon)(1-p)
\end{align*}
$$

(b) Given that the k^th symbol was received accurately, what's the probability that the $k$th symbol submitted was a zero.

$$
\b{P}(Z|A) = \frac{\b{P}(A|Z)\b{P}(Z)}{\b{P}(A)} = \frac{(1-\epsilon\_0)p}{(1\epsilon\_0)p + (1-\epsilon\_0)(1-p)}
$$

(c\) What's the probability that 1011 is correctly received.

$\b{P}(\text{1 is correctly received}) = 1\epsilon\_1$<br>
$\b{P}(\text{0 is correctly received}) = 1\epsilon\_0$

$$
\begin{align\*}
&\b{P}(\text{1011 correctly received}) \br
&= \b{P}(\text{1 is correctly received})^3\b{P}(\text{0 is correctly received}) \br
&= (1-\epsilon\_1)^3(1-\epsilon)
\end{align*}
$$

(d) suppose each symbol is transmitted 3 times, and the received symbol is decided by majority rule.
What is the probability that a zero is correctly recieved.

$\begin{align\*}
\b{P}(\text{zero received}) &= \b{P}(000) + \b{P}(100) + \b{P}(010) + \b{P}(001) \br
&= (1-\epsilon\_0)^3 + 3\epsilon\_0(1-\epsilon\_0)^2
\end{align*}$

{{% /example %}}

{{% example name="" %}}
Let $A$ and $B$ be events with $A\subset B$. Can $A$ and $B$ be independent?

Yes, if $B = \Omega$, then

$\b{P}(A\cap \Omega) = \b{P}(A) - \b{P}(A) \cdot 1 = \b{P}(A) \cdot \b{P}(\Omega)$
{{% /example %}}

{{% example name="" %}}
We know that $A$ and $B$ are independent, and that $A$ and $C$ are independent. Does it follow that $A$ and $B\cup C$ are independent?

No, it does not follow.

A = {HH, TH}
B = {HH, HT}
C = {HH, TT}

$\b{P}(A) = \b{P}(B) = P\(C) = \frac12, \b{P}(B\cup C) = \frac34$

$\b{P}(A\cap(B\cup C)) = \b{P}(HH) = \frac14 \neq \frac13 \frac34 = \b{P}(A)\b{P}(B\cup C)$

But,
$\b{P}(A\cap B) = \b{P}(HH) = \frac14 = \frac12 \frac12 = \b{P}(A)\b{P}(B)$

and similarly for A and C.

{{% /example %}}

{{% definition name="Mutually independent" %}}

$A, B, C$ are mutually independent if<br>
1.The pairs$(A,B),(A,C),(B,C)$ all independent
2.$\b{P}(A\cap B\cap C) = \b{P}(A)\b{P}(B)P\(C)$

{{% /definition %}}

{{% example name="" %}}

Suppose $A,B, C$ are mutually independent, show that A and $B\cup C$ are independent (contrast this with previous example, we have a stronger hypothesis here!)

$\b{P}(A\cap(B\cup C))$<br>
$= \b{P}((A\cap B) \cup (A\cap C))$<br>
$= \b{P}(A\cap B)+\b{P}(A\cap) - \b{P}(A\cap B \cap C)$<br>
$= \b{P}(A)(\b{P}(B) + P\(C) -\b{P}(B)P\(C))$<br>
$= \b{P}(A)(\b{P}(B) + P\(C) - \b{P}(B\cap C))$

{{% /example %}}
