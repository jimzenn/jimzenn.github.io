---
title: "Discussion"
date: 2018-08-28T11:03:48+08:00
volumes: ["D"]
layout: "note"
type: "notes"
issue: 4
draft: true

---


<!--more-->
{{% example name="11.5" %}}

$SSL \subseteq [0, 1], \because [0, 1]$ is a closed set.

$[0, 1] \subseteq SSL $ Fix $t \in [0, 1]$ Apply Thm 11.2 part blah.

{{% /example %}}

Question

Alternating sequence: $\sum\ (-1)^n$

Recall ... if $\sum\ a\_n $ converges, then $\lim a\_n = 0 $

By contrapositive, since $\lim(-1)^n = 1 \neq 0$. $\sum\ (-1)^n$ converges.

Strategy for showing that a series $\sum\ a\_n $ converges, is to show that sums of tails are small. i.e. show $\forall \epsilon > 0 $, $\exists N \forall n \geq N, \abs{ a\_N + ... + a\_n } < \epsilon$.

Fact, suppose $\sum a\_n$ converges and $(b\_n)$ bounded sequence.
Show that $\sum a\_nb\_n$ converges.

bounded $\iff \abs{ b\_n } \leq M$.

Use the strategy:

Fix $\epsilon > 0 $, observe if $N \in \N $ and $n \geq N $ that $a\_N b\_N + ... + a\_nb\_N \leq \abs{ a\_N } \abs{ b\_N } + ... + \abs{ a\_n } \abs{ b\_n } \leq M(\abs{ a\_N } + ... + \abs{ a\_n })$

Since $\sum \abs{ a\_n }$ converges, fix $N$ s.t. $\forall n \geq N \sum\_{ i=N }^{ n } \abs{ a\_i } < \frac{ \epsilon }{ m } $.

By the inequality, then $\abs{ \sum\_{ i = N }^{ n } a\_i b\_i } \leq M (\frac{ \epsilon }{ M }) = \epsilon$

{{% example name="" %}}
Consider $\sum \frac{(-1)^n}{ n }$ converges, but not abs. since $\sum \frac{ 1 }{ n } $ Dic.

{{% /example %}}

{{% example name="" %}}

suppose $\lim\infi{ \abs{ a\_n }} = 0.$ Show there is a subseq. $a\_{n\_k} $ s.t. $\sum\_{ k=1 }^{ \infty } \abs{ a\_{n\_k}} $ converges.

{{% proof index="" method="" %}}

We construct recursively the sequence $a\_{n\_k}  s.t. \abs{ a\_{n\_k}} \leq \frac{ 1 }{ k^2 }$

Suppose we've constructed $a\_n ... a\_{n\_k} $ since $\lim \infi{ \abs{ a\_n }} = 0 $, we ??? that \set{ n \in \N \mid \abs{ a\_n } < \frac{ 1 }{(k+1)^2 }} = A is infinite..

$\therefore$

{{% /proof %}}

{{% /example %}}

{{% example name="" %}}

Suppose $\sum a\_n  $ converges then $\lim n a\_n = 0 $.

{{% proof index="" method="" %}}

Fix $\epsilon > 0 $. Find an $N $ s.t. if $n \geq N, \abs{ n a\_n } < \epsilon$.

$\abs{ n a\_n } = \abs{ a\_n + ... + a\_n }$ n times

we can make terms lite

$a\_N + ... +     a\_n $ small
so since decrease, \abs{ a\_n ... + a\_n } n -N + 1 terms small

$\leq \abs{ N a\_n } + \abs{(n - N + 1) a\_n }$.


First, fix $N\_0 $ s.t. $\forall n \geq N\_0 \abs{ a\_{N\_0} + ... + a\_n } < \frac{ \epsilon }{ 42 } $.

Choose next, $N \geq N\_0$ s.t. $\forall n \geq N$.

$\abs{ a\_n } < \frac{ \epsilon }{ 42 N\_0 } $  we claim that this $N $.

works so ... fix $n \geq N $ . We show $\abs{ n a\_n } < \epsilon$. $\abs{ na\_n } \leq \abs{ N\_0 a\_n } + \abs{(n - N\_0) a\_n} \leq (\frac{ \epsilon }{ 42 N\_0 }) N\_0 + \abs{ a\_{N\_0} + ... + a\_n } \leq \frac{ \epsilon }{ 42 } + \frac{ \epsilon }{ 42 }.$

{{% /proof %}}

{{% /example %}}

$ f : D \to R $(D \subseteq \R)

is continuous @ $x\_0 \in D$ iff

for any seq (a\_n) in $ D $,

IF $(a\_n \to x\_0), then f(a\_n) \to f(x\_0) $

Equivalently, $\forall \epsilon > 0 \exists \delta > 0 \forall x if \abs{ x - x\_0 } < \delta$

then $ f(x) - f(x\_0) < \epsilon $.

