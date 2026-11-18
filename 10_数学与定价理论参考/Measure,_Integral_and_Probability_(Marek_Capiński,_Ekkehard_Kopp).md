

<!-- === Source: MinerU_markdown_Measure,_Integral_and_Probability_(Marek_Capiński,_Ekkehard_Kopp)_1_2122706850364366854.md (Page 1) === -->

Measure, Integral and Probability 

Second Edition $P ( A \mid B ) = { \frac { P ( A \cap B ) } { P ( B ) } }$ Springer 

# Measure, Integral and Probability

To our children; grandchildren: Piotr, Maciej, Jan, Anna; Luk asz Anna, Emily 

The central concepts in this book are Lebesgue measure and the Lebesgue integral. Their role as standard fare in UK undergraduate mathematics courses is not wholly secure; yet they provide the principal model for the development of the abstract measure spaces which underpin modern probability theory, while the Lebesgue function spaces remain the main source of examples on which to test the methods of functional analysis and its many applications, such as Fourier analysis and the theory of partial diferential equations. 

It follows that not only budding analysts have need of a clear understanding of the construction and properties of measures and integrals, but also that those who wish to contribute seriously to the applications of analytical methods in a wide variety of areas of mathematics, physics, electronics, engineering and, most recently, finance, need to study the underlying theory with some care. 

We have found remarkably few texts in the current literature which aim explicitly to provide for these needs, at a level accessible to current undergraduates. There are many good books on modern probability theory, and increasingly they recognize the need for a strong grounding in the tools we develop in this book, but all too often the treatment is either too advanced for an undergraduate audience or else somewhat perfunctory. We hope therefore that the current text will not be regarded as one which fills a much-needed gap in the literature! 

One fundamental decision in developing a treatment of integration is whether to begin with measures or integrals, i.e. whether to start with sets or with functions. Functional analysts have tended to favour the latter approach, while the former is clearly necessary for the development of probability. We have decided to side with the probabilists in this argument, and to use the (reasonably) systematic development of basic concepts and results in probability theory as the principal field of application – the order of topics and the terminology we use reflect this choice, and each chapter concludes with further development of the relevant probabilistic concepts. At times this approach may seem less ‘eficient’ than the alternative, but we have opted for direct proofs and explicit constructions, sometimes at the cost of elegance. We hope that it will increase understanding. 

The treatment of measure and integration is as self-contained as we could make it within the space and time constraints: some sections may seem too pedestrian for final-year undergraduates, but experience in testing much of the material over a number of years at Hull University teaches us that familiarity and confidence with basic concepts in analysis can frequently seem somewhat shaky among these audiences. Hence the preliminaries include a review of Riemann integration, as well as a reminder of some fundamental concepts of elementary real analysis. 

While probability theory is chosen here as the principal area of application of measure and integral, this is not a text on elementary probability, of which many can be found in the literature. 

Though this is not an advanced text, it is intended to be studied (not skimmed lightly) and it has been designed to be useful for directed self-study as well as for a lecture course. Thus a significant proportion of results, labelled ‘Proposition’, are not proved immediately, but left for the reader to attempt before proceeding further (often with a hint on how to begin), and there is a generous helping of Exercises. To aid self-study, proofs of the Propositions are given at the end of each chapter, and outline solutions of the Exercises are given at the end of the book. Thus few mysteries should remain for the diligent. 

After an introductory chapter, motivating and preparing for the principal definitions of measure and integral, Chapter 2 provides a detailed construction of Lebesgue measure and its properties, and proceeds to abstract the axioms appropriate for probability spaces. This sets a pattern for the remaining chapters, where the concept of independence is pursued in ever more general contexts, as a distinguishing feature of probability theory. 

Chapter 3 develops the integral for non-negative measurable functions, and introduces random variables and their induced probability distributions, while Chapter 4 develops the main limit theorems for the Lebesgue integral and com pares this with Riemann integration. The applications in probability lead to a discussion of expectations, with a focus on densities and the role of characteristic functions. 

In Chapter 5 the motivation is more functional-analytic: the focus is on the Lebesgue function spaces, including a discussion of the special role of the space $L ^ { 2 }$ of square-integrable functions. Chapter 6 sees a return to measure theory, with the detailed development of product measure and Fubini’s theorem, now leading to the role of joint distributions and conditioning in probability. Finally, following a discussion of the principal modes of convergence for sequences of integrable functions, Chapter 7 adopts an unashamedly probabilistic bias, with a treatment of the principal limit theorems, culminating in the Lindeberg–Feller version of the Central Limit Theorem. 

The treatment is by no means exhaustive, as this is a textbook, not a treatise. Nonetheless the range of topics is probably slightly too extensive for a one-semester course at third-year level: the first five chapters might provide a useful course for such students, with the last two left for self-study or as part of a reading course for students wishing to continue in probability theory. Alternatively, students with a stronger preparation in analysis might use the first two chapters as background material and complete the remainder of the book in a one-semester course. 

May 1998 

Marek Capinski´ Ekkehard Kopp 

# Preface to the Second Edition

After five years and six printings it seems only fair to our readers that we should respond to their comments and also correct errors and imperfections to which we have been alerted in addition to those we have discovered ourselves in reviewing the text. This second edition also introduces additional material which earlier constraints of time and space had precluded, and which has, in our view, become more essential as the make-up of our potential readership has become clearer. We hope that we manage to do this in a spirit which preserves the essential features of the text, namely providing the material rigorously and in a form suitable for directed self-study. Thus the focus remains on accessibility, explicitness and emphasis on concrete examples, in a style that seeks to encourage readers to become directly involved with the material and challenges them to prove many of the results themselves (knowing that solutions are also given in the text!). 

Apart from further examples and exercises, the new material presented here is of two contrasting kinds. The new Chapter 7 adds a discussion of the comparison of general measures, with the Radon-Nikodym Theorem as its focus. The proof given here, while not new, is in our view more constructive and elementary than the usual ones, and we utilise the result consistently to examine the structure of Lebesgue-Stieltjes measures on the line and to deduce the Hahn-Jordan decomposition of signed measures. The common origin of the concepts of variation and absolute continuity of functions and measures is clarified. The main probabilistic application is to conditional expectations, for which an alternative construction via orthogonal projections is also provided in Chapter 5. This is applied in turn in Chapter 7 to derive elementary properties of martingales in discrete time. 

The other addition occurs at the end of each chapter (with the exception of Chapters 1 and 5). Since it is clear that a significant proportion of our current readership is amongst students of the burgeoning field of mathematical finance, each relevant chapter ends with a brief discussion of ideas from that subject. In these sections we depart from our aim of keeping the book self-contained, since we can hardly develop this whole discipline afresh. Thus we neither define nor explain the origin of the finance concepts we address, but instead seek to locate them mathematically within the conceptual framework of measure and probability. This leads to conclusions with a mathematical precision that sometimes eludes authors writing from a finance perspective. 

To avoid misunderstanding we repeat that the purpose of this book remains the development of the ideas of measure and integral, especially with a view to their applications in probability and (briefly) in finance. This is therefore neither a textbook in probability theory nor in mathematical finance. Both of these disciplines have a large specialist literature of their own, and our comments on these areas of application are intended to assist the student in understanding the mathematical framework which underpins them. 

We are grateful to those of our readers and to colleagues who have pointed out many of the errors, both typographical and conceptual, of the first edition. The errors that inevitably remain are our sole responsibility. To facilitate their speedy correction a webpage has been created for the notification of errors, inaccuracies and queries, at http://www.springer.co.uk/MIP and we encourage our readers to use it mercilessly. Our thanks also go to Stephanie Harding and Karen Borthwick at Springer Verlag, London, for their continuing care and helpfulness in producing this edition. 

October 2003 

Marek Capinski´ Ekkehard Kopp 

1. Motivation and preliminaries ..... 1
1.1 Notation and basic set theory ..... 2
1.1.1 Sets and functions ..... 2
1.1.2 Countable and uncountable sets in $\mathbb{R}$ ..... 4
1.1.3 Topological properties of sets in $\mathbb{R}$ ..... 5
1.2 The Riemann integral: scope and limitations ..... 7
1.3 Choosing numbers at random ..... 12

2. Measure ..... 15
2.1 Null sets ..... 15
2.2 Outer measure ..... 20
2.3 Lebesgue measurable sets and Lebesgue measure ..... 26
2.4 Basic properties of Lebesgue measure ..... 35
2.5 Borel sets ..... 40
2.6 Probability ..... 45
2.6.1 Probability space ..... 46
2.6.2 Events: conditioning and independence ..... 46
2.6.3 Applications to mathematical finance ..... 49
2.7 Proofs of propositions ..... 51

3. Measurable functions ..... 55
3.1 The extended real line ..... 55
3.2 Lebesgue-measurable functions ..... 55
3.3 Examples ..... 59
3.4 Properties ..... 60
3.5 Probability ..... 66 

3.5.1 Random variables 66  
3.5.2 Sigma fields generated by random variables 67  
3.5.3 Probability distributions 68  
3.5.4 Independence of random variables 70  
3.5.5 Applications to mathematical finance 71  
3.6 Proofs of propositions 73  

4. Integral 75  
4.1 Definition of the integral 75  
4.2 Monotone Convergence Theorems 82  
4.3 Integrable functions 86  
4.4 The Dominated Convergence Theorem 92  
4.5 Relation to the Riemann integral 97  
4.6 Approximation of measurable functions 102  
4.7 Probability 105  
4.7.1 Integration with respect to probability distributions 105  
4.7.2 Absolutely continuous measures: examples of densities 106  
4.7.3 Expectation of a random variable 114  
4.7.4 Characteristic function 115  
4.7.5 Applications to mathematical finance 117  
4.8 Proofs of propositions 119  

5. Spaces of integrable functions 125  
5.1 The space $L^1$ 126  
5.2 The Hilbert space $L^2$ 131  
5.2.1 Properties of the $L^2$ -norm 132  
5.2.2 Inner product spaces 135  
5.2.3 Orthogonality and projections 137  
5.3 The $L^p$ spaces: completeness 140  
5.4 Probability 146  
5.4.1 Moments 146  
5.4.2 Independence 150  
5.4.3 Conditional Expectation (first construction) 153  
5.5 Proofs of propositions 155  

6. Product measures 159  
6.1 Multi-dimensional Lebesgue measure 159  
6.2 Product σ-fields 160  
6.3 Construction of the product measure 162  
6.4 Fubini's Theorem 169  
6.5 Probability 173  
6.5.1 Joint distributions 173 

6.5.2 Independence again....175
6.5.3 Conditional probability....178
6.5.4 Characteristic functions determine distributions....180
6.5.5 Application to mathematical finance....182
6.6 Proofs of propositions....185

7. The Radon–Nikodym Theorem....187
7.1 Densities and Conditioning....187
7.2 The Radon–Nikodym Theorem....188
7.3 Lebesgue–Stieltjes measures....198
7.3.1 Construction of Lebesgue–Stieltjes measures....199
7.3.2 Absolute continuity of functions....204
7.3.3 Functions of bounded variation....206
7.3.4 Signed measures....210
7.4 Probability....218
7.4.1 Conditional expectation relative to a σ-field....218
7.4.2 Martingales....221
7.4.3 Applications to mathematical finance....231
7.5 Proofs of propositions....234

8. Limit theorems....241
8.1 Modes of convergence....241
8.2 Probability....243
8.2.1 Convergence in probability....245
8.2.2 Weak law of large numbers....249
8.2.3 The Borel–Cantelli Lemmas....255
8.2.4 Strong law of large numbers....260
8.2.5 Weak convergence....268
8.2.6 Central Limit Theorem....273
8.2.7 Applications to mathematical finance....280
8.3 Proofs of propositions....283

9. Solutions to exercises....287
10. Appendix....301
References....305
Bibliography....305
Index....307 

# Motivation and preliminaries

Life is an uncertain business. We can seldom be sure that our plans will work out as we intend, and are thus conditioned from an early age to think in terms of the likelihood that certain events will occur, and which are ‘more likely’ than others. Turning this vague description into a probability modelamounts to the construction of a rational framework for thinking about uncertainty. The framework ought to be a general one, which enables us equally to handle situations where we have to sift a great deal of prior information, and those where we have little to go on. Some degree of judgement is needed in all cases; but we seek an orderly theoretical framework and methodology which enables us to formulate general laws in quantitative terms. 

This leads us to mathematical models for probability, that is to say, idealized abstractions of empirical practice, which nonetheless have to satisfy the criteria of wide applicability, accuracy and simplicity. In this book our concern will be with the construction and use of generally applicable probability models in which we can also consider infinite sample spaces and infinite sequences of trials: that such are needed is easily seen when one tries to make sense of apparently simple concepts such as ‘drawing a number at random from the interval [0, 1]’ and in trying to understand the limit behaviour of a sequence of identical trials. Just as elementary probabilities are computed by finding the comparative sizes of sets of outcomes, we will find that the fundamental problem to be solved is that of measuring the ‘size’ of a set with infinitely many elements. At least for sets on the real line, the ideas of basic real analysis provide us with a convincing answer, and this contains all the ideas needed for the abstract axiomatic framework on which to base the theory of probability. For this reason the development of the concept of measure, and Lebesgue measureon R in particular, has pride of place in this book. 

## 1.1 Notation and basic set theory

In measure theory we deal typically with families of subsets of some arbitrary given set and consider functions which assign real numbers to sets belonging to these families. Thus we need to review some basic set notation and operations on sets, as well as discussing the distinction between countably and uncountably infinite sets, with particular reference to subsets of the real line R. We shall also need notions from analysis such as limits of sequences, series, and open sets. Readers are assumed to be largely familiar with this material and may thus skip lightly over this section, which is included to introduce notation and make the text reasonably self-contained and hence useful for self-study. The discussion remains quite informal, without reference to foundational issues, and the reader is referred to basic texts on analysis for most of the proofs. Here we mention just two recent introductory textbooks: [8] and [11]. 

## 1.1.1 Sets and functions

In our operations with sets we shall always deal with collections of subsets of some universal set $\varOmega ;$ the nature of this set will be clear from the context – frequently $\varOmega$ will be the set R of real numbers or a subset of it. We leave the concept of ‘set’ as undefined and given, and concern ourselves only with set membership and operations. The empty set is denoted by $\mathrm { O } ;$ it has no members. Sets are generally denoted by capital letters. 

Set membership is denoted by $\in , \ { \mathrm { s o } } \ x \in A$ means that the element x is a member of the set A. Set inclusion, $A \subset B$ , means that every member of A is a member of B. This includes the case when A and B are equal; if the inclusion is strict, i.e. $A \subset B$ and B contains elements which are not in A (written $x \not \in A )$ this will be stated separately. The notation $\{ x \in A : P ( x ) \}$ is used to denote the set of elements of A with property P. The set of all subsets of A (its power set) is denoted by ${ \mathcal { P } } ( A )$ 

We define the intersection $A \cap B = \{ x : x \in A$ and $x \in B \}$ and union $A \cup B = \{ x : x \in A { \mathrm { ~ o r ~ } } x \in B \}$ . The complement $A ^ { \mathrm { c } }$ of A consists of the elements of $\varOmega$ which are not members of A; we also write $A ^ { \mathrm { c } } = \varOmega \setminus A$ , and, more generally, we have the diference $B \setminus A = \{ x \in B : x \notin A \} = B \cap A ^ { \mathrm { c } }$ and the symmetric diference $A A B = ( A \setminus B ) \cup ( B \setminus A )$ . Note that $A \varDelta B = 0$ if 

and only if $A = B$ 

Intersection (resp. union) gives expression to the logical connective ‘and’ $\left( \mathrm { r e s p . ~ } ^ { \cdot } \mathrm { o r } ^ { \cdot } \right)$ and, via the logical symbols  (there exists) and  (for all), they have extensions to arbitrary collections; indexed by some set Λ these are given by 

$$
\bigcap_ {\alpha \in \Lambda} A _ {\alpha} = \{x: x \in A _ {\alpha} \text {   for   all   } \alpha \in \Lambda \} = \{x: \forall \alpha \in \Lambda ,   x \in A _ {\alpha} \}
$$

$$
\bigcup_ {\alpha \in \Lambda} A _ {\alpha} = \{x: x \in A _ {\alpha} \text {   for   some   } \alpha \in \Lambda \} = \{x: \exists \alpha \in \Lambda ,   x \in A _ {\alpha} \}.
$$

These are linked by de Morgan’s laws: 

$$
(\bigcup_ {\alpha} A _ {\alpha}) ^ {c} = \bigcap_ {\alpha} A _ {\alpha} ^ {c}; \qquad (\bigcap_ {\alpha} A _ {\alpha}) ^ {c} = \bigcup_ {\alpha} A _ {\alpha} ^ {c}.
$$

If $A \cap B = \emptyset$ then A and B are disjoint. A family of sets $( A _ { \alpha } ) _ { \alpha \in \Lambda }$ is pairwise disjoint if $A _ { \alpha } \cap A _ { \beta } = \emptyset$ whenever α $\neq \beta \ ( \alpha , \beta \in A )$ 

The Cartesian product $A \times B$ of sets A and B is the set of ordered pairs $A \times B = \{ ( a , b ) : a \in A , b \in B \}$ . As already indicated, we use $\mathbb { N , Z , Q }$ , R for the basic number systems of natural numbers, integers, rationals and reals respectively. Intervals in R are denoted via each endpoint, with a square bracket indicating its inclusion, an open bracket exclusion, e.g. $[ a , b ) = \{ x \in \mathbb { R } : a \leq$ $x < b \}$ . We use and $- \infty$ to describe unbounded intervals, $\mathrm { e . g . ~ } ( - \infty , b ) =$ $\{ x \in \mathbb { R } : x < b \} , [ 0 , \infty ) = \{ x \in \mathbb { R } : x \geq 0 \} = \mathbb { R } ^ { + } . \mathbb { R } ^ { 2 } = \mathbb { R } \times \mathbb { R }$ denotes the plane, more generally, $\mathbb { R } ^ { n }$ is the $n { \mathrm { - f o l d } }$ Cartesian product of R with itself, i.e. the set of all n-tuples $( x _ { 1 } , \ldots , x _ { n } )$ composed of real numbers. Products of intervals, called rectangles, are denoted similarly. 

Formally, a function $f : A  B$ is a subset of $A \times B$ in which each first coordinate determines the second: if $( a , b ) , ( a , c ) \in f$ then $b = c .$ . Its domain ${ \mathcal { D } } _ { f } = \{ a \in A : \exists b \in B , ( a , b ) \in f \}$ , and range ${ \mathcal { R } } _ { f } = \left\{ b \in B : \exists a \in A , ( a , b ) \in f \right\}$ describe its scope. Informally, f associates elements of B with those of A, such that each $a \in A$ has at most one image $b \in B$ . We write this as $b = f ( a )$ The set $X \subset A$ has image $f ( X ) = \{ b \in B : b = f ( a )$ for some $a \in X \}$ and the inverse image of a set $Y \subset B$ is $f ^ { - 1 } ( Y ) = \{ a \in A : f ( a ) \in Y \}$ . The composition $f _ { 2 } \circ f _ { 1 }$ of $f _ { 1 } : A \to B$ and $f _ { 2 } : B \to C$ is the function $h : A  C$ defined by $h ( a ) = f _ { 2 } ( f _ { 1 } ( a ) )$ . When $A = B = C , x \mapsto ( f _ { 1 } \circ f _ { 2 } ) ( x ) = f _ { 1 } ( f _ { 2 } ( x ) )$ and $x \mapsto ( f _ { 2 } \circ f _ { 1 } ) ( x ) = f _ { 2 } ( f _ { 1 } ( x ) )$ both define functions from A to A. In general, these will not be the same: for example, let $f _ { 1 } ( x ) = \sin x , f _ { 2 } ( x ) = x ^ { 2 }$ , then $x \mapsto \sin ( x ^ { 2 } )$ and $x \mapsto ( \sin x ) ^ { 2 }$ are not equal. 

The function g extends f if $\mathcal { D } _ { f } \subset \mathcal { D } _ { g }$ and $g = f$ on $\mathcal { D } _ { f } \colon$ ; alternatively we say that f restricts g to $\mathcal { D } _ { f }$ . These concepts will be used frequently for real-valued set functions, where the domains are collections of sets and the range is a subset of R. 

The algebra of real functions is defined pointwise, i.e. the sum $f + g$ and product $f \cdot g$ are given by $( f + g ) ( x ) = f ( x ) + g ( x ) , ( f \cdot g ) ( x ) = f ( x ) \cdot g ( x )$ 

The indicator function $\mathbf { 1 } _ { A }$ of the set A is the function 

$$
\mathbf {1} _ {A} (x) = \left\{ \begin{array}{l l} 1 & \text { for } x \in A \\ 0 & \text { for } x \notin A. \end{array} \right.
$$

Note that $\mathbf { 1 } _ { A \cap B } = \mathbf { 1 } _ { A } \cdot \mathbf { 1 } _ { B } , \ \mathbf { 1 } _ { A \cup B } = \mathbf { 1 } _ { A } + \mathbf { 1 } _ { B } - \mathbf { 1 } _ { A } \mathbf { 1 } _ { B } , \mathrm { a n d } \ \mathbf { 1 } _ { A ^ { c } } = 1 - \mathbf { 1 } _ { A }$ 

We need one more concept from basic set theory, which should be familiar: For any set $E _ { : }$ an equivalence relation on E is a relation (i.e. a subset R of $E \times E$ , where we write $x \sim y$ to indicate that $( x , y ) \in R )$ with the following properties: 

1. reflexive: for all $x \in E , x \sim x$ 2 

2. symmetric: $x \sim y$ implies $y \sim x ,$ 

3. transitive: $x \sim y$ and $y \sim z$ implies $x \sim z$ 

An equivalence relation on E partitions E into disjoint equivalence classes: given $x \in E$ , write $[ x ] = \{ z : z \sim x \}$ for the equivalence class of x, i.e. the set of all elements of E that are equivalent to x. Thus $x \in [ x ]$ , hence $\textstyle E = \bigcup _ { x \in E } [ x ]$ . This is a disjoint union: if $[ x ] \cap [ y ] \neq \emptyset$ , then there is $z \in E$ with $x \sim z$ Sand $z \sim y$ , hence $x \sim y .$ , so that $[ x ] = [ y ]$ . We shall denote the set of all equivalence classes so obtained by $E / \sim$ 

## 1.1.2 Countable and uncountable sets in R

We say that a set A is countable if there is a one–one correspondence between A and a subset of N, i.e. a function $f : A  \mathbb { N }$ that takes distinct points to distinct points. Informally, A is finite if this correspondence can be set up using only an initial segment $\{ 1 , 2 , . . . , N \}$ of N (for some $N \in \mathbb { N } )$ , while we call A countably infinite or denumerable if all of N is used. It is not dificult to see that countable unions of countable sets are countable; in particular, the set Q of rationals is countable. 

Cantor showed that the set R cannot be placed in one–one correspondence with (a subset of) N; thus it is an example of an uncountable set. Cantor’s proof assumes that we can write each real number uniquely as a decimal (always choosing the non-terminating version). We can also restrict ourselves (why?) to showing that the interval [0,1] is uncountable. 

If this set were countable, then we could write its elements as a sequence $( x _ { n } ) _ { n \geq 1 }$ , and since each $x _ { n }$ has a unique decimal expansion of the form 

$$
x _ {n} = 0. a _ {n 1} a _ {n 2} a _ {n 3} \dots . a _ {n n} \dots
$$

for digits $a _ { i j }$ chosen from the set $\{ 0 , 1 , 2 . . . , 9 \}$ , we could therefore write down the array 

$$
x _ {1} = 0. a _ {1 1} a _ {1 2} a _ {1 3} \ldots
$$

$$
x _ {2} = 0. a _ {2 1} a _ {2 2} a _ {2 3} \dots
$$

$$
x _ {3} = 0. a _ {3 1} a _ {3 2} a _ {3 3} \dots
$$

Now write down $y = 0 . b _ { 1 } b _ { 2 } b _ { 3 } \ldots$ , where the digits $b _ { n }$ are chosen to difer from $a _ { n n }$ . Such a decimal expansion defines a number $y \in [ 0 , 1 ]$ that difers from each of the $x _ { n }$ (since its expansion difers from that of $x _ { n }$ in the nth place). Hence our sequence does not exhaust [0,1], and the contradiction shows that [0,1] cannot be countable. 

Since the union of two countable sets must be countable, and since $\mathbb { Q }$ is countable, it follows that $\mathbb { R } \backslash \mathbb { Q }$ is uncountable, i.e. there are far ‘more’ irrationals than rationals! One way of making this seem more digestible is to consider the problem of choosing numbers at random from an interval in R. 

Recall that rational numbers are precisely those real numbers whose decimal expansion recurs (we include ‘terminates’ under ‘recurs’). Now imagine choosing a real number from [0,1] at random: think of the set R as a pond containing all real numbers, and imagine you are ‘fishing’ in this pond, pulling out one number at a time. 

How likely is it that the first number will be rational, i.e. how likely are we to find a number whose expansion recurs? It would be like rolling a ten-sided die infinitely many times and expecting, after a finite number of throws, to say with certainty that all subsequent throws will give the same digit. This does not seem at all likely, and we should therefore not be too surprised to find that countable sets (including Q) will be among those we can ‘neglect’ when measuring sets on the real line in the ‘unbiased’ or uniform way in which we have used the term ‘random’ so far. Possibly more surprising, however, will be the discovery that even some uncountable sets can be ‘negligible’ from the point of view adopted here. 

## 1.1.3 Topological properties of sets in R

Recall the definition of an open set $O \subset \mathbb { R }$ 

## Definition 1.1

A subset O of the real line R is open if it is a union of open intervals, i.e. for intervals $( I _ { \alpha } ) _ { \alpha \in \Lambda }$ , where Λ is some index set (countable or not) 

$$
O = \bigcup_ {\alpha \in \Lambda} I _ {\alpha}.
$$

A set is closed if its complement is open. Open sets in $\mathbb { R } ^ { n } { \bf \Pi } ( n > 1 )$ can be defined as unions of n-fold products of intervals. 

This definition seems more general than it actually is, since, on R, countable unions will always sufice – though the freedom to work with general unions will be convenient later on. If Λ is an index set and $I _ { \alpha }$ is an open interval for each $\alpha \in { \cal { A } }$ , then there exists a countable collection $\left( I _ { \alpha _ { k } } \right) _ { k \geq 1 }$ of these intervals whose union equals $\cup _ { \alpha \in A } I _ { \alpha }$ . What is more, the sequence of intervals can be chosen to be pairwise disjoint. 

It is easy to see that a finite intersection of open sets is open; however, a countable intersection of open sets need not be open: let $O _ { n } = \left( - { \frac { 1 } { n } } , 1 \right)$ for $n \geq 1$ , then $E = \cap _ { n = 1 } ^ { \infty } O _ { n } = [ 0 , 1 )$ is not open. 

Note that R, unlike R<sup>n</sup> or more general spaces, has a linear order, i.e. given $x , y \in \mathbb { R }$ we can decide whether $x \leq y$ or $y \leq x .$ . Thus u is an upper bound for a set $A \subset \mathbb { R }$ if $a \leq u$ for all $a \in A$ , and a lower bound is defined similarly. The supremum (or least upper bound) is then the minimum of all upper bounds and written sup A. The infimum (or greatest lower bound) inf A is defined as the maximum of all lower bounds. The completeness property of R can be expressed by the statement that every set which is bounded above has a supremum. 

A real function f is said to be continuous if $f ^ { - 1 } ( O )$ is open for each open set O. Every continuous real function defined on a closed bounded set attains its bounds on such a set, i.e. has a minimum and maximum value there. For example, if $f : [ a , b ] \to \mathbb { R }$ is continuous, $M = \operatorname* { s u p } \{ f ( x ) : x \in [ a , b ] \} = f ( x _ { \operatorname* { m a x } } )$ 2 $m = \operatorname* { i n f } \{ f ( x ) : x \in [ a , b ] \} = f ( x _ { \operatorname* { m i n } } )$ for some points $x _ { \mathrm { m a x } } , x _ { \mathrm { m i n } } \ \in \ [ a , b ]$ The Intermediate Value Theorem says that a continuous function takes all intermediate values between the extreme ones, i.e. for each $y \in [ m , M ]$ there is a $\theta \in [ a , b ]$ such that $y = f ( \theta )$ 

Specializing to real sequences $( x _ { n } )$ , we can further define the upper limit lim $\operatorname { s u p } _ { n } x _ { n }$ as 

$$
\inf \{\sup _ {m \geq n} x _ {m}: n \in \mathbb {N} \}
$$

and the lower limit lim in $\mathrm { f } _ { n } x _ { n }$ as 

$$
\sup \bigl \{\inf _ {m \geq n} x _ {m}: n \in \mathbb {N} \bigr \}.
$$

The sequence $x _ { n }$ convergesif and only if these quantities coincide and their common value is then its limit. Recall that a sequence $( x _ { n } )$ converges and the real number x is its limit, written $x = \operatorname* { l i m } _ { x \to \infty } x _ { n }$ , if for every $\varepsilon > 0$ there is an $N \in \mathbb N$ such that $| x _ { n } - x | < \varepsilon$ whenever $n \geq N$ . A series $\textstyle \sum _ { n \geq 1 } a _ { n }$ converges if the sequence $\textstyle x _ { m } = \sum _ { n = 1 } ^ { m } a _ { n }$ Pof its partial sums converges, and its limit is then the sum $\textstyle \sum _ { n = 1 } ^ { \infty } a _ { n }$ Pof the series. 

## 1.2 The Riemann integral: scope and limitations

In this section we give a brief review of the Riemann integral, which forms part of the staple diet in introductory analysis courses, and consider some of the reasons why it does not sufice for more advanced applications. 

Let $f : [ a , b ] \to \mathbb { R }$ be a bounded real function, where $a , b ,$ , with $a < b .$ , are real numbers. A partition of $[ a , b ]$ is a finite set $P = \left\{ a _ { 0 } , a _ { 1 } , a _ { 2 } , . . . , a _ { n } \right\}$ with 

$$
a = a _ {0} <   a _ {1} <   a _ {2} <   \dots <   a _ {n} = b.
$$

The partition P gives rise to the upper and lower Riemann sums 

$$
U (P, f) = \sum_ {i = 1} ^ {n} M _ {i} \Delta a _ {i}, \quad L (P, f) = \sum_ {i = 1} ^ {n} m _ {i} \Delta a _ {i}
$$

where $\varDelta a _ { i } = a _ { i } - a _ { i - 1 }$ 

$$
M _ {i} = \sup _ {a _ {i - 1} \leq x \leq a _ {i}} f (x)
$$

and 

$$
m _ {i} = \inf _ {a _ {i - 1} \leq x \leq a _ {i}} f (x)
$$

for each $i \leq n$ . (Note that $M _ { i }$ and $m _ { i }$ are well-defined real numbers since $f$ is bounded on each interval $[ a _ { i - 1 } , a _ { i } ] . )$ 

In order to define the Riemann integral of $f ,$ one first shows that for any given partition P, $L ( P , f ) \leq U ( P , f )$ , and next that for any refinement, i.e. a partition $P ^ { \prime } \supset P$ , we must have $L ( P , f ) \leq L ( P ^ { \prime } , f )$ and $U ( P ^ { \prime } , f ) \leq U ( P , f )$ Finally, since for any two partitions $P _ { 1 }$ and $P _ { 2 }$ , their union $P _ { 1 } \cup P _ { 2 }$ is a refinement of both, we see that $L ( P , f ) \leq U ( Q , f )$ for any partitions $P , Q$ . The set $\{ L ( P , f ) : P$ is a partition of $[ a , b ] \}$ is thus bounded above in R, and we call its supremum the lower integral ${ \underline { { \int _ { a } ^ { b } } } } { \overset { . } { f } }$ of $f$ on $[ a , b ]$ . Similarly, the infimum of the set of upper sums is the upper integral ${ \overline { { \int _ { a } ^ { b } } } } f$ . The function f is now said to be 

Riemann-integrable on $[ a , b ]$ if these two numbers coincide, and their common value is the Riemann integral of $f ,$ denoted by $\textstyle \int _ { a } ^ { b } f$ or, more commonly, 

$$
\int_ {a} ^ {b} f (x) \mathrm{d} x.
$$

This definition does not provide a convenient criterion for checking the integrability of particular functions; however, the following formulation provides a useful criterion for integrability – see [8] for a proof. 

## Theorem 1.1 (Riemann’s Criterion)

$f : [ a , b ] $ R is Riemann-integrable if and only if for every $\varepsilon > 0$ there exists a partition $P _ { \varepsilon }$ such that $U ( P _ { \varepsilon } , f ) - L ( P _ { \varepsilon } , f ) < \varepsilon$ 

## Example 1.1

We calculate $\textstyle \int _ { 0 } ^ { 1 } f ( x )$ dx when $f ( x ) \ = \ { \sqrt { x } } { \mathrm { : } }$ : our immediate problem is that square roots are hard to find except for perfect squares. Therefore we take partition points which are perfect squares, even though this means that the interval lengths of the diferent intervals do not stay the same (there is nothing to say that they should do, even if it often simplifies the calculations). In fact, take the sequence of partitions 

$$
P _ {n} = \{0, (\frac {1}{n}) ^ {2}, (\frac {2}{n}) ^ {2}, \ldots , (\frac {i}{n}) ^ {2}, \ldots , 1 \}
$$

and consider the upper and lower sums, using the fact that f is increasing: 

$$
U (P _ {n}, f) = \sum_ {i = 1} ^ {n} (\frac {i}{n}) \{(\frac {i}{n}) ^ {2} - (\frac {i - 1}{n}) ^ {2} \} = \frac {1}{n ^ {3}} \sum_ {i = 1} ^ {n} (2 i ^ {2} - i)
$$

$$
L (P _ {n}, f) = \sum_ {i = 1} ^ {n} (\frac {i - 1}{n}) \{(\frac {i}{n}) ^ {2} - (\frac {i - 1}{n}) ^ {2} \} = \frac {1}{n ^ {3}} \sum_ {i = 1} ^ {n} (2 i ^ {2} - 3 i + 1).
$$

Hence 

$$
U (P _ {n}, f) - L (P _ {n}, f) = \frac {1}{n ^ {3}} \sum_ {i = 1} ^ {n} (2 i - 1) = \frac {1}{n ^ {3}} \{n (n + 1) - n \} = \frac {1}{n}.
$$

By choosing n large enough, we can make this diference less than any given $\varepsilon > 0$ , hence $f$ is integrable. The integral must be $\textstyle { \frac { 2 } { 3 } }$ , since both $U ( P _ { n } , f )$ and $L ( P _ { n } , f )$ converge to this value, as is easily seen. 

Riemann’s criterion still does not give us a precise picture of the class of Riemann-integrable functions. However, it is easy to show (see [8]) that any bounded monotone function belongs to this class, and only a little more dificult to see that any continuous function $f : [ a , b ] \to \mathbb { R }$ (which is of course automatically bounded) will be Riemann-integrable. 

This provides quite suficient information for many practical purposes, and the tedium of calculations such as that given above can be avoided by proving 

## Theorem 1.2 (Fundamental Theorem of Calculus)

If $f : [ a , b ]  \mathbb { R }$ is continuous and the function $F : [ a , b ] \to \mathbb { R }$ has derivative f $( \mathrm { i . e . ~ } F ^ { \prime } = f \mathrm { ~ o n ~ } ( a , b ) )$ then 

$$
F (b) - F (a) = \int_ {a} ^ {b} f (x) \mathrm{d} x.
$$

This result therefore links the Riemann integral with diferentiation, and displays $F$ as a primitive (also called ‘anti-derivative’) of $f \colon$ 

$$
F (x) = \int_ {- a} ^ {x} f (x) \mathrm{d} x
$$

up to a constant, thus justifying the elementary techniques of integration that form part of any Calculus course. 

We can relax the continuity requirement. A trivial step is to assume $f$ bounded and continuous on $[ a , b ]$ except at finitely many points. Then $f$ is Riemann integrable. To see this split the interval into pieces on which $f$ is continuous. Then $f$ is integrable on each and hence one can derive integrability of $f$ on the whole interval. As an example consider a function $f$ equal to zero for all $x \in [ 0 , 1 ]$ except $a _ { 1 } , \ldots , a _ { n }$ where it equals 1. It is integrable with integral over [0, 1] equal to 0. 

Taking this further, however, will require the power of the Lebesgue theory: in Theorem 4.23 we show that $f$ is Riemann-integrable if and only if it is continuous at ‘almost all’ points of $[ a , b ]$ . This result is by no means trivial, as you will discover if you try to prove directly that the following function $f ,$ due to Dirichlet, is Riemann-integrable over [0, 1]: 

$$
f (x) = \left\{ \begin{array}{l l} \frac {1}{n} & \text { if } x = \frac {m}{n} \in \mathbb {Q} \\ 0 & \text { if } x \notin \mathbb {Q}. \end{array} \right.
$$

In fact, it is not dificult, see [8], to show that $f$ is continuous at each irrational and discontinuous at every rational point, hence (as we will see) is continuous at ‘almost all’ points of [0, 1]. 

Since the purpose of this book is to present Lebesgue’s theory of integration, we should discuss $w h y$ we need a new theory of integration at all: what, if anything, is wrong with the simple Riemann integral described above? 

First, scope: it doesn’t deal with all the kinds of functions that we hope to handle. 

The results that are most easily proved rely on continuous functions on bounded intervals; in order to handle integrals over unbounded intervals, e.g. 

$$
\int_ {- \infty} ^ {\infty} \mathrm{e} ^ {- x ^ {2}} \mathrm{d} x
$$

or the integral of an unbounded function: 

$$
\int_ {0} ^ {1} \frac {1}{\sqrt {x}} \mathrm{d} x,
$$

we have to resort to ‘improper’ Riemann integrals, defined by a limit process: e.g. considering the integrals 

$$
\int_ {- n} ^ {n} \mathrm{e} ^ {- x ^ {2}} \mathrm{d} x, \quad \int_ {\varepsilon} ^ {1} \frac {1}{\sqrt {x}} \mathrm{d} x,
$$

and letting $n  \infty \mathrm { o r } \varepsilon  0$ respectively. This isn’t all that serious a flaw. 

Second, dependence on intervals: we have no easy way of integrating over more general sets, or of integrating functions whose values are distributed ‘awkwardly’ over sets that difer greatly from intervals. For example, consider the upper and lower sums for the indicator function $\mathbf { 1 } _ { \mathbb { Q } }$ of $\mathbb { Q }$ over [0, 1]; however we partition [0, 1], each subinterval must contain both rational and irrational points; thus each upper sum is 1 and each lower sum 0. Hence we cannot calculate the Riemann integral of $f$ over the interval [0,1]; it is simply ‘too discontinuous’. (You may easily convince yourself that $f$ is discontinuous at all points of [0, 1].) 

Third, lack of completeness: rather more importantly from the point of view of applications, the Riemann integral doesn’t interact well with taking the limit of a sequence of functions. One may expect results of the following form: if a sequence $f _ { n }$ of Riemann-integrable functions converges (in some appropriate sense) to $f ,$ then $\textstyle \int _ { a } ^ { b } f _ { n } \mathrm { d } x \to \bar { \int _ { a } ^ { b } f }$ dx. 

R RWe give two counterexamples showing what dificulties can arise if the functions $\left( f _ { n } \right)$ converge to $f$ pointwise, i.e. $f _ { n } ( x )  f ( x )$ for all $x .$ 

1. The limit need not be Riemann integrable, and so the convergence question does not even make sense. Here we may take $f = 1 _ { \mathbb { Q } } , f _ { n } = 1 _ { A _ { n } }$ where 

$A _ { n } = \left\{ q _ { 1 } , \ldots , q _ { n } \right\}$ , and the sequence $( q _ { n } ) , n \ge 1$ is an enumeration of the rationals, so that $\left( f _ { n } \right)$ is even monotone increasing. 

2. The limit is Riemann integrable, but the convergence of Riemann integrals does not hold. Let $f = 0$ , consider $[ a , b ] = [ 0 , 1 ]$ , and put 

$$
f _ {n} (x) = \left\{ \begin{array}{l l} 4 n ^ {2} x & \text {if} 0 \leq x <   \frac {1}{2 n} \\ 4 n - 4 n ^ {2} x & \text {if} \frac {1}{2 n} \leq x <   \frac {1}{n} \\ 0 & \text {if} \frac {1}{n} \leq x \leq 1. \end{array} \right.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/4f5ec154023e1b2ee7e26158ecc06df644ee16bd0d96facd3930e43c60d13f20.jpg)



Figure 1.1 Graph of $f _ { n }$ .


This is a continuous function with integral 1. On the other hand, the sequence $f _ { n } ( x )$ converges to $f = 0$ since for all $x , f _ { n } ( x ) = 0$ for n suficiently large (such that $\textstyle { \frac { 1 } { n } } < x )$ . See Figure 1.1. 

To avoid problems of this kind, we can introduce the idea of uniform convergence: a sequence $\left( f _ { n } \right)$ in $C [ 0 , 1 ]$ converges uniformly to f if the sequence $a _ { n } = \operatorname* { s u p } \{ | f _ { n } ( x ) - f ( x ) | : 0 \leq x \leq 1 \}$ converges to 0. In this case one can easily prove the convergence of the Riemann integrals: 

$$
\int_ {0} ^ {1} f _ {n} (x) \mathrm{d} x \rightarrow \int_ {0} ^ {1} f (x) \mathrm{d} x.
$$

However, the ‘distance’ s $\operatorname* { u p } \{ | f ( x ) - g ( x ) | : 0 \leq x \leq 1 \}$ has nothing to do with integration as such and the uniform convergence is too restrictive for many applications. A more natural concept of ‘distance’, given by $\begin{array} { r } { \int _ { 0 } ^ { 1 } | f ( x ) - g ( x ) | } \end{array}$ dx, leads to another problem. Defining 

$$
g _ {n} (x) = \left\{ \begin{array}{l l} 0 & \text { if } 0 \leq x \leq \frac {1}{2} \\ n (x - \frac {1}{2}) & \text { if } \frac {1}{2} <   x <   \frac {1}{2} + \frac {1}{n} \\ 1 & \text { otherwise } \end{array} \right.
$$

it can be shown that $\begin{array} { r } { \int _ { 0 } ^ { 1 } | g _ { n } ( x ) - g _ { m } ( x ) | \mathrm { d } x  0 } \end{array}$ as $m , n \to \infty ;$ in Figure 1.2 the Rshaded area vanishes. (We say that $\left( f _ { n } \right)$ is a Cauchy sequence in this distance.) 

Yet there is no continuous function f to which this sequence converges since the pointwise limit is $f ( x ) = 1$ for $\begin{array} { r } { x > \frac { 1 } { 2 } } \end{array}$ and 0 otherwise, so that $f = \mathbf { 1 } _ { ( \frac { 1 } { 2 } , 1 ] }$ So the space $C ( [ 0 , 1 ] )$ of all continuous functions $f \colon [ 0 , 1 ] \to \mathbb { R }$ is too small from this point of view. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/5db496d27bdd28a03b7903431d89aa83573837237406d66712c60c0b803abe2c.jpg)



Figure 1.2 Graphs of $g _ { n }$ , $g _ { m }$


This is rather similar to the situation which leads one to work with R rather than just with the set of rationals Q (there are Cauchy sequences without limits in Q, for example a sequence of rational approximations of $\sqrt { 2 } )$ . Recalling the crucial importance of completeness in the case of R, we naturally look for a theory of integration which does not have this shortcoming. In the process we shall find that our new theory, which will include the Riemann integral as a special case, also solves the other problems listed. 

## 1.3 Choosing numbers at random

Before we start to develop the theory of Lebesgue measure to make sense of the ‘length’ of a general subset of R, let us pause to consider some practical motivation. The simplicity of elementary probability with finite sample spaces vanishes rapidly when we have an infinite number of outcomes, such as when we ‘pick a number between 0 and 1 at random’. We face making sense of the ‘probability’ that a given $x \in [ 0 , 1 ]$ is chosen. A similar, slightly more general question, is the following: what is the probability that the number we pick is rational? 

First a prior question: what do we mean by saying that we pick the number x at random? ‘Random’ plausibly means that in each such trial, each real number is ‘equally likely’ to be picked, so that we impose the uniform probability distribution on [0, 1]. But the ‘number’ of possible choices is infinite. Hence the event $A _ { x }$ that a fixed x is chosen ought to have zero probability. On the other hand, since some number between 0 and 1 is chosen, and it is not impossible that it could be our x. Thus a set $A _ { x } \neq \varnothing$ can have $P ( A _ { x } ) = 0$ . Our way of ‘measuring’ probabilities need not, therefore, be able to distinguish completely between sets – we could not really expect this in general if we want to handle infinite sets. 

We can go slightly further: the probability that any one of a finite set of reals $A = \{ x _ { 1 } , x _ { 2 } , . . . , x _ { n } \}$ is selected should also be 0, since it seems natural that this probability $P ( A )$ should equal $\textstyle \sum _ { i = 1 } ^ { n } P ( \{ x _ { i } \} )$ . We can extend this to Pclaim the finite additivity property of the probability function $A \mapsto P ( A )$ , i.e. that if $A _ { 1 } , A _ { 2 } , . . . , A _ { n }$ are disjoint sets, then $\begin{array} { r } { P ( \bigcup _ { i = 1 } ^ { n } A _ { i } ) = \sum _ { i = 1 } ^ { n } P ( A _ { i } ) } \end{array}$ . This S Pclaim looks very plausible, and we shall see that it becomes an essential feature of any sensible basis for a calculus of probabilities. 

Less obvious is the claim that, under the uniform distribution, any countably infinite set, such as $\mathbb { Q }$ , must also carry probability $0 -$ yet that is exactly what an analysis of the ‘area under the graph’ of the function $\mathbf { 1 } _ { \mathbb { Q } }$ suggests. We can reinterpret this as a result of a ‘continuity property’ of the mapping $A \mapsto P ( A )$ when we let $n \to \infty$ in the above: if the sequence $\left( A _ { i } \right)$ of subsets of R is disjoint then we would like to have 

$$
P (\bigcup_ {i = 1} ^ {\infty} A _ {i}) = \lim _ {n \to \infty} \sum_ {i = 1} ^ {n} P (A _ {i}) = \sum_ {i = 1} ^ {\infty} P (A _ {i}).
$$

We shall see in Chapter 2 that this condition is indeed satisfied by Lebesgue measure on the real line R, and it will be used as the defining property of abstract measures on arbitrary sets. 

There is much more to probability than is developed in this book: for example, we do not discuss finite sample spaces and the elegant combinatorial ideas that characterize a good introduction to probability, such as [6] and [9]. Our focus throughout remains on the essential role played by Lebesgue measure in the description of probabilistic phenomena based on infinite sample spaces. This leads us to leave to one side many of the interesting examples and applications which can be found in these texts, and provide, instead, a consistent development of the theoretical underpinnings of random variables with densities. 

## 2.1 Null sets

The idea of a ‘negligible’ set relates to one of the limitations of the Riemann integral, as we saw in the previous chapter. Since the function $f = \mathbf { 1 } _ { \mathbb { Q } }$ takes a non-zero value only on Q, and equals 1 there, the ‘area under its graph’ (if such makes sense) must be very closely linked to the ‘length’ of the set Q. This is why it turns out that we cannot integrate f in the Riemann sense: the sets Q and $\mathbb { R } \setminus \mathbb { Q }$ are so diferent from intervals that it is not clear how we should measure their ‘lengths’ and it is clear that the ‘integral’ of f over [0, 1] should equal the ‘length’ of the set of rationals in [0, 1]. So how should we define this concept for more general sets? 

The obvious way of defining the ‘length’ of a set is to start with intervals nonetheless. Suppose that I is a bounded interval of any kind, i.e. $I = [ a , b ]$ 2 $I = [ a , b ) , I = ( a , b ] { \mathrm { o r } } I = ( a , b )$ . We simply define the length of I as $l ( I ) = b { - } a$ in each case. 

As a particular case we have $l ( \{ a \} ) = l ( [ a , a ] ) = 0$ . It is then natural to say that a one-element set is ‘null’. Before we extend this idea to more general sets, first consider the length of a finite set. A finite set is not an interval but since a single point has length 0, adding finitely many such lengths together should still give 0. The underlying concept here is that if we decompose a set into a finite number of disjoint intervals, we compute the length of this set by adding the lengths of the pieces. 

As we have seen, in general it may not be always possible actually to decompose a set into intervals. Therefore, we consider systems of intervals that cover a given set. We shall generalize the above idea by allowing a countable number of covering intervals. Thus we arrive at the following more general definition of sets of ‘zero length’: 

## Definition 2.1

A null set $A \subseteq \mathbb { R }$ is a set that may be covered by a sequence of intervals of arbitrarily small total length, i.e. given any $\varepsilon > 0$ we can find a sequence $\{ I _ { n } : n \geq 1 \}$ of intervals such that 

$$
A \subseteq \bigcup_ {n = 1} ^ {\infty} I _ {n}
$$

and 

$$
\sum_ {n = 1} ^ {\infty} l (I _ {n}) <   \varepsilon .
$$

(We also say simply that ‘A is null’.) 

## Exercise 2.1

Show that we get an equivalent notion if in the above definition we replace the word ‘intervals’ by any of these: ‘open intervals’, ‘closed intervals’, ‘the intervals of the form $( a , b ]$ , ‘the intervals of the form $[ a , b ) ^ { \prime }$ 

Note that the intervals do not need to be disjoint. It follows at once from the definition that the empty set is null. 

Next, any one-element set x is a null set. For, let $\varepsilon > 0$ and take $I _ { 1 } =$ $( x - { \textstyle { \frac { \varepsilon } { 4 } } } , x + { \textstyle { \frac { \varepsilon } { 4 } } } ) , I _ { n } = [ 0 , 0 ]$ for $n \geq 2$ . (Why take $I _ { n } = [ 0 , 0 ]$ for $n \geq 2 ?$ Well, why not! We could equally have taken $I _ { n } = ( 0 , 0 ) = \emptyset$ , of course!) Now 

$$
\sum_ {n = 1} ^ {\infty} l (I _ {n}) = l (I _ {1}) = \frac {\varepsilon}{2} <   \varepsilon .
$$

More generally, any countable set $A = \{ x _ { 1 } , x _ { 2 } , \ldots \}$ is null. The simplest way to show this is to take $I _ { n } = [ x _ { n } , x _ { n } ]$ , for all n. However, as a gentle introduction to the next theorem we will cover A by open intervals. This way it is more fun. 

For, let $\varepsilon > 0$ and cover A with the following sequence of intervals 

$$
I _ {1} = (x _ {1} - \frac {\varepsilon}{8}, x _ {1} + \frac {\varepsilon}{8}) l (I _ {1}) = \frac {1}{2} \varepsilon \cdot \frac {1}{2 ^ {1}}
$$

$$
I _ {2} = (x _ {2} - \frac {\varepsilon}{1 6}, x _ {2} + \frac {\varepsilon}{1 6}) l (I _ {2}) = \frac {1}{2} \varepsilon \cdot \frac {1}{2 ^ {2}}
$$

$$
I _ {3} = (x _ {3} - \frac {\varepsilon}{3 2}, x _ {3} + \frac {\varepsilon}{3 2}) l (I _ {3}) = \frac {1}{2} \varepsilon \cdot \frac {1}{2 ^ {3}}
$$

$$
I _ {n} = \left(x _ {n} - \frac {\varepsilon}{2 \cdot 2 ^ {n}}, x _ {n} + \frac {\varepsilon}{2 \cdot 2 ^ {n}}\right) l (I _ {n}) = \frac {1}{2} \varepsilon \cdot \frac {1}{2 ^ {n}}
$$

Since $\textstyle \sum _ { n = 1 } ^ { \infty } { \frac { 1 } { 2 ^ { n } } } = 1$ 

$$
\sum_ {n = 1} ^ {\infty} l (I _ {n}) = \frac {\varepsilon}{2} <   \varepsilon
$$

as needed. 

Here we have the following situation: A is the union of countably many one-element sets. Each of them is null and A turns out to be null as well. 

We can generalize this simple observation: 

## Theorem 2.1

If $( N _ { n } ) _ { n \geq 1 }$ is a sequence of null sets, then their union 

$$
N = \bigcup_ {n = 1} ^ {\infty} N _ {n}
$$

is also null. 

## Proof

We assume that all $N _ { n } , n \geq 1$ , are null and to show that the same is true for N we take any $\varepsilon > 0$ . Our goal is to cover the set N by countably many intervals with total length less than ε. 

The proof goes in three steps, each being a little bit tricky. 

Step 1. We carefully cover each $N _ { n }$ by intervals. 

‘Carefully’ means that the lengths have to be small. ‘Small’ means that we are going to add them up later to end up with a small number (and ‘small here means less than ε). 

Since $N _ { 1 }$ is null, there exist intervals $I _ { k } ^ { 1 } , k \geq 1$ , such that 

$$
\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {1}) <   \frac {\varepsilon}{2}, N _ {1} \subseteq \bigcup_ {k = 1} ^ {\infty} I _ {k} ^ {1}.
$$

For $N _ { 2 }$ we find a system of intervals $I _ { k } ^ { 2 } , k \geq 1$ , with 

$$
\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {2}) <   \frac {\varepsilon}{4}, \quad N _ {2} \subseteq \bigcup_ {k = 1} ^ {\infty} I _ {k} ^ {2}.
$$

You can see a cunning plan of making the total lengths smaller at each step at a geometric rate. In general, we cover $N _ { n }$ with intervals $I _ { k } ^ { n } , k \geq 1$ , whose total length is less than $\frac { \varepsilon } { 2 ^ { n } }$ : 

$$
\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {n}) <   \frac {\varepsilon}{2 ^ {n}}, N _ {n} \subseteq \bigcup_ {k = 1} ^ {\infty} I _ {k} ^ {n}.
$$

Step 2. The intervals $I _ { k } ^ { n }$ form a sequence. 

We arrange the countable family of intervals $\{ I _ { k } ^ { n } \} _ { k \geq 1 , n \geq 1 }$ into a sequence $J _ { j } , j \ge 1$ . For instance we put $J _ { 1 } = I _ { 1 } ^ { 1 } , J _ { 2 } = I _ { 2 } ^ { 1 } , J _ { 3 } = I _ { 1 } ^ { 2 } , J _ { 4 } = I _ { 3 } ^ { 1 }$ , etc. so that none of the $I _ { k } ^ { n }$ are skipped. The union of the new system of intervals is the same as the union of the old one and so 

$$
N = \bigcup_ {n = 1} ^ {\infty} N _ {n} \subseteq \bigcup_ {n = 1} ^ {\infty} \bigcup_ {k = 1} ^ {\infty} I _ {k} ^ {n} = \bigcup_ {j = 1} ^ {\infty} J _ {j}.
$$

Step 3. Compute the total length of $J _ { j }$ . 

This is tricky because we have a series of numbers with two indices: 

$$
\sum_ {j = 1} ^ {\infty} l (J _ {j}) = \sum_ {n = 1, k = 1} ^ {\infty} l (I _ {k} ^ {n}).
$$

Now we wish to write this as a series of numbers each being the sum of a series. We can rearrange the double sum because the components are non-negative (a fact from elementary calculus). 

$$
\sum_ {n = 1, k = 1} ^ {\infty} l (I _ {k} ^ {n}) = \sum_ {n = 1} ^ {\infty} \left(\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {n})\right) <   \sum_ {n = 1} ^ {\infty} \frac {\varepsilon}{2 ^ {n}} = \varepsilon ,
$$

which completes the proof. 

Thus any countable set is null, and null sets appear to be closely related to countable sets – this is no surprise as any proper interval is uncountable, so any countable subset is quite ‘sparse’ when compared with an interval, hence makes no real contribution to its ‘length’. (You may also have noticed the similarity between Step 2 in the above proof and the ‘diagonal argument’ which is commonly used to show that $\mathbb { Q }$ is a countable set.) 

However, uncountable sets can be null, provided their points are suficiently ‘sparsely distributed’, as the following famous example, due to Cantor, shows: 

1. Start with the interval [0, 1], remove the ‘middle third’, that is the interval $\left( { \frac { 1 } { 3 } } , { \frac { 2 } { 3 } } \right)$ , obtaining the set $C _ { 1 }$ , which consists of the two intervals $[ 0 , \textstyle { \frac { 1 } { 3 } } ]$ and $[ \frac { 2 } { 3 } , 1 ]$ 

2. Next remove the middle third of each of these two intervals, leaving $C _ { 2 }$ consisting of four intervals, each of length $\textstyle { \frac { 1 } { 9 } }$ , etc. (See Figure 2.1.) 

3. At the nth stage we have a set $C _ { n }$ , consisting of $2 ^ { n }$ disjoint closed intervals, each of length $\frac { 1 } { 3 ^ { n } }$ . Thus the total length of $C _ { n }$ is $\left( { \frac { 2 } { 3 } } \right) ^ { n }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/64f587f3ba5be2d0187e209dab22d3c97e1aed915d368b0ce0d5afb1a921b4f1.jpg)



Figure 2.1 Cantor set construction $\left( C _ { 3 } \right)$


We call 

$$
C = \bigcap_ {n = 1} ^ {\infty} C _ {n}
$$

the Cantor set. 

Now we show that C is null as promised. 

Given any $\varepsilon > 0$ , choose n so large that $\left( { \frac { 2 } { 3 } } \right) ^ { n } < \varepsilon$ . Since $C \subseteq C _ { n }$ , and $C _ { n }$   consists of a (finite) sequence of intervals of total length less than ε, we see that C is a null set. 

All that remains is to check that C is an uncountable set. This is left for you as 

Exercise 2.2 

Prove that C is uncountable. 

Hint Adapt the proof of the uncountability of R: begin by expressing each x in [0, 1] in ternary form: 

$$
x = \sum_ {k = 1} ^ {\infty} \frac {a _ {k}}{3 ^ {k}} = 0. a _ {1} a _ {2} \dots
$$

with $a _ { k } = 0 , 1$ or 2. Note that $x \in C$ if all its $a _ { k }$ equal 0 or 2. 

Why is the Cantor set null, even though it is uncountable? Clearly it is the distribution of its points, the fact that it is ‘spread out’ all over [0,1], which causes the trouble. This makes it the source of many examples which show that intuitively ‘obvious’ things are not always true! For example, we can use the Cantor set to define a function, due to Lebesgue, with very odd properties: 

If $x \in [ 0 , 1 ]$ has ternary expansion $( a _ { n } ) , { \mathrm { i . e . ~ } } x = 0 . a _ { 1 } a _ { 2 } \ldots$ . with $a _ { n } = 0 , 1$ or 2, define N as the first index n for which $a _ { n } = 1$ , and set $N = \infty$ if none of the $a _ { n }$ are 1 (i.e. when $x \in C )$ . Now set $\begin{array} { r } { b _ { n } = \frac { a _ { n } } { 2 } } \end{array}$ for $n < N$ and $b _ { N } = 1$ and let $\begin{array} { r } { F ( x ) = \sum _ { n = 1 } ^ { N } \frac { b _ { n } } { 2 ^ { n } } } \end{array}$ for each $x \in [ 0 , 1 ]$ . Clearly, this function is monotone Pincreasing and has $F ( 0 ) = 0 , F ( 1 ) = 1$ . Yet it is constant on the middle thirds (i.e. the complement of C), so all its increase occurs on the Cantor set. Since we have shown that C is a null set, $F$ ‘grows’ from 0 to 1 entirely on a ‘negligible set. The following exercise shows that it has no jumps! 

## Exercise 2.3

Prove that the Lebesgue function F is continuous and sketch its graph. 

## 2.2 Outer measure

The simple concept of null sets provides the key to our idea of length, since it tells us what we can ‘ignore’. A quite general notion of ‘length’ is now provided by: 

## Definition 2.2

The (Lebesgue) outer measure of any set $A \subseteq \mathbb { R }$ is given by 

$$
m ^ {*} (A) = \inf Z _ {A}
$$

where 

$$
Z _ {A} = \left\{\sum_ {n = 1} ^ {\infty} l \left(I _ {n}\right): I _ {n} \text { are   intervals }, A \subseteq \bigcup_ {n = 1} ^ {\infty} I _ {n} \right\}.
$$

We say the $( I _ { n } ) _ { n \geq 1 }$ cover the set A. So the outer measure is the infimum of lengths of all possible covers of A. (Note again that some of the $I _ { n }$ may be empty; this avoids having to worry whether the sequence $\left( I _ { n } \right)$ has finitely or infinitely many diferent members.) 

Clearly $m ^ { * } ( A ) \geq 0$ for any $A \subseteq \mathbb { R }$ . For some sets A, the series $\textstyle \sum _ { n = 1 } ^ { \infty } l ( I _ { n } )$ may diverge for any covering of A, so $m ^ { * } ( A )$ may by equal to $\infty$ . Since we wish to be able to add the outer measures of various sets we have to adopt a convention to deal with infinity. An obvious choice is $a + \infty = \infty , \infty + \infty = \infty$ and a less obvious but quite practical assumption is $0 \times \infty = 0$ , as we have already seen. 

The set $Z _ { A }$ is bounded from below by 0 so the infimum always exists. If $r \in Z _ { A }$ , then $[ r , + \infty ] \subseteq Z _ { A }$ (clearly, we may expand the first interval of any cover to increase the total length by any number). This shows that $Z _ { A }$ is either $\{ + \infty \}$ or the interval $( x , + \infty ]$ or $[ x , + \infty ]$ for some real number x. So the infimum of $Z _ { A }$ is just x. 

First we show that the concept of null set is consistent with that of outer measure: 

## Theorem 2.2

$A \subseteq \mathbb { R }$ is a null set if and only if $m ^ { * } ( A ) = 0$ 

## Proof

Suppose that A is a null set. We wish to show that inf $Z _ { A } = 0$ . To this end we show that for any $\varepsilon > 0$ we can find an element $z \in Z _ { A }$ such that $z < \varepsilon$ 

By the definition of null set we can find a sequence $\left( I _ { n } \right)$ of intervals covering A with $\textstyle \sum _ { n = 1 } ^ { \infty } l ( I _ { n } ) < \varepsilon$ and so $\textstyle \sum _ { n = 1 } ^ { \infty } l ( I _ { n } )$ is the required element $z$ of $Z _ { A }$ 

PConversely, if $A \subseteq \mathbb { R }$ has $m ^ { * } ( A ) = 0$ , then by the definition of inf, given any $\varepsilon > 0$ , there is $z \in Z _ { A } , z < \varepsilon$ . But a member of $Z _ { A }$ is the total length of some covering of A. That is, there is a covering $\left( I _ { n } \right)$ of A with total length less than $\varepsilon ,$ so A is null. □ 

This combines our general outer measure with the special case of ‘zero measure’. Note that $m ^ { * } ( \emptyset ) = 0 , m ^ { * } ( \{ x \} ) = 0$ for any $x \in \mathbb { R }$ , and $m ^ { * } ( \mathbb { Q } ) = 0$ (and in fact, for any countable X, $m ^ { * } ( X ) = 0 )$ 

Next we observe that $m ^ { * }$ is monotone: the bigger the set, the greater its outer measure. 

## Proposition 2.3

If $A \subset B$ then $m ^ { * } ( A ) \leq m ^ { * } ( B )$ 

Hint Show that $Z _ { B } \subset Z _ { A }$ and use the definition of inf. 

The second step is to relate outer measure to the length of an interval. This innocent result contains the crux of the theory, since it shows that the formal definition of $m ^ { * }$ , which is applicable to all subsets of R, coincides with the intuitive idea for intervals, where our thought processes began. We must therefore expect the proof to contain some hidden depths, and we have to tackle these in stages: the hard work lies in showing that the length of the interval cannot be greater than its outer measure: for this we need to appeal to the famous Heine–Borel theorem, which states that every closed, bounded subset B of R is compact: given any collection of open sets $O _ { \alpha }$ covering B (i.e. $\textstyle B \subset \bigcup _ { \alpha } O _ { \alpha } )$ , there is a finite subcollection $( O _ { \alpha _ { i } } ) _ { i \leq n }$ which still covers B, i.e. $B \subset \textstyle \bigcup _ { i = 1 } ^ { n } O _ { \alpha _ { i } }$ (for a proof see [1]). 

## Theorem 2.4

The outer measure of an interval equals its length. 

## Proof

If I is unbounded, then it is clear that it cannot be covered by a system of intervals with finite total length. This shows that $m ^ { * } ( I ) = \infty$ and so $m ^ { * } ( I ) =$ $l ( I ) = \infty$ 

So we restrict ourselves to bounded intervals. 

Step 1. $m ^ { * } ( I ) \leq l ( I )$ 

We claim that $l ( I ) \in Z _ { I }$ . Take the following sequence of intervals: $I _ { 1 } = I$ $I _ { n } = [ 0 , 0 ]$ for $n \geq 2$ . This sequence covers the set I, and the total length is equal to the length of I hence $l ( I ) \in Z _ { I }$ . This is suficient since the infimum of $Z _ { I }$ cannot exceed any of its elements. 

Step 2. $l ( I ) \leq m ^ { * } ( I )$ 

(1) $I = [ a , b ]$ . We shall show that for any $\varepsilon > 0$ 

$$
l ([ a, b ]) \leq m ^ {*} ([ a, b ]) + \varepsilon .\tag{2.1}
$$

This is suficient since we may obtain the required inequality passing to the limit, $\varepsilon  0$ . (Note that if $x , y \in \mathbb { R }$ and $y > x$ then there is an $\varepsilon > 0$ with $y > x + \varepsilon , { \mathrm { e . g . ~ } } \varepsilon = { \textstyle { \frac { 1 } { 2 } } } ( y - x ) . )$ 

So we take an arbitrary $\varepsilon > 0$ . By the definition of outer measure we can find a sequence of intervals $I _ { n }$ covering [a, b] such that 

$$
\sum_ {n = 1} ^ {\infty} l (I _ {n}) \leq m ^ {*} ([ a, b ]) + \frac {\varepsilon}{2}.\tag{2.2}
$$

We shall slightly increase each of the intervals to an open one. Let the endpoints of $I _ { n }$ be $a _ { n } , b _ { n }$ , and we take 

$$
J _ {n} = \big (a _ {n} - \frac {\varepsilon}{2 ^ {n + 2}}, b _ {n} + \frac {\varepsilon}{2 ^ {n + 2}} \big).
$$

It is clear that 

$$
l (I _ {n}) = l (J _ {n}) - \frac {\varepsilon}{2 ^ {n + 1}}
$$

so that 

$$
\sum_ {n = 1} ^ {\infty} l (I _ {n}) = \sum_ {n = 1} ^ {\infty} l (J _ {n}) - \frac {\varepsilon}{2}.
$$

We insert this in (2.2) and we have 

$$
\sum_ {n = 1} ^ {\infty} l (J _ {n}) \leq m ^ {*} ([ a, b ]) + \varepsilon .\tag{2.3}
$$

The new sequence of intervals of course covers $[ a , b ]$ so by the Heine–Borel theorem we can choose a finite number of $J _ { n }$ to cover $[ a , b ]$ (the set $[ a , b ]$ is compact in R). We can add some intervals to this finite family to form an initial segment of the sequence $( J _ { n } ) \mathrm { ~ - ~ } \mathrm { j u s t }$ for simplicity of notation. So for some finite index m we have 

$$
[ a, b ] \subseteq \bigcup_ {n = 1} ^ {m} J _ {n}.\tag{2.4}
$$

Let $J _ { n } = \left( c _ { n } , d _ { n } \right)$ . Put $c = \operatorname* { m i n } \{ c _ { 1 } , \dots , c _ { m } \} , d = \operatorname* { m a x } \{ d _ { 1 } , \dots , d _ { m } \}$ . The covering (2.4) means that $c < a$ and $b < d$ hence $l ( [ a , b ] ) < d - c .$ 

Next, the number $d - c$ is certainly smaller than the total length of $J _ { n }$ $n = 1 , \ldots , m$ (some overlapping takes place) and 

$$
l ([ a, b ]) <   d - c <   \sum_ {n = 1} ^ {m} l (J _ {n}).\tag{2.5}
$$

Now it is suficient to put (2.3) and (2.5) together in order to deduce (2.1) (the finite sum is less than or equal to the sum of the series since all terms are non-negative). 

(2) $\boldsymbol { I } = \left( a , b \right)$ . As before, it is suficient to show (2.1). Let us fix any $\varepsilon > 0$ 

$$
\begin{array}{l} l ((a, b)) = l ([ a + \frac {\varepsilon}{2}, b - \frac {\varepsilon}{2} ]) + \varepsilon \\ \qquad \leq m ^ {*} ([ a + \frac {\varepsilon}{2}, b - \frac {\varepsilon}{2} ]) + \varepsilon \quad (\text { by   (1) }) \\ \qquad \leq m ^ {*} ((a, b)) + \varepsilon \quad (\text { by   Proposition   2.3 }). \end{array}
$$

(3) $I = [ a , b ) { \mathrm { ~ o r ~ } } I = ( a , b ] .$ 

$$
\begin{array}{r l} & l (I) = l ((a, b)) \leq m ^ {*} ((a, b)) \quad (\text { by   (2) }) \\ & \qquad \leq m ^ {*} (I) \quad (\text { by   Proposition   2.3 }) \end{array}
$$

which completes the proof. 

Having shown that outer measure coincides with the natural concept of length for intervals, we now need to investigate its properties. The next theorem gives us an important technical tool which will be used in many proofs. 

## Theorem 2.5

Outer measure is countably subadditive, i.e. for any sequence of sets $\{ E _ { n } \}$ 

$$
m ^ {*} \big (\bigcup_ {n = 1} ^ {\infty} E _ {n} \big) \leq \sum_ {n = 1} ^ {\infty} m ^ {*} (E _ {n}).
$$

(Note that both sides may be infinite here.) 

## Proof (a warm up)

Let us prove first a simpler statement: 

$$
m ^ {*} (E _ {1} \cup E _ {2}) \leq m ^ {*} (E _ {1}) + m ^ {*} (E _ {2}).
$$

Take an $\varepsilon > 0$ and we show an even easier inequality 

$$
m ^ {*} (E _ {1} \cup E _ {2}) \leq m ^ {*} (E _ {1}) + m ^ {*} (E _ {2}) + \varepsilon .
$$

This is however suficient because taking $\textstyle { \varepsilon = { \frac { 1 } { n } } }$ and letting $n \to \infty$ we get what we need. 

So for any $\varepsilon > 0$ we find covering sequences $( I _ { k } ^ { 1 } ) _ { k \geq 1 }$ of $E _ { 1 }$ and $( I _ { k } ^ { 2 } ) _ { k \geq 1 }$ of $E _ { 2 }$ such that 

$$
\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {1}) \leq m ^ {*} (E _ {1}) + \frac {\varepsilon}{2},
$$

$$
\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {2}) \leq m ^ {*} (E _ {2}) + \frac {\varepsilon}{2}
$$

hence, adding up, 

$$
\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {1}) + \sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {2}) \leq m ^ {*} (E _ {1}) + m ^ {*} (E _ {2}) + \varepsilon .
$$

The sequence of intervals $( I _ { 1 } ^ { 1 } , I _ { 1 } ^ { 2 } , I _ { 2 } ^ { 1 } , I _ { 2 } ^ { 2 } , I _ { 3 } ^ { 1 } , I _ { 3 } ^ { 2 } , . . . )$ covers $E _ { 1 } \cup E _ { 2 }$ hence 

$$
m ^ {*} (E _ {1} \cup E _ {2}) \leq \sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {1}) + \sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {2})
$$

which combined with the previous inequality gives the result. 

## Proof (of the Theorem)

If the right-hand side is infinite, then the inequality is of course true. $\mathrm { S o } .$ suppose that $\textstyle \sum _ { n = 1 } ^ { \infty } m ^ { * } ( E _ { n } ) < \infty$ . For each given $\varepsilon > 0$ and $n \geq 1$ find a covering sequence $( I _ { k } ^ { n } ) _ { k \geq 1 }$ of $E _ { n }$ with 

$$
\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {n}) \leq m ^ {*} (E _ {n}) + \frac {\varepsilon}{2 ^ {n}}.
$$

The iterated series converges: 

$$
\sum_ {n = 1} ^ {\infty} \left(\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {n})\right) \leq \sum_ {n = 1} ^ {\infty} m ^ {*} (E _ {n}) + \varepsilon <   \infty
$$

and since all its terms are non-negative, 

$$
\sum_ {n = 1} ^ {\infty} \left(\sum_ {k = 1} ^ {\infty} l (I _ {k} ^ {n})\right) = \sum_ {n, k = 1} ^ {\infty} l (I _ {k} ^ {n}).
$$

The system of intervals $( I _ { k } ^ { n } ) _ { k , n \geq 1 }$ covers $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ hence 

$$
m ^ {*} \big (\bigcup_ {n = 1} ^ {\infty} E _ {n} \big) \leq \sum_ {n, k = 1} ^ {\infty} l (I _ {k} ^ {n}) \leq \sum_ {n = 1} ^ {\infty} m ^ {*} (E _ {n}) + \varepsilon .
$$

To complete the proof we let $\varepsilon \to 0$ 

A similar result is of course true for a finite family $( E _ { n } ) _ { n = 1 } ^ { m }$ 

$$
m ^ {*} \left(\bigcup_ {n = 1} ^ {m} E _ {n}\right) \leq \sum_ {n = 1} ^ {m} m ^ {*} \left(E _ {n}\right).
$$

It is a corollary to Theorem 2.5 with $E _ { k } = \emptyset$ for $k > m$ 

## Exercise 2.4

Prove that if $m ^ { * } ( A ) = 0$ then for each B, $m ^ { * } ( A \cup B ) = m ^ { * } ( B )$ 

Hint Employ both monotonicity and subadditivity of outer measure. 

Exercise 2.5 

Prove that if $m ^ { * } ( A { \varDelta } B ) = 0 , \mathrm { t h e n } m ^ { * } ( A ) = m ^ { * } ( B )$ 

Hint Note that $A \subseteq B \cup ( A \varDelta B )$ 

We conclude this section with a simple and intuitive property of outer measure. Note that the length of an interval does not change if we shift it along the real line: $l ( [ a , b ] ) = l ( [ a + t , b + t ] ) = b - a$ for example. Since the outer measure is defined in terms of the lengths of intervals, it is natural to expect it to share this property. For $A \subset \mathbb { R }$ and $t \in \mathbb { R }$ we put $A + t = \{ a + t : a \in A \}$ 

## Proposition 2.6

Outer measure is translation invariant, i.e. 

$$
m ^ {*} (A) = m ^ {*} (A + t)
$$

for each A and t. 

Hint Combine two facts: the length of interval does not change when the interval is shifted and outer measure is determined by the length of the coverings. 

## 2.3 Lebesgue measurable sets and Lebesgue measure

With outer measure, subadditivity (as in Theorem 2.5 is as far as we can get. We wish, however, to ensure that if sets $\left( E _ { n } \right)$ are pairwise disjoint $( \mathrm { i . e . } \ E _ { i } \cap E _ { j } = \emptyset$ if $i \neq j )$ , then the inequality in Theorem 2.5 becomes an equality. It turns out that this will not in general be true for outer measure, although examples where it fails are quite dificult to construct (we give such examples in the Appendix). But our wish is an entirely reasonable one: any ‘length function’ should at least be finitely additive, since decomposing a set into finitely many disjoint pieces should not alter its length. Moreover, since we constructed our length function via approximation of complicated sets by ‘simpler’ sets (i.e. intervals) it seems fair to demand a continuity property: if pairwise disjoint $\left( E _ { n } \right)$ have union $E _ { : }$ then the lengths of the sets $B _ { n } = E \setminus \bigcup _ { k = 1 } ^ { n } E _ { k }$ may be expected to decrease to 0 as $n \to \infty$ S. Combining this with finite additivity leads quite naturally to the demand that ‘length’ should be countably additive, i.e. that 

$$
m ^ {*} \left(\bigcup_ {n = 1} ^ {\infty} E _ {n}\right) = \sum_ {n = 1} ^ {\infty} m ^ {*} (E _ {n}) \quad \text { when } E _ {i} \cap E _ {j} = \emptyset \text { for } i \neq j.
$$

We therefore turn to the task of finding the class of sets in R which have this property. It turns out that it is also the key property of the abstract concept of measure, and we will use it to provide mathematical foundations for probability. 

In order to define the ‘good’ sets which have this property, it also seems plausible that such a set should apportion the outer measure of every set in R properly, as we state in Definition 2.3 below. Remarkably, this simple demand will sufice to guarantee that our ‘good’ sets have all the properties we demand of them! 

## Definition 2.3

A set $E \subseteq \mathbb { R }$ is (Lebesgue) measurable if for every set $A \subseteq \mathbb { R }$ we have 

$$
m ^ {*} (A) = m ^ {*} (A \cap E) + m ^ {*} (A \cap E ^ {c})\tag{2.6}
$$

where $E ^ { c } = \mathbb { R } \backslash E$ , and we write $E \in { \mathcal { M } }$ 

We obviously have $A = ( A \cap E ) \cup ( A \cap E ^ { \mathrm { c } } )$ hence by Theorem 2.5 we have 

$$
m ^ {*} (A) \leq m ^ {*} (A \cap E) + m ^ {*} (A \cap E ^ {\mathrm{c}})
$$

for any A and E. So our future task of verifying (2.6) has simplified: $E \in { \mathcal { M } }$ if and only if the following inequality holds 

$$
m ^ {*} (A) \geq m ^ {*} (A \cap E) + m ^ {*} (A \cap E ^ {\mathrm{c}}) \text {   for   all   } A \subseteq \mathbb {R}.\tag{2.7}
$$

Now we give some examples of measurable sets. 

## Theorem 2.7

(i) Any null set is measurable. 

(ii) Any interval is measurable. 

## Proof

(i) If N is a null set, then (Proposition 2.2) $m ^ { * } ( N ) = 0$ . So for any $A \subset \mathbb { R }$ we have 

$$
m ^ {*} (A \cap N) \leq m ^ {*} (N) = 0 \quad \text { since } A \cap N \subseteq N
$$

$$
m ^ {*} (A \cap N ^ {c}) \leq m ^ {*} (A) \quad \text { since } A \cap N ^ {c} \subseteq A
$$

and adding together we have proved (2.7). 

(ii) Let $E = I$ be an interval. Suppose, for example, that $I = [ a , b ]$ . Take any $A \subseteq \mathbb { R }$ and $\varepsilon > 0$ . Find a covering of A with 

$$
m ^ {*} (A) \leq \sum_ {n = 1} ^ {\infty} l \left(I _ {n}\right) \leq m ^ {*} (A) + \varepsilon .
$$

Clearly the intervals $I _ { n } ^ { \prime } = I _ { n } \cap [ a , b ]$ cover $A \cap [ a , b ]$ hence 

$$
m ^ {*} (A \cap [ a, b ]) \leq \sum_ {n = 1} ^ {\infty} l \left(I _ {n} ^ {\prime}\right).
$$

The intervals $I _ { n } ^ { \prime \prime } = I _ { n } \cap ( - \infty , a ) , I _ { n } ^ { \prime \prime \prime } = I _ { n } \cap ( b , + \infty )$ cover $A \cap [ a , b ] ^ { \mathrm { c } }$ so 

$$
m ^ {*} (A \cap [ a, b ] ^ {\mathrm{c}}) \leq \sum_ {n = 1} ^ {\infty} l (I _ {n} ^ {\prime \prime}) + \sum_ {n = 1} ^ {\infty} l (I _ {n} ^ {\prime \prime \prime}).
$$

Putting the above three inequalities together we obtain (2.7). 

If I is unbounded, $I = [ a , \infty )$ say, then the proof is even simpler since it is suficient to consider ${ \cal I } _ { n } ^ { \prime } = I _ { n } \cap [ a , \infty )$ and $I _ { n } ^ { \prime \prime } = I _ { n } \cap ( - \infty , a )$ □ 

The fundamental properties of the class  of all Lebesgue-measurable subsets of R can now be proved. They fall into two categories: first we show that <sup>certain</sup> <sup>set</sup> <sup>operations</sup> <sup>on</sup> <sup>sets</sup> <sup>in</sup> M <sup>again</sup> <sup>produce</sup> <sup>sets</sup> <sup>in</sup> $\mathcal { M }$ (these are what we call ‘closure properties’) and second we prove that for sets in  the outer measure $m ^ { * }$ has the property of countable additivity announced above. 

Theorem 2.8 

(i) $\mathbb { R } \in { \mathcal { M } }$ 

(ii) if $E \in { \mathcal { M } }$ then $E ^ { \mathrm { c } } \in \mathcal { M }$ ， 

(iii) if $E _ { n } \in { \mathcal { M } }$ for all $n = 1 , 2 , \dots$ . then $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n } \in { \mathcal { M } }$ 

Moreover, if $E _ { n } \in { \mathcal { M } } , n = 1 , 2 , . .$ . and $E _ { j } \cap E _ { k } = \emptyset$ for $j \neq k$ , then 

$$
m ^ {*} \big (\bigcup_ {n = 1} ^ {\infty} E _ {n} \big) = \sum_ {n = 1} ^ {\infty} m ^ {*} (E _ {n}).\tag{2.8}
$$

## Remark 2.1

This result is the most important theorem in this chapter and provides the basis for all that follows. It also allows us to give names to the quantities under discussion. 

Conditions (i)–(iii) mean that  is a $\sigma { - } f i e l d .$ In other words, we say that a family of sets is a σ-field if it contains the base set and is closed under complements and countable unions. A [0, ]-valued function defined on a $\sigma -$ field is called a measure if it satisfies (2.8) for pairwise disjoint sets, i.e. it is countably additive. 

An alternative, rather more abstract and general, approach to measure theory is to begin with the above properties as axioms, i.e. to call a triple $( \varOmega , \mathcal { F } , \mu )$ a measure space if $\varOmega$ is an abstractly given set, $\mathcal { F }$ is a $\sigma { - } \mathrm { f i e l d }$ of subsets of $\varOmega$ and $\mu : { \mathcal { F } } \mapsto [ 0 , \infty ]$ is a function satisfying (2.8) (with $\mu$ instead of $m ^ { * } )$ . The task of defining Lebesgue measure on R then becomes that of verifying, with $\mathcal { M }$ and $m = m ^ { * }$ on $\mathcal { M }$ defined as above, that the triple $( \mathbb { R } , \mathcal { M } , m )$ satisfies these axioms, i.e. becomes a measure space. 

Although the requirements of probability theory will mean that we have to consider such general measure spaces in due course, we have chosen our more concrete approach to the fundamental example of Lebesgue measure in order to demonstrate how this important measure space arises quite naturally from considerations of the ‘lengths’ of sets in $\mathbb { R } ,$ , and leads to a theory of integration which greatly extends that of Riemann. It is also suficient to allow us to develop most of the important examples of probability distributions. 

Proof (of the Theorem) 

(i) Let $A \subseteq \mathbb { R }$ . Note that $A \cap \mathbb { R } = A , \mathbb { R ^ { c } } = \emptyset$ , so that $A \cap \mathbb { R } ^ { \mathrm { c } } = \emptyset$ . Now (2.6) reads $m ^ { * } ( A ) = m ^ { * } ( A ) + m ^ { * } ( \emptyset )$ and is of course true since $m ^ { * } ( \varnothing ) = 0$ 

(ii) Suppose $E \in { \mathcal { M } }$ and take any $A \subseteq \mathbb { R }$ . We have to show (2.6) for $E ^ { \mathrm { c } }$ , i.e. 

$$
m ^ {*} (A) = m ^ {*} \left(A \cap E ^ {\mathrm{c}}\right) + m ^ {*} \left(A \cap \left(E ^ {\mathrm{c}}\right) ^ {\mathrm{c}}\right)
$$

but since $( E ^ { \mathrm { c } } ) ^ { \mathrm { c } } = E$ this reduces to the condition for $E$ which holds by hypothesis. 

We split the proof of (iii) into several steps. But first: 

A warm up. Suppose that $E _ { 1 } \cap E _ { 2 } = \emptyset , E _ { 1 } , E _ { 2 } \in \mathcal { M }$ . We shall show that $E _ { 1 } \cup E _ { 2 } \in { \mathcal { M } }$ and $m ^ { * } ( E _ { 1 } \cup E _ { 2 } ) = m ^ { * } ( E _ { 1 } ) + m ^ { * } ( E _ { 2 } )$ 

Let $A \subseteq \mathbb { R }$ . We have the condition for $E _ { 1 }$ : 

$$
m ^ {*} (A) = m ^ {*} (A \cap E _ {1}) + m ^ {*} (A \cap E _ {1} ^ {\mathrm{c}}).\tag{2.9}
$$

Now, apply (2.6) for $E _ { 2 }$ with $A \cap E _ { 1 } ^ { \mathrm { { c } } }$ in place of A: 

$$
\begin{array}{c} m ^ {*} (A \cap E _ {1} ^ {\mathrm{c}}) = m ^ {*} ((A \cap E _ {1} ^ {\mathrm{c}}) \cap E _ {2}) + m ^ {*} ((A \cap E _ {1} ^ {\mathrm{c}}) \cap E _ {2} ^ {\mathrm{c}}). \\ = m ^ {*} (A \cap (E _ {1} ^ {\mathrm{c}} \cap E _ {2})) + m ^ {*} (A \cap (E _ {1} ^ {\mathrm{c}} \cap E _ {2} ^ {\mathrm{c}})) \end{array}
$$

(the situation is depicted in Figure 2.2). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/e93df8c2bdff20b4a7441318a96196db07bc0adafc8228849fbe3e56fbcca721.jpg)



Figure 2.2 The sets A, $E _ { 1 }$ , $E _ { 2 }$


Since $E _ { 1 }$ and $E _ { 2 }$ are disjoint, $E _ { 1 } ^ { \mathrm { c } } \cap E _ { 2 } = E _ { 2 }$ . By de Morgan’s law $E _ { 1 } ^ { \mathrm { c } } \cap E _ { 2 } ^ { \mathrm { c } } =$ $( E _ { 1 } \cup E _ { 2 } ) ^ { \mathrm { c } }$ . We substitute and we have 

$$
m ^ {*} (A \cap E _ {1} ^ {c}) = m ^ {*} (A \cap E _ {2}) + m ^ {*} (A \cap (E _ {1} \cup E _ {2}) ^ {c}).
$$

Substituting this into (2.9) we get 

$$
m ^ {*} (A) = m ^ {*} \left(A \cap E _ {1}\right) + m ^ {*} \left(A \cap E _ {2}\right) + m ^ {*} \left(A \cap \left(E _ {1} \cup E _ {2}\right) ^ {\mathrm{c}}\right).\tag{2.10}
$$

Now by the subadditivity property of $m ^ { * }$ we have 

$$
\begin{array}{c} m ^ {*} (A \cap E _ {1}) + m ^ {*} (A \cap E _ {2}) \geq m ^ {*} \big ((A \cap E _ {1}) \cup (A \cap E _ {2}) \big) \\ = m ^ {*} (A \cap (E _ {1} \cup E _ {2})) \end{array}
$$

so (2.10) gives 

$$
m ^ {*} (A) \geq m ^ {*} (A \cap (E _ {1} \cup E _ {2})) + m ^ {*} (A \cap (E _ {1} \cup E _ {2}) ^ {c})
$$

which is suficient for $E _ { 1 } \cup E _ { 2 }$ to belong to  (the inverse inequality is always true, as observed before (2.7)). 

Finally, put $A = E _ { 1 } \cup E _ { 2 }$ in (2.10) to get $m ^ { * } ( E _ { 1 } \cup E _ { 2 } ) = m ^ { * } ( E _ { 1 } ) + m ^ { * } ( E _ { 2 } )$ 2which completes the argument. 口

We return to the proof of the theorem. 

## Proof

Step 1. If pairwise disjoint $E _ { k } , k = 1 , 2 , \ldots$ , are in  then their union is in and (2.8) holds. 

We begin as in the proof of Warm up and we have 

$$
m ^ {*} (A) = m ^ {*} \left(A \cap E _ {1}\right) + m ^ {*} \left(A \cap E _ {1} ^ {\mathrm{c}}\right)
$$

$$
m ^ {*} (A) = m ^ {*} \left(A \cap E _ {1}\right) + m ^ {*} \left(A \cap E _ {2}\right) + m ^ {*} \left(A \cap \left(E _ {1} \cup E _ {2}\right) ^ {\mathrm{c}}\right)
$$

(see (2.10)) and after n steps we expect 

$$
m ^ {*} (A) = \sum_ {k = 1} ^ {n} m ^ {*} \left(A \cap E _ {k}\right) + m ^ {*} \left(A \cap \left(\bigcup_ {k = 1} ^ {n} E _ {k}\right) ^ {c}\right).\tag{2.11}
$$

Let us demonstrate this by induction. The case $n = 1$ is the first line above. Suppose that 

$$
m ^ {*} (A) = \sum_ {k = 1} ^ {n - 1} m ^ {*} \left(A \cap E _ {k}\right) + m ^ {*} \left(A \cap \left(\bigcup_ {k = 1} ^ {n - 1} E _ {k}\right) ^ {c}\right).\tag{2.12}
$$

Since $E _ { n } \in { \mathcal { M } }$ , we may apply (2.6) with $A \cap \left( \bigcup _ { k = 1 } ^ { n - 1 } E _ { k } \right) ^ { \mathrm { { c } } }$ in place of A: 

$$
m ^ {*} (A \cap (\bigcup_ {k = 1} ^ {n - 1} E _ {k}) ^ {\mathrm{c}}) = m ^ {*} (A \cap (\bigcup_ {k = 1} ^ {n - 1} E _ {k}) ^ {\mathrm{c}} \cap E _ {n}) + m ^ {*} (A \cap (\bigcup_ {k = 1} ^ {n - 1} E _ {k}) ^ {\mathrm{c}} \cap E _ {n} ^ {\mathrm{c}}).\tag{2.13}
$$

Now we make the same observations as in the Warm up: 

$$
\big (\bigcup_ {k = 1} ^ {n - 1} E _ {k} \big) ^ {c} \cap E _ {n} = E _ {n} \quad (E _ {i} \text {   are   pairwise   disjoint }),
$$

$$
\big (\bigcup_ {k = 1} ^ {n - 1} E _ {k} \big) ^ {\mathrm{c}} \cap E _ {n} ^ {\mathrm{c}} = \big (\bigcup_ {k = 1} ^ {n} E _ {k} \big) ^ {\mathrm{c}} \quad (\text { by   de   Morgan's   law }).
$$

Inserting these into (2.13) we get 

$$
m ^ {*} (A \cap \big (\bigcup_ {k = 1} ^ {n - 1} E _ {k} \big) ^ {c}) = m ^ {*} (A \cap E _ {n}) + m ^ {*} (A \cap \big (\bigcup_ {k = 1} ^ {n} E _ {k} \big) ^ {c}),
$$

and inserting this into the induction hypothesis (2.12) we get 

$$
m ^ {*} (A) = \sum_ {k = 1} ^ {n - 1} m ^ {*} (A \cap E _ {k}) + m ^ {*} (A \cap E _ {n}) + m ^ {*} \left(A \cap \left(\bigcup_ {k = 1} ^ {n} E _ {k}\right) ^ {\mathrm{c}}\right)
$$

as required to complete the induction step. Thus (2.11) holds for all n by induction. 

As will be seen at the next step the fact that $E _ { k }$ are pairwise disjoint is not necessary in order to ensure that their union belongs to $\mathcal { M } .$ . However, with this assumption we have equality in (2.11) which does not hold otherwise. This equality will allow us to prove countable additivity (2.8). 

Since 

$$
\Bigl (\bigcup_ {k = 1} ^ {n} E _ {k} \Bigr) ^ {\mathrm{c}} \supseteq \Bigl (\bigcup_ {k = 1} ^ {\infty} E _ {k} \Bigr) ^ {\mathrm{c}},
$$

from (2.11) by monotonicity (Proposition 2.3) we get 

$$
m ^ {*} (A) \geq \sum_ {k = 1} ^ {n} m ^ {*} \left(A \cap E _ {k}\right) + m ^ {*} \left(A \cap \left(\bigcup_ {k = 1} ^ {\infty} E _ {k}\right) ^ {c}\right).
$$

The inequality remains true after we pass to the limit $n  \infty { : }$ 

$$
m ^ {*} (A) \geq \sum_ {k = 1} ^ {\infty} m ^ {*} \left(A \cap E _ {k}\right) + m ^ {*} \left(A \cap \left(\bigcup_ {k = 1} ^ {\infty} E _ {k}\right) ^ {c}\right).\tag{2.14}
$$

By countable subadditivity (Theorem 2.5) 

$$
\sum_ {k = 1} ^ {\infty} m ^ {*} (A \cap E _ {k}) \geq m ^ {*} \left(A \cap \bigcup_ {k = 1} ^ {\infty} E _ {k}\right)
$$

and so 

$$
m ^ {*} (A) \geq m ^ {*} \left(A \cap \bigcup_ {k = 1} ^ {\infty} E _ {k}\right) + m ^ {*} \left(A \cap \left(\bigcup_ {k = 1} ^ {\infty} E _ {k}\right) ^ {c}\right)\tag{2.15}
$$

as required. So we have shown that $\textstyle \bigcup _ { k = 1 } ^ { \infty } E _ { k } \in { \mathcal { M } }$ and hence the two sides of S(2.15) are equal. The right hand side of (2.14) is squeezed between the left and right of (2.15) which yields 

$$
m ^ {*} (A) = \sum_ {k = 1} ^ {\infty} m ^ {*} \left(A \cap E _ {k}\right) + m ^ {*} \left(A \cap \left(\bigcup_ {k = 1} ^ {\infty} E _ {k}\right) ^ {c}\right).\tag{2.16}
$$

The equality here is a consequence of the assumption that $E _ { k }$ are pairwise disjoint. It holds for any set $A$ so we may insert $A = \textstyle \bigcup _ { i = 1 } ^ { \infty } E _ { j }$ . The last term on the right is zero because we have $m ^ { * } ( \varnothing )$ . Next $( \bigcup _ { i = 1 } ^ { \infty } E _ { j } ) \cap E _ { n } = E _ { n }$ and so we have (2.8). 

Step 2. If $E _ { 1 } , E _ { 2 } \in \mathcal { M }$ , then $E _ { 1 } \cup E _ { 2 } \in { \mathcal { M } }$ (not necessarily disjoint). 

Again we begin as in the Warm up: 

$$
m ^ {*} (A) = m ^ {*} \left(A \cap E _ {1}\right) + m ^ {*} \left(A \cap E _ {1} ^ {\mathrm{c}}\right).\tag{2.17}
$$

Next, applying (2.6) to $E _ { 2 }$ with $A \cap E _ { 1 } ^ { \mathrm { c } }$ in place of A we get 

$$
m ^ {*} (A \cap E _ {1} ^ {\mathrm{c}}) = m ^ {*} (A \cap E _ {1} ^ {\mathrm{c}} \cap E _ {2}) + m ^ {*} (A \cap E _ {1} ^ {\mathrm{c}} \cap E _ {2} ^ {\mathrm{c}}).
$$

We insert this into (2.17) to get 

$$
m ^ {*} (A) = m ^ {*} \left(A \cap E _ {1}\right) + m ^ {*} \left(A \cap E _ {1} ^ {c} \cap E _ {2}\right) + m ^ {*} \left(A \cap E _ {1} ^ {c} \cap E _ {2} ^ {c}\right).\tag{2.18}
$$

By de Morgan’s law, $E _ { 1 } ^ { \mathrm { c } } \cap E _ { 2 } ^ { \mathrm { c } } = ( E _ { 1 } \cup E _ { 2 } ) ^ { \mathrm { c } }$ so (as before) 

$$
m ^ {*} (A \cap E _ {1} ^ {\mathrm{c}} \cap E _ {2} ^ {\mathrm{c}}) = m ^ {*} (A \cap (E _ {1} \cup E _ {2}) ^ {\mathrm{c}}).\tag{2.19}
$$

By subadditivity of $m ^ { * }$ we have 

$$
m ^ {*} (A \cap E _ {1}) + m ^ {*} (A \cap E _ {1} ^ {\mathrm{c}} \cap E _ {2}) \geq m ^ {*} (A \cap (E _ {1} \cup E _ {2})).\tag{2.20}
$$

Inserting (2.19) and (2.20) into (2.18) we get 

$$
m ^ {*} (A) \geq m ^ {*} (A \cap (E _ {1} \cup E _ {2})) + m ^ {*} (A \cap (E _ {1} \cup E _ {2}) ^ {c})
$$

as required. 

Step 3. If $E _ { k } \in { \mathcal { M } } , k = 1 , . . . , n$ , then $E _ { 1 } \cup \dots \cup E _ { n } \in { \mathcal { M } }$ (not necessarily disjoint). 

We argue by induction. There is nothing to prove for $n = 1$ . Suppose the claim is true for $n - 1$ . Then 

$$
E _ {1} \cup \dots \cup E _ {n} = (E _ {1} \cup \dots \cup E _ {n - 1}) \cup E _ {n}
$$

so that the result follows from Step 2. 

Step 4. If $E _ { 1 } , E _ { 2 } \in \mathcal { M }$ , then $E _ { 1 } \cap E _ { 2 } \in { \mathcal { M } }$ 

We have $E _ { 1 } ^ { \mathrm { c } } , E _ { 2 } ^ { \mathrm { c } } \in \mathcal { M }$ by (ii), $E _ { 1 } ^ { \mathrm { c } } \cup E _ { 2 } ^ { \mathrm { c } } \in { \mathcal { M } }$ by Step 2, $( E _ { 1 } ^ { \mathrm { c } } \cup E _ { 2 } ^ { \mathrm { c } } ) ^ { \mathrm { c } } \in \mathcal { M }$ by (ii) again, but by de Morgan’s law the last set is equal to $E _ { 1 } \cap E _ { 2 }$ 

Step 5. The general case: if $E _ { 1 } , E _ { 2 } , \ldots$ are in , then so is $\textstyle \bigcup _ { k = 1 } ^ { \infty } E _ { k }$ 

Let $E _ { k } \in \mathcal { M } , k = 1 , 2 , . . . .$ . We define an auxiliary sequence of pairwise disjoint sets $F _ { k }$ with the same union as $E _ { k }$ : 

$$
\begin{array}{l} F _ {1} = E _ {1} \\ F _ {2} = E _ {2} \backslash E _ {1} = E _ {2} \cap E _ {1} ^ {\mathrm{c}} \\ F _ {3} = E _ {3} \backslash (E _ {1} \cup E _ {2}) = E _ {3} \cap (E _ {1} \cup E _ {2}) ^ {\mathrm{c}} \end{array}
$$

$$
F _ {k} = E _ {k} \backslash (E _ {1} \cup \dots \cup E _ {k - 1}) = E _ {k} \cap (E _ {1} \cup \dots \cup E _ {k - 1}) ^ {c},
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/34014208e1e5059ff94754d94c548229c6e6fcbf8a708fdc499ed0da08f01903.jpg)



Figure 2.3 The sets $F _ { k }$


see Figure 2.3. 

By Steps 3 and 4 we know that all $F _ { k }$ are in . By the very construction they are pairwise disjoint so by Step 1 their union is in . We shall show that 

$$
\bigcup_ {k = 1} ^ {\infty} F _ {k} = \bigcup_ {k = 1} ^ {\infty} E _ {k}.
$$

This will complete the proof since the latter is now in . The inclusion 

$$
\bigcup_ {k = 1} ^ {\infty} F _ {k} \subseteq \bigcup_ {k = 1} ^ {\infty} E _ {k}
$$

is obvious since for each k, $F _ { k } \subseteq E _ { k }$ by definition. For the inverse let $a \in$ $\bigcup _ { k = 1 } ^ { \infty } E _ { k } . \mathrm { \ : P u t \ : } S = \{ n \in \mathbb { N } : a \in E _ { n } \}$ which is non-empty since a belongs to the union. Let n = min $S \in S$ . If $n _ { 0 } = 1$ , then $a \in E _ { 1 } = F _ { 1 }$ . Suppose $n _ { 0 } > 1$ . So $a \in E _ { n _ { 0 } }$ and, by the definition of $n _ { 0 }$ , a / $E _ { 1 } , \dots , a \notin E _ { n _ { 0 } - 1 }$ . By the definition of $F _ { n _ { 0 } }$ this means that $a \in F _ { n _ { 0 } }$ so a is in $\textstyle \bigcup _ { k = 1 } ^ { \infty } F _ { k }$ □ 

Using de Morgan’s laws you should easily verify an additional property of . 

Proposition 2.9 

If $E _ { k } \in \mathcal { M } , k = 1 , 2 , . . . ,$ then 

$$
E = \bigcap_ {k = 1} ^ {\infty} E _ {k} \in \mathcal {M}.
$$

We can therefore summarize the properties of the family of Lebesgue measurable sets as follows: 

1. is closed under countable unions, countable intersections, and complements. It contains intervals and all null sets. 

## Definition 2.4

We shall write $m ( E )$ instead of $m ^ { * } ( E )$ for any E in and call $m ( E )$ the Lebesgue measure of the set E. 

Thus Theorems 2.8 and 2.4 now read as follows, and describe the construction which we have laboured so hard to establish: 

1. Lebesgue measure m $: \mathcal { M }  [ 0 , \infty ]$ is a countably additive set function defined on the σ-field of measurable sets. Lebesgue measure of an interval is equal to its length. Lebesgue measure of a null set is zero. 

## 2.4 Basic properties of Lebesgue measure

Since Lebesgue measure is nothing else than the outer measure restricted to a special class of sets, some properties of the outer measure are automatically inherited by Lebesgue measure: 

Proposition 2.10 

Suppose that $A , B \in { \mathcal { M } }$ 

(i) If $A \subset B$ then $m ( A ) \leq m ( B )$ 

(ii) If $A \subset B$ and $m ( A )$ is finite then $m ( B \setminus A ) = m ( B ) - m ( A )$ 

(iii) m is translation invariant. 

Since $\emptyset \in { \mathcal { M } }$ we can take $E _ { i } = \mathcal { O }$ for all $i > n$ in (2.8) to conclude that Lebesgue measure is additive: if $E _ { i } \in \mathcal { M }$ are pairwise disjoint, then 

$$
m (\bigcup_ {i = 1} ^ {n} E _ {i}) = \sum_ {i = 1} ^ {n} m (E _ {i}).
$$

## Exercise 2.6

Find a formula describing $m ( A \cup B )$ and $m ( A \cup B \cup C )$ in terms of measures of the individual sets and their intersections (we do not assume that the sets are pairwise disjoint). 

Recalling that the symmetric diference $A \varDelta B$ of two sets is defined by $A \varDelta B = ( A \setminus B ) \cup ( B \setminus A )$ the following result is also easy to check: 

## Proposition 2.11

If A , m(A∆B) = 0, then B and $m ( A ) = m ( B )$ 

Hint Recall that null sets belong to and that subsets of null sets are null. 

As we noted in Chapter 1, every open set in R can be expressed as the union of a countable number of open intervals. This ensures that open sets in R are Lebesgue-measurable, since  contains intervals and is closed under countable unions. We can approximate the Lebesgue measure of any $A \in { \mathcal { M } }$ from above by the measures of a sequence of open sets containing A. This is clear from the following result: 

## Theorem 2.12

(i) For any $\varepsilon > 0 , A \subset \mathbb { R }$ we can find an open set O such that 

$$
A \subset O, \qquad m (O) \leq m ^ {*} (A) + \varepsilon .
$$

Consequently, for any $E \in { \mathcal { M } }$ we can find an open set O containing E such that $m ( O \setminus E ) < \varepsilon$ 

(ii) For any $A \subset \mathbb { R }$ we can find a sequence of open sets $O _ { n }$ such that 

$$
A \subset \bigcap_ {n} O _ {n}, \qquad m (\bigcap_ {n} O _ {n}) = m ^ {*} (A).
$$

## Proof

(i) By definition of $m ^ { * } ( A )$ we can find a sequence $\left( I _ { n } \right)$ of intervals with $A \subset$ $\textstyle \bigcup _ { n } I _ { n }$ and $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } l ( I _ { n } ) - \frac { \varepsilon } { 2 } \leq m ^ { * } ( A ) } \end{array}$ . Each $I _ { n }$ is contained in an open interval S Pwhose length is very close to that of $I _ { n } ;$ ; if the left and right endpoints of $I _ { n }$ are $a _ { n }$ and $b _ { n }$ respectively let $\begin{array} { r } { J _ { n } = ( a _ { n } - \frac { \varepsilon } { 2 ^ { n + 2 } } , b _ { n } + \frac { \varepsilon } { 2 ^ { n + 2 } } ) } \end{array}$ . Set $O = \textstyle \bigcup _ { n } J _ { n }$ , which is open. Then $A \subset O$ and 

$$
m (O) \leq \sum_ {n = 1} ^ {\infty} l (J _ {n}) \leq \sum_ {n = 1} ^ {\infty} l (I _ {n}) + \frac {\varepsilon}{2} \leq m ^ {*} (A) + \varepsilon .
$$

When $m ( E ) < \infty$ the final statement follows at once from (ii) in Proposition 2.10, since then $m ( O \setminus E ) = m ( O ) - m ( E ) \leq \varepsilon .$ . When $m ( E ) = \infty$ we first write R as a countable union of finite intervals: $\mathbb { R } = \bigcup _ { n } ( - n , n )$ . Now 

$E _ { n } = E \cap ( - n , n )$ has finite measure, so we can find an open $O _ { n } \supset E _ { n }$ with $m ( O _ { n } \setminus E _ { n } ) \leq \frac { \varepsilon } { 2 ^ { n } }$ . The set $\textstyle O = \bigcup _ { n } O _ { n }$ is open and contains E. Now 

$$
O \setminus E = (\bigcup_ {n} O _ {n}) \setminus (\bigcup_ {n} E _ {n}) \subset \bigcup_ {n} (O _ {n} \setminus E _ {n})
$$

so that $\begin{array} { r } { m ( O \setminus E ) \leq \sum _ { n } m ( O _ { n } \setminus E _ { n } ) \leq \varepsilon } \end{array}$ as required. 

(ii) In (i) use $\textstyle { \varepsilon = { \frac { 1 } { n } } }$ and let $O _ { n }$ be the open set so obtained. With $\textstyle E = \bigcap _ { n } O _ { n }$ we obtain a measurable set containing A such that $m ( E ) < m ( O _ { n } ) \leq m ^ { * } ( A ) + \frac { 1 } { n }$ for each n, hence the result follows. □ 

## Remark 2.2

Theorem 2.12 shows how the freedom of movement allowed by the closure properties of the σ-field  can be exploited by producing, for any set $A \subset$ R, a measurable set $O \supset A$ which is obtained from open intervals with two operations (countable unions followed by countable intersections) and whose measure equals the outer measure of A. 

Finally we show that monotone sequences of measurable sets behave as one would expect with respect to m. 

## Theorem 2.13

Suppose that $A _ { n } \in { \mathcal { M } }$ for all $n \geq 1$ . Then we have: 

(i) if $A _ { n } \subset A _ { n + 1 }$ for all n, then 

$$
m (\bigcup_ {n} A _ {n}) = \lim _ {n \to \infty} m (A _ {n}),
$$

(ii) if $A _ { n } \supset A _ { n + 1 }$ for all n and $m ( A _ { 1 } ) < \infty$ , then 

$$
m (\bigcap_ {n} A _ {n}) = \lim _ {n \to \infty} m (A _ {n}).
$$

Proof 

(i) Let $B _ { 1 } = A _ { 1 } , B _ { i } = A _ { i } - A _ { i - 1 }$ for $i > 1$ . Then $\textstyle \bigcup _ { i = 1 } ^ { \infty } B _ { i } = \bigcup _ { i = 1 } ^ { \infty } A _ { i }$ and the $B _ { i } \in \mathcal { M }$ are pairwise disjoint, so that 

$$
\begin{array}{l} m (\bigcup_ {i} A _ {i}) = m (\bigcup_ {i} B _ {i}) \\ \qquad = \sum_ {i = 1} ^ {\infty} m (B _ {i}) \quad \text {(by countable additivity)} \\ \qquad = \lim _ {n \to \infty} \sum_ {i = 1} ^ {n} m (B _ {i}) \\ \qquad = \lim _ {n \to \infty} m (\bigcup_ {n = 1} ^ {n} B _ {i}) \quad \text {(by additivity)} \\ \qquad = \lim _ {n \to \infty} m (A _ {n}), \end{array}
$$

since $\textstyle A _ { n } = \bigcup _ { i = 1 } ^ { n } B _ { i }$ by construction – see Figure 2.4. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/e07351e90fb7b4869ec51c8ce95a99711a79c6964d973cce076d98d89d69bb48.jpg)



Figure 2.4 Sets $A _ { n } , B _ { n }$


(ii) $A _ { 1 } \setminus A _ { 1 } = \emptyset \subset A _ { 1 } \setminus A _ { 2 } \subset . . . \subset A _ { 1 } \setminus A _ { n } \subset . .$ . for all $n _ { \mathrm { : } }$ , so that by (i) 

$$
m (\bigcup_ {n} (A _ {1} \setminus A _ {n})) = \lim _ {n \to \infty} m (A _ {1} \setminus A _ {n})
$$

and since $m ( A _ { 1 } )$ is finite, $m ( A _ { 1 } \setminus A _ { n } ) = m ( A _ { 1 } ) - m ( A _ { n } )$ . On the other hand, $\begin{array} { r } { \bigcup _ { n } ( A _ { 1 } \setminus A _ { n } ) = A _ { 1 } \setminus \bigcap _ { n } A _ { n } } \end{array}$ , so that 

$$
m (\bigcup_ {n} (A _ {1} \setminus A _ {n})) = m (A _ {1}) - m (\bigcap_ {n} A _ {n}) = m (A _ {1}) - \lim _ {n \to \infty} m (A _ {n}).
$$

The result follows. 

## Remark 2.3

The proof of Theorem 2.13 simply relies on the countable additivity of m and on the definition of the sum of a series in $[ 0 , \infty ]$ , i.e. that 

$$
\sum_ {i = 1} ^ {\infty} m (A _ {i}) = \lim _ {n \to \infty} \sum_ {i = 1} ^ {n} m (A _ {i}).
$$

Consequently the result is true, not only for the set function m we have constructed on $\mathcal { M } .$ , but for any countably additive set function defined on a σ-field. It also leads us to the following claim, which, though we consider it here only for m, actually characterizes countably additive set functions. 

## Theorem 2.14

The set function m satisfies: 

(i) m is finitely additive, i.e. for pairwise disjoint sets $\left( A _ { i } \right)$ we have 

$$
m (\bigcup_ {i = 1} ^ {n} A _ {i}) = \sum_ {i = 1} ^ {n} m (A _ {i})
$$

for each n; 

(ii) m is continuous at Ø, i.e. if $\left( B _ { n } \right)$ decrease to $\mathrm { \ o }$ , then $m ( B _ { n } )$ decreases to 0. 

## Proof

To prove this claim, recall that $m : \mathcal { M } \mapsto [ 0 , \infty ]$ is countably additive. This implies (i), as we have already seen. To prove (ii), consider a sequence $\left( B _ { n } \right)$ in which decreases to Ø. Then $A _ { n } = B _ { n } \setminus B _ { n + 1 }$ defines a disjoint sequence in $\mathcal { M }$ , and $\textstyle \bigcup _ { n } A _ { n } = B _ { 1 }$ . We may assume that $B _ { 1 }$ is bounded, so that $m ( B _ { n } )$ is Sfinite for all n, so that, by Proposition 2.10 (ii), $m ( A _ { n } ) = m ( B _ { n } ) - m ( B _ { n + 1 } ) \geq 0$ and hence we have 

$$
\begin{array}{l} m (B _ {1}) = \sum_ {n = 1} ^ {\infty} m (A _ {n}) \\ \qquad = \lim _ {k \to \infty} \sum_ {n = 1} ^ {k} [ m (B _ {n}) - m (B _ {n + 1}) ] \\ \qquad = m (B _ {1}) - \lim _ {n \to \infty} m (B _ {n}) \end{array}
$$

which shows that $m ( B _ { n } ) \to 0$ , as required. 

## 2.5 Borel sets

The definition of does not easily lend itself to verification that a particular set belongs to ; in our proofs we have had to work quite hard to show that is closed under various operations. It is therefore useful to add another construction to our armoury; one which shows more directly how open sets (and indeed open intervals) and the structure of σ-fields lie at the heart of many of the concepts we have developed. 

We begin with an auxiliary construction enabling us to produce new σ-fields. 

## Theorem 2.15

The intersection of a family of σ-fields is a σ-field. 

## Proof

Let ${ \mathcal { F } } _ { \alpha }$ be σ-fields for $\alpha \in { \cal { A } }$ (the index set Λ can be arbitrary). Put 

$$
\mathcal {F} = \bigcap_ {\alpha \in \varLambda} \mathcal {F} _ {\alpha}.
$$

We verify the conditions of the definition. 

1. R $\in \mathcal { F } _ { \alpha }$ for all $\alpha \in { \cal { A } }$ so $\mathbb { R } \in \mathcal { F }$ 

2. If $E \in { \mathcal { F } }$ , then $E \in { \mathcal { F } } _ { \alpha }$ for all $\alpha \in { \cal { A } }$ . Since the ${ \mathcal { F } } _ { \alpha }$ are σ-fields, $E ^ { \mathrm { c } } \in \mathcal { F } _ { \alpha }$ and so $E ^ { \mathrm { c } } \in { \mathcal { F } }$ 

3. If $E _ { k } \in \mathcal { F }$ for $k = 1 , 2 , \ldots$ , then $E _ { k } \in \mathcal { F } _ { \alpha }$ , all $\alpha , k$ , hence $\textstyle \bigcup _ { k = 1 } ^ { \infty } E _ { k } \in { \mathcal { F } } _ { \alpha }$ 2 all α, and so $\textstyle \bigcup _ { k = 1 } ^ { \infty } E _ { k } \in { \mathcal { F } }$ □ 

## Definition 2.5

Put 

$$
\mathcal {B} = \bigcap \{\mathcal {F}: \mathcal {F} \text {   is   a   } \sigma \text {-field   containing   all   intervals } \}.
$$

We say that is the σ-field generated by all intervals and we call the elements of Borel sets (after Emile Borel 1871–1956). It is obviously the smallest $\sigma -$ field containing all intervals. In general, we say that $\mathcal { G }$ is the σ-field generated by a family of sets if $\mathcal { G } = \cap \{ \mathcal { F } : \mathcal { F }$ is a σ-field such that ${ \mathcal { F } } \supset A \}$ 

## Example 2.1

(Borel sets) The following examples illustrate how the closure properties of the σ-field  may be used to verify that most familiar sets in R belong to . 

(i) By construction, all intervals belong to $B ,$ and since $\boldsymbol { B }$ is a $\sigma { - } \mathrm { f i e l d }$ , all open sets must belong to $B { \mathrm { . } }$ as any open set is a countable union of (open) intervals. 

(ii) Countable sets are Borel sets, since each is a countable union of closed intervals of the form $[ a , a ]$ ; in particular N and $\mathbb { Q }$ are Borel sets. Hence, as the complement of a Borel set, the set of irrational numbers is also Borel. Similarly, finite and cofinite sets are Borel sets. 

The definition of is also very flexible – as long as we start with all intervals of a particular type, these collections generate the same Borel σ-field: 

## Theorem 2.16

If instead of the family of all intervals we take all open intervals, all closed intervals, all intervals of the form $( a , \infty )$ (or of the form $[ a , \infty ) , ( - \infty , b )$ , or $( - \infty , b ] )$ , all open sets, or all closed sets, then the σ-field generated by them is the same as $B _ { \cdot }$ 

## Proof

Consider for example the σ-field generated by the family of open intervals OI and denote it by $\mathcal { C } \mathrm { : }$ 

$$
\mathcal {C} = \bigcap \{\mathcal {F} \supset O I, \mathcal {F} \text {   is   a   } \sigma \text {-field} \}.
$$

We have to show that $\boldsymbol { B } = \boldsymbol { \mathcal { C } }$ . Since open intervals are intervals, $O I \subset I$ (the family of all intervals), then 

$$
\{\mathcal {F} \supset I \} \subset \{\mathcal {F} \supset O I \}
$$

i.e. the collection of all σ-fields $\mathcal { F }$ which contain I is smaller than the collection of all σ-fields which contain the smaller family OI, since it is a more demanding requirement to contain a bigger family, so there are fewer such objects. The inclusion is reversed after we take the intersection on both sides, thus $\mathcal { C } \subset B$ (the intersection of a smaller family is bigger, as the requirement of belonging to each of its members is a less stringent one). 

We shall show that contains all intervals. This will be suficient, since is the intersection of such σ-fields, so it is contained in each, so $B \subset { \mathcal { C } }$ 

To this end consider intervals [a, b), [a, b], (a, b] (the intervals of the form $( a , b )$ are in  by definition): 

$$
[ a, b) = \bigcap_ {n = 1} ^ {\infty} (a - \frac {1}{n}, b),
$$

$$
[ a, b ] = \bigcap_ {n = 1} ^ {\infty} (a - \frac {1}{n}, b + \frac {1}{n}),
$$

$$
(a, b ] = \bigcap_ {n = 1} ^ {\infty} (a, b + \frac {1}{n}).
$$

as a σ-field is closed with respect to countable intersection, so it contains the sets on the right. The argument for unbounded intervals is similar. The proof is complete. □ 

## Exercise 2.7

Show that the family of intervals of the form $( a , b ]$ also generates the σ-field of Borel sets. Show that the same is true for the family of all intervals $[ a , b )$ 

## Remark 2.4

Since is a σ-field containing all intervals, and is the smallest such σ-field, we have the inclusion $B \subset { \mathcal { M } }$ , i.e. every Borel set in R is Lebesgue-measurable. The question therefore arises whether these σ-fields might be the same. In fact the inclusion is proper. It is not altogether straightforward to construct a set in $\mathcal { M } \backslash \mathcal { B }$ , and we shall not attempt this here (but see the Appendix). However, by Theorem 2.12 (ii), given any $E \in { \mathcal { M } }$ we can find a Borel set $B \supset E$ of the form $B = \cap _ { n } O _ { n }$ , where the $( O _ { n } )$ are open sets, and such that $m ( E ) = m ( B )$ In particular, 

$$
m (B \Delta E) = m (B \setminus E) = 0.
$$

Hence m cannot distinguish between the measurable set E and the Borel set B we have constructed. 

Thus, given a Lebesgue-measurable set E we can find a Borel set B such that their symmetric diference $E \varDelta B$ is a null set. Now we know that $E \varDelta B \in \mathcal { M }$ 2 and it is obvious that subsets of null sets are also null, and hence in . However, we cannot conclude that every null set will be a Borel set (if did contain all null sets then by Theorem 2.12 (ii) we would have $B = { \mathcal { M } } )$ , and this points to an ‘incompleteness’ in $\boldsymbol { B }$ which explains why, even if we begin by defining m on intervals and then extend the definition to Borel sets, we would also need to extend it further in order to be able to identify precisely which sets are ‘negligible’ for our purposes. On the other hand, extension of the measure m to the σ-field will sufice, since $\mathcal { M }$ does contain all m-null sets and all subsets of null sets also belong to . 

We show that  is the smallest σ-field on R with this property, and we say that is the completion of relative to m and $( \mathbb { R } , \mathcal { M } , m )$ is complete (whereas the measure space (R, , m) is not complete). More precisely, a measure space $( X , { \mathcal { F } } , \mu )$ is complete if for all $F \in { \mathcal { F } }$ with $\mu ( F ) = 0$ , for all $N \subset F$ we have $N \in { \mathcal { F } }$ (and so $\mu ( N ) = 0 )$ 

The completion of a σ-field , relative to a given measure $\mu ,$ is defined as the smallest σ-field $\mathcal { F }$ containing $\mathcal { G }$ such that, if $N \subset G \in { \mathcal { G } }$ and $\mu ( G ) = 0$ 2 then $N \in \mathcal { F }$ 

## Proposition 2.17

The completion of $\mathcal { G }$ is of the form $\{ G \cup N : G \in { \mathcal { F } } , N \subset F \in { \mathcal { F } }$ with $\mu ( F ) =$ <sup>0</sup>}<sup>.</sup> 

This allows us to extend the measure µ uniquely to a measure $\bar { \mu }$ on $\mathcal { F }$ by setting ${ \bar { \mu } } ( G \cup N ) = \mu ( G )$ for $G \in { \mathcal { G } }$ 

## Theorem 2.18

is the completion of . 

## Proof

We show first that contains all subsets of null sets in : so let $N \subset B \in B$ B null, and suppose $A \subset \mathbb { R }$ . To show that $N \in \mathcal { M }$ we need to show that 

$$
m ^ {*} (A) \geq m ^ {*} (A \cap N) + m ^ {*} (A \cap N ^ {\mathrm{c}}).
$$

First note that $m ^ { * } ( A \cap N ) \leq m ^ { * } ( N ) \leq m ^ { * } ( B ) = 0$ . So it remains to show that $m ^ { * } ( A ) \geq m ^ { * } ( A \cap N ^ { \mathrm { c } } )$ but this follows at once from monotonicity of $m ^ { * }$ 

Thus we have shown that $N \in \mathcal { M }$ <sup>.</sup> <sup>Since</sup> M <sup>is</sup> <sup>a</sup> <sup>complete</sup> <sup>σ-field</sup> <sup>containing</sup> , this means that also contains the completion of . 

Finally, we show that is the minimal such σ-field, i.e. that ${ \mathcal { M } } \subset { \mathcal { C } } ;$ first consider $E \in { \mathcal { M } }$ with $m ^ { * } ( E ) < \infty$ , and choose $\begin{array} { r } { B = \bigcap _ { n } O _ { n } \in B } \end{array}$ as described above such that $B \supset E , m ( B ) = m ^ { * } ( E )$ T. (We reserve the use of m for sets in throughout this argument.) 

Consider $N = B \setminus E$ , which is in and has $m ^ { * } ( N ) = 0$ , since $m ^ { * }$ is additive on . By Theorem 2.12 (ii) we can find $L \supset N , L \in B$ and $m ( L ) = 0$ In other words, N is a subset of a null set in , and therefore $E = B \setminus N$ belongs to the completion of . For $E \in { \mathcal { M } }$ with $m ^ { * } ( E ) = \infty$ , apply the above to $E _ { n } = E \cap [ - n , n ]$ for each $n \in \mathbb { N }$ . Each $m ^ { * } ( E _ { n } )$ is finite, so the $E _ { n }$ all belong to $\mathcal { C }$ and hence so does their countable union E. Thus ${ \mathcal { M } } \subset { \mathcal { C } }$ and so they are equal. □ 

Despite these technical diferences, measurable sets are never far from ‘nice’ sets, and, in addition to approximations from above by open sets, as observed in Theorem 2.12, we can approximate the measure of any $E \in { \mathcal { M } }$ from below by those of closed subsets. 

## Theorem 2.19

If $E \in { \mathcal { M } }$ then for given $\varepsilon > 0$ there exists a closed set $F \subset E$ such that $m ( E \setminus F ) < \varepsilon$ . Hence there exists $B \subset E$ in the form $\textstyle B = \bigcup _ { n } F _ { n }$ , where all the $F _ { n }$ are closed sets, and $m ( E \setminus B ) = 0$ 

## Proof

The complement $E ^ { \mathrm { c } }$ is measurable and by Theorem 2.12 we can find an open set O containing $E ^ { \mathrm { c } }$ such that $m ( O \setminus E ^ { \mathrm { c } } ) \leq \varepsilon$ . But $O \setminus E ^ { \mathrm { c } } = O \cap E = E \setminus O ^ { \mathrm { c } }$ , and $F = O ^ { \mathrm { c } }$ is closed and contained in E. Hence this F is what we need. The final part is similar to Theorem 2.12 (ii), and the proof is left to the reader. 

## Exercise 2.8

Show that each of the following two statements is equivalent to saying that $E \in { \mathcal { M } }$ : 

(i) given $\varepsilon > 0$ there is an open set $O \supset E$ with $m ^ { * } ( O \setminus E ) < \varepsilon$ 2 

(ii) given $\varepsilon > 0$ there is a closed set $F \subset E$ with $m ^ { * } ( E \setminus F ) < \varepsilon$ 

## Remark 2.5

The two statements in the above Exercise are the key to a considerable generalization, linking the ideas of measure theory to those of topology: 

A non-negative countably additive set function $\mu$ defined on $\boldsymbol { B }$ is called a regular Borel measure if for every Borel set B we have: 

$$
\begin{array}{l} \mu (B) = \inf \{\mu (O): O \text { open,} O \supset B \}, \\ \mu (B) = \sup \{\mu (F): F \text { closed,} F \subset B \}. \end{array}
$$

In Theorems 2.12 and 2.19 we have verified these relations for Lebesgue measure. We shall consider other concrete examples of regular Borel measures later. 

## 2.6 Probability

The ideas which led to Lebesgue measure may be adapted to construct measures generally on arbitrary sets: any set $\varOmega$ carrying an outer measure (i.e. a mapping from $P ( \varOmega )$ to $[ 0 , \infty ]$ monotone and countably sub-additive) can be equipped with a measure $\mu$ defined on an appropriate σ-field $\mathcal { F }$ of its subsets. The resulting triple $( \varOmega , \mathcal { F } , \mu )$ is then called a measure space, as observed in Remark 2.1. Note that in the construction of Lebesgue measure we only used the properties, not the particular form of the outer measure. 

For the present, however, we shall be content with noting simply how to restrict Lebesgue measure to any Lebesgue measurable subset B of R with $m ( B ) > 0 ;$ 

Given Lebesgue measure m on the Lebesgue σ-field let 

$$
\mathcal {M} _ {B} = \{A \cap B: A \in \mathcal {M} \}
$$

and for $A \in \mathcal { M } _ { B }$ write 

$$
m _ {B} (A) = m (A).
$$

## Proposition 2.20

$\left( B , \mathcal { M } _ { B } , m _ { B } \right)$ is a complete measure space. 

$$
\text { Hint } \bigcup_ {i} (A _ {i} \cap B) = (\bigcup_ {i} A _ {i}) \cap B \text { and } (A _ {1} \cap B) \setminus (A _ {2} \cap B) = (A _ {1} \setminus A _ {2}) \cap B.
$$

We can finally state precisely what we mean by ‘selecting a number from $[ 0 , 1 ]$ at random’: restrict Lebesgue measure m to the interval $B = [ 0 , 1 ]$ and consider the $\sigma { - } \mathrm { f i e l d }$ of $\mathcal { M } _ { [ 0 , 1 ] }$ of measurable subsets of [0, 1]. Then $m _ { [ 0 , 1 ] }$ is a measure on $\mathcal { M } _ { [ 0 , 1 ] }$ with ‘total mass’ 1. Since all subintervals of $[ 0 , 1 ]$ with the same length have equal measure, the ‘mass’ of $m _ { [ 0 , 1 ] }$ is spread uniformly over $[ 0 , 1 ]$ , so that, for example, the ‘probability’ of choosing a number from $[ 0 , \frac { 1 } { 1 0 } )$ is the same as that of choosing a number from $[ \frac { 6 } { 1 0 } , \frac { 7 } { 1 0 } )$ , namely $\textstyle { \frac { 1 } { 1 0 } }$ . Thus all numerals are equally likely to appear as first digits of the decimal expansion of the chosen number. On the other hand, with this measure, the probability that the chosen number will be rational is 0, as is the probability of drawing an element of the Cantor set C. 

We now have the basis for some probability theory, although a general development still requires the extension of the concept of measure from R to abstract sets. Nonetheless the building blocks are already evident in the detailed development of the example of Lebesgue measure. The main idea in providing a mathematical foundation for probability theory is to use the concept of measure to provide the mathematical model of the intuitive notion of probability. The distinguishing feature of probability is the concept of independence, which we introduce below. We begin by defining the general framework. 

## 2.6.1 Probability space

## Definition 2.6

A probability space is a triple $( \varOmega , \mathcal { F } , P )$ where $\varOmega$ is an arbitrary set, $\mathcal { F }$ is a σ-field of subsets of $\varOmega .$ , and $P$ is a measure on $\mathcal { F }$ such that 

$$
P (\Omega) = 1,
$$

called probability measure or briefly probability. 

## Remark 2.6

The original definition, given by Kolmogorov in 1932, is a variant of the above (see Theorem 2.14): $( \varOmega , \mathcal { F } , P )$ is a probability space if $( \varOmega , \mathscr { F } )$ are given as above, and P is a finitely additive set function with $P ( \varnothing ) = 0$ and $P ( \varOmega ) = 1$ such that $P ( B _ { n } ) \setminus { 0 }$ whenever $\left( B _ { n } \right)$ in $\mathcal { F }$ decreases to Ø. 

## Example 2.2

We see at once that Lebesgue measure restricted to $[ 0 , 1 ]$ is a probability measure. More generally: suppose we are given an arbitrary Lebesgue measurable set $\Omega \subset \mathbb { R }$ , with $m ( \varOmega ) > 0$ . Then $P = c \cdot m _ { \varOmega }$ , where $\begin{array} { r } { c = \frac { 1 } { m ( \varOmega ) } } \end{array}$ , and $m = m _ { \varOmega }$ denotes the restriction of Lebesgue measure to measurable subsets of $\varOmega .$ , provides a probability measure on Ω, since P is complete and $P ( \varOmega ) = 1$ 

For example, if $\varOmega = [ a , b ]$ , we obtain $\begin{array} { r } { c = \frac { 1 } { b - a } } \end{array}$ , and $P$ becomes the ‘uniform distribution’ over $[ a , b ]$ . However, we can also use less familiar sets for our base space; for example, $\begin{array} { r } { \varOmega = [ a , b ] \cap ( \mathbb { R } \setminus \mathbb { Q } ) , c = \frac { 1 } { b - a } } \end{array}$ gives the same distribution over the irrationals in [a, b]. 

## 2.6.2 Events: conditioning and independence

The word ‘event’ is used to indicate that something is happening. In probability a typical event is to draw elements from a set and then the event is concerned with the outcome belonging to a particular subset. So, as described above, if $\varOmega = [ 0 , 1 ]$ we may be interested in the fact that a number drawn at random from [0, 1] belongs to some $A \subset [ 0 , 1 ]$ . We want to estimate the probability of this happening, and in the mathematical setup this is the number $P ( A )$ , here $m _ { [ 0 , 1 ] } ( A )$ . So it is natural to require that A should belong to $\mathcal { M } _ { [ 0 , 1 ] }$ , since these are the sets we may measure. By a slight abuse of the language, probabilists tend to identify the actual ‘event’ with the set A which features in the event. The next definition simply confirms this abuse of language. 

## Definition 2.7

Given a probability space $( \varOmega , \mathcal { F } , P )$ we say that the elements of $\mathcal { F }$ are events. 

Suppose next that a number has been drawn from [0, 1] but has not been revealed yet. We would like to bet on it being in $[ 0 , { \textstyle \frac { 1 } { 4 } } ]$ and we get a tip that it certainly belongs to $[ 0 , \textstyle { \frac { 1 } { 2 } } ]$ . Clearly, given this ‘inside information’, the probability of success is now $\textstyle { \frac { 1 } { 2 } }$ rather than $\textstyle { \frac { 1 } { 4 } }$ . This motivates the following general definition. 

## Definition 2.8

Suppose that $P ( B ) > 0$ . Then the number 

$$
P (A | B) = \frac {P (A \cap B)}{P (B)}
$$

is called the conditional probability of A given B. 

## Proposition 2.21

The mapping $A \mapsto P ( A | B )$ is countably additive on the σ-field $\mathcal { F } _ { B }$ 

Hint Use the fact that $A \mapsto P ( A \cap B )$ is countably additive on ${ \mathcal F } .$ 

A classical application of the conditional probability is the total probability formula which enables the computation of the probability of an event by means of conditional probabilities given some disjoint hypotheses: 

## Exercise 2.9

Prove that if $H _ { i }$ are pairwise disjoint events such that $\textstyle \bigcup _ { i = 1 } ^ { \infty } H _ { i } = \varOmega$ 8 $P ( H _ { i } ) \neq 0$ , then 

$$
P (A) = \sum_ {i = 1} ^ {\infty} P (A | H _ {i}) P (H _ {i}).
$$

It is natural to say that the event A is independent of B if the fact that B takes place has no influence on the chances of A, i.e. 

$$
P (A | B) = P (A).
$$

By definition of $P ( A | B )$ this immediately implies the relation 

$$
P (A \cap B) = P (A) \cdot P (B)
$$

which is usually taken as the definition of independence. The advantage of this practice is that we may dispose of the assumption $P ( B ) > 0$ 

## Definition 2.9

The events A, B are independent if 

$$
P (A \cap B) = P (A) \cdot P (B).
$$

Exercise 2.10 

Suppose that A and B are independent events. Show that $A ^ { c }$ and B are also independent. 

The Exercise indicates that if A and B are independent events, then all elements of the σ-fields they generate are mutually independent, since these $\sigma -$ fields are simply the collections $\mathcal { F } _ { A } = \{ \emptyset , A , A ^ { \mathrm { c } } , \Omega \}$ and $\mathcal { F } _ { B } = \{ \boldsymbol { \emptyset } , B , B ^ { \mathrm { c } } , \boldsymbol { \varOmega } \}$ respectively. This leads us to a natural extension of the definition: two σ-fields $\mathcal { F } _ { 1 }$ and $\mathcal { F } _ { 2 }$ are independent if for any choice of sets $A _ { 1 } \in { \mathcal { F } } _ { 1 }$ and $A _ { 2 } \in \mathcal { F } _ { 2 }$ we have $P ( A _ { 1 } \cap A _ { 2 } ) = P ( A _ { 1 } ) P ( A _ { 2 } )$ 

However, the extension of these definitions to three or more events (or several $\sigma { \mathrm { - f i e l d s } } )$ needs a little care, as the following simple examples show: 

## Example 2.3

Let $\begin{array} { r } { \varOmega = [ 0 , 1 ] , A = [ 0 , \frac { 1 } { 4 } ] } \end{array}$ as before; then A is independent of $\begin{array} { r } { B = \left[ \frac { 1 } { 8 } , \frac { 5 } { 8 } \right] } \end{array}$ and of $C = [ \textstyle { \frac { 1 } { 8 } } , \frac { 3 } { 8 } ] \cup [ \frac { 3 } { 4 } , 1 ]$ . In addition, B and C are independent. However, 

$$
P (A \cap B \cap C) \neq P (A) \cdot P (B) \cdot P (C).
$$

Thus, given three events, the pairwise independence of each of the three possible pairs does not sufice for the extension of ‘independence’ to all three events. 

On the other hand, with $\begin{array} { r } { A = [ 0 , \frac { 1 } { 4 } ] , B = C = [ 0 , \frac { 1 } { 1 6 } ] \cup [ \frac { 1 } { 4 } , \frac { 1 1 } { 1 6 } ] } \end{array}$ , (or alternatively with $C = [ 0 , \frac { 1 } { 1 6 } ] \cup [ \frac { 9 } { 1 6 } , 1 ] )$ 

$$
P (A \cap B \cap C) = P (A) \cdot P (B) \cdot P (C)\tag{2.21}
$$

but none of the pairs make independent events. 

This confirms further that we need to demand rather more if we wish to extend the above definition – pairwise independence is not enough, nor is (2.21); therefore we need to require both conditions to be satisfied together. Extending this to n events leads to: 

## Definition 2.10

The events $A _ { 1 } , \ldots , A _ { n }$ are independent if for all $k \leq n$ for each choice of k events, the probability of their intersection is the product of the probabilities. 

Again there is a powerful counterpart for σ-fields (which can be extended to sequences, and even arbitrary families): 

## Definition 2.11

The σ-fields $\mathcal { F } _ { 1 } , \mathcal { F } _ { 2 } , . . . , \mathcal { F } _ { n }$ defined on a given probability space $( \varOmega , \mathcal { F } , P )$ are independent if, for all choices of distinct indices $i _ { 1 } , i _ { 2 } , . . . , i _ { k }$ from $\{ 1 , 2 , . . . , n \}$ and all choices of sets $F _ { i _ { n } } \in \mathcal { F } _ { i _ { \tau } }$ we have 

$$
P (F _ {i _ {1}} \cap F _ {i _ {2}} \cap \ldots \cap F _ {i _ {k}}) = P (F _ {i _ {1}}) \cdot P (F _ {i _ {2}}) \cdot \dots \cdot P (F _ {i _ {k}}).
$$

The issue of independence will be revisited in the subsequent chapters where we develop some more tools to calculate probabilities 

## 2.6.3 Applications to mathematical finance

As indicated in the Preface, we will explore briefly how the ideas developed in each chapter can be applied in the rapidly growing field of mathematical finance. This is not intended as an introduction to this subject, but hopefully it will demonstrate how a consistent mathematical formulation can help to clarify ideas central to many disciplines. Readers who are unfamiliar with mathematical finance should consult texts such as [4], [5], [7] for definitions and a discussion of the main ideas of the subject. 

Probabilistic modelling in finance centres on the analysis of models for the evolution of the value of traded assets, such as stocks or bonds, and seeks to identify trends in their future behaviour. Much of the modern theory is concerned with evaluating derivative securities such as options, whose value is determined by the (random) future values of some underlying security, such as a stock. 

We illustrate the above probability ideas on a classical model of stock prices, namely the binomial tree. This model is based on finitely many time instants at which the prices may change, and the changes are of a very simple nature. Suppose that the number of steps is N, denote the price at the k-th step by $S ( k ) , 0 \leq k \leq N$ . At each step the stock price changes in the following way: the price at a given step is the price at the previous step multiplied by $U$ with probability p or D with probability $q = 1 - p$ , where $0 < D < U .$ Therefore the final price depends on the sequence ${ \boldsymbol \omega } = ( \omega _ { 1 } , \omega _ { 2 } , \ldots , \omega _ { N } )$ where $\omega _ { i } = 1$ indicates the application of the factor U or $\omega _ { i } = 0$ , which indicates application of the factor D. Such a sequence is called a path and we take $\varOmega$ to consist of all possible paths. In other words, 

$$
S (k) = S (0) \times \eta (1) \times \dots \times \eta (k),
$$

where 

$$
\eta (k) = \left\{ \begin{array}{l l} U \text {   with   probability   } p, \\ D \text {   with   probability   } q. \end{array} \right.
$$

## Exercise 2.11

Suppose $N = 5 , U = 1 . 2 , D = 0 . 9$ , and $S ( 0 ) = 5 0 0$ . Find the number of all paths. How many paths lead to the price $S ( 5 ) = 5 2 4 . 8 8 ?$ What is the probability that $S ( 5 ) > 9 0 0$ if the probability going up in a single step is 0.5? 

In general, the total number of paths is clearly $2 ^ { N }$ and at step k there are $k + 1$ possible prices. 

We construct a probability space by equipping Ω with the sigma field $2 ^ { \varOmega }$ of all subsets of $\varOmega .$ and the probability defined on single-element sets by $P ( \{ \omega \} ) =$ $p ^ { k } q ^ { n - k }$ , where $\begin{array} { r } { k = \sum _ { i = 1 } ^ { N } \omega _ { i } } \end{array}$ 

PAs time progresses we gather information about stock prices, or, what amounts to the same, about paths. This means, that having observed some prices the range of possible future developments is restricted. Our information increases with time and this idea can be captured by the following family of σ-fields. 

Fix $m < n$ and define a σ-field $\mathcal { F } _ { m } = \{ A : \omega , \omega ^ { \prime } \in A \Longrightarrow \omega _ { 1 } = \omega _ { 1 } ^ { \prime } , \omega _ { 2 } =$ $\omega _ { 2 } ^ { \prime } , \ldots , \omega _ { m } = \omega _ { m } ^ { \prime } \big \}$ . So all paths from a particular set A in this sigma field have identical initial segments while the remaining coordinates are arbitrary. Note that 

$$
\mathcal {F} _ {0} = \{\Omega , \emptyset \},
$$

$\mathcal { F } _ { 1 } = \{ A _ { 1 } , A _ { 1 } ^ { c } , \Omega , \emptyset \}$ , where $A _ { 1 } = \{ \omega : \omega _ { 1 } = 1 \}$ , i.e. $S ( 1 ) = S ( 0 ) U ,$ , and $A _ { 1 } ^ { c } = \{ \omega : \omega _ { 1 } = 0 \} \mathrm { i . e . } S ( 1 ) = S ( 0 ) D .$ 

## Exercise 2.12

Prove that $\mathcal { F } _ { m }$ has $2 ^ { 2 ^ { m } }$ elements. 

## Exercise 2.13

Prove that the sequence $\mathcal { F } _ { m }$ is increasing. 

This sequence is an example of a filtration (the identifying features are that the sigma fields should be contained in $\mathcal { F }$ and form an increasing chain), a concept which we shall revisit later on. 

The consecutive choices of stock prices are closely related to coin tossing. Intuition tells us that the latter are independent. This can be formally seen by introducing another σ-field describing the fact that at a particular step we have a particular outcome. Suppose $\omega$ is such that $\omega _ { k } = 1$ . Then we can identify the set of all paths with this property $A _ { k } = \{ \omega : \omega _ { k } = 1 \}$ and extend to a σ-field: $\mathcal { G } _ { k } = \{ A _ { k } , A _ { k } ^ { c } , \Omega , \emptyset \}$ . In fact, $A _ { k } ^ { c } = \{ \omega : \omega _ { k } = 0 \}$ 

Exercise 2.14 

Prove that $\mathcal { G } _ { m }$ and $\mathcal { G } _ { k }$ are independent if m $\neq k$ 

## 2.7 Proofs of propositions

## Proof (of Proposition 2.3)

If the intervals $I _ { n }$ cover B, then they also cover A: $A \subset B \subset \textstyle \bigcup _ { n } I _ { n }$ , hence $Z _ { B } \subset Z _ { A }$ S. The infimum of a larger set cannot be greater than the infimum of a smaller set (trivial illustration: inf $\{ 0 , 1 , 2 \} < \operatorname* { i n f } \{ 1 , 2 \} , \operatorname* { i n f } \{ 0 , 1 , 2 \} = \operatorname* { i n f } \{ 0 , 2 \} )$ hence the result. □ 

## Proof (of Proposition 2.6)

If a system $I _ { n }$ of intervals covers A then the intervals $I _ { n } + t$ cover $A + t$ Conversely, if $J _ { n }$ cover $A + t$ then $J _ { n } - t$ cover A. Moreover, the total length of a family of intervals does not change when we shift each by a number. So we have a one–one correspondence between the interval coverings of A and $A + t$ and this correspondence preserves the total length of the covering. This implies that the sets $Z _ { A }$ and $Z _ { A + t }$ are the same so their infima are equal. □ 

## Proof (of Proposition 2.9)

By de Morgan’s law 

$$
\bigcap_ {k = 1} ^ {\infty} E _ {k} = \left(\bigcup_ {k = 1} ^ {\infty} E _ {k} ^ {\mathrm{c}}\right) ^ {c}.
$$

By Theorem 2.8 (ii) all $E _ { k } ^ { \mathrm { c } }$ are in $\mathcal { M }$ , hence by (iii) the same can be said about the union $\textstyle \bigcup _ { k = 1 } ^ { \infty } E _ { k } ^ { c }$ . Finally, by (ii) again, the complement of this union is in $\mathcal { M }$ S, and so the intersection $\cap _ { k = 1 } ^ { \infty } E _ { k }$ is in $\mathcal { M }$ □ 

## Proof (of Proposition 2.10)

(i) Proposition 2.3 tells us that the outer measure is monotone, but since m is just the restriction of $m ^ { * }$ to , then the same is true for m: $A \subset B$ implies $m ( A ) = m ^ { * } ( A ) \leq m ^ { * } ( B ) = m ( B )$ 

(ii) We write B as a disjoint union $B = A \cup ( B \setminus A )$ and then by additivity of m we have $m ( B ) = m ( A ) + m ( B \setminus A )$ . Subtracting $m ( A )$ (here it is important that $m ( A )$ is finite) we get the result. 

(iii) Translation invariance of m follows at once from translation invariance of the outer measure in the same way as in (i) above. □ 

## Proof (of Proposition 2.11)

The set $A \varDelta B$ is null hence so are its subsets A B and $B \setminus A$ . Thus these sets are measurable, and so is $A \cap B = A \setminus ( A \setminus B )$ , and therefore also $B =$ $( A \cap B ) \cup ( B \setminus A ) \in { \mathcal { M } }$ . Now $m ( B ) = m ( A \cap B ) + m ( B \setminus A )$ as the sets on the right are disjoint. But $m ( B \setminus A ) = 0 = m ( A \setminus B ) , \operatorname { s o } m ( B ) = m ( A \cap B ) =$ m $( A \cap B ) + m ( A \setminus B ) = m ( ( A \cap B ) \cup ( A \setminus B ) ) = m ( A )$ □ 

## Proof (of Proposition 2.17)

The family $\mathcal { G } = \{ G \cup N : G \in \mathcal { F } , N \subset F \in \mathcal { F }$ with $\mu ( F ) = 0 \}$ contains the set X since $X \in { \mathcal { F } }$ . If $G _ { i } \cup N _ { i } \in \mathcal { G } , N _ { i } \subset F _ { i } , \mu ( F _ { i } ) = 0$ , then $\bigcup G _ { i } \cup N _ { i } = \bigcup G _ { i } \cup \bigcup N _ { i }$ is S S Sin since the first set on the right is in and the second is a subset of a null set $\bigcup F _ { i } \in \mathcal { F }$ . If $G \cup N \in { \mathcal { G } } , N \subset F ,$ then $( G \cup N ) ^ { c } = ( G \cup F ) ^ { c } \cup ( ( F \backslash N ) \cap G ^ { c } )$ .which Sis also in $\mathcal { G }$ Thus $\mathcal { G }$ is a σ-field. Consider any other σ-field  containing $\mathcal { F }$ and all subsets of null sets. Since $\mathcal { H }$ is closed with respect to the unions, it contains $\mathcal { G }$ and so $\mathcal { G }$ is the smallest σ-field with this property. □ 

## Proof (of Proposition 2.20)

It follows at once from the definitions and the Hint that $\mathcal { M } _ { B }$ is a $\sigma { - } \mathrm { f i e l d }$ . To see that $m _ { B }$ is a measure we check countable additivity: with ${ \cal C } _ { i } = A _ { i } \cap B$ pairwise disjoint in $\mathcal { M } _ { B }$ , we have 

$$
m _ {B} (\bigcup_ {i} C _ {i}) = m (\bigcup_ {i} (A _ {i} \cap B)) = \sum_ {i} m (A _ {i} \cap B) = \sum_ {i} m (C _ {i}) = \sum_ {i} m _ {B} (C _ {i}).
$$

Therefore $\left( B , \mathcal { M } _ { B } , m _ { B } \right)$ is a measure space. It is complete, since subsets of null sets contained in B are by definition m -measurable. □ 

## Proof (of Proposition 2.21)

Assume that $A _ { n }$ are measurable and pairwise disjoint. By the definition of conditional probability 

$$
\begin{array}{l} P (\bigcup_ {n = 1} ^ {\infty} A _ {n} | B) = \frac {1}{P (B)} P ((\bigcup_ {n = 1} ^ {\infty} A _ {n}) \cap B) \\ \qquad = \frac {1}{P (B)} P (\bigcup_ {n = 1} ^ {\infty} (A _ {n} \cap B)) \\ \qquad = \frac {1}{P (B)} \sum_ {n = 1} ^ {\infty} P (A _ {n} \cap B) \\ \qquad = \sum_ {n = 1} ^ {\infty} P (A _ {n} | B) \end{array}
$$

since $A _ { n } \cap B$ are also pairwise disjoint and P is countably additive. □ 

## 3.1 The extended real line

The length of R is unbounded above, i.e. ‘infinite’. To deal with this we defined Lebesgue measure for sets of infinite as well as finite measure. In order to handle functions between such sets comprehensively, it is convenient to allow functions which take infinite values: we take their range to be (part of) the ‘extended real line’ $\overline { { \mathbb { R } } } = [ - \infty , \infty ]$ , obtained by adding the ‘points at infinity’ $- \infty$ and $+ \infty$ to R. Arithmetic in this set needs a little care as already observed in Section 2.2: we assume that $a + \infty = \infty$ for all real a, $a \times \infty = \infty$ for $a > 0 , a \times \infty = - \infty$ for $a < 0 , \infty \times \infty = \infty$ and $0 \times \infty = 0$ , with similar definitions for $- \infty$ . These are all ‘obvious’ intuitively (except possibly $0 \times \infty )$ , and (as for measures) we avoid ever forming ‘sums’ of the form $\infty + ( - \infty )$ . With these assumptions ‘arithmetic works as before’. 

## 3.2 Lebesgue-measurable functions

The domain of the functions we shall be considering is usually R. Now we have the freedom of defining f only ‘up to null sets’: once we have shown two functions $f$ and $g$ to be equal on $\mathbb { R } \backslash E$ where E is some null set, then $f = g$ for all practical purposes. To formalize this, we say that $f$ has a property (P) almost everywhere (a.e.) if f has this property at all points of its domain, except 

possibly on some null set. 

For example, the function 

$$
f (x) = \left\{ \begin{array}{l l} 1 & \text {for} x \neq 0 \\ 0 & \text {for} x = 0 \end{array} \right.
$$

is almost everywhere continuous, since it is continuous on $\mathbb { R } \ \backslash \ \{ 0 \}$ , and the exceptional set 0 is null. (Note: Probabilists tend to say ‘almost surely’ (a.s.) instead of ‘almost everywhere’ (a.e.) and we shall follow their lead in the sections devoted to probability.) 

The next definition will introduce the class of Lebesgue-measurable functions. The condition imposed on $f : \mathbb { R }  \mathbb { R }$ will be necessary (though not suficient) to give meaning to the (Lebesgue) integral f dm. Let us first give some motivation. 

Integration is always concerned with the process of approximation. In the Riemann integral we split the interval $I = [ a , b ]$ , over which we integrate into small pieces $I _ { n } - \mathrm { a g a i n }$ intervals. The simplest method of doing this is to divide the interval into N equal parts. Then we construct approximating sums by multiplying the lengths of the small intervals by certain numbers $c _ { n }$ (related to the values of the function in question; for example $\begin{array} { r } { c _ { n } = \operatorname* { i n f } _ { I _ { n } } f , c _ { n } = \operatorname* { s u p } _ { I _ { n } } f . } \end{array}$ 8 or $c _ { n } = f ( x )$ for some $x \in I _ { n } )$ : 

$$
\sum_ {n = 1} ^ {N} c _ {n} l (I _ {n}).
$$

For large n this sum is close to the Riemann integral $\textstyle \int _ { a } ^ { b } f ( x )$ dx (given some regularity of f). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/073e2ee46fd678d1662d2e3ebd34bb57825e86bb559d94896b3c0e341b54f556.jpg)



Figure 3.1 Riemann vs. Lebesgue


The approach to the Lebesgue integral is similar but there is a crucial diference. Instead of splitting the integration domain into small parts, we decompose the range of the function. Again, a simple way is to introduce short intervals $J _ { n }$ of equal length. To build the approximating sums we first take the inverse images of $J _ { n }$ by f, i.e. $f ^ { - 1 } ( J _ { n } )$ . These may be complicated sets, not necessarily intervals. Here the theory of measure developed previously comes into its own. We are able to measure sets provided they are measurable, i.e. they are in . Given that, we compute 

$$
\sum_ {n = 1} ^ {N} c _ {n} m (f ^ {- 1} (J _ {n}))
$$

where $c _ { n } \in J _ { n }$ or $c _ { n } = \operatorname* { i n f } J _ { n }$ , for example. 

The following definition guarantees that this procedure makes sense (though some extra care may be needed to arrive at a finite number as $N \to \infty )$ 

## Definition 3.1

Suppose that E is a measurable set. We say that a function $f : E \longrightarrow$ R is (Lebesgue-)measurable if for any interval $I \subseteq \mathbb { R }$ 

$$
f ^ {- 1} (I) = \{x \in \mathbb {R}: f (x) \in I \} \in \mathcal {M}.
$$

In what follows, the term measurable (without qualification) will refer to Lebesgue-measurable functions. 

If all the sets $f ^ { - 1 } ( I ) ~ \in ~ B$ , i.e. if they are Borel sets, we call f Borelmeasurable, or simply a Borel function. 

The underlying philosophy is one which is common for various mathematical notions: the inverse image of a nice set is nice. Remember continuous functions, for example, where the inverse image of any open set is required to be open. The actual meaning of the word nice depends on the particular branch of mathematics. In the above definitions, note that since $B \subset { \mathcal { M } }$ , every Borel function is (Lebesgue-)measurable. 

## Remark 3.1

The terminology is somewhat unfortunate. ‘Measurable’ objects should be measured (as with measurable sets). However, measurable functions will be integrated. This confusion stems from the fact that the word integrable which would probably fit best here, carries a more restricted meaning, as we shall see later. This terminology is widely accepted and we are not going to try to fight the whole world here. 

We give some equivalent formulations: 

## Theorem 3.1

The following conditions are equivalent 

(a) f is measurable, 

(b) for all $a , f ^ { - 1 } ( \left( a , \infty \right) )$ is measurable, 

(c) for all $a , f ^ { - 1 } ( [ a , \infty ) )$ is measurable, 

(d) for all $a , f ^ { - 1 } ( ( - \infty , a ) )$ is measurable, 

(e) for all $a , f ^ { - 1 } ( ( - \infty , a ] )$ is measurable. 

## Proof

Of course (a) implies any of the other conditions. We show that (b) implies (a). The proofs of the other implications are similar, and are left as exercises (which you should attempt). 

We have to show that for any interval I, $f ^ { - 1 } ( I ) \in \mathcal { M }$ . By (b) we have that for the particular case $I = ( a , \infty )$ . Suppose $I = ( - \infty , a ]$ . Then 

$$
f ^ {- 1} ((- \infty , a ]) = f ^ {- 1} (\mathbb {R} \setminus (a, \infty)) = E \setminus f ^ {- 1} ((a, \infty)) \in \mathcal {M}\tag{3.1}
$$

since both E and $f ^ { - 1 } ( ( a , \infty ) )$ are in (we use the closure properties of established before). Next 

$$
\begin{array}{c} f ^ {- 1} ((- \infty , b)) = f ^ {- 1} \Big (\bigcup_ {n = 1} ^ {\infty} (- \infty , b - \frac {1}{n} ] \Big) \\ = \bigcup_ {n = 1} ^ {\infty} f ^ {- 1} \Big ((- \infty , b - \frac {1}{n} ] \Big). \end{array}
$$

By (3.1), $f ^ { - 1 } \left( \left( - \infty , b - \frac { 1 } { n } \right] \right) \in \mathcal { M }$ and the same is true for the countable union. From this we can easily deduce that 

$$
f ^ {- 1} ([ b, \infty)) \in \mathcal {M}.
$$

Now let $\boldsymbol { I } = \left( a , b \right)$ , and 

$$
\begin{array}{c} f ^ {- 1} ((a, b)) = f ^ {- 1} ((- \infty , b) \cap (a, \infty)) \\ = f ^ {- 1} ((- \infty , b)) \cap f ^ {- 1} ((a, \infty)) \end{array}
$$

is in as the intersection of two elements of . By the same reasoning contains 

$$
\begin{array}{c} f ^ {- 1} ([ a, b ]) = f ^ {- 1} ((- \infty , b ] \cap [ a, \infty)) \\ = f ^ {- 1} ((- \infty , b ]) \cap f ^ {- 1} ([ a, \infty)) \end{array}
$$

and half-open intervals are handled similarly. 

## 3.3 Examples

The following simple results show that most of the functions encountered ‘in practice’ are measurable. 

(i) Constant functions are measurable. Let $f ( x ) \equiv c .$ . Then 

$$
f ^ {- 1} ((a, \infty)) = \left\{ \begin{array}{l l} \mathbb {R} & \text { if } a <   c \\ \emptyset & \text { otherwise } \end{array} \right.
$$

and in both cases we have measurable sets. 

(ii) Continuous functions are measurable. For we note that $( a , \infty )$ is an open set and so is $f ^ { - 1 } ( ( a , \infty ) )$ . As we know, all open sets are measurable. 

(iii) Define the indicator function of a set A by 

$$
\mathbf {1} _ {A} (x) = \left\{ \begin{array}{l l} 1 & \text {if x\in A} \\ 0 & \text {otherwise.} \end{array} \right.
$$

Then 

$$
A \in \mathcal {M} \quad \Leftrightarrow \quad \mathbf {1} _ {A} \text {is measurable}
$$

since 

$$
\mathbf {1} _ {A} ^ {- 1} ((a, \infty)) = \left\{ \begin{array}{l l} \mathbb {R} & \text {if a <   0} \\ A & \text {if 0\leq a <   1} \\ \emptyset & \text {if a\geq 1.} \end{array} \right.
$$

Exercise 3.1 

Prove that every monotone function is measurable. 

Exercise 3.2 

Prove that if f is a measurable function, then the level set $\{ x : f ( x ) = a \}$ is measurable for every $a \in { \overline { { \mathbb { R } } } }$ 

Hint Don’t forget about the case when a is infinite! 

## Remark 3.2

In the Appendix, assuming the validity of the Axiom of Choice, we show that there are subsets of R which fail to be Lebesgue-measurable, and that there are Lebesgue-measurable sets which are not Borel sets. Thus, if ${ \mathcal { P } } ( \mathbb { R } )$ denotes the σ-field of all subsets of R, the following inclusions are strict 

$$
\mathcal {B} \subset \mathcal {M} \subset \mathcal {P} (\mathbb {R}).
$$

These (rather esoteric) facts can be used, by considering the indicator functions of these sets, to construct examples of non-measurable functions and of measurable functions which are not Borel functions. While it is important to be aware of these distinctions in order to understand why these diferent concepts are introduced at all, such examples will not feature in the applications of the theory which we have in mind. 

## 3.4 Properties

The class of measurable functions is very rich, as the following results show. 

## Theorem 3.2

The set of real-valued measurable functions defined on $E \in { \mathcal { M } }$ is a vector space and closed under multiplication, i.e. if f and g are measurable functions then $f + g$ , and $f g$ are also measurable (in particular, if g is a constant function $g \equiv c , c f$ is measurable for all real c). 

## Proof

Fix measurable functions $f , g : E \to \mathbb { R }$ . First consider $f + g .$ . Our goal is to show that for each $a \in \mathbb { R }$ 2 

$$
B = (f + g) ^ {- 1} (- \infty , a) = \{t: f (t) + g (t) <   a \} \in \mathcal {M}.
$$

Suppose that all the rationals are arranged in a sequence $\left\{ q _ { n } \right\}$ . Now 

$$
B = \bigcup_ {n = 1} ^ {\infty} \{t: f (t) <   q _ {n}, g (t) <   a - q _ {n} \}
$$

– we decompose the half-plane below the line $x + y = a$ into a countable union of unbounded ‘boxes’: $\{ ( x , y ) : x < q _ { n } , y < a - q _ { n } \}$ . Clearly 

$$
\{t: f (t) <   q _ {n}, g (t) <   a - q _ {n} \} = \{t: f (t) <   q _ {n} \} \cap \{t: g (t) <   a - q _ {n} \}
$$

is measurable as an intersection of measurable sets. Hence $B \in { \mathcal { M } }$ as a countable union of elements of $\mathcal { M }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/e64764fc69d45571567e35e44982cb626bc5f8bcf84118fbd0337ae3d80ce847.jpg)



Figure 3.2 Boxes


To deal with $f g$ we adopt a slightly indirect approach in order to remain ‘one-dimensional’: first note that if $g$ is measurable, then so is $- g$ . Hence $f - g =$ $f + ( - g )$ is measurable. Since $\begin{array} { r } { f g = \frac { 1 } { 4 } \{ ( f + g ) ^ { 2 } - ( f - g ) ^ { 2 } \} } \end{array}$ , it will sufice to prove that the square of a measurable function is measurable. So take a measurable $h : E \to \mathbb { R }$ and consider $\{ x \in E : h ^ { 2 } ( x ) > a \}$ . For $a < 0$ this set is $E \in { \mathcal { M } }$ , and for $a \geq 0$ 

$$
\{x: h ^ {2} (x) > a \} = \{x: h (x) > \sqrt {a} \} \cup \{x: h (x) <   - \sqrt {a} \}.
$$

Both sets on the right are measurable, hence we have shown that $h ^ { 2 }$ is measurable. Apply this with $h = f + g$ and $h = f - g$ respectively, to conclude that $f g$ is measurable. It follows that $c f$ is measurable for constant $^ { c , }$ hence that the class of real-valued measurable functions forms a vector space under addition. □ 

## Remark 3.3

An elegant proof of the theorem is based on the following lemma, which will also be useful later. Its proof makes use of the simple topological fact that every open set in $\mathbb { R } ^ { 2 }$ decomposes into a countable union of rectangles, in precise analogy with open sets in R and intervals. 

## Lemma 3.3

Suppose that $F : \mathbb { R } \times \mathbb { R } \to \mathbb { R }$ is a continuous function. If f and g are measurable, then $h ( x ) = F ( f ( x ) , g ( x ) )$ is also measurable. 

It now sufices to take $F ( u , v ) = u + v , F ( u , v ) = u v$ to obtain a second proof of Theorem 3.2. 

Proof (of the Lemma) 

For any real a 

$$
\{x: h (x) > a \} = \{x: (f (x), g (x)) \in G _ {a} \}
$$

where $G _ { a } = \{ ( u , v ) : F ( u , v ) > a \} = F ^ { - 1 } ( ( a , \infty ) )$ . Suppose for the moment that we have been lucky and $G _ { a }$ is a rectangle: $G _ { a } = \left( a _ { 1 } , b _ { 1 } \right) \times \left( c _ { 1 } , d _ { 1 } \right)$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/bd96670535da17051f63d833ba0d4d928293b63488a2bab7188a98faaf15bbe3.jpg)



Figure 3.3 The sets $G _ { a }$


It is clear from Figure 3.3 that 

$$
\begin{array}{c} \{x: h (x) > a \} = \{x: f (x) \in (a _ {1}, b _ {1}) \text {and} g (x) \in (c _ {1}, d _ {1}) \} \\ = \{x: f (x) \in (a _ {1}, b _ {1}) \} \cap \{x: g (x) \in (c _ {1}, d _ {1}) \}. \end{array}
$$

In general, we have to decompose the set $G _ { a }$ into a union of rectangles. The set $G _ { a }$ is an open subset of $\mathbb { R } \times \mathbb { R }$ since $F$ is continuous. Hence it can be written as 

$$
G _ {a} = \bigcup_ {n = 1} ^ {\infty} R _ {n}
$$

where $R _ { n }$ are open rectangles $R _ { n } = \left( a _ { n } , b _ { n } \right) \times \left( c _ { n } , d _ { n } \right)$ . So 

$$
\{x: h (x) > a \} = \bigcup_ {n = 1} ^ {\infty} \left\{x: f (x) \in \left(a _ {n}, b _ {n}\right) \right\} \cap \left\{x: g (x) \in \left(c _ {n}, d _ {n}\right) \right\}
$$

is measurable due to the stability properties of $\mathcal { M } .$ 

A simple application of Theorem 3.2 is to consider the product $f \cdot { \bf 1 } _ { A }$ . If $f$ is a measurable function, A is a measurable set, then $f \cdot { \bf 1 } _ { A }$ is measurable. This function is simply $f$ on A and 0 outside A. Applying this to the set $A = \{ x \in E : f ( x ) > 0 \}$ we see that the positive part $f ^ { + }$ of a measurable function is measurable: we have 

$$
f ^ {+} (x) = \left\{ \begin{array}{l l} f (x) & \text {if} f (x) > 0 \\ 0 & \text {if} f (x) \leq 0. \end{array} \right.
$$

Similarly the negative part $f ^ { - }$ of $f$ is measurable, since 

$$
f ^ {-} (x) = \left\{ \begin{array}{l l} 0 & \text {if} f (x) > 0 \\ - f (x) & \text {if} f (x) \leq 0. \end{array} \right.
$$

## Proposition 3.4

Let E be a measurable subset of $\mathbb { R }$ 

(i) $f : E \to \mathbb { R }$ is measurable if and only if both $f ^ { + }$ and $f ^ { - }$ are measurable. 

(ii) If f is measurable, then so is $| f | ;$ but the converse is false. 

Hint Part (ii) requires the existence of non-measurable sets (as proved in the Appendix) not their particular form. 

## Exercise 3.3

Show that if f is measurable, then the truncation of $f \colon$ 

$$
f ^ {a} (x) = \left\{ \begin{array}{l l} a & \text {if} f (x) > a \\ f (x) & \text {if} f (x) \leq a \end{array} \right.
$$

is also measurable. 

## Exercise 3.4

Find a non-measurable f such that $f ^ { 2 }$ is measurable. 

Passage to the limit does not destroy measurability – all the work needed was done when we established the stability properties of ! 

## Theorem 3.5

If $\left\{ f _ { n } \right\}$ is a sequence of measurable functions defined on the set E in R, then the following are measurable functions also: 

$$
\max _ {n \leq k} f _ {n}, \quad \min _ {n \leq k} f _ {n}, \quad \sup _ {n \in \mathbb {N}} f _ {n}, \quad \inf _ {n \in \mathbb {N}} f _ {n}, \quad \operatorname * {l i m s u p} _ {n \to \infty} f _ {n}, \quad \operatorname * {l i m i n f} _ {n \to \infty} f _ {n}.
$$

## Proof

It is suficient to note that the following are measurable sets: 

$$
\{x: (\max _ {n \leq k} f _ {n}) (x) > a \} = \bigcup_ {n = 1} ^ {k} \{x: f _ {n} (x) > a \},
$$

$$
\{x: (\min _ {n \leq k} f _ {n}) (x) > a \} = \bigcap_ {n = 1} ^ {k} \{x: f _ {n} (x) > a \},
$$

$$
\{x: (\sup _ {n \geq k} f _ {n}) (x) > a \} = \bigcup_ {n = k} \{x: f _ {n} (x) > a \},
$$

$$
\{x: (\inf _ {n \geq k} f _ {n}) (x) \geq a \} = \bigcap_ {n = k} \{x: f _ {n} (x) \geq a \}.
$$

For the upper limit, by definition 

$$
\limsup _ {n \to \infty} f _ {n} = \inf _ {n \geq 1} \left\{\sup _ {m \geq n} f _ {m} \right\}
$$

and the above relations show that $h _ { n } \ = \ \operatorname* { s u p } _ { m \geq n } f _ { m }$ is measurable, hence $\operatorname* { i n f } _ { n \geq 1 } h _ { n } ( x )$ is measurable. The lower limit is done similarly. □ 

## Corollary 3.6

If a sequence $f _ { n }$ of measurable functions converges (pointwise) then the limit is a measurable function. 

## Proof

This is immediate since $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f _ { n } = \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } f _ { n } } \end{array}$ which is measurable. 

## Remark 3.4

Note that Theorems 3.2 and 3.5 have counterparts for Borel functions, i.e. they remain valid upon replacing ‘measurable’ by ‘Borel’ throughout. 

Things are slightly more complicated when we consider the role of null sets. On the one hand, changing a function on a null set cannot destroy its measurability, i.e. any measurable function which is altered on a null set remains measurable. However, as not all null sets are Borel sets, we cannot conclude similarly for Borel sets, and thus the following results have no natural ‘Borel counterparts. 

## Theorem 3.7

If $f : E \to \mathbb { R }$ is measurable, $E \in { \mathcal { M } } , g : E \to \mathbb { R }$ is arbitrary, and the set $\{ x : f ( x ) = g ( x ) \}$ is null, then g is measurable. 

## Proof

Consider the diference $d ( x ) = g ( x ) - f ( x )$ . It is zero except on a null set so 

$$
\{x: d (x) > a \} = \left\{ \begin{array}{l l} \text {   a   null   set   } & \text {   if   } a \geq 0 \\ \text {   a   full   set   } & \text {   if   } a <   0 \end{array} \right.
$$

where a full set is the complement of a null set. Both null and full sets are measurable hence d is a measurable function. Thus $g = f + d$ is measurable. 

## Corollary 3.8

If $\left( f _ { n } \right)$ is a sequence of measurable functions and $f _ { n } ( x )  f ( x )$ almost everywhere for x in E, then f is measurable. 

## Proof

Let A be the null set such that $f _ { n } ( x )$ converges for all $x \in E \setminus A$ . Then $\mathbf { 1 } _ { A ^ { c } } f _ { n }$ converge everywhere to $g = { \bf 1 } _ { A ^ { c } } f$ which is therefore measurable. But $f = g$ almost everywhere, so f is also measurable. □ 

## Exercise 3.5

Let $f _ { n }$ be a sequence of measurable functions. Show that the set $E =$ $\{ x : f _ { n } ( x )$ converges is measurable. 

Since we are able to adjust a function f at will on a null set without altering its measurability properties, the following definition is a useful means of concentrating on the values of f that ‘really matter’ for integration theory, by identifying its bounds ‘outside null sets’: 

## Definition 3.2

Suppose $f : E \to { \overline { { \mathbb { R } } } }$ is measurable. The essential supremum ess sup f is defined as inf $\left\{ z : f \leq z { \mathrm { ~ a . e . } } \right\}$ and the essential infimum ess inf f is sup $\{ z : f \geq z { \mathrm { ~ a . e . } } \}$ 

Note that ess sup f can be $+ \infty$ . If ess sup $f = - \infty$ , then $f = - \infty \mathrm { a . e }$ . since by definition of ess sup, $f \leq - n { \mathrm { ~ a . e ~ } }$ . for all $n \geq 1$ . Now if ess sup f is finite, and $A = \{ x : \exp { \quad } \quad$ sup $f < f ( x ) \}$ , define $A _ { n }$ for $n \geq 1$ by 

$$
A _ {n} = \{x: \mathrm{ess} \sup f <   f (x) - \frac {1}{n} \}.
$$

These are null sets, hence so is $A = \textstyle \bigcup _ { n } A _ { n }$ , and thus we have verified: 

$$
f \leq \mathrm{ess} \sup f \mathrm{a.e.}
$$

The following is now straightforward to prove. 

## Proposition 3.9

If $f , g$ are measurable functions, then 

$$
\operatorname{ess} \sup (f + g) \leq \operatorname{ess} \sup f + \operatorname{ess} \sup g.
$$

Exercise 3.6 

Show that for measurable $f ,$ ess sup $f \leq \operatorname* { s u p } f$ . Show that these quantities coincide when f is continuous. 

## 3.5 Probability

## 3.5.1 Random variables

In the special case of probability spaces we use the phrase random variable to mean a measurable function. That is, if $( \varOmega , \mathcal { F } , P )$ is a probability space, then $X : \varOmega \to \mathbb { R }$ is a random variable if for all $a \in \mathbb { R }$ the set $X ^ { - 1 } ( [ a , \infty ) )$ is in ${ \mathcal { F } } \mathrm { : }$ 

$$
\{\omega \in \Omega : X (\omega) \geq a \} \in \mathcal {F}.
$$

In the case where $\Omega \subset \mathbb { R }$ is a measurable set and $\mathcal { F } = B$ is the σ-field of Borel subsets of $\varOmega ,$ , random variables are just Borel functions $\mathbb { R } \to \mathbb { R }$ 

In applied probability, the set $\varOmega$ represents the outcomes of a random experiment that can be observed by means of various measurements. These measurements assign numbers to outcomes and thus we arrive at the notion of random variable in a natural way. The condition imposed guarantees that questions of the following sort make sense: what is the probability that the value of the random variable lies within given limits? 

## 3.5.2 Sigma fields generated by random variables

As indicated before, the random variables we encounter will in fact be Borel measurable functions. The values of the random variable X will not lead us to non-Borel sets; in fact, they are likely to lead us to discuss much coarser distinctions between sets than are already available within the complexity of the Borel σ-field . We should therefore be ready to consider diferent σ-fields contained within . To be precise: 

The family of sets 

$$
X ^ {- 1} (\mathcal {B}) = \{S \subset \mathcal {F}: S = X ^ {- 1} (B) \text {   for   some   } B \in \mathcal {B} \}
$$

is a σ-field. If X is a random variable, $X ^ { - 1 } ( B ) \subset { \mathcal { F } }$ but it may be a much smaller subset depending on the degree of sophistication of X. We denote this σ-field by ${ \mathcal { F } } _ { X }$ and call it the σ-field generated by X. 

The simplest possible case is where X is constant, $X \equiv a$ . The $X ^ { - 1 } ( B )$ is either Ω or Ø depending on whether $a \in B$ or not and the σ-field generated is trivial: $\mathcal { F } = \{ \boldsymbol { O } , \boldsymbol { \varOmega } \}$ 

If X takes two values $a \ \ne \ b ,$ then ${ \mathcal { F } } _ { X }$ contains four elements: ${ \mathcal { F } } _ { X } ~ =$ $\{ \emptyset , \Omega , X ^ { - 1 } ( \{ a \} ) , X ^ { - 1 } ( \{ b \} ) \}$ . If X takes finitely many values, ${ \mathcal { F } } _ { X }$ is finite. If X takes denumerably many values, ${ \mathcal { F } } _ { X }$ is uncountable (it may be identified with the σ-field of all subsets of a countable set). We can see that the size of ${ \mathcal { F } } _ { X }$ grows together with the level of complication of X. 

Exercise 3.7 

Show that ${ \mathcal { F } } _ { X }$ is the smallest σ-field containing the inverse images $X ^ { - 1 } ( B )$ of all Borel sets B. 

Exercise 3.8 

Is the family of sets $\{ X ( A ) : A \in { \mathcal { F } } \}$ a σ-field? 

The notion of ${ \mathcal { F } } _ { X }$ has the following interpretation. The values of the measurement $X$ are all we can observe. From these we deduce some information on the level of complexity of the random experiment, that is the size of Ω and ${ \mathcal { F } } _ { X }$ 2 and we can estimate the probabilities of the sets in ${ \mathcal { F } } _ { X }$ by statistical methods. The $\sigma { - } \mathrm { f i e l d }$ generated represents the amount of information produced by the random variable. For example, suppose that a die is thrown and only 0 and 1 are reported depending on the number shown being odd or even. We will never distinguish this experiment from coin tossing. The information provided by the measurement is insuficient to explore the complexity of the experiment (which has six possible outcomes, here grouped together into two sets). 

## 3.5.3 Probability distributions

For any random variable X we can introduce a measure on the σ-field of Borel sets B by setting 

$$
P _ {X} (B) = P \left(X ^ {- 1} (B)\right).
$$

We call $P _ { X }$ the probability distribution of the random variable $X$ 

## Theorem 3.10

The set function $P _ { X }$ is countably additive. 

## Proof

Given pairwise disjoint Borel sets $B _ { i }$ their inverse images $X ^ { - 1 } ( B _ { i } )$ are pairwise disjoint and $\begin{array} { r } { X ^ { - 1 } ( \bigcup _ { i } B _ { i } ) = \bigcup _ { i } X ^ { - 1 } ( B _ { i } ) } \end{array}$ , so 

$$
\begin{array}{c} P _ {X} (\bigcup_ {i} B _ {i}) = P (X ^ {- 1} (\bigcup_ {i} B _ {i})) = P (\bigcup_ {i} X ^ {- 1} (B _ {i})) = \sum_ {i} P (X ^ {- 1} (B _ {i})) \\ = \sum_ {i} P _ {X} (B _ {i}) \end{array}
$$

as required. 

□ 

Thus $( \mathbb { R } , B , P _ { X } )$ is a probability space. For this it is suficient to note that $P _ { X } ( \mathbb { R } ) = P ( \varOmega ) = 1$ 

We consider some simple examples. Suppose that X is constant, i.e. $X \equiv a$ Then we call $P _ { X }$ the Dirac measure concentrated at a and denote by $\delta _ { a }$ . Clearly 

$$
\delta_ {a} (B) = \left\{ \begin{array}{l l} 1 & \text { if } a \in B \\ 0 & \text { if } a \notin B. \end{array} \right.
$$

In particular, $\delta _ { a } ( \{ a \} ) = 1$ 

If X takes 2 values: 

$$
X (\omega) = \left\{ \begin{array}{l l} a & \text { with   probability } p \\ b & \text { with   probability } 1 - p, \end{array} \right.
$$

then 

$$
P _ {X} (B) = \left\{ \begin{array}{l l} 1 & \text {if a,b\in B} \\ p & \text {if a\in B,b\notin B} \\ 1 - p & \text {if b\in B,a\notin B} \\ 0 & \text {otherwise,} \end{array} \right.
$$

and so 

$$
P _ {X} (B) = p \delta_ {a} (B) + (1 - p) \delta_ {b} (B).
$$

The distribution of a general discrete random variable (i.e. one which takes only finitely many diferent values, except possibly on some null set) is of the form: if the values of X are $a _ { i }$ taken with probabilities $p _ { i } > 0 , i = 1 , 2 , . . .$ $\sum p _ { i } = 1$ , then 

$$
P _ {X} (B) = \sum_ {i = 1} ^ {\infty} p _ {i} \delta_ {a _ {i}} (B).
$$

Classical examples are: 

(i) the geometric distribution, where $p _ { i } = ( 1 - q ) q ^ { i }$ for some $q \in ( 0 , 1 )$ 

(ii) the Poisson distribution where $\begin{array} { r } { p _ { i } = \frac { \lambda ^ { i } } { i ! } \mathrm { e } ^ { - \lambda } } \end{array}$ 

We shall not discuss the discrete case further since this is not our the primary goal in this text, and it is covered in many elementary texts on probability theory (such as [9]). 

Now consider the classical probability space with $\varOmega = [ 0 , 1 ] , \mathscr { F } = \mathscr { B } , P =$ m <sub>[0,1]</sub> – Lebesgue measure restricted to [0,1]. We can give examples of random variables given by explicit formulae. 

For instance, let $X ( \omega ) = a \omega + b $ . Then the image of [0, 1] is the interval $[ b , a + b ]$ and $\begin{array} { r } { P _ { X } = \frac { 1 } { a } m | _ { [ b , a + b ] } } \end{array}$ , i.e. for Borel B 

$$
P _ {X} (B) = \frac {m (B \cap [ b , a + b ])}{a}.
$$

## Example 3.1

Suppose a car leaves city A at random between 12 am and 1 pm. It travels at 50 mph towards B which is 25 miles from A. What is the probability distribution of the distance between the car and B at 1 pm? 

Clearly, this distance is 0 with probability $\textstyle { \frac { 1 } { 2 } }$ , i.e. if the car departs before 12.30. As a function of the starting time (represented as $\omega \in [ 0 , 1 ] )$ the distance has the form 

$$
X (\omega) = \left\{ \begin{array}{l l} 0 & \mathrm{if} \omega \in [ 0, \frac {1}{2} ] \\ 5 0 \omega - 2 5 & \mathrm{if} \omega \in (\frac {1}{2}, 1 ] \end{array} \right.
$$

and $\begin{array} { r } { P _ { X } = \frac { 1 } { 2 } P _ { 1 } + \frac { 1 } { 2 } P _ { 2 } } \end{array}$ where $\begin{array} { r } { P _ { 1 } = \delta _ { 0 } , P _ { 2 } = \frac { 1 } { 2 5 } m _ { [ 0 , 2 5 ] } } \end{array}$ . In this example, therefore, $P _ { X }$ is a combination of Dirac and Lebesgue measures. 

In later chapters we shall explore more complicated forms of X and the corresponding distributions after developing further machinery needed to handle the computations. 

## 3.5.4 Independence of random variables

## Definition 3.3

X, Y are independent if the σ-fields generated by them are independent. 

In other words, for any Borel sets B, C in R, 

$$
P (X ^ {- 1} (B) \cap Y ^ {- 1} (C)) = P (X ^ {- 1} (B)) P (Y ^ {- 1} (C)).
$$

## Example 3.2

Let $( \varOmega = [ 0 , 1 ] , \mathcal { M } )$ be equipped with Lebesgue measure. Consider $X = \mathbf { 1 } _ { [ 0 , \frac { 1 } { 2 } ] }$ 8 $Y = \mathbf { 1 } _ { [ \frac { 1 } { 4 } , \frac { 3 } { 4 } ] }$ . Then $\mathscr { F } _ { X } = \{ \emptyset , [ 0 , 1 ] , [ 0 , \frac { 1 } { 2 } ] , ( \frac { 1 } { 2 } , 1 ] \} , \mathscr { F } _ { Y } = \{ \emptyset , [ 0 , 1 ] , [ \frac { 1 } { 4 } , \frac { 3 } { 4 } ] , [ 0 , \frac { 1 } { 4 } ) ^ { \circ } \cup \}$ $\textstyle { \left( { \frac { 3 } { 4 } } , 1 \right] } \}$ are clearly independent. 

## Example 3.3

Let Ω be as above and let $X ( \omega ) = \omega , Y ( \omega ) = 1 - \omega$ . Then $\mathcal { F } _ { X } = \mathcal { F } _ { Y } = \mathcal { M }$ . A σ-field cannot be independent with itself (unless it is trivial): Take $A \in { \mathcal { F } }$ and then independence requires $P ( A \cap A ) = P ( A ) \times P ( A )$ (the set A belongs to ‘both’ σ-fields), i.e. $P ( A ) = P ( A ) ^ { 2 }$ which can happen only if either $P ( A ) = 0$ or $P ( A ) = 1$ . So a σ-field independent with itself consists of sets of measure zero or one. 

## 3.5.5 Applications to mathematical finance

Consider a model of stock prices, discrete in time, i.e. assume that the stock prices are given by a sequence $S ( n )$ of random variables, $n = 1 , 2 , \ldots , N$ . If the length of one step is h, then we have the time horizon $T = N h$ and we shall often write $S ( T )$ instead of $S ( N )$ . An example of such a model is the binomial tree considered in the previous chapter. Recall that a European call option is the random variable of the form $( S ( N ) - K ) ^ { + }$ (N is the exercise time, K is the strike price, S is the underlying asset). A natural generalisation of this is a random variable of the form $f ( S ( N ) )$ for some measurable function $f : \mathbb { R } \to \mathbb { R }$ . This random variable is of course measurable with respect to the σ-field generated by $S ( N )$ . This allows us to formulate a general definition: 

## Definition 3.4

A European derivative security (contingent claim) with the underlying asset represented by a sequence $S ( n )$ and exercise time N is a random variable X measurable with respect to the σ-field  generated by $S ( N )$ 

## Proposition 3.11

A European derivative security X must be of the form $X = f ( S ( N ) )$ for some measurable real function f. 

The above definition is not suficient for applications. For example, it does not cover one of the basic derivative instruments, namely futures. Recall that a holder of the futures contract has the right to receive (or an obligation to pay in case of negative values) a certain sequence $( X ( 1 ) , \ldots , X ( N ) )$ of cash payments depending on the values of the underlying security. To be specific, if for example the length of one step is one year and r is the risk free interest rate for annual compounding, then 

$$
X (n) = S (n) (1 + r) ^ {N - n} - X (n - 1) (1 + r) ^ {N - n + 1}.
$$

In order to introduce a general notion of derivative security which would cover futures, we first consider a natural generalisation 

$$
X (n) = f _ {n} (S (0), S (1), \dots , S (n))
$$

and then we push the level of generality ever further: 

## Definition 3.5

A derivative security (contingent claim) with the underlying asset represented by a sequence $( S ( n ) )$ and the expiry time N is a sequence $( X ( 1 ) , \ldots , X ( N ) )$ of random variables such that $X ( n )$ is measurable with respect to the σ-field ${ \mathcal { F } } _ { n }$ generated by $( S ( 0 ) , S ( 1 ) , \ldots , S ( n ) )$ , for each $n = 1 , \ldots , N $ 

## Proposition 3.12

A derivative security X must be of the form $X = f ( S ( 0 ) , S ( 1 ) , \ldots , S ( N ) )$ for some measurable $f : \mathbb { R } ^ { N + 1 } \longrightarrow \mathbb { R }$ 

We could make one more step and dispose of the underlying random variables. The role of the underlying object would be played by an increasing sequence of σ-fields ${ \mathcal { F } } _ { n }$ and we would say that a contingent claim (avoiding here the other term) is a sequence of random variables $X ( n )$ such that $X ( n )$ is ${ \mathcal { F } } _ { n }$ -measurable, but there is little need for such a generality in practical applications. The only case where that formulation would be relevant is the situation where there are no numerical observations but only some flow of information modelled by events and σ-fields. 

## Example 3.4

Payofs of exotic options depend on the whole paths of consecutive stock prices. For example, the payof of a European lookback option with exercise time N is determined by 

$$
f (x _ {0}, x _ {1}, \ldots , x _ {N}) = \max \{x _ {0}, x _ {1}, \ldots , x _ {N} \} - x _ {N}
$$

## Exercise 3.9

Find the function f for a down-and-out call (which is a European call except that is ceases to exist if the stock price at any time before the exercise date goes below the barrier $L < S ( 0 ) )$ . 

## Example 3.5

Consider an American put option in a binomial model. We shall see that it fits the above abstract scheme. Recall that American options can be exercised at any time before expiry and the payof of a put exercised at time n is $( K - S ( n ) ) ^ { + }$ written $g ( S ( n ) )$ for brevity, $g ( x ) = ( K - x ) ^ { + }$ . This option ofers to the holder cash flow of the same nature as the stock. The latter is determined by the stock price and stock can be sold at any time, of course only once. The American option can be sold or exercised also only once. The value of this option will be denoted by $P ^ { A } ( n )$ we shall show that it is a derivative security in the sense of Definition 3.5. 

We shall demonstrate that it is possible to write 

$$
P ^ {A} (n) = f _ {n} (S (n))
$$

for some functions $f _ { n }$ . Consider an option expiring at $N = 2$ . Clearly 

$$
f _ {2} (x) = g (x)
$$

At time $n = 1$ the holder of the option can exercise or wait till $n = 2$ . The value of waiting is the same as the value of European put issued at $n = 1$ with exercise time $N = 2$ (which, as is well known and will be seen in Section 7.4.3 in some detail) can be computed as the expectation with respect to some probability p of the discounted payof). The value of the American put is the greater of the two so 

$$
f _ {1} (x) = \max \left\{g (x), \frac {1}{1 + r} \left[ p f _ {2} (x U) + (1 - p) f _ {2} (x D) \right] \right\}.
$$

The same argument gives 

$$
f _ {0} (x) = \max \Big \{g (x), \frac {1}{1 + r} \left[ p f _ {1} (x U) + (1 - p _ {*}) f _ {1} (x D) \right] \Big \}.
$$

In general, for an American option expiring at time N we have the following chain of recursive formulae: 

$$
\begin{array}{c} f _ {N} (x) = g (x), \\ f _ {n - 1} (x) = \max \Big \{g (x), \frac {1}{1 + r} [ p f _ {n} (x U) + (1 - p) f _ {n} (x D) ] \Big \}. \end{array}
$$

## 3.6 Proofs of propositions

## Proof (of Proposition 3.4)

(i) We have proved that if f is measurable then so are $f ^ { + } , f ^ { - }$ . Conversely, note that $f ( x ) = f ^ { + } ( x ) - f ^ { - } ( x )$ so Theorem 3.2 gives the result. 

(ii) The function $u \mapsto | u |$ is continuous so Lemma 3.3 with $F ( u , v ) = | u |$ givesmeasurability of $| f |$ (an alternative is to use $| f | = f ^ { + } + f ^ { - } )$ . To see that theconverse is not true take a non-measurable set A and let $f = \mathbf { 1 } _ { A } - \mathbf { 1 } _ { A ^ { \mathrm { c } } }$ . It isnon-measurable since $\{ x : f ( x ) > 0 \} = A$ is non-measurable. But $| f | = 1$ isclearly measurable. 口

## Proof (of Proposition 3.9)

Since $f \leq$ ess supf and $g \leq \mathrm { e s s ~ s u p } g \mathrm { ~ a . e . ~ }$ ., by adding we have $f + g \le$ ess sup $f +$ ess sup g a.e. So the number ess sup f + ess sup g belongs to the set $\{ z : f + g \leq$ $z \ \mathrm { a . e . } \}$ hence the infimum of this set is smaller than this number. □ 

## Proof (of Proposition 3.11)

First note that the σ-field generated by $S ( N )$ is of the form $\mathcal { F } = \{ S ( N ) ^ { - 1 } ( B )$ : $B \mathrm { - B o r e l } \}$ since these sets form a σ-field and any other σ-field such that $S ( N )$ is measurable with respect to it has to contain all inverse images of Borel sets. Next we proceed in three steps: 

1) Suppose $X = \mathbf { 1 } _ { A }$ for $A \in { \mathcal { F } }$ . Then $A = S ( N ) ^ { - 1 } ( B )$ for a Borel subset of R. Put $f = \mathbf { 1 } _ { B }$ and clearly $X = f \circ S ( N )$ 

2) If X is a step function, $X = \sum c _ { i } \mathbf { 1 } _ { A _ { i } }$ then take $f = \sum c _ { i } \mathbf { 1 } _ { B _ { i } }$ where $A _ { i } = S ( N ) ^ { - 1 } ( B _ { i } )$ 

3) In general, a measurable function X can be approximated by step functions $\begin{array} { r } { X _ { n } = \sum _ { k = 0 } ^ { 2 ^ { 2 n } } \frac { k } { 2 ^ { n } } \cdot { \bf 1 } _ { Y ^ { - 1 } \left( \left[ \frac { k } { 2 ^ { n } } , \frac { k + 1 } { 2 ^ { n } } \right) \right) } } \end{array}$ (see Proposition 4.10 for more details) and we take $f = \operatorname* { l i m } \operatorname* { s u p } f _ { n }$ , where $f _ { n }$ corresponds to $Y _ { n }$ as in step 2) and the sequence clearly converges on the range of $S ( N )$ □ 

## Proof (of Proposition 3.12)

1) Suppose $X = \mathbf { 1 } _ { A }$ for $A \in { \mathcal { F } }$ . Then $A = ( S ( 1 ) , \ldots , S ( N ) ) ^ { - 1 } ( B )$ for Borel $B \subset \mathbb { R } ^ { N }$ , and $f = \mathbf { 1 } _ { B }$ satisfies the claim. 

Steps 2) and 3) are the same as in the proof of the previous proposition. 

The theory developed below deals with Lebesgue measure for the sake of simplicity. However, all we need (except for the section where we discuss the Riemann integration) is the property of $m$ being a measure, i.e. a countably additive (extended-) real valued function $\mu$ defined on a σ-field $\mathcal { F }$ of subsets of a fixed set $\varOmega .$ . Therefore, the theory developed for the measure space $( \mathbb { R } , \mathcal { M } , m )$ in the following sections can be extended virtually without change to an abstractly given measure space $( \varOmega , \mathcal { F } , \mu )$ 

We encourage the reader to bear in mind the possibility of such a generalization. We will need it in the probability section at the end of the chapter, and in the following chapters. 

## 4.1 Definition of the integral

We are now able to resolve one of the problems we identified earlier: how to integrate functions like $\mathbf { 1 } _ { \mathbb { Q } }$ , which take only finitely many values, but where the sets on which these values are taken are not at all ‘like intervals’. 

## Definition 4.1

A non-negative function $\varphi : \mathbb { R }  \mathbb { R }$ which takes only finitely many values, i.e. the range of $\varphi$ is a finite set of distinct non-negative reals $\{ a _ { 1 } , a _ { 2 } , \ldots , a _ { n } \}$ , is a 

simple function if all the sets 

$$
A _ {i} = \varphi^ {- 1} (\{a _ {i} \}) = \{x: \varphi (x) = a _ {i} \}, \qquad i = 1, 2, \ldots , n,
$$

are measurable sets. Note that the sets $A _ { i } \in { \mathcal { M } }$ are pairwise disjoint and their union is R. 

Clearly we can write 

$$
\varphi (x) = \sum_ {i = 1} ^ {n} a _ {i} {\bf 1} _ {A _ {i}} (x)
$$

so that (by Theorem 3.2) each simple function is measurable. 

## Definition 4.2

The (Lebesgue) integral over $E \in { \mathcal { M } }$ of the simple function $\varphi$ is given by: 

$$
\int_ {E} \varphi \mathrm{d} m = \sum_ {i = 1} ^ {n} a _ {i} m (A _ {i} \cap E).
$$

(Note: Since we shall allow $m ( A _ { i } ) = + \infty$ , we use the convention $0 \times \infty = 0$ here.) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/615a528ed1387e215a5f6f23b91750ef96faea58b952145f70382318c3c555eb.jpg)



Figure 4.1 Integral of a simple function


## Example 4.1

Consider the simple function $\mathbf { 1 } _ { \mathbb { Q } }$ which takes the value 1 on $\mathbb { Q }$ and 0 on $\mathbb { R } \setminus \mathbb { Q } .$ By the above definition we have 

$$
\int_ {\mathbb {R}} \mathbf {1} _ {\mathbb {Q}} \mathrm{d} m = 1 \times m (\mathbb {Q}) + 0 \times m (\mathbb {R} \setminus \mathbb {Q}) = 0
$$

since $\mathbb { Q }$ is a null set. Recall that this function is not Riemann-integrable. Similarly, $\mathbf { 1 } _ { C }$ has integral 0, where C is the Cantor set. 

## Exercise 4.1

Find the integral of $\varphi$ over E where 

(a) $\varphi ( x ) = \mathrm { I n t } ( x ) , E = [ 0 , 1 0 ]$ 

(b) $\varphi ( x ) = \operatorname { I n t } ( x ^ { 2 } ) , E = [ 0 , 2 ]$ 

(c) $\varphi ( x ) = \operatorname { I n t } ( \sin x ) , E = [ 0 , 2 \pi ]$ 

and Int denotes the integer part of a real number. (Note: many texts use the symbol [x] to denote Int(x). We prefer to use Int for increased clarity.) 

In order to extend the integral to more general functions, Henri Lebesgue (in 1902) adopted an apparently obvious, but subtle device: instead of partitioning the domain of a bounded function $f$ into many small intervals, he partitioned its range into a finite number of small intervals of the form $A _ { i } = [ a _ { i - 1 } , a _ { i } )$ 2 and approximated the ‘area’ under the graph of f by the upper sum 

$$
S (n) = \sum_ {i = 1} ^ {n} a _ {i} m (f ^ {- 1} (A _ {i}))
$$

and the lower sum 

$$
s (n) = \sum_ {i = 1} ^ {n} a _ {i - 1} m (f ^ {- 1} (A _ {i}))
$$

respectively; then integrable functions had the property that the infimum of all upper sums equals the supremum of all lower sums – mirroring Riemann’s construction (see also Figure 3.1). 

A century of experience with the Lebesgue integral has led to many equivalent definitions, some of them technically (if not always conceptually) simpler. We shall follow a version which, while very similar to Lebesgue’s original construction, allows us to make full use of the measure theory developed already. First we stay with non-negative functions: 

## Definition 4.3

For any non-negative measurable function f and $E \in { \mathcal { M } }$ the integral $\textstyle \int _ { E } f$ dm is defined as f 

$$
\int_ {E} f \mathrm{d} m = \sup Y (E, f)
$$

where 

$$
Y (E, f) = \Big \{\int_ {E} \varphi \mathrm{d} m: 0 \leq \varphi \leq f, \varphi \text {   is   simple } \Big \}.
$$

Note that the integral can be $+ \infty .$ , and is always non-negative. Clearly, the set $Y ( E , f )$ is always of the form $[ 0 , x ] { \mathrm { ~ o r ~ } } [ 0 , x )$ , where the value $x = + \infty$ is allowed. 

If $E = [ a , b ]$ we write the integral as 

$$
\int_ {a} ^ {b} f \mathrm{d} m, \quad \int_ {a} ^ {b} f (x) \mathrm{d} m (x),
$$

or even as $\textstyle \int _ { a } ^ { b } f ( x )$ dx, when no confusion is possible (and we set $\textstyle \int _ { a } ^ { b } f \mathrm { d } m =$ $- \int _ { b } ^ { a }$ Rf dm if $a > b )$ . The notation f dm means $\textstyle \int _ { \mathbb { R } } f \mathrm { d } m$ 

Clearly, if for some $A \in { \mathcal { M } }$ and a non-negative measurable function $g$ we have $g = 0$ on $A ^ { \mathrm { c } }$ , then any non-negative simple function that lies below g must be zero on $A ^ { \mathrm { c } }$ . Applying this to $g = f . 1 _ { A }$ we obtain the important identity 

$$
\int_ {A} f \mathrm{d} m = \int f {\bf 1} _ {A} \mathrm{d} m.
$$

## Exercise 4.2

Suppose that $f : [ 0 , 1 ] \to \mathbb { R }$ is defined by letting $f ( x ) = 0$ on the Cantor set and $f ( x ) = k$ for all x in each interval of length $3 ^ { - k }$ which has been removed from [0, 1]. Calculate $\textstyle \int _ { 0 } ^ { 1 } f$ dm. 

Hint Recall that $\begin{array} { r } { \sum _ { k = 1 } ^ { \infty } k x ^ { k - 1 } = \frac { d } { d x } ( \sum _ { k = 0 } ^ { \infty } x ^ { k } ) = \frac { 1 } { ( 1 - x ) ^ { 2 } } \mathrm { ~ w h e n ~ } | x | < 1 . } \end{array}$ 

If f is a simple function, we now have two definitions of the integral; thus for consistency you should check carefully that the above definitions coincide. 

## Proposition 4.1

For simple functions, Definitions 4.2 and 4.3 are equivalent. 

Furthermore, we can prove the following basic properties of integrals of simple functions: 

## Theorem 4.2

Let $\varphi , \psi$ be simple functions. Then: 

(i) if $\varphi \leq \psi$ then $\begin{array} { r } { \int _ { E } \varphi \mathrm { d } m \le \int _ { E } \psi \mathrm { d } m } \end{array}$ 2 

(ii) if $A , B$ are disjoint sets in $\mathcal { M }$ , then 

$$
\int_ {A \cup B} \varphi \mathrm{d} m = \int_ {A} \varphi \mathrm{d} m + \int_ {B} \varphi \mathrm{d} m,
$$

(iii) for all constants $a > 0$ 

$$
\int_ {E} a \varphi \mathrm{d} m = a \int_ {E} \varphi \mathrm{d} m.
$$

Proof 

(i) Notice that $Y ( E , \varphi ) \subseteq Y ( E , \psi )$ (we use Definition 4.3). 

(ii) Employing the properties of m we have $\left( \varphi = \sum c _ { i } \mathbf { 1 } _ { D _ { i } } \right)$ 

$$
\begin{array}{r l} \int_ {A \cup B} \varphi \mathrm{d} m & = \sum c _ {i} m (D _ {i} \cap (A \cup B)) \\ & = \sum c _ {i} \big (m (D _ {i} \cap A) + m (D _ {i} \cap B) \big) \\ & = \sum c _ {i} m (D _ {i} \cap A) + \sum c _ {i} (D _ {i} \cap B) \\ & = \int_ {A} \varphi \mathrm{d} m + \int_ {B} \varphi \mathrm{d} m. \end{array}
$$

(iii) If $\varphi = \sum c _ { i } { \bf 1 } _ { A _ { i } }$ <sub>i</sub> then $a \varphi = \sum a c _ { i } \mathbf { 1 } _ { A _ { i } }$ and 

$$
\int_ {E} a \varphi \mathrm{d} m = \sum a c _ {i} m (E \cap A _ {i}) = a \sum c _ {i} m (E \cap A _ {i}) = a \int_ {E} \varphi \mathrm{d} m
$$

as required. 

Next we show that the properties of the integrals of simple functions extend to the integrals of non-negative measurable functions: 

## Theorem 4.3

Suppose f and $g$ are non-negative measurable functions. 

(i) If $A \in { \mathcal { M } }$ , and $f \leq g$ on A, then 

$$
\int_ {A} f \mathrm{d} m \leq \int_ {A} g \mathrm{d} m.
$$

(ii) If $B \subseteq A , A , B \in { \mathcal { M } }$ , then 

$$
\int_ {B} f \mathrm{d} m \leq \int_ {A} f \mathrm{d} m.
$$

(iii) For $a \geq 0$ 

$$
\int_ {A} a f \mathrm{d} m = a \int_ {A} f \mathrm{d} m.
$$

(iv) If A is null then 

$$
\int_ {A} f \mathrm{d} m = 0.
$$

(v) If A, $B \in { \mathcal { M } } , A \cap B = \emptyset$ , then 

$$
\int_ {A \cup B} f \mathrm{d} m = \int_ {A} f \mathrm{d} m + \int_ {B} f \mathrm{d} m.
$$

Proof 

(i) Notice that $Y ( A , f ) \subseteq Y ( A , g )$ (there is more room to squeeze simple functions under g than under $f )$ and the sup of a bigger set is larger. 

(ii) If $\varphi$ is a simple function lying below $f$ on $B .$ , then extending it by zero outside B we obtain a simple function which is below $f$ on A. The integrals of these simple functions are the same so $Y ( B , f ) \subseteq Y ( A , f )$ and we conclude as in (i). 

(iii) The elements of the set $Y ( A , a f )$ are of the form $a \times x$ where $x \in Y ( A , f )$ so the same relation holds between their suprema. 

(iv) For any simple function $\varphi , \int _ { A } \varphi \mathrm { d } m = 0$ . To see this, take $\varphi = \sum c _ { i } \mathbf { 1 } _ { E _ { i } }$ say, then $m ( A \cap E _ { i } ) = 0$ Rfor each i, so $Y ( A , f ) = \{ 0 \}$ 

(v) The elements of $Y ( A \cup B , f )$ are of the form ϕ dm so by Theorem 4.2 (ii) they are of the form $\textstyle \int _ { A } \varphi \mathrm { d } m + \int _ { B } \varphi \mathrm { d } m$ R. So ${ \bar { Y } } ( A \cup B , f ) = Y ( A , f ) +$ $Y ( B , f )$ and taking suprema this yields $\textstyle \int _ { A \cup B } f \mathrm { d } m \leq \int _ { A } f \mathrm { d } m + \int _ { B } f$ dm. For R Rthe opposite inequality, suppose that the simple functions $\varphi$ Rand ψ satisfy: $\varphi \leq f$ on A and $\varphi = 0$ of A, while $\psi \leq f$ on B and $\psi = 0$ of B. Since $A \cap B = \emptyset$ , we can construct a new simple function $\gamma \leq f$ by setting $\gamma = \varphi$ on $A , \gamma = \psi$ on B and $\gamma = 0$ outside $A \cup B$ . Then 

$$
\begin{array}{r l} \int_ {A} \varphi \mathrm{d} m + \int_ {B} \psi \mathrm{d} m & = \int_ {A} \gamma \mathrm{d} m + \int_ {B} \gamma \mathrm{d} m \\ & = \int_ {A \cup B} \gamma \mathrm{d} m \\ & \leq \int_ {A \cup B} f \mathrm{d} m. \end{array}
$$

On the right we have an upper bound which remains valid for all simple functions that lie below f on $A \cup B$ . Thus taking suprema over $\varphi$ and $\psi$ separately on the left gives $\textstyle { \int _ { A } f \mathrm { d } m + \int _ { B } f \mathrm { d } m \leq \int _ { A \cup B } f \mathrm { d } m }$ □ 

## Exercise 4.3

Prove the following Mean Value Theorem for the integral: if $a \leq f ( x ) \leq b$ for $x \in A$ , then am $\textstyle ( A ) \leq \int _ { A } f \mathrm { d } m \leq b m ( A )$ 

We now confirm that null sets are precisely the ‘negligible sets’ for integration theory: 

## Theorem 4.4

Suppose f is a non-negative measurable function. Then $f = 0 ~ \mathrm { a . e }$ . if and only if $\textstyle \int _ { \mathbb { R } } f \mathrm { d } m = 0$ 

## Proof

First, note that if $f = 0 ~ \mathrm { a . e }$ . and $0 \leq \varphi \leq f$ is a simple function, then $\varphi = 0$ a.e. since neither f nor $\varphi$ take negative values. Thus $\textstyle \int _ { \mathbb { R } } \varphi \mathrm { d } m = 0$ for all such $\varphi$ and so $\textstyle \int _ { \mathbb { R } } f \mathrm { d } m = 0$ also. 

RConversely, given $\textstyle \int _ { \mathbb { R } } f \mathrm { d } m = 0$ , let $E = \{ x : f ( x ) > 0 \}$ . Our goal is to show that m $( E ) = 0 . \ \mathrm { P u t }$ 

$$
E _ {n} = f ^ {- 1} ([ \frac {1}{n}, \infty)) \quad \text { for } \quad n \geq 1.
$$

Clearly, $\{ E _ { n } \}$ increase to $E$ with 

$$
E = \bigcup_ {n = 1} ^ {\infty} E _ {n}.
$$

To show that $m ( E ) = 0$ it is suficient to prove that $m ( E _ { n } ) = 0$ for all n. (See Theorem 2.13.) The function $\begin{array} { r } { \varphi = \frac { 1 } { n } { \bf 1 } _ { E _ { n } } } \end{array}$ is simple and $\varphi \leq f$ by the definition of $E _ { n }$ . So 

$$
\int_ {\mathbb {R}} \varphi \mathrm{d} m = \frac {1}{n} m (E _ {n}) \leq \int_ {\mathbb {R}} f \mathrm{d} m = 0
$$

hence $m ( E _ { n } ) = 0$ for all $n$ . 

Using the results proved so far the following ‘a.e.’ version of the monotonicity of the integral is not dificult to prove: 

## Proposition 4.5

If f and g are measurable then $f \leq g$ a.e. implies $\textstyle { \int { f \mathrm { d } m } \leq \int g \mathrm { d } m }$ 

Hint Let $A = \{ x : f ( x ) \leq g ( x ) \}$ , then $B = A ^ { \mathrm { c } }$ is null and $f \mathbf { 1 } _ { A } \leq g \mathbf { 1 } _ { A }$ Now use Theorems 4.3 and 4.4. 

Using Theorems 3.2 and 3.5 you should now provide a second proof of a result we already noted in Proposition 3.4 but repeat here for emphasis: 

Proposition 4.6 

The function $f : \mathbb { R } \to \mathbb { R }$ is measurable if both $f ^ { + }$ and $f ^ { - }$ are measurable. 

## 4.2 Monotone Convergence Theorems

The crux of Lebesgue integration is its convergence theory. We can make a start on that by giving a famous result 

## Theorem 4.7 (Fatou’s Lemma)

If $\left\{ f _ { n } \right\}$ is a sequence of non-negative measurable functions then 

$$
\liminf _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m \geq \int_ {E} \left(\liminf _ {n \to \infty} f _ {n}\right) \mathrm{d} m.
$$

Proof 

Write 

$$
f = \liminf _ {n \to \infty} f _ {n}
$$

and recall that 

$$
f = \lim _ {n \to \infty} g _ {n}
$$

where $g _ { n } = \operatorname* { i n f } _ { k \geq n } f _ { k }$ (the sequence $g _ { n }$ is non-decreasing). Let $\varphi$ be a simple function, $\varphi \leq f$ . To show that 

$$
\int_ {E} f \mathrm{d} m \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m
$$

it is suficient to see that 

$$
\int_ {E} \varphi   \mathrm{d} m \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {E} f _ {n}   \mathrm{d} m
$$

for any such $\varphi .$ . 

The set where $f = 0$ is irrelevant since it does not contribute to $\textstyle \int _ { E } f$ dm so we can assume, without loss of generality, that $f > 0$ on $E .$ . Put 

$$
\overline {{\varphi}} (x) = \left\{ \begin{array}{l l} \varphi (x) - \varepsilon > 0 & \text {if} \varphi (x) > 0 \\ 0 & \text {if} \varphi (x) = 0 \text {or} x \notin E \end{array} \right.
$$

where $\varepsilon$ is suficiently small to ensure $\overline { { \varphi } } \geq 0$ 

Now $\overline { { \varphi } } < f , g _ { n } \nearrow f$ so ‘eventually’ $g _ { n } \geq \overline { { \varphi } }$ . We make the last statement more precise: put 

$$
A _ {k} = \{x: g _ {k} (x) \geq \overline {{\varphi}} (x) \}
$$

and we have 

$$
A _ {k} \subseteq A _ {k + 1}, \quad \bigcup_ {k = 1} ^ {\infty} A _ {k} = \mathbb {R}.
$$

Next, 

$$
\begin{array}{l} \int_ {A _ {n} \cap E} \overline {{\varphi}}   \mathrm{d} m \leq \int_ {A _ {n} \cap E} g _ {n}   \mathrm{d} m \quad (\text { as } g _ {n} \text { dominates } \overline {{\varphi}} \text { on } A _ {k}) \\ \qquad \leq \int_ {A _ {n} \cap E} f _ {k}   \mathrm{d} m \quad \text { for } k \geq n (\text { by   the   definition   of } g _ {n}) \\ \qquad \leq \int_ {E} f _ {k}   \mathrm{d} m \quad (\text { as } E \text { is   the   larger   set }) \end{array}
$$

for $k \geq n$ . Hence 

$$
\int_ {A _ {n} \cap E} \overline {{\varphi}}   \mathrm{d} m \leq \operatorname * {l i m i n f} _ {k \to \infty} \int_ {E} f _ {k}   \mathrm{d} m.\tag{4.1}
$$

Now we let $n \to \infty { : }$ writing $\begin{array} { r } { \overline { { \varphi } } = \sum _ { i = 1 } ^ { l } c _ { i } \mathbf { 1 } _ { B _ { i } } } \end{array}$ for some $c _ { i } \geq 0 , B _ { i } \in \mathcal { M } , i \leq l$ 

$$
\int_ {A _ {n} \cap E} \overline {{\varphi}} \mathrm{d} m = \sum_ {i = 1} ^ {l} c _ {i} m (A _ {n} \cap E \cap B _ {i}) \longrightarrow \sum_ {i = 1} ^ {l} c _ {i} m (E \cap B _ {i}) = \int_ {E} \overline {{\varphi}} \mathrm{d} m
$$

and the inequality (4.1) remains true in the limit: 

$$
\int_ {E} \overline {{\varphi}}   \mathrm{d} m \leq \operatorname * {l i m i n f} _ {k \to \infty} \int_ {E} f _ {k}   \mathrm{d} m.
$$

We are close – all we need is to replace $\overline { { \varphi } }$ by $\varphi$ in the last relation. This will be done by letting $\varepsilon \to 0$ but some care will be needed. 

Suppose that m $( \{ x : \varphi ( x ) > 0 \} ) < \infty$ . Then 

$$
\int_ {E} \overline {{\varphi}} \mathrm{d} m = \int_ {E} \varphi \mathrm{d} m - \varepsilon m (\{x: \varphi (x) > 0 \})
$$

and we get the result by letting $\varepsilon \to 0$ 

The case $m ( \{ x : \varphi ( x ) > 0 \} ) = \infty$ has to be treated separately. Here $\textstyle \int _ { E } \varphi \mathrm { d } m = \infty$ , so $\textstyle \int _ { E } f { \mathrm { d } } m = \infty$ . We have to show that 

$$
\liminf _ {k \to \infty} \int_ {E} f _ {k} \mathrm{d} m = \infty .
$$

Let $c _ { i }$ be the values of $\varphi$ and let $\begin{array} { r } { a = \frac { 1 } { 2 } \operatorname* { m i n } \{ c _ { i } \} \left( \{ c _ { i } \} \right. } \end{array}$ is a finite set!). Similarly to above put 

$$
D _ {n} = \{x: g _ {n} (x) > a \}
$$

and 

$$
\int_ {D _ {n} \cap E} g _ {n} \mathrm{d} m \to \infty
$$

since $D _ { n } \nearrow \mathbb { R }$ . As before 

$$
\int_ {D _ {n} \cap E} g _ {n} \mathrm{d} m \leq \int_ {D _ {n} \cap E} f _ {k} \mathrm{d} m \leq \int_ {E} f _ {k} \mathrm{d} m
$$

for $k \geq n$ , so lim inf $\int _ { E } f _ { k }$ dm has to be infinite. 

## Example 4.2

Let $f _ { n } = \mathbf { 1 } _ { [ n , n + 1 ] }$ . Clearly $\textstyle \int f _ { n } \mathrm { d } m = 1$ for all $n ,$ lim inf $f _ { n } = 0 ~ ( = \operatorname* { l i m } f _ { n } )$ , so Rthe above inequality may be strict and we have 

$$
\int \left(\lim f _ {n}\right) \mathrm{d} m \neq \lim \int f _ {n} \mathrm{d} m.
$$

## Exercise 4.4

Construct an example of a sequence of functions with the strict inequality as above, such that all $f _ { n }$ are zero outside the interval [0, 1]. 

It is now easy to prove one of the two main convergence theorems. 

## Theorem 4.8 (Monotone Convergence Theorem)

If $\left\{ f _ { n } \right\}$ is a sequence of non-negative measurable functions, and $\{ f _ { n } ( x ) : n \geq 1 \}$ increases monotonically to $f ( x )$ for each $x ,$ , i.e. $f _ { n } \nearrow f$ pointwise, then 

$$
\lim _ {n \to \infty} \int_ {E} f _ {n} (x) \mathrm{d} m = \int_ {E} f \mathrm{d} m.
$$

Proof 

Since $\begin{array} { r } { f _ { n } \leq f , \int _ { E } f _ { n } \mathrm { d } m \leq \int _ { E } f } \end{array}$ dm and so 

$$
\limsup _ {n \to \infty} \int_ {E} f _ {n}   \mathrm{d} m \leq \int_ {E} f   \mathrm{d} m.
$$

Fatou’s lemma gives 

$$
\int_ {E} f \mathrm{d} m \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m
$$

which together with the basic relation 

$$
\liminf _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m \leq \operatorname * {l i m s u p} _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m
$$

gives 

$$
\int_ {E} f \mathrm{d} m = \operatorname * {l i m i n f} _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m = \operatorname * {l i m s u p} _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m
$$

hence the sequence $\int _ { E } f _ { n }$ dm converges to $\textstyle \int _ { E } f \mathrm { d } m$ 

## Corollary 4.9

Suppose $\left\{ f _ { n } \right\}$ and f are non-negative and measurable. If $\left\{ f _ { n } \right\}$ increases to f almost everywhere, then we still have $\int _ { E } f _ { n }$ dm $\textstyle { \nearrow } \int _ { E } f$ dm for all measurable $E$ 

## Proof

Suppose that $f _ { n } \nearrow f$ a.e. and A is the set where the convergence holds, so that $A ^ { \mathrm { c } }$ is null. We can define 

$$
g _ {n} = \left\{ \begin{array}{l l} f _ {n} & \mathrm{on} A \\ 0 & \mathrm{on} A ^ {c}, \end{array} \right.
$$

$$
g = \left\{ \begin{array}{l l} f & \text {on A} \\ 0 & \text {on A} ^ {c}. \end{array} \right.
$$

Then using $E = [ E \cap A ^ { \mathrm { c } } ] \cup [ E \cap A ]$ we get 

$$
\begin{array}{r l} \int_ {E} g _ {n} \mathrm{d} m & = \int_ {E \cap A} f _ {n} \mathrm{d} m + \int_ {E \cap A ^ {\mathrm{c}}} 0 \mathrm{d} m \\ & = \int_ {E \cap A} f _ {n} \mathrm{d} m + \int_ {E \cap A ^ {\mathrm{c}}} f _ {n} \mathrm{d} m \\ & = \int_ {E} f _ {n} \mathrm{d} m \end{array}
$$

(since $E \cap A ^ { \mathrm { c } }$ is null) and similarly $\textstyle \int _ { E } g \mathrm { d } m = \int _ { E } f$ dm. The convergence $g _ { n }  g$ Rholds everywhere so by Theorem 4.8, $\begin{array} { r } { \int _ { E } g _ { n } \mathrm { d } m \longrightarrow \int _ { E } g \mathrm { d } m . } \end{array}$ □ 

To apply the monotone convergence theorem it is convenient to approximate non-negative measurable functions by increasing sequences of simple functions. 

## Proposition 4.10

For any non-negative measurable f there is a sequence $s _ { n }$ of non-negative simple functions such that $s _ { n } \nearrow f$ 

Hint Put 

$$
s _ {n} = \sum_ {k = 0} ^ {2 ^ {2 n}} \frac {k}{2 ^ {n}} \cdot {\bf 1} _ {f ^ {- 1} ([ \frac {k}{2 ^ {n}}, \frac {k + 1}{2 ^ {n}}))} .
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/1ea49dbe8faa591fcce70a499be7c603ffda441e3c6adc4803216c3fb0144d9d.jpg)



Figure 4.2 Approximation by simple functions


## 4.3 Integrable functions

All the hard work is done: we can extend the integral very easily to general real functions, using the positive part $f ^ { + } = \operatorname* { m a x } ( f , 0 )$ , and the negative part $f ^ { - } = \operatorname* { m a x } ( - f , 0 )$ , of any measurable function $f : \mathbb { R } \to \mathbb { R }$ . We will not use the non-negative measurable function $| f |$ alone: as we saw in Proposition 3.4, f can be measurable without f being measurable! 

## Definition 4.4

If $E \in { \mathcal { M } }$ and the measurable function f has both $\int _ { E } f ^ { + }$ dm and $\int _ { E } f ^ { - }$ dm finite, then we say that f is integrable, and define 

$$
\int_ {E} f \mathrm{d} m = \int_ {E} f ^ {+} \mathrm{d} m - \int_ {E} f ^ {-} \mathrm{d} m.
$$

The set of all functions that are integrable over E is denoted by $\mathcal { L } ^ { 1 } ( E )$ . In what follows E will be fixed and we often simply write $\mathcal { L } ^ { 1 }$ for $\mathcal { L } ^ { 1 } ( E )$ 

## Exercise 4.5

For which α, is $f ( x ) = x ^ { \alpha }$ in $\mathcal { L } ^ { 1 } ( E )$ where (a) $E = ( 0 , 1 )$ ; (b) $E =$ $( 1 , \infty ) ?$ 

Note that f is integrable if $| f |$ is integrable, and that 

$$
\int_ {E} | f | \mathrm{d} m = \int_ {E} f ^ {+} \mathrm{d} m + \int_ {E} f ^ {-} \mathrm{d} m.
$$

Thus the Lebesgue integral is an ‘absolute’ integral: we cannot ‘make’ a function integrable by cancellation of large positive and negative parts. This has the consequence that some functions which have improper Riemann integrals fail to be Lebesgue integrable (see Section. 4.5). 

The properties of the integral of non-negative functions extend to any, not necessarily non-negative, integrable functions. 

## Proposition 4.11

If f and g are integrable, $f \leq g$ , then $\textstyle { \int { f \mathrm { d } m } \leq \int g \mathrm { d } m }$ 

Hint If $f \leq g$ , then $f ^ { + } \leq g ^ { + }$ but $f ^ { - } \geq g ^ { - }$ 

## Remark 4.1

We observe (following [12], 5.12) that many proofs of results concerning integrable functions follow a standard pattern, utilising linearity and monotone convergence properties. To prove that a ’linear’ result holds for all functions in a space such as $\mathcal { L } ^ { 1 } ( E )$ we proceed in four steps: 

(i) verify that the required property holds for indicator functions – this is usually so by definition, 

(ii) use linearity to extend the property to non-negative simple functions, 

(iii) then use Monotone Convergence to show that the property is shared by all non-negative measurable functions, 

(iv) finally, extend to the whole class of functions by writing $f = f ^ { + } - f ^ { - }$ and using linearity again. 

The next result gives a good illustration of the technique. 

We wish to show that the mapping $f \mapsto \int _ { A } f$ dm is linear. This fact is Rinteresting on its own, but will also allow us to show that $\mathcal { L } ^ { 1 }$ is a vector space. 

## Theorem 4.12

For any integrable functions $f , g$ their sum $f + g$ is also integrable and 

$$
\int_ {E} (f + g) \mathrm{d} m = \int_ {E} f \mathrm{d} m + \int_ {E} g \mathrm{d} m.
$$

## Proof

We apply the technique described in Remark 4.1. 

Step 1. Suppose first that f and g are non-negative simple functions. The result is a matter of routine calculation: let $\begin{array} { r } { f = \sum a _ { i } \mathbf { 1 } _ { A _ { i } } , g = \sum b _ { j } \mathbf { 1 } _ { B _ { j } } } \end{array}$ . The sum $f + g$ P Pis also a simple function which can be written in the form 

$$
f + g = \sum_ {i, j} (a _ {i} + b _ {j}) \mathbf {1} _ {A _ {i} \cap B _ {j}}.
$$

Therefore 

$$
\begin{array}{l} \int_ {E} (f + g) \mathrm{d} m = \sum_ {i, j} (a _ {i} + b _ {j}) m (A _ {i} \cap B _ {j} \cap E) \\ \qquad = \sum_ {i} \sum_ {j} a _ {i} m (A _ {i} \cap B _ {j} \cap E) + \sum_ {j} \sum_ {i} b _ {j} m (A _ {i} \cap B _ {j} \cap E) \\ \qquad = \sum_ {i} a _ {i} \sum_ {j} m (A _ {i} \cap B _ {j} \cap E) + \sum_ {j} b _ {j} \sum_ {i} m (A _ {i} \cap B _ {j} \cap E) \\ \qquad = \sum_ {i} a _ {i} m (\bigcup_ {j} (A _ {i} \cap B _ {j} \cap E)) + \sum_ {j} b _ {j} m (\bigcup_ {i} (A _ {i} \cap B _ {j} \cap E)) \\ \qquad = \sum_ {i} a _ {i} m (A _ {i} \cap \bigcup_ {j} B _ {j} \cap E) + \sum_ {j} b _ {j} m (B _ {j} \cap \bigcup_ {i} A _ {i} \cap E) \\ \qquad = \sum_ {i} a _ {i} m (A _ {i} \cap E) + \sum_ {j} b _ {j} m (B _ {j} \cap E) \\ \qquad = \int_ {E} f   \mathrm{d} m + \int_ {E} g   \mathrm{d} m \end{array}
$$

where we have used the additivity of m and the facts that $A _ { i }$ cover R and the same is true for $B _ { j }$ 

Step 2. Now suppose that $f , g$ are non-negative measurable (not necessarily simple) functions. By Proposition 4.10 we can find sequences $s _ { n } , \ t _ { n }$ of simple functions such that $s _ { n } \nearrow f$ and $t _ { n } \nearrow g$ . Clearly $s _ { n } + t _ { n } \nearrow f + g$ hence using the monotone convergence theorem and the additivity property for simple functions we obtain 

$$
\begin{array}{l} \int_ {E} (f + g) \mathrm{d} m = \lim _ {n \to \infty} \int_ {E} (s _ {n} + t _ {n}) \mathrm{d} m \\ \qquad = \lim _ {n \to \infty} \int_ {E} s _ {n} \mathrm{d} m + \lim _ {n \to \infty} \int_ {E} t _ {n} \mathrm{d} m \\ \qquad = \int_ {E} f \mathrm{d} m + \int_ {E} g \mathrm{d} m. \end{array}
$$

This, in particular, implies that the integral of $f + g$ is finite if the integrals of f and g are finite. 

Step 3. Finally, let $f , g$ be arbitrary integrable functions. Since 

$$
\int_ {E} | f + g | \mathrm{d} m \leq \int_ {E} (| f | + | g |) \mathrm{d} m,
$$

we can use Step 2 to deduce that the left-hand side is finite. 

We have 

$$
\begin{array}{l} f + g = (f + g) ^ {+} - (f + g) ^ {-} \\ f + g = (f ^ {+} - f ^ {-}) + (g ^ {+} - g ^ {-}) \end{array}
$$

so 

$$
(f + g) ^ {+} - (f + g) ^ {-} = f ^ {+} - f ^ {-} + g ^ {+} - g ^ {-}.
$$

We rearrange the equality to have only additions on both sides 

$$
(f + g) ^ {+} + f ^ {-} + g ^ {-} = f ^ {+} + g ^ {+} + (f + g) ^ {-}.
$$

We have non-negative functions on both sides, so by what we have proved so far 

$$
\int_ {E} (f + g) ^ {+} \mathrm{d} m + \int_ {E} f ^ {-} \mathrm{d} m + \int_ {E} g ^ {-} \mathrm{d} m = \int_ {E} f ^ {+} \mathrm{d} m + \int_ {E} g ^ {+} \mathrm{d} m + \int_ {E} (f + g) ^ {-} \mathrm{d} m
$$

hence 

$$
\int_ {E} (f + g) ^ {+} \mathrm{d} m - \int_ {E} (f + g) ^ {-} \mathrm{d} m = \int_ {E} f ^ {+} \mathrm{d} m - \int_ {E} f ^ {-} \mathrm{d} m + \int_ {E} g ^ {+} \mathrm{d} m - \int_ {E} g ^ {-} \mathrm{d} m.
$$

By definition of the integral the last relation implies the claim of the theorem. 

The following result is a routine application of monotone convergence: 

Proposition 4.13 

If f is integrable and $c \in \mathbb { R }$ , then 

$$
\int_ {E} (c f) \mathrm{d} m = c \int_ {E} f \mathrm{d} m.
$$

Hint Approximate f by a sequence of simple functions. 

We complete the proof that $\mathcal { L } ^ { 1 }$ is a vector space: 

## Theorem 4.14

For any measurable E, $\mathcal { L } ^ { 1 } ( E )$ is a vector space. 

## Proof

Let $f , g \in { \mathcal { L } } ^ { 1 }$ . To show that $f + g \in { \mathcal { L } } ^ { 1 }$ we have to prove that $| f { + } g |$ is integrable: 

$$
\int_ {E} | f + g | \mathrm{d} m \leq \int_ {E} (| f | + | g |) \mathrm{d} m = \int_ {E} | f | \mathrm{d} m + \int_ {E} | g | \mathrm{d} m <   \infty .
$$

Now let c be a constant: 

$$
\int_ {E} | c f | \mathrm{d} m = \int_ {E} | c | | f | \mathrm{d} m = | c | \int_ {E} | f | \mathrm{d} m <   \infty
$$

so that $c f \in \mathcal { L } ^ { 1 } ( E )$ 

We can now answer an important question on the extent to which the integral determines the integrand. 

## Theorem 4.15

If $\textstyle { \int _ { A } f \mathrm { d } m \leq \int _ { A } g }$ dm for all $A \in { \mathcal { M } }$ , then $f \leq g$ almost everywhere. In partic-Rular, if $\textstyle { \int _ { A } f \mathrm { d } m = \int _ { A } }$ g dm for all $A \in { \mathcal { M } }$ , then $f = g$ almost everywhere. 

## Proof

By additivity of the integral (and Proposition 4.12 below) it is suficient to show that $\textstyle \int _ { A } h \mathrm { d } m \geq 0$ for all $A \in { \mathcal { M } }$ implies $h \geq 0$ (and then take $h = g - f )$ 

Write $A = \{ x : h ( x ) < 0 \}$ ; then $A = \bigcup A _ { n }$ where $A _ { n } = \{ x : h ( x ) \leq - { \frac { 1 } { n } } \}$ . By monotonicity of the integral 

$$
\int_ {A _ {n}} h \mathrm{d} m \leq \int_ {A _ {n}} \left(- \frac {1}{n}\right) \mathrm{d} m = - \frac {1}{n} m (A _ {n}),
$$

which is non-negative but this can only happen if $m ( A _ { n } ) = 0$ . The sequence of sets $A _ { n }$ increases with $n ,$ hence $m ( A ) = 0$ , and so $h ( x ) \geq 0$ almost everywhere. 

A similar argument shows that if $\textstyle \int _ { A } h \mathrm { d } m \leq 0$ for all $A .$ , then $h \leq 0 ~ \mathrm { a . e }$ This implies the second claim of the theorem: put $h = g - f$ and $\int _ { A }$ h dm is both non-negative and non-positive, hence $h \geq 0$ and $h \leq 0 ~ \mathrm { a . e }$ R. thus $h = 0$ a.e. □ 

The next Proposition lists further important properties of integrable functions, whose straightforward proofs are typical applications of the results proved so far. 

## Proposition 4.16

(i) An integrable function is a.e. finite. 

(ii) For measurable f and A 

$$
m (A) \inf _ {A} f \leq \int_ {A} f \mathrm{d} m \leq m (A) \sup _ {A} f.
$$

<sup>(iii)</sup> | $f \mathrm { d } m | \leq \int | f |$ dm. 

(iv) Assume that $f \geq 0$ and $\textstyle \int f \mathrm { d } m = 0$ . Then $f = 0 { \mathrm { ~ a . e . } }$ 

The following theorem gives us the possibility of constructing many interesting measures, and is essential for the development of probability distributions. 

## Theorem 4.17

Let $f \geq 0$ . Then $A \mapsto \textstyle \int _ { A } f$ dm is a measure. 

Proof 

Denote $\textstyle \mu ( A ) = \int _ { A } f$ dm. The goal is to show 

$$
\mu (\bigcup_ {i} E _ {i}) = \sum \mu (E _ {i})
$$

for pairwise disjoint $E _ { i }$ . To this end consider the sequence $g _ { n } = f \mathbf { 1 } _ { \bigcup _ { i = 1 } ^ { n } E _ { i } }$ and note that $g _ { n } \nearrow g$ , where $g = f \mathbf { 1 } _ { \mathsf { U } _ { i = 1 } ^ { \infty } E _ { i } }$ . Now 

$$
\int g \mathrm{d} m = \mu (\bigcup_ {i = 1} ^ {\infty} E _ {i}),
$$

$$
\int g _ {n} \mathrm{d} m = \int_ {\bigcup_ {i = 1} ^ {n} E _ {i}} f \mathrm{d} m = \sum_ {i = 1} ^ {n} \int_ {E _ {i}} f \mathrm{d} m = \sum_ {i = 1} ^ {n} \mu (E _ {i})
$$

and the monotone convergence theorem completes the proof. 

## 4.4 The Dominated Convergence Theorem

Many questions in analysis centre on conditions under which the order of two limit processes, applied to certain functions, can be interchanged. Since integration is a limit process applied to measurable functions, it is natural to ask under what conditions on a pointwise (or pointwise a.e.) convergent sequence $\left( f _ { n } \right)$ , the limit of the integrals is the integral of the pointwise limit function $f _ { : }$ i.e. when can we state that lim $\textstyle { \int f _ { n } \mathrm { d } m = \int ( \operatorname* { l i m } f _ { n } ) }$ dm? The monotone con-R Rvergence theorem (Theorem 4.8) provided the answer that this conclusion is valid for monotone increasing sequences of non-negative measurable functions, though in that case, of course, the limits may equal + . The following example shows that for general sequences of integrable functions the conclusion will not hold without some further conditions: 

## Example 4.3

Let $f _ { n } ( x ) = n \mathbf { 1 } _ { [ 0 , \frac { 1 } { n } ] } ( x )$ . Clearly $f _ { n } ( x ) \to 0$ for all x but $\textstyle \int f _ { n } ( x ) \mathrm { d } x = 1$ 

The limit theorem which turns out to be the most useful in practice states that convergence holds for an a.e. convergent sequence which is dominated by an integrable function. Again Fatou’s lemma holds the key to the proof. 

## Theorem 4.18 (Dominated Convergence Theorem)

Suppose $E \in { \mathcal { M } }$ . Let $\left( f _ { n } \right)$ be a sequence of measurable functions such that $| f _ { n } | \leq g$ a.e. on E for all $n \geq 1$ , where g is integrable over E. If $f = \operatorname* { l i m } _ { n \to \infty } f _ { n }$ a.e. then f is integrable over E and 

$$
\lim _ {n \to \infty} \int_ {E} f _ {n} (x) \mathrm{d} m = \int_ {E} f \mathrm{d} m.
$$

Proof 

Suppose for the moment that $f _ { n } \geq 0$ . Fatou’s lemma gives 

$$
\int_ {E} f \mathrm{d} m \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m.
$$

It is therefore suficient to show that 

$$
\limsup _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m \leq \int_ {E} f \mathrm{d} m.\tag{4.2}
$$

Fatou’s lemma applied to $g - f _ { n }$ gives 

$$
\int_ {E} \lim _ {n \to \infty} (g - f _ {n}) \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {E} (g - f _ {n})   \mathrm{d} m.
$$

On the left we have 

$$
\int_ {E} (g - f) \mathrm{d} m = \int_ {E} g \mathrm{d} m - \int_ {E} f \mathrm{d} m.
$$

On the right 

$$
\begin{array}{l} \underset {n \to \infty} {\liminf} \int_ {E} (g - f _ {n})   \mathrm{d} m \\ = \underset {n \to \infty} {\liminf} \left(\int_ {E} g   \mathrm{d} m - \int_ {E} f _ {n}   \mathrm{d} m\right) \\ = \int_ {E} g   \mathrm{d} m - \underset {n \to \infty} {\limsup} \int_ {E} f _ {n}   \mathrm{d} m, \end{array}
$$

where we have used the elementary fact that 

$$
\liminf _ {n \to \infty} (- a _ {n}) = - \limsup _ {n \to \infty} a _ {n}.
$$

Putting this together we get 

$$
\int_ {E} g \mathrm{d} m - \int_ {E} f \mathrm{d} m \leq \int_ {E} g \mathrm{d} m - \operatorname * {l i m s u p} _ {n \to \infty} \int_ {E} f _ {n} \mathrm{d} m.
$$

Finally, subtract $\textstyle \int _ { E } g$ dm (which is finite) and multiply by 1 to arrive at (4.2). 

Now consider a general, not necessarily non-negative sequence $\left( f _ { n } \right)$ . Since by the hypothesis 

$$
- g (x) \leq f _ {n} (x) \leq g (x)
$$

we have 

$$
0 \leq f _ {n} (x) + g (x) \leq 2 g (x)
$$

and we can apply the result proved for non-negative functions to the sequence $f _ { n } ( x ) + g ( x )$ (the function $2 g$ is of course integrable). □ 

## Example 4.4

Going back to the example preceding the theorem, $f _ { n } = n \mathbf { 1 } _ { [ 0 , \frac { 1 } { n } ] }$ , we can see that an integrable $g$ to dominate $f _ { n }$ cannot be found. The least upper bound is $\begin{array} { r } { g ( x ) = \operatorname* { s u p } _ { n } f _ { n } ( x ) , g ( x ) = k } \end{array}$ on $\textstyle { \big ( } { \frac { 1 } { k + 1 } } , { \frac { 1 } { k } } { \big ] }$ so 

$$
\int g (x) \mathrm{d} x = \sum_ {k = 1} ^ {\infty} k (\frac {1}{k} - \frac {1}{k + 1}) = \sum_ {k = 1} ^ {\infty} \frac {1}{k + 1} = + \infty .
$$

For a typical positive example consider 

$$
f _ {n} (x) = \frac {n \sin x}{1 + n ^ {2} x ^ {1 / 2}}
$$

for $x \in ( 0 , 1 )$ . Clearly $f _ { n } ( x ) \to 0$ . To conclude that lim $n \int f _ { n } \mathrm { d } m = 0$ we need an integrable dominating function. This is usually where some ingenuity is needed; however in the present example the most straightforward estimate will sufice: 

$$
\left| \frac {n \sin x}{1 + n ^ {2} x ^ {1 / 2}} \right| \leq \frac {n}{1 + n ^ {2} x ^ {1 / 2}} \leq \frac {n}{n ^ {2} x ^ {1 / 2}} = \frac {1}{n x ^ {1 / 2}} \leq \frac {1}{x ^ {1 / 2}}.
$$

(To see from first principles that the dominating function $\textstyle g : x \mapsto { \frac { 1 } { \sqrt { x } } }$ is integrable over [0, 1] can be rather tedious – cf. the worked example in Chapter 1 for the Riemann integral of $x \mapsto { \sqrt { x } }$ . However, we shall show shortly that the Lebesgue and Riemann integrals of a bounded function coincide if the latter exists, and hence we can apply the Fundamental Theorem of the Calculus to confirm the integrability of $g . \int$ 

The following facts will be useful later. 

## Proposition 4.19

Suppose $f$ is integrable and define $g _ { n } = f \mathbf { 1 } _ { [ - n , n ] } , h _ { n } = \operatorname* { m i n } ( f , n )$ (both truncate $f$ in some way: the $g _ { n }$ vanish outside a bounded interval, the $h _ { n }$ are bounded). Then $\begin{array} { r } { \int \left| f - g _ { n } \right| \mathrm { d } m \to 0 , \int \left| f - h _ { n } \right| \mathrm { d } m \to 0 } \end{array}$ 

Hint Use the dominated convergence theorem. 

## Exercise 4.6

Use the dominated convergence theorem to find 

$$
\lim _ {n \to \infty} \int_ {1} ^ {\infty} f _ {n} (x) \mathrm{d} x
$$

where 

$$
f _ {n} (x) = \frac {\sqrt {x}}{1 + n x ^ {3}}.
$$

Exercise 4.7 

Investigate the convergence of 

$$
\int_ {a} ^ {\infty} \frac {n ^ {2} x \mathrm{e} ^ {- n ^ {2} x ^ {2}}}{1 + x ^ {2}} \mathrm{d} x
$$

for $a > 0$ , and for $a = 0$ 

Exercise 4.8 

Investigate the convergence of 

$$
\int_ {0} ^ {\infty} \frac {1}{(1 + \frac {x}{n}) ^ {n} \sqrt [ n ]{x}} \mathrm{d} x.
$$

We will need the following extension of Theorem 4.12: 

## Proposition 4.20

For a sequence of non-negative measurable functions $f _ { n }$ we have 

$$
\int \sum_ {n = 1} ^ {\infty} f _ {n} \mathrm{d} m = \sum_ {n = 1} ^ {\infty} \int f _ {n} \mathrm{d} m.
$$

Hint The sequence $\textstyle g _ { k } = \sum _ { n = 1 } ^ { k } f _ { n }$ is increasing and converges to $\textstyle \sum _ { n = 1 } ^ { \infty } f _ { n }$ 

We cannot yet conclude that the sum of the series on the right-hand side is a.e. finite, so $\textstyle \sum _ { n = 1 } ^ { \infty } f _ { n }$ need not be integrable. However: 

## Theorem 4.21 (Beppo–Levi)

Suppose that 

$$
\sum_ {k = 1} ^ {\infty} \int | f _ {k} | \mathrm{d} m \text { is   finite. }
$$

Then the series $\scriptstyle \sum _ { k = 1 } ^ { \infty } f _ { k } ( x )$ converges for almost all $x ,$ its sum is integrable, and 8 8 

$$
\int \sum_ {k = 1} ^ {\infty} f _ {k} \mathrm{d} m = \sum_ {k = 1} ^ {\infty} \int f _ {k} \mathrm{d} m.
$$

Proof 

The function $\textstyle \varphi ( x ) = \sum _ { k = 1 } ^ { \infty } | f _ { k } ( x ) |$ is non-negative, measurable, and by Proposition 4.20 

$$
\int \varphi \mathrm{d} m = \sum_ {k = 1} ^ {\infty} \int | f _ {k} | \mathrm{d} m.
$$

This is finite, so $\varphi$ is integrable. Therefore $\varphi$ is finite a.e. Hence the series $\scriptstyle \sum _ { k = 1 } ^ { \infty } | f _ { k } ( x ) |$ converges a.e. and so the series $\scriptstyle \sum _ { k = 1 } ^ { \infty } f _ { k } ( x )$ converges (since it Pconverges absolutely) for almost all x. Let $\textstyle f ( x ) = \sum _ { k = 1 } ^ { \infty } f _ { k } ( x )$ (put $f ( x ) = 0$ Pfor x for which the series diverges – the value we choose is irrelevant since the set of such x is null). For all partial sums we have 

$$
\left| \sum_ {k = 1} ^ {n} f _ {k} (x) \right| \leq \varphi (x)
$$

so we can apply the dominated convergence theorem to find 

$$
\begin{array}{l} \int f \mathrm{d} m = \int \lim _ {n \to \infty} \sum_ {k = 1} ^ {n} f _ {k} \mathrm{d} m \\ \qquad = \lim _ {n \to \infty} \int \sum_ {k = 1} ^ {n} f _ {k} \mathrm{d} m \\ \qquad = \lim _ {n \to \infty} \sum_ {k = 1} ^ {n} \int f _ {k} \mathrm{d} m \\ \qquad = \sum_ {k = 1} ^ {\infty} \int f _ {k} \mathrm{d} m \end{array}
$$

as required. 

## Example 4.5

Recalling that $\begin{array} { r } { \sum _ { k = 1 } ^ { \infty } k x ^ { k - 1 } = \frac { 1 } { ( 1 - x ) ^ { 2 } } } \end{array}$ we can use the Beppo–Levi theorem to evaluate the integral $\textstyle \int _ { 0 } ^ { 1 } ( { \frac { \log x } { 1 - x } } ) ^ { 2 } \mathrm { d } x$ : first let $f _ { n } ( x ) \ = \ n x ^ { n - 1 } ( \log x ) ^ { 2 }$ for $n \geq 1 , x \in ( 0 , 1 )$ R, so that $f _ { n } \geq 0 , f _ { n }$ is continuous, hence measurable, and $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } f _ { n } ( x ) ~ = ~ ( \frac { \log { x } } { 1 - x } ) ^ { 2 } ~ = ~ f ( x ) } \end{array}$ is finite for $x \in \mathsf { \Gamma } ( 0 , 1 )$ . By Beppo–Levi the sum is integrable and $\begin{array} { r } { \int _ { 0 } ^ { 1 } f ( x ) \mathrm { d } x = \sum _ { n = 1 } ^ { \infty } \int _ { 0 } ^ { 1 } f _ { n } ( x ) } \end{array}$ dx. To calculate $\textstyle \int _ { 0 } ^ { 1 } f _ { n } ( x )$ dx we first use integration by parts to obtain $\begin{array} { r } { \int _ { 0 } ^ { 1 } x ^ { n - 1 } ( \log x ) ^ { 2 } \mathrm { d } x \ = \ \frac { 2 } { n ^ { 3 } } } \end{array}$ . Thus $\begin{array} { r } { \int _ { 0 } ^ { 1 } f ( x ) \mathrm { d } x = 2 \sum _ { n = 1 } ^ { \infty } \frac { 1 } { n ^ { 2 } } = \frac { \pi ^ { 2 } } { 3 . } } \end{array}$ 

## Exercise 4.9

The following are variations on the above theme: 

(a) For which values of $a \in \mathbb { R }$ does the power series $\textstyle \sum _ { n \geq 0 } n ^ { a } x ^ { n }$ define an integrable function on $[ - 1 , 1 ] ?$ 

(b) Show that $\begin{array} { r } { \int _ { 0 } ^ { \infty } \frac { x } { \mathrm { e } ^ { x } - 1 } \mathrm { d } x = \frac { \pi ^ { 2 } } { 6 } } \end{array}$ 

## 4.5 Relation to the Riemann integral

Our prime motivation for introducing the Lebesgue integral has been to provide a sound theoretical foundation for the twin concepts of measure and integral, and to serve as the model upon which an abstract theory of measure spaces can be built. Such a general theory has many applications, a principal one being the mathematical foundations of the theory of probability. At the same time, Lebesgue integration has greater scope and more flexibility in dealing with limit operations than does its Riemann counterpart. 

However, just as with the Riemann integral, the computation of specific integrals from first principles is laborious, and we have, as yet, no simple ‘recipes for handling particular functions. To link the theory with the convenient techniques of elementary calculus we therefore need to take two further steps: to prove the Fundamental Theorem of the Calculus as stated in Chapter 1 and to show that the Lebesgue and Riemann integrals coincide whenever the latter exists. In the process we shall find necessary and suficient conditions for the existence of the Riemann integral. 

In fact, given Proposition 4.16 the proof of the Fundamental Theorem becomes a simple application of the intermediate value theorem for continuous functions, and is left to the reader: 

## Proposition 4.22

If $f : [ a , b ]  \mathbb { R }$ is continuous then f is integrable and the function F given by $\begin{array} { r } { F ( x ) = \int _ { a } ^ { x } f } \end{array}$ dm is diferentiable for $x \in ( a , b )$ , with derivative $F ^ { \prime } = f$ 

Hint Note that if $f \in \mathcal { L } ^ { 1 }$ and $A , B \in { \mathcal { M } }$ are disjoint, then $\textstyle \int _ { A \cup B } f \mathrm { d } m =$ $\textstyle { \int _ { A } f \operatorname { d } m + \int _ { B } f }$ dm. Thus show that we can write $\begin{array} { r } { F ( x + h ) - F ( x ) = \int _ { x } ^ { x + h } f } \end{array}$ dm Rfor fixed $[ x , x + h ] \subset ( a , b )$ 

We turn to showing that Lebesgue’s theory extends that of Riemann: 

## Theorem 4.23

Let $f : \left[ a , b \right] \mapsto \mathbb { R }$ be bounded. 

(i) f is Riemann-integrable if and only if f is a.e. continuous with respect to Lebesgue measure on $[ a , b ]$ 

(ii) Riemann integrable functions on $[ a , b ]$ are integrable with respect to Lebesgue measure on $[ a , b ]$ and the integrals are the same. 

## Proof

We need to prepare a little for the proof by recalling notation and some basic facts. Recall from Chapter 1 that any partition 

$$
\mathcal {P} = \left\{a _ {i}: a = a _ {0} <   a _ {1} <   \dots <   a _ {n} = b \right\}
$$

of the interval $[ a , b ]$ , with $\varDelta _ { i } = a _ { i } - a _ { i - 1 } \ ( i = 1 , 2 , \ldots , n )$ and with $M _ { i }$ (resp. $m _ { i } )$ the sup (resp. inf) of f on $I _ { i } = [ a _ { i - 1 } , a _ { i } ]$ , induces upper and lower Riemann sums $\begin{array} { r } { U _ { \mathcal { P } } = \sum _ { i = 1 } ^ { n } M _ { i } \varDelta _ { i } } \end{array}$ and $\begin{array} { r } { L _ { \mathcal { P } } = \sum _ { i = 1 } ^ { n } m _ { i } \varDelta _ { i } } \end{array}$ . But these are just the Lebesgue Pintegrals of the simple functions $\begin{array} { r } { u _ { \mathcal { P } } = \sum _ { i = 1 } ^ { n } M _ { i } \mathbf { 1 } _ { I _ { i } } } \end{array}$ and $\begin{array} { r } { l _ { \mathcal { P } } = \sum _ { i = 1 } ^ { n } m _ { i } \mathbf { 1 } _ { I _ { i } } } \end{array}$ , by Pdefinition of the integral for such functions. 

Choose a sequence of partitions $\left( \mathcal { P } _ { n } \right)$ such that each $\mathcal { P } _ { n + 1 }$ refines $\mathcal { P } _ { n }$ and the length of the largest subinterval in $\mathcal { P } _ { n }$ goes to 0; writing $u _ { n }$ for $u _ { \mathcal { P } _ { n } }$ and $l _ { n }$ for $l _ { \mathcal { P } _ { r } }$ we have $l _ { n } \ \leq \ f \ \leq \ u _ { n }$ for all n. Apply this on the measure space $( [ a , b ] , \mathcal { M } _ { [ a , b ] } , m )$ where $m = m _ { [ a , b ] }$ denotes Lebesgue measure restricted to $[ a , b ]$ . Then $u = \operatorname* { i n f } _ { n } u _ { n }$ and $l = \operatorname* { s u p } _ { n } l _ { n }$ are measurable functions, and both sequences are monotone, since 

$$
l _ {1} \leq l _ {2} \leq \ldots \leq f \leq \ldots \leq u _ {2} \leq u _ {1}.\tag{4.3}
$$

Thus $u = \operatorname* { l i m } _ { n } u _ { n }$ and $l = \operatorname* { l i m } _ { n } l _ { n }$ (pointwise) and all functions in (4.3) are bounded on $[ a , b ]$ by $M = \operatorname* { s u p } \{ f ( x ) : x \in [ a , b ] \}$ , which is integrable on $[ a , b ]$ By dominated convergence we conclude that 

$$
\lim _ {n} U _ {n} = \lim _ {n} \int_ {a} ^ {b} u _ {n} \mathrm{d} m = \int_ {a} ^ {b} u \mathrm{d} m, \quad \lim _ {n} L _ {n} = \lim _ {n} \int_ {a} ^ {b} l _ {n} \mathrm{d} m = \int_ {a} ^ {b} l \mathrm{d} m
$$

and the limit functions u and l are (Lebesgue-)integrable. 

Now suppose that x is not an endpoint of any of the intervals in the partitions $\left( \mathcal { P } _ { n } \right) ~ -$ which excludes only countably many points of $[ a , b ]$ . Then we have: 

$$
f \text {   is   continuous   at   } x \text {   iff   } u (x) = f (x) = l (x).
$$

This follows at once from the definition of continuity, since the length of each subinterval approaches 0 and so the variation of $f$ over the intervals containing x approaches 0 if f is continuous at x. 

The Riemann integral $\textstyle \int _ { a } ^ { b } f ( x )$ dx was defined as the common value of $\begin{array} { r } { \operatorname* { l i m } _ { n } U _ { n } = \int _ { a } ^ { b } } \end{array}$ u dm and $\begin{array} { r } { \operatorname* { l i m } _ { n } L _ { n } = \int _ { a } ^ { b } } \end{array}$ ldm whenever these limits are equal. 

To prove (i), assume first that f is Riemann-integrable, so that the upper and lower integrals coincide: $\begin{array} { r } { \int _ { a } ^ { b } u \mathrm { d } \dot { m } = \int _ { a } ^ { b } l \mathrm { d } m } \end{array}$ . But $l \leq f \leq u$ , hence $\int _ { a } ^ { b } ( u -$ $l ) \mathrm { d } m = 0$ means that $u = l = f { \mathrm { ~ a . e ~ } }$ . by Theorem 4.15. Hence f is continuous a.e. by the above characterization of continuity of f at x, which only excludes a further null set of partition points. 

Conversely, if $f$ is a.e. continuous, then $u = f = l { \mathrm { ~ a . e ~ } }$ . and u and l are Lebesgue-measurable, hence so is $f$ (note that this uses the completeness of Lebesgue measure!). But $f$ is also bounded by hypothesis, so it is Lebesgueintegrable over $[ a , b ]$ , and as the integrals are a.e. equal, the integrals coincide (but note that ${ \bar { \int _ { a } ^ { b } } } f$ dm denotes the Lebesgue integral of f!): 

$$
\int_ {a} ^ {b} l \mathrm{d} m = \int_ {a} ^ {b} f \mathrm{d} m = \int_ {a} ^ {b} u \mathrm{d} m.\tag{4.4}
$$

Since the outer integrals are the same, $f$ is by definition also Riemannintegrable, which proves (i). 

To prove (ii), note simply that if f is Riemann-integrable, (i) shows that $f$ is a.e. continuous, hence measurable, and then (4.4) shows that its Lebesgue integral coincides with the two outer integrals, hence with its Riemann integral. □ 

## Example 4.6

Recall the following example from Section 1.2: Dirichlet’s function defined on [0, 1] by 

$$
f (x) = \left\{ \begin{array}{l l} \frac {1}{n} & \text { if } x = \frac {m}{n} \in \mathbb {Q} \\ 0 & \text { if } x \notin \mathbb {Q} \end{array} \right.
$$

is a.e. continuous, hence Riemann-integrable, and its Riemann integral equals its Lebesgue integral, which is 0, since $f$ is zero outside the null set $\mathbb { Q } .$ 

We have now justified the unproven claims made in earlier examples when evaluating integrals, since, at least for any continuous functions on bounded intervals, the techniques of elementary calculus also give the Lebesgue integrals of the functions concerned. Since the integral is additive over disjoint domains use of these techniques also extends to piecewise continuous functions. 

## Example 4.7 (Improper Riemann Integrals)

Dealing with improper Riemann integrals involves an additional limit opera-

tion; we define such an integral by: 

$$
\int_ {- \infty} ^ {\infty} f (x) \mathrm{d} x := \lim _ {a \to - \infty , b \to \infty} \int_ {a} ^ {b} f (x) \mathrm{d} x
$$

whenever the double limit exists. (Other cases of ‘improper integrals’ are discussed in Remark 4.2.) 

Now suppose for the function $f : \mathbb { R } \mapsto \mathbb { R }$ this improper Riemann integral exists. Then the Riemann integral $\textstyle \int _ { a } ^ { b } f ( x )$ dx exists for each bounded interval $[ a , b ]$ R, so that f is a.e. continuous on each $[ a , b ]$ , and thus on R. The converse is false, however: the function f which takes the value 1 on $[ n , n + 1 )$ when n is even, and 1 when n is odd, is a.e. continuous (and thus Lebesgue measurable on R) but clearly the above limits fail to exist. 

More generally, it is not hard to show that if $f \in { \mathcal { L } } ^ { 1 } ( \mathbb { R } )$ then the above double limits will always exist. On the other hand, the existence of the double limit does not by itself guarantee that $f \in \mathcal { L } ^ { 1 }$ without further conditions: consider 

$$
f (x) = \left\{ \begin{array}{l l} \frac {(- 1) ^ {n}}{n + 1} & \text { if } x \in [ n, n + 1), n \geq 0 \\ 0 & \text { if } x <   0. \end{array} \right.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/d0279c21c118ed7976f2d493a573f2d8ccb8ec74df189b2e4cd6c91b13390e38.jpg)



Figure 4.3 Graph of f


Clearly the improper Riemann integral exists, 

$$
\int_ {- \infty} ^ {\infty} f (x) \mathrm{d} x = \sum_ {n = 0} ^ {\infty} \frac {(- 1) ^ {n}}{n + 1}
$$

and the series converges. However, f $\notin \mathcal { L } ^ { 1 }$ , since $\begin{array} { r } { \int _ { \mathbb { R } } \left| f \right| \mathrm { d } m = \sum _ { n = 0 } ^ { \infty } \frac { 1 } { n + 1 } } \end{array}$ , which diverges. 

This yields another illustration of the ‘absolute’ nature of the Lebesgue integral: $f \in { \mathcal { L } } ^ { 1 } \operatorname { i f f } | f | \in { \mathcal { L } } ^ { 1 }$ , so we cannot expect a finite sum for an integral whose ‘pieces’ make up a conditionally convergent series. For non-negative functions these problems do not arise; we have: 

## Theorem 4.24

If $f \geq 0$ and the above improper Riemann integral of f exists, then the Lebesgue integral $\textstyle \int _ { \mathbb { R } } f$ dm always exists and equals the improper integral. 

## Proof

To see this, simply note that the sequence $\left( f _ { n } \right)$ with $f _ { n } = f \mathbf { 1 } _ { [ - n , n ] }$ increases monotonically to $f ,$ hence $f$ is Lebesgue-measurable. Since $f _ { n }$ is Riemannintegrable on $[ - n , n ]$ , the integrals coincide there, i.e. 

$$
\int_ {\mathbb {R}} f _ {n} \mathrm{d} m = \int_ {- n} ^ {n} f (x) \mathrm{d} x
$$

for each $n ,$ so that $f _ { n } \in \mathcal { L } ^ { 1 } ( \mathbb { R } )$ for all n. By hypothesis the double limit 

$$
\lim _ {n} \int_ {- n} ^ {n} f (x) \mathrm{d} x = \int_ {- \infty} ^ {\infty} f (x) \mathrm{d} x
$$

exists. On the other hand 

$$
\lim _ {n} \int_ {\mathbb {R}} f _ {n} \mathrm{d} m = \int_ {\mathbb {R}} f \mathrm{d} m
$$

by monotone convergence, and so $f \in { \mathcal { L } } ^ { 1 } ( \mathbb { R } )$ and 

$$
\int_ {\mathbb {R}} f \mathrm{d} m = \int_ {- \infty} ^ {\infty} f (x) \mathrm{d} x
$$

as required. 

## Exercise 4.10

Show that the function f given by $\textstyle f ( x ) = { \frac { \sin x } { x } } \left( x \neq 0 \right)$ has an improper Riemann integral over R, but is not in $\mathcal { L } ^ { 1 }$ 

## Remark 4.2

A second kind of improper Riemann integral is designed to handle functions which have asymptotes on a bounded interval, such as $\begin{array} { r } { f ( x ) = \frac { 1 } { x } \mathrm { ~ o n ~ } ( 0 , 1 ) } \end{array}$ . For such cases we can define 

$$
\int_ {a} ^ {b} f (x) \mathrm{d} x = \lim _ {\varepsilon \searrow 0} \int_ {a + \varepsilon} ^ {b} f (x) \mathrm{d} x
$$

when the limit exists. (Similar remarks apply to the upper limit of integration.) 

## 4.6 Approximation of measurable functions

The previous section provided an indication of the extent of the additional ‘freedom’ gained by developing the Lebesgue integral: Riemann integration binds us to functions whose discontinuities form an m-null set, while we can still find the Lebesgue integral of functions that are nowhere continuous, such as $\mathbf { 1 } _ { \mathbb { Q } }$ . We may ask, however, how real this additional generality is: can we, for example, approximate an arbitrary $f \in \mathcal { L } ^ { 1 }$ by continuous functions? In fact, since continuity is a local property, can we do this for arbitrary measurable functions? And this, in turn, provides a link with simple functions, since every measurable function is a limit of simple functions. We can go further, and ask whether for a simple function g approximating a given measurable function f we can choose the inverse image $g ^ { - 1 } ( \{ a _ { i } \} )$ of each element of the range of $g$ to be an interval (such a g is usually called a step function; $\begin{array} { r } { g = \sum _ { n } c _ { n } \mathbf { 1 } _ { I _ { n } } } \end{array}$ , where $I _ { n }$ are intervals). We shall tackle this question first: 

## Theorem 4.25

If f is a bounded measurable function on $[ a , b ]$ and $\varepsilon > 0$ is given, then there exists a step function h such that $\textstyle \int _ { a } ^ { b } | f - h | \mathrm { d } m < \varepsilon$ 

## Proof

First assume additionally that $f \geq 0$ . Then $\textstyle \int _ { a } ^ { b } f$ dm is well-defined as 

$$
\sup \left\{\int_ {a} ^ {b} \varphi \mathrm{d} m: 0 \leq \varphi \leq f, \text {   simple } \right\}.
$$

Since $f \geq \varphi$ we have $| f - \varphi | = f - \varphi$ , so we can find a simple function $\varphi$ satisfying 

$$
\int_ {a} ^ {b} | f - \varphi | \mathrm{d} m = \int_ {a} ^ {b} f \mathrm{d} m - \int_ {a} ^ {b} \varphi \mathrm{d} m <   \frac {\varepsilon}{2}.
$$

It then remains to approximate an arbitrary simple function $\varphi$ which vanishes of $[ a , b ]$ by a step function h. The finite range $\{ a _ { 1 } , a _ { 2 } , . . . , a _ { n } \}$ of the function $\varphi$ partitions $[ a , b ]$ , yielding disjoint measurable sets $E _ { i } = \varphi ^ { - 1 } ( \{ a _ { i } \} )$ such that $\textstyle \bigcup _ { i = 1 } ^ { n } E _ { i } = [ a , b ]$ . We now approximate each $E _ { i }$ by intervals: note that since $\varphi$ Sis simple, $M = \operatorname* { s u p } \{ \varphi ( x ) : x \in [ a , b ] \} < \infty$ . By Theorem 2.12 we can find open sets $O _ { i }$ such that $E _ { i } \subset O _ { i }$ and $\begin{array} { r } { m ( O _ { i } \setminus E _ { i } ) < \frac { \varepsilon } { 2 n M } } \end{array}$ for $i \leq n$ . Since each $E _ { i }$ has finite measure, so do the $O _ { i }$ , hence each $O _ { i }$ can in turn be approximated by a finite union of disjoint open intervals: we know that $\textstyle O _ { i } = \bigcup _ { j = 1 } ^ { \infty } I _ { i j }$ , where the open intervals can be chosen disjoint, so that $\begin{array} { r } { m ( O _ { i } ) = \sum _ { j = 1 } ^ { \infty ^ { \circ } } m ( I _ { i j } ) < \infty } \end{array}$ . As the series converges, we can find $k _ { i }$ such that $\begin{array} { r } { m ( O _ { i } ) - m ( \bigcup _ { j = 1 } ^ { k _ { i } } I _ { i j } ) < \frac { \varepsilon } { 2 n M } } \end{array}$ . Thus with $\begin{array} { r } { G _ { i } = \bigcup _ { j = 1 } ^ { k _ { i } } I _ { i j } } \end{array}$ we have $\begin{array} { r } { \int _ { a } ^ { b } | \mathbf { 1 } _ { E _ { i } } - \mathbf { 1 } _ { G _ { i } } | \mathrm { d } m = m ( E _ { i } \varDelta G _ { i } ) < \frac { \varepsilon } { n M } } \end{array}$ for each $i \leq n$ . So set $\begin{array} { r } { h = \sum _ { i = 1 } ^ { n } a _ { i } \mathbf { 1 } _ { G _ { i } } } \end{array}$ . This step function satisfies $\textstyle \int _ { a } ^ { b } | \varphi - h | \mathrm { d } m < { \frac { \varepsilon } { 2 } }$ and hence $\textstyle \int _ { a } ^ { b } | f - h | \mathrm { d } m < \varepsilon$ 

The extension to general f is clear: $f ^ { + }$ and f−can be approximated to within $\frac { \varepsilon } { 2 }$ by step functions $h _ { 1 }$ and $h _ { 2 }$ say, so with $h = h _ { 1 } - h _ { 2 }$ we obtain 

$$
\int_ {a} ^ {b} | f - h | \mathrm{d} m \leq \int_ {a} ^ {b} | f ^ {+} - h _ {1} | \mathrm{d} m + \int_ {a} ^ {b} | f ^ {-} - h _ {2} | \mathrm{d} m <   \varepsilon
$$

which completes the proof. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/13cfac6d55bc757245f269e4c1cb68af89896e0ab8a90419ce7d39d1449c0c10.jpg)



Figure 4.4 Approximation by continuous functions


The ‘payof’ is now immediate: with f and h as above, we can reorder the intervals $I _ { i j }$ into a single finite sequence $( J _ { m } ) _ { m \leq n }$ with $J _ { m } = \left( c _ { m } , d _ { m } \right)$ and $h =$ $\textstyle \sum _ { m = 1 } ^ { n } a _ { m } \mathbf { 1 } _ { J _ { m } }$ . We may assume that $\begin{array} { r } { l ( J _ { m } ) = ( d _ { m } - c _ { m } ) > \frac { \varepsilon ^ { \prime } } { 2 } } \end{array}$ , and approximate ${ \mathbf { 1 } } _ { J _ { m } }$ by a continuous function $g _ { m }$ by setting $g _ { m } = 1$ on the slightly smaller interval $\begin{array} { r l r } {  { } } & { { } } & { ( c _ { m } + \frac { \varepsilon ^ { \prime } } { 4 } , d - \frac { \varepsilon ^ { \prime } } { 4 } ) } \end{array}$ and 0 outside $J _ { m }$ , while extending linearly in between (see Figure 4.4). It is obvious that $g _ { m }$ is continuous and $\begin{array} { r } { \int _ { a } ^ { b } | \mathbf { 1 } _ { J _ { m } } - g _ { m } | \mathrm { d } m < \frac { \varepsilon ^ { \prime } } { 2 } } \end{array}$ Repeating for each $J _ { m }$ and taking $\varepsilon ^ { \prime } < \frac { \varepsilon } { n K }$ , where $K = \operatorname* { m a x } _ { m \leq n } \left| a _ { m } \right|$ , shows that the continuous function $\begin{array} { r } { g \ = \ \sum _ { m = 1 } ^ { n } a _ { m } g _ { m } } \end{array}$ satisfies $\begin{array} { r } { \int _ { a } ^ { b } | h - g | \mathrm { d } m < \frac { \varepsilon } { 2 } } \end{array}$ PCombining this inequality with Theorem 4.25 yields: 

## Theorem 4.26

Given $f \in \mathcal { L } ^ { 1 }$ and $\varepsilon > 0$ , we can find a continuous function $g ,$ , vanishing outside some finite interval, such that $\textstyle { \int { | f - g | \mathrm { d } m } < \varepsilon }$ 

## Proof

The preceding argument has verified this when f is a bounded measurable function vanishing of some interval $[ a , b ]$ . For a given $f \in \mathcal { L } ^ { 1 } [ a , b ]$ we can again assume without loss that $f \geq 0$ . Let $f _ { n } = \operatorname* { m i n } ( f , n )$ ; Then the $f _ { n }$ are bounded measurable functions dominated by $f , f _ { n } \to f ,$ so that $\begin{array} { r } { \int _ { a } ^ { b } | f - \mathbf { \dot { f } } _ { N } | \mathrm { d } m < \frac { \varepsilon } { 2 } } \end{array}$ for some N. We can now find a continuous $^ { g , }$ Rvanishing outside a finite interval, such that $\textstyle \int _ { a } ^ { b } | f _ { N } - g |$ dm $< \frac { \varepsilon } { 2 }$ . Thus $\begin{array} { r } { \int _ { a } ^ { b } | f - g | \mathrm { d } m < \varepsilon } \end{array}$ 

RFinally, let $f \in { \mathcal { L } } ^ { 1 } ( \mathbb { R } )$ and $f \geq 0$ Rbe given. Choose n large enough to ensure that $\int _ { \{ | x | \geq n \} }$ f dm $< \frac { \varepsilon } { 3 }$ (which we can do as $\textstyle \int _ { \mathbb { R } } | f |$ dm is finite; Proposition 4.19), and simultaneously choose a continuous g with $\begin{array} { r } { \int _ { \{ | x | \geq n \} } g \mathrm { d } m < \frac { \varepsilon } { 3 } } \end{array}$ which satisfies $\textstyle \int _ { - n } ^ { n } | f - g | \mathrm { d } m < { \frac { \varepsilon } { 3 } }$ . Thus $\textstyle \int _ { \mathbb { R } } | f - g | \mathrm { d } m < \varepsilon$ □ 

The well-known Riemann-Lebesgue lemma, which is very useful in the discussion of Fourier series, is easily deduced from the above approximation theorems: 

## Lemma 4.27 (Riemann-Lebesgue)

Suppose $f \in { \mathcal { L } } ^ { 1 } ( \mathbb { R } )$ . Then the sequences $\begin{array} { r } { s _ { k } = \int _ { - \infty } ^ { \infty } f ( x ) } \end{array}$ sin kx dx and $c _ { k } =$ $\textstyle \int _ { - \infty } ^ { \infty } f ( x )$ cos kx dx both converge to 0 as $k \to \infty$ 

## Proof

We prove this for $\left( \boldsymbol { s } _ { k } \right)$ leaving the other, similar, case to the reader. For simplicity of notation write for $\int _ { - \infty } ^ { \infty }$ . The transformation $\textstyle x = y + { \frac { \pi } { k } }$ shows that 

$$
s _ {k} = \int f (y + \frac {\pi}{k}) \sin (k y + \pi) \mathrm{d} y = - \int f (y + \frac {\pi}{k}) \sin (k y) \mathrm{d} y.
$$

Since sin $x | \le 1$ 2 

$$
\int | f (x) - f (x + \frac {\pi}{k}) | \mathrm{d} x \geq | \int (f (x) - f (x + \frac {\pi}{k})) \sin k x \mathrm{d} x | = 2 | s _ {k} |.
$$

It will therefore sufice to prove that $\begin{array} { r } { \int | f ( x ) - f ( x + h ) | \mathrm { d } x \to 0 } \end{array}$ when $h  0$ RThis is most easily done by approximating $f$ by a continuous g which vanishes outside some finite interval $[ a , b ]$ , and such that $\textstyle \int | f - g | \mathrm { d } m < { \frac { \varepsilon } { 3 } }$ for a given $\varepsilon > 0$ . For $| h | < 1$ , the continuous function $g _ { h } ( x ) = g ( x + h )$ then vanishes of $[ a - 1 , b + 1 ]$ and 

$$
\int | f (x + h) - f (x) | \mathrm{d} m \leq \int | f (x + h) - g (x + h) | \mathrm{d} m
$$

$$
+ \int | g (x + h) - g (x) | \mathrm{d} m + \int | g (x) - f (x) | \mathrm{d} m.
$$

The first and last integrals on the right are less than $\frac { \varepsilon } { 3 }$ , while the integrand of the second can be made less than $\frac { \varepsilon } { 3 ( b - a + 2 ) }$ whenever $| h | < \delta$ , by an appropriate choice of $\delta > 0$ , as $g$ is continuous. As g vanishes outside $[ a - 1 , b + 1 ]$ , the second integral is also less than $\frac { \varepsilon } { 3 }$ . Thus if $\begin{array} { r } { | h | < \delta , \int | f ( x + h ) - f ( x ) \mathrm { d } m < \varepsilon } \end{array}$ This proves that lim $_ { k \to \infty } \int f ( x )$ sin $k x \mathrm { d } x = 0$ □ 

## 4.7 Probability

## 4.7.1 Integration with respect to probability distributions

Let X be a random variable with probability distribution $P _ { X }$ . The following theorem shows how to perform a change of variable when integrating a function of X. In other words, it shows how to change the measure in an integral. This is fundamental in applying integration theory to probabilities. We emphasize again that only the closure properties of σ-fields and the countable additivity of measures are needed for the theorems we shall apply here, so that we can use an abstract formulation of a probability space $( \varOmega , \mathcal { F } , P )$ in discussing their applications. 

## Theorem 4.28

Given a random variable $X : \varOmega \to \mathbb { R }$ 2 

$$
\int_ {\Omega} g (X (\omega)) \mathrm{d} P (\omega) = \int_ {\mathbb {R}} g (x) \mathrm{d} P _ {X} (x).\tag{4.5}
$$

## Proof

We employ the technique described in Remark 4.1. For the indicator function $g = \mathbf { 1 } _ { A }$ we have $P ( X \in A )$ on both sides. Then by linearity we have the result for simple functions. Approximation of non-negative measurable g by a monotone sequence of simple functions combined with the monotone convergence theorem gives the equality for such $g .$ . The case of general $g \in \mathcal { L } ^ { 1 }$ follows as before from the linearity of the integral, using $g = g ^ { + } - g ^ { - }$ □ 

The formula is useful in the case where the form of $P _ { X }$ is known and allows one to carry out explicit computations. 

Before we proceed to these situations, consider a very simple case as an illustration of the formula. Suppose that X is constant, i.e. $X ( \omega ) \equiv a$ . Then on the left in (4.5) we have the integral of a constant function, which equals $g ( a ) P ( \varOmega ) = g ( a )$ according to the general scheme of integrating indicator functions. On the right $P _ { X } = \delta _ { a }$ and thus we have a method of computing an integral with respect to Dirac measure: $\begin{array} { r } { \int g ( x ) \mathrm { d } \delta _ { a } = g ( a ) } \end{array}$ 

For discrete $X$ taking values $a _ { i }$ Rwith probabilities $p _ { i }$ we have 

$$
\int g (X) \mathrm{d} P = \sum_ {i} g (a _ {i}) p _ {i}
$$

which is a well-known formula from elementary probability theory (see also Section 3.5.3). In this case we have $\begin{array} { r } { P _ { X } = \sum _ { i } p _ { i } \delta _ { a _ { i } } } \end{array}$ and on the right, the integral Pwith respect to the combination of measures is the combination of the integrals: 

$$
\int g (x) \mathrm{d} P _ {X} = \sum_ {i} p _ {i} \int g (x) \mathrm{d} \delta_ {a _ {i}} (x).
$$

In fact, this is a general property. 

## Theorem 4.29

If $\begin{array} { r } { P _ { X } = \sum _ { i } p _ { i } P _ { i } } \end{array}$ , where the $P _ { i }$ are probability measures, $\sum p _ { i } = 1 , p _ { i } \ge 0$ , then 

$$
\int g (x) \mathrm{d} P _ {X} (x) = \sum_ {i} p _ {i} \int g (x) \mathrm{d} P _ {i}.
$$

## Proof

The method is the same as above: first consider indicator functions $\mathbf { 1 } _ { A }$ and the claim is just the definition of $P _ { X }$ : on the left we have $P _ { X } ( A )$ , on the right $\textstyle \sum _ { i } p _ { i } P _ { i } ( A )$ . Then by additivity we get the formula for simple functions, and Pfinally, approximation and use of the monotone convergence theorem completes the proof as before. □ 

## 4.7.2 Absolutely continuous measures: examples of densities

The measures P of the form 

$$
A \mapsto P (A) = \int_ {A} f \mathrm{d} m
$$

with non-negative integrable f will be called absolutely continuous, and the function f will be called a density of P with respect to Lebesgue measure, or simply a density. Clearly, for P to be a probability we have to impose the condition 

$$
\int f \mathrm{d} m = 1.
$$

Students of probability often have an oversimplified mental picture of the world of random variables, believing that a random variable is either discrete or absolutely continuous. This image stems from the practical computational approach of many elementary textbooks, which present probability without the necessary background in measure theory. We have already provided a simple example which shows this to be a false dichotomy (Example 3.1). 

The simplest example of a density is this: let $\Omega \subset \mathbb { R }$ be a Borel set with finite Lebesgue measure and put 

$$
f (x) = \left\{ \begin{array}{l l} \frac {1}{m (\varOmega)} & \text { if } x \in \varOmega \\ 0 & \text { otherwise. } \end{array} \right.
$$

We have already come across this sort of measure in the previous chapter, that is, the probability distribution of a specific random variable. We say that in this case the measure (distribution) is uniform. It corresponds to the case where the values of the random variable are spread evenly across some set, typically an interval, such as in choosing a number at random (Example 2.2). 

Slightly more complicated is the so-called triangle distribution with the density of the form shown in Figure 4.5. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/143f3f82d567d98a638804072de22b4719b8afb80930fe86fa1963790a28cd02.jpg)



Figure 4.5 Triangle distribution


The most famous is the Gaussian or normal density 

$$
n (x) = \frac {1}{\sqrt {2 \pi} \sigma} \mathrm{e} ^ {- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}}.\tag{4.6}
$$

This function is symmetric with respect to $x = \mu$ , and vanishes at infinity, i.e. $\begin{array} { r } { \operatorname* { l i m } _ { x  - \infty } n ( x ) = 0 = \operatorname* { l i m } _ { x  \infty } n ( x ) } \end{array}$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/72af2982f6c581dc147f63c2a41364e8d08706c91b6e06795e9f35c4494df10f.jpg)



Figure 4.6 Gaussian distribution


Exercise 4.11 

Show that $\textstyle \int _ { - \infty } ^ { \infty } n ( x ) \mathrm { d } x = 1$ 

Hint First consider the case $\mu = 0 , \sigma = 1$ and then transform the general case to this. 

The meaning of the number $\mu$ will become clear below and $\sigma$ will be explained in the next chapter. 

Another widely used example is the Cauchy density: 

$$
c (x) = \frac {1}{\pi} \frac {1}{1 + x ^ {2}}.
$$

This density gives rise to many counterexamples to ‘theorems’ which are too good to be true. 

Exercise 4.12 

Show that $\textstyle \int _ { - \infty } ^ { \infty } c ( x ) \mathrm { d } x = 1$ 

The exponential density is given by 

$$
f (x) = \left\{ \begin{array}{l l} c \mathrm{e} ^ {- \lambda x} & \text {if} x \geq 0 \\ 0 & \text {otherwise.} \end{array} \right.
$$

Exercise 4.13 

Find the constant c for f to be a density of probability distribution. 

The gamma distribution is really a large family of distributions, indexed by a parameter $t > 0$ . It contains the exponential distribution as the special case where $t = 1$ . Its density is defined as 

$$
f (x) = \left\{ \begin{array}{l l} \frac {1}{\Gamma (t)} \lambda^ {t} x ^ {t - 1} \mathrm{e} ^ {- \lambda x} & \text { if } x \geq 0 \\ 0 & \text { otherwise } \end{array} \right.
$$

where the gamma function $\textstyle T ( t ) = \int _ { 0 } ^ { \infty } x ^ { t - 1 } \mathrm { e } ^ { - x }$ dx. 

RThe gamma distribution contains another widely used distribution as a special case: the distribution obtained from the density f when $\begin{array} { r } { \lambda = \frac { 1 } { 2 } \operatorname { a n d } t = \frac { d } { 2 } } \end{array}$ for some $d \in \mathbb { N }$ is denoted by $\chi ^ { 2 } ( d )$ and called the chi-squared distribution with d degrees of freedom. 

The (cumulative) distribution function corresponding to a density is given by 

$$
F (y) = \int_ {- \infty} ^ {y} f (x) \mathrm{d} x.
$$

If f is continuous then F is diferentiable and $F ^ { \prime } ( x ) = f ( x )$ by the Fundamental Theorem of Calculus (see Proposition 4.22). We say that $F$ is absolutely continuous if this relation holds with integrable f, and then $f$ is the density of the probability measure induced by F. The following example due to Lebesgue shows that continuity of F is not suficient for the existence of a density. 

## Example 4.8

Recall the Lebesgue function F define on page 20. We have $F ( y ) = 0$ for $y \le 0$ 2 $F ( y ) = 1$ for $\textstyle y \geq 1 , F ( y ) = { \frac { 1 } { 2 } }$ for $\begin{array} { r } { y \in [ \frac { 1 } { 3 } , \frac { 2 } { 3 } ) , F ( y ) = \frac { 1 } { 4 } } \end{array}$ for $\begin{array} { r } { y \in [ \frac { 1 } { 9 } , \frac { 2 } { 9 } ) , F ( y ) = \frac { 3 } { 4 } } \end{array}$ for $y \in [ \frac { 7 } { 9 } , \frac { 8 } { 9 } )$ and so on. The function F is constant on the intervals removed in the process of constructing the Cantor set. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/704792eee7127e33a04652a4e615344a5b7812a05d77b70155df34bedf7da5a7.jpg)



Figure 4.7 Lebesgue’s function


It is diferentiable almost everywhere and the derivative is zero. So $F$ cannot be absolutely continuous since then $f$ would be zero almost everywhere, but on the other hand its integral is 1. 

We now define the (cumulative) distribution function of a random variable $X : \varOmega \to \mathbb { R }$ , where, as above, $( \varOmega , \mathcal { F } , P )$ is a given probability space: 

$$
F _ {X} (y) = P (\{\omega : X (\omega) \leq y \}) = P _ {X} ((- \infty , y ]).
$$

## Proposition 4.30

(i) $F _ { X }$ is non-decreasing $( y _ { 1 } \le y _ { 2 }$ implies $F _ { X } ( y _ { 1 } ) \leq F _ { X } ( y _ { 2 } ) )$ 

(ii) $\begin{array} { r } { \operatorname* { l i m } _ { y \to \infty } F _ { X } ( y ) = 1 , \operatorname* { l i m } _ { y \to - \infty } F _ { X } ( y ) = 0 , } \end{array}$ 

(iii) $F _ { X }$ is right continuous $( { \mathrm { i f ~ } } y \to y _ { 0 } , y \geq y _ { 0 }$ , then $F _ { X } ( y ) \to F ( y _ { 0 } ) )$ 

Exercise 4.14 

Show that $F _ { X }$ is continuous if and only if $P _ { X } ( \{ y \} ) = 0$ for all $y .$ 

Exercise 4.15 

Find $F _ { X }$ for 

(a) a constant random variable X, $X ( \omega ) = a$ for all $\omega$ 

(b) $X : [ 0 , 1 ] \to \mathbb { R }$ given by $X ( \omega ) = \operatorname* { m i n } \{ \omega , 1 - \omega \}$ (the distance to the nearest endpoint of the interval [0, 1]) 

(c) $X : [ 0 , 1 ] ^ { 2 } \to \mathbb { R }$ , the distance to the nearest edge of the square $[ 0 , 1 ] ^ { 2 }$ 

The fact that we are doing probability on subsets of $\mathbb { R } ^ { n }$ as sample spaces turns out to be not restrictive. In fact, the interval [0, 1] is suficient as the following Skorokhod representation theorem shows. 

## Theorem 4.31

If a function $F : \mathbb { R } \to [ 0 , 1 ]$ satisfies conditions (i)–(iii) of Proposition 4.30, then there is a random variable defined on the probability space $( [ 0 , 1 ] , B , m _ { [ 0 , 1 ] } )$ $X : [ 0 , 1 ]  \mathbb { R }$ , such that $F = F _ { X }$ 

Proof 

We write, for $\omega \in [ 0 , 1 ]$ 

$$
X ^ {+} (\omega) = \inf \{x: F (x) > \omega \}, \quad X ^ {-} (\omega) = \sup \{x: F (x) <   \omega \}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/a7f5f7301c0f7c7719ddaa1cbd0adf5970cae2d779cc7a5349b0148efaa25a7d.jpg)



Figure 4.8 Construction of $X ^ { - } ;$ ; continuity point


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/06b8f5a8c3f4213ce7009e8fdfa66b6f64b98afce6a48b89b8cde9f0e04afb79.jpg)



Figure 4.9 Construction of $X ^ { - }$ ; discontinuity point


Three possible cases are illustrated in Figures 4.8, 4.9 and 4.10. We show that $F _ { X ^ { - } } = F$ , and for that we have to show that $F ( y ) = m ( \{ \omega : X ^ { - } ( \omega ) \leq y \} )$ The set $\lbrace \omega : X ^ { - } ( \omega ) \leq y \rbrace$ is an interval with left endpoint 0. We are done if we show that its right endpoint is $F ( y )$ , i.e. if $X ^ { - } ( \omega ) \leq y$ is equivalent to $\omega \leq F ( y )$ 

Suppose that $\omega \leq F ( y )$ . Then 

$$
\{x: F (x) <   \omega \} \subset \{x: F (x) <   F (y) \} \subset \{x: x \leq y \}
$$

(the last inclusion by the monotonicity of $F )$ , hence $X ^ { - } ( \omega ) = \operatorname* { s u p } \{ x : F ( x ) <$ $\omega \} \leq y .$ 

Suppose that $X ^ { - } ( \omega ) \leq y$ . By monotonicity $F ( X ^ { - } ( \omega ) ) \leq F ( y )$ . By the rightcontinuity of $F , \omega \leq F ( X ^ { - } ( \omega ) ) { \mathrm { ~ ( i f ~ } } \omega > F ( X ^ { - } ( \omega ) )$ , then there is $x _ { 0 } > X ^ { - } ( \omega )$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/8d868cc12598e24d3498774ad0ec9a41bb8e5088973a39af76857e2dd95f61dd.jpg)



Figure 4.10 Construction of $X ^ { - } ; \thinspace \mathrm { { \cdot \mathrm { { \mathrm { { f l a t } } } } } } $ piece


such that $F ( X ^ { - } ( \omega ) ) < F ( x _ { 0 } ) < \omega .$ , which is impossible since $x _ { 0 }$ is in the set whose supremum is taken to get $X ^ { - } ( \omega ) )$ so $\omega \leq F ( y )$ 

For future use we also show that $F _ { X ^ { + } } = F$ . It is suficient to see that $m ( \{ \omega$ $X ^ { - } ( \omega ) < X ^ { + } ( \omega ) \} ) = 0$ (which is intuitively clear as this may happen only when the graph of $F$ is $\mathrm { \hbar \hbar \mathrm { a t } } ^ { \prime }$ , and there are countably many values corresponding to the ‘flat’ pieces, their Lebesgue measure being zero). More rigorously, 

$$
\{\omega : X ^ {-} (\omega) <   X ^ {+} (\omega) \} = \bigcup_ {q \in \mathbb {Q}} \{\omega : X ^ {-} (\omega) \leq q <   X ^ {+} (\omega) \}
$$

and $m ( \{ \omega : X ^ { - } ( \omega ) \leq q < X ^ { + } ( \omega ) \} ) = m ( \{ \omega : X ^ { - } ( \omega ) \leq q \} \setminus \{ \omega : X ^ { + } ( \omega ) \leq q \} )$ $q \} ) = F ( q ) - F ( q ) = 0$ □ 

The following theorem provides a powerful method for calculating integrals relative to absolutely continuous distributions. The result holds for general measures but we formulate it for a probability distribution of a random variable in order not to overload or confuse the notation. 

## Theorem 4.32

If $P _ { X }$ defined on $\mathbb { R } ^ { n }$ is absolutely continuous with density $f _ { X } , g : \mathbb { R } ^ { n } \longrightarrow \mathbb { R }$ is integrable with respect to $P _ { X }$ , then 

$$
\int_ {\mathbb {R} ^ {n}} g (x) \mathrm{d} P _ {X} (x) = \int_ {\mathbb {R} ^ {n}} f _ {X} (x) g (x) \mathrm{d} x.
$$

## Proof

For an indicator function $g ( x ) = \mathbf { 1 } _ { A } ( x )$ we have $P _ { X } ( A )$ on the left which equals $\textstyle \int _ { A } f _ { X } ( x )$ dx by the form of $P ,$ and consequently is equal to $\begin{array} { r } { \int _ { \mathbb { R } ^ { n } } \mathbf { 1 } _ { A } ( x ) f _ { X } ( x ) } \end{array}$ dx, i.e. the right-hand side. Extension to simple functions by linearity and to general integrable g by limit passage is routine. □ 

## Corollary 4.33

In the situation of the previous theorem we have 

$$
\int_ {\Omega} g (X) \mathrm{d} P = \int_ {\mathbb {R} ^ {n}} f _ {X} (x) g (x) \mathrm{d} x.
$$

## Proof

This is an immediate consequence of the above theorem and Theorem 4.28. 

We conclude this section with a formula for a density of a function of a random variable with given density. Suppose that $f _ { X }$ is known and we want to find the density of $Y = g ( X )$ 

## Theorem 4.34

If $g : \mathbb { R } \to \mathbb { R }$ is increasing and diferentiable (thus invertible), then 

$$
f _ {g (X)} (y) = f _ {X} (g ^ {- 1} (y)) \frac {\mathrm{d}}{\mathrm{d} y} g ^ {- 1} (y).
$$

## Proof

Consider the distribution function: 

$$
F _ {g (X)} (y) = P (g (X) \leq y) = P (X \leq g ^ {- 1} (y)) = F _ {X} (g ^ {- 1} (y)).
$$

Diferentiate with respect to y to get the result. 

## Remark 4.3

A similar result holds if g is decreasing. The same argument as above gives 

$$
f _ {g (X)} (y) = - f _ {X} \left(g ^ {- 1} (y)\right) \frac {\mathrm{d}}{\mathrm{d} y} g ^ {- 1} (y).
$$

## Example 4.9

If X has standard normal distribution 

$$
n (x) = \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} x ^ {2}}
$$

(i.e. $\mu = 0$ and $\sigma = 1$ in (4.6)), then the density of $Y = \mu + \sigma X$ is given by (4.6). This follows at once from Theorem 4.34: $\begin{array} { r } { g ^ { - 1 } ( y ) = \frac { \mu - x } { \sigma } } \end{array}$ ; its derivative is equal to $\textstyle { \frac { 1 } { \sigma } }$ . 

## Exercise 4.16

Find the density of $Y = X ^ { 3 }$ where $f _ { X } = \mathbf { 1 } _ { [ 0 , 1 ] }$ 

## 4.7.3 Expectation of a random variable

If X is a random variable defined on a probability space $( \varOmega , \mathcal { F } , P )$ then we introduce the following notation: 

$$
\mathbb {E} (X) = \int_ {\Omega} X \mathrm{d} P
$$

and we call this abstract integral the mathematical expectation of $X$ 

Using the results from the previous section we immediately have the following formulae: the expectation can be computed using the probability distribution: 

$$
\mathbb {E} (X) = \int_ {- \infty} ^ {\infty} x \mathrm{d} P _ {X} (x),
$$

and for absolutely continuous X we have 

$$
\mathbb {E} (X) = \int_ {- \infty} ^ {\infty} x f _ {X} (x) \mathrm{d} x.
$$

## Example 4.10

Suppose that $\begin{array} { r } { P _ { X } = \frac { 1 } { 2 } P _ { 1 } + \frac { 1 } { 2 } P _ { 2 } } \end{array}$ , where $P _ { 1 } = \delta _ { a } , P _ { 2 }$ has a density $f _ { 2 }$ . Then 

$$
\mathbb {E} (X) = \frac {1}{2} a + \frac {1}{2} \int x f (x) \mathrm{d} x.
$$

So, going back to Example 3.1 we can compute the expectation of the random variable considered there: 

$$
\mathbb {E} (X) = \frac {1}{2} \cdot 0 + \frac {1}{2} \frac {1}{2 5} \int_ {0} ^ {2 5} x \mathrm{d} x = 6. 2 5.
$$

## Exercise 4.17

Find the expectation of 

(a) a constant random variable X, $X ( \omega ) = a$ for all $\omega$ 

(b) $X : [ 0 , 1 ] \to \mathbb { R }$ given by $X ( \omega ) = \operatorname* { m i n } \{ \omega , 1 - \omega \}$ (the distance to the nearest endpoint of the interval [0, 1]) 

(c) $X : [ 0 , 1 ] ^ { 2 } \to \mathbb { R }$ , the distance to the nearest edge of the square $[ 0 , 1 ] ^ { 2 }$ 

## Exercise 4.18

Find the mathematical expectation of a random variable with 

(a) uniform distribution over the interval $[ a , b ]$ 

(b) triangle distribution, 

(c) exponential distribution. 

## 4.7.4 Characteristic function

In what follows we will need the integrals of some complex functions. The theory is a straightforward extension of the real case. 

Let $Z = X + \mathrm { i } Y$ where X, Y are real-valued random variables and define 

$$
\int Z \mathrm{d} P = \int X \mathrm{d} P + \mathrm{i} \int Y \mathrm{d} P.
$$

Clearly, linearity of the integral and the dominated convergence theorem hold for the complex case. Another important relation which remains true is: 

$$
\left| \int Z \mathrm{d} P \right| \leq \int | Z | \mathrm{d} P.
$$

To see this consider the polar decomposition of $\textstyle \int Z \mathrm { d } P = | \int Z \mathrm { d } P | \mathrm { e } ^ { - \mathrm { i } \theta }$ . Then, with $\Re ( z )$ Ras the real part of the complex number $z , | \int Z { \dot { \mathrm { d } } } P | = \mathrm { e } ^ { \mathrm { i } \theta } \int Z { \mathrm { d } } P =$ $\int \mathrm { e } ^ { \mathrm { i } \theta } Z \mathrm { d } P$ is real, hence equal to $\textstyle \int \Re ( \mathrm { e } ^ { \mathrm { i } \theta } Z ) \mathrm { d } P$ , but $\Re ( \mathrm { e } ^ { \mathrm { i } \theta } Z ) \le | \mathrm { e } ^ { \mathrm { i } \theta } Z | = | Z |$ and Rwe are done. 

The function we wish to integrate is exp itX where X is a real random variable, $t \in \mathbb { R }$ . Then 

$$
\int \exp \{\mathrm{i} t X \} \mathrm{d} P = \int \cos (t X) \mathrm{d} P + \mathrm{i} \int \sin (t X) \mathrm{d} P
$$

which always exists, by the boundedness of $x \mapsto \exp \{ { \mathrm { i } t x } \}$ 

## Definition 4.5

For a random variable X we write 

$$
\varphi_ {X} (t) = \mathbb {E} (\mathrm{e} ^ {\imath t X})
$$

for $t \in \mathbb { R }$ . We call $\varphi _ { X }$ the characteristic function of $X$ . 

To compute $\varphi _ { X }$ it is suficient to know the distribution of $X$ : 

$$
\varphi_ {X} (t) = \int \mathrm{e} ^ {\mathrm{i} t x} \mathrm{d} P _ {X} (x)
$$

and in the absolutely continuous case 

$$
\varphi_ {X} (t) = \int \mathrm{e} ^ {\mathrm{i} t x} f _ {X} (x) \mathrm{d} x.
$$

Some basic properties of the characteristic function are given below. Other properties are explored in Chapters 6 and 8. 

## Theorem 4.35

The function $\varphi _ { X }$ satisfies 

(i) $\varphi _ { X } ( 0 ) = 1 , | \varphi _ { X } ( t ) | \leq 1 $ 

(ii) $\varphi _ { a X + b } ( t ) = \operatorname { e } ^ { \mathrm { i } t b } \varphi _ { X } ( a t )$ 

## Proof

(i) The value at 0 is 1 since the expectation of the constant function is its value. The estimate follows from Proposition 4.16 (iii): $\begin{array} { r } { \left| \int \mathrm { e } ^ { \mathrm { i } t x } \mathrm { d } P _ { X } ( x ) \right| \le } \end{array}$ $\begin{array} { r } { \int | \mathrm { e } ^ { \mathrm { i } t x } | \mathrm { d } P _ { X } ( x ) = 1 } \end{array}$ 

R(ii) Here we use the linearity of the expectation: 

$$
\varphi_ {a X + b} (t) = \mathbb {E} (\mathrm{e} ^ {\imath t (a X + b)}) = \mathbb {E} (\mathrm{e} ^ {\imath t a X} \mathrm{e} ^ {\imath t b})) = \mathrm{e} ^ {\imath t b} \mathbb {E} (\mathrm{e} ^ {\imath (t a) X}) = \mathrm{e} ^ {\imath t b} \varphi_ {X} (t a),
$$

as required. 

## Exercise 4.19

Find the characteristic function of a random variable with 

(a) uniform distribution over the interval $[ a , b ]$ 

(b) exponential distribution, 

(c) Gaussian distribution. 

## 4.7.5 Applications to mathematical finance

Consider a derivative security of European type, that is, a random variable of the form $f ( S ( N ) )$ , where ${ \cal S } ( n ) , n = 1 , \ldots , N _ { ! }$ , is the price of the underlying security, which we call a stock for simplicity. (Or we write $f ( S ( T ) )$ , where the underlying security is described in continuous time $t \in [ 0 , T ]$ with prices $S ( t ) . )$ One of the crucial problems in finance is to find the price $Y ( 0 )$ of such a security. Here we assume that the reader is familiar with the following fact, which is true for certain specific models consisting of a probability space and random variables representing the stock prices: 

$$
Y (0) = \exp \{- r T \} \mathbb {E} (f (S (T))).\tag{4.7}
$$

where $r$ is the risk-free interest rate for continuous compounding. This will be explained in some detail in Section 7.4.3 but here we just want to draw some conclusions from this formula using the experience gathered in the present chapter. 

In particular, taking account of the form of the payof functions for the European call $( f ( x ) = ( x - K ) ^ { + } )$ and put $( f ( x ) = ( K - x ) ^ { + } )$ we have the following general formulae for the value of call and put, respectively: 

$$
\begin{array}{r} C = \exp \{- r T \} \mathbb {E} (S (T) - K) ^ {+}, \\ P = \exp \{- r T \} \mathbb {E} (K - S (T)) ^ {+}. \end{array}
$$

Without relying on any particular model one can prove the following relation, called call-put parity (see [4] for instance): 

$$
S (0) = C - P + K \exp \{- r T \}.\tag{4.8}
$$

## Proposition 4.36

The right hand side of the call-put parity identity is independent of K. 

## Remark 4.4

This proposition allows us to make an interesting observation, which is a version of a famous result in finance, namely the Miller-Modigliani theorem which says that the value of a company does not depend on the way it is financed. Let us very briefly recall that the value of a company is the sum of equity (represented by stock) and debt, so the theorem says that the level of debt has no impact on company’s value. Assume that the company borrowed $K \exp \{ - r T \}$ at the rate equal to r and it has to pay back the amount of K at time T. Should it fail, the company goes bankrupt. So the stockholders, who control the company, can ‘buy it back’ by paying K. This will make sense only if the value $S ( T )$ of the company exceeds K. The stock can be regarded as a call option so its value is C. The value of the debt is thus $K \exp \{ - r T \} - P ;$ less than the present value of K, which captures the risk that the sum K may not be recovered in full. 

We now evaluate the expectation to establish explicit forms of the general formula (4.7) in the two most widely used models. 

Consider first the binomial model introduced in Section 2.6.3. Assume that the probability space is equipped with a measure determined by the probability $\begin{array} { r } { p \ : = \ : \frac { R - D } { U - D } } \end{array}$ for the up movement in single step, where $R = \exp \{ r h \}$ , h being the length of one step. (This probability is called risk-neutral; observe that $\mathbb { E } ( \eta ) = R . )$ To ensure that $0 \leq p \leq 1$ we assume throughout that $D \leq R \leq U$ 

## Proposition 4.37

In the binomial model the price C of a call option with exercise time $T = h N$ is given by the Cox-Ross-Rubinstein formula 

$$
C = S (0) \Psi (A, N, p U \mathrm{e} ^ {- r T}) - K \mathrm{e} ^ {- r T} \Psi (A, N, p)
$$

where $\begin{array} { r } { \varPsi ( A , N , p ) = \sum _ { k = A } ^ { N } \binom { N } { k } p ^ { k } ( 1 - p ) ^ { N - k } } \end{array}$ and A is the first integer k such that $S ( 0 ) U ^ { k } D ^ { N - k } > K$ 

In the famous continuous-time Black-Scholes model, the stock price at time T is of the form 

$$
S (T) = S (0) \exp \{(r - \frac {\sigma^ {2}}{2}) T + \sigma w (T) \},
$$

where r is the risk-free rate, $\sigma > 0$ and $w ( T )$ is a random variable with Gaussian distribution with mean 0 and variance T. (The reader familiar with finance will notice that we again assume that the probability space is equipped with a risk-neutral measure.) 

## Proposition 4.38

We have the following Black-Scholes formula for $C$ : 

$$
C = S (0) N \left(d _ {1}\right) - K \mathrm{e} ^ {- r T} N \left(d _ {2}\right).
$$

where 

$$
d _ {1} = \frac {\ln \frac {S (0)}{K \mathrm{e} ^ {- r T}} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}} d _ {2} = \frac {\ln \frac {S (0)}{K \mathrm{e} ^ {- r T}} - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}.
$$

Exercise 4.20 

Find the formula for the put option. 

## 4.8 Proofs of propositions

## Proof (of Proposition 4.1)

Let $\begin{array} { r } { f = \sum c _ { i } \mathbf { 1 } _ { A _ { i } } } \end{array}$ . We have to show that 

$$
\sum c _ {i} m (A _ {i} \cap E) = \sup Y (E, f).
$$

First, we may take $\varphi = f$ in the definition of $Y ( E , f )$ so the number on the left $( \sum c _ { i } m ( A _ { i } \cap E ) )$ belongs to $Y ( E , f )$ and so 

$$
\sum c _ {i} m (A _ {i} \cap E) \leq \sup Y (E, f).
$$

For the converse take any $a \in Y ( E , f )$ . So 

$$
a = \int_ {E} \psi \mathrm{d} m = \sum \mathrm{d} _ {j} m (E \cap B _ {j})
$$

for some simple $\psi \leq f$ . Now 

$$
a = \sum_ {j} \sum_ {i} \mathrm{d} _ {j} m (E \cap B _ {j} \cap A _ {i})
$$

by the properties of measure $( A _ { i }$ form a partition of R). For $x \in B _ { j } \cap A _ { i }$ $f ( x ) = c _ { i }$ and $\boldsymbol { \psi } ( \boldsymbol { x } ) = \mathrm { d } _ { j }$ and so $\mathrm { d } _ { j } \leq c _ { i }$ (if only $B _ { j } \cap A _ { i } \neq \emptyset )$ . Hence 

$$
a \leq \sum_ {i} \sum_ {j} c _ {i} m (E \cap B _ {j} \cap A _ {i}) = \sum_ {i} c _ {i} m (E \cap A _ {i})
$$

since $B _ { j }$ partition R. 

## Proof (of Proposition 4.5)

Let $A = \{ x : f ( x ) \leq g ( x ) \}$ , then $A ^ { \mathrm { c } }$ is null and $\begin{array} { r } { f \mathbf { 1 } _ { A } \leq g \mathbf { 1 } _ { A } . \mathrm { ~ S o ~ } \int f \mathbf { 1 } _ { A } \mathrm { d } m \leq } \end{array}$ $\int g \mathbf { 1 } _ { A }$ dm by Theorem 4.3. But since $A ^ { \mathrm { c } }$ is null, $\begin{array} { r } { \int f \mathbf { 1 } _ { A ^ { \mathrm { c } } } \mathrm { d } m = 0 = \int g \mathbf { 1 } _ { A ^ { \mathrm { c } } } \mathrm { d } m . } \end{array}$ RSo by (v) of the same Theorem 

$$
\int_ {\mathbb {R}} f \mathrm{d} m = \int_ {A} f \mathrm{d} m + \int_ {A ^ {c}} f \mathrm{d} m = \int_ {A} f \mathrm{d} m
$$

$$
\leq \int_ {A} g \mathrm{d} m = \int_ {A} g \mathrm{d} m + \int_ {A ^ {c}} g \mathrm{d} m = \int_ {\mathbb {R}} g \mathrm{d} m.
$$

## Proof (of Proposition 4.6)

If both $f ^ { + }$ and $f ^ { - }$ are measurable then the same is true for f since $f = f ^ { + } - f ^ { - }$ Conversely, $( f ^ { + } ) ^ { - 1 } ( [ a , \infty ) ) = \mathbb { R } { \mathrm { ~ i f ~ } } a \leq 0$ and $( f ^ { + } ) ^ { - 1 } ( [ a , \infty ) ) = f ^ { - 1 } ( [ a , \infty ) )$ otherwise; in each case a measurable set. Similarly for $f ^ { - }$ □ 

## Proof (of Proposition 4.10)

Put 

$$
s _ {n} = \sum_ {k = 0} ^ {2 ^ {2 n}} \frac {k}{2 ^ {n}} {\bf 1} _ {f ^ {- 1} ([ \frac {k}{2 ^ {n}}, \frac {k + 1}{2 ^ {n}}))}
$$

which are measurable since the sets $\begin{array} { r } { A _ { k } = f ^ { - 1 } ( [ \frac { k } { 2 ^ { n } } , \frac { k + 1 } { 2 ^ { n } } ) ) } \end{array}$ are measurable. The sequence increases since if we take $n + 1$ , then each $A _ { k }$ is split in half, and to each component of the sum there correspond two new components. The two values of the fraction are equal to or greater than the old one, respectively. The convergence holds since for each x the values $s _ { n } ( x )$ will be a fraction of the form $\frac { k } { 2 ^ { n } }$ approximating $f ( x )$ . Figure 4.2 illustrates the above argument. 

## Proof (of Proposition 4.11)

If $f \leq g$ , then $f ^ { + } \leq g ^ { + }$ but $f ^ { - } \geq g ^ { - }$ . These inequalities imply $\int f ^ { + } \mathrm { d } m \leq$ $\int g ^ { + }$ dm and $\begin{array} { r } { \int g ^ { - } \mathrm { d } m \le \int f ^ { - } } \end{array}$ Rdm. Adding and rearranging gives the result. 

## Proof (of Proposition 4.13)

The claim is obvious for simple functions $f = \sum a _ { i } \mathbf { 1 } _ { A _ { i } }$ it is just elementary algebra. For non-negative measurable $f ,$ and positive c take $s _ { n } \nearrow f$ , and note that $c s _ { n } ~ { \nearrow } ~ c f$ and so 

$$
\int c f \mathrm{d} m = \lim \int c s _ {n} \mathrm{d} m = \lim c \int s _ {n} \mathrm{d} m = c \lim \int s _ {n} \mathrm{d} m = c \int f \mathrm{d} m.
$$

Finally for any $f$ and c we employ the usual trick introducing the positive and negative parts. □ 

## Proof (of Proposition 4.16)

(i) Suppose that $f ( x ) = \infty$ for $x \in A$ with $m ( A ) > 0$ . Then the simple functions $s _ { n } = n \mathbf { 1 } _ { A }$ satisfy $s _ { n } \leq f$ , but $\textstyle \int s _ { n } \mathrm { d } m = n m ( A )$ and the supremum here is $\infty$ . Thus $\begin{array} { r } { \int f \mathrm { d } m = \infty - \mathbf { a } } \end{array}$ Rcontradiction. 

(ii) The simple function $s ( x ) = c \mathbf { 1 } _ { A }$ with $c = \operatorname { i n f } _ { A } f$ has integral in $\operatorname { \dot { \operatorname { \rho } } } _ { A } f m ( A )$ and satisfies $s \leq f$ , which proves the first inequality. Put $t ( x ) = \mathrm { d } \mathbf { 1 } _ { A }$ with $\mathrm { d } = \operatorname* { s u p } _ { A } f$ and $f \leq t$ so $\textstyle { \int f \mathrm { d } m \leq \int }$ t dm which is the second inequality. 

(iii) Note that $- | f | \leq f \leq | f |$ hence $\begin{array} { r } { - \int | f | \mathrm { d } m \leq \int f \mathrm { d } m \leq \int | f | \mathrm { d } m } \end{array}$ and we are done. 

(iv) Let $E _ { n } = f ^ { - 1 } ( [ \frac { 1 } { n } , \infty ) )$ , and $\textstyle E = \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ . The sets $E _ { i }$ are measurable and so is E. The function $\begin{array} { r } { s = \frac { 1 } { n } \mathbf { 1 } _ { E _ { n } } } \end{array}$ Sis a simple function with $s \leq f .$ . Hence $\begin{array} { r } { \int s \mathrm { d } m \leq \int f \mathrm { d } m = 0 . } \end{array}$ , so $\textstyle \int s _ { n } \mathrm { d } m = 0$ , hence $\begin{array} { r } { \frac { 1 } { n } m ( E _ { n } ) = 0 } \end{array}$ . Finally, $m ( E _ { n } ) = 0$ R Rfor all n. Since $E _ { n } \subset E _ { n + 1 } , m ( E ) = \operatorname* { l i m } m ( E _ { n } ) = 0$ . But $E = \{ x : f ( x ) > 0 \}$ so f is zero outside the null set E. □ 

## Proof (of Proposition 4.19)

If $n  \infty$ then $\mathbf { 1 } _ { [ - n , n ] } \ \to \ 1$ hence $g _ { n } ~ = ~ f \mathbf { 1 } _ { [ - n , n ] } ~ \longrightarrow ~ f$ . The convergence is dominated: $g _ { n } \leq | f |$ and by the dominated convergence theorem we have $\begin{array} { r } { \int | f - g _ { n } | \mathrm { d } m \to 0 } \end{array}$ . Similarly, $h _ { n } = \operatorname* { m i n } ( f , n ) \to f$ as $n \to \infty$ and $h _ { n } \leq | f |$ so $\begin{array} { r } { \int | f - h _ { n } | \mathrm { d } m  0 } \end{array}$ □ 

## Proof (of Proposition 4.20)

Using $\begin{array} { r } { \int ( f + g ) \mathrm { d } m = \int f \mathrm { d } m + \int } \end{array}$ g dm we can easily obtain (by induction) 

$$
\int \sum_ {k = 1} ^ {n} f _ {k} \mathrm{d} m = \sum_ {k = 1} ^ {n} \int f _ {k} \mathrm{d} m
$$

for any n. The sequence $\scriptstyle \sum _ { k = 1 } ^ { n } f _ { k }$ is increasing $\left( f _ { k } \ \ge \ 0 \right)$ and converges to $\textstyle \sum _ { k = 1 } ^ { \infty } f _ { k }$ P. So the monotone convergence theorem gives 

$$
\int \sum_ {k = 1} ^ {\infty} f _ {k} \mathrm{d} m = \lim _ {n \rightarrow \infty} \int \sum_ {k = 1} ^ {n} f _ {k} \mathrm{d} m = \lim _ {n \rightarrow \infty} \sum_ {k = 1} ^ {n} \int f _ {k} \mathrm{d} m = \sum_ {k = 1} ^ {\infty} \int f _ {k} \mathrm{d} m
$$

as required. 

## Proof (of Proposition 4.22)

Continuous functions are measurable, and f is bounded on $[ a , b ]$ , hence $f \in$ $\textstyle { \mathcal { L } } ^ { 1 } [ a , b ]$ . Fix $a < x < x + h < b$ , then $\begin{array} { r } { F ( x + h ) - F ( x ) = \int _ { x } ^ { x + h } f } \end{array}$ dm, since the intervals $[ a , x ]$ and $( x , x + h ]$ are disjoint, so that the integral is additive with respect to the upper endpoint. By the mean value property the values of righthand integrals are contained in the interval $[ A h , B h ]$ , where $A = \operatorname* { i n f } \{ f ( t ) : t \in$ $[ x , x + h ] \}$ and $B = \operatorname* { s u p } \{ f ( t ) : t \in [ x , x + h ] \}$ . Both extrema are attained, as f is continuous, so we can find $t _ { 1 } , t _ { 2 }$ in $[ x , x + h ]$ with $A = f ( t _ { 1 } ) , B = f ( t _ { 2 } )$ Thus 

$$
f (t _ {1}) \leq \frac {1}{h} \int_ {x} ^ {x + h} f \mathrm{d} m \leq f (t _ {2}).
$$

The intermediate value theorem provides $\theta \in [ 0 , 1 ]$ such that $f ( x + \theta h ) =$ $\begin{array} { r } { \frac { 1 } { h } \int _ { x } ^ { x + h } f \mathrm { d } m = \frac { F ( x + h ) - F ( x ) } { h } } \end{array}$ . Letting $h  0$ , the continuity of f ensures that $F ^ { \prime } ( x ) = f ( x )$ □ 

## Proof (of Proposition 4.30)

(i) If $y _ { 1 } \le y _ { 2 }$ , then $\{ \omega : X ( \omega ) \subset y _ { 1 } \} \subset \{ \omega : X ( \omega ) \leq y _ { 2 } \}$ and by the monotonicity of measure 

$$
F _ {X} (y _ {1}) = P (\{\omega : X (\omega) \leq y _ {1} \}) \leq P (\{\omega : X (\omega) \leq y _ {2} \}) = F _ {X} (y _ {2}).
$$

(ii) Let $n  \infty { : }$ ; then $\bigcup _ { n } \{ \omega : X ( \omega ) \leq n \} = \varOmega$ (the sets increase). Hence $P ( \{ \omega : X ( \omega ) \leq n \} ) \to P ( \varOmega ) = 1$ by Theorem 2.13 (i) and so $\begin{array} { r } { \operatorname* { l i m } _ { y \to \infty } F _ { X } ( y ) = } \end{array}$ 1. For the second claim consider $F _ { X } ( - n ) = P ( \{ \omega : X ( \omega ) \leq - n \} )$ and note that $\begin{array} { r } { \operatorname* { l i m } _ { y  - \infty } F _ { X } ( y ) = P ( \bigcap _ { n } \{ \omega : X ( \omega ) \leq - n \} ) = P ( \emptyset ) = 0 . } \end{array}$ 

(iii) This follows directly from Theorem 2.13 (ii) with $A _ { n } = \{ \omega : X ( \omega ) \leq y _ { n } \}$ 2 $y _ { n } \nearrow  { y }$ , because $F _ { X } ( y ) = P ( \bigcap _ { n } \{ \omega : X ( \omega ) \leq y _ { n } \} )$ □ 

## Proof (of Proposition 4.36)

Inserting the formulae for the option prices in call-put parity we have 

$$
\begin{array}{l} S (0) = \exp \{- r T \} \Big (\int_ {\Omega} (S (T) - K) ^ {+} \mathrm{d} P - \int_ {\Omega} (K - S (T)) ^ {+} \mathrm{d} P + K \Big) \\ \qquad = \exp \{- r T \} \Big (\int_ {\{S (T) \geq K \}} (S (T) - K) \mathrm{d} P \\ \qquad \qquad - \int_ {\{S (T) <   K \}} (K - S (T)) \mathrm{d} P + K \Big) \\ \qquad = \exp \{- r T \} \int_ {\Omega} S (T) \mathrm{d} P, \end{array}
$$

which is independent of K, as claimed. 

## Proof (of Proposition 4.37)

The general formula $C = \mathrm { e } ^ { - r T } \mathbb { E } ( S ( N ) - K ) ^ { + }$ , where $S ( N )$ has binomial distribution, gives 

$$
\begin{array}{c} C = \mathrm{e} ^ {- r T} \sum_ {k = 1} ^ {N} \binom {N} {k} p ^ {k} (1 - q) ^ {N - k} (S (0) U ^ {k} D ^ {N - k} - K) ^ {+} \\ = \mathrm{e} ^ {- r T} \sum_ {k = A} ^ {N} \binom {N} {k} p ^ {k} (1 - q) ^ {N - k} (S (0) U ^ {k} D ^ {N - k} - K) \end{array}
$$

We can rewrite this as follows: note that if we set $q = P U \mathrm { e } ^ { - r T }$ then $1 - q =$ $( 1 - p ) U \mathrm { e } ^ { - r T }$ , so that $0 \leq q \leq 1$ and 

$$
C = S (0) \sum_ {k = A} ^ {N} {\binom {N} {k}} q ^ {k} (1 - q) ^ {N - k} - K \mathrm{e} ^ {- r T} \sum_ {k = A} ^ {N} {\binom {N} {k}} p ^ {k} (1 - p) ^ {N - k}
$$

which we write concisely as 

$$
C = S (0) \Psi (A, N, p U \mathrm{e} ^ {- r T}) - K \mathrm{e} ^ {- r T} \Psi (A, N, p)\tag{4.9}
$$

where $\begin{array} { r } { \varPsi ( A , N , p ) \ = \ \sum _ { k = A } ^ { N } \binom { N } { k } p ^ { k } ( 1 - p ) ^ { N - k } } \end{array}$ is the complementary binomial distribution function. □ 

## Proof (of Proposition 4.38)

To compute the expectation $\mathbb { E } ( S ( T ) - K ) ^ { + }$ we employ the density of the Gaussian distribution, hence 

$$
C = \frac {1}{\sqrt {2 \pi}} \int_ {\mathbb {R}} \mathrm{e} ^ {- \frac {1}{2} y ^ {2}} \Big (S (0) \mathrm{e} ^ {- \frac {1}{2} \sigma^ {2} T} \mathrm{e} ^ {y \sigma \sqrt {T}} - K \mathrm{e} ^ {- r T} \Big) ^ {+} \mathrm{d} y
$$

The integration reduces to the values of y satisfying 

$$
S (0) \mathrm{e} ^ {- \frac {1}{2} \sigma^ {2} T} \mathrm{e} ^ {y \sigma \sqrt {T}} - K \mathrm{e} ^ {- r T} \geq 0
$$

since otherwise the integrand is zero. Solving for y gives 

$$
y \geq d = \frac {\ln \frac {K \mathrm{e} ^ {- r T}}{S (0)} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}.
$$

For those y we can drop the positive part and employ linearity. The first term on the right is of the form 

$$
S (0) \int_ {d} ^ {+ \infty} \mathrm{e} ^ {y \sigma \sqrt {T} - \frac {1}{2} \sigma^ {2} T} g (y) \mathrm{d} y
$$

where $g$ denotes the Gaussian density with zero mean and unit standard variation. Substituting $z = y - \sigma { \sqrt { T } }$ yields 

$$
S (0) \int_ {d - \sigma \sqrt {T}} ^ {+ \infty} n (z) \mathrm{d} z = S (0) N (- d + \sigma \sqrt {T})
$$

where $N$ is the cumulative distribution function of the Gaussian (normal) distribution. The second term is of the form 

$$
- K \mathrm{e} ^ {- r T} \int_ {d} ^ {+ \infty} n (y) \mathrm{d} y = - K \mathrm{e} ^ {- r T} N (- d)
$$

so writing $d _ { 1 } = - d + \sigma { \sqrt { T } } , d _ { 2 } = - d .$ , we are done. 

# Spaces of integrable functions

Until now we have treated the points of the measure space $( \mathbb { R } , \mathcal { M } , m )$ and, more generally, of any abstract probability space $( \varOmega , \mathcal { F } , P )$ , as the basic objects, and regarded measurable or integrable functions as mappings associating real numbers with them. We now alter our point of view a little, by treating an integrable function as a ‘point’ in a function space, or, more precisely, as an element of a normed vector space. For this we need some extra structure on the space of functions we deal with, and we need to come to terms with the fact that the measure and integral cannot distinguish between functions which are almost everywhere equal. 

The additional structure we require is to define a concept of distance (i.e. a metric) between given integrable functions – by analogy with the familiar Euclidean distance for vectors in $\mathbb { R } ^ { n }$ we shall obtain the distance between two functions as the length, or norm, of their diference – thus utilizing the vector space structure of the space of functions. We shall be able to do this in a variety of ways, each with its own advantages – unlike the situation in $\mathbb { R } ^ { n }$ , where all norms turn out to be equivalent, we now obtain genuinely diferent distance functions. 

It is worth noting that the spaces of functions we shall discuss are all infinitedimensional vector spaces: this can be seen already by considering the vector space $\mathcal { C } ( [ a , b ] , \mathbb { R } )$ of real-valued continuous functions defined on $[ a , b ]$ and noting that a polynomial function of degree n cannot be represented as a linear combination of polynomials of lower degree. 

Finally, recall that in introducing characteristic functions at the end of the previous chapter, we needed to extend the concept of integrability to complexvalued functions. We observed that for $f = u + \mathrm { i } v$ the integral defined by $\begin{array} { r } { \int _ { E } f \mathrm { d } m = \int _ { E } u \mathrm { d } m + \mathrm { i } \int _ { E } : } \end{array}$ v dm is linear, and that the inequality $| \int _ { E } f \mathrm { d } m | \leq$ $\textstyle \int _ { E } | f |$ R Rdm remains valid. When considering measurable functions $f : E \to \mathbb { C }$ Rin defining the appropriate spaces of integrable functions in this chapter, this inequality will show that $\textstyle \int _ { E } f \mathrm { d } m \in \mathbb { C }$ is well-defined. 

RThe results proved below extend to the case of complex-valued functions, unless otherwise specified. When wishing to emphasize that we are dealing with complex-valued functions in particular applications or examples, we shall use notation such as $f \in { \mathcal { L } } ^ { 1 } ( E , \mathbb { C } )$ to indicate this. Complex-valued functions will have particular interest when we consider the important space $\mathcal { L } ^ { 2 } ( E )$ of ‘square-integrable’ functions. 

## 5.1 The space $L ^ { 1 }$

First we recall the definition of a general concept of ‘distance’ between points of a set: 

## Definition 5.1

Let X be any set. The function $d : X \times X \to \mathbb { R }$ is a metric on X (and $( X , d )$ is called a metric space) if it satisfies: 

(i) $d ( x , y ) \geq 0$ for all $x , y \in X$ 

(ii) $d ( x , y ) = 0$ if and only if $x = y$ 

(iii) $d ( y , x ) = d ( x , y )$ for all $x , y \in X$ 

(iv) $d ( x , z ) \leq d ( x , y ) + d ( y , z )$ for all $x , y , z \in X$ 

The final property is known as the triangle inequality and generalizes the well-known inequality of that name for vectors in $\mathbb { R } ^ { n }$ . When X is a vector space (as will be the case in almost all our examples) then there is a very simple way to generate a metric by defining the distance between two vectors as the ‘length of their diference. For this we require a further definition: 

## Definition 5.2

Let X be a vector space over $\mathbb { R } \ ( \mathrm { o r } \ \mathbb { C } )$ . The function $x \mapsto \| x \|$ from X into R is a norm on X if it satisfies: 

(i) $\| { \boldsymbol x } \| \geq 0$ for all $x \in X$ 

(ii) $\| x \| = 0$ if and only if $x = 0$ 

(iii) $\| \alpha x \| = | \alpha | \| x \|$ for all $\alpha \in \mathbb { R } { \mathrm { ~ ( o r ~ } } \mathbb { C } { \mathrm { ) } } , x \in X$ 

(iv) $\| x + y \| \leq \| x \| + \| y \|$ for all x, $y \in X$ 

Clearly a norm $x \mapsto \| x \|$ on X induces a metric by setting $d ( x , y ) = \| x - y \|$ The triangle inequality follows once we observe that $\| x - z \| = \| ( x - y ) + ( y - z ) \|$ and apply (iv). 

We naturally wish to use the integral to define the concept of distance between functions in $\mathcal { L } ^ { 1 } ( E )$ , for measurable $E \subset \mathbb { R }$ . The presence of null sets in $( \mathbb { R } , \mathcal { M } , m )$ means that the integral cannot distinguish between the function that is identically 0 and one which is 0 a.e. The natural idea of defining the ‘length’ of the vector f as $\textstyle \int _ { E } | f |$ dm thus runs into trouble, since it would be Rpossible for non-zero elements of $\mathcal { L } ^ { 1 } ( E )$ to have ‘zero length’. 

The solution adopted is to identify functions which are a.e. equal, by defining an equivalence relation on $\mathcal { L } ^ { 1 } ( E )$ and defining the length function for the resulting equivalence classes of functions, rather than for the functions themselves. 

Thus we define 

$$
L ^ {1} (E) = \mathcal {L} ^ {1} (E) / _ {\equiv}
$$

where the equivalence relation is given by: 

$f \equiv g$ if and only if $f ( x ) = g ( x )$ for almost all $x \in E$ 

(that is, $\{ x \in E : f ( x ) \neq g ( x ) \}$ is null). 

Write [f] for the equivalence class containing the function $f \in { \mathcal { L } } ^ { 1 } ( E )$ . Thus $h \in [ f ]$ if $h ( x ) = f ( x ) { \mathrm { ~ a . e . } }$ 

## Exercise 5.1

Check that is an equivalence relation on $\mathcal { L } ^ { 1 } ( E )$ 

We now show that $L ^ { 1 } ( E )$ is a vector space, since $\mathcal { L } ^ { 1 }$ is a vector space by Theorem 4.14. However, this requires that we explain what we mean by a linear combination of equivalence classes. This can be done quite generally for any equivalence relation; however, we shall focus on what is needed in our particular case: define the $[ f ] + [ g ]$ as the class $[ f + g ]$ of $f + g$ , i.e. $h \in [ f ] + [ g ]$ if $h ( x ) = f ( x ) + g ( x )$ except possibly on some null set. This is consistent, since the union of two null sets is null. The definition clearly does not depend on the choice of representative taken from each equivalence class. Similarly for multiplication by constants: $a [ f ] = [ a f ]$ for $a \in \mathbb { R }$ . Hence $L ^ { 1 } ( E )$ is a vector space with these operations. 

Convention Strictly speaking we should continue to distinguish between the equivalence class $[ f ] \in L _ { 1 } ( E )$ and the function $f \in \mathcal { L } _ { 1 } ( E )$ which is a representative of this class. To do so consistently in all that follows would, however, obscure the underlying ideas, and there is no serious loss of clarity by treating $f$ interchangeably as a member of $L ^ { 1 }$ and of $\mathcal { L } ^ { 1 }$ , depending on the context. In other words, by treating the equivalence class $[ f ]$ as if it were the function $f _ { : }$ we implicitly identify two functions as soon as they are a.e. equal. With this convention it will be clear that the ‘length function’ defined below is a genuine norm on $L ^ { 1 } ( E )$ 

We equip $L ^ { 1 } ( E )$ with the norm 

$$
\| f \| _ {1} = \int_ {E} | f | \mathrm{d} m.
$$

This is a norm on $L ^ { 1 } ( E )$ 

1. $\| f \| _ { 1 } = 0$ if and only if $f = 0 { \mathrm { ~ a . e . } }$ , so that $f \equiv 0$ as an element of $L ^ { 1 } ( E )$ 

$$
\left\| c f \right\| _ {1} = \int_ {E} | c f | \mathrm{d} m = | c | \int_ {E} | f | \mathrm{d} m = | c | \cdot \| f \| _ {1}, (c \in \mathbb {R}),
$$

<sup>3.</sup> k<sup>f</sup> <sup>+</sup> <sup>g</sup>k1 <sup>=</sup> |<sup>f</sup> <sup>+</sup> <sup>g</sup>| <sup>dm</sup> ≤ |<sup>f</sup>| <sup>dm</sup> <sup>+</sup> |<sup>g</sup>| <sup>dm</sup> <sup>=</sup> k<sup>f</sup>k1 <sup>+</sup> k<sup>g</sup>k1<sup>.</sup> 

The most important feature of $L ^ { 1 } ( E )$ , from our present perspective, is the fact that it is a complete normed vector space. The precise definition is given below. Completeness of the real line R and Euclidean spaces $\mathbb { R } ^ { n }$ is what guides the analysis of real functions, and here we seek an analogue which has a similar impact in the infinite-dimensional context provided by function spaces. The definition will be stated for general normed vector spaces: 

## Definition 5.3

Let X be a vector space with norm $\| \cdot \| _ { X }$ . We say that a sequence $f _ { n } \in X$ is Cauchy if 

$$
\forall \varepsilon > 0 \exists N: \forall n, m \geq N \| f _ {n} - f _ {m} \| _ {X} <   \varepsilon .
$$

If each Cauchy sequence is convergent to some element of X, then we say that X is complete. 

## Example 5.1

Let $\begin{array} { r } { f _ { n } ( x ) = \frac { 1 } { x } \mathbf { 1 } _ { [ n , n + 1 ] } ( x ) } \end{array}$ , and suppose that $n \neq m$ 

$$
\begin{array}{l} \| f _ {n} - f _ {m} \| _ {1} = \int_ {0} ^ {\infty} \frac {1}{x} | \mathbf {1} _ {[ n, n + 1 ]} - \mathbf {1} _ {[ m, m + 1 ]} |   \mathrm{d} x \\ \qquad = \int_ {n} ^ {n + 1} \frac {1}{x}   \mathrm{d} x + \int_ {m} ^ {m + 1} \frac {1}{x}   \mathrm{d} x \\ \qquad = \log \frac {n + 1}{n} + \log \frac {m + 1}{m}. \end{array}
$$

If $a _ { n } \ \to \ 1$ , then log $a _ { n } \to 0$ and the right-hand side can be as small as we wish: for $\varepsilon > 0$ take N such that log $\textstyle { \frac { N + 1 } { N } } < { \frac { \varepsilon } { 2 } }$ . So $f _ { n }$ is a Cauchy sequence in $L ^ { 1 } ( 0 , \infty )$ . (When $E = ( a , b )$ , we write $L ^ { 1 } ( a , b )$ for $L ^ { 1 } ( E ) , { \mathrm { e t c . } } )$ 

## Exercise 5.2

Decide whether each of the following is Cauchy as a sequence in $L ^ { 1 } ( 0 , \infty )$ 

(a) ${ f _ { n } } = \mathbf { 1 } _ { [ n , n + 1 ] }$ 

(b) $\begin{array} { r } { f _ { n } = \frac { 1 } { x } \mathbf { 1 } _ { ( 0 , n ) } } \end{array}$ 

(c) $\begin{array} { r } { f _ { n } = \frac { 1 } { x ^ { 2 } } \mathbf { 1 } _ { ( 0 , n ) } } \end{array}$ 

The proof of the main result below makes essential use of the Beppo–Levi theorem in order to transfer the main convergence question to that of series of real numbers; its role is essentially to provide the analogue of the fact that in R (and hence in C) absolutely convergent series will always converge. (The Beppo–Levi theorem clearly extends to complex-valued functions, just as we showed for the dominated convergence theorem, but we shall concentrate on the real case in the proof below, since the extension to C is immediate.) 

We digress briefly to recall how this property of series ensures completeness in R: let $( x _ { n } )$ be a Cauchy sequence in R, and extract a subsequence $\left( { x _ { n _ { k } } } \right)$ such that $| x _ { n } - x _ { n _ { k } } | < 2 ^ { - k }$ for all $n \geq n _ { k }$ as follows: 

1. find $n _ { 1 }$ such that $| x _ { n } - x _ { n _ { 1 } } | < 2 ^ { - 1 }$ for all $n \geq n _ { 1 }$ 

2. find $n _ { 2 } > n _ { 1 }$ such that $| x _ { n } - x _ { n _ { 2 } } | < 2 ^ { - 2 }$ for all $n \geq n _ { 2 }$ 2 

3. . . . 

4. find $n _ { k } > n _ { k - 1 }$ with $| x _ { n } - x _ { n _ { k } } | < 2 ^ { - k }$ for all $n \geq n _ { k }$ 

The Cauchy property ensures each time that such $n _ { k }$ can be found. Now consider the telescoping series with partial sums 

$$
y _ {k} = x _ {n _ {1}} + (x _ {n _ {2}} - x _ {n _ {1}}) + \dots + (x _ {n _ {k}} - x _ {n _ {k - 1}}) = x _ {n _ {k}}
$$

which has 

$$
\left| y _ {k} \right| \leq \left| x _ {n _ {1}} \right| + \sum_ {i = 1} ^ {k} \left| x _ {n _ {i}} - x _ {n _ {i - 1}} \right| <   \left| x _ {n _ {1}} \right| + \sum_ {i = 1} ^ {k} \frac {1}{2 ^ {i}}.
$$

Thus this series converges, in other words $( x _ { n _ { k } } )$ converges in R, and its limit is also that of the whole Cauchy sequence $( x _ { n } )$ 

To apply the Beppo–Levi theorem below we therefore need to extract a ‘rapidly convergent sequence’ from the given Cauchy sequence in $L ^ { 1 } ( E )$ . This provides an a.e. limit for the original sequence, and the Fatou lemma does the rest. 

## Theorem 5.1

The space $L ^ { 1 } ( E )$ is complete. 

## Proof

Suppose that $f _ { n }$ is a Cauchy sequence. Let $\begin{array} { r } { \varepsilon = \frac { 1 } { 2 } } \end{array}$ . There is $N _ { 1 }$ such that for $n \geq N _ { 1 }$ 

$$
\left\| f _ {n} - f _ {N _ {1}} \right\| _ {1} \leq \frac {1}{2}.
$$

Next, let $\begin{array} { r } { \varepsilon = \frac { 1 } { 2 ^ { 2 } } } \end{array}$ , and for some $N _ { 2 } > N _ { 1 }$ we have 

$$
\| f _ {n} - f _ {N _ {2}} \| _ {1} \leq \frac {1}{2 ^ {2}}
$$

for $n \geq N _ { 2 }$ . In this way we construct a subsequence $f _ { N _ { k } }$ satisfying 

$$
\left\| f _ {N _ {n + 1}} - f _ {N _ {n}} \right\| _ {1} \leq \frac {1}{2 ^ {n}}
$$

for all $n .$ . Hence the series $\begin{array} { r l } { \sum _ { n \geq 1 } \| f _ { N _ { n + 1 } } - f _ { N _ { n } } \| _ { 1 } } & { { } } \end{array}$ converges and by the Beppo– Levi theorem, the series 

$$
f _ {N _ {1}} (x) + \sum_ {n = 1} ^ {\infty} [ f _ {N _ {n + 1}} (x) - f _ {N _ {n}} (x) ]
$$

converges a.e.; denote the sum by f(x). Since 

$$
f _ {N _ {1}} (x) + \sum_ {n = 1} ^ {k} [ f _ {N _ {n + 1}} (x) - f _ {N _ {n}} (x) ] = f _ {N _ {k + 1}}
$$

the left-hand side converges to $f ( x )$ , so $f _ { N _ { k + 1 } } ( x )$ converges to $f ( x )$ . Since the sequence of real numbers $f _ { n } ( x )$ is Cauchy and the above subsequence converges, the whole sequence converges to the same limit $f ( x )$ 

We have to show that $f \in L ^ { 1 }$ and $\| f _ { k } - f \| _ { 1 } \to 0$ 

Let $\varepsilon > 0$ . The Cauchy condition gives an N such that 

$$
\forall n, m \geq N, \| f _ {n} - f _ {m} \| _ {1} <   \varepsilon .
$$

By Fatou’s lemma 

$$
\| f - f _ {m} \| _ {1} = \int | f - f _ {m} |   \mathrm{d} m \leq \operatorname * {l i m i n f} _ {k \to \infty} \int | f _ {N _ {k}} - f _ {m} |   \mathrm{d} m = \operatorname * {l i m i n f} _ {k \to \infty} \| f _ {N _ {k}} - f _ {m} \| _ {1} <   \varepsilon .\tag{5.1}
$$

So $f - f _ { m } \in L ^ { 1 }$ which implies $f = ( f - f _ { m } ) + f _ { m } \in L ^ { 1 }$ , but (5.1) also gives$\| f - f _ { m } \| _ { 1 } \to 0$ 口

## 5.2 The Hilbert space $L ^ { 2 }$

The space we now introduce plays a special role in the theory. It provides the closest analogue of the Euclidean space $\mathbb { R } ^ { n }$ among the spaces of functions, and its geometry is closely modelled on that of $\mathbb { R } ^ { n }$ . It is possible, via the integral, to induce the norm via an inner product, which in turn provides a concept of orthogonality (and hence ‘angles’) between functions. This gives $L ^ { 2 }$ many pleasant properties, such as a ‘Pythagoras theorem’ and the concept of orthogonal projections, which plays vital role in many applications. 

To define the norm, and hence the space $L ^ { 2 } ( E )$ for a given measurable set $E \subset \mathbb { R }$ , let 

$$
\| f \| _ {2} = (\int_ {E} | f | ^ {2} \mathrm{d} m) ^ {\frac {1}{2}}
$$

and define $\mathcal { L } ^ { 2 } ( E )$ as the set of measurable functions for which this quantity is finite. (Note that, as for $L ^ { 1 }$ , we require non-negative integrands; it is essential that the integral is non-negative in order for the square root to make sense. Although we always have $f ^ { 2 } ( x ) = ( f ( x ) ) ^ { 2 } \geq 0$ when $f ( x )$ is real, the modulus is needed to include the case of complex-valued functions $f : E \to \mathbb { C }$ . This also makes the notation consistent with that of the other L<sup>p</sup>-spaces we shall consider below where $| f | ^ { 2 }$ is replaced by $| f | ^ { p }$ for arbitrary $p \geq 1 . )$ 

We introduce $L ^ { 2 } ( E )$ as the set of equivalence classes of elements of $\mathcal { L } ^ { 2 } ( E )$ under the equivalence relation $f \equiv g$ if $f \ = \ g \ \mathrm { \ a . e } .$ , exactly as for $L ^ { 1 } ( E )$ 2 and continue the convention of treating the equivalence classes as functions. If $f : E \to \mathbb { C }$ satisfies $\textstyle \int _ { E } | f | ^ { 2 } \mathrm { d } m < \infty$ we write $f \in L ^ { 2 } ( E , \mathbb { C } )$ – again using f interchangeably as a representative of its equivalence class and to denote the class itself. 

It is straightforward to prove that $L ^ { 2 } ( E )$ is a vector space: clearly, for $a \in \mathbb { R }$ $\vert a f \vert ^ { 2 }$ is integrable if $| f | ^ { 2 }$ is, while 

$$
| f + g | ^ {2} \leq 2 ^ {2} \max \{| f | ^ {2}, | g | ^ {2} \} \leq 4 (| f | ^ {2} + | g | ^ {2})
$$

shows that $L ^ { 2 } ( E )$ is closed under addition. 

## 5.2.1 Properties of the $L ^ { 2 } .$ -norm

We provide a simple proof that the map $f \mapsto \| f \| _ { 2 }$ is a norm: to see that it satisfies the triangle inequality requires a little work, but the ideas will be very familiar from elementary analysis in $\mathbb { R } ^ { n }$ , as is the terminology, though the context is rather diferent. We state and prove the result for the general case of $L ^ { 2 } ( E , \mathbb { C } )$ 

## Theorem 5.2 (The Schwarz Inequality)

If $f , g \in L ^ { 2 } ( E , \mathbb { C } )$ then $f g \in L ^ { 1 } ( E , \mathbb { C } )$ and 

$$
\left| \int_ {E} f \overline {{g}} \mathrm{d} m \right| \leq \| f g \| _ {1} \leq \| f \| _ {2} \| g \| _ {2}\tag{5.2}
$$

where $\overline { { g } }$ denotes the complex conjugate of $g$ . 

## Proof

Replacing $f , g$ by $| f | , | g |$ we may assume that $f$ and $g$ are non-negative (the first inequality has already been verified, since $\begin{array} { r } { \| f g \| _ { 1 } = \int _ { E } | f g | } \end{array}$ dm, and the second Ronly involves the modulus in each case). Since we do not know in advance that $\textstyle \int _ { E } f g \mathrm { d } m$ is finite, we shall first restrict attention to bounded measurable Rfunctions by setting $f _ { n } = f \wedge n$ and $g _ { n } = g \wedge n$ , and confine our domain of integration to the bounded set $E \cap [ - k , k ] = E _ { k }$ 

For any $t \in \mathbb { R }$ we have 

$$
0 \leq \int_ {E _ {k}} (f _ {n} + t g _ {n}) ^ {2} \mathrm{d} m = \int_ {E _ {k}} f _ {n} ^ {2} \mathrm{d} m + 2 t \int_ {E _ {k}} f _ {n} g _ {n} \mathrm{d} m + t ^ {2} \int_ {E _ {k}} g _ {n} ^ {2} \mathrm{d} m.
$$

As a quadratic in t this does not have two distinct solutions, so the discriminant is non-positive. Thus for all $n \geq 1$ 

$$
\begin{array}{r l} & {(2 \int_ {E _ {k}} f _ {n} g _ {n} \mathrm{d} m) ^ {2} \leq 4 (\int_ {E _ {k}} f _ {n} ^ {2} \mathrm{d} m) (\int_ {E _ {k}} g _ {n} ^ {2} \mathrm{d} m) ^ {2}} \\ & {\qquad \leq 4 (\int_ {E} ^ {2} | f | ^ {2} \mathrm{d} m) (\int_ {E} ^ {2} | g | ^ {2} \mathrm{d} m)} \\ & {\qquad = \| f \| _ {2} ^ {2} \| g \| _ {2} ^ {2}.} \end{array}
$$

Monotone convergence now yields 

$$
(\int_ {E _ {k}} f g \mathrm{d} m) ^ {2} \leq \| f \| _ {2} ^ {2} \| g \| _ {2} ^ {2}
$$

for each k, and since $\textstyle E = \bigcup _ { k } E _ { k }$ we obtain finally that 

$$
(\int_ {E} f g \mathrm{d} m) ^ {2} \leq \| f \| _ {2} ^ {2} \| g \| _ {2} ^ {2},
$$

which implies the Schwarz inequality. 

The triangle inequality for the norm on $L ^ { 2 } ( E , \mathbb { C } )$ now follows at once – we need to show that $\| f + g \| _ { 2 } \leq \| f \| _ { 2 } + \| g \| _ { 2 }$ for f $, g \in L ^ { 2 } ( E , \mathbb { C } )$ : 

$$
\| f + g \| _ {2} ^ {2} = \int_ {E} | f + g | ^ {2}   \mathrm{d} m = \int_ {E} (f + g) \overline {{(f + g)}} \mathrm{d} m = \int_ {E} (f + g) (\overline {{f}} + \overline {{g}})   \mathrm{d} m.
$$

The latter integral is 

$$
\int_ {E} | f | ^ {2} \mathrm{d} m + \int_ {E} (f \overline {{g}} + \overline {{f}} g) \mathrm{d} m + \int_ {E} | g | ^ {2} \mathrm{d} m,
$$

which is dominated by $( \| f \| _ { 2 } + \| g \| _ { 2 } ) ^ { 2 }$ since the Schwarz inequality gives 

$$
\int_ {E} (f \overline {{g}} + g \overline {{f}}) \mathrm{d} m \leq 2 \int_ {E} | f g | \mathrm{d} m \leq 2 \| f \| _ {2} \| g \| _ {2}.
$$

The result follows. 

The other properties are immediate: 

(i) clearly $\| f \| _ { 2 } = 0$ means that $| f | ^ { 2 } = 0 { \mathrm { ~ a . e . } }$ ., hence $f = 0 { \mathrm { ~ a . e . } }$ , 

(ii) for $\begin{array} { r } { a \in \mathbb { C } , \| a f \| _ { 2 } = ( \int _ { E } ^ { 2 } | a f | ^ { 2 } \mathrm { d } m ) ^ { \frac { 1 } { 2 } } = | a | \| f \| _ { 2 } . } \end{array}$ 

Thus the map $f \mapsto \| f \| _ { 2 }$ is a norm on $L ^ { 2 } ( E , \mathbb { C } )$ 

The proof that $L ^ { 2 } ( E )$ is complete under this norm is similar to that for $L ^ { 1 } ( E )$ , and will be given in Theorem 5.11 below for arbitrary L<sup>p</sup>-spaces $( 1 <$ $p < \infty )$ 

In general, without restriction of the domain set $E _ { : }$ , neither $L ^ { 1 } \subseteq L ^ { 2 }$ nor $L ^ { 2 } \subseteq L ^ { 1 }$ . To see this consider $\begin{array} { r } { E = [ 1 , \infty ) , f ( x ) = \frac { 1 } { x } } \end{array}$ . Then $f \in L ^ { 2 } ( E )$ but $f \notin L ^ { 1 } ( E )$ . Next put $\begin{array} { r } { F = ( 0 , 1 ) , g ( x ) = \frac { 1 } { \sqrt { x } } } \end{array}$ . Now $g \in L ^ { 1 } ( F )$ but $g \not \in L ^ { 2 } ( F )$ 

For finite measure spaces – and hence for probability spaces! – we do have a useful inclusion: 

## Proposition 5.3

If the set D has finite measure (that is, $m ( D ) < \infty )$ , then $L ^ { 2 } ( D ) \subset L ^ { 1 } ( D )$ 

Hint Estimate $| f |$ by means of $| f | ^ { 2 }$ and then use the fact that the integral of $| f | ^ { 2 }$ is finite. 

Before exploring the geometry induced on $L ^ { 2 }$ by its norm, we consider examples of sequences in $L ^ { 2 }$ to provide a little practice in determining which are Cauchy sequences for the $L ^ { 2 } \mathrm { - n o r m }$ , and compare this with their behaviour as elements of $L ^ { 1 }$ 

## Example 5.2

We show that the sequence $\begin{array} { r } { f _ { n } = \frac { 1 } { x } \mathbf { 1 } _ { [ n , n + 1 ] } } \end{array}$ is Cauchy in $L ^ { 2 } ( 0 , \infty )$ 

$$
\begin{array}{l} \| f _ {n} - f _ {m} \| _ {2} = \int_ {0} ^ {\infty} \frac {1}{x ^ {2}} | \mathbf {1} _ {[ n, n + 1 ]} - \mathbf {1} _ {[ m, m + 1 ]} | ^ {2}   \mathrm{d} x \\ = \int_ {n} ^ {n + 1} \frac {1}{x ^ {2}}   \mathrm{d} x + \int_ {m} ^ {m + 1} \frac {1}{x ^ {2}}   \mathrm{d} x \\ = \left(\frac {1}{n} - \frac {1}{n + 1}\right) + \left(\frac {1}{m} - \frac {1}{m + 1}\right) \\ \leq \frac {2}{n} + \frac {2}{m} \end{array}
$$

and for $\varepsilon > 0$ let N be such that $\textstyle { \frac { 2 } { N } } < { \frac { \varepsilon } { 2 } }$ . Then $\| f _ { m } - f _ { n } \| < \varepsilon$ whenever $m , n \geq N$ 

Exercise 5.3 

Is the sequence 

$$
g _ {n} (x) = \mathbf {1} _ {(n, \infty)} (x) \frac {1}{x ^ {2}}
$$

a Cauchy sequence in $L ^ { 2 } ( R ) ?$ 

## Exercise 5.4

Decide whether each of the following is Cauchy as a sequence in $L ^ { 2 } ( 0 , \infty )$ 

(a) $f _ { n } = \mathbf { 1 } _ { ( 0 , n ) }$ 

(b) $\begin{array} { r } { f _ { n } = \frac { 1 } { x } \mathbf { 1 } _ { ( 0 , n ) } } \end{array}$ 

(c) $\begin{array} { r } { f _ { n } = \frac { 1 } { x ^ { 2 } } \mathbf { 1 } _ { ( 0 , n ) } } \end{array}$ 

## 5.2.2 Inner product spaces

We are ready for the additional structure specific (among the Lebesgue function spaces) to $L ^ { 2 }$ : 

$$
\forall f, g \in L ^ {2} (E, \mathbb {C}) \quad (f, g) = \int f \overline {{g}} \mathrm{d} m\tag{5.3}
$$

defines an inner product, which induces the $L ^ { 2 } .$ -norm: 

$$
\sqrt {(f , f)} = (\int_ {E} f \overline {{f}} \mathrm{d} m) ^ {\frac {1}{2}} = (\int_ {E} | f | ^ {2} \mathrm{d} m) ^ {\frac {1}{2}} = \| f \| _ {2}.
$$

To explain what this means we verify the following properties, all of which follow easily from the integration theory we have developed: 

## Proposition 5.4

Linearity (in the first argument) 

$$
(f + g, h) = (f, h) + (g, h),
$$

$$
(c f, h) = c (f, h).
$$

Conjugate Symmetry 

$$
(f, g) = \overline {{(g , f)}}.
$$

Positive Definiteness 

$$
(f, f) \geq 0, \quad (f, f) = 0 \Leftrightarrow f = 0.
$$

Hint Use the additivity of the integral in the first part, and recall for the last part that if $f = 0 ~ \mathrm { a . e }$ . then f is the zero element of $L ^ { 2 } ( E , \mathbb { C } )$ 

As an immediate consequence we get conjugate-linearity with respect to the second argument 

$$
(f, c g + h) = \overline {{c}} (f, g) + (f, h).
$$

Of course, if $f , g \in L ^ { 2 }$ are real-valued, the inner product is real and linear in the second argument also. 

Examination of the proof of the Schwarz inequality reveals that the particular form of the inner product defined here on $L ^ { 2 } ( E , \mathbb { C } )$ is entirely irrelevant for this result: all we need for the proof is that the map defined in (5.3) has the properties proved for it in the last Proposition. 

We shall therefore make the following important definition, which will be familiar from the finite-dimensional context of $\mathbb { R } ^ { n }$ , and which we now wish to apply more generally. 

## Definition 5.4

An inner product on a vector space H over C is a map $( \cdot , \cdot ) : H \times H \to \mathbb { C }$ which satisfies the three conditions listed in Proposition 5.4. The pair $\left( H , \left( \cdot , \cdot \right) \right)$ is called an inner product space. 

## Example 5.3

The usual scalar product in $\mathbb { R } ^ { n }$ makes this space into a real inner product space, and $\mathbb { C } ^ { n }$ equipped with $\begin{array} { r } { ( z , w ) = \sum _ { i = 1 } ^ { n } z _ { i } \overline { { w } } _ { i } } \end{array}$ is a complex one. 

Proposition 5.4 shows that $L ^ { 2 } ( E , \mathbb { C } )$ is a (complex) inner product space. With the obvious simplifications in the definitions the vector space $L ^ { 2 } ( E , \mathbb { R } ) =$ $L ^ { 2 } ( E )$ is a real inner product space, i.e. with R as the set of scalars. 

The following identities are immediate consequences of the above definitions. 

## Proposition 5.5

Let $\left( H , \left( \cdot , \cdot \right) \right)$ be a complex inner product space, with induced norm $\| \cdot \|$ . The following identities hold for all $h _ { 1 } , h _ { 2 } \in H$ : 

(i) Parallelogram law: 

$$
\left\| h _ {1} + h _ {2} \right\| ^ {2} + \left\| h _ {1} - h _ {2} \right\| ^ {2} = 2 (\left\| h _ {1} \right\| ^ {2} + \left\| h _ {2} \right\| ^ {2}).
$$

(ii) Polarization identity: 

$$
4 (h _ {1}, h _ {2}) = \| h _ {1} + h _ {2} \| ^ {2} - \| h _ {1} - h _ {2} \| ^ {2} + \mathrm{i} \{\| h _ {1} + \mathrm{i} h _ {2} \| ^ {2} - \| h _ {1} - \mathrm{i} h _ {2} \| ^ {2} \}.
$$

## Remark 5.1

These identities, while trivial consequences of the definitions, are useful in checking that certain norms cannot be induced by inner products. An example is given in the Exercise below. With the addition of completeness, the identities serve to characterize inner product norms: it can be proved that in the class of complete normed spaces (known as Banach spaces), those whose norms are induced by inner products (i.e. are Hilbert spaces) are precisely those for which the parallelogram law holds, and the inner product is then recovered from the norm via the polarization identity. We shall not prove this here. 

## Exercise 5.5

Show that it is impossible to define an inner product on the space $C [ 0 , 1 ]$ of continuous functions $f : [ 0 , 1 ] \to \mathbb { R }$ which will induce the sup norm $\| f \| _ { \infty } = \operatorname* { s u p } \{ | f ( x ) | : x \in [ 0 , 1 ] \}$ 

Hint Try to verify the parallelogram law with the functions $f , g \in C [ 0 , 1 ]$ given by $f ( x ) = 1 , g ( x ) = x$ for all x. 

## Exercise 5.6

Show that it is impossible to define an inner product on the space $L ^ { 1 } ( [ 0 , 1 ] )$ with the norm $\| \cdot \| _ { 1 }$ 

Hint Try to verify the parallelogram law with the functions given by $\begin{array} { r } { f ( x ) = \frac { 1 } { 2 } - x , g ( x ) = x - \frac { 1 } { 2 } } \end{array}$ 

## 5.2.3 Orthogonality and projections

We have introduced the concept of inner product space in a somewhat roundabout way, in order to emphasize that this structure is the natural additional tool available in the space $L ^ { 2 }$ , which remains our principal source of interest. The additional structure does, however, allow us to simplify many arguments and prove results which are not available for other function spaces. In a sense, mathematical life in $L ^ { 2 }$ is ‘as good as it gets’ in an infinite-dimensional vector space, since the structure is so similar to that of the more familiar spaces $\mathbb { R } ^ { n }$ and $\mathbb { C } ^ { n }$ 

As an example of the power of this new tool, recall that for vectors in $\mathbb { R } ^ { n }$ we have the important notion of orthogonality, which means that the scalar product of two vectors is zero. This extends to any inner product space, though we shall first state it and produce explicit examples for $L ^ { 2 }$ : the functions $f , g$ are orthogonal if 

$$
(f, g) = 0.
$$

## Example 5.4

If $f = \mathbf { 1 } _ { [ 0 , 1 ] }$ , then $( f , g ) = 0$ if and only if $\begin{array} { r } { \int _ { 0 } ^ { 1 } g ( x ) \mathrm { d } x = 0 } \end{array}$ , for example if $\begin{array} { r } { g ( x ) = x - \frac { 1 } { 2 } } \end{array}$ 

Exercise 5.7 

Show that $f ( x ) = \sin n x , g ( x ) = \cos m x { \mathrm { ~ f o r ~ } } x \in [ - \pi , \pi ]$ , and 0 outside, 

are orthogonal. 

Show that f(x) = sin nx, g(x) = sin mx for $x \in [ - \pi , \pi ]$ , and 0 outside, are orthogonal for $n \neq m$ 

In fact, in any inner product space we can define the angle between the elements g, h by setting 

$$
\cos \theta = \frac {(g , h)}{\| g \| \| h \|}.
$$

Note that by the Schwarz inequality this quantity – which, as we shall see below, also has a natural interpretation as the correlation between two (centred) random variables – lies in $[ - 1 , 1 ]$ and that $( g , h ) = 0$ means that cos θ = $\theta = 0$ , i.e. θ is an odd multiple of $\frac { \pi } { 2 }$ . It is therefore natural to say that $g$ is orthogonal to h if $( g , h ) = 0$ 

Orthogonality of vectors in a complex inner product space $\left( H , \left( \cdot , \cdot \right) \right)$ provides a way of formulating Pythagoras’ Theorem in H: since $\| g + h \| ^ { 2 } = ( g + h , g + h ) =$ $( g , g ) + ( h , h ) + ( g , h ) + ( h , g ) = \| g \| ^ { 2 } + \| h \| ^ { 2 } + ( g , h ) + ( h , g )$ we see at once that if g and h are orthogonal in H, then $\| g + h \| ^ { 2 } = \| g \| ^ { 2 } + \| h \| ^ { 2 }$ 

Now restrict attention to the case where $\left( H , \left( \cdot , \cdot \right) \right)$ is complete in the inner product norm . - recall that this means (see Definition 5.3) that if $\left( h _ { n } \right)$ is a Cauchy sequence in H then there exists $h \in H$ such that $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } \| h _ { n } = h \| = 0 } \end{array}$ As noted in Remark 5.1 we call H a Hilbert space if this holds. We content ourselves with one basic fact about such spaces: 

Let K be a complete subspace of H, so that the above condition also holds for $\left( h _ { n } \right)$ in K and then yields $h \in K$ . Just as the horizontal side of a rightangled triangle in standard position in the $( x , y ) – \mathrm { p l a n e }$ is the projection of the hypotenuse onto the horizontal axis, and the vertical side is orthogonal to that axis, we now prove the existence of orthogonal projections of a vector in H onto the subspace $K$ 

## Theorem 5.6

Let K be a complete subspace of the Hilbert space H. For each $h \in H$ we can find a unique $h ^ { \prime } \in K$ such that $h ^ { \prime \prime } = h - h ^ { \prime }$ is orthogonal to every element of K. Equivalently, $\| h - h ^ { \prime } \| = \operatorname* { i n f } \{ \| h - k \| : k \in K \}$ 

## Proof

The two conditions defining $h ^ { \prime }$ are equivalent: assume that $h ^ { \prime } \in K$ has been found so that $h ^ { \prime \prime } = h - h ^ { \prime }$ is orthogonal to every $k \in K$ . Given $k \in K$ , note that, as $( h ^ { \prime } - k ) \in K , ( h ^ { \prime \prime } , h ^ { \prime } - k ) - 0$ , so Pythagoras’ theorem implies 

$$
\| h - k \| ^ {2} = \left\| \left(h - h ^ {\prime}\right) + \left(h ^ {\prime} - k\right) \right\| ^ {2} = \left\| h ^ {\prime \prime} \right\| ^ {2} + \left\| h ^ {\prime} - k \right\| ^ {2} > \left\| h ^ {\prime \prime} \right\| ^ {2}
$$

unless $k = h ^ { \prime }$ . Hence $\| h ^ { \prime \prime } \| = \| h - h ^ { \prime } \| = \operatorname* { i n f } \{ \| h - k \| : k \in K \} = \delta _ { K }$ , say. 

Conversely, having found $h ^ { \prime } \in K$ such that $\| h - h ^ { \prime } \| = \delta _ { K }$ then for any real t and $k \in K , h ^ { \prime } + t k \in K$ , so that 

$$
\left\| h - \left(h ^ {\prime} + t k\right) \right\| ^ {2} \geq \left\| h - h ^ {\prime} \right\| ^ {2}.
$$

Multiplying out the inner products and writing $h ^ { \prime \prime } = h - h ^ { \prime }$ , this means that $- t [ ( h ^ { \prime \prime } , k ) + ( k , h ^ { \prime \prime } ) ] + t ^ { 2 } \| k \| ^ { 2 } \geq 0$ . This can only hold for all t near 0 if $( h ^ { \prime \prime } , k ) = 0$ so that $ { \boldsymbol { h } } ^ { \prime \prime } \bot  { \boldsymbol { k } }$ for every $k \in K$ 

To find $h ^ { \prime } \in K$ with $\| h - h ^ { \prime } \| = \delta _ { K }$ , first choose a sequence $\left( k _ { n } \right)$ in K such that $\| h - k _ { n } \| \to \delta _ { K } { \mathrm { a s } } n \to \infty$ . Then apply the parallelogram law (Proposition 5.5 (i)) to the vectors $\begin{array} { r } { h _ { 1 } = h - \frac 1 2 ( k _ { m } + k _ { n } ) } \end{array}$ and $\begin{array} { r } { h _ { 2 } = \frac 1 2 ( k _ { m } - k _ { n } ) } \end{array}$ Note that $h _ { 1 } + h _ { 2 } = h - k _ { n }$ and $h _ { 1 } - h _ { 2 } = h - k _ { m }$ . Hence the parallelogram law reads 

$$
\| h - k _ {n} \| ^ {2} + \| h - k _ {m} \| ^ {2} = 2 (\| h - \frac {1}{2} (k _ {m} + k _ {n}) \| ^ {2} + \| \frac {1}{2} (k _ {m} - k _ {n}) \| ^ {2})
$$

and since $\begin{array} { r } { \frac 1 2 ( k _ { m } + k _ { n } ) \in K , \| h - \frac 1 2 ( k _ { m } + k _ { n } ) \| ^ { 2 } \geq \delta _ { K } ^ { 2 } } \end{array}$ . As $m , n  \infty$ the left-hand side converges to $2 \delta _ { K } ^ { 2 }$ , hence that final term on the right must converge to 0. Thus the sequence $\left( k _ { n } \right)$ is Cauchy in K, and so converges to an element $h ^ { \prime }$ of K. But since $\| h - k _ { n } \| \to \delta _ { K }$ while $\| k _ { n } - h ^ { \prime } \| \to 0 { \mathrm { ~ a s ~ } } n \to \infty , \| h - h ^ { \prime } \| \leq$ $\| h - k _ { n } \| + \| k _ { n } - h ^ { \prime } \|$ shows that $\| h - h ^ { \prime } \| = \delta _ { K }$ . This completes the proof. 

In writing $h = h ^ { \prime } + h ^ { \prime \prime }$ we have decomposed the vector $h \in H$ as the sum of two vectors, the first being its orthogonal projection onto K, while the second is orthogonal to all vectors in K. We say that $h ^ { \prime \prime }$ is orthogonal to K, and denote the set of all vectors orthogonal to K by $K ^ { \perp }$ . This exhibits H as a direct sum $H = K \oplus K ^ { \perp }$ with each vector of the first factor being orthogonal to each vector in the second factor. 

We shall use the existence of orthogonal projections onto subspaces of $L ^ { 2 } ( \varOmega , \mathcal { F } , P )$ to construct the conditional expectation of a random variable with respect to a σ-field in Section 5.4.3. 

## Remark 5.2

The foregoing discussion barely scratches the surface of the structure of inner product spaces, such as $L ^ { 2 } ( E )$ , which is elegantly explained, for example in [10]. On the one hand, the concept of orthogonality in an inner product space leads to consideration of orthonormal sets, i.e. families $\left( e _ { \alpha } \right)$ in H that are mutually orthogonal and have norm 1. A natural question arises whether every element of H can be represented (or at least approximated) by linear combinations of the $\left( e _ { \alpha } \right)$ . In $L ^ { 2 } ( [ - \pi , \pi ] )$ this leads, for example, to Fourier series representations of functions in the form $\begin{array} { r } { f ( x ) = \sum _ { n = 0 } ^ { \infty } ( f , \psi _ { n } ) \psi _ { n } } \end{array}$ , where the orthonormal functions are $\begin{array} { r } { \psi _ { 0 } = \frac { 1 } { \sqrt { 2 \pi } } , \psi _ { 2 n } ( x ) = \frac { 1 } { \sqrt { \pi } } \cos n x , \psi _ { 2 n - 1 } ( x ) = \frac { 1 } { \sqrt { \pi } } } \end{array}$ sin nx, and the series converges in $L ^ { 2 } \mathrm { - n o r m }$ . The completeness of $L ^ { 2 }$ is crucial in ensuring the existence of such an orthonormal basis. 

## 5.3 The $L ^ { p }$ spaces: completeness

More generally, the space $L ^ { p } ( E )$ is obtained when we integrate the $p ^ { t h }$ powers of $| f |$ . For $p \geq 1$ , we say that $f \in L ^ { p }$ (and similarly for $L ^ { p } ( E )$ and $L ^ { p } ( E , \mathbb { C } ) )$ ) if $| f | ^ { p }$ is integrable (with the same convention of identifying f and g when they are a.e. equal). Some work will be required to check that $L ^ { p }$ is a vector space and that the ‘natural’ generalization of the norm introduced for $L ^ { 2 }$ is in fact a norm. We shall need $p \geq 1$ to achieve this. 

## Definition 5.5

For each $p \geq 1 , p < \infty$ , we define (identifying classes and functions) 

$$
L ^ {p} (E) = \{f: \int_ {E} | f | ^ {p} \mathrm{d} m \text { is   finite } \}
$$

and the norm on $L ^ { p }$ is defined by 

$$
\| f \| _ {p} = \left(\int_ {E} | f | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}}.
$$

(With this in mind, we denoted the norm in $L ^ { 1 } ( E )$ by $\| f \|$ <sub>1</sub> and that in $L ^ { 2 } ( E )$ by $\| f \| _ { 2 } . )$ 

Recall Definition 3.2: for any measurable function $f : E \to [ 0 , \infty ]$ 

$$
\text { ess   sup } f := \inf \{c: | f | \leq c \text {   a.e. } \}.
$$

More precisely, if $F = \{ c \geq 0 : m \{ | f | ^ { - 1 } ( ( c , \infty ] ) \} = 0 \}$ , we set ess $\operatorname* { s u p } f = \operatorname { i n f } F$ (with the convention inf $\ 0 = + \infty )$ . It is easy to see that the infimum belongs to F. 

## Definition 5.6

A measurable function f satisfying ess $\operatorname { s u p } | f | < \infty$ is said to be essentially bounded and the set of all essentially bounded functions on E is denoted by $L ^ { \infty } ( E )$ (again with the usual identification of functions with a.e. equivalence classes), with the norm $\left| \left| f \right| \right| _ { \infty } = \mathrm { e s s \ s u p } f$ 

It is clear from Proposition 3.9 and the obvious identity ess $\operatorname* { s u p } ( c f ) =$ $c ( \cos \operatorname* { s u p } f )$ that $L ^ { \infty } ( E )$ is a vector space. 

We shall need to justify the notation by showing that for each $p \ ( 1 \leq p \leq$ $\infty ) , ( L ^ { p } ( E ) , \parallel \cdot \parallel )$ is a normed vector space. 

First we observe that $L ^ { p } ( E )$ is a vector space for $1 \leq p < \infty$ . If f and $g$ belong to $L ^ { p }$ , then they are measurable, hence so are $c f$ and $f + g$ . We have $| c f ( x ) | ^ { p } = | c | ^ { p } | f ( x ) | ^ { p }$ hence 

$$
\| c f \| _ {p} = \left(\int | c f (x) | ^ {p} \mathrm{d} x\right) ^ {\frac {1}{p}} = | c | \left(\int | f (x) | ^ {p} \mathrm{d} x\right) ^ {\frac {1}{p}} = | c | \| f \| _ {p}.
$$

Next $| f ( x ) + g ( x ) | ^ { p } \leq 2 ^ { p } \operatorname* { m a x } \{ | f ( x ) | ^ { p } , | g ( x ) | ^ { p } \}$ and so $\| f + g \| _ { p }$ is finite if only $\| f \| _ { p }$ and $\| g \| _ { p }$ are. Moreover, if $\| f \| _ { p } = 0$ then $| f ( x ) | ^ { p } = 0$ almost everywhere and so $f ( x ) = 0$ almost everywhere. The converse is obvious. 

The triangle inequality 

$$
\| f + g \| _ {p} \leq \| f \| _ {p} + \| g \| _ {p}
$$

is by no means obvious for general $p \geq 1$ : we need to derive a famous inequality due to H¨older, which is also extremely useful in many contexts, and generalizes the Schwarz inequality. 

## Remark 5.3

Before tackling this, we observe that the case of $L ^ { \infty } ( E )$ is rather easier: $| f + g | \leq$ $| f | + | g |$ at once implies that $\| f + g \| _ { \infty } \leq \| f \| _ { \infty } + \| g \| _ { \infty }$ and similarly $| a f | = | a | | f |$ gives $\| a f \| _ { \infty } = \| a \| \| f \| _ { \infty }$ . Thus $L ^ { \infty } ( E )$ is a vector space and since $\| f \| _ { \infty } = 0$ obviously holds if and only if $f = 0 \ { \mathrm { a . e . } }$ , it follows that $\| \cdot \| _ { \infty }$ is a norm on $L ^ { \infty } ( E )$ .Exercises 3.6 and 5.6 show that this norm cannot be induced by any inner product on $L ^ { \infty }$ 

## Lemma 5.7

For any non-negative real numbers x, y and all $\alpha , \beta \in ( 0 , 1 )$ with $\alpha + \beta = 1$ we have 

$$
x ^ {\alpha} y ^ {\beta} \leq \alpha x + \beta y.
$$

## Proof

If $x = 0$ the claim is obvious. So take $x > 0$ . Consider $f ( t ) = ( 1 - \beta ) + \beta t - t ^ { \beta }$ for $t \geq 0$ and β as given. We have $f ^ { \prime } ( t ) = \beta - \beta t ^ { \beta - 1 } = \beta ( 1 - t ^ { \beta - 1 } )$ and since $0 < \beta < 1 , f ^ { \prime } ( t ) < 0$ on (0,1). So f decreases on $[ 0 , 1 ]$ while $f ^ { \prime } ( t ) > 0$ on $( 1 , \infty )$ 2 hence f increases on $[ 1 , \infty )$ . So $f ( 1 ) = 0$ is the only minimum point of f on $[ 0 , \infty )$ , that is $f ( t ) \geq 0$ for $t \geq 0$ . Now set $\begin{array} { r } { t = \frac { y } { x } } \end{array}$ , then $\begin{array} { r } { ( 1 - \beta ) + \beta \frac { y } { x } - \left( \frac { y } { x } \right) ^ { \beta } \geq 0 } \end{array}$ 2 that is, $\begin{array} { r } { \left( \frac { y } { x } \right) ^ { \beta } \leq \alpha + \beta \frac { y } { x } } \end{array}$ . Writing $x = x ^ { \alpha + \beta }$ we have $\begin{array} { r } { x ^ { \alpha + \beta } \left( \frac { y } { x } \right) ^ { \beta } \leq \alpha x + \beta x \frac { y } { x } } \end{array}$ so that $x ^ { \alpha } y ^ { \beta } \leq \alpha x + \beta y$ as required. □ 

## Theorem 5.8 (H¨older’s Inequality)

If $\textstyle { \frac { 1 } { p } } + { \frac { 1 } { q } } = 1 , p > 1$ , then for $f \in L ^ { p } ( E ) , g \in L ^ { q } ( E )$ , we have $f g \in L ^ { 1 }$ and 

$$
\| f g \| _ {1} \leq \| f \| _ {p} \| g \| _ {q}
$$

that is 

$$
\int | f \overline {{g}} | \mathrm{d} m \leq \left(\int | f | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}} \left(\int | g | ^ {q} \mathrm{d} m\right) ^ {\frac {1}{q}}.
$$

## Proof

Step 1. Assume that $\| f \| _ { p } = \| g \| _ { q } = 1$ , so we only need to show that $\| f g \| _ { 1 } \leq 1$ We apply Lemma 5.7 with $\begin{array} { r } { \alpha = \frac { 1 } { p } , \beta = \frac { 1 } { q } , x = | f | ^ { p } , y = | g | ^ { q } } \end{array}$ , then we have 

$$
| f \overline {{g}} | = x ^ {\frac {1}{p}} y ^ {\frac {1}{q}} \leq \frac {1}{p} | f | ^ {p} + \frac {1}{q} | g | ^ {q}.
$$

Integrating we obtain 

$$
\int | f g | \mathrm{d} m \leq \frac {1}{p} \int | f | ^ {p} \mathrm{d} m + \frac {1}{q} \int | g | ^ {q} \mathrm{d} m = \frac {1}{p} + \frac {1}{q} = 1
$$

since $\begin{array} { r } { \int | f | ^ { p } \mathrm { d } m = 1 , \int | g | ^ { q } \mathrm { d } m = 1 } \end{array}$ . So we have $\| f g \| _ { 1 } \leq 1$ as required. 

Step 2. For general $f \in L ^ { p }$ and $g \in L ^ { q }$ we write $\| f \| _ { p } = a , \| g \| _ { q } = b$ for some $a , b > 0$ . (If either a or b is zero, then one of the functions is zero almost everywhere and the inequality is trivial.) Hence the functions $\begin{array} { r } { \tilde { f } = \frac { 1 } { a } f , \tilde { g } = \frac { 1 } { b } g } \end{array}$ satisfy the assumption of Step 1, and so $\| \tilde { f } \tilde { g } \| _ { 1 } \le \| \tilde { f } \| _ { p } \| \tilde { g } \| _ { q }$ . This yields 

$$
\frac {1}{a b} \| f g \| _ {1} \leq \frac {1}{a} \| f \| _ {p} \frac {1}{b} \| g \| _ {q}
$$

and after multiplying by ab the result is proved. 

Letting $p = q = 2$ and recalling the definition of the scalar product in $L ^ { 2 }$ we obtain the following now familiar special case of H¨older’s inequality. 

## Corollary 5.9 (Schwarz Inequality)

If $f , g \in L ^ { 2 }$ , then 

$$
| (f, g) | \leq \| f \| _ {2} \| g \| _ {2}.
$$

We may now complete the verification that $\| \cdot \| _ { p }$ is a norm on $L ^ { p } ( E )$ 

## Theorem 5.10 (Minkowski’s Inequality)

For each $p \geq 1 , f , g \in L ^ { p } ( E )$ 

$$
\| f + g \| _ {p} \leq \| f \| _ {p} + \| g \| _ {p}.
$$

Proof 

Assume $1 < p < \infty$ (the case $p = 1$ was done earlier). We have 

$$
| f + g | ^ {p} = | (f + g) (f + g) ^ {p - 1} | \leq | f \| f + g | ^ {p - 1} + | g \| f + g | ^ {p - 1},
$$

and also taking q such that $\textstyle { \frac { 1 } { p } } + { \frac { 1 } { q } } = 1$ , in other words, $p + q = p q$ , we obtain 

$$
| f + g | ^ {(p - 1) q} = | f + g | ^ {p} <   \infty .
$$

Hence $( f + g ) ^ { p - 1 } \in L ^ { q }$ and 

$$
\| (f + g) ^ {p - 1} \| _ {q} = \left(\int | f + g | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{q}}.
$$

We may apply H¨older’s inequality: 

$$
\begin{array}{l} \int | f + g | ^ {p} \mathrm{d} m \leq \int | f \| f + g | ^ {p - 1} \mathrm{d} m + \int | g \| f + g | ^ {p - 1} \mathrm{d} m \\ \qquad \qquad \qquad \qquad \leq \left(\int | f | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}} \left(\int | f + g | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{q}} \\ \qquad \qquad \qquad + \left(\int | g | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}} \left(\int | f + g | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{q}} \\ \qquad = \left(\left(\int | f | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}} + \left(\int | g | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}}\right) \cdot A \end{array}
$$

with $\begin{array} { r } { A = \left( \int | f + g | ^ { p } \mathrm { d } m \right) ^ { \frac { 1 } { q } } } \end{array}$ . If $A = 0$ then $\| f + g \| _ { p } = 0$ and there is nothing to prove. So suppose $A > 0$ and divide by A 

$$
\begin{array}{l} \| f + g \| _ {p} = \left(\int | f + g | ^ {p} \mathrm{d} m\right) ^ {1 - \frac {1}{q}} \\ \quad = \frac {1}{A} \left(\int | f + g | ^ {p} \mathrm{d} m\right) \\ \quad \leq \left(\int | f | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}} + \left(\int | g | ^ {p} \mathrm{d} m\right) ^ {\frac {1}{p}} \\ \quad = \| f \| _ {p} + \| g \| _ {p} \end{array}
$$

which was to be proved. 

Next we prove that $L ^ { p } ( E )$ is an example of a complete normed space (i.e. a Banach space) for $1 < p < \infty$ , i.e. that every Cauchy sequence in $L ^ { p } ( E )$ converges in norm to an element of $L ^ { p } ( E )$ . We sometimes refer to convergence of sequences in the $L ^ { p } { \mathrm { - n o r m } }$ as convergence in $p ^ { t h }$ mean. 

The proof is quite similar to the case $p = 1$ 

## Theorem 5.11

The space $L ^ { p } ( E )$ is complete for $1 < p < \infty$ 

## Proof

Given a Cauchy sequence $f _ { n }$ (that is, $\| f _ { n } - f _ { m } \| _ { p } \to 0 { \mathrm { ~ a s ~ } } n , m \to \infty )$ we find a subsequence $f _ { n _ { k } }$ with 

$$
\| f _ {n} - f _ {n _ {k}} \| _ {p} <   \frac {1}{2 ^ {k}}
$$

for all $k \geq 1$ and we set 

$$
g _ {k} = \sum_ {i = 1} ^ {k} | f _ {n _ {i + 1}} - f _ {n _ {i}} |, \quad g = \lim _ {k \rightarrow \infty} g _ {k} = \sum_ {i = 1} ^ {\infty} | f _ {n _ {i + 1}} - f _ {n _ {i}} |.
$$

The triangle inequality yields $\begin{array} { r } { \| g _ { k } \| _ { p } \leq \sum _ { i = 1 } ^ { k } \frac { 1 } { 2 ^ { i } } < 1 } \end{array}$ and we can apply Fatou’s Plemma to the non-negative measurable functions $g _ { k } ^ { p } , k \geq 1$ , so that 

$$
\| g \| _ {p} ^ {p} = \int \lim _ {n \to \infty} g _ {k} ^ {p}   \mathrm{d} m \leq \operatorname * {l i m i n f} _ {k \to \infty} \int g _ {k} ^ {p}   \mathrm{d} m \leq 1.
$$

Hence g is almost everywhere finite and $\begin{array} { r } { f _ { n _ { 1 } } + \sum _ { i > 1 } ( f _ { n _ { i + 1 } } - f _ { n _ { i } } ) } \end{array}$ converges Pabsolutely almost everywhere, defining a measurable function f as its sum. 

We need to show that $f \in L ^ { p }$ . Note first that $f = \operatorname* { l i m } _ { k \to \infty } f _ { n _ { k } } { \mathrm { ~ a . e . } }$ , and given $\varepsilon > 0$ we can find N such that $\| f _ { n } - f _ { m } \| _ { p } < \varepsilon$ for $m , n \geq N$ . Applying Fatou’s lemma to the sequence $\left( | f _ { n _ { i } } - f _ { m } | ^ { p } \right) _ { i \geq 1 }$ , letting $i \to \infty$ , we have 

$$
\int | f - f _ {m} | ^ {p}   \mathrm{d} m \leq \operatorname * {l i m i n f} _ {i \to \infty} \int | f _ {n _ {i}} - f _ {m} | ^ {p}   \mathrm{d} m \leq \varepsilon^ {p}.
$$

Hence $f - f _ { m } \in L ^ { p }$ and so $f = f _ { m } + ( f - f _ { m } ) \in L ^ { p }$ and we have $\| f - f _ { m } \| _ { p } < \varepsilon$ for all $m \geq N$ . Thus $f _ { m } \to f$ in $L ^ { p } .$ -norm as required. □ 

The space $L ^ { \infty } ( E )$ is also complete, since for any Cauchy sequence $\left( f _ { n } \right)$ in $L ^ { \infty } ( E )$ the union of the null sets where $| f _ { k } ( x ) | > \| f \| _ { \infty } { \mathrm { ~ o r ~ } } | f _ { n } ( x ) - f _ { m } ( x ) | >$ $\| f _ { n } - f _ { m } \| _ { \infty }$ for $k , m , n \in \mathbb { N } ,$ is still a null set, F say. Outside F the sequence $\left( f _ { n } \right)$ converges uniformly to a bounded function, f say. It is clear that $\| f _ { n } - f \| _ { \infty } \to 0$ and $f \in L ^ { \infty } ( E )$ , so we are done. 

Exercise 5.8 

Is the sequence 

$$
g _ {n} (x) = \mathbf {1} _ {(0, \frac {1}{n} ]} (x) \frac {1}{\sqrt {x}}
$$

Cauchy in $L ^ { 4 \gamma }$ 

We have the following relations between the $L ^ { p }$ spaces for diferent p which generalize Proposition 5.3. 

## Theorem 5.12

If E has finite Lebesgue measure, then $L ^ { q } ( E ) \subseteq L ^ { p } ( E )$ when $1 \leq p \leq q \leq \infty$ 

Proof 

Note that $| f ( x ) | ^ { p } \leq 1 { \mathrm { ~ i f ~ } } | f ( x ) | \leq 1 . { \mathrm { ~ I f ~ } } | f ( x ) | \geq 1$ , then $| f ( x ) | ^ { p } \leq | f ( x ) | ^ { q }$ . Hence 

$$
| f (x) | ^ {p} \leq 1 + | f (x) | ^ {q},
$$

$$
\int_ {E} | f | ^ {p} \mathrm{d} m \leq \int_ {E} 1 \mathrm{d} m + \int_ {E} | f | ^ {q} \mathrm{d} m = m (E) + \int_ {E} | f | ^ {q} \mathrm{d} m <   \infty ,
$$

so if $m ( E )$ and $\textstyle \int _ { E } | f | ^ { q }$ dm are finite, the same is true for $\int _ { E } | f | ^ { p } \mathrm { d } m$ □ 

## 5.4 Probability

## 5.4.1 Moments

Random variables belonging to spaces $L ^ { p } ( \varOmega )$ , where the exponent $p \in \mathbb N$ , play an important role in probability. 

## Definition 5.7

The moment of order n of a random variable $X \in L ^ { n } ( \varOmega )$ is the number 

$$
\mathbb {E} (X ^ {n}), \quad n = 1, 2, \ldots
$$

Write $\mathbb { E } ( X ) = \mu ;$ then central moments are given by 

$$
\mathbb {E} (X - \mu) ^ {n}, \quad n = 1, 2, \ldots
$$

By Theorem 4.28 moments are determined by the probability distribution: 

$$
\mathbb {E} (X ^ {n}) = \int x ^ {n} \mathrm{d} P _ {X} (x),
$$

$$
\mathbb {E} ((X - \mu) ^ {n}) = \int (x - \mu) ^ {n} \mathrm{d} P _ {X} (x),
$$

and if X has a density $f _ { X }$ then by Theorem 4.32 we have 

$$
\mathbb {E} (X ^ {n}) = \int x ^ {n} f _ {X} (x) \mathrm{d} x,
$$

$$
\mathbb {E} ((X - \mu) ^ {n}) = \int (x - \mu) ^ {n} f _ {X} (x) \mathrm{d} x.
$$

## Proposition 5.13

If E(X<sup>n</sup>) is finite for some n, then for $k \le n , \mathbb { E } ( X ^ { k } )$ are finite. If $\mathbb { E } ( X ^ { n } )$ is infinite, then the same is true for $\mathbb { E } ( X ^ { k } )$ for $k \geq n$ 

Hint Use Theorem 5.12. 

Exercise 5.9 

Find X so that $\mathbb { E } ( X ^ { 2 } ) = \infty , \mathbb { E } ( X ) < \infty$ . Can such an X have $\mathbb { E } ( X ) = 0 ?$ 

Hint You may use some previous examples in this chapter. 

## Definition 5.8

The variance of a random variable is the central moment of second order: 

$$
\operatorname{Var} (X) = \mathbb {E} (X - \mathbb {E} (X)) ^ {2}.
$$

Clearly, writing $\mu = \operatorname { \mathbb { E } } ( X )$ 

$$
\operatorname{Var} (X) = \mathbb {E} (X ^ {2} - 2 \mu X + \mu^ {2}) = \mathbb {E} (X ^ {2}) - 2 \mu \mathbb {E} (X) + \mu^ {2} = \mathbb {E} (X ^ {2}) - \mu^ {2}.
$$

This shows that the first two moments determine the second central moment. This may be generalized to arbitrary order and what is more, this relationship also goes the other way round. 

## Proposition 5.14

Central moments of order n are determined by moments of order k for $k \leq n$ 

Hint Use the binomial theorem and linearity of the integral. 

## Proposition 5.15

Moments of order n are determined by central moments of order k for $k \leq n$ 

Hint Write $\mathbb { E } ( X ^ { n } )$ as $\mathbb { E } ( ( X - \mu + \mu ) ^ { n } )$ and then use the binomial theorem. 

Exercise 5.10 

Find Var(aX) in terms of Var(X). 

## Example 5.5

If X has the uniform distribution on [a, b], that is, $\begin{array} { r } { f _ { X } ( x ) = \frac { 1 } { b - a } \mathbf { 1 } _ { [ a , b ] } ( x ) } \end{array}$ then 

$$
\int x f _ {X} (x) \mathrm{d} x = \frac {1}{b - a} \int_ {a} ^ {b} x \mathrm{d} x = \frac {1}{b - a} \frac {1}{2} x ^ {2} | _ {a} ^ {b} = \frac {1}{2} (a + b).
$$

Exercise 5.11 

Show that for uniformly distributed X, $\textstyle \operatorname { V a r } X = { \frac { 1 } { 1 2 } } ( b - a ) ^ { 2 }$ 

Exercise 5.12 

Find the variance of 

(a) a constant random variable X, $X ( \omega ) = a$ for all $\omega$ 

(b) $X : [ 0 , 1 ] \to \mathbb { R }$ given by $X ( \omega ) = \operatorname* { m i n } \{ \omega , 1 - \omega \}$ (the distance to the nearest endpoint of the interval [0, 1]) 

(c) $X : [ 0 , 1 ] ^ { 2 } \to \mathbb { R }$ , the distance to the nearest edge of the square $[ 0 , 1 ] ^ { 2 }$ 

We shall see that for the Gaussian distribution the first two moments determine the remaining ones. First we compute the expectation: 

Theorem 5.16 

$$
\frac {1}{\sqrt {2 \pi} \sigma} \int_ {\mathbb {R}} x \mathrm{e} ^ {- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}} \mathrm{d} x = \mu .
$$

Proof 

Make the substitution $\begin{array} { r } { z = \frac { x - \mu } { \sigma } } \end{array}$ , then, writing for $\textstyle \int _ { \mathbb { R } } .$ 

$$
\frac {1}{\sqrt {2 \pi} \sigma} \int x \mathrm{e} ^ {- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}} \mathrm{d} x = \frac {\sigma}{\sqrt {2 \pi}} \int z \mathrm{e} ^ {- \frac {z ^ {2}}{2}} \mathrm{d} z + \frac {\mu}{\sqrt {2 \pi}} \int \mathrm{e} ^ {- \frac {z ^ {2}}{2}} \mathrm{d} z.
$$

Notice that the first integral is zero since the integrand is an odd function. The second integral is $\sqrt { 2 \pi }$ , hence the result. □ 

So the parameter $\mu$ in the density is the mathematical expectation. We show now that $\sigma ^ { 2 }$ is the variance. 

Theorem 5.17 

$$
\frac {1}{\sqrt {2 \pi} \sigma} \int_ {\mathbb {R}} (x - \mu) ^ {2} \mathrm{e} ^ {- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}} \mathrm{d} x = \sigma^ {2}.
$$

Proof 

Make the same substitution as before: $\begin{array} { r } { z = \frac { x - \mu } { \sigma } } \end{array}$ ; then 

$$
\frac {1}{\sqrt {2 \pi} \sigma} \int (x - \mu) ^ {2} \mathrm{e} ^ {- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}} \mathrm{d} x = \frac {\sigma^ {2}}{\sqrt {2 \pi}} \int z ^ {2} \mathrm{e} ^ {- \frac {z ^ {2}}{2}} \mathrm{d} z.
$$

Integrate by parts $u = z , v = z \mathrm { e } ^ { - z ^ { 2 } / 2 }$ <sup>2</sup>, to get 

$$
\frac {\sigma^ {2}}{\sqrt {2 \pi}} \int z ^ {2} \mathrm{e} ^ {- \frac {z ^ {2}}{2}} \mathrm{d} z = - \frac {\sigma^ {2}}{\sqrt {2 \pi}} z \mathrm{e} ^ {- \frac {z ^ {2}}{2}} \Big | _ {- \infty} ^ {+ \infty} + \frac {\sigma^ {2}}{\sqrt {2 \pi}} \int \mathrm{e} ^ {- \frac {z ^ {2}}{2}} \mathrm{d} z = \sigma^ {2}
$$

since the first term vanishes. 

Note that the odd central moments for a Gaussian random variable are zero: the integrals 

$$
\frac {1}{\sqrt {2 \pi} \sigma} \int (x - \mu) ^ {2 k + 1} \mathrm{e} ^ {- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}} \mathrm{d} x
$$

vanish since after the above substitution we integrate an odd function. By repeating the integration by parts argument one can prove that 

$$
\mathbb {E} (X - \mu) ^ {2 k} = 1 \cdot 3 \cdot 5 \dots (2 k - 1) \sigma^ {k}.
$$

## Example 5.6

Let us consider the Cauchy density $\textstyle { \frac { 1 } { \pi } } { \frac { 1 } { 1 + x ^ { 2 } } }$ and try to compute the expectation (we shall see it is impossible): 

$$
\frac {1}{\pi} \int_ {- \infty} ^ {+ \infty} \frac {x}{1 + x ^ {2}} \mathrm{d} x = \frac {1}{2 \pi} \left(\lim _ {x _ {n} \rightarrow + \infty} \ln (1 + x _ {n} ^ {2}) - \lim _ {y _ {n} \rightarrow - \infty} \ln (1 + y _ {n} ^ {2})\right)
$$

for some sequences $x _ { n } , \ y _ { n }$ . The result, if finite, should not depend on their choice, however if we set for example $x _ { n } = a y _ { n }$ , then we have 

$$
\left(\lim _ {x _ {n} \to + \infty} \ln (1 + x _ {n} ^ {2}) - \lim _ {y _ {n} \to - \infty} \ln (1 + y _ {n} ^ {2})\right) = \lim _ {y _ {n} \to \infty} \ln {\frac {1 + a y _ {n} ^ {2}}{1 + y _ {n} ^ {2}}} = \ln a
$$

which is a contradiction. As a consequence, we see that for the Cauchy density the moments do not exist. 

## Remark 5.4

We give without proof a simple relation between the characteristic function and the moments: (Recall that $\varphi _ { X } ( t ) = \mathbb { E } ( e ^ { i t X } )$ – see Definition 4.5.) 

If $\varphi _ { X }$ is k-times continuously diferentiable then X has finite kth moment and 

$$
\mathbb {E} (X ^ {k}) = \frac {1}{i ^ {k}} \frac {d ^ {k}}{d t ^ {k}} \varphi_ {X} (0).
$$

Conversely, if X has kth moment finite then $\varphi _ { X } ( t )$ is k-times diferentiable and the above formula holds. 

## 5.4.2 Independence

The expectation provides a useful criterion for the independence of two random variables. 

## Theorem 5.18

The random variables $X , Y$ are independent if and only if 

$$
\mathbb {E} (f (X) g (Y)) = \mathbb {E} (f (X)) \mathbb {E} (g (Y))\tag{5.4}
$$

holds for all Borel measurable bounded functions $f , g .$ 

## Proof

Suppose that (5.4) holds and take any Borel sets $B _ { 1 } , B _ { 2 }$ . Let $f = \mathbf { 1 } _ { B _ { 1 } } , g = \mathbf { 1 } _ { B _ { 2 } }$ and application of (5.4) gives 

$$
\int_ {\Omega} \mathbf {1} _ {B _ {1}} (X (\omega)) \mathbf {1} _ {B _ {2}} (Y (\omega)) \mathrm{d} P (\omega) = \int_ {\Omega} \mathbf {1} _ {B _ {1}} (X (\omega)) \mathrm{d} P (\omega) \int_ {\Omega} \mathbf {1} _ {B _ {2}} (Y (\omega)) \mathrm{d} P (\omega).
$$

The left-hand side equals 

$$
\int_ {\Omega} \mathbf {1} _ {B _ {1} \times B _ {2}} (X (\omega), Y (\omega)) \mathrm{d} P (\omega) = P ((X \in B _ {1}) \cap (Y \in B _ {2})),
$$

whereas the right-hand side is $P ( X \in B _ { 1 } ) P ( Y \in B _ { 2 } )$ , thus proving the inde pendence of X and $Y$ . 

Suppose now that $X , Y$ are independent. Then (5.4) holds for $f = \mathbf { 1 } _ { B _ { 1 } }$ ， $g = { \bf 1 } _ { B _ { 2 } } , B _ { 1 } , B _ { 2 }$ Borel sets, by the above argument. By linearity we extend the formula to simple functions: $\begin{array} { r } { \varphi = \sum b _ { i } \mathbf { 1 } _ { B _ { i } } , \psi = \sum _ { j } c _ { j } \mathbf { 1 } _ { C _ { j } } } \end{array}$ 2 

$$
\begin{array}{l} \mathbb {E} (\varphi (X) \psi (Y)) = \mathbb {E} (\sum b _ {i} \mathbf {1} _ {B _ {i}} (X) \sum c _ {j} \mathbf {1} _ {C _ {j}} (Y)) \\ \qquad = \sum_ {i, j} b _ {i} c _ {j} \mathbb {E} (\mathbf {1} _ {B _ {i}} (X) \mathbf {1} _ {C _ {j}} (Y)) \\ \qquad = \sum_ {i, j} b _ {i} c _ {j} \mathbb {E} (\mathbf {1} _ {B _ {i}} (X)) \mathbb {E} (\mathbf {1} _ {C _ {j}} (Y)) \\ \qquad = \sum_ {i} b _ {i} \mathbb {E} (\mathbf {1} _ {B _ {i}} (X)) \sum_ {j} c _ {j} \mathbb {E} (\mathbf {1} _ {C _ {j}} (Y)) \\ \qquad = \mathbb {E} (\varphi (X)) \mathbb {E} (\psi (Y)). \end{array}
$$

We approximate general $f , g$ by simple functions and the dominated convergence theorem $( f , g$ are bounded) extends the formula to $f , g .$ □ 

## Proposition 5.19

Assume that X, Y are independent random variables. Show that if $\mathbb { E } ( X ) = 0$ $\mathbb { E } ( Y ) = 0$ , then $\mathbb { E } ( X Y ) = 0$ 

Hint The above theorem cannot be applied with $f ( x ) = x , g ( x ) = x$ (these functions are not bounded). So some approximation is required. 

The expectation is nothing but an integral so the number $( X , Y ) = \mathbb { E } ( X Y )$ is the inner product in the space $L ^ { 2 } ( \varOmega )$ of random variables square integrable with respect to P. Hence independence implies orthogonality in this space. If the expectation of a random variable is non-zero, we modify the notion of orthogonality. The idea is that adding (or subtracting) a number does not destroy or improve independence. 

## Definition 5.9

For a random variable with finite $\mu = \operatorname { \mathbb { E } } ( X )$ we write $X _ { c } = X - \mathbb { E } ( X )$ and we call $X _ { c }$ a centred random variable $( \mathrm { c l e a r l y ~ } \mathbb { E } ( X _ { c } ) = 0 )$ . The covariance of X and Y is defined as 

$$
\operatorname{Cov} (X, Y) = \left(X _ {c}, Y _ {c}\right) = \mathbb {E} \bigl ((X - \mathbb {E} (X)) (Y - \mathbb {E} (Y)) \bigr).
$$

The correlation is the cosine of the angle between $X _ { c }$ and $Y _ { c }$ : 

$$
\rho_ {X, Y} = \frac {\left(X _ {c} , Y _ {c}\right)}{\| X \| _ {2} \| Y \| _ {2}} = \frac {\operatorname{Cov} (X , Y)}{\| X \| _ {2} \| Y \| _ {2}}.
$$

We say that $X , Y$ are uncorrelated if $\rho = 0$ 

Note that some elementary algebra gives a more convenient expression for the covariance: 

$$
\operatorname{Cov} (X, Y) = \mathbb {E} (X Y) - \mathbb {E} (X) \mathbb {E} (Y).
$$

Thus uncorrelated X, Y satisfy $\mathbb { E } ( X Y ) \ : = \ : \mathbb { E } ( X ) \mathbb { E } ( Y )$ . Clearly independent random variables are uncorrelated; it is suficient to take $f ( x ) = x - \mathbb { E } ( X )$ 2 $g ( x ) = x - \mathbb { E } ( Y )$ in Theorem 5.18. The converse is not true in general, although – as we shall see in Chapter 6 – it holds for Gaussian random variables. 

## Example 5.7

Let $\varOmega = [ - 1 , 1 ]$ with Lebesgue measure: $P = \textstyle { \frac { 1 } { 2 } } m | _ { [ - 1 , 1 ] } , \ X = \ x , \ Y = \ x ^ { 2 }$ Then $\begin{array} { r } { \mathbb { E } ( X ) = 0 , \mathbb { E } ( X Y ) = \int _ { - 1 } ^ { 1 } x ^ { 3 } { \mathrm { d } } x = 0 } \end{array}$ , hence $C o v ( X , Y ) = 0$ and thus $\rho _ { X , Y } = 0$ R. However X, Y are not independent. Intuitively this is clear since 

$Y = X ^ { 2 }$ , so that each of X, Y is a function of the other. Specifically, take $A = B = [ - \frac { 1 } { 2 } , \frac { 1 } { 2 } ]$ and compare (as required by Definition 3.3) the probabilities $P ( X ^ { - 1 } ( A ) \cap Y ^ { - 1 } ( A ) )$ and $P ( X ^ { - 1 } ( A ) ) P ( Y ^ { - 1 } ( A ) )$ . We obtain $X ^ { - 1 } ( A ) = A$ 2 $Y ^ { - 1 } ( A ) = [ - \frac { 1 } { \sqrt { 2 } } , \frac { 1 } { \sqrt { 2 } } ]$ , hence $\begin{array} { r } { P ( X ^ { - 1 } ( A ) \cap Y ^ { - 1 } ( A ) ) = \frac { 1 } { \sqrt { 2 } } , P ( X ^ { - 1 } ( A ) ) = \frac { 1 } { 2 } } \end{array}$ $\begin{array} { r } { P ( Y ^ { - 1 } ( A ) ) = \frac { \overset { . } { \sqrt { 2 } } } { \sqrt { 2 } } } \end{array}$ and so X and Y are not independent. 

## Exercise 5.13

Find the correlation $\rho _ { X , Y }$ if $X = 2 Y + 1$ 

## Exercise 5.14

Take $\varOmega = [ 0 , 1 ]$ with Lebesgue measure and let $X ( \omega ) = \sin 2 \pi \omega , Y ( \omega ) =$ cos $2 \pi \omega$ . Show that X, Y are uncorrelated but not independent. 

We close the section with two further applications. 

## Proposition 5.20

The variance of the sum of uncorrelated random variables is the sum of their variances: 

$$
\operatorname{Var} (\sum_ {i = 1} ^ {n} X _ {i}) = \sum_ {i = 1} ^ {n} \operatorname{Var} (X _ {i}).
$$

Hint To avoid cumbersome notation first prove the formula for two random variables 

$$
\operatorname{Var} (X + Y) = \operatorname{Var} (X) + \operatorname{Var} (Y)
$$

using the formula $\operatorname { V a r } ( X ) = \mathbb { E } ( X ^ { 2 } ) - ( \mathbb { E } X ) ^ { 2 }$ 

## Proposition 5.21

Suppose that X, Y are independent random variables. Then we have the following formula for the characteristic function: 

$$
\varphi_ {X + Y} (t) = \varphi_ {X} (t) \varphi_ {Y} (t).
$$

More generally, if $X _ { 1 } , \ldots , X _ { n }$ are independent, then 

$$
\varphi_ {X _ {1} + \dots + X _ {n}} (t) = \varphi_ {X _ {1}} (t) \cdot \cdot \cdot \varphi_ {X _ {n}} (t).
$$

Hint Use the definition of characteristic functions and Theorem 5.18. 

## 5.4.3 Conditional Expectation (first construction)

The construction of orthogonal projections in complete inner product spaces, undertaken in Section 5.2.3, allows us to provide a preview of perhaps the most important concept in modern probability theory: the conditional expectation of an ${ \mathcal { F } } .$ measurable integrable random variable X, given a $\sigma \mathrm { - }$ field $\mathcal { G }$ contained in $\mathcal { F }$ (i.e. such that every set in $\mathcal { G }$ also belongs to $\mathcal { F } )$ . We study this idea in detail in Chapter $7$ where we will also justify the definition below by reference to more familiar concepts, but the construction of the conditional expectation as a -measurable random variable can be achieved for any integrable X with the tools we have readily to hand. Our argument owes much to the elegant construction given in [12]. 

## Definition 5.10

Let $( \varOmega , \mathcal { F } , P )$ be a probability space and suppose that $\mathcal { G }$ is a sub-σ-field of $\mathcal { F }$ Given $X \in \mathcal { L } ^ { 1 } ( \varOmega , \mathcal { F } , P ) = \mathcal { L } ^ { 1 } ( \mathcal { F } )$ there exists $Y \in \mathcal { L } ^ { 1 } ( \varOmega , \mathcal { G } , P ) = \mathcal { L } ^ { 1 } ( \mathcal { G } )$ such that $\textstyle \int _ { G } Y \mathrm { d } P = \int _ { G } X \mathrm { d } P $ for every $G \in { \mathcal { G } }$ . We write $Y = \mathbb { E } ( X | \mathcal { G } )$ and call $Y$ R Rthe conditional expectation of X given $\mathcal { G }$ . These conditions define Y uniquely up to P-null sets. 

Theorem 4.15, applied to P instead of m and $\mathcal { G }$ instead of $\mathcal { M } .$ , implies that $Y$ is $P \mathrm { - a . s }$ . unique: if $Z \in { \mathcal { L } } ^ { 1 } ( { \mathcal { G } } )$ also satisfies $\textstyle \int _ { G } Z \mathrm { d } P = \int _ { G } X \mathrm { d } P $ for every $G \in { \mathcal { G } }$ , then $Z = Y \ P \mathrm { - a . s }$ R R. This is often expressed by saying that $Y$ is a version of $\mathbb { E } ( X | \mathcal { G } )$ : by definition of $L ^ { 1 } ( \varOmega , \mathcal { G } , P )$ the uniqueness claim is that all versions belong to the same equivalence class in $L ^ { 1 } ( \varOmega , \mathcal { G } , P )$ under the equivalence relation $f \equiv g$ if and only if $P ( \{ \omega \in \Omega : f ( \omega ) \neq g ( \omega ) \} )$ . In accordance with our convention (Section 5.1) we shall nonetheless continue to work with functions rather than with equivalence classes. 

To construct $Y$ we first restrict attention to the case when $X \in \mathcal { L } ^ { 2 } ( \mathcal { F } ) =$ $\mathcal { L } ^ { 2 } ( \varOmega , \mathcal { F } , P )$ . By Theorem 5.11, the inner product space $H = L ^ { 2 } ( { \mathcal { F } } )$ is complete, and the vector subspace $K = L ^ { 2 } ( \mathcal G )$ is a complete subspace. Thus the construction of the orthogonal projection in Section 5.2.3 applies, and provides an element of $L ^ { 2 } ( { \mathcal { G } } )$ , which by our convention we represent as a function $Y$ $\in \mathcal { L } ^ { 2 } ( \mathcal { G } )$ , such that $( X - Y )$ is orthogonal to $K$ . By definition of the inner product in $L ^ { 2 }$ this means that 

$$
(X - Y, Z) = \int_ {\Omega} (X - Y) Z \mathrm{d} P = 0
$$

for every $Z \in L ^ { 2 } ( \mathcal G )$ . In particular, since $\mathbf { 1 } _ { G } \in L ^ { 2 } ( \mathcal { G } )$ for every $G \in { \mathcal { G } }$ , we have $\textstyle \int _ { G } Y \mathrm { d } P = \int _ { G } X \mathrm { d } P .$ 

To construct Y for an arbitrary $X \in \mathcal { L } ^ { 1 } ( \mathcal { F } ) )$ we proceed in four stages: 

(i) first, note that if the result has been proved for non-negative functions in $\mathcal { L } ^ { 1 } ( \mathcal { F } ) )$ , we can consider $X = X ^ { + } - X ^ { - }$ . By hypothesis there are $Y ^ { + } , Y ^ { - } \in$ ${ \mathcal { L } } ^ { 1 } ( { \mathcal { G } } ) )$ such that for $G \in { \mathcal { G } }$ both $\textstyle \int _ { G } Y ^ { + } \mathrm { d } P = \int _ { G } X ^ { + } \mathrm { d } P $ and $\textstyle \int _ { G } Y ^ { - } \mathrm { d } P =$ $\int _ { G } X ^ { - } \mathrm { d } P .$ RSubtracting on both sides we obtain $\textstyle { \tilde { \int _ { G } } } Y \mathrm { d } P = \int _ { G } X { \bar { \mathrm { d } } } P$ , where $\bar { Y ^ { - } } = Y ^ { + } - Y ^ { - } \in \mathcal { L } ^ { 1 } ( \mathcal { G } )$ R R. So we need only verify the result for non-negative integrable X. 

(ii) second, if a random variable Z is bounded, it is in $\mathcal { L } ^ { 2 } ( \mathcal { F } )$ by Theorem 5.12, since $P ( \varOmega )$ is finite. Hence Z has a conditional expectation, i.e. there exists $W \in { \mathcal { L } } ^ { 2 } ( { \mathcal { G } } )$ such that $\textstyle \int _ { G } W \mathrm { d } P = \int _ { G } Z \mathrm { d } P $ for $G \in { \mathcal { G } }$ . Also: if $Z \geq 0$ , then $W \ge 0 \ P \mathrm { - a . s }$ R R. To see this, suppose that W takes negative values with positive probability. Then there exists $n \geq 1$ such that the set $G = \{ W < - \textstyle { \frac { 1 } { n } } \} \in { \mathcal { G } }$ has $P ( G ) > 0$ . Thus $\begin{array} { r } { \int _ { G } W \mathrm { d } P < - \frac { 1 } { n } P ( G ) < 0 } \end{array}$ . But $\textstyle \int _ { G } W \mathrm { d } P = \int _ { G } Z \mathrm { d } P \geq 0$ , since $Z \geq 0$ R R(Proposition 4.11). The contradiction shows that $W \geq 0 , P \mathrm { - a . s } .$ 

(iii) Now take an arbitrary $X ~ \geq ~ 0$ in $\mathcal { L } ^ { 1 } ( \mathcal { F } )$ , and for $n \geq 1$ set $X _ { n } \ =$ min $( X , n )$ . Then $X _ { n }$ is bounded and non-negative, so part (ii) applies to $X _ { n } .$ 8 yielding a non-negative $Y _ { n } \in { \mathcal { L } } ^ { 2 } ( { \mathcal { G } } )$ with $\begin{array} { r } { \int _ { G } Y _ { n } \mathrm { d } P = \int _ { G } X _ { n } \mathrm { d } P . } \end{array}$ Since $( X _ { n } )$ is increasing with n, for any fixed n the bounded random variable $Z = X _ { n + 1 } - X _ { n }$ is non-negative, and has a conditional expectation $W \geq 0 ,$ , as in (ii). But so have both $X _ { n + 1 }$ and $X _ { n }$ ,and the a.s. uniqueness property therefore implies that $W = Y _ { n + 1 } - Y _ { n } \ P _ { \mathrm { - a . s } }$ . Therefore $( Y _ { n } )$ also increases (a.s.) with n. 

(iv) Finally, set $Y ( \omega ) = \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } Y _ { n } ( \omega )$ for each $\omega \in \varOmega$ . By Theorem 3.5 Y is -measurable, and the sequence $( Y _ { n } )$ increases a.s. to Y. Moreover $0 \leq$ $X \in \mathcal { L } ^ { 1 } ( \mathcal { F } )$ and for $\begin{array} { r } { G \in \mathcal { G } , \int _ { G } Y _ { n } \mathrm { d } P = \int _ { G } X _ { n } \mathrm { d } P \le \int _ { G } X \mathrm { d } P < \infty } \end{array}$ for all $n .$ R R RThe Monotone Convergence Theorem shows that the integrals $\textstyle ( \int _ { G } Y _ { n } \mathrm { d } P ) _ { n \geq 1 }$ increase to $\textstyle \int _ { G } Y { \mathrm { d } } P , $ and that the final integral is finite, so that $Y \in { \mathcal { L } } ^ { 1 } ( { \mathcal { G } } )$ . On Rthe other hand, $\begin{array} { r } { \int _ { G } Y _ { n } \mathrm { d } P = \int _ { G } X _ { n } } \end{array}$ dP and the latter integrals also increase to $\textstyle \int _ { G } X \mathrm { d } P ,$ R Rso that we have shown: $\textstyle { \int _ { G } Y \mathrm { d } P = \int _ { G } }$ X dP for all $G \in { \mathcal { G } }$ 

## Remark 5.5

Note that since the orthogonal projection Y minimises the distance between the vector $X \in \mathcal { L } ^ { 2 } ( \mathcal { F } )$ and the subspace ${ \mathcal { L } } ^ { 2 } ( { \mathcal { G } } )$ , the $L ^ { 2 } \mathrm { . }$ norm, and hence its square $\begin{array} { r } { \int _ { \Omega } ( X - Z ) ^ { 2 } \mathrm { d } P , } \end{array}$ is minimised for elements in ${ \mathcal { L } } ^ { 2 } ( { \mathcal { G } } )$ if we take $Z = Y$ . Writing this in terms of expectations: E $( [ X - \mathbb { E } ( X | \mathcal { G } ) ] ^ { 2 } ) = \operatorname* { i n f } \{ \mathbb { E } ( [ X - Z ] ^ { 2 } ) : Z \in \mathcal { L } ^ { 2 } ( \mathcal { G } ) \}$ Thinking of σ-fields as containing ‘information’ about random events, we can interpret $\mathbb { E } ( X | \mathcal { G } )$ as the ‘best predictor’ of X amongst the class of -measurable square-integrable functions, since it minimises the least-mean-square distance to X. This idea has led to many useful applications in many areas of science. 

## 5.5 Proofs of propositions

## Proof (of Proposition 5.3)

Suppose that $\textstyle \int _ { D } f ^ { 2 } ( x )$ dx is finite. Then using $a \leq 1 + a ^ { 2 }$ (which follows from $( a - 1 ) ^ { 2 } \geq 0 )$ Rwe have 

$$
\int_ {D} f (x) \mathrm{d} x \leq \int_ {D} 1 \mathrm{d} x + \int_ {D} f ^ {2} (x) \mathrm{d} x = m (D) + \int_ {D} f ^ {2} (x) \mathrm{d} (x) <   \infty .
$$

## Proof (of Proposition 5.4)

We verify the first two properties using the linearity of the integral 

$$
\begin{array}{l} (f + g, h) = \int (f (x) + g (x)) h (x)   \mathrm{d} x \\ \qquad = \int f (x) h (x)   \mathrm{d} x + \int g (x) h (x)   \mathrm{d} x \\ \qquad = (f, h) + (g, h), \end{array}
$$

$$
(c f, h) = \int c f (x) h (x) \mathrm{d} x = c \int f (x) h (x) \mathrm{d} x = c (f, h).
$$

The symmetry is obvious since $f ( x ) g ( x ) = g ( x ) f ( x )$ under the integral. 

## Proof (of Proposition 5.5)

Parallelogram law: $\| h _ { 1 } + h _ { 2 } \| ^ { 2 } = ( h _ { 1 } + h _ { 2 } , h _ { 1 } + h _ { 2 } ) = ( h _ { 1 } , h _ { 1 } ) + ( h _ { 1 } , h _ { 2 } ) +$ $( h _ { 2 } , h _ { 1 } ) + ( h _ { 2 } , h _ { 2 } ) , \| h _ { 1 } - h _ { 2 } \| ^ { 2 } = ( h _ { 1 } - h _ { 2 } , h _ { 1 } - h _ { 2 } ) = ( h _ { 1 } , h _ { 1 } ) - ( h _ { 1 } , h _ { 2 } ) - $ $( h _ { 2 } , h _ { 1 } ) + ( h _ { 2 } , h _ { 2 } )$ , and adding we get the result. 

Polarization identity: subtract the above $\| h _ { 1 } + h _ { 2 } \| ^ { 2 } - \| h _ { 1 } - h _ { 2 } \| ^ { 2 } = 2 ( h _ { 1 } , h _ { 2 } ) +$ $2 ( h _ { 2 } , h _ { 1 } )$ , replace $h _ { 2 }$ by $\mathrm { i } h _ { 2 }$ to get $\| h _ { 1 } + \mathrm { i } h _ { 2 } \| ^ { 2 } - \| h _ { 1 } - \mathrm { i } h _ { 2 } \| ^ { 2 } = 2 ( h _ { 1 } , \mathrm { i } h _ { 2 } ) +$ $2 ( \mathrm { i } h _ { 2 } , h _ { 1 } )$ . Insert the obtained expressions into the right-hand side of the iden-tity in question. On the left we have $2 [ ( h _ { 1 } , h _ { 2 } ) + ( h _ { 2 } , h _ { 1 } ) + \mathrm { i } ( h _ { 1 } , \mathrm { i } h _ { 2 } ) + \mathrm { i } ( \mathrm { i } h _ { 2 } , h _ { 1 } ) ] =$ $2 [ ( h _ { 1 } , h _ { 2 } ) + ( h _ { 2 } , h _ { 1 } ) + \mathrm { i } ( - \mathrm { i } ) ( h _ { 1 } , h _ { 2 } ) + \mathrm { i } ^ { 2 } ( h _ { 2 } , h _ { 1 } ) ] = 4 ( h _ { 1 } , h _ { 2 } )$ 口

## Proof (of Proposition 5.13)

Suppose $\mathbb { E } ( X ^ { n } ) < \infty$ , which means that $X \in L ^ { n } ( \varOmega )$ , then since the measure of Ω is finite we may apply Theorem 5.12 and so $X \in L ^ { k } ( \varOmega )$ for all $k \leq n$ If $\mathbb { E } ( X ^ { n } ) = \infty$ the same must be true for $\mathbb { E } ( X ^ { k } )$ for $k \geq n$ since otherwise $\mathbb { E } ( X ^ { k } ) < \infty$ would imply $\mathbb { E } ( X ^ { n } ) < \infty - \mathbf { a }$ contradiction. □ 

## Proof (of Proposition 5.14)

Using the binomial expansion we have 

$$
(X - \mu) ^ {n} = \sum_ {i = 0} ^ {n} {\binom {n} {i}} X ^ {i} (- \mu) ^ {n - i},
$$

and so by linearity of the expectation 

$$
\mathbb {E} (X - \mu) ^ {n} = \sum_ {i = 0} ^ {n} {\binom {n} {i}} (- \mu) ^ {n - i} \mathbb {E} (X ^ {i}).
$$

## Proof (of Proposition 5.15)

We have 

$$
\mathbb {E} (X ^ {n}) = \mathbb {E} ((X - \mu + \mu) ^ {n}) = \sum_ {i = 1} ^ {n} {\binom {n} {i}} \mathbb {E} \bigl ((X - \mu) ^ {i} \bigr) \mu^ {n - i}.
$$

## Proof (of Proposition 5.19)

Let $f _ { n } ( x ) = \operatorname* { m a x } \{ - n , \operatorname* { m i n } \{ x , n \} \}$ . By Theorem 5.18, since $X , Y$ are independent, we have $\begin{array} { r } { \mathbb { E } ( f _ { n } ( X ) f _ { n } ( Y ) ) = \mathbb { E } ( f _ { n } ( X ) ) \mathbb { E } ( f _ { n } ( Y ) ) } \end{array}$ . Integrability of X and $Y$ enables us to pass to the limit, which is 0 on the right. □ 

## Proof (of Proposition 5.20)

Let X, Y be uncorrelated random variables. Then 

$$
\begin{array}{r l} & {\mathrm{Var} (X + Y) = \mathbb {E} \big (((X + Y) - \mathbb {E} (X + Y)) ^ {2} \big)} \\ & {\qquad = \mathbb {E} (X + Y) ^ {2} - (\mathbb {E} (X) + \mathbb {E} (Y)) ^ {2}} \\ & {\qquad = \mathbb {E} X ^ {2} + 2 \mathbb {E} (X Y) + \mathbb {E} Y ^ {2} - (\mathbb {E} X) ^ {2} - 2 \mathbb {E} (X) \mathbb {E} (Y) - (\mathbb {E} Y) ^ {2}} \\ & {\qquad = \mathbb {E} X ^ {2} - (\mathbb {E} X) ^ {2} + \mathbb {E} Y ^ {2} - (\mathbb {E} Y) ^ {2} + 2 [ \mathbb {E} (X Y) - \mathbb {E} (X) \mathbb {E} (Y) ]} \\ & {\qquad = \mathrm{Var} (X) + \mathrm{Var} (Y)} \end{array}
$$

since $\mathbb { E } ( X Y ) = \mathbb { E } ( X ) \mathbb { E } ( Y )$ . The general case for n random variables follows by 

induction or by repetitive use of the formula for two: 

$$
\begin{array}{r l} \operatorname{Var} (X _ {1} + \dots + X _ {n}) & = \operatorname{Var} (X _ {1} + [ X _ {2} + \dots + X _ {n} ]) \\ & = \operatorname{Var} (X _ {1}) + \operatorname{Var} (X _ {2} + [ X _ {3} + \dots + X _ {n} ]) \\ & \dots \\ & = \operatorname{Var} (X _ {1}) + \operatorname{Var} (X _ {2}) + \dots + \operatorname{Var} (X _ {n}). \end{array}
$$

Proof (of Proposition 5.21) 

By definition 

$$
\begin{array}{l} \varphi_ {X + Y} (t) = \mathbb {E} (\mathrm{e} ^ {\mathrm{i} t (X + Y)}) \\ \qquad = \mathbb {E} (\mathrm{e} ^ {\mathrm{i} t X} \mathrm{e} ^ {\mathrm{i} t Y}) \\ \qquad = \mathbb {E} (\mathrm{e} ^ {\mathrm{i} t X}) \mathbb {E} (\mathrm{e} ^ {\mathrm{i} t Y}) \quad \text {(by Theorem 5.18)} \\ \qquad = \varphi_ {X} (t) \varphi_ {Y} (t). \end{array}
$$

The generalization to n components is straightforward – induction or step-bystep application of the result for two. □ 

## 6.1 Multi-dimensional Lebesgue measure

In Chapter 2 we constructed Lebesgue measure on the real line. The basis for that was the notion of the length of an interval. Consider now the plane $\mathbb { R } ^ { 2 }$ in place of R. Here by interval we understand a rectangle of any sort: 

$$
R = I _ {1} \times I _ {2}
$$

where $I _ { 1 } , I _ { 2 }$ are any intervals. The ‘length’ of a rectangle is its area 

$$
a (R) = l (I _ {1}) \times l (I _ {2}).
$$

The concept of null set is introduced as in the one-dimensional case. As before, countable sets are null. It is worth noting that on the plane we have more sophisticated null sets such as, for example, a line segment or the graph of a function. 

The whole construction goes through without change and the resulting measure is the Lebesgue measure $m _ { 2 }$ on the plane defined on the σ-field generated by the rectangles. 

A subtle point which clearly illustrates the diference from linear measure is the following: any set of the form $A \times \{ a \} , a \in \mathbb { R }$ , is null and hence Lebesgue measurable on the plane. An interesting case of this is when A is a non-measurable set on the real line! 

Next, we consider $\mathbb { R } ^ { 3 }$ . By ‘interval’ here we mean a cube, and the ‘length is its volume: 

$$
C = I _ {1} \times I _ {2} \times I _ {3},
$$

$$
v (C) = l (I _ {1}) \times l (I _ {2}) \times l (I _ {3}).
$$

Now surfaces are examples of null sets. Following the same construction we obtain Lebesgue measure $m _ { 3 }$ in $\mathbb { R } ^ { 3 }$ 

Finally, we consider $\mathbb { R } ^ { n }$ (this includes the particular cases $n = 1 , 2 , 3$ so for a true mathematician this is the only case worth attention as it covers all the others). ‘Intervals’ are now n-dimensional cubes: 

$$
\mathbf {I} = I _ {1} \times \dots \times I _ {n}
$$

and generalized ‘length’ is given by 

$$
l (\mathbf {I}) = l (I _ {1}) \times \dots \times l (I _ {n}).
$$

An interesting example of a null set is a hyperplane. 

The above provides motivation for what follows. The multi-dimensional Lebesgue measures will emerge again from the considerations below where we will work with general measure spaces. Bearing in mind that we are principally interested in probabilistic applications, we stick to the notation of probability theory. 

## 6.2 Product σ-fields

Let $( \varOmega _ { 1 } , \mathcal { F } _ { 1 } , P _ { 1 } ) , ( \varOmega _ { 2 } , \mathcal { F } _ { 2 } , P _ { 2 } )$ be two measure spaces. Put 

$$
\varOmega = \varOmega_ {1} \times \varOmega_ {2}.
$$

We want to define a measure P on $\varOmega$ to ‘agree’ with the measures given on $\varOmega _ { 1 }$ , $\varOmega _ { 2 }$ 

Before we construct P we need to specify its domain, that is, a σ-field on $\varOmega .$ 

## Definition 6.1

Let $\mathcal { F }$ be the smallest σ-field of subsets of $\varOmega$ containing the ‘rectangles’ $A _ { 1 } \times A _ { 2 }$ for all $A _ { 1 } \in \mathcal { F } _ { 1 } , A _ { 2 } \in \mathcal { F } _ { 2 }$ . We call $\mathcal { F }$ the product σ-field of $\mathcal { F } _ { 1 }$ and $\mathcal { F } _ { 2 }$ . In other words, the product σ-field is generated by the family of sets (‘rectangles’) 

$$
\mathcal {R} = \left\{A _ {1} \times A _ {2}: A _ {1} \in \mathcal {F} _ {1}, A _ {2} \in \mathcal {F} _ {2} \right\}.
$$

The notation used for the product σ-field is simply: $\mathcal { F } = \mathcal { F } _ { 1 } \times \mathcal { F } _ { 2 }$ 

There are many ways in which the same product σ-field may be generated, each of which will prove useful in the sequel. 

## Theorem 6.1

(i) The product σ-field $\mathcal { F } _ { 1 } \times \mathcal { F } _ { 2 }$ is generated by the family of sets (‘cylinders or ‘strips’) 

$$
\mathcal {C} = \left\{A _ {1} \times \varOmega_ {2}: A _ {1} \in \mathcal {F} _ {1} \right\} \cup \left\{\varOmega_ {1} \times A _ {2}: A _ {2} \in \mathcal {F} _ {2} \right\}.
$$

(ii) The product σ-field is the smallest σ-field such that the projections 

$$
\operatorname * {P r} _ {1}: \varOmega \to \varOmega_ {1}, \quad \operatorname * {P r} _ {1} (\omega_ {1}, \omega_ {2}) = \omega_ {1}
$$

$$
\operatorname * {P r} _ {2}: \varOmega \to \varOmega_ {2}, \quad \operatorname * {P r} _ {2} (\omega_ {1}, \omega_ {2}) = \omega_ {2}
$$

are measurable. 

## Proof

Recall that we write $\sigma ( \mathcal { E } )$ for the σ-field generated by a family . 

Clearly is contained in hence the σ-field generated by is smaller than the σ-field generated by . On the other hand, 

$$
A _ {1} \times A _ {2} = (A _ {1} \times \varOmega_ {2}) \cap (\varOmega_ {1} \times A _ {2})
$$

hence the rectangles belong to the σ-field generated by cylinders: ${ \mathcal { R } } \subset \sigma ( { \mathcal { C } } )$ This implies $\sigma ( \mathcal { R } ) \subset \sigma ( \sigma ( \mathcal { C } ) ) = \sigma ( \mathcal { C } )$ which completes the proof of (i). 

For (ii) note that 

$$
\operatorname * {P r} _ {1} ^ {- 1} (A _ {1}) = A _ {1} \times \varOmega_ {2}, \quad \operatorname * {P r} _ {2} ^ {- 1} (A _ {2}) = \varOmega_ {1} \times A _ {2}
$$

hence the projections are measurable by (i). But the smallest σ-field such that they are both measurable is the smallest σ-field containing the cylinders, which is $\mathcal { F }$ by (i) again. □ 

Consider a particular case of $\varOmega _ { 1 } , \varOmega _ { 2 } = \mathbb { R } , \varPsi _ { 1 } = \mathscr { F } _ { 2 } = \mathscr { B }$ Borel sets. Then we have two ways of producing $\mathcal { F } = B _ { 2 } \mathcal { - }$ the Borel sets on the plane: we can use the family of products of Borel sets or the family of products of intervals. The following result shows that they give the same collection of subsets of $\mathbb { R } ^ { 2 }$ 

## Proposition 6.2

The σ-fields generated by 

$$
\mathcal {R} = \{B _ {1} \times B _ {2}: B _ {1}, B _ {2} \in \mathcal {B} \},
$$

$$
\mathcal {I} = \left\{I _ {1} \times I _ {2}: I _ {1}, I _ {2} \text {   are   intervals } \right\}
$$

are the same. 

Hint Use the idea of the proof of the preceding theorem. 

We may easily generalize to n factors: suppose we are given n measure spaces $( \varOmega _ { i } , \mathcal F _ { i } , P _ { i } ) , i = 1 , \ldots , n$ , then the product σ-fields in $\varOmega = \varOmega _ { 1 } \times \cdots \times \varOmega _ { n }$ is the σ-field generated by the sets 

$$
\left\{A _ {1} \times \dots \times A _ {n}: A _ {i} \in \mathcal {F} _ {i} \right\}.
$$

## 6.3 Construction of the product measure

Recall that $( \varOmega _ { 1 } , \mathscr { F } _ { 1 } , P _ { 1 } ) , ( \varOmega _ { 2 } , \mathscr { F } _ { 2 } , P _ { 2 } )$ are arbitrary measure spaces. We shall construct a measure $P$ on $\varOmega = \varOmega _ { 1 } \times \varOmega _ { 2 }$ which is determined by $P _ { 1 } , P _ { 2 }$ in a natural way. A technical assumption is needed here: $P _ { 1 }$ and $P _ { 2 }$ are taken to be σ-finite, that is, there is a sequence of measurable sets $A _ { n }$ with $\textstyle \bigcup _ { n = 1 } ^ { \infty } A _ { n } = \varOmega _ { 1 }$ 2 $P _ { 1 } ( A _ { n } )$ finite (and the same for $P _ { 2 } , \varOmega _ { 2 } )$ S. This is of course true for probability measures and also for Lebesgue measure (in the latter case $A _ { n } = [ - n , n ]$ will do for example). For simplicity we assume that $P _ { 1 } , P _ { 2 }$ are finite. (The extension to the case of σ-finite is obtained by a routine limit passage n in the results obtained for the restrictions of the measures to $A _ { n } . )$ 

The motivation provided by construction of multi-dimensional Lebesgue measures gives the following natural condition on $P$ : 

$$
P (A _ {1} \times A _ {2}) = P _ {1} (A _ {1}) P _ {2} (A _ {2})\tag{6.1}
$$

for $A _ { 1 } \in \mathcal { F } _ { 1 } , A _ { 2 } \in \mathcal { F } _ { 2 }$ 

We want to generalize (6.1) to all sets from the product σ-field. To do this we introduce the notion of a section of a subset A of $\varOmega _ { 1 } \times \varOmega _ { 2 }$ : for $\omega _ { 2 } \in \varOmega _ { 2 }$ 2 

$$
A _ {\omega_ {2}} = \left\{\omega_ {1} \in \Omega_ {1}: \left(\omega_ {1}, \omega_ {2}\right) \in A \right\} \subset \Omega_ {1}.
$$

A similar construction is carried out for $\omega _ { 1 } \in \varOmega _ { 1 }$ 

$$
A _ {\omega_ {1}} = \left\{\omega_ {2} \in \Omega_ {2}: \left(\omega_ {1}, \omega_ {2}\right) \in A \right\} \subset \Omega_ {2}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/0be368e5d8abb33fd730a6e3381b13d1fd34440cd1f0170d066c6fdb7dc5d1a2.jpg)



Figure 6.1 $\omega _ { 2 }$ section of a set


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/3b4c0d20eea9aebc4f0738cef789cf1272ef3feb02baf308992bc6791132442a.jpg)



Figure 6.2 $\omega _ { 1 }$ section of a set


Theorem 6.3 

If A is in the product σ-field $\mathcal { F }$ , then for each $\omega _ { 2 } , A _ { \omega _ { 2 } } \in \mathcal { F } _ { 1 }$ , and for each $\omega _ { 1 }$ , $A _ { \omega _ { 1 } } \in \mathcal { F } _ { 2 }$ 

Proof 

Let 

$$
\mathcal {G} = \{A \in \mathcal {F}: \text {   for   all   } \omega_ {2}, A _ {\omega_ {2}} \in \mathcal {F} _ {1} \}.
$$

If we show that $\mathcal { G }$ is a σ-field containing rectangles, then $\mathcal { G } = \mathcal { F }$ since $\mathcal { F }$ is the smallest σ-field with this property. 

If $A = A _ { 1 } \times A _ { 2 } , A _ { 1 } \in \mathcal { F } _ { 1 }$ , then 

$$
A _ {\omega_ {2}} = \left\{ \begin{array}{l l} A _ {1} & \text {if} \omega_ {2} \in A _ {2} \\ \emptyset & \text {if} \omega_ {2} \notin A _ {2} \end{array} \right.
$$

is in $\mathcal { F } _ { 1 }$ so the rectangles are in ${ \mathcal { G } } .$ 

If $A \in { \mathcal { G } }$ , then $\varOmega \setminus A \in \mathcal G$ since 

$$
\begin{array}{c} (\varOmega \setminus A) _ {\omega_ {2}} = \{\omega_ {1}: (\omega_ {1}, \omega_ {2}) \in (\varOmega \setminus A) \} \\ = \varOmega_ {1} \setminus \{\omega_ {1}: (\omega_ {1}, \omega_ {2}) \in A \} \\ = \varOmega_ {1} \setminus A _ {\omega_ {2}}. \end{array}
$$

Finally, let $A _ { n } \in \mathcal { G }$ . Since 

$$
\left(\bigcup_ {n = 1} ^ {\infty} A _ {n}\right) _ {\omega_ {2}} = \bigcup_ {n = 1} ^ {\infty} (A _ {n}) _ {\omega_ {2}},
$$

the union $\textstyle \bigcup _ { n = 1 } ^ { \infty } A _ { n }$ is also in $\mathcal { G }$ . 

SThe proof for $A _ { \omega _ { 1 } }$ is exactly the same. 

If $A = A _ { 1 } \times A _ { 2 }$ , then the function $\omega _ { 2 } \mapsto P ( A _ { \omega _ { 2 } } )$ is a step function: 

$$
P (A _ {\omega_ {2}}) = \left\{ \begin{array}{l l} P (A _ {1}) & \text { if } \omega_ {2} \in A _ {2} \\ 0 & \text { if } \omega_ {2} \notin A _ {2} \end{array} \right.
$$

and hence we have 

$$
P (A) = P _ {1} (A _ {1}) P _ {2} (A _ {2}) = \int_ {\Omega_ {2}} P (A _ {\omega_ {2}}) \mathrm{d} P _ {2} (\omega_ {2}).
$$

This motivates the general formula; for any A we write 

$$
P (A) = \int_ {\Omega_ {2}} P _ {1} (A _ {\omega_ {2}}) \mathrm{d} P _ {2} (\omega_ {2}).\tag{6.2}
$$

We call P the product measure and we will sometimes denote it by $P = P _ { 1 } \times P _ { 2 }$ We already know that $P _ { 1 } ( A _ { \omega _ { 2 } } )$ makes sense since $A _ { \omega _ { 2 } } \in \mathcal { F } _ { 1 }$ as shown before. For the integral to make sense we need more: 

## Theorem 6.4

Suppose that $P _ { 1 } , P _ { 2 }$ are finite. If $A \in { \mathcal { F } }$ , then the functions 

$$
\omega_ {2} \mapsto P _ {1} (A _ {\omega_ {2}}), \quad \omega_ {1} \mapsto P _ {2} (A _ {\omega_ {1}})
$$

are measurable with respect to $\mathcal { F } _ { 2 } , \mathcal { F } _ { 1 }$ , respectively, and 

$$
\int_ {\Omega_ {1}} P _ {1} (A _ {\omega_ {2}}) \mathrm{d} P _ {2} (\omega_ {2}) = \int_ {\Omega_ {2}} P _ {2} (A _ {\omega_ {1}}) \mathrm{d} P _ {1} (\omega_ {1}).\tag{6.3}
$$

Before we prove this theorem we allow ourselves a digression concerning the ways in which σ-fields can be produced. This will greatly simplify several proofs. Given a family of sets ${ \mathcal { A } } ,$ let $\mathcal { F }$ be the smallest σ-field containing . Suppose that $\mathcal { A }$ is a field, i.e. it is closed with respect to finite unions and diferences: $A , B \in { \mathcal { A } }$ implies $A \cup B , A \setminus B \in { \mathcal { A } }$ . Then we have an alternative way of characterizing σ-fields by means of so-called monotone classes. 

## Definition 6.2

A monotone class is a family of sets closed under countable unions of increasing sets and countable intersections of decreasing sets. That is, $\mathcal { G }$ is a monotone class if 

$$
A _ {1} \subset A _ {2} \subset \ldots , \quad A _ {i} \in \mathcal {G} \quad \Rightarrow \quad \bigcup_ {i = 1} ^ {\infty} A _ {i} \in \mathcal {G},
$$

$$
A _ {1} \supset A _ {2} \supset \dots , \quad A _ {i} \in \mathcal {G} \quad \Rightarrow \quad \bigcap_ {i = 1} ^ {\infty} A _ {i} \in \mathcal {G}.
$$

## Lemma 6.5 (Monotone Class Theorem)

The smallest monotone class $\mathcal { G } _ { A }$ containing a field coincides with the σ-field $\mathcal { F } _ { A }$ generated by . 

## Proof

A σ-field is a monotone class, so $\mathcal { G } _ { \mathcal { A } } \subset \mathcal { F } _ { \mathcal { A } }$ (since $\mathcal { G } _ { A }$ is the smallest monotone class containing ). 

To prove the converse, we first show that $\mathcal { G } _ { A }$ is a field. The family of sets 

$$
\{A: A ^ {\mathrm{c}} \in \mathcal {G} _ {\mathcal {A}} \}
$$

contains since $A \in { \mathcal { A } }$ implies $A ^ { \mathrm { c } } \in { \mathcal { A } } \subset { \mathcal { G } } _ { \mathcal { A } }$ . We observe that it is a monotone class. Suppose that $A _ { 1 } \subset A _ { 2 } \subset . . . ,$ are such that $A _ { i } ^ { \mathrm { c } } \in \mathcal { G } _ { A }$ . We have to show that $( \bigcup A _ { i } ) ^ { \mathrm { c } } \in \mathcal G _ { A }$ . We have $A _ { 1 } ^ { \mathrm { c } } \supset A _ { 2 } ^ { \mathrm { c } } \supset . .$ . and hence $\bigcap A _ { i } ^ { \mathrm { c } } \in { \mathcal { G } } _ { A }$ because $\mathcal { G } _ { A }$ Sis a monotone class. By de Morgan’s law $\cap A _ { i } ^ { \mathrm { c } } = ( \bigcup A _ { i } ) ^ { \mathrm { c } }$ so the union satisfies T Sthe required condition. The proof for the intersection is similar: $A _ { 1 } \supset A _ { 2 } \supset \ldots$ implies $A _ { 1 } ^ { \mathrm { c } } \subset A _ { 2 } ^ { \mathrm { c } } \subset . . . .$ , hence $\cup A _ { i } ^ { \mathrm { c } } \in \mathcal { G } _ { A }$ and so $( \bigcap A _ { i } ) ^ { \mathrm { { c } } } = \bigcup A _ { i } ^ { \mathrm { { c } } }$ also belongs to $\mathcal { G } _ { A }$ 

We conclude that 

$$
\mathcal {G} _ {\mathcal {A}} \subset \{A: A ^ {\mathrm{c}} \in \mathcal {G} _ {\mathcal {A}} \}
$$

so $\mathcal { G } _ { A }$ is closed with respect to taking complements. 

Now consider unions. First fix $A \in { \mathcal { A } }$ and consider 

$$
\{B: A \cup B \in \mathcal {G} _ {\mathcal {A}} \}.
$$

This family contains $\mathcal { A } \left( \mathrm { i f } \ B \in \mathcal { A } \right.$ , then $A \cup B \in { \mathcal { A } } \subset { \mathcal { G } } _ { A } )$ and is a monotone class. For, let $B _ { 1 } \subset B _ { 2 } \subset . .$ . be such that $A \cup B _ { i } \in { \mathcal { G } } _ { A }$ . Then $A \cup B _ { 1 } \subset A \cup B _ { 2 } \subset$ $\cdot \cdot \cdot$ hence $\bigcup ( A \cup B _ { i } ) \in \mathcal { G } _ { A }$ , thus $A \cup \bigcup B _ { i } \in { \mathcal { G } } _ { A }$ . Similar arguments work for S Sthe intersection of a decreasing chain of sets so for this fixed A 

$$
\mathcal {G} _ {\mathcal {A}} \subset \{B: A \cup B \in \mathcal {G} _ {\mathcal {A}} \}.
$$

This means that for $A \in { \mathcal { A } }$ and $B \in { \mathcal { G } } _ { A }$ we have $A \cup B \in { \mathcal { G } } _ { A }$ 

Now take arbitrary $A \in { \mathcal { G } } _ { A }$ . By what we have just observed, 

$$
\mathcal {A} \subset \{B: A \cup B \in \mathcal {G} _ {\mathcal {A}} \}
$$

and by the same argument as before, the latter family is a monotone class. So 

$$
\mathcal {G} _ {\mathcal {A}} \subset \{B: A \cup B \in \mathcal {G} _ {\mathcal {A}} \}
$$

this time for general A, which completes the proof that $\mathcal { G } _ { A }$ is a field. 

Now, having shown that $\mathcal { G } _ { A }$ is a field, we observe that it is a σ-field. This is obvious since for a sequence $A _ { i } \in { \mathcal { G } } _ { A }$ we have $A _ { 1 } \subset A _ { 1 } \cup A _ { 2 } \subset . . . ,$ they all are in $\mathcal { G } _ { A }$ (by the field property) and so is their union (since $\mathcal { G } _ { A }$ is a monotone class). 

Therefore $\mathcal { G } _ { A }$ is a σ-field containing so it is bigger than the σ-field generated by $\mathcal { A } \mathrm { : }$ 

$$
\mathcal {F} _ {\mathcal {A}} \subset \mathcal {G} _ {\mathcal {A}}
$$

which completes the proof. 

口

The family of rectangles introduced above is not a field so it cannot be used in the above result. Therefore we take $\mathcal { A }$ to be the family of all unions of disjoint rectangles. 

Proof (of Theorem 6.4) 

Write 

$$
\mathcal {G} = \left\{A: \omega_ {2} \mapsto P _ {1} (A _ {\omega_ {2}}), \quad \omega_ {1} \mapsto P _ {2} (A _ {\omega_ {1}}) \text {   are   measurable   and   } \right.
$$

$$
\left. \int_ {\Omega_ {2}} P _ {1} (A _ {\omega_ {2}}) \mathrm{d} P _ {2} (\omega_ {2}) = \int_ {\Omega_ {1}} P _ {2} (A _ {\omega_ {1}}) \mathrm{d} P _ {1} (\omega_ {1}) \right\}.
$$

The idea of the proof is this. First we show that $\mathcal { R } \subset \mathcal { G }$ , then ${ \mathcal { A } } \subset { \mathcal { G } }$ , and finally we show that $\mathcal { G }$ is a monotone class. By Lemma 6.5, $\mathcal { G } = \mathcal { F }$ which means that the claim of the theorem holds for all sets from $\mathcal { F }$ 

If A is a rectangle, $A = A _ { 1 } \times A _ { 2 }$ , then as we noticed before, $\omega _ { 2 } \mapsto P _ { 1 } ( A _ { \omega _ { 2 } } )$ $\omega _ { 1 } \mapsto P _ { 2 } ( A _ { \omega _ { 1 } } )$ are indicator functions multiplied by some constants and (6.3) holds each side being equal to $P _ { 1 } ( A _ { 1 } ) P _ { 2 } ( A _ { 2 } )$ 

Next let $A = ( A _ { 1 } \times A _ { 2 } ) \cup ( B _ { 1 } \times B _ { 2 } )$ be the union of disjoint rectangles. Disjoint means that either $A _ { 1 } \cap B _ { 1 } = \emptyset$ or $A _ { 2 } \cap B _ { 2 } = \ O \ O$ . Assume the former, for example. Then 

$$
A _ {\omega_ {2}} = \left\{ \begin{array}{l l} A _ {1} \cup B _ {1} & \text { if } \omega_ {2} \in A _ {2} \cap B _ {2} \\ A _ {1} & \text { if } \omega_ {2} \in A _ {2} \setminus B _ {2} \\ B _ {1} & \text { if } \omega_ {2} \in B _ {2} \setminus A _ {2} \\ \emptyset & \text { otherwise } \end{array} \right.
$$

and 

$$
\begin{array}{l} \int_ {\Omega_ {2}} P _ {1} (A _ {\omega_ {2}})   \mathrm{d} P _ {2} (\omega_ {2}) = [ P _ {1} (A _ {1}) + P _ {1} (B _ {1}) ] P _ {2} (A _ {2} \cap B _ {2}) \\ \qquad \qquad + P _ {1} (A _ {1}) P _ {2} (A _ {2} \setminus B _ {2}) + P _ {1} (B _ {1}) P _ {2} (B _ {2} \setminus A _ {2}) \\ \qquad = P _ {1} (A _ {1}) [ P _ {2} (A _ {2} \cap B _ {2}) + P _ {2} (A _ {2} \setminus B _ {2}) ] \\ \qquad \qquad + P _ {1} (B _ {1}) [ P _ {2} (A _ {2} \cap B _ {2}) + P _ {2} (B _ {2} \setminus A _ {2}) ] \\ \qquad = P _ {1} (A _ {1}) P _ {2} (A _ {2}) + P _ {1} (B _ {1}) P _ {2} (B _ {2}). \end{array}
$$

On the other hand 

$$
A _ {\omega_ {1}} = \left\{ \begin{array}{l l} A _ {2} & \text { if } \omega_ {1} \in A _ {1} \\ B _ {2} & \text { if } \omega_ {1} \in B _ {1} \\ \emptyset & \text { otherwise } \end{array} \right.
$$

and 

$$
\int_ {\Omega_ {1}} P _ {2} (A _ {\omega_ {1}}) \mathrm{d} P _ {1} (\omega_ {1}) = P _ {1} (A _ {1}) P _ {2} (A _ {2}) + P _ {1} (B _ {1}) P _ {2} (B _ {2})
$$

as before. 

The general case of finitely many rectangles can be proved in the same way. This is easy but tedious and we skip this argument hoping that presenting it in detail for two rectangles is suficient to guide the reader in the general case. It remains true that the functions $\omega _ { 2 } \mapsto P _ { 1 } ( A _ { \omega _ { 2 } } ) , \omega _ { 1 } \mapsto P _ { 2 } ( A _ { \omega _ { 1 } } )$ are simple functions, and so the verification of (6.3) is just simple algebra. 

It remains to verify that is a monotone class. Let $A _ { 1 } \subset A _ { 2 } \subset . . .$ . be sets from ${ \mathcal { G } } ;$ ; hence the functions $\omega _ { 2 } \mapsto P _ { 1 } ( ( A _ { i } ) _ { \omega _ { 2 } } ) , \omega _ { 1 } \mapsto P _ { 2 } ( ( A _ { i } ) _ { \omega _ { 1 } } )$ are measurable. They increase with i since the sections $( A _ { i } ) _ { \omega _ { 2 } } , ( A _ { i } ) _ { \omega _ { 1 } }$ are increasing. If $i \to \infty$ 2 then 

$$
P _ {1} ((A _ {i}) _ {\omega_ {2}}) \to P _ {1} (\bigcup_ {i} (A _ {i}) _ {\omega_ {2}}) = P _ {1} ((\bigcup_ {i} A _ {i}) _ {\omega_ {2}})
$$

and so the function $\omega _ { 2 } \mapsto P _ { 1 } ( ( \cup _ { i } A _ { i } ) _ { \omega _ { 2 } } )$ is measurable. The same argument shows that the function $\begin{array} { r } { \omega _ { 1 } \mapsto P _ { 2 } ( ( \bigcup _ { i } A _ { i } ) _ { \omega _ { 1 } } ) } \end{array}$ is measurable. The equality (6.3) 

holds for each i and by the monotone convergence theorem it is preserved in the limit. Thus (6.3) holds for unions $\bigcup A _ { i }$ 

SFor intersections the argument is similar. The sequences in question are decreasing; the functions $\omega _ { 2 } \mapsto P _ { 1 } ( ( \bigcap _ { i } A _ { i } ) _ { \omega _ { 2 } } ) , \omega _ { 1 } \mapsto P _ { 2 } ( ( \bigcap _ { i } A _ { i } ) _ { \omega _ { 1 } } )$ are measur-T Table as their limits and (6.3) holds by the monotone convergence theorem. 

## Theorem 6.6

Suppose that $P _ { 1 } , P _ { 2 }$ are finite measures. The set function P given by (6.2) is countably additive. Any other measure coinciding with P on rectangles is equal to P on the product σ-field. 

## Proof

Let $A _ { i } \in { \mathcal { F } }$ be pairwise disjoint. Then $( A _ { i } ) _ { \omega _ { 2 } }$ are also pairwise disjoint and 

$$
\begin{array}{l} P (\bigcup A _ {i}) = \int_ {\Omega_ {2}} P _ {1} ((\bigcup_ {i} A _ {i}) _ {\omega_ {2}})   \mathrm{d} P _ {2} (\omega_ {2}) \\ \qquad = \int_ {\Omega_ {2}} P _ {1} (\bigcup_ {i} (A _ {i}) _ {\omega_ {2}})   \mathrm{d} P _ {2} (\omega_ {2}) \\ \qquad = \int_ {\Omega_ {2}} \sum_ {i} P _ {1} ((A _ {i}) _ {\omega_ {2}})   \mathrm{d} P _ {2} (\omega_ {2}) \\ \qquad = \sum_ {i} \int_ {\Omega_ {2}} P _ {1} ((A _ {i}) _ {\omega_ {2}})   \mathrm{d} P _ {2} (\omega_ {2}) \\ \qquad = \sum_ {i} P (A _ {i}) \end{array}
$$

where we have employed the fact that the section of the union is the union of the sections (see Figure 6.3) and the Beppo–Levi theorem. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/40fe1d1d709a838250b73f848edec06f25cc8a2c14361bd296af63cf58dae8f6.jpg)



Figure 6.3 Section of a union


For uniqueness let $Q$ be a measure defined on the product σ-field $\mathcal { F }$ such that $P ( A _ { 1 } \times A _ { 2 } ) = Q ( A _ { 1 } \times A _ { 2 } ) , A _ { 1 } \in \mathcal { F } _ { 1 } , A _ { 2 } \in \mathcal { F } _ { 2 }$ . Let 

$$
\mathcal {H} = \{A \subset \Omega_ {1} \times \Omega_ {2}: A \in \mathcal {F}, P (A) = Q (A) \}.
$$

This family contains all rectangles by the hypothesis. It contains unions of disjoint rectangles by the additivity of both $P$ and $Q ;$ in other words contains the field ${ \mathcal { A } } .$ 

It remains to show that it is a monotone class since then it coincides with $\mathcal { F }$ by Lemma 6.5. This is quite straightforward using again the fact that $P$ and $Q$ are measures. If $A _ { 1 } \subset A _ { 2 } \subset . . . , A _ { i } \in { \mathcal { H } } .$ , then $P ( A _ { i } ) = Q ( A _ { i } ) , P ( \bigcup A _ { i } ) =$ lim $P ( A _ { i } ) , Q ( \bigcup A _ { i } ) = \operatorname* { l i m } Q ( A _ { i } )$ , hence $P ( \bigcup A _ { i } ) = Q ( \bigcup A _ { i } )$ Swhich means that $\mathcal { H }$ S S Sis closed with respect to monotone unions. The argument for monotone intersections is exactly the same: if $A _ { 1 } \supset A _ { 2 } \supset . . . ,$ then $P ( \bigcap A _ { i } ) = \operatorname* { l i m } P ( A _ { i } )$ , $Q ( \bigcap A _ { i } ) = \operatorname* { l i m } Q ( A _ { i } )$ , hence $P ( A _ { i } ) = Q ( A _ { i } )$ implies $P ( \bigcap A _ { i } ) = Q ( \bigcap A _ { i } )$ □ 

## Remark 6.1

The uniqueness part of the proof of Theorem 6.6 illustrates an important technique: in order to show that two measures on a σ-field coincide it sufices to prove that they coincide on the generating sets of that σ-field, by an application of the monotone class theorem. 

As an immediate consequence of Theorem 6.4 we have 

$$
P (A) = \int_ {\Omega_ {1}} P _ {2} (A _ {\omega_ {1}}) \mathrm{d} P _ {1} (\omega_ {1}).
$$

The completion of the product σ-field $\mathcal { M } \times \mathcal { M }$ built from the σ-field of Lebesgue measurable sets is the σ-field $\mathcal { M } _ { 2 }$ on which $m _ { 2 }$ is defined. 

It easy to see that two-dimensional Lebesgue measure coincides with the completion of the product of one-dimensional ones: $m _ { 2 } = c ( m \times m )$ . First, they agree on rectangles built from intervals. As a consequence, they agree on the σ-field generated by such rectangles, which is the Borel σ-field on the plane. The completion of Borel sets gives the σ-field of Lebesgue measurable sets in the same way as in the one-dimensional case. 

## 6.4 Fubini’s Theorem

We wish to integrate functions defined on the product of the spaces $\left( \varOmega _ { 1 } , \mathcal { F } _ { 1 } , P _ { 1 } \right)$ $\left( \varOmega _ { 2 } , \mathcal { F } _ { 2 } , P _ { 2 } \right)$ by exploiting the integration with respect to the measures $P _ { 1 } , P _ { 2 }$ individually. 

We tackle the issue of measurability first. 

## Theorem 6.7

If a non-negative function $f : \varOmega _ { 1 } \times \varOmega _ { 2 } \to \mathbb R$ is measurable with respect to $\mathcal { F } _ { 1 } \times \mathcal { F } _ { 2 }$ , then for each $\omega _ { 1 } \in \Omega _ { 1 }$ the function (which we shall call a section of $f ) \ \omega _ { 2 } \ \mapsto \ f ( \omega _ { 1 } , \omega _ { 2 } )$ is $\mathcal { F } _ { \mathrm { 2 - m e a s u r a b l e } }$ , and for each $\omega _ { 2 } ~ \in ~ \varOmega _ { 2 }$ the section $\omega _ { 1 } \mapsto f ( \omega _ { 1 } , \omega _ { 2 } )$ is <sub>1</sub>-measurable. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3a6696ab-930f-42ac-b6c5-7436ce0b537b/e53a165d9cdd93e397623f683b4b38c26517da853090227c9ef354e828769c66.jpg)



Figure 6.4 Section of f


## Proof

First we approximate f by simple functions in similar fashion to Proposition 4.10; we write 

$$
f _ {n} (\omega_ {1}, \omega_ {2}) = \left\{ \begin{array}{l l} \frac {k}{n} & \text {if} f (\omega_ {1}, \omega_ {2}) \in [ \frac {k}{n}, \frac {k + 1}{n}), k <   n ^ {2} \\ n & \text {if} f (\omega_ {1}, \omega_ {2}) > n \end{array} \right.
$$

and as $n  \infty , f _ { n }  f .$ 

The sections of simple measurable functions are simple and measurable. This is clear for the indicator functions as observed above, and next we use the fact that the section of the sum is the sum of the sections. 

Finally, it is clear that the sections of $f _ { n }$ converge to the sections of f andsince measurability is preserved in the limit, the theorem is proved. 口

## Corollary 6.8

The functions 

$$
\omega_ {1} \mapsto \int_ {\Omega_ {2}} f (\omega_ {1}, \omega_ {2}) \mathrm{d} P _ {2} (\omega_ {2}), \quad \omega_ {2} \mapsto \int_ {\Omega_ {1}} f (\omega_ {1}, \omega_ {2}) \mathrm{d} P _ {1} (\omega_ {1})
$$

are <sub>1</sub>, <sub>2</sub>-measurable, respectively. 

## Proof

The integrals may be taken (being possibly infinite) due to measurability of the functions in question. By the monotone convergence theorem, they are limits of the integrals of the sections of $f _ { n }$ . The integrals $\begin{array} { r l } { \int _ { \Omega _ { 1 } } f _ { n } ( \omega _ { 1 } , \omega _ { 2 } ) \mathrm { d } P _ { 1 } ( \omega _ { 1 } ) } \end{array}$ 2 $\begin{array} { r l } { \int _ { \Omega _ { 2 } } f _ { n } ( \omega _ { 1 } , \omega _ { 2 } ) \mathrm { d } P _ { 2 } ( \omega _ { 2 } ) } & { { } } \end{array}$ Rare simple functions, and hence the limits are measur-Rable. □ 

## Theorem 6.9

Let f be a measurable non-negative function defined on $\varOmega _ { 1 } \times \varOmega _ { 2 }$ . Then 

$$
\begin{array}{l} \int_ {\Omega_ {1} \times \Omega_ {2}} f (\omega_ {1}, \omega_ {2}) \mathrm{d} (P _ {1} \times P _ {2}) (\omega_ {1}, \omega_ {2}) = \int_ {\Omega_ {1}} \left(\int_ {\Omega_ {2}} f (\omega_ {1}, \omega_ {2}) \mathrm{d} P _ {2} (\omega_ {2})\right) \mathrm{d} P _ {1} (\omega_ {1}) \\ = \int_ {\Omega_ {2}} \left(\int_ {\Omega_ {1}} f (\omega_ {1}, \omega_ {2}) \mathrm{d} P _ {1} (\omega_ {1})\right) \mathrm{d} P _ {2} (\omega_ {2}). \end{array} \tag {6.4}
$$

## Proof

For the indicator function of a rectangle $A _ { 1 } \times A _ { 2 }$ each side of (6.4) just becomes $P _ { 1 } ( A _ { 1 } ) P _ { 2 } ( A _ { 2 } )$ . Then by additivity of the integral the formula is true for simple functions. Monotone approximation of any measurable f by simple functions allows us to extend this formula to the general case. □ 

## Theorem 6.10 (Fubini’s Theorem)

If $f \in L ^ { 1 } ( \varOmega _ { 1 } \times \varOmega _ { 2 } )$ then the sections are integrable in appropriate spaces, the functions 

$$
\omega_ {1} \mapsto \int_ {\Omega_ {2}} f (\omega_ {1}, \omega_ {2}) \mathrm{d} P _ {2} (\omega_ {2}), \quad \omega_ {2} \mapsto \int_ {\Omega_ {1}} f (\omega_ {1}, \omega_ {2}) \mathrm{d} P _ {1} (\omega_ {1})
$$

are in $L ^ { 1 } ( \varOmega _ { 1 } ) , L ^ { 1 } ( \varOmega _ { 2 } )$ , respectively, and (6.4) holds: in concise form it reads 

$$
\int_ {\Omega_ {1} \times \Omega_ {2}} f \mathrm{d} (P _ {1} \times P _ {2}) = \int_ {\Omega_ {1}} \left(\int_ {\Omega_ {2}} f \mathrm{d} P _ {2}\right) \mathrm{d} P _ {1} = \int_ {\Omega_ {2}} \left(\int_ {\Omega_ {1}} f \mathrm{d} P _ {1}\right) \mathrm{d} P _ {2}.
$$

## Proof

This relation is immediate by the decomposition $f = f ^ { + } - f ^ { - }$ and the result proved for non-negative functions. The integrals are finite since if $f \in L ^ { 1 }$ then $f ^ { + } , f ^ { - } \in L ^ { 1 }$ and all the integrals on the right are finite. □ 

## Remark 6.2

The whole procedure may be extended to the product of an arbitrary finite number of spaces. In particular, we have a method of constructing ndimensional Lebesgue measure as the completion of the product of n copies of one-dimensional Lebesgue measure. 

## Example 6.1

Let $\varOmega _ { 1 } = \varOmega _ { 2 } = [ 0 , 1 ] , P _ { 1 } = P _ { 2 } = m _ { [ 0 , 1 ] } ,$ 7 

$$
f (x, y) = \left\{ \begin{array}{l l} \frac {1}{x ^ {2}} & \text { if } 0 <   y <   x <   1 \\ 0 & \text { otherwise. } \end{array} \right.
$$

We shall see that the integral of f over the square is infinite. For this we take a non-negative simple function dominated by f and compute its integral. Let $\varphi ( x , y ) = n { \mathrm { ~ i f ~ } } f ( x , y ) \in [ n , n + 1 )$ . Then $\begin{array} { r } { \varphi ( x , y ) = n { \mathrm { ~ i f ~ } } x > y , x \in ( { \frac { 1 } { \sqrt { n + 1 } } } , { \frac { 1 } { \sqrt { n } } } ] } \end{array}$ The area of this set is $\textstyle { \frac { 1 } { 2 } } { \bigl ( } { \frac { 1 } { n } } - { \frac { 1 } { n + 1 } } { \bigr ) }$ and 

$$
\int_ {[ 0, 1 ] ^ {2}} \varphi \mathrm{d} m _ {2} = \sum_ {n = 1} ^ {\infty} n \frac {1}{2} (\frac {1}{n} - \frac {1}{n + 1}) = \sum_ {n = 1} ^ {\infty} \frac {1}{2} \frac {1}{n + 1} = \infty .
$$

Hence the function 

$$
g (x, y) = \left\{ \begin{array}{l l} \frac {1}{x ^ {2}} & \text { if } 0 <   y <   x <   1 \\ - \frac {1}{y ^ {2}} & \text { if } 0 <   x <   y <   1 \\ 0 & \text { otherwise } \end{array} \right.
$$

is not integrable since the integral of $g ^ { + }$ is infinite (the same is true for the integral of $g ^ { - } )$ 

## Exercise 6.1

For g from the above example show that 

$$
\int_ {0} ^ {1} \int_ {0} ^ {1} g (x, y) \mathrm{d} x \mathrm{d} y = - 1, \quad \int_ {0} ^ {1} \int_ {0} ^ {1} g (x, y) \mathrm{d} y \mathrm{d} x = 1
$$

which shows that the iterated integrals may not be equal if Fubini’s theorem condition is violated. 

The following proposition opens the way for many applications of product measures and Fubini’s theorem. 

## Proposition 6.11

Let $f : \mathbb { R } \to \mathbb { R }$ be measurable and positive. Consider the set of all points in the upper half-plane being below the graph of $f \colon$ 

$$
A _ {f} = \{(x, y): 0 \leq y <   f (x) \}.
$$

Show that $A _ { f }$ is m -measurable and $\begin{array} { r } { m _ { 2 } ( A _ { f } ) = \int f ( x ) \mathrm { d } x } \end{array}$ 

Hint For measurability ‘fill’ $A _ { f }$ with rectangles using the approximation of $f$ by simple functions. Then apply the definition of the product measure. 

Exercise 6.2 

Compute $\begin{array} { r l } { \int _ { [ 0 , 3 ] \times [ - 1 , 2 ] } x ^ { 2 } y \mathrm { d } m _ { 2 } } \end{array}$ 

Exercise 6.3 

Compute the area of the region inside the ellipse $\begin{array} { r } { \frac { x ^ { 2 } } { a ^ { 2 } } + \frac { y ^ { 2 } } { b ^ { 2 } } = 1 } \end{array}$ 

## 6.5 Probability

## 6.5.1 Joint distributions

Let $X , ~ Y$ be two random variables defined on the same probability space $( \varOmega , \mathcal { F } , P )$ . Consider the random vector 

$$
(X, Y): \Omega \to \mathbb {R} ^ {2}.
$$

Its distribution is the measure defined for the Borel sets on the plane given by 

$$
P _ {(X, Y)} (B) = P ((X, Y) \in B), \quad B \subset \mathbb {R} ^ {2}.
$$

If this measure can be written as 

$$
P _ {(X, Y)} (B) = \int_ {B} f _ {(X, Y)} (x, y) \mathrm{d} m _ {2} (x, y)
$$

for some integrable $f _ { ( X , Y ) }$ , then we say that X, Y have a joint density. 

The joint distribution determines the distributions of one-dimensional random variables X, Y : 

$$
P _ {X} (A) = P _ {(X, Y)} (A \times \mathbb {R}),
$$

$$
P _ {Y} (A) = P _ {(X, Y)} (\mathbb {R} \times A),
$$

for Borel $A \subset \mathbb { R }$ , these are called marginal distributions. If X, Y have a joint density, then both X and Y are absolutely continuous with densities given by 

$$
f _ {X} (x) = \int_ {\mathbb {R}} f _ {(X, Y)} (x, y) \mathrm{d} y,
$$

$$
f _ {Y} (y) = \int_ {\mathbb {R}} f _ {(X, Y)} (x, y) \mathrm{d} x.
$$

The following example shows that the converse is not true in general. 

## Example 6.2

Let $\varOmega = [ 0 , 1 ]$ with $P = m _ { [ 0 , 1 ] }$ and let $( X , Y ) ( \omega ) = ( \omega , \omega )$ . This vector does not have density since $P _ { ( X , Y ) } ( \{ ( x , y ) : x = y \} ) = 1$ and for any integrable function $\begin{array} { r } { f : \mathbb { R } ^ { 2 }  \mathbb { R } , \int _ { \{ ( x , y ) : x = y \} } f ( x , y ) \mathrm { d } m _ { 2 } ( x , y ) = 0 ; } \end{array}$ a contradiction. However the Rmarginal distributions $\mathit { \bar { P } } _ { X } , \mathit { \Pi } _ { Y _ { Y } }$ are absolutely continuous with the densities $f _ { X } = f _ { Y } = \mathbf { 1 } _ { [ 0 , 1 ] }$ 

## Example 6.3

A simple example of joint density is the uniform one: $\begin{array} { r } { f = \frac { 1 } { m ( A ) } \mathbf { 1 } _ { A } } \end{array}$ , with Borel $A \ \subset \ \mathbb { R } ^ { 2 }$ . A particular case is $A = [ 0 , 1 ] \times [ 0 , 1 ]$ , then clearly the marginal densities are $\mathbf { 1 } _ { [ 0 , 1 ] }$ 

## Exercise 6.4

Take A to be the square with corners at (0, 1), (1, 0), (2, 1), (1, 2). Find the marginal densities of $f = \mathbf { 1 } _ { A }$ 

## Exercise 6.5

Let $f _ { X , Y } ( x , y ) = { \textstyle { \frac { 1 } { 5 0 } } } ( x ^ { 2 } + y ^ { 2 } ) { \mathrm { ~ i f ~ } } 0 < x < 2 , 1 < y < 4$ and zero otherwise. Find $P ( X + Y > 4 ) , P ( Y > X )$ 

The two-dimensional Gaussian (normal) density is given by 

$$
n (x, y) = \frac {1}{2 \pi \sqrt {1 - \rho^ {2}}} \exp \left\{- \frac {1}{2 (1 - \rho^ {2})} (x ^ {2} - 2 \rho x y + y ^ {2}) \right\}.\tag{6.5}
$$

It can be shown that $\rho$ is the correlation of $X , Y .$ , random variables whose densities are the marginal densities of $n ( x , y )$ , (see [9]). 

Joint densities enable us to compute the distributions of various functions of random variables. Here is an important example. 

## Theorem 6.12

If X, Y have joint density $f _ { X , Y }$ , then the density of their sum is given by 

$$
f _ {X + Y} (z) = \int_ {\mathbb {R}} f _ {X, Y} (x, z - x) \mathrm{d} x.\tag{6.6}
$$

Proof 

We employ the distribution function: 

$$
\begin{array}{l} F _ {X + Y} (z) = P (X + Y \leq z) \\ \qquad = P _ {X, Y} (\{(x, y): x + y \leq z \}) \\ \qquad = \int \int_ {\{(x, y): x + y \leq z \}} f _ {X, Y} (x, y)   \mathrm{d} x \mathrm{d} y \\ \qquad = \int_ {\mathbb {R}} \int_ {- \infty} ^ {z - x} f _ {X, Y} (x, y)   \mathrm{d} y \mathrm{d} x \\ \qquad = \int_ {- \infty} ^ {z} \int_ {\mathbb {R}} f _ {X, Y} (x, y ^ {\prime} - x)   \mathrm{d} x \mathrm{d} y ^ {\prime} \end{array}
$$

(we have used the substitution $y ^ { \prime } = y + x$ and Fubini’s theorem), which by diferentiation gives the result. 

Exercise 6.6 

Find $f _ { X + Y } { \mathrm { ~ i f ~ } } f _ { X , Y } = \mathbf { 1 } _ { [ 0 , 1 ] \times [ 0 , 1 ] } .$ 

## 6.5.2 Independence again

Suppose that the random variables X, Y are independent. Then for a Borel rectangle: $B = B _ { 1 } \times B _ { 2 }$ we have 

$$
\begin{array}{r l} P _ {(X, Y)} (B _ {1} \times B _ {2}) & = P ((X, Y) \in B _ {1} \times B _ {2}) \\ & = P ((X \in B _ {1}) \cap (Y \in B _ {2})) \\ & = P (X \in B _ {1}) P (Y \in B _ {2}) \\ & = P _ {X} (B _ {1}) P _ {Y} (B _ {2}) \end{array}
$$

and so the distribution $P _ { ( X , Y ) }$ coincides with the product measure $P _ { X } \times P _ { Y }$ on rectangles, therefore they are the same. The converse is also true: 

## Theorem 6.13

The random variables $X , Y$ are independent if and only if 

$$
P _ {(X, Y)} = P _ {X} \times P _ {Y}.
$$

## Proof

The ‘only $\mathrm { i f } ^ { \prime }$ part was shown above. Suppose that $P _ { ( X , Y ) } = P _ { X } \times P _ { Y }$ and takeany Borel sets $B _ { 1 } , B _ { 2 }$ . The same computation shows that $P ( ( X \in B _ { 1 } ) \cap ( Y \in$ $B _ { 2 } ) ) = P ( X \in B _ { 1 } ) P ( Y \in B _ { 2 } )$ , i.e. X and Y are independent. 口

We have a useful version of this theorem in the case of absolutely continuous random variables. 

## Theorem 6.14

If X, Y have a joint density, then they are independent if and only if 

$$
f _ {(X, Y)} (x, y) = f _ {X} (x) f _ {Y} (y).\tag{6.7}
$$

If X and Y are absolutely continuous and independent, then they have a joint density and it is given by (6.7). 

## Proof

Suppose $f _ { ( X , Y ) }$ is the joint density of X, Y . If they are independent, then 

$$
\begin{array}{r l} \int_ {B _ {1} \times B _ {2}} f _ {(X, Y)} (x, y) \mathrm{d} m _ {2} (x, y) & = P ((X, Y) \in B _ {1} \times B _ {2}) \\ & = P (X \in B _ {1}) P (Y \in B _ {2}) \\ & = \int_ {B _ {1}} f _ {X} (x) \mathrm{d} m (x) \int_ {B _ {2}} f _ {Y} (y) \mathrm{d} m (y) \\ & = \int_ {B _ {1} \times B _ {2}} f _ {X} (x) f _ {Y} (y) \mathrm{d} m _ {2} (x, y) \end{array}
$$

which implies (6.7). The same computation shows the converse: 

$$
\begin{array}{l} P ((X, Y) \in B _ {1} \times B _ {2}) = \int_ {B _ {1} \times B _ {2}} f _ {(X, Y)} (x, y)   \mathrm{d} m _ {2} (x, y) \\ \qquad = \int_ {B _ {1} \times B _ {2}} f _ {X} (x) f _ {Y} (y)   \mathrm{d} m _ {2} (x, y) \\ \qquad = P (X \in B _ {1}) P (Y \in B _ {2}). \end{array}
$$

For the final claim note that the function $f _ { X } ( x ) f _ { Y } ( y )$ plays the role of the joint density if X and $Y$ are independent. □ 

## Corollary 6.15

If Gaussian random variables are orthogonal, then they are independent. 

## Proof

Inserting $\rho = 0$ into (6.5) we immediately see that the two-dimensional Gaussian density is the product of the one-dimensional ones. □ 

## Proposition 6.16

The density of the sum of independent random variables with densities $f _ { X } , f _ { Y }$ is given by 

$$
f _ {X + Y} (z) = \int_ {\mathbb {R}} f _ {X} (x) f _ {Y} (z - x) \mathrm{d} x.
$$

## Exercise 6.7

Suppose that the joint density of $X , Y$ is $\mathbf { 1 } _ { A }$ where A is the square with corners at $( 0 , 1 ) , ( 1 , 0 ) , ( 2 , 1 ) , ( 1 , 2 )$ . Are X, Y independent? 

## Exercise 6.8

Find $P ( Y > X )$ and $P ( X + Y > 1 )$ , if X, Y are independent with $\begin{array} { r } { f _ { X } = \mathbf { 1 } _ { [ 0 , 1 ] } , f _ { Y } = \frac { 1 } { 2 } \mathbf { 1 } _ { [ 0 , 2 ] } } \end{array}$ 

## 6.5.3 Conditional probability

We consider the case of two random variables X, Y with joint density $f _ { X , Y } ( x , y )$ Given Borel sets $A , B ,$ , we compute 

$$
\begin{array}{l} P (Y \in B | X \in A) = \frac {P (X \in A , Y \in B)}{P (X \in A)} \\ \qquad = \frac {\int_ {A \times B} f _ {(X , Y)} (x , y) \mathrm{d} m _ {2} (x , y)}{\int_ {A} f _ {X} (x) \mathrm{d} m (x)} \\ \qquad = \int_ {B} \frac {\int_ {A} f _ {(X , Y)} (x , y) \mathrm{d} x}{\int_ {A} f _ {X} (x) \mathrm{d} x} \mathrm{d} y \end{array}
$$

using Fubini’s theorem. So the conditional distribution of Y given $X \in A$ has a density 

$$
h (y | X \in A) = \frac {\int_ {A} f _ {(X , Y)} (x , y) \mathrm{d} x}{\int_ {A} f _ {X} (x) \mathrm{d} x}.
$$

The case where $A = \{ a \}$ does not make sense here since then we would have zero in the denominator. However, formally we may put 

$$
h (y | X = a) = \frac {f _ {(X , Y)} (a , y)}{f _ {X} (a)}
$$

which makes sense if only $f _ { X } ( a ) \ \neq \ 0$ . This restriction turns out to be not relevant since 

$$
\begin{array}{l} P ((X, Y) \in \{(x, y): f _ {X} (x) = 0 \}) = \int_ {\{(x, y): f _ {X} (x) = 0 \}} f _ {(X, Y)} (x, y)   \mathrm{d} x   \mathrm{d} y \\ \qquad = \int_ {\{x: f _ {X} (x) = 0 \}} \int_ {\mathbb {R}} f _ {(X, Y)} (x, y)   \mathrm{d} y   \mathrm{d} x \\ \qquad = \int_ {\{x: f _ {X} (x) = 0 \}} f _ {X} (x)   \mathrm{d} x \\ \qquad = 0. \end{array}
$$

We may thus define the conditional probability of $Y \in B$ given $X \ = \ a$ by means of $h ( y | X = a )$ which we briefly write as $h ( y | a )$ 

$$
P (Y \in B | X = a) = \int_ {B} h (y | a) \mathrm{d} y
$$

and the conditional expectation 

$$
\mathbb {E} (Y | X = a) = \int_ {\mathbb {R}} y h (y | a) \mathrm{d} y.
$$

This can be viewed as a random variable with X as the source of randomness. Namely, for $\omega \in \varOmega$ we write 

$$
\mathbb {E} (Y | X) (\omega) = \int_ {\mathbb {R}} y h (y | X (\omega)) \mathrm{d} y.
$$

This function is of course measurable with respect to the σ-field generated by $X$ 

The expectation of this random variable can be computed using Fubini’s theorem: 

$$
\begin{array}{l} \mathbb {E} (\mathbb {E} (Y | X)) = \mathbb {E} (\int_ {\mathbb {R}} y h (y | X (\omega)) \mathrm{d} y) \\ \qquad = \int_ {\mathbb {R}} \int_ {\mathbb {R}} y h (y | x) \mathrm{d} y f _ {X} (x) \mathrm{d} x \\ \qquad = \int_ {\mathbb {R}} \int_ {\mathbb {R}} y f _ {(X, Y)} (x, y) \mathrm{d} x \mathrm{d} y \\ \qquad = \int_ {\mathbb {R}} y f _ {Y} (y) \mathrm{d} y \\ \qquad = \mathbb {E} (Y). \end{array}
$$

More generally, for $A \subset \varOmega , A = X ^ { - 1 } ( B )$ , B Borel, 

$$
\begin{array}{l} \int_ {A} \mathbb {E} (Y | X) \mathrm{d} P = \int_ {\Omega} \mathbf {1} _ {B} (X) \mathbb {E} (Y | X) \mathrm{d} P \\ \qquad = \int_ {\Omega} \mathbf {1} _ {B} (X (\omega)) (\int_ {\mathbb {R}} y h (y | X (\omega)) \mathrm{d} y) \mathrm{d} P (\omega) \\ \qquad = \int_ {\mathbb {R}} \int_ {\mathbb {R}} \mathbf {1} _ {B} (x) y h (y | x) \mathrm{d} y f _ {X} (x) \mathrm{d} x \\ \qquad = \int_ {\mathbb {R}} \int_ {\mathbb {R}} \mathbf {1} _ {B} (x) y f _ {(X, Y)} (x, y) \mathrm{d} x \mathrm{d} y \\ \qquad = \int_ {\Omega} \mathbf {1} _ {A} (X) Y \mathrm{d} P \\ \qquad = \int_ {A} Y \mathrm{d} P. \end{array}
$$

This provides a motivation for a general notion of conditional expectation of a random variable Y given random variable $X \colon \mathbb { E } ( Y | X )$ is a random variable measurable with respect to the σ-field ${ \mathcal { F } } _ { X }$ generated by X and such that for all $A \in { \mathcal { F } } _ { X }$ 

$$
\int_ {A} \mathbb {E} (Y | X) \mathrm{d} P = \int_ {A} Y \mathrm{d} P.
$$

We will pursue these ideas further in the next chapter. 

## Exercise 6.9

Let $f _ { X , Y } = \mathbf { 1 } _ { A }$ , where A is the triangle with corners at $( 0 , 0 ) , ( 2 , 0 )$ 2 $( 0 , 1 )$ . Find the conditional density $h ( y , x )$ and conditional expectation E $( Y | X = 1 )$ 

## Exercise 6.10

Let $f _ { X , Y } ( x , y ) = ( x + y ) \mathbf { 1 } _ { A }$ , where $A = [ 0 , 1 ] \times [ 0 , 1 ]$ . Find $\mathbb { E } ( X | Y = y )$ for each $y \in \mathbb R$ 

## 6.5.4 Characteristic functions determine distributions

We have now suficient tools to prove a fundamental property of characteristic functions. 

## Theorem 6.17 (Inversion Formula)

If the cumulative distribution function of a random variable X is continuous at $a , b \in \mathbb { R }$ , then 

$$
F _ {X} (b) - F _ {X} (a) = \lim _ {c \to \infty} \frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\mathrm{e} ^ {- \mathrm{i} u a} - \mathrm{e} ^ {- \mathrm{i} u b}}{\mathrm{i} u} \varphi_ {X} (u) \mathrm{d} u.
$$

## Proof

First, by the definition of $\varphi _ { X }$ 

$$
\frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\mathrm{e} ^ {- \mathrm{i} u a} - \mathrm{e} ^ {- \mathrm{i} u b}}{\mathrm{i} u} \varphi_ {X} (u) \mathrm{d} u = \frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\mathrm{e} ^ {- \mathrm{i} u a} - \mathrm{e} ^ {- \mathrm{i} u b}}{\mathrm{i} u} \int_ {\mathbb {R}} \mathrm{e} ^ {\mathrm{i} u x} \mathrm{d} P _ {X} (x) \mathrm{d} u.
$$

We may apply Fubini’s theorem since 

$$
\left| \frac {\mathrm{e} ^ {- \mathrm{i} u a} - \mathrm{e} ^ {- \mathrm{i} u b}}{\mathrm{i} u} \mathrm{e} ^ {\mathrm{i} u x} \right| = \left| \int_ {a} ^ {b} \mathrm{e} ^ {\mathrm{i} u x} \mathrm{d} (x) \right| \leq b - a
$$

which is integrable with respect to $P _ { X } \times m _ { [ - c , c ] }$ . We compute the integral in u 

$$
\frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\mathrm{e} ^ {- \mathrm{i} u a} - \mathrm{e} ^ {- \mathrm{i} u b}}{\mathrm{i} u} \mathrm{e} ^ {\mathrm{i} u x} \mathrm{d} u = \frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\mathrm{e} ^ {\mathrm{i} u (x - a)} - \mathrm{e} ^ {\mathrm{i} u (x - b)}}{\mathrm{i} u} \mathrm{d} u =
$$

$$
\frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\sin u (x - a) - \sin u (x - b)}{u} \mathrm{d} u + \frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\cos u (x - a) - \cos u (x - b)}{\mathrm{i} u} \mathrm{d} u.
$$

The second integral vanishes since the integrand is an odd function. We change variables in the first: $y = u ( x - a ) , z = u ( x - b )$ and then it takes the form 

$$
I (x, c) = \frac {1}{2 \pi} \int_ {- c (x - a)} ^ {c (x - a)} \frac {\sin y}{y} \mathrm{d} y - \frac {1}{2 \pi} \int_ {- c (x - b)} ^ {c (x - b)} \frac {\sin z}{z} \mathrm{d} z = I _ {1} (x, c) - I _ {2} (x, c),
$$

say. We employ the following elementary fact without proof: 

$$
\int_ {s} ^ {t} \frac {\sin y}{y} \mathrm{d} y \rightarrow \pi \quad \mathrm{as} t \rightarrow \infty , s \rightarrow - \infty .
$$

Consider the following cases: 

1. $x < a ,$ , then also $x < b$ and $c ( x - a )  - \infty , c ( x - b )  - \infty , - c ( x - a )  \infty .$ $- c ( x - b ) \to \infty { \mathrm { ~ a s ~ } } c \to \infty$ . Hence $I _ { 1 } ( x , c ) \to - { \textstyle \frac { 1 } { 2 } } , I _ { 2 } ( x , c ) \to - { \textstyle \frac { 1 } { 2 } }$ and so $I ( x , c ) \to 0 .$ 

2. $x > b ,$ , then also $x > a ,$ , and $c ( x - a )  \infty , c ( x - b )  \infty , - c ( x - a )  - \infty .$ $\begin{array} { r } { - c ( x - b )  - \infty , \mathrm { ~ a s ~ } c  \infty \mathrm { ~ s o ~ } I _ { 1 } ( x , c )  \frac { 1 } { 2 } , I _ { 2 } ( x , c )  \frac { 1 } { 2 } } \end{array}$ and the result is the same as in 1. 

3. $a < x < b$ hence $I _ { 1 } ( x , c )  { \textstyle { \frac { 1 } { 2 } } } , I _ { 2 } ( x , c )  - { \textstyle { \frac { 1 } { 2 } } }$ and the limit of the whole expression is 1. 

Write $f ( x ) = \operatorname* { l i m } _ { c \to \infty } I ( x , c )$ (we have not discussed the values $x = a , x = b$ but they are irrelevant as will be seen). 

$$
\begin{array}{r} \lim _ {c \to \infty} \frac {1}{2 \pi} \int_ {- c} ^ {c} \frac {\mathrm{e} ^ {- \mathrm{i} u a} - \mathrm{e} ^ {- \mathrm{i} u b}}{\mathrm{i} u} \varphi_ {X} (u) \mathrm{d} u = \lim _ {c \to \infty} \int_ {\mathbb {R}} I (x, c) \mathrm{d} P _ {X} (x) \\ = \int_ {\mathbb {R}} f (x) \mathrm{d} P _ {X} (x) \end{array}
$$

by Lebesgue’s dominated convergence theorem. The integral of f can be easily computed since f is a simple function: 

$$
\int_ {\mathbb {R}} f (x) \mathrm{d} P _ {X} (x) = P _ {X} ((a, b ]) = F _ {X} (b) - F _ {X} (a)
$$

$( P _ { X } ( \{ a \} ) = P _ { X } ( \{ b \} ) = 0$ since $F _ { X }$ is continuous at a and b). 

## Corollary 6.18

The characteristic function determines the probability distribution. 

## Proof

Since $F _ { X }$ is monotone, it is continuous except (possibly) at countably many points where it is right-continuous. Its values at discontinuity points can be approximated from above by the values at continuity points. The latter are determined by the characteristic function via the inversion formula. 

Finally, we see that $F _ { X }$ determines the measure $P _ { X }$ . This is certainly so for $B = ( a , b ] \colon P _ { X } ( ( a , b ] ) = F _ { X } ( b ) - F _ { X } ( a )$ . Next we show the same for any interval, then for finite unions of intervals, and the final extension to any Borel set is via the monotone class theorem. □ 

## Theorem 6.19

If $\varphi _ { X }$ is integrable, then X has a density which is given by 

$$
f _ {X} (x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \mathrm{e} ^ {- \mathrm{i} u x} \varphi_ {X} (u) \mathrm{d} u.
$$

## Proof

The function f is well-defined. To show that it is a density of X we first show that it gives the right values of the probability distribution of intervals $( a , b ]$ where $F _ { X }$ is continuous: 

$$
\begin{array}{r l} & {\int_ {a} ^ {b} f _ {X} (x) \mathrm{d} x = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \varphi_ {X} (u) \left(\int_ {a} ^ {b} \mathrm{e} ^ {- \mathrm{i} u x} \mathrm{d} x\right) \mathrm{d} u} \\ & {\qquad = \lim _ {c \to \infty} \frac {1}{2 \pi} \int_ {- c} ^ {c} \varphi_ {X} (u) \left(\int_ {a} ^ {b} \mathrm{e} ^ {- \mathrm{i} u x} \mathrm{d} x\right) \mathrm{d} u} \\ & {\qquad = \lim _ {c \to \infty} \frac {1}{2 \pi} \int_ {- c} ^ {c} \varphi_ {X} (u) {\frac {\mathrm{e} ^ {- \mathrm{i} u a} - \mathrm{e} ^ {- \mathrm{i} u b}}{\mathrm{i} u}} \mathrm{d} u} \\ & {\qquad = F _ {X} (b) - F _ {X} (a)} \end{array}
$$

by the inversion formula. This extends to all a, b since $F _ { X }$ is right continuous and the integral on the left is continuous with respect to a and b. Moreover, $F _ { X }$ is non-decreasing so $\begin{array} { r } { \int _ { a } ^ { b } f _ { X } ( x ) \mathrm { d } x \geq 0 } \end{array}$ for all $a \leq b$ hence $f _ { X } \geq 0$ . Finally 

$$
\int_ {- \infty} ^ {\infty} f _ {X} (x) \mathrm{d} x = \lim _ {b \to \infty} F _ {X} (b) - \lim _ {a \to - \infty} F _ {X} (a) = 1
$$

so $f _ { X }$ is a density. 

## 6.5.5 Application to mathematical finance

Classical portfolio theory is concerned with an analysis of the balance between risk and return. This balance is of fundamental importance, particularly in corporate finance, where the key concept is the cost of capital, which is a rate of return based on the level of risk of an investment. In probabilistic terms, return is represented by the expectation and risk by the variance. A theory which deals only with two moments of a random variable is relevant if we assume the normal (Gaussian) distribution of random variables in question, since in that case these two moments determine the distribution uniquely. We give a brief account of basic facts of portfolio theory under this assumption. 

Let k be a return on some investment in single period, that is, $k ( \omega ) =$ $\frac { V ( 1 , \omega ) - V ( 0 ) } { V ( 0 ) }$ where $V ( 0 )$ is the known amount invested at the beginning, and $V ( 1 )$ is the random terminal value. A typical example which should be kept in mind is buying and selling one share of some stock. With a number of stocks available, we are facing a sequence $k _ { i }$ of returns on stock $\begin{array} { r } { S _ { i } , k _ { i } = \frac { S _ { i } ( 1 , \omega ) - S _ { i } ( 0 ) } { S _ { i } ( 0 ) } } \end{array}$ 2 but for simplicity we restrict our attention to just two, $k _ { 1 } , \ k _ { 2 }$ . A portfolio is formed by deciding the percentage split, between holdings in $S _ { 1 }$ and $S _ { 2 }$ , of the initial wealth $V ( 0 )$ by choosing the weights $\mathbf { w } = ( w _ { 1 } , w _ { 2 } ) , w _ { 1 } + w _ { 2 } = 1$ . Then, as is well known and elementary to verify, the portfolio of $\begin{array} { r } { n _ { 1 } = \frac { w _ { 1 } V ( 0 ) } { S _ { 1 } ( 0 ) } } \end{array}$ shares of stock number one and $\begin{array} { r } { n _ { 2 } = \frac { w _ { 2 } V ( 0 ) } { S _ { 2 } ( 0 ) } } \end{array}$ shares of stock number two, has return 

$$
k _ {\mathbf {w}} = w _ {1} k _ {1} + w _ {2} k _ {2}.
$$

We assume that the vector $( k _ { 1 } , k _ { 2 } )$ is jointly normal with correlation coeficient $\rho .$ . We denote the expectations and variances of the ingredients by $\mu _ { i } = \mathbb { E } ( k _ { i } )$ $\sigma _ { i } ^ { 2 } = \mathrm { V a r } ( k _ { i } )$ . It is convenient to introduce the following matrix 

$$
C = \left[ \begin{array}{c c} {c _ {1 1}} & {c _ {1 2}} \\ {c _ {2 1}} & {c _ {2 2}} \end{array} \right] = \left[ \begin{array}{c c} {\sigma_ {1} ^ {2}} & {\rho \sigma_ {1} \sigma_ {2}} \\ {\rho \sigma_ {1} \sigma_ {2}} & {\sigma_ {2} ^ {2}} \end{array} \right]
$$

where $c _ { 1 2 } = c _ { 2 1 }$ is the covariance between $k _ { 1 }$ and $k _ { 2 }$ . Assume (which is not elegant to do but saves us an algebraic detour) that C is invertible, with $C ^ { - 1 } =$ $\left[ d _ { i j } \right]$ . By definition, the joint density has the form 

$$
f (x _ {1}, x _ {2}) = \frac {1}{2 \pi \sqrt {\det C}} \exp \{- \frac {1}{2} \sum_ {i, j = 1} ^ {2} d _ {i j} (x _ {i} - \mu_ {i}) (x _ {j} - \mu_ {j}) \}
$$

It is easy to see that (6.5) is a particular case of this formula with $\mu _ { i } = 0$ 2 $\sigma _ { i } = 1 , - 1 < \rho < 1$ . It is well known that the characteristic function $\varphi ( t _ { 1 } , t _ { 2 } ) =$ $\mathbb { E } ( \exp \{ \mathrm { i } ( t _ { 1 } k _ { 1 } + t _ { 2 } k _ { 2 } ) \} )$ of the vector $( k _ { 1 } , k _ { 2 } )$ is of the form 

$$
\varphi (t _ {1}, t _ {2}) = \exp \{i \sum_ {i = 1} ^ {2} t _ {i} \mu_ {i} - \frac {1}{2} \sum_ {i. j = 1} ^ {2} c _ {i j} t _ {i} t _ {j} \}.\tag{6.8}
$$

We shall show that the return on the portfolio is also normally distributed and we shall find the expectation and standard deviation. This can all be done in one step 

## Theorem 6.20

The characteristic $\varphi _ { \mathbf { w } }$ function of $k _ { \mathbf { w } }$ is of the form 

$$
\varphi_ {\mathbf {w}} (t) = \exp \{i t (w _ {1} \mu_ {1} + w _ {2} \mu_ {2})) - \frac {1}{2} t ^ {2} (w _ {1} ^ {2} \sigma_ {1} ^ {2} + w _ {2} ^ {2} \sigma_ {2} ^ {2} + 2 w _ {1} w _ {2} \rho \sigma_ {1} \sigma_ {2}) \}
$$

## Proof

By definition $\varphi _ { \mathbf { w } } ( t ) = \mathbb { E } ( \exp \{ i t k _ { \mathbf { w } } \} )$ and using the form of $k _ { \mathbf { w } }$ we have 

$$
\begin{array}{r l} & {\varphi_ {\mathbf {w}} (t) = \mathbb {E} (\exp \{i t (w _ {1} k _ {1} + w _ {2} k _ {2}) \}} \\ & {\qquad = \mathbb {E} (\exp \{i t w _ {1} k _ {1} + i t w _ {2} k _ {2} \})} \\ & {\qquad = \varphi (t w _ {1}, t w _ {2})} \end{array}
$$

by the definition of the characteristic function of a vector. Since the vector is normal, (6.8) immediately gives the result. □ 

The multi-dimensional version of Corollary 6.18 (which is easy to believe after mastering the one-dimensional case, but slightly tedious to prove, so we take it for granted, referring the reader to any probability textbook) shows that $k _ { \mathbf { w } }$ has normal distribution with 

$$
\begin{array}{r l} & {\mu_ {\mathbf {w}} = w _ {1} \mu_ {1} + w _ {2} \mu_ {2}} \\ & {\sigma_ {\mathbf {w}} ^ {2} = w _ {1} ^ {2} \sigma_ {1} ^ {2} + w _ {2} ^ {2} \sigma_ {2} ^ {2} + 2 w _ {1} w _ {2} \rho \sigma_ {1} \sigma_ {2}} \end{array}
$$

The fact that the variance of a portfolio can be lower than the variances of the components is crucial. These formulae are valid in general case (i.e. without the assumption of a normal distribution) and can be easily proved using the formula for $k _ { \mathbf { w } }$ . The main goal of this section was to see that the portfolio return is normally distributed. 

## Example 6.4

Suppose that the second component is not random, i.e. $S _ { 2 } ( 1 )$ is a constant independent of ω. Then the return $k _ { 2 }$ is risk-free and it is denoted by r (the notation is usually reserved for the case where the length of the period is one year). It can be thought of as a bank account and it is convenient to assume that $S _ { 2 } ( 0 ) = 1$ . Then the portfolio of n shares purchased at the price $S _ { 1 } ( 0 )$ and m units of the bank account has the value $V ( 1 ) = n S _ { 1 } ( 1 ) + m ( 1 + r )$ at the end of the period and the expected return is $\begin{array} { r } { \dot { k } _ { \bf w } ~ = ~ w _ { 1 } \dot { \mu } _ { 1 } + w _ { 2 } r , ~ w _ { 1 } ~ = ~ \frac { n S _ { 1 } ( 0 ) } { V ( 0 ) } ~ } \end{array}$ $w _ { 2 } ~ = ~ 1 - w _ { 1 }$ . The assumption of normal joint returns is violated but the standard deviation of this portfolio can be easily computed directly from the 

<!-- === Source: MinerU_markdown_Measure,_Integral_and_Probability_(Marek_Capiński,_Ekkehard_Kopp)_201_2122706850364366855.md (Page 201) === -->

definition giving $\sigma _ { \mathbf { w } } = w _ { 1 } \sigma _ { 1 } ~ ( \sigma _ { 2 } = 0$ of course and the formula is consistent with the above). 

## Remark 6.3

The above considerations can be immediately generalized to portfolios built of any finite number of ingredients with the following key formulae 

$$
\begin{array}{l} k _ {\mathbf {w}} = \sum w _ {i} k _ {i}, \\ \mu_ {\mathbf {w}} = \sum w _ {i} \mu_ {i}, \\ \sigma_ {\mathbf {w}} ^ {2} = \sum_ {i, j} w _ {i} w _ {j} c _ {i j}. \end{array}
$$

This is just the beginning of the story started in the 1950s by Nobel prize winner Harry Markowitz. A vast number of papers and books on this topic have been written since, proving the general observation that ‘simple is beautiful’. 

## 6.6 Proofs of propositions

## Proof (of Proposition 6.2)

Denote by $\mathcal { F } _ { \mathcal { R } }$ the σ-field generated by the Borel ‘rectangles’ $\mathcal { R } \ : = \ : \{ B _ { 1 } \times $ $B _ { 2 } : B _ { 1 } , B _ { 2 } \in B \}$ , and by $\mathcal { F } _ { \mathcal { T } }$ the σ-field generated by the true rectangles $\mathcal { T } = \{ I _ { 1 } \times I _ { 2 } : I _ { 1 } , I _ { 2 }$ are intervals . 

Since $\mathcal { T } \subset \mathcal { R }$ , obviously $\mathcal { F } _ { \mathcal { Z } } \subset \mathcal { F } _ { \mathcal { R } }$ 

To show the inverse inclusion we show that Borel cylinders $B _ { 1 } \times \varOmega _ { 2 }$ and $\varOmega _ { 1 } \times B _ { 2 }$ are in $\mathcal { F } _ { \mathcal { T } }$ . For that write $\mathcal { D } = \{ A : A \times \Omega _ { 2 } \in \mathcal { F } _ { \mathcal { I } } \}$ , note that this is a σ-field containing all intervals hence $B \subset D$ as required. □ 

## Proof (of Proposition 6.11)

Let $s _ { n } = \sum c _ { k } \mathbf { 1 } _ { A _ { k } }$ be an increasing sequence of simple functions convergent to $f .$ . Let $R _ { k } = A _ { k } \times [ 0 , c _ { k } ]$ and the union of such rectangles is in fact $\textstyle \int s _ { n } \mathrm { d } m$ Then $\textstyle \bigcup _ { n = 1 } ^ { \infty } \bigcup _ { k } R _ { k } = A _ { f }$ so $A _ { f }$ is measurable. 

S SFor the second claim take a $y$ section of $A _ { f }$ which is the interval $[ 0 , f ( x ) )$ Its measure is $f ( x )$ and by the definition of the product measure $m _ { 2 } ( A _ { f } ) =$ $\textstyle \int f ( x )$ dx. □ 

## Proof (of Proposition 6.16)

The joint density is the product of the densities: $f _ { X , Y } ( x , y ) = f _ { X } ( x ) f _ { Y } ( y )$ and substituting this to (6.6) immediately gives the result. □ 

# The Radon–Nikodym Theorem

In this chapter we shall consider the relationship between a real Borel measure ν and the Lebesgue measure m. Key to such relationships is Theorem 4.17, which shows that for each non-negative integrable real function f, the set function 

$$
A \mapsto \nu (A) = \int_ {A} f \mathrm{d} m\tag{7.1}
$$

defines a (Borel) measure ν on (R, ). The natural question to ask is the converse: exactly which real Borel measures can be found in this way? We shall find a complete answer to this question in this chapter, and in keeping with our approach in Chapters 5 and 6, we shall phrase our results in terms of general measures on an abstract set Ω. 

## 7.1 Densities and Conditioning

The results we shall develop in this chapter also allow us to study probability densities (introduced in Section 4.7.2), conditional probabilities and conditional expectations (see Sections 5.4.3 and 6.5.3) in much greater detail. For ν as defined above to be a probability measure, we clearly require $\textstyle \int f \mathrm { d } m = 1$ . In particular, if $\nu = P _ { X }$ is the distribution of a random variable X the function $f = f _ { X }$ corresponding to $\nu$ in (7.1) was called the density of X. 

In similar fashion we defined the joint density $f _ { ( X , Y ) }$ of two random variables in Section 6.5.1, by reference of their joint distribution to two-dimensional 

Lebesgue measure $m _ { 2 } { \mathrm { : } }$ if X and $Y$ are real random variables defined on some probability space $( \varOmega , \mathcal { F } , P )$ their joint distribution is the measure defined on Borel subsets B of $\mathbb { R } ^ { 2 }$ by $P _ { ( X , Y ) } ( B ) = P ( ( X , Y ) \in B )$ . In the special case where this measure, relative to $m _ { 2 }$ , is given as above by an integrable function $f _ { ( X , Y ) }$ , we say that X and $Y$ have this function as their joint density. 

This, in turn, leads naturally (see Section 6.5.3) to the concepts of conditional density 

$$
h (y | a) = h (y | X = a) = \frac {f _ {(X , Y)} (a , y)}{f _ {X} (a)}
$$

and conditional expectation 

$$
\mathbb {E} (Y | X = a) = \int_ {\mathbb {R}} y h (y | a) \mathrm{d} y.
$$

Recalling that $X : \varOmega  \mathbb { R }$ , the last equation can be written as ${ \mathbb E } ( Y | X ) ( \omega ) =$ $\begin{array} { r } { \int _ { \mathbb { R } } y h ( y | X ( \omega ) ) } \end{array}$ dy, displaying the conditional expectation as a random variable $\mathbb { E } ( Y | X ) : \varOmega \to \mathbb { R }$ , measurable with respect to the σ-field ${ \mathcal { F } } _ { X }$ generated by X. An application of Fubini’s theorem leads to a fundamental identity, valid for all $A \in { \mathcal { F } } _ { X }$ f f 

$$
\int_ {A} \mathbb {E} (Y | X) \mathrm{d} P = \int_ {A} Y \mathrm{d} P.\tag{7.2}
$$

The existence of this random variable in the general case, irrespective of the existence of a joint density, is of great importance in both theory and applications – Williams [12] calls it ‘the central definition of modern probability’. It is essential for the concept of martingale, which plays such a crucial role in many applications, and which we introduce at the end of this chapter. 

As we described in Section 5.4.3, the existence of orthogonal projections in $L ^ { 2 }$ allows one to extend the scope of the definition further still: instead of restricting ourselves to random variables measurable with respect to σ-fields of the form ${ \mathcal { F } } _ { X }$ we specify any sub-σ-field $\mathcal { G }$ of $\mathcal { F }$ and ask for a -measurable random variable $\mathbb { E } ( Y | \mathcal { G } )$ to play the role of $\mathbb { E } ( Y | X ) = \mathbb { E } ( Y | \mathcal { F } _ { X } )$ in (7.2). As was the case for product measures, the most natural context for establishing the properties of the conditional expectation is that of general measures; note that the proof of Theorem 4.17 simply required monotone convergence to establish the countable additivity of P. We therefore develop the comparison of abstract measures further, as always guided by the specific examples of random variables and distributions. 

## 7.2 The Radon–Nikodym Theorem

In the special case where the measure ν has the form $\textstyle \nu ( A ) = \int _ { A } f$ dm for some Rnon-negative integrable function f we said (Section 4.7.2) that ν is absolutely continuous with respect to m. It is immediate that $\textstyle \int _ { A } f \mathrm { d } m = 0$ whenever $m ( A ) = 0$ (see Theorem 4.3 (iv)). Hence $m ( A ) = 0$ Rimplies $\nu ( A ) = 0$ when the measure ν is given by a density. We use this as a definition for the general case of two given measures. 

## Definition 7.1

Let $\varOmega$ be a set and let $\mathcal { F }$ be a $\sigma \mathrm { - }$ -field of its subsets. (The pair $( \varOmega , \mathscr { F } )$ is a measurable space) Suppose that ν and $\mu$ are measures on $( \varOmega , \mathscr { F } )$ . We say that $\nu$ is absolutely continuous with respect to $\mu$ if $\mu ( A ) = 0$ implies $\nu ( A ) = 0$ for $A \in { \mathcal { F } }$ . We write this as $\nu \ll \mu$ 

## Exercise 7.1

Let $\lambda _ { 1 } , \lambda _ { 2 }$ and $\mu$ be measures on $( \varOmega , \mathscr { F } )$ . Show that if $\lambda _ { 1 } \ll \mu$ and $\lambda _ { 2 } \ll \mu$ then $\left( \lambda _ { 1 } + \lambda _ { 2 } \right) \ll \mu$ 

It will not be immediately obvious what this definition has to do with the usual notion of continuity of functions. We shall see later in this chapter how it fits with the concept of absolute continuity of real functions. For the present, we note the following reformulation of the definition, which is not needed for the main result we will prove, but serves to bring the relationship between ν and $\mu$ a little ‘closer to home’ and is useful in many applications: 

## Proposition 7.1

Let ν and $\mu$ be finite measures on the measurable space $( \varOmega , \mathscr { F } )$ . Then $\nu \ll \mu$ if and only if for every $\varepsilon > 0$ there exists a $\delta > 0$ such that for $F \in { \mathcal { F } } , \mu ( F ) < \delta$ implies $\nu ( F ) < \varepsilon$ 

Hint Suppose the $( \varepsilon , \delta )$ -condition fails. We can then find $\varepsilon > 0$ and sets $\left( F _ { n } \right)$ such that for all $\textstyle n \geq 1 , \mu ( F _ { n } ) < { \frac { 1 } { 2 ^ { n } } }$ but $\nu ( F _ { n } ) > \varepsilon$ . Consider $\mu ( A )$ and $\nu ( A )$ for $\begin{array} { r } { A = \bigcap _ { n \geq 1 } ( \bigcup _ { i \geq n } F _ { i } ) } \end{array}$ 

We generalise from the special case of Lebesgue measure: if $\mu$ is any measure on $( \varOmega , \mathscr { F } )$ and $f : \varOmega \to \mathbb { R }$ is a measurable function for which $\textstyle \int f \mathrm { d } \mu$ exists, then $\textstyle \nu ( F ) = \int _ { F } f \mathrm { d } \mu$ defines a measure $\nu \ll \mu$ R. (This follows exactly as for $m$ , since $\mu ( F ) = 0$ implies $\textstyle \int _ { F } f \mathrm { d } \mu = 0$ . Note that we employ the convention $0 \times \infty = 0 . )$ RFor σ-finite measures, the following key result asserts the converse: 

## Theorem 7.2 (Radon–Nikodym)

Given two σ-finite measures ν, µ on a measurable space $( \varOmega , \mathscr { F } )$ , with $\nu \ll \mu ,$ then there is a non-negative measurable function $h : \varOmega \to \mathbb { R }$ such that $\nu ( F ) =$ $\textstyle \int _ { F } h \mathrm { d } \mu$ for every $F \in { \mathcal { F } }$ . The function h is unique up to µ-null sets: if g also Rsatisfies $\textstyle \nu ( F ) = \int _ { F } g \mathrm { d } \mu$ for all $F \in { \mathcal { F } }$ , then $g = h \mathrm { \ a . e . \ } ( \mu )$ 

Since the most interesting case for applications arises for probability spaces and then $h \in \mathcal { L } ^ { 1 } ( \mu )$ , we shall initially restrict attention to the case where $\mu$ and ν are finite measures. In fact, it is helpful initially to take $\mu$ to be a probability measure, i.e. $\mu ( \varOmega ) = 1$ . From among several diferent approaches to this very important theorem, we base our argument on one given by R.C. Bradley in the American Mathematical Monthly (Vol 96, no 5., May 1989, pp. 437–440), since it ofers the most ‘constructive’ and elementary treatment of which we are aware. 

It is instructive to begin with a special case: Suppose (until further notice) that $\mu ( \varOmega ) = 1$ . We say that the measure µ dominates ν when $0 \leq \nu ( F ) \leq \mu ( F )$ for every $F \in { \mathcal { F } }$ . This obviously implies $\nu \ll \mu .$ . In this simplified situation we shall construct the required function h explicitly. First we generalise the idea of partitions and their refinements, which we used to good efect in constructing the Riemann integral, to measurable subsets in $( \varOmega , \mathscr { F } )$ 

## Definition 7.2

Let $( \varOmega , \mathscr { F } )$ be a measurable space. A finite (measurable) partition of $\varOmega$ is a finite collection of disjoint subsets $\mathcal { P } = ( A _ { i } ) _ { i \leq n }$ in $\mathcal { F }$ whose union is $\varOmega .$ . The finite partition ${ \mathcal { P } } ^ { \prime }$ is a refinementof if each set in $\mathcal { P }$ is a disjoint union of sets in ${ \mathcal { P } } ^ { \prime }$ 

Exercise 7.2 

Let $\mathcal { P } _ { 1 }$ and $\mathcal { P } _ { 2 }$ be finite partitions of Ω. Show that the coarsest partition (i.e. with least number of sets) which refines them both consists of all intersections $A \cap B$ , where $A \in \mathcal { P } _ { 1 } , B \in \mathcal { P } _ { 2 }$ 

The following is a simplified ‘Radon–Nikodym theorem’ for dominated measures: 

## Theorem 7.3

Suppose that $\mu ( \varOmega ) = 1$ and $0 \leq \nu ( F ) \leq \mu ( F )$ for every $F \in { \mathcal { F } }$ . Then there exists a non-negative ${ \mathcal { F } } .$ -measurable function h on Ω such that $\textstyle \nu ( F ) = \int _ { F } h \mathrm { d } \mu$ for all $F \in { \mathcal { F } }$ 

We shall prove this in three steps: in Step 1 we define the required function $h _ { \mathcal { P } }$ for sets in a finite partition $\mathcal { P }$ and compare the functions $h _ { \mathcal { P } _ { 1 } }$ and $h _ { \mathcal { P } _ { 2 } }$ when the partition $\mathcal { P } _ { 2 }$ refines $\mathcal { P } _ { 1 }$ . This enables us to show that the integrals $\int _ { \Omega } h _ { \mathcal { P } } ^ { 2 } \mathrm { d } \mu$ are non-decreasing if we take successive refinements. Since they are also bounded above (by 1), $\begin{array} { r } { c = \operatorname* { s u p } \int _ { \Omega } h _ { \mathcal { P } } ^ { 2 } \mathrm { d } \mu } \end{array}$ exists in R. In Step 2 we then construct the desired function h by a careful limit argument, using the convergence theorems of Chapter 4. In Step 3 we show that h has the desired properties. 

## Step 1: The function h for a finite partition

Suppose that $0 \leq \nu ( F ) \leq \mu ( F )$ for every $F \in { \mathcal { F } }$ . Let $\mathcal { P } = \{ A _ { 1 } , A _ { 2 } , \ldots , A _ { k } \}$ be a finite partition of Ω such that each $A _ { i } \in { \mathcal { F } }$ . Define the simple function $h _ { \mathcal { P } } : \varOmega \to \mathbb { R }$ by setting 

$h _ { \mathcal { P } } ( \omega ) = c _ { i } = \frac { \nu ( A _ { i } ) } { \mu ( A _ { i } ) }$ for $\omega \in A _ { i }$ when $\mu ( A _ { i } ) > 0$ , and $h _ { \mathcal { P } } ( \omega ) = 0$ otherwise. 

Since $h _ { \mathcal { P } }$ is constant on each ‘atom $\begin{array} { r } { A _ { i } , \nu ( A _ { i } ) = \int _ { A _ { i } } h _ { \mathcal { P } } \mathrm { d } \mu } \end{array}$ . Then $h _ { \mathcal { P } }$ has the following properties: 

(i) For each finite partition of $\varOmega , 0 \leq h _ { \mathcal { P } } ( \omega ) \leq 1$ for all $\omega \in \varOmega$ 

(ii) If $A = \textstyle \bigcup _ { i \in J } A _ { j }$ for an index set $J \subset \{ 1 , 2 , . . . k \}$ then $\textstyle \nu ( A ) = \int _ { F } h _ { \mathcal { P } } \mathrm { d } \mu$ Thus $\begin{array} { r } { \nu ( \bar { \varOmega } ) = \int _ { \varOmega } h _ { \mathcal { P } } \mathrm { d } \mu } \end{array}$ 

(iii) If $\mathcal { P } _ { 1 }$ and $\mathcal { P } _ { 2 }$ are finite partitions of Ω and $\mathcal { P } _ { 2 }$ refines $\mathcal { P } _ { 1 }$ then, with $\boldsymbol { h _ { n } } = \boldsymbol { h _ { \mathcal { P } _ { n } } }$ $( n = 1 , 2 )$ we have 

(a) for all $\begin{array} { r } { A \in \mathcal { P } _ { 1 } , \int _ { A } h _ { 1 } \mathrm { d } \mu = \nu ( A ) = \int _ { A } h _ { 2 } \mathrm { d } \mu , } \end{array}$ 

(b) for all $\begin{array} { r } { A \in \mathcal { P } _ { 1 } , \int _ { A } h _ { 1 } h _ { 2 } \mathrm { d } \mu = \int _ { A } h _ { 1 } ^ { 2 } \mathrm { d } \mu . } \end{array}$ 

(iv) $\begin{array} { r } { \int _ { \Omega } ( h _ { 2 } ^ { 2 } - h _ { 1 } ^ { 2 } ) \mathrm { d } \mu = \int _ { \Omega } ( h _ { 2 } - h _ { 1 } ) ^ { 2 } \mathrm { d } \mu } \end{array}$ and therefore 

$$
\int_ {\Omega} h _ {2} ^ {2} \mathrm{d} \mu = \int_ {\Omega} h _ {1} ^ {2} \mathrm{d} \mu + \int_ {\Omega} (h _ {2} - h _ {1}) ^ {2} \mathrm{d} \mu \geq \int_ {\Omega} h _ {1} ^ {2} \mathrm{d} \mu .
$$

We now prove these assertions in turn. 

(i) This is trivial by construction of $h _ { \mathcal { P } }$ , since $\mu$ dominates $\nu .$ 

(ii) Let $A = \textstyle \bigcup _ { j \in J } A _ { j }$ for some index set $J \subset \{ 1 , 2 , \ldots , k \}$ . Since the $\{ A _ { j } \}$ are disjoint and $\nu ( A _ { j } ) = 0$ whenever $\mu ( A _ { j } ) = 0$ , we have 

$$
\begin{array}{l} \nu (A) = \sum_ {j \in J} \nu (A _ {j}) = \sum_ {j \in J, \mu (A _ {i}) > 0} \frac {\nu (A _ {j})}{\mu (A _ {j})} \mu (A _ {j}) \\ \qquad = \sum_ {j \in J, \mu (A _ {i}) > 0} c _ {j} \mu (A _ {j}) = \sum_ {j \in J} \int_ {A _ {j}} h _ {\mathcal {P}}   \mathrm{d} \mu \\ \qquad = \int_ {A} h _ {\mathcal {P}}   \mathrm{d} \mu . \end{array}
$$

In particular, since $\mathcal { P }$ partitions Ω, this holds for $A = \varOmega$ 

(iii) (a) With the $\mathcal { P } _ { n } , h _ { n }$ as above $( n = 1 , 2 )$ we can write $A = \cup _ { j \in J } B _ { j }$ for each $A \in \mathcal { P } _ { 1 }$ , where J is a finite index set and $B _ { j } \in { \mathcal { P } } _ { 2 }$ S. The sets $B _ { j }$ are pairwise disjoint, and again $\nu ( B _ { j } ) = 0$ when $\mu ( B _ { j } ) = 0$ , so that 

$$
\begin{array}{c} \int_ {A} h _ {1} \mathrm{d} \mu = \nu (A) = \sum_ {j \in J} \nu (B _ {j}) = \sum_ {j \in J, \mu (B _ {j}) > 0} \frac {\nu (B _ {j})}{\mu (B _ {j})} \mu (B _ {j}) \\ = \sum_ {j \in J} \int_ {B _ {j}} h _ {2} \mathrm{d} \mu = \int_ {A} h _ {2} \mathrm{d} \mu . \end{array}
$$

(b) With A as in part (a) and $\mu ( A ) > 0$ , note that $\begin{array} { r } { h _ { 1 } = \frac { \nu ( A ) } { \mu ( A ) } } \end{array}$ is constant on A, so that 

$$
\int_ {A} h _ {1} h _ {2} \mathrm{d} \mu = \frac {\nu (A)}{\mu (A)} \int_ {A} h _ {2} \mathrm{d} \mu = \frac {(\nu (A)) ^ {2}}{\mu (A)} = \int_ {A} (\frac {\nu (A)}{\mu (A)}) ^ {2} \mathrm{d} \mu = \int_ {A} h _ {1} ^ {2} \mathrm{d} \mu .
$$

(iv) By (iii) (b), $\begin{array} { r } { \int _ { A } h _ { 1 } ( h _ { 2 } - h _ { 1 } ) \mathrm { d } \mu = 0 } \end{array}$ for every $A \in { \mathcal { P } } _ { 1 }$ . Since the $A _ { i } \in \mathcal { P } _ { 1 }$ partition Ω, we also have 

$$
\int_ {\Omega} h _ {1} (h _ {2} - h _ {1}) \mathrm{d} \mu = \sum_ {i = 1} ^ {k} \int_ {A _ {i}} h _ {1} (h _ {2} - h _ {1}) \mathrm{d} \mu = 0.
$$

Hence 

$$
\begin{array}{r l} \int_ {\Omega} (h _ {2} - h _ {1}) ^ {2} \mathrm{d} \mu & = \int_ {\Omega} (h _ {2} ^ {2} - 2 h _ {1} h _ {2} + h _ {1} ^ {2}) \mathrm{d} \mu \\ & = \int_ {\Omega} [ h _ {2} ^ {2} - 2 h _ {1} (h _ {2} - h _ {1}) - h _ {1} ^ {2} ] \mathrm{d} \mu \\ & = \int_ {\Omega} (h _ {2} ^ {2} - h _ {1} ^ {2}) \mathrm{d} \mu , \end{array}
$$

and thus 

$$
\int_ {\Omega} h _ {2} ^ {2} \mathrm{d} \mu = \int_ {\Omega} h _ {1} ^ {2} \mathrm{d} \mu + \int_ {\Omega} (h _ {2} - h _ {1}) ^ {2} \mathrm{d} \mu \geq \int_ {\Omega} h _ {1} ^ {2} \mathrm{d} \mu .
$$

## Step 2: Passage to the limit – construction of $h .$

In Step 1 we showed that the integrals $\int _ { \Omega } h _ { \mathcal { P } } ^ { 2 } \mathrm { d } \mu$ are non-decreasing over suc-Rcessive refinements of a finite partition of Ω. Moreover, by (i) above, each function $h _ { \mathcal { P } }$ satisfies $0 \leq h _ { \mathcal { P } } ( \omega ) \leq 1$ for all $\omega \in \varOmega$ . Thus, setting $\begin{array} { r } { c = \operatorname* { s u p } \int _ { \Omega } h _ { \mathcal { P } } ^ { 2 } \mathrm { d } \mu } \end{array}$ 8 where the supremum is taken over all finite partitions of $\varOmega .$ , we have $0 \leq c \leq 1$ (Here we use the assumption that $\mu ( \varOmega ) = 1 . )$ 

For each $n \geq 1$ let $\mathcal { P } _ { n }$ be a finite measurable partition of Ω such that $\begin{array} { r } { \int _ { \Omega } h _ { \mathcal { P } _ { n } } ^ { 2 } \mathrm { d } \mu > c - \frac { 1 } { 4 ^ { n } } } \end{array}$ . Let $\mathcal { Q } _ { n }$ be the smallest common refinement of the partitions $\mathcal { P } _ { 1 } , \mathcal { P } _ { 2 } , \ldots , \mathcal { P } _ { n }$ . For each $n , \mathcal { Q } _ { n }$ refines $\mathcal { P } _ { n }$ by construction, and $\mathcal { Q } _ { n + 1 }$ refines $\mathcal { Q } _ { n }$ since each $\mathcal { Q } _ { k }$ consists of all intersections $A _ { 1 } \cap A _ { 2 } \cap . . . \cap A _ { k }$ , where $A _ { i } \in { \mathcal { P } } _ { i }$ 8 $i \leq k$ . Hence each set in $\mathcal { Q } _ { n }$ is a disjoint union of sets in $\mathcal { Q } _ { n + 1 }$ . We therefore have the inequalities: 

$$
c - \frac {1}{4 ^ {n}} <   \int_ {\Omega} h _ {\mathcal {P} _ {n}} ^ {2} \mathrm{d} \mu \leq \int_ {\Omega} h _ {\mathcal {Q} _ {n}} ^ {2} \mathrm{d} \mu \leq \int_ {\Omega} h _ {\mathcal {Q} _ {n + 1}} ^ {2} \mathrm{d} \mu \leq c.
$$

Using the identity proved in Step 1 (iv), we now have 

$$
\int_ {\Omega} (h _ {\mathcal {Q} _ {n + 1}} - h _ {\mathcal {Q} _ {n}}) ^ {2} \mathrm{d} \mu = \int_ {\Omega} (h _ {\mathcal {Q} _ {n + 1}} ^ {2} - h _ {\mathcal {Q} _ {n}} ^ {2}) \mathrm{d} \mu <   \frac {1}{4 ^ {n}}.
$$

The Schwarz inequality applied with $f = | h _ { \mathcal { Q } _ { n + 1 } } - h _ { \mathcal { Q } _ { n } } |$ and $g \equiv 1$ , then yields for each $n \geq 1$ 

$$
\int_ {\Omega} \left| h _ {\mathcal {Q} _ {n + 1}} - h _ {\mathcal {Q} _ {n}} \right| \mathrm{d} \mu <   \frac {1}{2 ^ {n}}.
$$

By the Beppo–Levi Theorem, since $\begin{array} { r l } { } & { { } \sum _ { n > 1 } \int _ { \Omega } \left| h _ { \mathcal { Q } _ { n + 1 } } - h _ { \mathcal { Q } _ { n } } \right| \mathrm { d } \mu } \end{array}$ is finite, we conclude that the series $\begin{array} { r } { \sum _ { n \geq 1 } ( h _ { \mathcal { Q } _ { n + 1 } } - h _ { \mathcal { Q } _ { n } } ) } \end{array}$ converges almost everywhere $( \mu )$ ， Pso that the limit function 

$$
h = h _ {\mathcal {P} _ {1}} + \sum_ {n \geq 1} (h _ {\mathcal {Q} _ {n + 1}} - h _ {\mathcal {Q} _ {n}}) = \lim _ {n} h _ {\mathcal {Q} _ {n}}
$$

(noting that $\mathcal { Q } _ { 1 } = \mathcal { P } _ { 1 } )$ is well-defined almost everywhere $( \mu )$ . We complete the construction by setting $h = 0$ on the exceptional µ-null set. 

Step 3: Verification of the properties of h. 

By Step 1 (i) it follows that $0 \leq h ( \omega ) \leq 1$ , and it is clear from its construc tion that h is -measurable. 

We need to show that $\textstyle \nu ( F ) = \int _ { F } h \mathrm { d } \mu$ for every $F \in \mathcal { F }$ . Fix any such measurable set F and let $n \geq 1$ R. Define $\mathcal { R } _ { n }$ as the smallest common refinement of the two partitions $\mathcal { Q } _ { n }$ (defined as in Step 2) and $\{ F , F ^ { c } \}$ . Since F is a finite disjoint union of sets in $\mathcal { R } _ { n }$ , we have $\textstyle \nu ( F ) = \int _ { F } h _ { \mathcal { R } _ { n } } \mathrm { d } \mu$ from Step 1 (ii). 

By Step 2, $\begin{array} { r } { c - \frac { 1 } { 4 ^ { n } } < \int _ { \Omega } h _ { \mathcal { Q } _ { n } } ^ { 2 } \mathrm { d } \mu \leq \int _ { \Omega } h _ { \mathcal { R } _ { n } } ^ { 2 } \mathrm { d } \mu \leq c , } \end{array}$ so, as before, we can conclude that $\begin{array} { r } { \int _ { \Omega } ( h _ { \mathcal { R } _ { n } } - h _ { \mathcal { Q } _ { n } } ) ^ { 2 } \mathrm { d } \mu < \frac { 1 } { 4 ^ { n } } } \end{array}$ , and using the Schwarz inequality once more, this time with $g = { \bf 1 } _ { F }$ , we have 

$$
\left| \int_ {F} \left(h _ {\mathcal {R} _ {n}} - h _ {\mathcal {Q} _ {n}}\right) \mathrm{d} \mu \right| \leq \int_ {F} \left| h _ {\mathcal {R} _ {n}} - h _ {\mathcal {Q} _ {n}} \right| \mathrm{d} \mu <   \frac {1}{2 ^ {n}}.
$$

For all $\begin{array} { r } { n , \nu ( F ) = \int _ { F } h _ { \mathcal { R } _ { n } } \mathrm { d } \mu = \int _ { F } ( h _ { \mathcal { R } _ { n } } - h _ { \mathcal { Q } _ { n } } ) \mathrm { d } \mu + \int _ { F } h _ { \mathcal { Q } _ { n } } \mathrm { d } \mu } \end{array}$ . The first integral on the right converges to 0 as $n \to \infty$ , while the second converges to $\textstyle \int _ { F } h \mathrm { d } \mu$ by dominated convergence theorem (since for all $n \geq 1 , 0 \leq h _ { \mathscr { Q } _ { n } } \leq 1$ Rand $\mu ( \varOmega )$ is finite). Thus we have verified that $\textstyle \nu ( F ) = \int _ { F } h \mathrm { d } \mu$ , as required. 

It is straightforward to check that the assumption $\mu ( \varOmega ) = 1$ is not essential since for any finite positive measure $\mu$ we can repeat the above arguments using $\frac { \mu } { \mu ( \varOmega ) }$ instead of $\mu$ . We write the function h defined above as $\textstyle { \frac { d \nu } { d \mu } }$ and call it the Radon–Nikodym derivative of ν with respect to $\mu$ . Its relationship to derivatives of functions will become clear when we consider real functions of bounded variation. 

## Exercise 7.3

Let $\varOmega = [ 0 , 1 ]$ with Lebesgue measure and consider measures $\mu , \nu$ given by densities ${ \bf 1 } _ { A } , { \bf 1 } _ { B }$ respectively. Find a condition on the sets $A , B$ so that $\mu$ dominates ν and find the Radon-Nikodym derivative $\textstyle { \frac { d \nu } { d \mu } }$ applying the above definition of the function h. 

## Exercise 7.4

Suppose $\varOmega$ is a finite set equipped with the algebra of all subsets. Let $\mu$ and ν be two measures on $\varOmega$ such that $\mu ( \{ \omega \} ) \neq 0 , \nu ( \{ \omega \} ) \neq 0$ , for all $\omega \in \varOmega$ . Decide under which conditions $\mu$ dominates ν and find $\textstyle { \frac { d \nu } { d \mu } }$ 

The next observation is an easy application of the general procedure highlighted in Remark 4.1: 

## Proposition 7.4

If $\mu$ and $\varphi$ are finite measures with $0 \leq \mu \leq \varphi$ , and if $\begin{array} { r } { h _ { \mu } = \frac { d \mu } { d \varphi } } \end{array}$ is constructed as above, then for any non-negative -measurable function $g$ on $\varOmega$ we have 

$$
\int_ {\Omega} g \mathrm{d} \mu = \int_ {\Omega} g h _ {\mu} \mathrm{d} \varphi .
$$

The same identity holds for any $g \in { \mathcal { L } } ^ { 1 } ( \mu )$ 

Hint Begin with indicator functions, use linearity of the integral to extend to simple functions, and monotone convergence for general non-negative $g .$ . The rest is obvious from the definitions. 

For finite measures we can now prove the general result announced earlier: 

## Theorem 7.5 (Radon–Nikodym)

Let ν and $\mu$ be finite measures on the measurable space $( \varOmega , \mathscr { F } )$ and suppose that $\nu \ll \mu$ . Then there is a non-negative ${ \mathcal { F } } .$ -measurable function h on $\varOmega$ such that $\textstyle \nu ( A ) = \int _ { A } h \mathrm { d } \mu$ for all $A \in { \mathcal { F } }$ 

## Proof

Let $\varphi = \nu + \mu$ . Then $\varphi$ is a positive finite measure which dominates both ν and $\mu .$ . Hence the Radon–Nikodym derivatives $\begin{array} { r } { h _ { v } \ = \ \frac { d \nu } { d \varphi } } \end{array}$ and $\begin{array} { r } { h _ { \mu } \ : = \ : \frac { d \mu } { d \varphi } } \end{array}$ are well-defined by the earlier constructions. Consider the sets $F = \{ h _ { \mu } > 0 \}$ and $G = \{ h _ { \mu } = 0 \}$ in $\mathcal { F }$ . Clearly $\begin{array} { r } { \mu ( G ) = \int _ { G } h _ { \mu } \mathrm { d } \varphi = 0 } \end{array}$ , hence also $\nu ( G ) = 0$ , since $\begin{array} { r } { h = \frac { h _ { \nu } } { h _ { \mu } } \mathbf { 1 } _ { F } } \end{array}$ C $\nu \ll \mu$ . Define , and let $A \in { \mathcal { F } } , A \subset F$ . By the previous proposition, with $h \mathbf { 1 } _ { A }$ instead of $g _ { ; }$ , we have 

$$
\nu (A) = \int_ {A} h _ {\nu} \mathrm{d} \varphi = \int_ {A} h h _ {\mu} \mathrm{d} \varphi = \int_ {A} h \mathrm{d} \mu
$$

as required. Since $\mu$ and ν are both null on $G$ this proves the theorem. 

## Exercise 7.5

Let $\varOmega = [ 0 , 1 ]$ with Lebesgue measure and consider probability measures µ, ν given by densities $f , g$ respectively. Find a condition characterising the absolute continuity $\nu \ll \mu$ and find the Radon-Nikodym derivative $\textstyle { \frac { d \nu } { d \mu } }$ 

## Exercise 7.6

Suppose $\varOmega$ is a finite set equipped with the algebra of all subsets and let $\mu$ and ν be two measures on $\varOmega$ . Characterise the absolute continuity $\nu \ll \mu$ and find $\textstyle { \frac { d \nu } { d \mu } }$ 

You can now easily complete the picture for σ-finite measures and verify that the function $h$ is ‘essentially unique’: 

## Proposition 7.6

The Radon–Nikodym theorem remains valid if the measures ν and $\mu$ are $\sigma -$ finite: for any two such measures with $\nu \ll \mu$ we can find a finite-valued nonnegative measurable function $f$ on $\varOmega$ such that $\textstyle \nu ( F ) = \int _ { F } h \mathrm { d } \mu$ for all $F \in { \mathcal { F } }$ The function $h$ Rso defined is unique up to µ-null sets, i.e. if $g : \varOmega \to \mathbb { R } ^ { + }$ also satisfies $\textstyle \nu ( F ) = \int _ { \Omega } g \mathrm { d } \mu$ for all $F \in { \mathcal { F } }$ then $g = h { \mathrm { ~ a . e ~ } }$ . (with respect to $\mu )$ 

Hint There are sequences $( A _ { n } ) , ( B _ { m } )$ of sets in $\mathcal { F }$ with $\mu ( A _ { n } ) , \nu ( B _ { m } )$ finite for all $m , n \geq 1$ and $\textstyle \bigcup _ { n > 1 } A _ { n } = \varOmega = \bigcup _ { m > 1 } B _ { m }$ . We can choose these to be Ssequences of disjoint sets $\mathrm { ( w h y ? ) }$ S. Hence display $\varOmega$ as the disjoint union of the sets $A _ { n } \cap B _ { m } \ ( m , n \geq 1 )$ , thus finding a sequence $\left( C _ { n } \right)$ of disjoint sets with union $\varOmega .$ all of whose members have finite measure under both $\mu$ and $\nu .$ Fix n and apply the above results to the measurable space $( \varOmega , \mathcal { F } _ { n } )$ , where ${ \mathcal { F } } _ { n } = \{ F \cap C _ { n } : F \in { \mathcal { F } } \}$ , then ‘paste together’ the resulting functions for all $n$ . 

Radon-Nikodym derivatives of measures obey simple combination rules which follow from the uniqueness property. We illustrate this with the sum and composition of two Radon-Nikodym derivatives, and leave the ’inverse $\mathrm { r u l e } ^ { \prime }$ as an exercise. 

## Proposition 7.7

Assume we are given $\sigma { \mathrm { - f i n i t e } }$ measures $\lambda , \nu , \mu$ satisfying $\lambda \ll \mu$ and $\nu \ll \mu$ with Radon-Nikodym derivatives $\textstyle { \frac { d \lambda } { d \mu } }$ and $\textstyle { \frac { d \nu } { d \mu } }$ , respectively. 

(i) With $\phi = \lambda + \nu$ we have $\begin{array} { r } { \frac { d \phi } { d \mu } = \frac { d \lambda } { d \mu } + \frac { d \nu } { d \mu } } \end{array}$ a.s. (µ), 

(ii) If $\lambda \ll \nu$ then $\begin{array} { r } { \frac { d \lambda } { d \mu } = \frac { d \lambda } { d \nu } \frac { d \nu } { d \mu } } \end{array}$ a.s. $( \mu )$ 

## Exercise 7.7

Show that if $\mu , \nu$ are equivalent measures, i.e. both $\nu \ll \mu$ and $\mu \ll \nu$ are true, then 

$$
\frac {d \mu}{d \nu} = (\frac {d \nu}{d \mu}) ^ {- 1} \mathrm{a.s.} (\mu).
$$

Given a pair of σ-finite measures $\lambda , \mu$ on $( \varOmega , \mathscr { F } )$ it is natural to ask whether we can identify the sets for which $\mu ( E ) = 0$ implies $\lambda ( E ) = 0$ . This would mean that we can split the mass of λ into two pieces, one being represented by a µ-integral, and the other ‘concentrated’ on $\mu { \mathrm { - } } \mathrm { n u l l }$ sets, i.e. away from the mass of $\mu$ . We turn this idea of ‘separating’ the masses of two measures into the following 

## Definition 7.3

If there is a set $E \in { \mathcal { F } }$ such that $\lambda ( F ) = \lambda ( E \cap F )$ for every $F \in { \mathcal { F } }$ then λ is concentrated on E. If two measures µ, ν are concentrated on disjoint subsets of $\varOmega$ , we say that they are mutually singular and write $\mu \perp \nu$ 

Clearly, if λ is concentrated on E and $E \cap F = \emptyset$ , then $\lambda ( F ) = \lambda ( E \cap F ) = 0$ Conversely, if for all $F \in { \mathcal { F } } , F \cap E = \emptyset$ implies $\lambda ( F ) = 0$ , consider $\lambda ( F ) =$ $\lambda ( F \cap E ) + \lambda ( F \setminus E )$ . Since $( F \setminus E ) \cap E = \emptyset$ we must have $\lambda ( F { \setminus } E ) = 0 .$ , so $\lambda ( F ) = \lambda ( F \cap E )$ . We have proved that λ is concentrated on E if and only if for all $F \in { \mathcal { F } } , F \cap E = \emptyset$ implies $\lambda ( F ) = 0$ . We gather some simple facts about mutually singular measures: 

## Proposition 7.8

If $\mu , \nu , \lambda _ { 1 , } \lambda _ { 2 }$ are measures on a σ-field , the following are true: 

(i) If $\lambda _ { 1 } \perp \mu$ and $\lambda _ { 2 } \perp \mu$ then also $( \lambda _ { 1 } + \lambda _ { 2 } ) \perp \mu$ 

(ii) If $\lambda _ { 1 } \ll \mu$ and $\lambda _ { 2 } \perp \mu$ then $\lambda _ { 2 } \perp \lambda _ { 1 }$ 

(iii) If $\nu \ll \mu$ and $\nu \perp \mu$ then $\nu = 0$ 

Hint For (i), with $i = 1 , 2$ let $A _ { i } , B _ { i }$ be disjoint sets with $\lambda _ { i }$ concentrated on $A _ { i } , \mu$ on $B _ { i }$ . Consider $A _ { 1 } \cup A _ { 2 }$ and $B _ { 1 } \cap B _ { 2 }$ . For (ii) use the remark preceding the proposition. 

The next result shows that a unique ‘mass splitting’ of a σ-finite measure relative to another is always possible: 

## Theorem 7.9 (Lebesgue decomposition)

Let $\lambda , \mu$ be σ-finite measures on $( \varOmega , \mathscr { F } )$ . Then λ can be expressed uniquely as a sum of two measures, $\lambda = \lambda _ { a } + \lambda _ { s }$ where $\lambda _ { a } \ll \mu$ and $\lambda _ { s } \bot \mu$ 

## Proof

Existence: We consider finite measures; the extension to the σ-finite case is routine. Since $0 \leq \lambda \leq \lambda + \mu = \varphi$ , i.e. $\phi$ dominates λ, there is $0 \leq h \leq 1$ such that $\textstyle \lambda ( E ) = \int _ { E } h \mathrm { d } \varphi$ for all measurable E. Let $A = \{ \omega : h ( \omega < 1 \}$ and $B =$ $\{ \omega : h ( \omega ) = 1 \}$ . Set $\lambda _ { a } ( E ) = \lambda ( A \cap E )$ and $\lambda _ { s } ( E ) = \lambda ( B \cap E )$ for every $E \in { \mathcal { F } }$ Now if $E \subset A$ and $\mu ( E ) = 0$ then $\begin{array} { r } { \lambda ( E ) \ : = \ : \int _ { E } h \mathrm { d } \varphi \ : = \ : \int _ { E } h \mathrm { d } \lambda } \end{array}$ , so that $\begin{array} { r } { \int _ { E } ( 1 - h ) \mathrm { d } \lambda = 0 } \end{array}$ . But $h < 1$ R Ron A, hence also on E. Therefore we must have $\lambda ( E ) = 0$ . Hence if $E \in { \mathcal { F } }$ and $\mu ( E ) = 0 , \lambda _ { a } ( E ) = \lambda ( A \cap E ) = 0$ as $A \cap E \subset A$ 

So $\lambda _ { a } ~ \ll ~ \lambda$ . On the other hand, if $E \subset B$ we obtain $\begin{array} { r } { \lambda ( E ) ~ = ~ \int _ { E } h \mathrm { d } \varphi ~ = ~ } \end{array}$ $\begin{array} { r } { \int _ { E } \mathbf { 1 } \mathrm { d } ( \lambda + \mu ) = \lambda ( E ) + \mu ( E ) } \end{array}$ , so that $\mu ( E ) = 0 . { \mathrm { ~ A s ~ } } A = B ^ { c }$ Rwe have shown Rthat $\mu ( E ) = 0$ whenever $E \cap A = \emptyset$ , so that $\mu$ is concentrated on A. Since $\lambda _ { s }$ is concentrated on B this shows that $\lambda _ { s }$ and $\mu$ are mutually singular. 

Uniqueness is left to the reader. (Hint: employ Proposition 7.8.) The theorem is proved. □ 

Combining this with the Radon–Nikodym theorem we can describe the structure of λ with respect to $\mu$ as ‘basis measure’: 

## Corollary 7.10

With $\mu , \lambda , \lambda _ { a } , \lambda _ { s }$ as in the theorem, there is a µ-a.s. unique non-negative measurable function h such that $\begin{array} { r } { \lambda ( E ) = \int _ { E } h \mathrm { d } \mu + \lambda _ { s } ( E ) } \end{array}$ for every $E \in { \mathcal { F } }$ 

## Remark 7.1

This result is reminiscent of the structure theory of finite-dimensional vector spaces: if $x \in \mathbb { R } ^ { n }$ and $m < n$ , we can write $x = y + z$ , where $\boldsymbol { y } = \sum _ { i = 1 } ^ { m } y _ { i } \boldsymbol { e } _ { i }$ is the orthogonal projection onto $\mathbb { R } ^ { m }$ Pand z is orthogonal to this subspace. We also exploited similar ideas for Hilbert space. In this sense the measure $\mu$ has the role of a ‘basis’ providing the ‘linear combination’ which describes the projection of the measure λ onto a subspace of the space of measures on $\varOmega$ 

## Exercise 7.8

Consider the following measures on the real line: $P _ { 1 } ~ = ~ \delta _ { 0 } , ~ P _ { 2 } ~ =$ ${ \textstyle \frac { 1 } { 2 5 } } m | _ { [ 0 , 2 5 ] } , P _ { 3 } = { \textstyle \frac { 1 } { 2 } } P _ { 1 } + { \textstyle \frac { 1 } { 2 } } P _ { 2 }$ (see Example 3.1). For which $i \neq j$ do we have $P _ { i } \ll P _ { j } ?$ Find the Radon-Nikodym derivative in each such case. 

## Exercise 7.9

Let $\lambda = \delta _ { 0 } + m | _ { [ 1 , 3 ] } , \mu = \delta _ { 1 } + m | _ { [ 2 , 4 ] }$ and find $\lambda _ { a } , \lambda _ { s }$ , and h as in Corollary 7.10. 

## 7.3 Lebesgue–Stieltjes measures

Recall (see Section 3.5.3) that given any random variable $X : \varOmega \longrightarrow \mathbb { R }$ , we define its probability distribution as the measure $P _ { X } = P \circ X ^ { - 1 }$ on Borel sets on R (i.e. we set $P ( X \ \leq \ x ) = P \circ X ^ { - 1 } ( ( - \infty , x ] ) = P _ { X } ( ( - \infty , x ] )$ and extend this to .) Setting $F _ { X } ( x ) \ = \ P _ { X } ( ( - \infty , x ] )$ we verified in Proposition 4.30 that the distribution function $F _ { X }$ so defined is monotone increasing, right-continuous, with limits at infinity $\begin{array} { r } { F _ { X } ( - \infty ) = \operatorname* { l i m } _ { x  - \infty } F _ { X } ( x ) = 0 } \end{array}$ and $\begin{array} { r } { F _ { X } ( + \infty ) = \operatorname* { l i m } _ { x \to \infty } F _ { X } ( x ) = 1 } \end{array}$ 

In Chapter 4 we studied the special case where $F _ { X } ( x ) = P _ { X } ( ( - \infty , x ] ) =$ $\textstyle \int _ { - \infty } ^ { x } f _ { X }$ dm for some real function $f _ { X }$ , the density of $P _ { X }$ with respect to Lebesgue measure m, Proposition 4.22 showed that if $f _ { X }$ is continuous, then $F _ { X }$ is diferentiable and has the density $f _ { X }$ as its derivative at every $x \in \mathbb { R }$ . On the other hand, the Lebesgue function in Example 4.8 illustrated that continuity of $F _ { X }$ is not suficient to guarantee the existence of a density. 

Moreover, when $F _ { X }$ has a density $f _ { X }$ , the measure $P _ { X }$ was said to be $\mathrm { ^ 6 a b \mathrm { - } }$ solutely continuous’ with respect to m. In the context of the Radon–Nikodym theorem we should reconcile the terminology of this special case with the general one considered in the present Chapter. Trivially, when $\textstyle P _ { X } ( B ) = \int _ { B } f _ { X }$ dm we have $P _ { X } \ \ll \ m$ , so that $P _ { X }$ has a Radon–Nikodym derivative $\textstyle { \frac { d { \bar { P } } _ { X } } { d m } }$ with respect to m. The a.s. uniqueness ensures that $\textstyle { \frac { d P _ { X } } { d m } } = f _ { X } { \mathrm { ~ a . s } }$ 

Later in this chapter we shall establish the precise analytical requirements on the cumulative distribution function $F _ { X }$ which will guarantee the existence of a density. 

## 7.3.1 Construction of Lebesgue–Stieltjes measures

To do this we first study, only slightly more generally, measures defined on (R, ) which correspond in similar fashion to increasing, right-continuous functions on $\mathbb { R } .$ . Their construction mirrors that of Lebesgue measure, with only a few changes, by generalising the concept of ‘interval length’. The measures we obtain are known as Lebesgue-Stieltjes measures. In this context we call a function $F : \mathbb { R } \longrightarrow \mathbb { R }$ a distribution function if $F$ is monotone increasing and right-continuous. It is clear that every finite measure $\mu$ defined on (R, ) defines such a function by $F ( x ) = \mu ( ( - \infty , x ] )$ , with $F ( - \infty ) = \operatorname* { l i m } _ { x  - \infty } F ( x ) = 0$ 2 $\begin{array} { r } { F ( + \infty ) = \operatorname* { l i m } _ { x  \infty } F ( x ) = \mu ( \varOmega ) } \end{array}$ 

Our principal concern, however, is with the converse: given a monotone right-continuous $F : \mathbb { R } \longrightarrow \mathbb { R }$ , can we always associate with $F$ a measure on (Ω, ), and if so, what is its relation to Lebesgue measure? 

The first question is answered by looking back carefully at the construction of Lebesgue measure m on R in Chapter 2: first we defined the natural concept of interval length, $l ( I ) = b - a .$ for any interval I with endpoints $a , b \ ( a < b )$ 2 and by analogy with our discussion of null sets, we defined Lebesgue outer measure $m ^ { * }$ for an arbitrary subset of R as the infimum of the total lengths $\textstyle \sum _ { n = 1 } ^ { \infty } l ( I _ { n } )$ of all sequences $( I _ { n } ) _ { n \geq 1 } \mathrm { o f }$ intervals covering A. To generalise this idea, we should clearly replace $b - a$ by $F ( b ) - F ( a )$ to obtain a ’generalised interval length’ relative to $F$ , but since F is only right-continuous we will need to take care of possible discontinuities. Thus we need to identify the possible discontinuities of monotone increasing functions – fortunately these functions are rather well-behaved, as you can easily verify in the following: 

## Proposition 7.11

If $F : \mathbb { R } \longrightarrow \mathbb { R }$ is monotone increasing $( { \mathrm { i . e . ~ } } x _ { 1 } \leq x _ { 2 }$ implies $F ( x _ { 1 } ) \leq F ( x _ { 2 } ) )$ then the left-limit $F ( x - )$ and the right-limit $F ( x + )$ exist at every $x \in \mathbb { R }$ and $F ( x - ) \leq F ( x ) \leq F ( x + )$ . Hence $F$ has at most countably many discontinuities, and these are jump discontinuities, i.e. $F ( x - ) < F ( x + )$ 

Hint For any x, consider sup $\{ F ( y ) : y < x \}$ and inf $\{ F ( y ) : x < y \}$ to verify the first claim. For the second, note that $F ( x - ) < F ( x + )$ if F has a discontinuity at x. Use the fact that $\mathbb { Q }$ is dense in R to show that there can only be countably many such points. 

Since $F$ is monotone, it remains bounded on bounded sets. For simplicity we assume that lim $_ { \cdot x \to - \infty } F ( x ) = 0$ . We define the ‘length relative to $F ^ { \prime }$ of the bounded interval $( a , b ]$ by 

$$
l _ {F} (a, b ] = F (b) - F (a).
$$

Note that we have restricted ourselves to left-open, right-closed intervals. Since $F$ is right-continuous, $F ( x + ) \ = \ F ( x )$ for all $x ,$ including $a , b .$ . Thus $l _ { F } ( a , b ] = F ( b + ) - F ( a + )$ , and all jumps of F have the form $F ( x ) - F ( x - )$ By restricting to intervals of this type we also ensure that $l _ { F }$ is additive over adjoining intervals: if $a < c < b$ then $l _ { F } ( a , b ] = l _ { F } ( a , c ] + l _ { F } ( c , b ]$ 

We generalise Definition 2.2 as follows: 

## Definition 7.4

The F-outer measure of any set $A \subseteq \mathbb { R }$ is the element of $[ 0 , \infty ]$ 

$$
m _ {F} ^ {*} (A) = \inf Z _ {F} (A)
$$

where 

$$
Z _ {F} (A) = \{\sum_ {n = 1} ^ {\infty} l _ {F} (I _ {n}): I _ {n} = (a _ {n}, b _ {n} ], a _ {n} \leq b _ {n}, A \subseteq \bigcup_ {n = 1} ^ {\infty} I _ {n} \}.
$$

Our ‘covering intervals’ are now also restricted to be left-open and rightclosed. This is essential to ‘make things fit together’, but does not afect measurability: recall (Theorem 2.16) that the Borel σ-field is generated whether we start from the family of all intervals or from various sub-families. 

Now consider the proof of Theorem 2.4 in more detail: our purpose there was to prove that the outer measure of an interval equals its length. We show how to adapt the proof to make this claim valid for $m _ { F } ^ { * }$ and $l _ { F }$ applied to intervals of the form $( a , b ]$ . It will be therefore helpful to review the proof of Theorem 2.4 before reading on! 

Step 1. The proof that $m _ { F } ^ { * } ( ( a , b ] ) \leq l _ { F } ( a , b ]$ remains much the same: 

To see that $l _ { F } ( a , b ] \in Z _ { F } ( ( a , b ] )$ , we cover $( a , b ] \ \mathrm { b y } \ ( I _ { n } )$ with $I _ { 1 } = ( a , b ]$ 2 ${ { I } _ { n } } = ( a , a ] = \emptyset , n > 1$ . The total length of this sequence is $F ( b ) - F ( a ) =$ $l _ { F } ( a , b ]$ , hence the result follows by definition of inf. 

Step 2. It remains to show that $l _ { F } ( a , b ] \leq m _ { F } ^ { * } ( ( a , b ] )$ . Here we need to be careful always to ‘approach points from the right’ in order to make use of the right-continuity of F and thus to avoid its jumps. 

Fix $\varepsilon > 0$ and $0 < \delta < b - a$ . By definition of inf we can find a covering of $I = ( a , b ]$ by intervals $I _ { n } = ( a _ { n } , b _ { n } ]$ such that $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } l _ { F } ( I _ { n } ) < m _ { F } ^ { * } ( I ) + \frac { \varepsilon } { 2 } } \end{array}$ . Next, let $J _ { n } = \left( a _ { n } , b _ { n } ^ { \prime } \right)$ , where by right-continuity of $F$ , for each $n \geq 1$ we can choose $b _ { n } ^ { \prime } > b _ { n }$ and $\begin{array} { r } { F ( b _ { n } ^ { \prime } ) - F ( b _ { n } ) < \frac { \varepsilon } { 2 ^ { n + 1 } } } \end{array}$ . Then $F ( b _ { n } ^ { \prime } ) - F ( a _ { n } ) < \{ F ( b _ { n } ) - F ( a _ { n } ) \} +$ $\frac { \varepsilon } { 2 ^ { n + 1 } }$ 

The $( J _ { n } ) _ { n \geq 1 }$ then form an open cover of the compact interval $[ a + \delta , b ]$ , so that by the Heine–Borel Theorem there is a finite subfamily $( J _ { n } ) _ { n \leq N }$ , which also covers $[ a + \delta , b ]$ . Re-ordering these N intervals $J _ { n }$ we can assume that their right-hand endpoints form an increasing sequence and then 

$$
\begin{array}{l} F (b) - F (a + \delta) = l _ {F} (a + \delta , b ] \leq \sum_ {n = 1} ^ {N} \{F (b _ {n} ^ {\prime}) - F (a _ {n}) \} \\ <   \sum_ {n = 1} ^ {N} \{F (b _ {n}) - F (a _ {n}) + \frac {\varepsilon}{2 ^ {n + 1}} \} <   \sum_ {n = 1} ^ {\infty} l _ {F} (I _ {n}) + \frac {\varepsilon}{2} \\ <   m _ {F} ^ {*} (I) + \varepsilon . \end{array}
$$

This holds for all $\varepsilon > 0$ , hence $F ( b ) - F ( a + \delta ) \leq m _ { F } ^ { * } ( I )$ for every $\delta > 0$ By right-continuity of F, letting $\delta \downarrow 0$ we obtain $\begin{array} { r } { l _ { F } ( a , b ] = \operatorname* { l i m } _ { \delta \downarrow 0 } l _ { F } ( a + \delta , b ] \leq } \end{array}$ $m _ { F } ^ { * } ( a , b ]$ . This completes the proof that $m _ { F } ^ { * } ( ( a , b ] ) = l _ { F } ( a , b ]$ 

This is the only substantive change needed from the construction that led to Lebesgue measure. The proof that $m _ { F } ^ { * }$ is an outer measure, i.e. 

$$
m _ {F} ^ {*} (A) \geq 0, \quad m _ {F} ^ {*} (\emptyset) = 0, \quad m _ {F} ^ {*} (A) \leq m _ {F} ^ {*} (B) \text {   if   } A \subseteq B,
$$

$$
m _ {F} ^ {*} (\bigcup_ {i = 1} ^ {\infty} A _ {i}) \leq \sum_ {i = 1} ^ {\infty} m _ {F} ^ {*} (A _ {i}),
$$

is word-for-word identical with that given for Lebesgue outer measure (Proposition 2.3, Theorem 2.5). Hence, as in Definition 2.3 we say that a set $E$ is measurable (for the outer measure $m _ { F } ^ { * } )$ if for each $A \subseteq \mathbb { R }$ 

$$
m _ {F} ^ {*} (A) = m _ {F} ^ {*} (A \cap E) + m _ {F} ^ {*} (A \cap E ^ {c}).
$$

Again, the proof of Theorem 2.8 goes through verbatim, and we denote the resulting Lebesgue–Stieltjes measure, i.e. $m _ { F } ^ { * }$ restricted to the σ-field $\mathcal { M } _ { F }$ of Lebesgue–Stieltjes measurable sets, by $m _ { F }$ . By construction, just like Lebesgue measure, m is a complete measure: subsets of $m _ { F } { \mathrm { - n u l l } }$ sets are in $\mathcal { M } _ { F }$ . However, as we shall see later, $\mathcal { M } _ { F }$ does not always coincide with the σ-field  of Lebesgue-measurable sets, although both contain all the Borel sets. It is also straightforward to verify that the properties of Lebesgue measure proved in Section 2.4 hold for general Lebesgue–Stieltjes measures, with one exception: the outer measure $m _ { F } ^ { * }$ will not, in general, be translation-invariant. We can see this at once for intervals, since $l _ { F } ( ( a + t , b + t ] ) = F ( b + t ) - F ( a + t )$ will not usually equal $F ( b ) - F ( a )$ ; simply take $F ( x ) = x ^ { 3 }$ , for example. In fact, it can be shown that Lebesgue measure is the unique translation-invariant measure on R. 

Note, moreover, that a singleton $\{ a \}$ is now not necessarily a null set for $m _ { F } \colon$ we have, by the analogue of Theorem 2.13, that 

$$
m _ {F} (\{a \}) = \lim _ {n \rightarrow \infty} m _ {F} ((a - \frac {1}{n}, a ]) = F (a) - \lim _ {n \rightarrow \infty} F (a - \frac {1}{n}) = F (a) - F (a -).
$$

Thus, the measure of the set $\{ a \}$ is precisely the size of the jump at a (if any). From this it is easy to see by similar arguments how the ‘length’ of an interval depends on the presence or absence of its endpoints: given that m $_ { F } ( ( a , b ] ) =$ $F ( b ) { - } F ( a )$ , we see that: m $\mathbf { \nabla } _ { F } ( ( a , b ) ) = F ( b - ) - F ( a ) , m _ { F } ( [ a , b ] ) = F ( b ) - F ( a - )$ 2 $m _ { F } ( [ a , b ) ) = F ( b - ) - F ( a )$ 

## Example 7.1

When $F = \mathbf { 1 } _ { [ a , \infty ) }$ we obtain $m _ { F } = \delta _ { a }$ , the Dirac measure concentrated at a. Similarly, we can describe a general discrete probability distribution, where the random variable X takes the values $\{ a _ { i } : i = 1 , 2 , \ldots , n \}$ with probabilities $\{ p _ { i } = 1 , 2 , \ldots , n \}$ as the Lebesgue–Stieltjes measure arising from the function $\textstyle F = \sum _ { i = 1 } ^ { n } p _ { i } \mathbf { 1 } _ { [ a _ { i } , \infty ) }$ 

Mixtures of discrete and continuous distributions, such as described in Example 3.1, clearly also fit into this picture. Of course, Lebesgue measure m is the special case where the distribution is uniform, i.e. if $F ( x ) = x$ for all $x \in \mathbb { R }$ then $m _ { F } = m$ 

## Example 7.2

Only slightly more generally, every finite Borel measure $\mu$ on $\mathbb { R }$ corresponds to a Lebesgue–Stieltjes measure, since the distribution function $F ( x ) = \mu ( ( - \infty , x ] )$ is obviously increasing and is right-continuous by Theorem 2.13 applied to $\mu$ and the intervals $I _ { n } = ( - \infty , x + \textstyle { \frac { 1 } { n } } ] )$ . The corresponding Lebesgue–Stieltjes measure $m _ { F } = \mu _ { \mathrm { : } }$ , since they coincide on the generating family of intervals of the above form. Hence they coincide on the σ-field $\boldsymbol { B }$ of Borel sets. By our construction of $m _ { F }$ as a complete measure it follows that $m _ { F }$ is the completion of $\mu$ . 

## Example 7.3

Return to the Lebesgue function F discussed in Example 4.8. Since $F$ is continuous and monotone increasing, it induces a Lebesgue–Stieltjes measure $m _ { F }$ on the interval [0, 1], whose properties we now examine. On each ‘middle thirds’ set $F$ is constant, hence these intervals are null sets for $m _ { F }$ , and as there are countably many of them, so is their union, the ‘middle thirds’ set, D. Hence the Cantor set $C = D ^ { c }$ satisfies 

$$
1 = F (1) - F (0) = m _ {F} ([ 0, 1 ]) = m _ {F} (C)
$$

(Note that since F is continuous, $m _ { F } ( \{ 0 \} ) = F ( 0 ) - F ( 0 - ) = 0 ;$ ; in fact, each singleton is $m _ { F ^ { - } \mathrm { n u l l } . } )$ We thus conclude that $m _ { F }$ is concentrated on a null set for Lebesgue measure m, i.e. m $_ { F \perp m }$ , and that in the Lebesgue decomposition of $m _ { F }$ relative to m there is no absolutely continuous component (by uniqueness of the decomposition). 

## Exercise 7.10

Suppose the monotone increasing function $F$ is non-constant at most countably many points (as would be the case for a discrete distribution). Show that every subset of R is m -measurable. 

Hint Consider $m _ { F }$ over the bounded interval $[ - M , M ]$ first. 

## Exercise 7.11

Find the Lebesgue-Stieltjes measure m<sub>F</sub> generated by 

$$
F (x) = \left\{ \begin{array}{l l} 0 \text {   if   } x <   0, \\ 2 x \text {   if   } x \in [ 0, 1 ], \\ 2 \text {   if   } x \geq 1. \end{array} \right.
$$

## 7.3.2 Absolute continuity of functions

We now address the requirements on a distribution F which ensure that it has a density. As we saw in Example 4.8, continuity of a probability distribution function does not guarantee the existence of a density. The following stronger restriction, however, does the trick: 

## Definition 7.5

A real function F is absolutely continuous on the interval [a, b] if, given $\varepsilon > 0$ there is $\delta > 0$ such that for every finite set of disjoint intervals $J _ { k } = ( x _ { k } , y _ { k } ) , k \le$ n, contained in [a, b] and with $\textstyle \sum _ { k = 1 } ^ { n } ( y _ { k } - x _ { k } ) < \delta$ , we have $\scriptstyle \sum _ { k = 1 } ^ { n } | F ( x _ { k } ) -$ $F ( y _ { k } ) | < \varepsilon$ 

This condition will allow us to identify those distribution functions which generate Lebesgue–Stieltjes measures that are absolutely continuous (in the sense of measures) relative to Lebesgue measure. We will see shortly that absolutely continuous functions are also ‘of bounded variation’: this describes functions which do not ‘vary too much’ over small intervals. First we verify that the indefinite integral (see Proposition 4.22) relative to a density is absolutely continuous. 

## Proposition 7.12

If $f \in { \mathcal { L } } ^ { 1 } ( [ a , b ] )$ , where the interval [a, b] is finite, then the function $F ( x ) =$ $\textstyle \int _ { a } ^ { x } f$ dm is absolutely continuous. 

Hint Use the absolute continuity of $\textstyle \mu ( G ) = \int _ { G } | f |$ dm with respect to Lebesgue measure m. 

## Exercise 7.12

Decide which of the following functions are absolutely continuous: (a) 

$f ( x ) \ = \ | x | , \ x \ \in \ [ - 1 , 1 ] , \ ( \mathrm { b } ) \ g ( x ) \ = \ { \sqrt { x } } , \ x \ \in \ [ 0 , 1 ]$ , (c) the Lebesgue function. 

The next result is the important converse to the above example, and shows that all Stieltjes integrals arising from absolutely continuous functions lead to measures which are absolutely continuous relative to Lebesgue measure, and hence have a density. Together with the Example this characterises the distributions arising from densities (under the conditions we have imposed on distribution functions). 

## Theorem 7.13

If F is monotone increasing and absolutely continuous on R, let $m _ { F }$ be the Lebesgue–Stieltjes measure it generates. Then every Lebesgue-measurable set is m -measurable, and on these sets $m _ { F } \ll m$ 

## Proof

We first show that if the Borel set B has $m ( B ) = 0$ , then also $m _ { F } ( B ) = 0$ Recall that, given $\delta > 0$ we can find an open set O containing B with $m ( O ) < \delta$ (Theorem 2.12), and there is a sequence of disjoint open intervals $( I _ { k } ) _ { k \geq 1 }$ $I _ { k } = \left( a _ { k } , b _ { k } \right)$ with union O. Since the intervals are disjoint, their total length is less than δ. By the absolute continuity of F, given any $\varepsilon > 0$ , we can find $\delta > 0$ such that for every finite sequence of intervals $J _ { k } = ( x _ { k } , y _ { k } ) , k \le n$ , with total length $\begin{array} { r } { \sum _ { k = 1 } ^ { n } ( y _ { k } - x _ { k } ) < \delta } \end{array}$ , we have $\begin{array} { r } { \sum _ { k = 1 } ^ { n } \{ F ( y _ { k } ) - F ( x _ { k } ) \} < \frac { \varepsilon } { 2 } . \mathrm { ~ A ~ } } \end{array}$ pplying this Pto the sequence $( I _ { k } ) _ { k \leq n }$ Pfor a fixed n we obtain $\textstyle \sum _ { k = 1 } ^ { n } \{ F ( b _ { k } ) - F ( a _ { k } ) \} < { \frac { \varepsilon } { 2 } }$ As this holds for every n, we also have $\begin{array} { r } { \sum _ { k = 1 } ^ { \infty } \{ F ( b _ { k } ) - F ( a _ { k } ) \} \le \frac { \varepsilon } { 2 } < \varepsilon } \end{array}$ . This Pis the total length of a sequence of disjoint intervals covering $O \supset B$ , hence $m _ { F } ( B ) < \varepsilon$ for every $\varepsilon > 0 , \sec ( B ) = 0$ 

Now for every Lebesgue-measurable set E with $m ( E ) = 0$ we can find aBorel set $B \supseteq E$ with $m ( B ) = 0$ . Thus also $m _ { F } ( B ) = 0$ . Now E is a subset ofan m -null set, hence it is also $m _ { F } { \mathrm { - n u l l } }$ . Hence all m-measurable sets are m<sub>F</sub>-measurable and m-null sets are $m _ { F } \mathrm { - n u l l }$ , i.e. $m _ { F } \ll$ m when both are regardedas measures on . 口

Together with the Radon-Nikodym Theorem, the above result helps to clarify the structural relationship between Lebesgue measure and Lebesgue– Stieltjes measures generated by monotone increasing right-continuous functions, and thus, in particular, for probability distributions: when the function $F$ is absolutely continuous it has a density f, and can therefore be written as its ‘indefinite integral’. Since the Lebesgue–Stieltjes measure $m _ { F } \ll m$ , the Radon–Nikodym derivative $\textstyle { \frac { d m _ { F } } { d m } }$ is well-defined. Conversely, for the density $f$ of $F$ to exist, the function $F$ must be absolutely continuous. It now remains to clarify the relationship between the Radon–Nikodym derivative $\textstyle { \frac { d m _ { F } } { d m } }$ and the density f. It is natural to expect from the example of a continuous f (Proposition 4.22) that $f$ should be the derivative of $F$ (at least $m \mathrm { - a . e . ) }$ . So we need to understand which conditions on $F$ will ensure that $F ^ { \prime } ( x )$ exists for m-almost all $x \in \mathbb { R }$ 

We shall address this question in the somewhat wider context where the ‘integrator’ function $F$ is no longer necessarily monotone increasing, but has bounded variation, as introduced in the next section. 

## 7.3.3 Functions of bounded variation

Since in general we need to handle set functions that can take negative values, for example, the map 

$$
E \longrightarrow \int_ {E} g \mathrm{d} m, \text {   where   } g \in \mathcal {L} ^ {1} (m),
$$

we therefore need a concept of ‘generalised length functions’ which are expressed as the diference of two monotone increasing functions. We need first to characterise such functions. This is done by introducing the following 

## Definition 7.6

A real function $F$ is of bounded variation on $[ a , b ]$ (briefly $F \in B V [ a , b ] )$ if $T _ { F } [ a , b ] < \infty$ , where for any $x \in [ a , b ]$ 

$$
T _ {F} [ a, x ] = \sup \left\{\sum_ {k = 1} ^ {n} | F (x _ {k}) - F (x _ {k - 1}) | \right\}
$$

with the supremum taken over all finite partitions of $[ a , x ]$ with $a = x _ { 0 } < x _ { 1 } <$ $\ldots < x _ { n } = x$ 

We introduce two further non-negative functions by setting 

$$
P _ {F} [ a, x ] = \sup \{\sum_ {k = 1} ^ {n} [ F (x _ {k}) - F (x _ {k - 1}) ] ^ {+} \}
$$

and 

$$
N _ {F} [ a, x ] = \sup \{\sum_ {k = 1} ^ {n} [ F (x _ {k}) - F (x _ {k - 1}) ] ^ {-} \}
$$

where the supremum is again taken over all partitions of $[ a , x ]$ . The functions $T _ { F } ( P _ { F } , N _ { F } )$ are known respectively as the total (positive, negative) variation functions of F. We shall keep a fixed in what follows, and consider these as functions of x for $x \geq a$ 

We can easily verify the following basic relationships between these definitions: 

## Proposition 7.14

If $F$ is of bounded variation on $[ a , b ]$ , we have $F ( x ) - F ( a ) = P _ { F } ( x ) - N _ { F } ( x )$ while $T _ { F } ( x ) = P _ { F } ( x ) + N _ { F } ( x )$ for $x \in [ a , b ]$ 

Hint Consider $\begin{array} { r } { p ( x ) = \sum _ { k = 1 } ^ { n } [ F ( x _ { k } ) - F ( x _ { k - 1 } ) ] ^ { + } } \end{array}$ and $\begin{array} { r } { n ( x ) = \sum _ { k = 1 } ^ { n } [ F ( x _ { k } ) - } \end{array}$ $F ( x _ { k - 1 } ) ] ^ { - }$ Pfor a fixed partition of $[ a , x ]$ and note that $F ( x ) - F ( a ) = p ( x ) -$ $n ( x )$ . Now use the definition of the supremum. For the second identity consider $T _ { F } ( x ) \geq p ( x ) + n ( x ) = 2 p ( x ) - F ( x ) + F ( a )$ and use the first identity. 

## Proposition 7.15

If $F$ is of bounded variation and $a \leq x \leq b$ then $T _ { F } [ a , b ] = T _ { F } [ a , x ] + T _ { F } [ x , b ]$ Similar results hold for $P _ { F }$ and $N _ { F }$ . Hence all three variation functions are monotone increasing in x for fixed $a \in \mathbb { R }$ . Moreover, if F has bounded variation on [a, b], then it has bounded variation on any $[ c , d ] \subset [ a , b ]$ 

Hint Adding a point to a partition will increase all three sums. On the other hand, putting together partitions of $[ a , c ]$ and $[ c , b ]$ we obtain a partition of $[ a , b ]$ 

We show that bounded variation functions on finite intervals are exactly what we are looking for: 

## Theorem 7.16

Let $[ a , b ]$ be a finite interval. A real function is of bounded variation on $[ a , b ]$ if and only if it is the diference of two monotone increasing real functions on $[ a , b ]$ 

## Proof

If $F$ is of bounded variation, use $F ( x ) = [ F ( a ) + P _ { F } ( x ) ] - N _ { F } ( x )$ from Proposition 7.14 to represent $F$ as the diference of two monotone increasing functions. 

Conversely, if $F = g - h$ is the diference of two monotone increasing functions, then for any partition $a = x _ { 0 } < x _ { 1 } < . . . < x _ { n } = b$ of $[ a , b ]$ we obtain, since $g , h$ are increasing, 

$$
\begin{array}{l} \sum_ {i = 1} ^ {n} | F (x _ {i}) - F (x _ {i - 1}) | = \sum_ {i = 1} ^ {n} | g (x _ {i}) - h (x _ {i}) - g (x _ {i - 1}) + h (x _ {i - 1}) | \\ \qquad \leq \sum_ {i = 1} ^ {n} [ g (x _ {i}) - g (x _ {i - 1}) ] + \sum_ {i = 1} ^ {n} [ h (x _ {i}) - h (x _ {i - 1}) ] \\ \qquad \leq g (b) - g (a) + h (b) - h (a). \end{array}
$$

Thus $M = g ( b ) - g ( a ) + h ( b ) - h ( a )$ is an upper bound independent of the choice of partition, and so ${ \cal T } _ { F } [ a , b ] \leq M < \infty$ , as required. □ 

This decomposition is minimal: if $F = F _ { 1 } - F _ { 2 }$ and $F _ { 1 } , F _ { 2 }$ are increasing, then for any partition $a = x _ { 0 } < x _ { 1 } \ldots < x _ { n } = b$ we can write, for fixed $i \leq n$ 

$$
\begin{array}{l} \{F (x _ {i}) - F (x _ {i - 1}) \} ^ {+} - \{F (x _ {i}) - F (x _ {i - 1}) \} ^ {-} = F (x _ {i}) - F (x _ {i - 1}) \\ = \{F _ {1} (x _ {i}) - F _ {1} (x _ {i - 1}) \} - \{F _ {2} (x _ {i}) - F _ {2} (x _ {i - 1}) \} \end{array}
$$

which shows from the minimality property of $x = x ^ { + } - x ^ { - }$ that each term in the diference on the right dominates its counterpart of the left. Adding and taking suprema we conclude that $P _ { F }$ is dominated by the total variation of $F _ { 1 }$ and $N _ { F }$ by that of $F _ { 2 }$ . In other words, in the collection of increasing functions whose diference is $F _ { ; }$ , the functions $( F ( a ) + P _ { F } )$ and $N _ { F }$ have the smallest sum at every point of [a, b]. 

## Exercise 7.13

(a) Let $F$ be monotone increasing on $[ a , b ]$ . Find $T _ { F } [ a , b ]$ 

(b) Prove that if $F ~ \in ~ B V [ a , b ]$ then F is continuous a.e. (m) and Lebesgue-measurable. 

(c) Find a diferentiable function which is not in $B V [ 0 , 1 ]$ 

(d) Show that if there is a (Lipschitz) constant $M > 0$ such that $| F ( x ) -$ $F ( y ) | \leq M | x - y |$ for all $x , y \in [ a , b ]$ , then $F \in B V [ a , b ]$ 

The following simple facts link bounded variation and absolute continuity for functions on a bounded interval $[ a , b ]$ 

## Proposition 7.17

Suppose the real function F is absolutely continuous on $[ a , b ]$ ; then we have: 

(i) $F \in B V [ a , b ] .$ 

(ii) If $F = F _ { 1 } - F _ { 2 }$ is the minimal decomposition of F as the diference of two monotone increasing functions described in Theorem 7.16, then both $F _ { 1 }$ and $F _ { 2 }$ are absolutely continuous on $[ a , b ]$ 

Hint Given $\varepsilon > 0$ choose $\delta > 0$ as in Definition 7.5. In (i), starting with an arbitrary partition $( x _ { i } )$ of $[ a , b ]$ we cannot use the absolute continuity of $F$ unless we know that the subintervals are of length δ. So add enough new partition points to guarantee this and consider the sums they generate. For (ii), compare the various variation functions when summing over a partition where the sum of intervals lengths is bounded by $\delta .$ 

## Definition 7.7

If $F \in B V [ a , b ]$ , where $a , b \in \mathbb { R }$ , let $F = F _ { 1 } - F _ { 2 }$ be its minimal decomposition into monotone increasing functions. Define the Lebesgue–Stieltjes signed measure of $F$ as the countably additive set function $m _ { F }$ given on the σ-field  of Borel sets by $\ i _ { F } = m _ { F _ { 1 } } - m _ { F _ { 2 } }$ , where $m _ { F _ { i } }$ is the Lebesgue–Stieltjes measure of $F _ { i } , ( i = 1 , 2 )$ 

We shall examine signed measures more generally in the next section. For the present, we note the following 

## Example 7.4

When considering the measure $\textstyle P _ { X } ( E ) = \int _ { E } f _ { X }$ dm induced on R by a density $f _ { X }$ we restrict attention to $f _ { X } \geq 0$ Rto ensure that $P _ { X }$ is non-negative. But for a measurable function $f : \mathbb { R } \longrightarrow \mathbb { R }$ we set (Definition 4.4) 

$$
\int_ {E} f \mathrm{d} m = \int_ {E} f ^ {+} \mathrm{d} m - \int_ {E} f ^ {-} \mathrm{d} m \text {whenever} \int_ {E} | f | \mathrm{d} m <   \infty .
$$

The set function ν defined by $\begin{array} { r } { \nu ( E ) = \int _ { E } j } \end{array}$ f dm then splits naturally into the diference of two measures, i.e. $\nu = \nu ^ { + } - \nu ^ { - }$ , where $\begin{array} { r } { \nu ^ { + } ( E ) = \int _ { E } f ^ { + } } \end{array}$ dm and $\textstyle \nu ^ { - } ( E ) = \int _ { E } f ^ { - }$ dm. Restricting to a function f supported on $[ a , b ]$ and setting $\textstyle F ( x ) \ = \ \int _ { a } ^ { x } f$ dm we obtain $m _ { F } = \nu ,$ and if $F = F _ { 1 } - F _ { 2 }$ as in the above Rdefinition, then $m _ { F 1 } = \nu ^ { + } , m _ { F 2 } = \nu ^ { - }$ by the minimality properties of the splitting of $F$ . 

## 7.3.4 Signed measures

The above example and the definition of Lebesgue–Stieltjes measures generated by a BV function motivate the following abstract definition and the subsequent search for a similar decomposition into the diference of two measures. We proceed to outline briefly the structure of signed measures in the abstract setting, which provides a general context for the above development of Stieltjes integrals and distribution functions. Our results will enable us to define integrals of functions relative to signed measures by reference to the decomposition of the signed measure into ‘positive and negative parts’, exactly as above. We also obtain a more general Lebesgue decomposition and Radon–Nikodym theorem, thus completing the description of the structure of a bounded signed measure relative to a given σ-finite measure. This leads to the general version of the Fundamental Theorem of the Calculus signalled earlier. 

## Definition 7.8

A signed measure on a measurable space $( \varOmega , \mathscr { F } )$ is a set function $\nu : \mathcal { F } \longrightarrow$ $( - \infty , + \infty ]$ satisfying 

(i) $\nu ( \ r { O } ) = 0$ 

$$
\text {(ii)} \nu (\bigcup_ {i = 1} ^ {\infty} E _ {i}) = \sum_ {i = 1} ^ {\infty} \nu (E _ {i}) \text {if} E _ {i} \in \mathcal {F} \text {and} E _ {i} \cap E _ {j} = \emptyset \text {for} i \neq j.
$$

We need to avoid ambiguities like $\infty { - } \infty$ by demanding that ν should take at most one of the values ; therefore we consistently demand that $\nu ( E ) > - \infty$ for all sets E in its domain. Note also that in (ii) either both sides are + , or they are both finite, so that the series converges in R. Since the left side is unafected by any re-arrangement of the terms of the series, it follows that the series converges absolutely whenever it converges, i.e. $\textstyle \sum _ { i = 1 } ^ { \infty } | \nu ( E _ { i } ) | < \infty$ if and only if $| \nu ( \bigcup _ { i = 1 } ^ { \infty } E _ { i } ) | < \infty$ P. The convergence is clear in the motivating example, Ssince for any $E \subseteq \mathbb { R }$ we have 

$$
| \nu (E) | = \left| \int_ {E} f \mathrm{d} m \right| \leq \int_ {E} | f | \mathrm{d} m <   \infty \text {   when   } f \in \mathcal {L} ^ {1} (\mathbb {R}).
$$

Note that ν is finitely additive (let $E _ { i } = \mathcal { O }$ for all $i > n$ in (ii), then (i) implies $\begin{array} { r } { \nu ( \bigcup _ { i = 1 } ^ { n } E _ { i } ) = \sum _ { i = 1 } ^ { n } \nu ( E _ { i } ) } \end{array}$ if $E _ { i } \in \mathcal { F }$ and $E _ { i } \cap E _ { j } = \emptyset$ for $i \neq j , i , j \leq n )$ SHence if $F \subseteq E , F \in { \mathcal { F } }$ , and $| \nu ( E ) | < \infty$ , then $| \nu ( F ) | < \infty$ , since both sides of $\nu ( E ) = \nu ( F ) + \nu ( E \setminus F )$ are finite and $\nu ( E \setminus F ) > - \infty$ by hypothesis. 

Signed measures do not inherit the properties of measures without change: as a negative result we have 

## Proposition 7.18

A signed measure ν defined on a σ-field $\mathcal { F }$ is monotone increasing $( F \subset E$ implies $\nu ( F ) \leq \nu ( E ) )$ if and only ν is a measure on $\mathcal { F }$ 

Hint Ø is a subset of every $E \in { \mathcal { F } } !$ 

On the other hand, a signed measure attains its bounds at some sets in $\mathcal { F }$ More precisely: given a signed measure ν on $( \varOmega , \mathscr { F } )$ one can find sets A and B in $\mathcal { F }$ such that $\nu ( A ) = \operatorname* { i n f } \{ \nu ( F ) : F \in { \mathcal { F } } \}$ and $\nu ( B ) = \operatorname* { s u p } \{ \nu ( F ) : F \in { \mathcal { F } } \}$ 

Rather than prove this result directly we shall deduce it from the Hahn– Jordan decomposition theorem. This basic result shows how the set A and its complement can be used to define two (positive) measures $\nu ^ { + } , \nu ^ { - }$ such that $\nu = \nu ^ { + } - \nu ^ { - }$ , with $\nu ^ { + } ( F ) = \nu ( F \cap A ^ { c } )$ and $\nu ^ { - } ( F ) = - \nu ( F \cap A )$ for all $F \in { \mathcal { F } }$ The decomposition is minimal: if $\nu = \lambda _ { 1 } - \lambda _ { 2 }$ where the $\lambda _ { i }$ are measures, then $\nu ^ { + } \leq \lambda _ { 1 }$ and $\nu ^ { - } \leq \lambda _ { 2 }$ 

Restricting attention to bounded signed measures (which sufices for applications to probability theory), we can derive this decomposition by applying the Radon–Nikodym theorem. (Our account is a special case of the treatment given in [10], Ch.6, for complex-valued set functions.) First, given a bounded signed measure $\nu : \mathcal { F } \longrightarrow \mathbb { R }$ , we seek the smallest (positive) measure $\mu$ that dominates $\nu ,$ i.e. satisfies $\mu ( E ) \geq | \nu ( E ) |$ for all $E \in { \mathcal { F } }$ . Defining 

$$
| \nu | (E) = \sup \left\{\sum_ {i = 1} ^ {\infty} | \nu \left(E _ {i}\right) |: \left\{E _ {i} \right\} \subset \mathcal {F}, E = \bigcup_ {i \geq 1} E _ {i}, E _ {i} \cap E _ {j} = \emptyset \text {   if   } i \neq j \right\}
$$

produces a set function which satisfies $| \nu | ( E ) \geq | \nu ( E ) |$ for every E. The requirement $\mu ( E _ { i } ) \geq | \nu ( E _ { i } ) |$ for all i then yields 

$$
\mu (E) = \sum_ {i = 1} ^ {\infty} \mu (E _ {i}) \geq \sum_ {i = 1} ^ {\infty} | \nu (E _ {i}) |
$$

for any measure $\mu$ dominating ν. Hence to prove that $| \nu |$ has the desired properties we only need to show that it is countably additive. We call $| \nu |$ the total variation of $\nu .$ Note that we use countable partitions of $\varOmega$ here, just as we used sequences of intervals when defining Lebesgue measure in R. 

## Theorem 7.19

The total variation $| \nu |$ of a bounded signed measure is a (positive) measure on ${ \mathcal F } .$ 

## Proof

Partitioning $E \in { \mathcal { F } }$ into sets $\{ E _ { i } \}$ , choose $( a _ { i } )$ in $\mathbb { R } ^ { + }$ such that $a _ { i } < | \nu | ( E _ { i } )$ for all i. Partition each $E _ { i }$ in turn into sets $\{ A _ { i j } \} _ { j }$ , and by definition of sup we can choose these to ensure that $\begin{array} { r } { a _ { i } < \sum _ { j } | \nu ( A _ { i j } ) | } \end{array}$ for every $i \geq 1$ . But the $\{ A _ { i j } \}$ also partition E, hence $\textstyle \sum _ { i } a _ { i } < \sum _ { i , j } | \nu ( A _ { i , j } ) | < | \nu | ( E )$ . Taking the supremum over all sequences $( a _ { i } )$ P Psatisfying these requirements ensures that $\begin{array} { r } { \sum _ { i } | \boldsymbol { \nu } | ( E _ { i } ) = \operatorname* { s u p } \sum _ { i } a _ { i } \leq | \boldsymbol { \nu } | ( E ) } \end{array}$ 

PFor the converse inequality consider any partition $\{ B _ { k } \}$ of E and note that for fixed k, $\{ B _ { k } \cap E _ { i } \} _ { i \geq 1 }$ partitions $B _ { k }$ , while for fixed i, $\{ B _ { k } \cap E _ { i } \} _ { k \ge 1 }$ partitions $E _ { i }$ . This means that 

$$
\sum_ {k \geq 1} | \nu (B _ {k}) | = \sum_ {k \geq 1} | \sum_ {i \geq 1} \nu (B _ {k} \cap E _ {i}) | \leq \sum_ {k \geq 1} \sum_ {i \geq 1} | \nu (B _ {k} \cap E _ {i}) |.
$$

Since the terms of the double series are all non-negative, we can exchange the order of summation, so that finally 

$$
\sum_ {k \geq 1} | \nu (B _ {k}) | \leq \sum_ {i \geq 1} \sum_ {k \geq 1} | \nu (B _ {k} \cap E _ {i}) | \leq \sum_ {i \geq 1} | \nu | (E _ {i}).
$$

But the partition $\{ B _ { k } \}$ of $E$ was arbitrary, so the estimate on the right alsodominates $| \nu | ( E )$ . This completes the proof that $| \nu |$ is a measure. 口

We now define the positive (resp. negative) variation of the signed measure $\nu$ by setting: 

$$
\nu^ {+} = \frac {1}{2} (| \nu | + \nu), \quad \nu^ {-} = \frac {1}{2} (| \nu | - \nu).
$$

Clearly both are positive measures on ${ \mathcal F } _ { : }$ , and we have 

$$
\nu = \nu^ {+} - \nu^ {-} \text { and } | \nu | = \nu^ {+} + \nu^ {-}.
$$

With these definitions we can immediately extend the Radon–Nikodym and Lebesgue decomposition theorems to the case where ν is a bounded signed measure (we keep the notation used in Section 7.3.2, so here $\mu$ remains positive!): 

## Theorem 7.20

Let $\mu$ be σ-finite (positive) measure and suppose that ν is a bounded signed measure. Then there is unique decomposition $\nu = \nu _ { a } + \nu _ { s }$ , into two signed measures, with $\nu _ { a } \ll \mu$ and $\nu _ { s } \perp \mu$ . Moreover, there is a unique (up to sets of µ-measure 0) $h \in \mathcal { L } ^ { 1 } ( \mu )$ such that $\textstyle \nu _ { a } ( F ) = \int _ { F }$ h dµ for all $F \in { \mathcal { F } }$ 

## Proof

Given $\nu = \nu ^ { + } - \nu ^ { - }$ we wish to apply the Lebesgue decomposition and Radon– Nikodym theorems to the pairs of finite measures $( \nu ^ { + } , \mu )$ and $( \nu ^ { - } , \mu )$ . First we need to check that for a signed measure $\lambda \ll \mu$ we also have $| \lambda | \ll \mu$ (for then clearly both $\lambda ^ { + } \ll \mu$ and $\lambda ^ { - } \ll \mu )$ . But if $\mu ( E ) = 0$ and $\{ F _ { i } \}$ partitions $E _ { i }$ then each $\mu ( F _ { i } ) = 0$ , hence $\lambda ( F _ { i } ) = 0$ , so that $\begin{array} { r } { \sum _ { i \geq 1 } \left. \lambda ( F _ { i } ) \right. = 0 } \end{array}$ . As this holds for each partition, $| \lambda ( E ) | = 0$ 

Similarly, if λ is concentrated on a set A, and $A \cap E = \emptyset$ , then for any partition $\{ F _ { i } \}$ of E we will have $\lambda ( F _ { i } ) = 0$ for every $i \geq 1$ . Thus $| \lambda | ( E ) = 0$ so λ is also concentrated on A. Hence if two signed measures are mutually singular, so are their total variation measures, and thus also their positive and negative variations. Applying the Lebesgue decomposition and Radon– Nikodym theorems to the measures $\nu ^ { + }$ and $\nu ^ { - }$ provides (positive) measures $( \nu ^ { + } ) _ { a } , ( \nu ^ { + } ) _ { s } , ( \nu ^ { - } ) _ { a } , ( \nu ^ { - } ) _ { s }$ such that $\nu ^ { + } = ( \nu ^ { + } ) _ { a } + ( \nu ^ { + } ) _ { s }$ , and $( \nu ^ { + } ) _ { a } ( F ) =$ $\begin{array} { r } { \int _ { F } h ^ { \prime } \mathrm { d } \mu ; } \end{array}$ while $\nu ^ { - } = ( \nu ^ { - } ) _ { a } + ( \nu ^ { - } ) _ { \mathrm { { : } } }$ <sub>s</sub> and $\begin{array} { r } { ( \nu ^ { - } ) _ { a } ( F ) = \int _ { F } h ^ { \prime \prime } \mathrm { d } \mu } \end{array}$ , for non-negative Rfunctions $h ^ { \prime } , h ^ { \prime \prime } \in \mathcal { L } ^ { 1 } ( \mu )$ , and with the measures $( \nu ^ { + } ) _ { s } , ( \nu ^ { - } ) _ { s }$ each mutually singular with $\mu .$ . Letting $\nu _ { a } = ( \nu ^ { + } ) _ { a } - ( \nu ^ { - } ) _ { a }$ we obtain a signed measure $\nu _ { a } \ll \mu$ 8 and a function $h = h ^ { \prime } - h ^ { \prime \prime } \in \mathcal { L } ^ { 1 } ( \mu )$ with $\textstyle \nu _ { a } ( F ) = \int _ { F } h \mathrm { d } \mu$ for all $F \in { \mathcal { F } }$ . The signed measure $\nu _ { s } = ( \nu ^ { + } ) _ { s } - ( \nu ^ { - } ) _ { s }$ R<sub>s</sub> is clearly singular to $\mu ,$ and h is unique up to $\mu { \mathrm { - } } \mathrm { n u l l }$ sets, since this holds for $h ^ { \prime } , h ^ { \prime \prime }$ and the decomposition $\nu = \nu ^ { + } - \nu ^ { - }$ is minimal. □ 

## Example 7.5

If $g \in L ^ { 1 } ( \mu )$ then $\textstyle \nu ( E ) = \int _ { E } g \mathrm { d } \mu$ is a signed measure and $\nu \ll \mu$ . The Radon– Nikodym theorem shows that (with our conventions) all signed measures $\nu \ll \mu$ have this form. 

We are nearly ready for the general form of the Fundamental Theorem of Calculus. First we confirm, as may be expected from the proof of the Radon– Nikodym theorem, the close relationship between the derivative of the bounded variation function F induced by a bounded signed (Borel) measure ν on R and the derivative $f = F ^ { \prime }$ 

## Theorem 7.21

If ν is a bounded signed measure on R and $F ( x ) = \nu ( ( - \infty , x ] )$ then for any $a \in \mathbb { R }$ , the following are equivalent: 

(i) F is diferentiable at a, and $F ^ { \prime } ( a ) = L$ 

(ii) given $\varepsilon > 0$ there exists $\delta > 0$ such that $\begin{array} { r } { | \frac { \nu ( J ) } { m ( J ) } - L | < \varepsilon } \end{array}$ if the open interval 

J contains a and $l ( J ) < \varepsilon$ 

## Proof

We may assume that $L = 0 ;$ otherwise consider $\rho = \nu - L m$ instead, restricted to a bounded interval containing a. If (i) holds with $L = 0$ and $\varepsilon > 0$ is given, we can find $\delta > 0$ such that 

$$
| F (y) - F (x) | <   \varepsilon | y - x | \text { whenever } | y - x | <   \delta .
$$

Let $J = ( x , y )$ be an open interval containing a with $\left( y - x \right) < \delta$ . For suficiently large N we can ensure that $\textstyle a > x + { \frac { 1 } { N } } > x$ and so for $\textstyle k \geq 1 , y _ { k } = x + { \frac { 1 } { N + k } }$ is bounded above by a and decreases to x as $k \to \infty$ . Thus 

$$
\begin{array}{c} | \nu (y _ {k}, y) | = | F (y) - F (y _ {k}) | \leq | F (y) - F (a) | + | F (a) - F (y _ {k}) | \\ \leq \varepsilon \{(y - a) + (a - y _ {k}) \} <   \varepsilon m (J). \end{array}
$$

But since $y _ { k } \to x , \nu ( y _ { k } , y ] \to \nu ( x , y ]$ and we have shown that $\begin{array} { r } { | \frac { \nu ( J ) } { m ( J ) } | < \varepsilon } \end{array}$ . Hence (ii) holds. For the converse, let $\varepsilon , \delta$ be as in (ii), so that with $x < a < y$ and $y - x < \delta \ \mathrm { ( i i ) }$ implies $\begin{array} { r } { | \nu ( x , y + \frac { 1 } { n } ) | < \varepsilon ( y + \frac { 1 } { n } - x ) } \end{array}$ for all large enough n. But as $\begin{array} { r } { ( x , y ] = \bigcap _ { n } ( x , y + \frac { 1 } { n } ) } \end{array}$ , we also have 

$$
| \nu (x, y) | <   | F (y) - F (x) | <   \varepsilon (y - x).\tag{7.3}
$$

Finally, since (ii) holds, $| \nu ( \{ a \} ) | \leq | \nu ( I ) | < \varepsilon l ( I )$ for any small enough open interval I containing a. Thus $F ( a ) = F ( a - )$ and so $F$ is continuous at a. Since $x < a < y < x + \delta ,$ we conclude that (7.3) holds with a instead of x, which shows that the right-hand derivative of F at a is 0, and with a instead of y which shows the same for the left-hand derivative. Thus $F ^ { \prime } ( a ) = 0$ , and so (i) holds. □ 

## Theorem 7.22 (Fundamental Theorem of Calculus)

Let F be absolutely continuous on $[ a , b ]$ . Then F is diferentiable $m { \mathrm { - a . e } }$ . and its Lebesgue–Stieltjes signed measure m<sub>F</sub> has Radon–Nikodym derivative $\begin{array} { r l r } {  { \frac { d m _ { F } } { d m } = } } \end{array}$ $F ^ { \prime } \ m { \mathrm { - a . e } }$ . Moreover, for each $x \in [ a , b ]$ 

$$
F (x) - F (a) = m _ {F} [ a, x ] = \int_ {a} ^ {x} F ^ {\prime} (t) \mathrm{d} t.
$$

## Proof

The Radon–Nikodym theorem provides $\begin{array} { r } { \frac { d m _ { F } } { d m } = h \in \mathcal { L } ^ { 1 } ( m ) } \end{array}$ such that $m _ { F } ( E ) =$ $\textstyle \int _ { E } h$ dm for all $E \in B$ . Choosing the partitions 

$$
\mathcal {P} _ {n} = \left\{\left(t _ {i}, t _ {i + 1} \right]: t _ {i} = a + \frac {i}{2 ^ {n}} (b - a), i \leq 2 ^ {n} \right\}
$$

we obtain, successively, each $\mathcal { P } _ { n }$ as the smallest common refinement of the partitions $\mathcal { P } _ { 1 } , \mathcal { P } _ { 2 } , \ldots , \mathcal { P } _ { n - 1 }$ . Thus, setting $h _ { n } ( a ) = 0$ and 

$$
h _ {n} (x) = \sum_ {i = 1} ^ {2 ^ {n}} \frac {m _ {F} (t _ {i} , t _ {i + 1} ]}{m (t _ {i} , t _ {i + 1} ]} \mathbf {1} _ {(t _ {i}, t _ {i + 1} ]} = \sum_ {i = 1} ^ {2 ^ {n}} \frac {F (t _ {i + 1}) - F (t _ {i})}{t _ {i + 1} - t _ {i}} \mathbf {1} _ {(t _ {i}, t _ {i + 1} ]} \text { for } a <   x \leq b,
$$

we obtain a sequence $\left( h _ { n } \right)$ corresponding to the sequence $\left( h _ { \mathcal { Q } _ { n } } \right)$ constructed in Step 2 of the proof of the Radon–Nikodym theorem. It follows that $h _ { n } ( x ) $ $h ( x ) \ m { \cdot } { \mathrm { e } }$ . But for any fixed $x \in ( a , b )$ , condition (ii) in Theorem 4.2 applied to the function $F$ on each interval $\left( { { t } _ { i } } , { { t } _ { i + 1 } } \right)$ with length less than $\delta ,$ and with $L = h ( x )$ , shows that $h = F ^ { \prime } \ m { \mathrm { - a . e } }$ . The final claim is now obvious from the definitions. □ 

The following result is therefore immediate and it justifies the terminology ‘indefinite integral’ in this general setting. 

## Corollary 7.23

If F is absolutely continuous on $[ a , b ]$ and $F ^ { \prime } { = } 0 ~ { \mathrm { } m } { \mathrm { - } } { \mathrm { a . e } }$ . then $F$ is constant. 

A final corollary now completes the circle of ideas for distribution functions and their densities: 

## Corollary 7.24

If $f \in \mathcal { L } ^ { 1 } ( [ a , b ] )$ and $\textstyle F ( x ) = \int _ { a } ^ { x } f$ dm for each $x \in [ a , b ]$ then $F$ is diferentiable m-a.e. and $F ^ { \prime } ( x ) = f ( x )$ Rfor almost every $x \in [ a , b ]$ 

As a further application of the Radon–Nikodym theorem we derive the Hahn–Jordan decomposition of ν which was outlined earlier. First we need the following 

## Theorem 7.25

Let ν be a bounded signed measure and let $| \nu |$ be its total variation. Then we can find a measurable function h such that $| h ( \omega ) | = 1$ for all $\omega \in { \mathcal { Q } }$ and $\textstyle \nu ( E ) = \int _ { E } h \mathrm { d } | \nu |$ for all $E \in { \mathcal { F } }$ 

## Proof

The Radon–Nikodym theorem provides a measurable function h with $\nu ( E ) =$ $\textstyle \int _ { E } h \mathrm { d } | \nu |$ for all $E \in { \mathcal { F } }$ since every $\lvert \nu \rvert \mathrm { - n u l l }$ set is ν-null $( \{ E , \emptyset , \emptyset , \dots \}$ is a Rpartition of E). Let $C _ { \alpha } = \{ \omega : | h ( \omega ) | < \alpha \}$ for $\alpha > 0$ . Then, for any partition $\{ E _ { i } \}$ of $C _ { \alpha }$ , 

$$
\sum_ {i \geq 1} | \nu (E _ {i}) | = \sum_ {i \geq 1} \left| \int_ {E _ {i}} h d | \nu | \right| \leq \sum_ {i \geq 1} \alpha | \nu | (E _ {i}) = \alpha | \nu | (C _ {\alpha}).
$$

As this holds for any partition, it holds for their supremum, i.e. $| \nu | ( C _ { \alpha } ) ~ \leq$ $\alpha | \nu | ( C _ { \alpha } )$ . For $\alpha \ : < \ : 1$ we must conclude that $C _ { \alpha }$ is $\lvert \nu \rvert \mathrm { - n u l l }$ , and hence also ν-null. Therefore $| h | \geq 1 \ \nu { \mathrm { - a . e } }$ 

To show that $| h | \leq 1 \nu \mathrm { - a . e }$ . we note that if E has positive $\left| \nu \right| \mathrm { - m e a s u r e } .$ , then, by definition of $h$ , 

$$
\frac {\left| \int_ {E} h \mathrm{d} | \nu | \right|}{| \nu | (E)} = \frac {| \nu (E) |}{| \nu | (E)} \leq 1.
$$

That this implies $| h | \leq 1 \ \nu { \mathrm { - a . e } }$ . follows from the proposition below, applied with $\rho = | \nu |$ . Thus the set where $| h | \neq 1 { \mathrm { ~ i s ~ } } | \nu | { \mathrm { - n u l l } }$ , hence also ν-null, and we can redefine h there so that $| h ( \omega ) | = 1$ for all $\omega \in \varOmega$ □ 

## Proposition 7.26

Given a finite measure $\rho$ and a function $f \in { \mathcal { L } } ^ { 1 } ( \rho )$ , suppose that for every $E \in { \mathcal { F } }$ with $\rho ( E ) > 0$ we have $\begin{array} { r } { | \frac { 1 } { \rho ( E ) } \int _ { E } f \mathrm { d } \rho | \le 1 } \end{array}$ . Then $| f ( \omega ) | \leq 1 , \rho { \mathrm { - a . e } }$ 

Hint Let $E = \{ f > 1 \}$ . If $\rho ( E ) > 0$ consider $\begin{array} { r } { \int _ { E } \frac { f } { \rho ( E ) } \mathrm { d } \rho . } \end{array}$ 

We are ready to derive the Hahn–Jordan decomposition very simply: 

## Proposition 7.27

Let ν be a bounded signed measure. There are disjoint measurable sets A, B such that $A \cup B = \varOmega$ and $\nu ^ { + } ( F ) = \nu ( B \cap F ) , \nu ^ { - } ( F ) = \nu ( A \cap F )$ for all $F \in { \mathcal { F } }$ Consequently, if $\nu = \lambda _ { 1 } - \lambda _ { 2 }$ for measures $\lambda _ { 1 } , \lambda _ { 2 }$ then $\lambda _ { 1 } \geq \nu ^ { + }$ and $\lambda _ { 2 } \geq \nu ^ { - }$ 

Hint Since $\mathrm { d } \nu = h \mathrm { ~ d } | \nu |$ and $| h | = 1$ let $A = \{ h = - 1 \} , B = \{ h = 1 \}$ . Use the definition of $\nu ^ { + }$ to show that $\begin{array} { r } { \nu ^ { + } ( F ) = \frac { 1 } { 2 } \int _ { F } ( 1 + h ) \mathrm { d } | \nu | = \nu ( F \cap B ) } \end{array}$ for every $F .$ 

## Exercise 7.14

Let ν be a bounded signed measure. Show that for all $F , \nu ^ { + } ( F ) =$ $\operatorname* { s u p } _ { G \subset F } \nu ( G ) , \ \nu ^ { - } ( F ) \ = \ - \operatorname* { i n f } _ { G \subset F } \nu ( G )$ , all the sets concerned being members of ${ \mathcal F } .$ . 

$$
\mathbf {H i n t} \nu (G) \leq \nu^ {+} (G) \leq \nu (B \cap G) + \nu ((B \cap F) \backslash (B \cap G)) = \nu (B \cap F).
$$

## Exercise 7.15

Show that when $\textstyle \nu ( F ) = \int _ { F } f \mathrm { d } \mu$ where $f \in { \mathcal { L } } ^ { 1 } ( \mu )$ , where $\mu$ is a (positive) measure, the Hahn decomposition sets are $A = \{ f < 0 \}$ and $B = \{ f \geq$ $0 \}$ , and $\begin{array} { r } { \nu ^ { + } ( F ) = \int \displaylimits _ { F } f ^ { + } \mathrm { d } \nu , } \end{array}$ while $\textstyle \nu ^ { - } ( F ) = \int _ { F } f ^ { - } \mathrm { d } \nu$ 

We finally arrive at a general definition of integrals relative to signed measures: 

## Definition 7.9

Let $\mu$ be signed measure and f a measurable function on $F \in { \mathcal { F } }$ . Define the integral $\textstyle \int _ { F } f \mathrm { d } \mu$ by 

$$
\int_ {F} f \mathrm{d} \mu = \int_ {F} f \mathrm{d} \mu^ {+} - \int_ {F} f \mathrm{d} \mu^ {-}
$$

whenever both terms on the right are finite or are not of the form $\pm ( \infty - \infty )$ 

The function is sometimes called summable if the integral so defined is finite. Note that the earlier definition of a Lebesgue–Stieltjes signed measure fits into this general framework. We normally restrict attention to the case when both terms are finite, which clearly holds when $\mu$ is bounded. 

## Exercise 7.16

Verify the following: Let $\mu$ be a finite measure and define the signed measure ν by $\begin{array} { r } { \nu ( F ) = \int _ { F } g \mathrm { d } \mu } \end{array}$ . Prove that $f \in L ^ { 1 } ( \nu )$ if and only if $f g \in L ^ { 1 } ( \mu )$ and $\textstyle \int _ { E } f \mathrm { d } \nu = \int _ { E } f g \mathrm { d } \mu$ for all µ-measurable sets $E$ 

## 7.4 Probability

## 7.4.1 Conditional expectation relative to a σ-field

Suppose we are given a random variable $X \in \mathcal { L } ^ { 1 } ( P )$ , where $( \varOmega , \mathcal { F } , P )$ is a probability space. In Chapter 5 we defined the conditional expectation $\mathbb { E } ( X | \mathcal { G } )$ of $X \in L ^ { 2 } ( P )$ relative to a sub-σ-field  of $\mathcal { F }$ as the a.s. unique random variable $Y \in L ^ { 2 } ( { \mathcal { G } } )$ satisfying the condition 

$$
\int_ {G} Y \mathrm{d} P = \int_ {G} X \mathrm{d} P \text { for   all } G \in \mathcal {G}.\tag{7.4}
$$

The construction was a consequence of orthogonal projections in the Hilbert space $\mathcal { L } ^ { 2 }$ with the extension to all integrable random variables undertaken ‘by hand’, which required a little care. With the Radon–Nikodym theorem at our disposal we can verify the existence of conditional expectations for integrable random variables very simply: 

The (possibly signed) bounded measure $\textstyle \nu ( F ) = \int _ { F } X$ dP is absolutely continuous with respect to $P .$ R. Restricting both measures to $( \varOmega , \mathcal { G } )$ maintains this relationship, so that there is a -measurable, $P \mathrm { - a . s }$ . unique random variable Y such that $\textstyle \nu ( G ) = \int _ { G } Y \mathrm { d } P$ for every $G \in { \mathcal { G } }$ . But by definition $\textstyle \nu ( G ) = \int _ { G } X \mathrm { d } P$ 2 Rso the defining equation (7.4) of $Y = \mathbb { E } ( X | \mathcal { G } )$ has been verified. 

## Remark 7.2

In particular, this shows that for $X \in \mathcal { L } ^ { 2 } ( \mathcal { F } )$ its orthogonal projection onto ${ \mathcal { L } } ^ { 2 } ( { \mathcal { G } } )$ is a version of the Radon–Nikodym derivative of the measure $\nu : F $ $\textstyle \int _ { F } X \mathrm { d } P$ 

We shall write $\mathbb { E } ( X | \mathcal { G } )$ instead of Y from now on, always keeping in mind that we have freedom to choose a particular ‘version’, i.e. as long as the results we seek demand only that relations concerning $\mathbb { E } ( X | \mathcal { G } )$ hold $P \mathrm { - a . s . }$ , we can alter this random variable on a null set without afecting the truth of the defining equation: 

## Definition 7.10

A random variable $\mathbb { E } ( X | \mathcal { G } )$ is called the conditional expectation of X relative to a σ-field if 

(1) $\mathbb { E } ( X | \mathcal { G } )$ is -measurable, 

(2) $\begin{array} { r } { \int _ { G } \mathbb { E } ( X | \mathcal { G } ) \mathrm { d } P = \int _ { G } X } \end{array}$ dP for all $G \in { \mathcal { G } }$ 

We investigate the properties of the conditional expectation. To begin with, the simplest are left for the reader as a proposition. In this and the subsequent theorem we make the following assumptions: 

(i) All random variables concerned are defined on a probability space $( \varOmega , \mathcal { F } , P )$ ; 

(ii) X, Y and all $( X _ { n } )$ used below are assumed to be in $\mathcal { L } ^ { 1 } ( \varOmega , \mathcal { F } , P )$ ; 

(iii)  and  are sub-σ-fields of . 

The properties listed in the next proposition are basic, and are used time and again. Where appropriate we give verbal description of its ‘meaning’ in terms of information about X. 

## Proposition 7.28

The conditional expectation E(X ) has the following properties: 

(i) E $( \mathbb { E } ( X | { \mathcal { G } } ) ) = \mathbb { E } ( X )$ 

(more precisely: any version of the conditional expectation of X has the same expectation as X). 

(ii) If X is  -measurable, then $\mathbb { E } ( X | { \mathcal { G } } ) = X$ (if, given , we already ‘know’ X, our ‘best estimate’ of it is perfect). 

(iii) If X is independent of , then $\mathbb { E } ( X | { \mathcal { G } } ) = \mathbb { E } ( X )$ 

(if  ‘tells us nothing’ about X, our best guess of X is its average value). 

(iv) (Linearity) ${ \mathbb E } ( ( a X + b Y ) | { \mathcal G } ) = a { \mathbb E } ( X | { \mathcal G } ) + b { \mathbb E } ( Y | { \mathcal G } )$ for any real numbers a, b (note again that this is really says that each linear combination of versions of the right-hand-side is a version of the left-hand-side). 

## Theorem 7.29

The following properties hold for $\mathbb { E } ( X | \mathcal { G } )$ as defined above: 

(i) If $X \geq 0$ then $\mathbb { E } ( X | \mathcal { G } ) \geq 0 \ \mathrm { a . s . }$ (positivity). 

(ii) If $\{ X _ { n } \} _ { n \geq 1 }$ are non-negative and increase a.s. to X, then $\{ \mathbb { E } ( X _ { n } | \mathcal { G } ) \} _ { n \geq 1 }$ increase a.s. to E(X ) 

(‘monotone convergence’ of conditional expectations). 

(iii) If Y is -measurable and XY is integrable, then $\mathbb { E } ( X Y | \mathcal { G } ) = Y \mathbb { E } ( X | \mathcal { G } )$ 

(iv) If $\mathcal { H } \subset \mathcal { G }$ then $\mathbb { E } ( [ \mathbb { E } ( X | \mathcal { G } ) ] | \mathcal { H } ) = \mathbb { E } ( X | \mathcal { H } )$ (the tower property). 

(v) If $\varphi : \mathbb { R }  \mathbb { R }$ is a convex function and $\varphi ( X ) \in { \mathcal { L } } ^ { 1 } ( P )$ , then 

$$
\mathbb {E} (\varphi (X) | \mathcal {G}) \geq \varphi (\mathbb {E} (X | \mathcal {G})).
$$

(This is known as the conditional Jensen inequality $\mathrm { ~ - ~ a ~ }$ similar result holds for expectations. Recall that a real function $\varphi$ is convex on $( a , b )$ if for all $x , y \in ( a , b ) , \varphi ( p x + ( 1 - p ) y ) \leq p \varphi ( x ) + ( 1 - p ) \varphi ( y )$ ; the graph of $\varphi$ stays on or below the straight line joining $( x , \varphi ( x ) ) , ( y , \varphi ( y ) ) . )$ 

Proof 

(i) For each $k \geq 1$ the set $E _ { k } = \left\{ \mathbb { E } ( X | { \mathcal { G } } ) < - { \frac { 1 } { k } } \right\} \in { \mathcal { G } }$ , so that 

$$
\int_ {E _ {k}} X \mathrm{d} P = \int_ {E _ {k}} \mathbb {E} (X | \mathcal {G}) \mathrm{d} P.
$$

As $X \geq 0$ , the left-hand side is non-negative, while the right-hand-side is bounded above by $\begin{array} { r l } { \mathrm { - } \frac { 1 } { k } P ( E _ { k } ) } & { { } } \end{array}$ . This forces $P ( E _ { k } ) = 0$ for each $k .$ , hence also $\begin{array} { r } { P ( \mathbb { E } ( X | \mathcal { G } ) < 0 ) = P ( \dot { \bigcup _ { k } } E _ { k } ) = 0 } \end{array}$ . Thus $\mathbb { E } ( X | { \mathcal { G } } ) \geq 0 { \mathrm { ~ a . s } }$ 

(ii) For each n let $Y _ { n }$ be a version of $\mathbb { E } ( X _ { n } | \mathcal { G } ) . \mathrm { B y ~ ( i ) }$ and as in Section 5.4.3, the $( Y _ { n } )$ are non-negative and increase a.s. Letting $Y = \operatorname* { l i m } \operatorname* { s u p } _ { n } Y _ { n }$ provides a -measurable random variable such that the real sequence $( Y _ { n } ( \omega ) ) _ { n }$ converges to $Y ( \omega )$ for almost all $\omega .$ . Corollary 4.9 then shows that $\textstyle ( \int _ { G } Y _ { n } \mathrm { d } P ) _ { n \geq 1 }$ increases to $\textstyle \int _ { G } Y \mathrm { d } P . $ . But we have $\textstyle \int _ { G } Y _ { n } \mathrm { d } P = \int _ { G } X _ { n } \mathrm { d } P$ Rfor each $n ,$ and $( X _ { n } )$ Rincreases pointwise to $X$ R R. By the monotone convergence theorem it follows that $\textstyle ( \int _ { G } X _ { n } \mathrm { d } P ) _ { n \geq 1 }$ increases to $\textstyle \int _ { G } X \mathrm { d } P ,$ , so that $\textstyle \int _ { G } X \mathrm { d } P = \int _ { G } Y \mathrm { d } P .$ This shows Rthat $Y$ is a version of $\mathbb { E } ( X | \mathcal { G } )$ R Rand therefore proves our claim. 

(iii) We can restrict attention to $X \geq 0$ , since the general case follows from this by linearity. Now first consider the case of indicators: if $Y = \mathbf { 1 } _ { E }$ for some $E \in { \mathcal { G } }$ , we have, for all $G \in { \mathcal { G } }$ ， 

$$
\int_ {G} \mathbf {1} _ {E} \mathbb {E} (X | \mathcal {G}) \mathrm{d} P = \int_ {E \cap G} \mathbb {E} (X | \mathcal {G}) \mathrm{d} P = \int_ {E \cap G} X \mathrm{d} P = \int_ {G} \mathbf {1} _ {E} X \mathrm{d} P
$$

so that $\mathbf { 1 } _ { E } \mathbb { E } ( X | \mathcal { G } )$ satisfies the defining equation and hence is a version of the conditional expectation of the product $X Y .$ So ${ \mathfrak { T } } ( X Y | { \mathcal { G } } ) = Y { \mathbb { E } } ( X | { \mathcal { G } } )$ has been verified when $Y = \mathbf { 1 } _ { E }$ and $E \in { \mathcal { G } }$ . By the linearity property this extends to simple functions, and for arbitrary $Y ~ \geq ~ 0$ we now use (ii) and a sequence $( Y _ { n } )$ of simple functions increasing to $Y$ to deduce that, for non-negative $X$ $\mathbb { E } ( X Y _ { n } | \mathcal { G } ) = Y _ { n } \mathbb { E } ( X | \mathcal { G } )$ increases to $\mathbb { E } ( X Y | \mathcal { G } )$ on the one hand and to $Y \mathbb { E } ( X | \mathcal { G } )$ on the other. Thus if X and $Y$ are both non-negative we have verified (iii). Linearity allows us to extend this to general $Y = Y ^ { + } - Y ^ { - }$ 

(iv) We have $\textstyle \int _ { G } \mathbb { E } ( X | { \mathcal { G } } ) \mathrm { d } P = \int _ { G } X \mathrm { d } P$ for $G \in { \mathcal { G } }$ and $\begin{array} { r l } { \int _ { H } \mathbb { E } ( X | \mathcal { H } ) \mathrm { d } P = } \end{array}$ $\textstyle \int _ { H } X \mathrm { d } P$ for $H \in { \mathcal { H } } \subset { \mathcal { G } }$ R. Hence for $H \ \in \ \mathcal { H }$ we obtain $\begin{array} { r l } { \bar { \int _ { H } \mathbb { E } } ( X | \mathcal { G } ) \mathrm { d } P } & { = } \end{array}$ $\begin{array} { r } { \int _ { H } \mathbb { E } ( X | \mathcal { H } ) \mathrm { d } P . } \end{array}$ Thus $\mathbb { E } ( X | \mathcal { H } )$ satisfies the condition defining the conditional expectation of $\mathbb { E } ( X | \mathcal { G } )$ with respect to ${ \mathcal { H } } ,$ so that $\mathbb { E } [ \mathbb { E } ( X | { \mathcal { G } } ) | { \mathcal { H } } ] = \mathbb { E } ( X | { \mathcal { H } } )$ 

(v) A convex function can be written as the supremum of a sequence of afine functions, i.e. there are sequences $( a _ { n } ) , ( b _ { n } )$ of reals such that $\varphi ( x ) =$ $\operatorname* { s u p } _ { n } ( a _ { n } x + b _ { n } )$ for every $x \in \mathbb { R }$ . Fix n, then since $\varphi ( X ( \omega ) ) \geq a _ { n } X ( \omega ) + b _ { n }$ for all $\omega _ { \mathrm { { i } } }$ the positivity and linearity properties ensure that 

$$
\mathbb {E} (\varphi (X) | \mathcal {G}) (\omega) \geq \mathbb {E} ([ a _ {n} X + b _ {n} ] | \mathcal {G}) (\omega) = a _ {n} \mathbb {E} (X | \mathcal {G}) (\omega) + b _ {n}
$$

for all $\omega \in \varOmega \setminus A _ { n }$ where $P ( A _ { n } ) = 0$ . Since $\textstyle A = \bigcup _ { n } A _ { n }$ is also null, it follows that for all $n \geq 1 , \mathbb { E } ( \varphi ( X ) | \mathcal { G } ) ( \omega ) \geq a _ { n } \mathbb { E } ( X | \mathcal { G } ) ( \omega ) + b _ { n } \mathrm { ~ a . s ~ }$ . Hence the inequality also holds when we take the supremum on the right, so that $( \mathbb { E } ( \varphi ( X ) | \mathcal { G } ) ( \omega ) \geq$ $\varphi [ ( \mathbb { E } ( X | \mathcal { G } ) ( \omega ) ]$ a.s. This proves $\mathrm { ( v ) }$ □ 

An immediate consequence of $\mathrm { ( v ) }$ is that the $L ^ { P } \mathrm { - n o r m }$ of $\mathbb { E } ( X | \mathcal { G } )$ is bounded by that of X for $p \geq 1$ , since the function $\varphi ( x ) = | x | ^ { p }$ is then convex: we obtain 

$$
| \mathbb {E} (X | \mathcal {G}) | ^ {p} = \varphi (\mathbb {E} (X | \mathcal {G})) \leq \mathbb {E} (\varphi (X) | \mathcal {G}) = \mathbb {E} (| X | ^ {p} | \mathcal {G}) \text { a.s. }
$$

so that 

$$
\| \mathbb {E} (X | \mathcal {G}) \| _ {p} ^ {p} = \mathbb {E} (| \mathbb {E} (X | \mathcal {G}) | ^ {p}) \leq \mathbb {E} (\mathbb {E} (| X | ^ {p} | \mathcal {G})) = \mathbb {E} (| X | ^ {p}) = \| X \| _ {p} ^ {p},
$$

where the penultimate step applies property (1) to $| X | ^ { p }$ . Take $p ^ { t h }$ roots to have $\| \mathbb { E } ( X | { \mathcal { G } } ) \| _ { p } \leq \| X \| _ { p }$ 

## Exercise 7.17

Let $\varOmega = [ 0 , 1 ]$ with Lebesgue measure and let $X ( \omega ) = \omega$ . Find $\mathbb { E } ( X | \mathcal { G } )$ if (a) $\mathcal { G } = \left\{ [ 0 , \frac { 1 } { 2 } ] , ( \frac { 1 } { 2 } , 1 ] , [ 0 , 1 ] , \emptyset \right\}$ , (b) $\mathcal { G }$ is generated by the family of sets $\{ B \subset [ 0 , \frac { 1 } { 2 } ]$ , Borel . 

## 7.4.2 Martingales

Suppose we wish to model the behaviour of some physical phenomenon by a sequence $( X _ { n } )$ of random variables. The value $X _ { n } ( \omega )$ might be the outcome of the $n ^ { t h }$ toss of a ‘fair’ coin which is tossed 1000 times, with ‘Heads’ recorded as 1, ‘Tails’ as 0. Then $\begin{array} { r } { Y ( \omega ) = \sum _ { n = 1 } ^ { 1 0 0 0 } X _ { n } ( \omega ) } \end{array}$ would record the number of times Pthat the coin had landed ‘Heads’. Typically, we would perform this random experiment a large number of times before venturing to make statements about the probability of ‘Heads’ for this coin. We could average our results, i.e. seek to compute $\mathbb { E } ( Y )$ . But we might also be interested in guessing what the value of $X _ { n } ( \omega )$ might be after $k < n$ tosses have been performed, i.e. for a fixed $\omega \in \varOmega$ does knowing the values of $( X _ { i } ( \omega ) ) _ { i \leq k }$ give us any help in predicting the value of $X _ { n } ( \omega )$ for $n > k ?$ In an ‘idealised’ coin-tossing experiment it is assumed that it does not, that is, the successive tosses are assumed to be independent — a fact which often perplexes the beginner in probability theory. 

There are many situations where the $( X _ { n } )$ would represent outcomes where the past behaviour of the process being modelled can reasonably be taken to influence its future behaviour, e.g. if $X _ { n }$ records whether it rains on day $n .$ We seek a mathematical description of the way in which our knowledge of past behaviour of $( X _ { n } )$ can be codified. A natural idea is to use the σ-field $\mathcal { F } _ { k } = \sigma \{ X _ { i } : 0 \leq i \leq k \}$ generated by the sequence $( X _ { n } ) _ { n \geq 0 }$ as representing the knowledge gained from knowing the first k outcomes of our experiment. We call $( X _ { n } ) _ { n \geq 0 }$ a (discrete) stochastic process to emphasise that our focus is now on the ‘dynamics’ of the sequence of outcomes as it unfolds. We include a $0 ^ { t h }$ stage for notational convenience, so that there is a ‘starting point’ before the experiment begins, and then $\mathcal { F } _ { 0 }$ represents our knowledge before any outcome is observed. 

So the information available to us by ‘time’ k (i.e. after k outcomes have been recorded) about the ‘state of the world’ $\omega$ is given by the values $( X _ { i } ( \omega ) ) _ { 0 \leq i \leq k }$ and this is encapsulated in knowing which sets of $\mathcal { F } _ { k }$ contain the point $\omega$ . But we can postulate a sequence of σ-fields $( \mathcal { F } _ { n } ) _ { n \geq 0 }$ quite generally, without reference to any sequence of random variables. Again, our knowledge of any particular $\omega$ is then represented at stage $k \geq 1$ by knowing which sets in $\mathcal { F } _ { k }$ contain $\omega .$ . A simple example is provided by the binomial stock price model of Section 2.6.3 (see Exercise 2.13). Guided by this example, we turn this into a general 

## Definition 7.11

Given a probability space $( \varOmega , \mathcal { F } , P )$ a (discrete) filtration is an increasing sequence of sub-σ-fields $( \mathcal { F } _ { n } ) _ { n \geq 0 }$ of ${ \mathcal { F } } ;$ i.e. 

$$
\mathcal {F} _ {0} \subset \mathcal {F} _ {1} \subset \mathcal {F} _ {2} \subset \ldots \subset \mathcal {F} _ {n} \subset \ldots \subset \mathcal {F}.
$$

We write $\mathbb { F } = ( \mathcal { F } _ { n } ) _ { n \geq 0 }$ . We say that the sequence $( X _ { n } ) _ { n \geq 0 }$ of random variables is adapted to the filtration F if $X _ { n }$ is ${ \mathcal { F } } _ { n }$ -measurable for every $n \geq 0$ . The tuple $( \varOmega , \mathcal F , ( \mathcal F _ { n } ) _ { n \geq 0 } , P )$ is called a filtered probability space. 

We shall normally assume in our applications that $\mathcal { F } _ { 0 } = \{ \emptyset , \emptyset \}$ , so that we begin with ‘no information’, and very often we shall assume that the ‘final σ-field generated by the whole sequence, i.e. $\mathcal { F } _ { \infty } = \sigma ( \cup _ { n \geq 0 } \mathcal { F } _ { n } )$ , is all of $\mathcal { F }$ (so that, by the end of the experiment, ‘we know all there is to know’). Clearly $( X _ { n } )$ is adapted to its natural filtration $( \mathcal F _ { n } ) _ { n }$ , where $\mathcal { F } _ { n } = \sigma ( X _ { i } : 0 \leq i \leq n \}$ for each $n _ { : }$ , and it is adapted to every filtration which contains this one. But equally, if $\mathcal { F } _ { n } = \sigma ( X _ { i } : 0 \leq i \leq n \}$ for some process $( X _ { n } ) _ { n }$ , it may be that some for other process $( Y _ { n } ) _ { n }$ , each $Y _ { n }$ is $\mathcal { F } _ { n } { \mathrm { - m e a s u r a b l e } } .$ , i.e. $( Y _ { n } ) _ { n }$ is adapted to $( \mathcal F _ { n } ) _ { n }$ . Recall that by Proposition 3.12 this implies that for each $n \geq 1$ there is a Borel-measurable function $f _ { n } : \mathbb { R } ^ { n + 1 }  \mathbb { R }$ such that $Y _ { n } = f ( X _ { 0 } , X _ { 1 } , X _ { 2 } , . . , X _ { n } )$ 

We come to the main concept introduced in this section: 

## Definition 7.12

Let $( \varOmega , \mathcal F , ( \mathcal F _ { n } ) _ { n \geq 0 } , P )$ be a filtered probability space. A sequence of random variables $( X _ { n } ) _ { n \geq 0 }$ on $( \varOmega , \mathcal { F } , P )$ is a martingale relative to the filtration $\mathbb { F } =$ $( \mathcal { F } _ { n } ) _ { n \geq 0 }$ provided: 

(i) $( X _ { n } ) _ { n }$ is adapted to $\mathbb { F } { : }$ 

(ii) each $X _ { n }$ is in $\mathcal { L } ^ { 1 } ( \boldsymbol { P } )$ 

(iii) for each $n \geq 0 , \mathbb { E } ( X _ { n + 1 } | \mathcal { F } _ { n } ) = X _ { n }$ 

We note two immediate consequences of this definition which are used over and over again: 

1) If $m > n \geq 0$ then $\mathbb { E } ( X _ { m } | \mathcal { F } _ { n } ) = X _ { n }$ . This follows from the tower property of conditional expectations, since (a.s.) 

$$
\mathbb {E} (X _ {m} | \mathcal {F} _ {n}) = \mathbb {E} (\mathbb {E} (X _ {m} | \mathcal {F} _ {m - 1}) | \mathcal {F} _ {n}) = \mathbb {E} (X _ {m - 1} | \mathcal {F} _ {n}) = \dots = \mathbb {E} (X _ {n + 1} | \mathcal {F} _ {n}) = X _ {n}.
$$

2) Any martingale $( X _ { n } )$ has constant expectation: 

$$
\mathbb {E} (X _ {n}) = \mathbb {E} (\mathbb {E} (X _ {n} | \mathcal {F} _ {0})) = \mathbb {E} (X _ {0})
$$

holds for every $n \geq 0$ , by 1) and (i) in Proposition 7.28. 

A martingale represents a ‘fair game’ in gambling: betting, for example, on the outcome of the coin tosses, our winnings in ‘game $n ^ { \prime }$ (the outcome of the $n ^ { t h }$ toss) would be $\varDelta X _ { n } = X _ { n } - X _ { n - 1 }$ , that is the diference between what we had before and after that game. (We assume that $X _ { 0 } = 0 . )$ If the games are fair we would predict at time $( n - 1 )$ , before the $n ^ { t h }$ outcome is known, that $\mathbb { E } ( \varDelta X _ { n } | \mathcal { F } _ { n - 1 } ) = 0$ , where ${ \mathcal { F } } _ { k } = \sigma \{ X _ { i } : i \leq k \}$ are the $\sigma { \mathrm { - f i e l d s } }$ of the natural filtration of the process $( X _ { n } )$ . This follows because our knowledge at time $( n - 1 )$ is encapsulated in $\mathcal { F } _ { n - 1 }$ and in a fair game we would expect our incremental winnings at any stage to be 0 on average. Hence in this situation the $( X _ { n } )$ form a martingale. 

Similarly, in a game favourable to the gambler we should expect that $\mathbb { E } ( \varDelta X _ { n } | \mathcal F _ { n - 1 } ) \geq 0$ , i.e. $\mathbb { E } ( X _ { n } | \mathcal { F } _ { n - 1 } ) \ \geq \ X _ { n - 1 }$ a.s. We call a sequence satisfying this inequality (and (i), (ii) of Definition 7.12) a submartingale, while a game unfavourable to the gambler (hence favourable to the casino!) is represented similarly by a supermartingale, which has E $( X _ { n } | { \mathcal { F } } _ { n - 1 } ) \leq X _ { n - 1 } { \mathrm { ~ a . s } }$ . for every n. Note that for a submartingale the expectations of the $( X _ { n } )$ increase with $n ,$ while for a supermartingale they decrease. Finally, note that the properties of these processes do not change if we replace $X _ { n }$ by $X _ { n } - X _ { 0 }$ (as long as $X _ { 0 } \in \mathcal { L } ^ { 1 } ( \mathcal { F } _ { 0 } )$ , to retain integrability and adaptedness) so that we can work without loss of generality with processes that start with $X _ { 0 } = 0$ 

## Example 7.6

The most obvious, yet in some ways quite general, example of a martingale consists of a sequence of conditional expectations: given a random variable $X \in \mathcal { L } ^ { 1 } ( \mathcal { F } )$ and a filtration $( \mathcal { F } _ { n } ) _ { n \geq 0 }$ of sub-σ-fields of ${ \mathcal F } .$ , let $X _ { n } = \operatorname { \mathbb { E } } ( X | { \mathcal { F } } _ { n } )$ for every n. Then $\mathbb { E } ( X _ { n + 1 } | \mathcal { F } _ { n } ) = \mathbb { E } ( \mathbb { E } ( X | \mathcal { F } _ { n + 1 } ) | \mathcal { F } _ { n } ) = \mathbb { E } ( X | \mathcal { F } _ { n } ) = X _ { n }$ , using the tower property again. We can interpret this by regarding each $X _ { n }$ as giving us the information available at time n, i.e. contained in the σ-field ${ \mathcal { F } } _ { n }$ , about the random variable X. (Remember that the conditional expectation is the ‘best guess’ of $X$ , with respect to mean-square errors, when we work in ${ \mathcal { L } } ^ { 2 } . )$ For a finite filtration $\lbrace \mathcal { F } _ { n } : 0 \leq n \leq N \rbrace$ with $\mathcal { F } _ { N } ~ = ~ \mathcal { F }$ it is obvious that $\mathbb { E } ( X | \mathcal { F } _ { N } ) = X$ . For an infinite sequence we might hope similarly that ‘in the limit’ we will have $\mathrm { \Phi _ { f u l l } } ,$ information about X, which suggests that we should be able to retrieve X as the limit of the $( X _ { n } )$ in some sense. The conditions under which limits exist require careful study — see e.g. [12], [8] for details. 

A second standard example of a martingale is: 

## Example 7.7

Suppose $( Z _ { n } ) _ { n \geq 1 }$ is a sequence of independent random variables with zero mean. Let $X _ { 0 } = 0 , \mathcal { F } _ { 0 } = \{ \emptyset , \Omega \}$ , set $\begin{array} { r } { X _ { n } = \sum _ { k = 1 } ^ { n } Z _ { k } } \end{array}$ and define $\mathcal { F } _ { n } = \sigma \{ Z _ { k }$ : $k \leq n \}$ for each $n \geq 1$ . Then $( X _ { n } ) _ { n \geq 0 }$ Pis a martingale relative to the filtration $\left( \mathcal { F } _ { n } \right)$ . To see this recall that for each $n , Z _ { n }$ is independent of $\mathcal { F } _ { n - 1 }$ , so that $\mathbb { E } ( Z _ { n } | \mathcal { F } _ { n - 1 } ) = \mathbb { E } ( Z _ { n } ) = 0$ . Hence $\begin{array} { r } { \mathbb { E } ( X _ { n } | \mathcal { F } _ { n - 1 } ) = \mathbb { E } ( X _ { n - 1 } | \mathcal { F } _ { n - 1 } ) + \mathbb { E } ( Z _ { n } ) = } \end{array}$ $X _ { n - 1 }$ , since $X _ { n - 1 }$ is $\mathcal { F } _ { n - 1 } { \mathrm { - m e a s u r a b l e } } .$ (You should check carefully which properties of the conditional expectation we used here!) 

A ‘multiplicative’ version of this example is the following: 

Exercise 7.18 

Let $Z _ { n } \geq 0$ be a sequence of independent random variables with $\mathbb { E } ( Z _ { n } ) =$ $\mu = 1$ Let ${ \mathcal { F } } _ { n } = \sigma \{ Z _ { k } : k \leq n \}$ and show that, $X _ { 0 } = 1 , X _ { n } = Z _ { 1 } Z _ { 2 } \ldots Z _ { n }$ $( n \geq 1 )$ defines a martingale for $\left( \mathcal { F } _ { n } \right)$ , provided all the products are integrable random variables, which holds, e.g., if all $Z _ { n } \in \mathcal { L } ^ { \infty } ( \varOmega , \mathcal { F } , P )$ 

## Exercise 7.19

Let $( Z _ { n } ) _ { n \geq 1 }$ be a sequence of independent random variables with mean $\mu = \mathbb { E } ( Z _ { n } ) \neq 0$ for all n. Show that the sequence of their partial sums $X _ { n } = Z _ { 1 } + Z _ { 2 } + \cdot \cdot \cdot + Z _ { n } $ is not a martingale for the filtration $( \mathcal F _ { n } ) _ { n }$ 2 where ${ \mathcal { F } } _ { n } = \sigma \{ Z _ { k } : k \leq n \}$ . How can we ‘compensate’ for this by altering $X _ { n } !$ 

Let $X \ = \ ( X _ { n } ) _ { n \geq 0 }$ be a martingale for the filtration $\mathbb { F } = ( \mathscr { F } _ { n } ) _ { n \geq 0 }$ (with our above conventions); briefly we simply refer to the martingale $( X , \mathbb { F } )$ . The function $\phi ( x ) \ : = \ : x ^ { 2 }$ is convex, hence by Jensen’s inequality (Theorem 7.29) we have $\begin{array} { r } { \mathbb { E } ( X _ { n + 1 } ^ { 2 } | \mathcal { F } _ { n } ) \ge ( \mathbb { E } ( X _ { n + 1 } | \mathcal { F } _ { n } ) ) ^ { 2 } = X _ { n } ^ { 2 } } \end{array}$ , so $X ^ { 2 }$ is a submartingale. We investigate whether it is possible to ‘compensate’, as in Exercise 7.19, to make the resulting process again a martingale. Note that the expectations of the $X _ { n } ^ { 2 }$ are increasing, so we will need to subtract an increasing process from $X ^ { 2 }$ to achieve this. 

In fact, the construction of this ‘compensator’ process is quite general. Let $Y = \left( Y _ { n } \right)$ be any adapted process with each $Y _ { n } \in { \mathcal { L } } ^ { 1 }$ . For any process Z write its increments as $\varDelta Z _ { n } = Z _ { n } - Z _ { n - 1 }$ for all n. Recall that in this notation the martingale property can be expressed succinctly as $\mathbb { E } ( \varDelta Z _ { n } | \mathcal F _ { n - 1 } ) = 0 \textrm { -- }$ we shall use repeatedly in what follows. 

We define two new processes $A = \left( A _ { n } \right)$ and $M = \left( M _ { n } \right)$ with $A _ { 0 } = 0 , M _ { 0 } = 0$ via their successive increments 

$$
\Delta A _ {n} = \mathbb {E} (\Delta Y _ {n} | \mathcal {F} _ {n - 1}) \text {   and   } \Delta M _ {n} = \Delta Y _ {n} - \Delta A _ {n} \text {   for   } n \geq 1.
$$

We obtain $\mathbb { E } ( \varDelta M _ { n } | \mathcal F _ { n - 1 } ) = \mathbb { E } ( [ \varDelta Y _ { n } - \mathbb { E } ( \varDelta Y _ { n } | \mathcal F _ { n - 1 } ) ] | \mathcal F _ { n - 1 } ) = \mathbb { E } ( \varDelta Y _ { n } | \mathcal F _ { n - 1 } ) -$ $\mathbb { E } ( \varDelta Y _ { n } | \mathcal { F } _ { n - 1 } ) = 0$ , as $\mathbb { E } ( \varDelta Y _ { n } | \mathcal { F } _ { n - 1 } )$ is $\mathcal { F } _ { n - 1 } { \mathrm { - m e a s u r a b l e } }$ . Hence M is a martingale. Moreover, the process A is increasing if and only if $0 ~ \leq ~ \varDelta A _ { n } ~ =$ $\mathbb { E } ( \varDelta Y _ { n } | \mathcal F _ { n - 1 } ) = \mathbb { E } ( Y _ { n } | \mathcal F _ { n - 1 } ) - Y _ { n - 1 }$ , which holds if and only if Y is a submartingale. Note that $\begin{array} { r } { A _ { n } = \sum _ { k = 1 } ^ { n } \varDelta A _ { k } = \sum _ { k = 1 } ^ { n } [ \mathbb { E } ( Y _ { k } | \mathcal { F } _ { k - 1 } ) - Y _ { k - 1 } ] } \end{array}$ is $\mathcal { F } _ { n - 1 ^ { - } }$ Pmeasurable. Thus the value of $A _ { n }$ Pis ‘known’ by time $n - 1$ . A process with this property is called predictable, since we can ‘predict’ its future values one step ahead. It is a fundamental property of martingales that they are not predictable: in fact, if X is a predictable martingale, then we have 

$$
X _ {n - 1} = \mathbb {E} (X _ {n} | \mathcal {F} _ {n - 1}) = X _ {n} \text { a.s.   for   every } n
$$

where the first equality is the definition of martingale, while the second follows since $X _ { n }$ is $\mathcal { F } _ { n - 1 }$ -measurable. Hence a predictable martingale is a.s. constant, and if it starts at 0 it will stay there. This fact gives the decomposition of an adapted process Y into the sum of a martingale and a predictable process a useful uniqueness property: first, since $M _ { 0 } = 0 = A _ { 0 }$ , we have $Y _ { n } = Y _ { 0 } + M _ { n } +$ $A _ { n }$ for the processes M, A defined above. If also $Y _ { n } = Y _ { 0 } + M _ { n } ^ { \prime } + A _ { n } ^ { \prime }$ , where $M _ { n } ^ { \prime }$ is a martingale, and $A _ { n } ^ { \prime }$ is predictable, then 

$$
M _ {n} - M _ {n} ^ {\prime} = A _ {n} ^ {\prime} - A _ {n} \mathrm{a.s.}
$$

is a predictable martingale, 0 at time 0. Hence both sides are 0 for every n and so the decomposition is a.s. unique. 

We call this the Doob decomposition of an adapted process. It takes on special importance when applied to the submartingale $Y = X ^ { 2 }$ which arises from a martingale X. In that case, as we saw above, the predictable process A is increasing, so that $A _ { n } \leq A _ { n + 1 }$ a.s. for every n, and the Doob decomposition reads: 

$$
X ^ {2} = X _ {0} ^ {2} + M + A
$$

In particular, if $X _ { 0 } = 0$ (as we can assume without loss of generality), we have written $X ^ { 2 } = M + A$ as the sum of a martingale M and a predictable increasing process A. The significance of this is revealed in a very useful property of martingales, which was a key component of the proof of the Radon–Nikodym theorem (see Step 1 (iv) of Theorem 7.3, where the martingale connection is well hidden!): for any martingale X we can write, with $( \varDelta X _ { n } ) ^ { 2 } = ( X _ { n } - X _ { n - 1 } ) ^ { 2 }$ 

$$
\begin{array}{r l} & {\mathbb {E} (\varDelta X _ {n}) ^ {2} | \mathcal {F} _ {n - 1}) = \mathbb {E} ([ X _ {n} ^ {2} - 2 X _ {n} X _ {n - 1} + X _ {n - 1} ^ {2} ] | \mathcal {F} _ {n - 1})} \\ & {\qquad = \mathbb {E} (X _ {n} ^ {2} | \mathcal {F} _ {n - 1}) - 2 X _ {n - 1} \mathbb {E} (\varDelta X _ {n} | \mathcal {F} _ {n - 1}) - X _ {n - 1} ^ {2}} \\ & {\qquad = \mathbb {E} ([ X _ {n} ^ {2} - X _ {n - 1} ^ {2} ] | \mathcal {F} _ {n - 1}).} \end{array}
$$

Hence given the martingale X with $X _ { 0 } = 0$ , the decomposition $X ^ { 2 } = M + A$ yields, since M is also a martingale: 

$$
\begin{array}{r} 0 = \mathbb {E} (\varDelta M _ {n} | \mathcal {F} _ {n - 1}) = \mathbb {E} ((\varDelta X _ {n}) ^ {2} - \varDelta A _ {n}) | \mathcal {F} _ {n - 1}) \\ = \mathbb {E} ([ X _ {n} ^ {2} - X _ {n - 1} ^ {2} ] | \mathcal {F} _ {n - 1}) - \mathbb {E} (\varDelta A _ {n} | \mathcal {F} _ {n - 1}). \end{array}
$$

In other words, since A is predictable, 

$$
\mathbb {E} ((\Delta X _ {n}) ^ {2} | \mathcal {F} _ {n - 1}) = \mathbb {E} (\Delta A _ {n} | \mathcal {F} _ {n - 1}) = \Delta A _ {n}\tag{7.5}
$$

which exhibits the process A as a conditional ‘quadratic variation’ process of the original martingale X. Taking expectations: E $( ( \varDelta X _ { n } ) ^ { 2 } ) = \mathbb { E } ( \varDelta A _ { n } )$ 

## Example 7.8

Note also that $\mathbb { E } ( X _ { n } ^ { 2 } ) = \mathbb { E } ( M _ { n } ) + \mathbb { E } ( A _ { n } ) = \mathbb { E } ( A _ { n } )$ (why?), so that both sides are bounded for all n if and only if the martingale X is bounded as a sequence in $\mathcal { L } ^ { 2 } ( \varOmega , \mathcal { F } , P )$ . Since $\left( A _ { n } \right)$ is increasing, the a.s. limit $\begin{array} { r } { A _ { \infty } ( \omega ) = \operatorname* { l i m } _ { n \to \infty } A _ { n } ( \omega ) } \end{array}$ exists, and the boundedness of the integrals ensures in that case that $\mathbb { E } ( A _ { \infty } ) <$ . 

## Exercise 7.20

Suppose $( Z _ { n } ) _ { n \geq 1 }$ is a sequence of Bernoulli random variables, with each $Z _ { n }$ taking the values 1 and 1, each with probability $\textstyle { \frac { 1 } { 2 } }$ . Let $X _ { 0 } = 0$ $X _ { n } = Z _ { 1 } + Z _ { 2 } + \cdot \cdot \cdot + Z _ { n } $ , and let $( \mathcal F _ { n } ) _ { n }$ be the natural filtration generated by the $\left( Z _ { n } \right)$ . Verify that $( X _ { n } ^ { 2 } )$ is a submartingale, and find the increasing process $\left( A _ { n } \right)$ in its Doob decomposition. What ‘unexpected’ property of $\left( A _ { n } \right)$ can you detect in this example? 

In the discrete setting we now have the tools to construct ‘stochastic integrals’ and show that they preserve the martingale property. In fact, as we saw for Lebesgue–Stieltjes measures, for discrete distributions the ‘integral is simply an appropriate linear combination of increments of the distribution function. If we wish to use a martingale X as an integrator, we therefore need to deal with linear combinations of the increments $\varDelta X _ { n } = X _ { n } - X _ { n - 1 }$ . Since we are now dealing with stochastic processes (that it, functions of both n and ω) rather than real functions, measurability conditions will help determine what constitutes an ‘appropriate’ linear combination. So, if for $\omega \in { \mathcal { Q } }$ we set $I _ { 0 } ( \omega ) = 0$ and form sums 

$$
I _ {n} (\omega) = \sum_ {k = 1} ^ {n} c _ {k} (\omega) (\Delta X _ {k}) (\omega) = \sum_ {k = 1} ^ {n} c _ {k} (\omega) (X _ {k} (\omega) - X _ {k - 1} (\omega)) \text { for } n \geq 1,
$$

we look for measurability properties of the process $( c _ { n } ) _ { n }$ which ensure that the new process $( I _ { n } ) _ { n }$ has useful properties. We investigate this when $( c _ { n } ) _ { n }$ is a bounded predictable process and X is a martingale for a given filtration $( \mathcal F _ { n } ) _ { n }$ Some texts call the process $( I _ { n } ) _ { n }$ a martingale transform — we prefer the term discrete stochastic integral. We calculate the conditional expectation of $I _ { n }$ : 

$$
\mathbb {E} (I _ {n} | \mathcal {F} _ {n - 1}) = \mathbb {E} ([ I _ {n - 1} + c _ {n} \varDelta X _ {n} ] | \mathcal {F} _ {n - 1}) = I _ {n - 1} + c _ {n} \mathbb {E} (\varDelta X _ {n} | \mathcal {F} _ {n - 1}) = I _ {n - 1},
$$

since $c _ { n }$ is $\mathcal { F } _ { n - 1 } { \mathrm { - m e a s u r a b l e } }$ and $\mathbb { E } ( \varDelta X _ { n } \vert \mathcal F _ { n - 1 } ) = \mathbb { E } ( X _ { n } \vert \mathcal F _ { n - 1 } ) - X _ { n - 1 } = 0 .$ Therefore, when the process $c = ( c _ { n } ) _ { n }$ which is integrated against the martingale $X = \left( X _ { n } \right)$ , is predictable, the martingale property is preserved under the discrete stochastic integral: $I = ( I _ { n } ) _ { n }$ is also a martingale with respect to the filtration $( \mathcal F _ { n } ) _ { n }$ . We shall write this stochastic integral as $c \cdot X$ , meaning that for all $n \geq 0 , I _ { n } = ( c \cdot X ) _ { n }$ . The result has suficient importance for us to record it as a theorem: 

## Theorem 7.30

Let $( \varOmega , \mathcal F , ( \mathcal F _ { n } ) _ { n \geq 0 } , P )$ be a filtered probability space. If X is a martingale and c is a bounded predictable process, then the discrete stochastic integral $c \cdot X$ is again a martingale. 

Note that we use the boundedness assumption in order to ensure that $c _ { k } \varDelta X _ { k }$ is integrable, so that its conditional expectation makes sense. For $\mathcal { L } ^ { 2 } .$ martingales (which are what we obtain in most applications) we can relax this condition and demand merely that $c _ { n } \in \mathcal { L } ^ { 2 } ( \mathcal { F } _ { n - 1 } )$ for each n. 

While the preservation of the martingale property may please mathematicians, it is depressing news for gamblers! We can interpret the process c as representing the size of the stake the gambler ventures in every game, so that $c _ { n }$ is the amount (s)he bets in game n. Note that $c _ { n }$ could be 0, which mean that the gambler ‘sits out’ game n and places no bet. It also seems reasonable that the size of the stake depends on the outcomes of the previous games, hence $c _ { n }$ is $\mathcal { F } _ { n - 1 } { \mathrm { - m e a s u r a b l e } }$ , and thus c is predictable. 

The conclusion that $c \cdot X$ is then a martingale means that ‘clever’ gambling strategies will be of no avail when the game is fair. It remains fair, whatever strategy the gambler employs! And, of course, if it starts out unfavourable to the gambler, so that X is a supermartingale $( X _ { n - 1 } \geq \mathbb { E } ( X _ { n } | \mathcal { F } _ { n - 1 } ) )$ , the above calculation shows that, as long as $c _ { n } \geq 0$ for each n , then E $( I _ { n } | \mathcal { F } _ { n - 1 } ) \leq I _ { n - 1 }$ , so that the game remains unfavourable, whatever non-negative stakes the gambler places (and negative bets seem unlikely to be accepted, after all. . . ). You will verify immediately, of course, that a submartingale X produces a submartingale $c \cdot X$ when c is a non-negative process. Sadly, such favourable games are hard to find in practice. 

Combining the definition of $( I _ { n } ) _ { n }$ with the Doob decomposition of the submartingale $X ^ { 2 }$ we obtain the identity which illustrates why martingales make useful ‘integrators’. We calculate the expected value of the square of $( c \cdot X ) _ { n }$ when $c = \left( c _ { n } \right)$ is predictable and $X = \left( X _ { n } \right)$ is a martingale: 

$$
\mathbb {E} ((c \cdot X) _ {n} ^ {2}) = \mathbb {E} ([ \sum_ {k = 1} ^ {n} c _ {k} \Delta X _ {k} ] ^ {2}) = \mathbb {E} (\sum_ {j, k = 1} ^ {n} c _ {j} c _ {k} \Delta X _ {j} \Delta X _ {k}).
$$

Consider terms in the double sum separately: when $j < k$ we have 

$$
\mathbb {E} (c _ {j} c _ {k} \Delta X _ {j} \Delta X _ {k}) = \mathbb {E} (c _ {j} c _ {k} \Delta X _ {j} \Delta X _ {k} | \mathcal {F} _ {k - 1}) = \mathbb {E} (c _ {j} c _ {k} \Delta X _ {j} \mathbb {E} (\Delta X _ {k} | \mathcal {F} _ {k - 1})) = 0
$$

since the first three factors are all $\mathcal { F } _ { k - 1 } .$ - measurable, while $\mathbb { E } ( \varDelta X _ { k } | \mathcal F _ { k - 1 } ) = 0$ since X is a martingale. With j, k interchanged this also shows that these terms are 0 when $k < j$ 

The remaining terms have the form 

$$
\mathbb {E} (c _ {k} ^ {2} (\varDelta X _ {k}) ^ {2}) = \mathbb {E} (c _ {k} ^ {2} \mathbb {E} ((\varDelta X _ {k}) ^ {2} | \mathcal {F} _ {k - 1})) = \mathbb {E} (c _ {k} ^ {2} \varDelta A _ {k}).
$$

By linearity, therefore, we have the fundamental identity for stochastic integrals relative to martingales (also called the Ito isometry): 

$$
\mathbb {E} ([ \sum_ {k = 1} ^ {n} c _ {k} \varDelta X _ {k} ] ^ {2}) = \mathbb {E} (\sum_ {k = 1} ^ {n} c _ {k} ^ {2} \varDelta A _ {k}).
$$

## Remark 7.3

The sum inside the expectation sign on the right is a ‘Stieltjes sum’ for the increasing process, so that it is now at least plausible that this identity allows us to define martingale integrals in the continuous-time setting, using approximation of processes by simple processes, much as was done throughout this book for real functions. The Ito isometry is of critical importance in the definition of stochastic integrals relative to processes such as Brownian motion: in defining Lebesgue–Stieltjes integrals our integrators were of bounded variation. Typically, the paths of Brownian motion (a process we shall not define in this book ${ \it \_ \mathrm { s e e \left( e . g . \right) } }$ [3] for its basic properties) are not of bounded variation, but the Ito isometry shows that their quadratic variation can be handled in the (much subtler) continuous-time version of the above framework, and this enables one to define integrals of a wide class of functions, using Brownian motion (and more general martingales) as ‘integrator’. 

We turn finally to the idea of stopping a martingale at a random time. 

## Definition 7.13

A random variable $\tau : \varOmega  \{ 0 , 1 , 2 , \dots , n , \dots \} \cup \{ \infty \}$ is a stopping time relative to the filtration $\left( \mathcal { F } _ { n } \right)$ if for every $n \geq 1$ , the event $\{ \tau = n \}$ belongs to ${ \mathcal { F } } _ { n }$ 

Note that we include the value $\tau ( \omega ) = \infty$ , so that we need $\{ \tau = \infty \} \ \in$ ${ \mathcal { F } } _ { \infty } = \sigma ( \cup _ { n \geq 1 } { \mathcal { F } } _ { n } )$ , the ‘limit σ-field’. Stopping times are also called random times, to emphasise that the ‘time’ τ is a random variable. 

For a stopping time τ the event $\{ \tau \leq n \} = \cup _ { k = 0 } ^ { n } \{ \tau = k \}$ is in ${ \mathcal { F } } _ { n }$ since for each $k \leq n \ \{ \tau = k \} \in { \mathcal { F } } _ { k }$ and the σ-fields increase with n. On the other hand, given that for each n the event $\{ \tau \leq n \} \in \mathcal { F } _ { n }$ , then 

$$
\{\tau = n \} = \{\tau \leq n \} \backslash \{\tau \leq n - 1 \} \in \mathcal {F} _ {n}.
$$

Thus we could equally well have taken the condition $\{ \tau \leq n \} \in \mathcal { F } _ { n }$ for all n as the definition of stopping time. 

## Example 7.9

A gambler may decide to stop playing after a random number of games, depending on whether his winnings X have reached a pre-determined level L (or his funds are exhausted!). The time $\tau = \operatorname* { m i n } \{ n : X _ { n } \geq L \}$ is the first time at which the process X hits the interval $[ L , \infty )$ ; more precisely, for $\omega \in { \mathcal { Q } }$ , $\tau ( \omega ) = n \mathrm { i f } X _ { n } ( \omega ) \geq L$ while $X _ { k } ( \omega ) < L$ for all $k < n$ . Since $\{ \tau = n \}$ is thus determined by the values of X and those of the $X _ { k }$ for $k < n$ it is now clear that τ is a stopping time. 

## Example 7.10

Similarly, we may decide to sell our shares in a stock S if its value falls below 75% of its current (time 0) price. Thus we sell at the random time $\tau = \operatorname* { m i n } \{ n$ : $\begin{array} { r } { S _ { n } < \frac { 3 } { 4 } S _ { 0 } \} } \end{array}$ , which is again a stopping time. This is an example of a ‘stop-loss strategy’, and is much in evidence in a bear market. 

Quite generally, the first hitting time $\tau _ { A }$ of a Borel set $A \subset \mathbb { R }$ by an adapted process X is defined by setting $\tau _ { A } = \operatorname* { m i n } \{ n \geq 0 : X _ { n } \in A \}$ . For any $n \geq 0$ we have $\{ \tau _ { A } \leq n \} = \cup _ { k \leq n } \{ X _ { k } \in A \} \in \mathcal { F } _ { n }$ . To cater for the possibility that X never hits A we use the convention min $\mathrm { O } = \infty$ , so that $\{ \tau _ { A } = \infty \} = \varOmega \setminus ( \cup _ { n \geq 0 } \{ \tau _ { A } \leq$ $n \}$ represents this event. But its complement is in $\mathcal { F } _ { \infty } = \sigma ( \cup _ { n \geq 0 } \mathcal { F } _ { n } )$ , thus so is $\{ \tau _ { A } = \infty \}$ . We have proved that $\tau _ { A }$ is a stopping time. 

Returning to the gambling theme, we see that stopping is simply a particular form of gambling strategy, and it should thus come as no surprise that the martingale property is preserved under stopping (with similar conclusions for super- and submartingales). For any adapted process X and stopping time τ , we define the stopped process $X ^ { \tau }$ by setting $X _ { n } ^ { \tau } ( \omega ) = X _ { n \wedge \tau ( \omega ) } ( \omega )$ at each $\omega \in \varOmega$ . (Recall that for real $x , y$ we write x $\land y = \operatorname* { m i n } \{ x , y \} . )$ 

The stopped process $X ^ { \tau }$ is again adapted to the filtration $( \mathcal F _ { n } ) _ { n }$ , since $\{ X _ { \tau \wedge n } \in A \}$ means that either $\tau > n$ and $X _ { n } \in A$ , or $\tau = k$ for some $k \leq n$ and $X _ { k } \in A$ . Now the event $\left\{ \ X _ { n } \in A \right\} \cap \left\{ \tau > n \right\} \in { \mathcal F } _ { n }$ , while for each k the event $\{ \tau = k \} \cap \{ X _ { k } \in A \} \in { \mathcal { F } } _ { k }$ . For all $k \leq n$ these events therefore all belong to ${ \mathcal { F } } _ { n }$ . Hence so does $\{ X _ { \tau \wedge n } \in A \}$ , which proves that $X ^ { \tau }$ is adapted. 

## Theorem 7.31

Let $( \varOmega , \mathcal F , ( \mathcal F _ { n } ) , P )$ be a filtered probability space, and let X be a martingale with $X _ { 0 } = 0$ . If $\tau$ is a stopping time, the stopped process $X ^ { \tau }$ is again a martingale. 

## Proof

We use the preservation of the martingale property under discrete stochastic integrals (‘gambling strategies’). Let $c _ { n } = \mathbf { 1 } _ { \{ \tau \geq n \} }$ for each $n \geq 1$ . This defines a bounded predictable process $c = \left( c _ { n } \right)$ , since it takes only the values 0, 1 and $\{ c _ { n } = 0 \} = \{ \tau \leq n - 1 \} \in \mathcal { F } _ { n - 1 }$ , so that also $\{ c _ { n } = 1 \} = \Omega \setminus \{ c _ { n } = 0 \} \in$ $\mathcal { F } _ { n - 1 }$ . Hence by Theorem 7.30 the process $c \cdot X$ is again a martingale. But by construction $( c \cdot X ) _ { 0 } = 0 = X _ { 0 } = X _ { 0 } ^ { \tau }$ , while for any $n \geq 1$ 

$$
(c \cdot X) _ {n} = c _ {1} (X _ {1} - X _ {0}) + c _ {2} (X _ {2} - X _ {1}) + \ldots + c _ {n} (X _ {n} - X _ {n - 1}) = X _ {\tau \wedge n}.
$$

Since $c _ { n } \geq 0$ as defined in the proof, it follows that the supermartingale and submartingale properties are also preserved under stopping. For a martingale we have, in addition, that expectation is preserved, i.e. (in general) $\mathbb { E } ( X _ { \tau \wedge n } ) = \mathbb { E } ( X _ { 0 } )$ . Similarly, expectations increase for stopped submartingales, and decrease for stopped supermartingales. 

None of this, however, guarantees that the random variable $X _ { \tau }$ defined by $X _ { \tau } ( \omega ) = X _ { \tau ( \omega ) } ( \omega )$ has finite expectation – to obtain a result which relates its expectation to that of $X _ { 0 }$ we generally need to satisfy much more stringent conditions. For bounded stopping times (where there is a uniform upper bound N with $\tau ( \omega ) \leq N$ for all $\omega \in \varOmega )$ , matters are simple: if X is a martingale, $X _ { \tau \wedge n }$ is integrable for all $n ,$ and by the above theorem E $( X _ { \tau \wedge n } ) = \mathbb { E } ( X _ { 0 } )$ . Now apply this with $n = N$ , so that $X _ { \tau \wedge n } = X _ { \tau \wedge N } = X _ { \tau }$ . Thus we have $\mathbb { E } ( X _ { \tau } ) = \mathbb { E } ( X _ { 0 } )$ whenever $\tau$ is a bounded stopping time. We shall not delve any further, but refer the reader instead to texts devoted largely to martingale theory, e.g. [12], [8], [3]. Bounded stopping times sufice for many practical applications, for example in the analysis of discrete American options in finance. 

## 7.4.3 Applications to mathematical finance

A major task and challenge for the theory of finance is to price assets and securities building models consistent with market practice. This consistency means that any deviation from the theoretical price should be penalized by the market. Specifically, if a market player quotes a price diferent from the price provided by the model, she should be bound to lose money. 

The problem is the unknown future which has somehow to be reflected in the price since market participants express their beliefs about the future by agreeing on prices. Mathematically, an ideal situation is where the price process $X ( t )$ is a martingale. Then we would have the obvious pricing formula $X ( 0 ) = \mathbb { E } ( X ( T ) )$ and in addition we would have the whole range of formulae for the intermediate prices by means of conditional expectation based on information gathered. 

However, the situation where the prices follow a martingale is incompatible with the market fact that money can be invested risk-free, which creates a benchmark for expectations for investors investing in risky securities. So we modify our task by insisting that the discounted values $Y ( t ) = X ( t ) \exp \{ - r t \}$ form a martingale. The modification is by means of a deterministic constant so it does not create a problem for asset valuation. 

A particular goal is pricing derivative securities where we are given the terminal value (a claim) of the form $f ( S ( T ) )$ , where f is known and the probability distributions of the values underlying asset $S ( t )$ are assumed to be known by taking some mathematical model. The above martingale idea would solve the pricing problem by constructing a process $X ( t )$ in such a way that $X ( T ) = f ( S ( T ) )$ (We call X a replication of the claim.) 

We can summarise the tasks: Build a model of the prices of the underlying security $S ( t )$ such that 

1. There is a replication $X ( t )$ such that $X ( T ) = f ( S ( T ) )$ 

2. The process $Y ( t ) = X ( t ) \exp \{ - r t \}$ is a martingale, so $Y ( 0 )$ is the price of the security described by f, 

3. Any deviation from the resulting prices leads to a loss. 

Steps 1 and 2 are mathematical in nature, but Step 3 is related to real market activities. 

We perform the task for the single step binomial model. 

Step 1. Recall that the prices in this model are $S ( 0 ) , S ( 1 ) = S ( 0 ) \eta$ where $\eta = U \ \mathrm { o r } \ \eta = D$ with some probabilities. Let $f ( x ) = ( x - K ) ^ { + }$ . We can easily find $X ( 0 )$ so that $X ( 1 ) = ( S ( 1 ) - K ) ^ { + }$ by building a portfolio of n shares S and m units of bank account (see Section 6.5.5) after solving the system 

$$
\begin{array}{r} n S (0) U + m R = (S (0) U - K) ^ {+}, \\ n S (0) D + m R = (S (0) D - K) ^ {+}. \end{array}
$$

Note that $X ( 1 )$ is obtained by means of the data at time $t = 0$ and the model parameters. 

Step 2. Write $R = \exp \{ r \}$ . The martingale condition we need is trivial: $X ( 0 ) R \ : = \ : \mathbb { E } ( X ( 1 ) )$ ). The task here is to find the probability measure (X is defined, we have no influence on R, so this is the only parameter we can adjust). Recall that we assume $D \leq R \leq U$ . We solve 

$$
X (0) R = p X (0) U + (1 - p) X (0) D
$$

which gives 

$$
p = \frac {R - D}{U - D}
$$

and we are done. Hence the theoretical price of a call is 

$$
C = R ^ {- 1} p (S (0) U - K) = \exp \{- r \} \mathbb {E} (S (1) - K) ^ {+}.
$$

Step 3. To see that within our model the price is right suppose that someone is willing to buy a call for $C ^ { \prime } > C$ We sell it immediately investing the proceeds in the portfolio from step 1. At exercise our portfolio matches the call payof and have earned the diference $C ^ { \prime } - C .$ . So we keep buying the call until the seller realises the mistake and raises the price. Similarly if someone is selling a call at $C ^ { \prime } < C$ we generate cash by forming the $( - n , - m )$ portfolio, buy a call (which, as a result of replication, settles our portfolio liability at maturity) and we have profit until the call prices quoted hit the theoretical price C. 

The above analysis summarises the key features of a general theory. A straightforward extension of this trivial model to n steps gives the so-called CRR (Cox–Ross–Rubinstein) model, which for large n is quite adequate for realistic pricing. We evaluated the expectation in the binomial model to establish the CRR price of a European call option in Proposition 4.37. 

For continuous time the task becomes quite dificult. In the Black–Scholes model $\begin{array} { r } { S ( t ) = S ( 0 ) \exp \{ ( r - \frac { 1 } { 2 } \sigma ^ { 2 } ) t + \sigma w ( t ) \} } \end{array}$ , where $w ( t )$ is a stochastic process (called the Wiener process or Brownian motion) with $w ( 0 ) = 0$ and independent increments such that $w ( t ) - w ( s )$ is Gaussian with zero mean and variance $t - s$ $s < t$ 

Exercise 7.21 

Show that exp $\{ - r t \} S ( t )$ is a martingale. 

Existence of the replication process $X ( t )$ is not easy but can be proved, as well as the fact that the process $Y ( t )$ is a martingale. This results in the same general pricing formula: exp $\{ - r T \} \mathbb { E } ( f ( S ( T ) )$ . Using the density of $w ( T )$ this number can be written in an explicit form for particular derivative securities (see Section 4.7.5 where the formulae for the prices of a call and put options were derived). 

## Remark 7.4

The reader familiar with finance theory will notice that we are focused on pricing derivative securities and this results in considering the model where the discounted prices form a martingale. This model is a mathematical creation not necessarily consistent with real life, which requires a diferent probability space and diferent parameters within the same framework. The link between the real world and the martingale one is provided by a special application of Radon-Nikodym theorem which links the probability measures, but this is a story we shall not pursue here and refer the reader to numerous books devoted to the subject (for example [5]). 

## 7.5 Proofs of propositions

## Proof (of Proposition 7.1)

Suppose the $( \varepsilon , \delta )$ -condition fails. With A as in the hint, we have $\mu ( A ) \ \leq$ $\begin{array} { r } { \mu ( \bigcup _ { i \geq n } F _ { i } ) ~ \leq ~ \sum _ { i = n } ^ { \infty } \frac { 1 } { 2 ^ { i } } ~ = ~ \frac { 1 } { 2 ^ { n - 1 } } } \end{array}$ for every $n \ \geq \ 1$ . Thus $\mu ( A ) ~ = ~ 0$ . But $\nu ( F _ { n } ) ~ \ge ~ \varepsilon$ Pfor every n, hence $\nu ( E _ { n } ) ~ \geq ~ \varepsilon ,$ where $E _ { n } ~ = ~ \bigcup { } _ { i \geq n } F _ { i }$ . The sequence $( E _ { n } ) _ { n }$ decreases, so that, as $\nu ( F _ { 1 } )$ Sis finite, Theorem 2.13 (i) gives: $\nu ( A ) = \nu ( \operatorname* { l i m } _ { n } E _ { n } ) = \operatorname* { l i m } _ { n } \nu ( E _ { n } ) \geq \varepsilon$ . Thus $\nu$ is not absolutely continuous with respect to $\mu .$ . Conversely, if the $( \varepsilon , \delta )$ -condition holds, and $\mu ( F ) = 0$ , then $\mu ( F ) < \delta$ for any $\delta > 0$ , and so, for every given $\varepsilon > 0 , \nu ( F ) < \varepsilon$ . Hence $\nu ( F ) = 0 . \mathrm { S o } \ \nu \ll \mu$ □ 

## Proof (of Proposition 7.4)

We proceed as in Remark 4.1. Begin with g as the indicator function ${ \bf 1 } _ { G }$ for $G \in { \mathcal { G } }$ . Then we have: $\begin{array} { r } { \int _ { \Omega } g \mathrm { d } \mu = \mu ( G ) = \int _ { G } h _ { \mu } } \end{array}$ dϕ by construction of $h _ { \mu }$ . Next, let $\begin{array} { r } { g = \sum _ { i = 1 } ^ { n } a _ { i } \mathbf { 1 } _ { G _ { i } } } \end{array}$ Rfor sets $G _ { 1 } , G _ { 2 } , \ldots , G _ { n }$ in $\mathcal { G }$ , and reals $a _ { 1 } , a _ { 2 } , \ldots , a _ { n }$ ; then Plinearity of the integrals yields 

$$
\int_ {\Omega} g \mathrm{d} \mu = \sum_ {i = 1} ^ {n} a _ {i} \mu (G _ {i}) = \sum_ {i = 1} ^ {n} a _ {i} (\int_ {G _ {i}} h _ {\mu} \mathrm{d} \varphi) = \sum_ {i = 1} ^ {n} a _ {i} (\int_ {\Omega} \mathbf {1} _ {G _ {i}} h _ {\mu} \mathrm{d} \varphi) = \int_ {\Omega} g h _ {\mu} \mathrm{d} \varphi .
$$

Finally, any -measurable non-negative function g is approximated from below by an increasing sequence of -simple functions $\begin{array} { r } { g _ { n } = \sum _ { i = 1 } ^ { n } a _ { i } \mathbf { 1 } _ { G _ { i } } } \end{array}$ , its integral $\textstyle \int _ { \Omega } g \mathrm { d } \mu$ is the limit of the increasing sequence $\begin{array} { r } { ( \int _ { \Omega } g _ { n } h _ { \mu } \mathrm { d } \varphi ) _ { n } } \end{array}$ . But since $0 \leq$ $h _ { \mu } \leq 1$ by construction, $( g _ { n } h _ { \mu } )$ increases to $g h _ { \mu }$ pointwise, hence the sequence $\textstyle ( \int _ { \Omega } g _ { n } h _ { \mu } \mathrm { d } \varphi ) _ { n }$ also increases to $\int _ { \varOmega } g h _ { \mu } \mathrm { d } \varphi$ , so the limits are equal. For integrable $g = g ^ { + } - g ^ { - }$ apply the above to each of $g ^ { + } , g ^ { - }$ separately, and use linearity. 

## Proof (of Proposition 7.6)

If $\textstyle \bigcup _ { n > 1 } A _ { n } \ = \ \varOmega$ and the $A _ { n }$ are not disjoint, replace them by $E _ { n }$ , where $E _ { 1 } = A _ { 1 } , E _ { n } = A _ { n } \setminus ( \bigcup _ { i = 1 } ^ { n - 1 } E _ { i } ) , n > 1$ . The same can be done for the $B _ { m }$ and Shence we can take both sequences as disjoint. Now $\begin{array} { r } { \varOmega = \bigcup _ { m , n \geq 1 } ( A _ { n } \cap B _ { m } ) } \end{array}$ is also a disjoint union, and $\nu , \mu$ are both finite on each $A _ { n } \cap B _ { m }$ . Re-order these sets into a single sequence $( C _ { n } ) _ { n \geq 1 }$ and fix $n \geq 1$ . Restricting both measures to the σ-field ${ \mathcal { F } } _ { n } = \{ F \cap C _ { n } : F \in { \mathcal { F } } \}$ yields them as finite measures on $( \Omega , { \mathcal { F } } _ { n } )$ 2 so that the Radon-Nikodym theorem applies, and provides a non-negative $\mathcal { F } _ { n ^ { - } }$ measurable function $h _ { n }$ such that $\textstyle \nu ( E ) = \int _ { E } h \mathrm { d } \mu$ for each $E \in \mathcal { F } _ { n }$ . But any set $F \in \mathcal { F }$ has the form $F = \textstyle \bigcup _ { n } F _ { n }$ for $F _ { n } ~ \in ~ \mathcal { F } _ { n } .$ , so we can define h by setting $h = h _ { n }$ for every $n \geq 1$ S. Now $\begin{array} { r } { \nu ( F ) = \sum _ { n = 1 } ^ { \infty } \int _ { F _ { n } } h _ { n } \mathrm { d } \mu = \int _ { F } h \mathrm { d } \mu } \end{array}$ . The P Runiqueness is clear: if g has the same properties as h,then $\begin{array} { r } { \int _ { F } ( h - g ) \mathrm { d } \mu = 0 } \end{array}$ for each $F \in { \mathcal { F } }$ , so $h - g = 0 ~ \mathrm { a . e }$ . by Theorem 4.15. □ 

## Proof (of Proposition 7.7)

(i) This is trivial, since $\phi = \lambda + \nu$ is σ-finite and absolutely continuous with respect to $\mu ,$ and we have, for $F \in { \mathcal { F } }$ : 

$$
\int_ {F} \frac {d \phi}{d \mu} \mathrm{d} \mu = \phi (F) = (\lambda + \nu) (F) = \lambda (F) + \nu (F) = \int_ {F} [ \frac {d \lambda}{d \mu} + \frac {d \nu}{d \mu} ] \mathrm{d} \mu .
$$

The integrands on the right and left extremes are thus a.s. $( \mu )$ equal, so the result follows. 

(ii) Write $\begin{array} { r } { \frac { d \lambda } { d \nu } = g } \end{array}$ and $\begin{array} { r } { \frac { d \nu } { d \mu } = h } \end{array}$ . These are non-negative measurable functions and we need to show that, for $F \in { \mathcal { F } }$ 

$$
\lambda (F) = \int_ {F} g h \mathrm{d} \mu .
$$

First consider this when $g$ is replaced by a simple function of the form $\phi =$ $\scriptstyle \sum _ { i = 1 } ^ { n } c _ { i } \mathbf { 1 } _ { E _ { i } }$ . Then we obtain: 

$$
\int_ {F} \phi \mathrm{d} \nu = \sum_ {i = 1} ^ {n} c _ {i} \nu (F \cap E _ {i}) = \sum_ {i = 1} ^ {n} c _ {i} \int_ {F \cap E _ {i}} h \mathrm{d} \mu = \int_ {F} \phi h \mathrm{d} \mu .
$$

Now let $\left( \phi _ { n } \right)$ be a sequence of simple functions increasing pointwise to $g .$ . Then 

by monotone convergence theorem: 

$$
\lambda (F) = \int_ {F} g \mathrm{d} \nu = \lim _ {n} \int_ {F} \phi_ {n} \mathrm{d} \nu = \lim _ {n} \int_ {F} \phi_ {n} h \mathrm{d} \mu = \int_ {F} g h \mathrm{d} \mu ,
$$

since $( \phi _ { n } h )$ increases to $g h$ . This proves our claim. 

## Proof (of Proposition 7.8)

Use the hint: $\lambda _ { 1 } + \lambda _ { 2 }$ is concentrated on $A _ { 1 } \cup A _ { 2 }$ , while $\mu$ is concentrated on $B _ { 1 } \cap B _ { 2 }$ . But $A _ { 1 } \cup A _ { 2 }$ is disjoint from $B _ { 1 } \cap B _ { 2 }$ , hence the measures $\lambda _ { 1 } + \lambda _ { 2 }$ and $\mu$ are mutually singular. This proves (i). For (ii), choose a set E for which $\mu ( E ) = 0$ while $\lambda _ { 2 }$ is concentrated on $E$ . Let $F \subset E$ , so that $\mu ( F ) = 0$ and hence $\lambda _ { 1 } ( F ) = 0$ (since $\lambda _ { 1 } \ll \mu )$ . This shows that $\lambda _ { 1 }$ is concentrated on $E ^ { c }$ 8 hence $\lambda _ { 1 }$ and $\lambda _ { 2 }$ are mutually singular. Finally, (ii) applied with $\lambda _ { 1 } = \lambda _ { 2 } = \nu$ shows that $\nu \perp \nu$ , which can only happen when $\nu = 0$ □ 

## Proof (of Proposition 7.11)

Fix $x \in \mathbb { R }$ . The set $A = \{ F ( y ) : y < x \}$ is bounded above by $F ( x )$ , while $B = \{ F ( y ) : x < y \}$ is bounded below by $F ( x )$ . Hence sup $A = K _ { 1 } \leq F ( x )$ and inf $B = K _ { 2 } \geq F ( x )$ both exist in R and for any $\varepsilon > 0$ , we can find $y _ { 1 } < x$ such that $K _ { 1 } - \varepsilon < F ( y _ { 1 } )$ and $y _ { 2 } > x$ such that $K _ { 2 } + \varepsilon > F ( y _ { 2 } )$ . But since $F$ is increasing this means that $K _ { 1 } - \varepsilon < F ( y ) < K _ { 1 }$ throughout the interval $( y _ { 1 } , x )$ and $K _ { 2 } < F ( y ) < K _ { 2 } + \varepsilon$ throughout $( y , y _ { 2 } )$ . Thus both one-sided limits $F ( x - ) = \operatorname* { l i m } _ { y \uparrow x } F ( y )$ and $F ( x + ) = \operatorname* { l i m } { } _ { y \downarrow x } F ( y )$ are well-defined and by their definition $F ( x - ) \leq F ( x ) \leq F ( x + )$ 

Now let $C = \{ x \in \mathbb { R } : F$ is discontinuous at $x \}$ . For any $x \in C$ we have $F ( x - ) < F ( x + )$ . Hence we can find a rational $r = r ( x )$ in the open interval $( F ( x - ) , F ( x + ) )$ . No two distinct x can have the same $r ( x )$ , since if $x _ { 1 } < x _ { 2 }$ we obtain $F ( x _ { 1 } + ) ~ \leq ~ F ( x _ { 2 } - )$ from the definition of these limits. Thus the correspondence $x  r ( x )$ defines a one-one correspondence between C and a subset of Q, so C is at most countable. At each discontinuity we have $F ( x - ) <$ $F ( x + )$ , so all discontinuities result from jumps of $F .$ □ 

## Proof (of Proposition 7.12)

Fix $\varepsilon > 0$ , and let a finite set of disjoint intervals $J _ { k } = \left( x _ { k } , y _ { k } \right)$ be given. Let $\textstyle E = \bigcup _ { k } J _ { k }$ . Then 

$$
\sum_ {k = 1} ^ {n} | F (y _ {k}) - F (x _ {k}) | = \sum_ {k = 1} ^ {n} \left| \int_ {x _ {k}} ^ {y _ {k}} f \mathrm{d} m \right| \leq \sum_ {k = 1} ^ {n} \int_ {x _ {k}} ^ {y _ {k}} | f | \mathrm{d} m = \int_ {E} | f | \mathrm{d} m.
$$

But since $f \in \mathcal { L } ^ { 1 }$ , the measure $\textstyle \mu ( G ) = \int _ { G } | f |$ dm is absolutely continuous with respect to Lebesgue measure m and hence, by Proposition 7.1, there exists $\delta > 0$ such that $m ( F ) < \delta$ implies $\mu ( F ) < \varepsilon$ . But if the total length of the intervals $J _ { k }$ is less than $\delta ,$ , then $m ( F ) < \delta$ , hence $\mu ( F ) < \varepsilon$ . This proves that the function F is absolutely continuous. □ 

## Proof (of Proposition 7.14)

Use the functions defined in the hint: for any partition $( x _ { k } ) _ { k \leq n }$ of $[ a , x ]$ we have 

$$
\begin{array}{l} F (x) - F (a) = \sum_ {k = 1} ^ {n} [ F (x _ {k}) - F (x _ {k - 1}) ] \\ \qquad = \sum_ {k = 1} ^ {n} [ F (x _ {k}) - F (x _ {k - 1}) ] ^ {+} - \sum_ {k = 1} ^ {n} [ F (x _ {k}) - F (x _ {k - 1}) ] ^ {-} \\ \qquad = p (x) - n (x) \end{array}
$$

so that $p ( x ) = n ( x ) + [ F ( b ) - F ( a ) ] \leq N _ { F } ( x ) + [ F ( ( b ) - F ( a ) ]$ by definition of sup. This holds for all partitions, hence $P _ { F } ( x ) = \operatorname* { s u p } p ( x ) \leq N _ { F } ( x ) + [ F ( ( b ) - F ( a ) ]$ On the other hand, writing $n ( x ) = p ( x ) + [ F ( a ) - F ( b ) ]$ yields $N _ { F } ( x ) \leq P _ { F } ( x ) +$ $[ F ( a ) - F ( b ) ]$ ]. Thus $P _ { F } ( x ) - N _ { F } ( x ) = F ( b ) - F ( a )$ . Now for any fixed partition we have 

$$
\begin{array}{l} T _ {F} (x) \geq \sum_ {k = 1} ^ {n} | F (x _ {k}) - F (x _ {k - 1}) | = p (x) + n (x) = p (x) + \{p (x) - [ F (b) - F (a) ] \} \\ \qquad = 2 p (x) - [ P _ {F} (x) - N _ {F} (x) ] = 2 p (x) + N _ {F} (x) - P _ {F} (x). \end{array}
$$

Take the supremum on the right: $T _ { F } ( x ) \ge 2 { \cal P } _ { F } ( x ) + { \cal N } _ { F } ( x ) - { \cal P } _ { F } ( x ) =$ $P _ { F } ( x ) + N _ { F } ( x )$ . But we can also write $\begin{array} { r } { \sum _ { k = 1 } ^ { n } | F ( x _ { k } ) - F ( x _ { k - 1 } ) | = p ( x ) + } \end{array}$ $n ( x ) \leq P _ { F } ( x ) + N _ { F } ( x )$ Pfor any partition, so taking the sup on the left provides $T _ { F } ( x ) \le { \cal P } _ { F } ( x ) + N _ { F } ( x )$ . So the two sides are equal. □ 

## Proof (of Proposition 7.15)

It will sufice to prove this for $T _ { F }$ , as the other cases are similar. If the partition of $[ a , b ]$ produces the sum $t ( \mathcal P )$ for the absolute diferences, and if ${ \mathcal { P } } ^ { \prime } = { \mathcal { P } } \cup \{ c \}$ for some $c \in ( a , b )$ , then $t ( \mathcal { P } ) [ a , b ] \leq t ( \mathcal { P } ^ { \prime } ) [ a , c ] + t ( \mathcal { P } ^ { \prime } ) [ c , b ]$ and this is bounded above by $T _ { F } [ a , c ] + T _ { F } [ c , b ]$ for all partitions. Thus it bounds $T _ { F } [ a , b ]$ also. On the other hand, any partitions of $[ a , c ]$ and [c, b] together make up a partition of $[ a , b ]$ , so that $T _ { F } [ a , b ]$ bounds their joint sums. So the two sides must be equal. In particular, fixing $a , T _ { F } ( [ a , c ] \leq T _ { F } [ a , b ]$ when $c \leq b$ , hence $T _ { F } ( x ) = T _ { F } [ a , x ]$ is increasing with x. The same holds for $P _ { F }$ and $N _ { F }$ . The final statement is obvious. □ 

## Proof (of Proposition 7.17)

(i) Given $\varepsilon > 0$ , find $\delta > 0$ such that $\begin{array} { r } { \sum _ { i = 1 } ^ { n } ( y _ { i } - x _ { i } ) < \delta } \end{array}$ implies $\textstyle \sum _ { i = 1 } ^ { n } | F ( y _ { i } ) -$ $\begin{array} { r } { F ( x _ { i } ) | \ < \ \frac { \varepsilon \delta } { b - a } } \end{array}$ . Given a partition $( t _ { i } ) _ { i \le K }$ of $[ a , b ]$ P, we add further partition points, uniformly spaced and at a distance $\textstyle { \frac { b - a } { M } }$ from each other, to ensure that the combined partition $( z _ { i } ) _ { i \leq N }$ has all its points less than $\delta$ apart. To do this we simply need to choose M as the integer part of $\begin{array} { r } { T = \frac { b - a } { \delta } + 1 } \end{array}$ . Since the $( t _ { j } )$ form a subset of the partition points $( z _ { i } ) _ { i = 0 , 1 , . . . , N }$ it follows that 

$$
\sum_ {i = 1} ^ {K} | F (t _ {i}) - F (t _ {i - 1}) | \leq \sum_ {i = 1} ^ {N} | F (z _ {i}) - F (z _ {i - 1}) |.
$$

The latter sum can be re-ordered into M groups of terms where each group begins and ends with two consecutive new partition points: the $k ^ { t h }$ group then contains $( \operatorname { s a y } ) \ m _ { k }$ points altogether, and by their construction, the sum of their consecutive distances (i.e. the distance between the two new endpoints!) is less than $\delta ,$ so for each $\begin{array} { r } { k \leq M , \sum _ { i = 1 } ^ { m _ { k } } | F ( w _ { i , k } ) - F ( w _ { i - 1 , k } ) | < \frac { \varepsilon \delta } { b - a } } \end{array}$ , where the $( w _ { i , k } )$ are the re-ordered points $\left( z _ { i } \right)$ . Thus the whole sum is bounded by $\begin{array} { r } { M ( \frac { \varepsilon \delta } { b - a } ) \ \leq \ T ( \frac { \varepsilon \delta } { b - a } ) \ < \ \varepsilon } \end{array}$ . This shows that $F \in B V [ a , b ]$ , since the bound is independent of the original partition $( t _ { i } ) _ { i \le K }$ 

For (ii), note first that, by (i), the function F has bounded variation on $[ a , b ]$ , so that over any subinterval $[ x _ { i } , y _ { i } ]$ the total variation function $T _ { F } [ x _ { i } , y _ { i } ]$ is finite. Again take $\varepsilon , \delta$ as given in the definition of absolutely continuous functions. If $( x _ { i } , y _ { i } ) _ { i \leq n }$ are subintervals with $\begin{array} { r } { \sum _ { i = 1 } ^ { n } | y _ { i } - x _ { i } | < \delta } \end{array}$ then $\begin{array} { r } { \sum _ { i = 1 } ^ { n } | F ( y _ { i } ) - F ( x _ { i } ) | < \varepsilon } \end{array}$ P. As in the previous proposition this implies that $T _ { F } [ x _ { i } , y _ { i } ] \leq \varepsilon$ . Thus both $P _ { F } [ x _ { i } , y _ { i } ]$ and $N _ { F } [ x _ { i } , y _ { i } ]$ are less than $\varepsilon ,$ so that the functions $F _ { 1 }$ and $F _ { 2 }$ are absolutely continuous. □ 

## Proof (of Proposition 7.18)

Obviously $\nu ( \ r _ { \bigcirc } ) = 0$ and $\emptyset \subset E$ for any E. So if ν is monotone increasing, $\nu ( E ) \geq \nu ( \mathbb { O } ) \geq 0$ . Hence ν is a measure. Conversely, if $\nu$ is a measure, $F \subset E$ 2 $\nu ( E ) = \nu ( F ) + \nu ( E \setminus F ) \geq \nu ( E )$ □ 

## Proof (of Proposition 7.26)

If $E ~ = ~ \{ f ~ > ~ 1 \}$ has $\rho ( E ) ~ > ~ 0 , ~ \frac { f } { \rho ( E ) }$ is well-defined and $\begin{array} { r } { \int _ { E } \frac { f } { \rho ( E ) } \mathrm { d } \rho \ = } \end{array}$ $\begin{array} { r } { \frac { 1 } { \rho ( E ) } \int _ { E } f \mathrm { d } \rho > 1 } \end{array}$ . This contradicts the hypothesis, so $\rho ( E ) = 0$ . Similarly, $\stackrel { \cdot } { F } = \left\{ f < - 1 \right\}$ has $\rho ( F ) = 0$ . Hence $| f | \le 1 \ \rho { \mathrm { - a . e } }$ □ 

## Proof (of Proposition 7.27)

Choose $h , A , B$ as in the hint. Recall that $\nu ^ { + } = \textstyle { \frac { 1 } { 2 } } ( | \nu | + \nu )$ , and note that ${ \bf \Pi } _ { 2 } ^ { 1 } ( 1 + h ) = h \mathbf { 1 } _ { B }$ , so that, for $F \in { \mathcal { F } }$ 

$$
\nu^ {+} (F) = \frac {1}{2} \int_ {F} (1 + h) \mathrm{d} | \nu |) = \int_ {F \cap B} h \mathrm{d} | \nu | = \nu (F \cap B).
$$

But then, since $B = A ^ { c }$ 

$$
\nu^ {-} (F) = - [ \nu (F) - \nu^ {+} (F) ] = - [ \nu (F) - \nu (F \cap B) ] = - \nu (F \cap A).
$$

Finally, if $\nu = \lambda _ { 1 } - \lambda _ { 2 }$ where the $\lambda _ { i }$ are measures, then $\nu \leq \lambda _ { 1 }$ , so that $\nu ^ { + } ( F ) = \nu ( F \cap B ) \leq \lambda _ { 1 } ( F \cap B ) \leq \lambda _ { 1 } ( F )$ by monotonicity. This proves the final statement of the proposition. □ 

## Proof (of Proposition 7.28)

(i) Is immediate, as $\begin{array} { r } { \int _ { \Omega } \mathbb { E } ( X | \mathcal { G } ) \mathrm { d } P = \int _ { \Omega } X } \end{array}$ dP by definition. 

(ii) If both integrands are -measurable and $\textstyle \int _ { G } \operatorname { \mathbb { E } } ( X | { \mathcal { G } } ) \mathrm { d } P = \int _ { G } X \mathrm { d } P$ for all $G \in { \mathcal { G } }$ , then the integrands are a.s. equal by Theorem 4.15, and thus X is a version of $\mathbb { E } ( X | \mathcal { G } )$ 

(iii) For any $G \in { \mathcal { G } } , 1 _ { G }$ and X are independent random variables, so that 

$$
\int_ {G} X \mathrm{d} P = \mathbb {E} (X \mathbf {1} _ {G}) = \mathbb {E} (X) \mathbb {E} (\mathbf {1} _ {G}) = \int_ {G} \mathbb {E} (X) \mathrm{d} P
$$

Hence by definition $\mathbb { E } ( X )$ is a version of $\mathbb { E } ( X | \mathcal { G } )$ . But $\mathbb { E } ( X )$ is constant, so the identity holds everywhere. 

(iv) Use the linearity of integrals: 

$$
\begin{array}{c} \int_ {G} (a X + b Y) = a \int_ {G} X   \mathrm{d} P + b \int_ {G} Y   \mathrm{d} P = a \int_ {G} \mathbb {E} (X | \mathcal {G})   \mathrm{d} P + b \int_ {G} \mathbb {E} (Y | \mathcal {G})   \mathrm{d} P \\ = \int_ {G} [ a \mathbb {E} (X | \mathcal {G})   \mathrm{d} P + b \mathbb {E} (Y | \mathcal {G}) ]   \mathrm{d} P, \end{array}
$$

so the result follows. 

In this chapter we introduce something of a change of pace and the reader may omit the more technically demanding proofs at a first reading, in order to gain an overview of the principal limit theorems for sequences of random variables. We put the spotlight firmly on probability to derive substantive applications of the preceding theory. 

First, however we discuss some basic modes of convergence of sequences of functions of real variable. Then we move to the probabilistic setting to which this chapter is largely devoted. 

## 8.1 Modes of convergence

Let E be a Borel subset of $\mathbb { R } ^ { n }$ . For a given sequence $\left( f _ { n } \right)$ in $L ^ { p } ( E ) , p \geq 1$ , we can express the statement $\cdot f _ { n }  f$ as $n \to \infty ^ { \prime }$ in a number of distinct ways: 

## Definition 8.1

(1) $f _ { n }  f$ uniformly on E: given $\varepsilon > 0$ , there exists $N = N ( \varepsilon )$ such that, for all $n \geq N$ 2 

$$
\| f _ {n} - f \| _ {\infty} = \sup _ {x \in E} (| f _ {n} (x) - f (x) |) <   \varepsilon .
$$

(Note that we need $f _ { n } \in L ^ { \infty } ( E )$ for the sup to be finite in general.) 

(2) $f _ { n }  f$ pointwise on $E \colon$ for each $x \in E$ , given $\varepsilon > 0$ , there exists $N =$ $N ( \varepsilon , x )$ such that $| f _ { n } ( x ) - f ( x ) | < \varepsilon$ for all $n \geq N$ 

(3) $f _ { n }  f$ almost everywhere $\left( \mathrm { a . e . } \right)$ on $E \colon$ there is a null set $F \subset E$ such that $f _ { n }  f$ pointwise on $E \backslash F$ 

(4) $f _ { n }  f$ in $L ^ { p } - n o r m$ (in the $\mathrm { p } ^ { \mathrm { t h } }$ mean): $\| f _ { n } - f \| _ { p } \to 0$ as $n \to \infty$ , i.e. for given $\varepsilon > 0 , \exists N = N ( \varepsilon )$ such that 

$$
\| \mathrm {f_ {n} - f \| _ {p}} = \left(\int_ {\mathrm{E}} | \mathrm {f_ {n} - f | ^ {p} dm}\right) ^ {\frac {1}{\mathrm{p}}} <   \varepsilon
$$

for all $n \geq N$ 

Handling these diferent modes of convergence requires some care; at this point we have not even shown that they are all genuinely diferent. Clearly, pointwise (and a.e.) limits are often easier to ‘guess’, however, we cannot always be certain that the limit function, if it exists, is again a member of $L ^ { p } ( E )$ For mean convergence, however, this is ensured by the completeness of $L ^ { p } ( E )$ and similarly for uniform convergence, which is just convergence in the $L ^ { \infty _ { - } }$ norm. Note that the conclusions of the dominated and monotone convergence theorems yield the mean convergence of a.e. convergent sequences $\left( f _ { n } \right)$ , but only by imposing additional conditions on the $\left( f _ { n } \right)$ 

## Theorem 8.1

With $\left( f _ { n } \right)$ as above, the only valid implications are the following: $( 1 ) \Rightarrow ( 2 ) \Rightarrow$ (3). For finite measures, $( 1 ) \Rightarrow ( 4 )$ 

## Proof

The above implications are obvious. It is also obvious that $( 3 )  { \neq } ( 2 )$ . To see that $( 2 )  { \not \Rightarrow } ( 1 )$ take $E = [ 0 , 1 ] , f _ { n } = \mathbf { 1 } _ { ( 0 , \frac { 1 } { n } ) }$ which converges to $f = 0$ at all points but sup $f _ { n } = 1$ for all n. 

For $( 3 ) \ \not \Rightarrow \ ( 4 )$ take $f _ { n } ~ = ~ n { \bf 1 } _ { ( 0 , \frac { 1 } { n } ] } ; ~ f _ { n }$ converges to 0 pointwise, but $\begin{array} { r } { \int _ { 0 } ^ { 1 } f _ { n } ^ { p } \mathrm { d } m = n ^ { p } \frac { 1 } { n } = n ^ { p - 1 } \geq 1 } \end{array}$ 

To see that $( 4 ) \not \Rightarrow ( 3 )$ , let $E = [ 0 , 1 ]$ and put 

$$
\begin{array}{l l} g _ {1} = \mathbf {1} _ {[ 0, \frac {1}{2} ]} & g _ {2} = \mathbf {1} _ {[ \frac {1}{2}, 1 ]} \\ g _ {3} = \mathbf {1} _ {[ 0, \frac {1}{4} ]} & g _ {4} = \mathbf {1} _ {[ \frac {1}{4}, \frac {2}{4} ]} \\ & g _ {5} = \mathbf {1} _ {[ \frac {2}{4}, \frac {3}{4} ]} \\ & g _ {6} = \mathbf {1} _ {[ \frac {3}{4}, 1 ]} \end{array}
$$

Then 

$$
\int_ {0} ^ {1} g _ {n} ^ {p} \mathrm{d} m = \int_ {0} ^ {1} g _ {n} \mathrm{d} m \rightarrow 0
$$

but for each $x \in [ 0 , 1 ] , g _ { n } ( x ) = 1$ for infinitely many n, so $g _ { n } ( x )$ does not converge at any x in E. □ 

## Example 8.1

We investigate 

$$
h _ {n} (x) = x ^ {n}
$$

for convergence in each of these modes on $E = [ 0 , 1 ]$ 

The sequence converges everywhere to the function $h ( x ) = 0$ for $x \in [ 0 , 1 )$ $h ( 1 ) = 1$ , and so it also converges almost everywhere. 

It does not converge uniformly since $\begin{array} { r } { \operatorname* { s u p } _ { [ 0 , 1 ] } | h _ { n } ( x ) - h ( x ) | = 1 } \end{array}$ for all n. It converges in $L ^ { p }$ for $p > 0$ : 

$$
\int_ {0} ^ {1} | h _ {n} (x) - h (x) | ^ {p} \mathrm{d} x = \int_ {0} ^ {1} x ^ {p n} \mathrm{d} x = \frac {1}{p n + 1} x ^ {p n + 1} \Big | _ {0} ^ {1} \to 0.
$$

## Remark 8.1

There are still other modes of convergence which can be considered for sequences of measurable functions, and the relations between these and the above are quite complex in general. Here we will not pursue this theme in general, but specialize instead to probability spaces, where we derive additional relationships between the diferent limit processes. 

## Exercise 8.1

For each of the following decide whether $f _ { n } \to 0 ( \mathrm { i } )$ in L<sup>p</sup>, (ii) uniformly, (iii) pointwise, (iv) a.e. 

(a) $f _ { n } = \mathbf { 1 } _ { [ n , n + \frac { 1 } { n } ] } ,$ 

(b) $f _ { n } = n \mathbf { 1 } _ { [ 0 , \frac { 1 } { n } ] } - n \mathbf { 1 } _ { [ - \frac { 1 } { n } , 0 ] } .$ 

## 8.2 Probability

The remainder of this chapter is devoted to a discussion of the basic limit theorems for random variables in probability theory. The very definition of ‘probabilities’ relies on a belief in such results, i.e. that we can ascribe a meaning to the ‘limiting average’ of successes in a sequence of independent identically distributed trials. Then the purpose of the ‘endless repetition’ of tossing a coin is to use the ‘limiting frequency’ of Heads as the definition of the probability of Heads. 

Similarly, the pivotal role ascribed in statistics to the Gaussian density has its origin in the famous Central Limit Theorem (of which there is actually a large variety) which shows this density to describe the limit distribution of a sequence of distributions under appropriate conditions. Convergence of distributions therefore provides yet a further important limit concept for sequences of random variables. 

In both cases the concept of independence plays a crucial role and first of all we need to extend this concept to infinite sequences of random variables. In what follows, 

$$
X _ {1}, X _ {2}, \ldots , X _ {n}, \ldots
$$

will denote a sequence of random variables defined on a probability space. 

## Definition 8.2

We say that random variables $X _ { 1 } , X _ { 2 } , . . .$ . are independent if for any $n \in \mathbb { N }$ the variables $X _ { 1 } , \ldots , X _ { n }$ are independent (see Definition 3.3). 

An alternative is to demand that any finite collection of $X _ { i }$ be independent. Of course this condition implies independence since finite collections cover the initial segments of n variables. 

Conversely, take any finite collection of $X _ { i }$ and let n be the greatest index of this finite collection. Now $X _ { 1 } , \ldots , X _ { n }$ are independent and then for each subset the collection of its elements is independent; this includes, in particular, the chosen one. 

We study the following sequence 

$$
S _ {n} = X _ {1} + \dots + X _ {n}.
$$

If all $X _ { i }$ have the same distribution (we say that they are identically distributed), then $\scriptstyle { \frac { S _ { n } } { n } }$ is the average value of $X _ { n }$ (or $X _ { 1 }$ , it does not matter) after n repetitions of the same experiment. 

We study the bahaviour of $S _ { n }$ as n goes to infinity? The two main questions we address are: 

1. When do the random variables $\frac { S _ { n } } { n }$ converge to a certain number? Here there is an immediate question of the appropriate mode of convergence. Positive answers to such questions are known as laws of large numbers. 

2. When do the distributions of the random variables $\scriptstyle { \frac { S _ { n } } { n } }$ converge to a measure? Under what conditions is this limit measure Gaussian? The results we obtain in response are known as central limit theorems. 

## 8.2.1 Convergence in probability

Our first additional mode of convergence, convergence in probability, is sometimes termed ‘convergence in measure’. 

## Definition 8.3

A sequence $X _ { 1 } , X _ { 2 } , . . .$ . converges to X in probability if for each $\varepsilon > 0$ 

$$
P (| X _ {n} - X | > \varepsilon) \rightarrow 0
$$

as $n \to \infty$ 

## Exercise 8.2

Go back to the proof of Theorem 8.1 (with $E = [ 0 , 1 ] )$ to see which of the sequences of random variables constructed there converge in probability. 

## Exercise 8.3

Find an example of a sequence of random variables on [0, 1] that does not converge to 0 in probability. 

We begin by showing that convergence almost surely (i.e. almost everywhere) is stronger than convergence in probability. But first we prove an auxiliary result. 

## Lemma 8.2

The following conditions are equivalent 

(a) $Y _ { n }  0$ almost surely 

(b) for each $\varepsilon > 0$ 

$$
\lim _ {k \to \infty} P (\bigcup_ {n = k} ^ {\infty} \{\omega : | Y _ {n} (\omega) | \geq \varepsilon \}) = 0.
$$

Proof 

Convergence almost surely, expressed succinctly, means that 

$$
P (\{\omega : \forall \varepsilon > 0 \exists N \in \mathbb {N}: \forall n \geq N, | Y _ {n} (\omega) | <   \varepsilon \}) = 1.
$$

Writing this set of full measure another way we have 

$$
P (\bigcap_ {\varepsilon > 0} \bigcup_ {N \in \mathbb {N}} \bigcap_ {n \geq N} \{\omega : | Y _ {n} (\omega) | <   \varepsilon \}) = 1.
$$

The probability of the outer intersection (over all $\varepsilon > 0 )$ is less then the prob ability of any of its terms, but being already 1, it cannot increase, hence for all $\varepsilon > 0$ 

$$
P (\bigcup_ {N \in \mathbb {N}} \bigcap_ {n \geq N} \{\omega : | Y _ {n} (\omega) | <   \varepsilon \}) = 1.
$$

We have a union of increasing sets so 

$$
\lim _ {N \to \infty} P (\bigcap_ {n \geq N} \{\omega : | Y _ {n} (\omega) | <   \varepsilon \}) = 1
$$

thus 

$$
\lim _ {N \to \infty} (1 - P (\bigcap_ {n \geq N} \{\omega : | Y _ {n} (\omega) | <   \varepsilon \})) = 0
$$

but we can write $1 = P ( \varOmega )$ so that 

$$
\begin{array}{c} P (\varOmega) - P (\bigcap_ {n \geq N} \{\omega : | Y _ {n} (\omega) | <   \varepsilon \}) = P (\varOmega \setminus \bigcap_ {n \geq N} \{\omega : | Y _ {n} (\omega) | <   \varepsilon \}) \\ = P (\bigcup_ {n \geq N} \{\omega : | Y _ {n} (\omega) | \geq \varepsilon \}) \end{array}
$$

by De Morgan’s law. Hence (a) implies (b). Working backwards, these steps also prove the converse. □ 

## Theorem 8.3

If $X _ { n } \to X$ almost surely then $X _ { n } \to X$ in probability. 

## Proof

For simplicity of notation consider the diference $Y _ { n } = X _ { n } - X$ and the problem reduces to the discussion of convergence of $Y _ { n }$ to zero. We have 

$$
\lim _ {k \to \infty} P (\bigcup_ {n = k} ^ {\infty} \{\omega : | Y _ {n} (\omega) | \geq \varepsilon \}) \geq \lim _ {k \to \infty} P (\{\omega : | Y _ {k} (\omega) | \geq \varepsilon \})
$$

and by Lemma 8.2 the limit on the left is zero hence so is that on the right. 

Note that the two sides of the inequality neatly summarize the diference between convergence a.s. and in probability. For convergence in probability we consider the probabilities that individual $Y _ { n }$ are at least ε away from the limit, while for almost sure convergence we need to consider the whole tail sequence $( Y _ { n } ) _ { n \geq k }$ simultaneously. 

The following example shows that the implication in the above theorem cannot be reversed and also shows that the convergence in $L ^ { p }$ does not imply almost sure convergence. 

## Example 8.2

Consider the following sequence of random variables defined on $\varOmega \ = \ [ 0 , 1 ]$ with Lebesgue measure: $Y _ { 1 } = \mathbf { 1 } _ { [ 0 , 1 ] } , Y _ { 2 } = \mathbf { 1 } _ { [ 0 , 1 / 2 ] } , Y _ { 3 } = \mathbf { 1 } _ { [ 1 / 2 , 1 ] } , Y _ { 4 } = \mathbf { 1 } _ { [ 0 , 1 / 4 ] }$ $Y _ { 5 } = \mathbf { 1 } _ { [ 1 / 4 , 1 / 2 ] }$ and so on (like in the proof of Theorem 8.1). The sequence clearly converges to zero in probability and in $L ^ { p }$ but for each $\omega \in [ 0 , 1 ] , Y _ { n } ( \omega ) = 1$ for infinitely many n, so it fails to converge pointwise. 

Convergence in probability has an additional useful feature: 

## Proposition 8.4

The function defined by $\begin{array} { r } { d ( X , Y ) = \mathbb { E } ( \frac { | X - Y | } { 1 + | X - Y | } ) } \end{array}$ is a metric and convergence in d is equivalent to convergence in probability. 

Hint If $X _ { n } \ \to \ X$ in probability then decompose the expectation into $\textstyle { \int _ { A } + \int _ { \Omega \backslash A } }$ where $A = \{ \omega : | X _ { n } ( \omega ) - X ( \omega ) | < \varepsilon \}$ 

We now give a basic estimate of the probability of a non-negative random variable taking values in a given set by means of the moments of this random variable. 

## Theorem 8.5 (Chebyshev’s Inequality)

If Y is a non-negative random variable, $\varepsilon > 0 , 0 < p < \infty$ , then 

$$
P (Y \geq \varepsilon) \leq \frac {\mathbb {E} (Y ^ {p})}{\varepsilon^ {p}}.\tag{8.1}
$$

## Proof

This is immediate from basic properties of integral: let $A = \{ \omega : Y ( \omega ) \geq \varepsilon \}$ 

and then 

$$
\begin{array}{l l} \mathbb {E} (Y ^ {p}) \geq \int_ {A} Y ^ {p}   \mathrm{d} P & \text {(integration over a smaller set)} \\ \geq P (A) \cdot \varepsilon^ {p} \end{array}
$$

since $Y ^ { p } ( \omega ) > \varepsilon ^ { p }$ on A, which gives the result after dividing by $\varepsilon ^ { p }$ 

Chebyshev’s inequality will be used mainly with small ε. But let us see what happens if ε is large. 

## Proposition 8.6

Assume that $\mathbb { E } ( Y ^ { p } ) < \infty$ . Then 

$$
\varepsilon^ {p} P (Y \geq \varepsilon) \rightarrow 0 \quad \mathrm{as} \varepsilon \rightarrow \infty .
$$

Hint Write 

$$
\mathbb {E} (Y ^ {p}) = \int_ {\{\omega : Y (\omega) \geq \varepsilon \}} Y ^ {p} \mathrm{d} P + \int_ {\{\omega : Y (\omega) <   \varepsilon \}} Y ^ {p} \mathrm{d} P
$$

and estimate the first term as in the proof of Chebyshev’s inequality. 

## Corollary 8.7

Let X be a random variable with finite expectation $\mathbb { E } ( X ) = m$ and variance $\sigma ^ { 2 }$ . Let $0 < a < \infty ;$ then 

$$
P (| X - m | \geq a \sigma) \leq \frac {1}{a ^ {2}}.
$$

## Proof

Using Chebyshev’s inequality with $Y = | X - m |$ and $p = 2 , \varepsilon = a \sigma$ we find that 12 

$$
P (| X - m | \geq a \sigma) \leq \frac {\mathbb {E} (| X - m | ^ {2})}{a ^ {2} \sigma^ {2}} = \frac {1}{a ^ {2}}
$$

as required. 

## Remark 8.2

Chebyshev’s inequality also shows that convergence in $L ^ { p }$ implies convergence in probability. For, let $Y _ { n } = | X _ { n } - X |$ and assume that $\| X _ { n } - X \| _ { p } \to 0$ . This implies that $P ( Y _ { n } \ \geq \ \varepsilon )  \ 0$ . The converse is false in general, as the next example shows. 

## Example 8.3

Let $\varOmega = [ 0 , 1 ]$ with Lebesgue measure and let $X _ { n } = n \mathbf { 1 } _ { [ 0 , \frac { 1 } { n } ] }$ . The sequence $X _ { n }$ converges to 0 pointwise so we take $X = 0$ and we see that $\| X _ { n } - X \| _ { p } =$ $\begin{array} { r } { \int _ { 0 } ^ { \frac { 1 } { n } } n ^ { p } \mathrm { d } m = n ^ { p - 1 } } \end{array}$ . If $p \geq 1$ , then $\| X _ { n } - X \| _ { p } \not \to 0$ , however as we have already Rseen (Exercise 8.2), 

$$
P (| X _ {n} - X | \geq \varepsilon) = P (X _ {n} = n) = \frac {1}{n} \rightarrow 0
$$

showing that $X _ { n } \to X$ in probability. 

## 8.2.2 Weak law of large numbers

The simplest ‘law of large numbers’ provides an $L ^ { 2 } .$ -convergence result: 

## Theorem 8.8

If $X _ { 1 } , X _ { 2 } , . . .$ . are independent, E $\therefore ( X _ { i } ) = m , \mathrm { V a r } ( X _ { i } ) \leq K < \infty$ , then $\begin{array} { r } { \frac { S _ { n } } { n }  m } \end{array}$ in $L ^ { 2 }$ and hence in probability. 

## Proof

First note that $\mathfrak { T } ( S _ { n } ) = \mathbb { E } ( X _ { 1 } ) + \cdot \cdot \cdot + \mathbb { E } ( X _ { n } ) = n m$ by the linearity of expectation. Hence $\begin{array} { r } { \mathbb { E } ( \frac { S _ { n } } { n } ) = m } \end{array}$ and so E $\begin{array} { r } { ( \frac { S _ { n } } { n } - m ) ^ { 2 } = \mathrm { V a r } ( \frac { S _ { n } } { n } ) } \end{array}$ . By the properties of the variance (Proposition 5.20) 

$$
\operatorname{Var} \left(\frac {S _ {n}}{n}\right) = \frac {1}{n ^ {2}} \operatorname{Var} \left(S _ {n}\right) = \frac {1}{n ^ {2}} \left(\operatorname{Var} \left(X _ {1}\right) + \dots + \operatorname{Var} \left(X _ {n}\right)\right) \leq \frac {1}{n ^ {2}} n K = \frac {K}{n} \rightarrow 0
$$

as $n  \infty$ . This in turn implies convergence in probability as we saw in Remark 8.2. □ 

## Exercise 8.4

Using Chebyshev’s inequality find a lower bound for the probability that the average number of heads in 100 tosses of a coin difers from $\textstyle { \frac { 1 } { 2 } }$ by 0.1. 

## Exercise 8.5

Find a lower bound for the probability that the average number shown on a die in 1000 tosses difers from 3.5 by 0.01. 

We give some classical applications of the weak law of large numbers. The Weierstrass theorem says that every continuous function can be uniformly approximated by polynomials. The Chebyshev inequality provides an easy proof. 

## Theorem 8.9 (Bernstein–Weierstrass Approximation Theorem)

If $f : [ 0 , 1 ] \to \mathbb { R }$ is continuous then the sequence of Bernstein polynomials 

$$
f _ {n} (x) = \sum_ {k = 0} ^ {n} {\binom {n} {k}} x ^ {k} (1 - x) ^ {n - k} f (\frac {k}{n})
$$

converges to f uniformly. 

## Proof

The number $f _ { n } ( x )$ has a probabilistic meaning. Namely, $\begin{array} { r } { f _ { n } ( x ) \ = \ \mathbb { E } ( f ( \frac { S _ { n } } { n } ) ) } \end{array}$ where $S _ { n } = X _ { 1 } + \cdot \cdot \cdot + X _ { n }$ 2 

$$
X _ {i} = \left\{ \begin{array}{l l} 1 & \mathrm{withprobability} x \\ 0 & \mathrm{withprobability} 1 - x. \end{array} \right.
$$

Then writing $\mathbb { E } _ { x }$ instead of E to emphasize the fact that the underlying probability depends on x, we have 

$$
\begin{array}{c} \sup _ {x \in [ 0, 1 ]} | f _ {n} (x) - f (x) | \leq \sup _ {x \in [ 0, 1 ]} | \mathbb {E} _ {x} (f (\frac {S _ {n}}{n})) - f (x) | \\ \leq \sup _ {x \in [ 0, 1 ]} \mathbb {E} _ {x} | f (\frac {S _ {n}}{n}) - f (x) |. \end{array}
$$

Take any $\varepsilon > 0$ and find $\delta > 0$ such that if $| x - y | < \delta$ then $\begin{array} { r } { | f ( x ) - f ( y ) | < \frac { \varepsilon } { 2 } } \end{array}$ (this is possible since f is uniformly continuous). 

$$
\begin{array}{l} \mathbb {E} _ {x} | f (\frac {S _ {n}}{n}) - f (x) | = \int_ {\{\omega : | \frac {S _ {n}}{n} - x | <   \delta \}} | f (\frac {S _ {n}}{n}) - f (x) |   \mathrm{d} P \\ \qquad + \int_ {\{\omega : | \frac {S _ {n}}{n} - x | \geq \delta \}} | f (\frac {S _ {n}}{n}) - f (x) |   \mathrm{d} P \\ \qquad \leq \frac {\varepsilon}{2} + 2 \sup _ {x \in [ 0, 1 ]} | f (x) | \cdot P (| \frac {S _ {n}}{n} - x | \geq \delta). \end{array}
$$

The last term converges to zero by the law of large numbers since $\begin{array} { r } { x = \mathbb { E } ( \frac { S _ { n } } { n } ) } \end{array}$ 2 and $\operatorname { V a r } ( { \frac { S _ { n } } { n } } )$ is finite. This convergence is uniform in x: 

$$
P (| \frac {S _ {n}}{n} - x | \geq \delta) \leq \frac {\mathrm{Var} (\frac {S _ {n}}{n})}{\delta^ {2}} = \frac {x (1 - x)}{n \delta^ {2}} \leq \frac {1}{4 n \delta^ {2}}
$$

(due to $4 x ( 1 - x ) \leq 1$ and $\operatorname { V a r } ( S _ { n } ) = n \operatorname { V a r } ( X _ { i } ) = n x ( 1 - x ) \ )$ . So, for suficiently large n the right-hand side is less than ε which completes the proof. □ 

In many practical situations it is impossible to compute integrals (in particular areas or volumes) directly. The law of large numbers is the basis of the so-called Monte Carlo method which gives an approximate solution by random selection of points. The next two examples illustrate this method. 

## Example 8.4

We restrict ourselves to $F \subset [ 0 , 1 ] \times [ 0 , 1 ]$ for simplicity. Assume that $F$ is Lebesgue measurable and our goal is to find its measure. Let $X _ { n } , Y _ { n }$ be independent, uniformly distributed in [0, 1]. Let $\begin{array} { r } { M _ { n } = \frac { 1 } { n } \sum _ { k = 1 } ^ { n } \mathbf { 1 } _ { F } ( X _ { k } , Y _ { k } ) } \end{array}$ . If we Pdraw the pairs of numbers n times, then this sum gives the number of hits of the set F, and $M _ { n } \to m ( F )$ in probability. To see this first observe that $\mathbb { E } ( \mathbf { 1 } _ { F } ( X _ { k } , Y _ { k } ) ) = P ( ( X _ { k } , Y _ { k } ) \in F ) = m ( F )$ by the assumption on the distribution of $X _ { k } , ~ Y _ { k }$ : independence guarantees that the distribution of the pair is two-dimensional Lebesgue measure restricted to the square. Then 

$$
P (| M _ {n} - m (F) | \geq \varepsilon) \leq \frac {m (F)}{n \varepsilon} \to 0.
$$

A similar example illustrates the use of the Monte Carlo method for computing integrals. 

## Example 8.5

Let $f$ be an integrable function defined on [0, 1]. With $X _ { n }$ independent uniformly distributed on [0, 1] we take 

$$
I _ {n} = \frac {1}{n} \sum_ {k = 1} ^ {n} f (X _ {k})
$$

and we show that 

$$
I _ {n} \rightarrow \int_ {0} ^ {1} f (x) \mathrm{d} x
$$

in probability. First note that the distribution of $X _ { k }$ is Lebesgue measure on [0,1] hence 

$$
\mathbb {E} (f (X _ {k})) = \int f (x) d P _ {X _ {k}} (x) = \int_ {0} ^ {1} f (x) \mathrm{d} x,
$$

and so $\begin{array} { r } { \mathbb { E } ( I _ { n } ) = \int _ { 0 } ^ { 1 } f ( x ) } \end{array}$ dx. The weak law provides the desired convergence. 

$$
P (| I _ {n} - \int_ {0} ^ {1} f (x) \mathrm{d} x | \geq \varepsilon) \rightarrow 0.
$$

We return to considering further weak laws of large numbers for sequences of random variables. The assumption that $\mathbb { E } ( X _ { k } )$ and $\mathrm { V a r } ( X _ { k } )$ are finite can be relaxed. There is, however, a price to pay by imposing additional conditions. 

First we introduce some convenient notation. For a given sequence of random variables $( X _ { k } ) _ { k \geq 1 }$ introduce the truncated random variables 

$$
X _ {k} (n) = X _ {k} \cdot \mathbf {1} _ {\{\omega : | X _ {k} (\omega) | \leq n \}}
$$

and set $m _ { n } = \mathbb { E } ( X _ { 1 } ( n ) )$ . Note that $m _ { n } = \mathbb { E } ( X _ { k } ( n )$ for all $k \geq 1$ since the distributions of all $X _ { k }$ are the same. Also write 

$$
\hat {S} _ {m} = X _ {1} (n) + \dots + X _ {m} (n)
$$

for all $m \geq 1$ 

## Theorem 8.10

If $X _ { k }$ are independent identically distributed random variables such that 

$$
a P (| X _ {1} | > a) \rightarrow 0 \quad \text { as } a \rightarrow \infty ,\tag{8.2}
$$

then 

$$
\frac {S _ {n}}{n} - m _ {n} \rightarrow 0 \quad \mathrm{inprobability}.\tag{8.3}
$$

We shall need the following lemma which is of interest in itself and will be useful in what follows. 

Lemma 8.11 

If $Y \ge 0 , Y \in L ^ { p } , 0 < p < \infty$ , then 

$$
\mathbb {E} (Y ^ {p}) = \int_ {0} ^ {\infty} p y ^ {p - 1} P (Y > y) \mathrm{d} y.
$$

In particular $( p = 1 )$ 

$$
\mathbb {E} (Y) = \int_ {0} ^ {\infty} P (Y > y) \mathrm{d} y.
$$

## Proof (of the Lemma)

This is a simple application of Fubini’s theorem: 

$$
\begin{array}{l} \int_ {0} ^ {\infty} p y ^ {p - 1} P (Y > y) \mathrm{d} y \\ = \int_ {0} ^ {\infty} \int_ {\Omega} p y ^ {p - 1} \mathbf {1} _ {\{\omega : Y (\omega) > y \}} (\omega) \mathrm{d} P (\omega) \mathrm{d} y \\ = \int_ {\Omega} \int_ {0} ^ {\infty} p y ^ {p - 1} \mathbf {1} _ {\{\omega : Y (\omega) > y \}} (\omega) \mathrm{d} y \mathrm{d} P (\omega) \quad \text {(by Fubini)} \\ = \int_ {\Omega} \int_ {0} ^ {Y (\omega)} p y ^ {p - 1} \mathrm{d} y \mathrm{d} P (\omega) \\ = \int_ {\Omega} Y ^ {p} (\omega) \mathrm{d} P (\omega) \quad \text {(computing the inner integral, \omega fixed)} \\ = \mathbb {E} (Y ^ {p}) \end{array}
$$

as required. 

## Proof (of the Theorem)

Take $\varepsilon > 0$ and obviously 

$$
P (| \frac {S _ {n}}{n} - m _ {n} | \geq \varepsilon) \leq P (| \frac {\hat {S} _ {n}}{n} - m _ {n} | \geq \varepsilon) + P (\hat {S} _ {n} \neq S _ {n}).
$$

We estimate the first term 

$$
\begin{array}{r l} & P (| \frac {\hat {S} _ {n}}{n} - m _ {n} | \geq \varepsilon) \leq \frac {E (| \frac {\hat {S} _ {n}}{n} - m _ {n} | ^ {2})}{\varepsilon^ {2}} \quad (\text {by Chebyshev}) \\ & \qquad = \frac {E (| \sum X _ {k} (n) - n m _ {n} | ^ {2})}{n ^ {2} \varepsilon^ {2}} \\ & \qquad = \frac {\operatorname{Var} (\sum X _ {k} (n))}{n ^ {2} \varepsilon^ {2}}. \end{array}
$$

Note that the truncated random variables are independent, being functions of 

the original ones, hence we may continue the estimation: 

$$
\begin{array}{l} \leq \frac {\sum_ {k} \operatorname{Var} (X _ {k} (n))}{n ^ {2} \varepsilon^ {2}} \\ = \frac {\operatorname{Var} (X _ {1} (n))}{n \varepsilon^ {2}} \quad (\text {as Var} (X _ {k} (n)) \text {are the same}) \\ \leq \frac {\mathbb {E} (X _ {1} ^ {2} (n))}{n \varepsilon^ {2}} \quad (\text {by Var} (Z) = \mathbb {E} (Z ^ {2}) - (\mathbb {E} Z) ^ {2} \leq \mathbb {E} (Z ^ {2})) \\ = \frac {1}{n \varepsilon^ {2}} \int_ {0} ^ {\infty} 2 y P (| X _ {1} (n) | > y)   \mathrm{d} y \quad (\text {by the Lemma for p = 2}) \\ = \frac {1}{n \varepsilon^ {2}} \int_ {0} ^ {n} 2 y P (| X _ {1} | > y)   \mathrm{d} y. \end{array}
$$

The function $y \mapsto 2 y P ( | X _ { 1 } | > y )$ converges to 0 as $y  \infty$ by hypothesis, hence for given $\delta > 0$ there is $y _ { 0 }$ such that for $y \geq y _ { 0 }$ this quantity is less than $\scriptstyle { \frac { 1 } { 2 } } \delta \varepsilon ^ { 2 }$ , and we have 

$$
\begin{array}{l} = \frac {1}{n \varepsilon^ {2}} \int_ {0} ^ {y _ {0}} 2 y P (| X _ {1} | > y)   \mathrm{d} y + \frac {1}{n \varepsilon^ {2}} \int_ {y _ {0}} ^ {n} 2 y P (| X _ {1} | > y)   \mathrm{d} y \\ \leq \frac {1}{n \varepsilon^ {2}} y _ {0} \max _ {y \in [ 0, \infty ]} \{y P (| X _ {1} | > y) \} + \frac {1}{n \varepsilon^ {2}} n \frac {\delta \varepsilon^ {2}}{2} \\ \leq \delta \end{array}
$$

provided $n$ is suficiently large. So the first term converges to 0. Now we tackle the second term: 

$$
\begin{array}{l}P (\hat {S} _ {n} \neq S _ {n}) \leq P (X _ {k} (n) \neq X _ {k} \text {   for   some   } k \leq n)\\\quad \leq \sum_ {k = 1} ^ {n} P (X _ {k} (n) \neq X _ {k}) \quad \text {(by subadditivity of   } P)\\\quad = n P (X _ {1} (n) \neq X _ {1}) \quad \text {(the same distributions)}\\\quad = n P (| X _ {1} | > n)\\\quad \rightarrow 0 \quad \text { by   hypothesis. }\end{array}
$$

This completes the proof. 

□ 

## Remark 8.3

Note that we cannot generalize the last theorem to the case of uncorrelated random variables since we made essential use of the independence. Although the identity 

$$
\operatorname{Var} \left(\sum X _ {k} (n)\right) = \sum \operatorname{Var} (X _ {k} (n))
$$

holds for uncorrelated random variable, we needed the independence of the $( X _ { k } )$ — which implies that of the $\left( X _ { k } ( n ) \right) \ -$ to conclude that the truncated random variables are uncorrelated. 

## Theorem 8.12

If $X _ { n }$ are independent and identically distributed, $\mathbb { E } ( | X _ { 1 } | ) < \infty$ , then (8.2) is satisfied, $m _ { n } \to m = \mathbb { E } ( X _ { 1 } )$ and $\begin{array} { r } { \frac { S _ { n } } { n }  } \end{array}$ m in probability. (Note that we do not assume here that $X _ { 1 }$ has finite variance.) 

## Proof

The finite expectation of $| X _ { 1 } |$ gives condition (8.2): 

$$
\begin{array}{l} a P (| X _ {1} | > a) = a \int_ {\Omega} \mathbf {1} _ {\{\omega : | X _ {1} (\omega) | > a \}}   \mathrm{d} P \\ \qquad \leq \int_ {\Omega} | X _ {1} | \mathbf {1} _ {\{\omega : | X _ {1} (\omega) | > a \}}   \mathrm{d} P \\ \qquad = \int_ {\{\omega : | X _ {1} (\omega) | > a \}} | X _ {1} |   \mathrm{d} P \\ \qquad \to 0 \end{array}
$$

as $a  \infty$ by the dominated convergence theorem. Hence $\begin{array} { r } { \frac { S _ { n } } { n } - m _ { n } \to 0 } \end{array}$ but $m _ { n } = \mathbb { E } ( X _ { 1 } \mathbf { 1 } _ { \left\{ \omega : | X _ { 1 } ( \omega ) | \leq n \right\} } ) \longrightarrow \mathbb { E } ( X _ { 1 } )$ as $n \to \infty$ so the result follows. □ 

## 8.2.3 The Borel–Cantelli Lemmas

The idea that a point $\omega \in \Omega$ belongs to ‘infinitely many’ events of a given sequence $\left( A _ { n } \right) \subset { \mathcal { F } }$ can easily be made precise: for every $n \geq 1$ we need to be able to find an $m _ { n } \geq n$ such that $\omega \in A _ { m _ { n } }$ . This identifies a subsequence $( m _ { n } )$ of indices such that for each $n \geq 1 , \omega \in A _ { m _ { n } } ,$ i.e. $\textstyle \omega \in \bigcup _ { m \geq n } A _ { m }$ for every $n \geq 1$ . Thus we say that $\omega \in A _ { n }$ infinitely often, and write $\omega \in A _ { n } \operatorname { i . o . }$ 2 if $\textstyle \omega \in \bigcap _ { n = 1 } ^ { \infty } \bigcup _ { m = n } ^ { \infty } A _ { m }$ . We call this set the upper limit of the sequence $\left( A _ { n } \right)$ T Sand write it as 

$$
\limsup _ {n \to \infty} A _ {n} = \bigcap_ {n = 1} ^ {\infty} \bigcup_ {m = n} ^ {\infty} A _ {m}.
$$

## Exercise 8.6

Find lim $\operatorname* { s u p } _ { n \to \infty } A _ { n }$ for a sequence $\begin{array} { r } { A _ { 1 } = [ 0 , 1 ] , A _ { 2 } = [ 0 , \frac { 1 } { 2 } ] , A _ { 3 } = [ \frac { 1 } { 2 } , 1 ] } \end{array}$ 2 $\begin{array} { r } { A _ { 4 } = [ 0 , \frac { 1 } { 4 } ] , A _ { 5 } = [ \frac { 1 } { 4 } , \frac { 1 } { 2 } ] } \end{array}$ etc. 

Given $\varepsilon > 0$ , a sequence of random variables $( X _ { n } )$ and a random variable $X$ , for each n set $A _ { n } = \left\{ \left| X _ { n } - X \right| > \varepsilon \right\}$ . Then $\omega \in A _ { n } \quad \mathrm { i . o }$ . precisely when for every $\varepsilon > 0 , \ | X _ { n } ( \omega ) - X ( \omega ) | > \varepsilon$ occurs for all elements of an infinite subsequence $( m _ { n } )$ of indices, which means that $( X _ { n } )$ fails to converge to $X$ Hence it follows that 

$$
X _ {n} \longrightarrow X \text { a.s. } (P) \quad \Longleftrightarrow \quad \forall \varepsilon > 0 P (\limsup _ {n \to \infty} A _ {n}) = P (| X _ {n} - X | > \varepsilon \text { i.o. }) = 0.
$$

Similarly, define 

$$
\liminf _ {n \to \infty} A _ {n} = \bigcup_ {n = 1} ^ {\infty} \bigcap_ {m = n} ^ {\infty} A _ {n}.
$$

(We say that this set is the lower limit of the sequence $( A _ { n } ) . )$ 

Proposition 8.13 

(i) We have $\omega \in \operatorname* { l i m } \operatorname* { i n f } _ { n \to \infty } A _ { n }$ if and only if $\omega \in A _ { n }$ except for finitely many n. (We say that $\omega \in A _ { n }$ eventually.) 

(ii) P(X<sub>n</sub> X) = lim<sub>ε 0</sub> P( X<sub>n</sub> X < ε eventually). 

(iii) If $A = \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } A _ { n }$ then $A ^ { c } = \operatorname* { l i m } \operatorname* { i n f } _ { n \to \infty } A _ { n } ^ { c }$ 

(iv) For any sequence $\left( A _ { n } \right)$ of events, $P ( \{ \omega \in A _ { n } { \mathrm { ~ e v . } } \} ) \leq P ( \{ \omega \in A _ { n } { \mathrm { ~ i . o . } } \} )$ 

Hint: Use Fatou’s lemma on the indicator functions of the sets in (iv). 

The sets lim in $\operatorname { f } _ { n  \infty } A _ { n }$ and lim $\operatorname* { s u p } _ { n \to \infty } A _ { n }$ are ‘tail events’ of the sequence $\left( A _ { n } \right)$ : we can only determine whether a point belongs to them by knowing the whole sequence. It is frequently true that the probability of a tail event is either 0 or 1 - such results are known as $0 - 1$ laws. The simplest of these is provided by combining the two ‘Borel-Cantelli lemmas’ to which we now turn: together they show that for a sequence of independent events $\left( A _ { n } \right)$ , lim $\operatorname* { s u p } _ { n \to \infty } A _ { n }$ has either probability 0 or 1, depending on whether the series of their individual probabilities converges or diverges. In the first case, we do not even need independence, but can prove the result in general. 

Exercise 8.7 

Let $S _ { n } = X _ { 1 } + X _ { 2 } + \ldots + X _ { n } $ describe the position after n steps of a symmetric random walk on $\mathbb { Z } ^ { d }$ . Using the asymptotic formula: $n ! \sim$ $\left( { \textstyle { \frac { n } { e } } } \right) ^ { n } { \sqrt { 2 \pi n } }$ and the Borel-Cantelli lemmas show that the probability of $\{ S _ { n } = 0 \ \mathrm { i . o . } \}$ is 1 when $d = 1 , 2$ and 0 for $d > 2$ 

We have the following simple but fundamental fact. 

Theorem 8.14 (Borel–Cantelli Lemma) 

If 

$$
\sum_ {n = 1} ^ {\infty} P (A _ {n}) <   \infty
$$

then 

$$
P (\limsup _ {n \to \infty} A _ {n}) = 0
$$

i.e. $\textstyle { \mathfrak { c } } _ { \omega } \in A _ { n }$ for infinitely many $n ^ { \prime }$ occurs only with probability zero. 

## Proof

First note that lim $\textstyle \operatorname* { s u p } _ { n \to \infty } A _ { n } \subset \bigcup _ { n = k } ^ { \infty } A _ { n }$ hence 

$$
\begin{array}{l l}P (\limsup _ {n \to \infty} A _ {n}) \leq P (\bigcup_ {n = k} ^ {\infty} A _ {n})&\text {(for all k)}\\\leq \sum_ {n = k} ^ {\infty} P (A _ {n})&\text {(by subadditivity)}\\\rightarrow 0\end{array}
$$

since the tail of a convergent series converges to 0. 

The basic application of the lemma provides a link between almost sure convergence and convergence in probability. 

## Theorem 8.15

If $X _ { n } \to X$ in probability then there is a subsequence $X _ { k _ { n } }$ converging to X almost surely. 

## Proof

We have to find a set of full measure on which a subsequence would converge. So the set on which the behaviour of the whole sequence is ‘bad’ should be of measure zero. For this we employ the Borel–Cantelli lemma whose conclusion is precisely that. So we introduce the sequence $A _ { n }$ encapsulating the ‘bad behaviour of $X _ { n }$ , which from the point of convergence is expressed by inequalities of the type $| X _ { n } ( \omega ) - X ( \omega ) | > a$ . Specifically, we take $a = 1$ and since $P ( | X _ { n } - X | > 1 ) \to 0$ we find $k _ { 1 }$ such that 

$$
P (| X _ {n} - X | > 1) <   1
$$

for $n \geq k _ { 1 }$ . Next for $\begin{array} { r } { a = \frac { 1 } { 2 } } \end{array}$ we find $k _ { 2 } > k _ { 1 }$ such that for all $n \geq k _ { 2 }$ 

$$
P (| X _ {n} - X | > \frac {1}{2}) <   \frac {1}{4}.
$$

We continue that process obtaining an increasing sequence of integers $k _ { n }$ with 

$$
P (| X _ {k _ {n}} - X | > \frac {1}{n}) <   \frac {1}{n ^ {2}}.
$$

The series $\textstyle \sum _ { n = 1 } ^ { \infty } P ( A _ { n } )$ converges, where $\begin{array} { r } { A _ { n } = \{ \omega : | X _ { k _ { n } } ( \omega ) - X ( \omega ) | > \frac { 1 } { n } \} } \end{array}$ hence $A =$ Plim sup $A _ { n }$ has probability zero. 

We observe that for $\omega \in \varOmega \setminus A$ , lim sup $X _ { k _ { n } } ( \omega ) = X ( \omega )$ . For, if $\omega \in \varOmega \setminus A$ then for some k, $\omega \in \bigcap _ { n = k } ^ { \infty } ( { \mathcal { \Omega } } \setminus A _ { n } )$ so for all $\begin{array} { r } { n \geq k , | X _ { k _ { n } } ( \omega ) - X ( \omega ) | \leq \frac { 1 } { n } , } \end{array}$ Thence we have obtained the desired convergence. □ 

The second Borel–Cantelli lemma partially completes the picture. Under the additional condition of independence it shows when the probability that infinitely many events occur is one. 

## Theorem 8.16

Suppose that the events $A _ { n }$ are independent. We have 

$$
\sum_ {n = 1} ^ {\infty} P (A _ {n}) = \infty \quad \Rightarrow \quad P (\limsup _ {n \to \infty} A _ {n}) = 1.
$$

## Proof

It is suficient to show that for all k 

$$
P (\bigcup_ {n = k} ^ {\infty} A _ {n}) = 1
$$

since then the intersection over k will also have probability 1. Fix k and consider the partial union up to $m > k$ . The complements of $A _ { n }$ are also independent hence 

$$
P (\bigcap_ {n = k} ^ {m} A _ {n} ^ {\mathrm{c}}) = \prod_ {n = k} ^ {m} P (A _ {n} ^ {\mathrm{c}}) = \prod_ {n = k} ^ {m} (1 - P (A _ {n})).
$$

Since $1 - x \leq \mathrm { e } ^ { - x }$ 

$$
\prod_ {n = k} ^ {m} (1 - P (A _ {n})) \leq \prod_ {n = k} ^ {m} \mathrm{e} ^ {- P (A _ {n})} = \exp (- \sum_ {n = k} ^ {m} P (A _ {n})).
$$

The last expression converges to 0 as $m \to \infty$ by the hypothesis, hence 

$$
P (\bigcap_ {n = k} ^ {m} A _ {n} ^ {\mathrm{c}}) \to 0
$$

but 

$$
P (\bigcap_ {n = k} ^ {m} A _ {n} ^ {\mathrm{c}}) = P (\Omega \setminus \bigcup_ {n = k} ^ {m} A _ {n}) = 1 - P (\bigcup_ {n = k} ^ {m} A _ {n}).
$$

The sets $\textstyle B _ { m } = \bigcup _ { n = k } ^ { m } A _ { n }$ form an increasing chain with $\textstyle \bigcup _ { m = k } ^ { \infty } B _ { m } = \bigcup _ { n = k } ^ { \infty } A _ { n }$ and so $P ( B _ { m } )$ S S, which as we know converges to 1, converges to $\textstyle P ( \bigcup _ { n = k } ^ { \infty } A _ { n } )$ Thus this quantity is also equal to 1. □ 

Below we discuss strong laws of large numbers, where convergence in probability is strengthened to almost sure convergence. But already we can observe some limitations of these improvements. Drawing on the second Borel–Cantelli lemma we give a negative result. 

## Theorem 8.17

Suppose that $X _ { 1 } , X _ { 2 } , \ldots$ . are independent identically distributed random variables and assume that $\mathbb { E } ( | X _ { 1 } | ) = \infty$ (hence also $\mathbb { E } ( | X _ { n } | ) = \infty$ for all n). Then (i) $P ( \{ \omega : | X _ { n } ( \omega ) | \ge n \}$ for infinitely many $n \} ) = 1$ 2 

(ii) $\scriptstyle P ( \operatorname* { l i m } _ { n \to \infty } { \frac { S _ { n } } { n } }$ exists and is finite) = 0. 

Proof 

(i) First 

$$
\begin{array}{l} \mathbb {E} (| X _ {1} |) = \int_ {0} ^ {\infty} P (| X _ {1} | > x) \mathrm{d} x \quad (\text { by   Lemma   8.11 }) \\ = \sum_ {k = 0} ^ {\infty} \int_ {k} ^ {k + 1} P (| X _ {1} | > x) \mathrm{d} x \quad (\text { countable   additivity }) \\ \leq \sum_ {k = 0} ^ {\infty} P (| X _ {1} | > k) \end{array}
$$

because the function $x \mapsto P ( | X _ { 1 } | > x )$ reaches its maximum on $[ k , k + 1 ]$ for $x = k$ since $\{ \omega : | X _ { 1 } ( \omega ) | > k \} \supset \{ \omega : | X _ { 1 } ( \omega ) | > x \}$ if $x \geq k$ . By the hypothesis this series is divergent, but $P ( | X _ { 1 } | > k ) = P ( | X _ { k } | > k )$ as the distributions are identical, so 

$$
\sum_ {k = 0} ^ {\infty} P (| X _ {k} | > k) = \infty .
$$

The second Borel–Cantelli lemma is applicable yielding the claim. 

(ii) Denote by A the set where the limit of $\scriptstyle { \frac { S _ { n } } { n } }$ exists (and is finite). Some elementary algebra of fractions gives 

$$
\frac {S _ {n}}{n} - \frac {S _ {n + 1}}{n + 1} = \frac {(n + 1) S _ {n} - n S _ {n + 1}}{n (n + 1)} = \frac {S _ {n} - n X _ {n + 1}}{n (n + 1)} = \frac {S _ {n}}{n (n + 1)} - \frac {X _ {n + 1}}{n + 1}.
$$

For any $\omega _ { 0 } \in A$ the left-hand side converges to zero and also 

$$
\frac {S _ {n} (\omega_ {0})}{n (n + 1)} \rightarrow 0.
$$

Hence also $\frac { X _ { n + 1 } ( \omega _ { 0 } ) } { n + 1 }  0$ . This means that 

ω<sub>0</sub> $\notin \{ \omega : | X _ { k } ( \omega ) | > k$ for infinitely many $k \} = B$ 

say, so $A \subset \varOmega \setminus B$ . But $P ( B ) = 1$ by (i), hence $P ( A ) = 0$ 

## 8.2.4 Strong law of large numbers

We shall consider several versions of the strong law of large numbers, first by imposing additional conditions on the moments of the sequence $( X _ { n } )$ , and then gradually relaxing these we arrive at Theorem 8.21, which provides the most general positive result. 

The first result is due to von Neumann. Note that we do not impose the condition that the $X _ { n }$ have identical distributions. The price we pay is having to assume that higher order moment are finite. However, for many familiar random variables, Gaussian for example, this is not a serious restriction. 

## Theorem 8.18

Suppose that the random variables $X _ { n }$ are independent, $\mathbb { E } ( X _ { n } ) ~ = ~ m$ , and $\mathbb { E } ( X _ { n } ^ { 4 } ) \le K$ . Then 

$$
{\frac {S _ {n}}{n}} = {\frac {1}{n}} \sum_ {k = 1} ^ {n} X _ {k} \rightarrow m \quad {\mathrm{a.s.}}
$$

Proof 

By considering $X _ { n } - m$ we may assume that $\mathbb { E } ( X _ { n } ) = 0$ for all n. This simplifies 

the following computation 

$$
\begin{array}{l} \mathbb {E} (S _ {n} ^ {4}) = \mathbb {E} \left(\sum_ {k = 1} ^ {n} X _ {k}\right) ^ {4} \\ = \mathbb {E} \left(\sum_ {k = 1} ^ {n} X _ {k} ^ {4} + \sum_ {i \neq j} X _ {i} ^ {2} X _ {j} ^ {2} + \sum_ {i \neq j} X _ {i} X _ {j} X _ {k} ^ {2} \right. \\ \left. + \sum_ {i, j, k, l \text {   distinct }} X _ {i} X _ {j} X _ {k} X _ {l}\right). \end{array}
$$

The last two terms vanish by independence: 

$$
\mathbb {E} (\sum_ {i \neq j} X _ {i} X _ {j} X _ {k} ^ {2}) = \sum_ {i \neq j} \mathbb {E} (X _ {i} X _ {j} X _ {k} ^ {2}) = \sum_ {i \neq j} \mathbb {E} (X _ {i}) \mathbb {E} (X _ {j}) \mathbb {E} (X _ {k} ^ {2}) = 0
$$

and similarly for the term with all indices distinct 

$$
\begin{array}{c} \mathbb {E} (\sum X _ {i} X _ {j} X _ {k} X _ {l}) = \sum \mathbb {E} (X _ {i} X _ {j} X _ {k} X _ {l}) \\ = \sum \mathbb {E} (X _ {i}) \mathbb {E} (X _ {j}) \mathbb {E} (X _ {k}) \mathbb {E} (X _ {l}) = 0. \end{array}
$$

The first term is easily estimated by the hypothesis 

$$
\mathbb {E} (\sum X _ {k} ^ {4}) = \sum \mathbb {E} (X _ {k} ^ {4}) \leq n K.
$$

To the remaining term we first apply the Schwarz inequality 

$$
\mathbb {E} (\sum_ {i \neq j} X _ {i} ^ {2} X _ {j} ^ {2}) = \sum_ {i \neq j} \mathbb {E} (X _ {i} ^ {2} X _ {j} ^ {2}) \leq \sum_ {i \neq j} \sqrt {\mathbb {E} (X _ {i} ^ {4})} \sqrt {\mathbb {E} (X _ {j} ^ {4})} \leq N K
$$

where N is the number of components of this kind. (We could do better by employing independence, but then we would have to estimate the second moments by the fourth and it would boil down to the same.) 

To find N first note that the pairs of two distinct indices can be chosen in $\textstyle { { \binom { n } { 2 } } = { \frac { n ( n - 1 ) } { 2 } } }$ ways. Having fixed, $i , j$ the term $X _ { i } ^ { 2 } X _ { j } ^ { 2 }$ arises in 6 ways corre-  sponding to possible arrangements of 2 pairs of 2 indices: $( i , i , j , j ) , ( i , j , i , j )$ $( i , j , j , i ) , ( j , j , i , i ) , ( j , i , j , i ) , ( j , i , i , j )$ . So $N = 3 n ( n - 1 )$ and we have 

$$
\mathbb {E} (S _ {n} ^ {4}) \leq K (n + 3 n (n - 1)) = K (n + 3 n ^ {2} - 3 n) \leq 3 K n ^ {2}.
$$

By Chebyshev’s inequality 

$$
P (| \frac {S _ {n}}{n} | \geq \varepsilon) = P (| S _ {n} | \geq n \varepsilon) \leq \frac {\mathbb {E} (S _ {n} ^ {4})}{(n \varepsilon) ^ {4}} \leq \frac {3 K}{\varepsilon^ {4}} \cdot \frac {1}{n ^ {2}}.
$$

The series $\sum { \frac { 1 } { n ^ { 2 } } }$ converges and by Borel–Cantelli the set lim sup $A _ { n }$ with $A _ { n } =$ $\{ \omega : | \frac { S _ { n } } { n } | \geq \varepsilon \}$ has measure zero. Its complement is the set of full measure we need on which the sequence $\frac { S _ { n } } { n }$ converges to 0. To see this let $\omega \not \in$ lim sup $A _ { n }$ which means that $\omega$ is in finitely many $A _ { n }$ . So for a certain $n _ { 0 }$ , all $n \geq n _ { 0 }$ $\omega \not \in A _ { n }$ , i.e. $\begin{array} { r } { \frac { S _ { n } } { n } < \varepsilon } \end{array}$ (as observed before). and this is precisely what was needed for the convergence in question. □ 

The next law will only require finite moments of order 2, even not necessarily uniformly bounded. 

We precede it by an auxiliary but crucial inequality due to Kolmogorov. It gives a better estimate than does the Chebyshev inequality. The latter says that 

$$
P (| S _ {n} | \geq \varepsilon) \leq \frac {\operatorname{Var} (S _ {n})}{\varepsilon^ {2}}.
$$

In the theorem below the left-hand side is larger hence the result is stronger. 

## Theorem 8.19

If $X _ { 1 } , \ldots , X _ { n }$ are independent with 0 expectation and finite variances, then for any $\varepsilon > 0$ 

$$
P (\max _ {1 \leq k \leq n} | S _ {k} | \geq \varepsilon) \leq \frac {\operatorname{Var} (S _ {n})}{\varepsilon^ {2}}
$$

where $S _ { n } = X _ { 1 } + \cdot \cdot \cdot + X _ { n }$ 

## Proof

We fix an $\varepsilon > 0$ and describe the first instance that $| S _ { k } |$ exceeds $\varepsilon .$ Namely, we write 

$$
\varphi_ {k} = \left\{ \begin{array}{l l} 1 & \text { if } | S _ {1} | <   \varepsilon , \ldots , | S _ {k - 1} | <   \varepsilon , | S _ {k} | \geq \varepsilon \\ 0 & \text { if all } | S _ {i} | <   \varepsilon . \end{array} \right.
$$

For any $\omega$ at most one of the numbers $\varphi _ { k } ( \omega )$ may be 1, the remaining ones being 0, hence their sum is either 0 or 1. Clearly 

$$
\sum_ {k = 1} ^ {n} \varphi_ {k} = 0 \quad \Leftrightarrow \quad \max _ {1 \leq k \leq n} | S _ {k} | <   \varepsilon ,
$$

$$
\sum_ {k = 1} ^ {n} \varphi_ {k} = 1 \quad \Leftrightarrow \quad \max _ {1 \leq k \leq n} | S _ {k} | \geq \varepsilon .
$$

Hence 

$$
P (\max _ {1 \leq k \leq n} | S _ {k} | \geq \varepsilon) = P (\sum_ {k = 1} ^ {n} \varphi_ {k} = 1) = \mathbb {E} (\sum_ {k = 1} ^ {n} \varphi_ {k})
$$

since the expectation is the integral of an indicator function: 

$$
\mathbb {E} \left(\sum_ {k = 1} ^ {n} \varphi_ {k}\right) = \int_ {\{\omega : \sum_ {k = 1} ^ {n} \varphi_ {k} (\omega) = 0 \}} 0 \mathrm{d} P + \int_ {\{\omega : \sum_ {k = 1} ^ {n} \varphi_ {k} (\omega) = 1 \}} 1 \mathrm{d} P.
$$

So it remains to show that 

$$
\mathbb {E} (\sum_ {k = 1} ^ {n} \varphi_ {k}) \leq \frac {1}{\varepsilon^ {2}} \mathrm{Var} (S _ {n}) = \frac {1}{\varepsilon^ {2}} \mathbb {E} (S _ {n} ^ {2}),
$$

the last equality because $\mathbb { E } ( S _ { n } ) = 0$ . We estimate $\mathbb { E } ( S _ { n } ^ { 2 } )$ from below 

$$
\begin{array}{l} \mathbb {E} (S _ {n} ^ {2}) \geq \mathbb {E} (\sum_ {k = 1} ^ {n} \varphi_ {k} \cdot S _ {n} ^ {2}) \quad (\text { since } \sum_ {k = 1} ^ {n} \varphi_ {k} \leq 1) \\ \qquad = \mathbb {E} (\sum_ {k = 1} ^ {n} [ S _ {k} ^ {2} + 2 S _ {k} (S _ {n} - S _ {k}) + (S _ {n} - S _ {k}) ^ {2} ] \varphi_ {k}) \quad (\text { simple   algebra }) \\ \qquad \geq \mathbb {E} (\sum_ {k = 1} ^ {n} [ S _ {k} ^ {2} + 2 S _ {k} (S _ {n} - S _ {k}) ] \varphi_ {k}) \quad (\text { non - negative   term   deleted }) \\ \qquad = \mathbb {E} (\sum_ {k = 1} ^ {n} S _ {k} ^ {2} \varphi_ {k}) + 2 \mathbb {E} (\sum_ {k = 1} ^ {n} S _ {k} (S _ {n} - S _ {k}) \varphi_ {k}). \end{array}
$$

We show that the last expectation is equal to 0. Observe that $\varphi _ { k }$ is a function of random variables $X _ { 1 } , \ldots , X _ { k }$ so it is independent of $X _ { k + 1 } , \ldots , X _ { n }$ and also $S _ { k }$ is independent of $X _ { k + 1 } , \ldots , X _ { n }$ for the same reason. We compute one component of this last sum: 

$$
\begin{array}{l} \mathbb {E} (S _ {k} (S _ {n} - S _ {k}) \varphi_ {k}) = \mathbb {E} (S _ {k} \varphi_ {k} (\sum_ {i = k + 1} ^ {n} X _ {i})) \quad \text {(by the definition of S_{n})} \\ \qquad = \mathbb {E} (S _ {k} \varphi_ {k}) \mathbb {E} (\sum_ {i = k + 1} ^ {n} X _ {i}) \quad \text {(by independence)} \\ \qquad = 0 \quad \text {(since \mathbb {E} (X_{i}) = 0 for all i).} \end{array}
$$

In the remaining sum note that for each $k \le n , \varphi _ { k } S _ { k } ^ { 2 } \ge \varphi _ { k } \varepsilon ^ { 2 }$ (this is $0 \geq 0$ if $\varphi _ { k } = 0$ and $S _ { k } ^ { k } \geq \varepsilon ^ { 2 }$ if $\varphi _ { k } = 1$ , both true), hence 

$$
\mathbb {E} (\sum_ {k = 1} ^ {n} S _ {k} ^ {2} \varphi_ {k}) \geq \mathbb {E} (\varepsilon^ {2} \sum_ {k = 1} ^ {n} \varphi_ {k}) = \varepsilon^ {2} \mathbb {E} (\sum_ {k = 1} ^ {n} \varphi_ {k})
$$

which gives the desired inequality. 

Theorem 8.20 

Suppose that $X _ { 1 } , X _ { 2 } , . . .$ . are independent with $\mathbb { E } ( X _ { n } ) = 0$ and 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} \mathrm{Var} (X _ {n}) <   \infty .
$$

Then 

$$
\frac {S _ {n}}{n} \rightarrow 0 \quad \mathrm{almostsurely}.
$$

Proof 

We introduce auxiliary random variables 

$$
Y _ {m} = \max _ {k \leq 2 ^ {m}} | S _ {k} |
$$

and for $2 ^ { m - 1 } \leq n \leq 2 ^ { m }$ 

$$
| \frac {S _ {n}}{n} | \leq \frac {1}{n} \max _ {k \leq 2 ^ {m}} | S _ {k} | \leq \frac {1}{2 ^ {m - 1}} Y _ {m}.
$$

It is suficient to show that $\begin{array} { r } { { \frac { Y _ { m } } { 2 ^ { m } } } \to 0 } \end{array}$ almost surely and by Lemma 8.2 it is suficient to show that for each $\varepsilon > 0$ 

$$
\sum_ {m = 1} ^ {\infty} P (| \frac {Y _ {m}}{2 ^ {m}} | \geq \varepsilon) <   \infty .
$$

First take a single term $P ( | Y _ { m } | \geq 2 ^ { m } \varepsilon )$ and estimate it by Kolmogorov’s inequality (Theorem 8.19) 

$$
P (| Y _ {m} | \geq 2 ^ {m} \varepsilon) \leq \frac {\mathrm{Var} (S _ {2 ^ {m}})}{\varepsilon^ {2} 2 ^ {2 m}}.
$$

The problem reduces to showing that 

$$
\sum_ {m = 1} ^ {\infty} \mathrm{Var} (S _ {2 ^ {m}}) \frac {1}{4 ^ {m}} <   \infty .
$$

We rearrange the components 

$$
\begin{array}{l} \sum_ {m = 1} ^ {\infty} \operatorname{Var} (S _ {2 ^ {m}}) \frac {1}{4 ^ {m}} = \sum_ {m = 1} ^ {\infty} \frac {1}{4 ^ {m}} \sum_ {k = 1} ^ {2 ^ {m}} \operatorname{Var} (X _ {k}) \\ \qquad = \operatorname{Var} (X _ {1}) \sum_ {m = 1} ^ {\infty} \frac {1}{4 ^ {m}} + \operatorname{Var} (X _ {2}) \sum_ {m = 1} ^ {\infty} \frac {1}{4 ^ {m}} \\ \qquad + \operatorname{Var} (X _ {3}) \sum_ {m = 2} ^ {\infty} \frac {1}{4 ^ {m}} + \operatorname{Var} (X _ {4}) \sum_ {m = 2} ^ {\infty} \frac {1}{4 ^ {m}} \\ \qquad + \operatorname{Var} (X _ {5}) \sum_ {m = 3} ^ {\infty} \frac {1}{4 ^ {m}} + \dots + \operatorname{Var} (X _ {8}) \sum_ {m = 3} ^ {\infty} \frac {1}{4 ^ {m}} \\ \qquad + \dots \end{array}
$$

since $\mathrm { V a r } ( X _ { 1 } )$ , Var $( X _ { 2 } )$ appear in all components of the series in m $( 1 , 2 \leq$ $2 ^ { 1 } )$ ), $\operatorname { V a r } ( X _ { 3 } ) , \operatorname { V a r } ( X _ { 4 } )$ appear in all except the first one $( 2 ^ { 1 } < 3 , 4 \le 2 ^ { 2 } )$ $\operatorname { V a r } ( X _ { 5 } ) , . . . , \operatorname { V a r } ( X _ { 8 } )$ appear in all except the first two $( 2 ^ { 2 } < 5 , 6 , 7 , 8 \leq 2 ^ { 3 } )$ and so on. We arrive at the series 

$$
\sum_ {k = 1} ^ {\infty} \mathrm{Var} (X _ {k}) a _ {k}
$$

where 

$$
a _ {k} = \sum_ {\{m: 2 ^ {m} > k \}} \frac {1}{4 ^ {m}}.
$$

This is a geometric series with ratio $\textstyle { \frac { 1 } { 4 } }$ and the first term $\textstyle { \frac { 1 } { 4 ^ { j } } }$ where j is the least integer such that $2 ^ { j } > k$ . If we replace $2 ^ { j }$ by $k$ we increase the sum by adding more terms and the first terms is then $\scriptstyle { \frac { 1 } { 2 ^ { k } } }$ : 

$$
a _ {k} \leq \frac {\frac {1}{2 ^ {k}}}{1 - \frac {1}{4}}
$$

and by the hypothesis 

$$
\sum_ {k = 1} ^ {\infty} \operatorname{Var} (X _ {k}) a _ {k} \leq \frac {4}{3} \sum_ {k = 1} ^ {\infty} \operatorname{Var} (X _ {k}) \frac {1}{2 ^ {k}} <   \infty
$$

which completes the proof. 

Finally, we relax the conditions on moments even further; simultaneously we need to impose the assumption that the random variables are identically distributed. 

## Theorem 8.21

Suppose that $X _ { 1 } , X _ { 2 } , . . .$ . are independent identically distributed, with $\mathbb { E } ( X _ { 1 } ) =$ $m < \infty$ . Then Q 

$$
\frac {S _ {n}}{n} \rightarrow m \quad \mathrm{almostsurely}.
$$

## Proof

The idea is to use the previous theorem where we needed finite variances. Since we do not have that here we truncate $X _ { n }$ 

$$
Y _ {n} = X _ {n} (n) = X _ {n} \mathbf {1} _ {\{\omega : | X _ {n} (\omega) | \leq n \}}.
$$

The truncated random variables have finite variances since each is bounded: $| Y _ { n } | \leq n$ (the right-hand side is forced to be zero if $X _ { n }$ dare upcross the level n). The new variables difer from the original ones if $| X _ { n } | > n$ . This, however, cannot happen too often as the following argument shows. First 

$$
\begin{array}{l} \sum_ {n = 1} ^ {\infty} P (Y _ {n} \neq X _ {n}) \\ = \sum_ {n = 1} ^ {\infty} P (| X _ {n} | > n) \\ = \sum_ {n = 1} ^ {\infty} P (| X _ {1} | > n) \quad (\text { the   distributions   being   the   same }) \\ \leq \sum_ {n = 1} ^ {\infty} \int_ {n - 1} ^ {n} P (| X _ {1} | > x)   \mathrm{d} x \quad (\text { as } P (| X _ {1} | > x) \geq P (| X _ {1} | > n)) \\ \leq \int_ {0} ^ {\infty} P (| X _ {1} | > x)   \mathrm{d} x \\ = \mathbb {E} (| X _ {1} |) \quad (\text { by   Lemma   8.11 }) \\ <   \infty . \end{array}
$$

So by Borel–Cantelli, with probability one only finitely many events $X _ { n } \neq Y _ { n }$ happen, so in other words, there is a set $\varOmega ^ { \prime }$ with $P ( \varOmega ^ { \prime } ) = 1$ such that for $\omega \in \varOmega ^ { \prime } , X _ { n } ( \omega ) = Y _ { n } ( \omega )$ for all except finitely many n. So on $\varOmega ^ { \prime } \mathrm { ~ i f ~ } \frac { Y _ { 1 } + \cdots + Y _ { n } } { n }$ converges to some limit, then the same holds for $\scriptstyle { \frac { S _ { n } } { n } }$ 

To use the previous theorem we have to show the convergence of the series 

$$
\sum_ {n = 1} ^ {\infty} \frac {\operatorname{Var} (Y _ {n})}{n ^ {2}}
$$

but since $\operatorname { V a r } ( Y _ { n } ) = \operatorname { \mathbb { E } } ( Y _ { n } ^ { 2 } ) - ( \operatorname { \mathbb { E } } Y _ { n } ) ^ { 2 } \leq \operatorname { \mathbb { E } } Y _ { n } ^ { 2 }$ it is suficient to show the convergence of 

$$
\sum_ {n = 1} ^ {\infty} \frac {\mathbb {E} (Y _ {n} ^ {2})}{n ^ {2}}.
$$

To this end note first 

$$
\begin{array}{l l} \mathbb {E} (Y _ {n} ^ {2}) = \int_ {0} ^ {\infty} 2 x P (| Y _ {n} | > x)   \mathrm{d} x & \text {(by Lemma 8.11)} \\ = \int_ {0} ^ {n} 2 x P (| Y _ {n} | > x)   \mathrm{d} x & \text {(since P(|Y_{n}|>n)=0)} \\ = \int_ {0} ^ {n} 2 x P (| X _ {n} | > x)   \mathrm{d} x & \text {(if |Y_{n}|\leq n then Y_{n}=X_{n})} \\ = \int_ {0} ^ {n} 2 x P (| X _ {1} | > x)   \mathrm{d} x & \text {(identical distributions)}. \end{array}
$$

Next 

$$
\begin{array}{l} \sum_ {n = 1} ^ {\infty} \frac {\mathbb {E} (Y _ {n} ^ {2})}{n ^ {2}} = \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} \int_ {0} ^ {n} 2 x P (| X _ {1} | > x)   \mathrm{d} x \\ \qquad = \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} \int_ {0} ^ {\infty} 2 x \mathbf {1} _ {[ 0, n)} (x) P (| X _ {1} | > x)   \mathrm{d} x \\ \qquad = 2 \int_ {0} ^ {\infty} \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} x \mathbf {1} _ {[ 0, n)} (x) P (| X _ {1} | > x)   \mathrm{d} x. \end{array}
$$

We examine the function $\textstyle x \mapsto \sum _ { n = 1 } ^ { \infty } { \frac { 1 } { n ^ { 2 } } } x \mathbf { 1 } _ { [ 0 , n ) } ( x )$ 

If $0 \leq x \leq 1$ Pthen none of the terms in the series is killed and 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} x \mathbf {1} _ {[ 0, n)} (x) \leq \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} = \frac {\pi^ {2}}{6} <   2
$$

as is well known. 

If $x > 1$ , then we only have the sum over $n \geq x$ . Let $m = \operatorname { I n t } ( x )$ (the integer part of x). We have 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} x \mathbf {1} _ {[ 0, n)} (x) = x \sum_ {n = m + 1} ^ {\infty} \frac {1}{n ^ {2}} \leq x \int_ {m} ^ {\infty} \frac {1}{x ^ {2}} \mathrm{d} x = x \frac {1}{m} \leq 2.
$$

In each case the function in question is bounded by 2 so 

$$
\sum_ {n = 1} ^ {\infty} \frac {\mathbb {E} (Y _ {n} ^ {2})}{n ^ {2}} \leq 4 \int_ {0} ^ {\infty} P (| X _ {1} | > x) \mathrm{d} x = 4 \mathbb {E} (| X _ {1} |) <   \infty .
$$

Consider $Y _ { n } - \mathbb { E } Y _ { n }$ and apply the previous theorem to get 

$$
\frac {1}{n} \sum_ {k = 1} ^ {n} (Y _ {k} - \mathbb {E} Y _ {k}) \rightarrow 0 \quad \text { almost   surely }.
$$

We have 

$$
\mathbb {E} (Y _ {k}) = \mathbb {E} (X _ {k} \mathbf {1} _ {\{\omega : | X _ {k} | \leq k \}}) = \mathbb {E} (X _ {1} \mathbf {1} _ {\{\omega : | X _ {1} (\omega) | \leq k \}}) \to m
$$

since $X _ { 1 } \mathbf { 1 } _ { \{ \omega : | X _ { 1 } ( \omega ) | \le k \} } \to X _ { 1 }$ , the sequence being dominated by $| X _ { 1 } |$ which is integrable. So we have by the triangle inequality 

$$
\left| \frac {1}{n} \sum_ {k = 1} ^ {n} Y _ {k} - m \right| \leq \left| \frac {1}{n} \sum_ {k = 1} ^ {n} \left(Y _ {k} - \mathbb {E} Y _ {k}\right)\right| + \frac {1}{n} \sum_ {k = 1} ^ {n} \left| \mathbb {E} Y _ {k} - m \right|\rightarrow 0.
$$

As observed earlier, this implies almost sure convergence of $\scriptstyle { \frac { S _ { n } } { n } }$ . 

## 8.2.5 Weak convergence

In order to derive central limit theorems we first need to investigate the convergence of the distributions of the sequence $( X _ { n } )$ of random variables. 

## Definition 8.4

A sequence $P _ { n }$ of Borel probability measures on $\mathbb { R } ^ { n }$ converges weakly to $P$ if and only their cumulative distribution functions $F _ { n }$ converge to the distribution function $F$ of P at all points where F is continuous. If $P _ { n } = P _ { X _ { n } } , P = P _ { X }$ are the distributions of some random variables, then we say that the sequence $( X _ { n } )$ converges weakly to $X$ 

The name ‘weak’ is justified since this convergence is implied by the weakest we have come across so far, i.e. convergence in probability. 

## Theorem 8.22

If $X _ { n }$ converge in probability to $X$ , then the distributions of $X _ { n }$ converge weakly. 

Proof 

Let $F ( y ) = P ( X \leq y )$ . Fix $y ,$ , a continuity point of $F$ , and $\varepsilon > 0$ . The goal is to obtain 

$$
F (y) - \varepsilon <   F _ {n} (y) <   F (y) + \varepsilon
$$

for suficiently large n. By continuity of $F$ we can find $\delta > 0$ such that 

$$
P (X \leq y) - \frac {\varepsilon}{2} <   P (X \leq y - \delta), \quad P (X \leq y + \delta) <   F (y) + \frac {\varepsilon}{2}.
$$

By convergence in probability, 

$$
P (| X _ {n} - X | > \delta) <   \frac {\varepsilon}{2}.
$$

Clearly, if $X _ { n } \leq y$ and $\left| X _ { n } - X \right| < \delta$ , then $X < y + \delta$ so 

$$
P ((X _ {n} \leq y) \cap (| X _ {n} - X | <   \delta)) \leq P (X <   y + \delta).
$$

We can estimate the left-hand side from below: 

$$
P (X _ {n} \leq y) - \frac {\varepsilon}{2} <   P ((X _ {n} \leq y) \cap (| X _ {n} - X | <   \delta)).
$$

Putting all these together we get 

$$
P (X _ {n} \leq y) <   P (X \leq y) + \varepsilon
$$

and letting $\varepsilon \to 0$ we have achieved half of the goal. The other half is obtained similarly. □ 

However it turns out that weak convergence in a certain sense implies convergence almost surely. What we mean by ‘in a certain sense’ is explained in the next theorem: it also gives a central role to the Borel sets and Lebesgue measure in [0, 1]. 

## Theorem 8.23 (Skorokhod Representation Theorem)

If $P _ { n }$ converge weakly to P, then there exist $X _ { n } , X$ , random variables defined on the probability $( [ 0 , 1 ] , B , m _ { [ 0 , 1 ] } )$ , such that $P _ { X _ { n } } = P _ { n } , P _ { X } = P$ and $X _ { n } \to X$ a.s. 

## Proof

Take $X _ { n } ^ { + } , X _ { n } ^ { - } , X ^ { + } , X ^ { - }$ corresponding to $F _ { n } , F$ , the distribution functions of $P _ { n } , P$ , as in Theorem 4.31. We have shown there that $F _ { X ^ { + } } = F _ { X ^ { - } } = F$ which implies $P ( X ^ { + } = X ^ { - } ) = 1$ . Fix an ω such that $X ^ { + } ( \omega ) = X ^ { - } ( \omega )$ . Let $y$ be a continuity point of F such that $y > X ^ { + } ( \omega )$ . Then $F ( y ) > \omega$ and, by the weak convergence, for suficiently large n we have $F _ { n } ( y ) > \omega$ . Then, by the construction, $X _ { n } ^ { + } ( \omega ) \leq y$ . This inequality holds for all except finitely many n so it is preserved if we take the upper limit on the left: 

$$
\limsup X _ {n} ^ {+} (\omega) \leq y.
$$

Take a sequence $y _ { k }$ of continuity points of F converging to $X ^ { + } ( \omega )$ from above (the set of discontinuity points of a monotone function is at most countable). For $y = y _ { k }$ consider the above inequality and pass to the limit with k to get 

$$
\limsup X _ {n} ^ {+} (\omega) \leq X ^ {+} (\omega).
$$

Similarly 

$$
\liminf X _ {n} ^ {-} (\omega) \geq X ^ {-} (\omega)
$$

so 

$$
X ^ {-} (\omega) \leq \liminf X _ {n} ^ {-} (\omega) \leq \limsup X _ {n} ^ {+} (\omega) \leq X ^ {+} (\omega).
$$

The extremes are equal a.s. so the convergence holds a.s. 

The Skorokhod theorem is an important tool in probability. We will only need it for the following result, which links convergence of distributions to that of the associated characteristic functions. 

## Theorem 8.24

If $P _ { X _ { n } }$ converge weakly to $P _ { X }$ then $\varphi _ { X _ { n } } \longrightarrow \varphi _ { X }$ 

## Proof

Take the Skorokhod representation $Y _ { n } , ~ Y$ of the measures $P _ { X _ { n } } , P _ { X }$ . Almost sure convergence of $Y _ { n }$ to Y implies that $\mathbb { E } ( \mathrm { e } ^ { \mathrm { i } t Y _ { n } } ) \to \mathbb { E } ( \mathrm { e } ^ { \mathrm { i } t Y } )$ by the dominated convergence theorem. But the distributions of $X _ { n } , ~ X$ are the same as the distributions of $Y _ { n } , Y$ , so the characteristic functions are the same. □ 

## Theorem 8.25 (Helly’s Theorem)

Let $F _ { n }$ be a sequence of distribution functions of some probability measures. There exists F, the distribution function of a measure (not necessarily probability), and a sequence $k _ { n }$ such that $F _ { k _ { n } } ( x )  F ( x )$ at the continuity points of $F .$ 

## Proof

Arrange the rational numbers in a sequence: $\mathbb { Q } = \{ q _ { 1 } , q _ { 2 } , . . . \}$ . The sequence $F _ { n } ( q _ { 1 } )$ is bounded (the values of a distribution function lie in [0,1]), hence it has a convergent subsequence, 

$$
F _ {k _ {n} ^ {1}} (q _ {1}) \to y _ {1}.
$$

Next consider the sequence $F _ { k _ { n } ^ { 1 } } ( q _ { 2 } )$ , which is again bounded, so for a subsequence $k _ { n } ^ { 2 }$ of $k _ { n } ^ { 1 }$ we have convergence 

$$
F _ {k _ {n} ^ {2}} (q _ {2}) \rightarrow y _ {2}.
$$

Of course also 

$$
F _ {k _ {n} ^ {2}} (q _ {1}) \to y _ {1}.
$$

Proceeding in this way we find $k _ { n } ^ { 3 } , \ k _ { n } ^ { 4 } , \ldots$ , each term a subsequence of the previous one, with 

$$
F _ {k _ {n} ^ {3}} (q _ {m}) \to y _ {m} \quad \text { for } m \leq 3,
$$

$$
F _ {k _ {n} ^ {4}} (q _ {m}) \rightarrow y _ {m} \quad \mathrm{for} m \leq 4,
$$

and so on. The diagonal sequence $F _ { k _ { n } } = F _ { k _ { n } ^ { n } }$ converges at all rational points. We define $F _ { \mathbb { Q } }$ on $\mathbb { Q }$ by 

$$
F _ {\mathbb {Q}} (q) = \lim F _ {k _ {n}} (q)
$$

and next we write 

$$
F (x) = \inf \{F _ {\mathbb {Q}} (q): q \in \mathbb {Q}, q > x \}.
$$

We show that F is non-decreasing. Since $F _ { n }$ are non-decreasing, the same is true for $F _ { \mathbb { Q } } \ ( q _ { 1 } < q _ { 2 }$ implies $F _ { k _ { n } } ( q _ { 1 } ) \leq F _ { k _ { n } } ( q _ { 2 } )$ which remains true in the limit). Now let $x _ { 1 } < x _ { 2 } . \ F ( x _ { 1 } ) \le F _ { \mathbb { Q } } ( q )$ for all $q > x _ { 1 }$ hence in particular for all $q > x _ { 2 }$ , so $\begin{array} { r } { F ( x _ { 1 } ) \le \operatorname* { i n f } _ { q > x _ { 2 } } F _ { \mathbb { Q } } ( q ) = F ( x _ { 2 } ) } \end{array}$ 

We show that F is right-continuous. Let $x _ { n } \searrow x$ . By the monotonicity of $F , F ( x ) \leq F ( x _ { n } )$ hence $F ( x ) \leq \operatorname* { l i m } F ( x _ { n } )$ . Suppose that $F ( x ) < \operatorname* { l i m } F ( x _ { n } )$ By the definition of $F$ there is $q \in \mathbb { Q } , x < q$ , such that $F _ { \mathbb { Q } } ( q ) < \operatorname* { l i m } F ( x _ { n } )$ . For some $n _ { 0 } , x \le x _ { n _ { 0 } } < q$ hence $F ( x _ { n _ { 0 } } ) \leq F _ { \mathbb { Q } } ( q )$ again by the definition of F, thus $F ( x _ { n _ { 0 } } ) < \operatorname* { l i m } F ( x _ { n } )$ which is a contradiction. 

Finally, we show that if F is continuous at x, then $F _ { k _ { n } } ( x )  F ( x )$ . Let $\varepsilon > 0$ be arbitrary and find rationals $q _ { 1 } < q _ { 2 } < x < q _ { 3 }$ such that 

$$
F (x) - \varepsilon <   F (q _ {1}) \leq F (x) \leq F (q _ {3}) <   F (x) + \varepsilon .
$$

Since $F _ { k _ { n } } ( q _ { 2 } ) \longrightarrow F _ { \mathbb { Q } } ( q _ { 2 } ) \ge F ( q _ { 1 } )$ , for suficiently large n 

$$
F (x) - \varepsilon <   F _ {k _ {n}} (q _ {2}).
$$

But $F _ { k _ { n } }$ is non-decreasing, so 

$$
F _ {k _ {n}} (q _ {2}) \leq F _ {k _ {n}} (x) \leq F _ {k _ {n}} (q _ {3}).
$$

Finally, $F _ { k _ { n } } ( q _ { 3 } ) \to F _ { \mathbb { Q } } ( q _ { 3 } ) \geq F ( q _ { 3 } )$ , so for suficiently large n 

$$
F _ {k _ {n}} (q _ {3}) <   F (x) + \varepsilon .
$$

Putting together the above three inequalities we get 

$$
F (x) - \varepsilon <   F _ {k _ {n}} (x) <   F (x) + \varepsilon
$$

which proves the convergence. 

## Remark 8.4

The limit distribution function need not correspond to a probability measure. Example: $F _ { n } = \mathbf { 1 } _ { [ n , \infty ) } , F _ { n } \to 0$ so $F = 0$ . This is a distribution function (nondecreasing, right continuous) and the corresponding measure satisfies $P ( A ) = 0$ for all A. We then say informally that the mass escapes to infinity. The following concept is introduced to prevent this happening. 

## Definition 8.5

We say that a sequence of probabilities $P _ { n }$ on $\mathbb { R } ^ { d }$ is tight if for each $\varepsilon > 0$ there is M such that $P _ { n } ( \mathbb { R } ^ { d } \setminus [ - M , M ] ) < \varepsilon$ for all n. 

By an interval in $\mathbb { R } ^ { n }$ we understand the product of intervals: $[ - M , M ] =$ $\{ x = ( x _ { 1 } , \ldots , x _ { n } ) \in \mathbb { R } ^ { n } : x _ { i } \in [ - M , M ]$ all i . It is important that the M chosen for ε is good for all $n \mathrm { ~ - ~ }$ the inequality is uniform. It is easy to find such an $M \ = \ M _ { n }$ for each $P _ { n }$ separately. This follows from the fact that $P _ { n } ( [ - M , M ] ) \to 1$ as $M \to \infty$ 

## Theorem 8.26 (Prokhorov’s Theorem)

If a sequence $P _ { n }$ is tight, then it has a subsequence convergent weakly to some probability measure P. 

## Proof

By Helly’s theorem a subsequence $F _ { k _ { n } }$ converges to some distribution function F. All we have to do is to show that F corresponds to some probability measure P, which means we have to show that $F ( \infty ) = 1 \ ( { \mathrm { i . e . } } \ \operatorname* { l i m } _ { y \to \infty } F ( y ) = 1 )$ . Fix $\varepsilon > 0$ and find a continuity point such that $F _ { n } ( y ) = P _ { n } ( ( - \infty , y ] ) > 1 - \varepsilon$ for all n (find M from the definition of tightness and take a continuity point of F which is larger than M). Hence $\begin{array} { r } { \operatorname* { l i m } _ { n  \infty } F _ { k _ { n } } ( y ) \geq 1 - \varepsilon } \end{array}$ , but this limit is $F ( y )$ This proves that lim $\iota _ { y \to \infty } F ( y ) = 1$ □ 

We need to extend the notion of the characteristic function. 

## Definition 8.6

We say that $\varphi$ is the characteristic function of a Borel measure $P$ on R if $\begin{array} { r } { \varphi ( t ) = \int e ^ { i t x } \mathrm { d } P ( x ) } \end{array}$ 

In the case where $P = P _ { X }$ we obviously have $\varphi _ { P } = \varphi _ { X }$ , so the two definitions are consistent. 

## Theorem 8.27

Suppose $( P _ { n } )$ is tight and let $P$ be the limit of a subsequence of $( P _ { n } )$ as provided by Prokhorov’s theorem. If $\varphi _ { n } ( u ) ~ \to ~ \varphi ( u )$ where $\varphi _ { n }$ are the characteristic functions of $P _ { n }$ and $\varphi$ is the characteristic function of $P .$ , then $P _ { n } \to P$ weakly. 

## Proof

Fix a continuity point of $F$ . For every subsequence $F _ { k _ { n } }$ there is a subsequence (subsubsequence) $l _ { k _ { n } } , l _ { n }$ for brevity, such that $F _ { l _ { n } }$ converge to some function H (Helly’s theorem). Denote the corresponding measure by $P ^ { \prime }$ . Hence $\varphi _ { l _ { n } }  \varphi _ { P ^ { \prime } }$ 2 but on the other hand, $\varphi _ { l _ { n } } \ \to \ \varphi$ . So $\varphi _ { P ^ { \prime } } = \varphi$ and consequently $P ^ { \prime } = P$ (Corollary 6.18). The above is suficient for the convergence of the sequence $F _ { n } ( y )$ □ 

## 8.2.6 Central Limit Theorem

The following lemma will be useful in what follows. It shows how to estimate the ‘weight’ of the ‘tails’ of a probability measure, and will be a useful tool in proving tightness. 

## Lemma 8.28

If $\varphi$ is the characteristic function of $P _ { \mathrm { : } }$ , then 

$$
P (\mathbb {R} \setminus [ - M, M ]) \leq 7 M \int_ {0} ^ {\frac {1}{M}} [ 1 - \Re \varphi (u) ] \mathrm{d} u.
$$

Proof 

$$
\begin{array}{l} M \int_ {0} ^ {\frac {1}{M}} [ 1 - \Re \varphi (u) ]   \mathrm{d} u = M \int_ {0} ^ {\frac {1}{M}} [ 1 - \Re \int_ {\mathbb {R}} \mathrm{e} ^ {\mathrm{i} x u}   \mathrm{d} P (x) ]   \mathrm{d} u \\ \qquad = M \int_ {0} ^ {\frac {1}{M}} [ 1 - \int_ {\mathbb {R}} \cos (x u)   \mathrm{d} P (x) ]   \mathrm{d} u \\ \qquad = \int_ {\mathbb {R}} M \int_ {0} ^ {\frac {1}{M}} [ 1 - \cos (x u) ]   \mathrm{d} u   \mathrm{d} P (x) \quad (\text { by   Fubini }) \\ \qquad = \int_ {\mathbb {R}} (1 - \frac {\sin (\frac {x}{M})}{\frac {x}{M}})   \mathrm{d} P (x) \\ \qquad \geq \int_ {| t | \geq 1} (1 - \frac {\sin (\frac {x}{M})}{\frac {x}{M}})   \mathrm{d} P (x) \\ \qquad \geq \inf _ {| t | \geq 1} (1 - \frac {\sin t}{t}) \int_ {| \frac {x}{M} | > 1}   \mathrm{d} P (x) \\ \qquad \geq \frac {1}{7} P (\mathbb {R} \setminus [ - M, M ]) \end{array}
$$

since $\textstyle 1 - { \frac { \sin t } { t } } \geq 1 - \sin 1 \geq { \frac { 1 } { 7 } }$ 

## Theorem 8.29 (Levy’s Theorem)

Let $\varphi _ { n }$ be the characteristic functions of $P _ { n }$ . Suppose that $\varphi _ { n } \to \varphi$ where $\varphi$ is a function continuous at 0. Then $\varphi$ is the characteristic function of a measure $P$ and $P _ { n } \to P$ weakly. 

## Proof

It is suficient to show that $P _ { n }$ is tight (then $P _ { k _ { n } }  P$ weakly for some $P$ and $k _ { n } , \varphi _ { k _ { n } } \longrightarrow \varphi _ { P } , \varphi = \varphi _ { P }$ , and by the previous theorem we are done). 

Applying Lemma 8.28 we have 

$$
P _ {n} (\mathbb {R} \setminus [ - M, M ]) \leq 7 M \int_ {0} ^ {\frac {1}{M}} [ 1 - \Re \varphi_ {n} (u) ] \mathrm{d} u.
$$

Since $\varphi _ { n } \to \varphi , | \varphi _ { n } | \leq 1$ , and for fixed $M$ , this upper bound is integrable, so by the dominated convergence theorem 

$$
7 M \int_ {0} ^ {\frac {1}{M}} [ 1 - \Re \varphi_ {n} (u) ] \mathrm{d} u \rightarrow 7 M \int_ {0} ^ {\frac {1}{M}} [ 1 - \Re \varphi (u) ] \mathrm{d} u.
$$

If $M \to \infty$ , then 

$$
7 M \int_ {0} ^ {\frac {1}{M}} [ 1 - \Re \varphi (u) ] \mathrm{d} u \leq 7 M \cdot \frac {1}{M} \cdot \sup _ {[ 0, \frac {1}{M} ]} | 1 - \Re \varphi (u) | \to 0
$$

by continuity of $\varphi$ at 0 (recall that $\varphi ( 0 ) = 1 )$ . Now let $\varepsilon > 0$ and find $M _ { 0 }$ such that $\begin{array} { r } { 7 \operatorname* { s u p } _ { [ 0 , \frac { 1 } { M _ { 0 } } ] } | 1 - \Re \varphi ( u ) | < \frac { \varepsilon } { 2 } } \end{array}$ , and $n _ { 0 }$ such that for $n \geq n _ { 0 }$ 

$$
| \int_ {0} ^ {\frac {1}{M _ {0}}} [ 1 - \Re \varphi_ {n} (u) ] \mathrm{d} u - \int_ {0} ^ {\frac {1}{M _ {0}}} [ 1 - \Re \varphi (u) ] \mathrm{d} u | <   \frac {\varepsilon}{2}.
$$

Hence 

$$
P _ {n} (\mathbb {R} \setminus [ - M _ {0}, M _ {0} ]) <   \varepsilon
$$

for $n \geq n _ { 0 }$ . Now for each $n = 1 , 2 , \ldots , n _ { 0 }$ find $M _ { n }$ such that $P _ { n } ( [ - M _ { n } , M _ { n } ] ) >$ $1 \ - \ \varepsilon$ and let $M \ = \ \operatorname* { m a x } \{ M _ { 0 } , M _ { 1 } , . . . , M _ { n _ { 0 } } \}$ . Of course since $M \ \geq \ M _ { k }$ $P _ { n } ( [ - M , M ] ) \ge P _ { n } ( [ - M _ { k } , M _ { k } ] ) > 1 - \varepsilon$ for each n which proves the tightness of $P _ { n }$ . □ 

For a sequence $X _ { k }$ with $m _ { k } = \operatorname { \mathbb { E } } ( X _ { k } ) , \sigma _ { k } ^ { 2 } = \operatorname { V a r } ( X _ { k } )$ finite, let $S _ { n } = X _ { 1 } +$ $\cdots + X _ { n }$ as usual and consider the normalized random variables 

$$
T _ {n} = \frac {S _ {n} - \mathbb {E} (S _ {n})}{\sqrt {\operatorname{Var} (S _ {n})}}.
$$

Clearly $\mathbb { E } ( T _ { n } ) = 0$ and $\operatorname { V a r } ( T _ { n } ) = 1 \ ( \mathrm { b y } \ \operatorname { V a r } ( a X ) = a ^ { 2 } \operatorname { V a r } ( X ) )$ . Write $c _ { n } ^ { 2 } = $ ${ \mathrm { V a r } } ( S _ { n } ) \ ( \mathrm { i f } \ X _ { n }$ are independent, then as we already know, $\begin{array} { r } { c _ { n } ^ { 2 } = \sum _ { k = 1 } ^ { n } \sigma _ { k } ^ { 2 } ) } \end{array}$ . We state a condition under which the sequence of distributions of $T _ { n }$ Pconverges to the standard Gaussian measure G (with the density ${ \textstyle { \frac { 1 } { \sqrt { 2 \pi } } } } \mathrm { e } ^ { - { \frac { 1 } { 2 } } x ^ { 2 } } )$ : 

$$
\frac {1}{c _ {n} ^ {2}} \sum_ {k = 1} ^ {n} \int_ {\{x: | x - m _ {k} | \geq \varepsilon c _ {n} \}} (x - m _ {k}) ^ {2} \mathrm{d} P _ {X _ {k}} (x) \to 0 \quad \mathrm{as} n \to \infty .\tag{8.4}
$$

In particular, if the distributions of $X _ { n }$ are the same, $m _ { k } = m , \sigma _ { k } = \sigma$ , then this condition is satisfied. To see this, note that assuming independence we have $c _ { n } ^ { 2 } = n \sigma ^ { 2 }$ and then 

$$
\int_ {\{x: | x - m | \geq \varepsilon \sigma \sqrt {n} \}} (x - m) ^ {2} \mathrm{d} P _ {X _ {k}} (x) = \int_ {\{x: | x - m | \geq \varepsilon \sigma \sqrt {n} \}} (x - m) ^ {2} \mathrm{d} P _ {X _ {1}} (x)
$$

hence 

$$
\begin{array}{c} \frac {1}{n \sigma^ {2}} \sum_ {k = 1} ^ {n} \int_ {\{x: | x - m | \geq \varepsilon \sigma \sqrt {n} \}} (x - m) ^ {2} \mathrm{d} P _ {X _ {k}} (x) \\ = \frac {1}{\sigma^ {2}} \int_ {\{x: | x - m | \geq \varepsilon \sigma \sqrt {n} \}} (x - m) ^ {2} \mathrm{d} P _ {X _ {1}} (x) \to 0 \end{array}
$$

as $n \to \infty$ since the set $\{ x : | x - m | \geq \varepsilon \sigma { \sqrt { n } } \}$ decreases to $\mathrm { \ o }$ 

We are ready for the main theorem in probability. The proof is quite technical and advanced, and may be omitted at a first reading. 

## Theorem 8.30 (Lindeberg–Feller Theorem)

Let $X _ { n }$ be independent with finite expectations and variances. If condition (8.4) holds, then $P _ { T _ { n } } \to G$ weakly. 

## Proof

Assume first that $m _ { k } = 0$ . It is suficient to show that the characteristic functions $\varphi _ { T _ { n } }$ converge to the characteristic function of G, i.e. to show that 

$$
\varphi_ {T _ {n}} (u) \rightarrow \mathrm{e} ^ {- \frac {1}{2} u ^ {2}}.
$$

We compute 

$$
\begin{array}{l} \varphi_ {T _ {n}} (u) = \mathbb {E} (\mathrm{e} ^ {\mathrm{i} u T _ {n}}) \quad \text {(by the definition of \varphi_ {T _ {n}})} \\ \qquad = \mathbb {E} (\mathrm{e} ^ {\mathrm{i} \frac {u}{c _ {n}} \sum_ {k = 1} ^ {n} X _ {k}}) \\ \qquad = \mathbb {E} (\prod_ {k = 1} ^ {n} \mathrm{e} ^ {\mathrm{i} \frac {u}{c _ {n}} X _ {k}}) \\ \qquad = \prod_ {k = 1} ^ {n} \mathbb {E} (\mathrm{e} ^ {\mathrm{i} \frac {u}{c _ {n}} X _ {k}}) \quad \text {(by independence)} \\ \qquad = \prod_ {k = 1} ^ {n} \varphi_ {X _ {k}} (\frac {u}{c _ {n}}) \quad \text {(by the definition of \varphi_ {X _ {k}})}. \end{array}
$$

What we need to show is that 

$$
\log \prod_ {k = 1} ^ {n} \varphi_ {X _ {k}} (\frac {u}{c _ {n}}) \rightarrow - \frac {1}{2} u ^ {2}.
$$

We shall make use of the following formulae (particular cases of Taylor’s formula for a complex variable) 

$$
\log (1 + z) = z + \theta_ {1} | z | ^ {2} \quad \text { for   some } \theta_ {1} \text { with } | \theta_ {1} | \leq 1,
$$

$$
\mathrm{e} ^ {\mathrm{i} y} = 1 + \mathrm{i} y + \frac {1}{2} \theta_ {2} y ^ {2} \quad \text { for   some } \theta_ {2} \text { with } | \theta_ {2} | \leq 1,
$$

$$
\mathrm{e} ^ {\mathrm{i} y} = 1 + \mathrm{i} y - \frac {1}{2} y ^ {2} + \frac {1}{6} \theta_ {3} | y | ^ {3} \quad \text { for   some } \theta_ {3} \text { with } | \theta_ {3} | \leq 1.
$$

So for fixed $\varepsilon > 0$ 

$$
\begin{array}{l} \varphi_ {X _ {k}} (u) = \int_ {| x | \geq \varepsilon c _ {n}} \mathrm{e} ^ {\mathrm{i} u x} \mathrm{d} P _ {X _ {k}} (x) + \int_ {| x | <   \varepsilon c _ {n}} \mathrm{e} ^ {\mathrm{i} u x} \mathrm{d} P _ {X _ {k}} (x) \\ \quad = \int_ {| x | \geq \varepsilon c _ {n}} (1 + \mathrm{i} u x + \frac {1}{2} \theta_ {2} u ^ {2} x ^ {2}) \mathrm{d} P _ {X _ {k}} (x) \\ \quad + \int_ {| x | <   \varepsilon c _ {n}} (1 + \mathrm{i} u x - \frac {1}{2} u ^ {2} x ^ {2} + \frac {1}{6} \theta_ {3} | u | ^ {3} | x | ^ {3}) \mathrm{d} P _ {X _ {k}} (x) \\ \quad = 1 + \frac {1}{2} u ^ {2} \int_ {| x | \geq \varepsilon c _ {n}} \theta_ {2} x ^ {2} \mathrm{d} P _ {X _ {k}} (x) - \frac {1}{2} u ^ {2} \int_ {| x | <   \varepsilon c _ {n}} x ^ {2} \mathrm{d} P _ {X _ {k}} (x) \\ \quad + \frac {1}{6} | u | ^ {3} \int_ {| x | <   \varepsilon c _ {n}} \theta_ {3} | x | ^ {3} \mathrm{d} P _ {X _ {k}} (x) \end{array}
$$

since ${ \textstyle \int } x \mathrm { d } P _ { X _ { k } } ( x ) = 0 \ ( \mathrm { t h i s ~ i s ~ } \mathbb { E } ( X _ { k } ) )$ . For clarity we introduce the following Rnotation 2 

$$
\alpha_ {n k} = \int_ {| x | \geq \varepsilon c _ {n}} x ^ {2} \mathrm{d} P _ {X _ {k}} (x),
$$

$$
\beta_ {n k} = \int_ {| x | <   \varepsilon c _ {n}} x ^ {2} \mathrm{d} P _ {X _ {k}} (x).
$$

Observe, that $\beta _ { n k } \le \varepsilon ^ { 2 } c _ { n } ^ { 2 }$ because on the set over which we take the integral we have $x ^ { 2 } < \varepsilon ^ { 2 } c _ { n } ^ { 2 }$ and we integrate with respect to a probability measure. Condition (8.4) now takes the form 

$$
\sum_ {k = 1} ^ {n} \frac {1}{c _ {n} ^ {2}} \alpha_ {n k} \rightarrow 0 \quad \mathrm{as} n \rightarrow \infty .\tag{8.5}
$$

Since 

$$
\sum_ {k = 1} ^ {n} (\alpha_ {n k} + \beta_ {n k}) = \sum_ {k = 1} ^ {n} \mathrm{Var} (X _ {k}) = c _ {n} ^ {2}
$$

we have 

$$
\sum_ {k = 1} ^ {n} \frac {1}{c _ {n} ^ {2}} \beta_ {n k} \rightarrow 1 \quad \mathrm{as} n \rightarrow \infty .\tag{8.6}
$$

The numbers $\alpha _ { n k } , \beta _ { n k }$ are positive so the last convergence is monotone (the sequence is increasing). The above relations hold for each $\varepsilon > 0$ 

We now analyse some terms in the expression for $\varphi _ { X _ { k } }$ . Since 

$$
\left| \int_ {| x | \geq \varepsilon c _ {n}} \theta_ {2} x ^ {2} \mathrm{d} P _ {X _ {k}} (x) \right| \leq \int_ {| x | \geq \varepsilon c _ {n}} x ^ {2} \mathrm{d} P _ {X _ {k}} (x),
$$

we have a $\theta _ { 2 } ^ { \prime }$ with $| \theta _ { 2 } ^ { \prime } | \leq 1$ such that 

$$
\int_ {| x | \geq \varepsilon c _ {n}} \theta_ {2} x ^ {2} \mathrm{d} P _ {X _ {k}} (x) = \theta_ {2} ^ {\prime} \int_ {| x | \geq \varepsilon c _ {n}} x ^ {2} \mathrm{d} P _ {X _ {k}} (x) = \theta_ {2} ^ {\prime} \alpha_ {n k}.
$$

Next 

$$
| \int_ {| x | <   \varepsilon c _ {n}} \theta_ {3} | x | ^ {3} \mathrm{d} P _ {X _ {k}} (x) | \leq \int_ {| x | <   \varepsilon c _ {n}} | x | ^ {3} \mathrm{d} P _ {X _ {k}} (x) \leq \int_ {| x | <   \varepsilon c _ {n}} \varepsilon c _ {n} x ^ {2} \mathrm{d} P _ {X _ {k}} (x)
$$

(we replace one x by $\varepsilon c _ { n }$ leaving the remaining two) hence for some $\theta _ { 3 } ^ { \prime }$ with $| \theta _ { 3 } ^ { \prime } | \leq 1$ 

$$
\left| \int_ {| x | <   \varepsilon c _ {n}} \theta_ {3} | x | ^ {3} \mathrm{d} P _ {X _ {k}} (x) \right| \leq \theta_ {3} ^ {\prime} \int_ {| x | <   \varepsilon c _ {n}} \varepsilon c _ {n} x ^ {2} \mathrm{d} P _ {X _ {k}} (x) = \theta_ {3} ^ {\prime} \varepsilon c _ {n} \beta_ {n k}.
$$

We substitute this to the expression for $\varphi _ { X _ { k } }$ obtaining 

$$
\varphi_ {X _ {k}} (u) = 1 + \frac {1}{2} u ^ {2} \theta_ {2} ^ {\prime} \alpha_ {n k} - \frac {1}{2} u ^ {2} \beta_ {n k} + \frac {1}{6} | u | ^ {3} \theta_ {3} ^ {\prime} \varepsilon c _ {n} \beta_ {n k}.
$$

Replace u by $\frac { u } { c _ { n } }$ to get 

$$
\varphi_ {X _ {k}} (\frac {u}{c _ {n}}) = 1 + \frac {1}{2} u ^ {2} \theta_ {2} ^ {\prime} \frac {1}{c _ {n} ^ {2}} \alpha_ {n k} - \frac {1}{2} u ^ {2} \frac {1}{c _ {n} ^ {2}} \beta_ {n k} + \frac {1}{6} | u | ^ {3} \theta_ {3} ^ {\prime} \varepsilon \frac {1}{c _ {n} ^ {2}} \beta_ {n k} = 1 + \gamma_ {n k}
$$

with 

$$
\gamma_ {n k} = \frac {1}{2} u ^ {2} \theta_ {2} ^ {\prime} \frac {1}{c _ {n} ^ {2}} \alpha_ {n k} - \frac {1}{2} u ^ {2} \frac {1}{c _ {n} ^ {2}} \beta_ {n k} + \frac {1}{6} | u | ^ {3} \theta_ {3} ^ {\prime} \varepsilon \frac {1}{c _ {n} ^ {2}} \beta_ {n k}.
$$

The relations (8.5), (8.6) give 

$$
\sum_ {k = 1} ^ {n} \gamma_ {n k} \rightarrow - \frac {1}{2} u ^ {2} + \frac {1}{6} | u | ^ {3} \theta_ {3} ^ {\prime} \varepsilon .\tag{8.7}
$$

Recall that what we are really after is 

$$
\log \prod_ {k = 1} ^ {n} \varphi_ {X _ {k}} (\frac {u}{c _ {n}}) = \sum_ {k = 1} ^ {n} \log \varphi_ {X _ {k}} (\frac {u}{c _ {n}}) = \sum_ {k = 1} ^ {n} (\gamma_ {n k} + \theta_ {1} | \gamma_ {n k} | ^ {2})
$$

where we introduced Taylor’s formula for the logarithm, so we are not that far from the target. All we have to do is to show that 

$$
| \log \prod_ {k = 1} ^ {n} \varphi_ {X _ {k}} (\frac {u}{c _ {n}}) + \frac {1}{2} u ^ {2} | \rightarrow 0
$$

as $n \to \infty$ . So let $\delta > 0$ be arbitrary and u fixed. 

$$
\begin{array}{r l} & {| \log \prod_ {k = 1} ^ {n} \varphi_ {X _ {k}} (\frac {u}{c _ {n}}) + \frac {1}{2} u ^ {2} |} \\ & {\leq | \sum_ {k = 1} ^ {n} \gamma_ {n k} + \frac {1}{2} u ^ {2} | + | \theta_ {1} | \sum_ {k = 1} ^ {n} | \gamma_ {n k} | ^ {2}} \\ & {\leq \left| \sum_ {k = 1} ^ {n} \gamma_ {n k} + \frac {1}{2} u ^ {2} - \frac {1}{6} | u | ^ {3} \theta_ {3} ^ {\prime} \varepsilon \right| + \sum_ {k = 1} ^ {n} | \gamma_ {n k} | ^ {2} + | u | ^ {3} \varepsilon | \theta_ {3} ^ {\prime} |.} \end{array}
$$

The first term on the right converges to zero by (8.7) so it is less than $\textstyle { \frac { \delta } { 2 } }$ for suficiently large n. It remains to show that 

$$
\sum_ {k = 1} ^ {n} | \gamma_ {n k} | ^ {2} + | u | ^ {3} \varepsilon <   \frac {\delta}{2}
$$

for large n. We choose $\varepsilon$ so small that $\begin{array} { r } { | u | ^ { 3 } \varepsilon < \frac { \delta } { 4 } } \end{array}$ . It remains to show that 

$$
\sum_ {k = 1} ^ {n} | \gamma_ {n k} | ^ {2} <   \frac {\delta}{4}
$$

for large n. We have a formula for $\gamma _ { n k }$ and we know something about $\scriptstyle \sum _ { k = 1 } ^ { n }$ γ<sub>nk</sub> hence we use the following trick 

$$
\sum_ {k = 1} ^ {n} | \gamma_ {n k} | ^ {2} \leq \max _ {k = 1, \ldots , n} | \gamma_ {n k} | \cdot \sum_ {k = 1} ^ {n} | \gamma_ {n k} |.
$$

The first factor has: 

$$
\max _ {k = 1, \dots , n} | \gamma_ {n k} | \leq \frac {1}{2} u ^ {2} \max _ {k = 1, \dots , n} | \frac {\alpha_ {n k}}{c _ {n} ^ {2}} | + \frac {1}{2} u ^ {2} \varepsilon^ {2} + \frac {1}{6} | u | ^ {3} \varepsilon^ {3}
$$

(using $\beta _ { n k } \leq \varepsilon ^ { 2 } c _ { n } ^ { 2 } )$ but 

$$
\max _ {k = 1, \dots , n} | \frac {\alpha_ {n k}}{c _ {n} ^ {2}} | \leq \sum_ {k = 1} ^ {n} \frac {\alpha_ {n k}}{c _ {n} ^ {2}} \to 0.
$$

The second factor satisfies 

$$
\sum_ {k = 1} ^ {n} | \gamma_ {n k} | \leq \frac {1}{2} u ^ {2} \sum_ {k = 1} ^ {n} \frac {1}{c _ {n} ^ {2}} \alpha_ {n k} + \frac {1}{2} u ^ {2} + \frac {1}{6} | u | ^ {3} \varepsilon
$$

where we used the fact $\begin{array} { r } { \sum \frac { \beta _ { n k } } { c _ { n } ^ { 2 } } \leq 1 } \end{array}$ . Writing $\begin{array} { r } { \sum _ { k = 1 } ^ { n } \frac { 1 } { c _ { n } ^ { 2 } } \alpha _ { n k } = a _ { n } , a _ { n } \to 0 } \end{array}$ , for clarity we have, taking $\varepsilon \leq 1$ 2 

$$
\sum_ {k = 1} ^ {n} | \gamma_ {n k} | ^ {2} \leq (\frac {u ^ {2}}{2} a _ {n} + \frac {u ^ {2} \varepsilon^ {2}}{2} + \frac {| u | ^ {3} \varepsilon^ {3}}{6}) (\frac {u ^ {2}}{2} a _ {n} + \frac {u ^ {2}}{2} + \frac {| u | ^ {3} \varepsilon}{6}) \leq C a _ {n} + D \varepsilon
$$

for some numbers (depending only on u) C, D. So finally choose $\varepsilon$ so that $\begin{array} { r } { D \varepsilon < \frac { \delta } { 8 } } \end{array}$ and then take $n _ { 0 }$ so large that $\begin{array} { r } { C a _ { n } < \frac { \delta } { 8 } } \end{array}$ for $n \geq n _ { 0 }$ □ 

As a special case we immediately deduce a famous result: 

## Corollary 8.31 (de Moivre–Laplace Theorem)

Let $X _ { n }$ be identically distributed independent random variables with $P ( X _ { n } =$ $\begin{array} { r } { 1 ) = P ( X _ { n } = - 1 ) = \frac { 1 } { 2 } } \end{array}$ . Then 

$$
P (a <   \frac {S _ {n}}{\sqrt {n}} <   b) \rightarrow \frac {1}{\sqrt {2 \pi}} \int_ {a} ^ {b} \mathrm{e} ^ {- \frac {1}{2} x ^ {2}} \mathrm{d} x.
$$

## Exercise 8.8

Use the Central Limit Theorem to estimate the probability that the number of Heads in 1000 independent tosses difers from 500 by less than 2%. 

## Exercise 8.9

How many tosses of a coin are required to have the probability at least 0.99 that the average number of Heads difers from 0.5 by less than 1%? 

## 8.2.7 Applications to mathematical finance

We shall show that the Black-Scholes model is a limit of a sequence of suitably defined CRR models with option prices converging as well. For fixed $T$ recall that in the Black-Scholes model the stock price is of the form 

$$
S (T) = S (0) \exp \{\xi (T) \}
$$

where $\begin{array} { r } { \xi ( T ) = ( r - \frac { \sigma ^ { 2 } } { 2 } ) T + \sigma w ( T ) , } \end{array}$ r is the risk-free rate for continuous compounding. Randomness is only in $w ( T )$ , which is Gaussian with zero mean and variance T. 

To construct the approximating sequence fix n to decompose the time period into n steps of length $\frac { \bar { T } } { n }$ and write 

$$
R _ {n} = \exp \{r \frac {T}{n} \},
$$

which is the risk free growth factor for one step. We construct a sequence $\eta _ { n } ( i ) , i = 1 , \ldots , n$ of independent, identically distributed random variables, with binomial distribution, so that the price in the binomial model after n steps 

$$
S _ {n} (T) = S (0) \times \eta_ {n} (1) \times \dots \times \eta_ {n} (n)
$$

converges to S(T). Write 

$$
\eta_ {n} (i) = \left\{ \begin{array}{l l} U _ {n} \\ D _ {n} \end{array} \right.
$$

where each value is taken with probability $\textstyle { \frac { 1 } { 2 } }$ . Our task is to find $U _ { n } , \ D _ { n }$ 2 assuming that $U _ { n } > D _ { n }$ . The following condition 

$$
R _ {n} = \frac {1}{2} (U _ {n} + D _ {n})\tag{8.8}
$$

guarantees that $S _ { n } ( T )$ is a martingale (see Section 7.4.3). We look at the logarithmic returns: 

$$
\ln \frac {S _ {n} (T)}{S (0)} = \ln (\eta_ {n} (1) \times \dots \times \eta_ {n} (n)) = \sum_ {i = 1} ^ {n} \ln \eta_ {n} (i).
$$

We wish to apply the Central Limit Theorem to the sequence ln $\eta _ { n } ( i )$ so we adjust the variance. We want to have 

$$
\mathrm{Var} (\ln (\eta_ {n} (1) \times \dots \times \eta_ {n} (n))) = T \sigma^ {2}.
$$

On the left, using independence, 

$$
\operatorname{Var} \left(\sum_ {i = 1} ^ {n} \ln \eta_ {n} (i)\right) = \sum_ {i = 1} ^ {n} \operatorname{Var} \left(\ln \eta_ {n} (i)\right) = n \operatorname{Var} \left(\ln \eta_ {n} (1)\right).
$$

For the binomial distribution with $\begin{array} { r } { p = \frac { 1 } { 2 } } \end{array}$ 

$$
\mathrm{Var} (\ln \eta_ {n} (1)) = \frac {1}{4} (\ln (U _ {n}) - \ln (D _ {n})) ^ {2},
$$

so the condition needed is 

$$
n \frac {1}{4} (\ln (U _ {n}) - \ln (D _ {n})) ^ {2} = T \sigma^ {2}.
$$

Since $U _ { n } > D _ { n }$ ， 

$$
\ln (\frac {U _ {n}}{D _ {n}}) = 2 \sigma \frac {\sqrt {T}}{\sqrt {n}},
$$

so finally 

$$
U _ {n} = D _ {n} \exp \{2 \sigma \sqrt {\frac {T}{n}} \}.\tag{8.9}
$$

We solve the system (8.8),(8.9) to get 

$$
\begin{array}{l} {D _ {n} = e ^ {r \frac {T}{n}} \frac {2}{1 + e ^ {2 \sigma \sqrt {T / n}}},} \\ {U _ {n} = D _ {n} e ^ {2 \sigma \sqrt {T / n}}.} \end{array}
$$

Consider the expected values 

$$
\begin{array}{c} \mathbb {E} (\ln (\eta_ {n} (1) \times \dots \times \eta_ {n} (n))) = \mathbb {E} (\sum_ {i = 1} ^ {n} \ln \eta_ {n} (i)) = n \mathbb {E} (\ln \eta_ {n} (1)) \\ = n \frac {1}{2} (\ln (U _ {n}) + \ln (D _ {n})) = a _ {n}, \end{array}
$$

say. 

Exercise 8.10 

Show that 

$$
a _ {n} \rightarrow (r - \frac {1}{2} \sigma^ {2}) T.
$$

For each n we have a sequence of n independent identically distributed random variables $\xi _ { n } ( i ) = \ln \eta _ { n } ( i )$ forming the so-called triangular array. We have the following version of Central Limit Theorem. It can be proved in exactly the same way as Theorem 8.30 (see also [2]). 

## Theorem 8.32

If $\xi _ { n } ( i )$ is a triangular array, $\begin{array} { r } { \lambda _ { n } \ = \ \sum \xi _ { n } ( i ) , \ \mathbb { E } ( \lambda _ { n } ) \ \to \ \mu \ = \ ( r - \frac { 1 } { 2 } { \sigma } ^ { 2 } ) T , } \end{array}$ $V a r ( \lambda _ { n } ) \to \sigma ^ { 2 } T$ then the sequence $\left( \lambda _ { n } \right)$ converges weakly to a Gaussian random variable with mean $\mu$ and variance $\sigma ^ { 2 } T$ 

The conditions stated in the Theorem hold true with the values assigned above to $U _ { n }$ and $D _ { n }$ , as we have seen. As a result, ln $S _ { n } ( T )$ converges to ln $S ( T )$ weakly. The value of put in the binomial model is given by 

$$
P _ {n} (0) = \exp \{- r T \} \mathbb {E} (K - S _ {n} (T)) ^ {+} = \exp \{- r T \} \mathbb {E} (g (\ln S _ {n} (T)))
$$

where $g ( x ) = ( K - \mathrm { e } ^ { x } ) ^ { + }$ is a bounded, continuous function. Therefore 

$$
P _ {n} (0) \to \exp \{- r T \} \mathbb {E} (g (\ln S (T)))
$$

which, as we know (see Exercise 4.20) , gives the Black-Scholes formula. The convergence of call prices follows immediately form the call-put parity which holds universally, in each model. 

## 8.3 Proofs of propositions

## Proof (of Proposition 8.4)

Clearly $d ( X , Y ) = d ( Y , X )$ . If $d ( X , Y ) = 0$ then $\mathbb { E } ( | X - Y | ) = 0$ hence $X = Y$ almost everywhere so $X = Y$ in $L ^ { 1 }$ . The triangle inequality follows from the triangle inequality for the metric $\textstyle \rho ( x , y ) = { \frac { | x - y | } { 1 + | x - y | } }$ 

Next, assume that $X _ { n } \to X$ in probability. Let $\varepsilon > 0$ 

$$
\begin{array}{l} d (X _ {n}, X) = \int_ {| X _ {n} - X | <   \frac {\varepsilon}{2}} \frac {| X _ {n} - X |}{1 + | X _ {n} - X |} \mathrm{d} P \\ \qquad + \int_ {| X _ {n} - X | \geq \frac {\varepsilon}{2}} \frac {| X _ {n} - X |}{1 + | X _ {n} - X |} \mathrm{d} P \\ \qquad \leq \frac {\varepsilon}{2} + P (| X _ {n} - X | \geq \frac {\varepsilon}{2}) \end{array}
$$

since the integrand in the first term is less than ε (estimating the denominator by 1) and we estimate the integrand in the second term by 1. For n large enough the second term is less than $\frac { \varepsilon } { 2 }$ . 

Conversely, let $E _ { \varepsilon , n } = \{ \omega : | X _ { n } ( \omega ) - X ( \omega ) | > \varepsilon \}$ and assume $0 < \varepsilon < 1$ Additionally let $A _ { n } = \{ \omega : | X _ { n } ( \omega - X ( \omega ) | < 1 \}$ and write 

$$
d (X _ {n} X) = \int_ {A _ {n}} \frac {| X _ {n} - X |}{1 + | X _ {n} - X |} \mathrm{d} P + \int_ {A _ {n} ^ {c}} \frac {| X _ {n} - X |}{1 + | X _ {n} - X |} \mathrm{d} P.
$$

We estimate from below each of the two terms. First, 

$$
\begin{array}{l} \int_ {A _ {n}} \frac {| X _ {n} - X |}{1 + | X _ {n} - X |} \mathrm{d} P \geq \int_ {A _ {n} \cap E _ {\varepsilon , n}} \frac {| X _ {n} - X |}{1 + | X _ {n} - X |} \mathrm{d} P \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \geq \frac {1}{2} \int_ {A _ {n} \cap E _ {\varepsilon}} \varepsilon   \mathrm{d} P \\ \qquad \qquad \qquad = \frac {\varepsilon}{2} P (A _ {n} \cap E _ {\varepsilon , n}) \end{array}
$$

since $\textstyle { \frac { a } { 1 + a } } > { \frac { a } { 2 } }$ if $a < 1$ . Second, 

$$
\int_ {A _ {n} ^ {c}} \frac {| X _ {n} - X |}{1 + | X _ {n} - X |} \mathrm{d} P \geq \int_ {A _ {n} ^ {c}} \frac {1}{2} \mathrm{d} P \geq \int_ {A _ {n} ^ {c} \cap E _ {\varepsilon , n}} \frac {1}{2} \mathrm{d} P \geq \frac {\varepsilon}{2} P (A _ {n} \cap E _ {\varepsilon , n})
$$

since $\varepsilon \smile 1$ . Hence, $d ( X _ { n } , X ) \geq { \frac { \varepsilon } { 2 } } P ( E _ { \varepsilon , n } ) \to 0 , { \mathrm { ~ s o ~ } } ( X _ { n } )$ converges to $X$ in probability. □ 

Proof (of Proposition 8.6) 

First 

$$
\begin{array}{c} \mathbb {E} (Y ^ {p}) = \int_ {\{\omega : Y (\omega) \geq \varepsilon \}} Y ^ {p}   \mathrm{d} P + \int_ {\{\omega : Y (\omega) <   \varepsilon \}} Y ^ {p}   \mathrm{d} P \\ \geq \varepsilon^ {p} P (Y \geq \varepsilon) + \int_ {\{\omega : Y (\omega) <   \varepsilon \}} Y ^ {p}   \mathrm{d} P. \end{array}
$$

Now if we let $\varepsilon  \infty$ , then the second term converges to $\begin{array} { r } { \int _ { \Omega } Y ^ { p } \mathrm { d } P = \mathbb { E } ( Y ^ { p } ) } \end{array}$ and the first term has no choice but to converge to 0. □ 

## Proof (of Proposition 8.13)

(i) Write $A = \operatorname* { l i m } \operatorname* { i n f } _ { n \to \infty } A _ { n } . { \mathrm { ~ I f ~ } } \omega \in A$ then there is an N such that $\omega \in A _ { n }$ for all $n \geq N .$ , which implies $\omega \in A _ { n }$ for all except finitely many n. Conversely, if $n \in A _ { n }$ eventually, then there exists N such that $\omega \in A _ { n }$ for all $n \geq N$ and $\omega \in A$ 

(ii) Fix $\varepsilon > 0$ . If $A _ { n } ^ { \varepsilon } \ = \ \{ | X _ { n } - X | \ < \ \varepsilon \}$ then $\left\{ \left| X _ { n } - X \right| < \varepsilon { \mathrm { ~ e . v . } } \right\} =$ lim in $\operatorname { f } _ { n \to \infty } A _ { n } ^ { \varepsilon } = A ^ { \varepsilon }$ , say. But 

$$
\left\{X _ {n} \rightarrow X \right\} = \bigcap_ {\varepsilon > 0} \left\{\left| X _ {n} - X \right| <   \varepsilon \text {ev.} \right\} = \bigcap_ {\varepsilon > 0} A ^ {\varepsilon}
$$

and the sets $A ^ { \varepsilon }$ decrease as $\varepsilon \searrow 0$ . Taking $\textstyle { \varepsilon = { \frac { 1 } { n } } }$ successively shows that 

$$
P (X _ {n} \to X) = P (\bigcap_ {n = 1} ^ {\infty} \liminf A _ {n} ^ {1 / n}) = \lim _ {\varepsilon \to 0} A ^ {\varepsilon} = \lim _ {\varepsilon \to 0} P (| X _ {n} - X | <   \varepsilon \text {   ev. } \}.
$$

(iii) By de Morgan 

$$
(\bigcap_ {n = 1} ^ {\infty} \bigcup_ {m = n} ^ {\infty} A _ {m}) ^ {c} = \bigcup_ {n = 1} ^ {\infty} (\bigcup_ {m = n} ^ {\infty} A _ {m}) ^ {c} = \bigcup_ {n = 1} ^ {\infty} \bigcap_ {m = n} ^ {\infty} A _ {m} ^ {c}.
$$

(iv) If $A = \operatorname* { l i m } \operatorname* { i n f } _ { n \to \infty } A _ { n }$ then $\mathbf { 1 } _ { A } \ = \ \operatorname* { l i m } \operatorname* { i n f } _ { n \to \infty } \mathbf { 1 } _ { A _ { n } }$ (since $\mathbf { 1 } _ { A } ( \omega ) =$ 1 if and only if ${ \bf 1 } _ { A _ { n } } ~ = ~ 1 ~ \mathrm { e v . } )$ and if $B \ = \ \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } A _ { n }$ , then $\begin{array} { r l } { \mathbf { 1 } _ { B } } & { { } = } \end{array}$ lim $\operatorname* { s u p } _ { n \to \infty } { \mathbf { 1 } } _ { A _ { n } }$ (since $\mathbf { 1 } _ { B } ( \omega ) = 1$ if and only if $\mathbf { 1 } _ { A _ { n } } = 1 \ { \mathrm { i . o . } } )$ . Fatou’s lemma implies 

$$
P (A _ {n} \text {   ev. }) = \int_ {\Omega} \liminf _ {n \to \infty} \mathbf {1} _ {A _ {n}}   \mathrm{d} P \leq \liminf _ {n \to \infty} \int_ {\Omega} \mathbf {1} _ {A _ {n}}   \mathrm{d} P
$$

that is 

$$
P (B) \leq \liminf _ {n \to \infty} P (A _ {n}) \leq \limsup _ {n \to \infty} P (A _ {n}).
$$

But 

$$
\limsup _ {n \to \infty} P (A _ {n}) = \limsup _ {n \to \infty} \int_ {\Omega} \mathbf {1} _ {A _ {n}}   \mathrm{d} P \leq \int_ {\Omega} \limsup _ {n \to \infty} \mathbf {1} _ {A _ {n}}   \mathrm{d} P
$$

$$
\limsup _ {n \to \infty} P (A _ {n}) = \int_ {\Omega} \mathbf {1} _ {A}   \mathrm{d} P = P (A) = P (A _ {n} \text {   i.o. }).
$$

by Fatou in reverse (see the proof of Theorem 4.18), hence 

## Chapter 2

2.1 If we can cover A by open intervals with prescribed total length, then we can also cover A by closed intervals with the same endpoints (closed intervals are bigger), and the total length is the same. The same is true for any other kind of intervals. For the converse, suppose that A is null in the sense of covering by closed intervals. Let $\varepsilon > 0$ , take a cover ${ \cal C } _ { n } = [ a _ { n } , b _ { n } ]$ with $\textstyle \sum _ { n } ( b _ { n } - a _ { n } ) < { \frac { \varepsilon } { 2 } }$ , let $\begin{array} { r } { I _ { n } = ( a _ { n } - \varepsilon \frac { 1 } { 2 ^ { n + 2 } } , b _ { n } + \varepsilon \frac 1 { 2 ^ { n + 2 } } ) } \end{array}$ . They are bigger so Pthey cover $A ;$ ; the total length is less than ε. In the same way we refine the cover by any other kind of intervals. 

2.2 Write each element of $C$ in ternary form. Suppose C is countable and so they can be arranged in a sequence. Define a number which is not in this sequence but has ternary expansion and so is in $C ,$ by exchanging 0 and 2 at the nth position. 

2.3 For continuity at $x \in [ 0 , 1 ]$ take any $\varepsilon > 0$ and find $F ( x ) \mathrm { ~ - ~ } \varepsilon < a <$ $F ( x ) < b < F ( x ) + \varepsilon$ of the form $\textstyle a = { \frac { k } { 2 ^ { n } } } , b = { \frac { m } { 2 ^ { n } } }$ . By the construction of $F ,$ these numbers are values of $F$ taken on some intervals $( a _ { 1 } , a _ { 2 } ) , ( b _ { 1 } , b _ { 2 } )$ , with ternary ends, and $a _ { 1 } < x < b _ { 2 }$ . Take a $\delta$ such that $a _ { 1 } < x - \delta < x + \delta < b _ { 2 }$ to get the continuity condition. For the graph, see Figure 4.7. 

2.4 $m ^ { * } ( B ) \leq m ^ { * } ( A \cup B ) \leq m ^ { * } ( A ) + m ^ { * } ( B ) = m ^ { * } ( B )$ by monotonicity (Proposition 2.3) and subadditivity (Theorem 2.5). Thus $m ^ { * } ( A \cup B )$ is squeezed between $m ^ { * } ( B )$ and $m ^ { * } ( B )$ so has little choice. 

2.5 Since $A \subset B \cup ( A \varDelta B ) , m ^ { * } ( A ) \leq m ^ { * } ( B ) + m ^ { * } ( A \varDelta B ) = m ^ { * } ( B )$ (monotonic-

ity and subadditivity), and the inverse is shown in the same way. 

2.6 Since $A \cup B = A \cup ( B \setminus A ) = A \cup ( B \setminus ( A \cap B ) )$ , using additivity and Proposition 2.10 we have $P ( A \cup B ) = P ( A ) + P ( B ) - P ( A \cap B )$ . Similarly $P ( A \cup B \cup C ) = P ( A ) + P ( B ) + P ( C ) - P ( A \cap B ) - P ( A \cap C ) - P ( B \cap C ) .$ $C ) + P ( A \cap B \cap C )$ 

2.7 It is suficient to note that 

$$
(a, b) = \bigcup_ {n = 1} ^ {\infty} (a, b - \frac {1}{n} ], \quad (a, b) = \bigcup_ {n = 1} ^ {\infty} [ a + \frac {1}{n}, b).
$$

2.8 If E is Lebesgue measurable, then existence of O and F is given by Theorems 2.12 and 2.19, respectively. Conversely, let $\textstyle { \varepsilon = { \frac { 1 } { n } } }$ , find $O _ { n } , F _ { n }$ , and then $m ^ { * } ( \bigcap O _ { n } \setminus E ) = 0 , m ^ { * } ( E \setminus \bigcup F _ { n } ) = 0$ so E is Borel up to null set. THence E is in . 

2.9 We can decompose A into $\textstyle \bigcup _ { i = 1 } ^ { \infty } ( A \cap H _ { i } )$ ; the components are pairwise disjoint, so 

$$
P (A) = \sum_ {i = 1} ^ {\infty} P (A \cap H _ {i}) = \sum_ {i = 1} ^ {\infty} P (A | H _ {i}) \cdot P (H _ {i})
$$

using the definition of conditional probability. 

2.10 Since $A ^ { \mathsf { c } } \cap B = ( { \boldsymbol { \varOmega } } \setminus A ) \cap B = B \setminus ( A \cap B ) , P ( A ^ { \mathsf { c } } \cap B ) = P ( B ) - P ( A \cap B ) =$ $P ( B ) - P ( A ) \cdot P ( B ) = P ( B ) ( 1 - P ( A ) ) = P ( B ) \cdot P ( A ^ { \mathrm { c } } ) .$ 

2.11 There are 32 paths altogether. $S ( 5 ) = 5 2 4 . 8 8 = 5 0 0 U ^ { 2 } D ^ { 3 }$ so there are ${ \binom { 5 } { 2 } } = 1 0$ paths. $S ( 5 ) > 9 0 0$ in two cases: $S ( 5 ) = 1 2 4 4 . 1 6 = 5 0 0 U ^ { 5 } \mathrm { o r } S ( 5 ) =$ $9 3 3 . 1 2 = 5 0 0 U ^ { 4 } D$ so we have 6 paths with probability $0 . 5 ^ { 5 } = 0 . 0 3 1 2 5$ each so the probability in question is 0.1875. 

2.12 There are $2 ^ { m }$ paths of length m, $\mathcal { F } _ { m }$ can be identified with the power set of the set of all such paths, thus it has $2 ^ { 2 ^ { n } }$ elements. 

2.13 $\mathcal { F } _ { m } \subset \mathcal { F } _ { m + 1 }$ since if the first $m + 1$ elements of a sequence are identical, so are the first m elements. 

2.14 It sufices to note that $\begin{array} { r } { P ( A _ { m } \cap A _ { k } ) = \frac { 1 } { 4 } } \end{array}$ , which is the same as $P ( A _ { m } ) P ( A _ { k } )$ 

## Chapter 3

3.1 If f is monotone (in the sense that $x _ { 1 } \leq x _ { 2 }$ implies $f ( x _ { 1 } ) \leq f ( x _ { 2 } ) )$ , the inverse image of interval $( a , \infty )$ is either $[ b , \infty )$ or $( b , \infty )$ with $b = \operatorname* { s u p } \{ x :$ $f ( x ) \leq a \}$ , so it is obviously measurable. 

3.2 The level set $\{ x \ : \ f ( x ) \ = \ a \}$ is the intersection of $f ^ { - 1 } ( [ a , \infty ) )$ and $f ^ { - 1 } ( ( - \infty , a ] )$ , each measurable by Theorem 3.1. 

3.3 If $b \geq a$ , then $( f ^ { a } ) ^ { - 1 } ( ( - \infty , b ] ) = \mathbb { R }$ , and if $b < a$ , then $( f ^ { a } ) ^ { - 1 } ( ( - \infty , b ] ) =$ $f ^ { - 1 } ( ( - \infty , b ] )$ ; in each case a measurable set. 

3.4 Let A be a non-measurable set and let $f ( x ) = 1 { \mathrm { ~ i f ~ } } x \in A , f ( x ) = - 1$ otherwise. The set $f ^ { - 1 } ( [ 1 , \infty ) )$ is non-measurable (it is A) so f is nonmeasurable, but $f ^ { 2 } \equiv 1$ which is clearly measurable. 

3.5 Let g(x) = lim sup $f _ { n } ( x ) , h ( x ) = \operatorname* { l i m } \operatorname* { i n f } f _ { n } ( x )$ ; they are measurable by Theorem 3.5. Their diference is also measurable and the set where $f _ { n }$ converges is the level set of this diference: $\{ x : f _ { n } { \mathrm { ~ c o n v e r g e s } } \} = \{ x : ( h - g ) ( x ) = 0 \}$ hence is measurable. 

3.6 If sup $f = \infty$ then there is nothing to prove. If sup f = M, then $f ( x ) \leq M$ for all x so M is one of the z in the definition of ess sup. Let f be continuous and suppose ess $\operatorname* { s u p } f < M$ finite. Then we take z between these numbers and by the definition of ess sup, $f ( x ) \leq z { \mathrm { ~ a . e ~ } }$ . Hence $A = \{ x : f ( x ) > z \}$ is null. However, by continuity A contains the set $f ^ { - 1 } ( ( z , M ) )$ ) which is open – a contradiction. If sup f is infinite, then for each z the condition $f ( x ) \leq z$ a.e. does not hold. The infimum of the empty set is + so we are done. 

3.7 It is suficient to notice that if is any σ-field containing the inverse images of Borel sets, then ${ \mathcal { F } } _ { X } \subset { \mathcal { G } }$ 

3.8 Let $f : \mathbb { R }  \mathbb { R }$ be given by $f ( x ) = x ^ { 2 }$ . The complement of the set f(R) equal to $( - \infty , 0 )$ cannot be of the form f(A) since each of these is contained in $[ 0 , \infty )$ 

3.9 The payof of a down-and-out European call is $f ( ( S ( 0 ) , S ( 1 ) , \dots , S ( n ) ) )$ with $f ( x _ { 0 } , x _ { 1 } , \ldots , x _ { N } ) = ( x _ { N } - K ) ^ { + } \cdot { \bf 1 } _ { A }$ , where $A = \left\{ \left( x _ { 0 } , x _ { 1 } , \ldots , x _ { N } \right) : \right.$ min $\{ x _ { 0 } , x _ { 1 } , \ldots , x _ { N } \} \ge L \}$ 

## Chapter 4

4.1 (a) $\begin{array} { r } { \int _ { 0 } ^ { 1 0 } \operatorname { I n t } ( x ) \mathrm { d } x = 0 m ( [ 0 , 1 ) ) + 1 m ( [ 1 , 2 ) ) + 2 m ( [ 2 , 3 ) ) + \cdot \cdot \cdot + 9 m ( [ 9 , 1 0 ) ) + } \end{array}$ 10m $( [ 1 0 , 1 0 ] ) = 4 5$ (b) $\begin{array} { r } { \int _ { 0 } ^ { 4 } \operatorname { I n t } ( \dot { x ^ { 2 } } ) \mathrm { d } x = 0 m ( [ 0 , 1 ] ) + 1 m ( [ 1 , \sqrt { 2 } ) ) + 2 m ( [ \sqrt { 2 } , \sqrt { 3 } ) ) + 3 m ( [ \sqrt { 3 } , 4 ) ) = } \end{array}$ $5 - { \sqrt { 3 } } - { \sqrt { 2 } } .$ (c) $\begin{array} { r } { \int _ { 0 } ^ { 2 \pi } \operatorname { I n t } ( \sin x ) \mathrm { d } x = 0 m ( [ 0 , \frac { \pi } { 2 } ) ) + 1 m ( [ \frac { \pi } { 2 } , \frac { \pi } { 2 } ] ) + 0 m ( ( \frac { \pi } { 2 } , \pi ] ) - 1 m ( ( \pi , 2 \pi ] ) = 0 . } \end{array}$ −<sup>π.</sup> 

4.2 We have $\begin{array} { r } { f ( x ) = \sum _ { k = 1 } ^ { \infty } k 2 ^ { k - 1 } \mathbf { 1 } _ { A _ { k } } ( x ) } \end{array}$ , where $A _ { k }$ is the union of $2 ^ { k - 1 }$ intervals of length $\textstyle { \frac { 1 } { 3 ^ { k } } }$ Peach, that are removed from [0, 1] at the kth stage. The 

convergence is monotone so 

$$
\int_ {[ 0, 1 ]} f \mathrm{d} m = \lim _ {n \to \infty} \sum_ {k = 1} ^ {n} k \frac {2 ^ {k - 1}}{3 ^ {k}} = \frac {1}{3} \sum_ {k = 1} ^ {\infty} k \left(\frac {2}{3}\right) ^ {k - 1}.
$$

Since $\begin{array} { r } { \sum _ { k = 1 } ^ { \infty } \alpha ^ { k } = \frac { 1 } { 1 - \alpha } , } \end{array}$ , diferentiating term by term with respect to α we have $\begin{array} { r } { \sum _ { k = 1 } ^ { \infty } k \alpha ^ { k - 1 } = \frac { 1 } { ( 1 - \alpha ) ^ { 2 } } } \end{array}$ . With $\begin{array} { r } { \alpha = \frac { 2 } { 3 } } \end{array}$ we get $\textstyle \int _ { [ 0 , 1 ] } f \mathrm { d } m = 3$ 

4.3 The simple function $a \mathbf { 1 } _ { A }$ is less than f so its integral, equal to $a m ( A )$ , is smaller than the integral of f. Next, $f \leq b \mathbf { 1 } _ { A }$ , hence the second inequality. 

4.4 Let $f _ { n } = n { \bf 1 } _ { ( 0 , \frac { 1 } { n } ] } ;$ lim $f _ { n } ( x ) = 0$ for all x but $\textstyle \int f _ { n } \mathrm { d } m = 1$ 

4.5 Let $\alpha \neq - 1$ . We have $\textstyle \int x ^ { \alpha } \mathrm { d } x = { \frac { 1 } { \alpha + 1 } } x ^ { \alpha + 1 }$ (indefinite integral). First consider $E = ( 0 , 1 )$ : 

$$
\int_ {0} ^ {1} x ^ {\alpha} \mathrm{d} x = \frac {1}{\alpha + 1} \left. x ^ {\alpha + 1} \right| _ {0} ^ {1}
$$

which is finite if $\alpha > - 1$ . Next $E = ( 1 , \infty )$ : 

$$
\int_ {1} ^ {\infty} x ^ {\alpha} \mathrm{d} x = \frac {1}{\alpha + 1} \lim _ {n \rightarrow \infty} \left. x ^ {\alpha + 1} \right| _ {1} ^ {n}
$$

and for this to be finite we need $\alpha < - 1$ 

4.6 The sequence $\textstyle f _ { n } ( x ) \ = \ { \frac { \sqrt { x } } { 1 + n x ^ { 3 } } }$ converges to 0 pointwise, $\begin{array} { r } { \frac { \sqrt { x } } { 1 + n x ^ { 3 } } \leq \frac { \sqrt { x } } { n x ^ { 3 } } \leq } \end{array}$ ${ \scriptstyle { \frac { 1 } { n } } } x ^ { - 2 . 5 } \leq x ^ { - 2 . 5 }$ which is integrable on $\lbrack 1 , \infty )$ , so the sequence of integrals converges to 0. 

4.7 First $a = 0$ . Substitute $u = n x \colon$ 

$$
\int_ {0} ^ {\infty} \frac {n ^ {2} x \mathrm{e} ^ {- n ^ {2} x ^ {2}}}{1 + x ^ {2}} \mathrm{d} x = \int_ {0} ^ {\infty} \frac {u \mathrm{e} ^ {- u ^ {2}}}{1 + (\frac {u}{n}) ^ {2}} \mathrm{d} u.
$$

The sequence of integrands converges to $u \mathrm { e } ^ { - u ^ { 2 } }$ for all $u \geq 0$ , it is dominated by $g ( u ) = u \mathrm { e } ^ { - u ^ { 2 } }$ , so 

$$
\lim \int_ {0} ^ {\infty} f _ {n} \mathrm{d} m = \int_ {0} ^ {\infty} \lim f _ {n} \mathrm{d} m = \int_ {0} ^ {\infty} u \mathrm{e} ^ {- u ^ {2}} \mathrm{d} u = \frac {1}{2}.
$$

Now $a > 0$ . After the same substitution we have 

$$
\int_ {a} ^ {\infty} \frac {n ^ {2} x \mathrm{e} ^ {- n ^ {2} x ^ {2}}}{1 + x ^ {2}} \mathrm{d} x = \int_ {\mathbb {R}} \frac {u \mathrm{e} ^ {- u ^ {2}}}{1 + (\frac {u}{n}) ^ {2}} \mathbf {1} _ {[ n a, \infty)} (u) \mathrm{d} u = \int_ {\mathbb {R}} f _ {n} (u) \mathrm{d} u,
$$

say, and $f _ { n } \to 0 , f _ { n } ( u ) \leq u \mathrm { e } ^ { - u ^ { 2 } }$ , so lim $\textstyle \int f _ { n } \mathrm { d } m = 0$ 

4.8 The sequence $f _ { n } ( x )$ converges for $x \ge 0$ to $\mathrm { e } ^ { - x }$ . We find the dominating function. Let $n > 1$ . For $x \in ( 0 , 1 ) , x ^ { \frac { 1 } { n } } \geq x ^ { \frac { 1 } { 2 } } , ( 1 + { \frac { x } { n } } ) ^ { n } \geq 1$ , so $\textstyle f _ { n } ( x ) \leq { \frac { 1 } { \sqrt { x } } }$ which is integrable over (0, 1). For $x \in [ 1 , \infty ) , x ^ { - { \frac { 1 } { n } } } \leq 1 , \mathrm { { s o } } \ f _ { n } ( x ) \leq ( 1 +$ $\textstyle { \frac { x } { n } } ) ^ { - n }$ . Next 

$$
\left(1 + \frac {x}{n}\right) ^ {n} = 1 + x + \frac {n (n - 1)}{2 !} \left(\frac {x}{n}\right) ^ {2} + \dots > x ^ {2} \frac {n - 1}{2 n} \geq \frac {1}{4} x ^ {2}
$$

so $\textstyle f _ { n } ( x ) \leq { \frac { 4 } { x ^ { 2 } } }$ which is integrable over $[ 1 , \infty )$ 

Therefore, by the dominated convergence theorem, 

$$
\lim \int_ {0} ^ {\infty} f _ {n} \mathrm{d} m = \int_ {0} ^ {\infty} \mathrm{e} ^ {- x} \mathrm{d} x = 1.
$$

4.9 (a) $\begin{array} { r } { \int _ { - 1 } ^ { 1 } | n ^ { a } x ^ { n } | \mathrm { d } x = n ^ { a } \int _ { - 1 } ^ { 1 } | x | ^ { n } \mathrm { d } x = n ^ { a } \int _ { 0 } ^ { 1 } x ^ { n } } \end{array}$ dx $( | x | ^ { n }$ is an even function) $\begin{array} { r l r } { \mathrm { ~ } } & { { } } & { = \frac { 2 n ^ { a } } { n + 1 } } \end{array}$ . If $a < 0$ , then the series $\sum { _ { n \geq 1 } { \frac { 2 n ^ { a } } { n + 1 } } }$ converges by comparison with $\frac { 1 } { n ^ { 1 - \alpha } }$ P, we may apply the Beppo–Levi theorem and the power series in question defines an integrable function. If $a = 0$ the series is $\textstyle \sum _ { n \geq 1 } x ^ { n } = { \frac { x } { 1 - x } }$ which is not integrable since $\begin{array} { r } { \int _ { - 1 } ^ { 1 } ( \sum _ { n \geq 1 } x ^ { n } ) \mathrm { d } x = \sum _ { n = 1 } ^ { \infty } \int _ { - 1 } ^ { 1 } x ^ { n } \mathrm { d } x = \infty } \end{array}$ . By R P P Rcomparison the series fails to give an integrable function if $a > 0$ 

(b) Write $\begin{array} { r } { \frac { x } { \mathrm { e } ^ { x } - 1 } = x \frac { \mathrm { e } ^ { - x } } { 1 - \mathrm { e } ^ { - x } } = \sum _ { n > 1 } x \mathrm { e } ^ { - n x } , \int _ { 0 } ^ { \infty } x \mathrm { e } ^ { - n x } \mathrm { d } x = x ( - \frac { 1 } { n } ) \mathrm { e } ^ { - n x } | _ { 0 } ^ { \infty } - } \end{array}$ $\begin{array} { r } { \left( - \frac { 1 } { n } \right) \int _ { 0 } ^ { \infty } \mathrm { e } ^ { - n x } \mathrm { d } x = \frac { 1 } { n ^ { 2 } } } \end{array}$ P R(integration by parts) and, as is well known, $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } \frac { 1 } { n ^ { 2 } } = \frac { \pi ^ { 2 } } { 6 } } \end{array}$ 

4.10 We extend f by putting $f ( 0 ) = 1$ so that f is continuous hence Riemann integrable on any finite interval. Let $\begin{array} { r } { a _ { n } = \int _ { n \pi } ^ { ( n + 1 ) \pi } f ( x ) } \end{array}$ dx. Since f is even, $a _ { - n } = a _ { n }$ and hence $\textstyle { \int _ { - \infty } ^ { \infty } f ( x ) \mathrm { d } x = 2 \sum _ { n = 0 } ^ { \infty } a _ { n } }$ . The series converges since $\begin{array} { r } { a _ { n } = ( - 1 ) ^ { n } | a _ { n } | , | a _ { n } | \le \frac { 2 } { n \pi } ( x \ge n \pi , | \int _ { n \pi } ^ { ( n + 1 ) } \sin x \mathrm { d } x | = 2 ) } \end{array}$ . However for f to be in $L ^ { 1 }$ we would need $\begin{array} { r } { \int _ { \mathbb { R } } | f | \mathrm { d } m \stackrel { \cdots } { = } 2 \sum _ { n = 0 } ^ { \infty } b _ { n } } \end{array}$ finite, where $b _ { n } \ =$ $\begin{array} { r } { \int _ { n \pi } ^ { ( n + 1 ) \pi } | f ( x ) | \mathrm { d } x } \end{array}$ . This is impossible due to $\begin{array} { r } { b _ { n } \ge \frac { 2 } { ( n + 1 ) \pi } } \end{array}$ 

4.11 Denote $\begin{array} { r } { \int _ { - \infty } ^ { \infty } \operatorname { e } ^ { - x ^ { 2 } } \mathrm { d } x = I ; } \end{array}$ ; then 

$$
I ^ {2} = \int \int_ {\mathbb {R} ^ {2}} \mathrm{e} ^ {- (x ^ {2} + y ^ {2})} \mathrm{d} x \mathrm{d} y = \int_ {0} ^ {2 \pi} \int_ {0} ^ {\infty} r \mathrm{e} ^ {- r ^ {2}} \mathrm{d} r \mathrm{d} \alpha = \pi
$$

using polar coordinates and Fubini’s theorem (Chapter 6). 

Substitute $\begin{array} { r } { x = { \frac { z - \mu } { \sqrt { 2 } \sigma } } } \end{array}$ in $\begin{array} { r } { I ; \sqrt { \pi } = \int _ { - \infty } ^ { \infty } \mathrm { e } ^ { - x ^ { 2 } } \mathrm { d } x = \frac { 1 } { \sqrt { 2 } \sigma } \int _ { - \infty } ^ { \infty } \mathrm { e } ^ { - \frac { ( z - \mu ) ^ { 2 } } { 2 \sigma ^ { 2 } } } \mathrm { d } z , } \end{array}$ which completes the computation. 

4.12 $\begin{array} { r } { \int _ { \mathbb { R } } \frac { 1 } { 1 + x ^ { 2 } } \mathrm { d } x = \mathrm { a r c } \tan x | _ { - \infty } ^ { + \infty } = \pi \mathrm { ~ h e n c e ~ } \int _ { - \infty } ^ { \infty } c ( x ) \mathrm { d } x = 1 . } \end{array}$ 

4.13 $\begin{array} { r } { \int _ { 0 } ^ { \infty } \mathrm { e } ^ { - \lambda x } \mathrm { d } x = - \frac { 1 } { \lambda } \mathrm { e } ^ { - \lambda x } | _ { 0 } ^ { \infty } = \frac { 1 } { \lambda } } \end{array}$ , hence $c = \lambda$ 

4.14 Let $a _ { n }  0 , a _ { n } \geq 0$ . Then $\begin{array} { r } { P _ { X } ( \{ y \} ) = \operatorname* { l i m } _ { n \to \infty } P _ { X } ( ( y - a _ { n } , y ] ) = F _ { X } ( y ) - } \end{array}$ $\scriptstyle \operatorname* { l i m } _ { n \to \infty } F _ { X } ( y - a _ { n } )$ which proves the required equivalence. (Recall that $P _ { X }$ is always right-continuous.) 

4.15 (a) $F _ { X } ( y ) = 1$ for $y \geq a$ and zero otherwise. 

(b) $F _ { X } ( y ) = 0$ for $y \ < \ 0 , \ F _ { X } ( y ) = 1$ for $y \geq \frac 1 2$ , and $F _ { X } ( y ) = 2 y$ otherwise. 

(c) $F _ { X } ( y ) = 0$ for $y < 0 , F _ { X } ( y ) = 1$ for $\begin{array} { r } { y \ge \frac { 1 } { 2 } } \end{array}$ , and $F _ { X } ( y ) = 1 - ( 1 - 2 y ) ^ { 2 }$ otherwise. 

4.16 In this case $\begin{array} { r } { \varphi ( x ) = x ^ { 3 } , \varphi ^ { - 1 } ( y ) = \sqrt [ 3 ] { y } , \frac { \mathrm { d } } { \mathrm { d } y } \varphi ^ { - 1 } ( y ) = \frac { 1 } { 3 } y ^ { - \frac { 2 } { 3 } } } \end{array}$ hence $f _ { X ^ { 3 } } ( y ) =$ $\mathbf { 1 } _ { [ 0 , 1 ] } ( \sqrt [ 3 ] { y } ) \frac { 1 } { 3 } y ^ { - \frac { 2 } { 3 } } = \frac { 1 } { 3 } y ^ { - \frac { 2 } { 3 } } \mathbf { 1 } _ { [ 0 , 1 ] } ( y )$ 

4.17 (a) $\begin{array} { r } { \int _ { \Omega } a \mathrm { d } P = a P ( \Omega ) = a } \end{array}$ (constant function is a simple function). 

(b) Using Exercise 4.15 $\begin{array} { r } { f _ { X } ( x ) = 2 \mathbf { 1 } _ { [ 0 , \frac { 1 } { 2 } ] } ( x ) \operatorname { s o } E ( X ) = \int _ { 0 } ^ { \frac { 1 } { 2 } } 2 x \mathrm { d } x = \frac { 1 } { 4 } . } \end{array}$ 

(c) Again by Exercise 4.15, $\begin{array} { r } { f _ { X } = 4 x \mathbf { 1 } _ { [ 0 , \frac { 1 } { 2 } ] } ( x ) , E ( X ) = \int _ { 0 } ^ { \frac { 1 } { 2 } } 4 x ^ { 2 } \mathrm { d } x = \frac { 1 } { 6 } } \end{array}$ 

4.18 (a) With $\begin{array} { r } { f _ { X } = \frac { 1 } { b - a } \mathbf { 1 } _ { [ a , b ] } , E ( X ) = \frac { 1 } { b - a } \int _ { a } ^ { b } x \mathrm { d } x = \frac { 1 } { b - a } \frac { 1 } { 2 } ( b ^ { 2 } - a ^ { 2 } ) = \frac { 1 } { 2 } ( a + b ) } \end{array}$ 

R(b) Consider the simple triangle distribution with $f _ { X } ( x ) = x + 1$ for $x \in [ - 1 , 0 ] , f _ { X } ( x ) = - x + 1$ for $x \in ( 0 , 1 ]$ and zero elsewhere. Then immediately $\begin{array} { r } { \int _ { - 1 } ^ { 1 } x f _ { X } ( x ) \mathrm { d } x = 0 . } \end{array}$ . A similar computation for the density $f _ { Y }$ whose triangle’s base is $[ a , b ]$ gives $\textstyle E ( X ) = { \frac { a + b } { 2 } }$ 

(c) $\begin{array} { r } { \lambda \int _ { 0 } ^ { \infty } x \mathrm { e } ^ { - \lambda x } \mathrm { d } x = \frac { 1 } { \lambda } } \end{array}$ (integration by parts). 

4.19 (a) $\begin{array} { r } { \varphi _ { X } ( t ) = \frac { 1 } { ( b - a ) \mathrm { i } t } ( \mathrm { e } ^ { \mathrm { i } b t } - \mathrm { e } ^ { \mathrm { i } a t } ) } \end{array}$ 2 

(b) ϕ<sub>X</sub> (t) = λ ∞<sub>0</sub> e(it−λ)xdx = λ it λ 

(c) $\varphi _ { X } ( t ) = \mathrm { e } ^ { \mathrm { i } \mu t - \frac { 1 } { 2 } \sigma ^ { 2 } t ^ { 2 } } .$ 

4.20 Using call-put parity, the formula for the call and symmetry of the Gaussian distribution we have $P = S ( 0 ) ( N ( d _ { 1 } ) - 1 ) - K \mathrm { e } ^ { - r T } ( N ( d _ { 2 } ) - 1 ) =$ $- S ( 0 ) N ( - d _ { 1 } ) + K \mathrm { e } ^ { - r T } N ( - d _ { 2 } )$ 

## Chapter 5

5.1 First $f \equiv f$ as $f = f$ everywhere. Second, if $f = g { \mathrm { ~ a . e . } }$ , then of course $g = f$ a.e. Third, if $f = g$ on a full set $F _ { 1 } \subset E \left( m ( E \setminus F _ { 1 } ) = 0 \right)$ and $g = h$ on a full set $F _ { 2 } \subset E$ , then $f = h$ on $F _ { 1 } \cap F _ { 2 }$ which is full as well. 

5.2 (a) $\| f _ { n } - f _ { m } \| _ { 1 } = m - n { \mathrm { ~ i f ~ } } m > n$ so the sequence is not Cauchy. 

(b) $\begin{array} { r } { \| f _ { n } - f _ { m } \| _ { 1 } = \int _ { n } ^ { m } \frac { 1 } { x } \mathrm { d } x = \log m - \log n } \end{array}$ (for simplicity assume that $n < m )$ , let $\varepsilon = 1$ R, take any N, let $n = N$ , take m such that log $m { - } \log N > 1$ $( \log m \to \infty$ as $m  \infty ) -$ the sequence is not Cauchy. 

(c) $\begin{array} { r } { \| f _ { n } - f _ { m } \| _ { 1 } = \int _ { n } ^ { m } \frac { 1 } { x ^ { 2 } } \mathrm { d } x = - \frac { 1 } { x } | _ { n } ^ { m } = \frac { 1 } { n } - \frac { 1 } { m } \left( n < m \right. } \end{array}$ as before), and for any $\varepsilon > 0$ Rtake N such that $\begin{array} { r } { \frac { 1 } { N } < \frac { \varepsilon } { 2 } } \end{array}$ and for $n , m \geq N$ , clearly $\begin{array} { r } { \frac { 1 } { n } - \frac { 1 } { m } < \varepsilon } \end{array}$ – the sequence is Cauchy. 

5.3 $\begin{array} { r } { \| g _ { n } - g _ { m } \| _ { 2 } ^ { 2 } = \int _ { n } ^ { m } \frac { 1 } { x ^ { 4 } } \mathrm { d } x = - \frac { 1 } { 3 x ^ { 3 } } | _ { n } ^ { m } = \frac { 1 } { 3 } \big ( \frac { 1 } { n ^ { 3 } } - \frac { 1 } { m ^ { 3 } } \big ) } \end{array}$ – the sequence is Cauchy. 

5.4 (a) $\| f _ { n } - f _ { m } \| _ { 2 } ^ { 2 } = m - n { \mathrm { ~ i f ~ } } n > m$ so the sequence is not Cauchy. 

(b) $\begin{array} { r } { \| f _ { n } - f _ { m } \| _ { 2 } ^ { 2 } = \int _ { n } ^ { m } { \frac { 1 } { x ^ { 2 } } } \mathrm { d } x = { \frac { 1 } { n } } - { \frac { 1 } { m } } \to 0 } \end{array}$ – the sequence is Cauchy. 

(c) $\begin{array} { r } { \| f _ { n } - f _ { m } \| _ { 2 } ^ { 2 } = \int _ { n } ^ { m } \frac { 1 } { x ^ { 4 } } \mathrm { d } x = ( \frac { 1 } { 3 n ^ { 3 } } - \frac { 1 } { 3 m ^ { 3 } } ) } \end{array}$ – the sequence is Cauchy. 

5.5 $\| f + g \| ^ { 2 } = 4 , \| f - g \| ^ { 2 } = 1 , \| f \| ^ { 2 } = 1 , \| g \| ^ { 2 } = 1$ , and the parallelogram law is violated. 

5.6 $\begin{array} { r } { \| f + g \| _ { 1 } ^ { 2 } = 0 , \| f - g \| _ { 1 } ^ { 2 } = \frac { 1 } { 2 } , \| f \| _ { 1 } ^ { 2 } = \frac { 1 } { 4 } , \| g \| _ { 1 } ^ { 2 } = \frac { 1 } { 4 } } \end{array}$ , which contradicts the parallelogram law. 

5.7 Since sin nx cos mx $= { \textstyle { \frac { 1 } { 2 } } } [ \sin ( n + m ) x + \sin ( n - m ) x ]$ and sin nx sin $m x =$ $\begin{array} { r } { \frac { 1 } { 2 } [ \cos ( n - m ) x + \cos ( n + m ) x ] } \end{array}$ , it is easy to compute the indefinite integrals. They are periodic functions so the integrals over $[ - \pi , \pi ]$ are zero (for the latter we need $n \neq m )$ 

5.8 No: take any n, m (suppose $n < m )$ and compute 

$$
\| g _ {n} - g _ {m} \| _ {4} ^ {4} = \int_ {\frac {1}{m}} ^ {\frac {1}{n}} \left(\frac {1}{\sqrt {x}}\right) ^ {4} \mathrm{d} x = - x ^ {- 1} \bigg | _ {1 / m} ^ {1 / n} = (m - n) \geq 1
$$

so the sequence is not Cauchy. 

5.9 Let $\varOmega = [ 0 , 1 ]$ with Lebesgue measure, $\begin{array} { r } { X ( \omega ) = \frac { 1 } { \sqrt { \omega } } , E ( X ) = \int _ { 0 } ^ { 1 } X \mathrm { d } m = } \end{array}$ $\begin{array} { r } { \int _ { 0 } ^ { 1 } \frac { 1 } { \sqrt { x } } \mathrm { d } x = 2 , E ( X ^ { 2 } ) = \int _ { 0 } ^ { 1 } \frac { 1 } { x } \mathrm { d } x = \infty } \end{array}$ . If we take $\begin{array} { r } { X ( \omega ) = \frac { 1 } { \sqrt { \omega } } - 2 } \end{array}$ then R<sub>E(X)</sub> <sub>=</sub> <sub>0</sub> <sub>and</sub> $E ( X ^ { 2 } ) = \infty$ 

$$
\operatorname{Var} (a X) = E ((a X) ^ {2}) - (E (a X)) ^ {2} = a ^ {2} (E (X ^ {2}) - (E (X)) ^ {2}) = a ^ {2} \operatorname{Var} (X).
$$

5.11 Let $\begin{array} { r } { f _ { X } ( x ) = \frac { 1 } { b - a } { \bf 1 } _ { [ a , b ] } , E ( X ) = \frac { a + b } { 2 } , \mathrm { V a r } X = E ( X ^ { 2 } ) - \frac { ( a + b ) ^ { 2 } } { 4 } , E ( X ^ { 2 } ) = \frac { b + b } { 2 } . } \end{array}$ $\begin{array} { r } { \frac { 1 } { b - a } \int _ { a } ^ { b } x ^ { 2 } \mathrm { d } x = \frac { 1 } { b - a } \frac { 1 } { 3 } ( b ^ { 3 } - a ^ { 3 } ) } \end{array}$ and simple algebra gives the result. 

5.12 (a) E(X) = a, E((X a)<sup>2</sup>) = 0 since X = a a.s. 

(b) By Exercise 4.15 $f _ { X } ( x ) = 2 \mathbf { 1 } _ { [ 0 , \frac { 1 } { 2 } ] } ( x )$ and by Exercise 4. $\begin{array} { r } { { 1 } 7 , { E } ( X ) = \frac { 1 } { 4 } } \end{array}$ ; $\begin{array} { r } { \operatorname { s o } \operatorname { V a r } ( X ) = \int _ { 0 } ^ { \frac { 1 } { 2 } } 2 ( x - \frac { 1 } { 4 } ) ^ { 2 } \mathrm { d } x = 2 \int _ { - \frac { 1 } { 4 } } ^ { \frac { 1 } { 4 } } x ^ { 2 } \mathrm { d } x = \frac { 1 } { 4 8 } . } \end{array}$ 

(c) By Exercise 4.15, $f _ { X } = 4 x \mathbf { 1 } _ { [ 0 , \frac { 1 } { 2 } ] } ( x )$ , and by Exercise 4.17, $\textstyle E ( X ) = { \frac { 1 } { 6 } }$ hence $\begin{array} { r } { \operatorname { V a r } ( X ) = 4 \int _ { 0 } ^ { \frac { 1 } { 2 } } x ( x - \frac { 1 } { 6 } ) ^ { 2 } \mathrm { d } x = \frac { 1 } { 4 8 } , } \end{array}$ 

5.13 C $\mathrm { o v } ( Y , 2 Y + 1 ) = E ( ( Y ) ( 2 Y + 1 ) ) - E ( Y ) E ( 2 Y + 1 ) = 2 E ( Y ^ { 2 } ) - 2 ( E ( Y ) ) ^ { 2 } = 1$ $2 \mathrm { V a r } ( Y ) , \mathrm { V a r } ( 2 Y + 1 ) = \mathrm { V a r } ( 2 Y ) = 4 \mathrm { V a r } ( Y )$ , hence $\rho = 1$ 

5.14 X, Y are uncorrelated by Exercise 5.7. Take $a > 0$ so small that the sets $A = \{ \omega : \sin 2 \pi \omega > 1 - a \} , B = \{ \omega : \cos 2 \pi \omega > 1 - a \}$ are disjoint. Then $P ( A \cap B ) = 0 { \mathrm { ~ b u t ~ } } P ( A ) P ( B ) \neq 0 .$ 

## Chapter 6

6.1 The function 

$$
g (x, y) = \left\{ \begin{array}{l l} \frac {1}{x ^ {2}} & \text { if } 0 <   y <   x <   1 \\ - \frac {1}{y ^ {2}} & \text { if } 0 <   x <   y <   1 \\ 0 & \text { otherwise } \end{array} \right.
$$

is not integrable since the integral of $g ^ { + }$ is infinite (the same is true for the integral of $g ^ { - } )$ . However, 

$$
\int_ {0} ^ {1} \int_ {0} ^ {1} g (x, y) \mathrm{d} x \mathrm{d} y = - 1, \quad \int_ {0} ^ {1} \int_ {0} ^ {1} g (x, y) \mathrm{d} y \mathrm{d} x = 1
$$

which shows that the iterated integrals may not be equal if Fubini’s theorem condition is violated. 

6.2  <sub>[0,3] [ 1,2]</sub> x<sup>2</sup>y dm<sub>2</sub> = <sup>2</sup><sub>1</sub> <sup>3</sup><sub>0</sub> x<sup>2</sup>y dx dy = <sup>2</sup><sub>1</sub> 9y dy = <sup>27</sup><sub>2</sub> . 

6.3 By symmetry it is suficient to consider $x \ge 0 , y \ge 0$ , and hence the area is $\textstyle 4 { \frac { b } { a } } \int _ { 0 } ^ { a } { \sqrt { a ^ { 2 } - x ^ { 2 } } } \mathrm { d } x = a b \pi .$ 

6.4 Fix $\begin{array} { r } { x \in [ 0 , 2 ] , ~ \int _ { 0 } ^ { 2 } \mathbf { 1 } _ { A } ( x , y ) \mathrm { d } y = m ( A _ { x } ) } \end{array}$ , hence $f _ { X } ( x ) = x$ for $x \in [ 0 , 1 ]$ $f _ { X } ( x ) = 2 - x$ Rfor $x \in ( 1 , 2 ]$ and zero otherwise (triangle distribution). By symmetry, the same holds for $f _ { Y }$ 

6.5 $\begin{array} { r } { P ( X + Y > 4 ) = P ( Y > - X + 4 ) = \int \int _ { A } f _ { X , Y } ( x , y ) } \end{array}$ dx dy where $A =$ $\{ ( x , y ) : y > 4 - x \} \cap [ 0 , 2 ] \times [ 1 , 4 ] \ : .$ , so $\begin{array} { r } { P ( X + Y > 4 ) = \int _ { 0 } ^ { 2 } \int _ { 4 - x } ^ { 4 } \frac { 1 } { 5 0 } ( x ^ { 2 } + } \end{array}$ $\begin{array} { r } { y ^ { 2 } ) \mathrm { d } y \mathrm { d } x = \frac { 1 } { 5 0 } \int _ { 0 } ^ { 2 } ( - 4 x ^ { 2 } + \frac { 4 } { 3 } x ^ { 3 } + 1 6 x ) ) \mathrm { d } x = \frac { 8 } { 1 5 } . } \end{array}$ 

$$
\begin{array}{l} P (Y > X) = \int_ {1} ^ {2} \int_ {0} ^ {y} \frac {1}{5 0} (x ^ {2} + y ^ {2}) \mathrm{d} x \mathrm{d} y + \int_ {2} ^ {4} \int_ {0} ^ {2} \frac {1}{5 0} (x ^ {2} + y ^ {2}) \mathrm{d} x \mathrm{d} y \\ = \frac {1}{5 0} \int_ {1} ^ {2} \frac {4}{3} y ^ {3} \mathrm{d} y + \frac {1}{5 0} \int_ {2} ^ {4} (\frac {8}{3} + 2 y ^ {2}) \mathrm{d} y \\ = \frac {1 4 3}{1 5 0} \end{array}
$$

Similarly $\begin{array} { r } { P ( Y > X ) = \int \int _ { A } f _ { X , Y } ( x , y ) } \end{array}$ dx dy where $A = \{ ( x , y ) : y > x \} \cap$ $[ 0 , 2 ] \times [ 1 , 4 ]$ , so we get $\begin{array} { r } { \int _ { 1 } ^ { 2 } \int _ { 0 } ^ { y } \frac { 1 } { 5 0 } ( x ^ { 2 } + y ^ { 2 } ) \mathrm { d } x \mathrm { d } y + \int _ { 2 } ^ { 4 } \int _ { 0 } ^ { 2 } \frac { 1 } { 5 0 } ( x ^ { 2 } + y ^ { 2 } ) \mathrm { d } y \mathrm { d } x = } \end{array}$ $\begin{array} { r } { \frac { 1 } { 5 0 } \int _ { 1 } ^ { 2 } \frac { 4 } { 3 } y ^ { 3 } \mathrm { d } y + \frac { 1 } { 5 0 } \int _ { 2 } ^ { 4 } ( \frac { 8 } { 3 } + 2 y ^ { 2 } ) \mathrm { d } y = \frac { 1 4 3 } { 1 5 0 } } \end{array}$ 

6.6 

$$
f _ {X + Y} (z) = \int_ {R} f _ {X, Y} (x, z - x) \mathrm{d} x = \left\{ \begin{array}{l l} 0 & z <   0 \\ z & 0 \leq z \leq 1 \\ 2 - z & 1 \leq z \leq 2 \\ 0 & 2 <   z \end{array} \right.
$$

6.7 By Exercise 6.4, $f _ { X , Y } ( x , y ) \neq f _ { X } ( x ) f _ { Y } ( y )$ so $X , Y$ are not independent. 

$$
6. 8 f _ {Y + (- X)} (z) = \int_ {- \infty} ^ {+ \infty} f _ {Y} (y) f _ {- X} (z - y) d y = \int_ {- \infty} ^ {+ \infty} \frac {1}{2} 1 _ {[ 0, 2 ]} (y) 1 _ {[ - 1, 0 ]} (z - y) d y \text { so }
$$

$$
f _ {Y - X} (z) = \left\{ \begin{array}{l l} 0 & z <   - 1 \text {or} 2 <   z \\ \frac {1}{2} (z + 1) & - 1 \leq z \leq 0 \\ \frac {1}{2} & 0 \leq z \leq 1 \\ \frac {1}{2} (2 - z) & 1 \leq z \leq 2 \end{array} \right.
$$

$$
f _ {X + Y} (z) = \int_ {- \infty} ^ {+ \infty} f _ {X} (x) f _ {Y} (z - x) \mathrm{d} x = \int_ {- \infty} ^ {+ \infty} 1 _ {[ 0, 1 ]} (x) \frac {1}{2} 1 _ {[ 0, 2 ]} (z - x) \mathrm{d} x \text {hence}
$$

$$
f _ {X + Y} (z) = \left\{ \begin{array}{l l} 0 & z <   0 \text {or} 3 <   z \\ \frac {1}{2} z & 0 \leq z \leq 1 \\ \frac {1}{2} & 1 \leq z \leq 2 \\ \frac {1}{2} (3 - z) & 2 \leq z \leq 3 \end{array} \right.
$$

$$
\begin{array}{l} P (Y > X) = P (Y - X > 0) = \int_ {0} ^ {\infty} f _ {Y - X} (z)   \mathrm{d} z = \frac {1}{2} + \int_ {1} ^ {2} \frac {1}{2} (2 - z)   \mathrm{d} z = \\ \frac {1}{2} + \frac {1}{4} = \frac {3}{4}; \end{array}
$$

$$
P (X + Y > 1) = \int_ {1} ^ {\infty} f _ {X + Y} (z) \mathrm{d} z = \frac {1}{2} + \int_ {2} ^ {3} \frac {1}{2} (3 - z) \mathrm{d} z = \frac {1}{2} + \frac {1}{3} = \frac {3}{4}.
$$

$$
\begin{array}{l} 6. 9 f _ {X} (x) = \int_ {0} ^ {- \frac {1}{2} x + 1} 1 _ {A}   \mathrm{d} y = 1 - \frac {1}{2} x, h (y, x) = \frac {\mathbf {1} _ {A} (x , y)}{1 - \frac {1}{2} x} \text { and } E (Y | X = 1) = \\ 2 \int_ {0} ^ {\frac {1}{2}} x   \mathrm{d} x = \frac {1}{4}. \end{array}
$$

$$
6. 1 0 f _ {Y} (y) = \int_ {0} ^ {1} (x + y) \mathrm{d} x = \frac {1}{2} + y, h (x | y) = \frac {x + y}{\frac {1}{2} + y} \mathbf {1} _ {A} (x, y), E (X | Y = y) =
$$

$$
\int_ {0} ^ {1} x \frac {x + y}{\frac {1}{2} + y} \mathrm{d} x = \frac {\frac {1}{3} + \frac {1}{2} y}{\frac {1}{2} + y}.
$$

## Chapter 7

7.1 If $\mu ( A ) = 0$ then $\lambda _ { 1 } ( A ) = 0$ and $\lambda _ { 2 } ( A ) = 0$ , hence $( \lambda _ { 1 } + \lambda _ { 2 } ) ( A ) = 0$ 

7.2 Let be a finite partition of Ω which refines both $\mathcal { P } _ { 1 }$ and $\mathcal { P } _ { 2 }$ . Thus each set $A \in \mathcal { Q }$ can be written as a disjoint union $A = \textstyle \bigcup _ { i = 1 } ^ { n } E _ { i } = \bigcup _ { i = 1 } ^ { m } F _ { j }$ where $E _ { i } \in \mathcal { P } _ { 1 } , F _ { j } \in \mathcal { P } _ { 2 }$ S. Each element of A belongs to exactly one $E _ { i }$ and exactly one $F _ { j }$ so $\begin{array} { r } { A = \bigcup _ { i , j } ( E _ { i } \cap F _ { j } ) } \end{array}$ is a disjoint union as well. Hence refines the partition $\mathcal { R } = \left\{ E \cap F : E \in \mathcal { P } _ { 1 } , F \in \mathcal { P } _ { 2 } \right\}$ (which is a partition as the above argument applied to $A = \varOmega$ shows). It is suficient to see that $\mathcal { R }$ refines $\mathcal { P } _ { i } .$ $i = 1 , 2$ . But $E \in { \mathcal { P } } _ { 1 }$ can be written as $\begin{array} { r } { E = E \cap \bigcup _ { F \in \mathcal { P } _ { 2 } } F = \bigcup _ { F \in \mathcal { P } _ { 2 } } ( E \cap F ) } \end{array}$ so $E$ S Sis a disjoint union of elements of . Similar argument shows that refines $\mathcal { P } _ { 2 }$ 

7.3 We have to assume first that $m ( A ) ~ \neq ~ 0$ . Then $B \subset A$ clearly implies that $\mu$ dominates ν. (In fact $m ( B \setminus A ) = 0$ is slightly more general.) Then consider the partition $\{ B , A \backslash B , \Omega \backslash A \}$ to see that $h = \mathbf { 1 } _ { B }$ . To double check, $\begin{array} { r } { \nu ( F ) = m ( F \cap B ) = \int _ { F \cap B } \mathbf { 1 } _ { B } \mathrm { d } m = \int _ { F \cap B } \mathbf { 1 } _ { B } \mathrm { d } \mu . } \end{array}$ 

7.4 Clearly $\mu ( \{ \omega \} ) \geq \nu ( \{ \omega \} )$ is equivalent to $\mu$ dominating ν. For each $\omega$ we have $\begin{array} { r } { \frac { d \nu } { d \mu } ( \omega ) = \frac { \nu ( \{ \omega \} ) } { \mu ( \{ \omega \} ) } } \end{array}$ 

7.5 Since $\nu ( E ) = \textstyle \int _ { E }$ g dm and we wish to have $\begin{array} { r } { \nu ( E ) = \int _ { E } \frac { d \nu } { d \mu } \mathrm { d } \mu = \int _ { E } \frac { d \nu } { d \mu } f \mathrm { d } m } \end{array}$ it is natural to aim at taking $\begin{array} { r } { \frac { d \nu } { d \mu } ( x ) = \frac { g ( x ) } { f ( x ) } } \end{array}$ . Then a suficient condition for this to work is that if $A = \{ x : f ( x ) \stackrel { } { = } 0 \}$ then $\nu ( A ) = 0 , \mathrm { i . e . } \ g ( x ) = 0$ a.e. on A. Then we put $\begin{array} { r } { \frac { d \nu } { d \mu } ( x ) \ = \ \frac { g ( x ) } { f ( x ) } } \end{array}$ on A and 0 on A<sup>c</sup> and we have $\begin{array} { r } { \nu ( E ) = \int _ { E \cap A ^ { c } } g \mathrm { d } m = \int _ { E \cap A ^ { c } } \frac { d \nu } { d \mu } f \mathrm { d } m = \int _ { E } \frac { d \nu } { d \mu } \mathrm { d } \mu , } \end{array}$ , as required. 

7.6 Clearly $\nu \ll \mu$ is equivalent to $A = \{ \omega : \mu ( \{ \omega \} ) = 0 \} \subset \{ \omega : \nu ( \{ \omega \} ) = 0 \}$ and then $\begin{array} { r } { \frac { d \nu } { d \mu } \overset { \cdot } { ( \omega ) } = \frac { \bar { \nu } ( \{ \omega \} ) } { \mu ( \{ \omega \} ) } } \end{array}$ on A and zero outside. 

7.7 Since $\nu \ll \mu$ we may write $\textstyle h = { \frac { d \nu } { d \mu } }$ , so that $\begin{array} { r } { \nu ( F ) = \int _ { F } h \mathrm { d } \mu . \mathrm { A s } \ \mu ( F ) = 0 } \end{array}$ if and only if $\nu ( F ) = 0$ , the set $\{ h = 0 \}$ Ris both µ-null and $\nu { \mathrm { - } } \mathrm { n u l l }$ . Thus $\begin{array} { r } { h ^ { - 1 } = ( \frac { d \nu } { d \mu } ) ^ { - 1 } } \end{array}$ is well-defined a.s., and we can use (ii) in Proposition 7.7 with $\lambda = \mu$ to conclude that $1 = h ^ { - 1 } h$ implies $\textstyle { \frac { d \mu } { d \nu } } = h ^ { - 1 }$ , as required. 

7.8 $\delta _ { 0 } ( ( 0 , 2 5 ] ) = 0$ , but $\begin{array} { r } { \frac { 1 } { 2 5 } m | _ { [ 0 , 2 5 ] } ( ( 0 , 2 5 ] ) = 1 ; \frac { 1 } { 2 5 } m | _ { [ 0 , 2 5 ] } ( \{ 0 \} ) = 0 } \end{array}$ but $\delta _ { 0 } ( \{ 0 \} ) =$ 1 so neither $P _ { 1 } \ll P _ { 2 }$ nor $P _ { 2 } \ll P _ { 1 }$ . Clearly $P _ { 1 } \ll P _ { 3 }$ with $\begin{array} { r } { \frac { d P _ { 1 } } { d P _ { 3 } } ( x ) = } \end{array}$ ${ \bf 2 } \times { \bf 1 } _ { \{ 0 \} } ( x )$ and $P _ { 2 } \ll P _ { 3 }$ with $\begin{array} { r } { \frac { d P _ { 2 } } { d P _ { 3 } } ( x ) = 2 \times \mathbf { 1 } _ { ( 0 , 2 5 ] } ( x ) } \end{array}$ 

7.9 $\lambda _ { a } = m | _ { [ 2 , 3 ] } , \lambda _ { s } = \delta _ { 0 } + m | _ { ( 1 , 2 ) }$ , and $h = \mathbf { 1 } _ { [ 2 , 3 ] }$ 

7.10 Suppose F is non-constant at $a _ { i }$ with positive jumps $c _ { i } , i = 1 , 2 , . . .$ . Take $M \neq a _ { i }$ , with $- M \neq a _ { i }$ and let $I = \{ i : a _ { i } \in [ - M , M ] \}$ . Then 

$$
m _ {F} ([ - M, M ]) = F (M) - F (- M) = \sum_ {i \in I} c _ {i} = \sum_ {i \in I} m _ {F} (\{a _ {i} \}),
$$

which is finite since F is bounded on a bounded interval. So any $A \subset$ $[ - M , M ] \setminus \bigcup _ { i \in I } \{ a _ { i } \}$ is $m _ { F } { \mathrm { - n u l l } }$ hence measurable. But $\{ a _ { i } \}$ are $m _ { F ^ { - } }$ Smeasurable hence each subset of $[ - M , M ]$ is m -measurable. Finally, any subset E of R is a union of the sets of the form $E \cap [ - M , M ]$ , so $E$ is m<sub>F</sub>-measurable as well. 

7.11 $m _ { F }$ has density $f ( x ) = 2$ for $x \in [ 0 , 1 ]$ and zero otherwise. 

7.12 $\begin{array} { r } { \mathrm { ( a ) } \ | x | = 1 + \int _ { - 1 } ^ { x } f ( y ) \mathrm { d } y } \end{array}$ , where $f ( y ) = - 1$ for $y \in [ - 1 , 0 ]$ , and $f ( y ) = 1$ for $y \in ( 0 , 1 ]$ 

(b) Let $1 > \varepsilon > 0$ , take $\begin{array} { r } { \delta = \varepsilon ^ { 2 } , \sum _ { k = 1 } ^ { n } ( y _ { k } - x _ { k } ) < \delta _ { 1 } } \end{array}$ with $y _ { k } \le x _ { k + 1 } ;$ then 

$$
(\sum_ {k = 1} ^ {n} | \sqrt {x _ {k}} - \sqrt {y _ {k}} |) ^ {2} \leq (\sqrt {y _ {n}} - \sqrt {x _ {1}}) ^ {2} = y _ {n} - 2 \sqrt {y _ {n} x _ {1}} + x _ {1} <   y _ {n} - x _ {1}
$$

$$
\leq \sum_ {k = 1} ^ {n} (y _ {k} - x _ {k}) <   \varepsilon^ {2}.
$$

(c) Lebesgue function f is a.e. diferentiable with $f ^ { \prime } = 0$ a.e. If it were absolutely continuous, it could be written as $\begin{array} { r } { f ( x ) = \int _ { 0 } ^ { x } f ^ { \prime } ( y ) \mathrm { d } y = 0 } \end{array}$ , a contradiction. 

7.13 (a) If F is monotone increasing on $[ a , b ] , \textstyle \sum _ { i = 1 } ^ { k } | F ( x _ { i } ) - F ( x _ { i - 1 } ) | = F ( b ) -$ $F ( a )$ for any partition $a = x _ { 0 } < x _ { 1 } < \cdots < x _ { k } = b$ . Hence ${ \cal T } _ { \cal F } [ a , b ] =$ $F ( b ) - F ( a )$ 

(b) If $F \in B V [ a , b ]$ we can write $F = F _ { 1 } - F _ { 2 }$ where both $F _ { 1 } , F _ { 2 }$ are monotone increasing, hence have only countably many points of discontinuity. So F is continuous a.e. and thus Lebesgue-measurable. 

(c) $\begin{array} { r } { f ( x ) = x ^ { 2 } \cos \frac { \pi } { x ^ { 2 } } } \end{array}$ for $x \neq 0$ and $f ( 0 ) = 0$ is diferentiable but does not belong to $B V [ 0 , 1 ]$ 

(d) If F is Lipschitz, $\begin{array} { r } { \sum _ { i = 1 } ^ { k } | F ( x _ { i } ) - F ( x _ { i - 1 } ) | \leq M \sum _ { i = 1 } ^ { k } | x _ { i } - x _ { i - 1 } | = } \end{array}$ $M ( b - a )$ Pfor any partition so $T _ { F } [ a , b ] \leq M ( b - a )$ Pis finite. 

7.14 Recall that $\nu ^ { + } ( E ) = \nu ( E \cap B )$ , where B is the positive set in the Hahn decomposition. As in the hint, if $G \subseteq F , \nu ( G ) \leq \nu ^ { + } ( G \cap B ) \leq \nu ( G \cap B ) +$ $\nu ( ( F \cap B ) \setminus ( G \cap B ) ) = \nu ( F \cap B )$ . Since the set $( F \cap B ) \setminus ( G \cap B ) \subseteq B$ 2 its ν-measure is non-negative. But $F \cap B \subseteq F$ so $\operatorname* { s u p } \{ \nu ( G ) : G \subseteq F \}$ is attained and equals $\nu ( F \cap B ) = \nu ^ { + } ( F )$ . A similar argument shows $\nu ^ { - } ( F ) =$ sup $\{ - \nu ( G ) \} = - \operatorname* { i n f } _ { G \subset F } \{ \nu ( G ) \}$ 

7.15 For all $\begin{array} { r } { F \in \mathscr { F } , \nu ^ { + } ( F ) = \int _ { B \cap F } f \mathrm { d } \mu = \operatorname* { s u p } _ { G \subset F } \int _ { G } f \mathrm { d } \mu } \end{array}$ . If $f > 0$ on a set $C \subset A \cap F$ with $\mu ( C ) > 0$ R, then $\textstyle \int _ { C } f \mathrm { d } \mu > 0 .$ R, so that $\begin{array} { r } { \int _ { C } f \mathrm { d } \mu + \int _ { B \cap F } f \mathrm { d } \mu > } \end{array}$ $\textstyle \operatorname* { s u p } _ { G \subset F } \int _ { G } f \mathrm { d } \mu$ . This is a contradiction since $C \cup ( B \cap F ) \subset F .$ . So $f \leq 0$ a.s. (µ) on $A \cap F$ . We can take the set $\{ f = 0 \}$ into B, since it does not afect the integrals. Hence $\{ f < 0 \} \subset A$ and $\{ f \geq 0 \} \subset B$ . But the two smaller sets partition $\varOmega .$ , so we have equality in both cases. Hence $f ^ { + } = f \mathbf { 1 } _ { B }$ and $f ^ { - } = - f \mathbf { 1 } _ { A }$ , therefore for all $F \in { \mathcal { F } }$ 

$$
\begin{array}{l} \nu^ {+} (F) = \nu (B \cap F) = \int_ {B \cap F} f   \mathrm{d} \mu = \int_ {F} f ^ {+}   \mathrm{d} \mu , \\ \nu^ {-} (F) = - \nu (A \cap F) = - \int_ {A \cap F} f   \mathrm{d} \mu = \int_ {F} f ^ {-}   \mathrm{d} \mu . \end{array}
$$

7.16 $f \in L ^ { 1 } ( \nu )$ if both $\int f ^ { + } \mathrm { d } \nu$ and $\int f ^ { - } \mathrm { d } \nu$ are finite. Then $\int _ { E } f ^ { + } g \mathrm { d } \mu$ and $\int _ { E } f ^ { - } g \mathrm { d } \mu$ R R Rare well-defined and finite and their diference is $\textstyle \int _ { E } f g \mathrm { d } \mu$ . So $f g \in L ^ { 1 } ( \mu )$ , as $\begin{array} { r } { \int _ { E } \bigl ( f ^ { + } - f ^ { - } \bigr ) \vert g \vert \mathrm { d } \mu < \infty } \end{array}$ . Conversely, if $f g \in L ^ { 1 } ( \mu )$ then both $\textstyle \int _ { E } f ^ { + } | g | \mathrm { d } \mu$ R and $\textstyle \int _ { E } f ^ { - } | g | \mathrm { d } \mu$ are finite hence so is their diference $\textstyle \int _ { E } f \mathrm { d } \nu$ 

7.17 (a) E $\begin{array} { r } { \mathfrak { c } ( X | \mathcal { G } ) ( \omega ) = \frac { 1 } { 4 } \mathrm { ~ i f ~ } \omega \in [ 0 , \frac { 1 } { 2 } ] , \mathbb { E } ( X | \mathcal { G } ) ( \omega ) = \frac { 3 } { 4 } } \end{array}$ otherwise. 

(b) $\begin{array} { r } { \mathbb { E } ( X | \mathcal { G } ) ( \omega ) = \omega \mathrm { ~ i f ~ } \omega \in [ 0 , \frac 1 2 ] , \mathbb { E } ( X | \mathcal { G } ) ( \omega ) = \frac { 3 } { 4 } } \end{array}$ otherwise. 

7.18 E $( X _ { n } | { \mathcal F } _ { n - 1 } ) \ = \ \mathbb { E } ( Z _ { 1 } Z _ { 2 } \ldots Z _ { n } | { \mathcal F } _ { n - 1 } ) \ = \ Z _ { 1 } Z _ { 2 } \ldots Z _ { n - 1 } \mathbb { E } ( Z _ { n } | { \mathcal F } _ { n - 1 } )$ , and since $Z _ { n }$ is independent of $\mathcal { F } _ { n - 1 }$ ， $\mathbb { E } ( Z _ { n } | \mathcal { F } _ { n - 1 } ) = \mathbb { E } ( Z _ { n } ) = 1$ , hence the result. 

7.19 E $( X _ { n } ) = n \mu \neq \mu = \operatorname { \mathbb { E } } ( X _ { 1 } )$ so $X _ { n }$ is not a martingale. Clearly $Y _ { n } = X _ { n } - n \mu$ is a martingale. 

7.20 $\begin{array} { r } { \mathbb { E } ( ( Z _ { 1 } + Z _ { 2 } + \cdot \cdot \cdot + Z _ { n } ) ^ { 2 } | \mathcal { F } _ { n - 1 } ) \le \mathbb { E } ( Z _ { 1 } + Z _ { 2 } + \cdot \cdot \cdot + Z _ { n } | \mathcal { F } _ { n - 1 } ) ^ { 2 } = ( Z _ { 1 } + \frac { 1 } { n - 1 } ) ^ { n - 1 } . } \end{array}$ $Z _ { 2 } + \cdots + Z _ { n - 1 } ) ^ { 2 }$ using Jensen inequality. The compensator is deterministic: $A _ { n } = n$ 

7.21 For $s < t ,$ , since the increments are independent and $w ( t ) - w ( s )$ has the same distribution as $w ( t - s )$ , 

$$
\begin{array}{r l} & {\mathbb {E} (\exp (- \sigma w (t) - \frac {1}{2} \alpha^ {2} t)) = e ^ {- \sigma w (s) - \frac {1}{2} \sigma^ {2} t} \mathbb {E} (\exp (- [ \sigma (w (t) - w (s) ]) | \mathcal {F} _ {s})} \\ & {\qquad = e ^ {- \sigma w (s) - \frac {1}{2} \sigma^ {2} t} \mathbb {E} (\exp (- [ \sigma (w (t) - w (s) ])} \\ & {\qquad = e ^ {- \sigma w (s) - \frac {1}{2} \sigma^ {2} t} \mathbb {E} (\exp (- \sigma w (t - s))).} \end{array}
$$

Now $\sigma w ( t - s ) \backsim N ( 0 , \sigma ^ { 2 } ( t - s ) )$ so the expectation equals E $( e ^ { - \sigma { \sqrt { t - s } } Z } ) =$ $e ^ { - { \frac { 1 } { 2 } } \sigma ^ { 2 } ( t - \dot { s } ) }$ (where $Z \sim N ( 0 , 1 ) )$ and so the result follows. 

## Chapter 8

8.1 (a) $f _ { n } = \mathbf { 1 } _ { [ n , n + \frac { 1 } { n } ] }$ converges to 0 in $L ^ { p }$ , pointwise, a.e. but not uniformly. (b) $f _ { n } = n \mathbf { 1 } _ { [ 0 , \frac { 1 } { n } ] } - n \mathbf { 1 } _ { [ - \frac { 1 } { n } , 0 ] }$ converges to 0 pointwise and a.e. It converges neither in $L ^ { p }$ nor uniformly. 

8.2 We have $\varOmega = [ 0 , 1 ]$ with Lebesgue measure. The sequences $X _ { n } = \mathbf { 1 } _ { ( 0 , \frac { 1 } { n } ) }$ $X _ { n } = n \mathbf { 1 } _ { ( 0 , \frac { 1 } { n } ] }$ converge to 0 in probability since $\begin{array} { r } { P ( | X _ { n } | > \varepsilon ) \le \frac { 1 } { n } } \end{array}$ and the same holds for the sequence $g _ { n }$ 

8.3 There are endless possibilities, the simplest being $X _ { n } ( \omega ) \equiv 1$ (but this sequence converges to 1) or, to make sure that it does not converge to anything, $X _ { n } ( \omega ) \equiv n$ 

8.4 Let $X _ { n } ~ = ~ 1$ indicate the heads and $X _ { n } ~ = ~ 0$ the tail, then $\frac { S _ { 1 0 0 } } { 1 0 0 }$ is the average number of heads in 100 tosses. Clearly $\begin{array} { r } { E ( X _ { n } ) = \frac { 1 } { 2 } , E ( \frac { \mathbf { \tilde { { S } } } _ { 1 0 0 } ^ { < } } { 1 0 0 } ) = \frac { 1 } { 2 } } \end{array}$ 2 $\begin{array} { r } { \operatorname { V a r } ( X _ { n } ) = \frac { 1 } { 4 } , \operatorname { V a r } ( \frac { S _ { 1 0 0 } } { 1 0 0 } ) = \frac { 1 } { 1 0 0 ^ { 2 } } 1 0 0 \cdot \frac { 1 } { 4 } = \frac { 1 } { 4 0 0 } } \end{array}$ so 

$$
P (| \frac {S _ {1 0 0}}{1 0 0} - \frac {1}{2} | \geq 0. 1) \leq \frac {1}{0 . 1 ^ {2} 4 0 0}
$$

and 

$$
P \left(\left| \frac {S _ {1 0 0}}{1 0 0} - \frac {1}{2} \right| <   0. 1\right) \geq 1 - \frac {1}{0 . 1 ^ {2} 4 0 0} = \frac {3}{4}.
$$

8.5 Let $X _ { n }$ be the number shown on the die, $E ( X _ { n } ) = 3 . 5 , \operatorname { V a r } ( X _ { n } ) \approx 2 . 9$ 

$$
P (| \frac {S _ {1 0 0 0}}{1 0 0 0} - 3. 5 | <   0. 0 1) \geq 0. 2 9.
$$

8.6 The union $\textstyle \bigcup _ { m = n } ^ { \infty } A _ { m }$ is equal to $[ 0 , 1 ]$ for all m and so is lim s $\textstyle \operatorname { l p } _ { n \to \infty } A _ { n }$ 

8.7 Let d = 1. There are $\textstyle { \binom { 2 n } { n } }$ paths that return to 0, so $\begin{array} { r } { P ( S _ { 2 n } = 0 ) = { \binom { 2 n } { n } } \frac { 1 } { 2 ^ { 2 n } } } \end{array}$ Now 

$$
\frac {(2 n) !}{(n !) ^ {2}} \sim \frac {(\frac {2 n}{e}) ^ {2 n} \sqrt {2 \pi 2 n}}{(\frac {n}{e}) ^ {2 n} 2 \pi n} = \frac {2 n \sqrt {2}}{\sqrt {n \pi}}
$$

so $\begin{array} { r } { P ( S _ { 2 n } = 0 ) \sim \frac { c } { \sqrt { n } } } \end{array}$ with $c = { \sqrt { \textstyle { \frac { 2 } { \pi } } } } .$ . Hence $\textstyle \sum _ { n = 1 } ^ { \infty } P ( A _ { n } )$ diverges and Borel-Cantelli applies $\left( \operatorname { a s } \ \left( A _ { n } \right) \right.$ are independent) so that $P ( S _ { 2 n } = 0 \ \mathrm { i . o . } ) = 1$ Same for $d = 2$ since $\begin{array} { r } { P ( A _ { n } ) \sim \frac { 1 } { n } } \end{array}$ . But for $\begin{array} { r } { d > 2 , P ( A _ { n } ) \sim \frac { 1 } { n ^ { d / 2 } } } \end{array}$ , the series converges and by the first Borel-Cantelli lemma $P ( S _ { 2 n } = 0 \mathrm { i } . 0 . ) = 0$ 

8.8 Write $\begin{array} { r } { S = S _ { 1 0 0 0 } ; P ( | S - 5 0 0 | < 1 0 ) = P ( \frac { | S - 5 0 0 | } { \sqrt { 2 5 0 } } < 0 . 6 3 ) \approx 0 . 4 7 . } \end{array}$ 

8.9 The condition on n is $\begin{array} { r } { P ( | \frac { S _ { n } } { n } - 0 . 5 | < 0 . 0 0 5 ) = P ( \frac { | S _ { n } - 0 . 5 n | } { \sqrt { n / 4 } } < 0 . 0 1 \sqrt { n } ) \ge } \end{array}$ 0.99, hence $n \geq 6 6 6 1 5$ 

8.10 Write $x _ { n } = e ^ { \sigma { \sqrt { T / n } } }$ . Then 

$$
\frac {1}{2} (\ln U _ {n} + \ln D _ {n}) = \frac {1}{2} \ln (U _ {n} D _ {n}) = \frac {1}{2} \ln \frac {(2 R _ {n} x _ {n}) ^ {2}}{(1 + x _ {n} ^ {2}) ^ {2}} = \ln e ^ {r \frac {T}{n} n} - \ln (\frac {1 + x _ {n} ^ {2}}{2 x _ {n}}).
$$

So it sufices to show that the last term on the right is $\textstyle { \frac { \sigma ^ { 2 } T } { 2 n } } + o \left( { \frac { 1 } { n } } \right)$ . But 

$$
\begin{array}{r l} & {\frac {1 + x _ {n} ^ {2}}{2 x _ {n}} = \frac {x _ {n} ^ {- 1} + x _ {n}}{2} = \frac {e ^ {\sigma \sqrt {T / n}} + e ^ {\sigma \sqrt {T / n}}}{2} = \cosh (\sigma \sqrt {T / n})} \\ & {\qquad = 1 + \frac {\sigma^ {2} T}{2 n} + o (\frac {1}{n})} \end{array}
$$

so that 

$$
\ln (\frac {1 + x _ {n} ^ {2}}{2 x _ {n}}) = \ln (1 + \frac {\sigma^ {2} T}{2 n} + o (\frac {1}{n})) = \frac {\sigma^ {2} T}{2 n} + o (\frac {1}{n}).
$$

## Existence of non-measurable and non-Borel sets

In Chapter 2 we defined the σ-field of Borel sets and the larger σ-field of Lebesgue-measurable sets, and all our subsequent analysis of the Lebesgue integral and its properties involved these two families of subsets of R. The set inclusions 

$$
\mathcal {B} \subset \mathcal {M} \subset \mathcal {P} (\mathbb {R})
$$

are trivial; however, it is not at all obvious at first sight that they are strict, i.e. that there are sets in R which are not Lebesgue-measurable, as well as that there are Lebesgue-measurable sets which are not Borel sets. In this appendix we construct examples of such sets. Using the fact that $A \subset \mathbb { R }$ is measurable (resp. Borel-measurable) if its indicator function $\mathbf { 1 } _ { A } \in \mathcal { M }$ (resp. ) it follows that we will automatically have examples of non-measurable (resp. measurable but not Borel) functions. 

The construction of a non-measurable set requires some set-theoretic preparation. This takes the form of an axiom which, while not needed for the consistent development of set theory, nevertheless enriches that theory considerably. Its truth or falsehood cannot be proved from the standard axioms on which modern set theory is based, but we shall accept its validity as an axiom, without delving further into foundational matters. 

## The Axiom of Choice

Suppose that $\mathcal { A } = \{ A _ { \alpha } : \alpha \in A \}$ is a non-empty collection, indexed by some set Λ, of non-empty disjoint subsets of a fixed set $\varOmega ,$ , Then there exists a set $E \subset { \mathcal { Q } }$ which contains precisely one element from each of the sets $A _ { \alpha }$ , i.e. there is a choice function $f : { \cal { \Lambda } } \longrightarrow { \cal { A } }$ 

## Remark

The Axiom may seem innocuous enough, yet it can be shown to be independent of the (Zermelo–Fraenkel) axioms of sets theory. If the collection $\mathcal { A }$ has only finitely many members there no problem in finding a choice function, of course. To see that the existence of such a function is problematic for infinite sets, consider the following illustration given by Bertrand Russell: imagine being faced with an infinite collection of pairs of shoes and another of pairs of socks. Constructing the set consisting of all left shoes is simple; that of defining the set of all left socks is not! 

To construct our example of a non-measurable set, first define the following equivalence relation on [0, 1]: x  y if $y - x$ is a rational number (which will be in [ 1, 1]). This relation is easily seen to be reflexive, symmetric and transitive. Hence it partitions [0, 1] into disjoint equivalence classes $\left( { \cal A } _ { \alpha } \right)$ , where for each α, any two elements $x , y$ of $A _ { \alpha }$ difer by a rational, while elements of diferent classes will always difer by an irrational. Thus each $A _ { \alpha }$ is countable, since Q is, but there are uncountably many diferent classes, as [0, 1] is uncountable. 

Now use the Axiom of Choice to construct a new set $E \subset [ 0 , 1 ]$ which contains exactly one member $a _ { \alpha }$ from each of the $A _ { \alpha }$ . Now enumerate the rationals in [ 1, 1]: there are only countably many, so we can order them as a sequence $\left( q _ { n } \right)$ . Define a sequence of translates of E by $E _ { n } = E + q _ { n }$ . If E is Lebesgue-measurable, then so is each $E _ { n }$ and their measures are the same, by Proposition 2.10. 

But the $\left( E _ { n } \right)$ are disjoint: to see this, suppose that $z \in E _ { m } \cap E _ { n }$ for some m $\neq m$ . Then we can write $a _ { \alpha } + q _ { m } = z = a _ { \beta } + q _ { n }$ for some $a _ { \alpha } , a _ { \beta } \in E$ , and their diference $a _ { \alpha } - a _ { \beta } = q _ { n } - q _ { m }$ is rational. Since E contains only one element from each class, $\alpha = \beta$ and therefore $m = n$ . Thus $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ is a disjoint union containing [0, 1]. 

Thus we have $[ 0 , 1 ] \subset \bigcup _ { n = 1 } ^ { \infty } E _ { n } \subset [ - 1 , 2 ]$ and $m ( E _ { n } ) = m ( E )$ for all n. By Scountable additivity and monotonicity of m this implies: 

$$
1 = m ([ 0, 1 ]) \leq \sum_ {n = 1} ^ {\infty} m (E _ {n}) = m (E) + m (E) + \dots \leq 3.
$$

This is clearly impossible, since the sum must be either 0 or . Hence we must conclude that E is not measurable. 

For an example of a measurable set that is not Borel, let $C$ denote the Cantor set, and define the Cantor function $f : [ 0 , 1 ] \to C$ as follows: for $x \in [ 0 , 1 ]$ write $x = 0 . a _ { 1 } a _ { 2 } . . .$ . in binary form, i.e. $\begin{array} { r } { x = \sum _ { n = 1 } ^ { \infty } \frac { a _ { n } } { 2 ^ { n } } } \end{array}$ , where each $a _ { n } = 0$ or 1 (taking Pnon-terminating expansions where the choice exists). The function $x \mapsto a _ { n }$ is determined by a system of finitely many binary intervals (i.e. the value of $a _ { n }$ is fixed by x satisfying finitely many linear inequalities) and so is measurable – hence so is the function $f$ given by $\begin{array} { r } { f ( x ) = \sum _ { n = 1 } ^ { \infty } { \frac { 2 a _ { n } } { 3 ^ { n } } } } \end{array}$ . Since all the terms of $\begin{array} { r } { y = \sum _ { n = 1 } ^ { \infty } \frac { 2 a _ { n } } { 3 ^ { n } } } \end{array}$ Phave numerators 0 or 2, it follows that the range $R _ { f }$ of $f$ is a Psubset of C. Moreover, the value of $y$ determines the sequence $\left( a _ { n } \right)$ and hence $x ,$ uniquely, so that $f$ is invertible. 

Now consider the image in C of the non-measurable set E constructed above, i.e. let $B = f ( E )$ . Then B is a subset of the null set $C _ { i }$ , hence by the completeness of m it is also measurable and null. On the other hand, $E =$ $f ^ { - 1 } ( B )$ is non-measurable. We show that this situation is incompatible with $B$ being a Borel set. 

Given a set $B \in B$ and a measurable function $^ { g , }$ then $g ^ { - 1 } ( B )$ must be measurable. For, by definition of measurable functions, $g ^ { - 1 } ( I )$ is measurable for every interval I, and we have 

$$
g ^ {- 1} \left(\bigcup_ {i = 1} ^ {\infty} A _ {i}\right) = \bigcup_ {i = 1} ^ {\infty} g ^ {- 1} \left(A _ {i}\right), \quad g ^ {- 1} \left(A ^ {\mathrm{c}}\right) = \left(g ^ {- 1} (A)\right) ^ {\mathrm{c}}
$$

quite generally for any sets and functions. Hence the collection of sets whose inverse images under the measurable function g are again measurable forms a σ-field containing the intervals, hence also contains all Borel sets. 

But we have found a measurable function f and a Lebesgue-measurable set $B$ for which $f ^ { - 1 } ( B ) = E$ is not measurable. Therefore the measurable set $B$ cannot be a Borel set, i.e. the inclusion $B \subset { \mathcal { M } }$ is strict. 



[1] T.M. Apostol, Mathematical Analysis, Addison–Wesley, Reading, 1974. 





[2] P.Billingsley, Probability and Measure, John Wiley and Sons, New York 1995 





[3] Z.Brzezniak, T.Zastawniak, Basic Stochastic Processes, Springer–Verlag, London 1999 





[4] M.Capinski, T.Zastawniak, Mathematics for Finance, An Introduction to Financial Engineering, Springer–Verlag, London 2003 





[5] R.J.Elliott, P.E.Kopp, Mathematics of Financial markets, Springer–Verlag, New York 1999 





[6] G.R. Grimmett and D.R. Stirzaker, Probability and Random Processes, Clarendon Press, Oxford, 1982. 





[7] J.Hull, Options, Futures, and Other Derivatives, Prentice Hall, Upper Saddle River NJ 2000 





[8] P.E. Kopp, Analysis, Modular Mathematics, Edward Arnold, London, 1996. 





[9] J. Pitman, Probability, Springer–Verlag, New York, 1995. 





[10] W. Rudin, Real and Complex Analysis, McGraw–Hill, New York, 1966. 





[11] G. Smith, Introductory Mathematics: Algebra and Analysis, Springer– Verlag, SUMS, 1998. 





[12] D. Williams, Probability with Martingales, Cambridge University Press, Cambridge, 1991. 



a.e., 55 – convergence, 242 a.s., 56 absolutely continuous, 189 – function, 109, 204 – measure, 107 adapted, 222 additive – countably, 27 additivity – countable, 29 – finite, 39 – of measure, 35 almost everywhere, 55 almost surely, 56 American option, 72 angle, 138 Banach space, 136 Beppo-Levi – theorem, 95 Bernstein – polynomials, 250 Bernstein-Weierstrass – theorem, 250 binomial – tree, 50 Black-Scholes – formula, 118 – model, 118 Borel – function, 57 – measure, regular, 44 – set, 40 Borel-Cantelli lemma 

– first, 257 – second, 258 bounded variation, 206 Brownian motion, 233 BV[a,b], 206 call option, 71 – down-and-out, 72 call-put parity, 117 Cantor – function, 303 – set, 19 Cauchy – density, 108 – sequence, 11, 128 central limit theorem, 276, 280 central moment, 146 centred – random variable, 151 characteristic function, 116, 272 Chebyshev’s inequality, 247 complete – measure space, 43 – space, 128 completion, 43 concentrated, 197 conditional – expectation, 153, 178, 179, 218 – probability, 47 contingent claim, 71, 72 continuity of measure, 39 continuous – absolutely, 204 convergence – almost everywhere, 242 

```txt
eventually, 256 
```

in L<sup>p</sup>, 242 

– in p-th mean, 144 

– in probability, 245 

– pointwise, 242 

– uniform, 11, 241 

– weak, 268 

correlation, 138, 151 

countable 

– additivity, 27, 29 

covariance, 151 

cover, 20 

## de Moivre–Laplace theorem, 280

de Morgan’s laws, 3 

– Cauchy, 108 

– Gaussian, 107, 174 

– joint, 173 

– normal, 107, 174 

– Radon-Nikodym, 194 

derivative security, 72 

Dirac measure, 68 

direct sum, 139 

distance, 126 

distribution 

– function, 109, 110, 199 

– gamma, 109 

– geometric, 69 

– marginal, 174 

– Poisson, 69 

– triangle, 107 

– uniform, 107 

dominated convergence theorem, 92 

dominating measure, 190 

Doob decomposition, 226 

## essential

– infimum, 66 

essentially bounded, 141 

```txt
event, 47 
```

```txt
expectation 
```

– conditional, 153, 178, 179, 218 

– of random variable, 114 

```txt
filtration, 51, 222 
```

```txt
- natural, 222 
```

first hitting time, 230 

## formula

– inversion, 180 

Fourier series, 140 

Fubini’s theorem, 171 

function 

– Borel, 57 

– Cantor, 303 

– characteristic, 116, 272 

– Dirichlet, 99 

– essentially bounded, 141 

– integrable, 86 

– Lebesgue, 20 

– Lebesgue measurable, 57 

– simple, 76 

– step, 102 

fundamental theorem of calculus, 9, 97, 214 

futures, 71 

## gamma distribution, 109

Gaussian density, 107, 174 

geometric distribution, 69 

## H¨older inequality, 142

Hahn-Jordan decomposition, 211, 216 

Hilbert space, 136, 138 

## i.o., 255

identically distributed, 244 

– random variables, 70, 244 

– Chebyshev, 247 

– H¨older, 142 

– Jensen, 220 

– Kolmogorov, 262 – Minkowski, 143 – Schwarz, 132, 143 – triangle, 126 

inner product, 135, 136 

integrable function, 86 

– improper Riemann, 99 

– Lebesgue, 77, 87 

– of a simple function, 76 

– Riemann, 7 

invariance
- translation, 35
inversion formula, 180
Ito isometry, 229

Jensen inequality, 220
joint density, 173

Kolmogorov inequality, 262 $L^{2}(E)$ , 131 $L^{p}(E)$ , 140 $L^{\infty}(E)$ , 141
law of large numbers
- strong, 260, 266
- weak, 249 $L^{p}$ convergence, 242
Lebesgue
- decomposition, 197
- function, 20
- integral, 76, 87
- measurable set, 27
- measure, 35
Lebesgue-Stieltjes
- measurable, 202
- measure, 199
lemma
- Borel-Cantelli, 257
- Fatou, 82
- Riemann–Lebesgue, 104
Levy's theorem, 274
liminf, 6
limsup, 6
Lindeberg–Feller theorem, 276
lower limit, 256
lower sum, 77

marginal distribution, 174
martingale, 223
- transform, 227
mean value theorem, 81
measurable
- function, 57
- Lebesgue-Stieltjes, 202
- set, 27
- space, 189
measure, 29
- absolutely continuous, 107
- Dirac, 68
- F-outer, 200
- Lebesgue, 35
- Lebesgue-Stieltjes, 199
- outer, 20, 45
- probability, 46 

– product, 164 – regular, 44 – σ-finite, 162 – signed, 209, 210 space, 29 measures – mutually singular, 197 metric, 126 Minkowski inequality, 143 model – binomial, 50 – Black-Scholes, 118 – CRR, 233 moment, 146 monotone class, 165 – theorem, 165 monotone convergence theorem, 84 monotonicity – of integral, 81 – of measure, 21, 35 Monte-Carlo method, 251 mutually singular measures, 197 negative part, 63 negative variation, 207 norm, 126 normal density, 107, 174 null set, 16 option – American, 72 – European, 71 – exotic, 72 – lookback, 72 orthogonal, 137–139 orthonormal – basis, 140 – set, 139 outer measure, 20, 45 parallelogram law, 136 partition, 190 path, 50 pointwise convergence, 242 Poisson distribution, 69 polarization identity, 136 portfolio, 183 positive part, 63 positive variation, 207 power set, 2 predictable, 225 probability, 46 conditional, 47 – distribution, 68 

– measure, 46 – space, 46 probability space – filtered, 222 process – stochastic, 222 – stopped, 230 product – measure, 164 – σ-field, 160 Prokhorov’s theorem, 272 put option, 72 

Radon-Nikodym – derivative, 194 – theorem, 190, 195 random time, 229 random variable, 66 – centred, 151 rectangle, 3 refinement, 7, 190 replication, 232 return, 183 Riemann – integral, 7 – – improper, 99 Riemann’s criterion, 8 Riemann–Lebesgue lemma, 104 – inner product, 136 – L<sup>2</sup>(E), 131 – L<sup>p</sup>(E), 140 – measurable, 189 – measure, 29 – probability, 46 standard normal distribution, 114 step function, 102 stochastic – integral, discrete, 227 – process, discrete, 222 stopped process, 230 stopping time, 229 strong law of large numbers, 266 subadditivity, 24 submartingale, 223 summable, 217 supermartingale, 224 supremum, 6 symmetric diference, 35 

## theorem

Beppo–Levi, 95 Bernstein-Weierstrass Approximation, 250 central limit, 276, 280 de Moivre–Laplace, 280 dominated convergence, 92 Fubini, 171 Fundamental of Calculus, 214 fundamental of calculus, 9, 97 – Helly, 270 intermediate value, 6 Levy, 274 Lindeberg–Feller, 276 mean value, 81 Miller-Modigliani, 117 monotone class, 165 monotone convergence, 84 Prokhorov, 272 Radon-Nikodym, 190, 195 Skorokhod representation, 110, 269 tight sequence, 272 total variation, 207 translation invariance – of measure, 35 – of outer measure, 26 triangle inequality, 126 triangular array, 282 

uncorrelated random variables, 151 uniform convergence, 11, 241 uniform distribution, 107 upper limit, 255 

upper sum, 77 

– positive, 212 – total, 207, 211 variance, 147 

variation 

weak 

– bounded, 206 

– convergence, 268 

– function, 207 

– negative, 212 

– law of large numbers, 249 

Wiener process, 233 

SPRINGER 

U 

UNDERGRADUATE 

MATHEMATICS 

Measure, Integral and Probability is a gentle introduction that makes measure and integration theory accessible to the average third-year undergraduate student. The ideas are developed at an easy pace in a form that is suitable for self-study, with an emphasis on clear explanations and concrete examples rather than abstract theory. 

SERIES 

For this second edition, the text has been thoroughly revised and expanded. New features include: 

• a substantial new chapter, featuring a constructive proof of the Radon-Nikodym theorem, an analysis of the structure of Lebesgue-Stieltjes measures, the Hahn-Jordan decomposition. and a brief introduction to martingales 

• key aspects of financial modelling, including the Black-Scholes formula, discussed briefly from a measure-theoretical perspective to help the reader understand the underlying mathematical frame-

In addition, further exercises and examples are provided to encourage the reader to become directly involved with the material. 

From the reviews of the first edition: 

"The level of explanation is excellent and great care has gone into providing motivation for the study of all aspects of the material. Overall, this is an excellent and interesting text. 

—Times Higher Education Supplement 

"A clear, understandable treatment of a very problematic area... The authors are to be commended for their lucid writing style —Journal of the American Statistical Association 

The Springer Undergraduate Mathematics Series (SUMS) is designed for undergraduates in the mathematical sciences. From core foundational material to final year topics, SUMS books take a fresh and modern approach and are ideal for self-study or for a one- or two-semester course. Each book includes numerous examples, problems and fully-worked solutions. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/6bca3f0a-251c-4443-9236-83abf830ad26/016438acddbe2636798c97a05299e349c3f89eb21c6691683d1c8c06dc785763.jpg)


springeronline.com 