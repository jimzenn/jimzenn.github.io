---
title: "Review"
date: 2018-08-01T10:34:48+08:00
volumes: ["D"]
layout: "note"
type: "notes"
issue: 7
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
    $\newcommand{\B}{\mathcal{B}}$
    $\newcommand{\U}{\mathcal{U}}$
    $\newcommand{\N}{\mathcal{N}}$
    $\newcommand{\spa}[1]{\text{span}(#1)}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
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
    $\newcommand{\rank}[1]{\text{rank }#1}$
    $\newcommand{\tr}[1]{\text{tr}(#1)}$
    $\newcommand{\var}[1]{\text{var}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$
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

|                                         | Discrete                                        | Continuous                                             |
| -------------                           | ----------------------------------------------- | ------------                                           |
| Probability                             | PMF                                             | PDF                                                    |
| Cummulative                             | $\b{P}(X \leq x) =  \sum\_{ i = \min(X)}^{ X } P\_X(i)$                                                | CDF\: $F\_X(x) = \int\_{ -\infty }^{ x } f(t) \d t  $|
| Conditional Probability <br>$\b{P}(A\| B)$  | $\frac{ \b{P}(A \cap B)}{ \b{P}(B)}$                    | $\int\_{ E } f\_{X \| A}(x) \d x$                      |
| Joint Probability<br> $P\_{X,Y}(x, y) $ | $P\_{X,Y}(x, y) $                               | $\int\_{ y\_1 }^{ y\_2 } \int\_{ x\_1 }^{ x\_2 } f\_{X, Y}(x, y) \d x \d y $ |
| Marginal Probability<br> $P\_X(x) $     | $\sum\_{ y } P\_{X, Y}(x,y) $                   | $\int\_{ -\infty }^{ +\infty } f\_{X, Y}(x, y) \d y $  |
| Independence| $P\_{X, Y} = P\_X(x)P\_Y(y)$| $f\_{X, Y} (x ,y) = f\_X(x)f\_Y(y)$  |
| Covariance | $\text{cov}(X, Y)$ <br> $ = E[(X - E[X])(Y - E[Y])] $ <br> $=\text{cov}(E[XY] - E[X]E[Y]) $ | $\text{cov}(X, Y) = E[(X - E[X])(Y - E[Y])] $ <br> $=\text{cov}(E[XY] - E[X]E[Y]) $|
| Conditional on set of $X$ | $P\_{X}(x \| A) = \frac{ \b{P}(X \cap A)}{ \b{P}(A)} $ | $f\_{X \in A}(x) = \begin{cases} \frac{ f(X \in A)}{f(A)} & x \in A \br 0 & \otherwise \end{cases} $ |
| Conditional on another R.V. | $P\_{X\|Y}(x \| y) = \frac{ \b{P}(X = x, Y = y)}{ \b{P}(Y = y)} $ | $f\_{X\|Y}(x \| y) = \frac{ f(X = x, Y = y)}{ f(Y = y)} $|
| Total Probability Theorem (TPT) | $\b{P}(B) = \sum\_{ i= 0 }^{ n } \b{P}(B\|A\_i) $ | $f\_X(x) = \int\_{ -\infty }^ { +\infty } f\_{X\|y}(x) f\_Y(y) \d y$ |
| Total Expectation Theorem (TET) | $E[X] = \sum\_{ y } E[X \| Y = y]P\_Y(y) $ | $E[X] = \int\_{ -\infty }^{ +\infty } E[X \| Y = y]f\_Y(y) \d y$ |
| Bayes' Law | $ \b{P}(X \| A) =  \frac{ \b{P}(A \| X) \b{P}(A)}{ \sum\_{ i = 1 }^{ n }\b{P}(A \| X) \b{P}(A\_i)} $ | $ P\_{X \| Y}(x \| y) = \frac{ f\_X(x) f\_{Y\|X}(y\|x)}{ \int\_{ -\infty }^{ +\infty } f\_{X}(t)f\_{Y\|X}(y \| t)\d t} $ |
| Uniform Dist. $\U(a, b)$ | $ P\_X(x) = \frac{ 1 }{ n } $ | $f\_X(x) = \begin{cases}\frac {1}{b-a} & {\text{for }}x\in [a,b] \br0 &  \otherwise\end{cases}$  $F\_X(x) = {\begin{cases}0&{\text{ for }}x<a\br{\frac {x-a}{b-a}}&{\text{ for }}x\in [a,b)\br 1&{\text{ for }}x\geq b\end{cases}}$ $ E[X] = \frac{ b - a }{ 2 }, \var{ X } = \frac{ 1 }{ 12 } (b -a)^2$|
| Bernoulli Dist. <br> $\text{Bernoulli}(p) $| $P\_X(k) \br = B(1, p) \br =  \begin{cases} 1 &\if k = 1 \br 0 &\if k = 0 \end{cases}$ |
| Geometric Dist. (discrete) <br> Exponential Dist. (continuous) <br> | $P\_X(k) = (1- p)^{k - 1 } p,$ <br>$k = 1, 2, ...$<br> $E[X] = \frac{ 1 }{ p }, \var {X} = \frac {1-p}{p^{2}}$  | $f\_X(x) = \begin{cases}\lambda e ^{- \lambda x} &\if x \geq 0 \br 0 &\otherwise\end{cases}$ $ F\_X(x) = \begin{cases} 1- e^{ - \lambda x } &\if x \geq 0 \br 0 &\otherwise\end{cases} $ <br> $E[X] = \frac{ 1 }{ \lambda }, \var{X} = \frac{ 1 }{ \lambda^2 } $ |
| Binom. Dist. <br>$\B(n, p) $ | $P\_X(k) = \binom{ n }{ k }p^k(1-p)^{n - k}$ |
| Gaussian Dist. <br> $\N(\mu, \sigma^2) $ | $B(n, p) \simeq \N(np, np(1-p))$ <br> \* [De Moivre–Laplace Theorem](https://www.wikiwand.com/en/De\_Moivre%E2%80%93Laplace\_theorem)  | $f\_X(x) = \frac{1}{\sqrt{2\pi}{ \sigma }}e^{-\frac{(x-{ \mu })^2}{2{ \sigma }^2}}$ |

