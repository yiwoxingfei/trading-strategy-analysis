

<!-- === Source: MinerU_markdown_Optimization_Methods_in_Finance_1_2122706526345998353.md (Page 1) === -->

# Optimization Methods in Finance

Gerard Cornuejols Reha Tut¨ unc¨ u¨ Carnegie Mellon University, Pittsburgh, PA 15213 USA 

January 2006 

## Foreword

Optimization models play an increasingly important role in financial decisions. Many computational finance problems ranging from asset allocation to risk management, from option pricing to model calibration can be solved eficiently using modern optimization techniques. This course discusses several classes of optimization problems (including linear, quadratic, integer, dynamic, stochastic, conic, and robust programming) encountered in financial models. For each problem class, after introducing the relevant theory (optimality conditions, duality, etc.) and eficient solution methods, we discuss several problems of mathematical finance that can be modeled within this problem class. In addition to classical and well-known models such as Markowitz’ mean-variance optimization model we present some newer optimization models for a variety of financial problems. 

## Acknowledgements

This book has its origins in courses taught at Carnegie Mellon University in the Masters program in Computational Finance and in the MBA program at the Tepper School of Business (G´erard Cornu´ejols), and at the Tokyo Institute of Technology, Japan, and the University of Coimbra, Portugal (Reha Tut¨ unc¨ u).¨ We thank the attendants of these courses for their feedback and for many stimulating discussions. We would also like to thank the colleagues who provided the initial impetus for this project, especially Michael Trick, John Hooker, Sanjay Srivastava, Rick Green, Yanjun Li, Lu´ıs Vicente and Masakazu Kojima. Various drafts of this book were experimented with in class by Javier Pena,˜ Fran¸cois Margot, Miroslav Karamanov and Kathie Cameron, and we thank them for their comments. 

## Contents

1 Introduction 9
1.1 Optimization Problems . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
1.1.1 Linear Programming . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
1.1.2 Quadratic Programming . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
1.1.3 Conic Optimization . . . . . . . . . . . . . . . . 11
1.1.4 Integer Programming 12
1.1.5 Dynamic Programming 13
1.2 Optimization with Data Uncertainty 13
1.2.1 Stochastic Programming 13
1.2.2 Robust Optimization 14
1.3 Financial Mathematics 15
1.3.1 Portfolio Selection and Asset Allocation 16
1.3.2 Pricing and Hedging of Options 18
1.3.3 Risk Management 19
1.3.4 Asset/Liability Management 20
2 Linear Programming: Theory and Algorithms 21
2.1 The Linear Programming Problem 21
2.2 Duality 23
2.3 Optimality Conditions 26
2.4 The Simplex Method 29
2.4.1 Basic Solutions 30
2.4.2 Simplex Iterations 33
2.4.3 The Tableau Form of the Simplex Method 37
2.4.4 Graphical Interpretation 40
2.4.5 The Dual Simplex Method 41
2.4.6 Alternatives to the Simplex Method 43
3 LP Models: Asset/Liability Cash Flow Matching 45
3.1 Short Term Financing 45
3.1.1 Modeling 46
3.1.2 Solving the Model with SOLVER 48
3.1.3 Interpreting the output of SOLVER 51
3.1.4 Modeling Languages 52
3.1.5 Features of Linear Programs 53
3.2 Dedication 54
3.3 Sensitivity Analysis for Linear Programming 56 

3.3.1 Short Term Financing 56
3.3.2 Dedication 61
3.4 Case Study 64

4 LP Models: Asset Pricing and Arbitrage 67
4.1 The Fundamental Theorem of Asset Pricing 67
4.1.1 Replication 69
4.1.2 Risk-Neutral Probabilities 70
4.1.3 The Fundamental Theorem of Asset Pricing 72
4.2 Arbitrage Detection Using Linear Programming 73
4.3 Additional Exercises 76
4.4 Case Study: Tax Clientele Effects in Bond Portfolio Management 80

5 Nonlinear Programming: Theory and Algorithms 83
5.1 Introduction 83
5.2 Software 85
5.3 Univariate Optimization 86
5.3.1 Binary search 86
5.3.2 Newton's Method 90
5.3.3 Approximate Line Search 93
5.4 Unconstrained Optimization 95
5.4.1 Steepest Descent 95
5.4.2 Newton's Method 99
5.5 Constrained Optimization 102
5.5.1 The generalized reduced gradient method 105
5.5.2 Sequential Quadratic Programming 110
5.6 Nonsmooth Optimization: Subgradient Methods 111

6 NLP Models: Volatility Estimation 113
6.1 Volatility Estimation with GARCH Models 113
6.2 Estimating a Volatility Surface 117

7 Quadratic Programming: Theory and Algorithms 123
7.1 The Quadratic Programming Problem 123
7.2 Optimality Conditions 124
7.3 Interior-Point Methods 126
7.4 The Central Path 129
7.5 Interior-Point Methods 130
7.5.1 Path-Following Algorithms 130
7.5.2 Centered Newton directions 131
7.5.3 Neighborhoods of the Central Path 133
7.5.4 A Long-Step Path-Following Algorithm 136
7.5.5 Starting from an Infeasible Point 136
7.6 QP software 137
7.7 Additional Exercises 137 

8 QP Models: Portfolio Optimization 139
8.1 Mean-Variance Optimization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
8.1.1 Example . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 141
8.1.2 Large-Scale Portfolio Optimization . . . . . . . . . . . . . . . . . . . . . 146
8.1.3 The Black-Litterman Model .. 149
8.1.4 Mean-Absolute Deviation to Estimate Risk .. 153
8.2 Maximizing the Sharpe Ratio .. 155
8.3 Returns-Based Style Analysis .. 158
8.4 Recovering Risk-Neural Probabilities from Options Prices .. 160
8.5 Additional Exercises .. 164
8.6 Case Study .. 166
9 Conic Optimization Tools 169
9.1 Introduction .. 169
9.2 Second-order cone programming: .. 169
9.2.1 Ellipsoidal Uncertainty for Linear Constraints .. 171
9.2.2 Conversion of quadratic constraints into second-order
cone constraints .. 173
9.3 Semidefinite programming: .. 174
9.3.1 Ellipsoidal Uncertainty for Quadratic Constraints .. 176
9.4 Algorithms and Software .. 177
10 Conic Optimization Models in Finance 179
10.1 Tracking Error and Volatility Constraints .. 179
10.2 Approximating Covariance Matrices .. 182
10.3 Recovering Risk-Neural Probabilities from Options Prices .. 185
10.4 Arbitrage Bounds for Forward Start Options .. 187
10.4.1 A Semi-Static Hedge .. 188
11 Integer Programming: Theory and Algorithms 193
11.1 Introduction .. 193
11.2 Modeling Logical Conditions .. 194
11.3 Solving Mixed Integer Linear Programs .. 197
11.3.1 Linear Programming Relaxation .. 197
11.3.2 Branch and Bound .. 198
11.3.3 Cutting Planes .. 206
11.3.4 Branch and Cut .. 210
12 IP Models: Constructing an Index Fund 213
12.1 Combinatorial Auctions .. 213
12.2 The Lockbox Problem .. 214
12.3 Constructing an Index Fund .. 217
12.3.1 A Large-Scale Deterministic Model .. 218
12.3.2 A Linear Programming Model .. 221
12.4 Portfolio Optimization with Minimum Transaction Levels .. 222
12.5 Exercises .. 223
12.6 Case Study .. 224 

13 Dynamic Programming Methods 225
13.1 Introduction ..... 225
13.1.1 Backward Recursion ..... 228
13.1.2 Forward Recursion ..... 231
13.2 Abstraction of the Dynamic Programming Approach ..... 232
13.3 The Knapsack Problem. ..... 235
13.3.1 Dynamic Programming Formulation ..... 235
13.3.2 An Alternative Formulation ..... 236
13.4 Stochastic Dynamic Programming ..... 237

14 DP Models: Option Pricing 239
14.1 A Model for American Options ..... 239
14.2 Binomial Lattice ..... 241
14.2.1 Specifying the parameters ..... 242
14.2.2 Option Pricing ..... 243

15 DP Models: Structuring Asset Backed Securities 247
15.1 Data ..... 249
15.2 Enumerating possible tranches ..... 251
15.3 A Dynamic Programming Approach ..... 252
15.4 Case Study ..... 253

16 Stochastic Programming: Theory and Algorithms 255
16.1 Introduction ..... 255
16.2 Two Stage Problems with Recourse ..... 256
16.3 Multi Stage Problems ..... 258
16.4 Decomposition ..... 260
16.5 Scenario Generation ..... 263
16.5.1 Autoregressive model ..... 263
16.5.2 Constructing scenario trees ..... 265

17 SP Models: Value-at-Risk 271
17.1 Risk Measures ..... 271
17.2 Minimizing CVaR ..... 274
17.3 Example: Bond Portfolio Optimization ..... 276

18 SP Models: Asset/Liability Management 279
18.1 Asset/Liability Management ..... 279
18.1.1 Corporate Debt Management ..... 282
18.2 Synthetic Options ..... 285
18.3 Case Study: Option Pricing with Transaction Costs ..... 288
18.3.1 The Standard Problem ..... 289
18.3.2 Transaction Costs ..... 290

19 Robust Optimization: Theory and Tools 293
19.1 Introduction to Robust Optimization ..... 293
19.2 Uncertainty Sets ..... 294
19.3 Different Flavors of Robustness ..... 296 

19.3.1 Constraint Robustness . . . . . . . . . . . . . . . . . . . . 296   
19.3.2 Objective Robustness . . . . . . . . . . . . . . . . . . . 297   
19.3.3 Relative Robustness . . . . . . . . . . . . . . . . . . 299   
19.3.4 Adjustable Robust Optimization . . . . . . . . . . . . . 301   
19.4 Tools and Strategies for Robust Optimization . . . . . . . . 302   
19.4.1 Sampling . . . . . . . . . . . . . . . 303   
19.4.2 Conic Optimization . . . . . . . . . 303   
19.4.3 Saddle-Point Characterizations . . . . . 305   
20 Robust Optimization Models in Finance 307   
20.1 Robust Multi-Period Portfolio Selection 307   
20.2 Robust Profit Opportunities in Risky Portfolios 311   
20.3 Robust Portfolio Selection 313   
20.4 Relative Robustness in Portfolio Selection 315   
20.5 Moment Bounds for Option Prices 317   
20.6 Additional Exercises 318   
A Convexity 321   
B Cones 323   
C A Probability Primer 325   
D The Revised Simplex Method 329 

## Chapter 1

## Introduction

Optimization is a branch of applied mathematics that derives its importance both from the wide variety of its applications and from the availability of eficient algorithms. Mathematically, it refers to the minimization (or maximization) of a given objective function of several decision variables that satisfy functional constraints. A typical optimization model addresses the allocation of scarce resources among possible alternative uses in order to maximize an objective function such as total profit. 

Decision variables, the objective function, and constraints are three essential elements of any optimization problem. Problems that lack constraints are called unconstrained optimization problems, while others are often referred to as constrained optimization problems. Problems with no objective functions are called feasibility problems. Some problems may have multiple objective functions. These problems are often addressed by reducing them to a single-objective optimization problem or a sequence of such problems. 

If the decision variables in an optimization problem are restricted to integers, or to a discrete set of possibilities, we have an integer or discrete optimization problem. If there are no such restrictions on the variables, the problem is a continuous optimization problem. Of course, some problems may have a mixture of discrete and continuous variables. We continue with a list of problem classes that we will encounter in this book. 

## 1.1 Optimization Problems

We start with a generic description of an optimization problem. Given a function $f ( x ) : I R ^ { n }  I R$ and a set $S \subset \mathbb { R } ^ { n }$ , the problem of finding an $x ^ { * } \in \mathbb { R } ^ { n }$ that solves 

$$
\begin{array}{l l} \min _ {x} & f (x) \\ \mathrm{s.t.} & x \in S \end{array}\tag{1.1}
$$

is called an optimization problem (OP). We refer to f as the objective function and to S as the feasible region. If S is empty, the problem is called infeasible. If it is possible to find a sequence $x ^ { k } \in S$ such that $f ( x ^ { k } ) \longrightarrow - \infty$ as $k  + \infty$ , then the problem is unbounded. If the problem is neither infeasible nor unbounded, then it is often possible to find a solution $x ^ { * } \in S$ 

that satisfies 

$$
f (x ^ {*}) \leq f (x), \forall x \in S.
$$

Such an $x ^ { * }$ is called a global minimizer of the problem (OP). If 

$$
f (x ^ {*}) <   f (x), \forall x \in S, x \neq x ^ {*},
$$

then $x ^ { * }$ is a strict global minimizer. In other instances, we may only find an $x ^ { * } \in S$ that satisfies 

$$
f (x ^ {*}) \leq f (x), \forall x \in S \cap B _ {x ^ {*}} (\varepsilon)
$$

for some $\varepsilon > 0$ , where $B _ { x ^ { * } } ( \varepsilon )$ is the open ball with radius $\varepsilon$ centered at $x ^ { * }$ , i.e., 

$$
B _ {x ^ {*}} (\varepsilon) = \{x: \| x - x ^ {*} \| <   \varepsilon \}.
$$

Such an $x ^ { * }$ is called a local minimizer of the problem (OP). A strict local minimizer is defined similarly. 

In most cases, the feasible set $S$ is described explicitly using functional constraints (equalities and inequalities). For example, S may be given as 

$$
S := \{x: g _ {i} (x) = 0, i \in \mathcal {E} \text {and} g _ {i} (x) \geq 0, i \in \mathcal {I} \},
$$

where $\mathcal { E }$ and $\mathcal { T }$ are the index sets for equality and inequality constraints. Then, our generic optimization problem takes the following form: 

<sup>(</sup>OP<sup>)</sup> 

$$
\begin{array}{r c l} \min _ {x} & f (x) \\ & g _ {i} (x) = 0, i \in \mathcal {E} \\ & g _ {i} (x) \geq 0, i \in \mathcal {I}. \end{array}\tag{1.2}
$$

Many factors afect whether optimization problems can be solved eficiently. For example, the number n of decision variables, and the total number of constraints $| \mathcal { E } | + | \mathcal { T } |$ , are generally good predictors of how dificult it will be to solve a given optimization problem. Other factors are related to the properties of the functions $f$ and $g _ { i }$ that define the problem. Problems with a linear objective function and linear constraints are easier, as are problems with convex objective functions and convex feasible sets. For this reason, instead of general purpose optimization algorithms, researchers have developed diferent algorithms for problems with special characteristics. We list the main types of optimization problems we will encounter. A more complete list can be found, for example, on the Optimization Tree available from http://www-fp.mcs.anl.gov/otc/Guide/OptWeb/. 

## 1.1.1 Linear Programming

One of the most common and easiest optimization problems is linear optimization or linear programming (LP). It is the problem of optimizing a linear objective function subject to linear equality and inequality constraints. This corresponds to the case in $\mathcal { O P }$ where the functions $f$ and $g _ { i }$ are all linear. If either $f$ or one of the functions $g _ { i }$ is not linear, then the resulting problem is a nonlinear programming (NLP) problem. 

## 1.1. OPTIMIZATION PROBLEMS

The standard form of the LP is given below: 

$$
\begin{array}{r c l} (\mathcal {L P}) & \min _ {x} & c ^ {T} x \\ & A x & = b \\ & x & \geq 0, \end{array}\tag{1.3}
$$

where $A \in I R ^ { m \times n } , b \in I R ^ { m } , c \in I R ^ { n }$ are given, and $x \in \mathbb { R } ^ { n }$ is the variable vector to be determined. In this book, a k-vector is also viewed as a $k \times 1$ matrix. For an $m \times n$ matrix $M ,$ the notation $M ^ { T }$ denotes the transpose matrix, namely the $n \times m$ matrix with entries $M _ { i j } ^ { T } = M _ { j i }$ . As an example, in the above formulation $c ^ { T }$ is a $1 \times n$ matrix and $c ^ { T } x$ is the $1 \times 1$ matrix with entry $\scriptstyle \sum _ { j = 1 } ^ { n } c _ { j } x _ { j }$ . The objective in (1.3) is to minimize the linear function $\textstyle \sum _ { j = 1 } ^ { n } c _ { j } { x _ { j } }$ 

As with , the problem $\mathcal { L } \mathcal { P }$ is said to be feasible if its constraints are consistent and it is called unbounded if there exists a sequence of feasible vectors $\{ x ^ { k } \}$ such that $c ^ { T } x ^ { k } \to - \infty$ . When $\mathcal { L } \mathcal { P }$ is feasible but not unbounded it has an optimal solution, i.e., a vector x that satisfies the constraints and minimizes the objective value among all feasible vectors. 

The best known (and most successful) methods for solving LPs are the interior-point and simplex methods. 

## 1.1.2 Quadratic Programming

A more general optimization problem is the quadratic optimization or the quadratic programming (QP) problem, where the objective function is now a quadratic function of the variables. The standard form $\mathrm { Q P }$ is defined as follows: 

<sup>(</sup>QP<sup>)</sup> 

$$
\begin{array}{r l r} \min _ {x} & \frac {1}{2} x ^ {T} Q x + c ^ {T} x \\ A x & = & b \\ x & \geq & 0, \end{array}\tag{1.4}
$$

where $A \in I R ^ { m \times n } , b \in I R ^ { m } , c \in I R ^ { n } , Q \in I R ^ { n \times n }$ are given, and $x \in \mathbb { R } ^ { n }$ Since $\begin{array} { r } { x ^ { T } Q x = \frac { 1 } { 2 } x ^ { T } ( Q + Q ^ { T } ) x . } \end{array}$ , one can assume without loss of generality that Q is symmetric, i.e. $Q _ { i j } = Q _ { j i }$ 

The objective function of the problem is a convex function of x when Q is a positive semidefinite matrix, i.e., when $y ^ { T } Q y \ge 0$ for all y (see the Appendix for a discussion on convex functions). This condition is equivalent to Q having only nonnegative eigenvalues. When this condition is satisfied, the QP problem is a convex optimization problem and can be solved in polynomial time using interior-point methods. Here we are referring to a classical notion used to measure computational complexity. Polynomial time algorithms are eficient in the sense that they always find an optimal solution in an amount of time that is guaranteed to be at most a polynomial function of the input size. 

## 1.1.3 Conic Optimization

Another generalization of (LP) is obtained when the nonnegativity constraints $x \ge 0$ are replaced by general conic inclusion constraints. This is called a conic optimization (CO) problem. For this purpose, we consider a closed convex cone C (see the Appendix for a brief discussion on cones) in a finite-dimensional vector space X and the following conic optimization problem: 

<sup>(</sup>CO<sup>)</sup> 

$$
\begin{array}{r c l} \min _ {x} & c ^ {T} x \\ & A x & = b \\ & x & \in C. \end{array}\tag{1.5}
$$

When $X = \mathbb { R } ^ { n }$ and $C = \textstyle { \mathbb { R } _ { + } ^ { n } }$ this problem is the standard form LP. However, much more general nonlinear optimization problems can also be formulated in this way. Furthermore, some of the most eficient and robust algorithmic machinery developed for linear optimization problems can be modified to solve these general optimization problems. Two important subclasses of conic optimization problems we will address are: (i) second-order cone optimization, and (ii) semidefinite optimization. These correspond to the cases when C is the second-order cone: 

$$
C _ {q} := \{x = (x _ {1}, x _ {2}, \ldots , x _ {n}) \in \mathbb {R} ^ {n}: x _ {1} ^ {2} \geq x _ {2} ^ {2} + \ldots + x _ {n} ^ {2}, x _ {1} \geq 0 \},
$$

and the cone of symmetric positive semidefinite matrices: 

$$
C _ {s} := \left\{X = \left[ \begin{array}{c c c} x _ {1 1} & \dots & x _ {1 n} \\ \vdots & \ddots & \vdots \\ x _ {n 1} & \dots & x _ {n n} \end{array} \right] \in \mathbb {R} ^ {n \times n}: X = X ^ {T}, X \text {is positive semidefinite} \right\}
$$

When we work with the cone of positive semidefinite matrices, the standard inner products used in $c ^ { T } x$ and Ax in (1.5) are replaced by an appropriate inner product for the space of n-dimensional square matrices. 

## 1.1.4 Integer Programming

Integer programs are optimization problems that require some or all of the variables to take integer values. This restriction on the variables often makes the problems very hard to solve. Therefore we will focus on integer linear programs, which have a linear objective function and linear constraints. A pure integer linear program is given by: 

<sup>(</sup>ILP<sup>)</sup> 

$$
\begin{array}{r c l} \min _ {x} & c ^ {T} x \\ & A x & \geq b \\ & x & \geq 0 \text { and integral, } \end{array}\tag{1.6}
$$

where $A \in I R ^ { m \times n } , b \in I R ^ { m } , c \in I R ^ { n }$ are given, and $x \in \mathbb { N } ^ { n }$ is the variable vector to be determined. 

An important case occurs when the variables $x _ { j }$ represent binary decision variables, that is $x \in \{ 0 , 1 \} ^ { n }$ . The problem is then called a 0–1 linear program. 

When there are both continuous variables and integer constrained variables, the problem is called a mixed integer linear program: 

<sup>(</sup>MILP<sup>)</sup> 

$$
\begin{array}{r l} \min _ {x} & c ^ {T} x \\ & A x \geq b \\ & x \geq 0 \\ & x _ {j} \in I N \text {for} j = 1, \ldots , p. \end{array}\tag{1.7}
$$

where $A , b ,$ c are given data and the integer $p \ ( { \mathrm { w i t h } } \ 1 \leq p < n )$ is also part of the input. 

## 1.1.5 Dynamic Programming

Dynamic programming refers to a computational method involving recurrence relations. This technique was developed by Richard Bellman in the early 1950’s. It arose from studying programming problems in which changes over time were important, thus the name “dynamic programming”. However, the technique can also be applied when time is not a relevant factor in the problem. The idea is to divide the problem into “stages” in order to perform the optimization recursively. It is possible to incorporate stochastic elements into the recursion. 

## 1.2 Optimization with Data Uncertainty

In all the problem classes we discussed so far (except dynamic programming), we made the implicit assumption that the data of the problem, namely the parameters such as Q, A, b and c in QP, are all known. This is not always the case. Often, the problem parameters correspond to quantities that will only be realized in the future, or cannot be known exactly at the time the problem must be formulated and solved. Such situations are especially common in models involving financial quantities such as returns on investments, risks, etc. We will discuss two fundamentally diferent approaches that address optimization with data uncertainty. Stochastic programming is an approach used when the data uncertainty is random and can be explained by some probability distribution. Robust optimization is used when one wants a solution that behaves well in all possible realizations of the uncertain data. These two alternative approaches are not problem classes (as in LP, QP, etc.) but rather modeling techniques for addressing data uncertainty. 

## 1.2.1 Stochastic Programming

The term stochastic programming refers to an optimization problem in which some problem data are random. The underlying optimization problem might be a linear program, an integer program, or a nonlinear program. An important case is that of stochastic linear programs. 

A stochastic program with recourse arises when some of the decisions (recourse actions) can be taken after the outcomes of some (or all) random events have become known. For example, a two-stage stochastic linear program with recourse can be written as follows: 

$$
\begin{array}{r c l r c l} \max _ {x} & a ^ {T} x & + & E [ \max _ {y (\omega)} c (\omega) ^ {T} y (\omega) ] & \\ & A x & & & = & b \\ & B (\omega) x & + & C (\omega) y (\omega) & = & d (\omega) \\ & x \geq 0, & & y (\omega) \geq 0, \end{array}\tag{1.8}
$$

where the first-stage decisions are represented by vector x and the secondstage decisions by vector $y ( \omega )$ , which depend on the realization of a random event ω. A and b define deterministic constraints on the first-stage decisions $x ,$ whereas $B ( \omega ) , C ( \omega )$ , and $d ( \omega )$ define stochastic linear constraints linking the recourse decisions $y ( \omega )$ to the first-stage decisions. The objective function contains a deterministic term $a ^ { T } x$ and the expectation of the second-stage objective $c ( \omega ) ^ { T } y ( \omega )$ taken over all realization of the random event ω. 

Note that, once the first-stage decisions x have been made and the random event ω has been realized, one can compute the optimal second-stage decisions by solving the following linear program: 

$$
\begin{array}{r l r} {f (x, \omega) = \max} & {c (\omega) ^ {T} y (\omega)} \\ & {C (\omega) y (\omega)} & {=} & {d (\omega) - B (\omega) x} \\ & {y (\omega) \geq 0,} \end{array}\tag{1.9}
$$

Let $f ( x ) = E [ f ( x , \omega ) ]$ denote the expected value of the optimal value of this problem. Then, the two-stage stochastic linear program becomes 

$$
\begin{array}{r c l} \max & a ^ {T} x + f (x) \\ & A x & = b \\ & x & \geq 0, \end{array}\tag{1.10}
$$

Thus, if the (possibly nonlinear) function $f ( x )$ is known, the problem reduces to a nonlinear programming problem. When the data $c ( \omega ) , B ( \omega )$ 2 $C ( \omega )$ , and $d ( \omega )$ are described by finite distributions, one can show that $f$ is piecewise linear and concave. When the data are described by probability densities that are absolutely continuous and have finite second moments, one can show that $f$ is diferentiable and concave. In both cases, we have a convex optimization problem with linear constraints for which specialized algorithms are available. 

## 1.2.2 Robust Optimization

Robust optimization refers to the modeling of optimization problems with data uncertainty to obtain a solution that is guaranteed to be “good” for all possible realizations of the uncertain parameters. In this sense, this approach departs from the randomness assumption used in stochastic optimization for uncertain parameters and gives the same importance to all possible realizations. Uncertainty in the parameters is described through uncertainty sets that contain all (or most) possible values that can be realized by the uncertain parameters. 

There are diferent definitions and interpretations of robustness and the resulting models difer accordingly. One important concept is constraint robustness, often called model robustness in the literature. This refers to solutions that remain feasible for all possible values of the uncertain inputs. This type of solution is required in several engineering applications. Here is an example adapted from Ben-Tal and Nemirovski. Consider a multiphase engineering process (a chemical distillation process, for example) and a related process optimization problem that includes balance constraints (materials entering a phase of the process cannot exceed what is used in that phase plus what is left over for the next phase). The quantities of the end products of a particular phase may depend on external, uncontrollable factors and are therefore uncertain. However, no matter what the values of these uncontrollable factors are, the balance constraints must be satisfied. Therefore, the solution must be constraint robust with respect to the uncertainties of the problem. Here is a mathematical model for finding constraint robust solutions: Consider an optimization problem of the form: 

$$
\begin{array}{r l r} (\mathcal {O P} _ {u c}) & \qquad \min _ {x} \quad f (x) \\ & \qquad \qquad G (x, p) \in K. \end{array}\tag{1.11}
$$

Here, x are the decision variables, $f$ is the (certain) objective function, $G$ and $K$ are the structural elements of the constraints that are assumed to be certain and $p$ are the uncertain parameters of the problem. Consider an uncertainty set $\boldsymbol { \mathcal { U } }$ that contains all possible values of the uncertain parameters $p .$ Then, a constraint robust optimal solution can be found by solving the following problem: 

<sup>(</sup>CROP<sup>)</sup> 

$$
\begin{array}{r c l} \min _ {x} & f (x) \\ & G (x, p) & \in K, \forall p \in \mathcal {U}. \end{array}\tag{1.12}
$$

A related concept is objective robustness, which occurs when uncertain parameters appear in the objective function. This is often referred to as solution robustness in the literature. Such robust solutions must remain close to optimal for all possible realizations of the uncertain parameters. Consider an optimization problem of the form: 

$$
(\mathcal {O P} _ {u o}) \qquad \min _ {x} \begin{array}{l l} f (x, p) \\ x \in S. \end{array}\tag{1.13}
$$

Here, $S$ is the (certain) feasible set and $f$ is the objective function that depends on uncertain parameters $p .$ Assume as above that $\mathcal { U }$ is the uncertainty set that contains all possible values of the uncertain parameters $p .$ . Then, an objective robust solution is obtained by solving: 

<sup>(</sup>OROP<sup>)</sup> 

$$
\min _ {x \in S} \max _ {p \in \mathcal {U}} f (x, p).\tag{1.14}
$$

Note that objective robustness is a special case of constraint robustness. Indeed, by introducing a new variable t (to be minimized) into $O P _ { u o }$ and imposing the constraint $f ( x , p ) \leq t .$ , we get an equivalent problem to $O P _ { u o }$ The constraint robust formulation of the resulting problem is equivalent to OROP. 

Constraint robustness and objective robustness are concepts that arise in conservative decision making and are not always appropriate for optimization problems with data uncertainty. 

## 1.3 Financial Mathematics

Modern finance has become increasingly technical, requiring the use of sophisticated mathematical tools in both research and practice. Many find the roots of this trend in the portfolio selection models and methods described by Markowitz in the 1950’s and the option pricing formulas developed by Black, Scholes, and Merton in the late 1960’s. For the enormous efect these works produced on modern financial practice, Markowitz was awarded the Nobel prize in Economics in 1990, while Scholes and Merton won the Nobel prize in Economics in 1997. 

Below, we introduce topics in finance that are especially suited for mathematical analysis and involve sophisticated tools from mathematical sciences. 

## 1.3.1 Portfolio Selection and Asset Allocation

The theory of optimal selection of portfolios was developed by Harry Markowitz in the 1950’s. His work formalized the diversification principle in portfolio selection and, as mentioned above, earned him the 1990 Nobel prize for Economics. Here we give a brief description of the model and relate it to QPs. 

Consider an investor who has a certain amount of money to be invested in a number of diferent securities (stocks, bonds, etc.) with random returns. For each security $i = 1 , \ldots , n$ , estimates of its expected return $\mu _ { i }$ and variance $\sigma _ { i } ^ { 2 }$ are given. Furthermore, for any two securities i and $j ,$ their correlation coeficient $\rho _ { i j }$ is also assumed to be known. If we represent the proportion of the total funds invested in security i by $x _ { i }$ , one can compute the expected return and the variance of the resulting portfolio $x = ( x _ { 1 } , \ldots , x _ { n } )$ as follows: 

$$
E [ x ] = x _ {1} \mu_ {1} + \ldots + x _ {n} \mu_ {n} = \mu^ {T} x,
$$

and 

$$
V a r [ x ] = \sum_ {i, j} \rho_ {i j} \sigma_ {i} \sigma_ {j} x _ {i} x _ {j} = x ^ {T} Q x
$$

where $\rho _ { i i } \equiv 1 , Q _ { i j } = \rho _ { i j } \sigma _ { i } \sigma _ { j }$ , and $\boldsymbol { \mu } = \left( \mu _ { 1 } , \ldots , \mu _ { n } \right)$ 

The portfolio vector x must satisfy $\textstyle \sum _ { i } x _ { i } = 1$ and there may or may Pnot be additional feasibility constraints. A feasible portfolio x is called eficient if it has the maximal expected return among all portfolios with the same variance, or alternatively, if it has the minimum variance among all portfolios that have at least a certain expected return. The collection of eficient portfolios form the eficient frontier of the portfolio universe. 

Markowitz’ portfolio optimization problem, also called the mean-variance optimization (MVO) problem, can be formulated in three diferent but equivalent ways. One formulation results in the problem of finding a minimum variance portfolio of the securities 1 to n that yields at least a target value R of expected return. Mathematically, this formulation produces a convex quadratic programming problem: 

$$
\begin{array}{r c l} \min _ {x} & x ^ {T} Q x \\ & e ^ {T} x & = 1 \\ & \mu^ {T} x & \geq R \\ & x & \geq 0, \end{array}\tag{1.15}
$$

where e is an n-dimensional vector all of which components are equal to 1. The first constraint indicates that the proportions $x _ { i }$ should sum to 1. The second constraint indicates that the expected return is no less than the target value and, as we discussed above, the objective function corresponds to the total variance of the portfolio. Nonnegativity constraints on x<sub>i</sub> are introduced to rule out short sales (selling a security that you do not have). Note that the matrix Q is positive semidefinite since $x ^ { T } Q x$ , the variance of the portfolio, must be nonnegative for every portfolio (feasible or not) x. 

As an alternative to problem (1.15), we may choose to maximize the expected return of a portfolio while limiting the variance of its return. $\mathrm { O r } ,$ we can maximize a risk-adjusted expected return which is defined as the expected return minus a multiple of the variance. These two formulations are essentially equivalent to (1.15) as we will see in Chapter 8. 

The model (1.15) is rather versatile. For example, if short sales are permitted on some or all of the securities, then this can be incorporated into the model simply by removing the nonnegativity constraint on the corresponding variables. If regulations or investor preferences limit the amount of investment in a subset of the securities, the model can be augmented with a linear constraint to reflect such a limit. In principle, any linear constraint can be added to the model without making it significantly harder to solve. 

Asset allocation problems have the same mathematical structure as portfolio selection problems. In these problems the objective is not to choose a portfolio of stocks (or other securities) but to determine the optimal investment among a set of asset classes. Examples of asset classes are large capitalization stocks, small capitalization stocks, foreign stocks, government bonds, corporate bonds, etc. There are many mutual funds focusing on specific asset classes and one can therefore conveniently invest in these asset classes by purchasing the relevant mutual funds. After estimating the expected returns, variances, and covariances for diferent asset classes, one can formulate a QP identical to (1.15) and obtain eficient portfolios of these asset classes. 

A diferent strategy for portfolio selection is to try to mirror the movements of a broad market population using a significantly smaller number of securities. Such a portfolio is called an index fund. No efort is made to identify mispriced securities. The assumption is that the market is eficient and therefore no superior risk-adjusted returns can be achieved by stock picking strategies since the stock prices reflect all the information available in the marketplace. Whereas actively managed funds incur transaction costs which reduce their overall performance, index funds are not actively traded and incur low management fees. They are typical of a passive management strategy. How do investment companies construct index funds? There are numerous ways of doing this. One way is to solve a clustering problem where similar stocks have one representative in the index fund. This naturally leads to an integer programming formulation. 

## 1.3.2 Pricing and Hedging of Options

We first start with a description of some of the well-known financial options. A European call option is a contract with the following conditions: 

At a prescribed time in the future, known as the expiration date, the holder of the option has the right, but not the obligation to 

purchase a prescribed asset, known as the underlying, for a 

prescribed amount, known as the strike price or exercise price. 

A European put option is similar, except that it confers the right to sell the underlying asset (instead of buying it for a call option). An American option is like a European option, but it can be exercised anytime before the expiration date. 

Since the payof from an option depends on the value of the underlying security, its price is also related to the current value and expected behavior of this underlying security. To find the fair value of an option, we need to solve a pricing problem. When there is a good model for the stochastic behavior of the underlying security, the option pricing problem can be solved using sophisticated mathematical techniques. 

Option pricing problems are often solved using the following strategy. We try to determine a portfolio of assets with known prices which, if updated properly through time, will produce the same payof as the option. Since the portfolio and the option will have the same eventual payofs, we conclude that they must have the same value today (otherwise, there is arbitrage) and we can therefore obtain the price of the option. A portfolio of other assets that produces the same payof as a given financial instrument is called a replicating portfolio (or a hedge) for that instrument. Finding the right portfolio, of course, is not always easy and leads to a replication (or hedging) problem. 

Let us consider a simple example to illustrate these ideas. Let us assume that one share of stock XYZ is currently valued at $40. The price of XYZ a month from today is random. Assume that its value will either double or halve with equal probabilities. 

$$
S _ {0} = 4 0 \begin{array}{c} 8 0 = S _ {1} (u) \\ 2 0 = S _ {1} (d) \end{array}
$$

Today, we purchase a European call option to buy one share of XYZ stock for $50 a month from today. What is the fair price of this option? 

Let us assume that we can borrow or lend money with no interest between today and next month, and that we can buy or sell any amount of the XYZ stock without any commissions, etc. These are part of the “frictionless market” assumptions we will address later. Further assume that XYZ will not pay any dividends within the next month. 

To solve the option pricing problem, we consider the following hedging problem: Can we form a portfolio of the underlying stock (bought or sold) 

## 1.3. FINANCIAL MATHEMATICS

and cash (borrowed or lent) today, such that the payof from the portfolio at the expiration date of the option will match the payof of the option? Note that the option payof will be $30 if the price of the stock goes up and $0 if it goes down. Assume this portfolio has $\Delta$ shares of XYZ and $B cash. This portfolio would be worth $4 0 \Delta + \mathrm { B }$ today. Next month, payofs for this portfolio will be: 

$$
P _ {0} = 4 0 \Delta + B \begin{array}{c} 8 0 \Delta + B = P _ {1} (u) \\ 2 0 \Delta + B = P _ {1} (d) \end{array}
$$

Let us choose $\Delta$ and B such that 

$$
\begin{array}{r c l} 8 0 \Delta + B & = & 3 0 \\ 2 0 \Delta + B & = & 0, \end{array}
$$

so that the portfolio replicates the payof of the option at the expiration date. This gives $\begin{array} { r } { \Delta = \frac { 1 } { 2 } } \end{array}$ and $B = - 1 0$ , which is the hedge we were looking for. This portfolio is worth $P _ { 0 } = 4 0 \Delta + B = \mathfrak { G } 1 0$ today, therefore, the fair price of the option must also be $10. 

## 1.3.3 Risk Management

Risk is inherent in most economic activities. This is especially true of financial activities where results of decisions made today may have many possible diferent outcomes depending on future events. Since companies cannot usually insure themselves completely against risk, they have to manage it. This is a hard task even with the support of advanced mathematical techniques. Poor risk management led to several spectacular failures in the financial industry during the 1990’s (e.g., Barings Bank, Long Term Capital Management, Orange County). 

A coherent approach to risk management requires quantitative risk measures that adequately reflect the vulnerabilities of a company. Examples of risk measures include portfolio variance as in the Markowitz MVO model, the Value-at-Risk (VaR) and the expected shortfall (also known as conditional Value-at-Risk, or CVaR)). Furthermore, risk control techniques need to be developed and implemented to adapt to rapid changes in the values of these risk measures. Government regulators already mandate that financial institutions control their holdings in certain ways and place margin requirements for “risky” positions. 

Optimization problems encountered in financial risk management often take the following form. Optimize a performance measure (such as expected investment return) subject to the usual operating constraints and the constraint that a particular risk measure for the company’s financial holdings does not exceed a prescribed amount. Mathematically, we may have the following problem: 

$$
\begin{array}{r c l} \max _ {x} & \mu^ {T} x \\ & \mathrm{RM} [ x ] & \leq \gamma \\ & e ^ {T} x & = 1 \\ & x & \geq 0. \end{array}\tag{1.16}
$$

As in the Markowitz MVO model, $x _ { i }$ represent the proportion of the total funds invested in security. The objective is the expected portfolio return and $\mu$ is the expected return vector for the diferent securities. RM[x] denotes the value of a particular risk measure for portfolio x and $\gamma$ is the prescribed upper limit on this measure. Since RM[x] is generally a nonlinear function of x, (1.16) is a nonlinear programming problem. Alternatively, we can minimize the risk measure while constraining the expected return of the portfolio to achieve or exceed a given target value R. This would produce a problem very similar to (1.15). 

## 1.3.4 Asset/Liability Management

How should a financial institution manage its assets and liabilities? A static mean-variance optimizing model, such as the one we discussed for asset allocation, fails to incorporate the multiple liabilities faced by financial institutions. Furthermore, it penalizes returns both above and below the mean. A multi-period model that emphasizes the need to meet liabilities in each period for a finite (or possibly infinite) horizon is often required. Since liabilities and asset returns usually have random components, their optimal management requires tools of “Optimization under Uncertainty” and most notably, stochastic programming approaches. 

Let $L _ { t }$ be the liability of the company in period t for $t = 1 , \dots , T$ . Here, we assume that the liabilities $L _ { t }$ are random with known distributions. A typical problem to solve in asset/liability management is to determine which assets (and in what quantities) the company should hold in each period to maximize its expected wealth at the end of period T. We can further assume that the asset classes the company can choose from have random returns (again, with known distributions) denoted by $R _ { i t }$ for asset class i in period t. Since the company can make the holding decisions for each period after observing the asset returns and liabilities in the previous periods, the resulting problem can be cast as a stochastic program with recourse: 

$$
\begin{array}{r l r} \max _ {x} & E [ \sum_ {i} x _ {i, T} ] \\ & \sum_ {i} (1 + R _ {i t}) x _ {i, t - 1} - \sum_ {i} x _ {i, t} & = L _ {t}, t = 1, \ldots , T \\ & x _ {i, t} & \geq 0 \quad \forall i, t. \end{array}\tag{1.17}
$$

The objective function represents the expected total wealth at the end of the last period. The constraints indicate that the surplus left after liability $L _ { t }$ is covered will be invested as follows: $x _ { i , t }$ invested in asset class i. In this formulation, $x _ { i , 0 }$ are the fixed, and possibly nonzero initial positions in the diferent asset classes. 

# Linear Programming: Theory and Algorithms

## 2.1 The Linear Programming Problem

One of the most common and fundamental optimization problems is the linear optimization, or linear programming (LP) problem. LP is the problem of optimizing a linear objective function subject to linear equality and inequality constraints. A generic linear optimization problem has the following form: 

$$
\begin{array}{r c l} \min _ {x} & c ^ {T} x \\ & a _ {i} ^ {T} x & = b _ {i}, i \in \mathcal {E} \\ & a _ {i} ^ {T} x & \geq b _ {i}, i \in \mathcal {I}, \end{array}\tag{2.1}
$$

where  and  are the index sets for equality and inequality constraints, respectively. Linear programming is arguably the best known and the most frequently solved optimization problem. It owes its fame mostly to its great success; real world problems coming from as diverse disciplines as sociology, finance, transportation, economics, production planning, and airline crew scheduling have been formulated and successfully solved as LPs. 

For algorithmic purposes, it is often desirable to have the problems structured in a particular way. Since the development of the simplex method for LPs the following form has been a popular standard and is called the standard form LP: 

$$
\begin{array}{r c l} \min _ {x} & c ^ {T} x \\ & A x & = b \\ & x & \geq 0. \end{array}\tag{2.2}
$$

Here $A \in \mathcal { I } ^ { m \times n } , b \in \mathcal { I } ^ { n } , c \in \mathcal { I } ^ { n }$ are given, and $x \in \mathbb { R } ^ { n }$ is the variable vector to be determined as the solution of the problem. 

The standard form is not restrictive: Inequalities other than nonnegativity constraints can be rewritten as equalities after the introduction of a so-called slack or surplus variable that is restricted to be nonnegative. For 

example, 

$$
\begin{array}{r l r l r l} \min & - x _ {1} & - & x _ {2} \\ & 2 x _ {1} & + & x _ {2} & \leq & 1 2 \\ & x _ {1} & + & 2 x _ {2} & \leq & 9 \\ & x _ {1} \geq 0, & x _ {2} \geq 0 \end{array}\tag{2.3}
$$

can be rewritten as 

$$
\begin{array}{r l r l r l r l} \min & - x _ {1} & - & x _ {2} \\ & 2 x _ {1} & + & x _ {2} & + & x _ {3} & = & 1 2 \\ & x _ {1} & + & 2 x _ {2} & & + & x _ {4} & = & 9 \\ & x _ {1} \geq 0, & x _ {2} \geq 0, & x _ {3} \geq 0, & x _ {4} \geq 0. \end{array}\tag{2.4}
$$

Variables that are unrestricted in sign can be expressed as the diference of two new nonnegative variables. Maximization problems can be written as minimization problems by multiplying the objective function by a negative constant. Simple transformations are available to rewrite any given LP in the standard form above. Therefore, in the rest of our theoretical and algorithmic discussion we assume that the LP is in the standard form. 

Exercise 2.1 Write the following linear program in standard form. 

$$
\begin{array}{r l r} \min & & x _ {2} \\ & x _ {1} + x _ {2} \geq 1 \\ & x _ {1} - x _ {2} \leq 0 \\ & x _ {1}, x _ {2} \text {unrestricted in sign.} \end{array}
$$

## Answer:

After writing $x _ { i } = y _ { i } - z _ { i } , i = 1 , 2$ with $y _ { i } \geq 0$ and $z _ { i } \geq 0$ and introducing surplus variable $s _ { 1 }$ for the first constraint and slack variable $s _ { 2 }$ for the second constraint we obtain: 

min 

$$
\begin{array}{r c l r c l r c l r c l} & & & y _ {2} & - & z _ {2} \\ y _ {1} & - & z _ {1} & + & y _ {2} & - & z _ {2} & - & s _ {1} & & = 1 \\ y _ {1} & - & z _ {1} & - & y _ {2} & + & z _ {2} & & + & s _ {2} & = 0 \\ y _ {1} \geq 0, & z _ {1} \geq 0, & y _ {2} \geq 0, & z _ {2} \geq 0, & s _ {1} \geq 0, & s _ {2} \geq 0. \end{array}
$$

Exercise 2.2 Write the following linear program in standard form. 

$$
\begin{array}{l l l l l} \max & 4 x _ {1} + x _ {2} - x _ {3} \\ & x _ {1} + 3 x _ {3} & \leq 6 \\ & 3 x _ {1} + x _ {2} + 3 x _ {3} & \geq 9 \\ & x _ {1} \geq 0, x _ {2} \geq 0, x _ {3} \text {unrestricted in sign.} \end{array}
$$

Recall the following definitions from the Chapter 1: The LP (2.2) is said to be feasible if its constraints are consistent and it is called unbounded if there exists a sequence of feasible vectors $\{ x ^ { k } \}$ such that $c ^ { T } x ^ { k } \to - \infty$ When we talk about a solution (without any qualifiers) to (2.2) we mean any candidate vector $x \in \mathbb { R } ^ { n }$ . A feasible solution is one that satisfies the constraints, and an optimal solution is a vector x that satisfies the constraints and minimizes the objective value among all feasible vectors. When $\mathcal { L } \mathcal { P }$ is feasible but not unbounded it has an optimal solution. 

## Exercise 2.3

(a) Write a 2-variable linear program that is unbounded. 

(b) Write a 2-variable linear program that is infeasible. 

Exercise 2.4 Draw the feasible region of the following 2-variable linear program. 

$$
\begin{array}{r l} \max & 2 x _ {1} - x _ {2} \\ & x _ {1} + x _ {2} \geq 1 \\ & x _ {1} - x _ {2} \leq 0 \\ & 3 x _ {1} + x _ {2} \leq 6 \\ & x _ {1} \geq 0, x _ {2} \geq 0. \end{array}
$$

Determine the optimal solution to this problem by inspection. 

The most important questions we will address in this chapter are the following: How do we recognize an optimal solution and how do we find such solutions? One of the most important tools in optimization to answer these questions is the notion of a dual problem associated with the LP problem (2.2). We describe the dual problem in the next subsection. 

## 2.2 Duality

Consider the standard form LP in (2.4) above. Here are a few alternative feasible solutions: 

$$
\begin{array}{r l} (x _ {1}, x _ {2}, x _ {3}, x _ {4}) = (0, \frac {9}{2}, \frac {1 5}{2}, 0) & \text { Objective   value } = - \frac {9}{2} \\ (x _ {1}, x _ {2}, x _ {3}, x _ {4}) = (6, 0, 0, 3) & \text { Objective   value } = - 6 \\ (x _ {1}, x _ {2}, x _ {3}, x _ {4}) = (5, 2, 0, 0) & \text { Objective   value } = - 7 \end{array}
$$

Since we are minimizing, the last solution is the best among the three feasible solutions we found, but is it the optimal solution? We can make such a claim if we can, somehow, show that there is no feasible solution with a smaller objective value. 

Note that the constraints provide some bounds on the value of the objective function. For example, for any feasible solution, we must have 

$$
- x _ {1} - x _ {2} \geq - 2 x _ {1} - x _ {2} - x _ {3} = - 1 2
$$

using the first constraint of the problem. The inequality above must hold for all feasible solutions since $x _ { i } \mathrm { { ' s } }$ are all nonnegative and the coeficient of each variable on the LHS are at least as large as the coeficient of the corresponding variable on the RHS. We can do better using the second constraint: 

$$
- x _ {1} - x _ {2} \geq - x _ {1} - 2 x _ {2} - x _ {4} = - 9
$$

and even better by adding a negative third of each constraint: 

$$
\begin{array}{r c l} - x _ {1} - x _ {2} & \geq & - x _ {1} - x _ {2} - \frac {1}{3} x _ {3} - \frac {1}{3} x _ {4} \\ & = & - \frac {1}{3} (2 x _ {1} + x _ {2} + x _ {3}) - \frac {1}{3} (x _ {1} + 2 x _ {2} + x _ {4}) = - \frac {1}{3} (1 2 + 9) = - 7. \end{array}
$$

This last inequality indicates that for any feasible solution, the objective function value cannot be smaller than -7. Since we already found a feasible solution achieving this bound, we conclude that this solution, namely $( x _ { 1 } , x _ { 2 } , x _ { 3 } , x _ { 4 } ) = ( 5 , 2 , 0 , 0 )$ must be an optimal solution of the problem. 

This process illustrates the following strategy: If we find a feasible solution to the LP problem, and a bound on the optimal value of problem such that the bound and the objective value of the feasible solution coincide, then we can conclude that our feasible solution is an optimal solution. We will comment on this strategy shortly. Before that, though, we formalize our approach for finding a bound on the optimal objective value. 

Our strategy was to find a linear combination of the constraints, say with multipliers $y _ { 1 }$ and $y _ { 2 }$ for the first and second constraint respectively, such that the combined coeficient of each variable forms a lower bound on the objective coeficient of that variable. Namely, we tried to choose multipliers y<sub>1</sub> and $y _ { 2 }$ associated with constraints 1 and 2 such that 

$$
y _ {1} (2 x _ {1} + x _ {2} + x _ {3}) + y _ {2} (x _ {1} + 2 x _ {2} + x _ {4}) = (2 y _ {1} + y _ {2}) x _ {1} + (y _ {1} + 2 y _ {2}) x _ {2} + y _ {1} x _ {3} + y _ {2} x _ {4}
$$

provides a lower bound on the optimal objective value. Since $x _ { i } \mathrm { { ' s } }$ must be nonnegative, the expression above would necessarily give a lower bound if the coeficient of each $x _ { i }$ is less than or equal to the corresponding objective function coeficient, or if: 

$$
\begin{array}{r c l r c l} 2 y _ {1} & + & y _ {2} & \leq & - 1 \\ y _ {1} & + & 2 y _ {2} & \leq & - 1 \\ y _ {1} & & & \leq & 0 \\ & & y _ {2} & \leq & 0. \end{array}
$$

Note that the objective coeficients of $x _ { 3 }$ and $x _ { 4 }$ are zero. Naturally, to obtain the largest possible lower bound, we would like to find $y _ { 1 }$ and $y _ { 2 }$ that achieve the maximum combination of the right-hand-side values: 

$$
\max 1 2 y _ {1} + 9 y _ {2}.
$$

This process results in a linear programming problem that is strongly related to the LP we are solving. We want to 

$$
\begin{array}{r l r l r l} \max & 1 2 y _ {1} & + & 9 y _ {2} \\ & 2 y _ {1} & + & y _ {2} & \leq & - 1 \\ & y _ {1} & + & 2 y _ {2} & \leq & - 1 \\ & y _ {1} & & & \leq & 0 \\ & & & y _ {2} & \leq & 0. \end{array}\tag{2.5}
$$

This problem is called the dual of the original problem we considered. The original LP in (2.2) is often called the primal problem. For a generic primal LP problem in standard form (2.2) the corresponding dual problem can be written as follows: 

$$
\begin{array}{r l} \max _ {y} & b ^ {T} y \\ & A ^ {T} y \leq c, \end{array}\tag{\((\mathcal{LD})\}
$$

(2.6) 

where $y \in R ^ { m }$ . Rewriting this problem with explicit dual slacks, we obtain the standard form dual linear programming problem: 

$$
\begin{array}{r l r} (\mathcal {L D}) & \quad \max _ {y, s} & b ^ {T} y \\ & & A ^ {T} y + s = c \\ & & s \geq 0, \end{array}\tag{2.7}
$$

where $s \in \mathbb { R } ^ { n }$ 

Exercise 2.5 Consider the following LP: 

$$
\begin{array}{c c c c c c} \min & 2 x _ {1} & + & 3 x _ {2} \\ & x _ {1} & + & x _ {2} & \geq & 5 \\ & x _ {1} & & & \geq & 1 \\ & & & x _ {2} & \geq & 2. \end{array}
$$

Prove that $x ^ { * } = ( 3 , 2 )$ is the optimal solution by showing that the objective value of any feasible solution is at least 12. 

Next, we make some observations about the relationship between solutions of the primal and dual LPs. The objective value of any primal feasible solution is at least as large as the objective value of any feasible dual solution. This fact is known as the weak duality theorem: 

Theorem 2.1 (Weak Duality Theorem) Let x be any feasible solution to the primal LP (2.2) and y be any feasible solution to the dual LP (2.6). Then 

$$
c ^ {T} x \geq b ^ {T} y.
$$

Proof: 

Since $x \ge 0$ and $c - A ^ { T } y \geq 0$ , the inner product of these two vectors must be nonnegative: 

$$
(c - A ^ {T} y) ^ {T} x = c ^ {T} x - y ^ {T} A x = c ^ {T} x - y ^ {T} b \geq 0.
$$

The quantity $\boldsymbol { c } ^ { T } \boldsymbol { x } - \boldsymbol { y } ^ { T } \boldsymbol { b }$ is often called the duality gap. The following three results are immediate consequences of the weak duality theorem. 

Corollary 2.1 If the primal LP is unbounded, then the dual LP must be infeasible. 

Corollary 2.2 If the dual LP is unbounded, then the primal LP must be infeasible. 

Corollary 2.3 If x is feasible for the primal LP, y is feasible for the dual $L P ,$ and $c ^ { T } x = b ^ { T } y$ , then x must be optimal for the primal LP and y must be optimal for the dual LP. 

Exercise 2.6 Show that the dual of the linear program 

$$
\begin{array}{r c l} \min _ {x} & c ^ {T} x \\ & A x & \geq b \\ & x & \geq 0 \end{array}
$$

is the linear program 

$$
\begin{array}{r c l} \max _ {y} & b ^ {T} y \\ & A ^ {T} y & \leq c \\ & y & \geq 0. \end{array}
$$

Exercise 2.7 We say that two linear programming problems are equivalent if one can be obtained from the other by (i) multiplying the objective function by -1 and changing it from min to max, or max to min, and/or (ii) multiplying some or all constraints by -1. For example, min $\{ c ^ { T } x : \overset { \cdot } { A x } \geq \overset { \cdot } { b } \}$ and max $\left\{ - c ^ { T } x : \ - A x \leq - b \right\}$ are equivalent problems. Find a linear program which is equivalent to its own dual. 

Exercise 2.8 Give an example of a linear program such that it and its dual are both infeasible. 

Exercise 2.9 For the following pair of primal-dual problems, determine whether the listed solutions are optimal. 

$$
\begin{array}{r c c c c c} \min & 2 x _ {1} & + & 3 x _ {2} \\ & 2 x _ {1} & + & 3 x _ {2} & \leq & 3 0 \\ & x _ {1} & + & 2 x _ {2} & \geq & 1 0 \\ & x _ {1} & - & x _ {2} & \geq & 0 \\ & x _ {1}, & & x _ {2} & \geq & 0 \end{array} \qquad \begin{array}{r c c c c c} \max & - 3 0 y _ {1} & + & 1 0 y _ {2} \\ & - 2 y _ {1} & + & y _ {2} & + & y _ {3} & \leq & 2 \\ & - 3 y _ {1} & + & 2 y _ {2} & - & y _ {3} & \leq & 3 \\ & y _ {1}, & & y _ {2}, & & y _ {3} & \geq & 0. \end{array}
$$

$$
\text {(a)} x _ {1} = 1 0, x _ {2} = \frac {1 0}{3}; y _ {1} = 0, y _ {2} = 1, y _ {3} = 1.
$$

$$
\text {(b)} x _ {1} = 2 0, x _ {2} = 1 0; y _ {1} = - 1, y _ {2} = 4, y _ {3} = 0.
$$

$$
\mathrm{(c)} x _ {1} = \frac {1 0}{3}, x _ {2} = \frac {1 0}{3}; y _ {1} = 0, y _ {2} = \frac {5}{3}, y _ {3} = \frac {1}{3}.
$$

## 2.3 Optimality Conditions

Corollary 2.3 in the previous section identified a suficient condition for optimality of a primal-dual pair of feasible solutions, namely that their objective values coincide. One natural question to ask is whether this is a necessary condition. The answer is yes, as we illustrate next. 

Theorem 2.2 (Strong Duality Theorem) If the primal (dual) problem has an optimal solution $x \ ( y )$ , then the dual (primal) has an optimal solution y (x) such that $c ^ { T } x = b ^ { T } y$ 

The reader can find a proof of this result in most standard linear programming textbooks (see Chv´atal [19] for example). A consequence of the Strong Duality Theorem is that, if both the primal LP problem and the dual LP have feasible solutions then they both have optimal solutions and for any primal optimal solution x and dual optimal solution y we have that $c ^ { T } x = b ^ { T } y .$ 

## 2.3. OPTIMALITY CONDITIONS

The strong duality theorem provides us with conditions to identify optimal solutions (called optimality conditions): $x \in \mathbb { R } ^ { n }$ is an optimal solution of (2.2) if and only if 

1. x is primal feasible: $A x = b , x \geq 0$ , and there exists a $y \in \mathbb { R } ^ { m }$ such that 

2. y is dual feasible: $A ^ { T } y \leq c ,$ and 

3. there is no duality gap: $c ^ { T } x = b ^ { T } y$ 

Further analyzing the last condition above, we can obtain an alternative set of optimality conditions. Recall from the proof of the weak duality theorem that $\bar { c ^ { T } } x - b ^ { T } y = ( c - A ^ { T } y ) ^ { T } x \ge 0$ for any feasible primal-dual pair of solutions, since it is given as an inner product of two nonnegative vectors. This inner product is $0 \ ( c ^ { T } x = b ^ { T } y )$ if and only if the following statement holds: For each $i = 1 , \ldots , n$ , either $x _ { i }$ or $( c - A ^ { T } y ) _ { i } = s _ { i }$ is zero. This equivalence is easy to see. All the terms in the summation on the RHS of the following equation are nonnegative: 

$$
0 = (c - A ^ {T} y) ^ {T} x = \sum_ {i = 1} ^ {n} (c - A ^ {T} y) _ {i} x _ {i}
$$

Since the sum is zero, each term must be zero. Thus we found an alternative set of optimality conditions: $x \in \mathbb { R } ^ { n }$ is an optimal solution of (2.2) if and only if 

1. x is primal feasible: $A x = b , x \geq 0$ , and there exists a $y \in \mathbb { R } ^ { m }$ such that 

2. y is dual feasible: $s : = c - A ^ { T } y \geq 0$ , and 

3. complementary slackness: for each $i = 1 , \ldots , n$ we have $x _ { i } s _ { i } = 0$ 

Exercise 2.10 Consider the linear program 

$$
\begin{array}{r c l r c l} \min & 5 x _ {1} & + & 1 2 x _ {2} & + & 4 x _ {3} \\ & x _ {1} & + & 2 x _ {2} & + & x _ {3} = & 1 0 \\ & 2 x _ {1} & - & x _ {2} & + & 3 x _ {3} = & 8 \\ & x _ {1} \geq 0, x _ {2} \geq 0, x _ {3} \geq 0. \end{array}
$$

You are $\mathrm { g i }$ ven the information that $x _ { 2 }$ and $x _ { 3 }$ are positive in the optimal solution. Use the complementary slackness conditions to find the optimal dual solution. 

Exercise 2.11 Consider the following linear programming problem: 

$$
\begin{array}{ccccccccc} \max & 6 x _ {1} & + & 5 x _ {2} & + & 4 x _ {3} & + & 5 x _ {4} & + & 6 x _ {5} \\ & x _ {1} & + & x _ {2} & + & x _ {3} & + & x _ {4} & + & x _ {5} & \leq & 3 \\ & 5 x _ {1} & + & 4 x _ {2} & + & 3 x _ {3} & + & 2 x _ {4} & + & x _ {5} & \leq & 1 4 \\ \end{array}
$$

$$
x _ {1} \geq 0, x _ {2} \geq 0, x _ {3} \geq 0, x _ {4} \geq 0, x _ {5} \geq 0
$$

Solve this problem using the following strategy: 

a) Find the dual of the above LP. The dual has only two variables. Solve the dual by inspection after drawing a graph of the feasible set. 

b) Now using the optimal solution to the dual problem, and complementary slackness conditions, determine which primal constraints are active, and which primal variables must be zero at an optimal solution. Using this information determine the optimal solution to the primal problem. 

Exercise 2.12 Using the optimality conditions for 

$$
\begin{array}{r l r} \min _ {x} & c ^ {T} x \\ & A x = b \\ & x \geq 0, \end{array}
$$

deduce that the optimality conditions for 

$$
\begin{array}{r c l} \max _ {x} & c ^ {T} x \\ & A x & \leq b \\ & x & \geq 0 \end{array}
$$

are $A x \leq b , x \geq 0$ and there exists y such that $A ^ { T } y \geq c , y \geq 0 , c ^ { T } x = b ^ { T } y$ 

Exercise 2.13 Consider the following investment problem over $T$ years, where the objective is to maximize the value of the investments in year $T .$ . We assume a perfect capital market with the same annual lending and borrowing rate $r > 0$ each year. We also assume that exogenous investment funds $b _ { t }$ are available in year t, for $t = 1 , \dots , T$ . Let $n$ be the number of possible investments. We assume that each investment can be undertaken fractionally (between 0 and 1). Let $a _ { t j }$ denote the cash flow associated with investment $j$ in year t. Let $c _ { j }$ be the value of investment $j$ in year $T$ (including all cash flows subsequent to year T discounted at the interest rate $r )$ 

The linear program that maximizes the value of the investments in year $T$ is the following. Denote by $x _ { j }$ the fraction of investment $j$ undertaken, and let $y _ { t }$ be the amount borrowed (if negative) or lent (if positive) in year $t .$ 

$$
\begin{array}{r c l l} \max & \sum_ {j = 1} ^ {n} c _ {j} x _ {j} + y _ {T} \\ & - \sum_ {j = 1} ^ {n} a _ {1 j} x _ {j} + y _ {1} & \leq & b _ {1} \\ & - \sum_ {j = 1} ^ {n} a _ {t j} x _ {j} - (1 + r) y _ {t - 1} + y _ {t} & \leq & b _ {t} \quad \text {for t = 2,\ldots,T} \\ & 0 \leq x _ {j} & \leq & 1 \quad \text {for j = 1,\ldots,n.} \end{array}
$$

(i) Write the dual of the above linear program. 

(ii) Solve the dual linear program found in (i). [Hint: Note that some of the dual variables can be computed by backward substitution.] 

(iii) Write the complementary slackness conditions. 

(iv) Deduce that the first $T$ constraints in the primal linear program hold as equalities. 

(v) Use the complementary slackness conditions to show that the solution obtained by setting $x _ { j } ~ = ~ 1$ if $c _ { j } + \textstyle \sum _ { t = 1 } ^ { T } ( 1 + r ) ^ { T - t } a _ { t j } > 0$ , and $x _ { j } ~ = ~ 0$ otherwise, is an optimal solution. 

(vi) Conclude that the above investment problem always has an optimal solution where each investment is either undertaken completely or not at all. 

## 2.4 The Simplex Method

The best known and most successful methods for solving LPs are interiorpoint methods (IPMs) and the simplex method. We discuss the simplex method here and postpone our discussion IPMs till we study quadratic programming problems, as IPMs are also applicable to quadratic programs and other more general classes of optimization problems. 

We introduce the essential elements of the simplex method using a simple bond portfolio selection problem. 

Example 2.1 A bond portfolio manager has $100,000 to allocate to two diferent bonds; one corporate and one government bond. The corporate bond has a yield of 4%, a maturity of 3 years and an A rating from a rating agency that is translated into a numerical rating of 2 for computational purposes. In contrast, the government bond has a yield of 3%, a maturity of 4 years and rating of Aaa with the corresponding numerical rating of 1 (lower numerical ratings correspond to higher quality bonds). The portfolio manager would like to allocate her funds so that the average rating for the portfolio is no worse than Aa (numerical equivalent 1.5) and average maturity of the portfolio is at most 3.6 years. Any amount not invested in the two bonds will be kept in a cash account that is assumed to earn no interest for simplicity and does not contribute to the average rating or maturity computations<sup>1</sup>. How should the manager allocate her funds between these two bonds to achieve her objective of maximizing the yield from this investment? 

Letting variables x and x denote the allocation offunds to the corporate and government bond respectively (in thousands of dollars) we obtain the following formulation for the portfolio manager’s problem: 

$$
\max Z = 4 x _ {1} + 3 x _ {2}
$$

subject to: 

$$
\begin{array}{r l r} {x _ {1} + x _ {2}} & \leq & 1 0 0 \\ {\frac {2 x _ {1} + x _ {2}}{1 0 0}} & \leq & 1. 5 \\ {\frac {3 x _ {1} + 4 x _ {2}}{1 0 0}} & \leq & 3. 6 \\ {x _ {1}, x _ {2}} & \geq & 0. \end{array}
$$

We first multiply the second and third inequalities by 100 to avoid fractions. After we add slack variables to each of the functional inequality constraints we obtain a representation of the problem in the standard form, suitable for the simplex method<sup>2</sup>. For example, letting x<sub>3</sub> denote the amount we keep as cash, we can rewrite the first constraint as $x _ { 1 } + x _ { 2 } + x _ { 3 } = 1 0 0$ with the additional condition of x<sub>3</sub>. Continuing with this strategy we obtain the following formulation: 

max $\begin{array} { r } { Z = \begin{array} { l l l } { 4 x _ { 1 } } & { + } & { 3 x _ { 2 } } \end{array} } \end{array}$ 

subject to: 

$$
\begin{array}{r c l r c l r c l r c l} x _ {1} & + & x _ {2} & + & x _ {3} & & & & & = & 1 0 0 \\ 2 x _ {1} & + & x _ {2} & & & + & x _ {4} & & & = & 1 5 0 \\ 3 x _ {1} & + & 4 x _ {2} & & & & & + & x _ {5} & = & 3 6 0 \\ x _ {1} & , & x _ {2} & , & x _ {3} & , & x _ {4} & , & x _ {5} & \geq & 0. \end{array}\tag{2.8}
$$

## 2.4.1 Basic Solutions

Let us consider a general LP problem in the following form: 

$$
\max \mathbf {c x}\tag{2.9}
$$

$$
\mathbf {A x} \leq \mathbf {b}\tag{2.10}
$$

$$
\mathbf {x} \geq \mathbf {0},\tag{2.11}
$$

where A is an $m \times n$ matrix, b is an m-dimensional column vector and c is an n-dimensional row vector. The n-dimensional column vector x represents the variables of the problem. (In the bond portfolio example we have $m = 3$ and $n = 2 . )$ Here is how we can represent these vectors and matrices: 

$$
\mathbf {A} = \left[ \begin{array}{c c c c} a _ {1 1} & a _ {1 2} & \ldots & a _ {1 n} \\ a _ {2 1} & a _ {2 2} & \ldots & a _ {2 n} \\ \vdots & \vdots & \ddots & \vdots \\ a _ {m 1} & a _ {m 2} & \ldots & a _ {m n} \end{array} \right], \quad \mathbf {b} = \left[ \begin{array}{c} b _ {1} \\ b _ {2} \\ \vdots \\ b _ {m} \end{array} \right], \quad \mathbf {c} = \left[ \begin{array}{c c c c} c _ {1} & c _ {2} & \ldots & c _ {n} \end{array} \right],
$$

$$
\mathbf {x} = \left[ \begin{array}{c} x _ {1} \\ x _ {2} \\ \vdots \\ x _ {n} \end{array} \right], \quad \mathbf {0} = \left[ \begin{array}{c} 0 \\ 0 \\ \vdots \\ 0 \end{array} \right].
$$

Next, we add slack variables to each of the functional constraints to get the augmented form of the problem. Let $\mathbf { x } _ { s }$ denote the vector of slack variables 

$$
\mathbf {x} _ {s} = \left[ \begin{array}{c} x _ {n + 1} \\ x _ {n + 2} \\ \vdots \\ x _ {n + m} \end{array} \right]
$$

and let I denote the $m \times m$ identity matrix. Now, the constraints in the augmented form can be written as 

$$
\left[ \begin{array}{l l} \mathbf {A}, & \mathbf {I} \end{array} \right] \left[ \begin{array}{l} \mathbf {x} \\ \mathbf {x _ {s}} \end{array} \right] = \mathbf {b}, \quad \left[ \begin{array}{l} \mathbf {x} \\ \mathbf {x _ {s}} \end{array} \right] \geq \mathbf {0}.\tag{2.12}
$$

such a transformation to leave the objective function in its natural form–it should be straightforward to adapt the steps of the algorithm in the following discussion to address minimization problems. 

## 2.4. THE SIMPLEX METHOD

There are many potential solutions to system (2.12). Let us focus on the equation $\left[ \begin{array} { l l } { \mathbf { A } , } & { \mathbf { I } } \end{array} \right] \left[ \begin{array} { l } { \mathbf { x } } \\ { \mathbf { x _ { s } } } \end{array} \right] = \mathbf { b }$ . By choosing $\mathbf { x } = \mathbf { 0 }$ and $\mathbf { x _ { s } } = \mathbf { b }$ , we immediately satisfy this equation–but not necessarily all the inequalities. More generally, we can consider partitions of the augmented matrix $[ A , I ] ^ { 3 }$ 

$$
\left[ \begin{array}{l l} {\mathbf {A},} & {\mathbf {I}} \end{array} \right] \equiv \left[ \begin{array}{l l} {\mathbf {B},} & {\mathbf {N}} \end{array} \right],
$$

where B is an $m \times m$ square matrix that consists of linearly independent columns of $[ \mathbf { A } , \mathbf { I } ]$ . If we partition the variable vector $\left[ \begin{array} { l } { \mathbf { x } } \\ { \mathbf { x _ { s } } } \end{array} \right]$ in the same way 

$$
\left[ \begin{array}{c} \mathbf {x} \\ \mathbf {x _ {s}} \end{array} \right] \equiv \left[ \begin{array}{c} \mathbf {x _ {B}} \\ \mathbf {x _ {N}} \end{array} \right],
$$

we can rewrite the equality constraints in (2.12) as 

$$
\left[ \begin{array}{l} \mathbf {B}, \mathbf {N} \end{array} \right] \left[ \begin{array}{l} \mathbf {x _ {B}} \\ \mathbf {x _ {N}} \end{array} \right] = \mathbf {B x _ {B}} + \mathbf {N x _ {N}} = \mathbf {b},
$$

or by multiplying both sides by $B ^ { - 1 }$ from left, 

$$
\mathbf {x _ {B}} + \mathbf {B} ^ {- 1} \mathbf {N x _ {N}} = \mathbf {B} ^ {- 1} \mathbf {b}.
$$

By our construction, the following three systems of equations are equivalent in the sense that any solution to one is a solution for the other two: 

$$
\begin{array}{r} \left[ \begin{array}{l l} \mathbf {A}, & \mathbf {I} \end{array} \right] \left[ \begin{array}{l} \mathbf {x} \\ \mathbf {x _ {s}} \end{array} \right] = \mathbf {b}, \\ \mathbf {B x _ {B}} + \mathbf {N x _ {N}} = \mathbf {b} \\ \mathbf {x _ {B}} + \mathbf {B ^ {- 1}} \mathbf {N x _ {N}} = \mathbf {B ^ {- 1}} \mathbf {b} \end{array}
$$

Indeed, the second and third linear systems are just other representations of the first one in terms of the matrix B. As we observed above, an obvious solution to the last system (and therefore, to the other two) is $\mathbf { x } _ { \mathbf { N } } = \mathbf { 0 }$ 2 $\mathbf { x _ { B } = B ^ { - 1 } b }$ . In fact, for any fixed values of the components of x<sub>N</sub> we can obtain a solution by simply setting 

$$
\mathbf {x _ {B}} = \mathbf {B} ^ {- 1} \mathbf {b} - \mathbf {B} ^ {- 1} \mathbf {N} \mathbf {x _ {N}}.\tag{2.13}
$$

One can think of $\mathbf { x _ { N } }$ as the independent variables that we can choose freely, and once they are chosen, the dependent variables $\mathbf { x _ { B } }$ are determined uniquely. We call a solution of the systems above a basic solution if it is of the form 

$$
\mathbf {x} _ {\mathbf {N}} = \mathbf {0}, \mathbf {x} _ {\mathbf {B}} = \mathbf {B} ^ {- 1} \mathbf {b},
$$

for some basis matrix B. If in addition, $\mathbf { x _ { B } } = \mathbf { B } ^ { - 1 } \mathbf { b } \geq \mathbf { 0 }$ , the solution $\mathbf { x _ { B } } = \mathbf { B } ^ { - 1 } \mathbf { b } , \mathbf { x _ { N } } = \mathbf { 0 }$ is a basic feasible solution of the LP problem above. The variables x<sub>B</sub> are called the basic variables, while $\mathbf { x } _ { \mathbf { N } }$ are the nonbasic variables. Geometrically, basic feasible solutions correspond to extreme points of the feasible set $\{ x : A x \leq b , x \geq 0 \}$ . Extreme points of a set are those that cannot be written as a convex combination of two other points in the set. 

The objective function ${ \bf Z } = { \bf c } { \bf x }$ can be represented similarly using the basis partition. Let $\mathbf { c } = { \left| \begin{array} { l l } { \mathbf { c _ { B } } , } & { \mathbf { c _ { N } } } \end{array} \right| }$ represent the partition of the objective vector. Now, we have the following sequence of equivalent representations of the objective function equation: 

$$
\begin{array}{r} \mathbf {Z} = \texttt {c x} \Leftrightarrow \mathbf {Z} - \texttt {c x} = 0 \\ \mathbf {Z} - \left[ \begin{array}{l l} \mathbf {c} _ {\mathrm{B}}, & \mathbf {c} _ {\mathrm{N}} \end{array} \right] \left[ \begin{array}{l} \mathbf {x} _ {\mathrm{B}} \\ \mathbf {x} _ {\mathrm{N}} \end{array} \right] = 0 \\ \mathbf {Z} - \mathbf {c} _ {\mathrm{B}} \mathbf {x} _ {\mathrm{B}} - \mathbf {c} _ {\mathrm{N}} \mathbf {x} _ {\mathrm{N}} = 0 \end{array}
$$

Now substituting $\mathbf { x _ { B } } = \mathbf { B } ^ { - 1 } \mathbf { b } - \mathbf { B } ^ { - 1 } \mathbf { N } \mathbf { x _ { N } }$ from (2.13) we obtain 

$$
\mathbf {Z} - \mathbf {c} _ {\mathrm{B}} (\mathbf {B} ^ {- 1} \mathbf {b} - \mathbf {B} ^ {- 1} \mathbf {N x} _ {\mathrm{N}}) - \mathbf {c} _ {\mathrm{N}} \mathbf {x} _ {\mathrm{N}} = \mathbf {0 Z} - (\mathbf {c} _ {\mathrm{N}} - \mathbf {c} _ {\mathrm{B}} \mathbf {B} ^ {- 1} \mathbf {N}) \mathbf {x} _ {\mathrm{N}} = \mathbf {c} _ {\mathrm{B}} \mathbf {B} ^ {- 1} \mathbf {b}
$$

Note that the last equation does not contain the basic variables. This representation allows us to determine the net efect on the objective function of changing a nonbasic variable. This is an essential property used by the simplex method as we discuss in the following subsection. The vector of objective function coeficients $\mathbf { c _ { N } } - \mathbf { c _ { B } } \mathbf { B } ^ { - 1 } \mathbf { N }$ corresponding to the nonbasic variables is often called the vector of reduced costs since they contain the cost coeficients $\mathbf { c _ { N } }$ “reduced” by the cross efects of the basic variables given by $\mathbf { c _ { B } } \mathbf { B } ^ { - 1 } \mathbf { N }$ 

Exercise 2.14 Consider the following linear programming problem: 

$$
\begin{array}{r c l r c l} \max & 4 x _ {1} & + & 3 x _ {2} \\ & 3 x _ {1} & + & x _ {2} & \leq & 9 \\ & 3 x _ {1} & + & 2 x _ {2} & \leq & 1 0 \\ & x _ {1} & + & x _ {2} & \leq & 4 \\ & x _ {1} \geq 0, & x _ {2} \geq 0. \end{array}
$$

First, transform this problem into the standard form. How many basic solutions does the standard form problem have? What are the basic feasible solutions and what are the extreme points of the feasible region? 

Exercise 2.15 A plant can manufacture five products $P _ { 1 } , P _ { 2 } , P _ { 3 } , P _ { 4 }$ and $P _ { 5 }$ . The plant consists of two work areas: the job shop area $A _ { 1 }$ and the assembly area $A _ { 2 }$ . The time required to process one unit of product $P _ { j }$ in work area $A _ { i }$ is $p _ { i j }$ (in hours), for $i = 1 , 2$ and $j = 1 , \ldots , 5 .$ The weekly capacity of work area $A _ { i }$ is $C _ { i }$ (in hours). The company can sell all it produces of product $P _ { j }$ at a profit of $s _ { j }$ , for $i = 1 , \ldots , 5$ 

The plant manager thought of writing a linear program to maximize profits, but never actually did for the following reason: From past experience, he observed that the plant operates best when at most two products are manufactured at a time. He believes that if he uses linear programming, the optimal solution will consist of producing all five products and therefore it will not be of much use to him. Do you agree with him? Explain, based on your knowledge of linear programming. 

Answer: The linear program has two constraints (one for each of the work areas). Therefore, at most two variables are positive in a basic solution. In particular, this is the case for an optimal basic solution. So the plant manager is mistaken in his beliefs. There is always an optimal solution of the linear program in which at most two products are manufactured. 

## 2.4.2 Simplex Iterations

A key result of linear programming theory is that when a linear programming problem has an optimal solution, it must have an optimal solution that is an extreme point. The significance of this result lies in the fact that when we are looking for a solution of a linear programming problem we can focus on the objective value of extreme point solutions only. There are only finitely many of them, so this reduces our search space from an infinite space to a finite one. 

The simplex method solves a linear programming problem by moving from one extreme point to an adjacent extreme point. Since, as we discussed in the previous section, extreme points of the feasible set correspond to basic feasible solutions (BFSs), algebraically this is achieved by moving from one BFS to another. We describe this strategy in detail in this section. 

The process we mentioned in the previous paragraph must start from an initial BFS. How does one find such a point? While finding a basic solution is almost trivial, finding feasible basic solutions can be dificult. Fortunately, for problems of the form (2.9), such as the bond portfolio optimization problem (2.8) there is a simple strategy. Choosing 

$$
\mathbf {B} = \left[ \begin{array}{l l l} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{array} \right], \mathbf {x _ {B}} = \left[ \begin{array}{l} x _ {3} \\ x _ {4} \\ x _ {5} \end{array} \right], \mathbf {N} = \left[ \begin{array}{l l} 1 & 1 \\ 2 & 1 \\ 5 & 1 0 \end{array} \right], \mathbf {x _ {N}} = \left[ \begin{array}{l} x _ {1} \\ x _ {2} \end{array} \right]
$$

we get an initial basic feasible solution (BFS) with $\mathbf { x _ { B } } = \mathbf { B ^ { - 1 } b } = [ 1 0 0 , 1 5 0 , 3 6 0 ] ^ { T }$ The objective value for this BFS is $4 \cdot 0 + 3 \cdot 0 = 0$ 

Once we obtain a BFS, we first need to determine whether this solution is optimal or whether there is a way to improve the objective value. Recall that the basic variables are uniquely determined once we choose to set the nonbasic variables to a specific value, namely zero. $\mathrm { S o } .$ , the only way to obtain alternative solutions is to modify the values of the nonbasic variables. We observe that both the nonbasic variables $x _ { 1 }$ and $x _ { 2 }$ would improve the objective value if they were introduced into the basis. Why? The initial basic feasible solution has $x _ { 1 } = x _ { 2 } = 0$ and we can get other feasible solutions by increasing the value of one of these two variables. To preserve feasibility of the equality constraints, this will require adjusting the values of the basic variables $x _ { 3 } , x _ { 4 }$ , and $x _ { 5 }$ . But since all three are strictly positive in the initial basic feasible solution, it is possible to make $x _ { 1 }$ strictly positive without violating any of the constraint, including the nonnegativity requirements. 

None of the variables $x _ { 3 } , \ x _ { 4 }$ , x<sub>5</sub> appear in the objective row. Thus, we only have to look at the coeficient of the nonbasic variable we would increase to see what efect this would have on the objective value. The rate of improvement in the objective value for $x _ { 1 }$ is 4 and for $x _ { 2 }$ this rate is only 3. While a diferent method may choose the increase both of these variables simultaneously, the simplex method requires that only one nonbasic variable is modified at a time. This requirement is the algebraic equivalent of the geometric condition of moving from one extreme point to an adjacent extreme point. Between $x _ { 1 }$ and $x _ { 2 }$ , we choose the variable $x _ { 1 }$ to enter the basis since it has a faster rate of improvement. 

The basis holds as many variables as there are equality constraints in the standard form formulation of the problem. Since $x _ { 1 }$ is to enter the basis, one of $x _ { 3 } , \ x _ { 4 }$ , and $x _ { 5 }$ must leave the basis. Since nonbasic variables have value zero in a basic solution, we need to determine how much to increase $x _ { 1 }$ so that one of the current basic variables becomes zero and can be designated as nonbasic. The important issue here is to maintain the nonnegativity of all basic variables. Because each basic variable only appears in one row, this is an easy task. As we increase $x _ { 1 }$ , all current basic variables will decrease since $x _ { 1 }$ has positive coeficients in each $\mathrm { r o w } ^ { 4 }$ . We guarantee the nonnegativity of the basic variables of the next iteration by using the ratio test. We observe that 

$$
\begin{array}{l l l} \text {increasing x_ {1} beyond 100 / 1 = 100} & \Rightarrow & x _ {3} <   0, \\ \text {increasing x_ {1} beyond 150 / 2 = 75} & \Rightarrow & x _ {4} <   0, \\ \text {increasing x_ {1} beyond 360 / 3 = 120} & \Rightarrow & x _ {5} <   0, \end{array}
$$

so we should not increase $x _ { 1 }$ more than min $\{ 1 0 0 , 7 5 , 1 2 0 \} = 7 5$ . On the other hand if we increase $x _ { 1 }$ exactly by $7 5 , x _ { 4 }$ will become zero. The variable $x _ { 4 }$ is said to leave the basis. It has now become a nonbasic variable. 

Now we have a new basis: $\{ x _ { 3 } , x _ { 1 } , x _ { 5 } \}$ . For this basis we have the following basic feasible solution: 

$$
\mathbf {B} = \left[ \begin{array}{l l l} 1 & 1 & 0 \\ 0 & 2 & 0 \\ 0 & 3 & 1 \end{array} \right], \mathbf {x} _ {B} = \left[ \begin{array}{l} x _ {3} \\ x _ {1} \\ x _ {5} \end{array} \right] = \mathbf {B} ^ {- 1} \mathbf {b} = \left[ \begin{array}{l l l} 1 & - 1 / 2 & 0 \\ 0 & 1 / 2 & 0 \\ 0 & - 3 / 2 & 1 \end{array} \right] \left[ \begin{array}{l} 1 0 0 \\ 1 5 0 \\ 3 6 0 \end{array} \right] = \left[ \begin{array}{l} 2 5 \\ 7 5 \\ 1 3 5 \end{array} \right],
$$

$$
\mathbf {N} = \left[ \begin{array}{l l} 1 & 0 \\ 1 & 1 \\ 4 & 0 \end{array} \right], \mathbf {x _ {N}} = \left[ \begin{array}{l} x _ {2} \\ x _ {4} \end{array} \right] = \left[ \begin{array}{l} 0 \\ 0 \end{array} \right].
$$

## 2.4. THE SIMPLEX METHOD

After finding a new feasible solution, we always ask the question ‘Is this the optimal solution, or can we still improve $\mathrm { i t ? } \ '$ . Answering that question was easy when we started, because none of the basic variables were in the objective function. Now that we have introduced $x _ { 1 }$ into the basis, the situation is more complicated. If we now decide to increase $x _ { 2 }$ , the objective row coeficient of $x _ { 2 }$ does not tell us how much the objective value changes per unit change in $x _ { 2 }$ , because changing $x _ { 2 }$ requires changing $x _ { 1 }$ , a basic variable that appears in the objective row. It may happen that, increasing $x _ { 2 }$ by 1 unit does not increase the objective value by 3 units, because $x _ { 1 }$ may need to be decreased, pulling down the objective function. It could even happen that increasing $x _ { 2 }$ actually decreases the objective value even though $x _ { 2 }$ has a positive coeficient in the objective function. So, what do we do? We could still do what we did with the initial basic solution if $x _ { 1 }$ did not appear in the objective row and the rows where it is not the basic variable. To achieve this, all we need to do is to use the row where $x _ { 1 }$ is the basic variable (in this case the second row) to solve for $x _ { 1 }$ in terms of the nonbasic variables and then substitute this expression for $x _ { 1 }$ in the objective row and other equations. $\mathrm { S o } ,$ the second equation 

$$
2 x _ {1} + x _ {2} + x _ {4} = 1 5 0
$$

would give us: 

$$
x _ {1} = 7 5 - \frac {1}{2} x _ {2} - \frac {1}{2} x _ {4}.
$$

Substituting this value in the objective function we get: 

$$
Z = 4 x _ {1} + 3 x _ {2} = 4 (7 5 - \frac {1}{2} x _ {2} - \frac {1}{2} x _ {4}) + 3 x _ {2} = 3 0 0 + x _ {2} - 2 x _ {4}.
$$

Continuing the substitution we get the following representation of the original bond portfolio problem: 

max $Z$ 

subject to: 

$$
\begin{array}{r l r l r l r l r l r l r l} {Z} & {- x _ {2}} & & {+} & {2 x _ {4}} & & & & & & & = & 3 0 0 \\ & & & {\frac {1}{2} x _ {2}} & {-} & {\frac {1}{2} x _ {4}} & + & {x _ {3}} & & & & & = & 2 5 \\ & & & {\frac {1}{2} x _ {2}} & {+} & {\frac {1}{2} x _ {4}} & & & + & {x _ {1}} & & & = & 7 5 \\ & & & {\frac {5}{2} x _ {2}} & {-} & {\frac {3}{2} x _ {4}} & & & & & + & {x _ {5}} & = & 1 3 5 \\ & & & {x _ {2}} & , & {x _ {4}} & , & {x _ {3}} & , & {x _ {1}} & , & {x _ {5}} & \geq & 0. \end{array}
$$

This representation looks exactly like the initial system. Once again, the objective row is free of basic variables and basic variables only appear in the row where they are basic, with a coeficient of 1. Therefore, we now can tell how a change in a nonbasic variables would efect the objective function: increasing $x _ { 2 }$ by 1 unit will increase the objective function by 1 unit (not 3!) and increasing $x _ { 4 }$ by 1 unit will decrease the objective function by 2 units. 

Now that we represented the problem in a form identical to the original, we can repeat what we did before, until we find a representation that gives 

## 36CHAPTER 2. LINEAR PROGRAMMING: THEORY AND ALGORITHMS

the optimal solution. If we repeat the steps of the simplex method , we find that x<sub>2</sub> will be introduced into the basis next, and the leaving variable will be $x _ { 3 }$ . If we solve for $x _ { 1 }$ using the first equation and substitute for it in the remaining ones, we get the following representation: 

max Z 

subject to: 

$$
\begin{array}{r c l r c l r c l r c l r c l} {Z} & {+} & {2 x _ {3}} & {+} & {x _ {4}} & & & & & & & {=} & {3 5 0} \\ & & {2 x _ {3}} & {-} & {x _ {4}} & {+} & {x _ {2}} & & & & & {=} & {5 0} \\ & & {- x _ {3}} & {+} & {x _ {4}} & & & {+} & {x _ {1}} & & & {=} & {5 0} \\ & & {- 5 x _ {3}} & {+} & {x _ {4}} & & & & & {+} & {x _ {5}} & {=} & {1 0} \\ & & {x _ {3}} & {,} & {x _ {4}} & {,} & {x _ {2}} & {,} & {x _ {1}} & {,} & {x _ {5}} & {\geq} & {0.} \end{array}
$$

Once again, notice that this representation is very similar to the tableau we got at the end of the previous section. The basis and the basic solution that corresponds to the system above is: 

$$
\mathbf {B} = \left[ \begin{array}{l l l} 1 & 1 & 0 \\ 1 & 2 & 0 \\ 4 & 3 & 1 \end{array} \right], \mathbf {x _ {B}} = \left[ \begin{array}{l} x _ {2} \\ x _ {1} \\ x _ {5} \end{array} \right] = B ^ {- 1} b = \left[ \begin{array}{r r r} 2 & - 1 & 0 \\ - 1 & 1 & 0 \\ - 5 & 1 & 1 \end{array} \right] \left[ \begin{array}{l} 1 0 0 \\ 1 5 0 \\ 3 6 0 \end{array} \right] = \left[ \begin{array}{l} 5 0 \\ 5 0 \\ 1 0 \end{array} \right],
$$

$$
\mathbf {N} = \left[ \begin{array}{l l} 1 & 0 \\ 0 & 1 \\ 0 & 0 \end{array} \right],   \mathbf {x _ {N}} = \left[ \begin{array}{l} x _ {3} \\ x _ {4} \end{array} \right] = \left[ \begin{array}{l} 0 \\ 0 \end{array} \right].
$$

At this point we can conclude that this basic solution is the optimal solution. Let us try to understand why. From the objective function row of our final representation of the problem we have that for any feasible solution ${ \boldsymbol x } = ( x _ { 1 } , x _ { 2 } , x _ { 3 } , x _ { 4 } , x _ { 5 } )$ , the objective function Z satisfies 

$$
\mathbf {Z} + 2 x _ {3} + x _ {4} = 3 5 0.
$$

Since $x _ { 3 } \geq 0$ and $x _ { 4 } \geq 0$ is also required, this implies that in every feasible solution 

$$
\mathbf {Z} \leq 3 5 0.
$$

But we just found a basic feasible solution with value 350. So this is the optimal solution. 

More generally, recall that for any $\mathrm { B F S } \mathbf { x } = ( \mathbf { x _ { B } } , \mathbf { x _ { N } } )$ , the objective value Z satisfies 

$$
\mathbf {Z} - \left(\mathbf {c _ {N}} - \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \mathbf {N}\right) \mathbf {x _ {N}} = \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \mathbf {b}
$$

If for a BFS $\mathbf { x _ { B } } = \mathbf { B } ^ { - 1 } \mathbf { b } \geq \mathbf { 0 } , \mathbf { x _ { N } } = \mathbf { 0 }$ , we have 

$$
\mathbf {c} _ {\mathbf {N}} - \mathbf {c} _ {\mathbf {B}} \mathbf {B} ^ {- 1} \mathbf {N} \leq \mathbf {0},
$$

then this solution is an optimal solution since it has objective value $\mathbf { Z } = \mathbf { c _ { B } } \mathbf { B } ^ { - 1 } \mathbf { b }$ whereas, for all other solutions, ${ \bf x } _ { \bf N } \geq { \bf 0 }$ implies that $\mathbf { Z } \leq \mathbf { c _ { B } } \mathbf { B } ^ { - 1 } \mathbf { b }$ 

Exercise 2.16 What is the solution to the following linear programming problem: 

$$
\begin{array}{r l} \text {Max} & z = c _ {1} x _ {1} + c _ {2} x _ {2} + \dots + c _ {n} x _ {n} \\ \text {s.t.} & a _ {1} x _ {1} + a _ {2} x _ {2} + \dots + a _ {n} x _ {n} \leq b, \\ & 0 \leq x _ {i} \leq u _ {i} (i = 1, 2, \ldots , n), \end{array}
$$

Assume that all the data elements $( c _ { i } , a _ { i }$ , and $u _ { i } )$ are strictly positive and the coeficients are arranged such that: 

$$
\frac {c _ {1}}{a _ {1}} \geq \frac {c _ {2}}{a _ {2}} \geq \ldots \geq \frac {c _ {n}}{a _ {n}}.
$$

Write the problem in standard form and apply the simplex method to it. What will be the steps of the simplex method when applied to this problem, i.e., in what order will the variables enter and leave the basis? 

## 2.4.3 The Tableau Form of the Simplex Method

In most linear programming textbooks, the simplex method is described using tableaus that summarize the information in the diferent representations of the problem we saw above. Since the reader will likely encounter simplex tableaus elsewhere, we include a brief discussion for the purpose of completeness. To study the tableau form of the simplex method, we recall the bond portfolio example of the previous subsection. We begin by rewriting the objective row as 

$$
Z - 4 x _ {1} - 3 x _ {2} = 0
$$

and represent this system using the following tableau: 

<table><tr><td rowspan="2"></td><td rowspan="2">Basic var.</td><td colspan="5"><eq>\Downarrow</eq></td><td rowspan="2"></td></tr><tr><td><eq>x_1</eq></td><td><eq>x_2</eq></td><td><eq>x_3</eq></td><td><eq>x_4</eq></td><td><eq>x_5</eq></td></tr><tr><td></td><td>Z</td><td>-4</td><td>-3</td><td>0</td><td>0</td><td>0</td><td>0</td></tr><tr><td rowspan="3"><eq>\Leftarrow</eq></td><td><eq>x_3</eq></td><td>1</td><td>1</td><td>1</td><td>0</td><td>0</td><td>100</td></tr><tr><td><eq>x_4</eq></td><td><eq>2^*</eq></td><td>1</td><td>0</td><td>1</td><td>0</td><td>150</td></tr><tr><td><eq>x_5</eq></td><td>3</td><td>4</td><td>0</td><td>0</td><td>1</td><td>360</td></tr></table>

This tableau is often called the simplex tableau. The columns labeled by each variable contain the coeficients of that variable in each equation, including the objective row equation. The leftmost column is used to keep track of the basic variable in each row. The arrows and the asterisk will be explained below. 

## Step 0. Form the initial tableau.

Once we have formed this tableau we look for an entering variable, i.e., a variable that has a negative coeficient in the objective row and will improve the objective function if it is introduced into the basis. In this case, two of the variables, namely $x _ { 1 }$ and $x _ { 2 }$ , have negative objective row coeficients. 

Since $x _ { 1 }$ has the most negative coeficient we will pick that one (this is indicated by the arrow pointing down on $x _ { 1 } )$ , but in principle any variable with a negative coeficient in the objective row can be chosen to enter the basis. 

Step 1. Find a variable with a negative coeficient in the first row (the objective row). If all variables have nonnegative coeficients in the objective row, STOP, the current tableau is optimal. 

After we choose $x _ { 1 }$ as the entering variable, we need to determine a leaving variable. The leaving variable is found by performing a ratio test. In the ratio test, one looks at the column that corresponds to the entering variable, and for each positive entry in that column computes the ratio of that positive number to the right hand side value in that row. The minimum of these ratios tells us how much we can increase our entering variable without making any of the other variables negative. The basic variable in the row that gives the minimum ratio becomes the leaving variable. In the tableau above the column for the entering variable, the column for the right-hand-side values, and the ratios of corresponding entries are 

$$
\left[ \begin{array}{c} x _ {1} \\ 1 \\ 2 \\ 5 \end{array} \right], \quad \left[ \begin{array}{c} \text {RHS} \\ 1 0 0 \\ 1 5 0 \\ 3 6 0 \end{array} \right], \quad \begin{array}{c} \text {ratio} \\ 1 0 0 / 1 \\ 1 5 0 / 2 \\ 3 6 0 / 3 \end{array} , \min \{\frac {1 0 0}{1}, \frac {1 5 0 ^ {*}}{2}, \frac {3 6 0}{3} \} = 7 5,
$$

and therefore $x _ { 4 } ,$ the basic variable in the second row, is chosen as the leaving variable, as indicated by the left-pointing arrow in the tableau. 

One important issue here is that, we only look at the positive entries in the column when we perform the ratio test. Notice that if some of these entries were negative, then increasing the entering variable would only increase the basic variable in those rows, and would not force them to be negative, therefore we need not worry about those entries. Now, if all of the entries in a column for an entering variable turn out to be zero or negative, then we conclude that the problem must be unbounded; we can increase the entering variable (and the objective value) indefinitely, the equalities can be balanced by increasing the basic variables appropriately, and none of the nonnegativity constraints will be violated. 

Step 2. Consider the column picked in Step 1. For each positive entry in this column, calculate the ratio of the right-hand-side value to that entry. Find the row that gives minimum such ratio and choose the basic variable in that row as the leaving variable. If all the entries in the column are zero or negative, STOP, the problem is unbounded. 

Before proceeding to the next iteration, we need to update the tableau to reflect the changes in the set of basic variables. For this purpose, we choose a pivot element, which is the entry in the tableau that lies in the intersection of the column for the entering variable (the pivot column), and the row for the leaving variable (the pivot row). In the tableau above, the 

## 2.4. THE SIMPLEX METHOD

pivot element is the number 2, marked with an asterisk. The next job is pivoting. When we pivot, we aim to get the number 1 in the position of the pivot element (which can be achieved by dividing the entries in the pivot row by the pivot element), and zeros elsewhere in the pivot column (which can be achieved by adding suitable multiples of the pivot row to the other rows, including the objective row). All these operations are row operations on the matrix that consists of the numbers in the tableau, and what we are doing is essentially Gaussian elimination on the pivot column. Pivoting on the tableau above yields: 

<table><tr><td rowspan="2"></td><td rowspan="2">Basic var.</td><td colspan="5"><eq>\Downarrow</eq></td><td rowspan="2"></td></tr><tr><td><eq>x_1</eq></td><td><eq>x_2</eq></td><td><eq>x_3</eq></td><td><eq>x_4</eq></td><td><eq>x_5</eq></td></tr><tr><td></td><td>Z</td><td>0</td><td>-1</td><td>0</td><td>2</td><td>0</td><td>300</td></tr><tr><td rowspan="3"><eq>\Leftarrow</eq></td><td><eq>x_3</eq></td><td>0</td><td><eq>1/2^*</eq></td><td>1</td><td>-1/2</td><td>0</td><td>25</td></tr><tr><td><eq>x_1</eq></td><td>1</td><td>1/2</td><td>0</td><td>1/2</td><td>0</td><td>75</td></tr><tr><td><eq>x_5</eq></td><td>0</td><td>5/2</td><td>0</td><td>-3/2</td><td>1</td><td>135</td></tr></table>

Step 3. Find the entry (the pivot element) in the intersection of the column picked in Step 1 (the pivot column) and the row picked in Step 2 (the pivot row). Pivot on that entry, $i . e . ,$ divide all the entries in the pivot row by the pivot element, add appropriate multiples of the pivot row to the others in order to get zeros in other components of the pivot column. Go to Step 1. 

If we repeat the steps of the simplex method, this time working with the new tableau, we first identify $x _ { 2 }$ as the only candidate to enter the basis. Next, we do the ratio test: 

$$
\min \{\frac {2 5 ^ {*}}{1 / 2}, \frac {7 5}{1 / 2}, \frac {1 3 5}{5 / 2} \} = 5 0,
$$

so $x _ { 3 }$ leaves the basis. Now, one more pivot produces the optimal tableau: 

<table><tr><td>Basic var.</td><td><eq>x_{1}</eq></td><td><eq>x_{2}</eq></td><td><eq>x_{3}</eq></td><td><eq>x_{4}</eq></td><td><eq>x_{5}</eq></td><td></td></tr><tr><td>Z</td><td>0</td><td>0</td><td>2</td><td>1</td><td>0</td><td>350</td></tr><tr><td><eq>x_{2}</eq></td><td>0</td><td>1</td><td>2</td><td>-1</td><td>0</td><td>50</td></tr><tr><td><eq>x_{1}</eq></td><td>1</td><td>0</td><td>-1</td><td>1</td><td>0</td><td>50</td></tr><tr><td><eq>x_{5}</eq></td><td>0</td><td>0</td><td>-5</td><td>1</td><td>1</td><td>10</td></tr></table>

This solution is optimal since all the coeficients in the objective row are nonnegative. 

Exercise 2.17 Solve the following linear program by the simplex method. 

max 

$$
\begin{array}{r c l r c l r c l} 4 x _ {1} & + & x _ {2} & - & x _ {3} \\ x _ {1} & & & + & 3 x _ {3} & \leq & 6 \\ 3 x _ {1} & + & x _ {2} & + & 3 x _ {3} & \leq & 9 \\ x _ {1} \geq 0, & & x _ {2} \geq 0, & & x _ {3} \geq 0. \end{array}
$$

## Answer:

<table><tr><td></td><td><eq>x_{1}</eq></td><td><eq>x_{2}</eq></td><td><eq>x_{3}</eq></td><td><eq>s_{1}</eq></td><td><eq>s_{2}</eq></td><td></td></tr><tr><td>Z</td><td>-4</td><td>-1</td><td>1</td><td>0</td><td>0</td><td>0</td></tr><tr><td><eq>s_{1}</eq></td><td>1</td><td>0</td><td>3</td><td>1</td><td>0</td><td>6</td></tr><tr><td><eq>s_{2}</eq></td><td>3</td><td>1</td><td>3</td><td>0</td><td>1</td><td>9</td></tr><tr><td>Z</td><td>0</td><td><eq>\frac{1}{3}</eq></td><td>5</td><td>0</td><td><eq>\frac{4}{3}</eq></td><td>12</td></tr><tr><td><eq>s_{1}</eq></td><td>0</td><td><eq>\frac{-1}{3}</eq></td><td>2</td><td>1</td><td><eq>\frac{-1}{3}</eq></td><td>3</td></tr><tr><td><eq>x_{1}</eq></td><td>1</td><td><eq>\frac{1}{3}</eq></td><td>1</td><td>0</td><td><eq>\frac{1}{3}</eq></td><td>3</td></tr></table>


The optimal solution is $x _ { 1 } = 3 , x _ { 2 } = x _ { 3 } = 0 .$ 


Exercise 2.18 Solve the following linear program by the simplex method. 

$$
\begin{array}{r l r l r l r l} \max & 4 x _ {1} + & x _ {2} - & x _ {3} \\ & x _ {1} & & + & 3 x _ {3} \leq 6 \\ & 3 x _ {1} + & x _ {2} + & 3 x _ {3} \leq 9 \\ & x _ {1} + & x _ {2} - & x _ {3} \leq 2 \\ & x _ {1} \geq 0, & x _ {2} \geq 0, & x _ {3} \geq 0. \end{array}
$$

Exercise 2.19 Suppose the following tableau was obtained in the course of solving a linear program with nonnegative variables $x _ { 1 } , x _ { 2 } , x _ { 3 }$ and two inequalities. The objective function is maximized and slack variables $x _ { 4 }$ and x were added. 

<table><tr><td>Basic var.</td><td><eq>x_{1}</eq></td><td><eq>x_{2}</eq></td><td><eq>x_{3}</eq></td><td><eq>x_{4}</eq></td><td><eq>x_{5}</eq></td><td></td></tr><tr><td>Z</td><td>0</td><td>a</td><td>b</td><td>0</td><td>4</td><td>82</td></tr><tr><td><eq>x_{4}</eq></td><td>0</td><td>-2</td><td>2</td><td>1</td><td>3</td><td>c</td></tr><tr><td><eq>x_{1}</eq></td><td>1</td><td>-1</td><td>3</td><td>0</td><td>-5</td><td>3</td></tr></table>

Give conditions on $^ { a , }$ b and c that are required for the following statements to be true: 

(i) The current basic solution is a basic feasible solution. 

Assume that the condition found in (i) holds in the rest of the exercise. 

(ii) The current basic solution is optimal. 

(iii) The linear program is unbounded (for this question, assume that $b > 0 )$ 

(iv) The current basic solution is optimal and there are alternate optimal solutions (for this question, assume that $a > 0 )$ 

## 2.4.4 Graphical Interpretation

Figure 2.1 shows the feasible region for Example 2.1. The five inequality constraints define a convex pentagon. The five corner points of this pentagon (the black dots on the figure) are the basic feasible solutions: each such solution satisfies two of the constraints with equality. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/4e898543ce6995221cefac05be1e2d9cabae616830ca2e1f81ff4ebdb7526a33.jpg)



Figure 2.1: Graphical interpretation of the simplex iterations


Which are the solutions explored by the simplex method? The simplex method starts from the basic feasible solution $( x _ { 1 } = 0 , x _ { 2 } = 0 )$ (in this solution, $x _ { 1 }$ and $x _ { 2 }$ are the nonbasic variables. The basic variables $x _ { 3 } =$ 100, $x _ { 4 } = 1 5 0$ and $x _ { 5 } ~ = ~ 3 6 0$ correspond to the constraints that are not satisfied with equality). The first iteration of the simplex method makes $x _ { 1 }$ basic by increasing it along an edge of the feasible region until some other constraint is satisfied with equality. This leads to the new basic feasible solution $( x _ { 1 } = 7 5 , x _ { 2 } = 0 )$ (in this solution, $x _ { 2 }$ and $x _ { 4 }$ are nonbasic, which means that the constraints $x _ { 2 } \geq 0$ and $2 x _ { 1 } + x _ { 2 } \le 1 5 0$ are satisfied with equality). The second iteration makes $x _ { 2 }$ basic while keeping $x _ { 4 }$ nonbasic. This correspond to moving along the edge $2 x _ { 1 } + x _ { 2 } = 1 5 0$ . The value $x _ { 2 }$ is increased until another constraint becomes satisfied with equality. The new solution is $x _ { 1 } = 5 0$ and $x _ { 2 } = 5 0$ . No further movement from this point can increase the objective, so this is the optimal solution. 

Exercise 2.20 Solve the linear program of Exercise 2.14 by the simplex method. Give a graphical interpretation of the simplex iterations. 

Exercise 2.21 Find basic solutions of Example 2.1 that are not feasible. Identify these solutions in Figure 2.1. 

## 2.4.5 The Dual Simplex Method

The previous sections describe the primal simplex method, which moves from a basic feasible solution to another until all the reduced costs are nonpositive. There are certain applications where the dual simplex method is faster. In contrast to the primal simplex method, this method keeps the reduced costs nonpositive and moves from a basic (infeasible) solution to another until a basic feasible solution is reached. 

We illustrate the dual simplex method on an example. Consider Exam-

ple 2.1 with the following additional constraint. 

$$
6 x _ {1} + 5 x _ {2} \leq 5 0 0
$$

Adding a slack variable $x _ { 6 } .$ , we get $6 x _ { 1 } + 5 x _ { 2 } + x _ { 6 } = 5 0 0$ . To initialize the dual simplex method, we can start from any basic solution with nonpositive reduced costs. For example, we can start from the optimal solution that we found in Section 2.4.3, without the additional constraint, and make $x _ { 6 }$ basic. This gives the following tableau. 

<table><tr><td>Basic var.</td><td><eq>x_{1}</eq></td><td><eq>x_{2}</eq></td><td><eq>x_{3}</eq></td><td><eq>x_{4}</eq></td><td><eq>x_{5}</eq></td><td><eq>x_{6}</eq></td><td></td></tr><tr><td>Z</td><td>0</td><td>0</td><td>2</td><td>1</td><td>0</td><td>0</td><td>350</td></tr><tr><td><eq>x_{2}</eq></td><td>0</td><td>1</td><td>2</td><td>-1</td><td>0</td><td>0</td><td>50</td></tr><tr><td><eq>x_{1}</eq></td><td>1</td><td>0</td><td>-1</td><td>1</td><td>0</td><td>0</td><td>50</td></tr><tr><td><eq>x_{5}</eq></td><td>0</td><td>0</td><td>-5</td><td>1</td><td>1</td><td>0</td><td>10</td></tr><tr><td><eq>x_{6}</eq></td><td>6</td><td>5</td><td>0</td><td>0</td><td>0</td><td>1</td><td>500</td></tr></table>

Actually, this tableau is not yet in the right format. Indeed, $x _ { 1 }$ and $x _ { 2 }$ are basic and therefore their columns in the tableau should be unit vectors. To restore this property, it sufices to eliminate the 6 and 5 in the row of x by subtracting appropriate multiples of the rows of $x _ { 1 }$ and $x _ { 2 }$ . This now gives the tableau in the correct format. 

<table><tr><td>Basic var.</td><td><eq>x_{1}</eq></td><td><eq>x_{2}</eq></td><td><eq>x_{3}</eq></td><td><eq>x_{4}</eq></td><td><eq>x_{5}</eq></td><td><eq>x_{6}</eq></td><td></td></tr><tr><td>Z</td><td>0</td><td>0</td><td>2</td><td>1</td><td>0</td><td>0</td><td>350</td></tr><tr><td><eq>x_{2}</eq></td><td>0</td><td>1</td><td>2</td><td>-1</td><td>0</td><td>0</td><td>50</td></tr><tr><td><eq>x_{1}</eq></td><td>1</td><td>0</td><td>-1</td><td>1</td><td>0</td><td>0</td><td>50</td></tr><tr><td><eq>x_{5}</eq></td><td>0</td><td>0</td><td>-5</td><td>1</td><td>1</td><td>0</td><td>10</td></tr><tr><td><eq>x_{6}</eq></td><td>0</td><td>0</td><td>-4</td><td>-1</td><td>0</td><td>1</td><td>-50</td></tr></table>

Now we are ready to apply the dual simplex algorithm. Note that the current basic solution $x _ { 1 } = 5 0 , x _ { 2 } = 5 0 , x _ { 3 } = x _ { 4 } = 0 , x _ { 5 } = 1 0 , x _ { 6 } = - 5 0$ is infeasible since $x _ { 6 }$ is negative. We will pivot to make it nonnegative. As a result, variable $x _ { 6 }$ will leave the basis. The pivot element will be one of the negative entry in the row of $x _ { 6 } .$ , namely -4 or -1. Which one should we choose in order to keep all the reduced costs nonnegative? The minimum ratio between $\frac { 2 } { | - 4 | }$ and $\frac { 1 } { | - 1 | }$ determines the variable that enters the basis. Here the minimum is $\begin{array} { l } { { \frac { 1 } { 2 } } } \end{array}$ , which means that $x _ { 3 }$ enters the basis. After pivoting on -4, the tableau becomes: 

<table><tr><td>Basic var.</td><td><eq>x_{1}</eq></td><td><eq>x_{2}</eq></td><td><eq>x_{3}</eq></td><td><eq>x_{4}</eq></td><td><eq>x_{5}</eq></td><td><eq>x_{6}</eq></td><td></td></tr><tr><td>Z</td><td>0</td><td>0</td><td>0</td><td>0.5</td><td>0</td><td>0.5</td><td>325</td></tr><tr><td><eq>x_{2}</eq></td><td>0</td><td>1</td><td>0</td><td>-1.5</td><td>0</td><td>0.5</td><td>25</td></tr><tr><td><eq>x_{1}</eq></td><td>1</td><td>0</td><td>0</td><td>1.25</td><td>0</td><td>-0.25</td><td>62.5</td></tr><tr><td><eq>x_{5}</eq></td><td>0</td><td>0</td><td>0</td><td>2.25</td><td>1</td><td>-1.25</td><td>72.5</td></tr><tr><td><eq>x_{3}</eq></td><td>0</td><td>0</td><td>1</td><td>0.25</td><td>0</td><td>-0.25</td><td>12.5</td></tr></table>

## 2.4. THE SIMPLEX METHOD

The corresponding basic solution is $x _ { 1 } = 6 2 . 5 , \ x _ { 2 } = 2 5 , \ x _ { 3 } = 1 2 . 5 .$ $x _ { 4 } = 0 , x _ { 5 } = 7 2 . 5 , x _ { 6 } = 0$ . Since it is feasible and all reduced costs are nonpositive, this is the optimum solution. If there had still been negative basic variables in the solution, we would have continued pivoting using the rules outlined above: the variable that leaves the basis is one with a negative value, the pivot element is negative, and the variable that enters the basis is chosen by the minimum ratio rule. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/aaa3641b77cdc4f9ff1f6ddf27051c462cbd40733efcc14ced16d807dad67c61.jpg)



Figure 2.2: Graphical interpretation of the dual simplex iteration


Exercise 2.22 Solve the following linear program by the dual simplex method, starting from the solution found in Exercise 2.17. 

$$
\begin{array}{c c c c c c c c} \max & 4 x _ {1} & + & x _ {2} & - & x _ {3} \\ & x _ {1} & & & + & 3 x _ {3} & \leq & 6 \\ & 3 x _ {1} & + & x _ {2} & + & 3 x _ {3} & \leq & 9 \\ & x _ {1} & + & x _ {2} & - & x _ {3} & \leq & 2 \\ & x _ {1} \geq 0, & & x _ {2} \geq 0, & & x _ {3} \geq 0. \end{array}
$$

## 2.4.6 Alternatives to the Simplex Method

Performing a pivot of the simplex method is extremely fast on today’s computers, even for problems with thousands of variables and hundreds of constraints. This explains the success of the simplex method. However, for large problems, the number of iterations also tends to be large. At the time of this writing, LPs with tens of thousands of constraints and 100,000 or more variables are generally considered large problems. Such models are not uncommon in financial applications and can often be handled by the simplex method. 

Although the simplex method demonstrates satisfactory performance for the solution of most practical problems, it has the disadvantage that, in the worst case, the amount of computing time (the so-called worst-case complexity) can grow exponentially in the size of the problem. Here size refers to the space required to write all the data in binary. If all the numbers are bounded (say between $1 0 ^ { - 6 }$ and $1 0 ^ { 6 } )$ , a good proxy for the size of a linear program is the number of variables times the number of constraints. One of the important concepts in the theoretical study of optimization algorithms is the concept of polynomial-time algorithms. This refers to an algorithm whose running time can be bounded by a polynomial function of the input size for all instances of the problem class that it is intended for. After it was discovered in the 1970s that the worst case complexity of the simplex method is exponential (and, therefore, that the simplex method is not a polynomial-time algorithm) there was an efort to identify alternative methods for linear programming with polynomial-time complexity. The first such method, called the ellipsoid method was developed by Yudin and Nemirovski in 1979. The same year Khachiyan [41] proved that the ellipsoid method is a polynomial-time algorithm for linear programming. But the more exciting and enduring development was the announcement by Karmarkar in 1984 that an Interior Point Method (IPM) can solve LPs in polynomial time. What distinguished Karmarkar’s IPM from the ellipsoid method was that, in addition to having this desirable theoretical property, it could solve some real-world LPs much faster than the simplex method. These methods use a diferent strategy to reach the optimum, generating iterates in the interior of the feasible region rather than at its extreme points. Each iteration is fairly expensive, but the number of iterations needed does not depend much on the size of the problem and is often less than 50. As a result, interior point methods can be faster than the simplex method for large scale problems. Most state-of-the-art linear programming packages (Cplex, Xpress, OSL, etc.) give you the option to solve your linear programs by either method. 

We present interior point methods in Chapter 7, in the context of solving quadratic programs. 

## Chapter 3

# LP Models: Asset/Liability Cash Flow Matching

## 3.1 Short Term Financing

Corporations routinely face the problem of financing short term cash commitments. Linear programming can help in figuring out an optimal combination of financial instruments to meet these commitments. To illustrate this, consider the following problem. For simplicity of exposition, we keep the example very small. 


A company has the following short term financing problem.


<table><tr><td>Month</td><td>Jan</td><td>Feb</td><td>Mar</td><td>Apr</td><td>May</td><td>Jun</td></tr><tr><td>Net Cash Flow</td><td>-150</td><td>-100</td><td>200</td><td>-200</td><td>50</td><td>300</td></tr></table>

Net cash flow requirements are given in thousands of dollars. The company has the following sources of funds 

A line of credit of up to $100K at an interest rate of 1% per month, 

In any one of the first three months, it can issue 90-day commercial paper bearing a total interest of 2% for the 3-month period, 

Excess funds can be invested at an interest rate of 0.3% per month. 

There are many questions that the company might want to answer. What interest payments will the company need to make between January and June? Is it economical to use the line of credit in some of the months? If so, when? How much? Linear programming gives us a mechanism for answering these questions quickly and easily. It also allows to answer some “what if” questions about changes in the data without having to resolve the problem. What if Net Cash Flow in January were -200 (instead of -150)? What if the limit on the credit line were increased from 100 to 200? What if the negative Net Cash Flow in January is due to the purchase of a machine worth 150 and the vendor allows part or all of the payment on this machine to be made in June at an interest of 3% for the 5-month period? The answers to these questions are readily available when this problem is formulated and solved as a linear program. 

There are three steps in applying linear programming: modeling, solving, and interpreting. 

## 3.1.1 Modeling

We begin by modeling the above short term financing problem. That is, we write it in the language of linear programming. There are rules about what one can and cannot do within linear programming. These rules are in place to make certain that the remaining steps of the process (solving and interpreting) can be successful. 

Key to a linear program are the decision variables, objective, and constraints. 

Decision Variables. The decision variables represent (unknown) decisions to be made. This is in contrast to problem data, which are values that are either given or can be simply calculated from what is given. For the short term financing problem, there are several possible choices of decision variables. We will use the following decision variables: the amount $x _ { i }$ drawn from the line of credit in month i, the amount $y _ { i }$ of commercial paper issued in month $i ,$ the excess funds $z _ { i }$ in month i and the company’s wealth v in June. Note that, alternatively, one could use the decision variables $x _ { i }$ and $z _ { i }$ only, since excess funds and company’s wealth can be deduced from these variables. 

Objective. Every linear program has an objective. This objective is to be either minimized or maximized. This objective has to be linear in the decision variables, which means it must be the sum of constants times decision variables. $3 x _ { 1 } - 1 0 x _ { 2 }$ is a linear function. $x _ { 1 } x _ { 2 }$ is not a linear function. In this case, our objective is simply to maximize v. 

Constraints. Every linear program also has constraints limiting feasible decisions. Here we have three types of constraints: (i) cash inflow = cash outflow for each month, (ii) upper bounds on $x _ { i }$ and (iii) nonnegativity of the decision variables $x _ { i }$ , y<sub>i</sub> and $z _ { i } .$ 

For example, in January $( i = 1 )$ , there is a cash requirement of $150. To meet this requirement, the company can draw an amount $x _ { 1 }$ from its line of credit and issue an amount $y _ { 1 }$ of commercial paper. Considering the possibility of excess funds $z _ { 1 }$ (possibly 0), the cash flow balance equation is as follows. 

$$
x _ {1} + y _ {1} - z _ {1} = 1 5 0
$$

Next, in February $( i = 2 )$ , there is a cash requirement of $100. In addition, principal plus interest of 1.01x<sub>1</sub> is due on the line of credit and $1 . 0 0 3 z _ { 1 }$ is received on the invested excess funds. To meet the requirement in February, the company can draw an amount $x _ { 2 }$ from its line of credit and issue an amount $y _ { 2 }$ of commercial paper. So, the cash flow balance equation for February is as follows. 

$$
x _ {2} + y _ {2} - 1. 0 1 x _ {1} + 1. 0 0 3 z _ {1} - z _ {2} = 1 0 0
$$

## 3.1. SHORT TERM FINANCING

Similarly, for March we get the following equation: 

$$
x _ {3} + y _ {3} - 1. 0 1 x _ {2} + 1. 0 0 3 z _ {2} - z _ {3} = - 2 0 0
$$

For the months of April, May, and June, issuing a commercial paper is no longer an option, so we will not have variables $y _ { 4 } , \ y _ { 5 }$ , and $y _ { 6 }$ in the formulation. Furthermore, any commercial paper issued between January and March requires a payment with 2% interest 3 months later. Thus, we have the following additional equations: 

$$
\begin{array}{ccccccccc}x _ {4} & - & 1. 0 2 y _ {1} & - & 1. 0 1 x _ {3} & + & 1. 0 0 3 z _ {3} & - & z _ {4} & = & 2 0 0 \\ x _ {5} & - & 1. 0 2 y _ {2} & - & 1. 0 1 x _ {4} & + & 1. 0 0 3 z _ {4} & - & z _ {5} & = & - 5 0 \\ & - & 1. 0 2 y _ {3} & - & 1. 0 1 x _ {5} & + & 1. 0 0 3 z _ {5} & - & v & = & - 3 0 0 \end{array}
$$

Note that $x _ { i }$ is the balance on the credit line in month $i ,$ not the incremental borrowing in month $i .$ Similarly, $z _ { i }$ represents the overall excess funds in month i. This choice of variables is quite convenient when it comes to writing down the upper bound and nonnegativity constraints. 

$$
\begin{array}{r c l} {0} & {\leq} & {x _ {i} \leq 1 0 0} \\ {y _ {i}} & {\geq} & {0} \\ {z _ {i}} & {\geq} & {0.} \end{array}
$$

Final Model. This gives us the complete model of this problem: 

max v 

$$
\begin{array}{ccccccccc}x _ {1} & + & y _ {1} &  &  &  & - & z _ {1} & = & 1 5 0 \\ x _ {2} & + & y _ {2} & - & 1. 0 1 x _ {1} & + & 1. 0 0 3 z _ {1} & - & z _ {2} & = & 1 0 0 \\ x _ {3} & + & y _ {3} & - & 1. 0 1 x _ {2} & + & 1. 0 0 3 z _ {2} & - & z _ {3} & = & - 2 0 0 \\ x _ {4} & - & 1. 0 2 y _ {1} & - & 1. 0 1 x _ {3} & + & 1. 0 0 3 z _ {3} & - & z _ {4} & = & 2 0 0 \\ x _ {5} & - & 1. 0 2 y _ {2} & - & 1. 0 1 x _ {4} & + & 1. 0 0 3 z _ {4} & - & z _ {5} & = & - 5 0 \\  & - & 1. 0 2 y _ {3} & - & 1. 0 1 x _ {5} & + & 1. 0 0 3 z _ {5} & - & v & = & - 3 0 0 \\ x _ {1} & \leq & 1 0 0 &  &  &  &  &  &  &  &  \\ x _ {2} & \leq & 1 0 0 &  &  &  &  &  &  &  &  \\ x _ {3} & \leq & 1 0 0 &  &  &  &  &  &  &  &  \\ x _ {4} & \leq & 1 0 0 &  &  &  &  &  &  &  &  \\ x _ {5} & \leq & 1 0 0 &  &  &  &  &  &  &  &  \\ x _ {i}, y _ {i}, z _ {i} & \geq & 0. \end{array}
$$

Formulating a problem as a linear program means going through the above process of clearly defining the decision variables, objective, and constraints. 

Exercise 3.1 How would the formulation of the short-term financing problem above change if the commercial papers issued had a 2 month maturity instead of 3? 


Exercise 3.2 A company will face the following cash requirements in the next eight quarters (positive entries represent cash needs while negative entries represent cash surpluses).


<table><tr><td>Q1</td><td>Q2</td><td>Q3</td><td>Q4</td><td>Q5</td><td>Q6</td><td>Q7</td><td>Q8</td></tr><tr><td>100</td><td>500</td><td>100</td><td>-600</td><td>-500</td><td>200</td><td>600</td><td>-900</td></tr></table>

The company has three borrowing possibilities. 

a 2-year loan available at the beginning of Q1, with a 1% interest per quarter. 

The other two borrowing opportunities are available at the beginning of every quarter: a 6-month loan with a 1.8% interest per quarter, and a quarterly loan with a 2.5% interest for the quarter. 

Any surplus can be invested at a 0.5% interest per quarter. 

Formulate a linear program that maximizes the wealth of the company at the beginning of Q9. 

Exercise 3.3 A home buyer in France can combine several mortgage loans to finance the purchase of a house. Given borrowing needs B and a horizon of T months for paying back the loans, the home buyer would like to minimize his total cost (or equivalently, the monthly payment p made during each of the next $T$ months). Regulations impose limits on the amount that can be borrowed from certain sources. There are n diferent loan opportunities available. Loan i has a fixed interest rate $\boldsymbol { r } _ { i } ,$ a length $T _ { i } \le T$ and a maximum amount borrowed $b _ { i } .$ . The monthly payment on loan i is not required to be the same every month, but a minimum payment $m _ { i }$ is required each month. However the total monthly payment p over all loans is constant. Formulate a linear program that finds a combination of loans that minimizes the home buyer’s cost of borrowing. [Hint: In addition to variables $x _ { t i }$ for the payment on loan i in month t, it may be useful to introduce a variable for the amount of outstanding principal on loan i in month t.] 

## 3.1.2 Solving the Model with SOLVER

Special computer programs can be used to find solutions to linear programming models. The most widely available program is undoubtedly SOLVER, included in all recent versions of the Excel spreadsheet program. Here are other suggestions: 

MATLAB has a linear programming solver that can be accessed with the command linprog. Type help linprog to find out details. 

Even if one does not have access to any linear programming software, it is possible to solve linear programs (and other optimization problems) using the website http://www-neos.mcs.anl.gov/neos/ 

## 3.1. SHORT TERM FINANCING

This is the website for the Network Enabled Optimization Server. Using the JAVA submission tool on this site, one can submit a linear programming problem (in some standard format) and have a remote computer solve his/her problem using one of the several solver options. The solution is then transmitted to the submitting person by e-mail. 

A good open source LP code written in C is CLP available from the following website at the time of this writing: http://www.coin-or.org/ 

SOLVER, while not a state of the art code (which can cost upwards of $10,000 per copy) is a reasonably robust, easy-to-use tool for linear programming. SOLVER uses standard spreadsheets together with an interface to define variables, objective, and constraints. 

Here are a brief outline and some hints and shortcuts on how to create a SOLVER spreadsheet: 

Start with a spreadsheet that has all of the data entered in some reasonably neat way. 

In the short term financing example, the spreadsheet might contain the cash flows, interest rates and credit limit. 

The model will be created in a separate part of the spreadsheet. Identify one cell with each decision variable. SOLVER will eventually put the optimal values in these cells. 

In the short term financing example, we could associate cells $B$2 to $B$6 with variables $x _ { 1 }$ to $x _ { 5 }$ respectively, cells $C$2 to $C$4 with the $y _ { i }$ variables, cells $D$2 to $D$6 with the $z _ { i }$ variables and, finally, $E$2 with the variable v. 

A separate cell represents the objective. Enter a formula that represents the objective. 

For the short term financing example, we might assign cell $B$8 to the objective function. Then, in cell $B$8, we enter the function = $E$2. 

This formula must be a linear formula, so, in general, it must be of the form: cell1*cell1’ + cell2*cell2’ + ..., where cell1, cell2 and so on contain constant values and cell1’, cell2’ and so on are the decision variable cells. 

We then have a cell to represent the left hand side of each constraint (again a linear function) and another cell to represent the right hand side (a constant). 

In the short term financing example, cells $B$10 to $B$15 might contain the amounts generated through financing, for each month, and cells $D$10 to $D$15 the cash requirements for each month. For example, cell $B$10 would contain the function = $C$2 + $B$2 -$D$2 and cell $D$10 the value 150. Similarly, rows 16 to 20 could be used to write the credit limit constraints. 

Helpful Hint: Excel has a function sumproduct() that is designed for linear programs. sumproduct(a1..a10,b1..b10) is identical to a1*b1+a2*b2+a3*b3+...+a10*b10. This function can save much time and aggravation. All that is needed is that the length of the first range be the same as the length of the second range (so one can be horizontal and the other vertical). 

Helpful Hint: It is possible to assign names to cells and ranges (under the Insert-Name menu). Rather than use a1..a10 as the variables, you can name that range var (for example) and then use var wherever a1..a10 would have been used. 

We then select Solver under the Tools menu. This gives a form to fill out to define the linear program. 

In the ‘‘Set Cell’’ box, select the objective cell. Choose Maximize or Minimize. 

In the ‘‘By Changing Cells’’, put in the range containing the variable cells. 

We next add the constraints. Press the ‘‘Add...’’ button to add constraints. The dialog box has three parts for the left hand side, the type of constraint, and the right hand side. Put the cell references for a constraint in the form, choose the right type, and press ‘‘Add’’. Continue until all constraints are added. On the final constraint, press ‘‘OK’’. 

Helpful Hint: It is possible to include ranges of constraints, as long as they all have the same type. c1..e1 <= c3..e3 means c1 <= c3, d1 <= d3, e1 <= e3. a1..a10 >= 0 means each individual cell must be greater than or equal to 0. 

Push the options button and toggle the ‘‘Assume Linear Model’’ in the resulting dialog box. This tells Excel to call a linear rather than a nonlinear programming routine so as to solve the problem more eficiently. This also gives you sensitivity ranges, which are not available for nonlinear models. 

Note that, if you want your variables to assume nonnegative values only, you need to specify this in the options box (alternatively, you can add nonnegativity constraints in the previous step, in your constraints). 

Push the Solve button. In the resulting dialog box, select ‘‘Answer’’ and ‘‘Sensitivity’’. This will put the answer and sensitivity analysis in two new sheets. Ask Excel to ‘‘Keep Solver values’’, and your worksheet will be updated so that the optimal values are in the variable cells. 

Exercise 3.4 Solve the linear program formulated in Exercise 3.2 with your favorite software package. 

## 3.1.3 Interpreting the output of SOLVER

If we were to solve the short-term financing problem above using SOLVER, the solution is given in the ‘‘Answer’’ report that looks as follows. 


Target Cell (Max)


<table><tr><td>Cell</td><td>Name</td><td>Original Value</td><td>Final Value</td></tr><tr><td>$B$8</td><td>Objective</td><td>0</td><td>92.49694915</td></tr></table>

<table><tr><td colspan="4">Adjustable Cells</td></tr><tr><td>Cell</td><td>Name</td><td>Original Value</td><td>Final Value</td></tr><tr><td>$B$2</td><td>x1</td><td>0</td><td>0</td></tr><tr><td>$B$3</td><td>x2</td><td>0</td><td>50.98039216</td></tr><tr><td>$B$4</td><td>x3</td><td>0</td><td>0</td></tr><tr><td>$B$5</td><td>x4</td><td>0</td><td>0</td></tr><tr><td>$B$6</td><td>x5</td><td>0</td><td>0</td></tr><tr><td>$C$2</td><td>y1</td><td>0</td><td>150</td></tr><tr><td>$C$3</td><td>y2</td><td>0</td><td>49.01960784</td></tr><tr><td>$C$4</td><td>y3</td><td>0</td><td>203.4343636</td></tr><tr><td>$D$2</td><td>z1</td><td>0</td><td>0</td></tr><tr><td>$D$3</td><td>z2</td><td>0</td><td>0</td></tr><tr><td>$D$4</td><td>z3</td><td>0</td><td>351.9441675</td></tr><tr><td>$D$5</td><td>z4</td><td>0</td><td>0</td></tr><tr><td>$D$6</td><td>z5</td><td>0</td><td>0</td></tr><tr><td>$E$2</td><td>v</td><td>0</td><td>92.49694915</td></tr></table>


Constraints


<table><tr><td>Cell</td><td>Name</td><td>Cell Value</td><td>Formula</td><td>Slack</td></tr><tr><td>$B$10</td><td>January</td><td>150</td><td>$B$10 = $D$10</td><td>0</td></tr><tr><td>$B$11</td><td>February</td><td>100</td><td>$B$11 = $D$11</td><td>0</td></tr><tr><td>$B$12</td><td>March</td><td>-200</td><td>$B$12 = $D$12</td><td>0</td></tr><tr><td>$B$13</td><td>April</td><td>200</td><td>$B$13 = $D$13</td><td>0</td></tr><tr><td>$B$14</td><td>May</td><td>-50</td><td>$B$14 = $D$14</td><td>0</td></tr><tr><td>$B$15</td><td>June</td><td>-300</td><td>$B$15 = $D$15</td><td>0</td></tr><tr><td>$B$16</td><td>x1limit</td><td>0</td><td>$B$16 &lt;= $D$16</td><td>100</td></tr><tr><td>$B$17</td><td>x2limit</td><td>50.98039216</td><td>$B$17 &lt;= $D$17</td><td>49.01960784</td></tr><tr><td>$B$18</td><td>x3limit</td><td>0</td><td>$B$18 &lt;= $D$18</td><td>100</td></tr><tr><td>$B$19</td><td>x4limit</td><td>0</td><td>$B$19 &lt;= $D$19</td><td>100</td></tr><tr><td>$B$20</td><td>x5limit</td><td>0</td><td>$B$20 &lt;= $D$20</td><td>100</td></tr></table>

This report is fairly easy to read: the company’s wealth v in June will be $92,497. This is reported in Final Value of the Objective (recall that our units are in $1000). To achieve this, the company will issue $150,000 in commercial paper in January, $49,020 in February and $203,434 in March. In addition, it will draw $50,980 from its line of credit in February. Excess cash of $351,944 in March will be invested for just one month. All this is reported in the Adjustable Cells section of the report. For this particular application, the Constraints section of the report does not contain anything useful. On the other hand, very useful information can be found in the sensitivity report. This will be discussed in Section 3.3. 

Exercise 3.5 Formulate and solve the variation of the short-term financing problem you developed in Exercise 3.1 using SOLVER. Interpret the solution. 

Exercise 3.6 Recall Example 2.1. Solve the problem using your favorite linear programming solver. Compare the output provided by the solver to the solution we obtained in Chapter 2. 

## 3.1.4 Modeling Languages

Linear programs can be formulated using modeling languages such as AMPL, GAMS, MOSEL or OPL. The need for these modeling languages arises because the Excel spreadsheet format becomes inadequate when the size of the linear program increases. A modeling language lets people use common notation and familiar concepts to formulate optimization models and examine solutions. Most importantly, large problems can be formulated in a compact way. Once the problem has been formulated using a modeling language, it can be solved using any number of solvers. A user can switch between solvers with a single command and select options that may improve solver performance. The short term financing model would be formulated as follows (all variables are assumed to be nonnegative unless otherwise specified). 

```txt
DATA
LET T=6 be the number of months to plan for
L(t) = Liability in month t=1,...,T
ratex = monthly interest rate on line of credit
ratey = 3-month interest rate on commercial paper
ratez = monthly interest rate on excess funds
VARIABLES
x(t) = Amount drawn from line of credit in month t
y(t) = Amount of commercial paper issued in month t
z(t) = Excess funds in month t
OBJECTIVE (Maximize wealth in June)
Max z(6)
CONSTRAINTS
Month(t=1:T): x(t) - (1+ratex)*x(t-1) + y(t) - (1+ratey)*y(t-3)
-z(t) + (1+ratez)*z(t-1) = L(t)
Month(t=1:T-1): x(t) < 100 
```

Boundary conditions on x: $x(0)=x(6)=0$ Boundary conditions on y: $y(-2)=y(-1)=y(0)=y(4)=y(5)=y(6)=0$ Boundary conditions on z: $z(0)=0$ END 

Exercise 3.7 Formulate the linear program of Exercise 3.3 with one of the modeling languages AMPL, GAMS, MOSEL or OPL. 

## 3.1.5 Features of Linear Programs

Hidden in each linear programming formulation are a number of assumptions. The usefulness of an LP model is directly related to how closely reality matches up with these assumptions. 

The first two assumptions are due to the linear form of the objective and constraint functions. The contribution to the objective of any decision variable is proportional to the value of the decision variable. Similarly, the contribution of each variable to the left hand side of each constraint is proportional to the value of the variable. This is the Proportionality Assumption. 

Furthermore, the contribution of a variable to the objective and constraints is independent of the values of the other variables. This is the Additivity Assumption. When additivity or proportionality assumptions are not satisfied, a nonlinear programming model may be more appropriate. We discuss such models in Chapters 5 and 6. 

The next assumption is the Divisibility Assumption: is it possible to take any fraction of any variable? A fractional production quantity may be worrisome if we are producing a small number of battleships or be innocuous if we are producing millions of paperclips. If the Divisibility Assumption is important and does not hold, then a technique called integer programming rather than linear programming is required. This technique takes orders of magnitude more time to find solutions but may be necessary to create realistic solutions. We discuss integer programming models and methods in Chapters 11 and 12. 

The final assumption is the Certainty Assumption: linear programming allows for no uncertainty about the input parameters such as the cash-flow requirements or interest rates we used in the short-term financing model. Problems with uncertain parameters can be addressed using stochastic programming or robust optimization approaches. We discuss such models in Chapters 16 through 20. 

It is very rare that a problem will meet all of the assumptions exactly. That does not negate the usefulness of a model. A model can still give useful managerial insight even if reality difers slightly from the rigorous requirements of the model. 

Exercise 3.8 Give an example of an optimization problem where the proportionality assumption is not satisfied. 

Exercise 3.9 Give an example of an optimization problem where the additivity assumption is not satisfied. 

Exercise 3.10 Consider the LP model we develop for the cash-flow matching problem in Section 3.2. Which of the linear programming assumptions used for this formulation is the least realistic one? Why? 

## 3.2 Dedication

Dedication or cash flow matching is a technique used to fund known liabilities in the future. The intent is to form a portfolio of assets whose cash inflows will exactly ofset the cash outflows of the liabilities. The liabilities will therefore be paid of, as they come due, without the need to sell or buy assets in the future. The portfolio is formed today and then held until all liabilities are paid of. Dedicated portfolios usually only consist of riskfree non-callable bonds since the portfolio future cash inflows need to be known when the portfolio is constructed. This eliminates interest rate risk completely. It is used by some municipalities and small pension funds. For example, municipalities sometimes want to fund liabilities stemming from bonds they have issued. These pre-refunded municipal bonds can be taken of the books of the municipality. This may allow them to evade restrictive covenants in the bonds that have been pre-refunded and perhaps allow them to issue further debt. 

It should be noted however that dedicated portfolios cost typically from 3% to 7% more in dollar terms than do “immunized” portfolios that are constructed based on matching present value, duration and convexity of the assets and of the liabilities. The present value of the liability stream $L _ { t }$ for $t = 1 , \dots , T$ is $\begin{array} { r } { P = \sum _ { t = 1 } ^ { T } \frac { L _ { t } } { ( 1 + r _ { t } ) ^ { t } } } \end{array}$ , where $r _ { t }$ denotes the risk-free rate in year t. Its duration is $\begin{array} { r } { D \ = \ \frac { 1 } { P } \sum _ { t = 1 } ^ { T } \frac { t L _ { t } } { ( 1 + r _ { t } ) ^ { t } } } \end{array}$ and its convexity is $C =$ $\begin{array} { r } { \frac { 1 } { P } \sum _ { t = 1 } ^ { T } \frac { t ( t + 1 ) L _ { t } } { ( 1 + r _ { t } ) ^ { t + 2 } } } \end{array}$ . Intuitively, duration is the average (discounted) time at which the liabilities occur, whereas convexity, a bit like variance, indicates how concentrated the cash flows are over time. For a portfolio that consists only of risk-free bonds, the present value $P ^ { * }$ of the portfolio future cash inflows can be computed using the same risk-free rate $r _ { t }$ (this would not be the case for a portfolio containing risky bonds). Similarly for the duration $D ^ { * }$ and convexity $C ^ { * }$ of the portfolio future cash inflows. An “immunized” portfolio can be constructed based on matching $P ^ { * } = P , D ^ { * } = D$ and $C ^ { * } = C$ . Portfolios that are constructed by matching these three factors are immunized against parallel shifts in the yield curve, but there may still be a great deal of exposure and vulnerability to other types of shifts, and they need to be actively managed, which can be costly. By contrast, dedicated portfolios do not need to be managed after they are constructed. 

When municipalities use cash flow matching, the standard custom is to call a few investment banks, send them the liability schedule and request bids. The municipality then buys its securities from the bank that ofers the lowest price for a successful cash flow match. 

## 3.2. DEDICATION

Assume that a bank receives the following liability schedule: 

<table><tr><td>Year 1</td><td>Year 2</td><td>Year 3</td><td>Year 4</td><td>Year 5</td><td>Year 6</td><td>Year 7</td><td>Year 8</td></tr><tr><td>12,000</td><td>18,000</td><td>20,000</td><td>20,000</td><td>16,000</td><td>15,000</td><td>12,000</td><td>10,000</td></tr></table>

The bonds available for purchase today (Year 0) are given in the next table. All bonds have a face value of $100. The coupon figure is annual. For example, Bond 5 costs $98 today, and it pays back $4 in Year 1, $4 in Year 2, $4 in Year 3 and $104 in Year 4. All these bonds are widely available and can be purchased in any quantities at the stated price. 

<table><tr><td>Bond</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td><td>9</td><td>10</td></tr><tr><td>Price</td><td>102</td><td>99</td><td>101</td><td>98</td><td>98</td><td>104</td><td>100</td><td>101</td><td>102</td><td>94</td></tr><tr><td>Coupon</td><td>5</td><td>3.5</td><td>5</td><td>3.5</td><td>4</td><td>9</td><td>6</td><td>8</td><td>9</td><td>7</td></tr><tr><td>MaturityYear</td><td>1</td><td>2</td><td>2</td><td>3</td><td>4</td><td>5</td><td>5</td><td>6</td><td>7</td><td>8</td></tr></table>

Formulate and solve a linear program to find the least cost portfolio of bonds to purchase today, to meet the obligations of the municipality over the next eight years. To eliminate the possibility of any reinvestment risk, we assume a 0% reinvestment rate. 

Using a modeling language, the formulation might look as follows. 

```prolog
DATA
LET T=8 be the number of years to plan for.
LET N=10 be the number of bonds available for purchase today.
L(t) = Liability in year t=1,...,T
P(i) = Price of bond i, i=1,...,N
C(i) = Annual coupon for bond i, i=1,...,N
M(i) = Maturity year of bond i, i=1,...,N
VARIABLES
x(i) = Amount of bond i in the portfolio
z(t) = Surplus at the end of year t, for t=0,...,T
OBJECTIVE (Minimize cost)
Min z(0) + SUM(i=1:N) P(i)*x(i)
CONSTRAINTS Year(t=1:T):
SUM(i=1:N | M(i) > t-1) C(i)*x(i) + SUM(i=1:N | M(i) = t) 100*x(i)
-z(t) + z(t-1) = L(t)
END 
```

Exercise 3.11 Solve the dedication linear program above using an LP software package and verify that we can optimally meet the municipality’s liabilities for $93,944 with the following portfolio: 62 Bond1, 125 Bond3, 152 Bond4, 157 Bond5, 123 Bond6, 124 Bond8, 104 Bond9 and 93 Bond10. 


Exercise 3.12 A small pension fund has the following liabilities (in million dollars):


<table><tr><td>Year1</td><td>Year2</td><td>Year3</td><td>Year4</td><td>Year5</td><td>Year6</td><td>Year7</td><td>Year8</td><td>Year9</td></tr><tr><td>24</td><td>26</td><td>28</td><td>28</td><td>26</td><td>29</td><td>32</td><td>33</td><td>34</td></tr></table>


It would like to construct a dedicated bond portfolio. The bonds available for purchase are the following:


<table><tr><td>Bond</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td></tr><tr><td>Price</td><td>102.44</td><td>99.95</td><td>100.02</td><td>102.66</td><td>87.90</td><td>85.43</td><td>83.42</td><td>103.82</td></tr><tr><td>Coupon</td><td>5.625</td><td>4.75</td><td>4.25</td><td>5.25</td><td>0.00</td><td>0.00</td><td>0.00</td><td>5.75</td></tr><tr><td>MaturityYear</td><td>1</td><td>2</td><td>2</td><td>3</td><td>3</td><td>4</td><td>5</td><td>5</td></tr></table>

<table><tr><td>Bond</td><td>9</td><td>10</td><td>11</td><td>12</td><td>13</td><td>14</td><td>15</td><td>16</td></tr><tr><td>Price</td><td>110.29</td><td>108.85</td><td>109.95</td><td>107.36</td><td>104.62</td><td>99.07</td><td>103.78</td><td>64.66</td></tr><tr><td>Coupon</td><td>6.875</td><td>6.5</td><td>6.625</td><td>6.125</td><td>5.625</td><td>4.75</td><td>5.5</td><td>0.00</td></tr><tr><td>MaturityYear</td><td>6</td><td>6</td><td>7</td><td>7</td><td>8</td><td>8</td><td>9</td><td>9</td></tr></table>


Formulate an LP that minimizes the cost of the dedicated portfolio, assuming a 2% reinvestment rate. Solve the LP using your favorite software package.


## 3.3 Sensitivity Analysis for Linear Programming

The optimal solution to a linear programming model is the most important output of LP solvers, but it is not the only useful information they generate. Most linear programming packages produce a tremendous amount of sensitivity information, or information about what happens when data values are changed. 

Recall that in order to formulate a problem as a linear program, we had to invoke a certainty assumption: we had to know what value the data took on, and we made decisions based on that data. Often this assumption is somewhat dubious: the data might be unknown, or guessed at, or otherwise inaccurate. How can we determine the efect on the optimal decisions if the values change? Clearly some numbers in the data are more important than others. Can we find the “important” numbers? Can we determine the efect of estimation errors? 

Linear programming ofers extensive capabilities for addressing these questions. We give examples of how to interpret the SOLVER output. To access the information in SOLVER, one can simply ask for the sensitivity report after optimizing. Rather than simply giving rules for reading the reports, we show how to answer a set of questions from the output. 

## 3.3.1 Short Term Financing

The Solver sensitivity report looks as follows. 


Adjustable Cells


<table><tr><td>Cell</td><td>Name</td><td>Final Value</td><td>Reduced Cost</td><td>Objective Coefficient</td><td>Allowable Increase</td><td>Allowable Decrease</td></tr><tr><td>$B$2</td><td>x1</td><td>0</td><td>-0.0032</td><td>0</td><td>0.0032</td><td>1E+30</td></tr><tr><td>$B$3</td><td>x2</td><td>50.98</td><td>0</td><td>0</td><td>0.0032</td><td>0</td></tr><tr><td>$B$4</td><td>x3</td><td>0</td><td>-0.0071</td><td>0</td><td>0.0071</td><td>1E+30</td></tr><tr><td>$B$5</td><td>x4</td><td>0</td><td>-0.0032</td><td>0</td><td>0.0032</td><td>1E+30</td></tr><tr><td>$B$6</td><td>x5</td><td>0</td><td>0</td><td>0</td><td>0</td><td>1E+30</td></tr><tr><td>$C$2</td><td>y1</td><td>150</td><td>0</td><td>0</td><td>0.0040</td><td>0.0032</td></tr><tr><td>$C$3</td><td>y2</td><td>49.02</td><td>0</td><td>0</td><td>0</td><td>0.0032</td></tr><tr><td>$C$4</td><td>y3</td><td>203.43</td><td>0</td><td>0</td><td>0.0071</td><td>0</td></tr><tr><td>$D$2</td><td>z1</td><td>0</td><td>-0.0040</td><td>0</td><td>0.0040</td><td>1E+30</td></tr><tr><td>$D$3</td><td>z2</td><td>0</td><td>-0.0071</td><td>0</td><td>0.0071</td><td>1E+30</td></tr><tr><td>$D$4</td><td>z3</td><td>351.94</td><td>0</td><td>0</td><td>0.0039</td><td>0.0032</td></tr><tr><td>$D$5</td><td>z4</td><td>0</td><td>-0.0039</td><td>0</td><td>0.0039</td><td>1E+30</td></tr><tr><td>$D$6</td><td>z5</td><td>0</td><td>-0.007</td><td>0</td><td>0.007</td><td>1E+30</td></tr><tr><td>$E$2</td><td>v</td><td>92.50</td><td>0</td><td>1</td><td>1E+30</td><td>1</td></tr></table>


Constraints


<table><tr><td>Cell</td><td>Name</td><td>Final Value</td><td>Shadow Price</td><td>Constraint R.H.Side</td><td>Allowable Increase</td><td>Allowable Decrease</td></tr><tr><td>$B$10</td><td>January</td><td>150</td><td>-1.0373</td><td>150</td><td>89.17</td><td>150</td></tr><tr><td>$B$11</td><td>February</td><td>100</td><td>-1.030</td><td>100</td><td>49.020</td><td>50.980</td></tr><tr><td>$B$12</td><td>March</td><td>-200</td><td>-1.020</td><td>-200</td><td>90.683</td><td>203.434</td></tr><tr><td>$B$13</td><td>April</td><td>200</td><td>-1.017</td><td>200</td><td>90.955</td><td>204.044</td></tr><tr><td>$B$14</td><td>May</td><td>-50</td><td>-1.010</td><td>-50</td><td>50</td><td>52</td></tr><tr><td>$B$15</td><td>June</td><td>-300</td><td>-1</td><td>-300</td><td>92.497</td><td>1E+30</td></tr><tr><td>$B$16</td><td>x1</td><td>0</td><td>0</td><td>100</td><td>1E+30</td><td>100</td></tr><tr><td>$B$17</td><td>x2</td><td>50.98</td><td>0</td><td>100</td><td>1E+30</td><td>49.020</td></tr><tr><td>$B$18</td><td>x3</td><td>0</td><td>0</td><td>100</td><td>1E+30</td><td>100</td></tr><tr><td>$B$19</td><td>x4</td><td>0</td><td>0</td><td>100</td><td>1E+30</td><td>100</td></tr><tr><td>$B$20</td><td>x5</td><td>0</td><td>0</td><td>100</td><td>1E+30</td><td>100</td></tr></table>

The key columns for sensitivity analysis are the Reduced Cost and Shadow Price columns in SOLVER. The shadow price u of a constraint C has the following interpretation: 

If the right hand side of the constraint C changes by an amount $\Delta ,$ the optimal objective value changes by u∆, as long as the amount of change $\Delta$ is within the allowable range. 

For a linear program, the shadow price u is an exact figure, as long as the amount of change $\Delta$ is within the allowable range given in the last two columns of the SOLVER output. When the change $\Delta$ falls outside this range, the rate of change in the optimal objective value changes and the shadow price u cannot be used. When this occurs, one has to resolve the linear program using the new data. 

Next, we consider several examples of sensitivity questions and demonstrate how they can be answered using shadow prices and reduced costs. 

For example, assume that Net Cash Flow in January were -200 (instead of - 150). By how much would the company’s wealth decrease at the end of June? 

The answer is in the shadow price of the January constraint, $u \ =$ 1.0373. The RHS of the January constraint would go from 150 to 200, an increase of $\Delta \ : = \ : 5 0$ , which is within the allowable increase (89.17). So the company’s wealth in June would decrease by 1.0373 * $5 0 , 0 0 0 = \$ 51, 8 6 5$ 

Now assume that Net Cash Flow in March were 250 (instead of 200). By how much would the company’s wealth increase at the end of June? Again, the change $\Delta = - 5 0$ is within the allowable decrease (203.434), so we can use the shadow price $u = - 1 . 0 2$ to calculate the change in objective value. The increase is $( - 1 . 0 2 ) \mathrm { ~ } ^ { * } \mathrm { ~ } ( - 5 0 ) = \mathfrak { H H } , 0 0 0$ 

Assume that the credit limit were increased from 100 to 200. By how much would the company’s wealth increase at the end of June? 

In each month, the change $\Delta = 1 0 0$ is within the allowable increase $( \mathbf { \Gamma } + \infty )$ and the shadow price for the credit limit constraint is $u = 0 .$ So there is no efect on the company’s wealth in June. Note that non-binding constraints–such as the credit limit constraint for months January through May–always have zero shadow price. 

Assume that the negative Net Cash Flow in January is due to the purchase of a machine worth $150,000. The vendor allows the payment to be made in June at an interest rate of 3% for the 5-month period. Would the company’s wealth increase or decrease by using this option? What if the interest rate for the 5-month period were 4%? 

The shadow price of the January constraint is -1.0373. This means that reducing cash requirements in January by $1 increases the wealth in June by $1.0373. In other words, the break even interest rate for the 5-month period is 3.73%. So, if the vendor charges 3%, we should accept, but if he charges 4% we should not. Note that the analysis is valid since the amount $\Delta = - 1 5 0$ is within the allowable decrease. 

Now, let us consider the reduced costs. The basic variables always have a zero reduced cost. The nonbasic variables (which by definition take the value 0) have a nonpositive reduced cost and, frequently their reduced cost is strictly negative. There are two useful interpretations of the reduced cost $c ,$ for a nonbasic variable x. 

First, assume that x is set to a positive value ∆ instead of its optimal value 0. Then, the objective value is changed by $c \Delta$ . For example, what would be the efect of financing part of the January cash needs through the line of credit? The answer is in the reduced cost of variable $x _ { 1 }$ . Because this reduced cost -0.0032 is strictly negative, the objective function would decrease. Specifically, each dollar financed through the line of credit in January would result in a decrease of $0.0032 in the company’s wealth v in June. 

The second interpretation of c is that its magnitude c is the minimum amount by which the objective coeficient of x must be increased in order for the variable x to become positive in an optimal solution. For example, consider the variable x<sub>1</sub> again. Its value is zero in the current optimal solution, with objective function v. However, if we changed the objective to $v + 0 . 0 0 3 2 x _ { 1 }$ , it would now be optimal to use the line of credit in January. In other words, the reduced cost on x<sub>1</sub> can be viewed as the minimum rebate that the bank would have to ofer (payable in June) to make it attractive to use the line of credit in January. 

Exercise 3.13 Recall Example 2.1. Determine the shadow price and reduced cost information for this problem using an LP software package. How would the solution change if the average maturity of the portfolio is required to be 3.3 instead of 3.6? 

Exercise 3.14 Generate the sensitivity report for Exercise 3.2 with your favorite LP solver. 

(i) Suppose the cash requirement in Q2 is 300 (instead of 500). How would this afect the wealth in Q9? 

(ii) Suppose the cash requirement in Q2 is 100 (instead of 500). Can the sensitivity report be used to determine the wealth in Q9? 

(iii) One of the company’s suppliers may allow difered payments of $ 50 from Q3 to Q4. What would be the value of this? 


Exercise 3.15 Workforce Planning: Consider a restaurant that is open seven days a week. Based on past experience, the number of workers needed on a particular day is given as follows:


<table><tr><td>Day</td><td>Mon</td><td>Tue</td><td>Wed</td><td>Thu</td><td>Fri</td><td>Sat</td><td>Sun</td></tr><tr><td>Number</td><td>14</td><td>13</td><td>15</td><td>16</td><td>19</td><td>18</td><td>11</td></tr></table>

Every worker works five consecutive days, and then takes two days of, repeating this pattern indefinitely. How can we minimize the number of workers that staf the restaurant? 

Let the days be numbers 1 through 7 and let x be the number of workers who begin their five day shift on day i. The linear programming formulation is as follows. 

$$
\begin{array}{l c l} \text {Minimize} & \sum_ {i} x _ {i} \\ \text {Subject to} & \\ x _ {1} + x _ {4} + x _ {5} + x _ {6} + x _ {7} & \geq & 1 4 \\ x _ {1} + x _ {2} + x _ {5} + x _ {6} + x _ {7} & \geq & 1 3 \\ x _ {1} + x _ {2} + x _ {3} + x _ {6} + x _ {7} & \geq & 1 5 \\ x _ {1} + x _ {2} + x _ {3} + x _ {4} + x _ {7} & \geq & 1 6 \\ x _ {1} + x _ {2} + x _ {3} + x _ {4} + x _ {5} & \geq & 1 9 \\ x _ {2} + x _ {3} + x _ {4} + x _ {5} + x _ {6} & \geq & 1 8 \\ x _ {3} + x _ {4} + x _ {5} + x _ {6} + x _ {7} & \geq & 1 1 \\ x _ {i} & \geq & 0 (\text {for all i}) \end{array}
$$

Sensitivity Analysis The following table gives the sensitivity report for the solution of the workforce planning problem. 

<table><tr><td>Cell</td><td>Name</td><td>Final Value</td><td>Reduced Cost</td><td>Objective Coefficient</td><td>Allowable Increase</td><td>Allowable Decrease</td></tr><tr><td>$B$14</td><td>Shift1</td><td>4</td><td>0</td><td>1</td><td>0.5</td><td>1</td></tr><tr><td>$B$15</td><td>Shift2</td><td>7</td><td>0</td><td>1</td><td>0</td><td>0.333333</td></tr><tr><td>$B$16</td><td>Shift3</td><td>1</td><td>0</td><td>1</td><td>0.5</td><td>0</td></tr><tr><td>$B$17</td><td>Shift4</td><td>4</td><td>0</td><td>1</td><td>0.5</td><td>0</td></tr><tr><td>$B$18</td><td>Shift5</td><td>3</td><td>0</td><td>1</td><td>0</td><td>0.333333</td></tr><tr><td>$B$19</td><td>Shift6</td><td>3</td><td>0</td><td>1</td><td>0.5</td><td>1</td></tr><tr><td>$B$20</td><td>Shift7</td><td>0</td><td>0.333333</td><td>1</td><td>1E+30</td><td>0.333333</td></tr></table>

<table><tr><td>Cell</td><td>Name</td><td>Final Value</td><td>Shadow Price</td><td>Constraint R.H. Side</td><td>Allowable Increase</td><td>Allowable Decrease</td></tr><tr><td>$B$24</td><td>Monday</td><td>14</td><td>0.333333</td><td>14</td><td>1.5</td><td>6</td></tr><tr><td>$B$25</td><td>Tuesday</td><td>17</td><td>0</td><td>13</td><td>4</td><td>1E+30</td></tr><tr><td>$B$26</td><td>Wednesday</td><td>15</td><td>0.333333</td><td>15</td><td>6</td><td>3</td></tr><tr><td>$B$27</td><td>Thursday</td><td>16</td><td>0</td><td>16</td><td>3</td><td>4</td></tr><tr><td>$B$28</td><td>Friday</td><td>19</td><td>0.333333</td><td>19</td><td>4.5</td><td>3</td></tr><tr><td>$B$29</td><td>Saturday</td><td>18</td><td>0.333333</td><td>18</td><td>1.5</td><td>6</td></tr><tr><td>$B$30</td><td>Sunday</td><td>11</td><td>0</td><td>11</td><td>4</td><td>1</td></tr></table>

Answer each of the following questions independently of the others. 

1. What is the current total number of workers needed to staf the restaurant? 

2. Due to a special ofer, demand on Thursdays increases. As a result, 18 workers are needed instead of 16. What is the efect on the total number of workers needed to staf the restaurant? 

3. Assume that demand on Mondays decreases: 11 workers are needed instead of 14. What is the efect on the total number of workers needed to staf the restaurant? 

4. Every worker in the restaurant is paid $1000 per month. So the objective function in the formulation can be viewed as total wage expenses (in thousand dollars). Workers have complained that Shift 4 is the least desirable shift. Management is considering increasing the wages of workers on Shift 4 to $1100. Would this change the optimal solution? What would be the efect on total wage expenses? 

5. Shift 2, on the other hand, is very desirable (Sundays of while on duty Fridays and Saturdays, which are the best days for tips). Management is considering reducing the wages of workers on Shift 1 to $900 per month. Would this change the optimal solution? What would be the efect on total wage expenses? 

6. Management is considering introducing a new shift with the days of on Tuesdays and Sundays. Because these days are not consecutive, the wages will be $1200 per month. Will this increase or reduce the total wage expenses? 

## 3.3.2 Dedication

We end this section with the sensitivity report of the dedication problem formulated in Section 3.2. 


Adjustable Cells


<table><tr><td>Cell</td><td>Name</td><td>Final Value</td><td>Reduced Cost</td><td>Objective Coefficient</td><td>Allowable Increase</td><td>Allowable Decrease</td></tr><tr><td>$B$5</td><td>x1</td><td>62.13612744</td><td>0</td><td>102</td><td>3</td><td>5.590909091</td></tr><tr><td>$B$6</td><td>x2</td><td>0</td><td>0.830612245</td><td>99</td><td>1E+30</td><td>0.830612245</td></tr><tr><td>$B$7</td><td>x3</td><td>125.2429338</td><td>0</td><td>101</td><td>0.842650104</td><td>3.311081442</td></tr><tr><td>$B$8</td><td>x4</td><td>151.5050805</td><td>0</td><td>98</td><td>3.37414966</td><td>4.712358277</td></tr><tr><td>$B$9</td><td>x5</td><td>156.8077583</td><td>0</td><td>98</td><td>4.917243419</td><td>17.2316607</td></tr><tr><td>$B$10</td><td>x6</td><td>123.0800686</td><td>0</td><td>104</td><td>9.035524153</td><td>3.74817022</td></tr><tr><td>$B$11</td><td>x7</td><td>0</td><td>8.786840002</td><td>100</td><td>1E+30</td><td>8.786840002</td></tr><tr><td>$B$12</td><td>x8</td><td>124.1572748</td><td>0</td><td>101</td><td>3.988878399</td><td>8.655456271</td></tr><tr><td>$B$13</td><td>x9</td><td>104.0898568</td><td>0</td><td>102</td><td>9.456887408</td><td>0.860545483</td></tr><tr><td>$B$14</td><td>x10</td><td>93.45794393</td><td>0</td><td>94</td><td>0.900020046</td><td>1E+30</td></tr><tr><td>$H$4</td><td>z0</td><td>0</td><td>0.028571429</td><td>1</td><td>1E+30</td><td>0.028571429</td></tr><tr><td>$H$5</td><td>z1</td><td>0</td><td>0.055782313</td><td>0</td><td>1E+30</td><td>0.055782313</td></tr><tr><td>$H$6</td><td>z2</td><td>0</td><td>0.03260048</td><td>0</td><td>1E+30</td><td>0.03260048</td></tr><tr><td>$H$7</td><td>z3</td><td>0</td><td>0.047281187</td><td>0</td><td>1E+30</td><td>0.047281187</td></tr><tr><td>$H$8</td><td>z4</td><td>0</td><td>0.179369792</td><td>0</td><td>1E+30</td><td>0.179369792</td></tr><tr><td>$H$9</td><td>z5</td><td>0</td><td>0.036934059</td><td>0</td><td>1E+30</td><td>0.036934059</td></tr><tr><td>$H$10</td><td>z6</td><td>0</td><td>0.086760435</td><td>0</td><td>1E+30</td><td>0.086760435</td></tr><tr><td>$H$11</td><td>z7</td><td>0</td><td>0.008411402</td><td>0</td><td>1E+30</td><td>0.008411402</td></tr><tr><td>$H$12</td><td>z8</td><td>0</td><td>0.524288903</td><td>0</td><td>1E+30</td><td>0.524288903</td></tr></table>

## Constraints

<table><tr><td>Cell</td><td>Name</td><td>Final Value</td><td>Shadow Price</td><td>Constraint R.H.Side</td><td>Allowable Increase</td><td>Allowable Decrease</td></tr><tr><td>$B$19</td><td>year1</td><td>12000</td><td>0.971428571</td><td>12000</td><td>1E+30</td><td>6524.293381</td></tr><tr><td>$B$20</td><td>year2</td><td>18000</td><td>0.915646259</td><td>18000</td><td>137010.161</td><td>13150.50805</td></tr><tr><td>$B$21</td><td>year3</td><td>20000</td><td>0.883045779</td><td>20000</td><td>202579.3095</td><td>15680.77583</td></tr><tr><td>$B$22</td><td>year4</td><td>20000</td><td>0.835764592</td><td>20000</td><td>184347.1716</td><td>16308.00686</td></tr><tr><td>$B$23</td><td>year5</td><td>16000</td><td>0.6563948</td><td>16000</td><td>89305.96314</td><td>13415.72748</td></tr><tr><td>$B$24</td><td>year6</td><td>15000</td><td>0.619460741</td><td>15000</td><td>108506.7452</td><td>13408.98568</td></tr><tr><td>$B$25</td><td>year7</td><td>12000</td><td>0.532700306</td><td>12000</td><td>105130.9798</td><td>11345.79439</td></tr><tr><td>$B$26</td><td>year8</td><td>10000</td><td>0.524288903</td><td>10000</td><td>144630.1908</td><td>10000</td></tr></table>

Exercise 3.16 Analyze the solution tables above and 

Interpret the shadow price in year $t \left( t = 1 , \dots , 8 \right)$ 

Interpret the reduced cost of bond i $( i = 1 , \ldots , 1 0 )$ 

Interpret the reduced cost of each surplus variable $z _ { t } ~ ( t = 0 , \ldots , 7 )$ 

## Answers:

The shadow price in Year t is the cost of the bond portfolio that can be attributed to a dollar of liability in Year t. For example, each dollar of liability in Year 3 is responsible for $ 0.883 in the cost of the bond portfolio. Note that, by setting the shadow price in Year t equal to $\displaystyle \frac { 1 } { ( 1 + r _ { t } ) ^ { t } }$ , we get a term structure of interest rates. Here $r _ { 3 } = 0 . 0 4 2 3$ . In Figure 3.3.2 we plot the term structure of interest rates we compute from this solution. How does this compare with the term structure of Treasury rates? 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/1416deb967eacea3b54defb3bfcdefcf4fdfe3f23366388c5f7e5697662a0c37.jpg)



Figure 3.1: Interest rates implied by shadow prices


The reduced cost of bond i indicates by how much bond i is overpriced for inclusion in the optimal portfolio. For example, bond 2 would have to be $ 0.83 lower, at $ 98.17, for inclusion in the optimal portfolio. 

Exercise 3.17 Note that the optimal solution has no holdings in Bond 7 which matures in Year 5, despite the $16,000 liability in Year 5. This is likely due to a mispricing of this bond at $100. What would be a more realistic price for this bond? 

Answer: Row 7 of the “Adjustable Cells” table indicates that variable x<sub>7</sub>, corresponding to Bond 7 holdings, will become positive only if the price is reduced by 8.786 or more. So, a more realistic price for this bond would be just above $91. By checking the reduced costs, one may sometimes spot errors in the data! 

The reduced cost of the surplus variable $z _ { t }$ indicates what the interest rate on cash reinvested in Year t would have to be in order to keep excess cash in Year t. 

Exercise 3.18 Generate the sensitivity report for Exercise 3.12. 

(i) Suppose that the liability in Year 3 is 29 (instead of 28). What would be the increase in cost of the dedicated portfolio? 

(ii) Draw a graph of the term structure of interest rates implied by the shadow prices. 

(iii) Bond 4 is not included in the optimal portfolio. By how much would the price of Bond 4 have to decrease for Bond 4 to become part of the optimal portfolio? 

(iv) The fund manager would like to have 10000 units of Bond 3 in the portfolio. By how much would this increase the cost of the portfolio? 

(v) Is there any bond that looks badly mispriced? 

(vi) What interest rate on cash would make it optimal to include cash as part of the optimal portfolio? 

## 3.4 Case Study

We are currently in year i. A municipality sends you the following liability stream (in million dollars) in years i + 1 to $i + 8 i$ 

<table><tr><td>6/15/i+1</td><td>12/15/i+1</td><td>6/15/i+2</td><td>12/15/i+2</td><td>6/15/i+3</td><td>12/15/i+3</td></tr><tr><td>6</td><td>6</td><td>9</td><td>9</td><td>10</td><td>10</td></tr></table>

<table><tr><td>6/15/i+4</td><td>12/15/i+4</td><td>6/15/i+5</td><td>12/15/i+5</td><td>6/15/i+6</td><td>12/15/i+6</td></tr><tr><td>10</td><td>10</td><td>8</td><td>8</td><td>8</td><td>8</td></tr></table>

<table><tr><td>6/15/i+7</td><td>12/15/i+7</td><td>6/15/i+8</td><td>12/15/i+8</td></tr><tr><td>6</td><td>6</td><td>5</td><td>5</td></tr></table>

Your job: 

Value the liability using the Treasury curve. 

Identify between 30 and 50 assets that are suitable for a dedicated portfolio (non-callable bonds, treasury bills or notes). Explain why they are suitable. You can find current data on numerous web sites such as www.bondsonline.com 

Set up a linear program to identify a lowest cost dedicated portfolio of assets (so no short selling) and solve with Excel’s solver (or any other linear programming software that you prefer). What is the cost of your portfolio? Discuss the composition of your portfolio. Discuss the assets and the liabilities in light of the Sensitivity Report. What is the term structure of interest rates implied by the shadow prices? Compare with the term structure of Treasury rates. (Hint: refer to Section 3.3.2.) 

## 3.4. CASE STUDY

Set up a linear program to identify a lowest cost portfolio of assets (no short selling) that matches present value, duration and convexity (or a related measure) between the liability stream and the bond portfolio. Solve the linear program with your favorite software. Discuss the solution. How much would you save by using this immunization strategy instead of dedication? Can you immunize the portfolio against nonparallel shifts of the yield curve? Explain. 

Set up a linear program to identify a lowest cost portfolio of assets (no short selling) that combines a cash matching strategy for the liabilities in the first 3 years and an immunization strategy based on present value, duration and convexity for the liabilities in the last 5 years. Compare the cost of this portfolio with the cost of the two previous portfolios. 

The municipality would like you to make a second bid: what is your lowest cost dedicated portfolio of riskfree bonds if short sales are allowed? Discuss the feasibility of your solution. 

66CHAPTER 3. LP MODELS: ASSET/LIABILITY CASH FLOW MATCHING 

## Chapter 4

# LP Models: Asset Pricing and Arbitrage

## 4.1 Derivative Securities and The Fundamental Theorem of Asset Pricing

One of the most widely studied problems in financial mathematics is the pricing of derivative securities, also known as contingent claims. These are securities whose price depends on the value of another underlying security. Financial options are the most common examples of derivative securities. For example, a European call option gives the holder the right to purchase an underlying security for a prescribed amount (called the strike price) at a prescribed time in the future, known as the expiration or exercise date. The exercise date is also known as the maturity date of the derivative security. Recall the similar definitions of European put options as well as American call and put options from Section 1.3.2. 

Options are used mainly for two purposes: speculation and hedging. By speculating on the direction of the future price movements of the underlying security, investors can take (bare) positions in options on this security. Since options are often much cheaper than their underlying security, this bet results in much larger earnings in relative terms if the price movements happen in the expected direction compared to what one might earn by taking a similar position in the underlying. Of course, if one guesses the direction of the price movements incorrectly, the losses are also much more severe. 

The more common and sensible use of options is for hedging. Hedging refers to the reduction of risk in an investor’s overall position by forming a suitable portfolio of assets that are expected to have opposing risks. For example, if an investor holds a share of XYZ and is concerned that the price of this security may fall significantly, she can purchase a put option on XYZ and protect herself against price levels below a certain threshold–the strike price of the put option. 

Recall the option example in the simple one-period binomial model of Section 1.3.2. Below, we summarize some of the information from that example: 

We consider the share price of XYZ stock which is currently valued at $40. A month from today, we expect the share price of XYZ to either double or halve, with equal probabilities. We also consider a European call option on XYZ with a strike price of $50 which will expire a month from today. The payof function for the call is shown in Figure 4.1. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/d90c0f36becca2380abd2f83fcc9a49f92309679096f56a73f3e7ccb9f5d6bd5.jpg)



Figure 4.1: Piecewise linear payof function for a call option


We assume that interest rates for cash borrowing or lending are zero and that any amount of XYZ shares can be bought or sold with no commission. 

$$
S _ {0} = 4 0 \quad \begin{array}{l} 8 0 = S _ {1} (u) \\ 2 0 = S _ {1} (d) \end{array} \quad \text { and } C _ {0} = ? \quad \begin{array}{l} (8 0 - 5 0) ^ {+} = 3 0 \\ (2 0 - 5 0) ^ {+} = 0 \end{array}
$$

In Section 1.3.2 we obtained a fair price of $10 for the option using a replication strategy and the no-arbitrage principle. Two portfolios of securities that have identical future payofs under all possible realizations of the random states must have the same value today. In the example, the first portfolio is the option while the second one is the portfolio of $\frac { 1 } { 2 }$ share of XYZ and -$10 in cash. Since we know the current value of the second portfolio, we can deduce the fair price of the option. To formalize this approach, we first give a definition of arbitrage: 

## Definition 4.1 An arbitrage is a trading strategy

that has a positive initial cash flow and has no risk of a loss later (type $A ) _ { . }$ , or 

that requires no initial cash input, has no risk of a loss, and a positive probability of making profits in the future (type B). 

In the example, any price other than $10 for the call option would lead to a type A arbitrage–guaranteed profits at the initial time point and no future obligations. We do not need to have a guarantee of profits for $\mathrm { t y p e }$ B arbitrage–all we need is a guarantee of no loss, and a positive probability of a gain. Prices adjust quickly so that arbitrage opportunities cannot persist in the markets. Therefore, in pricing arguments it is often assumed that arbitrage opportunities do not exist. 

## 4.1.1 Replication

In the above example, we formulated and solved the following question to determine the fair price of an option: Can we form a portfolio of the underlying security (long or short) and cash (borrowed or lent) today, such that the payof of the portfolio at the expiration date of the option will match the payof of the option? In other words, can we replicate the option using a portfolio of the underlying security and cash? 

Let us work in a slightly more general setting. Let $S _ { 0 }$ be the current price of the underlying security and assume that there are two possible outcomes at the end of the period: $S _ { 1 } ^ { u } = S _ { 0 } \cdot u$ and ${ \cal S } _ { 1 } ^ { d } = { \cal S } _ { 0 } \cdot d .$ Assume $u > d .$ . We also assume that there is a fixed interest rate of r on cash positions for the given period. Let $R = 1 + r$ 

Now we consider a derivative security which has payofs of $C _ { 1 } ^ { u }$ and $C _ { 1 } ^ { d }$ in the up and down states respectively: 

$$
S _ {0} \begin{array}{c} S _ {1} ^ {u} = S _ {0} \cdot u \\ S _ {1} ^ {d} = S _ {0} \cdot d \end{array} \quad C _ {0} = ? \begin{array}{c} C _ {1} ^ {u} \\ C _ {1} ^ {d} \end{array}
$$

To price the derivative security, we will replicate its payof. For replication consider a portfolio of $\Delta$ shares of the underlying and $\$ 8$ cash. For what values of $\Delta$ and $B$ does this portfolio have the same payofs at the expiration date as the derivative security? 

In the “up” state, the replicating portfolio will have value $\Delta S _ { 0 } \cdot u + B R$ and in the “down” state it will be worth $\Delta S _ { 0 } \cdot d + B R$ . Therefore, for perfect replication, we need to solve the following simple system of equations: 

$$
\begin{array}{r c l} \Delta S _ {0} \cdot u + B R & = & C _ {1} ^ {u} \\ \Delta S _ {0} \cdot d + B R & = & C _ {1} ^ {d}. \end{array}
$$

We obtain: 

$$
\begin{array}{r c l} \Delta & = & \frac {C _ {1} ^ {u} - C _ {1} ^ {d}}{S _ {0} (u - d)} \\ B & = & \frac {u C _ {1} ^ {d} - d C _ {1} ^ {u}}{R (u - d)}. \end{array}
$$

Since this portfolio is worth $S _ { 0 } \Delta + B$ today, that should be the price of the derivative security as well: 

$$
C _ {0} = \frac {C _ {1} ^ {u} - C _ {1} ^ {d}}{u - d} + \frac {u C _ {1} ^ {d} - d C _ {1} ^ {u}}{R (u - d)}
$$

$$
= \frac {1}{R} \left[ \frac {R - d}{u - d} C _ {1} ^ {u} + \frac {u - R}{u - d} C _ {1} ^ {d} \right].
$$

## 4.1.2 Risk-Neutral Probabilities

Let 

$$
p _ {u} = \frac {R - d}{u - d} \quad \mathrm{and} \quad p _ {d} = \frac {u - R}{u - d}.
$$

Note that we must have $d < R < u$ to avoid arbitrage opportunities as indicated in the following simple exercise. 

Exercise 4.1 Let $S _ { 0 }$ be the current price of a security and assume that there are two possible prices for this security at the end of the current period: $S _ { 1 } ^ { u } = S _ { 0 } \cdot u$ and ${ \cal S } _ { 1 } ^ { d } = { \cal S } _ { 0 } \cdot d .$ (Assume $u > d . )$ Also assume that there is a fixed interest rate of r on cash positions for the given period. Let $R = 1 + r$ . Show that there is an arbitrage opportunity if $u > R > d$ is not satisfied. 

An immediate consequence of this observation is that both $p _ { u } > 0$ and $p _ { d } > 0$ . Noting also that $p _ { u } + p _ { d } = 1$ one can interpret $p _ { u }$ and $p _ { d }$ as probabilities. In fact, these are the so-called risk-neutral probabilities (RNPs) of up and down states, respectively. Note that they are completely independent from the physical probabilities of these states. 

The price of any derivative security can now be calculated as the present value of the expected value of its future payofs where the expected value is taken using the risk-neutral probabilities. 

In our example above $\textstyle u = 2 , d = { \frac { 1 } { 2 } }$ and $r = 0$ so that $R = 1$ . Therefore: 

$$
p _ {u} = \frac {1 - 1 / 2}{2 - 1 / 2} = \frac {1}{3} \quad \text {and} \quad p _ {d} = \frac {2 - 1}{2 - 1 / 2} = \frac {2}{3}.
$$

As a result, we have 

$$
\begin{array}{r c l} S _ {0} = 4 0 & = & \frac {1}{R} (p _ {u} S _ {1} ^ {u} + p _ {d} S _ {1} ^ {d}) = \frac {1}{3} 8 0 + \frac {2}{3} 2 0, \\ C _ {0} = 1 0 & = & \frac {1}{R} (p _ {u} C _ {1} ^ {u} + p _ {d} C _ {1} ^ {d}) = \frac {1}{3} 3 0 + \frac {2}{3} 0, \end{array}
$$

as expected. Using risk neutral probabilities we can also price other derivative securities on the XYZ stock. For example, consider a European put option on the XYZ stock struck at $60 and with the same expiration date as the call of the example. 

$$
P _ {0} = ? \begin{array}{c} P _ {1} ^ {u} = \max \{0, 6 0 - 8 0 \} = 0 \\ P _ {1} ^ {d} = \max \{0, 6 0 - 2 0 \} = 4 0 \end{array}
$$

We can easily compute: 

$$
P _ {0} = \frac {1}{R} (p _ {u} P _ {1} ^ {u} + p _ {d} P _ {1} ^ {d}) = \frac {1}{3} 0 + \frac {2}{3} 4 0 = \frac {8 0}{3},
$$

without needing to replicate the option again. 

Exercise 4.2 Compute the price of a binary (digital) call option on the XYZ stock that pays $1 if the XYZ price is above the strike price of $50. 

Exercise 4.3 Assume that the XYZ stock is currently priced at $40. At the end of the next period, the XYZ price is expected to be in one of the following two states: $S _ { 0 } \cdot u$ or $S _ { 0 } \cdot d .$ We know that $d < 1 < u$ but do not know d or $u .$ . The interest rate is zero. If a European call option with strike price $50 is priced at $10 while a European call option with strike price $40 is priced at $13. If we assume that these prices do not contain any arbitrage opportunities, what is the fair price of a European put option with a strike price of $40? 

Hint: First note that $u > \frac { 5 } { 4 }$ –otherwise the first call would be worthless. Then we must have $1 0 = p _ { u } ( S _ { 0 } \cdot u - 5 0 )$ and $1 3 = p _ { u } ( S _ { 0 } \cdot u - 4 0 )$ . From these equations determine $p _ { u }$ and then u and d. 

Exercise 4.4 Assume that the XYZ stock is currently priced at $40. At the end of the next period, the XYZ price is expected to be in one of the following two states: $S _ { 0 } \cdot u$ or $S _ { 0 } \cdot d .$ . We know that $d < 1 < u$ but do not know d or $u .$ The interest rate is zero. European call options on XYZ with strike prices of $30, $40, $50, and $60 are priced at $10, $7, $\$ 10$ , and $0. Which one of these options is mispriced? Why? 

Remark 4.1 Exercises $4 . 3$ and $4 . 4$ are much simplified and idealized examples of the pricing problems encountered by practitioners. Instead of a set of possible future states for prices which may be dificult to predict, they must work with a set of market prices for related securities. Then, they must extrapolate prices for an unpriced security using no-arbitrage arguments. 

Next we move from our binomial setting to a more general setting and let 

$$
\Omega = \{\omega_ {1}, \omega_ {2}, \dots , \omega_ {m} \}\tag{4.1}
$$

be the (finite) set of possible future “states”. For example, these could be prices for a security at a future date. 

For securities $S ^ { i } , i = 0 \dots n$ , let $S _ { 1 } ^ { i } ( \omega _ { j } )$ denote the price of this security in state $\omega _ { j }$ at time 1. Also let $S _ { 0 } ^ { i }$ denote the current (time 0) price of security $S ^ { i }$ . We use $i = 0$ for the “riskless” security that pays the interest rate $r \geq 0$ between time 0 and time 1. It is convenient to assume that $S _ { 0 } ^ { 0 } = 1$ and that $S _ { 1 } ^ { 0 } ( \omega _ { j } ) = R = 1 + r , \forall j$ 

Definition 4.2 A risk-neutral probability measure on the set $\Omega = \{ \omega _ { 1 } , \omega _ { 2 } , \ldots , \omega _ { m } \}$ is a vector of positive numbers $\left( p _ { 1 } , p _ { 2 } , \ldots , p _ { m } \right)$ such that 

$$
\sum_ {j = 1} ^ {m} p _ {j} = 1
$$

and for every security $S ^ { i } , i = 0 , \dots , n$ 

$$
S _ {0} ^ {i} = \frac {1}{R} \left(\sum_ {j = 1} ^ {m} p _ {j} S _ {1} ^ {i} (\omega_ {j})\right) = \frac {1}{R} \hat {\mathbf {E}} [ S _ {1} ^ {i} ].
$$

Above, $\hat { \mathbf { E } } [ S ]$ denotes the expected value of the random variable S under the probability distribution $\left( p _ { 1 } , p _ { 2 } , \ldots , p _ { m } \right)$ 

## 4.1.3 The Fundamental Theorem of Asset Pricing

In this section we state the first fundamental theorem of asset pricing and prove it for finite Ω. This proof is a simple exercise in linear programming duality that also utilizes the following well-known result of Goldman and Tucker on the existence of strictly complementary optimal solutions of LPs: 

Theorem 4.1 (Goldman and Tucker [30]) When both the primal and dual linear programming problems 

<sup>(</sup>LP<sup>)</sup> 

$$
\begin{array}{r l r} \min _ {x} & c ^ {T} x \\ & A x = b \\ & x \geq 0 \end{array}\tag{4.2}
$$

and 

<sup>(</sup>LD<sup>)</sup> 

$$
\begin{array}{r l r} \max _ {y} & b ^ {T} y \\ & A ^ {T} y \leq c, \end{array}\tag{4.3}
$$

have feasible solutions, they have optimal solutions satisfying strict complementarity, i.e., there exist $x ^ { * }$ and $y ^ { * }$ optimal for the respective problems such that 

$$
x ^ {*} + (c - A ^ {T} y ^ {*}) > 0.
$$

Now, we are ready to prove the following theorem: 

Theorem 4.2 (The First Fundamental Theorem of Asset Pricing) A risk-neutral probability measure exists if and only if there is no arbitrage. 

## Proof:

We provide the proof for the case when the state space Ω is finite and is given by (4.1). We assume without loss of generality that every state has a positive probability of occuring (since states that have no probability of occuring can be removed from Ω.) Given the current prices $S _ { 0 } ^ { i }$ and the future prices $S _ { 1 } ^ { i } ( \omega _ { j } )$ in each state $\omega _ { j }$ , for securities 0 to $n ,$ consider the following linear program with variables $x _ { i }$ , for $i = 0 , \ldots , n \colon$ 

$$
\begin{array}{r l} \min _ {x} & \sum_ {i = 0} ^ {n} S _ {0} ^ {i} x _ {i} \\ & \sum_ {i = 0} ^ {n} S _ {1} ^ {i} (\omega_ {j}) x _ {i} \geq 0, j = 1, \ldots , m. \end{array}\tag{4.4}
$$

Note that type-A arbitrage corresponds to a feasible solution to this LP with a negative objective value. Since $x = ( x _ { 1 } , \ldots , x _ { n } )$ with $x _ { i } = 0 , \forall i$ is a feasible solution, the optimal objective value is always non-positive. Furthermore, since all the constraints are homogeneous, if there exists a feasible solution such that $\sum S _ { 0 } ^ { i } x _ { i } < 0$ (this corresponds to type-A arbitrage), the problem is unbounded. In other words, there is no type-A arbitrage if and only if the optimal objective value of this LP is 0. 

Suppose that there is no type-A arbitrage. Then, there is no type-B arbitrage if and only if all constraints are tight for all optimal solutions of (4.4) since every state has a positive probability of occuring. Note that these solutions must have objective value 0. 

Consider the dual of (4.4): 

$$
\begin{array}{r c l} \max _ {p} & \sum_ {j = 1} ^ {m} 0 p _ {j} \\ & \sum_ {j = 1} ^ {m} S _ {1} ^ {i} (\omega_ {j}) p _ {j} & = S _ {0} ^ {i}, i = 0, \ldots , n, \\ & p _ {j} & \geq 0, j = 1, \ldots , m. \end{array}\tag{4.5}
$$

Since the dual objective function is constant at zero for all dual feasible solutions, any dual feasible solution is also dual optimal. 

When there is no type-A arbitrage, (4.4) has an optimal solution. Now, Theorem 2.2–Strong Duality Theorem–indicates that the dual must have a feasible solution. If there is no type-B arbitrage either, Goldman and Tucker’s theorem indicates that there exists a feasible and therefore optimal dual solution $p ^ { * }$ such that $p ^ { * } > 0$ . This follows from strict complementarity with primal constraints $\begin{array} { r } { \sum _ { i = 1 } ^ { n } S _ { 1 } ^ { i } ( \omega _ { j } ) x _ { i } \ge 0 } \end{array}$ which are tight. From the dualnconstraint corresponding to $i = 0$ , we have that $\begin{array} { r } { \sum _ { j = 1 } ^ { m } p _ { j } ^ { * } = \frac { 1 } { R } } \end{array}$ . Multiplying $p ^ { * }$ by R one obtains a risk-neutral probability distribution. Therefore, the “no arbitrage” assumption implies the existence of RNPs. 

The converse direction is proved in an identical manner. The existence of a RNP measure implies that (4.5) is feasible, and therefore its dual, (4.4) must be bounded, which implies that there is no type-A arbitrage. Furthermore, since we have a strictly feasible (and optimal) dual solution, any optimal solution of the primal must have tight constraints, indicating that there is no type-B arbitrage. 

## 4.2 Arbitrage Detection Using Linear Programming

The linear programming problems (4.4) and (4.5) formulated in the proof of Theorem 4.2 can naturally be used for detection of arbitrage opportunities. However, as we discussed above, this argument works only for finite state spaces. In this section, we discuss how LP formulations can be used to detect arbitrage opportunities without limiting consideration to finite state spaces. The price we pay for this flexibility is the restriction on the selection of the securities: we only consider the prices of a set of derivative securities written on the same underlying with same maturity. This discussion is based on Herzel [38]. 

Consider an underlying security with a current, time 0, price of $S _ { 0 }$ and a random price $S _ { 1 }$ at time 1. Consider n derivative securities written on this security that mature at time 1, and have piecewise linear payof functions $\Psi _ { i } ( S _ { 1 } )$ , each with a single breakpoint $K _ { i } ,$ , for $i = 1 , \ldots , n .$ The obvious motivation is the collection of calls and puts with diferent strike prices written on this security. If, for example, the i-th derivative security were a European call with strike price $K _ { i }$ , we would have $\Psi i ( S _ { 1 } ) = ( S _ { 1 } - K _ { i } ) ^ { + }$ We assume that the $K _ { i } \mathrm { s }$ are in increasing order, without loss of generality. Finally, let $S _ { 0 } ^ { i }$ denote the current price of the i-th derivative security. 

Consider a portfolio $x = ( x _ { 1 } , \ldots , x _ { n } ) $ of the derivative securities 1 to n and let $\Psi ^ { x } ( S _ { 1 } )$ denote the payof function of the portfolio: 

$$
\Psi^ {x} (S _ {1}) := \sum_ {i = 1} ^ {n} \Psi_ {i} (S _ {1}) x _ {i}.\tag{4.6}
$$

The cost of forming the portfolio x at time 0 is given by 

$$
\sum_ {i = 1} ^ {n} S _ {0} ^ {i} x _ {i}.\tag{4.7}
$$

To determine whether a static arbitrage opportunity exists in the current prices $S _ { 0 } ^ { i }$ , we consider the following problem: What is the cheapest portfolio of the derivative securities 1 to n whose payof function $\Psi ^ { x } ( S _ { 1 } )$ is nonnegative for all $S _ { 1 } \in [ 0 , \infty ) ?$ Non-negativity of $\Psi ^ { x } ( S _ { 1 } )$ corresponds to “no future obligations” part of the arbitrage definition. If the minimum initial cost of such a portfolio is negative, then we have a type-A arbitrage. 

Since all $\Psi _ { i } ( S _ { 1 } )$ s are piecewise linear, so is $\Psi ^ { x } ( S _ { 1 } )$ . It will have up to n breakpoints at points $K _ { 1 }$ through $K _ { n }$ . Observe that a piecewise linear function is nonnegative over $[ 0 , \infty )$ if and only if it is nonnegative at 0 and at all the breakpoints, and if the slope of the function is nonnegative to the right of the largest breakpoint. From our notation, $\Psi ^ { x } ( S _ { 1 } )$ is nonnegative for all non-negative values of $S _ { 1 }$ if and only if 

1. $\Psi ^ { x } ( 0 ) \geq 0 .$ 

2. $\Psi ^ { x } ( K _ { j } ) \geq 0 , \ \forall j$ 

3. and $[ ( \Psi ^ { x } ) _ { + } ^ { \prime } ( K _ { n } ) ] \geq 0 .$ 

Now consider the following linear programming problem: 

min<sub>x</sub> 

$$
\begin{array}{r c l} \sum_ {i = 1} ^ {n} S _ {0} ^ {i} x _ {i} & \\ \sum_ {i = 1} ^ {n} \Psi_ {i} (0) x _ {i} & \geq & 0 \\ \sum_ {i = 1} ^ {n} \Psi_ {i} (K _ {j}) x _ {i} & \geq & 0, j = 1, \ldots , n \\ \sum_ {i = 1} ^ {n} (\Psi_ {i} (K _ {n} + 1) - \Psi_ {i} (K _ {n})) x _ {i} & \geq & 0 \end{array}\tag{4.8}
$$

Since all $\Psi _ { i } ( S _ { 1 } ) \mathrm { { ' s } }$ are piecewise linear, the quantity $\Psi i ( K _ { n } + 1 ) - \Psi _ { i } ( K _ { n } )$ gives the right-derivative of $\Psi _ { i } ( S _ { 1 } )$ at $K _ { n }$ . Thus, the expression in the last constraint is the right derivative of $\Psi ^ { x } ( S _ { 1 } )$ at $K _ { n }$ . The following observation follows from our arguments above: 

Proposition 4.1 There is no type-A arbitrage in prices $S _ { 0 } ^ { i }$ if and only if the optimal objective value of $( 4 . 8 )$ is zero. 

Similar to the previous section, we have the following result: 

Proposition 4.2 Suppose that there are no type-A arbitrage opportunities in prices $S _ { 0 } ^ { i }$ . Then, there are no type-B arbitrage opportunities if and only $i f$ the dual of the problem $( 4 . 8 )$ has a strictly feasible solution. 

## 4.2. ARBITRAGE DETECTION USING LINEAR PROGRAMMING 75

Exercise 4.5 Prove Proposition 4.2. 

Next, we focus on the case where the derivative securities under consideration are European call options with strikes at $K _ { i }$ for $i = 1 , \ldots , n ,$ so that $\Psi i ( S _ { 1 } ) = ( S _ { 1 } - K _ { i } ) ^ { + }$ . Thus 

$$
\Psi_ {i} (K _ {j}) = (K _ {j} - K _ {i}) ^ {+}.
$$

In this case, (4.8) reduces to the following problem: 

$$
\begin{array}{r l} \min _ {x} & c ^ {T} x \\ & A x \geq 0, \end{array}\tag{4.9}
$$

where $c ^ { T } = [ S _ { 0 } ^ { 1 } , \ . . . , S _ { 0 } ^ { n } ]$ and 

$$
A = \left[ \begin{array}{c c c c c} K _ {2} - K _ {1} & 0 & 0 & \dots & 0 \\ K _ {3} - K _ {1} & K _ {3} - K _ {2} & 0 & \dots & 0 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ K _ {n} - K _ {1} & K _ {n} - K _ {2} & K _ {n} - K _ {3} & \dots & 0 \\ 1 & 1 & 1 & \dots & 1 \end{array} \right].\tag{4.10}
$$

This formulation is obtained by removing the first two constraints of (4.8) which are redundant in this particular case. 

Using this formulation and our earlier results, one can prove a theorem giving necessary and suficient conditions for a set of call option prices to contain arbitrage opportunities: 

Theorem 4.3 Let $K _ { 1 } < K _ { 2 } < \cdots < K _ { n }$ denote the strike prices of $E u -$ ropean call options written on the same underlying security with the same maturity. There are no arbitrage opportunities if and only if the prices $S _ { 0 } ^ { i }$ satisfy the following conditions: 

1. $S _ { 0 } ^ { i } > 0 , \ i = 1 , \dots , n$ 

2. $S _ { 0 } ^ { i } > S _ { 0 } ^ { i + 1 } , \ i = 1 , . . . , n - 1$ 

3. The function $C ( K _ { i } ) : = S _ { 0 } ^ { i }$ defined on the set $\{ K _ { 1 } , K _ { 2 } , \ldots , K _ { n } \}$ is a strictly convex function. 

Exercise 4.6 Use Proposition 4.2 to show that there are no arbitrage opportunities for the option prices in Theorem 4.3 if and only if there exists strictly positive scalars $y _ { 1 } , \ldots , y _ { n }$ satisfying $y _ { n } = S _ { 0 } ^ { n } , y _ { n - 1 } = ( S _ { 0 } ^ { n - 1 }$ $S _ { 0 } ^ { n } ) / ( K ^ { n } - K ^ { n - 1 } )$ , and 

$$
y _ {i} = \frac {S _ {0} ^ {i} - S _ {0} ^ {i + 1}}{K ^ {i + 1} - K ^ {i}} - \frac {S _ {0} ^ {i + 1} - S _ {0} ^ {i + 2}}{K ^ {i + 2} - K ^ {i + 1}}, i = 1, \ldots , n - 2.
$$

Use this observation to prove Theorem 4.3 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/a998bcb26ee6ef30a49413b7b437bad008eab72fa9eca0c822c63ea8df053703.jpg)



Figure 4.2: Nonconvexity in the call price function indicates arbitrage


As an illustration of Theorem 4.3, consider the scenario in Exercise 4.4: XYZ stock is currently priced at $40. European call options on XYZ with strike prices of $30, $40, $50, and $60 are priced at $10, $\$ 7,\ S \frac {10 } { 3 }$ , and $0. Do these prices exhibit an arbitrage opportunity? As we see in Figure 4.2, the option prices violate the third condition of the Theorem and therefore must carry an arbitrage opportunity. 

Exercise 4.7 Construct a portfolio of the options in the example above that provides a type-A arbitrage opportunity. 

## 4.3 Additional Exercises

Exercise 4.8 Consider the linear programming problem (4.9) that we developed to detect arbitrage opportunities in the prices of European call options with a common underlying security and common maturity (but diferent strike prices). This formulation implicitly assumes that the $i ^ { \mathrm { t h } }$ call can be bought or sold at the same current price of $S _ { 0 } ^ { i }$ . In real markets, there is always a gap between the price a buyer pays for a security and the amount the seller collects called the bid-ask spread. 

Assume that the ask price of the $i ^ { \mathrm { t h } }$ call is given by $S _ { a } ^ { i }$ while its bid price is denoted by $S _ { b } ^ { i }$ with $S _ { a } ^ { i } > S _ { b } ^ { i }$ . Develop an analogue of the LP (4.9) in the case where we can purchase the calls at their ask prices or sell them at their bid prices. Consider using two variables for each call option in your new LP. 

Exercise 4.9 Consider all the call options on the S&P 500 index that expire on the same day, about three months from the current date. Their current prices can be downloaded from the website of the Chicago Board of Options Exchange at www.cboe.com or several other market quote websites. Formulate the linear programming problem (4.9) (or, rather the version you developed for Exercise 4.8 since market quotes will include bid and ask prices) to determine whether these prices contain any arbitrage opportunities. Solve this linear programming problem using an LP software. 

Sometimes, illiquid securities can have misleading prices since the reported price corresponds to the last transaction in that security which may have happened several days ago, and if there were to be a new transaction, this value would change dramatically. As a result, it is quite possible that you will discover false “arbitrage opportunities” because of these misleading prices. Repeat the LP formulation and solve it again, this time only using prices of the call options that have had a trading volume of at least 100 on the day you downloaded the prices. 

Exercise 4.10 (i) You have $20,000 to invest. Stock XYZ sells at $20 per share today. A European call option to buy 100 shares of stock XYZ at $15 exactly six months from today sells for $1000. You can also raise additional funds which can be immediately invested, if desired, by selling call options with the above characteristics. In addition, a 6-month riskless zero-coupon bond with $100 face value sells for $90. You have decided to limit the number of call options that you buy or sell to at most 50. 

You consider three scenarios for the price of stock XYZ six months from today: the price will be the same as today, the price will go up to $40, or drop to $12. Your best estimate is that each of these scenarios is equally likely. Formulate and solve a linear program to determine the portfolio of stocks, bonds, and options that maximizes expected profit. 

Answer: First, we define the decision variables. 

B = number of bonds purchased, 

S = number of shares of stock XYZ purchased, 

C = number of call options purchased (if > 0) or sold (if < 0). 

The expected profits (per unit of investment) are computed as follows. 

Bonds: 10
Stock XYZ: $\frac{1}{3}(20+0-8)=4$ Call Option: $\frac{1}{3}(1500-500-1000)=0$ 

Therefore, we get the following linear programming formulation. 

```txt
max 10B + 4S
90B + 20S + 1000C ≤ 20000 (budget constraint)
C ≤ 50 (limit on number of call options purchased)
C ≥ -50 (limit on number of call options sold)
B ≥ 0, S ≥ 0 (nonnegativity). 
```

Solving (using SOLVER, say), we get the optimal solution B = 0, S = 3500, C = -50 with an expected profit of $14,000. 

Note that, with this portfolio, the profit is not positive under all scenarios. In particular, if the price of stock XYZ goes to $40, a loss of $5000 will be incurred. 

(ii) Suppose that the investor wants a profit of at least $2000 in any of the three scenarios. Write a linear program that will maximize the investor’s expected profit under this additional constraint. 

Answer: This can be done by introducing three additional variables. 

P = profit in scenario i 

The formulation is now the following. 

max 

$$
\begin{array}{c c c c c c c c} \frac {1}{3} P _ {1} & + & \frac {1}{3} P _ {2} & + & \frac {1}{3} P _ {3} \\ 9 0 B & + & 2 0 S & + & 1 0 0 0 C & \leq & 2 0 0 0 0 \\ 1 0 B & + & 2 0 S & + & 1 5 0 0 C & = & P _ {1} \\ 1 0 B & & & - & 5 0 0 C & = & P _ {2} \\ 1 0 B & - & 8 S & - & 1 0 0 0 C & = & P _ {3} \\ & & & & P _ {1} & \geq & 2 0 0 0 \\ & & & & P _ {2} & \geq & 2 0 0 0 \\ & & & & P _ {3} & \geq & 2 0 0 0 \\ & & & C & \leq & 5 0 \\ & & & C & \geq & - 5 0 \\ B \geq 0, S \geq 0. \end{array}
$$

(iii) Solve this linear program with SOLVER to find out the expected profit. 

How does it compare with the earlier figure of $14,000? 

Answer: The optimum solution is to buy 2,800 shares of XYZ and sell 36 call options. The resulting expected worth in six months will be $31,200. Therefore, the expected profit is $11,200 (=$31,200 - 20,000). 

(iv) Riskless profit is defined as the largest possible profit that a portfolio is guaranteed to earn, no matter which scenario occurs. What is the portfolio that maximizes riskless profit for the above three scenarios? 

Answer: To solve this question, we can use a slight modification of the previous model, by introducing one more variable. 

Z = riskless profit. 

Here is the formulation. 

max 

$$
\begin{array}{c c c c c c c c} Z & & & & & & \\ 9 0 B & + & 2 0 S & + & 1 0 0 0 C & \leq & 2 0 0 0 0 \\ 1 0 B & + & 2 0 S & + & 1 5 0 0 C & = & P _ {1} \\ 1 0 B & & & - & 5 0 0 C & = & P _ {2} \\ 1 0 B & - & 8 S & - & 1 0 0 0 C & = & P _ {3} \\ & & & & P _ {1} & \geq & Z \\ & & & & P _ {2} & \geq & Z \\ & & & & P _ {3} & \geq & Z \\ & & & C & \leq & 5 0 \\ & & & C & \geq & - 5 0 \\ B \geq 0, S \geq 0. \end{array}
$$

The result is (obtained using SOLVER) a riskless profit of $7272. This is obtained by buying 2,273 shares of XYZ and selling 25.45 call options. The resulting expected profit is $9,091 in this case. 

## Exercise 4.11 Arbitrage in the Currency Market

Consider the global currency market. Given two currencies, say the Yen and the USDollar, there is an exchange rate between them (about 118 Yens to the Dollar in February 2006). It is axiomatic of arbitrage-free markets that there is no method of converting, say, a Dollar to Yens then to Euros, then Pounds, and to Dollars so that you end up with more than a dollar. How would you recognize when there is an arbitrage opportunity? 

The following are actual trades made on February 14, 2002. 

<table><tr><td>from</td><td></td><td>Dollar</td><td>Euro</td><td>Pound</td><td>Yen</td></tr><tr><td rowspan="4">into</td><td>Dollar</td><td></td><td>.8706</td><td>1.4279</td><td>.00750</td></tr><tr><td>Euro</td><td>1.1486</td><td></td><td>1.6401</td><td>.00861</td></tr><tr><td>Pound</td><td>.7003</td><td>.6097</td><td></td><td>.00525</td></tr><tr><td>Yen</td><td>133.38</td><td>116.12</td><td>190.45</td><td></td></tr></table>

For example, one dollar converted into euros yielded 1.1486 euros. It is not obvious from the chart above, but in the absence of any conversion costs, the Dollar-Pound-Yen-Dollar conversion actually makes $0.0003 per dollar converted while changing the order to Dollar-Yen-Euro-Dollar loses about $0.0002 per dollar converted. How can one formulate a linear program to identify such arbitrage possibilities? 

## Answer:

VARIABLES 

DE = quantity of dollars changed into euros 

DP = quantity of dollars changed into pounds 

DY = quantity of dollars changed into yens 

ED = quantity of euros changed into dollars 

EP = quantity of euros changed into pounds 

EY = quantity of euros changed into yens 

PD = quantity of pounds changed into dollars 

PE = quantity of pounds changed into euros 

PY = quantity of pounds changed into yens 

YD = quantity of yens changed into dollars 

YE = quantity of yens changed into euros 

YP = quantity of yens changed into pounds 

D = quantity of dollars generated through arbitrage 

OBJECTIVE 

Max D 

CONSTRAINTS 

Dollar: D + DE + DP + DY - 0.8706*ED - 1.4279*PD - 0.00750*YD = 

1 

Euro: ED + EP + EY - 1.1486*DE - 1.6401*PE - .00861*YE = 0 

```txt
Pound: PD + PE + PY - 0.7003*DP - 0.6097*EP - 0.00525*YP = 0
Yen: YD + YE + YP - 133.38*DY - 116.12*EY - 190.45*PY = 0
BOUNDS
D < 10000
END 
```

Solving this linear program, we find that, in order to gain $10,000 in arbitrage, we have to change about $34 million dollars into euros, then convert these euros into yens and finally change the yens into dollars. There are other solutions as well. The arbitrage opportunity is so tiny ($0.0003 to the dollar) that, depending on the numerical precision used, some LP solvers do not find it, thus concluding that there is no arbitrage here. An interesting example illustrating the role of numerical precision in optimization solvers! 

## 4.4 Case Study: Tax Clientele Efects in Bond Portfolio Management

The goal is to construct an optimal tax-specific bond portfolio, for a given tax bracket, by exploiting the price diferential of an after-tax stream of cash flows. This objective is accomplished by purchasing at the ask price “underpriced” bonds (for the specific tax bracket), while simultaneously selling at the bid price “overpriced” bonds. The following model was proposed by E.I. Ronn [62]. See also S.M. Schaefer [64]. 

Let 

<sup>J</sup> <sup>=</sup> {<sup>1,</sup> <sup>.</sup> <sup>.</sup> <sup>.</sup> <sup>,</sup> <sup>j,</sup> <sup>.</sup> <sup>.</sup> <sup>.</sup> <sup>,</sup> <sup>N</sup>} <sup>=</sup> <sup>set</sup> <sup>of</sup> <sup>riskless</sup> <sup>bonds.</sup> 

$P _ { j } ^ { a }$ = asked price of bond j 

$P _ { j } ^ { b }$ = bid price of bond j 

$X _ { j } ^ { a }$ = amount of bond j bought 

$X _ { j } ^ { b }$ = amount of bond j sold short, and 

We make the natural assumption that $P _ { j } ^ { a } > P _ { j } ^ { b }$ . The objective function of the program is 

$$
Z = \max \sum_ {j = 1} ^ {N} P _ {j} ^ {b} X _ {j} ^ {b} - \sum_ {j = 1} ^ {N} P _ {j} ^ {a} X _ {j} ^ {a}\tag{4.11}
$$

since the long side of an arbitrage position must be established at ask prices while the short side of the position must be established at bid prices. Now consider the future cash-flows of the portfolio. 

$$
C _ {1} = \sum_ {j = 1} ^ {N} a _ {j} ^ {1} X _ {j} ^ {a} - \sum_ {j = 1} ^ {N} a _ {j} ^ {1} X _ {j} ^ {b}\tag{4.12}
$$

$$
\mathrm{For} t = 2, \ldots , T, \qquad C _ {t} = (1 + \rho) C _ {t - 1} + \sum_ {j = 1} ^ {N} a _ {j} ^ {t} X _ {j} ^ {a} - \sum_ {j = 1} ^ {N} a _ {j} ^ {t} X _ {j} ^ {b},\tag{4.13}
$$

$$
\begin{array}{r c l} \text {where} & \rho & = \text {Exogenous riskless reinvestment rate} \\ & a _ {j} ^ {t} & = \text {coupon and/or principal payment on bond j at time t.} \end{array}
$$

For the portfolio to be riskless, we require 

$$
C _ {t} \geq 0 \quad t = 1, \dots , T.\tag{4.14}
$$

Since the bid-ask spread has been explicitly modeled, it is clear that $X _ { j } ^ { a } \geq 0$ and $X _ { j } ^ { b } ~ \geq ~ 0$ are required. Now the resulting linear program admits two possible solutions. Either all bonds are priced to within the bid-ask spread, i.e. $Z = 0$ , or infinite arbitrage profits may be attained, i.e. $Z = \infty$ . Clearly any attempt to exploit price diferentials by taking extremely large positions in these bonds would cause price movements: the bonds being bought would appreciate in price; the bonds being sold short would decline in value. In order to provide a finite solution, the constraints $X _ { j } ^ { a } \leq 1$ and $X _ { j } ^ { b } \leq 1$ are imposed. Thus, with 

$$
0 \leq X _ {j} ^ {a}, X _ {j} ^ {b} \leq 1 j = 1, \ldots , N,\tag{4.15}
$$

the complete problem is now specified as (4.11)-(4.15). 

## Taxes

The proposed model explicitly accounts for the taxation of income and capital gains for specific investor classes. This means that the cash flows need to be adjusted for the presence of taxes. 

For a discount bond (i.e. when $P _ { j } ^ { a } < 1 0 0 )$ , the after-tax cash-flow of bond j in period t is given by 

$$
a _ {j} ^ {t} = c _ {j} ^ {t} (1 - \tau),
$$

$$
\begin{array}{l l} \text {where} & c _ {j} ^ {t} \quad \text {is the semiannual coupon payment} \\ \text {and} & \tau \quad \text {is the ordinary income tax rate.} \end{array}
$$

At maturity, the $j ^ { t h }$ bond yields 

$$
a _ {j} ^ {t} = (1 0 0 - P _ {j} ^ {a}) (1 - g) + P _ {j} ^ {a},
$$

where $g$ is the capital gains tax rate. 

For premium bond (i.e. when $P _ { j } ^ { a } > 1 0 0 )$ , the premium is amortized against ordinary income over the life of the bond, giving rise to an after-tax coupon payment of 

$$
a _ {j} ^ {t} = \left[ c _ {j} ^ {t} - \frac {P _ {j} ^ {a} - 1 0 0}{n _ {j}} \right] (1 - \tau) + \frac {P _ {j} ^ {a} - 1 0 0}{n _ {j}}
$$

where $n _ { j }$ is the number of coupon payments remaining to maturity. 

A premium bond also makes a nontaxable repayment of 

$$
a _ {j} ^ {t} = 1 0 0
$$

at maturity. 

## Data

The model requires that the data contain bonds with perfectly forcastable cash flows. All callable bonds are excluded from the sample. For the same reason, flower bonds of all types are excluded. Thus, all noncallable bonds and notes are deemed appropriate for inclusion in the sample. 

Major categories of taxable investors are Domestic Banks, Insurance Companies, Individuals, Nonfinancial Corporations, Foreigners. In each case, one needs to distinguish the tax rates on capital gains versus ordinary income. 

The fundamental question to arise from this study is: does the data reflect tax clientele efects or arbitrage opportunities? 

Consider first the class of tax-exempt investors. Using current data, form the optimal “purchased” and “sold” bond portfolios. Do you observe the same tax clientele efect as documented by Schaefer for British government securities; namely, the “purchased” portfolio contains high coupon bonds and the “sold” portfolio is dominated by low coupon bonds. This can be explained as follows: The preferential taxation of capital gains for (most) taxable investors causes them to gravitate towards low coupon bonds. Consequently, for tax-exempt investors, low coupon bonds are “overpriced” and not desirable as investment vehicles. 

Repeat the same analysis with the diferent types of taxable investors. Do you observe: 

1. a clientele efect in the pricing of US Government investments, with tax-exempt investors, or those without preferential treatment of capital gains, gravitating towards high coupon bonds? 

2. that not all high coupon bonds are desirable to investors without preferential treatment of capital gains? Nor are all low coupon bonds attractive to those with preferential treatment of capital gains. Can you find reasons why this may be the case? 

The dual price, say $u _ { t } .$ , associated with constraint (4.13) represents the present value of an additional dollar at time t. Explain why. It follows that $u _ { t }$ may be used to compute the term structure of spot interest rates $R _ { t }$ 2 given by the relation 

$$
R _ {t} = \left(\frac {1}{u _ {t}}\right) ^ {\frac {1}{t}} - 1.
$$

Compute this week’s term structure of spot interest rates for tax-exempt investors. 

# Nonlinear Programming: Theory and Algorithms

## 5.1 Introduction

So far, we focused on optimization problems with linear constraints and a linear objective function. Linear functions are “nice”–they are smooth and predictable. Consequently, we were able to use specialized and highly eficient techniques for their solution. Many realistic formulations of optimization problems however, do not fit into this nice structure and require more general methods. In this chapter we study general optimization problems of the form 

$$
\begin{array}{r c l} (\mathcal {O P}) & \min _ {x} & f (x) \\ & g _ {i} (x) & = 0, i \in \mathcal {E} \\ & g _ {i} (x) & \geq 0, i \in \mathcal {I}. \end{array}\tag{5.1}
$$

where $f$ and $g _ { i }$ are functions of $R ^ { n } \to \mathbb { R } .$ , and are index sets for the equality and inequality constraints respectively. Such optimization problems are often called nonlinear programming problems, or nonlinear programs. 

There are many problems where the general framework of nonlinear programming is needed. Here are some illustrations: 

1. Economies of scale: In many applications costs or profits do not grow linearly with the corresponding activities. In portfolio construction, an individual investor may benefit from economies of scale as fixed costs of trading become negligible for larger trades. Conversely, an institutional investor may sufer from diseconomies of scale if a large trade has an unfavorable market impact on the security traded. Realistic models of such trades must involve nonlinear objective or constraint functions. 

2. Probabilistic elements: Nonlinearities frequently arise when some of the coeficients in the model are random variables. For example, consider a linear program where the right–hand sides are random. To illustrate, suppose the LP has two constraints: 

maximize 

$$
\begin{array}{r c l} {c _ {1} x _ {1} + \ldots + c _ {n} x _ {n}} \\ {a _ {1 1} x _ {1} + \ldots + a _ {1 n} x _ {n}} & \leq & {b _ {1}} \\ {a _ {2 1} x _ {1} + \ldots + a _ {2 n} x _ {n}} & \leq & {b _ {2}} \end{array}
$$

where the coeficients $b _ { 1 }$ and $b _ { 2 }$ are independently distributed and $G _ { i } ( y )$ represents the probability that the random variable $b _ { i }$ is at least as large as ${ \mathrm { y } } .$ Suppose you want to select the variable $x _ { 1 } , \ldots , x _ { n }$ so that the joint probability of both the constraints being satisfied is at least $\beta \colon$ 

$$
P \left[ a _ {1 1} x _ {1} + \dots + a _ {1 n} x _ {n} \leq b _ {1} \right] \times P \left[ a _ {2 1} x _ {1} + \dots + a _ {2 n} x _ {n} \leq b _ {2} \right] \geq \beta .
$$

Then this condition can be written as the following set of constraints: 

$$
\begin{array}{r c l} - y _ {1} & + & a _ {1 1} x _ {1} + \ldots + a _ {1 n} x _ {n} = 0 \\ - y _ {2} & + & a _ {2 1} x _ {1} + \ldots + a _ {2 n} x _ {n} = 0 \\ & & G _ {1} (y _ {1}) \times G _ {2} (y _ {2}) \geq \beta , \end{array}
$$

where this product leads to nonlinear restrictions on $y _ { 1 }$ and $y _ { 2 }$ . 

3. Value-at-Risk: The Value-at-Risk is a risk measure that focuses on rare events. For example, for a random variable X that represents daily loss from an investment portfolio, VaR would be the largest loss that occurs with a specified frequency such as once per year. Given a probability level $\alpha ,$ say $\alpha = 0 . 9 9$ , the Value-at-Risk $\operatorname { V a R } _ { \alpha } ( X )$ of a random variable X with a continuous distribution function is the value $\gamma$ such that $P ( X \leq \gamma ) = \alpha$ As such, VaR focuses on the tail of the distribution of the random variable X. Depending on the distributional assumptions for portfolio returns, the problem of finding a portfolio that minimizes VaR can be a highly nonlinear optimization problem. 

4. Mean-Variance Optimization: Markowitz’s MVO model introduced in Section 1.3.1 is a quadratic program: the objective function is quadratic and the constraints are linear. In Chapter 7 we will present an interior point algorithm for this class of nonlinear optimization problems. 

5. Constructing an index fund: In integer programming applications, such as the model discussed in Section 12.3 for constructing an index fund, the “relaxation” can be written as a multivariate function that is convex but non-diferentiable. Subgradient techniques can be used to solve this class of nonlinear optimization problems. 

In contrast to linear programming, where the simplex method can handle most instances and reliable implementations are widely available, there is not a single preferred algorithm for solving general nonlinear programs. Without dificulty, one can find ten or fifteen methods in the literature and the underlying theory of nonlinear programming is still evolving. A systematic comparison between diferent methods and packages is complicated by the fact that a nonlinear method can be very efective for one type of problem and yet fail miserably for another. In this chapter, we sample a few ideas: 

1. the method of steepest descent for unconstrained optimization, 

2. Newton’s method, 

3. the generalized reduced-gradient algorithm, 

4. sequential quadratic programming, 

5. subgradient optimization for nondiferentiable functions. 

We address the solution of two special classes of nonlinear optimization problems, namely quadratic and conic optimization problems in Chapters 7 and 9. For these problem classes, interior-point methods (IPMs) are very efective. While IPMs are heavily used for general nonlinear programs also, we delay their discussion until Chapter 7. 

## 5.2 Software

Some software packages for solving nonlinear programs are: 

1. CONOPT, GRG2, Excel’s SOLVER (all three are based on the generalized reduced-gradient algorithm), 

2. MATLAB optimization toolbox, SNOPT, NLPQL (sequential quadratic programming), 

3. MINOS, LANCELOT (Lagrangian approach), 

4. LOQO, MOSEK, IPOPT (Interior point algorithms for the KKT conditions, see Section 5.5). 

The Network Enabled Optimization Server (NEOS) website we already mentioned in Chapter 2 and available at 

$$
\mathrm{http://www-neos.mcs.anl.gov/neos}
$$

provides access to many academic and commercial nonlinear optimization solvers. In addition, the Optimization Software Guide based on the book by Mor´e and Wright [52] and available from 

http://www-fp.mcs.anl.gov/otc/Guide/SoftwareGuide 

lists information on more than 30 nonlinear programming packages. 

Of course, as is the case for linear programming, you will need a modeling language to work eficiently with large nonlinear models. Two of the most popular are GAMS and AMPL. Most of the optimizers described above accept models written in either of these mathematical programming languages. 

## 5.3 Univariate Optimization

Before discussing optimization methods for multivariate and or constrained problems, we start with a description of methods for solving univariate equations and optimizing univariate functions. These methods, often called line search methods are important components to many nonlinear programming algorithms. 

## 5.3.1 Binary search

Binary search is a very simple idea for numerically solving the nonlinear equation $f ( x ) = 0$ , where f is a function of a single variable. 

For example, suppose we want to find the maximum of $g ( x ) = 2 x ^ { 3 } - e ^ { x }$ For this purpose we need to identify the critical points of the function, namely, those points that satisfy the equation $g ^ { \prime } ( x ) = 6 x ^ { 2 } - e ^ { x } = 0$ . But there is no closed form solution to this equation. So we solve the equation numerically, through binary search. Letting $f ( x ) : = g ^ { \prime } ( x ) = 6 x ^ { 2 } - e ^ { x }$ , we first look for two points, say $a , b ,$ such that the signs of $f ( a )$ and $f ( b )$ are opposite. Here $a = 0$ and $b = 1$ would do since $f ( 0 ) = - 1$ and $f ( 1 ) \approx 3 . 3$ Since f is continuous, we know that there exists an x with $0 < x < 1$ such that $f ( x ) = 0$ . We say that our confidence interval is [0,1]. Now let us try the middle point $x = 0 . 5$ . Since $f ( 0 . 5 ) \approx - 0 . 1 5 < 0$ we know that there is a solution between 0.5 and 1 and we get the new confidence interval [0.5, 1.0]. We continue with $x = 0 . 7 5$ and since $f ( 0 . 7 5 ) > 0$ we get the confidence interval $[ 0 . 5 , 0 . 7 5 ]$ . Repeating this, we converge very quickly to a value of x where $f ( x ) = 0$ . Here, after 10 iterations, we are within 0.001 of the real value. 

In general, if we have a confidence interval of $[ a , b ]$ , we evaluate $\textstyle f ( { \frac { a + b } { 2 } } )$ to cut the confidence interval in half. 

Binary search is fast. It reduces the confidence interval by a factor of 2 for every iteration, so after k iterations the original interval is reduced to $( b - a ) \times 2 ^ { - k }$ . A drawback is that binary search only finds one solution. So, if g had local extrema in the above example, binary search could converge to any of them. In fact, most algorithms for nonlinear programming are subject to failure for this reason. 

Example 5.1 Binary search can be used to compute the internal rate of return $\left( I R R \right) r$ of an investment. Mathematically, r is the interest rate that satisfies the equation 

$$
\frac {F _ {1}}{1 + r} + \frac {F _ {2}}{(1 + r) ^ {2}} + \frac {F _ {3}}{(1 + r) ^ {3}} + \dots + \frac {F _ {N}}{(1 + r) ^ {N}} - C = 0
$$

where 

$F_{t}$ = cash flow in year $t$ $N$ = number of years $C$ = cost of the investment 

## 5.3. UNIVARIATE OPTIMIZATION

For most investments, the above equation has a unique solution and therefore the IRR is uniquely defined, but one should keep in mind that this is not always the case. The IRR of a bond is called its yield. As an example, consider a 4-year non-callable bond with a 10% coupon rate paid annually and a par value of $1000. Such a bond has the following cash flows: 

<table><tr><td>In Yr. t</td><td><eq>F_t</eq></td></tr><tr><td>1</td><td>$ 100</td></tr><tr><td>2</td><td>100</td></tr><tr><td>3</td><td>100</td></tr><tr><td>4</td><td>1100</td></tr></table>

Suppose this bond is now selling for $900. Compute the yield of this bond. 

The yield r of the bond is given by the equation 

$$
\frac {1 0 0}{1 + r} + \frac {1 0 0}{(1 + r) ^ {2}} + \frac {1 0 0}{(1 + r) ^ {3}} + \frac {1 1 0 0}{(1 + r) ^ {4}} - 9 0 0 = 0
$$

Let us denote by $f ( r )$ the left-hand-side of this equation. We find r such that $f ( r ) = 0$ using binary search. 

We start by finding values $( a , b )$ such that $f ( a ) \ > \ 0$ and $f ( b ) < 0$ In this case, we expect $r$ to be between 0 and 1. Since $f ( 0 ) = 5 0 0$ and $f ( 1 ) = - 7 4 3 . 7 5$ , we have our starting values. 

Next, we let $c = 0 . 5$ (the midpoint) and calculate $f ( c )$ . Since $f ( 0 . 5 ) =$ $- 5 4 1 . 9 7 5$ , we replace our range with $a = 0$ and $b = 0 . 5$ and repeat. When we continue, we get the following table of values: 


Table 5.1: Binary search to find the IRR of a non-callable bond


<table><tr><td>Iter.</td><td>a</td><td>c</td><td>b</td><td>f(a)</td><td>f(c)</td><td>f(b)</td></tr><tr><td>1</td><td>0</td><td>0.5</td><td>1</td><td>500</td><td>-541.975</td><td>-743.75</td></tr><tr><td>2</td><td>0</td><td>0.25</td><td>0.5</td><td>500</td><td>-254.24</td><td>-541.975</td></tr><tr><td>3</td><td>0</td><td>0.125</td><td>0.25</td><td>500</td><td>24.85902</td><td>-254.24</td></tr><tr><td>4</td><td>0.125</td><td>0.1875</td><td>0.25</td><td>24.85902</td><td>-131.989</td><td>-254.24</td></tr><tr><td>5</td><td>0.125</td><td>0.15625</td><td>0.1875</td><td>24.85902</td><td>-58.5833</td><td>-131.989</td></tr><tr><td>6</td><td>0.125</td><td>0.140625</td><td>0.15625</td><td>24.85902</td><td>-18.2181</td><td>-58.5833</td></tr><tr><td>7</td><td>0.125</td><td>0.132813</td><td>0.140625</td><td>24.85902</td><td>2.967767</td><td>-18.2181</td></tr><tr><td>8</td><td>0.132813</td><td>0.136719</td><td>0.140625</td><td>2.967767</td><td>-7.71156</td><td>-18.2181</td></tr><tr><td>9</td><td>0.132813</td><td>0.134766</td><td>0.136719</td><td>2.967767</td><td>-2.39372</td><td>-7.71156</td></tr><tr><td>10</td><td>0.132813</td><td>0.133789</td><td>0.134766</td><td>2.967767</td><td>0.281543</td><td>-2.39372</td></tr><tr><td>11</td><td>0.133789</td><td>0.134277</td><td>0.134766</td><td>0.281543</td><td>-1.05745</td><td>-2.39372</td></tr><tr><td>12</td><td>0.133789</td><td>0.134033</td><td>0.134277</td><td>0.281543</td><td>-0.3883</td><td>-1.05745</td></tr></table>

According to this computation the yield of the bond is approximately r = 13.4%. Of course, this routine sort of calculation can be easily implemented on a computer. 

Exercise 5.1 Find a root of the polynomial $f ( x ) = 5 x ^ { 4 } - 2 0 x + 2$ in the interval [0,1] using binary search. 

Exercise 5.2 Compute the yield on a 6-year non-callable bond that makes 5% coupon payments in years 1,3, and 5, coupon payments of $1 0 \%$ in years 2 and 4, and pays the par value in year 6. 

Exercise 5.3 The well-known Black-Scholes-Merton option pricing formula has the following form for European call option prices: 

$$
{ C ( K , T ) } { = } { S _ { 0 } \Phi ( d _ { 1 } ) - K e ^ { - r T } \Phi ( d _ { 2 } ) , }
$$

where 

$$
\begin{array}{r c l} {d _ {1}} & = & {\frac {\log (\frac {S _ {0}}{K}) + (r + \frac {\sigma^ {2}}{2}) T}{\sigma \sqrt {T}},} \\ {d _ {2}} & = & {d _ {1} - \sigma \sqrt {T},} \end{array}
$$

and $\Phi ( \cdot )$ is the cumulative distribution function for the standard normal distribution. r in the formula represents the continuously compounded risk-free and constant interest rate and $\sigma$ is the volatility of the underlying security that is assumed to be constant. Given the market price of a particular option and an estimate for the interest rate $^ { r , }$ the unique value of the volatility parameter σ that satisfies the pricing equation above is called the implied volatility of the underlying security. Calculate the implied volatility of a stock currently valued at $20 if a European call option on this stock with a strike price of $18 and a maturity of 3 months is worth $2.20. Assume a zero interest rate and use binary search. 

## Golden Section Search

Golden section search is similar in spirit to binary search. It can be used to solve a univariate equation as above, or to compute the maximum of a function $f ( x )$ defined on an interval $[ a , b ]$ . The discussion here is for the optimization version. The main diference between the golden section search and the binary search is in the way the new confidence interval is generated from the old one. 

We assume that 

(i) f is continuous 

(ii) f has a unique local maximum in the interval $[ a , b ]$ 

The golden search method consists in computing $f ( c )$ and $\operatorname { f } ( \mathrm { d } )$ for $a \textless$ d $< c < b$ 

If $f ( c ) > f ( d )$ , the procedure is repeated with the interval $( a , b )$ replaced by (d, b). 

If $f ( c ) < f ( d )$ , the procedure is repeated with the interval $( a , b )$ replaced by $( a , c )$ 

## 5.3. UNIVARIATE OPTIMIZATION

Remark 5.1 The name “golden section” comes from a certain choice of c and d that yields fast convergence, namely $c = a + r ( b - a )$ and $d = b + r ( a - b )$ where $\begin{array} { r } { r = \frac { \sqrt { 5 } - 1 } { 2 } = . 6 1 8 0 3 4 . . . . } \end{array}$ This is the golden ratio, already known to the ancient Greeks. 

Example 5.2 Find the maximum of the function $x ^ { 5 } - 1 0 x ^ { 2 } + 2 x$ in the interval [0, 1]. 

In this case, we begin with $a = 0$ and $b = 1$ . Using golden section search, that gives $d = 0 . 3 8 2$ and $c = 0 . 6 1 8$ . The function values are $f ( a ) = 0$ 2 $f ( d ) = - 0 . 6 8 7 , f ( c ) = - 2 . 4 9 3$ , and $f ( b ) = - 7$ . Since $f ( c ) < f ( d )$ , our new range is $a = 0 , b = . 6 1 8$ . Recalculating from the new range gives $d = . 2 3 6 ,$ $c = . 3 8 2$ (note that our current c was our previous d: it is this reuse of calculated values that gives golden section search its speed). We repeat this process to get the following table: 


Table 5.2: Golden section search in Example 5.2.


<table><tr><td>Iter.</td><td>a</td><td>d</td><td>c</td><td>b</td><td>f(a)</td><td>f(d)</td><td>f(c)</td><td>f(b)</td></tr><tr><td>1</td><td>0</td><td>0.382</td><td>0.618</td><td>1</td><td>0</td><td>-0.6869</td><td>-2.4934</td><td>-7</td></tr><tr><td>2</td><td>0</td><td>0.2361</td><td>0.382</td><td>0.618</td><td>0</td><td>-0.0844</td><td>-0.6869</td><td>-2.4934</td></tr><tr><td>3</td><td>0</td><td>0.1459</td><td>0.2361</td><td>0.382</td><td>0</td><td>0.079</td><td>-0.0844</td><td>-0.6869</td></tr><tr><td>4</td><td>0</td><td>0.0902</td><td>0.1459</td><td>0.2361</td><td>0</td><td>0.099</td><td>0.079</td><td>-0.0844</td></tr><tr><td>5</td><td>0</td><td>0.0557</td><td>0.0902</td><td>0.1459</td><td>0</td><td>0.0804</td><td>0.099</td><td>0.079</td></tr><tr><td>6</td><td>0.0557</td><td>0.0902</td><td>0.1115</td><td>0.1459</td><td>0.0804</td><td>0.099</td><td>0.0987</td><td>0.079</td></tr><tr><td>7</td><td>0.0557</td><td>0.077</td><td>0.0902</td><td>0.1115</td><td>0.0804</td><td>0.0947</td><td>0.099</td><td>0.0987</td></tr><tr><td>8</td><td>0.077</td><td>0.0902</td><td>0.0983</td><td>0.1115</td><td>0.0947</td><td>0.099</td><td>0.1</td><td>0.0987</td></tr><tr><td>9</td><td>0.0902</td><td>0.0983</td><td>0.1033</td><td>0.1115</td><td>0.099</td><td>0.1</td><td>0.0999</td><td>0.0987</td></tr><tr><td>10</td><td>0.0902</td><td>0.0952</td><td>0.0983</td><td>0.1033</td><td>0.099</td><td>0.0998</td><td>0.1</td><td>0.0999</td></tr><tr><td>11</td><td>0.0952</td><td>0.0983</td><td>0.1002</td><td>0.1033</td><td>0.0998</td><td>0.1</td><td>0.1</td><td>0.0999</td></tr><tr><td>12</td><td>0.0983</td><td>0.1002</td><td>0.1014</td><td>0.1033</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.0999</td></tr><tr><td>13</td><td>0.0983</td><td>0.0995</td><td>0.1002</td><td>0.1014</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>14</td><td>0.0995</td><td>0.1002</td><td>0.1007</td><td>0.1014</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>15</td><td>0.0995</td><td>0.0999</td><td>0.1002</td><td>0.1007</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>16</td><td>0.0995</td><td>0.0998</td><td>0.0999</td><td>0.1002</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>17</td><td>0.0998</td><td>0.0999</td><td>0.1</td><td>0.1002</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>18</td><td>0.0999</td><td>0.1</td><td>0.1001</td><td>0.1002</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>19</td><td>0.0999</td><td>0.1</td><td>0.1</td><td>0.1001</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>20</td><td>0.0999</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr><tr><td>21</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td><td>0.1</td></tr></table>

Exercise 5.4 One of the most fundamental techniques of statistical analysis is the method of maximum likelihood estimation. Given a sample set of independently drawn observations from a parametric distribution, the estimation problem is to determine the values of the distribution parameters that maximize probability that the observed sample set comes from this distribution. 

Consider, for example, the observations $x _ { 1 } = - 0 . 2 4 , x _ { 2 } = 0 . 3 1 , x _ { 3 } = 2 . 3$ 2 and $x _ { 4 } ~ = ~ - 1 . 1$ sampled from a normal distribution. If the mean of the distribution is known to be $0 ,$ what is the maximum likelihood estimate of the standard deviation, $\sigma ?$ Construct the log-likelihood function and maximize it using golden section search. 

## 5.3.2 Newton’s Method

The main workhorse of many optimization algorithms is a centuries old technique for the solution of nonlinear equations developed by Sir Isaac Newton. We will discuss the multivariate version of Newton’s method later. We focus on the univariate case first. For a given nonlinear function $f$ we want to find an x such that 

$$
f (x) = 0.
$$

Assume that $f$ is continuously diferentiable and that we currently have an estimate $x ^ { k }$ of the solution (we will use superscripts for iteration indices in the following discussion). The first order (i.e., linear) Taylor series approximation to the function $f$ around $x ^ { k }$ can be written as follows: 

$$
f (x ^ {k} + \delta) \approx \hat {f} (\delta) := f (x ^ {k}) + \delta f ^ {\prime} (x ^ {k}).
$$

This is equivalent to saying that we can approximate the function $f$ by the line ${ \hat { f } } ( \delta )$ that is tangent to it at $x ^ { k }$ . If the first order approximation ${ \hat { f } } ( \delta )$ were perfectly good, and if $f ^ { \prime } ( x ^ { k } ) \neq 0$ , the value of δ that satisfies 

$$
\hat {f} (\delta) = f (x ^ {k}) + \delta f ^ {\prime} (x ^ {k}) = 0
$$

would give us the update on the current iterate $x ^ { k }$ necessary to get to the solution. This value of δ is computed easily: 

$$
\delta = - \frac {f (x ^ {k})}{f ^ {\prime} (x ^ {k})}.
$$

The expression above is called the Newton update and Newton’s method determines its next estimate of the solution as 

$$
x ^ {k + 1} = x ^ {k} + \delta = x ^ {k} - \frac {f (x ^ {k})}{f ^ {\prime} (x ^ {k})}.
$$

Since ${ \hat { f } } ( \delta )$ is only an approximation to $f ( x ^ { k } + \delta )$ , we do not have a guarantee that $f ( x ^ { k + 1 } )$ is zero, or even small. However, as we discuss below, when $x ^ { k }$ is close enough to a solution of the equation $f ( x ) = 0 , x ^ { k + 1 }$ is even closer. We can then repeat this procedure until we find an $x ^ { k }$ such that $f ( x ^ { k } ) = 0 ,$ 2 or in most cases, until $f ( x ^ { k } )$ becomes reasonably small, say, less than some pre-specified $\varepsilon > 0$ 

There is an intuitive geometric explanation of the procedure we just described: We first find the line that is tangent to the function at the current iterate, then we calculate the point where this line intersects the x-axis, and we set the next iterate to this value and repeat the process. See Figure 5.1 for an illustration. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/522d69436ce86e6fdfaf5f8296528f81f830ce1252ae6a9e2101a3a0725762c2.jpg)



Figure 5.1: First step of Newton’s method in Example 5.3


Example 5.3 Let us recall Example 5.1 where we computed the IRR of an investment. Here we solve the problem using Newton’s method. Recall that the yield r must satisfy the equation 

$$
f (r) = \frac {1 0 0}{1 + r} + \frac {1 0 0}{(1 + r) ^ {2}} + \frac {1 0 0}{(1 + r) ^ {3}} + \frac {1 1 0 0}{(1 + r) ^ {4}} - 9 0 0 = 0.
$$

The derivative of $f ( r )$ is easily computed: 

$$
f ^ {\prime} (r) = - \frac {1 0 0}{(1 + r) ^ {2}} - \frac {2 0 0}{(1 + r) ^ {3}} - \frac {3 0 0}{(1 + r) ^ {4}} - \frac {4 4 0 0}{(1 + r) ^ {5}}.
$$

We need to start Newton’s method with an initial guess, let us choose $x ^ { 0 } = 0$ . Then 

$$
\begin{array}{r c l} x ^ {1} & = & x ^ {0} - \frac {f (0)}{f ^ {\prime} (0)} \\ & = & 0 - \frac {5 0 0}{- 5 0 0 0} = 0. 1 \end{array}
$$

We mentioned above that the next iterate of Newton’s method is found by calculating the point where the line tangent to $f$ at the current iterate intersects the axis. This observation is illustrated in Figure 5.1. 

Since $f ( x ^ { 1 } ) = f ( 0 . 1 ) = 1 0 0$ is far from zero we continue by substituting $x ^ { 1 }$ into the Newton update formula to obtain $x ^ { 2 } = 0$ .131547080371 and so on. The complete iteration sequence is given in Table 5.3. 

A few comments on the speed and reliability of Newton’s method are in order. Under favorable conditions, Newton’s method converges very fast to a solution of a nonlinear equation. Indeed, if $x ^ { k }$ is suficiently close to a solution $x ^ { * }$ and if $f ^ { \prime } ( x ^ { * } ) \neq 0$ , then the following relation holds: 


Table 5.3: Newton’s method for Example 5.3


<table><tr><td>k</td><td><eq>x^{k}</eq></td><td><eq>f(x^{k})</eq></td></tr><tr><td>0</td><td>0.000000000000</td><td>500.000000000000</td></tr><tr><td>1</td><td>0.100000000000</td><td>100.000000000000</td></tr><tr><td>2</td><td>0.131547080371</td><td>6.464948211497</td></tr><tr><td>3</td><td>0.133880156946</td><td>0.031529863053</td></tr><tr><td>4</td><td>0.133891647326</td><td>0.000000758643</td></tr><tr><td>5</td><td>0.133891647602</td><td>0.000000000000</td></tr></table>

$$
x ^ {k + 1} - x ^ {*} \approx C (x ^ {k} - x ^ {*}) ^ {2} \text {with} C = \frac {f ^ {\prime \prime} (x ^ {*})}{2 f ^ {\prime} (x ^ {*})}\tag{5.2}
$$

(5.2) indicates that, the error in our approximation $( x ^ { k } - x ^ { * } )$ is approximately squared in each iteration. This behavior is called the quadratic convergence of Newton’s method. Note that the number of correct digits is doubled in each iteration of the example above and the method required much fewer iterations than the simple bisection approach. 

However, when the ‘favorable conditions’ we mentioned above are not satisfied, Newton’s method may fail to converge to a solution. For example, consider $f ( x ) = x ^ { 3 } - 2 x + 2$ . Starting at 0, one would obtain iterates cycling between 1 and 0. Starting at a point close to 1 or 0, one similarly gets iterates alternating in close neighborhoods of 1 and 0, without ever reaching the root around -1.76. Therefore, it often has to be modified before being applied to general problems. Common modifications of Newton’s method include the line-search and trust-region approaches. We briefly discuss line search approaches in Section 5.3.3. More information on these methods can be found in standard numerical optimization texts such as [55]. 

Next, we derive a variant of Newton’s method that can be applied to univariate optimization problems. If the function to be minimized/maximized has a unique minimizer/maximizer and is twice diferentiable, we can do the following. Diferentiability and the uniqueness of the optimizer indicate that $x ^ { * }$ maximizes (or minimizes) $g ( x )$ if and only if $g ^ { \prime } ( x ^ { * } ) = 0$ . Defining $f ( x ) = g ^ { \prime } ( x )$ and applying Newton’s method to this function we obtain iterates of the following form: 

$$
x ^ {k + 1} = x ^ {k} - \frac {f (x ^ {k})}{f ^ {\prime} (x ^ {k})} = x ^ {k} - \frac {g ^ {\prime} (x ^ {k})}{g ^ {\prime \prime} (x ^ {k})}.
$$

Example 5.4 Let us apply the optimization version of Newton’s method to Example 5.2. Recalling that $f ( x ) = x ^ { 5 } - 1 0 x ^ { 2 } + 2 x ,$ we have $f ^ { \prime } ( x ) =$ $5 x ^ { 4 } - 2 0 x + 2$ and $f ^ { \prime \prime } ( x ) = 2 0 ( x ^ { 3 } - 1 )$ ). Thus, the Newton update formula is given as 

$$
x ^ {k + 1} = x ^ {k} - \frac {5 (x ^ {k}) ^ {4} - 2 0 x ^ {k} + 2}{2 0 ((x ^ {k}) ^ {3} - 1)}.
$$


Table 5.4: Iterates of Newton’s method in Example 5.4


<table><tr><td>k</td><td><eq>x^{k}</eq></td><td><eq>f(x^{k})</eq></td><td><eq>f&#x27;(x^{k})</eq></td></tr><tr><td>0</td><td>0.000000000000</td><td>0.000000000000</td><td>2.000000000000</td></tr><tr><td>1</td><td>0.100000000000</td><td>0.100010000000</td><td>0.000500000000</td></tr><tr><td>2</td><td>0.100025025025</td><td>0.100010006256</td><td>0.000000000188</td></tr><tr><td>3</td><td>0.100025025034</td><td>0.100010006256</td><td>0.000000000000</td></tr></table>

Starting from 0 and iterating we obtain the sequence given in Table $5 . 4 .$ 

Once again, observe that Newton’s method converged very rapidly to the solution and generated several more digits of accuracy than the golden section search. Note however that the method would have failed if we had chosen $x ^ { 0 } = 1$ as our starting point. 

Exercise 5.5 Repeat Exercises 5.2, 5.3, and 5.4 using Newton’s method. 

Exercise 5.6 We derived Newton’s method by approximating a given function f using the first two terms of its Taylor series at the current point $x _ { k }$ When we use Taylor series approximation to a function, there is no a priori reason that tells us to stop at two terms. We can consider, for example, using the first three terms of the Taylor series expansion of the function and get a quadratic approximation. Derive a variant of Newton’s method that uses this approximation to determine the roots of the function $f .$ Can you determine the rate of convergence for this new method, assuming that the method converges? 

## 5.3.3 Approximate Line Search

When we are optimizing a univariate function, sometimes it is not necessary to find the minimizer/maximizer of the function very accurately. This is especially true when the univariate optimization is only one of the steps in an iterative procedure for optimizing a more complicated function. This happens, for example, when the function under consideration corresponds to the values of a multivariate function along a fixed direction. In such cases, one is often satisfied with a new point that provides a suficient amount of improvement over the previous point. Typically, a point with suficient improvement can be determined much quicker than the exact minimizer of the function which results in a shorter computation time for the overall algorithm. 

The notion of “suficient improvement” must be formalized to ensure that such an approach will generate convergent iterates. Say we wish to minimize the nonlinear, diferentiable function $f ( x )$ and we have a current estimate $x ^ { k }$ of its minimizer. Assume that $f ^ { \prime } ( x ^ { k } ) < 0$ which indicates that the function will decrease by increasing $x ^ { k }$ . Recall the linear Taylor series approximation to the function: 

$$
f (x ^ {k} + \delta) \approx \hat {f} (\delta) := f (x ^ {k}) + \delta f ^ {\prime} (x ^ {k}).
$$

The derivative of the function $f ^ { \prime } ( x ^ { k } )$ gives a prediction of the decrease in the function value as we move forward from $x ^ { k }$ . If f has a minimizer, we can not expect that it will decrease forever as we increase $x ^ { k }$ like its linear approximation above. We can require, however, that we find a new point such that the improvement in the function value is at least a fraction of the improvement predicted by the linear approximation. Mathematically, we can require that 

$$
f (x ^ {k} + \delta) \leq f (x ^ {k}) + \mu \delta f ^ {\prime} (x ^ {k})\tag{5.3}
$$

where $\mu \in ( 0 , 1 )$ is the desired fraction. This suficient decrease requirement is often called the Armijo-Goldstein condition. See Figure 5.2 for an illustration. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/74f356cffba4ac4f352211cac863977cd08627c8b14e93f976e4ebbc48541f18.jpg)



Figure 5.2: Armijo-Goldstein suficient decrease condition


Among all step sizes satisfying the suficient decrease condition, one would typically prefer as large a step size as possible. However, trying to find the maximum such step size accurately will often be too time consuming and will beat the purpose of this approximation approach. A typical strategy used in line search is backtracking. We start with a reasonably large initial estimate. We check whether this step size satisfies condition (5.3). If it does, we accept this step size, modify our estimate and continue. If not, we backtrack by using a step size that is a fraction of the previous step size we tried. We continue to backtrack until we obtain a step size satisfying the suficient decrease condition. For example, if the initial step size is 5 and we use the fraction 0.8, first backtracking iteration will use a step size of 4, and then 3.2 and so on. 

Exercise 5.7 Consider the function $\begin{array} { r } { f ( x ) = \frac { 1 } { 4 } x ^ { 4 } - x ^ { 2 } + 2 x - 1 } \end{array}$ . We want to minimize this function using Newton’s method. Verify that starting at a point close to 0 or 1 and using Newton’s method, one would obtain iterates alternating between close neighborhoods of 0 and 1 and never converge. Apply Newton’s method to this problem with the Armijo-Goldstein condition and backtracking starting from the point 0. Use $\mu = . 5$ and a backtracking ratio of 0.9. Experiment with other values of $\mu \in ( 0 , 1 )$ and the backtracking ratio. 

Exercise 5.8 Re-solve Exercise 5.4 using the optimization version of Newton’s method with line search and backtracking. Use $\mu = . 1$ and a backtracking ratio of 0.8. 

Exercise 5.9 As Figure 5.2 illustrates the Armijo-Goldstein condition disallows step sizes that are too large and beyond which the predictive power of the gradient of the function is weak. Backtracking strategy balances this by trying to choose as large an acceptable value of the step size as possible, ensuring that the step size is not too small. Another condition, called the Wolfe condition, rules out step sizes that are too small by requiring that 

$$
\| f ^ {\prime} (x ^ {k} + \delta) \| \leq \eta \| f ^ {\prime} (x ^ {k}) \|
$$

for some $\eta ~ \in ~ [ 0 , 1 ]$ The motivation for this condition is the following: For a diferentiable function $f$ , minimizers (or maximizers) will occur at points where the derivative of the function is zero. The Wolfe condition seeks points whose derivatives are closer to zero than the current point. Interpret the Wolfe condition geometrically on $\mathrm { F i g u r e ~ 5 . 2 }$ . For function $f ( x ) = { \textstyle { \frac { 1 } { 4 } } } x ^ { 4 } - x ^ { 2 } + 2 x - 1$ with current iterate $x ^ { k } = 0 . 1$ determine the Newton update and calculate which values of the step size satisfy the Wolfe condition for $\begin{array} { r } { \eta = \frac { 1 } { 4 } } \end{array}$ and also for $\begin{array} { r } { \eta = \frac { 3 } { 4 } } \end{array}$ 

## 5.4 Unconstrained Optimization

We now move on to nonlinear optimization problems with multiple variables. First, we will focus on problems that have no constraints. Typical examples of unconstrained nonlinear optimization problems arise in model fitting and regression. The study of unconstrained problems is also important for constrained optimization as one often solves a sequence of unconstrained problems as subproblems in various algorithms for the solution of constrained problems. 

We use the following generic format for unconstrained nonlinear programs we consider in this section: 

$$
\min f (\mathbf {x}), \text {   where   } \mathbf {x} = (x _ {1}, \ldots , x _ {n}).
$$

For simplicity, we will restrict our discussion to minimization problems. These ideas can be trivially adapted for maximization problems. 

## 5.4.1 Steepest Descent

The simplest numerical method for finding a minimizing solution is based on the idea of going downhill on the graph of the function $f .$ . When the function $f$ is diferentiable, its gradient always points in the direction of fastest initial increase and the negative gradient is the direction of fastest decrease. This suggests that, if our current estimate of the minimizing point is $\mathbf { x } ^ { * }$ , moving in the direction of $- \nabla f ( \mathbf { x } ^ { * } )$ is desirable. Once we choose direction, deciding how far we should move along this direction is determined using line search. The line search problem is a univariate problem that can be solved, perhaps in an approximate fashion, using the methods of the previous section. This will provide a new estimate of the minimizing point and the procedure can be repeated. 

We illustrate this approach on the following example: 

$$
\min f (\mathbf {x}) = (x _ {1} - 2) ^ {4} + \exp (x _ {1} - 2) + (x _ {1} - 2 x _ {2}) ^ {2}.
$$

The first step is to compute the gradient of the function, namely the vector of the partial derivatives of the function with respect to each variable: 

$$
\nabla f (\mathbf {x}) = \left[ \begin{array}{c} 4 (x _ {1} - 2) ^ {3} + \exp (x _ {1} - 2) + 2 (x _ {1} - 2 x _ {2}) \\ - 4 (x _ {1} - 2 x _ {2}) \end{array} \right].\tag{5.4}
$$

Next, we need to choose a starting point. We arbitrarily select the point $\mathbf { x } ^ { 0 } = [ 0 , 3 ] ^ { \top }$ . Now we are ready to compute the steepest descent direction at point $\mathbf { x } ^ { 0 }$ . It is the direction opposite to the gradient vector computed at $\mathbf { x } ^ { 0 }$ , namely 

$$
\mathbf {d} ^ {\mathbf {0}} = - \nabla f (\mathbf {x} ^ {0}) = \left[ \begin{array}{c} 4 4 + e ^ {- 2} \\ - 2 4 \end{array} \right].
$$

If we move from $\mathbf { x } ^ { 0 }$ in the direction $\mathbf { d } ^ { 0 }$ , using a step size α we get a new point ${ \bf x } ^ { 0 } + \alpha { \bf d } ^ { 0 } { \bf \alpha } ( \alpha = 0$ corresponds to staying at $\mathbf { x } ^ { 0 } )$ . Since our goal is to minimize $f ,$ we will try to move to a point $\mathbf { x } ^ { 1 } = \mathbf { x } ^ { 0 } + \alpha \mathbf { d } ^ { 0 }$ where $\alpha$ is chosen to approximately minimize the function along this direction. For this purpose, we evaluate the value of the function $f$ along the steepest descent direction as a function of the step size α: 

$$
\begin{array}{r c l} \phi (\alpha) := f (\mathbf {x} ^ {0} + \alpha \mathbf {d} ^ {0}) & = & ([ 0 + (4 4 + e ^ {- 2}) \alpha ] - 2) ^ {4} + \exp ([ 0 + (4 4 + e ^ {- 2}) \alpha ] - 2) \\ & & + ([ 0 + (4 4 + e ^ {- 2}) \alpha ] - 2 [ 3 - 2 4 \alpha ]) ^ {2} \end{array}
$$

Now, the optimal value of α can be found by solving the one–dimensional minimization problem min $\phi ( \alpha )$ 

This minimization can be performed through one of the numerical line search procedures of the previous section. Here we use the approximate line search approach with suficient decrease condition we discussed in Section 5.3.3. We want to choose a step size alpha satisfying 

$$
\phi (\alpha) \leq \phi (0) + \mu \alpha \phi^ {\prime} (0)
$$

where $\mu \in ( 0 , 1 )$ is the desired fraction for the suficient decrease condition. We observe that the derivative of the function $\phi$ at 0 can be expressed as 

$$
\phi^ {\prime} (0) = \nabla f (\mathbf {x} ^ {0}) ^ {T} \mathbf {d} ^ {0}.
$$

## 5.4. UNCONSTRAINED OPTIMIZATION

This is the directional derivative of the function f at point $\mathbf { x } ^ { 0 }$ and direction $\mathbf { d } ^ { 0 }$ . Using this identity the suficient decrease condition on function $\phi$ can be written in terms of the original function f as follows: 

$$
f (\mathbf {x} ^ {0} + \alpha \mathbf {d} ^ {0}) \leq f (\mathbf {x} ^ {0}) + \mu \alpha \nabla f (\mathbf {x} ^ {0}) ^ {T} \mathbf {d} ^ {0}.\tag{5.5}
$$

The condition (5.5) is the multivariate version of the Armijo-Goldstein condition (5.3). 

As discussed in Section 5.3.3, the suficient decrease condition (5.5) can be combined with a backtracking strategy. For this example, we use $\mu = 0 . 3$ for the suficient decrease condition and apply backtracking with an initial trial step size of 1 and a backtracking factor of $\beta = 0 . 8$ . Namely, we try step sizes 1, 0.8, 0.64, 0.512 and so on, until we find a step size of the form $0 . 8 ^ { k }$ that satisfied the Armijo-Goldstein condition. The first five iterates of this approach as well as the 20th iterate are given in Table 5.5. For completeness, one also has to specify a termination criterion for the approach. Since the gradient of the function must be the zero vector at an unconstrained minimizer, most implementations will use a termination criterion of the form $\left\| \nabla f ( \mathbf { x } ) \right\| \leq \varepsilon$ where $\varepsilon > 0$ is an appropriately chosen tolerance parameter. Alternatively, one might stop when successive iterations are getting very close to each other, that is when $\| \mathbf { x } ^ { k + 1 } - \mathbf { x } ^ { k } \| \leq \varepsilon$ for some $\varepsilon > 0$ . This last condition indicates that progress has stalled. While this may be due to the fact that iterates approached the optimizer and can not progress any more, there are instances where the stalling is due to the high degree of nonlinearity in $f .$ 


Table 5.5: Steepest descent iterations


<table><tr><td>k</td><td><eq>(x_1^k, x_2^k)</eq></td><td><eq>(d_1^k, d_2^k)</eq></td><td><eq>\alpha^k</eq></td><td><eq>\| \nabla f(\mathbf{x}^{k+1}) \|</eq></td></tr><tr><td>0</td><td>(0.000, 3.000)</td><td>(43.864, -24.000)</td><td>0.055</td><td>3.800</td></tr><tr><td>1</td><td>(2.412, 1.681)</td><td>(0.112, -3.799)</td><td>0.168</td><td>2.891</td></tr><tr><td>2</td><td>(2.430, 1.043)</td><td>(-2.544, 1.375)</td><td>0.134</td><td>1.511</td></tr><tr><td>3</td><td>(2.089, 1.228)</td><td>(-0.362, -1.467)</td><td>0.210</td><td>1.523</td></tr><tr><td>4</td><td>(2.013, 0.920)</td><td>(-1.358, 0.690)</td><td>0.168</td><td>1.163</td></tr><tr><td>5</td><td>(1.785, 1.036)</td><td>(-0.193, -1.148)</td><td>0.210</td><td>1.188</td></tr><tr><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td></tr><tr><td>20</td><td>(1.472, 0.736)</td><td>(-0.001, 0.000)</td><td>0.134</td><td>0.001</td></tr></table>

A quick examination of Table 5.5 reveals that the signs of the second coordinate of the steepest descent directions change from one iteration to the next in most cases. What we are observing is the zigzagging phenomenon, a typical feature of steepest descent approaches that explain their slow convergence behavior for most problems. When we pursue the steepest descent algorithm for more iterations, the zigzagging phenomenon becomes even more pronounced and the method is slow to converge to the optimal solution $\mathbf { x } ^ { * } \approx ( 1 . 4 7 2 , 0 . 7 3 6 )$ . Figure 5.3 shows the steepest descent iterates for our example superimposed on the contour lines of the objective function. Steepest descent directions are perpendicular to the contour lines and zigzag between the two sides of the contour lines, especially when these lines create long and narrow corridors. It takes more than 30 steepest descent iterations in this small example to achieve $\| \nabla f ( x ) \| \leq 1 0 ^ { - 5 }$ . In summary, while the steepest descent approach is easy to implement and intuitive, and has relatively cheap iterations, it can also be quite slow to converge to solutions. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/aed3e53ca7f0797f8abc7b110ffd39b5112f8aa16a7cdde1c08479f451b292e2.jpg)



Figure 5.3: Zigzagging Behavior in the Steepest Descent Approach


Exercise 5.10 Consider a diferentiable multivariate function $f ( x )$ that we wish to minimize. Let $x _ { k }$ be a given estimate of the solution, and consider the first order Taylor series expansion of the function around $x _ { k } \mathrm { : }$ 

$$
\hat {f} (\delta) = f (x _ {k}) + \nabla f (x) ^ {\top} \delta .
$$

The quickest decrease in $\hat { f }$ starting from $x _ { k }$ is obtained in the direction that solves 

$$
\begin{array}{r c l} \min & \hat {f} (\delta) \\ & \| \delta \| & \leq 1 \end{array}
$$

Show that the solution $\delta ^ { * } = \alpha \nabla f ( x )$ with some $\alpha < 0 ,$ , i.e., the opposite direction to the gradient is the direction of steepest descent. 

Exercise 5.11 Recall the maximum likelihood estimation problem we considered in Exercise 5.4. While we maintain the assumption that the observed samples come from a normal distribution, we will no longer assume that we know the mean of the distribution to be zero. In this case, we have a two parameter (mean $\mu$ and standard deviation $\sigma )$ maximum likelihood estimation problem. Solve this problem using the steepest descent method. 

## 5.4.2 Newton’s Method

There are several numerical techniques for modifying the method of steepest descent that reduce the propensity of this approach to zigzag, and thereby speed up convergence. Steepest descent method uses the gradient of the objective function, only a first-order information on the function. Improvements can be expected by employing second-order information on the function, that is by considering its curvature. Methods using curvature information include Newton’s method that we have already discussed in the univariate setting. Here, we describe the generalization of this method to multivariate problems. 

Once again, we begin with the version of the method for solving equations: We will look at the case where there are several equations involving several variables: 

$$
\begin{array}{r c l} f _ {1} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) & = & 0 \\ f _ {2} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) & = & 0 \\ \vdots & & \vdots \\ f _ {n} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) & = & 0 \end{array}\tag{5.6}
$$

Let us represent this system as 

$$
F (\mathbf {x}) = 0,
$$

where $\mathbf { x }$ is a vector of n variables, and $F ( \mathbf { x } )$ is $\varPsi ^ { n }$ -valued function with components $f _ { 1 } ( \mathbf { x } ) , \ldots , f _ { n } ( \mathbf { x } )$ . We repeat the procedure in Section 5.3.2: First, we write the first order Taylor’s series approximation to the function $F$ around the current estimate $\mathbf { x } ^ { k }$ : 

$$
F (\mathbf {x} ^ {k} + \delta) \approx \hat {F} (\delta) := F (\mathbf {x} ^ {k}) + \nabla F (\mathbf {x} ^ {k}) \delta .\tag{5.7}
$$

Above, $\nabla F ( \mathbf { x } )$ denotes the Jacobian matrix of the function F, i.e., $\nabla F ( \mathbf { x } )$ has rows $( \nabla f _ { 1 } ( \mathbf { x } ) ) ^ { \top } , \ldots , ( \nabla f _ { n } ( \mathbf { x } ) ) ^ { \top }$ , the transposed gradients of the functions $f _ { 1 }$ through $f _ { n }$ . We denote the components of the n-dimensional vector x using subscripts, i.e. $\mathbf { x } = ( \mathbf { x } _ { 1 } , \ldots , \mathbf { x } _ { n } )$ . Let us make these statements more precise: 

$$
\begin{array}{r l r} \nabla F (\mathbf {x} _ {1}, \ldots , \mathbf {x} _ {n}) & = & \left[ \begin{array}{c c c} \frac {\partial f _ {1}}{\partial \mathbf {x} _ {1}} & \dots & \frac {\partial f _ {1}}{\partial \mathbf {x} _ {n}} \\ \vdots & \ddots & \vdots \\ \frac {\partial f _ {n}}{\partial \mathbf {x} _ {1}} & \dots & \frac {\partial f _ {n}}{\partial \mathbf {x} _ {n}} \end{array} \right]. \end{array}
$$

As before, $\hat { F } ( \delta )$ is the linear approximation to the function F by the hyperplane that is tangent to it at the current point $\mathbf { x } ^ { k }$ . The next step is to find the value of $\delta$ that would make the approximation equal to zero, i.e., the value that satisfies: 

$$
F (\mathbf {x} ^ {k}) + \nabla F (\mathbf {x} ^ {k}) \delta = \mathbf {0}.
$$

Notice that what we have on the right-hand-side is a vector of zeros and the equation above represents a system of linear equations. $\mathrm { I f } \ \nabla F ( \mathbf { x } ^ { k } )$ is nonsingular, the equality above has a unique solution given by 

$$
\delta = - \nabla F (\mathbf {x} ^ {k}) ^ {- 1} F (\mathbf {x} ^ {k}),
$$

and the formula for the Newton update in this case is: 

$$
\mathbf {x} ^ {k + 1} = \mathbf {x} ^ {k} + \delta = \mathbf {x} ^ {k} - \nabla F (\mathbf {x} ^ {k}) ^ {- 1} F (\mathbf {x} ^ {k}).
$$

Example 5.5 Consider the following problem: 

$$
F (\mathbf {x}) = F (\mathbf {x} _ {1}, \mathbf {x} _ {2}) = \binom{f _ {1} (\mathbf {x} _ {1}, \mathbf {x} _ {2})}{f _ {2} (\mathbf {x} _ {1}, \mathbf {x} _ {2})} = \binom{\mathbf {x} _ {1} \mathbf {x} _ {2} - 2 \mathbf {x} _ {1} + \mathbf {x} _ {2} - 2}{(\mathbf {x} _ {1}) ^ {2} + 2 \mathbf {x} _ {1} + (\mathbf {x} _ {2}) ^ {2} - 7 \mathbf {x} _ {2} + 7} = \mathbf {0}
$$

First we calculate the Jacobian: 

$$
\nabla F (\mathbf {x} _ {1}, \mathbf {x} _ {2}) = \left( \begin{array}{c c} \mathbf {x} _ {2} - 2 & \mathbf {x} _ {1} + 1 \\ 2 \mathbf {x} _ {1} + 2 & 2 \mathbf {x} _ {2} - 7 \end{array} \right).
$$

If our initial estimate of the solution is $\mathbf { x } _ { 0 } ~ = ~ ( 0 , 0 )$ , then the next point generated by Newton’s method will be: 

$$
\begin{array}{r c l} (\mathbf {x} _ {1} ^ {1}, \mathbf {x} _ {2} ^ {1}) & = & (\mathbf {x} _ {1} ^ {0}, \mathbf {x} _ {2} ^ {0}) - \left( \begin{array}{c c} \mathbf {x} _ {2} ^ {0} - 2 & \mathbf {x} _ {1} ^ {0} + 1 \\ 2 \mathbf {x} _ {1} ^ {0} + 2 & 2 \mathbf {x} _ {2} ^ {0} - 7 \end{array} \right) ^ {- 1} \binom{\mathbf {x} _ {1} ^ {0} \mathbf {x} _ {2} ^ {0} - 2 \mathbf {x} _ {1} ^ {0} + \mathbf {x} _ {2} ^ {0} - 2}{(\mathbf {x} _ {1} ^ {0}) ^ {2} + 2 \mathbf {x} _ {1} ^ {0} + (\mathbf {x} _ {2} ^ {0}) ^ {2} - 7 \mathbf {x} _ {2} ^ {0} + 7} \\ & = & (0, 0) - \left( \begin{array}{c c} - 2 & 1 \\ 2 & - 7 \end{array} \right) ^ {- 1} \binom{- 2}{7} \\ & = & (0, 0) - (\frac {7}{1 2}, - \frac {5}{6}) = (- \frac {7}{1 2}, \frac {5}{6}). \end{array}
$$

## Optimization Version

When we use Newton’s method for unconstrained optimization of a twice diferentiable function $f ( \mathbf { x } )$ , the nonlinear equality system that we want to solve is the first order necessary optimality condition $\nabla f ( \mathbf { x } ) = 0$ . In this case, the functions $f _ { i } ( \mathbf { x } )$ in (5.6) are the partial derivatives of the function $f .$ That is, 

$$
{f _ {i} (\mathbf {x})} = {\frac {\partial f}{\partial \mathbf {x} _ {i}} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}).}
$$

Writing 

$$
\begin{array}{r l r} {F (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n})} & = & {\left[ \begin{array}{c} f _ {1} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) \\ f _ {2} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) \\ \vdots \\ f _ {n} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) \end{array} \right] = \left[ \begin{array}{c} \frac {\partial f}{\partial \mathbf {x} _ {1}} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) \\ \frac {\partial f}{\partial \mathbf {x} _ {i}} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) \\ \vdots \\ \frac {\partial f}{\partial \mathbf {x} _ {n}} (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) \end{array} \right] = \nabla f (\mathbf {x}),} \end{array}
$$

we observe that the Jacobian matrix $\nabla F ( \mathbf { x } _ { 1 } , \mathbf { x } _ { 2 } , \ldots , \mathbf { x } _ { n } )$ is nothing but the Hessian matrix of function $f \colon$ 

$$
\begin{array}{r l r} \nabla F (\mathbf {x} _ {1}, \mathbf {x} _ {2}, \ldots , \mathbf {x} _ {n}) & = & \left[ \begin{array}{c c c} \frac {\partial^ {2} f}{\partial \mathbf {x} _ {1} \partial \mathbf {x} _ {1}} & \dots & \frac {\partial^ {2} f}{\partial \mathbf {x} _ {1} \partial \mathbf {x} _ {n}} \\ \vdots & \ddots & \vdots \\ \frac {\partial^ {2} f}{\partial \mathbf {x} _ {n} \partial \mathbf {x} _ {1}} & \ldots & \frac {\partial^ {2} f}{\partial \mathbf {x} _ {n} \partial \mathbf {x} _ {n}} \end{array} \right] = \nabla^ {2} f (\mathbf {x}). \end{array}
$$

## 5.4. UNCONSTRAINED OPTIMIZATION

Therefore, the Newton direction at iterate $\mathbf { x } ^ { k }$ is given by 

$$
\delta = - \nabla^ {2} f (\mathbf {x} ^ {k}) ^ {- 1} \nabla f (\mathbf {x} ^ {k})\tag{5.8}
$$

and the Newton update formula is 

$$
{\bf x} ^ {k + 1} = {\bf x} ^ {k} + \delta = {\bf x} ^ {k} - \nabla f ^ {2} ({\bf x} ^ {k}) ^ {- 1} \nabla f ({\bf x} ^ {k}).
$$

For illustration and comparison purposes, we apply this technique to the example problem of Section 5.4.1. Recall that the problem was to 

$$
\min f (\mathbf {x}) = (x _ {1} - 2) ^ {4} + \exp (x _ {1} - 2) + (x _ {1} - 2 x _ {2}) ^ {2}
$$

starting from $\mathbf { x } ^ { 0 } = ( 0 , 3 ) ^ { \top }$ 

The gradient of f was given in (5.4) and the Hessian matrix is given below: 

$$
\nabla^ {2} f (\mathbf {x}) = \left[ \begin{array}{c c} 1 2 (x _ {1} - 2) ^ {2} + \exp (x _ {1} - 2) + 2 & - 4 \\ - 4 & 8 \end{array} \right].\tag{5.9}
$$

Thus, we calculate the Newton direction at $\mathbf { x } ^ { 0 } = ( 0 , 3 ) ^ { \top }$ as follows: 

$$
\delta = - \nabla^ {2} f (\left[ \begin{array}{c} 0 \\ 3 \end{array} \right]) ^ {- 1} \nabla f (\left[ \begin{array}{c} 0 \\ 3 \end{array} \right]) = - \left[ \begin{array}{c c} 5 0 + e ^ {- 2} & - 4 \\ - 4 & 8 \end{array} \right] ^ {- 1} \left[ \begin{array}{c} - 4 4 + e ^ {- 2} \\ 2 4 \end{array} \right] = \left[ \begin{array}{c} 0. 6 6 2 \\ - 2. 6 6 9 \end{array} \right].
$$

We list the first five iterates in Table 5.6 and illustrate the rapid progress of the algorithm towards the optimal solution in Figure 5.4. Note that the ideal step size for Newton’s method is almost always one. In our example, this step size always satisfied the suficient decrease condition and was chosen in each iteration. Newton’s method identifies a point with $\| \nabla f ( x ) \| \leq 1 0 ^ { - 5 }$ after 7 iterations. 


Table 5.6: Newton iterations


<table><tr><td>k</td><td><eq>(x_1^k, x_2^k)</eq></td><td><eq>(d_1^k, d_2^k)</eq></td><td><eq>\alpha^k</eq></td><td><eq>\| \nabla f(\mathbf{x}^{k+1}) \|</eq></td></tr><tr><td>0</td><td>(0.000, 3.000)</td><td>(0.662, -2.669)</td><td>1.000</td><td>9.319</td></tr><tr><td>1</td><td>(0.662, 0.331)</td><td>(0.429, 0.214)</td><td>1.000</td><td>2.606</td></tr><tr><td>2</td><td>(1.091, 0.545)</td><td>(0.252, 0.126)</td><td>1.000</td><td>0.617</td></tr><tr><td>3</td><td>(1.343, 0.671)</td><td>(0.108, 0.054)</td><td>1.000</td><td>0.084</td></tr><tr><td>4</td><td>(1.451, 0.726)</td><td>(0.020, 0.010)</td><td>1.000</td><td>0.002</td></tr><tr><td>5</td><td>(1.471, 0.735)</td><td>(0.001, 0.000)</td><td>1.000</td><td>0.000</td></tr></table>

Despite its excellent convergence behavior close to a solution, Newton’s method is not always the best option, especially for large-scale optimization. Often the Hessian matrix is expensive to compute at each iteration. In such cases, it may be preferable to use an approximation of the Hessian matrix instead. These approximations are usually chosen in such a way that the solution of the linear system in (5.8) is much cheaper that what it would be with the exact Hessian. Such approaches are known as quasi-Newton methods. Most popular variants of quasi-Newton methods are BFGS and DFP methods. These acronyms represent the developers of these algorithms in the late 60s and early 70s. Detailed information on quasi-Newton approaches can be found in, for example, [55]. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/a818e4148cd0a57a2f20e8afab0a11ae9f32a12fa68e063c7de720dec7608ac4.jpg)



Figure 5.4: Rapid convergence of Newton’s method


Exercise 5.12 Repeat Exercise 5.11, this time using the optimization version of Newton’s method. Use line-search with $\begin{array} { r } { \mu = \frac { 1 } { 2 } } \end{array}$ in Armijo-Goldstein condition and a backtracking ratio of $\begin{array} { r } { \beta = \frac { 1 } { 2 } } \end{array}$ 

## 5.5 Constrained Optimization

We now move on to the more general case of nonlinear optimization problems with constraints. Specifically, we consider an optimization problem given by a nonlinear objective function and/or nonlinear constraints. We can represent such problems in the following generic form: 

$$
\begin{array}{r l r} \min _ {x} & f (x) \\ & g _ {i} (x) = 0, i \in \mathcal {E} \\ & g _ {i} (x) \geq 0, i \in \mathcal {I}. \end{array}\tag{5.10}
$$

In the remainder of this section we assume that $f$ and $g _ { i } , \ i \in \mathcal { E } \cup \mathcal { T }$ are all continuously diferentiable functions. 

An important tool in the study of constrained optimization problems is the Lagrangian function. To define this function, one associates a multiplier λ<sub>i</sub>–the so-called Lagrange multiplier–with each one of the constraints. For problem (5.10) the Lagrangian is defined as follows: 

$$
\mathcal {L} (x, \lambda) := f (x) - \sum_ {i \in \mathcal {E} \cup \mathcal {I}} \lambda_ {i} g _ {i} (x).\tag{5.11}
$$

Essentially, we are considering an objective function that is penalized for violations of the feasibility constraints. For properly chosen values of $\lambda _ { i } .$ minimizing the unconstrained function $\mathcal { L } ( x , \lambda )$ is equivalent to solving the constrained optimization problem (5.10). This equivalence is the primary reason for our interest in the Lagrangian function. 

One of the most important theoretical issues related to this problem is the identification of necessary and suficient conditions for optimality. Collectively, these conditions are called the optimality conditions and are the subject of this section. 

Before presenting the optimality conditions for (5.10) we first discuss a technical condition called regularity that is encountered in the theorems that follow: 

Definition 5.1 Let x be a vector satisfying $g _ { i } ( x ) = 0 , i \in \mathcal { E }$ and $g _ { i } ( x ) \geq$ $0 , i \in \mathcal { T }$ . Let $\mathcal { I } \subset \mathcal { I }$ be the set of indices for which $g _ { i } ( x ) \geq 0$ is satisfied with equality. Then, x is a regular point of the constraints $o f \ ( 5 . 1 0 )$ if the gradient vectors $\nabla g _ { i } ( x ) \ f o r \ i \in \mathcal { E } \cup \mathcal { T }$ are linearly independent. 

Constraints corresponding to the set $\mathcal { E } \cup \mathcal { I }$ in the definition above, namely, the constraints for which we have $g _ { i } ( x ) = 0$ , are called the active constraints at x. 

We discussed two notions of optimality in Chapter 1, local and global. Recall that a global optimal solution to (5.10) is a vector $x ^ { * }$ that is feasible and satisfies $f ( x ^ { * } ) \leq f ( x )$ for all feasible x. In contrast, a local optimal solution $x ^ { * }$ is feasible and satisfies $f ( x ^ { * } ) \leq f ( x )$ for all feasible x in the set $\{ x : \| x - x ^ { * } \| \leq \varepsilon \}$ for some $\varepsilon > 0$ . So, a local solution must be better than all the feasible points in a neighborhood of itself. The optimality conditions we consider below identify local solutions only, which may or may not be global solutions to the problem. Fortunately, there is an important class of problems where local and global solutions coincide, namely convex optimization problems. See Appendix A for a discussion on convexity and convex optimization problems. 

Theorem 5.1 (First Order Necessary Conditions) Let $x ^ { * }$ be a local minimizer of the problem $( 5 . 1 0 )$ and assume that $x ^ { * }$ is a regular point $f o r$ the constraints of this problem. Then, there exists $\lambda _ { i } , \ i \in \mathcal { E } \cup \mathcal { T }$ such that 

$$
\nabla f (x ^ {*}) - \sum_ {i \in \mathcal {E} \cup \mathcal {I}} \lambda_ {i} \nabla g _ {i} (x ^ {*}) = 0\tag{5.12}
$$

$$
\lambda_ {i} \geq 0, i \in \mathcal {I}\tag{5.13}
$$

$$
\lambda_ {i} g _ {i} (x ^ {*}) = 0, i \in \mathcal {I}.\tag{5.14}
$$

Note that the expression on the left hand side of (5.12) is the gradient of the Lagrangian function $\mathcal { L } ( x , \lambda )$ with respect to the variables x. First order conditions are satisfied at local minimizers as well as local maximizers and saddle points. When the objective and constraint functions are twice continuously diferentiable, one can eliminate maximizers and saddle points using curvature information on the functions. As in Theorem 5.1, we consider the Lagrangian function $\mathcal { L } ( x , \lambda )$ and use the Hessian of this function with respect to the x variables to determine the collective curvature in the objective function as well as the constraint functions at the current point. 

Theorem 5.2 (Second Order Necessary Conditions) Assume that f and $g _ { i } , i \in \mathcal { E } \cup \mathcal { T }$ are all twice continuously diferentiable functions. Let $x ^ { * }$ be a local minimizer of the problem $( 5 . 1 0 )$ and assume that $x ^ { * }$ is a regular point for the constraints of this problem. Then, there exists $\lambda _ { i } , \ i \in \mathcal { E } \cup \mathcal { T }$ satisfying (5.12)–(5.14) as well as the following condition: 

$$
\nabla^ {2} f (x ^ {*}) - \sum_ {i \in \mathcal {E} \cup \mathcal {I}} \lambda_ {i} \nabla^ {2} g _ {i} (x ^ {*})\tag{5.15}
$$

is positive semidefinite on the tangent subspace of active constraints at $x ^ { * }$ 

The last part of the theorem above can be restated in terms of the Jacobian of the active constraints. Let $A ( x ^ { * } )$ denote the Jacobian of the active constraints at $x ^ { * }$ and let $N ( x ^ { * } )$ be a null-space basis for $A ( x ^ { * } )$ . Then, the last condition of the theorem above is equivalent to the following condition: 

$$
N ^ {T} (x ^ {*}) \left(\nabla^ {2} f (x ^ {*}) - \sum_ {i \in \mathcal {E} \cup \mathcal {I}} \lambda_ {i} \nabla^ {2} g _ {i} (x ^ {*})\right) N (x ^ {*})\tag{5.16}
$$

is positive semidefinite. 

The satisfaction of the second order necessary conditions does not always guarantee the local optimality of a given solution vector. The conditions that are suficient for local optimality are slightly more stringent and a bit more complicated since they need to consider the possibility of degeneracy. 

Theorem 5.3 (Second Order Suficient Conditions) Assume that f and $g _ { i } , i \in \mathcal { E } \cup \mathcal { T }$ are all twice continuously diferentiable functions. Let $x ^ { * }$ be a feasible and regular point for the constraints of the problem $( 5 . 1 0 )$ . Let $A ( x ^ { * } )$ denote the Jacobian of the active constraints at $x ^ { * }$ and let $N ( x ^ { * } )$ be a nullspace basis for $A ( x ^ { * } )$ . If there exists $\lambda _ { i } , \ i \in \mathcal { E } \cup \mathcal { T }$ satisfying (5.12)–(5.14) as well as 

$$
g _ {i} (x ^ {*}) = 0, i \in \mathcal {I} \text {implies} \lambda_ {i} > 0,\tag{5.17}
$$

and 

$$
N ^ {T} (x ^ {*}) \left(\nabla^ {2} f (x ^ {*}) - \sum_ {i \in \mathcal {E} \cup \mathcal {I}} \lambda_ {i} \nabla^ {2} g _ {i} (x ^ {*})\right) N (x ^ {*}) i s p o s i t i v e d e f i n i t e\tag{5.18}
$$

then $x ^ { * }$ is a local minimizer of the problem $( 5 . 1 0 )$ 

The conditions listed in Theorems 5.1, 5.2, and 5.3 are often called Karush-Kuhn-Tucker (KKT) conditions, after their inventors. 

Some methods for solving constrained optimization problems formulate a sequence of simpler optimization problems whose solutions are used to generate iterates progressing towards the solution of the original problem. These “simpler” problems can be unconstrained, in which case they can be solved using the techniques we saw in the previous section. We discuss such 

## 5.5. CONSTRAINED OPTIMIZATION

a strategy in Section 5.5.1. In other cases, the simpler problem solved is a quadratic programming problem and can be solved using the techniques of Chapter 7. The prominent example of this strategy is the sequential quadratic programming method that we discuss in Section 5.5.2. 

Exercise 5.13 Recall the definition of the quadratic programming problem given in Chapter 1: 

$$
\begin{array}{r l r} (\mathcal {Q P}) & \qquad \min _ {x} & \frac {1}{2} x ^ {T} Q x + c ^ {T} x \\ & & A x = b \\ & & x \geq 0, \end{array}\tag{5.19}
$$

where $A \ \in \ R ^ { m \times n } , \ b \ \in \ R ^ { m } , \ c \ \in \ R ^ { n } , \ Q \ \in \ R ^ { n \times n }$ are given, and $x \in$ $\varPsi ^ { n }$ . Assume that $Q$ is symmetric and positive definite. Derive the KKT conditions for this problem. Show that the second order necessary conditions are also suficient given our assumptions. 

Exercise 5.14 Consider the following optimization problem: 

$$
\begin{array}{l l l l} \min & f (x _ {1}, x _ {2}) = - x _ {1} - x _ {2} - x _ {1} x _ {2} + \frac {1}{2} x _ {1} ^ {2} + x _ {2} ^ {2} \\ \text {s.t.} & x _ {1} + x _ {2} ^ {2} & \leq & 3, \\ \text {and} & (x _ {1}, x _ {2}) & \geq & 0. \end{array}
$$

List the Karush-Kuhn-Tucker optimality conditions for this problem. Verify that $x ^ { * } = ( 2 , 1 )$ is a local optimal solution to this problem by finding Lagrange multipliers $\lambda _ { i }$ satisfying the KKT conditions in combination with $x ^ { * }$ . Is $x ^ { * } = ( 2 , 1 )$ a global optimal solution? 

## 5.5.1 The generalized reduced gradient method

In this section, we introduce an approach for solving constrained nonlinear programs. It builds on the method of steepest descent method we discussed in the context of unconstrained optimization. The idea is to reduce the number of variables using the constraints and then to solve this reduced and unconstrained problem using the steepest descent method. 

## Linear Equality Constraints

First we consider an example where the constraints are linear equations. 

$$
\begin{array}{r c l r c l r c l r c l} \min & f (\mathbf {x}) & = & x _ {1} ^ {2} & + & x _ {2} & + & x _ {3} ^ {2} & + & x _ {4} \\ & g _ {1} (\mathbf {x}) & = & x _ {1} & + & x _ {2} & + & 4 x _ {3} & + & 4 x _ {4} & - & 4 & = & 0 \\ & g _ {2} (\mathbf {x}) & = & - x _ {1} & + & x _ {2} & + & 2 x _ {3} & - & 2 x _ {4} & + & 2 & = & 0. \end{array}
$$

It is easy to solve the constraint equations for two of the variables in terms of the others. Solving for $x _ { 2 }$ and $x _ { 3 }$ in terms of $x _ { 1 }$ and $x _ { 4 }$ gives 

$$
x _ {2} = 3 x _ {1} + 8 x _ {4} - 8 \mathrm{and} x _ {3} = - x _ {1} - 3 x _ {4} + 3.
$$

Substituting these expressions into the objective function yields the following reduced problem: 

$$
\min f (x _ {1}, x _ {4}) = x _ {1} ^ {2} + (3 x _ {1} + 8 x _ {4} - 8) + (- x _ {1} - 3 x _ {4} + 3) ^ {2} + x _ {4}.
$$

This problem is unconstrained and therefore it can be solved by the method of steepest descent, see Section 5.4.1. 

## Nonlinear Equality Constraints

Now consider the possibility of approximating a problem where the constraints are nonlinear equations by a problem with linear equations, which can then be solved like the preceding example. To see how this works, consider the following example, which is similar to the preceding one but has constraints that are nonlinear. 

## Example 5.6

$$
\begin{array}{r c l r c l r c l r c l} \min & f (\mathbf {x}) & = & x _ {1} ^ {2} & + & x _ {2} & + & x _ {3} ^ {2} & + & x _ {4} \\ & g _ {1} (\mathbf {x}) & = & x _ {1} ^ {2} & + & x _ {2} & + & 4 x _ {3} & + & 4 x _ {4} & - & 4 & = & 0 \\ & g _ {2} (\mathbf {x}) & = & - x _ {1} & + & x _ {2} & + & 2 x _ {3} & - & 2 x _ {4} ^ {2} & + & 2 & = & 0. \end{array}
$$

We use the Taylor series approximation to the constraint functions at the current point x¯: 

$$
g (\mathbf {x}) \approx g (\bar {\mathbf {x}}) + \nabla g (\bar {\mathbf {x}}) (\mathbf {x} - \bar {\mathbf {x}}) ^ {T}.
$$

This gives 

$$
\begin{array}{r l} {g _ {1} (\mathbf {x})} & {\approx (\bar {x} _ {1} ^ {2} + \bar {x} _ {2} + 4 \bar {x} _ {3} + 4 \bar {x} _ {4} - 4) + (2 \bar {x} _ {1}, 1, 4, 4) \left( \begin{array}{l} x _ {1} - \bar {x} _ {1} \\ x _ {2} - \bar {x} _ {2} \\ x _ {3} - \bar {x} _ {3} \\ x _ {4} - \bar {x} _ {4} \end{array} \right)} \\ & {\approx 2 \bar {x} _ {1} x _ {1} + x _ {2} + 4 x _ {3} + 4 x _ {4} - (\bar {x} _ {1} ^ {2} + 4) = 0} \end{array}
$$

and 

$$
{g _ {2} (\mathbf {x})} {\approx - x _ {1} + x _ {2} + 2 x _ {3} - 4 \bar {x} _ {4} x _ {4} + (\bar {x} _ {4} ^ {2} + 2) = 0.}
$$

The idea of the generalized reduced gradient algorithm (GRG) is to solve a sequence of subproblems, each of which uses a linear approximation of the constraints. In each iteration of the algorithm, the constraint linearization is recalculated at the point found from the previous iteration. Typically, even though the constraints are only approximated, the subproblems yield points that are progressively closer to the optimal point. A property of the linearization is that, at the optimal point, the linearized problem has the same solution as the original problem. 

The first step in applying GRG is to pick a starting point. Suppose that we start with $\mathbf { x } ^ { 0 } = ( 0 , - 8 , 3 , 0 )$ , which happens to satisfy the original constraints. It is possible to start from an infeasible point as we discuss later on. Using the approximation formulas derived earlier, we form our first approximation problem as follows. 

$$
\begin{array}{r c l r c l} \min & f (\mathbf {x}) & = & x _ {1} ^ {2} + x _ {2} + x _ {3} ^ {2} + x _ {4} \\ & g _ {1} (\mathbf {x}) & = & x _ {2} + 4 x _ {3} + 4 x _ {4} - 4 & = 0 \\ & g _ {2} (\mathbf {x}) & = & - x _ {1} + x _ {2} + 2 x _ {3} + 2 & = 0. \end{array}
$$

Now we solve the equality constraints of the approximate problem to express two of the variables in terms of the others. Arbitrarily selecting x<sub>2</sub> and $x _ { 3 }$ , we get 

$$
x _ {2} = 2 x _ {1} + 4 x _ {4} - 8 \text {and} x _ {3} = - \frac {1}{2} x _ {1} - 2 x _ {4} + 3.
$$

Substituting these expressions in the objective function yields the reduced problem 

$$
f (x _ {1}, x _ {4}) = x _ {1} ^ {2} + (2 x _ {1} + 4 x _ {2} - 8) + (- \frac {1}{2} x _ {1} - 2 x _ {4} + 3) ^ {2} + x _ {4}.
$$

Solving this unconstrained minimization problem yields $x _ { 1 } = - 0 . 3 7 5 .$ $x _ { 4 } = 0 . 9 6 8 7 5$ . Substituting in the equations for $x _ { 2 }$ and $x _ { 3 }$ gives $x _ { 2 } = - 4 . 8 7 5$ and $x _ { 3 } = 1 . 2 5$ . Thus the first iteration of GRG has produced the new point $\mathbf { x } ^ { 1 } = ( - 0 . 3 7 5 , - 4 . 8 7 5 , 1 . 2 5 , 0 . 9 6 8 7 5 )$ 

To continue the solution process, we would re-linearize the constraint functions at the new point, use the resulting system of linear equations to express two of the variables in terms of the others, substitute into the objective to get the new reduced problem, solve the reduced problem for $\mathbf { x } ^ { 2 } .$ and so forth. Using the stopping criterion $\| \mathbf { x } ^ { k + 1 } - \mathbf { x } ^ { k } \| < T$ where $T = 0 . 0 0 2 5$ , we get the results summarized in Table 5.7. 

<table><tr><td>k</td><td><eq>(x_1^k, x_2^k, x_3^k, x_4^k)</eq></td><td><eq>f(\mathbf{x}^k)</eq></td><td><eq>||\mathbf{x}^{k+1} - \mathbf{x}^k||</eq></td></tr><tr><td>0</td><td>(0.000, -8.000, 3.000, 0.000)</td><td>1.000</td><td>3.729</td></tr><tr><td>1</td><td>(-0.375, -4.875, 1.250, 0.969)</td><td>-2.203</td><td>0.572</td></tr><tr><td>2</td><td>(-0.423, -5.134, 1.619, 0.620)</td><td>-1.714</td><td>0.353</td></tr><tr><td>3</td><td>(-0.458, -4.792, 1.537, 0.609)</td><td>-1.610</td><td>0.022</td></tr><tr><td>4</td><td>(-0.478, -4.802, 1.534, 0.610)</td><td>-1.611</td><td>0.015</td></tr><tr><td>5</td><td>(-0.488, -4.813, 1.534, 0.610)</td><td>-1.612</td><td>0.008</td></tr><tr><td>6</td><td>(-0.494, -4.818, 1.534, 0.610)</td><td>-1.612</td><td>0.004</td></tr><tr><td>7</td><td>(-0.497, -4.821, 1.534, 0.610)</td><td>-1.612</td><td>0.002</td></tr><tr><td>8</td><td>(-0.498, -4.823, 1.534, 0.610)</td><td>-1.612</td><td></td></tr></table>


Table 5.7: Summarized results


This is to be compared with the optimum solution which is 

$$
x ^ {*} = (- 0. 5 0 0, - 4. 8 2 5, 1. 5 3 4, 0. 6 1 0)
$$

and has an objective value of -1.612. Note that, in Table 5.7, the values of the function $f ( x ^ { k } )$ are sometimes smaller than the minimum value for $k = 1$ 2 and 2. How is this possible? The reason is that the points $x ^ { k }$ computed by GRG are usually not feasible to the constraints. They are only feasible to a linear approximation of these constraints. 

Now we discuss the method used by GRG for starting at an infeasible solution: a phase 1 problem is solved to construct a feasible one. The objective function for the phase 1 problem is the sum of the absolute values of the violated constraints. The constraints for the phase 1 problem are the non-violated ones. Suppose we had started at the point $\mathbf { x } ^ { 0 } = \left( 1 , 1 , 0 , 1 \right)$ in our example. This point violates the first constraint but satisfies the second, so the phase 1 problem would be 

$$
\begin{array}{r l} \min & | x _ {1} ^ {2} + x _ {2} + 4 x _ {3} + 4 x _ {4} - 4 | \\ & - x _ {1} + x _ {2} + 2 x _ {3} - 2 x _ {4} ^ {2} + 2 = 0. \end{array}
$$

Once a feasible solution has been found by solving the phase 1 problem, the method illustrated above is used to find an optimal solution. 

## Linear Inequality Constraints

Finally, we discuss how GRG solves problems having inequality constraints as well as equalities. At each iteration, only the tight inequality constraints enter into the system of linear equations used for eliminating variables (these inequality constraints are said to be active). The process is complicated by the fact that active inequality constraints at the current point may need to be released in order to move to a better solution. We illustrate the ideas on the following example. 

$$
\begin{array}{r c l c l} \min & f (x _ {1}, x _ {2}) = & (x _ {1} - \frac {1}{2}) ^ {2} + & (x _ {2} - \frac {5}{2}) ^ {2} \\ & & x _ {1} - & x _ {2} \geq 0 \\ & & x _ {1} & \geq 0 \\ & & & x _ {2} \geq 0 \\ & & & x _ {2} \leq 2. \end{array}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/0c8f5e0b21486b8aa74a471074975510437628a5e502f74e436f0c1c8d1099eb.jpg)



Figure 5.5: Progress of the Generalized Reduced Gradient Algorithm


The feasible set of this problem is shown in Figure 5.5. The arrow in the figure indicate the feasible hyperplanes dictated by each constraint. Suppose that we start from $\mathbf { x } ^ { 0 } = ( 1 , 0 )$ . This point satisfies all the constraints. As can be seen from Figure 5.5, $x _ { 1 } - x _ { 2 } \geq 0 , x _ { 1 } \geq 0$ and $x _ { 2 } \le 2$ are inactive, whereas the constraint $x _ { 2 } \geq 0$ is active. We have to decide whether x<sub>2</sub> should stay at its lower bound or be allowed to leave its bound. 

$$
\nabla f (\mathbf {x} ^ {0}) = (2 x _ {1} ^ {0} - 1, 2 x _ {2} ^ {0} - 5) = (1, - 5).
$$

This indicates that we will get the largest decrease in f if we move in the direction $\mathbf { d } ^ { 0 } = - \nabla f ( \mathbf { x } ^ { 0 } ) = ( - 1 , 5 )$ , i.e. if we decrease $x _ { 1 }$ and increase $x _ { 2 }$ . Since this direction is towards the interior of the feasible region, we decide to release $x _ { 2 }$ from its bound. The new point will be $\mathbf { x } ^ { 1 } = \mathbf { x } ^ { 0 } + \alpha ^ { 0 } \mathbf { d } ^ { 0 }$ , for some $\alpha ^ { 0 } > 0$ . The constraints of the problem induce an upper bound on $\alpha ^ { 0 }$ , namely $\alpha ^ { 0 } \leq 0 . 8 3 3 3$ . Now we perform a line search to determine the best value of $\alpha ^ { 0 }$ in this range. It turns out to be $\alpha ^ { 0 } = 0 . 8 3 3 3$ , so $\mathbf { x } ^ { 1 } = ( 0 . 8 3 3 3 , 0 . 8 3 3 3 )$ ; see Figure 5.5. 

Now, we repeat the process: the constraint $x _ { 1 } - x _ { 2 } \geq 0$ has become active whereas the others are inactive. Since the active constraint is not a simple upper or lower bound constraint, we introduce a surplus variable, say $x _ { 3 }$ , and solve for one of the variables in terms of the others. Substituting $x _ { 1 } = x _ { 2 } + x _ { 3 }$ , we obtain the reduced optimization problem 

$$
\begin{array}{r l r} \min & f (x _ {2}, x _ {3}) = & (x _ {2} + x _ {3} - \frac {1}{2}) ^ {2} + (x _ {2} - \frac {5}{2}) ^ {2} \\ & & 0 \leq x _ {2} \leq 2 \\ & & x _ {3} \geq 0. \end{array}
$$

The reduced gradient is 

$$
\begin{array}{r l} \nabla f (x _ {2}, x _ {3}) & = (2 x _ {2} + 2 x _ {3} - 1 + 2 x _ {2} - 5, 2 x _ {2} + 2 x _ {3} - 1) \\ & = (- 2. 6 6 7, 0. 6 6 7) \text {   at   point   } (x _ {2}, x _ {3}) ^ {1} = (0. 8 3 3 3, 0). \end{array}
$$

Therefore, the largest decrease in f occurs in the direction $( 2 . 6 6 7 , - 0 . 6 6 7 )$ that is when we increase $x _ { 2 }$ and decrease $x _ { 3 }$ . But $x _ { 3 }$ is already at its lower bound, so we cannot decrease it. Consequently, we keep $x _ { 3 }$ at its bound, i.e. we move in the direction $\mathbf { d } ^ { 1 } = ( 2 . 6 6 7 , 0 )$ to a new point $( x _ { 2 } , x _ { 3 } ) ^ { 2 } =$ $( x _ { 2 } , x _ { 3 } ) ^ { 1 } + \alpha ^ { 1 } \mathbf { d } ^ { 1 }$ . A line search in this direction yields $\alpha ^ { 1 } ~ = ~ 0 . 2 5$ and $( x _ { 2 } , x _ { 3 } ) ^ { 2 } = ( 1 . 5 , 0 )$ . The same constraints are still active so we may stay in the space of variables $x _ { 2 }$ and $x _ { 3 }$ . Since 

$$
\nabla f (x _ {2}, x _ {3}) = (0, 2) \text {   at   point   } (x _ {2}, x _ {3}) ^ {2} = (1. 5, 0)
$$

is perpendicular to the boundary line at the current solution $\mathbf { x } ^ { 2 }$ and points towards the exterior of the feasible region, no further decrease in $f$ is possible. We have found the optimal solution. In the space of original variables, this optimal solution is $x _ { 1 } = 1 . 5$ and $x _ { 2 } = 1 . 5$ 

This is how some of the most widely distributed nonlinear programming solvers, such as Excel’s SOLVER, GINO, CONOPT, GRG2 and several others, solves nonlinear programs, with just a few additional details such as the Newton-Raphson direction for line search. Compared with linear programs, the problems that can be solved within a reasonable amount of computational time are typically smaller and the solutions produced may not be very accurate. Furthermore, the potential non-convexity in the feasible set or in the objective function may generate local optimal solutions which are far from a global solution. Therefore, the interpretation of the output of a nonlinear program requires more care. 

Exercise 5.15 Consider the following optimization problem: 

$$
\begin{array}{l l l l} \min & f (x _ {1}, x _ {2}) = - x _ {1} - x _ {2} - x _ {1} x _ {2} + \frac {1}{2} x _ {1} ^ {2} + x _ {2} ^ {2} \\ \text {s.t.} & x _ {1} + x _ {2} ^ {2} & \leq & 3, \\ & x _ {1} ^ {2} - x _ {2} & = & 3, \\ & (x _ {1}, x _ {2}) & \geq & 0. \end{array}
$$

Find a solution to this problem using the generalized reduced gradient approach. 

## 5.5.2 Sequential Quadratic Programming

Consider a general nonlinear optimization problem: 

$$
\begin{array}{r c l} \min _ {x} & f (x) \\ & g _ {i} (x) = 0, i \in \mathcal {E} \\ & g _ {i} (x) \geq 0, i \in \mathcal {I}. \end{array}\tag{5.20}
$$

To solve this problem, one might try to capitalize on the good algorithms available for solving the more structured and easier quadratic programs (see Chapter 7). This is the idea behind sequential quadratic programming. At the current feasible point $x ^ { k }$ , the problem (5.20) is approximated by a quadratic program: a quadratic approximation of the Lagrangian function is computed as well as linear approximations of the constraints. The resulting quadratic program is of the form 

$$
\begin{array}{l l} \min & \nabla f (x ^ {k}) ^ {T} (x - x ^ {k}) + \frac {1}{2} (x - x ^ {k}) ^ {T} B _ {k} (x - x ^ {k}) \\ & \nabla g _ {i} (x ^ {k}) ^ {T} (x - x ^ {k}) + g _ {i} (x ^ {k}) = 0 \quad \text {for all} i \in \mathcal {E} \\ & \nabla g _ {i} (x ^ {k}) ^ {T} (x - x ^ {k}) + g _ {i} (x ^ {k}) \geq 0 \quad \text {for all} i \in \mathcal {I} \end{array}\tag{5.21}
$$

where 

$$
{B ^ {k}} = {\nabla_ {x x} ^ {2} \mathcal {L} (x ^ {k}, \lambda^ {k})}
$$

is the Hessian of the Lagrangian function (5.11) with respect to the x variables and $\lambda ^ { k }$ is the current estimate of the Lagrange multipliers. 

This problem can be solved with one of the specialized algorithms for quadratic programming problems such as the interior-point methods we discuss in Chapter 7. The optimal solution of the quadratic program is used to determine a search direction. Then a line search or trust region procedure is performed to determine the next iterate. 

Perhaps the best way to think of sequential quadratic programming is as an extension of the optimization version of Newton’s method to constrained problems. Recall that the optimization version of Newton’s method uses a quadratic approximation to the objective function and defines the minimizer of this approximation as the next iterate, much like what we described for the SQP method. Indeed, for an unconstrained problem, the $\mathrm { S Q P }$ is identical to Newton’s method. For a constrained problem, the optimality conditions for the quadratic problem we solve in SQP correspond to the Newton direction for the optimality conditions of the original problem at the current iterate. 

## 5.6. NONSMOOTH OPTIMIZATION: SUBGRADIENT METHODS 111

Sequential quadratic programming iterates until the solution converges. Much like Newton’s method, the SQP approaches are very powerful, especially if equipped with line search or trust region methodologies to navigate the nonlinearities and nonconvexities. We refer the reader to the survey of Boggs and Tolle [14] and the text by Nocedal and Wright [55] for further details on the sequential quadratic programming approach. 

Exercise 5.16 Consider the following nonlinear optimization problem with equality constraints: 

$$
\begin{array}{r c l r c l r c l r c l} \min & f (\mathbf {x}) & = & x _ {1} ^ {2} & + & x _ {2} & + & x _ {3} ^ {2} & + & x _ {4} \\ & g _ {1} (\mathbf {x}) & = & x _ {1} ^ {2} & + & x _ {2} & + & 4 x _ {3} & + & 4 x _ {4} & - & 4 & = & 0 \\ & g _ {2} (\mathbf {x}) & = & - x _ {1} & + & x _ {2} & + & 2 x _ {3} & - & 2 x _ {4} ^ {2} & + & 2 & = & 0. \end{array}
$$

Construct the quadratic programming approximation (5.21) for this problem at point $\mathbf { x } ^ { 0 } = ( 0 , - 8 , 3 , 0 )$ and derive the KKT conditions for this quadratic programming problem. 

## 5.6 Nonsmooth Optimization: Subgradient Methods

In this section, we consider unconstrained nonlinear programs of the form 

$$
\min f (\mathbf {x})
$$

where $\mathbf { x } = ( x _ { 1 } , \ldots , x _ { n } )$ and $f$ is a nondiferentiable convex function. Optimality conditions based on the gradient are not available since the gradient is not defined in this case. However, the notion of gradient can be generalized as follows. A subgradient of $f$ at point $x ^ { * }$ is a vector $s ^ { * } = ( s _ { 1 } ^ { * } , \ldots , s _ { n } ^ { * } )$ such that 

$$
s ^ {*} (x - x ^ {*}) \leq f (x) - f (x ^ {*}) \text {   for   every   } x.
$$

When the function $f$ is diferentiable, the subgradient is identical to the gradient. When $f$ is not diferentiable at point $x ,$ there are typically many subgradients at x. For example, consider the convex function of one variable 

$$
f (x) = \max \{1 - x, x - 1 \} = | x - 1 |.
$$

As is evident from Figure 5.6 this function is nondiferentiable at the point $x = 1$ and it is easy to verify that any vector s such that $- 1 \leq s \leq 1$ is a subgradient of $f$ at point $x = 1$ . Some of these subgradients and the linear approximations defined by them are shown in Figure 5.6. Note that each subgradient of the function at a point defines a linear “tangent” to the function that stays always below the plot of the function–this is the defining property of subgradients. 

Consider a nondiferentiable convex function $f .$ . The point $x ^ { * }$ is a minimum of f if and only if $f$ has a zero subgradient at $x ^ { * }$ . In the above example, 0 is a subgradient of $f$ at point $x ^ { * } = 1$ and therefore this is where the minimum of $f$ is achieved. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/73f275041b52bf7e8a847a9c28fae26dbc59f94321d0f168d20d30761b8f2921.jpg)



Figure 5.6: Subgradients provide under-estimating approximations to functions


The method of steepest descent can be extended to nondiferentiable convex functions by computing any subgradient direction and using the opposite direction to make the next step. Although subgradient directions are not always directions of ascent, one can nevertheless guarantee convergence to the optimum point by choosing the step size appropriately. 

A generic subgradient method can be stated as follows. 

1. Initialization: Start from any point $x ^ { 0 }$ . Set $i = 0$ 

2. Iteration i: Compute a subgradient $s ^ { i }$ of $f$ at point $x ^ { i }$ . If $s ^ { i }$ is 0 or close to 0, stop. Otherwise, let $x ^ { i + 1 } = x ^ { i } - \alpha _ { i } s ^ { i }$ , where $\alpha _ { i } > 0$ denotes a step size, and perform the next iteration. 

Several choices of the step size $\alpha _ { i }$ have been proposed in the literature. To guarantee convergence to the optimum, the step size $\alpha _ { i }$ needs to be decreased very slowly (for example $\alpha _ { i } \to 0$ such that $\textstyle \sum _ { i } \alpha _ { i } = + \infty$ will do). But the slow decrease in $\alpha _ { i }$ Presults in slow convergence of $x _ { i }$ to the optimum. In practice, in order to get fast convergence, the following choice is popular: start from $\alpha _ { 0 } = 2$ and then half the step size if no improvement in the objective value $f ( x ^ { i } )$ is observed for k consecutive iterations $( k = 7$ or 8 is often used). This choice is well suited when one wants to get close to the optimum quickly and when finding the exact optimum is not important (this is the case in integer programming applications where subgradient optimization is used to obtain quick bounds in branch-and-bound algorithms). With this in mind, a stopping criterion that is frequently used in practice is a maximum number of iterations (say 200) instead of $^ { 6 6 } s ^ { i }$ is 0 or close to $0 ^ { \dag }$ 

We will see in Chapter 12 how subgradient optimization is used in a model to construct an index fund. 

# NLP Models: Volatility Estimation

Volatility is a term used to describe how much the security prices, market indices, interest rates, etc. move up and down around their mean. It is measured by the standard deviation of the random variable that represents the financial quantity we are interested in. Most investors prefer low volatility to high volatility and therefore expect to be rewarded with higher long-term returns for holding higher volatility securities. 

Many financial computations require volatility estimates. Mean-variance optimization trades of the expected return and volatility of a portfolio of securities. Celebrated option valuation formulas of Black, Scholes, and Merton (BSM) involve the volatility of the underlying security. Risk management revolves around the volatility of the current positions. Therefore, accurate estimation of the volatilities of security returns, interest rates, exchange rates and other financial quantities is crucial to many quantitative techniques in financial analysis and management. 

Most volatility estimation techniques can be classified as either a historical or an implied method. One either uses historical time series to infer patterns and estimates the volatility using a statistical technique, or considers the known prices of related securities such as options that may reveal the market sentiment on the volatility of the security in question. GARCH models exemplify the first approach while the implied volatilities calculated from the BSM formulas are the best known examples of the second approach. Both types of techniques can benefit from the use of optimization formulations to obtain more accurate volatility estimates with desirable characteristics such as smoothness. We discuss two examples in the remainder of this chapter. 

## 6.1 Volatility Estimation with GARCH Models

Empirical studies analyzing time series data for returns of securities, interest rates, and exchange rates often reveal a clustering behavior for the volatility of the process under consideration. Namely, these time series exhibit high volatility periods alternating with low volatility periods. These observations suggest that future volatility can be estimated with some degree of confidence by relying on historical data. 

Currently, describing the evolution of such processes by imposing a stationary model on the conditional distribution of returns is one of the most popular approaches in the econometric modeling of financial time series. This approach expresses the conventional wisdom that models for financial returns should adequately represent the nonlinear dynamics that are demonstrated by the sample autocorrelation and cross-correlation functions of these time series. ARCH (autoregressive conditional heteroscedasticity) and GARCH (generalized ARCH) models of Engle [25] and Bollerslev [15] have been popular and successful tools for future volatility estimation. For the multivariate case, rich classes of stationary models that generalize the univariate GARCH models have also been developed; see, for example, the comprehensive survey by Bollerslev et al. [16]. 

The main mathematical problem to be solved in fitting ARCH and GARCH models to observed data is the determination of the best model parameters that maximize a likelihood function, i.e., an optimization problem. Typically, these models are presented as unconstrained optimization problems with recursive terms. In a recent study, Altay-Salih et al. [1] argue that because of the recursion equations and the stationarity constraints, these models actually fall into the domain of nonconvex, nonlinearly constrained nonlinear programming. This study shows that using a sophisticated nonlinear optimization package (sequential quadratic programming based FILTER method of Fletcher and Leyfer [28] in their case) they are able to significantly improve the log-likelihood functions for multivariate volatility (and correlation) estimation. While this study does not provide a comparison of forecasting efectiveness of the standard approaches to that of the constrained optimization approach, the numerical results suggest that constrained optimization approach provides a better prediction of the extremal behavior of the time series data; see [1]. Here, we briefly review this constrained optimization approach for expository purposes. 

We consider a stochastic process Y indexed by natural numbers. $Y _ { t } ,$ its value at time t, is an n-dimensional vector of random variables. Autoregressive behavior of these random variables is modeled as: 

$$
Y _ {t} = \sum_ {i = 1} ^ {m} \phi_ {i} Y _ {t - i} + \varepsilon_ {t}\tag{6.1}
$$

where m is a positive integer representing the number of periods we look back in our model and $\varepsilon _ { t }$ satisfies 

$$
E [ \varepsilon_ {t} | \varepsilon_ {1}, \ldots , \varepsilon_ {t - 1} ] = 0.
$$

While these models are of limited value, if at all, in the estimation of the actual time series $( Y _ { t } )$ , they have been shown to provide useful information for volatility estimation. For this purpose, GARCH models define 

$$
{h _ {t}} {:=} {E [ \varepsilon_ {t} ^ {2} | \varepsilon_ {1}, \ldots , \varepsilon_ {t - 1} ]}
$$

in the univariate case and 

$$
{H _ {t}} {:=} {E [ \varepsilon_ {t} \varepsilon_ {t} ^ {T} | \varepsilon_ {1}, \ldots , \varepsilon_ {t - 1} ]}
$$

in the multivariate case. Then one models the conditional time dependence of these squared residuals in the univariate case as follows: 

$$
h _ {t} = c + \sum_ {i = 1} ^ {q} \alpha_ {i} \varepsilon_ {t - i} ^ {2} + \sum_ {j = 1} ^ {p} \beta_ {j} h _ {t - j}.\tag{6.2}
$$

This model is called $\mathrm { G A R C H } ( p , q )$ . Note that ARCH models correspond to choosing $p = 0$ 

The generalization of the model (6.2) to the multivariate case can be done in a number of ways. One approach is to use the operator vech to turn the matrices $H _ { t }$ and $\varepsilon _ { t } \varepsilon _ { t } ^ { T }$ into vectors. The operator vech takes an $n \times n$ symmetric matrix as an input and produces an $\textstyle { \frac { n ( n + 1 ) } { 2 } }$ -dimensional vector as output by stacking the elements of the matrix on and below the diagonal on top of each other. Using this operator, one can write a multivariate generalization of (6.2) as follows: 

$$
\mathbf {v e c h} (H _ {t}) = \mathbf {v e c h} (C) + \sum_ {i = 1} ^ {q} A _ {i} \mathbf {v e c h} (\varepsilon_ {t - i} \varepsilon_ {t - i} ^ {T}) + \sum_ {j = 1} ^ {p} B _ {j} \mathbf {v e c h} (H _ {t - j}) (6. 3)
$$

In (6.3), $A _ { i } { } ^ { : }$ ’s and $B _ { j }$ ’s are square matrices of dimension $\textstyle { \frac { n ( n + 1 ) } { 2 } }$ and $C$ is an $n \times n$ symmetric matrix. 

After choosing a superstructure for the GARCH model, that is, after choosing p and $q ,$ the objective is to determine the optimal parameters $\phi _ { i } .$ $\alpha _ { i } .$ , and $\beta _ { j }$ . Most often, this is achieved via maximum likelihood estimation. If one assumes a normal distribution for $Y _ { t }$ conditional on the historical observations, the log-likelihood function can be written as follows [1]: 

$$
- \frac {T}{2} \log 2 \pi - \frac {1}{2} \sum_ {t = 1} ^ {T} \log h _ {t} - \frac {1}{2} \sum_ {t = 1} ^ {T} \frac {\varepsilon_ {t} ^ {2}}{h _ {t}},\tag{6.4}
$$

in the univariate case and 

$$
- \frac {T}{2} \log 2 \pi - \frac {1}{2} \sum_ {t = 1} ^ {T} \log \det H _ {t} - \frac {1}{2} \sum_ {t = 1} ^ {T} \varepsilon_ {t} ^ {T} H _ {t} ^ {- 1} \varepsilon_ {t}\tag{6.5}
$$

in the multivariate case. 

Exercise 6.1 Show that the function in $\left( 6 . 4 \right)$ is a diference of convex functions by showing that log $h _ { t }$ is concave and $\frac { \varepsilon _ { t } ^ { 2 } } { h _ { t } }$ is convex in $\varepsilon _ { t }$ and $h _ { t }$ . Does the same conclusion hold for the function in (6.5)? 

Now, the optimization problem to solve in the univariate case is to maximize the log-likelihood function (6.4) subject to the model constraints (6.1) and (6.2) as well as the condition that $h _ { t }$ is nonnegative for all t since $h _ { t } = E [ \varepsilon _ { t } ^ { 2 } | \varepsilon _ { 1 } , \dots , \varepsilon _ { t - 1 } ]$ . In the multivariate case we maximize (6.5) subject to the model constraints (6.1) and (6.3) as well as the condition that $H _ { t }$ is a positive semidefinite matrix for all t since $H _ { t }$ defined as $E [ \varepsilon _ { t } \varepsilon _ { t } ^ { T } | \varepsilon _ { 1 } , \dots , \varepsilon _ { t - 1 } ]$ must necessarily satisfy this condition. The positive semidefiniteness of the matrices $H _ { t }$ can either be enforced using the techniques discussed in Chapter 9 or using a reparametrization of the variables via Cholesky-type $L D L ^ { T }$ decomposition as discussed in [1]. 

An important issue in GARCH parameter estimation is the stationarity properties of the resulting model. There is a continuing debate about whether it is reasonable to assume that the model parameters for financial time series are stationary over time. It is, however, clear that the estimation and forecasting is easier on stationary models. A suficient condition for the stationarity of the univariate GARCH model above is that $\alpha _ { i } { ' }$ s and $\beta _ { j } '$ s as well as the scalar c are strictly positive and that 

$$
\sum_ {i = 1} ^ {q} \alpha_ {i} + \sum_ {j = 1} ^ {p} \beta_ {j} <   1,\tag{6.6}
$$

see, for example, [33]. The suficient condition for the multivariate case is more involved and we refer the reader to [1] for these details. 

Especially in the multivariate case, the problem of maximizing the loglikelihood function with respect to the model constraints is a dificult nonlinear, non-convex optimization problem. To find a quick solution, more tractable versions of the model (6.3) have been developed where the model is simplified by imposing additional structure on the matrices $A _ { i }$ and $B _ { j }$ such as diagonality. While the resulting problems are easier to solve, the loss of generality from their simplifying assumptions can be costly. As Altay-Salih et al. demonstrate, using the full power of state-of-the-art constrained optimization software, one can solve the more general model in reasonable computational time (at least for bivariate and trivariate estimation problems) with much improved log-likelihood values. While the forecasting eficiency of this approach is still to be tested, it is clear that sophisticated nonlinear optimization is emerging as a valuable tool in volatility estimation problems that use historical data. 

Exercise 6.2 Consider the model in (6.3) for the bivariate case when $q = 1$ and $p = 0 ~ { \mathrm { ( i . e . } }$ , an ARCH(1) model). Explicitly construct the nonlinear programming problem to be solved in this case. The comparable simplification of the BEKK representation [3] gives 

$$
H _ {t} = C ^ {T} C + A ^ {T} \varepsilon_ {t - 1} \varepsilon_ {t - 1} ^ {t} A.
$$

Compare these two models and comment on the additional degrees of freedom in the NLP model. Note that the BEKK representation ensures the positive semidefiniteness of $H _ { t }$ by construction at the expense of lost degrees of freedom. 

Exercise 6.3 Test the NLP model against the model resulting from the BEKK representation in the previous exercise using daily return data for two market indices, $\mathrm { e . g . }$ , S & P 500 and FTSE 100, and an NLP solver. Compare the optimal log-likelihood values achieved by both models and comment. 

## 6.2 Estimating a Volatility Surface

The discussion in this section is largely based on the work of Coleman, Kim, Li, and Verma, see [21, 20]. 

The BSM equation for pricing European options is based on a geometric Brownian motion model for the movements of the underlying security. Namely, one assumes that the underlying security price $S _ { t }$ at time t satisfies 

$$
{\frac {d S _ {t}}{S _ {t}}} = {\mu d t + \sigma d W _ {t}}\tag{6.7}
$$

where $\mu$ is the drift, σ is the (constant) volatility, and $W _ { t }$ is the standard Brownian motion. Using this equation and some standard assumptions about the absence of frictions and arbitrage opportunities, one can derive the BSM partial diferential equation for the value of a European option on this underlying security. Using the boundary conditions resulting from the payof structure of the particular option, one determines the value function for the option. Recall from Exercise 5.3 that the price of a European call option with strike K and maturity $T$ is given by: 

$$
{ C ( K , T ) } { = } { S _ { 0 } \Phi ( d _ { 1 } ) - K e ^ { - r T } \Phi ( d _ { 2 } ) , }\tag{6.8}
$$

where 

$$
\begin{array}{r c l} {d _ {1}} & = & {\frac {\log (\frac {S _ {0}}{K}) + (r + \frac {\sigma^ {2}}{2}) T}{\sigma \sqrt {T}},} \\ {d _ {2}} & = & {d _ {1} - \sigma \sqrt {T},} \end{array}
$$

and $\Phi ( \cdot )$ is the cumulative distribution function for the standard normal distribution. $r$ in the formula represents the continuously compounded riskfree and constant interest rate and $\sigma$ is the volatility of the underlying security that is assumed to be constant. Similarly, the European put option price is given by 

$$
P (K, T) = K e ^ {- r T} \Phi (- d _ {2}) - S _ {0} \Phi (- d _ {1}).\tag{6.9}
$$

The risk-free interest rate r, or a reasonably close approximation to it is often available, for example from Treasury bill prices in US markets. Therefore, all one needs to determine the call or put price using these formulas is a reliable estimate of the volatility parameter $\sigma .$ . Conversely, given the market price for a particular European call or put, one can uniquely determine the volatility of the underlying asset implied by this price, called its implied volatility, by solving the equations above with the unknown $\sigma .$ . Any one of the univariate equation solving techniques we discussed in Section 5.3 can be used for this purpose. 

Empirical evidence against the appropriateness of (6.7) as a model for the movements of most securities is abundant. Most studies refute the assumption of a volatility that does not depend on time or underlying price level. Indeed, studying the prices of options with same maturity but different strikes, researchers observed that the implied volatilities for such options often exhibit a “smile” structure, i.e., higher implied volatilities away from the money in both directions, decreasing to a minimum level as one approaches the at-the-money option from in-the-money or out-of-the-money strikes. This is clearly in contrast with the constant (flat) implied volatilities one would expect had (6.7) been an appropriate model for the underlying price process. 

There are many models that try to capture the volatility smile including stochastic volatility models, jump difusions, etc. Since these models introduce non-traded sources of risk, perfect replication via dynamic hedging as in BSM approach becomes impossible and the pricing problem is more complicated. An alternative that is explored in [21] is the one-factor continuous difusion model: 

$$
\frac {d S _ {t}}{S _ {t}} = \mu (S _ {t}, t) d t + \sigma (S _ {t}, t) d W _ {t}, t \in [ 0, T ]\tag{6.10}
$$

where the constant parameters $\mu$ and σ of (6.7) are replaced by continuous and diferentiable functions $\mu ( S _ { t } , t )$ and $\sigma ( S _ { t } , t )$ of the underlying price $S _ { t }$ and time t. T denotes the end of the fixed time horizon. If the instantaneous risk-free interest rate r is assumed constant and the dividend rate is constant, given a function $\sigma ( S , t )$ , a European call option with maturity T and strike $K$ has a unique price. Let us denote this price with $C ( \sigma ( S , t ) , K , T )$ 

While an explicit solution for the price function $C ( \sigma ( S , t ) , K , T )$ as in (6.8) is no longer possible, the resulting pricing problem can be solved eficiently via numerical techniques. Since $\mu ( S , t )$ does not appear in the generalized BSM partial diferential equation, all one needs is the specification of the function $\sigma ( S , t )$ and a good numerical scheme to determine the option prices in this generalized framework. 

So, how does one specify the function $\sigma ( S , t ) ?$ First of all, this function should be consistent with the observed prices of currently or recently traded options on the same underlying security. If we assume that we are given market prices of $m$ call options with strikes $K _ { j }$ and maturities $T _ { j }$ in the form of bid-ask pairs $( \beta _ { j } , \alpha _ { j } )$ for $j = 1 , \dots , n ,$ it would be reasonable to require that the volatility function $\sigma ( S , t )$ is chosen so that 

$$
\beta_ {j} \leq C (\sigma (S, t), K _ {j}, T _ {j}) \leq \alpha_ {j}, j = 1, \ldots , n.\tag{6.11}
$$

To ensure that (6.11) is satisfied as closely as possible, one strategy is to minimize the violations of the inequalities in (6.11): 

$$
\min _ {\sigma (S, t) \in \mathcal {H}} \sum_ {j = 1} ^ {n} [ \beta_ {j} - C (\sigma (S, t), K _ {j}, T _ {j}) ] ^ {+} + [ C (\sigma (S, t), K _ {j}, T _ {j}) - \alpha_ {j} ] ^ {+}.\tag{6.12}
$$

Above, denotes the space of measurable functions $\sigma ( S , t )$ with domain $I R ^ { + } \times [ 0 , T ]$ and $u ^ { + } = \operatorname* { m a x } \{ 0 , u \}$ . Alternatively, using the closing prices $C _ { j }$ for the options under consideration, or choosing the mid-market prices $\dot { C _ { j } } = ( \beta _ { j } + \alpha _ { j } ) / 2$ , we can solve the following nonlinear least squares problem: 

$$
\min _ {\sigma (S, t) \in \mathcal {H}} \sum_ {j = 1} ^ {n} \left(C (\sigma (S, t), K _ {j}, T _ {j}) - C _ {j}\right) ^ {2}.\tag{6.13}
$$

This is a nonlinear least squares problem since the function $C ( \sigma ( S , t ) , K _ { j } , T _ { j } )$ depends nonlinearly on the variables, namely the local volatility function $\sigma ( S , t )$ 

While the calibration of the local volatility function to the observed prices using the objective functions in (6.12) and (6.13) is important and desirable, there are additional properties that are desirable in the local volatility function. Arguably, the most common feature sought in existing models is smoothness. For example, in [46] authors try to achieve a smooth volatility function by appending the objective function in (6.13) as follows: 

$$
\min _ {\sigma (S, t) \in \mathcal {H}} \sum_ {j = 1} ^ {n} \left(C (\sigma (S, t), K _ {j}, T _ {j}) - C _ {j}\right) ^ {2} + \lambda \| \nabla \sigma (S, t) \| _ {2}.\tag{6.14}
$$

Here, λ is a positive trade-of parameter and $\| \cdot \| _ { 2 }$ represents the $L ^ { 2 } .$ -norm. Large deviations in the volatility function would result in a high value for the norm of the gradient function and by penalizing such occurrences, the formulation above encourages a smoother solution to the problem. The most appropriate value for the trade-of parameter λ must be determined experimentally. To solve the resulting problem numerically, one must discretize the volatility function on the underlying price and time grid. Even for a relatively coarse discretization of the $S _ { t }$ and t spaces, one can easily end up with an optimization problem with many variables. 

An alternative strategy is to build the smoothness into the volatility function by modeling it with spline functions. To define a spline function, the domain of the function is partitioned into smaller subregions and then, the spline function is chosen to be a polynomial function in each subregion. Since polynomials are smooth functions, spline functions are smooth within each subregion by construction and the only possible sources of nonsmoothness are the boundary regions between subregions. When the polynomial is of a high enough degree, the continuity and diferentiability of the spline function at the boundaries between subregions can be ensured by properly choosing the polynomial function coeficients. This strategy is similar to the model we consider in more detail in Section 8.4, except that here we model the volatility function rather than the risk-neutral density and also we generate a function that varies over time rather than an estimate at a single point in time. We defer a more detailed discussion of spline functions to Section 8.4. The use of the spline functions not only guarantees the smoothness of the resulting volatility function estimates but also reduces the degrees of freedom in the problem. As a consequence, the optimization problem to be solved has much fewer variables and is easier. This strategy is proposed in [21] and we review it below. 

We start by assuming that $\sigma ( S , t )$ is a bi-cubic spline. While higher-order splines can also be used, cubic splines often ofer a good balance between flexibility and complexity. Next we choose a set of spline knots at points $( \bar { S } _ { j } , \bar { t } _ { j } )$ for $j = 1 , \dots , k$ . If the value of the volatility function at these points is given by $\bar { \sigma } _ { j } : = \sigma ( \bar { S } _ { j } , \bar { t } _ { j } )$ , the interpolating cubic spline that goes through these knots and satisfies a particular end condition is uniquely determined. For example, in Section 8.4 we use the natural spline end condition which sets the second derivative of the function at the knots at the boundary of the domain to zero to obtain our cubic spline approximations uniquely. Therefore, to completely determine the volatility function as a natural bicubic spline and to determine the resulting call option prices we have k degrees of freedom represented with the choices $\bar { \sigma } = ( \bar { \sigma } _ { 1 } , \dots , \bar { \sigma } _ { k } )$ 

Let $\Sigma ( S , t , \bar { \sigma } )$ the bi-cubic spline local volatility function obtained setting $\sigma ( \bar { S } _ { j } , \bar { t } _ { j } ) ^ { \dag }$ s to $\bar { \sigma } _ { j }$ . Let $C ( \Sigma ( S , t , \bar { \sigma } ) , S , t )$ denote the resulting call price function. The analog of the objective function (6.13) is then 

$$
\min _ {\bar {\sigma} \in \mathbb {R} ^ {k}} \sum_ {j = 1} ^ {n} \left(C (\Sigma (S, t, \bar {\sigma}), K _ {j}, T _ {j}) - C _ {j}\right) ^ {2}.\tag{6.15}
$$

One can introduce positive weights $w _ { j }$ for each of the terms in the objective function above to address diferent accuracies or confidence in the call prices $C _ { j }$ . We can also introduce lower and upper bounds $l _ { i }$ and $u _ { i }$ for the volatilities at each knot to incorporate additional information that may be available from historical data, etc. This way, we form the following nonlinear least-squares problem with k variables: 

$$
\begin{array}{l l} \min _ {\bar {\sigma} \in \mathbb {R} ^ {k}} & f (\sigma) := \sum_ {j = 1} ^ {n} w _ {j} \left(C (\Sigma (S, t, \bar {\sigma}), K _ {j}, T _ {j}) - C _ {j}\right) ^ {2} \\ \text {s.t.} & l \leq \bar {\sigma} \leq u. \end{array}\tag{6.16}
$$

It should be noted that the formulation above will not be appropriate if there are many more knots than prices, that is if k is much larger than n. In this case, the problem will be underdetermined and solutions may exhibit consequences of “over-fitting”. It is better to use fewer knots than available option prices. 

The problem (6.16) is a standard nonlinear optimization problem except that the term $C ( \Sigma ( S , t , \bar { \sigma } ) , K _ { j } , T _ { j } )$ in the objective function depends on the decision variables σ¯ in a complicated and non-explicit manner. Since most of the nonlinear optimization methods we discussed in the previous chapter require at least the gradient of the objective function (and sometimes its Hessian matrix as well), is potentially troublesome. Without an explicit expression for $f ,$ , its gradient must be either estimated using a finite diference scheme or using automatic diferentiation. Coleman et al. implement both alternatives and report that local volatility functions can be estimated very accurately using these strategies. They also test the hedging accuracy 

## 6.2. ESTIMATING A VOLATILITY SURFACE

of diferent delta-hedging strategies, one using a constant volatility estimation and another using the local volatility function produced by the strategy above. These tests indicate that the hedges obtained from the local volatility function are significantly more accurate. 

Exercise 6.4 The partial derivative $\partial f ( \boldsymbol { x } ) / \partial \boldsymbol { x } _ { i }$ of the function $f ( x )$ with respect to the i-th coordinate of the x vector can be estimated as 

$$
\frac {\partial f (x)}{\partial x _ {i}} \approx \frac {f (x + h e _ {i}) - f (x)}{h},
$$

where $e _ { i }$ denotes the i-th unit vector. Assuming that f is continuously differentiable, provide an upper bound on the estimation error from this finite diference approximation using Taylor series expansion for the function f around x. Next, compute a similar bound for the alternative finite diference formula given by 

$$
\frac {\partial f (x)}{\partial x _ {i}} \approx \frac {f (x + h e _ {i}) - f (x - h e _ {i})}{2 h}.
$$

Comment on the potential advantages and disadvantages of these two approaches. 

Chapter 7 

# Quadratic Programming: Theory and Algorithms

## 7.1 The Quadratic Programming Problem

As we discussed in the introductory chapter, quadratic programming (QP) refers to the problem of minimizing a quadratic function subject to linear equality and inequality constraints. In its standard form, this problem is represented as follows: 

$$
\begin{array}{r c l} (\mathcal {Q P}) & \min _ {x} & \frac {1}{2} x ^ {T} Q x + c ^ {T} x \\ & A x & = b \\ & x & \geq 0, \end{array}\tag{7.1}
$$

where $A \in I R ^ { m \times n } , b \in I R ^ { m } , c \in I R ^ { n } , Q \in I R ^ { n \times n }$ are given, and $x \in \mathbb { R } ^ { n }$ QPs are special classes of nonlinear optimization problems and contain linear programming problems as special cases. 

Quadratic programming structures are encountered frequently in optimization models. For example, ordinary least squares problems which are used often in data fitting are QPs with no constraints. Mean-variance optimization problems developed by Markowitz for the selection of eficient portfolios are QP problems. In addition, QP problems are solved as subproblems in the solution of general nonlinear optimization problems via sequential quadratic programming (SQP) approaches; see Section 5.5.2. 

Recall that, when $Q$ is a positive semidefinite matrix, i.e., when $y ^ { T } Q y \ge$ 0 for all y, the objective function of problem $\mathcal { Q P }$ is a convex function of x. Since the feasible set is a polyhedral set (i.e., a set defined by linear constraints) it is a convex set. Therefore, when Q is positive semidefinite, the QP (7.1) is a convex optimization problem. As such, its local optimal solutions are also global optimal solutions. This property is illustrated in Figure 7.1 where the contours of a quadratic function with a positive semidefinite $Q$ are contrasted with those of an indefinite $Q .$ 

Exercise 7.1 Consider the quadratic function $\begin{array} { r } { f ( x ) = c ^ { T } x + \frac { 1 } { 2 } x ^ { T } Q x } \end{array}$ , where the matrix $Q$ is n by n and symmetric. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/26920848891a404a1d4209a81648269f1f9ab8b20822f7efd8461c7aa7a8eab5.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/ad9056c92a9f58c133006a94c005840edb8c9a863f33bae4a8a4b0ee4fa36c82.jpg)



Figure 7.1: Contours of positive semidefinite and indefinite quadratic functions


a. Prove that if $x ^ { T } Q x < 0$ for some x, then $f$ is unbounded below. 

b. Prove that if $Q$ is positive semidefinite (but not positive definite), then either $f$ is unbounded below or it has an infinite number of solutions. 

c. True or false: $f$ has a unique minimizer if and only if Q is positive definite. 

As in linear programming, we can develop a dual of quadratic programming problems. The dual of the problem (7.1) is given below: 

$$
\begin{array}{r c l r c l r c l} (\mathcal {Q D}) & \max _ {x, y, s} & b ^ {T} y & - & \frac {1}{2} x ^ {T} Q x \\ & & A ^ {T} y & - & Q x & + & s & = & c \\ & & & & x & , & s & \geq & 0. \end{array}\tag{7.2}
$$

Note that, unlike the case of linear programming, the variables of the primal quadratic programming problem also appear in the dual QP. 

## 7.2 Optimality Conditions

One of the fundamental tools in the study of optimization problems is the Karush-Kuhn-Tucker theorem that gives a list of conditions which are necessarily satisfied at any (local) optimal solution of a problem, provided that some mild regularity assumptions are satisfied. These conditions are commonly called KKT conditions and were already discussed in the context of general nonlinear optimization problems in Section 5.5. 

Applying the KKT theorem to the QP problem (7.1), we obtain the following set of necessary conditions for optimality: 

Theorem 7.1 Suppose that x is a local optimal solution of the $Q P$ given in (7.1) so that it satisfies $A x = b , \ x \geq 0$ and assume that Q is a positive semidefinite matrix. Then, there exist vectors y and s such that the following 

## 7.2. OPTIMALITY CONDITIONS

conditions hold: 

$$
A ^ {T} y - Q x + s = c
$$

$$
s \geq 0\tag{7.3}
$$

(7.4) 

$$
x _ {i} s _ {i} = 0, \forall i.\tag{7.5}
$$

Furthermore, x is a global optimal solution. 

Note that the positive semidefiniteness condition related to the Hessian of the Lagrangian function in the KKT theorem is automatically satisfied for convex quadratic programming problems, and therefore is not included in Theorem 7.1. 

Exercise 7.2 Show that in the case of a positive definite Q, the objective function of (7.1) is strictly convex, and therefore, must have a unique minimizer. 

Conversely, if vectors x, y and s satisfy conditions (7.3)-(7.5) as well as primal feasibility conditions 

$$
A x = b\tag{7.6}
$$

$$
x \geq 0\tag{7.7}
$$

then, x is a global optimal solution of (7.1). In other words, conditions (7.3)-(7.7) are both necessary and suficient for $x , \ y .$ and s to describe a global optimal solution of the QP problem. 

In a manner similar to linear programming, optimality conditions (7.3)- (7.7) can be seen as a collection of conditions for 

1. primal feasibility: $A x = b , x \geq 0$ 7 

2. dual feasibility: $A ^ { T } y - Q x + s = c , \ s \geq 0$ , and 

3. complementary slackness: for each $i = 1 , \ldots , n$ we have $x _ { i } s _ { i } = 0$ 

Using this interpretation, one can develop modifications of the simplex method that can also solve convex quadratic programming problems (Wolfe’s method). We do not present this approach here. Instead, we describe an alternative algorithm that is based on Newton’s method; see Section 5.4.2. 

Exercise 7.3 Consider the following quadratic program 

subject to 

$$
\begin{array}{r c l c l c l c l} \min & x _ {1} x _ {2} & + & x _ {1} ^ {2} & + & \frac {3}{2} x _ {2} ^ {2} & + & 2 x _ {3} ^ {2} \\ & & + & 2 x _ {1} & + & x _ {2} & + & 3 x _ {3} \\ \text {t to} & & & x _ {1} & + & x _ {2} & + & x _ {3} & = & 1 \\ & & & x _ {1} & - & x _ {2} & & & = & 0 \\ & & & x _ {1} \geq 0, & x _ {2} \geq 0, & x _ {3} \geq 0. \end{array}
$$

Is the quadratic objective function convex? Show that $x ^ { * } = ( { \textstyle \frac { 1 } { 2 } } , { \textstyle \frac { 1 } { 2 } } , 0 )$ is an optimal solution to this problem by finding vectors y and s that satisfy the optimality conditions jointly with $x ^ { * }$ 

## 7.3 Interior-Point Methods

In 1984, Karmarkar proved that an Interior-Point Method (IPM) can solve LPs in polynomial time. The two decades that followed the publication of Karmarkar’s paper have seen a very intense efort by the optimization research community to study theoretical and practical properties of IPMs. One of the early discoveries was that IPMs can be viewed as modifications of Newton’s method that are able to handle inequality constraints. Some of the most important contributions were made by Nesterov and Nemirovski who showed that the IPM machinery can be applied to a much larger class of problems than just LPs [54]. Convex quadratic programming problems, for example, can be solved in polynomial time, as well as many other convex optimization problems using IPMs. For most instances of conic optimization problems we discuss in Chapter 9 and 10, IPMs are by far the best available methods. 

Here, we will describe a variant of IPMs for convex quadratic programming. For the QP problem in (7.1) we can write the optimality conditions in matrix form as follows: 

$$
F (x, y, s) = \left[ \begin{array}{c} A ^ {T} y - Q x + s - c \\ A x - b \\ X S e \end{array} \right] = \left[ \begin{array}{c} 0 \\ 0 \\ 0 \end{array} \right], (x, s) \geq 0.\tag{7.8}
$$

Above, X and S are diagonal matrices with the entries of the x and s vectors, respectively, on the diagonal, i.e., $X _ { i i } = x _ { i }$ , and $X _ { i j } = 0 , i \neq j$ , and similarly for S. Also, as before, e is an n-dimensional vector of ones. 

The system of equations $F ( x , y , s ) = 0$ has $n { + } m { + } n$ variables and exactly the same number of constraints, i.e., it is $\mathrm { a \ ^ { 6 } s q u a r e ^ { 3 } }$ system. Because of the nonlinear equations $x _ { i } s _ { i } = 0$ we cannot solve this system using linear system solution methods such as Gaussian elimination. But, since the system is square we can apply Newton’s method. In fact, without the nonnegativity constraints, finding $( x , y , s )$ satisfying these optimality conditions would be a straightforward exercise by applying Newton’s method. 

The existence of nonnegativity constraints creates a dificulty. The existence and the number of inequality constraints are among the most important factors that contribute to the dificulty of the solution of any optimization problem. Interior-point approaches use the following strategy to handle these inequality constraints: One first identifies an initial solution $( x ^ { 0 } , y ^ { 0 } , s ^ { 0 } )$ that satisfies the first two (linear) blocks of equations in $F ( x , y , s ) = 0$ but not necessarily the third block $X S e = 0$ , and also satisfies the nonnegativity constraints strictly, i.e., $x ^ { 0 } > 0$ and $s ^ { 0 } > 0$ . Notice that a point satisfying some inequality constraints strictly lies in the interior of the region defined by these inequalities–rather than being on the boundary. This is the reason why the method we are discussing is called an interior-point method. 

Once we find such an $( x ^ { 0 } , y ^ { 0 } , s ^ { 0 } )$ we try to generate new points $( x ^ { k } , y ^ { k } , s ^ { k } )$ that also satisfy these same conditions and get progressively closer to satisfying the third block of equations. This is achieved via careful application of a modified Newton’s method. 

## 7.3. INTERIOR-POINT METHODS

Let us start by defining two sets related to the conditions (7.8): 

$$
\mathcal {F} := \{(x, y, s): A x = b, A ^ {T} y - Q x + s = c, x \geq 0, s \geq 0 \}\tag{7.9}
$$

is the set of feasible points, or simply the feasible set. Note that, we are using a primal-dual feasibility concept here. More precisely, since x variables come from the primal QP and $( y , s )$ come from the dual QP, we impose both primal and dual feasibility conditions in the definition of $\mathcal { F }$ . If $( x , y , s ) \in { \mathcal { F } }$ also satisfy $x > 0$ and $s > 0$ we say that $( x , y , s )$ is a strictly feasible solution and define 

$$
\mathcal {F} ^ {o} := \{(x, y, s): A x = b, A ^ {T} y - Q x + s = c, x > 0, s > 0 \}\tag{7.10}
$$

to be the strictly feasible set. In mathematical terms, ${ \mathcal { F } } ^ { o }$ is the relative interior of the set $\mathcal { F }$ 

IPMs we discuss here will generate iterates $( x ^ { k } , y ^ { k } , s ^ { k } )$ that all lie in ${ \mathcal { F } } ^ { o }$ Since we are generating iterates for both the primal and dual problems, this version of IPMs are often called primal-dual interior-point methods. Using this approach, we will obtain solutions for both the primal and dual problems at the end of the solution procedure. Solving the dual may appear to be a waste of time since we are only interested in the solution of the primal problem. However, years of computational experience demonstrated that primal-dual IPMs lead to the most eficient and robust implementations of the interior-point approach. Intuitively speaking, this happens because having some partial information on the dual problem in the form of the dual iterates $( y ^ { k } , s ^ { k } )$ ) helps us make better and faster improvements on the iterates of the primal problem. 

Iterative optimization algorithms have two essential components: 

a measure that can be used to evaluate and compare the quality of alternative solutions and search directions 

a method to generate a better solution, with respect to the measure just mentioned, from a non-optimal solution. 

As we stated before, IPMs rely on Newton’s method to generate new estimates of the solutions. Let us discuss this more in depth. Ignore the inequality constraints in (7.8) for a moment, and focus on the nonlinear system of equations $F ( x , y , s ) = 0$ . Assume that we have a current estimate $( x ^ { k } , y ^ { k } , s ^ { k } )$ of the optimal solution to the problem. The Newton step from this point is determined by solving the following system of linear equations: 

$$
\begin{array}{r l r} {J (x ^ {k}, y ^ {k}, s ^ {k}) \left[ \begin{array}{l} {\Delta x ^ {k}} \\ {\Delta y ^ {k}} \\ {\Delta s ^ {k}} \end{array} \right]} & = & {- F (x ^ {k}, y ^ {k}, s ^ {k}),} \end{array}\tag{7.11}
$$

where $J ( x ^ { k } , y ^ { k } , s ^ { k } )$ is the Jacobian of the function $F$ and $[ \Delta x ^ { k } , \Delta y ^ { k } , \Delta s ^ { k } ] ^ { T }$ is the search direction. First, we observe that 

$$
\begin{array}{r l r} {J (x ^ {k}, y ^ {k}, s ^ {k})} & = & {\left[ \begin{array}{c c c} {- Q} & {A ^ {T}} & {I} \\ {A} & {0} & {0} \\ {S ^ {k}} & {0} & {X ^ {k}} \end{array} \right]} \end{array}\tag{7.12}
$$

where, $X ^ { k }$ and $S ^ { k }$ are diagonal matrices with the components of the vectors $x ^ { k }$ and $s ^ { k }$ along their diagonals. Furthermore, if $( x ^ { k } , y ^ { k } , s ^ { k } ) \in \mathcal { F } ^ { o }$ , then 

$$
F (x ^ {k}, y ^ {k}, s ^ {k}) = \left[ \begin{array}{c} 0 \\ 0 \\ X ^ {k} S ^ {k} e \end{array} \right]\tag{7.13}
$$

and the Newton equation reduces to 

$$
\left[ \begin{array}{c c c} - Q & A ^ {T} & I \\ A & 0 & 0 \\ S ^ {k} & 0 & X ^ {k} \end{array} \right] \left[ \begin{array}{c} \Delta x ^ {k} \\ \Delta y ^ {k} \\ \Delta s ^ {k} \end{array} \right] = \left[ \begin{array}{c} 0 \\ 0 \\ - X ^ {k} S ^ {k} e \end{array} \right].\tag{7.14}
$$

Exercise 7.4 Consider the quadratic programming problem given in Exercise 7.3 and the current primal-dual estimate of the solution $\begin{array} { r } { x ^ { k } = \left( \frac { 1 } { 3 } , \frac { 1 } { 3 } , \frac { 1 } { 3 } \right) ^ { T } } \end{array}$ 2 $y ^ { k } = \left( 1 , { \frac { 1 } { 2 } } \right) ^ { T }$ , and $\begin{array} { r } { s ^ { k } = \left( \frac { 1 } { 2 } , \frac { 1 } { 2 } , 2 \right) ^ { T } } \end{array}$ . Is $( x ^ { k } , y ^ { k } , s ^ { k } ) \in { \mathcal { F } } ?$ How about ${ \mathcal { F } } ^ { o } ?$ Form and solve the Newton equation for this problem at $( x ^ { k } , y ^ { k } , s ^ { k } )$ 

In the standard Newton method, once a Newton step is determined in this manner, it is added to the current iterate to obtain the new iterate. In our case, this action may not be permissible, since the Newton step may take us to a new point that does not necessarily satisfy the nonnegativity constraints $x \ge 0$ and $s \geq 0$ . In our modification of Newton’s method, we want to avoid such violations and therefore will seek a step-size parameter $\alpha _ { k } \in ( 0 , 1 ]$ such that $x ^ { k } + \alpha _ { k } \Delta x ^ { k } > 0$ and $s ^ { k } + \alpha _ { k } \Delta s ^ { k } > 0$ . Note that the largest possible value of $\alpha _ { k }$ satisfying these restrictions can be found using a procedure similar to the ratio test in the simplex method. Once we determine the step-size parameter, we choose the next iterate as 

$$
(x ^ {k + 1}, y ^ {k + 1}, s ^ {k + 1}) = (x ^ {k}, y ^ {k}, s ^ {k}) + \alpha_ {k} (\Delta x ^ {k}, \Delta y ^ {k}, \Delta s ^ {k}).
$$

If a value of $\alpha _ { k }$ results in a next iterate $( x ^ { k + 1 } , y ^ { k + 1 } , s ^ { k + 1 } )$ that is also in ${ \mathcal { F } } ^ { o }$ we say that this value of $\alpha _ { k }$ is permissible. 

Exercise 7.5 What is the largest permissable stepsize $\alpha _ { k }$ for the Newton direction you found in Exercise 7.4? 

A naive modification of Newton’s method as we described above is, unfortunately, not very good in practice since the permissible values of $\alpha _ { k }$ eventually become too small and the progress toward the optimal solution stalls. Therefore, one needs to modify the search direction as well as adjusting the step size along the direction. The usual Newton search direction obtained from (7.14) is called the pure Newton direction. We will consider modifications of pure Newton directions called centered Newton directions. To describe such directions, we first need to discuss the concept of the central path. 

## 7.4 The Central Path

The central path is a trajectory in the relative interior of the feasible region ${ \mathcal { F } } ^ { o }$ that is very useful for both the theoretical study and also the implementation of IPMs. This trajectory is parameterized by a scalar $\tau > 0$ 2 and the points $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ on the central path are obtained as solutions of the following system: 

$$
F (x _ {\tau}, y _ {\tau}, s _ {\tau}) = \left[ \begin{array}{c} 0 \\ 0 \\ \tau e \end{array} \right], (x _ {\tau}, s _ {\tau}) > 0.\tag{7.15}
$$

Then, the central path is defined as 

$$
\mathcal {C} = \{(x _ {\tau}, y _ {\tau}, s _ {\tau}): \tau > 0 \}.\tag{7.16}
$$

The third block of equations in (7.15) can be rewritten as 

$$
(x _ {\tau}) _ {i} (s _ {\tau}) _ {i} = \tau , \forall i.
$$

The similarities between (7.8) and (7.15) are evident. Note that instead of requiring that x and s are complementary vectors as in the optimality conditions (7.8), we require their component products to be all equal. Note that as $\tau  0$ , the conditions (7.15) defining the points on the central path approximate the set of optimality conditions (7.8) more and more closely. 

The system (7.15) has a unique solution for every $\tau > 0$ , provided that ${ \mathcal { F } } ^ { o }$ is nonempty. Furthermore, when ${ \mathcal { F } } ^ { o }$ is nonempty, the trajectory $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ converges to an optimal solution of the problem (7.1). Figure 7.2 depicts a sample feasible set and its central path. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/449af40e57e2a315201e19106bc5776063d110ac17528a3afc608092d0ef18ba.jpg)



Figure 7.2: The Central Path


Exercise 7.6 Recall the quadratic programming problem given in Exercise 7.3 and the current primal-dual estimate of the solution $\begin{array} { r } { x ^ { k } = \left( \frac { 1 } { 3 } , \frac { 1 } { 3 } , \frac { 1 } { 3 } \right) ^ { T } } \end{array}$ , $y ^ { k } = \left( 1 , \frac { 1 } { 2 } \right) ^ { T }$ , and $\begin{array} { r } { s ^ { k } = \left( \frac { 1 } { 2 } , \frac { 1 } { 2 } , 2 \right) ^ { T } } \end{array}$ . Verify that $( x ^ { k } , y ^ { k } , s ^ { k } )$ is not on the central path. Find a vector xˆ such that $( \hat { x } , y ^ { k } , s ^ { k } )$ is on the central path. What value of $\tau$ does this primal dual solution correspond to? 

## 7.5 Interior-Point Methods

## 7.5.1 Path-Following Algorithms

The observation that points on the central path converge to optimal solutions of the primal-dual pair of quadratic programming problems suggests the following strategy for finding such solutions: In an iterative manner, generate points that approximate central points for decreasing values of the parameter τ. Since the central path converges to an optimal solution of the QP problem, these approximations to central points should also converge to a desired solution. This simple idea is the basis of path-following interior-point algorithms for optimization problems. 

The strategy we outlined in the previous paragraph may appear confusing in a first reading. For example, one might ask why we do not approximate or find the solutions of the optimality system (7.8) directly rather than generating all these intermediate iterates leading to such a solution. Or, one might wonder, why we would want to find approximations to central points, rather than central points themselves. Let us respond to these potential questions. First of all, there is no good and computationally cheap way of solving (7.8) directly since it involves nonlinear equations of the form $x _ { i } s _ { i } = 0$ . As we discussed above, if we apply Newton’s method to the equations in (7.8), we run into trouble because of the additional nonnegativity constraints. While we also have bilinear equations in the system defining the central points, being somewhat safely away from the boundaries defined by nonnegativity constraints, central points can be computed without most of the dificulties encountered in solving (7.8) directly. This is why we use central points for guidance. 

Instead of insisting that we obtain a point exactly on the central path, we are often satisfied with an approximation to a central point for reasons of computational eficiency. Central points are also defined by systems of nonlinear equations and additional nonnegativity conditions. Solving these systems exactly (or very accurately) can be as hard as solving the optimality system (7.8) and therefore would not be an acceptable alternative for a practical implementation. It is, however, relatively easy to find a well-defined approximation to central points–see the definition of the neighborhoods of the central path below–especially those that correspond to larger values of τ. Once we identify a point close to a central point on , we can do a clever and inexpensive search to find another point which is close to another central point on ${ \mathcal { C } } ,$ corresponding to a smaller value of τ. Furthermore, this idea can be used repeatedly, resulting in approximations to central points with progressively smaller τ values, allowing us to approach an optimal solution of the QP we are trying to solve. This is the essence of the path-following strategies. 

## 7.5.2 Centered Newton directions

We say that a Newton step used in an interior-point method is a pure Newton step if it is a step directed toward the optimal point satisfying $F ( x , y , s )$ = $[ 0 , \ 0 , \ 0 ] ^ { T }$ . Especially at points close to the boundary of the feasible set, pure Newton directions can be poor search directions as they may point to the exterior of the feasible set and lead to small admissible stepsizes. To avoid such behavior, most interior-point methods take a step toward points on the central path $\mathcal { C }$ corresponding to predetermined value of $\tau .$ . Since such directions are aiming for central points, they are called centered directions. Figure 7.3 depicts a pure and centered Newton direction from a sample iterate. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/20276c9371355498deb002d82e8636e585f9cf9360d996d8a7444740fb582626.jpg)



Figure 7.3: Pure and centered Newton directions


A centered direction is obtained by applying Newton update to the following system: 

$$
\hat {F} (x, y, s) = \left[ \begin{array}{c} A ^ {T} y - Q x + s - c \\ A x - b \\ X S e - \tau e \end{array} \right] = \left[ \begin{array}{c} 0 \\ 0 \\ 0 \end{array} \right].\tag{7.17}
$$

Since the Jacobian of $\hat { F }$ is identical to the Jacobian of $F$ , proceeding as in equations (7.11)–(7.14), we obtain the following (modified) Newton equation for the centered direction: 

$$
\left[ \begin{array}{c c c} {- Q} & {A ^ {T}} & {I} \\ {A} & {0} & {0} \\ {S ^ {k}} & {0} & {X ^ {k}} \end{array} \right] \left[ \begin{array}{c} {\Delta x _ {c} ^ {k}} \\ {\Delta y _ {c} ^ {k}} \\ {\Delta s _ {c} ^ {k}} \end{array} \right] = \left[ \begin{array}{c} {0} \\ {0} \\ {\tau e - X ^ {k} S ^ {k} e} \end{array} \right].\tag{7.18}
$$

We used the subscript c with the direction vectors to note that they are centered directions. Notice the similarity between (7.14) and (7.18). 

One crucial choice we need to make is the value of $\tau$ to be used in determining the centered direction. To illustrate potential strategies for this choice, we first define the following measure often called the duality gap, or the average complementarity: 

$$
\mu = \mu (x, s) := \frac {\sum_ {i = 1} ^ {n} x _ {i} s _ {i}}{n} = \frac {x ^ {T} s}{n}.\tag{7.19}
$$

Note that, when $( x , y , s )$ satisfy the conditions $A x = b , x \geq 0$ and $A ^ { T } y -$ $Q x + s = c , s \geq 0$ , then $( x , y , s )$ are optimal if and only if $\mu ( x , s ) = 0$ . If $\mu$ is large, then we are far away from the solution. Therefore, µ serves as a measure of optimality for feasible points–the smaller the duality gap, the closer the point to optimality. 

For a central point $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ we have 

$$
\mu (x _ {\tau}, s _ {\tau}) = \frac {\sum_ {i = 1} ^ {n} (x _ {\tau}) _ {i} (s _ {\tau}) _ {i}}{n} = \frac {\sum_ {i = 1} ^ {n} \tau}{n} = \tau .
$$

Because of this identity, we associate the central point $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ with all feasible points $( x , y , s )$ satisfying $\mu ( x , s ) = \tau$ . All such points can be regarded as being at the same “level” as the central point $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ When we choose a centered direction from a current iterate $( x , y , s )$ , we have the possibility of choosing to target a central point that is (i) at a lower level than our current point $( \tau < \mu ( x , s ) )$ , (ii) at the same level as our current point $( \tau = \mu ( x , s ) )$ , or (iii) at a higher level than our current point $( \tau > \mu ( x , s ) )$ In most circumstances, the third option is not a good choice as it targets a central point that is “farther” than the current iterate to the optimal solution. Therefore, we will always choose $\tau \leq \mu ( x , s )$ in defining centered directions. Using a simple change in notation, the centered direction can now be described as the solution of the following system: 

$$
\left[ \begin{array}{c c c} {- Q} & {A ^ {T}} & {I} \\ {A} & {0} & {0} \\ {S ^ {k}} & {0} & {X ^ {k}} \end{array} \right] \left[ \begin{array}{c} {\Delta x _ {c} ^ {k}} \\ {\Delta y _ {c} ^ {k}} \\ {\Delta s _ {c} ^ {k}} \end{array} \right] = \left[ \begin{array}{c} {0} \\ {0} \\ {\sigma^ {k} \mu^ {k} e - X ^ {k} S ^ {k} e} \end{array} \right],\tag{7.20}
$$

where $\begin{array} { r } { \mu ^ { k } : = \mu ( x ^ { k } , s ^ { k } ) = \frac { ( x ^ { k } ) ^ { T } s ^ { k } } { n } } \end{array}$ and $\sigma ^ { k } \in [ 0 , 1 ]$ is a user defined quantity describing the ratio of the duality gap at the target central point and the current point. 

When $\sigma ^ { k } = 1$ (equivalently, $\textstyle { \boldsymbol { \tau } } = { \boldsymbol { \mu } } ^ { k }$ in our earlier notation), we have a pure centering direction. This direction does not improve the duality gap and targets the central point whose duality gap is the same as our current iterate. Despite the lack of progress in terms of the duality gap, these steps are often desirable since large step sizes are permissible along such directions and points get well-centered so that the next iteration can make significant progress toward optimality. At the other extreme, we have $\sigma ^ { k } = 0$ This, as we discussed before, corresponds to the pure Newton step, also called the afine-scaling direction. Practical implementations often choose intermediate values for $\sigma ^ { k }$ 

We are now ready to describe a generic interior-point algorithm that uses centered directions: 

## Algorithm 7.1 Generic Interior Point Algorithm

0. Choose $( x ^ { 0 } , y ^ { 0 } , s ^ { 0 } ) \in \mathcal { F } ^ { o }$ . For $k = 0 , 1 , 2 , . . .$ . repeat the following steps. 

1. Choose $\sigma ^ { k } \in [ 0 , 1 ]$ , let $\begin{array} { r } { \mu ^ { k } = \frac { ( x ^ { k } ) ^ { T } s ^ { k } } { n } } \end{array}$ . Solve 

$$
\left[ \begin{array}{c c c} {- Q} & {A ^ {T}} & {I} \\ {A} & {0} & {0} \\ {S ^ {k}} & {0} & {X ^ {k}} \end{array} \right] \left[ \begin{array}{c} {\Delta x ^ {k}} \\ {\Delta y ^ {k}} \\ {\Delta s ^ {k}} \end{array} \right] = \left[ \begin{array}{c} {0} \\ {0} \\ {\sigma^ {k} \mu^ {k} e - X ^ {k} S ^ {k} e} \end{array} \right].
$$

2. Choose $\alpha ^ { k }$ such that 

$$
x ^ {k} + \alpha^ {k} \Delta x ^ {k} > 0, a n d s ^ {k} + \alpha^ {k} \Delta s ^ {k} > 0.
$$

Set 

$$
(x ^ {k + 1}, y ^ {k + 1}, s ^ {k + 1}) = (x ^ {k}, y ^ {k}, s ^ {k}) + \alpha_ {k} (\Delta x ^ {k}, \Delta y ^ {k}, \Delta s ^ {k}),
$$

and $k = k + 1$ 

Exercise 7.7 Compute the centered Newton direction for the iterate in Exercise 7.4 for $\sigma ^ { k } = 1$ , 0.5, and 0.1. For each $\sigma ^ { k }$ , compute the largest permissable stepsize along the computed centered direction and compare your findings with that of Exercise 7.5. 

## 7.5.3 Neighborhoods of the Central Path

Variants of interior-point methods difer in the way they choose the centering parameter $\sigma ^ { k }$ and the step-size parameter $\alpha ^ { k }$ in each iteration. Pathfollowing methods aim to generate iterates that are approximations to central points. This is achieved by a careful selection of the centering and step-size parameters. Before we discuss the selection of these parameters we need to make the notion of “approximate central points” more precise. 

Recall that central points are those in the set ${ \mathcal { F } } ^ { o }$ that satisfy the additional conditions that $x _ { i } s _ { i } = \tau , \forall i$ , for some positive $\tau .$ . Consider a central point $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ . If a point $( x , y , s )$ approximates this central point, we would expect that the Euclidean distance between these two points is small, i.e., 

$$
\left\| (x, y, s) - \left(x _ {\tau}, y _ {\tau}, s _ {\tau}\right) \right\|
$$

is small. Then, the set of approximations to $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ may be defined as: 

$$
\{(x, y, s) \in \mathcal {F} ^ {o}: \| (x, y, s) - (x _ {\tau}, y _ {\tau}, s _ {\tau}) \| \leq \varepsilon \},\tag{7.21}
$$

for some $\varepsilon \geq 0$ . Note, however, that it is dificult to obtain central points explicitly. Instead, we have their implicit description through the system (7.17). Therefore, a description such as (7.21) is of little practical/algorithmic value when we do not know $( x _ { \tau } , y _ { \tau } , s _ { \tau } )$ . Instead, we consider descriptions of sets that imply proximity to central points. Such descriptions are often called the neighborhoods of the central path. Two of the most commonly used neighborhoods of the central path are: 

$$
\mathcal {N} _ {2} (\theta) := \{(x, y, s) \in \mathcal {F} ^ {o}: \| X S e - \mu e \| \leq \theta \mu , \mu = \frac {x ^ {T} s}{n} \},\tag{7.22}
$$

for some $\theta \in ( 0 , 1 )$ and 

$$
\mathcal {N} _ {- \infty} (\gamma) := \{(x, y, s) \in \mathcal {F} ^ {o}: x _ {i} s _ {i} \geq \gamma \mu \forall i, \mu = \frac {x ^ {T} s}{n} \},\tag{7.23}
$$

for some $\gamma \in ( 0 , 1 )$ . The first neighborhood is called the 2-norm neighborhood while the second one the one-sided -norm neighborhood (but often called the -norm neighborhood, hence the notation). One can guarantee that the generated iterates are “close” to the central path by making sure that they all lie in one of these neighborhoods. If we choose $\theta = 0$ in (7.22) or $\gamma = 1$ in (7.23), the neighborhoods we defined degenerate to the central path . 

Exercise 7.8 Show that $\mathcal { N } _ { 2 } ( \theta _ { 1 } ) \subset \mathcal { N } _ { 2 } ( \theta _ { 2 } )$ when $0 < \theta _ { 1 } \leq \theta _ { 2 } < 1$ , and that $\mathcal { N } _ { - \infty } ( \gamma _ { 1 } ) \subset \mathcal { N } _ { - \infty } ( \gamma _ { 2 } )$ for $0 < \gamma _ { 2 } \leq \gamma _ { 1 } < 1$ 

Exercise 7.9 Show that $\mathcal { N } _ { 2 } ( \theta ) \subset \mathcal { N } _ { - \infty } ( \gamma ) \mathrm { ~ i f ~ } \gamma \leq 1 - \theta .$ 

As hinted in the last exercise, for typical values of θ and $\gamma ,$ the 2-norm neighborhood is often much smaller than the -norm neighborhood. Indeed, 

$$
\| X S e - \mu e \| \leq \theta \mu \Leftrightarrow \left\| \begin{array}{c} \frac {x _ {1} s _ {1}}{\mu} - 1 \\ \frac {x _ {2} s _ {2}}{\mu} - 1 \\ \vdots \\ \frac {x _ {n} s _ {n}}{\mu} - 1 \end{array} \right\| \leq \theta ,\tag{7.24}
$$

which, in turn, is equivalent to 

$$
\sum_ {i = 1} ^ {n} \left(\frac {x _ {i} s _ {i}}{\mu} - 1\right) ^ {2} \leq \theta^ {2}.
$$

In this last expression, the quantity $\begin{array} { r } { \frac { x _ { i } s _ { i } } { \mu } - 1 = \frac { x _ { i } s _ { i } - \mu } { \mu } } \end{array}$ is the relative deviation of $x _ { i } s _ { i } { ^ \mathrm { { ' } s } }$ from their average value $\mu .$ . Therefore, a point is in the 2-norm neighborhood only if the sum of the squared relative deviations is small. Thus, $\mathcal { N } _ { 2 } ( \theta )$ contains only a small fraction of the feasible points, even when $\theta$ is close to 1. On the other hand, for the -norm neighborhood, the only requirement is that each $x _ { i } s _ { i }$ should not be much smaller than their average value $\mu$ . For small (but positive) $\gamma , \mathcal { N } _ { - \infty } ( \gamma )$ may contain almost the entire set ${ \mathcal { F } } ^ { o }$ 

In summary, 2-norm neighborhoods are narrow while the -norm neighborhoods are relatively wide. The practical consequence of this observation is that, when we restrict our iterates to be in the 2-norm neighborhood of the central path as opposed to the -norm neighborhood, we have much less room to maneuver and our step-sizes may be cut short. Figure 7.4 illustrates this behavior. For these reasons, algorithms using the narrow 2- norm neighborhoods are often called short-step path-following methods while the methods using the wide -norm neighborhoods are called long-step path-following methods 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/53c4ed48fefea32eebc83a91922f38e4c6e9e373738b8b353d35b00a7ce0669a.jpg)



Figure 7.4: Narrow and wide neighborhoods of the central path


The price we pay for the additional flexibility with wide neighborhoods come in the theoretical worst-case analysis of algorithms using such neighborhoods. When the iterates are restricted to the 2-norm neighborhood, we have a stronger control of the iterates as they are very close to the central path– a trajectory with many desirable theoretical features. Consequently, we can guarantee that even in the worst case the iterates that lie in the 2-norm neighborhood will converge to an optimal solution relatively fast. In contrast, iterates that are only restricted to a -norm neighborhood can get relatively far away from the central path and may not possess its nice theoretical properties. $\mathrm { A s }$ a result, iterates may “get stuck” in undesirable corners of the feasible set and the convergence may be slow in these worst-case scenarios. Of course, the worst case scenarios rarely happen and typically (on average) we see faster convergence with long-step methods than with short-step methods. 

Exercise 7.10 Verify that the iterate given in Exercise 7.4 is in $N _ { - \infty } ( \textstyle { \frac { 1 } { 2 } } )$ What is the largest $\gamma$ such that this iterate lies in $N _ { - \infty } ( \gamma ) ?$ 

Exercise 7.11 Recall the centered Newton directions in Exercise 7.7 as well as the pure Newton direction in Exercise 7.5. For each direction, compute the largest $\alpha _ { k }$ such that the updated iterate remains in $N _ { - \infty } ( \scriptstyle { \frac { 1 } { 2 } } )$ 

## 7.5.4 A Long-Step Path-Following Algorithm

Next, we formally describe a long-step path following algorithm that specifies some of the parameter choices of the generic algorithm we described above. 

## Algorithm 7.2 Long-Step Path-Following Algorithm

0. Given $\gamma \in ( 0 , 1 ) , 0 < \sigma _ { \operatorname* { m i n } } < \sigma _ { \operatorname* { m a x } } < 1$ , choose $( x ^ { 0 } , y ^ { 0 } , s ^ { 0 } ) \in \mathcal { N } _ { - \infty } ( \gamma )$ For $k = 0 , 1 , 2 , \ldots$ repeat the following steps. 

1. Choose $\sigma ^ { k } \in [ \sigma _ { \operatorname* { m i n } } , \sigma _ { \operatorname* { m a x } } ]$ , let $\begin{array} { r } { \mu ^ { k } = \frac { ( x ^ { k } ) ^ { T } s ^ { k } } { n } } \end{array}$ . Solve 

$$
\left[ \begin{array}{c c c} {- Q} & {A ^ {T}} & {I} \\ {A} & {0} & {0} \\ {S ^ {k}} & {0} & {X ^ {k}} \end{array} \right] \left[ \begin{array}{c} {\Delta x ^ {k}} \\ {\Delta y ^ {k}} \\ {\Delta s ^ {k}} \end{array} \right] = \left[ \begin{array}{c} {0} \\ {0} \\ {\sigma^ {k} \mu^ {k} e - X ^ {k} S ^ {k} e} \end{array} \right].
$$

2. Choose $\alpha ^ { k }$ such that 

$$
(x ^ {k}, y ^ {k}, s ^ {k}) + \alpha_ {k} (\Delta x ^ {k}, \Delta y ^ {k}, \Delta s ^ {k}) \in \mathcal {N} _ {- \infty} (\gamma).
$$

Set 

$$
(x ^ {k + 1}, y ^ {k + 1}, s ^ {k + 1}) = (x ^ {k}, y ^ {k}, s ^ {k}) + \alpha_ {k} (\Delta x ^ {k}, \Delta y ^ {k}, \Delta s ^ {k}),
$$

and $k = k + 1$ 

## 7.5.5 Starting from an Infeasible Point

Both the generic interior-point method and the long-step path-following algorithm we described above require that one starts with a strictly feasible iterate. This requirement is not practical since finding such a starting point is not always a trivial task. Fortunately, however, we can accommodate infeasible starting points in these algorithms with a small modification of the linear system we solve in each iteration. 

For this purpose, we only require that the initial point $( x ^ { 0 } , y ^ { 0 } , s ^ { 0 } )$ satisfy the nonnegativity restrictions strictly: $x ^ { 0 } > 0$ and $s ^ { 0 } > 0$ . Such points can be generated trivially. We are still interested in solving the following nonlinear system: 

$$
\hat {F} (x, y, s) = \left[ \begin{array}{c} A ^ {T} y - Q x + s - c \\ A x - b \\ X S e - \tau e \end{array} \right] = \left[ \begin{array}{c} 0 \\ 0 \\ 0 \end{array} \right],\tag{7.25}
$$

as well as $x \ge 0 , s \ge 0$ . As in (5.7), the Newton step from an infeasible point $( x ^ { k } , y ^ { k } , s ^ { k } )$ is determined by solving the following system of linear equations: 

$$
\begin{array}{r l r} {J (x ^ {k}, y ^ {k}, s ^ {k}) \left[ \begin{array}{l} {\Delta x ^ {k}} \\ {\Delta y ^ {k}} \\ {\Delta s ^ {k}} \end{array} \right]} & = & {- \hat {F} (x ^ {k}, y ^ {k}, s ^ {k}),} \end{array}\tag{7.26}
$$

which reduces to 

$$
\left[ \begin{array}{c c c} - Q & A ^ {T} & I \\ A & 0 & 0 \\ S ^ {k} & 0 & X ^ {k} \end{array} \right] \left[ \begin{array}{c} \Delta x ^ {k} \\ \Delta y ^ {k} \\ \Delta s ^ {k} \end{array} \right] = \left[ \begin{array}{c} c + Q x ^ {k} - A ^ {T} y ^ {k} - s ^ {k} \\ b - A x ^ {k} \\ \tau e - X ^ {k} S ^ {k} e \end{array} \right].\tag{7.27}
$$

We no longer have zeros in the first and second blocks of the right-handside vector since we are not assuming that the iterates satisfy $A x ^ { k } = b$ and $A ^ { T } y ^ { k } - Q x ^ { k } + s ^ { k } = c .$ Replacing the linear system in the two algorithm descriptions above with (7.27) we obtain versions of these algorithms that work with infeasible iterates. In these versions of the algorithms, search for feasibility and optimality are performed simultaneously. 

## 7.6 QP software

As for linear programs, there are several software options for solving practical quadratic programming problems. Many of the commercial software options are very eficient and solve very large QPs within seconds or minutes. A survey of nonlinear programming software, which includes software designed for QPs, can be found at 

## http://www.lionhrtpub.com/orms/surveys/nlp/nlp.html

The Network Enabled Optimization Server (NEOS) website and the $O p \mathrm { . }$ timization Software Guide website we mentioned when we discussed NLP software are also useful for QP solvers. LOQO is a very eficient and robust interior-point based software for QPs and other nonlinear programming problems. It is available from 

## http://www.orfe.princeton.edu/ loqo

OOQP is an object-oriented C++ package, based on a primal-dual interiorpoint method, for solving convex quadratic programming problems. It contains code that can be used ”out of the box” to solve a variety of structured QPs, including general sparse QPs, QPs arising from support vector machines, Huber regression problems, and QPs with bound constraints. It is available for free from the following website: 

## http://www.cs.wisc.edu/ swright/ooqp

## 7.7 Additional Exercises

Exercise 7.12 In the study of interior-point methods for solving quadratic programming problems we encountered the following matrix: 

$$
M := \left[ \begin{array}{c c c} - Q & A ^ {T} & I \\ A & 0 & 0 \\ S ^ {k} & 0 & X ^ {k} \end{array} \right],
$$

where $( x ^ { k } , y ^ { k } , s ^ { k } )$ is the current iterate, $X ^ { k }$ and $S ^ { k }$ are diagonal matrices with the components of the vectors $x ^ { k }$ and $s ^ { k }$ along their diagonals. Recall that M is the Jacobian matrix of the function that defines the optimality conditions of the QP problem. This matrix appears in linear systems we need to solve in each interior-point iteration. We can solve these systems only when M is nonsingular. Show that M is necessarily nonsingular when $A$ has full row rank and $Q$ is positive semidefinite. Provide an example with $\mathrm { ~ a ~ } Q$ matrix that is not positive semidefinite (but A matrix has full row rank) such that M is singular. (Hint: To prove non-singularity of M when $Q$ is positive semidefinite and A has full row rank, consider a solution of the system 

$$
\left[ \begin{array}{c c c} - Q & A ^ {T} & I \\ A & 0 & 0 \\ S ^ {k} & 0 & X ^ {k} \end{array} \right] \left[ \begin{array}{c} \Delta x \\ \Delta y \\ \Delta s \end{array} \right] = \left[ \begin{array}{c} 0 \\ 0 \\ 0 \end{array} \right].
$$

It is suficient to show that the only solution to this system is $\Delta x = 0 , \Delta y =$ $0 , \Delta s = 0$ . To prove this, first eliminate $\Delta s$ variables from the system, and then eliminate $\Delta x$ variables.) 

Exercise 7.13 Consider the following quadratic programming formulation obtained from a small portfolio selection model: 

$$
\begin{array}{c} \min _ {x} \left[ x _ {1} x _ {2} x _ {3} x _ {4} \right] \left[ \begin{array}{c c c c} 0. 0 1 & 0. 0 0 5 & 0 & 0 \\ 0. 0 0 5 & 0. 0 1 & 0 & 0 \\ 0 & 0 & 0. 0 4 & 0 \\ 0 & 0 & 0 & 0 \end{array} \right] \left[ \begin{array}{c} x _ {1} \\ x _ {2} \\ x _ {3} \\ x _ {4} \end{array} \right] \\ x _ {1} + x _ {2} + x _ {3} = 1 \\ - x _ {2} + x _ {3} + x _ {4} = 0. 1 \\ x _ {1}, x _ {2}, x _ {3}, x _ {4} \geq 0. \end{array}
$$

We have the following iterate for this problem: 

$$
x = \left[ \begin{array}{l} x _ {1} \\ x _ {2} \\ x _ {3} \\ x _ {4} \end{array} \right] = \left[ \begin{array}{l} 1 / 3 \\ 1 / 3 \\ 1 / 3 \\ 0. 1 \end{array} \right], y = \left[ \begin{array}{l} y _ {1} \\ y _ {2} \end{array} \right] = \left[ \begin{array}{c} 0. 0 0 1 \\ - 0. 0 0 1 \end{array} \right], s = \left[ \begin{array}{l} s _ {1} \\ s _ {2} \\ s _ {3} \\ s _ {4} \end{array} \right] = \left[ \begin{array}{l} 0. 0 0 4 \\ 0. 0 0 3 \\ 0. 0 1 3 3 \\ 0. 0 0 1 \end{array} \right].
$$

Verify that $( x , y , s ) \in \mathcal { F } ^ { o }$ . Is this point on the central path? Is it on $\mathcal { N } _ { - \infty } ( 0 . 1 ) ?$ How about $\mathcal { N } _ { - \infty } ( 0 . 0 5 ) ?$ Compute the pure centering $( \sigma = 1 )$ and pure Newton $( \sigma = 0 )$ directions from this point. For each direction, find the largest step-size α that can be taken along that direction without leaving the neighborhood $\mathcal { N } _ { - \infty } ( 0 . 0 5 ) ?$ Comment on your results. 

Exercise 7.14 Implement the long-step path-following algorithm given in Section 7.5.4 using $\sigma _ { \mathrm { m i n } } = 0 . 2 , \sigma _ { \mathrm { m a x } } = 0 . 8 , \gamma = 0 . 2 5$ . Solve the quadratic programming problem in Exercise 7.13 starting from the iterate given in that exercise using your implementation. Experiment with alternative choices for σ<sub>min</sub>, $\sigma _ { \mathrm { m a x } }$ and γ. 

# Chapter 8

# QP Models: Portfolio Optimization

## 8.1 Mean-Variance Optimization

Markowitz’ theory of mean-variance optimization (MVO) provides a mechanism for the selection of portfolios of securities (or asset classes) in a manner that trades of the expected returns and the risk of potential portfolios. We explore this model in more detail in this chapter. 

Consider assets $S 1 , S _ { 2 } , \ldots , S _ { n } \ ( n \geq 2 )$ with random returns. Let $\mu _ { i }$ and $\sigma _ { i }$ denote the expected return and the standard deviation of the return of asset $S _ { i }$ . For $i \neq j , \rho _ { i j }$ denotes the correlation coeficient of the returns of assets $S _ { i }$ and $S _ { j }$ . Let $\boldsymbol { \mu } = [ \mu _ { 1 } , \ldots , \mu _ { n } ] ^ { T } .$ and $\Sigma = \left( \sigma _ { i j } \right)$ be the $n \times n$ symmetric covariance matrix with $\sigma _ { i i } = \sigma _ { i } ^ { 2 }$ and $\sigma _ { i j } = \rho _ { i j } \sigma _ { i } \sigma _ { j }$ for $i \neq j$ Denoting by $x _ { i }$ the proportion of the total funds invested in security $i ,$ one can represent the expected return and the variance of the resulting portfolio $x = ( x _ { 1 } , \ldots , x _ { n } )$ as follows: 

$$
\operatorname{E} [ x ] = x _ {1} \mu_ {1} + \ldots + x _ {n} \mu_ {n} = \mu^ {T} x,
$$

and 

$$
\mathrm{Var} [ x ] = \sum_ {i, j} \rho_ {i j} \sigma_ {i} \sigma_ {j} x _ {i} x _ {j} = x ^ {T} \Sigma x,
$$

where $\rho _ { i i } \equiv 1$ 

Since variance is always nonnegative, it follows that $x ^ { T } \Sigma x \geq 0$ for any $x , \ { \mathrm { i . e . } }$ , Σ is positive semidefinite. In this section, we will assume that it is in fact positive definite, which is essentially equivalent to assuming that there are no redundant assets in our collection $S _ { 1 } , S _ { 2 } , \ldots , S _ { n }$ . We further assume that the set of admissible portfolios is a nonempty polyhedral set and represent it as $\mathcal { X } : = \{ x : A x = b , C x \geq d \}$ , where $A$ is an $m \times n$ matrix, $b$ is an m-dimensional vector, $C$ is a $p \times n$ matrix and d is a p-dimensional vector. In particular, one of the constraints in the set $\mathcal { X }$ is 

$$
\sum_ {i = 1} ^ {n} x _ {i} = 1.
$$

Linear portfolio constraints such as short-sale restrictions or limits on asset/sector allocations are subsumed in our generic notation  for the polyhedral feasible set. 

Recall that a feasible portfolio x is called eficient if it has the maximal expected return among all portfolios with the same variance, or alternatively, if it has the minimum variance among all portfolios that have at least a certain expected return. The collection of eficient portfolios form the eficient frontier of the portfolio universe. The eficient frontier is often represented as a curve in a two-dimensional graph where the coordinates of a plotted point corresponds to the standard deviation and the expected return of an eficient portfolio. 

When we assume that Σ is positive definite, the variance is a strictly convex function of the portfolio variables and there exists a unique portfolio in that has the minimum variance; see Exercise 7.2. Let us denote this portfolio with $x _ { \mathrm { m i n } }$ and its return $\mu ^ { T } x _ { \mathrm { m i n } }$ with $R _ { \mathrm { m i n } }$ . Note that $x _ { \mathrm { m i n } }$ is an eficient portfolio. We let $R _ { \mathrm { m a x } }$ denote the maximum return for an admissible portfolio. 

Markowitz’ mean-variance optimization (MVO) problem can be formulated in three diferent but equivalent ways. We have seen one of these formulations in the first chapter: Find the minimum variance portfolio of the securities 1 to n that yields at least a target value of expected return (say b). Mathematically, this formulation produces a quadratic programming problem: 

$$
\begin{array}{r c l} \min _ {x} & \frac {1}{2} x ^ {T} \Sigma x \\ & \mu^ {T} x & \geq R \\ & A x & = b \\ & C x & \geq d. \end{array}\tag{8.1}
$$

The first constraint indicates that the expected return is no less than the target value R. Solving this problem for values of R ranging between $R _ { \mathrm { m i n } }$ and $R _ { \mathrm { m a x } }$ one obtains all eficient portfolios. As we discussed above, the objective function corresponds to one half the total variance of the portfolio. The constant $\textstyle { \frac { 1 } { 2 } }$ is added for convenience in the optimality conditions–it obviously does not afect the optimal solution. 

This is a convex quadratic programming problem for which the first order conditions are both necessary and suficient for optimality. We present these conditions next. $x _ { R }$ is an optimal solution of problem (8.1) if and only if there exists $\lambda _ { R } \in \mathrm { ~ } I R , \gamma _ { E } \in \mathrm { ~ } I R ^ { m }$ , and $\gamma _ { I } ~ \in ~ \mathcal { R } ^ { p }$ satisfying the following conditions: T 

$$
\begin{array}{r l} & {\Sigma x _ {R} - \lambda_ {R} \mu - A ^ {T} \gamma_ {E} - C ^ {T} \gamma_ {I} = 0,} \\ & {\mu^ {T} x _ {R} \geq R, A x _ {R} = b, C x _ {R} \geq d,} \\ & {\lambda_ {R} \geq 0, \lambda_ {R} (\mu^ {T} x _ {R} - R) = 0,} \\ & {\gamma_ {I} \geq 0, \gamma_ {I} ^ {T} (C x _ {R} - d) = 0.} \end{array}\tag{8.2}
$$

The two other variations of the MVO problem are the following: 

$$
\begin{array}{r l r} \max _ {x} & \mu^ {T} x \\ & x ^ {T} \Sigma x & \leq \sigma^ {2} \\ & A x & = b \\ & C x & \geq d. \end{array}\tag{8.3}
$$

$$
\begin{array}{r c l} \max _ {x} & \mu^ {T} x - \frac {\delta}{2} x ^ {T} \Sigma x \\ & A x & = b \\ & C x & \geq d. \end{array}\tag{8.4}
$$

In (8.3), $\sigma ^ { 2 }$ is a given upper limit on the variance of the portfolio. In (8.4), the objective function is a risk-adjusted return function where the constant δ serves as a risk-aversion constant. While (8.4) is another quadratic programming problem, (8.3) has a convex quadratic constraint and therefore is not a QP. This problem can be solved using the general nonlinear programming solution techniques discussed in Chapter 5. We will also discuss a reformulation of (8.3) as a second-order cone program in Chapter 10. This opens the possibility of using specialized and eficient second-order cone programming methods for its solution. 

Exercise 8.1 What are the Karush-Kuhn-Tucker optimality conditions for problems (8.3) and $( 8 . 4 ) ?$ 

Exercise 8.2 Consider the following variant of $( 8 . 4 ) { : }$ 

$$
\begin{array}{r l} \max _ {x} & \mu^ {T} x - \eta \sqrt {x ^ {T} \Sigma x} \\ A x & = b \\ C x & \geq d. \end{array}\tag{8.5}
$$

For each $\eta ,$ let $x ^ { * } ( \eta )$ denote the optimal solution of (8.5). Show that there exists a $\delta > 0$ such that $x ^ { * } ( \eta )$ solves (8.4) for that δ. 

## 8.1.1 Example

We apply Markowitz’s MVO model to the problem of constructing a longonly portfolio of US stocks, bonds and cash. We will use historical return data for these three asset classes to estimate their future expected returns. We note that most models for MVO combine historical data with other indicators such as earnings estimates, analyst ratings, valuation and growth metrics, etc. Here we restrict our attention to price based estimates for expositional simplicity. We use the S&P 500 index for the returns on stocks, the 10-year Treasury bond index for the returns on bonds, and we assume that the cash is invested in a money market account whose return is the 1-day federal fund rate. The annual times series for the “Total Return” are given below for each asset between 1960 and 2003. 

<table><tr><td>Year</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>1960</td><td>20.2553</td><td>262.935</td><td>100.00</td></tr><tr><td>1961</td><td>25.6860</td><td>268.730</td><td>102.33</td></tr><tr><td>1962</td><td>23.4297</td><td>284.090</td><td>105.33</td></tr><tr><td>1963</td><td>28.7463</td><td>289.162</td><td>108.89</td></tr><tr><td>1964</td><td>33.4484</td><td>299.894</td><td>113.08</td></tr><tr><td>1965</td><td>37.5813</td><td>302.695</td><td>117.97</td></tr><tr><td>1966</td><td>33.7839</td><td>318.197</td><td>124.34</td></tr><tr><td>1967</td><td>41.8725</td><td>309.103</td><td>129.94</td></tr><tr><td>1968</td><td>46.4795</td><td>316.051</td><td>137.77</td></tr><tr><td>1969</td><td>42.5448</td><td>298.249</td><td>150.12</td></tr><tr><td>1970</td><td>44.2212</td><td>354.671</td><td>157.48</td></tr><tr><td>1971</td><td>50.5451</td><td>394.532</td><td>164.00</td></tr><tr><td>1972</td><td>60.1461</td><td>403.942</td><td>172.74</td></tr><tr><td>1973</td><td>51.3114</td><td>417.252</td><td>189.93</td></tr><tr><td>1974</td><td>37.7306</td><td>433.927</td><td>206.13</td></tr><tr><td>1975</td><td>51.7772</td><td>457.885</td><td>216.85</td></tr><tr><td>1976</td><td>64.1659</td><td>529.141</td><td>226.93</td></tr><tr><td>1977</td><td>59.5739</td><td>531.144</td><td>241.82</td></tr><tr><td>1978</td><td>63.4884</td><td>524.435</td><td>266.07</td></tr><tr><td>1979</td><td>75.3032</td><td>531.040</td><td>302.74</td></tr><tr><td>1980</td><td>99.7795</td><td>517.860</td><td>359.96</td></tr><tr><td>1981</td><td>94.8671</td><td>538.769</td><td>404.48</td></tr></table>

<table><tr><td>Year</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>1982</td><td>115.308</td><td>777.332</td><td>440.68</td></tr><tr><td>1983</td><td>141.316</td><td>787.357</td><td>482.42</td></tr><tr><td>1984</td><td>150.181</td><td>907.712</td><td>522.84</td></tr><tr><td>1985</td><td>197.829</td><td>1200.63</td><td>566.08</td></tr><tr><td>1986</td><td>234.755</td><td>1469.45</td><td>605.20</td></tr><tr><td>1987</td><td>247.080</td><td>1424.91</td><td>646.17</td></tr><tr><td>1988</td><td>288.116</td><td>1522.40</td><td>702.77</td></tr><tr><td>1989</td><td>379.409</td><td>1804.63</td><td>762.16</td></tr><tr><td>1990</td><td>367.636</td><td>1944.25</td><td>817.87</td></tr><tr><td>1991</td><td>479.633</td><td>2320.64</td><td>854.10</td></tr><tr><td>1992</td><td>516.178</td><td>2490.97</td><td>879.04</td></tr><tr><td>1993</td><td>568.202</td><td>2816.40</td><td>905.06</td></tr><tr><td>1994</td><td>575.705</td><td>2610.12</td><td>954.39</td></tr><tr><td>1995</td><td>792.042</td><td>3287.27</td><td>1007.84</td></tr><tr><td>1996</td><td>973.897</td><td>3291.58</td><td>1061.15</td></tr><tr><td>1997</td><td>1298.82</td><td>3687.33</td><td>1119.51</td></tr><tr><td>1998</td><td>1670.01</td><td>4220.24</td><td>1171.91</td></tr><tr><td>1999</td><td>2021.40</td><td>3903.32</td><td>1234.02</td></tr><tr><td>2000</td><td>1837.36</td><td>4575.33</td><td>1313.00</td></tr><tr><td>2001</td><td>1618.98</td><td>4827.26</td><td>1336.89</td></tr><tr><td>2002</td><td>1261.18</td><td>5558.40</td><td>1353.47</td></tr><tr><td>2003</td><td>1622.94</td><td>5588.19</td><td>1366.73</td></tr></table>


Let $I _ { i t }$ denote the above “Total $\mathrm { R e t u r n } ^ { \dag }$ for asset $i = { 1 , 2 , 3 }$ and $t =$ $0 , \ldots T$ , where $t = 0$ corresponds to 1960 and $t = T$ to 2003. For each asset $i ,$ we can convert the raw data $I _ { i t } , \ t = 0 , . . . , T$ , into rates of returns $r _ { i t } .$ $t = 1 , \dots , T$ , using the formula 


$$
r _ {i t} = \frac {I _ {i , t} - I _ {i , t - 1}}{I _ {i , t - 1}}.
$$

<table><tr><td>Year</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>1961</td><td>26.81</td><td>2.20</td><td>2.33</td></tr><tr><td>1962</td><td>-8.78</td><td>5.72</td><td>2.93</td></tr><tr><td>1963</td><td>22.69</td><td>1.79</td><td>3.38</td></tr><tr><td>1964</td><td>16.36</td><td>3.71</td><td>3.85</td></tr><tr><td>1965</td><td>12.36</td><td>0.93</td><td>4.32</td></tr><tr><td>1966</td><td>-10.10</td><td>5.12</td><td>5.40</td></tr><tr><td>1967</td><td>23.94</td><td>-2.86</td><td>4.51</td></tr><tr><td>1968</td><td>11.00</td><td>2.25</td><td>6.02</td></tr><tr><td>1969</td><td>-8.47</td><td>-5.63</td><td>8.97</td></tr><tr><td>1970</td><td>3.94</td><td>18.92</td><td>4.90</td></tr><tr><td>1971</td><td>14.30</td><td>11.24</td><td>4.14</td></tr><tr><td>1972</td><td>18.99</td><td>2.39</td><td>5.33</td></tr><tr><td>1973</td><td>-14.69</td><td>3.29</td><td>9.95</td></tr><tr><td>1974</td><td>-26.47</td><td>4.00</td><td>8.53</td></tr><tr><td>1975</td><td>37.23</td><td>5.52</td><td>5.20</td></tr><tr><td>1976</td><td>23.93</td><td>15.56</td><td>4.65</td></tr><tr><td>1977</td><td>-7.16</td><td>0.38</td><td>6.56</td></tr><tr><td>1978</td><td>6.57</td><td>-1.26</td><td>10.03</td></tr><tr><td>1979</td><td>18.61</td><td>-1.26</td><td>13.78</td></tr><tr><td>1980</td><td>32.50</td><td>-2.48</td><td>18.90</td></tr><tr><td>1981</td><td>-4.92</td><td>4.04</td><td>12.37</td></tr><tr><td>1982</td><td>21.55</td><td>44.28</td><td>8.95</td></tr></table>

<table><tr><td>Year</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>1983</td><td>22.56</td><td>1.29</td><td>9.47</td></tr><tr><td>1984</td><td>6.27</td><td>15.29</td><td>8.38</td></tr><tr><td>1985</td><td>31.17</td><td>32.27</td><td>8.27</td></tr><tr><td>1986</td><td>18.67</td><td>22.39</td><td>6.91</td></tr><tr><td>1987</td><td>5.25</td><td>-3.03</td><td>6.77</td></tr><tr><td>1988</td><td>16.61</td><td>6.84</td><td>8.76</td></tr><tr><td>1989</td><td>31.69</td><td>18.54</td><td>8.45</td></tr><tr><td>1990</td><td>-3.10</td><td>7.74</td><td>7.31</td></tr><tr><td>1991</td><td>30.46</td><td>19.36</td><td>4.43</td></tr><tr><td>1992</td><td>7.62</td><td>7.34</td><td>2.92</td></tr><tr><td>1993</td><td>10.08</td><td>13.06</td><td>2.96</td></tr><tr><td>1994</td><td>1.32</td><td>-7.32</td><td>5.45</td></tr><tr><td>1995</td><td>37.58</td><td>25.94</td><td>5.60</td></tr><tr><td>1996</td><td>22.96</td><td>0.13</td><td>5.29</td></tr><tr><td>1997</td><td>33.36</td><td>12.02</td><td>5.50</td></tr><tr><td>1998</td><td>28.58</td><td>14.45</td><td>4.68</td></tr><tr><td>1999</td><td>21.04</td><td>-7.51</td><td>5.30</td></tr><tr><td>2000</td><td>-9.10</td><td>17.22</td><td>6.40</td></tr><tr><td>2001</td><td>-11.89</td><td>5.51</td><td>1.82</td></tr><tr><td>2002</td><td>-22.10</td><td>15.15</td><td>1.24</td></tr><tr><td>2003</td><td>28.68</td><td>0.54</td><td>0.98</td></tr></table>

Let $R _ { i }$ denote the random rate of return of asset i. From the above historical data, we can compute the arithmetic mean rate of return for each asset: 

$$
\bar {r} _ {i} = \frac {1}{T} \sum_ {t = 1} ^ {T} r _ {i t},
$$

which gives 

<table><tr><td></td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>Arithmetic mean <eq>\bar{r}_{i}</eq></td><td>12.06 %</td><td>7.85 %</td><td>6.32 %</td></tr></table>

Since the rates of return are multiplicative over time, we prefer to use the geometric mean instead of the arithmetic mean. The geometric mean is the constant yearly rate of return that needs to be applied in years $t = 0$ through $t = T - 1$ in order to get the compounded Total Return $I _ { i T }$ , starting from $I _ { i 0 }$ . The formula for the geometric mean is: 

$$
\mu_ {i} = \left(\prod_ {t = 1} ^ {T} (1 + r _ {i t})\right) ^ {\frac {1}{T}} - 1.
$$

We get the following results. 

<table><tr><td></td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>Geometric mean <eq>\mu_{i}</eq></td><td>10.73 %</td><td>7.37 %</td><td>6.27 %</td></tr></table>

We also compute the covariance matrix: 

$$
\operatorname{cov} (R _ {i}, R _ {j}) = \frac {1}{T} \sum_ {t = 1} ^ {T} (r _ {i t} - \bar {r} _ {i}) (r _ {j t} - \bar {r} _ {j}).
$$

<table><tr><td>Covariance</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>Stocks</td><td>0.02778</td><td>0.00387</td><td>0.00021</td></tr><tr><td>Bonds</td><td>0.00387</td><td>0.01112</td><td>-0.00020</td></tr><tr><td>MM</td><td>0.00021</td><td>-0.00020</td><td>0.00115</td></tr></table>

It is interesting to compute the volatility of the rate of return on each asset $\sigma _ { i } = \sqrt { \mathrm { c o v } ( R _ { i } , R _ { i } ) }$ 

<table><tr><td></td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>Volatility</td><td>16.67 %</td><td>10.55 %</td><td>3.40 %</td></tr></table>

and the correlation matrix $\rho _ { i j } = { \frac { \mathrm { c o v } ( R _ { i } , R _ { j } ) } { \sigma _ { i } \sigma _ { j } } }$ 

<table><tr><td>Correlation</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>Stocks</td><td>1</td><td>0.2199</td><td>0.0366</td></tr><tr><td>Bonds</td><td>0.2199</td><td>1</td><td>-0.0545</td></tr><tr><td>MM</td><td>0.0366</td><td>-0.0545</td><td>1</td></tr></table>

Setting up the $\mathrm { Q P }$ for portfolio optimization 

$$
\begin{array}{r l} \min & 0. 0 2 7 7 8 x _ {S} ^ {2} + 2 \cdot 0. 0 0 3 8 7 x _ {S} x _ {B} + 2 \cdot 0. 0 0 0 2 1 x _ {S} x _ {M} \\ & + 0. 0 1 1 1 2 x _ {B} ^ {2} - 2 \cdot 0. 0 0 0 2 0 x _ {B} x _ {M} + 0. 0 0 1 1 5 x _ {M} ^ {2} \\ & 0. 1 0 7 3 x _ {S} + 0. 0 7 3 7 x _ {B} + 0. 0 6 2 7 x _ {M} \geq R \\ & x _ {S} + x _ {B} + x _ {M} = 1 \\ & x _ {S}, x _ {B}, x _ {M} \geq 0 \end{array}\tag{8.6}
$$

and solving it for $R = 6 . 5 \%$ to $R = 1 0 . 5 \%$ with increments of 0.5% we get the optimal portfolios shown in Table 8.1.1 and the corresponding variance. The optimal allocations on the eficient frontier are also depicted in the right-hand-side graph in Figure 8.1. 

Based on the first two columns of Table 8.1.1, the left-hand-side graph of Figure 8.1 plots the maximum expected rate of return R of a portfolio as a function of its volatility (standard deviation). This curve is the efficient frontier we discussed earlier. Every possible portfolio of consisting of long positions in stocks, bonds, and money market investments is represented by a point lying on or below the eficient frontier in the standard deviation/expected return plane. 

<table><tr><td>Rate of Return R</td><td>Variance</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>0.065</td><td>0.0010</td><td>0.03</td><td>0.10</td><td>0.87</td></tr><tr><td>0.070</td><td>0.0014</td><td>0.13</td><td>0.12</td><td>0.75</td></tr><tr><td>0.075</td><td>0.0026</td><td>0.24</td><td>0.14</td><td>0.62</td></tr><tr><td>0.080</td><td>0.0044</td><td>0.35</td><td>0.16</td><td>0.49</td></tr><tr><td>0.085</td><td>0.0070</td><td>0.45</td><td>0.18</td><td>0.37</td></tr><tr><td>0.090</td><td>0.0102</td><td>0.56</td><td>0.20</td><td>0.24</td></tr><tr><td>0.095</td><td>0.0142</td><td>0.67</td><td>0.22</td><td>0.11</td></tr><tr><td>0.100</td><td>0.0189</td><td>0.78</td><td>0.22</td><td>0</td></tr><tr><td>0.105</td><td>0.0246</td><td>0.93</td><td>0.07</td><td>0</td></tr></table>


Table 8.1: Eficient Portfolios


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/148d19f2e2c3d7414182e6fcaafe5fa9dbe75712b926234020ca71c58cba714b.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/10819580eb04864dbb2527a06195de0aa349a77b8409fbb89e53fec28434ea60.jpg)



Figure 8.1: Eficient Frontier and the Composition of Eficient Portfolios


Exercise 8.3 Solve Markowitz’s MVO model for constructing a portfolio of US stocks, bonds and cash using arithmetic means, instead of geometric means as above. Vary R from 6.5 % to 12 % with increments of 0.5 % . Compare with the results obtained above. 

Exercise 8.4 In addition to the three securities given earlier (S&P 500 Index, 10-year Treasury Bond Index and Money Market), consider a 4th security (the NASDAQ Composite Index) with following “Total Return”: 

<table><tr><td>Year</td><td>NASDAQ</td></tr><tr><td>1960</td><td>34.461</td></tr><tr><td>1961</td><td>45.373</td></tr><tr><td>1962</td><td>38.556</td></tr><tr><td>1963</td><td>46.439</td></tr><tr><td>1964</td><td>57.175</td></tr><tr><td>1965</td><td>66.982</td></tr><tr><td>1966</td><td>63.934</td></tr><tr><td>1967</td><td>80.935</td></tr><tr><td>1968</td><td>101.79</td></tr><tr><td>1969</td><td>99.389</td></tr><tr><td>1970</td><td>89.607</td></tr><tr><td>1971</td><td>114.12</td></tr><tr><td>1972</td><td>133.73</td></tr><tr><td>1973</td><td>92.190</td></tr><tr><td>1974</td><td>59.820</td></tr></table>

<table><tr><td>Year</td><td>NASDAQ</td></tr><tr><td>1975</td><td>77.620</td></tr><tr><td>1976</td><td>97.880</td></tr><tr><td>1977</td><td>105.05</td></tr><tr><td>1978</td><td>117.98</td></tr><tr><td>1979</td><td>151.14</td></tr><tr><td>1980</td><td>202.34</td></tr><tr><td>1981</td><td>195.84</td></tr><tr><td>1982</td><td>232.41</td></tr><tr><td>1983</td><td>278.60</td></tr><tr><td>1984</td><td>247.35</td></tr><tr><td>1985</td><td>324.39</td></tr><tr><td>1986</td><td>348.81</td></tr><tr><td>1987</td><td>330.47</td></tr><tr><td>1988</td><td>381.38</td></tr><tr><td>1989</td><td>454.82</td></tr></table>

<table><tr><td>Year</td><td>NASDAQ</td></tr><tr><td>1990</td><td>373.84</td></tr><tr><td>1991</td><td>586.34</td></tr><tr><td>1992</td><td>676.95</td></tr><tr><td>1993</td><td>776.80</td></tr><tr><td>1994</td><td>751.96</td></tr><tr><td>1995</td><td>1052.1</td></tr><tr><td>1996</td><td>1291.0</td></tr><tr><td>1997</td><td>1570.3</td></tr><tr><td>1998</td><td>2192.7</td></tr><tr><td>1999</td><td>4069.3</td></tr><tr><td>2000</td><td>2470.5</td></tr><tr><td>2001</td><td>1950.4</td></tr><tr><td>2002</td><td>1335.5</td></tr><tr><td>2003</td><td>2003.4</td></tr></table>


Construct a portfolio consisting of the S&P 500 index, the NASDAQ index, the 10-year Treasury bond index and cash, using Markowitz’s MVO model. Solve the model for diferent values of R.


Exercise 8.5 Repeat the previous exercise, this time assuming that one can leverage the portfolio up to 50% by borrowing at the money market rate. How do the risk/return profiles of optimal portfolios change with this relaxation? How do your answers change if the borrowing rate for cash is expected to be 1% higher than the lending rate? 

## 8.1.2 Large-Scale Portfolio Optimization

In this section, we consider practical issues that arise when the Mean-Variance model is used to construct a portfolio from a large underlying family of assets. For concreteness, let us consider a portfolio of stocks constructed from a set of n stocks with known expected returns and covariance matrix, where n may be in the hundreds or thousands. 

## Diversification

In general, there is no reason to expect that solutions to the Markowitz model will be well diversified portfolios. In fact, this model tends to produce portfolios with unreasonably large weights in certain asset classes and, when short positions are allowed, unintuitively large short positions. This issue is well documented in the literature, including the paper by Green and Hollifield [34] and is often attributed to estimation errors. Estimates that may be slightly “of” may lead the optimizer to chase phantom low-risk highreturn opportunities by taking large positions. Hence, portfolios chosen by this quadratic program may be subject to idiosyncratic risk. Practitioners often use additional constraints on the $x _ { i } \mathrm { { ^ { s } } }$ to insure themselves against estimation and model errors and to ensure that the chosen portfolio is well diversified. For example, a limit m may be imposed on the size of each $x _ { i }$ say 

$$
x _ {i} \leq m \quad \text { for } i = 1, \ldots , n.
$$

One can also reduce sector risk by grouping together investments in securities of a sector and setting a limit on the exposure to this sector. For example, if $m _ { k }$ is the maximum that can be invested in sector k, we add the constraint 

$$
\sum_ {i \text {in sector} k} x _ {i} \leq m _ {k}.
$$

Note however that, the more constraints one adds to a model, the more the objective value deteriorates. So the above approach to producing diversification, at least ex ante, can be quite costly. 

## Transaction Costs

We can add a portfolio turnover constraint to ensure that the change between the current holdings $x ^ { 0 }$ and the desired portfolio x is bounded by h. This constraint is essential when solving large mean-variance models since the covariance matrix is almost singular in most practical applications and hence the optimal decision can change significantly with small changes in the problem data. To avoid big changes when reoptimizing the portfolio, turnover constraints are imposed. Let $y _ { i }$ be the amount of asset i bought and $z _ { i }$ the amount sold. We write 

$$
\begin{array}{l} x _ {i} - x _ {i} ^ {0} \leq y _ {i}, \quad y _ {i} \geq 0, \\ x _ {i} ^ {0} - x _ {i} \leq z _ {i}, \quad z _ {i} \geq 0, \\ \sum_ {i = 1} ^ {n} (y _ {i} + z _ {i}) \leq h. \end{array}
$$

Instead of a turnover constraint, we can introduce transaction costs directly into the model. Suppose that there is a transaction cost t<sub>i</sub> proportional to the amount of asset i bought, and a transaction cost $t _ { i } ^ { \prime }$ proportional to the amount of asset i sold. Suppose that the portfolio is reoptimized once per period. As above, let $x ^ { 0 }$ denote the current portfolio. Then a reoptimized portfolio is obtained by solving 

$$
\min \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} \sigma_ {i j} x _ {i} x _ {j}
$$

subject to 

$$
\sum_ {i = 1} ^ {n} (\mu_ {i} x _ {i} - t _ {i} y _ {i} - t _ {i} ^ {\prime} z _ {i}) \geq R
$$

$$
\sum_ {i = 1} ^ {n} x _ {i} = 1
$$

$$
x _ {i} - x _ {i} ^ {0} \leq y _ {i} \quad {\mathrm{for}} i = 1, \ldots , n
$$

$$
x _ {i} ^ {0} - x _ {i} \leq z _ {i} \quad \mathrm{for} i = 1, \ldots , n
$$

$$
\begin{array}{l l} y _ {i} \geq 0 & \text { for } i = 1, \ldots , n \\ z _ {i} \geq 0 & \text { for } i = 1, \ldots , n \\ x _ {i} \text { unrestricted   for } i = 1, \ldots , n. \end{array}
$$

## Parameter Estimation

The Markowitz model gives us an optimal portfolio assuming that we have perfect information on the $\mu _ { i } \mathrm { { ^ { s } } }$ and $\sigma _ { i j } \mathrm { ^ { * } s }$ for the assets that we are considering. Therefore, an important practical issue is the estimation of the $\mu _ { i } { } ^ { \mathrm { ' } } \mathrm { s }$ and $\sigma _ { i j } \mathrm { ^ { * } s }$ 

A reasonable approach for estimating these data is to use time series of past returns $( r _ { i t } =$ return of asset i from time $t - 1$ to time t, where $i = 1 , \ldots , n , t = 1 , \ldots , T )$ . Unfortunately, it has been observed that small changes in the time series $r _ { i t }$ lead to changes in the $\mu _ { i } \mathrm { { ^ { s } } }$ and $\sigma _ { i j } \mathrm { ^ { * } s }$ that often lead to significant changes in the “optimal” portfolio. 

Markowitz recommends using the $\beta \mathrm { ^ { * } s }$ of the securities to calculate the $\mu _ { i } \mathrm { { ^ { s } } }$ and $\sigma _ { i j }$ ’s as follows. Let 

$$
\begin{array}{r c l} r _ {i t} & = & \text {return of asset i in period t,i = 1,\ldots,n, and t = 1,\ldots,T}, \\ r _ {m t} & = & \text {market return in period t}, \\ r _ {f t} & = & \text {return of risk - free asset in period t}. \end{array}
$$

We estimate $\beta _ { i }$ by a linear regression based on the capital asset pricing model 

$$
r _ {i t} - r _ {f t} = \beta_ {i} (r _ {m t} - r _ {f t}) + \varepsilon_ {i t}
$$

where the vector $\varepsilon _ { i }$ represents the idiosyncratic risk of asset i. We assume that cov $\begin{array} { r } { ( \varepsilon _ { i } , \varepsilon _ { j } ) = 0 } \end{array}$ . The $\beta \mathrm { ^ { * } s }$ can also be purchased from financial research groups and risk model providers. 

Knowing $\beta _ { i }$ , we compute $\mu _ { i }$ by the relation 

$$
\mu_ {i} - E (r _ {f}) = \beta_ {i} (E (r _ {m}) - E (r _ {f}))
$$

and $\sigma _ { i j }$ by the relation 

$$
\begin{array}{c} \sigma_ {i j} = \beta_ {i} \beta_ {j} \sigma_ {m} ^ {2} \text {for} i \neq j \\ \sigma_ {i i} = \beta_ {i} ^ {2} \sigma_ {m} ^ {2} + \sigma_ {\varepsilon_ {i}} ^ {2} \end{array}
$$

where $\sigma _ { m } ^ { 2 }$ denotes the variance of the market return and $\sigma _ { \varepsilon _ { i } } ^ { 2 }$ the variance of the idiosyncratic risk. 

But the fundamental weakness of the Markowitz model remains, no matter how cleverly the $\mu _ { i } \mathrm { { ^ { s } } }$ and $\sigma _ { i j } \mathrm { ^ { * } s }$ are computed: The solution is extremely sensitive to small changes in the data. Only one small change in one $\mu _ { i }$ may produce a totally diferent portfolio x. What can be done in practice to overcome this problem, or at least reduce it? Michaud [51] recommends to resample returns from historical data to generate alternative $\mu$ and $\sigma$ estimates, to solve the MVO problem repeatedly with inputs generated this way, and then to combine the optimal portfolios obtained in this manner. Robust optimization approaches provide an alternative strategy to mitigate the input sensitivity in MVO models; we discuss some examples in Chapters 19 and 20. Another interesting approach is considered in the next section. 

Exercise 8.6 Express the following restrictions as linear constraints: 

(i) The $\beta$ of the portfolio should be between 0.9 and 1.1 . 

(ii) Assume that the stocks are partitioned by capitalization: large, medium and small. We want the portfolio to be divided evenly between large and medium cap stocks, and the investment in small cap stocks to be between two and three times the investment in large cap stocks. 

Exercise 8.7 Using historical returns of the stocks in the DJIA, estimate their mean $\mu _ { i }$ and covariance matrix. Let R be the median of the $\mu _ { i } \mathrm { s }$ 

(i) Solve Markowitz’s MVO model to construct a portfolio of stocks from the DJIA that has expected return at least R. 

(ii) Generate a random value uniformly in the interval $[ 0 . 9 5 \mu _ { i } , 1 . 0 5 \mu _ { i } ]$ 2 for each stock i. Resolve Markowitz’s MVO model with these mean returns, instead of $\mu _ { i } \mathrm { s }$ as in (i). Compare the results obtained in (i) and (ii). 

(iii) Repeat three more times and average the five portfolios found in (i), (ii) and (iii). Compare this portfolio with the one found in (i). 

## 8.1.3 The Black-Litterman Model

Black and Litterman [13] recommend to combine the investor’s view with the market equilibrium, as follows. 

The expected return vector $\mu$ is assumed to have a probability distribution that is the product of two multivariate normal distributions. The first distribution represents the returns at market equilibrium, with mean π and covariance matrix $\tau \Sigma$ , where $\tau$ is a small constant and $\Sigma = \left( \sigma _ { i j } \right)$ denotes the covariance matrix of asset returns (Note that the factor $\tau$ should be small since the variance $\tau \sigma _ { i } ^ { 2 }$ of the random variable $\mu _ { i }$ is typically much smaller than the variance $\sigma _ { i } ^ { 2 }$ of the underlying asset returns). The second distribution represents the investor’s view about the $\mu _ { i } \mathrm { { ^ { s } } }$ . These views are expressed as 

$$
P \mu = q + \varepsilon
$$

where $P$ is a $k \times n$ matrix and $q$ is a k-dimensional vector that are provided by the investor and $\varepsilon$ is a normally distributed random vector with mean 0 and diagonal covariance matrix Ω (the stronger the investor’s view, the smaller the corresponding $\omega _ { i } = \Omega _ { i i } )$ 

The resulting distribution for $\mu$ is a multivariate normal distribution with mean 

$$
\bar {\mu} = [ (\tau \Sigma) ^ {- 1} + P ^ {T} \Omega^ {- 1} P ] ^ {- 1} [ (\tau \Sigma) ^ {- 1} \pi + P ^ {T} \Omega^ {- 1} q ].\tag{8.7}
$$

Black and Litterman use $\bar { \mu }$ as the vector of expected returns in the Markowitz model. 


Example 8.1 Let us illustrate the Black-Litterman approach on the example of Section 8.1.1. The expected returns on Stocks, Bonds and Money Market were computed to be


<table><tr><td></td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>Market Rate of Return</td><td>10.73 %</td><td>7.37 %</td><td>6.27 %</td></tr></table>

This is what we use for the vector π representing market equilibrium. In practice, π is obtained from the vector of shares of global wealth invested in diferent asset classes via reverse optimization. We need to choose the value of the small constant τ . We take $\tau = 0 . 1$ . We have two views that we would like to incorporate into the model. First, we hold a strong view that the Money Market rate will be 2% next year. Second, we also hold the view that S&P 500 will outperform 10-year Treasury Bonds by 5% but we are not as confident about this view. These two views can be expressed as follows 

$$
\mu_ {M} = 0. 0 2 \text {strong view:} \omega_ {1} = 0. 0 0 0 0 1\tag{8.8}
$$

$$
\mu_ {S} - \mu_ {B} = 0. 0 5 w e a k e r v i e w: \omega_ {2} = 0. 0 0 1
$$

$$
T h u s P = \left( \begin{array}{c c c} 0 & 0 & 1 \\ 1 & - 1 & 0 \end{array} \right), q = \binom{0. 0 2}{0. 0 5} a n d \Omega = \left( \begin{array}{c c} 0. 0 0 0 0 1 & 0 \\ 0 & 0. 0 0 1 \end{array} \right).
$$


Applying formula (8.7) to compute $\bar { \mu } _ { ; }$ , we get


<table><tr><td></td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>Mean Rate of Return <eq>\bar{\mu}</eq></td><td>11.77 %</td><td>7.51 %</td><td>2.34 %</td></tr></table>

We solve the same $Q P$ as in $( 8 . 6 )$ except for the modified expected return constraint: 

$$
\begin{array}{r l} \min & 0. 0 2 7 7 8 x _ {S} ^ {2} + 2 \cdot 0. 0 0 3 8 7 x _ {S} x _ {B} + 2 \cdot 0. 0 0 0 2 1 x _ {S} x _ {M} \\ & + 0. 0 1 1 1 2 x _ {B} ^ {2} - 2 \cdot 0. 0 0 0 2 0 x _ {B} x _ {M} + 0. 0 0 1 1 5 x _ {M} ^ {2} \\ & 0. 1 1 7 7 x _ {S} + 0. 0 7 5 1 x _ {B} + 0. 0 2 3 4 x _ {M} \geq R \\ & x _ {S} + x _ {B} + x _ {M} = 1 \\ & x _ {S}, x _ {B}, x _ {M} \geq 0 \end{array}\tag{8.9}
$$

Solving for $R = 4 . 0 \%$ to $R = 1 1 . 5 \%$ with increments of 0.5% we now get the optimal portfolios and the eficient frontier depicted in Table 8.1.3 and Figure 8.2. 

Exercise 8.8 Repeat the example above, with the same investor’s views, but adding the 4th security of Exercise 8.4 (the NASDAQ Composite Index). 

Black and Litterman give the following intuition for their approach using the following example. Suppose we know the true structure of the asset returns: For each asset, the return is composed of an equilibrium risk premium plus a common factor and an independent shock. 

$$
R _ {i} = \pi_ {i} + \gamma_ {i} Z + \nu_ {i}
$$

<table><tr><td>Rate of Return R</td><td>Variance</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>0.040</td><td>0.0012</td><td>0.08</td><td>0.17</td><td>0.75</td></tr><tr><td>0.045</td><td>0.0015</td><td>0.11</td><td>0.21</td><td>0.68</td></tr><tr><td>0.050</td><td>0.0020</td><td>0.15</td><td>0.24</td><td>0.61</td></tr><tr><td>0.055</td><td>0.0025</td><td>0.18</td><td>0.28</td><td>0.54</td></tr><tr><td>0.060</td><td>0.0032</td><td>0.22</td><td>0.31</td><td>0.47</td></tr><tr><td>0.065</td><td>0.0039</td><td>0.25</td><td>0.35</td><td>0.40</td></tr><tr><td>0.070</td><td>0.0048</td><td>0.28</td><td>0.39</td><td>0.33</td></tr><tr><td>0.075</td><td>0.0059</td><td>0.32</td><td>0.42</td><td>0.26</td></tr><tr><td>0.080</td><td>0.0070</td><td>0.35</td><td>0.46</td><td>0.19</td></tr><tr><td>0.085</td><td>0.0083</td><td>0.38</td><td>0.49</td><td>0.13</td></tr><tr><td>0.090</td><td>0.0096</td><td>0.42</td><td>0.53</td><td>0.05</td></tr><tr><td>0.095</td><td>0.0111</td><td>0.47</td><td>0.53</td><td>0</td></tr><tr><td>0.100</td><td>0.0133</td><td>0.58</td><td>0.42</td><td>0</td></tr><tr><td>0.105</td><td>0.0163</td><td>0.70</td><td>0.30</td><td>0</td></tr><tr><td>0.110</td><td>0.0202</td><td>0.82</td><td>0.18</td><td>0</td></tr><tr><td>0.115</td><td>0.0249</td><td>0.94</td><td>0.06</td><td>0</td></tr></table>


Table 8.2: Black-Litterman Eficient Portfolios


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/6a3c52307c2e4cce22bb5c668487ddd616655abcafbdf78be887e84b091fb47f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/45eb87e8ed9a22667d146b9d40b239076845d286c8cd133f6210673de8681250.jpg)



Figure 8.2: Eficient Frontier and the Composition of Eficient Portfolios using the Black-Litterman approach


where 

$R _ { i }$ = the return on the ith asset, 

$\pi _ { i }$ = the equilibrium risk premium on the ith asset, 

$Z$ = a common factor, 

$\gamma _ { i }$ = the impact of Z on the ith asset, 

$\nu _ { i }$ = an independent shock to the ith asset. 

The covariance matrix Σ of asset returns is assumed to be known. The expected returns of the assets are given by: 

$$
\mu_ {i} = \pi_ {i} + \gamma_ {i} E [ Z ] + E [ \nu_ {i} ].
$$

While a consideration of the equilibrium motivates the Black-Litterman model, they do not assume that $E [ Z ]$ and $E [ \nu _ { i } ]$ are equal to 0 which would indicate that the expected excess returns are equal to the equilibrium risk premiums. Instead, they assume that the expected excess returns $\mu _ { i }$ are unobservable random variables whose distribution is determined by the distribution of $E [ Z ]$ and $E [ \nu _ { i } ] \mathrm { { { s } } }$ . Their additional assumptions imply that the covariance matrix of expected returns is $\tau \Sigma$ for some small positive scalar τ. All this information is assumed to be known to all investors. 

Investors difer in the additional, subjective informative they have about future returns. They express this information as their “views” such as “I expect that asset A will outperform asset B by $2 \% ^ { 9 }$ . Coupled with a measure of confidence, such views can be incorporated into the equilibrium returns to generate conditional distribution of the expected returns. For example, if we assume that the equilibrium distribution of $\mu$ is given by the normal distribution $\mathrm { N } ( \pi , \tau \Sigma )$ and views are represented using the constraint $P \mu = q$ (with 100% confidence), the mean $\bar { \mu }$ of the normal distribution conditional on this view is obtained as the optimal solution of the following quadratic optimization problem: 

$$
\begin{array}{l l} \min & (\mu - \pi) ^ {T} (\tau \Sigma) ^ {- 1} (\mu - \pi) \\ \mathrm{s.t.} & \mu_ {A} - \mu_ {B} = q. \end{array}\tag{8.10}
$$

Using the KKT optimality conditions presented in Section 5.5, the solution to the above minimization problem can be shown to be 

$$
\bar {\mu} = \pi + (\tau \Sigma) P ^ {T} [ P (\tau \Sigma) P ^ {T} ] ^ {- 1} (q - P \pi).\tag{8.11}
$$

Exercise 8.9 Prove that $\bar { \mu }$ in (8.11) solves (8.10) using KKT conditions. 

Of course, one rarely has 100% confidence in his/her views. In the more general case, the views are expressed as $P \mu = q + \varepsilon$ where P and $q$ are given by the investor as above and ε is an unobservable normally distributed random vector with mean 0 and diagonal covariance matrix Ω. A diagonal Ω corresponds to the assumption that the views are independent. When this is the case, $\bar { \mu }$ is given by the Black-Litterman formula 

$$
\bar {\mu} = [ (\tau \Sigma) ^ {- 1} + P ^ {T} \Omega^ {- 1} P ] ^ {- 1} [ (\tau \Sigma) ^ {- 1} \pi + P ^ {T} \Omega^ {- 1} q ],
$$

as stated earlier. We refer to the Black and Litterman paper for additional details and an example of an international portfolio [13]. 

Exercise 8.10 Repeat Exercise 8.4, this time using the Black-Litterman methodology outlined above. Use the expected returns you computed in Exercise 8.4 as equilibrium returns and incorporate the view that NASDAQ stocks will outperform the S & P 500 stocks by $4 \%$ and that the average of NASDAQ and S & P 500 returns will exceed bond returns by 3%. Both views are relatively strong and are expressed with $\omega _ { 1 } = \omega _ { 2 } = 0 . 0 0 0 1$ 

## 8.1.4 Mean-Absolute Deviation to Estimate Risk

Konno and Yamazaki [43] propose a linear programming model instead of the classical quadratic model. Their approach is based on the observation that diferent measures of risk, such a volatility and $L _ { \mathrm { { 1 ^ { - r i s k } } } }$ , are closely related, and that alternate measures of risk are also appropriate for portfolio optimization. 

The volatility of the portfolio return is 

$$
\sigma = \sqrt {E [ (\sum_ {i = 1} ^ {n} (R _ {i} - \mu_ {i}) x _ {i}) ^ {2} ]}
$$

where $R _ { i }$ denotes the random return of asset $i ,$ and $\mu _ { i }$ denotes its mean. 

The $L _ { 1 } .$ -risk of the portfolio return is defined as 

$$
w = E [ | \sum_ {i = 1} ^ {n} (R _ {i} - \mu_ {i}) x _ {i} | ].
$$

Theorem 8.1 (Konno and Yamazaki) $I f \left( R _ { 1 } , \ldots , R _ { n } \right)$ are multivariate normally distributed random variables, then $w = \textstyle { \sqrt { \frac { 2 } { \pi } } } \sigma$ 

Proof: 

Let $( \mu _ { 1 } , \ldots , \mu _ { n } )$ be the mean of $( R _ { 1 } , \ldots , R _ { n } )$ . Also let $\Sigma = ( \sigma _ { i j } ) \in I R ^ { n \times n }$ be the covariance matrix of $( R _ { 1 } , \ldots , R _ { n } )$ . Then $\sum R _ { i } x _ { i }$ is normally distributed [59] with mean $\sum \mu _ { i } x _ { i }$ Pand standard deviation 

$$
\sigma (x) = \sqrt {\sum_ {i} \sum_ {j} \sigma_ {i j} x _ {i} x _ {j}}.
$$

Therefore $w = E [ | U | ]$ where $U \sim N ( 0 , \sigma )$ 

$$
w (x) = \frac {1}{\sqrt {2 \pi} \sigma (x)} \int_ {- \infty} ^ {+ \infty} | u | e ^ {- \frac {u ^ {2}}{2 \sigma^ {2} (x)}} d u = \frac {2}{\sqrt {2 \pi} \sigma (x)} \int_ {0} ^ {+ \infty} u e ^ {- \frac {u ^ {2}}{2 \sigma^ {2} (x)}} d u = \sqrt {\frac {2}{\pi}} \sigma (x).
$$

This theorem implies that minimizing $\sigma$ is equivalent to minimizing w when $( R _ { 1 } , \ldots , R _ { n } )$ is multivariate normally distributed. With this assumption, the Markowitz model can be formulated as 

$$
\min E [ | \sum_ {i = 1} ^ {n} (R _ {i} - \mu_ {i}) x _ {i} | ]
$$

subject to 

$$
\sum_ {i = 1} ^ {n} \mu_ {i} x _ {i} \geq R
$$

$$
\sum_ {i = 1} ^ {n} x _ {i} = 1
$$

$$
0 \leq x _ {i} \leq m _ {i} \quad \text { for } i = 1, \dots , n.
$$

Whether $( R _ { 1 } , \ldots , R _ { n } )$ has a multivariate normal distribution or not, the above Mean-Absolute Deviation (MAD) model constructs eficient portfolios for the $L _ { \mathrm { { 1 ^ { - r i s k } } } }$ measure. Let $r _ { i t }$ be the realization of random variable $R _ { i }$ during period t for $t = 1 , \dots , T$ , which we assume to be available through the historical data or from future projection. Then 

$$
\mu_ {i} = \frac {1}{T} \sum_ {t = 1} ^ {T} r _ {i t}
$$

Furthermore 

$$
E [ | \sum_ {i = 1} ^ {n} (R _ {i} - \mu_ {i}) x _ {i} | ] = \frac {1}{T} \sum_ {t = 1} ^ {T} | \sum_ {i = 1} ^ {n} (r _ {i t} - \mu_ {i}) x _ {i} |
$$

Note that the absolute value in this expression makes it nonlinear. But it can be linearized using additional variables. Indeed, one can replace x by $y + z$ where $x = y - z$ and $y , z \geq 0$ . When the objective is to minimize $y + z$ , at most one of y or z will be positive. Therefore the model can be rewritten as 

$$
\min \sum_ {t = 1} ^ {T} y _ {t} + z _ {t}
$$

subject to 

$$
y _ {t} - z _ {t} = \sum_ {i = 1} ^ {n} (r _ {i t} - \mu_ {i}) x _ {i} \quad \mathrm{for} t = 1, \ldots , T
$$

$$
\sum_ {i = 1} ^ {n} \mu_ {i} x _ {i} \geq R
$$

$$
\sum_ {i = 1} ^ {n} x _ {i} = 1
$$

$$
0 \leq x _ {i} \leq m _ {i} \quad \text { for } i = 1, \ldots , n
$$

$$
y _ {t} \geq 0, z _ {t} \geq 0 \mathrm{for} t = 1, \ldots , T
$$

This is a linear program! Therefore this approach can be used to solve large scale portfolio optimization problems. 

Example 8.2 We illustrate the approach on our $\mathcal { B } \mathrm { - }$ asset example, using the historical data on stocks, bonds and cash given in Section 8.1.1. Solving the linear program for $R = 6 . 5 \%$ to $R = 1 0 . 5 \%$ with increments of 0.5 % we get the optimal portfolios and the eficient frontier depicted in Table 8.2 and Figure 8.3. 

In the above table, we computed the variance of the MAD portfolio for each level R of the rate of return. These variances can be compared with the results obtained in Section 8.1.1 for the MVO portfolio. As expected, the variance of a MAD portfolio is always at least as large as that of the corresponding MVO portfolio. Note however that the diference is small. This indicates that, although the normality assumption of Theorem 8.1 does not hold, minimizing the $\scriptstyle { L _ { 1 } - r i s k }$ (instead of volatility) produces comparable portfolios. 

<table><tr><td>Rate of Return R</td><td>Variance</td><td>Stocks</td><td>Bonds</td><td>MM</td></tr><tr><td>0.065</td><td>0.0011</td><td>0.05</td><td>0.01</td><td>0.94</td></tr><tr><td>0.070</td><td>0.0015</td><td>0.15</td><td>0.04</td><td>0.81</td></tr><tr><td>0.075</td><td>0.0026</td><td>0.25</td><td>0.11</td><td>0.64</td></tr><tr><td>0.080</td><td>0.0046</td><td>0.32</td><td>0.28</td><td>0.40</td></tr><tr><td>0.085</td><td>0.0072</td><td>0.42</td><td>0.32</td><td>0.26</td></tr><tr><td>0.090</td><td>0.0106</td><td>0.52</td><td>0.37</td><td>0.11</td></tr><tr><td>0.095</td><td>0.0144</td><td>0.63</td><td>0.37</td><td>0</td></tr><tr><td>0.100</td><td>0.0189</td><td>0.78</td><td>0.22</td><td>0</td></tr><tr><td>0.105</td><td>0.0246</td><td>0.93</td><td>0.07</td><td>0</td></tr></table>


Table 8.3: Konno-Yamazaki Eficient Portfolios


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/c05962d3ebecf2037cab5238895cec97449023904a60e9082bef34b51fdab4df.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/e0dac41540129a1805e62379bd559457d0079f4c9a3321504206c4f20ed99e93.jpg)



Figure 8.3: Eficient Frontier and the Composition of Eficient Portfolios using the Konno-Yamazaki approach


Exercise 8.11 Add the 4th security of Exercise 8.4 (the NASDAQ Composite Index) to the 3-asset example. Solve the resulting MAD model for varying values of R. Compare with the portfolios obtained in Exercise 8.4. 

## 8.2 Maximizing the Sharpe Ratio

Consider the setting in Section 8.1. Recall that we denote with $R _ { \mathrm { m i n } }$ and $R _ { \mathrm { m a x } }$ the minimum and maximum expected returns for eficient portfolios. Let us define the function 

$$
\sigma (R): [ R _ {\mathrm{min}}, R _ {\mathrm{max}} ] \to I R, \sigma (R) := (x _ {R} ^ {T} \Sigma x _ {R}) ^ {1 / 2},
$$

where $x _ { R }$ denotes the unique solution of problem (8.1). Since we assumed that Σ is positive definite, it is easy to show that the function $\sigma ( R )$ is strictly convex in its domain. The eficient frontier is the graph 

$$
E = \bigl \{(R, \sigma (R)): R \in [ R _ {\mathrm{min}}, R _ {\mathrm{max}} ] \bigr \}.
$$

We now consider a riskless asset whose return is $r _ { f } \geq 0$ with probability 1. We will assume that $r _ { f } < R _ { \mathrm { m i n } }$ , which is natural since the portfolio $x _ { \mathrm { m i n } }$ has a positive risk associated with it while the riskless asset does not. 

Return/risk profiles of diferent combinations of a risky portfolio with the riskless asset can be represented as a straight line—a capital allocation line (CAL)—on the standard deviation vs. mean graph; see Figure 8.4. The optimal CAL is the CAL that lies below all the other CALs for $R > r _ { f }$ since the corresponding portfolios will have the lowest standard deviation for any given value of $R > r _ { f }$ . Then, it follows that this optimal CAL goes through a point on the eficient frontier and never goes above a point on the eficient frontier. In other words, the slope of the optimal CAL is a sub-derivative of the function $\sigma ( R )$ that defines the eficient frontier. The point where the optimal CAL touches the eficient frontier corresponds to the optimal risky portfolio. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/a7153be7c3d739abd8da69fb7a101c7a0c980baf210cda793b774792b4a858a0.jpg)



Figure 8.4: Capital Allocation Line


Alternatively, one can think of the optimal CAL as the CAL with the smallest slope. Mathematically, this can be expressed as the portfolio x that maximizes the quantity 

$$
h (x) = \frac {\mu^ {T} x - r _ {f}}{(x ^ {T} \Sigma x) ^ {1 / 2}},
$$

among all $x \in S .$ This quantity is precisely the reward-to-volatility ratio introduced by Sharpe to measure the performance of mutual funds [68]. This quantity is now more commonly known as the Sharpe ratio. The portfolio that maximizes the Sharpe ratio is found by solving the following problem: 

$$
\begin{array}{r l} \max _ {x} & \frac {\mu^ {T} x - r _ {f}}{(x ^ {T} \Sigma x) ^ {1 / 2}} \\ A x & = b \\ C x & \geq d. \end{array}\tag{8.12}
$$

In this form, this problem is not easy to solve. Although it has a nice polyhedral feasible region, its objective function is somewhat complicated, and worse, it is possibly non-concave. Therefore, (8.12) is not a convex optimization problem. The standard strategy to find the portfolio maximizing the Sharpe ratio, often called the optimal risky portfolio, is the following: First, one traces out the eficient frontier on a two dimensional return vs. standard deviation graph. Then, the point on this graph corresponding to the optimal risky portfolio is found as the tangency point of the line going through the point representing the riskless asset and is tangent to the eficient frontier. Once this point is identified, one can recover the composition of this portfolio from the information generated and recorded while constructing the eficient frontier. 

Here, we describe a direct method to obtain the optimal risky portfolio by constructing a convex quadratic programming problem equivalent to (8.12). We need two assumptions: First, we assume that $\textstyle \sum _ { i = 1 } ^ { n } x _ { i } = 1$ for any feasible Pportfolio x. This is a natural assumption since the x<sub>i</sub>s are the proportions of the portfolio in diferent asset classes. Second, we assume that there exists a feasible portfolio $\hat { x }$ with $\mu ^ { T } \hat { x } > r _ { f } { - } \mathrm { i f }$ all feasible portfolios have expected return bounded by the risk-free rate, there is no need to optimize, the risk-free investment dominates all others. 

Proposition 8.1 Given a set of feasible portfolios with the properties that $e ^ { T } x = 1 , \forall x \in \mathcal { X }$ and $\exists \hat { x } \in \mathcal { X } , \mu ^ { T } \hat { x } > r _ { f }$ , the portfolio $x ^ { * }$ with the maximum Sharpe ratio in this set can be found by solving the following problem 

$$
\min y ^ {T} \Sigma y s. t. (y, \kappa) \in \mathcal {X} ^ {+}, (\mu - r _ {f} e) ^ {T} y = 1,\tag{8.13}
$$

where 

$$
\mathcal {X} ^ {+} := \{x \in I R ^ {n}, \kappa \in I R | \kappa > 0, \frac {x}{\kappa} \in \mathcal {X} \} \cup (0, 0).\tag{8.14}
$$

$I f \left( y , \kappa \right)$ solves (8.13), then $\textstyle x ^ { * } = { \frac { y } { \kappa } }$ 

Problem (8.13) is a quadratic program and can be solved using the methods discussed in Chapter 7. Proof: 

By our second assumption, it sufices to consider only those x for which $( \mu - r _ { f } e ) ^ { T } x > 0$ . Let us make the following change of variables in (8.12): 

$$
\begin{array}{r c l} \kappa & = & \frac {1}{(\mu - r _ {f} e) ^ {T} x} \\ y & = & \kappa x. \end{array}
$$

Then, $\begin{array} { r } { \sqrt { x ^ { T } \Sigma x } = \frac { 1 } { \kappa } \sqrt { y ^ { T } \Sigma y } } \end{array}$ and the objective function of (8.12) can be written as $1 / \sqrt { y ^ { T } \Sigma y }$ in terms of the new variables. Note also that 

$$
\left(\mu - r _ {f} e\right) ^ {T} x > 0, x \in \mathcal {X} \Leftrightarrow \kappa > 0, \frac {y}{\kappa} \in \mathcal {X},
$$

and 

$$
\kappa = \frac {1}{(\mu - r _ {f} e) ^ {T} x} \Leftrightarrow (\mu - r _ {f} e) ^ {T} y = 1
$$

given $y / \kappa = x$ . Thus, (8.12) is equivalent to 

$$
\min y ^ {T} \Sigma y \mathrm{s.t.} \kappa > 0, (y, \kappa) \in \mathcal {X}, (\mu - r _ {f} e) ^ {T} y = 1.
$$

Since $( \mu - r _ { f } e ) ^ { T } y = 1$ rules out (0,0) as a solution, replacing $\kappa > 0 , ~ ( y , \kappa ) \in$ $\mathcal { X }$ with $( y , \kappa ) \in \mathcal { X } ^ { + }$ does not afect the solutions–it just makes the feasible set a closed set. 

Exercise 8.12 Show that $\mathcal { X } ^ { + }$ is a cone. If $\mathcal { X } = \{ x | A x \ge b , C x = d \}$ show that $\mathcal { X } ^ { + } ~ = ~ \{ ( x , \kappa ) | A x - b \kappa ~ \geq ~ 0 , C x - d \kappa ~ = ~ 0 , \kappa ~ \geq ~ 0 \}$ . What if $\mathcal { X } = \{ x : \| x \| \leq 1 \} ?$ 

Exercise 8.13 Find the Sharpe ratio maximizing portfolio of the four assets in Exercise 8.4 assuming that the risk-free return rate is 3% by solving the QP (8.13) resulting from its reformulation. Verify that the CAL passing through the point representing the standard deviation and the expected return of this portfolio is tangent to the eficient frontier. 

## 8.3 Returns-Based Style Analysis

In two very influential articles, Sharpe described how constrained optimization techniques can be used to determine the efective asset mix of a fund using only the return time series for the fund and contemporaneous time series for returns of a number of carefully chosen asset classes [66, 67]. Often, passive indices or index funds are used to represent the chosen asset classes and one tries to determine a portfolio of these funds and indices whose returns provide the best match for the returns of the fund being analyzed. The allocations in the portfolio can be interpreted as the fund’s style and consequently, this approach has become to known as returns-based style analysis, or RBSA. 

RBSA provides an inexpensive and timely alternative to fundamental analysis of a fund to determine its style/asset mix. Fundamental analysis uses the information on actual holdings of a fund to determine its asset mix. When all the holdings are known, the asset mix of the fund can be inferred easily. However, this information is rarely available, and when it is available, it is often quite expensive and several weeks or months old. Since RBSA relies only on returns data which is immediately available for publicly traded funds, and well-known optimization techniques, it can be employed in circumstances where fundamental analysis cannot be used. 

The mathematical model for RBSA is surprisingly simple. It uses the following generic linear factor model: Let $R _ { t }$ denote the return of a security– usually a mutual fund, but can be an index, etc.–in period t for $t = 1 , \dots , T$ where T corresponds to the number of periods in the modeling window. Further, let $F _ { i t }$ denote the return on factor i in period $t ,$ for $i = 1 , \ldots , n$ 2 $t = 1 , \dots , T$ . Then, $R _ { t }$ can be represented as follows: 

$$
\begin{array}{r c l} {R _ {t}} & = & {w _ {1 t} F _ {1 t} + w _ {2 t} F _ {2 t} + \ldots + w _ {n t} F _ {n t} + \varepsilon_ {t}} \\ & = & {F _ {t} w _ {t} + \varepsilon_ {t}, t = 1, \ldots , T.} \end{array}\tag{8.15}
$$

In this equation, $w _ { i t }$ quantities represent the sensitivities of $R _ { t }$ to each one of the n factors, and $\varepsilon _ { t }$ represents the non-factor return. We use the notation $w _ { t } = { \left| \begin{array} { l } { w _ { 1 t } , \dots , w _ { n t } } \end{array} \right| } ^ { T } { \mathrm { ~ a n d ~ } } F _ { t } = { \left| \begin{array} { l } { F _ { 1 t } , \dots , F _ { n t } } \end{array} \right| }$ 

The linear factor model (8.15) has the following convenient interpretation when the factor returns $F _ { i t }$ correspond to the returns of passive investments, such as those in an index fund for an asset class: One can form a benchmark portfolio of the passive investments (with weights $w _ { i t } )$ , and the diference between the fund return $R _ { t }$ and the return of the benchmark portfolio $F _ { t } w _ { t }$ is the non-factor return contributed by the fund manager using stock selection, market timing, etc. In other words, $\varepsilon _ { t }$ represents the additional return resulting from active management of the fund. Of course, this additional return can be negative. 

The benchmark portfolio return interpretation for the quantity $F _ { t } w _ { t }$ suggests that one should choose the sensitivities (or weights) $w _ { i t }$ such that they are all nonnegative and sum to one. With these constraints in mind, Sharpe proposes to choose $w _ { i t }$ to minimize the variance of the non-factor return $\varepsilon _ { t }$ . In his model, Sharpe restricts the weights to be constant over the period in consideration so that $w _ { i t }$ does not depend on t. In this case, we use $w = \left\lceil \begin{array} { l } { w _ { 1 } , \dots , w _ { n } } \end{array} \right\rceil ^ { T }$ to denote the time-invariant factor weights and formulate the following quadratic programming problem: 

$$
\begin{array}{l l} \min _ {w \in \mathbb {R} ^ {n}} & \operatorname{var} (\varepsilon_ {t}) = \operatorname{var} (R _ {t} - F _ {t} w) \\ \text {s.t.} & \sum_ {i = 1} ^ {n} w _ {i} = 1 \\ & w _ {i} \geq 0, \forall i. \end{array}\tag{8.16}
$$

The objective of minimizing the variance of the non-factor return $\varepsilon _ { t }$ deserves some comment. Since we are essentially formulating a tracking problem, and since $\varepsilon _ { t }$ represents the “tracking error”, one may wonder why we do not minimize the magnitude of this quantity rather than its variance. Since the Sharpe model interprets the quantity $\varepsilon _ { t }$ as a consistent management efect, the objective is to determine a benchmark portfolio such that the diference between fund returns and the benchmark returns is as close to constant (i.e., variance 0) as possible. $\mathrm { S o } .$ , we want the fund return and benchmark return graphs to show two almost parallel lines with the distance between these lines corresponding to manager’s consistent contribution to the fund return. This objective is almost equivalent to choosing weights in order to maximize the R-square of this regression model. The equivalence is not exact since we are using constrained regression and this may lead to correlation between $\varepsilon _ { t }$ and asset class returns. 

The objective function of this $\mathrm { Q P }$ can be easily computed: 

$$
\begin{array}{r c l} \operatorname{var} (R _ {t} - w ^ {T} F _ {t}) & = & \frac {1}{T} \sum_ {t = 1} ^ {T} (R _ {t} - w ^ {T} F _ {t}) ^ {2} - \left(\frac {\sum_ {t = 1} ^ {T} (R _ {t} - w ^ {T} F _ {t})}{T}\right) ^ {2} \\ & = & \frac {1}{T} \| R - F w \| ^ {2} - \left(\frac {e ^ {T} (R - F w)}{T}\right) ^ {2} \\ & = & \left(\frac {\| R \| ^ {2}}{T} - \frac {(e ^ {T} R) ^ {2}}{T ^ {2}}\right) - 2 \left(\frac {R ^ {T} F}{T} - \frac {e ^ {T} R}{T ^ {2}} e ^ {T} F\right) w \\ & & + w ^ {T} \left(\frac {1}{T} F ^ {T} F - \frac {1}{T ^ {2}} F ^ {T} e e ^ {T} F\right) w. \end{array}
$$

Above, we introduced and used the notation 

$$
R = \left[ \begin{array}{c} R _ {1} \\ \vdots \\ R _ {T} \end{array} \right], \text {and} F = \left[ \begin{array}{c} F _ {1} \\ \dots \\ F _ {T} \end{array} \right] = \left[ \begin{array}{c c c} F _ {1 1} & \ldots & F _ {n 1} \\ \vdots & \ddots & \vdots \\ F _ {1 T} & \ldots & F _ {n T} \end{array} \right]
$$

and e denotes a vector of ones of appropriate size. Convexity of this quadratic function of w can be easily verified. Indeed, 

$$
\frac {1}{T} F ^ {T} F - \frac {1}{T ^ {2}} F ^ {T} e e ^ {T} F = \frac {1}{T} F ^ {T} \left(I - \frac {e e ^ {T}}{T}\right) F,\tag{8.17}
$$

and the symmetric matrix $\begin{array} { r } { M = I - \frac { e e ^ { T } } { T } } \end{array}$ in the middle of the right-hand-side expression above is a positive semidefinite matrix with only two eigenvalues: 0 (multiplicity 1) and 1 (multiplicity $T - 1 )$ . Since M is positive semidefinite, so is $F ^ { T } M F$ and therefore the variance of $\varepsilon _ { t }$ is a convex quadratic function of w. Therefore, the problem (8.16) is convex quadratic programming problem and is easily solvable using well-known optimization techniques such as interior-point methods we discussed in Chapter 7. 

Exercise 8.14 Implement the returns-based style analysis approach to determine the efective asset mix of your favorite mutual fund. Use the following asset classes as your “factors”: Large growth stocks, large value stocks, small growth stocks, small value stocks, international stocks, and fixed income investments. You should obtain time series of returns representing these asset classes from on-line resources. You should also obtain a corresponding time series of returns for the mutual fund you picked for this exercise. Solve the problem using 30 periods of data $( \mathrm { i . e . , } T = 3 0 )$ 

## 8.4 Recovering Risk-Neural Probabilities from Options Prices

Recall our discussion on risk-neutral probability measures in Section 4.1.2. There, we considered a one-period economy with n securities. Current prices of these securities are denoted by $S _ { 0 } ^ { i }$ for $i = 1 , \ldots , n .$ . At the end of the current period, the economy will be in one of the states from the state space Ω. If the economy reaches state $\omega \in \Omega$ at the end of the current period, security i will have the payof $S _ { 1 } ^ { i } ( \omega )$ . We assume that we know all $S _ { 0 } ^ { i } { } ^ { , }$ s and $S _ { 1 } ^ { i } ( \omega ) ^ { \ast } \mathrm { s }$ but do not know the particular terminal state ω, which will be determined randomly. 

Let r denote the one-period (riskless) interest rate and let $R = 1 + r$ A risk neutral probability measure (RNPM) is defined as the probability measure under which the present value of the expected value of future payofs of a security equals its current price. More specifically, 

(discrete case:) on the state space $\Omega = \{ \omega _ { 1 } , \omega _ { 2 } , \ldots , \omega _ { m } \}$ , an RNPM is a vector of positive numbers $p 1 , p 2 , \ldots , p _ { m }$ such that 

1. $\begin{array} { r } { \sum _ { j = 1 } ^ { m } p _ { j } = 1 . } \end{array}$ 

2. $\begin{array} { r } { S _ { 0 } ^ { i } = \frac { 1 } { R } \sum _ { j = 1 } ^ { m } p _ { j } S _ { 1 } ^ { i } ( \omega _ { j } ) , \forall i . } \end{array}$ 

(continuous case:) on the state space $\Omega = ( a , b )$ an RNPM is a density function $p : \Omega \to { \cal R } _ { + }$ such that 

1. $\begin{array} { r } { \int _ { a } ^ { b } p ( \omega ) d \omega = 1 } \end{array}$ 

2. $\begin{array} { r } { S _ { 0 } ^ { i } = \frac { 1 } { R } \int _ { a } ^ { b } p ( \omega ) S _ { 1 } ^ { i } ( \omega ) d \omega , \forall i . } \end{array}$ 

Also recall the following result from Section 4.1.2 that is often called the First Fundamental Theorem of Asset Pricing: 

Theorem 8.2 A risk-neutral probability measure exists if and only if there are no arbitrage opportunities. 

If we can identify a risk-neutral probability measure associated with a given state space and a set of observed prices we can price any security for which we can determine the payofs for each state in the state space. Therefore, a fundamental problem in asset pricing is the identification of a RNPM consistent with a given set of prices. Of course, if the number of states in the state space is much larger than the number of observed prices, this problem becomes under-determined and we cannot obtain a sensible solution without introducing some additional structure into the RNPM we seek. In this section, we outline a strategy that guarantees the smoothness of the RNPM by constructing it through cubic splines. We first describe spline functions briefly: 

Consider a function $f : [ a , b ] \ \to \ { \mathcal { R } }$ to be estimated using its values $f _ { i } = f ( x _ { i } )$ given on a set of points $\{ x _ { i } \} , i = 1 , \ldots , m + 1$ . It is assumed that $x _ { 1 } = a$ and $x _ { m + 1 } = b$ 

A spline function, or spline, is a piecewise polynomial approximation $S ( x )$ to the function f such that the approximation agrees with f on each node $x _ { i } , \mathrm { i . e . , } S ( x _ { i } ) = f ( x _ { i } ) , \forall i$ 

The graph of a spline function S contains the data points $( x _ { i } , f _ { i } )$ (called knots) and is continuous on [a, b]. 

A spline on $[ a , b ]$ is of order n if (i) its first $n - 1$ derivatives exist on each interior knot, (ii) the highest degree for the polynomials defining the spline function is n. 

A cubic (third order) spline uses cubic polynomials of the form $f _ { i } ( x ) =$ $\alpha _ { i } x ^ { 3 } + \beta _ { i } x ^ { 2 } + \gamma _ { i } x + \delta _ { i }$ to estimate the function in each interval $[ x _ { i } , x _ { i + 1 } ]$ for $i = 1 , \ldots , m$ . A cubic spline can be constructed in such a way that it has second derivatives at each node. For $m + 1$ knots $( x _ { 1 } = a , \dots x _ { m + 1 } = b )$ in $[ a , b ]$ there are m intervals and, therefore 4m unknown constants to evaluate. To determine these 4m constants we use the following 4m equations: 

$$
f _ {i} (x _ {i}) = f (x _ {i}), i = 1, \dots , m, \text { and } f _ {m} (x _ {m + 1}) = f (x _ {m + 1}),\tag{8.18}
$$

$$
f _ {i - 1} (x _ {i}) = f _ {i} (x _ {i}), i = 2, \ldots , m,\tag{8.19}
$$

$$
f _ {i - 1} ^ {\prime} (x _ {i}) = f _ {i} ^ {\prime} (x _ {i}), i = 2, \ldots , m,\tag{8.20}
$$

$$
f _ {i - 1} ^ {\prime \prime} (x _ {i}) = f _ {i} ^ {\prime \prime} (x _ {i}), i = 2, \dots , m,\tag{8.21}
$$

$$
f _ {1} ^ {\prime \prime} (x _ {1}) = 0 \mathrm{and} f _ {m} ^ {\prime \prime} (x _ {m + 1}) = 0.\tag{8.22}
$$

The last condition leads to a so-called natural spline. 

We now formulate a quadratic programming problem with the objective of finding a risk-neutral probability density function (described by cubic splines) for future values of an underlying security that best fits the observed option prices on this security. 

We choose a security for consideration, say a stock or an index. We then fix an exercise date–this is future the date for which we will obtain a probability density function of the price of our security. Finally, we fix a range $[ a , b ]$ for possible terminal values of the price of the underlying security at the exercise date of the options and an interest rate r for the period between now and the exercise date. The inputs to our optimization problem are current market prices $C _ { K }$ of call options and $P _ { K }$ for put options on the chosen underlying security with strike price K and the chosen expiration date. This data is easily available from newspapers and online sources. Let and ${ \mathcal { P } } _ { : }$ , respectively, denote the set of strike prices K for which reliable market prices $C _ { K }$ and $P _ { K }$ are available. For example,  may denote the strike prices of call options that were traded on the day the problem is formulated. 

Next, we fix a super-structure for the spline approximation to the riskneutral density, meaning that we choose how many knots to use, where to place the knots and what kind of polynomial (quadratic, cubic, etc.) functions to use. For example, we may decide to use cubic splines and $m + 1$ equally spaced knots. The parameters of the polynomial functions that comprise the spline function will be the variables of the optimization problem we are formulating. For cubic splines with $m + 1$ knots, we will have 4m variables $( \alpha _ { i } , \beta _ { i } , \gamma _ { i } , \delta _ { i } )$ for $i = 1 , \ldots , m$ . Collectively, we will represent these variables with y. For all y chosen so that the corresponding polynomial functions $f _ { i }$ satisfy the equations (8.19)–(8.22) above, we will have a particular choice of a natural spline function defined on the interval $[ a , b ] ^ { 1 }$ . Let $p _ { y } ( \cdot )$ denote this function. Imposing the following additional restrictions we make sure that $p _ { y }$ is a probability density function: 

$$
p _ {y} (x) \geq 0, \forall x \in [ a, b ]\tag{8.23}
$$

$$
\int_ {a} ^ {b} p _ {y} (\omega) d \omega = 1.\tag{8.24}
$$

The constraint (8.24) is a linear constraint on the variables $( \alpha _ { i } , \beta _ { i } , \gamma _ { i } , \delta _ { i } )$ of the problem and can be enforced as follows: 

$$
\sum_ {s = 1} ^ {n _ {s}} \int_ {x _ {s}} ^ {x _ {s + 1}} f _ {s} (\omega) d \omega = 1.\tag{8.25}
$$

On the other hand, enforcing condition (8.23) is not straightforward as it requires the function to be nonnegative for all values of x in $[ a , b ]$ . Here, 

## 8.4. RECOVERING RISK-NEURAL PROBABILITIES FROM OPTIONS PRICES163

we relax condition (8.23), and require the cubic spline approximation to be nonnegative only at the knots: 

$$
p _ {y} (x _ {i}) \geq 0, i = 1, \ldots , m.\tag{8.26}
$$

While this relaxation simplifies the problem greatly, we cannot guarantee that the spline approximation we generate will be nonnegative in its domain. We will discuss in Chapter 10.3 a more sophisticated technique that rigorously enforces condition (8.23). 

Next, we define the discounted expected value of the terminal value of each option using $p _ { y }$ as the risk-neutral density function: 

$$
C _ {K} (y) := \frac {1}{1 + r} \int_ {a} ^ {b} (\omega - K) ^ {+} p _ {y} (\omega) d \omega ,\tag{8.27}
$$

$$
P _ {K} (y) := \frac {1}{1 + r} \int_ {a} ^ {b} (K - \omega) ^ {+} p _ {y} (\omega) d \omega .\tag{8.28}
$$

Then, $C _ { K } ( \boldsymbol { y } )$ is the theoretical option price if $p _ { y }$ is the true risk-neutral probability measure and 

$$
(C _ {K} - C _ {K} (y)) ^ {2}
$$

is the squared diference between the actual option price and this theoretical value. Now consider the aggregated error function for a given $y \colon$ 

$$
E (y) := \sum_ {K \in \mathcal {C}} (C _ {K} - C _ {K} (y)) ^ {2} + \sum_ {K \in \mathcal {P}} (P _ {K} - P _ {K} (y)) ^ {2}
$$

The objective now is to choose y such that conditions (8.19)–(8.22) of spline function description as well as (8.26) and (8.24) are satisfied and $E ( y )$ is minimized. This is essentially a constrained least squares problem. 

We choose the number of knots and their locations so that the knots form a superset of $\mathcal { C } \cup \mathcal { P }$ . Let $x _ { 0 } = a , x _ { 1 } , \ldots , x _ { m } = b$ denote the locations of the knots. Now, consider a call option with strike K and assume that K coincides with the location of the jth knot, $\mathrm { i . e . , } x _ { j } = K$ . Recall that y denotes collection of variables $( \alpha _ { i } , \beta _ { i } , \gamma _ { i } , \delta _ { i } )$ for $i = 1 , \ldots , m$ . Now, we can derive a formula for $C _ { K } ( \boldsymbol { y } )$ 

$$
\begin{array}{r c l} (1 + r) C _ {K} (y) & = & \int_ {a} ^ {b} S _ {y} (\omega) (\omega - K) ^ {+} d \omega \\ & = & \sum_ {i = 1} ^ {m} \int_ {x _ {i - 1}} ^ {x _ {i}} S _ {y} (\omega) (\omega - K) ^ {+} d \omega \\ & = & \sum_ {i = j + 1} ^ {m} \int_ {x _ {i - 1}} ^ {x _ {i}} S _ {y} (\omega) (\omega - K) d \omega \\ & = & \sum_ {i = j + 1} ^ {m} \int_ {x _ {i - 1}} ^ {x _ {i}} \left(\alpha_ {i} \omega^ {3} + \beta_ {i} \omega^ {2} + \gamma_ {i} \omega + \delta_ {i}\right) (\omega - K) d \omega . \end{array}
$$

It is easily seen that this expression for $C _ { K } ( \boldsymbol { y } )$ is a linear function of the components $( \alpha _ { i } , \beta _ { i } , \gamma _ { i } , \delta _ { i } )$ of the y variable. A similar formula can be derived for $P _ { K } ( y )$ . The reason for choosing the knots at the strike prices is the third equation in the sequence above—we can immediately ignore some of the terms in the summation and the $( \cdot ) ^ { + }$ function is linear (and not piecewise linear) in each integral. 

Now, it is clear that the problem of minimizing $E ( y )$ subject to spline function conditions, (8.26) and (8.24) is a quadratic optimization problem and can be solved using the techniques of the previous chapter. 

## 8.5 Additional Exercises

Exercise 8.15 Recall the mean-variance optimization problem we considered in Section 8.1: 

$$
\begin{array}{r c l} \min _ {x} & x ^ {T} \Sigma x \\ & \mu^ {T} x & \geq R \\ & A x & = b \\ & C x & \geq d. \end{array}\tag{8.29}
$$

Now, consider the problem of finding the feasible portfolio with smallest overall variance, without imposing any expected return constraint: 

$$
\begin{array}{r c l} \min _ {x} & x ^ {T} \Sigma x \\ & A x & = b \\ & C x & \geq d. \end{array}\tag{8.30}
$$

(i) Does the optimal solution to (8.30) give an eficient portfolio? Why? 

(ii) Let $x _ { R } , \ \lambda _ { R } \in \ I R , \ \gamma _ { E } \in \ I R ^ { m }$ , and $\gamma _ { I } ~ \in ~ \mathcal { R } ^ { p }$ satisfy the optimality conditions of (8.29) (see system (8.2)). $\mathrm { I f } ~ \lambda _ { R } = 0$ , show that $x _ { R }$ is an optimal solution to (8.30). (Hint: What are the optimality conditions for (8.30)? How are they related to (8.2)?) 

Exercise 8.16 Classification problems are among the important classes of problems in financial mathematics that can be solved using optimization models and techniques. In a classification problem we have a vector of “features” describing an entity and the objective is to analyze the features to determine which one of the two (or more) “classes” each entity belongs to. For example, the classes might be “growth stocks” and “value stocks”, and the entities (stocks) may be described by a feature vector that may contain elements such as stock price, price-earnings ratio, growth rate for the previous periods, growth estimates, etc. 

Mathematical approaches to classification often start with a “training” exercise. One is supplied with a list of entities, their feature vectors and the classes they belong to. From this information, one tries to extract a mathematical structure for the entity classes so that additional entities can be classified using this mathematical structure and their feature vectors. For two-class classification, a hyperplane is probably the simplest mathematical structure that can be used to “separate” the feature vectors of these two diferent classes. Of course, a hyperplane is often not suficient to separate two sets of vectors, but there are certain situations it may be suficient. 

Consider feature vectors $a _ { i } \in \mathbb { R } ^ { n }$ for $i = 1 , \ldots , k _ { 1 }$ corresponding to class 1, and vectors $b _ { i } \in \mathbb { R } ^ { n }$ for $i = 1 , \ldots , k _ { 2 }$ corresponding to class 2. If these two vector sets can be linearly separated, there exists a hyperplane $w ^ { T } x = \gamma$ with $w \in \mathbb { R } ^ { n } , \gamma \in \mathbb { R }$ such that 

$$
\begin{array}{r c l} w ^ {T} a _ {i} & \geq & \gamma , \text {for} i = 1, \ldots , k _ {1} \\ w ^ {T} b _ {i} & \leq & \gamma , \text {for} i = 1, \ldots , k _ {2}. \end{array}
$$

To have a “strict” separation, we often prefer to obtain w and $\gamma$ such that 

$$
\begin{array}{r c l} {w ^ {T} a _ {i}} & \geq & {\gamma + 1, \mathrm{for} i = 1, \ldots , k _ {1}} \\ {w ^ {T} b _ {i}} & \leq & {\gamma - 1, \mathrm{for} i = 1, \ldots , k _ {2}.} \end{array}
$$

In this manner, we find two parallel lines $( w ^ { T } x = \gamma + 1$ line and $w ^ { T } x = \gamma - 1 )$ that form the boundary of the class 1 and class 2 portion of the vector space. This type of separation is shown in Figure 8.5. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/0abcc1beabff193fd134fd58391829b7c7242a3da7a51ee1f51992bea4402348.jpg)



Figure 8.5: Linear separation of two classes of data points


There may be several such parallel lines that separate the two classes. Which one should one choose? $\mathrm { A }$ good criterion is to choose the lines that have the largest margin (distance between the lines). 

a) Consider the following quadratic problem: 

$$
\begin{array}{r l r l} \min _ {w, \gamma} & \| w \| _ {2} ^ {2} \\ & a _ {i} ^ {T} w & \geq & \gamma + 1, \text {for} i = 1, \ldots , k _ {1} \\ & b _ {i} ^ {T} w & \leq & \gamma - 1, \text {for} i = 1, \ldots , k _ {2}. \end{array}\tag{8.31}
$$

Show that the objective function of this problem is equivalent to maximizing the margin between the lines $w ^ { T } x = \gamma + 1$ and $w ^ { T } x = \gamma - 1$ b) The linear separation idea we presented above can be used even when the two vector sets $\left\{ { a } _ { i } \right\}$ and $\{ b _ { i } \}$ are not linearly separable. (Note that linearly inseparable sets will result in an infeasible problem in formulation (8.31).) This is achieved by introducing a nonnegative “violation” variable for each constraint of (8.31). Then, one has two objectives: to minimize the total of the violations of the constraints of (1) and to maximize the margin. Develop a quadratic programming model that combines these two objectives using an adjustable parameter that can be chosen in a way to put more weight on violations or margin, depending on one’s preference. 

Exercise 8.17 The classification problems we discussed in the previous exercise can also be formulated as linear programming problems, if one agrees to use 1-norm rather than 2-norm of w in the objective function. Recall that $\| w \| _ { 1 } = \textstyle \sum _ { i } | w _ { i } |$ . Show that if we replace $\lVert \boldsymbol { w } \rVert _ { 2 } ^ { 2 }$ with $\lVert \boldsymbol { w } \rVert _ { 1 }$ in the objective Pfunction of (1), we can write the resulting problem as an LP. Show also that, this new objective function is equivalent to maximizing the distance between $w ^ { T } x = \gamma + 1$ and $w ^ { T } x = \gamma - 1$ if one measures the distance using -norm $( \| g \| _ { \infty } = \operatorname* { m a x } _ { i } \left| g _ { i } \right| )$ 

## 8.6 Case Study

Investigate the performance of one of the variations on the classical Markowitz model proposed by Michaud, or Black-Litterman or Konno-Yamazaki. 

Possible suggestions: 

Choose 30 stocks and retrieve their historical returns over a meaningful horizon. 

Use the historical information to compute expected returns and the variance-covariance matrix for these stock returns. 

Set up the model and solve it with MATLAB or Excel’s Solver for diferent levels R of expected return. Allow for short sales and include no diversification constraints. 

Recompute these portfolios with no short sales and various diversification constraints. 

Compare portfolios constructed in period t (based on historical data up to period t) by observing their performance in period $t + 1$ , using the actual returns from period t + 1. 

Investigate how sensitive the optimal portfolios that you obtained are to small changes in the data. For example, how sensitive are they to a small change in the expected return of the assets? 

You currently own the following portfolio: $x _ { i } ^ { 0 } = 0 . 2 0$ for $i = 1 , \ldots , 5$ and $x _ { i } ^ { 0 } = 0$ for $i = 6 , \ldots , 3 0$ . Include turnover constraints to reoptimize the portfolio for a fixed level R of expected return and observe the dependency on $h ,$ , the total turnover allowed for reoptimization. 

You currently own the following portfolio: $x _ { i } ^ { 0 } = 0 . 2 0$ for $i = 1 , \ldots , 5$ and $x _ { i } ^ { 0 } = 0$ for $i = 6 , \ldots , 3 0$ . Reoptimize the portfolio considering transaction costs for buying and selling. Solve for a fixed level R of expected return and observe the dependency on transaction costs. 

## Chapter 9

# Conic Optimization Tools

## 9.1 Introduction

In this chapter and the next, we address conic optimization problems and their applications in finance. Conic optimization refers to the problem of minimizing or maximizing a linear function over a set defined by linear equalities and cone membership constraints. Cones are defined and discussed in Appendix B. While they are not as well known or as widely used as their close relatives linear and quadratic programming, conic optimization problems continue to grow in importance thanks to their wide applicability and the availability of powerful methods for their solution. 

We recall the definition of a standard form conic optimization problem that was provided in the Chapter 1: 

<sup>(</sup>CO<sup>)</sup> 

$$
\begin{array}{r l r} \min _ {x} & c ^ {T} x \\ & A x = b \\ & x \in C. \end{array}\tag{9.1}
$$

Here, C denotes a closed convex cone in a finite-dimensional vector space X. 

When $X = \varmathbb { R } ^ { n }$ and $C = \mathbb { R } _ { + } ^ { n }$ , this problem is the standard form linear programming problem. Therefore, conic optimization is a generalization of linear optimization. In fact, it is much more general than linear programming since we can use non-polyhedral (i.e., nonlinear) cones C in the description of these problems and formulate certain classes of nonlinear convex objective functions and nonlinear convex constraints. In particular, conic optimization provides a powerful and unifying framework for problems in linear programming (LP), second-order cone programming (SOCP), and semidefinite programming (SDP). We describe these two new and important classes of conic optimization problems in more detail: 

## 9.2 Second-order cone programming:

SOCPs involve the second-order cone which is defined by the property that for each of its members the first element is at least as large as the Euclidean norm of the remaining elements. This corresponds to the case where C is the second-order cone (also known as the quadratic cone, Lorenz cone, and the ice-cream cone): 

$$
C _ {q} := \{x = (x _ {1}, x _ {2}, \dots , x _ {n}) \in \mathbb {R} ^ {n}: x _ {1} \geq \| (x _ {2}, \dots , x _ {n}) \| \}.\tag{9.2}
$$

A portion of the second-order cone in 3 dimensions for $x _ { 1 } ~ \in ~ [ 0 , 1 ]$ is depicted in Figure 9.1. As seen from the figure, the second-order cone in three dimensions resembles an ice-cream cone that stretches to infinity. We observe that by “slicing” the second-order cone, i.e., by intersecting it with a hyperplane at diferent angles we can obtain spherical and ellipsoidal sets. Any convex quadratic constraint can be expressed using the second-order cone (or its rotations) and one or more hyperplanes. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/dd09cf9ffeb97f77014a6a34231b19f0466db02c1318da4828e8bc39eb351dc3.jpg)



Figure 9.1: The second-order cone


Exercise 9.1 Another important cone that appears in conic optimization formulations is the rotated quadratic cone defined as follows: 

$$
C _ {q} ^ {r} := \{(x _ {1}, x _ {2}, x _ {3}, \dots , x _ {n}): 2 x _ {1} x _ {2} \geq \sum_ {j = 3} ^ {n} x _ {j} ^ {2}, x _ {1}, x _ {2} \geq 0. \}.\tag{9.3}
$$

Show that $x = ( x _ { 1 } , x _ { 2 } , x _ { 3 } , \ldots , x _ { n } ) \in C _ { q } ^ { r }$ if and only if $y = ( y _ { 1 } , y _ { 2 } , y _ { 3 } , \dots , y _ { n } ) \in$ $C _ { q }$ where $\textstyle y _ { 1 } = { \frac { 1 } { \sqrt { 2 } } } ( x _ { 1 } + x _ { 2 } ) , y _ { 2 } = { \frac { 1 } { \sqrt { 2 } } } ( x _ { 1 } - x _ { 2 } )$ , and $y _ { j } = x _ { j } , j = 3 , \dotsc , n$ The vector y given here is obtained by rotating the vector x by 45 degrees in the plane defined by the first two coordinate axes. In other words, each element of the cone $C _ { q } ^ { r }$ can be mapped to a corresponding element of $C _ { q }$ through a 45 degree rotation (Why?). This is why the cone $C _ { q } ^ { r }$ is called the rotated quadratic cone. 

Exercise 9.2 Show that the problem 

$$
\begin{array}{l l} \min & x ^ {\frac {3}{2}} \\ \text {s.t.} & x \geq 0, x \in S \end{array}
$$

is equivalent to the following problem: 

$$
\begin{array}{c c} \min & t \\ \text {s.t.} & x \geq 0, x \in S \\ & x ^ {2} \leq t \cdot u \\ & u ^ {2} \leq x. \end{array}
$$

Express the second problem as an SOCP using $C _ { q } ^ { r }$ . 

Exercise 9.3 Consider the following optimization problem: 

$$
\begin{array}{r l r} \min & c _ {1} x _ {1} + c _ {2} x _ {2} + d _ {1} x _ {1} ^ {\frac {3}{2}} + d _ {2} x _ {2} ^ {\frac {3}{2}} \\ \text {s.t.} & a _ {1 1} x _ {1} + a _ {1 2} x _ {2} & = b _ {1}, \\ & x _ {1}, x _ {2} & \geq 0, \end{array}
$$

where $d _ { 1 } , d _ { 2 } > 0$ . The nonlinear objective function of this problem is a convex function. Write this problem as a conic optimization problem with a linear objective function and convex cone constraints. 

HINT: Use the previous exercise. 

A recent review of second-order cone programming models and methods is provided in [26]. One of the most common uses of second-order cone programs in financial applications is in the modeling and treatment of parameter uncertainties in optimization problems. After generating an appropriate description of the uncertainties, robust optimization models seek to find solutions to such problems that will perform well under many scenarios. As we will see in Chapter 19, ellipsoidal sets are among the most popular structures used for describing uncertainty in such problems and the close relationship between ellipsoidal sets and second-order cones make them particularly useful. We illustrate this approach in the following subsection. 

## 9.2.1 Ellipsoidal Uncertainty for Linear Constraints

Consider the following single-constraint linear program: 

$$
\begin{array}{r l r} \min & c ^ {T} x \\ \mathrm{s.t.} & a ^ {T} x + b & \geq 0. \end{array}
$$

We consider the setting where the objective function is certain but the constraint coeficients are uncertain. We assume that the constraint coeficients [a; b] belong to an ellipsoidal uncertainty set: 

$$
\mathcal {U} = \{[ a; b ] = [ a ^ {0}; b ^ {0} ] + \sum_ {j = 1} ^ {k} u _ {j} [ a ^ {j}; b ^ {j} ], \| u \| \leq 1 \}.
$$

Our objective is to find a solution that minimizes the objective function among the vectors that are feasible for all $[ a ; b ] \in \mathcal { U }$ . In other words, we want to solve 

$$
\begin{array}{r l r} \min & c ^ {T} x \\ \text {s.t.} & a ^ {T} x + b & \geq 0, \forall [ a; b ] \in \mathcal {U}. \end{array}
$$

For a fixed x the “robust” version of the constraint is satisfied if and only if 

$$
0 \leq \min _ {[ a; b ] \in \mathcal {U}} a ^ {T} x + b \equiv \min _ {u: \| u \| \leq 1} \alpha + u ^ {T} \beta ,\tag{9.4}
$$

where $\alpha = ( a ^ { 0 } ) ^ { T } x + b ^ { 0 }$ and $\beta = ( \beta _ { 1 } , \ldots , \beta _ { k } )$ with $\beta _ { j } = ( a ^ { j } ) ^ { T } x + b ^ { j }$ 

The second minimization problem in (9.4) is easy. Since α is constant, all we need to do is to minimize $u ^ { T } \beta$ subject to the constraint $\| u \| \leq 1$ . Recall that for the angle θ between vectors u and $\beta$ the following trigonometric equality holds: 

$$
\cos \theta = \frac {u ^ {T} \beta}{\| u \| \| \beta \|},
$$

or $u ^ { T } \beta = \| u \| \| \beta \|$ cos θ. Since $\| \beta \|$ is constant, this expression is minimized when $\lVert u \rVert = 1$ and cos $\theta = - 1$ . This means that u points in the opposite direction from $\beta ,$ , namely $- \beta$ . Normalizing to satisfy the bound constraint we obtain $\begin{array} { r } { u ^ { * } = - \frac { \beta } { \| \beta \| } } \end{array}$ as shown in Figure 9.2. Substituting this value we find 

$$
\min _ {[ a; b ] \in \mathcal {U}} a ^ {T} x + b = \alpha - \| \beta \| = (a ^ {0}) ^ {T} x + b ^ {0} - \sqrt {\sum_ {j = 1} ^ {k} ((a ^ {j}) ^ {T} x + b ^ {j}) ^ {2}},\tag{9.5}
$$

and we obtain the robust version of the inequality $a ^ { T } x + b \geq 0$ as 

$$
(a ^ {0}) ^ {T} x + b ^ {0} - \sqrt {\sum_ {j = 1} ^ {k} ((a ^ {j}) ^ {T} x + b ^ {j}) ^ {2}} \geq 0.\tag{9.6}
$$

It is now easy to observe that (9.6) can be written equivalently using the second-order cone: 

$$
\begin{array}{c} z _ {j} = (a ^ {j}) ^ {T} x + b ^ {j}, j = 0, \ldots k \\ (z _ {0}, z _ {1}, \ldots , z _ {k}) \in C _ {q} \end{array}
$$

The approach outlined above generalizes to multiple constraints as long as the uncertainties are constraint-wise, that is, if the uncertainty sets of parameters in diferent constraints are unrelated. Thus, robust optimization models for uncertain linear constraints with ellipsoidal uncertainty leads to SOCPs. The strategy outlined above is well-known and is used in, for example, [7]. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/82fb9bd7352dc0f7fee5c3d73a93629cc4a76c92da74a279f624e3129fba572c.jpg)



Figure 9.2: Minimization of a linear function over a circle


## 9.2.2 Conversion of quadratic constraints into second-order cone constraints

The second-order cone membership constraint $( x _ { 0 } , x _ { 1 } , \ldots , x _ { k } ) \in { \hat { C } } _ { q }$ can be written equivalently as the combination of a linear and a quadratic constraint: 

$$
x _ {0} \geq 0, x _ {0} ^ {2} - x _ {1} ^ {2} - \ldots - x _ {k} ^ {2} \geq 0.
$$

Conversely, any convex quadratic constraint of an optimization problem can be rewritten using second-order cone membership constraints. When we have access to a reliable solver for second-order cone optimization, it may be desirable to convert convex quadratic constraints to second-order cone constraints. Fortunately, a simple recipe is available for these conversions. 

Consider the following quadratic constraint: 

$$
x ^ {T} Q x + 2 p ^ {T} x + \gamma \leq 0.\tag{9.7}
$$

This is a convex constraint if the function on the left-hand-side is convex which is true if and only if Q is a positive semidefinite matrix. Let us assume $Q$ is positive definite for simplicity. In that case, there exists an invertible matrix, say R, satisfying $Q \stackrel { \bar { } } { = } R R ^ { \bar { T } }$ . For example, the Cholesky factor of $Q$ satisfies this property. Then, (9.7) can be written as 

$$
(R ^ {T} x) ^ {T} (R ^ {T} x) + 2 p ^ {T} x + \gamma \leq 0.\tag{9.8}
$$

Define $y = ( y _ { 1 } , \ldots , y _ { k } ) ^ { T } = R ^ { T } x + R ^ { - 1 } p .$ . Then, we have 

$$
y ^ {T} y = (R ^ {T} x) ^ {T} (R ^ {T} x) + 2 p ^ {T} x + p ^ {T} Q ^ {- 1} p.
$$

Thus, (9.8) is equivalent to 

$$
\exists y \mathrm{s.t.} y = R ^ {T} x + R ^ {- 1} p, y ^ {T} y \leq p ^ {T} Q ^ {- 1} p - \gamma .
$$

From this equivalence, we observe that the constraint (9.7) can be satisfied only if $p ^ { T } Q ^ { - 1 } p - \gamma \geq 0 \mathrm { ~ . }$ –we will assume that this is the case. 

Now, it is straightforward to note that (9.7) is equivalent to the following set of linear equations coupled with a second-order cone constraint: 

$$
\begin{array}{r c l} \left[ \begin{array}{c} y _ {1} \\ \vdots \\ y _ {k} \end{array} \right] & = & R ^ {T} x + R ^ {- 1} p, \\ y _ {0} & = & \sqrt {p ^ {T} Q ^ {- 1} p - \gamma}, \\ (y _ {0}, y _ {1}, \ldots , y _ {k}) \in C _ {q}. \end{array}
$$

Exercise 9.4 Rewrite the following convex quadratic constraint in “conic form”, i.e., as the intersection of linear equality constraints and a secondorder cone constraint: 

$$
1 0 x _ {1} ^ {2} + 2 x _ {1} x _ {2} + 5 x _ {2} ^ {2} + 4 x _ {1} + 6 x _ {2} + 1 \leq 0.
$$

Exercise 9.5 Discuss how the approach outlined in this section must be modified to address the case when $Q$ is positive semidefinite but not positive definite. In this case there still exists a matrix R satisfying $Q = R R ^ { T }$ . But R is no longer invertible and we can no longer define the vector y as above. 

## 9.3 Semidefinite programming:

In SDPs, the set of variables are represented by a symmetric matrix which is required to be in the cone of positive semidefinite matrices in addition to satisfying a system of linear equations. We say that a matrix $M \in \pi ^ { n \times n }$ is positive semidefinite if $y ^ { T } M y \ge 0$ for all $y \in \mathbb { R } ^ { n }$ . When M is symmetric, this is equivalent to M having eigenvalues that are all nonnegative. A stronger condition is positive definiteness. M is positive definite if $y ^ { T } M y > 0$ for all $y \in B ^ { n }$ with the exception of $y = 0$ . For symmetric M, positive definiteness is equivalent to the positivity of all of its eigenvalues. 

Since multiplication by a positive number preserves the positive semidefiniteness property, the set of positive semidefinite matrices is a cone. In fact, it is a convex cone. The cone of positive semidefinite matrices of a fixed dimension $\left( \operatorname { s a y } n \right)$ is defined as follows: 

$$
C _ {s} ^ {n} := \left\{X = \left[ \begin{array}{c c c} x _ {1 1} & \dots & x _ {1 n} \\ \vdots & \ddots & \vdots \\ x _ {n 1} & \dots & x _ {n n} \end{array} \right] \in I R ^ {n \times n}: X \succeq 0 \right\}.\tag{9.9}
$$

Above, the notation $X \succeq 0$ means that X is a symmetric positive semidefinite matrix. We provide a depiction of the cone of positive semidefinite 

## 9.3. SEMIDEFINITE PROGRAMMING:

matrices of dimension 2 in Figure 9.3. The diagonal elements $X _ { 1 1 }$ and $X _ { 2 2 }$ of a 2-dimensional symmetric matrix are shown on the horizontal axes while the of-diagonal element $X _ { 1 2 } ~ = ~ X _ { 2 1 }$ is on the vertical axis. Symmetric two-dimensional matrices whose elements lie inside the shaded region are positive semidefinite matrices. As the nonnegative orthant and the secondorder cone, the cone of positive semidefinite matrices has a point or a corner at the origin. Also note the convexity of the cone and the nonlinearity of its boundary. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/12bc0983d9d9e5d4b8a6e2524eb45545aeb49b7f3e9851cbcb60cd3045a03f0a.jpg)



Figure 9.3: The cone of positive semidefinite matrices


Semidefinite programming problems arise in a variety of disciplines. The recent review by Todd provides an excellent introduction to their solution methods and the rich set of applications [70]. One of the common occurrences of semidefiniteness constraints results from the so-called S-procedure, which is a generalization of the well-known S-lemma [58]: 

Lemma 9.1 Let $F _ { i } ( x ) = x ^ { T } A _ { i } x + 2 + b _ { i } ^ { T } x + c _ { i } , i = 0 , 1 , \dots , p$ be quadratic functions of $x \in \mathbb { R } ^ { n }$ . Then, 

$$
F _ {i} (x) \geq 0, i = 1, \dots , p \Rightarrow F _ {0} (x) \geq 0
$$

$i f$ there exist $\lambda _ { i } \geq 0$ such that 

$$
\left[ \begin{array}{c c} A _ {0} & b _ {0} \\ b _ {0} ^ {T} & c _ {0} \end{array} \right] - \sum_ {i = 1} ^ {p} \lambda_ {i} \left[ \begin{array}{c c} A _ {i} & b _ {i} \\ b _ {i} ^ {T} & c _ {i} \end{array} \right] \succeq 0.
$$

$I f p = 1$ , converse also holds as long as $\exists x _ { 0 }$ s.t. $F _ { 1 } ( x _ { 0 } ) > 0$ 

The S-procedure provides a suficient condition for the implication of a quadratic inequality by other quadratic inequalities. Furthermore, this condition is also a necessary condition in certain special cases. This equivalence can be exploited in robust modeling of quadratic constraints as we illustrate next. 

## 9.3.1 Ellipsoidal Uncertainty for Quadratic Constraints

This time we consider a convex-quadratically constrained problem where the objective function is certain but the constraint coeficients are uncertain: 

$$
\begin{array}{l l} \min & c ^ {T} x \\ \text {s.t.} & - x ^ {T} (A ^ {T} A) x + 2 b ^ {T} x + \gamma \geq 0, \forall [ A; b; \gamma ] \in \mathcal {U}, \end{array}
$$

where $A \in I R ^ { m \times n } , b \in I R ^ { n }$ and $\gamma$ is a scalar. We again consider the case where the uncertainty set is ellipsoidal: 

$$
\mathcal {U} = \{[ A; b; \gamma ] = [ A ^ {0}; b ^ {0}; \gamma^ {0} ] + \sum_ {j = 1} ^ {k} u _ {j} [ A ^ {j}; b ^ {j}; \gamma^ {j} ], \| u \| \leq 1 \}.
$$

To reformulate the robust version of this problem we use the S-procedure described above. The robust version of our convex quadratic inequality can be written as 

$$
[ A; b; \gamma ] \in \mathcal {U} \Rightarrow - x ^ {T} (A ^ {T} A) x + 2 b ^ {T} x + \gamma \geq 0.\tag{9.10}
$$

This is equivalent to the following expression: 

$$
\| u \| \leq 1 \Rightarrow - x ^ {T} (A ^ {0} + \sum_ {j = 1} ^ {k} A ^ {j} u _ {j}) (A ^ {0} + \sum_ {j = 1} ^ {k} A ^ {j} u _ {j}) ^ {T} x + 2 (b ^ {0} + \sum_ {j = 1} ^ {k} b ^ {j} u _ {j}) ^ {T} x + (\gamma^ {0} + \sum_ {j = 1} ^ {k} \gamma^ {j} u _ {j}) \geq 0.\tag{9.11}
$$

Defining $A ( x ) : I R ^ { n }  I R ^ { m \times k }$ as 

$$
A (x) = \left[ A ^ {1} x | A ^ {2} x | \dots | A ^ {k} x \right],
$$

$b ( x ) : I R ^ { n } \to I R ^ { k }$ as 

$$
b (x) = \left[ x ^ {T} b ^ {1} x ^ {T} b ^ {2} \dots x ^ {T} b ^ {k} \right] ^ {T} + \frac {1}{2} \left[ \gamma^ {1} \gamma^ {2} \dots \gamma^ {k} \right] ^ {T} - A (x) ^ {T} A ^ {0} x
$$

and 

$$
\gamma (x) = \gamma^ {0} + 2 (b ^ {0}) ^ {T} x - x ^ {T} (A ^ {0}) ^ {T} A ^ {0} x
$$

and rewriting $\| u \| \leq 1 { \mathrm { ~ a s ~ } } - u ^ { T } I u + 1 \geq 0$ we can simplify (9.11) as follows: 

$$
- u ^ {T} I u + 1 \geq 0 \Rightarrow - u ^ {T} A (x) ^ {T} A (x) u + 2 b (x) ^ {T} u + \gamma (x) \geq 0.\tag{9.12}
$$

Now we can apply Lemma 9.1 with $p = 1 , A _ { 1 } = I , b _ { 1 } = 0 , c _ { 1 } = 1$ and $A _ { 0 } = A ( x ) ^ { T } A ( x ) , \ : b _ { 0 } = b ( x )$ and $c _ { 0 } = \gamma ( x )$ . Thus, the robust constraint (9.12) can be written as 

$$
\exists \lambda \geq 0 \text {s.t.} \left[ \begin{array}{c c} \gamma (x) - \lambda & b (x) ^ {T} \\ b (x) & A (x) ^ {T} A (x) - \lambda I \end{array} \right] \succeq 0.\tag{9.13}
$$

## 9.4. ALGORITHMS AND SOFTWARE

Thus, we transformed the robust version of the quadratic constraint into a semidefiniteness constraint for a matrix that depends on the variables x and also a new variable λ. However, because of the term $A ( x ) ^ { T } A ( x )$ , this results in a nonlinear semidefinite optimization problem, which is dificult and beyond the immediate territory of most conic optimization algorithms. Fortunately, however, the semidefiniteness condition above is equivalent to the following semidefiniteness condition: 

$$
\exists \lambda \geq 0 \text {s.t.} \left[ \begin{array}{c c c} \gamma^ {\prime} (x) - \lambda & b ^ {\prime} (x) ^ {T} & (A ^ {0} x) ^ {T} \\ b ^ {\prime} (x) & \lambda I & A (x) ^ {T} \\ A ^ {0} x & A (x) & I \end{array} \right] \succeq 0\tag{9.14}
$$

where 

$$
b ^ {\prime} (x) = \left[ x ^ {T} b ^ {1} x ^ {T} b ^ {2} \dots x ^ {T} b ^ {k} \right] ^ {T} + \frac {1}{2} \left[ \gamma^ {1} \gamma^ {2} \dots \gamma^ {k} \right] ^ {T}
$$

and 

$$
\gamma^ {\prime} (x) = \gamma^ {0} + 2 (b ^ {0}) ^ {T} x.
$$

Since all of $A ( x ) , b ^ { \prime } ( x )$ and $\gamma ^ { \prime } ( x )$ are linear in $x ,$ we obtain a linear semidefinite optimization problem from the reformulation of the robust quadratic constraint via the S-procedure. For details of this technique and many other useful results for reformulation of robust constraints, we refer the reader to [7]. 

Exercise 9.6 Verify that (9.11) is equivalent to (9.10). 

Exercise 9.7 Verify that (9.13) and (9.14) are equivalent. 

## 9.4 Algorithms and Software

Since most conic optimization problem classes are special cases of nonlinear programming problems, they can be solved using general nonlinear optimization strategies we discussed in Chapter 5. As in linear and quadratic programming problems, the special structure of conic optimization problems allows the use of specialized and more eficient methods that take advantage of this structure. In particular, many conic optimization problems can be solved eficiently using the generalizations of sophisticated interior-point algorithms for linear and quadratic programming problems. These generalizations of interior-point methods are based on the ground-breaking work of Nesterov and Nemirovski [54] as well as the theoretical and computational advances that followed their work. 

During the past decade, an intense theoretical and algorithmic study of conic optimization problems produced a number of increasingly sophisticated software products for several problem classes including SeDuMi [69] and SDPT3 [72] which are freely available. Interested readers can obtain additional information on such software by following the software link of the following page dedicated to semidefinite programming and maintained by Christoph Helmberg: 

http://www-user.tu-chemnitz.de/~helmberg/semidef.html 

There are also commercial software products that address conic optimization problems. For example, MOSEK (www.mosek.com) provides a powerful engine for second-order and linear cone optimization. AXIOMA’s (www.axiomainc.com) portfolio optimization software employs a conic optimization solver that handles convex quadratic constraints as well as ellipsoidal uncertainties among other things. 

## Chapter 10

# Conic Optimization Models in Finance

Conic optimization problems are encountered in a wide array of fields including truss design, control and system theory, statistics, eigenvalue optimization, and, antenna array weight design. Robust optimization formulations of many convex programming problems also lead to conic optimization problems, see, e.g. [7, 8]. Furthermore, conic optimization problems arise as relaxations of hard combinatorial optimization problems such as the maxcut problem. Finally, some of the most interesting applications of conic optimization are encountered in financial mathematics and we will address several examples in this chapter. 

## 10.1 Tracking Error and Volatility Constraints

In most quantitative asset management environments, portfolios are chosen with respect to a carefully selected benchmark. Typically, the benchmark is a market index, reflecting a particular market (e.g., domestic or foreign), or a segment of the market (e.g., large cap growth) the investor wants to invest in. Then, the portfolio manager’s problem is to determine an index tracking portfolio with certain desirable characteristics. An index tracking portfolio intends to track the movements of the underlying index closely with the ultimate goal of adding value by beating the index. Since this goal requires departures from the underlying index, one needs to balance the expected excess return (i.e., expected return in excess of the benchmark return) with the variance of the excess returns. 

The tracking error for a given portfolio with a given benchmark refers to the diference between the returns of the portfolio and the benchmark. If the return vector is given by $^ { r , }$ the weight vector for the benchmark portfolio is denoted by $x _ { B M }$ , and the weight vector for the portfolio is $x ,$ then this diference is given as: 

$$
r ^ {T} x - r ^ {T} x _ {B M} = r ^ {T} (x - x _ {B M}).
$$

While some references in the literature define tracking error as this quantity, we will prefer to refer to it as the excess return. Using the common conventions, we define tracking error as a measure of variability of excess returns. The ex ante, or predicted tracking error of the portfolio (with respect to the risk model given by Σ) is defined as follows: 

$$
{ T E ( x ) } { : = } { \sqrt { ( x - x _ { B M } ) ^ { T } \Sigma ( x - x _ { B M } ) } . }\tag{10.1}
$$

In contrast, the ex-post, or realized, tracking error is a statistical dispersion measure for the realized excess returns, typically the standard deviation of regularly (e.g., daily) observed excess returns. 

In benchmark relative portfolio optimization, we solve mean-variance optimization problems where expected absolute return and standard deviation of returns are replaced by expected excess return and the predicted tracking error. For example, variance constrained MVO problem (8.3) is replaced by the following formulation: 

$$
\begin{array}{r l r} \max _ {x} & \mu^ {T} (x - x _ {B M}) \\ & (x - x _ {B M}) ^ {T} \Sigma (x - x _ {B M}) & \leq \mathrm{TE} ^ {2} \\ & A x = b \\ & C x \geq d, \end{array}\tag{10.2}
$$

where ${ \boldsymbol x } = ( x _ { 1 } , \dots , x _ { n } )$ is the variable vector whose components $x _ { i }$ denote the proportion of the total funds invested in security i, µ and Σ are the expected return vector and the covariance matrix, and $A , b , C ,$ and d are the coeficients of the linear equality and inequality constraints that define feasible portfolios. The objective is to maximize the expected excess return while limiting the portfolio tracking error to a predefined value of TE. 

Unlike the formulations (8.1) and (8.4) that have only linear constraints, this formulation is not in standard quadratic programming form and therefore can not be solved directly using eficient and widely available QP algorithms. The reason for this is the existence of a nonlinear constraint, namely the constraint limiting the portfolio tracking error. So, if all MVO formulations are essentially equivalent as we argued before, why would anyone use the “harder” formulations with the risk constraint? 

As Jorion observes [40], ex post returns are “enormously noisy measures of expected returns” and therefore investors may not be able or willing to determine minimum acceptable expected return levels, or risk-aversion constants–inputs required for problems (8.1) and (8.4)–with confidence. Jorion [40] notes that “it is much easier to constrain the risk profile, either before or after the fact–which is no doubt why investors give managers tracking error constraints.” 

Fortunately, the tracking error constraint is a convex quadratic constraint which means that we can rewrite this constraint in conic form as we saw in the previous chapter. If the remaining constraints are linear as in (10.2), the resulting problem is a second-order cone optimization problem that can be solved with specialized methods. 

Furthermore, in situations where the control of multiple measures of risk is desired the conic reformulations can become very useful. In [40], Jorion observes that MVO with only a tracking error constraint may lead to portfolios with high overall variance. He considers a model where a variance constraint as well as a tracking error constraint is imposed for optimizing the portfolio. When no additional constraints are present, Jorion is able to solve the resulting problem since analytic solutions are available. His approach, however, does not generalize to portfolio selection problems with additional constraints such as no-shorting limitations, or exposure limitations to such factors as size, beta, sectors or industries. The strength of conic optimization models, and in this particular case, of second-order cone programming approaches is that the algorithms developed for them will work for any combination of linear equality, linear inequality, and convex quadratic inequality constraints. Consider, for example, the following generalization of the models in [40]: 

$$
\begin{array}{r l r} \max _ {x} & \mu^ {T} x \\ & \sqrt {x ^ {T} \Sigma x} & \leq \sigma \\ & \sqrt {(x - x _ {B M}) ^ {T} \Sigma (x - x _ {B M})} & \leq T E \\ & A x & = b \\ & C x & \geq d. \end{array}\tag{10.3}
$$

This problem can be rewritten as a second-order cone programming problem using the conversions outlined in Section 9.2.2. Since Σ is positive semidefinite, there exists a matrix R such that $\Sigma = R R ^ { T }$ . Defining 

$$
\begin{array}{r c l} {y} & = & {R ^ {T} x} \\ {z} & = & {R ^ {T} x - R ^ {T} x _ {B M}} \end{array}
$$

we see that the first two constraints of (10.3) are equivalent to $( y _ { 0 } , y ) \in C _ { q } ,$ $( z _ { 0 } , z ) \in C _ { q }$ with $y _ { 0 } = \sigma$ and $z _ { 0 } = T E$ . Thus, (10.3) is equivalent to the following second-order cone program: 

$$
\begin{array}{r l r} \max _ {x} & \mu^ {T} x \\ & A x & = b \\ & C x & \geq d \\ & R ^ {T} x - y & = 0 \\ & R ^ {T} x - z & = R ^ {T} x _ {B M} \\ & y _ {0} & = \sigma \\ & z _ {0} & = T E \\ & (y _ {0}, y) \in C _ {q}, (z _ {0}, z) \in C _ {q} \end{array}\tag{10.4}
$$

Exercise 10.1 Second-order cone formulations can also be used for modeling a tracking error constraint under diferent risk models. For example, if we had k alternative estimates of the covariance matrix denoted by $\Sigma _ { 1 } , \dots , \Sigma _ { k }$ and wanted to limit the tracking error with respect to each estimate we would have a sequence of constraints of the form 

$$
\sqrt {(x - x _ {B M}) ^ {T} \Sigma_ {i} (x - x _ {B M})} \leq T E _ {i}, i = 1, \ldots , k.
$$

Show how these constraints can be converted to second-order cone constraints. 

Exercise 10.2 Using historical returns of the stocks in the DJIA, estimate their mean $\mu _ { i }$ and covariance matrix. Let R be the median of the $\mu _ { i } \mathrm { s }$ . Find an expected return maximizing long-only portfolio of Dow Jones constituents that has (i) a tracking error of 10% or less, and (ii) a volatility of 20% or less. 

## 10.2 Approximating Covariance Matrices

The covariance matrix of a vector of random variables is one of the most important and widely used statistical descriptors of the joint behavior of these variables. Covariance matrices are encountered frequently is financial mathematics, for example, in mean-variance optimization, in forecasting, in time-series modeling, etc. 

Often, true values of covariance matrices are not observable and one must rely on estimates. Here, we do not address the problem of estimating covariance matrices and refer the reader, e.g., to Chapter 16 in [48]. Rather, we consider the case where a covariance matrix estimate is already provided and one is interested in determining a modification of this estimate that satisfies some desirable properties. Typically, one is interested finding the smallest distortion of the original estimate that achieves these desired properties. 

Symmetry and positive semidefiniteness are structural properties shared by all “proper” covariance matrices. A correlation matrix satisfies the additional property that its diagonal consists of all ones. Recall that a symmetric and positive semidefinite matrix $M \in \pi ^ { n \times n }$ satisfies the property that 

$$
x ^ {T} M x \geq 0, \forall x \in \mathbb {R} ^ {n}.
$$

This property is equivalently characterized by the nonnegativity of the eigenvalues of the matrix M. 

In some cases, for example when the estimation of the covariance matrix is performed entry-by-entry, the resulting estimate may not be a positive semidefinite matrix, that is it may have negative eigenvalues. Using such an estimate would suggest that some linear combinations of the underlying random variables have negative variance and possibly result in disastrous results in mean-variance optimization. Therefore, it is important to correct such estimates before they are used in any financial decisions. 

Even when the initial estimate is symmetric and positive semidefinite, it may be desirable to modify this estimate without compromising these properties. For examples, if some pairwise correlations or covariances appear counter-intuitive to a financial analyst’s trained eye, the analyst may want to modify such entries in the matrix. All these variations of the problem of obtaining a desirable modification of an initial covariance matrix estimate can be formulated within the powerful framework of semidefinite optimization and can be solved with standard software available for such problems. 

We start the mathematical treatment of the problem by assuming that we have an estimate $\hat { \Sigma } \in S ^ { n }$ of a covariance matrix and that $\hat { \Sigma }$ is not necessarily positive semidefinite. Here, $S ^ { n }$ denotes the space of symmetric $n \times n$ matrices. An important question in this scenario is the following: What is the “closest” positive semidefinite matrix to $\hat { \Sigma } ?$ For concreteness, we use the Frobenius norm of the distortion matrix as a measure of closeness: 

$$
d _ {F} (\Sigma , \hat {\Sigma}) := \sqrt {\sum_ {i , j} (\Sigma_ {i j} - \hat {\Sigma} _ {i j}) ^ {2}}.
$$

Now we can state the closest covariance matrix problem as follows: Given $\hat { \Sigma } \in S ^ { n }$ , 

$$
\begin{array}{r l} \min _ {\Sigma} & d _ {F} (\Sigma , \hat {\Sigma}) \\ & \Sigma \in C _ {s} ^ {n} \end{array}\tag{10.5}
$$

where $C _ { s } ^ { n }$ is the cone of $n \times n$ symmetric and positive semidefinite matrices as defined in (9.9). Notice that the decision variable in this problem is represented as a matrix rather than a vector as in all previous optimization formulations we considered. 

Furthermore, introducing a dummy variable $t ,$ we can rewrite the last problem above as: 

$$
\begin{array}{r c l} \min & t \\ & d _ {F} (\Sigma , \hat {\Sigma}) & \leq t \\ & \Sigma \in C _ {s} ^ {n}. \end{array}
$$

It is easy to see that the inequality $d _ { F } ( \Sigma , \hat { \Sigma } ) \leq t$ can be written as a secondorder cone constraint, and therefore, the formulation above can be transformed into a conic optimization problem. 

Variations of this formulation can be obtained by introducing additional linear constraints. As an example, consider a subset $E$ of all $( i , j )$ covariance pairs and lower/upper limits $l _ { i j } , u _ { i j } \forall ( i , j ) \in E$ that we wish to impose on these entries. Then, we would need to solve the following problem: 

min 

$$
\begin{array}{r c l r c l} & & d _ {F} (\Sigma , \hat {\Sigma}) \\ l _ {i j} & \leq & \Sigma_ {i j} & \leq & u _ {i j}, \forall (i, j) \in E \\ & & \Sigma & \in & C _ {s} ^ {n}. \end{array}\tag{10.6}
$$

When $E$ consists of all the diagonal $( i , i )$ elements and $l _ { i i } = u _ { i i } = 1$ , i, we get the correlation matrix version of the original problem. For example, three-dimensional correlation matrices have the following form: 

$$
\Sigma = \left[ \begin{array}{c c c} 1 & x & y \\ x & 1 & z \\ y & z & 1 \end{array} \right], \Sigma \in C _ {s} ^ {3}.
$$

The feasible set for this instance is shown in Figure 10.2. 

Example 10.1 We consider the following estimate ofthe correlation matrix $o f \ 4$ securities: 

$$
\hat {\Sigma} = \left[ \begin{array}{l l l l} 1. 0 & 0. 8 & 0. 5 & 0. 2 \\ 0. 8 & 1. 0 & 0. 9 & 0. 1 \\ 0. 5 & 0. 9 & 1. 0 & 0. 7 \\ 0. 2 & 0. 1 & 0. 7 & 1. 0 \end{array} \right].\tag{10.7}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/5d987e74278d0a45449c7f31123d7872e6cb952588ec727ac02b91225d9f163b.jpg)



Figure 10.1: The feasible set of the nearest correlation matrix problem in 3-dimensions


This, in $f a c t ,$ is not a valid correlation matrix; its smallest eigenvalue is negative: $\lambda _ { \operatorname* { m i n } } = - 0 . 1 3 3 7$ . Note, for example, the high correlations between assets 1 and 2 as well as assets 2 and 3. This suggests that 1 and 3 should be highly correlated as well, but they are not. Which entry should one adjust to find a valid correlation matrix? 

We can approach this problem using formulation $( 1 0 . 6 )$ with E consisting of all the diagonal (i, i) elements and $l _ { i i } = u _ { i i } = 1 , \forall i$ . Solving the resulting problem, for example, using SDPT3 $\left[ { \widetilde { 7 } } { \overset { \partial } { \partial } } \right]$ , we obtain (approximately) the following nearest correction to $\hat { \Sigma }$ 4 

$$
\Sigma = \left[ \begin{array}{c c c c} 1. 0 0 & 0. 7 6 & 0. 5 3 & 0. 1 8 \\ 0. 7 6 & 1. 0 0 & 0. 8 2 & 0. 1 5 \\ 0. 5 3 & 0. 8 2 & 1. 0 0 & 0. 6 5 \\ 0. 1 8 & 0. 1 5 & 0. 6 5 & 1. 0 0 \end{array} \right].
$$

Exercise 10.3 Use a semidefinite optimization software package to verify that Σ given above is the solution to (10.5) when $\hat { \Sigma }$ is given by (10.7). 

Exercise 10.4 Resolve the problem above, this time imposing the constraint that $\Sigma _ { 2 3 } = \Sigma _ { 3 2 } \geq 0 . 8 5$ 

One can consider several variations on the “plain vanilla” version of the nearest correlation matrix problem. For example, if we would rather keep some of the entries of the matrix $\hat { \Sigma }$ constant, we can expand the set E to contain those elements with matching lower and upper bounds. Another possibility is to weight the changes in diferent entries, for example if estimates of some entries are more trust-worthy than others. 

## 10.3. RECOVERING RISK-NEURAL PROBABILITIES FROM OPTIONS PRICES185

Another important variation of the original problem is obtained by placing lower limits on the smallest eigenvalue of the correlation matrix. Even when we have a valid (positive semidefinite) correlation matrix estimate, having small eigenvalues in the matrix can be undesirable as they lead to unstable portfolios. Indeed, the valid correlation matrix we obtained above has a positive but very small eigenvalue, which would in fact be exactly zero in exact arithmetic. Hauser and Zuev consider models where minimum eigenvalue of the covariance matrix is maximized and use the matrices in a robust optimization setting [37]. 

Exercise 10.5 We want to find the nearest symmetric matrix to $\hat { \Sigma }$ in (10.7) whose smallest eigenvalue is at least 0.25. Express this problem as a semidefinite optimization problem. Solve it using an SDP software package. 

All these variations are easily handled using semidefinite programming formulations and solved using semidefinite optimization software. As such, semidefinite optimization presents a new tool for asset managers that was not previously available at this level of sophistication and flexibility. While these tools are not yet available as commercial software packages, many academic products are freely available; see the link $\mathrm { g i }$ ven in Section 9.4. 

## 10.3 Recovering Risk-Neural Probabilities from Options Prices

In this section, we revisit our study of the risk-neutral density estimation problem in Section 8.4. Recall that the objective of this problem is to estimate an implied risk-neutral density function for the future price of an underlying security using the prices of options written on that security. Representing the density function using cubic splines to ensure its smoothness, and using a least-squares type objective function for the fit of the estimate with the observed option prices, we formulated an optimization problem in Section 8.4. 

One issue that we left open in Section 8.4 is the rigorous enforcement of the nonnegativity of the risk-neutral density estimate. While we heuristically handled this issue by enforcing the nonnegativity of the cubic splines at the knots, it is clear that a cubic function that is nonnegative at the endpoints of an interval can very well become negative in between and therefore, the heuristic technique of Section 8.4 may be inadequate. Here we discuss an alternative formulation that is based on necessary and suficient conditions for ensuring the nonnegativity of a single variable polynomial in intervals. This characterization is due to Bertsimas and Popescu [10] and is stated in the next proposition. 

Proposition 10.1 (Proposition 1 (d),[10]) The polynomial $\begin{array} { r } { g ( x ) = \sum _ { r = 0 } ^ { k } y _ { r } x ^ { r } } \end{array}$ satisfies $g ( x ) \geq 0$ for all $x \in [ a , b ]$ Pif and only if there exists a positive 

semidefinite matrix $X = [ x _ { i j } ] _ { i , j = 0 , \dots , k }$ such that 

$$
\sum_ {i, j: i + j = 2 \ell - 1} x _ {i j} = 0, \ell = 1, \ldots , k,\tag{10.8}
$$

$$
\sum_ {i, j: i + j = 2 \ell} x _ {i j} = \sum_ {m = 0} ^ {\ell} \sum_ {r = m} ^ {k + m - \ell} y _ {r} \left(r m\right) \binom{k - r}{\ell - m} a ^ {r - m} b ^ {m},\tag{10.9}
$$

$$
\ell = 0, \dots , k,\tag{10.10}
$$

$$
X \succeq 0.\tag{10.11}
$$

In the statement of the proposition above, the notation $\left( \begin{array} { c } { r } \\ { m } \end{array} \right)$ stands for $\frac { r ! } { m ! ( r - m ) ! }$ and $X \succeq 0$ indicates that the matrix X is symmetric and positive semidefinite. For the cubic polynomials $f _ { s } ( x ) = \alpha _ { s } x ^ { 3 } + \beta _ { s } x ^ { 2 } + \gamma _ { s } x + \delta _ { s }$ that are used in the formulation of Section 8.4, the result can be simplified as follows: 

Corollary 10.1 The polynomial $f _ { s } ( x ) = \alpha _ { s } x ^ { 3 } + \beta _ { s } x ^ { 2 } + \gamma _ { s } x + \delta _ { s }$ satisfies $f _ { s } ( x ) \geq 0$ for all $x \in [ x _ { s } , x _ { s + 1 } ]$ if and only if there exists $a \mathrm { ~ 4 ~ } \times \mathrm { ~ 4 ~ }$ matrix $X ^ { s } = [ x _ { i j } ^ { s } ] _ { i , j = 0 , \ldots , 3 }$ such that 

$$
\begin{array}{r c l} x _ {i j} ^ {s} & = & 0, \text {if} i + j \text {is 1 or 5}, \\ x _ {0 3} ^ {s} + x _ {1 2} ^ {s} + x _ {2 1} ^ {s} + x _ {3 0} ^ {s} & = & 0, \\ x _ {0 0} ^ {s} & = & \alpha_ {s} x _ {s} ^ {3} + \beta_ {s} x _ {s} ^ {2} + \gamma_ {s} x _ {s} + \delta_ {s}, \\ x _ {0 2} ^ {s} + x _ {1 1} ^ {s} + x _ {2 0} ^ {s} & = & 3 \alpha_ {s} x _ {s} ^ {2} x _ {s + 1} + \beta_ {s} (2 x _ {s} x _ {s + 1} + x _ {s} ^ {2}) \\ & & + \gamma_ {s} (x _ {s + 1} + 2 x _ {s}) + 3 \delta_ {s}, \\ x _ {1 3} ^ {s} + x _ {2 2} ^ {s} + x _ {3 1} ^ {s} & = & 3 \alpha_ {s} x _ {s} x _ {s + 1} ^ {2} + \beta_ {s} (2 x _ {s} x _ {s + 1} + x _ {s + 1} ^ {2}) \\ & & + \gamma_ {s} (x _ {s} + 2 x _ {s + 1}) + 3 \delta_ {s}, \\ x _ {3 3} ^ {s} & = & \alpha_ {s} x _ {s + 1} ^ {3} + \beta_ {s} x _ {s + 1} ^ {2} + \gamma_ {s} x _ {s + 1} + \delta_ {s}, \\ X ^ {s} & \succeq & 0. \end{array}\tag{10.12}
$$

Observe that the positive semidefiniteness of the matrix $X ^ { s }$ implies that the first diagonal entry $x _ { 0 0 } ^ { s }$ is nonnegative, which corresponds to our earlier requirement $f _ { s } ( x _ { s } ) \geq 0$ . In light of Corollary 10.1, we see that introducing the additional variables $X ^ { s }$ and the constraints (10.12), for $s = 1 , \ldots , n _ { s } ,$ 2 into the earlier quadratic programming problem in Section $8 . 4 ,$ , we obtain a new optimization problem which necessarily leads to a risk-neutral probability distribution function that is nonnegative in its entire domain. The new formulation has the following form: 

$$
\min _ {y, X ^ {1}, \dots , X ^ {n _ {s}}} E (y) \text {s.t.} (8. 1 9), (8. 2 0), (8. 2 1), (8. 2 2), (8. 2 5), [ (1 0. 1 2), s = 1, \dots , n _ {s} ].\tag{10.13}
$$

All constraints in (10.13), with the exception of the positive semidefiniteness constraints $X ^ { s } \succeq 0 , s = 1 , \dots , n _ { s }$ , are linear in the optimization variables $( \alpha _ { s } , \beta _ { s } , \gamma _ { s } , \delta _ { s } )$ and $X ^ { s } , s = 1 , \ldots , n _ { s }$ . The positive semidefiniteness constraints are convex constraints and thus the resulting problem can be reformulated as a convex semidefinite programming problem with a quadratic objective function. 

For appropriate choices of the vectors $c , f _ { i } , g _ { k } ^ { s }$ , and matrices Q and $H _ { k } ^ { s }$ we can rewrite problem (10.13) in the following equivalent form: 

$$
\begin{array}{r l} \min _ {y, X ^ {1}, \ldots , X ^ {n _ {s}}} & c ^ {T} y + \frac {1}{2} y ^ {T} Q y \\ \mathrm{s.t.} & f _ {i} ^ {T} y = b _ {i}, i = 1, \ldots , 3 n _ {s}, \\ & H _ {k} ^ {s} \bullet X ^ {s} = 0, k = 1, 2, s = 1, \ldots , n _ {s}, \\ & (g _ {k} ^ {s}) ^ {T} y + H _ {k} ^ {s} \bullet X ^ {s} = 0, k = 3, 4, 5, 6, s = 1, \ldots , n _ {s}, \\ & X ^ {s} \succeq 0, s = 1, \ldots , n _ {s}, \end{array}
$$

where  denotes the trace matrix inner product. 

(10.14) 

We should note that standard semidefinite optimization software such as SDPT3 [72] can solve only problems with linear objective functions. Since the objective function of (10.14) is quadratic in y a reformulation is necessary to solve this problem using SDPT3 or other SDP solvers. We can replace the objective function with min t where t is a new artificial variable and impose the constraint $\begin{array} { r } { t \ge c ^ { T } y + \frac { 1 } { 2 } y ^ { T } Q y } \end{array}$ . This new constraint can be expressed as a second-order cone constraint after a simple change of variables; see, e.g., [49]. This final formulation is a standard form conic optimization problem — a class of problems that contain semidefinite programming and secondorder cone programming as special classes. Since SDPT3 can solve standard form conic optimization problems we used this formulation in our numerical experiments. 

Exercise 10.6 Express the constraint $\begin{array} { r } { t \ge c ^ { T } y + \frac { 1 } { 2 } y ^ { T } Q y } \end{array}$ using linear constraints and a second-order cone constraint. 

## 10.4 Arbitrage Bounds for Forward Start Options

When pricing securities with complicated payof structures, one of the strategies analysts use is to develop a portfolio of “related” securities in order to form a super (or sub) hedge and then use no-arbitrage arguments to bound the price of the complicated security. Finding the super or sub hedge that gives the sharpest no-arbitrage bounds is formulated as an optimization problem. We considered an similar approach in Section 4.2 when we used linear programming models for detecting arbitrage possibilities in prices of European options with a common underlying asset and same maturity. 

In this section, we consider the problem of finding arbitrage bounds for prices of forward start options using prices of standard options expiring either at the activation or expiration date of the forward start option. As we will see this problem can be solved using semidefinite optimization. The tool we use to achieve this is the versatile result of Bertsimas and Popescu given in Proposition 10.1. 

A forward start option is an advance purchase, say at time $T _ { 0 }$ , of a put or call option that will become active at some specified future time, say $T _ { 1 }$ These options are encountered frequently in employee incentive plans where an employee may be ofered an option on the company stock that will be available after the employee remains with the company for a predetermined length of time. A premium is paid at $T _ { 0 }$ , and the underlying security and the expiration date $\left( T _ { 2 } \right)$ are specified at that time. Let $S _ { 1 }$ and $S _ { 2 }$ denote the spot price of the underlying security at times $T _ { 1 }$ and $T _ { 2 }$ , respectively. 

The strike price is described as a known function of $S _ { 1 }$ but is unknown at $T _ { 0 }$ . It is determined at $T _ { 1 }$ when the option becomes active. Typically, it is chosen to be the value of the underlying asset at that time, $\mathrm { i . e . , } S _ { 1 }$ , so that the option is at-the-money at time $T _ { 1 }$ . More generally, the strike can be chosen as $\gamma S _ { 1 }$ for some positive constant $\gamma$ . We address the general case here. The payof to the buyer of a forward start call option at time $T _ { 2 }$ is max $( 0 , S _ { 2 } - \gamma S _ { 1 } ) = ( S _ { 2 } - \gamma S _ { 1 } ) ^ { + }$ , and similarly it is $( \gamma S _ { 1 } - S _ { 2 } ) ^ { + }$ for puts. 

Our primary objective is to find tightest possible no-arbitrage bounds $( { \mathrm { i . e . } }$ , maximize the lower bound and minimize the upper bound) by finding the best possible sub- and super-replicating portfolios of European options of several strikes with exercise dates at $T _ { 1 }$ and also others with exercise dates at $T _ { 2 }$ . We will also consider the possibility of trading the underlying asset at time $T _ { 1 }$ in a self-financing manner (via risk-free borrowing/lending). For concreteness, we limit our attention to the forward start call option problem and only consider calls for replication purposes. Since we allow the shorting of calls, the omission of puts does not lose generality. 

We show how to (approximately) solve the following problem: Find the cheapest portfolio of the underlying (traded now and/or at $T _ { 1 } )$ , cash, calls expiring at time $T _ { 1 }$ , and calls expiring at time $T _ { 2 }$ , such that the payof from the portfolio always is at least max $( 0 , S _ { 2 } - \phi ( S _ { 1 } ) )$ , no matter what $S _ { 1 }$ and $S _ { 2 }$ turn out to be. There is a similar lower bound problem which can be solved identically. 

For simplification, we assume throughout the rest of this discussion that the risk-free interest rate r is zero and that the underlying does not pay any dividends. We also assume throughout the discussion that the prices of options available for replication are arbitrage-free which implies the existence of equivalent martingale measures consistent with these prices. Furthermore, we ignore trading costs. 

## 10.4.1 A Semi-Static Hedge

For replication purposes, we assume that a number of options expiring at $T _ { 1 }$ and $T _ { 2 }$ are available for trading. Let $K _ { 1 } ^ { 1 } < K _ { 2 } ^ { 1 } < . . . < K _ { m } ^ { 1 }$ denote the strike prices of options expiring at $T _ { 1 }$ and $K _ { 1 } ^ { 2 } < K _ { 2 } ^ { 2 } < \ldots < K _ { n } ^ { 2 }$ denote the strike prices of the options expiring at $T _ { 2 }$ . Let $p ^ { 1 } = ( p _ { 1 } ^ { 1 } , . . . , p _ { m } ^ { 1 } )$ and $p ^ { 2 } = ( p _ { 1 } ^ { 2 } , . . . , p _ { n } ^ { 2 } )$ denote the (arbitrage free) prices of these options at time $T _ { 0 }$ 

We assume that $K _ { 1 } ^ { 1 } = 0$ , so that the first ”call” is the underlying itself and $p _ { 1 } ^ { 1 } = S _ { 0 }$ , the price of the underlying at $T _ { 0 }$ . For our formulation, let $x = ( x _ { 1 } , x _ { 2 } , \ldots , x _ { m } )$ and $y = ( y _ { 1 } , y _ { 2 } , \dotsc , y _ { n } )$ correspond to the positions in the $T _ { 1 }$ and T<sub>2</sub>-expiry options in our portfolio. Let $B$ denote the cash position in the portfolio at time $T _ { 0 }$ . Then the cost of this portfolio is 

$$
c (x, y, B) := \sum_ {i = 1} ^ {m} p _ {i} ^ {1} x _ {i} + \sum_ {j = 1} ^ {n} p _ {j} ^ {2} y _ {j} + B.\tag{10.15}
$$

With only positions in these call options, we would have a static hedge. To improve the bounds, we consider a semi-static hedge that is rebalanced at time $T _ { 1 }$ through the purchase of underlying shares whose quantity is determined based on the price of the underlying at that time. If $f ( S _ { 1 } )$ shares of the underlying is purchased at time $T _ { 1 }$ and if this purchase is financed by risk-free borrowing, our overall position would have the final payof of: 

$$
\begin{array}{r c l} g (S _ {1}, S _ {2}) & := & g _ {S} (S _ {1}, S _ {2}) + f (S _ {1}) (S _ {2} - S _ {1}) \\ & = & \sum_ {i = 1} ^ {m} (S _ {1} - K _ {i} ^ {1}) ^ {+} x _ {i} + \sum_ {j = 1} ^ {n} (S _ {2} - K _ {j} ^ {2}) ^ {+} y _ {j} + B + f (S _ {1}) (S _ {2} - S _ {1}). \end{array} \tag {10.16}
$$

Exercise 10.7 Verify equation (10.16). 

Then, we would find the lower and upper bounds on the price of the forward start option by solving the following problems: 

$$
\begin{array}{r l} {u := \min _ {x, y, B, f}} & {c (x, y, B)} \\ {\mathrm{s.t.}} & {g (S _ {1}, S _ {2}) \geq (S _ {2} - \gamma S _ {1}) ^ {+}, \forall S _ {1}, S _ {2} \geq 0} \end{array}\tag{10.17}
$$

The inequalities in this optimization problem ensure the super-replication properties of the semi-static hedge we constructed. Unfortunately, there are infinitely many constraints indexed by the parameters $S _ { 1 }$ and $S _ { 2 }$ . Therefore, (10.17) is a semi-infinite linear optimization problems and can be dificult. 

Fortunately, however, the constraint functions are expressed using piecewiselinear functions of $S _ { 1 }$ and $S _ { 2 }$ . The breakpoints for these functions are at the strike sets $\{ K _ { 1 } ^ { 1 } , \ldots , K _ { m } ^ { 1 } \}$ and $\{ K _ { 1 } ^ { 2 } , \ldots , K _ { n } ^ { 2 } \}$ . The right-hand-side function $( S _ { 2 } - \gamma S _ { 1 } ) ^ { + }$ has breakpoints along the line $S _ { 2 } = \gamma S _ { 1 }$ . The remaining dificulty is about the specification of the function $f .$ By limiting our attention to functions $f$ that are piecewise linear we will obtain a conic optimization formulation. 

A piecewise linear function $f ( S _ { 1 } )$ is determined by its values at the breakpoints: $z _ { i } = f ( K _ { i } ^ { 1 } )$ for $i = 1 , \dots ,$ m and its slope past $K _ { m } ^ { 1 }$ the last breakpoint given by $\lambda _ { z } = f ( K _ { m } ^ { 1 } + 1 ) - f ( K _ { m } ^ { 1 } )$ 

Thus, we approximate $f ( S _ { 1 } )$ as 

$$
f (S _ {1}) = \left\{ \begin{array}{l l} z _ {i} + (S _ {1} - K _ {i} ^ {1}) \frac {z _ {i + 1} - z _ {i}}{K _ {i + 1} ^ {1} - K _ {i} ^ {1}} & \text {if} S _ {1} \in [ K _ {i} ^ {1}, K _ {i + 1} ^ {1}), \\ z _ {m} + (S _ {1} - K _ {m} ^ {1}) \lambda_ {z} & \text {if} S _ {1} \geq K _ {m} ^ {1}. \end{array} \right.
$$

Next, we consider a decomposition of the nonnegative orthant $( S _ { 1 } , S _ { 2 } \geq$ 0) into a grid with breakpoints at $K _ { i } ^ { 1 }$ ’s and $K _ { j } ^ { 2 } { } ^ { , }$ s such that the payof function is linear in each box $B _ { i j } = [ K _ { i } ^ { 1 } , K _ { i + 1 } ^ { 1 } ] \times [ K _ { j } ^ { 2 } , K _ { j + 1 } ^ { 2 } ] ;$ 

$$
\begin{array}{r c l} g (S _ {1}, S _ {2}) & = & \sum_ {k = 1} ^ {n} (S _ {1} - K _ {k} ^ {1}) ^ {+} x _ {k} + \sum_ {l = 1} ^ {n} (S _ {2} - K _ {l} ^ {2}) ^ {+} y _ {l} + B + (S _ {2} - S _ {1}) f (S _ {1}) \\ & = & \sum_ {k = 1} ^ {i} (S _ {1} - K _ {k} ^ {1}) x _ {k} + \sum_ {l = 1} ^ {j} (S _ {2} - K _ {l} ^ {2}) y _ {l} + B + (S _ {2} - S _ {1}) \left(z _ {i} + (S _ {1} - K _ {i} ^ {1}) \frac {z _ {i + 1} - z _ {i}}{K _ {i + 1} ^ {1} - K _ {i} ^ {1}}\right) \end{array}
$$

Recall that we want to super-replicate the payof $( S _ { 2 } \mathrm { ~ - ~ } \gamma S _ { 1 } ) ^ { + }$ . This is the term $g ( S _ { 1 } , S _ { 2 } )$ must exceed for all $S _ { 1 } , S _ { 2 }$ . When we consider the box $B _ { i j } : = [ K _ { i } ^ { 1 } , K _ { i + 1 } ^ { 1 } ] \times [ K _ { j } ^ { 2 } , K _ { j + 1 } ^ { 2 } ]$ there are three possibilities involving $\gamma ;$ see also Figure 10.4.1: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/1e24183b7fbfa8dbfc6659f7bf1f273c4df1e9edb1e892e22d33e9cb1612d614.jpg)



Figure 10.2: Three possible relative positions of the $S _ { 2 } = \gamma S _ { 1 }$ line


1. $S _ { 2 } > \gamma S _ { 1 }$ for all $( S _ { 1 } , S _ { 2 } ) \in B _ { i j }$ . Then, we replace $( S _ { 2 } - \gamma S _ { 1 } ) ^ { + }$ with $( S _ { 2 } - \gamma S _ { 1 } )$ 

2. $S _ { 2 } < \gamma S _ { 1 }$ for all $( S _ { 1 } , S - 2 ) \in B _ { i j }$ . Then, we replace $( S _ { 2 } - \gamma S _ { 1 } ) ^ { + }$ with 0. 

3. Otherwise, we replace $g ( S _ { 1 } , S _ { 2 } ) \geq ( S _ { 2 } { - } \gamma S _ { 1 } ) ^ { + }$ with the two inequalities $g ( S _ { 1 } , S _ { 2 } ) \geq ( S _ { 2 } - \gamma S _ { 1 } )$ and $g ( S _ { 1 } , S _ { 2 } ) \geq 0$ 

In all cases, we remove the nonlinearity on the RHS. Now, we can rewrite the super-replication inequality 

$$
g (S _ {1}, S _ {2}) \geq (S _ {2} - \gamma S _ {1}) +, \forall (S _ {1}, S _ {2}) \in B _ {i j} \text { as }\tag{10.18}
$$

$$
\alpha_ {i j} (w) S _ {1} ^ {2} + \beta_ {i j} (w) S _ {1} + \delta_ {i j} (w) S _ {1} S _ {2} + \epsilon_ {i j} (w) S _ {2} + \eta_ {i j} (w) \geq 0, \forall (S _ {1}, S _ {2})\tag{\( \notin1B_{i}19) \}
$$

where $\boldsymbol { w } = ( x , y , z , B )$ represents the variables of the problem collectively and the constants $\alpha _ { i j }$ etc. are linear functions of these variables that are easily obtained. In Case 3, we have two such inequalities rather than one. 

Thus, the super-replication constraints in each box are polynomial inequalities that must hold within these boxes. This is very similar to the situation addressed by Proposition 10.1 with the important distinction that these polynomial inequalities are in two variables rather than one. 

Next, observe that for a fixed value of $S _ { 1 }$ , the function on the left-handside of inequality (10.19) is linear in $S _ { 2 }$ . Let us denote this function with $h _ { i j } ( S _ { 1 } , S _ { 2 } )$ . Since it is linear in $S _ { 2 }$ , for a fixed value of $S _ { 1 } , h _ { i j }$ will assume its minimum value in the interval $[ K _ { j } ^ { 2 } , K _ { j + 1 } ^ { 2 } ]$ either at $S _ { 2 } = K _ { j } ^ { 2 }$ or $S _ { 2 } = K _ { j + 1 } ^ { 2 } .$ Thus, if $h _ { i j } ( S _ { 1 } , K _ { j } ^ { 2 } ) \geq 0$ and $h _ { i j } ( \check { S } _ { 1 } , \check { K } _ { j + 1 } ^ { 2 } ) \geq 0$ , then $h _ { i j } ( S _ { 1 } , S _ { 2 } ) \geq 0$ , S<sub>2</sub> $[ K _ { j } ^ { 2 } , K _ { j + 1 } ^ { 2 } ]$ . As a result, $h _ { i j } ( S _ { 1 } , S _ { 2 } ) \geq \bar { 0 } , \forall ( S _ { 1 } , S _ { 2 } ) \in B _ { i j }$ is equivalent to the following two constraints: 

$$
\begin{array}{r c l} H _ {i j} ^ {l} (S _ {1}) := h _ {i j} (S _ {1}, K _ {j} ^ {2}) & \geq & 0, \forall S _ {1} \in [ K _ {i} ^ {1}, K _ {i + 1} ^ {1} ], \\ H _ {i j} ^ {u} (S _ {1}) := h _ {i j} (S _ {1}, K _ {j + 1} ^ {2}) & \geq & 0, \forall S _ {1} \in [ K _ {i} ^ {1}, K _ {i + 1} ^ {1} ] \end{array}
$$

The situation is illustrated in Figure 10.4.1. Instead of satisfying the inequality on the whole box as in the left-hand-side figure, we only need to consider two line segments as in the right-hand-side figure. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/9cad0afc6199ab28a3b700f74f94f2fa4d6f9b006515d83a9b6f8d18fd7d7bba.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/debfee2a31832ab49d500f979bd04e24f257d8bc8a9956565595a67403979370.jpg)



Figure 10.3: Super-replication constraints in the box $B _ { i j }$ and on the line segments


The bivariate polynomial inequality is reduced to two univariate polynomial inequalities. Now, we can use the Bertsimas/Popescu result and represent this inequality eficiently. In summary, the super-replication constraints can be rewritten using a finite number of linear constraints and semidefiniteness constraints. Since $H _ { i j } ^ { l }$ and $H _ { i j } ^ { u }$ are quadratic polynomials in $S _ { 1 }$ , semidefiniteness constraints are on $3 \times 3$ matrices (see Proposition 10.1) and are easily handled with semidefinite programming software. 

CHAPTER 10. CONIC OPTIMIZATION MODELS IN FINANCE 

# Integer Programming: Theory and Algorithms

## 11.1 Introduction

A linear programming model for constructing a portfolio of assets might produce a solution with 3,205.7 shares of stock XYZ and similarly complicated figures for the other assets. Most portfolio managers would have no trouble rounding the value 3,205.7 to 3,205 shares or even 3,200 shares. In this case, a linear programming model would be appropriate. Its optimal solution can be used efectively by the decision maker, with minor modifications. On the other hand, suppose that the problem is to find the best among many alternatives (for example, a traveling salesman wants to find a shortest route going through 10 specified cities). A model that suggests taking fractions of the roads between the various cities would be of little value. A 0,1 decision has to be made (a road between a pair of cities is either on the shortest route or it is not), and we would like the model to reflect this. 

This integrality restriction on the variables is the central aspect of integer programming. From a modeling standpoint, integer programming has turned out to be useful in a wide variety of applications. With integer variables, one can model logical requirements, fixed costs and many other problem aspects. Many software products can change a linear programming problem into an integer program with a single command. 

The downside of this power, however, is that problems with more than a thousand variables are often not possible to solve unless they show a specific exploitable structure. Despite the possibility (or even likelihood) of enormous computing times, there are methods that can be applied to solving integer programs. The most widely used is “branch and bound” (it is used, for example, in SOLVER). More sophisticated commercial codes (CPLEX and XPRESS are currently two of the best) use a combination of “branch and bound” and another complementary approach called “cutting plane”. Open source software codes in the COIN-OR library also implement a combination of branch and bound and cutting plane, called “branch and cut” (such as cbc, which stands for COIN Branch and Cut or bcp, which stands for Branch, Cut and Price). The purpose of this chapter is to describe some of the solution techniques. For the reader interested in learning more about integer programming, we recommend Wolsey’s introductory book [74]. The next chapter discusses problems in finance that can be modeled as integer programs: combinatorial auctions, constructing an index fund, portfolio optimization with minimum transaction levels. 

First we introduce some terminology. An integer linear program is a linear program with the additional constraint that some of, or all, the variables are required to be integer. When all variables are required to be integer the problem is called a pure integer linear program. If some variables are restricted to be integer and some are not then the problem is a mixed integer linear program, denoted MILP. The case where the integer variables are restricted to be 0 or 1 comes up surprisingly often. Such problems are called pure (mixed) 0–1 linear programs or pure (mixed) binary integer linear programs. The case of an NLP with the additional constraint that some of the variables are required to be integer is called MINLP is receiving an increasing amount of attention from researchers. In this chapter, we concentrate on MILP. 

## 11.2 Modeling Logical Conditions

Suppose we wish to invest $19,000. We have identified four investment opportunities. Investment 1 requires an investment of $6,700 and has a net present value of $8,000; investment 2 requires $10,000 and has a value of $11,000; investment 3 requires $5,500 and has a value of $6,000; and investment 4 requires $3,400 and has a value of $4,000. Into which investments should we place our money so as to maximize our total present value? Each project is a “take it or leave it” opportunity: It is not allowed to invest partially in any of the projects. Such problems are called capital budgeting problems. 

As in linear programming, our first step is to decide on the variables. In this case, it is easy: We will use a 0–1 variable $x _ { j }$ for each investment. If $x _ { j }$ is 1 then we will make investment j. If it is 0, we will not make the investment. 

This leads to the 0–1 programming problem: 

$\max 8x_{1} + 11x_{2} + 6x_{3} + 4x_{4}$ subject to $6.7x_{1} + 10x_{2} + 5.5x_{3} + 3.4x_{4}\leq 19$ $x_{j} = 0$ or 1. 

Now, a straightforward “bang for buck” suggests that investment 1 is the best choice. In fact, ignoring integrality constraints, the optimal linear programming solution is $x _ { 1 } = 1 , x _ { 2 } = 0 . 8 9 , x _ { 3 } = 0 , x _ { 4 } = 1$ for a value of $21,790. Unfortunately, this solution is not integral. Rounding $x _ { 2 }$ down to 0 gives a feasible solution with a value of $12,000. There is a better integer solution, however, of $x _ { 1 } = 0 , x _ { 2 } = 1 , x _ { 3 } = 1 , x _ { 4 } = 1$ for a value of $21,000. This example shows that rounding does not necessarily give an optimal solution. 

There are a number of additional constraints we might want to add. For instance, consider the following constraints: 

1. We can only make two investments. 

2. If investment 2 is made, then investment 4 must also be made. 

3. If investment 1 is made, then investment 3 cannot be made. 

All of these, and many more logical restrictions, can be enforced using 0–1 variables. In these cases, the constraints are: 

1. $x_{1} + x_{2} + x_{3} + x_{4}\leq 2$ 2. $x_{2} - x_{4}\leq 0$ 3. $x_{1} + x_{3}\leq 1$ 

## Solving the model with SOLVER

Modeling an integer program in SOLVER is almost the same as modeling a linear program. For example, if you placed binary variables x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, x<sub>4</sub> in cells $B$5:$B$8, simply Add the constraint 

to your other constraints in the SOLVER dialog box. Note that the Bin option is found in the small box where you usually indicate the type of inequality: =, <= or >=. Just click on Bin. That’s all there is to it! 

It is equally easy to model an integer program within other commercial codes. The formulation might look as follows. 

```fortran
! Capital budgeting example
VARIABLES
x(i=1:4)
OBJECTIVE
Max: 8*x(1) + 11*x(2) + 6*x(3) + 4*x(4)
CONSTRAINTS
Budget: 6.7*x(1) + 10*x(2) + 5.5*x(3) + 3.4*x(4) < 19
BOUNDS
x(i=1:4) Binary
END 
```

Exercise 11.1 As the leader of an oil exploration drilling venture, you must determine the best selection of 5 out of 10 possible sites. Label the sites $s _ { 1 } , s _ { 2 } , \ldots , s _ { 1 0 }$ and the expected profits associated with each as $p _ { 1 } , p _ { 2 } , \ldots , p _ { 1 0 }$ 

(i) If site s<sub>2</sub> is explored, then site s<sub>3</sub> must also be explored. Furthermore, regional development restrictions are such that 

(ii) Exploring sites $s _ { 1 }$ and s<sub>7</sub> will prevent you from exploring site $s _ { 8 }$ . 

(iii) Exploring sites $s _ { 3 }$ or $s _ { 4 }$ will prevent you from exploring site $s _ { 5 }$ . 

Formulate an integer program to determine the best exploration scheme and solve with SOLVER. 

$$
\begin{array}{r l r} \text {Solution:} & & \\ \max & \sum_ {j = 1} ^ {1 0} p _ {j} x _ {j} \\ \text {subject to} & & \\ & \sum_ {j = 1} ^ {1 0} x _ {j} & = 5 \\ & x _ {2} - x _ {3} & \leq 0 \\ & x _ {1} + x _ {7} + x _ {8} & \leq 2 \\ & x _ {3} + x _ {5} & \leq 1 \\ & x _ {4} + x _ {5} & \leq 1 \\ & x _ {j} & = 0 \text {or} 1 \text {for j = 1,\ldots,10.} \end{array}
$$


Exercise 11.2 Consider the following investment projects where, for each project, you are given its NPV as well as the cash outflow required during each year (in million dollars).


<table><tr><td></td><td>NPV</td><td>Year 1</td><td>Year 2</td><td>Year 3</td><td>Year 4</td></tr><tr><td>Project 1</td><td>30</td><td>12</td><td>4</td><td>4</td><td>0</td></tr><tr><td>Project 2</td><td>30</td><td>0</td><td>12</td><td>4</td><td>4</td></tr><tr><td>Project 3</td><td>20</td><td>3</td><td>4</td><td>4</td><td>4</td></tr><tr><td>Project 4</td><td>15</td><td>10</td><td>0</td><td>0</td><td>0</td></tr><tr><td>Project 5</td><td>15</td><td>0</td><td>11</td><td>0</td><td>0</td></tr><tr><td>Project 6</td><td>15</td><td>0</td><td>0</td><td>12</td><td>0</td></tr><tr><td>Project 7</td><td>15</td><td>0</td><td>0</td><td>0</td><td>13</td></tr><tr><td>Project 8</td><td>24</td><td>8</td><td>8</td><td>0</td><td>0</td></tr><tr><td>Project 9</td><td>18</td><td>0</td><td>0</td><td>10</td><td>0</td></tr><tr><td>Project 10</td><td>18</td><td>0</td><td>0</td><td>0</td><td>10</td></tr></table>

No partial investment is allowed in any of these projects. The firm has 18 million dollars available for investment each year. 

(i) Formulate an integer linear program to determine the best investment plan and solve with SOLVER. 

(ii) Formulate the following conditions as linear constraints. 

Exactly one of Projects 4, 5, 6, 7 must be invested in. 

If Project 1 is invested in, then Project 2 cannot be invested in. 

If Project 3 is invested in, then Project 4 must also be invested in. 

If Project 8 is invested in, then either Project 9 or Project 10 must also be invested in. 

If either Project 1 or Project 2 is invested in, then neither Project 8 nor Project 9 can be invested in. 

$\begin{array}{r}\max 20x_{1} + 10x_{2} + 10x_{3}\\ 2x_{1} + 20x_{2} + 4x_{3}\leq 15\\ 6x_{1} + 20x_{2} + 4x_{3} = 20\\ x_{1},x_{2},x_{3}\geq 0\text{integer}. \end{array}$ 

## 11.3 Solving Mixed Integer Linear Programs

Historically, the first method developed for solving MILP’s was based on cutting planes (adding constraints to the underlying linear program to cut of noninteger solutions). This idea was proposed by Gomory in 1958. Branch and bound was proposed in 1960 by Land and Dong. It is based on dividing the problem into a number of smaller problems (branching) and evaluating their quality based on solving the underlying linear programs (bounding). Branch and bound has been the most efective technique for solving MILP’s in the following forty years or so. However, in the last ten years, cutting planes have made a resurgence and are now eficiently combined with branch and bound into an overall procedure called branch and cut. This term was coined by Padberg and Rinaldi in 1987. All these approaches involve solving a series of linear programs. So that is where we begin. 

## 11.3.1 Linear Programming Relaxation

Given a mixed integer linear program 

$$
\begin{array}{c} \text {(MILP) min c^ {T} x} \\ A x \geq b \\ x \geq 0 \\ x _ {j} \text {integer for j = 1,\ldots,p} \end{array}
$$

there is an associated linear program called the relaxation formed by dropping the integrality restrictions: 

(R) min $c ^ { T } x$ 

$$
\begin{array}{l} A x \geq b \\ x \geq 0. \end{array}
$$

Since R is less constrained than MILP, the following are immediate: 

The optimal objective value for R is less than or equal to the optimal objective for MILP. 

If R is infeasible, then so is MILP. 

If the optimal solution $x ^ { * }$ of R satisfies $\boldsymbol { x } _ { j } ^ { * }$ integer for $j = 1 , \dotsc , p ,$ then $x ^ { * }$ is also optimal for MILP. 

So solving R does give some information: it gives a bound on the optimal value, and, if we are lucky, may give the optimal solution to MILP. However, rounding the solution of R will not in general give the optimal solution of MILP. 

## Exercise 11.3 Consider the problem

Solve its linear programming relaxation. Then, show that it is impossible to obtain a feasible integral solution by rounding the values of the variables. 

Exercise 11.4 (a) Compare the feasible solutions of the three following integer linear programs: 

(i) $\max 14x_{1} + 8x_{2} + 6x_{3} + 6x_{4}$ $28x_{1} + 15x_{2} + 13x_{3} + 12x_{4}\leq 39$ $x_{1},x_{2},x_{3},x_{4}\in \{0,1\} ,$ 

(ii) $\max 14x_{1} + 8x_{2} + 6x_{3} + 6x_{4}$ $2x_{1} + x_{2} + x_{3} + x_{4}\leq 2$ $x_{1},x_{2},x_{3},x_{4}\in \{0,1\} ,$ 

(iii) $\max 14x_{1} + 8x_{2} + 6x_{3} + 6x_{4}$ $x_{2} + x_{3} + x_{4}\leq 2$ $x_{1} + x_{2}\leq 1$ $x_{1} + x_{3}\leq 1$ $x_{1} + x_{4}\leq 1$ $x_{1},x_{2},x_{3},x_{4}\in \{0,1\} .$ 

(b) Compare the relaxations of the above integer programs obtained by replacing $x _ { 1 } , x _ { 2 } , x _ { 3 } , x _ { 4 } \in \{ 0 , 1 \}$ by $0 \leq x _ { j } \leq 1$ for $j = 1 , \dots , 4 .$ . Which is the best formulation among (i), (ii) and (iii) for obtaining a tight bound from the linear programming relaxation? 

## 11.3.2 Branch and Bound

## An example:

We first explain branch and bound by solving the following pure integer linear program (see Figure 11.1). 

$\begin{array}{r}\max x_1 + x_2\\ -x_1 + x_2\leq 2\\ 8x_1 + 2x_2\leq 19\\ x_1,x_2\geq 0\\ x_1,x_2\text{integer}. \end{array}$ 

The first step is to solve the linear programming relaxation obtained by ignoring the last constraint. The solution is $x _ { 1 } = 1 . 5 , x _ { 2 } = 3 . 5$ with objective value 5. This is not a feasible solution to the integer program since the values of the variables are fractional. How can we exclude this solution while preserving the feasible integral solutions? One way is to branch, creating two linear programs, say one with $x _ { 1 } \leq 1$ , the other with $x _ { 1 } \geq 2$ . Clearly, any solution to the integer program must be feasible to one or the other of these two problems. We will solve both of these linear programs. Let us start with 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/f00d970e441533813b34191dda84fb470316ab19535a824efe26b1e426776480.jpg)



Figure 11.1: A two-variable integer program


$\max x_{1} + x_{2}$ $-x_{1} + x_{2}\leq 2$ $8x_{1} + 2x_{2}\leq 19$ $x_{1}\leq 1$ $x_{1},x_{2}\geq 0.$ 

The solution is $x _ { 1 } = 1 , x _ { 2 } = 3$ with objective value 4. This is a feasible integral solution. So we now have an upper bound of 5 as well as a lower bound of 4 on the value of an optimum solution to the integer program. Now we solve the second linear program 

$\begin{array}{rl}\max x_1 + x_2 & \\ -x_1 + x_2 \leq 2 & \\ 8x_1 + 2x_2 \leq 19 & \\ x_1 \geq 2 & \\ x_1, x_2 \geq 0. \end{array}$ 

The solution is $x _ { 1 } = 2 , x _ { 2 } = 1 . 5$ with objective value 3.5. Because this value is worse that the lower bound of 4 that we already have, we do not need any further branching. We conclude that the feasible integral solution of value 4 found earlier is optimum. 

The solution of the above integer program by branch and bound required the solution of three linear programs. These problems can be arranged in a branch-and-bound tree, see Figure 11.2. Each node of the tree corresponds to one of the problems that were solved. 

We can stop the enumeration at a node of the branch-and-bound tree for three diferent reasons (when they occur, the node is said to be pruned). 

Pruning by integrality occurs when the corresponding linear program has an optimum solution that is integral. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/4fdc8021-b28c-456e-9dfa-00a53a256dcc/d363615b91c48a587e22bda665a1b898a31569c2e70045346feefbd167ccf559.jpg)



Figure 11.2: Branch-and-bound tree


Pruning by bounds occurs when the objective value of the linear program at that node is worse than the value of the best feasible solution found so far. 

Pruning by infeasibility occurs when the linear program at that node is infeasible. 

To illustrate a larger tree, let us solve the same integer program as above, with a diferent objective function: 

$$
\begin{array}{r l} & {\max 3 x _ {1} + x _ {2}} \\ & {- x _ {1} + x _ {2} \leq 2} \\ & {8 x _ {1} + 2 x _ {2} \leq 1 9} \\ & {x _ {1}, x _ {2} \geq 0} \\ & {x _ {1}, x _ {2} \mathrm{integer}.} \end{array}
$$

The solution of the linear programming relaxation is $x _ { 1 } = 1 . 5$ , x<sub>2</sub> = 3.5 with objective value 8. Branching on variable $x _ { 1 }$ , we create two linear programs. The one with the additional constraint $x _ { 1 } \ \leq \ 1$ has solution $x _ { 1 } = 1 , x _ { 2 } = 3$ with value 6 (so now we have an upper bound of 8 and a lower bound of 6 on the value of an optimal solution of the integer program). The linear program with the additional constraint $x _ { 2 } \geq 2$ has solution $x _ { 1 } = 2$ 2 $x _ { 2 } = 1 . 5$ and objective value 7.5. Note that the value of $x _ { 2 }$ is fractional, so this solution is not feasible to the integer program. Since its objective value is higher than 6 (the value of the best integer solution found so far), we need to continue the search. Therefore we branch on variable $x _ { 2 }$ . We create two linear programs, one with the additional constraint $x _ { 2 } \geq 2$ , the other with $x _ { 2 } \leq 1$ , and we solve both. The first of these linear programs is infeasible. The second is 

$\begin{array}{r}\max 3x_{1} + x_{2}\\ -x_{1} + x_{2}\leq 2\\ 8x_{1} + 2x_{2}\leq 19\\ x_{1}\geq 2\\ x_{2}\leq 1\\ x_{1},x_{2}\geq 0. \end{array}$ 

<!-- === Source: MinerU_markdown_Optimization_Methods_in_Finance_201_2122706384180064275.md (Page 201) === -->

The solution is $x _ { 1 } = 2 . 1 2 5 , x _ { 2 } = 1$ with objective value 7.375. Because this value is greater than 6 and the solution is not integral, we need to branch again on $x _ { 1 }$ . The linear program with $x _ { 1 } \geq 3$ is infeasible. The one with $x _ { 1 } \leq 2$ is 

$\begin{array}{r}\max 3x_{1} + x_{2}\\ -x_{1} + x_{2}\leq 2\\ 8x_{1} + 2x_{2}\leq 19\\ x_{1}\geq 2\\ x_{2}\leq 1\\ x_{1}\leq 2\\ x_{1},x_{2}\geq 0. \end{array}$ 

The solution is $x _ { 1 } = 2 , x _ { 2 } = 1$ with objective value 7. This node is pruned by integrality and the enumeration is complete. The optimal solution is the one with value 7. See Figure 11.3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/f4e2e51b647b50f1a7c866599ca9f29d3e2fe056745419294609cde1ac4eae46.jpg)



Figure 11.3: Branch-and-bound tree for modified example


## The branch-and-bound algorithm:

Consider a mixed integer linear program 

$$
\begin{array}{r l} \text {(MILP)} z _ {I} = & \min c ^ {T} x \\ & A x \geq b \\ & x \geq 0 \\ & x _ {j} \text {integer for} j = 1, \ldots , p. \end{array}
$$

The data are an n-vector $c ,$ an m n matrix $A ,$ , an m-vector b and an integer $p$ such that $1 \leq p \leq n$ . The set $I = \{ 1 , \ldots , p \}$ indexes the integer variables whereas the set $C = \{ p + 1 , \ldots , n \}$ indexes the continuous variables. The branch-and-bound algorithm keeps a list of linear programming problems obtained by relaxing the integrality requirements on the variables and imposing constraints such as $x _ { j } \ \leq \ u _ { j } \ \mathrm { o r } \ x _ { j } \ \geq \ l _ { j }$ . Each such linear program corresponds to a node of the branch-and-bound tree. For a node $N _ { i } ,$ let $z _ { i }$ denote the value of the corresponding linear program (it will be convenient to denote this linear program by $N _ { i }$ as well). Let $\mathcal { L }$ denote the list of nodes that must still be solved (i.e. that have not been pruned nor branched on). Let $z _ { U }$ denote an upper bound on the optimum value $z _ { I }$ (initially, the bound $z _ { U }$ can be derived from a heuristic solution of (MILP), or it can be set to + ). 

## 0. Initialize

$$
\mathcal {L} = \{M I L P \}, z _ {U} = + \infty , x ^ {*} = \emptyset .
$$

## 1. Terminate?

If ${ \mathcal { L } } = \emptyset .$ the solution $x ^ { * }$ is optimal. 

## 2. Select node

Choose and delete a problem $N _ { i }$ from ${ \mathcal { L } } .$ 

## 3. Bound

Solve $N _ { i }$ . If it is infeasible, go to Step 1. Else, let $x ^ { i }$ be its solution and z<sub>i</sub> its objective value. 

## 4. Prune

If $z _ { i } \geq z _ { U } .$ , go to Step 1. 

If $x ^ { i }$ is not feasible to (MILP), go to Step 5. 

If $x ^ { i }$ is feasible to (MILP), let $z _ { U } = z _ { i } , x ^ { * } = x ^ { i }$ and delete from all problems with $z _ { j } \geq z _ { U }$ . Go to Step 1. 

## 5. Branch

$\vdots$ From $N _ { i }$ , construct linear programs $N _ { i } ^ { 1 } , \ldots , N _ { i } ^ { k }$ with smaller feasible regions whose union contains all the feasible solutions of (MILP) in $N _ { i }$ Add $N _ { i } ^ { 1 } , \ldots , N _ { i } ^ { k }$ to $\mathcal { L }$ and go to Step 1. 

Various choices are left open by the algorithm, such as the node selection criterion and the branching strategy. We will discuss some options for these choices. Even more important to the success of branch-and-bound is the ability to prune the tree (Step 4). This will occur when $z _ { U }$ is a good upper bound on $z _ { I }$ and when $z _ { i }$ is a good lower bound. For this reason, it is crucial to have a formulation of (MILP) such that the value of its linear programming relaxation $z _ { L P }$ is as close as possible to $z _ { I }$ . To summarize, four issues need attention when solving MILP’s by branch and bound. 

Formulation (so that the gap $z _ { I } - z _ { L P }$ is small). 

Heuristics (to find a good upper bound $z _ { U } )$ 

• <sup>Branching.</sup> 

Node selection. 

We defer the formulation issue to Section 11.3.3 on cutting planes. This issue will also be addressed in Chapter 12. Heuristics can be designed either as stand alone (an example will be given in Section 12.3) or as part of the branch-and-bound algorithm (by choosing branching and node selection strategies that are more likely to produce feasible solutions $x ^ { i }$ to (MILP) in Step 4). We discuss branching strategies first, followed by node selection strategies and heuristics. 

## Branching

Problem $N _ { i }$ is a linear program. A way of dividing its feasible region is to impose bounds on a variable. Let $\boldsymbol { x } _ { j } ^ { i }$ be one of the fractional values for $j = 1 , \dotsc , p ,$ in the optimal solution $x ^ { i }$ of $N _ { i }$ (we know that there is such $\mathrm { ~ a ~ } j .$ since otherwise $N _ { i }$ would have been pruned in Step 4 on account of $x ^ { i }$ being feasible to (MILP)). ¿From problem $N _ { i }$ , we can construct two linear programs $N _ { i j } ^ { - }$ and $N _ { i j } ^ { + }$ that satisfy the requirements of Step 5 by adding the constraints $x _ { j } \leq \lfloor x _ { j } ^ { i } \rfloor$ and $x _ { j } \geq \lceil x _ { j } ^ { i } \rceil$ respectively to $N ^ { i }$ . This is called branching on a variable. The advantage of branching on a variable is that the number of constraints in the linear programs does not increase, since linear programming solvers treat bounds on variables implicitly. 

An important question is: On which variable $x _ { j }$ should we branch, among the $j = 1 , \dotsc , p$ such that $\boldsymbol { x } _ { j } ^ { i }$ is fractional? To answer this question, it would be very helpful to know the increase $D _ { i j } ^ { - }$ in objective value between $N _ { i }$ and $N _ { i j } ^ { - }$ , and $D _ { i j } ^ { + }$ between $N _ { i }$ and $N _ { i j } ^ { + }$ . A good branching variable $x _ { j }$ at node $N ^ { i }$ is one for which both $D _ { i j } ^ { - }$ and $D _ { i j } ^ { + }$ are relatively large (thus tightening the lower bound $z _ { i } ,$ which is useful for pruning). For example, researchers have proposed to choose $j = 1 , \dotsc , p$ such that min $( D _ { i j } ^ { - } , D _ { i j } ^ { + } )$ is the largest. Others have proposed to choose $j$ such that $D _ { i j } ^ { - } + D _ { i j } ^ { + }$ is the largest. Combining these two criteria is even better, with more weight on the first. 

The strategy which consists in computing $D _ { i j } ^ { - }$ and $D _ { i j } ^ { + }$ explicitly for each j is called strong branching. It involves solving linear programs that are small variations of $N _ { i }$ by performing dual simplex pivots (recall Section 2.4.5), for each $j = 1 , \dotsc , p$ such that $\boldsymbol { x } _ { j } ^ { i }$ is fractional and each of the two bounds. Experiments indicate that strong branching reduces the size of the enumeration tree by a factor of 20 or more in most cases, relative to a simple branching rule such as branching on the most fractional variable. Thus there is a clear benefit to spending time on strong branching. But the computing time of doing it at each node $N _ { i }$ , for every fractional variable $\boldsymbol { x } _ { j } ^ { i }$ may be too high. A reasonable strategy is to restrict the $j ^ { \prime } \mathrm { s }$ that are evaluated to those for which the fractional part of $\boldsymbol { x } _ { j } ^ { i }$ is closest to 0.5 so that the amount of computing time spent performing these evaluations is limited. Significantly more time should be spent on these evaluations towards the top of the tree. This leads to the notion of pseudocosts that are initialized at the root node and then updated throughout the branch-and-bound tree. 

Let $f _ { j } ^ { i } = x _ { j } ^ { i } - \lfloor x _ { j } ^ { i } \rfloor$ be the fractional part of $\boldsymbol { x } _ { j } ^ { i }$ , for $j = 1 , \hdots p$ . For an index j such that $f _ { j } ^ { i } > 0$ , define the down pseudocost and up pseudocost as 

$$
P _ {j} ^ {-} = \frac {D _ {i j} ^ {-}}{f _ {j} ^ {i}} \text {and} P _ {j} ^ {+} = \frac {D _ {i j} ^ {+}}{1 - f _ {j} ^ {i}}
$$

respectively. Benichou et al [9] observed that the pseudocosts tend to remain fairly constant throughout the branch-and-bound tree. Therefore the pseudocosts need not be computed at each node of the tree. They are estimated instead. How are they initialized and how are they updated in the tree? A good way of initializing the pseudocosts is through strong branching at the root node or other nodes of the tree when a variable becomes fractional for the first time. The down pseudocost $P _ { j } ^ { - }$ − is updated by averaging the observations $\frac { D _ { i j } ^ { - } } { f _ { j } ^ { i } }$ over all the nodes of the tree where $x _ { j }$ was branched on. Similarly for the up pseudocost $P _ { j } ^ { + }$ . The decision of which variable to branch on at a node $N _ { i }$ of the tree is done as follows. The estimated pseudocosts $P _ { j } ^ { - }$ and $P _ { j } ^ { + }$ are used to compute estimates of $D _ { i j } ^ { - }$ and $D _ { i j } ^ { + }$ at node $N _ { i }$ , namely $\begin{array} { r } { D _ { i j } ^ { - } = P _ { j } ^ { - } f _ { j } ^ { i } } \end{array}$ and $D _ { i j } ^ { + } = P _ { j } ^ { + } ( 1 - f _ { j } ^ { i } )$ for each $j = 1 , \dotsc , p$ such that $f _ { j } ^ { i } > 0$ . Among these candidates, the branching variable $x _ { j }$ is chosen to be the one with largest min $( D _ { i j } ^ { - } , D _ { i j } ^ { + } )$ (or other criteria such as those mentioned earlier). 

## Node selection

How does one choose among the diferent problems $N _ { i }$ available in Step 2 of the algorithm? Two goals need to be considered: finding good feasible solutions (thus decreasing the upper bound $z _ { U } )$ and proving optimality of the current best feasible solution (by increasing the lower bound as quickly as possible). 

For the first goal, we estimate the value of the best feasible solution in each node $N _ { i }$ . For example, we could use the following estimate: 

$$
E _ {i} = z _ {i} + \sum_ {j = 1} ^ {p} \min (P _ {j} ^ {-} f _ {j} ^ {i}, P _ {j} ^ {+} (1 - f _ {j} ^ {i}))
$$

based on the pseudocosts defined above. This corresponds to rounding the noninteger solution $x ^ { i }$ to a nearby integer solution and using the pseudocosts to estimate the degradation in objective value. We then select a node $N _ { i }$ with the smallest $E _ { i }$ . This is the so-called “best estimate criterion” node selection strategy. 

For the second goal, the best strategy depends on whether the first goal has been achieved already. If we have a very good upper bound $z _ { U }$ , it is reasonable to adopt a depth-first search strategy. This is because the linear programs encountered in a depth-first search are small variations of one another. As a result they can be solved faster in sequence, using the dual simplex method initialized with the optimal solution of the father node (about 10 times faster, based on empirical evidence). On the other hand, if no good upper bound is available, depth-first search is wasteful: it may explore many nodes with a value $z _ { i }$ that is larger than the optimum $z _ { I }$ . This can be avoided by using the “best bound” node selection strategy, which consists in picking a node $N _ { i }$ with the smallest bound $z _ { i }$ . Indeed, no matter how good a solution of (MILP) is found in other nodes of the branch-andbound tree, the node with the smallest bound $z _ { i }$ cannot be pruned by bounds (assuming no ties) and therefore it will have to be explored eventually. So we might as well explore it first. This strategy minimizes the total number of nodes in the branch-and-bound tree. 

The most successful node selection strategy may difer depending on the application. For this reason, most MILP solvers have several node selection strategies available as options. The default strategy is usually a combination of the “best estimate criterion” (or a variation) and depth-first search. Specifically, the algorithm may dive using depth-first search until it reaches an infeasible node $N _ { i }$ or it finds a feasible solution of (MILP). At this point, the next node might be chosen using the “best estimate criterion” strategy, and so on, alternating between dives in a depth-first search fashion to get feasible solutions at the bottom of the tree and the “best estimate criterion” to select the next most promising node. 

## Heuristics

Heuristics are useful for improving the bound $z _ { U }$ , which helps in Step 4 for pruning by bounds. Of course, heuristics are even more important when the branch-and-bound algorithm is too time consuming and has to be terminated before completion, returning a solution of value $z _ { U }$ without a proof of its optimality. 

We have already presented all the ingredients needed for a diving heuristic: Solve the linear programming relaxation, use strong branching or pseudocosts to determine a branching variable; then compute the estimate $E _ { i }$ at each of the two sons and move down the branch corresponding to the smallest of the two estimates. Solve the new linear programming relaxation with this variable fixed and repeat until infeasibility is reached or a solution of (MILP) is found. The diving heuristic can be repeated from a variety of starting points (corresponding to diferent sets of variables being fixed) to improve the chance of getting good solutions. 

An interesting idea that has been proposed recently to improve a feasible solution of (MILP) is called local branching [27]. This heuristic is particularly suited for $\mathrm { M L P ^ { \prime } s }$ that are too large to solve to optimality, but where the linear programming relaxation can be solved in reasonable time. For simplicity, assume that all the integer variables are 0,1 valued. Let x¯ be a feasible solution of (MILP) (found by a diving heuristic, for example). The idea is to define a neighborhood of x¯ as follows: 

$$
\sum_ {j = 1} ^ {p} | x _ {j} - \bar {x} _ {j} | \leq k
$$

where $k$ is an integer chosen by the user (for example k = 20 seems to work well), to add this constraint to (MILP) and apply your favorite MILP solver. Instead of getting lost in a huge enumeration tree, the search is restricted to the neighborhood of x¯ by this constraint. Note that the constraint should be linearized before adding it to the formulation, which is easy to do: 

$$
\sum_ {j \in I: \bar {x} _ {j} = 0} x _ {j} + \sum_ {j \in I: \bar {x} _ {j} = 1} (1 - x _ {j}) \leq k.
$$

If a better solution than x¯ is found, the neighborhood is redefined relatively to this new solution, and the procedure is repeated until no better solution can be found. 

Exercise 11.5 Consider an investment problem as in Section 11.2. We have $14,000 to invest among four diferent investment opportunities. Investment 1 requires an investment of $7,000 and has a net present value of $11,000; investment 2 requires $5,000 and has a value of $8,000; investment 3 requires $4,000 and has a value of $6,000; and investment 4 requires $3,000 and has a value of $4,000. As in Section 11.2, these are “take it or leave $\mathrm { i t } ^ { \dag }$ opportunities and we are not allowed to invest partially in any of the projects. The objective is to maximize our total value given the budget constraint. We do not have any other (logical) constraints. 

We formulate this problem as an integer program using 0–1 variables x<sub>j</sub> for each investment. As before, $x _ { j }$ is 1 if make investment $j$ and 0 if we do not. This leads to the following formulation: 

$$
\begin{array}{c} M a x 1 1 x _ {1} + 8 x _ {2} + 6 x _ {3} + 4 x _ {4} \\ 7 x _ {1} + 5 x _ {2} + 4 x _ {3} + 3 x _ {4} \leq 1 4 \\ x _ {j} = 0 o r 1. \end{array}
$$

The linear relaxation solution is $x _ { 1 } = 1 , x _ { 2 } = 1 , x _ { 3 } = 0 . 5 , x _ { 4 } = 0$ with a value of 22. Since $x _ { 3 }$ is not integer, we do not have an integer solution yet. Solve this problem using the branch-and-bound technique. 

Exercise 11.6 Solve the 3 integer linear programs of Exercise 11.4 using your favorite solver. In each case, report the number of nodes in the enumeration tree. Is it related to the tightness of the linear programming relaxtion studied in Exercise 11.4 (b)? 

Exercise 11.7 Modify the branch-and-bound algorithm so that it stops as soon as it has a feasible solution that is guaranteed to be within $p \%$ of the optimum. 

## 11.3.3 Cutting Planes

In order to solve the mixed integer linear program 

(MILP) min $c ^ { T } x$ 

$$
A x \geq b
$$

$$
x \geq 0
$$

x<sub>j</sub> integer for j = 1, . . . , p 

a possible approach is to strengthen the linear programming relaxation 

(R) min c<sup>T</sup> x 

$$
\begin{array}{l} c ^ {T} x \\ A x \geq b \\ x \geq 0. \end{array}
$$

by adding valid inequalities for (MILP). When the optimal solution $x ^ { * }$ of the strengthened linear program is valid for (MILP), then $x ^ { * }$ is also an optimal solution of (MILP). Even when this does not occur, the strengthened linear program may provide better lower bounds in the context of a branch-andbound algorithm. How do we generate valid inequalities for (MILP)? 

Gomory [31] proposed the following approach. Consider nonnegative variables $x _ { j }$ for $j \in I \cup C$ , where $x _ { j }$ must be integer valued for $j \in I$ . We allow the possibility that $C = \emptyset$ . Let 

$$
\sum_ {j \in I} a _ {j} x _ {j} + \sum_ {j \in C} a _ {j} x _ {j} = b\tag{11.1}
$$

be an equation satisfied by these variables. Assume that b is not an integer and let $f _ { 0 }$ be its fractional part, i.e. $b = \lfloor b \rfloor + f _ { 0 }$ where $0 < f _ { 0 } < 1$ . For $j \in I$ , let $a _ { j } = \lfloor a _ { j } \rfloor + f _ { j }$ where $0 \leq f _ { j } < 1$ . Replacing in (11.1) and moving sums of integer products to the right, we get: 

$$
\sum_ {j \in I: f _ {j} \leq f _ {0}} f _ {j} x _ {j} + \sum_ {j \in I: f _ {j} > f _ {0}} (f _ {j} - 1) x _ {j} + \sum_ {j \in C} a _ {j} x _ {j} = k + f _ {0}
$$

where $k$ is some integer. 

Using the fact that $k \leq - 1$ or $k \geq 0$ , we get the disjunction 

$$
\sum_ {j \in I: f _ {j} \leq f _ {0}} \frac {f _ {j}}{f _ {0}} x _ {j} - \sum_ {j \in I: f _ {j} > f _ {0}} \frac {1 - f _ {j}}{f _ {0}} x _ {j} + \sum_ {j \in C} \frac {a _ {j}}{f _ {0}} x _ {j} \geq 1
$$

OR 

$$
- \sum_ {j \in I: f _ {j} \leq f _ {0}} \frac {f _ {j}}{1 - f _ {0}} x _ {j} + \sum_ {j \in I: f _ {j} > f _ {0}} \frac {1 - f _ {j}}{1 - f _ {0}} x _ {j} - \sum_ {j \in C} \frac {a _ {j}}{1 - f _ {0}} x _ {j} \geq 1.
$$

This is of the form $\begin{array} { r } { \sum _ { j } a _ { j } ^ { 1 } x _ { j } \geq 1 \ o r \sum _ { j } a _ { j } ^ { 2 } x _ { j } \geq 1 } \end{array}$ which implies $\sum \operatorname* { m a x } ( a _ { j } ^ { 1 } , a _ { j } ^ { 2 } ) x _ { j } \geq$ 1 for $x \geq 0$ 

Which is the largest of the two coeficients in our case? The answer is easy since one coeficient is positive and the other is negative for each variable. 

$$
\sum_ {j \in I: f _ {j} \leq f _ {0}} \frac {f _ {j}}{f _ {0}} x _ {j} + \sum_ {j \in I: f _ {j} > f _ {0}} \frac {1 - f _ {j}}{1 - f _ {0}} x _ {j} + \sum_ {j \in C: a _ {j} > 0} \frac {a _ {j}}{f _ {0}} x _ {j} - \sum_ {j \in C: a _ {j} <   0} \frac {a _ {j}}{1 - f _ {0}} x _ {j} \geq 1.\tag{11.2}
$$

Inequality (11.2) is valid for all $x \geq 0$ that satisfy (11.1) with $x _ { j }$ integer for all $j \in I$ . It is called the Gomory mixed integer cut (GMI cut). 

Let us illustrate the use of Gomory’s mixed integer cuts on the 2-variable example of Figure 11.1. Recall that the corresponding integer program is 

## 208CHAPTER 11. INTEGER PROGRAMMING: THEORY AND ALGORITHMS

$\max z = x_{1} + x_{2}$ $-x_{1} + x_{2}\leq 2$ $8x_{1} + 2x_{2}\leq 19$ $x_{1},x_{2}\geq 0$ $x_{1},x_{2}$ integer. 

We first add slack variables $x _ { 3 }$ and $x _ { 4 }$ to turn the inequality constraints into equalities. The problem becomes: 

$z - x_{1} - x_{2} = 0$ $-x_{1} + x_{2} + x_{3} = 2$ $8x_{1} + 2x_{2} + x_{4} = 19$ $x_{1},x_{2},x_{3},x_{4}\geq 0$ $x_{1},x_{2},x_{3},x_{4}$ integer. 

Solving the linear programming relaxation by the simplex method (Section 2.4), we get the optimal tableau: 

$z + 0.6x_{3} + 0.2x_{4} = 5$ $x_{2} + 0.8x_{3} + 0.1x_{4} = 3.5$ $x_{1} - 0.2x_{3} + 0.1x_{4} = 1.5$ $x_{1},x_{2},x_{3},x_{4}\geq 0$ 

The corresponding basic solution is $x _ { 3 } = x _ { 4 } = 0 , x _ { 1 } = 1 . 5 , x _ { 2 } = 3 . 5$ and $z = 5$ . This solution is not integer. Let us generate the Gomory mixed integer cut corresponding to the equation 

$$
x _ {2} + 0. 8 x _ {3} + 0. 1 x _ {4} = 3. 5
$$

found in the final tableau. We have $f _ { 0 } = 0 . 5 , \ f _ { 1 } = f _ { 2 } = 0 , \ f _ { 3 } = 0 . 8$ and $f _ { 4 } = 0 . 1$ . Applying formula (11.2), we get the GMI cut 

$$
\frac {1 - 0 . 8}{1 - 0 . 5} x _ {3} + \frac {0 . 1}{0 . 5} x _ {4} \geq 1, \quad \mathrm{i.e.} \quad 2 x _ {3} + x _ {4} \geq 5.
$$

We could also generate a GMI cut from the other equation in the final tableau $x _ { 1 } - 0 . 2 x _ { 3 } + 0 . 1 x _ { 4 } = 1 . 5$ . It turns out that, in this case, we get exactly the same GMI cut. We leave it to the reader to verify this. 

Since $x _ { 3 } = 2 + x _ { 1 } - x _ { 2 } { \mathrm { ~ a n d ~ } } x _ { 4 } = 1 9 - x _ { 1 } - 2 x _ { 2 }$ , we can express the above GMI cut in the space $( x _ { 1 } , x _ { 2 } )$ . This yields 

$$
3 x _ {1} + 2 x _ {2} \leq 9.
$$

Adding this cut to the linear programming relaxation, we get the following formulation (see Figure 11.4). 

$\begin{array}{r}\max x_1 + x_2\\ -x_1 + x_2\leq 2\\ 8x_1 + 2x_2\leq 19\\ 3x_1 + 2x_2\leq 9\\ x_1,x_2\geq 0 \end{array}$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/e1e34b029a61cb4e1fffc172c091fd2ad200274412d9887757c1b829d90986c1.jpg)



Figure 11.4: Formulation strengthened by a cut


Solving this linear program by the simplex method, we find the basic solution $x _ { 1 } = 1 , x _ { 2 } = 3 { \mathrm { ~ a n d ~ } } z = 4$ . Since $x _ { 1 }$ and $x _ { 2 }$ are integer, this is the optimal solution to the integer program. 

## Exercise 11.8 Consider the integer program

$\begin{array}{r}\max 10x_{1} + 13x_{2}\\ 10x_{1} + 14x_{2}\leq 43\\ x_{1},x_{2}\geq 0\\ x_{1},x_{2}\text{integer}. \end{array}$ 

(i) Introduce slack variables and solve the linear programming relaxation by the simplex method. (Hint: You should find the following optimal tableau: 

$$
\begin{array}{c} \min x _ {2} + x _ {3} \\ x _ {1} + 1. 4 x _ {2} + 0. 1 x _ {3} = 4. 3 \\ x _ {1}, x _ {2} \geq 0 \end{array}
$$

with basic solution $x _ { 1 } = 4 . 3 , x _ { 2 } = x _ { 3 } = 0 . )$ 

(ii) Generate a GMI cut that cuts of this solution. 

(iii) Multiply both sides of the equation $x _ { 1 } + 1 . 4 x _ { 2 } + 0 . 1 x _ { 3 } = 4 . 3$ by the constant $k = 2$ and generate the corresponding GMI cut. Repeat for $k = 3 .$ 4 and 5. Compare the five GMI cuts that you found. 

(iv) Add the GMI cut generated for $k \mathit { \Theta } = \mathit { \Theta } 3$ to the linear programming relaxation. Solve the resulting linear program by the simplex method. What is the optimum solution of the integer program? 

Exercise 11.9 (a) Consider the 2-variable mixed integer set 

$$
S := \{(x, y) \in \mathbb {N} \times \mathbb {R} _ {+}: x - y \leq b \}
$$

where $b \in \mathcal { W }$ . Let $f _ { 0 } = b - \lfloor b \rfloor$ . Show that 

$$
x - \frac {1}{1 - f _ {0}} y \leq \lfloor b \rfloor
$$

is a valid inequality for S. 

(b) Consider the mixed integer set 

$$
S := \{(x, y) \in \mathbb {N} ^ {n} \times \mathbb {R} _ {+} ^ {p}: a ^ {T} x - g ^ {T} y \leq b \}
$$

where $a \in I R ^ { n } , g \in I R ^ { p }$ and $b \in \mathbb { R }$ . Let $f _ { 0 } = b - \lfloor b \rfloor$ and $f _ { j } = a _ { j } - \lfloor a _ { j } \rfloor $ Show that 

$$
\sum_ {j = 1} ^ {n} \left(\left\lfloor a _ {j} \right\rfloor + \frac {\left(f _ {j} - f _ {0}\right) ^ {+}}{1 - f _ {0}}\right) x _ {j} + \frac {1}{1 - f _ {0}} \sum_ {j: g _ {j} <   0} g _ {j} y _ {j} \leq \left\lfloor b \right\rfloor
$$

is a valid inequality for $S .$ 

## 11.3.4 Branch and Cut

The best software packages for solving MILPs use neither pure branch-andbound nor pure cutting plane algorithms. Instead they combine the two approaches in a method called branch and cut. The basic structure is essentially the same as branch and bound. The main diference is that, when a node $N _ { i }$ is explored, cuts may be generated to strengthen the formulation, thus improving the bound $z _ { i }$ . Some cuts may be local (i.e. valid only at node $N _ { i }$ and its descendants) or global (valid at all the nodes of the branch-and-bound tree). Cplex and Xpress are two excellent commercial branch-and-cut codes. cbc (COIN branch and cut) and bcp (branch, cut and price) are open source codes in the COIN-OR library. 

Below, we give an example of an enumeration tree obtained when running the branch-and-cut algorithm of a commercial code on an instance with 89 binary variables and 28 constraints. Nodes of degree two (other than the root) occur when one the sons can be pruned immediately by bounds or infeasibility. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/938deda44578a201ea209817dc0a5a4e2ef814403b563709628efa9b589c4772.jpg)



Figure 11.5: A branch-and-cut enumeration tree


212CHAPTER 11. INTEGER PROGRAMMING: THEORY AND ALGORITHMS 

# Integer Programming Models: Constructing an Index Fund

This chapter presents several applications of integer linear programming: combinatorial auctions, the lockbox problem and index funds. We also present a model of integer quadratic programming: portfolio optimization with minimum transaction levels. 

## 12.1 Combinatorial Auctions

In many auctions, the value that a bidder has for a set of items may not be the sum of the values that he has for individual items. It may be more or it may be less. Examples are equity trading, electricity markets, pollution right auctions and auctions for airport landing slots. To take this into account, combinatorial auctions allow the bidders to submit bids on combinations of items. 

Specifically, let $M = \{ 1 , 2 , \dots , m \}$ be the set of items that the auctioneer has to sell. A bid is a pair $B _ { j } = ( S _ { j } , p _ { j } )$ where $S _ { j } \subseteq M$ is a nonempty set of items and $p _ { j }$ is the price ofer for this set. Suppose that the auctioneer has received n bids $B _ { 1 } , B _ { 2 } , \ldots , B _ { n }$ . How should the auctioneer determine the winners in order to maximize his revenue? This can be done by solving an integer program. Let $x _ { j }$ be a 0,1 variable that takes the value 1 if bid $B _ { j }$ wins, and 0 if it looses. The auctioneer maximizes his revenue by solving the integer program: 

$$
\begin{array}{r c l} \max & \sum_ {i = 1} ^ {n} & p _ {j} x _ {j} \\ \text {subject to} & \sum_ {j: i \in S _ {j}} x _ {j} & \leq 1 \quad \text {for} i = 1, \ldots , m \\ & x _ {j} & = 0 \text {or} 1 \quad \text {for} j = 1, \ldots , n. \end{array}
$$

The constraints impose that each item i is sold at most once. 

For example, if there are four items for sale and the following bids have been received: $B _ { 1 } \ = \ ( \{ 1 \} , 6 ) , \ B _ { 2 } \ = \ ( \{ 2 \} , 3 ) , \ B _ { 3 } \ = \ ( \{ 3 , 4 \} , 1 2 ) , \ B _ { 4 } \ =$ ( 1, 3 , 12), B<sub>5</sub> = ( 2, 4 , 8), B<sub>6</sub> = ( 1, 3, 4 , 16), the winners can be determined by the following integer program: 

$$
\begin{array}{r l} \max & 6 x _ {1} + 3 x _ {2} + 1 2 x _ {3} + 1 2 x _ {4} + 8 x _ {5} + 1 6 x _ {6} \\ \text {subject to} & x _ {1} + x _ {4} + x _ {6} \leq 1 \\ & x _ {2} + x _ {5} \leq 1 \\ & x _ {3} + x _ {4} + x _ {6} \leq 1 \\ & x _ {3} + x _ {5} + x _ {6} \leq 1 \\ & x _ {j} = 0 \text {or} 1 \quad \text {for} j = 1, \ldots , 6. \end{array}
$$

In some auctions, there are multiple indistinguishable units of each item for sale. A bid in this setting is defined as $B _ { j } = ( \lambda _ { 1 } ^ { j } , \lambda _ { 2 } ^ { j } , \ldots , \lambda _ { m } ^ { j } ; p _ { j } )$ where $\lambda _ { i } ^ { j }$ is the desired number of units of item i and $p _ { j }$ is the price ofer. The auctioneer maximizes his revenue by solving the integer program: 

$$
\begin{array}{r c l} & \max & \sum_ {i = 1} ^ {n} \qquad p _ {j} x _ {j} \\ \text { subject   to } & \sum_ {j: i \in S _ {j}} \lambda_ {i} ^ {j} x _ {j} & \leq u _ {i} \quad \text { for } i = 1, \ldots , m \\ & x _ {j} & = 0 \text { or } 1 \quad \text { for } j = 1, \ldots , n. \end{array}
$$

where $u _ { i }$ is the number of units of item i for sale. 

Exercise 12.1 In a combinatorial exchange, both buyers and sellers can submit combinatorial bids. Bids are like in the multiple item case, except that the $\lambda _ { i } ^ { j }$ values can be negative, as can the prices $p _ { j }$ , representing selling instead of buying. Note that a single bid can be buying some items while selling other items. Write an integer linear program that will maximize the surplus generated by the combinatorial exchange. 

## 12.2 The Lockbox Problem

Consider a national firm that receives checks from all over the United States. Due to the vagaries of the U.S. Postal Service, as well as the banking system, there is a variable delay from when the check is postmarked (and hence the customer has met her obligation) and when the check clears (and when the firm can use the money). For instance, a check mailed in Pittsburgh sent to a Pittsburgh address might clear in just 2 days. A similar check sent to Los Angeles might take 4 days to clear. It is in the firm’s interest to have the check clear as quickly as possible since then the firm can use the money. In order to speed up this clearing process, firms open ofices (called lockboxes) in diferent cities to handle the checks. 

## 12.2. THE LOCKBOX PROBLEM

For example, suppose we receive payments from 4 regions (West, Midwest, East, and South). The average daily value from each region is as follows: $600,000 from the West, $240,000 from the Midwest, $720,000 from the East, and $360,000 from the South. We are considering opening lockboxes in Los Angeles, Pittsburgh, Boston, and/or Houston. Operating a lockbox costs $90,000 per year. The average days from mailing to clearing is given in Table 12.1. Which lockboxes should we open? 

<table><tr><td>From</td><td>L.A.</td><td>Pittsburgh</td><td>Boston</td><td>Houston</td></tr><tr><td>West</td><td>2</td><td>4</td><td>6</td><td>6</td></tr><tr><td>Midwest</td><td>4</td><td>2</td><td>5</td><td>5</td></tr><tr><td>East</td><td>6</td><td>5</td><td>2</td><td>5</td></tr><tr><td>South</td><td>7</td><td>5</td><td>6</td><td>3</td></tr></table>


Table 12.1: Clearing Times


First we must calculate the lost interest for each possible assignment. For example, if the West sends its checks to a lockbox in Boston, then on average there will be $\$ 3,600,000 \ (=6 \times \ S 600,00 0 )$ in process on any given day. Assuming an investment rate of 5%, this corresponds to a yearly loss of $180,000. We can calculate the losses for the other combinations in a similar fashion to get Table 12.2. 

<table><tr><td>From</td><td>L.A.</td><td>Pittsburgh</td><td>Boston</td><td>Houston</td></tr><tr><td>West</td><td>60</td><td>120</td><td>180</td><td>180</td></tr><tr><td>Midwest</td><td>48</td><td>24</td><td>60</td><td>60</td></tr><tr><td>East</td><td>216</td><td>180</td><td>72</td><td>180</td></tr><tr><td>South</td><td>126</td><td>90</td><td>108</td><td>54</td></tr></table>


Table 12.2: Lost Interest (’000)


To formulate the problem as an integer linear program, we will use the following variables. Let $y _ { j }$ be a 0–1 variable that is 1 if lockbox j is opened and 0 if it is not. Let $x _ { i j }$ be 1 if region i sends its checks to lockbox $j$ . 

The objective is to minimize total yearly costs: 

$$
6 0 x _ {1 1} + 1 2 0 x _ {1 2} + 1 8 0 x _ {1 3} + 1 8 0 x _ {1 4} + 4 8 x _ {2 1} + \dots + 9 0 y _ {1} + 9 0 y _ {2} + 9 0 y _ {3} + 9 0 y _ {4}.
$$

Each region must be assigned to one lockbox: 

$$
\sum_ {j} x _ {i j} = 1 \text { for   all } i.
$$

The regions cannot send checks to closed lockboxes. For lockbox 1 (Los Angeles), this can be written as: 

$$
x _ {1 1} + x _ {2 1} + x _ {3 1} + x _ {4 1} \leq 4 y _ {1}.
$$

Indeed, suppose that we do not open a lockbox in L.A. Then $y _ { 1 }$ is 0, so all of $x _ { 1 1 } , x _ { 2 1 } , x _ { 3 1 }$ , and $x _ { 4 1 }$ must also be. On the other hand, if we open a lockbox in $\mathrm { L . A . } ,$ then $y _ { 1 }$ is 1 and there is no restriction on the x values. 

We can create constraints for the other lockboxes to finish of the integer program. For this problem, we would have 20 variables (4 y variables, 16 x variables) and 8 constraints. This gives the following integer program: 

$$
\begin{array}{l} \text {MIN} \quad 6 0 X 1 1 + 1 2 0 X 1 2 + 1 8 0 X 1 3 + 1 8 0 X 1 4 + 4 8 X 2 1 \\ \quad + 2 4 X 2 2 + 6 0 X 2 3 + 6 0 X 2 4 + 2 1 6 X 3 1 + 1 8 0 X 3 2 \\ \quad + 7 2 X 3 3 + 1 8 0 X 3 4 + 1 2 6 X 4 1 + 9 0 X 4 2 + 1 0 8 X 4 3 \\ \quad + 5 4 X 4 4 + 9 0 Y 1 + 9 0 Y 2 + 9 0 Y 3 + 9 0 Y 4 \\ \text {SUBJECT TO} \\ \quad X 1 1 + X 1 2 + X 1 3 + X 1 4 = \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \end{array}
$$

If we ignore integrality, we get the solution $x _ { 1 1 } = x _ { 2 2 } = x _ { 3 3 } = x _ { 4 4 } = 1$ $y _ { 1 } = y _ { 2 } = y _ { 3 } = y _ { 4 } = 0 . 2 5$ and the rest equals 0. Note that we get no useful information out of this linear programming solution: all 4 regions look the same. 

The above is a perfectly reasonable 0–1 programming formulation of the lockbox problem. There are other formulations, however. For instance, consider the sixteen constraints of the form 

$$
x _ {i j} \leq y _ {j}.
$$

These constraints also force a region to only use open lockboxes. It might seem that a larger formulation is less eficient and therefore should be avoided. This is not the case! If we solve the linear program with the above constraints, we get the solution $x _ { 1 1 } = x _ { 2 1 } = x _ { 3 3 } = x _ { 4 3 } = y _ { 1 } = y _ { 3 } = 1$ with the rest equal to zero. In fact, we have an integer solution, which must therefore be optimal! Diferent integer programming formulations can have very diferent properties with respect to their linear programming relaxations. As a general rule, one prefers an integer programming formulation whose linear programming relaxation provides a tight bound. 

Exercise 12.2 Consider a lockbox problem where $c _ { i j }$ is the cost of assigning region i to a lockbox in region $j ,$ for $j = 1 , \dots , n$ . Suppose that we wish to open exactly q lockboxes where q is a given integer, $1 \leq q \leq n$ 

(a) Formulate as an integer linear program the problem of opening q lockboxes so as to minimize the total cost of assigning each region to an open lockbox. 

(b) Formulate in two diferent ways the constraint that regions cannot send checks to closed lockboxes. 

(c) For the following data, 

$$
q = 2 \quad \text {and} \quad (c _ {i j}) = \left( \begin{array}{l l l l l} 0 & 4 & 5 & 8 & 2 \\ 4 & 0 & 3 & 4 & 6 \\ 5 & 3 & 0 & 1 & 7 \\ 8 & 4 & 1 & 0 & 4 \\ 2 & 6 & 7 & 4 & 0 \end{array} \right)
$$

compare the linear programming relaxations of your two formulations in question (b). 

## 12.3 Constructing an Index Fund

An old and recurring debate about investing lies in the merits of active versus passive management of a portfolio. Active portfolio management tries to achieve superior performance by using technical and fundamental analysis as well as forecasting techniques. On the other hand, passive portfolio management avoids any forecasting techniques and rather relies on diversification to achieve a desired performance. There are 2 types of passive management strategies: “buy and hold” or “indexing”. In the first one, assets are selected on the basis of some fundamental criteria and there is no active selling or buying of these stocks afterwards (see the sections on Dedication in Chapter 3 and Portfolio Optimization in Chapter 8). In the second approach, absolutely no attempt is made to identify mispriced securities. The goal is to choose a portfolio that mirrors the movements of a broad market population or a market index. Such a portfolio is called an index fund. Given a target population of n stocks, one selects q stocks (and their weights in the index fund), to represent the target population as closely as possible. 

In the last twenty years, an increasing number of investors, both large and small, have established index funds. Simply defined, an index fund is a portfolio designed to track the movement of the market as a whole or some selected broad market segment. The rising popularity of index funds can be justified both theoretically and empirically. 

Market Eficiency: If the market is eficient, no superior risk-adjusted returns can be achieved by stock picking strategies since the prices reflect all the information available in the marketplace. Additionally, since the market portfolio provides the best possible return per unit of risk, to the extent that it captures the eficiency of the market via diversification, one may argue that the best theoretical approach to fund management is to invest in an index fund. 

Empirical Performance: Considerable empirical literature provides strong evidence that, on average, money managers have consistently underperformed the major indexes. In addition, studies show that, in most cases, top performing funds for a year are no longer amongst the top performers in the following years, leaving room for the intervention of luck as an explanation for good performance. 

Transaction Cost: Actively managed funds incur transaction costs, which reduce the overall performance of these funds. In addition, active management implies significant research costs. Finally, fund managers may have costly compensation packages that can be avoided to a large extent with index funds. 

Here we take the point of view of a fund manager who wants to construct an index fund. Strategies for forming index funds involve choosing a broad market index as a proxy for an entire market, e.g. the Standard and Poor list of 500 stocks (S & P 500). A pure indexing approach consists in purchasing all the issues in the index, with the same exact weights as in the index. In most instances, this approach is impractical (many small positions) and expensive (rebalancing costs may be incurred frequently). An index fund with q stocks, where q is substantially smaller than the size n of the target population seems desirable. We propose a large-scale deterministic model for aggregating a broad market index of stocks into a smaller more manageable index fund. This approach will not necessarily yield mean/variance eficient portfolios but will produce a portfolio that closely replicates the underlying market population. 

## 12.3.1 A Large-Scale Deterministic Model

We present a model that clusters the assets into groups of similar assets and selects one representative asset from each group to be included in the index fund portfolio. The model is based on the following data, which we will discuss in more detail later: 

$$
\rho_ {i j} = \text { similarity   between   stock } i \text { and   stock } j.
$$

For example, $\rho _ { i i } = 1 , \rho _ { i j } \leq 1$ for $i \neq j$ and $\rho _ { i j }$ is larger for more similar stocks. An example of this is the correlation between the returns of stocks i and $j .$ . But one could choose other similarity indices $\rho _ { i j }$ 

$$
\begin{array}{l l l} Z = \max & \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} & \rho_ {i j} x _ {i j} \\ \text { subject   to } & \sum_ {j = 1} ^ {n} y _ {j} & = q \\ & \sum_ {j = 1} ^ {n} x _ {i j} & = 1 \qquad \text { for   } i = 1, \ldots , n \\ & x _ {i j} & \leq y _ {j} \qquad \text { for   } i = 1, \ldots , n; j = 1, \ldots , n \\ & x _ {i j}, y _ {j} & = 0 \text {   or   } 1 \qquad \text { for   } i = 1, \ldots , n; j = 1, \ldots , n. \end{array}\tag{M}
$$

The variables $y _ { j }$ describe which stocks $j$ are in the index fund $( y _ { j } = 1$ if $j$ is selected in the fund, 0 otherwise). For each stock $i = 1 , \ldots , n$ , the variable $x _ { i j }$ indicates which stock $j$ in the index fund is most similar to i $( x _ { i j } = 1 \mathrm { i f } \ j$ is the most similar stock in the index fund, 0 otherwise). 

The first constraint selects $q$ stocks in the fund. The second constraint imposes that each stock i has exactly one representative stock $j$ in the fund. The third constraint guarantees that stock i can be represented by stock $j$ only if j is in the fund. The objective of the model maximizes the similarity between the n stocks and their representatives in the fund. 

Once the model has been solved and a set of $q$ stocks has been selected for the index fund, a weight $w _ { j }$ is calculated for each $j$ in the fund: 

$$
w _ {j} = \sum_ {i = 1} ^ {n} V _ {i} x _ {i j}
$$

where $V _ { i }$ is the market value of stock i. So $w _ { j }$ is the total market value of the stocks “represented” by stock $j$ in the fund. The fraction of the index fund to be invested in stock $j$ is proportional to the stock’s weight $w _ { j } .$ , i.e. 

$$
\frac {w _ {j}}{\sum_ {f = 1} ^ {n} w _ {f}}
$$

Note that, instead of the objective function used in $( M )$ , one could have used an objective function that takes the weights $w _ { j }$ directly into account, such as $\begin{array} { r } { \sum _ { i = 1 } ^ { n } \sum _ { j = 1 } ^ { n } V _ { i } \rho _ { i j } x _ { i j } } \end{array}$ . The q stocks in the index fund found by this P Pvariation of Model $( M )$ would still need to be weighted as explained in the previous paragraph. 

## Data Requirements

We need a coeficient $\rho _ { i j }$ which measures the similarity between stocks i and $j .$ . There are several ways of constructing meaningful coeficients $\rho _ { i j }$ One approach is to consider the time series of stock prices over a calibration period $T$ and to compute the correlation between each pair of assets. 

## Testing the Model

Stocks comprising the S&P 500 were chosen as the target population to test the model. A calibration period of sixty months was used. Then a portfolio of 25 stocks was constructed using model (M) and held for periods ranging from three months to three years. The following table gives the ratio of the population’s market value (normalized) to the index fund’s market value. A perfect index fund would have a ratio equal unity. 

## Solution Strategy

Branch-and-bound is a natural candidate for solving model (M). Note however that the formulation is very large. Indeed, for the S&P 500, there are 250,000 variables $x _ { i j }$ and 250,000 constraints $x _ { i j } \leq y _ { j }$ . So the linear programming relaxation needed to get upper bounds in the branch-and-bound algorithm is a very large linear program to solve. It turns out, however, that one does not need to solve this large linear program to obtain good upper bounds. Cornu´ejols, Fisher and Nemhauser [22] proposed using the following Lagrangian relaxation, which is defined for any vector $u = ( u _ { 1 } , \ldots , u _ { n } )$ 

<table><tr><td>Length</td><td>Ratio</td></tr><tr><td>1 QTR</td><td>1.006</td></tr><tr><td>2 QTR</td><td>.99</td></tr><tr><td>1 YR</td><td>.985</td></tr><tr><td>3 YR</td><td>.982</td></tr></table>


Table 12.3: Performance of a 25 stock index fund


$$
\begin{array}{r l r l} L (u) = \max & \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} \rho_ {i j} x _ {i j} + \sum_ {i = 1} ^ {n} u _ {i} (1 - \sum_ {j = 1} ^ {n} x _ {i j}) \\ \text {subject to} & \sum_ {j = 1} ^ {n} y _ {j} = q \\ & x _ {i j} \leq y _ {j} & & \text {for i = 1,\ldots,n} \\ & & j = 1, \ldots , n \\ & x _ {i j}, y _ {j} = 0 \text {or} 1 & & \text {for i = 1,\ldots,n} \\ & & j = 1, \ldots , n. \end{array}
$$

Property 1: $L ( u ) \ge Z$ , where $Z$ is the maximum for model (M). 

Exercise 12.3 Prove Property 1. 

The objective function $L ( u )$ may be equivalently stated as 

$$
L (u) = \max \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} (\rho_ {i j} - u _ {i}) x _ {i j} + \sum_ {i = 1} ^ {n} u _ {i}.
$$

Let 

$$
(\rho_ {i j} - u _ {i}) ^ {+} = \left\{ \begin{array}{c c} (\rho_ {i j} - u _ {i}) & \text { if } \rho_ {i j} - u _ {i} > 0 \\ 0 & \text { otherwise } \end{array} \right.
$$

and 

$$
C _ {j} = \sum_ {i = 1} ^ {n} (\rho_ {i j} - u _ {i}) ^ {+}.
$$

Then 

Property 2: 

$$
\begin{array}{r c l} L (u) & = & \max \sum_ {j = 1} ^ {n} C _ {j} y _ {j} + \sum_ {i = 1} ^ {n} u _ {i} \\ & & \text {subject to} \sum_ {j = 1} ^ {n} y _ {j} = q \\ & & y _ {j} = 0 \text {or} 1 \text {for} j = 1, \ldots , n. \end{array}
$$

Exercise 12.4 Prove Property 2. 

Property 3: In an optimal solution of the Lagrangian relaxation, $y _ { j }$ is equal to 1 for the $q$ largest values of $C _ { j }$ , and the remaining $y _ { j }$ are equal to 0. Furthermore, if $\rho _ { i j } - u _ { i } > 0$ , then $x _ { i j } = y _ { j }$ and otherwise $x _ { i j } = 0$ 

Exercise 12.5 Prove Property $3 .$ 

Interestingly, the set of $q$ stocks corresponding to the q largest values of $C _ { j }$ can also be used as a heuristic solution for model $( M )$ . Specifically, construct an index fund containing these $q$ stocks and assign each stock $i = 1 , \ldots , n$ to the most similar stock in this fund. This solution is feasible to model $( M )$ , although not necessarily optimal. This heuristic solution provides a lower bound on the optimum value $Z$ of model (M). As previously shown, $L ( u )$ provides an upper bound on $Z .$ So for any vector $u ,$ we can compute quickly both a lower bound and an upper bound on the optimum value of $( M )$ . To improve the upper bound $L ( u )$ , we would like to solve the nonlinear problem 

$$
\min L (u).
$$

How does one minimize $L ( u ) ?$ Since $L ( u )$ is nondiferentiable and convex, one can use the subgradient method (see Section 5.6). At each iteration, a revised set of Lagrange multipliers u and an accompanying lower bound and upper bound to model $( M )$ are computed. The algorithm terminates when these two bounds match or when a maximum number of iterations is reached (It is proved in [22] that min $L ( u )$ is equal to the value of the linear programming relaxation of $( M )$ . In general, min $L ( u )$ is not equal to $Z ,$ and therefore it is not possible to match the upper and lower bounds). If one wants to solve the integer program (M) to optimality, one can use a branch-and-bound algorithm, using the upper bound min $L ( u )$ for pruning the nodes. 

## 12.3.2 A Linear Programming Model

In this section, we consider a diferent approach to constructing an index fund. It can be particularly useful as one tries to rebalance the portfolio at minimum cost. This approach assumes that we have identified important characteristics of the market index to be tracked. Such characteristics might be the fraction $f _ { i }$ of the index in each sector $i ,$ the fraction of companies with market capitalization in various ranges (small, medium, large), the fraction of companies that pay no dividends, the fraction in each region etc. Let us assume that there are m such characteristics that we would like our index fund to track as well as possible. Let $a _ { i j } = 1$ if company $j$ has characteristic i and 0 if it does not. 

Let $x _ { j }$ denote the optimum weight of asset $j$ in the portfolio. Assume that initially, the portfolio has weights $x _ { j } ^ { 0 }$ . Let $y _ { j }$ denote the fraction of asset $j$ bought and $z _ { j }$ the fraction sold. The problem of rebalancing the portfolio at minimum cost is the following: 

subject to 

$$
\begin{array}{l l} \min \sum_ {j = 1} ^ {n} (y _ {j} + z _ {j}) \\ \sum_ {j = 1} ^ {n} a _ {i j} x _ {j} = f _ {i} & \text {for i = 1,\ldots,m} \\ \sum_ {j = 1} ^ {n} x _ {j} = 1 \\ x _ {j} - x _ {j} ^ {0} \leq y _ {j} & \text {for j = 1,\ldots,n} \\ x _ {j} ^ {0} - x _ {j} \leq z _ {j} & \text {for j = 1,\ldots,n} \\ y _ {j} \geq 0 & \text {for j = 1,\ldots,n} \\ z _ {j} \geq 0 & \text {for j = 1,\ldots,n} \\ x _ {j} \geq 0 & \text {for j = 1,\ldots,n}. \end{array}
$$

## 12.4 Portfolio Optimization with Minimum Transaction Levels

When solving the classical Markowitz model, the optimal portfolio often contains positions $x _ { i }$ that are too small to execute. In practice, one would like a solution of T 

$$
\begin{array}{r c l} \min _ {x} & \frac {1}{2} x ^ {T} Q x \\ & \mu^ {T} x & \geq R \\ & A x & = b \\ & C x & \geq d. \end{array}\tag{12.1}
$$

with the additional property that 

$$
x _ {j} > 0 \Rightarrow x _ {j} \geq l _ {j}\tag{12.2}
$$

where $l _ { j }$ are given minimum transaction levels. This constraint states that, if an investment is made in a stock, then it must be “large enough”, for example at least 100 shares. Because the constraint (12.2) is not a simple linear constraint, it cannot be handled directly by quadratic programming. 

This problem is considered by Bienstock [11]. He also considers the portfolio optimization problem where there is an upper bound on the number of positive variables, that is 

$$
x _ {j} > 0 \text {   for   at   most   } K \text {   distinct   } j = 1, \ldots , n.\tag{12.3}
$$

Requirement (12.2) can easily be incorporated within a branch-andbound algorithm: First solve the basic Markowitz model (12.1) using the usual algorithm (see Chapter 7). Let $x ^ { * }$ be the optimal solution found. If no minimum transaction level constraint (12.2) is violated by $x ^ { * }$ , then $x ^ { * }$ is also optimum to (12.1)-(12.2) and we can stop. Otherwise, let $j$ be an index for which (12.2) is violated by $x ^ { * }$ . Form two subproblems, one obtained from (12.1) by adding the constraint $x _ { j } = 0$ , and the other obtained from (12.1) by adding the constraint $x _ { j } \geq l _ { j }$ Both are quadratic programs that can be solved using the usual algorithms of Chapter 7. Now we check whether the optimum solutions to these two problems satisfy the transaction level constraint (12.2). If a solution violates (12.2) for index k, the corresponding problem is further divided by adding the constraint $x _ { k } = 0$ on one side and $x _ { k } \ge l _ { k }$ on the other. A branch-and-bound tree is expanded in this way. 

The constraint (12.3) is a little more tricky to handle. Assume that there is a given upper bound $u _ { j }$ on how much can be invested in stock $j .$ That is, we assume that constraints $x _ { j } \leq u _ { j }$ are part of the formulation (12.1). Then, clearly, constraint (12.3) implies the weaker constraint 

$$
\sum_ {j} \frac {x _ {j}}{u _ {j}} \leq K.\tag{12.4}
$$

We add this constraint to (12.1) and solve the resulting quadratic program. Let $x ^ { * }$ be the optimal solution found. If $x ^ { * }$ satisfies (12.3), it is optimum to (12.1)-(12.3) and we can stop. Otherwise, let k be an index for which $x _ { k } > 0$ Form two subproblems, one obtained from (12.1) by adding the constraint $x _ { k } = 0$ (down branch), and the other obtained from (12.1) by adding the constraint $\begin{array} { r } { \sum _ { j \neq k } \frac { x _ { j } } { u _ { i } } \leq K - 1 } \end{array}$ (up branch). The branch-and-bound tree is developped recursively. When a set $T$ of variables has been branched up, the constraint added to the basic model (12.1) becomes 

$$
\sum_ {j \not \in T} \frac {x _ {j}}{u _ {j}} \leq K - | T |.
$$

## 12.5 Exercises

Exercise 12.6 You have $ 250,000 to invest in the following possible investments. The cash inflows/outflows are as follows: 

<table><tr><td></td><td>Year 1</td><td>Year 2</td><td>Year 3</td><td>Year 4</td></tr><tr><td>Investment 1</td><td>-1.00</td><td></td><td>1.18</td><td></td></tr><tr><td>Investment 2</td><td></td><td>-1.00</td><td></td><td>1.22</td></tr><tr><td>Investment 3</td><td></td><td></td><td>-1.00</td><td>1.10</td></tr><tr><td>Investment 4</td><td>-1.00</td><td>0.14</td><td>0.14</td><td>1.00</td></tr><tr><td>Investment 5</td><td></td><td>-1.00</td><td>0.20</td><td>1.00</td></tr></table>

For example, if you invest one dollar in Investment 1 at the beginning of Year 1, you receive $ 1.18 at the beginning of Year 3. If you invest in any of these investments, the required minimum level is $ 100,000 in each case. Any or all the available funds at the beginning of a year can be placed in a money market account that yields 3 % per year. Formulate a mixed integer linear program to maximize the amount of money available at the beginning of Year 4. Solve the integer program using your favorite solver. 


Exercise 12.7 You currently own a portfolio of eight stocks. Using the Markowitz model, you computed the optimal mean/variance portfolio. The weights of these two portfolios are shown in the following table:


<table><tr><td>Stock</td><td>A</td><td>B</td><td>C</td><td>D</td><td>E</td><td>F</td><td>G</td><td>H</td></tr><tr><td>Your Portfolio</td><td>0.12</td><td>0.15</td><td>0.13</td><td>0.10</td><td>0.20</td><td>0.10</td><td>0.12</td><td>0.08</td></tr><tr><td>M/V Portfolio</td><td>0.02</td><td>0.05</td><td>0.25</td><td>0.06</td><td>0.18</td><td>0.10</td><td>0.22</td><td>0.12</td></tr></table>

You would like to rebalance your portfolio in order to be closer to the M/V portfolio. To avoid excessively high transaction costs, you decide to rebalance only three stocks from your portfolio. Let $x _ { i }$ denote the weight of stock i in your rebalanced portfolio. The objective is to minimize the quantity 

$$
\vert x _ {1} - 0. 0 2 \vert + \vert x _ {2} - 0. 0 5 \vert + \vert x _ {3} - 0. 2 5 \vert + \ldots + \vert x _ {8} - 0. 1 2 \vert
$$

which measures how closely the rebalanced portfolio matches the $\mathrm { M } / \mathrm { V }$ portfolio. 

Formulate this problem as a mixed integer linear program. Note that you will need to introduce new continuous variables in order to linearize the absolute values and new binary variables in order to impose the constraint that only three stocks are traded. 

## 12.6 Case Study

The purpose of this project is to construct an index fund that will track a given segment of the market. First, choose a segment of the market and discuss the collection of data. Compare diferent approaches for computing an index fund: Model (M) solved as a large integer program, Lagrangian relaxations and the subgradient approach, the linear programming approach of Section 12.3.2, or others. The index fund should be computed using an in-sample period and evaluated on an out-of-sample period. 

# Dynamic Programming Methods

## 13.1 Introduction

Decisions must often be made in a sequential manner when the information used for these decisions is revealed through time. In that case, decisions made at an earlier time may afect the feasibility and performance of later decisions. In such environments, myopic decisions that try to optimize only the impact of the current decision are usually suboptimal for the overall process. To find optimal strategies one must consider current and future decisions simultaneously. These types of multi-stage decision problems are the typical settings where one employs dynamic programming, or DP. Dynamic programming is a term used both for the modeling methodology and the solution approaches developed to solve sequential decision problems. In some cases the sequential nature of the decision process is obvious and natural, in other cases one reinterprets the original problem as a sequential decision problem. We will consider examples of both types below. 

Dynamic programming models and methods are based on Bellman’s Principle of Optimality, namely that for overall optimality in a sequential decision process, all the remaining decisions after reaching a particular state must be optimal with respect to that state. In other words, if a strategy for a sequential decision problem makes a sub-optimal decision in any one of the intermediate stages, it cannot be optimal for the overall problem. This principle allows one to formulate recursive relationships between the optimal strategies of successive decision stages and these relationships form the backbone of DP algorithms. 

Common elements of DP models include decision stages, a set of possible states in each stage, transitions from states in one stage to states in the next, value functions that measure the best possible objective values that can be achieved starting from each state, and finally the recursive relationships between value functions of diferent states. For each state in each stage, the decision maker needs to specify a decision she would make if she were to reach that state and the collection of all decisions associated with all states form the policy or strategy of the decision maker. Transitions from the states of a given stage to those of the next may happen as a result of the actions of the decision-maker, as a result of random external events, or a combination of the two. If a decision at a particular state uniquely determines the transition state, the DP is a deterministic DP. If probabilistic events also afect the transition state, then one has a stochastic DP. We will discuss each one of these terms below. 

Dynamic programming models are pervasive in the financial literature. The best-known and most common examples are the tree or lattice models (binomial, trinomial, etc.) used to describe the evolution of security prices, interest rates, volatilities, etc. and the corresponding pricing and hedging schemes. We will discuss several such examples in the next chapter. Here, we focus on the fundamentals of the dynamic programming approach and for this purpose, it is best to start with an example. 

We consider a capital budgeting problem. A manager has $ 4 million to allocate to diferent projects in three diferent regions where her company operates. In each region, there are a number of possible projects to consider with estimated costs and projected profits. Let us denote the costs with $c _ { j } \mathrm { ^ { \circ } s }$ and profits with $\mathrm { \Delta } p _ { j } \mathrm { \Delta } ^ { \circ } \mathrm { \tilde { s } }$ . The following table lists the information for possible project options; both the costs and the profits are given in millions of dollars. 

<table><tr><td rowspan="2">Project</td><td colspan="2">Region 1</td><td colspan="2">Region 2</td><td colspan="2">Region 3</td></tr><tr><td><eq>c_1</eq></td><td><eq>p_1</eq></td><td><eq>c_2</eq></td><td><eq>p_2</eq></td><td><eq>c_3</eq></td><td><eq>p_3</eq></td></tr><tr><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr><tr><td>2</td><td>1</td><td>2</td><td>1</td><td>3</td><td>1</td><td>2</td></tr><tr><td>3</td><td>2</td><td>4</td><td>3</td><td>9</td><td>2</td><td>5</td></tr><tr><td>4</td><td>4</td><td>10</td><td>—</td><td>—</td><td>—</td><td>—</td></tr></table>


Table 13.1: Project costs and profits


Note that the projects in the first row with zero costs and profits correspond to the option of doing nothing in that particular region. The manager’s objective is to maximize the total profits from projects financed in all regions. She will choose only one project from each region. 

One may be tempted to approach this problem using integer programming techniques we discussed in the previous two chapters. Indeed, since there is a one-to-one correspondence between the projects available at each region and their costs, letting $x _ { i }$ denote the investment amount in region $i ,$ we can formulate an integer programming problem with the following constraints: 

$$
\begin{array}{c} x _ {1} + x _ {2} + x _ {3} \leq 4 \\ x _ {1} \in \{0, 1, 2, 4 \}, x _ {2} \in \{0, 1, 3 \}, x _ {3} \in \{0, 1, 2 \}. \end{array}
$$

The problem with this approach is, the profits are not linear functions of the variables $x _ { i } .$ . For example, for region 3, while the last project costs twice as much as the the second one, the expected profits from this last project is only two and half times that of the second project. To avoid formulating a nonlinear integer programming problem which can be quite dificult, one might consider a formulation that uses a binary variable for each project in each region. For example, we can use binary decision variables $x _ { i j }$ to represent whether project $j$ in region i is to be financed. This results in an integer linear program but with many more variables. 

Another strategy we can consider is total enumeration of all investment possibilities. We have 4 choices for the first region, and 3 choices for each of the second and third regions. Therefore, we would end up with $4 \times 3 \times 3 = 3 6$ possibilities to consider. We can denote these possibilities with $( x _ { 1 } , x _ { 2 } , x _ { 3 } )$ where, for example, (2, 3, 1) corresponds to the choices of the second, the third and the first projects in regions 1, 2, and 3, respectively. We could evaluate each of these possibilities and then pick the best one. There are obvious problems with this approach, as well. 

First of all, for larger problems with many regions and/or many options in each region, the total number of options we need to consider will grow very quickly and become computationally prohibitive. Further, many of the combinations are not feasible with respect to the constraints of the problem. In our example, choosing the third project in each region would require $2 + 3 + 2 = 7$ million dollars, which is above the $4 million budget, and therefore is an infeasible option. In fact, only 21 of the 36 possibilities are feasible in our example. In an enumeration scheme, such infeasibilities will not be detected in advance leading to ineficiencies. Finally, an enumeration scheme does not take advantage of the information generated during the investigation of other alternatives. For example, after discovering that (3, 3, 1) is an infeasible option, we should no longer consider the more expensive (3, 3, 2) or (3, 3, 3). Unfortunately, the total enumeration scheme will not take advantage of such simple deductions. 

We will approach this problem using the dynamic programming methodology. For this purpose, we will represent our problem in a graph. The construction of this graph representation is not necessary for the solution procedure; it is provided here for didactic purposes. We will use the root node of the graph to correspond to stage 0 with $4 million to invest and use the pair $^ { ( 0 , 4 ) }$ to denote this node. In stage 1 we will consider investment possibilities in region 1. In stage 2, we will consider investment possibilities in regions 1 and 2, and finally in stage 3 we will consider all three regions. Throughout the graph, nodes will be denoted by pairs $( i , j )$ where i represents the stage and $j$ represents the particular state of that stage. States in stage i will correspond to the diferent amounts of money left after some projects are already funded in regions 1 through i. For example, the node (2,3) in stage 2 of the graph represents the state of having $3 million left for investment after funding projects in regions 1 and 2. 

The branches in the graphical representation correspond to the projects undertaken in a particular region. Say we are at node $( i , j )$ meaning that we have already considered regions 1 to i and have $j$ million dollars left for investment. Then, the branch corresponding to project $k$ in the next region will take us to the node $( i + 1 , j ^ { \prime } )$ where $j ^ { \prime }$ equals $j$ minus the cost of project k. For example, starting from node (1,3), the branch corresponding to project 2 in the second region will take us to node (2,2). For each one of these branches, we will use the expected profit from the corresponding project as the weight of the branch. The resulting graph is shown in Figure 13.1. Now the manager’s problem is to find the largest weight path from node (0,4) to a third stage node. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/50d5d327af0f266fe8528c12be070f11b549cc333c1aa9269e20bef7d3e79946.jpg)



Figure 13.1: Graphical representation of the 3-region capital budgeting problem


At this point, we can proceed in two alternative ways: using either a backward or a forward progression on the graph. In the backward mode, we first identify the largest weight path from each one of the nodes in stage 2 to a third stage node. Then using this information and the Principle of Optimality, we will determine the largest weight paths from each of the nodes in stage 1 to a third stage node, and finally from node (0,4) to a third stage node. In contrast, the forward mode will first determine the largest weight path from (0,4) to all first stage nodes, then to all second stage nodes and finally to all third stage nodes. We illustrate the backward method first and then the forward method. 

Exercise 13.1 Formulate an integer linear program for the capital budgeting problem with project costs and profits given in Table 13.1. 

## 13.1.1 Backward Recursion

For each state, or node, we keep track of the largest profit that can be collected starting from that state. These quantities form what we will call the value function associated with each state. For the backward approach, we start with stage 3 nodes. Since we are assuming that any money that is not invested in regions 1 through 3 will generate no profits, the value function for each one of the stage 3 states is zero and there are no decisions associated with these states. 

Next, we identify the largest weight paths from each one of the second stage nodes to the third stage nodes. It is clear that for nodes (2,4), (2,3), and (2,2) the best alternative is to choose project 3 of the third region and collect an expected profit of $5 million. Since node (2,1) corresponds to the state where there is only $1 million left for investment, the best alternative from the third region is project 2, with the expected profit of $2 million. For node (2,0), the only alternative is project 1 (“do nothing”) with no profit. We illustrate these choices in Figure 13.2. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/ac5d606818e314532adbbec674dbd61f23ab9316ab2b3db2ad97f407cb3ff4db.jpg)



Figure 13.2: Optimal allocations from stage 2 nodes


For each node, we indicated the value function associated with that node in a box on top of the node label in Figure 13.2. Next, we determine the value function and optimal decisions for each one of the first stage nodes. These computations are slightly more involved, but still straightforward. Let us start with node (1,4). From Figure 13.1 we see that one can reach the third stage nodes via one of (2,4), (2,3), and (2,1). The maximum expected profit on the paths through (2,4) is $0 + 5 { = } 5$ , the sum of the profit on the arc from (1,4) to (2,4), which is zero, and the largest profit from (2,4) to a period 3 node. Similarly, we compute the maximum expected profit on the paths through (2,3) and (2,1) to be $3 + 5 { = } 8 .$ , and $9 + 2 { = } 1 1$ . The maximum profit from (1,4) to a stage three node is then 

$$
\max \{0 + v (2, 4), 3 + v (2, 3), 9 + v (2, 1) \} = \{0 + 5, 3 + 5, 9 + 2 \} = 1 1
$$

which is achieved by following the path $( 1 , 4 )  ( 2 , 1 )  ( 3 , 0 )$ . After performing similar computations for all period 1 nodes we obtain the node values and optimal branches given in Figure 13.3. 

Finally, we need to compute the best allocations from node (0,4) by comparing the profits along the branches to first stage nodes and the best possible profits starting from those first period nodes. To be exact, we compute 

$$
\max \{0 + v (1, 4), 2 + v (1, 3), 4 + v (1, 2), 1 0 + v (1, 0) \} = \{0 + 1 1, 2 + 9, 4 + 5, 1 0 + 0 \} = 1 1.
$$

Therefore, the optimal expected profit is $11 million and is achieved on either of the two alternative paths $( 0 , 4 )  ( 1 , 4 )  ( 2 , 1 )  ( 3 , 0 )$ and $( 0 , 4 )  ( 1 , 3 )  ( 2 , 0 )  ( 3 , 0 )$ . These paths correspond to the selections of project 1 in region 1, project 3 in region 2, and project 2 in region 3 in the first case, and project 2 in region 1, project 3 in region 2, and project 1 in region 3 in the second case. Figure 13.4 summarizes the whole process. The optimal paths are shown using thicker lines. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/cc755eca3597e977d713d46a9d00976298c794913d03430824027f9ff64f16f4.jpg)



Figure 13.3: Optimal allocations from stage 1 nodes


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/705eff139bff4d443a898fd39e76a4e63844c98513c72138eb19160e4b89d788.jpg)



Figure 13.4: Optimal paths from (0,4) to (3,0)


Exercise 13.2 Construct a graphical representation of a 5-region capital budgeting problem with the project costs and profits given in Table 13.2. Exactly one project must be chosen in each region and there is a total budget of 10. Solve by backward recursion. 

<table><tr><td rowspan="2">Project</td><td colspan="2">Region 1</td><td colspan="2">Region 2</td><td colspan="2">Region 3</td><td colspan="2">Region 4</td><td colspan="2">Region 5</td></tr><tr><td><eq>c_1</eq></td><td><eq>p_1</eq></td><td><eq>c_2</eq></td><td><eq>p_2</eq></td><td><eq>c_3</eq></td><td><eq>p_3</eq></td><td><eq>c_4</eq></td><td><eq>p_4</eq></td><td><eq>c_5</eq></td><td><eq>p_5</eq></td></tr><tr><td>1</td><td>1</td><td>8</td><td>3</td><td>20</td><td>2</td><td>15</td><td>0</td><td>3</td><td>1</td><td>6</td></tr><tr><td>2</td><td>2</td><td>15</td><td>2</td><td>14</td><td>4</td><td>26</td><td>1</td><td>10</td><td>2</td><td>15</td></tr><tr><td>3</td><td>3</td><td>25</td><td>1</td><td>7</td><td>5</td><td>40</td><td>3</td><td>25</td><td>3</td><td>22</td></tr></table>


Table 13.2: Project costs and profits


## 13.1.2 Forward Recursion

Next, we explore the “forward” method. In this case, in the first step we will identify the best paths from (0, 4) to all nodes in stage 1, then best paths from (0, 4) to all stage 2 nodes, and finally to stage 3 nodes. The first step is easy since there is only one way to get from node (0, 4) to each one of the stage 1 nodes, and hence all these paths are optimal. Similar to the backward method, we will keep track of a value function for each node. For node (i, j), its value function will represent the highest total expected profit we can collect from investments in regions 1 through i if we want to have $j million left for future investment. For (0, 4) the value function is zero and for all stage 1 nodes, they are equal to the weight of the tree branch that connects (0, 4) and the corresponding node. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/f5e1a6a2e6d4de4645797c8fc22461acbda0bd50012696f3874e8830df904440.jpg)



Figure 13.5: Optimal paths between stage 0, stage 1 and stage 2 nodes


For most of the second stage nodes, there are multiple paths from (0, 4) to that corresponding node and we need to determine the best option. For example, let us consider the node (2, 2). One can reach (2, 2) from (0, 4) either via (1, 3) or (1, 2). The value function at (2, 2) is the maximum of the following two quantities: The sum of the value function at (1, 3) and the weight of the branch from (1, 3) to (2, 2), and, the sum of the value function at (1, 2) and the weight of the branch from (1, 2) to (2, 2): 

$$
v (2, 2) = \max \{v (1, 3) + 3, v (1, 2) + 0 \} = \max \{2 + 3, 4 + 0 \} = 5.
$$

After similar calculations we identify the value function at all stage 2 nodes and the corresponding optimal branches one must follow. The results are shown on the right side of Figure 13.5. 

Finally, we perform similar calculations for stage 3 nodes. For example, we can calculate the value function at (3, 0) as follows: 

$$
v (3, 0) = \max \{v (2, 2) + 5, v (2, 1) + 2, v (2, 0) + 0 \} = \{5 + 5, 9 + 2, 1 1 + 0 \} = 1 1.
$$

Optimal paths for all nodes are depicted in Figure 13.6. Note that there are three alternative optimal ways to reach node (3, 2) from (0, 4). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/5fad0b981aab30fb91ae310d7167d4f8c0ea66afd852deac8a4a8c46e514da86.jpg)



Figure 13.6: Optimal paths from (0,4) to all nodes


Clearly, both the forward and the backward method identified the two alternative optimal paths between (0, 4) and (3, 0). However, the additional information generated by these two methods difer. In particular, studying Figures 13.4 and 13.6, we observe that while the backward method produces the optimal paths from each node in the tree to the final stage nodes, in contrast, the forward method produces the optimal paths from the initial stage node to all nodes in the tree. There may be situations where one prefers to have one set of information above the other and this preference dictates which method to use. For example, if for some reason the actual transition state happens to be diferent from the one intended by an optimal decision, it would be important to know what to do when in a state that is not on the optimal path. In that case, the paths generated by the backward method would have the answer. 

Exercise 13.3 Solve the capital budgeting problem of Exercise 13.2 by forward recursion. 

## 13.2 Abstraction of the Dynamic Programming Approach

Before proceeding with additional examples, we study the common characteristics of dynamic programming models and methods. In particular, we will identify the aspects of the example considered in the previous section that qualified our approach as dynamic programming. 

We already mentioned the sequential nature of the decision-making process as the most important ingredient of a DP problem. Every DP model starts with the identification of stages that correspond to the order of the decisions to be made. There is an initial stage (for a forward recursion) or final stage (for a backward recursion) for which the optimal decisions are immediately or easily available and do not depend on decisions of other stages. In our example in Section 13.1, the number of regions considered for diferent project options constituted the stages of our formulation. Stage 0 was the initial stage and stage 3 the final stage. 

Each stage consists of a number of possible states. In allocation problems, states are typically used to represent the possible levels of availability for scarce resources in each stage. In financial binomial lattice models, states may correspond to spot prices of assets. 

In many cases, the set of states in each particular stage is finite or at least, discrete. Such DPs are categorized as discrete $D P s$ in contrast to continuous $D P s$ that may have a continuum of states in each stage. In the example of Section 13.1, the states represented the amount of money still available for investment at the end of that particular stage. For consistency with our earlier example, we continue to denote states of a DP formulation with the pair $( i , j )$ where i specifies the stage and j specifies the particular state in that stage. 

A DP formulation must also specify a decision set for each one of the states. As with states, decision sets may be discrete or continuous. In our example in Section 13.1, the decision sets were formed from the set of possible projects in each stage. Because of feasibility considerations, decision sets are not necessarily identical for all states in a given stage. For example, while the decision set consists of region 2 projects 1, 2, and 3 for state $( 1 , 4 )$ ， the decision set for state $( 1 , 0 )$ is the singleton corresponding to project 1 (do nothing). We denote the decision set associated with state $( i , j )$ with $\mathcal { S } ( i , j )$ 

In a deterministic DP, a choice d made from the decision set $\mathcal { S } ( i , j )$ uniquely determines what state one transitions to. We call this state the transition state associated with the particular state $( i , j )$ and decision $d \in$ $\mathcal { S } ( i , j )$ and use the notation $T \left( ( i , j ) , d \right)$ to denote this state. Furthermore, there is a cost (or benefit, for a maximization problem) associated with each transition that we indicate with $c ( ( i , j ) , d )$ . In our example in the previous section, from state $( 2 , 1 )$ , we can either transition to state (3, 1) by choosing project 1 with an associated profit of 0, or to state (3, 0) by choosing project 2 with an associated profit of 2. 

In our example above, all the transition states from a given state were among the states of the next stage. Although this is common, it is not required. All that is necessary for the DP method to function is that all the transition states from a given state are in the later stages whose computations are already completed. So, for example, in a five stage formulation, transition states of a state in stage 2 can be in any one of stages 3, 4, and 5. 

A value function keeps track of the costs (or benefits) accumulated optimally from the initial stage up to a particular state (in the forward method) or from a particular state to the final stage (in the backward method). Each such quantity will be called the value of the corresponding state. We use the notation $v ( i , j )$ to denote the value of the state $( i , j )$ 

The Principle of Optimality implies a recursive relationship between the values of states in consecutive stages. For example, in the backward method, to compute the optimal decision at and the value of a particular state, all we need to do is to compare the following quantity for each transition state of that state: the value of the transition state plus the cost of transitioning to that state. Namely, we do the following computation: 

$$
v (i, j) = \min _ {d \in \mathcal {S} (i, j)} \left\{v \left(T ((i, j), d)\right) + c ((i, j), d) \right\}.\tag{13.1}
$$

In a benefit maximization problem as in our example in the previous section, the values would be the benefits rather than costs and the min in (13.1) would be replaced by a max. Equation (13.1) is known as the Bellman equation and is a discrete-time deterministic special case of the Hamilton-Jacobi-Bellman (HJB) equation often encountered in optimal control texts. 

To illustrate the definitions above and equation (13.1), let us explicitly perform one of the calculations of the example in the previous section. Say, in the backward method we have already calculated the values of the states in stage 2 (5, 5, 5, 2, and 0, for states $( 2 , 4 ) , ( 2 , 3 ) , ( 2 , 2 ) , ( 2 , 1 )$ , and (2,0), respectively) and we intend to compute the value of the state (1,3). We first identify the decision set for $( 1 , 3 ) \colon S ( 1 , 3 ) = \{ 1 , 2 , 3 \}$ , i.e., projects 1, 2, and 3. The corresponding transition states are easily determined: 

$$
T ((1, 3), 1) = (2, 3), \quad T ((1, 3), 2) = (2, 2), \quad T ((1, 3), 3) = (2, 0).
$$

The associated benefits (or expected profits, in this case) are 

$$
c ((1, 3), 1) = 0, c ((1, 3), 2) = 3, c ((1, 3), 3) = 9.
$$

Now we can derive the value of state (1,3): 

$$
\begin{array}{r c l}v (1, 3)&=&\max _ {d \in \mathcal {S} (1, 3)} \left\{ \right.v \left( \right.T \left((1, 3), d)\right) + c \left((1, 3), d\right)\left. \right\}\\&=&\max \{v \left( \right.T \left((1, 3), 1)\right) + c \left((1, 3), 1\right), v \left(T \left((1, 3), 2)\right) + c \left((1, 3), 2\right), \right.\\&&\dots v \left(T \left((1, 3), 3)\right) + c \left((1, 3), 3\right) \right\}\\&=&\max \{v (2, 3) + 0, v (2, 2) + 3, v (2, 0) + 9 \}\\&=&\max \{5 + 0, 5 + 3, 0 + 9 \} = 9,\end{array}
$$

and the corresponding optimal decision at (1,3) is project 3. Note that for us to be able to compute the values recursively as above, we must be able to compute the values at the final stage without any recursion. 

If a given optimization problem can be formulated with the ingredients and properties outlined above, we can solve it using dynamic programming methods. Most often, finding the right formulation of a given problem, and specifying the stages, states, transitions, and recursions in a way that fits the framework above is the most challenging task in the dynamic programming approach. Even when a problem admits a DP formulation, there may be several alternative ways to do this (see, for example, Section 13.3) and it may not be clear which of these formulations would produce the quickest computational scheme. Developing the best formulations for a given optimization problem must be regarded as a form of art and in our opinion, is best learned through examples. We continue in the next section with a canonical example of both integer and dynamic programming. 

## 13.3 The Knapsack Problem.

A traveler has a knapsack that she plans to take along for an expedition. Each item she would like to take with her in the knapsack has a given size and a value associated with the benefit the traveler receives by carrying that item. Given that the knapsack has a fixed and finite capacity, how many of each of these items should she put in the knapsack to maximize the total value of the items in the knapsack? This is the well-known and well-studied integer program called the knapsack problem. It has the special property that it only has a single constraint other than the nonnegative integrality condition on the variables. 

We recall the investment problem considered in Exercise 11.5 in Chapter 11 which is an instance of the knapsack problem. We have $14,000 to invest among four diferent investment opportunities. Investment 1 requires an investment of $7,000 and has a net present value of $11,000; investment 2 requires $5,000 and has a value of $8,000; investment 3 requires $4,000 and has a value of $6,000; and investment 4 requires $3,000 and has a value of $4,000. 

As we discussed in Chapter 11, this problem can be formulated and solved as an integer program, say using the branch and bound method. Here, we will formulate it using the DP approach. To make things a bit more interesting, we will allow the possibility of multiple investments in the same investment opportunity. The efect of this modification is that the variables are now general integer variables rather than 0–1 binary variables and therefore the problem 

$$
\begin{array}{c} \text {Max} 1 1 x _ {1} + 8 x _ {2} + 6 x _ {3} + 4 x _ {4} \\ 7 x _ {1} + 5 x _ {2} + 4 x _ {3} + 3 x _ {4} \leq 1 4 \\ x _ {j} \geq 0 \text {an integer,} \forall j \end{array}
$$

is an instance of the knapsack problem. We will consider two alternative DP formulations of this problem. For future reference, let $y _ { j }$ and $p _ { j }$ denote the cost and the net present value of investment $j$ (in thousands of dollars), respectively, for $j = 1$ to 4. 

## 13.3.1 Dynamic Programming Formulation

One way to approach this problem using the dynamic programming methodology is by considering the following question that already suggests a recursion: If I already know how to allocate i thousand dollars to the investment options optimally for all $i = 1 , \ldots , k - 1$ , can I determine how to optimally allocate k thousand dollars to these investment option? The answer to this question is yes, and building the recursion equation is straightforward. 

The first element of our DP construction is the determination of the stages. The question in the previous paragraph suggests the use of stages $0 , 1 , . . . ,$ up to 14, where stage i corresponds to the decisions that need to be made with $j$ thousand dollars left to invest. Note that we need only one state per stage and therefore can denote stages/states using the single index i. The decision set at state j is the set of investments we can aford with the $j$ thousand dollars we have left for investment. That is, $S ( i ) = \{ d : y _ { d } \leq i \}$ The transition state is given by $T ( i , d ) = i - y _ { d }$ and the benefit associated with the transition is $c ( i , d ) = p _ { d }$ . Therefore, the recursion for the value function is given by the following equation: 

$$
v (i) = \max _ {d: y _ {d} \leq i} \{v (i - y _ {d}) + p _ {d} \}.
$$

Note that $S ( i ) = \emptyset$ and v(i) = 0 for i = 0, 1, and 2 in our example. 

Exercise 13.4 Using the recursion given above, determine $v ( i )$ for all i from 0 to 14 and the corresponding optimal decisions. 

## 13.3.2 An Alternative Formulation

As we discussed in Section 13.2, dynamic programming formulation of a given optimization problem need not be unique. Often, there exists alternative ways of defining the stages, states, and obtaining recursions. Here we develop an alternative formulation of our investment problem by choosing stages to correspond to each one of the investment possibilities. 

So, we will have four stages, $i = 1 , 2 , 3$ , and 4. For each stage i, we will have states $j$ corresponding to the total investment in opportunities i through 4. So, for example, in the fourth stage we will have states (4,0), (4,3), (4,6), (4,9), and (4,12), corresponding to 0, 1, 2, 3, and 4 investments in the fourth opportunity. 

The decision to be made at stage i is the number of times one invests in the investment opportunity i. Therefore, for state $( i , j )$ , the decision set is given by 

$$
\mathcal {S} (i, j) = \{d | \frac {j}{y _ {i}} \geq d, d \text {   non - negative   integer } \}.
$$

The transition states are given by $T \left( ( i , j ) , d \right) = ( i + 1 , j - y _ { i } d )$ and the value function recursion is: 

$$
v (i, j) = \max _ {d \in \mathcal {S} (i, j)} \left\{v (i + 1, j - y _ {i} d) + p _ {i} d \right\}.
$$

Finally, note that $v ( 4 , 3 k ) = 4 k$ for k = 0, 1,2,3, and 4. 

Exercise 13.5 Using the DP formulation given above, determine $v ( 0 , 1 4 )$ and the corresponding optimal decisions. Compare your results with the optimal decisions from Exercise 13.4. 

Exercise 13.6 Formulate a dynamic programming recursion for the following shortest path problem. City O (the origin) is in Stage 0, one can go from any city i in Stage $k - 1$ to any city $j$ in Stage k for $k = 1 , \dots N$ . The distance between such cities i and $j$ is denoted by $d _ { i j }$ . City D (the destination) is in Stage N. The goal is to find a shortest path from the origin O to the destination D. 

## 13.4 Stochastic Dynamic Programming

So far, we have only considered dynamic programming models that are deterministic, meaning that given a particular state and a decision from its decision set, the transition state is known and unique. This is not always the case for optimization problems involving uncertainty. Consider a blackjack player trying to maximize his earnings by choosing a strategy or a commuter trying to minimize her commute time by picking the roads to take. Suppose the blackjack player currently holds 12 (his current “state”) and asks for another card (his “decision”). His next state may be a “win” if he gets a 9, a “lose” if he gets a 10, or “15 (and keep playing)” if he gets a 3. The state he ends up in depends on the card he receives, which is beyond his control. Similarly, the commuter may choose Road 1 over Road 2, but her actual commute time will depend on the current level of congestion on the road she picks, a quantity beyond her control. 

Stochastic dynamic programming addresses optimization problems with uncertainty. The DP methodology we discussed above must be modified to incorporate uncertainty. This is done by allowing multiple transition states for a given state and decision. Each one of the possible transition states is assigned a probability associated with the likelihood of the corresponding state being reached when a certain decision is made. Since the costs are not certain anymore, the value function calculations and optimal decisions will be based on expected values. 

We have the following formalization: Stages and states are defined as before, and a decision set associated with each state. Given a state $( i , j )$ and d $\in \mathcal { S } ( i , j )$ , a random event will determine the transition state. We denote with $\mathcal { R } \left( ( i , j ) , d \right)$ the set of possible outcomes of the random event when we make decision d at state $( i , j )$ . For each possible outcome $r \in \mathcal { R } \left( ( i , j ) , d \right)$ we denote the likelihood of that outcome with $p \left( ( i , j ) , d , r \right)$ . We observe that the probabilities $p \left( ( i , j ) , d , r \right)$ must be nonnegative and satisfy 

$$
\sum_ {r \in \mathcal {R} ((i, j), d)} p \left((i, j), d, r\right) = 1, \forall (i, j) \text { and } \forall d \in \mathcal {S} (i, j).
$$

When we make decision d at state $( i , j )$ and when the random outcome r is realized, we transition to the state $T ( ( i , j ) , d , r )$ and the cost (or benefit) associated with this transition is denoted by $c \left( ( i , j ) , d , r \right)$ . The value function $v ( i , j )$ computes expected value of the costs accumulated and must satisfy the following recursion: 

$$
v (i, j) = \min _ {d \in \mathcal {S} (i, j)} \left\{\sum_ {r \in \mathcal {R} ((i, j), d)} p ((i, j), d, r) [ v (T ((i, j), d, r)) + c ((i, j), d, (1) ]. 2) \right.
$$

As before, in a benefit maximization problem, the min in (13.2) must be replaced by a max. 

In some problems, the uncertainty is only in the transition costs and not in the transition states. Such problems can be handled in our notation above by letting $\mathcal { R } \left( ( i , j ) , d \right)$ correspond to the possible outcomes for the cost of the transition. The transition state is independent from the random event, that is $T \left( ( i , j ) , d , r _ { 1 } \right) = T \left( ( i , j ) , d , r _ { 2 } \right)$ for all $r _ { 1 } , r _ { 2 } \in \mathcal { R } \left( ( i , j ) , d \right)$ . The cost function $c \left( ( i , j ) , d , r \right)$ reflects the uncertainty in the problem. 

Exercise 13.7 Recall the investment problem we discussed in Section 13.3. We have $14,000 to invest in four diferent options which cost $y _ { j }$ thousand dollars for $j = 1 \mathrm { ~ t o ~ } 4$ Here we introduce the element of uncertainty to the problem. While the cost of investment $j$ is fixed at $y _ { j }$ (all quantities in thousands of dollars), its net present value is uncertain because of the uncertainty of future cash-flows and interest rates. We believe that the net present value of investment $j$ has a discrete uniform distribution in the set $\{ p _ { j } - 2 , p _ { j } - 1 , p _ { j } , p _ { j } + 1 , p _ { j } + 2 \}$ . We want to invest in these investment options in order to maximize the expected net present value of our investments. Develop a stochastic DP formulation of this problem and solve it using the recursion (13.2). 

## Chapter 14

# DP Models: Option Pricing

The most common use of dynamic programming models and principles in financial mathematics is through the lattice models. The binomial lattice has become an indispensable tool for pricing and hedging of derivative securities. We study the binomial lattice in Section 14.2 below. Before we do that, however, we will show how the dynamic programming principles lead to optimal exercise decisions in a more general model than the binomial lattice. 

## 14.1 A Model for American Options

For a given stock, let $S _ { k }$ denote its price on day k. We can write 

$$
S _ {k} = S _ {k - 1} + X _ {k}
$$

where $X _ { k }$ is the change in price from day k 1 to day k. The random walk model for stock prices assumes that the random variables $X _ { k }$ are independent and identically distributed, and are also independent of the known initial price $S _ { 0 }$ . We will also assume that the distribution F of $X _ { k }$ has a finite mean $\mu .$ . 

Now consider an American call option on this stock: Purchasing such an option entitles us to buy the stock at a fixed price c on any day between today (let us call it day 0) and day N, when the option expires. We do not have to ever exercise the option, but if we do at a time when the stock price is S, then our profit is $S - c$ . What exercise strategy maximizes our expected profit? We assume that the interest rate is zero throughout the life of the option for simplicity. 

Let $v ( k , S )$ denote the maximum expected profit when the stock price is S and the option has k additional days before expiration. In our dynamic programming terminology, the stages are $k = 0 , 1 , 2 , \ldots , N$ and the state in each stage is $S ,$ the current stock price. Note that stage 0 corresponds to day N and vice versa. In contrast to the DP examples we considered in the previous chapter, we do not assume that the state space is finite in this model. That is, we are considering a continuous DP here, not a discrete DP. The decision set for each state has two elements, namely “exercise” or “do not exercise”. The “exercise” decision takes one to the transition state “option exercised” which should be placed at stage N for convenience. The immediate benefit from the “exercise” decision is $S - c .$ If we “do not exercise” the option in stage $k ,$ we hold the option for at least one more period and observe the random shock x to the stock price which takes us to state $S + x$ in stage $k - 1$ 

Given this formulation, our value function $v ( k , S )$ satisfies the following recursion: 

$$
v (k, S) = \max \{S - c, \int v (k - 1, S + x) d F (x) \}
$$

with the boundary condition 

$$
v (0, S) = \max \{S - c, 0 \}.
$$

For the case that we are considering (American call options), there is no closed form formula for $v ( k , S )$ . However dynamic programming can be used to compute a numerical solution. In the remainder of this section, we use the recursion formula to derive the structure of the optimal policy. 

Exercise 14.1 Using induction on k, show that $v ( k , S ) - S$ is a nonincreasing function of S. 

Solution The fact that $v ( 0 , S ) - S$ is a nonincreasing function of S follows from the definition of $v ( 0 , S )$ . Assume now $v ( k - 1 , S ) - S$ is a nonincreasing function of S. Using the recursion equation, we get 

$$
\begin{array}{r c l} v (k, S) - S & = & \max \{- c, \int (v (k - 1, S + x) - S)   d F (x) \} \\ & = & \max \{- c, \int (v (k - 1, S + x) - (S + x))   d F (x) + \int x d F (x) \} \\ & = & \max \{- c, \mu + \int (v (k - 1, S + x) - (S + x))   d F (x) \}, \end{array}
$$

recalling that $\textstyle \mu = \int x d F ( x )$ denotes the expected value of the random variable x representing daily shocks to the stock price. 

For any x, the function $v ( k - 1 , S + x ) - ( S + x )$ is a nonincreasing function of $S ,$ by the induction hypothesis. It follows that $v ( k , S ) - S$ is a nonincreasing function of S. End of solution. 

Theorem 14.1 The optimal policy for an American call option has the following form: 

There are nondecreasing numbers $s _ { 1 } \leq s _ { 2 } \leq . . . \leq s _ { k } \leq . . . s _ { N }$ such that, if the current stock price is $S$ and there are k days until expiration, then one should exercise the option if and only if $S \geq s _ { k }$ 

## Proof:

It follows from the recursion equation that if $v ( k , S ) \leq S - c ,$ then it is optimal to exercise the option when the stock price is S and there remain k days until expiration. Indeed this yields $v ( k , S ) = S - c ,$ which is the maximum possible under the above assumption. Define 

$$
s _ {k} = \min \{S: v (k, S) = S - c \}.
$$

If no S satisfies $v ( k , S ) = S - c .$ , then $s _ { k }$ is defined as $+ \infty$ . From the exercise above, it follows that 

$$
v (k, S) - S \leq v (k, s _ {k}) - s _ {k} = - c
$$

for any $s \geq s _ { k }$ since $v ( k , S ) - S$ is nonincreasing. Therefore it is optimal to exercise the option with k days to expiration whenever $S \geq s _ { k }$ . Since $v ( k , S )$ is nondecreasing in $k ,$ , it immediately follows that $s _ { k }$ is also nondecreasing in $k , { \mathrm { i . e . , ~ } } s _ { 1 } \leq s _ { 2 } \leq . . . \leq s _ { k } \leq . . . s _ { N }$ 

A consequence of the above result is that, when $\mu > 0$ , it is always optimal to wait until the maturity date to exercise an American call option. The optimal policy described above becomes nontrivial when $\mu < 0$ however. 

Exercise 14.2 A put option is an agreement to sell an asset for a fixed price c (the strike price). An American put option can be exercised at any time up to the maturity date. Prove a Theorem similar to Theorem 14.1 for American put options. Can you deduce that it is optimal to wait until maturity to exercise a put option when $\mu > 0 ?$ 

## 14.2 Binomial Lattice

If we want to buy or sell an option on an asset (whether a call or a put, an American, European, or another type of option), it is important to determine the fair value of the option today. Determining this fair value is called option pricing. The option price depends on the structure of the movements in the price of the underlying asset using information such as the volatility of the underlying asset, the current value of the asset, the dividends if any, the strike price, the time to maturity and the riskless interest rate. Several approaches can be used to determine the option price. One popular approach uses dynamic programming on a binomial lattice that models the price movements of the underlying asset. Our discussion here is based on the work of Cox, Ross, and Rubinstein [23]. 

In the binomial lattice model, a basic period length is used, such as a day or a week. If the price of the asset is S in a period, the asset price can only take two values in the next period. Usually, these two possibilities are represented as $u S$ and $d S$ where $u > 1$ and $d < 1$ are multiplicative factors (u stands for up and d for down). The probabilities assigned to these possibilities are p and $1 - p$ respectively, where $0 < p < 1$ . This can be represented on a lattice (see Figure 14.1). 

After several periods, the asset price can take many diferent values. Starting from price $S _ { 0 }$ in period 0, the price in period k is $u ^ { j } d ^ { k - j } S _ { 0 }$ if there are $j$ up moves and $k - j$ down moves. The probability of an up move is $p$ whereas that of a down move is $1 - p$ and there are $\textstyle { \binom { k } { j } }$ possible paths to reach the corresponding node. Therefore the probability that the price is $u ^ { j } d ^ { k - j } S _ { 0 }$ in period k is ${ \binom { k } { j } } p ^ { j } ( 1 - p ) ^ { k - j }$ . This is the binomial distribution.   <sub>As k increases, this distribution converges to the normal distribution.</sub> 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/4d092f42a7c96e1d7e4edb6ffbb9fb2a6c70201a05b13e665a2753814da8343c.jpg)



Figure 14.1: Asset price in the binomial lattice model


## 14.2.1 Specifying the parameters

To specify the model completely, one needs to choose values for $u ,$ d and $p .$ This is done by matching the mean and volatility of the asset price to the mean and volatility of the above binomial distribution. Because the model is multiplicative (the price $S$ of the asset being either $u S$ or $d S$ in the next period), it is convenient to work with logarithms. 

Let $S _ { k }$ denote the asset price in periods $k = 0 , \ldots , n$ . Let $\mu$ and $\sigma$ be the mean and volatility of ln $( S _ { n } / S _ { 0 } )$ (we assume that this information about the asset is known). Let $\begin{array} { r } { \Delta = \frac { 1 } { n } } \end{array}$ denote the length between consecutive periods. Then the mean and volatility of $\ln ( S _ { 1 } / S _ { 0 } )$ are $\mu \Delta$ and $\sigma \sqrt { \Delta }$ respectively. In the binomial lattice, we get by direct computation that the mean and variance of ln $( S _ { 1 } / S _ { 0 } )$ are $p$ ln $u + ( 1 - p )$ ln d and $p ( 1 - p ) \iota$ (ln u ln $d ) ^ { 2 }$ respectively. Matching these values we get two equations: 

$$
\begin{array}{r c l} {p \ln u + (1 - p) \ln d} & = & {\mu \Delta} \\ {p (1 - p) (\ln u - \ln d) ^ {2}} & = & {\sigma^ {2} \Delta .} \end{array}
$$

Note that there are three parameters but only two equations, so we can set $d = 1 / u$ as in [23]. Then the equations simplify to 

$$
\begin{array}{r c l} (2 p - 1) \ln u & = & \mu \Delta \\ 4 p (1 - p) (\ln u) ^ {2} & = & \sigma^ {2} \Delta . \end{array}
$$

Squaring the first and adding it to the second, we get $( \ln u ) ^ { 2 } = \sigma ^ { 2 } \Delta + ( \mu \Delta ) ^ { 2 }$ This yields 

$$
\begin{array}{r c l} {u} & {=} & {e ^ {\sqrt {\sigma^ {2} \Delta + (\mu \Delta) ^ {2}}}} \\ {d} & {=} & {e ^ {- \sqrt {\sigma^ {2} \Delta + (\mu \Delta) ^ {2}}}} \\ {p} & {=} & {\frac {1}{2} (1 + \frac {1}{\sqrt {1 + \frac {\sigma^ {2}}{\mu^ {2} \Delta}}}).} \end{array}
$$

When $\Delta$ is small, these values can be approximated as 

$$
\begin{array}{r c l} {u} & {=} & {e ^ {\sigma \sqrt {\Delta}}} \\ {d} & {=} & {e ^ {- \sigma \sqrt {\Delta}}} \\ {p} & {=} & {\frac {1}{2} (1 + \frac {\mu}{\sigma} \sqrt {\Delta}).} \end{array}
$$

As an example, consider a binomial model with 52 periods of a week each. Consider a stock with current known price $S _ { 0 }$ and random price $S _ { 5 2 }$ a year from today. We are given the mean $\mu$ and volatility $\sigma$ of ln $( S _ { 5 2 } / S _ { 0 } )$ , say $\mu = 1 0 \%$ and $\sigma = 3 0 \%$ . What are the parameters $u ,$ d and $p$ of the binomial lattice? Since $\begin{array} { r } { \Delta = \frac { 1 } { 5 2 } } \end{array}$ is small, we can use the second set of formulas: 

$$
u = e ^ {0. 3 0 / \sqrt {5 2}} = 1. 0 4 2 5 \quad \mathrm{and} \quad d = e ^ {- 0. 3 0 / \sqrt {5 2}} = 0. 9 5 9 2
$$

$$
p = \frac {1}{2} (1 + \frac {0 . 1 0}{0 . 3 0 \sqrt {5 2}}) = 0. 5 2 3
$$

## 14.2.2 Option Pricing

Using the binomial lattice described above for the price process of the underlying asset, the value of an option on this asset can be computed by dynamic programming, using backward recursion, working from the maturity date $T$ (period n) back to period 0 (the current period). The stages of the dynamic program are the periods $k = 0 , \ldots , N$ and the states are the nodes of the lattice in a given period. Thus there are $k + 1$ states in stage $k ,$ which we label $j = 0 , \ldots , k$ . The nodes in stage N are called the terminal nodes. ¿From a nonterminal node $j ,$ , we can go either to node $j + 1$ (up move) or to node $j$ (down move) in the next stage. ${ \mathrm { S o } } ,$ to reach node $j$ at stage k we must make exactly j up moves, and $k - j$ down moves between stage $0$ and stage $k .$ 

We denote by $v ( k , j )$ the value of the option in node $j$ of stage $k .$ . The value of the option at time 0 is then given by $v ( 0 , 0 )$ . This is the quantity we have to compute in order to solve the option pricing problem. 

The option values at maturity are simply given by the payof formulas, $\mathrm { i . e . , } \operatorname* { m a x } ( S - c , 0 )$ for call options and max $( c - S , 0 )$ for put options, where c denotes the strike price and $S$ is the asset price at maturity. Recall that, in our binomial lattice after $N$ time steps, the asset price in node $j$ is $u ^ { j } d ^ { N - j } S _ { 0 }$ Therefore the option values in the terminal nodes are: 

$$
v (N, j) = \max (u ^ {j} d ^ {N - j} S _ {0} - c, 0) \quad \mathrm{forcalloptions},
$$

$$
v (N, j) = \max (c - u ^ {j} d ^ {N - j} S _ {0}, 0) \quad \mathrm{forputoptions.}
$$

We can compute $v ( k , j )$ knowing $v ( k + 1 , j )$ and $v ( k + 1 , j + 1 )$ . Recall (Section 4.1.1) that this is done using the risk neutral probabilities 

$$
p _ {u} = \frac {R - d}{u - d} \quad \mathrm{and} \quad p _ {d} = \frac {u - R}{u - d}.
$$

where $R = 1 + r$ and $r$ is the one-period return on the risk-free asset. For European options, the value of $f _ { k } ( j )$ is 

$$
v (k, j) = \frac {1}{R} \left(p _ {u} v (k + 1, j + 1) + p _ {d} v (k + 1, j)\right).
$$

For an American call option, we have 

$$
v (k, j) = \max \left\{\frac {1}{R} \left(p _ {u} v (k + 1, j + 1) + p _ {d} v (k + 1, j)\right), u ^ {j} d ^ {k - j} S _ {0} - c \right\}
$$

and for an American put option, we have 

$$
v (k, j) = \max \{\frac {1}{R} \left(p _ {u} v (k + 1, j + 1) + p _ {d} v (k + 1, j)\right), c - u ^ {j} d ^ {k - j} S _ {0} \}.
$$

Let us illustrate the approach. We wish to compute the value of an American put option on a stock. The current stock price is $100. The strike price is $98 and the expiration date is 4 weeks from today. The yearly volatility of the logarithm of the stock return is $\sigma = 0 . 3 0$ . The risk-free interest rate is 4 %. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/f76b3ee8e8846963b0448fdb4f72200e5797821b13a83a8a5237d7c4837f140c.jpg)



Figure 14.2: Put option pricing in a binomial lattice


We consider a binomial lattice with $N = 4 ;$ see Figure 14.2. To get an accurate answer one would need to take a much larger value of N. Here the purpose is just to illustrate the dynamic programming recursion and $N = 4$ will sufice for this purpose. We recall the values of u and d computed in the previous section: 

$$
u = 1. 0 4 2 5 \quad \mathrm{and} \quad d = 0. 9 5 9 2
$$

In period $N = 4$ , the stock price in node $j$ is given by $u ^ { j } d ^ { 4 - j } S _ { 0 } = 1 . 0 4 2 5 ^ { j } 0 . 9 5 9 2 ^ { 4 - j } 1 0 0$ and therefore the put option payof is given by: 

$$
v (4, j) = \max (9 8 - 1. 0 4 2 5 ^ {j} 0. 9 5 9 2 ^ {4 - j} 1 0 0, 0).
$$

That is $v ( 4 , 0 ) = 1 3 . 3 3 , v ( 4 , 1 ) = 5 . 9 9 \mathrm { a n d } v ( 4 , 2 ) = v ( 4 , 3 ) = v ( 4 , 4 ) = 0 .$ Next, we compute the stock price in period $k = 3$ . The one-period return on the risk-free asset is $\begin{array} { r } { r = \frac { 0 . 0 4 } { 5 2 } = 0 . 0 0 0 7 7 } \end{array}$ and thus $R = 1 . 0 0 0 7 7 .$ 

Accordingly, the risk neutral probabilities are 

$$
p _ {u} = \frac {1 . 0 0 0 7 7 - 0 . 9 5 9 2}{1 . 0 4 2 5 - 0 . 9 5 9 2} = 0. 4 9 9, \mathrm{and} p _ {d} = \frac {1 . 0 4 2 5 - 1 . 0 0 0 7 7}{1 . 0 4 2 5 - 0 . 9 5 9 2} = 0. 5 0 1.
$$

We deduce that, in period 3, the stock price in node $j$ is 

$$
v (3, j) = \max \{\frac {1}{1 . 0 0 0 7 7} (0. 4 9 9 v (4, j + 1) + 0. 5 0 1 v (4, j)), 9 8 - 1. 0 4 2 5 ^ {j} 0. 9 5 9 2 ^ {3 - j} 1 0 0 \}.
$$

That is $v ( 3 , 0 ) = \mathrm { { m a x } } \{ 9 . 6 7 , 9 . 7 4 \} = 9 . 7 4$ (as a side remark, note that it is optimal to exercise the American option before its expiration in this case), $v ( 3 , 1 ) = \operatorname* { m a x } \{ 3 . 0 0 , 2 . 0 8 \} = \oint \ 3 . 0 0$ and $v ( 3 , 2 ) = v ( 3 , 3 ) = 0$ . Continuing the computations going backward, we compute $v ( 2 , j )$ for $j = 0 , 1 , 2$ , then $v ( 1 , j )$ for $j = 0 , 1$ and finally $v ( 0 , 0 )$ . See Figure 14.2. The option price is $v ( 0 , 0 ) = \mathbb { \ S } \ 2 . 3 5$ 

Note that the approach we outlined above can be used with various types of derivative securities with payof functions that may make other types of analysis dificult. 

Exercise 14.3 Compute the value of an American put option on a stock with current price equal to $ 100, strike price equal to $ 98 and expiration date 5 weeks from today. The yearly volatility of the logarithm of the stock return is $\sigma = 0 . 3 0$ . The risk-free interest rate is 4%. Use a binomial lattice with $N = 5$ 

Exercise 14.4 Compute the value of an American call option on a stock with current price equal to $ 100, strike price equal to $ 102 and expiration date 4 weeks from today. The yearly volatility of the logarithm of the stock return is $\sigma = 0 . 3 0$ . The risk-free interest rate is 4%. Use a binomial lattice with $N = 4$ 

Exercise 14.5 Computational exercise: Repeat Exercises 14.3 and 14.4 using a binimial lattice with $N = 1 0 0 0$ 

## Chapter 15

# DP Models: Structuring Asset Backed Securities

The structuring of collateralized mortgage obligations will give us an opportunity to apply the dynamic programming approach studied in Chapter 13. 

Mortgages represent the largest single sector of the US debt market, surpassing even the federal government. In 2000, there were over $5 trillion in outstanding mortgages. Because of the enormous volume of mortgages and the importance of housing in the US economy, numerous mechanisms have been developed to facilitate the provision of credit to this sector. The predominant method by which this has been accomplished since 1970 is securitization, the bundling of individual mortgage loans into capital market instruments. In 2000, $2.3 trillion of mortgage-backed securities were outstanding, an amount comparable to the $2.1 trillion corporate bond market and $3.4 trillion market in federal government securities. 

A mortgage-backed security (MBS) is a bond backed by a pool of mortgage loans. Principal and interest payments received from the underlying loans are passed through to the bondholders. These securities contain at least one type of embedded option due to the right of the home buyer to prepay the mortgage loan before maturity. Mortgage payers may prepay for a variety of reasons. By far the most important factor is the level of interest rates. As interest rates fall, those who have fixed rate mortgages tend to repay their mortgages faster. 

MBS were first packaged using the pass-through structure. The passthrough’s essential characteristic is that investors receive a pro rata share of the cash flows that are generated by the pool of mortgages – interest, scheduled amortization and principal prepayments. Exercise of mortgage prepayment options has pro rata efects on all investors. The pass-through allows banks that initiate mortgages to take their fees up front, and sell the mortgages to investors. One troublesome feature of the pass-through for investors is that the timing and level of the cash flows are uncertain. Depending on the interest rate environment, mortgage holders may prepay substantial portions of their mortgage in order to refinance at lower interest rates. 

A collateralized mortgage obligation (CMO) is a more sophisticated MBS. The CMO rearranges the cash flows to make them more predictable. This feature makes CMO’s more desirable to investors. The basic idea behind a CMO is to restructure the cash-flows from an underlying mortgage collateral (pool of mortgage loans) into a set of bonds with diferent maturities. These two or more series of bonds (called “tranches”) receive sequential, rather than pro rata, principal pay down. Interest payments are made on all tranches (except possibly the last tranche, called Z tranche or “accrual” tranche). A two tranche CMO is a simple example. Assume that there is $100 in mortgage loans backing two $50 tranches, say tranche A and tranche B. Initially, both tranches receive interest, but principal payments are used to pay down only the A tranche. For example, if $1 in mortgage scheduled amortization and prepayments is collected in the first month, the balance of the A tranche is reduced (paid down) by $1. No principal is paid on the B tranche until the A tranche is fully retired, i.e. $50 in principal payments have been made. Then the remaining $50 in mortgage principal pays down the $50 B tranche. In efect, the A or “fast-pay” tranche has been assigned all of the early mortgage principal payments (amortization and prepayments) and reaches its maturity sooner than would an ordinary pass-through security. The B or “slow-pay” tranche has only the later principal payments and it begins paying down much later than an ordinary pass-through security. 

By repackaging the collateral cash-flow in this manner, the life and risk characteristics of the collateral are restructured. The fast-pay tranches are guaranteed to be retired first, implying that their lives will be less uncertain, although not completely fixed. Even the slow-pay tranches will have less cash-flow uncertainty than the underlying collateral. Therefore the CMO allows the issuer to target diferent investor groups more directly than when issuing pass-through securities. The low maturity (fast-pay) tranches may be appealing to investors with short horizons while the long maturity bonds (slow-pay) may be attractive to pension funds and life insurance companies. Each group can find a bond which is better customized to their particular needs. 

A by-product of improving the predictability of the cash flows is being able to structure tranches of diferent credit quality from the same mortgage pool. With the payments of a very large pool of mortgages dedicated to the “fast-pay” tranche, it can be structured to receive a AAA credit rating even if there is a significant default risk on part of the mortgage pool. This high credit rating lowers the interest rate that must be paid on this slice of the CMO. While the credit rating for the early tranches can be very high, the credit quality for later tranches will necessarily be lower because there is less principal left to be repaid and therefore there is increased default risk on slow-pay tranches. 

We will take the perspective of an issuer of CMO’s. How many tranches should be issued? Which sizes? Which coupon rates? Issuers make money by issuing CMO’s because they can pay interest on the tranches that is lower than the interest payments being made by mortgage holders in the pool. The mortgage holders pay 10 or 30-year interest rates on the entire outstanding principal, while some tranches only pay 2, 4, 6 and 8-year interest rates plus an appropriate spread. 

The convention in mortgage markets is to price bonds with respect to their weighted average life (WAL), which is much like duration, i.e. 

$$
W A L = \frac {\sum_ {t = 1} ^ {T} t P _ {t}}{\sum_ {t = 1} ^ {T} P _ {t}}
$$

where $P _ { t }$ is the principal payment in period t $( t = 1 , \ldots , T )$ 

A bond with a WAL of 3 years will be priced at the 3 year treasury rate plus a spread, while a bond with a WAL of 7 years will be priced at the 7 year treasury rate plus a spread. The WAL of the CMO collateral is typically high, implying a high rate for (normal) upward sloping rate curves. By splitting the collateral into several tranches, some with a low WAL and some with a high WAL, lower rates are obtained on the fast-pay tranches while higher rates result for the slow-pay. Overall, the issuer ends up with a better (lower) average rate on the CMO than on the collateral. 

## 15.1 Data

When issuing a CMO, several restrictions apply. First it must be demonstrated that the collateral can service the payments on the issued CMO tranches under several scenarios. These scenarios are well defined and standardized, and cover conditional prepayment models (see below) as well as the two extreme cases of full immediate prepayment and no prepayment at all. Second, the tranches are priced using their expected WAL. For example, a tranche with a WAL between 2.95 and 3.44 will be priced at the 3-year Treasury rate plus a spread that depends on the tranche’s rating. For a AAA rating, the spread might be 1% whereas for a BB rating, the spread might be 2%. 

The following table contains the payment schedule for a $100 Million pool of 10-year mortgages with 10 $\%$ interest, assuming the same total payment (interest + scheduled amortization) each year. It may be useful to remember that, if the outstanding principal is $Q ,$ , interest is r and amortization occurs over k years, the scheduled amortization in the first year is 

$$
\frac {Q r}{(1 + r) ^ {k} - 1}.
$$

Exercise 15.1 Derive this formula, using the fact that the total payment (interest + scheduled amortization) is the same for years 1 through k. 

Here $Q = 1 0 0 \ r = 0 . 1 0$ and $k = 1 0$ , thus the scheduled amortization in the first year is 6.27. Adding the 10 % interest payment on $Q ,$ , the total payments (interest + scheduled amortization) are $16.27 M per year. 

<table><tr><td>Period (t)</td><td>Interest<eq>(I_t)</eq></td><td>Scheduled Amortization<eq>(P_t)</eq></td><td>Outstanding Principal<eq>(Q_t)</eq></td></tr><tr><td>1</td><td>10.00</td><td>6.27</td><td>93.73</td></tr><tr><td>2</td><td>9.37</td><td>6.90</td><td>86.83</td></tr><tr><td>3</td><td>8.68</td><td>7.59</td><td>79.24</td></tr><tr><td>4</td><td>7.92</td><td>8.35</td><td>70.89</td></tr><tr><td>5</td><td>7.09</td><td>9.19</td><td>61.70</td></tr><tr><td>6</td><td>6.17</td><td>10.11</td><td>51.59</td></tr><tr><td>7</td><td>5.16</td><td>11.12</td><td>40.47</td></tr><tr><td>8</td><td>4.05</td><td>12.22</td><td>28.25</td></tr><tr><td>9</td><td>2.83</td><td>13.45</td><td>14.80</td></tr><tr><td>10</td><td>1.48</td><td>14.80</td><td>0</td></tr><tr><td colspan="2">Total</td><td colspan="2">100.00</td></tr></table>

The above table assumes no prepayment. Next we want to analyze the following scenario: a conditional prepayment model reflecting the 100% PSA (Public Securities Association) industry-standard benchmark. For simplicity, we present a yearly PSA model, even though the actual PSA model is defined monthly. The rate of mortgage prepayments is 1% of the outstanding principal at the end of the first year. At the end of the second year, prepayment is 3% of the outstanding principal at that time. At the end of the third year, it is 5% of the outstanding principal. For each later year $t \geq 3$ , prepayment is 6% of the outstanding principal at the end of year t. Let us denote by $P P _ { t }$ the prepayment in year t. For example, in year 1, in addition to the interest payment $I _ { 1 } = 1 0$ and the amortization payment $A _ { 1 } = 6 . 2 7$ , there is $\mathrm { ~ a ~ 1 ~ \% ~ }$ prepayment on the $1 0 0 \textrm { - } 6 . 2 7 =$ 93.73 principal remaining after amortization. That is, there is a prepayment $P P _ { 1 } = 0 . 9 3 7 3$ collected at the end of year 1. Thus the principal pay down is $P _ { 1 } = A _ { 1 } + P P _ { 1 } = 6 . 2 7 + 0 . 9 3 7 3 = 7 . 2 0 7 3$ in year 1. The outstanding principal at the end of year 1 is $Q _ { 1 } = 1 0 0 - 7 . 2 0 7 3 = 9 2 . 7 9 2 7$ . In year 2, the interest paid is $I _ { 2 } = 9 . 2 7 9$ (that is 10% of $Q _ { 1 } )$ , the amortization payment is $\begin{array} { r } { A _ { 2 } = \frac { Q _ { 1 } \times 0 . 1 0 } { ( 1 . 1 0 ) ^ { 9 } - 1 } = 6 . 8 3 3 3 } \end{array}$ and the prepayment is $P P _ { 2 } = 2 . 5 7 8 8$ (that is 3% of $Q _ { 1 } - A _ { 2 } )$ and the principal pay down is $P _ { 2 } = A _ { 2 } + P P _ { 2 } = 9 . 4 1 2$ , etc. 

Exercise 15.2 Construct the table containing $I _ { t } , \ P _ { t }$ and $Q _ { t }$ to reflect the above scenario. 

## Loss multiple and required bufer

In order to achieve a high quality rating, tranches should be able to sustain higher than expected default rates without compromising payments to the tranche holders. For this reason, credit ratings are assigned based on how much money is “behind” the current tranche. That is, how much outstanding principal is left after the current tranche is retired, as a percentage of the total amount of principal. This is called the “bufer”. Early tranches receive higher credit ratings since they have greater bufers, which means that the CMO would have to experience very large default rates before their payments would be compromised. A tranche with AAA rating must have a bufer equal to six times the expected default rate. This is referred to as the “loss multiple”. The loss multiples are as follows: 

<table><tr><td>Credit Rating</td><td>AAA</td><td>AA</td><td>A</td><td>BBB</td><td>BB</td><td>B</td><td>CCC</td></tr><tr><td>Loss Multiple</td><td>6</td><td>5</td><td>4</td><td>3</td><td>2</td><td>1.5</td><td>0</td></tr></table>

The required bufer is computed by the following formula: 

Required Bufer = WAL * Expected Default Rate * Loss Multiple 

Let us assume a 0.9% expected default rate, based on foreclosure rates reported by the M&T Mortgage Corporation in 2004. With this assumption, the required bufer to get a AAA rating for a tranche with a WAL of 4 years is $4 \times 0 . 0 0 9 \times 6 = 2 1 . 6 \%$ 

Exercise 15.3 Construct the table containing the required bufer as a function of rating and WAL, assuming a 0.9% expected default rate. 

## Coupon Yields and Spreads

Each tranche is priced based on a credit spread to the current treasury rate for a risk-free bond of that approximate duration. These rates appear in the next table, based on the yields on U.S. Treasuries as of 10/12/04. The reader can get more current figures from on-line sources. Spreads on corporate bonds with similar credit ratings would provide reasonable figures. 

<table><tr><td rowspan="2">Period (t)</td><td rowspan="2">Risk-Free Spot</td><td colspan="6">Credit Spread in Basis Points</td></tr><tr><td>AAA</td><td>AA</td><td>A</td><td>BBB</td><td>BB</td><td>B</td></tr><tr><td>1</td><td>2.18 %</td><td>13</td><td>43</td><td>68</td><td>92</td><td>175</td><td>300</td></tr><tr><td>2</td><td>2.53 %</td><td>17</td><td>45</td><td>85</td><td>109</td><td>195</td><td>320</td></tr><tr><td>3</td><td>2.80 %</td><td>20</td><td>47</td><td>87</td><td>114</td><td>205</td><td>330</td></tr><tr><td>4</td><td>3.06 %</td><td>26</td><td>56</td><td>90</td><td>123</td><td>220</td><td>343</td></tr><tr><td>5</td><td>3.31 %</td><td>31</td><td>65</td><td>92</td><td>131</td><td>235</td><td>355</td></tr><tr><td>6</td><td>3.52 %</td><td>42</td><td>73</td><td>96</td><td>137</td><td>245</td><td>373</td></tr><tr><td>7</td><td>3.72 %</td><td>53</td><td>81</td><td>99</td><td>143</td><td>255</td><td>390</td></tr><tr><td>8</td><td>3.84 %</td><td>59</td><td>85</td><td>106</td><td>151</td><td>262</td><td>398</td></tr><tr><td>9</td><td>3.95 %</td><td>65</td><td>90</td><td>112</td><td>158</td><td>268</td><td>407</td></tr><tr><td>10</td><td>4.07 %</td><td>71</td><td>94</td><td>119</td><td>166</td><td>275</td><td>415</td></tr></table>

## 15.2 Enumerating possible tranches

We are going to consider every possible tranche: since there are 10 possible maturities t and t possible starting dates j with $j \le t$ for each t, there are $5 5$ possible tranches. Specifically, tranche $( j , t )$ starts amortizing at the beginning of year $j$ and ends at the end of year t. 

Exercise 15.4 From the principal payments $P _ { t }$ that you computed in Exercise 15.2, construct a table containing $\mathrm { W A L } _ { j t }$ for each possible combination $( j , t )$ 

For each of the 55 possible tranches $( j , t )$ , compute the bufer $\frac { \sum _ { k = t + 1 } ^ { 1 0 } P _ { k } } { \sum _ { k = 1 } ^ { 1 0 } P _ { k } }$ PIf there is no bufer, the corresponding tranche is a Z-tranche. When there is a bufer, calculate the Loss Multiple from the formula: Required Bufer $= \mathrm { W A L \ ^ { * } }$ Expected Default Rate * Loss Multiple. Finally construct a table containing the credit rating for each tranche that is not a Z-tranche. 

For each of the 55 tranches, construct a table containing the appropriate coupon rate $c _ { j t }$ (no coupon rate on a Z-tranche). As described earlier, these rates depend on the WAL and credit rating just computed. 

Define $T _ { j t }$ to be the present value of the payments on a tranche $( j , t )$ Armed with the proper coupon rate $c _ { j t }$ and a full curve of spot rates $r _ { t } , T _ { j t }$ is computed as follows. In each year $k ,$ the payment $C _ { k }$ for tranche $( j , t )$ is equal to the coupon rate $c _ { j t }$ times the remaining principal, plus the principal payment made to tranche $( j , t )$ if it is amortizing in year $k .$ The present value of $C _ { k }$ is simply equal to $\frac { C _ { k } } { ( 1 + r _ { k } ) ^ { k } }$ . Now $T _ { j t }$ is obtained by summing the present values of all the payments going to tranche $( j , t )$ 

## 15.3 A Dynamic Programming Approach

Based on the above data, we would like to structure a CMO with four sequential tranches A, B, C, Z. The objective is to maximize the profits from the issuance by choosing the size of each tranche. In this section, we present a dynamic programming recursion for solving the problem. 

Let $t = 1 , \ldots , 1 0$ index the years. The states of the dynamic program will be the years t and the stages will be the number k of tranches up to year t. 

Now that we have the matrix $T _ { j t }$ , we are ready to describe the dynamic programming recursion. Let 

v(k, t) = Minimum present value of total payments to bondholders in years 1 through t when the CMO has k tranches up to year t. 

Obviously, $v ( 1 , t )$ is simply $T _ { 1 t }$ . For $k \geq 2$ , the value $\boldsymbol { v } ( \boldsymbol { k } , t )$ is computed recursively by the formula: 

$$
v (k, t) = \min _ {j = k - 1, \dots , t - 1} (v (k - 1, j) + T _ {j + 1, t}).
$$

For example, for $k = 2$ and $t = 4$ , we compute $v ( 1 , j ) + T _ { j + 1 , 4 }$ for each $j = 1 , 2 , 3$ and we take the minimum. The power of dynamic programming becomes clear as k increases. For example, when $k = 4$ , there is no need to compute the minimum of thousands of possible combinations of 4 tranches. Instead, we use the optimal structure $v ( 3 , j )$ already computed in the previous stage. So the only enumeration is over the size of the last tranche. 

Exercise 15.5 Compute v(4, 10) using the above recursion. Recall that $v ( 4 , 1 0 )$ is the least cost solution of structuring the CMO into four tranches. What are the sizes of the tranches in this optimal solution? To answer this question, you will need to backtrack from the last stage and identify how the minimum leading to v(4, 10) was achieved at each stage. 

Exercise 15.6 The dynamic programming approach presented in this section is based on a single prepayment model. How would you deal with several scenarios for prepayment and default rates, each occuring with a given probability? 

## 15.4 Case Study

Repeat the above steps for a pool of mortgages using current data. Study the influence of the expected default rate on the profitability of structuring your CMO. What other factors have a significant impact on profitability? 

254CHAPTER 15. DP MODELS: STRUCTURING ASSET BACKED SECURITIES 

# Stochastic Programming: Theory and Algorithms

## 16.1 Introduction

In the introductory chapter and elsewhere, we argued that many optimization problems are described by uncertain parameters. There are diferent ways of incorporating this uncertainty. We consider two approaches: Stochastic programming in the present chapter and robust optimization in Chapter 19. Stochastic programming assumes that the uncertain parameters are random variables with known probability distributions. This information is then used to transform the stochastic program into a so-called deterministic equivalent which might be a linear program, a nonlinear program or an integer program (see Chapters 2, 5 and 11 respectively). 

While stochastic programming models have existed for several decades, computational technology has only recently allowed the solution of realistic size problems. The field continues to develop with the advancement of available algorithms and computing power. It is a popular modeling tool for problems in a variety of disciplines including financial engineering. 

The uncertainty is described by a certain sample space Ω, a σ-field of random events and a probability measure P (see Appendix C). In stochastic programming, Ω is often a finite set $\{ \omega _ { 1 } , \ldots , \omega _ { S } \}$ . The corresponding probabilities $p ( \omega _ { k } ) \ge 0$ satisfy $\begin{array} { r } { \sum _ { k = 1 } ^ { S } p ( \omega _ { k } ) = 1 } \end{array}$ . For example, to represent Pthe outcomes of flipping a coin twice in a row, we would use four random events $\Omega = \{ H H , H T , T H , T T \}$ , each with probability 1/4, where H stands for Head and T stands for Tail. 

Stochastic programming models can include anticipative and/or adaptive decision variables. Anticipative variables correspond to those decisions that must be made here-and-now and cannot depend on the future observations/partial realizations of the random parameters. Adaptive variables correspond to wait-and-see decisions that can be made after some (or, sometimes all) of the random parameters are observed. 

Stochastic programming models that include both anticipative and adaptive variables are called recourse models. Using a multi-stage stochastic programming formulation, with recourse variables at each stage, one can model a decision environment where information is revealed progressively and the decisions are adapted to each new piece of information. 

In investment planning, each new trading opportunity represents a new decision to be made. Therefore, trading dates where investment portfolios can be rebalanced become natural choices for decision stages, and these problems can be formulated conveniently as multi-stage stochastic programming problems with recourse. 

## 16.2 Two Stage Problems with Recourse

In Chapter 1, we have already seen a generic form of a two-stage stochastic linear program with recourse: 

$$
\begin{array}{r l r l} \max _ {x} & a ^ {T} x + E [ \max _ {y (\omega)} c (\omega) ^ {T} y (\omega) ] & = & b \\ A x & & C (\omega) y (\omega) & = d (\omega) \\ B (\omega) x + & & y (\omega) \geq 0. \end{array}\tag{16.1}
$$

In this formulation, the first-stage decisions are represented by vector x. These decisions are made before the random event $\omega$ is observed. The second-stage decisions are represented by vector $y ( \omega )$ . These decisions are made $a f t e r$ the random event $\omega$ has been observed, and therefore the vector $y$ is a function of $\omega .$ . A and b define deterministic constraints on the first-stage decisions x, whereas $B ( \omega ) , C ( \omega )$ , and $d ( \omega )$ define stochastic constraints linking the recourse decisions $y ( \omega )$ to the first-stage decisions x. The objective function contains a deterministic term $a ^ { T }$ x and the expectation of the second-stage objective $c ( \omega ) ^ { T } y ( \omega )$ taken over all realizations of the random event ω. 

Notice that the first-stage decisions will not necessarily satisfy the linking constraints $B ( \omega ) x + C ( \omega ) y ( \omega ) = d ( \omega )$ , if no recourse action is taken. Therefore, recourse allows one to make sure that the initial decisions can be “corrected” with respect to this second set of feasibility equations. 

In Section 1.2.1, we also argued that problem (16.1) can be represented in an alternative manner by considering the second-stage or recourse problem that is defined as follows, given $x _ { i }$ , the first-stage decisions: 

$$
\begin{array}{r c l} f (x, \omega) = \max & c (\omega) ^ {T} y (\omega) \\ & C (\omega) y (\omega) & = d (\omega) - B (\omega) x \\ & y (\omega) \geq 0. \end{array}\tag{16.2}
$$

Let $f ( x ) = E [ f ( x , \omega ) ]$ denote the expected value of this optimum. If the function $f ( x )$ is available, the two-stage stochastic linear program (16.1) reduces to a deterministic nonlinear program: 

$$
\begin{array}{l l} \max & a ^ {T} x + f (x) \\ & A x = b \\ & x \geq 0. \end{array}\tag{16.3}
$$

Unfortunately, computing $f ( x )$ is often very hard, especially when the sample space Ω is infinite. Next, we consider the case where Ω is a finite set. 

Assume that $\Omega \ = \ \{ \omega _ { 1 } , . . . , \omega _ { S } \}$ and let $p ~ = ~ ( p _ { 1 } , . . . , p _ { S } )$ denote the probability distribution on this sample space. The S possibilities $\omega _ { k }$ , for $k = 1 , \dots , S$ are also called scenarios. The expectation of the second-stage objective becomes: 

$$
E [ \max _ {y (\omega)} c (\omega) ^ {T} y (\omega) ] = \sum_ {k = 1} ^ {S} p _ {k} \max _ {y (\omega_ {k})} c (\omega_ {k}) ^ {T} y (\omega_ {k})
$$

For brevity, we write $c _ { k }$ instead of $c ( \omega _ { k } )$ , etc. Under this scenario $a p \textmd { - }$ proach the two-stage stochastic linear programming problem (16.1) takes the following form: 

$$
\begin{array}{r l} \max _ {x} & a ^ {T} x + \sum_ {k = 1} ^ {S} p _ {k} \max _ {y _ {k}} c _ {k} ^ {T} y _ {k} \\ & A x = b \\ & B _ {k} x + C _ {k} y _ {k} = d _ {k} \quad \text {for k = 1,\ldots S} \\ & x \geq 0 \\ & y _ {k} \geq 0 \quad \text {for k = 1,\ldots,S}. \end{array}\tag{16.4}
$$

Note that there is a diferent second stage decision vector $y _ { k }$ for each scenario k. The maximum in the objective is achieved by optimizing over all variables x and $y _ { k }$ simultaneously. Therefore, this optimization problem is: 

$$
\begin{array}{r l r l r l r l} \max _ {x, y _ {1}, \ldots , y _ {S}} & a ^ {T} x + p _ {1} c _ {1} ^ {T} y _ {1} + \ldots + p _ {S} c _ {S} ^ {T} y _ {S} & & \\ & A x & & = b \\ & B _ {1} x + C _ {1} y _ {1} & & = d _ {1} \\ & \vdots & \ddots & & \vdots \\ & B _ {S} x & & + C _ {S} y _ {S} = d _ {S} \\ & x, & y _ {1}, & \ldots & y _ {S} \geq 0. \end{array}\tag{16.5}
$$

This is a deterministic linear programming problem called the deterministic equivalent of the original uncertain problem. This problem has S copies of the second-stage decision variables and therefore, can be significantly larger than the original problem before we considered the uncertainty of the parameters. Fortunately, however, the constraint matrix has a very special sparsity structure that can be exploited by modern decomposition based solution methods (see Section 16.4). 

Exercise 16.1 Consider an investor with an initial wealth $W _ { 0 }$ . At time $0 ,$ the investor constructs a portfolio comprising one riskless asset with return $R _ { 1 }$ in the first period and one risky asset with return $R _ { 1 } ^ { + }$ with probability 0.5 and $R _ { 1 } ^ { - }$ with probability 0.5. At the end of the first period, the investor can rebalance her portfolio. The return in the second period is $R _ { 2 }$ for the riskless asset, while it is $R _ { 2 } ^ { + }$ with probability 0.5 and $R _ { 2 } ^ { - }$ with probability 0.5 for the risky asset. The objective is to meet a liability $L _ { 2 } = 0 . 9$ at the end of Period 2 and to maximize the expected remaining wealth $W _ { 2 }$ . Formulate a 2-stage stochastic linear program that solves the investor’s problem. 


Exercise 16.2 In Exercise 3.2, the cash requirement in quarter Q1 is known to be 100 but, for the remaining quarters, the company considers 3 equally likely scenarios:


<table><tr><td></td><td>Q2</td><td>Q3</td><td>Q4</td><td>Q5</td><td>Q6</td><td>Q7</td><td>Q8</td></tr><tr><td>Scenario 1</td><td>450</td><td>100</td><td>-650</td><td>-550</td><td>200</td><td>650</td><td>-850</td></tr><tr><td>Scenario 2</td><td>500</td><td>100</td><td>-600</td><td>-500</td><td>200</td><td>600</td><td>-900</td></tr><tr><td>Scenario 3</td><td>550</td><td>150</td><td>-600</td><td>-450</td><td>250</td><td>600</td><td>-800</td></tr></table>

Formulate a linear program that maximizes the expected wealth of the company at the end of quarter Q8. 

## 16.3 Multi Stage Problems

In a multi-stage stochastic program with recourse, the recourse decisions can be taken at several points in time, called stages. Let $n \geq 2$ be the number of stages. The random event ω is a vector $\left( o _ { 1 } , \ldots , o _ { n - 1 } \right)$ that gets revealed progressively over time. The first-stage decisions are taken before any component of $\omega$ is revealed. Then $o _ { 1 }$ is revealed. With this knowledge, one takes the second-stage decisions. After that, $O _ { 2 }$ is revealed, and so on, alternating between a new component of ω beeing revealed and new recourse decisions beeing implemented. We assume that $\Omega = \{ \omega _ { 1 } , \ldots , \omega _ { S } \}$ is a finite set. Let $p _ { k }$ be the probability of scenario $\omega _ { k }$ , for $k = 1 , \dots , S$ 

Some scenarios $\omega _ { k }$ may be identical in their first components and only become diferentiated in the later stages. Therefore it is convenient to introduce the scenario tree, which illustrates how the scenarios branch of at each stage. The nodes are labelled 1 through N, where node 1 is the root. Each node is in one stage, where the root is the unique node in stage 1. Each node i in stage $k \geq 2$ is adjacent to a unique node $a ( i )$ in stage $k - 1$ . Node $a ( i )$ is called the father of node i. The paths from the root to the leaves (in stage n) represent the scenarios. Thus the last stage has as many nodes as scenarios. These nodes are called the terminal nodes. The collection of scenarios passing through node i in stage k have identical components $o _ { 1 } , \ldots , o _ { k - 1 } .$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/d134bf38fd1a4e89d113b26a4dbf061a57400b787d9cffb2477770c7ef8eb508.jpg)



Figure 16.1: A scenario tree with 3 stages and 4 scenarios


In Figure 16.1, Node 1 is the root, Nodes 4, 5, 6 and 7 are the terminal nodes. The father of Node 6 is Node 2, in other words $a ( 6 ) = 2$ 

Associated with each node i is a recourse decision vector $x _ { i }$ . For a node i is stage k, the decisions $x _ { i }$ are taken based on the information that has been revealed up to stage k. Let $q _ { i }$ be the sum of the probabilities $p _ { k }$ over all the scenarios $\omega _ { k }$ that go through node i. Therefore $q _ { i }$ is the probability of node $i ,$ conditional on being in Stage k. The multi-stage stochastic program with recourse can be formulated as follows: 

$$
\begin{array}{r l r} \max _ {x _ {1}, \ldots , x _ {N}} & & \sum_ {i = 1} ^ {N} q _ {i} c _ {i} ^ {T} x _ {i} \\ A x _ {1} & & = b \\ B _ {i} x _ {a (i)} + C _ {i} x _ {i} & = d _ {i} & \text {for i = 2,\ldots,N} \\ & x _ {i} \geq 0. \end{array}\tag{16.6}
$$

In this formulation, A and b define deterministic constraints on the firststage decisions $x _ { 1 }$ , whereas $B _ { i } , C _ { i }$ , and $d _ { i }$ define stochastic constraints linking the recourse decisions $x _ { i }$ in node i to the recourse decisions $x _ { a ( i ) }$ in its father node. The objective function contains a term $c _ { i } ^ { T } x _ { i }$ for each node. 

To illustrate, we present formulation (16.6) for the example of Figure 16.1. The terminal nodes 4 to 7 correspond to scenarios 1 to 4 respectively. Thus we have $q _ { 4 } = p _ { 1 } , q _ { 5 } = p _ { 2 } , q _ { 6 } = p _ { 3 }$ and $q _ { 7 } = p _ { 4 }$ , where $p _ { k }$ is the probability of scenario k. We also have $q _ { 2 } = p _ { 1 } + p _ { 2 } + p _ { 3 } , q _ { 3 } = p _ { 4 }$ and $q _ { 2 } + q _ { 3 } = 1$ 

$$
\begin{array}{r l r l r l r l} \max & c _ {1} ^ {T} x _ {1} & + q _ {2} c _ {2} ^ {T} x _ {2} & + q _ {3} c _ {3} ^ {T} x _ {3} & + p _ {1} c _ {4} ^ {T} x _ {4} & + p _ {2} c _ {5} ^ {T} x _ {5} & + p _ {3} c _ {6} ^ {T} x _ {6} & p _ {4} c _ {7} ^ {T} x _ {7} \\ & A x _ {1} & & & & & & = & b \\ & B _ {2} x _ {1} & + C _ {2} x _ {2} & & & & & = & d _ {2} \\ & B _ {3} x _ {1} & & + C _ {3} x _ {3} & & & & = & d _ {3} \\ & & B _ {4} x _ {2} & & + C _ {4} x _ {4} & & & = & d _ {4} \\ & & B _ {5} x _ {2} & & & + C _ {5} x _ {5} & & = & d _ {5} \\ & & B _ {6} x _ {2} & & & & + C _ {6} x _ {6} & = & d _ {6} \\ & & & B _ {7} x _ {3} & & & + C _ {7} x _ {7} & = & d _ {7} \\ & & & & & & x _ {i} \geq 0. \end{array}
$$

Note that the size of the linear program (16.6) increases rapidly with the number of stages. For example, for a problem with 10 stages and a binary tree, there are 1024 scenarios and therefore the linear program (16.6) may have several thousand constraints and variables, depending on the number of variables and constraints at each node. Modern commercial codes can handle such large linear programs, but a moderate increase in the number of stages or in the number of branches at each stage could make (16.6) too large to solve by standard linear programming solvers. When this happens, one may try to exploit the special structure of (16.6) to solve the model (see Section 16.4). 

Exercise 16.3 In Exercise 3.2, the cash requirements in quarters Q1, Q2, Q3, Q6 and Q7 are known. On the other hand, the company considers two equally likely (and independent) possibilities for each of the quarters Q4, Q5 and Q8, giving rise to eight equally likely scenarios. In quarter Q4, the cash inflow will be either 600 or 650. In quarter Q5, it will be either 500 or 550. In quarter Q8, it will be either 850 or 900. Formulate a linear program that maximizes the expected wealth of the company at the end of quarter Q8. 

Exercise 16.4 Develop the linear program (16.6) for the following scenario tree. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/dd11e8db0f8399dcc16bb4d373764baac55075fefa97e42fbacb5395d840c3e4.jpg)


## 16.4 Decomposition

The size of the linear program (16.6) depends on the number of decision stages and the branching factor at each node of the scenario tree. For example, a 4-stage model with 25 branches at each node has $2 5 \times 2 5 \times$ $2 5 \times 2 5 = 3 9 0 6 2 5$ scenarios. Increasing the number of stages and branches quickly results in an explosion of dimensionality. Obviously, the size of (16.6) can be a limiting factor in solving realistic problems. When this occurs, it becomes essential to take advantage of the special structure of the linear program (16.6). In this section, we present a decomposition algorithm for exploiting this structure. It is called Benders decomposition or, in the stochastic programming literature, the L-shaped method. 

The structure that we really want to exploit is that of the two-stage problem (16.5). So we start with (16.5). We will explain subsequently how to deal with the general multi-stage model (16.6). The constraint matrix of (16.5) has the following form: 

$$
\left( \begin{array}{c c c c} A & & & \\ B _ {1} & C _ {1} & & \\ \vdots & & \ddots & \\ B _ {S} & & & C _ {S} \end{array} \right).
$$

Note that the blocks $C _ { 1 } , \ldots , C _ { S }$ of the constraint matrix are only interrelated through the blocks $B _ { 1 } , \ldots , B _ { S }$ which correspond to the first-stage decisions. In other words, once the first-stage decisions x have been fixed, (16.5) decomposes into S independent linear programs. The idea of Benders decomposition is to solve a “master problem” involving only the variables x and a series of independent “recourse problems” each involving a diferent vector of variables $y _ { k } .$ . The master problem and recourse problems are linear programs. The size of these linear programs is much smaller than the size of full model (16.5). The recourse problems are solved for a given vector x and their solutions are used to generate inequalities that are added to the master problem. Solving the new master problem produces a new x and the process is repeated. More specifically, let us write (16.5) as 

$$
\begin{array}{r c l r c l r c l} \max _ {x} & a ^ {T} x & + & P _ {1} (x) & + & \ldots & + & P _ {S} (x) \\ & A x & = & b \\ & x & \geq & 0 \end{array}\tag{16.7}
$$

where, for $k = 1 , \dots S$ 

$$
\begin{array}{r c l} P _ {k} (x) & = & \max _ {y _ {k}} p _ {k} c _ {k} ^ {T} y _ {k} \\ & & C _ {k} y _ {k} = d _ {k} - B _ {k} x \\ & & y _ {k} \geq 0. \end{array}\tag{16.8}
$$

The dual linear program of the recourse problem (16.8) is: 

$$
\begin{array}{r c l} P _ {k} (x) & = & \min _ {u _ {k}} u _ {k} ^ {T} (d _ {k} - B _ {k} x) \\ & & C _ {k} ^ {T} u _ {k} \geq p _ {k} c _ {k}. \end{array}\tag{16.9}
$$

For simplicity, we assume that the dual (16.9) is feasible, which is the case of interest in applications. The recourse linear program (16.8) will be solved for a sequence of vectors $x ^ { i }$ , for $i = 0 , \ldots$ . The initial vector $x ^ { 0 }$ might be obtained by solving 

$$
\begin{array}{r l r} \max _ {x} & a ^ {T} x \\ & A x = b \\ & x \geq 0. \end{array}\tag{16.10}
$$

For a given vector $x ^ { i } .$ , two possibilities can occur for the recourse linear program (16.8): either (16.8) has an optimal solution or it is infeasible. 

If (16.8) has an optimal solution $y _ { k } ^ { i }$ , and $u _ { k } ^ { i }$ is the corresponding optimal dual solution, then (16.9) implies that 

$$
P _ {k} (x ^ {i}) = (u _ {k} ^ {i}) ^ {T} (d _ {k} - B _ {k} x ^ {i})
$$

and, since 

$$
P _ {k} (x) \leq (u _ {k} ^ {i}) ^ {T} (d _ {k} - B _ {k} x)
$$

we get that 

$$
P _ {k} (x) \leq (u _ {k} ^ {i}) ^ {T} (B _ {k} x ^ {i} - B _ {k} x) + P _ {k} (x ^ {i}).
$$

This inequality, which is called an optimality cut, can be added to the current master linear program. Initially, the master linear program is just (16.10). 

If (16.8) is infeasible, then the dual problem is unbounded. Let $u _ { k } ^ { i }$ a direction where (16.9) is unbounded, i.e. $( u _ { k } ^ { i } ) ^ { T } ( d _ { k } - B _ { k } x ^ { i } ) < 0$ and $C _ { k } ^ { T } u _ { k } ^ { i } \ge$ $p _ { k } c _ { k }$ . Since we are only interested in first-stage decisions x that lead to feasible second-stage decisions $y _ { k }$ , the following feasibility cut can be added to the current master linear program: 

$$
(u _ {k} ^ {i}) ^ {T} (d _ {k} - B _ {k} x) \geq 0.
$$

After solving the recourse problems (16.8) for each $k ,$ we have the following lower bound on the optimal value of (16.5): 

$$
L B = a ^ {T} x ^ {i} + P _ {1} (x ^ {i}) + \ldots + P _ {S} (x ^ {i})
$$

where we set $P _ { k } ( x ^ { i } ) = - \infty$ if the corresponding recourse problem is infeasible. 

Adding all the optimality and feasibility cuts found so far (for $j ~ =$ $0 , \ldots , i )$ to the master linear program, we obtain: 

$$
\begin{array}{r c l} \max _ {x, z _ {1}, \ldots , z _ {S}} & a ^ {T} x & + \sum_ {k = 1} ^ {S} z _ {k} \\ & A x & = b \\ & z _ {k} & \leq (u _ {k} ^ {j}) ^ {T} (B _ {k} x ^ {j} - B _ {k} x) + P _ {k} (x ^ {j}) \text {for some pairs} (j, k) \\ & 0 & \leq (u _ {k} ^ {j}) ^ {T} (d _ {k} - B _ {k} x) \quad \text {for the remaining pairs} (j, k) \\ & x & \geq 0. \end{array}
$$

Denoting by $x ^ { i + 1 } , z _ { 1 } ^ { i + 1 } , \dotsc , z _ { S } ^ { i + 1 }$ an optimal solution to this linear program we get an upper bound on the optimal value of (16.5): 

$$
U B = a ^ {T} x ^ {i + 1} + z _ {1} ^ {i + 1} + \ldots + z _ {S} ^ {i + 1}.
$$

Benders decomposition alternately solves the recourse problems (16.8) and the master linear program with new optimality and feasibility cuts added at each iteration until the gap between the upper bound UB and the lower bound LB falls below a given threshold. One can show that $U B - L B$ converges to zero in a finite number of iterations. See, for instance, the book of Birge and Louveaux [12], pages 159-162. 

Benders decomposition can also be used for multi-stage problems (16.6) in a straightforward way: The stages are partitioned into a first set that gives rise to the “master problem” and a second set that gives rise to the “recourse problems”. For example in a 6-stage problem, the variables of the first 2 stages could define the master problem. When these variables are fixed, (16.6) decomposes into separate linear programs each involving variables of the last 4 stages. The solutions of these recourse linear programs provide optimality or feasibility cuts that can be added to the master problem. As before, upper and lower bounds are computed at each iteration and the algorithm stops when the diference drops below a given tolerance. Using this approach, Gondzio and Kouwenberg [32] were able to solve an asset liability management problem with over 4 million scenarios, whose linear programming formulation (16.6) had 12 million constraints and 24 million variables. This linear program was so large that storage space on the computer became an issue. The scenario tree had 6 levels and 13 branches at each node. In order to apply two-stage Benders decomposition, Gondzio and Kouwenberg divided the 6 period problem into a first stage problem containing the first 3 periods and a second stage containing periods 4 to 6. This resulted in 2,197 recourse linear programs, each involving 2,197 scenarios. These recourse linear programs were solved by an interior point algorithm. Note that Benders decomposition is ideally suited for parallel computations since the recourse linear programs can be solved simultaneously. When the solution of all the recourse linear programs is completed (which takes the bulk of the time), the master problem is then solved on one processor while the other processors remain idle temporarily. Gondzio and Kouwenberg tested a parallel implementation on a computer with 16 processors and they obtained an almost perfect speedup, that is a speedup factor of almost k when using k processors. 

## 16.5 Scenario Generation

How should one generate scenarios in order to formulate a deterministic equivalent formulation (16.6) that accurately represents the underlying stochastic program? There are two separate issues. First, one needs to model the correlation over time among the random parameters. For a pension fund, such a model might relate wage inflation (which influences the liability side) to interest rates and stock prices (which influence the asset side). Mulvey [53] describes the system developed by Towers Perrin, based on a cascading set of stochastic diferential equations. Simpler autoregressive models can also be used. This is discussed below. The second issue is the construction of a scenario tree from these models: A finite number of scenarios must reflect as accurately as possible the random processes modeled in the previous step, suggesting the need for a large number of scenarios. On the other hand, the linear program (16.6) can only be solved if the size of the scenario tree is reasonably small, suggesting a rather limited number of scenarios. To reconcile these two conflicting objectives, it might be crucial to use variance reduction techniques. We address these issues in this section. 

## 16.5.1 Autoregressive model

In order to generate the random parameters underlying the stochastic program, one needs to construct an economic model reflecting the correlation between the parameters. Historic data may be available. The goal is to generate meaningful time series for constructing the scenarios. One approach is to use an autoregressive model. 

Specifically, if $r _ { t }$ denotes the random vector of parameters in period $t ,$ an autoregressive model is defined by: 

$$
r _ {t} = D _ {0} + D _ {1} r _ {t - 1} + \ldots + D _ {p} r _ {t - p} + \epsilon_ {t}
$$

where $p$ is the number of lags used in the regression, $D _ { 0 } , D _ { 1 } , \ldots , D _ { p }$ are time independent constant matrices which are estimated through statistical methods such as maximum likelihood, and $\epsilon _ { t }$ is a vector of i.i.d. random disturbances with mean zero. 

To illustrate this, consider the example of Section 8.1.1. Let $s _ { t } , b _ { t }$ and $m _ { t }$ denote the rates of return of stocks, bonds and the money market, respectively, in year t. An autoregressive model with $p = 1$ has the form: 

$$
\left( \begin{array}{c} s _ {t} \\ b _ {t} \\ m _ {t} \end{array} \right) = \left( \begin{array}{c} d _ {1} \\ d _ {2} \\ d _ {3} \end{array} \right) + \left( \begin{array}{c c c} d _ {1 1} & d _ {1 2} & d _ {1 3} \\ d _ {2 1} & d _ {2 2} & d _ {2 3} \\ d _ {3 1} & d _ {3 2} & d _ {3 3} \end{array} \right) \left( \begin{array}{c} s _ {t - 1} \\ b _ {t - 1} \\ m _ {t - 1} \end{array} \right) + \left( \begin{array}{c} \epsilon_ {t} ^ {s} \\ \epsilon_ {t} ^ {b} \\ \epsilon_ {t} ^ {m} \end{array} \right) t = 2, \ldots , T
$$

In particular, to find the parameters $d _ { 1 } , d _ { 1 1 } , d _ { 1 2 } , d _ { 1 3 }$ in the first equation 

$$
{s _ {t}} = {d _ {1} + d _ {1 1} s _ {t - 1} + d _ {1 2} b _ {t - 1} + d _ {1 3} m _ {t - 1} + \epsilon_ {t} ^ {s}}
$$

one can use standard linear regression tools that minimize the sum of the squared errors $\epsilon _ { t } ^ { s } .$ . Within an Excel spreadsheet for instance, one can use the function LINEST. Suppose that the rates of return on the stocks are stored in cells B2 to B44 and that, for bonds and the money market, the rates are stored in columns C and D, rows 2 to 44 as well. LINEST is an array formula. Its first argument contains the known data for the left hand side of the equation (here the column $s _ { t } )$ , the second argument contains the known data in the right hand side (here the columns $s _ { t - 1 } , b _ { t - 1 }$ and $m _ { t - 1 } )$ Typing LINEST(B3:B44, B2:D43,,) one obtains the following values of the parameters: 

$$
d _ {1} = 0. 0 7 7, d _ {1 1} = - 0. 0 5 8, d _ {1 2} = 0. 2 1 9, d _ {1 3} = 0. 4 4 8.
$$

Using the same approach for the other two equations we get the following autoregressive model: 

$$
s _ {t} = 0. 0 7 7 - 0. 0 5 8 s _ {t - 1} + 0. 2 1 9 b _ {t - 1} + 0. 4 4 8 m _ {t - 1} + \epsilon_ {t} ^ {s}
$$

$$
{b _ {t}} = {0. 0 4 7 - 0. 0 5 3 s _ {t - 1} - 0. 0 7 8 b _ {t - 1} + 0. 7 0 7 m _ {t - 1} + \epsilon_ {t} ^ {b}}
$$

$$
m _ {t} = 0. 0 1 6 + 0. 0 3 3 s _ {t - 1} - 0. 0 4 4 b _ {t - 1} + 0. 7 4 6 m _ {t - 1} + \epsilon_ {t} ^ {m}
$$

The option LINEST(B3:B44, B2:D43,,TRUE) provides some useful statistics, such as the standard error of the estimate $s _ { t }$ . Here we get a standard error of $\sigma _ { s } = 0 . 1 7 3$ . Similarly, the standard error for $b _ { t }$ and $m _ { t }$ are $\sigma _ { b } = 0 . 1 0 8$ and $\sigma _ { m } = 0 . 0 2 2$ respectively. 

Exercise 16.5 Instead of an autoregressive model relating the rates of returns $r _ { t } , \ b _ { t }$ and $m _ { t }$ , construct an autoregressive model relating the logarithms of the returns $g _ { t } = l o g ( 1 + r _ { t } ) , h _ { t } = l o g ( 1 + b _ { t } )$ and $k _ { t } = l o g ( 1 + m _ { t } )$ Use one lag, i.e. $p = 1$ . Solve using LINEST or your prefered linear regression tool. 

Exercise 16.6 In the above autoregressive model, the coeficients of $m _ { t - 1 }$ are significantly larger than those of $s t { - 1 }$ and $b _ { t - 1 }$ . This suggests that these two variables might not be useful in the regression. Resolve the example assuming the following autoregressive model: 

$$
{s _ {t}} = {d _ {1} + d _ {1 3} m _ {t - 1} + \epsilon_ {t} ^ {s}}
$$

$$
{b _ {t}} = {d _ {2} + d _ {2 3} m _ {t - 1} + \epsilon_ {t} ^ {b}}
$$

$$
m _ {t} = d _ {3} + d _ {3 3} m _ {t - 1} + \epsilon_ {t} ^ {m}
$$

## 16.5.2 Constructing scenario trees

The random distributions relating the various parameters of a stochastic program must be discretized to generate a set of scenarios that is adequate for its deterministic equivalent. Too few scenarios may lead to approximation errors. On the other hand, too many scenarios will lead to an explosion in the size of the scenario tree, leading to an excessive computational burden. In this section, we discuss a simple random sampling approach and two variance reduction techniques: adjusted random sampling and tree fitting. Unfortunately, scenario trees constructed by these methods could contain spurious arbitrage opportunities. We end this section with a procedure to test that this does not occur. 

## Random sampling

One can generate scenarios directly from the autoregressive model introduced in the previous section: 

$$
r _ {t} = D _ {0} + D _ {1} r _ {t - 1} + \ldots + D _ {p} r _ {t - p} + \epsilon_ {t}
$$

where $\epsilon _ { t } \sim N ( 0 , \Sigma )$ are independently distributed multivariate normal distributions with mean 0 and covariance matrix Σ. 

In our example, Σ is a $3 \times 3$ diagonal matrix, with diagonal entries $\sigma _ { s } , \ \sigma _ { b }$ and $\sigma _ { m } .$ . Using the parameters $\sigma _ { s } = 0 . 1 7 3 , \sigma _ { b } = 0 . 1 0 8 , \sigma _ { m } = 0 . 0 2 2$ computed earlier, and a random number generator, we obtained $\epsilon _ { t } ^ { s } = - 0 . 1 8 6$ $\epsilon _ { t } ^ { b } = 0 . 0 5 2$ and $\epsilon _ { t } ^ { m } = 0 . 0 0 7$ . We use the autoregressive model to get rates of return for 2004 based on the known rates of returns for 2003 (see Table in Section 8.1.1): 

$$
s _ {2 0 0 4} = 0. 0 7 7 - 0. 0 5 8 \times 0. 2 8 6 8 + 0. 2 1 9 \times 0. 0 0 5 4 + 0. 4 4 8 \times 0. 0 0 9 8 - 0. 1 8 6 = - 0. 0 8 7
$$

$$
b _ {2 0 0 4} = 0. 0 4 7 - 0. 0 5 3 \times 0. 2 8 6 8 - 0. 0 7 8 \times 0. 0 0 5 4 + 0. 7 0 7 \times 0. 0 0 9 8 + 0. 0 5 2 = 0. 0 9 1
$$

$$
m _ {2 0 0 4} = 0. 0 1 6 + 0. 0 3 3 \times 0. 2 8 6 8 - 0. 0 4 4 \times 0. 0 0 5 4 + 0. 7 4 6 \times 0. 0 0 9 8 + 0. 0 0 7 = 0. 0 4 0
$$

These are the rates of return for one of the branches from node 1. For each of the other branches from node 1, one generates random values of $\epsilon _ { t } ^ { s } , \epsilon _ { t } ^ { b }$ and $\epsilon _ { t } ^ { m }$ and computes the corresponding values of s<sub>2004</sub>, $b _ { 2 0 0 4 }$ and m<sub>2004</sub>. Thirty branches or so may be needed to get a reasonable approximation of the distribution of the rates of return in stage 1. For a problem with 

3 stages, 30 branches at each stage represent 27,000 scenarios. With more stages, the size of the linear program (16.6) explodes. Kouwenberg [45] performed tests on scenario trees with fewer branches at each node (such as a 5-stage problem with branching structure 10-6-6-4-4, meaning 10 branches at the root, then 6 branches at each node in the next stage and so on) and he concluded that random sampling on such trees leads to unstable investment strategies. This occurs because the approximation error made by representing parameter distributions by random samples can be significant in a small scenario tree. As a result the optimal solution of (16.6) is not optimal for the actual parameter distributions. How can one construct a scenario tree that more accurately represents these distributions, without blowing up the size of (16.6)? 

## Adjusted random sampling

An easy way of improving upon random sampling is as follows. Assume that each node of the scenario tree has an even number $K = 2 k$ of branches. Instead of generating 2k random samples from the autoregressive model, generate k random samples only and use the negative of their error terms to compute the values on the remaining k branches. This will fit all the odd moments of the distributions correctly. In order to fit the variance of the distributions as well, one can scale the sampled values. The sampled values are all scaled by a multiplicative factor until their variance fits that of the corresponding parameter. 

As an example, corresponding to the branch with $\epsilon _ { t } ^ { s } = - 0 . 1 8 6 , \epsilon _ { t } ^ { b } = 0 . 0 5 2$ and $\epsilon _ { t } ^ { m } = 0 . 0 0 7$ at node 1, one would also generate another branch with $\epsilon _ { t } ^ { s } = 0 . 1 8 6 , \epsilon _ { t } ^ { b } = - 0 . 0 5 2$ and $\epsilon _ { t } ^ { m } = - 0 . 0 0 7$ . For this branch the autoregressive model gives the following rates of return for 2004: 

$$
s _ {2 0 0 4} = 0. 0 7 7 - 0. 0 5 8 \times 0. 2 8 6 8 + 0. 2 1 9 \times 0. 0 0 5 4 + 0. 4 4 8 \times 0. 0 0 9 8 + 0. 1 8 6 = 0. 2 8 5
$$

$$
b _ {2 0 0 4} = 0. 0 4 7 - 0. 0 5 3 \times 0. 2 8 6 8 - 0. 0 7 8 \times 0. 0 0 5 4 + 0. 7 0 7 \times 0. 0 0 9 8 - 0. 0 5 2 = - 0. 0 1 3
$$

$$
m _ {2 0 0 4} = 0. 0 1 6 + 0. 0 3 3 \times 0. 2 8 6 8 - 0. 0 4 4 \times 0. 0 0 5 4 + 0. 7 4 6 \times 0. 0 0 9 8 - 0. 0 0 7 = 0. 0 2 6
$$

Suppose that the set of $\epsilon _ { t } ^ { s }$ generated on the branches leaving from node 1 has standard deviation 0.228 but the corresponding parameter should have standard deviation 0.165. Then the $\epsilon _ { t } ^ { s }$ would be scaled down by $\frac { 0 . 1 6 5 } { 0 . 2 2 8 }$ on all the branches from node 1. For example, instead of $\epsilon _ { t } ^ { s } = - 0 . 1 8 6$ on the branch discussed earlier, one would use $\begin{array} { r } { \epsilon _ { t } ^ { s } = - 0 . 1 8 6 \frac { 0 . 1 6 5 } { 0 . 2 2 8 } = - 0 . 1 3 5 } \end{array}$ . This corresponds to the following rate of return: 

$$
s _ {2 0 0 4} = 0. 0 7 7 - 0. 0 5 8 \times 0. 2 8 6 8 + 0. 2 1 9 \times 0. 0 0 5 4 + 0. 4 4 8 \times 0. 0 0 9 8 - 0. 1 3 5 = - 0. 0 3 6
$$

The rates of returns on all the branches from node 1 would be modified in the same way. 

## Tree fitting

How can one best approximate a continuous distribution by a discrete distribution with K values? In other words, how should one choose values $v _ { k }$ and their probabilities $p _ { k }$ , for $k = 1 , \ldots , K$ , in order to approximate the given distribution as accurately as possible? A natural answer is to match as many of the moments as possible. In the context of a scenario tree, the problem is somewhat more complicated since there are several correlated parameters at each node and there is interdependence between periods as well. Hoyland and Wallace [39] propose to formulate this fitting problem as a nonlinear program. The fitting problem can be solved either at each node separately or on the overall tree. We explain the fitting problem at a node. Let $S _ { l }$ be the values of the statistical properties of the distributions that one desires to fit, for $l = 1 , \ldots , s .$ . These might be the expected values of the distributions, the correlation matrix, the skewness and kurtosis. Let $v _ { k }$ and $p _ { k }$ denote the vector of values on branch k and its probability, respectively, for $k = 1 , \ldots , K$ . Let $f _ { l } ( v , p )$ be the mathematical expression of property l for the discrete distribution (for example, the mean of the vectors $v _ { k } .$ , their correlation, skewness and kurtosis). Each property has a positive weight w<sub>l</sub> indicating its importance in the desired fit. Hoyland and Wallace formulate the fitting problem as 

$$
\begin{array}{r l} \min _ {v, p} & \sum_ {l} w _ {l} (f _ {l} (v, p) - S _ {l}) ^ {2} \\ & \sum_ {k} p _ {k} = 1 \\ & p \geq 0 \end{array}\tag{16.11}
$$

One might want some statistical properties to match exactly. As an example, consider again the autoregressive model: 

$$
r _ {t} = D _ {0} + D _ {1} r _ {t - 1} + \ldots + D _ {p} r _ {t - p} + \epsilon_ {t}
$$

where $\epsilon _ { t } \sim N ( 0 , \Sigma )$ are independently distributed multivariate normal distributions with mean 0 and covariance matrix Σ. To simplify notation, let us write  instead of $\epsilon _ { t } .$ . The random vector  has distribution $N ( 0 , \Sigma )$ and we would like to approximate this continuous distribution by a finite number of disturbance vectors $\epsilon ^ { k }$ occuring with probability $p _ { k }$ , for $k = 1 , \ldots , K$ . Let $\epsilon _ { q } ^ { k }$ denote the qth component of vector $\epsilon ^ { k }$ . One might want to fit the mean of  exactly and its covariance matrix as well as possible. In this case, the fitting problem is: 

$$
\begin{array}{r l} \min _ {\epsilon^ {1}, \dots , \epsilon^ {K}, p} & \sum_ {q = 1} ^ {l} \sum_ {r = 1} ^ {l} (\sum_ {k = 1} ^ {K} p _ {k} \epsilon_ {q} ^ {k} \epsilon_ {r} ^ {k} - \Sigma_ {q r}) ^ {2} \\ & \sum_ {k = 1} ^ {K} p _ {k} \epsilon^ {k} = 0 \\ & \sum_ {k} p _ {k} = 1 \\ & p \geq 0 \end{array}
$$

## Arbitrage-free scenario trees

Approximating the continuous distributions of the uncertain parameters by a finite number of scenarios in the linear programming (16.6) typically creates modeling errors. In fact, if the scenarios are not chosen properly or if their number is too small, the supposedly “linear programming equivalent” could be far from being equivalent to the original stochastic program. One of the most disturbing aspects of this phenomenon is the possibility of creating arbitrage opportunities when constructing the scenario tree. When this occurs, model (16.6) might produce unrealistic solutions that exploit these arbitrage opportunities. Klaassen [42] was the first to address this issue. In particular, he shows how arbitrage opportunities can be detected ex post in a scenario tree. When such arbitrage opportunities exist, a simple solution is to discard the scenario tree and to construct a new one with more branches. Klaassen [42] also discusses what constraints to add to the nonlinear program (16.11) in order to preclude arbitrage opportunities ex ante. The additional constraints are nonlinear, thus increasing the dificulty of solving (16.11). We present below Klassen’s ex post check. 

Recall that there are two types of arbitrage (Definition 4.1). We start we Type A. An arbitrage of Type A is a trading strategy with an initial positive cash flow and no risk of loss later. Let us express this at a node i of the scenario tree. Let $r ^ { k }$ denote the vectors of rates of return on the branches connecting node i to its sons in the next stage, for $k = 1 , \ldots , K$ . There exists an arbitrage of Type A if there exists an asset allocation $x = ( x _ { 1 } , \ldots , x _ { Q } )$ at node i such that O 

$$
\sum_ {q = 1} ^ {Q} x _ {q} <   0
$$

$$
\text { and } \quad \sum_ {q = 1} ^ {Q} x _ {q} r _ {q} ^ {k} \geq 0 \quad \text { for   all } k = 1, \ldots , K.
$$

To check whether such an allocation x exists, it sufices to solve the linear program 

$$
\begin{array}{r l} \min _ {x} & \sum_ {q = 1} ^ {Q} x _ {q} \\ & \sum_ {q = 1} ^ {Q} x _ {q} r _ {q} ^ {k} \geq 0 \quad \text {for all} k = 1, \ldots , K. \end{array}\tag{16.12}
$$

There is an arbitrage opportunity of Type A at node i if and only if this linear program is unbounded. 

Next we turn to Type B. An arbitrage of Type B requires no initial cash input, has no risk of a loss and a positive probability of making profits in the future. At node i of the scenario tree, this is expressed by the conditions: 

$$
\sum_ {q = 1} ^ {Q} x _ {q} = 0,
$$

$$
\sum_ {q = 1} ^ {Q} x _ {q} r _ {q} ^ {k} \geq 0 \quad \mathrm{forall} k = 1, \ldots , K
$$

$$
\text { and } \quad \sum_ {q = 1} ^ {Q} x _ {q} r _ {q} ^ {k} > 0 \quad \text { for   at   least   one } k = 1, \ldots , K.
$$

These conditions can be checked by solving the linear program 

$$
\begin{array}{r l} \max _ {x} & \sum_ {q = 1} ^ {Q} x _ {q} r _ {q} ^ {k} \\ & \sum_ {q = 1} ^ {Q} x _ {q} = 0 \\ & \sum_ {q = 1} ^ {Q} x _ {q} r _ {q} ^ {k} \geq 0 \quad \mathrm{forall} k = 1, \ldots , K. \end{array}\tag{16.13}
$$

## 16.5. SCENARIO GENERATION

There is an arbitrage opportunity of Type B at node i if and only if this linear program is unbounded. 

Exercise 16.7 Show that the linear program (16.12) is always feasible. 

Write the dual linear program of (16.12). Let $u _ { k }$ be the dual variable associated with the kth constraint of (16.12). 

Recall that a feasible linear program is unbounded if and only if its dual is infeasible. Show that there is no arbitrage of Type A at node i if and only if there exists $u _ { k } \geq 0$ , for $k = 1 , \ldots , K$ such that 

$$
\sum_ {k = 1} ^ {K} u _ {k} r _ {q} ^ {k} = 1 \quad \mathrm{forall} q = 1, \ldots , Q.
$$

Similarly, write the dual of (16.13). Let $v _ { 0 } , v _ { k }$ , for $k = 1 , \ldots , K$ be the dual variables. Write necessary and suficient conditions for the nonexistence of arbitrage of Type B at node i, in terms of $v _ { k }$ , for $k = 0 , \ldots , K$ 

Modify the nonlinear program (16.11) in order to formulate a fitting problem at node i that contains no arbitrage opportunities. 

# 270CHAPTER 16. STOCHASTIC PROGRAMMING: THEORY AND ALGORITHMS

Chapter 17 

# SP Models: Value-at-Risk and Conditional Value-at-Risk

In this chapter, we discuss Value-at-Risk, a widely used measure of risk in finance, and its relative Conditional Value-at-Risk. We then present an optimization model that optimizes a portfolio when the risk measure is the Conditional Value-at-Risk instead of the variance of the portfolio as in the Markowitz model. This is acheived through stochastic programming. In this case, the variables are anticipative. The random events are modeled by a large but finite set of scenarios, leading to a linear programming equivalent of the original stochastic program. 

## 17.1 Risk Measures

Financial activities involve risk. Our stock or mutual fund holdings carry the risk of losing value due to market conditions. Even money invested in a bank carries a risk–that of the bank going bankrupt and never returning the money let alone some interest. While individuals generally just have to live with such risks, financial and other institutions can and very often must manage risk using sophisticated mathematical techniques. Managing risk requires a good understanding of quantitative risk measures that adequately reflect the vulnerabilities of a company. 

Perhaps the best-known risk measure is Value-at-Risk (VaR) developed by financial engineers at J.P. Morgan. VaR is a measure related to percentiles of loss distributions and represents the predicted maximum loss with a specified probability level (e.g., 95%) over a certain period of time (e.g., one day). Consider, for example, a random variable X that represents loss from an investment portfolio over a fixed period of time. A negative value for X indicates gains. Given a probability level α, α-VaR of the random variable X is given by the following relation: 

$$
\operatorname{VaR} _ {\alpha} (X) := \min \{\gamma : P (X \geq \gamma) \leq 1 - \alpha \}.\tag{17.1}
$$

When the loss distribution is continuous, $\operatorname { V a R } _ { \alpha } ( X )$ is simply the loss such that 

$$
P (X \leq \mathrm{VaR} _ {\alpha} (X)) = \alpha .
$$

The following figure illustrates the 0.95-VaR on a portfolio loss distribution plot: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/e49ca90934f119554754ffefda5130886537bd0cba0f1813ea31f85e9a1dd78f.jpg)


VaR is widely used by people in the financial industry and VaR calculators are common features in most financial software. Despite this popularity, VaR has one important undesirable property–it lacks subadditivity. Risk measures should respect the maxim “diversification reduces risk” and therefore, satisfy the following property: “The total risk of two diferent investment portfolios does not exceed the sum of the individual risks.” This is precisely what we mean by saying that a risk measure should be a subadditive function, i.e., for a risk measure $f ,$ we should have 

$$
f (x _ {1} + x _ {2}) \leq f (x _ {1}) + f (x _ {2}), \forall x _ {1}, x _ {2}.
$$

Consider the following simple example that illustrates that diversification can actually increase the risk measured by VaR: 

Example 17.1 Consider two independent investment opportunities each returning a $1 gain with probability 0.96 and $2 loss with probability $0 . 0 4 \cdot$ Then, 0.95-VaR for both investments are -1. Now consider the sum of these two investment opportunities. Because of independence, this sum has the following loss distribution: $\$ 4$ with probability $0 . 0 4 \times 0 . 0 4 = 0 . 0 0 1 6 .$ , $1 with probability $2 \times 0 . 9 6 \times 0 . 0 4 = 0 . 0 7 6 8$ , and -$2 with probability $0 . 9 6 \times 0 . 9 6 =$ 0.9216. Therefore, the 0.95-VaR of the sum of the two investments is 1, which exceeds -2, the sum of the 0.95-VaR values for individual investments. 

An additional dificulty with VaR is in its computation and optimization. When VaR is computed by generating scenarios, it turns out to be a non-smooth and non-convex function of the positions in the investment portfolio. Therefore, when one tries to optimize VaR computed in this manner, multiple local optimizers are encountered, hindering the global optimization process. 

Another criticism of VaR is that it pays no attention to the magnitude of losses beyond the VaR value. This and other undesirable features of VaR led to the development of alternative risk measures. One well-known modification of VaR is obtained by computing the expected loss given that the loss exceeds VaR. This quantity is often called conditional Value-at-Risk or CVaR. There are several alternative names for this measure in the finance literature including Mean Expected Loss, Mean Shortfall, and Tail VaR. We now describe this risk measure in more detail and discuss how it can be optimized using linear programming techniques when the loss function is linear in the portfolio positions. Our discussion follows parts of articles by Rockafellar and Uryasev [61, 73]. 

We consider a portfolio of assets with random returns. We denote the portfolio choice vector by x and the random events by the vector $y .$ . Let $f ( x , y )$ denote the loss function when we choose the portfolio x from a set X of feasible portfolios and $y$ is the realization of the random events. We assume that the random vector $y$ has a probability density function denoted by p(y). 

For a fixed decision vector x, we compute the cumulative distribution function of the loss associated with that vector x: 

$$
\Psi (x, \gamma) := \int_ {f (x, y) <   \gamma} p (y) d y.\tag{17.2}
$$

Then, for a given confidence level $\alpha$ , the α-VaR associated with portfolio x is given by 

$$
\operatorname{VaR} _ {\alpha} (x) := \min \{\gamma \in I R: \Psi (x, \gamma) \geq \alpha \}.\tag{17.3}
$$

We define the α-CVaR associated with portfolio x as: 

$$
\mathrm{CVaR} _ {\alpha} (x) := \frac {1}{1 - \alpha} \int_ {f (x, y) \geq \mathrm{VaR} _ {\alpha} (x)} f (x, y) p (y) d y.\tag{17.4}
$$

Note that, 

$$
\begin{array}{r c l} \mathrm{CVaR} _ {\alpha} (x) & = & \frac {1}{1 - \alpha} \int_ {f (x, y) \geq \mathrm{VaR} _ {\alpha} (x)} f (x, y) p (y) d y \\ & \geq & \frac {1}{1 - \alpha} \int_ {f (x, y) \geq \mathrm{VaR} _ {\alpha} (x)} \mathrm{VaR} _ {\alpha} (x) p (y) d y \\ & = & \frac {\mathrm{VaR} _ {\alpha} (x)}{1 - \alpha} \int_ {f (x, y) \geq \mathrm{VaR} _ {\alpha} (x)} p (y) d y \\ & \geq & \mathrm{VaR} _ {\alpha} (x), \end{array}
$$

i.e., CVaR of a portfolio is always at least as big as its VaR. Consequently, portfolios with small CVaR also have small VaR. However, in general minimizing CVaR and VaR are not equivalent. 

For a discrete probability distribution (where event $y _ { j }$ occurs with probability $p _ { j }$ , for $j = 1 , \ldots , n )$ , the above definition of CVaR becomes 

$$
\operatorname{CVaR} _ {\alpha} (x) = \frac {1}{1 - \alpha} \sum_ {j: f (x, y _ {j}) \geq \operatorname{VaR} _ {\alpha} (x)} p _ {j} f (x, y _ {j})
$$

Example: 

Suppose we are given the loss function $f ( x , y )$ for a given decision $x$ as $f ( x , y ) = - y$ where $y = 7 5 - j$ with probability 1 % for $j = 0 , \ldots , 9 9$ . We would like to determine the Value-at-Risk $\operatorname { V a R } _ { \alpha } ( x )$ for $\alpha = 9 5 \%$ . We have $\mathrm { V a R } _ { 9 5 \% } ( x ) = 2 0$ since the loss is 20 or more with probability $5 \ \%$ 

To compute the Conditional Value-at-Risk, we use the above formula: $\begin{array} { r } { \mathrm { C V a R } _ { 9 5 \% } ( x ) = \frac { 1 } { 0 . 0 5 } ( 2 0 + 2 1 + 2 2 + 2 3 + 2 4 ) \times 1 \% = 2 2 . } \end{array}$ 

Exercise 17.1 (a) Compute the 0.90-VaR and 0.90-CVaR for the rates of return of stocks between 1961 and 2003 (see Section 8.1.1 for the data). 

(b) Compute the 0.90-VaR and 0.90-CVaR for the rates of return of bonds and a money market account. Again use the data of Section 8.1.1. 

Exercise 17.2 Give an example showing that CVaR is not subadditive. 

## 17.2 Minimizing CVaR

Since the definition of CVaR involves the VaR function explicitly, it is difficult to work with and optimize this function. Instead, we consider the following simpler auxiliary function: 

$$
F _ {\alpha} (x, \gamma) := \gamma + \frac {1}{1 - \alpha} \int_ {f (x, y) \geq \gamma} (f (x, y) - \gamma) p (y) d y.\tag{17.5}
$$

Alternatively, we can write $F _ { \alpha , x } ( \gamma )$ as follows: 

$$
F _ {\alpha} (x, \gamma) = \gamma + \frac {1}{1 - \alpha} \int (f (x, y) - \gamma) ^ {+} p (y) d y,\tag{17.6}
$$

where $a ^ { + } = \operatorname* { m a x } \{ a , 0 \}$ . This function, viewed as a function of $\gamma$ , has the following important properties that make it useful for the computation of VaR and CVaR: 

1. $F _ { \alpha } ( x , \gamma )$ is a convex function of $\gamma$ . 

2. $\operatorname { V a R } _ { \alpha } ( x )$ is a minimizer over $\gamma$ of $F _ { \alpha } ( x , \gamma )$ 

3. The minimum value over $\gamma$ of the function $F _ { \alpha } ( x , \gamma )$ is $\operatorname { C V a R } _ { \alpha } ( x )$ 

Exercise 17.3 Prove the properties of $F _ { \alpha , x } ( \gamma )$ stated above. 

As a consequence of the listed properties, we immediately deduce that, in order to minimize $\operatorname { C V a R } _ { \alpha } ( x )$ over $x ,$ we need to minimize the function $F _ { \alpha } ( x , \gamma )$ with respect to x and γ simultaneously: 

$$
\min _ {x \in X} \mathrm{CVaR} _ {\alpha} (x) = \min _ {x \in X, \gamma} F _ {\alpha} (x, \gamma).\tag{17.7}
$$

Consequently, we can optimize CVaR directly, without needing to compute VaR first. If the loss function $f ( x , y )$ is a convex (linear) function of the portfolio variables $x ,$ then $F _ { \alpha } ( x , \gamma )$ is also a convex (linear) function of $x .$ In this case, provided the feasible portfolio set X is also convex, the optimization problems in (17.7) are smooth convex optimization problems that can be solved using well known optimization techniques for such problems (see Chapter 5). 

Often it is not possible or desirable to compute/determine the joint density function $p ( y )$ of the random events in our formulation. Instead, we may have a number of scenarios, say $y _ { s }$ for $s = 1 , \ldots , S$ , which may represent some historical values of the random events or some values obtained via computer simulation. We will assume that all scenarios have the same probability. In this case, we obtain the following approximation to the function $F _ { \alpha } ( x , \gamma )$ by using the empirical distribution of the random events based on the available scenarios: 

$$
\tilde {F} _ {\alpha} (x, \gamma) := \gamma + \frac {1}{(1 - \alpha) S} \sum_ {s = 1} ^ {S} (f (x, y _ {s}) - \gamma) ^ {+}.\tag{17.8}
$$

Compare this definition to (17.6). Now, the problem min ${ } _ { x \in X } \operatorname { C V a R } _ { \alpha } ( x )$ can be approximated by replacing $F _ { \alpha } ( x , \gamma )$ with $\tilde { F } _ { \alpha } ( x , \gamma )$ in (17.7): 

$$
\min _ {x \in X, \gamma} \gamma + \frac {1}{(1 - \alpha) S} \sum_ {s = 1} ^ {S} (f (x, y _ {s}) - \gamma) ^ {+}.\tag{17.9}
$$

To solve this optimization problem, we introduce artificial variables $z _ { s }$ to replace $( f ( x , y _ { s } ) - \gamma ) ^ { + }$ . This is achieved by imposing the constraints $z _ { s } \ge$ $f ( x , y _ { s } ) - \gamma$ and $z _ { s } \geq 0 ;$ 

$$
\begin{array}{r l r l} \min _ {x, z, \gamma} & \gamma + \frac {1}{(1 - \alpha) S} \sum_ {s = 1} ^ {S} z _ {s} \\ \text {s.t.} & z _ {s} & \geq & 0, s = 1, \ldots , S, \\ & z _ {s} & \geq & f (x, y _ {s}) - \gamma , s = 1, \ldots , S, \\ & x \in X. \end{array}\tag{17.10}
$$

Note that the constraints $z _ { s } \ge f ( x , y _ { s } ) - \gamma$ and $z _ { s } \ge 0$ alone cannot ensure that $z _ { s } = ( f ( x , y _ { s } ) - \gamma ) ^ { + } = \operatorname* { m a x } \{ f ( x , y _ { s } ) - \gamma , 0 \}$ since $z _ { s }$ can be larger than both right-hand-sides and be still feasible. However, since we are minimizing the objective function which involves a positive multiple of $z _ { s } ,$ it will never be optimal to assign $z _ { s }$ a value larger than the maximum of the two quantities $f ( x , y _ { s } ) - \gamma$ and 0, and therefore, in an optimal solution $z _ { s }$ will be precisely $( f ( x , y _ { s } ) - \gamma ) ^ { + }$ , justifying our substitution. 

In the case that $f ( x , y )$ is linear in x, all the expressions $z _ { s } \ge f ( x , y _ { s } ) - \gamma$ represent linear constraints and therefore the problem (17.10) is a linear programming problem that can be solved using the simplex method or alternative LP algorithms. 

Other optimization problems arise naturally within the context of risk management. For example, risk managers often try to optimize a performance measure (e.g., expected return) while making sure that certain risk measures do not exceed a threshold value. When the risk measure is CVaR, the resulting optimization problem is: 

$$
\begin{array}{r l r} \max _ {x} & \mu^ {T} x \\ \text {s.t.} & \mathrm{CVaR} _ {\alpha^ {j}} (x) & \leq U _ {\alpha^ {j}}, j = 1, \ldots , J \\ & x \in X. \end{array}\tag{17.11}
$$

Above, J is an index set for diferent confidence levels used for CVaR computations and $U _ { \alpha ^ { j } }$ represents the maximum tolerable CVaR value at the confidence level $\alpha ^ { j }$ . As above, we can replace the CVaR functions in the constraints of this problem with the function $F _ { \alpha } ( x , \gamma )$ as above and then approximate this function using the scenarios for random events. This approach results in the following approximation of the CVaR-constrained problem (17.11): 

$$
\begin{array}{r l r} \max _ {x, z, \gamma} & \mu^ {T} x \\ \mathrm{s.t.} & \gamma + \frac {1}{(1 - \alpha^ {j}) S} \sum_ {s = 1} ^ {S} z _ {s} & \leq U _ {\alpha^ {j}}, j = 1, \ldots , J, \\ & z _ {s} & \geq 0, s = 1, \ldots , S, \\ & z _ {s} & \geq f (x, y _ {s}) - \gamma , s = 1, \ldots , S, \\ & x \in X. \end{array}\tag{17.12}
$$

## 17.3 Example: Bond Portfolio Optimization

A portfolio of risky bonds might be characterized by a large likelihood of small earnings, coupled with a small chance of loosing a large amount of the investment. The loss distribution is heavily skewed and, in this case, standard mean-variance analysis to characterize market risk is inadequate. VaR and CVaR are more appropriate criteria for minimizing portfolio credit risk. Credit risk is the risk of a trading partner not fulfilling their obligation in full on the due date or at any time thereafter. Losses can result both from default and from a decline in market value stemming from downgrades in credit ratings. A good reference is the paper of Anderson, Mausser, Rosen and Uryasev [2]. 

Anderson, Mausser, Rosen and Uryasev consider a portfolio of 197 bonds from 29 diferent countries with a market value of $ 8.8 billion and duration of approximately 5 years. Their goal is to rebalance the portfolio in order to minimize credit risk. That is they want to minimize losses resulting from default and from a decline in market value stemming from downgrades in credit ratings (credit migration). The loss due to credit migration is simply 

$$
f (x, y) = (b - y) ^ {T} x
$$

where b are the future values of each bond with no credit migration and y are the future values with credit migration (so y is a random vector). The one-year portfolio credit loss was generated using a Monte Carlo simulation: 20,000 scenarios of joint credit states of obligators and related losses. The distribution of portfolio losses has a long fat tail. The authors rebalanced the portfolio by minimizing CVaR. The set X of feasible porfolios was described by the following constraints. Let x<sub>i</sub> denote the weight of asset i in the portfolio. Upper and lower bounds were set on each x : 

$$
\begin{array}{r l} {l _ {i} \leq x _ {i} \leq u _ {i}} & {i = 1, \ldots , n} \\ {\sum_ {i} x _ {i} = 1} \end{array}
$$

To calculate the eficient frontier, the expected portfolio return was set to at least R: 

$$
\sum_ {i} \mu_ {i} x _ {i} \geq R
$$

To summarize, the linear program (17.10) to be solved was as follows: 

$$
\begin{array}{r l r} \min _ {x, z, \gamma} & \gamma + \frac {1}{(1 - \alpha) S} \sum_ {s = 1} ^ {S} z _ {s} \\ \mathrm{subjectto} & z _ {s} \geq \sum_ {i} (b _ {i} - y _ {i s}) x _ {i} - \gamma & \mathrm{for} s = 1, \ldots , S \\ & z _ {s} \geq 0 & \mathrm{for} s = 1, \ldots , S \\ & l _ {i} \leq x _ {i} \leq u _ {i} & i = 1, \ldots , n \\ & \sum_ {i} x _ {i} = 1 \\ & \sum_ {i} \mu_ {i} x _ {i} \geq R \end{array}
$$

Consider $\alpha = 9 9 \%$ . The original bond portfolio had an expected portfolio return of 7.26%. The expected loss was 95 million dollars with a standard deviation of 232 million. The VaR was 1.03 billion dollars and the CVaR was 1.32 billion. 

After optimizing the portfolio (with expected return of 7.26%), the expected loss was only 5 thousand dollars, with a standard deviation of 152 million. The VaR was reduced to 210 million and the CVaR to 263 million dollars. So all around, the characteristics of the portfolio were much improved. Positions were reduced in bonds from Brazil, Russia and Venezuela, whereas positions were increased in bonds from Thailand, Malaysia and Chile. Positions in bonds from Colombia, Poland and Mexico remained high and each accounted for about 5 % of the optimized CVaR. 

Chapter 18 

# Stochastic Programming Models: Asset/Liability Management

## 18.1 Asset/Liability Management

Financial health of any company, and in particular those of financial institutions, is reflected in the balance sheets of the company. Proper management of the company requires attention to both sides of the balance sheet–assets and liabilities. Asset/Liability Management (ALM) ofers sophisticated mathematical tools for an integrated management of assets and liabilities and is the focus of many studies in financial mathematics. 

ALM recognizes that static, one period investment planning models (such as mean-variance optimization) fail to incorporate the multi-period nature of the liabilities faced by the company. A multi-period model that emphasizes the need to meet liabilities in each period for a finite (or possibly infinite) horizon is often required. Since liabilities and asset returns usually have random components, their optimal management requires tools of “Optimization under Uncertainty” and most notably, stochastic programming approaches. 

We recall the ALM setting we introduced in Section 1.3.4: Let $L _ { t }$ be the liability of the company in year t for $t = 1 , \dots , T$ . The $L _ { t } { ' } \mathrm { s }$ are random variables. Given these liabilities, which assets (and in which quantities) should the company hold each year to maximize its expected wealth in year T? The assets may be domestic stocks, foreign stocks, real estate, bonds, etc. Let $R _ { i t }$ denote the return on asset i in year t. The $R _ { i t } '$ s are random variables. The decision variables are: 

$$
x _ {i t} = \mathrm{marketvalueinvestedinasset} i \mathrm{inyear} t.
$$

The decisions $x _ { i t }$ in year t are made after the random variables $L _ { t }$ and $R _ { i t }$ are realized. That is, the decision problem is multistage, stochastic, with recourse. The stochastic program can be written as follows. 

$$
\begin{array}{r l} \max & E [ \sum_ {i} x _ {i T} ] \\ \text {subject to} \\ \text {asset accumulation:} & \sum_ {i} (1 + R _ {i t}) x _ {i, t - 1} - \sum_ {i} x _ {i t} = L _ {t} \text {for} t = 1, \ldots , T \\ & x _ {i t} \geq 0. \end{array}
$$

The constraint says that the surplus left after liability $L _ { t }$ is covered will be invested as follows: $x _ { i t }$ invested in asset i. In this formulation, $x _ { 0 , t }$ are the fixed, and possibly nonzero initial positions in diferent asset classes. The objective selected in the model above is to maximize the expected wealth at the end of the planning horizon. In practice, one might have a diferent objective. For example, in some cases, minimizing Value at Risk (VaR) might be more appropriate. Other priorities may dictate other objective functions. 

To address the issue of the most appropriate objective function, one must understand the role of liabilities. Pension funds and insurance companies are among the most typical arenas for the integrated management of assets and liabilities through ALM. We consider the case of a Japanese insurance company, the Yasuda Fire and Marine Insurance Co, Ltd, following the work of Carino,˜ Kent, Myers, Stacy, Sylvanus, Turner, Watanabe, and Ziemba [17]. In this case, the liabilities are mainly savings-oriented policies issued by the company. Each new policy sold represents a deposit, or inflow of funds. Interest is periodically credited to the policy until maturity, typically three to five years, at which time the principal amount plus credited interest is refunded to the policyholder. The crediting rate is typically adjusted each year in relation to a market index like the prime rate. Therefore, we cannot say with certainty what future liabilities will be. Insurance business regulations stipulate that interest credited to some policies be earned from investment income, not capital gains. ${ \mathrm { S o } } ,$ in addition to ensuring that the maturity cash flows are met, the firm must seek to avoid interim shortfalls in income earned versus interest credited. In fact, it is the risk of not earning adequate income quarter by quarter that the decision makers view as the primary component of risk at Yasuda. 

The problem is to determine the optimal allocation of the deposited funds into several asset categories: cash, fixed rate and floating rate loans, bonds, equities, real estate and other assets. Since we can revise the portfolio allocations over time, the decision we make is not just among allocations today but among allocation strategies over time. A realistic dynamic asset/liability model must also account for the payment of taxes. This is made possible by distinguishing between interest income and price return. 

A stochastic linear program is used to model the problem. The linear program has uncertainty in many coeficients. This uncertainty is modeled through a finite number of scenarios. In this fashion, the problem is transformed into a very large scale linear program of the form (16.6). The random elements include price return and interest income for each asset class, as well as policy crediting rates. 

We now present a multistage stochastic program that was developed for The Yasuda Fire and Marine Insurance $\mathrm { C o . }$ , Ltd. Our presentation follows the description of the model as stated in [17]. 

## 18.1. ASSET/LIABILITY MANAGEMENT

Stages are indexed by $t = 0 , 1 , \ldots , T .$ 

Decision variables of the stochastic program: 

$$
x _ {i t}
$$

$$
{w _ {t}} = {\mathrm{interestincomeshortfallat} t \geq 1,}
$$

$$
t \geq 1
$$

Random variables appearing in the stochastic linear program: For $t \geq 1$ 2 

$RP_{it}$ = price return of asset i from t-1 to t, $RI_{it}$ = interest income of asset i from t-1 to t, $F_{t}$ = deposit inflow from t-1 to t, $P_{t}$ = principal payout from t-1 to t, $I_{t}$ = interest payout from t-1 to t, $g_{t}$ = rate at which interest is credited to policies from t-1 to t, $L_{t}$ = liability valuation at t. 

Parameterized function appearing in the objective: 

$$
{c _ {t}} = {\mathrm{piecewiselinearconvexcostfunction}.}
$$

The objective of the model is to allocate funds among available assets to maximize expected wealth at the end of the planning horizon $T$ less expected penalized shortfalls accumulated through the planning horizon. 

$$
\begin{array}{r l} \max & E [ \sum_ {i} x _ {i T} - \sum_ {t = 1} ^ {T} c _ {t} (w _ {t}) ] \\ \text {subject to} \\ \text {asset accumulation:} & \sum_ {i} x _ {i t} - \sum_ {i} (1 + R P _ {i t} + R I _ {i t}) x _ {i, t - 1} = F _ {t} - P _ {t} - I _ {t} \quad \text {for} t = 1, \ldots , T \\ \text {interest income shortfall:} & \sum_ {i} R I _ {i t} x _ {i, t - 1} + w _ {t} - v _ {t} = g _ {t} L _ {t - 1} \quad \text {for} t = 1, \ldots , T \\ & x _ {i t} \geq 0, w _ {t} \geq 0, v _ {t} \geq 0. \end{array}\tag{18.1}
$$

Liability balances and cash flows are computed so as to satisfy the liability accumulation relations. 

$$
L _ {t} = (1 + g _ {t}) L _ {t - 1} + F _ {t} - P _ {t} - I _ {t} \text {for} t \geq 1.
$$

The stochastic linear program (18.1) is converted into a large linear program using a finite number of scenarios to deal with the random elements in the data. Creation of scenario inputs is made in stages using a tree. The tree structure can be described by the number of branches at each stage. For example, a 1-8-4-4-2-1 tree has 256 scenarios. Stage $t = 0$ is the initial stage. Stage t = 1 may be chosen to be the end of Quarter 1 and has 8 diferent scenarios in this example. Stage $t = 2$ may be chosen to be the end of Year 1, with each of the previous scenarios giving rise to 4 new scenarios, and so on. For the Yasuda Fire and Marine Insurance Co., Ltd., a problem with 7 asset classes and 6 stages gives rise to a stochastic linear program (18.1) with 12 constraints (other than nonnegativity) and 54 variables. Using 256 scenarios, this stochastic program is converted into a linear program with several thousand constraints and over 10,000 variables. Solving this model yielded extra income estimated to about US$ 80 million per year for the company. 

Exercise 18.1 Discuss the relevance of the techniques from Chapter 16 in the solution of the Yasuda Fire and Marine Insurance Co., such as scenario generation (correlation of the random parameters over time, variance reduction techniques in constructing the scenario tree), decomposition techniques to solve the large-scale linear programs. 

## 18.1.1 Corporate Debt Management

A closely related problem to the asset/liability management (ALM) problem in corporate financial planning is the problem of debt management. Here the focus is on retiring (paying back) outstanding debt at minimum cost. More specifically, corporate debt managers must make financial decisions to minimize the costs and risks of borrowing to meet debt financing requirements. These requirements are often determined by the firm’s investment decisions. Our discussion in this subsection is based on the article [24]. 

Debt managers need to choose the sources of borrowing, types of debts to be used, timing and terms of debts, whether the debts will be callable<sup>1</sup>, etc., in a multi-period framework where the dificulty of the problem is compounded by the fact that the interest rates that determine the cost of debt are uncertain. Since interest rate movements can be modeled by random variables this problem presents an attractive setting for the use of stochastic programming techniques. Below, we discuss a deterministic linear programming equivalent of stochastic LP model for the debt management problem. 

We consider a multi-period framework with T time periods. We will use the indices s and t ranging between 0 (now) and T (termination date, or horizon) to denote diferent time periods in the model. We consider K types of debt that are distinguished by market of issue, term and the presence (or absence) of call option available to the borrower. In our notation, the superscript k ranging between 1 and K will denote the diferent types of debt being considered. 

The evolution of the interest rates are described using a scenario tree. We denote by $e _ { j } = e _ { j 1 } , e _ { j 2 } , \ldots , e _ { j T } , j = 1 , \ldots , J$ a sample path of this scenario tree which corresponds to a sequence of interest rate events. When a parameter or variable is contingent on the event sequence $e _ { j }$ we use the notation $( e _ { j } )$ (see below). 

The decision variables in this model are the following: 

$B _ { t } ^ { k } ( e _ { j } )$ : dollar amount at $\mathrm { p a r ^ { 2 } }$ of debt type k Borrowed at the beginning of period t. 

$O _ { s , t } ^ { k } ( e _ { j } )$ : dollar amount at par of debt type k borrowed in period s and Outstanding at the beginning of period t. 

$R _ { s , t } ^ { k } ( e _ { j } )$ : dollar amount at par of debt type k borrowed in period s and Retired (paid back) at the beginning of period t. 

$S _ { t } ( e _ { j } )$ : dollar value of Surplus cash held at the beginning of period t. 

Next, we list the input parameters to the problem: 

$r _ { s , t } ^ { k } ( e _ { j } )$ : interest payment in period t per dollar outstanding of debt type k issued in period s. 

● $f _ { t } ^ { k }$ : issue costs (excluding premium or discount) per dollar borrowed of debt type k issued in period t. 

$g _ { s , t } ^ { k } ( e _ { j } )$ : retirement premium or discount per dollar for debt type k issued in period $s ,$ if retired in period $t ^ { 3 }$ 

$i _ { t } ( e _ { j } )$ : interest earned per dollar on surplus cash in period t. 

$p ( e _ { j } ) { : }$ : probability of the event sequence $e _ { j }$ . Note that $p ( e _ { j } ) \ge 0$ , j and $\textstyle \sum _ { j = 1 } ^ { J } p ( e _ { j } ) = 1$ 

$C _ { t } \mathrm { : }$ cash requirements for period t, which can be negative to indicate an operating surplus. 

$M _ { t } \mathbf { . }$ maximum allowable cost of debt service in period t. 

$q _ { t } ^ { k } ( Q _ { t } ^ { k } )$ : minimum (maximum) borrowing of debt type k in period t. 

$L _ { t } ( e _ { j } ) ( U _ { t } ( e _ { j } ) )$ : minimum (maximum) dollar amount of debt (at par) retired in period t. 

The objective function of this problem is expressed as follows: 

$$
\min \sum_ {j = 1} ^ {J} p (e _ {j}) \left(\sum_ {k = 1} ^ {K} \sum_ {t = 1} ^ {T} \left(1 + g _ {t, T} ^ {k} (e _ {j})\right) \left[ O _ {t, T} ^ {k} (e _ {j}) - R _ {t, T} ^ {k} (e _ {j}) \right] + (1 - f _ {T} ^ {k}) B _ {T} ^ {k} (e _ {j})\right)\tag{18.2}
$$

This function expresses the expected retirement cost of the total debt outstanding at the end of period $T .$ 

We complete the description of the deterministic equivalent of the stochastic LP by listing the constraints of the problem: 

Cash Requirements: For each time period $t = 1 , \dots , T$ and scenario path $j = 1 , \dots , J ;$ 

$$
\begin{array}{r l r} & & {C _ {t} + S _ {t} (e _ {j}) = \sum_ {k = 1} ^ {K} \left\{\left(1 - f _ {t} ^ {k}\right) B _ {t} ^ {k} (e _ {j}) + (1 + i _ {t - 1} (e _ {j})) S _ {t - 1} (e _ {j}) \right.} \\ & & {\left. - \sum_ {s = 0} ^ {t - 1} \left[ r _ {s, t} ^ {k} (e _ {j}) O _ {s, t} ^ {k} (e _ {j}) - \left(1 + g _ {s, t} ^ {k} (e _ {j})\right) R _ {s, t} ^ {k} (e _ {j}) \right] \right\}.} \end{array}
$$

This balance equation indicates that the diference between cash available (new net borrowing, surplus cash from previous period and the interest earned on this cash) and the debt payments (interest on outstanding debt and cash outflows on repayment) should equal the cash requirements plus the surplus cash left for this period. 

Debt Balance Constraints: For $j = 1 , \dots , J , t = 1 , \dots , T , s =$ $0 , \ldots , t - 2$ , and $k = 1 , \dots K$ 

$$
\begin{array}{r c l} {O _ {s, t} ^ {k} (e _ {j}) - O _ {s, t - 1} ^ {k} (e _ {j}) + R _ {s, t - 1} ^ {k} (e _ {j})} & = & 0 \\ {O _ {t - 1, t} ^ {k} (e _ {j}) - B _ {t - 1} ^ {k} (e _ {j}) - R _ {t - 1, t} ^ {k} (e _ {j})} & = & 0 \end{array}
$$

Maximum cost of debt: For $j = 1 , \ldots , J , t = 1 , \ldots , T$ , and $k =$ $1 , \ldots . K$ : 

$$
\sum_ {s = 1} ^ {t - 1} \left(r _ {s, t} ^ {k} (e _ {j}) O _ {s, t} ^ {k} (e _ {j}) - i _ {t - 1} (e _ {j}) S _ {t - 1} (e _ {j})\right) \leq M _ {t}.
$$

Borrowing limits: For $j = 1 , \ldots , J , t = 1 , \ldots , T$ , and $k = 1 , \dots K$ 

$$
q _ {t} ^ {k} \leq B _ {t} ^ {k} (e _ {j}) \leq Q _ {t} ^ {k}.
$$

Payof limits: For $j = 1 , \dots , J$ and $t = 1 , \dots , T$ 

$$
L _ {t} (e _ {j}) \leq \sum_ {k = 1} ^ {K} \sum_ {s = 0} ^ {t - 1} R _ {s, t} ^ {k} (e _ {j}) \leq U _ {t} (e _ {j}).
$$

Nonnegativity: For $j = 1 , \dots , J , t = 1 , \dots , T , s = 0 , \dots , t - 2 ,$ , and $k = 1 , \dots K$ 

$$
B _ {t} ^ {k} (e _ {j}) \geq 0, O _ {s, t} ^ {k} (e _ {j}) \geq 0, R _ {s, t} ^ {k} (e _ {j}) \geq 0, S _ {t} (e _ {j}) \geq 0.
$$

In the formulation above, we used the notation of the article [24]. However, since the parameters and variables dependent on $e _ { j }$ can only depend on the portion of the sequence that is revealed by a certain time, a more precise notation can be obtained using the following ideas. First, let $e _ { j } ^ { t } = e _ { j 1 } , e _ { j 2 } , \ldots , e _ { j t } , j = 1 , \ldots , J , t = 1 , \ldots , T , \mathrm { i . e . , } e _ { j } ^ { t }$ represents the portion of $e _ { j }$ observed by time period t. Then, one replaces the expressions such as $S _ { t } ( e _ { j } )$ with $S _ { t } ( e _ { j } ^ { t } )$ , etc. 

## 18.2 Synthetic Options

An important issue in portfolio selection is the potential decline of the portfolio value below some critical limit. How can we control the risk of downside losses? A possible answer is to create a payof structure similar to a European call option. 

While one may be able to construct a diversified portfolio well suited for a corporate investor, there may be no option market available on this portfolio. One solution may be to use index options. However exchangetraded options with suficient liquidity are limited to maturities of about three months. This makes the cost of long-term protection expensive, requiring the purchase of a series of high priced short-term options. For large institutional or corporate investors, a cheaper solution is to artificially produce the desired payof structure using available resources. This is called a “synthetic option strategy”. 

The model is based on the following data. 

$W _ { 0 }$ = investor’s initial wealth, 

$T$ = planning horizon, 

$R$ = riskless return for one period, 

$R _ { t } ^ { i }$ = return for asset i at time t, 

$\theta _ { t } ^ { i }$ = transaction cost for purchases and sales of asset i at time t. 

The $R _ { t } ^ { i }$ ’s are random, but we know their distributions. 

The variables used in the model are the following. 

$\ v x _ { t } ^ { i }$ = amount allocated to asset i at time $t ,$ 

$A _ { t } ^ { i }$ = amount of asset i bought at time $t ,$ 

$D _ { t } ^ { i }$ = amount of asset i sold at time t, 

$\alpha _ { t }$ = amount allocated to riskless asset at time t. 

We formulate a stochastic program that produces the desired payof at the end of the planning horizon $T .$ , much in the flavor of the stochastic programs developed in the previous two sections. Let us first discuss the constraints. 

The initial portfolio is 

$$
\alpha_ {0} + x _ {0} ^ {1} + \ldots + x _ {0} ^ {n} = W _ {0}.
$$

The portfolio at time t is 

$$
x _ {t} ^ {i} = R _ {t} ^ {i} x _ {t - 1} ^ {i} + A _ {t} ^ {i} - D _ {t} ^ {i} \quad \mathrm{for} t = 1, \ldots , T
$$

$$
\alpha_ {t} = R \alpha_ {t - 1} - \sum_ {i = 1} ^ {n} (1 + \theta_ {t} ^ {i}) A _ {t} ^ {i} + \sum_ {i = 1} ^ {n} (1 - \theta_ {t} ^ {i}) D _ {t} ^ {i} \quad \text { for } t = 1, \ldots , T.
$$

One can also impose upper bounds on the proportion of any risky asset in the portfolio: 

$$
0 \leq x _ {t} ^ {i} \leq m _ {t} (\alpha_ {t} + \sum_ {j = 1} ^ {n} x _ {t} ^ {j}),
$$

where $m _ { t }$ is chosen by the investor. 

The value of the portfolio at the end of the planning horizon is: 

$$
v = R \alpha_ {T - 1} + \sum_ {i = 1} ^ {n} (1 - \theta_ {T} ^ {i}) R _ {T} ^ {i} x _ {T - 1} ^ {i},
$$

where the summation term is the value of the risky assets at time $T .$ 

To construct the desired synthetic option, we split v into the riskless value of the portfolio Z and a surplus $z \geq 0$ which depends on random events. Using a scenario approach to the stochastic program, Z is the worstcase payof over all the scenarios. The surplus z is a random variable that depends on the scenario. Thus 

$$
v = Z + z
$$

$$
z \geq 0.
$$

We consider $Z$ and z as variables of the problem, and we optimize them together with the asset allocations x and other variables described earlier. The objective function of the stochastic program is 

$$
\max E (z) + \mu Z
$$

where $\mu \geq 1$ is the risk aversion of the investor. The risk aversion $\mu$ is given data. 

When $\mu = 1$ , the objective is to maximize expected return. 

When $\mu$ is very large, the objective is to maximize “riskless profit” as we defined it in Chapter 4 (Exercise 4.10). 

As an example, consider an investor with initial wealth $W _ { 0 } = 1$ who wants to construct a portfolio comprising one risky asset and one riskless asset using the “synthetic option” model described above. We write the model for a two-period planning horizon, i.e. $T = 2$ . The return on the riskless asset is $R$ per period. For the risky asset, the return is $R _ { 1 } ^ { + }$ with probability .5 and $R _ { 1 } ^ { - }$ with the same probability at time $t = 1$ . Similarly, the return of the risky asset is $R _ { 2 } ^ { + }$ with probability .5 and $R _ { 2 } ^ { - }$ with the same probability at time $t = 2$ . The transaction cost for purchases and sales of the risky asset is θ. 

There are 4 scenarios in this example, each occurring with probability .25, which we can represent by a binary tree. The initial node will be denoted by 0, the up node from it by 1 and the down node by 2. Similarly the up node from node 1 will be denoted by 3, the down node by 4, and the successors of 2 by 5 and 6 respectively. Let $x _ { i } , \alpha _ { i }$ denote the amount of risky asset and of riskless asset respectively in the portfolio at node i of this binary tree. $Z$ is the riskless value of the portfolio and $z _ { i }$ is the surplus at node i. The linear program is: 

$$
\begin{array}{r l} \max & . 2 5 z _ {3} +. 2 5 z _ {4} +. 2 5 z _ {5} +. 2 5 z _ {6} + \mu Z \\ \text {subject to} \\ \text {initial portfolio:} & \alpha_ {0} + x _ {0} = 1 \\ \text {rebalancing constraints:} & x _ {1} = R _ {1} ^ {+} x _ {0} + A _ {1} - D _ {1} \\ & \alpha_ {1} = R \alpha_ {0} - (1 + \theta) A _ {1} + (1 - \theta) D _ {1} \\ & x _ {2} = R _ {1} ^ {-} x _ {0} + A _ {2} - D _ {2} \\ & \alpha_ {2} = R \alpha_ {0} - (1 + \theta) A _ {2} + (1 - \theta) D _ {2} \\ \text {payoff:} & z _ {3} + Z = R \alpha_ {1} + (1 - \theta) R _ {2} ^ {+} x _ {1} \\ & z _ {4} + Z = R \alpha_ {1} + (1 - \theta) R _ {2} ^ {-} x _ {1} \\ & z _ {5} + Z = R \alpha_ {2} + (1 - \theta) R _ {2} ^ {+} x _ {2} \\ & z _ {6} + Z = R \alpha_ {2} + (1 - \theta) R _ {2} ^ {-} x _ {2} \\ \text {nonnegativity:} & \alpha_ {i}, x _ {i}, z _ {i}, A _ {i}, D _ {i} \geq 0. \end{array}
$$

Example: An interesting paper discussing synthetic options is the paper of Y. Zhao and W.T. Ziemba [75]. Zhao and Ziemba apply the synthetic option model to an example with 3 assets (cash, bonds and stocks) and 4 periods (a one-year horizon with quarterly portfolio reviews). The quarterly return on cash is constant at $\rho = 0 . 0 0 9 5$ . For stocks and bonds, the expected logarithmic rates of returns are $s = 0 . 0 4$ and $b = 0 . 0 1 9$ respectively. Transaction costs are 0.5% for stocks and 0.1% for bonds. The scenarios needed in the stochastic program are generated using an auto regression model which is constructed based on historical data (quarterly returns from 1985 to 1998; the Salomon Brothers bond index and S&P 500 index respectively). Specifically, the auto regression model is 

$$
\left\{ \begin{array}{l} s _ {t} = 0. 0 3 7 - 0. 1 9 3 s _ {t - 1} + 0. 4 1 8 b _ {t - 1} - 0. 1 7 2 s _ {t - 2} + 0. 5 1 7 b _ {t - 2} + \epsilon_ {t} \\ b _ {t} = 0. 0 0 7 - 0. 1 4 0 s _ {t - 1} + 0. 1 7 5 b _ {t - 1} - 0. 0 2 3 s _ {t - 2} + 0. 1 2 2 b _ {t - 2} + \eta_ {t} \end{array} \right.
$$

where the pair $( \epsilon _ { t } , \eta _ { t } )$ characterizes uncertainty. The scenarios are generated by selecting 20 pairs of $( \epsilon _ { t } , \eta _ { t } )$ to estimate the empirical distribution of one period uncertainty. In this way, a scenario tree with $1 6 0 , 0 0 0 ~ ( = 2 0 \times 2 0 \times$ $2 0 \times 2 0 )$ paths describing possible outcomes of asset returns is generated for the 4 periods. 

The resulting large scale linear program is solved. We discuss the results obtained when this linear program is solved for a risk aversion of $\mu = 2 . 5 \mathrm { : }$ The value of the terminal portfolio is always at least 4.6% more than the initial portfolio wealth and the distribution of terminal portfolio values is skewed to larger values because of dynamic downside risk control. The expected return is 16.33% and the volatility is 7.2%. It is interesting to compare these values with those obtained from a static Markowitz model: The expected return is 15.4% for the same volatility but no minimum return is guaranteed! In fact, in some scenarios, the value of the Markowitz portfolio is 5% less at the end of the one-year horizon than it was at the beginning. 

It is also interesting to look at an example of a typical portfolio (one of the 160,000 paths) generated by the synthetic option model (the linear program was set up with an upper bound of 70 % placed on the fraction of stocks or bonds in the portfolio): 

<table><tr><td></td><td>Cash</td><td>Stocks</td><td>Bonds</td><td>Portfolio value at end of period</td></tr><tr><td>Period 1</td><td>12%</td><td>18%</td><td>70%</td><td>100</td></tr><tr><td>2</td><td></td><td>41%</td><td>59%</td><td>103</td></tr><tr><td>3</td><td></td><td>70%</td><td>30%</td><td>107</td></tr><tr><td>4</td><td>30%</td><td></td><td>70%</td><td>112</td></tr><tr><td></td><td></td><td></td><td></td><td>114</td></tr></table>

Exercise 18.2 Computational exercise: Develop a synthetic option model in the spirit of that used by Zhao and Ziemba, adapted to the size limitation of your linear programming solver. Compare with a static model. 

## 18.3 Case Study: Option Pricing with Transaction Costs

A European call option on a stock with maturity T and strike price X gives the right to buy the stock at price X at time T. The holder of the option will not exercise this option if the stock has a price S lower than X at time T. Therefore the value of a European call option is max $( S - X , 0 )$ . Since S is random, the question of pricing the option correctly is of interest. The Black Scholes Merton Option Pricing model relates the price of an option to the volatility of the stock return. The assumptions are that the market is eficient and that the returns are lognormal. ¿From the volatility σ of the stock return, one can compute the option price for any strike price X. Conversely, from option prices one can compute the implied volatility σ. For a given stock, options with diferent strike prices should lead to the same σ (if the assumptions of the Black Scholes Merton model are correct). 

The aim of the model developed in this section is to examine the extent to which market imperfections can explain the deviation of observed option prices from the Black Scholes Merton Option Pricing model. One way to measure the deviation of the Black Scholes Merton model from observed option prices is through the “volatility smile”: for a given maturity date, the implied volatility of a stock computed by the Black Scholes Merton model from observed option prices at diferent strike prices is typically not constant, but instead often exhibits a convex shape as the strike price increases (the “smile”). One explanation for the deviation is that the smile occurs because the Black Scholes Merton model assumes the ability to rebalance portfolios without costs imposed either by the inability to borrow or due to a bid-ask spread or other trading costs. Here we will look at the efect of transaction costs on option prices. 

The derivation of the Black Scholes Merton formula is through a replicating portfolio containing the stock and a riskless bond. If the market is eficient, we should be able to replicate the option payof at time T by rebalancing the portfolio between now and time T, as the stock price evolves. Rather than work with a continuous time model, we discretize this process. 

## 18.3. CASE STUDY: OPTION PRICING WITH TRANSACTION COSTS289

This discretization is called the binomial approximation to the Black Scholes Merton Option Pricing model. In this model, we specify a time period $\Delta$ between trading opportunities and postulate the behavior of stock and bond prices along successive time periods. The binomial model assumes that in between trading periods, only two possible stock price movements are possible. 

a) There are N stages in the tree, indexed $0 , 1 \ldots , N$ , where stage 0 is the root of the tree and stage N is the last stage. If we divide the maturity date $T$ of an option by N, we get that the length of a stage is $\Delta = T / N$ 

b) Label the initial node $k _ { 0 }$ 

c) For a node $\boldsymbol { k } \neq \boldsymbol { k } _ { 0 }$ , let $k ^ { - }$ − be the node that is the immediate predecessor of $k .$ . 

d) Let $S ( k )$ be the stock price at node k and let $B ( k )$ be the bond price at node k. 

e) We assume that the interest rate is fixed at the annualized rate r so that $B ( k ) = B ( k ^ { - } ) e ^ { r \Delta }$ 

f) Letting σ denote the volatility of the stock return, we use the standard parametrization $u = e ^ { \sigma { \sqrt { \Delta } } }$ and $d = 1 / u . \mathrm { \ S o \ } S ( k ) = S ( k ^ { - } ) e ^ { \sigma \sqrt { \Delta } }$ if an uptick occurs from k− to k and $S ( k ) = S ( k ^ { - } ) e ^ { - \sigma \sqrt { \Delta } }$ if a downtick occurs. 

g) Let $n ( k )$ be the quantity of stocks at node k and let $m ( k )$ be the quantity of bonds at k. 

## 18.3.1 The Standard Problem

In the binomial model, we have dynamically complete markets. This means that by trading the stock and the bond dynamically, we can replicate the payofs (and values) from a call option. The option value is simply the cost of the replicating portfolio, and the replicating portfolio is self-financing after the first stage. This means that after we initially buy the stock and the bond, all subsequent trades do not require any additional money and, at the last stage, we reproduce the payofs from the call option. 

Therefore, we can represent the option pricing problem as the following linear program. Choose quantities $n ( k )$ of the stock, quantities $m ( k )$ of the bond at each nonterminal node k to 

$$
\min \quad n (k _ {0}) S (k _ {0}) + m (k _ {0}) B (k _ {0}) \tag {5}
$$

subject to 

$$
\text { rebalancing   constraints: } \quad n (k ^ {-}) S (k) + m (k ^ {-}) B (k) \geq n (k) S (k) + m (k) B (k)
$$

$$
\text { for   every   node } k \neq k _ {0}
$$

replication constraints: 

$$
n (k ^ {-}) S (k) + m (k ^ {-}) B (k) \geq \max (S (k) - X, 0)
$$

for every terminal node k 

where $k ^ { - }$ denotes the predecessor of k. 

Note that we do not impose nonnegativity constraints since we will typically have a short position in the stock or bond. 

Exercise 18.3 For a nondividend paying stock, collect data on 4 or 5 call options for the nearest maturity (but at least one month). Calculate the implied volatility for each option. Solve the standard problem (5) when the number of stages is 7 using the implied volatility of the at-the-money option to construct the tree. 

## 18.3.2 Transaction Costs

To model transaction costs, we consider the simplest case where there are no costs of trading at the initial and terminal nodes, but there is a bid-ask spread on stocks at other nodes. So assume that if you buy a stock at node k, you pay $S ( k ) ( 1 + \theta )$ while if you sell a stock, you receive $S ( k ) ( 1 - \theta )$ . This means that the rebalancing constraint becomes 

$$
n (k ^ {-}) S (k) + m (k ^ {-}) B (k) \geq n (k) S (k) + m (k) B (k) + | n (k) - n (k ^ {-}) | \theta S (k).
$$

There is an absolute value in this constraint. So it is not a linear constraint. However it can be linearized as follows. Define two nonnegative variables: 

$x(k) =$ number of stocks bought at node $k$ , and $y(k) =$ number of stocks sold at node $k$ . 

The rebalancing constraint now becomes: 

$$
\begin{array}{l} n (k ^ {-}) S (k) + m (k ^ {-}) B (k) \geq n (k) S (k) + m (k) B (k) + (x (k) + y (k)) \theta S (k) \\ n (k) - n (k ^ {-}) = x (k) - y (k) \\ x (k) \geq 0, \quad y (k) \geq 0. \end{array}
$$

Note that this constraint leaves the possibility of simultaneously buying and selling stocks at the same node. But obviously this cannot improve the objective function that we minimize in (5), so we do not need to impose a constraint to prevent it. 

The modified formulation is: 

$$
\begin{array}{r l} {(6) \quad \min} & {n (k _ {0}) S (k _ {0}) + m (k _ {0}) B (k _ {0})} \\ {\mathrm{subjectto}} \\ {\mathrm{rebalancingconstraints:}} & {n (k ^ {-}) S (k) + m (k ^ {-}) B (k) \geq n (k) S (k) + m (k) B (k)} \\ & {+ (x (k) + y (k)) \theta S (k) \quad \mathrm{foreverynode} k \neq k _ {0}} \\ & {n (k) - n (k ^ {-}) = x (k) - y (k) \quad \mathrm{foreverynode} k \neq k _ {0}} \\ {\mathrm{replicationconstraints:}} & {n (k ^ {-}) S (k) + m (k ^ {-}) B (k) \geq \max (S (k) - X, 0)} \\ & {\mathrm{foreveryterminalnode} k} \\ {\mathrm{nonnegativity:}} & {x (k) \geq 0, \quad y (k) \geq 0 \quad \mathrm{foreverynode} k \neq k _ {0}.} \end{array}
$$

## 18.3. CASE STUDY: OPTION PRICING WITH TRANSACTION COSTS291

Exercise 18.4 Repeat the exercise in Section 18.3.1 allowing for transaction costs, with diferent values of θ, to see if the volatility smile can be explained by transaction costs. Specifically, given a value for σ and for θ, calculate option prices and see how they match up to observed prices. Try θ = 0.001, 0.005, 0.01, 0.02, 0.05. 

292 CHAPTER 18. SP MODELS: ASSET/LIABILITY MANAGEMENT 

# Chapter 19

# Robust Optimization: Theory and Tools

## 19.1 Introduction to Robust Optimization

In many optimization models the inputs to the problem are either not known at the time the problem must be solved, are computed inaccurately, or otherwise uncertain. Since the solutions obtained can be quite sensitive to these inputs, one serious concern is that we are solving the wrong problem, and that the solution we find is far from optimal for the correct problem. 

Robust optimization refers to the modeling of optimization problems with data uncertainty to obtain a solution that is guaranteed to be “good” for all or most possible realizations of the uncertain parameters. Uncertainty in the parameters is described through uncertainty sets that contain many possible values that may be realized for the uncertain parameters. The size of the uncertainty set is determined by the level of desired robustness. 

Robust optimization can be seen as a complementary alternative to sensitivity analysis and stochastic programming. Robust optimization models can be especially useful in the following situations: 

Some of the problem parameters are estimates and carry estimation risk. 

There are constraints with uncertain parameters that must be satisfied regardless of the values of these parameters. 

The objective function or the optimal solutions are particularly sensitive to perturbations. 

The decision-maker cannot aford to low-probability but high-magnitude risks. 

Recall from Chapter 1 that there are diferent definitions and interpretations of robustness; the resulting models and formulations difer accordingly. In particular, we can distinguish between constraint robustness and objective robustness. In the first case, data uncertainty puts the feasibility of potential solutions at risk. In the second, feasibility constraints are fixed and the uncertainty of the objective function afects the proximity of the generated solutions to optimality. 

Both the constraint and objective robustness models we considered in the introduction have a worst-case orientation. That is, we try to optimize the behavior of the solutions under the most adverse conditions. Following Kouvelis and Yu [44], we call solutions that optimize the worst-case behavior under uncertainty absolute robust solutions. While such conservatism is necessary in some optimization settings, it may not be desirable in others. Absolute robustness is not always consistent with a decision theoretic approach and with common utility functions. An alternative is to seek robustness in a relative sense. 

In uncertain decision environments, people whose performance is judged relative to their peers will want to make decisions that avoid falling severely behind their competitors under all scenarios rather than protecting themselves against the worst-case scenarios. For example, a portfolio manager will be considered successful in a down market as long as she loses less than her peers or a benchmark. These considerations motivate the concept of relative robustness which we discuss in Section 19.3.3. 

Another variant of the robust optimization models called adjustable robust optimization are attractive in multi-period models. To motivate these models one can consider a multi-period uncertain optimization problem where uncertainty is resolved progressively through periods. We assume that a subset of the decision variables can be chosen after these parameters are observed in a way to correct the sub-optimality of the decisions made with less information in earlier stages. In spirit, these models are closely related to two (or multi-) stage stochastic programming problems with recourse. They were introduced by Guslitzer and co-authors [35, 5] and we summarize this approach in Section 19.3.4. 

Each diferent interpretation of robustness and each diferent description of uncertainty leads to a diferent robust optimization formulation. These robust optimization problems often are or at least appear to be more dificult than their non-robust counterparts. Fortunately, many of them can be reformulated in a tractable manner. While it is dificult to expect a single approach to handle each one of the diferent variations in a unified manner, a close study of the existing robust optimization formulations reveals many common threads. In particular, methods of conic optimization appear frequently in the solution of robust optimization problems. We review some of the most commonly used reformulation techniques used in robust optimization at the end of the chapter. 

## 19.2 Uncertainty Sets

In robust optimization, the description of the uncertainty of the parameters is formalized via uncertainty sets. Uncertainty sets can represent or may be formed by diference of opinions on future values of certain parameters, alternative estimates of parameters generated via statistical techniques from historical data and/or Bayesian techniques, among other things. 

Common types of uncertainty sets encountered in robust optimization models include the following: 

Uncertainty sets representing a finite number of scenarios generated for the possible values of the parameters: 

$$
\mathcal {U} = \{p _ {1}, p _ {2}, \dots , p _ {k} \}.
$$

Uncertainty sets representing the convex hull of a finite number of scenarios generated for the possible values of the parameters (these are sometimes called polytopic uncertainty sets): 

$$
\mathcal {U} = \operatorname{conv} (p _ {1}, p _ {2}, \dots , p _ {k}).
$$

Uncertainty sets representing an interval description for each uncertain parameter: 

$$
\mathcal {U} = \{p: l \leq p \leq u \}.
$$

Confidence intervals encountered frequently in statistics can be the source of such uncertainty sets. 

Ellipsoidal uncertainty sets: 

$$
\mathcal {U} = \{p: p = p _ {0} + M u, \| u \| \leq 1 \}
$$

These uncertainty sets can also arise from statistical estimation in the form of confidence regions, see [29]. In addition to their mathematically compact description, ellipsoidal uncertainty sets have the nice property that they smoothen the optimal value function [65]. 

It is a non-trivial task to determine the uncertainty set that is appropriate for a particular model as well as the type of uncertainty sets that lead to tractable problems. As a general guideline, the shape of the uncertainty set will often depend on the sources of uncertainty as well as the sensitivity of the solutions to these uncertainties. The size of the uncertainty set, on the other hand, will often be chosen based on the desired level of robustness. 

When uncertain parameters reflect the “true” values of moments of random variables, as is the case in mean-variance portfolio optimization, we simply have no way of knowing these unobservable true values exactly since. In such cases, after making some assumptions about the stationarity of these random processes we can generate estimates of these true parameters using statistical procedures. Goldfarb and Iyengar, for example, show that if we use a linear factor model for the multivariate returns of several assets and estimate the factor loading matrices via linear regression, the confidence regions generated for these parameters are ellipsoidal sets and they advocate their use in robust portfolio selection as uncertainty sets [29]. To generate interval type uncertainty sets, Tut¨ unc¨ u¨ and Koenig use bootstrapping strategies as well as moving averages of returns from historical data [71]. The shape and the size of the uncertainty set can significantly afect the robust solutions generated. However with few guidelines backed by theoretical and empirical studies, their choice remains an art form at the moment. 

## 19.3 Diferent Flavors of Robustness

In this section we discuss each one of the robust optimization models we mentioned above in more detail. We start with model robustness. 

## 19.3.1 Constraint Robustness

One of the most important concepts in robust optimization is constraint robustness. This refers to situations where the uncertainty is in the constraints and we seek solutions that remain feasible for all possible values of the uncertain inputs. This type of solutions are required in many engineering applications. Typical instances include multi-stage problems where the uncertain outcomes of earlier stages have an efect on the decisions of the later stages and the decision variables must be chosen to satisfy certain balance constraints (e.g., inputs to a particular stage can not exceed the outputs of the previous stage) no matter what happens with the uncertain parameters of the problem. Therefore, our solution must be constraint-robust with respect to the uncertainties of the problem. Here is a mathematical model for finding constraint-robust solutions: Consider an optimization problem of the form: 

$$
\begin{array}{c c c c} \min _ {x} & f (x) \\ & G (x, p) & \in & K. \end{array}\tag{19.1}
$$

Here, x are the decision variables, $f$ is the (certain) objective function, G and $K$ are the structural elements of the constraints that are assumed to be certain and $p$ are the possibly uncertain parameters of the problem. Consider an uncertainty set $\boldsymbol { \mathcal { U } }$ that contains all possible values of the uncertain parameters $p .$ Then, a constraint-robust optimal solution can be found by solving the following problem: 

$$
\begin{array}{r l} \min _ {x} & f (x) \\ & G (x, p) \in K, \forall p \in \mathcal {U}. \end{array}\tag{19.2}
$$

As (19.2) indicates, the robust feasible set is the intersection of the feasible sets $S ( p ) \ = \ \{ x \ : \ G ( x , p ) \in \ K \}$ indexed by the uncertainty set $\mathcal { U } .$ We illustrate this in Figure 19.1 for an ellipsoidal feasible set with $\scriptscriptstyle { \mathcal { U } } =$ $\{ p _ { 1 } , p _ { 2 } , p _ { 3 } , p _ { 4 } \}$ , where $p _ { i }$ correspond to the uncertain center of the ellipse. 

There are no uncertain parameters in the objective function of the problem (19.2). This, however, is not a restrictive assumption. An optimization problem with uncertain parameters in both the objective function and constraints can be easily reformulated to fit the form in (19.2). In fact, 

$$
\begin{array}{r c l} \min _ {x} & f (x, p) \\ & G (x, p) \end{array} \in K\tag{19.3}
$$

is equivalent to the problem: 

$$
\begin{array}{r c l} \min _ {t, x} & t \\ & t - f (x, p) & \geq 0, \\ & G (x, p) & \in K. \end{array}\tag{19.4}
$$

This last problem has all its uncertainties in its constraints. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/386a95504d504c697832e33b16b2ac2f0774d26f82181b32baf80f73feab2ad6.jpg)



Figure 19.1: Constraint robustness


Exercise 19.1 Show that if $S ( p ) = \{ x : G ( x , p ) \in K \}$ is convex for all $p ,$ then the robust feasible set $\begin{array} { r } { S : = \bigcap _ { p \in { \mathcal { U } } } S ( p ) } \end{array}$ is also convex. If $S ( p )$ is polyhedral for all $p ,$ is $S$ Tnecessarily polyhedral? 

## 19.3.2 Objective Robustness

Another important robustness concept is objective robustness. This refers to solutions that will remain close to optimal for all possible realizations of the uncertain problem parameters. Since such solutions may be dificult to obtain, especially when uncertainty sets are relatively large, an alternative goal for objective robustness is to find solutions whose worst-case behavior is optimized. The worst-case behavior of a solution corresponds to the value of the objective function for the worst possible realization of the uncertain data for that particular solution. 

We now develop a mathematical model that addresses objective robustness. Consider an optimization problem of the form: 

$$
\begin{array}{r l} \min _ {x} & f (x, p) \\ & x \in S. \end{array}\tag{19.5}
$$

Here, $S$ is the (certain) feasible set and $f$ is the objective function that depends on uncertain parameters $p .$ $\mathrm { A s }$ before, $\boldsymbol { \mathcal { U } }$ denotes the uncertain $\mathrm { t y }$ set that contains all possible values of the uncertain parameters $p .$ Then, an objective robust solution can be obtained by solving: 

$$
\min _ {x \in S} \max _ {p \in \mathcal {U}} f (x, p).\tag{19.6}
$$

We illustrate objective robustness problem (19.6) in Figure 19.2. In this example, the feasible set $S$ is the real line, the uncertainty set is $u \ : = \ :$ 

$\{ p _ { 1 } , p _ { 2 } , p _ { 3 } , p _ { 4 } , p _ { 5 } \}$ , and the objective function $f ( x , p _ { i } )$ is a convex quadratic function whose parameters $p _ { i }$ determine its shape. Note that the robust minimizer is diferent from the minimizers of each $f ( x , p _ { i } )$ which are denoted by $x _ { i } ^ { * }$ in the figure. In fact, none of the $x _ { i } ^ { * } \mathrm { { s } }$ is particularly close to the robust minimizer. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/0a68af47c79b1b142b89cab9425bfe4db35b532bdb0b0a8e3c3737e7235636e7.jpg)



Figure 19.2: Objective robustness


As the argument at the end of the previous subsection shows, objective robustness can be seen as a special case of constraint robustness via a reformulation. However, it is important to distinguish between these two problem variants as their “natural” robust formulations lead to two diferent classes of optimization formulations, namely semi-infinite and min-max optimization problems respectively. This way, diferent methodologies available for these two problem classes can be readily used for respective problems. 

Exercise 19.2 In Chapter 8, for a given constant $\lambda ,$ expected return vector $\mu ,$ , and a positive definite covariance matrix $\Sigma$ we considered the following mean-variance optimization problem: 

$$
\max _ {x \in \mathcal {X}} \mu^ {T} x - \lambda x ^ {T} \Sigma x,\tag{19.7}
$$

where $\mathcal { X } = \{ x : e ^ { T } x = 1 \}$ with $e = [ 1 1 \dots 1 ] ^ { T }$ . Here, we consider the situation where we assume $\Sigma$ to be certain and given but $\mu$ is assumed to be uncertain. For a fixed $\mu$ let $z ( \mu )$ represent the optimal value of this problem. Determine $z ( \mu )$ as an explicit function of $\mu .$ . Verify that $z ( \mu )$ is a quadratic function. Is it convex? Let represent the uncertainty set for $\mu$ and formulate the objective robustness problem. 

## 19.3.3 Relative Robustness

The focus of constraint and objective robustness models on an absolute measure of worst-case performance is not consistent with risk tolerances of many decision makers. Instead, we may prefer to measure the worst case in a relative manner, relative to the best possible solution under each scenario. This leads us to the notion of relative robustness. 

Consider the following optimization problem: 

$$
\begin{array}{l l} \min _ {x} & f (x, p) \\ & x \in S. \end{array}\tag{19.8}
$$

where $p$ is uncertain with uncertainty set $\mathcal { U } .$ . To simplify the description, we restrict our attention to the case with objective uncertainty and assume that the constraints are certain. 

Given a fixed $p \in \mathcal { U }$ , let $z ^ { \ast } ( p )$ denote the optimal value function, i.e. 

$$
z ^ {*} (p) = \min _ {x} f (x, p) \text {s.t.} x \in S.
$$

Furthermore, we define the optimal solution map 

$$
x ^ {*} (p) = \arg \min _ {x} f (x, p) \text {s.t.} x \in S.
$$

Note that $z ^ { \ast } ( p )$ can be extended-valued and $x ^ { * } ( p )$ can be set-valued. 

To motivate the notion of relative robustness we first define a measure of regret associated with a decision after the uncertainty is resolved. If we choose x as our vector and $p$ is the realized value of the uncertain parameter, the regret associated with choosing x instead of an element of $x ^ { * } ( p )$ is defined as: 

$$
r (x, p) = f (x, p) - z ^ {*} (p) = f (x, p) - f (x ^ {*} (p), p).\tag{19.9}
$$

Note that the regret function is always nonnegative and can also be regarded as a measure of the “benefit of hindsight”. 

Now, for a given x in the feasible set we consider the maximum regret function: 

$$
R (x) := \max _ {p \in \mathcal {U}} r (x, p) = \max _ {p \in \mathcal {U}} f (x, p) - f (x ^ {*} (p), p).\tag{19.10}
$$

A relative robust solution to problem (19.8) is a vector x that minimizes the maximum regret: 

$$
\min _ {x \in S} \max _ {p \in \mathcal {U}} f (x, p) - z ^ {*} (p).\tag{19.11}
$$

While they are intuitively attractive, relative robust formulations can also be significantly more dificult than the standard absolute robust formulations. Indeed, since $z ^ { \ast } ( p )$ is the optimal value function and involves an optimization problem itself, problem (19.11) is a three-level optimization problem as opposed to the two-level problems in absolute robust formulations. Furthermore, the optimal value function $z ^ { * } ( p )$ is rarely available in analytic form, is typically non-smooth and is often hard to analyze. Another dificulty is that, if f is linear in p as is often the case, then $z ^ { * } ( p )$ is a concave function. Therefore, the inner maximization problem in (19.11) is a convex maximization problem and is dificult for most . 

A simpler variant of (19.11) can be constructed by deciding on the maximum level of regret to be tolerated beforehand and by solving a feasibility problem instead with this level imposed as a constraint. For example, if we decide to limit the maximum regret to R, the problem to solve becomes the following: Find an x satisfying $G ( x ) \in K$ such that 

$$
f (x, p) - z ^ {*} (p) \leq R, \forall p \in \mathcal {U}
$$

If desired, one can then use bi-section on R to find the its optimal value. 

Another variant of relative robustness models arises when we measure the regret in terms of the proximity of our chosen solution to the optimal solution set rather than in terms of the optimal objective values. For this model, consider the following distance function for a given x and $p \mathrm { : }$ 

$$
d (x, p) = \inf _ {x * \in x * (p)} \| x - x ^ {*} \|.\tag{19.12}
$$

When the solution set is a singleton, there is no optimization involved in the definition. As above, we then consider the maximum distance function: 

$$
D (x) := \max _ {p \in \mathcal {U}} d (x, p) = \max _ {p \in \mathcal {U}} \inf _ {x * \in x * (p)} \| x - x ^ {*} \|.\tag{19.13}
$$

For relative robustness in this new sense, we seek x that 

$$
\min _ {x \in S} \max _ {p \in \mathcal {U}} d (x, p).\tag{19.14}
$$

This variant is an attractive model for cases where we have time to revise our decision variables x, perhaps only slightly, once p is revealed. In such cases, we will want to choose an x that will not need much perturbation under any scenario, i.e., we seek the solution to (19.14). This model can also be useful for multi-period problems where revisions of decisions between periods can be costly. Portfolio rebalancing problems with transaction costs are examples of such settings. 

Exercise 19.3 Formulate the relative robustness formulation for the optimization problem discussed in Exercise 19.2. Comment on the consequences of the convexity of the function $z ^ { * } ( \mu )$ . Show that the relative robustness problems for $\mathcal { U } = \{ p _ { 1 } , p _ { 2 } , . . . , p _ { k } \}$ and $\mathcal { U } = \mathrm { c o n v } ( p _ { 1 } , p _ { 2 } , \dots , p _ { k } )$ are equivalent. 

Exercise 19.4 Recall the setting in Exercise 19.2. Let $x ^ { * } ( \mu )$ denote the unique optimal solution of the problem for a given $\mu$ and obtain an explicit expression for $x ^ { * } ( \mu )$ . Using this expression, formulate the variant of the relative robustness problem given in (19.14). 

## 19.3.4 Adjustable Robust Optimization

Robust optimization formulations we saw above assume that the uncertain parameters will not be observed until all the decision variables are determined and therefore do not allow for recourse actions that may be based on realized values of some of these parameters. This is not always the appropriate model for uncertain optimization problems. In particular, multi-period decision models involve uncertain parameters some of which are revealed during the decision process. After observing these parameters, later stage decisions can respond to this new information and can correct any sub-optimality resulting from less desirable outcomes in the uncertain parameters. Adjustable robust optimization (ARO) formulations model these decision environment and allow recourse action. These models are closely related to, and in fact, partly inspired by the multi-stage stochastic programming formulations with recourse. 

ARO models were recently introduced in [5, 35] for uncertain linear programming problems. Consider, for example, the two-stage linear optimization problem given below whose first-stage decision variables $x ^ { 1 }$ need to be determined now, while the second-stage decision variables $x ^ { 2 }$ can be chosen after the uncertain parameters of the problem $A ^ { 1 } , A ^ { 2 }$ , and b are realized: 

$$
\min _ {x ^ {1}, x ^ {2}} \{c ^ {T} x ^ {1}: A ^ {1} x ^ {1} + A ^ {2} x ^ {2} \leq b \}.\tag{19.15}
$$

Note that the second stage variables $x ^ { 2 }$ do not appear in the objective function–this is what Ben-Tal et al. call the “normalized” form of the problem [5]. Problems with objective functions involving variables $x ^ { 2 }$ can be reformulated as in (19.15) after introducing an artificial variable; see Exercise 19.5. Therefore, we can focus on this simpler and convenient form without loss of generality. 

Let denote the uncertainty set for parameters $A ^ { 1 } , A ^ { 2 }$ , and b. The standard constraint robust optimization formulation for this problem seeks to find vectors $x ^ { 1 }$ and $x ^ { 2 }$ that optimize the objective function and satisfy the constraints of the problem for all possible realizations of the constraint coeficients. In this formulation, both sets of variables must be chosen before the uncertain parameters can be observed and therefore cannot depend on these parameters. Consequently, the standard robust counterpart of this problem can be written as follows: 

$$
\min _ {x ^ {1}} \left\{c ^ {T} x ^ {1}: \exists x ^ {2} \forall \left(A ^ {1}, A ^ {2}, b\right) \in \mathcal {U}: A ^ {1} x ^ {1} + A ^ {2} x ^ {2} \leq b \right\}.\tag{19.16}
$$

Note that this formulation is equivalent to the formulation we saw before, i.e. 

$$
\min _ {x ^ {1}, x ^ {2}} \{c ^ {T} x ^ {1}: A ^ {1} x ^ {1} + A ^ {2} x ^ {2} \leq b, \forall (A ^ {1}, A ^ {2}, b) \in \mathcal {U} \}.\tag{19.17}
$$

We prefer (19.16) since it illustrates the diference between this formulation and the adjustable version more clearly. 

In contrast, the adjustable robust optimization formulation allows the choice of the second-period variables $x ^ { 2 }$ to depend on the realized values of the uncertain parameters. As a result, the adjustable robust counterpart problem is given as follows: 

$$
\min _ {x ^ {1}} \{c ^ {T} x ^ {1}: \forall (A ^ {1}, A ^ {2}, b) \in \mathcal {U}, \exists x ^ {2} \equiv x ^ {2} (A ^ {1}, A ^ {2}, b): A ^ {1} x ^ {1} + A ^ {2} x ^ {2} \leq b \}.\tag{19.18}
$$

The feasible set of the second problem is larger than that of the first problem in general and therefore, the model is more flexible. ARO models can be especially useful when robust counterparts are unnecessarily conservative. The price to pay for this additional modeling flexibility appears to be the increased dificulty of the resulting ARO formulations. Even for problems where the robust counterpart is tractable, it can happen that the ARO formulation leads to an NP-hard problem. One of the factors that contribute to the added dificulty in ARO models is the fact that the feasible set of the recourse actions (second-period decisions) depends not only on the realization of the uncertain parameters but also the first-period decisions. One way to overcome this dificulty is to consider simplifying assumptions either on the uncertainty set, or on the dependence structure of recourse actions to uncertain parameters. For example, if the recourse actions are restricted to be afine functions of the uncertain parameters. While this restriction will likely give us suboptimal solutions, it may be the only strategy to obtain tractable formulations. 

Exercise 19.5 Consider the following adjustable robust optimization problem: 

$$
\min _ {x ^ {1}} \{c _ {1} ^ {T} x ^ {1} + c _ {2} ^ {T} x _ {2}: \forall (A ^ {1}, A ^ {2}, b) \in \mathcal {U},   \exists x ^ {2} \equiv x ^ {2} (A ^ {1}, A ^ {2}, b): A ^ {1} x ^ {1} + A ^ {2} x ^ {2} \leq b \}.
$$

Show how this problem can be expressed in the “normalized” form (19.18) after introducing an artificial variable. 

## 19.4 Tools and Strategies for Robust Optimization

In this section we review a few of the commonly used techniques for the solution of robust optimization problems. The tools we discuss are essentially reformulation strategies for robust optimization problems so that they can be rewritten as a deterministic optimization problem with no uncertainty. In these reformulations, we look for economy so that the new formulation is not much bigger than the original, “uncertain” problem and tractability so that the new problem can be solved eficiently using standard optimization methods. 

The variety of the robustness models and the types of uncertainty sets rule out a unified approach. However, there are some common threads and the material in this section can be seen as a guide to the available tools which can be combined or appended with other techniques to solve a given problem in the robust optimization setting. 

## 19.4.1 Sampling

One of the simplest strategies for achieving robustness under uncertainty is to sample several scenarios for the uncertain parameters from a set that contains possible values of these parameters. This sampling can be done with or without using distributional assumptions on the parameters and produces a robust optimization formulation with a finite uncertainty set. 

If uncertain parameters appear in the constraints, we create a copy of each such constraint corresponding to each scenario. Uncertainty in the objective function can be handled in a similar manner. Recall, for example, the generic uncertain optimization problem given in (19.3): 

$$
\begin{array}{r l} \min _ {x} & f (x, p) \\ & G (x, p) \in K \end{array}\tag{19.19}
$$

If the uncertainty set  is a a finite set, i.e., $\mathcal { U } = \{ p _ { 1 } , p _ { 2 } , . . . , p _ { k } \}$ , the robust formulation is obtained as follows: 

$$
\begin{array}{r c l} \min _ {t, x} & t \\ & t - f (x, p _ {i}) & \geq 0, i = 1, \ldots , k, \\ & G (x, p _ {i}) & \in K, i = 1, \ldots , k. \end{array}\tag{19.20}
$$

Note that no reformulation is necessary in this case and the duplicated constraints preserve the structural properties (linearity, convexity, etc.) of the original constraints. Consequently, when the uncertainty set is a finite set the resulting robust optimization problem is larger but theoretically no more dificult than the non-robust version of the problem. The situation is somewhat similar to stochastic programming formulations. Examples of robust optimization formulations with finite uncertainty sets can be found, e.g., in the recent book by Rustem and Howe [63]. 

## 19.4.2 Conic Optimization

Moving from finite uncertainty sets to to continuous sets such as intervals or ellipsoids presents a theoretical challenge. The robust version of an uncertain constraint that has to be satisfied for all values of the uncertain parameters in a continuous set results in a semi-infinite optimization formulation. These problems are called semi-infinite since there are infinitely many constraints– indexed by the uncertainty set–but only finitely many variables. 

Fortunately, it is possible to reformulate certain semi-infinite optimization problems using a finite set of conic constraints. Such reformulations were already introduced in Chapter 9. We recall two constraint robustness examples from that chapter: 

The robust formulation for the linear programming problem 

$$
\begin{array}{r l r} \min & c ^ {T} x \\ \mathrm{s.t.} & a ^ {T} x + b & \geq 0 \end{array}\tag{19.21}
$$

where the uncertain parameters $[ a ; b ]$ belong to the ellipsoidal uncertainty set 

$$
\mathcal {U} = \{[ a; b ] = [ a ^ {0}; b ^ {0} ] + \sum_ {j = 1} ^ {k} u _ {j} [ a ^ {j}; b ^ {j} ], \| u \| \leq 1 \}
$$

is equivalent to the following second-order cone program: 

$$
\begin{array}{r l r} \min _ {x, z} & c ^ {T} x \\ \text {s.t.} & a _ {j} ^ {T} x + b _ {j} & = z _ {j}, j = 0, \ldots , k, \\ & (z _ {0}, z _ {1}, \ldots , z _ {k}) \in C _ {q} \end{array}
$$

where $C _ { q }$ is the second-order cone defined in (9.2). 

The robust formulation for the quadratically constrained optimization problem 

$$
\begin{array}{l l} \min & c ^ {T} x \\ \text {s.t.} & - x ^ {T} (A ^ {T} A) x + 2 b ^ {T} x + \gamma \geq 0 \end{array}\tag{19.22}
$$

where the uncertain parameters $\left[ A ; b ; \gamma \right]$ belong to the ellipsoidal uncertainty set 

$$
\mathcal {U} = \{[ A; b; \gamma ] = [ A ^ {0}; b ^ {0}; \gamma^ {0} ] + \sum_ {j = 1} ^ {k} u _ {j} [ A ^ {j}; b ^ {j}; \gamma^ {j} ], \| u \| \leq 1 \}
$$

is equivalent to the following semidefinite program: 

$$
\begin{array}{l} \min _ {x, z ^ {0}, \ldots , z ^ {k}, y, \lambda} c ^ {T} x \\ \text {s.t.} A ^ {j} x = z ^ {j}, j = 0, \ldots , k, \\ (b ^ {j}) ^ {T} x = y ^ {j}, j = 0, \ldots , k, \\ \lambda \geq 0, \\ \left[ \begin{array}{c c c c} \gamma^ {0} + 2 y ^ {0} - \lambda & \left[ \begin{array}{c c c} y ^ {1} + \frac {1}{2} \gamma^ {1} & \ldots & y ^ {k} + \frac {1}{2} \gamma^ {k} \end{array} \right] & (z ^ {0}) ^ {T} \\ \left[ \begin{array}{c} y ^ {1} + \frac {1}{2} \gamma^ {1} \\ \vdots \\ y ^ {k} + \frac {1}{2} \gamma^ {k} \end{array} \right] & \lambda I & \left[ \begin{array}{c} (z ^ {1}) ^ {T} \\ \vdots \\ (z ^ {k}) ^ {T} \end{array} \right] \\ z ^ {0} & \left[ \begin{array}{c c c} z ^ {1} & \ldots & z ^ {k} \end{array} \right] & I \end{array} \right] \succeq 0. \end{array}
$$

Exercise 19.6 Consider a simple, two-variable LP with nonnegative variables and a single uncertain constraint $a _ { 1 } x _ { 1 } + a _ { 2 } x _ { 2 } + b \geq 0 . \ [ a _ { 1 } , a _ { 2 } , b ]$ belong to the following uncertainty set: 

$$
\mathcal {U} = \{[ a _ {1}, a _ {2}, b ] | [ a _ {1}, a _ {2}, b ] = [ 1, 1, 1 ] + u _ {1} [ \frac {1}{2}, 0, 0 ] + u _ {2} [ 0, \frac {1}{3}, 0 ], \| u \| \leq 1 \}.
$$

Determine the robust formulation of this constraint and the projection of the robust feasible set to the $( x _ { 1 } , x _ { 2 } )$ space. Try to approximate this set using the sampling strategy outlined above. Comment on the number of samples required until the approximate robust feasible set is a relatively good approximation of the true robust feasible set. 

## 19.4. TOOLS AND STRATEGIES FOR ROBUST OPTIMIZATION 305

Exercise 19.7 When $A \ = \ 0$ for the quadratically constrained problem (19.22) above, the problem reduces to a linearly constrained problem. Verify that when $A ^ { j } = 0$ for all $j = 0 , 1 , \ldots , k$ in the uncertainty set , the robust formulation of this problem reduces to the robust formulation of the linearly constrained problem. 

Exercise 19.8 Note that the quadratically constrained optimization problem given above can alternatively be parameterized as follows: 

$$
\begin{array}{r l r} \min & c ^ {T} x \\ \mathrm{s.t.} & - x ^ {T} \Sigma x + 2 b ^ {T} x + \gamma & \geq 0 \end{array}
$$

where we used a positive semidefinite matrix Σ instead of $A ^ { T } A$ in the constraint definition. How can we define an ellipsoidal uncertainty set for this parameterization of the problem? What are the potential advantages and potential problems with using this parameterization? 

## 19.4.3 Saddle-Point Characterizations

For the solution of problems arising from objective uncertainty, the robust solution can be characterized using saddle-point conditions when the original problem satisfies certain convexity assumptions. The benefit of this characterization is that we can then use algorithms such as interior-point methods already developed and available for saddle-point problems. 

As an example of this strategy consider the problem (19.5) from Section 19.3.2 and its robust formulation reproduced below: 

$$
\min _ {x \in S} \max _ {p \in \mathcal {U}} f (x, p).\tag{19.23}
$$

We note that the dual of this robust optimization problem is obtained by changing the order of the minimization and maximization problems: 

$$
\max _ {p \in \mathcal {U}} \min _ {x \in S} f (x, p).\tag{19.24}
$$

From standard results in convex analysis we have the following conclusion: 

Lemma 19.1 If $f ( x , p )$ is a convex function of x and concave function of p, if S and are nonempty and at least one of them is bounded the optimal values of the problems (19.23) and (19.24) coincide and there exists a saddle point $( \boldsymbol { x } ^ { * } , \boldsymbol { p } ^ { * } )$ such that 

$$
f (x ^ {*}, p) \leq f (x ^ {*}, p ^ {*}) \leq f (x, p ^ {*}), \forall x \in S, p \in \mathcal {U}.
$$

This characterization is the basis of the robust optimization algorithms given in [36, 71]. 

306 CHAPTER 19. ROBUST OPTIMIZATION: THEORY AND TOOLS 

## Chapter 20

# Robust Optimization Models in Finance

As we discussed in the previous chapter, robust optimization formulations address problems with input uncertainty. Since many financial optimization problems involve future values of security prices, interest rates, exchange rates, etc. which are not known in advance but can only be forecasted or estimated, such problems fit perfectly into the framework of robust optimization. In this chapter, we give examples of robust optimization formulations for a variety of financial optimization problems including portfolio selection, risk management, and derivatives pricing/hedging. 

We start with the application of constraint-robust optimization approach to a multi-period portfolio selection problem: 

## 20.1 Robust Multi-Period Portfolio Selection

This section is adapted from an article by Ben-Tal, Margalit, and Nemirovski [6]. We consider an investor who currently holds the portfolio $x ^ { 0 } = ( x _ { 1 } ^ { 0 } , \ldots , x _ { n } ^ { 0 } )$ , where $x _ { i } ^ { 0 }$ denotes the number of shares of asset i in the portfolio, for $i = 1 , \ldots , n .$ . Also, let $x _ { 0 } ^ { 0 }$ denote her cash holdings. She wants to determine how to adjust her portfolio in the next L investment periods to maximize her total wealth at the end of period $L .$ 

We use the following decision variables to model this multi-period portfolio selection problem: $b _ { i } ^ { l }$ denotes the number of additional shares of asset i bought at the beginning of period l and $s _ { i } ^ { l }$ denotes the number of asset i shares sold at the beginning of period l, for $i = 1 , \ldots , n$ and $l = 1 , \ldots , L$ Then, the number of shares of asset i in the portfolio at the beginning of period l, denoted $x _ { i } ^ { l }$ , is given by the following simple equation: 

$$
x _ {i} ^ {l} = x _ {i} ^ {l - 1} - s _ {i} ^ {l} + b _ {i} ^ {l}, i = 1, \ldots , n, l = 1, \ldots , L.\tag{20.1}
$$

Let $P _ { i } ^ { l }$ denote the price of a share of asset i in period l. We make the assumption that the cash account earns no interest so that $P _ { 0 } ^ { l } = 1 , \forall l$ . This is not a restrictive assumption–we can always reformulate the problem in this way after a change of numeraire. 

We assume that proportional transaction costs are paid on asset purchases and sales and denote them with $\alpha _ { i } ^ { l }$ and $\beta _ { i } ^ { l }$ for sales and purchases, respectively, for asset i and period l. We assume that $\alpha _ { i } ^ { l } \mathrm { { ^ { s } } }$ and $\beta _ { i } ^ { l } \mathrm { { ^ { s } } }$ are all known at the beginning of period 0, although they can vary from period to period and from asset to asset. Transaction costs are paid from the investor’s cash account and therefore, we have the following balance equation for the cash account: 

$$
x _ {0} ^ {l} = x _ {0} ^ {l - 1} + \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l}, l = 1, \dots , L.
$$

This balance condition indicates that the cash available at the beginning of period l is the sum of last period’s cash holdings and the proceeds from sales (discounted by transaction costs) minus the cost of new purchases. For technical reasons, we will replace the equation above with an inequality, efectively allowing the investor “burn” some of her cash if she wishes to: 

$$
x _ {0} ^ {l} \leq x _ {0} ^ {l - 1} + \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l}, l = 1, \dots , L.
$$

The objective of the investor is to maximize her total wealth at the end of period L. This objective can be represented as follows: 

$$
\max \sum_ {i = 0} ^ {n} P _ {i} ^ {L} x _ {i} ^ {L}.
$$

If we assume that all the future prices $P _ { i } ^ { l }$ are known at the time this investment problem is to be solved, we obtain the following deterministic optimization problem: 

$$
\left. \begin{array}{l l l l} \max _ {x, s, b} \sum_ {i = 0} ^ {n} P _ {i} ^ {L} x _ {i} ^ {L} \\ x _ {0} ^ {l} \leq x _ {0} ^ {l - 1} + \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l}, \\ x _ {i} ^ {l} = x _ {i} ^ {l - 1} - s _ {i} ^ {l} + b _ {i} ^ {l}, & i = 1, \ldots , n, \\ s _ {i} ^ {l} \geq 0, & i = 1, \ldots , n, \\ b _ {i} ^ {l} \geq 0, & i = 1, \ldots , n, \\ x _ {i} ^ {l} \geq 0, & i = 0, \ldots , n, \end{array} \right\} l = 1, \ldots , L.\tag{20.2}
$$

This is a linear programming problem that can be solved easily using the simplex method or interior-point methods. The nonnegativity constraints imposed by Ben-Tal et al. [6] on $x _ { i } ^ { l } \mathrm { { s } }$ disallow short positions and borrowing. We note that these constraints are not essential to the model and some or all of them can be removed to allow short sales on a subset of the assets or to allow borrowing. Observe that the investor would, of course, never choose to burn money if she is trying to maximize her final wealth. Therefore, the cash balance inequalities will always be satisfied with equality in any optimal solution of this problem. 

In a realistic setting, we do not know $P _ { i } ^ { l } { ^ { \mathrm { * } } \mathrm { s } }$ in advance and therefore cannot solve the optimal portfolio allocation problem as the linear program we developed above. Instead, we will develop a robust optimization model that incorporates the uncertainty in $P _ { i } ^ { l } \mathrm { { ^ { , } s } }$ in (20.2). Since the objective function involves uncertain parameters $P _ { i } ^ { L }$ , we first reformulate the problem as in (19.4) to move all the uncertainty to the constraints: 

$$
\left. \begin{array}{l l l} \max _ {x, s, b, t} t \\ t & \leq & \sum_ {i = 0} ^ {n} P _ {i} ^ {L} x _ {i} ^ {L} \\ x _ {0} ^ {l} & \leq & x _ {0} ^ {l - 1} + \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l}, \\ x _ {i} ^ {l} & = & x _ {i} ^ {l - 1} - s _ {i} ^ {l} + b _ {i} ^ {l}, \quad i = 1, \ldots , n, \\ s _ {i} ^ {l} & \geq & 0, \qquad \qquad \qquad \qquad i = 1, \ldots , n, \\ b _ {i} ^ {l} & \geq & 0, \qquad \qquad \qquad i = 1, \ldots , n, \\ x _ {i} ^ {l} & \geq & 0, \qquad \qquad \qquad i = 0, \ldots , n, \end{array} \right\} l = 1, \ldots , L.\tag{20.3}
$$

The first two constraints of this reformulation are the constraints that are afected by uncertainty and we would like to find a solution that satisfies these constraints for most possible realizations of the uncertain parameters $P _ { i } ^ { l }$ . To determine the robust version of these constraints, we need to choose an appropriate uncertainty set for these uncertain parameters. For this purpose, we follow a 3-σ approach common in engineering and statistical applications. 

Future prices can be assumed to be random quantities. Let us denote Future prices can be assumed to be random quantities. Let us denote the expected value of the vector $P ^ { l } = \left[ \begin{array} { c } { P _ { 1 } ^ { l } } \\ { \vdots } \\ { P _ { n } ^ { l } } \end{array} \right]$ with ${ \boldsymbol { \mu } } ^ { l } = { \left[ \begin{array} { l } { \mu _ { 1 } ^ { l } } \\ { \vdots } \\ { \mu _ { n } ^ { l } } \end{array} \right] }$ and its covariance matrix with $V ^ { l }$ . First, consider the constraint: 

$$
t \leq \sum_ {i = 0} ^ {n} P _ {i} ^ {L} x _ {i} ^ {L}.
$$

Letting $\boldsymbol { x } ^ { L } = ( x _ { 1 } ^ { L } , \dots , x _ { n } ^ { L } )$ , the expected value and the standard deviation of the right-hand-side expression are given by $x _ { 0 } ^ { L } + ( \mu ^ { L } ) ^ { T } x ^ { L } = x _ { 0 } ^ { L } + \sum _ { i = 1 } ^ { n } \mu _ { i } ^ { L } x _ { i } ^ { L }$ and $\sqrt { ( \boldsymbol { x } ^ { L } ) ^ { T } V ^ { L } \boldsymbol { x } ^ { L } }$ . If $P _ { i } ^ { L }$ quantities are normally distributed, by requiring 

$$
t \leq {\bf E} (R H S) - 3 {\bf S T D} (R H S) = x _ {0} ^ {L} + (\mu^ {L}) ^ {T} x ^ {L} - 3 \sqrt {(x ^ {L}) ^ {T} V ^ {L} x ^ {L}}\tag{20.4}
$$

we would guarantee that the (random) inequality $\begin{array} { r c l } { t } & { \leq } & { \sum _ { i = 0 } ^ { n } P _ { i } ^ { L } x _ { i } ^ { L } } \end{array}$ would Pbe satisfied more than 99% of the time. Therefore, we regard (20.4) as the “robust” version of $\begin{array} { r } { t \ \leq \ \sum _ { i = 0 } ^ { n } P _ { i } ^ { L } x _ { i } ^ { L } } \end{array}$ 

We can apply a similar logic to other constraints afected by uncertainty: 

$$
x _ {0} ^ {l} - x _ {0} ^ {l - 1} \leq \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l}, l = 1, \dots , L
$$

where we moved $x _ { 0 } ^ { l - 1 }$ to the left-hand-side to isolate the uncertain terms on the right-hand-side of the inequality. In this case, the expected value and the variance of the right-hand-side expression are given by the following formulas: 

$$
\mathbf {E} \left[ \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l} \right] = (\mu^ {l}) ^ {T} D _ {\alpha} ^ {l} s ^ {l} - (\mu^ {l}) ^ {T} D _ {\beta} ^ {l} b ^ {l}
$$

$$
= (\mu^ {l}) ^ {T} \left[ \begin{array}{c c} D _ {\alpha} ^ {l} & - D _ {\beta} ^ {l} \end{array} \right] \left[ \begin{array}{c} s ^ {l} \\ b ^ {l} \end{array} \right],
$$

and 

$$
\mathbf {V a r} \left[ \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l} \right] = \left[ \begin{array}{c} s ^ {l} \\ b ^ {l} \end{array} \right] ^ {T} \left[ \begin{array}{c} D _ {\alpha} ^ {l} \\ - D _ {\beta} ^ {l} \end{array} \right] V ^ {l} \left[ \begin{array}{c c} D _ {\alpha} ^ {l} & - D _ {\beta} ^ {l} \end{array} \right] \left[ \begin{array}{c} s ^ {l} \\ b ^ {l} \end{array} \right].
$$

Above, $D _ { \alpha }$ and $D _ { \beta }$ are the diagonal matrices 

$$
D _ {\alpha} := \left[ \begin{array}{c c c} (1 - \alpha_ {1} ^ {l}) & & \\ & \ddots & \\ & & (1 - \alpha_ {n} ^ {l}) \end{array} \right], \text {and} D _ {\beta} := \left[ \begin{array}{c c c} (1 + \beta_ {1} ^ {l}) & & \\ & \ddots & \\ & & (1 + \beta_ {n} ^ {l}) \end{array} \right].
$$

Also, $s ^ { l } = ( s _ { 1 } ^ { l } , \ldots , s _ { n } ^ { l } ) ^ { T }$ , and $b ^ { l } = ( b _ { 1 } ^ { l } , \dots , b _ { n } ^ { l } ) ^ { T }$ . Replacing 

$$
x _ {0} ^ {l} - x _ {0} ^ {l - 1} \leq \sum_ {i = 1} ^ {n} (1 - \alpha_ {i}) P _ {i} ^ {l} s _ {i} ^ {l} - \sum_ {i = 1} ^ {n} (1 + \beta_ {i}) P _ {i} ^ {l} b _ {i} ^ {l}, l = 1, \dots , L
$$

with 

$$
x _ {0} ^ {l} - x _ {0} ^ {l - 1} \leq (\mu^ {l}) ^ {T} \left[ \begin{array}{c c} D _ {\alpha} ^ {l} & - D _ {\beta} ^ {l} \end{array} \right] \left[ \begin{array}{c} s ^ {l} \\ b ^ {l} \end{array} \right] - 3 \sqrt {\left[ \begin{array}{c} s ^ {l} \\ b ^ {l} \end{array} \right] ^ {T} \left[ \begin{array}{c} D _ {\alpha} ^ {l} \\ - D _ {\beta} ^ {l} \end{array} \right] V ^ {l} \left[ \begin{array}{c c} D _ {\alpha} ^ {l} & - D _ {\beta} ^ {l} \end{array} \right] \left[ \begin{array}{c} s ^ {l} \\ b ^ {l} \end{array} \right]}
$$

we obtain a “robust” version of the constraint. Once again, assuming normality in the distribution of the uncertain parameters, by satisfying this robust constraint we can guarantee that the original constraint will be satisfied with probability more than 0.99. 

The approach above corresponds to choosing the uncertainty sets for the uncertain parameter vectors $P ^ { l }$ in the following manner: 

$$
\mathcal {U} ^ {l} := \{P ^ {l}: \sqrt {(P ^ {l} - \mu^ {l}) ^ {T} (V ^ {l}) ^ {- 1} (P ^ {l} - \mu^ {l})} \leq 3 \}, l = 1, \ldots , L.\tag{20.5}
$$

The complete uncertainty set $\mathcal { U }$ for all the uncertain parameters is the Cartesian product of the sets $\mathcal { U } ^ { l }$ defined as $\mathcal { U } = \mathcal { U } ^ { 1 } \times \ldots \times \mathcal { U } ^ { L }$ 

Exercise 20.1 Let $\mathcal { U } ^ { L }$ be as in (20.5). Show that 

$$
t \leq \sum_ {i = 0} ^ {n} P _ {i} ^ {L} x _ {i} ^ {L}, \forall P ^ {L} \in \mathcal {U} ^ {L}
$$

if and only if 

$$
t \leq (\mu^ {L}) ^ {T} x ^ {L} - 3 \sqrt {(x ^ {L}) ^ {T} V ^ {L} x ^ {L}}.
$$

Thus, our $3 { - } \sigma$ approach is equivalent to the robust formulation of this constraint using an appropriate uncertainty set. 

(Hint: You may first want to show that 

$$
\mathcal {U} ^ {L} = \{\mu^ {L} + (V ^ {L}) ^ {1 / 2} u: \| u \| \leq 3 \}.
$$

## 20.2. ROBUST PROFIT OPPORTUNITIES IN RISKY PORTFOLIOS311

The resulting problem has nonlinear constraints, because of the squareroots and quadratic terms within the square-roots as indicated in Exercise 20.1. Fortunately, however, these constraints can be written as second order cone constraints and result in a second order cone optimization problem. 

Exercise 20.2 A vector $( y ^ { 0 } , y ^ { 1 } ) \in I R \times I R ^ { k }$ belongs to the $k + 1$ dimensional second-order cone if it satisfies the following inequality: 

$$
y ^ {0} \geq \| y ^ {1} \| _ {2}.
$$

Constraints of the form above are called second-order cone constraints. Show that the constraint 

$$
t \leq (\mu^ {L}) ^ {T} x ^ {L} - 3 \sqrt {(x ^ {L}) ^ {T} V ^ {L} x ^ {L}}
$$

can be represented as a second-order cone constraint using an appropriate change of variables. You can assume that $V ^ { L }$ is a given positive definite matrix. 

## 20.2 Robust Profit Opportunities in Risky Portfolios

Consider an investment environment with n financial securities whose future price vector $r \in \mathbb { R } ^ { n }$ is a random variable. Let $p \in \varmathbb { R } ^ { n }$ represent the current prices of these securities. Consider an investor who chooses a portfolio $x = ( x _ { 1 } , \ldots , x _ { n } ) $ where $x _ { i }$ denote the number of shares of security i in the portfolio. If x satisfies 

$$
p ^ {T} x <   0
$$

meaning that the portfolio is formed with negative cash flow (by pocketing money) and if the realization r˜ at the end of the investment period of the random variable r satisfies 

$$
\tilde {r} ^ {T} x \geq 0
$$

meaning that the portfolio has a nonnegative value at the end, then the investor would get to keep the money pocketed initially, and perhaps even more. A type A arbitrage opportunity would correspond to the situation when the ending portfolio value is guaranteed to be nonnegative, i.e., when the investor can choose a portfolio x such that $p ^ { T } x < 0$ and 

$$
\mathrm{Prob} [ r ^ {T} x \geq 0 ] = 1.\tag{20.6}
$$

Since arbitrage opportunities generally do not persist in financial markets, one might be interested in the alternative and weaker profitability notion where the nonnegativity of the final portfolio is not guaranteed but is highly likely. Consider, for example, the following relaxation of (20.6): 

$$
\mathrm{Prob} [ r ^ {T} x \geq 0 ] \geq 0. 9 9.\tag{20.7}
$$

This approach can be formalized using a similar construction to what we have seen in Section 20.1. Let $\mu$ and Σ represent the expected future price vector and covariance matrix of the random vector r. Then, $\mathbf { E } ( r ^ { T } x ) = { \boldsymbol { \mu } } ^ { T } x$ and $\mathbf { S } \mathbf { T } \mathbf { D } ( r ^ { T } x ) = \sqrt { x ^ { T } \Sigma } x$ 

Exercise 20.3 If r is a Gaussian random vector with mean $\mu$ and covariance matrix Σ, then 

$$
\operatorname{Prob} [ r ^ {T} x \geq 0 ] \geq 0. 9 9 \Leftrightarrow \mu^ {T} x - \theta \sqrt {x ^ {T} \Sigma x} \geq 0,
$$

where $\theta = \Phi ^ { - 1 } ( 0 . 9 9 )$ and $\Phi ^ { - 1 } ( \cdot )$ is the inverse map of standard normal cumulative distribution function. 

As Exercise 20.3 indicates, the inequality (20.6) can be relaxed as 

$$
\mu^ {T} x - \theta \sqrt {x ^ {T} \Sigma x} \geq 0,
$$

where $\theta$ determines the likelihood of the inequality being satisfied. Therefore, if we find an x satisfying 

$$
\mu^ {T} x - \theta \sqrt {x ^ {T} \Sigma x} \geq 0, p ^ {T} x <   0
$$

for a large enough positive value of θ we have an approximation of an arbitrage opportunity called a robust profit opportunity in [57]. Note that, by relaxing the constraint $p ^ { T } x < 0$ as $p ^ { T } x \leq 0$ or using $p ^ { T } x \leq - \varepsilon$ for some $\varepsilon > 0$ , we obtain a conic feasibility system. Therefore, the resulting system can be solved using the conic optimization approaches. These ideas are explored in detail in [56, 57]. 

Exercise 20.4 Consider the robust profit opportunity formulation for a given θ: 

$$
\mu^ {T} x - \theta \sqrt {x ^ {T} \Sigma x} \geq 0, p ^ {T} x \leq 0.\tag{20.8}
$$

In this exercise, we investigate the problem of finding the largest θ for which (20.8) has a solution other than the zero vector. Namely, we want to solve 

$$
\begin{array}{r l r} \max _ {\theta , x} & \theta \\ \text {s.t.} & \mu^ {T} x - \theta \sqrt {x ^ {T} \Sigma x} & \geq 0, \\ & p ^ {T} x & \leq 0. \end{array}\tag{20.9}
$$

This problem is no longer a convex optimization problem (Why?). However, we can rewrite the first constraint as 

$$
\frac {\mu^ {T} x}{\sqrt {x ^ {T} \Sigma x}} \geq \theta .
$$

Using the strategy we employed in Section 8.2, we can take advantage of the homogeneity of the constraints in x and impose the normalizing constraint $x ^ { T } \Sigma x = 1$ to obtain the following equivalent problem: 

$$
\begin{array}{r l r} \max _ {\theta , x} & \theta \\ \mathrm{s.t.} & \mu^ {T} x - \theta & \geq 0, \\ & p ^ {T} x & \leq 0, \\ & x ^ {T} \Sigma x & = 1. \end{array}\tag{20.10}
$$

While we got rid of the fractional terms, we now have a nonlinear equality constraint that creates nonconvexity for the optimization. We can now relax the constraint $x ^ { T } \Sigma x = 1$ as $x ^ { T } \Sigma x \leq 1$ and obtain a convex optimization problem. 

$$
\begin{array}{r l r} \max _ {\theta , x} & \theta \\ \mathrm{s.t.} & \mu^ {T} x - \theta & \geq 0, \\ & p ^ {T} x & \leq 0, \\ & x ^ {T} \Sigma x & \leq 1. \end{array}\tag{20.11}
$$

This relaxation can be expressed in conic form and solved using the methods discussed in Chapter 9. However, this relaxation we solve is not equivalent to (20.9) and its solution need not be a solution to that problem in general. Find suficient conditions under which the optimal solution of (20.11) satisfies $x ^ { T } \Sigma x \leq 1$ with equality and therefore the relaxation is equivalent to the original problem. 

Exercise 20.5 Note that the fraction $\begin{array} { r } { \frac { \mu ^ { T } x } { \sqrt { x ^ { T } \Sigma x } } } \end{array}$ in the θ-maximization exercise above resembles the Sharpe ratio. Assume that one of the assets in consideration is a riskless asset which has a return of $r _ { f } .$ Show that the θ- maximization problem is equivalent to maximizing the Sharpe ratio in this case. 

## 20.3 Robust Portfolio Selection

This section is adapted from an article by Tut¨ unc¨ u¨ and Koenig [36]. Recall that Markowitz’ mean-variance optimization problem can be stated in the following form that combines the reward and risk in the objective function: 

$$
\max _ {x \in \mathcal {X}} \mu^ {T} x - \lambda x ^ {T} \Sigma x.\tag{20.12}
$$

Here $\mu _ { i }$ is an estimate of the expected return of security $i , \sigma _ { i i }$ is the variance of this return, $\sigma _ { i j }$ is the covariance between the returns of securities i and $j ,$ , λ is a risk-aversion constant used to trade-of the reward (expected return) and risk (portfolio variance). The set is the set of feasible portfolios which may carry information on short-sale restrictions, sector distribution requirements, etc. Since such restrictions are typically predetermined, we can assume that the set  is known without any uncertainty at the time the problem is solved. 

Recall that solving the problem above for diferent values of λ we can obtain the eficient frontier of the set of feasible portfolios. The optimal portfolio will be diferent for individuals with diferent risk-taking tendencies, but it will always be on the eficient frontier. 

One of the limitations of this model is its need to accurately estimate the expected returns and covariances. In [4], Bawa, Brown, and Klein argue that using estimates of the unknown expected returns and covariances leads to an estimation risk in portfolio choice, and that methods for optimal selection of portfolios must take this risk into account. Furthermore, the optimal solution is sensitive to perturbations in these input parameters—a small change in the estimate of the return or the variance may lead to a large change in the corresponding solution, see, for example, [50, 51]. This property of the solutions is undesirable for many reasons. Most importantly, results can be unintuitive and the performance often sufers as the inaccuracies in the inputs lead to severely ineficient portfolios. If the modeler wants to periodically rebalance the portfolio based on new data, she may incur significant transaction costs to do so as small changes in inputs may dictate large changes in positions. Furthermore, using point estimates of the expected return and covariance parameters do not respond to the needs of a conservative investor who does not necessarily trust these estimates and would be more comfortable choosing a portfolio that will perform well under a number of diferent scenarios. Of course, such an investor cannot expect to get better performance on some of the more likely scenarios, but may prefer to accept that in exchange for insurance against more extreme cases. All these arguments point to the need of a portfolio optimization formulation that incorporates robustness and tries to find a solution that is relatively insensitive to inaccuracies in the input data. Since all the uncertainty is in the objective function coeficients, we seek an objective robust portfolio, as outlined in the previous chapter. 

For robust portfolio optimization we consider a model that allows return and covariance matrix information to be given in the form of intervals. For example, this information may take the form “the expected return on security j is between 8% and $1 0 \% ^ { \dag }$ rather than claiming that it is, say, 9%. Mathematically, we will represent this information as membership in the following set: 

$$
\mathcal {U} = \{(\mu , \Sigma): \mu^ {L} \leq \mu \leq \mu^ {U}, \Sigma^ {L} \leq \Sigma \leq \Sigma^ {U}, \Sigma \succeq 0 \},\tag{20.13}
$$

where $\mu ^ { L } , \mu ^ { U } , \Sigma ^ { L } , \Sigma ^ { U }$ are the extreme values of the intervals we just mentioned. Recall that the notation $\Sigma \succeq 0$ indicates that the matrix Σ is a symmetric and positive semidefinite matrix. This restriction is necessary for Σ to be a valid covariance matrix. 

The uncertainty intervals in (20.13) may be generated in diferent ways. An extremely cautious modeler may want to use historical lows and highs of certain input parameters as the range of their values. In a linear factor model of returns, one may generate diferent scenarios for factor return distributions and combine these scenarios to generate the uncertainty set. Diferent analysts may produce diferent estimates for these parameters and one may choose the extreme estimates as the endpoints of the intervals. One may choose a confidence level and then generate estimates of covariance and return parameters in the form of prediction intervals. 

Using the objective robustness model in (19.6), we want to find a portfolio that maximizes the objective function in (20.12) in the worst case realization of the input parameters $\mu$ and Σ from their uncertainty set  in (20.13). Given these considerations the robust optimization problem takes the following form 

$$
\max _ {x \in \mathcal {X}} \bigl \{\min _ {(\mu , \Sigma) \in \mathcal {U}} \mu^ {T} x - \lambda x ^ {T} \Sigma x \bigr \}.\tag{20.14}
$$

Since  is bounded, using classical results of convex analysis [60], it is easy to show that (20.14) is equivalent to its dual where the order of the min and the max is reversed: 

$$
\min _ {x \in \mathcal {X}} \{\max _ {(\mu , \Sigma) \in \mathcal {U}} - \mu^ {T} x + \lambda x ^ {T} \Sigma x \}.
$$

Furthermore, the solution to (20.14) is a saddle-point of the function $f ( x , \mu , \Sigma ) =$ $\mu ^ { T } x - \lambda x ^ { T } \Sigma x$ and can be determined using the technique outlined in [36]. 

Exercise 20.6 Consider a special case of problem (20.14) where we make the following assumptions 

$x \ge 0 , \ \forall x \in \mathcal { X } \ ( \mathrm { i . e . , } \ \mathcal { X }$ includes no-shorting constraints) 

$\Sigma ^ { U }$ is positive semidefinite. 

Under these assumptions, show that (20.14) reduces to the following singlelevel maximization problem: 

$$
\max _ {x \in \mathcal {X}} \left(\mu^ {L}\right) ^ {T} x - \lambda x ^ {T} \Sigma^ {U} x.\tag{20.15}
$$

Observe that this new problem is a simple concave quadratic maximization problem and can be solved easily using, for example, interior-point methods. (Hint: Note that the objective function of (20.14) is separable in $\mu$ and Σ and that $\begin{array} { r } { x ^ { T } \Sigma x = \sum _ { i , j } \sigma _ { i j } x _ { i j } } \end{array}$ with $x _ { i j } = x _ { i } x _ { j } \ge 0$ when $x \ge 0 . )$ 1 

## 20.4 Relative Robustness in Portfolio Selection

We consider the following simple portfolio optimization example derived from an example in [18]: 

Example 20.1 

$$
\begin{array}{c} \max \mu_ {1} x _ {1} + \mu_ {2} x _ {2} + \mu_ {3} x _ {3} \\ \mathrm{TE} (x _ {1}, x _ {2}, x _ {3}) \leq 0. 1 0 \\ x _ {1} + x _ {2} + x _ {3} = 1 \\ x _ {1} \geq 0, x _ {2} \geq 0, x _ {3} \geq 0. \end{array}\tag{20.16}
$$

where 

$$
\mathrm{TE} (x _ {1}, x _ {2}, x _ {3}) = \sqrt {\left[ \begin{array}{c} x _ {1} - 0 . 5 \\ x _ {2} - 0 . 5 \\ x _ {3} \end{array} \right] ^ {T} \left[ \begin{array}{c c c} 0 . 1 7 6 4 & 0 . 0 9 7 0 2 & 0 \\ 0 . 0 9 7 0 2 & 0 . 1 0 8 9 & 0 \\ 0 & 0 & 0 \end{array} \right] \left[ \begin{array}{c} x _ {1} - 0 . 5 \\ x _ {2} - 0 . 5 \\ x _ {3} \end{array} \right]}
$$

This is essentially a two-asset portfolio optimization problem where the third asset $\left( x _ { 3 } \right)$ represents proportion of the funds that are not invested. The first two assets have standard deviations of 42% and 33% respectively and a correlation coeficient of 0.7. The “benchmark” is the portfolio that invests funds half-and-half in the two assets. The function $T E ( x )$ represents the tracking error of the portfolio with respect to the half-and-half benchmark and the first constraint indicates that this tracking error should not exceed 10%. The second constraint is the budget constraint, the third enforces no shorting. We depict the projection of the feasible set of this problem onto the space spanned by variables $x _ { 1 }$ and $x - 2$ in Figure 20.4. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/d2faa18b41a8e99f76c5e44a1acdd265157bcadf05ed4d1a7d0b1ee905d292fa.jpg)



Figure 20.1: The feasible set of the MVO problem in (20.16)


We now build a relative robustness model for this portfolio problem. We assume that the covariance matrix estimate is certain. We consider a simple uncertainty set for expected return estimates consisting of three scenarios represented with arrows in Figure 20.2. These three scenarios correspond to the following values for $( \mu _ { 1 } , \mu _ { 2 } , \mu _ { 3 } ) \colon ( 6 , 4 , 0 ) , \ ( 5 , 5 , 0 )$ , and $( 4 , 6 , 0 )$ . The optimal solution when $( \mu _ { 1 } , \mu _ { 2 } , \mu _ { 3 } ) = ( 6 , 4 , 0 ) \mathrm { i s } ( 0 . 8 3 1 , 0 . 1 6 9 , 0 )$ with an objective value of 5.662. Similarly, when $( \mu _ { 1 } , \mu _ { 2 } , \mu _ { 3 } ) = ( 4 , 6 , 0 )$ the optimal solution is (0.169, 0.831, 0) with an objective value of 5.662. When $( \mu _ { 1 } , \mu _ { 2 } , \mu _ { 3 } ) = ( 5 , 5 , 0 )$ all points between the previous two optimal solutions are optimal with a shared objective value of 5.0. Therefore, the relative robust formulation for this problem can be written as follows: 

$$
\begin{array}{r c l} \min _ {x, t} & t \\ & 5. 6 6 2 - (6 x _ {1} + 4 x _ {2}) & \leq t \\ & 5. 6 6 2 - (4 x _ {1} + 6 x _ {2}) & \leq t \\ & 5. 0 - (5 x _ {1} + 5 x _ {2}) & \leq t \\ & \mathrm{TE} (x _ {1}, x _ {2}, x _ {3}) & \leq 0. 1 0 \\ & x _ {1} + x _ {2} + x _ {3} & = 1 \\ & x _ {1} \geq 0, x _ {2} \geq 0, x _ {3} & \geq 0. \end{array}\tag{20.17}
$$

Instead of solving the problem where the optimal regret level is a variable (t in the formulation), an easier strategy is to choose a level of regret that can be tolerated and find portfolios that do not exceed this level of regret in any scenario. For example, choosing a maximum tolerable regret level of 0.75 we get the following feasibility problem: 

$$
\begin{array}{r c l} \text {Find x} \\ \text {s.t.} & 5. 6 6 2 - (6 x _ {1} + 4 x _ {2}) & \leq 0. 7 5 \\ & 5. 6 6 2 - (4 x _ {1} + 6 x _ {2}) & \leq 0. 7 5 \\ & 5. 0 - (5 x _ {1} + 5 x _ {2}) & \leq 0. 7 5 \\ & \mathrm{TE} (x _ {1}, x _ {2}, x _ {3}) & \leq 0. 1 0 \\ & x _ {1} + x _ {2} + x _ {3} & = 1 \\ & x _ {1} \geq 0, x _ {2} \geq 0, x _ {3} & \geq 0. \end{array}\tag{20.18}
$$

This problem and its feasible set of solutions is illustrated in Figure 20.2. The small shaded triangle represents the portfolios that have a regret level of 0.75 or less under all three scenarios. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c4ab939d-0fc3-47d2-a441-4ec0fc1ef1bc/eaf2312b3a273dacbda724f203084a35cc554777b2784355e5abf95bc177dc40.jpg)



Figure 20.2: Set of solutions with regret less than 0.75 in Example 20.1


Exercise 20.7 Interpret the objective function of (20.17) geometrically in Figure 20.2. Verify that the vector $x ^ { * } = ( 0 . 5 , 0 . 5 , 0 )$ solves (20.17) with the maximum regret level of $t ^ { * } = 0 . 6 6 2$ 

## 20.5 Moment Bounds for Option Prices

To price derivative securities, a common strategy is to first assume a stochastic process for the future values of the underlying process and then derive a diferential equation satisfied by the price function of the derivative security that can be solved analytically or numerically. For example, this is the strategy used in the derivation of the Black-Scholes-Merton (BSM) formula for European options. 

The prices obtained in this manner are sensitive to the model assumptions made to determine them. For example, the removal of the constant volatility assumption used in the BSM derivation deems the resulting pricing formulas incorrect. Since there is uncertainty in the correctness of the models or model parameters used for pricing derivatives, robust optimization can be used as an alternative approach. 

One variation considered in the literature assumes that we have reliable estimates of the first few moments of the risk-neutral density of the underlying asset price but have uncertainty with respect to the actual shape of this density. Then, one asks the following question: What distribution for the risk neutral density with pre-specified moments produces the highest/lowest price estimate for the derivative security? This is the approach considered in [10] where the authors argue that the convex optimization models provide a natural framework for addressing the relationship between option and stock prices in the absence of distributional information for the underlying price dynamics. 

Another strategy, often called arbitrage pricing, or robust pricing, makes no model assumptions at all and tries to produce lower and upper price bounds by examining the known prices of related securities such as other options on the same underlying, etc. This is the strategy we employed for pricing forward start options in Section 10.4. Other examples of this strategy include the work of Laurence and Wang [47]. 

Each one of these considerations lead to optimization problems. Some of these problems are easy. For example, one can find an arbitrage bound for a (possibly exotic) derivative security from a static super- or sub-replicating portfolio by solving a linear optimization problem. Other robust pricing and hedging problems can appear quite intractable. Fortunately, modern optimization models and methods continue to provide eficient solution techniques for an expanding array of financial optimization problems including pricing and hedging problems. 

## 20.6 Additional Exercises

Exercise 20.8 Recall that we considered the following two-stage stochastic linear program with recourse in Section 16.2. 

$$
\begin{array}{r c l} \max & (c ^ {1}) ^ {T} x ^ {1} + E [ \max c ^ {2} (\omega) ^ {T} x ^ {2} (\omega) ] \\ & A ^ {1} x ^ {1} & = b ^ {1} \\ & B ^ {2} (\omega) x ^ {1} + A ^ {2} (\omega) x ^ {2} (\omega) & = b ^ {2} (\omega) \\ & x ^ {1} \geq 0, & x ^ {2} (\omega) \geq 0. \end{array}\tag{20.19}
$$

In this problem, it was assumed the uncertainty in $\omega$ was of “random” nature, and therefore, the stochastic programming approach was appropriate. Now consider the case where ω is not a random variable but is known to belong to an uncertainty set . Formulate a two-stage robust linear program with recourse using the ideas developed in Section 20.1. Next, assume that $B ^ { 2 }$ and $A ^ { 2 }$ are certain (they do not depend on ω), but $b ^ { 2 }$ and $c ^ { 2 }$ are uncertain and depend afinely on ω: $b ^ { 2 } ( \omega ) = b ^ { 2 } + P \omega$ and $c ^ { 2 } ( \omega ) = c ^ { 2 } + R \omega$ 2 where $b ^ { 2 } , c ^ { 2 } , P , R$ are (certain) vectors/matrices of appropriate dimension. Also, assume that $\mathcal { U } = \{ \omega : \textstyle \sum _ { i } d _ { i } w _ { i } ^ { 2 } \le 1 \}$ for some positive constants $d _ { i }$ PCan you simplify the two-stage robust linear program with recourse under these assumptions? 

Exercise 20.9 For a given constant $\lambda ,$ , expected return vector $\mu ,$ and a positive definite covariance matrix Σ consider the following MVO problem: 

$$
\max _ {x \in \mathcal {X}} \mu^ {T} x - \lambda x ^ {T} \Sigma x,\tag{20.20}
$$

where $\mathcal { X } = \{ x : e ^ { T } x = 1 \}$ with $e = [ 1 1 \dots 1 ] ^ { T }$ . Let $z ( \mu , \Sigma )$ represent the optimal value of this problem. Determine $z ( \mu , \Sigma )$ as an explicit function of $\mu$ and Σ. Next, assume that $\mu$ and Σ are uncertain and belong to the uncertainty set $\mathcal { U } : = \{ ( \mu _ { i } , \Sigma _ { i } ) : i = 1 , \dots , m \}$ , i.e., we have a finite number of scenarios for $\mu$ and Σ. Assume also that $z ( \mu _ { i } , \Sigma _ { i } ) > 0 \ \forall i$ . Now formulate the following robust optimization problem: Find a feasible portfolio vector $x$ such that the objective value with this portfolio under each scenario is within 10% of the optimal objective value corresponding to that scenario. Discuss how this problem can be solved. What would be a good objective function for this problem? 

320 CHAPTER 20. ROBUST OPTIMIZATION MODELS IN FINANCE 

# Appendix A

## Convexity

Convexity is an important concept in mathematics, and especially in optimization, that is used to describe certain sets and certain functions. Convex sets and convex functions are related but separate mathematical entities. 

Let x and y be given points in some vector space. Then, for any $\lambda \in [ 0 , 1 ]$ the point $\lambda x + ( 1 - \lambda ) y$ is called a convex combination of x and y. The set of all convex combinations of x and y is the line segment joining these two points. 

A subset S of a given vector space X is called a convex set if $x \in S$ $y \in S ,$ and $\lambda \in [ 0 , 1 ]$ always imply that $\lambda x + ( 1 - \lambda ) y \in S$ . In other words, a convex set is characterized by the following property: for any two given points in the set, the line segment connecting these two points lies entirely in the set. 

Polyhedral sets (or polyhedra) are sets defined by linear equalities and inequalities. So, for example, the feasible region of a linear optimization problem is a polyhedral set. It is a straightforward exercise to show that polyhedral sets are convex. 

Given a convex set S, a function $f : S  \mathbb { R }$ is called a convex function ${ \mathrm { i f ~ } } \forall x \in S , y \in S$ and $\lambda \in [ 0 , 1 ]$ the following inequality holds: 

$$
f (\lambda x + (1 - \lambda) y) \leq \lambda f (x) + (1 - \lambda) f (y).
$$

We say that f is a strictly convex function if $x \in S , y \in S$ and $\lambda \in ( 0 , 1 )$ implies the following strict inequality: 

$$
f (\lambda x + (1 - \lambda) y) <   \lambda f (x) + (1 - \lambda) f (y).
$$

A function f is concave $\mathrm { i f } \ - f$ is convex. Equivalently, f is concave, if $\forall x \in S , y \in S$ and $\lambda \in [ 0 , 1 ]$ the following inequality holds: 

$$
f (\lambda x + (1 - \lambda) y) \geq \lambda f (x) + (1 - \lambda) f (y).
$$

A function f is strictly concave $\mathrm { i f } - f$ is strictly convex. 

Given $f : S  \mathbb { R }$ with $S \subset X , \operatorname { e p i } ( f ) { \mathrm { - t } }$ he epigraph of f, is the following subset of $X \times \mathbb { R } \cdot$ 

$$
\operatorname{epi} (f) := \{(x, r): x \in S, f (x) \leq r \}.
$$

f is a convex function if and only if $\operatorname { e p i } ( f )$ is a convex set. 

For a twice-continuously diferentiable function $f : S  \mathbb { R }$ with $S \subset \mathbb { R }$ 2 we have a simple characterization of convexity: f is convex on S if and only if $f ^ { \prime \prime } ( x ) \geq 0$ , $\forall x \in S$ . For multivariate functions, we have the following generalization: If $f : S  \pi$ with $S \subset \mathbb { R } ^ { n }$ is twice-continuously diferentiable, then $f$ is convex on S if and only if $\nabla ^ { 2 } f ( x )$ is positive semidefinite for all $x \in S$ . Here, $\nabla ^ { 2 } f ( x )$ denotes the (symmetric) Hessian matrix of $f ;$ namely, $\begin{array} { r } { \left[ \nabla ^ { 2 } f ( x ) \right] _ { i j } = \frac { \partial ^ { 2 } f ( x ) } { \partial x _ { i } \partial x _ { j } } , \forall i , j } \end{array}$ . Recall that a symmetric matrix $H \in \mathbb { R } ^ { n \times n }$ is positive semidefinite (positive definite) if $y ^ { T } H y \geq 0 , \forall y \in I R ^ { n }$ $( y ^ { T } H y > 0 , \forall y \in I R ^ { n } , y \neq 0 )$ 

The following theorem is one of the many reasons for the importance of convex functions and convex sets for optimization: 

Theorem A.1 Consider the following optimization problem: 

$$
\begin{array}{c c c} (\mathcal {O P}) & \min _ {x} & f (x) \\ & s. t. & x \in S \end{array}\tag{A.1}
$$

$I f S$ is a convex set and $i f f$ is a convex function of x on $S _ { i }$ , then all local optimal solutions of $\mathcal { O P }$ are also global optimal solutions. 

## Appendix B

## Cones

A cone is a set that is closed under positive scalar multiplication. In other words, a set C is a cone if $\lambda x \in C$ for all $\lambda \geq 0$ and $x \in C$ . A cone is called pointed if it does not include any lines. We will generally be dealing with closed, convex, and pointed cones. Here are a few important examples: 

$C _ { l } : = \{ x \in I R ^ { n } : x \geq 0 \}$ , the non-negative orthant. In general, any set of the form $C : = \{ x \in I R ^ { n } : A x \geq 0 \}$ for some matrix $A \in \mathcal { R } ^ { m \times n }$ is called a polyhedral cone. The subscript l is used to indicate that this cone is defined by linear inequalities. 

$C _ { q } : = \{ x = ( x _ { 0 } , x _ { 1 } , \ldots , x _ { n } ) \in I R ^ { n + 1 } : x _ { 0 } \ \geq \ \| ( x _ { 1 } , \ldots , x _ { n } ) \| \}$ , the second-order cone. This cone is also called the quadratic cone (hence the subscript $q )$ , Lorentz cone, and the ice-cream cone. 

$$
\bullet C _ {s} := \left\{X = \left[ \begin{array}{c c c} x _ {1 1} & \dots & x _ {1 n} \\ \vdots & \ddots & \vdots \\ x _ {n 1} & \dots & x _ {n n} \end{array} \right] \in \mathbb {R} ^ {n \times n}: X = X ^ {T}, X \text {is positive semidefinite} \right\},
$$

the cone of symmetric positive semidefinite matrices. 

If $C$ is a cone in a vector space $X$ with an inner product denoted by $\langle \cdot , \cdot \rangle$ ， then its dual cone is defined as follows: 

$$
C ^ {*} := \{x \in X: \langle x, y \rangle \geq 0, \forall y \in C \}.
$$

It is easy to see that the nonnegative orthant in $\varPsi ^ { n }$ (with the usual inner product) is equal to its dual cone. The same holds for the second-order cone and the cone of symmetric positive semidefinite matrices, but not for general cones. 

The polar cone is the negative of the dual cone, i.e., 

$$
C ^ {P} := \{x \in X: \langle x, y \rangle \leq 0, \forall y \in C \}.
$$

## Appendix C

## A Probability Primer

One of the most basic concepts in probability theory is a random experiment, which is an experiment whose outcome can not be determined in advance. In most cases, however, one has a (possibly infinite) set of all possible outcomes of the event; we call this set the sample space of the random experiment. For example, flipping a coin is a random experiment, so is the score of the next soccer game between Japan and Korea. The set $\Omega = \{ \mathrm { h e a d s } , ~ \mathrm { t a i 1 s } \}$ is the sample space of the first experiment, $\Omega = I N \times I N$ with $I N = \{ 0 , 1 , 2 , \ldots \}$ is the sample space for the second experiment. 

Another important concept is an event: a subset of the sample space. It is customary to say that an event occurs if the outcome of the random experiment is in the corresponding subset. $\mathrm { S o } ,$ “Japan beats Korea” is an event for the second random experiment of the previous paragraph. A class of subsets of a sample space Ω is called a field if it satisfies the following conditions: 

i) $\Omega \in { \mathcal { F } } ,$ 

ii) $A \in { \mathcal { F } }$ implies that $A ^ { c } \in { \mathcal { F } }$ , where $A ^ { c }$ is the complement of $A ,$ 

iii) A, $B \in { \mathcal { F } }$ implies $A \cup B \in { \mathcal { F } } .$ 

The second and third conditions are known as closure under complements and (finite) unions. If, in addition, satisfies 

iv) $A _ { 1 } , A _ { 2 } , \dotsc \in { \mathcal { F } }$ implies $\cup _ { i = 1 } ^ { \infty } A _ { i } \in { \mathcal { F } }$ 

then $\mathcal { F }$ is called a σ-field. The condition (iv) is closure under countable unions. Note that, for subtle reasons, Condition (iii) does not necessarily imply Condition (iv). 

A probability measure or distribution P is a real-valued function defined on a field $\mathcal { F }$ (whose elements are subsets of the sample space Ω), and satisfies the following conditions 

i) $0 \leq P ( A ) \leq 1 , { \mathrm { f o r ~ } } \forall A \in { \mathcal { F } } ,$ 

ii) $P ( \varnothing ) = 0$ , and $P ( \Omega ) = 1$ 

iii) If $A _ { 1 } , A _ { 2 } , \ldots$ . is a sequence of disjoint sets in $\mathcal { F }$ and $\mathrm { i f } \cup _ { i = 1 } ^ { \infty } A _ { i } \in { \mathcal { F } }$ , then 

$$
P (\cup_ {i = 1} ^ {\infty} A _ {i}) = \sum_ {i = 1} ^ {\infty} P (A _ {i}).
$$

The last condition above is called countable additivity. 

A probability measure is said to be discrete if Ω has countably many (and possibly finite) number of elements. A density function $f$ is a nonnegative valued integrable function that satisfies 

$$
\int_ {\Omega} f (x) d x = 1.
$$

A continuous probability distribution is a probability defined by the following relation: 

$$
P [ X \in A ] = \int_ {A} f (x) d x,
$$

for a density function $f .$ 

The collection $\Omega , \mathcal { F } \mathrm { ~ ( a ~ } \sigma \mathrm { - f i e l d }$ in Ω), and $P \ ( \mathrm { \ a }$ probability measure on $\mathcal { F } )$ is called a probability space. 

Now we are ready to define a random variable. A random variable X is a real-valued function defined on the set $\Omega ^ { \mathrm { ~ 1 ~ } }$ . Continuing with the soccer example, the diference between the goals scored by the two teams is a random variable, and so is the “winner”, a function which is equal $^ { \mathrm { t o , } }$ say, 1 if the number of goals scored by Japan is higher, 2 if the number of goals scored by Korea is higher, and 0 if they are equal. A random variable is said to be discrete (respectively, continuous) if the underlying probability space is discrete (respectively, continuous). 

The probability distribution of a random variable X is, by definition, the probability measure $P _ { X }$ in the probability space $( \Omega , { \mathcal { F } } , P )$ 

$$
P _ {X} (B) = P [ X \in B ].
$$

The distribution function F of the random variable X is defined as: 

$$
F (x) = P [ X \leq x ] = P \left[ X \in (- \infty , x ] \right].
$$

For a continuous random variable X with the density function $f ,$ 

$$
F (x) = \int_ {- \infty} ^ {x} f (x) d x
$$

and therefore $\begin{array} { r } { f ( x ) = \frac { d } { d x } F ( x ) } \end{array}$ 

A random vector $\mathbf { X } = \left( X _ { 1 } , X _ { 2 } , \ldots , X _ { k } \right)$ is a k-tuple of random variables, or equivalently, a function from Ω to $\smash { \boldsymbol { \mathit { I R } } ^ { k } }$ that satisfies a technical condition similar to the one mentioned in the footnote. The joint distribution function F of random variables $X _ { 1 } , \ldots , X _ { k }$ is defined by 

$$
F (x _ {1}, \ldots , x _ {k}) = P _ {\mathbf {X}} [ X _ {1} \leq x _ {1}, \ldots , X _ {k} \leq x _ {k} ].
$$

In the special case of $k = 2$ we have 

$$
F (x _ {1}, x _ {2}) = P _ {\mathbf {X}} [ X _ {1} \leq x _ {1}, X _ {2} \leq x _ {2} ].
$$

Given the joint distribution function of random variables $X _ { 1 }$ and $X _ { 2 }$ , their marginal distribution functions are given by the following formulas: 

$$
F _ {X _ {1}} (x _ {1}) = \lim _ {x _ {2} \to \infty} F (x _ {1}, x _ {2})
$$

and 

$$
F _ {X _ {2}} (x _ {2}) = \lim _ {x _ {1} \to \infty} F (x _ {1}, x _ {2}).
$$

We say that random variables $X _ { 1 }$ and $X _ { 2 }$ are independent if 

$$
F (x _ {1}, x _ {2}) = F _ {X _ {1}} (x _ {1}) F _ {X _ {2}} (x _ {2})
$$

for every $x _ { 1 }$ and $x _ { 2 }$ . 

The expected value (expectation, mean) of the random variable X is defined by 

$$
\begin{array}{r c l} \operatorname{E} [ X ] & = & \int_ {\Omega} x d F (x) \\ & = & \left\{ \begin{array}{l l} \sum_ {x \in \Omega} x P [ X = x ] & \text {if X is discrete} \\ \int_ {\Omega} x f (x) d x & \text {if X is continuous} \end{array} \right. \end{array}
$$

(provided that the integrals exist) and is denoted by E[X]. For a function $g ( X )$ of a random variable, the expected value of $g ( X )$ (which is itself a random variable) is given by 

$$
\operatorname{E} [ g (X) ] = \int_ {\Omega} x d F _ {g} (x) = \int_ {\Omega} g (x) d F (x).
$$

The variance of a random variable X is defined by 

$$
\begin{array}{r c l} \operatorname{Var} [ X ] & = & E \left[ (X - \operatorname{E} [ X ]) ^ {2} \right] \\ & = & \operatorname{E} [ X ^ {2} ] - (\operatorname{E} [ X ]) ^ {2}. \end{array}
$$

The standard deviation of a random variable is the square-root of its variance. 

For two jointly distributed random variables $X _ { 1 }$ and $X _ { 2 } ,$ , their covariance is defined to be 

$$
\begin{array}{r c l} \operatorname{Cov} (X _ {1}, X _ {2}) & = & E [ (X _ {1} - \operatorname{E} [ X _ {1} ]) (X _ {2} - \operatorname{E} [ X _ {2} ]) ] \\ & = & \operatorname{E} [ X _ {1} X _ {2} ] - \operatorname{E} [ X _ {1} ] \operatorname{E} [ X _ {2} ] \end{array}
$$

The correlation coeficient of two random variables is the ratio of their covariance to the product of their standard deviations. 

For a collection of random variables $X _ { 1 } , \ldots , X _ { n }$ , the expected value of the sum of these random variables is equal to the sum of their expected values: 

$$
E \left[ \sum_ {i = 1} ^ {n} X _ {i} \right] = \sum_ {i = 1} ^ {n} \mathrm{E} [ X _ {i} ].
$$

The formula for the variance of the sum of the random variables $X _ { 1 } , \ldots , X _ { n }$ is a bit more complicated: 

$$
\operatorname{Var} \left[ \sum_ {i = 1} ^ {n} X _ {i} \right] = \sum_ {i = 1} ^ {n} \operatorname{Var} [ X _ {i} ] + 2 \sum_ {1 \leq i <   j \leq n} C o v (X _ {i}, X _ {j}).
$$

# The Revised Simplex Method

As we discussed in Chapter 2, in each iteration of the simplex method, we first choose an entering variable looking at the objective row of the current tableau, and then identify a leaving variable by comparing the ratios of the numbers on the right-hand-side and the column for the entering variable. Once these two variables are identified we update the tableau. Clearly, the most time-consuming job among these steps of the method is the tableau update. If we can save some time on this bottleneck step then we can make the simplex method much faster. The revised simplex method is a variant of the simplex method developed with precisely that intention. 

The crucial question here is whether it is necessary to update the whole tableau in every iteration. To answer this question, let us try to identify what parts of the tableau are absolutely necessary to run the simplex algorithm. As we mentioned before, the first task in each iteration is to find an entering variable. Let ue recall how we do that. In a maximization problem, we look for a nonbasic variable with a positive rate of improvement. In terms of the tableau notation, this translates into having a negative coeficient in the objective row, where Z is the basic variable. 

To facilitate the discussion below let us represent a simplex tableau in an algebraic form, using the notation from Section 2.4.1. As before, we consider a linear programming problem of the form: 

$$
\begin{array}{r c l} \max & \mathbf {c x} \\ & \mathbf {A x} & \leq \mathbf {b} \\ & \mathbf {x} & \geq \mathbf {0}. \end{array}
$$

After adding the slack variables and choosing them as the initial set of basic variables we get the following “initial” or “original” tableau: 

<table><tr><td rowspan="2">Current basic variables</td><td colspan="3">Coefficient of</td><td rowspan="2">RHS</td></tr><tr><td>Z</td><td>Original nonbasics</td><td>Original basics</td></tr><tr><td>Z</td><td>1</td><td>-c</td><td>0</td><td>0</td></tr><tr><td><eq>x_B</eq></td><td>0</td><td>A</td><td>I</td><td>b</td></tr></table>

Note that we wrote the objective function equation $Z = \mathbf { c } \mathbf { x }$ as $Z - \mathbf { c x } = 0$ to keep variables on the left-hand-side and the constants on the right. In the matrix form this can be written as: 

$$
\left[ \begin{array}{c c c} 1 & - \mathbf {c c c} & \mathbf {0} \\ \mathbf {0} & \mathbf {A} & \mathbf {I} \end{array} \right] \left[ \begin{array}{c} Z \\ \mathbf {x} \\ \mathbf {x _ {s}} \end{array} \right] = \left[ \begin{array}{c} 0 \\ \mathbf {b} \end{array} \right].
$$

Pivoting, which refers to the algebraic operations performed by the simplex method in each iteration to get a representation of the problem in a particular form, can be expressed in matrix form as a premultiplication of the original matrix representation of the problem with an appropriate matrix. If the current basis matrix is B, the premultuplying matrix happens to be the following: 

$$
\left[ \begin{array}{c c} 1 & \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \\ \mathbf {0} & \mathbf {B} ^ {- 1} \end{array} \right] \cdot
$$

Multiplying this matrix with the matrices in the matrix form of the equations above we get: 

$$
\left[ \begin{array}{c c} 1 & \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \\ \mathbf {0} & \mathbf {B} ^ {- 1} \end{array} \right] \left[ \begin{array}{c c c} 1 & - \mathbf {c c c} & \mathbf {0} \\ \mathbf {0} & \mathbf {A} & \mathbf {I} \end{array} \right] = \left[ \begin{array}{c c c} 1 & \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \mathbf {A} - \mathbf {c c c} & \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \\ \mathbf {0} & \mathbf {B} ^ {- 1} \mathbf {A} & \mathbf {B} ^ {- 1} \end{array} \right],
$$

and 

$$
\left[ \begin{array}{c c} 1 & \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \\ \mathbf {0} & \mathbf {B} ^ {- 1} \end{array} \right] \left[ \begin{array}{c} 0 \\ \mathbf {b} \end{array} \right] = \left[ \begin{array}{c} \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \mathbf {b} \\ \mathbf {B} ^ {- 1} \mathbf {b} \end{array} \right]
$$

which gives us the matrix form of the set of equations in each iteration represented with respect to the current set of basic variables: 

$$
\left[ \begin{array}{c c c} 1 & \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \mathbf {A} - \mathbf {c c c} & \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \\ \mathbf {0} & \mathbf {B} ^ {- 1} \mathbf {A} & \mathbf {B} ^ {- 1} \end{array} \right] \left[ \begin{array}{c} Z \\ \mathbf {x} \\ \mathbf {x _ {s}} \end{array} \right] = \left[ \begin{array}{c} \mathbf {c _ {B}} \mathbf {B} ^ {- 1} \mathbf {b} \\ \mathbf {B} ^ {- 1} \mathbf {b} \end{array} \right]
$$

In the tableau form, this is observed in the following tableau: 

<table><tr><td rowspan="2">Current basic variables</td><td colspan="3">Coefficient of</td><td rowspan="2">RHS</td></tr><tr><td>Z</td><td>Original nonbasics</td><td>Original basics</td></tr><tr><td>Z</td><td>1</td><td><eq>\mathbf{c_{B}B^{-1}A - c}</eq></td><td><eq>\mathbf{c_{B}B^{-1}}</eq></td><td><eq>\mathbf{c_{B}B^{-1}b}</eq></td></tr><tr><td><eq>x_{B}</eq></td><td>0</td><td><eq>B^{-1}A</eq></td><td><eq>B^{-1}</eq></td><td><eq>B^{-1}b</eq></td></tr></table>

Equipped with this algebraic representation of the simplex tableau, we continue our discussion of the revised simplex method. Recall that, for a maximization problem, an entering variable must have a negative objective row coeficient. Using the tableau above, we can look for entering variables by checking whether: 

$$
1. \mathbf {c _ {B} B ^ {- 1}} \geq 0
$$

$$
2. \mathbf {c} _ {\mathbf {B}} \mathbf {B} ^ {- 1} \mathbf {A} - \mathbf {c} \geq 0
$$

Furthermore, we only need to compute the parts of these vectors corresponding to nonbasic variables, since the parts corresponding to basic variables will be zero. Now, if both inequalities above are satisfied, we stop concluding that we found an optimal solution. If not, we pick a nonbasic variable, say $x _ { k } .$ , for which the updated objective row coeficient is negative, to enter the basis. So in this step we use the updated objective function row. 

Next step is to find the leaving variable. For that, we use the updated column k for the variable $x _ { k }$ and the updated right-hand-side vector. If the column that corresponds to $x _ { k }$ in the original tableau is $A _ { k }$ , then the updated column is $\bar { \mathbf { A } } _ { \mathbf { k } } = \mathbf { B } ^ { - 1 } \mathbf { A } _ { \mathbf { k } }$ and the updated RHS vector is $\bar { \mathbf { b } } = \mathbf { B } ^ { - 1 } \mathbf { b }$ 

Next, we make a crucial observation: For the steps above, we do not need to calculate the updated columns for the nonbasic variables that are not selected to enter the basis. Notice that, if there are a lot of nonbasic variables (which would happen if there were many more variables than constraints) this would translate into substantial savings in terms of computation time. However, we need to be able to compute $\bar { \mathbf { A } } _ { \mathbf { k } } = \mathbf { B } ^ { - 1 } \mathbf { A } _ { \mathbf { k } }$ which requires the matrix $\mathbf { B } ^ { - 1 }$ . So, how do we find $\mathbf { B } ^ { - \bar { 1 } }$ in each iteration? Taking the inverse from scratch in every iteration would be too expensive, instead we can keep track of $\mathbf { B } ^ { - 1 }$ in the tableau as we iterate the simplex method. We will also keep track of the updated RHS $\bar { \mathbf { b } } = \mathbf { B } ^ { - 1 } \mathbf { b }$ . Finally, we will keep track of the expression $\pi = \mathbf { c _ { B } } \mathbf { B } ^ { - 1 }$ . Looking at the tableau in the previous page, we see that the components of π are just the updated objective function coeficients of the initial basic variables. The components of the vectors π are often called the shadow prices, or dual prices. 

Now we are ready to give an outline of the revised simplex method: 

Step 0. Find an initial feasible basis B and compute $\mathbf { B } ^ { - 1 } , \bar { \mathbf { b } } = \mathbf { B } ^ { - 1 } \mathbf { b }$ 2 and $\pi = \mathbf { c _ { B } } \mathbf { B } ^ { - 1 }$ 

Now assuming that we are given the current basis B and we know $\mathbf { B } ^ { - 1 }$ $\bar { \mathbf { b } } = \mathbf { B } ^ { - 1 } \mathbf { b }$ , and $\pi = \mathbf { c _ { B } } \mathbf { B } ^ { - 1 }$ let us try to describe the iterative steps of the revised simplex method: 

Step 1. For each nonbasic variable $x _ { i }$ calculate ${ \bar { c } } _ { i } = c _ { i } - \mathbf { c _ { B } } \mathbf { B } ^ { - 1 } \mathbf { A _ { i } } =$ $c _ { i } - \pi \mathbf { A _ { i \cdot } } \ I f \ { \bar { c } } _ { i } \leq 0$ for all nonbasic variables $x _ { i }$ , then $S T O P ,$ , the current basis is optimal. Otherwise choose a variable $x _ { k }$ such that $\bar { c } _ { k } > 0$ 

Step 2. Compute the updated column $\bar { \mathbf { A } } _ { \mathbf { k } } = \mathbf { B } ^ { - 1 } \mathbf { A } _ { \mathbf { k } }$ and perform the ratio test, i.e., find 

$$
\min _ {\bar {a} _ {i k} > 0} \{\frac {\bar {b} _ {i}}{\bar {a} _ {i k}} \}.
$$

Here $\bar { a } _ { i k }$ and ${ \bar { b } } _ { i }$ denote the $i ^ { t h }$ entry of the vectors $\bar { \mathbf { A _ { k } } }$ and $\bar { \mathbf { b } } ,$ respectively. If $\bar { a } _ { i k } \le 0$ for every row i, then STOP, the problem is unbounded. Otherwise, choose the basic variable of the row that gives the minimum ratio in the ratio test (say row r) as the leaving variable. 

The pivoting step is where we achieve the computational savings: 


Step 3. Pivot on the entry $\bar { a } _ { r k }$ in the following truncated tableau:


<table><tr><td rowspan="2">Current basic variables</td><td colspan="2">Coefficient of</td><td rowspan="2">RHS</td></tr><tr><td><eq>x_{k}</eq></td><td>Original basics</td></tr><tr><td>Z</td><td><eq>-\bar{c}_{k}</eq></td><td><eq>\pi = \mathbf{c}_{\mathbf{B}} \mathbf{B}^{-1}</eq></td><td><eq>\mathbf{c}_{\mathbf{B}} \mathbf{B}^{-1} \mathbf{b}</eq></td></tr><tr><td><eq>\vdots</eq><eq>x_{B_{r}}</eq><eq>\vdots</eq></td><td><eq>\vdots</eq><eq>\bar{a}_{rk}</eq><eq>\vdots</eq></td><td><eq>\mathbf{B}^{-1}</eq></td><td><eq>\mathbf{B}^{-1} \mathbf{b}</eq></td></tr></table>

Replace the current values of $B ^ { - 1 } , \bar { b }$ , and $\pi$ with the matrices and vectors that appear in their respective positions after pivoting. Go back to Step 1. 

Once again, notice that when we use the revised simplex method, we work with a truncated tableau. This tableau has m + 2 columns; m columns corresponding to the initial basic variables, one for the entering variable, and one for the right hand side. In the standard simplex method, we work with $n + 1$ columns, n of them for all variables, and one for the RHS vector. For a problem that has many more variables (say, $n = 5 0 , 0 0 0 )$ than constraints (say, m = 10, 000) the savings are very significant. 

## An Example

Now we apply the revised simplex method described above to a linear programming problem. We will consider the following problem: 

$$
\begin{array}{r l r l r l r l r l r l r l r l} \text {Maximize} Z = & x _ {1} + 2 x _ {2} + x _ {3} - 2 x _ {4} \\ \text {subject to:} & & & & & & & & & & & & & & \\ & - 2 x _ {1} + x _ {2} + x _ {3} + 2 x _ {4} & & + x _ {6} & & & & & = 2 \\ & - x _ {1} + 2 x _ {2} + x _ {3} & + x _ {5} & + x _ {7} & & = 7 \\ & x _ {1} & + x _ {3} + x _ {4} + x _ {5} & & + x _ {8} = 3 \\ & x _ {1}, x _ {2}, x _ {3}, x _ {4}, x _ {5}, x _ {6}, x _ {7}, x _ {8} \geq 0. \end{array}
$$

The variables $x _ { 6 } , \ x _ { 7 }$ , and $x _ { 8 }$ form a feasible basis and we will start the algorithm with this basis. Then the initial simplex tableau is as follows: 

<table><tr><td>Basic var.</td><td><eq>x_1</eq></td><td><eq>x_2</eq></td><td><eq>x_3</eq></td><td><eq>x_4</eq></td><td><eq>x_5</eq></td><td><eq>x_6</eq></td><td><eq>x_7</eq></td><td><eq>x_8</eq></td><td>RHS</td></tr><tr><td>Z</td><td>-1</td><td>-2</td><td>-1</td><td>2</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td></tr><tr><td><eq>x_6</eq></td><td>-2</td><td>1</td><td>1</td><td>2</td><td>0</td><td>1</td><td>0</td><td>0</td><td>2</td></tr><tr><td><eq>x_7</eq></td><td>-1</td><td>2</td><td>1</td><td>0</td><td>1</td><td>0</td><td>1</td><td>0</td><td>7</td></tr><tr><td><eq>x_8</eq></td><td>1</td><td>0</td><td>1</td><td>1</td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr></table>

Once a feasible basis $B$ is determined, the first thing to do in the revised simplex method is to calculate the quantities $B ^ { - 1 } , \bar { b } = B ^ { - 1 } b$ , and $\pi =$ $c _ { B } B ^ { - 1 }$ . Since the basis matrix B for the basis above is the identity, we calculate these quantities easily: 

$$
\begin{array}{r c l} B ^ {- 1} & = & I, \\ \bar {b} = B ^ {- 1} b & = & \left[ \begin{array}{l} 2 \\ 7 \\ 3 \end{array} \right], \\ \pi = c _ {B} B ^ {- 1} = [ 0 0 0 ] I & = & [ 0 0 0 ]. \end{array}
$$

Above, I denotes the identity matrix of size 3. Note that, c<sub>B</sub>, i.e., the sub-vector of the objective function vector $c = [ 1 \mathrm { ~ 2 ~ 1 ~ } - 2 \mathrm { ~ 0 ~ 0 ~ 0 ~ 0 ~ } ] ^ { T }$ that corresponds to the current basic variables, consists of all zeroes. 

Now we calculate $\bar { c } _ { i }$ values for nonbasic variables using the formula $\bar { c } _ { i } =$ $c _ { i } - \pi A _ { i }$ , where $A _ { i }$ refers to the $i ^ { t h }$ column of the initial tableau. So, 

$$
\bar {c} _ {1} = c _ {1} - \pi A _ {1} = 1 - \left[ \begin{array}{l l l} 0 & 0 & 0 \end{array} \right] \left[ \begin{array}{r} - 2 \\ - 1 \\ 1 \end{array} \right] = 1,
$$

$$
\bar {c} _ {2} = c _ {2} - \pi A _ {2} = 2 - \left[ \begin{array}{l l l} 0 & 0 & 0 \end{array} \right] \left[ \begin{array}{l} 1 \\ 2 \\ 0 \end{array} \right] = 2,
$$

and similarly, 

$$
\bar {c} _ {3} = 1, \bar {c} _ {4} = - 1, \bar {c} _ {5} = 0.
$$

The quantity $\bar { c } _ { i }$ is often called the reduced cost of the variable $x _ { i }$ and it tells us the rate of improvement in the objective function when $x _ { i }$ is introduced into the basis. Since $\bar { c } _ { 2 }$ is the largest of all $\bar { c } _ { i }$ values we choose $x _ { 2 }$ as the entering variable. 

To determine the leaving variable, we need to compute the updated column ${ \bar { A } } _ { 2 } = B ^ { - 1 } A _ { 2 } \mathrm { { : } }$ 

$$
\bar {A} _ {2} = B ^ {- 1} A _ {2} = I \left[ \begin{array}{l} 1 \\ 2 \\ 0 \end{array} \right] = \left[ \begin{array}{l} 1 \\ 2 \\ 0 \end{array} \right].
$$

Now using the updated right-hand-side vector $\bar { b } = [ 2 7 3 ] ^ { T }$ we perform the ratio test and find that $x _ { 6 } .$ , the basic variable in the row that gives the minimum ratio has to leave the basis. (Remember that we only use the positive entries of ${ \bar { A } } _ { 2 }$ in the ratio test, so the last entry, which is a zero, does not participate in the ratio test.) 

Up to here, what we have done was exactly the same as in regular simplex, only the language was diferent. The next step, the pivoting step, is going to be significantly diferent. Instead of updating the whole tableau, we will only update a reduced tableau which has one column for the entering variable, three columns for the initial basic variables, and one more column for the RHS. So, we will use the following tableau for pivoting: 

<table><tr><td rowspan="2">Basic var.</td><td rowspan="2"><eq>x_{2}</eq></td><td colspan="3">Init. basics</td><td rowspan="2">RHS</td></tr><tr><td><eq>x_{6}</eq></td><td><eq>x_{7}</eq></td><td><eq>x_{8}</eq></td></tr><tr><td>Z</td><td>-2</td><td>0</td><td>0</td><td>0</td><td>0</td></tr><tr><td><eq>x_{6}</eq></td><td>1*</td><td>1</td><td>0</td><td>0</td><td>2</td></tr><tr><td><eq>x_{7}</eq></td><td>2</td><td>0</td><td>1</td><td>0</td><td>7</td></tr><tr><td><eq>x_{8}</eq></td><td>0</td><td>0</td><td>0</td><td>1</td><td>3</td></tr></table>

As usual we pivot in the column of the entering variable and try to get a 1 in the position of the pivot element, and zeros elsewhere in the column. After pivoting we get: 

<table><tr><td rowspan="2">Basic var.</td><td rowspan="2"><eq>x_{2}</eq></td><td colspan="3">Init. basics</td><td rowspan="2">RHS</td></tr><tr><td><eq>x_{6}</eq></td><td><eq>x_{7}</eq></td><td><eq>x_{8}</eq></td></tr><tr><td>Z</td><td>0</td><td>2</td><td>0</td><td>0</td><td>4</td></tr><tr><td><eq>x_{2}</eq></td><td>1</td><td>1</td><td>0</td><td>0</td><td>2</td></tr><tr><td><eq>x_{7}</eq></td><td>0</td><td>-2</td><td>1</td><td>0</td><td>3</td></tr><tr><td><eq>x_{8}</eq></td><td>0</td><td>0</td><td>0</td><td>1</td><td>3</td></tr></table>

Now we can read the basis inverse $B ^ { - 1 }$ , updated RHS vector <sup>¯</sup>b, and the shadow prices π for the new basis from this new tableau. Recalling the algebraic form of the simplex tableau we discussed above, we see that the new basis inverse lies in the columns corresponding to the initial basic variables, so 

$$
B ^ {- 1} = \left[ \begin{array}{r r r} {1} & {0} & {0} \\ {- 2} & {1} & {0} \\ {0} & {0} & {1} \end{array} \right].
$$

Updated values of the objective function coeficients of initial basic variables and the updated RHS vector give us the π and $\bar { b }$ vectors we will use in the next iteration: 

$$
\bar {b} = \left[ \begin{array}{l} 2 \\ 3 \\ 3 \end{array} \right], \qquad \pi = [ 2 0 0 ].
$$

Above, we only updated five columns and did not worry about the four columns that correspond to $x _ { 1 } , x _ { 3 } , x _ { 4 }$ , and $x _ { 5 }$ . These are the variables that are neither in the initial basis, nor are selected to enter the basis in this iteration. 

Now, we repeat the steps above. To determine the new entering variable, we need to calculate the reduced costs $\bar { c } _ { i }$ for nonbasic variables: 

$$
\bar {c} _ {1} = c _ {1} - \pi A _ {1} = 1 - [ 2 0 0 ] \left[ \begin{array}{r} - 2 \\ - 1 \\ 1 \end{array} \right] = 5
$$

$$
\bar {c} _ {3} = c _ {3} - \pi A _ {3} = 1 - [ 2 0 0 ] \left[ \begin{array}{l} 1 \\ 1 \\ 1 \end{array} \right] = - 1,
$$

and similarly, 

$$
\bar {c} _ {4} = - 6, \bar {c} _ {5} = 0, \mathrm{and} \bar {c} _ {6} = - 2.
$$

When we look at the $- { \bar { c } } _ { i }$ values we find that only $x _ { 1 }$ is eligible to enter. $\mathrm { S o } .$ we generate the updated column ${ \bar { A } } _ { 1 } = B ^ { - 1 } A _ { 1 }$ 

$$
\bar {A} _ {1} = B ^ {- 1} A _ {1} = \left[ \begin{array}{r r r} 1 & 0 & 0 \\ - 2 & 1 & 0 \\ 0 & 0 & 1 \end{array} \right] \left[ \begin{array}{r} - 2 \\ - 1 \\ 0 \end{array} \right] = \left[ \begin{array}{r} - 2 \\ 3 \\ 1 \end{array} \right].
$$

The ratio test indicates that $x _ { 7 }$ is the leaving variable: 

$$
\min \{\frac {3}{3}, \frac {3}{1} \} = 1.
$$

Next, we pivot on the following tableau: 

<table><tr><td rowspan="2">Basic var.</td><td rowspan="2"><eq>x_1</eq></td><td colspan="3">Init. basics</td><td rowspan="2">RHS</td></tr><tr><td><eq>x_6</eq></td><td><eq>x_7</eq></td><td><eq>x_8</eq></td></tr><tr><td>Z</td><td>-5</td><td>2</td><td>0</td><td>0</td><td>4</td></tr><tr><td><eq>x_2</eq></td><td>-2</td><td>1</td><td>0</td><td>0</td><td>2</td></tr><tr><td><eq>x_7</eq></td><td>3*</td><td>-2</td><td>1</td><td>0</td><td>3</td></tr><tr><td><eq>x_8</eq></td><td>1</td><td>0</td><td>0</td><td>1</td><td>3</td></tr></table>

And we obtain: 

<table><tr><td rowspan="2">Basic var.</td><td rowspan="2"><eq>x_1</eq></td><td colspan="3">Init. basics</td><td rowspan="2">RHS</td></tr><tr><td><eq>x_6</eq></td><td><eq>x_7</eq></td><td><eq>x_8</eq></td></tr><tr><td>Z</td><td>0</td><td><eq>-\frac{4}{3}</eq></td><td><eq>\frac{5}{3}</eq></td><td>0</td><td>9</td></tr><tr><td><eq>x_2</eq></td><td>0</td><td><eq>-\frac{1}{3}</eq></td><td><eq>\frac{2}{3}</eq></td><td>0</td><td>4</td></tr><tr><td><eq>x_1</eq></td><td>1</td><td><eq>-\frac{2}{3}</eq></td><td><eq>\frac{1}{3}</eq></td><td>0</td><td>1</td></tr><tr><td><eq>x_8</eq></td><td>0</td><td><eq>\frac{2}{3}</eq></td><td><eq>-\frac{1}{3}</eq></td><td>1</td><td>2</td></tr></table>

Once again, we read new values of $B ^ { - 1 } , \bar { b } ,$ and π from this tableau: 

$$
B ^ {- 1} = \left[ \begin{array}{c c c} - \frac {1}{3} & \frac {2}{3} & 0 \\ - \frac {2}{3} & \frac {1}{3} & 0 \\ \frac {2}{3} & - \frac {1}{3} & 1 \end{array} \right], \bar {b} = \left[ \begin{array}{c} 4 \\ 1 \\ 2 \end{array} \right], \pi = [ - \frac {4}{3} \frac {5}{3} 0 ]
$$

We start the third iteration by calculating the reduced costs: 

$$
\begin{array}{r l r} \bar {c} _ {3} = c _ {3} - \pi A _ {3} = 1 - [ - \frac {4}{3} \frac {5}{3} 0 ] \left[ \begin{array}{l} 1 \\ 1 \\ 1 \end{array} \right] & = & \frac {2}{3} \\ \bar {c} _ {4} = c _ {4} - \pi A _ {4} = - 2 - [ - \frac {4}{3} \frac {5}{3} 0 ] \left[ \begin{array}{l} 2 \\ 0 \\ 1 \end{array} \right] & = & \frac {2}{3}, \end{array}
$$

and similarly, 

$$
\bar {c} _ {5} = - \frac {2}{3}, \bar {c} _ {6} = \frac {4}{3}, \mathrm{and} \bar {c} _ {7} = - \frac {5}{3}.
$$

So, $x _ { 6 }$ is chosen as the next entering variable. Once again, we calculate the updated column ${ \bar { A } } _ { 6 }$ : 

$$
\bar {A} _ {6} = B ^ {- 1} A _ {6} = \left[ \begin{array}{c c c} - \frac {1}{3} & \frac {2}{3} & 0 \\ - \frac {2}{3} & \frac {1}{3} & 0 \\ \frac {2}{3} & - \frac {1}{3} & 1 \end{array} \right] \left[ \begin{array}{c} 1 \\ 0 \\ 0 \end{array} \right] = \left[ \begin{array}{c} - \frac {1}{3} \\ - \frac {2}{3} \\ \frac {2}{3} \end{array} \right].
$$

The ratio test indicates that $x _ { 8 }$ is the leaving variable, since it is the basic variable in the only row where ${ \bar { A } } _ { 6 }$ has a positive coeficient. Now we pivot on the following tableau: 

<table><tr><td rowspan="2">Basic var.</td><td rowspan="2"><eq>x_6</eq></td><td colspan="3">Init. basics</td><td rowspan="2">RHS</td></tr><tr><td><eq>x_6</eq></td><td><eq>x_7</eq></td><td><eq>x_8</eq></td></tr><tr><td>Z</td><td><eq>-\frac{4}{3}</eq></td><td><eq>-\frac{4}{3}</eq></td><td><eq>\frac{5}{3}</eq></td><td>0</td><td>9</td></tr><tr><td><eq>x_2</eq></td><td><eq>-\frac{1}{3}</eq></td><td><eq>-\frac{1}{3}</eq></td><td><eq>\frac{2}{3}</eq></td><td>0</td><td>4</td></tr><tr><td><eq>x_1</eq></td><td><eq>-\frac{2}{3}</eq></td><td><eq>-\frac{2}{3}</eq></td><td><eq>\frac{1}{3}</eq></td><td>0</td><td>1</td></tr><tr><td><eq>x_8</eq></td><td><eq>\frac{2}{3}^*</eq></td><td><eq>\frac{2}{3}</eq></td><td><eq>-\frac{1}{3}</eq></td><td>1</td><td>2</td></tr></table>

Pivoting yields: 

<table><tr><td rowspan="2">Basic var.</td><td rowspan="2"><eq>x_6</eq></td><td colspan="3">Init. basics</td><td rowspan="2">RHS</td></tr><tr><td><eq>x_6</eq></td><td><eq>x_7</eq></td><td><eq>x_8</eq></td></tr><tr><td>Z</td><td>0</td><td>-0</td><td>1</td><td>2</td><td>13</td></tr><tr><td><eq>x_2</eq></td><td>0</td><td>0</td><td><eq>\frac{1}{2}</eq></td><td><eq>\frac{1}{2}</eq></td><td>5</td></tr><tr><td><eq>x_1</eq></td><td>0</td><td>0</td><td>0</td><td>1</td><td>3</td></tr><tr><td><eq>x_6</eq></td><td>1</td><td>1</td><td><eq>-\frac{1}{2}</eq></td><td><eq>\frac{3}{2}</eq></td><td>3</td></tr></table>

The new value of the vector $\pi$ is given by: 

$$
\pi = [ 0   1   2 ].
$$

Using π we compute 

$$
\bar {c} _ {3} = c _ {3} - \pi A _ {3} = 1 - [ 0 1 2 ] \left[ \begin{array}{l} 1 \\ 1 \\ 1 \end{array} \right] = - 2
$$

$$
\bar {c} _ {4} = c _ {4} - \pi A _ {4} = - 2 - \left[ \begin{array}{l l l} 0 & 1 & 2 \end{array} \right] \left[ \begin{array}{l} 2 \\ 0 \\ 1 \end{array} \right] = - 4
$$

$$
\begin{array}{r l r} \bar {c} _ {5} = c _ {5} - \pi A _ {5} = 0 - [ 0 1 2 ] \left[ \begin{array}{l} 0 \\ 1 \\ 1 \end{array} \right] & = & - 3 \\ \bar {c} _ {7} = c _ {7} - \pi A _ {7} = 0 - [ 0 1 2 ] \left[ \begin{array}{l} 0 \\ 1 \\ 0 \end{array} \right] & = & - 1 \\ \bar {c} _ {8} = c _ {8} - \pi A _ {8} = 0 - [ 0 1 2 ] \left[ \begin{array}{l} 0 \\ 0 \\ 1 \end{array} \right] & = & - 2 \end{array}
$$

Since all the $\bar { c } _ { i }$ values are negative we conclude that the last basis is optimal. The optimal solution is: 

$$
x _ {1} = 3, x _ {2} = 5, x _ {6} = 3, x _ {3} = x _ {4} = x _ {5} = x _ {7} = x _ {8} = 0, \mathrm{and}, z = 1 3.
$$

Exercise D.1 Consider the following linear programming problem: 

$$
\begin{array}{r l r} \max Z = & 2 0 x _ {1} + 1 0 x _ {2} \\ & x _ {1} - x _ {2} + x _ {3} & = 1 \\ & 3 x _ {1} + x _ {2} + x _ {4} & = 7 \\ & x _ {1} \geq 0, x _ {2} \geq 0, x _ {3} \geq 0, x _ {4} \geq 0. \end{array}
$$

The initial simplex tableau for this problem is given below: 

<table><tr><td rowspan="2">Basic var.</td><td colspan="5">Coefficient of</td><td rowspan="2">RHS</td></tr><tr><td>Z</td><td><eq>x_1</eq></td><td><eq>x_2</eq></td><td><eq>x_3</eq></td><td><eq>x_4</eq></td></tr><tr><td>Z</td><td>1</td><td>-20</td><td>-10</td><td>0</td><td>0</td><td>0</td></tr><tr><td><eq>x_3</eq></td><td>0</td><td>1</td><td>-1</td><td>1</td><td>0</td><td>1</td></tr><tr><td><eq>x_4</eq></td><td>0</td><td>3</td><td>1</td><td>0</td><td>1</td><td>7</td></tr></table>

Optimal set of basic variables for this problem happen to be $\{ x _ { 2 } , x _ { 3 } \}$ Write the basis matrix B for this set of basic variables and determine its inverse. Then, using the algebraic representation of the simplex tableau given in Chapter D, determine the optimal tableau corresponding to this basis. 

Exercise D.2 One of the insights of the algebraic representation of the simplex tableau we considered in Chapter D is that, the simplex tableau at any iteration can be computed from the initial tableau and the matrix $\mathbf { B } ^ { - 1 }$ , the inverse of the current basis matrix. Using this insight, one can easily answer many types of “what $\mathrm { i f } ^ { \dag }$ questions. As an example, consider the LP problem given in the previous exercise. What would happen if the right-hand-side coeficients in the initial representation of the example above were 2 and 5 instead of 1 and 7? Would the optimal basis $\{ x _ { 2 } , x _ { 3 } \}$ still be optimal? If yes, what would the new optimal solution and new optimal objective value be? 

## Bibliography



[1] A. Altay-Salih, M. C¸ . Pınar, and S. Leyfer. Constrained nonlinear programming for volatility estimation with garch models. SIAM Review, 45(3):485–503, September 2003. 





[2] F. Anderson, H. Mausser, D. Rosen, and S. Uryasev. Credit risk optimization with conditional value-at-risk criterion. Mathematical Programming B, 89:273–291, 2001. 





[3] Y. Baba, R. F. Engle, D. Kraft, and K. F. Kroner. Multivariate simultaneous generalized arch. Technical report, Department of Economics, University of California San Diego, 1989. 





[4] V. S. Bawa, S. J. Brown, and R. W. Klein. Estimation Risk and Optimal Portfolio Choice. North-Holland, Amsterdam, Netherlands, 1979. 





[5] A. Ben-Tal, A. Goyashko, E. Guslitzer, and A. Nemirovski. Adjustable robust solutions of uncertain linear programs. Mathematical Programming, 99(2):351–376, 2004. 





[6] A. Ben-Tal, T. Margalit, and A. N. Nemirovski. Robust modeling of multi-stage portfolio problems. In H. Frenk, K. Roos, T. Terlaky, and S. Zhang, editors, High Performance Optimization, pages 303–328. Kluwer Academic Publishers, 2002. 





[7] A. Ben-Tal and A. N. Nemirovski. Robust convex optimization. Mathematics of Operations Research, 23(4):769–805, 1998. 





[8] A. Ben-Tal and A. N. Nemirovski. Robust solutions of uncertain linear programs. Operations Research Letters, 25(1):1–13, 1999. 





[9] M. B´enichou, J.M. Gauthier, Girodet P., G. Hentges, G. Ribi`ere, and Vincent O. Experiments in mixed-integer linear programming. Mathematical Programming, 1:76–94, 1971. 





[10] D. Bertsimas and I. Popescu. On the relation between option and stock prices: A convex programming approach. Operations Research, 50:358– 374, 2002. 





[11] D. Bienstock. Computational study of a family of mixed-integer quadratic programming problems. Mathematical Programming A, 74:121–140, 1996. 





[12] J.R. Birge and F. Louveaux. Introduction to Stochastic Programming. Springer, 1997. 





[13] F. Black and R. Litterman. Global portfolio optimization. Financial Analysts Journal, pages 28–43, 1992. 





[14] P. T. Boggs and J. W. Tolle. Sequential quadratic programming. Acta Numerica, 4:1–51, 1996. 





[15] T. Bollerslev. Generalized autoregressive conditional heteroskedasticity. Journal of Econometrics, 31:307–327, 1986. 





[16] T. Bollerslev, R. F. Engle, and D. B. Nelson. Garch models. In R. F. Engle and D. L. McFadden, editors, Handbook of Econometrics, volume 4, pages 2961–3038. Elsevier, 1994. 





[17] D. R. Carino,˜ T. Kent, D. H. Myers, C. Stacy, M. Sylvanus, A.L. Turner, K. Watanabe, and W. Ziemba. The Russell-Yasuda Kasai model: An asset/liability model for a Japanese insurance company using multistage stochastic programming. Interfaces, 24:29–49, 1994. 





[18] S. Ceria and R. Stubbs. Robust portfolio selection... submitted, 2005. 





[19] V. Chv´atal. Linear Programming. W. H. Freeman and Company, New York, 1983. 





[20] T. F. Coleman, Y. Kim, Y. Li, and A. Verma. Dynamic hedging in a volatile market. Technical report, Cornell Theory Center, 1999. 





[21] T. F. Coleman, Y. Li, and A. Verma. Reconstructing the unknown volatility function. Journal of Computational Finance, 2(3):77–102, 1999. 





[22] G. Cornu´ejols, M. L. Fisher, and G. L. Nemhauser. Location of bank accounts to optimize float: An analytic study of exact and approximate algorithms. Management Science, 23:789–810, 1977. 





[23] J. Cox, S. Ross, and M. Rubinstein. Option pricing: A simplified approach. Journal of Financial Economics, 7(3):229–263, 1979. 





[24] M. A. H. Dempster and A. M. Ireland. A financial expert decision support system. In G. Mitra, editor, Mathematical Models for Decision Support, volume F48 of NATO ASI Series, pages 415–440. 1988. 





[25] R. F. Engle. Autoregressive conditional heteroskedasticity with estimates of the variance of the u.k. inflation. Econometrica, 50:987–1008, 1982. 





[26] Alizadeh F. and D. Goldfarb. Second-order cone programming. Mathematical Programming. 





[27] M. Fischetti and Lodi A. Local branching. Mathematical Programming B, 98:23–47, 2003. 





[28] R. Fletcher and S. Leyfer. User manual for FILTER/SQP. University of Dundee, Dundee, Scotland, 1998. 





[29] D. Goldfarb and G. Iyengar. Robust portfolio selection problems. Mathematics of Operations Research, 28:1–38, 2003. 





[30] A. J. Goldman and A. W. Tucker. Linear Equalities and Related Systems, chapter Theory of linear programming, pages 53–97. Princeton University Press, Princeton, NJ, 1956. 





[31] R. Gomory. An algorithm for the mixed integer problem. Technical report, Technical Report RM-2597, The Rand Corporation, 1960. 





[32] J. Gondzio and Kouwenberg R. High performance for asset liability management. Operations Research, 49:879–891, 2001. 





[33] C. Gourieroux. ARCH Models and Financial Applications. Springer Ser. Statist. Springer-Verlag, New York, 1997. 





[34] R. Green and B. Hollifield. When will mean-variance eficient portfolios be well-diversified. Journal of Finance, 47:1785–1810, 1992. 





[35] E. Guslitser. Uncertainty-immunized solutions in linear programming. Master’s thesis, The Technion, Haifa, 2002. 





[36] B. Halldorsson and R. H. Tut ¨ unc ¨ u. ¨ An interior-point method for a class of saddle point problems. Journal of Optimization Theory and Applications, 116(3):559–590, 2003. 





[37] R. Hauser and D. Zuev. Robust portfolio optimisation using maximisation of min eigenvalue methodology. Presentation at the Workshop on Optimization in Finance, Coimbra, Portugal, July 2005. 





[38] S. Herzel. Arbitrage opportunities on derivatives: A linear programming approach. Technical report, Department of Economics, University of Perugia, 2000. 





[39] K. Hoyland and Wallace S. W. Generating scenario trees for multistage decision problems. Management Science, 47:295–307, 2001. 





[40] P. Jorion. Portfolio optimization with tracking error constraints. Financial Analysts Journal, 59(5):70–82, September/October 2003. 





[41] L. G. Khachiyan. A polynomial algorithm in linear programming. Soviet Mathematics Doklady, 20:191–194, 1979. 





[42] P. Klaassen. Comment on ”generating scenario trees for multistage decision problems”. Management Science, 48:1512–1516, 2002. 





[43] H. Konno and H. Yamazaki. Mean-absolute deviation portfolio optimization model and its applications to tokyo stock market. Management Science, 37:519–531, 1991. 





[44] P. Kouvelis and G. Yu. Robust Discrete Optimization and its Applications. Kluwer Academic Publishers, Amsterdam, 1997. 





[45] R. Kouwenberg. Scenario generation and stochastic programming models for asset liability management. European Journal of Operational Research, 134:279–292, 2001. 





[46] R. Lagnado and S. Osher. Reconciling diferences. Risk, 10:79–83, 1997. 





[47] P. Laurence and T. H. Wang. What’s a basket worth? Risk, 17(2):73– 78, 2004. 





[48] R. Litterman and Quantitative Resources Group. Modern Investment Management: An Equilibrium Approach. John Wiley and Sons, 2003. 





[49] M.S. Lobo, L.Vandenberghe, S. Boyd, and H. Lebret. Applications of second-order cone programming. Linear Algebra and Its Applications, 284:193–228, 1998. 





[50] R. O. Michaud. The Markowitz optimization enigma: Is optimized optimal? Financial Analysts Journal, 45:31–42, 1989. 





[51] R. O. Michaud. Eficient Asset Management. Harvard Business School Press, Boston, Massachusetts, 1998. 





[52] J.J. Mor´e and S. J. Wright. Optimization Software Guide. SIAM, 1993. 





[53] J.M. Mulvey. Generating scenarios for the Towers Perrin investment system. Interfaces, 26:1–15, 1996. 





[54] Yu. Nesterov and A. Nemirovski. Interior-Point Polynomial Algorithms in Convex Programming. SIAM, Philadelphia, Pennsylvania, 1994. 





[55] J. Nocedal and S. J. Wright. Numerical Optimization. Springer-Verlag, 1999. 





[56] M. Pınar. Minimum risk arbitrage with risky financial contracts. Technical report, Bilkent University, Ankara, Turkey, 2001. 





[57] M. Pınar and R. H. Tut ¨ unc ¨ u. ¨ Robust profit opportunities in risky financial portfolios. Operations Research Letters, 33(4):331–340, 2005. 





[58] I. P´olik and T. Terlaky. S-lemma: A survey. Technical Report 2004/14, AdvOL, McMaster University, Department of Computing and Software, 2004. 





[59] C.R. Rao. Linear Stastistical Inference and its Applications. John Wiley and Sons, New York, NY, 1965. 





[60] R. T. Rockafellar. Convex Analysis. Princeton University Press, Princeton, NJ, 1970. 





[61] R. T. Rockafellar and S. Uryasev. Optimization of conditional valueat-risk. The Journal of Risk, 2:21–41, 2000. 





[62] E. I. Ronn. A new linear programming approach to bond portfolio management. Journal of Financial and Quantitative Analysis, 22:439– 466, 1987. 





[63] B. Rustem and M. Howe. Algorithms for Worst-Case Design and Applications to Risk Management. Princeton University Press, 2002. 





[64] S. M. Schaefer. Tax induced clientele efects in the market for british government securities. Journal of Financial Economics, 10:121–159, 1982. 





[65] K. Sch¨ottle and R. Werner. Benefits and costs of robust conic optimization. Technical report, T. U. Munc ¨ hen, 2006. 





[66] W. F. Sharpe. Determining a fund’s efective asset mix. Investment Management Review, pages 59–69, December 1988. 





[67] W. F. Sharpe. Asset allocation: Management style and performance measurement. Journal of Portfolio Management, pages 7–19, Winter 1992. 





[68] W.F. Sharpe. The Sharpe ratio. Journal of Portfolio Management, Fall:49–58, 1994. 





[69] J. F. Sturm. Using sedumi 1.02, a matlab toolbox for optimization over symmetric cones. Optimization Methods and Software, 11-12:625–653, 1999. 





[70] M. J. Todd. Semidefinite optimization. Acta Numerica, 10:515–560, 2001. 





[71] R. H. Tut ¨ unc ¨ u¨ and M. Koenig. Robust asset allocation. Annals of Operations Research, 132:157–187, 2004. 





[72] R. H. Tut ¨ unc ¨ u, ¨ K. C. Toh, and M. J. Todd. Solving semidefinitequadratic-linear programs using SDPT3. Mathematical Programming, 95:189–217, 2003. 





[73] S. Uryasev. Conditional value-at-risk: Optimization algorithms and applications. Financial Engineering News, 14:1–6, 2000. 





[74] L.A. Wolsey. Integer Programming. John Wiley and Sons, New York, NY, 1988. 





[75] Y. Zhao and W. T. Ziemba. The Russell-Yasuda Kasai model: A stochastic programming model using a endogenously determined worst case risk measure for dynamic asset allocation. Mathematical Programming B, 89:293–309, 2001. 



## Index

0–1 linear program, 12, 194 

absolute robust, 294 accrual tranche, 248 active constraint, 103 adaptive decision variables, 255 adjustable robust optimization, 301 adjusted random sampling, 266 ALM, 279 American option, 18, 239, 244 anticipative decision variables, 255 arbitrage, 68 arbitrage pricing, 318 arbitrage-free scenario trees, 267 Armijo-Goldstein condition, 94 ARO, 301 asset allocation, 16 asset/liability management, 20, 279 autoregressive model, 263 backward recursion in DP, 228 basic feasible solution, 32 basic solution, 30 basic variable, 32 basis matrix, 32 Bellman equation, 234 Bellman’s principle of optimality, 225 benchmark, 179 Benders decomposition, 260 beta of a security, 148 binary integer linear program, 194 binary search, 86 binomial distribution, 241 binomial lattice, 241 Black Sholes Merton option pricing formula, 117 Black-Litterman model, 149 branch and bound, 201 branch and cut, 210 

branching, 198, 203 Brownian motion, 117 BSM formula, 117 CAL, 156 call option, 18 callable debt, 282 capital allocation line, 156 capital budgeting, 194, 226 cash flow matching, 54 centered direction, 131 central path, 129 CMO, 247 collateralized mortgage obligation, 247 combinatorial auction, 213 complementary slackness, 27 concave function, 321 conditional prepayment model, 250 conditional value-at-risk, 273 cone, 323 conic optimization, 12, 169 constrained optimization, 102 constraint robustness, 14, 296 constructing an index fund, 217 constructing scenario trees, 265 contingent claim, 67 convex combination, 321 convex function, 321 convex set, 321 convexity of bond portfolio, 54 corporate debt management, 282 correlation, 328 covariance, 327 covariance matrix approximation, 182 credit migration, 276 credit rating, 248 credit risk, 276 credit spread, 251 

## INDEX

cubic spline, 161 cutting plane, 206 CVaR, 273 

decision variables, 46 dedicated portfolio, 54 dedication, 54 default risk, 248 density function, 326 derivative security, 67 deterministic DP, 226 deterministic equivalent of an SP, 257 difusion model, 118 discrete probability measure, 326 distribution function, 326 diversified portfolio, 146 dual cone, 323 dual of an LP, 24 dual QP, 124 dual simplex method, 41 duality gap, 25, 132 duration, 54 dynamic program, 13, 225 

eficient frontier, 16 eficient portfolio, 16 ellipsoidal uncertainty set, 295 entering variable, 37 European option, 18 exercise price of an option, 18 expectation, 327 expected portfolio return, 16 expected value, 327 expiration date of an option, 18 extreme point, 32 

feasibility cut, 262 feasible solution of an LP, 22 first order necessary conditions for NLP, 103 formulating an LP, 47 forward recursion in DP, 231 forward start option, 187 Frobenius norm, 183 Fundamental Theorem of Asset Pricing, 72 GARCH model, 113 

generalized reduced gradient, 105 geometric mean, 143 global optimum, 10 GMI cut, 207 golden section search, 88 Gomory mixed integer cut, 207 gradient, 96 

hedge, 18 Hessian matrix, 100 heuristic for MILP, 205 

idiosyncratic risk, 148 implied volatility, 117 independent random variables, 327 index fund, 217 index tracking, 179 infeasible problem, 9 insurance company ALM problem, 280 integer linear program, 12 integer program, 193 interior-point method, 126 internal rate of return, 86 IPM, 126 IRR, 86 

Jacobian matrix, 99 joint distribution function, 327 

Karush-Kuhn-Tucker conditions, 104 KKT conditions, 104 knapsack problem, 235 knot, 161 

L-shaped method, 260 Lagrange multiplier, 102 Lagrangian function, 102 lagrangian relaxation, 220 leaving variable, 38 line search, 93 linear factor model, 158 linear optimization, 10 linear program, 10, 21 linear programming relaxation of an MILP, 197 local optimum, 10 lockbox problem, 214 Lorenz cone, 170 

loss function, 273 loss multiple, 251 LP, 21 

marginal distribution function, 327 market return, 148 Markowitz model, 139 master problem, 261 maturity date of an option, 67 maximum regret, 299 MBS, 247 mean, 327 mean-absolute deviation model, 153 mean-variance optimization, 16, 139 Michaud’s resampling approach, 148 MILP, 194 mixed integer linear program, 12, 194 model robustness, 14 modeling, 46 modeling logical conditions, 194 mortgage-backed security, 247 multi-stage stochastic program with recourse, 258 MVO, 139 

Newton’s method, 90, 99 NLP, 83 node selection, 204 nonbasic variable, 32 nonlinear program, 10, 83 

objective function, 9 objective robustness, 15, 297 optimal solution of an LP, 22 optimality cut, 261 optimization problem, 9 option pricing, 18, 243 

pass-through MBS, 247 path-following algorithm, 130 pay down, 248 payof, 243 pension fund, 280 pivoting in simplex method, 38 polar cone, 323 polyhedral cone, 323 polyhedral set, 321 

polyhedron, 321 polynomial time algorithm, 11 polynomial-time algorithm, 44 portfolio optimization, 16, 139 portfolio optimization with minimum transaction levels, 222 positive semidefinite matrix, 11 prepayment, 250 present value, 54 primal linear program, 24 probability distribution, 325 probability measure, 325 probability space, 326 pruning a node, 199 pure integer linear program, 12, 194 pure Newton step, 131 put option, 18 

quadratic convergence, 92 quadratic program, 11, 123 

random event, 325 random sampling, 265 random variable, 326 ratio test, 38 RBSA, 158 rebalancing, 289 recourse decision, 258 recourse problem, 261 reduced cost, 32, 58, 333 regular point, 103 relative interior, 127 relative robustness, 299 replicating portfolio, 18 replication, 69, 289 required bufer, 251 return-based style analysis, 158 revised simplex method, 329 risk management, 19 risk measure, 19 risk-neutral probabilities, 70 riskless profit, 78 robust multi-period portfolio selection, 307 robust optimization, 14, 293 robust portfolio optimization, 314 robust pricing, 318 

## INDEX

saddle point, 305 sample space, 325 scenario generation, 263 scenario tree, 258 scheduled amortization, 249 second order necessary conditions for NLP, 104 second order suficient conditions for NLP, 104 second-order cone program, 169 securitization, 247 self-financing, 289 semi-definite program, 174 sensitivity analysis, 56 sequential quadratic programming, 110 shadow price, 57, 331 Sharpe ratio, 155 short sale, 17 simplex method, 38 simplex tableau, 37 slack variable, 21 software for NLP, 85 SOLVER spreadsheet, 49 spline, 161 stage in DP, 232 standard deviation, 327 standard form LP, 21 state in DP, 233 steepest descent, 95 stochastic DP, 237 stochastic linear program, 13 stochastic program, 13, 256 stochastic program with recourse, 13 strict global optimum, 10 strict local optimum, 10 strictly convex function, 321 strictly feasible, 127 strike price, 18 strong branching, 203 strong duality, 26 subgradient, 111 surplus variable, 21 symmetric matrix, 11 synthetic option, 285 

terminal node, 258 tracking error, 180 tranche, 248 transaction cost, 147, 290 transition state, 233 transpose matrix, 11 tree fitting, 266 turnover constraint, 147 two stage stochastic program with recourse, 256 type A arbitrage, 68 type B arbitrage, 68 unbounded problem, 9 uncertainty set, 294 unconstrained optimization, 95 underlying security, 18 value-at-risk, 271 VaR, 271 variance, 327 variance of portfolio return, 16 volatility estimation, 113 volatility smile, 118 WAL, 249 weak duality, 25 weighted average life, 249 yield of a bond, 87 zigzagging, 97 