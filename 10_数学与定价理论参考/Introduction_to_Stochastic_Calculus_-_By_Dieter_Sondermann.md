

<!-- === Source: MinerU_markdown_Introduction_to_Stochastic_Calculus_-_By_Dieter_Sondermann_1_2122707133446336522.md (Page 1) === -->

## 579 AECTRE OTESIN COSOMCS

Dieter Sondermann 

# Lecture Notes in Economics and Mathematical Systems

Founding Editors: 

M. Beckmann H.P. Künzi 

Managing Editors: 

Prof. Dr. G. Fandel Fachbereich Wirtschaftswissenschaften Fernuniversität Hagen Feithstr. 140/AVZ II, 58084 Hagen, Germany 

Prof. Dr. W. Trockel Institut für Mathematische Wirtschaftsforschung (IMW) Universität Bielefeld Universitätsstr. 25, 33615 Bielefeld, Germany 

Editorial Board: A. Basile, A. Drexl, H. Dawid, K. Inderfurth, W. Kürsten, U. Schittko 

Dieter Sondermann 

# Introduction to Stochastic Calculus for Finance

A New Didactic Approach 

With 6 Figures 

Prof. Dr. Dieter Sondermann Department of Economics University of Bonn Adenauer Allee 24 53113 Bonn, Germany E-mail: sondermann@uni-bonn.de 

ISBN-10 3-540-34836-0 Springer Berlin Heidelberg New York ISBN-13 978-3-540-34836-8 Springer Berlin Heidelberg New York 

This work is subject to copyright. All rights are reserved, whether the whole or part of the material is concerned, specifically the rights of translation, reprinting, reuse of illustrations, recitation, broadcasting, reproduction on microfilm or in any other way, and storage in data banks. Duplication of this publication or parts thereof is permitted only under the provisions of the German Copyright Law of September 9, 1965, in its current version, and permission for use must always be obtained from Springer-Verlag Violations are liable for prosecution under the German Copyright Law. 

Springer is a part of Springer Science+Business Media springeronline.com © Springer-Verlag Berlin Heidelberg 2006 Printed in Germany 

The use of general descriptive names, registered names, trademarks, etc. in this publication does not imply, even in the absence of a specific statement, that such names are exempt from the relevant protective laws and regulations and therefore free for general use. 

Typesetting: Camera ready by author Cover: Erich Kirchner, Heidelberg Production: LE-T X, Jelonek, Schmidt & Vöckler GbR, Leipzig SPIN 11769675 Printed on acid-free paper – 42/3100 – 5 4 3 2 1 0 

To Freddy, Hans and Marek, who patiently helped me to a deeper understanding of stochastic calculus. 

## Preface

There are by now numerous excellent books available on stochastic calculus with specific applications to finance, such as Dufie (2001), Elliott-Kopp (1999), Karatzas-Shreve (1998), Lamberton-Lapeyre (1995), and Shiryaev (1999) on diferent levels of mathematical sophistication. What justifies another contribution to this subject? The motivation is mainly pedagogical. These notes start with an elementary approach to continuous time methods of Itˆo’s calculus due to F¨ollmer. In an fundamental, but not well-known paper published in French in the Seminaire de Probabilit´e in 1981 (see Foellmer (1981)), F¨ollmer showed that one can develop Itˆo’s calculus without probabilities as an exercise in real analysis. <sup>1</sup> 

The notes are based on courses ofered regularly to graduate students in economics and mathematics at the University of Bonn choosing “financial economics” as special topic. To students interested in finance the course opens a quick (but by no means “dirty”) road to the tools required for advanced finance. One can start the course with what they know about real analysis (e.g. Taylor’s Theorem) and basic probability theory as usually taught in undergraduate courses in economic departments and business schools. What is needed beyond (collected in Chap. 1) can be explained, if necessary, in a few introductory hours. 

The content of these notes was also presented, sometimes in condensed form, to MA students at the IMPA in Rio, ETH Z¨urich, to practitioners in the finance industry, and to PhD students and professors of mathematics at the Weizmann institute. There was always a positive feedback. In particular, the pathwise F¨ollmer approach to stochastic calculus was appreciated also by mathematicians not so much familiar with stochastics, but interested in mathematical finance. Thus the course proved suitable for a broad range of participants with quite different background. 

I am greatly indebted to many people who have contributed to this course. In particular I am indebted to Hans F¨ollmer for generously allowing me to use his lecture notes in stochastics. Most of Chapter 2 and part of Chapter 3 follows closely his lecture. Without his contribution these notes would not exist. Special thanks are due to my assistants, in particular to R¨udiger Frey, Antje Mahayni, Philipp Sch¨onbucher, and Frank Thierbach. They have accompanied my courses in Bonn with great enthusiasm, leading the students with engagement through the demanding course material in tutorials and contributing many useful exercises. I also profited from their critical remarks and from comments made by Freddy Delbaen, Klaus Sch¨urger, Michael Suchanecki, and an unknown referee. Finally, I am grateful to all those students who have helped in typesetting, in particular to Florian Schr¨oder. 

Bonn, June 2006 

## Contents

Introduction 1   
1 Preliminaries 3   
1.1 Brief Sketch of Lebesgue's Integral 3   
1.2 Convergence Concepts for Random Variables 7   
1.3 The Lebesgue-Stieltjes Integral.... 10   
1.4 Exercises.... 13   
2 Introduction to Itô-Calculus 15   
2.1 Stochastic Calculus vs. Classical Calculus .... 15   
2.2 Quadratic Variation and 1-dimensional Itô-Formula ... 18   
2.3 Covariation and Multidimensional Itô-Formula.... 26   
2.4 Examples.... 31   
2.5 First Application to Financial Markets.... 33   
2.6 Stopping Times and Local Martingales.... 36   
2.7 Local Martingales and Semimartingales.... 44   
2.8 Itô's Representation Theorem.... 49   
2.9 Application to Option Pricing.... 50   
3 The Girsanov Transformation.... 55   
3.1 Heuristic Introduction.... 55   
3.2 The General Girsanov Transformation.... 58   
3.3 Application to Brownian Motion.... 63   
4 Application to Financial Economics.... 67   
4.1 The Market Price of Risk and Risk-neutral Valuation... 68   
4.2 The Fundamental Pricing Rule.... 73   
4.3 Connection with the PDE-Approach (Feynman-Kac Formula).... 76 

4.4 Currency Options and Siegel-Paradox....78
4.5 Change of Numeraire....79
4.6 Solution of the Siegel-Paradox....84
4.7 Admissible Strategies and Arbitrage-free Pricing....86
4.8 The “Forward Measure”....89
4.9 Option Pricing Under Stochastic Interest Rates....92

5 Term Structure Models....95
5.1 Different Descriptions of the Term Structure of Interest Rates....96
5.2 Stochastics of the Term Structure....99
5.3 The HJM-Model....102
5.4 Examples....105
5.5 The “LIBOR Market” Model....107
5.6 Caps, Floors and Swaps....111

6 Why Do We Need Itô-Calculus in Finance?....113
6.1 The Buy-Sell-Paradox....114
6.2 Local Times and Generalized Itô Formula....115
6.3 Solution of the Buy-Sell-Paradox....120
6.4 Arrow-Debreu Prices in Finance....121
6.5 The Time Value of an Option as Expected Local Time..123

7 Appendix: Itô Calculus Without Probabilities....125
References....135 

## Introduction

The lecture notes are organized as follows: Chapter 1 gives a concise overview of the theory of Lebesgue and Stieltjes integration and convergence theorems used repeatedly in this course. For mathematic students, familiar e.g. with the content of Bauer (1996) or Bauer (2001), this chapter can be skipped or used as additional reference . 

Chapter 2 follows closely F¨ollmer’s approach to Itˆo’s calculus, and is to a large extent based on lectures given by him in Bonn (see Foellmer (1991)). A motivation for this approach is given in Sect. 2.1. This section provides a good introduction to the course, since it starts with familiar concepts from real analysis. 

In Chap. 3 the Girsanov transformation is treated in more detail, as usually contained in mathematical finance textbooks. Sect. 3.2 is taken from Revuz-Yor (1991) and is basic for the following applications to finance. 

The core of this lecture is Chapter 4, which presents the fundamentals of “financial economics” in continuous time, such as the market price of risk, the no-arbitrage principle, the fundamental pricing rule and its invariance under numeraire changes. Special emphasis is laid on the economic interpretation of the so-called “risk-neutral” arbitrage measure and its relation to the “real world” measure considered in general equilibrium theory, a topic sometimes leading to confusion between economists and financial engineers. 

Using the general Girsanov transformation, as developed in Sect. 3.2, the rather intricate problem of the change of numeraire can be treated in a rigorous manner, and the so-called “two-country” or “Siegel” paradox serves as an illustration. The section on Feynman-Kac relates the martingal approach used explicitly in these notes to the more classical approach based on partial diferential equations. 

In Chap. 5 the preceding methods are applied to term structure models. By looking at a term structure model in continuous time in the general form of Heath-Jarrow-Morton (1992) as an infinite collection of assets (the zerobonds of diferent maturities), the methods developed in Chap. 4 can be applied without modification to this situation. Readers who have gone through the original articles of HJM may appreciate the simplicity of this approach, which leads to the basic results of HJM in a straightforward way. The same applies to the now quite popular Libor Market Model treated in Sect. 5.5 . 

Chapter 6 presents some more advanced topics of stochastic calculus such as local times and the generalized Itˆo formula. The basic question here is: Does one really need the apparatus of Itˆo’s calculus in finance? A question which is tantamount to : are charts of financial assets in reality of unbounded variation? The answer is YES, as any practitioner experienced in “delta-hedging” can confirm. Chapter 6 provides the theoretical background for this phenomenon. 

## Preliminaries

Recommended literature : (Bauer 1996), (Bauer 2001) 

We assume that the reader is familiar with the following basic concepts: 

$\varOmega , \mathcal { F } , P )$ is a probability space, i.e. 

$\mathcal { F }$ is a σ-algebra of subsets of the nonempty set $\varOmega$ 

P is a σ-additive measure on $( \varOmega , \mathscr { F } )$ with $P [ \varOmega ] = 1$ 

X is a random variable on $( \varOmega , \mathcal { F } , P )$ with values in $\overline { { \mathbb { R } } } : = [ - \infty , \infty ]$ , i.e. 

X is a map $X : \varOmega \longrightarrow \overline { { \mathbb { R } } }$ with $[ X \leq a ] \in { \mathcal { F } }$ for all $a \in \mathbb { R }$ 

## 1.1 Brief Sketch of Lebesgue’s Integral

The Lebesgue integral of a random variable X can be defined in three steps. 

(a) For a discrete random variable of the form $X = \sum _ { i = 1 } ^ { n } \alpha _ { i } \textbf { 1 } _ { A _ { i } } , \alpha _ { i } \in \mathbb { R }$ 2 $A _ { i } \in { \mathcal { F } }$ the integral (resp. the expectation) of X is defined as 

$$
E [ X ] := \int_ {\Omega} X (\omega) d P (\omega) := \sum_ {i} \alpha_ {i} P [ A _ {i} ].
$$

Note: In the following we will drop the argument $\omega$ in the integral and write shortly $\operatorname* { f } _ { \Omega } X d P$ 

Let $\mathcal { E }$ denote the set of all discrete random variables. 

(b) Consider the set of all random variables which are monotone limits of discrete random variables, i.e. define 

$$
\mathcal {E} ^ {*} := \left\{X: \exists u _ {1} \leq \dots , u _ {n} \in \mathcal {E}, u _ {n} \uparrow X \right\}
$$

Remark: X random variable with $X \geq 0 \Longrightarrow X \in { \mathcal { E } } ^ { * }$ 

For $X \in { \mathcal { E } } ^ { * }$ define 

$$
\int_ {\Omega} X d P := \lim _ {n \longrightarrow \infty} \int_ {\Omega} u _ {n} d P.
$$

(c) For an arbitrary random variable X consider the decomposition $X = X ^ { + } - X ^ { - }$ with 

$$
X ^ {+} := \sup (X, 0)    ,    X ^ {-} := \sup (- X, 0).
$$

According to (b), $X ^ { + } , X ^ { - } \in \mathcal { E } ^ { * }$ 

If either $E [ X ^ { + } ] < \infty$ or $E [ X ^ { - } ] < \infty$ , define 

$$
\int_ {\Omega} X d P := \int_ {\Omega} X ^ {+} d P - \int_ {\Omega} X ^ {-} d P.
$$

Properties of the Lebesgue Integral: 

Linearity : $\int _ { \Omega } ( \alpha X + \beta Y ) d P = \alpha { \underset { \Omega } { \int } } X d P + \beta \int _ { \Omega } Y d P$ 

Positivity : $X \geq 0$ implies $\int X d P \geq 0$ and 

$$
\int X d P > 0 \Longleftrightarrow P [ X > 0 ] > 0.
$$

Monotone Convergence (Beppo Levi). 

Let $( X _ { n } )$ be a monotone sequence of random variables (i.e. $X _ { n } \leq$ $X _ { n + 1 } )$ with $X _ { 1 } \geq C$ . Then 

$$
X := \lim _ {n} X _ {n} \in \mathcal {E} ^ {*}
$$

and 

$$
\lim _ {n \longrightarrow \infty} \int_ {\Omega} X _ {n} d P = \int_ {\Omega} \lim _ {n \longrightarrow \infty} X _ {n} d P = \int_ {\Omega} X d P.
$$

Fatou’s Lemma 

(i) For any sequence $( X _ { n } )$ of random variables which are bounded from below one has 

$$
\int_ {\Omega} \lim _ {n \longrightarrow \infty} \inf X _ {n} d P \leq \lim _ {n \longrightarrow \infty} \inf \int_ {\Omega} X _ {n} d P.
$$

(ii) For any sequence $\left( X _ { n } \right)$ of random variables bounded from above one has 

$$
\int_ {\Omega} \quad \lim _ {n \longrightarrow \infty} \sup X _ {n} d P \geq \quad \lim _ {n \longrightarrow \infty} \sup \int_ {\Omega} X _ {n} d P.
$$

## Jensen’s Inequality

Let X be an integrable random variable with values in IR and $u :$ $\overline { { \mathbb { R } } } \longrightarrow \bar { \mathbb { R } }$ a convex function. 

Then one has 

$$
u (\operatorname{E} [ X ]) \leq \operatorname{E} [ u (X) ].
$$

Jensen’s inequality is frequently applied, e.g. to $u ( X ) = | X | \ , \ u ( X ) =$ $e ^ { X }$ or $u ( X ) = [ X - a ] ^ { + }$ 

## L<sup>p</sup>-Spaces $( 1 \leq p < \infty )$

$\mathrm { L } ^ { p } ( \varOmega )$ denotes the set of all real-valued random variables X on $( \varOmega , \mathcal { F } , P )$ with $\mathrm { { E } } [ | X | ^ { p } ] < \infty$ for some $1 \leq p < \infty$ . For $X \in \mathrm { L } ^ { p }$ , the $\operatorname { L } ^ { p } { \mathrm { - n o r m } }$ is defined as 

$$
| | X | | _ {p} := \left(E [ | X | ^ {p} ]\right) ^ {\frac {1}{p}}.
$$

## 1 Preliminaries

The $\mathrm { L } ^ { p _ { . } }$ -norm has the following properties: 

(a) H¨older’s Inequality 

Given $X \in \ \mathrm { L } ^ { p } ( \varOmega )$ and $Y \in \ \mathrm { L } ^ { q } ( \varOmega )$ with $\begin{array} { r } { \frac { 1 } { p } + \frac { 1 } { q } = 1 } \end{array}$ , one has 

$$
\int_ {\Omega} | X | \cdot | Y | d P \leq \left(\int_ {\Omega} | X | ^ {p} d P\right) ^ {\frac {1}{p}} \cdot \left(\int_ {\Omega} | Y | ^ {q} d P\right) ^ {\frac {1}{q}} d P <   \infty ,
$$

In particular, since $| X \cdot Y | \leq | X | \cdot | Y |$ , implies $X \cdot Y \in \mathrm { ~ L } ^ { 1 } ( \varOmega )$ 

(b) $\mathrm { L } ^ { p } ( \varOmega )$ is a normed vector space. In particular, $X , Y \in ~ \mathrm { L } ^ { p }$ implies $X + Y \in ~ \mathrm { L } ^ { p }$ and one has 

$$
\left| \left| X + Y \right| \right| _ {p} \leq \left| \left| X \right| \right| _ {p} + \left| \left| Y \right| \right| _ {p}. \quad (\text { triangle   inequality })
$$

(c) $\mathrm { L } ^ { q } ~ \subset ~ \mathrm { L } ^ { p }$ for $p < q$ 

## Important special case: $p = 2$

On $\mathrm { L } ^ { 2 }$ , the vector space of quadratically integrable random variables, there exists even a scalar product defined by 

$$
\langle X, Y \rangle := \int_ {\Omega} X \cdot Y d P
$$

Hence one has 

$$
| | X | | _ {2} = \sqrt {\langle X , X \rangle}
$$

and H¨older’s inequality takes the form 

$$
\langle X, Y \rangle = \int_ {\Omega} X \cdot Y d P \leq | | X | | _ {2} \cdot | | Y | | _ {2}.
$$

## 1.2 Convergence Concepts for Random Variables

The strength of the Lebesgue integral, as compared with the Riemann integral, consists in limit theorems - notably ’Lebesgue’s Theorem’ - which allow to study the limit of random variables and their integrals. Without the limit theorems - provided by the Lebesgue integration theory - stochastic analysis would be impossible. 

In this section we collect the basic convergence concepts for sequences of random variables and their relationships. 

Definition 1.2.1. Let $( X _ { n } ) _ { n \in \pmb { N } }$ , X be random variables on $( \varOmega , \mathcal { F } , P )$ 

(a) The sequence $( X _ { n } )$ converges to X P-almost surely if 

$$
P \left[ \{\omega : X _ {n} (\omega) \longrightarrow X (\omega) \} \right] = 1.
$$

We will then write $X _ { n } \longrightarrow X \ P \ - a . s .$ 

(b) The sequence $\left( X _ { n } \right)$ converges in probability if, for every $\epsilon > 0$ 

$$
\lim _ {n \longrightarrow \infty} P \Big [ | X _ {n} - X | > \epsilon \Big ] = 0.
$$

We will then write $P - \operatorname* { l i m } X _ { n } = X$ 

(c) Let $( X _ { n } )$ be in $L ^ { p } ( \varOmega )$ for some $p \in [ 1 , \infty )$ 

The sequence $( X _ { n } )$ converges to $X \underline { { { i n } } } \underline { { { L ^ { p } } } } i f$ 

$$
\lim _ {n \longrightarrow \infty} | | X _ {n} - X | | _ {p} = \lim _ {n \longrightarrow \infty} \left(E [ | X _ {n} - X | ^ {p} ]\right) ^ {\frac {1}{p}} = 0.
$$

We will then write $X _ { n } \longrightarrow X$ in L<sup>p</sup> or $X _ { n } \xrightarrow { L ^ { p } } X$ . (X is then also in $L ^ { p } )$ 

Still another convergence concept for random variables is that of weak convergence, also called convergence in distribution. Since here only the distributions of a random variable matter, the random variables $X _ { n }$ may be defined on diferent probability spaces. Let 

$$
X _ {n}: (\Omega_ {n}, \mathcal {F} _ {n}, P ^ {n}) \longrightarrow E \text {   and   } X: (\Omega , \mathcal {F}, P) \longrightarrow E
$$

be random variables with values in a metric space $E \ ( \mathrm { e . g . } \ E = \mathbb { R }$ or $E = C [ 0 , T ]$ the space of all continuous real-valued functions on $[ 0 , T ] )$ 

Definition 1.2.2. The sequence $( X _ { n } )$ converges to X weakly (or in distribution) if, for every continuous bounded function $f : \overline { { E \longrightarrow } } R$ 2 

$$
\lim _ {n \longrightarrow \infty} \int_ {\Omega_ {n}} f (X _ {n}) d P _ {n} = \lim _ {n \longrightarrow \infty} \int_ {\Omega} f (X) d P.
$$

We will then write $X _ { n } \longrightarrow X$ weakly or $X _ { n } \stackrel { \mathcal { D } } { \longrightarrow } X$ 

## Relations between the diferent notions of convergence

(a) a.s.-convergence and convergence in probability 

$$
\text {(i)} X _ {n} \longrightarrow X P \text {-a.s.} \Longrightarrow P - \lim X _ {n} = X
$$

(ii) P lim $X _ { n } = X \implies \exists$ subsequence $\left( X _ { n ^ { \prime } } \right)$ of $( X _ { n } )$ with $X _ { n ^ { \prime } } \longrightarrow X \ P \mathrm { - a . s . }$ 

(b) Convergence in probability and L<sup>1</sup>-convergence 

Assume $X _ { n } \longrightarrow X { \mathrm { ~ i n ~ L } } ^ { 1 }$ 

$$
\left| \int_ {\Omega} X _ {n} d P - \int_ {\Omega} X d P \right| \leq \int_ {\Omega} | X _ {n} - X | d P \longrightarrow 0
$$

and hence 

$$
\lim _ {n \longrightarrow \infty} \int_ {\Omega} X _ {n} d P = \int_ {\Omega} \lim _ {n \longrightarrow \infty} X _ {n} d P
$$

Thus L<sup>1</sup>-convergence allows to exchange limit and integration, a most important property for stochastic calculus. 

Clearly L<sup>1</sup>-convergence implies convergence in probability. The following simple example shows that the converse does not hold. 

## Example:

Let $\varOmega = [ 0 , 1 ] , \ F =$ Borel-σ-Algebra and $P =$ Lebesgue measure. Consider the sequence $X _ { n } ( \omega ) : = n \cdot \mathbf { 1 } _ { [ 0 , 1 / n ] }$ . Then $X _ { n } \longrightarrow 0 \ P \mathrm { - a . s . }$ ., hence also in probability. But $\textstyle \int X _ { n } d { \dot { P } } = { \dot { 1 } }$ , for all $n .$ . 

The above example shows that an additional condition is needed which prevents the $X _ { n }$ from growing too fast. A suficient condition (which is also necessary) is the following 

Definition 1.2.3. The sequence $( X _ { n } )$ is called uniformly integrable $i f$ 

$$
\lim _ {C \longrightarrow \infty} \sup _ {n} \int_ {| X _ {n} | > C} | X _ {n} | d P = 0.
$$

Suficient conditions for uniform integrability are the following: 1. sup $\mathrm { E } [ | X | ^ { p } ] < \infty$ for some $p > 1$ n 

2. There exists a random variable $Y \in \ \mathrm { L } ^ { 1 }$ such that $\left| X _ { n } \right| \leq Y ~ P _ { - }$ a.s. for all $n .$ . 

Condition 2. is Lebesgue’s ’dominated convergence’ condition. 

The relation between $\mathrm { L } ^ { 1 }$ -convergence and convergence in probability is now given by 

Proposition 1.2.4. (Lebesgue) The following are equivalent: 1. P lim $X _ { n } = X$ and $( X _ { n } )$ is uniformly integrable, 2. $X _ { n } \longrightarrow X$ in $L ^ { 1 }$ . 

Application: (Changing the order of diferentiation and integration) 

Let $X : \mathbb { R } \times \varOmega \longrightarrow \mathbb { R }$ be a family of random variables $X ( t , \cdot )$ , which is, for $P \mathrm { - a . e . } \ \omega \in \varOmega$ , diferentiable in t. If there exists a random variable $Y \in \ \mathrm { L } ^ { 1 } ( \varOmega )$ such that 

$$
| \dot {X} (t, \omega) | \leq Y (\omega) \quad P \text {-a.s.}
$$

then the function $t \longrightarrow \int _ { \Omega } X ( t , \omega ) \ d P ( \omega )$ is diferentiable in t and its derivative is $\intop _ { \Omega } \dot { X } ( t , \omega ) ~ d P ( \omega )$ 

(c) Convergence in distribution and convergence in probability 

Convergence in probability always implies convergence in distribution, i.e. 

$$
P - \lim X _ {n} = X \Longrightarrow X _ {n} \stackrel {\mathcal {D}} {\longrightarrow} X.
$$

The converse only holds if the limit X is $P \mathrm { - a . s }$ . constant. 

## 1.3 The Lebesgue-Stieltjes Integral

From an elementary statistics course the following concepts and notations should be well-known. 

Consider a real-valued random variable X on $( \varOmega , \mathcal { F } , P )$ and a Borelmeasurable mapping $f : \mathbb { R } \longrightarrow \mathbb { R }$ . I.e. we have 

$$
(\Omega , \mathcal {F}, P) \xrightarrow {X} (\mathbb {R}, \mathcal {B}, P _ {X}) \xrightarrow {f} \mathbb {R} \mathrm{with}
$$

$$
P _ {X} [ B ] := P [ X ^ {- 1} (B) ] \quad d i s t r i b u t i o n o f X
$$

$$
F _ {X} (x) := P _ {X} \left[ ] - \infty , x \right] = P [ X \leq x ] \quad \text { distribution   function   of } X.
$$

Then the (Lebesgues-Stieltjes) integral $\textit { f f } ( x ) \ d F _ { X } ( x )$ is well defined IR due to the following integral transformation formula: 

Proposition 1.3.1. 

$$
\int_ {\Omega} f \circ X d P = \int_ {\mathbb {R}} f d P _ {X} = \int_ {\mathbb {R}} f (x) d F _ {X} (x).
$$

Proof. Let $f = \mathbf { 1 } _ { B }$ be the characteristic function of the Borel set $B \in B$ Then by definition of $P _ { X }$ and $F _ { X }$ one has 

$$
\int_ {\Omega} f \circ X d P = \int \mathbf {1} _ {X ^ {- 1} (B)} d P = P [ X ^ {- 1} (B) ] = P _ {X} (B) = \int_ {\mathbb {R}} f d P _ {X}.
$$

By linearity of the integral operator the relation is then also true for all step functions $f \in { \mathcal { E } }$ . By Beppo Levi’s monotone convergence theorem it extends to all $f \in \mathcal { E } ^ { * }$ and hence to all integrable functions $f =$ $f ^ { + } - f ^ { - }$ with $f ^ { + } , f ^ { - } \in { \mathcal { E } } ^ { * }$ □ 

Corollary 1.3.2. $f \circ X \in L ^ { 1 } ( \varOmega , P ) \Longrightarrow f \in L ^ { 1 } ( \varLambda R , P _ { X } ) .$ 

Hence integration on Ω is reduced to integration on IR. In particular, the moments of a random variable $X$ can be computed as Lebesgue-Stieltjes integral with respect to $F _ { X }$ via 

$$
f (x) = x ^ {r} \Longrightarrow E [ X ^ {r} ] = \int_ {\mathbb {R}} x ^ {r} d F _ {X}.
$$

We recall two well-known facts from elementary statistics. 

Properties of $F = F _ { X }$ 

(i) $F$ is isotone, i.e. $x \leq y \Longrightarrow F ( x ) \leq F ( y )$ • 

(ii) $F$ is right continuous, 

(iii) $\operatorname * { l i m } _ { x \longrightarrow - \infty } F ( x ) = 0 ; \ \operatorname * { l i m } _ { x \longrightarrow \infty } F ( x ) = 1 .$ 

Remark 1.1. (i) implies that F has left limits. Together with (ii) this property is often called ’c`adl`ag’ (from the French “continu `a droite - limites `a gauche”). 

Proposition 1.3.3. X is a real random variable on $( \varOmega , \mathcal F , P ) \Longleftrightarrow F _ { X }$ satisfies (i) - (iii) 

Then, for any distribution function F and any Lebesgue-integrable real function $f _ { i }$ , the Lebesgue-Stieltjes Integral $\operatorname* { i f } _ { \mathbb { R } } f d F$ is well-defined and known from elementary statistics courses. 

## Generalization to functions of finite variation

We now consider real-valued right-continuous functions A on the time interval [0, [. The value of A at time t is denoted by A(t) or $A _ { t }$ (Note that the integration variable x is now replaced by t). 

Let Π be the set of all finite subdivisions $\pi$ of the interval [0, t] with $0 = t _ { 0 } < t _ { 1 } < . . . < t _ { n } = t$ . Consider the sum 

$$
V _ {t} ^ {\pi} := \sum_ {i = 0} ^ {n - 1} | A _ {t _ {i + 1}} - A _ {t _ {i}} |
$$

Definition 1.3.4. The function A is of finite variation $i f ,$ for every t, 

$$
V _ {t} (A) = \sup _ {\pi \in \Pi} V _ {t} ^ {\pi} <   + \infty .
$$

The function $t \longrightarrow V _ { t }$ is called the total variation of A. Let $\mathrm { F V } ( \mathbb { R } _ { + } )$ denote the set of all real-valued right-continuous functions on $\mathbb { R } _ { + } = [ 0 , \infty [$ of finite variation. 

Proposition 1.3.5. Every $A \in \mathrm { F V } ( { \mathbb R } _ { + } )$ is the diference of two isotone c`adl`ag functions. 

Proof. Obviously 

$$
A _ {t} = \frac {1}{2} (V _ {t} + A _ {t}) - \frac {1}{2} (V _ {t} - A _ {t}) = A _ {t} ^ {+} - A _ {t} ^ {-}
$$

Both terms are also right-continuous and clearly isotone, hence c`adl`ag. □ 

As a result the function A has left limits at every $t \in ] 0 , \infty [$ . We write $A _ { t ^ { - } } = \operatorname* { l i m } _ { s \nearrow t } A _ { s }$ and set $A _ { 0 ^ { - } } = 0$ 

In exactly the same way as a distribution function $F _ { X }$ defines a measure $P _ { X }$ on (IR, ) via $P _ { X } \Big [ ] - \infty , x \Big ] \Big ] = F _ { X } ( x )$ , every $A \in \mathrm { F V } ( \mathbb { R } _ { + } )$ defines a measure $\mu _ { A }$ on $( \mathbb { R } _ { + } , B )$ given by 

$$
\mu ([ 0, t ]) = A _ {t}.
$$

Note: Of course $\mu _ { A }$ is no longer a probability measure and may take negative values. Such a measure is called a signed measure. 

Likewise as for distribution functions one has 

$$
\mu ([ 0, t [) = A _ {t ^ {-}}
$$

and 

$$
\mu (\{t \}) = \mu_ {A ^ {+}} - \mu_ {A ^ {-}} = \varDelta A _ {t}
$$

is the mass of $\mu$ concentrated in point t. Proposition 1.3.5 leads to the decomposition 

$$
\mu_ {A} = \mu_ {A ^ {+}} - \mu_ {A ^ {-}}
$$

into two positive measures. Hence for any -measurable real-valued function $f$ on $\mathbb { R } _ { + }$ , the Lebesgue-Stieltjes integral is well defined as 

$$
\int f d \mu = \int f d \mu^ {+} - \int f d \mu^ {-} = \int f (s) \mu (d s) = \int f (s) d A (s).
$$

Definition 1.3.6. $\intop _ { 0 } ^ { t } f _ { s } \mathrm { \ } d A _ { s } : = \intop _ { } \mathbf { 1 } _ { | 0 , t | } ( s ) \ f _ { s } \mathrm { \ } d A _ { s }$ is called the integral of f with respect to A integrated over the interval ]0, t]. 

In particular, it follows 

$$
\int_ {0} ^ {t} d A _ {s} = \mu ([ 0, t ]) - \mu (\{0 \}) = A _ {t} - A _ {0}.
$$

## 1.4 Exercises

## Sect. 1.1

1. Show that the Definition 1.1(a) is independent of the representation of $X \in { \mathcal { E } }$ (Hint: If $\overline { { X } } = \sum _ { i = 1 } ^ { n } \alpha _ { i } \ \mathbf { 1 } _ { A _ { i } } = \sum _ { J = 1 } ^ { m } \beta _ { j } \ \mathbf { 1 } _ { B _ { j } }$ use a joint partition of $\varOmega$ as new representation) 

2. Show that the Definition 1.1(b) is independent of the approximating sequence of $X \in { \mathcal { E } } ^ { * }$ 

## Sect. 1.2

1. Let $\varOmega = [ 0 , 1 ]$ be the unit interval with $\mathcal { F }$ the σ-algebra of Borel sets and P the Lebesgue measure. Consider the following sequence $X _ { n } ( \omega ) : [ 0 , 1 ] \longrightarrow \mathbb { R }$ 

$$
X _ {1} (\omega) = \mathbf {1} _ {[ 0, 1 / 2 ]}, \text {   i.e.   } X _ {1} (\omega) = \left\{ \begin{array}{l l} 1, & \omega \in [ 0, 1 / 2 ] \\ 0, & \omega \in [ 1 / 2, 1 ] \end{array} \right.
$$

$$
X _ {2} (\omega) = \mathbf {1} _ {[ 1 / 2, 1 ]}
$$

$$
X _ {3} (\omega) = \mathbf {1} _ {[ 0, 1 / 3 ]}, X _ {4} (\omega) = \mathbf {1} _ {[ 1 / 3, 2 / 3 ]}, X _ {5} (\omega) = \mathbf {1} _ {[ 2 / 3, 1 ]}
$$

$$
X _ {6} (\omega) = \mathbf {1} _ {[ 0, 1 / 4 ]}, \ldots , X _ {9} (\omega) = \mathbf {1} _ {[ 3 / 4, 1 ]} \quad \mathrm{etc.}
$$

Show that $\left( X _ { n } \right)$ converges in probability, but does not converge $P -$ a.s. 

2. Consider $( \varOmega , \mathcal { F } , P )$ as in exercise 1. Define the sequence $X _ { n }$ by 

$$
X _ {n} (\omega) = \left\{ \begin{array}{l l} 0, & \omega <   \frac {1}{2} \\ 1, & \omega \geq \frac {1}{2} \end{array} \right. \text {for n even}
$$

$$
X _ {n} (\omega) = \left\{ \begin{array}{l l} 1, & \omega <   \frac {1}{2} \\ 0, & \omega \geq \frac {1}{2} \end{array} \right. \text { for } n \text { odd }
$$

Show that $X _ { n }$ converges in distribution, but not in probability. 

## Introduction to Itˆo-Calculus

This chapter is based on Foellmer (1981) and follows closely Foellmer (1991). For the techniques used in this chapter we refer to Chap. 1, or to Bauer (1996) resp. Bauer (2001). Some results are quoted (without proof) from Protter (1990) and Revuz-Yor (1991). 

The first elementary applications to option pricing in this chapter deal with the standard Black-Scholes model (Black-Scholes (1973)), first by means of the classical PDE approach (Sect. 2.5), then by using the martingale approach (Sect. 2.9). 

## 2.1 Stochastic Calculus vs. Classical Calculus

Let $X : [ 0 , \infty ] \mapsto$ IR be a real-valued function $X ( t ) = X _ { t }$ . For example the function $X _ { t }$ can describe the speed or the acceleration of a solid body in dependence of time t. But $X _ { t }$ can also represent the price of a security over time, called the chart of the security $X$ . However, there is a fundamental diference between the two interpretations. In the first case $X$ as a function of t is a “smooth” function, not only continuous (natura non facit saltus!), but also (suficiently often) diferentiable. For this class of functions the well-known tools of classical calculus apply. Using the notation $\begin{array} { r } { \dot { X } _ { t } : = \frac { d X _ { t } } { d t } } \end{array}$ for the diferentiation of $X _ { t }$ w.r.t. time $t ,$ as common in physics, the basic relation between diferentiation and integration can be stated as 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \dot {X} _ {s} d s
$$

or 

$$
d X _ {t} = \dot {X} _ {t} d t.
$$

Let $F \in C ^ { 2 } ( \mathbb { R } )$ be a twice continuously diferentiable real-valued function on the real line IR. Then Taylor’s theorem states 

$$
\triangle F (X _ {t}) = F (X _ {t + \triangle t}) - F (X _ {t}) = F ^ {\prime} (X _ {t}) \triangle X _ {t} + \frac {1}{2} F ^ {\prime \prime} (X _ {\tilde {t}}) (\triangle X _ {t}) ^ {2}
$$

with $\triangle X _ { t } = X _ { t + \triangle t } - X _ { t }$ and some $\widetilde t \in [ t , t + \triangle t ]$ 

Taking the limit for $\triangle t  0$ gives 

$$
d F (X _ {t}) = F ^ {\prime} (X _ {t}) d X _ {t}
$$

or, equivalently, 

$$
F (X _ {t}) = F (X _ {0}) + \int_ {0} ^ {t} F ^ {\prime} (X _ {s}) d X _ {s}
$$

since, for a smooth function $X _ { t } , \bigtriangleup X _ { t } \xrightarrow [ \bigtriangleup t  0 ] { } d X _ { t } = \dot { X } _ { t } d t$ , and the terms of higher order, which are of order $( d t ) ^ { 2 }$ , disappear. 

However, this classical relation is no longer applicable for real-valued functions occurring in mathematical finance. When in the 19th century the German mathematician Weierstraß constructed a real-valued function which is continuous, but nowhere diferentiable, this was considered as nothing else but a mathematical curiosity. Unfortunately, this “curiosity” is at the core of mathematical finance. Charts of exchange rates, interest rates, and liquid assets are practically continuous, as the nowadays available high frequency data show. But they are of unbounded variation in every given time interval, as argued in Chap. 6 of these notes. In particular, they are nowhere diferentiable, thus the Weierstraß function depicts a possible finance chart <sup>1</sup>. Therefore classical calculus requires an extension to functions of unbounded variation, a task for long time overlooked by mathematicians. This gap was filled by the development of stochastic calculus, which can be considered as the theory of diferentiation and integration of stochastic processes. 

As already mentioned in the preface, there are now numerous books available developing stochastic calculus with emphasis on applications to financial markets on diferent levels of mathematical sophistication. But here we follow the fundamentally diferent approach due to Foellmer (1981), who showed that one can develop Itˆo’s calculus with out probabilities as an exercise in real analysis. 

What extension of the classical calculus is needed for real-valued functions of unbounded variation? Simply, when forming the diferential $d F ( X _ { t } )$ the second term of the Taylor formula can no longer be neglected, since the term $( \varDelta X _ { t } ) ^ { 2 }$ , the quadratic variation of $X _ { t } ,$ , does not disappear for $\varDelta t  0$ . Thus for functions of unbounded variation the diferential is of the form 

$$
d F (X _ {t}) = F ^ {\prime} (X _ {t}) d X _ {t} + \frac {1}{2} F ^ {\prime \prime} (X _ {t}) (d X _ {t}) ^ {2}\tag{1}
$$

or, in explicit form, 

$$
F (X _ {t}) = F (X _ {0}) + \int_ {0} ^ {t} F ^ {\prime} (X _ {s}) d X _ {s} + \frac {1}{2} \int_ {0} ^ {t} F ^ {\prime \prime} (X _ {s}) (d X _ {s}) ^ {2}\tag{2}
$$

where $( d X _ { t } ) ^ { 2 }$ is the infinitesimal quadratic variation of X. 

Ironically, it was not the newly appearing second term which created the main dificulty in developing stochastic calculus. For functions of finite quadratic variation this $F ^ { \prime \prime } .$ -term is a well-defined classical Lebesgue-Stieltjes integral. The real challenge was to give a precise meaning to the first integral, where both the argument of the integrand and the integrator are of unbounded variation on any arbitrarily small time interval. This task was first <sup>2</sup> solved by Itˆo, hence the name Itˆo formula for the relation (1) and Itˆo integral for the first integral in (2). For a lucid overview over the historic development of the subject see e.g. Foellmer (1998). 

Using the path-wise approach of F¨ollmer one can derive both the Itˆo formula and the Itˆo integral without any recourse to probability theory. By looking at a stochastic process “path by path” one can give a precise meaning to the expressions (1) and (2) by using only elementary tools of classical real analysis.<sup>3</sup> Only later probability theory is needed, when we consider the interplay of all paths of stochastic processes like difusions and semimartingales. 

## 2.2 Quadratic Variation and 1-dimensional Itˆo-Formula

Following Foellmer (1981) we start with a fixed sequence $( \tau _ { n } ) _ { n = 1 , 2 , . . }$ <sub>.</sub> of finite partitions 

$$
\tau_ {n} = \left\{0 = t _ {0} <   t _ {1} <   \ldots <   t _ {i _ {n}} <   \infty \right\}
$$

of $[ 0 , \infty )$ with $t _ { i _ { n } } \to \infty$ and $\left| \tau _ { n } \right| = \operatorname* { s u p } _ { t _ { i } \in \tau _ { n } } \left| t _ { i + 1 } - t _ { i } \right| \underset { n } { \longrightarrow } 0 .$ 

Definition 2.2.1. Let X be a real-valued continuous function on $[ 0 , \infty )$ . If, for all $t \geq 0$ , the limit 

$$
\langle X\rangle_{t} = \lim_{n}\sum_{\substack{t_{i}\in \tau_{n}\\ t_{i}\leq t}}(X_{t_{i + 1}} - X_{t_{i}})^{2}\tag{3}
$$

exists, the function $t \longrightarrow \langle X \rangle _ { t }$ is called the quadratic variation of X. 

Remark 2.1. Following Foellmer $( 1 9 8 1 )$ we start with the study of the paths of a real-valued stochastic process, i.e. a real-valued function $t \longrightarrow X _ { t } ( \omega )$ for a fixed $\omega \in { \mathcal { Q } }$ . It will be shown later, that Definition 2.2.1 and the following results are, for almost all $\omega \in { \mathcal { Q } }$ , independent of the particular choice of the partition sequence $\left( \tau _ { n } \right)$ 

Remark 2.2. Unlike the total variation $V _ { t }$ of X, for the quadratic variation one has 

$$
\langle X \rangle_ {t} \neq \sup _ {\pi} \sum_ {t _ {i} \in \pi} (X _ {t _ {i + 1}} - X _ {t _ {i}}) ^ {2}
$$

where the supremum is taken over all partitions 

$\pi = ( 0 = t _ { 0 } < . . . < t _ { n } = t )$ of [0, t]. As will be shown, for the Brownian motion one has $\langle X \rangle _ { t } = t$ for almost all paths. However, the right-hand side equals + , for almost all paths (see L´evy (1965)). 

Proposition 2.2.2. $X \in { \mathrm { F V } } ( R _ { + } ) \Longrightarrow \langle X _ { t } \rangle \equiv 0 f o r \ a l l t \geq 0$ 

Proof. One has, for any $t \geq 0$ , 

$$
\sum_ {t \geq t _ {i} \in \tau_ {n}} (X _ {t _ {i + 1}} - X _ {t _ {i}}) ^ {2} \leq \sup | X _ {t _ {i + 1}} - X _ {t _ {i}} | \cdot \sum | X _ {t _ {i + 1}} - X _ {t _ {i}} |.
$$

$V _ { t } ( X ) < \infty$ implies that the second term is bounded. $\mathrm { B y }$ continuity of X the first term converges to zero with $\left| { t } _ { i + 1 } - { t } _ { i } \right| \underset { n } { \longrightarrow } 0$ □ 

The above proposition implies that functions $X _ { t }$ with positive quadratic variation $\langle X \rangle _ { t }$ are of unbounded total variation. Hence the integral $\textstyle { \int f ( X _ { t } ) ~ d X _ { t } }$ cannot be defined as a ’classical’ Lebesgue-Stieltjes integral. 

However $t \longrightarrow \langle X \rangle _ { t }$ is a positive and isotone function and thus belongs to $\mathrm { F V } ( \mathbb { R } _ { + } )$ . Hence, as shown in Sect. 1.3, 

$$
\mu ([ 0, t ]) := \langle X \rangle_ {t}
$$

defines a positive measure $\mu$ on $( \mathbb { R } _ { + } , B )$ and the integral 

$$
\int f (s) d \mu (s) = \int f (s) d \langle X \rangle_ {s}
$$

with respect to the quadratic variation $\langle X \rangle$ is well-defined as Lebesgue-Stieltjes integral. 

Remark 2.3. The convergence (3) can be interpreted as weak convergence of measures $\mu _ { n }$ defined by 

$$
\mu_ {n} = \sum_ {t _ {i} \in \tau_ {n}} \left(X _ {t _ {i + 1}} - X _ {t _ {i}}\right) ^ {2} \delta_ {t _ {i}}
$$

where $\delta _ { t _ { i } }$ denotes the Dirac measure with total mass one in $t = t _ { i }$ . Then the sequence $\left( \mu _ { n } \right)$ converges weakly to the measure µ with $d \mu = d \langle X \rangle$ 

Lemma 2.2.3. Let f be a real-valued continuous function on [0, t]. Then one has 

$$
\sum_{\substack{t_{i}\in \tau_{n}\\ t_{i}\leq t}}f(t_{i})  (X_{t_{i + 1}} - X_{t_{i}})^{2} = \int f  \mathbf{1}_{[0,t]}  d\mu_{n}
$$

$$
\underset {n \uparrow \infty} {\longrightarrow} \int f \mathbf {1} _ {[ 0, t ]} d \mu = \int_ {0} ^ {t} f (s) d \langle X \rangle_ {s}.
$$

## Quadratic Variation of the Brownian motion

Definition 2.2.4. A real-valued stochastic process $( B _ { t } ) _ { 0 \leq t < \infty }$ on a probability space $( \varOmega , \mathcal { F } , P )$ is called ’standard Brownian motion’ , if 

(i) $B _ { 0 } = 0$ 

(ii) $t \longrightarrow B _ { t } ( \omega )$ is a continuous function $P - a . s .$ 

(iii) the increments $B _ { t } - B _ { s }$ are independent and have normal distribution $\mathrm { N } ( 0 , t - s )$ , for any $0 \leq s < t$ 

Theorem 2.2.5. (L´evy) For P-almost all paths $t \longrightarrow B _ { t } ( \omega )$ one has 

$$
\langle B \rangle_ {t} (\omega) = t \quad \forall t \geq 0,\tag{4}
$$

Proof. It sufices prove the claim for a fixed $t _ { 0 } \in \mathbb { Q } _ { + }$ , the set of nonnegative rational numbers. Then, since $\mathbb { Q } _ { + }$ is countable, $\langle B \rangle _ { t } ( \omega ) = t$ P-a.s for all $t \in \mathbb { Q } _ { + }$ which by P-a.s continuity of the paths implies P-a.s convergence for all $t \in \mathbb { R } _ { + }$ 

Consider the sequence 

$$
X_{n}:= \sum_{\substack{t_{i}\in \tau_{n}\\ t_{i}\leq t_{0}}}(\underbrace{B_{t_{i + 1}} - B_{t_{i}}}_{=:Y_{i}})^{2} = \sum_{i}Y_{i}^{2}.
$$

By condition (iii) the $Y _ { i }$ are independent with normal distribution $\mathrm { N } ( 0 , \varDelta t _ { i + 1 } )$ . One has 

$$
\begin{array}{c} {\operatorname{E} [ Y _ {i} ^ {2} ] = \sigma^ {2} (Y _ {i}) = \varDelta t _ {i + 1}} \\ {\sigma^ {2} (Y _ {i} ^ {2}) = \operatorname{E} [ Y _ {i} ^ {4} ] - \operatorname{E} [ Y _ {i} ^ {2} ] ^ {2} = 3 \sigma^ {4} (Y _ {i}) - (\varDelta t _ {i + 1}) ^ {2} = 2 (\varDelta t _ {i + 1}) ^ {2}.} \end{array}
$$

From the Central Limit Theorem it follows that, for suficiently large n, the $X _ { n }$ are approximately distributed with normal distribution 

$$
\mathrm{N} \Big (\sum_ {i} \varDelta t _ {i}, 2 \sum_ {i} (\varDelta t _ {i}) ^ {2} \Big)
$$

Clearly, for $n \to \infty$ , these distributions converge to $\mathrm { N } ( t _ { 0 } , 0 )$ . Hence $X _ { n }$ converges weakly to the constant $t _ { 0 }$ , which (see section 1.2.(c)) implies 

$$
P - \lim _ {(\tau_ {n}) _ {n = 1, 2, \ldots}} X _ {n} = t _ {0}.
$$

But this implies (see Sect. 1.2.(a)) that there exists a subsequence $\left( \tau _ { n ^ { \prime } } \right)$ of $\left( \tau _ { n } \right)$ such that 

$$
\langle B \rangle_ {t} = \lim X _ {n ^ {\prime}} = t _ {0} P - a. s..
$$

An immediate consequence of $\mathrm { L e v y } ^ { \prime }$ s theorem is the following 

Corollary 2.2.6. For any $t > 0$ , the paths of the Brownian motion are of unbounded variation on the interval [0, t]. 

Theorem 2.2.7. (Itˆo’s formula in $\scriptstyle { \mathcal { R } } ^ { 1 } )$ : Let $X : [ 0 , \infty ) \longrightarrow I R ^ { 1 }$ be a continuous function with continuous quadratic variation $\langle X \rangle _ { t }$ , and $F \in C ^ { 2 } ( R ^ { 1 } )$ a twice continuously diferentiable real function. Then for any $t \geq 0$ 

$$
F (X _ {t}) = F (X _ {0}) + \int_ {0} ^ {t} F ^ {\prime} (X _ {s}) d X _ {s} + \frac {1}{2} \int_ {0} ^ {t} F ^ {\prime \prime} (X _ {s}) d \langle X \rangle_ {s}\tag{5}
$$

where 

$$
\int \limits_{0}^{t}F^{\prime}(X_{s})  dX_{s} = \lim_{n\uparrow \infty}\sum_{\substack{t_{i}\in \tau_{n}\\ t_{i}\leq t}}F^{\prime}(X_{t_{i}})  (X_{t_{i + 1}} - X_{t_{i}})\tag{6}
$$

Remark 2.4. The Itˆo formula is often written in short notation as 

$$
d F (X) = F ^ {\prime} (X) d X + \frac {1}{2} F ^ {\prime \prime} (X) d \langle X \rangle\tag{7}
$$

called the stochastic diferential of $F ( X )$ . This is nothing else as an equivalent notation for the relation (5). To make it meaningful the two integrals in (5) must be well-defined. This is the case for the second integral which is well-defined as Lebesgue-Stieltjes integral, since the quadratic variation $\langle X \rangle _ { t }$ is of finite variation (see Sect. 1.3). The important contribution of Itˆo consists in developing a well-defined concept for integrals of the first type, where the integrator is of unbounded variation. The existence of the limit (6) is shown in the following proof. 

Remark 2.5. For non-continuous functions X we refer to Foellmer (1981) or Protter (1990) 

Proof of the Theorem: Let $t > 0 \ , \ t _ { i } \in \tau _ { n } \ , \ t _ { i } \leq t$ . By Taylor’s theorem one has 

$$
\begin{array}{l} F (X _ {t _ {i + 1}}) - F (X _ {t _ {i}}) = F ^ {\prime} (X _ {t _ {i}}) (\underbrace {X _ {t _ {i + 1}} - X _ {t _ {i}}} _ {\varDelta X _ {t _ {i}}} \\ \qquad + \frac {1}{2} F ^ {\prime \prime} (X _ {\widetilde {t _ {i}}}) (\varDelta X _ {t _ {i}}) ^ {2} \qquad \widetilde {t} _ {i} \in (t _ {i}, t _ {i + 1}) \\ = F ^ {\prime} (X _ {t _ {i}}) \varDelta X _ {t _ {i}} + \frac {1}{2} F ^ {\prime \prime} (X _ {t _ {i}}) (\varDelta X _ {t _ {i}}) ^ {2} \\ \qquad + \underbrace {\frac {1}{2} \Bigl \{F ^ {\prime \prime} (X _ {\widetilde {t _ {i}}}) - F ^ {\prime \prime} (X _ {t _ {i}}) \Bigr \} (\varDelta X _ {t _ {i}}) ^ {2}} _ {R _ {n} (t _ {i})} \end{array}
$$

Define $\delta _ { n } ~ = ~ \operatorname* { m a x } _ { t _ { i } \in \tau _ { n } , t _ { i } \leq t } | \varDelta X _ { t _ { i } } |$ . Since $F ^ { \prime \prime }$ is uniformly continuous on $X [ 0 , t ]$ , it follows 

$$
\begin{array}{r l} & {| R _ {n} (t _ {i}) | \leq \frac {1}{2} \max _ {\substack {| x - y | \leq \delta_ {n} \\ x, y \in X [ 0, t ]}} | F ^ {\prime \prime} (x) - F ^ {\prime \prime} (y) | (\varDelta X _ {t _ {i}}) ^ {2}} \\ & {\quad \leq \epsilon_ {n} (\varDelta X _ {t _ {i}}) ^ {2}} \end{array}
$$

for some $\epsilon _ { n } > 0$ , which converges to zero as $\delta _ { n } \to 0$ 

For $n \longrightarrow \infty$ it follows 

$$
\begin{array}{l} \text {a)} \Big | \sum_ {t \geq t _ {i} \in \tau_ {n}} R _ {n} (t _ {i}) \Big | \leq \epsilon_ {n} \cdot \underbrace {\sum_ {t \geq t _ {i} \in \tau_ {n}} (\Delta X _ {t _ {i}}) ^ {2}} _ {\text {bounded}} \xrightarrow [ n \uparrow \infty ]{} 0. \\ \text {b)} \sum_ {t \geq t _ {i} \in \tau_ {n}} (F (X _ {t _ {i + 1}} - F (X _ {t _ {i}})) \xrightarrow [ n \uparrow \infty ]{} F (X _ {t}) - F (X _ {0}) \\ \text {c)} \sum \frac {1}{2}   F ^ {\prime \prime} (X _ {t _ {i}})   (\Delta X _ {t _ {i}}) ^ {2}   \xrightarrow [ n \uparrow \infty ]{} \frac {1}{2}   \int_ {0} ^ {t} F ^ {\prime \prime} (X _ {s})   d \langle X _ {s} \rangle . \end{array}
$$

(Observe that the left-hand side of b) is an alternating sum, hence all intermediate members cancel, and the sums in c) converge to the Lebesgue-Stieltjes integral.) 

Hence also $\sum F ^ { \prime } ( X _ { t _ { i } } ) \varDelta X _ { t _ { i } }$ must converge and there exists 

$$
\lim _ {n} \sum_ {t \geq t _ {i} \in \tau_ {n}} F ^ {\prime} (X _ {t _ {i}}) \Delta X _ {t _ {i}} =: \int_ {0} ^ {t} F ^ {\prime} (X _ {s}) d X _ {s}.
$$

Corollary 2.2.8. In the classical case $( \langle X \rangle \equiv 0$ or $X \in \operatorname { F V } )$ Itˆo’s formula reduces to 

$$
F (X _ {t}) = F (X _ {0}) + \int_ {0} ^ {t} F ^ {\prime} (X _ {s}) d X _ {s}
$$

or in short notation, for $X \in C ^ { 1 }$ ， 

$$
d F (X) = F ^ {\prime} (X) d X = F ^ {\prime} (X) \dot {X} d t.
$$

Examples: 

1) $F ( x ) = x ^ { n }$ implies 

$$
X _ {t} ^ {n} = X _ {0} ^ {n} + n \int_ {0} ^ {t} X _ {s} ^ {n - 1} d X _ {s} + \frac {n (n - 1)}{2} \int_ {0} ^ {t} X _ {s} ^ {n - 2} d \langle X \rangle_ {s},
$$

or in short notation 

$$
d (X ^ {n}) = n X ^ {n - 1} d X + \frac {n (n - 1)}{2} X ^ {n - 2} d \langle X \rangle .
$$

In particular, for $n = 2$ and $X _ { t } = B _ { t }$ standard Brownian motion, it follows 

$$
B _ {t} ^ {2} = 2 \int_ {0} ^ {t} B _ {s}. d B _ {s} + \underbrace {\int_ {0} ^ {t} d \langle B \rangle_ {s}} _ {= t}.
$$

2) $F ( x ) = e ^ { X }$ implies 

$$
d (e ^ {X}) = e ^ {X} d X + \frac {1}{2} e ^ {X} d \langle X \rangle ,
$$

$( { \mathrm { i . e . } } \quad d F = F d X$ no longer holds for $F ( X _ { t } ) = e ^ { X _ { t } }$ with $\langle X \rangle \not \equiv 0 )$ 

3) $F ( x ) = \log x$ implies 

$$
d (\log X) = \frac {d X}{X} - \frac {1}{2 X ^ {2}} d \langle X \rangle .
$$

Proposition 2.2.9. Let $X _ { t } ~ = ~ M _ { t } + A _ { t }$ with X and M continuous and $A \in \operatorname { F V }$ . Then the $Q V \langle X \rangle$ exists if and only if M exists, and $\langle X \rangle = \langle M \rangle$ 

Proof. 

$$
\sum (\Delta X) ^ {2} = \sum (\Delta M) ^ {2} + \underbrace {\sum (\Delta A) ^ {2}} _ {\underset {n} {\rightarrow 0}} + 2 \sum \Delta M \cdot \Delta A
$$

$$
\Big|\sum \Delta M\cdot \Delta A\Big|\leq \underbrace{\sup_{t_{i}\in\tau_{n}}|M_{t_{i + 1}} - M_{t_{i}}|}_{\substack{\longrightarrow \\ n0}}\cdot \underbrace{\sum|A_{t_{i + 1}} - A_{t_{i}}|}_{\text{bounded}}.
$$

Proposition 2.2.10. For $F \in C ^ { 1 }$ the quadratic variation of $F ( X _ { t } )$ is given by 

$$
\langle F (X) \rangle_ {t} = \int_ {0} ^ {t} F ^ {\prime} (X _ {s}) ^ {2} d \langle X \rangle_ {s}
$$

Proof. Consider $t > 0 , t _ { i } \in \tau _ { n } , t _ { i } \le t$ . By Taylor’s theorem one has, for some $\widetilde { t } _ { i } \in \left( t _ { i } , t _ { i + 1 } \right)$ , 

$$
\begin{array}{r l} & {| F (X _ {t _ {i + 1}}) - F (X _ {t _ {i}}) | ^ {2} = F (X _ {t _ {i}}) ^ {2} (\varDelta X _ {t _ {i}}) ^ {2}} \\ & {\qquad + \frac {1}{2} (F ^ {\prime} (X _ {\widetilde {t _ {i}}}) - F ^ {\prime} (X _ {t _ {i}})) ^ {2} (\varDelta X _ {t _ {i}}) ^ {2}.} \end{array}
$$

Since $F ^ { \prime }$ is uniformly continuous on $X [ t , 0 ]$ , it follows (see proof of Theorem 2.2.7) 

$$
\sum_{t\geq t_{i}\in \tau_{n}}(F(X_{t_{i + 1}}) - F(X_{t_{i}}))^{2} = \underbrace{\sum F^{\prime}(X_{t_{i}})^{2}(\varDelta X_{t_{i}})^{2}}_{\substack{\longrightarrow \\ \text{Lemma 2.2.3}\int \limits_{0}^{t}F^{\prime}(X_{s})^{2}d\langle X_{s}\rangle}} + \underbrace{\epsilon_{n}\sum(\varDelta X_{t_{i}})^{2}}_{\substack{\longrightarrow \\ n\uparrow\infty}0}
$$

 

Corollary 2.2.11. For $f \in C ^ { 1 }$ the Itˆo integral 

$$
M _ {t} = \int_ {0} ^ {t} f (X _ {s}) d X _ {s}
$$

has the quadratic variation 

$$
\langle M \rangle_ {t} = \int_ {0} ^ {t} f ^ {2} (X _ {s}) d \langle X \rangle_ {s}.
$$

Proof. (for the case that there exists a primitive function F with $F ^ { \prime } =$ $f )$ In this case the Itˆo formula for $F ( X _ { t } )$ is 

$$
F (X _ {t}) = F (X _ {0}) + M _ {t} + \frac {1}{2} \int_ {0} ^ {t} f ^ {\prime} (X _ {s}) d \langle X \rangle_ {s}.
$$

Thus, from Propositions 2.2.9 and 2.2.10, it follows 

$$
\Longrightarrow \langle M \rangle_ {t} = \langle F (X) \rangle_ {t} = \int_ {0} ^ {t} (F ^ {\prime}) ^ {2} (X _ {s}) d \langle X \rangle_ {s}.
$$

Example: $M _ { t } = \intop _ { 0 } ^ { t } B _ { s } d B _ { s }$ has, according to Corollary 2.2.11, the quadratic variation 

$$
\langle M \rangle_ {t} = \int_ {0} ^ {t} B _ {s} ^ {2} d \langle B \rangle_ {s} = \int_ {0} ^ {t} B _ {s} ^ {2} d s \Longrightarrow d \langle M \rangle_ {t} = B _ {t} ^ {2} d t.
$$

## 2.3 Covariation and Multidimensional Itˆo-Formula

Consider two functions $X , Y \in C ^ { 0 } [ 0 , \infty )$ with continuous quadratic variations $\langle X \rangle$ and Y w.r.t. to the (fixed) partition sequence $\left( \tau _ { n } \right)$ We shall see later that all concepts developed w.r.t. to $\left( \tau _ { n } \right)$ are independent of the choice of this particular sequence. 

Definition 2.3.1. If for any $t \geq 0$ 

$$
\langle X,Y\rangle_{t} = \lim_{n\uparrow \infty}\sum_{\substack{t_{i}\in \tau_{n}\\ t_{i}\leq t}}(X_{t_{i + 1}} - X_{t_{i}})(Y_{t_{i + 1}} - Y_{t_{i}})
$$

exists, then the map $t \to \langle X , Y \rangle _ { t }$ is called the covariation of X and $Y .$ Proposition 2.3.2. X, Y exists $i f ,$ and only $i f , \ \langle X + Y \rangle$ exists, and one has 

$$
\langle X, Y \rangle = \frac {1}{2} \left(\langle X + Y \rangle - \langle X \rangle - \langle Y \rangle\right) \quad (\text { Polarization   formula }).
$$

Proof. Follows immediately from 

$$
\begin{array}{r l} \langle X + Y \rangle_ {t} & = \lim \sum (\varDelta X + \varDelta Y) ^ {2} \\ & = \lim (\sum \varDelta X ^ {2} + \sum \varDelta Y ^ {2} + 2 \sum \varDelta X \varDelta Y) \end{array}
$$

Remark 2.6. The polarization formula is obviously equivalent to 

$$
\langle X + Y \rangle = \langle X \rangle + \langle Y \rangle + 2 \langle X, Y \rangle\tag{8}
$$

(compare the variance of the sum of two random variables). 

Example Let $X _ { t } ( w ) , Y _ { t } ( w )$ be two independent Brownian motions on $( \varOmega , \mathcal { F } , P )$ . Then one has 

$$
\langle X, Y \rangle_ {t} (w) = 0 \quad P \text {-a.s.} \quad \forall t \geq 0.
$$

This follows from the fact that $\frac { X _ { t } + Y _ { t } } { \sqrt { 2 } }$ is again the Brownian motion Hence $\langle X + Y \rangle _ { t } = 2 t$ which by (8) implies $\langle X , Y \rangle \equiv 0$ 

Remark 2.7. The covariation $\langle X , Y \rangle$ is the distribution function of a signed measure $\mu = \mu ^ { + } - \mu ^ { - }$ on $[ 0 , \infty )$ (see Sect. 1.3). 

Proposition 2.3.3. Consider f, $g \in C ^ { 1 }$ and their Itˆo integrals 

$$
\begin{array}{l} Y _ {t} = \int_ {0} ^ {t} f (X _ {s}) d X _ {s} \\ Z _ {t} = \int_ {0} ^ {t} g (X _ {s}) d X _ {s} \end{array}
$$

$w . r . t .$ to $X _ { t }$ . Then their covariation is $\langle Y , Z \rangle _ { t } = \intop _ { 0 } ^ { t } f ( X _ { s } ) \ g ( X _ { s } ) \ d \langle X \rangle _ { s }$ 

Proof. From Corollary 2.2.11 it follows 

$$
\begin{array}{r l} & {\langle Y + Z \rangle_ {t} = \Big \langle \int_ {0} ^ {t} (f + g) (X _ {s}) d X _ {s} \Big \rangle_ {t}} \\ & {\qquad = \int_ {0} ^ {t} (f + g) ^ {2} (X _ {s}) d \langle X \rangle_ {s}} \\ & {\qquad = \langle Y \rangle_ {t} + \langle Z \rangle_ {t} + 2 \int_ {0} ^ {t} (f \cdot g) (X _ {s}) d \langle X \rangle_ {s}.} \end{array}
$$

The proposition thus follows from the polarization formula resp. formula (8). 

Let now $X ~ = ~ ( X ^ { 1 } , \ldots , X ^ { d } ) ~ : ~ [ 0 , \infty ) ~ \longrightarrow ~ \mathbb { R } ^ { d }$ be continuous (i.e $X \in C ^ { 0 } [ 0 , \infty ) ^ { d } )$ with continuous covariation 

$$
\langle X ^ {k}, X ^ {l} \rangle_ {t} = \left\{ \begin{array}{c c} \langle X ^ {k} \rangle_ {t} & k = l \\ \frac {1}{2} \Big (\langle X ^ {k} + X ^ {l} \rangle_ {t} - \langle X ^ {k} \rangle_ {t} - \langle X ^ {l} \rangle_ {t} \Big) & k \neq l \end{array} \right.
$$

Example: Brownian motion on $\mathbb { R } ^ { d }$ realized on $\varOmega = C [ 0 , \infty ) ^ { d } ,$ , i.e 

$$
\begin{array}{l} B _ {t} = (B _ {t} ^ {1}, \ldots , B _ {t} ^ {d}) \quad P = \prod_ {i = 1} ^ {d} P _ {i} \qquad P _ {i} = \text {Wiener measure} \\ \implies \langle B ^ {k}, B ^ {l} \rangle_ {t} = t   \delta_ {k l}   P \text {-a.s.}, \qquad \text {where}   \delta_ {k l} = \left\{ \begin{array}{l l} 1 & k = l \\ 0 & k \neq l \end{array} \right. \end{array}
$$

(For existence of $B _ { t }$ and the construction of the Wiener measure on the path space $C ^ { 0 } [ 0 , \infty ) ^ { d }$ see e.g. Bauer (1996)) 

Given $F \in C ^ { 2 } ( \mathbb { R } ^ { d } )$ , we use the following notations: 

$$
\nabla F (x) = \Big (\frac {\partial F}{\partial x _ {1}}, \ldots , \frac {\partial F}{\partial x _ {d}} \Big) (x) = \Big (F _ {x _ {1}} (x), \ldots , F _ {x _ {d}} (x) \Big) = \text { gradient   of } F
$$

$$
\varDelta F (x) = \sum_ {i = 1} ^ {d} F _ {x _ {i}, x _ {i}} (x) = \mathrm{Laplace-operator,i.e.} \varDelta = \sum_ {i = 1} ^ {d} \frac {\partial^ {2}}{\partial x _ {i} ^ {2}}
$$

$$
d F (x) = (\underbrace {\nabla F (x) , d x} _ {\text {scalar product}}) = \sum_ {i} F _ {x _ {i}} (x) \underbrace {d x _ {i}} _ {\dot {x} _ {i} d t} \quad \text {classical differential.}
$$

Theorem 2.3.4. (d-dimensional Itˆo-formula): For $F \in C ^ { 2 } ( R ^ { d } )$ one has 

$$
F (X _ {t}) = F (X _ {0}) + \underbrace {\int_ {0} ^ {t} \nabla F (X _ {s}) d X _ {s}} _ {I t \hat {o} i n t e g r a l} + \frac {1}{2} \sum_ {k, l = 1} ^ {d} \int_ {0} ^ {t} F _ {x _ {k}, x _ {l}} (X _ {s}) d \langle X ^ {k}, X ^ {l} \rangle_ {s},
$$

$$
\text{and the limit}\lim_{n}\sum_{\substack{t_{i}\in \tau_{n}\\ t_{i}\leq t}}\Big(\nabla F(X_{t_{i}}),(X_{t_{i + 1}} - X_{t_{i}})\Big) = : \int \limits_{0}^{t}\nabla F(X_{s})  dX_{s}
$$

exists. 

Proof. The proof is analogous to that of Prop. 2.2.7 by applying the d-dimensional Taylor-formula to the discrete increments of $\mathrm { F }$ □ 

In diferential form the Itˆo-formula can be written as 

$$
d F (X _ {t}) = \left(\nabla F (X _ {t}), d X _ {t}\right) + \frac {1}{2} \sum_ {k, l} \frac {\partial^ {2} F}{\partial x _ {k} \partial x _ {l}} (X _ {t}) d \langle X ^ {k}, X ^ {l} \rangle_ {t}
$$

which is the chain rule for stochastic diferentials. 

Example: For the d-dimensional Brownian motion $B _ { t } = ( B _ { t } ^ { 1 } , \ldots , B _ { t } ^ { d } )$ ， $\langle B ^ { k } , B ^ { l } \rangle _ { t } = t \delta _ { k l }$ implies 

$$
d F (B _ {t}) = \left(\nabla F (B _ {t}), d B _ {t}\right) + \frac {1}{2} \Delta F (B _ {t}) d t.
$$

Corollary 2.3.5. (Product rule for Itˆo calculus): 

For $X , Y$ with continuous $\langle X \rangle , \langle Y \rangle , \langle X , Y \rangle$ it follows 

$$
d (X \cdot Y) = X d Y + Y d X + d \langle X, Y \rangle
$$

i.e. 

$$
X _ {t} Y _ {t} = X _ {0} Y _ {0} + \int_ {0} ^ {t} X _ {s} d Y _ {s} + \int_ {0} ^ {t} Y _ {s} d X _ {s} + \langle X, Y \rangle_ {t}.\tag{9}
$$

Proof. Apply Itˆo’s formula for $d = 2$ to the function $F ( X , Y ) = X \cdot Y \in$ $C ^ { 2 } (  { \mathbb { R } } ^ { 2 } )$ □ 

Remark 2.8. For $Y \in \mathrm { F V }$ it follows that $\langle X + Y \rangle = \langle X \rangle$ , and hence $\langle Y \rangle = 0$ . Thus (9) takes the form 

$$
\int_ {0} ^ {t} Y _ {s} d X _ {s} = X _ {t} Y _ {t} - X _ {0} Y _ {0} - \int_ {0} ^ {t} X _ {s} d Y _ {s}\tag{10}
$$

which is the classical partial integration formula. Observe that $X _ { t }$ may be of infinite variation, since the integral on the right-hand side is welldefined as Stieltjes integral, for $Y _ { t } \in F V$ . By this observation Wiener first obtained a “stochastic” integral for the integrator $X _ { t } ~ = ~ B _ { t }$ and $Y _ { t } = h ( t )$ a deterministic function, the so-called Wiener integral. 

Corollary 2.3.6. (Itˆo’s formula for a time-dependent function) For $F \in \dot { C } ^ { 2 , 1 } ( R _ { + } ^ { 2 } )$ and $X : I R _ { + } \longrightarrow I R$ continuous with continuous X one has 

$$
\begin{array}{l} 1) F (X, t) = F (X _ {0}, 0) + \int_ {0} ^ {t} F _ {x} (X _ {s}, s) d X _ {s} + \int_ {0} ^ {t} F _ {t} (X _ {s}, s) d s \\ \qquad + \frac {1}{2} \int_ {0} ^ {t} F _ {x x} (X _ {s}, s) d \langle X \rangle_ {s} \end{array}
$$

$$
\begin{array}{r l} & {2) F (X, \langle X \rangle_ {t}) = F (X _ {0}, 0) + \int_ {0} ^ {t} F _ {x} (X _ {s}, \langle X \rangle_ {s}) d X _ {s}} \\ & {\qquad + \int_ {0} ^ {t} (\frac {1}{2} F _ {x x} + F _ {t}) (X _ {s}, \langle X _ {s} \rangle) d \langle X \rangle_ {s}.} \end{array}
$$

Proof. Apply Itˆo’s formula for $d = 2$ , to $F ( X , Y )$ and choose $Y _ { t } = t$ resp. $Y _ { t } = \langle X \rangle _ { t }$ □ 

Remark 2.9. The transformation $t \longrightarrow \langle X \rangle _ { t }$ is called time change according to the “interior clock” of the process $X _ { t }$ . In particular, if $F ( X , t )$ satisfies the diferential equation (dual heat equation) 

$$
\frac {1}{2} F _ {x x} + F _ {t} = 0\tag{11}
$$

it follows 

$$
F (X, \langle X \rangle_ {t}) = F (X _ {0}, 0) + \int_ {0} ^ {t} F _ {x} (X _ {s}, \langle X \rangle_ {s}) d X _ {s}.\tag{12}
$$

## 2.4 Examples

1) dG = α G dX (X<sub>0</sub> = 0) 

We show that the above stochastic diferential equation (short: SDE) has the solution 

$$
G _ {t} = G _ {0} + \int_ {0} ^ {t} \alpha G _ {s} d X _ {s} = G _ {0} \mathcal {E} (\alpha X _ {t})
$$

where $\mathcal { E } ( X _ { t } ) : = \exp \{ X _ { t } - \frac { 1 } { 2 } \ \langle X \rangle _ { t } \}$ is the so called stochastic exponential or the Dol´eans-Dade exponential of $Y _ { t }$ 

Proof. $\ F ( x , t ) = G _ { 0 }$ exp $\left\{ \alpha x - { \frac { 1 } { 2 } } \alpha ^ { 2 } t \right\}$ satisfies the dual heat equation (11). Hence by (12), it follows 

$$
G _ {t} = F (X _ {t}, \langle X \rangle_ {t}) = G _ {0} \mathrm{E} (\alpha X _ {t})
$$

$$
\begin{array}{l} \Longrightarrow G _ {t} - G _ {0} = F (X _ {t}, \langle X \rangle_ {t}) - F (X _ {0}, 0) \\ \qquad = \int_ {0} ^ {t} F _ {x} (X _ {s}, \langle X \rangle_ {s}) d X _ {s} = \int_ {0} ^ {t} \alpha G _ {s} d X _ {s}. \end{array} \tag {12}
$$

Remark 2.10. $C l e a r l y , f o r \left. X \right. _ { t } \equiv 0$ one obtains the classical solution $G _ { t } = G _ { 0 } \cdot e ^ { \alpha X _ { t } }$ 

## 2) dG = µ G dt + σ G dX

Here a drift term $\mu$ is added. Using the previous result, it is easy to check that 

$$
G _ {t} = G _ {0} \mathcal {E} (\sigma X _ {t}) e ^ {\mu t} = G _ {0} \exp \left\{\mu t + \sigma X _ {t} - \frac {1}{2} \sigma^ {2} \langle X \rangle_ {t} \right\}
$$

is a solution of the above SDE. 

$$
3) \frac {d S _ {t}}{S _ {t}} = \mu (t) d t + \sigma (t) d B _ {t}
$$

The above SDE defines a difusion or Itˆo process. It is the standard model used in finance for the returns of a security price process $S _ { t }$ with infinitesimal drift $\mu ( t ) d t$ and stochastic noise $\sigma ( t ) d B _ { t }$ , where $\sigma ( t )$ is called the volatility of $S _ { t }$ 

We show that the SDE has the solution 

$$
S _ {t} = S _ {0} \exp \bigg \{\int_ {0} ^ {t} \Big (\mu (s) - \frac {1}{2} \sigma^ {2} (s) \Big) d s + \int_ {0} ^ {t} \sigma (s) d B _ {s} \bigg \}.\tag{13}
$$

Proof. We give a proof using Itˆo’s product formula. The process (13) can be written as 

$$
\begin{array}{l} S _ {t} = S _ {0} \exp \left\{\int_ {0} ^ {t} \mu (s) d s \right\} \cdot \mathcal {E} (M _ {t}) = Y _ {t} \cdot Z _ {t} \\ \text {with} M _ {t} = \int_ {0} ^ {t} \sigma (s) d B _ {s} \text {and} \langle M \rangle_ {t} = \int_ {0} ^ {t} \sigma^ {2} (s) d s. \end{array}
$$

Since $Y _ { t }$ is of finite variation, the product rule implies 

$$
\begin{array}{r l} & {d S _ {t} = Y _ {t} d Z _ {t} + Z _ {t} d Y _ {t} + d \langle Y _ {t}, Z _ {t} \rangle} \\ & {\qquad = Y _ {t} Z _ {t} d M _ {t} + Z _ {t} Y _ {t} \mu (t) d t + 0} \\ & {\qquad = S _ {t} \sigma (t) d B _ {t} + S _ {t} \mu (t) d t.} \end{array}
$$

## 2.5 First Application to Financial Markets

We consider a financial market with only one security without interest and divided payments. This market is modelled as follows: 

$( \varOmega , ( \mathcal F _ { t } ) _ { t \geq 0 } , P )$ is a filtered probability space, i.e., $( \mathcal { F } _ { t } )$ is a family of σ-algebras with $\mathcal { F } _ { s } ~ \subset ~ \mathcal { F } _ { t }$ for $s \ < \ t$ , representing the information available at time t. 

$X _ { t } = X _ { t } ( \omega )$ is the price process of the security adapted to the filtration $( \mathcal { F } _ { t } ) , \mathrm { i . e . } X _ { t }$ is $\mathcal { F } _ { t } .$ -measurable, for all $t \geq 0$ 

$\phi _ { t } = \phi _ { t } ( \omega )$ is another stochastic process adapted to $\mathcal { F } _ { t }$ , called a portfolio strategy. 

$\phi _ { t } = \phi _ { t } ( \omega )$ denotes the number of shares of the security held by an investor at time t in state $\omega$ . Adaptation to $( \mathcal { F } _ { t } )$ means that the investment decision can only be based on the information available at time t. 

Given the portfolio strategy $\phi _ { t }$ , the value of the portfolio at time t is of the form 

$$
V _ {t} = \phi_ {t} X _ {t} + \eta_ {t} = V (X _ {t}, t)\tag{14}
$$

where $\eta _ { t }$ is a money account, yielding no interest. 

A portfolio strategy ( short p.s.) is called self-financing if, after an initial investment $V _ { 0 } = \eta _ { 0 }$ , all changes in the value of the portfolio $V _ { t }$ are only due to the accumulated gains (or losses) resulting from price changes of $X _ { t }$ . Formally this means 

Definition 2.5.1. The $p . s . \phi _ { t }$ is self-financing $\underset { d e f . } { \longleftrightarrow } V _ { t } = V _ { 0 } + \underset { 0 } { \int ^ { t } } \phi _ { s } \ d X _ { s }$ 

$$
\longleftrightarrow d V = \phi d X.
$$

Recall that the Itˆo integral in (2.5.1) is defined as 

$$
\int_ {0} ^ {t} \phi_ {s} d X _ {s} := \lim _ {n} \sum_ {t \geq t _ {i} \in \tau_ {n}} \phi (t _ {i}) (X _ {t _ {i + 1}} - X _ {t _ {i}}),
$$

which means that $\phi ( t _ { i } )$ has to be fixed at the beginning of each investment interval. In other words: the Itˆo integral is non-anticipating, and hence the appropriate concept for finance (in contrast to other stochastic integrals like e.g. the Stratonovich integral). 

Applying Itˆo’s formula to the value process V yields 

$$
\begin{array}{c} {d V = V _ {x} d X + \dot {V} d t + \frac {1}{2} V _ {x x} d \langle X \rangle} \\ {= \phi d X + \dot {V} d t + \frac {1}{2} V _ {x x} d \langle X \rangle} \end{array}
$$

Hence $\phi$ is self-financing if, and only if, V satisfies the diferential equation 

$$
\dot {V} d t + \frac {1}{2} V _ {x x} d \langle X \rangle = 0\tag{15}
$$

for all t > 0, where $\begin{array} { r } { \dot { V } = \frac { \partial } { \partial t } V ( x , t ) } \end{array}$ 

Consequence: Let $H = F ( X _ { T } )$ be a contingent claim (e.g. a ”call” option $H = ( X _ { T } - K ) ^ { + } )$ . If there exists a self-financing p.s. $\phi _ { t }$ with $V _ { T } = H$ then the arbitrage price $V _ { t } = V ( X _ { t } , t )$ of H at the time t satisfies the partial diferential equation (PDE) (15) with boundary condition 

$$
V (X _ {T}, T) = H
$$

and for any $0 \leq t \leq T$ 

$$
V (X _ {t}, t) = V (X _ {0}, 0) + \int_ {0} ^ {t} V _ {x} (X _ {s}, s) d X _ {s}
$$

Remark 2.11. For $X _ { t } = S _ { t }$ as defined in example $\it 2 . 4 . 3$ (Black-Scholes model), one has $d \langle X \rangle _ { t } = \sigma _ { t } ^ { 2 } X _ { t } ^ { 2 }$ dt and (15) is equivalent to the (PDE) 

$$
\dot {V} + \frac {1}{2} \sigma^ {2} X ^ {2} V _ {x x} = 0
$$

This is the classical approach to option pricing, as pioneered by Black-Scholes (1973) and Merton (1973), which leads to the solution ofPDE’s under boundary conditions. 

Assume now that there exists an additional security $Y _ { t } ~ = ~ e ^ { r t }$ , i.e a bond with fixed compounded interest rate $r > 0$ . Consider the following portfolio strategy: 

buy one contingent claim H at price $V .$ 

sell $\phi = V _ { x }$ shares of security X. 

The value of this portfolio is 

$$
\varPi = V - V _ {x} X.
$$

According to Itˆo’s formula it follows 

$$
d \Pi = d V - V _ {x} d X = \dot {V} d t + \frac {1}{2} V _ {x x} \sigma^ {2} X ^ {2} d t.\tag{16}
$$

But, whereas the return $d X _ { t } ( \omega )$ depends on $\omega ,$ , the right-hand side of (16) does not, since $X _ { t } ^ { 2 } ( \omega )$ is fixed at t. Hence the portfolio Π is riskless and by the no-arbitrage principle its return must equal the riskless interest rate, i.e. 

$$
d \Pi = r \Pi d t.\tag{17}
$$

Combining (16) and (17) gives the PDE 

$$
\dot {V} + r X V _ {x} + \frac {1}{2} \sigma^ {2} X ^ {2} V _ {x x} = r \cdot V \quad (\text { Black - Scholes   PDE }).\tag{18}
$$

This PDE holds for any derivative of the form $F ( X _ { T } )$ . A simple example is a forward contract on $X _ { T }$ fixed at time $t = 0$ at price K. It is easy to check that 

$$
F (t) = X _ {t} - K e ^ {- r (T - t)} = V (X _ {t}, t)
$$

is the (unique) solution of (18) under the boundary constraint 

$$
F (T) = V (X _ {T}, T) = X _ {T} - K.
$$

## 2.6 Stopping Times and Local Martingales

In the previous sections we have concentrated on real-valued functions and shown how Itˆo’s calculus comes into play for functions of unbounded variations. The concepts of integration and diferentiation of such functions are quite independent of any probability concept and should indeed be considered as part of the calculus of real-valued functions<sup>4</sup>. But such functions were considered as rather exotic and uninteresting for practical applications and thus neglected in the ’classical’ calculus<sup>5</sup>. Only the study of stochastic processes brought up the need for such an extension of the classical calculus. As will be shown in the following sections, the paths of non-trivial stochastic processes are of unbounded variation. 

We now consider stochastic processes X defined on a probability space $( \varOmega , \mathcal { F } , P )$ with real-valued continuous paths $X _ { t } ( \omega )$ . Of course all concepts developed for real-valued functions in the previous sections apply to the paths of such processes. 

In the following $( \varOmega , ( \mathcal F _ { t } ) _ { t \geq 0 } , P )$ always denotes a probability space with right-continuous filtration satisfying the usual conditions: 

(i) $\mathcal { F } _ { t }$ is a σ-algebra for all $t \geq 0$ 

(ii) $\mathcal { F } _ { s } \subset \mathcal { F } _ { t }$ for $s < t$ 

(iii) $\mathcal { F } _ { s } = \bigcap _ { s < t } \mathcal { F } _ { t }$ for all $s \geq 0$ 

A stochastic process $X = ( X _ { t } ) _ { t \geq 0 }$ on $\bigl ( \Omega , \left( \mathcal { F } _ { t } \right) \bigr )$ is called adapted if, for any t, $X _ { t }$ is $\mathcal { F } _ { t }$ -measurable, i.e. 

$$
\left\{X _ {t} \leq \alpha \right\} \in \mathcal {F} _ {t} \quad \forall \alpha \in \mathbb {R}.
$$

or, shortly, $X _ { t } \in \mathcal { F } _ { t }$ 

Definition 2.6.1. A stochastic process M on $( \varOmega , ( \var F _ { t } ) , P )$ is called a martingale, if 

(i) $( M _ { t } )$ is adapted and integrable $( i . e . \ M _ { t } \in L ^ { 1 } ( \varOmega , \mathcal F _ { t } , P ) \quad \forall t \geq 0 , )$ (ii) $\mathrm { E } [ M _ { t } | { \mathcal F } _ { s } ] = M _ { s } ~ P \ – a . s . ,$ for all $0 \leq s \leq t$ 

Remark 2.12. For a stochastic process X on a probability space $( \varOmega , \mathcal { F } , P )$ consider the following filtration: 

<sup>0</sup><sub>t</sub> := σ(X<sub>s</sub> : s  t) σ-algebra generated by the sets 

$$
\{X _ {s} \leq \alpha : s \leq t, \alpha \in \mathbb {R} \}
$$

$$
\mathcal {F} _ {t} := \bigcap_ {t <   u} \mathcal {F} _ {u} ^ {0} \qquad \text {   right - continuous   modification.   }
$$

$( \mathcal { F } _ { t } )$ is called the natural filtration generated by $( X _ { t } )$ . Clearly, if X has right-continuous paths, $\mathcal { F } _ { t } = \mathcal { F } _ { t } ^ { 0 }$ 

Lemma 2.6.2. $( M _ { t } )$ martingale $\implies \operatorname { E } [ ( M _ { t } - M _ { 0 } ) ^ { 2 } ] = \operatorname { E } [ M _ { t } ^ { 2 } ] - \operatorname { E } [ M _ { 0 } ^ { 2 } ]$ 

$$
P r o o f. (M _ {t} - M _ {0}) ^ {2} = M _ {t} ^ {2} - M _ {0} ^ {2} - 2 M _ {0} (M _ {t} - M _ {0})
$$

$$
\Longrightarrow \operatorname{E} [ (M _ {t} - M _ {0}) ^ {2} ] = \operatorname{E} [ M _ {t} ^ {2} - M _ {0} ^ {2} ] - 2 \operatorname{E} \Big [ M _ {0} \underbrace {\operatorname{E} [ M _ {t} - M _ {0} | \mathcal {F} _ {0} ]} _ {= 0} \Big ]
$$

 

## Examples of martingales:

Let $B = ( B _ { t } ) _ { t \geq 0 }$ be a Brownian motion on $( \varOmega , \mathcal { F } , P )$ with natural filtration $( \mathcal F _ { t } ) _ { t \geq 0 }$ 

$\begin{array} { r l } { ( \mathrm { e . g . } ~ \varOmega } & { { } = C [ 0 , \infty ) = } \end{array}$ all continuous paths 

( ) filtration generated by $( B _ { t } )$ 

$$
\mathcal {F} = \mathcal {F} _ {\infty} = \sigma (B _ {t}: t \geq 0)
$$

$$
P = \text { Wiener   measure })
$$

Proposition 2.6.3. The following processes are martingales with $r e \mathrm { - }$ spect to the filtration $( \mathcal { F } _ { t } )$ 

(1) $B _ { t }$ 

(2) $B _ { t } ^ { 2 } - t$ 

$$
(3) S _ {t} = S _ {0} \exp \left\{\sigma B _ {t} - \frac {1}{2} \sigma^ {2} t \right\} = S _ {0} \mathcal {E} (\sigma B _ {t}).
$$

Proof. (i) The processes are clearly adapted. Integrability follows from (1) $\dot { \mathrm { E } } [ B _ { t } ^ { 2 } ] = \dot { t } < \infty \Longrightarrow B _ { t } \in L ^ { \bar { 2 } } \subset L ^ { \bar { 1 } }$ , 

$$
(2) \mathrm{E} [ | S _ {t} | ] = \mathrm{E} [ S _ {t} ] = S _ {0} \exp \left\{- \frac {1}{2} \sigma^ {2} t \right\} \cdot \underbrace {\mathrm{E} [ e ^ {\sigma B _ {t}} ]} _ {= \exp \{(1 / 2) \sigma^ {2} t \}} = S _ {0} \in L ^ {1}.
$$

Remark 2.13. $X \sim \mathrm { N } ( \mu , \sigma ^ { 2 } ) \Longrightarrow \mathrm { E } [ e ^ { X } ] = \exp \{ \mu + { \frac { 1 } { 2 } } \ \sigma ^ { 2 } \}$ 

(ii) (1) $B _ { t + h } - B _ { t }$ independent of $B _ { t }$ 

$$
\begin{array}{l} \Longrightarrow \operatorname{E} \Big [ B _ {\underbrace {t + h} _ {s}} - B _ {t} \Big | \mathcal {F} _ {t} \Big ] = \operatorname{E} [ B _ {t + h} - B _ {t} ] = 0 \\ \Longrightarrow \operatorname{E} [ B _ {s} | \mathcal {F} _ {t} ] = B _ {t} + \underbrace {\operatorname{E} [ B _ {s} - B _ {t} | \mathcal {F} _ {t} ]} _ {= 0} \quad s \geq t. \end{array}
$$

$$
\begin{array}{r l} & {(2) \mathrm{E} [ B _ {t + h} ^ {2} - B _ {t} ^ {2} | \mathcal {F} _ {t} ] = \mathrm{E} \Big [ (B _ {t + h} - B _ {t}) ^ {2} + 2 (B _ {t + h} - B _ {t}) B _ {t} | \mathcal {F} _ {t} \Big ]} \\ & {\qquad = h + 2 B _ {t} \underbrace {\mathrm{E} [ B _ {t + h} - B _ {t} | \mathcal {F} _ {t} ]} = h.} \end{array}
$$

$$
\begin{array}{c} \mathrm{E} [ S _ {t + h} | \mathcal {F} _ {t} ] = \mathrm{E} \Big [ \underbrace {S _ {0}   \mathcal {E} (\sigma   B _ {t})} _ {S _ {t}}   \mathcal {E} \Big (\sigma (B _ {t + h} - B _ {t}) \Big) \Big | \mathcal {F} _ {t} \Big ] \\ = S _ {t}   \underbrace {\mathrm{E} \Big [ \exp \Big \{\sigma (B _ {t + h} - B _ {t}) - \frac {1}{2}   \sigma^ {2}   h \Big \} \Big ]} _ {= 1}. \end{array}
$$

## Stopping Times

Definition 2.6.4. The random variable $T : \varOmega \longrightarrow [ 0 , \infty ]$ is called a stopping time $i f$ 

$$
[ T \leq t ] \in \mathcal {F} _ {t} \quad (t \geq 0).\tag{19}
$$

Lemma 2.6.5. For a right-continuous filtration the condition (19) is equivalent to 

$$
[ T <   t ] \in \mathcal {F} _ {t} (t \geq 0).
$$

$$
\text { Proof. } (\Longrightarrow) [ T <   t ] = \bigcup_ {n} \underbrace {[ T \leq t - \frac {1}{n} ]} _ {\in \mathcal {F} _ {t - 1 / n}} \in \mathcal {F} _ {t}
$$

$$
(\Longleftarrow) [ T \leq t ] = \bigcap_ {\epsilon > 0} \underbrace {[ T <   t + \epsilon ]} _ {\in \mathcal {F} _ {t + \epsilon}} \stackrel {{\text { right - continuous }}} {{\Longrightarrow}} [ T \leq t ] \in \mathcal {F} _ {t}
$$

Lemma 2.6.6. Every stopping time is a decreasing limit of discrete stopping times. 

Proof. Consider the sequence 

$$
D _ {n} = \left\{K 2 ^ {- n} \mid K = 0, 1, 2, \dots \right\} _ {n = 1, 2, \dots}
$$

of dyadic partitions of the interval $[ 0 , \infty )$ . Define, for any $n _ { ; }$ , 

$$
T _ {n} (\omega) = \left\{ \begin{array}{l l} K 2 ^ {- n} \text {   if   } T (\omega) \in [ (K - 1) 2 ^ {- n}, K 2 ^ {- n}) \\ + \infty \text {   if   } T (\omega) = \infty \end{array} \right.
$$

Clearly, 

$$
[ T _ {n} \leq d ] = [ T _ {n} <   d ] \in \mathcal {F} _ {d} \mathrm{for} d = K 2 ^ {- n} \in D _ {n}
$$

and 

$$
[ T _ {n} \leq t ] = \bigcup_ {t \geq d \in D _ {n}} [ T _ {n} = d ] \in \mathcal {F} _ {t}.
$$

Hence $\left( T _ { n } \right)$ are stopping times and $T _ { n } ( \omega ) \downarrow T ( \omega ) \quad \forall \omega \in \varOmega$ 

Definition 2.6.7. Let T be a stopping time. 

$$
\mathcal {F} _ {T} := \left\{A \in \mathcal {F} _ {\infty}: A \cap \{T \leq t \} \in \mathcal {F} _ {t} \quad \forall   t \geq 0 \right\}
$$

is called the σ-algebra of T-observable events. 

Clearly, for discrete $T _ { n } , \mathcal { F } _ { T _ { n } }$ is a σ-algebra. Hence, by Lemma 2.6.6, 

$$
\mathcal {F} _ {T} = \bigcap_ {n} \mathcal {F} _ {T _ {n}} \quad \mathrm{isa} \sigma \mathrm{-algebra.}
$$

$\mathcal { F } _ { T }$ contains all events which are observable up to the stopping time $T$ 

This is illustrated in the following Fig. 2.1, where ${ \varOmega } = \{ \omega _ { 1 } , \ldots , \omega _ { 8 } \}$ is the set of all paths from $t = 0$ to t = 3 and $\mathcal { F } _ { T } = \sigma \{ A _ { 1 } , A _ { 2 } , A _ { 3 } \}$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/15b73cfa8f4be86aa9c01e228b46d998592649c108caef1ee138500004e4b829.jpg)


t=2 

t=1 

t=0 

Fig. 2.1. Tree of $\mathcal { F } _ { T }$ -observable events 

Remark 2.14. One has 

$\mathcal { F } _ { T } = \sigma \{ X _ { T } : X$ all adapted c`adl`ag processes 

(Protter (1990), p.6) 

Lemma 2.6.8. For an adapted, right-continuous process X the map 

$$
\begin{array}{c} X _ {T}: \Omega \longrightarrow (\mathbb {R} ^ {d}, \mathcal {B} ^ {d}) \\ \omega \longmapsto X _ {T} (\omega) := X _ {T (\omega)} (\omega) \end{array}
$$

is $\mathcal { F } _ { T ^ { - } } m e a s u r a b l e .$ 

Proof. From Lemma 2.6.6 take $T _ { n } \downarrow T$ and $d \in D _ { n }$ 

1) For $X _ { T _ { n } } \in \mathcal { F } _ { T _ { n } }$ and $B \in B ^ { d } , t \geq 0$ it follows 

$$
\begin{array}{c} \{X _ {T _ {n}} \in B \} \cap \{T _ {n} \leq t \} = \bigcup_ {t \geq d \in D _ {n}} \{X _ {T _ {n}} \in B \} \cap \{T _ {n} = d \} \\ = \underbrace {\bigcup_ {t \geq d \in D _ {n}} \underbrace {\{X _ {d} \in B \}} _ {\in \mathcal {F} _ {d}}} _ {\in \mathcal {F} _ {t}}. \end{array}
$$

$$
\begin{array}{r l} 2) (X _ {t}) \text {right - continuous} & \Longrightarrow X _ {T} = \lim _ {n} X _ {T _ {n}} \quad \forall   \omega \in \Omega \\ & \Longrightarrow X _ {T}   \mathcal {F} _ {T} \text {-measurable with} \bigcap_ {n} \mathcal {F} _ {T _ {n}} = \mathcal {F} _ {T}. \end{array}
$$

For any stopping time T, one has 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/5aa8a680f02fe5f2d83d9fd951488668dbaf984eea70d87089b77cdadf7d9286.jpg)


One of the most useful theorems of probability theory is the following so-called ’Optional Stopping Theorem’. 

Theorem 2.6.9. Let $( X _ { t } ) _ { t \geq 0 }$ be a real-valued process which is adapted, integrable and c`adl`ag. 

The following statements are equivalent: 

(i) $( X _ { t } ) _ { t \geq 0 }$ is a martingale, 

(ii) $\operatorname { E } [ X _ { T } ] = \operatorname { E } [ X _ { 0 } ]$ for any bounded stopping time T 

$$
(i. e. T (\omega) \leq c \quad \forall \omega \in \Omega)
$$

(iii) $\operatorname { E } [ X _ { T } | { \mathcal { F } } _ { S } ] = X _ { S }$ for any bounded stopping times $S \leq T$ 

Proof. We use the following notation: 

$$
\int_ {A} X _ {s} d P =: \operatorname{E} [ X _ {s} \mathbf {1} _ {A} ] =: \operatorname{E} [ X _ {s}; A ].
$$

For $X _ { t } \in L ^ { 1 } \in ( \varOmega , \mathscr { F } _ { t } , P )$ it then follows 

$$
\left(X _ {t}\right) \text {   martingale   } \Longleftrightarrow \mathrm{E} [ X _ {s}; A ] = \mathrm{E} [ X _ {t}; A ] \quad \forall s \leq t \quad \forall A \in \mathcal {F} _ {s}.
$$

<sup>(i)</sup> <sup>=</sup>⇒ <sup>(ii):</sup> 

Let $T \leq c ,$ and let $T _ { n } \downarrow T$ be a discretization with partition $D _ { n }$ (compare Lemma 2.6.6), and $A \in \mathcal { F } _ { T _ { n } }$ . Then it follows 

$$
\begin{array}{l} \operatorname{E} [ X _ {T _ {n}}; A ] = \sum_ {d \in D _ {n}} \operatorname{E} [ X _ {d}; A \cap \underbrace {\{T _ {n} = d \}} _ {= \emptyset \text {for} d > c} ] \\ \qquad = \sum_ {d \in D _ {n}} \operatorname{E} [ X _ {c}; A \cap \{T _ {n} = d \} ], \text {since} X \text {is a martingale} \\ \qquad = \operatorname{E} [ X _ {c}; A ]. \end{array}
$$

In particular $\operatorname { E } [ X _ { T _ { n } } ] = \operatorname { E } [ X _ { c } ; { \varOmega } ] = \operatorname { E } [ X _ { 0 } ]$ 

Since $X _ { T } = \operatorname* { l i m } _ { n } X _ { T _ { n } } P \mathrm { - a . s . }$ , Lebesgue’s theorem implies $\operatorname { E } [ X _ { T } ] = \operatorname { E } [ X _ { 0 } ]$ 

(ii) $\implies ( \mathrm { i i i } )$ 

Let $A \in { \mathcal { F } } _ { s } \ , \ S \leq T \leq c$ . Define new stopping time 

$$
\hat {S} (\omega) := \left\{ \begin{array}{l} S (\omega) \omega \in A \\ T (\omega) \omega \in A ^ {c} \end{array} \right.
$$

Since $\hat { S }$ and T are bounded, (ii) implies 

$$
\operatorname{E} [ X _ {\hat {S}} ] = \operatorname{E} [ X _ {0} ] = \operatorname{E} [ X _ {T} ] = \operatorname{E} [ X _ {T}; A ] + \operatorname{E} [ X _ {T}; A ^ {c} ].
$$

On the other hand 

$$
\operatorname{E} [ X _ {\hat {S}} ] = \operatorname{E} [ X _ {S}; A ] + \operatorname{E} [ X _ {T}; A ^ {c} ],
$$

which together with the above equation implies $\operatorname { E } [ X _ { S } ; A ] = \operatorname { E } [ X _ { T } ; A ]$ 

(iii) $\implies ( \mathrm { i } )$ 

Set S s and T t 

 

Remark 2.15. By Lebesgue’s theorem the optional stopping theorem also holds for finite stopping times $T < \infty , P \mathrm { - } a . s . , f o r ( X _ { T \wedge n } )$ uniformly integrable. 

As an application of the optional stopping theorem we consider the hitting times of a Brownian motion for an interval $a \leq 0 < b$ defined by 

$$
T _ {a, b} (\omega) := \min \{t: B _ {t} (\omega) \notin [ a, b ] \}.
$$

Proposition 2.6.10. $P [ B _ { T _ { a , b } } = b ] = \frac { \left| a \right| } { b - a } , P [ B _ { T _ { a , b } } = a ] = \frac { b } { b - a } ,$ 

$$
a n d \quad \operatorname{E} [ T _ {a, b} ] = | a | \cdot b.
$$

Proof. 

$$
\begin{array}{l} 1) 0 = \operatorname{E} [ B _ {0} ] = \operatorname{E} [ B _ {T} ] = b \cdot P [ B _ {T} = b ] + a (1 - P [ B _ {T} = b ]) \\ \implies P [ B _ {T} = b ] = \frac {- a}{b - a}. \end{array}
$$

2) (B<sup>2</sup><sub>t</sub> t) martingale 

$$
\begin{array}{l} \Longrightarrow 0 = \operatorname{E} [ B _ {0} ^ {2} - 0 ] = \operatorname{E} [ B _ {T \wedge n} ^ {2} - T \wedge n ] \\ \Longrightarrow \operatorname{E} [ B _ {T \wedge n} ^ {2} ] = \operatorname{E} [ T \wedge n ] \uparrow \operatorname{E} [ T ] (\text {Beppo - Levi}). \end{array}
$$

On the other hand $\mathrm { E } [ B _ { T \wedge n } ^ { 2 } ] \xrightarrow [ n \uparrow \infty ] { } \mathrm { E } [ B _ { T } ^ { 2 } ]$ , and it follows 

$$
\operatorname{E} [ T ] = \operatorname{E} [ B _ {T} ^ {2} ] = b ^ {2} P [ B _ {T} = b ] + a ^ {2} P [ B _ {T} = a ]
$$

 

Corollary 2.6.11. For the hitting time of $b > 0 , T _ { b } ( \omega ) = \operatorname* { i n f } \{ t :$ $B _ { t } ( \omega ) > b \}$ , it follows 

$$
T _ {b} <   \infty P \text {-a.s., but E[T} _ {b} ] = + \infty .
$$

Proof. 

$$
P [ T _ {b} <   \infty ] = \lim _ {a \downarrow - \infty} P [ T _ {a, b} ] = \lim \frac {| a |}{b + | a |} = 1
$$

$$
\operatorname{E} [ T _ {b} ] \geq \operatorname{E} [ T _ {a, b} ] = | a | \cdot b \xrightarrow [ a \downarrow - \infty ]{} \infty
$$

 

Remark 2.16. This result is rather discouraging for gamblers who follow the “realize-modest-gains” strategy, i.e. choose some $b > 0$ , continue with fixed stake till the cumulated gains reach the bound b, then stop. If the game is “fair”, then, for any $b > 0$ , the gains will surpass b in finite time with probability one. But even for arbitrary small $b > 0$ the average waiting for this to happen is infinite. In the meantime the cumulated losses can become arbitrarily large. 

## 2.7 Local Martingales and Semimartingales

An important result of stochastic calculus is that Itˆo integrals with respect to a martingale are again martingales. This is, however, not quite correct: it is true for the class of local martingales, and more generally for semimartingales. 

Definition 2.7.1. An adapted c`adl`ag process $( M _ { t } ) _ { t \geq 0 }$ is called a local martingale, if there exist stopping times $T _ { 1 } \leq T _ { 2 } \leq . . .$ . such that 

(i) sup $T _ { n } = \infty \ a . s .$ n 

(ii) $( M _ { T _ { n } \wedge t } )$ is a martingale for all n. 

Remark 2.17. By defining new stopping times $T _ { n } ^ { \prime } = T _ { n } \wedge n$ the localizing sequence in the above definition can always be assumed to be bounded (which implies that the martingales $( M _ { T _ { n } ^ { \prime } \wedge t } )$ are uniformly integrable, as required in some standard textbooks). Furthermore, if M is continuous, by setting $S _ { n } = \operatorname* { i n f } \{ t : | X _ { t } | > n \}$ and ${ \cal T } _ { n } ^ { \prime } = T _ { n } \wedge S _ { n }$ one may assume the martingales to be bounded (see Revuz-Yor $( 1 9 9 1 ) , p . 1 1 7 )$ 

The following definition extends the Itˆo integral of stochastic integrands with respect to local martingales in a straightforward way. 

Definition 2.7.2. Let $( H _ { t } ) _ { t \geq 0 }$ be an adapted c`adl`ag process and $( X _ { t } ) _ { t \geq 0 }$ a continuous local martingale. If the following limit exists for all $t \geq 0$ $P - a . s .$ 

$$
M _ {t} (\omega) = \lim _ {n} \sum_ {t \geq t _ {i} \in \tau_ {n}} H _ {t _ {i}} (\omega) \left(X _ {t _ {i + 1}} (\omega) - X _ {t _ {i}} (\omega)\right)
$$

then $\begin{array} { l } { { \displaystyle M _ { t } = \int _ { 0 } ^ { t } H _ { s } d X _ { s } } } \\ { { \displaystyle c t t o ( X _ { t } ) . } } \end{array}$ is called the stochastic integral of $\left( H _ { t } \right)$ with respe 

Remark 2.18. We will see soon that this definition also does not $d e \mathrm { - }$ pend on the specific partition sequence $\left( \tau _ { n } \right)$ 

Theorem 2.7.3. 

$$
M _ {t} = \int_ {0} ^ {t} H _ {s} d X _ {s}\tag{20}
$$

is $a$ local martingale. 

Proof. 1) First assume $( X _ { t } )$ and $\left( H _ { t } \right)$ are bounded, i.e. 

$$
| X _ {t} (\omega) | \leq k \quad \text { and } \quad | H _ {t} (\omega) | \leq l \quad \forall   t, \omega .
$$

We show $( M _ { t } ) _ { t \geq 0 }$ is a $L ^ { 2 } .$ -martingale. Define 

$$
M _ {t} ^ {n} := \sum_ {t \geq t _ {i} \in \tau_ {n}} H _ {t _ {i}} \left(X _ {t _ {i + 1}} - X _ {t _ {i}}\right).
$$

$$
\begin{array}{l} \text {a)} \mathrm{E} [ (M _ {t} ^ {n}) ^ {2} ] = \sum \mathrm{E} \Big [ H _ {t _ {i}} ^ {2} (X _ {t _ {i + 1}} - X _ {t _ {i}}) ^ {2} \Big ] \\ \qquad \leq l ^ {2} \sum_ {t \geq t _ {i} \in \tau_ {n}} \mathrm{E} \Big [ X _ {t _ {i + 1}} ^ {2} - X _ {t _ {i}} ^ {2} - 2   X _ {t _ {i}} (X _ {t _ {i + 1}} - X _ {t _ {i}}) \Big ] \\ \qquad = l ^ {2}   \mathrm{E} \Big [ X _ {t _ {j}} ^ {2} - X _ {t _ {0}} ^ {2} \Big ] \leq l ^ {2} c _ {0} <   \infty \end{array}
$$

where $t _ { j } ~ = ~ \operatorname* { i n f } \{ t _ { i } ~ \in ~ \tau _ { n } ~ : ~ t _ { i } ~ > ~ t \}$ , since $\operatorname { E } [ X _ { t _ { i + 1 } } - X _ { t _ { i } } ] = 0$ and the remaining term is an alternating sum. 

$\implies M _ { t } ^ { n } \in L ^ { 2 }$ and bounded . 

b) $M _ { t } ^ { n }$ is a martingale, for any $t = t _ { i } \in \tau _ { n }$ 

$$
\mathrm{E} \left[ M _ {t _ {i + 1}} ^ {n} - M _ {t _ {i}} ^ {n} | \mathcal {F} _ {t _ {i}} \right] = H _ {t _ {i}} \mathrm{E} \left[ (X _ {t _ {i + 1}} - X _ {t _ {i}}) | \mathcal {F} _ {t _ {i}} \right] = 0
$$

since X is a martingale. 

c) Let $s < t \ , \ A _ { s } \in \mathcal { F } _ { s }$ . To show: 

$$
\operatorname{E} [ M _ {s}; A _ {s} ] = \operatorname{E} [ M _ {t}; A _ {s} ].\tag{21}
$$

Choose $s _ { n } , t _ { n } \in \tau _ { n }$ with $s < s _ { n } < t < t _ { n }$ and $s _ { n } \downarrow s , t _ { n } \downarrow t .$ 

$$
s <   s _ {n} \longrightarrow A _ {s} \in \mathcal {F} _ {s _ {n}} \underset {\text { b) }} {\longrightarrow} \mathrm{E} [ M _ {s _ {n}} ^ {n}; A _ {s} ] = \mathrm{E} [ M _ {t _ {n}} ^ {n}; A _ {s} ].
$$

$$
\left. \begin{array}{l} M _ {s _ {n}} ^ {n} (\omega) \longrightarrow M _ {s} (\omega) P \text {-f.s.} \\ M _ {t _ {n}} ^ {n} (\omega) \longrightarrow M _ {t} (\omega) P \text {-f.s.} \end{array} \right\} \underset {\text {Lebesgue}} {\Longrightarrow} (2 1)
$$

2) The general case can be reduced to 1) by defining the following stopping times 

$$
\begin{array}{l} S _ {n} (\omega) = \inf \{t: | X _ {t} (\omega) | > n \} \\ U _ {n} (\omega) = \inf \{t: | H _ {t} (\omega) | > n \}. \end{array}
$$

Consider the stopping time $V _ { n } = S _ { n } \wedge U _ { n } \wedge T _ { n }$ where $T _ { n }$ is a localizing sequence of bounded stopping times for $( X _ { t } )$ . By assumption $\left( X _ { T _ { n } \wedge t } \right)$ is a martingale. Since $V _ { n } \leq T _ { n }$ , the stopping theorem implies that $\left( X _ { V _ { n } \wedge t } \right)$ is a martingale, and hence by 1) also $\left( M _ { V _ { n } \wedge t } \right)$ Clearly $V _ { n } \uparrow \infty$ . Hence $( M _ { t } )$ is a local martingale. 

## Corollary 2.7.4. $I f \left( X _ { t } \right)$ is a local martingale, then

$X _ { t } ^ { 2 } - \langle X \rangle _ { t } \quad ( t \geq 0 )$ is a local martingale. 

Proof. $d X ^ { 2 } { = } 2 \ X \ d X + d \langle X \rangle , { \mathrm { i . e } }$ . Itˆo 

$$
X _ {t} ^ {2} - \langle X \rangle_ {t} = X _ {0} ^ {2} + \underbrace {2 \int_ {0} ^ {t} X _ {s} d X _ {s}} _ {\text {local martingale}}.
$$

Corollary 2.7.5. Let X be a continuous local martingale with $\langle X \rangle \equiv 0$ $P - a . s$ . Then 

$$
X _ {t} (\omega) \equiv X _ {0} (\omega) P \text {-a.s.},
$$

$i . e .$ , continuous local martingales with paths of finite variation are trivial stochastic processes. 

Proof. $M _ { t } = X _ { t } ^ { 2 } - \langle X \rangle _ { t } = X _ { t } ^ { 2 }$ is a local martingale. 

Let $T _ { n } = T _ { n } ^ { \prime } \wedge T _ { n } ^ { \prime \prime }$ be a joint localizing sequence for $X _ { t }$ and $X _ { t } ^ { 2 }$ . 

$\implies ( X _ { T _ { n } \wedge t } ) \ , \ ( X _ { T _ { n } \wedge t } ^ { 2 } )$ are martingales. Hence if follows: 

$$
0 \leq \operatorname{E} [ (X _ {t} - X _ {0}) ^ {2} ] \underset {(X _ {t} \text {cont.})} {=} \operatorname{E} \Big [ \lim _ {n} (X _ {T _ {n} \wedge t} - X _ {0}) ^ {2} \Big ]
$$

$$
\underset {(\mathrm{Fatou})} {\leq} \liminf _ {n} \mathrm{E} \Big [ (X _ {T _ {n} \wedge t} - X _ {0}) ^ {2} \Big ]
$$

$$
= \liminf _ {(X _ {T _ {n} \wedge t \text {   mart. }})} \operatorname{E} \left[ X _ {T _ {n} \wedge t} ^ {2} - X _ {0} ^ {2} \right]
$$

$$
= 0 _ {(X _ {T _ {n} \wedge t} ^ {2} \mathrm{mart.})}
$$

$$
\Longrightarrow P [ X _ {t} = X _ {0} \quad \forall t \in \mathbb {Q} ] = 1
$$

$$
\underset {(X _ {t} \text {cont.})} {\Longrightarrow} P [ X _ {t} = X _ {0} \quad \forall t ] = 1
$$

 

Now we are able to prove the 

Independence of the calculus from $\left( \tau _ { n } \right)$ : 

Let X be a continuous local martingale. Then 

$$
X _ {t} ^ {2} = X _ {0} ^ {2} + 2 \int_ {0} ^ {t} X _ {s} d X _ {s} + \langle X \rangle_ {t}.
$$

Assume there exist two partition sequences $( \tau _ { n } ^ { ( 1 ) } )$ and $( \tau _ { n } ^ { ( 2 ) } )$ with 

$$
X _ {t} ^ {2} - X _ {0} ^ {2} = \left\{ \begin{array}{l l} \mathrm{Itôintegral} ^ {(1)} + \langle X \rangle_ {t} ^ {(1)} \\ \mathrm{Itôintegral} ^ {(2)} + \langle X \rangle_ {t} ^ {(2)} \end{array} \right.
$$

Then $M _ { t } = \langle X \rangle _ { t } ^ { ( 1 ) } - \langle X \rangle _ { t } ^ { ( 2 ) }$ , as the diference of two Itˆo integrals, is a local martingale with paths of finite variation. Hence by corollary 2.7.5 

$$
M _ {t} (\omega) = M _ {0} = 0 \quad P - \mathrm{a.s.}
$$

But this implies 

$$
\langle X \rangle_ {t} ^ {(1)} - \langle X \rangle_ {t} ^ {(2)} \equiv 0 P - \mathrm{a.s.}
$$

and 

$$
\mathrm{It} \hat {\mathrm{o}} \mathrm{integral} ^ {(1)} \equiv \mathrm{It} \hat {\mathrm{o}} \mathrm{integral} ^ {(2)} P - \mathrm{a.s.}
$$

The same argument applies to the stochastic integral $M _ { t } = \int _ { 0 } ^ { t } H _ { s } d X _ { s } ,$ since $M _ { t }$ is a continuous local martingale. 

We end this section with several suficient conditions for a local martingale to be actually a martingale. 

Proposition 2.7.6. Let M be a local martingale. The following conditions are suficient for M to be a martingale (see Protter (1990) Theorem4 ${ \mathit { 7 } } \left( p . { \mathcal { 3 5 } } \right)$ and Theorem27, Corollary 3 $\left( p . 6 6 \right) )$ 

1) $\mathrm { E } [ \mathrm { s u p } | M _ { s } | ] < \infty \forall t \geq 0 \Longrightarrow M$ is a martingale . e<t 

2) $\mathrm { E } [ \tilde { \underset { t } { \operatorname* { s u p } } } \ | M _ { t } | ] < \infty \Longrightarrow M$ uniformly integrable martingale 

(in particular M bounded) . 

3) $\mathrm { E } [ \langle M \rangle _ { t } ] < \infty \forall t \geq 0 \Longrightarrow M$ is a $L ^ { 2 }$ -martingale and $M ^ { 2 } - \langle M \rangle$ is a 

$$
L ^ {1} \mathrm{-martingale}.
$$

Condition 3) is clearly satisfied by the Brownian motion $( B _ { t } ) _ { t \geq 0 }$ , since $\operatorname { E } [ \langle B \rangle _ { t } ] ~ = ~ t ~ < ~ \infty$ . Hence B is a $L ^ { 2 } { \mathrm { - m a r t i n g a l e } }$ and $\dot { B ^ { 2 } } - \overline { { { \langle } } } B \rangle \ L ^ { 1 } .$ martingale. 

Condition 3) has an interesting interpretation. Let M be a local martingale satisfying 3). Then it follows, for any $t > 0$ , 

$$
M _ {t} ^ {2} - \langle M \rangle_ {t} \quad \text { martingale } \implies \mathrm{E} \Big [ \underbrace {\mathrm{E} [ M _ {t} ^ {2} - \langle M \rangle_ {t} | \mathcal {F} _ {0} ]} _ {M _ {0} ^ {2} - 0} \Big ] = \mathrm{E} [ M _ {0} ^ {2} ].
$$

$$
\begin{array}{r l} \mathrm{Thus} & \mathrm{E} [ M _ {t} ^ {2} ] = \mathrm{E} [ M _ {0} ^ {2} ] + \mathrm{E} [ \langle M \rangle_ {t} ], \mathrm{whichimplies} \\ & \underbrace {\mathrm{Var} [ M _ {t} ]} _ {\mathrm{localin} t} = \mathrm{E} [ M _ {t} ^ {2} ] - (\underbrace {\mathrm{E} [ M _ {t} ]}) ^ {2} = \underbrace {\mathrm{E} [ \langle M \rangle_ {t} ]} _ {\mathrm{globalon} [ 0, t ]}. \end{array}
$$

I.e. the variance of M at time t equals the average quadratic variation of all paths of M on the interval [0, t]. 

According to Theorem2.7.3 the class of local martingales is closed with respect to stochastic integration. This property extends to the larger class of semimartingales. 

Definition 2.7.7. A continuous stochastic process X is called a semimartingale, if there exists a decomposition 

$$
X _ {t} = X _ {0} + M _ {t} + A _ {t}
$$

with $M _ { 0 } = A _ { 0 } = 0$ , M a local martingale and A a process of finite variation. 

If H is another semimartingale, for which - H dX exists, it follows 

$$
\int H d X = \underbrace {\int H d M} _ {\text {local mart.}} + \underbrace {\int H d A} _ {\in \text {FV}}.
$$

Hence - H dX is again a semimartingale. 

## 2.8 Itˆo’s Representation Theorem

Let B be a Brownian motion and H an adapted process. A suficient condition for the stochastic integral $\begin{array} { r } { M _ { t } = \int _ { 0 } ^ { t } H _ { s } \ d B _ { s } } \end{array}$ to be a martingale (see Prop. 2.7.6 (3)) is 

$$
\operatorname{E} [ \langle M \rangle_ {t} ] = \operatorname{E} \left[ \int_ {0} ^ {t} H _ {s} ^ {2} d s \right] <   \infty \quad \forall t
$$

which implies that M is a $L ^ { 2 } .$ -martingale and $M ^ { 2 } - \langle M \rangle$ a $L ^ { 1 }$ -martingale. 

The following theorem (see e.g. Revuz-Yor (1991) p.187) shows that the converse also holds. 

## Theorem 2.8.1. (Itˆo’s representation theorem)

Let B a Brownian motion on $( \varOmega , ( \var F _ { t } ) , P )$ with “natural” filtration (generated by $\left( B _ { t } \right)$ and all P-null sets) and M a $L ^ { 2 }$ -martingale on $( \mathcal { F } _ { t } , P )$ .Then there exists an adapted process H with 

$$
\operatorname{E} \left[ \int_ {0} ^ {t} H _ {s} ^ {2} d s \right] <   \infty t \geq 0
$$

such that 

$$
M _ {t} = M _ {0} + \int_ {0} ^ {t} H _ {s} d B _ {s} \quad \forall t \geq 0.
$$

## 2.9 Application to Option Pricing

Let B denote again a Brownian motion on $( \varOmega , ( \var F _ { t } ) , P )$ with natural filtration. 

Let $( S _ { t } ) _ { t \geq 0 }$ be a price process adapted to $( \mathcal { F } _ { t } )$ and $C$ an option depending on the paths of $( S _ { t } ) _ { 0 \leq t \leq T }$ , for some fixed $T$ . 

Examples: $C ( \omega ) = [ S _ { T } ( \omega ) - K ] ^ { + }$ 

call option 

$$
C (\omega) = \max _ {0 \leq t \leq T} S _ {t} (\omega)
$$

lookback option 

$$
C (\omega) = [ S _ {T} (\omega) - K ] ^ {+} \cdot \mathbf {1} _ {\{S _ {t} (\omega) > L   \forall   t \leq T \}}   \text {   knock - out   call   } (L <   \inf \{S _ {0}, K \})
$$

Then C is a $\mathcal { F } _ { T ^ { - } } \mathrm { m e a s u r a b l e }$ e so-called contingent claim. Assume there exists a self-financing trading strategy $( \phi _ { t } ) _ { 0 \leq t \leq T }$ which generates $C$ i.e. there exists a value process 

$$
V _ {t} = V _ {0} + \int_ {0} ^ {t} \phi_ {s} d S _ {s} \quad 0 \leq t \leq T
$$

with $V _ { T } = C .$ 

If $S _ { t }$ is a martingale, according to Theorem 2.7.3 $V _ { t }$ is a local martingale, and, under suitable conditions on $C$ (see Prop. 2.7.6), a martingale. Hence 

$$
V _ {t} = \operatorname{E} [ V _ {T} | \mathcal {F} _ {t} ] = \operatorname{E} [ C | \mathcal {F} _ {t} ]
$$

is the arbitrage price of $C$ at time t. 

In particular $V _ { 0 } = \mathrm { { E } } [ C ]$ 

Existence of $\left( \phi _ { t } \right)$ : 

If C is square-integrable, i.e. $C \in \mathrm { ~ \cal ~ L ^ { 2 } ~ } ( \mathcal { F } _ { T } , P )$ , by Itˆo’s representation Theorem (see Theorem 2.8.1) there exists an adapted process $( H _ { t } ) _ { 0 \leq t \leq T }$ with 

$$
\operatorname{E} \left[ \int_ {0} ^ {T} H _ {s} ^ {2} d s \right] <   \infty ,
$$

and 

$$
C = \operatorname{E} [ C ] + \int_ {0} ^ {T} H _ {s} d B _ {s}.
$$

$$
\mathrm{Assume} S _ {t} = S _ {0} \exp \left\{\sigma B _ {t} - \frac {1}{2} \sigma^ {2} t \right\} = S _ {0} \cdot \mathcal {E} (\sigma B _ {t}).
$$

$\Longrightarrow S _ { t }$ is $( \mathcal { F } _ { t } )$ -martingale with $d S _ { t } = \sigma ~ S _ { t } ~ d B _ { t }$ 

$$
\Longrightarrow C = \operatorname{E} [ C ] + \int_ {0} ^ {T} H _ {s} d B _ {s} = \underbrace {\operatorname{E} [ C ]} _ {\text { premium }} + \int_ {0} ^ {T} \underbrace {\frac {H _ {s}}{\sigma S _ {s}}} _ {\phi_ {s}} d S _ {s}.
$$

For the call option $C = [ S _ { T } - K ] ^ { + }$ it follows 

$$
\begin{array}{l} \operatorname{E} [ C ] = \int_ {\Omega} [ S _ {T} (\omega) - K ] ^ {+} P (d \omega) = \int_ {[ S _ {T} > K ]} S _ {T} d P - K \cdot P [ S _ {T} > K ] \\ \qquad = S _ {0}   \Phi (g (K)) - K \cdot \Phi (h (K)) \end{array}\tag{22}
$$

with 

$$
g (K) = \frac {\ln (S _ {0} / K)}{\sigma \sqrt {T}} + \frac {1}{2} \sigma \sqrt {T}
$$

$$
h (K) = g (K) - \sigma \sqrt {T}
$$

$$
\varPhi (x) = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {x} e ^ {- \frac {1}{2} z ^ {2}} d z \quad (\mathrm{standardnormaldistribution})
$$

which is the Black-Scholes formula for $r = 0$ 

This is the martingale approach to option pricing. 

Proof. (of equation (22)) 

$$
\begin{array}{l} F (x) = P [ S _ {T} \leq x ] \qquad \text {distribution function of} S _ {T} \\ \qquad = P [ \ln S _ {T} \leq \ln x ] = P \Big [ \ln S _ {0} + \sigma B _ {T} - \frac {1}{2} \sigma^ {2} T \leq \ln x \Big ] \\ \qquad = P \Big [ \sigma B _ {T} \leq \ln x - \ln S _ {0} + \frac {1}{2} \sigma^ {2} T \Big ] \\ \qquad = P \Big [ \frac {B _ {T}}{\sqrt {T}} \leq \underbrace {\frac {\ln (x / S _ {0})}{\sigma \sqrt {T}} + \frac {1}{2} \sigma \sqrt {T}} _ {- h (x)} \Big ] = \varPhi (- h (x)). \end{array}
$$

Hence $K \cdot P [ S _ { T } > K ] = K ( 1 - \varPhi ( - h ( K ) ) = K \cdot \varPhi ( h ( K ) )$ 

$$
\begin{array}{r l} & f (x) = F ^ {\prime} (x) = \varPhi^ {\prime} (- h (x)) \frac {d}{d x} (- h (x)) \\ & \qquad = \varphi (h (x)) \frac {1}{x \sigma \sqrt {T}} = \mathrm{densityof} F (x) \end{array}
$$

$$
\text { with } \quad \varphi (h) = \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {h ^ {2}}{2}} \quad \text { density   of   N(0,1). }
$$

Lemma 2.9.1. $\begin{array} { r } { g = h + \sigma \sqrt { T } \Longrightarrow \varphi ( g ( x ) ) = \varphi ( h ( x ) ) \frac { x } { S _ { 0 } } } \end{array}$ 

(The proof is left for exercise). 

It follows 

$$
\begin{array}{c} \int_ {[ S _ {T} \geq K ]} S _ {T} d P = \int_ {K} ^ {\infty} x f (x) d x = \int_ {K} ^ {\infty} \frac {\varphi (h (x))}{\sigma \sqrt {T}} d x = S _ {0} \int_ {K} ^ {\infty} \frac {\varphi (g (x))}{x \sigma \sqrt {T}} d x \\ = S _ {0} \Big [ - \Phi (g (x)) \Big ] _ {K} ^ {\infty} = S _ {0} \Phi (g (K)). \end{array}
$$

Remark 2.19. The above example illustrates the martingale approach to option pricing. It was pioneered by Harrison-Kreps (1979) and Harrison-Pliska (1981) and has proved as a powerful tool in finance. Whereas the original Black-Scholes approach leads to solving PDE’s under boundary constraints, the martingale technique leads to option prices as expectations under the “martingale measure”. This technique will be developed in detail in Chap. 4. The Feynman-Kac Theorem establishes a relation between these two apparently so diferent approaches (see Sect. 4.3). 

In the above example we have assumed that the security price process $S _ { t }$ is already a martingale. But in general $S _ { t }$ will only be a semimartingale under the given probability measure P. The technique of how to transform $P$ into an “equivalent martingale measure” is developed in Chap. 3. 

## The Girsanov Transformation

The Girsanov transformation is an important tool in mathematical finance. We first give a heuristic introduction taken from Foellmer (1991) (see also Karatzas-Shreve (1988), Sect.3.5). Using only elementary facts of independent normally distributed random variables, it leads to the Dol´eans-Dade exponential as new density under a change of measure for the Brownian motion. 

Sect. 3.2 deals with the Girsanov transformation in general form, as can be found in Revuz-Yor (1991). The proofs are straightforward applications of tools developed in Chap. 2. This section, which at first sight looks rather abstract, is basic for the applications to finance in Chapters 4 and 5, where the general Girsanov transformation is repeatedly used. 

Sect. 3.3 treats the special case of the Brownian motion. 

## 3.1 Heuristic Introduction

Following Foellmer (1991) we first give a heuristic derivation of the Girsanov transformation for the 1-dimensional Brownian motion based on elementary probability concepts. This heuristic will help to understand what happens under the Girsanov transformation. 

Let X be a random variable $\left( \mathrm { r . v . } \right)$ on $( \varOmega , \mathcal { F } , P )$ which is standardnormal, in short $X \sim \mathrm { { N } } ( 0 , 1 )$ 

$$
\Longrightarrow P [ X \leq a ] = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {a} e ^ {- \frac {1}{2} x ^ {2}} d x = \int_ {- \infty} ^ {a} \underbrace {f (x)} _ {n _ {0, 1} (x)} d x
$$

Consider now another density function: 

$$
\widehat {f} (x) = e ^ {(\mu x - \frac {1}{2} \mu^ {2})} f (x).
$$

$$
\Longrightarrow \widehat {P} [ X \leq a ] = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {a} e ^ {- \frac {1}{2} (x - \mu) ^ {2}} d x = \int_ {- \infty} ^ {a} n _ {\mu , 1} (x) d x
$$

$\implies X \sim \mathrm { N } ( \mu , 1 )$ under $\widehat { P }$ 

Observe that the r.v. X has not been changed, but its distribution has changed under the new measure $\widehat { P }$ 

Remark 3.1. Clearly $\widehat { P } _ { X } \sim P _ { X }$ and the Radon-Nikodym derivative is 

$$
\frac {d \widehat {P} _ {X}}{d P _ {X}} (x) = e ^ {(\mu x - \frac {1}{2} \mu^ {2})}.
$$

Under $\widehat { P }$ the ${ \mathrm { r . v . ~ } } { \widehat { X } } = X - \mu$ has now the distribution $\mathrm { { N } } ( 0 , 1 )$ , i.e. 

$$
P _ {X} \equiv \hat {P} _ {\hat {X}}
$$

distribution of X distribution of $\widehat { X }$ 

$$
\mathrm{under} P \equiv \mathrm{under} \widehat {P}
$$

For $X \sim \mathrm { N } ( 0 , \sigma ^ { 2 } )$ under $P$ 

$$
X \sim \mathrm{N} (\mu , \sigma^ {2}) \text {   under   } \widehat {P} (\leftrightarrow \widehat {X} = X - \mu \sim \mathrm{N} (0, \sigma^ {2}) \text {   under   } \widehat {P})
$$

it follows 

$$
\frac {d \widehat {P} _ {X}}{d P _ {X}} (x) = \frac {n _ {\mu , \sigma^ {2}} (x)}{n _ {0 , \sigma^ {2}} (x)} = e ^ {\frac {1}{\sigma^ {2}} (\mu x - \frac {1}{2} \mu^ {2})}.
$$

## Application to Brownian Motion

Let $( B _ { t } ) _ { 0 \leq t \leq 1 }$ be a BM on $( \varOmega , ( \mathcal F ) _ { t } , P )$ 

$\implies B _ { t } \sim \mathrm { N } ( 0 , t )$ under P 

and $\varDelta B _ { t } = B _ { t + \varDelta t } - B _ { t } \sim \mathrm { N } ( 0 , \varDelta t )$ , independent of $B _ { t }$ 

Consider now a BM with drift 

$$
\widehat {B} _ {t} = B _ {t} - \int_ {0} ^ {t} H _ {s} d s
$$

for some stochastic process $( H _ { s } ) _ { 0 \leq s \leq 1 }$ 

Question: Under which measure $\widehat { P }$ is $( \widehat { B } _ { t } )$ again a BM (without drift) ? 

We discretize the unit interval [0, 1] by $t _ { i } = { \frac { i } { n } } \quad ( i = 0 \ldots n )$ It follows 

$$
B _ {\frac {j}{n}} = \sum_ {i = 1} ^ {j} \underbrace {B _ {\frac {i}{n}} - B _ {\frac {i - 1}{n}}} _ {:= X _ {i} \sim \mathrm{N} (0, \Delta t) \text {under} P} \quad j = 1 \ldots n
$$

$\prod _ { i = 1 } ^ { n } \mathrm { N } ( 0 , \varDelta t )$ joint distribution of $X _ { 1 } , \ldots , X _ { n }$ (under P) 

$$
\begin{array}{r l} & {\widehat {X} _ {i} = X _ {i} - \underbrace {H _ {\frac {i - 1}{n}} \cdot \varDelta t} _ {\mu_ {i}}} \\ & {\Longrightarrow \widehat {X} _ {i} \sim \mathrm{N} (0, \varDelta t) \mathrm{under} \widehat {P}} \end{array}
$$

$$
\mathrm{withRadon-Nikodym-derivative} e ^ {\frac {1}{\Delta t} (\mu_ {i} x _ {i} - \frac {1}{2} \mu_ {i} ^ {2})} \mathrm{w.r.t.} P.
$$

Joint distribution of $\widehat { X } _ { i }$ under $\widehat { P }$ 

$$
\begin{array}{l} d \widehat {P} ^ {(n)} = \prod_ {i = 1} ^ {n} \exp \left\{\frac {1}{\Delta t} \left(H _ {\frac {i - 1}{n}} \Delta t \cdot X _ {i} - \frac {1}{2} H _ {\frac {i - 1}{n}} ^ {2} \Delta t ^ {2}\right) \right\} d P ^ {(n)} \\ \qquad = \exp \left\{\sum_ {i = 1} ^ {n} H _ {\frac {i - 1}{n}} (B _ {\frac {i}{n}} - B _ {\frac {i - 1}{n}}) - \frac {1}{2} \sum_ {i = 1} ^ {n} H _ {\frac {i - 1}{n}} ^ {2} \Delta t \right\} d P ^ {(n)} \\ \text {"} \xrightarrow [ n \to \infty ]{} \text {"} \exp \left\{\int_ {0} ^ {1} H _ {s}   d B _ {s} - \frac {1}{2} \int_ {0} ^ {1} H _ {s} ^ {2}   d s \right\} d P \\ \implies \boxed { \begin{array}{c} \widehat {P} = \mathcal {E} (L _ {1})   P \quad \text {with} L _ {1} = \int_ {0} ^ {1} H _ {s}   d B _ {s} \\ = \exp \{L _ {1} - \frac {1}{2}   \langle L _ {1} \rangle \} \cdot P \\ \end{array} } \end{array}\tag{1}
$$

Remark 3.2. $\begin{array} { r } { \mathcal { E } ( L _ { 1 } ) = \exp \{ L _ { 1 } - \frac { 1 } { 2 } \left. L _ { 1 } \right. \} } \end{array}$ is called the “stochastic exponential” or the “Dol´eans-Dade” exponential. 

The limit process (1) is of course only a heuristic argument. A mathematically rigorous derivation follows in Sect. 3.2 and 3.3. 

## 3.2 The General Girsanov Transformation

Let $( \varOmega , ( \mathcal F _ { t } ) _ { 0 \leq t } , P )$ satisfy the usual conditions, i.e. the filtration is right continuous, complete and $\mathcal { F } _ { \infty } = \sigma ( \bigcup _ { t } \mathcal { F } _ { t } )$ 

$\mathcal { M } _ { \mathrm { l o c } } ^ { ( c ) } ( P ) : = \mathrm { a l l }$ (continuous) local martingales w.r.t. P 

Definition 3.2.1. X is called P-semimartingale $\Longleftrightarrow X = M + A$ 

with $M \in \mathcal { M } _ { \mathrm { l o c } } ( P )$ and $A \in \operatorname { F V }$ 

Let Q be another probability measure on $( \varOmega , \mathcal { F } _ { \infty } )$ 

Definition 3.2.2. 

$$
(i) Q <   <   P \underset {\text { Def. }} {\Longleftrightarrow} P [ A ] = 0 \Longrightarrow Q [ A ] = 0 \quad \forall A \in \mathcal {F} _ {\infty}
$$

(ii) $Q \sim P { \{ \underset { \mathrm { D e f . } } { \Longleftrightarrow } } Q < < P $ and $P < < Q$ 

(i.e. Q and P have identical null sets) 

Proposition 3.2.3. (Radon-Nikodym) 

Let $Q < < P$ . Then there exists $Z \in L ^ { 1 } ( \varOmega , \mathcal { F } _ { \infty } )$ with $Q = Z P , i . e .$ 

$$
Q [ A ] = \int_ {A} Z (\omega) P (d \omega) \quad \forall A \in \mathcal {F} _ {\infty}
$$

Notation: $Z = { \frac { d Q } { d P } }$ 

$$
\Longrightarrow Z _ {t} = \mathrm{E} _ {P} [ Z | \mathcal {F} _ {t} ] = \mathrm{E} _ {P} \left[ \frac {d Q}{d P} | \mathcal {F} _ {t} \right]
$$

is a right continuous martingale, $\mathrm { E } _ { P } [ Z _ { t } ] \equiv 1$ . Furthermore 

(i) $Z _ { t } ( \omega ) > 0 \quad Q \mathrm { - a . s . }$ 

(ii) $Z _ { t } = { \frac { d Q _ { t } } { d P _ { t } } } \quad { \mathrm { ~ o n ~ } } { \mathcal { F } } _ { t }$ 

Lemma 3.2.4. Let $Q \sim P$ . Then one has 

$$
X \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (Q) \longleftrightarrow X Z \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (P).
$$

Proof. Let $s < t \ , \ A \in \mathcal { F } _ { s }$ . Is X a martingale, then obviously 

$$
\mathrm{E} _ {Q} [ X _ {s}; A ] = \mathrm{E} _ {Q} [ X _ {t}; A ] \Longleftrightarrow \mathrm{E} _ {P} [ X _ {s} Z _ {s}; A ] = \mathrm{E} _ {P} [ X _ {t} Z _ {t}; A ].\tag{2}
$$

Let $T _ { n } \uparrow \infty$ be a localizing stopping time for X. It follows 

$$
Q = Z _ {T _ {n}} P \text {   on   } \mathcal {F} _ {T _ {n}} \Longrightarrow (2) \text {   for   } X _ {T _ {n}}, X _ {T _ {n}} Z _ {T _ {n}}
$$

Notation: Following Protter (1990) we use the following short notation for stochastic integrals: $\begin{array} { r } { H \bullet X = \int } \end{array}$ HdX. Evaluating these processes at t, we have 

$$
H \bullet X _ {t} = \int_ {0} ^ {t} H _ {s} d X _ {s} = H _ {0} X _ {0} + \int_ {(0, t ]} H _ {s} d X _ {s}
$$

Theorem 3.2.5. (Girsanov) 

Let $Q < < P$ with $Z = { \frac { d Q } { d P } }$ continuous. 

It follows 

$$
M \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (P) \Longrightarrow \widetilde {M} = M - Z ^ {- 1} \bullet \langle M, Z \rangle \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (Q)
$$

$$
\mathrm{(i.e.} \quad \widetilde {M _ {t}} = M _ {t} - \int_ {0} ^ {t} \frac {1}{Z _ {s}} d \langle M, Z \rangle_ {s}).
$$

Proof. According to Lemma 3.2.4 one has to show: $\widetilde { M } Z \in \mathcal { M } _ { \mathrm { l o c } } ^ { c } ( P )$ 

$$
\begin{array}{l} \widetilde {M} _ {t} Z _ {t} = \widetilde {M} _ {0} Z _ {0} + \int_ {0} ^ {t} \widetilde {M} _ {s} d Z _ {s} + \int_ {0} ^ {t} Z _ {s} d \widetilde {M} _ {s} + \langle \widetilde {M}, Z \rangle_ {t} \\ = \widetilde {M} _ {0} Z _ {0} + \underbrace {\int_ {0} ^ {t} \widetilde {M} _ {s} d Z _ {s}} _ {\in \mathcal {M} _ {\mathrm{loc}} (P)} + \underbrace {\int_ {0} ^ {t} Z _ {s} d M _ {s}} _ {\in \mathcal {M} _ {\mathrm{loc}} (P)} \underbrace {- \langle M , Z \rangle_ {t} + \langle \widetilde {M} , Z \rangle_ {t}} _ {= 0 \text {since} \widetilde {M} - M \in \mathrm{FV}} \end{array}
$$

 

Let now $Q \sim P$ 

$$
Q <   <   P \longrightarrow Z = \frac {d Q}{d P} > 0 \quad Q \mathrm{-a.s.}
$$

$P < < Q \longrightarrow Z$ also $P \mathrm { - a . s }$ . strictly positive 

Lemma 3.2.6. Any strictly positive process $\left( Z _ { t } \right)$ can be represented as 

$$
Z _ {t} = \exp \left\{L _ {t} - \frac {1}{2} \left<   L \right> _ {t} \right\} = \mathcal {E} (L) _ {t}
$$

with 

$$
L _ {t} = \log Z _ {0} + \int_ {0} ^ {t} Z _ {s} ^ {- 1} d Z _ {s}.
$$

Proof. 

$$
\text {It} \hat {\mathrm{o}} \implies \log Z _ {t} = \underbrace {\log Z _ {0} + \int_ {0} ^ {t} Z _ {s} ^ {- 1} d Z _ {s}} _ {L _ {t}} - \frac {1}{2} \underbrace {\int_ {0} ^ {t} Z _ {s} ^ {- 2} d \langle Z \rangle_ {s}} _ {\langle L \rangle_ {t}},
$$

since by Corollary 2.2.11 

$$
M _ {t} = \int_ {0} ^ {t} f (X _ {s}) d X _ {s} \Longrightarrow \langle M \rangle_ {t} = \int_ {0} ^ {t} f ^ {2} (X _ {s}) d \langle X \rangle_ {s}.
$$

 

Proposition 3.2.7. (Girsanov for $Q \sim P )$ : Let $Q = { \mathcal { E } } ( L ) \cdot P$ . Then one has 

$$
M \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (P) \Longleftrightarrow \widetilde {M} = M - \langle M, L \rangle \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (Q)
$$

and $P = \mathcal { E } ( - \widetilde { L } ) \cdot Q$ 

Proof. $\widetilde { M } = M - Z ^ { - 1 } \bullet \langle M , Z \rangle \in { \mathcal { M } } _ { \mathrm { l o c } } ^ { c } ( Q ) ( { \mathrm { G i r s a n o v } } )$ , and 

$$
L _ {t} = \log Z _ {0} + \int_ {0} ^ {t} \frac {1}{Z _ {s}} d Z _ {s}, \text { i.e. } L = Z ^ {- 1} \bullet Z. \text { Thus }
$$

$$
\begin{array}{c} \langle M, L \rangle_ {t} = \langle M, Z ^ {- 1} \bullet Z \rangle_ {t} = \int_ {0} ^ {t} Z _ {s} ^ {- 1} d \langle M, Z \rangle_ {s} = (Z ^ {- 1} \bullet \langle M, Z \rangle) _ {t} \\ \uparrow \\ \text {computational rule for} \langle X, Y \rangle . \end{array}
$$

$$
\begin{array}{l} L \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (P) \longrightarrow - \widetilde {L} = - L + \underbrace {\langle L , L \rangle} _ {= \langle L \rangle} \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (Q) \\ P = \mathcal {E} (L) ^ {- 1} \cdot Q \\ \mathcal {E} (L) _ {t} ^ {- 1} = \exp \left\{- L _ {t} + \frac {1}{2}   \langle L \rangle_ {t} \right\} = \exp \left\{- \widetilde {L} _ {t} - \frac {1}{2}   \underbrace {\langle L \rangle_ {t}} _ {= \langle \widetilde {L} \rangle_ {t}} \right\} = \mathcal {E} (- \widetilde {L}) _ {t}. \end{array}
$$

Conversely one has 

$$
\begin{array}{c} \widetilde {M} \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (Q) \longrightarrow \widetilde {\widetilde {M}} = \widetilde {M} - \langle \widetilde {M}, - \widetilde {L} \rangle \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (P) \\ = \widetilde {M} + \underbrace {\langle \widetilde {M} , \widetilde {L} \rangle} _ {\langle M, L \rangle} = M. \end{array}
$$

Computational rule for covariation of stochastic integrals: (see Protter (1990) , Theorem29, p.68) 

Proposition 3.2.8. $X , Y$ continuous semimartingales, 

H, K admissible integrands $( w . r . t . \ X , Y )$ 

Then one has 

$$
\langle H \bullet X, K \bullet Y \rangle_ {t} = \int_ {0} ^ {t} H _ {s} K _ {s} d \langle X, Y \rangle_ {s}.
$$

Remark 3.3. $X = M + A \quad Y = N + B \quad M , N \in \mathcal { M } _ { \mathrm { l o c } } ^ { ( c ) }$ 

$$
\Longrightarrow \langle X, Y \rangle = \langle M, N \rangle
$$

In particular, it follows: 

$$
\langle H \bullet M, N \rangle_ {t} = \int_ {0} ^ {t} H _ {s} d \langle M, N \rangle_ {s}
$$

and 

$$
\langle M \rangle = \left\langle \int_ {0} ^ {t} f (X) d X _ {s} \right\rangle = \langle f (X) \bullet X, f (X) \bullet X \rangle_ {t} = \int_ {0} ^ {t} f ^ {2} (X _ {s}) d \langle X \rangle_ {s}.
$$

## 3.3 Application to Brownian Motion

Girsanov solves the following problem: 

$$
\text { Given }: \left. \begin{array}{c} X \in \mathcal {M} _ {\mathrm{loc}} (P) \\ Q \sim P \end{array} \right\} \underset {\text { Girsanov }} {\Longrightarrow} \widetilde {X} \in \mathcal {M} _ {\mathrm{loc}} (Q)
$$

We now consider the inverse problem: 

Given a semimartigale X = M +A w.r.t. P, i.e. $M \in \mathcal { M } _ { \mathrm { l o c } } ( P ) , A \in \mathrm { F V }$ 

$$
\exists Q \sim P: \quad X \in \mathcal {M} _ {\mathrm{loc}} (Q) \ref {e q : 1 . 2}
$$

I.e., we are looking for a P-equivalent measure $Q$ under which X is a martingale (so-called equivalent martingale measure). 

Approach: Q = (L) P 

$$
\begin{array}{l} Q = \mathcal {E} (L) \cdot P \\ \operatorname{Girsanov} \Longrightarrow \widetilde {M} = M - \langle M, L \rangle \in \mathcal {M} _ {\mathrm{loc}} (Q) \\ \widetilde {M} = X \Longleftrightarrow A = - \langle M, L \rangle . \end{array}
$$

However, there are two problems: 

1) Determination of L 

2) Under what conditions is $Q = { \mathcal { E } } ( L ) \cdot P$ a probability measure $? ?$ ad 2: 

$$
\begin{array}{r l} {Q \mathrm{prob.measure} \longleftrightarrow \mathrm{E} _ {P} [ \mathcal {E} (L) _ {t} ] \equiv 1} \\ & {\longleftrightarrow \mathcal {E} (L) _ {t} \mathrm{isarmtingale(since} L _ {0} = 0).} \end{array}\tag{3}
$$

A suficient condition for $\mathcal { E } ( L ) _ { t }$ to be a martingale is the so-called Novikov condition (see e.g. Revuz-Yor (1991), p.308): 

$$
\operatorname{E} \Big [ \exp \{\frac {1}{2} \langle L \rangle_ {t} \} \Big ] <   \infty \quad \forall t.\tag{4}
$$

ad 1: Solution for semimartingales of Brownian motion 

$$
X _ {t} = B _ {t} + \underbrace {\int_ {0} ^ {t} H _ {s} d s} _ {\mathrm{Drift} = A}
$$

with $( B _ { t } ) _ { 0 \leq t \leq T }$ Brownian motion w.r.t. P and $H _ { t } ( \omega )$ adapted, c`adl`ag (e.g. $H _ { t } = f ( B _ { s } ; s \le t ) )$ 

Claim: $L _ { t } = - \intop _ { 0 } ^ { t } H _ { s } \mathrm { ~ } d B _ { s }$ solves the problem. 

Proof. 

$$
- \langle B, L \rangle_ {t} = \langle B, H \bullet B \rangle_ {t} = \int_ {0} ^ {t} H _ {s} d \langle B \rangle_ {s} = \int_ {0} ^ {t} H _ {s} d s = A
$$

$$
\Longrightarrow X _ {t} \in \mathcal {M} _ {\mathrm{loc}} (Q) \text {   for   } Q = \mathcal {E} (L) \cdot P.
$$

 

Furthermore it follows 

$$
\langle X \rangle_ {t} = \langle B \rangle_ {t} = t <   \infty \Longrightarrow (X _ {t}) L ^ {2} \text {-martingale}.
$$

It even follows: $( X _ { t } )$ is a Brownian motion w.r.t. Q ! This follows from L´evy’s theorem: 

$$
(X _ {t}) \in \mathcal {M} _ {\mathrm{loc}} ^ {c} (P), \langle X \rangle_ {t} = t \forall t \geq 0 \quad P \text {-a.s.} \Longrightarrow (X _ {t}) \text { is   B.M.   w.r.t. } P.
$$

Example of a non-continuous local martingale with $\langle X \rangle _ { t } = t \colon$ 

$X _ { t }$ Poisson-Process (with parameter λ); i.e. 

$$
P [ X _ {t} = K ] = e ^ {- \lambda t} \frac {(\lambda t) ^ {K}}{K !}, E [ X _ {t} ] = \lambda t = \mathrm{Var} (X _ {t})
$$

$$
\Longrightarrow M _ {t} = X _ {t} - \lambda t \mathrm{martingaleand} M _ {t} ^ {2} - \lambda t \mathrm{martingale}
$$

$$
\Longrightarrow \langle M \rangle_ {t} = \lambda t
$$

Thus for $\lambda = 1 , M _ { t }$ is a martingale with $\langle M \rangle _ { t } = t$ , but not continuous. 

## Same procedure for d-dimensional Brownian motion:

Let $B _ { t } = ( B _ { t } ^ { 1 } , \ldots , B _ { t } ^ { d } )$ be d-dimensional Brownian motion, i.e. $( B _ { t } ^ { i } )$ $( i = 1 , \ldots , d )$ are independent one-dimensional Brownian motions. 

Proposition 3.3.1. $\left( \mathrm { L e v y } \right)$ For an $( \mathcal { F } _ { t } )$ -adapted continuous d-dimensional process $X _ { t } = ( X _ { t } ^ { 1 } , \ldots , X _ { t } ^ { d } )$ with $X _ { 0 } = 0$ the following statements are equivalent: 

(i) X is a Brownian motion w.r.t. $( \mathcal { F } _ { t } )$ 

(ii) X is a continuous local martingale mit $\langle X ^ { i } , X ^ { j } \rangle _ { t } = \delta _ { i j } \cdot t$ 

$$
\forall i, j = 1 \dots d.
$$

Proof. see Revuz-Yor (1991), p.141 . 

 

Proposition 3.3.2. (Girsanov for d-dimensional Brownian motion) 

Let $X _ { t } = B _ { t } + \intop _ { 0 } ^ { t } H _ { s }$ ds be a d-dimensional process with 

$$
\mathrm{E} \bigg [ \exp \left\{\frac {1}{2} \int_ {0} ^ {T} | | H _ {s} | | ^ {2} d s \right\} \bigg ] <   \infty
$$

(Novikov condition). 

(5) 

Define Q as $\frac { d Q } { d P } = \mathcal { E } \Big ( - \intop _ { 0 } ^ { T } H _ { s } \mathrm { ~ } d B _ { s } \Big )$ 

Then under $Q \left( X _ { t } \right)$ is a d-dimensional Brownian motion for $0 \leq t \leq T$ 

# Application to Financial Economics

In this chapter the methods developed in Chapter 2 and 3 are applied to derive the fundamentals of “financial economics” in continuous time, such as the market price of risk, the no-arbitrage principle, the fundamental pricing rule and its invariance under numeraire changes, and the forward measure, a useful tool to deal with stochastic interest rates. Special emphasis is laid on the economic interpretation of the so-called “risk-neutral” arbitrage measure and its relation to the “real world” measure considered in general equilibrium theory, a topic sometimes leading to confusion between economists and financial engineers. 

Using the general Girsanov transformation, as developed in Sect. 3.2, the rather intricate problem of the change of numeraire can be treated in a rigorous manner, and the so-called “two-country” or “Siegel” paradox serves as an illustration. The section on Feynman-Kac relates the martingale approach used explicitly in these notes to the more classical approach based on partial diferential equations. 

## 4.1 The Market Price of Risk and Risk-neutral Valuation

We consider an economy depending on d independent stochastic factors modelled by a d-dimensional Brownian motion $B _ { t } = ( B _ { t } ^ { 1 } , \ldots , B _ { t } ^ { d } )$ on the filtered probability space $( \varOmega , ( \mathcal F _ { t } ) _ { 0 \leq t \leq T } , P )$ 

Let X be a security with returns 

$$
\frac {d X _ {t}}{X _ {t}} = \mu_ {X} (t) d t + \underbrace {\sigma_ {X} (t) \circ d B _ {t}} _ {\text { scalar   product   in } \mathbb {R} ^ {d}} 0 \leq t \leq T\tag{1}
$$

where $\mu _ { X } ( t ) , \sigma _ { X } ( t ) = ( \sigma _ { X } ^ { 1 } , . . . , \sigma _ { X } ^ { d } )$ are adapted processes on $( \varOmega , ( \var F _ { t } ) , P )$ 

We assume that there exists a Lebesgue-integrable real function $\phi _ { X } ( t )$ on $[ 0 , T ]$ , such that $| \mu _ { X } ( t , \omega ) | \leq \phi _ { X } ( t )$ and $| | \sigma _ { X } ( t , \omega ) | | ^ { 2 } \leq \phi _ { X } ( t )$ P-a.s. 

Remark 4.1. A process of the form $( 1 )$ is a (positive) Itˆo-process. Every strictly positive difusion process $X _ { t }$ can be written as an Itˆoprocess by taking its logarithm (compare Lemma 3.2.6). 

Furthermore we consider the following processes: 

$r ( t ) = r ( t , \omega )$ an adapted and bounded process of the “spot” interest rate, 

$$
\beta (t) = \beta (t, \omega) = \exp \int_ {0} ^ {t} r (s, \omega) d s \text { the   accumulation   process }.
$$

$\beta ( t )$ is the “savings” account by rolling over one monetary unit at the prevailing spot rate. Clearly, $\beta ( t )$ is an adapted continuous process of finite variation. 

Definition 4.1.1. Let $\lambda ( t ) = ( \lambda ^ { 1 } , \ldots , \lambda ^ { d } ) _ { t }$ be an adapted process with 

$$
\begin{array}{c} \mu_ {X} (t) = r (t) + \lambda (t) \circ \sigma_ {X} (t) \\ = r (t) + \sum_ {i = 1} ^ {d} \lambda^ {i} (t)   \sigma_ {X} ^ {i} (t). \end{array}\tag{2}
$$

Then $\lambda ( t )$ is called the process of the “market price of risk” and $\lambda ^ { i } ( t )$ the price of the i-th risk-factor . 

## Remark 4.2. For $d = 1$ the relation $( { \mathcal { Q } } )$ can be written as

$$
\frac {\operatorname{E} \left[ \frac {d X _ {t}}{X _ {t}} | \mathcal {F} _ {t} \right] - r (t) d t}{\sqrt {\operatorname{Var} \left(\frac {d X _ {t}}{X _ {t}} | \mathcal {F} _ {t}\right)}} = \lambda (t) d t
$$

which can be interpreted as the (expected) excess return per risk unit. 

Let now Y be another security with 

$$
\frac {d Y _ {t}}{Y _ {t}} = \mu_ {Y} (t) d t + \sigma_ {Y} (t) \circ d B _ {t}.
$$

Let $\lambda _ { X } ( t )$ and $\lambda _ { Y } ( t )$ be the corresponding risk price processes of $X$ and $Y$ 

We assume that the underlying economy is in an equilibrium state, i.e. all price processes $X ( t ) , \ Y ( t ) , \ r ( t )$ etc. are determined by supply and demand of the agents in this economy. In order to determine such an equilibrium one would have to know the consumption and investment behavior of each agent depending on his initial endowment, preferences over consumption streams, expectations and attitude towards risk, a formidable task. The power of financial economics consists in working with a much weaker condition, which certainly is necessary for an economy to be in equilibrium, namely the condition of $^ { 6 6 } \mathrm { N o }$ arbitrage”, i.e. the absence of arbitrage profits without taking risks. Such an arbitrage opportunity would exist if, at any time t and any state $\omega ,$ one could form a riskless portfolio which has a higher return than the riskless interest rate $r ( t , \omega )$ . By “No arbitrage” we mean that such an arbitrage opportunity does not exist. 

The fundamental consequence of the above assumption is the following theorem: 

Theorem 4.1.2. “No arbitrage” implies 

$$
\lambda_ {X} (t, \omega) = \lambda_ {Y} (t, \omega) \quad f o r a l l (t, \omega) \in [ 0, T) \times \Omega .
$$

Proof. We give a proof for $d = 1$ (for d > 1 see Ingersoll (1987)). 

Assume there exists $( t , \omega )$ with $\lambda _ { X } ( t , \omega ) > \lambda _ { Y } ( t , \omega )$ . We may assume that $0 < \sigma _ { X } ( t , \omega ) < \sigma _ { Y } ( t , \omega )$ (otherwise replace $\phi$ by $- \phi$ in the following definition of $\phi )$ . 

Choose at time t the following portfolio of X and $Y$ : 

$$
\phi_ {X} = \frac {\sigma_ {Y}}{(\sigma_ {Y} - \sigma_ {X}) \cdot X _ {t}}, \phi_ {Y} = - \frac {\sigma_ {X}}{(\sigma_ {Y} - \sigma_ {X}) \cdot Y _ {t}}.
$$

The value of this portfolio is 

$$
V _ {t} (\phi) = \phi_ {X} X _ {t} + \phi_ {Y} Y _ {t} = 1
$$

and its return 

$$
\begin{array}{l} d V _ {t} = \phi_ {X} d X _ {t} + \phi_ {Y} d Y _ {t} \\ = \underbrace {\frac {1}{\sigma_ {Y} - \sigma_ {X}} \left[ \left(\sigma_ {Y} \mu_ {X} - \sigma_ {X} \mu_ {Y}\right) d t + \underbrace {\left(\sigma_ {Y} \sigma_ {X} - \sigma_ {X} \sigma_ {Y}\right) d B _ {t}} _ {\equiv 0} \right]} _ {\mu_ {V}} \end{array}
$$

Hence $V _ { t }$ has a riskless return 

$$
\begin{array}{c} \mu_ {V} = \frac {1}{\sigma_ {Y} - \sigma_ {X}} \Big [ \sigma_ {Y} (r _ {t} + \lambda_ {X} \sigma_ {X}) - \sigma_ {X} (r _ {t} + \lambda_ {Y} \sigma_ {Y}) \Big ] \\ = r _ {t} + \underbrace {\frac {\sigma_ {Y} \cdot \sigma_ {X}}{\sigma_ {Y} - \sigma_ {X}}} _ {> 0} (\underbrace {\lambda_ {X} - \lambda_ {Y}} _ {> 0}) > r _ {t} \end{array}
$$

which is in contradiction to the “No arbitrage” condition. 

Question: When is the process λ(t) P-a.s. uniquely determined $\it { ? }$ 

Assume there exist n securities $X ^ { 1 } , \ldots , X ^ { n }$ with 

$$
\sum (t) = \left( \begin{array}{c} \sigma_ {X _ {1}} (t) \\ . \\ . \\ . \\ \sigma_ {X _ {n}} (t) \end{array} \right) \quad (n \times d) \text {-matrix of volatilities}
$$

and 

$$
\mu (t) = \left( \begin{array}{c} \mu_ {X _ {1}} (t) \\ . \\ . \\ . \\ \mu_ {X _ {n}} (t) \end{array} \right), e = \left( \begin{array}{c} 1 \\ . \\ . \\ . \\ 1 \end{array} \right).
$$

No arbitrage implies 

$$
\mu (t) = r (t) \cdot e + \sum (t) \circ \lambda (t).
$$

Hence $\lambda ( t , \omega )$ is uniquely determined if and only if the stochastic matrix $\sum ( t , \omega )$ has full rank $d ,$ for all t, P-a.s. 

Clearly a necessary condition is $n \geq d ,$ , i.e. there must be at least as many securities as stochastic factors in the economy. A suficient condition for $d = 1$ is $\sigma _ { X } ( t , \omega ) > 0$ for all $t , \omega$ 

## Elimination of λ(t) by means of Girsanov:

Assume that the Novikov condition 

$$
\mathrm{E} \Big [ \exp \{\frac {1}{2} \int_ {0} ^ {T} | | \lambda (s) | | ^ {2} d s \} \Big ] <   \infty\tag{3}
$$

is fulfilled. Define 

$$
\begin{array}{l} L _ {t} = - \int_ {0} ^ {t} \lambda (s) \circ d B _ {s} \quad 0 \leq t \leq T \\ P ^ {*} = \mathcal {E} (L) \cdot P \quad , P ^ {*} \sim P. \end{array}
$$

Then the Girsanov theorem implies for each security price process $X _ { t }$ : 

$$
\begin{array}{r l} & {\frac {d X _ {t}}{X _ {t}} = \mu_ {X} (t) d t + \sigma_ {X} (t) d B _ {t} = r (t) d t + \sigma_ {X} (t) (d B _ {t} + \lambda (t) d t)} \\ & {\qquad = r (t) d t + \sigma_ {X} (t) d B _ {t} ^ {*}} \end{array}
$$

and $B _ { t } ^ { * }$ is a d-dimensional Brownian motion under $P ^ { * }$ 

## Remark 4.3. Clearly $P ^ { * }$ is unique if $\lambda ( t )$ is unique.

## Interpretation of P and $P ^ { * }$ :

We can interpret the original measure P as the (objective) ”real-world” measure or, in the equilibrium interpretation, as the (subjective) expectation of the “representative investor”. For the equilibrium price process $X _ { t }$ with respect to $P$ one has 

$$
\mathrm{E} _ {P} \left[ \frac {d X}{X} | \mathcal {F} _ {t} \right] = r (t) d t + \lambda (t) \sigma_ {X} (t) d t (\textbf {u n d e r} P)\tag{4}
$$

with λ(t) := market price of risk (varies with P !). 

The measure $P ^ { * }$ can be interpreted as the expectation of a risk-neutral investor, since 

$$
\mathrm{E} _ {P ^ {*}} \left[ \frac {d X}{X} | \mathcal {F} _ {t} \right] = r (t) d t + \text { zero - premium } (\text { under } P ^ {*}).\tag{5}
$$

The relation (5) has been called by Cox-Ingersoll-Ross (1981) the $^ { 6 6 } \mathrm { L o - }$ cal Expectation Hypothesis”, a terminology which has led to some confusion. Note that the equilibrium process has not been changed, it is the same under both measures $P$ and $P ^ { * }$ . Girsanov’s Theorem allows us to replace the relation (4) through the equivalent simpler relation (5). In particular, no assumption has been made about the existence of risk-neutral investors. In a real economy neither $\mathrm { a }$ “representative” nor a “risk-neutral” investor will exist, since both assumptions would prevent the existence of a (stable) equilibrium. The great advantage of the representation (5) under the (martingale) measure $P ^ { * }$ is that we do not have to know anything about the individual expectations $P$ and the investors’ attitude towards risk. 

In summary: $X _ { t }$ has not been changed. It is the same equilibrium price process as under $P ,$ , but in simpler representation under $P ^ { * } , P ^ { * }$ is called the “equivalent risk-neutral measure” or the $^ { 6 6 } P .$ -equivalent martingale measure”. 

## 4.2 The Fundamental Pricing Rule

Let $Z _ { t } > 0$ be the price process of an arbitrary security without dividend payments in $[ 0 , T ]$ with dynamics 

$$
\frac {d Z _ {t}}{Z _ {t}} = \mu_ {Z} (t) d t + \sigma_ {Z} (t) \circ d B _ {t} \quad (\text { Itô - process   under } P).
$$

with $\mu _ { Z } ( t ) , \ \sigma _ { Z } ( t )$ adapted processes as defined in Sect. 4.1 . 

Remark 4.4. Any strictly positive semimartingale of the Brownian motion can be written as an Itˆo-process (see Lemma 3.2.6). 

Theorem 4.2.1. The discounted process 

$$
\widehat {Z} _ {t} = \exp \left\{- \int_ {0} ^ {t} r (s) d s \right\} Z _ {t} = \frac {Z _ {t}}{\beta_ {t}}
$$

is $a$ martingale under the risk-neutral measure $P ^ { * }$ 

Proof. Under $P ^ { * }$ one has $\frac { d Z _ { t } } { Z _ { t } } = r ( t ) d t + \sigma _ { Z } ( t ) d B _ { t } ^ { * }$ 

By Itˆo it follows $d \widehat { Z } _ { t } = \widehat { Z } _ { t } \sigma _ { Z } ( t ) d B _ { t } ^ { * }$ , hence $\widehat { Z } _ { t }$ is a local martingale under $P ^ { * }$ , with solution $\widehat { Z } _ { t } = Z _ { 0 } \cdot \mathcal { E } ( N _ { t } )$ where $\begin{array} { r } { N _ { t } = \underset { 0 } { \overset { t } { \mathop { \left/ { \vphantom { \operatorname* { d e m } } } \right. } } } | | \sigma _ { Z } ( s ) | | ^ { 2 } d B _ { s } } \end{array}$ 

But $\begin{array} { r } { \langle N \rangle _ { t } = \int \displaystyle \operatorname* { l } _ { 0 } ^ { t } | | \sigma _ { Z } ( s ) | | ^ { 2 } d s \leq \displaystyle \int \displaylimits _ { 0 } ^ { t } \phi _ { Z } ( s ) d s < \infty \ P ^ { * } \mathrm { - a . s . } } \end{array}$ , which implies: 

$$
\mathrm{E} ^ {*} \Big [ \exp \{\frac {1}{2} \langle N \rangle_ {t} \} \Big ] \leq \exp \{\frac {1}{2} \int_ {0} ^ {t} \phi_ {Z} (s) d s \} <   \infty \quad \forall t
$$

and the Novikov condition (see Sect. 3.3 (4)) is satisfied. Hence $\widehat { Z } _ { t }$ is a martingale under $P ^ { * }$ □ 

Theorem 4.2.2. (Fundamental Pricing Rule) 

$$
\begin{array}{r l} & Z _ {t} = \mathrm{E} ^ {*} \bigg [ \exp \Big \{- \int_ {t} ^ {T} r (s) d s \Big \} \cdot Z _ {T} | \mathcal {F} _ {t} \bigg ] 0 \leq t \leq T \\ & \quad = \mathrm{E} ^ {*} \Big [ \frac {\beta_ {t}}{\beta_ {T}} Z _ {T} | \mathcal {F} _ {t} \Big ]. \end{array}
$$

Proof. Since $\widehat { Z } _ { T }$ is a $P ^ { * }$ - martingale, it follows: 

$$
\widehat {Z} _ {t} = \mathrm{E} ^ {*} [ \widehat {Z} _ {T} \mid \mathcal {F} _ {t} ] = \mathrm{E} ^ {*} \left[ \exp \left\{- \int_ {0} ^ {T} r (s) d s \right\} Z _ {T} \mid \mathcal {F} _ {t} \right]
$$

$$
Z _ {t} = \mathrm{E} ^ {*} [ \beta_ {t} \widehat {Z} _ {T} | \mathcal {F} _ {t} ] = \mathrm{E} ^ {*} \Bigl [ \frac {\beta_ {t}}{\beta_ {T}} Z _ {T} | \mathcal {F} _ {t} \Bigr ].
$$

□ 

## Examples:

1. $Z _ { t } = P _ { t } ( T )$ zero-bond with maturity T, i.e. $P _ { T } ( T ) = 1$ 

$$
\Longrightarrow P _ {t} (T) = \mathrm{E} ^ {*} \left[ \exp \left\{- \int_ {t} ^ {T} r (s) d s \right\} \mid \mathcal {F} _ {t} \right]
$$

2. $Z _ { t } = ( X _ { T } - K ) ^ { + }$ call option on security X 

$$
\Longrightarrow Z _ {t} = \mathrm{E} ^ {*} \left[ \exp \left\{- \int_ {t} ^ {T} r (s) d s \right\} \left(X _ {T} - K\right) ^ {+} \mid \mathcal {F} _ {t} \right]
$$

special case: $d = 1 \ , \ r ( t , \omega ) \equiv r , \ \sigma _ { Z } ( t , \omega ) \equiv \sigma$ 

$$
\begin{array}{l} \Longrightarrow Z _ {t} = X _ {t} \cdot \Phi (d _ {1}) - K \cdot \exp \{- (\underbrace {T - t} _ {s}) \cdot r \}   \Phi (d _ {2}) \\ \text {with} d _ {1, 2} = \frac {\ln (X _ {t} / K \cdot e ^ {- r s})}{\sigma \sqrt {s}} \pm \frac {1}{2}   \sigma \sqrt {s} \quad \text {(Black - Scholes - formula)}  . \end{array}
$$

The proof can be given as exercise (or see Sect. 2.9). 

Hint: $B ^ { * }$ is a Brownian motion under $P ^ { * }$ , i.e. 

$$
\begin{array}{c} P ^ {*} [ B _ {T} ^ {*} \leq x ] = \Phi \Big (\frac {x}{\sqrt {T}} \Big) \Longleftrightarrow B _ {T} ^ {*} \sim \mathrm{N} (0, T) \quad \text { under } P ^ {*} \\ \Longleftrightarrow \frac {B _ {T} ^ {*}}{\sqrt {T}} \sim \mathrm{N} (0, 1). \end{array}
$$

## Dividend paying securities

Let $Z ( t )$ be the price process of a security with continuous dividend payments given by the dividend rate $d _ { Z } ( t )$ which is proportional to $Z ( t ) . ^ { 1 }$ Assume that the dynamics of the (ex dividend) process is given by 

$$
\frac {d Z _ {t}}{Z _ {t}} = \mu_ {Z} (t) d t + \sigma_ {Z} (t) \circ d B _ {t} \quad (\mathrm{ex-dividendprocess})\tag{6}
$$

Let $\widetilde Z ( t )$ denote the process with accumulated dividends, i.e. 

$$
\frac {d \widetilde {Z} _ {t}}{\widetilde {Z} _ {t}} = (\underbrace {\mu_ {Z} (t) + d _ {Z} (t)} _ {\mu_ {\widetilde {Z}} (t)}) d t + \sigma_ {Z} (t) \circ d B _ {t} \quad (\text { cum - dividend   process }) \tag {7}
$$

Denote by $\xi ( t ) = { { e x p } \{ \intop _ { 0 } ^ { t } { d _ { Z } ( s ) d s } \} }$ the accumulated dividend process. One easily checks that $\widetilde { Z } _ { t } = \xi ( t ) \cdot Z ( t )$ is a solution of $( 7 )$ . Since $\widetilde { Z } _ { t }$ does not pay dividends, the Fundamental Pricing Rule implies 

$$
\widetilde {Z} _ {t} = \mathrm{E} ^ {*} \bigg [ \exp \Big \{- \int_ {t} ^ {T} r (s) d s \Big \} \cdot \widetilde {Z} _ {T} | \mathcal {F} _ {t} \bigg ] 0 \leq t \leq T,
$$

which implies 

$$
\begin{array}{r l} & Z _ {t} = \frac {\widetilde {Z} (t)}{\xi (t)} = \mathrm{E} ^ {*} \bigg [ \exp \Big \{- \int_ {t} ^ {T} r (s) d s \Big \} \frac {\xi (T)}{\xi (t)} Z _ {T} | \mathcal {F} _ {t} \bigg ] \\ & \qquad = \mathrm{E} ^ {*} \bigg [ \exp \Big \{- \int_ {t} ^ {T} (r (s) - d _ {Z} (s)) d s \Big \} Z _ {T} | \mathcal {F} _ {t} \bigg ]. \end{array}
$$

Remark 4.5. Both $r ( t )$ and $d _ { Z } ( t )$ may be stochastic. 

## 4.3 Connection with the PDE-Approach (Feynman-Kac Formula)

In Sect. 4.2 general valuation formulas for securities and derivatives were derived by martingale methods, which lead to the computation of conditional expectations. The classical approach of Black-Scholes-Merton is based on the solution of partial diferential equations under boundary conditions. A connection between these two at first sight fundamentally diferent approaches is provided by the so-called Feynman-Kac formula. If a number of technical conditions is satisfied, the Feynman-Kac formula enables one to switch back and forth between the martingale and the PDE-approach. In other words, the two seemingly so diferent approaches appear as two diferent sides of one coin. 

An essential condition for Feynman-Kac is, however, that the underlying security processes have to be markovian difusions, i.e. to be of the form 

$$
d X _ {t} = \mu (X _ {t}, t) d t + \sigma (X _ {t}, t) d B _ {t}\tag{8}
$$

with $( B _ { t } )$ a Brownian motion under the measure $P .$ 

## Feynman-Kac considers the following problem:

Find a solution $f ( x , t ) \in C ^ { 2 , 1 } ( \mathbb { R } \times [ 0 , T ] )$ for the PDE 

$$
A f (x, t) - r (x, t) f (x, t) = 0 \quad (x, t) \in \mathbb {R} \times [ 0, T)\tag{9}
$$

under the boundary condition 

$$
f (x, T) = g (x) \quad x \in \mathbb {R}\tag{10}
$$

where 

$$
A f (x, t) = f _ {t} (x, t) + f _ {x} (x, t) \mu (x, t) + \frac {1}{2} \sigma^ {2} (x, t) f _ {x x} (x, t).\tag{11}
$$

Remark 4.6. A f is the so-called “infinitesimal generator” of $f ( x , t )$ defined as the expected rate of change of $f ( X _ { t } , t )$ , given $X _ { t } = x , i . e .$ 

$$
A f (x, t) = \lim _ {\varDelta \to 0} \frac {1}{\varDelta} \left(\mathrm{E} [ f (X _ {t + \varDelta}, t + \varDelta) | X _ {t} = x ] - f (x, t)\right).
$$

From Itˆo’s formula applied to $d f ( X _ { t } , t )$ and the local martingale property of the Itˆo-integral one easily derives (11). 

The Feynman-Kac solution of (9) till (11), if it exists, is given by the conditional expectation 

$$
f (x, t) = \operatorname{E} _ {P} \Big [ \exp \Big \{- \int_ {t} ^ {T} r (X _ {s}, s) d s \Big \} g (X _ {T}) \Big | X _ {t} = x \Big ]\tag{12}
$$

where X is a solution of (8) with $X _ { t } = x$ 

For the necessary technical conditions (besides diferentiability a number of Lipschitz- and polynomial boundary conditions are required) we refer to Dufie (2001). 

Under additional assumptions the solution (12) is unique. In this case the Feynman-Kac formula also allows switching back: the conditional expectation (12) can be computed as the solution of the PDE (9) under the boundary constraint (10). 

Application: Let $X _ { t }$ be a security process with return 

$$
\frac {d X _ {t}}{X _ {t}} = \mu_ {X} (t) d t + \sigma_ {X} (t) d B _ {t},
$$

where $\mu _ { X }$ and $\sigma _ { X }$ are deterministic integrable functions of t. Consider a contingent claim $Z _ { T } ~ = ~ g ( X _ { T } )$ with $g : \mathbb { R } \longrightarrow \mathbb { R }$ continuous. By Girsanov there exists $P ^ { * } \sim P$ with 

$$
\frac {d X _ {t}}{X _ {t}} = r (t) d t + \sigma_ {X} (t) d B _ {t} ^ {*}\tag{13}
$$

Observe: In contrast to the martingale approach $r ( t )$ and $\sigma _ { X } ( t )$ have to be non-stochastic. 

According to the Fundamental Pricing Rule (see Sect. 4.2) one has 

$$
Z _ {t} = \mathrm{E} _ {P ^ {*}} \Big [ \exp \Big \{- \int_ {t} ^ {T} r (s) d s \Big \} g (X _ {T}) \Big | X _ {t} = x \Big ].\tag{14}
$$

Setting $Z _ { t } = f ( x , t ) \in C ^ { 2 , 1 }$ and 

$$
\mu (X _ {t}, t) = r (t) \cdot X _ {t}, \sigma (X _ {t}, t) = \sigma_ {X} (t) \cdot X _ {t},
$$

it follows from Feynman-Kac (when the technical FK-conditions are satisfied): 

$$
\begin{array}{l} Z _ {t} = f (x, t) \quad \text { is   solution   of   the   PDE } \\ - r (t) f (x, t) + f _ {t} (x, t) + r (t) x f _ {x} (x, t) + \frac {1}{2} \sigma_ {X} ^ {2} (t) x ^ {2} f _ {x x} (x, t) = 0 \end{array}\tag{15}
$$

under the boundary constraint 

$$
f (x, T) = g (x).\tag{16}
$$

Thus the solution of (14) is reduced to the solution of the partial differential equation (15) under the boundary constraint (16). 

(Check the equivalence of equation (15) with the Black-Scholes PDE in Sect. 2.5 (18)). 

## 4.4 Currency Options and Siegel-Paradox

In nostalgic remembrance of our dear deceased Deutschmark we consider the exchange rate USD/DM. (It is a good exercise to transfer this and the following sections to the exchange rate EUR/USD). 

We use the following notation: 

$$
\begin{array}{r l} {r ^ {\mathrm{DM}} (t) = \mathrm{DM} \text {spot rate at} t (\text {valid for the period} [ t, t + d t ])} \\ {r ^ {} (t)} & {= \mathbb {S} \text {spot - rate at} t} \\ {X _ {t}} & {= \text {exchange rate} / \mathrm{DM} (\text {price of 1} \mathbb {S} \text {in DM at} t)} \end{array}
$$

Note that $X _ { t }$ is a security with continuous dividend payment $r ^ { \mathbb { S } } ( t )$ According to Sect. 4.2 it follows 

$$
\frac {d X _ {t}}{X _ {t}} = (r ^ {\mathrm{DM}} (t) - r ^ {} (t)) d t + \sigma_ {X} (t) d B _ {t} ^ {*} \quad \text { under } P ^ {*}
$$

where $P ^ { * }$ is the risk-neutral expectation of a German investor. 

Consider now the process $Y _ { t } = X _ { t } ^ { - 1 }$ 100 which is (or was!) the exchange as quoted in the US for 1 DM in cents. 

$Y _ { t }$ is a security with continuous dividend $r ^ { \mathrm { D M } } ( t )$ . Note that $\sigma _ { Y } ( t ) =$ $- \sigma _ { X } ( t )$ since ln $Y _ { t } = - \ln X _ { t } + c _ { 0 }$ 

Question: Does the following relation hold 

$$
\frac {d Y _ {t}}{Y _ {t}} = (r ^ {} (t) - r ^ {\mathrm{DM}} (t)) d t + \sigma_ {Y} (t) d B _ {t} ^ {*} \quad \text { under } P ^ {*}
$$

for a risk-neutral American investor $\mathord { ? }$ 

Answer: From Itˆo it follows 

$$
\frac {d Y _ {t}}{Y _ {t}} = \frac {d X _ {t} ^ {- 1}}{X _ {t} ^ {- 1}} = \left(d \frac {1}{X _ {t}}\right) \cdot X _ {t}
$$

$$
d \frac {1}{X _ {t}} = - \frac {1}{X _ {t} ^ {2}} d X _ {t} + \frac {1}{2} \cdot 2 \cdot \frac {1}{X _ {t} ^ {3}} d \langle X \rangle_ {t}
$$

with 

$$
d \langle X \rangle_ {t} = \sigma_ {X} ^ {2} (t) X _ {t} ^ {2} d t.
$$

From $\sigma _ { Y } ( t ) = - \sigma _ { X } ( t )$ it then follows 

$$
\begin{array}{r l} & {\frac {d Y _ {t}}{Y _ {t}} = - \frac {d X _ {t}}{X _ {t}} + \sigma_ {X} ^ {2} (t) d t} \\ & {\qquad = (r ^ {} (t) - r ^ {\mathrm{DM}} (t) + \sigma_ {Y} ^ {2} (t)) d t + \sigma_ {Y} (t) d B _ {t} ^ {*}} \end{array}
$$

Thus a “risk-neutral” American investor requires a positive risk premium of $\sigma _ { Y } ^ { 2 } ( t )$ 

This is the so-called ”Siegel”- or ”Two-Country-Paradox” (see Siegel (1972), McCulloch (1975)). The solution to this Paradox will be given in Sect. 4.6. 

## 4.5 Change of Numeraire

A fundamental law in economics - the “Walras law” - implies that in equilibrium only relative prices can be determined. In order to ob tain absolute prices one has to choose one commodity as “numeraire”. Which commodity is chosen as numeraire is a question of convenience. The situation is similar in financial economics. However, here a nontrivial technical complication arises: the risk-neutral measure $P ^ { * }$ depends in a crucial way on the choice of the numeraire. 

Let $X _ { t } = ( X _ { t } ^ { 0 } , \ldots , X _ { t } ^ { n } ) _ { ( 0 \leq t \leq T ) }$ be the price process of $n + 1$ securities of the form 

$$
\frac {d X _ {t} ^ {i}}{X _ {t} ^ {i}} = \mu_ {i} (t) d t + \sigma_ {i} (t) d B _ {t} \quad \mathrm{under} P
$$

with $\mu _ { i } ( t ) , \sigma _ { i } ( t ) ( i = 0 , \ldots , n )$ adapted processes on $( \varOmega , ( \var F _ { t } ) , P )$ satisfying the boundary condition as defined in Sect. 4.1 . 

Usually $( X _ { t } ^ { 0 } )$ is chosen as numeraire, e.g. $d X _ { t } ^ { 0 } = r ( t ) X _ { t } ^ { 0 }$ dt (the accumulation process). Then absolute security prices, measured in units of $X ^ { 0 }$ , are given by the normed process 

$$
\widehat {X} _ {t} = \left(1, \frac {X ^ {1}}{X ^ {0}}, \dots , \frac {X ^ {n}}{X ^ {0}}\right) _ {t}.
$$

Consider a portfolio strategy $( \phi ) _ { t } = ( \phi ^ { 0 } , \dots , \phi ^ { n } ) _ { t }$ . Then $V _ { t } ( \phi ) = \phi _ { t } \circ X _ { t }$ is the value process with respect to $X _ { t }$ . Similarly $\widehat { V } _ { t } ( \phi ) = \phi _ { t } \circ \widehat { X } _ { t } =$ $V _ { t } ( \phi ) \cdot ( X _ { t } ^ { 0 } ) ^ { - 1 }$ is the value process with respect to $\widehat { X } _ { t }$ 

Recall: 

(φ<sub>t</sub>) is self-financing w.r.t. $X _ { t } \longleftrightarrow _ { \mathrm { ~ \tiny ~ d V } _ { t } ( \phi ) } = \phi _ { t } \circ d X _ { t }$ 

$$
\begin{array}{r l} \Longleftrightarrow & V _ {t} (\phi) = \phi_ {0} \circ X _ {0} + \int_ {0} ^ {t} \phi_ {s} \circ d X _ {s} \\ & = (\phi \bullet X) _ {t} 0 \leq t \leq T \end{array}
$$

Recall: (meaning of the diferent ’dots’) 

scalar multiplication 

scalar product 

stochastic integral 

Proposition 4.5.1. $\phi _ { t }$ is self-financing with respect to $X _ { t } \mathrm { \it { i f } } ,$ and only $i f , \phi _ { t }$ is self-financing with respect to ${ \hat { X _ { t } } }$ 

Proof. 

(= ) By assumption one has $d V _ { t } = \phi _ { t } \circ d X _ { t }$ 

Let $Y _ { t } ~ = ~ ( X _ { t } ^ { 0 } ) ^ { - 1 }$ . According to the rules for the covariation one has 

$$
d \langle V, Y \rangle_ {t} = d \langle \phi \bullet X, Y \rangle_ {t} = \phi_ {t} \circ d \langle X, Y \rangle_ {t}.
$$

Thus according to Itˆo’s product rule 

$$
\begin{array}{r l} & {d \widehat {V} _ {t} = d (V _ {t} \cdot Y _ {t}) = V _ {t} d Y _ {t} + Y _ {t} d V _ {t} + d \langle V, Y \rangle_ {t}} \\ & {\quad = (\phi_ {t} \circ X _ {t}) d Y _ {t} + Y _ {t} (\phi_ {t} \circ d X _ {t}) + \phi_ {t} \circ d \langle X, Y \rangle_ {t}} \\ & {\quad = \phi \circ (X _ {t} d Y _ {t} + Y _ {t} d X _ {t} + d \langle X, Y \rangle_ {t})} \\ & {\quad = \phi \circ d (X _ {t} \cdot Y _ {t}) = \phi \circ d \widehat {X} _ {t}} \end{array}
$$

( =) The procedure is analogous. 

Under the assumptions of Sect. 4.1, ”no arbitrage” and the Girsanov theorem applied to the ”market price of risk” process $\lambda ( t )$ under the Novikov condition (3) together with Prop. 4.2.1 imply: 

$\exists P ^ { * } \sim P : \widehat { X } _ { t }$ martingale under $P ^ { * }$ , and $B _ { t } ^ { * }$ B.M. w.r.t. $P ^ { * }$ 

Let $C _ { T } \in \mathcal { F } _ { T }$ be a contingent claim with $C _ { T } = V _ { T } ( \phi )$ for some selffinancing portfolio strategy $\phi$ . Consider $\widehat { C } _ { T } = C _ { T } / X _ { T } ^ { 0 } = \widehat { V } _ { T } ( \phi )$ . Since $d \widehat { V } = \phi \ d \widehat { X } , \widehat { V }$ is a local $P ^ { * }$ ! !-martingale. If it is a martingale, then it !follows: 

$$
\widehat {C} _ {t} = \mathrm{E} ^ {*} [ \widehat {V} _ {T} (\phi) | \mathcal {F} _ {t} ] = \mathrm{E} ^ {*} [ \widehat {C} _ {T} | \mathcal {F} _ {t} ]
$$

$$
C _ {t} = \widehat {C} _ {t} \cdot X _ {t} ^ {0} = \mathrm{E} ^ {*} \Big [ \frac {X _ {t} ^ {0}}{X _ {T} ^ {0}} \cdot C _ {T} | \mathcal {F} _ {t} \Big ].
$$

Question: Does the analysis depend on the choice of the numeraire $\mathord { ? }$ Let now $X ^ { i }$ be the numeraire. Consider 

${ \widetilde { X } } _ { t } = \Big ( \frac { X ^ { 0 } } { X ^ { i } } , \dots , 1 , \dots , \frac { X ^ { n } } { X ^ { i } } \Big ) _ { t }$ security prices measured in $X ^ { i }$ 

$$
\widetilde {V} = \frac {V}{X ^ {i}} \quad , \quad \widetilde {C} = \frac {C}{X ^ {i}}.
$$

According to Prop. 4.5.1 $\phi$ is also self-financing with respect to $\widetilde { X }$ 

Proposition 4.5.2. $\widetilde { X } _ { t }$ is a martingale under $Q _ { i } ^ { * } = \mathcal { E } ( N _ { i } ) \cdot P ^ { * }$ with 

$$
N _ {i} (t) = \int_ {0} ^ {t} \left(\underbrace {\sigma_ {i} (s) - \sigma_ {0} (s)} _ {\sigma_ {\hat {X} _ {i}}}\right) d B _ {s} ^ {*} \quad (0 \leq t \leq T)
$$

Remark 4.7. For $d X ^ { 0 } = X ^ { 0 } r ( t )$ dt one has $\sigma _ { 0 } = 0$ 

Proof. By assumption on $\sigma _ { i }$ and $\sigma _ { 0 }$ , there exist Lebesgue-integrable functions such that $| | \sigma _ { i } ( s , \omega ) - \sigma _ { 0 } ( s , \omega ) | | ^ { 2 } \leq \phi _ { i } ( s ) + \phi _ { 0 } ( s ) = \psi ( s )$ $P \mathrm { - a . s . }$ , which implies 

$$
\langle N _ {i} \rangle_ {t} = \int_ {0} ^ {t} | | \sigma_ {i} - \sigma_ {0} | | ^ {2} d s \leq \int_ {0} ^ {t} \psi (s) d s <   \infty \quad \forall t,
$$

and the Novikov condition (see Sect. 3.3 (4)) is fulfilled. Thus $N _ { i } ( t )$ is a martingale $\implies Z _ { t } = \mathcal { E } ( N _ { i } ( t ) )$ is a martingale. $\Rightarrow Q _ { i } ^ { * }$ is a probability measure. 

Hence (see Lemma 3.2.4) for any $j = 0 , 1 , \ldots , n$ 

$$
\widetilde {X} ^ {j} \in \mathcal {M} _ {l o c} ^ {c} (Q _ {i} ^ {*}) \longleftrightarrow \widetilde {X} ^ {j} \cdot Z \in \mathcal {M} _ {l o c} ^ {c} (P ^ {*}).
$$

We know $\frac { d \widehat { X } ^ { i } } { \widehat { X } ^ { i } } = \sigma _ { \widehat { X } ^ { i } } ( t ) d B _ { t } ^ { * }$ where $B _ { t } ^ { * }$ is a Brownian motion under $P ^ { * }$ 

$$
\Longrightarrow \widehat {X} _ {t} ^ {i} = \widehat {X} _ {0} ^ {i} \cdot \mathcal {E} (N _ {i} (t)).\tag{17}
$$

Thus it follows 

$$
\begin{array}{r l} \widetilde {X} ^ {j} \cdot Z = \frac {X ^ {j}}{X ^ {i}} \cdot Z & = \widehat {X} ^ {j} \cdot (\widehat {X} ^ {i}) ^ {- 1} \cdot Z \\ & = \widehat {X} ^ {j} \cdot (\widehat {X} _ {0} ^ {i}) ^ {- 1} \cdot \mathcal {E} (N _ {i}) ^ {- 1} \cdot \mathcal {E} (N _ {i}) \in \mathcal {M} _ {l o c} ^ {c} (P ^ {*}). \end{array}
$$

Therefore with $( X ^ { i } )$ as numeraire, we have 

$$
\frac {d \widetilde {X} _ {t} ^ {j}}{\widetilde {X} _ {t} ^ {j}} = \underbrace {\sigma_ {\widetilde {X} ^ {j}} (t)} _ {= \sigma_ {j} - \sigma_ {i}} d B _ {t} ^ {i} \qquad \text { where } B _ {t} ^ {i} \text { Brownian   motion   under } Q _ {i} ^ {*}.
$$

Again $\begin{array} { c } { { t } } \\ { { \int } } \\ { { 0 } } \end{array} | | \sigma _ { \widetilde { X } ^ { j } } ( s ) | | ^ { 2 } d s \leq \begin{array} { c } { { t } } \\ { { \overline { { { \psi } } } ( s ) d s < \infty } } \\ { { 0 } } \end{array}$ implies that $\widetilde { X } ^ { j }$ is indeed a martingale. 

Conclusion: $P ^ { * }$ is a martingale measure with respect to $( X ^ { 0 } )$ as numeraire if, and only if, $Q _ { i } ^ { * }$ is a martingale measure with respect to $( X ^ { i } )$ as numeraire. 

Connection $B _ { t } ^ { * } \longleftrightarrow B _ { t } ^ { i }$ 

$$
B _ {t} ^ {*} \in \mathcal {M} ^ {c} (P ^ {*}) , Q _ {i} ^ {*} = \mathcal {E} (N _ {i}) \cdot P ^ {*} \underset {\text {Girsanov}} {\Longrightarrow} B _ {t} ^ {i} = B _ {t} ^ {*} - \langle B ^ {*}, N _ {i} \rangle_ {t} \in \mathcal {M} ^ {c} (Q _ {i} ^ {*})
$$

$$
\Longrightarrow B _ {t} ^ {i} = B _ {t} ^ {*} - \int_ {0} ^ {t} \underbrace {\sigma_ {\widehat {X} _ {i}} (s)} _ {\sigma_ {i} - \sigma_ {0}} d \langle B \rangle_ {s} = B _ {t} ^ {*} + \int_ {0} ^ {t} (\sigma_ {0} - \sigma_ {i}) (s) d s.
$$

Thus we have $\widetilde { C } _ { t } = \mathrm { E } _ { i } ^ { * } \left[ \frac { C _ { T } } { X _ { T } ^ { i } } \left| \mathcal { F } _ { t } \right. \right]$ with $X _ { t } ^ { i }$ as numeraire. 

The decisive result is now given by the following proposition: 

Proposition 4.5.3. 

$$
X _ {t} ^ {i} \cdot \widetilde {C} _ {t} = X _ {t} ^ {0} \cdot \widehat {C} _ {t}.
$$

$( i . e .$ , the valuation of the contingent claim $C _ { T }$ does not depend on the numeraire.) 

Lemma 4.5.4. (Bayes rule): Let $Q = Z _ { T } \cdot P$ on $\mathcal { F } _ { T }$ and $Y \in L ^ { 1 } ( \varOmega , \mathcal { F } _ { t } , Q )$ . Then, for any $s < t \leq T$ , it follows 

$$
\mathrm{E} _ {Q} [ Y | \mathcal {F} _ {s} ] = \frac {1}{Z _ {s}} \mathrm{E} _ {P} [ Y \cdot Z _ {t} | \mathcal {F} _ {s} ].
$$

Proof. Let $A \in \mathcal { F } _ { s }$ . Since $\frac { d Q _ { t } } { d P _ { t } } = Z _ { t } = \mathrm { E } _ { P } [ Z _ { T } \left| \mathcal { F } _ { t } \right]$ it follows 

$$
\begin{array}{r l} & {\mathrm{E} _ {Q} [ \mathbf {1} _ {A} Y ] = \mathrm{E} _ {P} [ \mathbf {1} _ {A} Y \cdot Z _ {t} ] = \mathrm{E} _ {P} \Big [ \mathbf {1} _ {A} \mathrm{E} _ {P} [ Y \cdot Z _ {t} | \mathcal {F} _ {s} ] \Big ]} \\ & {\qquad = \mathrm{E} _ {Q} \Big [ \mathbf {1} _ {A} \cdot \frac {1}{Z _ {s}} \mathrm{E} _ {P} [ Y \cdot Z _ {t} | \mathcal {F} _ {s} ] \Big ].} \end{array}
$$

Proof of Prop. 4.5.3:. According to (17) one has $Z _ { t } = ( \widehat { X } _ { 0 } ^ { i } ) ^ { - 1 } \cdot \widehat { X } _ { t } ^ { i }$ . Thus Lemma 4.5.4 implies 

$$
\begin{array}{r} \widetilde {C} _ {t} = \mathrm{E} _ {i} ^ {*} [ \widetilde {C} _ {T} | \mathcal {F} _ {t} ] = \frac {1}{Z _ {t}} \mathrm{E} ^ {*} [ \widetilde {C} _ {T} Z _ {T} | \mathcal {F} _ {t} ] = \frac {\widehat {X} _ {0} ^ {i}}{\widehat {X} _ {t} ^ {i}} \mathrm{E} ^ {*} \Big [ \frac {C _ {T}}{X _ {T} ^ {i}} \cdot \frac {\widehat {X} _ {T} ^ {i}}{\widehat {X} _ {0} ^ {i}} | \mathcal {F} _ {t} \Big ] \\ = \frac {1}{\widehat {X} _ {t} ^ {i}} \mathrm{E} ^ {*} \Big [ \underbrace {\frac {C _ {T}}{X _ {T} ^ {i}} \cdot \frac {X _ {T} ^ {i}}{X _ {t} ^ {0}}} _ {\widehat {C} _ {T}} | \mathcal {F} _ {t} \Big ] = \frac {X _ {t} ^ {0}}{X _ {t} ^ {i}} \widehat {C} _ {t}. \end{array}
$$

## 4.6 Solution of the Siegel-Paradox

The techniques developed in the previous section solve the Siegel-Paradox. The spot price process for a portfolio in Deutschmark and Dollars is given by 

$$
Z _ {t} = (X _ {t}, Y _ {t}) = (\beta_ {t} ^ {\mathrm{DM}}, e _ {t} \beta_ {t} ^ {}) \qquad \mathrm{with}
$$

e = exchange rate $/DM 

$$
\beta_ {t} ^ {\mathrm{DM}} = \exp \int_ {0} ^ {t} r ^ {\mathrm{DM}} (s) d s
$$

$$
\beta_ {t} ^ {} = \exp \int_ {0} ^ {t} r ^ {} (s) d s.
$$

From the view point of the German investor $( X _ { t } )$ is the numeraire. Thus 

$$
\widehat {Z} _ {t} = (1, \widehat {Y} _ {t}) \quad \text {with} \widehat {Y} _ {t} = e _ {t} \frac {\beta_ {t} ^ {\S}}{\beta_ {t} ^ {\mathrm{DM}}}
$$

and 

$$
\frac {d \widehat {Y} _ {t}}{\widehat {Y} _ {t}} = \sigma_ {\widehat {Y}} (t) d B _ {t}, \sigma_ {\widehat {Y}} = \sigma_ {Y} - \sigma_ {X} = \sigma_ {e}
$$

!under the martingale measure $P ^ { * }$ which is the expectation of the riskneutral German investor. 

Applying Itˆo’s product rule it follows: 

$$
\Longrightarrow \frac {d e _ {t}}{e _ {t}} = (r _ {\mathrm{DM}} (t) - r _ {} (t)) d t + \sigma_ {e} (t) d B _ {t} \quad \text {   under   } P ^ {*}.
$$

However, from the viewpoint of the American investor the numeraire is $( Y _ { t } )$ 

$$
\implies \widetilde {Z} _ {t} = (\widetilde {X} _ {t}, 1) \quad \text {with} \widetilde {X} _ {t} = f _ {t} \cdot \frac {\beta_ {t} ^ {\mathrm{DM}}}{\beta_ {t} ^ {\S}}, f _ {t} = \frac {1}{e _ {t}} \quad (\text {exch. rate DM / \S})
$$

New martingale measure : $Q ^ { * } = { \mathcal { E } } ( N ) \cdot P ^ { * } \quad N _ { t } = \int _ { 0 } ^ { t } \underbrace { \sigma _ { \widehat { Y } } ( s ) } _ { = \sigma _ { e } } d B _ { s } .$ 

$\widetilde { X }$ martingale under $Q ^ { * } \Longrightarrow \frac { d { \widetilde { X } } _ { t } } { \widetilde { X } _ { t } } = \sigma _ { \widetilde { X } } ( t ) d { \widetilde { B } } _ { t }$ 

with $\sigma _ { \tilde { X } } = \sigma _ { X } - \sigma _ { Y } = - \sigma _ { e } = \sigma _ { f }$ and $d \widetilde { B } _ { t } = d B _ { t } + \sigma _ { f }$ dt is Brownian motion under $Q ^ { * }$ 

$$
\begin{array}{l l} \Longrightarrow & \frac {d f _ {t}}{f _ {t}} = (r ^ {} (t) - r ^ {\mathrm{DM}} (t)) d t + \sigma_ {f} (t) d \widetilde {B} _ {t} \\ & = \left(r ^ {} (t) - r ^ {\mathrm{DM}} (t) + \sigma_ {f} ^ {2} (t)\right) d t + \sigma_ {f} (t) d B _ {t} \end{array} \quad \begin{array}{l l} \textbf {u n d e r} Q ^ {*} \\ \textbf {u n d e r} P ^ {*} \end{array}
$$

Thus also from the view point of the American investor there is no risk premium under the correct martingale measure $Q ^ { * }$ 

## 4.7 Admissible Strategies and Arbitrage-free Pricing

The “No arbitrage” condition given in section 4.1 rules out arbitrage opportunities in a short (strictly speaking infinitesimal) time interval. As we have shown this condition implies that the “market price of risk” process $\lambda ( t )$ must be identic for all security price processes in the considered market, which under the “Novikov” condition implies the existence of an equivalent martingale measure $P ^ { * }$ . Conversely, if an equivalent martingale measure $P ^ { * }$ exists, then according to the relation (5) infinitesimal arbitrage opportunities cannot exist. 

However, the “no arbitrage” condition used so far does not rule out, that there may exist dynamic trading strategies $\phi$ which over a finite time horizon allow arbitrage profits. 

Let $X _ { t } = ( X ^ { 0 } , \ldots , X ^ { n } ) _ { 0 \leq t \leq T }$ be the price process of $n { \mathrel { + { 1 } } }$ securities satisfying the conditions given in section 4.5 . Let $( \phi ) _ { t } = ( \phi ^ { 0 } , \dots , \phi ^ { n } ) _ { i }$ <sub>t</sub> be a self-financing portfolio strategy, i.e. an adapted $( n + 1 )$ -dimensional stochastic process with $V _ { t } ( \phi ) = \phi _ { t } \circ X _ { t }$ and $d V _ { t } = \phi _ { t } \circ d X _ { t }$ . As shown in Prop. 4.5.1, the property of $\phi$ of being self-financing does not depend on the choice of the numeraire. 

Definition 4.7.1. An arbitrage opportunity is a self-financing portfolio strategy $\phi$ such that the wealth process $V _ { t } ( \phi )$ satisfies the following conditions: 

$$
V _ {0} (\phi) = 0, \quad P [ V _ {T} (\phi) \geq 0 ] = 1, \quad a n d \quad P [ V _ {T} (\phi) > 0 ] > 0.
$$

Such a portfolio or trading strategy would allow one to start with an initial investment of zero and without adding money in the time interval $[ 0 , T ]$ to receive a positive amount at time T with positive probability. Since even in the simplest case of the standard Black-Scholes model $( d = 1$ , µ and $\sigma = c o n s t . , \ r = 0 )$ there exist self-financing strategies which allow arbitrage (see e.g. Harrison-Kreps (1979) or Dufie (2001)) we need some subclass of “admissible” strategies which rule out such arbitrage opportunities. 

Consider the case where $X _ { t } ^ { 0 } = \beta ( t ) = \exp \intop _ { 0 } ^ { t } r ( s )$ ds is chosen as numeraire, and the discounted process is $\widehat { X } = X / X ^ { 0 }$ 

Let $\varPhi ^ { 0 }$ be the class of self-financing strategies which are integrable w.r.t. $\widehat { X }$ and for which there exists some constant k with 

$$
\widehat {V} _ {t} (\phi) = V _ {t} (\phi) / X _ {t} ^ {0} = \phi_ {t} \circ \widehat {X} _ {t} \geq k \quad \forall t \in [ 0, T ]\tag{18}
$$

The condition (18) can be interpreted as a credit constraint, which means that short sales are allowed, but the wealth process must stay above a lower bound k, which may be negative. The strategies in $\varPhi ^ { 0 }$ are also called “tame” (w.r.t. X<sup>0</sup>). 

Remark 4.8. If the short rate process $r ( t )$ is bounded, then obviously the condition (18) is equivalent to: $V _ { t } ( \phi )$ is bounded below. 

Let $M ( \widehat { X } )$ denote the set of equivalent martingale measures under which $\widehat { X }$ !is a martingale. 

Theorem 4.7.2. If $\mathcal { M } ( \widehat { X } ) \neq \emptyset$ , then there is no arbitrage in $\varPhi ^ { 0 }$ . 

Proof. Consider $\phi \in \varPhi ^ { 0 }$ with $V _ { 0 } ( \phi ) = 0$ and $P [ V _ { T } ( \phi ) \ge 0 ] = 1$ . Then $\widehat V _ { t } ( \phi ) = \phi _ { t } \circ \widehat X _ { t } = V _ { t } ( \phi ) \cdot ( X _ { t } ^ { 0 } ) ^ { - 1 }$ is the value process with respect to $\widehat { X } _ { t }$ . Since $X ^ { 0 }$ !is strictly positive, $V _ { t }$ is positive if $\widehat { V } _ { t }$ is positive. Since ! !Vt is self-financing w.r.t. X, it is also self-financing w.r.t. $\widehat { X }$ . Hence $\widehat { V } _ { t } ( \phi ) = \phi \bullet \widehat { X } _ { t }$ is a local martingale for any $P ^ { * } \in \mathcal { M } ( \widehat { X } )$ !. Since $\widehat { V } _ { t }$ is by ! ! ! !assumption bounded below, Fatou‘s lemma (see Sect. 1.1) applied to a sequence of localizing stopping times of $\widehat { V } _ { t }$ implies $E ^ { * } [ \widehat { V } _ { T } ] \leq E ^ { * } [ \widehat { V } _ { 0 } ] = 0$ , which together with $\widehat { V } _ { T } \geq 0 P ^ { \ast } \mathrm { { - a . s } }$ !. implies $P ^ { * } [ \widehat { V } _ { T } > 0 ] = 0$ !. Since $P ^ { * } \sim P$ !this is equivalent to $P [ V _ { T } > 0 ] = 0$ 

If $C _ { T } \in L ^ { 1 } ( \varOmega , \mathcal F _ { T } , P ^ { * } )$ is a (European) contingent claim, which settles at time $T _ { i }$ , then the fundamental pricing rule implies that its price $\varPi _ { t }$ under $P ^ { * } \in \mathcal { M } ( \widehat { X } )$ at any $0 \leq t \leq T$ is given by the process 

$$
\Pi_ {t} = X _ {t} ^ {0} E _ {P *} [ C _ {T} / X _ {T} ^ {0} \mid \mathcal {F} _ {t} ]\tag{19}
$$

If there is a unique $P ^ { * } \in \mathcal { M } ( \widehat { X } )$ this process is also uniquely deter-!mined. However, there may be many diferent equivalent martingale measures in $\mathcal { M } ( \widehat { X } )$ , as is the case when the market is “incomplete”. In !this case the price process (19) is no longer uniquely determined by the fundamental pricing rule, but depends on the choice of an equivalent martingale measure. In particular this is the case if $n < d ,$ , i.e. there are less securities in the market than sources of uncertainty. Thus in incomplete markets the price of an arbitrary contingent claim cannot be determined by “no arbitrage” arguments. 

Definition 4.7.3. A contingent claim $C _ { T } \in L ^ { 1 } ( \varOmega , \mathcal { F } _ { T } , P ^ { * } )$ is attainable $i f$ there exists an admissible strategy $\phi \in \varpi$ with $C _ { T } \ = \ V _ { T } ( \phi )$ and $\widehat { V } _ { t } ( \phi ) = \phi _ { t } \circ X _ { t } / X _ { t } ^ { 0 }$ is a $P ^ { * }$ -martingale for some $P ^ { * } \in \mathcal { M } ( \widehat { X } )$ 

If any integrable contingent claim is attainable, the market is called complete. 

Proposition 4.7.4. The price $\varPi _ { t }$ of any attainable contingent claim $C _ { T }$ is uniquely determined by no-arbitrage and is given by the relation (19), where the expectation is taken for arbitrary $P ^ { * } \in \mathcal { M } ( \widehat { X } )$ 

Proof. Let $\phi$ and $\psi$ be two admissible strategies with $V _ { T } ( \phi ) = V _ { T } ( \psi ) =$ $C _ { T }$ and $P _ { 1 } ^ { * } , P _ { 2 } ^ { * } \in \mathcal { M } ( \widehat { X } )$ . Then also $\widehat { V } _ { T } ( \phi ) = \widehat { V } _ { T } ( \psi ) = \mathrm { { } } \widehat { C } _ { T }$ . Consider !the two value processes 

$$
V _ {t} (\phi) = X _ {t} ^ {0} E _ {P _ {1} ^ {*}} [ \widehat {V} _ {T} (\phi) | \mathcal {F} _ {t}) ]\tag{20}
$$

$$
V _ {t} (\psi) = X _ {t} ^ {0} E _ {P _ {2} ^ {*}} [ \widehat {V} _ {T} (\psi) | \mathcal {F} _ {t}) ].\tag{21}
$$

Then $\widehat { V } _ { t } ( \phi ) = \phi _ { t } \circ \widehat { X } _ { t }$ is a local $P _ { 2 } ^ { * }$ - martingale and, since it is bounded ! !from below, by Fatou’s lemma, a $P _ { 2 } ^ { * }$ - sub-martingale, which implies 

$$
\widehat {V} _ {t} (\psi) = E _ {P _ {2} ^ {*}} [ \widehat {V} _ {T} (\psi) | \mathcal {F} _ {t}) ] = E _ {P _ {2} ^ {*}} [ \widehat {V} _ {T} (\phi) | \mathcal {F} _ {t}) ] \leq \widehat {V} _ {t} (\phi).\tag{22}
$$

By the same argument it also follows $\widehat { V } _ { t } ( \phi ) \leq \widehat { V } _ { t } ( \psi )$ . Hence $\varPi _ { t } = V _ { t } ( \phi ) = V _ { t } ( \psi )$ ! !is the unique arbitrage price of $C _ { T }$ . 

Unfortunately the condition of “tameness” depends on the choice of the numeraire. Thus an admissible strategy in $\varPhi ^ { 0 }$ may not be admissible for the numeraire $X ^ { i }$ , although the property of self-financing is independent of the numeraire, as shown in Proposition 4.5.1. This is unsatisfactory from an economic point of view. For the property of a market to be “arbitrage free” or not should not depend on the choice of the numeraire. 

A satisfactory solution of this problem, which requires very advanced technical methods, is beyond the scope of these notes. These problems have been dealt with in a number of papers by Delbaen and Schachermayer, see in particular Delbaen-Schachermayer (1995) and Delbaen-Schachermayer (1997). 

## 4.8 The “Forward Measure”

The “forward measure” is a useful tool when interest rates are stochastic. Then the accumulation factor 

$$
\beta_ {t} (\omega) = \exp \int_ {0} ^ {t} r (s, \omega) d s
$$

is a stochastic process, making the computation of the conditional expectation in the Fundamental Pricing Rule (Theorem 4.2.2) cumbersome. 

Consider the following connection between $\$ 123,456$ and $\$ 1$ $( T = \mathrm { \mathop {  } { t o m o r r o w } ^ { \prime \prime } } )$ : 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/e11cea2b172cc1d6f61dd6ff01b74a3d616e86615c61f834038e5e68fd834b37.jpg)


spot prices 

zerobond prices 

$$
P _ {0} (T) \longleftarrow P _ {t} (T) \longleftarrow 1
$$

Let $X _ { t } = ( X ^ { 0 } , X ^ { 1 } , \ldots ) t$ be price processes of securities. Choosing $X _ { t } ^ { 0 } =$ $\beta _ { t }$ as numeraire determines the martingale measure $P ^ { * }$ , under which 

$$
X _ {t} ^ {i} = \mathrm{E} ^ {*} \left[ \frac {\beta_ {t}}{\beta_ {T}} X _ {T} ^ {i} | \mathcal {F} _ {t} \right] i = 0, 1, 2 \dots , 0 \leq t \leq T.
$$

Remark 4.9. $P ^ { * }$ is also called the “spot martingale measure”, since the spot price process is chosen as numeraire. 

In particular one has 

$$
P _ {t} (T) = \mathrm{E} ^ {*} \left[ \frac {\beta_ {t}}{\beta_ {T}} \mid \mathcal {F} _ {t} \right] \quad \text { since } P _ {T} (T) \equiv 1.
$$

Thus 

$$
\widehat {P} _ {t} (T) = \frac {P _ {t} (T)}{\beta_ {t}} \quad \mathrm{isa} \quad P ^ {*} - m a r t i n g a l e
$$

and 

$$
\frac {d P _ {t} (T)}{P _ {t} (T)} = r (t) d t + \sigma (t, T) \circ d B _ {t} ^ {*} \quad \text { under } P ^ {*}.
$$

Remark 4.10. Observe that $\sigma ( t , t ) = 0$ since $P _ { t } ( t ) \equiv 1$ 

Change of numeraire from $\$ 6$ to $\$ 1$ 

Instead of $\beta _ { t }$ choose now $P _ { t } ( T )$ as numeraire. According to Sect. 4.5 the corresponding martingale measure $P _ { T }$ is given by 

$$
P _ {T} = \mathcal {E} (L (T)) \cdot P ^ {*} \quad \mathrm{with}
$$

$$
L _ {t} (T) = \int_ {0} ^ {t} \sigma_ {\hat {P} _ {t}} (s) \circ d B _ {s} ^ {*} = \int_ {0} ^ {t} \sigma (s, T) \circ d B _ {s} ^ {*}
$$

and one has 

$$
B _ {t} ^ {T} = B _ {t} ^ {*} - \langle B _ {t} ^ {*}, L _ {t} \rangle = B _ {t} ^ {*} - \int_ {0} ^ {t} \sigma (s, T) d s.
$$

Let $H _ { T } \in \mathcal { F } _ { T }$ be a contingent claim. Then under $P ^ { * }$ : 

$$
H _ {t} = \mathrm{E} ^ {*} \left[ \frac {\beta_ {t}}{\beta_ {T}} H _ {T} \mid \mathcal {F} _ {t} \right] (\text { Price   in   } t.)
$$

Under $P _ { T }$ it follows : 

$$
\widetilde {H} _ {T} = \frac {H _ {T}}{P _ {T} (T)} = H _ {T}
$$

$$
\widetilde {H} _ {t} = E _ {T} [ H _ {T} | \mathcal {F} _ {t} ] \quad (\text { Price   in   } \S_ {T})
$$

$$
H _ {t} = \widetilde {H} _ {t} \cdot P _ {t} (T) \quad \left(\text { Price   in   } t\right).
$$

Thus we have proved 

$$
H _ {t} = \mathrm{E} ^ {*} \Big [ \frac {\beta_ {t}}{\beta_ {T}} H _ {T} | \mathcal {F} _ {t} \Big ] = P _ {t} (T) \cdot \mathrm{E} _ {T} [ H _ {T} | \mathcal {F} _ {t} ]
$$

$P _ { T } = \mathbf { \partial } ^ { 6 }$ “forward measure” (see e.g. Geman-ElKaroui-Rochet (1995)) 

The connection with the definition of $P _ { T }$ sometimes given in the literature is established by the following proposition : 

Proposition 4.8.1. $P _ { T } [ A ] = \mathrm { E } ^ { * } \Big [ ( \beta _ { T } { \cdot } P _ { 0 } ( T ) ) ^ { - 1 } | \mathcal { F } _ { t } \Big ] { \cdot } P ^ { * } [ A ]$ for any $A \in$ $\mathcal { F } _ { t }$ 

Proof. $\widehat { X } _ { t } = \widehat { P } _ { t } ( T ) = \frac { P _ { t } ( T ) } { \beta _ { t } }$ is P∗-martingale with 

$$
\frac {d \widehat {X} _ {t}}{\widehat {X} _ {t}} = \sigma (t, T) \circ d B _ {t} = d L _ {t} (T)
$$

$$
\Longrightarrow \widehat {X} _ {t} = \underbrace {\widehat {X} _ {0}} _ {= P _ {0} (T)} \cdot \mathcal {E} (L _ {t} (T)).
$$

For $A \in { \mathcal { F } } _ { t }$ one has 

$$
\begin{array}{c} P _ {T} [ A ] = \mathrm{E} ^ {*} [ \mathcal {E} (L _ {T} (T))   |   \mathcal {F} _ {t} ] \cdot P ^ {*} [ A ] \\ = \mathcal {E} (L _ {t} (T)) \cdot P ^ {*} [ A ]. \end{array}\tag{23}
$$

Since $\widehat { X } _ { t } \ P ^ { * }$ -martingale, it follows 

$$
\mathrm{E} ^ {*} \Big [ \frac {1}{\beta_ {T}} | \mathcal {F} _ {t} \Big ] = \mathrm{E} ^ {*} [ \widehat {X} _ {T} | \mathcal {F} _ {t} ] = \widehat {X} _ {t} = P _ {0} (T) \cdot \mathcal {E} (L _ {t} (T))
$$

which together with (23) completes the proof. 

□ 

## 4.9 Option Pricing Under Stochastic Interest Rates

As an application of the forward measure we now study currency options when interest rates are stochastic. 

Let $\ S _ { t } \ \left( = \ e _ { t } \right)$ be the process of the exchange rate $\$ /\mathrm { D M }$ . This gives rise to the following price processes for a portfolio in $\mathrm { D M } / { \mathfrak { F } }$ 

$$
(\beta_ {t} ^ {\text { DM }}, _ {t} \beta_ {t} ^ {}) \qquad \begin{array}{l} \text { ``spot'' price processes } \\ (\text { DM }, _ {t} \text { ``today' }) \end{array} \quad 0 \leq t \leq T
$$

$$
(P_{t}^{\rm DM}(T),\\ (t)\cdot P_{t}^{(T)}) \text{forward price processes} 0\leq t\leq T  .\\ (\text{DM},\\ (tomorrow))
$$

Now choose $P _ { t } ^ { \mathrm { D M } } ( T )$ as numeraire, i.e. instead of $\mathrm { D M } _ { t } \ \mathrm { ( " t o d a y " ) }$ calculate in DM<sub>T</sub> (”tomorrow”). This leads to the following discounted processes: 

$$
\widehat {Z} _ {t} = (1, \widehat {Y} _ {t}) \quad \text { with } \widehat {Y} _ {t} = _ {t} ^ {} \cdot \frac {P _ {t} ^ {} (T)}{P _ {t} ^ {\mathrm{DM}} (T)} \quad (T \text {-forward -price at} t)
$$

By the Interest-rate-parity theorem, which is illustrated in the following diagram, $\widehat { Y } _ { t }$ is, at time t, the forward price $F _ { t } ( T )$ of one dollar delivered !at time T. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/7a05a8d5bbe801260fe05aea51c0eb4266c32aabdc2c8828cd016a597404526a.jpg)



Diagram: Interest-Rate-Parity Theorem


Under the forward measure $P _ { T } , \widehat { Y } _ { t }$ is a martingale. 

Clearly $\ S _ { T } = \widehat { Y } _ { T }$ . Thus it follows, that the price $H _ { t }$ of the call option $H _ { T } = ( \mathbb { S } _ { T } - K ) ^ { + }$ at time t is given by : 

$$
\begin{array}{r l} & H _ {t} = P _ {t} ^ {\mathrm{DM}} (T) \mathrm{E} _ {T} [ (\widehat {Y} _ {T} - K) ^ {+} | \mathcal {F} _ {t} ] = P _ {t} ^ {\mathrm{DM}} (T) \Big [ \widehat {Y} _ {t} \Phi (d _ {t} ^ {1}) - K \cdot \Phi (d _ {t} ^ {2}) \Big ] \\ & \quad = \S_ {t} \cdot P _ {t} ^ {} (T) \cdot \Phi (d _ {t} ^ {1}) - K \cdot P _ {t} ^ {\mathrm{DM}} (T) \cdot \Phi (d _ {t} ^ {2}) \end{array}
$$

where $d _ { t } ^ { 1 , 2 } = { \frac { \ln ( \widehat { Y _ { t } } / K ) } { \eta _ { t } } } \pm { \frac { 1 } { 2 } } \eta _ { t }$ with 

$$
\eta_ {t} ^ {2} = \int_ {t} ^ {T} | | \sigma_ {\widehat {Y}} (s) | | ^ {2} d s = \int_ {t} ^ {T} | | \sigma_ {} (s) + \sigma^ {} (s, T) - \sigma^ {\mathrm{DM}} (s, T) | | ^ {2} d s
$$

$( \sigma ^ { \mathfrak { S } } \ \mathrm { r e s p . } \ \sigma ^ { \mathrm { D M } }$ are the volatilities of $P ^ { \mathbb { S } } ( T )$ resp. $P ^ { \mathrm { D M } } ( T ) )$ 

Consider the following hedge strategy in T-forward contracts: 

Buy at $t : \varPhi ( d _ { t } ^ { 1 } )$ Dollar at T Sell at $t : - K \cdot \varPhi ( d _ { t } ^ { 2 } )$ DM at T 

$$
\Longrightarrow V _ {t} (\phi) = \Phi (d _ {t} ^ {1}) \cdot \widehat {Y} _ {t} - K \cdot \Phi (d _ {t} ^ {2}) \mathrm{DMat} T
$$

$$
\Longrightarrow V _ {T} (\phi) = \left\{ \begin{array}{c c} _ {T} - K & \text { for }   _ {T} = \widehat {Y} > K \\ 0 & \text { for }   _ {T} \leq K \end{array} \right\} = H _ {T}
$$

Hence the strategy $\phi$ duplicates the contingent claim $H _ { T }$ 

Exercise: Show that the strategy $\phi$ is self-financing. 

Hint: Consider the function $F ( x , t ) = x \cdot \varPhi ( d ^ { 1 } ( x , t ) ) - K \cdot \varPhi ( d ^ { 2 } ( x , t ) )$ 

$$
\text { where } d ^ {1, 2} (x, t) = \frac {\ln (x / K)}{\eta_ {t}} \pm \frac {1}{2} \eta_ {t} \qquad \text { with } \qquad \eta_ {t} ^ {2} = \int_ {t} ^ {T} | | \sigma_ {X} (s) | | ^ {2} d s.
$$

1) Show $x \cdot \varphi ( d ^ { 1 } ) = K \cdot \varphi ( d ^ { 2 } )$ where $\begin{array} { r } { \varphi ( z ) = \frac { 1 } { \sqrt { 2 \pi } } e ^ { - \frac { 1 } { 2 } z ^ { 2 } } } \end{array}$ (density of Φ) 

2) Using the relation 1) show $F _ { x } ( x , t ) = \varPhi ( d ^ { 1 } ( x , t ) )$ 

3) Show $\begin{array} { r } { F _ { t } ( x , t ) = x \cdot \varphi ( d ^ { 1 } ) \cdot \frac { d } { d t } \eta ( t ) } \end{array}$ 

4) Show $\begin{array} { r } { \frac { d } { d t } \eta ( t ) = - \frac { 1 } { 2 \eta } \cdot | | \boldsymbol { \sigma } _ { X } ( t ) | | ^ { 2 } } \end{array}$ 

5) Show $\begin{array} { r } { F _ { t } + \frac { 1 } { 2 } F _ { x x } x ^ { 2 } | | \boldsymbol { \sigma } _ { X } ( t ) | | ^ { 2 } = 0 } \end{array}$ 

$\implies V _ { t } ( \phi ) = F ( \widehat { Y } _ { t } , t )$ is self-financing (see Sect. 2.5 (15) and Rem. 2.11) 

$$
\Longrightarrow d V _ {t} (\phi) = \Phi (d _ {t} ^ {1}) d \widehat {Y} _ {t}
$$

# Term Structure Models

Term structure models are considered as one of the most complex and mathematically demanding subjects in finance. Contrary to the valuation of options, or more generally of contingent claims, the valuation of interest rate dependent instruments requires the study of many interacting markets, the so-called “term structure” of interest rates. 

One of the first term structure models was the short-rate model of Vasicek (1977). By modelling the “short rate” over time, the dynamics of the “forward rate” is also implicitly determined. A drawback of shortrate models is that they cannot be fitted to the total term structure (they only catch the first point of the “yield curve”). This shortcoming was first overcome by the Ho-Lee model (see Ho-Lee (1986)), which starts with the present term structure as given by the zerobond prices. Both models are sketched in Sect. 5.4 as special HJM models. 

A fundamental contribution was made by Heath-Jarrow-Morton (1992), who start by modelling the complete term structure as given by the (continuously compounded) forward rates. Most implementations of the HJM model are “Gaussian”, meaning that the forward rates are assumed to be normally distributed. But this implies that interest rates may become negative, a rather undesirable property. This problem was overcome by the “log-normal” models. However, assuming that continuously compounded interest rates are log-normally distributed led to new dificulties: the rates explode over time and thus these models (see Black-Derman-Toy (1990) or Black-Karasinski (1991)) are unstable. This problem was solved by the (discrete) log-normal Sandmann-Sondermann model (see Sandmann-Sondermann (1993)). By switching from continuously compounded to “efective”, i.e., annually compounded rates, they showed that such models have stable dynamics, and hence have a stable continuous limit (see Sandmann-Sondermann (1994)). This approach finally led to the so-called “LI-BOR” or “Market” models due to Sandmann-Sondermann-Miltersen (1995) and Miltersen-Sandmann-Sondermann (1997), and further developed by Brace-Gatarek-Musiela (1997). These models have become quite popular in the finance industry, since they are stable and arbitrage-free, produce non-negative interest rates and, most importantly, reflect the market practice of Black’s caplet formula (see Sect. 5.5 and 5.6). 

For a comprehensive treatment of Fixed Income Markets and term structure models we refer to Musiela-Rutkowski (1997), who also give a detailed overview of the historical development of this complex subject. 

By looking at a term structure model in continuous time in the general form of Heath-Jarrow-Morton (1992) as an infinite collection of assets (the zerobonds of diferent maturities), the methods developed in Chap. 4 can be applied without modification to this situation. Readers who have gone through the original articles of HJM may appreciate the simplicity of this approach, which leads to the basic results of HJM in a straightforward way. The same applies to the Libor Market Model treated in Sect. 5.5 . 

## 5.1 Diferent Descriptions of the Term Structure of Interest Rates

There are three equivalent descriptions of the term structure, namely by means of 

1) Zerobonds 

P(t, T) = price of one Euro, deliverable at T, at time t 

2) yields (continuously compounded) 

$$
y (t, T) := - \frac {1}{T - t} \log P (t, T)
$$

5.1 Diferent Descriptions of the Term Structure of Interest Rates 

3) forward rates (continuously compounded) 

$$
f (t, T) := - \frac {\partial}{\partial T} \log P (t, T).
$$

Relations between 1), 2) and 3) : 

$1 ) \implies 2 )  3 )$ by definition 

$$
2) \implies P (t, T) = \exp \{- y (t, T) (T - t) \}
$$

$$
f (t, T) = y (t, T) + (T - t) \frac {\partial}{\partial T} y (t, T)\tag{1}
$$

$$
3) \implies P (t, T) = \exp \left\{- \int_ {t} ^ {T} f (t, u) d u \right\}
$$

$$
y (t, T) = \frac {1}{T - t} \int_ {t} ^ {T} f (t, u) d u.
$$

Hence the term structure up to time $T ^ { * }$ is completely described by any of the following families: 

$$
\left(\mathrm{i}\right) \left\{P (t, T) \mid 0 \leq T \leq T ^ {*}, 0 \leq t \leq T \right\}
$$

$$
\left(\mathrm{ii}\right) \left\{y (t, T) \mid 0 \leq T \leq T ^ {*}, 0 \leq t \leq T \right\}
$$

$$
\text {(iii)} \left\{f (t, T) \mid 0 \leq T \leq T ^ {*}, 0 \leq t \leq T \right\}.
$$

For fixed t, $T \longrightarrow P ( t , T ) ~ , ~ t \leq T \leq T ^ { * }$ is a (smooth) curve of bond prices at t with diferent maturities. 

For fixed T, $t \longrightarrow P ( t , T )$ is the (stochastic) price process of a bond maturing at T. 

This is illustrated in the diagrams of Fig. 5.1 on page 98. 

Bond prices now (t = 0) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/ebdb82306ce52614ca4a9b63810df6ee1632efea90efec61a8635acd0f140bc7.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/c41c23c3662cafd5f12d26c7ae1a71196459c07a1e2bf87decbb087ceaa6428a.jpg)



Price of a bond maturing at $T ^ { * }$



Similar for y(t, T)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/768579290ac736a45132634c3303743dff4da5f419c61dbf6e093f741c30c226.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/7ecadb6e570405be9f6ebe8573df93fc2c81e5cbbd180226bc6e8dea071faedd.jpg)



and for f(t, T)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/89fb3669efaf340e48c80a19817d3e51f6a9ba5471a9bb34ddafb1f4198c94d0.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/96e0d3fe7d45802f86a5bf7e3e48aeab44b5b7593de2017485d569b1cf6c6a8c.jpg)



Fig. 5.1. Diferent descriptions of the Term Structure


From (1) it follows 

$$
f (t, T) \left( \begin{array}{c} > \\ = \\ <   \end{array} \right) y (t, T) \Longleftrightarrow \text { yield   curve   is } \left( \begin{array}{c} \text { rising } \\ \text { flat } \\ \text { falling } \end{array} \right)
$$

In particular, the relation (1) implies: the longer the maturity T, the more sensitive $f ( t , T )$ reacts to twists in the yield curve. 

Definition 5.1.1. The instantaneous spot rate is defined by 

$$
r (t) = f (t, t) = - \frac {\partial}{\partial T} (\log P (t, T)) _ {T = t}.
$$

## 5.2 Stochastics of the Term Structure

Again we assume that there are d independent stochastic factors modelled by a d-dimensional Brownian motion. 

$$
B _ {t} = (B _ {t} ^ {1}, \ldots , B _ {t} ^ {d}) \quad \mathrm{on} (\varOmega , (\mathcal {F} _ {t}) _ {0 \leq t \leq T ^ {*}}, P)
$$

satisfying the usual conditions. 

For each $T \leq T ^ { * }$ , consider the “asset” $X _ { t } ^ { T } = P ( t , T )$ . As before we assume that, for any $0 \leq T \leq T ^ { * }$ 

$$
\frac {d P (t , T)}{P (t , T)} = \mu (t, T) d t + \underbrace {\sigma (t , T) \circ d B _ {t}} _ {\text { scalar   product   in } \mathbb {R} ^ {d}} 0 \leq t \leq T
$$

with $\mu ( t , T ) , \ \sigma ( t , T )$ adapted processes, satisfying boundary conditions as defined in Sect. 4.1 . 

Thus we have a continuum of “assets”, whose dynamics are given by Borel-measurable mappings 

$$
\mu : C \times \Omega \longrightarrow \mathbb {R}, \sigma : C \times \Omega \longrightarrow \mathbb {R} ^ {d}
$$

with 

$$
C = \left\{(t, T): 0 \leq t \leq T \leq T ^ {*} \right\}.
$$

Assumption 5.2.1. (No-arbitrage) 

There exists a d-dimensional adapted process $\lambda ( t ) _ { 0 \leq t \leq T ^ { \ } }$ with 

$$
E \Big [ \exp \left\{\frac {1}{2} \int_ {0} ^ {T ^ {*}} | | \lambda (s) | | ^ {2} d s \right\} \Big ] <   \infty
$$

such that, for all $0 \leq t \leq T \leq T ^ { * }$ 

$$
\begin{array}{l} \mu (t, T) = r (t) + \lambda (t) \circ \sigma (t, T) \\ \qquad = r (t) + \sum_ {i = 1} ^ {d} \lambda_ {i} (t) \sigma_ {i} (t, T). \end{array}
$$

## Remark 5.1.

(1) As shown in Sect. 4.1, no arbitrage implies that the risk price process is the same for all “assets”, i.e. does not depend on the maturity T. 

(2) Since there is now a continuum of assets, but only d factors, NA imposes restrictions on the drift terms $\mu ( t , T )$ (term structure models with finitely many factors are $\cdots o v e r ^ { 3 } - c o m p l e t e )$ 

(3) $\lambda ( t )$ can be interpreted as a risk premium for long term investments, since 

$$
E \Big [ \frac {d P (t , T)}{P (t , T)} \mid \mathcal {F} _ {t} \Big ] = r (t) d t + \underbrace {\lambda (t) \circ \sigma (t , T) d t} _ {e x c e s s r e t u r n}.
$$

As before Girsanov’s theorem allows us to eliminate $\lambda ( t )$ as follows: 

$$
L _ {t} := - \int_ {0} ^ {t} \lambda (s) \circ d B _ {s}
$$

$$
P ^ {*} = \mathcal {E} (L _ {T ^ {*}}) P P ^ {*} \sim P \mathrm{on} \mathcal {F} _ {T ^ {*}}
$$

$$
B _ {t} ^ {*} = B _ {t} + \int_ {0} ^ {t} \lambda (s) d s \quad \mathrm{BMunder} P ^ {*}
$$

$$
\Longrightarrow \frac {d P (t , T)}{P (t , T)} = r (t) d t + \sigma (t, T) \circ d B _ {t} ^ {*} \quad 0 \leq t \leq T \leq T ^ {*}
$$

$$
\Longrightarrow E _ {P ^ {*}} \Big [ \frac {d P (t , T)}{P (t , T)} \mid \mathcal {F} _ {t} \Big ] = r (t) d t \quad (\mathrm{LocalExpectationHypothesis}).
$$

Again let 

$$
\beta (t) = \exp \left\{\int_ {0} ^ {t} r (s) d s \right\}
$$

be the accumulation factor (rolling over at the spot $\operatorname { r a t e } ) = s p o t ~ n u -$ meraire. 

As in Chap. 4 it follows, that the discounted price processes are martingales under $P ^ { * }$ , i.e. 

$$
\hat {P} (t, T) = \frac {P (t , T)}{\beta (t)}
$$

has dynamics 

$$
\frac {d \hat {P} (t , T)}{\hat {P} (t , T)} = \sigma (t, T) \circ d B _ {t} ^ {*} \quad \forall 0 \leq t \leq T \leq T ^ {*}.
$$

More generally, for any Itˆo-Process $( Z _ { t } ) _ { 0 \le t \le T \le T ^ { * } } \mathrm { o n } \left( \Omega , ( { \mathcal { F } } _ { t } ) , P \right)$ , which is of the form 17 

$$
\frac {d Z _ {t}}{Z _ {t}} = \mu_ {Z} (t) d t + \sigma_ {Z} (t) \circ d B _ {t}
$$

we have for $\hat { Z } _ { t } = \frac { Z _ { t } } { \beta _ { t } }$ 

$$
\frac {d \hat {Z} _ {t}}{\hat {Z} _ {t}} = \sigma_ {Z} (t) \circ d B _ {t} ^ {*} \quad \mathrm{under} P ^ {*}
$$

which again implies the Fundamental Pricing Rule: 

$$
Z _ {t} = E ^ {*} \Big [ \exp \left\{- \int_ {t} ^ {T} r (s) d s \right\} Z _ {T} \Big | \mathcal {F} _ {t} \Big ] = \beta_ {t} E ^ {*} [ \hat {Z} _ {T} | \mathcal {F} _ {t} ] \forall 0 \leq t \leq T \leq T ^ {*}
$$

In particular, for any contingent claim $H _ { T }$ which is ${ \mathcal { F } } _ { T }$ -measurable (and thus may depend on the whole term structure up to time $T )$ , we have : 

$$
H _ {t} = \beta_ {t} E ^ {*} \Big [ \frac {H _ {T}}{\beta_ {T}} \Big | \mathcal {F} _ {t} \Big ] = P (t, T) E _ {T} [ H _ {T} | \mathcal {F} _ {t} ],
$$

where $E _ { T }$ is the expectation w.r.t. the forward measure 

$$
P _ {T} = E ^ {*} [ (\beta_ {T} P (0, T)) ^ {- 1} | \mathcal {F} _ {t} ] P ^ {*} \mathrm{on} \mathcal {F} _ {t}
$$

i.e. $P _ { T }$ is the martingale measure with $\textstyle P ( t , T )$ as numeraire (see Sect. 4.8). 

## 5.3 The HJM-Model

We have completely described the term structure by taking the zerobonds as building blocks. As we have seen all results, as derived in Chap. 4 for asset prices and their derivatives, carry over to describe the stochastic nature of the term structure. However, the term structure is usually described by interest rates instead of bond prices, e.g. by the movements of the yield curve or the forward rate curve. 

Therefore HJM start with modelling the dynamics of the forward rates $f ( t , T )$ and assume that 

$$
d f (t, T) = \alpha (t, T) d t + \underbrace {\tau (t , T) \circ d B _ {t}} _ {\text {scalar product in} \mathbb {R} ^ {d}} 0 \leq t \leq T \leq T ^ {*}
$$

under the same conditions as in Sect. 5.2. Since the dynamics of the term structure is already completely described by the dynamics of $\textstyle P ( t , T )$ , all what remains to do is to reveal the implied dynamics for the forward rates $f ( t , T )$ 

For the technical conditions on the processes α and $\tau$ needed for a mathematical rigorous derivation of the HJM-model (in particular conditions allowing the change of stochastic diferentiation and integration) we refer to Heath-Jarrow-Morton (1992). 

Again, since there is a continuum of rates but only finitely many factors, the drift terms $\alpha ( t , T )$ must satisfy certain restrictions for the model to be consistent. 

Theorem 5.3.1. No arbitrage implies the existence of an adapted process $\lambda ( t )$ such that, for any $0 \leq t \leq T \leq T ^ { * }$ 

$$
\alpha (t, T) = \tau (t, T) \circ (\lambda (t) - \sigma (t, T))\tag{2}
$$

where 

$$
\sigma (t, T) = - \int_ {t} ^ {T} \tau (t, u) d u.
$$

Proof. We have the following relations between $f ( t , T )$ and $\textstyle P ( t , T )$ : 

$$
\ln P (t, T) = - \int_ {t} ^ {T} f (t, u) d u
$$

$$
f (t, T) = - \frac {\partial}{\partial T} \ln P (t, T).
$$

No arbitrage (see Sect. 4.1 and 5.2) implies the existence of a risk price process $\lambda ( t )$ , which is independent of $T$ , with 

$$
E \left[ \frac {d P (t , T)}{P (t , T)} | \mathcal {F} _ {t} \right] = r (t) d t + \lambda (t) \circ \sigma (t, T) d t
$$

where $\sigma ( t , T )$ is the volatility of $\textstyle P ( t , T )$ . By Itˆo 

$$
\begin{array}{l} d \ln P (t, T) = \frac {d P (t , T)}{P (t , T)} - \frac {1}{2} \frac {1}{P (t , T) ^ {2}} d \langle P (t, T) \rangle_ {t} \\ \qquad = \left(r (t) + \lambda (t) \circ \sigma (t, T) - \frac {1}{2} | | \sigma (t, T) | | ^ {2}\right) d t + \sigma (t, T) \circ d B _ {t}. \end{array}
$$

The crucial step now is that the HJM conditions allow changing differentials. In doing so it follows: 

$$
\begin{array}{l} d f (t, T) = - \frac {\partial}{\partial T} d \ln P (t, T) \\ \qquad = - \Big (\lambda (t) \frac {\partial}{\partial T} \sigma (t, T) - \sigma (t, T) \frac {\partial}{\partial T} \sigma (t, T) \Big) d t - \underbrace {\frac {\partial}{\partial T} \sigma (t , T)} _ {:= \tau (t, T)} d B _ {t}. \end{array}
$$

Hence 

$$
\alpha (t, T) = \lambda (t) \circ \tau (t, T) - \sigma (t, T) \circ \tau (t, T)
$$

and 

$$
\sigma (t, T) = - \int_ {t} ^ {T} \tau (t, u) d u.
$$

□ 

The relation (2) allows again the elimination of the risk process $\lambda ( t )$ (which is the same for $f ( t , T )$ and $\textstyle P ( t , T ) )$ by Girsanov. 

Since we have already done this change of measure from $P$ to $P ^ { * }$ for the bond prices, we can directly derive the dynamics of $f ( t , T )$ under $P ^ { * }$ by the same technique as above. 

Theorem 5.3.2. (HJM) 

Under $P ^ { * }$ the dynamics of $f ( t , T )$ is 

$$
d f (t, T) = \left(\tau (t, T) \circ \int_ {t} ^ {T} \tau (t, u) d u\right) d t + \tau (t, T) \circ d B _ {t} ^ {*}.
$$

Proof. Follows from 

$$
d \ln P (t, T) = \left(r (t) - \frac {1}{2} | | \sigma (t, T) | | ^ {2}\right) d t + \sigma (t, T) \circ d B _ {t} ^ {*}
$$

and 

$$
\sigma (t, T) = - \int_ {t} ^ {T} \tau (t, u) d u.
$$

□ 

Hence forward rates and spot rates under the (spot) martingale measure $P ^ { * }$ are given by 

$$
\begin{array}{l} f (t, T) = f (0, T) - \int_ {0} ^ {t} \tau (s, T) \circ \sigma (s, T) d s + \int_ {0} ^ {t} \tau (s, T) \circ d B _ {s} ^ {*} \\ r (t) = f (0, t) - \int_ {0} ^ {t} \tau (s, t) \circ \sigma (s, t) d s + \int_ {0} ^ {t} \tau (s, t) \circ d B _ {s} ^ {*}, \quad \text {where} \\ \sigma (s, T) = - \int_ {s} ^ {T} \tau (s, u) d u. \end{array}
$$

Attention: Observe that the volatility $\tau$ of the forward rates and the volatility $\sigma$ of the zerobonds have opposite signs, since both depend on the same Brownian motion. Hence, if forward rates move up, zerobond prices move down, and vice versa. 

## 5.4 Examples

Literature: Ho-Lee (1986), Vasicek (1977), Musiela-Rutkowski (1997). 

## 1. Ho-Lee Model

$$
d = 1 \quad \tau (t, T) = \tau > 0 \quad \forall t, T
$$

$$
\Longrightarrow d f (t, T) = \alpha (t, T) + \tau d B _ {t}
$$

No arbitrage $\longleftrightarrow _ { \mathrm { T h e o r e m ~ 5 . 3 . 1 } } \alpha ( t , T ) = \tau \lambda ( t ) + \tau ^ { 2 } ( T - t ) \ .$ 

$$
\begin{array}{r l} & {5. 3. 2 \implies d f (t, T) = \tau^ {2} (T - t) d t + \tau d B _ {t} ^ {*}} \\ & {\qquad \qquad f (t, T) = f (0, T) + \tau^ {2} \int_ {0} ^ {t} (T - s) d s + \tau B _ {t} ^ {*}} \\ & {\qquad \qquad = f (0, T) + \tau^ {2} t (T - \frac {t}{2}) + \tau B _ {t} ^ {*}} \\ & {\qquad r (t) = f (t, t) = f (0, t) + \frac {1}{2} \tau^ {2} t ^ {2} + \tau B _ {t} ^ {*}.} \end{array}\tag{\(f(t,T)\}
$$

f(0, T) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/4f1ac91e0f90b9ae8481dd6a62737d7d1b57808e6334988a73b66442ab1de304.jpg)


Ho-Lee turns any (flat) initial forward curve into an upward sloping curve at t . 

Dynamics of $\textstyle P ( t , T )$ of the Ho-Lee model: 

$$
\begin{array}{r l} & {\frac {d P (t , T)}{P (t , T)} = r (t) d t + \sigma (t, T) d B _ {t} ^ {*}} \\ & {\qquad = \left(f (0, t) + \frac {1}{2} \tau^ {2} t ^ {2} + \tau B _ {t} ^ {*}\right) d t - \tau (T - t) d B _ {t} ^ {*}.} \end{array}\tag{3}
$$

Proposition 5.4.1. 

$$
P (t, T) = \frac {P (0 , T)}{P (0 , t)} \exp \Big \{- \frac {1}{2} \tau^ {2} (T - t) T t - \tau (T - t) B _ {t} ^ {*} \Big \}.
$$

Proof. To show 

$$
P (t, T) = P (0, T) e ^ {X _ {t}}
$$

with 

$$
X _ {t} = \int_ {0} ^ {t} f (0, s) d s - \frac {1}{2} \tau^ {2} (T - t) T t - \tau (T - t) B _ {t} ^ {*}
$$

is the solution of (3). 

Itˆo’s formula implies: 

$$
\begin{array}{c} d P (t, T) = P (0, T) \left(e ^ {X _ {t}} d X _ {t} + \frac {1}{2} e ^ {X _ {t}} d \langle X \rangle_ {t}\right) \\ = P (t, T) \left(d X _ {t} + \frac {1}{2} d \langle X \rangle_ {t}\right) \end{array}
$$

$$
\begin{array}{l} d X _ {t} = f (0, t) d t - \frac {1}{2} \tau^ {2} (\underbrace {- T t + (T - t) T} _ {(T - t) ^ {2} - t ^ {2}}) d t + \tau B _ {t} ^ {*} d t - \tau (T - t) d B _ {t} ^ {*} \\ = \left(f (0, t) + \frac {1}{2} \tau^ {2} t ^ {2} + \tau B _ {t} ^ {*}\right) d t - \frac {1}{2} \underbrace {\tau^ {2} (T - t) ^ {2} d t} _ {d \langle X \rangle_ {t}} - \tau (T - t) d B _ {t} ^ {*} \\ \implies \frac {d P (t , T)}{P (t , T)} = r (t) d t - \tau (T - t) d B _ {t} ^ {*}. \end{array}
$$

 

## 2. Vasicek-Model

$$
\begin{array}{l} d = 1 \quad \tau (t, T) = \tau e ^ {- \alpha (T - t)} \quad \alpha , \tau > 0 \text {fixed} \\ \implies \sigma (t, T) = - \int_ {t} ^ {T} \tau (t, u) d u = \frac {\tau}{\alpha} \left(e ^ {- \alpha (T - t)} - 1\right). \end{array}
$$

$$
\begin{array}{r l} \mathrm{HJM} \longrightarrow d f (t, T) & = - \tau (t, T) \sigma (t, T) d t + \tau (t, T) d B _ {t} ^ {*} \\ & = \frac {\tau^ {2}}{\alpha} e ^ {- \alpha (T - t)} \left(1 - e ^ {- \alpha (T - t)}\right) d t + \tau e ^ {- \alpha (T - t)} d B _ {t} ^ {*} \\ & = \tau e ^ {- \alpha (T - t)} \left(- \frac {\tau}{\alpha} \left(e ^ {- \alpha (T - t)} - 1\right) d t + d B _ {t} ^ {*}\right). \end{array}
$$

$$
\frac {d P (t , T)}{P (t , T)} = r (t) d t - \frac {\tau}{\alpha} \left(1 - e ^ {- \alpha (T - t)}\right) d B _ {t} ^ {*}
$$

It can be shown (see e.g. Musiela-Rutkowski (1997) Chapt.13) that the short rate is of the form 

$$
d r (t) = \left(a (t) - \alpha r (t)\right) d t + \tau d B _ {t} ^ {*} (\mathrm{Ornstein-Uhlenbeckprocess})
$$

## 5.5 The “LIBOR Market” Model

Literature: see introduction to Chapter $5$ . 

Starting point are market rates (e.g. LIBOR = ”London Inter-Bank Ofer $\mathrm { R a t e } ^ { \prime \prime } )$ 

$f ( t , T , \delta ) = \mathrm { n o m i n a l }$ rate at t for period $[ T , T + \delta ] , \delta > 0$ 

$\delta = 0 . 2 5 \longrightarrow f ( t , T , \delta ) = 3 $ -month forward LIBOR rate 

Assumption 5.5.1. (MSS) 

$$
\frac {d f (t , T , \delta)}{f (t , T , \delta)} = \mu (t, T) d t + \gamma (t, T) \circ d B _ {t}.
$$

Corresponding HJM-Model 

$$
d P (t, T) = P (t, T) \left(r (t) + \sigma (t, T) \circ d B ^ {*} (t)\right)
$$

$$
\begin{array}{c} d f (t, T, d t) = - \tau (t, T) \circ \sigma (t, T) d t + \tau (t, T) \circ d B ^ {*} (t) \\ \sigma (t, T) = - \int_ {t} ^ {T} \tau (t, u) d u. \end{array}
$$

Switching to the forward measure by choosing $\textstyle P ( t , T )$ as numeraire (see Sect. 4.8 and 5.2), we get that 

$$
B _ {T} ^ {*} (t) = B ^ {*} (t) + \int_ {0} ^ {t} \sigma (s, T) d s
$$

is Brownian motion under the forward measure 

$$
P _ {T} = \mathcal {E} (L _ {T}) P ^ {*} \quad \text { with } \quad L _ {T} (t) = - \int_ {0} ^ {t} \sigma (s, T) \circ d B ^ {*} (s).
$$

The connection between the rates $f ( t , T , \delta )$ and $\textstyle P ( t , T )$ is given by the forward contracts 

$$
F (t, T, \delta) := \frac {P (t , T + \delta)}{P (t , T)} = \left[ 1 + \delta f (t, T, \delta) \right] ^ {- 1}.
$$

Proposition 5.5.2. 

$$
\begin{array}{l} \frac {d F (t , T , \delta)}{F (t , T , \delta)} = (\sigma (t, T) - \sigma (t, T + \delta)) \circ d B _ {T} ^ {*} (t) \\ = - \Big (\int_ {T} ^ {T + \delta} \tau (t, u) d u \Big) \circ d B _ {T} ^ {*} (t). \end{array}
$$

Proof. Set $X = P ( t , T + \delta )$ and $Y = P ( t , T )$ . Then Itˆo implies 

$$
\begin{array}{l} \frac {d (X Y ^ {- 1})}{X Y ^ {- 1}} = \big (\mu_ {X} - \mu_ {Y} + \sigma_ {Y} \circ (\sigma_ {Y} - \sigma_ {X}) \big) d t + (\sigma_ {X} - \sigma_ {Y}) \circ d B ^ {*} (t) \\ \qquad = \Big (r (t) - r (t) + \sigma (t, T) \circ (\sigma (t, T) - \sigma (t, T + \delta)) \Big) d t \\ \qquad + \Big (\sigma (t, T) - \sigma (t, T + \delta) \Big) \circ d B ^ {*} (t) \\ \qquad = \Big (\sigma (t, T) - \sigma (t, T + \delta) \Big) \circ (\underbrace {d B ^ {*} (t) + \sigma (t , T) d t} _ {d B _ {T} ^ {*} (t)}. \end{array}
$$

 

Theorem 5.5.3. The relation between the volatilities $\gamma ( t , T )$ and $\sigma ( t , T )$ is given $b y$ 

$$
\sigma (t, T + \delta) = \sigma (t, T) + \frac {\delta f (t , T , \delta)}{1 + \delta f (t , T , \delta)} \cdot \gamma (t, T).
$$

Proof. Since Girsanov does not change volatilities we have from the MSS-assumption 

$$
d f (t, T, \delta) = \dots d t + f (t, T, \delta) \cdot \gamma (t, T) \circ d B ^ {*} (t).
$$

By Itˆo this implies 

$$
d F (t, T, \delta) = d (1 + \delta f) ^ {- 1} = - F ^ {2} \delta d f - \frac {1}{2} F ^ {3} d \langle f \rangle .
$$

Hence 

$$
\begin{array}{c} \frac {d F (t , T \delta)}{F (t , T , \delta)} = - F   \delta   f   \gamma (t, T)   \circ d B ^ {*} (t) + \ldots d t \\ = - \frac {\delta   f}{1 + \delta   f}   \gamma (t, T) \circ d B ^ {*} (t) + \ldots d t. \end{array}
$$

By Prop. 5.5.2 we have 

$$
\frac {d F (t , T , \delta)}{F (t , T , \delta)} = (\sigma (t, T) - \sigma (t, T + \delta)) \circ d B _ {T} ^ {*} (t).
$$

Since Girsanov does not change the difusion coeficients, we get the result by comparison of volatilities. 

 

Remark 5.2. The HJM-volatilities are no longer deterministic (even $i f$ the $\gamma ( t , T )$ are assumed as deterministic), since they depend on $f ( t , T , \delta )$ , i.e. 

$$
\sigma (t, T + \delta , \omega) = \sigma (t, T, f (t, T, \delta) (\omega)).
$$

Starting with $\sigma ( 0 , T ) = 0$ and $f ( 0 , T , \delta ) , \ T = 0 , \delta , 2 \delta , . . . ,$ they can be computed pathwise by a binomial lattice. 

Theorem 5.5.4. 

$$
\frac {d f (t , T , \delta)}{f (t , T , \delta)} = \gamma (t, T) \circ d B _ {T + \delta} ^ {*} (t).
$$

Proof. 

$$
\begin{array}{l} (1 + \delta f (t, T, \delta)) ^ {- 1} = F (t, T, T + \delta) = \frac {P (t , T + \delta)}{P (t , T)} \\ \Longrightarrow f = \frac {1}{\delta} \Big (\frac {P (t , T)}{P (t , T + \delta)} - 1 \Big). \end{array}
$$

Take $P ( t , T + \delta )$ as numeraire 

$$
\implies \frac {P (t , T)}{P (t , T + \delta)} \text {   is   a   martingale   under   } B _ {T + \delta} ^ {*}
$$

= f and $d f / f$ are martingales under $B _ { T + \delta } ^ { * }$ 

$$
\implies d f = f \cdot \gamma (t, T) \circ d B _ {T + \delta} ^ {*}.
$$

## The Market Caplet Formula

A “caplet” is defined as the payof 

$$
C = \delta (f (T, T, \delta) - K) ^ {+}
$$

payable at $T + \delta .$ 

By the Fundamental Pricing Rule we have 

$$
\begin{array}{r l} & C _ {t} = \beta_ {t} E ^ {*} \Big [ \frac {C}{\beta_ {T + \delta}} \Big | \mathcal {F} _ {t} \Big ] \\ & \quad = \delta P (t, T + \delta) E _ {T + \delta} [ (f - K) ^ {+} | \mathcal {F} _ {t} ]. \end{array}
$$

Since $\frac { d f } { f } = \gamma ( t , T ) \circ d B _ { T + \delta } ^ { \ast }$ is a lognormal martingale under $P _ { T + \delta }$ $E _ { T + \delta } [ ( f - K ) ^ { + } ]$ is the Black-Scholes formula for the call $( f - K ) ^ { + }$ 

Hence 

$$
C _ {t} = \delta P (t, T + \delta) \left[ f (t, T, \delta) \Phi (d _ {1}) - K \Phi (d _ {2}) \right]
$$

$$
d _ {1, 2} (t) = \frac {1}{\eta (t , T)} \left(\ln \frac {f (t , T , \delta)}{K} \pm \frac {1}{2} \eta^ {2} (t, T)\right)
$$

$$
\eta^ {2} (t, T) = \int_ {t} ^ {T} \gamma^ {2} (s, T) d s.
$$

For a “floorlet” $F = \delta [ K - f ( t , T , \delta ) ] ^ { + }$ one obtains by the same method: 

$$
F _ {t} = \delta P (t, T + \delta) \left[ K \Phi (- d _ {2}) - f (t, T \delta) \Phi (- d _ {1}) \right].
$$

## 5.6 Caps, Floors and Swaps

Consider a sequence $\mathcal { T } = \{ T _ { 0 } < T _ { 1 } < . . . < T _ { n } \}$ of payment dates. 

Let $L ( t , T _ { i } )$ denote the forward LIBOR rate for $[ T _ { i } , T _ { i + 1 } ]$ , valid at $t ~ , ~ t \leq T _ { 0 } ~ , ~ ( i = 0 , \ldots , n - 1 )$ 

Set $\delta _ { i } = T _ { i + 1 } - T _ { i }$ 

E.g.: 3-month LIBOR rates $\implies \delta _ { i } \approx 0 . 2 5$ (varies with calendar) 

Definition 5.6.1. A cap at cap-rate K on $L ( t , T _ { i } )$ is a collection of caplets of the form 

$$
C (K, \mathcal {T}) = \left\{\delta_ {i} [ L _ {i} - K ] ^ {+}, \quad i = 0 \dots n - 1 \right\}
$$

which pays the amount $\delta _ { i } ~ [ L ( T _ { i } , T _ { i } ) - K ] ^ { + }$ at each $T _ { i + 1 }$ (payment in arrear) resp. $P ( T _ { i } , T _ { i + 1 } ) ~ \delta _ { i } ~ [ L _ { i } - K ] ^ { + } ~ a t ~ T _ { i }$ 

Similarly a floor on $L ( t , T _ { i } )$ is given by 

$$
F (K, \mathcal {T}) = \left\{\delta_ {i} [ K - L _ {i} ] ^ {+}, \quad i = 0 \dots n - 1 \right\}.
$$

A swap at rate K is a sequence of payments 

$$
\operatorname{Swap} (K, \mathcal {T}) = \left\{\delta_ {i} (L _ {i} - K), \quad i = 0 \dots n - 1 \right\}
$$

at each $T _ { i + 1 }$ (arrear swap). 

Let $C _ { t } ( K ) , F _ { t } ( K ) , S _ { t } ( K )$ denote the price of these instruments at time $t \leq T _ { 0 }$ 

The relation $a - b = [ a - b ] ^ { + } - [ b - a ] ^ { + }$ immediately gives the Cap-Floor relation 

$$
C _ {t} (K) = F _ {t} (K) + S _ {t} (K).
$$

With the preceding result on caplets we obtain 

$$
\begin{array}{c} C _ {t} (K) = \sum_ {i = 0} ^ {n - 1} \delta_ {i} P (t, T _ {i + 1}) \left(L (t, T _ {i}) \Phi (d _ {1} (t, T _ {i})) - K \Phi (d _ {2} (t, T _ {i}))\right) \\ d _ {1, 2} (t, T _ {i}) = \frac {1}{\eta (t , T)} \left(\ln \frac {L (t , T)}{K} \pm \frac {1}{2} \eta^ {2} (t, T)\right) \\ \eta^ {2} (t, T) = \int_ {t} ^ {T} \gamma^ {2} (s, T) d s. \end{array}
$$

The price of a (forward) swap at t is given by 

$$
\begin{array}{l} S _ {t} (K) = \sum_ {i = 0} ^ {n - 1} \delta_ {i} P (t, T _ {i + 1}) L (t, T _ {i}) - \sum_ {i = 0} ^ {n - 1} \delta_ {i} K P (t, T _ {i + 1}) \\ = P (t, T _ {0}) - \Big (\underbrace {P (t , T _ {n}) + \sum_ {i = 1} ^ {n} P (t , T _ {i}) K (T _ {i} - T _ {i - 1})} _ {\text {Coupon bond with coupon = K}} \Big). \end{array}
$$

The “forward swap rate” $K ~ = ~ K ( t , { \mathcal { T } } )$ is defined by the equation $S _ { t } ( K ) = 0$ . This gives 

$$
K (t, \mathcal {T}) = (P (t, T _ {0}) - P (t, T _ {n})) \left(\sum_ {i = 1} ^ {n} \delta_ {i - 1} P (t, T _ {i})\right) ^ {- 1}.
$$

The “swap rate” $K ( T _ { 0 } , T )$ is the rate which assigns a zero price to a swap starting at $T _ { 0 }$ . Hence 

$$
\begin{array}{c} K (T _ {0}, \mathcal {T}) = 0 \Longleftrightarrow \sum_ {i = 1} ^ {n} P (T _ {0}, T _ {i}) K (T _ {i} - T _ {i - 1}) + P (T _ {0}, T _ {n}) = 1 \\ \Longleftrightarrow \operatorname{CB} (K, \mathcal {T}) = 1. \end{array}
$$

I.e. the swap rate is equal to the coupon rate of a coupon bond (with payment dates $\tau )$ quoted at $\mathrm { ^ { 6 6 } p a r i ^ { \circ } }$ 

# Why Do We Need Itˆo-Calculus in Finance?

As pointed out in Sect. 2.1, Itˆo’s calculus is a necessary extension of real analysis to cope with functions of unbounded variation. Thus the question, whether we need stochastic calculus in finance, is tantamount to the question: are charts of stock prices, exchange or interest rates, in reality of unbounded variation? Such functions, like the Weierstraß function or a path of the Brownian motion, are pure mathematical constructs. Nobody can draw the graph of such a function, and even a computer can only give an approximate picture <sup>1</sup>. Why should such constructs represent what happens on the exchange markets? 

The answer is given by contradiction. Let us assume that stock price movements are in reality of finite variation. Then clever people could make huge arbitrage profits by generating options, which are traded in the market at high premiums, at almost zero costs. Clearly a contradiction to reality! 

This chapter requires some deeper results of stochastic analysis, like lo cal times and generalized Itˆo formulas, taken from Carr-Jarrow (1990) and Revuz-Yor (1991). Section 6.4 should be of special interest to economists, since it presents another view on option pricing by means of Arrow-Debreu prices for contingent claims. 

## 6.1 The Buy-Sell-Paradox

## Literature: Carr-Jarrow (1990)

Let $( X _ { t } )$ be a security price process in an economy with a non-stochastic interest rate $r ( t )$ and bond price 

$$
P _ {t} (T) = \exp \left\{- \int_ {t} ^ {T} r (s) d s \right\} \mathrm{asnumeraire.}
$$

X<sub>t</sub> <sup>=</sup>⇒ <sup>F</sup>t <sup>=</sup> T-forward price. P<sub>t</sub>(T) 

For a call $C _ { T } = ( X _ { T } - K ) ^ { + }$ consider the following hedging strategy 

$$
\phi_ {t} (\omega) = \mathbf {1} _ {\{F _ {t} (\omega) > K \}} = \mathbf {1} _ {\{X _ {t} (\omega) > P _ {t} (T) \cdot K \}}
$$

This strategy is realized as follows: buy one share of the stock when up-crossing the strike price K, sell it when down-crossing the strike (see Fig. 6.1). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/6ac2004065e845c91583821b506af6336c02feca6a5e1c517dd1166ec5b79ad3.jpg)



Fig. 6.1. Buy-Sell strategy


$$
\begin{array}{c} \Longrightarrow V _ {t} (\phi) = \mathbf {1} _ {\{F _ {t} > K \}} \cdot F _ {t} - \mathbf {1} _ {\{F _ {t} > K \}} \cdot K \\ = \max \{F _ {t} - K, 0 \} = [ F _ {t} - K ] ^ {+} \end{array}
$$

$$
\Longrightarrow V _ {T} (\phi) = [ F _ {T} - K ] ^ {+} = [ X _ {T} - K ] ^ {+} = C _ {T}
$$

The hedging strategy $\phi$ is ”apparently” self-financing and generates $C _ { T }$ . Thus it follows: 

$$
C _ {0} ^ {T} = V _ {0} (\phi) = [ F _ {0} - K ] ^ {+} \quad \text {   initial   investment   in   } \mathbb {S} \text {   deliverable   at   } T
$$

$$
\Longrightarrow C _ {0} = P _ {0} (T) \cdot \underbrace {V _ {0} (\phi)} _ {C _ {0} ^ {T}} = [ X _ {0} - K \cdot P _ {0} (T) ] ^ {+} \quad \text { price   in   } \mathbb {S} \text {-today } .
$$

Thus for $X _ { 0 } \le K \cdot P _ { 0 } ( T ) \Longrightarrow$ the option at time $t = 0$ has price zero. 

This is paradoxical, since also “out-of-the-money” options have positive prices. To solve this paradox we need the concept of local times, which is studied in the next two sections. 

## 6.2 Local Times and Generalized Itˆo Formula

Literature: Revuz-Yor (1991), Chap. 6 

Let $B _ { t } ( \omega )$ be a the path of the (1-dimensional) Brownian motion. 

$I = [ a , b ] \subset \mathbb { R }$ ; λ Lebesgue measure on $\mathbb { R }$ 

Definition 6.2.1. 

$$
\Gamma_ {t} (I, \omega) := \int_ {0} ^ {t} \mathbf {1} _ {I} (B _ {s} (\omega)) d s = \lambda \{s \leq t: B _ {s} (\omega) \in I \}
$$

is called the “occupation time in I till time $t ^ { \dprime }$ (see Fig. 6.2 on p.116). 

For all $( t , \omega ) , ~ T _ { t } ( \cdot , \omega )$ defines a measure on the Borel sets $\boldsymbol { B }$ in $\mathbb { R }$ . 

$$
A \in \mathcal {B} \quad \lambda (A) = 0 \Longrightarrow \Gamma_ {t} (A) = 0 \quad P \text {-a.s.}
$$

$\bigoplus _ { \mathrm { b y } } \Gamma _ { t } ( \cdot , \omega )$ has density $L _ { t } ( x , \omega )$ w.r.t. the Lebesgue measure λ, given 

$$
\begin{array}{l} L _ {t} (x, \omega) = \lim _ {\epsilon \downarrow 0} \frac {1}{2 \epsilon}   \Gamma_ {t} (I _ {x} ^ {\epsilon}, \omega) = \lim _ {\epsilon \downarrow 0} \frac {1}{2 \epsilon}   \lambda \{s \leq t: | B _ {s} (\omega) - x | \leq \epsilon \} \\ = \text {``local time in x till t''} \end{array}
$$

where $I _ { x } ^ { \epsilon } = [ x - \epsilon , x + \epsilon ]$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/9a1d11df7f7e0f8f372cc686255dfeb2cd11e2cf6d3daebc60e74547e7fe8a37.jpg)



Fig. 6.2. Occupation time of the path in interval I


Consequence: $g : \mathbb { R } \longrightarrow \mathbb { R }$ measurable 

$$
\Longrightarrow \int_ {0} ^ {t} g (B _ {s} (\omega)) d s = \int_ {- \infty} ^ {\infty} g (x) L _ {t} (x, \omega) d x.\tag{1}
$$

Proof. As in Prop. 1.3.1 it sufices to consider, for any $A \epsilon B _ { \cdot }$ , the characteristic function $g = \mathbf { 1 } _ { A }$ 

$$
\int_ {0} ^ {t} \mathbf {1} _ {A} (B _ {s}) d s = \Gamma_ {t} (A, \omega) = \int_ {\mathbb {R}} \mathbf {1} _ {A} (x) \cdot L _ {t} (x) d x.
$$

□ 

## Generalized Itˆo formula for convex functions

Let $F : \mathbb { R } \longrightarrow \mathbb { R }$ be a convex function, i.e., 

$$
F (t x + (1 - t) y) \leq t F (x) + (1 - t) F (y) \text {   for   } 0 \leq t \leq 1
$$

$$
(\text { e.g.   } F (x) = [ x - a ] ^ {+}).
$$

Convexity $\Longrightarrow F$ is continuous, a.s. diferentiable, and one has 

$F _ { - } ^ { \prime } ( x ) = \operatorname* { l i m } _ { h \downarrow 0 } { \frac { F ( x ) - F ( x - h ) } { h } }$ the left derivative of $F _ { ; }$ , exists $\forall x$ 

$F _ { - } ^ { \prime } \in \mathrm { F V } \Longrightarrow F _ { - } ^ { \prime }$ defines a measure µ on (IR, ) by 

$$
\mu [ a, b) = \int_ {[ a, b)} d F _ {-} ^ {\prime} = F _ {-} ^ {\prime} (b) - F _ {-} ^ {\prime} (a).
$$

Notation: $\mu = F _ { - } ^ { \prime \prime } \cdot \lambda$ (2nd derivative measure of F) 

Remark 6.1. ${ \cal F } \in C ^ { 2 } \Longrightarrow \mu = { \cal F } ^ { \prime \prime } \cdot \lambda$ . For one has 

$$
\int_ {a} ^ {b} F ^ {\prime \prime} (x) d x = F _ {-} ^ {\prime} (b) - F _ {-} ^ {\prime} (a) =: \int_ {[ a, b)} \mu (d x).
$$

For $F ( x ) = [ x - a ] ^ { + }$ one has $F _ { - } ^ { \prime } ( x ) = { \binom { 0 x \leq a } { 1 x > a } }$ 

Thus for $g : R \longrightarrow R$ it follows 

$$
\int_ {\mathbb {R}} g (x) \mu (d x) = \int_ {\mathbb {R}} g (x) d F _ {-} ^ {\prime} (x) = g (a), \text {i.e.} d F _ {-} ^ {\prime} = \delta_ {a} \text {Dirac - measure in} a.
$$

Theorem 6.2.2. (Generalized Itˆo Formula for convex functions) Let $F : \mathbb { R } \longrightarrow \mathbb { R }$ be a convex function. Then one has 

$$
F (B _ {t}) = F (B _ {0}) + \int_ {0} ^ {t} F _ {-} ^ {\prime} (B _ {s}) d B _ {s} + \frac {1}{2} \int_ {- \infty} ^ {\infty} L _ {t} (x) \mu (d x)
$$

where $\mu = F _ { - } ^ { \prime \prime } \cdot \lambda$ (2nd derivative measure of $F )$ 1 

Remark 6.2. $F \in C ^ { 2 } \longrightarrow F _ { - } ^ { \prime } = F ^ { \prime } , \mu ( d x ) = F ^ { \prime \prime } ( x ) d x$ 

$$
\int_ {- \infty} ^ {\infty} L _ {t} (x) F ^ {\prime \prime} (x) d x = \int_ {(1)} ^ {t} F ^ {\prime \prime} (B _ {s}) d s
$$

= “classical” Itˆo formula. 

## Generalization to Semi-Martingales

Let X be a continuous semimartingale, $A \subset \mathbb { R }$ a Borel set. 

Definition 6.2.3. $\varGamma _ { t } ( A ) = \int _ { 0 } ^ { t } \mathbf { 1 } _ { A } ( X _ { s } ) \underbrace { d \langle X \rangle _ { s } } _ { \mathrm { i n t e r i o r ~ c l o c l } }$ k 

is called the “occupation time of X in A till $t ^ { \dprime }$ 

Clearly $T _ { t } ( A )$ is a continuous process with monotonically increasing paths. 

Proposition 6.2.4. There exits a family ofcontinuous, adapted, monotonically increasing processes $( L _ { t } ^ { a } ) _ { t \geq 0 , a \in \mathcal { R } }$ with 

$$
L _ {t} ^ {a} = \lim _ {\epsilon \downarrow 0} \frac {1}{2 \epsilon} \int_ {0} ^ {t} \mathbf {1} _ {\{| X _ {s} - a | \leq \epsilon \}} d \langle X \rangle_ {s}
$$

and 

$$
\Gamma_ {t} (A) = \int_ {A} L _ {t} ^ {a} d a.\tag{2}
$$

$L _ { t } ^ { a } = L _ { t } ^ { a } ( X ) ( \omega )$ is called the “local time of X in a till time $t ^ { \dprime }$ 

The above proposition implies: 

(2) $\implies \intop _ { 0 } ^ { t } g ( X _ { s } ) ~ d \langle X \rangle _ { s } = \intop _ { - \infty } ^ { \infty } g ( a ) ~ L _ { t } ^ { a } ~ d a$ for any real measurable function $g$ 

Corollary 6.2.5. $g \equiv 1 { \underset { ( 2 ) } { \longrightarrow } } \ \langle X \rangle _ { t } = \int _ { 0 } ^ { t } d \langle X \rangle _ { s } = \int _ { - \infty } ^ { \infty } L _ { t } ^ { a } ( X ) \ d a .$ 

$$
\Longrightarrow X \in \mathrm{FV} \Longrightarrow L _ {t} (X) \equiv 0.
$$

Let $U _ { t } ^ { \epsilon } ( a , \omega )$ denote the number of up-crossings by path $X _ { t } ( \omega )$ of the interval $[ a , a + \epsilon ]$ (see Fig. 6.3 on page 119). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/0a84c614b03ec191e30593a9eb8d57d18ef72abbd40a3570db2ca588e0f578d5.jpg)



Fig. 6.3. $U _ { t } ^ { \epsilon } ( a , \omega ) = \#$ up-crossings from $X _ { t } ( \omega )$ of the interval $[ a , a + \epsilon ]$


Proposition 6.2.6. (El-Karoui) 

$$
\lim _ {\epsilon \downarrow 0} 2 \epsilon U _ {t} ^ {\epsilon} (a, \omega) = L _ {t} ^ {a} (\omega) \quad P \text {-a.s.}
$$

Consequence: $L _ { t } ^ { a } ( \omega ) > 0 \implies$ the path $X ( \omega )$ crosses the a-line till time t infinitely often. 

Theorem 6.2.7. (Itˆo-Tanaka formula) 

Let X be a continuous semimartingale, F a real convex function. Then one has 

$$
F (X _ {t}) = F (X _ {0}) + \int_ {0} ^ {t} F _ {-} ^ {\prime} (X _ {s}) d X _ {s} + \frac {1}{2} \int_ {- \infty} ^ {\infty} L _ {t} ^ {a} (X) F _ {-} ^ {\prime \prime} (d a)
$$

with $F _ { - } ^ { \prime \prime } ( d a )$ 2nd derivative measure of F (Lebesgue-Stieltjes integral). 

Remark 6.3. For $F \in C ^ { 2 }$ it follows 

$$
F(X_{t}) = F(X_{0}) + \int \limits_{0}^{t}F^{\prime}(X_{s})  dX_{s} + \frac{1}{2}\underbrace{\int\limits_{\substack{\mathbb{R}\\ }}L_{t}^{a}(X)  F^{\prime\prime}(a)  da}_{\substack{= \int \limits_{(Rem.6.2)}^{t}F^{\prime \prime}(X_{s})  d\langle X\rangle_{s}}}
$$

## 6.3 Solution of the Buy-Sell-Paradox

$g ( x ) = ( x - K ) ^ { + }$ is a convex function. Thus according to the Itˆo-Tanaka formula : 

$$
g(F_{T}) = (F_{T} - K)^{+} = (F_{0} - K)^{+} + \underbrace{\int\limits_{0}^{T}g^{\prime}_{-}(F_{s})  dF_{s}}_{= \int \limits_{0}^{T}dV(\phi_{s})}\underbrace+\frac{1}{2}\int\limits_{-\infty}^{\infty}L_{t}^{a}(F)\underbrace{g^{\prime\prime}_{-}(da)}_{\text{(transaction costs)}}
$$

But for a process $\left( F _ { t } \right)$ of infinite variation, its local time $L _ { T } ^ { K }$ becomes positive, once it crosses the barrier K. Hence the “buy-sell” strategy is not self-financing ! 

The transaction costs ${ \begin{array} { l l } { { \frac { 1 } { 2 } } } & { L _ { T } ^ { K } ( F ) } \end{array} }$ , which by Prop. 6.2.6 are equal to $\operatorname* { l i m } _ { \epsilon \downarrow 0 } \epsilon \cdot U _ { T } ^ { \epsilon } ( K )$ , have a nice interpretation: 

Assume that one tries to apply the Buy-Sell strategy in order to hedge the payof $g ( F _ { T } ) = ( F _ { T } - K ) ^ { + }$ , i.e., buy the stock at price K when up-crossing the barrier K, sell it again when down-crossing the barrier. But you cannot sell it at the same price. You need a so-called “cutout”, you can place only limit orders of the form: buy at $K$ , sell at $K - \varepsilon$ for some $\varepsilon > 0$ . The smaller you choose $\varepsilon ,$ the more cutouts you will face, and in the limit the sum of these cutouts is just equal to the transaction costs (see Fig. 6.4 on p. 121) . 

Taking the expectation under the forward measure $P _ { T }$ , it follows: 

$$
F _ {T} \in \mathcal {M} (P _ {T}) \Longrightarrow C _ {0} ^ {T} = \mathrm{E} _ {T} [ (F _ {T} - K) ^ {+} ] = \underbrace {(F _ {0} - K) ^ {+}} _ {\text {IV}} + \underbrace {\mathrm{E} _ {T} \left[ \frac {1}{2} L _ {T} ^ {K} (F) \right]} _ {\text {TV in   } \mathbb {S} _ {\text {tomorrow}}}
$$

$$
\Longrightarrow C _ {0} = P _ {0} (T) \cdot C _ {0} ^ {T} = \underbrace {(X _ {0} - K \cdot P _ {0} (T)) ^ {+}} _ {\text {PIV}} + \underbrace {P _ {0} (T) \operatorname{E} _ {T} \left[ \frac {1}{2} L _ {T} ^ {K} \right] \quad \text {in}   t o d a y} _ {\text {PV of expected local time}}
$$

Here $\mathrm { \Delta \Omega ^ { \prime } I V ^ { \prime } }$ stands for “interior value” and ’TV’ for “time value”. The prefix $\mathbf { \overrightarrow { P } } ^ { \prime }$ means “present”. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/63ae5f37-c0ee-49da-aced-d63600fbe886/5f831728631e9019131671edb8f86c80030665fb34ba0d517a8c9bc18c96ccf2.jpg)



Fig. 6.4. Transaction costs caused by ‘cutouts‘ 


Remark 6.4. $( X _ { t } ) \in \mathrm { F V } \implies L _ { T } ^ { K } \equiv 0 \Longrightarrow T V = 0$ = out-of-the money options are worthless 

However, this contradicts what we observe on the option markets which attach a positive time value also to out-of-the-money options. Hence it follows: 

Consequence: = (X<sub>t</sub>) is of infinite variation ! = Itˆo is a ’must’ for Option Pricing 

## 6.4 Arrow-Debreu Prices in Finance

Let $Z _ { t } = ( X _ { t } , Y _ { t } ) _ { 0 \leq t \leq T }$ be two security price processes with $Y _ { t }$ as numeraire. 

$$
1) Y _ {t} = \beta_ {t} = e ^ {r t} \quad \text { numeraire:   -today }
$$

$$
2) Y _ {t} = P _ {t} (T) = e ^ {- r (T - t)} \quad \text {numeraire:   -tomorrow}
$$

$$
3) Y _ {t} \equiv 1 (\Longleftrightarrow r = 0) \quad \Longrightarrow - t o d a y \equiv - t o m o r r o w
$$

W.l.o.g. we can always assume that 3) holds by using the following transformations: 

$$
\widehat {Z} _ {t} = \left(\widehat {X} _ {t} = \frac {X _ {t}}{Y _ {t}}, 1\right) \quad ; \quad \widehat {H} = \frac {H}{Y _ {T}} \in \mathcal {F} _ {T} \quad \text { contingent   claim }
$$

$$
\widehat {V} _ {t} (\phi) = \frac {V _ {t} (\phi)}{Y _ {t}}, \widehat {H} _ {t} = \mathrm{E} ^ {*} [ \widehat {H} | \mathcal {F} _ {t} ]
$$

$$
H _ {t} = \widehat {H} _ {t} \cdot Y _ {t} \quad \mathrm{back-transformation}.
$$

Consider the following special contingent claim $H _ { t } ( x ) \in { \mathcal { F } } _ { t }$ 

$$
H _ {t} (x) = \mathbf {1} _ {\{X _ {t} \leq x \}} = \left\{ \begin{array}{l l} 1 & X _ {t} \leq x \\ 0 & X _ {t} > x \end{array} \right.
$$

(= Arrow-Debreu security contingent on value of X at time t). 

AD-price at $t = 0$ 

$$
\mathrm{AD} (t, x) = \mathrm{E} ^ {*} [ H _ {t} (x) ] = P ^ {*} [ X _ {t} \leq x ] = \text { distribution   of } X _ {t} \text { under } P ^ {*}.
$$

$\mathrm { A D } ( t , x )$ has density $f ( t , x )$ defined by $\begin{array} { r } { f ( t , x ) = \underset { \epsilon \downarrow 0 } { \operatorname* { l i m } } \frac { 1 } { 2 \epsilon } \operatorname { E } ^ { * } [ \mathbf { 1 } _ { \{ | X _ { t } - x | \leq \epsilon \} } ] , } \end{array}$ or 

$$
\begin{array}{r l} & f (t, x) d x = \mathrm{E} ^ {*} [ \mathbf {1} _ {I _ {x}} (X _ {t}) ] \quad \text {with} I _ {x} = (x - \frac {1}{2} d x, x + \frac {1}{2} d x) \\ & \qquad = \text {density of AD - prices, given} X _ {t} = x. \end{array}
$$

Let $C ( X _ { t } )$ be a contingent claim on $X _ { t }$ . According to Prop. 1.3.1 

$$
\Longrightarrow \pi_ {0} (C _ {t}) = E ^ {*} [ C (X _ {t}) ] = \int_ {- \infty} ^ {\infty} C (x) d P _ {X} ^ {*} (x) = \int_ {- \infty} ^ {\infty} C (x) f (t, x) d x.
$$

Example: $C ( t , K ) = ( X _ { t } - K ) ^ { + }$ Call $P ( t , K ) = ( K - X _ { t } ) ^ { + }$ Put 

By partial integration one obtains: 

$$
\pi_ {0} (C) = \int_ {K} ^ {\infty} (x - K) f (t, x) d x = \int_ {K} ^ {\infty} (1 - \mathrm{AD} (t, x)) d x
$$

$$
\pi_ {0} (P) = \int_ {0} ^ {K} (K - x) f (t, x) d x = \int_ {0} ^ {K} \mathrm{AD} (t, x) d x.\tag{3}
$$

Consequence: $\mathrm { A D } ( t , K ) = \frac { d } { d K } \pi _ { 0 } ( P ( t , K ) )$ 

$$
f (t, K) = \frac {\partial^ {2}}{\partial K ^ {2}} \pi_ {0} (P (t, K)) = \frac {\partial^ {2}}{\partial K ^ {2}} \pi_ {0} (C (t, K)).
$$

Interpretation of (3): Payof at t 

$$
\begin{array}{c} \int_ {0} ^ {K} H _ {t} (x) d x = \int_ {0} ^ {K} \mathbf {1} _ {\{X _ {t} \leq x \}} d x = \lambda \{0 \leq x \leq K: X _ {t} \leq x \} \\ = \left\{ \begin{array}{c c} K - X _ {t} & X _ {t} \leq K \\ 0 & X _ {t} > K. \end{array} \right. \end{array}
$$

Exercise: For the standard Black-Scholes model $( \mu , \sigma$ constant, $r = 0 )$ one has (compare Sect. 2.9 ): 

$\mathrm { A D } ( t , x ) = 1 - \varPhi ( h ( t , x ) ) = \varPhi ( - h ( t , x ) )$ with density $f ( t , x ) = { \frac { \varphi ( h ) } { x \sigma { \sqrt { t } } } }$ 

where $\varPhi ( \cdot )$ is the distribution function of $\mathrm { N } ( 0 , 1 ) , \varphi = \varPhi ^ { \prime }$ , and 

$$
h (t, x) = \frac {\ln (X _ {0} / x)}{\sigma \sqrt {t}} - \frac {1}{2} \sigma \sqrt {t}.
$$

## 6.5 The Time Value of an Option as Expected Local Time

As shown in Sect. 6.2, the local time of the process $X _ { t }$ in K till maturity $T$ is given by 

$$
L _ {T} ^ {K} (\omega) = \lim _ {\epsilon \downarrow 0} \frac {1}{2 \epsilon} \int_ {0} ^ {T} \mathbf {1} _ {\{| X _ {t} (\omega) - K | \leq \epsilon \}} d \langle X (\omega) \rangle_ {t}.
$$

Under suitable boundary conditions on $\mu _ { X } ( t ) , \sigma _ { X } ( t )$ one may commute limit and integration to obtain 

$$
\begin{array}{l} \Longrightarrow \frac {1}{2}   \mathrm{E} ^ {*} [ L _ {T} ^ {K} ] = \frac {1}{2}   \mathrm{E} ^ {*} \Big [ \int_ {0} ^ {T} \lim _ {\epsilon} \frac {1}{2 \epsilon}   \mathbf {1} _ {\{| X _ {t} - K | \leq \epsilon \}}   d \langle X \rangle_ {t} \Big ] \\ \qquad = \frac {1}{2}   \int_ {0} ^ {T} f (t, K)   d \langle X _ {t} \rangle_ {X _ {t} = K} \\ \qquad = \frac {1}{2} \cdot \{\text { AD - price   of   the   quadr.   variation   of } X \text { in } K \text { till } T \}, \end{array}
$$

which gives a new interpretation of the time value of an option. 

For the standard Black-Scholes model one has: 

$$
d \langle X _ {t} \rangle_ {X _ {t} = K} = \sigma^ {2} K ^ {2} d t \quad \text { and } \quad f (t, K) = \frac {\varphi (h (t , K))}{K \sigma \sqrt {t}}
$$

(see Exercise in Sect. 6.4). Hence it follows: 

$$
\begin{array}{c} \Longrightarrow \frac {1}{2}   \mathrm{E} ^ {*} [ L _ {K} ^ {T} ] = \frac {1}{2}   K ^ {2}   \sigma^ {2} \int_ {0} ^ {T} f (t, K)   d t = \frac {1}{2}   K ^ {2} \sigma^ {2} \int_ {0} ^ {T} \frac {\varphi (h (t , K))}{K \cdot \sigma \sqrt {t}}   d t \\ = \frac {1}{2}   K   \sigma \int_ {0} ^ {t} \varphi (h (t, K)) \cdot \frac {1}{\sqrt {t}}   d t \end{array}
$$

Hence by Itˆo-Tanaka for $C _ { T } = ( X _ { T } - K ) ^ { + }$ 

$$
C _ {0} = \mathrm{E} ^ {*} [ (X _ {T} - K) ^ {+} ] = (X _ {0} - K) ^ {+} + \frac {1}{2} K \sigma \int_ {0} ^ {T} \varphi (h (t, K)) \cdot \frac {1}{\sqrt {t}} d t
$$

(alternative BS-formula for forward price $X _ { t } = F _ { t } \ ( r = 0 ) )$ 

# Appendix: Itˆo Calculus Without Probabilities

S´eminaire de Probabilit´es XV 

1979/80 

## ITO CALCULUS WITHOUT PROBABILITIES

by H. F¨ollmer 

The aim of this note is to show that the Itˆo calculus can be developed “path by path” in the strict meaning of this term. We will derive Itˆo’s formula as an exercise in analysis for a class of real functions of quadratic variation, including the construction of the stochastic integral $\int F ^ { \prime } ( X _ { s - } ) d X _ { s }$ , by means of Riemann sums. Only afterwards we shall speak of probabilities in order to verify that for certain stochas tic processes (semimartingales, processes of finite energy,...) almost all paths belong to this class. 

Let x be a real function on $\lbrack 0 , \infty \lbrack$ which is right continuous and has left limits (also called c`adl`ag). We will use the following notation: $x _ { t } = x ( t )$ ， $\triangle x _ { t } = x _ { t } - x _ { t - } , \triangle x _ { t } ^ { 2 } = ( \triangle x _ { t } ) ^ { 2 }$ 

We define a subdivision to be any finite sequence $\tau = ( t _ { o } , \cdots , t _ { k } )$ such that $0 \leq t _ { o } < \cdots < t _ { k } < \infty$ , and we put $t _ { k + 1 } = \infty$ and $x _ { \infty } = 0$ . Let $( \tau _ { n } ) _ { n = 1 , 2 , \cdots }$ be a sequence of subdivisions whose meshes converge to 0 on each compact interval. We say that x is of quadratic variation along $\left( \tau _ { n } \right)$ if the discrete measures 

$$
\xi_ {n} = \sum_ {t _ {i} \in \tau_ {n}} (x _ {t _ {i + 1}} - x _ {t _ {i}}) ^ {2} \varepsilon_ {t _ {i}}\tag{1}
$$

converge weakly to a Radon measure $\xi$ on $\lbrack 0 , \infty \lbrack$ whose atomic part is given by the quadratic jumps of x: 

$$
[ x, x ] _ {t} = [ x, x ] _ {t} ^ {c} + \sum_ {s \leq t} \triangle x _ {s} ^ {2},\tag{2}
$$

where $[ x , x ]$ denotes the distribution function of $\xi$ and $[ x , x ] ^ { c }$ its continuous part. 

Theorem. Let x be of quadratic variation along $\left( \tau _ { n } \right)$ and $F$ a function of class $C ^ { 2 }$ on IR. Then the Itˆo formula 

$$
\begin{array}{l} F (x _ {t}) = F (x _ {o}) + \int_ {0} ^ {t} F (x _ {s -}) d x _ {s} + \frac {1}{2} \int_ {[ 0, t ]} F ^ {\prime \prime} (x _ {s -}) d [ x, x ] _ {s} \\ + \sum_ {s \leq t} [ F (x _ {s}) - F (x _ {s -}) - F ^ {\prime} (x _ {s -}) \triangle x _ {s} - \frac {1}{2} F ^ {\prime \prime} (x _ {s -}) \triangle x _ {s} ^ {2} ], \end{array}\tag{3}
$$

holds with 

$$
\int_ {0} ^ {t} F ^ {\prime} (x _ {s -}) d x _ {s} = \lim _ {n} \sum_ {\tau_ {n} \ni t _ {i} \leq t} F ^ {\prime} (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}),\tag{4}
$$

and the series in $( 4 )$ is absolutely convergent. 

Remark. Due to (2) the last two terms of (3) can be written as 

$$
\frac {1}{2} \int_ {0} ^ {t} F ^ {\prime \prime} (x _ {s -}) d [ x, x ] _ {s} ^ {c} + \sum_ {s \leq t} [ F (x _ {s}) - F (x _ {s -}) - F ^ {\prime} (x _ {s -}) \triangle x _ {s} ],\tag{5}
$$

and we have 

$$
\int_ {0} ^ {t} F ^ {\prime \prime} (x _ {s -}) d [ x, x ] _ {s} ^ {c} = \int_ {0} ^ {t} F ^ {\prime \prime} (x _ {s}) d [ x, x ] _ {s} ^ {c},\tag{6}
$$

since x is a c`adl`ag function. 

Proof. Let $t > 0$ . Since x is right continuous we have 

$$
F (x _ {t}) - F (x _ {o}) = \lim _ {n} \sum_ {\tau_ {n} \ni t _ {i} \leq t} [ F (x _ {t _ {i + 1}}) - F (x _ {t _ {i}}) ].
$$

1) For the sake of clarity we first treat the particularly simple case where x is a continuous function. Taylor’s formula can be written as 

$$
\begin{array}{l} \sum_ {\tau_ {n} \ni t _ {i} \leq t} [ F (x _ {t _ {i + 1}}) - F (x _ {t _ {i}}) ] = \sum F ^ {\prime} (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}) \\ \qquad + \frac {1}{2} \sum F ^ {\prime \prime} (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}) ^ {2} + \sum r (x _ {t _ {i}}, x _ {t _ {i + 1}}), \end{array}
$$

where 

$$
r (a, b) \leq \varphi (| b - a |) (b - a) ^ {2},\tag{7}
$$

and where $\varphi ( \cdot )$ is an increasing function on $[ 0 , \infty [$ such that $\varphi ( c ) $ 0 for $c  0 \cdot$ . For n the second sum of the right hand side converges to 

$$
\frac {1}{2} \int_ {[ 0, t ]} F ^ {\prime \prime} (x _ {s}) d [ x, x ] _ {s} = \frac {1}{2} \int_ {[ 0, t ]} F ^ {\prime \prime} (x _ {s -}) d [ x, x ] _ {s}
$$

due to the weak convergence of the discrete measures $\left( \xi _ { n } \right)$ ; note that by (2) the continuity of x implies the continuity of $[ x , x ]$ . The third sum, which is dominated by 

$$
\varphi (\max _ {\tau_ {n} \ni t _ {i} \leq t} | x _ {t _ {i + 1}} - x _ {t _ {i}} |) \sum_ {\tau_ {n} \ni t _ {i} \leq t} (x _ {t _ {i + 1}} - x _ {t _ {i}}) ^ {2},
$$

converges to 0 since x is continuous. Thus one obtains the existence of the limit (4) and Itˆo’s formula (3). 

2) Consider now the general case. Let $\varepsilon > 0$ . We divide the jumps of x on [0, t] into two classes: a finite class $C _ { 1 } = C _ { 1 } ( \varepsilon , t )$ , and a class $C _ { 2 } = C _ { 2 } ( \varepsilon , t )$ such that $\sum _ { s \in C _ { 2 } } \triangle x _ { s } ^ { 2 } \le \varepsilon ^ { 2 }$ . Let us write 

$$
\sum_ {\tau_ {n} \ni t _ {i} \leq t} [ F (x _ {t _ {i + 1}}) - F (x _ {t _ {i}}) ] = \sum_ {1} [ F (x _ {t _ {i + 1}} - F (x _ {t _ {i}}) ] + \sum_ {2} [ F (x _ {t _ {i + 1}} - F (x _ {t _ {i}}) ]
$$

where $\textstyle \sum _ { 1 }$ indicates the summation over those $t _ { i } \in \tau _ { n }$ with $t _ { i } \leq t$ for which the interval $] t _ { i } , t _ { i + 1 } ]$ contains a jump of class $C _ { 1 }$ . We have 

$$
\lim _ {n} \sum_ {1} [ F (x _ {t _ {i + 1}}) - F (x _ {t _ {i}}) ] = \sum_ {s \in C _ {1}} [ F (x _ {s}) - F (x _ {s -}) ].
$$

On the other hand, Taylor’s formula allows us to write 

$$
\sum_ {2} [ F (x _ {t _ {i + 1}}) - F (x _ {t _ {i}}) ] =
$$

$$
\begin{array}{c} \sum_ {\tau_ {n} \ni t _ {i} \leq t} F ^ {\prime} (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}) + \frac {1}{2} \sum_ {\tau_ {n} \ni t _ {i} \leq t} F ^ {\prime \prime} (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}) ^ {2} \\ - \sum_ {1} [ F ^ {\prime} (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}) + \frac {1}{2} F ^ {\prime \prime} (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}) ^ {2} ] + \sum_ {2} r (x _ {t _ {i}}, x _ {t _ {i + 1}}) \end{array}
$$

We will show below that the second sum on the right hand side converges to 

$$
\frac {1}{2} \int_ {[ 0, t ]} F ^ {\prime \prime} (x _ {s -}) [ x, x ] _ {s},
$$

as $n \uparrow \infty ;$ see (9). The third sum converges to 

$$
\sum_ {s \in C _ {1}} [ F ^ {\prime} (x _ {s -}) \triangle x _ {s} + \frac {1}{2} F ^ {\prime \prime} (x _ {s -}) \triangle x _ {s} ^ {2} ].
$$

Due to the uniform continuity of $F ^ { \prime \prime }$ on the bounded set of values $x _ { s } ~ \left( 0 \leq s \leq t \right)$ we can assume $( 7 )$ , and this implies 

$$
\limsup _ {n} \sum_ {2} r (x _ {t _ {i}}, x _ {t _ {i + 1}}) \leq \varphi (\varepsilon +) [ x, x ] _ {t +}.\tag{8}
$$

Let $\varepsilon$ converge to 0. Then (8) converges to 0, and 

$$
\sum_ {s \in C _ {1} (\varepsilon , t)} [ F (x _ {s}) - F (x _ {s -}) - F ^ {\prime} (x _ {s -}) \triangle x _ {s} ] - \frac {1}{2} \sum_ {s \in C _ {1} (\varepsilon , t)} F ^ {\prime \prime} (x _ {s -}) \triangle x _ {s} ^ {2}
$$

converges to the series in (3). Furthermore the series converges absolutely since 

$$
\sum_ {s \leq t} | F (x _ {s}) - F (x _ {s -}) - F ^ {\prime} (x _ {s -}) \triangle x _ {s} | \leq \text { const } \sum_ {s \leq t} \triangle x _ {s} ^ {2}
$$

by Taylor’s formula. Thus we obtain the existence of the limit in (4) and Itˆo’s formula (3). 

3) Let us show that 

$$
\lim _ {n} \sum_ {\tau_ {n} \ni t _ {i} \leq t} f (x _ {t _ {i}}) (x _ {t _ {i + 1}} - x _ {t _ {i}}) ^ {2} = \int_ {[ 0, t ]} f (x _ {s -}) d [ x, x ] _ {s}\tag{9}
$$

for any continuous function f on IR. Let $\varepsilon > 0$ , and denote by z the distribution function of the jumps in class $C _ { 1 } = C _ { 1 } ( \varepsilon , t )$ , i. e., 

$$
z _ {u} = \sum_ {C _ {1} \ni s \leq u} \triangle x _ {s} (u \geq 0).
$$

We have 

$$
\lim _ {n} \sum_ {\tau_ {n} \ni t _ {i} \leq u} f (x _ {t _ {i}}) (z _ {t _ {i + 1}} - z _ {t _ {i}}) ^ {2} = \sum_ {C _ {1} \ni s \leq u} f (x _ {s -}) \triangle x _ {s} ^ {2}\tag{10}
$$

for each $u \geq 0$ . Denote by $\zeta _ { n }$ and $\eta _ { n }$ the discrete measures associated with $z$ and $y = x - z$ in the sense of (1). By (10) the measures $\zeta _ { n }$ converge weakly to the discrete measure 

$$
\zeta = \sum_ {s \in C _ {1}} \triangle x _ {s} ^ {2} \varepsilon_ {s}.
$$

Since the last sum of 

$$
\begin{array}{c} \sum_ {\tau_ {n} \ni t _ {i} \leq u} (x _ {t _ {i + 1}} - x _ {t _ {i}}) ^ {2} = \sum (y _ {t _ {i + 1}} - y _ {t _ {i}}) ^ {2} + \sum (z _ {t _ {i + 1}} - z _ {t _ {i}}) ^ {2} \\ + 2 \sum (y _ {t _ {i + 1}} - y _ {t _ {i}}) (z _ {t _ {i + 1}} - z _ {t _ {i}}) \end{array}
$$

converges to 0, the measures $\eta _ { n }$ converge weakly to the measure $\eta = \xi - \zeta$ whose atomic part has total mass $\leq \varepsilon ^ { 2 }$ . Hence the function f x is almost surely continuous with respect to the continuous part of $\eta ,$ and this implies 

$$
\limsup _ {n} \sum_ {\tau_ {n} \ni t _ {i} \leq t} f (x _ {t _ {i}}) (y _ {t _ {i + 1}} - y _ {t _ {i}}) ^ {2} - \int_ {[ 0, t ]} f (x _ {s -}) d \eta | \leq 2 \| f \| _ {t} \varepsilon^ {2}\tag{11}
$$

where $\| f \| _ { t } = \operatorname* { s u p } \{ f ( x _ { s } ) ; 0 \leq s \leq t \}$ . Combining (10) and (11) we obtain (9), and this completes the proof. Let us emphasize that we have followed closely the “classical ” argument; see Meyer [4]. The only new contribution is the use of weak convergence, which allows us to give a completely analytic version. 

## Remarks.

1) Let $x = ( x ^ { 1 } , \cdots , x ^ { n } )$ be a c`adl`ag function on $\lbrack 0 , \infty \lbrack$ with values in $\mathbb { R } ^ { n }$ . We say that x a is of quadratic variation along $\left( \tau _ { n } \right)$ if this holds for all real functions $x ^ { i } , x ^ { i } + x ^ { j } \ ( 1 \leq i , j \leq n )$ . In this case we put 

$$
\begin{array}{c} [ x ^ {i}, x ^ {j} ] _ {t} = \frac {1}{2} ([ x ^ {i} + x ^ {j}, x ^ {i} + x ^ {j} ] _ {t} - [ x ^ {i}, x ^ {i} ] _ {t} - [ x ^ {j}, x ^ {j} ] _ {t}) \\ = [ x ^ {i}, x ^ {j} ] _ {t} ^ {c} + \sum_ {s \leq t} \triangle x _ {s} ^ {i} \triangle x _ {s} ^ {j}. \end{array}
$$

Then we have the Itˆo formula 

$$
\begin{array}{c} F (x _ {t}) = F (x _ {o}) + \int_ {0} ^ {t} D F (x _ {s -}) d x _ {s} + \frac {1}{2} \sum_ {i, j} \int_ {0} ^ {t} D _ {i} D _ {j} F (x _ {s -}) d [ x ^ {i}, x ^ {j} ] _ {s} ^ {c} \\ + \sum_ {s \leq t} [ F (x _ {s}) - F (x _ {s -}) - \sum_ {i} D _ {i} F (x _ {s -}) \triangle x _ {s} ^ {i} ] \end{array}\tag{12}
$$

for any function F of class $C ^ { 2 }$ on $\mathbb { R } ^ { n }$ , where 

$$
\int_ {0} ^ {t} D F (x _ {s -}) d x _ {s} = \lim _ {n} \sum_ {\tau_ {n} \ni t _ {i} \leq t} <   D F (x _ {t _ {i}}), x _ {t _ {i + 1}} - x _ {t _ {i}} >\tag{13}
$$

$( < \cdot , \cdot > =$ scalar product on $\mathbb { R } ^ { n } )$ . The proof is the same as above, but with more cumbersome notation. 

2) The class of functions of quadratic variation is stable with respect to $C ^ { 1 }$ - operations. More precisely, if $x = ( x ^ { 1 } , \cdots , x ^ { n } )$ is of quadratic variation along $\left( \tau _ { n } \right)$ and $F$ a continuously diferentiable function on $\mathbb { R } ^ { n }$ then $y = F \circ x$ is of quadratic variation along $\left( \tau _ { n } \right)$ , with 

$$
[ y, y ] _ {t} = \sum_ {i, j} \int_ {0} ^ {t} D _ {i} F (x _ {s}) D _ {j} F (x _ {s}) d [ x ^ {i}, x ^ {j} ] _ {s} ^ {c} + \sum_ {s \leq t} \triangle y _ {s} ^ {2}.\tag{14}
$$

This is the analytic version of a result of Meyer for semimartingales, see [4] p. 359. The proof is analogous to the previous one. 

Let us now turn to stochastic processes. Let $( X _ { t } ) _ { t \geq 0 }$ be a semimartingale. Then, for any $t \geq 0$ , the sums 

$$
S _ {\tau , t} = \sum_ {\tau \ni t _ {i} \leq t} (X _ {t _ {i + 1}} - X _ {t _ {i}}) ^ {2}\tag{15}
$$

converge in probability to 

$$
[ X, X ] _ {t} = <   X ^ {c}, X ^ {c} > _ {t} + \sum_ {s \leq t} \triangle X _ {s} ^ {2}
$$

when the mesh of the subdivision $\tau$ converges to 0 on $[ 0 , t ]$ ; see Meyer [4] p. 358. For each sequence there exists thus a subsequence $\left( \tau _ { n } \right)$ such that, almost surely, 

$$
\lim _ {n} S _ {\tau_ {n}, t} = [ X, X ] _ {t}\tag{16}
$$

for each rational t . This implies that almost all paths are of quadratic variation along $\left( \tau _ { n } \right)$ . Furthermore the relation (16) is valid for all $t \geq 0$ due to (9). The Itˆo formula (3), applied strictly pathwise, does not depend on the sequence $\left( \tau _ { n } \right)$ . In particular, we obtain the convergence in probability of the Riemann sums in (4) to the stochastic integral 

$$
\int_ {0} ^ {t} F ^ {\prime} (X _ {s -}) d X _ {s},
$$

when the mesh of $\tau$ goes to 0 on $[ 0 , t ]$ 

## Remarks.

1) For Brownian motion and an arbitrary sequence of subdivisions $\left( \tau _ { n } \right)$ with mesh tending to 0 on each compact interval, almost all paths are of quadratic variation along $\left( \tau _ { n } \right)$ . Indeed, by L´evy’s theorem we have (16) without passing to subsequences. 

2) For the above argument it sufices to know that the sums (15) converge in probability to an increasing process $[ X , X ]$ which has paths of the form (2). The class of processes of quadratic variation is clearly larger than the class of semimartingales: Just consider a deterministic process of quadratic variation which is of unbounded variation. Let us mention also the processes offinite energy $X = M + A$ where M is a local martingale and $A$ is a process with paths of quadratic variation 0 along the dyadic subdivisions. These processes occur in the probabilistic study of Dirichlet spaces: see Fukushima [3]. 

3) For a semimartingale it is known how to construct the stochastic integral $\int H _ { s - } d X _ { s }$ (H c`adl`ag and adapted) pathwise as a limit of Riemann sums, in the sense that the sums converge almost surely outside an exceptional set which depends on H; see Bichteler [1]. We have just shown that for the particular needs of Itˆo calculus, where $H = f \circ X$ (f of class $C ^ { 1 } )$ , the exceptional set can be chosen in advance, independently of H. It is possible to go beyond the class $C ^ { 1 }$ by treating local times “path by path”. But not too far beyond: Stricker [5] has just shown that an extension to continuous functions is only possible for processes with paths of finite variation. 

## References



1) Bichteler, K.: Stochastic Integration and L<sup>p</sup>-theory of semimartingales. Technical report no. 5, U. of Texas (1979). 





2) Dellacherie, C., et Meyer, P.A.: Probabilit´es et Potentiel; Th´eorie des Martingales. Hermann (1980). 





3) Fukushima, M.: Dirichlet forms and Markov processes. North Holland (1980). 





4) Meyer, P.A.: Un cours sur les int´egrales stochastiques. Sem. Prob. X, LN 511 (1976). 





5) Stricker, C.: Quasimartingales et variations. Sem. Prob. XV, LN 850 (1980). 



## References



Bauer, H. (1996): Probability Theory. De Gruyter. (2001): Measure and Integration Theory. De Gruyter. 





Black-Derman-Toy (1990): “A one-factor model of interest rates and its application to Treasury bond options,” Financ. Analysts Journal, 46(1), 33–39. 





Black-Karasinski (1991): “Bond and option pricing when short rates are lognormal,” Financ. Analysts Journal, 47(4), 52–59. 





Black-Scholes (1973): “The pricing of options and corporate liabilities,” J. Polit. Economy, 81, 637–654. 





Brace-Gatarek-Musiela (1997): “The Market Model of Interest Rate Dynamics,” Mathematical Finance, 7, 127–154. 





Bru B. and M. Yor (2002): “Comments on the life and mathematical legacy of Wolfgang Doeblin,” Finance and Stochastics, 6(1), 3–47. 





Carr-Jarrow (1990): “The Stop-Loss Start-Gain Paradox and Option Valuation: A New Decomposition into Intrinsic and Time Value,” Review of Fin. Studies, 3(3). 





Cox-Ingersoll-Ross (1981): “A re-examination of traditional hypotheses about the term structure of interest rates,” Journal of Finance, 36, 769– 799. 





Delbaen-Schachermayer (1995): “The No-Arbitrage property under a change of numeraire,” Stochastics Stochastic Rep., 53, 213–226. 





(1997): “The Banach space of workable contingent claims in arbitrage theory,” Ann. Inst. H.Poincar´e Prob. Statist. 





Duffie, D. (2001): Dynamic Asset Pricing Theory. 3rd Ed. Princeton UP. 





Elliott-Kopp (1999): Mathematics of Financial Markets. Springer. 





Foellmer, H. (1981): “Calcul d’Itˆo sans probabilit´e,” Seminaire de Probabilit´e XV, Springer Lect. Notes 850, 143–150. 





(1991): Vorlesungsmanuskript Stochastische Analysis. Ausarbeitung Mueck. 





(1998): “Vom Leibniz-Kalkuel zur stochastischen Analysis,” LEOPOLDINA (R.3), 43, 249–257. 





Geman-ElKaroui-Rochet (1995): “Changes of numeraire, changes of probability measures and pricing of options,” J. Appl. Probability, 32, 443–458. 





Harrison-Kreps (1979): “Martingales and arbitrage in multiperiod securities markets,” Journal of Economic Theory, 20, 381–408. 





Harrison-Pliska (1981): “Martingales and stochastic integrals in the theory of continuous trading,” Stochastic Process. Appl., 11, 215–260. 





Heath-Jarrow-Morton (1992): “Bond Pricing and the Term Structure of Interest Rates,” Econometrica, 60, 77–105. 





Ho-Lee (1986): “Term structure movements and pricing interest rate contingent claims,” Journal of Finance, 41, 1011–1029. 





Ingersoll, J. J. (1987): Theory of Financial Decision Making. Rowman and Littlefield. 





Karatzas-Shreve (1988): Brownian Motion and Stochastic Calculus. Springer. 





(1998): Methods of Mathematical Finance. Springer. 





Lamberton-Lapeyre (1995): Introduction to Stochastic Calculus, applied to Finance. Chapman and Hall, London. 





Levy, P.<sup>´</sup> (1965): Processus stochastiques et Mouvement Brownien, 2nd Ed. Gauthier-Villars. 





McCulloch, J. (1975): “Operational Aspects of the Siegel Paradox,” Quart. Journal of Economics, 89, 170–172. 





Merton, R. (1973): “Theory of rational option pricing,” Bell J. Econom. Managm. Sci, 4, 141–183. 





Miltersen-Sandmann-Sondermann (1997): “Closed Form Solutions for Term Structure Derivatives with Log-Normal Interest Rates,” Journal of Finance, 52, 409–430. 





Musiela-Rutkowski (1997): Martingale Methods in Financial Modelling. Springer. 





Protter, P. (1990): Stochastic Integration and Diferential Equations. Springer. 





Revuz-Yor (1991): Continuous Martingales and Brownian Motion. Springer. 





Sandmann-Sondermann (1993): “A term structure model and the pricing of interest rate derivatives,” Rev. Futures Markets, 12, 391–423. 





(1994): “On the stability of lognormal interest models and the pricing of Eurodollar futures,” Working paper, University of Bonn. 





Sandmann-Sondermann-Miltersen (1995): “Closed Form Term Structure Derivatives in a Heath–Jarrow–Morton Model with Log–normal Annually Compounded Interest Rates,” Research Symposium Proceedings CBOT, pp. 145–164. 





Shiryaev, A. (1999): Essentials of Stochastic Finance. World Schientific Singapore. 





Siegel, J. (1972): “Risk, interest rates, and forward exchange,” Quart. Journal of Economics, 86, 303–309. 





Vasicek, O. (1977): “An equilibrium characterisation of the term structure,” J. Finan. Econom., 5, 177–188. 



# Lecture Notes in Economics and Mathematical Systems

For information about Vols. 1–483 please contact your bookseller or Springer-Verlag 



Vol. 488: B. Schmolck, Ommitted Variable Tests and Dynamic Specification. X, 144 pages. 2000. 





Vol. 489: T. Steger, Transitional Dynamics and Economic Growth in Developing Countries. VIII, 151 pages. 2000. 





Vol. 490: S. Minner, Strategic Safety Stocks in Supply Chains. XI, 214 pages. 2000. 





Vol. 491: M. Ehrgott, Multicriteria Optimization. VIII, 242 pages. 2000. 





Vol. 492: T. Phan Huy, Constraint Propagation in Flexible Manufacturing. IX, 258 pages. 2000. 





Vol. 493: J. Zhu, Modular Pricing of Options. X, 170 pages. 2000. 





Vol. 494: D. Franzen, Design of Master Agreements for OTC Derivatives. VIII, 175 pages. 2001. 





Vol. 495: I. Konnov, Combined Relaxation Methods for Variational Inequalities. XI, 181 pages. 2001. 





Vol. 496: P. Weiß, Unemployment in Open Economies. XII, 226 pages. 2001. 





Vol. 497: J. Inkmann, Conditional Moment Estimation of Nonlinear Equation Systems. VIII, 214 pages. 2001. 





Vol 498: M Reutter A Macroeconomic Model of West German Unemployment. X, 125 pages. 2001. 





Vol. 499: A. Casajus, Focal Points in Framed Games. XI, 131 pages. 2001. 





Vol. 500: F. Nardini, Technical Progress and Economic Growth. XVII, 191 pages. 2001. 





Vol. 501: M. Fleischmann, Quantitative Models for Reverse Logistics. XI, 181 pages. 2001. 





Vol. 502: N. Hadjisavvas, J. E. Martínez-Legaz, J.-P. Penot (Eds.). Generalized Convexity and Generalized Monotonicity. IX, 410 pages. 2001. 





Vol. 503: A. Kirman, J.-B. Zimmermann (Eds.), Econom ics with Heterogenous Interacting Agents. VII, 343 pages. 2001. 





Vol. 504: P.-Y. Moix (Ed.). The Measurement of Market Risk. XI, 272 pages. 2001. 





Vol. 505: S. Voß, J. R. Daduna (Eds.), Computer-Aided Scheduling of Public Transport. XI, 466 pages. 2001. 





Vol. 506: B. P. Kellerhals, Financial Pricing Models in Con-tinuous Time and Kalman Filtering. XIV, 247 pages 2001. 





Vol. 507: M. Koksalan, S. Zionts, Multiple Criteria Deci sion Making in the New Millenium. XII, 481 pages. 2001. 





Vol. 508: K. Neumann, C. Schwindt, J. Zimmermann, Project Scheduling with Time Windows and Scarce Resources. XI, 335 pages. 2002. 





Vol. 509: D. Hornung, Investment, R&D, and Long-Run Growth. XVI, 194 pages. 2002. 





Vol. 510: A. S. Tangian, Constructing and Applying Objective Functions. XII, 582 pages. 2002. 





Vol. 511: M. Külpmann, Stock Market Overreaction and Fundamental Valuation. IX, 198 pages. 2002. 





Vol. 512: W.-B. Zhang, An Economic Theory of Cities.XI, 220 pages. 2002. 





Vol. 513: K. Marti, Stochastic Optimization Techniques. VIII, 364 pages. 2002. 





Vol. 514: S. Wang, Y. Xia, Portfolio and Asset Pricing. XII, 200 pages. 2002. 





Vol. 515: G. Heisig, Planning Stability in Material Requirements Planning System. XII, 264 pages. 2002. 





Vol. 516: B. Schmid, Pricing Credit Linked Financia Instruments. X, 246 pages. 2002. 





Vol. 517: H. I. Meinhardt, Cooperative Decision Making in Common Pool Situations. VIII, 205 pages. 2002. 





Vol. 518: S. Napel, Bilateral Bargaining. VIII, 188 pages. 2002. 





Vol, 519: A. Klose, G. Speranza. L. N. Van Wassenhove (Eds.), Quantitative Approaches to Distribution Logistics and Supply Chain Management. XIII, 421 pages. 2002. 





Vol. 520: B. Glaser, Efficiency versus Sustainability in Dynamic Decision Making. IX, 252 pages. 2002. 





Vol. 521: R. Cowan, N. Jonard (Eds.), Heterogenous Agents, Interactions and Economic Performance. XIV, 339 pages. 2003. 





Vol. 522: C. Neff, Corporate Finance, Innovation, and Strategic Competition. IX, 218 pages. 2003. 





Vol. 523: W.-B. Zhang, A Theory of Interregional Dynamics. XI, 231 pages. 2003. 





Vol. 524: M. Frölich, Programme Evaluation and Treatment Choise. VIII, 191 pages. 2003. 





Vol. 525: S. Spinler, Capacity Reservation for Capital-Intensive Technologies. XVI, 139 pages. 2003. 





Vol. 526: C. F. Daganzo, A Theory of Supply Chains. VIII, 123 pages. 2003. 





Vol. 527: C. E. Metz, Information Dissemination in Currency Crises. XI, 231 pages. 2003. 





Vol. 528: R. Stolletz, Performance Analysis and Optimization of Inbound Call Centers. X, 219 pages. 2003. 





Vol. 529: W. Krabs, S. W. Pickl, Analysis, Controllability and Optimization of Time-Discrete Systems and Dynamical Games. XII, 187 pages. 2003. 





Vol. 530: R. Wapler, Unemployment, Market Structure and Growth. XXVII, 207 pages. 2003. 





Vol. 531: M. Gallegati, A. Kirman, M. Marsili (Eds.), The Complex Dynamics of Economic Interaction. XV, 402 pages, 2004. 





Vol. 532: K. Marti, Y. Ermoliev, G. Pflug (Eds.), Dynamic Stochastic Optimization. VIII, 336 pages. 2004. 





Vol. 533: G. Dudek, Collaborative Planning in Supply Chains. X, 234 pages. 2004. 





Vol. 534: M. Runkel, Environmental and Resource Policy for Consumer Durables. X, 197 pages. 2004. 





Vol. 535: X. Gandibleux, M. Sevaux, K. Sörensen, V. T’kindt (Eds.), Metaheuristics for Multiobjective Optimisation. IX, 249 pages. 2004. 





Vol. 536: R. Brüggemann, Model Reduction Methods for Vector Autoregressive Processes. X, 218 pages. 2004. 





Vol. 537: A. Esser, Pricing in (In)Complete Markets. XI, 122 pages, 2004. 





Vol. 538: S. Kokot, The Econometrics of Sequential Trade Models. XI, 193 pages. 2004. 





Vol. 539: N. Hautsch, Modelling Irregularly Spaced Financial Data. XII, 291 pages. 2004. 





Vol. 540: H. Kraft, Optimal Portfolios with Stochastic Interest Rates and Defaultable Assets. X, 173 pages. 2004. 





Vol. 541: G.-y. Chen, X. Huang, X. Yang, Vector Optimization. X, 306 pages. 2005. 





Vol. 542: J. Lingens, Union Wage Bargaining and Economic Growth. XIII, 199 pages. 2004. 





Vol. 543: C. Benkert, Default Risk in Bond and Credit Derivatives Markets. IX, 135 pages. 2004. 





Vol. 544: B. Fleischmann, A. Klose, Distribution Logistics. X, 284 pages. 2004. 





Vol. 545: R. Hafner, Stochastic Implied Volatility. XI, 229 pages. 2004. 





Vol. 546: D. Quadt, Lot-Sizing and Scheduling for Flexible Flow Lines. XVIII, 227 pages. 2004. 





Vol. 547: M. Wildi, Signal Extraction. XI, 279 pages. 2005. 





Vol. 548: D. Kuhn, Generalized Bounds for Convex Multi stage Stochastic Programs. XI, 190 pages. 2005. 





Vol. 549: G. N. Krieg, Kanban-Controlled Manufacturing Systems. IX, 236 pages. 2005. 





Vol. 550: T. Lux, S. Reitz, E. Samanidou, Nonlinear Dynamics and Heterogeneous Interacting Agents. XIII, 327 pages. 2005. 





Vol. 551: J. Leskow, M. Puchet Anyul, L. F. Punzo, New Tools of Economic Dynamics. XIX, 392 pages. 2005. 





Vol. 552: C. Suerie, Time Continuity in Discrete Time Models. XVIII, 229 pages. 2005. 





Vol. 553: B. Mönch, Strategic Trading in Illiquid Markets. XIII, 116 pages. 2005. 





Vol. 554: R. Foellmi, Consumption Structure and Macroeconomics. IX, 152 pages. 2005. 





Vol. 555: J. Wenzelburger, Learning in Economic Systems with Expectations Feedback (planned) 2005 





Vol. 556: R. Branzei, D. Dimitrov, S. Tijs, Models in Cooperative Game Theory. VIII, 135 pages. 2005. 





Vol. 557: S. Barbaro, Equity and Efficiency Considerations of Public Higer Education. XII, 128 pages. 2005. 





Vol. 558: M. Faliva, M. G. Zoia, Topics in Dynamic Mod el Analysis. X, 144 pages. 2005. 





Vol. 559: M. Schulmerich, Real Options Valuation. XVI, 357 pages. 2005. 





Vol. 560: A. von Schemde, Index and Stability in Bimatrix Games. X, 151 pages. 2005. 





Vol. 561: H. Bobzin, Principles of Network Economics. XX, 390 pages. 2006. 





Vol. 562: T. Langenberg, Standardization and Expectations. IX, 132 pages. 2006. 





Vol. 563: A. Seeger (Ed.), Recent Advances in Optimiza tion. XI, 455 pages. 2006. 





Vol. 564: P. Mathieu, B. Beaufils, O. Brandouy (Eds.), Artificial Economics. XIII, 237 pages. 2005. 





Vol. 565: W. Lemke, Term Structure Modeling and Esti mation in a State Space Framework. IX, 224 pages. 2006 





Vol. 566: M. Genser, A Structural Framework for the Pricing of Corporate Securities. XIX, 176 pages. 2006. 





Vol. 567: A. Namatame, T. Kaizouji, Y. Aruga (Eds.), The Complex Networks of Economic Interactions. XI, 343 pages. 2006. 





Vol. 568: M. Caliendo, Microeconometric Evaluation of Labour Market Policies. XVII, 258 pages. 2006. 





Vol. 569: L. Neubecker, Strategic Competition in Oligopolies with Fluctuating Demand. IX, 233 pages. 2006. 





Vol. 570: J. Woo, The Political Economy of Fiscal Policy. X, 169 pages. 2006. 





Vol. 571: T. Herwig, Market-Conform Valuation of Options. VIII, 104 pages. 2006. 





Vol. 572: M. F. Jäkel, Pensionomics. XII, 316 pages. 2006 





Vol. 573: J. Emami Namini, International Trade and Multi national Activity, X, 159 pages, 2006. 





Vol. 574: R. Kleber, Dynamic Inventory Management in Reverse Logisnes, XII, 181 pages, 2006 





Vol. 575: R. Hellermann, Capacity Options for Revenue Management, XV, 199 pages, 2006. 





Vol. 576: J. Zajac, Economics Dynamics, Information and Equilibnum, X, 284 pages, 2006. 





Vol. 577: K. Rudolph, Bargaining Power Effects in Finan cial Contracting, XVIII, 330 pages, 2006. 





Vol. 578: J. Kühn, Optimal Risk-Return Trade-Offs of Com mercial Banks, IX, 149 pages, 2006. 





Vol. 579: D. Sondermann, Introduction to Stochastic Calculus for Finance, X, 136 pages, 2006. 





Vol. 580: S. Seifert, Posted Price Offers in Internet Auction Markets, IX, 186 pages, 2006. 





Vol. 581: K. Marti; Y. Ermoliev; M. Makowsk; G. Pflug (Eds.), Coping with Uncertainty, XIII, 330 pages, 2006 (planned). 

