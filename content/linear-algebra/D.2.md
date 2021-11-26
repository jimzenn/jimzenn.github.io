---
title: "Discussion"
date: 2018-07-03T11:03:48+08:00
volumes: ["D"]
layout: "note"
type: "notes"
issue: 2
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

$$
\begin{bmatrix}
x\_{11} & x\_{12} \br
x\_{21} & x\_{22} \br
\end{bmatrix}
$$

Note for HW 1

{{% example name="1.3.14" %}}
$S\neq \emptyset$ F is the Field

For any  $s\_0 \in S, \set{f\in (s,F); f(s\_0) = 0}$
is a subspace of $F(S,F)$

(1) $0\in \F(S, F)$ ? What is it?

$0 \in \F(S, F)$? What is it?

$0 \in \F(S, F)$  is a function 0: S-> F s.t.

$0(S) = 0 \in F \forall s\in S$

ex. S= R F= R

o\in \F(S, F) is a function 0. R->R

(2)The meaning for (for any s\_0 \in S)

Gs\_0 = \set{f \in \F(S, F), f(s\_0)= 0} \subset \F(S, F)
this is set depends on choice  of s\_0 \in S

You can fix s\_0\in S and prove that Gs\_0 is a subspace of F(S,F)


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
(ii) $f,g \in C(S,F)$
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

M\_1 = (1 0 0 0), M\_2 = (0 0 0 1), M\_3 = (0 1 1 0)

S = {M\_1, M\_2, M\_3} Then,

span S = the set of all symmetric $2\times 2$ matrices

{{% note name="" %}}

**general strategy to prove A = B**

1.prove $A\subseteq B$
2.prove $B\subseteq A$

$\therefore A = B$

{{% /note %}}

{{% proof name="" %}}
note that W is a subspace of $M\_{2\times2}(F)$

Because $M\_1, M\_2, M\_3 \in W$

i.e. $M\_1 ~ M\_3$  are symmetric

$S \subset W$ and this implies $\spa{S} \subseteq W$

It remains to prove that W \subseq \spa{S}

let M \in W

$M = (a b c d) = a(1 0 0 0) + b(0 1 1 0) + c(0 0 0 1) = a M\_1 + bM\_2 + cM\_3 $

so $M \in \spa{S}$


{{% /proof %}}

{{% /example %}}

{{% example name="" %}}
$R^\infty, (a)\_n \geq 1 = (a\_1, a\_2, ....)$
$e\_1 = (0, 0, ..., 1, 0, ....$
$S = \set{e\_1,e\_2, ...}$
(1) e= (1, 1, 1, ....)
e \in span S?
span S, the set of all vectors in R^\infty
s.t. it is finite linear combination of vectors in S

(argue by contradition)
Suppose $e\in \spa{S}$
$e = a\_1e\_1 + ... + a\_ne\_n$ for some $n \in N$ and $a\_1 \in F$, derive the contradiction.
{{% /example %}}

{{% example name="1.4.14" %}}
S\_1, S\_2 \subeq V, V is vector space

Then $span(S\_1\cup S\_2) = Span(S\_1)+Span(S\_2)$

u\_1+ u\_2 = {u\_1+u\_2 | n\_1 \in u\_1, n\_2 \in u\_2)}

Span(S\_1) + span(S\_2) = \set{v\_1 + v\_2)| v\_1 \in Span(S\_1), v\_2 \in Span(S\_2)}

span(S\_1\cup S\_2) \subseteq Span(S\_1) + Span(S\_2)

{{% proof name="" %}}

($\subseteq$)

let $v\in Span(S\_1 \cup S\_2)$ b given
$v = a\_1w\_1 + ...+ a\_n w\_n$ for some $a\_i\in F w\_1 \in S\_1 \cup S\_2$

$w\_1 \in S\_1 \cup S\_2 \implies w\_i \in S\_1 or w\_i \in S\_2$,

without loss of generality assume $w\_1 ... w\_m  \in S\_1, w\_m+1 ... w\_n  \in S\_2$

$r = a\_1w\_1 +  ... + a\_mw\_m  + a\_\{m+1\}w\_\{m+1\}  + ... a\_nw\_n$

{{% /proof %}}



{{% proof name="" %}}
($\supseteq$)

$Span(S\_1) + Span(S\_2) \subseteq span(S\_1 \cup S\_2)$
$v \in Span(S\_1) + Span(S\_2)$
$v = v\_1 + v\_2$ s.t. $v\_i\in Span(S\_i)$
{{% /proof %}}


{{% /example %}}



{{% example name="1.4.12" %}}

$W \subseteq V, V$ is vector space

$W$ is a subspace $\iff$\spa{W} = W

{{% proof name="" %}}
$(\implies)$

if $W = \spa{W}$
because span of a set is a vector space,
$W = \spa{W}$ is a vector space

$(\impliedby)$
It is trivial to see that $W \subseteq \spa{W}$
it remains to prove $\spa{W} \subseteq W$

let $v \in \spa{W}$
$v = a\_1w\_1 + ... + a\_nw\_n$ for some $a\_i \in F w\_i \in W$,

$a\_1 \in F, w\_i \in W$ we know $W$ is a subspace of $V$

{{% /proof %}}

{{% /example %}}

{{% example name="1.4.16" %}}
$V$ is vector space, $S\subset V, S$ is linearly independent.

Whenever $v\_1, ..., v\_n \in S$ and $a\_1v\_1 + ... + a\_nv\_n = 0$whe have $a\_1= ... = a\_n =0$

Prove that every vector in \spa{S} can be uniquely written as a linear combination of vectors in $S$

{{% /example %}}

{{% example name="1.5.10" %}}
Given an example of three linearly dependent. vectors in $R^2$ s.t. none of the three is a multiple of another.

$v\_1 = (1,0,0), v\_2=(0,1,0)$
$v\_3 = v\_1 + v\_2=(1,1, 0)$

$v\_1 + v\_2 + (-1)v\_3 =0$
$(1, 1, -1) \neq (0, 0, 0)$

{{% /example %}}


{{% example name="1.5.14" %}}

$S$ is linearly dependent
$\iff S = {0}$ or $\exists$ distinct vectors $v\_1, u\_1, u\_2, ... , u\_n \in S$ s.t. $v$ is a linear combination of $u\_1, u\_2, ..., u\_n$

{{% proof name="$\impliedby$" %}}
if S = {0} ,ok
if ...,
$v = a\_1u\_1 + ... + a\_nu\_n$ for same $a\_1\in F$

$a\_1u\_1 + ... + a\_n u\_n + (-1) v = 0$ linearly dependent by definition

{{% /proof %}}

{{% proof name="$\implies$" %}}
If $S = \set{0}$ done
if $S \neq \set{0}$ we need to prove

Because $S$  is linearly dependent.

There are distince vectors $u\_1, u\_2, ..., u\_n \in S, a\_1 \in F $ s.t.


$a\_1u\_1 + ... + a\_nu\_n = 0$, and $(a\_1, ..., a\_n) \neq (0, ..., 0)$

without loss of generality assume

$a\_n \neq =-a\_n u\_n = a\_1u\_1 + ... + a\_{n-1}u\_{n-1}$

Because $a\_n \neq 0$ we have

$u\_n = (-\frac{a\_1}{a\_n}u\_1) + ... + (-\frac{a\_{n-1}}{a\_n}) u\_{n-1}$

{{% /proof %}}

{{% /example %}}

{{% example name="1.5.15" %}}
S = \set{u\_1, ..., u\_n}

S is linearly dependent
$\iff u\_1 =0 or (star)$u\_{k+1}\in Span(\set{u\_1, ..., u\_k})$

for same $k \in \set{1, ..., n -1}$

{{% proof name="$\impliedby$" %}}
if $u\_1 =0$

$u\_1 =0 $ done.

if (star) holds,

let's say $u\_{k+1} \in span(\set{u\_1, ..., u\_k})
$u\_{k+1}$ is a linear combination of $u\_1, ..., u\_k$
Then $S$ is linearly dependent by the previous exercise.

{{% /proof %}}

{{% proof name="$\implies$" %}}

Assume $S$ is linearly dependent

Assume also that $u\_1 \neq 0$ and prove (star)

S is linearly dependent

$\exists a\_i \in F$ s.t. $a\_1u\_1 + ... + a\_nu\_n =0$ and $(a\_1, ..., a\_n) \neq = (0, 0, ..., 0)$

let $k$  be the maximal element of {1, ..., n} s.t. $a\_k \neq 0$


ex) if $a\_n \neq 0$ then $k =n$
if $a\_n, a\_{n-1}, a\_{n-2} = 0, a\_{n-3} \neq 0$ then $k = n-3$

$a\_1u\_1 + ... + a\_ku\_k + a\_{k+1}u\_{k+1} + ...+ a\_nu\_n = 0$

This implies $a\_1u\_1 + ... + a\_ku\_k =0$

$a\_k \neq 0\implies u\_k = (-\frac{a\_1}{a\_k})u\_1+ ... + -\frac{a\_{k-1}{a\_k}u\_{k -1}$

\in $Span({u\_1, ..., u\_{k-1}})$



{{% /proof %}}

{{% /example %}}

We are done... qed. any questions? next
lin comb
elt
s.t.
