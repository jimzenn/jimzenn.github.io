---
title: "Discussion"
date: 2018-08-21T11:03:48+08:00
volumes: ["D"]
layout: "note"
type: "notes"
issue: 3
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

Prove that if $(a\_n)$ is a Cauchy sequence s.t. $a\_n \in N$ for all $n $, then after some N, $a\_n$ is a constant.

{{% /example %}}

{{% example name="" %}}

Write down a sequence with

- exactly 2 subsequences limits : 1, 0, 1, 0, ...
- exactly n subsequences limits : 1, 2, 3, ..., n, 1, 2, 3, ..., n, 1, 2, 3, ..., n, ...
- exactly n subsequences limits : 1, 1, 2, 1, 2, 3, 1, 2, 3, 4, ...

{{% proof index="3" method="" %}}

suppose $\alpha \in S $.

let $(a\_{n\_k})$ be a subsequence that converges to $\alpha $ Then $(a\_{n\_1}) $ is a convergent, hence Cauchy sequence of elements, hence Cauchy sequence of elements of $\N $.

so $\alpha$ must be this eventual value. so in particular, $\alpha $ must equal some $a\_{n\_k} $ but $a\_{n\_k} \in \N $, so $\alpha \in \N $, but $a\_{n\_k} \in \N $ so $\alpha \in \N $.

{{% /proof %}}




{{% /example %}}


{{% example name="" %}}

Does there exist a set $(a\_n) $ s.t. the set of subsequence limit of $(a\_n) $ is <u>exactly</u> $(0, 1) $.

No, there does not. Since there must be a case where $0 $ is the limit, but $0 $ is not in the set.

{{% /example %}}

{{% example name="" %}}

Let S be a bounded nonempty subset of $\R$ such that $\supr{ S } $ is not in $S$. Prove there is a sequence $(s\_n)$ of points in $S$ such that $lim s\_n = \supr{ S } $.

{{% proof index="" method="" %}}

We will define the sequence $(s\_n)$ as a fallout.

Fix an $n $ then $\beta - \frac{ 1 }{ n } < \beta $, so $\beta - \frac{ 1 }{ n } $ is not a lower bound.

Consequently there is an element $a\_n \in S $ s.t. $\beta < a\_n $.

That $a\_n < \beta $ so $\beta - \frac{ 1 }{ n } < 0 \leq \beta $

Then observe that $(a\_n) \to \beta $

Consider squeeze $(a\_n)$

$b\_n = \beta \frac{ 1 }{ n }$

and $c\_n = \beta $\forall n

and $b\_n \to \beta, c\_n \to \beta$ also $a\_n \to \beta $.

{{% /proof %}}

{{% /example %}}

{{% note name="" %}}

Let $(q\_n) $ be an enumeration of $\Q cap (0, 1) $(or $(a, b)$).

Then the set of subsequential limit $(q\_n) = [0, 1] $.

Claim (A) suppose $t\_n \in [0, 1] \forall n$, and $t\_n \to t$ then $t \in [0, 1]$.

From claim (A) we can show $SSLs \leq [0, 1]$

fix y \in SSL, let $(q\_{n\_k}) $ be a SS converging to $y$.

$q\_{n\_k} \in (0, 1) \leq [0, 1] \forall k$ so since $(q\_{n\_k}) \to y$,

$y $ also is in $[0, 1] $.

Claim (B) If $a < b $, then there are infinitely many rational.


{{% proof index="" method="" %}}

We define by recursion an increasing set $\pare{r\_n} $ of  $\Q(a, b) $.

Base case $n= 1 $. By density of $\Q $, $\exists r \in Q, a < r < b$ let $r\_1 $ be such be such

Recursive step $s\_p $ defined $r\_1, ..., r\_n $ and $a< r\_1 <r\_2 < ... < r\_n < b$

By density of $\Q $, choose $r\_{n + 1} s.t. r\_n < r\_{n + 1} < b$


This completes the definine $n $ since $(r\_n) $ is increasing, \set{ r\_n: n \in \N } is infinite, all rational, and $\subseteq (a, b) $

we can now prove that every element of $ [0, 1] $ is a SSL of $(q\_n) $

Fix $ 0 \leq \alpha \leq 1 $ suppose for simlicity that $ 0 < alpha < 1 $ we define the indice $n\_1 < n\_2 < n\_3$

(i.e. the subseq $(q\_{n\_1}, q{n\_2}, ..., $))

$\forall K$

{{% /proof %}}


{{% /note %}}
