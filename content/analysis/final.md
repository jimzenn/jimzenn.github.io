---
title: "Final"
date: 2019-02-22T16:14:00+08:00
volumes: ["15"]
layout: "note"
type: "notes"
issue: 2
weight: 1000

---

<!--more-->
## 1

Let $x\_0 \in \overline{ E }, y\_0 = f(x\_0)$.

Since $x\_0 \in E, \exists (x^{(n)})^\infty\_{ n =1}, x\_n \to x\_0$.

Since $f$ is continuous, $x\_n \to x\_0 $ implies that $f(x\_n) = f(x\_0) $.

Since $f(x\_n) \in f(E), \forall n, f(x\_0) \in \overline{ f(E)} $

{{% definition name="inner product space" status="" %}}

vector space with function $<, >: V \times V \to \C $

such that 

$\inner{ v }{ w } = \overline{ \inner{ w }{ v }} $

$\inner{ v }{ v } \geq 0, \forall v \in V $

$\inner{ v }{ v } = 0 \iff v = 0$

$\inner{ cv + w }{ z } = c \inner{ v }{ z } + \inner{ w }{ z } $

{{% /definition %}}

{{% example name="" %}}

$C(\R / \Z , \C) = V $

vectors are functions

$\inner{ f }{ g } = \int\_{ 0 }^{ 1 } f(x) \overline{ g(x)} \d x $

$\inner{ g }{ f } = \int\_{ 0 }^{ 1 } g(x) \overline{ f(x)} \d x = \overline{ \int\_{ 0 }^{ 1 } g(x) \overline{ f(x)} \d x } $

From those props, we have

1. (Cauchy-Scharz inequality) $\abs{ \inner{ f }{ g }} \leq \sqrt[  ]{ \inner{ f }{ f }} \sqrt[  ]{ \inner{ g }{ g }}$
2. For any inner vector space we define $2- $norm by

$$\norm{ v }\_2 = \sqrt[  ]{ v, v } $$

Using Cauchy Schwaz,

$$\norm{ v+w }\_2 \leq \norm{ v }\_2 + \norm{ w }\_2 $$

from other props, $\norm{ v }\_2 \geq 0, \forall v \in V$

$$\norm{ v }\_2 = 0 \implies v = 0\_v $$

$$\norm{ aV }\_2 = \abs{ a } \norm{ v }\_2 $$

$$\norm{ av }\_2 = \sqrt[  ]{ \inner{ av }{ av }} $$

$$\norm{ av }^2\_2 = \inner{ av }{ av } = \br a \inner{ v }{ av } = a \overline{ \inner{ av }{ v }} = a \overline{ a } \overline{ \inner{ v }{ v }} = \abs{ a }^2  \norm{ v }\_2$$

{{% /example %}}

{{% theorem name="Cauchy-Schwarz" index="" status="" %}}

$\abs{ \inner{ f }{ g }} \leq \norm{ f }\_2 \norm{ g }\_2$

$\inner{ v }{ v } \geq 0, v = f - tg, t \in \R$

$$\inner{ f-tg }{ f-tg } \geq 0 $$

$$\inner{ f }{ f-tg } - t \inner{ g }{ f-tg } $$

$$\inner{ f }{ f } - t \inner{ f }{ g } - t \inner{ g }{ f } + t^2 \inner{ g }{ g } $$

{{% /theorem %}}

minimum occurs when

$t = \frac{ -b }{ 2a }, a = \norm{ g }\_2^2 $

$b = - (\inner{ f }{ g } +? \inner{ g }{ f }) $

$b = -2 (\Re{(f, g)}) $



$$\norm{ f + g }\_2 = \norm{ f }\_2 + \norm{ g }\_2 $$


$$\begin{align}
\norm{ f+g }^2\_2 &= \inner{ f }{ f } + \inner{ f }{ g } + \inner{ g }{ f } + \inner{ g }{ g } \br
&= \inner{ f }{ f } + 2 \Re{ \inner{ f }{ g }} + \inner{ g }{ g } \br
\leq \inner{ f }{ f } + 2 \abs{ \inner{ f }{ g }} + \inner{ g }{ g } \br
\leq \inner{ f }{ f } + 2 \norm{ f }\_2 \norm{ g }\_2 + \inner{ g }{ g } \br
= (\norm{ f }\_2 + \norm{ g }\_2)^2
\end{align}$$

know the definition of 

$\inner{ f }{ g } V = C(\R / \Z , \C) $

Know how to compute 

$$\inner{ e\_n }{ e\_m } = \begin{cases}
\int\_{ 0 }^{ 1 } \exp 2 \pi i (n - m)x\d x = \frac{ \exp (2 \pi i (n - m))}{ 2 \pi i (n - m)} \big |^1\_0  = \frac{ e\_n(1)^2 - e\_k(0)}{ 2 \pi i (n - m)}\br
\int\_{ 0 }^{ 1 } 1 \d x
\end{cases} $$

$e\_n (0) = e\_n (1) $ by periodicity

$\inner{ f }{ g } = 0 $

$$f+g ^2\_2 = \norm{ f }^2\_2 + \norm{ g }^2\_2$$

Find function sequence such that

$f^{(n)}$ continuous, $f$ continuous.

1. $f^{(n)} \to f$, $L^2 $ but not uniformly
2. $f^{(n)} \to f $ L^2$ but not pointwise
3. pointwise but not $L^2 $

Idea:

$L^2 $ convergence measures area between functions
uniform convergence measures max height diff

if $f $ is analytic find $c\_n $

## 2

{{% example name="" %}}

$X$ connected.
show $\forall, a, b,d(a, b) > 0,  r \in [ 0, d(a, b) ], \exists x\_r, d(a, x\_r) = r $

{{% proof index="" method="" %}}

Choose $U = \set{y \in X : d(a, y) < r} = B(a, r)$ open set $U \neq \emptyset$.

Choose $V = \set{y \in X : d(a, y) > r} \neq \emptyset, V$ contains $b$.

Either $V \cup U = X$ or $V \cup U \neq X $.

$U, V$ open disjoint non-empty, contradicts that $X$ is connected.

Thus $\exists x\_r \not \in U, x\_r \not \in V$.

$d(a, x\_r) \geq r$ and $d(a, x\_r) \leq r$.

Then $d(a, x\_r) = r$

{{% /proof %}}

$s(a, r) = u $ open set $u \neq \emptyset $

$V = \set{ y \in X: d(a, y) > r } \neq \emptyset $

New question: Can you show $B(a,r) $ is open?

{{% proof index="" method="" %}}

Pick $y \in B(a, r), S = d(a, y) $

$r\_0 = r - S $

$B(y, r\_0) \leq B(a, r) $

$z \in B(y, r\_0) $

$d(z, a) < r $

(This shows $z \in B(a, r)$)

$d(z, a) \leq d(z, y) + d(a, y) < s + r\_0 = r $

{{% /proof %}}

{{% /example %}}

## 12

$f: X \to X, k \in [0, 1)$

$$d(f(x), f(y)) \leq k d (x, y) $$

points get "closer"

Show $\exists$ unique point $x\_0 $ such that $f(x\_0) = x\_0$

Two points such that $f(a) = a & f(b) = b$

$d(f(a), f(b)) \leq kd(a, b)$

$d(a, b) \leq k d(a, b)$

$d(a, b) = c$

Pick $x\_0 \in X$

$x\_n = f(x\_{n - 1})$

$d(x\_0, x\_1) = d$

$d(x\_1, x\_2) = d(f(x\_0), f(x\_1))  \leq k d(x\_0, d\_1) = k d$

$d(x\_2, x\_3) = d(f(x\_1, f(x\_2))) \leq k d(x\_1, x\_2) \leq k^2 d$

$d(x\_n, x\_3) = k^n d $

Maybe this is Cauchy $n < m $

$d(x\_n, x\_m)$

$d(x\_n, x\_m) \leq k^n d$

$d(x\_n, x\_{n+2}) \leq d(x\_n, x\_{n+1}) + d(x\_{n+1}, x\_{n+2})$

$$\leq k^n d + k^{n +1} d $$

$$d(x\_n, x\_{n+3}) \leq k^n d + k^{n+1} d + k^{n+2} d $$

$$d(x\_n, x\_m) \leq k^n d + k^{n+1}d + ... + k^{m - n - 1}d $$

$$\leq d (\sum\_{ j = n }^{ \infty } k^j) $$

$\exists N$ such that if $n > N $

$\sum\_{ j=n }^{ \infty }k^j < \epsilon / d $

$d(x\_n, x\_m) < \epsilon $ if $m> n> N$

$x\_n $ is Cauchy, so it converges to a point called $x^\* $

$f(x^\*) = f(\limu{ n }{ \infty } x\_n) \br $

$= \limu{ n }{ \infty } f(x\_n) $\br

$= \limu{ n }{ \infty } x\_{n+1} = x^\* $

## 5

$C\_c(\R^ -) =$ function such that $f : \R \to \R $

if $f(x) \neq 0 x \in$ compact set

given $f, \exists M $ such that if

$\abs{ x } \geq M, f(x) = 0 $

$C\_0$

bell curve $e^{- \frac{1}{x^2}}$

$C\_b(x) $

bounded continuous functions

If $f \in C\_c(\R) $ f \in c\_0(\R)

$g \in C\_0 (\R) show $ show g is bounded.

$\limu{ x}{ \infty } g(x) = 0$ implies

$\exists M\_1 $ such that $\abs{ g(x)} \leq 1 $ if $x > M\_1 $

$\exists M\_2 $ such that $\abs{ g(x)} \leq 1 $ if $x < M\_2 $

$g([M\_2, M\_1]) is compact $

$\abs{ g(x)} \leq M\_3 $ on $M\_2, M\_1 $

$\abs{ g(x)} \leq \max{ \set{ M\_3, 1 }} $

$g $ is bounded

$C\_c(\R) \leq C\_0(\R) \leq C\_b (\R) $

let $g(x) = e^{ - \frac{ 1 }{ x^2 }} \in C\_0$ 

$h(x) = 2$



