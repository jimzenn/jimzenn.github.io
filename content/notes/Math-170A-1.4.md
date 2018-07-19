---
title: "Total Probability Theorem and Bayes' Rule"
date: 2018-06-29T9:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 1.4


---

Total probability theorem, partition, inference, bayes law.

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

{{% theorem name=" Simplified version of Total Probability Theorem" %}}

let $B \subset \Omega$, for any event $A$ , $A\cap B$ and $A\cap B^c$ are **disjoint**. $$P(A) = P(A\cap B) + P(A\cap B^c)=P(A|B)P(B)+P(A|B^c)P(B^c)$$

{{% /theorem %}}

{{% example name="yogurt" %}}

At the store there are two flavours of yogurt, apple and berry. There are 100 Apple yogurts and 20% of which are expired; there are 200 Berry yogurts and 10% of which are expired.
<br>
I choose a yogurt at random. What's the chance that it's expired?

Let $E$ denote the event that yogurt I get is expired. <br>
Let $A$ and $B$ respectively denote the events that I get Apple or Berry yogurt.

$P(E) = P(E|A)P(A)+P(E|B)P(B)=P(E|A)P(A)+P(E|A^c)P(A^c)$

$=20\%\times\frac{100}{300}+10\%\times\frac{200}{300}$

$=\frac{2}{15}$

{{% /example %}}


{{% example name="yogurt2" %}}

A different store has same selection of apple and berry (same \% are expired) plus 300 Cherry yogurts, 5% of which are expired.

$P(E) = P(E|A)P(A)+P(E|B)P(B)+ P(E|C)P(C )$

$=20\%\times\frac{100}{600}+10\%\times\frac{200}{600}+5\%\times\frac{300}{600}$

$=\frac{11}{120}$



{{% /example %}}

{{% definition name="Partition" %}}

We say $B_1, B_2...$, are partitions of $\Omega,$ if $B_i \cap B_j = \emptyset$ for $ i\neq j$ and $\underset i \cup B_i = \Omega$.

{{% /definition %}}

 {{% theorem name=" Total Probability Theorem" %}}

If $B_1,B_2,... $ partitions $\Omega$ and $A\subset \Omega$, then  A = $\underset i \cup(A\cap B_i)$ and this is a disjoint union. Thus,
$$P(A) = \underset i \Sigma P(A|B_i)P(B_i)$$

 {{% /theorem %}}

{{% example name="Stack of Cards" %}}

Standard deck of 52 cards (4 suits, each suite has 13 cards, 2-10, J, Q, K, A).

> I draw a card at random.

$P(\text{not a heart}) = \frac34$

> Draw 2 cards (without replacement). $P(\text{neither is a heart}) = ?$

let $A_i$ be the event that $i$th card is not a heart.

$P(\text{neither is a heart}) = P(A_1\cap A_2)$

$P(A_1\cap A_2)=P(A_2 | A_1)P(A_1)= \frac{38}{51}\times \frac{39}{52}$

$P(A_1\cap A_2\cap A_3) =?$

In general, let $B_1, B_2, ..., B_n$ be events of positive probability. Note the telescoping product:

$P(\underset {i=1}{\overset n \cap} B_i)=P(B_1)\frac{P(B_1\cap B_2)}{P(B_1)}\frac{P(B_1\cap B_2 \cap B_3)}{P(B_1\cap B_2)}...\frac{P(\underset {i=1}{\overset n \cap} B_i)}{P(\underset {i=1}{\overset {n-1} \cap} B_i)}$

$P(\underset {i=1}{\overset n \cap} B_i)=P(B_1)P(B_2|B_1)P(B_3|B_1\cap B_2)...P(B_n|\underset {i=1}{\overset {n-1} \cap} B_i)$

$P(A_1\cap A_2\cap A_3) =P(A_1)\cdot P(A_2|A_1)\cdot P(A_3|A_1 \cap A_2)=\frac{39}{52}\cdot \frac{38}{51} \cdot \frac{37}{50}$

{{% /example %}}

# Inference

We have $A_1, ..., A_n$ underlying causes, i.e. events that form a partition of $\Omega$, and an "effect" or "observation" $B \subset \Omega$. I know $P(B|A_i)$, $i= 1, ... ,n$.

Want to know if I observe a $B$, how likely is it that $A_i$ was the cause?

I know $P(A_i)$ for $i=1,2,...,n$

Then $P(A_j|B)=\frac{P(A_j \cap B)}{P(B)}=\frac{P(B|A_j)P(A_j)}{P(B)}$

since $A_1, ..., A_n$ partition $\Omega$, $P(B)=\underset {i=1}{\overset {n} \Sigma} P(B|A_i)P(A_i),$

{{% theorem name="Bayes Rule" %}}

Let $A_1 , A_2, ..., A_n$ be disjoint events that form a partition of the sample space, and assume that $P(A_i) > 0, \forall i$. Then, for any event $B$ such that $P(B) > 0$, we have

$$P(A|B)= \frac{P(B|A\_j)P(A\_j)}{\underset {i=1}{\overset {n} \Sigma} P(B|A\_i)P(A\_i)}$$

{{% /theorem %}}

{{% example name="2 coins" %}}

We have 2 coins, coin 1 shows H with probability $90\%$, coin 2 shows H with probability $5\%$. They look the same. I pick one at random & toss it shows H. Chance it is coin 1?

"causes": picking the coin. Let $A_1$ be event I got coin 1, $A_2$ be event I got coin 2.

$B$ is event I got H tossing. seek $P(A_1|B)$.

Using Bayes rule,

$P(A_1|B)=\frac{P(B|A_1)P(A_1)}{P(B)}=\frac{P(B|A_1)P(A_1)}{P(B|A_1)P(A_1)+P(B|A_2)P(A_2)}=\frac{90\%\times\frac12}{90\%\times\frac12+5\%\frac12}=\frac{18}{19}$

{{% /example %}}

{{% example name="Disease" %}}
Some scientists design a test for a disease. The disease occurs 0.1% of the population. If the person has disease, test identifies 95% of the time; if the person has no disease, test gives negative result 95% of the time. Question: if a person picked at random from population tests positive, how likely is it that they have the disease?

Setup:
Let $A$ be the event that person has the disease.
Note: $A$ & $A^c$ are a partition.
Let $B$ be the event that the person test positive.
We seek $P(A|B)$ by Bayes' Law.

$$
\begin{align\*}
P(A|B) &= \frac{P(B|A)P(A)}{P(B|A)P(A) + P(B|A^c)P(A^c)} \br
&= \frac{0.95\times 0.001}{0.95\times 0.001 + 0.05 \times 0.999} \br
&= 0.0187 = 1.8\%
\end{align*}
$$

{{% /example %}}

Sometimes we want to capture idea that "knowing that $B \subset \Omega$ occrued gives no info about whether $A$ occured, \& vice versa". If this is the case, we think $P(A|B)=P(A).$ A more formal definition:
