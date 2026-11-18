

<!-- === Source: MinerU_markdown_PartA1819Ch3-4_1_2122706447723769857.md (Page 1) === -->

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
\begin{array}{l}\mathbb {P} (W _ {n} = k) = \binom {n} {k} p _ {n} ^ {k} (1 - p _ {n}) ^ {n - k}\\\qquad = \binom {n} {k} \left(\frac {\lambda_ {n}}{n}\right) ^ {k} \left(1 - \frac {\lambda_ {n}}{n}\right) ^ {n - k}\\\qquad = \frac {n (n - 1) \cdots (n - k + 1)}{n ^ {k}} \frac {\lambda_ {n} ^ {k}}{k !} \left(1 - \frac {\lambda_ {n}}{n}\right) ^ {n} \left(1 - \frac {\lambda_ {n}}{n}\right) ^ {- k}\\\qquad \rightarrow 1 \cdot \frac {\lambda^ {k}}{k !} e ^ {- \lambda} \cdot 1\end{array}
$$

as $n  \infty ,$ as desired. 

# Generating functions

## 3.1 Review of probability generating functions

Let X be a random variable taking non-negative integer values, and let $p _ { X }$ be its probability mass function. The probability generating function of X is defined by 

$$
G (z) := \mathbb {E} \left(z ^ {X}\right) = \sum_ {k = 0} ^ {\infty} p _ {X} (k) z ^ {k}.
$$

G is a power series whose radius of convergence is at least 1. We can recover the coeficients of the power series, i.e. the values of the function $p _ { X }$ , from the behaviour of G and its derivatives at the point 0, and we can compute the moments of X from the behaviour of G and its derivatives at 1: 

Theorem 3.1. 

(a) $G ^ { ( k ) } ( 0 ) = k ! p _ { X } ( k ) f o r k = 0 , 1 , 2 , \ldots .$ 

(b) G(1) = 1 and G<sup>(k)</sup>(1) = E -X(X − 1) · · · (X − k + 1)] for k = 1, 2, . . . . 

Here if the radius of convergence of G is exactly 1, then $G ^ { ( k ) } ( 1 )$ should be taken to mean $\begin{array} { r } { \operatorname* { l i m } _ { z \uparrow 1 } G ^ { ( k ) } ( z ) } \end{array}$ . In this case, the limit may be finite or infinite. 

From Theorem $\mathrm { 3 . 1 ( a ) }$ , we see immediately that a distribution is determined by its generating function: 

Theorem 3.2 (Uniqueness theorem for probability generating functions). If X and Y have the same generating function, then they have the same distribution. 

From Theorem 3.1(b), we have, for example, $\operatorname { \mathbb { E } } \left( X \right) = G ^ { \prime } ( 1 ) , \operatorname { V a r } ( X ) = G ^ { \prime \prime } ( 1 ) + G ^ { \prime } ( 1 ) -$ $[ G ^ { \prime } ( 1 ) ] ^ { 2 }$ 

Generating functions are extremely useful tools for dealing with sums of independent random variables. Let X and Y be independent random variables with generating functions $G _ { X }$ and $G _ { Y }$ . Then the generating function of their sum is given by 

$$
\begin{array}{c} G _ {X + Y} (z) = \mathbb {E} \left(z ^ {X + Y}\right) \\ = \mathbb {E} \left(z ^ {X} z ^ {Y}\right) \end{array}
$$

$$
\begin{array}{l} = \mathbb {E} (z ^ {X}) \mathbb {E} (z ^ {Y}) \text {(by independence)} \\ = G _ {X} (z) G _ {Y} (z). \end{array}
$$

(Again, “independence means multiply”). 

We can also treat the sum of a random number of random variables. Let $X _ { 1 } , X _ { 2 } , \dots$ . be i.i.d. random variables (taking non-negative integer values), and let N be another random variable, also taking non-negative integer values, independent of the sequence $X _ { i }$ . Define $S = X _ { 1 } + \cdot \cdot \cdot + X _ { N }$ . Then we can write the generating function of S in terms of the common generating function of the $X _ { i }$ and the generating function of N by 

$$
\begin{array}{l} G _ {S} (z) = \mathbb {E} \left(z ^ {S}\right) \\ \qquad = \mathbb {E} \left(z ^ {X _ {1} + \dots + X _ {N}}\right) \\ \qquad = \mathbb {E} \left(\mathbb {E} \left(z ^ {X _ {1} + \dots + X _ {N}} | N\right)\right) \\ \qquad = \mathbb {E} \left(\mathbb {E} \left((z ^ {X _ {1}})\right) ^ {N}\right) \\ \qquad = \mathbb {E} \left((G _ {X} (z)) ^ {N}\right) \\ \qquad = G _ {N} \left(G _ {X} (z)\right). \end{array}
$$

## 3.2 Moment generating functions

The probability generating function is well-adapted for handling random variables which take non-negative integer values. To treat random variables with general distribution, we now introduce two related objects, the moment generating function and the characteristic function. 

The moment generating function of a random variable X is defined by 

$$
M _ {X} (t) := \mathbb {E} \left(e ^ {t X}\right).\tag{3.1}
$$

This expectation may be finite or infinite. 

(Note that we could obtain the moment generating function by substituting $z = e ^ { t }$ in the definition of the probability generating function above. An advantage of this form is that we can conveniently consider an expansion around $t = 0 ,$ , whereas the expansion around $z = 0$ convenient when the random variables took only non-negative integer values, no longer gives a power series in the general case.) 

For the same reason as for probability generating functions, the mgf of a sum of independent random variables is the product of the mgfs: 

## Theorem 3.3.

(a) $I f Y = a X + b $ , then $M _ { Y } ( t ) = e ^ { b t } M _ { X } ( a t )$ 

(b) Let $X _ { 1 } , \ldots , X _ { n }$ be independent random variables, with mgfs $M _ { X _ { 1 } } , \ldots , M _ { X _ { n } }$ . Then the mgf of their sum is given by 

$$
M _ {X _ {1} + \dots + X _ {n}} (t) = M _ {X _ {1}} (t) \dots M _ {X _ {n}} (t).
$$

Proof. (a): easy exercise. Part (b) is also straightforward: 

$$
\begin{array}{l} M _ {X _ {1} + \dots + X _ {n}} (t) = \mathbb {E} \left(e ^ {t X _ {1} + \dots + t X _ {n}}\right) \\ \qquad = \mathbb {E} \left(e ^ {t X _ {1}} \ldots e ^ {t X _ {n}}\right) \\ \qquad = \mathbb {E} \left(e ^ {t X _ {1}}\right) \ldots \mathbb {E} \left(e ^ {t X _ {n}}\right) (\text {by independence}) \\ \qquad = M _ {X _ {1}} (t) \ldots M _ {X _ {n}} (t). \end{array}
$$

An immediate disadvantage of the moment generating function is that it may not be well defined. If the positive tail of the distribution is too heavy, the expectation in the definition in (3.1) may be infinite for all $t > 0 \colon$ while if the negative tail is too heavy, the expectation may be infinite for all $t < 0$ 

For the moment generating function to be useful, we will require $\mathbb { E } e ^ { t _ { 0 } | X | } < \infty$ for some $t _ { 0 } > 0$ . That is, X has “finite exponential moments” of some order (equivalently, the tails of the distribution function decay at least exponentially fast). Then (exercise!) the moment generating function is finite for all $t \in ( - t _ { 0 } , t _ { 0 } )$ , and also all the moments E $X ^ { k }$ are finite. 

Most of the classical distributions that we have looked at are either bounded or have tails that decay at least exponentially (for example uniform, geometric/exponential, normal, Poisson...). However, distributions with heavier tails are also of great importance, especially in many modelling contexts. For those distributions, the moment generating function is of no use; however, we can consider a variant of it, the characteristic function (see later). 

The next result explains the terminology “moment generating function”; the mgf of X can be expanded as a power series around 0, in which the coeficients are the moments of X. 

Theorem 3.4. Suppose $M _ { X } ( t )$ is finite for $| t | \leq t _ { 0 } .$ , for some $t _ { 0 } > 0$ . Then 

(a) $\begin{array} { r } { M _ { X } ( t ) = \sum _ { k = 0 } ^ { \infty } \frac { t ^ { k } \mathbb { E } ( X ^ { k } ) } { k ! } f o r | t | \leq t _ { 0 } . } \end{array}$ 

(b) $M _ { X } ^ { ( k ) } ( 0 ) = \mathbb { E } \left( X ^ { k } \right)$ 

Informal proof. 

$$
\begin{array}{l} M _ {X} (t) = \mathbb {E} \left(e ^ {t X}\right) \\ \qquad = \mathbb {E} \left(1 + t X + \frac {(t X) ^ {2}}{2 !} + \frac {(t X) ^ {3}}{3 !} + \dots\right) \\ \qquad = 1 + t E (X) + \frac {t ^ {2} \mathbb {E} \left(X ^ {2}\right)}{2 !} + \frac {t ^ {3} \mathbb {E} \left(X ^ {3}\right)}{3 !} + \dots , \end{array}
$$

using linearity of expectation. This gives (a) and taking derivatives at 0 gives (b). Exchanging expectation with an infinite sum, as we did here, really needs extra justification. In this case there is no problem (for example, it is always fine in the case where the sum of the absolute values also has finite expectation – in this case this gives E $e ^ { | t X | } < \infty$ which is easily seen to be true); but we do not pursue it further here. □ 

The following uniqueness and continuity results will be key to our applications of the moment generating function. 

Theorem 3.5. If X and Y are random variables with the same moment generating function, which is finite on $[ - t _ { 0 } , t _ { 0 } ]$ for some $t _ { 0 } > 0$ , then X and Y have the same distribution. 

Theorem 3.6. Suppose Y and $X _ { 1 } , X _ { 2 } , . . . ,$ . are random variables whose moment generating functions $M _ { Y }$ and $M _ { X _ { 1 } } , M _ { X _ { 2 } } , \dots$ . are all finite on $[ - t _ { 0 } , t _ { 0 } ]$ for some $t _ { 0 } > 0$ . If 

$$
M _ {X _ {n}} (t) \rightarrow M _ {Y} (t) a s n \rightarrow \infty , f o r a l l t \in [ - t _ {0}, t _ {0} ],
$$

then 

$$
X _ {n} \stackrel {d} {\to} Y a s n \to \infty .
$$

The proofs of the uniqueness and continuity results for mgfs are beyond the scope of the course. They correspond to an inversion theorem from Fourier analysis, by which the distribution function of X can be written in a suitable way as a linear mixture over t of terms E $\boldsymbol { \cdot } e ^ { i t \boldsymbol { X } }$ 

Example 3.7. Find the moment generating function of the exponential distribution with parameter λ. 

Solution: 

$$
\begin{array}{l} M (t) = \mathbb {E} \left(e ^ {t X}\right) \\ \qquad = \int_ {0} ^ {\infty} e ^ {t x} f (x) d x \\ \qquad = \int_ {0} ^ {\infty} \lambda e ^ {t x} e ^ {- \lambda x} d x \\ \qquad = \frac {\lambda}{\lambda - t} \int_ {0} ^ {\infty} (\lambda - t) \exp^ {- (\lambda - t) x} d x \\ \qquad = \frac {\lambda}{\lambda - t} \text {for} t \in (- \infty , \lambda). \end{array}
$$

In the last step we used the fact that the integrand is the density function of a random variable, namely one with $\mathrm { E x p } ( \lambda - t )$ distribution, so that the integral is 1. 

Example 3.8. Find the moment generating function of a random variable with $N ( \mu , \sigma ^ { 2 } )$ distribution. If $Y _ { 1 } \sim N ( \mu _ { 1 } , \sigma _ { 1 } ^ { 2 } )$ and $Y _ { 2 } \sim N ( \mu _ { 2 } , \sigma _ { 2 } ^ { 2 } )$ are independent, show that $Y _ { 1 } + Y _ { 2 } \sim$ $N ( \mu _ { 1 } + \mu _ { 2 } , \sigma _ { 1 } ^ { 2 } + \sigma _ { 2 } ^ { 2 } )$ 

Solution: Let $X \sim N ( \mu , \sigma ^ { 2 } )$ . Then $X = \sigma Z + \mu _ { ; }$ where Z is standard normal. We have 

$$
\begin{array}{r l} & M _ {Z} (t) = \mathbb {E} \left(e ^ {t Z}\right) \\ & \quad = \int_ {- \infty} ^ {\infty} \exp (t z) \frac {1}{\sqrt {2 \pi}} \exp \left(\frac {- z ^ {2}}{2}\right) d z \\ & \quad = \int_ {- \infty} ^ {\infty} \frac {1}{\sqrt {2 \pi}} \exp \left(\frac {- (z ^ {2} - 2 t z)}{2}\right) d z \\ & \quad = \int_ {- \infty} ^ {\infty} \exp \left(\frac {t ^ {2}}{2}\right) \frac {1}{\sqrt {2 \pi}} \exp \left(\frac {- (z - t) ^ {2}}{2}\right) d z \end{array}
$$

(this is “completing the square”) 

$$
= \exp \left(\frac {t ^ {2}}{2}\right) \int_ {- \infty} ^ {\infty} \frac {1}{\sqrt {2 \pi}} \exp \left(\frac {- (z - t) ^ {2}}{2}\right) d z
$$

$$
= e ^ {t ^ {2} / 2}
$$

(the same trick as before: the integrand is the density function of $N ( t , 1 )$ so the integral is 1). 

Then from the first part of Theorem 3.3, $M _ { X } ( t ) = e ^ { \mu t } M _ { Z } ( \sigma t ) = e ^ { \mu t + \sigma ^ { 2 } t ^ { 2 } / 2 }$ 

For the second part, 

$$
\begin{array}{r l} & M _ {Y _ {1} + Y _ {2}} (t) = M _ {Y _ {1}} (t) M _ {Y _ {2}} (t) \\ & \qquad = e ^ {\mu_ {1} t + \sigma_ {1} ^ {2} t ^ {2} / 2} e ^ {\mu_ {2} t + \sigma_ {2} ^ {2} t ^ {2} / 2} \\ & \qquad = e ^ {(\mu_ {1} + \mu_ {2}) t + (\sigma_ {1} ^ {2} + \sigma_ {2} ^ {2}) t ^ {2} / 2}. \end{array}
$$

Since this is the mgf of $N ( \mu _ { 1 } + \mu _ { 2 } , \sigma _ { 1 } ^ { 2 } + \sigma _ { 2 } ^ { 2 } )$ , and it is finite on an interval $[ - t _ { 0 } , t _ { 0 } ]$ (in fact, for all $t )$ , the uniqueness theorem for mgfs tells us that indeed that must be the distribution of $Y _ { 1 } + Y _ { 2 }$ 

## 3.2.1 Proof of WLLN and CLT using moment generating functions

Let $X _ { 1 } , X _ { 2 } , . . .$ . be a sequence of i.i.d. random variables with finite exponential moments of some order (i.e. their moment generating function is finite on some interval containing the origin in its interior). 

Let $S _ { n } = X _ { 1 } + X _ { 2 } + \cdot \cdot \cdot + X _ { n }$ . We can use moment generating functions to give a very compact proof of the Central Limit Theorem for the sequence $S _ { n }$ (and, even more simply, the Weak Law of Large Numbers). 

Let the $X _ { i }$ have mean $\mu$ and variance $\sigma ^ { 2 }$ , and let M be their moment generating function. 

## Weak law of large numbers

From Taylor’s Theorem and the expansion of M as a power series around 0 (Theorem 3.4) we can write, as $h  0$ , 

$$
\begin{array}{c} M (h) = M (0) + h M ^ {\prime} (0) + o (h) \\ = 1 + h \mu + o (h). \end{array}
$$

Here, we use notation $\ ^ { * } f ( h ) = o ( g ( h ) )$ as $h  0 ^ { \dag }$ to mean $f ( h ) / g ( h ) \to 0$ as $h  0$ . We will similarly use notation $\ " a _ { n } = o ( b _ { n } )$ as $n  \infty ^ { \mathfrak { r } }$ to mean $a _ { n } / b _ { n } \to 0$ as $n  \infty$ . Here, specifically, we therefore have $( M ( h ) - M ( 0 ) - h M ^ { \prime } ( 0 ) ) / h \to 0$ as $h  0$ 

Let ${ \overline { { M } } } _ { n }$ be the mgf of $S _ { n } / n$ . Using the independence of the $X _ { i }$ , we have 

$$
\begin{array}{l} \overline {{M}} _ {n} (t) = \mathbb {E} \left(e ^ {t S _ {n} / n}\right) \\ \qquad = \mathbb {E} \left(e ^ {t X _ {1} / n} \dots e ^ {t X _ {n} / n}\right) \\ \qquad = (M (t / n)) ^ {n} \\ \qquad = \left(1 + \frac {t}{n} \mu + o (t / n)\right) ^ {n} \text {as} n \to \infty \\ \qquad \to e ^ {t \mu} \text {as} n \to \infty . \end{array}
$$

But $e ^ { t \mu }$ is the mgf of a random variable which takes the constant value $\mu$ with probability 1. From the continuity theorem for mgfs, $S _ { n } / n \stackrel { d } { \to } \mu$ as $n \to \infty$ , and we have proved the weak law of large numbers. 

## Central limit theorem

Let $Y _ { i } = X _ { i } - \mu _ { \operatorname { \mathbf { \partial } } }$ , and let $M _ { Y }$ be the mgf of the common distribution of the $Y _ { i } .$ . Taking one more term in the Taylor expansion, we have that as $h  0$ , 

$$
\begin{array}{r l} & M _ {Y} (h) = M _ {Y} (0) + h M _ {Y} ^ {\prime} (0) + \frac {h ^ {2}}{2} M _ {Y} ^ {\prime \prime} (0) + o (h ^ {2}) \\ & \qquad = 1 + h \mathbb {E} (Y) + \frac {h ^ {2}}{2} \operatorname{Var} (Y) + o (h ^ {2}) \\ & \qquad = 1 + h ^ {2} \sigma^ {2} / 2 + o (h ^ {2}). \end{array}
$$

Let $\widetilde { M } _ { n }$ be the mgf of $\frac { S _ { n } - \mu n } { \sigma { \sqrt { n } } }$ . Then we have 

$$
\begin{array}{l} \widetilde {M} _ {n} (t) = \mathbb {E} \left(\exp \left(\frac {t (S _ {n} - \mu n)}{\sigma \sqrt {n}}\right)\right) \\ \qquad = \mathbb {E} \left(\exp \left(\frac {t (X _ {1} - \mu)}{\sigma \sqrt {n}}\right) \ldots \exp \left(\frac {t (X _ {n} - \mu)}{\sigma \sqrt {n}}\right)\right) \\ \qquad = M _ {Y} \left(\frac {t}{\sigma \sqrt {n}}\right) ^ {n} \\ \qquad = \left(1 + \frac {t ^ {2}}{2 n} + o \left(\frac {t ^ {2}}{n}\right)\right) ^ {n} \text {as} n \to \infty \\ \qquad \to \exp \left(\frac {t ^ {2}}{2}\right) \text {as} n \to \infty . \end{array}
$$

But the last line is the mgf of $N ( 0 , 1 )$ . Using the continuity theorem again, 

$$
\frac {S _ {n} - \mu n}{\sigma \sqrt {n}} \xrightarrow {d} N (0, 1),
$$

and we have proved the CLT. 

## 3.3 Using moment generating functions for tail bounds

Using a version of Markov’s inequality applied to a random variable like $e ^ { t X }$ , we can get bounds on the tail of a distribution in terms of the moment generating function which are much better than we would get from, for example, Chebyshev’s inequality, which is the application of Markov’s inequality to the random variable $( X - \mu ) ^ { 2 }$ . (Of course, this can only work if the moment generating function exists!) 

For example, we can apply this to simple random walk. Let $X _ { i }$ be i.i.d. taking values −1 and 1 with probability $1 / 2$ each. Let $S _ { n } = X _ { 1 } + \cdots + X _ { n } $ , so that $S _ { n }$ is the position of simple random walk on $\mathbb { Z }$ after n steps. 

We know from the central limit theorem that, for large $n , S _ { n }$ is typically on the order of $\sqrt { n }$ . So an event like $\left\{ \left| S _ { n } \right| > n a \right\}$ , for some $a > 0$ , ought to have probability which gets small as $n \to \infty$ 

First we bound the probability using Chebyshev. We have E $S _ { n } = 0$ and Var $S _ { n } = n$ . So 

$$
\mathbb {P} (| S _ {n} | > n a) \leq \frac {\operatorname{Var} S _ {n}}{(n a) ^ {2}}
$$

$$
= \frac {1}{n a ^ {2}}.
$$

This goes to 0 as desired but not very quickly! 

Let us try instead using the moment generating function. We have 

$$
\begin{array}{l} \mathbb {E} e ^ {t X _ {i}} = \frac {e ^ {t} + e ^ {- t}}{2} \\ \qquad = \cosh t \\ \qquad \leq \exp \left(\frac {t ^ {2}}{2}\right) \text {   for   all   } t. \end{array}
$$

(The inequality cosh $t \le \exp ( t ^ { 2 } / 2 )$ can be checked directly by expanding the exponential functions and comparing coeficients in the power series). 

For $t > 0 ,$ , we can now write 

$$
\begin{array}{r l} & {\mathbb {P} (S _ {n} > n a) = \mathbb {P} \left(\exp (t S _ {n}) > \exp (t n a)\right)} \\ & {\qquad \leq \frac {\mathbb {E} \exp (t S _ {n})}{\exp (t n a)} (\text {this is from Markov's inequality})} \\ & {\qquad = \left(\frac {\mathbb {E} \exp (t X _ {i})}{\exp (t a)}\right) ^ {n}} \\ & {\qquad \leq \left(\exp \left(t ^ {2} / 2 - t a\right)\right) ^ {n}.} \end{array}
$$

Note that this is true for any positive t, so we are free to choose whichever one we like. Naturally, we want to minimise the RHS. It is easy to check (just diferentiate) that this is done by choosing $t = a ,$ which gives 

$$
\mathbb {P} (S _ {n} > n a) \leq \exp \left(- n a ^ {2} / 2\right).
$$

By symmetry the bound on $\mathbb { P } ( S _ { n } < - n a )$ is exactly the same. Combining the two we get 

$$
\mathbb {P} (| S _ {n} | > n a) \leq 2 \exp \left(- n a ^ {2} / 2\right).
$$

This decays much quicker than the bound from Chebyshev above! 

## 3.4 Characteristic functions

The characteristic function is defined by replacing t by it in the definition of the moment generating function. The characteristic function of X is given by 

$$
\phi_ {X} (t) := \mathbb {E} \left(e ^ {i t X}\right),
$$

for $t \in \mathbb { R }$ . We can write 

$$
\phi_ {X} (t) = \mathbb {E} (\cos (t X)) + i \mathbb {E} (\sin (t X)).
$$

As a result we can see that the characteristic function is finite for every t, whatever the distribution of X. In fact, $| \phi _ { X } ( t ) | \leq 1$ for all t. 

This means that many of the results for the moment generating function which depended on exponential tails of the distribution have analogues for the characteristic function which hold for any distribution. Just as before we have $\phi _ { X + Y } ( t ) = \phi _ { X } ( t ) \phi _ { Y } ( t )$ . The uniqueness and continuity theorems given for mgfs hold in a similar way for characteristic functions. The Taylor expansion of the characteristic function around the origin involves the moments of the distribution in a similar way (except now with an added factor of $i ^ { k }$ for the kth term): 

$$
\phi_ {X} (t) = 1 + i t \mathbb {E} X + i ^ {2} t ^ {2} \frac {\mathbb {E} X ^ {2}}{2} + \dots + i ^ {k} t ^ {k} \frac {\mathbb {E} X ^ {k}}{k !} + o (t ^ {k})\tag{3.2}
$$

as $t \to 0$ , whenever E $X ^ { k }$ is finite. Hence by following exactly the same strategy, we could give a proof of the central limit theorem using characteristic functions instead of mgfs. This would now prove the CLT without any additional assumption on the distribution (only finiteness of the variance is needed). Apart from working with complex power series instead of real power series, there are no additional complications when translating the proof from mgfs to cfs. 

When the mgf is finite in an interval containing the origin in its interior, the theory of analytic continuation of complex functions allows us to obtain the characteristic function easily, by replacing t with it in the mgf. 

Example 3.9. (a) The mgf of $N ( 0 , 1 )$ is $\exp ( t ^ { 2 } / 2 )$ , and the cf is ex $\mathsf { p } ( ( i t ) ^ { 2 } / 2 ) = \mathsf { e x p } ( - t ^ { 2 } / 2 )$ 

(b) The mgf of Exp(1) is $1 / ( 1 - t )$ , and the cf is $ 1 / ( 1 - i t )$ 

(c) Suppose X has Cauchy distribution with density $\textstyle f ( x ) = { \frac { 1 } { \pi ( 1 + x ^ { 2 } ) } }$ . The moment generating function is infinite for all $t \neq 0$ (in fact, even the mean does not exist as $\mathbb { E } \left| X \right| = \infty$ exercise). The characteristic function is given by 

$$
\phi_ {X} (t) = \mathbb {E} e ^ {i t X} = \int_ {- \infty} ^ {\infty} \frac {e ^ {i t x}}{\pi (1 + x ^ {2})} d x
$$

and this can be evaluated by contour integration to give $e ^ { - | t | }$ 

Note that $\phi _ { X }$ is not diferentiable at $0 ;$ from (3.2), this corresponds to the fact that the mean does not exist. 

In fact, consider $X _ { 1 } , X _ { 2 } , \ldots X _ { n }$ i.i.d. Cauchy, and $S _ { n } = X _ { 1 } + \cdots + X _ { n }$ . Then 

$$
\phi_ {S _ {n} / n} (t) = \phi \left(\frac {t}{n}\right) ^ {n} = \left(e ^ {- | t | / n}\right) ^ {n} = e ^ {- | t |} = \phi_ {X} (t).
$$

So $S _ { n } / n$ and $X _ { i }$ have the same distribution! The law of large numbers and the CLT do not apply (since the mean does not exist). 

## 3.4.1 Comparing moment generating functions and characteristic functions

Question $\mathrm { M } 4 ( \mathrm { a } ) ( \mathrm { i i } )$ on Part A paper AO2 from 2011 asks: 

State one purpose for which you should use the characteristic function rather than the moment generating function, and one purpose for which you would want to use the moment generating function rather than the characteristic function. 

The previous section gives an obvious answer to the first part of the question: when the distribution does not have exponentially decaying tails, the moment generating function is not useful but the characteristic function certainly is (to prove the CLT, for example). In the other direction, one could refer to the use of the mgf to give bounds on the tail of a distribution. In Section 3.3 we did this using Markov’s inequality applied to the random variable $e ^ { t X }$ ; replacing this with $ e ^ { i t X }$ would give nothing sensible, since that function is not real-valued, let alone monotonic. 

## Joint distribution of continuous random variables

## 4.1 Review of jointly continuous random variables

The joint cumulative distribution function of two random variables X and Y is defined by 

$$
F _ {X, Y} (x, y) = \mathbb {P} (X \leq x, Y \leq y).
$$

$X$ and $Y$ are said to be jointly continuous if their joint cdf can be written as an integral: 

$$
F _ {X, Y} (x, y) = \int_ {u = - \infty} ^ {x} \int_ {v = - \infty} ^ {y} f (u, v) d u d v.
$$

Then $f$ is said to be the joint pdf of $X$ and $Y _ { z }$ , often written as $f _ { X , Y }$ . As in the case of a single random variable, we might more properly say $^ { 6 6 } \mathrm { a }$ joint $\mathrm { p d f } ^ { \mathrm { , } }$ rather than “the joint $\mathrm { p d f } ^ { \mathrm { p } }$ because we can, for example, change the value of $f$ at finitely many points without changing the value of any integrals of $f .$ But it is natural to put 

$$
f _ {X, Y} (x, y) = \frac {\partial^ {2}}{\partial x \partial y} F _ {X, Y} (x, y)
$$

whenever $F _ { X , Y }$ is diferentiable at $( x , y )$ 

For general (suitably nice<sup>1</sup>) sets $A \subset \mathbb { R } ^ { 2 }$ we have 

$$
\mathbb {P} \left((X, Y) \in A\right) = \int \int_ {A} f _ {X, Y} (x, y) d x d y.\tag{4.1}
$$

If $f _ { X , Y }$ satisfies (4.1) for all (nice) $A \subset \mathbb { R } ^ { 2 }$ , then, clearly, $f _ { X , Y }$ is a joint pdf of $( X , Y )$ . It sufices to check (4.1) for rectangles A or just for sets of the form $A = ( - \infty , u ] \times ( - \infty , v ]$ which yield the joint cdf. 

We can recover the distribution of one of the random variables X or of Y by integrating over the other one. (In this context the distribution of one of the variables is called the marginal distribution). 

$$
f _ {X} (x) = \int_ {y = - \infty} ^ {\infty} f _ {X, Y} (x, y) d y
$$

$$
f _ {Y} (y) = \int_ {x = - \infty} ^ {\infty} f _ {X, Y} (x, y) d x
$$

A function of X and Y is itself a random variable. Its expectation is given by 

$$
\mathbb {E} h (X, Y) = \int_ {x = - \infty} ^ {\infty} \int_ {y = - \infty} ^ {\infty} h (x, y) f _ {X, Y} (x, y) d x d y.
$$

Recall that X and $Y$ are independent if $F _ { X , Y } ( x , y ) = F _ { X } ( x ) F _ { Y } ( y )$ for all $x , y .$ Equivalently, the joint density can be written as a product: 

$$
f _ {X, Y} (x, y) = f _ {X} (x) f _ {Y} (y).
$$

All the above can be naturally generalised to describe the joint distribution of more than two random variables. 

## 4.2 Change of variables

Often there is more than one natural coordinate system in which to view a model. We have the following change of variables result: 

Theorem 4.1. Suppose $T : ( x , y ) \mapsto ( u , v )$ is a one-to-one mapping from some domain $D \subseteq \mathbb { R } ^ { 2 }$ to some range $R \subseteq \mathbb { R } ^ { 2 }$ 

Define the Jacobian J as a function of $( u , v )$ by 

$$
J = \det \left( \begin{array}{c c} \frac {\partial x}{\partial u} & \frac {\partial x}{\partial v} \\ \frac {\partial y}{\partial u} & \frac {\partial y}{\partial v} \end{array} \right) = \frac {\partial x}{\partial u} \frac {\partial y}{\partial v} - \frac {\partial x}{\partial v} \frac {\partial y}{\partial u}.
$$

Assume that the partial derivatives involved exists and are continuous. 

IfX, Y have joint probability density function $f _ { X , Y }$ , then the random variables $U , V$ defined by $( U , V ) = T ( X , Y )$ are jointly continuous with joint probability density function $f _ { U , V }$ given by 

$$
f _ {U, V} (u, v) = \left\{ \begin{array}{l l} f _ {X, Y} \big (x (u, v), y (u, v) \big) | J (u, v) | & \text { if } (u, v) \in R \\ 0 & \text { otherwise } \end{array} \right..
$$

Proof. The proof is simple using the familiar formula for change of variables in an integral. Suppose that $A \subseteq D$ and $T ( A ) = B$ . Then, since $T$ is one-to-one, 

$$
\begin{array}{l} \mathbb {P} \left((U, V) \in B\right) = \mathbb {P} \left((X, Y) \in A\right) \\ \qquad = \int \int_ {A} f _ {X, Y} (x, y) d x   d y \\ \qquad = \int \int_ {B} f _ {X, Y} \left(x (u, v), y (u, v)\right) | J (u, v) | d u   d v. \end{array}
$$

Hence the final integrand is the joint pdf of $( U , V )$ 

The formula for change of variables in the integral appeared in various contexts last year. Recall the general idea: after a suitable translation, the transformation T looks locally like a linear transformation whose matrix is the matrix of partial derivatives above. We know that the factor by which the area of a set changes under a linear transformation is given by the determinant of the matrix of the transformation. So, locally, the Jacobian $J ( u , v )$ gives the ratio between the area of a rectangle $( x , x + d x ) \times ( y , y + d y )$ and its image under T (which is a parallelogram). Since we want the probability to stay the same, and probability is area times density, we should rescale the density by the same amount $J ( u , v )$ 

Example 4.2. Let X, Y be i.i.d. exponentials with rate λ. Let $U = X / ( X + Y ) , V = X + Y$ What is the joint distribution of $( U , V ) ?$ 

Solution: 

$$
\begin{array}{r} f _ {X, Y} (x, y) = \lambda e ^ {- \lambda x} \lambda e ^ {- \lambda y} \\ = \lambda^ {2} e ^ {- \lambda (x + y)} \end{array}
$$

for $( x , y ) \in ( 0 , \infty ) ^ { 2 }$ . The transformation $( u , v ) = ( x / ( x + y ) , x + y )$ takes $( 0 , \infty ) ^ { 2 }$ to $( 0 , 1 ) \times$ $( 0 , \infty )$ . It is inverted by $x = u v , y = v ( 1 - u )$ . The Jacobian is given by 

$$
\begin{array}{r l} J (u, v) = \det \left( \begin{array}{c c} \frac {\partial x}{\partial u} & \frac {\partial x}{\partial v} \\ \frac {\partial y}{\partial u} & \frac {\partial y}{\partial v} \end{array} \right) & = \det \left( \begin{array}{c c} v & u \\ - v & 1 - u \end{array} \right) \\ & = v (1 - u) + u v \\ & = v. \end{array}
$$

So we have 

$$
\begin{array}{c} f _ {U, V} (u, v) = f _ {X, Y} \bigl (x (u, v), y (u, v) \bigr) | J (u, v) | \\ = \lambda^ {2} e ^ {- \lambda \bigl (x (u, v) + y (u, v) \bigr)} | J (u, v) | \\ = v \lambda^ {2} e ^ {- \lambda v} \end{array}
$$

for $( u , v ) \in ( 0 , 1 ) \times ( 0 , \infty )$ 

This factorises into a product of a function of u and a function of v (the function of u is trivial). So U and V are independent, with 

$$
\begin{array}{l} f _ {U} (u) = 1, u \in (0, 1) \\ f _ {V} (v) = \lambda^ {2} v e ^ {- \lambda v}, v \in (0, \infty) \end{array}
$$

So $U \sim U [ 0 , 1 ]$ and $V \sim \mathrm { G a m m a } ( 2 , \lambda )$ , independently. 

Example 4.3. Let X and Y be independent Exp(λ) as in the previous example, and now let $V = X + Y , W = X - Y$ . This transformation takes $( 0 , \infty ) ^ { 2 }$ to the set $\{ ( v , w ) : | w | < v \}$ The inverse transformation is 

$$
x = \frac {v + w}{2}, y = \frac {v - w}{2}
$$

with Jacobian 

$$
J (v, w) = \det \left( \begin{array}{c c} \frac {1}{2} & \frac {1}{2} \\ \frac {1}{2} & - \frac {1}{2} \end{array} \right) = - \frac {1}{2}.
$$

(Notice that any linear transformation always has constant Jacobian). So we have 

$$
\begin{array}{c} f _ {V, W} (v, w) = \left\{ \begin{array}{l l} f _ {X, Y} \left(\frac {v + w}{2}, \frac {v - w}{2}\right) | J (v, w) | & \text { for } | w | <   v \\ 0 & \text { otherwise } \end{array} \right. \\ = \left\{ \begin{array}{l l} \frac {1}{2} \lambda^ {2} e ^ {- \lambda v} & \text { for } | w | <   v \\ 0 & \text { otherwise }. \end{array} \right. \end{array}
$$

It looks like the pdf factorises into a product as in the previous example. But here this is not really the case! – because of the restriction to $| w | < v .$ . In fact, V and W could not be independent here, otherwise we could not have $\mathbb { P } ( | W | < V ) = 1$ 

From the previous example we already know that V ∼ Gamma $, ( 2 , \lambda )$ . What is the marginal distribution of $W ?$ 

$$
\begin{array}{r l} & f _ {W} (w) = \int_ {v = | w |} ^ {\infty} \frac {1}{2} \lambda^ {2} e ^ {- \lambda v} d v \\ & \qquad = \left[ - \frac {1}{2} \lambda e ^ {- \lambda v} \right] _ {| w |} ^ {\infty} \\ & \qquad = \frac {1}{2} \lambda e ^ {- \lambda | w |}. \end{array}
$$

We see that the distribution of W is symmetric around 0, and by adding the density at w and $- w ,$ the distribution of |W| has pdf $\lambda e ^ { - \lambda | w | }$ and so again has $\mathrm { E x p } ( \lambda )$ distribution. 

Example 4.4 (General formula for the sum of continuous random variables). If X and Y are jointly continuous with density function $f _ { X , Y }$ , what is the distribution of $X + Y ?$ We can change variables to $U = X + Y , V = X$ . This transformation has Jacobian 1 (check!), and we obtain $f _ { U , V } ( u , v ) = f _ { X , Y } ( v , u - v )$ 

To obtain the marginal distribution of $X + Y$ , which is $U _ { : }$ , we integrate over v: 

$$
f _ {X + Y} (u) = \int_ {- \infty} ^ {\infty} f _ {X, Y} (v, u - v) d v.
$$

An important case is when X and $Y$ are independent. Then we obtain the convolution formula: r∞ 

$$
f _ {X + Y} (u) = \int_ {- \infty} ^ {\infty} f _ {X} (v) f _ {Y} (u - v) d v.
$$

## 4.2.1 Multivariate distributions

Everything above can be generalised to the case of the joint distribution of $n > 2$ random variables. The Jacobian is now the determinant of an $n \times n$ matrix. 

## 4.3 Multivariate normal distribution

Let $Z _ { 1 } , Z _ { 2 } , \ldots , Z _ { n }$ be i.i.d. standard normal random variables. Their joint density function can be written as 

$$
\begin{array}{c} f _ {\mathbf {Z}} (\mathbf {z}) = \prod_ {i = 1} ^ {n} \frac {1}{\sqrt {2 \pi}} \exp \left(- \frac {z _ {i} ^ {2}}{2}\right) \\ = \frac {1}{(2 \pi) ^ {n / 2}} \exp \left(- \frac {1}{2} \mathbf {z} ^ {T} \mathbf {z}\right). \end{array}
$$

Define $W _ { 1 } , \dots , W _ { n }$ by 

$$
\left( \begin{array}{c} W _ {1} \\ W _ {2} \\ \vdots \\ W _ {n} \end{array} \right) = A \left( \begin{array}{c} Z _ {1} \\ Z _ {2} \\ \vdots \\ Z _ {n} \end{array} \right) + \left( \begin{array}{c} \mu_ {1} \\ \mu_ {2} \\ \vdots \\ \mu_ {n} \end{array} \right)
$$

where $A$ is some $n \times n$ matrix. 

Assume A is invertible. Then by change of variables (the Jacobian is constant) we get 

$$
f _ {\mathbf {W}} (\mathbf {w}) = \frac {1}{(2 \pi) ^ {n / 2} | \det A |} \exp \left(- \frac {1}{2} (\mathbf {w} - \boldsymbol {\mu}) ^ {T} (A A ^ {T}) ^ {- 1} (\mathbf {w} - \boldsymbol {\mu})\right).
$$

The matrix $\Sigma : = A A ^ { T }$ is the covariance matrix in the sense that Cov $( W _ { i } , W _ { j } ) = ( A A ^ { T } ) _ { i j }$ (check, e.g. for $n = 2$ if you want an easy case). $W _ { 1 } , \ldots , W _ { n }$ are said to have the multivariate normal distribution with mean vector $\pmb { \mu }$ and covariance matrix $\Sigma .$ 

For the case $n = 2$ , one can manipulate to obtain (with $X = W _ { 1 } , Y = W _ { 2 } )$ 

$$
\begin{array}{l} f _ {X, Y} (x, y) \\ = \frac {1}{2 \pi \sigma_ {X} \sigma_ {Y} \sqrt {1 - \rho^ {2}}} \exp \left(- \frac {1}{2 (1 - \rho^ {2})} \left[ \frac {(x - \mu_ {X}) ^ {2}}{\sigma_ {X} ^ {2}} - \frac {2 \rho (x - \mu_ {X}) (y - \mu_ {Y})}{\sigma_ {X} \sigma_ {Y}} + \frac {(y - \mu_ {Y}) ^ {2}}{\sigma_ {Y} ^ {2}} \right]\right) \end{array}
$$

where $\sigma _ { X } ^ { 2 }$ and $\sigma _ { Y } ^ { 2 }$ are the variances of X and $Y , \mu _ { X }$ and $\mu _ { Y }$ are the means, and $\rho$ is the correlation coeficient between $X$ and Y which is defined by 

$$
\rho = \frac {\operatorname{Cov} (X , Y)}{\sigma_ {X} \sigma_ {Y}}
$$

and lies in $( - 1 , 1 )$ . 

Note that 

(1) The density depends only on $\mu _ { X } , \mu _ { Y } , \sigma _ { X } , \sigma _ { Y }$ and $\rho .$ 

(2) X and Y are independent ⇔ $\rho = 0 . \ ( \Rightarrow$ is true for any joint distribution; ⇐ is a special property of joint normal.) 

A special case is the standard bivariate normal where $\sigma _ { X } = \sigma _ { Y } = 1$ and $\mu _ { X } = \mu _ { Y } = 0$ Then 

$$
f _ {X, Y} (x, y) = \frac {1}{2 \pi \sqrt {1 - \rho^ {2}}} \exp \left(- \frac {x ^ {2} - 2 \rho x y + y ^ {2}}{2 (1 - \rho^ {2})}\right).
$$

In this case $\Sigma = { \binom { 1 } { \rho } } \ \rho )$ 

## 4.4 Conditional densities

The basic definition of conditional probability: for two events A and B with $\mathbb { P } ( A ) > 0$ , the conditional probability of B given A is 

$$
\mathbb {P} (B | A) := \frac {\mathbb {P} (A \cap B)}{\mathbb {P} (A)}.\tag{4.2}
$$

Applying this to the distribution of a random variable, we have for example 

$$
\mathbb {P} (X \leq x | A) = \frac {\mathbb {P} (\{X \leq x \} \cap A)}{\mathbb {P} (A)}.
$$

The left-hand side is a cumulative distribution function. It gives the conditional distribution of X, given A. We might denote it by $F _ { X \mid A } ( x )$ 

In the case where X is discrete, we can write the conditional probability mass function: 

$$
p _ {X | A} (x) = \mathbb {P} (X = x | A).
$$

If X is continuous, we can diferentiate the conditional distribution function to get a conditional density function $f _ { X \mid A } ( x )$ , and then for a set $C ,$ 

$$
\mathbb {P} (X \in C | A) = \int_ {x \in C} f _ {X | A} (x) d x.
$$

The conditional expectation of X given A is the expectation of the conditional distribution, which is given by 

$$
\mathbb {E} (X | A) = \sum_ {x} x p _ {X | A} (x)
$$

in the discrete case, and by 

$$
\mathbb {E} (X | A) = \int x f _ {X | A} (x) d x
$$

in the continuous case. 

Example 4.5. Suppose X and Y are independent random variables which both have uniform distribution on $[ 0 , 1 ]$ . Find the conditional distribution and conditional expectation of Y given $X + Y > 1$ 

Solution: 

$$
\mathbb {P} (Y <   y | X + Y > 1) = \frac {\mathbb {P} (Y <   y , X + Y > 1)}{\mathbb {P} (X + Y > 1)}.
$$

Since $X , Y$ are uniform on the square $[ 0 , 1 ] ^ { 2 }$ , the probability of a set is equal to its area. 

The set $\{ x + y > 1 \}$ has area $1 / 2$ , while for fixed y, the set $\{ ( x , v ) : v < y , x + v > 1 \}$ has area $y ^ { 2 } / 2$ 

So the distribution function of Y given $X + Y > 1$ is $F ( y ) = ( y ^ { 2 } / 2 ) / ( 1 / 2 ) = y ^ { 2 }$ , and the conditional density is 2y on $[ 0 , 1 ]$ , and 0 elsewhere. 

The conditional expectation E $( Y | X + Y > 1 )$ is $\begin{array} { r } { \int _ { 0 } ^ { 1 } y \times 2 y d y = 2 / 3 . } \end{array}$ 

A common way in which conditional distributions arise is when we have two random variables X and Y with some joint distribution; we observe the value of X and want to know what this tells us about the value of Y. That is, what is the conditional distribution of $Y$ given $X = x ?$ 

When X is a discrete random variable, everything works fine; since $\mathbb { P } ( X = x )$ will be positive, we can use the approach above. 

However, if X is continuous, then $\mathbb { P } ( X = x )$ will be 0 for every x. Now we have a problem, since if the event A in (4.2) has probability 0, then the definition makes no sense. 

To resolve this problem, rather than conditioning directly on $\{ X = x \}$ , we look at the distribution of Y conditioned on $\{ x \leq X \leq x + \epsilon \}$ . If the joint distribution is well-behaved (as it will be in all the cases that we wish to consider), we can obtain a limit as $\epsilon \downarrow 0 .$ which we define as the distribution of Y given $X = x$ 

As $\epsilon  0 .$ we have 

$$
\begin{array}{l} \mathbb {P} \big (Y \leq y | x \leq X \leq x + \epsilon \big) = \frac {\int_ {v = - \infty} ^ {y} \int_ {u = x} ^ {x + \epsilon} f _ {X , Y} (u , v) d u   d v}{\int_ {u = x} ^ {x + \epsilon} f _ {X} (u) d u} \\ \sim \frac {\epsilon \int_ {v = - \infty} ^ {y} f _ {X , Y} (x , v) d v}{\epsilon f _ {X} (x)} \\ = \int_ {v = - \infty} ^ {y} \frac {f _ {X , Y} (x , v)}{f _ {X} (x)} d v. \end{array}\tag{4.3}
$$

So we define $F _ { Y \mid X = x } ( y )$ , the conditional distribution function of $Y$ given $X = x ,$ as the right-hand side of (4.3). 

Diferentiating with respect to y, we obtain the conditional density function of $Y$ given $X = x$ , written as $f _ { Y \mid X = x } ( y )$ : 

$$
\boxed {f _ {Y | X = x} (y) = \frac {f _ {X , Y} (x , y)}{f _ {X} (x)}.}
$$

These definitions make sense whenever $f _ { X } ( x ) > 0$ . In that case, note that $f _ { Y \mid X = x }$ is indeed a density function, because we have defined $\begin{array} { r } { f _ { X } ( x ) = \int _ { - \infty } ^ { \infty } f _ { X , Y } ( x , y ) d y } \end{array}$ . (Notice that the denominator $f _ { X } ( x )$ does not involve y at all; it is just a normalising constant). 

The idea is that the following two procedures are equivalent: 

(1) generate (X, Y ) according to the joint density function $f _ { X , Y } ;$ 

(2) first generate X according to the density function $f _ { X }$ , and then having observed $X = x$ generate Y according to the density function $f _ { Y \mid X = x }$ 

Example 4.6 (Simple example). Let $( X , Y )$ be uniform on the triangle $\{ 0 < y < x < 1 \}$ Then 

$$
f _ {X, Y} (x, y) = \left\{ \begin{array}{l l} 2 & 0 <   y <   x <   1 \\ 0 & \text { otherwise } \end{array} \right..
$$

For the conditional density of Y given $X = x ,$ 7 

$$
\begin{array}{l} f _ {Y | X = x} (y) = \frac {f _ {X , Y} (x , y)}{f _ {X} (x)} \\ = \left\{ \begin{array}{l l} 2 / f _ {X} (x) & 0 <   y <   x \\ 0 & \text {otherwise} \end{array} \right., \end{array}
$$

provided $x \in ( 0 , 1 )$ . We do not need to calculate $f _ { X } ( x )$ , since it is just a normalising constant. Since the conditional density function of Y is constant in y, we see that $Y$ is uniform on $[ 0 , x ]$ ， with distribution function given by 

$$
F _ {Y | X = x} (y) = \left\{ \begin{array}{l l} 0 & y <   0 \\ \frac {y}{x} & 0 \leq y \leq x \\ 1 & y > x \end{array} \right..
$$

The conditional mean of $Y$ given $X = x$ is $x / 2$ 

Example 4.7 (Bivariate normal). Let X and Y be jointly normal with means $\mu _ { 1 }$ and $\mu _ { 2 }$ respectively, variances $\sigma _ { 1 } ^ { 2 }$ and $\sigma _ { 2 } ^ { 2 }$ respectively, and correlation coeficient $\rho .$ What is the conditional distribution of $Y$ given $X = x ?$ 

Rather than working directly from the joint density function, we can proceed by writing $Y$ as the sum of two terms, one which is a function of X and one which is independent of X. 

First let us write X and Y as functions of independent standard normals $Z _ { 1 }$ and $Z _ { 2 }$ . If we put 

$$
\begin{array}{l} {X = \sigma_ {1} Z _ {1} + \mu_ {1}} \\ {Y = \rho \sigma_ {2} Z _ {1} + \sqrt {1 - \rho^ {2}} \sigma_ {2} Z _ {2} + \mu_ {2}} \end{array}
$$

then indeed X and Y have the desired means, variances and covariance (check!). 

Then we can write 

$$
Y = \rho \frac {\sigma_ {2}}{\sigma_ {1}} (X - \mu_ {1}) + \sqrt {1 - \rho^ {2}} \sigma_ {2} Z _ {2} + \mu_ {2}.
$$

The first term is a function of X and the second term, involving only $Z _ { 2 }$ , is independent of $X .$ 

So conditional on $X = x .$ , the distribution of Y is the distribution of 

$$
\rho \frac {\sigma_ {2}}{\sigma_ {1}} (x - \mu_ {1}) + \sqrt {1 - \rho^ {2}} \sigma_ {2} Z _ {2} + \mu_ {2},
$$

which is normal with mean $\rho _ { \sigma _ { 1 } } ^ { \sigma _ { 2 } } ( x - \mu _ { 1 } ) + \mu _ { 2 }$ and variance $( 1 - \rho ^ { 2 } ) \sigma _ { 2 } ^ { 2 }$ 

Note the way the variance of this conditional distribution depends on $\rho .$ We say that $\rho ^ { 2 }$ is the “amount of the variance of Y explained by $X ^ { \dag }$ . Consider the extreme cases. If $\rho = \pm 1$ then the conditional variance is 0. That is, Y is a function of X and once we observe X, there is no longer any uncertainty about the value of Y. If $\rho = 0$ , the conditional variance and the unconditional variance are the same; observing X tells us nothing about Y . 

## 4.5 Cautionary tale

The definition above of conditional distribution given the value of a continuous random variable makes sense in context, but keep in mind that conditioning directly on events on probability zero is not valid, and as a result the objects involved are not robust to seemingly innocent manipulation! Consider the following example: 

Example 4.8 (Borel’s paradox). Consider the uniform distribution on the half-disc $C =$ $\{ ( x , y ) : y \ge 0 , x ^ { 2 } + y ^ { 2 } \le 1 \}$ . The joint density of X and Y is given by 

$$
f (x, y) = \left\{ \begin{array}{l l} \frac {2}{\pi} & (x, y) \in C \\ 0 & \text { otherwise } \end{array} \right..
$$

What is the conditional distribution of Y given $X = 0 ?$ Its density is given by 

$$
f _ {Y | X = 0} (y) = \frac {2 / \pi}{f _ {X} (0)}
$$

for $y \in [ 0 , 1 ]$ , and 0 elsewhere. So the distribution is uniform on [0, 1] (we do not need to calculate $f _ { X } ( 0 )$ to see this, since it is only a normalising constant). 

We could change variables and represent the same distribution in polar coordinates. Then R and Θ are independent; R has density 2r on [0,1] and Θ is uniform on $[ 0 , \pi )$ . (See first question on problem sheet 2 for the transformation to polar coordinates. But in this case where the density of X, Y is uniform on a set, one can also easily derive the joint distribution of R and Θ directly by considering areas of subsets of the set C). 

Note that the events $\{ X = 0 \}$ and $\{ \Theta = \pi / 2 \}$ are the same. 

What is the conditional distribution of R given $\Theta = \pi / 2 ?$ Since R and Θ are independent, it still has density 2r on [0, 1]. This is not uniform on [0, 1]. 

But when $X = 0 .$ , i.e. when $\Theta = \pi / 2$ , R and Y are the same thing. So the distribution of R given $\Theta = \pi / 2$ ought to be the same as the distribution of Y given $X = 0 ,$ , should it not? 

What is happening is that, although the events $\{ X = 0 \}$ and $\{ \Theta = \pi / 2 \}$ are the same, it is not the case that the events $\{ | X | < \epsilon \}$ and $\lbrace \vert \Theta - \pi / 2 \vert < \epsilon \rbrace$ are the same. When we condition X to be within  of 0, we restrict to a set which is approximately a rectangle (the left-hand picture below). However, when we condition Θ to be near $\pi / 2 ,$ we restrict to a thin sector of the circle, which is approximately a triangle (the right-hand picture below). In the second case, we bias the point chosen to lie higher up. As $\epsilon  0 .$ , this bias persists; the two limits are not the same! 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d41801ab-b3a3-458a-8898-d5ac7fce9cb4/2e54fcef0267a62b109e329da13f16c5a09ee645f2e3545c461ba01f0eafc267.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d41801ab-b3a3-458a-8898-d5ac7fce9cb4/e8cd083341edba848f61340d49994b246dc9a3f9b17eba0e77caffd217acf4bc.jpg)


What this “paradox” illustrates is that conditioning for continuous random variables involves a limit, and that it can be important exactly how the limit is taken. The procedure whereby we generate X from $f _ { X }$ and then Y from $f _ { Y \mid X }$ makes sense in terms of a particular set of variables; but the conditional densities involved are not robust to a change of variables. 