---
title: "Probabilistic Models"
date: 2018-06-27T9:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 1.2


---

Sample spaces, outcomes, events, probability law, probability law axioms, discrete probability law, discrete uniform probability law, properties of probability laws.

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

# Probabilistic Models

{{% definition name="Probabilistic Model" %}}
A probabilistic model is a mathematical description of an uncertain situation.

A probabilistic model have two main ingredients: a **sample space** and a **probability law**.
{{% /definition %}}

{{% definition name="Sample Space" %}}

A **sample space** $\Omega$ is a the set of **outcomes** of an experiment.

{{% /definition %}}

{{% definition name="Probability Law" %}}
The **probability law** assigns a set $A$ of possible outcomes (also called an **event**) a nonnegative number $P(A)$ (called the **probability** of $A$).

The probability law should encode our knowledge or belief about the collective "likelihood" of the elements of $A$.

{{% axioms name="Probability Axioms" %}}

Any probability law must satisfies the following axioms:

1. **(Nonnegativity)** $P(A)\geq 0$, for every event $A$.
2. **(Additivity)** if $A_1,A_2,...$ is a sequence of disjoint events, then the probability of their union satisfies $P(A_1\cup A_2 \cup ...)=P(A_1) + P(A_2)+...$.
3. **(Normalization)** $P(\Omega)=1$.

{{% /axioms %}}

{{% /definition %}}

To represent the experiment well, $\Omega $ must be **collectively exhaustive**, In other words, no mather what happens, all outcomes are in $\Omega$, and $\Omega$ consists only of outcomes.



{{% examples %}}

Two coin tosses $\Omega = \set{\text{HH}, \text{TH}, \text{HT}, \text{TT}}$

$\text{HH}$ is an **outcome**, $\set{\text{HH}, \text{TT}}$ is an **event** i.e. "Getting same results on both tosses".


{{% /examples %}}

{{% definition %}}

**probability law** $P$ assigns to each event $A$ a number $P(A)$. called the **probability** of A.

{{% /definition %}}


{{% examples %}}

One fair coin toss $\Omega=\set{H, T}, P(\set{H})=P(\set{T})=0.5$

{{% /examples %}}

{{% definition %}}

Two sets $A,B$ are **disjoint** if $A\cap B=\emptyset$,

{{% /definition %}}

{{% examples %}}

Describe one <u>unfair</u> coin toss where chance of $H$ is $\frac{1}{4}$.

$\Omega =\set{\text{H}, \text{T}}, P(\set{\text{H}})=\frac{1}{4}, P(\set{\text{T}})=\frac{3}{4}$

note: $P(\text{H}\cup\text{T}) = 1$

{{% /examples %}}

{{% properties name="Discrete Probability Law" %}}

If a sample space consists of a **finite** or even just **countable** number of outcomes, then the probability law is specified by the probabilities of the events that consist of a single element. In particular, the probability of any event $\set{s_1,s_2,...,s_n}$ is the sum of the probabilities of its elements:

$$P(\set{x_1, x_2, ..., x_n})=P(\set{x_1})+P(\set{x_2})+...+P(\set{x_n})$$

{{% /properties %}}

We denote the number of possible outcomes in a set of outcomes A as $\abs{A}$.

{{% properties name="Discrete Uniform Probability Law" %}}

If a sample space consists of $n$ possible outcomes which are equally likely, then $\forall$ event $A$, $$P(A) = \abs A \cdot \frac{1}{n}=\frac{\abs{A}}{\abs \Omega}$$

{{% /properties %}}

{{% properties name="Properties of Probability Laws" %}}

Consider a probability law, and let $A$, $B$, and $C$ be events.

1. if $A \subset B$, then $P(A) \leq P(B)$.
2. $P(\emptyset)=0$
3. $P(A^c) = 1 - P(A)$
4. $P(A\cup B) = P(A) + P(B) - P(A\cap B)$

{{% /properties %}}


{{% proof %}}

**Properties of Probability Laws 1**

since $B=A\cup(B\cap A^C)$

$P(B) = P(A) + P(B\cap A^C) $ (prbability axioms 2, Additivity)

$\geq P(A) + 0$ (prbability axioms 1, Positivity)


{{% /proof %}}

{{% proof %}}
**Properties of Probability Laws 2**

$1 = P(\Omega)$     (prbability axioms 3, Normalization)

$=P(\Omega \cup \emptyset)$

$= P(\Omega) + P(\emptyset)$     (prbability axioms 1, Additivity)

$= 1 + P(\emptyset)$

$P(\emptyset) = 0$
{{% /proof %}}

<hr>

# Visualization

Constructing $\Omega$'s' visualizing

e.g. We roll a fair 4-sided die two times

$\Omega = \set{(i, j)| i, j \in \set{1, 2, 3, 4}}$

(Grid representation) (tree representation)

Let $A$ be the event that I roll doubles

$A=\set{(i, i)| i= \set{1 ,2 ,3, 4}}$



You can use array or tree to get an idea of what's going on in a problem, but  to carefully write a solution, write sample space $\Omega$ and events $A$ as explicitly as possible.


{{% example name="Skittles" %}}

A bag of skittles contains $n$ red skittles and $n$ green skittles. Two skittles are removed at the same time (without replacement) at random. What is the probability they're different colors?

**Step 1**: write down sample space $\Omega$.

$\Omega=\set{RR, RG, GG}$ is a correct sample space. However, we cannot use this sample space design, because we cannot assign events with it.

We use $\Omega = \set{1, ..., n, n+1, ..., 2n} $

$= \set{(i,j)| i\neq j, i, j \in\set{1, ..., 2n}}$ as our sample space.

**Step 2**: In this sample space, all outcomes are equally likely.

$\abs\Omega = 2n \times (2n-1)$

$P(\text{RG})=\frac{n\cdot n}{2n(2n-1)}=P(\text{GR})$

$P(\text{diff. colors})=P(\text{RG})+P(\text{GR})$

$=\frac{n^2}{2n(2n-1)} + \frac{n^2}{2n(2n-1)} = \frac{n}{2(2n-1)}$

{{% /example %}}


{{% example name="Romeo and Juliet Have a Date" %}}

Romeo & Juliet have a date. Each will arrive between midnight and 1 am (all times are equally likely). The 1st to arrive will wait 15 minutes for the other and then leave. Probability they meet?

$\Omega = [0, 1] \times [0, 1]$

> This is an example of a model of a continuous sample space. Note $\Omega$ is uncountable. Note $P(\set{x, y}) = 0$

we interpret 'equally likely' to mean $P(A) =$ area of $A$ .

The event that represents "they meet" is $M = \set{(i, j) \in \Omega | \abs{i - j} \leq \frac{1}{4}}$

P(M) = area of M = 1/4

{{% /example %}}
