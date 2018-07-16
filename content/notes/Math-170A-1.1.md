---
title: "Sets"
date: 2018-06-25T9:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 1.1


---

Sets, countability, subset, supset, set operations, algebra of sets, demorgan's Laws.

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\abs}[1]{|#1|}$  
  {{< /raw >}}
</div>

{{% definition %}}

A <strong>set</strong> is a collection of objects, called <strong>elements</strong> of the set.

{{% /definition %}}

# Notations


If $S$ is a set, and $x$ is an element of $S$, we write $x \in S$; if $y$ is not an element of $S$, we write $y \not\in S$.

An <u>empty set</u> is a set which has no elements, denoted $\emptyset$.

If a set $S$ consists of a finite number of elements say $x_1, ..., x_n$ , we write $S=\set{x_1, ..., x_n}$.

{{% examples %}}

1. The set of instructors in this course is $\set{\text{Olga Turanova}}$.
2. The set of letters in the name of this course is $\set{P, r, o, b, a, i, l, t, y, h, e}$.
3. The set of possible outcomes of one coin toss:
   $\set{\text{Head}, \text{Tail}}$.

4. The set of possible outcomes of one coin toss:
   $\set{\text{HH}, \text{HT}, \text{TH}, \text{TT}}$.

{{% /examples %}}

<hr>

# Countability

If $S$ consists of infinitely many elements which can be enumerated in a list, say $x_1, x_2, ...$, we write $S=\set{x_1, x_2, ...}$ & say $S$ is <u>countably infinite</u>.

{{% examples %}}

- $\N =\set{1, 2, 3, ...}$ is countably infinite.
- $\Q​$ is also countably infinite (the reason why will not be covered in this class).

{{% /examples %}}


If the elements of $S$ cannot be enumerated in a list, S is called <u>uncountable</u>

{{% examples %}}

- The real numbers $\R$ are uncountable.
- The interval $(1, 2]$ is uncountable.

{{% /examples %}}

<hr>

# Expression

We may want to consider the set $S$ of all $x$ that satisfy a certain property $P$. We write this as $S=\set{x|x\text{ satisfies }P}$

{{% examples %}}

$\set{x|x>0, \frac{x}{2}\in \N}=\set{2,4,6,8,...}$

Both can describe the set of even natural numbers $S$. 

{{% /examples %}}

<hr>

# Subset, Supset

If every element of $S$ is an element of $T$ (another set), we write $S \subseteq T$ (S is a subset of T) or $T \supseteq S$ ($T$ is a supset of $S$).

$S \subseteq T, T \supseteq S\iff S = T$.

{{% examples %}}

- $S=\set{1, 2}$ 
- $\set{1, 2}\subset S, \set{1,2,3}\not\subset S, 1 \in S, \set{1} \not\in S$
- $\set{5}\in\set{\set{5}, 7, \text{cat}}$
- $\set{5} \subset\set{\set{5}, 7, \text{cat}}$

{{% /examples %}}

<hr>

# Set Operations

We often introduce a universal set, $\Omega$ containing all objects of interest in a particular context.

The <u>complement</u> of $S$ is: $S^c=\set{x\in\Omega|x\not\in S}$.

The <u>union</u> of $S$ & $T$ is: $S\cup T = \set{x\in\Omega | x \in S \text{ or } x \in T}$.

The <u>intersection</u> of $S$ & $T$ is: $S\cap T = \set{x\in\Omega|x \in S \text{ and } x \in T}$. 

(make sure to use "or" or "and", do not use comma.)

${({S^c})^c}=S$

$S\cap S^c=\emptyset$

$S\cup S^c = \Omega$

<hr>

# Algebra of Sets

$S\cap(T\cup V)=(S\cap T)\cup(S\cap V)$

{{% proof %}}

Say $x\in S\cap (T \cup V)$,

Then $x \in S$ and $x\in T\cup V$,

which means $x\in S$ and either $x\in T$ or $x \in V$,

so $x \in S\cap T$ or $x \in S\cap V$,

so $x \in S \cup T$.

{{% /proof %}}

$S\cup(T\cap V)=(S\cup T)\cap(S\cup V)$

<u>De Morgan's Laws</u>, $S_1, S_2,...$ are sets

1. $(\underset{n}{\cup} S_n)^c = \underset n \cap S_n^c$
2. $(\underset{n}{\cap} S_n)^c = \underset n \cup S_n^c$
