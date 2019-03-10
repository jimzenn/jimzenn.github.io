---
title: "Midterm Review"
date: 2019-02-22T16:14:00+08:00
volumes: ["15"]
layout: "note"
issue: 1
weight: 999

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
    $\newcommand{\ite}[1]{\text{int}(#1)}$
    $\newcommand{\ext}[1]{\text{ext}(#1)}$
    $\newcommand{\bdry}[1]{\partial #1}$
    $\newcommand{\argmax}[1]{\underset{#1}{\text{argmax }}}$
    $\newcommand{\argmin}[1]{\underset{#1}{\text{argmin }}}$
    $\newcommand{\set}[1]{\left\{#1\right\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\tilde}{\text{~}}$
    $\newcommand{\otherwise}{\text{ otherwise }}$
    $\newcommand{\if}{\text{ if }}$
    $\newcommand{\proj}{\text{proj}}$
    $\newcommand{\union}{\cup}$
    $\newcommand{\intercept}{\cap}$
    $\newcommand{\abs}[1]{\left| #1 \right|}$
    $\newcommand{\norm}[1]{\left\lVert#1\right\rVert}$
    $\newcommand{\pare}[1]{\left(#1\right)}$
    $\newcommand{\brac}[1]{\left[#1\right]}$
    $\newcommand{\t}[1]{\text{ #1 }}$
    $\newcommand{\head}{\text H}$
    $\newcommand{\tail}{\text T}$
    $\newcommand{\d}{\text d}$
    $\newcommand{\limu}[2]{\underset{#1 \to #2}\lim}$
    $\newcommand{\limd}[3]{\underset{#1 \to #2; #3}\lim}$
    $\newcommand{\der}[2]{\frac{\d #1}{\d #2}}$
    $\newcommand{\derw}[2]{\frac{\d #1^2}{\d^2 #2}}$
    $\newcommand{\pder}[2]{\frac{\partial #1}{\partial #2}}$
    $\newcommand{\pderw}[2]{\frac{\partial^2 #1}{\partial #2^2}}$
    $\newcommand{\pderws}[3]{\frac{\partial^2 #1}{\partial #2 \partial #3}}$
    $\newcommand{\inv}[1]{{#1}^{-1}}$
    $\newcommand{\inner}[2]{\langle #1, #2 \rangle}$
    $\newcommand{\nullity}[1]{\text{nullity}(#1)}$
    $\newcommand{\rank}[1]{\text{rank }#1}$
    $\newcommand{\nullspace}[1]{\mathcal{N}\pare{#1}}$
    $\newcommand{\range}[1]{\mathcal{R}\pare{#1}}$
    $\newcommand{\var}[1]{\text{var}\pare{#1}}$
    $\newcommand{\cov}[2]{\text{cov}(#1, #2)}$
    $\newcommand{\tr}[1]{\text{tr}(#1)}$
    $\newcommand{\oto}{\text{ one-to-one }}$
    $\newcommand{\ot}{\text{ onto }}$
    $\newcommand{\ceil}[1]{\lceil#1\rceil}$
    $\newcommand{\floor}[1]{\lfloor#1\rfloor}$
    $\newcommand{\Re}[1]{\text{Re}(#1)}$
    $\newcommand{\Im}[1]{\text{Im}(#1)}$
    $\newcommand{\dom}[1]{\text{dom}(#1)}$
    $\newcommand{\fnext}[1]{\overset{\sim}{#1}}$
    $\newcommand{\transpose}[1]{{#1}^{\text{T}}}$
    $\newcommand{\b}[1]{\boldsymbol{#1}}$
    $\newcommand{\None}[1]{}$
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

Important problems

# 3

(important!!)

Show $\Q \cup \bdry{\Q} = \R$

Show if $x \in \R$ $x$ is an adherent point of $\Q$.

i.e. there exists a sequence of rational $E$'s $(q^{(n)})^\infty\_{n=1}$ in $Q $.

$q^{(n)} \to X\_0 $ $d\_(q^{(n)}, x\_0) \to 0$

Consider

$(x\_0 - 1, x\_0 + 1) \subseteq \R, B(x\_0, 1) \subseteq \R$

$\exists$ rational here $q^{(1)}$

$(x\_0 - \frac{ 1 }{ n }, x\_0 + \frac{ 1 }{ n })$ has a rational $q^{(n)}$

$d(x\_0, q^{(n)}) < \frac{ 1 }{ n }$

$\limu{ n }{ \infty } d(x\_0, q^{(n)}) = 0 $

$q^{(n)} \to x\_0, x\_0 \in \overline{\Q}$

What to take away from it? What is a closure?

Remember

$E$ is closed iff $\overline{ E } = E $ iff $x^{(n)} \in E$ & $(x^{(n)})^{ \infty }\_{n=1} \to x\_0 \in X$ then $x\_0 \in E$.

# 7

(not in exam!)

Show $X = (a^{(n)})^\infty\_{ n =1}: a\_n \in \set{ 0, 1 }$

view each entry as vectors 

Take a Cauchy sequence in $X$.

$X^{(1)} = (X^{(2)}\_1, X^{(2)}\_2, ...)$

$X^{(1)} = (X^{(1)}\_1, X^{(2)}\_2, ...)$

lower index = entry of the vector
upper index = term of sequence

If $(x^{(n)})^\infty\_{ n =1} $ is cauchy

$\exists N $ such that if $n, m > N $

then $d(x^{(n), x^{(m)}}) < 2 $ then $x\_0 = y\_0 $

$\sum\_{ j=0 }^{ \infty } \frac{ 1 }{ 2^j } \abs{ x\_j - y\_j } < 2$

$\frac{ 1 }{ 2^0 } \abs{ x\_0 - y\_0 }  + \sum\_{ j=0 }^{ \infty } \abs{ x\_0 - y\_0 } < 1$

contradiction because:

if $x\_0 \neq y\_0 $, $d(x, y) \geq 1 $

If n > N

The zeroth entry

$x\_0^{(n)} = x\_0^{(N+1)} $

0th entry of a possible by $(x\_0^{n+1})$

# 8

$K\_1 \subseteq K\_2 \subseteq K\_3 $ compact sets

$\bigcap\_{ n=1 }^ \infty \neq \emptyset$.

We will work in the space $X = K$, ($X$ is compact).jo

$K\_n $ compact $\implies$ closed

Notice $X \setminus K\_n = O\_n$ is open in $X$.

Assume

$\cap K\_n = \emptyset $

Take complement

$\bigcup\_{ n=1 }^ \infty (X \setminus K\_n) = X$

$\bigcup\_{ n=1 } ^ \infty O\_n = X$ Compact

We can find 

$O\_1, \_2, ..., \_n\_k $ such that

$O\_{n\_1} \cup O\_{n\_2} \cup ... \cup O\_{n\_k} \subseteq X$

Notice $X \setminus K\_n = O\_n $ is open in $X\_0$.

$m = \max{ n\_1, n\_2, ..., n\_\_k }$

$O\_m \subseteq X $

$K\_m = \emptyset$

If $K$ is compact then $K$ is closed.

If $K$ is compact then $K$ is complete.

If $K$ complete \implies $K$ is closed.

If $E \subseteq K $, $K  $ complete and $E $ closed, then $E $ is complete.

# 12

$f: S \to X $ injective. Show $d\_s(s\_1, s\_2) = d\_X(f(s\_1), f\_(s\_2)) $ is a metric.

step 0:

Show $0 \leq d\_s(s\_1, s\_2) < \infty $

$f(s\_1) \in x\_1, f(s\_2) \in x\_2 $.


$o \leq d\_X(x\_1, x\_2)  \leq \infty $

$o \leq d\_X(f(s\_1), f(s\_2))  \leq \infty $

$o \leq d\_s(s\_1, s\_2)  \leq \infty $

step 1:

$d\_s(s, s) = d\_X(f(s), f(s)) = 0$

step 2:

If $s\_1 \neq s\_2 $, show $d\_s(s\_1, s\_2) > 0$

step 3:

$d\_s(s\_1, s\_2) = d\_s(s\_2, s\_1)$


# 13

Show if $r\_n > 0 $ such that $r\_n \to 0 $ with the prop


$d(f(x), f^{(n)}(x)) < r^n $ then $f^{(n)} \to f $ uniformly.

$r\_n \to 0 $ if $\forall \epsilon > 0, \exists  $ such that $\abs{ r\_n -0 } < \epsilon$ if $n > N , r\_n < \epsilon$.

$d(f^{(n)}(x), f(x)) < r\_n < \epsilon, \forall x \in X$.

Suppose $f^{(n)} \to f $ uniformly, build $r\_n \to 0 $

if you want to build a sequence, try $\frac{ 1 }{n} $

# 14

(!! important)

Recall $d\_ \infty (r, g) = \supr\_{x \in X} d(f(x), g(x))$

Assume $\limu{ n }{ \infty } d\_ \infty(f^{(n)}, f) = 0 $

Let $\epsilon > 0 $, $\exists N $ such that if $n > N $

$\abs{ d\_ \infty(f^{(n)}, f) - 0 } < \epsilon $

$d\_i \infty(f^{(n)}, f) < \epsilon $

$\supr\_{x \in V}{ d(f^{(n)}(x), f(x)) < \epsilon} $

Thus,

$d(f^{(n)}(x), f(x)) < \epsilon, \forall x \in X $ 

Assume $f^{(n)} \to f $ uniformly show $\forall \epsilon > 0, \exists N$  such that if $n > N $

$d\_ \infty(f ^{(n)}, f)  < \epsilon$

Let $\epsilon > 0 $

$d(f^{(n)}(x), f(x)) < \epsilon $\forall x \in X$

$\supr\_{x \in V}{ d(f^{(n)}(n), f(x))} \leq \epsilon /2 < \epsilon $

# 15

!!! note If $x < S$, $\forall x \in E \subseteq \R$ $\supr{ E } \leq S$

if $d(f^{(n)}(x), f(x)) < \epsilon $

then $\supr{ d(f^{(n)}(x), f(x))} \leq \epsilon $

$f, g $ are bounded, show $0 \leq d\_ \infty(f, g) < \infty $

 Notice $0 \leq d(f(x), g(x)), \forall x \in X$, $0 \leq \supr{ x \in V } $

 $f $ is bounded, $\exists y\_1, r\_1 $

 $f(x) \subseteq B(y\_1, r\_1)$

 $g \to  g(x) \subseteq B(y\_2, r\_2)$

 $d(f(x), g(x)) \leq d(f(x), y\_1) + d(g(x), y\_2) + d(y\_1, y\_2) \leq r\_1 + r\_2 + (y\_1, y\_2) < \infty$

 $\supr\_{x \in X}{ d(f(x), g(x))} \leq r\_1 + r\_2 + d(y\_1, y\_2) < \infty  $

 step 1:

 $d(f, f) $

 $= \supr{ d(f(x), f(x))} $

 $= \supr 0 $

 $= 0 $

 !!!

 If $f \neq g $ then $\exists x\_0 \in X $ such that $f(x\_0) \neq g(x\_0) $

 $0 < d\_Y(f(x\_0), g(x\_0)) \leq \supr \_{x \in X}{ d(f(x), g(x))} $

# 16

By problem 14, we are done. 

# 17

$f^{(n)}(-1) = (-1^n) $ no convergence

If $x\_0 \in (-1, 1)  \limu{ n }{ \infty } x\_0^{(n)} = 0$

I partially define $f $ $f(x\_0) = 0 $

If $x\_0 = 1 $

$f^{(n)}(1) = 1^n = 1 $

$\limu{ n }{ \infty } 1 = 1 $

Define $f (1) = 1 $

$ f(x) = \begin{cases}
  0 & if x \in (-1, 1) \br
  1 & if x  = 1
\end{cases}$

Is a pointwise limit of $f^{(n)} $

But $f^{(n)} \to f$ uniformly

$f^{(n)} $ is cont, $f $ is not cont

# 21
!!!! important

Look at your notes online!

state a version of weistrass M-test

$f^{(n)}: X \to R $(complete) $\to f^{(n)} \in B(X, \R^5) $

$\abs{ f^{(n)}(x)} \leq M\_n $(bounded)

$\sum\_{ n=0 }^{ \infty  } M\_n < \infty $

$ f(x) + g(x) $

step 1

If $ g^{(n)} $ is Cauchy is  $B(X,Y)$ and $ Y $ is complete then $\exists g $ such that $ g^{(n)} \to g$ in $ d\_ \infty $ metric

$B(X, Y)$ is complete if $ Y $ is complete


{{% proof index="" method="" %}}

$g^{(n)} \in B(X, Y)$ be cauchy

$\forall \epsilon > 0, \exists N $ such that $ n, m > N \implies d\_ \infty(g^{(n)}, g^{(m)}) < \epsilon$

What might $ g(x\_0) = ? $ should be $\limu{ n }{ \infty  } g^{(n)}(x\_0) = g(x\_0) $

Does $ g^{(n)}(x\_0) $ converge?

points in $Y, Y is complete

show $ g^{(n)}(x\_0) $ is cauchy in $ Y $

$ d(g^{(n)}(x\_0), g^{(m)}(x\_0)) \leq d\_ \infty (g^{(n)}, g^{(m)}) < \epsilon$

Thus $ g^{(n)}(x\_0) is cauchy in $ Y $

Hence $ g^{(n)} (x\_0)$ converges $ y\_0 $

Define $ g(x\_0)  = y\_0 = \limu{  n }{ \infty } g^{(n)}(x\_0)$

Notice $ g^{(n)} \to g$ pairwise

Is this convergence uniform?

Let $\epsilon > 0 , \exists N $ such that if $ n, m > N $

$ d(g^{(n)}(x), g^{(m)}(x)) < \epsilon  \forall x \in X$ 

$\limu{ m  }{ 0 } d(g^{(n)}(x), g^{(m)}(x)) \leq \epsilon $

$ d(g^{(n)}(x), g(x)) \leq \epsilon $

$\supr{(g^{(n)}(x), g(x))} \leq \epsilon$

{{% /proof %}}

# 22

# 23

# 24

$\sum\_{ n=1 }^{ \infty } f^{(n)} $ converges uniformly

Need is an upper bound

on $f(n) = \frac{  }{ x^2 + y^2 + n^2 }, \frac{  }{ x^2 + y^2 + n^2 } $

$\norm{ f^{(n)}(x, y)} \leq \frac{ 1 }{ x^2 + y^2 + n^2 }, \frac{ 1 }{ x^2 + y^2 + n^2 } $

$\leq \abs{ \frac{ 1 }{ n^2 } + \frac{ 1 }{ n^2 }} $








Show $e^x = \sum\_{ n=0 }^{ \infty } \frac{ x^n }{ n! } $ converges uniformly on $[- R, R] $ pointwise convergence

To show $\sum\_{ n=0 }^{ \frac{ x^n }{ n! }}$ converges uniformly on $[- R, R] $.

$f^{(n)}(x) = \frac{ x^n }{ n! } $

$\abs{ f^{(n)}(x)} = \abs{ \frac{ x^n }{ n! }} \leq \frac{ R^n }{ n! } = \norm{ f }\_ \infty$


$\abs{ f^{(n)}(x)} \leq \frac{ R^n }{ n! } (= M\_n) $

$\sum\_{ n=0 }^{ \infty } M\_n < \infty$ M\_n real #? 

Ratio test

$\sum\_{ n=0 }^{ \infty } \frac{ R^n }{ n! } \to \limu{ n }{ \infty } \frac{ M\_n }{ m\_{n-1}} < 1$

$\frac{ M\_n }{ M\_{n-1}} = \frac{ R^n }{ n! } \frac{(n-1)! }{ R^{n-1}} = \frac{ R }{ n }$

$\limu{ n }{ \infty } \frac{ M\_n }{ M\_{n-1}} = 0 < 1$


Yes the series converges.

By the weierstrass M-test, $\sum\_{ n=0 }^{ \infty } \frac{ x^n }{ n! } $ converges uniformly on $[-R, R] $.


Ignore below -----------------

Pointwise convergence on $[- \infty, \infty] $.

$\sum\_{ n=0 }^{ \infty } \abs{ \frac{ c\_n }{ c\_{n-1}}} = L$

The radius of convergence is $ R = \begin{cases}
  0 &, if L = \infty \br
  \frac{ 1 }{ L } &, if 0 < L < \infty \br
  \infty &, if L = 0
\end{cases} $

Ignore above -----------------


