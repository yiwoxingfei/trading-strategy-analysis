

<!-- === Source: MinerU_markdown_Stochastic_Calculus_for_Finance_II_1_2122706224590991378.md (Page 1) === -->

Stochastic Calculus for Finance II 

Rex C. Liu, Tepper School of Business, Carnegie Mellon University Spring 2025 

To the faculty and staf of the MSCF program 

## Disclaimer

These are the lecture notes and problem sets for the course BUS 46-975 Stochastic Calculus for Finance II, given by Dr. Mykhaylo Shkolnikov and teaching assistant Chen Ai at Tepper School of Business, Carnegie Mellon University in Spring 2025. Most materials are inspired by Dr. Steven E. Shreve. 

This course uses stochastic calculus to develop models for equity and fixed income derivatives. The role and limitations of risk-neutral pricing will be discussed. Both risk-neutral and forward measures will be used, and change of measure associated with change of currency will be explained. Reference texts include [Shr04], [Shr], etc. The primary prerequisite for this course is Stochastic Calculus for Finance I, which covers material from [Shr04, §1 – 4]. Familiarity with partial diferential equations is also beneficial. Prior to formally beginning the course, readers are encouraged to work through the practices in Appendix A. 

The solutions of the problem sets are given by Rex Liu with help from Mathematics Stack Exchange, several large language models (primarily GPT o3-mini-high and Gemini 2.5 pro), and friends. If you see any mistakes or think that the presentation is unclear and could be improved, please send an email to: rexliu@andrew.cmu.edu. All comments and suggestions are appreciated. Special thanks to Vignesh RSB, Shujie (Trent) Zhang, and Yuhan (Alex) Jin who reported several mistakes and typos in the draft version of this document. 

## Notations

Throughout these notes, we use the following notation: 

$X ( t )$ denotes a stochastic process. For a function $f ( t , x )$ we denote partial derivatives by 

$$
f _ {t} = \frac {\partial f}{\partial t}, \quad f _ {x} = \frac {\partial f}{\partial x}, \quad \text { etc. }
$$

• A stochastic integral is written as 

$$
X (t) = \int_ {0} ^ {t} \Delta (u) d W (u),
$$

so that in diferential notation, 

$$
d X (t) = \Delta (t) d W (t).
$$

• The quadratic variation of X(t) is given by 

$$
[ X, X ] (t) = \int_ {0} ^ {t} \Delta (u) ^ {2} d u,
$$

which in diferential form is written as 

$$
d X (t) d X (t) = \Delta (t) ^ {2} d t.
$$

• A key aspect of Itô calculus is the multiplication table for the diferentials. In particular, 

$$
\begin{array}{c c c} & d t & d W (t) \\ \hline d t & 0 & 0 \\ d W (t) & 0 & d t \end{array}
$$

This table encapsulates the fact that the product of two dt terms (or dt with $d W ( t ) )$ is negligible, while $d W ( t ) \cdot d W ( t )$ is of order dt. 

## Contents

1 Lecture Notes 1   
1.1 A review of the big theorems . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1   
1.1.1 Itô's formula for functions of two stochastic processes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1   
1.1.2 Martingale representation theorem . . . . . . . . . . . . . . . . . . . . . . . . . 2   
1.1.3 Lévy's characterization of Brownian motion . . . . . . . . . . . . . 2   
1.1.4 Girsanov's theorem . . . . . . . . . . . . 3   
1.1.5 General models: the Brownian framework 10   
1.2 Pricing in the Markovian framework 16   
1.2.1 Stochastic differential equations and the Markov property 17   
1.2.2 Derivation of pricing partial differential equations (PDEs) 17   
1.2.3 Boundary conditions for the pricing PDE 19   
1.2.4 Kolmogorov's equations and Dupire's formula 27   
1.3 Fixed income models 32   
1.3.1 Yield curve and forward interest rates 32   
1.3.2 The Ho-Lee short rate model 34   
1.3.3 Heath-Jarrow-Morton (HJM) framework 42   
1.3.4 Forward contracts 47   
1.3.5 Black's formula 51   
1.3.6 Secured overnight funding rate (SOFR) 56   
1.3.7 Futures contracts 59   
1.4 Financing portfolios 63   
1.4.1 Self-financing portfolio 63   
1.4.2 Funding and collateral considerations 65   
1.5 Foreign and domestic risk-neutral measures 68   
1.5.1 Domestic risk-neutral measure 69   
1.5.2 Foreign risk-neutral measure 70   
1.6 Course summary 74   
2 Problem Sets 85   
2.1 A review of the big theorems 85   
2.1.1 Decorrelating two correlated Brownian motions 85   
2.1.2 Radon-Nikodym derivative process in a binomial model 87   
2.1.3 Change of measure for a normal random variable 90   
2.1.4 Quotient of martingales 93   
2.2 Connection with PDEs 95   
2.2.1 Binomial Markov process 95   
2.2.2 Four-step procedure and Brownian motion 97   
2.2.3 Corridor option 99   
2.2.4 Change of measure to price an Asian option 101   
2.3 Kolmogorov's equations and Dupire's formula 107   
2.3.1 Stochastic volatility 107 

2.3.2 Kolmogorov forward equation for an exponential martingale . 112   
2.3.3 Application of Dupire's formula . 114   
2.3.4 Black-Scholes with nonrandom time-dependent volatility . 118   
2.4 The Hull-White spot rate model . 119   
2.4.1 Solving the Hull-White stochastic differential equation . 119   
2.4.2 Zero-coupon bond prices in the Hull-White model . 120   
2.4.3 Matching the initial yield curve in the Hull-White model . 122   
2.4.4 Bond volatility, forward interest rates, and forward measure in the Hull-White model . 124   
2.4.5 Interest rate caplet in the Hull-White model . 126   
2.4.6 Hedging with futures in the Hull-White model . 127   
2.5 Secured overnight funding rate (SOFR) . 131   
2.5.1 SOFR caplet in the Ho-Lee model . 131   
2.5.2 Swaps measure . 133   
2.6 Forward, futures, and foreign exchange (FX) . 134   
2.6.1 Hedging with futures and different interest rate on margin account . 134   
2.6.2 FX call with funding costs . 137   
2.6.3 Forward exchange rate . 139   
2.6.4 Hedging multi-currency cashflows with various FX options . 140   
A Preliminary Review Sessions 143   
A.1 Itô calculus . 143   
A.1.1 Itô integrals . 144   
A.1.2 Itô's Formula . 146   
A.2 Information and conditioning . 149   
A.3 Change of measure . 151   
B Exams 157   
B.1 Midterm of spring 2025 . 157   
B.2 Final of spring 2025 . 160 

# Chapter 1

# Lecture Notes

## 1.1 A review of the big theorems

Reference: [Shr04, §4.6, 5.1 – 5.4]. 

“All models are wrong, but some are useful.” 

We recall five fundamental theorems which play a central role in stochastic calculus and financial mathematics: 

1. Martingale Representation Theorem 

2. Lévy’s Theorem (Characterization of Brownian Motion) 

3. Girsanov’s Theorem 

4. Fundamental Theorems of Asset Pricing 

## 1.1.1 Itô’s formula for functions of two stochastic processes

Let $X ( t )$ and $Y ( t )$ be defined by 

$$
X (t) = \int_ {0} ^ {t} \Delta (u) d W _ {1} (u), Y (t) = \int_ {0} ^ {t} \Gamma (u) d W _ {2} (u),
$$

where $W _ { 1 }$ and $W _ { 2 }$ are Brownian motions (possibly correlated). If $f ( t , x , y )$ is a function that is twice continuously diferentiable in x and y and once in t, then Itô’s formula gives 

$$
\begin{array}{l} d f (t, X (t), Y (t)) \\ = f _ {t} (t, X (t), Y (t))   d t + f _ {x} (t, X (t), Y (t))   d X (t) + f _ {y} (t, X (t), Y (t))   d Y (t) \\ \quad + \frac {1}{2} f _ {x x} (t, X (t), Y (t))   d X (t) d X (t) + \frac {1}{2} f _ {y y} (t, X (t), Y (t))   d Y (t) d Y (t) \\ \quad + f _ {x y} (t, X (t), Y (t))   d X (t) d Y (t). \end{array}
$$

Using the rules from the multiplication table, note that 

$$
d X (t) d X (t) = \Delta (t) ^ {2} d t, d Y (t) d Y (t) = \Gamma (t) ^ {2} d t.
$$

If the correlation between $W _ { 1 }$ and $W _ { 2 }$ is given by $\rho ,$ then 

$$
d X (t) d Y (t) = \Delta (t) \Gamma (t) d W _ {1} (t) d W _ {2} (t) = \Delta (t) \Gamma (t) \rho d t.
$$

Example 1.1.1. Consider $f ( t , x , y ) = x y$ . For the function $f ( t , x , y ) = x y$ , we compute: 

$$
f _ {t} = 0, \quad f _ {x} = y, \quad f _ {y} = x, \quad f _ {x x} = 0, \quad f _ {y y} = 0, \quad f _ {x y} = 1.
$$

Thus, applying Itô’s formula: 

$$
d (X (t) Y (t)) = Y (t) d X (t) + X (t) d Y (t) + d X (t) d Y (t).
$$

## 1.1.2 Martingale representation theorem

We recall the martingale representation theorem. 

Theorem 1.1.2. Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space and let $W _ { 1 } , W _ { 2 } , \ldots , W _ { d }$ be independent Brownian motions. Denote by $\{ \mathcal { F } _ { t } \} _ { 0 \leq t \leq T }$ the filtration generated by these Brownian motions. Then any squareintegrable martingale $M ( t )$ adapted to $\{ \mathcal { F } _ { t } \}$ admits the representation 

$$
M (t) = M (0) + \sum_ {i = 1} ^ {d} \int_ {0} ^ {t} \Delta_ {i} (u) d W _ {i} (u), \quad 0 \leq t \leq T,
$$

where $\Delta _ { i } ( u )$ are predictable processes. 

This result is fundamental in financial mathematics because it implies that all sources of uncertainty in a complete market can be represented as integrals with respect to Brownian motions. In the context of derivative pricing, the theorem guarantees that any contingent claim (represented as a martingale under the risk-neutral measure) can be replicated by a dynamic trading strategy in the underlying assets. 

## 1.1.3 Lévy’s characterization of Brownian motion

Theorem 1.1.3 (Lévy). Let $M _ { 1 } ( t )$ and $M _ { 2 } ( t )$ be two continuous martingales with $M _ { 1 } ( 0 ) = M _ { 2 } ( 0 ) = 0$ satisfying 

$$
\langle M _ {1} \rangle (t) = t, \quad \langle M _ {2} \rangle (t) = t,
$$

and with zero cross-variation, 

$$
\langle M _ {1}, M _ {2} \rangle (t) = 0.
$$

Then $M _ { 1 } ( t )$ and $M _ { 2 } ( t )$ are independent standard Brownian motions. 

We give a brief outline of the proof using Itô’s formula. 

Proof. Let $f ( t , x , y )$ be a suficiently smooth function. Applying Itô’s formula to $f ( t , M _ { 1 } ( t ) , M _ { 2 } ( t ) )$ , we obtain 

$$
\begin{array}{l} d f (t, M _ {1} (t), M _ {2} (t)) \\ = f _ {t} (t, M _ {1} (t), M _ {2} (t))   d t + f _ {x} (t, M _ {1} (t), M _ {2} (t))   d M _ {1} (t) + f _ {y} (t, M _ {1} (t), M _ {2} (t))   d M _ {2} (t) \\ \quad + \frac {1}{2} f _ {x x} (t, M _ {1} (t), M _ {2} (t))   d \langle M _ {1} \rangle (t) + \frac {1}{2} f _ {y y} (t, M _ {1} (t), M _ {2} (t))   d \langle M _ {2} \rangle (t) \\ \quad + f _ {x y} (t, M _ {1} (t), M _ {2} (t))   d \langle M _ {1}, M _ {2} \rangle (t). \end{array}
$$

Using the given quadratic variation properties: 

$$
d \langle M _ {1} \rangle (t) = d t, \quad d \langle M _ {2} \rangle (t) = d t, \quad d \langle M _ {1}, M _ {2} \rangle (t) = 0,
$$

the formula simplifies to 

$$
d f (t, M _ {1} (t), M _ {2} (t)) = \left(f _ {t} + \frac {1}{2} f _ {x x} + \frac {1}{2} f _ {y y}\right) d t + f _ {x} d M _ {1} (t) + f _ {y} d M _ {2} (t).
$$

Integrate from 0 to T to obtain 

$$
f (T, M _ {1} (T), M _ {2} (T)) = f (0, 0, 0) + \int_ {0} ^ {T} \left(f _ {t} + \frac {1}{2} f _ {x x} + \frac {1}{2} f _ {y y}\right) d t + \int_ {0} ^ {T} f _ {x} d M _ {1} (t) + \int_ {0} ^ {T} f _ {y} d M _ {2} (t).
$$

Taking expectations and noting that the stochastic integrals have zero mean yields 

$$
\mathbb {E} \left[ f (T, M _ {1} (T), M _ {2} (T)) \right] = f (0, 0, 0) + \mathbb {E} \left[ \int_ {0} ^ {T} \left(f _ {t} + \frac {1}{2} f _ {x x} + \frac {1}{2} f _ {y y}\right) d t \right].
$$

Now, choose the test function 

$$
f (t, x, y) = \exp \left(\alpha x + \beta y - \frac {1}{2} (\alpha^ {2} + \beta^ {2}) t\right),
$$

which satisfies 

$$
f _ {t} + \frac {1}{2} f _ {x x} + \frac {1}{2} f _ {y y} = 0 \quad \mathrm{forall} \alpha , \beta \in \mathbb {R}.
$$

Thus, 

$$
\mathbb {E} \left[ \exp \left(\alpha M _ {1} (T) + \beta M _ {2} (T) - \frac {1}{2} (\alpha^ {2} + \beta^ {2}) T\right) \right] = 1,
$$

or equivalently, 

$$
\mathbb {E} \left[ \exp \left(\alpha M _ {1} (T) + \beta M _ {2} (T)\right) \right] = \exp \left(\frac {1}{2} (\alpha^ {2} + \beta^ {2}) T\right).
$$

This is exactly the moment generating function of two independent normal random variables with mean 0 and variance $T .$ Hence, $M _ { 1 } ( T )$ and $M _ { 2 } ( T )$ are independent standard Brownian motions. □ 

## 1.1.4 Girsanov’s theorem

In practice, one often needs to change the probability measure from the physical (or real-world) measure to a risk-neutral (or forward) measure. Girsanov’s theorem provides the framework for such transformations. 

## A discrete example

In a discrete-time setting, we illustrate these ideas using a simple binomial model. Consider a model based on three independent coin tosses. For each toss $i = { 1 , 2 , 3 }$ , let: 

• $H$ (“head”) occur with probability $p _ { i }$ under the physical measure $\mathbb { P } _ { : }$ 

$T \ ( ^ { \mathrm { 6 4 } } \mathrm { t a i l } ^ { \mathrm { 9 } } )$ occur with probability $q _ { i } = 1 - p _ { i }$ 

Under a change of measure, the probabilities become $\widetilde { p } _ { i }$ for heads and $\widetilde { q } _ { i } = 1 - \widetilde { p } _ { i }$ for tails. For instance, 

$$
p _ {1} \rightarrow \widetilde {p} _ {1}, \quad p _ {2} \rightarrow \widetilde {p} _ {2}, \quad p _ {3} \rightarrow \widetilde {p} _ {3}.
$$

A typical outcome is a sequence such as HHT, T T H, etc. One may, for example, let 

X := number of heads in the first two tosses. 

Under P, one has 

$$
\mathbb {P} (X = 2) = p _ {1} p _ {2}, \quad \mathbb {P} (X = 1) = \dots , \quad \mathbb {P} (X = 0) = \dots
$$

Details for the cases $X = 1$ and $X = 0$ are analogous. 

For a given outcome $\omega = ( \omega _ { 1 } , \omega _ { 2 } , \omega _ { 3 } ) \in \Omega$ , the Radon-Nikodym derivative, which transforms the physical measure $\mathbb { P }$ into the risk-neutral measure $\widetilde { \mathbb { P } } _ { : }$ , is defined as 

$$
Z _ {3} (\omega) = \frac {\widetilde {\mathbb {P}} (\omega)}{\mathbb {P} (\omega)}.
$$

For example: 

$\mathrm { I f } \ \omega = H H H$ , then 

$$
Z _ {3} (H H H) = \frac {\widetilde {p} _ {1} \widetilde {p} _ {2} \widetilde {p} _ {3}}{p _ {1} p _ {2} p _ {3}}.
$$

$\mathrm { I f } \omega = H H T .$ , then 

$$
Z _ {3} (H H T) = \frac {\widetilde {p} _ {1} \widetilde {p} _ {2} \widetilde {q} _ {3}}{p _ {1} p _ {2} q _ {3}}.
$$

Define the process $\{ Z _ { n } \} _ { n = 0 } ^ { 3 }$ by taking conditional expectations: 

$$
Z _ {n} := \mathbb {E} \left[ Z _ {3} \mid \mathcal {F} _ {n} \right], \quad n = 0, 1, 2, 3,
$$

with the initial value 

$$
Z _ {0} = \mathbb {E} [ Z _ {3} ].
$$

This process is a martingale with respect to the natural filtration $\{ \mathcal { F } _ { n } \}$ under $\mathbb { P } ;$ that is, 

$$
\mathbb {E} \left[ Z _ {n + 1} \mid \mathcal {F} _ {n} \right] = Z _ {n}.
$$

For example, using the tower property, 

$$
\mathbb {E} \left[ Z _ {3} \mid \mathcal {F} _ {1} \right] = \mathbb {E} \left[ \mathbb {E} \left[ Z _ {3} \mid \mathcal {F} _ {2} \right] \mid \mathcal {F} _ {1} \right] = Z _ {1}.
$$

In certain cases the conditional density may be computed explicitly. For instance, if the first two outcomes are $H H$ , one finds 

$$
Z _ {2} (H H) = \frac {\widetilde {p} _ {1} \widetilde {p} _ {2}}{p _ {1} p _ {2}},
$$

since regardless of the outcome of the third toss, $\widetilde { p } _ { 3 } + \widetilde { q } _ { 3 } = 1$ 

For any ${ \mathcal { F } } _ { 3 } .$ -measurable random variable $X$ , the expectation under the new measure $\widetilde { \mathbb { P } }$ is given by 

$$
\widetilde {\mathbb {E}} [ X ] = \sum_ {\omega \in \Omega} \widetilde {\mathbb {P}} (\omega) X (\omega) = \sum_ {\omega \in \Omega} Z _ {3} (\omega) \mathbb {P} (\omega) X (\omega) = \mathbb {E} [ Z _ {3} X ].
$$

Similarly, the Bayes rule for conditional expectations under the measure change is 

$$
\widetilde {\mathbb {E}} [ X \mid \mathcal {F} _ {s} ] = \frac {1}{Z _ {s}} \mathbb {E} [ Z _ {t} X \mid \mathcal {F} _ {s} ],
$$

for any $0 \leq s < t \leq 3$ . In particular, for $s = 1$ and $t = 2$ one obtains 

$$
\widetilde {\mathbb {E}} [ X \mid \mathcal {F} _ {1} ] = \frac {1}{Z _ {1}} \mathbb {E} [ Z _ {2} X \mid \mathcal {F} _ {1} ].
$$

This formula is fundamental when pricing derivatives under the risk-neutral measure since it relates the conditional expectation under the new measure to that under the original measure, adjusted by the density process. 

End of Lecture 1 

(Recap) Recall that under the measure change we have 

$$
\widetilde {\mathbb {P}} \left(\omega_ {1}, \omega_ {2}, \omega_ {3}\right) = Z _ {3} \left(\omega_ {1}, \omega_ {2}, \omega_ {3}\right) \mathbb {P} \left(\omega_ {1}, \omega_ {2}, \omega_ {3}\right).
$$

Thus, for any event $A \subseteq \Omega$ 

$$
\begin{array}{l} \widetilde {\mathbb {P}} (A) = \sum_ {\omega_ {1}, \omega_ {2}, \omega_ {3} \in A} \widetilde {\mathbb {P}} (\omega_ {1}, \omega_ {2}, \omega_ {3}) \\ = \sum_ {\omega_ {1}, \omega_ {2}, \omega_ {3} \in A} Z _ {3} (\omega_ {1}, \omega_ {2}, \omega_ {3})   \mathbb {P} (\omega_ {1}, \omega_ {2}, \omega_ {3}) = \mathbb {E} [ Z _ {3} \cdot \mathbb {1} _ {A} ]. \end{array}
$$

The Radon-Nikodym derivative $Z _ { 3 }$ satisfies the following: 

$$
\begin{array}{l} Z _ {3} > 0 \quad \text { almost   surely }, \\ \mathbb {E} \left[ Z _ {3} \right] = 1. \end{array}
$$

## §1.1. A review of the big theorems

For each i = 0, 1, 2, 3, define 

$$
Z _ {i} = \mathbb {E} \left[ Z _ {3} \mid \mathcal {F} _ {i} \right],
$$

so that $\{ Z _ { i } \} _ { i = 0 } ^ { 3 }$ forms a martingale under P. This martingale property is crucial, as it implies for any ${ \mathcal { F } } _ { j }$ -measurable random variable $X$ (with $j \geq i )$ , 

$$
\widetilde {\mathbb {E}} [ X ] = \mathbb {E} \left[ Z _ {i} \cdot X \right],
$$

and more generally, the Bayes rule for conditional expectations under the measure change becomes 

$$
\widetilde {\mathbb {E}} \left[ X \mid \mathcal {F} _ {i} \right] = \frac {1}{Z _ {i}} \mathbb {E} \left[ Z _ {j} \cdot X \mid \mathcal {F} _ {i} \right],
$$

for any $0 \leq i < j \leq 3$ and X $\mathcal { F } _ { j }$ -measurable. 

## Girsanov’s theorem in continuous time

Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space equipped with a filtration $\{ \mathcal { F } ( t ) \} _ { 0 \leq t \leq \bar { T } } .$ . Suppose there exists a random variable $Z ( \bar { T } )$ satisfying 

$$
Z (\bar {T}) > 0 \quad \text { a   .   s   . } \qquad \text { a   n   d } \qquad \mathbb {E} \left[ Z (\bar {T}) \right] = 1.
$$

Then one may define a new probability measure $\widetilde { \mathbb { P } }$ on $\mathcal { F } ( \bar { T } )$ by 

$$
\widetilde {\mathbb {P}} (A) = \mathbb {E} \left[ Z (\bar {T}) \cdot \mathbb {1} _ {A} \right], \quad \forall A \in \mathcal {F} (\bar {T}).
$$

For $0 \leq t \leq \bar { T }$ , define the process 

$$
Z (t) = \mathbb {E} \left[ Z (\bar {T}) \mid \mathcal {F} (t) \right],
$$

so that $\{ Z ( t ) \} _ { 0 \leq t \leq \bar { T } }$ is a P-martingale. In particular, for any $\mathcal { F } ( \bar { T } )$ -measurable random variable X one has 

$$
\widetilde {\mathbb {E}} [ X ] = \mathbb {E} \left[ X \cdot Z (\bar {T}) \right].
$$

Theorem 1.1.4 (Bayes’ rule in change-of-measure). Suppose that $\widetilde { \mathbb { P } }$ and $\mathbb { P }$ are two probability measures that are equivalent on $\mathcal { F } _ { T }$ with Radon-Nikodym derivative 

$$
Z (T) = \left. \frac {d \widetilde {\mathbb {P}}}{d \mathbb {P}} \right| _ {\mathcal {F} _ {T}},
$$

and denote 

$$
Z (t) = \left. \frac {d \widetilde {\mathbb {P}}}{d \mathbb {P}} \right| _ {\mathcal {F} _ {t}}.
$$

Then for any integrable random variable X and any $t \leq T$ , the conditional expectation under $\widetilde { \mathbb { P } }$ is given by 

$$
\widetilde {\mathbb {E}} [ X \mid \mathcal {F} _ {t} ] = \frac {\mathbb {E} \left[ Z (T) X \mid \mathcal {F} _ {t} \right]}{Z (t)}.
$$

(Equivalence of measure) Since $Z ( { \bar { T } } ) > 0 \mathrm { a . s }$ ., the new measure $\widetilde { \mathbb { P } }$ is equivalent to P. In fact, one may recover P from $\widetilde { \mathbb { P } }$ via 

$$
\mathbb {P} (A) = \widetilde {\mathbb {E}} \left[ \frac {1}{Z (\bar {T})} \cdot \mathbb {1} _ {A} \right], \quad \forall A \in \mathcal {F} (\bar {T}).
$$

Thus, if $\mathbb { P } ( A ) = 0 \ ( \mathrm { o r } \ 1 )$ then necessarily ${ \widetilde { \mathbb { P } } } ( A ) = 0 ~ ( \mathrm { o r } ~ 1 )$ , and if $\mathbb { P } ( A ) \in ( 0 , 1 )$ then $ { \widetilde { \mathbb { P } } } ( A ) \in ( 0 , 1 )$ 

## Girsanov’s theorem for one-dimensional Brownian motion

Let $\{ \mathcal { F } ( t ) \} _ { 0 \leq t \leq \bar { T } }$ be a filtration and let $W ( t )$ be a one-dimensional P-Brownian motion (BM). For any F(t)-adapted process $\theta ( t )$ , define 

$$
Z (\bar {T}) := \exp \left(- \int_ {0} ^ {\bar {T}} \theta (u) d W (u) - \frac {1}{2} \int_ {0} ^ {\bar {T}} \theta (u) ^ {2} d u\right).
$$

Then, by construction, $Z ( \bar { T } ) > 0$ almost surely and 

$$
\mathbb {E} \left[ Z (\bar {T}) \right] = 1.
$$

For $0 \leq t \leq \bar { T }$ one similarly defines 

$$
Z (t) = \mathbb {E} \left[ Z (\bar {T}) \mid \mathcal {F} (t) \right] = \exp \left(- \int_ {0} ^ {t} \theta (u) d W (u) - \frac {1}{2} \int_ {0} ^ {t} \theta (u) ^ {2} d u\right).
$$

(Martingale property) Set 

$$
Y (t) := - \int_ {0} ^ {t} \theta (u) d W (u) - \frac {1}{2} \int_ {0} ^ {t} \theta (u) ^ {2} d u,
$$

so that $Z ( t ) = e ^ { Y ( t ) }$ . Applying Itô’s formula to the function $f ( y ) = e ^ { y }$ (with $f ^ { \prime } ( y ) = e ^ { y }$ and $f ^ { \prime \prime } ( y ) = e ^ { y } )$ yields 

$$
d e ^ {Y (t)} = e ^ {Y (t)} d Y (t) + \frac {1}{2} e ^ {Y (t)} d \langle Y \rangle_ {t}.
$$

Since 

$$
d Y (t) = - \theta (t) d W (t) - \frac {1}{2} \theta (t) ^ {2} d t
$$

and the quadratic variation is 

$$
d \langle Y \rangle_ {t} = \theta (t) ^ {2} d t,
$$

we obtain 

$$
d e ^ {Y (t)} = - e ^ {Y (t)} \theta (t) d W (t) - \frac {1}{2} e ^ {Y (t)} \theta (t) ^ {2} d t + \frac {1}{2} e ^ {Y (t)} \theta (t) ^ {2} d t = - e ^ {Y (t)} \theta (t) d W (t).
$$

Thus, $Z ( t ) = e ^ { Y ( t ) }$ is a P-martingale. 

(Transformation of BM ) Under the new measure $\widetilde { \mathbb { P } }$ defined via $Z ( \bar { T } )$ , the process 

$$
\widetilde {W} (t) = W (t) + \int_ {0} ^ {t} \theta (u) d u
$$

plays a central role. In diferential form, 

$$
d \widetilde {W} (t) = d W (t) + \theta (t) d t.
$$

Using the Bayes rule and the properties of the density process $Z ( t )$ , one can show that $\widetilde { W } ( t )$ is a standard BM under $\widetilde { \mathbb { P } } ;$ that is, 

$$
\widetilde {\mathbb {E}} \left[ \widetilde {W} (t) \mid \mathcal {F} (s) \right] = \widetilde {W} (s), \quad \text { for   all } 0 \leq s <   t \leq \bar {T}.
$$

A key step in this verification is establishing that the process $\widetilde { W } ( t ) Z ( t )$ is a P-martingale. 

(Extension to the multidimensional case) For a d-dimensional BM $\mathbf { W } ( t ) = ( W _ { 1 } ( t ) , \ldots , W _ { d } ( t ) )$ and an adapted process $\pmb \theta ( t ) = ( \theta _ { 1 } ( t ) , \dots , \theta _ { d } ( t ) )$ , one defines 

$$
Z (\bar {T}) = \exp \left(- \sum_ {i = 1} ^ {d} \int_ {0} ^ {\bar {T}} \theta_ {i} (u) d W _ {i} (u) - \frac {1}{2} \sum_ {i = 1} ^ {d} \int_ {0} ^ {\bar {T}} \theta_ {i} (u) ^ {2} d u\right).
$$

Then, as before, $Z ( { \bar { T } } ) > 0 \ \mathrm { a . s . }$ . and $\mathbb { E } [ Z ( \bar { T } ) ] = 1$ ; the corresponding change of measure procedure and transformation of the BMs follow analogously. 

## Girsanov’s theorem in the Black-Scholes model

We consider a financial market consisting of a risky asset and a risk-free asset. The dynamics of the risky asset S(t) are given by 

$$
\begin{array}{c} d S (t) = \alpha (t) S (t)   d t + \sigma S (t)   d W (t), \\ \text {with} \sigma > 0 (\text {constant}) \text {and} \alpha (t) \text {an adapted process}, \end{array}
$$

where $S ( t )$ represents the adapted price of the risky asset. The risk-free asset is given by 

$$
1 \text {   } \longrightarrow e ^ {r t} \text {   }, \quad t \geq 0,
$$

meaning that an investment of 1 dollar grows to $e ^ { r t }$ dollars at time $t ^ { 1 }$ 

(Discrete trading) Let $X ( t _ { j } )$ denote the portfolio value at trading time $t _ { j }$ and let $\Delta ( t _ { j - 1 } )$ denote the number of shares held in the risky asset at time $t _ { j - 1 }$ . In a discrete setting, the change in the portfolio value over the interval from a previous trading time to time $t _ { j }$ is modeled as 

$$
X (t _ {j}) - X (t _ {j - 1}) = \Delta (t _ {j - 1}) \left(S (t _ {j}) - S (t _ {j - 1})\right) + r \left(X (t _ {j - 1}) - \Delta (t _ {j - 1}) S (t _ {j - 1})\right) (t _ {j} - t _ {j - 1}).
$$

In the limit of continuous trading, the portfolio dynamics become more tractable. 

(Continuous trading) Under continuous trading, the evolution of the portfolio value $X ( t )$ is governed by 

$$
d X (t) = \Delta (t) d S (t) + r \left(X (t) - \Delta (t) S (t)\right) d t.
$$

Example 1.1.5 (Hedging a European call option). Consider a European call option with payof 

$$
(S (T) - K) _ {+}.
$$

A hedging strategy consists of an initial capital $X ( 0 )$ and a trading strategy $\Delta ( t )$ such that the terminal portfolio value satisfies 

$$
X (T) = (S (T) - K) _ {+}.
$$

One may introduce a pricing function $c ( t , x )$ with the terminal condition 

$$
c (T, x) = (x - K) _ {+},
$$

and identify 

$$
c (t, S (t)) = X (t).
$$

(Delta-hedging strategy) A naive approach would attempt to equate the diferentials 

$$
d c (t, S (t)) \stackrel {!} {=} d X (t).
$$

A more efective strategy is to work with the discounted processes. In particular, one imposes 

$$
d \left(e ^ {- r t} c (t, S (t))\right) = d \left(e ^ {- r t} X (t)\right).
$$

Using Itô’s formula, the diferential of $e ^ { - r t } c ( t , S ( t ) )$ is computed as 

$$
\begin{array}{r l} & {d \left(e ^ {- r t} c (t, S (t))\right) = e ^ {- r t} d c (t, S (t)) + c (t, S (t)) d \left(e ^ {- r t}\right)} \\ & {\qquad = e ^ {- r t} \left[ c _ {t} d t + c _ {x} d S (t) + \frac {1}{2} c _ {x x} d S (t) ^ {2} \right] + c (t, S (t)) d \left(e ^ {- r t}\right)} \\ & {\qquad = e ^ {- r t} \left[ c _ {t} d t + c _ {x} (\alpha (t) S (t) d t + \sigma S (t) d W (t)) + \frac {1}{2} c _ {x x} \sigma^ {2} S (t) ^ {2} d t \right] + c (t, S (t)) d \left(e ^ {- r t}\right).} \end{array}
$$

Similarly, for the portfolio process we have 

$$
\begin{array}{r l} & d \left(e ^ {- r t} X (t)\right) = e ^ {- r t} d X (t) + X (t) d \left(e ^ {- r t}\right) \\ & \quad = e ^ {- r t} \left[ \Delta (t) (\alpha (t) S (t) d t + \sigma S (t) d W (t)) + r (X (t) - \Delta (t) S (t)) d t \right] + X (t) d \left(e ^ {- r t}\right). \end{array}
$$

By equating the coeficients of the $d W ( t )$ terms in the two expressions, we obtain 

$$
e ^ {- r t} c _ {x} \sigma S (t) = e ^ {- r t} \Delta (t) \sigma S (t).
$$

It immediately follows that 

$$
\Delta (t) = c _ {x} (t, S (t)).
$$

This is the delta-hedging rule in the Black-Scholes model. 

End of Lecture 2 

(Recap) Recall that under the physical measure P the dynamics of the underlying asset $S ( t )$ are given by 

$$
d S (t) = \alpha (t) S (t) d t + \sigma S (t) d W (t),
$$

where $\alpha ( t )$ is the (possibly time-dependent) drift, $\sigma > 0$ is the volatility, and $W ( t )$ is a standard Brownian motion. 

For a European call option with payof 

$$
(S (T) - K) ^ {+},
$$

we denote by $c ( t , S ( t ) )$ its price at time t. By applying Itô’s formula to $c ( t , S ( t ) )$ we obtain 

$$
d c (t, S (t)) = c _ {t} d t + c _ {x} d S (t) + \frac {1}{2} c _ {x x} d \langle S \rangle (t),
$$

and since 

$$
d \langle S \rangle (t) = \sigma^ {2} S (t) ^ {2} d t,
$$

this becomes 

$$
d c (t, S (t)) = \left[ c _ {t} + \alpha (t) S (t) c _ {x} + \frac {1}{2} \sigma^ {2} S (t) ^ {2} c _ {x x} \right] d t + \sigma S (t) c _ {x} d W (t).
$$

Now consider a replicating portfolio composed of $\Delta ( t )$ units of the asset and an amount invested in the risk-free asset (with constant rate r). Its value $X ( t )$ satisfies 

$$
d X (t) = \Delta (t) d S (t) + r (X (t) - \Delta (t) S (t)) d t.
$$

Matching the $d W ( t )$ terms between $\mathit { d c } ( t , S ( t ) )$ and $d X ( t )$ requires 

$$
\sigma S (t) c _ {x} = \Delta (t) \sigma S (t),
$$

so that 

$$
\Delta (t) = c _ {x} (t, S (t)).
$$

Matching the dt terms then yields 

$$
c _ {t} + \alpha (t) S (t) c _ {x} + \frac {1}{2} \sigma^ {2} S (t) ^ {2} c _ {x x} = r \left(c (t, S (t)) - S (t) c _ {x} (t, S (t))\right).
$$

A rearrangement shows that the call price must satisfy the Black-Scholes partial diferential equation (PDE) 

$$
c _ {t} + r S c _ {x} + \frac {1}{2} \sigma^ {2} S ^ {2} c _ {x x} - r \cdot c = 0,
$$

with the terminal condition 

$$
c (T, S) = (S - K) ^ {+}.
$$

(Risk-neutral measure via Girsanov’s theorem) In order to simplify pricing we seek a probability measure under which the discounted asset price process is a martingale. Under P the asset dynamics are 

$$
d S (t) = \alpha (t) S (t) d t + \sigma S (t) d W (t).
$$

We wish to find an equivalent (risk-neutral) measure $\widetilde { \mathbb { P } }$ under which the dynamics become 

$$
d S (t) = r S (t) d t + \sigma S (t) d \widetilde {W} (t),
$$

with r being the risk-free rate and $\widetilde { W } ( t )$ a Brownian motion under $\widetilde { \mathbb { P } } .$ 

To this end, define the process<sup>2</sup> 

$$
\theta (t) = \frac {\alpha (t) - r}{\sigma}.
$$

Then set 

$$
\widetilde {d W} (t) = d W (t) + \theta (t) d t.
$$

Substituting into the dynamics gives 

$$
d S (t) = \alpha (t) S (t) d t + \sigma S (t) \left[ d \widetilde {W} (t) - \theta (t) d t \right] = [ \alpha (t) - \sigma \theta (t) ] S (t) d t + \sigma S (t) d \widetilde {W} (t).
$$

Since 

$$
\alpha (t) - \sigma \theta (t) = \alpha (t) - (\alpha (t) - r) = r,
$$

we obtain the desired risk-neutral dynamics: 

$$
d S (t) = r S (t) d t + \sigma S (t) d \widetilde {W} (t).
$$

Girsanov’s theorem guarantees that the process 

$$
Z (T) = \exp \left(- \int_ {0} ^ {T} \theta (u) d W (u) - \frac {1}{2} \int_ {0} ^ {T} \theta (u) ^ {2} d u\right)
$$

is a P-martingale with $\mathbb { E } [ Z ( T ) ] = 1$ . We then define the risk-neutral measure $\widetilde { \mathbb { P } }$ by 

$$
\widetilde {\mathbb {P}} (A) = \mathbb {E} \left[ Z (T) \mathbb {1} _ {A} \right],
$$

for all $A \in { \mathcal { F } } ( T )$ 

Under $\widetilde { \mathbb { P } }$ the discounted asset price process 

$$
\widetilde {S} (t) = e ^ {- r t} S (t)
$$

is a martingale, and the pricing of derivatives is given by the risk-neutral valuation formula. 

Example 1.1.6 (Black-Scholes). Under the risk-neutral measure $\widetilde { \mathbb { P } }$ the European call price is given by 

$$
c (t, S (t)) = \widetilde {\mathbb {E}} \left[ e ^ {- r (T - t)} (S (T) - K) ^ {+} \mid \mathcal {F} _ {t} \right].
$$

Since the SDE 

$$
d S (t) = r S (t) d t + \sigma S (t) d \widetilde {W} (t)
$$

is linear, we can solve it by applying Itô’s formula to log $S ( t )$ . A short computation yields 

$$
d \log S (t) = \left(r - \frac {1}{2} \sigma^ {2}\right) d t + \sigma d \widetilde {W} (t).
$$

Integrating from t to T we obtain 

$$
\log S (T) = \log S (t) + \left(r - \frac {1}{2} \sigma^ {2}\right) (T - t) + \sigma (\widetilde {W} (T) - \widetilde {W} (t)).
$$

Thus, 

$$
S (T) = S (t) \exp \left[ \left(r - \frac {1}{2} \sigma^ {2}\right) (T - t) + \sigma \sqrt {T - t} Y \right],
$$

where 

$$
Y \sim \mathcal {N} (0, 1) \quad u n d e r \widetilde {\mathbb {P}}.
$$

Setting $x = S ( t )$ and performing the standard expectation calculation, we arrive at the Black-Scholes formula: 

$$
c (t, x) = x N (d _ {+}) - K e ^ {- r (T - t)} N (d _ {-}),
$$

with 

$$
d _ {\pm} = \frac {\ln (x / K) + (r \pm \frac {1}{2} \sigma^ {2}) (T - t)}{\sigma \sqrt {T - t}},
$$

and where $N ( \cdot )$ denotes the cumulative distribution function of the standard normal distribution. 

## 1.1.5 General models: the Brownian framework

We consider a general financial market model defined on a probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ with independent standard Brownian motions $W _ { 1 } , \ldots , W _ { d }$ . The primary asset prices $S _ { i } ( t )$ for $i = 1 , \ldots , m$ evolve according to 

$$
d S _ {i} (t) = S _ {i} (t) \alpha_ {i} (t) d t + S _ {i} (t) \sum_ {j = 1} ^ {d} \sigma_ {i j} (t) d W _ {j} (t),
$$

and there is an interest rate process R(t). All processes are assumed to be adapted. 

(Risk-free asset and discount process) The risk-free asset is given by 

$$
1 \text {   } \longrightarrow e ^ {\int_ {0} ^ {t} R (u) d u} \text {   } \text {   at   time   } t.
$$

Define the discount process by 

$$
D (t) = e ^ {- \int_ {0} ^ {t} R (u) d u}.
$$

Under a risk-neutral measure ${ \widetilde { \mathbb { P } } } ,$ the discounted primary asset prices $D ( t ) S _ { i } ( t )$ for $i = 1 , \ldots , m$ are required to be martingales. (It then follows that $D ( t ) X ( t )$ is also a martingale for any portfolio value $X ( t ) . )$ 

By applying the product rule, 

$$
\begin{array}{l} d \left(D (t) S _ {i} (t)\right) = D (t) d S _ {i} (t) + S _ {i} (t) d D (t) \\ = D (t) \left[ S _ {i} (t) \alpha_ {i} (t) d t + S _ {i} (t) \sum_ {j = 1} ^ {d} \sigma_ {i j} (t) d W _ {j} (t) \right] + S _ {i} (t) \underbrace {d D (t)} _ {\dots (t)}. \end{array}
$$

The condition that $D ( t ) S _ { i } ( t )$ is a $\widetilde { \mathbb { P } } _ { - \mathrm { m a r t i n g a l e } }$ implies that its drift term must vanish; that is, under $\widetilde { \mathbb { P } }$ 

$$
D (t) S _ {i} (t) \quad \text { has   only   the   stochastic   integral   term } \quad D (t) S _ {i} (t) \sum_ {j = 1} ^ {d} \sigma_ {i j} (t) d \widetilde {W} _ {j} (t).
$$

(Market price of risk) For the discounted price $D ( t ) S _ { i } ( t )$ to be a Pe-martingale, it is necessary that 

$$
\alpha_ {i} (t) d t + \sum_ {j = 1} ^ {d} \sigma_ {i j} (t) d W _ {j} (t) - R (t) d t
$$

has no drift under $\widetilde { \mathbb { P } } .$ This requirement leads to (recall that $d \widetilde { W } ( t ) = d W ( t ) + \theta ( t ) d t )$ 

$$
\alpha_ {i} (t) - R (t) = \sum_ {j = 1} ^ {d} \sigma_ {i j} (t) \underbrace {\theta_ {j} (t)} _ {\text { market   price   of   risk }},
$$

for $i = 1 , \ldots , m$ . These m equations, with d unknown processes $\theta _ { j } ( t )$ , are known as the market price of risk (MPR) equations. 

Theorem 1.1.7 (First fundamental theorem of asset pricing (FTAP)). A model is arbitrage free if and only if there exists a risk-neutral probability measure $\widetilde { \mathbb { P } } \ i f$ and only if the MPR equations 

$$
\alpha_ {i} (t) - R (t) = \sum_ {j = 1} ^ {d} \sigma_ {i j} (t) \theta_ {j} (t), \quad i = 1, \dots , m,
$$

have a solution. 

Example 1.1.8. Consider 

$$
\begin{array}{l} d S _ {1} (t) = \alpha_ {1} S _ {1} (t)   d t + \sigma_ {1} S _ {1} (t)   d W _ {1} (t), \\ d S _ {2} (t) = \alpha_ {2} S _ {2} (t)   d t + \sigma_ {2} S _ {2} (t)   d W _ {1} (t). \end{array}
$$

Here both assets are driven by the same Brownian motion. The claim is that 

$$
\text { arbitrage   free } \iff \text { Sharpe   ratio } _ {1} = \text { Sharpe   ratio } _ {2};
$$

that is, the model is arbitrage free if and only if the two assets have the same market price of risk. 

Completeness means that every contract written in terms of the primary assets can be replicated by a portfolio in these primary assets. For a portfolio with positions $\Delta _ { 1 } ( t ) , \ldots , \Delta _ { m } ( t )$ , the portfolio value $X ( t )$ evolves as 

$$
d X (t) = \sum_ {i = 1} ^ {m} \Delta_ {i} (t) d S _ {i} (t) - \left(X (t) - \sum_ {i = 1} ^ {m} \Delta_ {i} (t) S _ {i} (t)\right) R (t) d t.
$$

An arbitrage opportunity is a portfolio with $X ( 0 ) = 0$ and 

$$
X (T) \geq 0, \quad X (T) > 0 \text { with   positive   probability }.
$$

(One rules out arbitrage if under some equivalent measure $\hat { \mathbb { P } }$ the discounted portfolio value $D ( t ) X ( t )$ is a martingale.) 

Theorem 1.1.9 (Second FTAP). A model is complete if and only if the risk-neutral measure $\widetilde { \mathbb { P } }$ is unique $i f$ and only if the MPR equations have a unique solution, i.e., there exists a unique set of processes $\theta _ { 1 } ( t ) , \ldots , \theta _ { d } ( t )$ such that 

$$
\alpha_ {i} (t) - R (t) = \sum_ {j = 1} ^ {d} \sigma_ {i j} (t) \theta_ {j} (t), \quad 1 \leq i \leq m.
$$

End of Lecture 3 

We now present a counterexample to the completeness of a financial market. Example 1.1.10 illustrates that even if an asset (such as a stock) has dynamics similar to those in the Black-Scholes framework, introducing an additional source of randomness (here, via a stochastic interest rate) may render the market incomplete In an incomplete market, there exist infinitely many risk-neutral measures and not every contingent claim can be perfectly replicated by trading in the primary assets. 

Example 1.1.10 (Incomplete market). We consider a market with two primary sources of uncertainty driven by independent Brownian motions. The dynamics are given by: 

$$
d S (u) = \alpha   S (u) d u + \sigma   S (u)   d W _ {1} (u),
$$

$$
d R (u) = \mu d u + \nu \left(\rho d W _ {1} (u) + \sqrt {1 - \rho^ {2}} d W _ {2} (u)\right), \quad \rho \in (- 1, 1),
$$

where: 

$S ( u )$ is the asset (stock) price, 

$R ( u )$ is the (random) short $r a t e ,$ 

• α is the (constant) rate of return of the stock under the physical measure, 

$\sigma > 0$ is the volatility of the stock, 

• $\mu$ and ν are constants for the interest rate dynamics, 

$W _ { 1 } ( u )$ and $W _ { 2 } ( u )$ are two independent standard Brownian motions. 

An investor trading in the risky asset S and investing the remaining wealth at rate R holds a portfolio $X ( t )$ which evolves according to 

$$
d X (t) = \Delta (t) d S (t) + R (t) [ X (t) - \Delta (t) S (t) ] d t,
$$

where $\Delta ( t )$ denotes the position in the stock. 

(Risk-neutral measure perspective) To price derivatives, we introduce a discount process that reflects the accumulation of the (stochastic) short rate: 

$$
D (t) = \exp \left\{- \int_ {0} ^ {t} R (u) d u \right\}.
$$

The discounted portfolio value is given by $D ( t ) X ( t )$ . Using Itô’s product rule, 

$$
d (D (t) X (t)) = D (t) d X (t) + X (t) d D (t),
$$

and substituting the dynamics of $X ( t )$ and noting that $d D ( t ) = - R ( t ) D ( t ) d t$ , we obtain 

$$
\begin{array}{c} d \left(D (t) X (t)\right) = D (t) \left[ \Delta (t) d S (t) + R (t) (X (t) - \Delta (t) S (t)) d t \right] - R (t) D (t) X (t) d t \\ = D (t) \Delta (t) \left[ d S (t) - R (t) S (t) d t \right]. \end{array}
$$

Thus, $i f$ we can adjust the dynamics of $S$ so that 

$$
d S (u) = R (u) S (u) d u + \sigma   S (u) d \widetilde {W} _ {1} (u),
$$

the drift term in the discounted asset dynamics will vanish, and $D ( t ) X ( t )$ becomes a martingale under the new measure. 

This is achieved by introducing the Sharpe ratio 

$$
\Theta (u) = \frac {\alpha - R (u)}{\sigma},
$$

and applying Girsanov’s theorem. Under the change of measure defined by the Radon-Nikodym derivative 

$$
Z (t) = \exp \left\{- \int_ {0} ^ {t} \Theta (u) d W _ {1} (u) - \frac {1}{2} \int_ {0} ^ {t} \Theta (u) ^ {2} d u \right\},
$$

one obtains a new Brownian motion 

$$
\widetilde {W} _ {1} (t) = W _ {1} (t) + \int_ {0} ^ {t} \Theta (u) d u,
$$

so that under the risk-neutral measure $\widetilde { \mathbb { P } } _ { * }$ 

$$
d S (u) = R (u) S (u) d u + \sigma S (u) d \widetilde {W} _ {1} (u).
$$

Hence, the discounted portfolio value 

$$
d \left(D (t) X (t)\right) = D (t) \Delta (t) \sigma S (t) d \widetilde {W} _ {1} (t)
$$

is a martingale, ensuring the model is arbitrage-free, following the first FTAP (Theorem 1.1.7). 

The model becomes incomplete because there is a second source of randomness from $W _ { 2 } ( u )$ that does not afect the stock price dynamics directly. To see this, define a one-parameter family of Radon-Nikodym derivatives for any arbitrary constant $\boldsymbol { \hat { \theta } } \in \mathbb { R }$ 

$$
\widehat {Z} (t) = \exp \left\{- \int_ {0} ^ {t} \Theta (u) d W _ {1} (u) - \hat {\theta} W _ {2} (t) - \frac {1}{2} \int_ {0} ^ {t} \Theta (u) ^ {2} d u - \frac {1}{2} \hat {\theta} ^ {2} t \right\}.
$$

Then, by setting 

$$
\widehat {\mathbb {P}} (A) = \mathbb {E} \left[ \mathbb {1} _ {A} \widehat {Z} (\bar {T}) \right], \quad \forall A \in \mathcal {F} (\bar {T}),
$$

Girsanov’s theorem ensures that under $\widehat { \mathbb { P } }$ the processes 

$$
\widehat {W} _ {1} (t) = W _ {1} (t) + \int_ {0} ^ {t} \Theta (u) d u, \quad \widehat {W} _ {2} (t) = W _ {2} (t) + \hat {\theta} t
$$

are independent standard Brownian motions. Notice that 

$$
\widehat {W} _ {1} (t) = \widetilde {W} _ {1} (t),
$$

so that the stock dynamics remain 

$$
d S (u) = R (u) S (u) d u + \sigma S (u) d \widehat {W} _ {1} (u).
$$

Thus, $\widehat { \mathbb { P } }$ is also a risk-neutral measure since the discounted portfolio evolution becomes 

$$
d \left(D (t) X (t)\right) = D (t) \Delta (t) \sigma S (t) d \widehat {W} _ {1} (t).
$$

Because $\hat { \theta }$ can be chosen arbitrarily, there exist infinitely many risk-neutral measures. According to the second FTAP (Theorem 1.1.9), the existence of more than one risk-neutral measure implies that the market is incomplete. 

(Replication perspective) An equivalent way to see the incompleteness is through replication. Under any risk-neutral measure $( s a y , \widehat { \mathbb { P } } )$ , the stock dynamics are given by 

$$
d S (u) = R (u) S (u) d u + \sigma S (u) d \widehat {W} _ {1} (u).
$$

However, the interest rate $R ( u )$ still evolves as 

$$
d R (u) = \mu d u + \nu \left(\rho d W _ {1} (u) + \sqrt {1 - \rho^ {2}} d W _ {2} (u)\right),
$$

and after the change of measure the dynamics for $R ( u )$ involve both $\widehat { W } _ { 1 } ( u )$ and $\widehat { W } _ { 2 } ( u )$ . Since the stock price $S ( u )$ is driven only by $\widehat { W } _ { 1 } ( u )$ , any claim (for example, a European call with payof $( S ( T ) - K ) ^ { + } )$ will depend on both $S ( T )$ and $R ( u )$ . A hedging strategy based solely on trading the stock (and the money market account) can at best cancel the risk due to $\widehat { W } _ { 1 } ( u )$ (via delta hedging), but the risk associated with $\widehat { W } _ { 2 } ( u )$ remains unhedged. Consequently, perfect replication of such claims is impossible, confirming the market’s incompleteness. 

End of the first half of Lecture 5 

## Exercises

Exercise 1.1.11 (Decorrelating correlated BMs). Consider $B _ { 1 } ( t ) , \ldots , B _ { n } ( t )$ adapted to the same filtration $\mathcal { F } ( t )$ , with 

$$
d B _ {i} (t) d B _ {j} (t) = \rho_ {i j} d t
$$

where $\rho _ { i , i } = 1$ since $B _ { i } ( t )$ are Brownian motions. 

Define the correlation matrix C as 

$$
C = \left[ \begin{array}{c c c c} 1 & \rho_ {1, 2} & \dots & \rho_ {1, n} \\ \rho_ {2, 1} & 1 & \dots & \rho_ {2, n} \\ \vdots & \vdots & \ddots & \vdots \\ \rho_ {n, 1} & \rho_ {n, 2} & \dots & 1 \end{array} \right]
$$

Note that $C$ is symmetric. Let $\vec { B } ( t ) = ( B _ { 1 } ( t ) , \ldots , B _ { n } ( t ) ) ^ { \top }$ . Then we can express the quadratic covariation in matrix form as 

$$
d \vec {B} (t) d \vec {B} (t) ^ {\top} = C d t
$$

For any vector $V = ( v _ { 1 } , \ldots , v _ { n } ) ^ { \top } \in \mathbb { R } ^ { n }$ , the quadratic variation $o f V ^ { \top } \vec { B }$ satisfies 

$$
\begin{array}{l} d [ V ^ {\top} \vec {B}, V ^ {\top} \vec {B} ] _ {t} = \sum_ {i = 1} ^ {n} v _ {i}   d B _ {i} (t) \cdot \sum_ {j = 1} ^ {n} v _ {j}   d B _ {j} (t) \\ = \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} v _ {i} v _ {j}   d B _ {i} (t)   d B _ {j} (t) = \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} v _ {i} v _ {j}   \rho_ {i j}   d t = V ^ {\top} C V   d t \end{array}
$$

Since quadratic variation is non-decreasing, we have $V ^ { \top } C V \geq 0$ for all $V \in \mathbb { R } ^ { n }$ , which implies that C is positive semidefinite. 

By the spectral theorem, C has n orthogonal eigenvectors $\vec { v } _ { 1 } , \dotsc , \vec { v } _ { n }$ with corresponding non-negative eigenvalues $\lambda _ { 1 } \geq \lambda _ { 2 } \geq \cdot \cdot \cdot \geq \lambda _ { n } \geq 0$ . Without loss of generality, we can assume the eigenvectors are normalized so that 

$$
\vec {v} _ {i} ^ {\top} \vec {v} _ {j} = \delta_ {i j} = \left\{ \begin{array}{l l} 1 & \text {if i = j} \\ 0 & \text {if i\neq j} \end{array} \right.
$$

We can diagonalize C as 

$$
C = P \Lambda P ^ {\top}
$$

where $P = [ \vec { v } _ { 1 } \mid \vec { v } _ { 2 } \mid \cdot \cdot \cdot \mid \vec { v } _ { n } ]$ is the matrix of eigenvectors and $\boldsymbol { \Lambda } = d i a g ( \lambda _ { 1 } , \lambda _ { 2 } , \ldots , \lambda _ { n } )$ is the diagonal matrix of eigenvalues. From the orthonormality of eigenvectors, we have $P P ^ { \top } = P ^ { \top } P = I$ 

If any $\lambda _ { i } = 0$ , then $r a n k ( C ) < n ,$ , which would mean that some Brownian motion could be expressed as a linear combination of others. To ensure full independence, we assume $\lambda _ { i } > 0$ for all i. 

Now consider the process $\vec { W } ( t )$ defined by 

$$
\vec {W} (t) = \Lambda^ {- \frac {1}{2}} P ^ {\top} \vec {B} (t)
$$

We claim that $\vec { W } ( t ) = ( W _ { 1 } ( t ) , \ldots , W _ { n } ( t ) ) ^ { \top }$ consists of independent Brownian motions. To verify this using Lévy’s characterization theorem, we need to check: 

$W _ { i } ( 0 ) = 0$ for all i 

$W _ { i } ( t )$ has continuous sample paths 

$W _ { i } ( t )$ is a martingale 

$d \vec { W } ( t ) d \vec { W } ( t ) ^ { \top } = I d t$ 

The first three conditions follow directly from the properties of $\vec { B } ( t )$ and the linear transformation. For the fourth condition, we compute: 

$$
\begin{array}{r} d \vec {W} (t) d \vec {W} (t) ^ {\top} = \Lambda^ {- \frac {1}{2}} P ^ {\top} d \vec {B} (t) d \vec {B} (t) ^ {\top} P \Lambda^ {- \frac {1}{2}} = \Lambda^ {- \frac {1}{2}} P ^ {\top} C d t P \Lambda^ {- \frac {1}{2}} \\ = \Lambda^ {- \frac {1}{2}} P ^ {\top} P \Lambda P ^ {\top} P \Lambda^ {- \frac {1}{2}} d t = \Lambda^ {- \frac {1}{2}} \Lambda \Lambda^ {- \frac {1}{2}} d t = I d t \end{array}
$$

Therefore, by Lévy’s characterization theorem, $W _ { i } ( t )$ are independent standard Brownian motions. Conversely, we can express the original correlated Brownian motions as 

$$
\vec {B} (t) = P \Lambda^ {\frac {1}{2}} \vec {W} (t)
$$

which provides a way to construct correlated Brownian motions from independent ones. 

Exercise 1.1.12 (Change of measure on exponential r.v.). Recall that an exponential random variable with parameter $\lambda > 0$ has cumulative distribution function $F _ { \lambda } ( x ) = 1 - e ^ { - \lambda x } \ f o r \ x \ge 0$ 

The inverse of this function is given by $\begin{array} { r } { F _ { \lambda } ^ { - 1 } ( w ) = \frac { 1 } { \lambda } \ln \left( \frac { 1 } { 1 - w } \right) f o r 0 \leq w \leq 1 } \end{array}$ 

Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space where $\Omega = [ 0 , 1 ] , \mathcal { F } = \mathcal { B } ( [ 0 , 1 ] )$ is the Borel σ-algebra on [0, 1], and P is the Lebesgue measure on [0, 1], $i . e . , \mathbb { P } ( [ a , b ] ) = b - a f o r 0 \leq a \leq b \leq 1$ 

Define the random variable $X : \Omega \to \mathbb { R } _ { + }$ by $X ( w ) = F _ { \lambda } ^ { - 1 } ( w )$ for w ∈ Ω. 

Claim. X is an exponential random variable with parameter λ. 

Proof. For any $b \geq 0$ , we have 

$$
\begin{array}{r l} X (w) \leq b & \Longleftrightarrow \frac {1}{\lambda} \ln \left(\frac {1}{1 - w}\right) \leq b \Longleftrightarrow \ln \left(\frac {1}{1 - w}\right) \leq \lambda b \\ & \Longleftrightarrow \frac {1}{1 - w} \leq e ^ {\lambda b} \Longleftrightarrow 1 - w \geq e ^ {- \lambda b} \Longleftrightarrow w \leq 1 - e ^ {- \lambda b} \end{array}
$$

Therefore, 

$$
\begin{array}{c} F _ {X} (b) = \mathbb {P} (\{w \in \Omega : X (w) \leq b \}) \\ = \mathbb {P} ([ 0, 1 - e ^ {- \lambda b} ]) = 1 - e ^ {- \lambda b} \end{array}
$$

which is the CDF of an exponential random variable with parameter λ. 

Now, let $\widetilde { \lambda } > 0$ be another parameter. Define the random variable $Z : \Omega \to \mathbb { R } _ { + }$ by 

$$
Z (w) = \frac {\widetilde {\lambda}}{\lambda} e ^ {(\lambda - \widetilde {\lambda}) X (w)}
$$

We verify that 

$Z > 0 { : }$ since $\widetilde { \lambda } > 0 , \lambda > 0$ , and the exponential function is positive. 

$\mathbb { E } [ Z ] = 1$ where 

$$
\begin{array}{l} \mathbb {E} [ Z ] = \int_ {0} ^ {1} Z (w) d w \\ \qquad = \frac {\widetilde {\lambda}}{\lambda} \int_ {0} ^ {1} \exp \left\{(\lambda - \widetilde {\lambda}) \frac {1}{\lambda} \ln \left(\frac {1}{1 - w}\right) \right\} d w: \end{array}
$$

Making the substitution $\begin{array} { r } { x = F _ { \lambda } ^ { - 1 } ( w ) = \frac { 1 } { \lambda } \ln \left( \frac { 1 } { 1 - w } \right) } \end{array}$ , we have $w = 1 - e ^ { - \lambda x }$ and $d w = \lambda e ^ { - \lambda x } d x$ . The limits of integration change from $w \in [ 0 , 1 ]$ to $x \in [ 0 , \infty )$ . Thus, 

$$
\begin{array}{c} \mathbb {E} [ Z ] = \frac {\widetilde {\lambda}}{\lambda} \int_ {0} ^ {\infty} \exp \{(\lambda - \widetilde {\lambda}) x \} \lambda e ^ {- \lambda x} d x \\ = \widetilde {\lambda} \int_ {0} ^ {\infty} e ^ {- \widetilde {\lambda} x} d x = \widetilde {\lambda} \cdot \frac {1}{\widetilde {\lambda}} = 1, \end{array}
$$

as desired. 

Since $Z$ is a non-negative random variable with $\mathbb { E } [ Z ] = 1$ , we can define a new probability measure $\widetilde { \mathbb { P } }$ on $( \Omega , { \mathcal { F } } ) \ b y$ 

$$
\widetilde {\mathbb {P}} (A) = \mathbb {E} [ \mathbb {1} _ {A} \cdot Z ] = \int_ {A} Z (w) d w, \quad A \in \mathcal {F}
$$

For any interval $[ a , b ] \subset [ 0 , 1 ]$ , we compute 

$$
\widetilde {\mathbb {P}} ([ a, b ]) = \int_ {a} ^ {b} Z (w) d w = \frac {\widetilde {\lambda}}{\lambda} \int_ {a} ^ {b} \exp \left\{(\lambda - \widetilde {\lambda}) \frac {1}{\lambda} \ln \left(\frac {1}{1 - w}\right) \right\} d w
$$

Using the same substitution as before, we get 

$$
\begin{array}{l} \widetilde {\mathbb {P}} ([ a, b ]) = \frac {\widetilde {\lambda}}{\lambda} \int_ {F _ {\lambda} ^ {- 1} (a)} ^ {F _ {\lambda} ^ {- 1} (b)} \exp \{(\lambda - \widetilde {\lambda}) x \} \lambda e ^ {- \lambda x} d x \\ = \widetilde {\lambda} \int_ {F _ {\lambda} ^ {- 1} (a)} ^ {F _ {\lambda} ^ {- 1} (b)} e ^ {- \widetilde {\lambda} x} d x = \left[ - e ^ {- \widetilde {\lambda} x} \right] _ {F _ {\lambda} ^ {- 1} (a)} ^ {F _ {\lambda} ^ {- 1} (b)} = e ^ {- \widetilde {\lambda} F _ {\lambda} ^ {- 1} (a)} - e ^ {- \widetilde {\lambda} F _ {\lambda} ^ {- 1} (b)} \end{array}
$$

Substituting $\begin{array} { r } { F _ { \lambda } ^ { - 1 } ( w ) = \frac { 1 } { \lambda } \ln \left( \frac { 1 } { 1 - w } \right) } \end{array}$ , we obtain 

$$
\begin{array}{l} \widetilde {\mathbb {P}} ([ a, b ]) = \exp \left\{- \widetilde {\lambda} \cdot \frac {1}{\lambda} \ln \left(\frac {1}{1 - a}\right) \right\} - \exp \left\{- \widetilde {\lambda} \cdot \frac {1}{\lambda} \ln \left(\frac {1}{1 - b}\right) \right\} \\ = \exp \left\{- \frac {\widetilde {\lambda}}{\lambda} \ln \left(\frac {1}{1 - a}\right) \right\} - \exp \left\{- \frac {\widetilde {\lambda}}{\lambda} \ln \left(\frac {1}{1 - b}\right) \right\} = (1 - a) ^ {\frac {\widetilde {\lambda}}{\lambda}} - (1 - b) ^ {\frac {\widetilde {\lambda}}{\lambda}} \end{array}
$$

Finally, we show that under the probability measure ${ \widetilde { \mathbb { P } } } ,$ , the random variable X follows an exponential distribution with parameter $\widetilde { \lambda } .$ . 

For any $b \geq 0$ , we have 

$$
\widetilde {\mathbb {P}} (\{w \in \Omega : X (w) \leq b \}) = \widetilde {\mathbb {P}} ([ 0, 1 - e ^ {- \lambda b} ]) = \mathbb {E} [ \mathbb {1} _ {[ 0, 1 - e ^ {- \lambda b} ]} \cdot Z ] = \mathbb {E} [ \mathbb {1} _ {\{X \leq b \}} \cdot Z ]
$$

We can rewrite this expectation as an integral with respect to the density function of X under P: 

$$
\begin{array}{r l} & {\widetilde {\mathbb {P}} (\{w \in \Omega : X (w) \leq b \}) = \frac {\widetilde {\lambda}}{\lambda} \int_ {0} ^ {\infty} \mathbb {1} _ {[ 0, b ]} (x) e ^ {(\lambda - \widetilde {\lambda}) x} f _ {X} (x) d x} \\ & {\qquad = \frac {\widetilde {\lambda}}{\lambda} \int_ {0} ^ {b} e ^ {(\lambda - \widetilde {\lambda}) x} \lambda e ^ {- \lambda x} d x = \widetilde {\lambda} \int_ {0} ^ {b} e ^ {- \widetilde {\lambda} x} d x} \\ & {\qquad = \left[ - e ^ {- \widetilde {\lambda} x} \right] _ {0} ^ {b} = 1 - e ^ {- \widetilde {\lambda} b}} \end{array}
$$

Therefore, X is an exponential random variable with parameter $\widetilde { \lambda }$ under the probability measure $\widetilde { \mathbb { P } } .$ 

End of Recitation 1 

## 1.2 Pricing in the Markovian framework

Reference: [Shr04, §6]. 

In this section we develop the Markovian framework for option pricing. We begin by introducing stochastic diferential equations (SDEs) and the Markov property, which ensures that the future evolution of a process depends solely on its current state. This property underpins our derivation of pricing partial diferential equations (PDEs) via a systematic four-step procedure based on martingale arguments. We then illustrate the method through examples—ranging from the standard Black-Scholes and local volatility models to the more intricate Asian option pricing problem. Finally, we explore Kolmogorov’s forward and backward equations, culminating in the derivation of Dupire’s formula—a powerful tool that links the observed market surface of European option prices to the local volatility function. This chapter lays the theoretical groundwork for the numerical methods used in modern derivative pricing and calibration. 

## 1.2.1 Stochastic diferential equations and the Markov property

We begin with the definition of a stochastic diferential equation (SDE). Consider a stochastic process $X ( u )$ that satisfies an equation of the form: 

$$
d X (u) = \beta (u, X (u)) d u + \gamma (u, X (u)) d \widetilde {W} (u)
$$

where $\widetilde { W } ( u )$ is a standard Brownian motion, and $\beta ( u , X ( u ) )$ and $\gamma ( u , X ( u ) )$ are deterministic functions of time u and the process value $X ( u )$ . This specific structure is crucial, as it restricts the source of randomness to only the Brownian motion $\widetilde { W } ( u )$ 

The key consequence of this formulation is the Markov property: the future evolution of the process depends only on its current state, not on its past trajectory. More precisely, if we know $X ( u ) = x$ at some time $u ,$ then the future evolution of X depends only on this current value x and not on the path taken to reach this point. 

This property is particularly valuable for simulation purposes. When generating Monte Carlo paths of the process from a given time point u forward, we only need to know the value $X ( u )$ and not the entire history of the process. This significantly simplifies numerical implementations. 

The Markov property allows us to characterize the future distribution of the process through transition probabilities. For any time $T > u ,$ , the conditional distribution of $X ( T )$ given $X ( u ) = x$ can be described by the conditional cumulative distribution function (CDF): 

$$
\frac {d}{d y} \widetilde {\mathbb {P}} (X (T) \leq y \mid X (u) = x) =: p (u, x; T, y) \quad \text { pdf   in } y
$$

where $p ( u , x ; T , y )$ represents the transition probability density function (PDF) for moving from state x at time u to state y at time $T .$ . This transition PDF satisfies the following normalization condition: 

$$
\int p (u, x; T, y) d y = 1
$$

where the integration is over all possible values of y that the process can take at time $T .$ 

## 1.2.2 Derivation of pricing partial diferential equations (PDEs)

In the context of option pricing, we define the pricing function $g ( u , x )$ as the expected value of a payof function h applied to the process at the terminal time $T ,$ conditional on the process being at level x at time u: 

$$
g (u, x) := \widetilde {\mathbb {E}} [ h (X (T)) \mid X (u) = x ]
$$

In a model with zero interest rate, if X represents the underlying asset price, then $g ( u , x )$ is precisely the price of a European option with payof h at time u when the underlying asset is at level x. 

The pricing function can be expressed as an integral using the transition PDF: 

$$
g (u, x) = \int h (y) p (u, x; T, y) d y
$$

where the integration bounds depend on the range of possible values for the process $X$ 

To compute the pricing function $g ( u , x )$ , we can derive a partial diferential equation (PDE) that $g$ must satisfy. This is accomplished through the following four-step procedure: 

1. Find a martingale 

2. Take its diferential 

3. Set the dt-terms to 0 

4. Replace random variables by real variables 

The advantage of obtaining a PDE is that it can be solved using established numerical methods such as finite diferences, which are often more tractable than working directly with the original stochastic diferential equation. 

Let us now implement this procedure step by step. 

## Step 1: Find a martingale

We begin by constructing a martingale related to our pricing function. Consider the process 

$$
g (u, X (u)) = \widetilde {\mathbb {E}} [ h (X (T)) \mid X (u) ]
$$

Using the Markov property, we can rewrite this as 

$$
g (u, X (u)) = \widetilde {\mathbb {E}} [ h (X (T)) \mid \mathcal {F} (u) ]
$$

This is a martingale with respect to the filtration $\{ \mathcal { F } ( t ) \}$ . To verify this, let $\widetilde u < u$ and compute 

$$
\begin{array}{c} \widetilde {\mathbb {E}} [ g (u, X (u)) \mid \mathcal {F} (\widetilde {u}) ] = \widetilde {\mathbb {E}} [ \widetilde {\mathbb {E}} [ h (X (T)) \mid \mathcal {F} (u) ] \mid \mathcal {F} (\widetilde {u}) ] \\ = \widetilde {\mathbb {E}} [ h (X (T)) \mid \mathcal {F} (\widetilde {u}) ] = g (\widetilde {u}, X (\widetilde {u})) \end{array}
$$

The second equality follows from the tower property of conditional expectations. This confirms that $\{ g ( u , X ( u ) ) \} _ { 0 \leq u \leq T }$ is indeed a martingale. 

## Step 2: Take its diferential

Now we compute the diferential of $g ( u , X ( u ) )$ using Itô’s formula: 

$$
\begin{array}{l} d g (u, X (u)) \\ = g _ {u} (u, X (u)) d u + g _ {x} (u, X (u)) d X (u) + \frac {1}{2} g _ {x x} (u, X (u)) d X (u) d X (u) \\ = g _ {u} (u, X (u)) d u + g _ {x} (u, X (u)) [ \beta (u, X (u)) d u + \gamma (u, X (u)) d \widetilde {W} (u) ] + \frac {1}{2} g _ {x x} (u, X (u)) \gamma (u, X (u)) ^ {2} d u \\ = \left[ g _ {u} (u, X (u)) + \beta (u, X (u)) g _ {x} (u, X (u)) + \frac {1}{2} \gamma (u, X (u)) ^ {2} g _ {x x} (u, X (u)) \right] d u \\ \quad + g _ {x} (u, X (u)) \gamma (u, X (u)) d \widetilde {W} (u) \end{array}
$$

## Step 3: Set the dt-terms to 0

Since $g ( u , X ( u ) )$ is a martingale, its drift term must be zero: 

$$
g _ {u} (u, X (u)) + \beta (u, X (u)) g _ {x} (u, X (u)) + \frac {1}{2} \gamma (u, X (u)) ^ {2} g _ {x x} (u, X (u)) = 0
$$

## Step 4: Replace random Variables by real variables

Finally, we replace the random variable $X ( u )$ with the real variable x to obtain the PDE: 

$$
g _ {u} (u, x) + \beta (u, x) g _ {x} (u, x) + \frac {1}{2} \gamma (u, x) ^ {2} g _ {x x} (u, x) = 0
$$

This is the desired pricing PDE. The expression $\begin{array} { r } { \beta ( u , x ) g _ { x } ( u , x ) + \frac { 1 } { 2 } \gamma ( u , x ) ^ { 2 } g _ { x x } ( u , x ) } \end{array}$ is known as the infinitesimal generator of the stochastic process $X ( u )$ 

## 1.2.3 Boundary conditions for the pricing PDE

To obtain a unique solution to the pricing PDE, we need to specify appropriate boundary conditions. The domain of the PDE is typically a rectangular region: 

$$
\{(u, x) \in [ 0, T ] \times \mathcal {X} \}
$$

where $\mathcal { X }$ is the range of possible values for the process $X ( u )$ (which depends on the specific model). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/e65d9d41-4c7a-4366-aaab-be3784392ae9/082dc8c52b215f32354a5a4ac9a2635cb9d567d5dd565a68e43272d538a1b8f9.jpg)



Figure 1.2.1: Domain for the pricing PDE in the $( u , x )$ plane


We need to specify boundary conditions on three of the four sides of this domain (see an illustration in Figure 1.2.1): 

1. Terminal condition $( \mathrm { a t } ~ u = T )$ : This is straightforward since by definition 

$$
g (T, x) = h (x)
$$

This follows directly from the definition of $g .$ 

2. Boundary conditions (at the extremes of X ): These are more challenging and typically require careful consideration of the specific problem. For example, in the case of a call option on a nonnegative asset, one might consider: 

${ \mathrm { A t ~ } } x = 0 { \mathrm { : } }$ If the asset price is zero, the call option is worthless, so $g ( u , 0 ) = 0$ 

${ \mathrm { A s ~ } } x \to \infty { \mathrm { : } }$ For very large asset prices, the call option behaves asymptotically like the asset itself, so $g ( u , x ) \sim x - K e ^ { - r ( T - u ) } { \mathrm { ~ a s ~ } } x \to \infty .$ 

Without proper specification of these boundary conditions, the PDE has infinitely many solutions. The correct choice of boundary conditions ensures that the solution corresponds to the true option price. 

## Examples of the four-step procedure

We now apply the aforementioned framework to specific models, including European options in a local volatility model and Asian option pricing. 

Example 1.2.1 (Local volatility model). The local volatility model extends the standard Black-Scholes framework by allowing the volatility to be a deterministic function of both time and the current asset price, rather than a constant. Under the risk-neutral measure ${ \widetilde { \mathbb { P } } } ,$ the asset price dynamics are given by: 

$$
d S (t) = r S (t) d t + \sigma (t, S (t)) S (t) d \widetilde {W} (t)
$$

where $r$ is the constant risk-free rate, $\sigma ( t , S ( t ) )$ is the local volatility function, and $\widetilde { W } ( t )$ is a standard Brownian motion. 

This model was developed to address the limitations of the constant volatility assumption in the Black-Scholes model, particularly to account for the volatility smile observed in market option prices. The local volatility function can be calibrated to match market prices using Dupire’s formula. 

Our goal is to price a European call option with strike price K and maturity T. The option price at time t when the asset price is x is defined as 

$$
c (t, x) = \widetilde {\mathbb {E}} [ e ^ {- r (T - t)} (S _ {T} - K) ^ {+} \mid S (t) = x ]
$$

To derive the pricing PDE, we apply our four-step procedure. 

(Step 1) The discounted option price $e ^ { - r t } c ( t , S ( t ) )$ is a martingale under the risk-neutral measure. This follows from the risk-neutral pricing principle and the martingale property of discounted asset prices in a complete market. 

(Step 2) Using Itô’s formula and the product rule: 

$$
d (e ^ {- r t} c (t, S (t))) = e ^ {- r t} d c (t, S (t)) - r e ^ {- r t} c (t, S (t)) d t
$$

Applying Itô’s formula to $c ( t , S ( t ) )$ : 

$$
\begin{array}{r l} & {d c (t, S (t)) = c _ {t} (t, S (t)) d t + c _ {x} (t, S (t)) d S (t) + \frac {1}{2} c _ {x x} (t, S (t)) d S (t) d S (t)} \\ & {\qquad = c _ {t} (t, S (t)) d t + c _ {x} (t, S (t)) [ r S (t) d t + \sigma (t, S (t)) S (t) d \widetilde {W} (t) ]} \\ & {\qquad + \frac {1}{2} c _ {x x} (t, S (t)) \sigma (t, S (t)) ^ {2} S (t) ^ {2} d t} \end{array}
$$

Substituting back: 

$$
\begin{array}{l} d (e ^ {- r t} c (t, S (t))) = e ^ {- r t} \left[ c _ {t} (t, S (t)) + r S (t) c _ {x} (t, S (t)) + \frac {1}{2} \sigma (t, S (t)) ^ {2} S (t) ^ {2} c _ {x x} (t, S (t)) - r c (t, S (t)) \right] d t \\ \qquad + e ^ {- r t} c _ {x} (t, S (t)) \sigma (t, S (t)) S (t) d \widetilde {W} (t) \end{array}
$$

(Step 3) Since $e ^ { - r t } c ( t , S ( t ) )$ is a martingale, the coeficient of dt must vanish: 

$$
c _ {t} (t, S (t)) + r S (t) c _ {x} (t, S (t)) + \frac {1}{2} \sigma (t, S (t)) ^ {2} S (t) ^ {2} c _ {x x} (t, S (t)) - r c (t, S (t)) = 0
$$

(Step 4) The resulting PDE is: 

$$
c _ {t} (t, x) + r x c _ {x} (t, x) + \frac {1}{2} \sigma (t, x) ^ {2} x ^ {2} c _ {x x} (t, x) - r c (t, x) = 0
$$

This PDE generalizes the Black-Scholes equation, reducing to it when $\sigma ( t , x ) = \sigma \ ( c o n s t a n t )$ 

To obtain a unique solution, we need appropriate boundary conditions. 

1. Terminal condition $( a t t = T )$ 

$$
c (T, x) = (x - K) ^ {+}
$$

2. Lower boundary $( a t \ x = 0 )$ 

$$
c (t, 0) = 0
$$

When the asset price is zero, it remains at zero (an absorbing state), making the call option worthless. 

3. Upper boundary $( a s x  \infty ) .$ : For very large asset prices significantly above the strike, the call option is almost certainly going to expire in-the-money. The boundary condition is approximately: 

$$
\begin{array}{r l} & c (t, x) = \widetilde {\mathbb {E}} \left[ e ^ {- r (T - t)} (S _ {T} - K) ^ {+} \mid S (t) = x \right] \\ & \quad \approx \widetilde {\mathbb {E}} \left[ e ^ {- r (T - t)} (S _ {T} - K) \mid S (t) = x \right] \\ & \quad = \widetilde {\mathbb {E}} \left[ e ^ {- r (T - t)} S _ {T} \mid S (t) = x \right] - K e ^ {- r (T - t)} \\ & \quad = S (t) - K e ^ {- r (T - t)} = x - K e ^ {- r (T - t)} \end{array}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/e65d9d41-4c7a-4366-aaab-be3784392ae9/074dde6dedb7ad08ae1fab660b2b1c4f0c3c3971a8048d27b38fb3e010f70570.jpg)



Figure 1.2.2: Domain for the call option pricing PDE in the local volatility model


For numerical implementation, we truncate the domain at a suficiently large value of x (typically 2-3 standard deviations above the strike) where this approximation is accurate. 

The illustration is shown in Figure 1.2.2. The PDE is solved in the rectangular region $[ 0 , T ] \times [ 0 , x _ { \mathrm { m a x } } ]$ 9 where $x _ { \mathrm { m a x } }$ is chosen large enough for the upper boundary approximation to be valid. The terminal condition specifies values at $t = T$ , while the lower and upper boundaries provide conditions at $x = 0$ and $x = x _ { \mathrm { m a x } }$ respectively. 

Unlike the Black-Scholes model, the local volatility model typically does not admit closed-form solutions and must be solved numerically using finite diference or Monte Carlo methods. 

Here is a little bit of background on Asian options before we delve into our next example: Asian options difer from standard European options in that their payof depends on the average price of the underlying asset over a time period, rather than solely on the terminal price. This structure was originally developed in Japan for commodity markets to prevent price manipulation at maturity. Since manipulating prices over an extended period is significantly more dificult than at a single point in time, Asian options ofer reduced vulnerability to market distortions. 

Example 1.2.2 (Asian options). We consider an Asian call option in the standard Black-Scholes framework where the asset price follows: 

$$
d S (t) = r S (t) d t + \sigma S (t) d W (t)
$$

where $r > 0$ is the constant risk-free rate, $\sigma > 0$ is the constant volatility, and $W ( t )$ is a standard Brownian motion under the risk-neutral measure Pe. 

The payof of an Asian call option at maturity T is given by: 

$$
\left(\frac {1}{T} \int_ {0} ^ {T} S (u) d u - K\right) ^ {+}
$$

where K is the strike price and the expression represents the diference between the arithmetic average of the asset price over [0, T] and the strike, if positive. 

(State variables and pricing function) To determine the appropriate form of the pricing function, we need to identify the state variables that fully characterize the future distribution of the payof. Unlike European options where the current price $S ( t )$ is suficient, Asian options require tracking both the current price and the running average. 

Consider two scenarios at time t with the same current price S(t) but diferent price paths up to time t. Despite having identical S(t) values, these scenarios would have diferent running averages and consequently diferent option prices. Similarly, two scenarios with identical running averages but diferent current prices would also have diferent option values, as the future evolution depends on the current price. 

Therefore, we define the state variable $Y ( t )$ to represent the running sum: 

$$
Y (t) = \int_ {0} ^ {t} S (u) d u
$$

The price of the Asian option at time t is then a function of three variables: 

$$
c (t, x, y) = \widetilde {\mathbb {E}} \left[ e ^ {- r (T - t)} \left(\frac {1}{T} \int_ {0} ^ {T} S (u) d u - K\right) ^ {+} \mid S (t) = x, Y (t) = y \right]
$$

where x represents the current asset price and y represents the accumulated integral. 

(System of SDEs) The joint evolution of the state variables $( S ( t ) , Y ( t ) )$ forms a two-dimensional Markov process governed by the system: 

$$
\begin{array}{l} d S (t) = r S (t) d t + \sigma S (t) d W (t) \\ d Y (t) = S (t) d t \end{array}
$$

Following our four-step procedure: 

(Step 1) The discounted option price $e ^ { - r t } c ( t , S ( t ) , Y ( t ) )$ is a martingale under the risk-neutral measure. 

(Step 2) Using the product rule for $I t \hat { o } \ ' s$ formula: 

$$
d (e ^ {- r t} c (t, S (t), Y (t))) = e ^ {- r t} d c (t, S (t), Y (t)) - r e ^ {- r t} c (t, S (t), Y (t)) d t
$$

Applying Itô’s formula to $c ( t , S ( t ) , Y ( t ) )$ : 

$$
\begin{array}{l} d c (t, S (t), Y (t)) = c _ {t} (t, S (t), Y (t)) d t + c _ {x} (t, S (t), Y (t)) d S (t) + c _ {y} (t, S (t), Y (t)) d Y (t) \\ \qquad + \frac {1}{2} c _ {x x} (t, S (t), Y (t)) (d S (t)) ^ {2} \\ \qquad = c _ {t} (t, S (t), Y (t)) d t + c _ {x} (t, S (t), Y (t)) [ r S (t) d t + \sigma S (t) d W (t) ] \\ \qquad + c _ {y} (t, S (t), Y (t)) S (t) d t + \frac {1}{2} c _ {x x} (t, S (t), Y (t)) \sigma^ {2} S (t) ^ {2} d t \end{array}
$$

Substituting back: 

$$
\begin{array}{r l} & {d (e ^ {- r t} c (t, S (t), Y (t))) = e ^ {- r t} \Big [ c _ {t} (t, S (t), Y (t)) + r S (t) c _ {x} (t, S (t), Y (t))} \\ & {\qquad + S (t) c _ {y} (t, S (t), Y (t)) + \frac {1}{2} \sigma^ {2} S (t) ^ {2} c _ {x x} (t, S (t), Y (t)) - r c (t, S (t), Y (t)) \Big ] d t} \\ & {\qquad + e ^ {- r t} c _ {x} (t, S (t), Y (t)) \sigma S (t) d W (t)} \end{array}
$$

(Step 3) Since $e ^ { - r t } c ( t , S ( t ) , Y ( t ) )$ is a martingale, the coeficient of dt must vanish: 

$$
c _ {t} (t, S _ {t}, Y _ {t}) + r S (t) c _ {x} (t, S _ {t}, Y _ {t}) + S (t) c _ {y} (t, S _ {t}, Y _ {t}) + \frac {1}{2} \sigma^ {2} S (t) ^ {2} c _ {x x} (t, S _ {t}, Y _ {t}) - r c (t, S _ {t}, Y _ {t}) = 0
$$

(Step 4) The resulting PDE is: 

$$
c _ {t} (t, x, y) + r x c _ {x} (t, x, y) + x c _ {y} (t, x, y) + \frac {1}{2} \sigma^ {2} x ^ {2} c _ {x x} (t, x, y) - r c (t, x, y) = 0\tag{1.2.1}
$$

Equation 1.2.1 is known as the Feynman-Kac equation for the Asian option. The term $x c _ { y } ( t , x , y )$ arises from the evolution of the running sum $Y ( t )$ and distinguishes this PDE from the standard Black-Scholes equation. 

Again, to obtain a unique solution to the PDE, we need appropriate boundary conditions. Since we now have three variables $( t , x , y )$ , the domain is a three-dimensional box, and we need to specify conditions on its boundaries: 

1. Terminal condition $( a t t = T )$ 

$$
c (T, x, y) = \left(\frac {y + 0}{T} - K\right) ^ {+} = \left(\frac {y}{T} - K\right) ^ {+}
$$

This follows from the definition of the option payof. At maturity, the running sum $Y ( T )$ contains the complete integral needed for the average calculation. 

2. Boundary at $x = 0 { : }$ When the asset price reaches zero, it remains at zero (an absorbing state). The future contribution to the average will be zero, and the option value depends only on whether the current accumulated average exceeds the strike: 

$$
c (t, 0, y) = e ^ {- r (T - t)} \left(\frac {y}{T} - K\right) ^ {+}
$$

3. Boundary for large $x \ ( a s \ x \ \to \infty ) ;$ For very large asset prices, the average is almost certain to exceed the strike by a significant amount, and the option behaves asymptotically like the discounted diference between the expected average and the strike: 

$$
c (t, x, y) \approx \widetilde {\mathbb {E}} \left[ e ^ {- r (T - t)} \left(\frac {Y (T)}{T} - K\right) \Bigg | S (t) = x, Y (t) = y \right]
$$

This can be computed explicitly using the martingale property of the discounted price. 

4. Boundary for very negative y (mathematical extension): Although $Y ( t )$ represents a running sum of non-negative values in the original problem, the PDE remains mathematically valid for negative y values. For suficiently negative y, such that the terminal average will almost certainly be below the strike, the option is worthless: 

$$
c (t, x, y) \approx 0 \quad f o r y \ll 0
$$

This extension facilitates numerical solutions by providing a clear boundary condition. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/e65d9d41-4c7a-4366-aaab-be3784392ae9/b7cc9ccc415b7e0ca294f14fbfb68e8349ebec5449430e49b000fc99b340f66b.jpg)



Figure 1.2.3: Three-dimensional domain for the Asian option pricing PDE


An illustration is shown in Figure 1.2.3. The PDE must be solved in the interior of the box with boundary conditions specified on all sides. The terminal condition at $t = T$ provides the option payof, while additional conditions are needed at extremes of x and y. 

The complexity of this PDE generally precludes analytical solutions, necessitating numerical methods such as finite diferences or Monte Carlo simulation for practical implementation. 

Exercise 1.2.3 (A four-step procedure example). Consider the stochastic diferential equation 

$$
d X (u) = d W (u)
$$

with the initial condition $X ( t ) = x$ . Then $X ( T ) = x + W ( T ) - W ( t )$ . The transition density is given by 

$$
p (t, x; T, y) = \frac {1}{\sqrt {2 \pi (T - t)}} \exp \left\{- \frac {(y - x) ^ {2}}{2 (T - t)} \right\}
$$

Define the pricing function $g ( t , x ) = \widetilde { \mathbb { E } } [ h ( X ( T ) ) \mid X ( t ) = x ]$ , which implies $g ( T , x ) = h ( x )$ . Also, $g ( t , x )$ can be expressed as an integral: 

$$
g (t, x) = \int_ {- \infty} ^ {\infty} h (y) p (t, x; T, y) d y
$$

1. Consider $h ( y ) = y ^ { 2 }$ . Compute $g ( t , x )$ using two methods: 

(a) Direct computation using properties of conditional expectation: 

$$
\begin{array}{r l} & g (t, x) = \widetilde {\mathbb {E}} [ X ^ {2} (T) \mid X (t) = x ] = \widetilde {\mathbb {E}} [ (x + W (T) - W (t)) ^ {2} ] \\ & \qquad = x ^ {2} + 2 x \widetilde {\mathbb {E}} [ W (T) - W (t) ] + \widetilde {\mathbb {E}} [ (W (T) - W (t)) ^ {2} ] = x ^ {2} + T - t \end{array}
$$

The result follows since $\widetilde { \mathbb { E } } [ W ( T ) - W ( t ) ] = 0 \ a n d \ \widetilde { \mathbb { E } } [ ( W ( T ) - W ( t ) ) ^ { 2 } ] = T - t .$ 

(b) Integration using the transition density: 

$$
g (t, x) = \int_ {- \infty} ^ {\infty} y ^ {2} p (t, x; T, y) d y = \frac {1}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} y ^ {2} \exp \left\{- \frac {(y - x) ^ {2}}{2 (T - t)} \right\} d y
$$

Using the substitution $z = y - x$ , we have: 

$$
g (t, x) = \frac {1}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} (x + z) ^ {2} \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} d z = I _ {1} + I _ {2} + I _ {3}
$$

where 

$$
\begin{array}{l} {I _ {1} = \frac {1}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} x ^ {2} \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} d z = x ^ {2}} \\ {I _ {2} = \frac {1}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} 2 x z \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} d z = \frac {2 x}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} z \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} d z = 0} \end{array}
$$

The integral in $I _ { 2 }$ evaluates to zero because the integrand is an odd function. 

For $I _ { 3 }$ : 

$$
I _ {3} = \frac {1}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} z ^ {2} \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} d z = \frac {1}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} z \cdot z \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} d z
$$

Using integration by parts with $u = z$ and $\begin{array} { r } { d v = z \exp \{ - \frac { z ^ { 2 } } { 2 ( T - t ) } \} d z } \end{array}$ 

$$
\begin{array}{l} I _ {3} = \frac {1}{\sqrt {2 \pi (T - t)}} \left[ z \cdot - (T - t) \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} \right] _ {z = - \infty} ^ {z = \infty} \\ \qquad - \frac {1}{\sqrt {2 \pi (T - t)}} \int_ {- \infty} ^ {\infty} - (T - t) \exp \left\{- \frac {z ^ {2}}{2 (T - t)} \right\} d z \\ \qquad = 0 + (T - t) = T - t \end{array}
$$

Therefore, $g ( t , x ) = I _ { 1 } + I _ { 2 } + I _ { 3 } = x ^ { 2 } + 0 + ( T - t ) = x ^ { 2 } + T - t .$ 

2. Show that $g ( t , x )$ is a martingale and derive the corresponding PDE. 

To show $g ( t , X ( t ) )$ is a martingale, we need to verify: 

$$
\widetilde {\mathbb {E}} [ g (\tau , X (\tau)) \mid \mathcal {F} (s) ] = \widetilde {\mathbb {E}} [ \widetilde {\mathbb {E}} [ X ^ {2} (T) \mid \mathcal {F} (\tau) ] \mid \mathcal {F} (s) ] = \widetilde {\mathbb {E}} [ X ^ {2} (T) \mid \mathcal {F} (s) ] = g (s, X (s))
$$

for $s < \tau _ { : }$ where we used the tower property of conditional expectations. 

$T o$ derive the PDE, we apply Itô’s formula to $g ( t , X ( t ) )$ 

$$
\begin{array}{c} d g (t, X (t)) = g _ {t} (t, X (t))   d t + g _ {x} (t, X (t))   d X (t) + \frac {1}{2} g _ {x x} (t, X (t))   d t \\ = g _ {t} (t, X (t))   d t + g _ {x} (t, X (t))   d W (t) + \frac {1}{2} g _ {x x} (t, X (t))   d t \end{array}
$$

Since $g ( t , X ( t ) )$ is a martingale, the dt terms must sum to zero: 

$$
g _ {t} (t, X (t)) + \frac {1}{2} g _ {x x} (t, X (t)) = 0
$$

Replacing X(t) with $x ,$ we get the PDE: 

$$
g _ {t} (t, x) + \frac {1}{2} g _ {x x} (t, x) = 0, \quad \forall 0 \leq t \leq T, \forall x \in \mathbb {R}
$$

3. Verify that $g ( t , x ) = x ^ { 2 } + T - t$ satisfies the PDE. 

We compute the partial derivatives: 

$$
g _ {t} (t, x) = - 1, \qquad g _ {x x} (t, x) = 2
$$

Substituting into the PDE: 

$$
g _ {t} (t, x) + \frac {1}{2} g _ {x x} (t, x) = - 1 + \frac {1}{2} \cdot 2 = - 1 + 1 = 0
$$

Therefore, $g ( t , x ) = x ^ { 2 } + T - t$ satisfies the PDE. 

## Sidenotes

There are a lot of processes that are not Markovian. Below is an example. 

Example 1.2.4 (Non-Markovian process). Consider the process in Figure 1.2.4. Note that 

$$
\mathbb {E} [ S _ {3} \mid \mathcal {F} _ {2} ] (H T) = \frac {1}{1} \cdot 2 = 2, \quad \mathbb {E} [ S _ {3} \mid \mathcal {F} _ {2} ] (T H) = \frac {1}{2} \cdot 4 + \frac {1}{2} \cdot 4 = 4
$$

For the process to be Markov, only the value of $S _ { 2 }$ (namely 4) should matter for predicting $S _ { 3 }$ . There should exist a single function 

$$
g \left(2, S _ {2}\right) \quad s u c h t h a t \quad \mathbb {E} [ S _ {3} \mid \mathcal {F} _ {2} ] = g (2, 4),
$$

regardless of how $S _ { 2 }$ ended up being 4. 

But here, depending on whether $S _ { 2 } = 4$ came from HT or TH, we get diferent conditional expectations $( 2$ vs. 4). That shows no single function $g \left( 2 , 4 \right)$ can represent both of those conditional expectations. The only way you can correctly predict $\mathbb { E } [ S _ { 3 } \mid { \mathcal { F } } _ { 2 } ]$ is to look at more than just the current state $S _ { 2 } ;$ you need to know the path taken. That violates the Markov property. 

End of Recitation 2 

A common misconception is that every stochastic integral with respect to Brownian motion is normally distributed. This is not true in general, especially when the integrand is itself a random process. However, if the integrand is a deterministic function, then the stochastic integral is indeed normally distributed. Below, we illustrate both points. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/e65d9d41-4c7a-4366-aaab-be3784392ae9/31b86b2957248a75bf60c3916fc697af4928edc80ec002cb95e7b813551f34bd.jpg)



Figure 1.2.4: An example of a non-Markovian process


Example 1.2.5 (A stochastic integral that is not Gaussian). Consider the process 

$$
\int_ {0} ^ {t} W _ {u} d W _ {u}.
$$

Applying $I t { \hat { o } } ^ { \prime } s$ formula to $W _ { t } ^ { 2 }$ , we recall that 

$$
d (W _ {t} ^ {2}) = 2 W _ {t} d W _ {t} + 1 d t,
$$

so rearranging and integrating from 0 to t gives 

$$
\int_ {0} ^ {t} W _ {u} d W _ {u} = \frac {1}{2} W _ {t} ^ {2} - \frac {t}{2}.
$$

Since $W _ { t } ^ { 2 } \geq 0 ;$ , it follows that 

$$
\int_ {0} ^ {t} W _ {u} d W _ {u} \geq - \frac {t}{2}.
$$

A Gaussian random varia $. b l e ,$ in contrast, takes values in $( - \infty , \infty )$ with nonzero probability everywhere. Hence, $\textstyle \int _ { 0 } ^ { t } W _ { u } d W _ { u }$ cannot be normally distributed. Indeed, it is supported on $[ - \frac { t } { 2 } , \infty )$ and thus fails to have the full real line as its range of possible values. 

While integrals of the form $\begin{array} { r } { \int _ { 0 } ^ { t } \left( \mathrm { r a n d o m } \right) d W } \end{array}$ can yield a wide variety of distributions, there is a crucial special case in which the result is always Gaussian: 

Proposition 1.2.6. Let $\alpha ( \cdot )$ be a deterministic function on $[ 0 , t ]$ . Then 

$$
\int_ {0} ^ {t} \alpha (u) d W (u) \sim \mathcal {N} \left(0, \int_ {0} ^ {t} \alpha (u) ^ {2} d u\right).
$$

Proof outline. Define 

$$
Z _ {t} (\theta) = \exp \left\{\theta \int_ {0} ^ {t} \alpha (u) d W (u) \right\} \exp \left\{- \frac {1}{2} \theta^ {2} \int_ {0} ^ {t} \alpha (u) ^ {2} d u \right\}, \quad \theta \in \mathbb {R}.
$$

Itô’s lemma and the properties of stochastic exponentials show that $Z _ { t } ( \theta )$ is a martingale with $\mathbb { E } [ Z _ { 0 } ( \theta ) ] = 1$ Hence 

$$
\mathbb {E} [ Z _ {t} (\theta) ] = 1.
$$

Rewriting, 

$$
\mathbb {E} \left[ \exp \left\{\theta \int_ {0} ^ {t} \alpha (u) d W (u) \right\} \right] = \exp \left\{\frac {1}{2} \theta^ {2} \int_ {0} ^ {t} \alpha (u) ^ {2} d u \right\}.
$$

The right-hand side is precisely the moment generating function of a normal random variable with mean 0 and variance $\textstyle \int _ { 0 } ^ { t } \alpha ( u ) ^ { 2 }$ du. Consequently, 

$$
\int_ {0} ^ {t} \alpha (u) d W (u) \sim \mathcal {N} \left(0, \int_ {0} ^ {t} \alpha (u) ^ {2} d u\right).
$$

When $\alpha ( u )$ is deterministic, the stochastic integral behaves like a linear combination of (infinitesimal) normal increments with fixed coeficients, preserving normality. If $\alpha ( u )$ is random (for instance, depends on $W _ { u }$ or other random processes), then the distribution can deviate significantly from Gaussian. 

In finance, one can exploit this fact in models where the volatility $\sigma ( t )$ is purely a deterministic function of time. Then $\textstyle \int _ { 0 } ^ { t } { \boldsymbol { \sigma } } ( u ) d W ( u )$ is normal, leading to closed-form solutions (e.g. a version of the Black-Scholes formula for time-dependent volatility). 

## 1.2.4 Kolmogorov’s equations and Dupire’s formula

We now turn to a central topic in local volatility modeling: how to ensure that a chosen volatility function $\sigma ( t , x )$ can match all observed market prices of European options. This line of reasoning leads us toward Dupire’s formula, but first we need to establish the relevant Kolmogorov equations for transition densities. 

Consider the local volatility model: 

$$
d S (t) = r S (t) d t + \sigma (t, S (t)) S (t) d \widetilde {W} (t),
$$

where 

$S ( t )$ is the underlying asset price at time t, 

• r is a (constant) risk-free rate, 

$\sigma ( t , S ( t ) )$ is a local volatility function depending on both time t and the current price $S ( t )$ 2 

$\widetilde { W } ( t )$ is a Brownian motion under the risk-neutral measure. 

Our goal is to see how one might choose $\sigma ( t , x )$ so that this model reproduces the full market surface of European option prices (i.e. perfect calibration). Before deriving Dupire’s formula, we recall how transition densities evolve in Markov difusion models. 

## Kolmogorov’s forward and backward equations

A process $X ( t )$ governed by the SDE 

$$
d X (t) = \beta (t, X (t)) d t + \gamma (t, X (t)) d \widetilde {W} (t)
$$

is Markovian, and hence for any times $t < T$ , the distribution of $X ( T )$ given $X ( t ) = x$ can be described via a transition probability density function (PDF), 

$$
p (t, x; T, y) = \frac {d}{d y} \widetilde {\mathbb {P}} \left(X (T) \leq y \mid X (t) = x\right).
$$

In the local volatility setting for S(t), we similarly define 

$$
p (t, x; T, y) = \frac {d}{d y} \mathbb {P} (S (T) \leq y \mid S (t) = x).
$$

These transition densities satisfy two important PDEs known as the Kolmogorov equations: 

• Backward Kolmogorov equation (BKE): 

For (t, x) in the “backward” variables and fixed $( T , y )$ 2 

$$
p _ {t} (t, x; T, y) + \beta (t, x) p _ {x} (t, x; T, y) + \frac {1}{2} \gamma (t, x) ^ {2} p _ {x x} (t, x; T, y) = 0.\tag{1.2.2}
$$

Note that the Black-Scholes PDE emerges as a special case of this backward equation when $\beta ( t , x ) = r x$ and $\gamma ( t , x ) = \sigma x$ are constants in x (up to a factor x). 

• Forward Kolmogorov equation (FKE): 

For $( T , y )$ in the “forward” variables and fixed $( t , x )$ 

$$
p _ {T} (t, x; T, y) + \frac {\partial}{\partial y} [ \beta (T, y) p (t, x; T, y) ] - \frac {1}{2} \frac {\partial^ {2}}{\partial y ^ {2}} [ \gamma (T, y) ^ {2} p (t, x; T, y) ] = 0.\tag{1.2.3}
$$

In essence, the backward PDE treats $( t , x )$ as the evolving variables (with $( T , y )$ fixed), while the forward PDE treats $( T , y )$ as the evolving variables (with (t, x) fixed). 

Proof outline of the FKE. We prove by contradiction. Define 

$$
q (t, x; T, y) = p _ {T} (t, x; T, y) + [ \beta (T, y) p (t, x; T, y) ] _ {y} - \frac {1}{2} \left[ \gamma (T, y) ^ {2} p (t, x; T, y) \right] _ {y y}.
$$

Suppose that at some point $( t _ { 0 } , x _ { 0 } , T _ { 0 } , y _ { 0 } )$ , this quantity is not zero. By continuity, q will be strictly positive (or negative) on a small interval (a, b) around $y _ { 0 }$ 

Choose a smooth bump function $h ( y )$ with support in [a, b] such that 

$$
h (a) = h (b) = h ^ {\prime} (a) = h ^ {\prime} (b) = 0, \quad h (y) > 0 \text {   for   } y \in (a, b).
$$

The idea is to multiply q by this positive function h and integrate, then show that the integral must be both zero and strictly positive, a contradiction. 

Applying Itô’s formula to $h \left( X ( t ) \right)$ , one has 

$$
\begin{array}{l} h \left(X (T)\right) = h \left(X (t)\right) + \int_ {t} ^ {T} h ^ {\prime} (X (u))   \beta \left(u, X (u)\right)   d u \\ \qquad + \int_ {t} ^ {T} h ^ {\prime} (X (u))   \gamma \left(u, X (u)\right)   d \widetilde {W} (u) \\ \qquad + \frac {1}{2} \int_ {t} ^ {T} h ^ {\prime \prime} (X (u))   \gamma \left(u, X (u)\right) ^ {2}   d u, \end{array}
$$

then taking conditional expectations $\widetilde { \mathbb { E } } [ \cdot | X ( t _ { 0 } ) = x ]$ yields an integral representation involving the transition density $p ( t _ { 0 } , x ; T , y )$ 

By carefully rearranging terms (integration by parts in $y )$ , one arrives at 

$$
\int_ {a} ^ {b} h (y) p (t _ {0}, x; T _ {0}, y) d y = h (x) - \int_ {t _ {0}} ^ {T _ {0}} \int_ {a} ^ {b} (\beta p) _ {y} h (y) d y d t + \int_ {t _ {0}} ^ {T _ {0}} \int_ {a} ^ {b} \frac {1}{2} \left[ \gamma^ {2} p \right] _ {y y} h (y) d y d t.
$$

Now, by the Leibniz rule for parameter diferentiation under the integral sign, 

$$
\frac {\partial}{\partial T} \mathrm{LHS} = \int_ {a} ^ {b} h (y) \frac {\partial}{\partial T} p (t _ {0}, x; T, y) d y = \int_ {a} ^ {b} h (y) p _ {T} (t _ {0}, x; T, y) d y,
$$

where $p _ { T }$ denotes the partial derivative of $p$ with respect to the second time argument $T .$ For RHS on the other hand, the derivative of the constant term $h ( x )$ with respect to $T$ is 0. For the double integrals (from $t _ { 0 }$ to $T )$ , diferentiation with respect to the upper limit T picks out the integrand evaluated at $t = T$ Concretely, 

$$
\frac {d}{d T} \left[ - \int_ {t _ {0}} ^ {T} \int_ {a} ^ {b} h (y) [ \beta (t, y) p (\cdot) ] _ {y} d y d t \right] = - \int_ {a} ^ {b} h (y) [ \beta (T, y) p (t _ {0}, x; T, y) ] _ {y} d y.
$$

$$
\frac {d}{d T} \left[ \int_ {t _ {0}} ^ {T} \int_ {a} ^ {b} \frac {1}{2} h (y) [ \gamma^ {2} (t, y) p (\cdot) ] _ {y y} d y d t \right] = \int_ {a} ^ {b} \frac {1}{2} h (y) [ \gamma^ {2} (T, y) p (t _ {0}, x; T, y) ] _ {y y} d y.
$$

Putting these pieces together, we obtain: 

$$
\frac {\partial}{\partial T} (\mathrm{RHS}) = - \int_ {a} ^ {b} h (y) [ \beta (T, y) p (t _ {0}, x; T, y) ] _ {y} d y + \int_ {a} ^ {b} \frac {1}{2} h (y) [ \gamma^ {2} (T, y) p (t _ {0}, x; T, y) ] _ {y y} d y.
$$

Equating the derivatives of LHS and RHS gives: 

$$
\int_ {a} ^ {b} h (y) p _ {T} \left(t _ {0}, x; T, y\right) d y = - \int_ {a} ^ {b} h (y) \left[ \beta (T, y) p (\cdot) \right] _ {y} d y + \int_ {a} ^ {b} \frac {1}{2} h (y) \left[ \gamma^ {2} (T, y) p (\cdot) \right] _ {y y} d y.
$$

Rearrange terms: 

$$
\int_ {a} ^ {b} h (y) \left\{p _ {T} (t _ {0}, x; T, y) + [ \beta (T, y) p (t _ {0}, x; T, y) ] _ {y} - \frac {1}{2} [ \gamma^ {2} (T, y) p (t _ {0}, x; T, y) ] _ {y y} \right\} d y = 0.
$$

That is, by our initial definition, 

$$
\int_ {a} ^ {b} h (y) q \left(t _ {0}, x; T, y\right) d y = 0.
$$

By assumption, if $q$ is strictly positive (or strictly negative) on $( a , b )$ , and h is chosen to be strictly positive on $( a , b )$ , then $\textstyle \int _ { a } ^ { b } h ( y ) q ( \cdot ) d y \neq 0$ . However, the above integral identity says it must be 0. Contradiction! 

End of the second half of Lecture 5 

## Dupire’s formula

In the local volatility framework the asset dynamics are described by 

$$
d S (t) = r   S (t)   d t + \sigma (t, S (t))   S (t)   d \widetilde {W} (t),
$$

where $r$ is the constant risk-free rate and $\sigma ( t , S ( t ) )$ is the local volatility function. The key calibration question is: given the observed market prices of European call options, 

$$
c (0, S (0); T, K) = \widetilde {\mathbb {E}} \left[ e ^ {- r T} (S (T) - K) ^ {+} \right],
$$

how can we choose $\sigma$ so that the model reproduces these prices across all strikes K and maturities $T ?$ 

Dupire’s formula provides an explicit relationship between the call price surface and the local volatility function. In particular, it states that 

Theorem 1.2.7 (Dupire). 

$$
\sigma (T, K) ^ {2} = \frac {2 \left(c _ {T} (0 , S (0) ; T , K) + r K c _ {K} (0 , S (0) ; T , K)\right)}{K ^ {2} c _ {K K} (0 , S (0) ; T , K)},\tag{1.2.4}
$$

where $c _ { T } , \ : c _ { K }$ , and $c _ { K K }$ denote the partial derivatives of the call price with respect to the maturity $T ,$ , strike $K ,$ and the second derivative with respect to $K _ { i }$ , respectively. 

Before delving into the full derivation of this result, we illustrate its consistency with the classical Black-Scholes model. 

Example 1.2.8 (Consistency with the Black-Scholes model). Assume that the call price is given by the Black-Scholes formula: 

$$
c (0, S (0); T, K) = S (0) N (d _ {+}) - e ^ {- r T} K N (d _ {-}),
$$

with 

$$
d _ {\pm} = \frac {\log (S (0) / K) + \left(r \pm \frac {1}{2} \sigma^ {2}\right) T}{\sigma \sqrt {T}},
$$

where $\sigma$ is the constant volatility and $N ( \cdot )$ is the standard normal cumulative distribution function. 

When this call price is substituted into Dupire’s formula, one should recover the constant volatility, i.e., $\sigma ( T , K ) = \sigma$ . We verify as follows. A crucial relation in the Black-Scholes model is 

$$
S (0) N ^ {\prime} (d _ {+}) = e ^ {- r T} K N ^ {\prime} (d _ {-}),\tag{1.2.5}
$$

where $N ^ { \prime } ( \cdot )$ is the standard normal PDF. It can be derived by 

$$
\frac {N ^ {\prime} (d _ {+})}{N ^ {\prime} (d _ {-})} = \frac {e ^ {- d _ {+} ^ {2} / 2}}{e ^ {- d _ {-} ^ {2} / 2}} = e ^ {- (\log (S (0) / K) + r T)} = \frac {K}{S (0)} e ^ {- r T}.
$$

The partial derivatives of the call price are computed as: 

$$
c _ {T} = \frac {1}{2} S (0) N ^ {\prime} (d _ {+}) \frac {\sigma}{\sqrt {T}} + r e ^ {- r T} K N ^ {\prime} (d _ {-}), c _ {K} = - e ^ {- r T} N (d _ {-}), c _ {K K} = \frac {1}{K ^ {2} \sigma \sqrt {T}} S (0) N ^ {\prime} (d _ {+}).
$$

Substituting these expressions into Dupire’s formula 

$$
\sigma (T, K) ^ {2} = \frac {2 (c _ {T} + r K c _ {K})}{K ^ {2} c _ {K K}},
$$

straightforward algebra shows that the resulting local volatility equals the constant $\sigma .$ 

This confirms that Dupire’s formula is consistent with the Black-Scholes model when the market call prices are generated by Black-Scholes. 

In practical applications, the partial derivatives $c _ { T } , c _ { K }$ , and $c _ { K K }$ are estimated from a continuum of observed call option prices across strikes and maturities. The formula thus enables one to determine the local volatility surface that exactly matches the market prices, making it a powerful tool for calibration in equity markets. 

Derivation of Dupire’s formula. We begin with the risk-neutral pricing formula for a European call option: 

$$
c (0, S (0); T, K) = c (T, K) = \widetilde {\mathbb {E}} \left[ e ^ {- r T} (S (T) - K) ^ {+} \right] = e ^ {- r T} \int_ {K} ^ {\infty} (y - K) p (0, S (0); T, y) d y,
$$

where $p ( 0 , S ( 0 ) ; T , y )$ denotes the transition density of $S ( T )$ given $S ( 0 )$ . For notational simplicity, we drop the explicit dependence on the initial time and spot, writing $c ( T , K )$ and $p ( T , y )$ 

Diferentiating the call price with respect to T and K yields: 

$$
c _ {T} (T, K) = - r c (T, K) + e ^ {- r T} \int_ {K} ^ {\infty} (y - K) p _ {T} (T, y) d y,
$$

$$
c _ {K} (T, K) = e ^ {- r T} \int_ {K} ^ {\infty} (- p (T, y)) d y = - e ^ {- r T} \widetilde {\mathbb {P}} [ S (T) \geq K ],
$$

$$
c _ {K K} (T, K) = e ^ {- r T} p (T, K).
$$

Next, we recall the FKE (Equation 1.2.3) for a Markov process governed by 

$$
d X (u) = \beta (u, X (u)) d u + \gamma (u, X (u)) d \widetilde {W} (u).
$$

Its transition density $p ( t , x ; T , y )$ satisfies 

$$
q (T, y) := p _ {T} (T, y) + \frac {\partial}{\partial y} [ \beta (T, y) p (T, y) ] - \frac {1}{2} \frac {\partial^ {2}}{\partial y ^ {2}} [ \gamma (T, y) ^ {2} p (T, y) ] = 0.
$$

In the local volatility model we have 

$$
\beta (T, y) = r y \quad \text { and } \quad \gamma (T, y) = \sigma (T, y) y,
$$

so that the FKE becomes 

$$
q (T, y) = p _ {T} (T, y) + \frac {\partial}{\partial y} [ r y p (T, y) ] - \frac {1}{2} \frac {\partial^ {2}}{\partial y ^ {2}} [ \sigma (T, y) ^ {2} y ^ {2} p (T, y) ] = 0.
$$

The key insight is to multiply $q ( T , y )$ by the call payof $( y - K )$ and integrate over y from $K$ to $\infty :$ 

$$
0 = \int_ {K} ^ {\infty} (y - K) q (T, y) d y = A _ {1} + A _ {2} - \frac {1}{2} A _ {3},
$$

with 

$$
A _ {1} := \int_ {K} ^ {\infty} (y - K) p _ {T} (T, y) d y, \quad A _ {2} := \int_ {K} ^ {\infty} (y - K) \frac {\partial}{\partial y} [ r y p (T, y) ] d y,
$$

$$
A _ {3} := \int_ {K} ^ {\infty} (y - K) \frac {\partial^ {2}}{\partial y ^ {2}} \left[ \sigma (T, y) ^ {2} y ^ {2} p (T, y) \right] d y.
$$

By the definition of $c _ { T }$ we have $c _ { T } ( T , K ) = - r c ( T , K ) + e ^ { - r T } A _ { 1 }$ , or equivalently, 

$$
A _ {1} = e ^ {r T} \left[ c _ {T} (T, K) + r   c (T, K) \right].
$$

Integrate by parts with 

$$
u (y) = y - K \quad \text { and } \quad d v = \frac {\partial}{\partial y} \left[ r y   p (T, y) \right]   d y.
$$

Then, 

$$
A _ {2} = \left[ (y - K) r y p (T, y) \right] _ {y = K} ^ {y = \infty} - \int_ {K} ^ {\infty} 1 \cdot \left[ r y p (T, y) \right] d y.
$$

Assuming that the boundary term vanishes as $y  \infty$ and noting that at $y = K$ the factor $( y - K ) = 0 ;$ , it follows that 

$$
A _ {2} = - r \int_ {K} ^ {\infty} (y - K) p (T, y) d y + r K \int_ {K} ^ {\infty} p (T, y) d y.
$$

Recognizing that 

$$
e ^ {- r T} \int_ {K} ^ {\infty} (y - K) p (T, y) d y = c (T, K)
$$

and 

$$
e ^ {- r T} \int_ {K} ^ {\infty} p (T, y) d y = - c _ {K} (T, K),
$$

we can rewrite $A _ { 2 }$ as 

$$
A _ {2} = - r e ^ {- r T} c (T, K) + r K e ^ {r T} c _ {K} (T, K).
$$

A similar (double) integration by parts yields 

$$
A _ {3} = \sigma (T, K) ^ {2} K ^ {2} p (T, K).
$$

Since $c _ { K K } ( T , K ) = e ^ { - r T } p ( T , K )$ , it follows that 

$$
A _ {3} = \sigma (T, K) ^ {2} K ^ {2} e ^ {r T} c _ {K K} (T, K).
$$

(Combining the results) Substitute $A _ { 1 } , A _ { 2 }$ , and $A _ { 3 }$ back into the integrated FKE: 

$$
0 = e ^ {r T} \left[ c _ {T} (T, K) + r c (T, K) \right] + \left[ - r e ^ {- r T} c (T, K) + r K e ^ {r T} c _ {K} (T, K) \right] - \frac {1}{2} \sigma (T, K) ^ {2} K ^ {2} e ^ {r T} c _ {K K} (T, K).
$$

Dividing both sides by $e ^ { r T }$ yields 

$$
0 = c _ {T} (T, K) + r c (T, K) - r e ^ {- 2 r T} c (T, K) + r K c _ {K} (T, K) - \frac {1}{2} \sigma (T, K) ^ {2} K ^ {2} c _ {K K} (T, K).
$$

Noting that the discount factors cancel appropriately in the derivation, we obtain the final relation 

$$
c _ {T} (T, K) + r K c _ {K} (T, K) - \frac {1}{2} \sigma (T, K) ^ {2} K ^ {2} c _ {K K} (T, K) = 0.
$$

Solving for $\sigma ( T , K ) ^ { 2 }$ gives Dupire’s formula 

$$
\sigma (T, K) ^ {2} = \frac {2 \left(c _ {T} (T , K) + r K c _ {K} (T , K)\right)}{K ^ {2} c _ {K K} (T , K)}
$$

as desired. 

Conclusion of materials for the midterm 

## 1.3 Fixed income models

Reference: [Shr]. 

Thus far, our focus has been on equity pricing using a Markovian framework and the tools of stochastic calculus. Now we shift our attention to fixed income, where our aim is to explore continuous-time models that capture the dynamics of interest rates. In this chapter, we introduce the fundamental concepts underlying fixed income modeling—from the construction of yield curves and the definition of forward rates to the formulation of short rate models and their applications in pricing bonds and related interest rate derivatives. 

Our approach will demonstrate how the techniques of stochastic calculus can be applied to analyze and calibrate models in the fixed income arena, ultimately providing a unified framework for understanding the behavior of interest rate instruments in continuous time 

## 1.3.1 Yield curve and forward interest rates

Reference: [Shr, §1.1–1.3]. 

The term structure of interest rates is a central concept in fixed income markets. It is graphically represented by the yield curve—a function that maps maturities $T$ to their corresponding continuously compounded yields. At the initial time (commonly taken as $t = 0 )$ , the yield curve is observable and fixed. For example, the yields for bonds expiring one month, six months, one year, and so forth, are known. Importantly, the yield curve at time zero also satisfies $Y ( 0 , 0 ) = R ( 0 )$ , indicating that the yield for an infinitely short investment is the short rate. 

Figure 1.3.1 portrays two configurations of the yield curve. In the left panel, the curve $Y ( 0 , T )$ represents the known yields at time zero for various maturities T. In contrast, the right panel shows the yield curve $Y ( t , T )$ observed at a later time $t > 0 ;$ here, while the yield corresponding to the instantaneous maturity $T = t$ (which equals the short rate $R ( t ) )$ is still defined, the yields for $T > t$ are not predetermined but are random, reflecting future market uncertainty. This dynamic perspective is essential, as a primary objective in fixed income modeling is to describe how the entire curve $Y ( t , \cdot )$ evolves over time. 

Now, our goal is to develop a model for the evolution in time of the yield curve, i.e., to characterize how the function 

$$
Y (t, \cdot): T \mapsto Y (t, T)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/e65d9d41-4c7a-4366-aaab-be3784392ae9/c33d8d933d425cc571a3e4a70ab495e038a736304a4580104ae2cd83880a8649.jpg)



Figure 1.3.1: Illustration of the term structure at time 0 (left) and at a later time t (right).


changes with the time parameter t. 

Observation 1: correspondence between yields and bond prices. 

Let $B ( t , T )$ denote the price, at time t, of a non-defaultable zero-coupon bond that pays $\$ 1$ at maturity T. The yield $Y ( t , T )$ is defined through the relation 

$$
B (t, T) = e ^ {- Y (t, T) (T - t)} \quad \Longrightarrow \quad Y (t, T) = \frac {- \log B (t , T)}{T - t}.
$$

Thus, bond prices and yields are in one-to-one correspondence and knowledge of one determines the other. Observation 2: (instantaneous) forward interest rate. 

Another quantity of central importance is the (instantaneous) forward interest rate, $f ( t , T )$ . This rate is defined as the rate agreed upon at time t for a loan that starts at time T and spans a very short interval. 

(Derivation via a replicating portfolio) Consider constructing the following portfolio at time t: 

1. Long: One unit of the bond maturing at $T ,$ with price $B ( t , T )$ 

2. Short: $\frac { B ( t , T ) } { B ( t , T + \tau ) }$ units of the bond maturing at $T + \tau ,$ with price $B ( t , T + \tau )$ 

The initial net cost of the portfolio is zero. At time $T ,$ the long bond pays $1. At time $T + \tau$ the short position must be covered by paying 

$$
\frac {B (t , T)}{B (t , T + \tau)}.
$$

Interpreting this as a borrowing with an efective interest rate $f ( t , T , T + \tau )$ for the period of length τ , we equate 

$$
\begin{array}{c} 1 + \tau   f (t, T, T + \tau) = \frac {B (t , T)}{B (t , T + \tau)} \\ \Longrightarrow \qquad f (t, T, T + \tau) = \frac {\frac {B (t , T)}{B (t , T + \tau)} - 1}{\tau} = - \frac {B (t , T + \tau) - B (t , T)}{\tau} \cdot \frac {1}{B (t , T + \tau)}. \end{array}
$$

Definition 1.3.1. Taking the limit as $\tau  0$ defines the instantaneous forward rate: 

$$
f (t, T) = \lim _ {\tau \downarrow 0} f (t, T, T + \tau) = - \frac {\partial}{\partial T} B (t, T) \cdot \frac {1}{B (t , T)} = - \frac {\partial}{\partial T} \log B (t, T).\tag{1.3.1}
$$

In particular, setting $T = t$ recovers the short rate: 

$$
f (t, t) = R (t).
$$

Furthermore, integrating the forward rate yields 

$$
\int_ {t} ^ {T} f (t, u) d u = - \log B (t, T), \qquad \Longrightarrow \qquad B (t, T) = e ^ {- \int_ {t} ^ {T} f (t, u) d u}, 0 \leq t \leq T \leq \bar {T}.\tag{1.3.2}
$$

This demonstrates the one-to-one correspondence between bond prices, yields, and forward rates. Consequently, a model for any one of these quantities inherently provides models for the others. 

## 1.3.2 The Ho-Lee short rate model

Reference: [Shr, §1.5, 1.6]. 

The Ho-Lee model is one of the simplest short-rate models, and it ofers a framework for pricing fixed income securities by modeling the dynamics of the instantaneous short rate. Recall that the short rate is given by 

$$
R (t) = f (t, t).
$$

In the Ho-Lee model the short rate evolves according to 

$$
d R (t) = \alpha (t) d t + \sigma d \widetilde {W} (t),
$$

where: 

$\alpha ( t )$ is a deterministic function (often chosen to fit the initial term structure), 

$\underline { { \sigma } }$ is a constant, representing the absolute volatility of the short rate, 

$\Breve { W } ( t )$ is a Brownian motion under the risk-neutral measure. 

The risk-neutral pricing formula for a zero-coupon bond remains: 

$$
B (t, T) = \widetilde {\mathbb {E}} \left[ e ^ {- \int_ {t} ^ {T} R (u) d u} \Big | \mathcal {F} (t) \right] = \frac {1}{D (t)} \widetilde {\mathbb {E}} \left[ D (T) \Big | \mathcal {F} (t) \right],
$$

where $D ( t )$ is the discount factor. This implies that the discounted bond price, $D ( t ) B ( t , T )$ , is a $\widetilde { \mathbb { P } } _ { - }$ martingale. 

Due to the Markov property of the short rate process, the bond price can be expressed as a function of time and the current short rate: 

$$
B (t, T) = g (t, T, R (t)).
$$

A standard four-step procedure yields a partial diferential equation (PDE) for the function $g ( t , T , r )$ . Solving this PDE provides explicit bond pricing formulas within the Ho-Lee framework. 

We continue the analysis of the Ho-Lee model, where the short rate $R ( t )$ follows the dynamics under the risk-neutral measure $\overset { \smile } { \mathbb { P } } :$ 

$$
d R (t) = \alpha (t) d t + \sigma \widetilde {d W} (t),\tag{1.3.3}
$$

with $\alpha ( t )$ being a deterministic function of time and $\sigma > 0$ a constant volatility. $\widetilde { W } ( t )$ is a standard Brownian motion under $\widetilde { \mathbb { P } } .$ 

Our primary goal is to determine the price $B ( t , T )$ of a zero-coupon bond maturing at time $T$ with face value 1. The risk-neutral pricing formula gives: 

$$
B (t, T) = \widetilde {\mathbb {E}} \left[ e ^ {- \int_ {t} ^ {T} R (u) d u} \Big | \mathcal {F} (t) \right].
$$

Since the process $R ( t )$ is Markovian, the bond price $B ( t , T )$ depends only on the current time t and the current short rate $R ( t )$ , along with the maturity T. We denote this functional dependence as $B ( t , T ) = g ( t , R ( t ) ; T )$ We aim to find the pricing function $g ( t , r ; T )$ . 

We employ the standard four-step procedure for finding the pricing function associated with a Markovian short-rate model. 

Step 1: Identify a martingale. The discounted bond price, $D ( t ) B ( t , T )$ , where $D ( t ) = e ^ { - \int _ { 0 } ^ { t } R ( u ) d u }$ is the discount factor, is a martingale under $\widetilde { \mathbb { P } } .$ This follows directly from the tower property of conditional expectation applied to the pricing formula: 

$$
D (t) B (t, T) = D (t) \widetilde {\mathbb {E}} \left[ \frac {D (T)}{D (t)} \Big | \mathcal {F} (t) \right] = \widetilde {\mathbb {E}} [ D (T) \mid \mathcal {F} (t) ].
$$

Since $D ( T )$ is an $\mathcal { F } ( T )$ -measurable random variable, its conditional expectation process is a martingale. 

Step 2: Compute the martingale diferential. We apply Itô’s formula to $D ( t ) B ( t , T ) = D ( t ) g ( t , R ( t ) ; T )$ . Let $g = g ( t , R ( t ) ; T )$ . First, $d D ( t ) = - R ( t ) D ( t ) d t$ . Second, applying Itô’s lemma to $g ( t , R ( t ) ; T )$ considering $R ( t )$ as the stochastic variable and t as the time variable: 

$$
\begin{array}{c} {d g = g _ {t} d t + g _ {r} d R (t) + \frac {1}{2} g _ {r r} (d R (t)) ^ {2}} \\ {= \left(g _ {t} + g _ {r} \alpha (t) + \frac {1}{2} g _ {r r} \sigma^ {2}\right) d t + g _ {r} \sigma d \widetilde {W} (t).} \end{array}
$$

Using the product rule $d ( X Y ) = X d Y + Y d X + d X d Y$ 

$$
\begin{array}{r l} & {d (D (t) g) = D (t) d g + g d D (t) + (d D (t)) (d g)} \\ & {\qquad = D (t) \left[ \left(g _ {t} + g _ {r} \alpha (t) + \frac {1}{2} g _ {r r} \sigma^ {2}\right) d t + g _ {r} \sigma d \widetilde {W} (t) \right] + g (- R (t) D (t) d t) + 0} \\ & {\qquad = D (t) \left[ \left(g _ {t} + g _ {r} \alpha (t) + \frac {1}{2} g _ {r r} \sigma^ {2} - R (t) g\right) d t + g _ {r} \sigma d \widetilde {W} (t) \right].} \end{array}
$$

Step 3: Set the $d r i f t$ term to zero. Since $D ( t ) B ( t , T )$ is a Pe-martingale, the dt term in its diferential must be zero. Dividing by the non-zero factor $D ( t ) { \mathrm { : } }$ 

$$
g _ {t} + g _ {r} \alpha (t) + \frac {1}{2} g _ {r r} \sigma^ {2} - R (t) g = 0.
$$

Step 4: Formulate the PDE. Replacing the stochastic process $R ( t )$ with the state variable $r ,$ we obtain the partial diferential equation (PDE) for the bond pricing function $g ( t , r ; T )$ 

$$
g _ {t} (t, r) + \alpha (t) g _ {r} (t, r) + \frac {1}{2} \sigma^ {2} g _ {r r} (t, r) - r g (t, r) = 0.\tag{1.3.4}
$$

The terminal condition comes from the definition $B ( T , T ) = 1$ (bond price at maturity equals face value), so $g ( T , r ; T ) = 1$ for all $r .$ . 

Solving the PDE using the afine ansatz. The Ho-Lee model belongs to the class of afine term structure models. For such models, the bond pricing function typically takes an exponential-afine form. We make the ansatz: 

$$
g (t, r; T) = \exp [ - C (t, T) r - A (t, T) ],\tag{1.3.5}
$$

where $A ( t , T )$ and $C ( t , T )$ are deterministic functions of time t and maturity T. We compute the necessary partial derivatives: 

$$
g _ {t} = (- C _ {t} r - A _ {t}) g, \quad g _ {r} = - C g, \quad g _ {r r} = (- C) ^ {2} g = C ^ {2} g.
$$

Substituting these into the PDE (1.3.4): 

$$
(- C _ {t} r - A _ {t}) \not g + \alpha (t) (- C \not g) + \frac {1}{2} \sigma^ {2} (C ^ {2} \not g) - r \not g = 0.
$$

Rearranging and grouping terms by powers of $r :$ 

$$
r (- C _ {t} - 1) + \left(- A _ {t} - \alpha (t) C + \frac {1}{2} \sigma^ {2} C ^ {2}\right) = 0.
$$

Since this equation must hold for all values of $r ,$ the coeficients of r and the constant term must both independently be zero: 

$$
- C _ {t} (t, T) - 1 = 0\tag{1.3.6}
$$

$$
- A _ {t} (t, T) - \alpha (t) C (t, T) + \frac {1}{2} \sigma^ {2} C (t, T) ^ {2} = 0\tag{1.3.7}
$$

The terminal condition $g ( T , r ; T ) = 1$ implies $\exp [ - C ( T , T ) r - A ( T , T ) ] = 1$ for all r. This requires the exponent to be zero, leading to the terminal conditions for the ODEs: 

$$
C (T, T) = 0, \qquad A (T, T) = 0.
$$

Solving the ODE for $C ( t , T ) ~ \left( 1 . 3 . 6 \right)$ with $C ( T , T ) = 0 \colon { \cal C } _ { t } = - 1 \Longrightarrow C ( t , T ) = - t + K ( T )$ . Using $C ( T , T ) = 0$ , we $\mathrm { g e t } - T + K ( T ) = 0 \implies K ( T ) = T$ . Thus, $C ( t , T ) = T - t .$ 

Substitute $C ( t , T ) = T - t$ into the ODE for A(t, T) (1.3.7): 

$$
- A _ {t} (t, T) - \alpha (t) (T - t) + \frac {1}{2} \sigma^ {2} (T - t) ^ {2} = 0 \quad \Longrightarrow \quad A _ {t} (t, T) = - \alpha (t) (T - t) + \frac {1}{2} \sigma^ {2} (T - t) ^ {2}.
$$

Integrating from t to T using $A ( T , T ) = 0 ;$ 

$$
A (t, T) = - \int_ {t} ^ {T} \left(- \alpha (u) (T - u) + \frac {1}{2} \sigma^ {2} (T - u) ^ {2}\right) d u = \int_ {t} ^ {T} \alpha (u) (T - u) d u - \int_ {t} ^ {T} \frac {1}{2} \sigma^ {2} (T - u) ^ {2} d u.
$$

The second integral can be computed explicitly: 

$$
\int_ {t} ^ {T} \frac {1}{2} \sigma^ {2} (T - u) ^ {2} d u = \frac {1}{2} \sigma^ {2} \left[ - \frac {(T - u) ^ {3}}{3} \right] _ {t} ^ {T} = \frac {1}{2} \sigma^ {2} \left(0 - (- \frac {(T - t) ^ {3}}{3})\right) = \frac {1}{6} \sigma^ {2} (T - t) ^ {3}.
$$

So, 

$$
A (t, T) = \int_ {t} ^ {T} \alpha (u) (T - u) d u - \frac {1}{6} \sigma^ {2} (T - t) ^ {3}.
$$

Plugging $A ( t , T )$ and $C ( t , T )$ back into the ansatz (1.3.5), the bond price is: 

$$
B (t, T) = g (t, R (t); T) = \exp \left[ - (T - t) R (t) - \int_ {t} ^ {T} \alpha (u) (T - u) d u + \frac {1}{6} \sigma^ {2} (T - t) ^ {3} \right].\tag{1.3.8}
$$

(Yield calculation) The continuously compounded yield $Y ( t , T )$ is defined by $B ( t , T ) = e ^ { - ( T - t ) Y ( t , T ) }$ . Comparing with (1.3.8): 

$$
- (T - t) Y (t, T) = - (T - t) R (t) - \int_ {t} ^ {T} \alpha (u) (T - u) d u + \frac {1}{6} \sigma^ {2} (T - t) ^ {3}.
$$

Dividing by $- ( T - t )$ 

$$
Y (t, T) = R (t) + \frac {1}{T - t} \int_ {t} ^ {T} \alpha (u) (T - u) d u - \frac {1}{6} \sigma^ {2} (T - t) ^ {2}.\tag{1.3.9}
$$

(Bond price dynamics) To find $d B ( t , T )$ , we first find the dynamics of the exponent in (1.3.8). Let 

$$
Y _ {\mathrm{exp}} (t) = - (T - t) R (t) - \int_ {t} ^ {T} \alpha (u) (T - u) d u + \frac {1}{6} \sigma^ {2} (T - t) ^ {3}.
$$

Applying Itô’s lemma and Leibniz rule: 

$$
\begin{array}{l} d Y _ {\mathrm{exp}} (t) = d (- (T - t) R (t)) - d \left(\int_ {t} ^ {T} \alpha (u) (T - u) d u\right) + d \left(\frac {1}{6} \sigma^ {2} (T - t) ^ {3}\right) \\ \qquad = - [ (T - t) d R (t) + R (t) d (T - t) + d (T - t) d R (t) ] - [ - \alpha (t) (T - t) d t ] + \frac {1}{6} \sigma^ {2} \cdot 3 (T - t) ^ {2} (- 1) d t \\ \qquad = - [ (T - t) (\alpha (t) d t + \sigma d \widetilde {W} (t)) + R (t) (- d t) + 0 ] + \alpha (t) (T - t) d t - \frac {1}{2} \sigma^ {2} (T - t) ^ {2} d t \\ \qquad = - (T - t) \alpha (t) d t - (T - t) \sigma d \widetilde {W} (t) + R (t) d t + \alpha (t) (T - t) d t - \frac {1}{2} \sigma^ {2} (T - t) ^ {2} d t \\ \qquad = \left(R (t) - \frac {1}{2} \sigma^ {2} (T - t) ^ {2}\right) d t - (T - t) \sigma d \widetilde {W} (t). \end{array}
$$

## §1.3. Fixed income models

Now, applying Itô’s lemma to $B ( t , T ) = e ^ { Y _ { \mathrm { e x p } } ( t ) }$ 

$$
\begin{array}{l} d B (t, T) = B (t, T) d Y _ {\mathrm{exp}} (t) + \frac {1}{2} B (t, T) (d Y _ {\mathrm{exp}} (t)) ^ {2} \\ \qquad = B (t, T) \left[ \left(R (t) - \frac {1}{2} \sigma^ {2} (T - t) ^ {2}\right) d t - (T - t) \sigma d \widetilde {W} (t) \right] + \frac {1}{2} B (t, T) (- (T - t) \sigma d \widetilde {W} (t)) ^ {2} \\ \qquad = B (t, T) \left[ \left(R (t) - \frac {1}{2} \sigma^ {2} (T - t) ^ {2}\right) d t - (T - t) \sigma d \widetilde {W} (t) \right] + \frac {1}{2} B (t, T) (T - t) ^ {2} \sigma^ {2} d t. \end{array}
$$

The $\sigma ^ { 2 }$ terms cancel, yielding the bond price dynamics under $\widetilde { \mathbb { P } } \mathrm { : }$ 

$$
d B (t, T) = R (t) B (t, T) d t - (T - t) \sigma B (t, T) d \widetilde {W} (t).\tag{1.3.10}
$$

This confirms that the expected instantaneous return under $\widetilde { \mathbb { P } }$ is $R ( t )$ . The term $- ( T - t ) \sigma$ represents the bond price volatility. 

(Discounted bond price dynamics) Using $d ( D ( t ) B ( t , T ) ) ~ = ~ D ( t ) d B ( t , T ) + B ( t , T ) d D ( t )$ , we substitute (1.3.10) and $d D ( t ) = - R ( t ) D ( t ) d t \colon$ 

$$
\begin{array}{r l} & d (D (t) B (t, T)) = D (t) [ R (t) B (t, T) d t - (T - t) \sigma B (t, T) d \widetilde {W} (t) ] + B (t, T) [ - R (t) D (t) d t ] \\ & \qquad = D (t) B (t, T) R (t) d t - D (t) B (t, T) (T - t) \sigma d \widetilde {W} (t) - D (t) B (t, T) R (t) d t \\ & \qquad = - D (t) B (t, T) (T - t) \sigma d \widetilde {W} (t). \end{array}
$$

This is an SDE of the form $d X _ { t } = X _ { t } \Theta ( t ) d \widetilde { W } ( t )$ with $\Theta ( t ) = - ( T - t ) \sigma$ . The solution is given by the stochastic exponential: 

$$
D (t) B (t, T) = B (0, T) \exp \left(\int_ {0} ^ {t} - (T - u) \sigma d \widetilde {W} (u) - \frac {1}{2} \int_ {0} ^ {t} (- (T - u) \sigma) ^ {2} d u\right).\tag{1.3.11}
$$

(Forward rate calculation) The instantaneous forward rate $f ( t , T )$ is related to the bond price by $f ( t , T ) =$ $\begin{array} { r } { - \frac { \partial } { \partial T } \log B ( t , T ) } \end{array}$ . Using the formula (1.3.8): 

$$
\begin{array}{r l} & {\log B (t, T) = - (T - t) R (t) - \int_ {t} ^ {T} \alpha (u) (T - u) d u + \frac {1}{6} \sigma^ {2} (T - t) ^ {3}} \\ & {\frac {\partial}{\partial T} \log B (t, T) = - R (t) - \frac {\partial}{\partial T} \left(\int_ {t} ^ {T} \alpha (u) (T - u) d u\right) + \frac {1}{6} \sigma^ {2} \cdot 3 (T - t) ^ {2}} \\ & {\qquad = - R (t) - \left[ \alpha (T) (T - T) + \int_ {t} ^ {T} \alpha (u) \frac {\partial}{\partial T} (T - u) d u \right] + \frac {1}{2} \sigma^ {2} (T - t) ^ {2}} \\ & {\qquad = - R (t) - \left[ 0 + \int_ {t} ^ {T} \alpha (u) d u \right] + \frac {1}{2} \sigma^ {2} (T - t) ^ {2} = - R (t) - \int_ {t} ^ {T} \alpha (u) d u + \frac {1}{2} \sigma^ {2} (T - t) ^ {2}.} \end{array}
$$

Therefore, the forward rate is: 

$$
f (t, T) = R (t) + \int_ {t} ^ {T} \alpha (u) d u - \frac {1}{2} \sigma^ {2} (T - t) ^ {2}.\tag{1.3.12}
$$

(Forward rate dynamics) We compute the diferential $d f ( t , T )$ using (1.3.12) and Itô’s lemma / Leibniz rule: 

$$
\begin{array}{l} d f (t, T) = d R (t) + d \left(\int_ {t} ^ {T} \alpha (u) d u\right) - d \left(\frac {1}{2} \sigma^ {2} (T - t) ^ {2}\right) \\ \qquad = (\alpha (t) d t + \sigma d \widetilde {W} (t)) + (- \alpha (t) d t) - (\frac {1}{2} \sigma^ {2} \cdot 2 (T - t) (- 1) d t) \\ \qquad = \alpha (t) d t + \sigma d \widetilde {W} (t) - \alpha (t) d t + \sigma^ {2} (T - t) d t = \sigma^ {2} (T - t) d t + \sigma d \widetilde {W} (t). \end{array}
$$

Note that the forward rate $f ( t , T )$ is not a traded asset price, and its drift under $\widetilde { \mathbb { P } }$ is not $R ( t ) f ( t , T )$ , nor is it zero in general. Thus, $f ( t , T )$ is not a martingale under $\widetilde { \mathbb { P } } .$ (The T-forward measure) We can define a change of measure from $\widetilde { \mathbb { P } }$ to the T-forward measure $\mathbb { P } ^ { T }$ such that $f ( t , T )$ becomes a martingale. Rearranging the dynamics: 

$$
d f (t, T) = \sigma (\sigma (T - t) d t + d \widetilde {W} (t)).
$$

Define a new process $W ^ { T } ( t )$ such that $d W ^ { T } ( t ) = \sigma ( T - t ) d t + d \widetilde { W } ( t )$ . By Girsanov’s theorem, $W ^ { T } ( t )$ is a Brownian motion under the measure $\mathbb { P } ^ { T }$ defined by the Radon-Nikodym derivative process $\begin{array} { r } { Z ( t ) = \frac { d \mathbb { P } ^ { T } } { d \mathbb { P } } | _ { \mathcal { F } _ { t } } } \end{array}$ This process is given by the stochastic exponential: 

$$
Z (t) = \mathcal {E} \left(\int_ {0} ^ {t} - \sigma (T - u) d \widetilde {W} (u)\right) = \exp \left(- \sigma \int_ {0} ^ {t} (T - u) d \widetilde {W} (u) - \frac {1}{2} \sigma^ {2} \int_ {0} ^ {t} (T - u) ^ {2} d u\right).
$$

Comparing this with the expression for the discounted bond price (1.3.11), we see a fundamental relationship: 

$$
Z (t) = \frac {D (t) B (t , T)}{B (0 , T)}.\tag{1.3.13}
$$

This identity holds generally for arbitrage-free short-rate models: the Radon-Nikodym process relating the risk-neutral measure $\widetilde { \mathbb { P } }$ to the $T -$ -forward measure $\mathbb { P } ^ { T }$ is the discounted bond price $D ( t ) B ( t , T )$ , normalized by its initial value $B ( 0 , T )$ 

Under the T-forward measure $\mathbb { P } ^ { T }$ , the forward rate dynamics become: 

$$
d f (t, T) = \sigma d W ^ {T} (t).\tag{1.3.14}
$$

This confirms that $f ( t , T )$ is a martingale under its corresponding forward measure $\mathbb { P } ^ { T }$ 

End of the first half of Lecture 7 

We present another interest rate model as an exercise. 

Exercise 1.3.2 (The Cox-Ingersoll-Ross (CIR) model). We consider the Cox-Ingersoll-Ross $( C I R )$ model for the short-term interest rate $R ( u )$ . Assume that $R ( u ) \geq 0$ for all $u \geq 0$ . The dynamics are specified under a risk-neutral measure $\tilde { P } _ { \ l }$ 

1. (Analysis of the CIR model SDE) The CIR process $R ( u )$ is defined by the following stochastic diferential equation (SDE) under the risk-neutral measure ${ \tilde { P } } \colon$ 

$$
d R (u) = k (\theta - R (u)) \mathrm{d} u + \sigma \sqrt {R (u)} \mathrm{d} \tilde {W} (u), \quad u \geq 0\tag{1.3.15}
$$

where $k , \theta , \sigma$ are positive constants, $R ( 0 )$ is the initial rate, and $\tilde { W } ( u )$ is a standard Brownian motion under $\tilde { P }$ The condition $2 k \theta \ge \sigma ^ { 2 }$ is typically required to ensure $R ( u ) > 0$ for $u > 0$ if $R ( 0 ) > 0$ We investigate the process $Y ( u ) = e ^ { k u } R ( u )$ . Applying Itô’s lemma to $f ( u , R ) = e ^ { k u } R$ , we have $\begin{array} { r } { \frac { \partial f } { \partial u } = } \end{array}$ $\begin{array} { r } { k e ^ { k u } R , \frac { \partial f } { \partial R } = e ^ { k u } } \end{array}$ , and $\begin{array} { r } { \frac { \partial ^ { 2 } f } { \partial R ^ { 2 } } = 0 } \end{array}$ . Therefore, 

$$
\begin{array}{l} d (e ^ {k u} R (u)) = \left(\frac {\partial f}{\partial u} + \frac {\partial f}{\partial R} k (\theta - R (u)) + \frac {1}{2} \frac {\partial^ {2} f}{\partial R ^ {2}} (\sigma \sqrt {R (u)}) ^ {2}\right) \mathrm{d} u + \frac {\partial f}{\partial R} \sigma \sqrt {R (u)} \mathrm{d} \tilde {W} (u) \\ = \left(k e ^ {k u} R (u) + e ^ {k u} k (\theta - R (u)) + \frac {1}{2} (0) \sigma^ {2} R (u)\right) \mathrm{d} u + e ^ {k u} \sigma \sqrt {R (u)} \mathrm{d} \tilde {W} (u) \\ = \left(k e ^ {k u} R (u) + k \theta e ^ {k u} - k e ^ {k u} R (u)\right) \mathrm{d} u + \sigma e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u) \\ = k \theta e ^ {k u} \mathrm{d} u + \sigma e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u). \end{array}
$$

Alternatively, as noted, using the informal product rule notation (justified by the Itô calculation above): 

$$
\begin{array}{r l} & {d (e ^ {k u} R (u)) = e ^ {k u} d R (u) + R (u) d (e ^ {k u})} \\ & {\qquad = e ^ {k u} (k (\theta - R (u)) \mathrm{d} u + \sigma \sqrt {R (u)} \mathrm{d} \tilde {W} (u)) + R (u) (k e ^ {k u} \mathrm{d} u)} \\ & {\qquad = (k \theta e ^ {k u} - k R (u) e ^ {k u} + k R (u) e ^ {k u}) \mathrm{d} u + \sigma e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u)} \\ & {\qquad = k \theta e ^ {k u} \mathrm{d} u + \sigma e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u).} \end{array}
$$

Integrating both sides from 0 to t: 

$$
\begin{array}{c} e ^ {k t} R (t) - e ^ {k \cdot 0} R (0) = \int_ {0} ^ {t} k \theta e ^ {k u} \mathrm{d} u + \int_ {0} ^ {t} \sigma e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u) \\ e ^ {k t} R (t) = R (0) + k \theta \left[ \frac {e ^ {k u}}{k} \right] _ {0} ^ {t} + \sigma \int_ {0} ^ {t} e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u) \\ = R (0) + \theta (e ^ {k t} - 1) + \sigma \int_ {0} ^ {t} e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u). \end{array}
$$

This gives an expression for $R ( t )$ : 

$$
R (t) = e ^ {- k t} R (0) + \theta (1 - e ^ {- k t}) + \sigma e ^ {- k t} \int_ {0} ^ {t} e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u).\tag{1.3.16}
$$

We cannot obtain a simple closed-form solution for $R ( t )$ itself because the Itô integral term depends on $R ( u )$ . However, we can compute the expected value under ${ \tilde { P } } .$ Since $\begin{array} { r } { \int _ { 0 } ^ { t } e ^ { k u } \sqrt { R ( u ) } \mathrm { d } \tilde { W } ( u ) } \end{array}$ is an Itô integral (assuming the integrand satisfies the necessary conditions, which it does for CIR), its expectation is zero: 

$$
\widetilde {\mathbb {E}} \int_ {0} ^ {t} e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u) = 0.
$$

Therefore, the expected value of the short rate is: 

$$
\widetilde {\mathbb {E}} R (t) = e ^ {- k t} R (0) + \theta (1 - e ^ {- k t}), \quad t \geq 0.\tag{1.3.17}
$$

Note that the long-term mean of the expected rate is: 

$$
\lim _ {t \to \infty} \widetilde {\mathbb {E}} R (t) = \lim _ {t \to \infty} (e ^ {- k t} R (0) + \theta (1 - e ^ {- k t})) = \theta .
$$

The Itô integral term $\begin{array} { r } { I ( t ) = \int _ { 0 } ^ { t } \sigma e ^ { k u } \sqrt { R ( u ) } \mathrm { d } \tilde { W } ( u ) } \end{array}$ determines the stochastic nature of $R ( t )$ around its mean. This integral has expected value $\widetilde { \mathbb { E } } I ( t ) = 0$ . Its variance is given by the Itô isometry: 

$$
\begin{array}{l} V a r (I (t)) = \widetilde {\mathbb {E}} I (t) ^ {2} - (\widetilde {\mathbb {E}} I (t)) ^ {2} \\ \qquad = \widetilde {\mathbb {E}} \bigg (\sigma \int_ {0} ^ {t} e ^ {k u} \sqrt {R (u)} \mathrm{d} \tilde {W} (u) \bigg) ^ {2} \\ \qquad = \sigma^ {2} \widetilde {\mathbb {E}} \int_ {0} ^ {t} \left(e ^ {k u} \sqrt {R (u)}\right) ^ {2} \mathrm{d} u \\ \qquad = \sigma^ {2} \int_ {0} ^ {t} e ^ {2 k u} \widetilde {\mathbb {E}} R (u) \mathrm{d} u. \end{array}
$$

The random variable $I ( t )$ is generally not normally distributed. This is because the integrand $H ( u ) =$ $\sigma e ^ { k u } \sqrt { R ( u ) }$ is itself stochastic and depends on the path of $\tilde { W } ( u )$ through $R ( u )$ . An Itô integral $\begin{array} { r } { \int _ { 0 } ^ { t } H ( u ) \mathrm { d } \tilde { W } ( u ) } \end{array}$ is normally distributed if and only if the integrand $H ( u )$ is deterministic. The fact that $\check { R } ( u ) \geq 0$ also implies the distribution of $R ( t )$ is skewed (specifically, related to a non-central chi-squared distribution). 

2. (Bond pricing under the CIR model) The CIR model (1.3.15) describes a Markov process for the short rate $R ( t )$ . We want to find the price at time t of a zero-coupon bond maturing at time $T > t$ . Let $\mathcal { F } _ { t }$ be the filtration generated by the Brownian motion $\tilde { W } ( u )$ up to time t. The price of the bond under the risk-neutral measure $\tilde { P }$ is given by the conditional expectation of the discounted payof: 

$$
B (t, T) = \tilde {\mathbb {E}} \left[ e ^ {- \int_ {t} ^ {T} R (u) \mathrm{d} u} \mid \mathcal {F} _ {t} \right].\tag{1.3.18}
$$

Since $R ( t )$ is Markov, the bond price depends only on the current time t and the current state $R ( t )$ $T h u s ,$ there exists a deterministic function $g ( t , r )$ such that $B ( t , T ) = g ( t , R ( t ) )$ 

Define the discount process $D ( t ) = e ^ { - \int _ { 0 } ^ { t } R ( u ) \mathrm { d } u }$ . The fundamental theorem of asset pricing states that the discounted price process of any traded asset is a martingale under the risk-neutral measure. For the bond, this means the process $D ( t ) B ( t , T )$ is a P<sup>˜</sup>-martingale for $0 \leq t \leq T$ . We can verify this using the tower property of conditional expectation: 

$$
\begin{array}{r l} & {\tilde {\mathbb {E}} \left[ D (T) B (T, T) \mid \mathcal {F} _ {t} \right] = \tilde {\mathbb {E}} \left[ e ^ {- \int_ {0} ^ {T} R (u) \mathrm{d} u} \cdot 1 \mid \mathcal {F} _ {t} \right]} \\ & {\qquad = e ^ {- \int_ {0} ^ {t} R (u) \mathrm{d} u} \tilde {\mathbb {E}} \left[ e ^ {- \int_ {t} ^ {T} R (u) \mathrm{d} u} \mid \mathcal {F} _ {t} \right]} \\ & {\qquad = D (t) B (t, T).} \end{array}
$$

Since $D ( t ) B ( t , T )$ is a martingale, its drift must be zero. We apply $I t { \hat { o } } ^ { \prime } s$ lemma to find the dynamics of $D ( t ) B ( t , T ) = D ( t ) g ( t , R ( t ) )$ ). First, $d D ( t ) = - R ( t ) D ( t ) \mathrm { d } t$ . Next, apply Itô’s lemma to $g ( t , R ( t ) )$ ). Let $r = R ( t )$ 

$$
\begin{array}{r l} & {d g (t, R (t)) = \frac {\partial g}{\partial t} \mathrm{d} t + \frac {\partial g}{\partial r} d R (t) + \frac {1}{2} \frac {\partial^ {2} g}{\partial r ^ {2}} d \langle R \rangle_ {t}} \\ & {\qquad d \langle R \rangle_ {t} = (\sigma \sqrt {R (t)}) ^ {2} \mathrm{d} t = \sigma^ {2} R (t) \mathrm{d} t = \sigma^ {2} r \mathrm{d} t.} \\ & {\qquad d g (t, r) = \frac {\partial g}{\partial t} \mathrm{d} t + \frac {\partial g}{\partial r} (k (\theta - r) \mathrm{d} t + \sigma \sqrt {r} \mathrm{d} \tilde {W} (t)) + \frac {1}{2} \frac {\partial^ {2} g}{\partial r ^ {2}} \sigma^ {2} r \mathrm{d} t} \\ & {\qquad = \left(\frac {\partial g}{\partial t} + k (\theta - r) \frac {\partial g}{\partial r} + \frac {1}{2} \sigma^ {2} r \frac {\partial^ {2} g}{\partial r ^ {2}}\right) \mathrm{d} t + \sigma \sqrt {r} \frac {\partial g}{\partial r} \mathrm{d} \tilde {W} (t).} \end{array}
$$

Now apply Itô’s product rule to $d ( D ( t ) g ( t , R ( t ) ) )$ ): 

$$
\begin{array}{l} d (D g) = g d D + D d g + d \langle D, g \rangle_ {t} \\ \qquad = g (- r D \mathrm{d} t) + D \left[ \left(\frac {\partial g}{\partial t} + k (\theta - r) \frac {\partial g}{\partial r} + \frac {1}{2} \sigma^ {2} r \frac {\partial^ {2} g}{\partial r ^ {2}}\right) \mathrm{d} t + \sigma \sqrt {r} \frac {\partial g}{\partial r} \mathrm{d} \tilde {W} (t) \right] + 0. \end{array}
$$

The quadratic covariation term $d \langle D , g \rangle _ { t } = 0$ because $D ( t )$ has no dW<sup>˜</sup> component. Collecting terms: 

$$
d (D g) = D \left[ - r g + \frac {\partial g}{\partial t} + k (\theta - r) \frac {\partial g}{\partial r} + \frac {1}{2} \sigma^ {2} r \frac {\partial^ {2} g}{\partial r ^ {2}} \right] \mathrm{d} t + D \sigma \sqrt {r} \frac {\partial g}{\partial r} \mathrm{d} \tilde {W} (t).
$$

For $D ( t ) g ( t , R ( t ) )$ to be a martingale, the drift term (the coeficient of dt) must be zero. This yields the following partial diferential equation (PDE) for $g ( t , r )$ 

$$
\frac {\partial g}{\partial t} + k (\theta - r) \frac {\partial g}{\partial r} + \frac {1}{2} \sigma^ {2} r \frac {\partial^ {2} g}{\partial r ^ {2}} - r g = 0,\tag{1.3.19}
$$

for $r > 0$ and $0 \leq t \leq T$ . The terminal condition for a zero-coupon bond is that its price at maturity equals its face value (assumed to be 1): 

$$
g (T, r) = 1 \quad f o r a l l r \geq 0.\tag{1.3.20}
$$

An educated guess is that the solution to this PDE with the given terminal condition has an afine form: 

$$
g (t, r) = \exp \{- C (t, T) r - A (t, T) \},
$$

where $A ( t , T )$ and $C ( t , T )$ are deterministic functions of t and T. We need to find these functions. Let’s denote $A ( t , T )$ by A and $C ( t , T )$ by C for brevity, and $\begin{array} { r } { \boldsymbol { A _ { t } } = \frac { \partial \boldsymbol { A } } { \partial t } , \boldsymbol { C _ { t } } = \frac { \partial \boldsymbol { C } } { \partial t } } \end{array}$ . The partial derivatives of g are: 

$$
\frac {\partial g}{\partial t} = - g (C _ {t} r + A _ {t}), \quad \frac {\partial g}{\partial r} = - C g, \quad \frac {\partial^ {2} g}{\partial r ^ {2}} = C ^ {2} g.
$$

Substitute these into the PDE (1.3.19): 

$$
- g (C _ {t} r + A _ {t}) + k (\theta - r) (- C g) + \frac {1}{2} \sigma^ {2} r (C ^ {2} g) - r g = 0.
$$

Assuming $g \neq 0$ , we can divide by $g \colon$ 

$$
- (C _ {t} r + A _ {t}) - k C (\theta - r) + \frac {1}{2} \sigma^ {2} r C ^ {2} - r = 0.
$$

Rearrange and collect terms multiplying r and constant terms: 

$$
r \left(- C _ {t} + k C + \frac {1}{2} \sigma^ {2} C ^ {2} - 1\right) + (- A _ {t} - k \theta C) = 0.
$$

This equation must hold for all $r \geq 0$ . Therefore, the coeficients of r and the constant term must both be zero: 

$$
- C _ {t} + k C + \frac {1}{2} \sigma^ {2} C ^ {2} - 1 = 0\tag{1.3.21}
$$

$$
- A _ {t} - k \theta C = 0\tag{1.3.22}
$$

These are ordinary diferential equations (ODEs) for C(t, T) and $A ( t , T )$ with respect to t. Equation (1.3.21) is a Riccati equation for C. Equation (1.3.22) is a linear equation for A, once $C$ is known. Now we apply the terminal condition $g ( T , r ) = 1$ . From the ansatz: 

$$
g (T, r) = \exp \{- C (T, T) r - A (T, T) \} = 1 \quad f o r a l l r \geq 0.
$$

This implies that the exponent must be zero for all $r \geq 0 .$ 

$$
- C (T, T) r - A (T, T) = 0.
$$

For this linear function of r to be identically zero, both coeficients must be zero. This gives the terminal conditions for the ODEs: 

$$
C (T, T) = A (T, T) = 0
$$

The ODEs (1.3.21) and (1.3.22) can be solved backwards from time $T$ using these terminal conditions to find the functions $C ( t , T )$ and $A ( t , T )$ ), thus fully specifying the bond price $B ( t , T ) = g ( t , R ( t ) )$ . 

End of Recitation $\it 4$ 

We now present an example of pricing interest rate caplets. 

Example 1.3.3 (Midterm of 2022, Problem 3). Consider a caplet that pays $( R ( T ) - K ) ^ { + }$ at time $T ,$ where K is the strike rate. Its price at time $t = 0$ is given by the risk-neutral expectation: 

$$
\text { Caplet   Price } = \widetilde {\mathbb {E}} \left[ D (T) (R (T) - K) ^ {+} \right].
$$

Using the change of measure to the T-forward measure $\mathbb { P } ^ { T }$ : 

$$
P r i c e = \widetilde {\mathbb {E}} \left[ \frac {D (T) B (T , T)}{B (0 , T)} \frac {B (0 , T)}{B (T , T)} (R (T) - K) ^ {+} \right].
$$

Since $B ( T , T ) = 1$ , this becomes: 

$$
P r i c e = \widetilde {\mathbb {E}} \left[ Z (T) B (0, T) (R (T) - K) ^ {+} \right] = B (0, T) \mathbb {E} ^ {T} \left[ (R (T) - K) ^ {+} \right],
$$

where $\mathbb { E } ^ { T }$ denotes expectation under $\mathbb { P } ^ { T }$ . To evaluate this, we need the distribution of $R ( T )$ under $\mathbb { P } ^ { T }$ Integrating $d R ( t ) = \alpha ( t ) d t + \sigma d \widetilde { W } ( t )$ 

$$
R (T) = R (0) + \int_ {0} ^ {T} \alpha (u) d u + \sigma \widetilde {W} (T).
$$

Substitute $\begin{array} { r } { \widetilde { W } ( T ) = W ^ { T } ( T ) - \int _ { 0 } ^ { T } \sigma ( T - u ) d u : } \end{array}$ 

$$
\begin{array}{l} R (T) = R (0) + \int_ {0} ^ {T} \alpha (u) d u + \sigma \left(W ^ {T} (T) - \sigma \int_ {0} ^ {T} (T - u) d u\right) \\ \qquad = \left(R (0) + \int_ {0} ^ {T} \alpha (u) d u - \sigma^ {2} \left[ T u - \frac {u ^ {2}}{2} \right] _ {0} ^ {T}\right) + \sigma W ^ {T} (T) \\ \qquad = \underbrace {\left(R (0) + \int_ {0} ^ {T} \alpha (u) d u - \frac {1}{2} \sigma^ {2} T ^ {2}\right)} _ {\text {Mean under \mathbb {P} ^{T}}} + \sigma W ^ {T} (T). \end{array}
$$

Under $\mathbb { P } ^ { T } , W ^ { T } ( T )$ is normally distributed with mean 0 and variance T. Therefore, $R ( T )$ is normally distributed under $\mathbb { P } ^ { T }$ . The expectation $\mathbb { E } ^ { T } [ ( R ( T ) - K ) ^ { + } ]$ is the price of a European call option on a normally distributed variable, which can be calculated using a formula analogous to the Black-Scholes formula for call options on log-normal variables. 

## 1.3.3 Heath-Jarrow-Morton (HJM) framework

Reference: [Shr, §1.4]. 

Short-rate models, such as the Vasicek or Ho-Lee models, postulate dynamics for the instantaneous short rate $R ( t )$ . While tractable, they often face practical challenges during calibration to market data. Consider the Ho-Lee model under the risk-neutral measure ${ \widetilde { \mathbb { P } } } ,$ where $d R ( t ) = \alpha ( t ) d t + \sigma d \widetilde { W } ( t )$ . The time-t price of a zero-coupon bond maturing at time $T , \ B ( t , T )$ , is given by $\begin{array} { r } { \mathbb { E } ^ {  { \widetilde { \mathbb { P } } } } [ \exp \left( - \int _ { t } ^ { T } R ( u ) d u \right) | \mathcal { F } _ { t } ] } \end{array}$ . For the Ho-Lee model, this leads to an explicit formula for the bond price at time $t = 0 \colon$ 

$$
B (0, T) = \exp \left[ - R (0) T - \int_ {0} ^ {T} \alpha (u) (T - u) d u + \frac {1}{6} \sigma^ {2} T ^ {3} \right].
$$

Market quotes are typically given in terms of yields, $Y ( 0 , T )$ , where $B ( 0 , T ) = \exp ( - T Y ( 0 , T ) )$ . Calibration involves choosing the model parameters, primarily the function $\alpha ( t )$ and the constant $\sigma ,$ such that the model-implied yields $Y ^ { \mathrm { M o d e l } } ( 0 , T )$ match the observed market yields $\overrightharpoon { Y } ^ { \mathrm { M a r k e t } } ( 0 , T )$ for various maturities $T ,$ Equating the exponents gives: 

$$
T Y ^ {\mathrm{Market}} (0, T) = R (0) T + \int_ {0} ^ {T} \alpha (u) (T - u) d u - \frac {1}{6} \sigma^ {2} T ^ {3}.
$$

To extract the function $\alpha ( T )$ , one typically diferentiates this expression with respect to the maturity T. A first derivative yields: 

$$
\frac {d}{d T} (T Y ^ {\mathrm{Market}} (0, T)) = R (0) + \int_ {0} ^ {T} \alpha (u) d u - \frac {1}{2} \sigma^ {2} T ^ {2}.
$$

A second derivative with respect to $T$ isolates $\alpha ( T )$ 

$$
\frac {d ^ {2}}{d T ^ {2}} (T Y ^ {\mathrm{Market}} (0, T)) = \alpha (T) - \sigma^ {2} T.
$$

Assuming $\sigma$ is estimated $( \mathrm { e . g . }$ , from historical data or option prices), this equation allows determining $\alpha ( T )$ . However, market yield data is typically available only for a discrete set of maturities $T _ { 1 } , T _ { 2 } , \dots , T _ { n }$ Estimating the second derivative of the yield curve from such sparse and potentially noisy data is numerically unstable and highly sensitive to the interpolation method used. This practical dificulty motivates alternative approaches to interest rate modeling 

The Heath-Jarrow-Morton (HJM) framework provides such an alternative by directly modeling the dynamics of the entire instantaneous forward rate curve $f ( t , T )$ , where $f ( t , T )$ is the forward interest rate at time t for an instantaneous borrowing or lending period at time $T \geq t .$ . The framework specifies the dynamics under the physical measure P. Let $W ( t )$ be a standard Brownian motion under P. The general HJM model assumes that for each fixed maturity $T _ { \mathrm { : } }$ the forward rate $f ( t , T )$ follows an Itô process for $t \in [ 0 , T ]$ 

$$
d f (t, T) = \alpha (t, T) d t + \sigma (t, T) d W (t), \quad 0 \leq t \leq T.\tag{1.3.23}
$$

Here, the drift process $\alpha ( t , T )$ and the volatility process $\sigma ( t , T )$ are adapted to the filtration $\mathcal { F } _ { t }$ generated by $W ( t )$ , and may depend on the current state of the entire forward curve or other factors. A key advantage is the calibration procedure. The initial state of the model, the forward curve $f ( 0 , T )$ for all $T \geq 0$ , is taken directly from the currently observed market term structure of interest rates. Recall that the forward rate is related to market bond prices or yields by 

$$
f (0, T) = - \frac {\partial}{\partial T} \log B (0, T) = \frac {\partial}{\partial T} (T Y (0, T)).
$$

While this still requires computing one derivative from market data, it avoids the problematic second derivative required in the Ho-Lee calibration example. The HJM framework thus ensures by construction that the model perfectly fits the initial yield curve. 

The primary assets in this framework are the zero-coupon bonds $B ( t , T )$ , whose prices are determined by the forward rates: 

$$
B (t, T) = \exp \left(- \int_ {t} ^ {T} f (t, u) d u\right).
$$

For pricing interest rate derivatives, we need to work under a risk-neutral measure $\widetilde { \mathbb { P } } .$ According to the fundamental theorems of asset pricing, under $\widetilde { \mathbb { P } } ,$ the price process of any traded asset, discounted by the money market account 

$$
M (t) = \exp \left(\int_ {0} ^ {t} R (s) d s\right)
$$

where $R ( t ) = f ( t , t )$ is the short rate, must be a martingale. Equivalently, the instantaneous expected return on any bond $B ( t , T )$ under $\widetilde { \mathbb { P } }$ must equal the risk-free rate $R ( t )$ . This means the dynamics of the bond price must take the form: 

$$
d B (t, T) = R (t) B (t, T) d t + (\text { volatility   terms }) d \widetilde {W} (t),
$$

where $\widetilde { W } ( t )$ is a Brownian motion under $\widetilde { \mathbb { P } } .$ By Girsanov’s theorem, the change of measure from $\mathbb { P }$ to $\widetilde { \mathbb { P } }$ is associated with a market price of risk process $\Theta ( t )$ , such that $d \widetilde { W } ( t ) = d W ( t ) + \Theta ( t ) d t$ . The dynamics of the bond price under P would then be: 

$$
d B (t, T) = (R (t) + (\text { volatility   terms }) \Theta (t)) B (t, T) d t + (\text { volatility   terms }) d W (t).
$$

A significant challenge arises because we have a continuum of assets (bonds $B ( t , T )$ for all $T > t )$ but only a single source of randomness $W ( t )$ in this specification. For the market to be arbitrage-free and for a unique risk-neutral measure $\widetilde { \mathbb { P } }$ to exist (associated with the numeraire $M ( t ) )$ , the market price of risk $\Theta ( t )$ derived from the dynamics of any bond $B ( t , T )$ must be the same, independent of the maturity T. This requirement imposes a strong consistency condition, known as the HJM drift condition, relating the drift $\alpha ( t , T )$ and volatility $\sigma ( t , T )$ of the forward rates under P. 

To derive this condition, we first need to compute the dynamics of the bond price $B ( t , T )$ under P. By Itô’s lemma, $d B ( t , T )$ depends on the dynamics of the exponent $\begin{array} { r } { X ( t , T ) = \int _ { t } ^ { T } f ( t , u ) d u } \end{array}$ . Let’s find $d X ( t , T )$ . We start by expressing $f ( t , u )$ using its definition (1.3.23): 

$$
f (t, u) = f (0, u) + \int_ {0} ^ {t} \alpha (s, u) d s + \int_ {0} ^ {t} \sigma (s, u) d W (s).
$$

Substituting this into the definition of $X ( t , T )$ : 

$$
X (t, T) = \int_ {t} ^ {T} \left(f (0, u) + \int_ {0} ^ {t} \alpha (s, u) d s + \int_ {0} ^ {t} \sigma (s, u) d W (s)\right) d u.
$$

Assuming suficient regularity of the coeficients α and σ to apply Fubini’s theorem and its stochastic counterpart (as rigorously justified in the original HJM papers), we can swap the order of integration: 

$$
X (t, T) = \int_ {t} ^ {T} f (0, u) d u + \int_ {0} ^ {t} \left(\int_ {t} ^ {T} \alpha (s, u) d u\right) d s + \int_ {0} ^ {t} \left(\int_ {t} ^ {T} \sigma (s, u) d u\right) d W (s).
$$

Let us define the integrated drift and volatility coeficients: 

$$
\alpha^ {*} (t, T) := \int_ {t} ^ {T} \alpha (t, u) d u \quad \sigma^ {*} (t, T) := \int_ {t} ^ {T} \sigma (t, u) d u.\tag{1.3.24}
$$

The diferential $d X ( t , T )$ can be found using Leibniz integral rule and properties of Itô integrals. A detailed derivation shows that (noting that $f ( t , t ) = R ( t )$ , the instantaneous short rate) 

$$
\begin{array}{r l} d \left(\int_ {t} ^ {T} f (t, u) d u\right) & = \ldots \text {see [Shr, p. 6]...} \\ & = [ - f (t, t) + \alpha^ {*} (t, T) ]   d t + \sigma^ {*} (t, T) d W (t) \\ & = [ - R (t) + \alpha^ {*} (t, T) ]   d t + \sigma^ {*} (t, T) d W (t). \end{array}
$$

This expression for the dynamics of the exponent is the crucial intermediate step. Applying Itô’s lemma to $B ( t , T ) = \exp ( - X ( t , T ) )$ using this result will yield the dynamics $d B ( t , T )$ under P, allowing us to identify the market price of risk $\Theta ( t )$ and derive the HJM no-arbitrage condition. 

End of the second half of Lecture 7 

We can now apply Itô’s lemma to the function $g ( x ) = e ^ { - x }$ with $x = X ( t , T )$ to find the dynamics of the bond price $B ( t , T ) = g ( X ( t , T ) )$ . Since $g ^ { \prime } ( x ) = - e ^ { - x }$ and $g ^ { \prime \prime } ( x ) = e ^ { - x }$ , we have (see $\left[ \mathrm { S h r } , \mathrm { p } , \mathrm { ~ } 7 \right]$ for a detailed calculation) 

$$
\begin{array}{l} d B (t, T) = g ^ {\prime} (X (t, T)) d X (t, T) + \frac {1}{2} g ^ {\prime \prime} (X (t, T)) (d X (t, T)) ^ {2} \\ \qquad = B (t, T) \left[ \bigg (R (t) - \alpha^ {*} (t, T) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2} \bigg) d t - \sigma^ {*} (t, T) d W (t) \right]. \end{array}\tag{1.3.25}
$$

This equation describes the bond price dynamics under the physical measure P. 

We summarize the above discussion with a theorem. 

Theorem 1.3.4. Every arbitrage-free term structure model driven by a single Brownian motion has the following form. For $0 \leq t \leq T$ 2 

$$
d f (t, T) = \sigma (t, T) \sigma^ {*} (t, T) d t + \sigma (t, T) d \widetilde {W} (t),\tag{1.3.26}
$$

$$
d B (t, T) = R (t) B (t, T) d t - \sigma^ {*} (t, T) B (t, T) d \widetilde {W} (t),\tag{1.3.27}
$$

$$
d (D (t) B (t, T)) = - \sigma^ {*} (t, T) D (t) B (t, T) d \widetilde {W} (t),\tag{1.3.28}
$$

$$
D (t) B (t, T) = B (0, T) \exp \left[ - \int_ {0} ^ {t} \sigma^ {*} (u, T) d \widetilde {W} (u) - \frac {1}{2} \int_ {0} ^ {t} (\sigma^ {*} (u, T)) ^ {2} d u \right]\tag{1.3.29}
$$

From Equation (1.3.2), we have 

$$
f (t, T) = - \frac {\partial}{\partial T} B (t, T), \quad B (t, T) = \exp \left[ - \int_ {t} ^ {T} f (t, u) d u \right]
$$

and $\sigma ^ { * } ( t , T )$ is given by (1.3.24): 

$$
\sigma^ {*} (t, T) = \int_ {t} ^ {T} \sigma (t, u) d u
$$

In these formulas, $\widetilde { W }$ is a Brownian motion under a risk-neutral measure $\widetilde { \mathbb { P } } .$ 

## HJM no-arbitrage condition

For the market to be free of arbitrage, there must exist an equivalent risk-neutral measure $\widetilde { \mathbb { P } }$ under which the discounted price of any traded asset is a martingale. Specifically, the instantaneous expected return of any bond under $\widetilde { \mathbb { P } }$ must equal the risk-free rate $R ( t )$ . This implies the bond price dynamics under $\widetilde { \mathbb { P } }$ must be of the form: 

$$
d B (t, T) = R (t) B (t, T) d t + (\text { volatility   terms }) d \widetilde {W} (t),
$$

where $\widetilde { W } ( t )$ is a Brownian motion under $\widetilde { \mathbb { P } } .$ . The transition between the measures is achieved via Girsanov’s theorem, which relates the Brownian motions through a market price of risk process $\Theta ( t )$ , independent of the specific asset: $d \widetilde { W } ( t ) = d W ( t ) + \Theta ( t ) d t$ . Comparing the drift term in (1.3.25) with the required risk-neutral drift $R ( t ) B ( t , T ) d t$ , we can identify the risk premium associated with the bond $B ( t , T )$ : 

$$
\text { Risk   Premium } = \left(- \alpha^ {*} (t, T) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2}\right) B (t, T) d t.
$$

The risk premium must equal the product of the volatility coeficient and the market price of risk increment: 

$$
\text { Risk   Premium } = (- \sigma^ {*} (t, T) B (t, T)) \Theta (t) d t.
$$

Equating these two expressions for the risk premium yields: 

$$
\left(- \alpha^ {*} (t, T) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2}\right) B (t, T) d t = - \sigma^ {*} (t, T) B (t, T) \Theta (t) d t.
$$

Solving for $\Theta ( t )$ , we find: 

$$
\Theta (t) = \frac {\alpha^ {*} (t , T) - \frac {1}{2} (\sigma^ {*} (t , T)) ^ {2}}{\sigma^ {*} (t , T)} = \frac {\alpha^ {*} (t , T)}{\sigma^ {*} (t , T)} - \frac {\sigma^ {*} (t , T)}{2}.
$$

A crucial requirement for the absence of arbitrage in the HJM framework is that the market price of risk $\Theta ( t )$ must be independent of the bond maturity T. If $\Theta ( t )$ depended on $T _ { \mathrm { : } }$ , we would need a diferent change of measure for each bond, contradicting the existence of a single consistent risk-neutral measure $\widetilde { \mathbb { P } }$ under which all discounted bond prices are martingales simultaneously. Therefore, the HJM no-arbitrage condition (or drift condition) states that the quantity 

$$
\frac {\alpha^ {*} (t , T)}{\sigma^ {*} (t , T)} - \frac {\sigma^ {*} (t , T)}{2} \quad \text { must   be   independent   of } T.\tag{1.3.30}
$$

Assuming this condition holds, we denote the resulting market price of risk process by $\Theta ( t )$ 

It is often more convenient to express this condition in terms of the original forward rate drift and volatility coeficients, $\alpha ( t , T )$ and $\sigma ( t , T )$ . Starting from $\begin{array} { r } { \Theta ( t ) = \frac { \alpha ^ { * } ( t , T ) } { \sigma ^ { * } ( t , T ) } - \frac { \sigma ^ { * } ( t , T ) } { 2 } } \end{array}$ , we multiply by $\sigma ^ { * } ( t , T )$ 

$$
\sigma^ {*} (t, T) \Theta (t) = \alpha^ {*} (t, T) - \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2}.
$$

Diferentiating both sides with respect to the maturity $T ,$ and recalling that $\begin{array} { r } { \frac { \partial } { \partial T } \sigma ^ { * } ( t , T ) = \sigma ( t , T ) } \end{array}$ and $\begin{array} { r } { \frac { \partial } { \partial T } \alpha ^ { * } ( t , T ) = \alpha ( t , T ) } \end{array}$ : 

$$
\sigma (t, T) \Theta (t) = \alpha (t, T) - \frac {1}{2} \cdot 2 \sigma^ {*} (t, T) \cdot \sigma (t, T) = \alpha (t, T) - \sigma^ {*} (t, T) \sigma (t, T).
$$

Rearranging gives the HJM drift condition in its standard form: 

$$
\alpha (t, T) = \sigma (t, T) (\Theta (t) + \sigma^ {*} (t, T)).\tag{1.3.31}
$$

This condition imposes a strict relationship between the drift and volatility structures of the forward rates under the physical measure P to ensure consistency with no arbitrage. In practice, modelers typically specify the volatility structure $\sigma ( t , T )$ (often based on market data like cap/swaption volatilities) and the market price of risk $\Theta ( t )$ (which might be set to zero for simplicity or calibrated to market prices reflecting risk aversion). The drift $\alpha ( t , T )$ under $\mathbb { P }$ is then uniquely determined by the no-arbitrage condition (1.3.31). 

## Forward rate dynamics under diferent measures

Having established the no-arbitrage condition and the market price of risk $\Theta ( t )$ , we can now express the dynamics of the forward rate $f ( t , T )$ and related quantities under the risk-neutral measure $\widetilde { \mathbb { P } }$ and the $T -$ forward measure $\mathbb { P } ^ { T }$ 

First, let’s verify the bond price dynamics under Pe. Substitute $\widetilde { \mathbb { P } } .$ $d W ( t ) = d \widetilde { W } ( t ) - \Theta ( t ) d t$ into (1.3.25): 

$$
\begin{array}{r} d B (t, T) = B (t, T) \left[ \left(R (t) - \alpha^ {*} (t, T) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2}\right) d t - \sigma^ {*} (t, T) (d \widetilde {W} (t) - \Theta (t) d t) \right] \\ = B (t, T) \left[ \left(R (t) - \alpha^ {*} (t, T) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2} + \sigma^ {*} (t, T) \Theta (t)\right) d t - \sigma^ {*} (t, T) d \widetilde {W} (t) \right]. \end{array}
$$

Using the relationship 

$$
\alpha^ {*} (t, T) = \sigma^ {*} (t, T) \Theta (t) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2}
$$

derived from the no-arbitrage condition (1.3.30), the drift term simplifies: 

$$
R (t) - \left(\sigma^ {*} (t, T) \Theta (t) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2}\right) + \frac {1}{2} (\sigma^ {*} (t, T)) ^ {2} + \sigma^ {*} (t, T) \Theta (t) = R (t).
$$

Thus, the bond price dynamics under $\widetilde { \mathbb { P } }$ are: 

$$
d B (t, T) = B (t, T) \left[ R (t) d t - \sigma^ {*} (t, T) d \widetilde {W} (t) \right].\tag{1.3.32}
$$

Now consider the discounted bond price $D ( t ) B ( t , T )$ , where $\begin{array} { r } { D ( t ) = \exp \left( - \int _ { 0 } ^ { t } R ( s ) d s \right) } \end{array}$ is the discount factor with $d D ( t ) = - R ( t ) D ( t ) d t$ . Using the product rule for Itô processes: 

$$
d (D (t) B (t, T)) = D (t) d B (t, T) + B (t, T) d D (t) + d D (t) d B (t, T)\tag{1.3.33}
$$

$$
= D (t) \left(B (t, T) [ R (t) d t - \sigma^ {*} (t, T) d \widetilde {W} (t) ]\right) + B (t, T) (- R (t) D (t) d t) + 0\tag{1.3.34}
$$

$$
= D (t) B (t, T) R (t) d t - D (t) B (t, T) \sigma^ {*} (t, T) d \widetilde {W} (t) - D (t) B (t, T) R (t) d t\tag{1.3.35}
$$

$$
= - D (t) B (t, T) \sigma^ {*} (t, T) d \widetilde {W} (t).\tag{1.3.36}
$$

Since the drift term is zero, this confirms that the discounted bond price $D ( t ) B ( t , T )$ is a martingale under the risk-neutral measure ${ \widetilde { \mathbb { P } } } ,$ as required by the no-arbitrage principle. 

The process $D ( t ) B ( t , T )$ plays a crucial role in defining the change of measure from the risk-neutral measure $\widetilde { \mathbb { P } }$ to the T-forward measure $\mathbb { P } ^ { T }$ . The T-forward measure uses the bond $B ( t , T )$ as the numeraire. The Radon-Nikodym derivative process for this change of measure on $\mathcal { F } _ { t }$ is given by: 

$$
Z _ {T} (t) := \left. \frac {d \mathbb {P} ^ {T}}{d \widetilde {\mathbb {P}}} \right| _ {\mathcal {F} _ {t}} = \frac {D (t) B (t , T)}{D (0) B (0 , T)} = \frac {D (t) B (t , T)}{B (0 , T)}.
$$

From (1.3.36), the dynamics of the Radon-Nikodym process are 

$$
d Z _ {T} (t) = - \frac {1}{B (0 , T)} D (t) B (t, T) \sigma^ {*} (t, T) d \widetilde {W} (t) = - Z _ {T} (t) \sigma^ {*} (t, T) d \widetilde {W} (t)
$$

By Girsanov’s theorem (using the convention $d W ^ { T } = d \widetilde { W } - \langle d \log Z _ { T } , d \widetilde { W } \rangle _ { t } )$ , the process $W ^ { T } ( t )$ defined by 

$$
d W ^ {T} (t) = d \widetilde {W} (t) + \sigma^ {*} (t, T) d t\tag{1.3.37}
$$

is a standard Brownian motion under the T-forward measure $\mathbb { P } ^ { T }$ 

Finally, we can summarize the dynamics of the forward rate $f ( t , T )$ under the three diferent measures: 

1. Under the physical measure P: Substitute the no-arbitrage condition (1.3.31) into the original definition (1.3.23): 

$$
d f (t, T) = [ \sigma (t, T) \Theta (t) + \sigma^ {*} (t, T) \sigma (t, T) ] d t + \sigma (t, T) d W (t).
$$

2. Under the risk-neutral measure $\widetilde { \mathbb { P } } \colon$ Substitute $d W ( t ) = d \widetilde { W } ( t ) - \Theta ( t ) d t$ into the P-dynamics: 

$$
\begin{array}{r l} & {d f (t, T) = [ \sigma (t, T) \Theta (t) + \sigma^ {*} (t, T) \sigma (t, T) ] d t + \sigma (t, T) (d \widetilde {W} (t) - \Theta (t) d t)} \\ & {\qquad = \sigma^ {*} (t, T) \sigma (t, T) d t + \sigma (t, T) d \widetilde {W} (t).} \end{array}
$$

Note that $f ( t , T )$ is generally not a martingale under $\widetilde { \mathbb { P } } .$ 

3. Under the T-forward measure $\mathbb { P } ^ { T }$ : Substitute $d \widetilde { W } ( t ) = d W ^ { T } ( t ) - \sigma ^ { * } ( t , T ) d t$ into the $\widetilde { \mathbb { P } } \mathrm { - d y n a m i c s : }$ 

$$
\begin{array}{r l} d f (t, T) & = \sigma^ {*} (t, T) \sigma (t, T) d t + \sigma (t, T) (d W ^ {T} (t) - \sigma^ {*} (t, T) d t) \\ & = \sigma^ {*} (t, T) \sigma (t, T) d t + \sigma (t, T) d W ^ {T} (t) - \sigma (t, T) \sigma^ {*} (t, T) d t \\ & = \sigma (t, T) d W ^ {T} (t). \end{array}
$$

The remarkable result is that under the T-forward measure $\mathbb { P } ^ { T }$ , the instantaneous forward rate $f ( t , T )$ for that specific maturity T follows a martingale process. This property is extremely useful for pricing derivatives whose payof depends on the forward rate at maturity, such as caplets and floorlets, as it simplifies expectation calculations, often leading to Black-Scholes-like formulas $( \mathrm { e . g . }$ , Black’s formula). 

## 1.3.4 Forward contracts

Reference: [Shr, §2.1, 2.2]. Most of the materials in this section are direct excerpts from [Shr, §2.1, 2.2]. 

Forward contracts and futures contracts allow agents to lock in prices before actual asset transactions, but through diferent mechanisms. 

A forward contract is an agreement where at time t, party A commits to pay $\mathrm { F o r } ( t , T )$ to party B at future time T in exchange for an asset S whose price $S ( T )$ will be unknown until time T. The price $\mathrm { F o r } ( t , T )$ is set so the contract has zero value at inception. After time t, the contract’s value fluctuates: if the asset price rises faster than expected, party A benefits; if it falls, party B benefits. 

Unlike options, forward contracts require both parties to complete the exchange. When one party gains value, the other faces a liability, creating counterparty default risk. This risk explains why forwards typically trade over-the-counter rather than on exchanges. Counterparties often establish collateral agreements or trade through clearing houses to mitigate this risk. 

## Definition of the forward price

Consider an asset with price $S ( t )$ at time t. Assume that this asset does not pay dividends and there is no cost associated with holding the asset. Owning some assets, gold for example, requires the payment of a storage cost. This is called a cost of carry. Financial assets, such as stocks and bonds, do not have a cost of carry. 

According to the definition of risk-neutral measure, the discounted price of assets that do not pay dividends and have no cost of carry are martingales under risk-neutral measures. Therefore, we assume there is a probability measure $\widetilde { \mathbb { P } }$ under which $D ( t ) S ( t )$ is a martingale. As usual, $D ( t )$ is the discount process 

$$
D (t) = \exp \left(- \int_ {0} ^ {t} R (u) d u\right)
$$

and $R ( t )$ is the spot interest rate. Now consider a forward contract, entered at time t, under which the agent in the long position agrees to pay cash K at a later time T in exchange for one unit of S at time $T .$ , valued at S(T). According to the risk-neutral pricing formula, the price of this contract at time t is 

$$
\frac {1}{D (t)} \widetilde {\mathbb {E}} [ D (T) (S (T) - K) \mid \mathcal {F} (t) ] = \frac {1}{D (t)} \widetilde {\mathbb {E}} [ D (T) S (T) \mid \mathcal {F} (t) ] - \frac {K}{D (t)} \widetilde {\mathbb {E}} [ D (T) \mid \mathcal {F} (t) ] = S (t) - K B (t, T).
$$

The price of this contract at time t is zero if and only if $K = S ( t ) / B ( t , T )$ . Therefore,<sup>3</sup> 

Definition 1.3.5 (forward price). Assume that S is an asset that does not pay a dividend and has zero cost of carry. For $0 \leq t \leq T$ , the forward price at time t for delivery of one unit of S at time T is 

$$
\operatorname{For} (t, T) = \frac {S (t)}{B (t , T)}\tag{1.3.38}
$$

## Price of a forward contract

The forward price is not the price/value of a forward contract. The forward price is instead the price one agrees to pay at a future date in order to receive an asset at that future date. 

Therefore, there is no reason that discounted forward prices should be martingales under the risk-neutral measure. We will however see that undiscounted forward prices are martingales under a diferent measure, called a forward measure. 

Let us consider a forward contract that is entered at time t for delivery of one unit of an asset valued at $S ( T )$ at time T. We continue to assume that S does not pay a dividend and has zero cost of carry. The forward price at time t is given by (1.3.38). The forward contract will have value 

$$
S (T) - \mathrm{For} (t, T) = S (T) - \frac {S (t)}{B (t , T)}
$$

at time T. At times u between t and T, the price of the forward contract, given by the risk-neutral pricing formula can be computed using the martingale property for $D ( t ) S ( t )$ and the fact that $S ( t ) / B ( t , T )$ is $\mathcal { F } ( u )$ -measurable to be 

$$
\begin{array}{l} P (u; t, T) = \frac {1}{D (u)} \widetilde {\mathbb {E}} \left[ D (T) \left(S (T) - \frac {S (t)}{B (t , T)}\right) \Bigg |   \mathcal {F} (u) \right] \\ = \frac {1}{D (u)} \widetilde {\mathbb {E}} [ D (T) S (T) \mid \mathcal {F} (u) ] - \frac {S (t)}{B (t , T)} \cdot \frac {1}{D (u)} \widetilde {\mathbb {E}} [ D (T) \mid \mathcal {F} (t) ] \\ = S (u) - \frac {S (t) B (u , T)}{B (t , T)} = B (u, T) \left(\frac {S (u)}{B (u , T)} - \frac {S (t)}{B (t , T)}\right), \quad t \leq u \leq T \end{array}
$$

Observations of the price (value) $P ( u ; t , T )$ at time u of the forward contract entered at time t for delivery at time $T \colon$ 

1. At the time the forward contract is entered, its price is zero: 

$$
P (t; t, T) = 0
$$

No money changes hands at time t. 

2. At the time the forward contract expires, $B ( T , T ) = 1$ and the price of the forward contract is 

$$
P (T; t, T) = S (T) - \frac {S (t)}{B (t , T)} = S (T) - \operatorname{For} (t, T)
$$

This is because the forward contract delivers one unit of S in exchange for $\mathrm { F o r } ( t , T )$ in cash. 

3. For times u between t and T, the price of the forward contract is positive if 

$$
\frac {S (u)}{B (u , T)} > \frac {S (t)}{B (t , T))}
$$

If the ratio of the asset price to the bond price has grown between times t and $u ,$ i.e., if the asset price has grown at a faster rate than the bond price, then the forward contract takes on positive value. If the asset price has grown more slowly than the bond price, then the forward contract takes on negative value. Since the asset price generally does not grow exactly at the rate of the bond price, the price of the forward contract is generally not zero after time t. 

4. Forward contracts are doubly indexed, i.e., $P ( u ; t , T )$ depends on the time t the contract is entered and the time of delivery T. Because of this, there cannot be deep markets in forward contracts. This is another reason futures contracts, which are indexed only by the time of delivery, are more common. 

## Forward measure

Undiscounted forward prices are a martingales under a diferent measure, called the forward measure. This fact plays an important role in pricing fixed income derivatives because it leads to Black’s formula. 

We begin with a Brownian motion $\widetilde { W }$ under a risk-neutral measure $\widetilde { \mathbb { P } }$ and use Girsanov’s Theorem to change to a diferent measure and a diferent Brownian motion. 

Definition 1.3.6. Let $T \in [ 0 , \bar { T } ]$ be given and consider the default-free zero-coupon bond price $B ( t , T ) , 0 \leq$ $t \leq T$ . According to Theorem $1 . 3 . 4 ,$ Equation (1.3.29), 

$$
\frac {D (t) B (t , T)}{B (0 , T)} = \exp \left[ - \int_ {0} ^ {t} \sigma^ {*} (u, T) d \widetilde {W} (u) - \frac {1}{2} \int_ {0} ^ {t} \left(\sigma^ {*} (u, T)\right) ^ {2} d u \right], \quad 0 \leq t \leq T
$$

$W e$ use this process as the Radon-Nikodym derivative to change to a new measure called the T-forward measure and denoted $\mathbb { P } ^ { T }$ . Under this measure, the process 

$$
W ^ {T} (t) = \widetilde {W} (t) + \int_ {0} ^ {t} \sigma^ {*} (u, T) d u, \quad 0 \leq t \leq T\tag{1.3.39}
$$

is a Brownian motion called the T-forward Brownian motion. 

By Girsanov’s theorem, we have 

$$
\mathbb {E} ^ {T} [ Y ] = \widetilde {\mathbb {E}} \left[ \frac {D (T) B (T , T)}{B (0 , T)} Y \right] = \frac {1}{B (0 , T)} \widetilde {\mathbb {E}} [ D (T) Y ]
$$

for $\mathcal { F } ( T )$ -measurable random variables Y. If Y is $\mathcal { F } ( t )$ -measurable for some $t \in [ 0 , T ]$ , this formula is still correct, but also 

$$
\mathbb {E} ^ {T} [ Y ] = \widetilde {\mathbb {E}} \left[ \frac {D (t) B (t , T)}{B (0 , T)} Y \right] = \frac {1}{B (0 , T)} \widetilde {\mathbb {E}} [ D (t) B (t, T) Y ]
$$

If Y is $\mathcal { F } ( t )$ -measurable for $t \in [ 0 , T ]$ and $0 \leq s \leq t .$ , then we have Bayes’ rule 

$$
\mathbb {E} ^ {T} [ Y \mid \mathcal {F} (s) ] = \frac {B (0 , T)}{D (s) B (s , T)} \widetilde {\mathbb {E}} \left[ \left. \frac {D (t) B (t , T)}{B (0 , T)} Y \right| \mathcal {F} (s) \right] = \frac {1}{D (s) B (s , T)} \widetilde {\mathbb {E}} [ D (t) B (t, T) Y \mid \mathcal {F} (s) ]\tag{1.3.40}
$$

We are now ready to state and prove the main result. 

Theorem 1.3.7. Assume that S is an asset that does not pay a dividend and has zero cost of carry. Let $T \in [ 0 , \bar { T } ]$ be given. The forward price of S for delivery at time T (1.3.38) is a martingale under the T-forward measure $\mathbb { P } ^ { T }$ 

Proof. We let $0 \leq u \leq t \leq T$ be given. We must show that 

$$
\mathbb {E} ^ {T} [ \mathrm{For} (t, T) \mid \mathcal {F} (u) ] = \mathrm{For} (u, T)
$$

Because For $( t , T )$ is $\mathcal { F } ( t )$ -measurable, we can use Bayes’ rule (1.3.40), the definition (1.3.38) of forward price, and the fact that discounted S is a Pe-martingale to compute 

$$
\begin{array}{r l} & {\mathbb {E} ^ {T} [ \mathrm{For} (t, T) \mid \mathcal {F} (u) ] = \frac {1}{D (u) B (u , T)} \widetilde {\mathbb {E}} \left[ D (t) B (t, T) \frac {S (t)}{B (t , T)} \bigg | \mathcal {F} (u) \right]} \\ & {\qquad = \frac {1}{D (u) B (u , T)} \widetilde {\mathbb {E}} [ D (t) S (t) \mid \mathcal {F} (u) ] = \frac {1}{D (\widehat {u}) B (u , T)} D (\widehat {u}) S (u) = \mathrm{For} (u, T)} \end{array}
$$

## Forward interest rate

Consider a model with a spot interest rate $R ( t )$ . According to the risk-neutral pricing formula, the price at time t of a default-free zero-coupon bond paying 1 at maturity $T$ is 

$$
B (t, T) = \widetilde {\mathbb {E}} \left[ e ^ {- \int_ {t} ^ {T} R (u) d u} \mid \mathcal {F} (t) \right]
$$

Therefore, 

$$
- \frac {\partial}{\partial T} B (t, T) = - \widetilde {\mathbb {E}} \left[ \left. \frac {\partial}{\partial T} e ^ {- \int_ {t} ^ {T} R (u) d u} \right| \mathcal {F} (t) \right] = \widetilde {\mathbb {E}} \left[ R (T) e ^ {- \int_ {t} ^ {T} R (u) d u} \mid \mathcal {F} (t) \right] = \frac {1}{D (t)} \widetilde {\mathbb {E}} [ D (T) R (T) \mid \mathcal {F} (t) ]
$$

According to the risk-neutral pricing formula, this is the price at time t of an asset that pays $R ( T )$ at time T. We call this price 

$$
S (t) := - \frac {\partial}{\partial T} B (t, T)
$$

The asset that pays $R ( T )$ at time T does not pay a dividend and has zero cost of carry, so its forward price is 

$$
\frac {S (t)}{B (t , T)} = - \frac {\frac {\partial}{\partial T} B (t , T)}{B (t , T)} = - \frac {\partial}{\partial T} \log B (t, T)
$$

This is the forward interest rate (1.3.1) of Definition 1.3.1. We thus have a second interpretation of the forward rate. In that part (§1.3.1) we saw the $f ( t , T )$ is the instantaneous rate that can be locked in a time t for borrowing or investing at time $T ;$ this is how we understood (1.3.1). Here we see that $f ( t , T )$ is the forward price at time t for a contract that delivers $R ( T )$ at time $T ,$ 

Example 1.3.8 (Forward rates in the Ho-Lee model). Recall the Ho-Lee model whose diferential is 

$$
d f (t, T) = \sigma^ {2} (T - t) d t + \sigma d \widetilde {W} (t) = \sigma (d \widetilde {W} (t) + \sigma (T - t) d t), \quad 0 \leq t \leq T\tag{1.3.41}
$$

We have just seen that this is the forward price of a contract that pays $R ( T )$ at time $T .$ . Therefore, Theorem 1.3.7 implies that $f ( t , T )$ is a martingale under the T-forward measure. We verify this. 

In the Ho-Lee model, $\sigma ^ { * } ( t , T ) = ( T - t ) \sigma$ . Therefore, the forward Brownian motion (1.3.39) is 

$$
W ^ {T} (t) = \widetilde {W} (t) + \sigma \int_ {0} ^ {t} (T - u) d u\tag{1.3.42}
$$

which implies that 

$$
d W ^ {T} (t) = d \widetilde {W} (t) + \sigma (T - t) d t\tag{1.3.43}
$$

Equation (1.3.41) can be rewritten as 

$$
d f (t, T) = \sigma d W ^ {T} (t), \quad 0 \leq t \leq T
$$

Because $W ^ { T }$ is a Brownian motion under $\mathbb { P } ^ { T } , f ( t , T )$ is a $\mathbb { P } ^ { T }$ -martingale. In addition, we see from Definition $\it 2 . 4$ and $\left( 1 . 5 3 \right)$ that in the Ho-Lee model the Radon-Nikodym derivative ${ \widetilde { \mathbb { P } } } .$ -martingale for the change ofmeasure from $\widetilde { \mathbb { P } } _ { t o } \mathbb { P } ^ { T }$ is 

$$
\frac {D (t) B (t , T)}{B (0 , T)} = \exp \left[ - \sigma \int_ {0} ^ {t} (T - u) d \widetilde {W} (u) - \frac {1}{2} \sigma^ {2} \int_ {0} ^ {t} (T - u) ^ {2} d u \right]
$$

## 1.3.5 Black’s formula

Reference: [Shr, §2.3]. Most of the materials in this section are direct excerpts from [Shr, §2.3]. 

The Black-Scholes formula, published in 1974, revolutionized finance by enabling the pricing and trading of derivative securities for both hedging and speculation. This work by Black, Scholes, and Merton established volatility as the standard quoting method for equity options. 

European call prices depend on five factors: interest rate, time to expiration, underlying asset price, asset volatility, and strike price. With constant interest rates typical for short-lived equity options, prices efectively depend on just three variables: expiration time, asset price, and volatility. 

Since expiration time and asset price constantly change, quoting option prices directly is impractical. Instead, specifying the volatility for the Black-Scholes formula provides a more stable quoting method. This approach eliminates the need to update quotes when time passes or asset prices fluctuate. 

Fischer Black later joined Goldman Sachs’ fixed income division, where he adapted his work for fixed income derivatives. Unlike equity options, these long-term instruments operate in changing interest rate environments. Black developed a formula using forward prices and forward measures to maintain volatility as an efective quoting convention for these derivatives. 

## Derivation of Black’s formula

Consider a model in which the spot interest rate $R ( t )$ is not necessarily constant. In this model, suppose S is an asset that does not pay a dividend and has zero cost of carry. Assume further that $S ( t ) > 0$ for $0 \leq t \leq T$ almost surely. According to the risk-neutral pricing formula, a European call on $S$ expiring at time $T$ with strike price K has time-zero price 

$$
C (0) = \widetilde {\mathbb {E}} \left[ D (T) (S (T) - K) ^ {+} \right]\tag{1.3.44}
$$

In models of fixed-income markets, the asset S is not a stock. It might be a bond. More frequently, it is a contract that makes a payment at a future date based on interest rates over a period of time just prior to that date. The computation of the right-hand side of (1.3.44) is dificult because of the correlation between $D ( T )$ and $( S ( T ) - K ) ^ { + }$ 

Suppose that $D ( T )$ and $( S ( T ) - K ) ^ { + }$ are uncorrelated under $\widetilde { \mathbb { P } } .$ In this case, we can write 

$$
C (0) = \widetilde {\mathbb {E}} [ D (T) ] \widetilde {\mathbb {E}} \left[ (S (T) - K) ^ {+} \right] = B (0, T) \widetilde {\mathbb {E}} \left[ (S (T) - K) ^ {+} \right]\tag{1.3.45}
$$

However, in fixed income applications, the second equality in (1.3.45) is always incorrect. We resolve this issue by recalling the T-forward measure $\mathbb { P } ^ { T }$ of Definition 1.3.6. We use up the troubling term $D ( T )$ in (1.3.45) by changing to expectation $\mathbb { E } ^ { T }$ under $\mathbb { P } ^ { T }$ . Thus, in place of (1.3.45), we write 

$$
C (0) = B (0, T) \widetilde {\mathbb {E}} \left[ \frac {D (T) B (T , T)}{B (0 , T)} (S (T) - K) ^ {+} \right] = B (0, T) \mathbb {E} ^ {T} \left[ (S (T) - K) ^ {+} \right],\tag{1.3.46}
$$

where noting that $B ( T , T ) \equiv 1$ and that $B ( 0 , T )$ is not random. We obtain a formula much like (1.3.45), but now $D ( T )$ and $( S ( T ) - K ) ^ { + }$ are allowed to be correlated and the expectation in the final result is computed under $\mathbb { P } ^ { T }$ . Of course, to compute this expectation, we need to know the distribution of $S ( T )$ under $\mathbb { P } ^ { \bar { T } }$ 

Recall that the forward price at time t for delivery of one unit of $S$ at time $T$ is 

$$
\operatorname{For} (t, T) = \frac {S (t)}{B (t , T)}, \quad 0 \leq t \leq T
$$

According to Theorem 1.3.7, $\mathrm { F o r } ( t , T )$ is a martingale under $\mathbb { P } ^ { T }$ . But we have assumed that $S ( t )$ is strictly positive for all $t \in [ 0 , T ]$ , so $\mathrm { F o r } ( t , T )$ is strictly positive for all $t \in [ 0 , T ]$ . A strictly positive martingale is a generalized geometric Brownian motion. In other words, there is an adapted process $\sigma ( t ) , 0 \leq t \leq T$ , such that for $0 \leq t \leq T$ ， 

$$
d \mathrm{For} (t, T) = \sigma (t) \mathrm{For} (t, T) d W ^ {T} (t)\tag{2.18}
$$

$$
\mathrm{For} (t, T) = \mathrm{For} (0, T) \exp \left[ \int_ {0} ^ {t} \sigma (u) d W ^ {T} (u) - \frac {1}{2} \int_ {0} ^ {t} \sigma^ {2} (u) d u \right].\tag{2.19}
$$

But $S ( T ) = \mathrm { F o r } ( T , T )$ , and therefore 

$$
S (T) = \operatorname{For} (T, T) = \operatorname{For} (0, T) \exp \left[ \int_ {0} ^ {T} \sigma (u) d W ^ {T} (u) - \frac {1}{2} \int_ {0} ^ {T} \sigma^ {2} (u) d u \right]\tag{1.3.47}
$$

We now consider special cases. 

The first case is when the volatility is either a positive or negative constant $\pm \sigma ^ { 4 }$ and thus $\mathrm { F o r } ( t , T )$ is a geometric Brownian motion under $\dot { \mathbb { P } } ^ { T }$ . In particular, (1.3.47) reduces to 

$$
S (T) = \mathrm{For} (0, T) \exp \left[ \pm \sigma W ^ {T} (T) - \frac {1}{2} \sigma^ {2} T \right]\tag{1.3.48}
$$

and $\mathbb { E } ^ { T } \left[ ( S ( T ) - K ) ^ { + } \right]$ is given by the Black-Scholes formula. 

Theorem 1.3.9 (Black’s formula with constant volatility). Let S be an asset that does not pay a dividend and has zero cost of carry. Let $C ( 0 )$ be the price at time zero of a European call option on $S$ with strike price K expiring at time T. Let σ be a positive constant, and assume that the forward price For(t, T) of S for delivery at time T has volatility σ $o r - \sigma$ . Then 

$$
C (0) = B (0, T) \left(\mathrm{For} (0, T) N \left(d _ {+}\right) - K N \left(d _ {-}\right)\right) = S (0) N \left(d _ {+}\right) - K B (0, T) N \left(d _ {-}\right),\tag{1.3.49}
$$

where 

$$
d _ {\pm} = \frac {1}{\sigma \sqrt {T}} \left[ \log \frac {\mathrm{For} (0 , T)}{K} \pm \frac {1}{2} \sigma^ {2} T \right].\tag{1.3.50}
$$

Proof. If the forward price volatility is $\sigma ,$ then the first equation in (1.3.49) together with (1.3.50) follow from the Black-Scholes formula applied to compute $\mathbb { E } ^ { T } [ ( S ( T ) - K ) ^ { + } ]$ using formula (1.3.48) for $S ( T )$ and then using formula (1.3.46) for $C ( 0 )$ 

If the forward price volatility is $- \sigma .$ , we observe that $- \sigma W ^ { T } ( T )$ and σ $W ^ { T } ( T )$ are both normal with expected value zero and variance $\sigma ^ { 2 } \dot { T }$ under $\mathbb { P } ^ { T }$ . Therefore, 

$$
S (T) = \mathrm{For} (0, T) \exp \left[ - \sigma W ^ {T} (T) - \frac {1}{2} \sigma^ {2} T \right]
$$

and 

$$
\widehat {S} (T) = \mathrm{For} (0, T) \exp \left[ \sigma W ^ {T} (T) - \frac {1}{2} \sigma^ {2} T \right]
$$

have the same distribution. It follows that 

$$
\widetilde {\mathbb {E}} \left[ (S (T) - K) ^ {+} \right] = \widetilde {\mathbb {E}} \left[ (\widehat {S} (T) - K) ^ {+} \right]
$$

and the computation of this last quantity proceeds by the standard Black-Scholes argument. In particular, we obtain formula (1.3.50) for $d _ { \pm }$ with leading term $1 / \sigma \sqrt { T }$ , not $- 1 / \sigma \sqrt { T }$ 

Regardless of whether the volatility of the forward price is $\sigma \mathrm { o r } - \sigma$ , the second formula in (1.3.49) follows from the first and the fact that $\mathrm { F o r } ( 0 , T ) = S ( 0 ) / B ( 0 , T )$ □ 

Remark. In the special case that the interest rate is a constant r and the volatility σ is positive, we have 

$$
B (0, T) = e ^ {- r T} \mathrm{and} \operatorname{For} (0, T) = e ^ {r T} S (0)
$$

In this case (1.3.49) reduces to the usual Black-Scholes formula 

$$
C (0) = S (0) N \left(d _ {+}\right) - e ^ {- r T} K N \left(d _ {-}\right)
$$

where 

$$
d _ {\pm} = \frac {1}{\sigma \sqrt {T}} \left[ \log \frac {e ^ {r T} S (0))}{K} \pm \frac {1}{2} \sigma^ {2} T \right] = \frac {1}{\sigma \sqrt {T}} \left[ \log \frac {S (0)}{K} + \left(r \pm \frac {1}{2} \sigma^ {2}\right) T \right]
$$

The beauty of Black’s formula, however, is that no assumption is made on the interest rate. The only assumption is that the forward price of the underlying asset rather than the asset price itself has constant volatility. 

Remark. Using the independence lemma, one can derive the following dynamic version of Black’s formula. Under the assumptions of Theorem 1.3.9, the call price at time $t ,$ denoted by 

$$
C (t) = \frac {1}{D (t)} \widetilde {\mathbb {E}} \left[ D (T) (S (T) - K) ^ {+} \mid \mathcal {F} (t) \right], \quad 0 \leq t \leq T
$$

is given by 

$$
C (t) = S (t) N \left(d _ {+} (t, \mathrm{For} (t, T))\right) - K B (t, T) N \left(d _ {-} (t, \mathrm{For} (t, T))\right), \quad 0 \leq t <   T,\tag{1.3.51}
$$

where 

$$
d _ {\pm} (t, x) = \frac {1}{\sigma \sqrt {T - t}} \left[ \log \frac {x}{K} \pm \frac {1}{2} \sigma^ {2} (T - t) \right].
$$

End of the first half of Lecture 8 

We next consider the case that $\sigma ( u )$ is a nonrandom function of time. First note that one term on the right-hand side of (1.3.47) follows 

$$
\int_ {0} ^ {T} \sigma (u) d W ^ {T} (u) \sim \mathcal {N} ^ {\mathbb {P} ^ {T}} (0, V (T)), \quad V (T) := \int_ {0} ^ {T} \sigma^ {2} (u) d u.
$$

We define<sup>5</sup> 

$$
\bar {\sigma} := \sqrt {\frac {V (T)}{T}} = \sqrt {\frac {1}{T} \int_ {0} ^ {T} \sigma^ {2} (u) d u}\tag{1.3.52}
$$

Then 

$$
S (T) = \operatorname{For} (0, T) \exp \left[ \int_ {0} ^ {T} \sigma (u) d W ^ {T} (u) - \frac {1}{2} \int_ {0} ^ {T} \sigma^ {2} (u) d u \right]
$$

has the same distribution as (noting that $W ^ { T } ( T ) \sim { \mathcal { N } } ( 0 , T ) )$ 

$$
\widetilde {S} (T) = \mathrm{For} (0, T) \exp \left[ \bar {\sigma} W ^ {T} (T) - \frac {1}{2} \bar {\sigma} ^ {2} T \right],
$$

which is the solution to the SDE $d \widetilde { S } ( t ) = \bar { \sigma } \widetilde { S } ( t ) d W ^ { T } ( t ) , \widetilde { S } ( 0 ) = \mathrm { F o r } ( 0 , T )$ . This implies that 

$$
\mathbb {E} ^ {T} \left[ (S (T) - K) ^ {+} \right] = \mathbb {E} ^ {T} \left[ (\widetilde {S} (T) - K) ^ {+} \right]
$$

This last quantity lends itself to a standard Black-Scholes calculation. This permits us to extend Black’s formula to the case of nonrandom, time-dependent volatility: 

Theorem 1.3.10 (Black’s formula with nonrandom, time-dependent volatility). Let S be an asset that does not pay a dividend and has zero cost of carry. Let $C ( 0 )$ be the price at time zero of a European call on S with strike price K expiring at time T. Assume that the forward price For(t, T) of S for delivery at time T has nonrandom, time-dependent volatility<sup>6</sup> $\sigma ( u ) , 0 \leq u \leq T$ . Then 

$$
C (0) = B (0, T) (\text { For } (0, T) N (d _ {+}) - K N (d _ {-})) = S (0) N (d _ {+}) - K B (0, T) N (d _ {-})\tag{1.3.53}
$$

where 

$$
d _ {\pm} = \frac {1}{\bar {\sigma} \sqrt {T}} \left[ \log \frac {\mathrm{For} (0 , T)}{K} \pm \frac {1}{2} \bar {\sigma} ^ {2} T \right]
$$

Remark. Again, one can use independence lemma to show that under the assumptions of Theorem 1.3.10, the call price at time t is given by (1.3.51), where now 

$$
d _ {\pm} (t, x) = \frac {1}{\bar {\sigma} (t) \sqrt {T - t}} \left[ \log \frac {x}{K} \pm \frac {1}{2} \bar {\sigma} ^ {2} (t) (T - t) \right], \quad \bar {\sigma} (t) := \sqrt {\frac {1}{T - t} \int_ {t} ^ {T} \sigma^ {2} (u) d u}.
$$

End of Recitation 5 

Example 1.3.11 (Bond option in the Ho-Lee model). Recall that in the Ho-Lee model, the spot interest rate has diferential 

$$
d R (u) = \alpha (u) d u + \sigma d \widetilde {W} (u), \quad 0 \leq u \leq \bar {T}\tag{1.3.54}
$$

and bond price are given by 

$$
B (t, T) = \exp \left[ - (T - t) R (t) - \int_ {t} ^ {T} \alpha (u) (T - u) d u + \frac {1}{6} \sigma^ {2} (T - t) ^ {3} \right]\tag{1.3.55}
$$

Let $0 < T _ { 1 } < T _ { 2 } \leq \bar { T }$ be given. For $0 \leq t \leq T _ { 1 }$ , the forward price at time t for delivery at time $T _ { 1 }$ of the $T _ { 2 }$ -maturity bond is<sup>7</sup> 

$$
\operatorname{For} _ {B} (t, T _ {1}) = \frac {B (t , T _ {2})}{B (t , T _ {1})} = \dots (\text {see Equation 1.3.56}) \dots = e ^ {Y (t)}
$$

where 

$$
\begin{array}{l} Y (t) := - \left(T _ {2} - T _ {1}\right) R (t) - \left(T _ {2} - T _ {1}\right) \int_ {t} ^ {T _ {1}} \alpha (u) d u - \int_ {T _ {1}} ^ {T _ {2}} \alpha (u) \left(T _ {2} - u\right) d u \\ \qquad + \frac {1}{6} \sigma^ {2} \left(T _ {2} - T _ {1}\right) ^ {3} + \frac {1}{2} \sigma^ {2} \left(T _ {2} - T _ {1}\right) ^ {2} \left(T _ {1} - t\right) + \frac {1}{2} \sigma^ {2} \left(T _ {2} - T _ {1}\right) \left(T _ {1} - t\right) ^ {2} \end{array}
$$

with diferential 

$$
d Y (t) = \ldots (\text {see Equation 1.3.57}) \ldots = - (T _ {2} - T _ {1}) \sigma d \widetilde {W} (t) - \frac {1}{2} \sigma^ {2} (T _ {2} - T _ {1}) ^ {2} d t - \sigma^ {2} (T _ {2} - T _ {1}) (T _ {1} - t) d t,
$$

so that 

$$
d Y (t) d Y (t) = \left(T _ {2} - T _ {1}\right) ^ {2} \sigma^ {2} d t.
$$

Because For $_ B \left( t , T _ { 1 } \right) = f ( Y ( t ) )$ where $f ^ { \prime } ( y ) = f ^ { \prime \prime } ( y ) = f ( y ) = e ^ { y }$ , we have 

$$
d \text { For } _ {B} (t, T _ {1}) = \dots (\text { see   Equation   1.3.58 }) \dots = - (T _ {2} - T _ {1}) \sigma \text { For } _ {B} (t, T _ {1}) d W ^ {T _ {1}} (t)
$$

where 

$$
W ^ {T _ {1}} (t) := \widetilde {W} (t) + \sigma \int_ {0} ^ {t} \left(T _ {1} - u\right) d u, \quad 0 \leq t \leq T _ {1}\tag{1.3.59}
$$

is the $T _ { 1 }$ -forward Brownian motion given by (1.3.42) with diferential given by (1.3.43) when $T$ in those equations is replaced by $T _ { 1 }$ . Under $\mathbb { P } ^ { T _ { 1 } }$ , the forward price For $_ B \left( t , T _ { 1 } \right)$ is a martingale. We have identified the volatility of the $T _ { 1 }$ -forward price of the T -maturity bond. It is the constant $- \left( T _ { 2 } - T _ { 1 } \right) \sigma$ 

According to Black’s formula with constant volatility (Theorem 1.3.9), a call on the $T _ { 2 }$ -maturity bond expiring at time $T _ { 1 }$ with strike price K has time-zero price 

$$
C (0) = B \left(0, T _ {2}\right) N \left(d _ {+}\right) - K B \left(0, T _ {1}\right) N \left(d _ {-}\right),\tag{1.3.60}
$$

where 

$$
d _ {\pm} = \frac {1}{\left(T _ {2} - T _ {1}\right) \sigma \sqrt {T _ {1}}} \left[ \log \frac {B (0 , T _ {2})}{K B (0 , T _ {1})} \pm \frac {1}{2} \left(T _ {2} - T _ {1}\right) ^ {2} \sigma^ {2} T _ {1} \right].\tag{1.3.61}
$$

## 1.3.6 Secured overnight funding rate (SOFR)

Reference: [Shr, §3.2 – 3.4]. 

Prior to 2008, the London Interbank Ofered Rate (LIBOR) was the primary benchmark for short-term unsecured borrowing costs. LIBOR was published by the British Bankers’ Association: each day the Bank of England solicited quotes from a panel of banks, discarded the highest and lowest submissions, and averaged the remainder. In the wake of the 2008 financial crisis it became clear that LIBOR was highly susceptible to manipulation; several traders were prosecuted and the benchmark was discontinued for many tenors in 2013. 

In response, market participants adopted the Secured Overnight Financing Rate (SOFR), a transaction-based overnight rate reflecting the cost of borrowing cash collateralized by U.S. Treasury securities in the tri-party repurchase agreement (repo) market. 

Denote by $R ( u )$ the overnight repo rate realized at time u. A repurchase agreement executed at the close of trading on day u involves 

$$
\begin{array}{l} \text {sell Treasury securities at time u,} \\ \text {and agree to repurchase them (slightly more) at time u+ \Delta ,} \end{array}
$$

thereby locking in a one-day interest rate. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/e65d9d41-4c7a-4366-aaab-be3784392ae9/d71e61a310185e46fbee658ce9b1766ec575504d6a5bd6f59c861fcfaa2c739b.jpg)



Figure 1.3.3: Time interval of length τ over which the SOFR average is computed.


In Figure 1.3.3, $[ T _ { j - 1 } , T _ { j } ]$ is a term interval $\left( \mathrm { e . g . } \right.$ three months, so that $\tau = 1 / 4 ~ \mathrm { y e a r } )$ . By rolling over overnight repos each day in this interval, the cumulative gross return is 

$$
\prod_ {u = T _ {j - 1}} ^ {T _ {j} - \Delta} (1 + R (u) \Delta) \approx \exp \left(\int_ {T _ {j - 1}} ^ {T _ {j}} R (u) d u\right).
$$

We define the (averaged) SOFR rate over $[ T _ { j - 1 } , T _ { j } ]$ as the unique constant $\mathrm { S O F R } _ { [ T _ { j - 1 } , T _ { j } ] }$ satisfying 

$$
\exp \left(\int_ {T _ {j - 1}} ^ {T _ {j}} R (u) d u\right) = 1 + \tau \mathrm{SOFR} _ {[ T _ {j - 1}, T _ {j} ]}.
$$

Hence 

$$
\boxed {\operatorname{SOFR} _ {[ T _ {j - 1}, T _ {j} ]} = \frac {\exp \left(\int_ {T _ {j - 1}} ^ {T _ {j}} R (u) d u\right) - 1}{\tau}} \quad (\tau = T _ {j} - T _ {j - 1}).
$$

## §1.3. Fixed income models

In the next lecture we will take 

$$
R (u), \quad u \in [ 0, T ],
$$

as a continuous-time stochastic process and study the evolution of term SOFR averages and related interestrate derivatives. 

End of the second half of Lecture 8 

(Recap) Let $0 \leq T _ { j } < T _ { j + 1 }$ be consecutive accrual dates and set $\tau : = T _ { j + 1 } - T _ { j }$ (in practice $\tau = 1 / 4 \sim 9 0$ days, $\tau = 1 / 2 \sim 1 8 0 ~ \mathrm { d a y s } )$ . Denote by $r ( t )$ the (continuously-compounded) short rate and by 

$$
D (t) = \exp \left(- \int_ {0} ^ {t} r (u) d u\right), \quad B (t, T) = \frac {\widetilde {\mathbb {E}} [ D (T) \mid \mathcal {F} _ {t} ]}{D (t)}
$$

the discount factor and the time-t price of a zero-coupon bond maturing at $T$ under the risk-neutral measure $\widetilde { \mathbb { P } } .$ 

Definition 1.3.12 (Average SOFR). The realised average SOFR for the period $[ T _ { j } , T _ { j + 1 } ]$ is 

$$
S \left(T _ {j + 1}; T _ {j}, T _ {j + 1}\right) = \frac {1}{\tau} \left(\frac {D (T _ {j})}{D (T _ {j + 1})} - 1\right) = \frac {1}{\tau} \left(\exp \left(\int_ {T _ {j}} ^ {T _ {j + 1}} r (u) d u\right) - 1\right).
$$

Thus 

$$
1 + \tau S = \exp \left(\int_ {T _ {j}} ^ {T _ {j + 1}} r (u) d u\right);
$$

this follows from rolling overnight repo loans and replacing 1 + δr by $e ^ { \delta r }$ for the daily tenor δ. 

Proposition 1.3.13 (no-arbitrage time-t price of average SOFR). For $t \leq T _ { j + 1 }$ the no-arbitrage price $S ( t ; T _ { j } , T _ { j + 1 } ) ~ o f ~ S ( T _ { j + 1 } ; T _ { j } , T _ { j + 1 } )$ is 

$$
S (t; T _ {j}, T _ {j + 1}) = \frac {1}{D (t)}   \widetilde {\mathbb {E}} \left[ D (T _ {j + 1})   S (T _ {j + 1}; T _ {j}, T _ {j + 1}) \mid \mathcal {F} _ {t} \right] = \left\{ \begin{array}{l l} \frac {B (t , T _ {j}) - B (t , T _ {j + 1})}{\tau}, & t \leq T _ {j}, \\ \frac {D (T _ {j})}{\tau D (t)} - \frac {B (t , T _ {j + 1})}{\tau}, & t \in [ T _ {j}, T _ {j + 1} ]. \end{array} \right.
$$

Proof. Insert the definition of $S ( T _ { j + 1 } ; T _ { j } , T _ { j + 1 } )$ and use $\widetilde { \mathbb { E } } [ D ( T ) \mid \mathcal { F } _ { t } ] = D ( t ) B ( t , T )$ , taking into account whether $D ( T _ { j } )$ is $\mathcal { F } _ { t } .$ -measurable $( t \geq T _ { j } )$ or not. □ 

Definition 1.3.14 (Forward SOFR). The forward SOFR rate observed at time $t \leq T _ { j + 1 }$ for the period $[ T _ { j } , T _ { j + 1 } ]$ is 

$$
\text { For } _ {S} \left(t; T _ {j}, T _ {j + 1}\right) := \frac {S (t ; T _ {j} , T _ {j + 1})}{B (t , T _ {j + 1})}.
$$

Consequently 

$$
\operatorname{For} _ {S} (t; T _ {j}, T _ {j + 1}) = \left\{ \begin{array}{l l} \frac {B (t , T _ {j})}{\tau B (t , T _ {j + 1})} - \frac {1}{\tau}, & t \leq T _ {j}, \\ \frac {D (T _ {j})}{\tau D (t) B (t , T _ {j + 1})} - \frac {1}{\tau}, & t \in [ T _ {j}, T _ {j + 1} ]. \end{array} \right.
$$

Unlike LIBOR, the realised average SOFR is fixed at the end of the accrual period, so For is the tradable rate that locks-in today the future average funding cost. 

Example 1.3.15 (Caplet on the compounded SOFR). Fix an accrual period $[ T _ { j } , T _ { j + 1 } ]$ of length $\tau = T _ { j + 1 } -$ $T _ { j }$ . The caplet pays 

$$
(S (T _ {j + 1}; T _ {j}, T _ {j + 1}) - K) ^ {+} \quad a t T _ {j + 1},
$$

where the realised average SOFR $S ( T _ { j + 1 } ; T _ { j } , T _ { j + 1 } )$ is given by $S = \tau ^ { - 1 } \left( D ( T _ { j } ) / D ( T _ { j + 1 } ) - 1 \right)$ 

Because $S ( T _ { j + 1 } ; T _ { j } , T _ { j + 1 } ) = \mathrm { F o r } _ { S } ( T _ { j + 1 } ; T _ { j } , T _ { j + 1 } )$ , the payof can be written as 

$$
(\mathrm{For} _ {S} (T _ {j + 1}; T _ {j}, T _ {j + 1}) - K) ^ {+},
$$

so the caplet is a European call on the forward SOFR. 

For any valuation time $t \leq T _ { j + 1 }$ ， 

$$
\operatorname{Caplet} (t) = \frac {1}{D (t)} \widetilde {\mathbb {E}} \left[ D (T _ {j + 1}) \left(\operatorname{For} _ {S} (T _ {j + 1}; T _ {j}, T _ {j + 1}) - K\right) ^ {+} \mid \mathcal {F} _ {t} \right].
$$

(Change to the $T _ { j + 1 }$ -forward measure) Introduce the density 

$$
Z _ {t} = \frac {D (t)   B (t , T _ {j + 1})}{B (0 , T _ {j + 1})}, \qquad \left. \frac {d \mathbb {P} ^ {T _ {j + 1}}}{d \widetilde {\mathbb {P}}} \right| _ {\mathcal {F} _ {t}} = Z _ {t}.
$$

Then $F _ { s } : = \mathrm { F o r } _ { S } ( s ; T _ { j } , T _ { j + 1 } )$ is $a \mathbb { P } ^ { T _ { j + 1 } }$ -martingale, and Caplet(t) becomes 

$$
\operatorname{Caplet} (t) = B \left(t, T _ {j + 1}\right) \mathbb {E} ^ {\mathbb {P} ^ {T _ {j + 1}}} \left[ \left(F _ {T _ {j + 1}} - K\right) ^ {+} \mid \mathcal {F} _ {t} \right].
$$

(Making the payof log-normal) The explicit form of $F _ { s }$ (Definition 1.3.14) contains a constant $s h i f t - \tau ^ { - 1 }$ Set $\widehat F _ { s } : = F _ { s } + \tau ^ { - 1 }$ . Then $\widehat { F } _ { s }$ is a quotient of discounted bond prices, hence a geometric Brownian motion under $\mathbb { P } ^ { T _ { j + 1 } }$ . The payof rewrites as 

$$
\left(\widehat {F} _ {T _ {j + 1}} - (K + \tau^ {- 1})\right) ^ {+}.
$$

Under Ho-Lee $( d r = \sigma d \widetilde { W } )$ every bond price is log-normal with volatility $\sigma _ { B } ( t , T ) = - \sigma ( T - t ) . \ F o r \ t \leq T _ { j }$ the ratio $\begin{array} { r } { \widehat { F } _ { t } = \frac { B ( t , T _ { j } ) } { \tau B ( t , T _ { j + 1 } ) } } \end{array}$ inherits the constant volatility 

$$
\sigma_ {F} = - \sigma (T _ {j + 1} - T _ {j}).
$$

For $t \in [ T _ { j } , T _ { j + 1 } ]$ one obtains the time-dependent volatility $\sigma _ { F } ( t ) = - \sigma \left( T _ { j + 1 } - t \right)$ . Hence, under $\mathbb { P } ^ { T _ { j + : } }$ 

$$
\ln \frac {\widehat {F} _ {T _ {j + 1}}}{\widehat {F} _ {t}} \sim \mathcal {N} \left(- \frac {1}{2} v (t),   v (t)\right), \qquad v (t) = \int_ {t} ^ {T _ {j + 1}} \sigma_ {F} (u) ^ {2}   d u = \sigma^ {2} \left\{ \begin{array}{l l} (T _ {j + 1} - T _ {j}) ^ {2}   (T _ {j + 1} - t), & t \leq T _ {j}, \\ \frac {(T _ {j + 1} - t) ^ {3}}{3}, & t \geq T _ {j}. \end{array} \right.
$$

Applying the Black formula with spot $F _ { t } ,$ , strike $K ,$ , and variance $v ( t )$ gives 

$$
\boxed {\operatorname{Caplet} (t) = \tau B (t, T _ {j + 1}) \left(F _ {t} N (d _ {+}) - K N (d _ {-})\right)}
$$

where 

$$
d _ {\pm} = \frac {\ln (F _ {t} / K) \pm \frac {1}{2} v (t)}{\sqrt {v (t)}}, \quad F _ {t} = \operatorname{For} _ {S} (t; T _ {j}, T _ {j + 1}).
$$

(The pre-factor τ restores the industry convention that caplet notionals are expressed in rate per annum.) 

To summarize the section, rolling overnight repos links the short rate to the realised average SOFR: 

$$
S = (\tau^ {- 1}) (D (T _ {j}) / D (T _ {j + 1}) - 1).
$$

The tradable forward SOFR 

$$
\mathrm{For} _ {S} = S / B (\cdot , T _ {j + 1})
$$

is known at the start of the interval and serves as LIBOR’s analogue. Caplets and other SOFR derivatives are valued by switching to the $T _ { j + 1 }$ -forward measure and applying the Black formula once the volatility of For<sub>S</sub> is identified (constant in Ho-Lee, piece-wise in general). 

## 1.3.7 Futures contracts

Reference: [Shr, §2.4]. Most of the materials in this section are direct excerpts from [Shr, §2.4]. 

Futures contracts also present a way of locking in a price in advance, but without the default risk inheren in forward contracts. These contracts are traded on exchanges. Suppose at time $t _ { 0 }$ an agent wishes to lock in a price for purchase of one unit of an underlying asset S at a later time $T .$ . She can do that by taking a long futures position on $S .$ This generates a cash flow depending on changes in the futures price for the asset between times $t _ { 0 }$ and $T .$ . The futures price is set by supply and demand at the exchange. An agent who buys a futures contract pays nothing for the contract but must deposit money into a margin account<sup>8</sup> held by the exchange. The next day, if the futures price has increased, the agent will receive the amount of the increase added to her margin account. If the futures prices has decreased, the amount of the decrease is deducted from her margin account. This process is called marking to market or daily resettlement. 

Suppose at time $t _ { 0 }$ an agent takes a long futures position with delivery at a later date $t _ { n } = T$ . Suppose at the end of day $t _ { j } , j = 0 , 1 , \ldots , n$ , the futures price for time- T delivery is Fut $( t _ { j } , T )$ . The futures price on the delivery date $T = t _ { n }$ is always the price of the underlying asset $S ( T )$ at that date, i.e., Fut $( t _ { n } , T ) = S ( T )$ . On each of the dates $t _ { j } , j = 1 , \ldots , n$ , the agent with the long futures position receives Fut $( t _ { j } , T ) - \mathrm { F u t } \left( t _ { j - 1 } , T \right)$ If this quantity is negative, “receives” means that money is deducted from the agent’s margin account. The total amount received by the long futures position between the time $t _ { 0 }$ when the long position is entered and the time T of delivery is 

$$
\begin{array}{l} \left(\operatorname{Fut} \left(t _ {1}, T\right) - \operatorname{Fut} \left(t _ {0}, T\right)\right) + \dots + \left(\operatorname{Fut} \left(t _ {n - 1}, T\right) - \operatorname{Fut} \left(t _ {n - 2}, T\right)\right) + \left(\operatorname{Fut} \left(t _ {n}, T\right) - \operatorname{Fut} \left(t _ {n - 1}, T\right)\right) \\ = \operatorname{Fut} \left(t _ {n}, T\right) - \operatorname{Fut} \left(t _ {0}, T\right) = S (T) - \operatorname{Fut} \left(t _ {0}, T\right) \end{array}
$$

If the agent holding the long futures position wishes to own the asset, at time $T$ she pays market price $S ( T )$ . From the cash flow associated with the long futures position, she has received $S ( T )$ , which covers this purchase, and has paid Fut $( t _ { 0 } , T )$ . Thus the futures price Fut $( t _ { 0 } , T )$ at time $t _ { 0 }$ has been locked in as the net amount the agent pays to acquire the asset S at time $T .$ 

Because the forward contract results in a single payment at time $T ,$ whereas a futures contract generates a cash flow between inception and delivery, the interest rate, especially if it is random, plays an important role in the diference between the two kinds of contracts and the resulting diference in forward prices and futures prices. 

We start with discrete-time setting. 

Let $\{ t _ { j } \} _ { j = 0 , 1 , \dots , n }$ be an increasing discrete time grid with $t _ { 0 } = 0$ and $t _ { n } = T$ . We work under a risk-neutral measure $\widetilde { \mathbb { P } }$ and denote by $R ( t _ { j } )$ the (forward) short rate over $[ t _ { j } , t _ { j + 1 } )$ . Define the discount factor 

$$
D (t _ {j}) = \exp \left[ - \sum_ {i = 0} ^ {j - 1} R (t _ {i}) \left(t _ {i + 1} - t _ {i}\right) \right].
$$

Note that $D ( t _ { j } )$ is $\mathcal { F } ( t _ { j - 1 } )$ )-measurable and strictly positive. 

For a payof $S ( T )$ at time $T _ { : }$ define the discrete-time futures price by 

$$
\operatorname{Fut} (t _ {j}, T) = \widetilde {\mathbb {E}} \left[ S (T) \mid \mathcal {F} (t _ {j}) \right].
$$

(Martingale property via zero-cost settlement) A futures contract is marked-to-market at each $t _ { j }$ , with payof 

$$
\Delta_ {j} = \operatorname{Fut} (t _ {j + 1}, T) - \operatorname{Fut} (t _ {j}, T),
$$

settled at $t _ { j + 1 }$ . The present value at $t _ { j }$ of that settlement is 

$$
\frac {1}{D (t _ {j})} \widetilde {\mathbb {E}} \left[ D (t _ {j + 1})   \Delta_ {j} \mid \mathcal {F} (t _ {j}) \right].
$$

Zero-cost entry and exit require this to vanish. Since $D ( t _ { j + 1 } ) / D ( t _ { j } ) \neq 0$ and is $\mathcal { F } ( t _ { j } )$ -measurable, 

$$
\widetilde {\mathbb {E}} \left[ \mathrm{Fut} (t _ {j + 1}, T) \mid \mathcal {F} (t _ {j}) \right] = \mathrm{Fut} (t _ {j}, T),
$$

i.e. $\{ \mathrm { F u t } ( t _ { j } , T ) \}$ is a $\widetilde { \mathbb { P } } _ { - }$ martingale. 

We now turn to continuous-time setting. 

Let $\{ r ( u ) \} _ { u \ge 0 }$ be a progressively measurable short-rate process, and set 

$$
D (t) = \exp \left[ - \int_ {0} ^ {t} r (u) d u \right], \quad 0 \leq t \leq T,
$$

the continuous-time discount factor. Again work under the risk-neutral measure $\widetilde { \mathbb { P } } .$ 

Definition 1.3.16 (futures price). Let $S ( T )$ be an $\mathcal { F } ( T )$ -measurable random variable in a model with a risk-neutral measure $\widetilde { \mathbb { P } } .$ . The futures price at time t for delivery of one unit of S at time $T$ is 

$$
\mathrm{Fut} (t, T) = \widetilde {\mathbb {E}} [ S (T) \mid \mathcal {F} (t) ], 0 \leq t \leq T
$$

In particular, Fut $( T , T ) = S ( T )$ 

(Zero-value of the futures contract) In continuous time the daily settlements $\sum D \Delta \mathrm { F u t }$ become the stochastic integral 

$$
\int_ {t} ^ {T} D (u) d \left[ \operatorname{Fut} (u, T) \right].
$$

By the risk-neutral pricing formula, the value at time t of entering and then immediately exiting the contract is 

$$
\frac {1}{D (t)} \widetilde {\mathbb {E}} \left[ \int_ {t} ^ {T} D (u) d \mathrm{Fut} (u, T) \Big | \mathcal {F} (t) \right].
$$

Since $\mathrm { F u t } ( \cdot , T )$ is a Pe-martingale, the martingale representation theorem gives 

$$
d \operatorname{Fut} (u, T) = \Psi (u) d \widetilde {W} (u)
$$

for some adapted process Ψ. Thus 

$$
\int_ {t} ^ {T} D (u) \Psi (u) d \widetilde {W} (u)
$$

is an Itô integral whose conditional expectation (given $\mathcal { F } ( t ) )$ vanishes. Hence the futures contract has zero value at all times: 

$$
\left| \frac {1}{D (t)} \widetilde {\mathbb {E}} \left[ \int_ {t} ^ {T} D (u) d \operatorname{Fut} (u, T) \Big | \mathcal {F} (t) \right] = 0. \right|
$$

In summary, futures contract value is always zero, both in discrete and continuous time, because daily (or instantaneous) marked-to-market settlements cost nothing to enter and exit; in other words, the value of the contract is identically zero under no-arbitrage. Futures price is the conditional expectation of the terminal payof. 

Theorem 1.3.17 (Forward-futures spread). Assume S is an asset that does not pay a dividend and has zero cost of carry. Let $\mathrm { F o r } ( 0 , T )$ be the time-zero forward price for delivery of one unit of S at time T, and let Fut(0, T) be the time-zero futures price for the same. Then 

$$
\mathrm{For} (0, T) - \mathrm{Fut} (0, T) = \frac {1}{B (0 , T)} \widetilde {\mathrm{Cov}} [ D (T), S (T) ]
$$

where $\widetilde { \mathrm { C o v } }$ denotes covariance under the risk-neutral measure $\widetilde { \mathbb { P } } .$ 

Proof. By the definition of forward and futures prices with $t = 0 ,$ , the fact the $D ( t ) S ( t ) , 0 \leq t \leq T$ , is a Pe-martingale, and the formula ${ \cal B } ( 0 , T ) = \widetilde { \mathbb { E } } [ D ( T ) ]$ to compute 

$$
\begin{array}{r l} & {\mathrm{For} (0, T) - \mathrm{Fut} (0, T) = \frac {S (0)}{B (0 , T)} - \widetilde {\mathbb {E}} [ S (T) ]} \\ & {\qquad = \frac {1}{B (0 , T)} [ \widetilde {\mathbb {E}} [ D (T) S (T) ] - \widetilde {\mathbb {E}} [ D (T) ] \widetilde {\mathbb {E}} [ S (T) ] ] = \frac {1}{B (0 , T)} \widetilde {\mathrm{Cov}} [ D (T), S (T) ]} \end{array}
$$

□ 

Roughly speaking, forward-futures spread says that if the asset price $S$ is negatively correlated with the interest rate, so that $D ( T )$ is positively correlated with $S ( T )$ , then For $( 0 , T ) > \mathrm { F u t } ( 0 , T )$ . In the case that $S$ is negatively correlated with the interest rate, the long futures position tends to receive cash when the interest rate is falling and pay cash when the interest rate is rising. This is less favorable than the long forward position, which does not pay cash until the delivery date. To compensate for this disadvantage, the price $\mathrm { F u t } ( 0 , T )$ ultimately paid by the long futures position is lower than the price $\mathrm { F o r } ( 0 , T )$ paid upon delivery by the long forward position. The correlation considered here is under a risk-neutral measure, not the physical measure, but the direction of correlation under these two measures is generally the same. 

Note that, if the interest rate is not random, the $D ( T )$ is not random, and thus its correlation with $S ( T )$ is zero, so we have 

Corollary 1.3.18. Assume $S$ is an asset that does not pay a dividend and has zero cost $o f$ carry. $I f$ the interest rate is not random, then the forward price and the futures price for delivery of one unit of $S$ at time $T$ are equal. 

Example 1.3.19 (Forward-futures interest rate spread in the Ho-Lee model). Recall that the forward interest rate in the Ho-Lee model is 

$$
f (t, T) = R (t) + \int_ {t} ^ {T} \alpha (u) d u - \frac {1}{2} \sigma^ {2} (T - t) ^ {2}, 0 \leq t \leq T
$$

In addition to being an instantaneous interest rate that can be locked in at time t for borrowing at time $T ,$ this is the forward price $\mathrm { F o r } _ { R } ( t , T ) ^ { 9 }$ of the contract that pays $R ( T )$ at time $T ,$ 

In the Ho-Lee model, we have 

$$
R (T) = R (t) + \int_ {t} ^ {T} \alpha (u) d u + \sigma (\widetilde {W} (T) - \widetilde {W} (t))
$$

from which we see that the futures $p r i c e ^ { 1 0 }$ at time t for the payment $R ( T )$ at time $\textit { T i s } ^ { 1 1 }$ 

$$
\mathrm{Fut} _ {R} (t, T) = \widetilde {\mathbb {E}} [ R (T) \mid \mathcal {F} (t) ] = R (t) + \int_ {t} ^ {T} \alpha (u) d u, 0 \leq t \leq T
$$

It follows that 

$$
d \mathrm{Fut} _ {R} (t, T) = d R (t) - \alpha (t) d t = \sigma d \widetilde {W} (t)
$$

The futures price is a martingale under the risk-neutral measure. In this case, the price $R ( T )$ of the underlying asset delivered at time $T$ is positively correlated with the interest rate and negatively correlated with $D ( T )$ We have the opposite of the situation described above. The interest rate forward-futures spread is 

$$
\mathrm{For} _ {R} (t, T) - \mathrm{Fut} _ {R} (t, T) = - \frac {1}{2} \sigma^ {2} (T - t) ^ {2}
$$

which is negative. Recall that σ appearing in this formula is the volatility of the interest rate. 

## Trading futures contracts

Futures contracts are traded on many asset classes, e.g., stock indices, agricultural commodities, metals, and oil. There are even futures contracts on non-asset time series such as weather. Futures can be easier to trade than the underlying assets, and hence are often used for hedging. In this section, we consider futures trading and give some examples of replication (hedging) with futures. 

Suppose at time $t , 0 \leq t \leq T$ , an agent holds $\Delta ( t )$ futures contracts and finances her trading using the money market account with interest rate $R ( t ) , 0 \leq t \leq T$ . For now let us assume that the interest paid on the agent’s margin account is also $R ( t )$ . The agent’s portfolio consists of the futures contracts held and cash. Some of the cash is in the margin account and the remainder is invested or borrowed at the money market rate $R ( t )$ . The position in futures always has zero value and thus does not contribute to the agent’s portfolio value. In other words, all the agent’s portfolio value is in cash. The futures contracts held afect the diferential of the portfolio value, but do not contribute to the portfolio value itself. Thus, 

$$
d X (t) = \Phi (t) d \mathrm{Fut} (t, T) + R (t) X (t) d t\tag{1.3.62}
$$

and 

$$
d (D (t) X (t)) = D (t) (- R (t) X (t) + d X (t)) = D (t) \Phi (t) d \operatorname{Fut} (t, T)\tag{1.3.63}
$$

Example 1.3.20 (Black-Scholes futures hedging). Consider a geometric Brownian motion price process S(t) with diferential 

$$
d S (t) = r S (t) d t + \sigma S (t) d \widetilde {W} (t), 0 \leq t \leq T
$$

where the interest rate r and the volatility $\sigma > 0$ are constant and $\widetilde { W }$ is a Brownian motion under a riskneutral measure $\widetilde { \mathbb { P } }$ . The futures price for delivery of one unit of $S$ at time $T$ is 

$$
\mathrm{Fut} _ {S} (t, T) = \widetilde {\mathbb {E}} [ S (T) \mid \mathcal {F} (t) ] = e ^ {r T} \widetilde {\mathbb {E}} \left[ e ^ {- r T} S (T) \mid \mathcal {F} (t) \right] = e ^ {r (T - t)} S (t)\tag{1.3.64}
$$

(This is also the forward price because the interest rate is constant. In particular, $B ( t , T ) = e ^ { - r ( T - t ) }$ , so $\operatorname { F o r } _ { S } ( t , T ) = S ( t ) / B ( t , T ) = e ^ { r ( T - t ) } S ( t ) . )$ The diferential of the futures price is 

$$
d \mathrm{Fut} _ {S} (t, T) = - r e ^ {r (T - t)} S (t) d t + e ^ {r (T - t)} d S (t) = \sigma e ^ {r (T - t)} S (t) d \widetilde {W} (t)
$$

As always, the futures price is a martingale under the risk-neutral measure. 

Consider an agent who at each time t holds $\Phi ( t )$ futures contracts and finances trading using the money market account. From (1.3.63) and $( 1 . 3 . 6 \% )$ , we have 

$$
d \left(e ^ {- r t} X (t)\right) = \sigma e ^ {r (T - 2 t)} \Phi (t) S (t) d \widetilde {W} (t)\tag{1.3.65}
$$

This discounted portfolio process is a martingale under the risk-neutral measure. For $0 \leq t \leq T$ , the price at time t of a European call on $S$ expiring at time T with strike price K is 

$$
c (t, S (t)) = S (t) N \left(d _ {+} (t)\right) - e ^ {- r (T - t)} K N \left(d _ {-} (t)\right)
$$

where 

$$
d _ {\pm} (t) = \frac {1}{\sigma \sqrt {T - t}} \left[ \log \frac {S (t)}{K} + \left(r \pm \frac {1}{2} \sigma^ {2}\right) (T - t) \right]
$$

The diferential of the discounted call price is 

$$
\begin{array}{r l} & {d \left(e ^ {- r t} c (t, S (t))\right) = e ^ {- r t} \left(- r c d t + c _ {t} d t + c _ {x} d S (t) + \frac {1}{2} c _ {x x} d S (t) d S (t)\right)} \\ & {\qquad = e ^ {- r t} \left(- r c + c _ {t} + r S (t) c _ {x} + \frac {1}{2} \sigma^ {2} S ^ {2} (t) c _ {x x}\right) d t + \sigma S (t) c _ {x} (t, S (t)) d \widetilde {W} (t)} \\ & {\qquad = \sigma e ^ {- r t} S (t) c _ {x} (t, S (t)) d \widetilde {W} (t)} \end{array}\tag{1.3.66}
$$

because $c ( t , x )$ satisfies the Black-Scholes partial diferential equation 

$$
r c (t, x) = c _ {t} (t, x) + r x c _ {x} (t, x) + \frac {1}{2} \sigma^ {2} x ^ {2} c _ {x x} (t, x), \quad 0 \leq t <   T, x \geq 0
$$

Equating (1.3.65) and (1.3.66), we see that to replicate the call, the agent should take $X ( 0 ) = c ( 0 , S ( 0 ) )$ and 

$$
\Phi (t) = e ^ {- r (T - t)} c _ {x} (t, S (t))
$$

From $( 1 . 3 . 6 4 ) ,$ we see that the futures price at time t is the asset price $S ( t )$ scaled up by $e ^ { r ( T - t ) }$ . Therefore, the hedge ratio $\Phi ( t )$ for trading in futures is the hedge ratio $\Delta ( t ) = c _ { x } ( t , S ( t ) )$ for trading in the underlying asset scaled down by $e ^ { - r ( T - t ) }$ 

End of Lecture 9 

## 1.4 Financing portfolios

## 1.4.1 Self-financing portfolio

For simplicity, consider a portfolio with two (risky) assets: $S _ { 1 } , S _ { 2 }$ , so that we have the portfolio value $X ( t )$ such that 

$$
X (t) = \Delta (t) S _ {1} (t) + \Gamma (t) S _ {2} (t)
$$

In diferential, we (wish to) have 

$$
d X (t) = \Delta (t) d S _ {1} (t) + \Gamma (t) d S _ {2} (t)\tag{1.4.1}
$$

Note that this is not true in general but a condition called self-financing. This is because, by Itô’s product rule, we have 

$$
d X (t) = \Delta (t) d S _ {1} (t) + S _ {1} (t) d \Delta (t) + d S _ {1} (t) d \Delta (t) + \Gamma (t) d S _ {2} (t) + S _ {2} (t) d \Gamma (t) + d S _ {2} (t) d \Gamma (t)
$$

So to satisfy (1.4.1), we need 

$$
S _ {1} (t) d \Delta (t) + d S _ {1} (t) d \Delta (t) + S _ {2} (t) d \Gamma (t) + d S _ {2} (t) d \Gamma (t) = 0\tag{1.4.2}
$$

In discrete time, (1.4.2) implies: 

$$
\begin{array}{c} S _ {1} \left(t _ {j - 1}\right) \left[ \Delta (t _ {j}) - \Delta (t _ {j - 1}) \right] + \left[ \Delta (t _ {j}) - \Delta (t _ {j - 1}) \right] \left[ S _ {1} (t _ {j}) - S _ {1} (t _ {j - 1}) \right] \\ + S _ {2} \left(t _ {j - 1}\right) \left[ \Gamma (t _ {j}) - \Gamma (t _ {j - 1}) \right] + \left[ S _ {2} (t _ {j}) - S _ {2} (t _ {j - 1}) \right] \left[ \Gamma (t _ {j}) - \Gamma (t _ {j - 1}) \right] \\ = S _ {1} (t _ {j}) \left[ \Delta (t _ {j}) - \Delta (t _ {j - 1}) \right] + S _ {2} (t _ {j}) \left[ \Gamma (t _ {j}) - \Gamma (t _ {j - 1}) \right] = 0. \end{array}
$$

Example 1.4.1 (Black’s formula). Consider the model 

$$
X (t) = C (t) = S (t) N \left(d _ {+} (t, \operatorname{For} (t, T))\right) - K B (t, T) N \left(d _ {-} (t, \operatorname{For} (t, T))\right)
$$

To equate 

$$
d X (t) \stackrel {?} {=} \Delta_ {1} (t) d S (t) + \Gamma (t) d B (t, T),
$$

We suggest that 

$$
\Delta_ {1} (t) = N (d _ {+} (t, \mathrm{For} (t, T))), \qquad \Gamma (t) = - K N (d _ {-} (t, \mathrm{For} (t, T)))
$$

achieves the self-financing condition. 

Example 1.4.2 (Using money market to finance trading). Let $S ( t )$ be a risky asset price process and let 

$$
M (t) = e ^ {r t}, \quad r > 0,
$$

be the value at time t of one unit invested in the risk-free money-market. Then 

$$
d M (t) = r M (t) d t.
$$

A trading strategy is given by progressively measurable processes $\Delta ( t )$ and $\Gamma ( t )$ , denoting the number of shares $o f S$ and units of M. The portfolio value is 

$$
X (t) = \Delta (t) S (t) + \Gamma (t) M (t).
$$

We require the strategy to be self-financing, i.e. 

$$
d X (t) = \Delta (t) d S (t) + \Gamma (t) d M (t).
$$

Applying Itô’s product rule to $X ( t ) = \Delta S + \Gamma M$ yields 

$$
d X (t) = \Delta d S + S d \Delta + d \langle \Delta , S \rangle + \Gamma d M + M d \Gamma + d \langle \Gamma , M \rangle .
$$

Comparison with the self-financing relation gives the financing condition 

$$
S (t) d \Delta (t) + M (t) d \Gamma (t) + d \langle \Delta , S \rangle_ {t} + d \langle \Gamma , M \rangle_ {t} = 0,
$$

which in continuous-difusion models reduces to 

$$
S (t) d \Delta (t) + M (t) d \Gamma (t) = 0.
$$

Since $X = \Delta S + \Gamma M _ { ; }$ , one solves 

$$
\Gamma (t) = \frac {X (t) - \Delta (t) S (t)}{M (t)},
$$

so that $\Gamma ( t ) M ( t )$ is precisely the cash position. 

To replicate a European call with payof $X ( T ) ~ = ~ ( S ( T ) - K ) ^ { + }$ , set $X ( t ) ~ = ~ c ( t , S ( t ) )$ Under the self-financing condition and risk-neutral valuation one obtains the Black-Scholes PDE. The resulting deltahedging strategy is 

$$
\Delta (t) = \frac {\partial c}{\partial S} \left(t, S (t)\right), \qquad \Gamma (t) = \frac {c \left(t , S (t)\right) - \Delta (t) S (t)}{M (t)}.
$$

## Trading-floor derivation of the Black-Scholes PDE

This section records the well-known “trading-floor” (heuristic) route to the Black-Scholes equation. The argument is illustrative—it shows why a delta-hedged portfolio is almost risk-free—but it is not itself rigorous; the two key shortcuts we highlight below happen to cancel. 

For the set up, at time t we hold one European call worth $c ( t , S ( t ) )$ and sell $\Delta ( t , S ( t ) )$ shares of the underlying $S ( t )$ . The portfolio 

$$
Y (t) = c (t, S (t)) - \Delta (t, S (t)) S (t), \quad \Delta (t, S (t)) := \frac {\partial c}{\partial S} (t, S (t)).
$$

Assume the stock follows 

$$
d S (t) = \mu S (t) d t + \sigma S (t) d W (t), \quad (d S) ^ {2} = \sigma^ {2} S ^ {2} d t.
$$

(Flawed Itô calculation) Applying Itô to $c ( t , S ( t ) )$ and ignoring the stochasticity of $\Delta ( t , S ( t ) )$ one obtains 

$$
d Y (t) = \left(\frac {\partial c}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} c}{\partial S ^ {2}}\right) d t\tag{1.4.3}
$$

The dS-terms appear to cancel. 

(Flawed risk-free argument) Because $\Delta ( t , S ( t ) )$ is chosen so that the portfolio is locally insensitive to $d S ,$ traders treat Y as instantaneously riskless; hence 

$$
d Y (t) = r Y (t) d t.\tag{1.4.4}
$$

Setting the right-hand sides of Equations (1.4.3) and (1.4.4) equal and rearranging yields 

$$
\frac {\partial c}{\partial t} + r S \frac {\partial c}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} c}{\partial S ^ {2}} - r c = 0,
$$

the Black-Scholes PDE. 

So why does this seem to be correct? Correction 1: define $\begin{array} { r } { \Delta : = { \frac { \partial c } { \partial S } } } \end{array}$ and apply Itô to the whole portfolio: 

$$
d Y = \left(\frac {\partial c}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} c}{\partial S ^ {2}}\right) d t - S d \Delta - d S d \Delta .\tag{1.4.5}
$$

Meanwhile, consider Figure 1.4.1. The solid curve is the call-price surface $x \mapsto c ( t , x )$ , a convex function of the spot. The dashed line is the tangent at the current spot $x = S ( t )$ ; its slope $\Delta = \partial c / \partial x$ represents the delta of the option. The current state is at $( S ( t ) , c ( t , S ( t ) ) )$ . The vertical gap between the curve and the tangent, $Y = c - \Delta S$ , equals the value of the delta-hedged portfolio. Although this gap is locally flat at $x = S ( t )$ (hence the position is instantaneously insensitive to small moves in S), the entire curve shifts over time, so re-hedging is required; the position is not truly risk-free. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/e65d9d41-4c7a-4366-aaab-be3784392ae9/6ffa60100c06a3ba3decac1ff9245622fd74d889b18a735569841cea90376f00.jpg)



Figure 1.4.1: Call price $c ( t , x )$ and its tangent at the current spot $x = S ( t )$


Correction 2: define Γ such that 

$$
Y (t) = c (t, S (t)) - \frac {\partial c}{\partial S} (t, S (t))   S (t) =: \Gamma (t)   e ^ {r t}.
$$

Taking the diferential correctly, one gets 

$$
d Y = \underbrace {\Gamma (t) r e ^ {r t}} _ {r Y (t)} d t + e ^ {r t} d \Gamma (t) + d e ^ {r t} d \Gamma (t);\tag{1.4.6}
$$

The terms omitted in (1.4.3) and (1.4.4) are exactly $- S d \Delta - d S d \Delta$ and $e ^ { r t } d \Gamma + d e ^ { r t } d \Gamma$ , respectively, and note that (1.4.5) and (1.4.6) reconcile and the two errors cancel, because 

$$
e ^ {r t} d \Gamma + d e ^ {r t} d \Gamma = - S d \Delta - d S d \Delta
$$

is exactly the self-financing condition (1.4.2). A fully rigorous derivation starts from (1.4.5)–(1.4.6) rather than (1.4.3)–(1.4.4). 

## 1.4.2 Funding and collateral considerations

Reference: [Pit10], [BBPL12]. Below is a direct excerpt from [Pit10]. 

Classic derivative-pricing textbooks assume a trader can borrow and lend at one universal “risk-free” rate. Since 2008, that fiction has broken down: banks face a menu of funding rates—secured vs. unsecured, bank-specific credit spreads, repo, collateral rates, etc. For a derivatives desk, funding is now the dominant practical cost because every hedge or replication step requires borrowing or lending cash or securities at one of those rates. 

We start with the risk-free curve for lending, a curve that corresponds to the safest available collateral (cash). We denote the corresponding short rate at time t by $r _ { C } ( t )$ ; C here stands for $\mathrm { \Delta C S A } '$ , as we assume this is the agreed overnight rate paid on collateral among dealers under CSA. It is convenient to parameterise term curves in terms of discount factors; we denote corresponding riskfree discount factors by $P _ { C } ( t , T ) , 0 \leq t \leq$ $T < \infty$ . Standard Heath-Jarrow-Morton theory applies, and we specify the following dynamics for the yield curve: 

$$
d P _ {C} (t, T) / P _ {C} (t, T) = r _ {C} (t) d t - \sigma_ {C} (t, T) ^ {\top} d W _ {C} (t)\tag{1.4.7}
$$

where $W _ { c } ( t )$ is a d-dimensional Brownian motion under the riskneutral measure $P$ and $\sigma _ { C }$ is a vector-valued (dimension d) stochastic process. 

In what follows, we shall consider derivatives contracts on a particular asset, whose price process we denote by $S ( t ) , t \geq 0$ . We denote by $r _ { R } ( t )$ the short rate on funding secured by this asset (here $^ { , } \mathrm { ~ R ~ } ^ { , }$ stands for ’repo’). The diference $r _ { C } ( \mathrm { t } ) - r _ { R } ( t )$ is sometimes called the stock lending fee. Finally, let us define the short rate for unsecured funding by $r _ { F } ( t ) , t \geq 0 .$ . As a rule, we would expect that $r _ { C } ( t ) \leq r _ { R } ( t ) \leq r _ { F } ( t )$ 

The existence of non-zero spreads between short rates based on diferent collateral can be recast in the language of credit risk, by introducing joint defaults between the bank and various assets used as collateral for funding. In particular, the funding spread $s _ { F } ( t ) : = r _ { F } ( t ) - r _ { C } ( t )$ could be thought of as the (stochastic) intensity of default of the bank. We do not pursue this formalism here, postulating the dynamics of funding curves directly instead. Likewise, we ignore the possibility of a counterparty default, an extension that could be developed rather easily. 

## Black-Scholes with collateral

Let us look at how the standard Black-Scholes pricing formula changes in the presence of a CSA. Let $S ( t )$ be an asset that follows, in the real world, the following dynamics: 

$$
d S (t) / S (t) = \mu_ {S} (t) d t + \sigma_ {S} (t) d W (t)
$$

Let $V ( t , S )$ be a derivatives security on the asset; by Itô’s lemma it follows that: 

$$
d V (t) = (\mathcal {L} V (t)) d t + \Delta (t) d S (t)
$$

where $\mathcal { L }$ is the standard pricing operator: 

$$
\mathcal {L} = \frac {\partial}{\partial t} + \frac {\sigma_ {S} (t) ^ {2} S ^ {2}}{2} \frac {\partial^ {2}}{\partial S ^ {2}}
$$

and $\Delta$ is the option’s delta: 

$$
\Delta (t) = \frac {\partial V (t)}{\partial S}
$$

Let $C ( t )$ be the collateral (cash in the collateral account) held at time t against the derivative. For flexibility, we allow this amount to be diferent<sup>12</sup> from $V ( t )$ 

To replicate the derivative, at time t we hold $\Delta ( t )$ units of stock and $\gamma ( t )$ cash. Then the value of the replication portfolio, which we denote by Π(t), is equal to: 

$$
V (t) = \Pi (t) = \Delta (t) S (t) + \gamma (t)\tag{1.4.8}
$$

The cash amount $\gamma ( t )$ is split among a number of accounts: 

• Amount $C ( t )$ is in collateral. 

• Amount $V ( t ) - C ( t )$ needs to be borrowed/lent unsecured from the treasury desk. 

• Amount $\Delta ( t ) S ( t )$ is borrowed to finance the purchase of $\Delta ( t )$ stocks. It is secured by stock purchased. 

• Stock is paying dividends at rate $r _ { D }$ 

The growth of all cash accounts $g ( t ) d t$ (collateral, unsecured, stock-secured, dividends) is given by: 

$$
g (t) d t = [ r _ {C} (t) C (t) + r _ {F} (t) (V (t) - C (t)) - r _ {R} (t) \Delta (t) S (t) + r _ {D} (t) \Delta (t) S (t) ] d t
$$

On the other hand, from (1.4.8), by the self-financing condition: 

$$
g (t) d t = d V (t) - \Delta (t) d S (t)
$$

which is, by Itô’s lemma: 

$$
d V (t) - \Delta (t) d S (t) = (\mathcal {L} V (t)) d t = \left(\frac {\partial}{\partial t} + \frac {\sigma_ {S} (t) ^ {2}}{2} S ^ {2} \frac {\partial^ {2}}{\partial S ^ {2}}\right) V (t) d t
$$

Thus we have: 

$$
\left(\frac {\partial}{\partial t} + \frac {\sigma_ {S} (t) ^ {2}}{2} S ^ {2} \frac {\partial^ {2}}{\partial S ^ {2}}\right) V = r _ {C} (t) C (t) + r _ {F} (t) (V (t) - C (t)) + \left(r _ {D} (t) - r _ {R} (t)\right) \frac {\partial V}{\partial S} S
$$

which, after some rearrangement, yields: 

$$
\left| \frac {\partial V}{\partial t} + (r _ {R} (t) - r _ {D} (t)) \frac {\partial V}{\partial S} S + \frac {\sigma_ {S} (t) ^ {2}}{2} S ^ {2} \frac {\partial^ {2} V}{\partial S ^ {2}} = r _ {F} (t) V (t) - (r _ {F} (t) - r _ {C} (t)) C (t) \right|
$$

The solution, obtained by essentially following the steps that lead to the Feynman-Kac formula, is given by: 

$$
V (t) = \mathbb {E} _ {t} \left(e ^ {- \int_ {t} ^ {T} r _ {F} (u) d u} V (T) + \int_ {t} ^ {T} e ^ {- \int_ {t} ^ {u} r _ {F} (v) d v} \left(r _ {F} (u) - r _ {C} (u)\right) C (u) d u\right)\tag{1.4.9}
$$

in the measure in which the stock grows at rate $r _ { R } ( t ) - r _ { D } ( t )$ , that is: 

$$
d S (t) / S (t) = \left(r _ {R} (t) - r _ {D} (t)\right) d t + \sigma_ {S} (t) d W _ {S} (t)\tag{1.4.10}
$$

By rearranging terms in (1.4.9), we obtain another useful formula for the value of the derivative: 

$$
V (t) = \mathbb {E} _ {t} \left(e ^ {- \int_ {t} ^ {T} r _ {c} (u) d u} V (T)\right) - \mathbb {E} _ {t} \left(\int_ {t} ^ {T} e ^ {- \int_ {t} ^ {u} r _ {c} (v) d v} \left(r _ {F} (u) - r _ {C} (u)\right) (V (u) - C (u)) d u\right)\tag{1.4.11}
$$

We note that: 

$$
\begin{array}{c} \mathbb {E} _ {t} (d V (t)) = (r _ {F} (t) V (t) - (r _ {F} (t) - r _ {C} (t))   C (t))   d t \\ = (r _ {F} (t) V (t) - s _ {F} (t) C (t))   d t \end{array}\tag{1.4.12}
$$

So, the rate of growth in the derivatives security is the funding spread $r _ { F } ( t )$ applied to its value minus the credit spread $s _ { F } ( t )$ applied to the collateral. 

(Full collateral) In particular, if the collateral is equal to the value V then: 

$$
\mathbb {E} _ {t} (d V (t)) = r _ {C} (t) V (t) d t, \quad V (t) = \mathbb {E} _ {t} \left(e ^ {- \int_ {t} ^ {T} r _ {c} (u) d u} V (T)\right)\tag{1.4.13}
$$

and the derivative grows at the risk-free rate. The final value is the only payment that appears in the discounted expression as the other payments net out given the assumption of full collateralisation. This is consistent with the drift in (1.4.7) as $P _ { C } ( t , T )$ corresponds to deposits secured by cash collateral. This case could be handled by using a measure that corresponds to the risk-free bond 

$$
P _ {C} (t, T) = \mathbb {E} _ {t} \left(e ^ {- \int_ {t} ^ {T} T _ {c} (u) d u}\right)
$$

as a numéraire. 

(Zero collateral) On the other hand, if the collateral is zero, then: 

$$
\mathbb {E} _ {t} (d V (t)) = r _ {F} (t) V (t) d t\tag{1.4.14}
$$

and the rate of growth is equal to the bank’s unsecured funding rate or, using credit risk language, adjusted for the possibility of the bank default. This case could be handled by using a measure that corresponds to the risky bond 

$$
P _ {F} (t, T) = \mathbb {E} _ {t} \left(e ^ {- \int_ {t} ^ {T _ {F}} (u) d u}\right)
$$

as a numéraire. 

End of Lecture 10 

## 1.5 Foreign and domestic risk-neutral measures

Reference: [Shr04, §9.3]. 

## FX is always confusing but never complicated.

We consider a market with two currencies, A (domestic) and B (foreign). For concreteness, one might think of A as US Dollars (USD) and B as Euros (EUR). The exchange rate process $X ^ { B | A } ( t )$ denotes the price of one unit of currency B expressed in units of currency A at time t. For example, if $\dot { X } ^ { \mathrm { E U R | U S D } } ( t ) = \dot { 1 } . 1 4$ , it costs 1.14 USD to buy 1 EUR at time t. 

This notation behaves algebraically like fractions: 

$X ^ { B | A } ( t ) \cdot X ^ { C | B } ( t ) = X ^ { C | A } ( t )$ (Triangular relationship) 

${ \frac { X ^ { B | A } ( t ) } { X ^ { C | A } ( t ) } } = X ^ { B | C } ( t )$ 

$\begin{array} { r } { X ^ { A | B } ( t ) = \frac { 1 } { X ^ { B | A } ( t ) } } \end{array}$ (Inversion) 

We model the financial market under the physical measure P. Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space equipped with a filtration $\{ \mathcal { F } ( t ) \} _ { t \geq 0 }$ generated by two independent standard Brownian motions $W _ { 1 } ( t )$ and $W _ { 2 } ( t )$ 

The market consists of: 

1. A domestic money market account $M ^ { A } ( t )$ growing at a constant risk-free rate $r _ { A } \colon$ 

$$
d M ^ {A} (t) = r _ {A} M ^ {A} (t) d t,
$$

with $M ^ { A } ( 0 ) = 1$ , so $M ^ { A } ( t ) = e ^ { r _ { A } t }$ . The corresponding discount factor is $D ^ { A } ( t ) = e ^ { - r _ { A } t }$ 

2. A foreign money market account $M ^ { B } ( t )$ growing at a constant risk-free rate $r _ { B } \colon$ 

$$
d M ^ {B} (t) = r _ {B} M ^ {B} (t) d t,
$$

with $M ^ { B } ( 0 ) = 1$ , so $M ^ { B } ( t ) = e ^ { r _ { B } t }$ . The corresponding discount factor is $D ^ { B } ( t ) = e ^ { - r _ { B } t }$ 

3. A risky asset $S ( t )$ , denominated in the domestic currency A, following a geometric Brownian motion: 

$$
d S (t) = \alpha S (t) d t + \sigma S (t) d W _ {1} (t),\tag{1.5.1}
$$

where α is the constant expected rate of return and $\sigma > 0$ is the constant volatility. 

4. The exchange rate $X ^ { B | A } ( t )$ , also following a geometric Brownian motion, potentially correlated with $S ( t )$ : 

$$
d X ^ {B | A} (t) = \gamma X ^ {B | A} (t) d t + \sigma_ {2} X ^ {B | A} (t) \left(\rho d W _ {1} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} (t)\right),\tag{1.5.2}
$$

where $\gamma$ is the constant expected rate of change, $\sigma _ { 2 } > 0$ is the constant volatility of the exchange rate, and $\rho \in ( - 1 , 1 )$ is the constant correlation coeficient between the Brownian drivers of $S ( t )$ and $X ^ { B | \dot { A } } ( t )$ 

It is sometimes convenient to represent the volatilities as vectors corresponding to the coeficients of $d W _ { 1 }$ and $d W _ { 2 }$ 

• Volatility vector for $S ( t ) \colon \vec { \sigma } _ { S } = ( \sigma , 0 )$ . The magnitude $| \vec { \sigma } _ { S } | = \sigma$ is the standard volatility. 

• Volatility vector for $X ^ { B | A } ( t ) \colon \vec { \sigma } _ { X } = ( \rho \sigma _ { 2 } , \sqrt { 1 - \rho ^ { 2 } } \sigma _ { 2 } )$ . The magnitude 

$$
| \vec {\sigma} _ {X} | = \sqrt {(\rho \sigma_ {2}) ^ {2} + (\sqrt {1 - \rho^ {2}} \sigma_ {2}) ^ {2}} = \sqrt {\rho^ {2} \sigma_ {2} ^ {2} + (1 - \rho^ {2}) \sigma_ {2} ^ {2}} = \sigma_ {2}
$$

is the standard volatility. 

Volatility vectors have the useful property that for a ratio of two processes $Z _ { 1 } / Z _ { 2 }$ , the volatility vector of the ratio is the diference of the individual volatility vectors: $\vec { \sigma } _ { Z _ { 1 } / Z _ { 2 } } = \vec { \sigma } _ { Z _ { 1 } } - \vec { \sigma } _ { Z _ { 2 } }$ 

## 1.5.1 Domestic risk-neutral measure

We seek a risk-neutral measure $\mathbb { P } ^ { A }$ equivalent to $\mathbb { P } ,$ under which asset prices denominated in the domestic currency A, when discounted by the domestic discount factor $D ^ { A } ( t )$ , become martingales. This implies that under $\mathbb { P } ^ { A }$ , the expected rate of return for any traded asset denominated in currency A must equal the domestic risk-free rate $r _ { A }$ 

Let $W _ { 1 } ^ { A } ( t )$ and $W _ { 2 } ^ { A } ( t )$ be two independent standard Brownian motions under $\mathbb { P } ^ { A }$ . By Girsanov’s theorem, there exist market price of risk processes $\Theta _ { 1 } ( t )$ and $\Theta _ { 2 } ( t )$ such that: 

$$
\begin{array}{l} {d W _ {1} ^ {A} (t) = d W _ {1} (t) + \Theta_ {1} (t) d t} \\ {d W _ {2} ^ {A} (t) = d W _ {2} (t) + \Theta_ {2} (t) d t} \end{array}
$$

In our constant coeficient setting, $\Theta _ { 1 }$ and $\Theta _ { 2 }$ will be constants. 

Applying the risk-neutral requirement to asset $S ( t )$ : The dynamics under $\mathbb { P }$ are $d S ( t ) ~ = ~ \alpha S ( t ) d t ~ +$ $\sigma S ( t ) d W _ { 1 } ( t )$ . Substituting $d W _ { 1 } ( t ) = d W _ { 1 } ^ { A } ( t ) - \Theta _ { 1 } d t ^ { }$ 

$$
d S (t) = \alpha S (t) d t + \sigma S (t) (d W _ {1} ^ {A} (t) - \Theta_ {1} d t) = (\alpha - \sigma \Theta_ {1}) S (t) d t + \sigma S (t) d W _ {1} ^ {A} (t).
$$

For the drift to be $r _ { A } S ( t ) d t$ under $\mathbb { P } ^ { A }$ , we must have: 

$$
\alpha - \sigma \Theta_ {1} = r _ {A} \quad \Longrightarrow \quad \alpha = r _ {A} + \sigma \Theta_ {1}.\tag{1.5.3}
$$

This is the first market price of risk (MPR) equation. It determines $\Theta _ { 1 } = ( \alpha - r _ { A } ) / \sigma$ 

Now consider the investment strategy from the perspective of a domestic (A) investor: investing in the foreign $( B )$ money market account $M ^ { B } ( t )$ . The value of this investment in the domestic currency A is $V ( t ) \stackrel { - } { = } \dot { M ^ { B } } ( t ) X ^ { \dot { B } | A } ( t )$ . This represents a traded asset denominated in currency A. We need to find its dynamics under P. Using Itô’s product rule for $V ( t ) = M ^ { B } ( t ) X ^ { B | A } ( t )$ : 

$$
\begin{array}{l} d V (t) = M ^ {B} (t) d X ^ {B | A} (t) + X ^ {B | A} (t) d M ^ {B} (t) + d M ^ {B} (t) d X ^ {B | A} (t) \\ \qquad = M ^ {B} (t) \left[ \gamma X ^ {B | A} (t) d t + \sigma_ {2} X ^ {B | A} (t) (\rho d W _ {1} + \sqrt {1 - \rho^ {2}} d W _ {2}) \right] + X ^ {B | A} (t) [ r _ {B} M ^ {B} (t) d t ] + 0 \\ \qquad \text {(since} d M ^ {B} d X ^ {B | A} \text {involves} d t \cdot d t \text {or} d t \cdot d W) \\ \qquad = (r _ {B} + \gamma) M ^ {B} (t) X ^ {B | A} (t) d t + \sigma_ {2} M ^ {B} (t) X ^ {B | A} (t) (\rho d W _ {1} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} (t)) \\ \qquad = (r _ {B} + \gamma) V (t) d t + \sigma_ {2} V (t) (\rho d W _ {1} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} (t)). \end{array}
$$

Under the risk-neutral measure $\mathbb { P } ^ { A }$ , this asset must also have an expected return of $r _ { A }$ . Substituting $d W _ { 1 } =$ $d W _ { 1 } ^ { A } - \Theta _ { 1 } d t$ and $d W _ { 2 } = d W _ { 2 } ^ { A } - \Theta _ { 2 } d t$ 

$$
\begin{array}{r l} & {d V (t) = (r _ {B} + \gamma) V (t) d t + \sigma_ {2} V (t) (\rho (d W _ {1} ^ {A} - \Theta_ {1} d t) + \sqrt {1 - \rho^ {2}} (d W _ {2} ^ {A} - \Theta_ {2} d t))} \\ & {\qquad = \Big [ r _ {B} + \gamma - \sigma_ {2} \rho \Theta_ {1} - \sigma_ {2} \sqrt {1 - \rho^ {2}} \Theta_ {2} \Big ] V (t) d t + \sigma_ {2} V (t) (\rho d W _ {1} ^ {A} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A} (t)).} \end{array}
$$

For the drift to be $r _ { A } V ( t ) d t$ under $\mathbb { P } ^ { A }$ , we must have: 

$$
r _ {B} + \gamma - \sigma_ {2} \rho \Theta_ {1} - \sigma_ {2} \sqrt {1 - \rho^ {2}} \Theta_ {2} = r _ {A}.\tag{1.5.4}
$$

This is the second MPR equation. 

Given $\alpha , \sigma , r _ { A } , \gamma , \sigma _ { 2 } , \rho , r _ { B }$ , equations (1.5.3) and (1.5.4) form a system of two linear equations for the two unknowns $\Theta _ { 1 }$ and $\Theta _ { 2 } .$ . Since $\sigma > 0$ and $\sigma _ { 2 } { \sqrt { 1 - \rho ^ { 2 } } } > 0$ (as $| \rho | < 1 )$ , this system has a unique solution for $\Theta _ { 1 }$ and $\Theta _ { 2 }$ . This implies the market is complete with respect to the sources of randomness $W _ { 1 } , W _ { 2 }$ and the traded assets $S ( t ) , M ^ { B } ( t ) X ^ { B | A } ( t )$ , and there exists a unique domestic risk-neutral measure $\mathbb { P } ^ { A }$ 

The Radon-Nikodym derivative process defining the change of measure from P to $\mathbb { P } ^ { A }$ on $\mathcal { F } _ { t }$ is given by the stochastic exponential $\begin{array} { r } { Z ^ { A } ( t ) = \frac { \hat { d } \mathbb { P } ^ { A } } { d \mathbb { P } } | _ { \mathcal { F } _ { t } } } \end{array}$ 

$$
Z ^ {A} (t) = \mathcal {E} \left(- \int_ {0} ^ {t} \Theta_ {1} d W _ {1} (u) - \int_ {0} ^ {t} \Theta_ {2} d W _ {2} (u)\right)
$$

$$
Z ^ {A} (t) = \exp \left(- \Theta_ {1} W _ {1} (t) - \Theta_ {2} W _ {2} (t) - \frac {1}{2} (\Theta_ {1} ^ {2} + \Theta_ {2} ^ {2}) t\right).
$$

Under the domestic risk-neutral measure $\mathbb { P } ^ { A }$ , the dynamics of the primary assets become: 

$$
d S (t) = r _ {A} S (t) d t + \sigma S (t) d W _ {1} ^ {A} (t)\tag{1.5.5}
$$

$$
d (M ^ {B} (t) X ^ {B | A} (t)) = r _ {A} M ^ {B} (t) X ^ {B | A} (t) d t + \sigma_ {2} M ^ {B} (t) X ^ {B | A} (t) (\rho d W _ {1} ^ {A} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A} (t))\tag{1.5.6}
$$

We can also derive the dynamics of the exchange rate $X ^ { B | A } ( t )$ itself under $\mathbb { P } ^ { A }$ . Note that $X ^ { B | A } ( t ) ~ =$ $D ^ { B } ( t ) V ( t ) = e ^ { - r _ { B } t } V ( t )$ . Using the product rule on this relationship with the dynamics (1.5.6): 

$$
d X ^ {B | A} (t) = d \left(e ^ {- r _ {B} t} V (t)\right)\tag{1.5.7}
$$

$$
= e ^ {- r _ {B} t} d V (t) + V (t) d (e ^ {- r _ {B} t}) + d (e ^ {- r _ {B} t}) d V (t)\tag{1.5.8}
$$

$$
= e ^ {- r _ {B} t} \left[ r _ {A} V (t) d t + \sigma_ {2} V (t) (\rho d W _ {1} ^ {A} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A}) \right] + V (t) [ - r _ {B} e ^ {- r _ {B} t} d t ] + 0\tag{1.5.9}
$$

$$
= (r _ {A} - r _ {B}) e ^ {- r _ {B} t} V (t) d t + \sigma_ {2} e ^ {- r _ {B} t} V (t) (\rho d W _ {1} ^ {A} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A} (t))\tag{1.5.10}
$$

$$
= (r _ {A} - r _ {B}) X ^ {B | A} (t) d t + \sigma_ {2} X ^ {B | A} (t) (\rho d W _ {1} ^ {A} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A} (t)).\tag{1.5.11}
$$

This is a crucial result: under the domestic risk-neutral measure $\mathbb { P } ^ { A }$ , the expected rate of change of the exchange rate $X ^ { B | A } ( t )$ (price of foreign currency in domestic units) is the diference between the domestic and foreign risk-free interest rates, $r _ { A } - r _ { B }$ . This relationship, often called the interest rate parity condition in a risk-neutral world, holds generally beyond this specific constant-coeficient model. 

## 1.5.2 Foreign risk-neutral measure

The dynamics of the exchange rate $X ^ { B | A } ( t )$ under the domestic risk-neutral measure $\mathbb { P } ^ { A }$ were found to be: 

$$
d X ^ {B | A} (t) = \left(r _ {A} - r _ {B}\right) X ^ {B | A} (t) d t + \sigma_ {2} X ^ {B | A} (t) \left(\rho d W _ {1} ^ {A} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A} (t)\right).
$$

The drift $r _ { A } - r _ { B }$ might seem counterintuitive initially, as $X ^ { B | A } ( t )$ is not a traded asset price denominated in currency A whose discounted value must be a $\mathbb { P } ^ { A }$ -martingale. The explanation lies in viewing the investment in the foreign money market account $M ^ { B } ( t )$ from the domestic perspective. The value in currency $A$ is $V ( t ) = M ^ { B } ( t ) X ^ { B | A } ( t )$ . An investor holding this position earns the domestic risk-free rate $r _ { A }$ on the value $V ( t )$ (as it’s a traded asset under $\mathbb { P } ^ { A } )$ but also implicitly receives the foreign interest $r _ { B }$ on the underlying quantity $M ^ { B } ( t )$ held in the foreign currency. This foreign interest acts like a continuous dividend stream paid at rate $r _ { B }$ on the asset $V ( t )$ . For the discounted value $D ^ { A } ( t ) V ( t )$ to be a martingale under $\mathbb { P } ^ { A }$ , the drift of $V ( t )$ must be $r _ { A } V ( t ) d t$ . However, the drift of the underlying exchange rate $X ^ { B | \overset { \smile } { A } } ( t )$ must adjust to account for the “dividend” $r _ { B }$ . If $X ^ { B | A } ( t )$ had drift $r _ { A } X ^ { B | A } ( t ) d t$ , then $V ( t )$ would have drift $( r _ { A } + r _ { B } ) V ( t ) d t .$ To achieve the required drift of $r _ { A } V ( t ) d t$ for $V ( t )$ , the drift of $X ^ { B | A } ( t )$ must be $( r _ { A } - r _ { B } ) X ^ { B | A } ( t ) d t$ . This ensures consistency: 

$$
\begin{array}{r l} & {d V (t) = d (M ^ {B} X ^ {B | A}) = M ^ {B} d X ^ {B | A} + X ^ {B | A} d M ^ {B}} \\ & {\qquad = M ^ {B} [ (r _ {A} - r _ {B}) X ^ {B | A} d t + \ldots d W ^ {A} ] + X ^ {B | A} [ r _ {B} M ^ {B} d t ]} \\ & {\qquad = (r _ {A} - r _ {B} + r _ {B}) M ^ {B} X ^ {B | A} d t + \ldots d W ^ {A} = r _ {A} V (t) d t + \ldots d W ^ {A}.} \end{array}
$$

Let’s consider pricing a European call option on the exchange rate with strike K and maturity $T ,$ paying $( X ^ { B | A } ( T ) - K ) ^ { + }$ in currency A. The price at time t under $\bar { \mathbb { P } ^ { A } }$ is: 

$$
\begin{array}{c} C (t, x) = \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ D ^ {A} (T) / D ^ {A} (t) (X ^ {B | A} (T) - K) ^ {+}   \Big |   X ^ {B | A} (t) = x \right] \\ = \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ e ^ {- r _ {A} (T - t)} (X ^ {B | A} (T) - K) ^ {+}   \Big |   X ^ {B | A} (t) = x \right]. \end{array}
$$

This expectation involves the process $X ^ { B | A } ( t )$ which has drift $r _ { A } - r _ { B }$ under $\mathbb { P } ^ { A }$ . This structure is analogous to pricing an option on a stock paying a continuous dividend yield equal to $r _ { B }$ . We can use a change of numeraire technique or directly adapt the Black-Scholes formula. Let’s adjust the discounting to match the asset’s growth rate temporarily: 

$$
\begin{array}{c} C (t, x) = \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ e ^ {- (r _ {A} - r _ {B}) (T - t)} e ^ {- r _ {B} (T - t)} (X ^ {B | A} (T) - K) ^ {+}   \Big |   X ^ {B | A} (t) = x \right] \\ = e ^ {- r _ {B} (T - t)} \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ e ^ {- (r _ {A} - r _ {B}) (T - t)} (X ^ {B | A} (T) - K) ^ {+}   \Big |   X ^ {B | A} (t) = x \right]. \end{array}
$$

The remaining expectation is now in the standard Black-Scholes form for an asset with drift $r _ { A } - r _ { B }$ and volatility $\sigma _ { 2 }$ , discounted at rate $r _ { A } - r _ { B }$ . The standard Black-Scholes formula applies with the interest rate replaced by $r _ { A } - r _ { B }$ and volatility σ : 

$$
\mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ e ^ {- (r _ {A} - r _ {B}) (T - t)} (X ^ {B | A} (T) - K) ^ {+}   \Big |   X ^ {B | A} (t) = x \right] = x N (d _ {+}) - K e ^ {- (r _ {A} - r _ {B}) (T - t)} N (d _ {-}),
$$

where $N ( \cdot )$ is the standard normal CDF and 

$$
d _ {\pm} = \frac {1}{\sigma_ {2} \sqrt {T - t}} \left[ \log \left(\frac {x}{K}\right) + \left((r _ {A} - r _ {B}) \pm \frac {1}{2} \sigma_ {2} ^ {2}\right) (T - t) \right].
$$

Substituting back, we obtain the Garman-Kohlhagen formula (1983): 

$$
C (t, x) = x e ^ {- r _ {B} (T - t)} N \left(d _ {+}\right) - K e ^ {- r _ {A} (T - t)} N \left(d _ {-}\right).\tag{1.5.12}
$$

This formula is the standard for pricing European options on foreign exchange rates. 

Now, consider the perspective of an investor based in currency B (e.g., Frankfurt). They would naturally use a risk-neutral measure $\mathbb { P } ^ { B }$ under which asset prices denominated in currency $B ,$ when discounted by the foreign discount factor $D ^ { B } ( t ) = e ^ { - r _ { B } t }$ , become martingales. Under $\mathbb { P } ^ { B }$ , the expected rate of return for any traded asset denominated in currency B must be $r _ { B }$ 

We can summarize the assets and their values in diferent units in the following table. Let $Q ( t ) = X ^ { B | A } ( t )$ be the price of 1 unit of B in A. Then $1 / Q ( t ) = X ^ { A | B } ( t )$ is the price of 1 unit of A in B. 

<table><tr><td>Denominated in ↓ / Asset →</td><td>Domestic money market (MA)</td><td>Stock (S)</td><td>Foreign money market (MB)</td></tr><tr><td>Domestic currency (A)</td><td>MA(t)</td><td>S(t)</td><td>MB(t)Q(t)</td></tr><tr><td>Units of MA(Domestic numeraire)</td><td>1</td><td>DA(t)S(t)</td><td>DA(t)MB(t)Q(t)</td></tr><tr><td>Foreign currency (B)</td><td>MA(t)/Q(t)</td><td>S(t)/Q(t)</td><td>MB(t)</td></tr><tr><td>Units of MB(Foreign numeraire)</td><td>MA(t)/(Q(t)MB(t))= DB(t)MA(t)/Q(t)</td><td>S(t)/(Q(t)MB(t))= DB(t)S(t)/Q(t)</td><td>1</td></tr></table>

The processes in the second row, denominated in units of $M ^ { A }$ , are martingales under the domestic riskneutral measure $\mathbb { P } ^ { A }$ . The processes in the fourth row, denominated in units of $M ^ { B }$ , must be martingales under the foreign risk-neutral measure $\mathbb { P } ^ { B }$ 

We can find the relationship between $\mathbb { P } ^ { A }$ and $\mathbb { P } ^ { B }$ using the change of numeraire technique. The Radon-Nikodym derivative process relating the two measures is given by the ratio of the *target* numeraire (for $\mathbb { P } ^ { B } )$ to the $^ { * } { \mathrm { s o u r c e } } ^ { * }$ numeraire (for $\operatorname { \bar { \mathbb { P } } } ^ { A } )$ , both normalized by their initial values and expressed in a common currency (say, A). Numeraire for $\mathbb { P } ^ { A } \colon \ { \dot { N } } _ { A } ( t ) = M ^ { A } ( t )$ . Value in currency A is $N _ { A } ^ { A } ( t ) = M ^ { A } ( t )$ . Numeraire for $\mathbb { P } ^ { B } \colon \dot { N } _ { B } ( t ) \dot { = } M ^ { B } ( t )$ Value in currency A is $\dot { N } _ { B } ^ { A } ( t ) \ : = \ : M ^ { B } ( t ) Q ( t )$ . The Radon-Nikodym derivative process $\begin{array} { r } { Z ^ { A  B } ( t ) = \frac { d \mathbb { P } ^ { B } } { d \mathbb { P } ^ { A } } | _ { \mathcal { F } _ { t } } } \end{array}$ is given by the ratio of the normalized target numeraire to the normalized source numeraire: 

$$
Z ^ {A \rightarrow B} (t) = \frac {N _ {B} ^ {A} (t) / N _ {B} ^ {A} (0)}{N _ {A} ^ {A} (t) / N _ {A} ^ {A} (0)} = \frac {(M ^ {B} (t) Q (t)) / (M ^ {B} (0) Q (0))}{M ^ {A} (t) / M ^ {A} (0)}
$$

Assuming the standard initializations $M ^ { A } ( 0 ) = 1$ and $M ^ { B } ( 0 ) = 1$ , this simplifies to: 

$$
Z ^ {A \to B} (t) = \frac {M ^ {B} (t) Q (t) / Q (0)}{M ^ {A} (t) / 1} = \frac {M ^ {B} (t) Q (t)}{M ^ {A} (t) Q (0)}.
$$

Alternatively, using the martingale approach from the lecture: the process used to change from $\mathbb { P } ^ { A }$ to $\mathbb { P } ^ { B }$ should correspond to the numeraire portfolio for $\mathbb { P } ^ { B }$ when expressed as a $\mathbb { P } ^ { A }$ -martingale. The third entry in the second row, $D ^ { A } ( t ) M ^ { B } ( t ) Q ( t )$ , represents the value of the foreign money market account (numeraire for $\mathbb { P } ^ { B } )$ expressed in units of the domestic money market account (numeraire for $\mathbb { P } ^ { A } )$ . This process is a $\mathbb { P } ^ { A }$ -martingale. Normalizing it to start at 1 gives the Radon-Nikodym derivative process: 

$$
Z ^ {A \rightarrow B} (t) = \frac {D ^ {A} (t) M ^ {B} (t) Q (t)}{D ^ {A} (0) M ^ {B} (0) Q (0)} = \frac {D ^ {A} (t) M ^ {B} (t) Q (t)}{Q (0)}.\tag{1.5.13}
$$

The volatility vector of $Z ^ { A \to B } ( t )$ under $\mathbb { P } ^ { A }$ is the same as the volatility vector of $Q ( t ) = X ^ { B | A } ( t )$ under $\mathbb { P } ^ { A } .$ as $D ^ { A } ( t )$ and $M ^ { B } ( t )$ are deterministic. Volatility vectors are invariant under equivalent measure changes, so the volatility vector is $\vec { \sigma } _ { X } = ( \rho \sigma _ { 2 } , \sqrt { 1 - \rho ^ { 2 } } \sigma _ { 2 } )$ . The dynamics of $Z ^ { A \to B } ( t )$ under $\mathbb { P } ^ { A }$ are $d Z ^ { A \to B } ( t ) =$ $Z ^ { A \to B } ( t ) ( \vec { \sigma } _ { X } \cdot d \vec { W } ^ { A } ( t ) )$ . By Girsanov’s theorem, the Brownian motions under $\mathbb { P } ^ { B }$ , denoted $W _ { 1 } ^ { B } , W _ { 2 } ^ { B }$ , are related to those under $\operatorname { \mathbb { P } } ^ { A }$ by $d W _ { i } ^ { B } = d W _ { i } ^ { A } - ( \vec { \sigma } _ { X } ) _ { i } d t$ 

$$
d W _ {1} ^ {B} (t) = d W _ {1} ^ {A} (t) - \rho \sigma_ {2} d t\tag{1.5.14}
$$

$$
d W _ {2} ^ {B} (t) = d W _ {2} ^ {A} (t) - \sqrt {1 - \rho^ {2}} \sigma_ {2} d t\tag{1.5.15}
$$

Using these relationships, one can derive the dynamics of assets $S ( t )$ and $Q ( t )$ under the foreign risk-neutral measure $\mathbb { P } ^ { B }$ . For example, under $\mathbb { P } ^ { B }$ , the drift of $S ( t ) / Q ( t )$ (stock price in currency B) discounted by $D ^ { B } ( t )$ should be zero. 

We now examine the market from the perspective of an investor based in currency B. Their natural pricing measure is the foreign risk-neutral measure $\mathbb { P } ^ { B }$ . We derived the relationship between the Brownian motions under $\mathbb { P } ^ { A }$ and $\mathbb { P } ^ { B }$ as: 

$$
\begin{array}{r l} & d W _ {1} ^ {A} (t) = d W _ {1} ^ {B} (t) + \rho \sigma_ {2} d t \\ & d W _ {2} ^ {A} (t) = d W _ {2} ^ {B} (t) + \sqrt {1 - \rho^ {2}} \sigma_ {2} d t \end{array}
$$

(Note: these are inverted from (1.5.14), (1.5.15) to express $\mathbb { P } ^ { A _ { - } } \mathrm { B N }$ s in terms of $\mathbb { P } ^ { B } \mathrm { - B M s ) }$ . 

Let’s verify the dynamics of the inverse exchange rate, $X ^ { A | B } ( t ) = 1 / X ^ { B | A } ( t )$ , which represents the price of 1 unit of domestic currency A in terms of foreign currency B. We expect its drift under $\mathbb { P } ^ { B }$ to be $r _ { B } - r _ { A }$ We start with the dynamics of $X ^ { B | A } ( t )$ under $\bar { \mathbb { P } } ^ { A } \ ( 1 . 5 . 1 1 )$ 

$$
d X ^ {B | A} (t) = (r _ {A} - r _ {B}) X ^ {B | A} (t) d t + \sigma_ {2} X ^ {B | A} (t) (\rho d W _ {1} ^ {A} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A} (t)).
$$

Apply Itô’s lemma to $f ( x ) = 1 / x$ , where $x = X ^ { B | A } ( t )$ . We have $f ^ { \prime } ( x ) = - 1 / x ^ { 2 }$ and $f ^ { \prime \prime } ( x ) = 2 / x ^ { 3 }$ 

$$
\begin{array}{r l} & d X ^ {A | B} (t) \\ & = d (f (X ^ {B | A} (t))) = f ^ {\prime} (X ^ {B | A}) d X ^ {B | A} + \frac {1}{2} f ^ {\prime \prime} (X ^ {B | A}) (d X ^ {B | A}) ^ {2} \\ & = - \frac {1}{(X ^ {B | A}) ^ {2}} \left[ (r _ {A} - r _ {B}) X ^ {B | A} d t + \sigma_ {2} X ^ {B | A} (\rho d W _ {1} ^ {A} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A}) \right] + \frac {1}{2} \frac {2}{(X ^ {B | A}) ^ {3}} \left[ \sigma_ {2} X ^ {B | A} (\rho d W _ {1} ^ {A} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A}) \right] ^ {2} \\ & = - \frac {1}{X ^ {B | A}} (r _ {A} - r _ {B}) d t - \frac {\sigma_ {2}}{X ^ {B | A}} (\rho d W _ {1} ^ {A} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A}) + \frac {1}{(X ^ {B | A}) ^ {3}} (X ^ {B | A}) ^ {2} \sigma_ {2} ^ {2} (\rho d W _ {1} ^ {A} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A}) ^ {2} \\ & = (r _ {B} - r _ {A}) X ^ {A | B} d t - \sigma_ {2} X ^ {A | B} (\rho d W _ {1} ^ {A} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A}) + X ^ {A | B} \sigma_ {2} ^ {2} (\rho^ {2} d t + (1 - \rho^ {2}) d t + 2 \rho \sqrt {1 - \rho^ {2}} d W _ {1} ^ {A} d W _ {2} ^ {A}) \\ & = (r _ {B} - r _ {A} + \sigma_ {2} ^ {2}) X ^ {A | B} d t - \sigma_ {2} X ^ {A | B} (\rho d W _ {1} ^ {A} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {A} (t)). \end{array}
$$

This gives the dynamics of $X ^ { A | B } ( t )$ under $\mathbb { P } ^ { A }$ . Now, substitute $d W _ { 1 } ^ { A } = d W _ { 1 } ^ { B } + \rho \sigma _ { 2 } d t$ and $d W _ { 2 } ^ { A } = d W _ { 2 } ^ { B } +$ ${ \sqrt { 1 - \rho ^ { 2 } } } \sigma _ { 2 } d t$ 

$$
\begin{array}{r l} & {d X ^ {A | B} (t) = (r _ {B} - r _ {A} + \sigma_ {2} ^ {2}) X ^ {A | B} d t - \sigma_ {2} X ^ {A | B} \left[ \rho (d W _ {1} ^ {B} + \rho \sigma_ {2} d t) + \sqrt {1 - \rho^ {2}} (d W _ {2} ^ {B} + \sqrt {1 - \rho^ {2}} \sigma_ {2} d t) \right]} \\ & {\qquad = (r _ {B} - r _ {A} + \sigma_ {2} ^ {2}) X ^ {A | B} d t - \sigma_ {2} X ^ {A | B} \left[ \rho d W _ {1} ^ {B} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {B} \right] - \sigma_ {2} X ^ {A | B} \left[ \rho^ {2} \sigma_ {2} d t + (1 - \rho^ {2}) \sigma_ {2} d t \right]} \\ & {\qquad = (r _ {B} - r _ {A} + \sigma_ {2} ^ {2}) X ^ {A | B} d t - \sigma_ {2} X ^ {A | B} (\rho d W _ {1} ^ {B} + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {B}) - \sigma_ {2} ^ {2} X ^ {A | B} d t} \\ & {\qquad = (r _ {B} - r _ {A}) X ^ {A | B} d t - \sigma_ {2} X ^ {A | B} (\rho d W _ {1} ^ {B} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {B} (t)).} \end{array}
$$

Thus, under the foreign risk-neutral measure $\mathbb { P } ^ { B }$ , the dynamics are: 

$$
d X ^ {A | B} (t) = (r _ {B} - r _ {A}) X ^ {A | B} (t) d t - \sigma_ {2} X ^ {A | B} (t) (\rho d W _ {1} ^ {B} (t) + \sqrt {1 - \rho^ {2}} d W _ {2} ^ {B} (t)).\tag{1.5.16}
$$

This confirms that the expected rate of change for $X ^ { A | B } ( t )$ (price of domestic currency in foreign units) is $r _ { B } - r _ { A }$ under $\mathbb { P } ^ { B }$ . Note that the volatility structure $- \sigma _ { 2 } ( \rho , \sqrt { 1 - \rho ^ { 2 } } )$ corresponds $\mathrm { t o } - \vec { \sigma } _ { X }$ , reflecting the inverse relationship $X ^ { A | B } = 1 / X ^ { B | A }$ 

Two examples under $\mathbb { P } ^ { B } .$ : 

Example 1.5.1 (Dynamics of Domestic Asset in Foreign Currency). Let $S ^ { B } ( t ) = S ( t ) / Q ( t ) = S ( t ) X ^ { A | B } ( t )$ be the price of the domestic stock S expressed in the foreign currency B. Using the dynamics under $\mathbb { P } ^ { B }$ for $S ( t )$ (derived by changing measure in $\left( 1 . 5 . 5 \right) )$ and $X ^ { \dot { A } | B } ( t ) \ ( 1 . 5 . 1 6 )$ , and applying Itô’s product rule, one can show that $d S ^ { B } ( t ) = \bar { r _ { B } } \bar { S ^ { B } } ( t ) d t + . . . d \dot { W } ^ { B }$ , confirming it grows at the foreign risk-free rate $r _ { B }$ under $\mathbb { P } ^ { B }$ . The volatility vector calculation is simpler: ${ \vec { \sigma } } _ { S ^ { B } } = { \vec { \sigma } } _ { S } - { \vec { \sigma } } _ { Q } = ( \sigma , 0 ) - ( \rho \sigma _ { 2 } , \sqrt { 1 - \rho ^ { 2 } } \sigma _ { 2 } ) = ( \sigma - \rho \sigma _ { 2 } , - \sqrt { 1 - \rho ^ { 2 } } \sigma _ { 2 } )$ 

Example 1.5.2 (Put-call duality). Consider the price $C ( 0 )$ of the European call option paying $( X ^ { B | A } ( T ) -$ $K ) ^ { + }$ in currency A at time T. We found $C ( 0 ) = \mathbb { E } ^ { \mathbb { P } ^ { A } } [ D ^ { A } ( T ) ( X ^ { B | A } ( T ) - K ) ^ { + } ]$ . Let’s manipulate this expression using the change of measure process $\begin{array} { r } { Z ^ { A  B } ( T ) \stackrel { \cdot } { = } \frac { { \bar { D ^ { A } ( T ) M ^ { B } ( T ) } } Q ( T ) } { Q ( 0 ) } } \end{array}$ . Recall $Q ( t ) = X ^ { B | A } ( t )$ 

$$
\begin{array}{r l} & C (0) = \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ D ^ {A} (T) X ^ {B | A} (T) \left(1 - \frac {K}{X ^ {B | A} (T)}\right) ^ {+} \right] = \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ D ^ {A} (T) X ^ {B | A} (T) (1 - K X ^ {A | B} (T)) ^ {+} \right] \\ & \quad = \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ \frac {D ^ {A} (T) M ^ {B} (T) X ^ {B | A} (T)}{Q (0)} \cdot \frac {Q (0)}{M ^ {B} (T)} (1 - K X ^ {A | B} (T)) ^ {+} \right] \\ & \quad = \mathbb {E} ^ {\mathbb {P} ^ {A}} \left[ Z ^ {A \to B} (T) \cdot Q (0) D ^ {B} (T) (1 - K X ^ {A | B} (T)) ^ {+} \right] \\ & \quad = Q (0) \mathbb {E} ^ {\mathbb {P} ^ {B}} \left[ D ^ {B} (T) (1 - K X ^ {A | B} (T)) ^ {+} \right] \quad (b y B a y e s r u l e) \\ & \quad = Q (0) K \mathbb {E} ^ {\mathbb {P} ^ {B}} \left[ D ^ {B} (T) \left(\frac {1}{K} - X ^ {A | B} (T)\right) ^ {+} \right]. \end{array}
$$

The term $\mathbb { E } ^ { \mathbb { P } ^ { B } } [ D ^ { B } ( T ) ( \frac { 1 } { \kappa } - X ^ { A | B } ( T ) ) ^ { + } ]$ is the price at time $0 ,$ in currency $B ,$ of a European put option with strike $1 / K$ on the exchange rate $X ^ { A | B } ( t )$ (price of A in B). Let $P ^ { B } ( 0 , 1 / K )$ denote this price. Then, 

$$
C ^ {A} (0, K) = Q (0) K P ^ {B} (0, 1 / K).
$$

This equation relates the price of a call option on $X ^ { B | A }$ (strike K, in currency A) to the price of a put option on $X ^ { A | B }$ (strike $1 / K$ , in currency B). Specifically, the value in currency A of one call option equals the value in currency A of K put options (since $Q ( 0 )$ converts the price $P ^ { B }$ from currency B to A). This relationship is known as FX put-call duality. It holds generally beyond the constant coeficient model, relying only on the no-arbitrage relationship between the pricing measures. It is distinct from the standard put-call parity for options on the same underlying asset. 

End of Lecture 11 

## 1.6 Course summmary

## Derivative security pricing

We work in a market with one or more primary assets $S ^ { i } ( t )$ (e.g. stocks or zero-coupon bonds, paying no dividends or coupons and with no cost of carry) and a money-market account 

$$
M (t) = \exp \left(\int_ {0} ^ {t} r (u) d u\right),
$$

where $r ( t )$ is the (possibly stochastic) short rate and 

$$
d M (t) = r (t) M (t) d t.
$$

We assume the model is arbitrage-free: no trading strategy in $\{ S ^ { i } \}$ alone can generate a sure profit. 

To price a derivative security with payof H at T, we seek a self-financing strategy $\left( \Delta ^ { 1 } ( t ) , \ldots , \Delta ^ { n } ( t ) , \Gamma ( t ) \right)$ such that its portfolio value 

$$
X (t) = \sum_ {i = 1} ^ {n} \Delta^ {i} (t) S ^ {i} (t) + \Gamma (t) M (t)
$$

satisfies $X ( T ) = H$ . The self-financing condition is 

$$
d X (t) = \sum_ {i = 1} ^ {n} \Delta^ {i} (t) d S ^ {i} (t) + \Gamma (t) d M (t),
$$

and the requirement $X ( T ) = H$ uniquely determines $\{ \Delta ^ { i } , \Gamma \}$ whenever H is replicable. $\mathrm { B y }$ matching the diferentials of the discounted processes 

$$
\widetilde {X} (t) = X (t) / M (t) \quad \text { and } \quad \widetilde {c} (t) = c (t, S (t)) / M (t),
$$

one derives (i) an explicit formula for each hedge ratio $\Delta ^ { i } ( t )$ and (ii) a partial-diferential equation for $c ( t , S )$ In particular, in the classical Black-Scholes setting one recovers 

$$
\frac {\partial c}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} c}{\partial S ^ {2}} + r S \frac {\partial c}{\partial S} - r c = 0,
$$

with terminal condition $c ( T , S ) = H$ . Finally, if H is replicable then the absence of arbitrage forces 

$$
c (t, S (t)) = X (t) \quad \text { for   all } 0 \leq t \leq T.
$$

## Risk-neutral measure

Definition 1.6.1. A probability measure $\mathbb { Q }$ on $\left( \Omega , \mathcal { F } , \{ \mathcal { F } _ { t } \} \right)$ is called a risk-neutral measure (or martingale measure) $i f$ 

$$
\mathbb {Q} \sim \mathbb {P} \quad a n d \quad \widetilde {S} ^ {i} (t) = \frac {S ^ {i} (t)}{M (t)}
$$

is a $\mathbb { Q } .$ -martingale for each primary asset i. Equivalently, under $\mathbb { Q }$ the drift of every asset equals the short rate: 

$$
d S ^ {i} (t) = r (t) S ^ {i} (t) d t + (d i f f u s i o n t e r m s).
$$

## §1.6. Course summmary

## Three fundamental consequences:

1. Risk-neutral pricing formula. If a derivative with payof H at T is replicable, then 

$$
c (t, S (t)) = M (t) \mathbb {E} ^ {\mathbb {Q}} \big [ M (T) ^ {- 1} H \mid \mathcal {F} _ {t} \big ].
$$

2. First Fundamental Theorem $o f$ Asset Pricing. The market is arbitrage-free if and only if at least one risk-neutral measure $\mathbb { Q }$ exists. 

3. Incomplete markets. The market is incomplete (some payofs are not replicable) precisely when there are infinitely many risk-neutral measures. 

## Incomplete markets

An incomplete market is one in which some contingent claims cannot be hedged exactly by trading in the available primary assets. By the Second Fundamental Theorem of Asset Pricing, an arbitrage-free market is incomplete if and only if there is more than one risk-neutral measure. 

Pricing in incomplete markets: 

• Replicable claims. Some contracts (e.g. forwards, European calls in simple models) remain replicable and thus have unique no-arbitrage prices. 

• Non-replicable claims. When replication fails, practitioners typically enlarge the market (add traded instruments) or choose a particular martingale measure (e.g. the minimal martingale measure, the variance-optimal measure, or an Esscher transform) to compute 

$$
c (t) = M (t) \mathbb {E} ^ {\mathbb {Q} ^ {*}} \left[ M (T) ^ {- 1} H \mid \mathcal {F} _ {t} \right].
$$

• No arbitrage. As long as the same $\mathbb { Q } ^ { * }$ is used consistently for all derivative prices, arbitrage between primary assets and derivatives is precluded. 

## The big theorems

• Martingale Representation Theorem. Every square-integrable martingale can be written as a stochastic integral with respect to a Brownian motion. 

• Multidimensional Lévy Theorem. A continuous local martingale with quadratic covariation matrix $[ M ^ { i } , M ^ { j } ] _ { t } = \delta _ { i j } t$ is a vector of independent Brownian motions. 

• Girsanov Theorem. If θ(t) is adapted and satisfies the Novikov condition, then 

$$
Z (t) = \left. \frac {d \mathbb {Q}}{d \mathbb {P}} \right| _ {\mathcal {F} _ {t}} = \exp \left(- \int_ {0} ^ {t} \theta (s) d W (s) - \frac {1}{2} \int_ {0} ^ {t} \theta (s) ^ {2} d s\right)
$$

is a P-martingale with $\mathbb { E } ^ { \mathbb { P } } [ Z ( t ) ] = 1$ and under the measure $\mathbb { Q }$ the process 

$$
W ^ {\mathbb {Q}} (t) = W (t) + \int_ {0} ^ {t} \theta (s) d s
$$

is a Brownian motion. 

• Radon-Nikodym derivative process. The process $Z ( t ) = d \mathbb { Q } / d \mathbb { P } | _ { \mathcal { F } _ { t } }$ is an exponential martingale of mean 1. 

• Change of expectation. For any integrable X, 

$$
\mathbb {E} ^ {\mathbb {Q}} [ X ] = \mathbb {E} ^ {\mathbb {P}} [ Z (T) X ], \quad \mathbb {E} ^ {\mathbb {Q}} [ X \mid \mathcal {G} ] = \frac {\mathbb {E} ^ {\mathbb {P}} [ Z (t) X \mid \mathcal {G} ]}{\mathbb {E} ^ {\mathbb {P}} [ Z (t) \mid \mathcal {G} ]} \quad (\text { Bayes' rule }).
$$

• Fundamental Theorems of Asset Pricing. 

1. First FTAP: No-arbitrage ⇐⇒ existence of a risk-neutral measure. 

2. Second FTAP: Market completeness ⇐⇒ uniqueness of the risk-neutral measure. 

## Markov processes

Definition 1.6.2. A one-dimensional process X(t) is Markov if for all $s \leq t ,$ 

$$
\mathbb {P} \left(X (t) \in A \mid \mathcal {F} _ {s}\right) = \mathbb {P} \left(X (t) \in A \mid X (s)\right).
$$

Equivalently, in its $S D E d X ( t ) = \mu \left( t , X ( t ) \right) d t + \sigma \left( t , X ( t ) \right) d W ( t )$ the coeficients depend only on t and $X ( t )$ 

Definition 1.6.3. A two-dimensional process $( X ( t ) , Y ( t ) )$ is Markov if its joint SDE 

$$
\begin{array}{l} {d X (t) = a (t, X (t), Y (t)) d t + b (t, X (t), Y (t)) d W ^ {1} (t),} \\ {d Y (t) = c (t, X (t), Y (t)) d t + d (t, X (t), Y (t)) d W ^ {2} (t)} \end{array}
$$

has coeficients depending only on $( t , X ( t ) , Y ( t ) )$ and the driving Brownian motions. 

Examples 

• Local-volatility model: 

$$
d S (t) = r S (t) d t + \sigma (t, S (t)) d \widetilde {W} (t).
$$

• Stochastic-volatility (Heston): 

$$
\left\{ \begin{array}{l} d S (t) = \sqrt {V (t)} S (t) d \widetilde {W} _ {1} (t), \\ d V (t) = \kappa (\lambda - V (t)) d t + \sigma \sqrt {V (t)} \left(\rho d \widetilde {W} _ {1} (t) + \sqrt {1 - \rho^ {2}} d \widetilde {W} _ {2} (t)\right). \end{array} \right.
$$

• Non-Markov example: 

$$
d Y (t) = S (t) d t,
$$

since the drift depends on $S ( t )$ not on $Y ( t )$ alone. 

## Conditional expectations and Markov property

If X is Markov then for any measurable $h ,$ 

$$
\widetilde {\mathbb {E}} \left[ h (X (T)) | \mathcal {F} _ {t} \right] = g (t, X (t)), \quad g (t, x) = \widetilde {\mathbb {E}} \left[ h (X (T)) | X (t) = x \right].
$$

The function $g$ satisfies a backward Kolmogorov PDE found by the four-step scheme. In particular, under constant rate $r ,$ 

$$
e ^ {- r t} c (t, x) = \widetilde {\mathbb {E}} \left[ e ^ {- r T} h (X (T)) \mid X (t) = x \right].
$$

For a two-dimensional Markov pair (S, Y ) one has 

$$
e ^ {- r t} c (t, x, y) = \widetilde {\mathbb {E}} \left[ \left(\frac {1}{T} Y (T) - K\right) ^ {+} \Bigg | S (t) = x, Y (t) = y \right].
$$

## Some common processes

Consider the linear SDE 

$$
d X (u) = Y (u) X (u) d W (u).
$$

By Itô’s formula, 

$$
d \log X (u) = Y (u) d W (u) - \frac {1}{2} Y (u) ^ {2} d u,
$$

so that 

$$
X (T) = X (t) \exp \left[ \int_ {t} ^ {T} Y (u) d W (u) - \frac {1}{2} \int_ {t} ^ {T} Y (u) ^ {2} d u \right].
$$

If Y is deterministic, then X is Markov and one can write down its log-normal transition density explicitly. 

## §1.6. Course summmary

The Black-Scholes asset price satisfies 

$$
d S (u) = r S (u) d u + \sigma S (u) d \widetilde {W} (u),
$$

and similarly 

$$
S (T) = S (t) \exp \left[ \sigma \left(\widetilde {W} (T) - \widetilde {W} (t)\right) + \left(r - \frac {1}{2} \sigma^ {2}\right) (T - t) \right].
$$

The Ho-Lee short-rate model is 

$$
d R (u) = \alpha (u) d u + \sigma d \widetilde {W} (u),
$$

so that 

$$
R (T) = R (t) + \int_ {t} ^ {T} \alpha (u) d u + \sigma \left(\widetilde {W} (T) - \widetilde {W} (t)\right).
$$

The Hull-White model satisfies 

$$
d R (u) = \kappa (\theta (u) - R (u)) d u + \sigma d \widetilde {W} (u).
$$

Multiplying by $e ^ { \kappa u }$ and integrating gives 

$$
R (T) = e ^ {- \kappa T} \left[ e ^ {\kappa t} R (t) + \kappa \int_ {t} ^ {T} e ^ {\kappa u} \theta (u) d u + \sigma \int_ {t} ^ {T} e ^ {\kappa u} d \widetilde {W} (u) \right].
$$

In each case, the Itô integral of a deterministic integrand is Gaussian. 

## Kolmogorov equations

The transition density of a Markov difusion X is 

$$
p (t, x; T, y) = \frac {\partial}{\partial y} \mathbb {P} [ X (T) \leq y \mid X (t) = x ].
$$

If 

$$
d X (u) = \beta (u, X (u)) d u + \gamma (u, X (u)) d W (u),
$$

then $p$ satisfies the backward and forward Kolmogorov equations: 

$$
\frac {\partial}{\partial t} p + \beta (t, x) \frac {\partial p}{\partial x} + \frac {1}{2} \gamma (t, x) ^ {2} \frac {\partial^ {2} p}{\partial x ^ {2}} = 0,
$$

$$
\frac {\partial}{\partial T} p + \frac {\partial}{\partial y} \left[ \beta (T, y) p \right] - \frac {1}{2} \frac {\partial^ {2}}{\partial y ^ {2}} \left[ \gamma (T, y) ^ {2} p \right] = 0.
$$

(Note that the roles of $( t , x )$ and $( T , y )$ swap between the two PDEs.) 

## Dupire’s formula

Under a local-volatility model 

$$
d S (u) = r S (u) d u + \sigma \left(u, S (u)\right) S (u) d \widetilde {W} (u),
$$

the time-0 price of a European call is 

$$
c (0, S (0); T, K) = \widetilde {\mathbb {E}} \left[ e ^ {- r T} (S (T) - K) ^ {+} \right] = e ^ {- r T} \int_ {K} ^ {\infty} (y - K) \widetilde {p} (0, S (0); T, y) d y,
$$

where $\widetilde { p }$ is the risk-neutral density of S(T). Diferentiation yields 

$$
\widetilde {\mathbb {P}} \{S (T) \geq K \} = - e ^ {r T} c _ {K} (0, S (0); T, K), \quad \widetilde {p} (0, S (0); T, K) = e ^ {r T} c _ {K K} (0, S (0); T, K).
$$

Substituting into the forward equation leads to Dupire’s formula for the local volatility: 

$$
\sigma^ {2} (T, K) = \frac {2 \left(c _ {T} (0 , S (0) ; T , K) + r K c _ {K} (0 , S (0) ; T , K)\right)}{K ^ {2} c _ {K K} (0 , S (0) ; T , K)}.
$$

## Arbitrage-free term structure models

One-factor short-rate models 

Let the short rate satisfy 

$$
d R (u) = \beta (u, R (u)) d u + \gamma (u, R (u)) d \widetilde {W} (u).
$$

The zero-coupon bond price is 

$$
B (t, T) = \widetilde {\mathbb {E}} \left[ \exp \left(- \int_ {t} ^ {T} R (u) d u\right) \Bigg | \mathcal {F} _ {t} \right] = g (t, R (t)).
$$

By the four-step procedure, g satisfies the PDE 

$$
r g (t, x) = g _ {t} (t, x) + \beta (t, x) g _ {x} (t, x) + \frac {1}{2} \gamma (t, x) ^ {2} g _ {x x} (t, x).
$$

Two-factor short-rate models 

Suppose 

$$
\begin{array}{l} d X _ {1} (u) = \beta_ {1} \left(u, X _ {1} (u), X _ {2} (u)\right) d u + \gamma_ {1, 1} \left(u, X _ {1} (u), X _ {2} (u)\right) d \widetilde {W} _ {1} (u) + \gamma_ {1, 2} \left(u, X _ {1} (u), X _ {2} (u)\right) d \widetilde {W} _ {2} (u), \\ d X _ {2} (u) = \beta_ {2} \left(u, X _ {1} (u), X _ {2} (u)\right) d u + \gamma_ {2, 1} \left(u, X _ {1} (u), X _ {2} (u)\right) d \widetilde {W} _ {1} (u) + \gamma_ {2, 2} \left(u, X _ {1} (u), X _ {2} (u)\right) d \widetilde {W} _ {2} (u), \end{array}
$$

and set $R ( u ) = X _ { 1 } ( u ) + X _ { 2 } ( u )$ . Then $B ( t , T ) = g \left( t , X _ { 1 } ( t ) , X _ { 2 } ( t ) \right)$ solves the PDE obtained by replacing r with $x _ { 1 } + x _ { 2 }$ in the one-factor equation and including mixed second derivatives $\partial _ { x _ { 1 } x _ { 2 } } g .$ 

## Afine yield short-rate models

Guess the bond price in the one-factor case is of the form 

$$
g (t, r) = \exp \left(- C (t, T) r - A (t, T)\right).
$$

Compute 

$$
g _ {t}, \quad g _ {r}, \quad g _ {r r},
$$

substitute into the PDE, and collect the terms multiplying r and those free of $r .$ This yields a system of ordinary diferential equations for $C ( t , T )$ and $A ( t , T )$ . 

In the two-factor case, guess 

$$
g \left(t, x _ {1}, x _ {2}\right) = \exp \left(- C _ {1} (t, T) x _ {1} - C _ {2} (t, T) x _ {2} - A (t, T)\right),
$$

compute the six partial derivatives $g _ { t } , g _ { x _ { i } } , g _ { x _ { i } x _ { j } } ,$ substitute into the PDE, and separate the coeficients of x , x , and the constant term. One obtains ODEs for $C _ { 1 } , C _ { 2 }$ , and A. 

## Matching the initial yield curve

The model-implied discount function at $t = 0$ is 

$$
B ^ {\mathrm{Model}} (0, T) = \exp \left(- C (0, T) R (0) - A (0, T)\right), \quad 0 \leq T \leq \bar {T},
$$

while the observed market discount function is 

$$
B ^ {\mathrm{Market}} (0, T) = \exp \left(- T Y (0, T)\right).
$$

Equate exponents: 

$$
C (0, T) R (0) + A (0, T) = T Y (0, T).
$$

The right-hand side $T Y ( 0 , T )$ is known from market data; the left-hand side depends on the model’s deterministic input (e.g. α(u) or $\theta ( u ) )$ . Diferentiate both sides with respect to $T$ to solve for the unknown function $( \mathrm { e . g . ~ } \alpha ( T ) \ \mathrm { o r ~ } \theta ( T ) )$ . Once α(·) is determined, it is known for all u. 

## §1.6. Course summmary

## Forward prices

For $0 \leq t \leq T$ the forward price For(t, T) for delivery of $S ( T )$ at $T$ is defined by 

$$
\frac {1}{D (t)} \widetilde {\mathbb {E}} \left[ D (T) \left(S (T) - \mathrm{For} (t, T)\right) \mid \mathcal {F} _ {t} \right] = 0.
$$

If $D ( t ) S ( t )$ is a $\widetilde { \mathbb { P } } _ { - }$ -martingale then 

$$
\operatorname{For} (t, T) = \frac {S (t)}{B (t , T)} = \frac {D (t) S (t)}{D (t) B (t , T)},
$$

and since $\mathrm { F o r } ( t , T )$ is the ratio of two martingales it is itself a martingale under the forward measure $\mathbb { P } ^ { T }$ defined by 

$$
\left. \frac {d \mathbb {P} ^ {T}}{d \widetilde {\mathbb {P}}} \right| _ {\mathcal {F} _ {t}} = \frac {D (t) B (t , T)}{B (0 , T)}.
$$

## Black’s formula

Let $S ( t )$ be an asset whose discounted price $D ( t ) S ( t )$ is a $\widetilde { \mathbb { P } } _ { - }$ martingale, and let $\mathrm { F o r } ( t , T )$ be its forward price. Under $\mathrm { ~ } \operatorname { \mathbb { P } } ^ { T }$ , For(t, T) is a martingale. If $\mathrm { F o r } ( t , T )$ has constant volatility $\sigma ,$ then 

$$
d \mathrm{For} (t, T) = \sigma \mathrm{For} (t, T) d W ^ {T} (t).
$$

The time-t price of a call with strike K and payof $S ( T )$ at $T$ is 

$$
\begin{array}{r l} & {\frac {1}{D (t)} \widetilde {\mathbb {E}} \left[ D (T) (S (T) - K) ^ {+} \mid \mathcal {F} _ {t} \right] = B (t, T) \mathbb {E} ^ {T} \left[ (\mathrm{For} (T, T) - K) ^ {+} \mid \mathcal {F} _ {t} \right]} \\ & {\qquad = S (t) N \left(d _ {+} (t)\right) - B (t, T) K N \left(d _ {-} (t)\right),} \end{array}
$$

where 

$$
d _ {\pm} (t) = \frac {1}{\sigma \sqrt {T - t}} \left[ \ln \frac {\mathrm{For} (t , T)}{K} \pm \frac {1}{2} \sigma^ {2} (T - t) \right].
$$

## (Instantaneous) forward interest rate

The time-t price of a contract paying $R ( T )$ at $T$ is 

$$
S (t) = \widetilde {\mathbb {E}} \left[ e ^ {- \int_ {t} ^ {T} R (u) d u} R (T) \mid \mathcal {F} _ {t} \right] = - \frac {\partial}{\partial T} \widetilde {\mathbb {E}} \left[ e ^ {- \int_ {t} ^ {T} R (u) d u} \mid \mathcal {F} _ {t} \right] = - \frac {\partial}{\partial T} B (t, T).
$$

Define the instantaneous forward rate 

$$
f (t, T) = \frac {S (t)}{B (t , T)} = - \frac {\partial}{\partial T} \ln B (t, T).
$$

Writing $f ( t , u ) = - \partial _ { u } \ln B ( t , u )$ and integrating from $u = t$ to $u = T$ gives 

$$
B (t, T) = \exp \left(- \int_ {t} ^ {T} f (t, u) d u\right).
$$

## Heath-Jarrow-Morton framework

Assume the instantaneous forward rate satisfies 

$$
d f (t, T) = \alpha (t, T) d t + \sigma (t, T) d W (t),
$$

and define 

$$
\sigma^ {*} (t, T) = \int_ {t} ^ {T} \sigma (t, u) d u.
$$

A risk-neutral measure exists if and only if 

$$
\theta (t, T) = \frac {\alpha (t , T) - \sigma^ {*} (t , T) \sigma (t , T)}{\sigma (t , T)}
$$

is independent of T. In that case set 

$$
\theta (t) = \theta (t, T), \quad \widetilde {W} (t) = W (t) + \int_ {0} ^ {t} \theta (u) d u.
$$

Then under the risk-neutral measure 

$$
d f (t, T) = \sigma^ {*} (t, T) \sigma (t, T) d t + \sigma (t, T) d \widetilde {W} (t),
$$

and one shows 

$$
d \left(D (t) B (t, T)\right) = - \sigma^ {*} (t, T) D (t) B (t, T) d \widetilde {W} (t).
$$

## SOFR and forward SOFR

The overnight SOFR fixed at $T _ { j + 1 }$ over $[ T _ { j } , T _ { j + 1 } ]$ is 

$$
S \left(T _ {j + 1}; T _ {j}, T _ {j + 1}\right) = \frac {1}{\tau} \left(e ^ {\int_ {T _ {j}} ^ {T _ {j + 1}} R (u) d u} - 1\right), \quad \tau = T _ {j + 1} - T _ {j}.
$$

The forward SOFR observed at $t \leq T _ { j + 1 }$ is 

$$
\mathrm{For} _ {S} \left(t; T _ {j}, T _ {j + 1}\right) = \left\{ \begin{array}{l l} \frac {B (t , T _ {j})}{\tau B (t , T _ {j + 1})} - \frac {1}{\tau}, & 0 \leq t \leq T _ {j}, \\ \frac {D (T _ {j})}{\tau D (t) B (t , T _ {j + 1})} - \frac {1}{\tau}, & T _ {j} \leq t \leq T _ {j + 1}. \end{array} \right.
$$

Forward SOFR lets one lock in the overnight rate in advance by going long a SOFR-forward and borrowing at $T _ { j }$ at rate $S ( T _ { j + 1 } ; T _ { j } , T _ { j + 1 } )$ 

## Futures prices

The futures price for delivery of S(T) at T is 

$$
\operatorname{Fut} (t, T) = \widetilde {\mathbb {E}} \left[ S (T) \mid \mathcal {F} _ {t} \right], \quad 0 \leq t \leq T,
$$

and satisfies $\mathrm { F u t } ( T , T ) = S ( T )$ . A futures contract has zero initial price; if one trades futures with position $\Delta ( t )$ , self-financing in the money-market, then 

$$
\begin{array}{c} {d X (t) = \Delta (t) d \mathrm{Fut} (t, T) + R (t) X (t) d t,} \\ {d \left(D (t) X (t)\right) = D (t) \Delta (t) d \mathrm{Fut} (t, T).} \end{array}
$$

## Forward-futures spread

Assume $D ( t ) S ( t )$ is a $\widetilde { \mathbb { P } } _ { - }$ -martingale. Then at $t = 0$ 

$$
\begin{array}{r l} \mathrm{For} (0, T) - \mathrm{Fut} (0, T) & = \frac {S (0)}{B (0 , T)} - \widetilde {\mathbb {E}} \left[ S (T) \right] = \frac {1}{B (0 , T)} \left(\widetilde {\mathbb {E}} \left[ D (T) S (T) \right] - B (0, T) \widetilde {\mathbb {E}} \left[ S (T) \right]\right) \\ & = \frac {1}{B (0 , T)} \left(\widetilde {\mathbb {E}} \left[ D (T) S (T) \right] - \widetilde {\mathbb {E}} \left[ D (T) \right] \widetilde {\mathbb {E}} \left[ S (T) \right]\right) \\ & = \frac {1}{B (0 , T)} \mathrm{Cov} _ {\widetilde {\mathbb {P}}} \left(D (T), S (T)\right). \end{array}
$$

## §1.6. Course summmary

## Self-financing trading

Let $S _ { 1 } ( t )$ and $S _ { 2 } ( t )$ be two asset price processes. A trading strategy holds $\Delta ( t )$ shares of $S _ { 1 }$ and $\Gamma ( t )$ shares of $S _ { 2 }$ at time $t ,$ and no other assets. The portfolio value is 

$$
X (t) = \Delta (t) S _ {1} (t) + \Gamma (t) S _ {2} (t).
$$

The strategy is self-financing if 

$$
d X (t) = \Delta (t) d S _ {1} (t) + \Gamma (t) d S _ {2} (t).
$$

By Itô’s product rule applied to $X = \Delta S _ { 1 } + \Gamma S _ { 2 }$ , one obtains the financing condition 

$$
S _ {1} (t) d \Delta (t) + d S _ {1} (t) d \Delta (t) + S _ {2} (t) d \Gamma (t) + d S _ {2} (t) d \Gamma (t) = 0.
$$

## Funding using the money-market account

Introduce the money-market account 

$$
M (t) = \exp \left(\int_ {0} ^ {t} R (u) d u\right), \quad d M (t) = R (t) M (t) d t.
$$

A portfolio holding $\Delta ( t )$ shares of $S$ and cash $\mathrm { C a s h } ( t ) = X ( t ) - \Delta ( t ) S ( t )$ has value 

$$
X (t) = \Delta (t) S (t) + \mathrm{Cash} (t) = \Delta (t) S (t) + \Gamma (t) M (t).
$$

Self-financing with funding at the short rate $R ( t )$ means 

$$
d X (t) = \Delta (t) d S (t) + R (t) \left(X (t) - \Delta (t) S (t)\right) d t = \Delta (t) d S (t) + \Gamma (t) d M (t),
$$

since 

$$
R (t) \Gamma (t) M (t) d t = \Gamma (t) d M (t).
$$

## Black’s formula

The time-t price of a European call with strike K and maturity $T$ is 

$$
C (t) = N \left(d _ {+} (t)\right) S (t) - K N \left(d _ {-} (t)\right) B (t, T),
$$

where 

$$
d _ {\pm} (t) = \frac {1}{\sigma \sqrt {T - t}} \left[ \ln \frac {\mathrm{For} (t , T)}{K} \pm \frac {1}{2} \sigma^ {2} (T - t) \right].
$$

A detailed Itô-calculation shows 

$$
d C (t) = N \left(d _ {+} (t)\right) d S (t) - K N \left(d _ {-} (t)\right) d B (t, T),
$$

but this derivation is not required. 

## Trading-floor derivation of Black-Scholes

Form the portfolio that is long one call and short $\Delta ( t ) = c _ { x } \left( t , S ( t ) \right)$ shares of stock. Its value is 

$$
Y (t) = c \left(t, S (t)\right) - \Delta (t) S (t).
$$

First method: apply Itô to c: 

$$
d Y (t) = \left[ c _ {t} + \frac {1}{2} \sigma^ {2} S ^ {2} c _ {x x} \right] d t + c _ {x} d S - \Delta d S = \left[ c _ {t} + \frac {1}{2} \sigma^ {2} S ^ {2} c _ {x x} \right] d t.
$$

Second method: since the portfolio is instantaneously riskless, 

$$
d Y (t) = r Y (t) d t = r \left(c - S c _ {x}\right) d t.
$$

Equating coeficients of dt gives the Black-Scholes PDE: 

$$
c _ {t} (t, S) + \frac {1}{2} \sigma^ {2} S ^ {2} c _ {x x} (t, S) = r c (t, S) - r S c _ {x} (t, S).
$$

To summarize, we set up the portfolio that is long one call and short $\Delta ( t ) = c _ { X } ( t , S ( t ) )$ shares of stock. When time passes, there are two efects: 

1. Portfolio value changes due to underlying stock movement. 

2. Portfolio value changes due to rebalancing. 

3. If the trading is self-financing, the second efect is not present. 

4. The trading floor derivation portfolio $Y ( t )$ is not self financing because it does not account for the position in cash. 

Including the cash position and accounting for rebalancinng results in the same correction to both methods of computing $d Y$ 

## Funding considerations

Traders encounter several funding requirements in collateralized transactions: 

• (Posting cash collateral) When a trader is required to post cash collateral, interest accrues on the amount posted. 

• (Receiving cash Collateral) Conversely, when a counterparty posts cash collateral with the trader, the trader pays interest on that collateral. 

• (Futures margin accounts) Trading futures mandates margin deposits, which earn interest. 

• (Repo financing) A trader may borrow at the repo rate—typically below the federal funds rate—by pledging assets as collateral. 

• (Rate discrepancies) Each of these funding rates (collateral interest, repo rate, margin rate) may difer, afecting total funding costs. 

Remark. In modeling the portfolio value X(t), one must: 

1. Include gains or losses from asset price changes, $d S ( t ) \times$ holdings. 

2. Track all cash positions, including posted and received collateral, margin, and repo financing. 

3. Account for interest income and expense on each cash component. 

4. Discount both X(t) and any derivative price $c ( t , x )$ by the appropriate discount factors to derive the governing PDE for $c ( t , x )$ 

5. Identify a pricing measure under which the discounted derivative price is a martingale, yielding an expectation representation analogous to Black-Scholes. 

## Quotients of martingales

Let $M ( t )$ and $N ( t )$ be positive martingales under a probability measure P. In general, the ratio $M ( t ) / N ( t )$ is not a martingale under P, but becomes one after a change of measure: 

1. Define the Radon-Nikodym derivative process $L ( t ) = N ( t ) / N ( 0 )$ . Then L has expectation 1. 

2. Change to the measure $\mathbb { Q }$ via $d \mathbb { Q } / d \mathbb { P } | _ { \mathcal { F } _ { t } } = L ( t )$ . Under Q, $M ( t ) / N ( t )$ is a martingale. 

3. The volatility vector of $M / N$ is the diference of the volatility vectors of M and N. 

4. The new Brownian motions satisfy 

$$
W _ {i} ^ {\mathbb {Q}} (t) = W _ {i} ^ {\mathbb {P}} (t) - \int_ {0} ^ {t} \theta_ {i} (u) d u,
$$

where θ is the volatility vector of N. 

5. The volatility scalar of a process is the Euclidean norm of its volatility vector. 

## §1.6. Course summmary

## Foreign exchange options

Under the domestic (currency A) measure $\mathbb { P } ^ { A }$ , the spot exchange rate $X ^ { B | A } ( t )$ satisfies 

$$
d X ^ {B | A} (t) = X ^ {B | A} (t) \left[ (R ^ {A} - R ^ {B}) d t + \sum_ {i = 1} ^ {d} \nu_ {i} d W _ {i} ^ {A} (t) \right],
$$

where $\boldsymbol { \nu } = ( \nu _ { 1 } , \dots , \nu _ { d } )$ is the volatility vector and $\begin{array} { r } { \| \boldsymbol { \nu } \| = \sqrt { \sum _ { i } \nu _ { i } ^ { 2 } } } \end{array}$ . If rates and volatilities are constant, the price of a European call with strike K and maturity T is given by the Garman-Kohlhagen formula: 

$$
C (0) = e ^ {- r ^ {B} T} \left(X ^ {B | A} (0) N (d _ {+}) - e ^ {- (r ^ {A} - r ^ {B}) T} K N (d _ {-})\right),
$$

where 

$$
d _ {\pm} = \frac {\ln \left(X ^ {B | A} (0) / K\right) + (r ^ {A} - r ^ {B} \pm \frac {1}{2} \| \nu \| ^ {2}) T}{\| \nu \| \sqrt {T}}.
$$

## Changing currency of a risky asset

Let $S ^ { A } ( t )$ be the price of an asset in currency A and $X ^ { B | A } ( t )$ the exchange rate from A to B. Then the price in currency B is 

$$
S ^ {B} (t) = \frac {S ^ {A} (t)}{X ^ {B | A} (t)}.
$$

Using discounted martingale ratios, one shows under the currency-B measure that 

$$
d S ^ {B} (t) = S ^ {B} (t) \left[ R ^ {B} d t + \sum_ {i = 1} ^ {d} (\sigma_ {i} - \nu_ {i}) d W _ {i} ^ {B} (t) \right],
$$

where 

$$
W _ {i} ^ {B} (t) = W _ {i} ^ {A} (t) - \int_ {0} ^ {t} \nu_ {i} (u) d u.
$$

End of Lecture 12 

## Bibliography



[BBPL12] Damiano Brigo, Cristin Buescu, Andrea Pallavicini, and Qing Liu. Illustrating a problem in the self-financing condition in two 2010-2011 papers on funding, collateral and discounting. arXiv preprint arXiv:1207.2316, 2012. doi:10.48550/arXiv.1207.2316. 



[Pit10] Vladimir Piterbarg. Funding beyond discounting: Collateral agreements and derivatives pricing. Risk Magazine, pages 97–102, 01 2010. 

[Shr] Steven E. Shreve. Lecture notes on fixed income models. Unpublished manuscript. 

[Shr04] Steven E. Shreve. Stochastic Calculus for Finance II: Continuous-Time Models. Springer, New York, NY; Heidelberg, 2004. URL: https://link.springer.com/book/9780387401010. 