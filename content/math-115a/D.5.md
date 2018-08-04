---
title: "Discussion"
date: 2018-07-24T11:03:48+08:00
menuTitle: "Linear Algebra"
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


$\beta = \set{ u\_1, u\_2, ..., u\_{ n }}$

$x = \sum\_{ i = 1 }^{ n } a\_i u\_i $

$[ x ]\_{ \beta } = {\Vcr{ a\_1 }{ a\_2 }{ \vdots }{ a\_n }} $

$T: \underset{ \beta }{ V } \to \underset{ W }{ \gamma }, \beta = \set{ v\_1, v\_2, ..., v\_{ n }}, \gamma = \set{ w\_1, w\_2, ..., w\_{ n }}$

$T(v\_j)  = \sum\_{ i= 1 }^{ m } a\_{ij} w\_1$

$[ T(v\_j) ]\_{ gamma } = {\Vcr{ a\_{1j}}{ a\_{2j}}{ \vdots }{ v\_{mj}}} $

$[ T ]\_{ \beta }^{ \gamma } = {\Mqr{{\Vce{ \vdots }{ [ T(v\_1) ]\_{ \gamma }}{ \vdots }}}{ [ T(v\_2) ]\_{ \gamma }}{ \vdots }}}{ \hdots }{ [ T(v\_n) ]\_{ \gamma }}{ \vdots }}}} $


{{% example name="HW 4 2.5.14" %}}

$A, B : m \times n matrices$

$P: m \times m , Q : n \times n , invertible$

$B = \inv{ P } A Q $

Then $\exists vector space V $(n-dim) \beta, \beta' W (m-dim) \gamma, \gamma'

$T: V \to  W , s.t. A = [ T ]\_{ \beta }^{ \gamma } B = [ T ]\_{ \beta' }^{ \gamma' }$

$V = F^n, W = F^m$

$\beta, \gamma$ standard ordered bases of $V, W$.

Consider $Q$ this is invertible.

$\beta = \set{ x\_1, ..., x\_n }$

Define $x\_j = \sum\_{ i=1 }^{ n } Q\_{ij}x\_i$ and let $\beta' = \set{ x'\_1, x'\_2, ..., x'\_{ n }} $.

By 2.5.13. $\beta' $ is also a basis. $Q = [ I\_v ]\_{ \beta }^{ \beta' }$.

Similarly, define a basis $\gamma' $ of $W $ s.t.

$P = [ I\_w ]\_{ \gamma }^{ \gamma' } $

Define $T = L\_A $ and check $T(x) = L\_A(x) = Ax $.

{{% /example %}}

{{% example name="HW4 2.5.13" %}}

V. fd vector space over F.

$\beta = \set{ x\_1, x\_2, ..., x\_{ n }}$ ordered basis

$Q: n \times n$ invertible matrix with entries in $F$

define $x\_j = \sum\_{ i=1 }^{ n } Q\_{ij} x\_i $

Then $\beta' = \set{ x'\_1, x'\_2, ..., x'\_{ n }}$ is also a basis of $V$.


Rmk. If $\beta' $ is a basis, then Q is a change of variable mamtrix i.e. $Q = [ I\_v ]\_{ \beta' }^{ \beta }$

{{% /example %}}

{{% proof index="2.5.13" name="" %}}

It is enough to prove that $\beta' $ in linearly independent.

Suppose $a\_1x'\_1 + a\_2x'\_2 + ... + a\_{ n }x'\_{ n } = 0 $

$0 = \sum\_{ j=1 }^{ n } a\_jx'\_j = \sum\_{ j=1 }^{ n } a\_j \sum\_{ i=1 }^{ n }Q\_{ij} x\_i$


$\sum\_{ i=1 }^{ n } \sum\_{ j=1 }^{ n } Q\_{ij} a\_{j} x\_i $

$\because \beta$ is a basis

(\*)  implies that for each $i $.

$b\_i = \sum\_{ j = 1 }^{ n } Q\_{ij} a\_j = 0$

$= {\Vcr{ b\_1 }{ b\_2 }{ \vdots }{ b\_n }} = 0$

denote $v = {\Vcr{ a\_1 }{ a\_2 }{ \vdots }{ a\_n }} $

Then it holds that $Q \cdot v = 0 $

We know $Q $ is invertible.

$\inv{ Q } Q v = \inv{ \Q } 0$

$\implies V = 0$ i.e. $a\_1 = a\_2 = ... = a\_n = 0 $

$\implies \beta' linearly independent $

$implies \beta' basis $


{{% /proof %}}

Recall $T: V \to W $ linear transformation.

T is invertible if there is a map $V: W \to V $ s.t. $TU = Id\_w , UT = Id\_V$

we write $U= \inv{ T } \if exists$

facts:

1. if $T,V$ invertible, then $\inv{ TU } = \inv{ U } \inv{ T }$
2. $\inv{ \inv{ T }} = T$
3. A function is invertible if and only if it is both one-to-one and onto.
4. If $V, W$ is finite dimensional vector space, then
$$T\text{ is invertible} \iff \dim V = \rank{ T } $$ <br>
In general,
$$T\text{ is invertible} \iff T \oto and \ot $$

{{% proof index="" name="" %}}

($\implies $) Suppose $T $ is invertible.

$\inv{ T } T = Id\_V, T \inv{ T }  = Id\_W $


{{% /proof %}}

{{% example name="2.3.12" %}}

(a) UT is H then T is one-to-one.
(b) TU is onto then T is onto.

By (a) (1) T is H.
By (b) (2) T is onto.

($\impliedby $) (outline)

If $T $ is one-to-one, then for each $w \in W $
there is $v \in V $ s.t. $Tv = w (onto) $

and v is unque (one-to-one)

define:

$U: W \to V $ by $U\_w  = v $.

check $U $ is linear.

UT = id

TU = id

{{% /example %}}

{{% example name="2.4.15" %}}

$T: V \to W, T$ is linear transformation. $\beta$ is a basis.

T isomorphism (i.e. linear transformation and invertible).

$\iff T(\beta)# is a basis of $W $

To prove this problem, use (3-2).

Try the case when $\dim V = \infty$.

{{% /example %}}

{{% example name="extra 2.4.16" %}}

$B  n \times n$ matrix.

$\Phi: M\_{n \times n}(F) \to M\_{n \times n}(F) $

$\Phi(A) = \inv{ B }A B $

prove $\Phi $ is isomorphism.

{{% proof index="" name="" %}}

**step 1** $\Phi $ is a linear transformation.o
easy.

**step 2** $\Phi $ is onto.

$\forall c \in M\_{n \times n}(F) $ we  want to find $A \in M\_{n \times n}(F)$

s.t. $C= \Phi (A) $ i.e. $C = \inv{ B }A B $

choose $A = B C \inv{ B } $

$\Phi (B C \inv{  B }) = \inv{ B } (BC \inv{ B }) B = B \inv{ B } C \inv{ B } B = C$

**step 3** $\Phi $ one-to-one.

$\Phi $ linear transformation. It is enough to prove that $N(\Phi)  = \set{ 0 }$

Suppose $\Phi(A) = 0$  i.e. $\inv{ B }A B = 0 $

$A  = B \inv{ B }AB \inv{ B } = B 0 \inv{ B } = 0 $

so $M(\Phi) = \set{ 0 } \Phi $ one-to-one.

By step 1-3, $\Phi $ is invertible.

{{% /proof %}}

{{% /example %}}

{{% example name="2.5" %}}

Characteristic poly, $f(t) = \det(A - tI)$

5.1.11 A, B similar if there is an invertible matrix $Q $ s.t. $B= \inv{ Q } A Q $.

Recall $\lambda $ is an eigenvalue of $T $ if there is a non-zero vector $r \neq 0 $ s.t. $TV = \lambda v $ we call $v $ eigenvector with respect to eigenvalue $\lambda$.

5.1.5

$T lin op on V $

$x $ is an eignevector of $T $ corresponding to eigenvalue $\lambda $ Then for each positive integer $m , x  $ ix an eigenvector, of $T^n $ with eigenvalue $\lambda^m$.

{{% proof index="" name="" %}}
induction on m, m = 1, true.

Suppose the statement is true for some m = x.

$T^nx = \lambda^n x$

Then,


$$\begin{align\*}
T^{n+1}x &= T(T^n x) \br
&= T(\lambda^n x) \text{(by assumption)} \br
&= \lambda^n T(x) \text{(T is linear transformation)} \br
&= \lambda\^n \lambda x \text{(x eigenvector with eigenvalue lambda) \br
&= \lambda \^ n+1 x
\end{align\*}$$

The statement is true for m = n +1

c.f.
$S_1 $ is true, $S_{n+1} $ is true given $S_n $ is true,

$S_1 \to S_2 \to S_3 \to ... $

$S_n$ true for all $n \in N$.

$0 = \emptyset ,1 = \set{ \emptyset, \set{ \emptyset }}, 2 = {1, \set{ 1 }}$.


{{% /proof %}}

{{% /example %}}

{{% example name="5.2.12" %}}

$T$ is invertible. $V$ finite-dimensional vector space.

(a) Recall $\lambda$ eigenvalue of T \implies  \inv{ \lambda } eigenvalue of $\inv{ T' } $. Eigenspace of $T $ with respect to $\lambda $(E_\lambda^T).
= eigenspcae of $\inv{ T } $ with respect to $\inv{ \lambda } (E_{ \inv{ \lambda }})^{ \inv{ T }} $

Eigenspace $E_\lambda = $ set of vectors $v $ s.t. $Tv = \lambda v$ = $v \in V \mid Tv = \lambda v $

$E_ \lambda ^T = E_{ \inv{ \lambda }} ^ { \inv{ T }}$



{{% proof index="" name=" $\subseteq $" %}}

let $v \in E_ \lambda ^T  $ be given.

By definition, T_v = lambda v.

$v = \inv{ T } Tv = \inv{ T } (\lambda v)  = \lambda \cdot \inv{ T } v$

so $\inv{ T } v = \inv{ \lambda } v $

$v $ is and eigenvector of $\inv{ T } $ corresponding to $\inv{ \lambda } $

i.e. $v \in E_{ \inv{ \lambda }}^ { \inv{ T }} $

so $E_\lambda ^ T \subseteq E_{ \inv{ \lambda }} ^ \inv{ T } $

{{% /proof %}}



{{% /example %}}
