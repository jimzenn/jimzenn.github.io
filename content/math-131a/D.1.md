---
title: "Discussion"
date: 2018-08-07T11:03:48+08:00
menuTitle: "Analysis"
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
    $\newcommand{\N}{\mathcal{N}}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
    $\newcommand{\proj}{\text{proj}}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{| #1 |}$
    $\newcommand{\norm}[1]{\left\lVert#1\right\rVert}$
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
    $\newcommand{\t}[1]{\text{ #1 }}$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
    $\newcommand{\d}{\text d}$
    $\newcommand{\limu}[2]{\underset{#1 \to #2}\lim}$
    $\newcommand{\inv}[1]{{#1}^{-1}}$
    $\newcommand{\inner}[2]{\langle #1, #2 \rangle}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\rank}[1]{\text{rank}(#1)}$
    $\newcommand{\var}[1]{\text{var}(#1)}$
    $\newcommand{\tr}[1]{\text{tr}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$
    $\newcommand{\Re}[1]{\text{Re}(#1)}$
    $\newcommand{\Im}[1]{\text{Im}(#1)}$


    $\newcommand{\Vcw}[2]{\begin{pmatrix} #1 \br #2 \end{pmatrix}}$
    $\newcommand{\Vce}[3]{\begin{pmatrix} #1 \br #2 \br #3 \end{pmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \end{pmatrix}}$
    $\newcommand{\Vct}[5]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{pmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{pmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{pmatrix}}$

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

TA: Thomas Gilton
tdgilton@math.ucla.edu
math.ucla.edu/~tdgilton
Office MS 6603
OH Th 9:45 - 10:50 and 1pm - 2:15 pm

(This thursday, staart @ 10:15)

Email is great.

Section 1

1A propositional logic

start with basic statements and for mmore complicated ones

connections lite

$\land \lor \neg \to $

idea truth value of a "complicated statement" is a function of the T vals of simple props

"Truth tables"

| $p$ | $q$ | $p \land q $ | $p \lor q $ | $p \to q $ |
| --- | --- | ---           | ---          | ---         |
| T   | T   | T             | T            | T           |
| T   | F   | T             | F            | F           |
| F   | T   | T             | F            | T           |
| F   | F   | F             | F            | T           |


{{% example name="" %}}

" If 2 + 2 = 5, then whales are cats. "

True.

{{% /example %}}

{{% example name="" %}}

If $x > 0 $, then $2x > 0 $.

{{% proof index="" name="" %}}

We assume $x > 0$. By field axiom (n), 2x > x.

Since $< $ is transitive, then $2x > x $ and $x > 0 $ implies 2x > 0.

Q.E.D.

{{% /proof %}}

{{% /example %}}

Upshot: when you want to prove $p \to \sigma $, assume the "$p$", and argue for " $\sigma$".

HW guidelines

1. stable

2. First, Last, student ID $\to $ to the top right

3. Own work

3.1 Collaboration ... encouraged!

3.2 DO NOT COPY. Internet ... don't copy!

3.3 cite! Collaborators

4. Neat clear arguments, lots of details.


Common mistakes of implications

Some argue like

$p \to q; q; \therefore p$

$\neg q; \neg q \to \neg p; p \to q$

which is NOT true.

{{% note name="" %}}

$\neg q \to \neg p$

conclude $\neg \neg p \to \neg \neg q $

but $\neg \neg r $ equivalent to $r $, so "same"

{{% /note %}}

HOW TO NEGATE

$\neg (p \land q) \equiv \neg p \lor \neg q $

$\neg (p \lor q) \equiv \neg p \land \neg q $

$\neg p \to q \equiv p \land \neg q $

{{% proof index="" name="" %}}

$p \to q \equiv \neg p \lor q $

state that as a fact

$\neg p \to q  \equiv \neg (\neg p \lor q)$

$\equiv \neg \neg p \land \neg q \equiv p \land \neg q$

{{% /proof %}}

{{% example name="" %}}

Negate the following

 $p \to (q \lor r) $ <br>
 $p \land (q \lor r) $ <br>
 $(p \land q) \to r $ <br>
 $p \land (q \to r) $

$\neg p \to (q \lor r) \equiv \neg (\neg p \lor (q \lor r)) \equiv p \land \neg q \land \neg r $

$\neg (p \land (q \lor r)) \equiv \neg \neg p \lor \neg (q \lor r) \equiv p \lor (\neg q \land \neg r) $

$\neg ((p \land q) \to r) \equiv \neg (\neg (p \land q) \lor r) \equiv \neg \neg (p \land q) \land \neg r \equiv p \land q \land \neg r$

{{% /example %}}

{{% example name="" %}}

Quantifiers
$\exists, \forall $



$(\forall x \in \R)  [ x > 0, \lor x = 0 \lor x < 0 ]$

$(\exists x \in \R)  [ y^2 = 2 ]$

$(\forall x, y \in \R)[ x \neq y \to (x < y \lor y < x) ]$

{{% /example %}}

What is quite tricky is alternating quantifiers

{{% example name="" %}}

$(\forall x \in \R) (\exists y \in \R)(x < y) $

{{% /example %}}


{{% example name="" %}}

$T $ or $F $ ? In real domain

1. $(\forall x)(\exists y)[ y^2 = x ] $  False, $-1$ is not a square
2. $(\forall x)(\exists y) [ x^2 = y ]$   True
3. $(\exists y)(\forall x)[ x < y ]$  False, $\exists y = 2,$ let $x = 3 $.
4. $(\forall x)(\exists y)[ y^3 = x ]$ True

{{% /example %}}

Think of quantifiers as "moves" in a game. To prove a statement like $(\forall x) (\exists y) [x^2 = y]$

{{% note name="" %}}

You are the "$\exists $" player
your opponent is the "$\forall $" player

{{% /note %}}


| players     | moves   |
| ----------- | ------- |
| $\forall$   | 7       |
| $\exists$   | 49      |


No matter what opponent plays, we plays a move so that the statement is true.

| players     | moves   |
| ----------- | ------- |
| $\forall$   | -1      |
| $\exists$   | none    |

{{% example name="" %}}

$(\exists x)(\forall y) [ x \leq y^2 ] $

| players     | moves   |
| ----------- | ------- |
| $\exists$   | 0       |
| $\forall$   | y       |


Define x = -42

We claim that for any $y \in \R $.

$-42 \leq y^2. $ so to see this.

fix an arbitrary $y $.

Well by earlier results. We know that $0 \leq y^2 $.

so -42 \leq

{{% /example %}}

To negate quantifiers... $\neg \forall \equiv \exists \neg $ $\neg \exists \equiv \forall \neg $.

{{% example name="" %}}

$\forall x, [ x > 0 ]$

False. It's neg

$\neg \forall x [ x > 0 ] \equiv \exists x \neg [ x > 0 ] \equiv x [ x \leq 0 ]$

{{% /example %}}

{{% example name="" %}}

Write the following precisely, and write its negation.

$ f: X \to Y $ injective if

"Whenever, $ x\_1, x\_2 \in X $, and $ f(x\_1) = f(x\_2), then x\_1 = x\_2 $"

$\forall x\_1, x\_2 \in X, f(x\_1) = f(x\_2) $, then $ x\_1 = x\_2 $

negation

$\exists x\_1, x\_2 \in X, f(x\_1) = f(x\_2) $ s.t. $ x\_1 \neq x\_2 $

{{% /example %}}

