---
title: "Discussion 02"
date: 2018-07-03T11:03:48+08:00
author: "Jim Zenn"
volumes: ["Math 115A"]
issue: D2
draft: true
hide: true

---

<!--more-->

<div class="latex-macros">
  {{< raw >}}
    $\newcommand{\R}{\mathbb{R}}$
    $\newcommand{\Q}{\mathbb{Q}}$
    $\newcommand{\Z}{\mathbb{Z}}$
    $\newcommand{\N}{\mathbb{N}}$
    $\newcommand{\C}{\mathbb{C}}$
    $\newcommand{\P}{\mathbb{P}}$
    $\newcommand{\F}{\mathcal{F}}$
    $\newcommand{\set}[1]{\{#1\}}$
    $\newcommand{\emptyset}{\varnothing}$
    $\newcommand{\union}{\cup}$  
    $\newcommand{\intercept}{\cap}$  
    $\newcommand{\abs}[1]{|#1|}$  
    $\newcommand{\t#1}{\text}[1]$  
    $\newcommand{\head}{\text H}$  
    $\newcommand{\tail}{\text T}$  
  {{< /raw >}}
</div>
$$
\begin{bmatrix}
x\_{11} & x\_{12} \\\\\
x\_{21} & x\_{22} \\\\\
\end{bmatrix}
$$

Note for HW 1

{{% example name="1.3.14" %}} 
$S\neq \emptyset$ F is the Field

For any  $s_0 \in S, \set{f\in (s,F); f(s_0) = 0}$
is a subspace of $F(S,F)$

(1) $0\in \F(S, F)$ ? What is it?

$0 \in \F(S, F)$? What is it?

$0 \in \F(S, F)$  is a function 0: S-> F s.t.

$0(S) = 0 \in F \forall s\in S$

ex. S= R F= R

o\in \F(S, F) is a function 0. R->R

(2)The meaning for (for any s_0 \in S)

Gs_0 = \set{f \in \F(S, F), f(s_0)= 0} \subset \F(S, F)
this is set depends on choice  of s_0 \in S

You can fix s_0\in S and prove that Gs_0 is a subspace of F(S,F)


$W\subseteq V$ is a subspace if

(i) $0 \in W$, because V is a vector space there is a unique $0\in V$ In (1) the should prove that this $0\in W$
(ii) add 
(iii) multiplication

{{% /example %}}


{{% example name="1.3.14" %}} 

$S\neq \emptyset, F$ is the field

$C(S, F)$ denote the set of all functions in $\F(S,F)$
s.t. f(s) = 0 for all but a finite number of elements of S.

Prove that $C(S,F)$ is a subspace of $\F(S,F)$

{{% remarks name="" %}} 
f(s) = 0 for all but finitely many  elements of $S$
This means $\set{s \in S, f(s) \neq 0}$ is finite.

This is note equivalent to ${s\in, f(s) = 0}$ is infinite!

example. $f: N -> R, f(0) = 0$ when even 1 when odd


Then {n \in N, f)n = 0} is inifinite.

but does not satisfing C's definition

{{% /remarks %}}

{{% proof name="" %}} 
By definition $C(S, F) \subseteq \F(S, F)$
(1) 0\in C(S, F) because

$0(s) = 0, \forall s\in S$
There is no $s\in S s.t. 0(s) \neq 0$
(ii) $f,g \in C(S,F )$
$A = {s, \in S, f(s) \neq 0}$
$A = {s, \in S, g(s) \neq 0}$
$A, B$ are finite by definition.

$C = \set{s \in S, (f+g)(s) \neq 0} \subset A\cup B$

so $f(s) \neq s\in A$ or $g(s) \neq 0 s\in B$

whenever $s\in C$ we have $s\in A$ or $s \in B$
This means $C\subset A\cup B$
Because $A,B$ are finite, $C$ is also finite, and so $f, g \in C(s,F)$
{{% /proof %}}

{{% /example %}}


{{% example name="1.4.10" %}} 

M_1 = (1 0 0 0 ), M_2 = (0 0 0 1), M_3 = (0 1 1 0)

S = {M_1, M_2, M_3} Then,

span S = the set of all symmetric $2\times 2$ matrices

{{% note name="" %}} 

**general strategy to prove A = B**

1.prove $A\subseteq B$
2.prove $B\subseteq A$

$\therefore A = B$

{{% /note %}}

{{% proof name="" %}} 
note that W is a subspace of $M_{2\times2}(F)$

Because $M_1, M_2, M_3 \in W$

i.e. $M_1 ~ M_3$  are symmetric

$S \subset W$ and this implies $Span(S) \subseteq W$

It remains to prove that W \subseq Span(S)

let M \in W

$M = (a b c d) = a(1 0 0 0) + b(0 1 1 0) + c(0 0 0 1) = a M_1 + bM_2 + cM_3 $

so $M \in Span(S)$


{{% /proof %}}

{{% /example %}}

{{% example name="" %}} 
$R^\infty, (a)_n \geq 1 = (a_1, a_2, ....)$
$e_1 = (0, 0, ..., 1, 0, ....$
$S = \set{e_1,e_2, ...}$
(1) e= (1, 1, 1, ....)
e \in span S?
span S, the set of all vectors in R^\infty
s.t. it is finite linear combination of vectors in S

(argue by contradition)
Suppose $e\in Span(S)$
$e = a_1e_1 + ... + a_ne_n$ for some $n \in N$ and $a_1 \in F$, derive the contradiction.
{{% /example %}}

{{% example name="1.4.14" %}} 
S_1, S_2 \subeq V, V is vector space

Then $span(S_1\cup S_2) = Span(S_1)+Span(S_2)$

u_1+ u_2 = {u_1+u_2 | n_1 \in u_1, n_2 \in u_2)}

Span(S_1) + span(S_2) = \set{v_1 + v_2)| v_1 \in Span(S_1), v_2 \in Span(S_2)}

span(S_1\cup S_2) \subseteq Span(S_1) + Span(S_2)

{{% proof name="" %}} 

($\subseteq$)

let $v\in Span(S_1 \cup S_2)$ b given
$v = a_1w_1 + ...+ a_n w_n$ for some $a_i\in F w_1 \in S_1 \cup S_2$

$w_1 \in S_1 \cup S_2 \implies w_i \in S_1 or w_i \in S_2$,

without loss of generality assume $w_1 ... w_m  \in S_1, w_m+1 ... w_n  \in S_2$

$r = a\_1w\_1 +  ... + a\_mw\_m  + a\_\{m+1\}w\_\{m+1\}  + ... a\_nw\_n$

{{% /proof %}}



{{% proof name="" %}} 
($\supseteq$)

$Span(S_1) + Span(S_2) \subseteq span(S_1 \cup S_2)$
$v \in Span(S_1) + Span(S_2)$
$v = v_1 + v_2$ s.t. $v_i\in Span(S_i)$
{{% /proof %}}


{{% /example %}}



{{% example name="1.4.12" %}} 

$W \subseteq V, V$ is vector space

$W$ is a subspace $\iff$ Span(W) = W

{{% proof name="" %}} 
$(\implies)$

if $ W = Span(W)$
because span of a set is a vector space,
$W = Span(W)$ is a vector space

$(\impliedby)$
It is trivial to see that $W \subseteq Span(W)$
it remains to prove $Span(W) \subseteq W$

let $v \in Span(W)$
$v = a_1w_1 + ... + a_nw_n$ for some $a_i \in F w_i \in W$,

$a_1 \in F, w_i \in W$ we know $W$ is a subspace of $V$

{{% /proof %}}

{{% /example %}}

{{% example name="1.4.16" %}} 
$V$ is vector space, $S\subset V$, $S$ is linearly independent.

Whenever $v_1, ..., v_n \in S$ and $a_1v_1 + ... + a_nv_n = 0$whe have $a_1= ... = a_n =0$

Prove that every vector in Span(S) can be uniquely written as a linear combination of vectors in $S$

{{% /example %}}

{{% example name="1.5.10" %}} 
Given an example of three linearly dependent. vectors in $R^2$ s.t. none of the three is a multiple of another.

$v_1 = (1,0,0), v_2=(0,1,0)$
$v_3 = v_1 + v_2=(1,1, 0)$

$v_1 + v_2 + (-1)v_3 =0$
$(1, 1, -1) \neq (0, 0, 0)$

{{% /example %}}


{{% example name="1.5.14" %}} 

$S$ is linearly dependent
$\iff S = {0}$ or $\exists$ distinct vectors $v_1, u_1, u_2, ... , u_n \in S$ s.t. $v$ is a linear combination of $u_1, u_2, ..., u_n$

{{% proof name="$\impliedby$" %}} 
if S = {0} ,ok
if ...,
$v = a\_1u\_1 + ... + a\_nu\_n$ for same $a\_1\in F$

$a_1u_1 + ... + a_n u_n + (-1) v = 0$ linearly dependent by definition

{{% /proof %}}

{{% proof name="$\implies$" %}} 
If $S = \set{0}$ done
if $S \neq \set{0}$ we need to prove 

Because $S$  is linearly dependent.

There are distince vectors $u\_1, u\_2, ..., u\_n \in S, a\_1 \in F $ s.t. 


$a\_1u\_1 + ... + a\_nu\_n = 0$, and $(a\_1, ..., a\_n) \neq (0, ..., 0)$

without loss of generality assume 

$a\_n \neq =-a\_n u\_n = a\_1u\_1 + ... + a\_{n-1}u\_{n-1}$

Because $a_n \neq 0$ we have

$u\_n = (-\frac{a\_1}{a\_n}u\_1) + ... + (-\frac{a\_{n-1}}{a\_n}) u\_{n-1}$

{{% /proof %}}

{{% /example %}}

{{% example name="1.5.15" %}} 
S = \set{u_1, ..., u_n}

S is linearly dependent
$\iff u_1 =0 or (star)$u_{k+1}\in Span(\set{u_1, ..., u_k})$

for same $k \in \set{1, ..., n -1}$

{{% proof name="$\impliedby$" %}} 
if $u_1 =0$

$u_1 =0 $ done.

if (star) holds,

let's say $u_{k+1} \in span(\set{u_1, ..., u_k})
$u_{k+1}$ is a linear combination of $u_1, ..., u_k$
Then $S$ is linearly dependent by the previous exercise.

{{% /proof %}}

{{% proof name="$\implies$" %}} 

Assume $S$ is linearly dependent

Assume also that $u_1 \neq 0$ and prove (star)

S is linearly dependent

$\exists a_i \in F$ s.t. $a_1u_1 + ... + a_nu_n =0$ and $(a_1, ..., a_n) \neq = (0, 0, ..., 0)$

let $k$  be the maximal element of {1, ..., n } s.t. $a_k \neq 0$


ex) if $a_n \neq 0$ then $k =n$
if $a_n, a_{n-1}, a_{n-2} = 0, a_{n-3} \neq 0$ then $k = n-3$

$a_1u_1 + ... + a_ku_k + a_{k+1}u_{k+1} + ...+ a_nu_n = 0$

This implies $a_1u_1 + ... + a_ku_k =0$ 

$a_k \neq 0\implies u_k = (-\frac{a_1}{a_k})u_1+ ... + (-\frac{a_{k-1}{a_k}u_{k -1}$

\in $Span({u_1, ..., u_{k-1}})$



{{% /proof %}}

{{% /example %}}

We are done... qed. any questions? next
lin comb
elt
s.t.