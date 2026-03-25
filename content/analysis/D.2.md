---
title: "Discussion"
date: 2018-08-14T11:03:48+08:00
volumes: ["D"]
layout: "note"
type: "notes"
issue: 2
draft: true

---


<!--more-->
{{% example name="" %}}

$A, B \neq \emptyset$ bounded above, show $\supr{A+B} = \supr{ A } + \supr{B}$

2 startegies

(1) WTS $\supr{ X } \leq \alpha$ argue that $\forall x \in X, x \leq \alpha $.

(2) To show that $\alpha = \beta $ argue $\alpha \leq \beta$ and $\beta \leq \alpha $.

{{% proof index="" method="" %}}

($\leq $) To show $\supr{ A + B } \leq \supr{ A } + \supr{ B } $

fix an element $z \in A +B $, show

$z \leq \supr{ A } + \supr{ B } $, $z = a+b$

some $a \in A, b \in B$, by def

By def of $sup $, $a \leq \alpha, b \leq \beta$, so

$z = a + b \leq \alpha + \beta $

Hence $\supr{A + B} \leq \alpha + \beta$.

($\geq $) We'll first argue

$\alpha \leq \supr{ A+B } - b, \forall b \in B$

So fix $a \in A$, and $b \in B $.

Then, $a + b \leq \supr{ A + B } $

Then, $a \leq \supr{ A + B } - b$

True for all $a \in A, b \in B $

Hence, $\supr{ A } \leq \supr{ A + B } - b, \forall b \in B$

Also,

$b \leq \supr{ A + B } - \alpha, \forall b \in B $

Thus

$\beta \leq \supr{ A+B } - \alpha $

i.e. $\alpha + \beta \leq \supr{ A+ B } $

{{% /proof %}}

{{% /example %}}

{{% definition name="" status="" %}}

$s\_n \to L$ say $s\_n \to L \forall \epsilon > 0$ there is some $N \in \N $s.t. $\forall n \geq N $, $\abs{ s\_n - L } < \epsilon $.

{{% /definition %}}

{{% example name="" %}}

Determine and prove the limit for $s\_n = \frac{ 2n+1 }{ 5n+3 } $.

{{% proof index="" method="" %}}

We claim that the limit exists and is $\frac{ 2 }{ 5 }$.

Fix an $\epsilon > 0, $ our goal is to find $N $ s.t. if $n \geq N, \abs{ s\_n - \frac{ 2 }{ 5 }} < \epsilon$.

strat 3:

manipulate $\abs{ s\_n - L } $ until you can make it small.

$\abs{ \frac{ 2n+1 }{ 5n+3 } - \frac{ 2 }{ 5 }}  = \abs{ \frac{ 1 }{ 5(5n + 3)}}$

$\frac{ 1 }{ 5(5n + 3)} < \epsilon $

$\iff \frac{ 1 }{ 5 \epsilon } < (5n + 3) $

$\iff \frac{ 1 }{ 5 } \pare{ \frac{ 1 }{ 5 \epsilon } -3 } $

Now fix $n \geq N $ we show $\frac{ 2n + 1 }{ 5n+3 } \frac{ 2 }{ 5 } < \epsilon$

Well, $n \geq N \geq \frac{ 1 }{ 5 }(\frac{ 1 }{ 5 \epsilon } - 3) $ and by earlier arguments.



{{% /proof %}}

{{% /example %}}

{{% example name="" %}}

Show th limit of $\frac{ 6n+4 }{ 3n^2 + 2 } $ is $0$.

{{% proof index="" method="" %}}

Fix $\epsilon > 0$, Find $N $.

s.t.  if $n \geq N $

$\abs{ \frac{ 6n + 4 }{ 4n^2 + 2 }} < \epsilon $

observe that $\forall n \geq 1 $

$\frac{ 6n+4 }{ 3n^2 + 2 } < \frac{ 6n+4 }{ 3n^2 } \leq \frac{ 6n+4 }{ 3n^2 } = \frac{ 10n }{ 3n^2 } = \frac{ 10 }{ 3 } \frac{ 1 }{ n }$

we know that

$\abs{ \frac{ 6n+4 }{ 3n^2 + 2 }} < \frac{ 10 }{ 3 } \frac{ 1 }{ n } < \epsilon$

{{% /proof %}}

{{% /example %}}

{{% lemma name="" index="" %}}

Suppose $t\_n $ bounded, and $s\_n \to 0 $ show $s\_n t\_n \to 0 $.

{{% proof index="" method="" %}}

By def of $t\_n $ bounded, $\exists M > 0 s.t. \forall n$.

$\abs{ t\_n } \leq M$

To show $\lim{s\_n t\_n} \to 0 $

Fix $\epsilon > 0 $

show $\abs{ s\_n t\_n } < \epsilon$

(same $N$)

Observe that $\abs{ s\_nt\_n = \abs{ s\_n } \abs{ t\_n }} \leq \abs{ s\_n } M$

\forall $n$ since $s\_n \to 0 $, we can find same $N $.

s.t. if $n \geq N $(\epsilon := \frac{ \epsilon }{ M })

$\abs{ s\_n } < \frac{ \epsilon }{ M } $ then if $n \geq N $.

$\abs{ s\_n } M < \epsilon $

But $\abs{ s\_n t\_n } \leq \abs{ s\_n } M $.

so $\abs{ s\_n t\_n } < \epsilon $.

{{% /proof %}}

{{% /lemma %}}

