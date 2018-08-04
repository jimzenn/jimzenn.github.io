---
title: "Disucission"
date: 2018-07-24T10:03:48+08:00
volumes: ["D"]
layout: "note"
issue: 5


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
    $\newcommand{\rank}[1]{\text{rank}(#1)}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$


    $\newcommand{\Vcw}[2]{\begin{pmatrix} #1 \br #2 \end{pmatrix}}$
    $\newcommand{\Vce}[3]{\begin{pmatrix} #1 \br #2 \br #3 \end{pmatrix}}$
    $\newcommand{\Vcr}[4]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \end{pmatrix}}$
    $\newcommand{\Vct}[5]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \end{pmatrix}}$
    $\newcommand{\Vcy}[6]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \end{pmatrix}}$
    $\newcommand{\Vcu}[7]{\begin{pmatrix} #1 \br #2 \br #3 \br #4 \br #5 \br #6 \br #7 \end{pmatrix}}$

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

**Correction**:

Last problem ,about $n $ couples seated uniformly at random at a random table with $2n $ chairs. X = number of couples seated next t o each other.

$$E[X] = n \cdot (\frac{ 2 }{ 2n-1 }) $$

{{% example name="1" %}}

Joe plays the lottery on a given week with probability $p$ independently of other weeks. Each time he plays, he wins with probability $q$ again independent of everything else. During a particular period of $n$ weeks. <br>
Let $X$ = number of weeks he plays, $Y$ = number of weeks he wins.

**(a)** What is the probability that he played the lottery on a particular week, given that he didn't win that week. Let $A$ = he plays that week, $B$ = he wins that week.


$$\begin{align\*}
P(A \mid B^c) &= \frac{ P(B^c \mid A) P(A)}{ P(B^c \mid A)P(A) + P(B ^c \mid A^c)P(A^c)} \br
&= \frac{(1-q) p }{(1-q)p + 1(1-p)}
\end{align\*}$$

**(b)** Find the marginal PMF $P(Y=y \mid X = x)$ conditioned on $X = x, Y$ is Binomial $(x, q)$.

So, $P(Y = y \mid X = x) = \begin{cases}
\binom{ x }{ y } q^y (1-q)^{x-y} \if y \in \set{0, 1, ..., x} \text{ and } x \in \set{ 0,1, ..., n }\br
0 \otherwise
\end{cases}$

**(c\)** Find the joint PMF of $X,Y $.

$P(X = x, Y = y) = P(Y = y \mid X = x)P(X = x) = \begin{cases}
\binom{ x }{ y }q^y(1-q)^{x-y} \binom{ n }{ x }p^x (1-p^{n-x}), \if y \in \set{0, 1, ..., x} \text{ and } x \in \set{ 0,1, ..., n } \br
0, \otherwise
\end{cases}$

**(d)** What is the marginal PMF of $Y$?

$P(\text{win on a particular week}) = p \cdot q$.

$Y$ is Binomial$(n, pq)$.

**(e)** Find the conditional PMF $P(X = x | Y = y)$.

$P(X=x \mid Y = y) = \begin{cases}
\frac{ \binom{ n }{ x } \binom{ x }{ y } p^x(1-p)^{n - x} q^y (1-q)^{x-y}}{ \binom{ n }{ x }(pq^y)(1-pq)^y}, \if x \in \set{ 1, 2, ..., n } y \in \set{ 1, 2, ..., x }  \br
0, \otherwise
\end{cases}$

{{% /example %}}

{{% example name="supplementary 2, #13" %}}

$n$ students in a class,

$X = $ number of students who get As, <br>
$Y = $ number of students who get Bs.

$P(X = x, Y = y) = \begin{cases}
\binom{ n }{ x } \binom{ n-x }{ y } p^x q^y (1-p-q)^{n-x-y}, \if \begin{align\*}
0 \leq x \leq n \br
0 \leq y \leq n \br
x + y \leq n
\end{align\*}\br
0 \otherwise
\end{cases}$

<small>(\*) Always be careful with the domain.</small>

{{% /example %}}

{{% example name="2" %}}

Let $X, Y$ be continuous random variables which are jointly uniform on the region perimeterred by $((0, 0), (0, 1), (1, 2), (1, 1))$.

**(a)** find f(X=x \mid Y = y) the joint density.

$f(X= x \mid Y = y) = \begin{cases}
\frac{ 1 }{ area } = 1, \if 0 \leq x \leq 1 \text{ and } x \leq y \leq x + y \br
0, \otherwise
\end{cases}$

**(b)** Compute $f\_X, f\_Y $(marginally)

$f\_X(x) = \int\_{ -\infty }^{ +\infty } (x,y) \d y = \int\_{ x }^{ x+1 } 1 \d y = 1 $

$f\_X(x) = \begin{cases}
1, \if o \leq x \leq 1 \br
0, \otherwise
\end{cases}$

So, $X$ is uniform on $[0, 1]$.

<br>

$\begin{align\*}
f\_Y(y) &= \int\_{ -\infty }^{ +\infty } f(X=x \mid Y = y) \d x \br
&= \begin{cases}
\int\_{ 0 }^{ y } 1 \d x, \if 0 \leq y \leq 1 \br
\int\_{ y-1 }^{ 1 } 1 \d x, \if 1-y \leq y \leq 2 \br
\end{cases} \br
&= \begin{cases}
y, \if 0 \leq y \leq 1 \br
2-y, \if 1 < y \leq 2 \br
0, \otherwise
\end{cases}
\end{align\*}$

**(c\)** Compute: $E[Y], var(y), E[X], var(X)$.

$E[X] = \frac{ 1 }{ 2 }, var(X) = \frac{ 1 }{ 12 } $.

$E[Y] = \int\_{ -\infty }^{ +\infty } y f\_Y(y) \d y = \int\_{ 0 }^{ 1 } y \cdot y \d y + \int\_{ 1 }^{ 2 } y (2-y) \d y \br = [ \frac{ 1 }{ 3 } y^3 ]\_{ 0 }^{ 1 } + [ y^2 - \frac{ 1 }{ 3 } y^3 ]\_{ 1 }^{ 2 } = 1$

$var(y) = E[y^2] - E^2[y] $

**(d)** Compute PDF of $T = Y - X, T \in [0, 1]$
Let $t \in [0, 1]$.

$P(T \leq t) = P(Y - X \leq t) = \int\_{ 0 }^{ 1 } \int\_{ x }^{ x+t } f(X=x, Y = y) \d y \d x = \int\_{ 0 }^{ 1 } t \d x = t$

CDF:

$F\_T(t) = \begin{cases}
1, \if t > 1 \br
t, \if t 0 \leq t \leq 1 \br
o, \otherwise
\end{cases}$

$f\_T(t) = \begin{cases}
1, \if 0 \leq t \leq 1 \br
0, \otherwise
\end{cases}$

{{% /example %}}

{{% example name="" %}}

X standard normal:

$f\_X(x) = \frac{ 1 }{ \sqrt(2 \pi) e^{- \frac{ x^2 }{ 2 }}}$

$E[X] = 0 $

Compute variance of X.

$E[X] = 0, so, var(X) = E[X^2]$

$\begin{align\*}
E[X^2] &= \int\_{ -\infty }^{ +\infty } x^2 \frac{ 1 }{ \sqrt{2 \pi}} e^{- \frac{ x^2 }{ 2 }} \d x \br
&= \frac{ 1 }{ \sqrt{2 \pi}}\int\_{ -\infty }^{ +\infty } x^2  e^{- \frac{ x^2 }{ 2 }} \d x \br
&= \frac{ 1 }{ \sqrt{2 \pi}} ([ -x e^{- \frac{ x^2 }{ 2 }} ]\_{ -\infty }^{ +\infty } + \int\_{ -\infty }^{ +\infty } e^{- \frac{ x^2 }{ 2 }} \d x)
\end{align\*}$

{{% /example %}}

Exercise, Let $X\_1, X\_2, ..., X\_n$ be independent, continuous random variables. each $X\_i$ uniform $[0, 1]$. $Y\_n = \max \set{ X\_1, ..., X\_n } $.

**(a)** Compute PDF of $y\_n$.

**Step 1**. Compute CDF $F\_{y\_n}$ of $y\_n$.

**Step 2**. Takes derivative of $F\_{y\_n} $ to get $f\_{y\_n} $.

$y\_n \in [0, 1)$.

Let, $y \in [0, 1)$.

$F\_{Y\_n}(y) = P(Y\_n \leq y) = P(\max \set{ X\_1, X\_2, ..., X\_{ n } \leq y })$


**(b)** Compute $E[y\_n] $ and $\limu{n}{ \infty } E[y\_n] $

**(c\)** Compute $var(y\_n)$ and $\limu{n}{ \infty } var(y\_n)$.

{{% example name="" %}}

$1000$ items being produced, each item will be defective with probability $p = 0.05 $, independently of other items.

**(a)** Find the probability that at least $4$ items are defective.

$X = $  number of defective items

$X $ is $Binomial(1000, 0.05)$.

$$\begin{align\*}
P(X \leq 4) &= 1 - p(X \leq 4) \br
& = 1 - \sum\_{ i=0 }^{ 3 }P(x=i) \br
&= \sum\_{ i=0 }^{ 3 } \binom{ 1000 }{ i }(0.05)^i (0.95)^{1000-i}
\end{align\*}$$

**(b)** Repeat (a), but using a Poisson approximation.

Let $Y$ be $Poisson(1000, 0.5)$.

{{% remarks name="" %}}

$E[X] = E[Y] = np$

{{% /remarks %}}

So, $Y $ is Poisson with parameter $50$.

$\begin{align\*}
P(X \geq 4) \approx P(Y \geq 4) &= 1 - P(Y < 4) \br
&= 1 -  (P(Y=0) + p(Y= 1) + P(Y = 2) + P(Y = 3))
\end{align\*}$


{{% /example %}}
