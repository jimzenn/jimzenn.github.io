---
title: "Disucission"
date: 2018-07-31T10:03:48+08:00
volumes: ["D"]
layout: "note"
issue: 6
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
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{| #1 |}$
    $\newcommand{\pare}[1]{\left\(#1\right\)}$
    $\newcommand{\t}[1]{\text{ #1 }}$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
    $\newcommand{\d}{\text d}$
    $\newcommand{\inv}[1]{{#1}^{-1}}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\rank}[1]{\text{rank }#1}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$


    $\newcommand{\Vcw}[2]{\begin{bmatrix} #1 \br #2 \end{bmatrix}}$
    $\newcommand{\Vce}[3]{\begin{bmatrix} #1 \br #2 \br #3 \end{bmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \end{bmatrix}}$
    $\newcommand{\Vct}[5]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{bmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{bmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{bmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{bmatrix}}$

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

Let $X, Y $ be independent are continuous random variables. Both $X, Y $ are uniform on [0, 1]. Find the probability of each of the following events. <br>
1. $X > \frac{ 3 }{ 5 } $ <br>
2. $Y < X $ <br>
3. $X + Y \leq \frac{ 3 }{ 10 } $ <br>
4. $\max(\set{ X, Y }) \geq \frac{ 1 }{ 3 } $ <br>
5. $XY \leq \frac{ 1 }{ 4 } $

{{% /example %}}

{{% example name="" %}}

Let $X $ be uniform $[0, 1] $, $Y $ be exponential(2). $X, Y $ are independent. <br>
1. Find $\b{P}(Y \geq X)$ <br>
2. Let $Z = X+Y $, find the conditional density of $Z $ given $Y = y $.

1\. $\b{P}(Y \geq X) = \int\_{ 0 }^{ 1 } \int\_{ x }^{ \infty } f\_{X,Y}(x,y) \d y \d x $

$\because X, Y $ are independent

$=\int\_{ 0 }^{ 1 } \int\_{ x }^{ \infty } f\_X(x) f\_Y(y) \d y \d x $

$= \int\_{ 0 }^{ 1 } \int\_{ x }^{ \infty } 1 \cdot 2 e^{-2y} \d y \d x $

$= \int\_{ 0 }^{ 1 } e ^{ -2x  \d x} $

$= - \frac{ 1 }{ 2 } e^{-2} + \frac{ 1 }{ 2 } $


2\. Let $Z = X+Y $, find the conditional density of $Z $ given $Y = y $.

Notice that given $Y=y $, Z = X + y.

Fact: If $W $ is uniform $[a, b] $ and $c \in R $, $W + C $ is uniform $[a + c, b + c] $.

So, by the fact, conditioned on $Y = y $, $Z = X+y $ is uniform [y, y + 1] is uniform [y, y + 1]

$f\_{Z|Y}(z | y) = \begin{cases}
1, \if 0 \leq y \leq \leq z \leq y+1
0, \otherwise
\end{cases}$

{{% /example %}}

{{% example name="" %}}

A professor schedules two student appointments for the same time. The appointment duration are independent random variables, each is exponentially distributed with mean of 30 mins. The first student shows u on time, the second is 5 mins late. What is the expected value of the time between the arrival of the first student and the departure of the second.

Let $T\_1 = \text{duration of first student appointment} $, $T\_2 = \text{duration of the second student's appointment} $.

$T\_1, T\_2$ independent.


Both $T\_1, T\_2 $ are exponential $\frac{ 1 }{ 30 } $.

$W $ is the time between first student's arrival and departure of second student.

If $T\_1 \geq 5 $, then $W = T\_1 + T\_2 $.

If $T\_1 < 5 $, then $W = 5 + T\_2  $.

Let $p = \b{P}(T\_1 < 5) $

$\begin{align\*}
E[W] &= E[W | T\_1 \geq 5] \(1 - p\) + E[W| T\_1 < 5] p \br
&= E[T\_1 + T\_2 | T\_1 \geq 5]\(1 - p\) + E[5 + T\_2 | T\_1 < 5] p \br
&= (E[T\_1 | T\_1 \geq 5] + E[T\_2|T\_1 \geq 5])(1-p) + E[5+ T\_2] p
\end{align\*}$

So, we need $p = \b{P}(T\_1 < 5), E[ T\_1 | T\_1 \geq 5 ] $

$p= \int\_{ 0 }^{ 5 } \frac{ 1 }{ 30 }e ^ { -\frac{ x }{ 30 }} \d x = 1 - e^{- \frac{ 5 }{ 30 }}$

$A = \set{ T\_1 \geq 5 }$

$ f\_{T\_1 | A}(t) =
\begin{cases}
  \frac{ f\_{T\_1}(t)}{ \b{P}(A)}, t \in A \br
  0,  \otherwise
\end{cases}$

$\begin{align\*}
E [T\_1 | T\_1 \geq 5] &= \int\_{ -\infty }^{ \infty } t \cdot f\_{T\_1 \mid A} (t) \d t \br
&= \int\_{ 5 }^{ \infty } \frac{ t \cdot \frac{ 1 }{ 30 }e^{- \frac{ t }{30}}}{ \b{P}(A)} \d t \br
&= \frac{ 1 }{ \b{P}(A)} \int\_{ 5 }^{ \infty }  \frac{ t e^{- \frac{ t }{ 30 }}}{ 30 } \d t \br
\end{align\*}$


{{% /example %}}

{{% example name="" %}}

Consider two continuous random variables $Y, Z$. Let $X $ be continuous random variable which is equal to $Y $ with probability $p $, and equal to $Z $ with probability $1-p $, as determined by and independent toss of a P-weighted coin.
<br>Find the PDF of $X $ in terms of the PDFs of $Y $ and $Z$, as determined by an independent toss of a $p $ -weighted coin.

For $x$,

$\begin{align\*}
F\_X(x) &= \b{P}(X \leq x) \br
&= \b{P}(X \leq x \mid X = Y)P (X = Y) + \b{P}(X \leq x \mid X = Z) \b{P}(X = Z) \br
&= \b{P}(Y \leq x)P (X = Y) + \b{P}(Z \leq x) \b{P}(X = Z) \br
&= F\_y(x) \cdot p + F\_Z(x) \cdot (1-p)
\end{align\*}$

$f\_X(x) = p(f\_Y)(x) + (1 - p)f\_Z(x)$

{{% /example %}}

{{% example name="" %}}

Calculate the CDF of the two-sided exponential random variable $X $ with $f\_X(x) = \begin{cases}
p \lambda e^{- \lambda x}, \if x < 0 \br
(1 - p) \lambda e^{- \lambda x}, \if x \geq 0
\end{cases}$

$x < 0,$

$\begin{align\*}
F\_X(x) &= \b{P}(X \leq x)  \br
&= \int\_{ -\infty }^{ x } p \lambda e^ { \lambda t } \d t \br
&=pe^{ \lambda t } \Big | ^x\_ { -\infty }
\end{align\*}$

$x \geq 0 $

$\begin{align\*}
P\_X(x) &= \b{P}(X \leq x) \br
&= \int\_{ -\infty }^{ 0 } p \lambda e^ { \lambda t } \d t + \int\_{ 0 }^{ x } (1-p) \lambda e^{ - \lambda t } \d t \br
&= pe^{ \lambda t } \Big |^ 0\_ { -\infty } + [ - (1 - p) e^{ - \lambda t } ]^x\_0
&= 1 - (1 - p)e^{ - \lambda x }
\end{align\*}$

{{% /example %}}

{{% example name="" %}}

$X $ is a random variable with PDF $f\_X(x) = \begin{cases}
\frac{ x }{ 4 }, \if 1 < x \leq 3 \br
0, \otherwise
\end{cases}$

$A = {x \geq 2} $

find $E[X], \b{P}(A, f\_{X|A}(x)), E[X|A] $

$\begin{align\*}
 E[X] &= \int\_{ 1 }^{ 3 } x \frac{ x }{ 4 } \d x \br
&= \int\_{ 1 }^{ 3 } \frac{ x^2 }{ 4 } \d x
&= \frac{ 26 }{ 12 }
\end{align\*}$

$\b{P}(A) = \b{P}(X \geq 2) = \int\_{ 2 }^{ 3 } \frac{ x }{ 4 } \d x = \frac{ 5 }{ 8 } $

$\begin{align\*}
f\_{X \mid A}(x) &= \begin{cases}
  \frac{ f\_X(x)}{ \b{P}(A)}, \if x \in A \br
  0, \otherwise
\end{cases}
&= \begin{cases}
\frac{ 2x }{ 5 }, \if 2 \leq x \leq 3 \br
0 , \otherwise
\end{cases}
\end{align\*}$

$E[X|A] = \int\_{ 2 }^{ 3 } x \cdot \frac{ 2x }{ 5 } \d x = \frac{ 2x^3 }{ 15 } \Big | ^3\_2 = \frac{ 2 \cdot 27 - 2 \cdot 8}{ 15 } $

{{% /example %}}

{{% example name="bi-variant" %}}

$f\_{XY}(x, y) = \frac{1}{\sqrt{2\pi(1-\rho^2)}}e^{-\frac{x^2 - 2\rho xy + y^2}{2{(1-\rho)}^2}}$
What is the marginal density of $Y $?

$f\_{Y}(y) = \int\_{ -\infty }^{ +\infty } \frac{1}{\sqrt{2\pi(1-\rho^2)}}e^{-\frac{(x-\rho y)^2 - \rho^2y^2 + y^2}{2{(1-\rho)}^2}} \d x$

{{% /example %}}

