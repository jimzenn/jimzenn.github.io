---
title: "Continuous Random Variables"
date: 2018-07-18T10:03:48+08:00
author: "Olga Turanova"
volumes: ["MATH 170A"]
layout: "note"
issue: 2.3

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
    $\newcommand{\B}{\beta}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{{#1}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{|#1|}$
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
    $\newcommand{\t#1}{\text}[1]$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$

    $\newcommand{\Vcw}[2]{\begin{pmatrix} #1 \br #2 \end{pmatrix}}$
    $\newcommand{\Vce}[3]{\begin{pmatrix} #1 \br #2 \br #3 \end{pmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \end{pmatrix}}$
    $\newcommand{\Vct}[5]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{pmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{pmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{pmatrix}}$

    $\newcommand{\Mqw}[2]{\begin{bmatrix}#1 & #2 \end{bmatrix}}$
    $\newcommand{\Mqe}[3]{\begin{bmatrix}#1 & #2 & #3 \end{bmatrix}}$
    $\newcommand{\Mqr}[4]{\begin{bmatrix}#1 & #2 & #3 & #4 \end{bmatrix}}$
    $\newcommand{\Mqt}[5]{\begin{bmatrix}#1 & #2 & #3 & #4 & #5 \end{bmatrix}}$

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

{{% definition name="" %}}
A is random variable, X is <u>continuous</u>. If there is a nonnegative function $f_X$, called the **probability density function** (PDF) of $X$ s.t.
$P(X \in B) = \int_B f_X(x)dx$where $B$is any subset of $\R$.

{{% /definition %}}

{{% example name="" %}}
uniform random variable, if $X $ takes values in $[a,b] $, and any subintervals of the same length are equally likely then $X$ is called uniform and has PDF.

$$
f_X(x) = \begin{cases}
\frac{1}{ b-a }, \if x \in [a,b] \br
0 \otherwise
\end{cases}$$

{{% /example %}}

{{% properties name="" %}}

Let $X $ be a continuous random variable.

1. $P(a \leq X \leq b) = \int_a^b f_X(x) dx$
2. $1 = P(- \infty < x < \infty) = \int_{-\infty}^\infty f_X(x) dx$

From $(1)$ we see, $\forall a \in R, $

$p(X=a) = \int_a^af_X(x)dx = 0$

{{% /properties %}}
