

<!-- === Source: MinerU_markdown_Basics_of_Financial_Mathematics_1_2122707855927779342.md (Page 1) === -->

# The Basics of Financial Mathematics

Spring 2003 

Richard F. Bass 

Department of Mathematics 

University of Connecticut 

These notes are c 2003 by Richard Bass. They may be used for personal use or class use, but not for commercial purposes. If you find any errors, I would appreciate hearing from you: bass@math.uconn.edu 

## 1. Introduction.

In this course we will study mathematical finance. Mathematical finance is not about predicting the price of a stock. What it is about is figuring out the price of options and derivatives. 

The most familiar type of option is the option to buy a stock at a given price at a given time. For example, suppose Microsoft is currently selling today at $40 per share. A European call option is something I can buy that gives me the right to buy a share of Microsoft at some future date. To make up an example, suppose I have an option that allows me to buy a share of Microsoft for $50 in three months time, but does not compel me to do so. If Microsoft happens to be selling at $45 in three months time, the option is worthless. I would be silly to buy a share for $50 when I could call my broker and buy it for $45. So I would choose not to exercise the option. On the other hand, if Microsoft is selling for $60 three months from now, the option would be quite valuable. I could exercise the option and buy a share for $50. I could then turn around and sell the share on the open market for $60 and make a profit of $10 per share. Therefore this stock option I possess has some value. There is some chance it is worthless and some chance that it will lead me to a profit. The basic question is: how much is the option worth today? 

The huge impetus in financial derivatives was the seminal paper of Black and Scholes in 1973. Although many researchers had studied this question, Black and Scholes gave a definitive answer, and a great deal of research has been done since. These are not just academic questions; today the market in financial derivatives is larger than the market in stock securities. In other words, more money is invested in options on stocks than in stocks themselves. 

Options have been around for a long time. The earliest ones were used by manufacturers and food producers to hedge their risk. A farmer might agree to sell a bushel of wheat at a fixed price six months from now rather than take a chance on the vagaries of market prices. Similarly a steel refinery might want to lock in the price of iron ore at a fixed price. 

The sections of these notes can be grouped into five categories. The first is elementary probability. Although someone who has had a course in undergraduate probability will be familiar with some of this, we will talk about a number of topics that are not usually covered in such a course: σ-fields, conditional expectations, martingales. The second category is the binomial asset pricing model. This is just about the simplest model of a stock that one can imagine, and this will provide a case where we can see most of the major ideas of mathematical finance, but in a very simple setting. Then we will turn to advanced probability, that is, ideas such as Brownian motion, stochastic integrals, stochastic diferential equations, Girsanov transformation. Although to do this rigorously requires measure theory, we can still learn enough to understand and work with these concepts. We then return to finance and work with the continuous model. We will derive the Black-Scholes formula, see the Fundamental Theorem of Asset Pricing, work with equivalent martingale measures, and the like. The fifth main category is term structure models, which means models of interest rate behavior. 

I found some unpublished notes of Steve Shreve extremely useful in preparing these notes. I hope that he has turned them into a book and that this book is now available. The stochastic calculus part of these notes is from my own book: Probabilistic Techniques in Analysis, Springer, New York, 1995. 

I would also like to thank Evarist Gin´e who pointed out a number of errors. 

## 2. Review of elementary probability.

Let’s begin by recalling some of the definitions and basic concepts of elementary probability. We will only work with discrete models at first. 

We start with an arbitrary set, called the probability space, which we will denote by $\Omega ,$ the capital Greek letter “omega.” We are given a class $\mathcal { F }$ of subsets of Ω. These are called events. We require $\mathcal { F }$ to be a σ-field. 

Definition 2.1. A collection $\mathcal { F }$ of subsets of Ω is called a σ-field if 

(1) $\varnothing \in { \mathcal { F } } ,$ 

(2) $\Omega \in { \mathcal { F } } ,$ 

(3) $A \in { \mathcal { F } }$ implies $A ^ { c } \in { \mathcal { F } }$ , and 

(4) $A _ { 1 } , A _ { 2 } , \dotsc \in { \mathcal { F } }$ implies both $\cup _ { i = 1 } ^ { \infty } A _ { i } \in { \mathcal { F } }$ and $\cap _ { i = 1 } ^ { \infty } A _ { i } \in { \mathcal { F } }$ 

Here $A ^ { c } = \{ \omega \in \Omega : \omega \notin A \}$ denotes the complement of A. ∅ denotes the empty set, that is, the set with no elements. We will use without special comment the usual notations of ∪ (union), ∩ (intersection), $\subset$ (contained in), $\in$ (is an element of). 

Typically, in an elementary probability course, $\mathcal { F }$ will consist of all subsets of Ω, but we will later need to distinguish between various σ-fields. Here is an example. Suppose one tosses a coin two times and lets Ω denote all possible outcomes. So $\Omega = \{ H H , H T , T H , T T \}$ . A typical σ-field $\mathcal { F }$ would be the collection of all subsets of Ω. In this case it is trivial to show that $\mathcal { F }$ is a σ-field, since every subset is in ${ \mathcal F } .$ . But if we let $\mathcal { G } = \{ \emptyset , \Omega , \{ H H , H T \} , \{ T H , T T \} \}$ , then $\mathcal { G }$ is also a σ-field. One has to check the definition, but to illustrate, the event {HH, HT} is in ${ \mathcal { G } } .$ so we require the complement of that set to be in $\mathcal { G }$ as well. But the complement is $\{ T H , T T \}$ and that event is indeed in ${ \mathcal { G } } .$ 

One point of view which we will explore much more fully later on is that the σ-field tells you what events you “know.” In this example, $\mathcal { F }$ is the σ-field where you “know” everything, while $\mathcal { G }$ is the σ-field where you “know” only the result of the first toss but not the second. We won’t try to be precise here, but to try to add to the intuition, suppose one knows whether an event in $\mathcal { F }$ has happened or not for a particular outcome. We would then know which of the events {HH}, {HT}, {TH}, or {TT} has happened and so would know what the two tosses of the coin showed. On the other hand, if we know which events in $\mathcal { G }$ happened, we would only know whether the event $\{ H H , H T \}$ happened, which means we would know that the first toss was a heads, or we would know whether the event {TH, TT} happened, in which case we would know that the first toss was a tails. But there is no way to tell what happened on the second toss from knowing which events in $\mathcal { G }$ happened. Much more on this later. 

The third basic ingredient is a probability. 

Definition 2.2. A function P on $\mathcal { F }$ is a probability if it satisfies 

(1) if $A \in { \mathcal { F } } _ { \mathrm { : } }$ , then $0 \leq \mathbb { P } ( A ) \leq 1$ 

(2) $\mathbb { P } ( \Omega ) = 1$ , and 

(3) $\mathbb { P } ( \varnothing ) = 0 _ { ; }$ , and 

(4) if $A _ { 1 } , A _ { 2 } , \dotsc \in { \mathcal { F } }$ are pairwise disjoint, then $\begin{array} { r } { \mathbb { P } \big ( \cup _ { i = 1 } ^ { \infty } A _ { i } \big ) = \sum _ { i = 1 } ^ { \infty } \mathbb { P } \big ( A _ { i } \big ) } \end{array}$ 

A collection of sets $A _ { i }$ is pairwise disjoint if $A _ { i } \cap A _ { j } = \varnothing$ unless $i = j$ 

There are a number of conclusions one can draw from this definition. As one example, if $A \subset B$ , then $\mathbb { P } ( A ) \le \mathbb { P } ( B )$ and $\mathbb { P } ( A ^ { c } ) = 1 - \mathbb { P } ( A )$ . See Note 1 at the end of this section for a proof. 

Someone who has had measure theory will realize that a σ-field is the same thing as a σ-algebra and a probability is a measure of total mass one. 

A random variable (abbreviated $\mathrm { r . v . ) }$ is a function X from Ω to R, the reals. To be more precise, to be a r.v. X must also be measurable, which means that $\{ \omega : X ( \omega ) \geq$ $a \} \in { \mathcal { F } }$ for all reals $a .$ 

The notion of measurability has a simple definition but is a bit subtle. If we take the point of view that we know all the events in ${ \mathcal { G } } ,$ then if $Y$ is G-measurable, then we know Y. Phrased another way, suppose we know whether or not the event has occurred for each event in ${ \mathcal { G } } .$ . Then if $Y$ is $\mathcal { G }$ -measurable, we can compute the value of $Y$ 

Here is an example. In the example above where we tossed a coin two times, let X be the number of heads in the two tosses. Then X is $\mathcal { F }$ measurable but not $\mathcal { G }$ measurable. To see this, let us consider $A _ { a } = \{ \omega \in \Omega : X ( \omega ) \geq a \}$ . This event will equal 

$$
\left\{ \begin{array}{l l} \Omega & \text {if a\leq 0 ;} \\ \{H H, H T, T H \} & \text {if 0 <   a\leq 1 ;} \\ \{H H \} & \text {if 1 <   a\leq 2 ;} \\ \emptyset & \text {if 2 <   a .} \end{array} \right.
$$

For example, if $\begin{array} { r } { a = \frac { 3 } { 2 } . } \end{array}$ , then the event where the number of heads is $\frac { 3 } { 2 }$ or greater is the event where we had two heads, namely, {HH}. Now observe that for each a the event $A _ { a }$ is in $\mathcal { F }$ because $\mathcal { F }$ contains all subsets of Ω. Therefore X is measurable with respect to $\mathcal { F }$ However it is not true that $A _ { a }$ is in $\mathcal { G }$ for every value of a – take $\textstyle a = { \frac { 3 } { 2 } }$ as just one example – the subset {HH} is not in G. So X is not measurable with respect to the σ-field $\mathcal { G } .$ 

A discrete r.v. is one where $\mathbb { P } ( \omega : X ( \omega ) = a ) = 0$ for all but countably many $a \mathrm { \ ' } \mathrm { s } .$ say, $a _ { 1 } , a _ { 2 } , \dotsc ,$ and $\begin{array} { r } { \sum _ { i } \mathbb { P } ( \omega : X ( \omega ) = a _ { i } ) = 1 } \end{array}$ . In defining sets one usually omits the ω; thus $( X = x )$ means the same as $\{ \omega : X ( \omega ) = x \}$ 

In the discrete case, to check measurability with respect to a σ-field ${ \mathcal { F } } _ { : }$ it is enough that $( X = a ) \in { \mathcal { F } }$ for all reals a. The reason for this is that if $x _ { 1 } , x _ { 2 } , \dotsc .$ . are the values of x for which $\mathbb { P } ( X = x ) \neq 0$ , then we can write $( X \geq a ) = \cup _ { x _ { i } \geq a } ( X = x _ { i } )$ and we have a countable union. So if $( X = x _ { i } ) \in \mathcal { F }$ , then $( X \geq a ) \in { \mathcal { F } }$ 

Given a discrete r.v. X, the expectation or mean is defined by 

$$
\mathbb {E} X = \sum_ {x} x \mathbb {P} (X = x)
$$

provided the sum converges. If X only takes finitely many values, then this is a finite sum and of course it will converge. This is the situation that we will consider for quite some time. However, if X can take an infinite number of values (but countable), convergence needs to be checked. For example, if $\mathbb { P } ( X = 2 ^ { n } ) = 2 ^ { - n } { \mathrm { ~ f o r ~ } } n = 1 , 2 , . . . ,$ , then $\mathbb { E } X =$ $\textstyle \sum _ { n = 1 } ^ { \infty } 2 ^ { n } \cdot 2 ^ { - n } = \infty$ 

There is an alternate definition of expectation which is equivalent in the discrete setting. Set 

$$
\mathbb {E} X = \sum_ {\omega \in \Omega} X (\omega) \mathbb {P} (\{\omega \}).
$$

To see that this is the same, look at Note 2 at the end of the section. The advantage of the second definition is that some properties of expectation, such as $\mathbb { E } \left( X + Y \right) = \mathbb { E } X + \mathbb { E } Y$ are immediate, while with the first definition they require quite a bit of proof. 

We say two events A and B are independent i ${ \dot { \mathbb { P } } } ( A \cap B ) = \mathbb { P } ( A ) \mathbb { P } ( B )$ . Two random variables X and Y are independent if $\mathbb { P } ( X \in A , Y \in B ) = \mathbb { P } ( X \in A ) \mathbb { P } ( X \in B )$ for all A and B that are subsets of the reals. The comma in the expression $\mathbb { P } ( X \in A , Y \in B )$ means “and.” Thus 

$$
\mathbb {P} (X \in A, Y \in B) = \mathbb {P} ((X \in A) \cap (Y \in B)).
$$

The extension of the definition of independence to the case of more than two events or random variables is not surprising: $A _ { 1 } , \ldots , A _ { r }$ are independent if 

$$
\mathbb {P} (A _ {i _ {1}} \cap \dots \cap A _ {i _ {j}}) = \mathbb {P} (A _ {i _ {1}}) \dots \mathbb {P} (A _ {i _ {j}})
$$

whenever $\{ i _ { 1 } , \dotsc , i _ { j } \}$ is a subset of $\{ 1 , \ldots , n \}$ 

A common misconception is that an event is independent of itself. If A is an event that is independent of itself, then 

$$
\mathbb {P} (A) = \mathbb {P} (A \cap A) = \mathbb {P} (A) \mathbb {P} (A) = (\mathbb {P} (A)) ^ {2}.
$$

The only finite solutions to the equation $x = x ^ { 2 }$ are $x = 0$ and $x = 1$ , so an event is independent of itself only if it has probability 0 or 1. 

Two σ-fields F and $\mathcal { G }$ are independent if A and B are independent whenever $A \in { \mathcal { F } }$ and $B \in { \mathcal { G } }$ . A r.v. X and a σ-field $\mathcal { G }$ are independent ${ \mathrm { i f ~ } } \mathbb { P } ( ( X \in A ) \cap B ) = \mathbb { P } ( X \in A ) \mathbb { P } ( B )$ whenever A is a subset of the reals and $B \in { \mathcal { G } }$ 

As an example, suppose we toss a coin two times and we define the σ-fields $\mathcal { G } _ { 1 } =$ $\{ \emptyset , \Omega , \{ H H , H T \} , \{ T H , T T \} \}$ and $\mathcal { G } _ { 2 } = \{ \varnothing , \Omega , \{ H H , T H \} , \{ H T , T T \} \}$ . Then $\mathcal { G } _ { 1 }$ and $\mathcal { G } _ { 2 }$ are independent if $\begin{array} { r } { \mathbb { P } ( H H ) = \mathbb { P } ( H T ) = \mathbb { P } ( T H ) = \mathbb { P } ( T T ) = \frac { 1 } { 4 } \boldsymbol { \cdot } } \end{array}$ . (Here we are writing $\mathbb { P } ( H H )$ when a more accurate way would be to write $\mathbb { P } ( \{ H H \} ) . )$ An easy way to understand this is that if we look at an event in $\mathcal { G } _ { 1 }$ that is not ∅ or Ω, then that is the event that the first toss is a heads or it is the event that the first toss is a tails. Similarly, a set other than ∅ or Ω in $\mathcal { G } _ { 2 }$ will be the event that the second toss is a heads or that the second toss is a tails. 

If two r.v.s X and Y are independent, we have the multiplication theorem, which says that E $( X Y ) = ( \mathbb { E } X ) ( \mathbb { E } Y )$ provided all the expectations are finite. See Note 3 for a proof. 

Suppose $X _ { 1 } , \ldots , X _ { n }$ are n independent r.v.s, such that for each one $\mathbb { P } ( X _ { i } = 1 ) = p .$ $\mathbb { P } ( X _ { i } = 0 ) = 1 - p ,$ where $p \in [ 0 , 1 ]$ ]. The random variable $\begin{array} { r } { S _ { n } \ = \ \sum _ { i = 1 } ^ { n } X _ { i } } \end{array}$ is called a binomial r.v., and represents, for example, the number of successes in n trials, where the probability of a success is $p .$ An important result in probability is that 

$$
\mathbb {P} (S _ {n} = k) = \frac {n !}{k ! (n - k) !} p ^ {k} (1 - p) ^ {n - k}.
$$

The variance of a random variable is 

$$
\operatorname{Var} X = \mathbb {E} \left[ (X - \mathbb {E} X) ^ {2} \right].
$$

This is also equal to 

$$
\mathbb {E} \left[ X ^ {2} \right] - (\mathbb {E} X) ^ {2}.
$$

It is an easy consequence of the multiplication theorem that if X and Y are independent, 

$$
\operatorname{Var} (X + Y) = \operatorname{Var} X + \operatorname{Var} Y.
$$

The expression E $[ X ^ { 2 } ]$ is sometimes called the second moment of $X$ . 

We close this section with a definition of conditional probability. The probability of A given B, written $\mathbb { P } ( A \mid B )$ is defined by 

$$
\frac {\mathbb {P} (A \cap B)}{\mathbb {P} (B)},
$$

provided $\mathbb { P } ( B ) \neq 0$ . The conditional expectation of X given B is defined to be 

$$
\frac {\mathbb {E} \left[ X ; B \right]}{\mathbb {P} (B)},
$$

provided $\mathbb { P } ( B ) \neq 0$ . The notation $\mathbb { E } \left[ X ; B \right]$ means $\mathbb { E } \left[ X 1 _ { B } \right]$ , where $1 _ { B } ( \omega )$ is 1 if $\omega \in B$ and 0 otherwise. Another way of writing $\mathbb { E } \left[ X ; B \right]$ is 

$$
\mathbb {E} \left[ X; B \right] = \sum_ {\omega \in B} X (\omega) \mathbb {P} (\{\omega \}).
$$

(We will use the notation $\mathbb { E } \left[ X ; B \right]$ frequently.) 

Note 1. Suppose we have two disjoint sets C and D. Let $A _ { 1 } = C , A _ { 2 } = D$ , and $A _ { i } = \emptyset$ for $i \geq 3$ . Then the $A _ { i }$ are pairwise disjoint and 

$$
\mathbb {P} (C \cup D) = \mathbb {P} (\cup_ {i = 1} ^ {\infty} A _ {i}) = \sum_ {i = 1} ^ {\infty} \mathbb {P} (A _ {i}) = \mathbb {P} (C) + \mathbb {P} (D)\tag{2.1}
$$

by Definition $2 . 2 ( 3 )$ and (4). Therefore Definition $2 . 2 ( 4 )$ holds when there are only two sets instead of infinitely many, and a similar argument shows the same is true when there are an arbitrary (but finite) number of sets. 

Now suppose $A \subset B$ . Let $C = A$ and $D = B - A$ , where $B - A$ is defined to be $B \cap A ^ { c }$ (this is frequently written $B \setminus A$ as well). Then $C$ and $D$ are disjoint, and by (2.1) 

$$
\mathbb {P} (B) = \mathbb {P} (C \cup D) = \mathbb {P} (C) + \mathbb {P} (D) \geq \mathbb {P} (C) = \mathbb {P} (A).
$$

The other equality we mentioned is proved by letting $C = A$ and $D = A ^ { c }$ . Then $C$ and $D$ are disjoint, and 

$$
1 = \mathbb {P} (\Omega) = \mathbb {P} (C \cup D) = \mathbb {P} (C) + \mathbb {P} (D) = \mathbb {P} (A) + \mathbb {P} (A ^ {c}).
$$

Solving for $\mathbb { P } ( A ^ { c } )$ , we have 

$$
\mathbb {P} (A ^ {c}) = 1 - \mathbb {P} (A).
$$

Note 2. Let us show the two definitions of expectation are the same (in the discrete case). Starting with the first definition we have 

$$
\begin{array}{l} \mathbb {E}   X = \sum_ {x} x \mathbb {P} (X = x) \\ \qquad = \sum_ {x} x \sum_ {\{\omega \in \Omega : X (\omega) = x \}} \mathbb {P} (\{\omega \}) \\ \qquad = \sum_ {x} \sum_ {\{\omega \in \Omega : X (\omega) = x \}} X (\omega) \mathbb {P} (\{\omega \}) \\ \qquad = \sum_ {\omega \in \Omega} X (\omega) \mathbb {P} (\{\omega \}), \end{array}
$$

and we end up with the second definition. 

Note 3. Suppose X can takes the values $x _ { 1 } , x _ { 2 } , . . .$ . and Y can take the values $y _ { 1 } , y _ { 2 } , \ldots$ Let $A _ { i } = \{ \omega : X ( \omega ) = x _ { i } \}$ and $B _ { j } = \{ \omega : Y ( \omega ) = y _ { j } \}$ . Then 

$$
X = \sum_ {i} x _ {i} 1 _ {A _ {i}}, \quad Y = \sum_ {j} y _ {j} 1 _ {B _ {j}},
$$

and so 

$$
X Y = \sum_ {i} \sum_ {j} x _ {i} y _ {i} 1 _ {A _ {i}} 1 _ {B _ {j}}.
$$

Since $1 _ { A _ { i } } 1 _ { B _ { j } } = 1 _ { A _ { i } \cap B _ { j } }$ , it follows that 

$$
\mathbb {E} \left[ X Y \right] = \sum_ {i} \sum_ {j} x _ {i} y _ {j} \mathbb {P} (A _ {i} \cap B _ {j}),
$$

$$
\begin{array}{l} \mathbb {E} [ X Y ] = \sum_ {i} \sum_ {j} x _ {i} y _ {j} \mathbb {P} (A _ {i}) \mathbb {P} (B _ {j}) \\ \qquad = \sum_ {i} x _ {i} \mathbb {P} (A _ {i}) \Big [ \sum_ {j} y _ {j} \mathbb {P} (B _ {j}) \Big ] \\ \qquad = \sum_ {i} x _ {i} \mathbb {P} (A _ {i}) \mathbb {E} Y \\ \qquad = (\mathbb {E} X) (\mathbb {E} Y). \end{array}
$$

assuming the double sum converges. Since X and Y are independent, $A _ { i } = \left( X = x _ { i } \right)$ is independent of $B _ { j } = ( Y = y _ { j } )$ and so 

## 3. Conditional expectation.

Suppose we have 200 men and 100 women, 70 of the men are smokers, and 50 of the women are smokers. If a person is chosen at random, then the conditional probability that the person is a smoker given that it is a man is 70 divided by 200, or 35%, while the conditional probability the person is a smoker given that it is a women is 50 divided by 100, or 50%. We will want to be able to encompass both facts in a single entity. 

The way to do that is to make conditional probability a random variable rather than a number. To reiterate, we will make conditional probabilities random. Let $M , W$ be man, woman, respectively, and $S , S ^ { c }$ smoker and nonsmoker, respectively. We have 

$$
\mathbb {P} (S \mid M) = . 3 5, \qquad \mathbb {P} (S \mid W) = . 5 0.
$$

We introduce the random variable 

$$
(. 3 5) 1 _ {M} + (. 5 0) 1 _ {W}
$$

and use that for our conditional probability. So on the set M its value is .35 and on the set W its value is .50. 

We need to give this random variable a name, so what we do is let $\mathcal { G }$ be the $\sigma \cdot$ -field consisting of $\{ \emptyset , \Omega , M , W \}$ and denote this random variable $\mathbb { P } ( S \mid \mathcal { G } )$ . Thus we are going to talk about the conditional probability of an event given a σ-field. 

## What is the precise definition?

Definition 3.1. Suppose there exist finitely (or countably) many sets $B _ { 1 } , B _ { 2 } , . . . ,$ all having positive probability, such that they are pairwise disjoint, Ω is equal to their union, and $\mathcal { G }$ is the σ-field one obtains by taking all finite or countable unions of the $B _ { i }$ . Then the conditional probability of A given $\mathcal { G }$ is 

$$
\mathbb {P} (A \mid \mathcal {G}) = \sum_ {i} \frac {\mathbb {P} (A \cap B _ {i})}{\mathbb {P} (B _ {i})} 1 _ {B _ {i}} (\omega).
$$

In short, on the set $B _ { i }$ the conditional probability is equal to $\mathbb { P } ( A \mid B _ { i } )$ 

Not every σ-field can be so represented, so this definition will need to be extended when we get to continuous models. σ-fields that can be represented as in Definition 3.B are called finitely (or countably) generated and are said to be generated by the sets $B _ { 1 } , B _ { 2 } , \ldots$ 

Let’s look at another example. Suppose Ω consists of the possible results when we toss a coin three times: HHH, HHT, etc. Let $\mathcal { F } _ { 3 }$ denote all subsets of Ω. Let $\mathcal { F } _ { 1 }$ consist of the sets ∅, Ω, {HHH, HHT, HTH, HTT}, and $\{ T H H , T H T , T T H , T T T \}$ . So $\mathcal { F } _ { 1 }$ consists of those events that can be determined by knowing the result of the first toss. We want to let $\mathcal { F } _ { 2 }$ denote those events that can be determined by knowing the first two tosses. This will include the sets $\emptyset , \Omega , \{ H H H , H H T \} , \{ H T H , H T T \} , \{ T H H , T H T \} , \{ T T H , T T T \}$ . This is not enough to make $\mathcal { F } _ { \mathrm { 2 } } \mathrm { ~ a ~ } \sigma { \mathrm { - f i e l d } }$ , so we add to $\mathcal { F } _ { 2 }$ all sets that can be obtained by taking unions of these sets. 

Suppose we tossed the coin independently and suppose that it was fair. Let us calculate $\mathbb { P } ( A \mid \mathcal { F } _ { 1 } ) , \mathbb { P } ( A \mid \mathcal { F } _ { 2 } )$ , and $\mathbb { P } ( A \mid { \mathcal F } _ { 3 } )$ when A is the event $\{ H H H \}$ . First the conditional probability given $\mathcal { F } _ { 1 }$ . Let $C _ { 1 } = \{ H H H , H H T , H T H , H T T \}$ and $C _ { 2 } =$ $\{ T H H , T H T , T T H , T T T \}$ . On the set $C _ { 1 }$ the conditional probability is $\mathbb { P } ( A \cap C _ { 1 } ) / \mathbb { P } ( C _ { 1 } ) =$ $\begin{array} { r } { \mathbb { P } ( H H H ) / \mathbb { P } ( C _ { 1 } ) = \frac { 1 } { 8 } / \frac { 1 } { 2 } = \frac { 1 } { 4 } } \end{array}$ . On the set $C _ { 2 }$ the conditional probability is ${ \mathbb { P } } ( A \cap C _ { 2 } ) / { \mathbb { P } } ( C _ { 2 } )$ $= \mathbb { P } ( \varnothing ) / \mathbb { P } ( C _ { 2 } ) = 0$ . Therefore $\mathbb { P } ( A \mid { \mathcal { F } } _ { 1 } ) = ( . 2 5 ) 1 _ { C _ { 1 } }$ . This is plausible – the probability of getting three heads given the first toss is $\textstyle { \frac { 1 } { 4 } }$ if the first toss is a heads and 0 otherwise. 

Next let us calculate $\mathbb { P } ( A \mid \mathcal { F } _ { 2 } )$ . Let $D _ { 1 } = \{ H H H , H H T \} , D _ { 2 } = \{ H T H , H T T \} , D _ { 3 }$ $= \{ T H H , T H T \} , D _ { 4 } = \{ T T H , T T T \}$ . So $\mathcal { F } _ { 2 }$ is the σ-field consisting of all possible unions of some of the $\begin{array} { r } { D _ { i } \mathrm { ' s . ~ } \mathbb { P } ( A \mid D _ { 1 } ) = \mathbb { P } ( H H H ) / \mathbb { P } ( D _ { 1 } ) = \frac { 1 } { 8 } / \frac { 1 } { 4 } = \frac { 1 } { 2 } } \end{array}$ . Also, as above, $\mathbb { P } ( A \mid$ $D _ { i } ) = 0$ for $i = 2 , 3 , 4$ . So $\mathbb { P } ( A \mid { \mathcal { F } } _ { 2 } ) = ( . 5 0 ) 1 _ { D _ { 1 } }$ . This is again plausible – the probability of getting three heads given the first two tosses is $\frac { 1 } { 2 }$ if the first two tosses were heads and 0 otherwise. 

What about conditional expectation? Recall $\mathbb { E } \left[ X ; B _ { i } \right] = \mathbb { E } \left[ X 1 _ { B _ { i } } \right]$ and also that $\mathbb { E } \left[ 1 _ { B } \right] = 1 \cdot \mathbb { P } ( 1 _ { B } = 1 ) + 0 \cdot \mathbb { P } ( 1 _ { B } = 0 ) = \mathbb { P } ( B )$ . Given a random variable $X$ , we define 

$$
\mathbb {E} \left[ X \mid \mathcal {G} \right] = \sum_ {i} \frac {\mathbb {E} \left[ X ; B _ {i} \right]}{\mathbb {P} (B _ {i})} 1 _ {B _ {i}}.
$$

This is the obvious definition, and it agrees with what we had before because $\mathbb { E } \left[ 1 _ { A } \ | \ \mathcal { G } \right]$ should be equal to $\mathbb { P } ( A \mid { \mathcal { G } } )$ 

We now turn to some properties of conditional expectation. Some of the following propositions may seem a bit technical. In fact, they are! However, these properties are crucial to what follows and there is no choice but to master them. 

Proposition 3.2. $\mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ is $\mathcal { G }$ measurable, that is, $i f Y = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ , then $( Y > a )$ is a set in $\mathcal { G }$ for each real $a .$ . 

Proof. By the definition, 

$$
Y = \mathbb {E} [ X \mid \mathcal {G} ] = \sum_ {i} \frac {\mathbb {E} [ X ; B _ {i} ]}{\mathbb {P} (B _ {i})} 1 _ {B _ {i}} = \sum_ {i} b _ {i} 1 _ {B _ {i}}
$$

if we set $b _ { i } = \mathbb { E } \left[ X ; B _ { i } \right] / \mathbb { P } ( B _ { i } )$ . The set $( Y \geq a )$ is a union of some of the $B _ { i }$ , namely, those $B _ { i }$ for which $b _ { i } \geq a$ . But the union of any collection of the $B _ { i }$ is in $\mathcal { G }$ . □ 

An example might help. Suppose 

$$
Y = 2 \cdot 1 _ {B _ {1}} + 3 \cdot 1 _ {B _ {2}} + 6 \cdot 1 _ {B _ {3}} + 4 \cdot 1 _ {B _ {4}}
$$

and $a = 3 . 5$ . Then $( Y \geq a ) = B _ { 3 } \cup B _ { 4 }$ , which is in $\mathcal { G }$ . 

Proposition 3.3. If $C \in { \mathcal { G } }$ and $Y = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ , then $\mathbb { E } \left[ Y ; C \right] = \mathbb { E } \left[ X ; C \right]$ 

Proof. Since $\begin{array} { r } { Y = \sum \frac { \mathbb { E } [ X ; B _ { i } ] } { \mathbb { P } ( B _ { i } ) } 1 _ { B _ { i } } } \end{array}$ and the $B _ { i }$ are disjoint, then 

$$
\mathbb {E} \left[ Y; B _ {j} \right] = \frac {\mathbb {E} \left[ X ; B _ {j} \right]}{\mathbb {P} (B _ {j})} \mathbb {E} 1 _ {B _ {j}} = \mathbb {E} \left[ X; B _ {j} \right].
$$

Now if $C = B _ { j _ { 1 } } \cup \dots \cup B _ { j _ { n } } \cup \dots .$ , summing the above over the $j _ { k }$ gives $\mathbb { E } \left[ Y ; C \right] = \mathbb { E } \left[ X ; C \right]$ $\boxed { \begin{array} { r l } \end{array} }$ 

Let us look at the above example for this proposition, and let us do the case where $C = B _ { 2 }$ . Note $1 _ { B _ { 2 } } 1 _ { B _ { 2 } } = 1 _ { B _ { 2 } }$ because the product is $1 \cdot 1 = 1 { \mathrm { ~ i f ~ } } \omega$ is in $B _ { 2 }$ and 0 otherwise. On the other hand, it is not possible for an ω to be in more than one of the $B _ { i } .$ , so $1 _ { B _ { 2 } } 1 _ { B _ { i } } = 0 \mathrm { i f } i \neq 2$ . Multiplying $Y$ in the above example by $1 _ { B _ { 2 } }$ , we see that 

$$
\begin{array}{c} \mathbb {E} \left[ Y; C \right] = \mathbb {E} \left[ Y; B _ {2} \right] = \mathbb {E} \left[ Y 1 _ {B _ {2}} \right] = \mathbb {E} \left[ 3 \cdot 1 _ {B _ {2}} \right] \\ = 3 \mathbb {E} \left[ 1 _ {B _ {2}} \right] = 3 \mathbb {P} (B _ {2}). \end{array}
$$

However the number 3 is not just any number; it is $\mathbb { E } \left[ X ; B _ { 2 } \right] / \mathbb { P } ( B _ { 2 } )$ . So 

$$
3 \mathbb {P} (B _ {2}) = \frac {\mathbb {E} [ X ; B _ {2} ]}{\mathbb {P} (B _ {2})} \mathbb {P} (B _ {2}) = \mathbb {E} [ X; B _ {2} ] = \mathbb {E} [ X; C ],
$$

just as we wanted. If $C = B _ { 1 } \cup B _ { 4 }$ , for example, we then write 

$$
\begin{array}{r l} & {\mathbb {E} [ X; C ] = \mathbb {E} [ X 1 _ {C} ] = \mathbb {E} [ X (1 _ {B _ {2}} + 1 _ {B _ {4}}) ]} \\ & {\qquad = \mathbb {E} [ X 1 _ {B _ {2}} ] + \mathbb {E} [ X 1 _ {B _ {4}} ] = \mathbb {E} [ X; B _ {2} ] + \mathbb {E} [ X; B _ {4} ].} \end{array}
$$

By the first part, this equals E $[ Y ; B _ { 2 } ] + \mathbb { E } \left[ Y ; B _ { 4 } \right]$ , and we undo the above string of equalities but with Y instead of X to see that this is $\mathbb { E } \left[ Y ; C \right]$ 

If a r.v. Y is $\mathcal { G }$ measurable, then for any a we have $( Y = a ) \in \mathcal { G }$ which means that $( Y = a )$ is the union of one or more of the $B _ { i }$ . Since the $B _ { i }$ are disjoint, it follows that $Y$ must be constant on each $B _ { i }$ 

Again let us look at an example. Suppose Z takes only the values 1, 3, 4, 7. Let $D _ { 1 } = ( Z = 1 ) , D _ { 2 } = ( Z = 3 ) , D _ { 3 } = ( Z = 4 ) , D _ { 4 } = ( Z = 7 )$ . Note that we can write 

$$
Z = 1 \cdot 1 _ {D _ {1}} + 3 \cdot 1 _ {D _ {2}} + 4 \cdot 1 _ {D _ {3}} + 7 \cdot 1 _ {D _ {4}}.
$$

To see this, if $\omega \in D _ { 2 }$ , for example, the right hand side will be $0 + 3 \cdot 1 + 0 + 0$ , which agrees with $Z ( \omega )$ . Now if Z is $\mathcal { G }$ measurable, then $( Z \geq a ) \in { \mathcal { G } }$ for each a. Take $a = 7$ , and we see ${ \cal D } _ { 4 } \in \mathcal G$ . Take $a = 4$ and we see $D _ { 3 } \cup D _ { 4 } \in { \mathcal { G } }$ . Taking $a = 3$ shows $D _ { 2 } \cup D _ { 3 } \cup D _ { 4 } \in \mathcal { G }$ 

Now $D _ { 3 } = ( D _ { 3 } \cup D _ { 4 } ) \cap D _ { 4 } ^ { c }$ , so since $\mathcal { G }$ is a σ-field, $D _ { 3 } \in { \mathcal { G } }$ . Similarly $D _ { 2 } , D _ { 1 } \in { \mathcal { G } }$ . Because sets in $\mathcal { G }$ are unions of the $B _ { i } { } ^ { \ ' } \mathrm { s } .$ we must have $Z$ constant on the $B _ { i } \mathrm { ^ { 8 } s }$ . For example, if it so happened that $D _ { 1 } = B _ { 1 } , D _ { 2 } = B _ { 2 } \cup B _ { 4 } , D _ { 3 } = B _ { 3 } \cup B _ { 6 } \cup B _ { 7 } .$ , and $D _ { 4 } = B _ { 5 } ,$ , then 

$$
Z = 1 \cdot 1 _ {B _ {1}} + 3 \cdot 1 _ {B _ {2}} + 4 \cdot 1 _ {B _ {3}} + 3 \cdot 1 _ {B _ {4}} + 7 \cdot 1 _ {B _ {5}} + + 4 \cdot 1 _ {B _ {6}} + 4 \cdot 1 _ {B _ {7}}.
$$

We still restrict ourselves to the discrete case. In this context, the properties given in Propositions 3.2 and 3.3 uniquely determine E [X | G]. 

Proposition 3.4. Suppose $Z$ is $\mathcal { G }$ measurable and $\mathbb { E } \left[ Z ; C \right] = \mathbb { E } \left[ X ; C \right]$ whenever $C \in { \mathcal { G } }$ Then $Z = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ 

Proof. Since $Z$ is $\mathcal { G }$ measurable, then $Z$ must be constant on each $B _ { i }$ . Let the value of $Z$ on $B _ { i }$ be $z _ { i }$ . So $\begin{array} { r } { Z = \sum _ { i } z _ { i } 1 _ { B _ { i } } } \end{array}$ . Then 

$$
z _ {i} \mathbb {P} (B _ {i}) = \mathbb {E} [ Z; B _ {i} ] = \mathbb {E} [ X; B _ {i} ],
$$

or $z _ { i } = \mathbb { E } \left[ X ; B _ { i } \right] / \mathbb { P } ( B _ { i } )$ as required. 

The following propositions contain the main facts about this new definition of conditional expectation that we will need. 

Proposition 3.5. (1) $I f X _ { 1 } \geq X _ { 2 }$ , then $\mathbb { E } \left[ X _ { 1 } \mid { \mathcal { G } } \right] \geq \mathbb { E } \left[ X _ { 2 } \mid { \mathcal { G } } \right]$ 

(2) ${ \mathfrak { T } } \left[ a X _ { 1 } + b X _ { 2 } \mid { \mathcal { G } } \right] = a \mathbb { E } \left[ X _ { 1 } \mid { \mathcal { G } } \right] + b \mathbb { E } \left[ X _ { 2 } \mid { \mathcal { G } } \right]$ 

(3) If X is G measurable, then $\mathbb { E } \left[ X \mid { \mathcal { G } } \right] = X$ 

(4) $\mathbb { E } \left[ \mathbb { E } \left[ X \mid { \mathcal { G } } \right] \right] = \mathbb { E } X$ 

(5) If X is independent of ${ \mathcal { G } } ,$ then E $[ X \mid { \mathcal { G } } ] = \mathbb { E } X$ 

We will prove Proposition 3.5 in Note 1 at the end of the section. At this point it is more fruitful to understand what the proposition says. 

We will see in Proposition 3.8 below that we may think of $\mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ as the best prediction of X given G. Accepting this for the moment, we can give an interpretation of (1)-(5). (1) says that if $X _ { 1 }$ is larger than $X _ { 2 }$ , then the predicted value of $X _ { 1 }$ should be larger than the predicted value of $X _ { 2 }$ . (2) says that the predicted value of $X _ { 1 } + X _ { 2 }$ should be the sum of the predicted values. (3) says that if we know $\mathcal { G }$ and X is $\mathcal { G }$ measurable, then we know X and our best prediction of X is X itself. (4) says that the average of the predicted value of X should be the average value of X. (5) says that if knowing $\mathcal { G }$ gives us no additional information on X, then the best prediction for the value of X is just E X. 

Proposition 3.6. If Z is $\mathcal { G }$ measurable, then $\mathbb { E } \left[ X Z \mid { \mathcal { G } } \right] = Z \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ 

We again defer the proof, this time to Note 2. 

Proposition 3.6 says that as far as conditional expectations with respect to a $\sigma -$ field G go, G-measurable random variables act like constants: they can be taken inside or outside the conditional expectation at will. 

Proposition 3.7. $I f { \mathcal { H } } \subset { \mathcal { G } } \subset { \mathcal { F } }$ , then 

$$
\mathbb {E} \left[ \mathbb {E} \left[ X \mid \mathcal {H} \right] \mid \mathcal {G} \right] = \mathbb {E} \left[ X \mid \mathcal {H} \right] = \mathbb {E} \left[ \mathbb {E} \left[ X \mid \mathcal {G} \right] \mid \mathcal {H} \right].
$$

Proof. $\mathbb { E } \left[ X \ | \ \mathcal { H } \right]$ is H measurable, hence $\mathcal { G }$ measurable, since $\mathcal { H } \subset \mathcal { G }$ . The left hand equality now follows by Proposition 3.5(3). To get the right hand equality, let W be the right hand expression. It is H measurable, and if $C \in { \mathcal { H } } \subset { \mathcal { G } }$ , then 

$$
\mathbb {E} \left[ W; C \right] = \mathbb {E} \left[ \mathbb {E} \left[ X \mid \mathcal {G} \right]; C \right] = \mathbb {E} \left[ X; C \right]
$$

as required. 

In words, if we are predicting a prediction of X given limited information, this is the same as a single prediction given the least amount of information. 

Let us verify that conditional expectation may be viewed as the best predictor of a random variable given a σ-field. If X is a r.v., a predictor Z is just another random variable, and the goodness of the prediction will be measured by E $[ ( X - Z ) ^ { 2 } ]$ , which is known as the mean square error. 

Proposition 3.8. If X is a r.v., the best predictor among the collection of ${ \mathcal { G } } .$ -measurable random variables is $Y = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ 

Proof. Let Z be any G-measurable random variable. We compute, using Proposition 3.5(3) and Proposition 3.6, 

$$
\begin{array}{r l} & {\mathbb {E} \left[ (X - Z) ^ {2} \mid \mathcal {G} \right] = \mathbb {E} \left[ X ^ {2} \mid \mathcal {G} \right] - 2 \mathbb {E} \left[ X Z \mid \mathcal {G} \right] + \mathbb {E} \left[ Z ^ {2} \mid \mathcal {G} \right]} \\ & {\qquad = \mathbb {E} \left[ X ^ {2} \mid \mathcal {G} \right] - 2 Z \mathbb {E} \left[ X \mid \mathcal {G} \right] + Z ^ {2}} \\ & {\qquad = \mathbb {E} \left[ X ^ {2} \mid \mathcal {G} \right] - 2 Z Y + Z ^ {2}} \\ & {\qquad = \mathbb {E} \left[ X ^ {2} \mid \mathcal {G} \right] - Y ^ {2} + (Y - Z) ^ {2}} \\ & {\qquad = \mathbb {E} \left[ X ^ {2} \mid \mathcal {G} \right] - 2 Y \mathbb {E} \left[ X \mid \mathcal {G} \right] + Y ^ {2} + (Y - Z) ^ {2}} \\ & {\qquad = \mathbb {E} \left[ X ^ {2} \mid \mathcal {G} \right] - 2 \mathbb {E} \left[ X Y \mid \mathcal {G} \right] + \mathbb {E} \left[ Y ^ {2} \mid \mathcal {G} \right] + (Y - Z) ^ {2}} \\ & {\qquad = \mathbb {E} \left[ (X - Y) ^ {2} \mid \mathcal {G} \right] + (Y - Z) ^ {2}.} \end{array}
$$

We also used the fact that Y is $\mathcal { G }$ measurable. Taking expectations and using Proposition $3 . 5 ( 4 )$ , 

$$
\mathbb {E} \left[ (X - Z) ^ {2} \right] = \mathbb {E} \left[ (X - Y) ^ {2} \right] + \mathbb {E} \left[ (Y - Z) ^ {2} \right].
$$

The right hand side is bigger than or equal to $\mathbb { E } \left[ ( X - Y ) ^ { 2 } \right]$ because $( Y - Z ) ^ { 2 } \geq 0 .$ . So the error in predicting X by Z is larger than the error in predicting X by $Y$ , and will be equal if and only if $Z = Y . \ \operatorname { S o } \ Y$ is the best predictor. □ 

There is one more interpretation of conditional expectation that may be useful. The collection of all random variables is a linear space, and the collection of all G-measurable random variables is clearly a subspace. Given $X$ , the conditional expectation $Y = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ is equal to the projection of X onto the subspace of $\mathcal { G } \mathrm { - }$ -measurable random variables. To see this, we write $X = Y + ( X - Y ) $ , and what we have to check is that the inner product of Y and $X - Y$ is 0, that is, Y and $X - Y$ are orthogonal. In this context, the inner product of $X _ { 1 }$ and $X _ { 2 }$ is defined to be $\mathbb { E } \left[ X _ { 1 } X _ { 2 } \right]$ , so we must show $\mathbb { E } \left[ Y ( X - Y ) \right] = 0$ . Note 

$$
\mathbb {E} \left[ Y (X - Y) \mid \mathcal {G} \right] = Y \mathbb {E} \left[ X - Y \mid \mathcal {G} \right] = Y (\mathbb {E} \left[ X \mid \mathcal {G} \right] - Y) = Y (Y - Y) = 0.
$$

Taking expectations, 

$$
\mathbb {E} \left[ Y (X - Y) \right] = \mathbb {E} \left[ \mathbb {E} \left[ Y (X - Y) \mid \mathcal {G} \right] \right] = 0,
$$

just as we wished. 

If Y is a discrete random variable, that is, it takes only countably many values $y _ { 1 } , y _ { 2 } , . . . ,$ we let $B _ { i } = ( Y = y _ { i } )$ . These will be disjoint sets whose union is Ω. If $\sigma ( Y )$ is the collection of all unions of the $B _ { i }$ , then $\sigma ( Y )$ is a $\sigma \cdot$ -field, and is called the σ-field generated by $Y$ . It is easy to see that this is the smallest σ-field with respect to which Y is measurable. We write E $[ X \mid Y ]$ for $\mathbb { E } \left[ X \mid \sigma ( Y ) \right]$ 

Note 1. We prove Proposition 3.5. (1) and (2) are immediate from the definition. To prove (3), note that if $Z = X$ , then $Z$ is $\mathcal { G }$ measurable and $\mathbb { E } \left[ X ; C \right] = \mathbb { E } \left[ Z ; C \right]$ for any $C \in { \mathcal { G } }$ ; this is trivial. By Proposition 3.4 it follows that $Z = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ ];this proves (3). To prove (4), if we let $C = \Omega$ and $Y = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ ], then E $Y = \mathbb { E } \left[ Y ; C \right] = \mathbb { E } \left[ X ; C \right] = \mathbb { E } X$ 

Last is (5). Let $Z ~ = ~ \mathbb { E } X$ . Z is constant, so clearly G measurable. By the independence, if $C \in \mathcal G$ , then $\operatorname { \mathbb { E } } \left[ X ; C \right] = \operatorname { \mathbb { E } } \left[ X 1 _ { C } \right] = ( \operatorname { \mathbb { E } } X ) ( \operatorname { \mathbb { E } } 1 _ { C } ) = ( \operatorname { \mathbb { E } } X ) ( \operatorname { \mathbb { P } } ( C ) )$ . But $\mathbb { E } \left[ Z ; C \right] = ( \mathbb { E } X ) ( \mathbb { P } ( C ) )$ since $Z$ is constant. By Proposition 3.4 we see $Z = \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ □ 

Note 2. We prove Proposition 3.6. Note that $Z \mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ is $\mathcal { G }$ measurable, so by Proposition 3.4 we need to show its expectation over sets C in G is the same as that of $X Z .$ . As in the proof of Proposition 3.3, it sufices to consider only the case when $C$ is one of the $B _ { i }$ . Now $Z$ is $\mathcal { G }$ measurable, hence it is constant on $B _ { i }$ ; let its value be $z _ { i }$ . Then 

$$
\mathbb {E} \left[ Z \mathbb {E} [ X \mid \mathcal {G} ]; B _ {i} \right] = \mathbb {E} \left[ z _ {i} \mathbb {E} [ X \mid \mathcal {G} ]; B _ {i} \right] = z _ {i} \mathbb {E} \left[ \mathbb {E} [ X \mid \mathcal {G} ]; B _ {i} \right] = z _ {i} \mathbb {E} [ X; B _ {i} ] = \mathbb {E} [ X Z; B _ {i} ]
$$

as desired. 

## 4. Martingales.

Suppose we have a sequence of σ-fields ${ \mathcal { F } } _ { 1 } \subset { \mathcal { F } } _ { 2 } \subset { \mathcal { F } } _ { 3 } \cdot \cdot \cdot$ . An example would be repeatedly tossing a coin and letting $\mathcal { F } _ { k }$ be the sets that can be determined by the first k tosses. Another example is to let $\mathcal { F } _ { k }$ be the events that are determined by the values of a stock at times 1 through k. A third example is to let $X _ { 1 } , X _ { 2 } , . . .$ . be a sequence of random variables and let $\mathcal { F } _ { k }$ be the σ-field generated by $X _ { 1 } , \ldots , X _ { k }$ , the smallest σ-field with respect to which $X _ { 1 } , \ldots , X _ { k }$ are measurable. 

Definition 4.1. A r.v. X is integrable if $\mathbb { E } \left| X \right| < \infty$ . Given an increasing sequence of σ-fields ${ \mathcal { F } } _ { n }$ , a sequence of $r . v . \ ' { s } X _ { n }$ is adapted if $X _ { n }$ is ${ \mathcal { F } } _ { n }$ measurable for each n. 

Definition 4.2. A martingale $M _ { n }$ is a sequence of random variables such that 

(1) $M _ { n }$ is integrable for all n, 

(2) $M _ { n }$ is adapted to ${ \mathcal { F } } _ { n }$ , and 

(3) for all n 

$$
\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right] = M _ {n}.\tag{4.1}
$$

Usually (1) and (2) are easy to check, and it is (3) that is the crucial property. If we have (1) and (2), but instead of (3) we have 

(30) for all n 

$$
\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right] \geq M _ {n},
$$

then we say $M _ { n }$ is a submartingale. If we have (1) and (2), but instead of (3) we have (300) for all n 

$$
\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right] \leq M _ {n},
$$

then we say $M _ { n }$ is a supermartingale. 

Submartingales tends to increase and supermartingales tend to decrease. The nomenclature may seem like it goes the wrong way; Doob defined these terms by analogy with the notions of subharmonic and superharmonic functions in analysis. (Actually, it is more than an analogy: we won’t explore this, but it turns out that the composition of a subharmonic function with Brownian motion yields a submartingale, and similarly for superharmonic functions.) 

Note that the definition of martingale depends on the collection of σ-fields. When it is needed for clarity, one can say that $\left( M _ { n } , \mathcal { F } _ { n } \right)$ is a martingale. To define conditional expectation, one needs a probability, so a martingale depends on the probability as well. When we need to, we will say that $M _ { n }$ is a martingale with respect to the probability P. This is an issue when there is more than one probability around. 

We will see that martingales are ubiquitous in financial math. For example, security prices and one’s wealth will turn out to be examples of martingales. 

The word “martingale” is also used for the piece of a horse’s bridle that runs from the horse’s head to its chest. It keeps the horse from raising its head too high. It turns out that martingales in probability cannot get too large. The word also refers to a gambling system. I did some searching on the Internet, and there seems to be no consensus on the derivation of the term. 

Here is an example of a martingale. Let $X _ { 1 } , X _ { 2 } , \ldots$ . be a sequence of independent $\mathrm { r . v . \dot { s } }$ with mean 0 that are independent. (Saying a r.v. X has mean 0 is the same as saying E $X _ { i } \ = \ 0 ;$ this presupposes that E $| X _ { 1 } |$ is finite.) Set ${ \mathcal { F } } _ { n } = \sigma ( X _ { 1 } , \ldots , X _ { n } )$ , the σ-field generated by $X _ { 1 } , \ldots , X _ { n }$ . Let $\begin{array} { r } { M _ { n } \ = \ \sum _ { i = 1 } ^ { n } X _ { i } } \end{array}$ . Definition $4 . 2 ( 2 )$ is easy to see. Since $\begin{array} { r } { \mathbb { E } \left| M _ { n } \right| \leq \sum _ { i = 1 } ^ { n } \mathbb { E } \left| X _ { i } \right| } \end{array}$ , Definition $4 . 2 ( 1 )$ also holds. We now check 

$$
\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right] = X _ {1} + \dots + X _ {n} + \mathbb {E} \left[ X _ {n + 1} \mid \mathcal {F} _ {n} \right] = M _ {n} + \mathbb {E} X _ {n + 1} = M _ {n},
$$

where we used the independence. 

Another example: suppose in the above that the $X _ { k }$ all have variance 1, and let $M _ { n } = S _ { n } ^ { 2 } - n$ , where $\begin{array} { r } { S _ { n } = \sum _ { i = 1 } ^ { n } X _ { i } } \end{array}$ . Again (1) and (2) of Definition 4.2 are easy to check. We compute 

$$
\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right] = \mathbb {E} \left[ S _ {n} ^ {2} + 2 X _ {n + 1} S _ {n} + X _ {n + 1} ^ {2} \mid \mathcal {F} _ {n} \right] - (n + 1).
$$

We have $\mathbb { E } \left[ S _ { n } ^ { 2 } \mid \mathcal { F } _ { n } \right] = S _ { n } ^ { 2 }$ since $S _ { n }$ is ${ \mathcal { F } } _ { n }$ measurable. 

$$
\mathbb {E} \left[ 2 X _ {n + 1} S _ {n} \mid \mathcal {F} _ {n} \right] = 2 S _ {n} \mathbb {E} \left[ X _ {n + 1} \mid \mathcal {F} _ {n} \right] = 2 S _ {n} \mathbb {E} X _ {n + 1} = 0.
$$

And E $[ X _ { n + 1 } ^ { 2 } \mid \mathcal { F } _ { n } ] = \mathbb { E } X _ { n + 1 } ^ { 2 } = 1$ . Substituting, we obtain E $\left[ M _ { n + 1 } \mid { \mathcal { F } } _ { n } \right] = M _ { n }$ , or $M _ { n }$ is a martingale. 

A third example: Suppose you start with a dollar and you are tossing a fair coin independently. If it turns up heads you double your fortune, tails you go broke. This is “double or nothing.” Let $M _ { n }$ be your fortune at time n. To formalize this, let $X _ { 1 } , X _ { 2 } , \ldots$ be independent r.v.’s that are equal to 2 with probability $\begin{array} { l } { { \frac { 1 } { 2 } } } \end{array}$ and 0 with probability $M _ { n } = X _ { 1 } \cdot \cdot \cdot X _ { n }$ . Let ${ \mathcal { F } } _ { n }$ be the σ-field generated by $X _ { 1 } , \ldots , X _ { n }$ . Note $0 \leq M _ { n } \leq 2 ^ { n }$ , and so Definition 4.2(1) is satisfied, while (2) is easy. To compute the conditional expectation, note E $X _ { n + 1 } = 1$ . Then 

$$
\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right] = M _ {n} \mathbb {E} \left[ X _ {n + 1} \mid \mathcal {F} _ {n} \right] = M _ {n} \mathbb {E} X _ {n + 1} = M _ {n},
$$

using the independence. 

Before we give our fourth example, let us observe that 

$$
\left| \mathbb {E} [ X \mid \mathcal {F} ] \right| \leq \mathbb {E} \left[ | X | \mid \mathcal {F} \right].\tag{4.2}
$$

To see this, we have $- | X | \leq X \leq | X | ,$ so $- \mathbb { E } \left[ | X | \mid { \mathcal { F } } \right] \leq \mathbb { E } \left[ X \mid { \mathcal { F } } \right] \leq \mathbb { E } \left[ | X | \mid { \mathcal { F } } \right]$ . Since $\mathbb { E } [ | X | | { \mathcal { F } } ]$ is nonnegative, (4.2) follows. 

Our fourth example will be used many times, so we state it as a proposition. 

Proposition 4.3. Let $\mathcal { F } _ { 1 } , \mathcal { F } _ { 2 } , \ldots$ . be given and let X be a fixed r.v. with $\mathbb { E } \left| X \right| < \infty$ . Let $M _ { n } = \mathbb { E } \left[ X \mid { \mathcal { F } } _ { n } \right]$ . Then $M _ { n }$ is a martingale. 

Proof. Definition 4.2(2) is clear, while 

$$
\mathbb {E} \left| M _ {n} \right| \leq \mathbb {E} \left[ \mathbb {E} \left[ | X | \mid \mathcal {F} _ {n} \right] \right] = \mathbb {E} \left| X \right| <   \infty
$$

by (4.2); this shows Definition 4.2(1). We have 

$$
\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right] = \mathbb {E} \left[ \mathbb {E} \left[ X \mid \mathcal {F} _ {n + 1} \right] \mid \mathcal {F} _ {n} \right] = \mathbb {E} \left[ X \mid \mathcal {F} _ {n} \right] = M _ {n}.
$$

## 5. Properties of martingales.

When it comes to discussing American options, we will need the concept of stopping times. A mapping τ from Ω into the nonnegative integers is a stopping time if $( \tau = k ) \in \mathcal { F } _ { k }$ for each k. 

An example is $\tau =$ min $\{ k : S _ { k } \geq A \}$ . This is a stopping time because $( \tau = k ) =$ $( S _ { 1 } , \ldots , S _ { k - 1 } < A , S _ { k } \ge A ) \in { \mathcal { F } } _ { k }$ . We can think of a stopping time as the first time something happens. $\sigma = \operatorname* { m a x } \{ k : S _ { k } \geq A \}$ , the last time, is not a stopping time. (We will use the convention that the minimum of an empty set $\mathrm { i s \ t { \infty } ; \ s o }$ , for example, with the above definition of τ, on the event that $S _ { k }$ is never in A, we have $\tau = \infty$ 

Here is an intuitive description of a stopping time. If I tell you to drive to the city limits and then drive until you come to the second stop light after that, you know when you get there that you have arrived; you don’t need to have been there before or to look ahead. But if I tell you to drive until you come to the second stop light before the city limits, either you must have been there before or else you have to go past where you are supposed to stop, continue on to the city limits, and then turn around and come back two stop lights. You don’t know when you first get to the second stop light before the city limits that you get to stop there. The first set of instructions forms a stopping time, the second set does not. 

Note $( \tau \leq k ) = \cup _ { i = 0 } ^ { k } ( \tau = j )$ . Since $( \tau = j ) \in \mathcal { F } _ { j } \subset \mathcal { F } _ { k }$ , then the event $( \tau \leq k ) \in \mathcal { F } _ { k }$ for all k. Conversely, if τ is a r.v. with $( \tau \leq k ) \in \mathcal { F } _ { k }$ for all k, then 

$$
(\tau = k) = (\tau \leq k) - (\tau \leq k - 1).
$$

Since $( \tau \leq k ) \in \mathcal { F } _ { k }$ and $( \tau \le k - 1 ) \in \mathcal { F } _ { k - 1 } \subset \mathcal { F } _ { k }$ , then $( \tau = k ) \in \mathcal { F } _ { k }$ , and such $\mathrm { ~ a ~ } \tau$ must be a stopping time. 

Our first result is Jensen’s inequality. 

Proposition 5.1. ${ \mathit { I f } } { \mathit { g } }$ is convex, then 

$$
g (\mathbb {E} [ X \mid \mathcal {G} ]) \leq \mathbb {E} [ g (X) \mid \mathcal {G} ]
$$

provided all the expectations exist. 

For ordinary expectations rather than conditional expectations, this is still true. That is, if g is convex and the expectations exist, then 

$$
g (\mathbb {E} X) \leq \mathbb {E} [ g (X) ].
$$

We already know some special cases of this: when $g ( x ) = | x | .$ , this says $\left| \mathbb { E } X \right| \leq \mathbb { E } \left| X \right|$ when $g ( x ) = x ^ { 2 }$ , this says $( \mathbb { E } X ) ^ { 2 } \ \leq \ \mathbb { E } X ^ { 2 }$ , which we know because E $X ^ { 2 } - ( \mathbb { E } X ) ^ { 2 } \ =$ $\mathbb { E } \left( X - \mathbb { E } X \right) ^ { 2 } \geq 0$ 

For Proposition 5.1 as well as many of the following propositions, the statement of the result is more important than the proof, and we relegate the proof to Note 1 below. 

One reason we want Jensen’s inequality is to show that a convex function applied to a martingale yields a submartingale. 

Proposition 5.2. If $M _ { n }$ is a martingale and g is convex, then $g ( M _ { n } )$ is a submartingale, provided all the expectations exist. 

Proof. By Jensen’s inequality, 

$$
\mathbb {E} \left[ g (M _ {n + 1}) \mid \mathcal {F} _ {n} \right] \geq g (\mathbb {E} \left[ M _ {n + 1} \mid \mathcal {F} _ {n} \right]) = g (M _ {n}).
$$

If $M _ { n }$ is a martingale, then E $M _ { n } = \mathbb { E } \left[ \mathbb { E } \left[ M _ { n + 1 } \mid \mathcal { F } _ { n } \right] \right] = \mathbb { E } M _ { n + 1 }$ . So E $M _ { 0 }$ = $\mathbb { E } M _ { 1 } = \cdot \cdot \cdot = \mathbb { E } M _ { n }$ . Doob’s optional stopping theorem says the same thing holds when fixed times n are replaced by stopping times. 

Theorem 5.3. Suppose K is a positive integer, N is a stopping time such that $N \leq K$ $a . S . ,$ and $M _ { n }$ is a martingale. Then 

$$
\mathbb {E} M _ {N} = \mathbb {E} M _ {K}.
$$

Here, to evaluate $M _ { N }$ , one first finds $N ( \omega )$ and then evaluates $M . ( \omega )$ for that value of N. 

Proof. We have 

$$
\mathbb {E} M _ {N} = \sum_ {k = 0} ^ {K} \mathbb {E} [ M _ {N}; N = k ].
$$

If we show that the k-th summand is $\mathbb { E } \left[ M _ { n } ; N = k \right]$ , then the sum will be 

$$
\sum_ {k = 0} ^ {K} \mathbb {E} \left[ M _ {n}; N = k \right] = \mathbb {E} M _ {n}
$$

as desired. We have 

$$
\mathbb {E} \left[ M _ {N}; N = k \right] = \mathbb {E} \left[ M _ {k}; N = k \right]
$$

by the definition of $M _ { N }$ . Now $( N = k )$ is in $\mathcal { F } _ { k }$ , so by Proposition 2.2 and the fact that $M _ { k } = \mathbb { E } \left[ M _ { k + 1 } \mid \mathcal { F } _ { k } \right]$ 2 

$$
\mathbb {E} \left[ M _ {k}; N = k \right] = \mathbb {E} \left[ M _ {k + 1}; N = k \right].
$$

We have $( N = k ) \in \mathcal { F } _ { k } \subset \mathcal { F } _ { k + 1 }$ . Since $M _ { k + 1 } = \operatorname { \mathbb { E } } \left[ M _ { k + 2 } \ | \ \mathcal { F } _ { k + 1 } \right]$ , Proposition 2.2 tells us that 

$$
\mathbb {E} \left[ M _ {k + 1}; N = k \right] = \mathbb {E} \left[ M _ {k + 2}; N = k \right].
$$

We continue, using $( N = k ) \in \mathcal { F } _ { k } \subset \mathcal { F } _ { k + 1 } \subset \mathcal { F } _ { k + 2 }$ , and we obtain 

$$
\mathbb {E} \left[ M _ {N}; N = k \right] = \mathbb {E} \left[ M _ {k}; N = k \right] = \mathbb {E} \left[ M _ {k + 1}; N = k \right] = \dots = \mathbb {E} \left[ M _ {n}; N = k \right].
$$

If we change the equalities in the above to inequalities, the same result holds for submartingales. 

As a corollary we have two of Doob’s inequalities: 

Theorem 5.4. $I f M _ { n }$ is a nonnegative submartingale, 

(a) $\begin{array} { r } { \mathbb { P } ( \operatorname* { m a x } _ { k \leq n } M _ { k } \geq \lambda ) \leq \frac { 1 } { \lambda } \mathbb { E } M _ { n } . } \end{array}$ 

(b) E (max<sub>k≤n</sub> M<sup>2</sup>) ≤ 4E M<sup>2</sup>. 

For the proof, see Note 2 below. 

Note 1. We prove Proposition 5.1. If $g$ is convex, then the graph of $g$ lies above all the tangent lines. Even if $g$ does not have a derivative at $x _ { 0 }$ , there is a line passing through $x _ { 0 }$ which lies beneath the graph of $g .$ So for each $x _ { 0 }$ there exists $c ( x _ { 0 } )$ such that 

$$
g (x) \geq g (x _ {0}) + c (x _ {0}) (x - x _ {0}).
$$

Apply this with $x = X ( \omega )$ and $x _ { 0 } = \mathbb { E } \left[ X \mid { \mathcal { G } } \right] ( \omega )$ . We then have 

$$
g (X) \geq g (\mathbb {E} [ X \mid \mathcal {G} ]) + c (\mathbb {E} [ X \mid \mathcal {G} ]) (X - \mathbb {E} [ X \mid \mathcal {G} ]).
$$

If $g$ is diferentiable, we let $c ( x _ { 0 } ) = g ^ { \prime } ( x _ { 0 } )$ . In the case where $g$ is not diferentiable, then we choose c to be the left hand upper derivate, for example. (For those who are not familiar with derivates, this is essentially the left hand derivative.) One can check that if c is so chosen, then $c ( \mathbb { E } \left[ X \mid { \mathcal { G } } \right] )$ is $\mathcal { G }$ measurable. 

Now take the conditional expectation with respect to $\mathcal { G }$ . The first term on the right is $\mathcal { G }$ measurable, so remains the same. The second term on the right is equal to 

$$
c (\mathbb {E} [ X \mid \mathcal {G} ]) \mathbb {E} [ X - \mathbb {E} [ X \mid \mathcal {G} ] \mid \mathcal {G} ] = 0.
$$

Note 2. We prove Theorem 5.4. Set $M _ { n + 1 } = M _ { n }$ . It is easy to see that the sequence $M _ { 1 } , M _ { 2 } , \ldots , M _ { n + 1 }$ is also a submartingale. Let $N = \operatorname* { m i n } \{ k : M _ { k } \geq \lambda \} \wedge ( n + 1 )$ , the first time that $M _ { k }$ is greater than or equal to $\lambda ,$ where $a \wedge b = \operatorname* { m i n } ( a , b )$ . Then 

$$
\mathbb {P} (\max _ {k \leq n} M _ {k} \geq \lambda) = \mathbb {P} (N \leq n)
$$

and if $N \leq n$ , then $M _ { N } \ge \lambda$ . Now 

$$
\begin{array}{r l} & {\mathbb {P} (\max _ {k \leq n} M _ {k} \geq \lambda) = \mathbb {E} [ 1 _ {(N \leq n)} ] \leq \mathbb {E} \left[ \frac {M _ {N}}{\lambda}; N \leq n \right]} \\ & {\qquad = \frac {1}{\lambda} \mathbb {E} [ M _ {N \wedge n}; N \leq n ] \leq \frac {1}{\lambda} \mathbb {E} M _ {N \wedge n}.} \end{array}\tag{5.1}
$$

Finally, since $M _ { n }$ is a submartingale, E $M _ { N \wedge n } \leq \mathbb { E } M _ { n }$ 

We now look at (b). Let us write $M ^ { * }$ for $\operatorname* { m a x } _ { k \leq n } M _ { k }$ . If E $M _ { n } ^ { 2 } = \infty$ , there is nothing to prove. If it is finite, then by Jensen’s inequality, we have 

$$
\mathbb {E} M _ {k} ^ {2} = \mathbb {E} \left[ \mathbb {E} \left[ M _ {n} \mid \mathcal {F} _ {k} \right] ^ {2} \right] \leq \mathbb {E} \left[ \mathbb {E} \left[ M _ {n} ^ {2} \mid \mathcal {F} _ {k} \right] \right] = \mathbb {E} M _ {n} ^ {2} <   \infty
$$

for $k \leq n$ . Then 

$$
\mathbb {E} \left(M ^ {*}\right) ^ {2} = \mathbb {E} \left[ \max _ {1 \leq k \leq n} M _ {k} ^ {2} \right] \leq \mathbb {E} \left[ \sum_ {k = 1} ^ {n} M _ {k} ^ {2} \right] <   \infty .
$$

We have 

$$
\mathbb {E} \left[ M _ {N \wedge n}; N \leq n \right] = \sum_ {k = 0} ^ {\infty} \mathbb {E} \left[ M _ {k \wedge n}; N = k \right].
$$

Arguing as in the proof of Theorem 5.3, 

$$
\mathbb {E} \left[ M _ {k \wedge n}; N = k \right] \leq \mathbb {E} \left[ M _ {n}; N = k \right],
$$

and so 

$$
\mathbb {E} \left[ M _ {N \wedge n}; N \leq n \right] \leq \sum_ {k = 0} ^ {\infty} \mathbb {E} \left[ M _ {n}; N = k \right] = \mathbb {E} \left[ M _ {n}; N \leq n \right].
$$

The last expression is at most $\mathbb { E } \left[ M _ { n } ; M ^ { * } \ge \lambda \right]$ . If we multiply (5.1) by 2λ and integrate over λ from 0 to ∞, we obtain 

$$
\begin{array}{r l} & {\int_ {0} ^ {\infty} 2 \lambda \mathbb {P} (M ^ {*} \geq \lambda) d \lambda \leq 2 \int_ {0} ^ {\infty} \mathbb {E} [ M _ {n}: M ^ {*} \geq \lambda ]} \\ & {\qquad = 2 \mathbb {E} \int_ {0} ^ {\infty} M _ {n} 1 _ {(M ^ {*} \geq \lambda)} d \lambda} \\ & {\qquad = 2 \mathbb {E} \left[ M _ {n} \int_ {0} ^ {M ^ {*}} d \lambda \right]} \\ & {\qquad = 2 \mathbb {E} [ M _ {n} M ^ {*} ].} \end{array}
$$

Using Cauchy-Schwarz, this is bounded by 

$$
2 (\mathbb {E} M _ {n} ^ {2}) ^ {1 / 2} (\mathbb {E} (M ^ {*}) ^ {2}) ^ {1 / 2}.
$$

On the other hand, 

$$
\begin{array}{c} \int_ {0} ^ {\infty} 2 \lambda \mathbb {P} (M ^ {*} \geq \lambda) d \lambda = \mathbb {E} \int_ {0} ^ {\infty} 2 \lambda 1 _ {(M ^ {*} \geq \lambda)} d \lambda \\ = \mathbb {E} \int_ {0} ^ {M ^ {*}} 2 \lambda d \lambda = \mathbb {E} (M ^ {*}) ^ {2}. \end{array}
$$

We therefore have 

$$
\mathbb {E} \left(M ^ {*}\right) ^ {2} \leq 2 (\mathbb {E} M _ {n} ^ {2}) ^ {1 / 2} (\mathbb {E} \left(M ^ {*}\right) ^ {2}) ^ {1 / 2}.
$$

Recall we showed $\mathbb { E } { ( M ^ { * } ) } ^ { 2 } < \infty$ . We divide both sides by $( \mathbb { E } ( M ^ { * } ) ^ { 2 } ) ^ { 1 / 2 }$ , square both sides, and obtain (b). □ 

Note 3. We will show that bounded martingales converge. (The hypothesis of boundedness can be weakened; for example, $\mathbb { E } \left| M _ { n } \right| \le c < \infty$ for some c not depending on n sufices.) 

Theorem 5.5. Suppose $M _ { n }$ is a martingale bounded in absolute value by K. That is, $| M _ { n } | \leq K$ for all n. Then lim $\mathsf { \Pi } _ { { n } \to \infty } M _ { n }$ exists a.s. 

Proof. Since $M _ { n }$ is bounded, it can’t tend $_ { \mathsf { t } 0 } + \infty \mathrm { o r } \mathrm { - } \infty$ . The only possibility is that it might oscillate. Let $a < b$ be two rationals. What might go wrong is that $M _ { n }$ might be larger than b infinitely often and less than a infinitely often. If we show the probability of this is 0, then taking the union over all pairs of rationals $( a , b )$ shows that almost surely $M _ { n }$ cannot oscillate, and hence must converge. 

Fix $a < b ,$ let $N _ { n } = ( M _ { n } - a ) ^ { + }$ , and let $S _ { 1 } = \operatorname* { m i n } \{ k : N _ { k } \leq 0 \} , T _ { 1 } = \operatorname* { m i n } \{ k > S _ { 1 }$ $N _ { k } \ge b - a \} , S _ { 2 } = \operatorname* { m i n } \{ k > T _ { 1 } : N _ { k } \le 0 \}$ , and so on. Let $U _ { n } = \operatorname* { m a x } \{ k : T _ { k } \leq n \} . \ U _ { n }$ is called the number of upcrossings up to time n. We want to show that ma $\mathrm { x } _ { n } U _ { n } <$ ∞ a.s. Note by Jensen’s inequality $N _ { n }$ is a submartingale. Since $S _ { 1 } < T _ { 1 } < S _ { 2 } < \cdots$ , then $S _ { n + 1 } > n$ 

We can write 

$$
2 K \geq N _ {n} - N _ {S _ {n + 1} \wedge n} = \sum_ {k = 1} ^ {n + 1} (N _ {S _ {k + 1} \wedge n} - N _ {T _ {k} \wedge n}) + \sum_ {k = 1} ^ {n + 1} (N _ {T _ {k} \wedge n} - N _ {S _ {k} \wedge n}).
$$

Now take expectations. The expectation of the first sum on the right and the last term are greater than or equal to zero by optional stopping. The middle term is larger than $( b - a ) U _ { n }$ so we conclude 

$$
(b - a) \mathbb {E} U _ {n} \leq 2 K.
$$

Let $n \to \infty$ to see that E $\operatorname* { m a x } _ { n } U _ { n } < \infty$ , which implies ma $\qquad \mathrm { x } _ { n } U _ { n } < \infty { \mathsf { a } } . 5 .$ ., which is what we needed. □ 

Note 4. We will state Fatou’s lemma in the following form. 

If $X _ { n }$ is a sequence of nonnegative random variables converging to $X \ \mathsf { a } . \mathsf { s } .$ , then $\mathbb { E } X \leq$ $\operatorname* { s u p } _ { n } \mathbb { E } X _ { n }$ 

This formulation is equivalent to the classical one and is better suited for our use. 

## 6. The one step binomial asset pricing model.

Let us begin by giving the simplest possible model of a stock and see how a European call option should be valued in this context. 

Suppose we have a single stock whose price is $S _ { 0 }$ . Let d and u be two numbers with $0 < d < 1 < u$ . Here $^ { 6 } d ^ { 5 }$ is a mnemonic for “down” and $^ { \circ } u ^ { \prime \prime }$ for $\mathrm { \ddot { \ u p . } } ^ { \mathrm { \prime \prime } }$ After one time unit the stock price will be either $u S _ { 0 }$ with probability P or else $d S _ { 0 }$ with probability $Q ,$ where $P + Q = 1$ . We will assume $0 < P , Q < 1$ . Instead of purchasing shares in the stock, you can also put your money in the bank where one will earn interest at rate r. Alternatives to the bank are money market funds or bonds; the key point is that these are considered to be risk-free. 

A European call option in this context is the option to buy one share of the stock at time 1 at price K. K is called the strike price. Let $S _ { 1 }$ be the price of the stock at time 1. If $S _ { 1 }$ is less than $K .$ , then the option is worthless at time 1. If $S _ { 1 }$ is greater than $K$ , you can use the option at time 1 to buy the stock at price $K$ , immediately turn around and sell the stock for price $S _ { 1 }$ and make a profit of $S _ { 1 } - K$ . So the value of the option at time 1 is 

$$
V _ {1} = (S _ {1} - K) ^ {+},
$$

where $x ^ { + }$ is $\mathrm { m a x } ( x , 0 )$ . The principal question to be answered is: what is the value $V _ { 0 }$ of the option at time 0? In other words, how much should one pay for a European call option with strike price K? 

It is possible to buy a negative number of shares of a stock. This is equivalent to selling shares of a stock you don’t have and is called selling short. If you sell one share of stock short, then at time 1 you must buy one share at whatever the market price is at that time and turn it over to the person that you sold the stock short to. Similarly you can buy a negative number of options, that is, sell an option. 

You can also deposit a negative amount of money in the bank, which is the same as borrowing. We assume that you can borrow at the same interest rate $r ,$ , not exactly a totally realistic assumption. One way to make it seem more realistic is to assume you have a large amount of money on deposit, and when you borrow, you simply withdraw money from that account. 

We are looking at the simplest possible model, so we are going to allow only one time step: one makes an investment, and looks at it again one day later. 

Let’s suppose the price of a European call option is $V _ { 0 }$ and see what conditions one can put on $V _ { 0 }$ . Suppose you start out with $V _ { 0 }$ dollars. One thing you could do is buy one option. The other thing you could do is use the money to buy $\Delta _ { 0 }$ shares of stock. If $V _ { 0 } > \Delta _ { 0 } S _ { 0 }$ , there will be some money left over and you put that in the bank. If $V _ { 0 } < \Delta _ { 0 } S _ { 0 }$ , you do not have enough money to buy the stock, and you make up the shortfall by borrowing money from the bank. In either case, at this point you have $V _ { 0 } - \Delta _ { 0 } S _ { 0 }$ in 

the bank and $\Delta _ { 0 }$ shares of stock. 

If the stock goes up, at time 1 you will have 

$$
\Delta_ {0} u S _ {0} + (1 + r) (V _ {0} - \Delta_ {0} S _ {0}),
$$

and if it goes down, 

$$
\Delta_ {0} d S _ {0} + (1 + r) \left(V _ {0} - \Delta_ {0} S _ {0}\right).
$$

We have not said what $\Delta _ { 0 }$ should be. Let us do that now. Let $V _ { 1 } ^ { u } = ( u S _ { 0 } - K ) ^ { - }$ + and $V _ { 1 } ^ { d } = ( d { \cal S } _ { 0 } - K ) ^ { + }$ . Note these are deterministic quantities, i.e., not random. Let 

$$
\Delta_ {0} = \frac {V _ {1} ^ {u} - V _ {1} ^ {d}}{u S _ {0} - d S _ {0}},
$$

and we will also need 

$$
W _ {0} = \frac {1}{1 + r} \Big [ \frac {1 + r - d}{u - d} V _ {1} ^ {u} + \frac {u - (1 + r)}{u - d} V _ {1} ^ {d} \Big ].
$$

In a moment we will do some algebra and see that if the stock goes up and you had bought stock instead of the option you would now have 

$$
V _ {1} ^ {u} + (1 + r) (V _ {0} - W _ {0}),
$$

while if the stock went down, you would now have 

$$
V _ {1} ^ {d} + (1 + r) (V _ {0} - W _ {0}).
$$

Let’s check the first of these, the second being similar. We need to show 

$$
\Delta_ {0} u S _ {0} + (1 + r) (V _ {0} - \Delta_ {0} S _ {0}) = V _ {1} ^ {u} + (1 + r) (V _ {0} - W _ {0}).\tag{6.1}
$$

The left hand side of (6.1) is equal to 

$$
\Delta_ {0} S _ {0} (u - (1 + r)) + (1 + r) V _ {0} = \frac {V _ {1} ^ {u} - V _ {1} ^ {d}}{u - d} (u - (1 + r)) + (1 + r) V _ {0}.\tag{6.2}
$$

The right hand side of (6.1) is equal to 

$$
V _ {1} ^ {u} - \left[ \frac {1 + r - d}{u - d} V _ {1} ^ {u} + \frac {u - (1 + r)}{u - d} V _ {1} ^ {d} \right] + (1 + r) V _ {0}.\tag{6.3}
$$

Now check that the coeficients of $V _ { 0 } { \mathrm { . } }$ , of $V _ { 1 } ^ { u }$ , and of $V _ { 1 } ^ { d }$ agree in (6.2) and (6.3). 

Suppose that $V _ { 0 } > W _ { 0 }$ . What you want to do is come along with no money, sell one option for $V _ { 0 }$ dollars, use the money to buy $\Delta _ { 0 }$ shares, and put the rest in the bank (or borrow if necessary). If the buyer of your option wants to exercise the option, you give him one share of stock and sell the rest. If he doesn’t want to exercise the option, you sell your shares of stock and pocket the money. Remember it is possible to have a negative number of shares. You will have cleared $( 1 + r ) ( V _ { 0 } - W _ { 0 } )$ , whether the stock went up or down, with no risk. 

If $V _ { 0 } < W _ { 0 } ,$ , you just do the opposite: sell $\Delta _ { 0 }$ shares of stock short, buy one option, and deposit or make up the shortfall from the bank. This time, you clear $( 1 + r ) ( W _ { 0 } - V _ { 0 } )$ whether the stock goes up or down. 

Now most people believe that you can’t make a profit on the stock market without taking a risk. The name for this is “no free lunch,” or “arbitrage opportunities do not exist.” The only way to avoid this is if $V _ { 0 } = W _ { 0 }$ . In other words, we have shown that the only reasonable price for the European call option is $W _ { 0 }$ 

The “no arbitrage” condition is not just a reflection of the belief that one cannot get something for nothing. It also represents the belief that the market is freely competitive. The way it works is this: suppose $W _ { 0 } = { \mathfrak { H } } 3$ . Suppose you could sell options at a price $V _ { 0 } = \mathbb { S } 5 ;$ this is larger than $W _ { 0 }$ and you would earn $V _ { 0 } - W _ { 0 } = \mathfrak { H } 2$ per option without risk. Then someone else would observe this and decide to sell the same option at a price less than $V _ { 0 }$ but larger than $W _ { 0 }$ , say $\$ 4$ . This person would still make a profit, and customers would go to him and ignore you because they would be getting a better deal. But then a third person would decide to sell the option for less than your competition but more than $W _ { 0 }$ , say at $3.50. This would continue as long as any one would try to sell an option above price $W _ { 0 }$ 

We will examine this problem of pricing options in more complicated contexts, and while doing so, it will become apparent where the formulas for $\Delta _ { 0 }$ and $W _ { 0 }$ came from. At this point, we want to make a few observations. 

Remark 6.1. First of all, ${ \mathrm { i f ~ } } 1 + r > u .$ , one would never buy stock, since one can always do better by putting money in the bank. So we may suppose $1 + r < u$ . We always have $1 + r \geq 1 > d .$ . If we set 

$$
\overline {{p}} = \frac {1 + r - d}{u - d}, \qquad \overline {{q}} = \frac {u - (1 + r)}{u - d},
$$

then $\overline { { p } } , \overline { { q } } \geq 0$ and $\overline { { p } } + \overline { { q } } = 1$ . Thus $\overline { { p } }$ and $\overline { { q } }$ act like probabilities, but they have nothing to do with $P$ and $Q .$ . Note also that the price $V _ { 0 } = W _ { 0 }$ does not depend on $P$ or $Q .$ It does depend on $\overline { { p } }$ and ${ \overline { { q } } } ,$ which seems to suggest that there is an underlying probability which controls the option price and is not the one that governs the stock price. 

Remark 6.2. There is nothing special about European call options in our argument above. One could let $V _ { 1 } ^ { u }$ and $V _ { d } ^ { 1 }$ be any two values of any option, which are paid out if the stock goes up or dow $^ { \mathrm { n , } }$ respectively. The above analysis shows we can exactly duplicate the result of buying any option V by instead buying some shares of stock. If in some model one can do this for any option, the market is called complete in this model. 

Remark 6.3. If we let $\overline { { \mathbb { P } } }$ be the probability so that $S _ { 1 } = u S _ { 0 }$ with probability $\overline { { p } }$ and $S _ { 1 } = d S _ { 0 }$ with probability $\overline { { q } }$ and we let $\overline { { \mathbb { E } } }$ be the corresponding expectation, then some algebra shows that 

$$
V _ {0} = \frac {1}{1 + r} \overline {{\mathbb {E}}} V _ {1}.
$$

This will be generalized later. 

Remark 6.4. If one buys one share of stock at time $0 ,$ then one expects at time 1 to have $( P u + Q d ) S _ { 0 }$ . One then divides by $1 + r$ to get the value of the stock in today’s dollars. $( r ,$ the risk-free interest rate, can also be considered the rate of inflation. A dollar tomorrow is equivalent to $1 / ( 1 + r )$ dollars today.) Suppose instead of P and $Q$ being the probabilities of going up and down, they were in fact $\overline { { p } }$ and ${ \overline { { q } } } .$ One would then expect to have $( \overline { { p } } u + \overline { { q } } d ) S _ { 0 }$ and then divide by $1 + r .$ . Substituting the values for $\overline { { p } }$ and ${ \overline { { q } } } ,$ this reduces to $S _ { 0 }$ . In other words, if $\overline { { p } }$ and $\overline { { q } }$ were the correct probabilities, one would expect to have the same amount of money one started with. When we get to the binomial asset pricing model with more than one step, we will see that the generalization of this fact is that the stock price at time n is a martingale, still with the assumption that $\overline { { p } }$ and $\overline { { q } }$ are the correct probabilities. This is a special case of the fundamental theorem of finance: there always exists some probabili $\mathrm { t y , }$ not necessarily the one you observe, under which the stock price is a martingale. 

Remark 6.5. Our model allows after one time step the possibility of the stock going up or going down, but only these two options. What if instead there are 3 (or more) possibilities. Suppose for example, that the stock goes up a factor u with probability $P ,$ , down a factor d with probability $Q ,$ and remains constant with probability $R ,$ where $P + Q + R = 1$ The corresponding price of a European call option would be $( u S _ { 0 } - K ) ^ { + } , ( d S _ { 0 } - K ) ^ { + }$ , or $( S _ { 0 } - K ) ^ { + }$ . If one could replicate this outcome by buying and selling shares of the stock, then the “no arbitrage” rule would give the exact value of the call option in this model. But, except in very special circumstances, one cannot do this, and the theory falls apart. One has three equations one wants to satisfy, in terms of $V _ { 1 } ^ { u } , \ V _ { 1 } ^ { d } .$ , and $V _ { 1 } ^ { c }$ . (The $^ { 6 6 } c ^ { 9 }$ is a mnemonic for “constant.”) There are however only two variables, $\Delta _ { 0 }$ and $V _ { 0 }$ at your disposal, and most of the time three equations in two unknowns cannot be solved. 

Remark 6.6. In our model we ruled out the cases that $P$ or $Q$ were zero. If $Q = 0$ that is, we are certain that the stock will go up, then we would always invest in the stock if $u > 1 + r$ , as we would always do better, and we would always put the money in the bank if $u \leq 1 + r$ . Similar considerations apply when $P = 0$ . It is interesting to note that the cases where P = 0 or Q = 0 are the only ones in which our derivation is not valid. It turns out that in more general models the true probabilities enter only in determining which events have probability 0 or 1 and in no other way. 

## 7. The multi-step binomial asset pricing model.

In this section we will obtain a formula for the pricing of options when there are n time steps, but each time the stock can only go up by a factor u or down by a factor d. The “Black-Scholes” formula we will obtain is already a nontrivial result that is useful. 

We assume the following. 

(1) Unlimited short selling of stock 

(2) Unlimited borrowing 

(3) No transaction costs 

(4) Our buying and selling is on a small enough scale that it does not afect the market. 

We need to set up the probability model. Ω will be all sequences of length n of $H \ '$ s and $T \mathrm { { s . } } \ S _ { 0 }$ will be a fixed number and we define $S _ { k } ( \omega ) = u ^ { j } d ^ { k - j } S _ { 0 }$ if the first k elements of a given $\omega \in \Omega$ has $j$ occurrences of $H$ and $k - j$ occurrences of $T .$ . (What we are doing is saying that if the $j \mathrm { - t h }$ element of the sequence making up $\omega$ is an $H$ , then the stock price goes up by a factor u; if $T$ , then down by a factor d.) $\mathcal { F } _ { k }$ will be the σ-field generated by $S _ { 0 } , \ldots , S _ { k }$ 

Let 

$$
\overline {{p}} = \frac {(1 + r) - d}{u - d}, \quad \overline {{q}} = \frac {u - (1 + r)}{u - d}
$$

and define $\overline { { \mathbb { P } } } ( \omega ) = \overline { { p } } ^ { j } \overline { { q } } ^ { n - j } \mathrm { ~ i f ~ } \omega$ has $j$ appearances of $H$ and $n - j$ appearances of $T .$ . We observe that under $\overline { { \mathbb { P } } }$ the random variables $S _ { k + 1 } / S _ { k }$ are independent and equal to u with probability $\overline { { p } }$ and d with probability ${ \overline { { q } } } .$ To see this, let $Y _ { k } = { S _ { k } } / { S _ { k - 1 } }$ . Thus $Y _ { k }$ is the factor the stock price goes up or down at time $k .$ . Then $\mathbb { P } ( Y _ { 1 } = y _ { 1 } , \dots , Y _ { n } = y _ { n } ) = { \overline { { p } } } ^ { j } { \overline { { q } } } ^ { n - j }$ where $j$ is the number of the $y _ { k }$ that are equal to $u .$ . On the other hand, this is equal to $\mathbb { P } ( Y _ { 1 } = y _ { 1 } ) \cdot \cdot \cdot \mathbb { P } ( Y _ { n } = y _ { n } )$ . Let $\overline { { \mathbb { E } } }$ denote the expectation corresponding to $\overline { { \mathbb { P } } } .$ . 

The $\overline { { \mathbb { P } } }$ we construct may not be the true probabilities of going up or down. That doesn’t matter - it will turn out that using the principle of “no arbitrage,” it is $\overline { { \mathbb { P } } }$ that governs the price. 

Our first result is the fundamental theorem of finance in the current context. 

Proposition 7.1. Under $\overline { { \mathbb { P } } }$ the discounted stock price $( 1 + r ) ^ { - k } S _ { k }$ is a martingale. 

Proof. Since the random variable $S _ { k + 1 } / S _ { k }$ is independent of $\mathcal { F } _ { k }$ , we have 

$$
\overline {{\mathbb {E}}} [ (1 + r) ^ {- (k + 1)} S _ {k + 1} \mid \mathcal {F} _ {k} ] = (1 + r) ^ {- k} S _ {k} (1 + r) ^ {- 1} \overline {{\mathbb {E}}} [ S _ {k + 1} / S _ {k} \mid \mathcal {F} _ {k} ].
$$

Using the independence the conditional expectation on the right is equal to 

$$
\overline {{\mathbb {E}}} [ S _ {k + 1} / S _ {k} ] = \overline {{p}} u + \overline {{q}} d = 1 + r.
$$

Substituting yields the proposition. 

Let $\Delta _ { k }$ be the number of shares held between times $k$ and $k + 1$ . We require $\Delta _ { k }$ to be $\mathcal { F } _ { k }$ measurable. $\Delta _ { 0 } , \Delta _ { 1 } , \ldots$ . is called the portfolio process. Let $W _ { 0 }$ be the amount of money you start with and let $W _ { k }$ be the amount of money you have at time k. $W _ { k }$ is the wealth process. If we have $\Delta _ { k }$ shares between times $k$ and $k + 1$ , then at time $k + 1$ those shares will be worth $\Delta _ { k } S _ { k + 1 }$ . The amount of cash we hold between time k and $k + 1$ is $W _ { k }$ minus the amount held in stock, that is, $W _ { k } - \Delta _ { k } S _ { k }$ . At time $k + 1$ this is worth $( 1 + r ) [ W _ { k } - \Delta _ { k } S _ { k } ]$ . Therefore 

$$
W _ {k + 1} = \Delta_ {k} S _ {k + 1} + (1 + r) [ W _ {k} - \Delta_ {k} S _ {k} ].
$$

Note that in the case where $r = 0$ we have 

$$
W _ {k + 1} - W _ {k} = \Delta_ {k} (S _ {k + 1} - S _ {k}),
$$

or 

$$
W _ {k + 1} = W _ {0} + \sum_ {i = 0} ^ {k} \Delta_ {i} (S _ {i + 1} - S _ {i}).
$$

This is a discrete version of a stochastic integral. Since 

$$
\overline {{\mathbb {E}}} [ W _ {k + 1} - W _ {k} \mid \mathcal {F} _ {k} ] = \Delta_ {k} \overline {{\mathbb {E}}} [ S _ {k + 1} - S _ {k} \mid \mathcal {F} _ {k} ] = 0,
$$

it follows that in the case $r = 0$ that $W _ { k }$ is a martingale. More generally 

Proposition 7.2. Under $\overline { { \mathbb { P } } }$ the discounted wealth process $( 1 + r ) ^ { - k } W _ { k }$ is a martingale. 

Proof. We have 

$$
(1 + r) ^ {- (k + 1)} W _ {k + 1} = (1 + r) ^ {- k} W _ {k} + \Delta_ {k} [ (1 + r) ^ {- (k + 1)} S _ {k + 1} - (1 + r) ^ {- k} S _ {k} ].
$$

Observe that 

$$
\begin{array}{r l} & {\overline {{\mathbb {E}}} [ \Delta_ {k} [ (1 + r) ^ {- (k + 1)} S _ {k + 1} - (1 + r) ^ {- k} S _ {k} | \mathcal {F} _ {k} ]} \\ & {\qquad = \Delta_ {k} \overline {{\mathbb {E}}} [ (1 + r) ^ {- (k + 1)} S _ {k + 1} - (1 + r) ^ {- k} S _ {k} | \mathcal {F} _ {k} ] = 0.} \end{array}
$$

The result follows. 

Our next result is that the binomial model is complete. It is easy to lose the idea in the algebra, so first let us try to see why the theorem is true. 

For simplicity let us first consider the case $r = 0$ . Let $V _ { k } = \mathbb { E } \left[ V \mid { \mathcal { F } } _ { k } \right]$ ; by Proposition 4.3 we see that $V _ { k }$ is a martingale. We want to construct a portfolio process, i.e., choose $\Delta _ { k } { } ^ { \prime } \mathrm { s } .$ so that $W _ { n } \ = \ V$ . We will do it inductively by arranging matters so that $W _ { k } = V _ { k }$ for all k. Recall that $W _ { k }$ is also a martingale. 

Suppose we have $W _ { k } = V _ { k }$ at time k and we want to find $\Delta _ { k }$ so that $W _ { k + 1 } = V _ { k + 1 }$ At the $( k + 1 )$ )-st step there are only two possible changes for the price of the stock and so since $V _ { k + 1 }$ is $\mathcal { F } _ { k + 1 }$ measurable, only two possible values for $V _ { k + 1 }$ . We need to choose $\Delta _ { k }$ so that $W _ { k + 1 } = V _ { k + 1 }$ for each of these two possibilities. We only have one parameter, $\Delta _ { k } .$ to play with to match up two numbers, which may seem like an overconstrained system of equations. But both V and $W$ are martingales, which is why the system can be solved. 

Now let us turn to the details. In the following proof we allow $r \geq 0$ 

## Theorem 7.3. The binomial asset pricing model is complete.

The precise meaning of this is the following. If V is any random variable that is ${ \mathcal { F } } _ { n }$ measurable, there exists a constant $W _ { 0 }$ and a portfolio process $\Delta _ { k }$ so that the wealth process $W _ { k }$ satisfies $W _ { n } \ = \ V$ . In other words, starting with $W _ { 0 }$ dollars, we can trade shares of stock to exactly duplicate the outcome of any option V. 

Proof. Let 

$$
V _ {k} = (1 + r) ^ {k} \overline {{\mathbb {E}}} [ (1 + r) ^ {- n} V \mid \mathcal {F} _ {k} ].
$$

By Proposition $4 . 3 ~ ( 1 + r ) ^ { - k } V _ { k }$ is a martingale. If $\omega = ( t _ { 1 } , \ldots , t _ { n } )$ , where each $t _ { i }$ is an H or $T .$ , let 

$$
\Delta_ {k} (\omega) = \frac {V _ {k + 1} (t _ {1} , \ldots , t _ {k} , H , t _ {k + 2} , \ldots , t _ {n}) - V _ {k + 1} (t _ {1} , \ldots , t _ {k} , T , t _ {k + 2} , \ldots , t _ {n})}{S _ {k + 1} (t _ {1} , \ldots , t _ {k} , H , t _ {k + 2} , \ldots , t _ {n}) - S _ {k + 1} (t _ {1} , \ldots , t _ {k} , T , t _ {k + 2} , \ldots , t _ {n})}.
$$

Set $W _ { 0 } = V _ { 0 }$ , and we will show by induction that the wealth process at time k equals $V _ { k }$ The first thing to show is that $\Delta _ { k }$ is $\mathcal { F } _ { k }$ measurable. Neither $S _ { k + 1 }$ nor $V _ { k + 1 }$ depends on $t _ { k + 2 } , \ldots , t _ { n } . \ \mathrm { S o } \ \Delta _ { k }$ depends only on the variables $t _ { 1 } , \ldots , t _ { k }$ , hence is $\mathcal { F } _ { k }$ measurable. 

Now $t _ { k + 2 } , \ldots , t _ { n }$ play no role in the rest of the proof, and $t _ { 1 } , \ldots , t _ { k }$ will be fixed, so we drop the $t \mathrm { { } ^ { \circ } s }$ from the notation. If we write $V _ { k + 1 } ( H )$ , this is an abbreviation for $V _ { k + 1 } ( t _ { 1 } , \dots , t _ { k } , H , t _ { k + 2 } , \dots , t _ { n } )$ 

We know $( 1 + r ) ^ { - k } V _ { k }$ is a martingale under $\overline { { \mathbb { P } } } \operatorname { s o }$ that 

$$
\begin{array}{l} V _ {k} = \overline {{\mathbb {E}}} [ (1 + r) ^ {- 1} V _ {k + 1} \mid \mathcal {F} _ {k} ] \\ = \frac {1}{1 + r} [ \overline {{p}} V _ {k + 1} (H) + \overline {{q}} V _ {k + 1} (T) ]. \end{array}\tag{7.1}
$$

(See Note 1.) We now suppose $W _ { k } = V _ { k }$ and want to show $W _ { k + 1 } ( H ) = V _ { k + 1 } ( H )$ and $W _ { k + 1 } ( T ) = V _ { k + 1 } ( T )$ . Then using induction we have $W _ { n } = V _ { n } = V$ as required. We show the first equality, the second being similar. 

$$
\begin{array}{l} W _ {k + 1} (H) = \Delta_ {k} S _ {k + 1} (H) + (1 + r) [ W _ {k} - \Delta_ {k} S _ {k} ] \\ \qquad = \Delta_ {k} [ u S _ {k} - (1 + r) S _ {k} ] + (1 + r) V _ {k} \\ \qquad = \frac {V _ {k + 1} (H) - V _ {k + 1} (T)}{(u - d) S _ {k}} S _ {k} [ u - (1 + r) ] + \overline {{p}} V _ {k + 1} (H) + \overline {{q}} V _ {k + 1} (T) \\ \qquad = V _ {k + 1} (H). \end{array}
$$

We are done. 

Finally, we obtain the Black-Scholes formula in this context. Let $V$ be any option that is ${ \mathcal { F } } _ { n }$ -measurable. The one we have in mind is the European call, for which $V =$ $( S _ { n } - K ) ^ { + }$ , but the argument is the same for any option whatsoever. 

Theorem 7.4. The value of the option V at time 0 is $V _ { 0 } = ( 1 + r ) ^ { - n } \overline { { \mathbb { E } } } V$ 

Proof. We can construct a portfolio process $\Delta _ { k }$ so that if we start with $W _ { 0 } = ( 1 + r ) ^ { - n } \overline { { \mathbb { E } } } V$ 2 then the wealth at time n will equal $V _ { ; }$ , no matter what the market does in between. If we could buy or sell the option $V$ at a price other than $W _ { 0 }$ , we could obtain a riskless profit. That ${ \mathrm { i s } } ,$ if the option $V$ could be sold at a price $c _ { 0 }$ larger than $W _ { 0 }$ , we would sell the option for $c _ { 0 }$ dollars, use $W _ { 0 }$ to buy and sell stock according to the portfolio process $\Delta _ { k } ,$ have a net worth of $V + ( 1 + r ) ^ { n } ( c _ { 0 } - W _ { 0 } )$ ) at time $n ,$ , meet our obligation to the buyer of the option by using V dollars, and have a net profit, at no risk, of $( 1 + r ) ^ { n } ( c _ { 0 } - W _ { 0 } )$ If $c _ { 0 }$ were less than $W _ { 0 } ,$ we would do the same except buy an option, hold $- \Delta _ { k }$ shares at time $k ,$ and again make a riskless profit. By the “no arbitra $\mathrm { \Delta \ g e ^ { \gamma } }$ rule, that can’t happen, so the price of the option $V$ must be $W _ { 0 }$ □ 

Remark 7.5. Note that the proof of Theorem 7.4 tells you precisely what hedging strategy (i.e., what portfolio process) to use. 

In the binomial asset pricing model, there is no dificulty computing the price of a European call. We have 

$$
\overline {{{{\mathbb {E}}}}} (S _ {n} - K) ^ {+} = \sum_ {x} (x - K) ^ {+} \overline {{{{\mathbb {P}}}}} (S _ {n} = x)
$$

and 

$$
\overline {{\mathbb {P}}} (S _ {n} = x) = \binom{n}{k} \overline {{p}} ^ {k} \overline {{q}} ^ {n - k}
$$

if $x = u ^ { k } d ^ { n - k } S _ { 0 }$ . Therefore the price of the European call is 

$$
(1 + r) ^ {- n} \sum_ {k = 0} ^ {n} (u ^ {k} d ^ {n - k} S _ {0} - K) ^ {+} \binom{n}{k} \overline {{p}} ^ {k} \overline {{q}} ^ {n - k}.
$$

The formula in Theorem 7.4 holds for exotic options as well. Suppose 

$$
V = \max _ {i = 1, \dots , n} S _ {i} - \min _ {j = 1, \dots , n} S _ {j}.
$$

In other words, you sell the stock for the maximum value it takes during the first n time steps and you buy at the minimum value the stock takes; you are allowed to wait until time n and look back to see what the maximum and minimum were. You can even do this if the maximum comes before the minimum. This V is still ${ \mathcal { F } } _ { n }$ measurable, so the theory applies. Naturally, such a “buy low, sell high” option is very desirable, and the price of such a V will be quite high. It is interesting that even without using options, you can duplicate the operation of buying low and selling high by holding an appropriate number of shares $\Delta _ { k }$ at time $k ,$ where you do not look into the future to determine $\Delta _ { k }$ 

Let us look at an example of a European call so that it is clear how to do the calculations. Consider the binomial asset pricing model with $n = 3 , u = 2 , d = \textstyle { \frac { 1 } { 2 } } , r = 0 . 1$ $S _ { 0 } = 1 0 $ , and $K = 1 5$ . If V is a European call with strike price K and exercise date $n ,$ let us compute explicitly the random variables $V _ { 1 }$ and $V _ { 2 }$ and calculate the value $V _ { 0 }$ . Let us also compute the hedging strategy $\Delta _ { 0 } , \Delta _ { 1 }$ , and $\Delta _ { 2 }$ 

Let 

$$
\overline {{{p}}} = \frac {(1 + r) - d}{u - d} = . 4, \qquad \overline {{{q}}} = \frac {u - (1 + r)}{u - d} = . 6.
$$

The following table describes the values of the stock, the payof $V .$ and the probabilities for each possible outcome ω. 

<table><tr><td><eq>\omega</eq></td><td><eq>S_1</eq></td><td><eq>S_2</eq></td><td><eq>S_3</eq></td><td><eq>V</eq></td><td>Probability</td></tr><tr><td>HHH</td><td>10u</td><td><eq>10u^2</eq></td><td><eq>10u^3</eq></td><td>65</td><td><eq>\overline{p}^3</eq></td></tr><tr><td>HHT</td><td>10u</td><td><eq>10u^2</eq></td><td><eq>10u^2d</eq></td><td>5</td><td><eq>\overline{p}^2\overline{q}</eq></td></tr><tr><td>HTH</td><td>10u</td><td>10ud</td><td><eq>10u^2d</eq></td><td>5</td><td><eq>\overline{p}^2\overline{q}</eq></td></tr><tr><td>HTT</td><td>10u</td><td>10ud</td><td><eq>10ud^2</eq></td><td>0</td><td><eq>\overline{pq}^2</eq></td></tr><tr><td>THH</td><td>10d</td><td>10ud</td><td><eq>10u^2d</eq></td><td>5</td><td><eq>\overline{p}^2\overline{q}</eq></td></tr><tr><td>THT</td><td>10d</td><td>10ud</td><td><eq>10ud^2</eq></td><td>0</td><td><eq>\overline{pq}^2</eq></td></tr><tr><td>TTH</td><td>10d</td><td><eq>10d^2</eq></td><td><eq>10ud^2</eq></td><td>0</td><td><eq>\overline{pq}^2</eq></td></tr><tr><td>TTT</td><td>10d</td><td><eq>10d^2</eq></td><td><eq>10d^3</eq></td><td>0</td><td><eq>\overline{q}^3</eq></td></tr></table>


We then calculate 


$$
V _ {0} = (1 + r) ^ {- 3} \overline {{\mathbb {E}}} V = (1 + r) ^ {- 3} (6 5 \overline {{p}} ^ {3} + 1 5 \overline {{p}} ^ {2} \overline {{q}}) = 4. 2 0 7 4.
$$

$V _ { 1 } = ( 1 + r ) ^ { - 2 } \overline { { \mathbb { E } } } \left[ V \mid \mathcal { F } _ { 1 } \right] ,$ , so we have 

$$
V _ {1} (H) = (1 + r) ^ {- 2} (6 5 \overline {{p}} ^ {2} + 1 0 \overline {{p q}}) = 1 0. 5 7 8 5, \qquad V _ {1} (T) = (1 + r) ^ {- 2} 5 \overline {{p q}} = . 9 9 1 7.
$$

$V _ { 2 } = ( 1 + r ) ^ { - 1 } \overline { { \mathbb { E } } } \left[ V \mid \mathcal { F } _ { 2 } \right]$ , so we have 

$$
\begin{array}{c c} V _ {2} (H H) = (1 + r) ^ {- 1} (6 5 \overline {{p}} + 5 \overline {{q}}) = 2 4. 5 4 5 4, & V _ {2} (H T) = (1 + r) ^ {- 1} 5 \overline {{p}} = 1. 8 1 8 2, \\ V _ {2} (T H) = (1 + r) ^ {- 1} 5 \overline {{p}} = 1. 8 1 8 2, & V _ {2} (T T) = 0. \end{array}
$$

The formula for $\Delta _ { k }$ is given by 

$$
\Delta_ {k} = \frac {V _ {k + 1} (H) - V _ {k + 1} (T)}{S _ {k + 1} (H) - S _ {k + 1} (T)},
$$

so 

$$
\Delta_ {0} = \frac {V _ {1} (H) - V _ {1} (T)}{S _ {1} (H) - S _ {1} (T)} = . 6 3 9 1,
$$

where $V _ { 1 }$ and $S _ { 1 }$ are as above. 

$$
\Delta_ {1} (H) = \frac {V _ {2} (H H) - V _ {2} (H T)}{S _ {2} (H H) - S _ {2} (H T)} = . 7 5 7 6, \quad \Delta_ {1} (T) = \frac {V _ {2} (T H) - V _ {2} (T T)}{S _ {2} (T H) - S _ {2} (T T)} = . 2 4 2 4.
$$

$$
\Delta_ {2} (H H) = \frac {V _ {3} (H H H) - V _ {3} (H H T)}{S _ {3} (H H H) - S _ {3} (H H T)} = 1. 0,
$$

$$
\Delta_ {2} (H T) = \frac {V _ {3} (H T H) - V _ {3} (H T T)}{S _ {3} (H T H) - S _ {3} (H T T)} = . 3 3 3 3,
$$

$$
\Delta_ {2} (T H) = \frac {V _ {3} (T H H) - V _ {3} (T H T)}{S _ {3} (T H H) - S _ {3} (T H T)} = . 3 3 3 3,
$$

$$
\Delta_ {2} (T T) = \frac {V _ {3} (T T H) - V _ {3} (T T T)}{S _ {3} (T T H) - S _ {3} (T T T)} = 0. 0.
$$

Note 1. The second equality is (7.1) is not entirely obvious. Intuitively, it says that one has a heads with probability $\overline { { p } }$ and the value of $V _ { k + 1 }$ is $V _ { k + 1 } ( H )$ and one has tails with probability ${ \overline { { q } } } ,$ and the value of $V _ { k + 1 }$ is $V _ { k + 1 } ( T )$ 

Let us give a more rigorous proof of (7.1). The right hand side of (7.1) is $\mathcal { F } _ { k }$ measurable, so we need to show that if $A \in \mathcal { F } _ { k }$ , then 

$$
\overline {{\mathbb {E}}} [ V _ {k + 1}; A ] = \overline {{\mathbb {E}}} [ \bar {p} V _ {k + 1} (H) + \bar {q} V _ {k + 1} (T); A ].
$$

By linearity, it sufices to show this for $A = \{ \omega = ( t _ { 1 } t _ { 2 } \cdot \cdot \cdot t _ { n } ) : t _ { 1 } = s _ { 1 } , \ldots , t _ { k } = s _ { k } \}$ , where $s _ { 1 } s _ { 2 } \cdots s _ { k }$ is any sequence of $H \thinspace s$ and $T ' \mathsf { s }$ . Now 

$$
\begin{array}{r l} & {\overline {{\mathbb {E}}} [ V _ {k + 1}; s _ {1} \dots s _ {k} ] = \overline {{\mathbb {E}}} [ V _ {k + 1}; s _ {1} \dots s _ {k} H ] + \overline {{\mathbb {E}}} [ V _ {k + 1}; s _ {1} \dots s _ {k} T ]} \\ & {\qquad = V _ {k + 1} (s _ {1} \dots s _ {k} H) \overline {{\mathbb {P}}} (s _ {1} \dots s _ {k} H) + V _ {k + 1} (s _ {1} \dots s _ {k} T) \overline {{\mathbb {P}}} (s _ {1} \dots s _ {k} T).} \end{array}
$$

By independence this is 

$$
V _ {k + 1} (s _ {1} \dots s _ {k} H) \overline {{\mathbb {P}}} (s _ {1} \dots s _ {k}) \overline {{p}} + V _ {k + 1} (s _ {1} \dots s _ {k} T) \overline {{\mathbb {P}}} (s _ {1} \dots s _ {k}) \overline {{q}},
$$

which is what we wanted. 

## 8. American options.

An American option is one where you can exercise the option any time before some fixed time T. For example, on a European call, one can only use it to buy a share of stock at the expiration time $T ,$ while for an American call, at any time before time $T ,$ one can decide to pay K dollars and obtain a share of stock. 

Let us give an informal argument on how to price an American call, giving a more rigorous argument in a moment. One can always wait until time $T$ to exercise an American call, so the value must be at least as great as that of a European call. On the other hand, suppose you decide to exercise early. You pay $K$ dollars, receive one share of stock, and your wealth is $S _ { t } - K$ . You hold onto the stock, and at time $T$ you have one share of stock worth $S _ { T }$ , and for which you paid $K$ dollars. So your wealth is $S _ { T } - K \le ( S _ { T } - K ) ^ { + }$ . In fact, we have strict inequality, because you lost the interest on your $K$ dollars that you would have received if you had waited to exercise until time $T .$ . Therefore an American call is worth no more than a European call, and hence its value must be the same as that of a European call. 

This argument does not work for puts, because selling stock gives you some money on which you will receive interest, so it may be advantageous to exercise early. (A put is the option to sell a stock at a price K at time T.) 

Here is the more rigorous argument. Suppose that if you exercise the option at time $k ,$ your payof is $g ( S _ { k } )$ . In present day dollars, that is, after correcting for inflation, you have $( 1 + r ) ^ { - k } g ( S _ { k } )$ . You have to make a decision on when to exercise the option, and that decision can only be based on what has already happened, not on what is going to happen in the future. In other words, we have to choose a stopping time $\tau ,$ and we exercise the option at time $\tau ( \omega )$ . Thus our payof is $( 1 + r ) ^ { - \tau } g ( S _ { \tau } )$ . This is a random quantity. What we want to do is find the stopping time that maximizes the expected value of this random variable. As usual, we work with ${ \overline { { \mathbb { P } } } } ,$ and thus we are looking for the stopping time $\tau$ such that $\tau \leq n$ and 

$$
\overline {{\mathbb {E}}} (1 + r) ^ {- \tau} g (S _ {\tau})
$$

is as large as possible. The problem of finding such a $\tau$ is called an optimal stopping problem. 

Suppose $g ( x )$ is convex with $g ( 0 ) = 0$ . Certainly $g ( x ) = ( x - K ) ^ { + }$ is such a function. We will show that $\tau \equiv n$ is the solution to the above optimal stopping problem: the best time to exercise is as late as possible. 

We have 

$$
g (\lambda x) = g (\lambda x + (1 - \lambda) \cdot 0) \leq \lambda g (x) + (1 - \lambda) g (0) = \lambda g (x), \quad 0 \leq \lambda \leq 1.\tag{8.1}
$$

By Jensen’s inequality, 

$$
\begin{array}{r l} & {\overline {{\mathbb {E}}} \big [ (1 + r) ^ {- (k + 1)} g (S _ {k + 1}) \mid \mathcal {F} _ {k} \big ] = (1 + r) ^ {- k} \overline {{\mathbb {E}}} \Big [ \frac {1}{1 + r} g (S _ {k + 1}) \mid \mathcal {F} _ {k} \Big ]} \\ & {\qquad \geq (1 + r) ^ {- k} \overline {{\mathbb {E}}} \Big [ g \Big (\frac {1}{1 + r} S _ {k + 1} \Big) \mid \mathcal {F} _ {k} \Big ]} \\ & {\qquad \geq (1 + r) ^ {- k} g \Big (\overline {{\mathbb {E}}} \Big [ \frac {1}{1 + r} S _ {k + 1} \mid \mathcal {F} _ {k} \Big ] \Big)} \\ & {\qquad = (1 + r) ^ {- k} g (S _ {k}).} \end{array}
$$

For the first inequality we used (8.1). So $( 1 + r ) ^ { - k } g ( S _ { k } )$ is a submartingale. By optional stopping, 

$$
\overline {{\mathbb {E}}} [ (1 + r) ^ {- \tau} g (S _ {\tau}) ] \leq \overline {{\mathbb {E}}} [ (1 + r) ^ {- n} g (S _ {n}) ],
$$

so $\tau \equiv n$ always does best. 

For puts, the payof is $g ( S _ { k } )$ , where $g ( x ) = ( K - x ) ^ { + }$ . This is also convex function, but this time $g ( 0 ) \neq 0$ , and the above argument fails. 

Although good approximations are known, an exact solution to the problem of valuing an American put is unknown, and is one of the major unsolved problems in financial mathematics. 

## 9. Continuous random variables.

We are now going to start working toward continuous times and stocks that can take any positive number as a value, so we need to prepare by extending some of our definitions. 

Given any random variable $X \geq 0$ , we can approximate it by $\operatorname { r } . \operatorname { v } ^ { \ } \mathrm { s } \ X _ { n }$ that are discrete. We let 

$$
X _ {n} = \sum_ {i = 0} ^ {n 2 ^ {n}} \frac {i}{2 ^ {n}} 1 _ {(i / 2 ^ {n} \leq X <   (i + 1) / 2 ^ {n})}.
$$

In words, if $X ( \omega )$ lies between 0 and n, we let $X _ { n } ( \omega )$ be the closest value $i / 2 ^ { n }$ that is less than or equal to $X ( \omega )$ . For $\omega$ where $X ( \omega ) > n + 2 ^ { - n }$ we set $X _ { n } ( \omega ) = 0$ . Clearly the $X _ { n }$ are discrete, and approximate X. In fact, on the set where $X \leq n ,$ , we have that $| X ( \omega ) - X _ { n } ( \omega ) | \leq 2 ^ { - n }$ 

For reasonable $X$ we are going to define $\mathbb { E } X = \operatorname* { l i m } \mathbb { E } X _ { n }$ . Since the $X _ { n }$ increase with $n ,$ the limit must exist, although it could be $+ \infty$ . If X is not necessarily nonnegative, we define E $X = \mathbb { E } X ^ { + } - \mathbb { E } X ^ { - }$ , provided at least one of $\mathbb { E } X ^ { + }$ and E $X ^ { - }$ is finite. Here $X ^ { + } = \operatorname* { m a x } ( X , 0 )$ and $X ^ { - } = \operatorname* { m a x } ( - X , 0 )$ 

There are some things one wants to prove, but all this has been worked out in measure theory and the theory of the Lebesgue integral; see Note 1. Let us confine ourselves here to showing this definition is the same as the usual one when X has a density. 

Recall X has a density $f _ { X }$ if 

$$
\mathbb {P} (X \in [ a, b ]) = \int_ {a} ^ {b} f _ {X} (x) d x
$$

for all a and b. In this case 

$$
\mathbb {E} X = \int_ {- \infty} ^ {\infty} x f _ {X} (x) d x
$$

provided $\textstyle \int _ { - \infty } ^ { \infty } | x | f _ { X } ( x ) d x < \infty$ . With our definition of $X _ { n }$ we have 

$$
\mathbb {P} (X _ {n} = i / 2 ^ {n}) = \mathbb {P} (X \in [ i / 2 ^ {n}, (i + 1) / 2 ^ {n})) = \int_ {i / 2 ^ {n}} ^ {(i + 1) / 2 ^ {n}} f _ {X} (x) d x.
$$

Then 

$$
\mathbb {E} X _ {n} = \sum_ {i} \frac {i}{2 ^ {n}} \mathbb {P} (X _ {n} = i / 2 ^ {n}) = \sum_ {i} \int_ {i / 2 ^ {n}} ^ {(i + 1) / 2 ^ {n}} \frac {i}{2 ^ {n}} f _ {X} (x) d x.
$$

Since x difers from $i / 2 ^ { n }$ by at most $1 / 2 ^ { n }$ when $x \in [ i / 2 ^ { n } , ( i + 1 ) / 2 ^ { n } )$ , this will tend to $\textstyle \int x f _ { X } ( x ) d$ x, unless the contribution to the integral for $| x | \geq n$ does not $\mathrm { g o }$ to 0 as $n \to \infty$ As long as $\textstyle \int | x | f _ { X } ( x ) d x < \infty$ , one can show that this contribution does indeed $\mathrm { g o }$ to 0. 

We also need an extension of the definition of conditional probability. A r.v. is $\mathcal { G }$ measurable if $( X > a ) \in { \mathcal { G } }$ for every a. How do we define E $[ Z \mid { \mathcal { G } } ]$ when $\mathcal { G }$ is not generated by a countable collection of disjoint sets? 

Again, there is a completely worked out theory that holds in all cases; see Note 2. Let us give a definition that is equivalent that works except for a very few cases. Let us suppose that for each n the σ-field ${ \mathcal { G } } _ { n }$ is finitely generated. This means that ${ \mathcal { G } } _ { n }$ is generated by finitely many disjoint sets $B _ { n 1 } , \ldots , B _ { n m _ { n } }$ . So for each $n ,$ the number of $B _ { n i }$ is finite but arbitrary, the $B _ { n i }$ are disjoint, and their union is $\Omega .$ . Suppose also that $\mathcal { G } _ { 1 } \subset \mathcal { G } _ { 2 } \subset \cdots$ ·. Now $\cup _ { n } \mathcal { G } _ { n }$ will not in general be a $\sigma { - } \mathrm { f i e l d }$ , but suppose $\mathcal { G }$ is the smallest σ-field that contains all the ${ \mathcal { G } } _ { n }$ . Finally, define $\mathbb { P } ( A \mid { \mathcal { G } } ) = \operatorname* { l i m } \mathbb { P } ( A \mid { \mathcal { G } } _ { n } )$ 

This is a fairly general set-up. For example, let Ω be the real line and let ${ \mathcal { G } } _ { n }$ be generated by the sets $( - \infty , n ) , [ n , \infty )$ and $[ i / 2 ^ { n } , ( i + 1 ) / 2 ^ { n } )$ . Then $\mathcal { G }$ will contain every interval that is closed on the left and open on the right, hence $\mathcal { G }$ must be the σ-field that one works with when one talks about Lebesgue measure on the line. 

The question that one might ask is: how does one know the limit exists? Since the ${ \mathcal { G } } _ { n }$ increase, we know by Proposition 4.3 that $M _ { n } = \mathbb { P } ( A \mid { \mathcal { G } } _ { n } )$ is a martingale with respect to the ${ \mathcal { G } } _ { n }$ . It is certainly bounded above by 1 and bounded below by $0 ,$ so by the martingale convergence theorem, it must have a limit as $n \to \infty$ 

Once one has a definition of conditional probability, one defines conditional expectation by what one expects. If X is discrete, one can write $X$ as $\textstyle \sum _ { j } a _ { j } 1 _ { A _ { j } }$ and then one defines 

$$
\mathbb {E} \left[ X \mid \mathcal {G} \right] = \sum_ {j} a _ {j} \mathbb {P} (A _ {j} \mid \mathcal {G}).
$$

If the X is not discrete, one write $X = X ^ { + } - X$ <sup>−</sup>, one approximates $X ^ { + }$ by discrete random variables, and takes a limit, and similarly for $X ^ { - }$ . One has to worry about convergence, but everything does go through. 

With this extended definition of conditional expectation, do all the properties of Section 2 hold? The answer is yes. See Note 2 again. 

With continuous random variables, we need to be more cautious about what we mean when we say two random variables are equal. We say $X = Y$ almost surely, abbreviated “a.s.”, if 

$$
\mathbb {P} (\{\omega : X (\omega) \neq Y (\omega) \}) = 0.
$$

So $X = Y$ except for a set of probability 0. The a.s. terminology is used other places as well: $X _ { n }  Y$ a.s. means that except for a set of $\omega \mathrm { { s } }$ of probability zero, $X _ { n } ( \omega )  Y ( \omega )$ 

Note 1. The best way to define expected value is via the theory of the Lebesgue integral. A probability $\mathbb { P }$ is a measure that has total mass 1. So we define 

$$
\mathbb {E} X = \int X (\omega) \mathbb {P} (d \omega).
$$

To recall how the definition goes, we say $X$ is simple if $\begin{array} { r } { X ( \omega ) = \sum _ { i = 1 } ^ { m } a _ { i } 1 _ { A _ { i } } ( \omega ) } \end{array}$ with each $a _ { i } \geq 0$ , and for a simple X we define 

$$
\mathbb {E} X = \sum_ {i = 1} ^ {m} a _ {i} \mathbb {P} (A _ {i}).
$$

If X is nonnegative, we define 

$$
\mathbb {E} X = \sup \{\mathbb {E} Y: Y \text {   simple   }, Y \leq X \}.
$$

Finally, provided at least one of E $X ^ { + }$ and $\mathbb { E } X ^ { - }$ is finite, we define 

$$
\mathbb {E} X = \mathbb {E} X ^ {+} - \mathbb {E} X ^ {-}.
$$

This is the same definition as described above. 

Note 2. The Radon-Nikodym theorem from measure theory says that if $\mathbb { Q }$ and $\mathbb { P }$ are two finite measures on $( \Omega , { \mathcal { G } } )$ and $\mathbb { Q } ( A ) = 0$ whenever $\mathbb { P } ( A ) = 0$ and $A \in { \mathcal { G } }$ , then there exists an integrable function $Y$ that is G-measurable such that $\textstyle \mathbb { Q } ( A ) = \int _ { A } Y d \mathbb { P }$ for every measurable set A. 

Let us apply the Radon-Nikodym theorem to the following situation. Suppose $( \Omega , { \mathcal { F } } , \mathbb { P } )$ is a probability space and $X \geq 0$ is integrable: $\mathbb { E } X < \infty$ . Suppose $\mathcal { G } \subset \mathcal { F }$ . Define two new probabilities on $\mathcal { G }$ as follows. Let $\mathbb { P } ^ { \prime } = \mathbb { P } | _ { \mathcal { G } }$ , that is, $\mathbb { P } ^ { \prime } ( A ) = \mathbb { P } ( A ) { \mathrm { ~ i f ~ } } A \in { \mathcal { G } }$ and $\mathbb { P } ^ { \prime } ( A )$ is not defined if $A \in { \mathcal { F } } - { \mathcal { G } }$ . Define $\mathbb { Q }$ by $\begin{array} { r } { \mathbb { Q } ( A ) = \int _ { A } X d \mathbb { P } = \mathbb { E } \left[ X ; A \right] \mathsf { i } \mathsf { f } \ A \in \mathcal { G } } \end{array}$ . One can show (using the monotone convergence theorem from measure theory) that $\mathbb { Q }$ is a finite measure on ${ \mathcal { G } } .$ (One can also use this definition to define $\mathbb { Q } ( A )$ for $A \in { \mathcal { F } }$ , but we only want to define $\mathbb { Q }$ on ${ \mathcal { G } } ,$ , as we will see in a moment.) So $\mathbb { Q }$ and $\mathbb { P } ^ { \prime }$ are two finite measures on $( \Omega , { \mathcal { G } } )$ . If $A \in { \mathcal { G } }$ and $\mathbb { P } ^ { \prime } ( A ) = 0$ , then $\mathbb { P } ( A ) = 0$ and so it follows that $\mathbb { Q } ( A ) = 0$ . By the Radon-Nikodym theorem there exists an integrable random variable $Y$ such that Y is $\mathcal { G }$ measurable (this is why we worried about which σ-field we were working with) and 

$$
\mathbb {Q} (A) = \int_ {A} Y d \mathbb {P} ^ {\prime}
$$

if $A \in { \mathcal { G } }$ . Note 

((a) $Y$ is $\mathcal { G }$ measurable, and 

(b) if $A \in { \mathcal { G } }$ 

$$
\mathbb {E} \left[ Y; A \right] = \mathbb {E} \left[ X; A \right]
$$

because 

$$
\mathbb {E} \left[ Y; A \right] = \mathbb {E} \left[ Y 1 _ {A} \right] = \int_ {A} Y d \mathbb {P} = \int_ {A} Y d \mathbb {P} ^ {\prime} = \mathbb {Q} (A) = \int_ {A} X d \mathbb {P} = \mathbb {E} \left[ X 1 _ {A} \right] = \mathbb {E} \left[ X; A \right].
$$

We define $\mathbb { E } \left[ X \mid { \mathcal { G } } \right]$ to be the random variable Y. If X is integrable but not necessarily nonnegative, then X<sup>+</sup> and X<sup>−</sup> will be integrable and we define 

$$
\mathbb {E} \left[ X \mid \mathcal {G} \right] = \mathbb {E} \left[ X ^ {+} \mid \mathcal {G} \right] - \mathbb {E} \left[ X ^ {-} \mid \mathcal {G} \right].
$$

We define 

$$
\mathbb {P} (B \mid \mathcal {G}) = \mathbb {E} \left[ 1 _ {B} \mid \mathcal {G} \right]
$$

if $B \in { \mathcal { F } } .$ 

Let us show that there is only one r.v., up to almost sure equivalence, that satisfies (a) and (b) above. If Y and $Z$ are $\mathcal { G }$ measurable, and $\operatorname { \mathbb { E } } \left[ Y ; A \right] = \operatorname { \mathbb { E } } \left[ X ; A \right] = \operatorname { \mathbb { E } } \left[ Z ; A \right]$ for $A \in { \mathcal { G } }$ then the set $A _ { n } = ( Y > Z + { \frac { 1 } { n } } )$ will be in $\mathcal { G }$ , and so 

$$
\mathbb {E} \left[ Z; A _ {n} \right] + \frac {1}{n} \mathbb {P} (A _ {n}) = \mathbb {E} \left[ Z + \frac {1}{n}; A _ {n} \right] \leq \mathbb {E} \left[ Y; A _ {n} \right] = \mathbb {E} \left[ Z; A _ {n} \right].
$$

Consequently $\mathbb { P } ( A _ { n } ) = 0$ . This is true for each positive integer n, so $\mathbb { P } ( Y > Z ) = 0$ . By symmetry, $\mathbb { P } ( Z > Y ) = 0$ , and therefore $\mathbb { P } ( Y \neq Z ) = 0$ as we wished. 

If one checks the proofs of Propositions 2.3, 2.4, and 2.5, one sees that only properties (a) and (b) above were used. So the propositions hold for the new definition of conditional expectation as well. 

In the case where $\mathcal { G }$ is finitely or countably generated, under both the new and old definitions (a) and (b) hold. By the uniqueness result, the new and old definitions agree. 

## 10. Stochastic processes.

We will be talking about stochastic processes. Previously we discussed sequences $S _ { 1 } , S _ { 2 } , . . .$ . of $\mathrm { r . v . \dot { s } }$ . Now we want to talk about processes $Y _ { t }$ for $t \geq 0$ . For example, we can think of $S _ { t }$ being the price of a stock at time t. Any nonnegative time t is allowed. 

We typically let $\mathcal { F } _ { t }$ be the smallest σ-field with respect to which $Y _ { s }$ is measurable for all $s \leq t .$ . So $\mathcal { F } _ { t } = \sigma ( Y _ { s } : s \le t )$ . As you might imagine, there are a few technicalities one has to worry about. We will try to avoid thinking about them as much as possible, but see Note 1. 

We call a collection of σ-fields $\mathcal { F } _ { t }$ with $\mathcal { F } _ { s } \subset \mathcal { F } _ { t }$ if $s < t \mathrm { ~ a ~ }$ filtration. We say the filtration satisfies the “usual conditions” if the $\mathcal { F } _ { t }$ are right continuous and complete (see Note 1); all the filtrations we consider will satisfy the usual conditions. 

We say a stochastic process has continuous paths if the following holds. For each $\omega ,$ the map $t \to Y _ { t } ( \omega )$ defines a function from $[ 0 , \infty )$ to R. If this function is a continuous function for all ω’s except for a set of probability zero, we say $Y _ { t }$ has continuous paths. 

Definition 10.1. A mapping $\tau : \Omega \to [ 0 , \infty )$ is a stopping time if for each t we have 

$$
(\tau \leq t) \in \mathcal {F} _ {t}.
$$

Typically, τ will be a continuous random variable and $\mathbb { P } ( \tau = t ) = 0$ for each $t ,$ which is why we need a definition just a bit diferent from the discrete case. 

Since $\begin{array} { r } { ( \tau < t ) = \cup _ { n = 1 } ^ { \infty } ( \tau \leq t - \frac { 1 } { n } ) } \end{array}$ and $( \tau \leq t - \frac { 1 } { n } ) \in \mathcal { F } _ { t - \frac { 1 } { n } } \subset \mathcal { F } _ { t }$ , then for a stopping time τ we have $( \tau < t ) \in \mathcal { F } _ { t }$ for all t. 

Conversely, suppose τ is a nonnegative r.v. for which $( \tau < t ) \in \mathcal { F } _ { t }$ for all t. We claim τ is a stopping time. The proof is easy, but we need the right continuity of the $\mathcal { F } _ { t }$ here, so we put the proof in Note 2. 

A continuous time martingale (or submartingale) is what one expects: each $M _ { t }$ is integrable, each $M _ { t }$ is $\mathcal { F } _ { t }$ measurable, and if $s < t ,$ , then 

$$
\mathbb {E} \left[ M _ {t} \mid \mathcal {F} _ {s} \right] = M _ {s}.
$$

(Here we are saying the left hand side and the right hand side are equal almost surely; we will usually not write the “a.s.” since almost all of our equalities for random variables are only almost surely.) 

The analogues of Doob’s theorems go through. Note 3 has the proofs. 

Note 1. For technical reasons, one typically defines $\mathcal { F } _ { t }$ as follows. Let $\mathcal { F } _ { t } ^ { 0 } = \sigma ( Y _ { s } : s \leq t )$ This is what we referred to as $\mathcal { F } _ { t }$ above. Next add to $\mathcal { F } _ { t } ^ { 0 }$ all sets $N$ for which $\mathbb { P } ( N ) = 0$ . Such sets are called null sets, and since they have probability 0, they don’t afect anything. In fact, one wants to add all sets N that we think of being null sets, even though they might not be measurable. To be more precise, we say $N$ is a null set if $\operatorname* { i n f } \{ \mathbb { P } ( A ) : A \in { \mathcal { F } } , N \subset A \} = 0$ Recall we are starting with a σ-field $\mathcal { F }$ and all the $\mathcal { F } _ { t } ^ { 0 } { \mathrm { : } }$ are contained in ${ \mathcal F } .$ Let $\mathcal { F } _ { t } ^ { 0 0 }$ be the $\sigma -$ field generated by $\mathcal { F } _ { t } ^ { 0 }$ and all null sets $N _ { \ast }$ , that is, the smallest $\sigma \cdot$ -field containing $\mathcal { F } _ { t } ^ { 0 }$ and every null set. In measure theory terminology, what we have done is to say $\mathcal { F } _ { t } ^ { 0 0 }$ is the completion of $\mathcal { F } _ { t } ^ { 0 }$ 

Lastly, we want to make our $\sigma \cdot$ -fields right continuous. We set $\mathcal { F } _ { t } = \cap _ { \varepsilon > 0 } \mathcal { F } _ { t + \varepsilon } ^ { 0 0 }$ . Although the union of σ-fields is not necessarily a σ-field, the intersection of σ-fields is. $\mathcal { F } _ { t }$ contains $\mathcal { F } _ { t } ^ { 0 0 }$ but might possibly contain more besides. An example of an event that is in $\mathcal { F } _ { t }$ but that may not be in $\mathcal { F } _ { t } ^ { 0 0 }$ is 

$$
A = \{\omega : \lim _ {n \to \infty} Y _ {t + \frac {1}{n}} (\omega) \geq 0 \}.
$$

$A \in \mathcal { F } _ { t + \frac { 1 } { m } } ^ { 0 0 }$ for each $m ,$ , so it is in $\mathcal { F } _ { t }$ . There is no reason it needs to be in $\mathcal { F } _ { t } ^ { 0 0 }$ if $Y$ is not necessarily continuous at t. It is easy to see that $\cap _ { \varepsilon > 0 } \mathcal { F } _ { t + \varepsilon } = \mathcal { F } _ { t }$ , which is what we mean when we say $\mathcal { F } _ { t }$ is right continuous. 

When talking about a stochastic process $Y _ { t }$ , there are various types of measurability one can consider. Saying $Y _ { t }$ is adapted to $\mathcal { F } _ { t }$ means $Y _ { t }$ is $\mathcal { F } _ { t }$ measurable for each t. However, since $Y _ { t }$ is really a function of two variables, t and $\omega$ , there are other notions of measurability that come into play. We will be considering stochastic processes that have continuous paths or that are predictable (the definition will be given later), so these various types of measurability will not be an issue for us. 

Note 2. Suppose $( \tau < t ) \in \mathcal { F } _ { t }$ for all t. Then for each positive integer $n _ { 0 }$ 

$$
(\tau \leq t) = \cap_ {n = n _ {0}} ^ {\infty} (\tau <   t + \frac {1}{n}).
$$

For $n \geq n _ { 0 }$ we have $\textstyle ( \tau < t + \frac { 1 } { n } ) \in \mathcal { F } _ { t + \frac { 1 } { n } } \subset \mathcal { F } _ { t + \frac { 1 } { n _ { 0 } } }$ . Therefore $( \tau \leq t ) \in \mathcal { F } _ { t + \frac { 1 } { n _ { 0 } } }$ for each $n _ { 0 }$ Hence the set is in the intersection: $\cap _ { n _ { 0 } > 1 } \mathcal { F } _ { t + \frac { 1 } { n _ { 0 } } } \stackrel { \cup } { \subset } \cap _ { \varepsilon > 0 } \mathcal { F } _ { t + \varepsilon } = \mathcal { F } _ { t }$ 

Note 3. We want to prove the analogues of Theorems 5.3 and 5.4. The proof of Doob’s inequalities are simpler. We only will need the analogue of Theorem 5.4(b). 

Theorem 10.2. Suppose $M _ { t }$ is a martingale with continuous paths and $\mathbb { E } M _ { t } ^ { 2 } < \infty$ for all t. Then for each $t _ { 0 }$ 

$$
\mathbb {E} \left[ (\sup _ {s \leq t _ {0}} M _ {s}) ^ {2} \right] \leq 4 \mathbb {E} \left[ | M _ {t _ {0}} | ^ {2} \right].
$$

Proof. By the definition of martingale in continuous time, $N _ { k }$ is a martingale in discrete time with respect to $\mathcal { G } _ { k }$ when we set $N _ { k } = M _ { k t _ { 0 } / 2 ^ { n } }$ and $\mathcal { G } _ { k } = \mathcal { F } _ { k t _ { 0 } / 2 ^ { n } }$ . By Theorem $5 . 4 ( \mathrm { b } )$ 

$$
\mathbb {E} \big [ \max _ {0 \leq k \leq 2 ^ {n}} M _ {k t _ {0} / 2 ^ {n}} ^ {2} \big ] = \mathbb {E} \big [ \max _ {0 \leq k \leq 2 ^ {n}} N _ {k} ^ {2} \big ] \leq 4 \mathbb {E}   N _ {2 ^ {n}} ^ {2} = 4 \mathbb {E}   M _ {t _ {0}} ^ {2}.
$$

(Recall $( \operatorname* { m a x } _ { k } a _ { k } ) ^ { 2 } = \operatorname* { m a x } a _ { k } ^ { 2 }$ if all the $a _ { k } \geq 0 . )$ 

Now let $n \to \infty$ . Since $M _ { t }$ has continuous paths, ma $\mathfrak { L } _ { 0 \leq k \leq 2 ^ { n } } M _ { k t _ { 0 } / 2 ^ { n } } ^ { 2 }$ increases up to $\mathrm { s u p } _ { s \leq t _ { 0 } } M _ { s } ^ { 2 }$ . Our result follows from the monotone convergence theorem from measure theory (see Note 4). □ 

We now prove the analogue of Theorem 5.3. The proof is simpler if we assume that E $M _ { t } ^ { 2 }$ is finite; the result is still true without this assumption. 

Theorem 10.3. Suppose $M _ { t }$ is a martingale with continuous paths, E $M _ { t } ^ { 2 } < \infty$ for all t, and τ is a stopping time bounded almost surely by $t _ { 0 }$ . Then E $M _ { \tau } = \mathbb { E } M _ { t _ { 0 } }$ 

Proof. We approximate τ by stopping times taking only finitely many values. For $n > 0$ define 

$$
\tau_ {n} (\omega) = \inf \left\{k t _ {0} / 2 ^ {n}: \tau (\omega) <   k t _ {0} / 2 ^ {n} \right\}.
$$

$\tau _ { n }$ takes only the values $k t _ { 0 } / 2 ^ { n }$ for some $k \leq 2 ^ { n }$ . The event $( \tau _ { n } ~ \le ~ j t _ { 0 } / 2 ^ { n } )$ is equal to $( \tau < j t _ { 0 } / 2 ^ { n } )$ , which is in $\mathcal { F } _ { j t _ { 0 } / 2 ^ { r } }$ since τ is a stopping time. So $( \tau _ { n } \leq s ) \in \mathcal { F } _ { s }$ if s is of the form $j t _ { 0 } / 2 ^ { n }$ for some $j . ~ \mathsf { A }$ moment’s thought, using the fact that $\tau _ { n }$ only takes values of the form $k t _ { 0 } / 2 ^ { n }$ , shows that $\tau _ { n }$ is a stopping time. 

It is clear that $\tau _ { n } \downarrow \tau$ for every ω. Since M has continuous paths, $M _ { \tau _ { n } }  M _ { \tau } \ \mathsf { a } . \mathsf { s }$ 

Let $N _ { k }$ and $\mathcal { G } _ { k }$ be as in the proof of Theorem 10.2. Let $\sigma _ { n } = k \ \mathrm { i f } \ \tau _ { n } = k t _ { 0 } / 2 ^ { n }$ . By Theorem 5.3, 

$$
\mathbb {E} N _ {\sigma_ {n}} = \mathbb {E} N _ {2 ^ {n}},
$$

which is the same as saying 

$$
\mathbb {E} M _ {\tau_ {n}} = \mathbb {E} M _ {t _ {0}}.
$$

To complete the proof, we need to show E $M _ { \tau _ { r } }$ converges to $\mathbb { E } M _ { \tau }$ . This is almost obvious, because we already observed that $M _ { \tau _ { n } } \ \to M _ { \tau }$ a.s. Without the assumption that E $M _ { t } ^ { 2 } < \infty$ for all t, this is actually quite a bit of work, but with the assumption it is not too bad. 

Either $| M _ { \tau _ { n } } - M _ { \tau } |$ is less than or equal to 1 or greater than 1. If it is greater than 1, it is less than $| M _ { \tau _ { n } } - M _ { \tau } | ^ { 2 }$ . So in either case, 

$$
\left| M _ {\tau_ {n}} - M _ {\tau} \right| \leq 1 + \left| M _ {\tau_ {n}} - M _ {\tau} \right| ^ {2}.\tag{10.1}
$$

Because both $| M _ { \tau _ { n } } |$ and $| M _ { \tau } |$ are bounded by $\mathrm { s u p } _ { s \leq t _ { 0 } } | M _ { s } |$ , the right hand side of (10.1) is bounded by $1 + 4 \mathrm { s u p } _ { s < t _ { 0 } } | M _ { s } | ^ { 2 }$ , which is integrable by Theorem 10.2. $| M _ { \tau _ { n } } - M _ { \tau } | \to 0$ , and so by the dominated convergence theorem from measure theory (Note 4), 

$$
\mathbb {E} \left| M _ {\tau_ {n}} - M _ {\tau} \right|\rightarrow 0.
$$

Finally, 

$$
| \mathbb {E} M _ {\tau_ {n}} - \mathbb {E} M _ {\tau} | = | \mathbb {E} (M _ {\tau_ {n}} - M _ {\tau}) | \leq \mathbb {E} | M _ {\tau_ {n}} - M _ {\tau} | \to 0.
$$

□ 

Note 4. The dominated convergence theorem says that if $X _ { n } \to X$ a.s. and $| X _ { n } | \leq Y$ a.s. for each $n ,$ , where $\mathbb { E } Y < \infty$ , then $\mathbb { E } X _ { n } \to \mathbb { E } X$ 

The monotone convergence theorem says that if $X _ { n } \geq 0$ for each $n , X _ { n } \leq X _ { n + 1 }$ for each $n ,$ and $X _ { n } \to X$ , then $\mathbb { E } X _ { n } \to \mathbb { E } X$ 

## 11. Brownian motion.

First, let us review a few facts about normal random variables. We say X is a normal random variable with mean a and variance $b ^ { 2 }$ if 

$$
\mathbb {P} (c \leq X \leq d) = \int_ {c} ^ {d} \frac {1}{\sqrt {2 \pi b ^ {2}}} e ^ {- (y - a) ^ {2} / 2 b ^ {2}} d y
$$

and we will abbreviate this by saying X is $\textstyle { \mathcal { N } } ( a , b ^ { 2 } )$ . If X is $\textstyle { \mathcal { N } } ( a , b ^ { 2 } )$ , then $\mathbb { E } X = a$ , Var $X = b ^ { 2 }$ , and $\mathbb { E } | X | ^ { p } < \infty$ is finite for every positive integer $p .$ . Moreover 

$$
\mathbb {E} e ^ {t X} = e ^ {a t} e ^ {t ^ {2} b ^ {2} / 2}.
$$

Let $S _ { n }$ be a simple symmetric random walk. This means that $Y _ { k } = S _ { k } - S _ { k - 1 }$ equals +1 with probability $\textstyle { \frac { 1 } { 2 } }$ , equals −1 with probability $\textstyle { \frac { 1 } { 2 } }$ , and is independent of $Y _ { j }$ for $j < k$ . We notice that $\mathbb { E } S _ { n } = 0$ while E $\begin{array} { r } { S _ { n } ^ { 2 } = \sum _ { i = 1 } ^ { n } \mathbb { E } Y _ { i } ^ { 2 } + \sum _ { i \neq j } \mathbb { E } Y _ { i } Y _ { j } = n } \end{array}$ using the fact that $\mathbb { E } \left[ Y _ { i } Y _ { j } \right] = ( \mathbb { E } Y _ { i } ) ( \mathbb { E } Y _ { j } ) = 0$ 

Define $X _ { t } ^ { n } = S _ { n t } / \sqrt { n }$ if nt is an integer and by linear interpolation for other t. If nt is an integer, E $X _ { t } ^ { n } = 0$ and E $( X _ { t } ^ { n } ) ^ { 2 } = t$ . It turns out $X _ { t } ^ { n }$ does not converge for any ω. However there is another kind of convergence, called weak convergence, that takes place. There exists a process $Z _ { t }$ such that for each k, each $t _ { 1 } < t _ { 2 } < \cdots < t _ { k }$ , and each $a _ { 1 } < b _ { 1 } , a _ { 2 } < b _ { 2 } , \ldots , a _ { k } < b _ { k }$ , we have 

(1) The paths of $Z _ { t }$ are continuous as a function of t. 

$$
(2) \mathbb {P} (X _ {t _ {1}} ^ {n} \in [ a _ {1}, b _ {1} ], \ldots , X _ {t _ {k}} ^ {n} \in [ a _ {k}, b _ {k} ]) \to \mathbb {P} (Z _ {t _ {1}} \in [ a _ {1}, b _ {1} ], \ldots , Z _ {t _ {k}} \in [ a _ {k}, b _ {k} ]).
$$

See Note 1 for more discussion of weak convergence. 

The limit $Z _ { t }$ is called a Brownian motion starting at 0. It has the following properties. 

(1) E $Z _ { t } = 0$ 

(2) E $, Z _ { t } ^ { 2 } = t .$ 

(3) $Z _ { t } - Z _ { s }$ is independent of $\mathcal { F } _ { s } = \sigma ( Z _ { r } , r \le s )$ 

(4) $Z _ { t } - Z _ { s }$ has the distribution of a normal random variable with mean 0 and variance $t - s .$ . This means 

$$
\mathbb {P} (Z _ {t} - Z _ {s} \in [ a, b ]) = \int_ {a} ^ {b} \frac {1}{\sqrt {2 \pi (t - s)}} e ^ {- y ^ {2} / 2 (t - s)} d y.
$$

(This result follows from the central limit theorem.) 

(5) The map $t \to Z _ { t } ( \omega )$ is continuous for almost all $\omega$ . 

See Note 2 for a few remarks on this definition. 

It is common to use $B _ { t } \ \mathrm { ~ ( ' s ) " ~ }$ for Brownian) or $W _ { t } \ \mathrm { ( ' 5 W " }$ for Wiener, who was the first person to prove rigorously that Brownian motion exists). We will most often use $W _ { t }$ 

We will use Brownian motion extensively and develop some of its properties. As one might imagine for a limit of a simple random walk, the paths of Brownian motion have a huge number of oscillations. It turns out that the function $t  W _ { t } ( \omega )$ is continuous, but it is not diferentiable; in fact one cannot define a derivative at any value of t. Another bizarre property: if one looks at the set of times at which $W _ { t } ( \omega )$ is equal to 0, this is a set which is uncountable, but contains no intervals. There is nothing special about $0 -$ the same is true for the set of times at which $W _ { t } ( \omega )$ is equal to a for any level $a .$ 

In what follows, one of the crucial properties of a Brownian motion is that it is a martingale with continuous paths. Let us prove this. 

Proposition 11.1. $W _ { t }$ is a martingale with respect to $\mathcal { F } _ { t }$ and $W _ { t }$ has continuous paths. 

Proof. As part of the definition of a Brownian motion, $W _ { t }$ has continuous paths. $W _ { t }$ is $\mathcal { F } _ { t }$ measurable by the definition of $\mathcal { F } _ { t }$ . Since the distribution of $W _ { t }$ is that of a normal random variable with mean 0 and variance t, then $\mathbb { E } \left| W _ { t } \right| < \infty$ for all t. (In fact, $\mathbb { E } | W _ { t } | ^ { n } < \infty$ for all $n . )$ 

The key property is to show $\mathbb { E } \left[ W _ { t } \mid \mathcal { F } _ { s } \right] = W _ { s }$ 

$$
\mathbb {E} \left[ W _ {t} \mid \mathcal {F} _ {s} \right] = \mathbb {E} \left[ W _ {t} - W _ {s} \mid \mathcal {F} _ {s} \right] + \mathbb {E} \left[ W _ {s} \mid \mathcal {F} _ {s} \right] = \mathbb {E} \left[ W _ {t} - W _ {s} \right] + W _ {s} = W _ {s}.
$$

We used here the facts that $W _ { t } \mathrm { ~ - ~ } W _ { s }$ is independent of $\mathcal { F } _ { s }$ and that $\mathbb { E } \left[ W _ { t } - W _ { s } \right] = 0$ because $W _ { t }$ and $W _ { s }$ have mean 0. □ 

We will also need 

Proposition 11.2. $W _ { t } ^ { 2 } - t$ is a martingale with continuous paths with respect to $\mathcal { F } _ { t }$ 

Proof. That $W _ { t } ^ { 2 } - t$ is integrable and is $\mathcal { F } _ { t }$ measurable is as in the above proof. We calculate 

$$
\begin{array}{r l} & {\mathbb {E} \left[ W _ {t} ^ {2} - t \mid \mathcal {F} _ {s} \right] = \mathbb {E} \left[ \left(\left(W _ {t} - W _ {s}\right) + W _ {s}\right) ^ {2} \mid \mathcal {F} _ {s} \right] - t} \\ & {\qquad = \mathbb {E} \left[ \left(W _ {t} - W _ {s}\right) ^ {2} \mid \mathcal {F} _ {s} \right] + 2 \mathbb {E} \left[ \left(W _ {t} - W _ {s}\right) W _ {s} \mid \mathcal {F} _ {s} \right] + \mathbb {E} \left[ W _ {s} ^ {2} \mid \mathcal {F} _ {s} \right] - t} \\ & {\qquad = \mathbb {E} \left[ \left(W _ {t} - W _ {s}\right) ^ {2} \right] + 2 W _ {s} \mathbb {E} \left[ W _ {t} - W _ {s} \mid \mathcal {F} _ {s} \right] + W _ {s} ^ {2} - t.} \end{array}
$$

We used the facts that $W _ { s }$ is $\mathcal { F } _ { s }$ measurable and that $( W _ { t } - W _ { s } ) ^ { 2 }$ is independent of $\mathcal { F } _ { s }$ because $W _ { t } - W _ { s }$ is. The second term on the last line is equal to $W _ { s } \mathbb { E } \left[ W _ { t } - W _ { s } \right] = 0$ . The first term, because $W _ { t } - W _ { s }$ is normal with mean 0 and variance $t - s$ , is equal to $t - s$ Substituting, the last line is equal to 

$$
(t - s) + 0 + W _ {s} ^ {2} - t = W _ {s} ^ {2} - s
$$

Note 1. A sequence of random variables $X _ { n }$ converges weakly to X if $\mathbb { P } ( a < X _ { n } < b ) \to$ $\mathbb { P } ( a < X < b )$ for all $a , b \in [ - \infty , \infty ]$ such that $\mathbb { P } ( X = a ) = \mathbb { P } ( X = b ) = 0$ . a and b can be infinite. If $X _ { n }$ converges to a normal random variable, then $\mathbb { P } ( X = a ) = \mathbb { P } ( X = b ) = 0$ for all a and b. This is the type of convergence that takes place in the central limit theorem. It will not be true in general that $X _ { n }$ converges to X almost surely. 

For a sequence of random vectors $( X _ { 1 } ^ { n } , \ldots , X _ { k } ^ { m } )$ to converge to a random vector $( X _ { 1 } , \ldots , X _ { k } )$ , one can give an analogous definition. But saying that the normalized random walks $X _ { n } ( t )$ above converge weakly to $Z _ { t }$ actually says more than (2). A result from probability theory says that $X _ { n }$ converges to X weakly if and only if $\mathbb { E } [ f ( X _ { n } ) ]  \mathbb { E } [ f ( X ) ]$ whenever f is a bounded continuous function on R. We use this to define weak convergence for stochastic processes. Let $C ( [ 0 , \infty )$ be the collection of all continuous functions from $[ 0 , \infty )$ to the reals. This is a metric space, so the notion of function from $C ( [ 0 , \infty ) )$ to R being continuous makes sense. We say that the processes $X _ { n }$ converge weakly to the process $Z ,$ and mean by this that E $[ F ( X _ { n } ) ] \to \mathbb { E } \left[ F ( Z ) \right]$ whenever F is a bounded continuous function on $C ( [ 0 , \infty ) )$ ). One example of such a function F would be $F ( f ) = \operatorname* { s u p } _ { 0 \leq t < \infty } | f ( t ) | { \mathrm { ~ i f ~ } } f \in C ( [ 0 , \infty ) )$ ; Another would be $\textstyle F ( f ) = \int _ { 0 } ^ { 1 } f ( t ) d t$ 

The reason one wants to show that $X _ { n }$ converges weakly to Z instead of just showing (2) is that weak convergence can be shown to imply that Z has continuous paths. 

Note 2. First of all, there is some redundancy in the definition: one can show that parts of the definition are implied by the remaining parts, but we won’t worry about this. Second, we actually want to let $\mathcal { F } _ { t }$ to be the completion of $\sigma ( Z _ { s } : s \le t )$ , that is, we throw in all the null sets into each $\mathcal { F } _ { t }$ . One can prove that the resulting $\mathcal { F } _ { t }$ are right continuous, and hence the filtration $\mathcal { F } _ { t }$ satisfies the “usual” conditions. Finally, the “almost all” in (5) means that $t \to Z _ { t } ( \omega )$ is continuous for all $\omega ,$ , except for a set of $\omega$ of probability zero. 

## 12. Stochastic integrals.

If one wants to consider the (deterministic) integral $\textstyle \int _ { 0 } ^ { t } f ( s ) d g ( s )$ , where $f$ and $g$ are continuous and $g$ is continuously diferentiable, we can define it analogously to the usual Riemann integral as the limit of Riemann sums $\begin{array} { r } { \sum _ { i = 1 } ^ { n } f ( s _ { i } ) [ g ( s _ { i } ) - g ( s _ { i - 1 } ) ] } \end{array}$ ], where $s _ { 1 } < s _ { 2 } < \cdots < s _ { n }$ is a partition of [0, t]. This is known as the Riemann-Stieltjes integral. One can show (using the mean value theorem, for example) that 

$$
\int_ {0} ^ {t} f (s) d g (s) = \int_ {0} ^ {t} f (s) g ^ {\prime} (s) d s.
$$

If we were to take $f ( s ) = 1 _ { [ 0 , a ] } ( s )$ (which is not continuous, but that is a minor matter here), one would expect the following: 

$$
\int_ {0} ^ {t} 1 _ {[ 0, a ]} (s) d g (s) = \int_ {0} ^ {t} 1 _ {[ 0, a ]} (s) g ^ {\prime} (s) d s = \int_ {0} ^ {a} g ^ {\prime} (s) d s = g (a) - g (0).
$$

Note that although we use the fact that $g$ is diferentiable in the intermediate stages, the first and last terms make sense for any $g .$ 

We now want to replace $g$ by a Brownian path and $f$ by a random integrand. The expression $\int f ( s ) d W ( s )$ does not make sense as a Riemann-Stieltjes integral because it is a fact that $W ( s )$ is not diferentiable as a function of t. We need to define the expression by some other means. We will show that it can be defined as the limit in $L ^ { 2 }$ of Riemann sums. The resulting integral is called a stochastic integral. 

Let us consider a very special case first. Suppose $f$ is continuous and deterministic (i.e., does not depend on ω). Suppose we take a Riemann sum approximation 

$$
I _ {n} = \sum_ {i = 0} ^ {2 ^ {n} - 1} f (\frac {i}{2 ^ {n}}) [ W (\frac {i + 1}{2 ^ {n}}) - W (\frac {i}{2 ^ {n}}) ].
$$

Since $W _ { t }$ has zero expectation for each $t , \mathbb { E } I _ { n } = 0$ . Let us calculate the second moment: 

$$
\begin{array}{l} \mathbb {E} I _ {n} ^ {2} = \mathbb {E} \left[ \left(\sum_ {i} f (\frac {i}{2 ^ {n}}) [ W (\frac {i + 1}{2 ^ {n}}) - W (\frac {i}{2 ^ {n}}) ]\right) ^ {2} \right] \\ = \mathbb {E} \sum_ {i = 0} ^ {2 ^ {n} - 1} f (\frac {i}{2 ^ {n}}) ^ {2} [ W (\frac {i + 1}{2 ^ {n}}) - W (\frac {i}{2 ^ {n}}) ] ^ {2} \\ \qquad + \mathbb {E} \sum_ {i \neq j} f (\frac {i}{2 ^ {n}}) f (\frac {j}{2 ^ {n}}) [ W (\frac {i + 1}{2 ^ {n}}) - W (\frac {i}{2 ^ {n}}) ] [ W (\frac {j + 1}{2 ^ {n}}) - W (\frac {j}{2 ^ {n}}) ]. \end{array}\tag{12.1}
$$

The first sum is bounded by 

$$
\sum_ {i} f (\frac {i}{2 ^ {n}}) ^ {2} \frac {1}{2 ^ {n}} \approx \int_ {0} ^ {1} f (t) ^ {2} d t,
$$

since the second moment of $W ( \textstyle { \frac { i + 1 } { 2 ^ { n } } } ) - W ( \textstyle { \frac { i } { 2 ^ { n } } } ) { \mathrm { ~ i s ~ } } 1 / 2 ^ { n }$ . Using the independence and the fact that $W _ { t }$ has mean zero, 

$$
\mathbb {E} \left[ [ W (\frac {i + 1}{2 ^ {n}} - W (\frac {i}{2 ^ {n}}) ] [ W (\frac {j + 1}{2 ^ {n}} - W (\frac {j}{2 ^ {n}}) ] \right] = \mathbb {E} \left[ W (\frac {i + 1}{2 ^ {n}} - W (\frac {i}{2 ^ {n}}) \right] \mathbb {E} \left[ W (\frac {j + 1}{2 ^ {n}} - W (\frac {j}{2 ^ {n}}) \right] = 0,
$$

and so the second sum on the right hand side of (12.1) is zero. This calculation is the key to the stochastic integral. 

We now turn to the construction. Let $W _ { t }$ be a Brownian motion. We will only consider integrands $H _ { s }$ such that $H _ { s }$ is $\mathcal { F } _ { s }$ measurable for each s (see Note 1). We will construct $\begin{array} { r } { \int _ { 0 } ^ { t } H _ { s } d W _ { \it \Psi } } \end{array}$ for all H with 

$$
\mathbb {E} \int_ {0} ^ {t} H _ {s} ^ {2} d s <   \infty .\tag{12.2}
$$

Before we proceed we will need to define the quadratic variation of a continuous martingale. We will use the following theorem without proof because in our applications we can construct the desired increasing process directly. We often say a process is a continuous process if its paths are continuous, and similarly a continuous martingale is a martingale with continuous paths. 

Theorem 12.1. Suppose $M _ { t }$ is a continuous martingale such that $\mathbb { E } M _ { t } ^ { 2 }$ < ∞ for all t. There exists one and only one increasing process $A _ { t }$ that is adapted to $\mathcal { F } _ { t }$ , has continuous paths, and $A _ { 0 } = 0$ such that $M _ { t } ^ { 2 } - A _ { t }$ is a martingale. 

The simplest example of such a martingale is Brownian motion. If $W _ { t }$ is a Brownian motion, we saw in Proposition 11.2 that $W _ { t } ^ { 2 } - t$ is a martingale. So in this case $A _ { t } = t$ almost surely, for all t. Hence $\langle W \rangle _ { t } = t$ 

We use the notation $\langle M \rangle .$ for the increasing process given in Theorem 12.1 and call it the quadratic variation process of M. We will see later that in the case of stochastic integrals, where 

$$
N _ {t} = \int_ {0} ^ {t} H _ {s} d W _ {s},
$$

it turns out that $\begin{array} { r } { { \langle N \rangle } _ { t } = \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s } \end{array}$ 

We will use the following frequently, and in fact, these are the only two properties of Brownian motion that play a significant role in the construction. 

Lemma 12.1. $( a ) \operatorname { \mathbb { E } } \left[ W _ { b } - W _ { a } \mid { \mathcal { F } } _ { a } \right] = 0 .$ 

$$
(b) \mathbb {E} [ W _ {b} ^ {2} - W _ {a} ^ {2} | \mathcal {F} _ {a} ] = \mathbb {E} [ (W _ {b} - W _ {a}) ^ {2} | \mathcal {F} _ {a} ] = b - a.
$$

Proof. (a) This is E $\left[ W _ { b } - W _ { a } \right] = 0$ by the independence of $W _ { b } - W _ { a }$ from ${ \mathcal { F } } _ { a }$ and the fact that $W _ { b }$ and $W _ { a }$ have mean zero. 

(b) $( W _ { b } - W _ { a } ) ^ { 2 }$ is independent of ${ \mathcal { F } } _ { a } ,$ so the conditional expectation is the same as $\mathbb { E } \left[ ( W _ { b } - W _ { a } ) ^ { 2 } \right]$ . Since $W _ { b } - W _ { a }$ is a ${ \mathcal { N } } ( 0 , b - a )$ , the second equality in (b) follows. 

To prove the first equality in (b), we write 

$$
\begin{array}{r l} & {\mathbb {E} \left[ W _ {b} ^ {2} - W _ {a} ^ {2} \mid \mathcal {F} _ {a} \right] = \mathbb {E} \left[ ((W _ {b} - W _ {a}) + W _ {a}) ^ {2} \mid \mathcal {F} _ {a} \right] - \mathbb {E} \left[ W _ {a} ^ {2} \mid \mathcal {F} _ {a} \right]} \\ & {\qquad = \mathbb {E} \left[ (W _ {b} - W _ {a}) ^ {2} \mid \mathcal {F} _ {a} \right] + 2 \mathbb {E} \left[ W _ {a} (W _ {b} - W _ {a}) \mid \mathcal {F} _ {a} \right] + \mathbb {E} \left[ W _ {a} ^ {2} \mid \mathcal {F} _ {a} \right]} \\ & {\qquad - \mathbb {E} \left[ W _ {a} ^ {2} \mid \mathcal {F} _ {a} \right]} \\ & {\qquad = \mathbb {E} \left[ (W _ {b} - W _ {a}) ^ {2} \mid \mathcal {F} _ {a} \right] + 2 W _ {a} \mathbb {E} \left[ W _ {b} - W _ {a} \mid \mathcal {F} _ {a} \right],} \end{array}
$$

and the first equality follows by applying (a). 

We construct the stochastic integral in three steps. We say an integrand $H _ { s } = H _ { s } ( \omega )$ is elementary if 

$$
H _ {s} (\omega) = G (\omega) 1 _ {(a, b ]} (s)
$$

where $0 \leq a < b$ and G is bounded and ${ \mathcal { F } } _ { a }$ measurable. We say H is simple if it is a finite linear combination of elementary processes, that is, 

$$
H _ {s} (\omega) = \sum_ {i = 1} ^ {n} G _ {i} (\omega) 1 _ {(a _ {i}, b _ {i} ]} (s).\tag{12.3}
$$

We first construct the stochastic integral for H elementary; the work here is showing the stochastic integral is a martingale. We next construct the integral for H simple and here the dificulty is calculating the second moment. Finally we consider the case of general H. 

First step. If G is bounded and ${ \mathcal { F } } _ { a }$ measurable, let $H _ { s } ( \omega ) = G ( \omega ) 1 _ { ( a , b ] } ( s )$ , and define the stochastic integral to be the process $N _ { t }$ , where $N _ { t } = G ( W _ { t \wedge b } - W _ { t \wedge a } )$ . Compare this to the first paragraph of this section, where we considered Riemann-Stieltjes integrals. 

Proposition 12.2. $N _ { t }$ is a continuous martingale, E $N _ { \infty } ^ { 2 } = \mathbb { E } \left[ G ^ { 2 } ( b - a ) \right]$ and 

$$
\langle N \rangle_ {t} = \int_ {0} ^ {t} G ^ {2} 1 _ {[ a, b ]} (s) d s.
$$

Proof. The continuity is clear. Let us look at $\mathbb { E } \left[ N _ { t } \ | \ \mathcal { F } _ { s } \right]$ . In the case $a < s < t < b .$ , this is equal to 

$$
\mathbb {E} \left[ G (W _ {t} - W _ {a}) \mid \mathcal {F} _ {s} \right] = G \mathbb {E} \left[ (W _ {t} - W _ {a}) \mid \mathcal {F} _ {s} \right] = G (W _ {s} - W _ {a}) = N _ {s}.
$$

In the case $\mathit { s } < a < t < b , \mathbb { E } \left[ N _ { t } \mid \mathcal { F } _ { s } \right]$ is equal to 

$$
\mathbb {E} \left[ G (W _ {t} - W _ {a}) \mid \mathcal {F} _ {s} \right] = \mathbb {E} \left[ G \mathbb {E} \left[ W _ {t} - W _ {a} \mid \mathcal {F} _ {a} \right] \mid \mathcal {F} _ {s} \right] = 0 = N _ {s}.
$$

The other possibilities are $s < t < a < b , a < b < s < t , a s < a < b < t .$ and $a < s < b < t ;$ these are done similarly. 

For E $N _ { \infty } ^ { 2 }$ , we have using Lemma 12.1(b) 

$$
\mathbb {E} N _ {\infty} ^ {2} = \mathbb {E} \left[ G ^ {2} \mathbb {E} \left[ (W _ {b} - W _ {a}) ^ {2} \mid \mathcal {F} _ {a} \right] \right] = \mathbb {E} \left[ G ^ {2} \mathbb {E} \left[ W _ {b} ^ {2} - W _ {a} ^ {2} \mid \mathcal {F} _ {a} \right] \right] = \mathbb {E} \left[ G ^ {2} (b - a) \right].
$$

For $\langle N \rangle _ { t } ,$ , we need to show 

$$
\begin{array}{r l} & {\mathbb {E} \left[ G ^ {2} (W _ {t \wedge b} - W _ {t \wedge a}) ^ {2} - G ^ {2} (t \wedge b - t \wedge a) \mid \mathcal {F} _ {s} \right]} \\ & {\qquad = G ^ {2} (W _ {s \wedge b} - W _ {s \wedge a}) ^ {2} - G ^ {2} (s \wedge b - s \wedge a).} \end{array}
$$

We do this by checking all six cases for the relative locations of $a , b , s ,$ , and $t ;$ we do one of the cases in Note 2. □ 

Second step. Next suppose $H _ { s }$ is simple as in (12.3). In this case define the stochastic integral 

$$
N _ {t} = \int_ {0} ^ {t} H _ {s} d W _ {s} = \sum_ {i = 1} ^ {n} G _ {i} (W _ {b _ {i} \wedge t} - W _ {a _ {i} \wedge t}).
$$

Proposition 12.3. $N _ { t }$ is a continuous martingale, E $\begin{array} { r } { N _ { \infty } ^ { 2 } = \mathbb { E } \int _ { 0 } ^ { \infty } H _ { s } ^ { 2 } d s } \end{array}$ , and $\langle N \rangle _ { t } =$ $\textstyle \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s$ 

Proof. We may rewrite H so that the intervals $\left( a _ { i } , b _ { i } \right]$ satisfy $a _ { 1 } \leq b _ { 1 } \leq a _ { 2 } \leq b _ { 2 } \leq \cdot \cdot \cdot \leq b _ { n }$ For example, if we had $a _ { 1 } < a _ { 2 } < b _ { 1 } < b _ { 2 }$ , we could write 

$$
H _ {s} = G _ {1} 1 _ {(a _ {1}, a _ {2} ]} + (G _ {1} + G _ {2}) 1 _ {(a _ {2}, b _ {1} ]} + G _ {2} 1 _ {(b _ {1}, b _ {2} ]},
$$

and then if we set $G _ { 1 } ^ { \prime } = G _ { 1 } , G _ { 2 } ^ { \prime } = G _ { 1 } + G _ { 2 } , G _ { 3 } ^ { \prime } = G _ { 2 }$ and $a _ { 1 } ^ { \prime } = a _ { 1 } , b _ { 1 } ^ { \prime } = a _ { 2 } , a _ { 2 } ^ { \prime } = a _ { 2 } , b _ { 2 } ^ { \prime } =$ $b _ { 1 } , a _ { 3 } ^ { \prime } = b _ { 1 } , b _ { 3 } ^ { \prime } = b _ { 2 }$ , we have written H as 

$$
\sum_ {i = 1} ^ {3} G _ {i} ^ {\prime} 1 _ {(a _ {i} ^ {\prime}, b _ {i} ^ {\prime} ]}.
$$

So now we have H simple but with the intervals $( a _ { i } ^ { \prime } , b _ { i } ^ { \prime } ]$ non-overlapping. 

Since the sum of martingales is clearly a martingale, $N _ { t }$ is a martingale. The sum of continuous processes will be continuous, so $N _ { t }$ has continuous paths. 

We have 

$$
\mathbb {E} N _ {\infty} ^ {2} = \mathbb {E} \left[ \sum G _ {i} ^ {2} (W _ {b _ {i}} - W _ {a _ {i}}) ^ {2} \right] + 2 \mathbb {E} \left[ \sum_ {i <   j} G _ {i} G _ {j} (W _ {b _ {i}} - W _ {a _ {i}}) (W _ {b _ {j}} - W _ {a _ {j}}) \right].
$$

The terms in the second sum vanish, because when we condition on $\mathcal { F } _ { a _ { i } }$ , we have 

$$
\mathbb {E} \left[ G _ {i} G _ {j} (W _ {b _ {i}} - W _ {a _ {i}}) \mathbb {E} \left[ (W _ {b _ {j}} - W _ {a _ {j}}) \mid \mathcal {F} _ {a _ {j}} \right] = 0. \right.
$$

Taking expectations, 

$$
\mathbb {E} \left[ G _ {i} G _ {j} (W _ {b _ {i}} - W _ {a _ {i}}) (W _ {b _ {j}} - W _ {a _ {j}}) \right] = 0.
$$

For the terms in the first sum, by Lemma 12.1 

$$
\mathbb {E} \left[ G _ {i} ^ {2} (W _ {b _ {i}} - W _ {a _ {i}}) ^ {2} \right] = \mathbb {E} \left[ G _ {i} ^ {2} \mathbb {E} \left[ (W _ {b _ {i}} - W _ {a _ {i}}) ^ {2} \mid \mathcal {F} _ {a _ {i}} \right] \right] = \mathbb {E} \left[ G _ {i} ^ {2} ([ b _ {i} - a _ {i}) ]. \right.
$$

So 

$$
\mathbb {E} N _ {\infty} ^ {2} = \sum_ {i = 1} ^ {n} E [ G _ {i} ^ {2} ([ b _ {i} - a _ {i}) ],
$$

and this is the same as E $\int _ { 0 } ^ { \infty } H _ { s } ^ { 2 } d s$ 

Third step. Now suppose $H _ { s }$ is adapted and E $\textstyle \int _ { 0 } ^ { \infty } H _ { s } ^ { 2 } d s < \infty$ . Using some results from measure theory (Note 3), we can choose $H _ { s } ^ { n }$ simple such that E $\begin{array} { r } { \int _ { 0 } ^ { \infty } ( H _ { s } ^ { n } - H _ { s } ) ^ { 2 } d s \to 0 . } \end{array}$ The triangle inequality then implies (see Note 3 again) 

$$
\mathbb {E} \int_ {0} ^ {\infty} (H _ {s} ^ {n} - H _ {s} ^ {m}) ^ {2} d s \to 0.
$$

Define $\begin{array} { r } { N _ { t } ^ { n } = \int _ { 0 } ^ { t } H _ { s } ^ { n } d W _ { s } } \end{array}$ using Step 2. By Doob’s inequality (Theorem 10.3) we have 

$$
\begin{array}{r l} & {\mathbb {E} \left[ \underset {t} {\sup} (N _ {t} ^ {n} - N _ {t} ^ {m}) ^ {2} \right] = \mathbb {E} \left[ \underset {t} {\sup} \left(\int_ {0} ^ {t} (H _ {s} ^ {n} - H _ {s} ^ {m}) d W _ {s}\right) ^ {2} \right]} \\ & {\qquad \leq 4 \mathbb {E} \left(\int_ {0} ^ {\infty} (H _ {s} ^ {n} - H _ {s} ^ {m}) d W _ {s}\right) ^ {2}} \\ & {\qquad = 4 \mathbb {E} \int_ {0} ^ {\infty} (H _ {s} ^ {n} - H _ {s} ^ {m}) ^ {2} d s \to 0.} \end{array}
$$

This should look reminiscent of the definition of Cauchy sequences, and in fact that is what is going on here; Note 3 has details. In the present context Cauchy sequences converge, and one can show (Note 3) that there exists a process $N _ { t }$ such that 

$$
\mathbb {E} \left[\left(\sup _ {t} \left| \int_ {0} ^ {t} H _ {s} ^ {n} d W _ {s} - N _ {t} \right|\right) ^ {2} \right]\rightarrow 0.
$$

If $H _ { s } ^ { n }$ and $H _ { s } ^ { n \prime }$ are two sequences converging to $H$ , then $\begin{array} { r } { \mathbb { E } \left( \int _ { 0 } ^ { t } ( H _ { s } ^ { n } - H _ { s } ^ { n \prime } ) d W _ { s } \right) ^ { 2 } = } \end{array}$ E $\begin{array} { r } { \int _ { 0 } ^ { t } ( H _ { s } ^ { n } - H _ { s } ^ { n \prime } ) ^ { 2 } d s \to 0 } \end{array}$ , or the limit is independent of which sequence $H ^ { n }$ we choose. See Note 4 for the proof that $N _ { t }$ is a martingale, E $\begin{array} { r } { N _ { t } ^ { 2 } = \mathbb { E } \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s } \end{array}$ , and $\begin{array} { r } { \langle N \rangle _ { t } = \int _ { 0 } ^ { t } H _ { s } ^ { 2 } } \end{array}$ ds. 

Because $\begin{array} { r } { \operatorname* { s u p } _ { t } [ \int _ { 0 } ^ { t } H _ { s } ^ { n } d W _ { s } - N _ { t } ]  0 } \end{array}$ , one can show there exists a subsequence such that the convergence takes place almost surely, and with probability one, $N _ { t }$ has continuous paths (Note 5). 

We write $\begin{array} { r } { N _ { t } = \int _ { 0 } ^ { t } H _ { s } d W _ { s } } \end{array}$ and call $N _ { t }$ the stochastic integral of H with respect to W. 

We discuss some extensions of the definition. First of all, if we replace $W _ { t }$ by a continuous martingale $M _ { t }$ and $H _ { s }$ is adapted with E $\begin{array} { r } { \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d \langle M \rangle _ { s } < \infty , } \end{array}$ we can duplicate everything we just did (see Note 6) with ds replaced by $d \langle M \rangle$ and get a stochastic integral. In particular, if $d \langle M \rangle _ { s } = K _ { s } ^ { 2 } d s$ , we replace ds by $K _ { s } ^ { 2 } d s$ 

There are some other extensions of the definition that are not hard. If the random variable $\int _ { 0 } ^ { \infty } H _ { s } ^ { 2 } d \langle M \rangle _ { s }$ is finite but without its expectation being finite, we can define the stochastic integral by defining it for $t \leq T _ { N }$ for suitable stopping times $T _ { N }$ and then letting $T _ { N } \to \infty ;$ look at Note 7. 

A process $A _ { t }$ is of bounded variation if the paths of $A _ { t }$ have bounded variation. This means that one can write $A _ { t } = A _ { t } ^ { + } - A _ { t } ^ { - }$ , where $A _ { t } ^ { + }$ and $A _ { t } ^ { - }$ have paths that are increasing. $| A | _ { t }$ is then defined to be $A _ { t } ^ { + } + A _ { t } ^ { - }$ . A semimartingale is the sum of a martingale and a process of bounded variation. If $\begin{array} { r } { \int _ { 0 } ^ { \infty } H _ { s } ^ { 2 } d \langle M \rangle _ { s } + \int _ { 0 } ^ { \infty } | H _ { s } | | d A _ { s } | < \infty } \end{array}$ and $X _ { t } = M _ { t } + A _ { t }$ , we define 

$$
\int_ {0} ^ {t} H _ {s} d X _ {s} = \int_ {0} ^ {t} H _ {s} d M _ {s} + \int_ {0} ^ {t} H _ {s} d A _ {s},
$$

where the first integral on the right is a stochastic integral and the second is a Riemann-Stieltjes or Lebesgue-Stieltjes integral. For a semimartingale, we define $\langle X \rangle _ { t } = \langle M _ { t } \rangle$ . Note $7$ has more on this. 

Given two semimartingales X and Y we define $\langle X , Y \rangle _ { i }$ by what is known as polarization: 

$$
\langle X, Y \rangle_ {t} = \frac {1}{2} [ \langle X + Y \rangle_ {t} - \langle X \rangle_ {t} - \langle Y \rangle_ {t} ].
$$

As an example, if $\begin{array} { r } { X _ { t } = \int _ { 0 } ^ { t } H _ { s } d W _ { s } } \end{array}$ and $\begin{array} { r } { Y _ { t } = \int _ { 0 } ^ { t } K _ { s } d W _ { s } } \end{array}$ , then $\begin{array} { r } { ( X + Y ) _ { t } = \int _ { 0 } ^ { t } ( H _ { s } + K _ { s } ) d W _ { s } } \end{array}$ ， so 

$$
\langle X + Y \rangle_ {t} = \int_ {0} ^ {t} (H _ {s} + K _ {s}) ^ {2} d s = \int_ {0} ^ {t} H _ {s} ^ {2} d s + \int_ {0} ^ {t} 2 H _ {s} K _ {s} d s + \int_ {0} ^ {t} K _ {s} ^ {2} d s.
$$

Since $\begin{array} { r } { { \langle X \rangle } _ { t } = \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s } \end{array}$ with a similar formula for $\langle Y \rangle _ { t }$ , we conclude 

$$
\langle X, Y \rangle_ {t} = \int_ {0} ^ {t} H _ {s} K _ {s} d s.
$$

The following holds, which is what one would expect. 

Proposition 12.4. Suppose $K _ { s }$ is adapted to $\mathcal { F } _ { s }$ and E $\textstyle \int _ { 0 } ^ { \infty } K _ { s } ^ { 2 } d s < \infty$ . Let $N _ { t } \ =$ $\begin{array} { r } { \int _ { 0 } ^ { t } K _ { s } d W _ { s } } \end{array}$ . Suppose $H _ { s }$ is adapted and E $\begin{array} { r } { \int _ { 0 } ^ { \infty } H _ { s } ^ { 2 } d \langle N \rangle _ { s } < \infty } \end{array}$ . Then E $\textstyle \int _ { 0 } ^ { \infty } H _ { s } ^ { 2 } K _ { s } ^ { 2 } d s <$ ∞ and 

$$
\int_ {0} ^ {t} H _ {s} d N _ {s} = \int_ {0} ^ {t} H _ {s} K _ {s} d W _ {s}.
$$

The argument for the proof is given in Note 8. 

What does a stochastic integral mean? If one thinks of the derivative of $Z _ { t }$ as being a white noise, then $\begin{array} { r } { \int _ { 0 } ^ { t } H _ { s } d Z _ { s } } \end{array}$ is like a filter that increases or decreases the volume by a factor $H _ { s }$ 

For us, an interpretation is that $Z _ { t }$ represents a stock price. Then $\begin{array} { r } { \int _ { 0 } ^ { t } H _ { s } d Z _ { s } } \end{array}$ represents our profit (or loss) if we hold $H _ { s }$ shares at time s. This can be seen most easily if $H _ { s } = G 1 _ { [ a , b ] }$ . So we buy $G ( \omega )$ shares at time a and sell them at time b. The stochastic integral represents our profit or loss. 

Since we are in continuous time, we are allowed to buy and sell continuously and instantaneously. What we are not allowed to do is look into the future to make our decisions, which is where the $H _ { s }$ adapted condition comes in. 

Note 1. Let us be more precise concernin the measurabilit of H that is needed. H is a stochastic process, so can be viewed as a map from $[ 0 , \infty ) \times \Omega$ to R by $H : ( s , \omega )  H _ { s } ( \omega )$ We define a σ-field $\mathcal { P }$ on $[ 0 , \infty ) \times \Omega$ as follows. Consider the collection of processes of the form $G ( \omega ) 1 _ { ( a , b ] ) } ( s )$ where $G$ is bounded and ${ \mathcal { F } } _ { a }$ measurable for some $a < b$ . Define $\mathcal { P }$ to be the smallest σ-field with respect to which every process of this form is measurable. $\mathcal { P }$ is called the predictable or previsible σ-field, and if a process H is measurable with respect to $\mathcal { P }$ , then the process is called predictable. What we require for our integrands H is that they be predictable processes. 

If $H _ { s }$ has continuous paths, then approximating continuous functions by step functions shows that such an H can be approximated by linear combinations of processes of the form $G ( \omega ) 1 _ { ( a , b ] ) } ( s )$ . So continuous processes are predictable. The majority of the integrands we will consider will be continuous. 

If one is slightly more careful, one sees that processes whose paths are functions which are continuous from the left at each time point are also predictable. This gives an indication of where the name comes from. If $H _ { s }$ has paths which are left continuous, then $H _ { t } \ =$ $\scriptstyle \operatorname* { l i m } _ { n \to \infty } H _ { t - { \frac { 1 } { n } } }$ , and we can “predict” the value of $H _ { t }$ from the values at times that come before t. If $H _ { t }$ is only right continuous and a path has a jump at time $t ,$ this is not possible. 

Note 2. Let us consider the case $a < s < t < b ;$ again similar arguments take care of the other five cases. We need to show 

$$
\mathbb {E} \left[ G ^ {2} (W _ {t} - W _ {a}) ^ {2} - G ^ {2} (t - a) \mid \mathcal {F} _ {s} \right] = G ^ {2} (W _ {s} - W _ {a}) ^ {2} - G ^ {2} (s - a).\tag{12.4}
$$

The left hand side is equal to $G ^ { 2 } \mathbb { E } \left[ ( W _ { t } - W _ { a } ) ^ { 2 } - ( t - a ) \ : | \ : \mathcal { F } _ { s } \right]$ . We write this as 

$$
\begin{array}{r l} & G ^ {2} \mathbb {E} \left[ ((W _ {t} - W _ {s}) + (W _ {s} - W _ {a})) ^ {2} - (t - a) \mid \mathcal {F} _ {s} \right] \\ & \quad = G ^ {2} \Bigl \{\mathbb {E} \left[ (W _ {t} - W _ {s}) ^ {2} \mid \mathcal {F} _ {s} \right] + 2 \mathbb {E} \left[ (W _ {t} - W _ {s}) (W _ {s} - W _ {a}) \mid \mathcal {F} _ {s} \right] \\ & \qquad + \mathbb {E} \left[ (W _ {s} - W _ {a}) ^ {2} \mid \mathcal {F} _ {s} \right] - (t - a) \Bigr \} \\ & \quad = G ^ {2} \Bigl \{\mathbb {E} \left[ (W _ {t} - W _ {s}) ^ {2} \right] + 2 (W _ {s} - W _ {a}) \mathbb {E} \left[ W _ {t} - W _ {s} \mid \mathcal {F} _ {s} \right] + (W _ {s} - W _ {a}) ^ {2} - (t - a) \Bigr \} \\ & \quad = G ^ {2} \Bigl \{(t - s) + 0 + (W _ {s} - W _ {a}) ^ {2} - (t - a) \Bigr \}. \end{array}
$$

The last expression is equal to the right hand side of (12.4). 

Note 3. A definition from measure theory says that if $\mu$ is a measure, $\| f \| _ { 2 }$ , the $L ^ { 2 }$ norm of $f$ with respect to the measure $\mu ,$ , is defined as $\scriptstyle \left( \int f ( x ) ^ { 2 } \mu ( d x ) \right) ^ { 1 / 2 }$ . The space $L ^ { 2 }$ is defined to be the set of functions $f$ for which $\| f \| _ { 2 } < \infty \quad$ . (A technical proviso: one has to identify as equal functions which difer only on a set of measure 0.) If one defines a distance between two functions $f$ and $g$ by $d ( f , g ) = \| f - g \| _ { 2 }$ , this is a metric on the space $L ^ { 2 }$ , and a theorem from measure theory says that $L ^ { 2 }$ is complete with respect to this metric. Another theorem from measure theory says that the collection of simple functions (functions of the form $\scriptstyle \sum _ { i = 1 } ^ { n } c _ { i } 1 _ { A _ { i } } )$ is dense in $L ^ { 2 }$ with respect to the metric. 

Let us define a norm on stochastic processes; this is essentially an $L ^ { 2 }$ norm. Define 

$$
\| N \| = \left(\mathbb {E} \sup _ {0 \leq t <   \infty} N _ {t} ^ {2}\right) ^ {1 / 2}.
$$

One can show that this is a norm, and hence that the triangle inequality holds. Moreover, the space of processes $N$ such that $\| N \| < \infty$ is complete with respect to this norm. This means that if $N ^ { n }$ is a Cauchy sequence, i.e., if given ε there exists $n _ { 0 }$ such that $\| N ^ { n } - N ^ { m } \| < \varepsilon$ whenever n, m $\geq n _ { 0 } ,$ , then the Cauchy sequence converges, that is, there exists $N$ with $\left\| N \right\| <$ ∞ such that $\| N ^ { n } - N \| \to 0$ 

We can define another norm on stochastic processes. Define 

$$
\| H \| _ {2} = \left(\mathbb {E} \int_ {0} ^ {\infty} H _ {s} ^ {2} d s\right) ^ {1 / 2}.
$$

This can be viewed as a standard $L ^ { 2 }$ norm, namely, the $L ^ { 2 }$ norm with respect to the measure $\mu$ defined on $\mathcal { P }$ by 

$$
\mu (A) = \mathbb {E} \int_ {0} ^ {\infty} 1 _ {A} (s, \omega) d s.
$$

Since the set of simple functions with respect to $\mu$ is dense in $L ^ { 2 }$ , this says that if $H$ is measurable with respect to ${ \mathcal P } ,$ then there exist simple processes $H _ { s } ^ { n }$ that are also measurable with respect to $\mathcal { P }$ such that $\| H ^ { n } - H \| _ { 2 } \to 0$ 

Note 4. We have $\| N ^ { n } - N \| \to 0$ , where the norm here is the one described in Note 3. Each $N ^ { n }$ is a stochastic integral of the type described in Step 2 of the construction, hence each $N _ { t } ^ { n }$ is a martingale. Let $s < t$ and $A \in \mathcal { F } _ { s }$ . Since $\mathbb { E } \left[ N _ { t } ^ { n } \ | \ \mathcal { F } _ { s } \right] = N _ { s } ^ { n }$ , then 

$$
\mathbb {E} \left[ N _ {t} ^ {n}; A \right] = \mathbb {E} \left[ N _ {s} ^ {n}; A \right].\tag{12.5}
$$

By Cauchy-Schwarz, 

$$
\begin{array}{c} | \mathbb {E} \left[ N _ {t} ^ {n}; A \right] - \mathbb {E} \left[ N _ {t}; A \right] | \leq \mathbb {E} \left[ | N _ {t} ^ {n} - N _ {t} |; A \right] \leq \Big (\mathbb {E} \left[ (N _ {t} ^ {n} - N _ {t}) ^ {2} \right] \Big) ^ {1 / 2} \Big (\mathbb {E} \left[ 1 _ {A} ^ {2} \right] \Big) ^ {1 / 2} \\ \leq \| N ^ {n} - N \| \to 0. \end{array}\tag{12.6}
$$

We have a similar limit when t is replaced by s, so taking the limit in (12.5) yields 

$$
\mathbb {E} \left[ N _ {t}; A \right] = \mathbb {E} \left[ N _ {s}; A \right].
$$

Since $N _ { s }$ is $\mathcal { F } _ { s }$ measurable and has the same expectation over sets $A \in \mathcal { F } _ { s }$ as $N _ { t }$ does, then by Proposition $4 . 3 \mathbb { E } \left[ N _ { t } \mid \mathcal { F } _ { s } \right] = N _ { s }$ , or $N _ { t }$ is a martingale. 

Suppose $\| N ^ { n } - N \| \to 0$ . Given $\varepsilon > 0$ there exists $n _ { 0 }$ such that $\| N ^ { n } - N \| < \varepsilon$ if $n \geq n _ { 0 }$ . Take $\varepsilon = 1$ and choose $n _ { 0 }$ . By the triangle inequality, 

$$
\| N \| \leq \| N ^ {n} \| + \| N ^ {n} - N \| \leq \| N ^ {n} \| + 1 <   \infty
$$

since $\| N ^ { n } \|$ is finite for each $n$ . 

That $N _ { t } ^ { 2 } \mathrm { ~ - ~ } \langle N \rangle _ { \mathrm { ~ } }$ is a martingale is similar to the proof that $N _ { t }$ is a martingale, but slightly more delicate. We leave the proof to the reader, but note that in place of (SEC.402) one writes 

$$
| \mathbb {E} [ (N _ {t} ^ {n}) ^ {2}; A ] - \mathbb {E} [ (N _ {t}) ^ {2}; A ] | \leq \mathbb {E} [ | (N _ {t} ^ {n}) ^ {2} - (N _ {t}) ^ {2} | ] \leq \mathbb {E} [ | N _ {t} ^ {n} - N _ {t} | | N _ {t} ^ {n} + N _ {t} | ].\tag{12.7}
$$

By Cauchy-Schwarz this is less than 

$$
\left\| N _ {t} ^ {n} - N _ {t} \right\| \left\| N _ {t} ^ {n} + N _ {t} \right\|.
$$

since $\| N _ { t } ^ { n } + N _ { t } \| \leq \| N _ { t } ^ { n } \| + \| N _ { t } \|$ is bounded independently of $n ,$ , we see that the left hand side of (12.7) tends to 0. 

Note 5. We have $\| N ^ { n } - N \| \to 0$ , where the norm is described in Note 3. This means that 

$$
\mathbb {E} \left[ \sup _ {t} | N _ {t} ^ {n} - N _ {t} | ^ {2} \right] \to 0.
$$

A result from measure theory implies that there exists a subsequence $n _ { k }$ such that 

$$
\sup _ {t} \left| N _ {t} ^ {n _ {k}} - N _ {t} \right| ^ {2} \to 0, \qquad \mathsf {a . s .}
$$

So except for a set of ω’s of probability $0 , N _ { t } ^ { n _ { k } } ( \omega )$ converges to $N _ { t } ( \omega )$ uniformly. Each $N _ { t } ^ { n _ { k } } ( \omega )$ is continuous by Step 2, and the uniform limit of continuous functions is continuous, therefore $N _ { t } ( \omega )$ is a continuous function of t. Incidentally, this is the primary reason we considered Doob’s inequalities. 

Note 6. If M is a continuous martingale, $\mathbb { E } \left[ M _ { b } - M _ { a } \ | \ { \mathcal F } _ { a } \right] = \mathbb { E } \left[ M _ { b } \ | \ { \mathcal F } _ { a } \right] - M _ { a } =$ $M _ { a } - M _ { a } = 0$ . This is the analogue of Lemma 12.1(a). To show the analogue of Lemma 12.1(b), 

$$
\begin{array}{r l} & {\mathbb {E} \left[ (M _ {b} - M _ {a}) ^ {2} \mid \mathcal {F} _ {a} \right] = \mathbb {E} \left[ M _ {b} ^ {2} \mid \mathcal {F} _ {a} \right] - 2 \mathbb {E} \left[ M _ {b} M _ {a} \mid \mathcal {F} _ {a} \right] + \mathbb {E} \left[ M _ {a} ^ {2} \mid \mathcal {F} _ {a} \right]} \\ & {\qquad = \mathbb {E} \left[ M _ {b} ^ {2} \mid \mathcal {F} _ {a} \right] - 2 M _ {a} \mathbb {E} \left[ M _ {b} \mid \mathcal {F} _ {a} \right] + M _ {a} ^ {2}} \\ & {\qquad = \mathbb {E} \left[ M _ {b} ^ {2} - \langle M \rangle_ {b} \mid \mathcal {F} _ {a} \right] + \mathbb {E} \left[ \langle M \rangle_ {b} - \langle M \rangle_ {a} \mid \mathcal {F} _ {a} \right] + M _ {a} ^ {2} - \langle M \rangle_ {a}} \\ & {\qquad = \mathbb {E} \left[ \langle M \rangle_ {b} - \langle M \rangle_ {a} \mid \mathcal {F} _ {a} \right],} \end{array}
$$

since $M _ { t } ^ { 2 } - \langle M \rangle$ is a martingale. That 

$$
\mathbb {E} \left[ M _ {b} ^ {2} - M _ {a} ^ {2} \mid \mathcal {F} _ {a} \right] = \mathbb {E} \left[ \left<   M \right> _ {b} - \left<   M \right> _ {a} \mid \mathcal {F} _ {a} \right]
$$

is just a rewriting of 

$$
\mathbb {E} \left[ M _ {b} ^ {2} - \langle M \rangle_ {b} \mid \mathcal {F} _ {a} \right] = M _ {a} ^ {2} - \langle M \rangle_ {a} = \mathbb {E} \left[ M _ {a} ^ {2} - \langle M \rangle_ {a} \mid \mathcal {F} _ {a} \right].
$$

With these two properties in place of Lemma 12.1, replacing $W _ { s }$ by M and ds by $d \langle M \rangle _ { s }$ , the construction of the stochastic integral $\begin{array} { r } { \int _ { 0 } ^ { t } H _ { s } d M _ { s } } \end{array}$ goes through exactly as above. 

Note 7. If we let $\begin{array} { r } { T _ { K } = \operatorname* { i n f } \{ t > 0 : \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d \langle M \rangle _ { s } \geq K \} } \end{array}$ , the first time the integral is larger than or equal to $K$ , and we let $H _ { s } ^ { K } = H _ { s } 1 _ { ( s \leq T _ { K } ) }$ , then $\begin{array} { r } { \int _ { 0 } ^ { \infty } H _ { s } ^ { K } d \langle M \rangle _ { s } \leq K } \end{array}$ and there is no dificulty defining $\begin{array} { r } { N _ { t } ^ { K } = \int _ { 0 } ^ { t } H _ { s } ^ { K } } \end{array}$ dM for every t. One can show that if $t \le T _ { K }$ and $T _ { K _ { 2 } }$ , then $N _ { t } ^ { K _ { 1 } } = N _ { t } ^ { K _ { 2 } }$ a.s. If $\int _ { 0 } ^ { t } H _ { s } d \langle M \rangle$ s is finite for every t, then $T _ { K } \to \infty$ as $K  \infty$ . If we call the common value $N _ { t }$ , this allows one to define the stochastic integral $N _ { t }$ for each t in the case where the integral $\int _ { 0 } ^ { t } H _ { s } ^ { 2 } d \langle M \rangle$ is finite for every t, even if the expectation of the integral is s not. 

We can do something similar is $M _ { t }$ is a martingale but where we do not have E $\left. M \right. _ { \infty } <$ ∞. Let $S _ { K } = \operatorname* { i n f } \{ t : | M _ { t } | \geq K \}$ , the first time $\lvert M _ { t } \rvert$ is larger than or equal to K. If we let $M _ { t } ^ { K } = M _ { t \wedge S _ { K } }$ , where $t \wedge S _ { k } = \operatorname* { m i n } ( t , S _ { K } )$ , then one can show $M ^ { K }$ is a martingale bounded in absolute value by K. So we can define $\begin{array} { r } { J _ { t } ^ { K } = \int _ { 0 } ^ { t } H _ { s } d M _ { t } ^ { K } } \end{array}$ for every t, using the paragraph above to handle the wider class of $H ^ { \prime } { \mathsf { s } }$ , if necessary. Again, one can show that if $t \le S _ { K }$ and $t \le S _ { K _ { 2 } }$ , then the value of the stochastic integral will be the same no matter whether we use $M ^ { K _ { 1 } }$ or $M ^ { K _ { 2 } }$ as our martingale. We use the common value as a definition of the stochastic integral $J _ { t }$ . We have $S _ { K }  \infty$ as $K  \infty$ , so we have a definition of $J _ { t }$ for each t. 

Note 8. We only outline how the proof goes. To show 

$$
\int_ {0} ^ {t} H _ {s} d N _ {s} = \int_ {0} ^ {t} H _ {s} K _ {s} d W _ {s},\tag{12.8}
$$

one shows that (SEC.801) holds for $H _ { s }$ simple and then takes limits. To show this, it sufices to look at $H _ { s }$ elementary and use linearity. To show (12.8) for $H _ { s }$ elementary, first prove this in the case when $K _ { s }$ is elementary, use linearity to extend it to the case when K is simple, and then take limits to obtain it for arbitrary K. Thus one reduces the proof to showing (12.8) when both H and K are elementary. In this situation, one can explicitly write out both sides of the equation and see that they are equal. 

## 13. Ito’s formula.

Suppose $W _ { t }$ is a Brownian motion and $f : \mathbb { R } \to$ R is a $C ^ { 2 }$ function, that is, $f$ and its first two derivatives are continuous. Ito’s formula, which is sometime known as the change of variables formula, says that 

$$
f (W _ {t}) - f (W _ {0}) = \int_ {0} ^ {t} f ^ {\prime} (W _ {s}) d W _ {s} + \frac {1}{2} \int_ {0} ^ {t} f ^ {\prime \prime} (W _ {s}) d s.
$$

Compare this with the fundamental theorem of calculus: 

$$
f (t) - f (0) = \int_ {0} ^ {t} f ^ {\prime} (s) d s.
$$

In Ito’s formula we have a second order term to carry along. 

The idea behind the proof is quite simple. By Taylor’s theorem. 

$$
\begin{array}{l} f (W _ {t}) - f (W _ {0}) = \sum_ {i = 0} ^ {n - 1} [ f (W _ {(i + 1) t / n}) - f (W _ {i t / n}) ] \\ \qquad \approx \sum_ {i = 1} ^ {n - 1} f ^ {\prime} (W _ {i t / n}) (W _ {(i + 1) t / n} - W _ {i t / n}) \\ \qquad \qquad + \frac {1}{2} \sum_ {i = 0} ^ {n - 1} f ^ {\prime \prime} (W _ {i t / n}) (W _ {(i + 1) t / n} - W _ {i t / n}) ^ {2}. \end{array}
$$

The first sum on the right is approximately the stochastic integral and the second is approximately the quadratic variation. 

For a more general semimartingale $X _ { t } = M _ { t } + A _ { t }$ , Ito’s formula reads 

Theorem 13.1. If $f \in C ^ { 2 }$ , then 

$$
f (X _ {t}) - f (X _ {0}) = \int_ {0} ^ {t} f ^ {\prime} (X _ {s}) d X _ {s} + \frac {1}{2} \int_ {0} ^ {t} f ^ {\prime \prime} (X _ {s}) d \langle M \rangle_ {s}.
$$

Let us look at an example. Let $W _ { t }$ be Brownian motion, $X _ { t } = \sigma W _ { t } - \sigma ^ { 2 } t / 2$ , and $f ( x ) = e ^ { x }$ . Then $\langle X \rangle _ { t } = \langle \sigma W \rangle _ { t } = \sigma ^ { 2 } t , f ^ { \prime } ( x ) = f " ( x ) = e ^ { x }$ , and 

$$
\begin{array}{r l} & e ^ {\sigma W _ {t} - \sigma^ {2} t / 2} = 1 + \int_ {0} ^ {t} e ^ {X _ {s}} \sigma d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} e ^ {X _ {s}} \frac {1}{2} \sigma^ {2} d s \\ & \qquad + \frac {1}{2} \int_ {0} ^ {t} e ^ {X _ {s}} \sigma^ {2} d s \\ & \qquad = 1 + \int_ {0} ^ {t} e ^ {X _ {s}} \sigma d W _ {s}. \end{array}\tag{13.1}
$$

This example will be revisited many times later on. 

Let us give another example of the use of Ito’s formula. Let $X _ { t } ~ = ~ W _ { t }$ and let $f ( x ) = x ^ { k }$ . Then $f ^ { \prime } ( x ) = k x ^ { k - 1 }$ and $f ^ { \prime \prime } ( x ) = k ( k - 1 ) x ^ { k - 2 }$ . We then have 

$$
\begin{array}{r} W _ {t} ^ {k} = W _ {0} ^ {k} + \int_ {0} ^ {t} k W _ {s} ^ {k - 1} d W _ {s} + \frac {1}{2} \int_ {0} ^ {t} k (k - 1) W _ {s} ^ {k - 2} d \langle W \rangle_ {s} \\ = \int_ {0} ^ {t} k W _ {s} ^ {k - 1} d W _ {s} + \frac {k (k - 1)}{2} \int_ {0} ^ {t} W _ {s} ^ {k - 2} d s. \end{array}
$$

When $k = 3$ , this says $\begin{array} { r } { W _ { t } ^ { 3 } - 3 \int _ { 0 } ^ { t } W _ { s } } \end{array}$ ds is a stochastic integral with respect to a Brownian motion, and hence a martingale. 

For a semimartingale $X _ { t } = M _ { t } + A _ { t }$ we set $\langle X \rangle _ { t } = \langle M \rangle _ { t }$ . Given two semimartingales $X , Y .$ , we define 

$$
\langle X, Y \rangle_ {t} = \frac {1}{2} [ \langle X + Y \rangle_ {t} - \langle X \rangle_ {t} - \langle Y \rangle_ {t} ].
$$

The following is known as Ito’s product formula. It may also be viewed as an integration by parts formula. 

Proposition 13.2. If $X _ { t }$ and $Y _ { t }$ are semimartingales, 

$$
X _ {t} Y _ {t} = X _ {0} Y _ {0} + \int_ {0} ^ {t} X _ {s} d Y _ {s} + \int_ {0} ^ {t} Y _ {s} d X _ {s} + \langle X, Y \rangle_ {t}.
$$

Proof. Applying Ito’s formula with $f ( x ) = x ^ { 2 }$ to $X _ { t } + Y _ { t }$ , we obtain 

$$
(X _ {t} + Y _ {t}) ^ {2} = (X _ {0} + Y _ {0}) ^ {2} + 2 \int_ {0} ^ {t} (X _ {s} + Y _ {s}) (d X _ {s} + d Y _ {s}) + \langle X + Y \rangle_ {t}.
$$

Applying Ito’s formula with $f ( x ) = x ^ { 2 }$ to X and to $Y$ , then 

$$
X _ {t} ^ {2} = X _ {0} ^ {2} + 2 \int_ {0} ^ {t} X _ {s} d X _ {s} + \langle X \rangle_ {t}
$$

and 

$$
Y _ {t} ^ {2} = Y _ {0} ^ {2} + 2 \int_ {0} ^ {t} Y _ {s} d Y _ {s} + \left\langle Y \right\rangle_ {t}.
$$

Then some algebra and the fact that 

$$
X _ {t} Y _ {t} = \frac {1}{2} [ (X _ {t} + Y _ {t}) ^ {2} - X _ {t} ^ {2} - Y _ {t} ^ {2} ]
$$

yields the formula. 

There is a multidimensional version of Ito’s formula: if $X _ { t } ~ = ~ ( X _ { t } ^ { 1 } , \ldots , X _ { t } ^ { d } )$ is a vector, each component of which is a semimartingale, and $f \in C ^ { 2 }$ , then 

$$
f (X _ {t}) - f (X _ {0}) = \sum_ {i = 1} ^ {d} \int_ {0} ^ {t} \frac {\partial f}{\partial x _ {i}} (X _ {s}) d X _ {s} ^ {i} + \frac {1}{2} \sum_ {i, j = 1} ^ {d} \int_ {0} ^ {t} \frac {\partial^ {2} f}{\partial x _ {i} ^ {2}} (X _ {s}) d \langle X ^ {i}, X ^ {j} \rangle_ {s}.
$$

The following application of Ito’s formula, known as L´evy’s theorem, is important. 

Theorem 13.3. Suppose $M _ { t }$ is a continuous martingale with $\langle M \rangle _ { t } = t$ . Then M is a Brownian motion. 

Before proving this, recall from undergraduate probability that the moment generating function of a r.v. X is defined by $m _ { X } ( a ) = \mathbb { E } e ^ { a X }$ and that if two random variables have the same moment generating function, they have the same law. This is also true if we replace a by iu. In this case we have $\varphi _ { X } ( u ) = \mathbb { E } e ^ { i u X }$ and $\varphi _ { X }$ is called the characteristic function of X. The reason for looking at the characteristic function is that $\varphi _ { X }$ always exists, whereas $m _ { X } ( a )$ might be infinite. The one special case we will need is that if X is a normal $\mathrm { { r . v . } }$ with mean 0 and variance t, then $\varphi _ { X } ( u ) = e ^ { - u ^ { 2 } t / 2 }$ . This follows from the formula for $m _ { X } ( a )$ with a replaced by iu (this can be justified rigorously). 

Proof. We will prove that $M _ { t }$ is a $\mathcal { N } ( 0 , t ) ;$ for the remainder of the proof see Note 1. 

We apply Ito’s formula with $f ( x ) = e ^ { i u x }$ . Then 

$$
e ^ {i u M _ {t}} = 1 + \int_ {0} ^ {t} i u e ^ {i u M _ {s}} d M _ {s} + \frac {1}{2} \int_ {0} ^ {t} (- u ^ {2}) e ^ {i u M _ {s}} d \langle M \rangle_ {s}.
$$

Taking expectations and using $\langle M \rangle _ { s } ~ = ~ s$ and the fact that a stochastic integral is a martingale, hence has 0 expectation, we have 

$$
\mathbb {E} e ^ {i u M _ {t}} = 1 - \frac {u ^ {2}}{2} \int_ {0} ^ {t} e ^ {i u M _ {s}} d s.
$$

Let $J ( t ) = \mathbb { E } e ^ { i u M _ { t } }$ . The equation can be rewritten 

$$
J (t) = 1 - \frac {u ^ {2}}{2} \int_ {0} ^ {t} J (s) d s.
$$

So $J ^ { \prime } ( t ) = - \textstyle { \frac { 1 } { 2 } } u ^ { 2 } J ( t )$ with $J ( 0 ) = 1$ . The solution to this elementary ODE is $J ( t ) =$ $e ^ { - u ^ { 2 } t / 2 }$ . Since 

$$
\mathbb {E} e ^ {i u M _ {t}} = e ^ {- u ^ {2} t / 2},
$$

then by our remarks above the law of $M _ { t }$ must be that of a $\mathcal { N } ( 0 , t )$ , which shows that $M _ { t }$ is a mean 0 variance t normal $\mathrm { { r . v } }$ □ 

Note 1. If $A \in \mathcal { F } _ { s }$ and we do the same argument with $M _ { t }$ replaced by $M _ { s + t } - M _ { s }$ , we have 

$$
e ^ {i u (M _ {s + t} - M _ {s})} = 1 + \int_ {0} ^ {t} i u e ^ {i u (M _ {s + r} - M _ {s})} d M _ {r} + \frac {1}{2} \int_ {0} ^ {t} (- u ^ {2}) e ^ {i u (M _ {s + r} - M _ {s})} d \langle M \rangle_ {r}.
$$

Multiply this by $1 _ { A }$ and take expectations. Since a stochastic integral is a martingale, the stochastic integral term again has expectation 0. If we let $K ( t ) = \mathbb { E } \left[ e ^ { i u \left( M _ { t + s } - M _ { t } \right) } ; A \right]$ ], we now arrive at $\begin{array} { r } { K ^ { \prime } ( t ) = - \frac { 1 } { 2 } u ^ { 2 } K ( t ) } \end{array}$ with $K ( 0 ) = \mathbb { P } ( A )$ , so 

$$
K (t) = \mathbb {P} (A) e ^ {- u ^ {2} t / 2}.
$$

Therefore 

$$
\mathbb {E} \left[ e ^ {i u (M _ {t + s} - M _ {s})}; A \right] = \mathbb {E} e ^ {i u (M _ {t + s} - M _ {s})} \mathbb {P} (A).\tag{13.2}
$$

If $f$ is a nice function and $\widehat { f }$ is its Fourier transform, replace u in the above by − $^ { \cdot u , }$ multiply by $\widehat { f } ( u )$ , and integrate over u. (To do the integral, we approximate the integral by a Riemann sum and then take limits.) We then have 

$$
\mathbb {E} \left[ f (M _ {s + t} - M _ {s}); A \right] = \mathbb {E} \left[ f ((M _ {s + t} - M _ {s}) ] \mathbb {P} (A). \right.
$$

By taking limits we have this for $f = 1 _ { B }$ , so 

$$
\mathbb {P} (M _ {s + t} - M _ {s} \in B, A) = \mathbb {P} (M _ {s + t} - M _ {s} \in B) \mathbb {P} (A).
$$

This implies that $M _ { s + t } - M _ { s }$ is independent of $\mathcal { F } _ { s }$ . 

Note Var $\left( M _ { t } - M _ { s } \right) = t - s ;$ take $A = \Omega$ in (13.2). 

## 14. The Girsanov theorem.

Suppose P is a probability and 

$$
d X _ {t} = d W _ {t} + \mu (X _ {t}) d t,
$$

where $W _ { t }$ is a Brownian motion. This is short hand for 

$$
X _ {t} = X _ {0} + W _ {t} + \int_ {0} ^ {t} \mu (X _ {s}) d s.\tag{14.1}
$$

Let 

$$
M _ {t} = \exp \Big (- \int_ {0} ^ {t} \mu (X _ {s}) d W _ {s} - \int_ {0} ^ {t} \mu (X _ {s}) ^ {2} d s / 2 \Big).\tag{14.2}
$$

Then as we have seen before, by Ito’s formula, $M _ { t }$ is a martingale. This calculation is reviewed in Note 1. We also observe that $M _ { 0 } = 1$ 

Now let us define a new probability by setting 

$$
\mathbb {Q} (A) = \mathbb {E} \left[ M _ {t}; A \right]\tag{14.3}
$$

if $A \in { \mathcal { F } } _ { t }$ . We had better be sure this $\mathbb { Q }$ is well defined. If $A \in \mathcal { F } _ { s } \subset \mathcal { F } _ { t }$ , then E $[ M _ { t } ; A ] =$ $\mathbb { E } \left[ M _ { s } ; A \right]$ because $M _ { t }$ is a martingale. We also check that $\mathbb { Q } ( \Omega ) = \mathbb { E } \left[ M _ { t } ; \Omega \right] = \mathbb { E } M _ { t }$ . This is equal to E $M _ { 0 } = 1$ , since $M _ { t }$ is a martingale. 

What the Girsanov theorem says is 

Theorem 14.1. Under $\mathbb { Q } , X _ { t }$ is a Brownian motion. 

Under P, $W _ { t }$ is a Brownian motion and $X _ { t }$ is not. Under $\mathbb { Q } ,$ the process $W _ { t }$ is no longer a Brownian motion. 

In order for a process $X _ { t }$ to be a Brownian motion, we need at a minimum that $X _ { t }$ is mean zero and variance t. To define mean and variance, we need a probability. Therefore a process might be a Brownian motion with respect to one probability and not another. Most of the other parts of the definition of being a Brownian motion also depend on the probability. 

Similarly, to be a martingale, we need conditional expectations, and the conditional expectation of a random variable depends on what probability is being used. 

There is a more general version of the Girsanov theorem. 

Theorem 14.2. If X is a martingale under $\mathbb { P } _ { i }$ , then under $\mathbb { Q }$ the process $X _ { t } - D _ { t }$ is a martingale where 

$$
D _ {t} = \int_ {0} ^ {t} \frac {1}{M _ {s}} d \langle X, M \rangle_ {s}.
$$

$\langle X \rangle _ { t }$ is the same under both $\mathbb { P }$ and $\mathbb { Q }$ . 

Let us see how Theorem 14.1 can be used. Let $S _ { t }$ be the stock price, and suppose 

$$
d S _ {t} = \sigma S _ {t} d W _ {t} + m S _ {t} d t.
$$

(So in the above formulation, $\mu ( x ) = m$ for all $x . )$ Define 

$$
M _ {t} = e ^ {(- m / \sigma) (W _ {t}) - (m ^ {2} / 2 \sigma^ {2}) t}.
$$

Then from (13.1) $M _ { t }$ is a martingale and 

$$
M _ {t} = 1 + \int_ {0} ^ {t} \Big (- \frac {m}{\sigma} \Big) M _ {s} d W _ {s}.
$$

Let $X _ { t } = W _ { t }$ . Then 

$$
\langle X, M \rangle_ {t} = \int_ {0} ^ {t} \Big (- \frac {m}{\sigma} \Big) M _ {s} d s = - \int_ {0} ^ {t} M _ {s} \frac {m}{\sigma} d s.
$$

Therefore 

$$
\int_ {0} ^ {t} \frac {1}{M _ {s}} d \langle X, M \rangle_ {s} = - \int_ {0} ^ {t} \frac {m}{\sigma} d s = - (m / \sigma) t.
$$

Define $\mathbb { Q }$ by (14.3). By Theorem 14.2, under $\mathbb { Q }$ the process $\widetilde { W } _ { t } = W _ { t } + ( m / \sigma ) t$ is a martingale. Hence 

$$
d S _ {t} = \sigma S _ {t} (d W _ {t} + (m / \sigma) d t) = \sigma S _ {t} d \widetilde {W} _ {t},
$$

or 

$$
S _ {t} = S _ {0} + \int_ {0} ^ {t} \sigma S _ {s} d \widetilde {W} _ {s}
$$

is a martingale. So we have found a probability under which the asset price is a martingale. This means that $\mathbb { Q }$ is the risk-neutral probability, which we have been calling $\overline { { \mathbb { P } } } .$ 

Let us give another example of the use of the Girsanov theorem. Suppose $X _ { t } =$ $W _ { t } + \mu t$ , where $\mu$ is a constant. We want to compute the probability that $X _ { t }$ exceeds the level a by time $t _ { 0 }$ 

We first need the probability that a Brownian motion crosses a level a by time $t _ { 0 }$ If $A _ { t } = \operatorname* { s u p } _ { s \leq t } W _ { t }$ , (note we are not looking at $\left| W _ { t } \right| )$ , we have 

$$
\mathbb {P} (A _ {t} > a, c \leq W _ {t} \leq d) = \int_ {c} ^ {d} \varphi (t, a, x),\tag{14.4}
$$

where 

$$
\varphi (t, a, x) = \left\{ \begin{array}{l l} \frac {1}{\sqrt {2 \pi t}} e ^ {- x ^ {2} / 2 t} & x \geq a \\ \frac {1}{\sqrt {2 \pi t}} e ^ {- (2 a - x) ^ {2} / 2 t} & x <   a. \end{array} \right.
$$

This is called the reflection principle, and the name is due to the derivation, given in Note 2. Sometimes one says 

$$
\mathbb {P} (W _ {t} = x, A _ {t} > a) = \mathbb {P} (W _ {t} = 2 a - x), \qquad x <   a,
$$

but this is not precise because $W _ { t }$ is a continuous random variable and both sides of the above equation are zero; (14.4) is the rigorous version of the reflection principle. 

Now let $W _ { t }$ be a Brownian motion under P. Let $d \mathbb { Q } / d \mathbb { P } = M _ { t } = e ^ { \mu W _ { t } - \mu ^ { 2 } t / 2 }$ . Let $Y _ { t } ~ = ~ W _ { t } - \mu t$ . Theorem 14.1 says that under $\mathbb { Q } , \ Y _ { t }$ is a Brownian motion. We have $W _ { t } = Y _ { t } + \mu t .$ 

Let $A = ( \operatorname* { s u p } _ { s \leq t _ { 0 } } W _ { s } \geq a )$ . We want to calculate 

$$
\mathbb {P} (\sup _ {s \leq t _ {0}} (W _ {s} + \mu s) \geq a).
$$

$W _ { t }$ is a Brownian motion under $\mathbb { P }$ while $Y _ { t }$ is a Brownian motion under $\mathbb { Q }$ . So this probability is equal to 

$$
\mathbb {Q} (\sup _ {s \leq t _ {0}} (Y _ {s} + \mu s) \geq a).
$$

This in turn is equal to 

$$
\mathbb {Q} (\sup _ {s \leq t _ {0}} W _ {s} \geq a) = \mathbb {Q} (A).
$$

Now we use the expression for $M _ { t }$ : 

$$
\begin{array}{r l} & {\mathbb {Q} (A) = \mathbb {E} _ {\mathbb {P}} [ e ^ {\mu W _ {t _ {0}} - \mu^ {2} t _ {0} / 2}; A ]} \\ & {\quad = \int_ {- \infty} ^ {\infty} e ^ {\mu x - \mu^ {2} t _ {0} / 2} \mathbb {P} (\underset {s \leq t _ {0}} {\sup} W _ {s} \geq a, W _ {t _ {0}} = x) d x} \\ & {\quad = e ^ {- \mu^ {2} t _ {0} / 2} \Big [ \int_ {- \infty} ^ {a} \frac {1}{\sqrt {2 \pi t _ {0}}} e ^ {\mu x} e ^ {- (2 a - x) ^ {2} / 2 t _ {0}} d x + \int_ {a} ^ {\infty} \frac {1}{\sqrt {2 \pi t _ {0}}} e ^ {\mu x} e ^ {- x ^ {2} / 2 t _ {0}} d x. \Big ]} \end{array}
$$

Proof of Theorem 14.1. Using Ito’s formula with $f ( x ) = e ^ { x }$ 

$$
M _ {t} = 1 - \int_ {0} ^ {t} \mu (X _ {r}) M _ {r} d W _ {r}.
$$

So 

$$
\langle W, M \rangle_ {t} = - \int_ {0} ^ {t} \mu (X _ {r}) M _ {r} d r.
$$

Since $\mathbb { Q } ( A ) = \mathbb { E } _ { \mathbb { P } } [ M _ { t } ; A ]$ , it is not hard to see that 

$$
\mathbb {E} _ {\mathbb {Q}} [ W _ {t}; A ] = \mathbb {E} _ {\mathbb {P}} [ M _ {t} W _ {t}; A ].
$$

$\mathrm { B y }$ Ito’s product formula this is 

$$
\mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {t} M _ {r} d W _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {t} W _ {r} d M _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} \Big [ \langle W, M \rangle_ {t}; A \Big ].
$$

Since $\begin{array} { r } { \int _ { 0 } ^ { t } M _ { r } d W _ { r } } \end{array}$ and $\begin{array} { r } { \int _ { 0 } ^ { t } W _ { r } d M _ { r } } \end{array}$ are stochastic integrals with respect to martingales, they are themselves martingales. Thus the above is equal to 

$$
\mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {s} M _ {r} d W _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {s} W _ {r} d M _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} \Big [ \langle W, M \rangle_ {t}; A \Big ].
$$

Using the product formula again, this is 

$$
\mathbb {E} _ {\mathbb {P}} [ M _ {s} W _ {s}; A ] + \mathbb {E} _ {\mathbb {P}} [ \langle W, M \rangle_ {t} - \langle W, M \rangle_ {s}; A ] = \mathbb {E} _ {\mathbb {Q}} [ W _ {s}; A ] + \mathbb {E} _ {\mathbb {P}} [ \langle W, M \rangle_ {t} - \langle W, M \rangle_ {s}; A ].
$$

The last term on the right is equal to 

$$
\begin{array}{r l} & {\mathbb {E} _ {\mathbb {P}} \Big [ \int_ {s} ^ {t} d \langle W, M \rangle_ {r}; A \Big ] = \mathbb {E} _ {\mathbb {P}} \Big [ - \int_ {s} ^ {t} M _ {r} \mu (X _ {r}) d r; A \Big ] = \mathbb {E} _ {\mathbb {P}} \Big [ - \int_ {s} ^ {t} \mathbb {E} _ {\mathbb {P}} [ M _ {t} \mid \mathcal {F} _ {r} ] \mu (X _ {r}) d r; A \Big ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {P}} \Big [ - \int_ {s} ^ {t} M _ {t} \mu (X _ {r}) d r; A \Big ] = \mathbb {E} _ {\mathbb {Q}} \Big [ - \int_ {s} ^ {t} \mu (X _ {r}) d r; A \Big ]} \\ & {\qquad = - \mathbb {E} _ {\mathbb {Q}} \Big [ \int_ {0} ^ {t} \mu (X _ {r}) d r; A \Big ] + \mathbb {E} _ {\mathbb {Q}} \Big [ \int_ {0} ^ {s} \mu (X _ {r}) d r; A \Big ].} \end{array}
$$

Therefore 

$$
\mathbb {E} _ {\mathbb {Q}} \left[ W _ {t} + \int_ {0} ^ {t} \mu (X _ {r}) d r; A \right] = \mathbb {E} _ {\mathbb {Q}} \left[ W _ {s} + \int_ {0} ^ {s} \mu (X _ {r}) d r; A \right],
$$

which shows $X _ { t }$ is a martingale with respect to $\mathbb { Q } .$ . 

Similarly, $X _ { t } ^ { 2 } - t$ is a martingale with respect to $\mathbb { Q } .$ . By L´evy’s theorem, $X _ { t }$ is a Brownian motion. □ 

In Note 3 we give a proof of Theorem 14.2 and in Note 4 we show how Theorem 14.1 is really a special case of Theorem 14.2. 

Note 1. Let 

$$
Y _ {t} = - \int_ {0} ^ {t} \mu (X _ {s}) d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} [ \mu (X _ {s}) ] ^ {2} d s.
$$

We apply Ito’s formula with the function $f ( x ) = e ^ { x }$ . Note the martingale part of $Y _ { t }$ is the stochastic integral term and the quadratic variation of $Y$ is the quadratic variation of the martingale part, so 

$$
\langle Y \rangle_ {t} = \int_ {0} ^ {t} [ - \mu (X _ {s}) ] ^ {2} d s.
$$

Then $f ^ { \prime } ( x ) = e ^ { x } , f ^ { \prime \prime } ( x ) = e ^ { x }$ , and hence 

$$
\begin{array}{r l} & M _ {t} = e ^ {Y _ {t}} = e ^ {Y _ {0}} + \int_ {0} ^ {t} e ^ {Y _ {s}} d Y _ {s} + \frac 12 \int_ {0} ^ {t} e ^ {Y _ {s}} d \langle Y \rangle_ {s} \\ & \quad = 1 + \int_ {0} ^ {t} M _ {s} (- \mu (X _ {s}) d W _ {s} - \frac 12 \int_ {0} ^ {t} [ \mu (X _ {s}) ] ^ {2} d s \\ & \qquad + \frac 12 \int_ {0} ^ {t} M _ {s} [ - \mu (X _ {s}) ] ^ {2} d s \\ & \quad = 1 - \int_ {0} ^ {t} M _ {s} \mu (X _ {s}) d W _ {s}. \end{array}
$$

Since stochastic integrals with respect to a Brownian motion are martingales, this completes the argument that $M _ { t }$ is a martingale. 

Note 2. Let $S _ { n }$ be a simple random walk. This means that $X _ { 1 } , X _ { 2 } , \ldots ,$ are independent and identically distributed random variables with $\begin{array} { r } { \mathbb { P } ( X _ { i } = 1 ) = \mathbb { P } ( X _ { i } = - 1 ) = \frac { 1 } { 2 } } \end{array}$ ; let $S _ { n } =$ $\textstyle \sum _ { i = 1 } ^ { n } X _ { i }$ . If you are playing a game where you toss a fair coin and win $1 if it comes up heads and lose $1 if it comes up tails, then $S _ { n }$ will be your fortune at time $n .$ . Let $A _ { n } = \operatorname* { m a x } _ { 0 \leq k \leq n } S _ { k }$ We will show the analogue of (14.4) for $S _ { n }$ , which is 

$$
\mathbb {P} (S _ {n} = x, A _ {n} \geq a) = \left\{ \begin{array}{l l} \mathbb {P} (S _ {n} = x) & x \geq a \\ \mathbb {P} (S _ {n} = 2 a - x) & x <   a. \end{array} \right.\tag{14.5}
$$

(14.4) can be derived from this using a weak convergence argument. 

To establish (14.5), note that if $x \geq a$ and $S _ { n } = x ,$ , then automatically $A _ { n } \geq a$ , so the only case to consider is when $x < a$ . Any path that crosses a but is at level x at time n has a corresponding path determined by reflecting across level a at the first time the Brownian motion hits $a ;$ the reflected path will end up $\ a + ( a - x ) = 2 a - x$ . The probability on the left hand side of (14.5) is the number of paths that hit a and end up at x divided by the total number of paths. Since the number of paths that hit a and end up at x is equal to the number of paths that end up at $2 a - x$ , then the probability on the left is equal to the number of paths that end up at $2 a - x$ divided by the total number of paths; this is $\mathbb { P } ( S _ { n } = 2 a - x )$ , which is the right hand side. 

Note 3. To prove Theorem 14.2, we proceed as follows. Assume without loss of generality that $X _ { 0 } = 0$ . Then if $A \in \mathcal { F } _ { s }$ 

$$
\begin{array}{r l} & {\mathbb {E} _ {\mathbb {Q}} [ X _ {t}; A ] = \mathbb {E} _ {\mathbb {P}} [ M _ {t} X _ {t}; A ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {t} M _ {r} d X _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {t} X _ {r} d M _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} [ \langle X, M \rangle_ {t}; A ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {s} M _ {r} d X _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {0} ^ {s} X _ {r} d M _ {r}; A \Big ] + \mathbb {E} _ {\mathbb {P}} [ \langle X, M \rangle_ {t}; A ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {Q}} [ X _ {s}; A ] + \mathbb {E} _ {\mathbb {Q}} [ \langle X, M \rangle_ {t} - \langle X, M \rangle_ {s}; A ].} \end{array}
$$

Here we used the fact that stochastic integrals with respect to the martingales X and M are again martingales. 

On the other hand, 

$$
\begin{array}{r l} & {\mathbb {E} _ {\mathbb {P}} [ \langle X, M \rangle_ {t} - \langle X, M \rangle_ {s}; A ] = \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {s} ^ {t} d \langle X, M \rangle_ {r}; A \Big ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {s} ^ {t} M _ {r} d D _ {r}; A \Big ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {s} ^ {t} \mathbb {E} _ {\mathbb {P}} [ M _ {t} | \mathcal {F} _ {r} ] d D _ {r}; A \Big ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {P}} \Big [ \int_ {s} ^ {t} M _ {t} d D _ {r}; A \Big ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {P}} [ (D _ {t} - D _ {s}) M _ {t}; A ]} \\ & {\qquad = \mathbb {E} _ {\mathbb {Q}} [ D _ {t} - D _ {s}; A ].} \end{array}
$$

The proof of the quadratic variation assertion is similar. 

## Note 4. Here is an argument showing how Theorem 14.1 can also be derived from Theorem 14.2.

From our formula for M we have $d M _ { t } = - M _ { t } \mu ( X _ { t } ) d W _ { t }$ , and therefore $d \langle X , M \rangle _ { t } =$ $M _ { t } \mu ( X _ { t } ) d t$ . Hence by Theorem 14.2 we see that under $\mathbb { Q } , X _ { t }$ is a continuous martingale with $\langle X \rangle _ { t } = t .$ . By ${ \mathsf { L e v y } } ^ { \prime } { \mathsf { s } }$ theorem, this means that X is a Brownian motion under $\mathbb { Q } .$ □ 

## 15. Stochastic diferential equations.

Let $W _ { t }$ be a Brownian motion. We are interested in the existence and uniqueness for stochastic diferential equations (SDEs) of the form 

$$
d X _ {t} = \sigma (X _ {t}) d W _ {t} + b (X _ {t}) d t, \qquad X _ {0} = x _ {0}.\tag{15.1}
$$

This means $X _ { t }$ satisfies 

$$
X _ {t} = x _ {0} + \int_ {0} ^ {t} \sigma (X _ {s}) d W _ {s} + \int_ {0} ^ {t} b (X _ {s}) d s.\tag{15.2}
$$

Here $W _ { t }$ is a Brownian motion, and (15.2) holds for almost every ω. 

We have to make some assumptions on $\sigma$ and b. We assume they are Lipschitz, which means: 

$$
| \sigma (x) - \sigma (y) | \leq c | x - y |, \quad | b (x) - b (y) | \leq c | x - y |
$$

for some constant c. We also suppose that $\sigma$ and b grow at most linearly, which means: 

$$
| \sigma (x) | \leq c (1 + | x |), \qquad | b (x) | \leq c (1 + | x |).
$$

Theorem 15.1. There exists one and only one solution to (15.2). 

The idea of the proof is Picard iteration, which is how existence and uniqueness for ordinary diferential equations is proved; see Note 1. 

The intuition behind (15.1) is that $X _ { t }$ behaves locally like a multiple of Brownian motion plus a constant drift: locally $X _ { t + h } - X _ { t } \approx \sigma ( W _ { t + h } - W _ { t } ) + b ( ( t + h ) - t )$ . However the constants $\sigma$ and b depend on the current value of $X _ { t }$ . When $X _ { t }$ is at diferent points, the coeficients vary, which is why they are written $\sigma ( X _ { t } )$ and $b ( X _ { t } )$ . σ is sometimes called the difusion coeficient and $\mu$ is sometimes called the drift coeficient. 

The above theorem also works in higher dimensions. We want to solve 

$$
d X _ {t} ^ {i} = \sum_ {j = 1} ^ {d} \sigma_ {i j} (X _ {s}) d W _ {s} ^ {j} + b _ {i} (X _ {s}) d s, \qquad i = 1, \ldots , d.
$$

This is an abbreviation for the equation 

$$
X _ {t} ^ {i} = x _ {0} ^ {i} + \int_ {0} ^ {t} \sum_ {j = 1} ^ {d} \sigma_ {i j} (X _ {s}) d W _ {s} ^ {j} + \int_ {0} ^ {t} b _ {i} (X _ {s}) d s.
$$

Here the initial value is $\boldsymbol { x } _ { 0 } = ( x _ { 0 } ^ { 1 } , \ldots , x _ { 0 } ^ { d } )$ , the solution process is $X _ { t } = ( X _ { t } ^ { 1 } , \ldots , X _ { t } ^ { d } )$ , and $W _ { t } ^ { 1 } , \ldots , W _ { t } ^ { d }$ are d independent Brownian motions. If all of the $\sigma _ { i j }$ and $b _ { i }$ are Lipschitz and grow at most linearly, we have existence and uniqueness for the solution. 

Suppose one wants to solve 

$$
d Z _ {t} = a Z _ {t} d W _ {t} + b Z _ {t} d t.
$$

Note that this equation is linear in $Z _ { t } ,$ and it turns out that linear equations are almost the only ones that have an explicit solution. In this case we can write down the explicit solution and then verify that it satisfies the SDE. The uniqueness result above (Theorem 15.1) shows that we have in fact found the solution. 

Let 

$$
Z _ {t} = Z _ {0} e ^ {a W _ {t} - a ^ {2} t / 2 + b t}.
$$

We will verify that this is correct by using Ito’s formula. Let $X _ { t } = a W _ { t } - a ^ { 2 } t / 2 + b t$ . Then $X _ { t }$ is a semimartingale with martingale part $a W _ { t }$ and $\langle X \rangle _ { t } = a ^ { 2 } t$ $Z _ { t } = e ^ { X _ { t } }$ $\mathrm { B y }$ Ito’s formula with $f ( x ) = e ^ { x }$ , 

$$
\begin{array}{r l} & Z _ {t} = Z _ {0} + \int_ {0} ^ {t} e ^ {X _ {s}} d X _ {s} + \frac {1}{2} \int_ {0} ^ {t} e ^ {X _ {s}} a ^ {2} d s \\ & \quad = Z _ {0} + \int_ {0} ^ {t} a Z _ {s} d W _ {s} - \int_ {0} ^ {t} \frac {a ^ {2}}{2} Z _ {s} d s + \int_ {0} ^ {t} b Z _ {s} d s \\ & \qquad + \frac {1}{2} \int_ {0} ^ {t} a ^ {2} Z _ {s} d s \\ & \quad = \int_ {0} ^ {t} a Z _ {s} d W _ {s} + \int_ {0} ^ {t} b Z _ {s} d s. \end{array}
$$

This is the integrated form of the equation we wanted to solve. 

There is a connection between SDEs and partial diferential equations. Let $f$ be a $C ^ { 2 }$ function. If we apply Ito’s formula, 

$$
f (X _ {t}) = f (X _ {0}) + \int_ {0} ^ {t} f ^ {\prime} (X _ {s}) d X _ {s} + \frac {1}{2} \int_ {0} ^ {t} f ^ {\prime \prime} (X _ {s}) d \langle X \rangle_ {s}.
$$

From (15.2) we know $\begin{array} { r } { \langle X \rangle _ { t } = \int _ { 0 } ^ { t } \sigma ( X _ { s } ) ^ { 2 } d s } \end{array}$ . If we substitute for $d X _ { s }$ and $d \langle X \rangle _ { s }$ , we obtain 

$$
\begin{array}{r l} & f (X _ {t}) = f (X _ {0}) + \int_ {0} ^ {t} f ^ {\prime} (X _ {s}) d W _ {s} + \int_ {0} ^ {t} \mu (X _ {s}) d s \\ & \qquad + \frac {1}{2} \int_ {0} ^ {t} f ^ {\prime \prime} (X _ {s}) \sigma (X _ {s}) ^ {2} d s \\ & \qquad = f (X _ {0}) + \int_ {0} ^ {t} f ^ {\prime} (X _ {s}) d W _ {s} + \int_ {0} ^ {t} \mathcal {L} f (X _ {s}) d s, \end{array}
$$

where we write 

$$
\mathcal {L} f (x) = \frac {1}{2} \sigma (x) ^ {2} f ^ {\prime \prime} (x) + \mu (x) f ^ {\prime} (x).
$$

$\mathcal { L }$ is an example of a diferential operator. Since the stochastic integral with respect to a Brownian motion is a martingale, we see from the above that 

$$
f (X _ {t}) - f (X _ {0}) - \int_ {0} ^ {t} \mathcal {L} f (X _ {s}) d s
$$

is a martingale. This fact can be exploited to derive results about PDEs from SDEs and vice versa. 

Note 1. Let us illustrate the uniqueness part, and for simplicity, assume b is identically 0 and σ is bounded. 

Proof of uniqueness. If X and $Y$ are two solutions, 

$$
X _ {t} - Y _ {t} = \int_ {0} ^ {t} [ \sigma (X _ {s}) - \sigma (Y _ {s}) ] d W _ {s}.
$$

So 

$$
\mathbb {E} \left| X _ {t} - Y _ {t} \right| ^ {2} = \mathbb {E} \int_ {0} ^ {t} | \sigma (X _ {s}) - \sigma (Y _ {s}) | ^ {2} d s \leq c \int_ {0} ^ {t} \mathbb {E} \left| X _ {s} - Y _ {s} \right| ^ {2} d s,
$$

using the Lipschitz hypothesis on $\sigma .$ . If we let $g ( t ) = \mathbb { E } | X _ { t } - Y _ { t } | ^ { 2 }$ , we have 

$$
g (t) \leq c \int_ {0} ^ {t} g (s) d s.
$$

Since we are assuming $\sigma$ is bounded, E $\begin{array} { r } { X _ { t } ^ { 2 } = \mathbb { E } \int _ { 0 } ^ { t } ( \sigma ( X _ { s } ) ) ^ { 2 } d s \leq c t } \end{array}$ and similarly for E $Y _ { t } ^ { 2 }$ , so $g ( t ) \leq c t$ . Then 

$$
g (t) \leq c \int_ {0} ^ {t} \left[ c \int_ {0} ^ {s} g (r) d r \right] d s.
$$

Iteration implies 

$$
g (t) \leq A t ^ {n} / n!
$$

for each $n ,$ , which implies $g$ must be 0. 

## 16. Continuous time financial models.

The most common model by far in finance is one where the security price is based on a Brownian motion. One does not want to say the price is some multiple of Brownian motion for two reasons. First, of all, a Brownian motion can become negative, which doesn’t make sense for stock prices. Second, if one invests $1,000 in a stock selling for $1 and it goes up to $2, one has the same profit, namely, $1,000, as if one invests $1,000 in a stock selling for $100 and it goes up to $200. It is the proportional increase one wants. 

Therefore one sets $\Delta S _ { t } / S _ { t }$ to be the quantity related to a Brownian motion. Diferent stocks have diferent volatilities $\sigma$ (consider a high-tech stock versus a pharmaceutical). In addition, one expects a mean rate of return $\mu$ on one’s investment that is positive (otherwise, why not just put the money in the bank?). In fact, one expects the mean rate of return to be higher than the risk-free interest rate r because one expects something in return for undertaking risk. 

So the model that is used is to let the stock price be modeled by the SDE 

$$
d S _ {t} / S _ {t} = \sigma d W _ {t} + \mu d t,
$$

or what looks better, 

$$
d S _ {t} = \sigma S _ {t} d W _ {t} + \mu S _ {t} d t.\tag{16.1}
$$

Fortunately this SDE is one of those that can be solved explicitly, and in fact we gave the solution in Section 15. 

Proposition 16.1. The solution to (16.1) is given by 

$$
S _ {t} = S _ {0} e ^ {\sigma W _ {t} + (\mu - (\sigma^ {2} / 2) t)}.\tag{16.2}
$$

Proof. Using Theorem 15.1 there will only be one solution, so we need to verify that $S _ { t }$ as given in (16.2) satisfies (16.1). We already did this, but it is important enough that we will do it again. Let us first assume $S _ { 0 } = 1$ . Let $X _ { t } = \sigma W _ { t } + ( \mu - ( \sigma ^ { 2 } / 2 ) t$ , let $f ( x ) = e ^ { x }$ and apply Ito’s formula. We obtain 

$$
\begin{array}{r l} & S _ {t} = e ^ {X _ {t}} = e ^ {X _ {0}} + \int_ {0} ^ {t} e ^ {X _ {s}} d X _ {s} + \frac 12 \int_ {0} ^ {t} e ^ {X _ {s}} d \langle X \rangle_ {s} \\ & \qquad = 1 + \int_ {0} ^ {t} S _ {s} \sigma d W _ {s} + \int_ {0} ^ {t} S _ {s} (\mu - \frac 12 \sigma^ {2}) d s \\ & \qquad \qquad + \frac 12 \int_ {0} ^ {t} S _ {s} \sigma^ {2} d s \\ & \qquad = 1 + \int_ {0} ^ {t} S _ {s} \sigma d W _ {s} + \int_ {0} ^ {t} S _ {s} \mu d s, \end{array}
$$

which is (16.1). If $S _ { 0 } \ne 0$ , just multiply both sides by $S _ { 0 }$ . 

Suppose for the moment that the interest rate r is 0. If one purchases $\Delta _ { 0 }$ shares (possibly a negative number) at time $t _ { 0 }$ , then changes the investment to $\Delta _ { 1 }$ shares at time $t _ { 1 } .$ , then changes the investment to $\Delta _ { 2 }$ at time $t _ { 2 } .$ , etc., then one’s wealth at time t will be 

$$
X _ {t _ {0}} + \Delta_ {0} (S _ {t _ {1}} - S _ {t _ {0}}) + \Delta_ {1} (S _ {t _ {2}} - S _ {t _ {1}}) + \dots + \Delta_ {i} (S _ {t _ {i + 1}} - S _ {t _ {i}}).\tag{16.3}
$$

To see this, at time $t _ { 0 }$ one has the original wealth $X _ { t _ { 0 } }$ . One buys $\Delta _ { 0 }$ shares and the cost is $\Delta _ { 0 } S _ { t _ { 0 } }$ . At time $t _ { 1 }$ one sells the $\Delta _ { 0 }$ shares for the price of $S _ { t _ { 1 } }$ per share, and so one’s wealth is now $X _ { t _ { 0 } } + \Delta _ { 0 } ( S _ { t _ { 1 } } - S _ { t _ { 0 } } )$ . One now pays $\Delta _ { 1 } S _ { t _ { 1 } }$ for $\Delta _ { 1 }$ shares at time $t _ { 1 }$ and continues. The right hand side of (16.3) is the same as 

$$
X _ {t _ {0}} + \int_ {t _ {0}} ^ {t} \Delta (s) d S _ {s},
$$

where we have $t \geq t _ { i + 1 }$ and $\Delta ( s ) = \Delta _ { i }$ for $t _ { i } \leq s < t _ { i + 1 }$ . In other words, our wealth is given by a stochastic integral with respect to the stock price. The requirement that the integrand of a stochastic integral be adapted is very natural: we cannot base the number of shares we own at time s on information that will not be available until the future. 

How should we modify this when the interest rate r is not zero? Let $P _ { t }$ be the present value of the stock price. So 

$$
P _ {t} = e ^ {- r t} S _ {t}.
$$

Note that $P _ { 0 } = S _ { 0 }$ . When we hold $\Delta _ { i }$ shares of stock from $t _ { i }$ to $t _ { i + 1 }$ , our profit in present days dollars will be 

$$
\Delta_ {i} (P _ {t _ {i + 1}} - P _ {t _ {i}}).
$$

The formula for our wealth then becomes 

$$
X _ {t _ {0}} + \int_ {t _ {0}} ^ {t} \Delta (s) d P _ {s}.
$$

By Ito’s product formula, 

$$
\begin{array}{r l} & {d P _ {t} = e ^ {- r t} d S _ {t} - r e ^ {- r t} S _ {t} d t} \\ & {\qquad = e ^ {- r t} \sigma S _ {t} d W _ {t} + e ^ {- r t} \mu S _ {t} d t - r e ^ {- r t} S _ {t} d t} \\ & {\qquad = \sigma P _ {t} d W _ {t} + (\mu - r) P _ {t} d t.} \end{array}
$$

Similarly to (16.2), the solution to this SDE is 

$$
P _ {t} = P _ {0} e ^ {\sigma W _ {t} + (\mu - r - \sigma^ {2} / 2) t}.\tag{16.4}
$$

The continuous time model of finance is that the security price is given by (16.1) (often called geometric Brownian motion), that there are no transaction costs, but one can trade as many shares as one wants and vary the amount held in a continuous fashion. This clearly is not the way the market actually works, for example, stock prices are discrete, but this model has proved to be a very good one. 

## 17. Markov properties of Brownian motion.

Let $W _ { t }$ be a Brownian motion. Because $W _ { t + r } - W _ { t }$ is independent of $\sigma ( W _ { s } : s \le t )$ then knowing the path of $W$ up to time s gives no help in predicting $W _ { t + r } \ : - \ : W _ { t }$ . In particular, if we want to predict $W _ { t + r }$ and we know $W _ { t }$ , then knowing the path up to time t gives no additional advantage in predicting $W _ { t + r }$ . Phrased another way, this says that to predict the future, we only need to know where we are and not how we got there. 

Let’s try to give a more precise description of this property, which is known as the Markov property. 

Fix r and let $Z _ { t } = W _ { t + r } - W _ { r }$ . Clearly the map $t  Z _ { t }$ is continuous since the same is true for W. Since $Z _ { t } - Z _ { s } = W _ { t + r } - W _ { s + r }$ then the distribution of $Z _ { t } - Z _ { s }$ is normal with mean zero and variance $( t + r ) - ( s + r )$ . One can also check the other parts of the definition to show that $Z _ { t }$ is also a Brownian motion. 

Recall that a stopping time in the continuous framework is a r.v. $T$ taking values in $[ 0 , \infty )$ such that $( T \leq t ) \in \mathcal { F } _ { t }$ for all t. To make a satisfactory theory, we need that the $\mathcal { F } _ { t }$ be right continuous (see Section 10), but this is fairly technical and we will ignore it. 

If T is a stopping time, $\mathcal { F } _ { T }$ is the collection of events A such that $A \cap ( T > t ) \in { \mathcal { F } } _ { t }$ for all t. 

Let us try to provide some motivation for this definition of $\mathcal { F } _ { T }$ . It will be simpler to consider the discrete time case. The analogue of $\mathcal { F } _ { T }$ in the discrete case is the following: if N is a stopping time, let 

$$
\mathcal {F} _ {N} = \{A: A \cap (N \leq k) \in \mathcal {F} _ {k} \text {   for   all   } k \}.
$$

If $X _ { k }$ is a sequence that is adapted to the σ-fields $\mathcal { F } _ { k }$ , that is, $X _ { k }$ is $\mathcal { F } _ { k }$ measurable when $k = 0 , 1 , 2 , . . . ,$ then knowing which events in $\mathcal { F } _ { k }$ have occurred allows us to calculate $X _ { k }$ for each k. So a reasonable definition of $\mathcal { F } _ { N }$ should allow us to calculate $X _ { N }$ whenever we know which events in $\mathcal { F } _ { N }$ have occurred or not. Or phrased another way, we want $X _ { N }$ to be $\mathcal { F } _ { N }$ measurable. Where did the sequence $X _ { k }$ come from? It could be any adapted sequence. Therefore one definition of the σ-field of events occurring before time N might be: 

Consider the collection of random variables $X _ { N }$ where $X _ { k }$ is a sequence adapted to $\mathcal { F } _ { k }$ . Let $\mathcal { G } _ { N }$ be the smallest σ-field with respect to which each of these random variables $X _ { N }$ is measurable. 

In other words, we want $\mathcal { G } _ { N }$ to be the σ-field generated by the collection of random variables $X _ { N }$ for all sequences $X _ { k }$ that are adapted to $\mathcal { F } _ { k }$ 

We show in Note 1 that $\mathcal { F } _ { N } = \mathcal { G } _ { N }$ . The σ-field $\mathcal { F } _ { N }$ is just a bit easier to work with. 

Now we proceed to the strong Markov property for Brownian motion, the proof of which is given in Note 2. 

Proposition 17.1. If $X _ { t }$ is a Brownian motion and $T$ is a bounded stopping time, then $X _ { T + t } - X _ { T }$ is a mean 0 variance t random variable and is independent of $\mathcal { F } _ { T }$ 

This proposition says: if you want to predict $X _ { T + t } ,$ , you could do it knowing all of $\mathcal { F } _ { T }$ or just knowing $X _ { T }$ . Since $X _ { T + t } - X _ { T }$ is independent of $\mathcal { F } _ { T }$ , the extra information given in $\mathcal { F } _ { T }$ does you no good at all. 

We need a way of expressing the Markov and strong Markov properties that will generalize to other processes. 

Let $W _ { t }$ be a Brownian motion. Consider the process $W _ { t } ^ { x } = x + W _ { t }$ , which is known as Brownian motion started at x. Define $\Omega ^ { \prime }$ to be set of continuous functions on $[ 0 , \infty )$ , let $X _ { t } ( \omega ) = \omega ( t )$ , and let the σ-field be the one generated by the $X _ { t }$ . Define $\mathbb { P } ^ { x }$ on $( \Omega ^ { \prime } , \mathcal { F } ^ { \prime } )$ by 

$$
\mathbb {P} ^ {x} (X _ {t _ {1}} \in A _ {1}, \dots , X _ {t _ {n}} \in A _ {n}) = \mathbb {P} (W _ {t _ {1}} ^ {x} \in A _ {1}, \dots , W _ {t _ {n}} ^ {x} \in A _ {n}).
$$

What we have done is gone from one probability space Ω with many processes $W _ { t } ^ { x }$ to one process $X _ { t }$ with many probability measures $\mathbb { P } ^ { x }$ 

An example in the Markov chain setting might help. No knowledge of Markov chains is necessary to understand this. Suppose we have a Markov chain with 3 states, A, B, and C. Suppose we have a probability $\mathbb { P }$ and three diferent Markov chains. The first, called $X _ { n } ^ { A }$ , represents the position at time n for the chain started at A. So $X _ { 0 } ^ { A } = A ,$ , and $X _ { 1 } ^ { A }$ can be one of $A , B , C , X _ { 2 } ^ { A }$ can be one of $A , B , C ,$ and so on. Similarly we have $X _ { n } ^ { B }$ , the chain started at B, and $X _ { n } ^ { C }$ . Define $\Omega ^ { \prime } \ = \ \{ ( A A A ) , ( A A B ) , ( A B A ) , \ldots , ( B A A ) , ( B A B ) , \ldots \}$ So $\Omega ^ { \prime }$ denotes the possible sequence of states for time $n = 0 , 1 , 2$ . If $\omega ~ = ~ A B A$ , set $Y _ { 0 } ( \omega ) = A , Y _ { 1 } ( \omega ) = B , Y _ { 2 } ( \omega ) = A ,$ , and similarly for all the other 26 values of ω. Define $\mathbb { P } ^ { A } ( A A A ) \ = \ \mathbb { P } ( X _ { 0 } ^ { A } \ = \ A , X _ { 1 } ^ { A } \ = \ A , X _ { 2 } ^ { A } \ = \ A )$ . Similarly define $\mathbb { P } ^ { A } ( A A B ) , \ldots$ Define $\mathbb { P } ^ { B } ( A A A ) = \mathbb { P } ( X _ { 0 } ^ { B } = A , X _ { 1 } ^ { B } = A , X _ { 2 } ^ { B } = A )$ (this will be 0 because we know $X _ { 0 } ^ { B } = B )$ , and similarly for the other values of ω. We also define $\mathbb { P } ^ { C }$ . So we now have one process, $Y _ { n } .$ , and three probabilities $\mathbb { P } ^ { A } , \mathbb { P } ^ { B } , \mathbb { P } ^ { C }$ . As you can see, there really isn’t all that much going on here. 

Here is another formulation of the Markov property. 

Proposition 17.2. $I f s < t$ and $f$ is bounded or nonnegative, then 

$$
\mathbb {E} ^ {x} [ f (X _ {t}) \mid \mathcal {F} _ {s} ] = \mathbb {E} ^ {X _ {s}} [ f (X _ {t - s}) ], \qquad \mathrm{a.s.}
$$

The right hand side is to be interpreted as follows. Define $\varphi ( x ) = \mathbb { E } ^ { x } f ( X _ { t - s } )$ . Then $\mathbb { E } ^ { X _ { s } } f ( X _ { t - s } )$ means $\varphi ( X _ { s } ( \omega ) )$ . One often writes $P _ { t } f ( x )$ for $\mathbb { E } ^ { x } f ( X _ { t } )$ . We prove this in Note 3. 

This formula generalizes: If $s < t < u$ , then 

$$
\mathbb {E} ^ {x} [ f (X _ {t}) g (X _ {u}) \mid \mathcal {F} _ {s} ] = \mathbb {E} ^ {X _ {s}} [ f (X _ {t - s}) g (X _ {u - s}) ],
$$

and so on for functions of X at more times. 

Using Proposition 17.1, the statement and proof of Proposition 17.2 can be extended to stopping times. 

Proposition 17.3. If T is a bounded stopping time, then 

$$
\mathbb {E} ^ {x} [ f (X _ {T + t}) \mid \mathcal {F} _ {T} ] = \mathbb {E} ^ {X _ {T}} [ f (X _ {t}) ].
$$

We can also establish the Markov property and strong Markov property in the context of solutions of stochastic diferential equations. If we let $X _ { t } ^ { x }$ denote the solution to 

$$
X _ {t} ^ {x} = x + \int_ {0} ^ {t} \sigma (X _ {s} ^ {x}) d W _ {s} + \int_ {0} ^ {t} b (X _ {s} ^ {x}) d s,
$$

so that $X _ { t } ^ { x }$ is the solution of the SDE started at $x ,$ we can define new probabilities by 

$$
\mathbb {P} ^ {x} (X _ {t _ {1}} \in A _ {1}, \ldots , X _ {t _ {n}} \in A _ {n}) = \mathbb {P} (X _ {t _ {1}} ^ {x} \in A _ {1}, \ldots , X _ {t _ {n}} ^ {x} \in A _ {n}).
$$

This is similar to what we did in defining $\mathbb { P } ^ { x }$ for Brownian motion, but here we do not have translation invariance. One can show that when there is uniqueness for the solution to the SDE, the family $( \mathbb { P } ^ { x } , X _ { t } )$ satisfies the Markov and strong Markov property. The statement is precisely the same as the statement of Proposition 17.3. 

Note 1. We want to show $\mathcal { G } _ { N } = \mathcal { F } _ { N }$ . Since $\mathcal { G } _ { N }$ is the smallest $\sigma \mathrm { - }$ field with respect to which $X _ { N }$ is measurable for all adapted sequences $X _ { k }$ and it is easy to see that $\mathcal { F } _ { N }$ is a σ-field, to show $\mathcal { G } _ { N } \subset \mathcal { F } _ { N }$ , it sufices to show that $X _ { N }$ is measurable with respect to $\mathcal { F } _ { N }$ whenever $X _ { k }$ is adapted. Therefore we need to show that for such a sequence $X _ { k }$ and any real number $^ { a , }$ the event $( X _ { N } > a ) \in \mathcal { F } _ { N }$ 

Now $( X _ { N } \ > \ a ) \cap ( N \ = \ j ) \ = ( X _ { j } \ > \ a ) \cap ( N \ = \ j )$ . The event $( X _ { j } \ > \ a ) \in \mathcal F _ { j }$ since X is an adapted sequence. Since N is a stopping time, then $( N \leq j ) \in \mathcal { F } _ { j }$ and $( N \leq j - 1 ) ^ { c } \in \mathcal { F } _ { j - 1 } \subset \mathcal { F } _ { j }$ , and so the event $( N = j ) = ( N \leq j ) \cap ( N \leq j - 1 ) ^ { c }$ is in ${ \mathcal { F } } _ { j }$ . If $j \le k$ , then $( N = j ) \in \mathcal { F } _ { j } \subset \mathcal { F } _ { k }$ . Therefore 

$$
(X _ {N} > a) \cap (N \leq k) = \cup_ {j = 0} ^ {k} ((X _ {N} > a) \cap (N = j)) \in \mathcal {F} _ {k},
$$

which proves that $( X _ { N } > a ) \in \mathcal { F } _ { N }$ 

To show $\mathcal { F } _ { N } \subset \mathcal { G } _ { N }$ , we suppose that $A \in \mathcal { F } _ { N }$ . Let $X _ { k } = 1 _ { A \cap ( N \leq k ) }$ . Since $A \in \mathcal { F } _ { N }$ then $A \cap ( N \leq k ) \in \mathcal { F } _ { k }$ , so $X _ { k }$ is $\mathcal { F } _ { k }$ measurable. But $X _ { N } = 1 _ { A \cap ( N \leq N ) } = 1 _ { A } , 5 0 ~ A = ( X _ { N } >$ $0 ) \in \mathcal { G } _ { N }$ . We have thus shown that $\mathcal { F } _ { N } \subset \mathcal { G } _ { N }$ , and combining with the previous paragraph, we conclude $\mathcal { F } _ { N } = \mathcal { G } _ { N }$ □ 

Note 2. Let $T _ { n }$ be defined by $T _ { n } ( \omega ) = ( k + 1 ) / 2 ^ { n } { \mathrm { ~ i f ~ } } T ( \omega ) \in [ k / 2 ^ { n } , ( k + 1 ) / 2 ^ { n } )$ . It is easy to check that $T _ { n }$ is a stopping time. Let $f$ be continuous and $A \in \mathcal { F } _ { T }$ . Then $A \in \mathcal { F } _ { T _ { n } }$ as well. We have 

$$
\begin{array}{r l} & {\mathbb {E} \left[ f (X _ {T _ {n} + t} - X _ {T _ {n}}); A \right] = \sum \mathbb {E} \left[ f (X _ {\frac {k}{2 ^ {n}} + t} - X _ {\frac {k}{2 ^ {n}}}); A \cap T _ {n} = k / 2 ^ {n} \right]} \\ & {\qquad = \sum \mathbb {E} \left[ f (X _ {\frac {k}{2 ^ {n}} + t} - X _ {\frac {k}{2 ^ {n}}}) \right] \mathbb {P} (A \cap T _ {n} = k / 2 ^ {n})} \\ & {\qquad = \mathbb {E} f (X _ {t}) \mathbb {P} (A).} \end{array}
$$

Let $n \to \infty$ , so 

$$
\mathbb {E} \left[ f (X _ {T + t} - X _ {T}); A \right] = \mathbb {E} f (X _ {t}) \mathbb {P} (A).
$$

Taking limits this equation holds for all bounded $f .$ 

If we take $A = \Omega$ and $f = 1 _ { B }$ , we see that $X _ { T + t } - X _ { T }$ has the same distribution as $X _ { t }$ which is that of a mean 0 variance t normal random variable. If we let $A \in \mathcal { F } _ { T }$ be arbitrary and $f = 1 _ { B }$ , we see that 

$$
\mathbb {P} (X _ {T + t} - X _ {T} \in B, A) = \mathbb {P} (X _ {t} \in B) \mathbb {P} (A) = \mathbb {P} (X _ {T + t} - X _ {T} \in B) \mathbb {P} (A),
$$

which implies that $X _ { T + t } - X _ { T }$ is independent of $\mathcal { F } _ { T }$ 

Note 3. Before proving Proposition 17.2, recall from undergraduate analysis that every bounded function is the limit of linear combinations of functions $e ^ { i u x } , \ u \in \mathbb { R }$ . This follows from using the inversion formula for Fourier transforms. There are various slightly diferent formulas for the Fourier transform. We use $\begin{array} { r } { \widehat { f } ( u ) = \int e ^ { i u x } f ( x ) } \end{array}$ dx. If $f$ is smooth enough and has compact support, then one can recover $f$ by the formula 

$$
f (x) = \frac {1}{2 \pi} \int e ^ {- i u x} \widehat {f} (u) d u.
$$

We can first approximate this improper integral by 

$$
\frac {1}{2 \pi} \int_ {- N} ^ {N} e ^ {- i u x} \widehat {f} (u) d u
$$

by taking $N$ larger and larger. For each $N$ we can approximate $\begin{array} { r } { \frac { 1 } { 2 \pi } \int _ { - N } ^ { N } e ^ { - i u x } \widehat { f } ( u ) } \end{array}$ du by using Riemann sums. Thus we can approximate $f ( x )$ by a linear combination of terms of the form $e ^ { i u _ { j } x }$ . Finally, bounded functions can be approximated by smooth functions with compact support. 

Proof. Let $f ( x ) = e ^ { i u x }$ . Then 

$$
\begin{array}{r} \mathbb {E} ^ {x} [ e ^ {i u X _ {t}} | \mathcal {F} _ {s} ] = e ^ {i u X _ {s}} \mathbb {E} ^ {x} [ e ^ {i u (X _ {t} - X _ {s})} | \mathcal {F} _ {s} ] \\ = e ^ {i u X _ {s}} e ^ {- u ^ {2} (t - s) / 2}. \end{array}
$$

On the other hand, 

$$
\varphi (y) = \mathbb {E} ^ {y} [ f (X _ {t - s}) ] = \mathbb {E} \left[ e ^ {i u (W _ {t - s} + y)} \right] = e ^ {i u y} e ^ {- u ^ {2} (t - s) / 2}.
$$

So $\varphi ( X _ { s } ) = \mathbb { E } ^ { x } [ e ^ { i u X _ { t } } \mid { \mathcal { F } } _ { s } ]$ . Using linearity and taking limits, we have the lemma for all $f . \ \sqcup$ 

## 18. Martingale representation theorem.

In this section we want to show that every random variable that is $\mathcal { F } _ { t }$ measurable can be written as a stochastic integral of Brownian motion. In the next section we use this to show that under the model of geometric Brownian motion the market is complete. This means that no matter what option one comes up with, one can exactly replicate the result (no matter what the market does) by buying and selling shares of stock. 

In mathematical terms, we let $\mathcal { F } _ { t }$ be the σ-field generated by $W _ { s } , s \leq t .$ . From (16.2) we see that $\mathcal { F } _ { t }$ is also the same as the σ-field generated by $S _ { s } , s \leq t ,$ so it doesn’t matter which one we work with. We want to show that if $V$ is $\mathcal { F } _ { t }$ measurable, then there exists $H _ { s }$ adapted such that 

$$
V = V _ {0} + \int H _ {s} d W _ {s},\tag{18.1}
$$

where $V _ { 0 }$ is a constant. 

Our goal is to prove 

Theorem 18.1. If V is $\mathcal { F } _ { t }$ measurable and E $V ^ { 2 } < \infty$ , then there exists a constant c and an adapted integrand $H _ { s }$ with E $\textstyle \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s < \infty$ such that 

$$
V = c + \int_ {0} ^ {t} H _ {s} d W _ {s}.
$$

Before we prove this, let us explain why this is called a martingale representation theorem. Suppose $M _ { s }$ is a martingale adapted to $\mathcal { F } _ { s }$ , where the $\mathcal { F } _ { s }$ are the σ-field generated by a Brownian motion. Suppose also that E $M _ { t } ^ { 2 } < \infty$ . Set $V = M _ { t }$ $\mathrm { B y }$ Theorem 18.1, we can write 

$$
M _ {t} = V = c + \int_ {0} ^ {t} H _ {s} d W _ {s}.
$$

The stochastic integral is a martingale, so for $r \leq t ,$ 

$$
M _ {r} = \mathbb {E} \left[ M _ {t} \mid \mathcal {F} _ {r} \right] = c + \mathbb {E} \left[ \int_ {0} ^ {t} H _ {s} d W _ {s} \mid \mathcal {F} _ {r} \right] = c + \int_ {0} ^ {r} H _ {s} d W _ {s}.
$$

We already knew that stochastic integrals were martingales; what this says is the converse: every martingale can be represented as a stochastic integral. Don’t forget that we need E $M _ { t } ^ { 2 } < \infty$ and $M _ { s }$ adapted to the σ-fields of a Brownian motion. 

In Note 1 we show that if every martingale can be represented as a stochastic integral, then every random variable V that is $\mathcal { F } _ { t }$ measurable can, too, provided E $V ^ { 2 } < \infty$ 

There are several proofs of Theorem 18.1. Unfortunately, they are all technical. We outline one proof here, giving details in the notes. We start with the following, proved in Note 2. 

Proposition 18.2. Suppose 

$$
V ^ {n} = c _ {n} + \int_ {0} ^ {t} H _ {s} ^ {n} d W _ {s},
$$

$$
c _ {n} \rightarrow c,
$$

$$
\mathbb {E} \left| V ^ {n} - V \right| ^ {2} \rightarrow 0,
$$

and for each n the process $H ^ { n }$ is adapted with E $\begin{array} { r } { \int _ { 0 } ^ { t } ( H _ { s } ^ { n } ) ^ { 2 } d s < \infty } \end{array}$ . Then there exist a constant c and an adapted H with E $\textstyle \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s < \infty$ so that 

$$
V _ {t} = c + \int_ {0} ^ {t} H _ {s} d W _ {s}.
$$

What this proposition says is that if we can represent a sequence of random variables $V _ { n }$ and $V _ { n } \to V ,$ , then we can represent V . 

Let R be the collection of random variables that can be represented as stochastic integrals. By this we mean 

$$
\begin{array}{r l} & {\mathcal {R} = \{V: \mathbb {E} V ^ {2} <   \infty , V \mathrm{is} \mathcal {F} _ {t} \mathrm{measurable}, V = c + \int_ {0} ^ {t} H _ {s} d W _ {s}} \\ & {\qquad \mathrm{forsomeadapted} H \mathrm{with} \mathbb {E} \int_ {0} ^ {t} H _ {s} ^ {2} d s <   \infty \}.} \end{array}
$$

Next we show $\mathcal { R }$ contains a particular collection of random variables. (The proof is in Note 3.) 

Proposition 18.3. ${ \mathit { I f } } { \mathit { g } }$ is bounded, the random variable $g ( W _ { t } )$ is in $\mathcal { R }$ . 

An almost identical proof shows that if f is bounded, then 

$$
f (W _ {t} - W _ {s}) = c + \int_ {s} ^ {t} H _ {r} d W _ {r}
$$

for some c and $H _ { r }$ 

Proposition 18.4. $I f t _ { 0 } \leq t _ { 1 } \leq \cdot \cdot \cdot \leq t _ { n } \leq t$ and $f _ { 1 } , \ldots , f _ { n }$ are bounded functions, then $f _ { 1 } ( W _ { t _ { 1 } } - W _ { t _ { 0 } } ) f _ { 2 } ( W _ { t _ { 2 } } - W _ { t _ { 1 } } ) \cdot \cdot \cdot f _ { n } ( W _ { t _ { n } } - W _ { t _ { n - 1 } } )$ is in R. 

See Note 4 for the proof. 

We now finish the proof of Theorem 18.1. We have shown that a large class of random variables is contained in R. 

Proof of Theorem 18.1. We have shown that random variables of the form 

$$
f _ {1} (W _ {t _ {1}} - W _ {t _ {0}}) f _ {2} (W _ {t _ {2}} - W _ {t _ {1}}) \dots f _ {n} (W _ {t _ {n}} - W _ {t _ {n - 1}})\tag{18.2}
$$

are in $\mathcal { R } .$ . Clearly if $V _ { i } \in \mathcal { R }$ for $i = 1 , \ldots , m$ , and $a _ { i }$ are constants, then $a _ { 1 } V _ { 1 } + \cdots a _ { m } V _ { m }$ is also in R. Finally, from measure theory we know that if E $V ^ { 2 } < \infty$ and V is $\mathcal { F } _ { t }$ measurable, we can find a sequence $V _ { k }$ such that E $| V _ { k } - V | ^ { 2 } \to 0$ and each $V _ { k }$ is a linear combination of random variables of the form given in (18.2). Now apply Proposition 18.2. □ 

Note 1. Suppose we know that every martingale $M _ { s }$ adapted to $\mathcal { F } _ { s }$ with E $M _ { t } ^ { 2 }$ can be represented as $\begin{array} { r } { M _ { r } = c + \int _ { 0 } ^ { r } H _ { s } d W _ { s } } \end{array}$ for some suitable H. If V is $\mathcal { F } _ { t }$ measurable with E $V ^ { 2 } < \infty$ let $M _ { r } = \mathbb { E } \left[ V \mid \mathcal { F } _ { r } \right]$ . We know this is a martingale, so 

$$
M _ {r} = c + \int_ {0} ^ {r} H _ {s} d W _ {s}
$$

for suitable H. Applying this with $r = t$ 

$$
V = \mathbb {E} \left[ V \mid \mathcal {F} _ {t} \right] = M _ {t} = c + \int_ {0} ^ {t} H _ {s} d W _ {s}.
$$

Note 2. We prove Proposition 18.2. By our assumptions, 

$$
\mathbb {E} \left| (V ^ {n} - c _ {n}) - (V ^ {m} - c _ {m}) \right| ^ {2} \to 0
$$

as n, $m \to \infty$ . So 

$$
\mathbb {E} \left| \int_ {0} ^ {t} (H _ {s} ^ {n} - H _ {s} ^ {m}) d W _ {s} \right| ^ {2} \to 0.
$$

From our formulas for stochastic integrals, this means 

$$
\mathbb {E} \int_ {0} ^ {t} | H _ {s} ^ {n} - H _ {s} ^ {m} | ^ {2} d s \to 0.
$$

This says that $H _ { s } ^ { n }$ is a Cauchy sequence in the space $L ^ { 2 }$ (with respect to the norm $\| \cdot \| _ { 2 } { \mathrm { ~ g i v e n } }$ by $\begin{array} { r } { \| Y \| _ { 2 } = \Big ( \mathbb { E } \int _ { 0 } ^ { t } Y _ { s } ^ { 2 } d s \Big ) ^ { 1 / 2 } \big ) } \end{array}$ . Measure theory tells us that $L ^ { 2 }$ is a complete metric space, so there exists $\dot { H } _ { s }$ such that 

$$
\mathbb {E} \int_ {0} ^ {t} | H _ {s} ^ {n} - H _ {s} | ^ {2} d s \to 0.
$$

In particular $H _ { s } ^ { n }  H _ { s }$ , and this implies $H _ { s }$ is adapted. Another consequence, due to Fatou’s lemma, is that E $\textstyle \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s$ 

Let $\begin{array} { r } { U _ { t } = \int _ { 0 } ^ { t } H _ { s } d W _ { s } } \end{array}$ . Then as above, 

$$
\mathbb {E} \left| (V ^ {n} - c _ {n}) - U _ {t} \right| ^ {2} = \mathbb {E} \int_ {0} ^ {t} (H _ {s} ^ {n} - H _ {s}) ^ {2} d s \rightarrow 0.
$$

Therefore $U _ { t } = V - c ,$ and U has the desired form. 

Note 3. Here is the proof of Proposition 18.3. By Ito’s formula with $X _ { s } = - i u W _ { s } + u ^ { 2 } s / 2$ and $f ( x ) = e ^ { x }$ 7 

$$
\begin{array}{c} e ^ {X _ {t}} = 1 + \int_ {0} ^ {t} e ^ {X _ {s}} (- i u) d W _ {s} + \int_ {0} ^ {t} e ^ {X _ {s}} (u ^ {2} / 2) d s \\ + \frac {1}{2} \int_ {0} ^ {t} e ^ {X _ {s}} (- i u) ^ {2} d s \\ = 1 - i u \int_ {0} ^ {t} e ^ {X _ {s}} d W _ {s}. \end{array}
$$

If we multiply both sides by $e ^ { - u ^ { 2 } t / 2 }$ , which is a constant and hence adapted, we obtain 

$$
e ^ {- i u W _ {t}} = c _ {u} + \int_ {0} ^ {t} H _ {s} ^ {u} d W _ {s}\tag{18.3}
$$

for an appropriate constant $c _ { u }$ and integrand $H ^ { u }$ 

If f is a smooth function $( \mathsf { e } . \mathsf { g } . , C ^ { \infty }$ with compact support), then its Fourier transform $\widehat { f }$ will also be very nice. So if we multiply (18.3) by $\widehat { f } ( u )$ and integrate over u from $- \infty$ to ∞, we obtain 

$$
f (W _ {t}) = c + \int_ {0} ^ {t} H _ {s} d W _ {s}
$$

for some constant c and some adapted integrand H. (We implicitly used Proposition 18.2, because we approximate our integral by Riemann sums, and then take a limit.) Now using Proposition 18.2 we take limits and obtain the proposition. □ 

Note 4. The argument is by induction; let us do the case $n = 2$ for clarity. So we suppose 

$$
V = f (W _ {t}) g (W _ {u} - W _ {t}).
$$

From Proposition 18.3 we now have that 

$$
f (W _ {t}) = c + \int_ {0} ^ {t} H _ {s} d W _ {s}, \qquad g (W _ {u} - W _ {t}) = d + \int_ {t} ^ {u} K _ {s} d W _ {s}.
$$

Set ${ \overline { { H } } } _ { r } = H _ { r } \ { \mathsf { i f } } \ 0 \leq s < t$ and 0 otherwise. Set $\overline { { K } } _ { r } = K _ { r }$ if $s \leq r < t$ and 0 otherwise. Let $\begin{array} { r } { X _ { s } = c + \int _ { 0 } ^ { s } \overline { { H } } _ { r } d W _ { r } } \end{array}$ and $\begin{array} { r } { Y _ { s } = d + \int _ { 0 } ^ { s } \overline { { K } } _ { r } d W _ { r } } \end{array}$ . Then 

$$
\langle X, Y \rangle_ {s} = \int_ {0} ^ {s} \overline {{H}} _ {r} \overline {{K}} _ {r} d r = 0.
$$

Then by the Ito product formula, 

$$
\begin{array}{r l} & X _ {s} Y _ {s} = X _ {0} Y _ {0} + \int_ {0} ^ {s} X _ {r} d Y _ {r} + \int_ {0} ^ {s} Y _ {r} d X _ {r} \\ & \qquad + \langle X, Y \rangle_ {s} \\ & \qquad = c d + \int_ {0} ^ {s} [ X _ {r} \overline {{K}} _ {r} + Y _ {r} \overline {{H}} _ {r} ] d W _ {r}. \end{array}
$$

If we now take $s = u ,$ that is exactly what we wanted. Note that $X _ { r } \overline { { K } } _ { r } + Y _ { r } \overline { { H } } _ { \ i }$ is 0 if $r > u ;$ this is needed to do the general induction step. □ 

## 19. Completeness.

Now let $P _ { t }$ be a geometric Brownian motion. As we mentioned in Section $^ { 1 6 , }$ if $P _ { t } = P _ { 0 } \exp ( \sigma W _ { t } + ( \mu - r - \sigma ^ { 2 } / 2 ) t )$ , then given $P _ { t }$ we can determine $W _ { t }$ and vice versa, so the σ fields generated by $P _ { t }$ and $W _ { t }$ are the same. Recall $P _ { t }$ satisfies 

$$
d P _ {t} = \sigma P _ {t} d W _ {t} + (\mu - r) P _ {t} d t.
$$

Define a new probability $\overline { { \mathbb { P } } }$ by 

$$
\frac {d \overline {{\mathbb {P}}}}{d \mathbb {P}} = M _ {t} = \exp (a W _ {t} - a ^ {2} t / 2).
$$

By the Girsanov theorem, 

$$
\widetilde {W} _ {t} = W _ {t} - a t
$$

is a Brownian motion under $\overline { { \mathbb { P } } } .$ So 

$$
d P _ {t} = \sigma P _ {t} d \widetilde {W} _ {t} + \sigma P _ {t} a d t + (\mu - r) P _ {t} d t.
$$

If we choose $a = - ( \mu - r ) / \sigma$ , we then have 

$$
d P _ {t} = \sigma P _ {t} d \widetilde {W _ {t}}.\tag{19.1}
$$

Since $\widetilde { W _ { t } }$ is $\mathrm { a }$ Brownian motion under ${ \overline { { \mathbb { P } } } } ,$ then $P _ { t }$ must be a martingale, since it is a stochastic integral of a Brownian motion. We can rewrite (19.1) as 

$$
d \widetilde {W} _ {t} = \sigma^ {- 1} P _ {t} ^ {- 1} d P _ {t}.\tag{19.2}
$$

Given a $\mathcal { F } _ { t }$ measurable variable $V ,$ , we know by Theorem 18.1 that there exist a constant and an adapted process $H _ { s }$ such that E $\textstyle \int _ { 0 } ^ { t } H _ { s } ^ { 2 } d s < \infty$ and 

$$
V = c + \int_ {0} ^ {t} H _ {s} d \widetilde {W} _ {s}.
$$

But then using (19.2) we have 

$$
V = c + \int_ {0} ^ {t} H _ {s} \sigma^ {- 1} P _ {s} ^ {- 1} d P _ {s}.
$$

We have therefore proved 

Theorem 19.1. $I f P _ { t }$ is a geometric Brownian motion and V is $\mathcal { F } _ { t }$ measurable and square integrable, then there exist a constant c and an adapted process $K _ { s }$ such that 

$$
V = c + \int_ {0} ^ {t} K _ {s} d P _ {s}.
$$

Moreover, there is a probability $\overline { { \mathbb { P } } }$ under which $P _ { t }$ is a martingale. 

The probability $\overline { { \mathbb { P } } }$ is called the risk-neutral measure. Under $\overline { { \mathbb { P } } }$ the present day value of the stock price is a martingale. 

## 20. Black-Scholes formula, I.

We can now derive the formula for the price of any option. Let $T \geq 0$ be a fixed real. If V is $\mathcal { F } _ { T }$ measurable, we have by Theorem 19.1 that 

$$
V = c + \int_ {0} ^ {T} K _ {s} d P _ {s},\tag{20.1}
$$

and under ${ \overline { { \mathbb { P } } } } ,$ the process $P _ { s }$ is a martingale. 

Theorem 20.1. The price of V must be $\overline { { \mathbb { E } V } }$ 

Proof. This is the “no arbitrage” principle again. Suppose the price of the option $V$ at time 0 is W. Starting with 0 dollars, we can sell the option V for W dollars, and use the W dollars to buy and trade shares of the stock. In fact, if we use c of those dollars, and invest according to the strategy of holding $K _ { s }$ shares at time $s ,$ then at time $T$ we will have 

$$
e ^ {r T} (W _ {0} - c) + V
$$

dollars. At time $T$ the buyer of our option exercises it and we use V dollars to meet that obligation. That leaves us a profit of $e ^ { r T } ( W _ { 0 } - c )$ if $W _ { 0 } > c ,$ without any risk. Therefore $W _ { 0 }$ must be less than or equal to c. If $W _ { 0 } < c ,$ we just reverse things: we buy the option instead of sell it, and hold $- K _ { s }$ <sub>s</sub> shares of stock at time s. By the same argument, since we can’t get a riskless profit, we must have $W _ { 0 } \geq c ,$ or $W _ { 0 } = c$ 

Finally, under $\overline { { \mathbb { P } } }$ the process $P _ { t }$ is a martingale. So taking expectations in (20.1), we obtain 

$$
\overline {{\mathbb {E}}} V = c.
$$

□ 

The formula in the statement of Theorem 20.1. is amenable to calculation. Suppose we have the standard European option, where 

$$
V = e ^ {- r t} (S _ {t} - K) ^ {+} = (e ^ {- r t} S _ {t} - e ^ {- r t} K) ^ {+} = (P _ {t} - e ^ {- r t} K) ^ {+}.
$$

Recall that under $\overline { { \mathbb { P } } }$ the stock price satisfies 

$$
d P _ {t} = \sigma P _ {t} d \widetilde {W} _ {t},
$$

where $\widetilde { W _ { t } }$ is a Brownian motion under ${ \overline { { \mathbb { P } } } } .$ So then 

$$
P _ {t} = P _ {0} e ^ {\sigma \widetilde {W} _ {t} - \sigma^ {2} t / 2}.
$$

Hence 

$$
\begin{array}{r} \overline {{\mathbb {E}}} V = \overline {{\mathbb {E}}} [ (P _ {T} - e ^ {- r T} K) ^ {+} ] \\ = \overline {{\mathbb {E}}} [ (P _ {0} e ^ {\sigma \widetilde {W} _ {T} - (\sigma^ {2} / 2) T} - e ^ {- r T} K) ^ {+} ]. \end{array}\tag{20.2}
$$

We know the density of $\widetilde { W _ { T } }$ is just $( 2 \pi T ) ^ { - 1 / 2 } e ^ { - y ^ { 2 } / ( 2 T ) }$ , so we can do some calculations (see Note 1) and end up with the famous Black-Scholes formula: 

$$
W _ {0} = x \Phi (g (x, T)) - K e ^ {- r T} \Phi (h (x, T)),
$$

where $\begin{array} { r } { \Phi ( z ) = \frac { 1 } { \sqrt { 2 \pi } } \int _ { - \infty } ^ { z } e ^ { - y ^ { 2 } / 2 } d y , x = P _ { 0 } = S _ { 0 } } \end{array}$ 

$$
g (x, T) = \frac {\log (x / K) + (r + \sigma^ {2} / 2) T}{\sigma \sqrt {T}},
$$

$$
h (x, T) = g (x, T) - \sigma \sqrt {T}.
$$

It is of considerable interest that the final formula depends on $\sigma$ but is completely independent of $\mu .$ . The reason for that can be explained as follows. Under $\overline { { \mathbb { P } } }$ the process $P _ { t }$ satisfies $d P _ { t } = \sigma P _ { t } d \widetilde { W } _ { t }$ , where $\widetilde { W _ { t } }$ is a Brownian motion. Therefore, similarly to formulas we have already done, 

$$
P _ {t} = P _ {0} e ^ {\sigma \widetilde {W} _ {t} - \sigma^ {2} t / 2},
$$

and there is no $\mu$ present here. (We used the Girsanov formula to get rid of the $\mu . )$ The price of the option $V$ is 

$$
\overline {{\mathbb {E}}} [ P _ {T} - e ^ {- r T} K ] ^ {+},\tag{20.3}
$$

which is independent of $\mu$ since $P _ { t }$ is. 

Note 1. We want to calculate 

$$
\overline {{E}} \Big [ (x e ^ {\sigma \widetilde {W} _ {T} - \sigma^ {2} T / 2} - e ^ {- r T} K) ^ {+} \Big ],\tag{20.4}
$$

where $\widetilde { W _ { t } }$ is a Brownian motion under $\overline { { P } }$ and we write x for $P _ { 0 } = S _ { 0 }$ . Since $\widetilde { W _ { T } }$ is a normal random vairable with mean 0 and variance $T$ , we can write it as $\sqrt { T } Z$ , where $Z$ is a standard mean 0 variance 1 normal random variable. 

Now 

$$
x e ^ {\sigma \sqrt {T} Z - \sigma^ {2} T / 2} > e ^ {- r T} K
$$

if and only if 

$$
\log x + \sigma \sqrt {T} Z - \sigma^ {2} T / 2 > - r + \log K,
$$

or if 

$$
Z > (\sigma^ {2} T / 2) - r + \log K - \log x.
$$

We write $z _ { 0 }$ for the right hand side of the above inequality. Recall that $1 - \Phi ( z ) = \Phi ( - z )$ for all z by the symmetry of the normal density. So (20.4) is equal to 

$$
\begin{array}{r l} & {\frac {1}{\sqrt {2 \pi}} \int_ {z _ {0}} ^ {\infty} (x e ^ {\sigma \sqrt {T} z - \sigma^ {2} T / 2} - e ^ {- r T} K) ^ {+} e ^ {- z ^ {2} / 2} d z} \\ & {\quad = x \frac {1}{\sqrt {2 \pi}} \int_ {z _ {0}} ^ {\infty} e ^ {- \frac {1}{2} (z ^ {2} - 2 \sigma \sqrt {T} z + \sigma^ {2} T} d z - K e ^ {- r T} \frac {1}{\sqrt {2 \pi}} \int_ {z _ {0}} ^ {\infty} e ^ {- z ^ {2} / 2} d z} \\ & {\quad = x \frac {1}{\sqrt {2 \pi}} \int_ {z _ {0}} ^ {\infty} e ^ {- \frac {1}{2} (z - \sigma \sqrt {T}) ^ {2}} d z - K e ^ {- r T} (1 - \Phi (z _ {0}))} \\ & {\quad = x \frac {1}{\sqrt {2 \pi}} \int_ {z _ {0} - \sigma \sqrt {T}} ^ {\infty} e ^ {- y ^ {2} / 2} d y - K e ^ {- r T} \Phi (- z _ {0})} \\ & {\quad = x (1 - \Phi (z _ {0} - \sigma \sqrt {T})) - K e ^ {- r T} \Phi (- z _ {0})} \\ & {\quad = x \Phi (\sigma \sqrt {T} - z _ {0}) - K e ^ {- r T} \Phi (- z _ {0}).} \end{array}
$$

This is the Black-Scholes formula if we observe that $\sigma { \sqrt { T } } - z _ { 0 } = g ( x , T )$ and $- z _ { 0 } = h ( x , T )$ 

## 21. Hedging strategies.

The previous section allows us to compute the value of any option, but we would also like to know what the hedging strategy is. This means, if we know $\begin{array} { r } { V = \overline { { \mathbb { E } } } V + \int _ { 0 } ^ { T } H _ { s } d S _ { s } , } \end{array}$ what should $H _ { s }$ be? This might be important to know if we wanted to duplicate an option that was not available in the marketplace, or if we worked for a bank and wanted to provide an option for sale. 

It is not always possible to compute H, but in many cases of interest it is possible. We illustrate one technique with two examples. 

First, suppose we want to hedge the standard European call $V = e ^ { - r T } ( S _ { T } - K ) ^ { + } =$ $( P _ { T } - e ^ { - r T } K ) ^ { \dagger }$ . We are working here with the risk-neutral probability only. It turns out it makes no diference: the definition of $\begin{array} { r } { \int _ { 0 } ^ { t } H _ { s } d X _ { s } } \end{array}$ for a semimartingale X does not depend on the probability P, other than worrying about some integrability conditions. 

We can rewrite V as 

$$
V = \overline {{\mathbb {E}}} V + g (\widetilde {W} _ {T}),
$$

where 

$$
g (x) = (e ^ {\sigma x - \sigma^ {2} T / 2} - e ^ {- r T} K) ^ {+} - \overline {{\mathbb {E}}} V.
$$

Therefore the expectation of $g ( \widetilde { W } _ { T } )$ is 0. Recall that under $\overline { { \mathbb { P } } } , \ \widetilde { W }$ is a Brownian motion. If we write $g ( \widetilde { W } _ { T } )$ as 

$$
\int_ {0} ^ {T} H _ {s} d \widetilde {W} _ {s},\tag{21.1}
$$

then since $d P _ { t } = \sigma P _ { t } d \widetilde { W } _ { t }$ , we have 

$$
g (\widetilde {W} _ {T}) = c + \int_ {0} ^ {T} \frac {1}{\sigma P _ {s}} H _ {s} d P _ {s}.\tag{21.2}
$$

Therefore it sufices to find the representation of the form (21.1). 

Recall from the section on the Markov property that 

$$
P _ {t} f (x) = \overline {{\mathbb {E}}} ^ {x} f (\widetilde {W} _ {t}) = \overline {{\mathbb {E}}} f (x + \widetilde {W} _ {t}) = \int \frac {1}{\sqrt {2 \pi t}} e ^ {- (y) ^ {2} / 2 t} f (x + y) d y.
$$

Let $M _ { t } = \overline { { \mathbb { E } } } \big [ g ( \widetilde { W } _ { T } ) \mid \mathcal { F } _ { t } \big ]$ . By Proposition 4.3, we know that $M _ { t }$ is a martingale. By the Markov property Proposition 17.2, we see that 

$$
M _ {t} = \overline {{\mathbb {E}}} ^ {\widetilde {W} _ {t}} [ g (\widetilde {W} _ {T - t} ] = P _ {T - t} g (\widetilde {W} _ {t}).\tag{21.3}
$$

Now let us apply Ito’s formula with the function $f ( x _ { 1 } , x _ { 2 } ) = P _ { x _ { 2 } } g ( x _ { 1 } )$ to the process $X _ { t } = ( X _ { t } ^ { 1 } , X _ { t } ^ { 2 } ) = ( \widetilde { W } _ { t } , T - t )$ . So we need to use the multidimensional version of Ito’s formula. We have $d X _ { t } ^ { 1 } = d \widetilde { W } _ { t }$ and $d X _ { t } ^ { 2 } = - d t$ . Since $X _ { t } ^ { 2 }$ is a decreasing process and has no martingale part, then $d \langle X ^ { 2 } \rangle _ { t } = 0$ and $d \langle X ^ { 1 } , X ^ { 2 } \rangle _ { t } = 0$ , while $d \langle X ^ { 1 } \rangle _ { t } = d t$ . Ito’s formula says that 

$$
\begin{array}{l} f (X _ {t} ^ {1}, X _ {t} ^ {2}) = f (X _ {0} ^ {1}, X _ {0} ^ {2}) + \int_ {0} ^ {t} \sum_ {i = 1} ^ {2} \frac {\partial f}{\partial x _ {i}} (X _ {t}) d X _ {t} ^ {i} \\ \qquad + \frac {1}{2} \int_ {0} ^ {t} \sum_ {i, j = 1} ^ {2} \frac {\partial^ {2} f}{\partial x _ {i} \partial x _ {j}} (X _ {t}) d \langle X ^ {i}, X ^ {j} \rangle_ {t} \\ \qquad = c + \int_ {0} ^ {t} \frac {\partial f}{\partial x _ {1}} (X _ {t}) d \widetilde {W _ {t}} + \text { some   terms   with } d t. \end{array}
$$

But we know that $f ( X _ { t } ) = P _ { T - t } g ( \widetilde { W } _ { t } ) = M _ { t }$ is a martingale, so the sum of the terms involving dt must be zero; if not, $f ( X _ { t } )$ would have a bounded variation part. We conclude 

$$
M _ {t} = \int_ {0} ^ {t} \frac {\partial}{\partial x} P _ {T - s} g (\widetilde {W} _ {s}) d \widetilde {W} _ {s}.
$$

If we take $t = T$ , we then have 

$$
g (\widetilde {W} _ {T}) = M _ {T} = \int_ {0} ^ {T} \frac {\partial}{\partial x} P _ {T - s} g (\widetilde {W} _ {s}) d \widetilde {W} _ {s},
$$

and we have our representation. 

For a second example, let’s look at the sell-high option. Here the payof is $\mathrm { s u p } _ { s \leq T } S _ { s }$ the largest the stock price ever is up to time T. This is $\mathcal { F } _ { T }$ measurable, so we can compute its value. How can one get the equivalent outcome without looking into the future? 

For simplicity, let us suppose the interest rate r is 0. Let $N _ { t } = \operatorname* { s u p } _ { s \leq t } S _ { s } ,$ , the maximum up to time t. It is not the case that $N _ { t }$ is a Markov process. Intuitively, the reasoning goes like this: suppose the maximum up to time 1 is $100, and we want to predict the maximum up to time 2. If the stock price at time 1 is close to $100, then we have one prediction, while if the stock price at time 1 is close to $\$ 2$ , we would definitely have another prediction. So the prediction for $N _ { 2 }$ does not depend just on $N _ { 1 }$ , but also the stock price at time 1. This same intuitive reasoning does suggest, however, that the triple $Z _ { t } = ( S _ { t } , N _ { t } , t )$ is a Markov process, and this turns out to be correct. Adding in the information about the current stock price gives a certain amount of evidence to predict the future values of $N _ { t } ;$ adding in the history of the stock prices up to time t gives no additional information. 

Once we believe this, the rest of the argument is very similar to the first example. Let $P _ { u } f ( z ) = \overline { { \mathbb { E } } } ^ { z } f ( Z _ { u } )$ , where $z = ( s , n , t )$ . Let $g ( Z _ { t } ) = N _ { t } - \overline { { \mathbb { E } } } N _ { T }$ . Then 

$$
M _ {t} = \overline {{\mathbb {E}}} [ g (Z _ {T}) \mid \mathcal {F} _ {t} ] = \overline {{\mathbb {E}}} ^ {Z _ {t}} [ g (Z _ {T - t}) ] = P _ {T - t} g (Z _ {t}).
$$

We then let $f ( s , n , t ) = P _ { T - t } g ( s , n , t )$ and apply Ito’s formula. The process $N _ { t }$ is always increasing, so has no martingale part, and hence $\langle N \rangle _ { t } = 0$ . When we apply Ito’s formula, we get a $d S _ { t }$ term, which is the martingale term, we get some terms involving $d t ,$ which are of bounded variation, and we get a term involving $d N _ { t }$ , which is also of bounded variation. But $M _ { t }$ is a martingale, so all the dt and $d N _ { t }$ terms must cancel. Therefore we should be left with the martingale term, which is 

$$
\int_ {0} ^ {t} \frac {\partial}{\partial s} P _ {T - s} g (S _ {s}, N _ {s}, s) d S _ {s},
$$

where again $g ( s , n , t ) = n$ . This gives us our hedging strategy for the sell-high option, and it can be explicitly calculated. 

There is another way to calculate hedging strategies, using what is known as the Clark-Haussmann-Ocone formula. This is a more complicated procedure, and most cases can be done as well by an appropriate use of the Markov property. 

## 22. Black-Scholes formula, II.

Here is a second approach to the Black-Scholes formula. This approach works for European calls and several other options, but does not work in the generality that the first approach does. On the other hand, it allows one to compute more easily what the equivalent strategy of buying or selling stock should be to duplicate the outcome of the given option. In this section we work with the actual price of the stock instead of the present value. 

Let $V _ { t }$ be the value of the portfolio and assume $V _ { t } = f ( S _ { t } , T - t )$ for all $t ,$ where f is some function that is suficiently smooth. We also want $V _ { T } = ( S _ { T } - K ) ^ { + }$ 

Recall Ito’s formula. The multivariate version is 

$$
f (X _ {t}) = f (X _ {0}) + \int_ {0} ^ {t} \sum_ {i = 1} ^ {d} f _ {x _ {i}} (X _ {s}) d X _ {s} ^ {i} + \frac {1}{2} \int_ {0} ^ {t} \sum_ {i, j = 1} ^ {d} f _ {x _ {i} x _ {j}} (X _ {s}) d \langle X ^ {i}, X ^ {j} \rangle_ {s}.
$$

Here $X _ { t } = ( X _ { t } ^ { 1 } , \ldots , X _ { t } ^ { d } )$ and $f _ { x _ { i } }$ denotes the partial derivative of $f$ in the $x _ { i }$ direction, and similarly for the second partial derivatives. 

We apply this with $d = 2$ and $X _ { t } ~ = ~ ( S _ { t } , T - t )$ . From the SDE that $S _ { t }$ solves, $d \langle X ^ { 1 } \rangle _ { t } ~ = ~ \sigma ^ { 2 } S _ { t } ^ { 2 } d t , ~ \langle X ^ { 2 } \rangle _ { t } ~ = ~ 0$ (since $T - t$ is of bounded variation and hence has no martingale part), and $\langle X ^ { 1 } , X ^ { 2 } \rangle _ { t } = 0$ . Also, $d X _ { t } ^ { 2 } = - d t$ . Then 

$$
\begin{array}{l} V _ {t} - V _ {0} = f (S _ {t}, T - t) - f (S _ {0}, T) \\ \qquad = \int_ {0} ^ {t} f _ {x} (S _ {u}, T - u) d S _ {u} - \int_ {0} ^ {t} f _ {s} (S _ {u}, T - u) d u \\ \qquad + \frac {1}{2} \int_ {0} ^ {t} \sigma^ {2} S _ {u} ^ {2} f _ {x x} (S _ {u}, T - u) d u. \end{array}\tag{22.1}
$$

On the other hand, if $a _ { u }$ and $b _ { u }$ are the number of shares of stock and bonds, respectively, held at time $u ,$ 

$$
V _ {t} - V _ {0} = \int_ {0} ^ {t} a _ {u} d S _ {u} + \int_ {0} ^ {t} b _ {u} d \beta_ {u}.\tag{22.2}
$$

This formula says that the increase in net worth is given by the profit we obtain by holding $a _ { u }$ shares of stock and $b _ { u }$ bonds at time u. Since the value of the portfolio at time t is 

$$
V _ {t} = a _ {t} S _ {t} + b _ {t} \beta_ {t},
$$

we must have 

$$
b _ {t} = (V _ {t} - a _ {t} S _ {t}) / \beta_ {t}.\tag{22.3}
$$

Also, recall 

$$
\beta_ {t} = \beta_ {0} e ^ {r t}.\tag{22.4}
$$

To match up (22.2) with (22.1), we must therefore have 

$$
a _ {t} = f _ {x} (S _ {t}, T - t)\tag{22.5}
$$

and 

$$
r [ f (S _ {t}, T - t) - S _ {t} f _ {x} (S _ {t}, T - t) ] = - f _ {s} (S _ {t}, T - t) + \frac {1}{2} \sigma^ {2} S _ {t} ^ {2} f _ {x x} (S _ {t}, T - t)\tag{22.6}
$$

for all t and all $S _ { t }$ . (22.6) leads to the parabolic PDE 

$$
f _ {s} = \frac {1}{2} \sigma^ {2} x ^ {2} f _ {x x} + r x f _ {x} - r f, \qquad (x, s) \in (0, \infty) \times [ 0, T),\tag{22.7}
$$

and 

$$
f (x, 0) = (x - K) ^ {+}.\tag{22.8}
$$

Solving this equation for $f , \ f ( x , T )$ is what $V _ { 0 }$ should be, i.e., the cost of setting up the equivalent portfolio. Equation (22.5) shows what the trading strategy should be. 

## 23. The fundamental theorem of finance.

In Section 19, we showed there was a probability measure under which $P _ { t } = e ^ { - r t } S _ { t }$ was a martingale. This is true very generally. Let $S _ { t }$ be the price of a security in today’s dollars. We will suppose $S _ { t }$ is a continuous semimartingale, and can be written $S _ { t } ~ =$ $M _ { t } + A _ { t }$ . 

Arbitrage means that there is a trading strategy $H _ { s }$ such that there is no chance that we lose anything and there is a positive profit with positive probability. Mathematically, arbitrage exists if there exists $H _ { s }$ that is adapted and satisfies a suitable integrability condition with T 

$$
\int_ {0} ^ {T} H _ {s} d S _ {s} \geq 0, \quad \mathrm{a.s.}
$$

and 

$$
\mathbb {P} \left(\int_ {0} ^ {T} H _ {s} d S _ {s} > b\right) > \varepsilon
$$

for some $b , \varepsilon > 0$ . It turns out that to get a necessary and suficient condition for $S _ { t }$ to be a martingale, we need a slightly weaker condition. 

The NFLVR condition $( ^ { 6 6 } \mathrm { n o }$ free lunch with vanishing $\mathrm { r i s k } ^ { \prime \prime } )$ is that there do not exist a fixed time $T , \ \varepsilon , b \ > \ 0$ , and $H _ { n }$ (that are adapted and satisfy the appropriate integrability conditions) such that 

$$
\int_ {0} ^ {T} H _ {n} (s) d S _ {s} > - \frac {1}{n}, \mathrm{a.s.}
$$

for all t and 

$$
\mathbb {P} \left(\int_ {0} ^ {T} H _ {n} (s) d S _ {s} > b\right) > \varepsilon .
$$

Here $T , b , \varepsilon$ do not depend on n. The condition says that one can with positive probability $\varepsilon$ make a profit of b and with a loss no larger than $1 / n$ 

Two probabilities P and $\mathbb { Q }$ are equivalent if $\mathbb { P } ( A ) = 0 { \mathrm { ~ i f ~ } }$ and only $\mathbb { Q } ( A ) = 0$ i.e., the two probabilities have the same collection of sets of probability zero. $\mathbb { Q }$ is an equivalent martingale measure if $\mathbb { Q }$ is a probability measure, $\mathbb { Q }$ is equivalent to P, and $S _ { t }$ is a martingale under $\mathbb { Q }$ 

Theorem 23.1. If $S _ { t }$ is a continuous semimartingale and the NFLVR conditions holds, then there exists an equivalent martingale measure $\mathbb { Q }$ 

The proof is rather technical and involves some heavy-duty measure theory, so we will only point examine a part of it. Suppose that we happened to have $S _ { t } = W _ { t } + f ( t )$ , where $f ( t )$ is a deterministic increasing continuous function. To obtain the equivalent martingale measure, we would want to let 

$$
M _ {t} = e ^ {- \int_ {0} ^ {t} f ^ {\prime} (s) d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} (f ^ {\prime} (s)) ^ {2} d s}.
$$

In order for $M _ { t }$ to make sense, we need $f$ to be diferentiable. A result from measure theory says that if $f$ is not diferentiable, then we can find a subset A of $[ 0 , \infty )$ such that $\begin{array} { r } { \int _ { 0 } ^ { t } 1 _ { A } ( s ) d s = 0 } \end{array}$ but the amount of increase of $f$ over the set A is positive. This last statement is phrased mathematically by saying 

$$
\int_ {0} ^ {t} 1 _ {A} (s) d f (s) > 0,
$$

where the integral is a Riemann-Stieltjes (or better, a Lebesgue-Stieltjes) integral. Then if we hold $H _ { s } = 1 _ { A } ( s )$ shares at time $s ,$ our net profit is 

$$
\int_ {0} ^ {t} H _ {s} d S _ {s} = \int_ {0} ^ {t} 1 _ {A} (s) d W _ {s} + \int_ {0} ^ {t} 1 _ {A} (s) d f (s).
$$

The second term would be positive since this is the amount of increase of $f$ over the set $A .$ . The first term is $0 ,$ since $\begin{array} { r } { \mathbb { E } \left( \int _ { 0 } ^ { t } 1 _ { A } ( s ) d W _ { s } \right) ^ { 2 } = \int _ { 0 } ^ { t } 1 _ { A } ( s ) ^ { 2 } d s = 0 } \end{array}$ . So our net profit is nonrandom and positive, or in other words, we have made a net gain without risk. This contradicts “no arbitrage.” See Note 1 for more on this. 

Sometime Theorem 23.1 is called the first fundamental theorem of asset pricing. The second fundamental theorem is the following. 

Theorem 23.2. The equivalent martingale measure is unique if and only if the market is complete. 

We will not prove this. 

Note 1. We will not prove Theorem 23.1, but let us give a few more indications of what is going on. First of all, recall the Cantor set. This is where $E _ { 1 } = [ 0 , 1 ] , E _ { 2 }$ is the set obtained from $E _ { 1 }$ by removing the open interval $\big ( \frac { 1 } { 3 } , \frac { 2 } { 3 } \big ) , E _ { 3 }$ is the set obtained from $E _ { 2 }$ by removing the middle third from each of the two intervals making up $E _ { 2 }$ , and so on. The intersection, $E = \cap _ { n = 1 } ^ { \infty } E _ { n }$ , is the Cantor set, and is closed, nonempty, in fact uncountable, yet it contains no intervals. Also, the Lebesgue measure of A is 0. We set $A = E$ . Let $f$ be the Cantor-Lebesgue function. This is the function that is equal to 0 on $( - \infty , 0 ]$ , 1 on $[ 1 , \infty )$ , equal to $\begin{array} { l } { { \frac { 1 } { 2 } } } \end{array}$ on the interval $[ \frac { 1 } { 3 } , \frac { 2 } { 3 } ]$ , equal to ${ \frac { 1 } { 4 } } \ \mathsf { o n } \ \left[ { \frac { 1 } { 9 } } , \ { \frac { 2 } { 9 } } \right]$ , equal to $\frac 3 4$ on $\left[ { \frac { 7 } { 9 } } , { \frac { 8 } { 9 } } \right]$ , and is defined similarly on each interval making up the complement of A. It turns out we can define $f$ on A so that it is continuous, and one can show $\begin{array} { r } { \int _ { 0 } ^ { 1 } { 1 } _ { A } ( s ) d f ( s ) = 1 } \end{array}$ . So this A and $f$ provide a concrete example of what we were discussing. 

## 24. American puts.

The proper valuation of American puts is one of the important unsolved problems in mathematical finance. Recall that a European put pays out $( K - S _ { T } ) ^ { + }$ at time $T ,$ while an American put allows one to exercise early. If one exercises an American put at time $t < T$ , one receives $( K - S _ { t } ) ^ { + }$ . Then during the period $[ t , T ]$ one receives interest, and the amount one has is $( K - S _ { t } ) ^ { + } e ^ { r ( T - t ) }$ . In today’s dollars that is the equivalent of $( K - S _ { t } ) ^ { + } e ^ { - r t }$ . One wants to find a rule, known as the exercise policy, for when to exercise the put, and then one wants to see what the value is for that policy. Since one cannot look into the future, one is in fact looking for a stopping time τ that maximizes 

$$
\overline {{\mathbb {E}}} e ^ {- r \tau} (K - S _ {\tau}) ^ {+}.
$$

There is no good theoretical solution to finding the stopping time $\tau _ { : }$ , although good approximations exist. We will, however, discuss just a bit of the theory of optimal stopping, which reworks the problem into another form. 

Let $G _ { t }$ denote the amount you will receive at time t. For American puts, we set 

$$
G _ {t} = e ^ {- r t} (K - S _ {t}) ^ {+}.
$$

Our problem is to maximize $\overline { { \mathbb { E } G } }$ over all stopping times $\tau .$ 

We first need 

Proposition 24.1. If S and T are bounded stopping times with $S \le T$ and $M$ is a martingale, then 

$$
\mathbb {E} \left[ M _ {T} \mid \mathcal {F} _ {S} \right] = M _ {S}.
$$

Proof. Let $A \in { \mathcal { F } } _ { S }$ . Define U by 

$$
U (\omega) = \left\{ \begin{array}{l l} S (\omega) & \text { if } \omega \in A, \\ T (\omega) & \text { if } \omega \notin A. \end{array} \right.
$$

It is easy to see that U is a stopping time, so by Doob’s optional stopping theorem, 

$$
\mathbb {E} M _ {0} = \mathbb {E} M _ {U} = \mathbb {E} [ M _ {S}; A ] + \mathbb {E} [ M _ {T}; A ^ {c} ].
$$

Also, 

$$
\mathbb {E} M _ {0} = \mathbb {E} M _ {T} = \mathbb {E} [ M _ {T}; A ] + \mathbb {E} [ M _ {T}; A ^ {c} ].
$$

Taking the diference, E $[ M _ { T } ; A ] = \mathbb { E } \left[ M _ { s } ; A \right]$ , which is what we needed to show. □ 

Given two supermartingales $X _ { t }$ and $Y _ { t }$ , it is routine to check that $X _ { t } \wedge Y _ { t }$ is also a supermartingale. Also, if $X _ { t } ^ { n }$ are supermartingales with $X _ { t } ^ { n } \downarrow X _ { t } ,$ one can check that $X _ { t }$ is again a supermartingale. With these facts, one can show that given a process such as $G _ { t }$ , there is a least supermartingale larger than $G _ { t }$ 

So we define $W _ { t }$ to be a supermartingale (with respect to ${ \overline { { \mathbb { P } } } } _ { : }$ , of course) such that $W _ { t } \geq G _ { t }$ a.s for each t and if $Y _ { t }$ is another supermartingale with $Y _ { t } \geq G _ { t }$ for all $t ,$ then $W _ { t } \leq Y _ { t }$ for all t. We set $\overline { { \tau } } =$ inf $\{ t : W _ { t } = G _ { t } \}$ . We will show that τ is the solution to the problem of finding the optimal stopping time. Of course, computing $W _ { t }$ and $\overline { { \tau } }$ is another problem entirely. 

Let 

$$
\mathcal {T} _ {t} = \{\tau : \tau \text {   is   a   stopping   time }, t \leq \tau \leq T \}.
$$

Let 

$$
V _ {t} = \sup _ {\tau \in \mathcal {T} _ {t}} \overline {{\mathbb {E}}} [ G _ {\tau} \mid \mathcal {F} _ {t} ].
$$

Proposition 24.2. $V _ { t }$ is a supermartingale and $V _ { t } \geq G _ { t }$ for all $t .$ 

Proof. The fixed time t is a stopping time in $\mathcal { T } _ { t } ,$ so $V _ { t } \geq \overline { { \mathbb { E } } } \left[ G _ { t } \mid \mathcal { F } _ { t } \right] = G _ { t } ,$ , or $V _ { t } \geq G _ { t }$ . so we only need to show that $V _ { t }$ is a supermartingale. 

Suppose $s \ < \ t$ . Let $\pi$ be the stopping time in $\mathcal { T } _ { t }$ for which $V _ { t } ~ = ~ \overline { { \mathbb { E } } } [ G _ { \pi } ~ | ~ \mathcal { F } _ { t } ]$ $\pi \in \mathcal { T } _ { t } \subset \mathcal { T } _ { s }$ . Then 

$$
\overline {{\mathbb {E}}} [ V _ {t} \mid \mathcal {F} _ {s} ] = \overline {{\mathbb {E}}} [ G _ {\pi} \mid \mathcal {F} _ {s} ] \leq \sup _ {\tau \in \mathcal {T} _ {s}} \mathbb {E} [ G _ {\tau} \mid \mathcal {F} _ {s} ] = V _ {s}.
$$

Proposition 24.3. $I f Y _ { t }$ is a supermartingale with $Y _ { t } \geq G _ { t }$ for all $t ,$ then $Y _ { t } \geq V _ { t }$ 

Proof. $\operatorname { I f } \tau \in \tau _ { t } .$ , then since $Y _ { t }$ is a supermartingale, we have 

$$
\overline {{\mathbb {E}}} [ Y _ {\tau} \mid \mathcal {F} _ {t} ] \leq Y _ {t}.
$$

So 

$$
V _ {t} = \sup _ {\tau \in \mathcal {T} _ {t}} \overline {{\mathbb {E}}} [ G _ {\tau} \mid \mathcal {F} _ {t} ] \leq \sup _ {\tau \in \mathcal {T} _ {t}} \overline {{\mathbb {E}}} [ Y _ {\tau} \mid \mathcal {F} _ {t} ] \leq Y _ {t}.
$$

What we have shown is that $W _ { t }$ is equal to $V _ { t }$ . It remains to show that $\overline { { \tau } }$ is optimal. There may in fact be more than one optimal time, but in any case $\overline { { \tau } }$ is one of them. Recall we have $\mathcal { F } _ { 0 }$ is the $\sigma \cdot$ -field generated by $S _ { 0 }$ , and hence consists of only $\varnothing$ and Ω. 

Proposition 24.4. $\overline { { \tau } }$ is an optimal stopping time. 

Proof. Since $\mathcal { F } _ { 0 }$ is trivial, $\begin{array} { r } { V _ { 0 } = \operatorname* { s u p } _ { \tau \in { \mathcal { T } } _ { 0 } } \overline { { \mathbb { E } } } \left[ G _ { \tau } \ | \ { \mathcal { F } } _ { 0 } \right] = \operatorname* { s u p } _ { \tau } \overline { { \mathbb { E } } } \left[ G _ { \tau } \right] } \end{array}$ . Let $\sigma$ be a stopping time where the supremum is attained. Then 

$$
V _ {0} \geq \overline {{\mathbb {E}}} [ V _ {\sigma} \mid \mathcal {F} _ {0} ] = \overline {{\mathbb {E}}} [ V _ {\sigma} ] \geq \overline {{\mathbb {E}}} [ G _ {\sigma} ] = V _ {0}.
$$

Therefore all the inequalities must be equalities. Since $V _ { \sigma } \geq G _ { \sigma }$ , we must have $V _ { \sigma } = G _ { \sigma }$ Since $\overline { { \tau } }$ was the first time that $W _ { t }$ equals $G _ { t }$ and $W _ { t } = V _ { t }$ , we see that $\overline { { \tau } } \leq \sigma$ . Then 

$$
\overline {{\mathbb {E}}} [ G _ {\overline {{\tau}}} ] = \overline {{\mathbb {E}}} [ V _ {\overline {{\tau}}} ] \geq \overline {{E}} V _ {\sigma} = \overline {{\mathbb {E}}} G _ {\sigma}.
$$

Therefore the expected value of $G _ { \overline { { \tau } } }$ is as least as large as the expected value of $G _ { \sigma }$ , and hence $\overline { { \tau } }$ is also an optimal stopping time. □ 

The above representation of the optimal stopping problem may seem rather bizarre. However, this procedure gives good usable results for some optimal stopping problems. An example is where $G _ { t }$ is a function of just W . 

## 25. Term structure.

We now want to consider the case where the interest rate is nondeterministic, that is, it has a random component. To do so, we take another look at option pricing. 

Accumulation factor. Let $r ( t )$ be the (random) interest rate at time t. Let 

$$
\beta (t) = e ^ {\int_ {0} ^ {t} r (u) d u}
$$

be the accumulation factor. One dollar at time $T$ will be worth $1 / \beta ( T )$ in today’s dollars. 

Let $V = ( S _ { T } - K ) ^ { + }$ be the payof on the standard European call option at time $T$ with strike price $K$ , where $S _ { t }$ is the stock price. In today’s dollars it is worth, as we have seen, $V / \beta ( T )$ . Therefore the price of the option should be 

$$
\overline {{\mathbb {E}}} \left[ \frac {V}{\beta (T)} \right].
$$

We can also get an expression for the value of the option at time t. The payof, in terms of dollars at time t, should be the payof at time $T$ discounted by the interest or inflation rate, and so should be 

$$
e ^ {- \int_ {t} ^ {T} r (u) d u} (S _ {T} - K) ^ {+}.
$$

Therefore the value at time t is 

$$
\overline {{\mathbb {E}}} \Big [ e ^ {- \int_ {t} ^ {T} r (u) d u} (S _ {T} - K) ^ {+} \mid \mathcal {F} _ {t} \Big ] = \overline {{\mathbb {E}}} \Big [ \frac {\beta (t)}{\beta (T)} V \mid \mathcal {F} _ {t} \Big ] = \beta (t) \overline {{\mathbb {E}}} \Big [ \frac {V}{\beta (T)} \mid \mathcal {F} _ {t} \Big ].
$$

From now on we assume we have already changed to the risk-neutral measure and we write $\mathbb { P }$ instead of P. 

Zero coupon. A zero coupon bond with maturity date T pays $1 at time T and nothing before. This is equivalent to an option with payof value $V = 1$ . So its price at time $t ,$ as above, should be 

$$
B (t, T) = \beta (t) \mathbb {E} \left[ \frac {1}{\beta (T)} \mid \mathcal {F} _ {t} \right] = \mathbb {E} \left[ e ^ {- \int_ {t} ^ {T} r (u) d u} \mid \mathcal {F} _ {t} \right].
$$

Let’s derive the SDE satisfied by $B ( t , T )$ . Let $N _ { t } = \mathbb { E } \left[ 1 / \beta ( T ) \ | \ \mathcal { F } _ { t } \right]$ . This is a martingale. By the martingale representation theorem, 

$$
N _ {t} = \mathbb {E} \left[ 1 / \beta (T) \right] + \int_ {0} ^ {t} H _ {s} d W _ {s}
$$

for some adapted integrand $H _ { s }$ . So $B ( t , T ) = \beta ( t ) N _ { t }$ . Here T is fixed. By Ito’s product formula, 

$$
\begin{array}{r l} & {d B (t, T) = \beta (t) d N _ {t} + N _ {t} d \beta (t)} \\ & {\qquad = \beta (t) H _ {t} d W _ {t} + N _ {t} r (t) \beta (t) d t} \\ & {\qquad = \beta (t) H _ {t} d W _ {t} + B (t, T) r (t) d t,} \end{array}
$$

and we thus have 

$$
d B (t, T) = \beta (t) H _ {t} d W _ {t} + B (t, T) r (t) d t.\tag{25.1}
$$

Forward rates. We now discuss forward rates. If one holds $T$ fixed and graphs $B ( t , T )$ as a function of t, the graph will not clearly show the behavior of $^ r \cdot$ One sometimes specifies interest rates by what are known as forward rates. 

Suppose we want to borrow $\$ 1$ at time $T$ and repay it with interest at time $T + \varepsilon$ At the present time we are at time $t \leq T$ . Let us try to accomplish this by buying a zero coupon bond with maturity date $T$ and shorting $( { \mathrm { i . e . } }$ , selling) N zero coupon bonds with maturity date $T + \varepsilon$ . Our outlay of money at time t is 

$$
B (t, T) - N B (t, T + \varepsilon) = 0.
$$

If we set 

$$
N = B (t, T) / B (t, T + \varepsilon),
$$

our outlay at time t is 0. At time $T$ we receive $1. At time $T + \varepsilon$ we pay $B ( t , T ) / B ( t , T + \varepsilon )$ The efective rate of interest $R$ over the time period $T$ to $T + \varepsilon$ is 

$$
e ^ {\varepsilon R} = \frac {B (t , T)}{B (t , T + \varepsilon)}.
$$

Solving for $R ,$ we have 

$$
R = \frac {\log B (t , T) - \log B (t , T + \varepsilon)}{\varepsilon}.
$$

We now let $\varepsilon \to 0$ . We define the forward rate by 

$$
f (t, T) = - \frac {\partial}{\partial T} \log B (t, T).\tag{25.2}
$$

Sometimes interest rates are specified by giving $f ( t , T )$ instead of $B ( t , T )$ or $r ( t )$ 

Recovering B from $f .$ Let us see how to recover $B ( t , T )$ from $f ( t , T )$ . Integrating, we have 

$$
\begin{array}{c} \int_ {t} ^ {T} f (t, u) d u = - \int_ {t} ^ {T} \frac {\partial}{\partial u} \log B (t, u) d u = - \log B (t, u) | _ {u = t} ^ {u = T} \\ = - \log B (t, T) + \log B (t, t). \end{array}
$$

Since $B ( t , t )$ is the value of a zero coupon bond at time t which expires at time $t ,$ it is equal to 1, and its log is 0. Solving for $B ( t , T )$ , we have 

$$
B (t, T) = e ^ {- \int_ {t} ^ {T} f (t, u) d u}.\tag{25.3}
$$

Recovering r from $f .$ Next, let us show how to recover $r ( t )$ from the forward rates. We have cT 

$$
B (t, T) = \mathbb {E} \left[ e ^ {- \int_ {t} ^ {T} r (u) d u} \mid \mathcal {F} _ {t} \right].
$$

Diferentiating, 

$$
\frac {\partial}{\partial T} B (t, T) = \mathbb {E} \left[ - r (T) e ^ {- \int_ {t} ^ {T} r (u) d u} | \mathcal {F} _ {t} \right].
$$

Evaluating this when $T = t .$ , we obtain 

$$
\mathbb {E} \left[ - r (t) \mid \mathcal {F} _ {t} \right] = - r (t).\tag{25.4}
$$

On the other hand, from (25.3) we have 

$$
\frac {\partial}{\partial T} B (t, T) = - f (t, T) e ^ {- \int_ {t} ^ {T} f (t, u) d u}.
$$

$$
r (t) = f (t, t).
$$

Setting $T = t$ we obtain $- f ( t , t )$ . Comparing with (25.4) yields 

(25.5) 

## 26. Some interest rate models.

Heath-Jarrow-Morton model 

Instead of specifying r, the Heath-Jarrow-Morton model (HJM) specifies the forward rates: 

$$
d f (t, T) = \sigma (t, T) d W _ {t} + \alpha (t, T) d t.\tag{26.1}
$$

Let us derive the SDE that $B ( t , T )$ satisfies. Let 

$$
\alpha^ {*} (t, T) = \int_ {t} ^ {T} \alpha (t, u) d u, \quad \sigma^ {*} (t, T) = \int_ {t} ^ {T} \sigma (t, u) d u.
$$

Since $\begin{array} { r } { B ( t , T ) = \exp ( - \int _ { t } ^ { T } f ( t , u ) d u ) } \end{array}$ , we derive the SDE for B by using Ito’s formula with the function $e ^ { x }$ and $\begin{array} { r } { X _ { t } = - \int _ { t } ^ { T } f ( t , u ) d u } \end{array}$ . We have 

$$
\begin{array}{r l} & {d X _ {t} = f (t, t) d t - \int_ {t} ^ {T} d f (t, u) d u} \\ & {\qquad = r (t) d t - \int_ {t} ^ {T} [ \alpha (t, u) d t + \sigma (t, u) d W _ {t} ] d u} \\ & {\qquad = r (t) d t - \Big [ \int_ {t} ^ {T} \alpha (t, u) d u \Big ] d t - \Big [ \int_ {t} ^ {T} \sigma (t, u) d u \Big ] d W _ {t}} \\ & {\qquad = r (t) d t - \alpha^ {*} (t, T) d t - \sigma^ {*} (t, T) d W _ {t}.} \end{array}
$$

Therefore, using Ito’s formula, 

$$
\begin{array}{c} d B (t, T) = B (t, T) d X _ {t} + \frac {1}{2} B (t, T) (\sigma^ {*} (t, T)) ^ {2} d t \\ = B (t, T) \Big [ r (t) - \alpha^ {*} + \frac {1}{2} (\sigma^ {*}) ^ {2} \Big ] d t - \sigma^ {*} B (t, T) d W _ {t}. \end{array}
$$

From (25.1) we know the dt term must be $B ( t , T ) r ( t ) d t$ , hence 

$$
d B (t, T) = B (t, T) r (t) d t - \sigma^ {*} B (t, T) d W _ {t}.
$$

Comparing with (26.1), we see that if P is the risk-neutral measure, we have $\begin{array} { r } { \alpha ^ { * } = \frac { 1 } { 2 } ( \sigma ^ { * } ) ^ { 2 } } \end{array}$ See Note 1 for more on this. 

Hull and White model 

In this model, the interest rate $r$ is specified as the solution to the SDE 

$$
d r (t) = \sigma (t) d W _ {t} + (a (t) - b (t) r (t)) d t.\tag{26.2}
$$

Here $\sigma , a ,$ b are deterministic functions. The stochastic integral term introduces randomness, while the $a - b r$ term causes a drift toward $a ( t ) / b ( t )$ . (Note that if $\sigma ( t ) = \sigma , a ( t ) =$ $a , b ( t ) = b$ are constants and $\sigma = 0$ , then the solution to (26.2) becomes $r ( t ) = a / b . )$ 

(26.2) is one of those SDE’s that can be solved explicitly. Let $\begin{array} { r } { K ( t ) = \int _ { 0 } ^ { t } b ( u ) d u } \end{array}$ Then 

$$
\begin{array}{r} d \Big [ e ^ {K (t)} r (t) \Big ] = e ^ {K (t)} r (t) b (t) d t + e ^ {K (t)} \Big [ a (t) - b (t) r (t) \Big ] d t + e ^ {K (t)} [ \sigma (t) d W _ {t} ] \\ = e ^ {K (t)} a (t) d t + e ^ {K (t)} [ \sigma (t) d W _ {t} ]. \end{array}
$$

Integrating both sides, 

$$
e ^ {K (t)} r (t) = r (0) + \int_ {0} ^ {t} e ^ {K (u)} a (u) d u + \int_ {0} ^ {t} e ^ {K (u)} \sigma (u) d W _ {u}.
$$

Multiplying both sides by $e ^ { - K ( t ) }$ , we have the explicit solution 

$$
r (t) = e ^ {- K (t)} \Big [ r (0) + \int_ {0} ^ {t} e ^ {K (u)} a (u) d u + \int_ {0} ^ {t} e ^ {K (u)} \sigma (u) d W _ {u} \Big ].
$$

If $F ( u )$ is deterministic, then 

$$
\int_ {0} ^ {t} F (u) d W _ {u} = \lim \sum F (u _ {i}) (W _ {u _ {i + 1}} - W _ {u _ {i}}).
$$

From undergraduate probability, linear combinations of Gaussian $\mathrm { r . v . \dot { s } }$ (Gaussian = normal) are Gaussian, and also limits of Gaussian r.v.’s are Gaussian, so we conclude that the r.v. $\begin{array} { r } { \int _ { 0 } ^ { t } F ( u ) d W _ { u } } \end{array}$ is Gaussian. We see that the mean at time t is 

$$
\mathbb {E} r (t) = e ^ {- K (t)} \left[ r (0) + \int_ {0} ^ {t} e ^ {K (u)} a (u) d u \right].
$$

We know how to calculate the second moment of a stochastic integral, so 

$$
\mathrm{Var} r (t) = e ^ {- 2 K (t)} \int_ {0} ^ {t} e ^ {2 K (u)} \sigma (u) ^ {2} d u.
$$

(One can similarly calculate the covariance of $r ( s )$ and $r ( t ) . )$ Limits of linear combinations of Gaussians are Gaussian, so we can calculate the mean and variance of $\begin{array} { r } { \int _ { 0 } ^ { T } r ( t ) d t } \end{array}$ and get an explicit expression for 

$$
B (0, T) = \mathbb {E} e ^ {- \int_ {0} ^ {T} r (u) d u}.
$$

## Cox-Ingersoll-Ross model

One drawback of the Hull and White model is that since $r ( t )$ is Gaussian, it can take negative values with positive probability, which doesn’t make sense. The Cox-Ingersoll-Ross model avoids this by modeling r by the SDE 

$$
d r (t) = (a - b r (t)) d t + \sigma \sqrt {r (t)} d W _ {t}.
$$

The diference from the Hull and White model is the square root of $r$ in the stochastic integral term. This square root term implies that when $r ( t )$ is small, the fluctuations in $r ( t )$ are larger than they are in the Hull and White model. Provided $a \geq { \textstyle { \frac { 1 } { 2 } } } \sigma ^ { 2 }$ , it can be shown that $r ( t )$ will never hit 0 and will always be positive. Although one cannot solve for r explicitly, one can calculate the distribution of $^ r \cdot$ . It turns out to be related to the square of what are known in probability theory as Bessel processes. (The density of $r ( t )$ for example, will be given in terms of Bessel functions.) 

Note 1. If P is not the risk-neutral measure, it is still possible that one exists. Let $\theta ( t )$ be a function of t, let $\begin{array} { r } { M _ { t } = \exp ( - \int _ { 0 } ^ { t } \theta ( u ) d W _ { u } - \frac { 1 } { 2 } \int _ { 0 } ^ { t } \theta ( u ) ^ { 2 } d u ) } \end{array}$ and define $\overline { { \mathbb { P } } } ( A ) = \mathbb { E } \left[ M _ { T } ; A \right]$ for $A \in \mathcal { F } _ { T }$ . By the Girsanov theorem, 

$$
d B (t, T) = B (t, T) \Big [ r (t) - \alpha^ {*} + \frac {1}{2} (\sigma^ {*}) ^ {2} + \sigma^ {*} \theta ] d t - \sigma^ {*} B (t, T) d \widetilde {W} _ {t},
$$

where $\widetilde { W _ { t } }$ is a Brownian motion under ${ \overline { { \mathbb { P } } } } .$ Again, comparing this with (25.1) we must have 

$$
\alpha^ {*} = \frac {1}{2} (\sigma^ {*}) ^ {2} + \sigma^ {*} \theta .
$$

Diferentiating with respect to $T ,$ , we obtain 

$$
\alpha (t, T) = \sigma (t, T) \sigma^ {*} (t, T) + \sigma (t, T) \theta (t).
$$

If we try to solve this equation for $\theta ,$ , there is no reason of-hand that θ depends only on t and not $T .$ . However, if θ does not depend on $T$ , P will be the risk-neutral measure. 

## Problems

1. Show $\mathbb { E } \left[ X \mathbb { E } \left[ Y \mid { \mathcal G } \right] \right] = \mathbb { E } \left[ Y \mathbb { E } \left[ X \mid { \mathcal G } \right] \right]$ 

2. Prove that ${ \mathbb { E } } \left[ a X _ { 1 } + b X _ { 2 } \mid { \mathcal { G } } \right] = a { \mathbb { E } } \left[ X _ { 1 } \mid { \mathcal { G } } \right] + b { \mathbb { E } } \left[ X _ { 2 } \mid { \mathcal { G } } \right] .$ 

3. Suppose $X _ { 1 } , X _ { 2 } , \ldots , X _ { n }$ are independent and for each i we have $\mathbb { P } ( X _ { i } = 1 )$ 

$\begin{array} { r } { \mathbb { = P } ( X _ { i } = - 1 ) = \frac { 1 } { 2 } } \end{array}$ . Let $\begin{array} { r } { S _ { n } = \sum _ { i = 1 } ^ { n } X _ { i } } \end{array}$ . Show that $M _ { n } = S _ { n } ^ { 3 } - 3 n S _ { n }$ is a martingale. 

4. Let $X _ { i }$ and $S _ { n }$ be as in Problem 3. Let $\begin{array} { r } { \phi ( x ) = \frac { 1 } { 2 } ( e ^ { x } + e ^ { - x } ) } \end{array}$ . Show that $M _ { n } = e ^ { a S _ { n } } \phi ( a ) ^ { - n }$ 2 is a martingale for each a real. 

5. Suppose $M _ { n }$ is a martingale, $N _ { n } = M _ { n } ^ { 2 }$ , and E $N _ { n } < \infty$ for each n. Show $\mathbb { E } \left[ N _ { n + 1 } \mid { \mathcal { F } } _ { n } \right] \geq N _ { n }$ for each n. Do not use Jensen’s inequality. 

6. Suppose $M _ { n }$ is a martingale, $N _ { n } = | M _ { n } |$ , and E $N _ { n } < \infty$ for each n. Show 

E $\left[ N _ { n + 1 } \mid { \mathcal { F } } _ { n } \right] \geq N _ { n }$ for each n. Do not use Jensen’s inequality. 

7. Suppose $X _ { n }$ is a martingale with respect to ${ \mathcal { G } } _ { n }$ and ${ \mathcal { F } } _ { n } = \sigma ( X _ { 1 } , \ldots , X _ { n } )$ . Show $X _ { n }$ is a martingale with respect to ${ \mathcal { F } } _ { n }$ 

8. Show that if $X _ { n }$ and $Y _ { n }$ are martingales with respect to $\{ \mathcal { F } _ { n } \}$ and $Z _ { n } = \operatorname* { m a x } ( X _ { n } , Y _ { n } )$ then $\mathbb { E } \left[ Z _ { n + 1 } \mid { \mathcal { F } } _ { n } \right] \geq Z _ { n }$ 

9. Let $X _ { n }$ and $Y _ { n }$ be martingales with E $X _ { n } ^ { 2 } < \infty$ and $\mathbb { E } Y _ { n } ^ { 2 } < \infty$ . Show 

$$
\mathbb {E} X _ {n} Y _ {n} - \mathbb {E} X _ {0} Y _ {0} = \sum_ {m = 1} ^ {n} \mathbb {E} (X _ {m} - X _ {m - 1}) (Y _ {m} - Y _ {m - 1}).
$$

10. Consider the binomial asset pricing model with $n = 3 , u = 3 , d = \textstyle { \frac { 1 } { 2 } } , r = 0 . 1 , S _ { 0 } = 2 0 \textstyle { \frac { 1 } { 2 } }$ , and $K = 1 0$ . If V is a European call with strike price K and exercise date n, compute explicitly the random variables $V _ { 1 }$ and $V _ { 2 }$ and calculate the value $V _ { 0 }$ 

11. In the same model as problem 1, compute the hedging strategy $\Delta _ { 0 } , \Delta _ { 1 }$ , and $\Delta _ { 2 }$ 

12. Show that in the binomial asset pricing model the value of the option V at time k is $V _ { k } .$ 

13. Suppose $X _ { n }$ is a submartingale. Show there exists a martingale $M _ { n }$ such that if $A _ { n } = X _ { n } - M _ { n } .$ , then $A _ { 0 } \leq A _ { 1 } \leq A _ { 2 } \leq \cdot \cdot \cdot$ and $A _ { n }$ is $\mathcal { F } _ { n - 1 }$ measurable for each n. 

14. Suppose $X _ { n }$ is a submartingale and $X _ { n } = M _ { n } + A _ { n } = M _ { n } ^ { \prime } + A _ { n } ^ { \prime }$ , where both $A _ { n }$ and $A _ { n } ^ { \prime }$ are $\mathcal { F } _ { n - 1 }$ measurable for each n, both M and M<sup>0</sup> are martingales, both $A _ { n }$ and $A _ { n } ^ { \prime }$ increase in $n ,$ , and $A _ { 0 } = A _ { 0 } ^ { \prime }$ . Show $M _ { n } = M _ { n } ^ { \prime }$ for each n. 

15. Suppose that S and $T$ are stopping times. Show that max(S, T) and min(S, T) are also stopping times. 

16. Suppose that $S _ { n }$ is a stopping time for each n and $S _ { 1 } \leq S _ { 2 } \leq \cdots$ . Show $S = \operatorname* { l i m } _ { n \to \infty } S _ { n }$ is also a stopping time. Show that if instead $S _ { 1 } \geq S _ { 2 } \geq \cdots$ and $S = \mathrm { l i m } _ { n  \infty } S _ { n } .$ , then $S$ is again a stopping time. 

17. Let $W _ { t }$ be Brownian motion. Show that $e ^ { i u W _ { t } + u ^ { 2 } t / 2 }$ can be written in the form $\begin{array} { r } { \int _ { 0 } ^ { t } H _ { s } d W _ { s } } \end{array}$ and give an explicit formula for $H _ { s }$ 

18. Suppose $M _ { t }$ is a continuous bounded martingale for which $\langle M \rangle _ { \infty }$ is also bounded. Show that 

$$
\sum_ {i = 0} ^ {2 ^ {n} - 1} (M _ {\frac {i + 1}{2 ^ {n}}} - M _ {\frac {i}{2 ^ {n}}}) ^ {2}
$$

converges to $\langle M \rangle _ { 1 }$ as $n \to \infty$ 

[Hint: Show that Ito’s formula implies 

$$
(M _ {\frac {i + 1}{2 ^ {n}}} - M _ {\frac {i}{2 ^ {n}}}) ^ {2} = \int_ {i / 2 ^ {n}} ^ {(i + 1) / 2 ^ {n}} (M _ {s} - M _ {\frac {i}{2 ^ {n}}}) d M _ {s} + \langle M \rangle_ {\frac {i + 1}{2 ^ {n}}} - \langle M \rangle_ {\frac {i}{2 ^ {n}}}.
$$

Then sum over i and show that the stochastic integral term goes to zero as $n  \infty . ]$ 

19. Let $f _ { \varepsilon } ( 0 ) = f _ { \varepsilon } ^ { \prime } ( 0 ) = 0$ and $\begin{array} { r } { f _ { \varepsilon } ^ { \prime \prime } ( x ) = \frac { 1 } { 2 \varepsilon } 1 _ { ( - \varepsilon , \varepsilon ) } ( x ) } \end{array}$ . You may assume that it is valid to use Ito’s formula with the function $f _ { \varepsilon }$ (note $f _ { \varepsilon } \notin C ^ { 2 } )$ ). Show that 

$$
\frac {1}{2 \varepsilon} \int_ {0} ^ {t} 1 _ {(- \varepsilon , \varepsilon)} (W _ {s}) d s
$$

converges as $\varepsilon \to 0$ to a continuous nondecreasing process that is not identically zero and that increases only when $X _ { t }$ is at 0. 

[Hint: Use Ito’s formula to rewrite $\begin{array} { r } { \frac { 1 } { 2 \varepsilon } \int _ { 0 } ^ { t } 1 _ { ( - \varepsilon , \varepsilon ) } ( W _ { s } ) d s } \end{array}$ in terms of $f _ { \varepsilon } ( W _ { t } ) - f _ { \varepsilon } ( W _ { 0 } )$ plus a stochastic integral term and take the limit in this formula.] 

20. Let $X _ { t }$ be the solution to 

$$
d X _ {t} = \sigma (X _ {t}) d W _ {t} + b (X _ {t}) d t, \qquad X _ {0} = x,
$$

where $W _ { t }$ is Brownian motion and σ and b are bounded $C ^ { \infty }$ functions and $\sigma$ is bounded below by a positive constant. Find a nonconstant function f such that $f ( X _ { t } )$ is a martingale. 

[Hint: Apply Ito’s formula to $f ( X _ { t } )$ and obtain an ordinary diferential equation that $f$ needs to satisfy.] 

21. Suppose $X _ { t } = W _ { t } + F ( t )$ , where $F$ is a twice continuously diferentiable function, $F ( 0 ) = 0$ , and $W _ { t }$ is a Brownian motion under P. Find a probability measure $\mathbb { Q }$ under which $X _ { t }$ is a Brownian motion and prove your statement. (You will need to use the general Girsanov theorem.) 

22. Suppose $\begin{array} { r } { X _ { t } = W _ { t } - \int _ { 0 } ^ { t } X _ { s } d s } \end{array}$ . Show that 

$$
X _ {t} = \int_ {0} ^ {t} e ^ {s - t} d W _ {s}.
$$

23. Suppose we have a stock where $\sigma = 2 , K = 1 5 , S _ { 0 } = 1 0 , r = 0 . 1$ , and $T = 3$ . Suppose we are in the continuous time model. Determine the price of the standard European call using the Black-Scholes formula. 

23. Let 

$$
\psi (t, x, y, \mu) = \mathbb {P} (\sup _ {s \leq t} (W _ {s} + \mu s) = y \text {   for   } s \leq t, W _ {t} = x),
$$

where $W _ { t }$ is a Brownian motion. More precisely, for each $A , B , C , D _ { \cdot }$ 27 

$$
\mathbb {P} (A \leq \sup _ {s \leq t} (W _ {s} + \mu s) \leq B, C \leq W _ {t} \leq D) = \int_ {C} ^ {D} \int_ {A} ^ {B} \psi (t, x, y, \mu) d y d x.
$$

(ψ has an explicit formula, but we don’t need that here.) Let the stock price $S _ { t }$ be given by the standard geometric Brownian motion. Let V be the option that pays of $\mathrm { s u p } _ { s < T } S _ { : }$ s at time T. Determine the price at time 0 of V as an expression in terms of $\psi .$ . 

25. Suppose the interest rate is 0 and $S _ { t }$ is the standard geometric Brownian motion stock price. Let A and B be fixed positive reals, and let V be the option that pays of 1 at time $T$ if $A \le S _ { T } \le B$ and 0 otherwise. 

(a) Determine the price at time 0 of $V$ . 

(b) Find the hedging strategy that duplicates the claim $V .$ 

26. Let V be the standard European call that has strike price K and exercise date $T$ . Let r and σ be constants, as usual, but let $\mu ( t )$ be a deterministic $( \mathrm { i . e . }$ , nonrandom) function. Suppose the stock price is given by 

$$
d S _ {t} = \sigma S _ {t} d W _ {t} + \mu (t) S _ {t} d t,
$$

where $W _ { t }$ is a Brownian motion. Find the price at time 0 of $V .$ . 