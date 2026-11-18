

<!-- === Source: MinerU_markdown_Mathematical_Economics_and_Finance_Harrison_&__Waldron_1_2122706940055363587.md (Page 1) === -->

Mathematical Economics and Finance 

Michael Harrison 

Patrick Waldron 

December 2, 1998 

## Contents

List of Tables iii
List of Figures v
PREFACE vii
What Is Economics? vii
What Is Mathematics? viii
NOTATION ix
I MATHEMATICS 1
1 LINEAR ALGEBRA 3
1.1 Introduction 3
1.2 Systems of Linear Equations and Matrices 3
1.3 Matrix Operations 7
1.4 Matrix Arithmetic 7
1.5 Vectors and Vector Spaces 11
1.6 Linear Independence 12
1.7 Bases and Dimension 12
1.8 Rank 13
1.9 Eigenvalues and Eigenvectors 14
1.10 Quadratic Forms 15
1.11 Symmetric Matrices 15
1.12 Definite Matrices 15
2 VECTOR CALCULUS 17
2.1 Introduction 17
2.2 Basic Topology 17
2.3 Vector-valued Functions and Functions of Several Variables 18 

2.4 Partial and Total Derivatives 20
2.5 The Chain Rule and Product Rule 21
2.6 The Implicit Function Theorem 23
2.7 Directional Derivatives 24
2.8 Taylor's Theorem: Deterministic Version 25
2.9 The Fundamental Theorem of Calculus 26

3 CONVEXITY AND OPTIMISATION 27
3.1 Introduction 27
3.2 Convexity and Concavity 27
3.2.1 Definitions 27
3.2.2 Properties of concave functions 29
3.2.3 Convexity and differentiability 30
3.2.4 Variations on the convexity theme 34
3.3 Unconstrained Optimisation 39
3.4 Equality Constrained Optimisation: The Lagrange Multiplier Theorems 43
3.5 Inequality Constrained Optimisation: The Kuhn-Tucker Theorems 50
3.6 Duality 58

II APPLICATIONS 61
4 CHOICE UNDER CERTAINTY 63
4.1 Introduction 63
4.2 Definitions 63
4.3 Axioms 66
4.4 Optimal Response Functions: Marshallian and Hicksian Demand 69
4.4.1 The consumer's problem 69
4.4.2 The No Arbitrage Principle 70
4.4.3 Other Properties of Marshallian demand 71
4.4.4 The dual problem 72
4.4.5 Properties of Hicksian demands 73
4.5 Envelope Functions: Indirect Utility and Expenditure 73
4.6 Further Results in Demand Theory 75
4.7 General Equilibrium Theory 78
4.7.1 Walras' law 78
4.7.2 Brouwer's fixed point theorem 78 

4.7.3 Existence of equilibrium 78
4.8 The Welfare Theorems 78
4.8.1 The Edgeworth box 78
4.8.2 Pareto efficiency 78
4.8.3 The First Welfare Theorem 79
4.8.4 The Separating Hyperplane Theorem 80
4.8.5 The Second Welfare Theorem 80
4.8.6 Complete markets 82
4.8.7 Other characterizations of Pareto efficient allocations 82
4.9 Multi-period General Equilibrium 84

5 CHOICE UNDER UNCERTAINTY 85
5.1 Introduction 85
5.2 Review of Basic Probability 85
5.3 Taylor's Theorem: Stochastic Version 88
5.4 Pricing State-Contingent Claims 88
5.4.1 Completion of markets using options 90
5.4.2 Restrictions on security values implied by allocational efficiency and covariance with aggregate consumption 91
5.4.3 Completing markets with options on aggregate consumption 92
5.4.4 Replicating elementary claims with a butterfly spread 93
5.5 The Expected Utility Paradigm 93
5.5.1 Further axioms 93
5.5.2 Existence of expected utility functions 95
5.6 Jensen's Inequality and Siegel's Paradox 97
5.7 Risk Aversion 99
5.8 The Mean-Variance Paradigm 102
5.9 The Kelly Strategy 103
5.10 Alternative Non-Expected Utility Approaches 104

6 PORTFOLIO THEORY 105
6.1 Introduction 105
6.2 Notation and preliminaries 105
6.2.1 Measuring rates of return 105
6.2.2 Notation 108
6.3 The Single-period Portfolio Choice Problem 110
6.3.1 The canonical portfolio problem 110
6.3.2 Risk aversion and portfolio composition 112
6.3.3 Mutual fund separation 114
6.4 Mathematics of the Portfolio Frontier 116 

6.4.1 The portfolio frontier in $\mathbb{R}^N$ : risky assets only 116  
6.4.2 The portfolio frontier in mean-variance space: risky assets only 124  
6.4.3 The portfolio frontier in $\mathbb{R}^N$ : riskfree and risky assets 129  
6.4.4 The portfolio frontier in mean-variance space: riskfree and risky assets 129  
6.5 Market Equilibrium and the CAPM 130  
6.5.1 Pricing assets and predicting security returns 130  
6.5.2 Properties of the market portfolio 131  
6.5.3 The zero-beta CAPM 131  
6.5.4 The traditional CAPM 132  
7 INVESTMENT ANALYSIS 137  
7.1 Introduction 137  
7.2 Arbitrage and Pricing Derivative Securities 137  
7.2.1 The binomial option pricing model 137  
7.2.2 The Black-Scholes option pricing model 137  
7.3 Multi-period Investment Problems 140  
7.4 Continuous Time Investment Problems 140 

## List of Tables

3.1 Sign conditions for inequality constrained optimisation ..... 51
5.1 Payoffs for Call Options on the Aggregate Consumption ..... 92
6.1 The effect of an interest rate of 10% per annum at different frequencies of compounding. ..... 106
6.2 Notation for portfolio choice problem ..... 108 

LIST OF FIGURES 

List of Figures 

## PREFACE

This book is based on courses MA381 and EC3080, taught at Trinity College Dublin since 1992. 

Comments on content and presentation in the present draft are welcome for the benefit of future generations of students. 

An electronic version of this book (in LAT X) is available on the World Wide Web at http://pwaldron.bess.tcd.ie/teaching/ma381/notes/ although it may not always be the current version. 

The book is not intended as a substitute for students’ own lecture notes. In particular, many examples and diagrams are omitted and some material may be presented in a different sequence from year to year. 

In recent years, mathematics graduates have been increasingly expected to have additional skills in practical subjects such as economics and finance, while economics graduates have been expected to have an increasingly strong grounding in mathematics. The increasing need for those working in economics and finance to have a strong grounding in mathematics has been highlighted by such layman’s guides as ?, ?, ? (adapted from ?) and ?. In the light of these trends, the present book is aimed at advanced undergraduate students of either mathematics or economics who wish to branch out into the other subject. 

The present version lacks supporting materials in Mathematica or Maple, such as are provided with competing works like ?. 

Before starting to work through this book, mathematics students should think about the nature, subject matter and scientific methodology of economics while economics students should think about the nature, subject matter and scientific methodology of mathematics. The following sections briefly address these questions from the perspective of the outsider. 

## What Is Economics?

This section will consist of a brief verbal introduction to economics for mathematicians and an outline of the course. 

## What is economics?

1. Basic microeconomics is about the allocation of wealth or expenditure among different physical goods. This gives us relative prices. 

2. Basic finance is about the allocation of expenditure across two or more time periods. This gives us the term structure of interest rates. 

3. The next step is the allocation of expenditure across (a finite number or a continuum of) states of nature. This gives us rates of return on risky assets, which are random variables. 

Then we can try to combine 2 and 3. 

Finally we can try to combine 1 and 2 and 3. 

Thus finance is just a subset of micoreconomics. 

What do consumers do? 

They maximise ‘utility’ given a budget constraint, based on prices and income. What do firms do? 

They maximise profits, given technological constraints (and input and output prices). Microeconomics is ultimately the theory of the determination of prices by the interaction of all these decisions: all agents simultaneously maximise their objective functions subject to market clearing conditions. 

## What is Mathematics?

This section will have all the stuff about logic and proof and so on moved into it. 

## NOTATION

Throughout the book, x etc. will denote points of $\Re ^ { n }$ for $n > 1$ and $x \ e t c .$ . will denote points of < or of an arbitrary vector or metric space X. X will generally denote a matrix. 

Readers should be familiar with the symbols ∀ and ∃ and with the expressions ‘such that’ and ‘subject $\mathbf { t o } ^ { \prime }$ and also with their meaning and use, in particular with the importance of presenting the parts of a definition in the correct order and with the process of proving a theorem by arguing from the assumptions to the conclusions. Proof by contradiction and proof by contrapositive are also assumed. There is a book on proofs by Solow which should be referred to here.<sup>1</sup> 

$\mathfrak R _ { + } ^ { N } \equiv \left\{ \mathbf x \in \mathfrak R ^ { N } : x _ { i } \geq 0 , i = 1 , \ldots , N \right\}$ is used to denote the non-negative orthant of $\Re ^ { N }$ , and $\mathfrak R _ { + + } ^ { N } \equiv \left\{ \mathbf x \in \mathfrak R ^ { N } : x _ { i } > 0 , i = 1 , \ldots , N \right\}$ used to denote the positive orthant. 

<sup>></sup> is the symbol which will be used to denote the transpose of a vector or a matrix. 

Part I MATHEMATICS 

## Chapter 1

# LINEAR ALGEBRA

## 1.1 Introduction

[To be written.] 

## 1.2 Systems of Linear Equations and Matrices

Why are we interested in solving simultaneous equations? 

We often have to find a point which satisfies more than one equation simultaneously, for example when finding equilibrium price and quantity given supply and demand functions. 

• To be an equilibrium, the point (Q, P) must lie on both the supply and demand curves. 

• Now both supply and demand curves can be plotted on the same diagram and the point(s) of intersection will be the equilibrium (equilibria): 

• solving for equilibrium price and quantity is just one of many examples of the simultaneous equations problem 

• The ISLM model is another example which we will soon consider at length. 

• We will usually have many relationships between many economic variables defining equilibrium. 

The first approach to simultaneous equations is the equation counting approach: 

• a rough rule of thumb is that we need the same number of equations as unknowns 

• this is neither necessary nor sufficient for existence of a unique solution, e.g. 

– fewer equations than unknowns, unique solution: 

$$
x ^ {2} + y ^ {2} = 0 \Rightarrow x = 0, y = 0
$$

– same number of equations and unknowns but no solution (dependent equations): 

$$
\begin{array}{r c l} {x + y} & = & 1 \\ {x + y} & = & 2 \end{array}
$$

– more equations than unknowns, unique solution: 

$$
\begin{array}{r c l} {x} & = & {y} \\ {x + y} & = & 2 \\ {x - 2 y + 1} & = & 0 \end{array}
$$

$$
\Rightarrow x = 1, \qquad y = 1
$$

Now consider the geometric representation of the simultaneous equation problem, in both the generic and linear cases: 

• two curves in the coordinate plane can intersect in 0, 1 or more points 

• two surfaces in 3D coordinate space typically intersect in a curve 

• three surfaces in 3D coordinate space can intersect in 0, 1 or more points 

• a more precise theory is needed 

There are three types of elementary row operations which can be performed on a system of simultaneous equations without changing the solution(s): 

1. Add or subtract a multiple of one equation to or from another equation 

2. Multiply a particular equation by a non-zero constant 

3. Interchange two equations 

Note that each of these operations is reversible (invertible). 

Our strategy, roughly equating to Gaussian elimination involves using elementary row operations to perform the following steps: 

1. (a) Eliminate the first variable from all except the first equation 

(b) Eliminate the second variable from all except the first two equations 

(c) Eliminate the third variable from all except the first three equations 

(d) &c. 

2. We end up with only one variable in the last equation, which is easily solved. 

3. Then we can substitute this solution in the second last equation and solve for the second last variable, and so on. 

4. Check your solution!! 

Now, let us concentrate on simultaneous linear equations: 

(2 × 2 EXAMPLE) 

$$
x + y = 2\tag{1.2.1}
$$

$$
2 y - x = 7\tag{1.2.2}
$$

• Draw a picture 

• Use the Gaussian elimination method instead of the following 

• Solve for x in terms of y 

$$
\begin{array}{r c l} x & = & 2 - y \\ x & = & 2 y - 7 \end{array}
$$

• Eliminate x 

$$
2 - y = 2 y - 7
$$

• Find y 

$$
\begin{array}{r c l} {3 y} & = & 9 \\ {y} & = & 3 \end{array}
$$

• Find x from either equation: 

$$
x = 2 - y = 2 - 3 = - 1
$$

$$
x = 2 y - 7 = 6 - 7 = - 1
$$

## SIMULTANEOUS LINEAR EQUATIONS (3 × 3 EXAMPLE)

• Consider the general 3D picture . . . 

• Example: 

$$
x + 2 y + 3 z = 6\tag{1.2.3}
$$

$$
4 x + 5 y + 6 z = 1 5\tag{1.2.4}
$$

$$
7 x + 8 y + 1 0 z = 2 5\tag{1.2.5}
$$

• Solve one equation (1.2.3) for x in terms of y and z: 

$$
x = 6 - 2 y - 3 z
$$

• Eliminate x from the other two equations: 

$$
\begin{array}{r c l} {4 (6 - 2 y - 3 z) + 5 y + 6 z} & = & {1 5} \\ {7 (6 - 2 y - 3 z) + 8 y + 1 0 z} & = & {2 5} \end{array}
$$

• What remains is $\mathbf { a } \ 2 \times 2$ system: 

$$
\begin{array}{r c l} {- 3 y - 6 z} & = & {- 9} \\ {- 6 y - 1 1 z} & = & {- 1 7} \end{array}
$$

• Solve each equation for y: 

$$
\begin{array}{r c l} {y} & = & {3 - 2 z} \\ {y} & = & {\frac {1 7}{6} - \frac {1 1}{6} z} \end{array}
$$

• Eliminate y: 

$$
3 - 2 z = \frac {1 7}{6} - \frac {1 1}{6} z
$$

• Find z: 

$$
\begin{array}{r c l} \frac {1}{6} & = & \frac {1}{6} z \\ z & = & 1 \end{array}
$$

• Hence y = 1 and $x = 1$ 

Revised: December 2, 1998 

## 1.3 Matrix Operations

We motivate the need for matrix algebra by using it as a shorthand for writing systems of linear equations, such as those considered above. 

• The steps taken to solve simultaneous linear equations involve only the coefficients so we can use the following shorthand to represent the system of equations used in our example: 

This is called a matrix, i.e.— a rectangular array of numbers. 

• We use the concept of the elementary matrix to summarise the elementary row operations carried out in solving the original equations: 

(Go through the whole solution step by step again.) 

• Now the rules are 

– Working column by column from left to right, change all the below diagonal elements of the matrix to zeroes 

– Working row by row from bottom to top, change the right of diagonal elements to 0 and the diagonal elements to 1 

– Read off the solution from the last column. 

• Or we can reorder the steps to give the Gaussian elimination method: column by column everywhere. 

## 1.4 Matrix Arithmetic

• Two n × m matrices can be added and subtracted element by element. 

• There are three notations for the general $3 \times 3$ system of simultaneous linear equations: 

1. ‘Scalar’ notation: 

$$
a _ {1 1} x _ {1} + a _ {1 2} x _ {2} + a _ {1 3} x _ {3} = b _ {1}
$$

$$
a _ {2 1} x _ {1} + a _ {2 2} x _ {2} + a _ {2 3} x _ {3} = b _ {2}
$$

$$
a _ {3 1} x _ {1} + a _ {3 2} x _ {2} + a _ {3 3} x _ {3} = b _ {3}
$$

2. ‘Vector’ notation without factorisation: 

$$
\left( \begin{array}{l} a _ {1 1} x _ {1} + a _ {1 2} x _ {2} + a _ {1 3} x _ {3} \\ a _ {2 1} x _ {1} + a _ {2 2} x _ {2} + a _ {2 3} x _ {3} \\ a _ {3 1} x _ {1} + a _ {3 2} x _ {2} + a _ {3 3} x _ {3} \end{array} \right) = \left( \begin{array}{l} b _ {1} \\ b _ {2} \\ b _ {3} \end{array} \right)
$$

3. ‘Vector’ notation with factorisation: 

$$
\left( \begin{array}{c c c} a _ {1 1} & a _ {1 2} & a _ {1 3} \\ a _ {2 1} & a _ {2 2} & a _ {2 3} \\ a _ {3 1} & a _ {3 2} & a _ {3 3} \end{array} \right) \left( \begin{array}{c} x _ {1} \\ x _ {2} \\ x _ {3} \end{array} \right) = \left( \begin{array}{c} b _ {1} \\ b _ {2} \\ b _ {3} \end{array} \right)
$$

It follows that: 

$$
\left( \begin{array}{c c c} a _ {1 1} & a _ {1 2} & a _ {1 3} \\ a _ {2 1} & a _ {2 2} & a _ {2 3} \\ a _ {3 1} & a _ {3 2} & a _ {3 3} \end{array} \right) \left( \begin{array}{c} x _ {1} \\ x _ {2} \\ x _ {3} \end{array} \right) = \left( \begin{array}{c} a _ {1 1} x _ {1} + a _ {1 2} x _ {2} + a _ {1 3} x _ {3} \\ a _ {2 1} x _ {1} + a _ {2 2} x _ {2} + a _ {2 3} x _ {3} \\ a _ {3 1} x _ {1} + a _ {3 2} x _ {2} + a _ {3 3} x _ {3} \end{array} \right)
$$

• From this we can deduce the general multiplication rules: 

The ijth element of the matrix product AB is the product of the ith row of A and the jth column of B. 

A row and column can only be multiplied if they are the same ‘length.’ 

In that case, their product is the sum of the products of corresponding elements. 

Two matrices can only be multiplied if the number of columns (i.e. the row lengths) in the first equals the number of rows (i.e. the column lengths) in the second. 

• The scalar product of two vectors in $\Re ^ { n }$ is the matrix product of one written as a row vector $( 1 \times n$ matrix) and the other written as a column vector $( n \times 1$ matrix). 

• This is independent of which is written as a row and which is written as a column. 

So we have $\mathbf { C } = \mathbf { A } \mathbf { B }$ if and only if $\begin{array} { r } { c _ { i j } = \sum k = 1 ^ { n } a _ { i k } b _ { k j } } \end{array}$ 

Note that multiplication is associative but not commutative. 

Other binary matrix operations are addition and subtraction. 

Addition is associative and commutative. Subtraction is neither. 

Matrices can also be multiplied by scalars. 

Both multiplications are distributive over addition. 

We now move on to unary operations. 

The additive and multiplicative identity matrices are respectively 0 and $\mathbf { I } _ { n } \equiv \left( \delta _ { j } ^ { i } \right)$ −A and ${ { \bf A } ^ { - 1 } }$ are the corresponding inverse. Only non-singular matrices have multiplicative inverses. 

Finally, we can interpret matrices in terms of linear transformations. 

• The product of an $m \times n$ matrix and an $n \times p$ matrix is an $m \times p$ matrix. 

• The product of an $m \times n$ matrix and an $n \times 1$ matrix (vector) is an $m \times 1$ matrix (vector). 

• So every $m \times n$ matrix, A, defines a function, known as a linear transformation, 

$$
T _ {\mathbf {A}}: \Re^ {n} \to \Re^ {m}: \mathbf {x} \mapsto \mathbf {A x},
$$

which maps n−dimensional vectors to m−dimensional vectors. 

• In particular, an $n \times n$ square matrix defines a linear transformation mapping n−dimensional vectors to n−dimensional vectors. 

• The system of n simultaneous linear equations in n unknowns 

$$
\mathbf {A} \mathbf {x} = \mathbf {b}
$$

has a unique solution ∀b if and only if the corresponding linear transformation $T _ { \mathbf { A } }$ is an invertible or bijective function: A is then said to be an invertible matrix. 

A matrix has an inverse if and only the corresponding linear transformation is an invertible function: 

• Suppose $\mathbf { A } \mathbf { x } = \mathbf { b } _ { 0 }$ does not have a unique solution. Say it has two distinct solutions, $\mathbf { x } _ { 1 }$ and $\mathbf { x } _ { 2 } \left( \mathbf { x } _ { 1 } \neq \mathbf { x } _ { 2 } \right)$ 

$$
\begin{array}{r c l} \mathbf {A x} _ {1} & = & \mathbf {b} _ {0} \\ \mathbf {A x} _ {2} & = & \mathbf {b} _ {0} \end{array}
$$

This is the same thing as saying that the linear transformation $T _ { \mathbf { A } }$ is not injective, as it maps both $\mathbf { x } _ { 1 }$ and $\mathbf { X } _ { 2 }$ to the same image. 

• Then whenever x is a solution of $\mathbf { A x } = \mathbf { b } ;$ 

$$
\begin{array}{r c l} \mathbf {A} (\mathbf {x} + \mathbf {x} _ {1} - \mathbf {x} _ {2}) & = & \mathbf {A x} + \mathbf {A x} _ {1} - \mathbf {A x} _ {2} \\ & = & \mathbf {b} + \mathbf {b} _ {0} - \mathbf {b} _ {0} \\ & = & \mathbf {b}, \end{array}
$$

so $\mathbf { x } + \mathbf { x } _ { 1 } - \mathbf { x } _ { 2 }$ is another, different, solution to $\mathbf { A } \mathbf { x } = \mathbf { b }$ • So uniqueness of solution is determined by invertibility of the coefficient matrix A independent of the right hand side vector b. 

• If A is not invertible, then there will be multiple solutions for some values of b and no solutions for other values of b. 

So far, we have seen two notations for solving a system of simultaneous linear equations, both using elementary row operations. 

1. We applied the method to scalar equations (in x, y and z). 

2. We then applied it to the augmented matrix (A b) which was reduced to the augmented matrix (I x). 

Now we introduce a third notation. 

3. Each step above (about six of them depending on how things simplify) amounted to premultiplying the augmented matrix by an elementary matrix, say 

$$
\mathbf {E} _ {6} \mathbf {E} _ {5} \mathbf {E} _ {4} \mathbf {E} _ {3} \mathbf {E} _ {2} \mathbf {E} _ {1} (\mathbf {A b}) = (\mathbf {I x}).\tag{1.4.1}
$$

Picking out the first 3 columns on each side: 

$$
\mathbf {E} _ {6} \mathbf {E} _ {5} \mathbf {E} _ {4} \mathbf {E} _ {3} \mathbf {E} _ {2} \mathbf {E} _ {1} \mathbf {A} = \mathbf {I}.\tag{1.4.2}
$$

We define 

$$
\mathbf {A} ^ {- 1} \equiv \mathbf {E} _ {6} \mathbf {E} _ {5} \mathbf {E} _ {4} \mathbf {E} _ {3} \mathbf {E} _ {2} \mathbf {E} _ {1}.\tag{1.4.3}
$$

And we can use Gaussian elimination in turn to solve for each of the columns of the inverse, or to solve for the whole thing at once. 

Lots of properties of inverses are listed in MJH’s notes $( \mathsf { p } . \mathrm { A } 7 ? )$ . 

The transpose is $\mathbf { A } ^ { \top }$ , sometimes denoted A<sup>0</sup> or $\mathbf { A } ^ { t }$ . 

A matrix is symmetric if it is its own transpose; skewsymmetric if $\mathbf { A } ^ { \top } = - \mathbf { A }$ 

Note that $\left( \mathbf { A } ^ { \top } \right) ^ { - 1 } = \left( \mathbf { A } ^ { - 1 } \right) ^ { \top }$ 

Lots of strange things can happen in matrix arithmetic. 

We can have $\mathbf { A } \mathbf { B } = \mathbf { 0 }$ even if $\mathbf { A } \neq \mathbf { 0 }$ and $\mathbf { B } \neq \mathbf { 0 } .$ 

Definition 1.4.1 orthogonal rows/columns 

Definition 1.4.2 idempotent matrix $\mathbf { A } ^ { 2 } = \mathbf { A }$ 

Definition 1.4.3 orthogonal<sup>1</sup> matrix $\mathbf { A } ^ { \top } = \mathbf { A } ^ { - 1 }$ 

Definition 1.4.4 partitioned matrices 

Definition 1.4.5 determinants 

Definition 1.4.6 diagonal, triangular and scalar matrices 

<sup>1</sup>This is what ? calls something that it seems more natural to call an orthonormal matrix. 

## 1.5 Vectors and Vector Spaces

## Definition 1.5.1 A vector is just an $n \times 1$ matrix.

The Cartesian product of n sets is just the set of ordered n-tuples where the ith component of each n-tuple is an element of the ith set. 

The ordered n-tuple $( x _ { 1 } , x _ { 2 } , \ldots , x _ { n } )$ is identified with the $n \times 1$ column vector 

$$
\left( \begin{array}{c} x _ {1} \\ x _ {2} \\ \vdots \\ x _ {n} \end{array} \right).
$$

Look at pictures of points in $\Re ^ { 2 }$ and $\Re ^ { 3 }$ and think about extensions to $\Re ^ { n }$ . 

Another geometric interpretation is to say that a vector is an entity which has both magnitude and direction, while a scalar is a quantity that has magnitude only. 

Definition 1.5.2 A real (or Euclidean) vector space is a set (of vectors) in which addition and scalar multiplication (i.e. by real numbers) are defined and satisfy thefollowing axioms: 

## 1. copy axiomsfrom simms 131 notes p.1

There are vector spaces over other fields, such as the complex numbers. 

Other examples are function spaces, matrix spaces. 

On some vector spaces, we also have the notion of a dot product or scalar product: 

$$
\mathbf {u}. \mathbf {v} \equiv \mathbf {u} ^ {\top} \mathbf {v}
$$

The Euclidean norm of u is 

$$
\sqrt {\mathbf {u} . \mathbf {u}} \equiv \| \mathbf {u} \|.
$$

A unit vector is defined in the obvious way . . . unit norm. 

The distance between two vectors is just $\| \mathbf { u } - \mathbf { v } \|$ 

There are lots of interesting properties of the dot product (MJH’s theorem 2). 

We can calculate the angle between two vectors using a geometric proof based on the cosine rule. 

$$
\left\| \mathbf {v} - \mathbf {u} \right\| ^ {2} = (\mathbf {v} - \mathbf {u}). (\mathbf {v} - \mathbf {u})\tag{1.5.1}
$$

$$
= \left\| \mathbf {v} \right\| ^ {2} + \left\| \mathbf {u} \right\| ^ {2} - 2 \mathbf {v}. \mathbf {u}\tag{1.5.2}
$$

$$
= \parallel \mathbf {v} \parallel^ {2} + \parallel \mathbf {u} \parallel^ {2} - 2 \parallel \mathbf {v} \parallel \parallel \mathbf {u} \parallel \cos \theta\tag{1.5.3}
$$

Two vectors are orthogonal if and only if the angle between them is zero. 

A subspace is a subset of a vector space which is closed under addition and scalar multiplication. 

For example, consider row space, column space, solution space, orthogonal complement. 

## 1.6 Linear Independence

Definition 1.6.1 The vectors $\mathbf { x } _ { 1 } , \mathbf { x } _ { 2 } , \mathbf { x } _ { 3 } , \ldots , \mathbf { x } _ { r } \in { \mathfrak { R } } ^ { n }$ are linearly independent if and only if 

$$
\sum_ {i = 1} ^ {r} \alpha_ {i} \mathbf {x} _ {i} = \mathbf {0} \Rightarrow \alpha_ {i} = 0 \forall i.
$$

Otherwise, they are linearly dependent. 

Give examples of each, plus the standard basis. 

If $r > n$ , then the vectors must be linearly dependent. 

If the vectors are orthonormal, then they must be linearly independent. 

## 1.7 Bases and Dimension

A basis for a vector space is a set of vectors which are linearly independent and which span or generate the entire space. 

Consider the standard bases in $\Re ^ { 2 }$ and $\Re ^ { n }$ 

Any two non-collinear vectors in $\Re ^ { 2 }$ form a basis. 

A linearly independent spanning set is a basis for the subspace which it generates. 

Proof of the next result requires stuff that has not yet been covered. 

If a basis has n elements then any set of more than n elements is linearly dependent and any set of less than n elements doesn’t span. 

Or something like that. 

Definition 1.7.1 The dimension of a vector space is the (unique) number of vectors in a basis. The dimension ofthe vector space {0} is zero. 

Definition 1.7.2 Orthogonal complement 

Decomposition into subspace and its orthogonal complement. 

Revised: December 2, 1998 

## 1.8 Rank

## Definition 1.8.1

The row space of an $m \times n$ matrix A is the vector subspace of $\Re ^ { n }$ generated by the m rows ofA. 

The row rank ofa matrix is the dimension ofits row space. 

The column space ofan m $\times \ n$ matrix A is the vector subspace of $\Re ^ { m }$ generated by the n columns ofA. 

The column rank ofa matrix is the dimension ofits column space. 

Theorem 1.8.1 The row space and the column space ofany matrix have the same dimension. 

Proof The idea of the proof is that performing elementary row operations on a matrix does not change either the row rank or the column rank of the matrix. 

Using a procedure similar to Gaussian elimination, every matrix can be reduced to a matrix in reduced row echelon form (a partitioned matrix with an identity matrix in the top left corner, anything in the top right corner, and zeroes in the bottom left and bottom right corner). 

By inspection, it is clear that the row rank and column rank of such a matrix are equal to each other and to the dimension of the identity matrix in the top left corner. 

In fact, elementary row operations do not even change the row space of the matrix. They clearly do change the column space of a matrix, but not the column rank as we shall now see. 

If A and B are row equivalent matrices, then the equations $\mathbf { A x } = \mathbf { 0 }$ and $\mathbf { B x } = \mathbf { 0 }$ have the same solution space. 

If a subset of columns of A are linearly dependent, then the solution space does contain a vector in which the corresponding entries are nonzero and all other entries are zero. 

Similarly, if a subset of columns of A are linearly independent, then the solution space does not contain a vector in which the corresponding entries are nonzero and all other entries are zero. 

The first result implies that the corresponding columns or B are also linearly dependent. 

The second result implies that the corresponding columns of B are also linearly independent. 

It follows that the dimension of the column space is the same for both matrices. 

Q.E.D. 

Definition 1.8.2 rank 

Definition 1.8.3 solution space, null space or kernel 

Theorem 1.8.2 dimension of row space + dimension of null space = number of columns 

The solution space of the system means the solution space of the homogenous equation $\mathbf { A x } = \mathbf { 0 }$ 

The non-homogenous equation Ax = b may or may not have solutions. 

System is consistent iff rhs is in column space of A and there is a solution. 

Such a solution is called a particular solution. 

A general solution is obtained by adding to some particular solution a generic element of the solution space. 

Previously, solving a system of linear equations was something we only did with non-singular square systems. 

Now, we can solve any system by describing the solution space. 

## 1.9 Eigenvalues and Eigenvectors

## Definition 1.9.1 eigenvalues and eigenvectors and λ-eigenspaces

Compute eigenvalues using det $( \mathbf { A } - \lambda \mathbf { I } ) = 0$ . So some matrices with real entries can have complex eigenvalues. 

Real symmetric matrix has real eigenvalues. Prove using complex conjugate argument. 

Given an eigenvalue, the corresponding eigenvector is the solution to a singular matrix equation, so one free parameter (at least). 

Often it is useful to specify unit eigenvectors. 

Eigenvectors of a real symmetric matrix corresponding to different eigenvalues are orthogonal (orthonormal if we normalise them). 

So we can diagonalize a symmetric matrix in the following sense: 

If the columns of P are orthonormal eigenvectors of A, and λ is the matrix with the corresponding eigenvalues along its leading diagonal, then $\mathbf { A P } = \mathbf { P } \boldsymbol { \lambda }$ so $\mathbf { P } ^ { - 1 } \mathbf { A } \mathbf { P } = \lambda = \mathbf { P } ^ { \top } \mathbf { A } \mathbf { P }$ as P is an orthogonal matrix. 

In fact, all we need to be able to diagonalise in this way is for A to have n linearly independent eigenvectors. 

P<sup>−1</sup>AP and A are said to be similar matrices. 

Two similar matrices share lots of properties: determinants and eigenvalues in particular. Easy to show this. 

But eigenvectors are different. 

## 1.10 Quadratic Forms

A quadratic form is 

## 1.11 Symmetric Matrices

Symmetric matrices have a number of special properties 

## 1.12 Definite Matrices

Definition 1.12.1 An $n \times n$ square matrix A is said to be 

$$
\begin{array}{r c l} \text {positive definite} & \Longleftrightarrow & \mathbf {x} ^ {\top} \mathbf {A} \mathbf {x} > 0   \forall \mathbf {x} \in \Re^ {n},   \mathbf {x} \neq \mathbf {0} \\ \text {positive semi - definite} & \Longleftrightarrow & \mathbf {x} ^ {\top} \mathbf {A} \mathbf {x} \geq 0   \forall \mathbf {x} \in \Re^ {n} \\ \text {negative definite} & \Longleftrightarrow & \mathbf {x} ^ {\top} \mathbf {A} \mathbf {x} <   0   \forall \mathbf {x} \in \Re^ {n},   \mathbf {x} \neq \mathbf {0} \\ \text {negative semi - definite} & \Longleftrightarrow & \mathbf {x} ^ {\top} \mathbf {A} \mathbf {x} \leq 0   \forall \mathbf {x} \in \Re^ {n} \end{array}
$$

Some texts may require that the matrix also be symmetric, but this is not essential and sometimes looking at the definiteness of non-symmetric matrices is relevant. If P is an invertible $n \times n$ square matrix and A is any $n \times n$ square matrix, then A is positive/negative (semi-)definite if and only if $\mathbf { P } ^ { - 1 } \mathbf { A P }$ is. 

In particular, the definiteness of a symmetric matrix can be determined by checking the signs of its eigenvalues. 

Other checks involve looking at the signs of the elements on the leading diagonal. Definite matrices are non-singular and singular matrices can not be definite. 

The commonest use of positive definite matrices is as the variance-covariance matrices of random variables. Since 

$$
v _ {i j} = \mathrm{Cov} [ \tilde {r} _ {i}, \tilde {r} _ {j} ] = \mathrm{Cov} [ \tilde {r} _ {j}, \tilde {r} _ {i} ]\tag{1.12.1}
$$

and 

$$
\mathbf {w} ^ {\top} \mathbf {V} \mathbf {w} = \sum_ {i = 1} ^ {N} \sum_ {j = 1} ^ {N} w _ {i} w _ {j} \operatorname{Cov} \left[ \tilde {r} _ {i}, \tilde {r} _ {j} \right]\tag{1.12.2}
$$

$$
{ = } { \operatorname{Cov} \left[ \sum _ { i = 1 } ^ { N } w _ { i } \tilde { r } _ { i } , \sum _ { j = 1 } ^ { N } w _ { j } \tilde { r } _ { j } \right] }\tag{1.12.3}
$$

$$
{ = } { \operatorname{Var} [ \sum _ { i = 1 } ^ { N } w _ { i } \tilde { r } _ { i } ] \geq 0 }\tag{1.12.4}
$$

a variance-covariance matrix must be real, symmetric and positive semi-definite. 

In Theorem 3.2.4, it will be seen that the definiteness of a matrix is also an essential idea in the theory of convex functions. 

We will also need later the fact that the inverse of a positive (negative) definite matrix (in particular, of a variance-covariance matrix) is positive (negative) definite. 

Semi-definite matrices which are not definite have a zero eigenvalue and therefore are singular. 

## Chapter 2

# VECTOR CALCULUS

## 2.1 Introduction

[To be written.] 

## 2.2 Basic Topology

The aim of this section is to provide sufficient introduction to topology to motivate the definitions of continuity of functions and correspondences in the next section, but no more. 

• A metric space is a non-empty set X equipped with a metric, i.e. a function $d : X \times X \to [ 0 , \infty )$ such that 

1. $d ( x , y ) = 0 \iff x = y .$ 

2. $d ( x , y ) = d ( y , x ) \forall x , y \in X .$ 

3. The triangular inequality: 

$$
d (x, z) + d (z, y) \geq d (x, y) \forall x, y, z \in X.
$$

• An open ball is a subset of a metric space, X, of the form 

$$
B \epsilon (x) = \{y \in X: d (y, x) <   \epsilon \}.
$$

• A subset A of a metric space is open 

$\forall x \in A , \exists \epsilon > 0$ such that $B \epsilon ( x ) \subseteq A$ 

2.3. VECTOR-VALUED FUNCTIONS AND FUNCTIONS OF SEVERAL 18 VARIABLES 

• A is closed $\iff X - A$ is open. (Note that many sets are neither open nor closed.) 

• A neighbourhood of $x \in X$ is an open set containing x. 

Definition 2.2.1 Let $X = \Re ^ { n } . ~ A \subseteq X$ is compact $\iff A$ is both closed and bounded (i.e. ∃x,  such that $A \subseteq B \epsilon ( \mathbf { x } ) ,$ ). 

We need to formally define the interior of a set before stating the separating theorem: 

Definition 2.2.2 If Z is a subset of a metric space X, then the interior of Z, denoted int Z, is defined by 

$$
z \in \operatorname{int} Z \iff B \epsilon (z) \subseteq Z \text {   for   some   } \epsilon > 0.
$$

## 2.3 Vector-valued Functions and Functions of Several Variables

Definition 2.3.1 A function (or map) $f : X \to Y$ from a domain X to a codomain Y is a rule which assigns to each element ofX a unique element ofY. 

Definition 2.3.2 A correspondence $f : X \to Y$ from a domain X to a co-domain Y is a rule which assigns to each element of X a non-empty subset of Y . 

Definition 2.3.3 The range ofthefunction $f : X \to Y$ is the set $f ( X ) = \{ f ( x ) \in$ $Y : x \in X \}$ 

Definition 2.3.4 Thefunction $f : X \to Y$ is injective (one-to-one) 

$$
f (x) = f \left(x ^ {\prime}\right) \Rightarrow x = x ^ {\prime}.
$$

Definition 2.3.5 Thefunction $f : X \to Y$ is surjective (onto) 

$$
\begin{array}{c} \Longleftrightarrow \\ f (X) = Y \end{array}
$$

Definition 2.3.6 Thefunction $f : X \to Y$ is bijective (or invertible) 

it is both injective and surjective. 

Revised: December 2, 1998 

Note that if $f \colon X \to Y$ and $A \subseteq X$ and $B \subseteq Y$ , then 

$$
f (A) \equiv \{f (x): x \in A \} \subseteq Y
$$

and 

$$
f ^ {- 1} (B) \equiv \{x \in X: f (x) \in B \} \subseteq X.
$$

Definition 2.3.7 A vector-valued function is afunction whose co-domain is a subset ofa vector space, say $\Re ^ { N }$ . Such afunction has N component functions. 

Definition 2.3.8 A function of several variables is a function whose domain is a subset ofa vector space. 

Definition 2.3.9 Thefunction $f \colon X \to Y ( X \subseteq \mathfrak { R } ^ { n } , Y \subseteq \mathfrak { R } )$ approaches the limit $y ^ { * } a s \mathbf { x } \longrightarrow \mathbf { x } ^ { * }$ 

$$
\forall \epsilon > 0, \exists \delta > 0 \text {s.t.} \| \mathbf {x} - \mathbf {x} ^ {*} \| <   \delta \Longrightarrow | f (\mathbf {x}) - \mathbf {y} ^ {*}) | <   \epsilon .
$$

This is usually denoted 

$$
\lim _ {\mathbf {x} \to \mathbf {x} ^ {*}} f (\mathbf {x}) = y ^ {*}.
$$

Definition 2.3.10 Thefunction f: $X \to Y ( X \subseteq { \mathfrak { R } } ^ { n } , Y \subseteq { \mathfrak { R } } )$ is continuous at $\mathbf { x } ^ { * }$ ⇐⇒ 

$$
\forall \epsilon > 0, \exists \delta > 0 \text {   s.t.   } \| \mathbf {x} - \mathbf {x} ^ {*} \| <   \delta \Longrightarrow | f (\mathbf {x}) - f (\mathbf {x} ^ {*}) | <   \epsilon .
$$

This definition just says that $f$ is continuous provided that 

$$
\lim _ {\mathbf {x} \to \mathbf {x} ^ {*}} f (\mathbf {x}) = f (\mathbf {x} ^ {*}).
$$

? discusses various alternative but equivalent definitions of continuity. 

Definition 2.3.11 Thefunction $f : X \to Y$ is continuous 

it is continuous at every point ofits domain. 

We will say that a vector-valued function is continuous if and only if each of its component functions is continuous. 

The notion of continuity of a function described above is probably familiar from earlier courses. Its extension to the notion of continuity of a correspondence, however, while fundamental to consumer theory, general equilibrium theory and much of microeconomics, is probably not. In particular, we will meet it again in Theorem 3.5.4. The interested reader is referred to ? for further details. 

Definition 2.3.12 1. The correspondence $f { \mathrm { : } } X \to Y ( X \subseteq \mathfrak { R } ^ { n } , Y \subseteq \mathfrak { R } )$ is upper hemi-continuous (u.h.c.) at x<sup>∗</sup> 

⇐⇒ 

for every open set N containing the set $f ( \mathbf { x } ^ { * } ) , \exists \delta > 0 s . t . \parallel \mathbf { x } - \mathbf { x } ^ { * } \parallel <$ $\delta \Longrightarrow f ( \mathbf { x } ) \subseteq N$ 

(Upper hemi-continuity basically means that the graph of the correspondence is a closed and connected set.) 

2. The correspondence $f \colon X \to Y ( X \subseteq \mathfrak { R } ^ { n } , Y \subseteq \mathfrak { R } )$ is lower hemi-continuous (l.h.c.) at x<sup>∗</sup> 

for every open set N intersecting the set $f ( \mathbf { x } ^ { * } ) , \exists \delta > 0 s . t . \parallel \mathbf { x } - \mathbf { x } ^ { * } \parallel <$ $\delta \Longrightarrow f ( \mathbf { x } )$ intersects N. 

3. The correspondence $f \colon X \to Y ( X \subseteq \mathfrak { R } ^ { n } , Y \subseteq \mathfrak { R } )$ is continuous (at x<sup>∗</sup>) ⇐⇒ 

it is both upper hemi-continuous and lower hemi-continuous (at x ) 

(There are a couple of pictures from ? to illustrate these definitions.) 

## 2.4 Partial and Total Derivatives

Definition 2.4.1 The (total) derivative or Jacobean ofa real-valuedfunction ofN variables is the N-dimensional row vector ofits partial derivatives. The Jacobean of a vector-valued function with values in <<sup>M</sup> is an M × N matrix of partial derivatives whose jth row is the Jacobean ofthe jth componentfunction. 

Definition 2.4.2 The gradient of a real-valuedfunction is the transpose of its Jacobean. 

Definition 2.4.3 Afunction is said to be differentiable at x ifall its partial derivatives exist at x. 

Definition 2.4.4 Thefunction $f : X \to Y$ is differentiable 

it is differentiable at every point ofits domain 

Definition 2.4.5 The Hessian matrix ofa real-valuedfunction is the (usually symmetric) square matrix ofits second order partial derivatives. 

Revised: December 2, 1998 

Note that if $f \colon { \mathfrak { R } } ^ { n }  { \mathfrak { R } }$ , then, strictly speaking, the second derivative (Hessian) of $f$ is the derivative of the vector-valued function 

$$
\left(f ^ {\prime}\right) ^ {\top}: \Re^ {n} \to \Re^ {n}: \mathbf {x} \mapsto \left(f ^ {\prime} (\mathbf {x})\right) ^ {\top}.
$$

Students always need to be warned about the differences in notation between the case of $n = 1$ and the case of $n > 1$ . Statements and shorthands that make sense in univariate calculus must be modified for multivariate calculus. 

## 2.5 The Chain Rule and Product Rule

Theorem 2.5.1 (The Chain Rule) Let $g \colon \mathfrak { R } ^ { n }  \mathfrak { R } ^ { m }$ and $f \colon \mathfrak { R } ^ { m }  \mathfrak { R } ^ { p }$ be continuously differentiablefunctions and let $h \colon \mathfrak { R } ^ { n } \to \mathfrak { R } ^ { p }$ be defined by 

$$
h \left(\mathbf {x}\right) \equiv f \left(g \left(\mathbf {x}\right)\right).
$$

Then 

$$
\underbrace {h ^ {\prime} \left(\mathbf {x}\right)} _ {p \times n} = \underbrace {f ^ {\prime} \left(g \left(\mathbf {x}\right)\right)} _ {p \times m} \underbrace {g ^ {\prime} \left(\mathbf {x}\right)} _ {m \times n}.
$$

Proof This is easily shown using the Chain Rule for partial derivatives. 

Q.E.D. 

One of the most common applications of the Chain Rule is the following: Let $g \colon \mathfrak { R } ^ { n }  \mathfrak { R } ^ { m }$ and $f \colon \Re ^ { m + n }  \Re ^ { p }$ be continuously differentiable functions, let $\mathbf { x } \in \Re ^ { n }$ , and define $h \colon \mathfrak { R } ^ { n } \to \mathfrak { R } ^ { p }$ by: 

$$
h (\mathbf {x}) \equiv f (g (\mathbf {x}), \mathbf {x}).
$$

The univariate Chain Rule can then be used to calculate $\begin{array} { r } { \frac { { \partial { h ^ { i } } } } { { \partial { x _ { j } } } } \left( { \bf { x } } \right) } \end{array}$ in terms of partial derivatives of $f$ and $g$ for $i = 1 , \ldots , p$ and $j = 1 , \dots , n \colon$ 

$$
\frac {\partial h ^ {i}}{\partial x _ {j}} (\mathbf {x}) = \sum_ {k = 1} ^ {m} \frac {\partial f ^ {i}}{\partial x _ {k}} (g (\mathbf {x}), \mathbf {x}) \frac {\partial g ^ {k}}{\partial x _ {j}} (\mathbf {x}) + \sum_ {k = m + 1} ^ {m + n} \frac {\partial f ^ {i}}{\partial x _ {k}} (g (\mathbf {x}), \mathbf {x}) \frac {\partial x ^ {k}}{\partial x _ {j}} (\mathbf {x}).\tag{2.5.1}
$$

Note that 

$$
\frac {\partial x ^ {k}}{\partial x _ {j}} \left(\mathbf {x}\right) = \delta_ {j} ^ {k} \equiv \left\{ \begin{array}{l l} 1 & \text { if } k = j \\ 0 & \text { otherwise } \end{array} \right.,
$$

which is known as the Kronecker Delta. Thus all but one of the terms in the second summation in (2.5.1) vanishes, giving: 

$$
\frac {\partial h ^ {i}}{\partial x _ {j}} (\mathbf {x}) = \sum_ {k = 1} ^ {m} \frac {\partial f ^ {i}}{\partial x _ {k}} (g (\mathbf {x}), \mathbf {x}) \frac {\partial g ^ {k}}{\partial x _ {j}} (\mathbf {x}) + \frac {\partial f ^ {i}}{\partial x _ {j}} (g (\mathbf {x}), \mathbf {x}).
$$

Stacking these scalar equations in matrix form and factoring yields: 

$$
\begin{array}{l} \left( \begin{array}{c c c} \frac {\partial h ^ {1}}{\partial x _ {1}} (\mathbf {x}) & \dots & \frac {\partial h ^ {1}}{\partial x _ {n}} (\mathbf {x}) \\ \vdots & \ddots & \vdots \\ \frac {\partial h ^ {p}}{\partial x _ {1}} (\mathbf {x}) & \dots & \frac {\partial h ^ {p}}{\partial x _ {n}} (\mathbf {x}) \end{array} \right) = \\ \left( \begin{array}{c c c} \frac {\partial f ^ {1}}{\partial x _ {1}} (g (\mathbf {x}), \mathbf {x}) & \dots & \frac {\partial f ^ {1}}{\partial x _ {m}} (g (\mathbf {x}), \mathbf {x}) \\ \vdots & \ddots & \vdots \\ \frac {\partial f ^ {p}}{\partial x _ {1}} (g (\mathbf {x}), \mathbf {x}) & \dots & \frac {\partial f ^ {p}}{\partial x _ {m}} (g (\mathbf {x}), \mathbf {x}) \end{array} \right) \left( \begin{array}{c c c} \frac {\partial g ^ {1}}{\partial x _ {1}} (\mathbf {x}) & \dots & \frac {\partial g ^ {1}}{\partial x _ {n}} (\mathbf {x}) \\ \vdots & \ddots & \vdots \\ \frac {\partial g ^ {m}}{\partial x _ {1}} (\mathbf {x}) & \dots & \frac {\partial g ^ {m}}{\partial x _ {n}} (\mathbf {x}) \end{array} \right) \\ + \left( \begin{array}{c c c} \frac {\partial f ^ {1}}{\partial x _ {m + 1}} (g (\mathbf {x}), \mathbf {x}) & \dots & \frac {\partial f ^ {1}}{\partial x _ {m + n}} (g (\mathbf {x}), \mathbf {x}) \\ \vdots & \ddots & \vdots \\ \frac {\partial f ^ {p}}{\partial x _ {m + 1}} (g (\mathbf {x}), \mathbf {x}) & \dots & \frac {\partial f ^ {p}}{\partial x _ {m + n}} (g (\mathbf {x}), \mathbf {x}) \end{array} \right). \end{array} \tag {2.}\tag{2.5.2}
$$

Now, by partitioning the total derivative of $f$ as 

$$
\underbrace {f ^ {\prime} (\cdot)} _ {p \times (m + n)} = \left[ \underbrace {D _ {\mathbf {g}} f (\cdot)} _ {p \times m} \quad \underbrace {D _ {\mathbf {x}} f (\cdot)} _ {p \times n} \right],\tag{2.5.3}
$$

we can use (2.5.2) to write out the total derivative $h ^ { \prime } \left( \mathbf { x } \right)$ as a product of partitioned matrices: 

$$
h ^ {\prime} (\mathbf {x}) = D _ {\mathbf {g}} f (g (\mathbf {x}), \mathbf {x}) g ^ {\prime} (\mathbf {x}) + D _ {\mathbf {x}} f (g (\mathbf {x}), \mathbf {x}).\tag{2.5.4}
$$

Theorem 2.5.2 (Product Rule for Vector Calculus) The multivariate Product Rule comes in two versions: 

1. Let $f , g \colon \mathfrak { R } ^ { m }  \mathfrak { R } ^ { n }$ and define h: $\Re ^ { m }  \Re$ by 

$$
\underbrace {h \left(\mathbf {x}\right)} _ {1 \times 1} \equiv \underbrace {\left(f \left(\mathbf {x}\right)\right) ^ {\top}} _ {1 \times n} \underbrace {g \left(\mathbf {x}\right)} _ {n \times 1}.
$$

Then 

$$
\underbrace {h ^ {\prime} (\mathbf {x})} _ {1 \times m} = \underbrace {(g (\mathbf {x})) ^ {\top}} _ {1 \times n} \underbrace {f ^ {\prime} (\mathbf {x})} _ {n \times m} + \underbrace {(f (\mathbf {x})) ^ {\top}} _ {1 \times n} \underbrace {g ^ {\prime} (\mathbf {x})} _ {n \times m}.
$$

2. Let $f \colon \mathfrak { R } ^ { m }  \mathfrak { R }$ and $g \colon { \mathfrak { R } } ^ { m }  { \mathfrak { R } } ^ { n }$ and define $h \colon \mathfrak { R } ^ { m } \to \mathfrak { R } ^ { n }$ by 

$$
\underbrace {h \left(\mathbf {x}\right)} _ {n \times 1} \equiv \underbrace {f \left(\mathbf {x}\right)} _ {1 \times 1} \underbrace {g \left(\mathbf {x}\right)} _ {n \times 1}.
$$

Then 

$$
\underbrace {h ^ {\prime} (\mathbf {x})} _ {n \times m} = \underbrace {g (\mathbf {x})} _ {n \times 1} \underbrace {f ^ {\prime} (\mathbf {x})} _ {1 \times m} + \underbrace {f (\mathbf {x})} _ {1 \times 1} \underbrace {g ^ {\prime} (\mathbf {x})} _ {n \times m}.
$$

Proof This is easily shown using the Product Rule from univariate calculus to calculate the relevant partial derivatives and then stacking the results in matrix form. Q.E.D. 

Revised: December 2, 1998 

## 2.6 The Implicit Function Theorem

Theorem 2.6.1 (Implicit Function Theorem) Let $g \colon \mathfrak { R } ^ { n }  \mathfrak { R } ^ { m }$ , where $m < n$ Consider the system ofm scalar equations in n variables, $g \left( \mathbf { x } ^ { * } \right) = \mathbf { 0 } _ { m } .$ 

Partition the n-dimensional vector x as $\displaystyle ( \mathbf { y } , \mathbf { z } )$ where $\mathbf { y } = \left( x _ { 1 } , x _ { 2 } , \ldots , x _ { m } \right)$ is mdimensional and $\mathbf { z } = ( x _ { m + 1 } , x _ { m + 2 } , \ldots , x _ { n } )$ is $( n - m )$ -dimensional. Similarly, partition the total derivative of g at $\mathbf { x } ^ { * }$ as 

$$
\begin{array}{r l r} {g ^ {\prime} \left(\mathbf {x} ^ {*}\right)} & = & {\left[ D _ {\mathbf {y}} g \right. \qquad \left. D _ {\mathbf {z}} g \right]} \\ {(m \times n)} & & {(m \times m) \quad (m \times (n - m))} \end{array}\tag{2.6.1}
$$

We aim to solve these equations for the first m variables, $\mathbf { y } ,$ which will then be written asfunctions, $h \left( \mathbf { z } \right)$ ofthe last $n - m$ variables, z. 

Suppose g is continuously differentiable in a neighbourhood of $\mathbf { x } ^ { * }$ , and that the m × m matrix: 

$$
D _ {\mathbf {y}} g \equiv \left( \begin{array}{c c c} \frac {\partial g ^ {1}}{\partial x _ {1}} \left(\mathbf {x} ^ {*}\right) & \ldots & \frac {\partial g ^ {1}}{\partial x _ {m}} \left(\mathbf {x} ^ {*}\right) \\ \vdots & \ddots & \vdots \\ \frac {\partial g ^ {m}}{\partial x _ {1}} \left(\mathbf {x} ^ {*}\right) & \ldots & \frac {\partial g ^ {m}}{\partial x _ {m}} \left(\mathbf {x} ^ {*}\right) \end{array} \right)
$$

formed by thefirst m columns ofthe total derivative ofg at $\mathbf { x } ^ { * }$ is non-singular. Then $\exists$ neighbourhoods Y of $\mathbf { y } ^ { * }$ and Z of $\mathbf { z } ^ { \ast }$ , and a continuously differentiable function $h \colon Z \to Y$ such that 

1. $\mathbf { y } ^ { * } = h \left( \mathbf { z } ^ { * } \right)$ 

2. $g \left( h \left( \mathbf { z } \right) , \mathbf { z } \right) = \mathbf { 0 } \quad \forall \mathbf { z } \in Z , a n d$ 

$$
3. h ^ {\prime} (\mathbf {z} ^ {*}) = - (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}} g.
$$

Proof The full proof of this theorem, like that of Brouwer’s Fixed Point Theorem later, is beyond the scope of this course. However, part 3 follows easily from material in Section 2.5. The aim is to derive an expression for the total derivative $h ^ { \prime } \left( \mathbf { z } ^ { * } \right)$ in terms of the partial derivatives of $g ,$ , using the Chain Rule. 

We know from part 2 that 

$$
f (\mathbf {z}) \equiv g (h (\mathbf {z}), \mathbf {z}) = \mathbf {0} _ {m} \quad \forall \mathbf {z} \in Z.
$$

Thus 

$$
f ^ {\prime} (\mathbf {z}) \equiv \mathbf {0} _ {m \times (n - m)} \quad \forall \mathbf {z} \in Z,
$$

in particular at $\mathbf { z } ^ { \ast }$ . But we know from (2.5.4) that 

$$
f ^ {\prime} (\mathbf {z}) = D _ {\mathbf {y}} g h ^ {\prime} (\mathbf {z}) + D _ {\mathbf {z}} g.
$$

Revised: December 2, 1998 

Hence 

$$
D _ {\mathbf {y}} g h ^ {\prime} (\mathbf {z}) + D _ {\mathbf {z}} g = \mathbf {0} _ {m \times (n - m)}
$$

and, since the statement of the theorem requires that $D _ { \mathbf { y } } g$ is invertible, 

$$
h ^ {\prime} (\mathbf {z} ^ {*}) = - (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}} g,
$$

as required. 

Q.E.D. 

To conclude this section, consider the following two examples: 

1. the equation $g \left( x , y \right) \equiv x ^ { 2 } + y ^ { 2 } - 1 = 0 .$ 

Note that $g ^ { \prime } \left( x , y \right) = \left( 2 x 2 y \right)$ 

We have $h ( y ) = { \sqrt { 1 - y ^ { 2 } } } \operatorname { o r } h ( y ) = - { \sqrt { 1 - y ^ { 2 } } }$ , each of which describes a single-valued, differentiable function on $( - 1 , 1 )$ . At $\begin{array} { r } { ( x , y ) = ( 0 , 1 ) , \frac { \partial g } { \partial x } = } \end{array}$ 0 and $h ( y )$ is undefined (for $y > 1 )$ or multi-valued (for $y \textless 1 )$ in any neighbourhood of $y = 1$ 

2. the system of linear equations $g \left( \mathbf { x } \right) \equiv \mathbf { B x } = \mathbf { 0 }$ , where B is an $m \times n$ matrix. 

We have $g ^ { \prime } \left( \mathbf { x } \right) = \mathbf { B } \quad \forall \mathbf { x }$ so the implicit function theorem applies provided the equations are linearly independent. 

## 2.7 Directional Derivatives

Definition 2.7.1 Let X be a vector space and $\mathbf { x } \neq \mathbf { x } ^ { \prime } \in X$ . Then 

1. for $\lambda \in { \mathfrak { R } }$ and particularlyfor $\lambda \in [ 0 , 1 ] , \lambda \mathbf { x } + ( 1 - \lambda ) \mathbf { x } ^ { \prime }$ is called a convex combination ofx and $\mathbf { x } ^ { \prime }$ . 

2. $L = \{ \lambda \mathbf { x } + ( 1 - \lambda ) \mathbf { x } ^ { \prime } : \lambda \in \mathfrak { R } \}$ is the line from $\mathbf { x } ^ { \prime }$ , where $\lambda = 0$ , to $\mathbf { x } ,$ where $\lambda = 1 .$ , in X. 

3. The restriction of the function $f \colon X  \Re$ to the line L is thefunction 

$$
f | _ {L} \colon \Re \to \Re \colon \lambda \mapsto f (\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}).
$$

4. $_ { I f f }$ is a differentiable function, then the directional derivative of $f$ at $\mathbf { x } ^ { \prime }$ in the direction from $\mathbf { x } ^ { \prime }$ to x is $f | _ { L } ^ { \prime } \left( 0 \right)$ 

• We will endeavour, wherever possible, to stick to the convention that $\mathbf { x } ^ { \prime }$ denotes the point at which the derivative is to be evaluated and x denotes the point in the direction of which it is measured.<sup>1</sup> 

• Note that, by the Chain Rule, 

$$
f | _ {L} ^ {\prime} (\lambda) = f ^ {\prime} (\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}) (\mathbf {x} - \mathbf {x} ^ {\prime})\tag{2.7.1}
$$

and hence the directional derivative 

$$
f | _ {L} ^ {\prime} (0) = f ^ {\prime} (\mathbf {x} ^ {\prime}) (\mathbf {x} - \mathbf {x} ^ {\prime}).\tag{2.7.2}
$$

• The ith partial derivative of $f$ at x is the directional derivative of $f$ at $\mathbf { x }$ in the direction from x to $\mathbf { x } + \mathbf { e } _ { i }$ , where $\mathbf { e } _ { i }$ is the ith standard basis vector. In other words, partial derivatives are a special case of directional derivatives or directional derivatives a generalisation of partial derivatives. 

• As an exercise, consider the interpretation of the directional derivatives at a point in terms of the rescaling of the parameterisation of the line $L .$ 

• Note also that, returning to first principles, 

$$
f | _ {L} ^ {\prime} (0) = \lim _ {\lambda \to 0} \frac {f (\mathbf {x} ^ {\prime} + \lambda (\mathbf {x} - \mathbf {x} ^ {\prime})) - f (\mathbf {x} ^ {\prime})}{\lambda}.\tag{2.7.3}
$$

• Sometimes it is neater to write ${ \bf x } - { \bf x } ^ { \prime } \equiv { \bf h }$ . Using the Chain Rule, it is easily shown that the second derivative of $f | _ { L }$ is 

$$
f | _ {L} ^ {\prime \prime} (\lambda) = \mathbf {h} ^ {\top} f ^ {\prime \prime} (\mathbf {x} ^ {\prime} + \lambda \mathbf {h}) \mathbf {h}
$$

and 

$$
f | _ {L} ^ {\prime \prime} (0) = \mathbf {h} ^ {\top} f ^ {\prime \prime} (\mathbf {x} ^ {\prime}) \mathbf {h}.
$$

## 2.8 Taylor’s Theorem: Deterministic Version

This should be fleshed out following ?. 

Readers are presumed to be familiar with single variable versions of Taylor’s Theorem. In particular recall both the second order exact and infinite versions. 

An interesting example is to approximate the discount factor using powers of the interest rate: 1 

$$
{\frac {1}{1 + i}} = 1 - i + i ^ {2} - i ^ {3} + i ^ {4} + \ldots\tag{2.8.1}
$$

We will also use two multivariate versions of Taylor’s theorem which can be obtained by applying the univariate versions to the restriction to a line of a function of n variables. 

Theorem 2.8.1 (Taylor’s Theorem) Let $f : X  \Re$ be twice differentiable, $X \subseteq \Re ^ { n }$ . Then for any x, $\mathbf { x } ^ { \prime } \in X , \exists \lambda \in ( 0 , 1 )$ such that 

$$
f (\mathbf {x}) = f \left(\mathbf {x} ^ {\prime}\right) + f ^ {\prime} \left(\mathbf {x} ^ {\prime}\right) \left(\mathbf {x} - \mathbf {x} ^ {\prime}\right) + \frac {1}{2} \left(\mathbf {x} - \mathbf {x} ^ {\prime}\right) ^ {\top} f ^ {\prime \prime} \left(\mathbf {x} ^ {\prime} + \lambda \left(\mathbf {x} - \mathbf {x} ^ {\prime}\right)\right) \left(\mathbf {x} - \mathbf {x} ^ {\prime}\right).\tag{2.8.2}
$$

Proof Let L be the line from $\mathbf { x } ^ { \prime }$ to x. 

Then the univariate version tells us that there exists $\lambda \in ( 0 , 1 ) ^ { 2 }$ such that 

$$
f | _ {L} (1) = f | _ {L} (0) + f | _ {L} ^ {\prime} (0) + \frac {1}{2} f | _ {L} ^ {\prime \prime} (\lambda).\tag{2.8.3}
$$

Making the appropriate substitutions gives the multivariate version in the theorem. 

Q.E.D. 

The (infinite) Taylor series expansion does not necessarily converge at all, or to $f ( x )$ . Functions for which it does are called analytic. ? is an example of a function which is not analytic. 

## 2.9 The Fundamental Theorem of Calculus

This theorem sets out the precise rules for cancelling integration and differentiation operations. 

Theorem 2.9.1 (Fundamental Theorem of Calculus) The integration and differentiation operators are inverses in thefollowing senses: 

1. 

$$
{\frac {d}{d b}} \int_ {a} ^ {b} f (x) d x = f (b)
$$

2. 

$$
\int_ {a} ^ {b} f ^ {\prime} (x) d x = f (b) - f (a)
$$

This can be illustrated graphically using a picture illustrating the use of integration to compute the area under a curve. 

## Chapter 3

# CONVEXITY AND OPTIMISATION

## 3.1 Introduction

[To be written.] 

## 3.2 Convexity and Concavity

## 3.2.1 Definitions

Definition 3.2.1 A subset X ofa vector space is a convex set ⇐⇒ 

$$
\forall \mathbf {x}, \mathbf {x} ^ {\prime} \in X, \lambda \in [ 0, 1 ], \lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime} \in X.
$$

Theorem 3.2.1 A sum ofconvex sets, such as 

$$
X + Y \equiv \left\{\mathbf {x} + \mathbf {y}: \mathbf {x} \in X, \mathbf {y} \in Y \right\},
$$

is also a convex set. 

Proof The proof of this result is left as an exercise. 

Q.E.D. 

Definition 3.2.2 Let $f : X \to Y$ where X is a convex subset of a real vector space and $Y \subseteq \Re$ <. Then 

Revised: December 2, 1998 

1. f is a convex function 

$$
\begin{array}{r l} & \Longleftrightarrow \\ & \forall \mathbf {x} \neq \mathbf {x} ^ {\prime} \in X, \lambda \in (0, 1) \\ & f (\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}) \leq \lambda f (\mathbf {x}) + (1 - \lambda) f (\mathbf {x} ^ {\prime}). \end{array}\tag{3.2.1}
$$

(This just says that afunction ofseveral variables is convex ifits restriction to every line segment in its domain is a convex function of one variable in thefamiliar sense.) 

2. f is a concave function 

$$
\begin{array}{r l} & {\Longleftrightarrow} \\ & {\forall \mathbf {x} \neq \mathbf {x} ^ {\prime} \in X, \lambda \in (0, 1)} \\ & {\qquad f (\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}) \geq \lambda f (\mathbf {x}) + (1 - \lambda) f (\mathbf {x} ^ {\prime}).} \end{array}\tag{3.2.2}
$$

3. f is affine 

f is both convex and concave.<sup>1</sup> 

Note that the conditions (3.2.1) and (3.2.2) could also have been required to hold (equivalently) 

$$
\forall \mathbf {x}, \mathbf {x} ^ {\prime} \in X, \lambda \in [ 0, 1 ]
$$

since they are satisfied as equalities ∀f when $\mathbf { x } \ = \ \mathbf { x } ^ { \prime }$ , when $\lambda = 0$ and when $\lambda = 1$ 

Note that f is convex $\iff - f$ is concave. 

Definition 3.2.3 Again let $f : X \to Y$ where X is a convex subset ofa real vector space and $Y \subseteq \Re .$ . Then 

1. f is a strictly convex function 

$$
\forall \mathbf {x} \neq \mathbf {x} ^ {\prime} \in X, \lambda \in (0, 1)
$$

$$
f \left(\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}\right) <   \lambda f (\mathbf {x}) + (1 - \lambda) f (\mathbf {x} ^ {\prime}).
$$

2. f is a strictly concave function 

$$
\begin{array}{r l} & \Longleftrightarrow \\ & \forall \mathbf {x} \neq \mathbf {x} ^ {\prime} \in X, \lambda \in (0, 1) \\ & f (\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}) > \lambda f (\mathbf {x}) + (1 - \lambda) f (\mathbf {x} ^ {\prime}). \end{array}
$$

Note that there is no longer any flexibility as regards allowing $\mathbf { x } = \mathbf { x } ^ { \prime } \mathbf { o r } \lambda = 0$ or $\lambda = 1$ in these definitions. 

## 3.2.2 Properties of concave functions

Note the connection between convexity of a function of several variables and convexity of the restrictions of that function to any line in its domain: the former is convex if and only if all the latter are. 

Note that a function on a multidimensional vector space, X, is convex if and only if the restriction of the function to the line L is convex for every line L in X, and similarly for concave, strictly convex, and strictly concave functions. 

Since every convex function is the mirror image of a concave function, and vice versa, every result derived for one has an obvious corollary for the other. In general, we will consider only concave functions, and leave the derivation of the corollaries for convex functions as exercises. 

Let $f : X  \Re$ and $g : X  \Re$ be concave functions. Then 

1. If $a , b > 0$ , then $a f + b g$ is concave. 

2. If $a < 0 .$ , then af is convex. 

3. min $\{ f , g \}$ is concave 

The proofs of the above properties are left as exercises. 

Definition 3.2.4 Consider the real-valuedfunction $f \colon X \to Y$ where $Y \subseteq \Re .$ 

1. The upper contour sets off are the sets $\{ \mathbf { x } \in X : f ( \mathbf { x } ) \geq \alpha \} \left( \alpha \in { \mathfrak { R } } \right)$ 

2. The level sets or indifference curves of f are the sets $\{ \mathbf { x } \in X : f ( \mathbf { x } ) = \alpha \}$ $( \alpha \in { \mathfrak { R } } )$ 

3. The lower contour sets off are the sets $\left\{ \mathbf { x } \in X : f ( \mathbf { x } ) \leq \alpha \right\} ( \alpha \in { \mathfrak { R } } )$ 

In Definition 3.2.4, X does not have to be a (real) vector space. 

Theorem 3.2.2 The upper contour sets $\{ \mathbf { x } \ \in \ { \cal { X } } \ : \ f ( \mathbf { x } ) \ \geq \ \alpha \}$ of a concave function are convex. 

Proof This proof is probably in a problem set somewhere. 

Q.E.D. 

Consider as an aside the two-good consumer problem. Note in particular the implications of Theorem 3.2.2 for the shape of the indifference curves corresponding to a concave utility function. Concave u is a sufficient but not a necessary condition for convex upper contour sets. 

## 3.2.3 Convexity and differentiability

In this section, we show that there are a total of three ways of characterising concave functions, namely the definition above, a theorem in terms of the first derivative (Theorem 3.2.3) and a theorem in terms of the second derivative or Hessian (Theorem 3.2.4). 

Theorem 3.2.3 [Convexity criterion for differentiable functions.] Let $f : X  \Re$ be differentiable, $X \subseteq \Re ^ { n }$ an open, convex set. Then: 

f is (strictly) concave 

$$
\forall \mathbf {x} \neq \mathbf {x} ^ {\prime} \in X,
$$

$$
f (\mathbf {x}) \leq (<  ) f \left(\mathbf {x} ^ {\prime}\right) + f ^ {\prime} \left(\mathbf {x} ^ {\prime}\right) \left(\mathbf {x} - \mathbf {x} ^ {\prime}\right).\tag{3.2.3}
$$

Theorem 3.2.3 says that a function is concave if and only if the tangent hyperplane at any point lies completely above the graph of the function, or that a function is concave if and only if for any two distinct points in the domain, the directional derivative at one point in the direction of the other exceeds the jump in the value of the function between the two points. (See Section 2.7 for the definition of a directional derivative.) 

Proof (See ?.) 

1. We first prove that the weak version of inequality 3.2.3 is necessary for concavity, and then that the strict version is necessary for strict concavity. 

Choose x, $\mathbf { x } ^ { \prime } \in X$ 

Revised: December 2, 1998 

(a) Suppose that $f$ is concave. 

Then, for $\lambda \in ( 0 , 1 )$ 

$$
f \left(\mathbf {x} ^ {\prime} + \lambda (\mathbf {x} - \mathbf {x} ^ {\prime})\right) \geq f (\mathbf {x} ^ {\prime}) + \lambda \left(f (\mathbf {x}) - f (\mathbf {x} ^ {\prime})\right).\tag{3.2.4}
$$

Subtract $f ( \mathbf { x } ^ { \prime } )$ from both sides and divide by λ: 

$$
\frac {f (\mathbf {x} ^ {\prime} + \lambda (\mathbf {x} - \mathbf {x} ^ {\prime})) - f (\mathbf {x} ^ {\prime})}{\lambda} \geq f (\mathbf {x}) - f (\mathbf {x} ^ {\prime}).\tag{3.2.5}
$$

Now consider the limits of both sides of this inequality as $\lambda \ \to \ 0$ The LHS tends to $f ^ { \prime } \left( \mathbf { x } ^ { \prime } \right) \left( \mathbf { x } - \mathbf { x } ^ { \prime } \right)$ by definition of a directional derivative (see (2.7.2) and (2.7.3) above). The RHS is independent of λ and does not change. The result now follows easily for concave functions. However, 3.2.5 remains a weak inequality even if f is a strictly concave function. 

(b) Now suppose that $f$ is strictly concave and $\mathbf { x } \neq \mathbf { x } ^ { \prime } .$ 

Since $f$ is also concave, we can apply the result that we have just proved to $\mathbf { x } ^ { \prime }$ and $\mathbf { x } ^ { \prime \prime } \equiv \frac { 1 } { 2 } \left( \mathbf { x } + \mathbf { x } ^ { \prime } \right)$ to show that 

$$
f ^ {\prime} (\mathbf {x} ^ {\prime}) (\mathbf {x} ^ {\prime \prime} - \mathbf {x} ^ {\prime}) \geq f (\mathbf {x} ^ {\prime \prime}) - f (\mathbf {x} ^ {\prime}).\tag{3.2.6}
$$

Using the definition of strict concavity (or the strict version of inequality (3.2.4)) gives: 

$$
f (\mathbf {x} ^ {\prime \prime}) - f (\mathbf {x} ^ {\prime}) > \frac {1}{2} \left(f (\mathbf {x}) - f (\mathbf {x} ^ {\prime})\right).\tag{3.2.7}
$$

Combining these two inequalities and multiplying across by 2 gives the desired result. 

2. Conversely, suppose that the derivative satisfies inequality (3.2.3). We will deal with concavity. To prove the theorem for strict concavity, just replace all the weak inequalities $( \geq )$ with strict inequalities $( > )$ , as indicated. 

Set $\mathbf { x } ^ { \prime } = \lambda \mathbf { x } + ( 1 - \lambda ) \mathbf { x } ^ { \prime \prime }$ . Then, applying the hypothesis of the proof in turn to x and $\mathbf { x } ^ { \prime }$ and to $\mathbf { x } ^ { \prime \prime }$ and $\mathbf { x } ^ { \prime }$ yields: 

$$
f (\mathbf {x}) \leq f (\mathbf {x} ^ {\prime}) + f ^ {\prime} (\mathbf {x} ^ {\prime}) (\mathbf {x} - \mathbf {x} ^ {\prime})
$$

(3.2.8) 

and 

$$
f (\mathbf {x} ^ {\prime \prime}) \leq f (\mathbf {x} ^ {\prime}) + f ^ {\prime} (\mathbf {x} ^ {\prime}) (\mathbf {x} ^ {\prime \prime} - \mathbf {x} ^ {\prime})\tag{3.2.9}
$$

A convex combination of (3.2.8) and (3.2.9) gives: 

$$
\lambda f (\mathbf {x}) + (1 - \lambda) f (\mathbf {x} ^ {\prime \prime})
$$

$$
\begin{array}{l l} \leq & f (\mathbf {x} ^ {\prime}) + f ^ {\prime} (\mathbf {x} ^ {\prime}) \left(\lambda \left((\mathbf {x} - \mathbf {x} ^ {\prime})\right) + (1 - \lambda) \left((\mathbf {x} ^ {\prime \prime} - \mathbf {x} ^ {\prime})\right)\right) \\ = & f (\mathbf {x} ^ {\prime}), \end{array}\tag{3.2.10}
$$

since 

$$
\lambda \left(\left(\mathbf {x} - \mathbf {x} ^ {\prime}\right)\right) + (1 - \lambda) \left(\left(\mathbf {x} ^ {\prime \prime} - \mathbf {x} ^ {\prime}\right)\right) = \lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime \prime} - \mathbf {x} ^ {\prime} = \mathbf {0} _ {n}.\tag{3.2.11}
$$

(3.2.10) is just the definition of concavity as required. 

Q.E.D. 

Theorem 3.2.4 [Concavity criterion for twice differentiable functions.] Let $f$ : $X \  \ \Re$ be twice continuously differentiable $( C ^ { 2 } ) , X \subseteq \mathfrak { R } ^ { n }$ open and convex. Then: 

1. f is concave 

⇐⇒ 

$\forall \mathbf { x } \in X$ , the Hessian matrix $f ^ { \prime \prime } ( \mathbf { x } )$ is negative semidefinite. 

2. $f ^ { \prime \prime } ( \mathbf { x } )$ negative definite $\forall \mathbf { x } \in X$ 

$f$ is strictly concave. 

The fact that the condition in the second part of this theorem is sufficient but not necessary for concavity inspires the search for a counter-example, in other words for a function which is strictly concave but has a second derivative which is only negative semi-definite and not strictly negative definite. The standard counterexample is given by $f ( x ) = x ^ { 2 n }$ for any integer $n > 1$ 

Proof We first use Taylor’s theorem to demonstrate the sufficiency of the condition on the Hessian matrices. Then we use the Fundamental Theorem of Calculus (Theorem 2.9.1) and a proof by contrapositive to demonstrate the necessity of this condition in the concave case for $n = 1$ . Then we use this result and the Chain Rule to demonstrate necessity for $n > 1$ . Finally, we show how these arguments can be modified to give an alternative proof of sufficiency for functions of one variable. 

1. Suppose first that $f ^ { \prime \prime } ( \mathbf { x } )$ is negative semi-definite $\forall \mathbf { x } \in X$ . Recall Taylor’s Theorem above (Theorem 2.8.1). 

It follows that $f ( \mathbf { x } ) \leq f ( \mathbf { x } ^ { \prime } ) + f ^ { \prime } ( \mathbf { x } ^ { \prime } ) ( \mathbf { x } - \mathbf { x } ^ { \prime } )$ . Theorem 3.2.3 shows that $f$ is then concave. A similar proof will work for negative definite Hessian and strictly concave function. 

2. To demonstrate necessity, we must consider separately first functions of a single variable and then functions of several variables. 

(a) First consider a function of a single variable. Instead of trying to show that concavity of $f$ implies a negative semi-definite (i.e. non-positive) second derivative $\forall x \in X$ , we will prove the contrapositive. In other words, we will show that if there is any point $x ^ { * } \in X$ where the second derivative is positive, then $f$ is locally strictly convex around $x ^ { * }$ and so cannot be concave. 

So suppose $f ^ { \prime \prime } ( x ^ { * } ) > 0$ . Then, since f is twice continuously differentiable, $f ^ { \prime \prime } ( x ) > 0$ for all x in some neighbourhood of $x ^ { * }$ , say $( a , b )$ Then $f ^ { \prime }$ is an increasing function on $( a , b )$ . Consider two points in $( a , b ) , x < x ^ { \prime \prime }$ and let $x ^ { \prime } = \lambda x + ( 1 - \lambda ) x ^ { \prime \prime } \in X$ , where $\lambda \in ( 0 , 1 )$ Using the fundamental theorem of calculus, 

$$
f (x ^ {\prime}) - f (x) = \int_ {x} ^ {x ^ {\prime}} f ^ {\prime} (t) d t <   f ^ {\prime} (x ^ {\prime}) (x ^ {\prime} - x)
$$

and 

$$
f (x ^ {\prime \prime}) - f (x ^ {\prime}) = \int_ {x ^ {\prime}} ^ {x ^ {\prime \prime}} f ^ {\prime} (t) d t <   f ^ {\prime} (x ^ {\prime}) (x ^ {\prime \prime} - x ^ {\prime}).
$$

Rearranging each inequality gives: 

$$
f (x) > f \left(x ^ {\prime}\right) + f ^ {\prime} \left(x ^ {\prime}\right) \left(x - x ^ {\prime}\right)
$$

and 

$$
f (x ^ {\prime \prime}) > f (x ^ {\prime}) + f ^ {\prime} (x ^ {\prime}) (x ^ {\prime \prime} - x ^ {\prime}),
$$

which are just the single variable versions of (3.2.8) and (3.2.9). As in the proof of Theorem 3.2.3, a convex combination of these inequalities reduces to 

$$
f (x ^ {\prime}) <   \lambda f (x) + (1 - \lambda) f (x ^ {\prime \prime}),
$$

and hence $f$ is locally strictly convex on $( a , b )$ 

(b) Now consider a function of several variables. Suppose that f is concave and fix $\mathbf x \in X$ and $\mathbf { h } \in \Re ^ { n }$ . (We use an x, x+h argument instead of an $\mathbf { x } , \mathbf { x } ^ { \prime }$ argument to tie in with the definition of a negative definite matrix.) Then, at least for sufficiently small λ, $g ( \lambda ) \equiv f ( { \bf x } + \lambda { \bf h } )$ also defines a concave function (of one variable), namely the restriction of $f$ to the line segment from x in the direction from $\textbf { x t o x } + \textbf { h }$ . Thus, using the result we have just proven for functions of one variable, $g$ has non-positive second derivative. But we know from p. 25 above that $g ^ { \prime \prime } ( 0 ) = \mathbf { h } ^ { \top } f ^ { \prime \prime } ( \mathbf { x } ) \mathbf { h } , \mathbf { s } \mathbf { o } f ^ { \prime \prime } ( \mathbf { x } )$ is negative semi-definite. 

3. For functions of one variable, the above arguments can give an alternative proof of sufficiency which does not require Taylor’s Theorem. In fact, we have something like the following: 

$$
f ^ {\prime \prime} (x) <   0 \text {   on   } (a, b) \Rightarrow f \text {   locally   strictly   concave   on   } (a, b)
$$

$$
f ^ {\prime \prime} (x) \leq 0 \text {   on   } (a, b) \Rightarrow f \text {   locally   concave   on   } (a, b)
$$

$$
f ^ {\prime \prime} (x) > 0 \text {   on   } (a, b) \Rightarrow f \text {   locally   strictly   convex   on   } (a, b)
$$

$$
f ^ {\prime \prime} (x) \geq 0 \text {   on   } (a, b) \Rightarrow f \text {   locally   convex   on   } (a, b)
$$

The same results which we have demonstrated for the interval $( a , b )$ also hold for the entire domain X (which of course is also just an open interval, as it is an open convex subset of <). 

Q.E.D. 

Theorem 3.2.5 A non-decreasing twice differentiable concave transformation of a twice differentiable concavefunction (ofseveral variables) is also concave. 

Proof The details are left as an exercise. 

Q.E.D. 

Note finally the implied hierarchy among different classes of functions: 

negative definite Hessian ⊂ strictly concave ⊂ concave = negative semidefinite Hessian. 

As an exercise, draw a Venn diagram to illustrate these relationships (and add other classes of functions to it later on as they are introduced) 

The second order condition above is reminiscent of that for optimisation and suggests that concave or convex functions will prove useful in developing theories of optimising behaviour. In fact, there is a wider class of useful functions, leading us to now introduce further definitions. 

## 3.2.4 Variations on the convexity theme

Let $X \subseteq \Re ^ { n }$ be a convex set and $f : X  \Re { \mathfrak { a } }$ real-valued function defined on X. In order (for reasons which shall become clear in due course) to maintain consistency with earlier notation, we adopt the convention when labelling vectors x and $\mathbf { x } ^ { \prime }$ that $f ( \mathbf { x } ^ { \prime } ) \leq f ( \mathbf { x } )$ .<sup>2</sup> 

## Definition 3.2.5 Let

$$
C (\alpha) = \{\mathbf {x} \in X: f (\mathbf {x}) \geq \alpha \}.
$$

Then $f : X \to \Re$ is quasiconcave 

$\forall \alpha \in \Re , \ C ( \alpha )$ is a convex set. 

Theorem 3.2.6 The following statements are equivalent to the definition of quasiconcavity: 

1. ∀x $\neq \mathbf { x } ^ { \prime } \in X$ such that $f ( \mathbf { x } ^ { \prime } ) \leq f ( \mathbf { x } )$ and $\forall \lambda \in ( 0 , 1 )$ 

$$
f \left(\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}\right) \geq f (\mathbf {x} ^ {\prime}).
$$

2. ∀x, $\mathbf { x } ^ { \prime } \in X , \lambda \in [ 0 , 1 ] , f \left( \lambda \mathbf { x } + ( 1 - \lambda ) \mathbf { x } ^ { \prime } \right) \geq \operatorname* { m i n } \{ f ( \mathbf { x } ) , f ( \mathbf { x } ^ { \prime } ) \}$ 

3. (If f is differentiable,) $) \forall \mathbf { x } , \mathbf { x ^ { \prime } } \in X$ such that $f ( \mathbf { x } ) - f ( \mathbf { x } ^ { \prime } ) \geq 0 , f ^ { \prime } ( \mathbf { x } ^ { \prime } ) ( \mathbf { x } - \mathbf { \relax }$ $\mathbf { x } ^ { \prime } ) \geq 0 .$ 

Proof 1. We begin by showing the equivalence between the definition and condition 1.<sup>3</sup> 

(a) First suppose that the upper contour sets are convex. Let x and $\mathbf { x } ^ { \prime } \in X$ and let $\alpha = \operatorname* { m i n } \{ f ( \mathbf { x } ) , f ( \mathbf { x } ^ { \prime } ) \}$ . Then x and $\mathbf { x } ^ { \prime }$ are in $C ( \alpha )$ . By the hypothesis of convexity, for any $\lambda \in ( 0 , 1 ) , \lambda \mathbf { x } + ( 1 - \lambda ) \mathbf { x } ^ { \prime } \in C ( \alpha )$ The desired result now follows. 

(b) Now suppose that condition 1 holds. To show that $C ( \alpha )$ is a convex set, we just take x and $\mathbf { x } ^ { \prime } \in C ( \alpha )$ and investigate whether $\lambda \mathbf { x } + ( 1 -$ $\lambda ) \mathbf { x } ^ { \prime } \in C ( \alpha )$ . But, by our previous result, 

$$
f \left(\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}\right) \geq \min \{f (\mathbf {x}), f (\mathbf {x} ^ {\prime}) \} \geq \alpha
$$

where the final inequality holds because x and $\mathbf { x } ^ { \prime }$ are in $C ( \alpha )$ 

2. It is almost trivial to show the equivalence of conditions 1 and 2. 

(a) In the case where $f ( \mathbf { x } ) \geq f ( \mathbf { x } ^ { \prime } )$ or $f ( \mathbf { x } ^ { \prime } ) = \operatorname* { m i n } \{ f ( \mathbf { x } ) , f ( \mathbf { x } ^ { \prime } ) \}$ , there is nothing to prove. Otherwise, we can just reverse the labels x and $\mathbf { x } ^ { \prime }$ . The statement is true for $\mathbf { x } = \mathbf { x ^ { \prime } } \operatorname { o r } \lambda = 0 \operatorname { o r } \lambda = 1$ even if $f$ is not quasiconcave. 

(b) The proof of the converse is even more straightforward and is left as an exercise. 

3. Proving that condition 3 is equivalent to quasiconcavity for a differentiable function (by proving that it is equivalent to conditions 1 and 2) is much the trickiest part of the proof. 

(a) Begin by supposing that f satisfies conditions 1 and 2. Proving that condition 3 is necessary for quasiconcavity is the easier part of the proof (and appears as an exercise on one of the problem sets). Pick any $\lambda \ \in \ ( 0 , 1 )$ and, without loss of generality, x and $\mathbf { x } ^ { \prime }$ such that $f ( \mathbf { x } ^ { \prime } ) \leq f ( \mathbf { x } )$ . By quasiconcavity, 

$$
f \left(\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}\right) \geq f (\mathbf {x} ^ {\prime}).\tag{3.2.12}
$$

Consider 

$$
f | _ {L} (\lambda) = f \left(\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}\right) = f \left(\mathbf {x} ^ {\prime} + \lambda \left(\mathbf {x} - \mathbf {x} ^ {\prime}\right)\right).\tag{3.2.13}
$$

We want to show that the directional derivative 

$$
f | _ {L} ^ {\prime} (0) = f ^ {\prime} (\mathbf {x} ^ {\prime}) (\mathbf {x} - \mathbf {x} ^ {\prime}) \geq 0.\tag{3.2.14}
$$

But 

$$
f | _ {L} ^ {\prime} (0) = \lim _ {\lambda \to 0} \frac {f (\mathbf {x} ^ {\prime} + \lambda (\mathbf {x} - \mathbf {x} ^ {\prime})) - f (\mathbf {x} ^ {\prime})}{\lambda}.\tag{3.2.15}
$$

Since the right hand side is non-negative for small positive values of λ $( \lambda < 1 )$ , the derivative must be non-negative as required. 

(b) Now the difficult part — to prove that condition 3 is a sufficient condition for quasiconcavity. 

Suppose the derivative satisfies the hypothesis of the theorem, but f is not quasiconcave. In other words, $\exists \mathbf { x } , \mathbf { x } ^ { \prime } , \lambda ^ { * }$ such that 

$$
f \left(\lambda^ {*} \mathbf {x} + (1 - \lambda^ {*}) \mathbf {x} ^ {\prime}\right) <   \min \{f (\mathbf {x}), f (\mathbf {x} ^ {\prime}) \},\tag{3.2.16}
$$

where without loss of generality $f ( \mathbf { x } ^ { \prime } ) \leq f ( \mathbf { x } )$ . The hypothesis of the theorem applied first to x and $\lambda ^ { * } { \bf x } + ( 1 - \lambda ^ { * } ) { \bf x } ^ { \prime }$ and then to $\mathbf { x } ^ { \prime }$ and $\lambda ^ { * } { \bf x } + ( 1 - \lambda ^ { * } ) { \bf x } ^ { \prime }$ tells us that: 

$$
f ^ {\prime} \left(\lambda^ {*} \mathbf {x} + (1 - \lambda^ {*}) \mathbf {x} ^ {\prime}\right) \left(\mathbf {x} - (\lambda^ {*} \mathbf {x} + (1 - \lambda^ {*}) \mathbf {x} ^ {\prime})\right) \geq 0\tag{3.2.17}
$$

$$
f ^ {\prime} \left(\lambda^ {*} \mathbf {x} + (1 - \lambda^ {*}) \mathbf {x} ^ {\prime}\right) \left(\mathbf {x} ^ {\prime} - (\lambda^ {*} \mathbf {x} ^ {\prime} + (1 - \lambda^ {*}) \mathbf {x})\right) \geq 0.\tag{3.2.18}
$$

Revised: December 2, 1998 

Multiplying the first inequality by $( 1 - \lambda ^ { * } )$ and the second by $\lambda ^ { * }$ yields a pair of inequalities which can only be satisfied simultaneously if: 

$$
f ^ {\prime} \left(\lambda^ {*} \mathbf {x} + (1 - \lambda^ {*}) \mathbf {x} ^ {\prime}\right) (\mathbf {x} ^ {\prime} - \mathbf {x}) = 0.\tag{3.2.19}
$$

In other words, $f | _ { L } ^ { \prime } ( \lambda ^ { * } ) = 0 ;$ we already know that $f | _ { L } ( \lambda ^ { * } ) < f | _ { L } ( 0 ) \leq$ $f | _ { L } ( 1 )$ . We can apply the same argument to any point where the value of $f | _ { L }$ is less than $f | _ { L } ( 0 )$ to show that the corresponding part of the graph of $f | _ { L }$ has zero slope, or is flat. But this is incompatible either with continuity of $f | _ { L }$ or with the existence of a point where $f | _ { L } ( \lambda ^ { * } )$ is strictly less than $f | _ { L } ( 0 )$ . So we have a contradiction as required. 

Q.E.D. 

In words, part 3 of Theorem 3.2.6 says that whenever a differentiable quasiconcave function has a higher value at x than at $\mathbf { x } ^ { \prime } ,$ , or the same value at both points, then the directional derivative of f at $\mathbf { x } ^ { \prime }$ in the direction of x is non-negative. It might help to think about this by considering $n = 1$ and separating out the cases $x > x ^ { \prime }$ and $x < x ^ { \prime }$ 

Theorem 3.2.7 Let $f : X  \Re$ be quasiconcave and $g : \mathfrak { R } \to \mathfrak { R }$ be increasing. Then $g \circ f$ is a quasiconcavefunction. 

Proof This follows easily from the previous result. The details are left as an exercise. 

Q.E.D. 

Note the implications of Theorem 3.2.7 for utility theory. In particular, if preferences can be represented by a quasiconcave utility function, then they can be represented by a quasiconcave utility function only. This point will be considered again in a later section of the course. 

## Definition 3.2.6 $f : X  \Re$ is strictly quasiconcave

$\forall \mathbf { x } \neq \mathbf { x } ^ { \prime } \in X$ such that $f ( \mathbf { x } ) \geq f ( \mathbf { x } ^ { \prime } )$ and $\forall \lambda \in ( 0 , 1 ) , f ( \lambda \mathbf { x } + ( 1 - \lambda ) \mathbf { x } ^ { \prime } ) >$ $f ( \mathbf { x } ^ { \prime } )$ 

## Definition 3.2.7 f is (strictly) quasiconvex

$- f$ is (strictly) quasiconcave<sup>4</sup> 

## Definition 3.2.8 f is pseudoconcave

f is differentiable and quasiconcave and 

$$
f (\mathbf {x}) - f \left(\mathbf {x} ^ {\prime}\right) > 0 \quad \Rightarrow \quad f ^ {\prime} \left(\mathbf {x} ^ {\prime}\right) \left(\mathbf {x} - \mathbf {x} ^ {\prime}\right) > 0.
$$

Note that the last definition modifies slightly the condition in Theorem 3.2.6 which is equivalent to quasiconcavity for a differentiable function. 

Pseudoconcavity will crop up in the second order condition for equality constrained optimisation. 

We conclude this section by looking at a couple of the functions of several variables which will crop repeatedly in applications in economics later on. 

First, consider the interesting case of the affine function 

$$
f \colon \mathfrak {R} ^ {n} \to \mathfrak {R} \colon \mathbf {x} \mapsto M - \mathbf {p} ^ {\top} \mathbf {x},
$$

where $M \in \Re$ and $\mathbf { p } \in \mathfrak { R } ^ { n }$ . This function is both concave and convex, but neither strictly concave nor strictly convex. Furthermore, 

$$
f (\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}) = \lambda f (\mathbf {x}) + (1 - \lambda) f (\mathbf {x} ^ {\prime})\tag{3.2.20}
$$

$$
\geq \min \{f (\mathbf {x}), f (\mathbf {x} ^ {\prime}) \}\tag{3.2.21}
$$

and 

$$
\begin{array}{r c l} (- f) (\lambda \mathbf {x} + (1 - \lambda) \mathbf {x} ^ {\prime}) & = & \lambda (- f) (\mathbf {x}) + (1 - \lambda) (- f) (\mathbf {x} ^ {\prime}) \\ & \geq & \min \{(- f) (\mathbf {x}), (- f) (\mathbf {x} ^ {\prime}) \}, \end{array}\tag{3.2.22}
$$

(3.2.23) 

so $f$ is both quasiconcave and quasiconcave, but not strictly so in either case. $f$ is, however, pseudoconcave (and pseudoconvex) since 

$$
f (\mathbf {x}) > f \left(\mathbf {x} ^ {\prime}\right) \quad \Longleftrightarrow \quad \mathbf {p} ^ {\top} \mathbf {x} <   \mathbf {p} ^ {\top} \mathbf {x} ^ {\prime}\tag{3.2.24}
$$

$$
\Longleftrightarrow \mathbf {p} ^ {\top} (\mathbf {x} - \mathbf {x} ^ {\prime}) <   0\tag{3.2.25}
$$

$$
\Longleftrightarrow - f ^ {\prime} (\mathbf {x} ^ {\prime}) (\mathbf {x} - \mathbf {x} ^ {\prime}) <   0\tag{3.2.26}
$$

$$
\Longleftrightarrow f ^ {\prime} (\mathbf {x} ^ {\prime}) (\mathbf {x} - \mathbf {x} ^ {\prime}) > 0.\tag{3.2.27}
$$

Finally, here are two graphs of Cobb-Douglas functions:<sup>5</sup> 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1ea539b3-d28a-4058-b081-2faf541b59b7/d5d94085220ea1d2909c29e08220c4462136ebcfc99eb97c048101d477ac1671.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1ea539b3-d28a-4058-b081-2faf541b59b7/0a42bafe104dffefe735203ae8add07268acf55cf2ffd011a311f7aab38e3078.jpg)


## 3.3 Unconstrained Optimisation

Definition 3.3.1 Let $X \subseteq \Re ^ { n } , f : X \to \Re .$ 

Then f has a (strict) global maximum at $\mathbf { x } ^ { * } \iff \forall \mathbf { x } \in X , \mathbf { x } \neq \mathbf { x } ^ { * } , f ( \mathbf { x } ) \leq ( <$ $) f ( \mathbf { x } ^ { * } )$ 

Also f has a (strict) local maximum at $\mathbf { x } ^ { * } \iff \exists \epsilon > 0$ such that ∀x $\in$ $B \epsilon ( \mathbf { x } ^ { * } ) , \mathbf { x } \neq \mathbf { x } ^ { * } , f ( \mathbf { x } ) \leq ( < ) f ( \mathbf { x } ^ { * } )$ 

Similarly for minima. 

Theorem 3.3.1 A continuous real-valuedfunction on a compact subset of $\Re ^ { n }$ attains a global maximum and a global minimum. 

Proof Not given here. See ?. 

Q.E.D. 

While this is a neat result for functions on compact domains, results in calculus are generally for functions on open domains, since the limit of the first difference of the function at x, say, makes no sense if the function and the first difference are not defined in some open neighbourhood of $x$ (some $B \epsilon ( x ) )$ ). 

The remainder of this section and the next two sections are each centred around three related theorems: 

1. a theorem giving necessary or first order conditions which must be satisfied by the solution to an optimisation problem (Theorems 3.3.2, 3.4.1 and 3.5.1); 

2. a theorem giving sufficient or second order conditions under which a solution to the first order conditions satisfies the original optimisation problem (Theorems 3.3.3, 3.4.2 and 3.5.2); and 

3. a theorem giving conditions under which a known solution to an optimisation problem is the unique solution (Theorems 3.3.4, 3.4.3 and 3.5.3). 

The results are generally presented for maximisation problems. However, any minimisation problem is easily turned into a maximisation problem by reversing the sign of the function to be minimised and maximising the function thus obtained. 

Throughout the present section, we deal with the unconstrained optimisation problem 

$$
\max _ {\mathbf {x} \in X} f (\mathbf {x})\tag{3.3.1}
$$

where $X \subseteq \mathfrak { N } ^ { n }$ and $f : X  \Re$ is a real-valued function of several variables, called the objectivefunction of Problem (3.3.1.) 

(It is conventional to use the letter λ both to parameterise convex combinations and as a Lagrange multiplier. To avoid confusion, in this section we switch to the letter α for the former usage.) 

Theorem 3.3.2 Necessary (first order) condition for unconstrained maxima and minima. 

Let X be open and f differentiable with a local maximum or minimum at $\mathbf { x ^ { * } } \in X$ Then $f ^ { \prime } ( \mathbf { x } ^ { * } ) = \mathbf { 0 }$ , or f has a stationary point at $\mathbf { x } ^ { * }$ 

Proof Without loss of generality, assume that the function has a local maximum at $\mathbf { x } ^ { * }$ . Then $\exists \epsilon > 0$ such that, whenever $\| \mathbf { h } \| < \epsilon ,$ 

$$
f (\mathbf {x} ^ {*} + \mathbf {h}) - f (\mathbf {x} ^ {*}) \leq 0.
$$

It follows that, for $0 < h < \epsilon$ 

$$
\frac {f (\mathbf {x} ^ {*} + h \mathbf {e} _ {i}) - f (\mathbf {x} ^ {*})}{h} \leq 0,
$$

Revised: December 2, 1998 

(where $\mathbf { e } _ { i }$ denotes the ith standard basis vector) and hence that 

$$
\frac {\partial f}{\partial x _ {i}} (\mathbf {x} ^ {*}) = \lim _ {h \to 0} \frac {f (\mathbf {x} ^ {*} + h \mathbf {e} _ {i}) - f (\mathbf {x} ^ {*})}{h} \leq 0.\tag{3.3.2}
$$

Similarly, for $0 > h > - \epsilon$ 

$$
\frac {f (\mathbf {x} ^ {*} + h \mathbf {e} _ {i}) - f (\mathbf {x} ^ {*})}{h} \geq 0,
$$

and hence 

$$
\frac {\partial f}{\partial x _ {i}} (\mathbf {x} ^ {*}) = \lim _ {h \to 0} \frac {f (\mathbf {x} ^ {*} + h \mathbf {e} _ {i}) - f (\mathbf {x} ^ {*})}{h} \geq 0.\tag{3.3.3}
$$

Combining (3.3.2) and (3.3.3) yields the desired result. 

Q.E.D. 

The first order conditions are only useful for identifying optima in the interior of the domain of the objective function: Theorem 3.3.2 applies only to functions whose domain $X$ is open. Other methods must be used to check for possible corner solutions or boundary solutions to optimisation problems where the objective function is defined on a domain that is not open. 

Theorem 3.3.3 Sufficient (second order) conditionfor unconstrained maxima and minima. 

Let $X \subseteq \Re ^ { n }$ be open and let $f : X \to \Re$ be a twice continuously differentiable function with $f ^ { \prime } ( \mathbf { x } ^ { * } ) = \mathbf { 0 }$ and $f ^ { \prime \prime } ( \mathbf { x } ^ { * } )$ negative definite. 

Then f has a strict local maximum at $\mathbf { x } ^ { * }$ . 

Similarlyfor positive definite Hessians and local minima. 

Proof Consider the second order Taylor expansion used previously in the proof of Theorem 3.2.4: for any $\mathbf { x } \in X , \exists s \in ( 0 , 1 )$ such that 

$$
f (\mathbf {x}) = f \left(\mathbf {x} ^ {*}\right) + f ^ {\prime} \left(\mathbf {x} ^ {*}\right) \left(\mathbf {x} - \mathbf {x} ^ {*}\right) + \frac {1}{2} \left(\mathbf {x} - \mathbf {x} ^ {*}\right) ^ {\top} f ^ {\prime \prime} \left(\mathbf {x} ^ {*} + s \left(\mathbf {x} - \mathbf {x} ^ {*}\right)\right) \left(\mathbf {x} - \mathbf {x} ^ {*}\right).
$$

or, since the first derivative vanishes at $\mathbf { x } ^ { * }$ , 

$$
f (\mathbf {x}) = f (\mathbf {x} ^ {*}) + \frac {1}{2} (\mathbf {x} - \mathbf {x} ^ {*}) ^ {\top} f ^ {\prime \prime} (\mathbf {x} ^ {*} + s (\mathbf {x} - \mathbf {x} ^ {*})) (\mathbf {x} - \mathbf {x} ^ {*}).
$$

Since $f ^ { \prime \prime }$ is continuous, $f ^ { \prime \prime } ( { \bf x } ^ { * } + s ( { \bf x } - { \bf x } ^ { * } ) )$ will also be negative definite for x in some open neighbourhood of $\mathbf { x } ^ { * }$ . Hence, for x in this neighbourhood, $f ( \mathbf { x } ) <$ $f ( \mathbf { x } ^ { * } )$ and $f$ has a strict local maximum at $\mathbf { x } ^ { * }$ 

Q.E.D. 

The weak form of this result does not hold. In other words, semi-definiteness of the Hessian matrix at $\mathbf { x } ^ { * }$ is not sufficient to guarantee that f has any sort of maximum at $\mathbf { x } ^ { * }$ . For example, if $f ( x ) = x ^ { 3 }$ , then the Hessian is negative semidefinite at $x = 0$ but the function does not have a local maximum there (rather, it has a point $o f i n f l e x i o n )$ 

Theorem 3.3.4 Uniqueness conditions for unconstrained maximisation. $H$ 

1. $\mathbf { x } ^ { * }$ solves Problem (3.3.1) and 

2. f is strictly quasiconcave (presupposing that X is a convex $s e t )$ , 

then $\mathbf { x } ^ { * }$ is the unique (global) maximum. 

Proof Suppose not, in other words that $\exists \mathbf { x } \neq \mathbf { x } ^ { * }$ such that $f \left( \mathbf { x } \right) = f \left( \mathbf { x } ^ { * } \right)$ Then, for any $\alpha \in ( 0 , 1 )$ 

$$
f \left(\alpha \mathbf {x} + (1 - \alpha) \mathbf {x} ^ {*}\right) > \min \left\{f (\mathbf {x}), f \left(\mathbf {x} ^ {*}\right) \right\} = f \left(\mathbf {x} ^ {*}\right),
$$

so $f$ does not have a maximum at either x or $\mathbf { x } ^ { * }$ . 

This is a contradiction, so the maximum must be unique. 

Q.E.D. 

Theorem 3.3.5 Tempting, but not quite true, corollaries ofTheorem 3.3.3 are: 

• Every stationary point of a twice continuously differentiable strictly concave function is a strict global maximum (and so there can be at most one stationary point). 

• Every stationary point ofa twice continuously differentiable strictly convex function is a strict global minimum. 

Proof If the Hessian matrix is positive/negative definite everywhere, then the argument in the proof of Theorem 3.3.3 can be applied for $\mathbf x \in X$ and not just for $\mathbf { x } \in B \epsilon \left( \mathbf { x } ^ { * } \right)$ . If there are points at which the Hessian is merely semi-definite, then the proof breaks down. 

Q.E.D. 

Note that many strictly concave and strictly convex functions will have no stationary points, for example 

$$
f \colon \Re \to \Re \colon x \mapsto e ^ {x}.
$$

Revised: December 2, 1998 

## 3.4 Equality Constrained Optimisation: The Lagrange Multiplier Theorems

Throughout this section, we deal with the equality constrained optimisation problem 

$$
\begin{array}{c} \max _ {\mathbf {x} \in X} f (\mathbf {x}) \\ \mathrm{s.t.} g (\mathbf {x}) = \mathbf {0} _ {m} \end{array}\tag{3.4.1}
$$

where $X \subseteq \Re ^ { n } , f : X \to \Re$ is a real-valued function of several variables, called the objective function of Problem (3.4.1) and $g : X  \Re ^ { m }$ is a vector-valued function of several variables, called the constraintfunction of Problem (3.4.1); or, equivalently, $g ^ { j } \colon X \  \ \Re$ are real-valued functions for $j = 1 , \dots , m$ . In other words, there are m scalar constraints represented by a single vector constraint: 

$$
\left( \begin{array}{c} g ^ {1} (\mathbf {x}) \\ \vdots \\ g ^ {m} (\mathbf {x}) \end{array} \right) = \left( \begin{array}{c} 0 \\ \vdots \\ 0 \end{array} \right).
$$

We will introduce and motivate the Lagrange multiplier method which applies to such constrained optimisation problems with equality constraints. We will assume where appropriate that the objective function f and the m constraint functions $g ^ { 1 } , \ldots , g ^ { m }$ are all once or twice continuously differentiable. 

The entire discussion here is again presented in terms of maximisation, but can equally be presented in terms of minimisation by reversing the sign of the objective function. Similarly, note that the signs of the constraint function(s) can be reversed without altering the underlying problem. We will see, however, that this also reverses the signs of the corresponding Lagrange multipliers. The significance of this effect will be seen from the formal results, which are presented here in terms of the usual three theorems. 

Before moving on to those formal results, we briefly review the methodology for solving constrained optimisation problems which should be familiar from introductory and intermediate economic analysis courses. 

If $\mathbf { x } ^ { * }$ is a solution to Problem (3.4.1), then there exist Lagrange multipliers, $^ 6 \lambda \equiv$ $\left( \lambda _ { 1 } , \ldots , \lambda _ { m } \right)$ , such that 

$$
f ^ {\prime} \left(\mathbf {x} ^ {*}\right) + \boldsymbol {\lambda} ^ {\top} g ^ {\prime} \left(\mathbf {x} ^ {*}\right) = \mathbf {0} _ {n}.
$$

Thus, to find the constrained optimum, we proceed as if optimising the Lagrangean: 

$$
\mathcal {L} \left(\mathbf {x}, \boldsymbol {\lambda}\right) \equiv f \left(\mathbf {x} ^ {*}\right) + \boldsymbol {\lambda} ^ {\top} g \left(\mathbf {x} ^ {*}\right).
$$

Note that 

1. ${ \mathcal { L } } = f$ whenever $g = \mathbf { 0 }$ and 

2. $g = \mathbf { 0 }$ where L is optimised. 

Roughly speaking, this is why the constrained optimum of $f$ corresponds to the optimum of $\mathcal { L } .$ 

The Lagrange multiplier method involves the following four steps: 

1. introduce the m Lagrange multipliers, $\pmb { \lambda } \equiv ( \lambda _ { 1 } , \ldots , \lambda _ { m } )$ 

2. Define the Lagrangean $\mathcal { L } \colon X \times \Re ^ { m }  \Re$ , where 

$$
X \times \Re^ {m} \equiv \left\{\left(\mathbf {x}, \boldsymbol {\lambda}\right): \mathbf {x} \in X, \boldsymbol {\lambda} \in \Re^ {m} \right\},
$$

by 

$$
\mathcal {L} \left(\mathbf {x}, \boldsymbol {\lambda}\right) \equiv f \left(\mathbf {x}\right) + \boldsymbol {\lambda} ^ {\top} g \left(\mathbf {x}\right).
$$

3. Find the stationary points of the Lagrangean, i.e. set $\mathcal { L } ^ { \prime } \left( \mathbf { x } , \lambda \right) = \mathbf { 0 }$ . Since the Lagrangean is a function of $n + m$ variables, this gives $n + m$ first order conditions. The first n are 

$$
f ^ {\prime} (\mathbf {x}) + \pmb {\lambda} ^ {\top} g ^ {\prime} (\mathbf {x}) = \mathbf {0}
$$

or 

$$
\frac {\partial f}{\partial x _ {i}} (\mathbf {x}) + \sum_ {j = 1} ^ {m} \lambda_ {j} \frac {\partial g ^ {j}}{\partial x _ {i}} (\mathbf {x}) = 0 i = 1, \ldots , n.
$$

The last m are just the original constraints, 

$$
g (\mathbf {x}) = \mathbf {0}
$$

or 

$$
g ^ {j} (\mathbf {x}) = 0 \quad j = 1, \ldots , m.
$$

4. Finally, the second order conditions must be checked. 

As an example, consider maximisation of a utility function representing Cobb-Douglas preferences subject to a budget constraint. 

The first n first order or Lagrangean conditions say that the total derivative (or gradient) of $f$ at x is a linear combination of the total derivatives (or gradients) of the constraint functions at x. 

Consider a picture with $n = 2$ and $m = 1$ 

Since the directional derivative along a tangent to a level set or indifference curve is zero at the point of tangency, x, (the function is at a maximum or minimum along the tangent) or $f ^ { \prime } \left( \mathbf { x } \right) \left( \mathbf { x } ^ { \prime } - \mathbf { x } \right) = 0$ , the gradient vector, $f ^ { \prime } \left( \mathbf { x } \right) ^ { \top }$ , must be perpendicular to the direction of the tangent, $\mathbf { x } ^ { \prime } - \mathbf { x }$ 

At the optimum, the level sets of f and g have a common tangent, so $f ^ { \prime } \left( \mathbf { x } \right)$ and $g ^ { \prime } \left( \mathbf { x } \right)$ are collinear, or $f ^ { \prime } \left( \mathbf { x } \right) = - \lambda g ^ { \prime } \left( \mathbf { x } \right)$ . It can also be seen with a little thought that for the solution to be a local constrained maximum, λ must be positive if $g$ is quasiconcave and negative if $g$ is quasiconvex (in either case, the constraint curve is the boundary of a convex set). 

We now consider the equality constrained optimisation problem in more depth. 

Theorem 3.4.1 First order (necessary) conditions for optimisation with equality constraints. 

Consider problem (3.4.1) or the corresponding minimisation problem. 

1. $\mathbf { x } ^ { * }$ solves this problem (which implies that $g \left( \mathbf { x } ^ { * } \right) = \mathbf { 0 } )$ , 

2. $f$ and g are continuously differentiable, and 

3. the $m \times n$ matrix 

$$
g ^ {\prime} \left(\mathbf {x} ^ {*}\right) = \left( \begin{array}{c c c} \frac {\partial g ^ {1}}{\partial x _ {1}} \left(\mathbf {x} ^ {*}\right) & \ldots & \frac {\partial g ^ {1}}{\partial x _ {n}} \left(\mathbf {x} ^ {*}\right) \\ \vdots & \ddots & \vdots \\ \frac {\partial g ^ {m}}{\partial x _ {1}} \left(\mathbf {x} ^ {*}\right) & \ldots & \frac {\partial g ^ {m}}{\partial x _ {n}} \left(\mathbf {x} ^ {*}\right) \end{array} \right)
$$

is of rank m (i.e. there are no redundant constraints, both in the sense that there are fewer constraints than variables and in the sense that the constraints which are present are ‘independent’), 

then $\exists \pmb { \lambda } ^ { * } \in \Re ^ { m }$ such that $f ^ { \prime } \left( \mathbf { x } ^ { * } \right) + { \boldsymbol { \lambda } } ^ { * } { \boldsymbol { \mathcal { I } } } ^ { \prime } g ^ { \prime } \left( \mathbf { x } ^ { * } \right) = \mathbf { 0 } ~ ( i . e .$ . in $\Re ^ { n } , f ^ { \prime } \left( \mathbf { x } ^ { * } \right)$ is in the m−dimensional subspace generated by the m vectors $g ^ { 1 ^ { \prime } } \left( \mathbf { x } ^ { * } \right) , \ldots , g ^ { m ^ { \prime } } \left( \mathbf { x } ^ { * } \right) )$ . 

Proof The idea is to solve $g \left( \mathbf { x } ^ { * } \right) = \mathbf { 0 }$ for m variables as a function of the other $n - m$ and to substitute the solution into the objective function to give an unconstrained problem with $n - m$ variables. 

For this proof, we need Theorem 2.6.1 on p. 2.6.1 above, the Implicit Function Theorem. Using this theorem, we must find the m weights $\lambda _ { 1 } , \ldots , \lambda _ { m }$ to prove that $f ^ { \prime } \left( \mathbf { x } ^ { * } \right)$ is a linear combination of $g ^ { 1 ^ { \prime } } \left( \mathbf { x } ^ { * } \right) , \ldots , g ^ { m ^ { \prime } } \left( \mathbf { x } ^ { * } \right)$ 

Without loss of generality, we assume that the first m columns of $g ^ { \prime } \left( \mathbf { x } ^ { * } \right)$ are linearly independent (if not, then we merely relabel the variables accordingly). 

Now we can partition the vector $\mathbf { x } ^ { * }$ as $\mathbf { \Psi } ( \mathbf { y } ^ { * } , \mathbf { z } ^ { * } )$ and, using the notation of the Implicit Function Theorem, find a neighbourhood $Z$ of $\mathbf { z } ^ { \ast }$ and a function h defined on $Z$ such that 

$$
g \left(h (\mathbf {z}), \mathbf {z}\right) = \mathbf {0} \quad \forall \mathbf {z} \in Z
$$

and also 

$$
h ^ {\prime} (\mathbf {z} ^ {*}) = - (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}} g.
$$

Now define a new objective function $F \colon Z  \Re$ by 

$$
F (\mathbf {z}) \equiv f (h (\mathbf {z}), \mathbf {z}).
$$

Since $\mathbf { x } ^ { * }$ solves the constrained problem $\operatorname* { m a x } _ { \mathbf { x } \in X } f \left( \mathbf { x } \right)$ subject to $g \left( \mathbf { x } \right) = \mathbf { 0 }$ , it follows that $\mathbf { z } ^ { \ast }$ solves the unconstrained problem ma $\tau _ { \mathbf { z } \in Z } F \left( \mathbf { z } \right)$ . (This is easily shown using a proof by contradiction argument.) 

Hence, $\mathbf { z } ^ { \ast }$ satisfies the first order conditions for unconstrained maximisation of $F ,$ namely 

$$
F ^ {\prime} \left(\mathbf {z} ^ {*}\right) = \mathbf {0}.
$$

Applying the Chain Rule in exactly the same way as in the proof of the Implicit Function Theorem yields an equation which can be written in shorthand as: 

$$
D _ {\mathbf {y}} f h ^ {\prime} (\mathbf {z}) + D _ {\mathbf {z}} f = \mathbf {0}.
$$

Substituting for $h ^ { \prime } \left( \mathbf { z } \right)$ gives: 

$$
D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}} g = D _ {\mathbf {z}} f.
$$

We can also partition $f ^ { \prime } \left( \mathbf { x } \right)$ as 

$$
\left( \begin{array}{c c} D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {y}} g & D _ {\mathbf {z}} f \end{array} \right)
$$

Substituting for the second sub-matrix yields: 

$$
\begin{array}{r c l} f ^ {\prime} (\mathbf {x}) & = & \left( \begin{array}{c c} D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {y}} g & D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}} g \end{array} \right) \\ & = & D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} \left( \begin{array}{c c} D _ {\mathbf {y}} g & D _ {\mathbf {z}} g \end{array} \right) \\ & = & - \pmb {\lambda} ^ {\top} g ^ {\prime} (\mathbf {x}) \end{array}
$$

where we define 

$$
\pmb {\lambda} \equiv - D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1}.\tag{Q.E.D.}
$$

Theorem 3.4.2 Second order (sufficient or concavity) conditions for maximisation with equality constraints. 

1. f and g are differentiable, 

Revised: December 2, 1998 

2. $f ^ { \prime } \left( \mathbf { x } ^ { * } \right) + { \lambda ^ { * } } ^ { \top } g ^ { \prime } \left( \mathbf { x } ^ { * } \right) = \mathbf { 0 }$ (i.e. thefirst order conditions are satisfied at ${ \mathbf { x } } ^ { * } ) ,$ 

3. $\lambda _ { j } ^ { * } \ge 0 f o r j = 1 , \ldots , m ,$ 

4. $f$ is pseudoconcave, and 

5. $g ^ { j }$ is quasiconcave for $j = 1 , \ldots , m$ 

then $\mathbf { x } ^ { * }$ solves the constrained maximisation problem. 

It should be clear that non-positive Lagrange multipliers and quasiconvex constraint functions can take the place of non-negative Lagrange multipliers and quasiconcave Lagrange multipliers to give an alternative set of second order conditions. 

Proof Suppose that the second order conditions are satisfied, but that $\mathbf { x } ^ { * }$ is not a constrained maximum. We will derive a contradiction. 

Since $\mathbf { x } ^ { * }$ is not a maximum, $\exists \mathbf { x } \neq \mathbf { x } ^ { * }$ such that $g \left( \mathbf { x } \right) = \mathbf { 0 }$ but $f \left( \mathbf { x } \right) > f \left( \mathbf { x } ^ { * } \right)$ 

By pseudoconcavity, $f \left( \mathbf { x } \right) - f \left( \mathbf { x } ^ { * } \right) > 0$ implies that $f ^ { \prime } \left( \mathbf { x } ^ { * } \right) \left( \mathbf { x } - \mathbf { x } ^ { * } \right) > 0 .$ 

$$
\mathbf {x} ^ {*}
$$

$$
g \left(\mathbf {x} ^ {*}\right) = g (\mathbf {x}) = \mathbf {0},
$$

By quasiconcavity of the constraint functions (see Theorem $3 . 2 . 6 ) , g ^ { j } \left( \mathbf { x } \right) - g ^ { j } \left( \mathbf { x } ^ { * } \right) =$ 0 implies that $g ^ { j ^ { \prime } } \left( \mathbf { x } ^ { * } \right) \left( \mathbf { x } - \mathbf { x } ^ { * } \right) \geq 0$ 

By assumption, all the Lagrange multipliers are non-negative, so 

$$
f ^ {\prime} \left(\mathbf {x} ^ {*}\right) \left(\mathbf {x} - \mathbf {x} ^ {*}\right) + \boldsymbol {\lambda} ^ {* \top} g ^ {\prime} \left(\mathbf {x} ^ {*}\right) \left(\mathbf {x} - \mathbf {x} ^ {*}\right) > 0.
$$

Rearranging yields: 

$$
\left[ f ^ {\prime} \left(\mathbf {x} ^ {*}\right) + \boldsymbol {\lambda} ^ {* \top} g ^ {\prime} \left(\mathbf {x} ^ {*}\right) \right] \left(\mathbf {x} - \mathbf {x} ^ {*}\right) > 0.
$$

But the first order condition guarantees that the LHS of this inequality is zero (not positive), which is the required contradiction. 

Q.E.D. 

## Theorem 3.4.3 Uniqueness condition for equality constrained maximisation. If

1. $\mathbf { x } ^ { * }$ is a solution, 

2. f is strictly quasiconcave, and 

3. $g ^ { j }$ is an affinefunction (i.e. both convex and concave)for $j = 1 , \ldots , m$ 

then $\mathbf { x } ^ { * }$ is the unique (global) maximum. 

Proof The uniqueness result is also proved by contradiction. Note that it does not require any differentiability assumption. 

• We first show that the feasible set is convex. 

Suppose $\mathbf { x } \neq \mathbf { x } ^ { * }$ are two distinct solutions. 

Consider the convex combination of these two solutions $\mathbf { x } \alpha \equiv \alpha \mathbf { x } + \left( 1 - \alpha \right) \mathbf { x } ^ { * } .$ Since each $g ^ { j }$ is affine and $g ^ { j } \left( \mathbf { x } ^ { * } \right) = g ^ { j } \left( \mathbf { x } \right) = 0$ , we have 

$$
g ^ {j} (\mathbf {x} \alpha) = \alpha g ^ {j} (\mathbf {x}) + (1 - \alpha) g ^ {j} (\mathbf {x} ^ {*}) = 0.
$$

In other words, xα also satisfies the constraints. 

• To complete the proof, we find the required contradiction: 

Since f is strictly quasiconcave and $f \left( \mathbf { x } ^ { * } \right) = f \left( \mathbf { x } \right)$ , it must be the case that $f \left( \mathbf { x } \alpha \right) > f \left( \mathbf { x } ^ { * } \right)$ 

Q.E.D. 

The construction of the obvious corollaries for minimisation problems is left as an exercise. 

We conclude this section with 

Theorem 3.4.4 (Envelope Theorem.) Consider the modified constrained optimisation problem: 

$$
\max _ {\mathbf {x}} f (\mathbf {x}, \boldsymbol {\alpha}) \quad \text { subject   to } \quad g (\mathbf {x}, \boldsymbol {\alpha}) = \mathbf {0},\tag{3.4.2}
$$

where $\mathbf { x } \in \mathbb { R } ^ { n }$ , α∈ $\Re ^ { q } , ~ f \colon \Re ^ { n + q } \  \ \Re$ and $g \colon \mathfrak { R } ^ { n + q } \ \longrightarrow \ \mathfrak { R } ^ { m }$ (i.e. as usual f is the real-valued objective function and g is a vector of m real-valued constraint functions, but either or both can depend on exogenous or control variables α as well as on the endogenous or choice variables x). 

Suppose that the standard conditions for application of the Lagrange multiplier theorems are satisfied. 

Let $\mathbf { x } ^ { * } \left( \alpha \right)$ denote the optimal choice ofxfor given α $( \mathbf { x } ^ { * } \colon \mathfrak { R } ^ { q }  \mathfrak { R } ^ { n }$ is called the optimal response function) and let $M \left( \alpha \right)$ denote the maximum value attainable by f for given α $( M \colon \mathfrak { R } ^ { q } \to \mathfrak { R }$ is called the envelope function). 

Then the partial derivative of M with respect to $\alpha _ { i }$ is just the partial derivative ofthe relevant Lagrangean, $f + \lambda ^ { \top } g ,$ , with respect to $\alpha _ { i } ,$ , evaluated at the optimal value ofx. The dependence ofthe vector ofLagrange multipliers, λ, on the vector α should be ignored in calculating the last-mentioned partial derivative. 

Proof The Envelope Theorem can be proved in the following steps: 

Revised: December 2, 1998 

1. Write down the identity relating the functions M, f and $\mathbf { x } ^ { * }$ : 

$$
M (\boldsymbol {\alpha}) \equiv f \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right)
$$

2. Use (2.5.4) to derive an expression for the partial derivatives $\frac { \partial M } { \partial \alpha _ { i } }$ of $M$ in terms of the partial derivatives of f and $\mathbf { x } ^ { * }$ : 

$$
M ^ {\prime} (\boldsymbol {\alpha}) = D _ {\mathbf {x}} f \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right) \mathbf {x} ^ {* \prime} (\boldsymbol {\alpha}) + D _ {\boldsymbol {\alpha}} f \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right).
$$

3. The first order (necessary) conditions for constrained optimisation say that 

$$
D _ {\mathbf {x}} f \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right) = - \boldsymbol {\lambda} ^ {\top} D _ {\mathbf {x}} g \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right)
$$

and allow us to eliminate the $\frac { \partial f } { \partial { { x } _ { i } } }$ terms from this expression. 

4. Apply (2.5.4) again to the identity $g \left( \mathbf { x } ^ { * } , \alpha \right) = \mathbf { 0 } _ { m }$ to obtain 

$$
D _ {\mathbf {x}} g \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right) \mathbf {x} ^ {* \prime} (\boldsymbol {\alpha}) + D _ {\boldsymbol {\alpha}} g \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right) = \mathbf {0} _ {m \times q}.
$$

Finally, use this result to eliminate the $\textstyle { \frac { \partial g } { \partial x _ { i } } }$ terms from your new expression for $\frac { \partial M } { \partial \alpha _ { i } }$ 

Combining all these results gives: 

$$
M ^ {\prime} (\boldsymbol {\alpha}) = D _ {\boldsymbol {\alpha}} f \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right) + \boldsymbol {\lambda} ^ {\top} D _ {\boldsymbol {\alpha}} g \left(\mathbf {x} ^ {*} (\boldsymbol {\alpha}), \boldsymbol {\alpha}\right),
$$

which is the required result. 

Q.E.D. 

In applications in economics, the most frequently encountered applications will make sufficient assumptions to guarantee that 

1. $\mathbf { x } ^ { * }$ satisfies the first order conditions with each $\lambda _ { i } \geq 0 $ 

2. the Hessian $f ^ { \prime \prime } \left( \mathbf { x } ^ { * } \right)$ is a negative definite $( n \times n )$ matrix; and 

3. $g$ is a linear function, 

so that $\mathbf { x } ^ { * }$ is the unique optimal solution to the equality constrained optimisation problem. 

# 3.5 Inequality Constrained Optimisation: The Kuhn-Tucker Theorems

Throughout this section, we deal with the inequality constrained optimisation problem 

$$
\begin{array}{r l} & {\max _ {\mathbf {x} \in X} f (\mathbf {x})} \\ {\mathrm{s.t.}} & {g ^ {i} (\mathbf {x}) \geq 0, i = 1, 2, \ldots , m} \end{array}\tag{3.5.1}
$$

where once again $X \ \subseteq \ { \mathfrak { R } } ^ { n } , \ f \ : \ X \ \to \ { \mathfrak { R } }$ is a real-valued function of several variables, called the objective function of Problem (3.5.1) and $g : X  \Re ^ { m }$ is a vector-valued function of several variables, called the constraint function of Problem (3.5.1). 

Before presenting the usual theorems formally, we need some graphical motivation concerning the interpretation of Lagrange multipliers. 

Suppose that the constraint functions are given by 

$$
g (\mathbf {x}, \boldsymbol {\alpha}) = \boldsymbol {\alpha} - h (\mathbf {x}).\tag{3.5.2}
$$

The Lagrangean is 

$$
\mathcal {L} (\mathbf {x}, \boldsymbol {\lambda}) = f (\mathbf {x}) + \boldsymbol {\lambda} ^ {\top} (\boldsymbol {\alpha} - h (\mathbf {x})).\tag{3.5.3}
$$

Thus, using the Envelope Theorem, it is easily seen that the rate of change of the envelope function $M \left( \alpha \right)$ with respect to the ‘level’ of the ith underlying constraint function $h ^ { i }$ is: 

$$
\frac {\partial M}{\partial \alpha_ {i}} = \frac {\partial \mathcal {L}}{\partial \alpha_ {i}} = \lambda_ {i}.\tag{3.5.4}
$$

Thus 

• when $\lambda _ { i } ~ = ~ 0$ , the envelope function is at its maximum, or the objective function at its unconstrained maximum, and the constraint is not binding. 

• when $\lambda _ { i } < 0$ , the envelope function is decreasing 

• when $\lambda _ { i } > 0$ , the envelope function is increasing 

Now consider how the nature of the inequality constraint change as $\alpha _ { i }$ increases (as illustrated, assuming $f$ quasiconcave as usual and $h ^ { i }$ quasiconvex or $g ^ { i }$ quasiconcave, so that the relationship between $\alpha _ { i }$ and $\lambda _ { i }$ is negative) 

$$
h ^ {i} (\mathbf {x}) \leq \alpha_ {i}\tag{3.5.5}
$$

Revised: December 2, 1998 

<table><tr><td>Type of constraint</td><td>Derivative of objective fn.</td><td>Lagrange Multiplier</td><td>Constraint fn.</td></tr><tr><td>Binding/active</td><td><eq>f&#x27; \leq 0</eq></td><td><eq>\lambda \geq 0</eq></td><td><eq>g = 0</eq></td></tr><tr><td>Non-binding/inactive</td><td><eq>f&#x27; = 0</eq></td><td><eq>\lambda = 0</eq></td><td><eq>g &gt; 0</eq></td></tr></table>


Table 3.1: Sign conditions for inequality constrained optimisation


(or $g ^ { i } \left( { \bf x } , { \pmb \alpha } \right) \ge 0 )$ . For values of $\alpha _ { i }$ such that $\lambda _ { i } > 0$ , this constraint is strictly binding. For values of $\alpha _ { i }$ such that $\lambda _ { i } = 0$ , this constraint is just binding. For values of $\alpha _ { i }$ such that $\lambda _ { i } < 0$ , this constraint is non-binding. 

Note that in this setup, 

$$
\frac {\partial^ {2} M}{\partial \alpha_ {i} ^ {2}} = \frac {\partial \lambda_ {i}}{\partial \alpha_ {i}} <   0,\tag{3.5.6}
$$

so that the envelope function is strictly concave (up to the unconstrained optimum, and constant beyond it). 

Thus we will find that part of the necessity conditions below is that the Lagrange multipliers be non-negative. (For equality constrained optimisation, the signs were important only when dealing with second order conditions). 

Consider also at this stage the first order conditions for maximisation of a function of one variable subject to a non-negativity constraint: 

$$
\max _ {x} f (x) \text {   s.t.   } x \geq 0.
$$

They can be expressed as: 

$$
f ^ {\prime} (x ^ {*}) \leq 0\tag{3.5.7}
$$

$$
f ^ {\prime} (x ^ {*}) = 0 \quad \text { if } x > 0\tag{3.5.8}
$$

The various sign conditions which we have looked at are summarised in Table 3.1. 

Theorem 3.5.1 Necessary (first order) conditions for optimisation with inequality constraints. 

$$
I f
$$

1. $\mathbf { x } ^ { * }$ solves Problem (3.5.1), with 

$$
g ^ {i} \left(\mathbf {x} ^ {*}\right) = 0, i = 1, 2, \ldots , b
$$

and 

$$
g ^ {i} \left(\mathbf {x} ^ {*}\right) > 0, i = b + 1, \ldots , m
$$

(in other words, the first b constraints are binding (active) at $\mathbf { x } ^ { * }$ and the last $n - b$ are non-binding (inactive) at $\mathbf { x } ^ { * }$ , renumbering the constraints if necessary to achieve this), 

2. f and g are continuously differentiable, and 

3. the $b \times n$ submatrix of $g ^ { \prime } \left( \mathbf { x } ^ { * } \right)$ 

$$
\left( \begin{array}{c c c} \frac {\partial g ^ {1}}{\partial x _ {1}} \left(\mathbf {x} ^ {*}\right) & \ldots & \frac {\partial g ^ {1}}{\partial x _ {n}} \left(\mathbf {x} ^ {*}\right) \\ \vdots & \ddots & \vdots \\ \frac {\partial g ^ {b}}{\partial x _ {1}} \left(\mathbf {x} ^ {*}\right) & \ldots & \frac {\partial g ^ {b}}{\partial x _ {n}} \left(\mathbf {x} ^ {*}\right) \end{array} \right),
$$

is offull rank b (i.e. there are no redundant binding constraints, both in the sense that there are fewer binding constraints than variables and in the sense that the constraints which are binding are ‘independent’), 

then $\exists \pmb { \lambda } \in \Re ^ { m }$ such that $f ^ { \prime } \left( \mathbf { x } ^ { * } \right) + \lambda ^ { \top } g ^ { \prime } \left( \mathbf { x } ^ { * } \right) = \mathbf { 0 }$ , with $\lambda _ { i } \ge 0 f o r i = 1 , 2 , . . . , m$ and $g ^ { i } ( { \bf x } ^ { * } ) = 0 i f \lambda _ { i } > 0 .$ 

Proof The proof is similar to that of Theorem 3.4.1 for the equality constrained case. It can be broken into seven steps. 

## 1. Suppose $\mathbf { x } ^ { * }$ solves Problem (3.5.1).

We begin by restricting attention to a neighbourhood $B _ { \epsilon } \left( \mathbf { x } ^ { * } \right)$ throughout which the non-binding constraints remain non-binding, i.e. 

$$
g ^ {i} (\mathbf {x}) > 0 \forall \mathbf {x} \in B _ {\epsilon} (\mathbf {x} ^ {*}), i = b + 1, \ldots , m.\tag{3.5.9}
$$

Such a neighbourhood exists since the constraint functions are continuous. Since $\mathbf { x } ^ { * }$ solves Problem (3.5.1) by assumption, it also solves the following problem: 

$$
\begin{array}{r l} & {\max _ {\mathbf {x} \in B _ {\epsilon} (\mathbf {x} ^ {*})} f (\mathbf {x})} \\ {\mathrm{s.t.}} & {g ^ {i} (\mathbf {x}) \geq 0, i = 1, 2, \ldots , b.} \end{array}\tag{3.5.10}
$$

In other words, since the non-binding constraints are non-binding $\forall \mathbf { x } \in \mathbf { \partial }$ $B _ { \epsilon } \left( \mathbf { x } ^ { * } \right)$ by construction, we can ignore them if we confine our search for a maximum to this neighbourhood. We will return to the non-binding constraints in the very last step of this proof, but until then $g$ will be taken to refer to the vector of b binding constraint functions only and λ to the vector of b Kuhn-Tucker multipliers corresponding to these binding constraints. 

2. We now introduce slack variables $\mathbf { s } \equiv ( s _ { 1 } , . . . , s _ { b } )$ , one corresponding to each binding constraint, and consider the following equality constrained maximisation problem: 

$$
\max _ {\mathbf {x} \in B _ {\epsilon} (\mathbf {x} ^ {*}), \mathbf {s} \in \Re_ {+} ^ {b}} f (\mathbf {x})
$$

Revised: December 2, 1998 

$$
\mathrm{s.t.} \quad G (\mathbf {x}, \mathbf {s}) = \mathbf {0} _ {b}\tag{3.5.11}
$$

where $G ^ { i } \left( \mathbf { x } , \mathbf { s } \right) \equiv g ^ { i } \left( \mathbf { x } \right) - s _ { i } , i = 1 , 2 , \ldots , b .$ 

Since $\mathbf { x } ^ { * }$ solves Problem (3.5.10) and all b constraints in that problem are binding at $\mathbf { x } ^ { * }$ , it can be seen that $\left( \mathbf { x } ^ { * } , \mathbf { 0 } _ { b } \right)$ solves this new problem. For consistency of notation, we define $\mathbf { s } ^ { * } \equiv \mathbf { 0 } _ { b }$ 

3. We proceed with Problem (3.5.11) as in the Lagrange case. In other words, we use the Implicit Function Theorem to solve the system of $\mathit { \Delta } \cdot \mathit { \Delta } b$ equations in $n + b$ unknowns, 

$$
G (\mathbf {x}, \mathbf {s}) = \mathbf {0} _ {b},\tag{3.5.12}
$$

for the first $b$ variables in terms of the last n. To do this, we partition the vector of choice and slack variables three ways: 

$$
(\mathbf {x}, \mathbf {s}) \equiv (\mathbf {y}, \mathbf {z}, \mathbf {s})\tag{3.5.13}
$$

where $\mathbf { y } \in \mathfrak { R } ^ { b }$ and $\mathbf { z } \in \Re ^ { n - b }$ , and correspondingly partition the matrix of partial derivatives evaluated at the optimum: 

$$
G ^ {\prime} \left(\mathbf {y} ^ {*}, \mathbf {z} ^ {*}, \mathbf {s} ^ {*}\right) = G ^ {\prime} \left(\mathbf {x} ^ {*}, \mathbf {s} ^ {*}\right)
$$

$$
= \left( \begin{array}{c c} D _ {\mathbf {y}} G & D _ {\mathbf {z}, \mathbf {s}} G \end{array} \right)\tag{3.5.14}
$$

(3.5.15) 

$$
= \left( \begin{array}{c c c} D _ {\mathbf {y}} G & D _ {\mathbf {z}} G & D _ {\mathbf {s}} G \end{array} \right)\tag{3.5.16}
$$

$$
= \left( \begin{array}{l l l} D _ {\mathbf {y}} g & D _ {\mathbf {z}} g & - \mathbf {I} _ {b} \end{array} \right).\tag{3.5.17}
$$

The rank condition allows us to apply the Implicit Function Theorem and to find a function $h : \mathfrak { R } ^ { n } \longrightarrow \mathfrak { R } ^ { b }$ such that ${ \bf y } = h \left( { \bf z } , { \bf s } \right)$ is a solution to $G \left( \mathbf { y } , \mathbf { z } , \mathbf { s } \right) = \mathbf { 0 }$ with 

$$
h ^ {\prime} (\mathbf {z} ^ {*}, \mathbf {s} ^ {*}) = - (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}, \mathbf {s}} G.\tag{3.5.18}
$$

(3.5.18) can in turn be partitioned to yield 

$$
D _ {\mathbf {z}} h = - \left(D _ {\mathbf {y}} g\right) ^ {- 1} D _ {\mathbf {z}} G = - \left(D _ {\mathbf {y}} g\right) ^ {- 1} D _ {\mathbf {z}} g\tag{3.5.19}
$$

and 

$$
D _ {\mathbf {s}} h = - \left(D _ {\mathbf {y}} g\right) ^ {- 1} D _ {\mathbf {s}} G = \left(D _ {\mathbf {y}} g\right) ^ {- 1} \mathbf {I} _ {b} = \left(D _ {\mathbf {y}} g\right) ^ {- 1}.\tag{3.5.20}
$$

4. This solution can be substituted into the original objective function $f$ to create a new objective function $F$ defined by 

$$
F (\mathbf {z}, \mathbf {s}) \equiv f (h (\mathbf {z}, \mathbf {s}), \mathbf {z})\tag{3.5.21}
$$

and another new maximisation problem where there are only (implicit) nonnegativity constraints: 

$$
\max _ {\mathbf {z} \in B _ {\epsilon} (\mathbf {z} ^ {*}), \mathbf {s} \in \Re_ {+} ^ {b}} F (\mathbf {z}, \mathbf {s})\tag{3.5.22}
$$

It should be clear that $\mathbf { z } ^ { \ast } , \mathbf { 0 } _ { b }$ solves Problem (3.5.22). The first order conditions for Problem (3.5.22) are just that the partial derivatives of $F$ with respect to the remaining $n - b$ choice variables equal zero (according to the first order conditions for unconstrained optimisation), while the partial derivatives of $F$ with respect to the $b$ slack variables must be less than or equal to zero. 

5. The Kuhn-Tucker multipliers can now be found exactly as in the Lagrange case. We know that 

$$
D _ {\mathbf {z}} F = D _ {\mathbf {y}} f D _ {\mathbf {z}} h + D _ {\mathbf {z}} f \mathbf {I} _ {n - b} = \mathbf {0} _ {n - b}.
$$

Substituting for $D _ { \mathbf { z } } h$ from (3.5.19) gives: 

$$
D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}} g = D _ {\mathbf {z}} f.
$$

We can also partition $f ^ { \prime } \left( \mathbf { x } \right)$ as 

$$
\left( \begin{array}{c c} D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {y}} g & D _ {\mathbf {z}} f \end{array} \right)
$$

Substituting for the second sub-matrix yields: 

$$
\begin{array}{r c l} f ^ {\prime} (\mathbf {x}) & = & \left( \begin{array}{c c} D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {y}} g & D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} D _ {\mathbf {z}} g \end{array} \right) \\ & = & D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1} \left( \begin{array}{c c} D _ {\mathbf {y}} g & D _ {\mathbf {z}} g \end{array} \right) \\ & \equiv & - \pmb {\lambda} ^ {\top} g ^ {\prime} (\mathbf {x}) \end{array}
$$

where we define the Kuhn-Tucker multipliers corresponding to the binding constraints, λ , by 

$$
\pmb {\lambda} \equiv - D _ {\mathbf {y}} f (D _ {\mathbf {y}} g) ^ {- 1}.\tag{3.5.23}
$$

6. Next, we calculate the partial derivatives of $F$ with respect to the slack variables and show that they can be less than or equal to zero if and only if the Kuhn-Tucker multipliers corresponding to the binding constraints are greater than or equal to zero. This can be seen by differentiating both sides of (3.5.21) with respect to s to obtain: 

$$
D _ {\mathbf {s}} F = D _ {\mathbf {y}} f D _ {\mathbf {s}} h + D _ {\mathbf {z}} f \mathbf {0} _ {(n - b) \times b}\tag{3.5.24}
$$

$$
{ = } { D _ { \mathbf { y } } f ( D _ { \mathbf { y } } g ) ^ { - 1 } }\tag{3.5.25}
$$

$$
= - \lambda ,\tag{3.5.26}
$$

where we have used (3.5.20) and (3.5.23). 

7. Finally just set the Kuhn-Tucker multipliers corresponding to the non-binding constraints equal to zero. 

Q.E.D. 

Theorem 3.5.2 Second order (sufficient or concavity) conditions for optimisation with inequality constraints. 

$$
I f
$$

1. f and g are differentiable, 

2. $\exists \pmb { \lambda } \in \Re ^ { m }$ such that $f ^ { \prime } \left( \mathbf { x } ^ { * } \right) + \lambda ^ { \top } g ^ { \prime } \left( \mathbf { x } ^ { * } \right) = \mathbf { 0 } ,$ , with $\lambda _ { i } \ge 0 f o r i = 1 , 2 , . . .$ , m and $g ^ { i } ( { \bf x } ^ { * } ) = 0 i f \lambda _ { i } > 0$ (i.e. thefirst order conditions are satisfied at $\mathbf { x } ^ { * } )$ 

3. f is pseudoconcave, and 

4. $g ^ { i } \left( \mathbf { x } ^ { * } \right) = 0 , i = 1 , 2 , \ldots , b ; g ^ { i } \left( \mathbf { x } ^ { * } \right) > 0 , i = b + 1 , \ldots .$ , m and $g ^ { j }$ is quasiconcave $f o r j = 1 , \ldots , b ( i . e .$ the binding constraint functions are quasiconcave), 

then $\mathbf { x } ^ { * }$ solves the constrained maximisation problem. 

Proof The proof just requires the first order conditions to be reduced to 

$$
f ^ {\prime} \left(\mathbf {x} ^ {*}\right) + \sum_ {i = 1} ^ {b} \lambda_ {i} g ^ {i \prime} \left(\mathbf {x} ^ {*}\right) = \mathbf {0}\tag{3.5.27}
$$

from where it is virtually identical to that for the Lagrange case, and so it is left as an exercise. 

Q.E.D. 

## Theorem 3.5.3 Uniqueness conditionfor inequality constrained optimisation. If

1. $\mathbf { x } ^ { * }$ is a solution, 

2. $f$ is strictly quasiconcave, and 

3. $g ^ { j }$ is a quasiconcavefunctionfor $j = 1 , \ldots , m ,$ 

then $\mathbf { x } ^ { * }$ is the unique (global) optimal solution. 

Proof The proof is again similar to that for the Lagrange case and is left as an exercise. The point to note this time is that the feasible set with equality constraints was convex if the constraint functions were affine, whereas the feasible set with inequality constraints is convex if the constraint functions are quasiconcave. This is because the feasible set (where all the inequality constraints are satisfied simultaneously) is the intersection of m upper contour sets of quasiconcave functions, or the intersection of m convex sets. Q.E.D. 

Q.E.D. 

The last important result on optimisation, the Theorem of the Maximum, is closely related to the Envelope Theorem. Before proceeding to the statement of the theorem, the reader may want to review Definition 2.3.12. 

Theorem 3.5.4 (Theorem of the maximum) Consider the modified inequality constrained optimisation problem: 

$$
\max _ {\mathbf {x}} f (\mathbf {x}, \boldsymbol {\alpha}) \quad \text {subject to} \quad g ^ {i} (\mathbf {x}, \boldsymbol {\alpha}) \geq 0, i = 1, \ldots , m\tag{3.5.28}
$$

$$
w h e r e \mathbf {x} \in \Re^ {n}, \boldsymbol {\alpha} \in \Re^ {q}, f: \Re^ {n + q} \rightarrow \Re a n d g: \Re^ {n + q} \rightarrow \Re^ {m}.
$$

Let $\mathbf { x } ^ { * } \left( \alpha \right)$ denote the optimal choice of x for given α $( \mathbf { x } ^ { * } { \mathrm { : } } \Re ^ { q } \ \longrightarrow \ \Re ^ { n } )$ and let M (α) denote the maximum value attainable by f for given α $( M \colon \mathfrak { R } ^ { q }  \mathfrak { R } )$ . If 

1. f is continuous; 

2. the range off is closed and bounded; and 

3. the constraint set is a non-empty, compact-valued, continuous correspondence of α, 

then 

1. M is a continuous (single-valued)function; and 

2. $\mathbf { x } ^ { * }$ is an upper hemi-continuous correspondence, and hence is continuous if it is a continuous (single-valued)function. 

Proof The proof of this theorem is omitted, along with some of the more technical material on continuity of (multi-valued) correspondences. Q.E.D 

Q.E.D. 

Theorem 3.5.4 will be used in consumer theory to prove such critical results as the continuity of demand functions derived from the maximisation of continuous utility functions. 

The following are two frequently encountered examples illustrating the use of the Kuhn-Tucker theorems in economics.<sup>7</sup> 

1. The canonical quadratic programming problem. 

Find the vector $\mathbf { x } \in \Re ^ { n }$ which maximises the value of the quadratic form $\mathbf { x } ^ { \top } \mathbf { A x }$ subject to the m linear inequality constraints $\mathbf { g } ^ { i \top } \mathbf { x } \geq \alpha _ { i }$ , where $\mathbf { A } \in \mathfrak { R } ^ { n \times n }$ is negative definite and $\mathbf { g } ^ { i } \in \Re ^ { n }$ for $i = 1 , \ldots , m$ 

The objective function can always be rewritten as a quadratic form in a symmetric (negative definite) matrixl, since as $\mathbf { x } ^ { \top } \mathbf { A x }$ is a scalar, 

$$
\mathbf {x} ^ {\top} \mathbf {A x} = \left(\mathbf {x} ^ {\top} \mathbf {A x}\right) ^ {\top}\tag{3.5.29}
$$

$$
= \mathbf {x} ^ {\top} \mathbf {A} ^ {\top} \mathbf {x}\tag{3.5.30}
$$

$$
= \frac {1}{2} \left(\mathbf {x} ^ {\top} \mathbf {A x} + \mathbf {x} ^ {\top} \mathbf {A} ^ {\top} \mathbf {x}\right)\tag{3.5.31}
$$

$$
= \mathbf {x} ^ {\top} \left(\frac {1}{2} \left(\mathbf {A} + \mathbf {A} ^ {\top}\right)\right) \mathbf {x}\tag{3.5.32}
$$

and $\begin{array} { r } { { \frac { 1 } { 2 } } \left( \mathbf { A } + \mathbf { A } ^ { \top } \right) } \end{array}$ is always symmetric. 

Let G be the $m \times n$ matrix whose ith row is $\mathbf { g } ^ { i }$ . G must have full rank if we are to apply the Kuhn-Tucker conditions. 

The Lagrangean is: 

$$
\mathbf {x} ^ {\top} \mathbf {A x} + \boldsymbol {\lambda} ^ {\top} (\mathbf {G x} - \boldsymbol {\alpha}).\tag{3.5.33}
$$

The first order conditions are: 

$$
2 \mathbf {x} ^ {\top} \mathbf {A} + \boldsymbol {\lambda} ^ {\top} \mathbf {G} = \mathbf {0} _ {n}\tag{3.5.34}
$$

or, transposing and multiplying across by $\frac { 1 } { 2 } \mathbf { A } ^ { - 1 }$ 

$$
\mathbf {x} = - \frac {1}{2} \mathbf {A} ^ {- 1} \mathbf {G} ^ {\top} \boldsymbol {\lambda}.\tag{3.5.35}
$$

If the constraints are binding, then we will have: 

$$
\boldsymbol {\alpha} = - \frac {1}{2} \mathbf {G A} ^ {- 1} \mathbf {G} ^ {\top} \boldsymbol {\lambda}.\tag{3.5.36}
$$

Now we need the fact that G (and hence $\mathbf { G A } ^ { - 1 } \mathbf { G } ^ { \top } )$ has full rank to solve for the Lagrange multipliers λ: 

$$
\boldsymbol {\lambda} = - 2 \left(\mathbf {G A} ^ {- 1} \mathbf {G} ^ {\top}\right) ^ {- 1} \boldsymbol {\alpha}.\tag{3.5.37}
$$

Now the sign conditions tell us that each component of $\lambda$ must be nonnegative. An easy fix is to let the Kuhn-Tucker multipliers be defined by: 

$$
\boldsymbol {\lambda} ^ {*} \equiv \max \left\{\mathbf {0} _ {m}, - 2 \left(\mathbf {G A} ^ {- 1} \mathbf {G} ^ {\top}\right) ^ {- 1} \boldsymbol {\alpha} \right\},
$$

(3.5.38) 

where the max operator denotes component-by-component maximisation. 

The effect of this is to knock out the non-binding constraints (those with negative Lagrange multipliers) from the original problem and the subsequent analysis. 

We can now find the optimal x by substituting for λ in (3.5.35) the value of $\lambda ^ { * }$ from (3.5.38). 

In the case in which all the constraints are binding, the solution is: 

$$
\mathbf {x} = \mathbf {A} ^ {- 1} \mathbf {G} ^ {\top} \left(\mathbf {G A} ^ {- 1} \mathbf {G} ^ {\top}\right) ^ {- 1} \boldsymbol {\alpha}\tag{3.5.39}
$$

and the envelope function is given by: 

$$
\begin{array}{r c l} \mathbf {x} ^ {\top} \mathbf {A x} & = & \boldsymbol {\alpha} ^ {\top} \left(\mathbf {G A} ^ {- 1} \mathbf {G} ^ {\top}\right) ^ {- 1} \mathbf {G A} ^ {- 1} \mathbf {A A} ^ {- 1} \mathbf {G} ^ {\top} \left(\mathbf {G A} ^ {- 1} \mathbf {G} ^ {\top}\right) ^ {- 1} \boldsymbol {\alpha} \\ & = & \boldsymbol {\alpha} ^ {\top} \left(\mathbf {G A} ^ {- 1} \mathbf {G} ^ {\top}\right) ^ {- 1} \boldsymbol {\alpha} \\ & = & - \frac {1}{2} \boldsymbol {\alpha} ^ {\top} \boldsymbol {\lambda}. \end{array} \tag {3.5}\tag{3.5.40}
$$

The applications of this problem will include ordinary least squares and generalised least squares regression and the mean-variance portfolio choice problem in finance. 

2. Maximising a Cobb-Douglas utility function subject to a budget constraint and non-negativity constraints. 

The applications of this problem will include choice under certainty, choice under uncertainty with log utility where the parameters are reinterpreted as probabilities, the extension to Stone-Geary preferences, and intertemporal choice with log utility, where the parameters are reinterpreted as time discount factors. 

Further exercises consider the duals of each of the forgoing problems, and it is to the question of duality that we will turn in the next section. 

## 3.6 Duality

Let $X \subseteq \mathfrak { R } ^ { n }$ and let $f , g : X \mapsto \Re$ be, respectively, pseudoconcave and pseudoconvex functions. Consider the envelope functions defined by the dual families of problems: 

$$
M (\alpha) \equiv \max _ {\mathbf {x}} f (\mathbf {x}) \text {s.t.} g (\mathbf {x}) \leq \alpha\tag{3.6.1}
$$

Revised: December 2, 1998 

and 

$$
N (\beta) \equiv \min _ {\mathbf {x}} g (\mathbf {x}) \text {s.t.} f (\mathbf {x}) \geq \beta .\tag{3.6.2}
$$

Suppose that these problems have solutions, say $\mathbf { x } ^ { * } \left( \alpha \right)$ and $\mathbf { x } ^ { \dagger } \left( { \boldsymbol { \beta } } \right)$ respectively, and that the constraints bind at these points. 

The first order conditions for the two problems are respectively: 

$$
f ^ {\prime} (\mathbf {x}) - \lambda g ^ {\prime} (\mathbf {x}) = \mathbf {0}\tag{3.6.3}
$$

and 

$$
g ^ {\prime} (\mathbf {x}) + \mu f ^ {\prime} (\mathbf {x}) = \mathbf {0},\tag{3.6.4}
$$

where λ and $\mu$ are the relevant Lagrange multipliers. 

Thus if x and $\lambda ^ { * } \neq 0$ solve (3.6.3), then x and $\mu ^ { * } \equiv - 1 / \lambda$ solve (3.6.4). However, for the x which solves the original problem (3.6.1) to also solve (3.6.2), it must also satisfy the constraint, or $f \left( \mathbf { x } \right) = \beta$ . But we know that $f \left( \mathbf { x } \right) = M \left( \alpha \right)$ . This allows us to conclude that: 

$$
\mathbf {x} ^ {*} (\alpha) = \mathbf {x} ^ {\dagger} (M (\alpha)).\tag{3.6.5}
$$

Similarly, 

$$
\mathbf {x} ^ {\dagger} (\beta) = \mathbf {x} ^ {*} (N (\beta)).\tag{3.6.6}
$$

Combining these equations leads to the conclusion that 

$$
\alpha = N (M (\alpha))\tag{3.6.7}
$$

and 

$$
\beta = M (N (\beta)).\tag{3.6.8}
$$

In other words, the envelope functions for the two dual problems are inverse functions (over any range where the Lagrange multipliers are non-zero, i.e. where the constraints are binding). Thus, either α or $\beta$ or indeed $\lambda$ or $\mu$ can be used to parameterise either family of problems. 

We will see many examples of these principles in the applications in the next part of the book. In particular, duality will be covered further in the context of its applications to consumer theory in Section 4.6. 

Part II APPLICATIONS 

## Chapter 4

# CHOICE UNDER CERTAINTY

## 4.1 Introduction

[To be written.] 

## 4.2 Definitions

There are two possible types of economy which we could analyse: 

• a pure exchange economy, in which households are endowed directly with goods, but there are no firms, there is no production, and economic activity consists solely of pure exchanges of an initial aggregate endowment; and 

• a production economy, in which households are further indirectly endowed with, and can trade, shares in the profit or loss of firms, which can use part of the initial aggregate endowment as inputs to production processes whose outputs are also available for trade and consumption. 

Economies of these types comprise: 

• H households or consumers or agents or (later) investors or, merely, individuals, indexed by the subscript<sup>1</sup> h; 

• N goods or commodities, indexed by the superscript n; and 

• (in the case of a production economy only) F firms, indexed by f. 

This chapter concentrates on the theory of optimal consumer choice and of equilibrium in a pure exchange economy. The theory of optimal production decisions and of equilibrium in an economy with production is mathematically similar. Goods can be distinguished from each other in many ways: 

• obviously, by intrinsic physical characteristics, e.g. apples or oranges. 

• by the time at which they are consumed, $e . g .$ an Easter egg delivered before Easter Sunday or an Easter egg delivered after Easter Sunday. (While all trading takes place simultaneously in the model, consumption can be spread out over many periods.) 

• by the state of the world in which they are consumed, $e . g .$ . the service provided by an umbrella on a wet day or the service which it provides on a dry day. (Typically, the state of the world can be any point $\omega$ in a sample space Ω.) 

The important characteristics of household h are that it is faced with the choice of a consumption vector or consumptionplan or consumption bundle, $\mathbf { x } _ { h } = \left( x _ { h } ^ { 1 } , \ldots , x _ { h } ^ { N } \right) ,$ from a (closed, convex) consumption set, $X _ { h }$ . Typically, $X _ { h } = \Re _ { + } ^ { N }$ . More generally, consumer $h \mathbf { \bar { s } }$ consumption set might require a certain subsistence consumption of some commodities, such as water, and rule out points of $\Re _ { + } ^ { N }$ not meeting this requirement. The household’s endowments are denoted ${ \bf e } _ { h } \in \mathring { \mathfrak { R } } _ { + } ^ { N }$ and can be traded. 

In a production economy, the shareholdings of households in firms are denoted ${ \mathbf c } _ { h } \in \Re ^ { F }$ 

A consumer’s net demand is denoted ${ \bf z } _ { h } \equiv { \bf x } _ { h } - { \bf e } _ { h } \in \Re ^ { N }$ 

Each consumer is assumed to have a preference relation or (weak) preference ordering which is a binary relation on the consumption set $X _ { h } ( ? , \mathbf { C h a p t e r } 7 )$ 

Since each household will have different preferences, we should really denote household $h \mathbf { \bar { s } }$ preference relation $\succeq _ { h }$ , but the subscript will be omitted for the time being while we consider a single household. Similarly, we will assume for the time being that each household chooses from the same consumption set, $x ,$ although this is not essential. 

Recall (see ?) that a binary relation R on X is just a subset R of $\mathcal { X } \times \mathcal { X }$ or a collection of pairs $( x , y )$ where $x \in \mathcal { X }$ and $y \in \mathcal X$ 

If $( x , y ) \in R$ , we usually just write $x R y$ 

Thus $x \succeq y$ means that either x is preferred to y or the consumer is indifferent between the two $( i . e .$ . that x is at least as good as y). 

The following properties of a general relation R on a general set X are often of interest: 

1. A relation R is reflexive ⇐⇒ xRx ∀x ∈ X 

2. A relation R is symmetric ⇐⇒ xRy ⇒ yRx 

3. A relation R is transitive ⇐⇒ xRy, yRz =⇒ xRz 

4. A relation R is complete 

∀x, $y \in X$ either xRy or yRx (or both) (in other words a complete relation orders the whole set) 

An indifference relation, ∼, and a strict preference relation, , can be derived from every preference relation: 

1. x  y means $x \succeq y$ but not $y \succeq x$ 

2. $x \sim y$ means $x \succeq y$ and $y \succeq x .$ 

The utilityfunction $u : \mathcal { X } $ < represents the preference relation $\succeq \mathrm { i f }$ 

$$
u (x) \geq u (y) \iff x \succeq y.
$$

If f: < → < is a monotonic increasing function and u represents the preference relation , then f ◦ u also represents , since 

$$
f (u (x)) \geq f (u (y)) \iff u (x) \geq u (y) \iff x \succeq y.
$$

If X is a countable set, then there exists a utility function representing any preference relation on X. To prove this, just write out the consumption plans in X in order of preference, and assign numbers to them, assigning the same number to any two or more consumption plans between which the consumer is indifferent. If X is an uncountable set, then there may not exist a utility function representing every preference relation on X. 

## 4.3 Axioms

We now consider six axioms which it are frequently assumed to be satisfied by preference relations when considering consumer choice under certainty. (Note that symmetry would not be a very sensible axiom!) Section 5.5.1 will consider further axioms that are often added to simplify the analysis of consumer choice under uncertainty. After the definition of each axiom, we will give a brief rationale for its use. 

Axiom 1 (Completeness) A (weak) preference relation is complete. 

Completeness means that the consumer is never agnostic. 

Axiom 2 (Reflexivity) A (weak) preference relation is reflexive. 

Reflexivity means that each bundle is at least as good as itself. 

Axiom 3 (Transitivity) A (weak) preference relation is transitive. 

Transitivity means that preferences are rational and consistent. 

Axiom 4 (Continuity) The preference relation  is continuous i.e. for all consumption plans $\mathbf { y } \in \mathcal { X }$ the sets $B _ { \mathbf { y } } \equiv \{ \mathbf { x } \in \mathcal { X } : \mathbf { x } \succeq \mathbf { y } \}$ and $W _ { \mathbf { y } } = \{ \mathbf { x } \in \mathcal { X } : \mathbf { y } \succeq$ $\mathbf { x } \}$ are closed sets. 

Consider the picture when $N = 2 \cdot$ 

We will see shortly that $B _ { \mathbf { y } }$ , the set of consumption plans which are better than or as good as ${ \bf y } ,$ and $W _ { \mathbf { y } }$ , the set of consumption plans which are worse than or as good as $\mathbf { y } ,$ are just the upper contour sets and lower contour sets respectively of utility functions, if such exist. 

E.g. consider lexicographic preferences: 

Lexicographic preferences violate the continuity axiom. A consumer with such preference prefers more of commodity 1 regardless of the quantities of other commodities, more of commodity 2 if faced with a choice between two consumption plans having the same amount of commodity 1, and so on. 

In the picture, the consumption plan y lies in the lower contour set $W _ { \mathbf { x } ^ { * } }$ but $B \boldsymbol { \epsilon } \left( \mathbf { y } \right)$ never lies completely in $W _ { \mathbf { x } }$ ∗ for any . Thus, lower contour sets are not open, and upper contour sets are not closed. 

Theorems on the existence of continuous utility functions have been proven by Gerard Debreu, Nobel laureate, whose proof used Axioms 1–4 only (see ? or ?) and by Hal Varian, whose proof was simpler by virtue of adding an additional axiom (see ?). 

Theorem 4.3.1 (Debreu) If X is a closed and convex set and  is a complete, reflexive, transitive and continuous preference relation on $\mathcal { X } ,$ , then ∃ a continuous utilityfunction $u \colon \mathcal { X }  \mathfrak { R }$ representing . 

Proof For the proof of this theorem, see ?. 

Q.E.D. 

Axiom 5 (Greed) Greed is incorporated into consumer behaviour by assuming either 

1. Strong monotonicity: 

$I f \mathcal { X } = \Re _ { + } ^ { N }$ , then  is said to be strongly monotonic iffwhenever $x _ { n } \geq y _ { n } \forall n$ but $\mathbf { x } \neq \mathbf { y } , \mathbf { x } \succ \mathbf { y . } \ I \mathbf { x } = ( x _ { 1 } , \ldots , x _ { N } ) \ \& c . J ;$ or 

2. Local non-satiation: 

$$
\forall \mathbf {x} \in \mathcal {X}, \epsilon > 0, \exists \mathbf {x} ^ {\prime} \in B \epsilon (\mathbf {x}) s. t. \mathbf {x} ^ {\prime} \succ \mathbf {x}
$$

The strong monotonicity axiom is a much stronger restriction on preferences than local non-satiation; however, it greatly simplifies the proof of existence of utility functions. 

We will prove the existence, but not the continuity, part of the following weaker theorem. 

Theorem 4.3.2 (Varian) If $\mathscr { X } = \Re _ { + } ^ { N }$ and $\succeq i s$ a complete, reflexive, transitive, continuous and strongly monotonic preference relation on $x ,$ , then $\exists a$ continuous utilityfunction u: $\mathcal X  \Re$ representing . 

Proof (of existence only $( ? , { \mathfrak { p } } . 9 7 ) ,$ ) 

Pick a benchmark consumption plan, $\boldsymbol { e } . \boldsymbol { g } . \ \mathbf { 1 } \equiv ( 1 , 1 , \dots , 1 )$ 

The idea is that the utility of x is the multiple of the benchmark consumption plan to which x is indifferent. 

By strong monotonicity, the sets $\{ t \in \Re : t { \bf 1 } \succeq { \bf x } \}$ and $\{ t \in \mathfrak { R } : \mathbf { x } \succeq t \mathbf { 1 } \}$ are both non-empty. 

By continuity of preferences, both are closed (intersection of a ray through the origin and a closed set); and by completeness, they cover <. 

By connectedness of $\Re ,$ they intersect in at least one point, $u ( { \bf x } )$ say, and $\mathbf { x } \sim$ $u ( { \bf x } ) { \bf 1 }$ 

Now 

$$
\begin{array}{r c l} \mathbf {x} \succeq \mathbf {y} & \Longleftrightarrow & u (\mathbf {x}) \mathbf {1} \succeq u (\mathbf {y}) \mathbf {1} \\ & \Longleftrightarrow & u (\mathbf {x}) \geq u (\mathbf {y}) \end{array}
$$

where the first equivalence follows from transitivity of preferences and the second from strong monotonicity. 

The assumption that preferences are reflexive is not used in establishing existence of the utility function, so it can be inferred that it is required to establish continuity. 

Q.E.D. 

The rule which the consumer will follow is to choose the most preferred bundle from the set of affordable alternatives (budget set), in other words the bundle at which the utility function is maximised subject to the budget constraint, if one exists. 

We know that an optimal choice will exist if the utility function is continuous and the budget set is closed and bounded. 

If the utility function is differentiable, we can go further and use calculus to find the maximum. 

So we usually assume differentiability. 

If u is a concave utility function, then $f \circ u .$ , which also represents the same preferences, is not necessarily a concave function (unless f itself is a convex function). In other words, concavity of a utility function is a property of the particular representation and not of the underlying preferences. Notwithstanding this, convexity of preferences is important, as indicated by the use of one or other of the following axioms, each of which relates to the preference relation itself and not to the particular utility function chosen to represent it. 

Axiom 6 (Convexity) There are two versions ofthis axiom: 

1. Convexity: 

The preference relation $\succeq i s$ convex $\Longleftrightarrow$ 

$$
\mathbf {x} \succeq \mathbf {y} \Longrightarrow \lambda \mathbf {x} + (1 - \lambda) \mathbf {y} \succeq \mathbf {y}.
$$

2. Strict convexity: 

The preference relation $\succeq i s$ strictly convex $\Longleftrightarrow$ 

$$
\mathbf {x} \succeq \mathbf {y} \Longrightarrow \lambda \mathbf {x} + (1 - \lambda) \mathbf {y} \succ \mathbf {y}.
$$

The difference between the two versions of the convexity axiom basically amounts to ruling out linear segments in indifference curves in the strict case. 

Theorem 4.3.3 The preference relation $\mathbf { \xi } \succeq i s \left( s t r i c t l y \right)$ convex if and only if every utilityfunction representing  is a (strictly) quasiconcavefunction. 

Proof In either case, both statements are equivalent to saying that 

$$
u (\mathbf {x}) \geq u (\mathbf {y}) \Longrightarrow u (\lambda \mathbf {x} + (1 - \lambda) \mathbf {y}) \geq (>) u (\mathbf {y}).\tag{4.3.1}
$$

Revised: December 2, 1998 

Q.E.D. 

Theorem 4.3.4 All upper contour sets of a utility function representing convex preferences are convex sets (i.e. indifference curves are convex to the origin for convex preferences). 

It can be seen that convexity of preferences is a generalisation of the two-good assumption of a diminishing marginal rate of substitution. 

Axiom 7 (Inada Condition) This axiom seems to be relegated to some other category in many existing texts and its attribution to Inada is also difficult to trace. It is not easy to see how to express it in terms of the underlying preference relation so perhaps it cannot be elevated to the status ofan axiom. Should it be expressed as: 

$$
\lim _ {x _ {i} \to 0} \frac {\partial u}{\partial x _ {i}} = \infty
$$

or as 

$$
\lim _ {x _ {i} \to \infty} \frac {\partial u}{\partial x _ {i}} = 0?
$$

The Inada condition will be required to rule out corner solutions in the consumer’s problem. Intuitively, it just says that indifference curves may be asymptotic to the axes but never reach them. 

## 4.4 Optimal Response Functions: Marshallian and Hicksian Demand

## 4.4.1 The consumer’s problem

A consumer with consumption set $X _ { h }$ , endowment vector $\mathbf { e } _ { h } \in X _ { h } .$ , shareholdings ${ \mathbf c } _ { h } \in \Re ^ { F }$ and preference ordering $\succeq _ { h }$ represented by utility function $u _ { h }$ who desires to trade his endowment at prices $ { \mathbf { p } } \in \Re _ { + } ^ { N }$ faces an inequality constrained optimisation problem: 

$$
\max _ {\mathbf {x} \in X _ {h}} u _ {h} (\mathbf {x}) \mathrm{s.t.} \mathbf {p} ^ {\top} \mathbf {x} \leq \mathbf {p} ^ {\top} \mathbf {e} _ {h} + \mathbf {c} _ {h} ^ {\top} \boldsymbol {\Pi} (\mathbf {p}) \equiv M _ {h}\tag{4.4.1}
$$

where Π (p) is the vector of the F firms’ maximised profits when prices are p. Constraining x to lie in the consumption set normally just means imposing nonnegativity constraints on the problem. From a mathematical point of view, the source of income is irrelevant, and in particular the distinction between pure exchange and production economy is irrelevant. Thus, income can be represented by M in either case. 

Since the constraint functions are linear in the choice variables x, the Kuhn-Tucker theorem on second order conditions (Theorem 3.5.2) can be applied, provided that the utility function $u _ { h }$ is pseudo-concave. In this case, the first order conditions identify a maximum. 

The Lagrangian, using multipliers λ for the budget constraint and $\pmb { \mu } \in \Re ^ { N }$ for the non-negativity constraints, is 

$$
u _ {h} (\mathbf {x}) + \lambda (M - \mathbf {p} ^ {\top} \mathbf {x}) + \boldsymbol {\mu} ^ {\top} \mathbf {x}.\tag{4.4.2}
$$

The first order conditions are given by the (N-dimensional) vector equation: 

$$
u _ {h} ^ {\prime} (\mathbf {x}) + \lambda (- \mathbf {p}) + \boldsymbol {\mu} = \mathbf {0} _ {N}\tag{4.4.3}
$$

and the sign condition $\lambda \geq 0$ with $\lambda > 0$ if the budget constraint is binding. We also have $\pmb { \mu } = \mathbf { 0 } _ { N }$ unless one of the non-negativity constraints is binding: Axiom 7 would rule out this possibility. 

Now for each $\mathbf { p } \in \Re _ { + + } ^ { N }$ (ruling out bads, or goods with negative prices, and even (see below) free goods), $\mathbf { e } _ { h } \in X _ { h }$ , and ${ \mathbf c } _ { h } \in \Re ^ { F }$ , or for each $\mathbf { p } , M _ { h }$ combination, there is a corresponding solution to the consumer’s utility maximisation problem, denoted $\mathbf { x } _ { h } \left( \mathbf { p } , \mathbf { e } _ { h } , \mathbf { c } _ { h } \right)$ or ${ \bf x } _ { h } \left( { \bf p } , M _ { h } \right)$ . The function (correspondence) $\mathbf { x } _ { h }$ is often called a Marshallian demand function (correspondence). 

If the utility function $u _ { h }$ is also strictly quasiconcave (i.e. preferences are strictly convex), then the conditions of the Kuhn-Tucker theorem on uniqueness (Theorem 3.5.3) are satisfied. In this case, the consumer’s problem has a unique solution for given prices and income, so that the optimal response correspondence is a single-valued demand function. On the other hand, the weak form of the convexity axiom would permit a multi-valued demand correspondence. 

## 4.4.2 The No Arbitrage Principle

Definition 4.4.1 An arbitrage opportunity means the opportunity to acquire a consumption vector or its constituents, directly or indirectly, at one price, and to sell the same consumption vector or its constituents, directly or indirectly, at a higher price. 

Theorem 4.4.1 (The No Arbitrage Principle) Arbitrage opportunities do not exist in equilibrium in an economy in which at least one agent has preferences which exhibit local non-satiation.<sup>2</sup> 

Proof If preferences exhibit local non-satiation, then Marshallian demand is not well-defined if the price vector permits arbitrage opportunities. 

If the no arbitrage principle doesn’t hold, then any individual can increase wealth without bound by exploiting the available arbitrage opportunity on an infinite scale. Thus there is no longer a budget constraint and, since local non-satiation rules out bliss points, utility too can be increased without bound. 

When we come to consider equilibrium, we will see that if even one individual has preferences exhibiting local non-satiation, then equilibrium prices can not permit arbitrage opportunities. 

Q.E.D. 

Examples are usually in the financial markets, in a multi-period context, e.g. covered interest parity, term structure of interest rates, $\& c .$ . The most powerful application is in the derivation of option-pricing formulae, since options can be shown to be identical to various synthetic portfolios made up of the underlying security and the riskfree security. 

The simple rule for figuring out how to exploit arbitrage opportunities is ‘buy low, sell high’. With interest rates and currencies, for example, this may be a non-trivial calculation. 

Exercise: If the interest rate for one-year deposits or loans is $r _ { 1 }$ per annum compounded annually, the interest rate for two-year deposits or loans is $r _ { 2 }$ per annum compounded annually and the forward interest rate for one year deposits or loans beginning in one year’s time is $f _ { 1 2 }$ per annum compounded annually, calculate the relationship that must hold between these three rates if there are to be no arbitrage opportunities. 

Solution: $\left( 1 + r _ { 1 } \right) \left( 1 + f _ { 1 2 } \right) = \left( 1 + r _ { 2 } \right) ^ { 2 }$ 

## 4.4.3 Other Properties of Marshallian demand

Other noteworthy properties of Marshallian demand include the following: 

1. If preferences exhibit local non-satiation, then the budget constraint is binding. 

This is because no consumption vector in the interior of the budget set can maximise utility as some nearby consumption vector will always be both preferred and affordable. At the optimum, on the budget hyperplane, the nearby consumption vector which is preferred will not be affordable. 

2. If p includes a zero price $( p ^ { n } = 0$ for some n), then ${ \bf x } _ { h } \left( { \bf p } , M _ { h } \right)$ may not be well defined. 

This is because, at least in the case of strongly monotonic preferences, the consumer will seek to acquire and consume an infinite amount of the free good, thereby increasing utility without bound. For this reason, it is neater to define Marshallian demand only on the open non-negative orthant in $\Re ^ { N }$ namely $\Re _ { + + } ^ { N }$ 

3. The demand ${ \bf x } _ { h } \left( { \bf p } , M _ { h } \right)$ is independent of the representation $u _ { h }$ of the underlying preference relation $\succeq _ { h }$ which is used in the statement of the consumer’s problem. 

4. ${ \bf x } _ { h } \left( { \bf p } , M _ { h } \right)$ is homogenous of degree 0 in $\mathbf { p } , M _ { h }$ 

In other words, if all prices and income are multiplied by $\alpha > 0$ , then demand does not change: 

$$
\mathbf {x} _ {h} \left(\alpha \mathbf {p}, \alpha M _ {h}\right) = \mathbf {x} _ {h} \left(\mathbf {p}, M _ {h}\right).\tag{4.4.4}
$$

5. Demand functions are continuous. 

This follows from the theorem of the maximum (Theorem 3.5.4). It follows that small changes in prices or income will lead to small changes in quantities demanded. 

## 4.4.4 The dual problem

Consider also the (dual) expenditure minimisation problem: 

$$
\min _ {\mathbf {x}} \mathbf {p} ^ {\top} \mathbf {x} s. t. u _ {h} (\mathbf {x}) \geq \bar {u}.\tag{4.4.5}
$$

In other words, what happens if expenditure is minimised subject to a certain level of utility, u¯, being attained? 

The solution (optimal response function) is called the Hicksian or compensated demand function (or correspondence) and is usually denoted $\mathbf { h } _ { h } \left( \mathbf { p } , \bar { u } \right)$ 

There should really be a more general discussion of duality, based on the meanvariance problem as well as the utility maximisation/expenditure minimisation problems. 

If the local non-satiation axiom holds, then the constraints are binding in both the utility-maximisation and expenditure-minimisation problems, and we have a number of duality relations. In particular, there will be a one-to-one correspondence between income M and utility u¯ for a given price vector p. The expenditure function and the indirect utility function will then act as a pair of inverse envelope functions mapping utility levels to income levels and vice versa respectively. 

A full page table setting out exactly the parallels between the two problems is called for here. 

The following duality relations (or fundamental identities as ? calls them) will prove extremely useful later on: 

$$
e (\mathbf {p}, v (\mathbf {p}, M)) = M\tag{4.4.6}
$$

$$
{v (\mathbf {p}, e (\mathbf {p}, \bar {u}))} = {\bar {u}}\tag{4.4.7}
$$

$$
\mathbf {x} (\mathbf {p}, M) = \mathbf {h} (\mathbf {p}, v (\mathbf {p}, M))\tag{4.4.8}
$$

$$
\mathbf {h} (\mathbf {p}, \bar {u}) = \mathbf {x} (\mathbf {p}, e (\mathbf {p}, \bar {u}))\tag{4.4.9}
$$

These are just equations (3.6.5)–(3.6.8) adapted to the notation of the consumer’s problem. 

## 4.4.5 Properties of Hicksian demands

As in the Marshallian approach, if preferences are strictly convex, then any solution to the expenditure minimisation problem is unique and the Hicksian demands are well-defined single valued functions. 

It’s worth going back to the uniqueness proof with this added interpretation. If two different consumption vectors minimise expenditure, then they both cost the same amount, and any convex combination of the two also costs the same amount. But by strict convexity, a convex combination yields higher utility, and nearby there must, by continuity, be a cheaper consumption vector still yielding utility u¯. 

If preferences are not strictly convex, then Hicksian demands may be correspondences rather than functions. 

Hicksian demands are homogenous of degree 0 in prices: 

$$
\mathbf {h} _ {h} \left(\alpha \mathbf {p}, \bar {u}\right) = \mathbf {h} _ {h} \left(\mathbf {p}, \bar {u}\right).\tag{4.4.10}
$$

## 4.5 Envelope Functions: Indirect Utility and Expenditure

Now consider the envelope functions corresponding to the two approaches: 

1. The indirect utility function: 

$$
v _ {h} (\mathbf {p}, M) \equiv u _ {h} (\mathbf {x} _ {h} (\mathbf {p}, M))\tag{4.5.1}
$$

2. The expenditure function: 

$$
e _ {h} \left(\mathbf {p}, \bar {u}\right) \equiv \mathbf {p} ^ {\top} \mathbf {h} _ {h} \left(\mathbf {p}, \bar {u}\right).\tag{4.5.2}
$$

Sometimes we meet two other related functions: 

3. The money metric utility function 

$$
m _ {h} \left(\mathbf {p}, \mathbf {x}\right) \equiv e _ {h} \left(\mathbf {p}, u _ {h} \left(\mathbf {x}\right)\right)\tag{4.5.3}
$$

is the (least) cost at prices p of being as well off as with the consumption vector x. 

4. The money metric indirect utility function 

$$
\mu_ {h} (\mathbf {p}; \mathbf {q}, M) \equiv e _ {h} (\mathbf {p}, v _ {h} (\mathbf {q}, M))\tag{4.5.4}
$$

is the (least) cost at prices p of being as well off as if prices were q and income was M. 

The following are interesting properties of the indirect utility function: 

1. By the Theorem of the Maximum, the indirect utility function is continuous for positive prices and income. 

2. The indirect utility function is non-increasing in p and non-decreasing in $M .$ 

3. The indirect utility function is quasi-convex in prices. 

To see this, let $B \left( \mathbf { p } \right)$ denote the budget set when prices are p and let $\mathbf { p } \lambda \equiv$ $\lambda \mathbf { p } + \left( { 1 - \lambda } \right) \mathbf { p } ^ { \prime }$ 

Then $B \left( \mathbf { p } \lambda \right) \subseteq \left( B \left( \mathbf { p } \right) \cup B \left( \mathbf { p } ^ { \prime } \right) \right)$ 

Suppose this was not the case, i.e. for some x, $\mathbf { p } \lambda ^ { \top } \mathbf { x } \leq M$ but $\mathbf { p } ^ { \intercal } \mathbf { x } >$ M and $\mathbf { p } ^ { \prime \top } \mathbf { x } > M$ . Then taking a convex combination of the last two inequalities yields 

$$
\lambda \mathbf {p} ^ {\top} \mathbf {x} + (1 - \lambda) \mathbf {p} ^ {\prime \top} \mathbf {x} > M,
$$

which contradicts the first inequality. 

It follows that the maximum value of $u _ { h } \left( \mathbf { x } \right)$ on the subset $B \left( \mathbf { p } \lambda \right)$ is less than or equal to its maximum value on the superset $B \left( \mathbf { p } \right) \cup B \left( \mathbf { p } ^ { \prime } \right)$ 

In terms of the indirect utility function, this says that 

$$
v _ {h} \left(\mathbf {p} \lambda , M\right) \leq \max \left\{v _ {h} \left(\mathbf {p}, M\right), v _ {h} \left(\mathbf {p} ^ {\prime}, M\right) \right\},
$$

or that $v _ { h }$ is quasiconvex. 

4. $v _ { h } \left( \mathbf { p } , M \right)$ is homogenous of degree zero in $\mathbf { p } , M .$ , or 

$$
v _ {h} (\lambda \mathbf {p}, \lambda M) = v _ {h} (\mathbf {p}, M).
$$

The following are interesting properties of the expenditure function: 

1. The expenditure function is continuous. 

2. The expenditure function itself is non-decreasing in prices, since raising the price of one good while holding the prices of all other goods constant can not reduce the minimum cost of attaining a fixed utility level. 

3. The expenditure function is concave in prices. 

To see this, we just fix two price vectors p and $\mathbf { p } ^ { \prime }$ and consider the value of the expenditure function at the convex combination $\mathbf { p } \lambda \equiv \lambda \mathbf { p } + \left( 1 - \lambda \right) \mathbf { p } ^ { \prime }$ 

$$
e (\mathbf {p} \lambda , \bar {u}) = (\mathbf {p} \lambda) ^ {\top} \mathbf {h} (\mathbf {p} \lambda , \bar {u})\tag{4.5.5}
$$

$$
= \lambda \mathbf {p} ^ {\top} \mathbf {h} (\mathbf {p} \lambda , \bar {u}) + (1 - \lambda) (\mathbf {p} ^ {\prime}) ^ {\top} \mathbf {h} (\mathbf {p} \lambda , \bar {u})\tag{4.5.6}
$$

$$
\geq \lambda \mathbf {p} ^ {\top} \mathbf {h} (\mathbf {p}, \bar {u}) + (1 - \lambda) (\mathbf {p} ^ {\prime}) ^ {\top} \mathbf {h} (\mathbf {p} ^ {\prime}, \bar {u})\tag{4.5.7}
$$

$$
= \lambda e (\mathbf {p}, \bar {u}) + (1 - \lambda) e \left(\mathbf {p} ^ {\prime}, \bar {u}\right),\tag{4.5.8}
$$

where the inequality follows because the cost of a suboptimal bundle for the given prices must be greater than the cost of the optimal (expenditureminimising) consumption vector for those prices. 

4. The expenditure function is homogenous of degree 1 in prices: 

$$
e _ {h} (\alpha \mathbf {p}, \bar {u}) = \alpha e _ {h} (\mathbf {p}, \bar {u}).\tag{4.5.9}
$$

## 4.6 Further Results in Demand Theory

In this section, we present four important theorems on demand functions and the corresponding envelope functions. Shephard’s Lemma will allow us to recover Hicksian demands from the expenditure function. Similarly, Roy’s Identity will allow us to recover Marshallian demands from the indirect utility function. The Slutsky symmetry condition and the Slutsky equation provide further insights into the properties of consumer demand. 

Theorem 4.6.1 (Shephard’s Lemma.) 

$$
\frac {\partial e _ {h}}{\partial p ^ {n}} (\mathbf {p}, \bar {u}) = \frac {\partial}{\partial p ^ {n}} \left(\mathbf {p} ^ {\top} \mathbf {x} + \lambda (u _ {h} (\mathbf {x}) - \bar {u})\right)\tag{4.6.1}
$$

$$
= x ^ {n}\tag{4.6.2}
$$

which, when evaluated at the optimum, is just $ { \mathbf { h } } _ { h } ^ { n } \left(  { \mathbf { p } } , \bar { u } \right)$ 

In other words, the partial derivatives of the expenditure function with respect to prices are the corresponding Hicksian demandfunctions. 

Proof $\mathtt { B y }$ differentiating the expenditure function with respect to the price of good n and applying the envelope theorem (Theorem 3.4.4), we obtain Shephard’s Lemma: 

(To apply the envelope theorem, we should be dealing with an equality constrained optimisation problem; however, if we assume local non-satiation, we know that the budget constraint or utility constraint will always be binding, and so the inequality constrained expenditure minimisation problem is essentially and equality constrained problem.) 

Q.E.D. 

Theorem 4.6.2 (Roy’s Identity.) Marshallian demands may be recovered from the indirect utility function using: 

$$
\mathbf {x} ^ {n} (\mathbf {p}, M) = - \frac {\frac {\partial v}{\partial p ^ {n}} (\mathbf {p} , M)}{\frac {\partial v}{\partial M} (\mathbf {p} , M)}.\tag{4.6.3}
$$

Proof For Roy’s Identity, see ?. 

It is obtained by differentiating equation (4.4.7) with respect to $p ^ { n }$ , using the Chain Rule: 

$$
v \left(\mathbf {p}, e \left(\mathbf {p}, \bar {u}\right)\right) = \bar {u}
$$

implies that 

$$
\frac {\partial v}{\partial p ^ {n}} (\mathbf {p}, e (\mathbf {p}, \bar {u})) + \frac {\partial v}{\partial M} (\mathbf {p}, e (\mathbf {p}, \bar {u})) \frac {\partial e}{\partial p ^ {n}} (\mathbf {p}, \bar {u}) = 0\tag{4.6.4}
$$

and using Shephard’s Lemma gives: 

$$
\frac {\partial v}{\partial p ^ {n}} \left(\mathbf {p}, e \left(\mathbf {p}, \bar {u}\right)\right) + \frac {\partial v}{\partial M} \left(\mathbf {p}, e \left(\mathbf {p}, \bar {u}\right)\right) \mathbf {h} ^ {n} \left(\mathbf {p}, \bar {u}\right) = 0\tag{4.6.5}
$$

Hence 

$$
\mathbf {h} ^ {n} (\mathbf {p}, \bar {u}) = - \frac {\frac {\partial v}{\partial p ^ {n}} (\mathbf {p} , e (\mathbf {p} , \bar {u}))}{\frac {\partial v}{\partial M} (\mathbf {p} , e (\mathbf {p} , \bar {u}))}\tag{4.6.6}
$$

and expressing this last equation in terms of the relevant level of income M rather than the corresponding value of utility u¯: 

$$
\mathbf {x} ^ {n} (\mathbf {p}, M) = - \frac {\frac {\partial v}{\partial p ^ {n}} (\mathbf {p} , M)}{\frac {\partial v}{\partial M} (\mathbf {p} , M)}.\tag{4.6.7}
$$

Q.E.D. 

Theorem 4.6.3 (Slutsky symmetry condition.) All cross-price substitution effects are symmetric: 

$$
\frac {\partial h _ {h} ^ {n}}{\partial p ^ {m}} = \frac {\partial h _ {h} ^ {m}}{\partial p ^ {n}}.\tag{4.6.8}
$$

Proof From Shephard’s Lemma, we can easily derive the Slutsky symmetry conditions, assuming that the expenditure function is twice continuously differentiable, and hence that 22 22 

$$
\frac {\partial^ {2} e _ {h}}{\partial p ^ {m} \partial p ^ {n}} = \frac {\partial^ {2} e _ {h}}{\partial p ^ {n} \partial p ^ {m}}.\tag{4.6.9}
$$

Since $\begin{array} { r } { h _ { h } ^ { m } = \frac { \partial e _ { h } } { \partial p ^ { m } } } \end{array}$ and $\begin{array} { r } { h _ { h } ^ { n } = \frac { \partial e _ { h } } { \partial p ^ { n } } } \end{array}$ , and the result follows. 

Q.E.D. 

The next result doesn’t really have a special name of its own. 

Theorem 4.6.4 Since the expenditurefunction is concave in prices (see p. 75), the corresponding Hessian matrix is negative semi-definite. In particular, its diagonal entries are non-positive, or 

$$
\frac {\partial^ {2} e _ {h}}{\partial (p ^ {n}) ^ {2}} \leq 0, \quad n = 1, \ldots , N.\tag{4.6.10}
$$

Using Shephard’s Lemma, itfollows that 

$$
\frac {\partial h _ {h} ^ {n}}{\partial p ^ {n}} \leq 0, \quad n = 1, \dots , N.\tag{4.6.11}
$$

In other words, Hicksian demandfunctions, unlike Marshallian demandfunctions, are uniformly decreasing in own price. Another way of saying this is that own price substitution effects are always negative. 

Theorem 4.6.5 (Slutsky equation.) The total effect of a price change on (Marshallian) demand can be decomposed as follows into a substitution effect and an income effect: 

$$
\frac {\partial x ^ {m}}{\partial p ^ {n}} (\mathbf {p}, M) = \frac {\partial h ^ {m}}{\partial p ^ {n}} (\mathbf {p}, \bar {u}) - \frac {\partial x ^ {m}}{\partial M} (\mathbf {p}, M) \mathbf {h} ^ {n} (\mathbf {p}, \bar {u}),\tag{4.6.12}
$$

where ${ \bar { u } } \equiv V \left( \mathbf { p } , { \cal M } \right)$ . 

Before proving this, let’s consider the signs of the various terms in the Slutsky equation and look at what it means in a two-good example. 

By Theorem 4.6.4, we know that own price substitution effects are always nonpositive. 

[This is still on a handwritten sheet.] 

Proof Differentiating both sides of the lth component of (4.4.9) with respect to $p ^ { n }$ , using the Chain Rule, will yield the so-called Slutsky equation which decomposes the total effect on demand of a price change into an income effect and a substitution effect. 

Differentiating the RHS of (4.4.9) with respect to $p ^ { n }$ yields: 

$$
\frac {\partial x ^ {m}}{\partial p ^ {n}} \left(\mathbf {p}, e \left(\mathbf {p}, \bar {u}\right)\right) + \frac {\partial x ^ {m}}{\partial M} \left(\mathbf {p}, e \left(\mathbf {p}, \bar {u}\right)\right) \frac {\partial e}{\partial p ^ {n}} \left(\mathbf {p}, \bar {u}\right).\tag{4.6.13}
$$

To complete the proof: 

1. set this equal to $\frac { \partial h ^ { m } } { \partial p ^ { n } } \left( \mathbf { p } , \bar { u } \right)$ 

2. substitute from Shephard’s Lemma 

3. define $M \equiv e \left( \mathbf { p } , \bar { u } \right)$ (which implies that $\bar { u } \equiv V \left( \mathbf { p } , M \right) )$ 

Q.E.D. 

## 4.7 General Equilibrium Theory

## 4.7.1 Walras’ law

Walras . . . <sup>3</sup> 

## 4.7.2 Brouwer’s fixed point theorem

## 4.7.3 Existence of equilibrium

## 4.8 The Welfare Theorems

## 4.8.1 The Edgeworth box

## 4.8.2 Pareto efficiency

Definition 4.8.1 A feasible allocation $\mathbf { X } \ = \ \left( \mathbf { x } _ { 1 } , \ldots \ldots , \mathbf { x } _ { H } \right)$ is Pareto efficient if there does not exist any feasible way of reallocating the same initial aggregate endowment, $\textstyle \sum _ { h = 1 } ^ { H } \mathbf { x } _ { h }$ , which makes one individual better off without making any other worse off. 

Definition 4.8.2 X is Pareto dominated by ${ \bf X } ^ { \prime } ~ = ~ ( { \bf x } _ { 1 } ^ { \prime } , \ldots , { \bf x } _ { H } ^ { \prime } ) ~ i f \sum _ { h = 1 } ^ { H } { \bf x } _ { h } ~ =$ $\begin{array} { r } { \sum _ { h = 1 } ^ { H } \mathbf { x } _ { h } ^ { \prime } , \mathbf { x } _ { h } ^ { \prime } \succeq _ { h } \mathbf { x } _ { h } } \end{array}$ ∀h and $\mathbf { x } _ { h } ^ { \prime } \succ _ { h } \mathbf { x } _ { h } f o r$ at least one h. 

## 4.8.3 The First Welfare Theorem

(See ?.) 

Theorem 4.8.1 (First Welfare Theorem) Ifthe pair $( \mathbf { p } , \mathbf { X } )$ is an equilibrium $( f o r$ given preferences, $\succeq _ { h } ,$ , which exibit local non-satiation and given endowments, $\mathbf { e } _ { h }$ $h = 1 , \ldots , H )$ , then X is a Pareto efficient allocation. 

Proof The proof is by contradiction. Suppose that X is an equilibrium allocation which is Pareto dominated by a feasible allocation $\mathbf { X } ^ { \prime }$ 

If individual $h$ is strictly better off under $\mathbf { X } ^ { \prime }$ or $\mathbf { x } _ { h } ^ { \prime } \succ _ { h } \mathbf { x } _ { h }$ , then it follows that individual $h$ cannot afford $\mathbf { x } _ { h } ^ { \prime }$ at the equilibrium prices p or 

$$
\mathbf {p} ^ {\top} \mathbf {x} _ {h} ^ {\prime} > \mathbf {p} ^ {\top} \mathbf {x} _ {h} = \mathbf {p} ^ {\top} \mathbf {e} _ {h}.\tag{4.8.1}
$$

The latter equality is just the budget constraint, which is binding since we have assumed local non-satiation. 

Similarly, if individual h is indifferent between $\mathbf { X }$ and $\mathbf { X } ^ { \prime }$ or $\mathbf { x } _ { h } ^ { \prime } \sim _ { h } \mathbf { x } _ { h }$ , then it follows that 

$$
\mathbf {p} ^ {\top} \mathbf {x} _ {h} ^ {\prime} \geq \mathbf {p} ^ {\top} \mathbf {x} _ {h} = \mathbf {p} ^ {\top} \mathbf {e} _ {h},\tag{4.8.2}
$$

since if ${ \bf x } _ { h } ^ { \prime }$ cost strictly less than $\mathbf { x } _ { h }$ , then by local non-satiation some consumption vector near enough to $\mathbf { x } _ { h } ^ { \prime }$ to also cost less than $\mathbf { x } _ { h }$ would be strictly preferred to $\mathbf { x } _ { h }$ and $\mathbf { x } _ { h }$ would not maximise utility given the budget constraint. 

Summing (4.8.1) and (4.8.2) over households yields 

$$
\mathbf {p} ^ {\top} \sum_ {h = 1} ^ {H} \mathbf {x} _ {h} ^ {\prime} > \mathbf {p} ^ {\top} \sum_ {h = 1} ^ {H} \mathbf {x} _ {h} = \mathbf {p} ^ {\top} \sum_ {h = 1} ^ {H} \mathbf {e} _ {h},\tag{4.8.3}
$$

(where the equality is essentially Walras’ Law). 

But since X<sup>0</sup> is feasible we must have for each good n 

$$
\sum_ {h = 1} ^ {H} x _ {h} ^ {\prime n} \leq \sum_ {h = 1} ^ {H} e _ {h} ^ {n}
$$

and, hence, multiplying by prices and summing over all goods, 

$$
\mathbf {p} ^ {\top} \sum_ {h = 1} ^ {H} \mathbf {x} _ {h} ^ {\prime} \leq \mathbf {p} ^ {\top} \sum_ {h = 1} ^ {H} \mathbf {e} _ {h}.\tag{4.8.4}
$$

But (4.8.4) contradicts the inequality in (4.8.3), so no such Pareto dominant allocation $\mathbf { X } _ { h } ^ { \prime }$ can exist. 

Q.E.D. 

Before proceeding to the second welfare theorem, we need to say a little bit about separating hyperplanes. 

## 4.8.4 The Separating Hyperplane Theorem

Definition 4.8.3 The set $\left\{ \mathbf { z } \in \Re ^ { N } : \mathbf { p } ^ { \top } \mathbf { z } = \mathbf { p } ^ { \top } \mathbf { z } ^ { * } \right\}$ is the hyperplane through $\mathbf { z } ^ { \ast }$ with normal p. 

Note that any hyperplane divides $\Re ^ { N }$ into two closed half-spaces, 

$$
\left\{\mathbf {z} \in \Re^ {N}: \mathbf {p} ^ {\top} \mathbf {z} \leq \mathbf {p} ^ {\top} \mathbf {z} ^ {*} \right\}
$$

and 

$$
\left\{\mathbf {z} \in \Re^ {N}: \mathbf {p} ^ {\top} \mathbf {z} \geq \mathbf {p} ^ {\top} \mathbf {z} ^ {*} \right\}.
$$

The intersection of these two closed half-spaces is the hyperplane itself. 

In two dimensions, a hyperplane is just a line; in three dimensions, it is just a plane. 

The idea behind the separating hyperplane theorem is quite intuitive: if we take any point on the boundary of a convex set, we can find a hyperplane through that point so that the entire convex set lies on one side of that hyperplane. We will essentially be applying this notion to the upper contour sets of quasiconcave utility functions, which are of course convex sets. We will interpret the separating hyperplane as a budget hyperplane, and the normal vector as a price vector, so that at those prices nothing giving higher utility than the cutoff value is affordable. 

Theorem 4.8.2 (Separating Hyperplane Theorem) If $Z$ is a convex subset of $\Re ^ { N }$ and $\mathbf { z } ^ { \ast } \in Z , \mathbf { z } ^ { \ast } \notin$ int $Z ,$ then ∃p<sup>∗</sup> $\neq \mathbf { 0 }$ in $\Re ^ { N }$ such that $\mathbf { p } ^ { * \top } \mathbf { z } ^ { * } \leq \mathbf { p } ^ { * \top } \mathbf { z } \forall \mathbf { z } \in Z ,$ or Z is contained in one ofthe closed half-spaces associated with the hyperplane through $\mathbf { z } ^ { \ast }$ with normal $\mathbf { p } ^ { * }$ 

Proof Not given. See ? 

Q.E.D. 

## 4.8.5 The Second Welfare Theorem

(See ?.) 

We make slightly stronger assumptions than are essential for the proof of this theorem. This allows us to give an easier proof. 

Theorem 4.8.3 (Second Welfare Theorem) Ifall individual preferences are strictly convex, continuous and strictly monotonic, and if $\mathbf { X } ^ { * }$ is a Pareto efficient allocation such that all households are allocated positive amounts of all goods $( x _ { h } ^ { * g } > 0 \forall g = 1 , \ldots , N ; h = 1 , \ldots , H )$ , then a reallocation of the initial aggregate endowment can yield an equilibrium where the allocation is $\mathbf { X } ^ { * }$ 

Proof There are four main steps in the proof. 

1. First we construct a set of utility-enhancing endowment perturbations, and use the separating hyperplane theorem to find prices at which no such endowment perturbation is affordable. 

We need to use the fact (Theorem 3.2.1) that a sum of convex sets, such as 

$$
X + Y \equiv \left\{\mathbf {x} + \mathbf {y}: \mathbf {x} \in X, \mathbf {y} \in Y \right\},
$$

is also a convex set. 

Given an aggregate initial endowment $\begin{array} { r } { \mathbf { x } ^ { * } = \sum _ { h = 1 } ^ { H } \mathbf { x } _ { h } ^ { * } } \end{array}$ , we interpret any vector of the form $\begin{array} { r } { \mathbf { z } = \sum _ { h = 1 } ^ { H } \mathbf { x } _ { h } - \mathbf { x } ^ { * } } \end{array}$ as an endowment perturbation. Now consider the set of all ways of changing the aggregate endowment without making anyone worse off: 

$$
Z \equiv \left\{\mathbf {z} \in \Re^ {N}: \exists x _ {h} ^ {n} \geq 0   \forall g, h s. t. u _ {h} (\mathbf {x} _ {h}) \geq u _ {h} (\mathbf {x} _ {h} ^ {*}) \& \mathbf {z} = \sum_ {h = 1} ^ {H} \mathbf {x} _ {h} - \mathbf {x} ^ {*} \right\}.\tag{4.8.5}
$$

$Z$ is a sum of convex sets provided that preferences are assumed to be convex: 

$$
Z = \sum_ {h = 1} ^ {H} X _ {h} - \left\{\mathbf {x} ^ {*} \right\}
$$

where 

$$
X _ {h} \equiv \left\{\mathbf {x} _ {h}: u _ {h} \left(\mathbf {x} _ {h}\right) \geq u _ {h} \left(\mathbf {x} _ {h} ^ {*}\right) \right\}.
$$

2. Next, we need to show that the zero vector is in the set $Z ,$ , but not in the interior of $Z$ . 

To show that $\mathbf { 0 } \in Z .$ , we just set $\mathbf { x } _ { h } = \mathbf { x } _ { h } ^ { * }$ and observe that $\begin{array} { r } { \mathbf { 0 } = \sum _ { h = 1 } ^ { H } \mathbf { x } _ { h } ^ { * } - } \end{array}$ $\mathbf { x } ^ { * } . ^ { 4 }$ 

The zero vector is not, however, in the interior of $Z ,$ , since then $Z$ would contain some vector, say $\mathbf { z } ^ { \ast }$ , in which all components were strictly negative. In other words, we could take away some of the aggregate endowment of every good without making anyone worse off than under the allocation $\mathbf { X } ^ { * }$ But by then giving $- \mathbf { z } ^ { \ast }$ back to one individual, he or she could be made better off without making anyone else worse off, contradicting Pareto optimality, again using the assumption that preferences are strictly monotonic. 

So, applying the Separating Hyperplane Theorem with $\mathbf { z } ^ { * } = \mathbf { 0 }$ , we have a price vector $\mathbf { p } ^ { * }$ such that $0 = \mathbf { p } ^ { * \top } \mathbf { 0 } \leq \mathbf { p } ^ { * \top } \mathbf { z } \forall \mathbf { z } \in Z$ 

Since preferences are monotonic, the set $Z$ must contain all the standard unit basis vectors ((1, 0, . . . , 0), &c.). This fact can be used to show that all components of $\mathbf { p } ^ { * }$ are non-negative, which is essential if it is to be interpreted as an equilibrium price vector. 

3. Next, we specify one way of redistributing the initial endowment in order that the desired prices and allocation emerge as a competitive equilibrium. All we need to do is value endowments at the equilibrium prices, and redistribute the aggregate endowment of each good to consumers in proportion to their share in aggregate wealth computed in this way. 

4. Finally, we confirm that utility is maximised by the given Pareto efficient allocation, $\mathbf { X } ^ { \ast }$ , at these prices. As usual, the proof is by contradiction: the details are left as an exercise. 

Q.E.D. 

## 4.8.6 Complete markets

The First Welfare Theorem tells us that competitive equilibrium allocations are Pareto optimal if markets are complete. If there are missing markets, then competitive trading may not lead to a Pareto optimal allocation. We can use the Edgeworth Box diagram to illustrate the simplest possible version of this principle. 

## 4.8.7 Other characterizations of Pareto efficient allocations

There are a total of five equivalent characterisations of Pareto efficient allocations. 

Theorem 4.8.4 Each of the following is an equivalent description of the set of allocations which are Pareto efficient: 

1. by definition, feasible allocations such that no other allocation strictly increases at least one individual’s utility without decreasing the utility ofany other individual; 

2. by the Welfare Theorems, equilibrium allocations for all possible distributions ofthefixed initial aggregate endowment; 

3. in two dimensions, allocations lying on the contract curve in the Edgeworth box; 

Revised: December 2, 1998 

4. allocations which solve: <sup>5</sup> 

$$
\max _ {\{\mathbf {x} _ {h}: h = 1, \dots , H \}} \sum_ {h = 1} ^ {H} \lambda_ {h} \left[ u _ {h} (\mathbf {x} _ {h}) \right]\tag{4.8.6}
$$

subject to thefeasibility constraints 

$$
\sum_ {h = 1} ^ {H} \mathbf {x} _ {h} = \sum_ {h = 1} ^ {H} \mathbf {e} _ {h}\tag{4.8.7}
$$

for some non-negative weights $\{ \lambda _ { h } \} _ { h = 1 } ^ { H }$ 

5. allocations which maximise the utility ofa representative agent given by 

$$
\sum_ {h = 1} ^ {H} \lambda_ {h} [ u _ {h} (\mathbf {x} _ {h}) ]\tag{4.8.8}
$$

where $\{ \lambda _ { h } \} _ { h = 1 } ^ { H }$ are again any non-negative weights. 

Proof If an allocation is not Pareto efficient, then the Pareto-dominating allocation gives a higher value of the objective function in the above problem for all possible weights. 

If an allocation is Pareto efficient, then the relative weights for which the above objective function is maximized are the ratios of the Lagrange multipliers from the problem of maximizing any individual’s utility subject to the constraint that all other individuals’ utilities are unchanged: 

$$
\max u _ {1} (\mathbf {x} _ {1})\tag{4.8.9}
$$

s.t. 

$$
u _ {h} (\mathbf {x} _ {h}) = u _ {h} (\mathbf {x} _ {h} ^ {*}) h = 2, \ldots , H\tag{4.8.10}
$$

since these two problems will have the same necessary and sufficient first order conditions. 

The absolute weights corresponding to a particular allocation are not unique, as they can be multiplied by any positive constant without affecting the maximum. 

Different absolute weights (or Lagrange multipliers) arise from fixing different individuals’ utilities in the last problem, but the relative weights will be the same. 

<sup>5</sup>The solution here would be unique if the underlying utility function were concave, since linear combinations of concave functions with non-negative weights are concave, and the constraints specify a convex set on which the objective function has a unique optimum. This argument can not be used with merely quasiconcave utility functions. 

Note that corresponding to each Pareto efficient allocation there is at least one: 

1. set of non-negative weights defining 

(a) the objective function in 4. and 

(b) the representative agent in 5. 

and 

2. initial allocation leading to the competitive equilibrium in 2. 

## 4.9 Multi-period General Equilibrium

In Section 4.2, it was pointed out that the objects of choice can be differentiated not only by their physical characteristics, but also both by the time at which they are consumed and by the state of nature in which they are consumed. These distinctions were suppressed in the intervening sections but are considered again in this section and in Section 5.4 respectively. 

The multi-period model should probably be introduced at the end of Chapter 4 but could also be left until Chapter 7. For the moment this brief introduction is duplicated in both chapters. 

Discrete time multi-period investment problems serve as a stepping stone from the single period case to the continuous time case. 

The main point to be gotten across is the derivation of interest rates from equilibrium prices: spot rates, forward rates, term structure, etc. 

This is covered in one of the problems, which illustrates the link between prices and interest rates in a multiperiod model. 

## Chapter 5

## CHOICE UNDER UNCERTAINTY

## 5.1 Introduction

[To be written.] 

## 5.2 Review of Basic Probability

Economic theory has, over the years, used many different, sometimes overlapping, sometimes mutually exclusive, approaches to the analysis of choice under uncertainty. This chapter deals with choice under uncertainty exclusively in a single period context. Trade takes place at the beginning of the period and uncertainty is resolved at the end of the period. This framework is sufficient to illustrate the similarities and differences between the most popular approaches. 

When we consider consumer choice under uncertainty, consumption plans will have to specify a fixed consumption vector for each possible state of nature or state ofthe world. This just means that each consumption plan is a random vector. Let us review the associated concepts from basic probability theory: probability space; random variables and vectors; and stochastic processes. 

Let Ω denote the set of all possible states of the world, called the sample space. A collection of states of the world, $A \subseteq \Omega$ , is called an event. 

Let A be a collection of events in Ω. The function $P : \mathcal { A }  [ 0 , 1 ]$ is a probability function if 

1. (a) $\Omega \in { \mathcal { A } }$ 

(b) $A \in \mathcal { A } \Rightarrow \Omega - A \in \mathcal { A }$ 

(c) $A _ { i } \in \mathcal { A } \mathrm { ~ f o r ~ } i = 1 , \dots , \infty \Rightarrow \bigcup _ { i = 1 } ^ { \infty } A _ { i } \in \mathcal { A }$ 

(i.e. A is a sigma-algebra of events) 

and 

2. (a) $P \left( \Omega \right) = 1$ 

(b) $P \left( \Omega - A \right) = 1 - P \left( A \right) \forall A \in \mathcal { A } \left( \mathrm { r e d u n d a n t ~ a s s u m p t i o n } \right)$ 

(c) ${ \begin{array} { r l } & { P \left( \bigcup _ { i = 1 } ^ { \infty } A _ { i } \right) \ = \ \sum _ { i = 1 } ^ { \infty } P \left( A _ { i } \right) } \\ & { { \mathrm { e v e n t s ~ i n ~ } } A . } \end{array} }$ when $A _ { 1 } , A _ { 2 } , . . .$ . are pairwise disjoint 

## (Ω, A, P) is then called a probability space

Note that the certainty case we considered already is just the special case of uncertainty in which the set Ω has only one element. 

We will consider these concepts in more detail when we come to intertemporal models. 

Suppose we are given such a probability space. 

The function $\tilde { x } : \Omega \to \Re$ is a random variable (r.v.) if $\forall x \in \Re \left\{ \omega \in \Omega : \tilde { x } \left( \omega \right) \leq \right.$ $x \} \in A ,$ i.e. a function is a random variable if we know the probability that the value of the function is less than or equals any given real number. 

The function $F _ { \tilde { x } } : \Re  [ 0 , 1 ] : x \mapsto \operatorname* { P r } ( \tilde { x } \leq x ) \equiv P ( \{ \omega \in \Omega : \tilde { x } ( \omega ) \leq x \} )$ is known as the cumulative distributionfunction (c.d.f.) of the random variable x˜. 

The convention of using a tilde over a letter to denote a random variable is common in financial economics; in other fields capital letters may be reserved for random variables. In either case, small letters usually denote particular real numbers (i.e. particular values of the random variable). 

A random vector is just a vector of random variables. It can also be thought of as a vector-valued function on the sample space Ω. 

A stochastic process is a collection of random variables or random vectors indexed by time, e.g. $\{ \tilde { x } _ { t } : t \in T \}$ or just $\{ \tilde { x } _ { t } \}$ if the time interval is clear from the context. For the purposes of this part of the course, we will assume that the index set consists of just a finite number of times i.e. that we are dealing with discrete time stochastic processes. 

Then a stochastic process whose elements are N-dimensional random vectors is equivalent to an $N \vert T \vert$ -dimensional random vector. 

The (joint) c.d.f. of a random vector or stochastic process is the natural extension of the one-dimensional concept. 

Random variables can be discrete, continuous or mixed. The expectation (mean, average) of a discrete r.v., x˜, with possible values $x _ { 1 } , x _ { 2 } , x _ { 3 } , . . .$ . is given by 

$$
E \left[ \tilde {x} \right] \equiv \sum_ {i = 1} ^ {\infty} x _ {i} P r \left(\tilde {x} = x _ {i}\right).
$$

For a continuous random variable, the summation is replaced by an integral. 

The covariance of two random variables x˜ and $\tilde { y }$ is given by 

$$
\operatorname{Cov} \left[ \tilde {x}, \tilde {y} \right] \equiv E \left[ \left(\tilde {x} - e \left[ \tilde {x} \right]\right) \left(\tilde {y} - E \left[ \tilde {y} \right]\right) \right].
$$

The covariance of a random variable with itself is called its variance. 

The expectation of a random vector is just the vector of the expectations of the component random variables. 

The variance (variance-covariance matrix) of a random vector is the (symmetric, positive semi-definite) matrix of the covariances between the component random variables. 

Given any two random variables x˜ and ${ \tilde { y } } ,$ , we can define a third random variable˜ by 

$$
\tilde {\epsilon} \equiv \tilde {y} - \alpha - \beta \tilde {x}.\tag{5.2.1}
$$

To specify $\widetilde { \epsilon }$ completely, we can either specify α and $\beta$ explicitly or fix them implicitly by imposing (two) conditions on˜. We do the latter by insisting 

1. $\widetilde { \epsilon }$ and $\tilde { x }$ are uncorrelated (this is not the same as assuming statistical independence, except in special cases such as bivariate normality) 

2. $E \left[ \tilde { \epsilon } \right] = 0$ 

It follows that: 

$$
\beta = \frac {\operatorname{Cov} [ \tilde {x} , \tilde {y} ]}{\operatorname{Var} [ \tilde {x} ]}\tag{5.2.2}
$$

and 

$$
\alpha = E [ \tilde {y} ] - \beta E [ \tilde {x} ].\tag{5.2.3}
$$

But what about the conditional expectation, $E [ \tilde { y } | \tilde { x } = x ] ?$ This is not equal to $\alpha + \beta x$ , as one might expect, unless $E \left[ \tilde { \epsilon } | \tilde { x } = x \right] = 0 .$ . This requires statistical independence rather than the assumed lack of correlation. Again, a sufficient condition is multivariate normality. 

The notion of the $\beta$ of $\tilde { y }$ with respect to $\tilde { x }$ as given in (5.2.2) will recur frequently. The final concept required from basic probability theory is the notion of a mixture of random variables. For lotteries which are discrete random variables, with payoffs $x _ { 1 } , x _ { 2 } , x _ { 3 } , . . .$ . occuring with probabilities $\pi _ { 1 } , \pi _ { 2 } , \pi _ { 3 } , . . .$ . respectively, we wil use the notation: 

$$
\pi_ {1} x _ {1} \oplus \pi_ {2} x _ {2} \oplus \pi_ {3} x _ {3} \oplus \dots
$$

Similar notation will be used for compound lotteries (mixtures of random variables) where the payoffs themselves are further lotteries. 

This might be a good place to talk about the MVN distribution and Stein’s lemma. 

## 5.3 Taylor’s Theorem: Stochastic Version

We will frequently use the univariate Taylor expansion as applied to a function of a random variable expanded about the mean of the random variable.<sup>1</sup> Taking expectations on both sides of the Taylor expansion: 

$$
f (\tilde {x}) = f (E [ \tilde {x} ]) + \sum_ {n = 1} ^ {\infty} \frac {1}{n !} f ^ {(n)} (E [ \tilde {x} ]) (\tilde {x} - E [ \tilde {x} ]) ^ {n}\tag{5.3.1}
$$

yields: 

$$
E [ f (\tilde {x}) ] = f (E [ \tilde {x} ]) + \sum_ {n = 2} ^ {\infty} \frac {1}{n !} f ^ {(n)} (E [ \tilde {x} ]) m ^ {n} (\tilde {x}),\tag{5.3.2}
$$

where 

$$
m ^ {n} (\tilde {x}) \equiv E \left[ (\tilde {x} - E [ \tilde {x} ]) ^ {n} \right].\tag{5.3.3}
$$

In particular, 

$$
m ^ {1} (\tilde {x}) = E \left[ (\tilde {x} - E [ \tilde {x} ]) ^ {1} \right] \equiv 0\tag{5.3.4}
$$

$$
m ^ {2} (\tilde {x}) = E \left[ (\tilde {x} - E [ \tilde {x} ]) ^ {2} \right] \equiv \operatorname{Var} [ \tilde {x} ]\tag{5.3.5}
$$

$$
m ^ {3} (\tilde {x}) = E \left[ (\tilde {x} - E [ \tilde {x} ]) ^ {3} \right] \equiv \operatorname{Skew} [ \tilde {x} ]\tag{5.3.6}
$$

and 

$$
m ^ {4} (\tilde {x}) = E \left[ (\tilde {x} - E [ \tilde {x} ]) ^ {4} \right] \equiv \mathrm{Kurt} [ \tilde {x} ],\tag{5.3.7}
$$

which allows us to start the summation in (5.3.2) at $n = 2$ rather than $n = 1$ Indeed, we can rewrite (5.3.2) as 

$$
\begin{array}{r c l} E [ f (\tilde {x}) ] & = & f (E [ \tilde {x} ]) + \frac {1}{2} f ^ {\prime \prime} (E [ \tilde {x} ]) \mathrm{Var}   [ \tilde {x} ] + \frac {1}{6} f ^ {\prime \prime \prime} (E [ \tilde {x} ]) \mathrm{Skew}   [ \tilde {x} ] \\ & & + \frac {1}{2 4} f ^ {\prime \prime \prime \prime} (E [ \tilde {x} ]) \mathrm{Kurt}   [ \tilde {x} ] + \sum_ {n = 5} ^ {\infty} \frac {1}{n !} f ^ {(n)} (E [ \tilde {x} ]) m ^ {n} (\tilde {x}). \end{array}\tag{5.3.8}
$$

## 5.4 Pricing State-Contingent Claims

This part of the course draws on ?, ? and ?. 

The analysis of choice under uncertaintly will begin by reinterpreting the general equilibrium model of Chapter 4 so that goods can be differentiated by the state of nature in which they are consumed. Specifically, it will be assumed that the underlying sample space comprises a finite number of states of nature. A more thorough analysis of choice under uncertainty, allowing for infinite and continuous sample spaces and based on additional axioms of choice, follows in Section 5.5. Consider a world with M possible states of nature (distinguished by a first subscript), markets for N securities (distinguished by a second subscript) and H consumers (distinguished by a superscript).<sup>2</sup> 

Definition 5.4.1 A state contingent claim or Arrow-Debreu security is a random variable or lottery which takes the value 1 in one particular state of nature and the value 0 in all other states. 

Definition 5.4.2 A complex security is a random variable or lottery which can take on arbitrary values. The payoffs of a typical complex security will be represented by a column vector, $\mathbf { y } _ { j } \in \Re ^ { M }$ , where $y _ { i j }$ is the payoff in state i of security j. 

The set of all complex securities on a given finite sample space is an M-dimensional vector space and the M possible Arrow-Debreu securities constitute the standard basis for this vector space. 

State contingent claims prices are determined by the market clearing equations in a general equilibrium model: 

Aggregate consumption in state i = Aggregate endowment in state i. 

Each individual will have an optimal consumption choice depending on endowments and preferences and conditional on the state of the world. Optimal future consumption is denoted 

$$
\mathbf {x} ^ {*} = \left( \begin{array}{c} x _ {1} ^ {*} \\ x _ {2} ^ {*} \\ \dots \\ x _ {N} ^ {*} \end{array} \right).\tag{5.4.1}
$$

If there are N complex securities, then the investor must find a portfolio $\mathbf { w } =$ $( w _ { 1 } , \dots , w _ { N } )$ whose payoffs satisfy 

$$
x _ {i} ^ {*} = \sum_ {j = 1} ^ {N} y _ {i j} w _ {j}.
$$

Let Y be the $M \times N$ matrix<sup>3</sup> whose jth column contains the payoffs of the jth complex security in each of the M states of nature, i.e. 

$$
\mathbf {Y} \equiv (\mathbf {y} _ {1}, \mathbf {y} _ {2}, \dots \mathbf {y} _ {N}).\tag{5.4.2}
$$

Theorem 5.4.1 Ifthere are M complex securities $( M = N )$ and the payoffmatrix Y is non-singular, then markets are complete. 

Proof Suppose the optimal trade for consumer $i$ state $j$ is $x _ { i j } - e _ { i j }$ . Then can invert Y to work out optimal trades in terms of complex securities. 

Q.E.D. 

An $( N + 1 )$ st security would be redundant. 

Either a singular square matrix $\mathrm { o r } < N$ complex securities would lead to incomplete markets. 

So far, we have made no assumptions about the form of the utility function, written purely as 

$$
u \left(x _ {0}, x _ {1}, x _ {2}, \ldots , x _ {N}\right),
$$

where $x _ { 0 }$ represents the quantity consumed at date 0 and $x _ { i } ( i > 0 )$ represents the quantity consumed at date 1 if state i materialises. 

## 5.4.1 Completion of markets using options

Assume that there exists a state index portfolio, $Y$ , yielding different non-zero payoffs in each state (i.e. a portfolio with a different payout in each state of nature, possibly one mimicking aggregate consumption). WLOG we can rank the states so that $Y _ { i } < Y _ { j } { \mathrm { ~ i f ~ } } i < j$ 

We now present some results, following ?, showing conditions under which trading in a state index portfolio and in options on the state index portfolio can lead to the Pareto optimal complete markets equilibrium allocation. Now consider completion of markets using options on aggregate consumption. 

In real-world markets, the number of linearly independent corporate securities is probably less than $M$ 

However, options on corporate securities may be sufficient to form complete markets, and thereby ensure allocational (Pareto) efficiency for arbitrary preferences. Further assume that $\exists ~ M - 1$ European call options on $Y$ with exercise prices $Y _ { 1 } , Y _ { 2 } , \dots , Y _ { M - 1 }$ 

A European call option with exercise price K is an option to buy a security for K on a fixed date. 

An American call option is an option to buy on or before the fixed date. 

A put option is an option to sell. 

Here, the original state index portfolio and the $M - 1$ European call options yield the payoff matrix: 

$$
\left( \begin{array}{c c c c c} y _ {1} & y _ {2} & y _ {3} & \ldots & y _ {M} \\ 0 & y _ {2} - y _ {1} & y _ {3} - y _ {1} & \ldots & y _ {M} - y _ {1} \\ 0 & 0 & y _ {3} - y _ {2} & \ldots & y _ {M} - y _ {2} \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & \ldots & y _ {M} - y _ {M - 1} \end{array} \right) = \left( \begin{array}{c} \text {security Y} \\ \text {call option 1} \\ \text {call option 2} \\ \vdots \\ \text {call option M - 1} \end{array} \right)\tag{5.4.3}
$$

and as this matrix is non-singular, we have constructed a complete market. Instead of assuming a state index portfolio exists, we can assume identical probability beliefs and state-independent utility and complete markets in a similar manner (see below). 

# 5.4.2 Restrictions on security values implied by allocational efficiency and covariance with aggregate consumption

$\left\{ \begin{array} { l l } { C \omega = } & { \mathrm { a g g r e g a t e c o n s u m p } } \\ { \Omega _ { k } = } & { \left\{ \omega \in \Omega : C \omega = k \right\} } \end{array} \right.$ tion in state ω Let 

Let $\phi ( k )$ be the value of the claim with payoffs 

$$
y _ {k \omega} = \left\{ \begin{array}{l l} 1 & \text { if } C \omega = k \\ 0 & \text { otherwise } \end{array} \right.\tag{5.4.4}
$$

and let the agreed probability of the event $\Omega _ { k }$ (i.e. of aggregate consumption taking the value k) be: 

$$
\pi (k) = \sum_ {\omega \in \Omega_ {k}} \pi \omega\tag{5.4.5}
$$

By time-additivity and state-independence of the utility function: 

$$
\phi \omega = \frac {\pi \omega u _ {i} ^ {\prime} (c _ {i \omega})}{u _ {i 0} ^ {\prime} (c _ {i 0})} \quad \forall \omega \in \Omega\tag{5.4.6}
$$

The no arbitrage condition implies 

$$
\phi (k) = \sum_ {\omega \in \Omega_ {k}} \phi \omega\tag{5.4.7}
$$

$$
= \frac {u _ {i} ^ {\prime} (f _ {i} (k))}{u _ {i 0} ^ {\prime} (c _ {i 0})} \sum_ {\omega \in \Omega_ {k}} \pi \omega\tag{5.4.8}
$$

$$
{ = } { \frac { u _ { i } ^ { \prime } ( f _ { i } ( k ) ) } { u _ { i 0 } ^ { \prime } ( c _ { i 0 } ) } \pi ( k ) }\tag{5.4.9}
$$

where $f _ { i } ( k )$ denotes the i-th individual’s equilibrium consumption in those states where aggregate consumption equals k. 

<table><tr><td></td><td>x(0)</td><td>x(1)</td><td>x(2)</td></tr><tr><td><eq>\tilde{C} = 1</eq></td><td>1</td><td>0</td><td>0</td></tr><tr><td><eq>\tilde{C} = 2</eq></td><td>2</td><td>1</td><td>0</td></tr><tr><td><eq>\tilde{C} = 3</eq></td><td>3</td><td>2</td><td>1</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td><eq>\tilde{C} = L</eq></td><td>L</td><td>L-1</td><td>L-2</td></tr></table>


Table 5.1: Payoffs for Call Options on the Aggregate Consumption


State-independence of the utility function is required for $f _ { i } ( k )$ to be well-defined. Therefore, an arbitrary security x has value: 

$$
S _ {x} = \sum_ {\omega \in \Omega} \phi \omega x \omega\tag{5.4.10}
$$

$$
= \sum_ {k} \sum_ {\omega \in \Omega_ {k}} \phi \omega x \omega\tag{5.4.11}
$$

$$
= \sum_ {k} \frac {u _ {i} ^ {\prime} (f _ {i} (k))}{u _ {i 0} ^ {\prime} (c _ {i 0})} \sum_ {\omega \in \Omega_ {k}} \pi \omega x \omega\tag{5.4.12}
$$

$$
= \sum_ {k} \phi (k) \sum_ {\omega \in \Omega_ {k}} \frac {\pi \omega}{\pi (k)} x \omega\tag{5.4.13}
$$

$$
= \sum_ {k} \phi (k) E [ \tilde {x} | \tilde {C} = k ]\tag{5.4.14}
$$

## 5.4.3 Completing markets with options on aggregate consumption

Let $x ( k )$ be the vector of payoffs in the various possible states on a European call option on aggregate consumption with one period to maturity and exercise price k. 

Let $\{ 1 , 2 , \ldots , L \}$ be the set of possible values of aggregate consumption $C ( \omega )$ Then payoffs are as given in Table 5.1. 

This all assumes 

1. identical probability beliefs 

2. time-additivity of u 

3. state-independent u 

## 5.4.4 Replicating elementary claims with a butterfly spread

Elementary claims against aggregate consumption can be constructed as follows, for example, for state 1, using a butterfly spread: 

$$
[ x (0) - x (1) ] - [ x (1) - x (2) ]\tag{5.4.15}
$$

yields the payoff: 

$$
\begin{array}{r l} \left[ \left( \begin{array}{c} 1 \\ 2 \\ 3 \\ \vdots \\ L \end{array} \right) - \left( \begin{array}{c} 0 \\ 1 \\ 2 \\ \vdots \\ L - 1 \end{array} \right) \right] - \left[ \left( \begin{array}{c} 0 \\ 1 \\ 2 \\ \vdots \\ L - 1 \end{array} \right) - \left( \begin{array}{c} 0 \\ 0 \\ 1 \\ \vdots \\ L - 2 \end{array} \right) \right] & = \left( \begin{array}{c} 1 \\ 1 \\ 1 \\ \vdots \\ 1 \end{array} \right) - \left( \begin{array}{c} 0 \\ 1 \\ 1 \\ \vdots \\ 1 \end{array} \right) \\ & = \left( \begin{array}{c} 1 \\ 0 \\ 0 \\ \vdots \\ 0 \end{array} \right) \end{array} \tag {5.4}\tag{5.4.16}
$$

i.e. this replicating portfolio pays 1 iff aggregate consumption is 1, and 0 otherwise. 

The prices of this, and the other elementary claims, must, by no arbitrage, equal the prices of the corresponding replicating portfolios. 

## 5.5 The Expected Utility Paradigm

## 5.5.1 Further axioms

The objects of choice with which we are concerned in a world with uncertainty could still be called consumption plans, but we will acknowledge the additional structure now described by terming them lotteries. 

If there are k physical commodities, a consumption plan must specify a k-dimensional vector, $\mathbf { x } \in \Re ^ { k }$ , for each time and state of the world. 

We assume a finite number of times, denoted by the set $T .$ . 

The possible states of the world are denoted by the set $\Omega$ . 

So a consumption plan or lottery is just a collection of |T| k-dimensional random vectors, i.e. a stochastic process. 

Again to distinguish the certainty and uncertainty cases, we let $\mathcal { L }$ denote the collection of lotteries under consideration; $\mathcal { X }$ will now denote the set of possible values of the lotteries in $\mathcal { L }$ 

Preferences are now described by a relation on ${ \mathcal { L } } .$ We will continue to assume that preference relations are complete, reflexive, transitive, and continuous. 

$\mathcal { X }$ can be identified with a subset of $\mathcal { L } ,$ , in that each sure thing in X can be identified with the trivial lottery that pays off that sure thing with probability (w.p.) 1. 

Although we have moved from a finite-dimensional to an infinite-dimensional problem by explicitly allowing a continuum of states of nature, it can be shown that the earlier theory of choice under certainty carries through to choice under uncertainty, in particular a preference relation can always be represented by a continuous utility function on $\mathcal { L }$ 

However, we would like utility functions to have a stronger property than continuity, namely the expected utility property. 

Axiom 8 (Substitution or Independence Axiom) $H a \in ( 0 , 1 ]$ and $\tilde { p } \succ \tilde { q } ,$ then 

$$
a \tilde {p} \oplus (1 - a) \tilde {r} \succ a \tilde {q} \oplus (1 - a) \tilde {r} \forall \tilde {r} \in \mathcal {L}.
$$

Axiom 9 (Archimedian Axiom) $I f \tilde { p } \succ \tilde { q } \succ \tilde { r }$ then 

$$
\exists a, b \in (0, 1) \text {   s.t.   } a \tilde {p} \oplus (1 - a) \tilde {r} \succ \tilde {q} \succ b \tilde {p} \oplus (1 - b) \tilde {r}.
$$

(The Archimedian axiom is just a generalisation of the continuity axiom.) 

Axiom 10 (Sure Thing Principle) Ifprobability is concentrated on a set of sure things which are preferred to $q ,$ then the associated consumption plan is also preferred to $q .$ 

(The Sure Thing Principle is just a generalisation of the Substitution Axiom.) Now let us consider the Allais paradox. 

Suppose 

$$
1 £ 1 m. \succ 0. 1 £ 5 m. \oplus 0. 8 9 £ 1 m. \oplus 0. 0 1 £ 0.
$$

Then, unless the substitution axiom is contradicted: 

$$
1 £ 1 m. \succ \frac {1 0}{1 1} £ 5 m. \oplus \frac {1}{1 1} £ 0.
$$

Finally, by the substitution axiom again, 

$$
0. 1 1 £ 1 m. \oplus 0. 8 9 £ 0 \succ 0. 1 £ 5 m. \oplus 0. 9 £ 0.
$$

If these appears counterintuitive, then so does the independence axiom above. One justification for persisting with the independence axiom is provided by ?. 

Revised: December 2, 1998 

## 5.5.2 Existence of expected utility functions

A function $u \colon \mathfrak { R } ^ { k \times | T | }  \mathfrak { R }$ can be thought of as a utility function on sure things. 

Definition 5.5.1 Let $V : { \mathcal { L } }  \Re$ be a utility function representing the preference relation . 

Then $\succeq i s$ said to have an expected utility representation if there exists a utility function on sure things, $u ,$ such that 

$$
\begin{array}{r c l} {V \left(\{\tilde {x} _ {t} \}\right)} & = & {E \left[ u \left(\{\tilde {x} _ {t} \}\right) \right]} \\ & = & {\int \ldots \int u \left(\{x _ {t} \}\right) d F _ {\{\tilde {x} _ {t} \}} \left(\{x _ {t} \}\right)} \end{array}
$$

Such a representation will often be called a Von Neumann-Morgenstern (or VNM) utility function, after its originators $( ? ) ,$ , orjust an expected utility function. 

Any strictly increasing transformation of a VNM utility function represents the same preferences. 

However, only increasing affine transformations: 

$$
f (x) = a + b x (b > 0)
$$

retain the expected utility property. 

Proof of this is left as an exercise. 

We will now consider necessary and sufficient conditions on preference relations for an expected utility representation to exist. 

Theorem 5.5.1 If X contains only a finite number of possible values, then the substitution and Archimidean axioms are necessary and sufficientfor a preference relation to have an expected utility representation. 

Proof We will just sketch the proof that the axioms imply the existence of an expected utility representation; the proof of the converse is left as an exercise. For full details, see ?. 

Since X is finite, and unless the consumer is indifferent among all possible choices, there must exist maximal and minimal sure things, say $p ^ { + }$ and $p _ { - }$ respectively. 

By the substitution axiom, and a simple inductive argument, these are maximal and minimal in $\mathcal { L }$ as well as in $\mathcal { X } .$ . (If X is not finite, then an inductive argument can no longer be used and the Sure Thing Principle is required.) 

From the Archimedean axiom, it can be deduced that for every other lottery, $\tilde { p } ,$ there exists a unique $V \left( \tilde { p } \right)$ such that 

$$
\tilde {p} \sim V (\tilde {p}) p ^ {+} \oplus (1 - V (\tilde {p})) p _ {-}.
$$

It is easily seen that $V$ represents $\succeq$ 

Linearity can be shown as follows: 

We leave it as an exercise to deduce from the axioms that if $\tilde { x } \sim \tilde { y }$ and $\tilde { z } \sim \tilde { t }$ then 

$$
\pi \tilde {x} \oplus (1 - \pi) \tilde {z} \sim \pi \tilde {y} \oplus (1 - \pi) \tilde {t}.
$$

Define $\tilde { z } \equiv \pi \tilde { x } \oplus \left( 1 - \pi \right) \tilde { y } .$ 

Then, using the definitions of $V \left( \tilde { x } \right)$ and $V \left( \tilde { y } \right)$ R 

$$
\begin{array}{r c l} \tilde {z} & \sim & \pi \tilde {x} \oplus (1 - \pi)   \tilde {y} \\ & \sim & \pi \left(V (\tilde {x})   p ^ {+} \oplus (1 - V (\tilde {x}))   p _ {-}\right) \oplus (1 - \pi) \left(V (\tilde {y})   p ^ {+} \oplus (1 - V (\tilde {y}))   p _ {-}\right) \\ & = & (\pi V (\tilde {x}) + (1 - \pi)   V (\tilde {y}))   p ^ {+} \oplus (\pi (1 - V (\tilde {x})) + (1 - \pi) (1 - V (\tilde {y})))   p _ {-}. \end{array}
$$

It follows that 

$$
V \left(\pi \tilde {x} \oplus (1 - \pi) \tilde {y}\right) = \pi V (\tilde {x}) + (1 - \pi) V (\tilde {y}).
$$

This shows linearity for compound lotteries with only two possible outcomes: by an inductive argument, every lottery can be reduced recursively to a two-outcome lottery when there are only a finite number of possible outcomes altogether.<sub>Q.E.D.</sub> 

Theorem 5.5.2 For more general ${ \mathcal { L } } ,$ to these conditions must be added some technical conditions and the Sure Thing Principle. 

Proof We will not consider the proof of this more general theorem. It can be found in ?. Q.E.D. 

Note that expected utility depends only on the distribution function of the consumption plan. 

Two consumption plans having very different consumption patterns across states of nature but the same probability distribution give the same utility. $E . g .$ . if wet days and dry days are equally likely, then an expected utility maximiser is indifferent between any consumption plan and the plan formed by switching consumption between wet and dry days. 

The basic objects of choice under expected utility are not consumption plans but classes of consumption plans with the same cumulative distribution function. 

Chapter 6 will consider the problem of portfolio choice in considerable depth. This chapter, however, must continue with some basic analysis of the choice between one riskfree and one risky asset, following ?. 

Such an example is sufficient to show several things: 

1. There is no guarantee that the portfolio choice problem has any finite or unique solution unless the expected utility function is concave. 

2. probably local risk neutrality and stuff like that too. 

## 5.6 Jensen’s Inequality and Siegel’s Paradox

Theorem 5.6.1 (Jensen’s Inequality) The expected value of a (strictly) concave function of a random variable is (strictly) less than the same concave function of the expected value ofthe random variable. 

$E \left[ u \left( \tilde { W } \right) \right] \leq u \left( E \left| \tilde { W } \right| \right)$ when u is concave 

Similarly, the expected value of a (strictly) convex function of a random variable is (strictly) greater than the same convex function of the expected value of the random variable. 

Proof There are three ways of motivating this result, but only one provides a fully general and rigorous proof. Without loss of generality, consider the concave case. 

1. One can reinterpret the defining inequality (3.2.1) in terms of a discrete random vector x˜ taking on the value x with probability π and $\mathbf { x } ^ { \prime }$ with probability $1 - \pi \cdot$ 

∀x 6= x<sup>0</sup> ∈ X, π ∈ (0, 1) 

$$
f \left(\pi \mathbf {x} + (1 - \pi) \mathbf {x} ^ {\prime}\right) \geq \pi f (\mathbf {x}) + (1 - \pi) f (\mathbf {x} ^ {\prime}),\tag{5.6.1}
$$

which just says that 

$$
f \left(E [ \tilde {\mathbf {x}} ]\right) \geq E \left[ f (\tilde {\mathbf {x}}) \right].\tag{5.6.2}
$$

An inductive argument can be used to extend the result to all discrete r.v.s with a finite number of possible values, but runs into problems if the number of possible values is either countably or uncountably infinite. 

2. Using a similar approach to that used with the Taylor series expansion in (5.3.2), take expectations on both sides of the first order condition for concavity (3.2.3) given by Theorem 3.2.3, where the two vectors considered are the mean $E \left[ \tilde { \mathbf { x } } \right]$ and a generic value x˜: 

$$
f (\tilde {\mathbf {x}}) \leq f (E [ \tilde {\mathbf {x}} ]) + f ^ {\prime} (E [ \tilde {\mathbf {x}} ]) (\tilde {\mathbf {x}} - E [ \tilde {\mathbf {x}} ]).\tag{5.6.3}
$$

Taking expectations on both sides, the first order term will again disappear, once more yielding: 

$$
f \left(E [ \tilde {\mathbf {x}} ]\right) \geq E \left[ f (\tilde {\mathbf {x}}) \right].\tag{5.6.4}
$$

3. One can also appeal to the second order condition for concavity, and the second order Taylor series expansion of f around $E \left[ \tilde { \mathbf { x } } \right]$ 

$$
E [ f (\tilde {x}) ] = f (E [ \tilde {x} ]) + \frac {1}{2} f ^ {\prime \prime} (x ^ {*}) \mathrm{Var} [ \tilde {x} ],\tag{5.6.5}
$$

for some $x ^ { * }$ in the support of x˜. However, this supposes that $x ^ { * }$ is fixed, whereas in fact it varies with the value taken on by x˜, and is itself a random variable, correlated with x˜. 

Accepting this (wrong) approximation, if f is concave, then by Theorem 3.2.4 the second derivative is non-positive and the variance is non-negative, so 

$$
E [ f (\tilde {x}) ] \leq f (E [ \tilde {x} ]).\tag{5.6.6}
$$

The arguments for convex functions, strictly concave functions and strictly concave functions are almost identical. 

Q.E.D. 

This result is often useful with functions such as $x \mapsto$ ln x and $\textstyle x \mapsto { \frac { 1 } { x } } .$ To get a feel for the extent to which $E [ f ( { \tilde { x } } ) ]$ differs from $f ( E [ { \tilde { x } } ] )$ , we can again use the following (wrong) second order Taylor approximation based on (5.3.8): 

$$
E [ f (\tilde {x}) ] \approx f (E [ \tilde {x} ]) + \frac {1}{2} f ^ {\prime \prime} (E [ \tilde {x} ]) \mathrm{Var} [ \tilde {x} ].\tag{5.6.7}
$$

This shows that the difference is larger the larger is the curvature of $f$ (as measured by the second derivative at the mean of x˜) and the larger is the variance of x˜. One area in which this idea can be applied is the computation of present values based on replacing uncertain future discount factors with point estimates derived from expected future interest rates. 

Another nice application of Jensen’s Inequality in finance is: 

Theorem 5.6.2 (Siegel’s Paradox) Current forward (relative) prices can not all equal expectedfuture spot prices. 

Proof Let $F _ { t }$ be the current forward price and $\tilde { S } _ { t + 1 }$ the unknown future spot price. If 

$$
E _ {t} \left[ \tilde {S} _ {t + 1} \right] = F _ {t},
$$

then Jensen’s Inequality tells us that 

$$
\frac {1}{\tilde {F} _ {t}} = \frac {1}{E _ {t} [ \tilde {S} _ {t + 1} ]} <   E _ {t} [ \frac {1}{\tilde {S} _ {t + 1}} ],
$$

except in the degenerate case where $\tilde { S } _ { t + 1 }$ is known with certainty at time t. But since the reciprocals of relatives prices are also relative prices, we have shown that our initial hypothesis is untenable in terms of a different numeraire. Revised: December 2, 1998 

Q.E.D. 

The original and most obvious application of Siegel’s paradox is in the case of currency exchange rates. In that case, $\left\{ \tilde { F } _ { t } \right\}$ and $\left\{ \tilde { S } _ { t } \right\}$ are stochastic processes representing forward and spot exhange rates respectively. It seems reasonable to assume that forward exchange rates are good predictors of spot exchange rates in the future, say: 

$$
\tilde {F} _ {t} = E _ {t} \left[ \tilde {S} _ {t + 1} \right].
$$

But this is an internally inconsistent hypothesis. 

However, Siegel’s paradox applies equally well to any theory which uses current prices as a predictor of future values. Another such theory which is enormously popular is the Efficient Markets Hypothesis of ?. In its general form, this says that current prices should fully reflect all available information about (expected) future values. Attempts to make the wordsfully reflect in any way mathematically rigorous quickly run into problems. 

## 5.7 Risk Aversion

An individual is risk averse if he or she is unwilling to accept, or indifferent to, any actuarially fair gamble. 

(An individual is strictly risk averse if he or she is unwilling to accept any actuarially fair gamble.) 

Figure 1.17.1 goes here. 

i.e. $\forall W _ { 0 }$ and $\forall p , h _ { 1 } , h _ { 2 }$ such that $p h _ { 1 } + ( 1 - p ) h _ { 2 } = 0$ 

$$
W _ {0} \succeq (\succ) W _ {0} + p h _ {1} + (1 - p) h _ {2}
$$

i.e. 

$$
u \left(W _ {0}\right) \geq (>) p u \left(W _ {0} + h _ {1}\right) + (1 - p) u \left(W _ {0} + h _ {2}\right)
$$

The following interpretation of the above definition of risk aversion is based on Jensen’s Inequality (see Section 5.6). 

In other words, a (strictly) risk averse individual is one whose VNM utility function is (strictly) concave. 

Similarly, a (strictly) risk loving individual is one whose VNM utility function is (strictly) convex. 

Finally, a risk neutral individual is one whose VNM utility function is affine. 

Most functions do not fall into any of these categories, and represent behaviour which is locally risk averse at some wealth levels and locally risk loving at other wealth levels. 

However, in most of what follows we will find it convenient to assume that individuals are globally risk averse. 

Individuals who are globally risk averse will never gamble, in the sense that they will never have a bet unless they believe that the expected return on the bet is positive. Thus assuming global risk aversion (and rational expectations) rules out the existence of lotteries (except with large rollovers) and most other forms of betting and gaming. 

We can distinguish between local and global risk aversion. An individual is locally risk averse at w if $u ^ { \prime \prime } ( w ) < 0$ and globally risk averse if $u ^ { \prime \prime } ( w ) < 0 \forall w$ 

Individuals who gamble are not globally risk averse but may still be locally risk averse around their current wealth level. 

Cut and paste relevant quotes from Purfield-Waldron papers in here. 

Some people are more risk averse than others; some functions are more concave than others; how do we measure this? 

The importance and usefulness of the Arrow-Pratt measures of risk aversion which we now define will become clearer as we proceed, in particular from the analysis of the portfolio choice problem: 

Definition 5.7.1 (The Arrow-Pratt coefficient of) absolute risk aversion is: 

$$
R _ {A} (w) = - u ^ {\prime \prime} (w) / u ^ {\prime} (w)
$$

which is the samefor u and $a u + b .$ 

Note that this varies with the level of wealth. 

$u ^ { \prime } \left( w \right)$ alone is meaningless, as u and $u ^ { \prime }$ can be multiplied by any positive constant and still represent the same preferences. However, the above ratio is independent of the expected utility function chosen to represent the preferences. 

Definition 5.7.2 (The Arrow-Pratt coefficient of) relative risk aversion is: 

$$
R _ {R} (w) = w R _ {A} (w)
$$

The utility function u exhibits increasing (constant, decreasing) absolute risk aversion (IARA, CARA, DARA) ⇐⇒ 

$$
R _ {A} ^ {\prime} (w) > (= , <  ) 0 \forall w.
$$

The utility function u exhibits increasing (constant, decreasing) relative risk aversion (IRRA, CRRA, DRRA) ⇐⇒ 

Revised: December 2, 1998 

$$
R _ {R} ^ {\prime} (w) > (= , <  ) 0 \forall w.
$$

Note: 

• CARA or IARA ⇒ IRRA 

• CRRA or DRRA ⇒ DARA 

Here are some examples of utility functions and their risk measures: 

• Quadratic utility (IARA, IRRA): 

$$
\begin{array}{r c l} {u (w)} & = & {w - \frac {b}{2} w ^ {2}, \qquad b > 0;} \\ {u ^ {\prime} (w)} & = & {1 - b w;} \\ {u ^ {\prime \prime} (w)} & = & {- b <   0} \\ {R _ {A} (w)} & = & {\frac {b}{1 - b w}} \\ {\frac {d R _ {A} (w)}{d w}} & = & {\frac {b ^ {2}}{(1 - b w) ^ {2}} > 0} \end{array}
$$

In this case, marginal utility is positive and utility increasing if and only if $w < 1 / b . \ 1 / b$ is called the bliss point of the quadratic utility function. For realism, $1 / b$ should be rather large and thus b rather small. 

• Negative exponential utility (CARA, IRRA): 

$$
\begin{array}{r c l} {u (w)} & = & {- e ^ {- b w}, \quad b > 0;} \\ {u ^ {\prime} (w)} & = & {b e ^ {- b w} > 0;} \\ {u ^ {\prime \prime} (w)} & = & {- b ^ {2} e ^ {- b w} <   0} \\ {R _ {A} (w)} & = & b \\ {\frac {d R _ {A} (w)}{d w}} & = & 0 \end{array}
$$

• Narrow power utility (CRRA, DARA): 

$$
u (w) = \frac {B}{B - 1} w ^ {1 - \frac {1}{B}}, w > 0, B > 0, B \neq 1
$$

The proofs in this case are left as an exercise. The solution is roughly as follows:<sup>4</sup> 

$$
\begin{array}{r c l} {u (z)} & = & {\frac {B}{B - 1} z ^ {1 - \frac {1}{B}}, z > 0, B > 0} \\ {u ^ {\prime} (z)} & = & {z ^ {- \frac {1}{B}}} \\ {u ^ {\prime \prime} (z)} & = & {- \frac {1}{B} z ^ {- \frac {1}{B} - 1}} \\ {R _ {A} (z)} & = & {\frac {1}{B} z ^ {- 1}} \\ {R _ {R} (z)} & = & {\frac {1}{B}} \\ {\frac {d R _ {A} (z)}{d z}} & = & {- \frac {1}{B} z ^ {- 2} <   0} \\ {\frac {d R _ {R} (z)}{d z}} & = & 0 \end{array}
$$

• Extended power utility $( ) ! ^ { 5 }$ 

$$
u (w) = \frac {1}{(C + 1) B} (A + B w) ^ {C + 1}
$$

Note that a risk neutral investor will seek to invest his or her entire wealth in the asset with the highest expected return. If all investors are risk neutral, then prices will adjust in equilibrium so that all securities have the same expected return. If there are risk averse or risk loving investors, then there is no reason for this result to hold, and in fact it almost certainly will not. 

## 5.8 The Mean-Variance Paradigm

Three arguments are commonly used to motivate the mean-variance framework for analysis of the portfolio choice problem: 

1. Taylor-approximated utility functions (see Section 2.8): 

$$
\begin{array}{r c l} {u (\tilde {W})} & = & {u (E [ \tilde {W} ]) + u ^ {\prime} (E [ \tilde {W} ]) (\tilde {W} - E [ \tilde {W} ])} \\ & + & {\frac {1}{2} u ^ {\prime \prime} (E [ \tilde {W} ]) (\tilde {W} - E [ \tilde {W} ]) ^ {2} + R _ {3}} \end{array}\tag{5.8.1}
$$

$$
R _ {3} = \sum_ {n = 3} ^ {\infty} \frac {1}{n !} u ^ {(n)} (E [ \tilde {W} ]) (\tilde {W} - E [ \tilde {W} ]) ^ {n}\tag{5.8.2}
$$

which implies: 

$$
\begin{array}{r c l} E [ u (\tilde {W}) ] & = & u (E [ \tilde {W} ]) + \frac {1}{2} u ^ {\prime \prime} (E [ \tilde {W} ]) \sigma^ {2} (\tilde {W}) + E [ R _ {3} ] \\ & \mathrm{where} & \\ & E [ R _ {3} ] & = \sum_ {n = 3} ^ {\infty} \frac {1}{n !} u ^ {(n)} (E [ \tilde {W} ]) m ^ {n} (\tilde {W}) \end{array}\tag{5.8.3}
$$

(5.8.4) 

It follows that the sign of the nth derivative of the utility function determines the direction of preference for the nth central moment of the probability distribution of terminal wealth. For example, a positive third derivative implies a preference for greater skewness. It can be shown fairly easily that an increasing utility function which exhibits non-increasing absolute risk aversion has a non-negative third derivative. 

## 2. Quadratic utility:

$$
{E [ u (\tilde {W}) ]} = {E [ \tilde {W} ] - \frac {b}{2} E [ \tilde {W} ^ {2} ]}\tag{5.8.5}
$$

$$
{ = } { E [ \tilde { W } ] - \frac { b } { 2 } \left( ( E [ \tilde { W } ] ) ^ { 2 } + \sigma ^ { 2 } ( \tilde { W } ) \right) }\tag{5.8.6}
$$

$$
{ = } { u ( E [ \tilde { W } ] ) - \frac { b } { 2 } \mathrm{Var} [ \tilde { W } ] }\tag{5.8.7}
$$

## 3. Normally distributed asset returns.

Note that the expected utility axioms are neither necessary nor sufficient to guarantee that the Taylor approximation to n moments is a valid representation of the utility function. Some counterexamples of both types are probably called for here, or maybe can be left as exercises. 

Extracts from my PhD thesis can be used to talk about signing the first three coefficients in the Taylor expansion, and to speculate about further extensions to higher moments. 

## 5.9 The Kelly Strategy

In a multi-period, discrete time, investment framework, investors will be concerned with both growth (return) and security (risk). There will be a trade-off between the two, and investors will be concerned with finding the optimal tradeoff. This, of course, depends on preferences, but some useful benchmarks exist. There are three ways of measuring growth: 

## 1. the expected wealth at time t

2. the expected rate of growth of wealth up to time t 

3. the expected first passage time to reach a critical level of wealth, say £1m Likewise, there are three ways of measuring security: 

1. the probability of reaching a critical level of wealth, say £1m, by a specific time t 

2. the probability that the wealth process lies above some critical path, say above $b _ { t }$ at time t, t = 1, 2, . . . 

3. the probability of reaching some goal U before falling to some low level of wealth L 

It can be shown that the ? strategy both maximises the long run exponential growth rate and minimises the expected time to reach large goals. All this is also covered in ? which is reproduced in ?. 

## 5.10 Alternative Non-Expected Utility Approaches

Those not happy with the explanations of choice under uncertainty provided within the expected utility paradigm have proposed various alternatives in recent years. These include both vague qualitative waffle about fun and addiction and more formal approaches looking at maximum or minimum possible payoffs, irrational expectations, etc. Before proceeding, the reader might want to review Section 3.2. 

## Chapter 6

# PORTFOLIO THEORY

## 6.1 Introduction

Portfolio theory is an important topic in the theory of choice under uncertainty. It deals with the problem facing an investor who must decide how to distribute an initial wealth of, say, $W _ { 0 }$ among a number of single-period investment opportunities, called securities or assets. 

The choice of portfolio will depend on both the investor’s preferences and his beliefs about the uncertain payoffs of the various securities. A mutualfund is just a special type of (managed) portfolio. 

The chapter begins by considering some issues of definition and measurement. Section 6.3 then looks at the portfolio choice problem in a general expected utility context. Section 6.4 considers the same problem from a mean-variance perspective. This leads on to a discussion of the properties of equilibrium security returns in Section 6.5. 

## 6.2 Notation and preliminaries

## 6.2.1 Measuring rates of return

Good background reading for this section is ?. 

A rate of interest (growth, inflation, $\hphantom { } \hphantom { } ⨏ \hphantom { } ⨏ \hphantom { } \{ d  \boldsymbol { c } . \boldsymbol { ) }$ is not properly defined unless we state the time period to which it applies and the method of compounding to be used. 

2% per annum is very different from 2% per month. 

Table 6.1 illustrates what happens to £100 invested at 10% per annum as we change the interval of compounding. The final calculation in the table uses the 

<table><tr><td>Annually</td><td>£100</td><td>→</td><td>£110</td></tr><tr><td>Semi-annually</td><td>£100</td><td>→</td><td>£100 × (1.05)2 = £110.25</td></tr><tr><td>Quarterly</td><td>£100</td><td>→</td><td>£100 × (1.025)4 = £110.381...</td></tr><tr><td>Monthly</td><td>£100</td><td>→</td><td>£100 × (1 + .10/12)12 = £110.471...</td></tr><tr><td>Weekly</td><td>£100</td><td>→</td><td>£100 × (1 + .10/52)52 = £110.506...</td></tr><tr><td>Daily</td><td>£100</td><td>→</td><td>£100 × (1 + .10/365)365 = £110.515...</td></tr><tr><td>Continuously</td><td>£100</td><td>→</td><td>£100 × e0.10 = £110.517...</td></tr></table>

## Compounded

Table 6.1: The effect of an interest rate of 10% per annum at different frequencies of compounding. 

fact that 

$$
\lim _ {n \to \infty} \left(1 + \frac {r}{n}\right) ^ {n} = e ^ {r}
$$

where $e \approx 2 . 7 1 8 2 . .$ 

This is sometimes used as the definition of e but others prefer to start with 

$$
e ^ {r} \equiv 1 + r + \frac {r ^ {2}}{2 !} + \frac {r ^ {3}}{3 !} + \ldots = \sum_ {j = 0} ^ {\infty} \frac {r ^ {j}}{j !}
$$

where n! $\equiv n \left( n - 1 \right) \left( n - 2 \right) . . . 3 . 2 . 1$ and $0 ! \equiv 1$ by convention. There are five concepts which we need to be familiar with: 

## 1. Discrete compounding:

$$
P _ {t} = \left(1 + \frac {r}{n}\right) ^ {n t} P _ {0}.
$$

We can solve this equation for any of five quantities given the other four: 

(a) present value 

(b) final value 

(c) implicit rate of return 

(d) time 

(e) interval of compounding 

Revised: December 2, 1998 

## 2. Continuous compounding:

$$
P _ {t} = e ^ {r t} P _ {0}.
$$

We can solve this equation for any of four quantities given the other three ((a)–(d) above). 

Note also that the exponential function is its own derivative; that $y = 1 + r$ is the tangent to $y = e ^ { r } \mathrm { a t } r = 0$ and hence that $e ^ { r } > 1 + r \forall r$ . In other words, given an initial value, continuous compounding yields a higher terminal value than discrete compounding for all interest rates, positive and negative, with equality for a zero interest rate only. Similarly, given a final value, continuous discounting yields a higher present value than does discrete. 

3. Aggregating and averaging returns across portfolios $( \tilde { r } _ { \mathbf { w } } = \mathbf { w } ^ { \top } \tilde { \mathbf { r } } )$ and over time: 

$$
\begin{array}{r c l} P _ {t} & = & e ^ {r t} P _ {0} \\ P _ {t + \Delta t} & = & e ^ {r \Delta t} P _ {t} \\ r & = & \frac {\ln P _ {t + \Delta t} - \ln P _ {t}}{\Delta t} \\ r (s) & = & \frac {d \ln P _ {s}}{d s} \\ \int_ {0} ^ {t} r (s) d s & = & \int_ {0} ^ {t} d \ln P _ {s} = \ln P _ {t} - \ln P _ {0} \\ P _ {t} & = & P _ {0} e ^ {\int_ {0} ^ {t} r (s) d s} \end{array}
$$

Discretely compounded rates aggregate nicely across portfolios; continuously compounded rates aggregate nicely across time. 

4. The (net) present value (NPV) of a stream of cash flows, 

$$
P _ {0}, P _ {1}, \ldots , P _ {T}
$$

is 

$$
N P V (r) \equiv \frac {P _ {0}}{(1 + r) ^ {0}} + \frac {P _ {1}}{(1 + r) ^ {1}} + \frac {P _ {2}}{(1 + r) ^ {2}} + \ldots + \frac {P _ {T}}{(1 + r) ^ {T}}.
$$

5. The internal rate ofreturn (IRR) of the stream of cash flows, 

$$
P _ {0}, P _ {1}, \ldots , P _ {T},
$$

is the solution of the polynomial of degree T obtained by setting the NPV equal to zero: 

$$
\frac {P _ {0}}{(1 + r) ^ {0}} + \frac {P _ {1}}{(1 + r) ^ {1}} + \frac {P _ {2}}{(1 + r) ^ {2}} + \ldots + \frac {P _ {T}}{(1 + r) ^ {T}} = 0.
$$

$\begin{array}{rcl}\boldsymbol{W}_0 & = & \text{the investor's initial wealth} \\ W_1 & = & \text{the investor's desired expected final wealth} \\ N & = & \text{number of risky assets} \\ r_f & = & \text{return on the riskfree asset} \\ \tilde{r}_j \in \Re & = & \text{return on jth risky asset} \\ \tilde{\mathbf{r}} \in \Re^N & = & (\tilde{r}_1, \ldots, \tilde{r}_N) \\ \mathbf{e} = E[\tilde{\mathbf{r}}] \in \Re^N & = & \text{vector of expected returns} \\ \mathbf{V} \in \Re^{N \times N} & = & \text{variance-covariance matrix of returns} \\ \mathbf{1} & = & (1, 1, \ldots, 1) \\ & = & N\text{-dimensional vector of 1s} \\ w_j \in \Re & = & \text{amount invested in jth risky asset} \\ \mathbf{w} \in \Re^N & = & (w_1, \ldots, w_n) \\ \tilde{r}_{\mathbf{w}} = \mathbf{w}^\top \tilde{\mathbf{r}} & = & \text{return on the portfolio w} \\ \mu \equiv E[\tilde{r}_{\mathbf{w}}] \equiv \frac{W_1}{W_0} \in \Re & = & \text{the investor's desired expected return} \end{array}$ 


Table 6.2: Notation for portfolio choice problem


In general, the polynomial defining the IRR has T (complex) roots. Conditions have been derived under which there is only one meaningful real root to this polynomial equation, in other words one corresponding to a positive IRR.<sup>1</sup> 

## Consider a quadratic example.

Simple rates of return are additive across portfolios, so we use them in one period cross sectional studies, in particular in this chapter. 

Continuously compounded rates of return are additive across time, so we use them in multi-period single variable studies, such as in Chapter 7. 

Consider as an example the problem of calculating mortgage repayments. 

## 6.2.2 Notation

The investment opportunity set for the portfolio choice problem will generally consist of N risky assets. From time to time, we will add a riskfree asset. The notation used throughout this chapter is set out in Table 6.2. The presentation is in terms of a single period problem, and the unconditional distribution of returns. The analysis of the multiperiod, infinite horizon, discrete time problem, concentrating on the conditional distribution of the next period’s returns given this period’s, is quite similar.<sup>2</sup> 

Definition 6.2.1 w is said to be a unit cost or normal portfolio ifits weights sum to $I \left( \mathbf { w } ^ { \top } \mathbf { 1 } = 1 \right)$ . 

The portfolio held by an investor with initial wealth $W _ { 0 }$ can be thought of either as a w with $\mathbf { w } ^ { \top } \mathbf { 1 } = W _ { 0 }$ or as the corresponding normal portfolio, $\frac { 1 } { W _ { 0 } } \mathbf { W }$ . It will hopefully be clear from the context which meaning of ‘portfolio’ is intended. 

Definition 6.2.2 w is said to be a zero cost or hedge portfolio if its weights sum to $O \left( \mathbf { w } ^ { \top } \mathbf { 1 } = 0 \right)$ . 

The vector of net trades carried out by an investor moving from the portfolio $\mathbf { w } _ { 0 }$ to the portfolio $\mathbf { w } _ { 1 }$ can be thought of as the hedge portfolio ${ \bf w } _ { 1 } - { \bf w } _ { 0 }$ 

Definition 6.2.3 Short-selling a security means owning a negative quantity of it. 

In practice short-selling means promising (credibly) to pay someone the same cash flows as would be paid by a security that one does not own, always being prepared, if required, to pay the current market price of the security to end the arrangement. Thus when short-selling is allowed w can have negative components; if shortselling is not allowed, then the portfolio choice problem will have non-negativity constraints, $w _ { i } \geq 0$ for $i = 1 , \ldots , N$ 

A number of further comments are in order at this stage. 

1. In the literature, initial wealth is often normalised to unity $( W _ { 0 } = 1 )$ , but the development of the theory will be more elegant if we avoid this. 

2. Since we will be dealing on occasion with hedge portfolios, we will in future avoid the concepts of rate ofreturn and net return, which are usually thought of as the ratio of profit to initial investment. These terms are meaningless for a hedge portfolio as the denominator is zero. 

Instead, we will speak of the gross return on a portfolio or the portfolio pay-$o f .$ This can be defined unambiguously as follows. There is no ambiguity about the payoff on one of the original securities, which is just the gross return per pound invested. The payoff on a unit cost or normal portfolio is equivalent to the gross return. It is just $\mathbf { w } ^ { \top } \tilde { \mathbf { r } }$ . The payoff on a zero cost portfolio can also be defined as $\mathbf { w } ^ { \top } \tilde { \mathbf { r } }$ 

Note that where we initially worked with net rates of return $( \textstyle { \frac { P _ { 1 } } { P _ { 0 } } } \mathrm { ~ - ~ } 1 )$ , we will deal henceforth with gross rates of return $\textstyle { \bigl ( } { \frac { P _ { 1 } } { P _ { 0 } } } { \bigr ) }$ 

## 6.3 The Single-period Portfolio Choice Problem

## 6.3.1 The canonical portfolio problem

Unless otherwise stated, we assume that individuals: 

1. have von Neumann-Morgenstern (VNM) utilities: 

i.e. preferences have the expected utility representation: 

$$
\begin{array}{r c l} v (\tilde {z}) & = & \operatorname{E} [ u (\tilde {z}) ] \\ & = & \int u (z) d F _ {\tilde {z}} (z) \end{array}
$$

where v is the utility function for random variables (gambles, lotteries) and u is the utility function for sure things. 

2. prefer more to less 

i.e. u is increasing: 

$$
u ^ {\prime} (z) > 0 \forall z\tag{6.3.1}
$$

3. are (strictly) risk-averse 

i.e. u is strictly concave: 

$$
u ^ {\prime \prime} (z) <   0 \forall z\tag{6.3.2}
$$

Date 0 investment: 

• $w _ { j }$ (pounds) in jth risky asset, $j = 1 , \ldots , N$ 

$\left( W _ { 0 } - \textstyle \sum _ { j } w _ { j } \right)$ in risk free asset 

Date 1 payoff: 

$w _ { j } \tilde { r } _ { j }$ from jth risky asset 

$( W _ { 0 } - \textstyle \sum _ { j } w _ { j } ) r _ { f }$ from risk free asset 

It is assumed here that there are no constraints on short-selling or borrowing (which is the same as short-selling the riskfree security). 

The solution is found as follows: 

Choose $w _ { j } \mathbf { s }$ to maximize expected utility of date 1 wealth, 

$$
\begin{array}{r c l} \tilde {W} & = & (W _ {0} - \sum_ {j} w _ {j}) r _ {f} + \sum_ {j} w _ {j} \tilde {r} _ {j} \\ & = & W _ {0} r _ {f} + \sum_ {j} w _ {j} (\tilde {r} _ {j} - r _ {f}) \end{array}
$$

Revised: December 2, 1998 

i.e. 

$$
\max _ {\{w _ {j} \}} f (w _ {1}, \dots , w _ {N}) \equiv E [ u (W _ {0} r _ {f} + \sum_ {j} w _ {j} (\tilde {r} _ {j} - r _ {f})) ]
$$

The first order conditions are: 

$$
E [ u ^ {\prime} (\tilde {W}) (\tilde {r} _ {j} - r _ {f}) ] = 0 \quad \forall j.\tag{6.3.3}
$$

The Hessian matrix of the objective function is: 

$$
\mathbf {A} \equiv E \left[ u ^ {\prime \prime} (\tilde {W}) (\tilde {\mathbf {r}} - r _ {f} \mathbf {1}) (\tilde {\mathbf {r}} - r _ {f} \mathbf {1}) ^ {\top} \right].\tag{6.3.4}
$$

$\mathbf { h } ^ { \top } \mathbf { A } \mathbf { h } < 0 \forall \mathbf { h } \neq \mathbf { 0 } _ { N }$ if and only if $u ^ { \prime \prime } < 0$ . Since we have assumed that investor behaviour is risk averse, A is a negative definite matrix and, by Theorem 3.2.4, f is a strictly concave (and hence strictly quasiconcave) function. Thus, under the present assumptions, Theorems 3.3.3 and 3.3.4 guarantee that the first order conditions have a unique solution. The trivial case in which the random returns are not really random at all can be ignored. 

The rest of this section should be omitted until I figure out what is going on. Another way of writing (6.3.3) is: 

$$
E [ u ^ {\prime} (\tilde {W}) \tilde {r} _ {j} ] = E [ u ^ {\prime} (\tilde {W}) ] r _ {f} \quad \forall j,\tag{6.3.5}
$$

or 

$$
\mathrm{Cov} \left[ u ^ {\prime} (\tilde {W}), \tilde {r} _ {j} \right] + E [ u ^ {\prime} (\tilde {W}) ] E [ \tilde {r} _ {j} ] = E [ u ^ {\prime} (\tilde {W}) ] r _ {f} \quad \forall j,\tag{6.3.6}
$$

or 

$$
E [ \tilde {r} _ {j} - r _ {f} ] = \frac {\operatorname{Cov} \left[ u ^ {\prime} (\tilde {W}) , \tilde {r} _ {j} \right]}{E [ u ^ {\prime} (\tilde {W}) ]} \quad \forall j,\tag{6.3.7}
$$

Suppose $p _ { j }$ is the price of the random payoff $\tilde { x } _ { j }$ . Then $\begin{array} { r } { \tilde { r } _ { j } = \frac { \tilde { x } _ { j } } { p _ { j } } } \end{array}$ and 

$$
p _ {j} = E \left[ \frac {u ^ {\prime} (\tilde {W})}{E [ u ^ {\prime} (\tilde {W}) ] r _ {f}} \tilde {x} _ {j} \right] \quad \forall j.\tag{6.3.8}
$$

In other words, payoffs are valued by taking their expected present value, using the stochastic discount factor $\frac { u ^ { \prime } ( \tilde { W } ) } { E [ u ^ { \prime } ( \tilde { W } ) ] r _ { f } }$ , which ends up being the same for all investors. Practical corporate finance and theoretical asset pricing models to a large extent are (or should be) concerned with analysing this discount factor. 

(We could consider here the explicit example with quadratic utility from the problem sets.) 

## 6.3.2 Risk aversion and portfolio composition

For the moment, assume only one risky asset $( N = 1 )$ 

We first consider the concept of local risk neutrality. The optimal investment in the risky asset is positive 

⇐⇒ 

The objective function is increasing at $a = 0$ 

⇐⇒ 

$$
f ^ {\prime} (a) > 0\tag{6.3.9}
$$

⇐⇒ 

$$
E [ u ^ {\prime} (W _ {0} r _ {f}) (\tilde {r} - r _ {f}) ] > 0\tag{6.3.10}
$$

⇐⇒ 

$$
u ^ {\prime} \left(W _ {0} r _ {f}\right) E [ (\tilde {r} - r _ {f}) ] > 0\tag{6.3.11}
$$

⇐⇒ 

$$
E [ \tilde {r} ] > E [ r _ {f} ] = r _ {f}
$$

This is the property of local risk neutrality — a risk averse investor will always prefer a little of a risky asset paying a higher expected return than $r _ { f }$ to none of the risky asset. 

Definition 6.3.1 Let $f \colon X \to \Re _ { + + }$ be a positive-valuedfunction defined on $X \subseteq$ $\Re _ { + + } ^ { k }$ . Then the elasticity of $f$ with respect to $x _ { i }$ at $\mathbf { x } ^ { * }$ is 

$$
\frac {x _ {i} ^ {*}}{f (\mathbf {x})} \frac {\partial f}{\partial x _ {i}} (\mathbf {x} ^ {*}).
$$

Roughly speaking, the elasticity is just $\textstyle { \frac { \partial \ln f } { \partial \ln x _ { i } , } }$ or the slope of the graph of the function on log-log graph paper. 

A function is said to be inelastic when the absolute value of the elasticity is less than unity; and elastic when the absolute value of the elasticity is greater than unity. The borderline case is called a unit elastic function. 

One useful application of elasticity is in analysing the behaviour of the total revenue function associated with a particular inverse demand function, $P ( Q )$ . We have: 

$$
{\frac {d P (Q) Q}{d Q}} = {q \frac {d P}{d Q} + P}\tag{6.3.12}
$$

$$
= P \left(1 + \frac {1}{\eta}\right).\tag{6.3.13}
$$

Revised: December 2, 1998 

Hence, total revenue is constant or maximised or minimised where elasticity equals −1; increasing when elasticity is less than −1 (demand is elastic); and decreasing when elasticity is between 0 and −1 (demand is inelastic). 

Now consider other properties of asset demands (assuming that $E \left[ \tilde { r } \right] > r _ { f } ) :$ 

$\mathrm { D A R A } \Rightarrow$ risky asset normal $\begin{array} { r } { \left( \frac { d a } { d W _ { 0 } } > 0 \right) } \end{array}$ 

$\begin{array} { r } { \mathbf { C } \mathbf { A } \mathbf { R } \mathbf { A } \Rightarrow \left( \frac { d a } { d W _ { 0 } } = 0 \right) } \end{array}$ 

$\mathbf { I A R A } \Rightarrow \mathbf { r i s k y }$ asset inferior $\begin{array} { r } { \left( \frac { d a } { d W _ { 0 } } < 0 \right) } \end{array}$ 

Define the wealth elasticity of demand for the risky asset to be 

$$
\eta = \frac {W _ {0}}{a} \frac {d a}{d W _ {0}}.\tag{6.3.14}
$$

Then we have 

$$
\begin{array}{r c l} \frac {d \left(\frac {a}{W _ {0}}\right)}{d W _ {0}} & = & \frac {W _ {0} \frac {d a}{d W _ {0}} - a}{W _ {0} ^ {2}} \\ & = & \frac {a}{W _ {0} ^ {2}} (\eta - 1). \end{array}
$$

Note that 

$$
\operatorname{sign} \left(\frac {d \frac {a}{W _ {0}}}{d W _ {0}}\right) = \operatorname{sign} (\eta - 1)\tag{6.3.15}
$$

since by assuming a positive expected risk premium on the risky asset we guarantee (by local risk-neutrality) that a is positive. 

• DRRA ⇒ increasing proportion of wealth invested in the risky asset $( \eta > 1 )$ 

• CRRA ⇒ constant proportion of wealth invested in the risky asset $( \eta = 1 )$ 

• IRRA ⇒ decreasing proportion of wealth invested in the risky asset $( \eta < 1 )$ 

## Theorem 6.3.1 DARA ⇒ RISKYASSETNORMAL

Proof By implicit differentiation of the now familiar first order condition (6.3.3), which can be written: 

$$
E [ u ^ {\prime} (W _ {0} r _ {f} + a (\tilde {r} - r _ {f})) (\tilde {r} - r _ {f}) ] = 0,\tag{6.3.16}
$$

we have 

$$
\frac {d a}{d W _ {0}} = \frac {E [ u ^ {\prime \prime} (\tilde {W}) (\tilde {r} - r _ {f}) ] r _ {f}}{- E [ u ^ {\prime \prime} (\tilde {W}) (\tilde {r} - r _ {f}) ^ {2} ]}.\tag{6.3.17}
$$

By concavity, the denominator is positive. Therefore: 

$$
\operatorname{sign} \left(d a / d W _ {0}\right) = \operatorname{sign} \left\{E \left[ u ^ {\prime \prime} (\tilde {W}) \left(\tilde {r} - r _ {f}\right) \right] \right\}\tag{6.3.18}
$$

We will show that both are positive. 

For decreasing absolute risk aversion:<sup>3</sup> 

$$
\begin{array}{r c l} \tilde {r} > r _ {f} & \Rightarrow & R _ {A} (\tilde {W}) <   R _ {A} (W _ {0} r _ {f}) \\ \tilde {r} \leq r _ {f} & \Rightarrow & R _ {A} (\tilde {W}) \geq R _ {A} (W _ {0} r _ {f}) \end{array}
$$

Multiplying both sides of each inequality by $- u ^ { \prime } ( \tilde { W } ) ( \tilde { r } - r _ { f } )$ gives respectively: 

$$
u ^ {\prime \prime} (\tilde {W}) (\tilde {r} - r _ {f}) > - R _ {A} (W _ {0} r _ {f}) u ^ {\prime} (\tilde {W}) (\tilde {r} - r _ {f})\tag{6.3.19}
$$

in the event that $\tilde { r } > r _ { f }$ , and 

$$
u ^ {\prime \prime} (\tilde {W}) (\tilde {r} - r _ {f}) \geq - R _ {A} (W _ {0} r _ {f}) u ^ {\prime} (\tilde {W}) (\tilde {r} - r _ {f})\tag{6.3.20}
$$

(the same result) in the event that $\tilde { r } \leq r _ { f }$ Integrating over both events implies: 

$$
E [ u ^ {\prime \prime} (\tilde {W}) (\tilde {r} - r _ {f}) ] > - R _ {A} (W _ {0} r _ {f}) E [ u ^ {\prime} (\tilde {W}) (\tilde {r} - r _ {f}) ],\tag{6.3.21}
$$

provided that $\tilde { r } > r _ { f }$ with positive probability. The RHS of inequality (6.3.21) is 0 at the optimum, hence the LHS is positive as claimed. 

Q.E.D. 

The other results are proved similarly (exercise!). 

## 6.3.3 Mutual fund separation

Commonly, investors delegate portfolio choice to mutual fund operators or managers. We are interested in conditions under which large groups of investors will agree on portfolio composition. For example, all investors with similar utility functions might choose the same portfolio, or all investors with similar probability beliefs might choose the same portfolio. More realistically, we may be able to define a group of investors whose portfolio choices all lie in a subspace of small dimension (say 2) of the N-dimensional portfolio space. The first such result is due to ?. 

## Theorem 6.3.2 ∃ Twofund monetary separation

i.e. Agents with different wealths (but the same increasing, strictly concave, VNM utility) hold the same risky unit cost portfolio, p<sup>∗</sup> say, (but may differ in the mix of the riskfree asset and risky portfolio) 

i.e. ∀ portfolios p, wealths $W _ { 0 } , \exists \lambda s . t .$ 

$$
E \left[ u \left(W _ {0} r _ {f} + \lambda W _ {0} \mathbf {p} ^ {* ^ {\top}} (\tilde {\mathbf {r}} - r _ {f} \mathbf {1})\right) \right] \geq E \left[ u \left(W _ {0} r _ {f} + \mathbf {p} ^ {\top} (\tilde {\mathbf {r}} - r _ {f} \mathbf {1})\right) \right]\tag{6.3.22}
$$

Risk-tolerance $( 1 / R _ { A } ( z ) )$ is linear (including constant) 

i.e. ∃ Hyperbolic Absolute Risk Aversion (HARA, incl. CARA) 

i.e. the utilityfunction is ofone ofthese types: 

• Extended power: $\begin{array} { r } { u ( z ) = \frac { 1 } { ( C + 1 ) B } ( A + B z ) ^ { C + 1 } } \end{array}$ 

• Logarithmic: $u ( z ) = \ln ( A + B z )$ 

• Negative exponential: $\begin{array} { r } { u ( z ) = - \frac { A } { B } \exp \{ B z \} } \end{array}$ 

where A, B and C are chosen to guarantee $u ^ { \prime } > 0 , u ^ { \prime \prime } < 0 \nonumber$ 

i.e. marginal utility satisfies 

$$
u ^ {\prime} (z) = (A + B z) ^ {C} \quad \text { or } \quad u ^ {\prime} (z) = A \exp \{B z \}\tag{6.3.23}
$$

where A, B and C are again chosen to guarantee $u ^ { \prime } > 0 , u ^ { \prime \prime } < 0 .$ 

Proof The proof that these conditions are necessary for two fund separation is difficult and tedious. The interested reader is referred to ?. 

We will show that $u ^ { \prime } ( z ) = ( A + B z ) ^ { C }$ is sufficient for two-fund separation. 

The optimal dollar investments $w _ { j }$ are the unique solution to the first order conditions: 

$$
0 = E [ u ^ {\prime} (\tilde {W}) \frac {\delta \tilde {W}}{\delta w _ {i}} ]\tag{6.3.24}
$$

$$
{ = } { E [ ( A + B \tilde { W } ) ^ { C } ( \tilde { r } _ { i } - r _ { f } ) ] }\tag{6.3.25}
$$

$$
= E \left[ \left(A + B W _ {0} r _ {f} + \sum_ {j} B w _ {j} \left(\tilde {r} _ {j} - r _ {f}\right)\right) ^ {C} \left(\tilde {r} _ {i} - r _ {f}\right) \right],\tag{6.3.26}
$$

or equivalently to the system of equations 

$$
E [ (1 + \sum_ {j} \frac {B w _ {j}}{A + B W _ {0} r _ {f}} (\tilde {r} _ {j} - r _ {f})) ^ {C} (\tilde {r} _ {i} - r _ {f}) ] = 0\tag{6.3.27}
$$

or 

$$
E [ (1 + \sum_ {j} x _ {j} (\tilde {r} _ {j} - r _ {f})) ^ {C} (\tilde {r} _ {i} - r _ {f}) ] = 0\tag{6.3.28}
$$

where 

$$
x _ {j} = \frac {B w _ {j}}{A + B W _ {0} r _ {f}}.
$$

The unique solutions for $x _ { j }$ are clearly independent of $W _ { 0 }$ which does not appear in (6.3.28). 

Since A and B do not appear either, the unique solutions for $x _ { j }$ are also independent of those parameters. 

However, they do depend on $C .$ . 

But the risky portfolio weights are 

$$
\begin{array}{r c l} \frac {w _ {i}}{\sum_ {j} w _ {j}} & = & \frac {B w _ {i} / (A + B W _ {0} r _ {f})}{\sum_ {j} B w _ {j} / (A + B W _ {0} r _ {f})} \\ & = & \frac {x _ {i}}{\sum_ {j} x _ {j}} \end{array}\tag{6.3.29}
$$

(6.3.30) 

and so are also independent of initial wealth. 

Since the dollar investment in the jth risky asset satisfies: 

$$
w _ {j} = x _ {j} (\frac {A}{B} + W _ {0} r _ {f})\tag{6.3.31}
$$

we also have in this case that the dollar investment in the common risky portfolio is a linear function of the initial wealth. The other sufficiency proofs are similar and are left as exercises. 

Q.E.D. 

Some humorous anecdotes about Cass may now follow. 

## 6.4 Mathematics of the Portfolio Frontier

## 6.4.1 The portfolio frontier in $\Re ^ { N }$ : risky assets only

## The portfolio frontier

Definition 6.4.1 The (mean-variance) portfolio frontier is the set of solutions to the mean-variance portfolio choice problemfaced by a (risk-averse) investor with an initial wealth of $W _ { 0 }$ who desires an expectedfinal wealth ofat least $W _ { 1 } \equiv \mu W _ { 0 }$ (or, equivalently, an expected rate of return of µ), but with the smallest possible variance offinal wealth. 

The mean-variance frontier can also be called the two-moment portfolio frontier, in recognition of the fact that the same approach can be extended (with difficulty) to higher moments. 

The mean-variance portfolio frontier is a subset of the portfolio space, which is just $\Re ^ { N }$ . However, introductory treatments generally present it (without proof) as the envelope function, in mean-variance space or mean-standard deviation space $( { \Re } _ { + } \times { \Re } )$ , of the variance minimisation problem. 

## Definition 6.4.2 w is a frontier portfolio

its return has the minimum variance among all portfolios that have the same cost, $\mathbf { w } ^ { \top } \mathbf { 1 }$ , and the same expected payoff, $\mathbf { w } ^ { \top }$ e. 

We will begin by supposing that all assets are risky. Formally, the frontier portfolio corresponding to initial wealth $W _ { 0 }$ and expected return $\mu$ (expected terminal wealth $\mu W _ { 0 } )$ is the solution to the quadratic programming problem: 

$$
\min _ {\mathbf {w}} \mathbf {w} ^ {\top} \mathbf {V} \mathbf {w}\tag{6.4.1}
$$

subject to the linear constraints: 

$$
\mathbf {w} ^ {\top} \mathbf {1} = W _ {0}\tag{6.4.2}
$$

and 

$$
\mathbf {w} ^ {\top} \mathbf {e} \geq W _ {1} = \mu W _ {0}.\tag{6.4.3}
$$

The first constraint is just the budget constraint, while the second constraint states that the expected rate of return on the portfolio is at least the desired mean return µ. 

The frontier in this case is the set of solutions for all values of $W _ { 0 }$ and $W _ { 1 } \left( \mathrm { o r } \mu \right)$ to this variance minimisation problem, or to the equivalent maximisation problem: 

$$
\max _ {\mathbf {w}} - \mathbf {w} ^ {\top} \mathbf {V} \mathbf {w}\tag{6.4.4}
$$

subject to the same linear constraints (6.4.2) and (6.4.3). 

The properties of this two-moment frontier are well known, and can be found, for example, in ? or ?. The notation here follows ?. The derivation of the meanvariance frontier is generally presented in the literature in terms of portfolio weight vectors or, equivalently, assuming that initial wealth, $W _ { 0 }$ , equals 1. This assumption is not essential and will be avoided. 

## The solution

The inequality constrained maximisation problem (6.4.4) is just a special case of the canonical quadratic programming problem considered at the end of Section 3.5, except that it has explicitly one equality constraint and one inequality constraint. 

To avoid degeneracies, we require: 

1. that not every portfolio has the same expected return, i.e. 

$$
\mathbf {e} \neq E [ \tilde {r} _ {1} ] \mathbf {1},\tag{6.4.5}
$$

and in particular that $N > 1$ 

2. that the variance-covariance matrix, V, is (strictly) positive definite. We already know from (1.12.4) that V must be positive semi-definite, but we require this slightly stronger condition. To see why, suppose 

$$
\exists \mathbf {w} \neq \mathbf {0} _ {N} s. t. \mathbf {w} ^ {\top} \mathbf {V} \mathbf {w} = 0\tag{6.4.6}
$$

Then $\exists \mathrm { ~ a ~ }$ portfolio whose return w ${ ^ \top } \tilde { \mathbf { r } } = \tilde { r } _ { \mathbf { w } }$ has zero variance. 

This implies that $\tilde { r } _ { \mathbf { w } } = r _ { 0 } ( \mathrm { s a y } ) \ \mathrm { w } . \mathrm { p } . 1$ or, essentially, that this portfolio is riskless. 

Arbitrage will force the returns on all riskless assets to be equal in equilibrium, so this situation is equivalent economically to the introduction of a riskless asset later. 

In the portfolio problem, the place of the matrix A in the canonical quadratic programming problem is taken by the (symmetric) negative definite matrix, −V, which is just the negative of the variance-covariance matrix of asset returns; $\mathbf { g } ^ { 1 } =$ $\mathbf { 1 } ^ { \top }$ and $\alpha _ { 1 } = W _ { 0 } ;$ ; and $\mathbf { g } ^ { 2 } = \mathbf { e } ^ { \top }$ and $\alpha _ { 2 } = W _ { 1 }$ . (6.4.5) guarantees that the $2 \times N$ matrix G is of full rank 2. 

The parallels are a little fuzzy in the case of the budget constraint since it is really an equality constraint. 

(3.5.39) says that the optimal w is a linear combination of the two columns of the $N \times 2$ matrix 

$$
\mathbf {V} ^ {- 1} \mathbf {G} ^ {\top} \left(\mathbf {G V} ^ {- 1} \mathbf {G} ^ {\top}\right) ^ {- 1},
$$

with columns weighted by initial wealth $W _ { 0 }$ and expected final wealth, $W _ { 1 }$ We will call these columns g and h and write the solution as 

$$
\mathbf {w} = W _ {0} \mathbf {g} + W _ {1} \mathbf {h} = W _ {0} (\mathbf {g} + \mu \mathbf {h}).\tag{6.4.7}
$$

Revised: December 2, 1998 

The components of g and h are functions of the means and variances of security returns. Thus the vector of optimal portfolio proportions, 

$$
\frac {1}{W _ {0}} \mathbf {w} = \mathbf {g} + \mu \mathbf {h},\tag{6.4.8}
$$

is independent of the initial wealth $W _ { 0 }$ 

It is easy to see the economic interpretation of g and h: 

• g is the frontier portfolio corresponding to $W _ { 0 } = 1$ and $W _ { 1 } = 0$ . In other words, it is the normal portfolio which would be held by an investor whose objective was to (just) go bankrupt with minimum variance. 

• Similarly, h is the frontier portfolio corresponding to $W _ { 0 } = 0$ and $W _ { 1 } = 1$ In other words, it is the hedge portfolio which would be purchased by a variance-minimising investor in order to increase his expected final wealth by one unit. 

Alternatively, (3.5.35) says that the optimal w is a linear combination of the two columns of the $N \times 2$ matrix 

$$
\frac {1}{2} \mathbf {V} ^ {- 1} \mathbf {G} ^ {\top} = \left( \begin{array}{c c} \frac {1}{2} \mathbf {V} ^ {- 1} \mathbf {1} & \frac {1}{2} \mathbf {V} ^ {- 1} \mathbf {e} \end{array} \right),
$$

with columns weighted by the Lagrange multipliers corresponding to the two constraints. We will call the Lagrange multipliers $2 \gamma / C$ and $2 \lambda / A$ respectively, where we define: 

$$
A \equiv \mathbf {1} ^ {\top} \mathbf {V} ^ {- 1} \mathbf {e} = \mathbf {e} ^ {\top} \mathbf {V} ^ {- 1} \mathbf {1}\tag{6.4.9}
$$

$$
B \equiv {\bf e} ^ {\top} {\bf V} ^ {- 1} {\bf e} > 0\tag{6.4.10}
$$

$$
C \equiv {\bf 1} ^ {\top} {\bf V} ^ {- 1} {\bf 1} > 0\tag{6.4.11}
$$

and 

$$
D \equiv B C - A ^ {2}\tag{6.4.12}
$$

and the inequalities follow from the fact that $\mathbf { V } ^ { - 1 }$ (like V) is positive definite. This allows the solution to be written as: 

$$
\mathbf {w} = \frac {\gamma}{C} (\mathbf {V} ^ {- 1} \mathbf {1}) + \frac {\lambda}{A} (\mathbf {V} ^ {- 1} \mathbf {e}).\tag{6.4.13}
$$

$\scriptstyle { \frac { 1 } { C } } ( \mathbf { V } ^ { - 1 } \mathbf { 1 } )$ and $\scriptstyle { \frac { 1 } { A } } ( \mathbf { V } ^ { - 1 } \mathbf { e } )$ are both unit portfolios, so $\gamma + \lambda = W _ { 0 }$ . We know that for the portfolio which minimises variance for a given initial wealth, regardless of expected final wealth, the corresponding Lagrange multiplier, $\lambda = 0$ . Thus $\scriptstyle { \frac { \gamma } { C } } ( \mathbf { V } ^ { - 1 } \mathbf { 1 } )$ is the global minimum variance portfolio with cost $W _ { 0 }$ (which in fact equals $\gamma$ in this case) and $\scriptstyle { \frac { 1 } { C } } ( \mathbf { V } ^ { - 1 } \mathbf { 1 } )$ is the global minimum variance unit cost portfolio, which we will denote w<sub>MVP</sub>. 

In fact, we can combine (6.4.7) and (6.4.13) and write the solution as: 

$$
\mathbf {w} = W _ {0} \left(\mathbf {w} _ {\mathrm{MVP}} + \left(\mu - \frac {A}{C}\right) \mathbf {h}\right).\tag{6.4.14}
$$

The details are left as an exercise.<sup>4</sup> 

The set of solutions to this quadratic programming problem for all possible $( W _ { 0 } , W _ { 1 } )$ combinations (including negative $W _ { 0 } )$ is the vector subspace of the portfolio space, which is generated either by the vectors g and h or by the vectors $\mathbf { w _ { M V P } }$ and h (or by any pair of linearly independent frontier portfolios). 

In $\Re ^ { N }$ , the set of unit cost frontier portfolios is the line passing thru g, parallel to h. 

It follows immediately that the frontier (like any straight line in $\Re ^ { N } )$ is a convex set, and can be generated by linear combinations of any pair of frontier portfolios with weights of the form α and $( 1 - \alpha )$ 

An important exercise at this stage is to work out the means, variances and covariances of the returns on w<sub>MVP</sub>, g and h. They will drop out of the portfolio decomposition below. 

The portfolio weight vectors g and h are 

$$
\textbf {g} = \frac {1}{D} [ B (\mathbf {V} ^ {- 1} \mathbf {1}) - A (\mathbf {V} ^ {- 1} \mathbf {e}) ]\tag{6.4.15}
$$

$$
\textbf {h} = \frac {1}{D} [ C (\mathbf {V} ^ {- 1} \mathbf {e}) - A (\mathbf {V} ^ {- 1} \mathbf {1}) ]\tag{6.4.16}
$$

We have 

$$
\mathrm{Var} [ \tilde {r} _ {\mathbf {g}} ] = \mathbf {g} ^ {\top} \mathbf {V} \mathbf {g} = \frac {B}{D}\tag{6.4.17}
$$

$$
\mathrm{Var} [ \tilde {r} _ {\mathbf {h}} ] = \mathbf {h} ^ {\top} \mathbf {V h} = \frac {C}{D}\tag{6.4.18}
$$

from which it follows that $D > 0$ 

## Orthogonal decomposition of portfolios

At this stage, we must introduce a scalar product on the portfolio space, namely that based on the variance-covariance matrix V. Since V is a non-singular, positive definite matrix, it defines a well behaved scalar product and all the standard results on orthogonal projection (&c.) from linear algebra are valid. 

Two portfolios $\mathbf { w } _ { 1 }$ and $\mathbf { w } _ { 2 }$ are orthogonal with respect to this scalar product ⇐⇒ 

$$
\mathbf {w} _ {1} ^ {\top} \mathbf {V} \mathbf {w} _ {2} = 0
$$

$$
\begin{array}{l} \stackrel {{\longleftrightarrow}} {{\Longleftrightarrow}} \\ \operatorname{Cov} \left[ \mathbf {w} _ {1} ^ {\top} \tilde {\mathbf {r}}, \mathbf {w} _ {2} ^ {\top} \tilde {\mathbf {r}} \right] = 0 \\ \Longleftrightarrow \end{array}
$$

the random variables representing the returns on the portfolios are uncorrelated. Thus, the terms ‘orthogonal’ and ‘uncorrelated’ may legitimately, and shall, be applied interchangeably to pairs of portfolios. Furthermore, the squared length of a weight vector corresponds to the variance of its returns. 

Note that $\mathbf { w _ { M V P } }$ and h are orthogonal vectors in this sense. In fact, we have the following theorem: 

Theorem 6.4.1 Ifw is afrontier portfolio and u is a zero mean hedge portfolio, then w and u are uncorrelated. 

Proof There is probably a full version of this proof lost somewhere but the following can be sorted out. 

Since $\mathbf { w _ { M V P } }$ is collinear with $\mathbf { V } ^ { - 1 } \mathbf { 1 }$ , it is orthogonal to all portfolios w for which $\mathbf { w } ^ { \top } \mathbf { V } \mathbf { V } ^ { - 1 } \mathbf { 1 } = 0$ or in other words to all portfolios for which $\mathbf { w } ^ { \top } \mathbf { 1 } = 0$ . But these are precisely all hedge portfolios, including h. 

Similarly, any portfolio collinear with $\mathbf { V } ^ { - 1 }$ e is orthogonal to all portfolios with zero expected return, since $\mathbf { w } ^ { \top } \mathbf { V } \mathbf { V } ^ { - 1 } \mathbf { e } = 0$ or in other words $\mathbf { w } ^ { \top } \mathbf { e } = 0$ 

Q.E.D. 

Some pictures are in order at this stage. 

For $N = 3 ,$ , in the set of portfolios costing $W _ { 0 }$ (the $W _ { 0 }$ simplex), the iso-variance curves are concentric ellipses, the iso-mean curves are parallel lines, and the solutions for different $\mu \mathbf { s }$ (or $W _ { 1 } \mathbf { s } )$ are the tangency points between these ellipses and lines, which themselves lie on a line orthogonal (in the sense defined above) to the iso-mean lines. The centre of the concentric ellipses is at the global minimum variance portfolio corresponding to $W _ { 0 }$ $W _ { 0 } \mathbf { w _ { M V P } }$ . A similar geometric interpretation can be applied in higher dimensions. 

? has some nice pictures of the frontier in portfolio space, as opposed to meanvariance space. 

At this stage, recall the definition of $\beta$ in (5.2.2). 

We will now derive an orthogonal decomposition of a portfolio q into two frontier portfolios and a zero-mean zero-cost portfolio and prove that the coefficients on the two frontier portfolios are the $\beta \mathbf { s }$ of q with respect to those portfolios and sum to unity. 

We can always choose an orthogonal basis for the portfolio frontier. 

For any frontier portfolio $\mathbf { p } \neq \mathbf { w } _ { \mathbf { M V P } }$ , there is a unique unit cost frontier portfolio $\mathbf { z _ { p } }$ which is orthogonal to p. 

Another important exercise is to figure out the relationship between $E \left[ \tilde { r } _ { \mathbf { p } } \right]$ and $E \left\lceil \tilde { r } _ { \mathbf { z _ { p } } } \right\rceil$ 

Any two frontier portfolios span the frontier, in particular any unit cost p 6= w<sub>MVP</sub> and $\mathbf { z _ { p } }$ (or the original basis, $\mathbf { w _ { M V P } }$ and h). 

Any (frontier or non-frontier) portfolio q with non-zero cost $W _ { 0 }$ can be written in the form $\bf f _ { q } + u _ { q }$ where 

$$
\begin{array}{r c l} \mathbf {f _ {q}} & \equiv & W _ {0} \left(\mathbf {g} + E [ \tilde {r} _ {\mathbf {q}} ] \mathbf {h}\right) \\ & = & W _ {0} \left(\beta_ {\mathbf {q p}} \mathbf {p} + (1 - \beta_ {\mathbf {q p}}) \mathbf {z _ {p}}\right) (\mathrm{say}) \end{array}\tag{6.4.19}
$$

(6.4.20) 

is the frontier portfolio with expected return $E [ \tilde { r } _ { \mathbf { q } } ]$ and cost $W _ { 0 }$ and $\mathbf { u _ { q } }$ is a hedge portfolio with zero expected return. Geometrically, this decomposition is equivalent to the orthogonal projection of q onto the frontier. 

Theorem 6.4.1 shown that any portfolio sharing these properties of $\mathbf { u _ { q } }$ is uncorrelated with all frontier portfolios.<sup>5</sup> 

If p is a unit cost frontier portfolio (i.e. the vector of portfolio proportions) and q is an arbitrary unit cost portfolio, then the following decomposition therefore holds: 

$$
\mathbf {q} = \mathbf {f _ {q}} + \mathbf {u _ {q}} = \beta_ {\mathbf {q p}} \mathbf {p} + (1 - \beta_ {\mathbf {q p}}) \mathbf {z _ {p}} + \mathbf {u _ {q}}\tag{6.4.21}
$$

where the three components (i.e. the vectors p, $\mathbf { z _ { p } }$ and $\bf { u } _ { q } )$ are mutually orthogonal. 

We can extend this decomposition to cover 

1. portfolio proportions (orthogonal vectors) 

2. portfolio proportions (scalars/components) 

3. returns (uncorrelated random variables) 

4. expected returns (numbers) 

Note again the parallel between orthogonal portfolio vectors and uncorrelated portfolio returns/payoffs. 

We will now derive the relation: 

$$
E [ \tilde {r} _ {\mathbf {q}} ] - E [ \tilde {r} _ {\mathbf {z _ {p}}} ] = \beta_ {\mathbf {q p}} (E [ \tilde {r} _ {\mathbf {p}} ] - E [ \tilde {r} _ {\mathbf {z _ {p}}} ])\tag{6.4.22}
$$

which may be familiar from earlier courses in financial economics and which is quite general and neither requires asset returns to be normally distributed nor any assumptions about preferences. 

Since Cov $\left[ { \tilde { r } } _ { \mathbf { u _ { q } } } , { \tilde { r } } _ { \mathbf { p } } \right] = \operatorname { C o v } \left[ { \tilde { r } } _ { \mathbf { z _ { p } } } , { \tilde { r } } _ { \mathbf { p } } \right] = 0$ , taking covariances with $\tilde { r } _ { \mathbf { p } }$ in (6.4.21) gives: 

$$
\mathrm{Cov} \left[ \tilde {r} _ {\mathbf {q}}, \tilde {r} _ {\mathbf {p}} \right] = \mathrm{Cov} \left[ \tilde {r} _ {\mathbf {f} _ {\mathbf {q}}}, \tilde {r} _ {\mathbf {p}} \right] = \beta_ {\mathbf {q p}} \mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ]\tag{6.4.23}
$$

or 

$$
\beta_ {\mathbf {q p}} = \frac {\mathrm{Cov} [ \tilde {r} _ {\mathbf {q}} , \tilde {r} _ {\mathbf {p}} ]}{\mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ]}\tag{6.4.24}
$$

Thus $\beta$ in (6.4.21) has its usual definition from probability theory, given by (5.2.2).<sup>6</sup> Reversing the roles of $\mathbf { p }$ and $\mathbf { z _ { p } }$ , it can be seen that 

$$
\beta_ {\mathbf {q z _ {p}}} = 1 - \beta_ {\mathbf {q p}}\tag{6.4.25}
$$

Taking expected returns in (6.4.21) yields again: 

$$
E [ \tilde {r} _ {\mathbf {q}} ] = \beta_ {\mathbf {q p}} E [ \tilde {r} _ {\mathbf {p}} ] + (1 - \beta_ {\mathbf {q p}}) E [ \tilde {r} _ {\mathbf {z _ {p}}} ],\tag{6.4.26}
$$

which can be rearranged to obtain (6.4.22). 

The Global Minimum Variance Portfolio 

$$
\mathrm{Var} [ \tilde {r} _ {\mathbf {g} + \mu \mathbf {h}} ] = \mathbf {g} ^ {\top} \mathbf {V} \mathbf {g} + 2 \mu (\mathbf {g} ^ {\top} \mathbf {V} \mathbf {h}) + \mu^ {2} (\mathbf {h} ^ {\top} \mathbf {V} \mathbf {h})\tag{6.4.27}
$$

which has its minimum at 

$$
\mu = - \frac {\mathbf {g} ^ {\top} \mathbf {V h}}{\mathbf {h} ^ {\top} \mathbf {V h}}\tag{6.4.28}
$$

The latter expression reduces to $A / C$ and the minimum value of the variance is $1 / C .$ . The global minimum variance portfolio is denoted MVP. 

$$
\begin{array}{r c l} \operatorname{Cov} \left[ \tilde {r} _ {\mathbf {h}}, \tilde {r} _ {\mathrm{MVP}} \right] & = & \mathbf {h} ^ {\top} \mathbf {V} \left(\mathbf {g} - \frac {\mathbf {g} ^ {\top} \mathbf {V h}}{\mathbf {h} ^ {\top} \mathbf {V h}} \mathbf {h}\right) \\ & = & \mathbf {h} ^ {\top} \mathbf {V g} - \frac {\mathbf {g} ^ {\top} \mathbf {V h . h} ^ {\top} \mathbf {V h}}{\mathbf {h} ^ {\top} \mathbf {V h}} = 0 \end{array}\tag{6.4.29}
$$

(6.4.30) 

i.e. the returns on the portfolio with weights h and the minimum variance portfolio are uncorrelated. 

Further, if $p$ is any portfolio, the MVP is the minimum variance combination of itself and $p ,$ i.e. $a = 0$ solves: 

$$
\min _ {a} \frac {1}{2} \mathrm{Var} [ \tilde {r} _ {a p + (1 - a) \mathrm{MVP}} ]\tag{6.4.31}
$$

which has necessary and sufficient first order condition: 

$$
a \mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ] + (1 - 2 a) \mathrm{Cov} [ \tilde {r} _ {\mathbf {p}}, \tilde {r} _ {\mathrm{MVP}} ] - (1 - a) \mathrm{Var} [ \tilde {r} _ {\mathrm{MVP}} ] = 0\tag{6.4.32}
$$

Hence, setting $a = 0 \cdot$ 

$$
\mathrm{Cov} [ \tilde {r} _ {\mathbf {p}}, \tilde {r} _ {\mathrm{MVP}} ] - \mathrm{Var} [ \tilde {r} _ {\mathrm{MVP}} ] = 0\tag{6.4.33}
$$

and the covariance of any portfolio with MVP is $1 / C$ . 

## 6.4.2 The portfolio frontier in mean-variance space: risky assets only

## The portfolio frontier in mean-variance and in mean-standard deviation space

We now move on to consider the mean-variance relationship along the portfolio frontier. 

The mean, $\mu ,$ and variance, $\sigma ^ { 2 }$ , of the rate of return associated with each point on the frontier are related by the quadratic equation: 

$$
(\sigma^ {2} - \mathrm{Var} [ \mathbf {w} _ {\mathrm{MVP}} ^ {\top} \tilde {\mathbf {r}} ]) = \phi (\mu - \mathrm{E} [ \mathbf {w} _ {\mathrm{MVP}} ^ {\top} \tilde {\mathbf {r}} ]) ^ {2},\tag{6.4.34}
$$

where the shape parameter $\phi = C / D$ represents the variance of the (gross) return on the hedge portfolio, h. The two-moment frontier is generally presented as the graph in mean-variance space of this parabola, showing the most desirable distributions attainable, but the frontier can also be thought of as a plane in portfolio space or as a line in portfolio weight space. The latter interpretations are far more useful when it comes to extending the analysis to higher moments. 

The equations of the frontier in mean-variance and mean-standard deviation space can be derived heuristically using the following stylized diagram illustrating the portfolio decomposition. 

Figure 3A goes here. 

Applying Pythagoras’ theorem to the triangle with vertices at $0 , p$ and MVP yields: 

$$
\sigma^ {2} = \operatorname{Var} [ \tilde {r} _ {\mathbf {p}} ] = \operatorname{Var} [ \tilde {r} _ {\mathrm{MVP}} ] + \left(\mu - \frac {A}{C}\right) ^ {2} \operatorname{Var} [ \tilde {r} _ {\mathbf {h}} ]\tag{6.4.35}
$$

Revised: December 2, 1998 

Recall from the coordinate geometry of conic sections that 

$$
\mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ] = \mathrm{Var} [ \tilde {r} _ {\mathrm{MVP}} ] + (\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]) ^ {2} \mathrm{Var} [ \tilde {r} _ {\mathbf {h}} ]\tag{6.4.36}
$$

or 

$$
V (\mu) = \frac {1}{C} + \frac {C}{D} \left(\mu - \frac {A}{C}\right) ^ {2}\tag{6.4.37}
$$

is a quadratic equation in $\mu .$ . 

i.e. the equation of the parabola with vertex at 

$$
\operatorname{Var} [ \tilde {r} _ {\mathbf {p}} ] = \operatorname{Var} [ \tilde {r} _ {\mathrm{MVP}} ] = \frac {1}{C}\tag{6.4.38}
$$

$$
\mu = E [ \tilde {r} _ {\mathrm{MVP}} ] = \frac {A}{C}\tag{6.4.39}
$$

Thus in mean-variance space, the frontier is a parabola. 

Figure 3.11.2 goes here: indicate position of g on figure. 

Similarly, in mean-standard deviation space, the frontier is a hyperbola. To see this, recall that: 

$$
\sigma^ {2} = \operatorname{Var} [ \tilde {r} _ {\mathrm{MVP}} ] + \left(\mu - \frac {A}{C}\right) ^ {2} \operatorname{Var} [ \tilde {r} _ {\mathbf {h}} ]\tag{6.4.40}
$$

is the equation of the hyperbola with vertex at 

$$
\sigma = \sqrt {\mathrm{Var} [ \tilde {r} _ {\mathrm{MVP}} ]} = \sqrt {\frac {1}{C}}\tag{6.4.41}
$$

$$
\mu = \frac {A}{C}\tag{6.4.42}
$$

centre at $\sigma = 0 , \mu = A / C$ and asymptotes as indicated. 

Figure 3.11.1 goes here: indicate position of g on figure. 

The other half of the hyperbola $( \sigma < 0 )$ has no economic meaning. 

Recall two other types of conic sections: 

$\mathrm { V a r } [ \tilde { r } _ { \mathbf { h } } ] < 0$ (impossible) gives a circle with center $( 1 / C , A / C )$ 

$\mathrm { V a r } [ \tilde { r } _ { \mathrm { M V P } } ] = 0$ (the presence of a riskless asset) allows the square root to be taken on both sides: 

$$
\sigma = \pm \left(\mu - \frac {A}{C}\right) \sqrt {\mathrm{Var} [ \tilde {r} _ {\mathbf {h}} ]}\tag{6.4.43}
$$

$i . e .$ the conic section becomes the pair of lines which are its asymptotes otherwise. 

Portfolios on which the expected return, $\mu ,$ exceeds ${ \bf w } _ { \mathrm { M V P } } ^ { \top } \mathbf { e }$ are termed efficient, since they maximise expected return given variance; other frontier portfolios minimise expected return given variance and are inefficient. 

A frontier portfolio is said to be an efficient portfolio iff 

its expected return exceeds the minimum variance expected return $A / C = E [ \tilde { r } _ { \mathrm { M V P } } ] .$ The set of efficient portfolios in $\Re ^ { N }$ (or efficient frontier) is the half-line emanating from MVP in the direction of h, and hence is also a convex set. 

Convex combinations (but not all linear combinations with weights summing to 1) of efficient portfolios are efficient. 

We now consider zero-covariance (zero-beta) portfolios. In portfolio weight space, can easily construct a frontier portfolio having zero covariance with any given frontier portfolio: 

Figure 3B goes here. 

Algebraically, the expected return $\mu _ { 0 }$ on the zero-covariance frontier portfolio of a frontier portfolio with expected return $\mu$ solves: 

$$
\operatorname{Cov} \left[ \tilde {r} _ {\mathrm{MVP}} + (\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]) \tilde {r} _ {\mathbf {h}}, \tilde {r} _ {\mathrm{MVP}} + (\mu_ {0} - E [ \tilde {r} _ {\mathrm{MVP}} ]) \tilde {r} _ {\mathbf {h}} \right] = 0\tag{6.4.44}
$$

or, since $\tilde { r } _ { \mathbf { h } }$ and $\tilde { r } _ { \mathrm { M V P } }$ are uncorrelated: 

$$
\mathrm{Var} [ \tilde {r} _ {\mathrm{MVP}} ] + (\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]) (\mu_ {0} - E [ \tilde {r} _ {\mathrm{MVP}} ]) \mathrm{Var} [ \tilde {r} _ {\mathbf {h}} ] = 0\tag{6.4.45}
$$

To make this true, we must have 

$$
(\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]) (\mu_ {0} - E [ \tilde {r} _ {\mathrm{MVP}} ]) <   0\tag{6.4.46}
$$

or $\mu$ and $\mu _ { 0 }$ on opposite sides of $E [ \tilde { r } _ { \mathrm { M V P } } ]$ as shown. 

There is a neat trick which allows zero-covariance portfolios to be plotted in meanstandard deviation space. 

Implicit differentiation of the $\mu - \sigma$ relationship (6.4.35) along the frontier yields: 

$$
\frac {d \mu}{d \sigma} = \frac {\sigma}{(\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]) \mathrm{Var} [ \tilde {r} _ {\mathbf {h}} ]}\tag{6.4.47}
$$

so the tangent at $( \sigma , \mu )$ intercepts the $\mu$ axis at 

$$
\mu - \sigma \frac {d \mu}{d \sigma} = \mu - \frac {\sigma^ {2}}{(\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]) \mathrm{Var} [ \tilde {r} _ {\mathbf {h}} ]}\tag{6.4.48}
$$

$$
{ = } { \mu - \frac { \mathrm{Var} [ \tilde { r } _ { \mathrm{MVP} } ] } { ( \mu - E [ \tilde { r } _ { \mathrm{MVP} } ] ) \mathrm{Var} [ \tilde { r } _ { \mathbf { h } } ] } - ( \mu - E [ \tilde { r } _ { \mathrm{MVP} } ] ) }\tag{6.4.49}
$$

$$
{ = } { E [ \tilde { r } _ { \mathrm{MVP} } ] - \frac { \operatorname{Var} [ \tilde { r } _ { \mathrm{MVP} } ] } { ( \mu - E [ \tilde { r } _ { \mathrm{MVP} } ] ) \operatorname{Var} [ \tilde { r } _ { \mathbf { h } } ] } }\tag{6.4.50}
$$

Revised: December 2, 1998 

where we substituted for $\sigma ^ { 2 }$ from the definition of the frontier. 

A little rearrangement shows that expression (6.4.50) satisfies the equation (6.4.45) defining the return on the zero-covariance portfolio. 

In mean-standard deviation space the picture is like this: 

Figure 3.15.1 goes here. 

To find $\mathbf { z _ { p } }$ in mean-variance space, note that the line joining $( \sigma ^ { 2 } , \mu )$ to the MVP intercepts the $\mu$ axis at: 

$$
\mu - \sigma^ {2} \frac {\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]}{\sigma^ {2} - \mathrm{Var} [ \tilde {r} _ {\mathrm{MVP}} ]} = \mu - \sigma^ {2} \frac {\mu - E [ \tilde {r} _ {\mathrm{MVP}} ]}{(\mu - E [ \tilde {r} _ {\mathrm{MVP}}) ^ {2} \mathrm{Var} [ \tilde {r} _ {\mathbf {h}} ]}\tag{6.4.51}
$$

After cancellation, this is exactly the first expression (6.4.48) for the zero-covariance return we had on the previous page. 

Figure 3.15.2 goes here. 

## Alternative derivations

The treatment of the portfolio frontier with risky assets only concludes with some alternative derivations following closely ?. They should probably be omitted altogether at this stage. 

1. The variance minimisation solution from first principles. 

It can be seen that w is the solution to: 

$$
\min _ {\{\mathbf {w}, \mathbf {\theta}, \mathbf {\theta} \}} L = \frac {1}{2} \mathbf {w} ^ {\top} \mathbf {V} \mathbf {w} + \lambda (\mu - \mathbf {w} ^ {\top} \mathbf {e}) + \gamma (W _ {0} - \mathbf {w} ^ {\top} \mathbf {1})\tag{6.4.52}
$$

which has necessary and sufficient first order conditions: 

$$
{\frac {\partial L}{\partial \mathbf {w}}} = {\mathbf {V} \mathbf {w} - \lambda \mathbf {e} - \gamma \mathbf {1} = \mathbf {0}}\tag{6.4.53}
$$

$$
\frac {\partial L}{\partial \lambda} = \mu - \mathbf {w} ^ {\top} \mathbf {e} = 0\tag{6.4.54}
$$

$$
{\frac {\partial L}{\partial \gamma}} = {W _ {0} - \mathbf {w} ^ {\top} \mathbf {1} = 0}\tag{6.4.55}
$$

The solution can be found by premultiplying the FOC (6.4.13) in turn by $\mathbf { e } ^ { \top }$ and $\mathbf { 1 } ^ { \top }$ and using the constraints yields: 

$$
\mu = \lambda (\mathbf {e} ^ {\top} \mathbf {V} ^ {- 1} \mathbf {e}) + \gamma (\mathbf {e} ^ {\top} \mathbf {V} ^ {- 1} \mathbf {1})\tag{6.4.56}
$$

$$
1 = \lambda (\mathbf {1} ^ {\top} \mathbf {V} ^ {- 1} \mathbf {e}) + \gamma (\mathbf {1} ^ {\top} \mathbf {V} ^ {- 1} \mathbf {1})
$$

(6.4.57) 

The solutions for λ and $\gamma$ are: 

$$
\lambda = \frac {C \mu - A}{D}\tag{6.4.58}
$$

$$
\gamma = \frac {B - A \mu}{D}\tag{6.4.59}
$$

2. Derivation of (6.4.22). 

If we only have frontier portfolio $p$ and interior portfolio $q ,$ , we get a frontier (in $\mu { - } \sigma$ space) entirely within the previous frontier and tangent to it at $p .$ 

The frontiers must have the same slope at $p \mathrm { : }$ 

Figure 3C goes here. 

We already saw that the outer frontier has slope $\frac { E [ \tilde { r } _ { \mathbf { p } } - \tilde { r } _ { \mathbf { z } _ { \mathbf { p } } } ] } { \sqrt { \mathrm { V a r } [ \tilde { r } _ { \mathbf { p } } ] } }$ 

At the point on the inner frontier with $w _ { \mathbf { q } }$ invested in $q$ and $( 1 - w _ { \mathbf { q } } )$ in p, 

$$
\mu = E [ \tilde {r} _ {\mathbf {p}} ] + w _ {\mathbf {q}} (E [ \tilde {r} _ {\mathbf {q}} - \tilde {r} _ {\mathbf {p}} ])\tag{6.4.60}
$$

$$
\begin{array}{r l r} \sigma^ {2} & = & w _ {\mathbf {q}} ^ {2} \mathrm{Var} [ \tilde {r} _ {\mathbf {q}} ] \\ & & + 2 w _ {\mathbf {q}} (1 - w _ {\mathbf {q}}) \mathrm{Cov} [ \tilde {r} _ {\mathbf {p}}, \tilde {r} _ {\mathbf {q}} ] + (1 - w _ {\mathbf {q}}) ^ {2} \mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ] \end{array}\tag{6.4.61}
$$

Differentiating these w.r.t. $w _ { \mathbf { q } } .$ : 

$$
{\frac {d \mu}{d w _ {\mathbf {q}}}} = {E [ \tilde {r} _ {\mathbf {q}} - \tilde {r} _ {\mathbf {p}} ]}\tag{6.4.62}
$$

$$
\begin{array}{r c l} 2 \sigma \frac {d \sigma}{d w _ {\mathbf {q}}} & = & 2 w _ {\mathbf {q}} \mathrm{Var} [ \tilde {r} _ {\mathbf {q}} ] \\ & & + 2 (1 - 2 w _ {\mathbf {q}}) \mathrm{Cov} [ \tilde {r} _ {\mathbf {p}}, \tilde {r} _ {\mathbf {q}} ] - 2 (1 - w _ {\mathbf {q}}) \mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ] (6. 4) \end{array}\tag{6.4.63}
$$

Taking the ratio and setting $w _ { \mathbf { q } } = 0$ gives the slope of the inner frontier at $p \mathrm { : }$ 

$$
\frac {d \mu}{d \sigma} = \frac {E [ \tilde {r} _ {\mathbf {q}} - \tilde {r} _ {\mathbf {p}} ]}{\frac {2 \mathrm{Cov} [ \tilde {r} _ {\mathbf {p}} , \tilde {r} _ {\mathbf {q}} ] - 2 \mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ]}{2 \sqrt {\mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ]}}}\tag{6.4.64}
$$

Equating this to the slope of the outer frontier, setting 

$$
\beta_ {\mathbf {q p}} = \frac {\mathrm{Cov} [ \tilde {r} _ {\mathbf {p}} , \tilde {r} _ {\mathbf {q}} ]}{\mathrm{Var} [ \tilde {r} _ {\mathbf {p}} ]}\tag{6.4.65}
$$

and rearranging yields: 

$$
E [ \tilde {r} _ {\mathbf {q}} ] - E [ \tilde {r} _ {\mathbf {z _ {p}}} ] = \beta_ {\mathbf {q p}} (E [ \tilde {r} _ {\mathbf {p}} ] - E [ \tilde {r} _ {\mathbf {z _ {p}}} ])\tag{6.4.66}
$$

Revised: December 2, 1998 

## 6.4.3 The portfolio frontier in $\Re ^ { N }$ : riskfree and risky assets

We now consider the mathematics of the portfolio frontier when there is a riskfree asset. 

In this case, the frontier portfolio solves: 

$$
\min _ {\mathbf {w}} \frac {1}{2} \mathbf {w} ^ {\top} \mathbf {V} \mathbf {w}\tag{6.4.67}
$$

$$
\mathrm{s.t.} \quad \mathbf {w} ^ {\top} \mathbf {e} + (1 - \mathbf {w} ^ {\top} \mathbf {1}) r _ {f} = \mu\tag{6.4.68}
$$

There is no longer a restriction on portfolio weights, and whatever is not invested in the N risky assets is assumed to be invested in the riskless asset. 

The solution (which can be left as an exercise) is by a similar method to the case where all assets were risky: 

$$
\mathbf {w} _ {p} = \mathbf {V} ^ {- 1} (\mathbf {e} - r _ {f} \mathbf {1}) \frac {\mu - r _ {f}}{H}\tag{6.4.69}
$$

where 

$$
H = (\mathbf {e} - \mathbf {1} r _ {f}) ^ {\top} \mathbf {V} ^ {- 1} (\mathbf {e} - \mathbf {1} r _ {f}) = B - 2 A r _ {f} + C r _ {f} ^ {2} > 0 \forall r _ {f}\tag{6.4.70}
$$

Along the frontier, we have: 

$$
\sigma = \left\{ \begin{array}{l l} \frac {\mu - r _ {f}}{\sqrt {H}} & \text {if} \mu \geq r _ {f}, \\ - \frac {\mu - r _ {f}}{\sqrt {H}} & \text {if} \mu <   r _ {f}, \end{array} \right.\tag{6.4.71}
$$

## 6.4.4 The portfolio frontier in mean-variance space: riskfree and risky assets

We can now establish the shape of the mean-standard deviation frontier with a riskless asset. 

Graphically, in mean-standard deviation space, combining any portfolio p with the riskless asset in proportions a and $( 1 - a )$ gives a portfolio with expected return 

$$
a E [ \tilde {r} _ {\mathbf {p}} ] + (1 - a) r _ {f} = r _ {f} + a (E [ \tilde {r} _ {\mathbf {p}} ] - r _ {f})
$$

and standard deviation of returns $a \sqrt { \mathrm { V a r } [ \tilde { r } _ { \mathbf { p } } ] }$ 

i.e. these portfolios trace out the ray in $\sigma { - } \mu$ space emanating from $( 0 , r _ { f } )$ and passing through $p .$ 

For each $\sigma$ the highest return attainable is along the ray from $r _ { f }$ which is tangent to the frontier generated by the risky assets. 

On this ray, the riskless asset is held in combination with the tangency portfolio t. This only makes sense for $r _ { f } < A / C = E [ \tilde { r } _ { m v p } ]$ 

Above t, there is a negative weight on the riskless asset — i.e. borrowing. 

Figure 3D goes here. 

## Limited borrowing

Unlimited borrowing as allowed in the preceding analysis is unrealistic. Consider what happens 

1. with margin constraints on borrowing: 

Figure 3E goes here. 

The frontier is the envelope of all the finite rays through risky portfolios, extending as far as the borrowing constraint allows. 

## 2. with differential borrowing and lending rates:

Figure 3F goes here. 

There is a range of expected returns over which a pure risky strategy provides minimum variance; 

lower expected returns are achieved by riskless lending; 

and higher expected returns are achieved by riskless borrowing. 

## 6.5 Market Equilibrium and the Capital Asset Pricing Model

## 6.5.1 Pricing assets and predicting security returns

Need more waffle here about prediction and the difficulties thereof and the properties of equilibrium prices and returns. 

We are looking for assumptions concerning probability distributions that lead to useful and parsimonious asset pricing models. The CAPM restrictions are the best known. At a very basic level, they can be expressed by saying that every investor has mean-variance preferences. This can be achieved either by restricting preferences to be quadratic or the probability distribution of asset returns to be normal. CAPM is basically a single-period model, but can be extended by assuming that return distributions are stable over time. ? and ? have generalised the distributional conditions. 

Recall also the limiting behaviour of the variance of the return on an equally weighted portfolio as the number of securities included goes to infinity. If securities are added in such a way that the average of the variance terms and the average of the covariance terms are stable, then the portfolio variance approaches the average covariance as a lower bound. 

## 6.5.2 Properties of the market portfolio

Let 

$m _ { j }$ = weight of security j in the market portfolio m 

$$
W _ {0} ^ {i} (> 0) = \text { individual   } i \text { 's   initial   wealth }
$$

$$
\begin{array}{r c l} w _ {i j} & = & \text { proportion   of   individual } i \text { 's   initial   wealth } \\ & & \text { invested   in } j \text {-th   security } \end{array}
$$

Then total wealth is defined by 

$$
W _ {m 0} \equiv \sum_ {i = 1} ^ {I} W _ {0} ^ {i}\tag{6.5.1}
$$

and in equilibrium the relation 

$$
\sum_ {i = 1} ^ {I} w _ {i j} W _ {0} ^ {i} = m _ {j} W _ {m 0} \quad \forall j\tag{6.5.2}
$$

must hold. Dividing by $W _ { m 0 }$ yields: 

$$
\sum_ {i = 1} ^ {I} w _ {i j} \frac {W _ {0} ^ {i}}{W _ {m 0}} = m _ {j} \quad \forall j\tag{6.5.3}
$$

and thus in equilibrium the market portfolio is a convex combination of individual portfolios. 

## 6.5.3 The zero-beta CAPM

Theorem 6.5.1 (Zero-beta CAPM theorem) Ifevery investor holds a mean-variance frontier portfolio, then the market portfolio, m, is a mean-variance frontier portfolio, and hence, ∀q, the CAPM equation 

$$
E [ \tilde {r} _ {\mathbf {q}} ] = (1 - \beta_ {\mathbf {q m}}) E [ \tilde {r} _ {\mathbf {z} _ {\mathbf {m}}} ] + \beta_ {\mathbf {q m}} E [ \tilde {r} _ {\mathbf {m}} ]\tag{6.5.4}
$$

holds. 

Theorem 6.5.2 All strictly risk-averse investors hold frontier portfolios if and only if 

$$
E \left[ \tilde {r} _ {\mathbf {u _ {q}}} | \tilde {r} _ {\mathbf {f _ {q}}} \right] = 0 \quad \forall \mathbf {q}\tag{6.5.5}
$$

Note the subtle distinction between uncorrelated returns (in the definition of the decomposition) and independent returns (in this theorem). They are the same only for the normal distribution and related distributions. 

We can view the market portfolio as a frontier portfolio under two fund separation. If p is a frontier portfolio, then we showed earlier that for purely mathematical reasons in the definition of a frontier portfolio: 

$$
E [ \tilde {r} _ {\mathbf {q}} ] = (1 - \beta_ {\mathbf {q p}}) E [ \tilde {r} _ {\mathbf {z _ {p}}} ] + \beta_ {\mathbf {q p}} E [ \tilde {r} _ {\mathbf {p}} ]\tag{6.5.6}
$$

If two fund separation holds, then individuals hold frontier portfolios. Since the market portfolio is then on the frontier, it follows that: 

$$
E [ \tilde {r} _ {\mathbf {q}} ] = (1 - \beta_ {\mathbf {q m}}) E [ \tilde {r} _ {\mathbf {z} _ {\mathbf {m}}} ] + \beta_ {\mathbf {q m}} E [ \tilde {r} _ {\mathbf {m}} ]\tag{6.5.7}
$$

where 

$$
\tilde {r} _ {\mathbf {m}} = \sum_ {j = 1} ^ {N} m _ {j} \tilde {r} _ {j}\tag{6.5.8}
$$

$$
\beta_ {\mathbf {q m}} = \frac {\mathrm{Cov} [ \tilde {r} _ {\mathbf {q}} , \tilde {r} _ {\mathbf {m}} ]}{\mathrm{Var} [ \tilde {r} _ {\mathbf {m}} ]}\tag{6.5.9}
$$

This implies for any particular security, from the economic assumptions of equilibrium and two fund separation: 

$$
E [ \tilde {r} _ {j} ] = (1 - \beta_ {j \mathbf {m}}) E [ \tilde {r} _ {\mathbf {z} _ {\mathbf {m}}} ] + \beta_ {j \mathbf {m}} E [ \tilde {r} _ {\mathbf {m}} ]\tag{6.5.10}
$$

This relation is the ? Zero-Beta version of the Capital Asset Pricing Model (CAPM). 

## 6.5.4 The traditional CAPM

Now we add the risk free asset, which will allow us to determine the tangency portfolio, t, and to talk about Capital Market Line (return v. standard deviation) and the Security Market Line (return v. β). 

Normally in equilibrium there is zero aggregate supply of the riskfree asset. Recommended reading for this part of the course is ?, ?, ? and ?. 

Now we can derive the traditional CAPM. Note that by construction 

$$
r _ {f} = E \left[ \tilde {r} _ {\mathbf {z _ {t}}} \right].\tag{6.5.11}
$$

Revised: December 2, 1998 

Theorem 6.5.3 (Separation Theorem) The risky asset holdings of all investors who hold mean-variance frontier portfolios are in the proportions given by the tangency portfolio, t. 

Theorem 6.5.4 (Traditional CAPM Theorem) If every investor holds a meanvariance frontier portfolio, then the market portfolio of risky assets, m, is the tangency portfolio, t, and hence, ∀q, the traditional CAPM equation 

$$
E \left[ \tilde {r} _ {\mathbf {q}} \right] = \left(1 - \beta_ {\mathbf {q m}}\right) r _ {f} + \beta_ {\mathbf {q m}} E \left[ \tilde {r} _ {\mathbf {m}} \right]\tag{6.5.12}
$$

holds. 

Theorem 6.5.4 is sometimes known as the Sharpe-Lintner Theorem. 

The riskless rate is unique by the No Arbitrage Principle, since otherwise a greedy investor would borrow an infinite amount at the lower rate and invest it at the higher rate, which is impossible in equilibrium. 

We can also think about what happens the CAPM if there are different riskless borrowing and lending rates (see ?). If all individuals face this situation in equi librium, realism demands that both riskless assets are in zero aggregate supply and hence that all investors hold risky assets only. 

Note that the No Arbitrage Principle also allows us to rule out correlation matrices for risky assets which permit the construction of portfolios with zero return variance, i.e. synthetic riskless assets. 

Assume that a riskless asset exists, with return $r _ { f } < E [ \tilde { r } _ { \mathrm { m v p } } ]$ 

If the distributional conditions for two fund separation are satisfied, then the tangency portfolio, t, must be the market portfolio of risky assets in equilibrium. We know then that for any portfolio q (with or without a riskless component): 

$$
E [ \tilde {r} _ {\mathbf {q}} ] - r _ {f} = \beta_ {\mathbf {q m}} (E [ \tilde {r} _ {\mathbf {m}} ] - r _ {f})\tag{6.5.13}
$$

This is the traditional Sharpe-Lintner version of the CAPM. 

Figure 4A goes here. 

The next theorem relates to the mean-variance efficiency of the market portfolio. 

## Theorem 6.5.5 If

1. the distributional conditionsfor twofund separation are satisfied; 

2. risky assets are in strictly positive supply; and 

3. investors have strictly increasing (concave) utilityfunctions 

then the market/tangency portfolio is efficient. 

Proof By Jensen’s inequality and monotonicity, the riskless asset dominates any portfolio with 

$$
E [ \tilde {r} ] <   r _ {f}\tag{6.5.14}
$$

for 

$$
E [ u (W _ {0} (1 + \tilde {r})) ] \leq u (E [ W _ {0} (1 + \tilde {r}) ])\tag{6.5.15}
$$

$$
<   u (W _ {0} (1 + r _ {f}))\tag{6.5.16}
$$

Hence the expected returns on all individuals’ portfolios exceed $r _ { f }$ 

It follows that the expected return on the market portfolio must exceed $r _ { f }$ . 

Q.E.D. 

Now we can calculate the risk premium of the market portfolio. 

CAPM gives a relation between the risk premia on individual assets and the risk premium on the market portfolio. 

The risk premium on the market portfolio must adjust in equilibrium to give market-clearing. 

In some situations, the risk premium on the market portfolio can be written in terms of investors’ utility functions. 

Assume there is a riskless asset and returns are multivariate normal (MVN). Recall the first order conditions for the canonical portfolio choice problem: 

$$
0 = E [ u _ {i} ^ {\prime} (\tilde {W} _ {i}) (\tilde {r} _ {j} - r _ {f}) ] \quad \forall i, j\tag{6.5.17}
$$

$$
= E \left[ u _ {i} ^ {\prime} \left(\tilde {W} _ {i}\right) \right] E \left[ \tilde {r} _ {j} - r _ {f} \right] + \operatorname{Cov} \left[ u _ {i} ^ {\prime} \left(\tilde {W} _ {i}\right), \tilde {r} _ {j} \right]\tag{6.5.18}
$$

$$
{ = } { E [ u _ { i } ^ { \prime } ( \tilde { W } _ { i } ) ] E [ \tilde { r } _ { j } - r _ { f } ] + E [ u _ { i } ^ { \prime \prime } ( \tilde { W } _ { i } ) ] \mathrm{Cov} \left[ \tilde { W } _ { i } , \tilde { r } _ { j } \right] }\tag{6.5.19}
$$

using the definition of covariance and Stein’s lemma for MVN distributions. Rearranging: 

$$
\frac {E [ \tilde {r} _ {j} - r _ {f} ]}{\theta_ {i}} = \mathrm{Cov} \left[ \tilde {W} _ {i}, \tilde {r} _ {j} \right]\tag{6.5.20}
$$

where 

$$
\theta_ {i} \equiv \frac {- E [ u _ {i} ^ {\prime \prime} (\tilde {W} _ {i}) ]}{E [ u _ {i} ^ {\prime} (\tilde {W} _ {i}) ]}\tag{6.5.21}
$$

is the i-th investor’s global absolute risk aversion. Since 

$$
\tilde {W} _ {i} = W _ {0} ^ {i} (1 + r _ {f} + \sum_ {k = 1} ^ {N} w _ {i k} (\tilde {r} _ {k} - r _ {f}))\tag{6.5.22}
$$

we have, dropping non-stochastic terms, 

$$
\operatorname{Cov} \left[ \tilde {W} _ {i}, \tilde {r} _ {j} \right] = \operatorname{Cov} \left[ W _ {0} ^ {i} \sum_ {k = 1} ^ {N} w _ {i k} \tilde {r} _ {k}, \tilde {r} _ {j} \right]\tag{6.5.23}
$$

Revised: December 2, 1998 

Hence, 

$$
\frac {E [ \tilde {r} _ {j} - r _ {f} ]}{\theta_ {i}} = \mathrm{Cov} \left[ W _ {0} ^ {i} \sum_ {k = 1} ^ {N} w _ {i k} \tilde {r} _ {k}, \tilde {r} _ {j} \right]\tag{6.5.24}
$$

Summing over $i ,$ this gives (since we have $\Sigma _ { i } W _ { 0 } ^ { i } w _ { i k } \ = \ W _ { 0 } ^ { m } w _ { m k }$ by marketclearing and $\begin{array} { r } { \sum _ { k } w _ { m k } \tilde { r } _ { k } = \tilde { r } _ { \mathbf { m } } } \end{array}$ by definition): 

$$
E [ \tilde {r} _ {j} - r _ {f} ] (\sum_ {i = 1} ^ {I} \theta_ {i} ^ {- 1}) = W _ {m 0} \mathrm{Cov} [ \tilde {r} _ {\mathbf {m}}, \tilde {r} _ {j} ]\tag{6.5.25}
$$

or 

$$
E [ \tilde {r} _ {j} - r _ {f} ] = (\sum_ {i = 1} ^ {I} \theta_ {i} ^ {- 1}) ^ {- 1} W _ {m 0} \mathrm{Cov} [ \tilde {r} _ {\mathbf {m}}, \tilde {r} _ {j} ]\tag{6.5.26}
$$

$i . e .$ , in equilibrium, the risk premium on the $j { \cdot } \mathrm { t h }$ asset is the product of the aggregate relative risk aversion of the economy and the covariance between the return on the $j \mathrm { - t h }$ asset and the return on the market. 

Now take the average over $j$ weighted by market portfolio weights: 

$$
E [ \tilde {r} _ {\mathbf {m}} - r _ {f} ] = (\sum_ {i = 1} ^ {I} \theta_ {i} ^ {- 1}) ^ {- 1} W _ {m 0} \mathrm{Var} [ (\tilde {} ] \tilde {r} _ {\mathbf {m}})\tag{6.5.27}
$$

$i . e .$ , in equilibrium, the risk premium on the market is the product of the aggregate relative risk aversion of the economy and the variance of the return on the market. Equivalently, the return to variability of the market equals the aggregate relative risk aversion. 

We conclude with some examples. 

1. Negative exponential utility: 

$$
u _ {i} (z) = - \frac {1}{a _ {i}} \exp \{- a _ {i} z \} \qquad a _ {i} > 0\tag{6.5.28}
$$

implies: 

$$
(\sum_ {i = 1} ^ {I} \theta_ {i} ^ {- 1}) ^ {- 1} = (\sum_ {i = 1} ^ {I} a _ {i} ^ {- 1}) ^ {- 1} > 0\tag{6.5.29}
$$

and hence the market portfolio is efficient. 

## 2. Quadratic utility:

$$
u _ {i} (z) = a _ {i} z - \frac {b _ {i}}{2} z ^ {2} \quad a _ {i}, b _ {i} > 0\tag{6.5.30}
$$

implies: 

$$
(\sum_ {i = 1} ^ {I} \theta_ {i} ^ {- 1}) ^ {- 1} = \left(\sum_ {i = 1} ^ {I} \left(\frac {a _ {i}}{b _ {i}} - E [ \tilde {W} _ {i} ]\right)\right) ^ {- 1}\tag{6.5.31}
$$

This result can also be derived without assuming MVN and using Stein’s lemma. 

## Chapter 7

# INVESTMENT ANALYSIS

## 7.1 Introduction

[To be written.] 

## 7.2 Arbitrage and the Pricing of Derivative Securities

## 7.2.1 The binomial option pricing model

This still has to be typed up. It follows very naturally from the stuff in Section 5.4. 

## 7.2.2 The Black-Scholes option pricing model

Fischer Black died in 1995. In 1997, Myron Scholes and Robert Merton were awarded the Nobel Prize in Economics ‘for a new method to determine the value of derivatives.’ See 

http://www.nobel.se/announcement-97/economy97.html 

Black and Scholes considered a world in which there are three assets: a stock, whose price, $\tilde { S } _ { t }$ , follows the stochastic differential equation: 

$$
d \tilde {S} _ {t} = \mu \tilde {S} _ {t} d t + \sigma \tilde {S} _ {t} d \tilde {z} _ {t},
$$

where $\left\{ \tilde { z } _ { t } \right\} _ { t = 0 } ^ { T }$ is a Brownian motion process; a bond, whose price, $B _ { t }$ , follows the differential equation: 

$$
d B _ {t} = r B _ {t} d t;
$$

and a call option on the stock with strike price X and maturity date $T$ . 

They showed how to construct an instantaneously riskless portfolio of stocks and options, and hence, assuming that the principle of no arbitrage holds, derived the Black-Scholes partial differential equation which must be satisfied by the option price. 

The option pays $( S _ { T } - X ) ^ { + } \equiv \operatorname* { m a x } { \{ S _ { T } - X , 0 \} }$ at maturity. 

Let the price of the call at time t be $\tilde { C } _ { t }$ . Guess that $\tilde { C } _ { t } = C ( \tilde { S } _ { t } , t )$ . By Ito’s lemma: 

$$
d \tilde {C} _ {t} = \left(\frac {\partial C}{\partial t} + \frac {\partial C}{\partial S} \mu \tilde {S} _ {t} + \frac {1}{2} \frac {\partial^ {2} C}{\partial S ^ {2}} \sigma^ {2} \tilde {S} _ {t} ^ {2}\right) d t + \frac {\partial C}{\partial S} \sigma \tilde {S} _ {t} d \tilde {z} _ {t}
$$

The no arbitrage principle yields the partial differential equation: 

$$
\frac {\partial C}{\partial t} + \frac {1}{2} \frac {\partial^ {2} C}{\partial S ^ {2}} \sigma^ {2} S ^ {2} + \frac {\partial C}{\partial S} r S - r C = 0
$$

subject to the boundary condition 

$$
C (S, T) = (S - X) ^ {+}.
$$

Let $\tau = T - t$ be the time to maturity. 

Then we claim that the solution to the Black-Scholes equation is: 

$$
C (S, t) = S N \left(d (S, \tau)\right) - X e ^ {- r \tau} N \left(d (S, \tau) - \sigma \sqrt {\tau}\right),
$$

where $N \left( \cdot \right)$ is the cumulative distribution function of the standard normal distribution and 

$$
d (S, \tau) = \frac {\ln \frac {S}{X} + (r - \frac {1}{2} \sigma^ {2}) \tau}{\sigma \sqrt {\tau}} + \sigma \sqrt {\tau}\tag{7.2.1}
$$

$$
= \frac {\ln \frac {S}{X} + \left(r + \frac {1}{2} \sigma^ {2}\right) \tau}{\sigma \sqrt {\tau}}.\tag{7.2.2}
$$

We can check that this is indeed the solution by calculating the various partial derivatives and substituting them in the original equation. 

Note first that 

$$
N (z) \equiv \int_ {- \infty} ^ {z} \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} t ^ {2}} d t
$$

and hence by the fundamental theorem of calculus 

$$
N ^ {\prime} (z) \equiv \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} z ^ {2}},
$$

Revised: December 2, 1998 

which of course is the corresponding probability density function. For the last step in this proof, we will need the partials of $d \left( S , \tau \right)$ with respect to S and t, which are: 

$$
\frac {\partial d (S , \tau)}{\partial t} = - \frac {\partial d (S , \tau)}{\partial \tau} = - \frac {(r + \frac {1}{2} \sigma^ {2})}{2 \sigma \sqrt {\tau}}\tag{7.2.3}
$$

and 

$$
\frac {\partial d (S , \tau)}{\partial S} = \frac {1}{S \sigma \sqrt {\tau}}.\tag{7.2.4}
$$

Note also that 

$$
N ^ {\prime} \left(d (S, \tau) - \sigma \sqrt {\tau}\right) = e ^ {- \frac {1}{2} \sigma^ {2} \tau} e ^ {d (S, \tau) \sigma \sqrt {\tau}} N ^ {\prime} (d (S, \tau))\tag{7.2.5}
$$

$$
= e ^ {- \frac {1}{2} \sigma^ {2} \tau} \left(\frac {S}{X} e ^ {\left(r + \frac {1}{2} \sigma^ {2}\right) \tau}\right) N ^ {\prime} (d (S, \tau))\tag{7.2.6}
$$

$$
= \frac {S}{X} e ^ {r \tau} N ^ {\prime} (d (S, \tau)).\tag{7.2.7}
$$

Using these facts and the chain rule, we have: 

$$
\begin{array}{r l} \frac {\partial C}{\partial t} & = S N ^ {\prime} (d (S, \tau)) \frac {\partial d (S , \tau)}{\partial t} - X e ^ {- r \tau} \times \\ & \left(N ^ {\prime} (d (S, \tau) - \sigma \sqrt {\tau}) \left(\frac {\partial d (S , \tau)}{\partial t} - \frac {\sigma}{2 \sqrt {\tau}}\right) + r N (d (S, \tau) - \sigma \sqrt {\tau})\right) \end{array}
$$

$$
= - S N ^ {\prime} (d (S, \tau)) \frac {\sigma}{2 \sqrt {\tau}} - X e ^ {- r \tau} r N (d (S, \tau) - \sigma \sqrt {\tau})\tag{7.2.8}
$$

(7.2.9) 

$$
\begin{array}{r l} \frac {\partial C}{\partial S} & = S N ^ {\prime} (d (S, \tau)) \frac {\partial d (S , \tau)}{\partial S} + N (d (S, \tau)) \\ & - X e ^ {- r \tau} N ^ {\prime} (d (S, \tau) - \sigma \sqrt {\tau}) \frac {\partial d (S , \tau)}{\partial S} \end{array}\tag{7.2.10}
$$

$$
\begin{array}{r l} {=} & {N \left(d \left(S, \tau\right)\right)} \\ {\frac {\partial^ {2} C}{\partial S ^ {2}}} \\ {=} & {N ^ {\prime} \left(d \left(S, \tau\right)\right) \frac {\partial d \left(S , \tau\right)}{\partial S}.} \end{array}\tag{7.2.11}
$$

(7.2.12) 

Substituting these expressions in the original partial differential equation yields: 

$$
\frac {\partial C}{\partial t} + \frac {1}{2} \frac {\partial^ {2} C}{\partial S ^ {2}} \sigma^ {2} S ^ {2} + \frac {\partial C}{\partial S} r S - r C
$$

$$
\begin{array}{r l} = & N (d (S, \tau)) (r S - r S) + N ^ {\prime} (d (S, \tau)) \left(\frac {- S \sigma}{2 \sqrt {\tau}} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial d (S , \tau)}{\partial S}\right) \\ & + N (d (S, \tau) - \sigma \sqrt {\tau}) (- X e ^ {- r \tau} r + r X e ^ {- r \tau}) \\ = & 0. \end{array} \tag {7.2}\tag{7.2.13}
$$

(7.2.14) 

The boundary condition should also be checked. $\mathrm { A s } ~ \tau \to ~ 0 , ~ d ( S , \tau ) \to \pm \infty$ according as $S > X \mathrm { o r } S < X$ . In the former case, $C \left( S , T \right) = S - X$ ; and in the latter case, $C \left( S , T \right) = 0$ , so the boundary condition is indeed satisfied. 

## 7.3 Multi-period Investment Problems

In Section 4.2, it was pointed out that the objects of choice can be differentiated not only by their physical characteristics, but also both by the time at which they are consumed and by the state of nature in which they are consumed. These distinctions were suppressed in the intervening sections but are considered again in this section and in Section 5.4 respectively. 

The multi-period model should probably be introduced at the end of Chapter 4 but could also be left until Chapter 7. For the moment this brief introduction is duplicated in both chapters. 

Discrete time multi-period investment problems serve as a stepping stone from the single period case to the continuous time case. 

The main point to be gotten across is the derivation of interest rates from equilibrium prices: spot rates, forward rates, term structure, etc. 

This is covered in one of the problems, which illustrates the link between prices and interest rates in a multiperiod model. 

## 7.4 Continuous Time Investment Problems