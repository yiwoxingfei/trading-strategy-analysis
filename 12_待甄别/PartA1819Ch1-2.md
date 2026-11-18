

<!-- === Source: MinerU_markdown_PartA1819Ch1-2_1_2122706447723769856.md (Page 1) === -->

# Lecture notes for Part A Probability

Notes written by James Martin, updated by Matthias Winkel 

Oxford, Michaelmas Term 2018 

winkel@stats.ox.ac.uk 

Version of 30 September 2018 

(Chapters 1-2 of 7) 

Updates for remaining chapters to follow 

## Review: probability spaces, random variables, distributions, independence

## 1.1 Probability spaces and random variables

We start by reviewing the basic idea of a probability space introduced in last year’s course. This framework underlies modern probability theory, even though we will seldom need to appeal to it directly in this course. 

A probability space is a collection (Ω, F, P) with the following structure: 

(i) Ω is a set, which we call the sample space. 

(ii) F is a collection of subsets of Ω. An element of F is called an event. 

(iii) The probability measure P is a function from F to [0, 1]. It assigns a probability to each event in ${ \mathcal F } .$ 

We can think of the probability space as modelling an experiment. The sample space Ω represents the set of all possible outcomes of the experiment. 

The set F of events should satisfy certain natural conditions: 

(1) $\Omega \in { \mathcal { F } } .$ 

(2) If F contains a set A, then it also contains the complement $A ^ { c } \ ( { \mathrm { i . e . } } \ \Omega \setminus A )$ 

(3) If $( A _ { i } , i \in \mathcal { I } )$ is a finite or countably infinite collection of events in ${ \mathcal { F } } _ { : }$ , then their union $\cup _ { i \in \mathcal { I } } A _ { i }$ is also in F. 

By combining (2) and (3), we can also obtain finite or countable intersections, as well as unions. 

Finally, the probability measure P should satisfy the following conditions (the probability axioms): 

(1) $\mathbb { P } ( \Omega ) = 1 .$ 

(2) If $( A _ { i } , i \in \mathcal { T } )$ is a finite or countably infinite collection of disjoint events, then 

$$
\mathbb {P} \left(\bigcup_ {i \in \mathcal {I}} A _ {i}\right) = \sum_ {i \in \mathcal {I}} \mathbb {P} (A _ {i}).\tag{1.1}
$$

A random variable is a function defined on Ω. We will consider real-valued random variables, i.e. functions from Ω to R. 

A random variable represents an observable in our experiment; something we can “measure”. 

Formally, for a function X from Ω to R to be a random variable, we require that the subset 

$$
\{\omega \in \Omega \colon X (\omega) \leq x \}
$$

of Ω is an event in ${ \mathcal F } ,$ for every $x \in \mathbb { R } .$ . (Then, by taking complements, unions and intersections, we will in fact have that the set $\{ \omega \in \Omega \colon X ( \omega ) \in B \}$ is in $\mathcal { F }$ for a very large class of sets B). 

We will usually write X rather than $X ( \omega )$ for the value taken by a random variable. Thus if X is a random variable we can talk about the probability of the event 

$$
\{X \in B \} = \{\omega \in \Omega \colon X (\omega) \in B \},
$$

which we will write as $\mathbb { P } ( X \in B )$ 

Within one experiment, there will be many observables! That is, on the same probability space we can consider many diferent random variables. 

## Remarks:

(a) For very simple models, there may be a natural way to set up the sample space Ω (e.g. to represent the set of possible outcomes of the throw of a die or a coin). For more complicated models, this quickly becomes less straightforward. In practice, we hardly ever want to consider Ω directly; instead we work directly with the “events” and “random variables” (the “observables”) in the experiment. 

(b) In contrast, there are settings in probability theory where we care a lot about the collection of events ${ \mathcal F } ,$ and its structure. (For example, modelling a process evolving in time, we might have a family of diferent collections $\mathcal { F } _ { t } , t \geq 0 .$ where $\mathcal { F } _ { t }$ represents the set of events which can be observed by watching the evolution of the process up to time t). However, for the purposes of this course we will hardly ever worry about F directly; we will be safe to assume that F will always contain any event that we wish to consider. 

## 1.1.1 Examples

Here are some examples of systems (or “experiments”) that we might model using a probability space, and, for each one, some examples of random variables that we might want to consider within our model: 

• We throw two dice, one red and one blue. Random variables: the score on the red die; the score on the blue die; the sum of the two; the maximum of the two; the indicator function of the event that the blue score exceeds the red score.... 

• A Geiger counter detecting particles emitted by a radioactive source. Random variables: the time of the kth particle detected, for $k = 1 , 2 , \ldots ;$ the number of particles detected in the time interval [0, t], for $t \in [ 0 , \infty )$ 

• A model for the evolution of a financial market. Random variables: the prices of various stocks at various times; interest rates at various times; exchange rates at various times.... 

• The growth of a colony of bacteria. Random variables: the number of bacteria present at a given time; the diameter of the colonised region at given times; the number of generations observed in a given time interval.... 

• A call-centre. The time of arrival of the kth call; the length of service required by the kth caller; the wait-time of the kth caller in the queue before receiving service.... 

## 1.2 Probability distributions

We consider the distribution of a random variable X. This can be summarised by the distribution function (or cumulative distribution function) of X, defined by 

$$
F (x) = \mathbb {P} (X \leq x)
$$

for $x \in \mathbb { R }$ . (Once we know $F ,$ we can derive the probabilities $\mathbb { P } ( X \in B )$ for a very wide class of sets B by taking complements, intersections and unions. Formally, the distribution of a random variable X is the map $B \mapsto \mathbb { P } ( X \in B )$ , considered on a suitable collection of subsets $B \subseteq \mathbb { R }$ . In practice, we identify distributions by identifying the cumulative distribution function or any other associated function that uniquely determines a distribution.) 

Any distribution function F must obey the following properties: 

(1) F is non-decreasing. 

(2) F is right-continuous. 

(3) $F ( x ) \to 0 { \mathrm { ~ a s ~ } } x \to - \infty .$ 

(4) $F ( x ) \to 1 { \mathrm { ~ a s ~ } } x \to \infty .$ 

Remark 1.1. Note that two diferent random variables can have the same distribution! For example, consider the model of two dice mentioned above. If the dice are “fair”, then the distribution of the score on the blue die might be the same as the distribution of the score on the red die. However, that does not mean that the two scores are always the same! They are two diferent “observables” within the same experiment. 

If two random variables X and Y have the same distribution, we write $X { \overset { d } { = } } Y$ 

We single out two important classes of random variables: discrete and continuous. 

## 1.2.1 Discrete random variables

A random variable X is discrete if there is a finite or countably infinite set B such that $\mathbb { P } ( X \in B ) = 1$ 

We can represent the distribution of a discrete random variable X by its probability mass function 

$$
p _ {X} (x) = \mathbb {P} (X = x)
$$

for $x \in \mathbb { R }$ . This function is zero except at a finite or countably infinite set of points. We have 

$\begin{array} { r } { \sum _ { x } p _ { X } ( x ) = 1 . } \end{array}$ 

$\begin{array} { r } { \mathbb { P } ( X \in A ) = \sum _ { x \in A } p _ { X } ( x ) } \end{array}$ for any set $A \subseteq \mathbb { R }$ 

The points x where $\mathbb { P } ( X = x ) > 0$ are sometimes called the atoms of the distribution of X. In many examples these will be a set of integers such as $\{ 1 , 2 , \ldots , n \}$ or $\{ 0 , 1 , 2 , \ldots \}$ or $\{ 1 , 2 , 3 , \ldots \}$ 

The cumulative distribution function of X has jumps at the location of the atoms, and is constant on any interval that does not contain an atom. 

## 1.2.2 Continuous random variables

A random variable X is called (absolutely) continuous if its distribution function F can be written as an integral. That is, there is a function f such that 

$$
\mathbb {P} (X \leq x) = F (x) = \int_ {- \infty} ^ {x} f (u) d u.
$$

$f$ is called the density function (or probability density function) of X. 

This certainly implies that F is a continuous function (although note that not all continuous F can be written in this way). In particular, $\mathbb { P } ( X = x ) = F ( x ) - \operatorname* { l i m } _ { y \uparrow x } F ( y ) = 0$ for any x. The density function is not unique; for example, we can change the value of $f$ at any single point without afecting the integral of $f .$ At points where F is diferentiable, it is natural to take $f ( x ) = F ^ { \prime } ( x )$ . For any $a < b ,$ we have 

$$
\mathbb {P} (a \leq X \leq b) = \int_ {a} ^ {b} f (u) d u.
$$

## 1.2.3 Median

The median of a distribution with cumulative distribution function $F$ is $m \in \mathbb { R }$ such that $F ( m ) = 1 / 2$ , if such m is unique, or the midpoint $m = ( a + b ) / 2$ of the interval $( a , b )$ , where where $F ( x ) = 1 / 2 , x \in ( a , b )$ 

## 1.3 Expectation and variance

Let X be a discrete random variable with probability mass function $p _ { X } ( x ) = \mathbb { P } ( X = x )$ . The expectation (or mean) of X is defined by 

$$
\mathbb {E} X = \mathbb {E} (X) = \sum_ {x} x p _ {X} (x),\tag{1.2}
$$

when this sum converges. 

If instead X is a continuous random variable with density function $f ,$ then its expectation is given by 

$$
\mathbb {E} X = \mathbb {E} (X) = \int_ {- \infty} ^ {\infty} x f (x) d x,\tag{1.3}
$$

when this integral converges. 

We often want to express the expectation of a function of a random variable X in terms of the density function or the mass function of X. We have 

$$
\mathbb {E} g (X) = \sum_ {x} g (x) p _ {X} (x)
$$

in the discrete case, and 

$$
\mathbb {E} g (X) = \int_ {- \infty} ^ {\infty} g (x) f (x) d x
$$

in the continuous case, always provided that the expectation exists, i.e. that the sum or integral converges. 

It is rather unsatisfactory that we have two diferent definitions of expectation for two diferent cases, and no definition at all for random variables which are neither continuous nor discrete. In fact it is not dificult to unify the definitions. A very natural way is to consider approximations of a general random variable by discrete random variables. This is analogous to the construction of the integral of a general function by defining the integral of a step function using sums, and then defining the integral of a general function using an approximation by step functions, which you saw in last year’s analysis course. 

This unifies the two definitions above, and extends the definition to all types of random variable, whether discrete, continuous or neither. We will not pursue this here – but we will collect together basic properties of expectation which we will use constantly: 

(1) For any event A, write $\mathbf { 1 } _ { A }$ for the indicator function of A. Then $\mathbb { E } \mathbf { 1 } _ { A } = \mathbb { P } ( A )$ 

(2) If $\mathbb { P } ( X \geq 0 ) = 1$ , then $\operatorname { \mathbb { E } } X \geq 0$ 

(3) (Linearity 1): $\mathbb { E } \left( a X \right) = a \mathbb { E } X$ for any constant a. 

(4) (Linearity 2): $\mathbb { E } \left( X + Y \right) = \mathbb { E } X + \mathbb { E } Y .$ 

Formally, E is a linear operator on the vector space of random variables $X \colon \Omega  \mathbb { R }$ whose expectations exist. 

## 1.3.1 Variance and covariance

The variance of a random variable X is defined by 

$$
\operatorname{Var} (X) = \mathbb {E} \left[ (X - \mathbb {E} X) ^ {2} \right],
$$

provided that the expectations exist. This can then alternatively be expressed as 

$$
\operatorname{Var} (X) = \mathbb {E} \left(X ^ {2}\right) - (\mathbb {E} X) ^ {2}.
$$

The covariance of two random variables X and Y is defined by 

$$
\operatorname{Cov} (X, Y) = \mathbb {E} \left[ (X - \mathbb {E} X) (Y - \mathbb {E} Y) \right],
$$

if the expectations exist, which can then alternatively be expressed as 

$$
\operatorname{Cov} (X, Y) = \mathbb {E} (X Y) - (\mathbb {E} X) (\mathbb {E} Y).
$$

Note that $\operatorname { V a r } ( X ) = \operatorname { C o v } ( X , X )$ . From the linearity of expectation, we get a bi-linearity property for covariance: 

$$
\operatorname{Cov} (a X + b, c Y + d) = a c \operatorname{Cov} (X, Y).
$$

As a special case we can obtain 

$$
\operatorname{Var} (a X + b) = a ^ {2} \operatorname{Var} (X).
$$

We also have the property 

$$
\operatorname{Var} (X + Y) = \operatorname{Var} (X) + \operatorname{Var} (Y) + 2 \operatorname{Cov} (X, Y)
$$

and more generally 

$$
\operatorname{Var} \left(X _ {1} + X _ {2} + \dots + X _ {n}\right) = \sum_ {i = 1} ^ {n} \operatorname{Var} \left(X _ {i}\right) + 2 \sum_ {1 \leq i <   j \leq n} \operatorname{Cov} \left(X _ {i}, X _ {j}\right),
$$

always provided that all expectations exist. 

## 1.4 Independence

Events A and B are independent if 

$$
\mathbb {P} (A \cap B) = \mathbb {P} (A) \mathbb {P} (B).
$$

More generally, a family of events $( A _ { i } , i \in \mathcal { I } )$ , possibly infinite, even uncountable, is called independent if for all finite subsets J of I, 

$$
\mathbb {P} \left(\bigcap_ {i \in J} A _ {i}\right) = \prod_ {i \in J} \mathbb {P} (A _ {i}).
$$

Remark 1.2. Remember that this is a stronger condition than pairwise independence! Even for three events, it is possible that $A _ { 1 } , A _ { 2 }$ are independent, $A _ { 2 } , A _ { 3 }$ are independent and $A _ { 1 } , A _ { 3 }$ are independent but that $A _ { 1 } , A _ { 2 } , A _ { 3 }$ are not independent. 

Random variables $X _ { 1 } , X _ { 2 } , \ldots , X _ { n }$ are independent if for all $B _ { 1 } , B _ { 2 } , \ldots , B _ { n } \subset \mathbb { R }$ , the events $\{ X _ { 1 } \in B _ { 1 } \} , \{ X _ { 2 } \in B _ { 2 } \} , . . . , \{ X _ { n } \in B _ { n } \}$ are independent. 

In fact, it turns out to be enough to check that for all $x _ { 1 } , x _ { 2 } , \ldots , x _ { n } .$ 

$$
\begin{array}{c} \mathbb {P} (X _ {1} \leq x _ {1}, \ldots , X _ {n} \leq x _ {n}) = \mathbb {P} (X _ {1} \leq x _ {1}) \dots \mathbb {P} (X _ {n} \leq x _ {n}) \\ = F _ {X _ {1}} (x _ {1}) \dots F _ {X _ {n}} (x _ {n}). \end{array}
$$

If the random variables are all discrete, another equivalent condition is that 

$$
\mathbb {P} (X _ {1} = x _ {1}, \ldots , X _ {n} = x _ {n}) = \mathbb {P} (X _ {1} = x _ {1}) \dots \mathbb {P} (X _ {n} = x _ {n}).
$$

When X and Y are independent random variables whose expectations exist, we have $\mathbb { E } \left( X Y \right) = \mathbb { E } \left( X \right) \mathbb { E } \left( Y \right)$ , or equivalently $\operatorname { C o v } ( X , Y ) = 0$ That is, X and Y are uncorrelated. The converse is not true; uncorrelated does not imply independent! 

Various of the properties above can be summarised by the phrase “independence means multiply”. 

## 1.5 Examples of probability distributions

We review some of the families of probability distributions which are of particular importance in applications and in theory. 

## 1.5.1 Continuous distributions

## Uniform distribution

X has the uniform distribution on an interval $[ a , b ]$ if its probability density function is given by 

$$
f (x) = \left\{ \begin{array}{l l} \frac {1}{b - a}, & \text { if } a \leq x \leq b, \\ 0, & \text { otherwise }. \end{array} \right.
$$

We write $X \sim U [ a , b ]$ 

## Exponential distribution

X has exponential distribution with parameter (or rate) λ if its distribution function is given by 

$$
F (x) = \left\{ \begin{array}{l l} 0, & x <   0, \\ 1 - e ^ {- \lambda x}, & x \geq 0. \end{array} \right.
$$

Its density function is 

$$
f (x) = \left\{ \begin{array}{l l} 0 & x <   0 \\ \lambda e ^ {- \lambda x} & x \geq 0 \end{array} \right..
$$

We write $X \sim \exp ( \lambda )$ We have $\mathbb { E } X = 1 / \lambda$ and Var $X = 1 / \lambda ^ { 2 }$ . If $X \sim \exp ( \lambda )$ and $a > 0 .$ , then $a X \sim \mathrm { E x p } ( \lambda / a )$ . An important property of the distribution is the memoryless property: $\mathbb { P } ( X > x + t | X > t )$ does not depend on t. 

## Normal distribution

X has the normal (or Gaussian) distribution with mean $\mu$ and variance $\sigma ^ { 2 }$ if its density function is given by 

$$
f (x) = \frac {1}{\sqrt {2 \pi \sigma^ {2}}} \exp \left(- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}\right).
$$

We write $X \sim N ( \mu , \sigma ^ { 2 } )$ . The standard normal distribution is $N ( 0 , 1 )$ 

If $X \sim N ( \mu , \sigma ^ { 2 } )$ then $a X + b \sim N ( a \mu + b , a ^ { 2 } \sigma ^ { 2 } )$ . In particular, $( X - \mu ) / \sigma$ has standard normal distribution. 

$\mathrm { I f } X \sim N ( \mu _ { X } , \sigma _ { X } ^ { 2 } )$ and $Y \sim N ( \mu _ { Y } , \sigma _ { Y } ^ { 2 } )$ are independent, $X + Y \sim N ( \mu _ { X } + \mu _ { Y } , \sigma _ { X } ^ { 2 } + \sigma _ { Y } ^ { 2 } )$ 

The normal distribution has an extremely important role in probability theory, exemplified by the fact that it appears as the limit in the Central Limit Theorem. 

We often write Φ for the distribution function of the standard normal distribution: 

$$
\Phi (x) = \int_ {- \infty} ^ {x} {\frac {1}{\sqrt {2 \pi}}} \exp \left(- \frac {z ^ {2}}{2}\right) d z.
$$

## Gamma distribution

The family of gamma distributions generalises the family of exponential distributions. The gamma distribution with rate λ and shape r has densit 

$$
f (x) = \left\{ \begin{array}{l l} \frac {\lambda^ {r}}{\Gamma (r)} x ^ {r - 1} e ^ {- \lambda x} & x \geq 0 \\ 0 & x <   0 \end{array} \right..
$$

Here $\Gamma ( r )$ is the gamma function, defined by $\begin{array} { r } { \Gamma ( r ) = \int _ { 0 } ^ { \infty } z ^ { r - 1 } e ^ { - z } d z } \end{array}$ . It is the analytic continuation of the factorial function, in that $\Gamma ( r ) = ( r - 1 ) !$ when r is an integer. 

A gamma distribution with shape $r = 1$ is an exponential distribution. 

If $X \sim \mathrm { G a m m a } ( r _ { X } , \lambda )$ and $Y \sim \mathrm { G a m m a } ( r _ { Y } , \lambda )$ are independent, then we have $X + Y \sim$ Gamma $\left( r _ { X } + r _ { Y } , \lambda \right)$ . As a special case, if $X _ { 1 } , X _ { 2 } , \ldots , X _ { n }$ are i.i.d. with Exp(λ) distribution, then $X _ { 1 } + X _ { 2 } + \cdots + X _ { n }$ has $\mathrm { G a m m a } ( n , \lambda )$ distribution. 

## 1.5.2 Discrete distributions

Discrete uniform distribution 

X has the discrete uniform distribution on a set B of size n (for example the set $\{ 1 , 2 , \ldots , n \} )$ 1 if 

$$
p _ {X} (x) = \left\{ \begin{array}{l l} 1 / n, & x \in B \\ 0, & x \notin B \end{array} \right..
$$

## Bernoulli distribution

X has Bernoulli distribution with parameter p if 

$$
p _ {X} (1) = p, p _ {X} (0) = 1 - p
$$

(and so of course $p _ { X } ( x ) = 0$ for other values of x). 

We have E $X = p$ and Var $X = p ( 1 - p )$ 

If A is an event with $\mathbb { P } ( A ) = p ,$ then its indicator function 14 $\mathbf { 1 } _ { A }$ has Bernoulli distribution with parameter p. 

## Binomial distribution

If $X _ { 1 } , X _ { 2 } , \ldots , X _ { n }$ are i.i.d. Bernoulli random variables with the same parameter $p ,$ then their sum $X _ { 1 } + \cdots + X _ { n }$ has Binomial distribution with parameters n and $p .$ 

Equivalently, if $A _ { 1 } , \ldots , A _ { n }$ are independent events, each with probability $p ,$ then the total number of those events which occur has Binomia $\scriptstyle { \mathrm { l } } ( n , p )$ distribution. 

If X ∼ Binomial(n, p) then 

$$
p _ {X} (k) = \binom {n} {k} p ^ {k} (1 - p) ^ {n - k} \quad \text { for } k \in \{0, 1, \ldots , n \}.
$$

E $X = n p$ and Var $X = n p ( 1 - p )$ 

## Geometric distribution

Let $p \in ( 0 , 1 )$ and let X have mass function 

$$
p _ {X} (k) = (1 - p) ^ {k - 1} p \quad \text { for } k \in \{1, 2, 3, \dots \}.
$$

Let $Y = X - 1 ;$ ; then Y has mass function 

$$
p _ {Y} (k) = (1 - p) ^ {k} p \quad \text { for } k \in \{0, 1, 2, \ldots \}.
$$

The terminology is not consistent; either X or Y might be said to have a geometric distribution with parameter $p .$ (Or even sometimes with parameter $1 - p )$ 

If we have a sequence of independent trials, with probability p of success at each trial, then X could represent the number of trials needed for the first success to occur, while $Y$ could represent the number of failures needed before the first success occurs. 

We have 

$$
\mathbb {P} (X > k) = \mathbb {P} (Y \geq k) = (1 - p) ^ {k} \quad \mathrm{for} k = 0, 1, 2, \ldots .
$$

The geometric distribution can be thought of as a discrete anaologue of the exponential distribution. It too has a memoryless property; for $k , m \in \{ 0 , 1 , 2 , \ldots \}$ , the conditional probability $\mathbb { P } ( X > k + m | X > k )$ does not depend on k. 

## Poisson distribution

X has Poisson distribution with mean λ if 

$$
\mathbb {P} (X = r) = \frac {e ^ {- \lambda} \lambda^ {r}}{r !} \quad \mathrm{for} r = 0, 1, 2, \ldots .
$$

E $X = \lambda$ and Var $X = \lambda$ 

I $\mathrm { ~ f ~ } X \sim \operatorname { P o i s s o n } ( \lambda )$ and $Y \sim \operatorname { P o i s s o n } ( \mu )$ are independent, then $X + Y \sim \operatorname { P o i s s o n } ( \lambda + \mu )$ 

The Poisson distribution arises in many applications; it is a good model for the total number of events occurring when there are a large number of possible events which each occur with small probability. There are close connections between the Poisson distribution and the exponential distribution, which we will see in detail when we study Poisson processes at the end of the course. 

# Convergence of random variables, and limit theorems

Let X and $Y$ be random variables. What might we mean by saying $^ { 6 6 } X$ and $Y$ are close”? 

(1) We might be describing a particular realisation. For example, we made an observation of X and $Y .$ , and on this occasion $| X - Y | < \epsilon$ 

(2) We might be making a statement about the joint distribution of X and Y, for example 

$$
\mathbb {P} (| X - Y | <   \epsilon) > 1 - \epsilon ,
$$

or 

$$
\mathbb {E} \left(\left| X - Y \right|\right) <   \epsilon .
$$

(3) We might be comparing the distribution of X with the distribution of $Y _ { ; }$ , for example 

$$
\left| F _ {X} (x) - F _ {Y} (x) \right| <   \epsilon \text {   for   all   } x.
$$

Correspondingly, there are several diferent things we might mean when we say that a sequence of random variables converges to a limit. 

## 2.1 Modes of convergence

Let $X _ { 1 } , X _ { 2 } , . . .$ . and X be random variables. 

Note that $\{ X _ { n } \to X { \mathrm { ~ a s ~ } } n \to \infty \}$ is an event. More formally we could write 

$$
\{\omega \in \Omega \colon X _ {n} (\omega) \to X (\omega) \text { as } n \to \infty \}
$$

to emphasise the dependence on $\omega ;$ the event might hold for some $\omega$ but not for others. 

Definition. $X _ { n } \to X$ almost surely $( o r$ “with probability 1”) $i f$ 

$$
\boxed {\mathbb {P} \left(X _ {n} \to X a s n \to \infty\right) = 1.}\tag{2.1}
$$

We often abbreviate to $^ { 4 } X _ { n }  X \ a . s . ^ { \ 3 5 }$ 

Definition. $X _ { n } \to X$ in probability (written $X _ { n } \ { \overset { P } { \to } } \ X ) \ i f$ for every $\epsilon > 0$ 2 

$$
\boxed {\mathbb {P} \Big (\big | X _ {n} - X \big | <   \epsilon \Big) \to 1 a s n \to \infty .}\tag{2.2}
$$

Let $F _ { 1 } , F _ { 2 } , \ldots$ . and F be the distribution functions of $X _ { 1 } , X _ { 2 } , . . .$ . and X respectively. 

Definition. $X _ { n } \to X$ in distribution $( o r \ w e a k l y )$ , written $X _ { n } \stackrel { d } { \to } X , i f ,$ for every x such that F is continuous at $x _ { i }$ 

$$
\boxed {F _ {n} (x) \to F (x) a s n \to \infty .}\tag{2.3}
$$

We will see later that these formulations are in decreasing order of strength. 

## 2.2 Convergence in distribution

Notice that in the definition of convergence in distribution in (2.3), the random variables involved appear only through their distributions. Hence we do not even need all the random variables to be defined on the same probability space. This is really a definition about convergence of distributions, not about convergence of random variables. The joint distribution of the random variables does not need to be defined. This is in contrast to the definitions of almost sure convergence in (2.1) and of convergence in probability in (2.2), where we genuinely do need all the random variables to be defined on the same space. 

As a result, we might sometimes vary the notation by writing a distribution rather than a random variable on the right-hand side; e.g. $\ ^ { * } X _ { n } \ { \overset { d } { \to } } \ N ( 0 , 1 ) ^ { * }$ if the limit in distribution is the standard normal, or $^ { \mathfrak { a } } X _ { n } \ { \overset { d } { \to } } \ U [ 0 , 1 ] ^ { \mathfrak { n } }$ if the limit in distribution is the uniform distribution on [0, 1]. 

In many cases the limit will be deterministic; e.g. if the limit is a distribution which puts all its mass at the value 0, then we will write $X _ { n } \overset { d } { \to } 0$ 

In (2.3), why did we ask for the limit to hold only for x which are continuity points of $F .$ , rather than at all x? The first couple of examples (which are almost trivial) make this clear. 

Example 2.1. Let $X _ { n }$ have the uniform distribution on the interval $[ - 1 / n , 1 / n ]$ . Then $F _ { n } ( x ) \to 0$ for all $x < 0$ , and $F _ { n } ( x ) \to 1$ for all $x > 0$ 

So we have $X _ { n } \stackrel { d } { \to } 0 , \mathrm { i . e }$ . the distribution of $X _ { n }$ converges to that of a deterministic random variable which is equal to 0 with probability 1. Such a random variable has distribution function given by $F ( x ) = 0$ for $x < 0$ and $F ( x ) = 1$ for $x \geq 0$ 

Note that $F _ { n } ( 0 ) = 1 / 2$ for all n, while $F ( 0 ) = 1$ . So convergence does not hold at the point 0 itself (but this is OK, since 0 is not a continuity point of $F )$ 

Example 2.2. Let $X _ { n }$ be a deterministic random variable taking the value $1 / n$ with probability 1. Let X be a deterministic random variable taking the value 0 with probability 1 (as above). Then once again, $X _ { n } \stackrel { d } { \to } X$ , (even though $\mathbb { P } ( X _ { n } \ \le \ 0 ) \ = \ 0$ for all n while $\mathbb { P } ( X \leq 0 ) = 1 )$ . 

There are many situations in which a sequence of discrete random variables converges to a continuous limit. Here is one example, showing that a geometric distribution with a small parameter is well approximated by an exponential distribution: 

Example 2.3. Let $X _ { n }$ have geometric distribution on the positive integers, with parameter $p _ { n } ,$ , i.e. $\mathbb { P } ( X _ { n } = k ) = ( 1 - p _ { n } ) ^ { k - 1 } p _ { n }$ for $k = 1 , 2 , \dots$ . Show that if $p _ { n } \to 0 { \mathrm { ~ a s ~ } } n \to \infty$ , then $p _ { n } X _ { n }$ converges in distribution to the exponential distribution with mean 1. 

Solution: We have $\mathbb { P } ( X _ { n } > k ) = ( 1 - p _ { n } ) ^ { k }$ for $k = 0 , 1 , 2 , \ldots$ . For $x \geq 0$ , we have 

$$
\begin{array}{r l} & {\mathbb {P} (p _ {n} X _ {n} > x) = \mathbb {P} \left(X _ {n} > \frac {x}{p _ {n}}\right)} \\ & {\qquad = \mathbb {P} \left(X _ {n} > \left\lfloor \frac {x}{p _ {n}} \right\rfloor\right)} \\ & {\qquad = (1 - p _ {n}) ^ {\lfloor x / p _ {n} \rfloor}} \\ & {\qquad \to e ^ {- x} \text {as} n \to \infty} \end{array}
$$

because $p _ { n }  0 ^ { }$ ; here we use the fact that $( 1 - \epsilon ) ^ { x / \epsilon } \to e ^ { - x } \mathrm { a s } \epsilon \to 0$ , and also that $| x / p _ { n } | - x / p _ { n }$ is bounded. 

Hence if $F _ { n }$ is the distribution function of $p _ { n } X _ { n }$ , then $1 - F _ { n } ( x ) \to e ^ { - x } { \mathrm { ~ a s ~ } } n \to \infty$ . So $F _ { n } ( x )  1 - e ^ { - x }$ for all $x > 0$ , while $F _ { n } ( x ) = 0$ for all $x \leq 0$ and all n. 

So indeed $F _ { n } ( x )  F ( x )$ for all $x ,$ where F is the distribution function of a random variable with Exp(1) distribution. 

There are several more examples on the problem sheets. 

## 2.3 Comparison of diferent modes of convergence

Theorem 2.4. The following implications hold: 

$$
\boxed {X _ {n} \rightarrow X \text {   almost   surely }} \Rightarrow \boxed {X _ {n} \rightarrow X \text {   in   probability }} \Rightarrow \boxed {X _ {n} \rightarrow X \text {   in   distribution }}
$$

The reverse implications do not hold in general. 

Before starting the proof we note a useful fact, which is a simple consequence of the countable additivity axiom for unions of disjoint sets (1.1). 

Lemma 2.5. Let $A _ { n } , n \geq 1$ , be an increasing sequence of events; that is, $A _ { 1 } \subseteq A _ { 2 } \subseteq A _ { 3 } \subseteq . . .$ Then 

$$
\lim _ {n \to \infty} \mathbb {P} (A _ {n}) = \mathbb {P} \left(\bigcup_ {n \geq 1} A _ {n}\right).\tag{2.4}
$$

Proof. Because the sequence $A _ { n }$ is increasing, it is easy to rewrite the union as a disjoint union: 

$$
\begin{array}{l} \mathbb {P} \left(\bigcup_ {n \geq 1} A _ {n}\right) = \mathbb {P} \Big (A _ {1} \cup \bigcup_ {n \geq 1} (A _ {n + 1} \setminus A _ {n}) \Big) \\ \qquad = \mathbb {P} (A _ {1}) + \sum_ {i = 1} ^ {\infty} \mathbb {P} \big (A _ {i + 1} \setminus A _ {i} \big) \quad (\text { using   countable   additivity }) \\ \qquad = \mathbb {P} (A _ {1}) + \lim _ {n \to \infty} \sum_ {i = 1} ^ {n - 1} \mathbb {P} \left(A _ {i + 1} \setminus A _ {i}\right) \end{array}
$$

$$
\begin{array}{l} = \lim _ {n \to \infty} \Big (\mathbb {P} (A _ {1}) + \sum_ {i = 1} ^ {n - 1} \mathbb {P} (A _ {i + 1} \setminus A _ {i}) \Big) \\ = \lim _ {n \to \infty} \mathbb {P} \Big (A _ {1} \cup \bigcup_ {1 \leq i \leq n - 1} (A _ {i + 1} \setminus A _ {i}) \Big) \\ = \lim _ {n \to \infty} \mathbb {P} (A _ {n}). \end{array}
$$

Proof of Theorem ${ 2 . 4 } .$ 

(1) First we will show that convergence in probability implies convergence in distribution. Let $F _ { n }$ be the distribution function of $X _ { n } ,$ , and F the distribution function of X. Fix any x such that F is continuous at x, and fix any $\epsilon > 0$ 

Observe that if $X _ { n } \leq x .$ , then either $X \leq x + \epsilon \ \mathrm { o r } \ | X _ { n } - X | > \epsilon$ . Hence 

$$
\begin{array}{l}F _ {n} (x) = \mathbb {P} (X _ {n} \leq x)\\\quad \leq \mathbb {P} \big (X \leq x + \epsilon \text {or} | X _ {n} - X | > \epsilon \big)\\\quad \leq \mathbb {P} \big (X \leq x + \epsilon \big) + \mathbb {P} \big (| X _ {n} - X | > \epsilon \big)\\\quad \rightarrow F (x + \epsilon) \text {as} n \rightarrow \infty ,\end{array}
$$

using the convergence in probability. So $F _ { n } ( x ) < F ( x + \epsilon ) + \epsilon$ for all large enough n. 

Similarly by looking at $1 - F _ { n } ( x ) = \mathbb { P } ( X _ { n } > x )$ , we can obtain that $F _ { n } ( x ) > F ( x - \epsilon ) - \epsilon$ for all large enough n. 

Since $\epsilon > 0$ is arbitrary, and since F is continuous at x, this implies that $F _ { n } ( x ) \to F ( x )$ as $n \to \infty$ 

(4) Finally we want to show that convergence in probability does not imply almost sure convergence. 

Consider a sequence of independent random variables $X _ { n }$ where $\mathbb { P } ( X _ { n } = 1 ) = 1 / n$ and $\mathbb { P } ( X _ { n } = 0 ) = ( n - 1 ) / n$ 

We have $X _ { n } \ \to \ 0$ in probability as $n  \infty$ because for any $\epsilon > 0 , \mathbb { P } ( | X _ { n } - 0 | < \epsilon ) \geq$ $\mathbb { P } ( X = 0 )  1$ 

Since $X _ { n }$ only take the values 0 and 1, the event $\{ X _ { n } \to 0 \}$ is the same as the event $\{ X _ { n } = 0$ eventually}. This is $\textstyle \bigcup _ { N \geq 1 } B _ { N }$ where $B _ { N } = \{ X _ { n } = 0$ for all $n \geq N \}$ 

But for any N and $K _ { \colon }$ 

$$
\begin{array}{l} \mathbb {P} (B _ {N}) \leq \mathbb {P} (X _ {n} = 0 \text {   for   all   } n = N, \ldots , N + K) = \frac {N - 1}{N} \frac {N}{N + 1} \frac {N + 1}{N + 2} \dots \frac {N + K - 1}{N + K} \\ = \frac {N - 1}{N + K}. \end{array}
$$

As $K \geq 1$ is arbitrary, we obtain that $\mathbb { P } ( B _ { N } ) = 0$ . Hence also by Lemma 2.5, $\begin{array} { r } { \mathbb { P } ( \bigcup _ { N \geq 1 } B _ { N } ) = } \end{array}$ 0, and so $\mathbb { P } ( X _ { n }  0 ) = 0$ . Hence it is not the case that $X _ { n }$ converges to 0 almost surely. 

Although convergence in distribution is weaker than convergence in probability, there is a partial converse, for the case when the limit is deterministic: 

Theorem 2.6. Let $X _ { 1 } , X _ { 2 } , . . .$ . be a sequence of random variables defined on the same probability space. If $X _ { n }  c$ in distribution where c is some constant, then also $X _ { n }  c$ in probability. 

Proof. Exercise (see problem sheet). 

## 2.4 Review: Weak law of large numbers

This was covered at the end of last year’s course (without explicitly introducing the notion of convergence in probability). 

Let $S _ { n } = X _ { 1 } + X _ { 2 } + \cdot \cdot \cdot + X _ { n } ,$ where $X _ { i }$ are i.i.d. with mean $\mu .$ The law of large numbers tells us that, roughly speaking, $S _ { n }$ behaves to first order like nµ as $n  \infty$ . The weak law phrases this in terms of convergence in probability. (Later we will see a stronger result in terms of almost sure convergence). 

Theorem (Weak Law of Large Numbers). Let $X _ { 1 } , X _ { 2 } , . . .$ . be i.i.d. random variables with finite mean $\mu .$ . Let $S _ { n } = X _ { 1 } + X _ { 2 } + \cdot \cdot \cdot + X _ { n }$ . Then 

$$
\frac {S _ {n}}{n} \stackrel {P} {\rightarrow} \mu \text {as} n \rightarrow \infty .
$$

That is, for all $\epsilon > 0$ ， 

$$
\mathbb {P} \left(\left| \frac {S _ {n}}{n} - \mu \right| <   \epsilon\right)\rightarrow 1 a s n \rightarrow \infty .\tag{2.5}
$$

Given Theorem 2.6, we could equivalently write ${ \frac { S _ { n } } { n } } \ { \overset { d } { \to } } \ \mu .$ 

We will give an extremely simple proof of the weak law of large numbers, under an additional condition (that the $X _ { i }$ have finite variance). To do this, we need some results which give probability bounds on the tail of a distribution in terms of its mean and variance. 

Theorem (Markov’s inequality). Let X be random variable taking non-negative values $( i . e .$ $\mathbb { P } ( X \geq 0 ) = 1 )$ . Then for any $z > 0$ 

$$
\mathbb {P} (X \geq z) \leq \frac {\mathbb {E} X}{z}.\tag{2.6}
$$

Proof. We consider a random variable $X _ { z } = z { \bf 1 } \{ X \ge z \}$ . So $X _ { z }$ takes the value 0 whenever X is in $[ 0 , z )$ and the value z whenever X is in $[ z , \infty )$ . So $X \geq X _ { z }$ always (here we use the fact that X is non-negative). 

Then E $\begin{array} { r } { \colon X \geq \operatorname { \mathbb { E } } X _ { z } = z \operatorname { \mathbb { E } } \mathbf { 1 } \{ X \geq z \} = z \operatorname { \mathbb { P } } ( X \geq z ) } \end{array}$ . Rearranging gives the result. 

Theorem (Chebyshev’s inequality). Let Y be a random variable with finite mean and variance. Then for any $\epsilon > 0$ 2 

$$
\mathbb {P} \big (| Y - \mathbb {E} Y | \geq \epsilon \big) \leq \frac {\operatorname{Var} Y}{\epsilon^ {2}}.
$$

Proof. 

$$
\begin{array}{c} \mathbb {P} \big (| Y - \mathbb {E} Y | \geq \epsilon \big) = \mathbb {P} \big ([ Y - \mathbb {E} Y ] ^ {2} \geq \epsilon^ {2} \big) \\ \leq \frac {\mathbb {E} \left([ Y - \mathbb {E} Y ] ^ {2}\right)}{\epsilon^ {2}} \end{array}
$$

(by applying Markov’s inequality (2.6) with $X = [ Y - \mathbb { E } Y ] ^ { 2 }$ and $z = \epsilon ^ { 2 } )$ 1 

$$
= \frac {\mathrm{Var} Y}{\epsilon^ {2}}.
$$

Proof of the weak law of large numbers in the case $o f$ random variables with finite variance. Let $X _ { i }$ be i.i.d. with mean $\mu$ and variance $\sigma ^ { 2 }$ . Recall $S _ { n } = X _ { 1 } + \cdot \cdot \cdot + X _ { n }$ . We want to show that $S _ { n } / n \stackrel { P } {  } \mu$ as $n \to \infty$ 

We have E $( S _ { n } / n ) = \mu ,$ and (using the independence of the $X _ { i } )$ 

$$
\begin{array}{r l} \operatorname{Var} \left(\frac {S _ {n}}{n}\right) & = \frac {\operatorname{Var} S _ {n}}{n ^ {2}} \\ & = \frac {\operatorname{Var} X _ {1} + \cdots + \operatorname{Var} X _ {n}}{n ^ {2}} \\ & = \frac {n \sigma^ {2}}{n ^ {2}} \\ & = \frac {\sigma^ {2}}{n}. \end{array}
$$

Fix any $\epsilon > 0$ . Using Chebyshev’s inequality applied to the random variable $S _ { n } / n .$ , we have 

$$
\begin{array}{c} \mathbb {P} \left(\left| \frac {S _ {n}}{n} - \mu \right| \geq \epsilon\right) \leq \frac {\operatorname{Var} \left(\frac {S _ {n}}{n}\right)}{\epsilon^ {2}} \\ = \frac {\sigma^ {2}}{n \epsilon^ {2}} \\ \to 0 \text {as} n \to \infty . \end{array}
$$

So indeed (2.5) holds, as required. 

Remark. Observe that we could relax considerably the assumptions in the weak law of large numbers, and still get the same result using almost the same proof. We never used at all the assumption that the $X _ { i }$ all had the same distribution. We could also relax the assumption that the $X _ { i }$ are independent, as long as the variance of $S _ { n }$ grows more slowly than $n ^ { 2 }$ . For example, if we have an upper bound on the variance of each $X _ { i } ,$ and a bound which is $o ( n ^ { 2 } )$ on the sum $\begin{array} { r } { \sum _ { 1 \leq i < j \leq n } \operatorname { C o v } ( X _ { i } , X _ { j } ) } \end{array}$ , then exactly the same idea applies to show that $( S _ { n } - \mathbb { E } S _ { n } ) / n$ converges to 0 in distribution. 

## 2.5 Strong law of large numbers

In the weak law of large numbers, we proved convergence in distribution of the average of i.i.d. random variables to the mean. The strong law says more: the convergence occurs with probability 1. 

Theorem (Strong Law of Large Numbers). Let $X _ { 1 } , X _ { 2 } , . . .$ . be $i . i . d .$ with mean µ. Let $S _ { n } =$ $X _ { 1 } + \cdots + X _ { n }$ . Then 

$$
\frac {S _ {n}}{n} \rightarrow \mu \text {almost surely as} n \rightarrow \infty .
$$

## 2.5.1 Proof of the strong law of large numbers (non-examinable)

A proof of the strong law of large numbers in full generality is somewhat involved. A nice proof uses martingales and is part of next year’s course on Probability, Measure and Martingales. 

However, if we assume an extra condition, namely that the distribution has a finite fourth moment, then a relatively straightforward proof is possible. [NB the proof is not examinable.] 

Proof of Strong Law of Large Numbers, under the additional condition E $X _ { n } ^ { 4 } < \infty$ 

Let us centre the $X _ { n } .$ writing $W _ { n } = X _ { n } - \mu .$ 

Then E $W _ { n } = 0$ , and we have E $X _ { n } ^ { 4 } < \infty \Rightarrow \mathbb { E } W _ { n } ^ { 4 } < \infty$ (exercise). 

Note also that 

$$
\begin{array}{c} (\mathbb {E}   W _ {n} ^ {2}) ^ {2} = \mathbb {E}   (W _ {n} ^ {4}) - \mathrm{Var} (W _ {n} ^ {2}) \\ \leq \mathbb {E}   (W _ {n} ^ {4}). \end{array}
$$

We will consider $\mathbb { E } \ \left[ ( S _ { n } - n \mu ) ^ { 4 } \right]$ . Expanding the fourth power and using linearity of expectation, we obtain 

$$
\begin{array}{l}\mathbb{E}\left[(S_{n} - n\mu)^{4}\right] = \mathbb{E}\left[(W_{1} + W_{2} + \dots +W_{n})^{4}\right]\\ = \sum_{1\leq i\leq n}\mathbb{E}W_{i}^{4} + 4\sum_{\substack{1\leq i,j\leq n\\ i\neq j}}\mathbb{E}W_{i}^{3}W_{j} + 3\sum_{\substack{1\leq i,j\leq n\\ i\neq j}}\mathbb{E}W_{i}^{2}W_{j}^{2}\\ \\ +6\sum_{\substack{1\leq i,j,k\leq n\\ i,j,k\text{distinct}}}\mathbb{E}W_{i}^{2}W_{j}W_{k} + \sum_{\substack{1\leq i,j,k,l\leq n\\ i,j,k,l\text{distinct}}}\mathbb{E}W_{i}W_{j}W_{k}W_{l}. \end{array}
$$

(The exact constants in front of the sums are not too important!) Using independence and E $W _ { i } = 0$ , most of these terms vanish. For example, E $W _ { i } ^ { 3 } W _ { j } = \mathbb { E } W _ { i } ^ { 3 } \mathbb { E } W _ { j } = 0$ . We are left 

with only 

$$
\begin{array}{c} \mathbb {E} \left[ (S _ {n} - n \mu) ^ {4} \right] = n \mathbb {E}   W _ {1} ^ {4} + 3 n (n - 1) \left(\mathbb {E} \left[ W _ {1} ^ {2} \right]\right) ^ {2} \\ \leq 3 n ^ {2} \mathbb {E}   W _ {1} ^ {4}. \end{array}
$$

From this we have 

$$
\begin{array}{l} \mathbb {E} \left[ \sum_ {n = 1} ^ {\infty} \left(\frac {S _ {n}}{n} - \mu\right) ^ {4} \right] = \sum_ {n = 1} ^ {\infty} \mathbb {E} \left[ \left(\frac {S _ {n}}{n} - \mu\right) ^ {4} \right] \\ = \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {4}} \mathbb {E} \left[ (S _ {n} - n \mu) ^ {4} \right] \\ \leq \sum_ {n = 1} ^ {\infty} \frac {3 \mathbb {E} W _ {1} ^ {4}}{n ^ {2}} \\ <   \infty . \end{array}
$$

Formally, interchanging the infinite series and expectation in the first line requires a justification refining the notion of absolute convergence to a framework involving general expectations, which is beyond the scope of this course in the present generality. This is not so hard for discrete random variables (changing the order of terms in absolutely convergent series). The theory for such interchanging of series and integrals is developed in next term’s course on Integration and transferred to a general setting of expectations on probability spaces at the very beginning of next year’s course on Probability, Measure and Martingales. 

But if Z is a random variable with E $Z < \infty ,$ then certainly $\mathbb { P } ( Z < \infty ) = 1$ . Applying this with $\begin{array} { r } { Z = \left( \frac { S _ { n } } { n } - \mu \right) ^ { 4 } } \end{array}$ , we get 

$$
\mathbb {P} \left(\sum_ {n = 1} ^ {\infty} \left(\frac {S _ {n}}{n} - \mu\right) ^ {4} <   \infty\right) = 1.
$$

Finally, if $\sum ( a _ { n } - \mu ) ^ { 4 }$ is finite, then certainly $a _ { n } \to \mu$ as $n \to \infty$ . So we can conclude that 

$$
\mathbb {P} \left(\frac {S _ {n}}{n} \rightarrow \mu \text { as } n \rightarrow \infty\right) = 1,
$$

as required. 

## 2.6 Central limit theorem

The weak law of large numbers tells us that the distribution of $S _ { n } / n$ concentrates around $\mu$ as n becomes large. The central limit theorem (CLT) goes much further, telling us that (if the random variables $X _ { i }$ have finite variance) the “fluctuations” of $S _ { n }$ around $n \mu$ are of order $\sqrt { n }$ . Moreover, the behaviour of these fluctuations is universal; whatever the distribution of the $X _ { i } ,$ , if we scale $S _ { n } - n \mu$ by $\sqrt { n }$ , we obtain a normal distribution as the limit as $n \to \infty$ 

Theorem (Central Limit Theorem). Let $X _ { 1 } , X _ { 2 } , \ldots$ be i.i.d. random variables with mean $\mu$ and variance $\sigma ^ { 2 } \in ( 0 , \infty )$ . Let $S _ { n } = X _ { 1 } + X _ { 2 } + \cdot \cdot \cdot + X _ { n }$ . Then 

$$
\frac {S _ {n} - n \mu}{\sigma \sqrt {n}} \xrightarrow {d} N (0, 1) a s n \to \infty .\tag{2.7}
$$

We will prove the CLT later using generating functions. 

Remark 2.7. We can summarise the CLT in three stages: 

(1) The distribution of $S _ { n }$ concentrates around nµ; 

(2) The fluctuations of $S _ { n }$ around nµ are of order ${ \sqrt { n } } ;$ 

(3) The asymptotic distribution of these fluctuations is normal. 

These are somehow in increasing order of refinement. Some students take in the third of these, but not the first two; they remember that the RHS in (2.7) is a normal distribution, but are hazy about what is going on on the LHS. This is a bit perverse; without knowing the scale of the fluctuations, or what they fluctuate around, knowing their distribution is not so useful! 

Example 2.8. An insurance company sells 10, 000 similar car insurance policies. They estimate that the amount paid out in claims on a typical policy has mean £240 and standard deviation £800. Estimate how much they need to put aside in reserves to be 99% sure that the reserve will exceed the total amount claimed. 

Solution: Let $\mu = \mathcal { L } 2 4 0 , \sigma = \mathcal { L } 8 0 0 , n = 1 0 , 0 0 0$ , and note $\Phi ^ { - 1 } ( 0 . 9 9 ) = 2 . 3 2 6$ where Φ is the distribution function of the standard normal. 

Let $S _ { n }$ be the total amount claimed. For large n, the Central Limit Theorem tells us that 

$$
\mathbb {P} \left(\frac {S _ {n} - n \mu}{\sigma \sqrt {n}} <   \Phi^ {- 1} (0. 9 9)\right) \approx 0. 9 9,
$$

i.e. 

$$
\mathbb {P} \left(S _ {n} <   \Phi^ {- 1} (0. 9 9) \sigma \sqrt {n} + n \mu\right) \approx 0. 9 9.
$$

So the amount needed in reserves is approximately $\Phi ^ { - 1 } ( 0 . 9 9 ) \sigma { \sqrt { n } } + n \mu$ , which in this case is £2, 586, 080. 

Notice that the reserve required per customer is about £258, which is £18 higher than µ. We can see from the calculation above that this surplus is proportional to $n ^ { - 1 / 2 }$ . If we had 100 customers rather than 10,000, we would need a surplus 10 times bigger, while with 1,000,000 customers it would be 10 times smaller. 

The fact that the amount per customer needed to cover the fluctuations around the mean is decreasing in the number of customers is an example of risk pooling. 

Of course, the example of identical customers is a bit simplistic, but the efect of risk pooling that we observe is a very real one. Our analysis also assumed that the diferent customers are independent – is that realistic? For car insurance, it is not such a bad assumption. Similarly for life insurance. In the case of property insurance, it could be a very bad assumption (for example, floods can damage many properties simultaneously). In that situation, the efect of risk pooling is a lot smaller (which explains why obtaining insurance for a property subject to a risk of flooding can be problematic, even if the risk is not that great). 

Example 2.9 (Binomial distribution: CLT and Poisson approximation). Let $p \in ( 0 , 1 )$ and let $Y _ { n }$ have Binomial(n, p) distribution. Then we can write $Y _ { n } = X _ { 1 } + \cdots + X _ { n }$ where the 

$X _ { i }$ are i.i.d. Bernoulli(p) random variables. (We can think of the $X _ { i }$ as indicator functions of independent events, all with the same probability, e.g. arising from random sampling). 

The $X _ { i }$ each have mean $p$ and variance $p ( 1 - p )$ . So we can apply the CLT to obtain 

$$
\frac {Y _ {n} - n p}{\sqrt {n}} \xrightarrow {d} N (0, p (1 - p)) \quad \text { as } n \to \infty .
$$

Now instead of considering fixed $p ,$ consider random variables $W _ { n }$ with Binomial $( n , p _ { n } )$ distribution, where $p _ { n } \to 0$ as $n  \infty$ . Now a very diferent limit applies, describing a situation in which we have a very large number of trials but each one has a very small probability of success. Let $\lambda _ { n } = n p _ { n }$ , the mean of $W _ { n }$ . Suppose that $\lambda _ { n }$ converges to a limit $\lambda$ as $n  \infty ,$ , so that the expected total number of successes stays approximately constant. Then we will show that $W _ { n }$ converges in distribution to Poisson(λ). 

It is enough to show (check!) that for each fixed $k = 0 , 1 , \ldots$ 2 

$$
\mathbb {P} (W _ {n} = k) \to \frac {\lambda^ {k}}{k !} e ^ {- \lambda}
$$

(since the RHS is the probability that a Poisson(λ) random variable takes the value k). 

We have 

$$
\begin{array}{l} \mathbb {P} (W _ {n} = k) = \lim \binom {n} {k} p _ {n} ^ {k} (1 - p _ {n}) ^ {n - k} \\ \qquad = \binom {n} {k} \left(\frac {\lambda_ {n}}{n}\right) ^ {k} \left(1 - \frac {\lambda_ {n}}{n}\right) ^ {n - k} \\ \qquad = \frac {n (n - 1) \cdots (n - k + 1)}{n ^ {k}} \frac {\lambda_ {n} ^ {k}}{k !} \left(1 - \frac {\lambda_ {n}}{n}\right) ^ {n} \left(1 - \frac {\lambda_ {n}}{n}\right) ^ {- k} \\ \qquad = 1 \cdot \frac {\lambda^ {k}}{k !} e ^ {- \lambda} \cdot 1 \end{array}
$$

as desired. 