

<!-- === Source: MinerU_markdown_Stochastic_Differential_Equations_1_2122706224590991377.md (Page 1) === -->

# Stochastic Diferential Equations

Do not worry about your problems with mathematics, I assure you mine are far greater. 

Albert Einstein. 

Florian Herzog 

2013 

## Stochastic Diferential Equations (SDE)

A ordinary diferential equation (ODE) 

$$
{\frac {d x (t)}{d t}} = f (t, x), d x (t) = f (t, x) d t,\tag{1}
$$

with initial conditions $x ( 0 ) = x _ { 0 }$ can be written in integral form 

$$
x (t) = x _ {0} + \int_ {0} ^ {t} f (s, x (s)) d s,\tag{2}
$$

where $x ( t ) = x ( t , x _ { 0 } , t _ { 0 } )$ is the solution with initial conditions $x ( t _ { 0 } ) ~ = ~ x _ { 0 }$ . An example is given as 

$$
{\frac {d x (t)}{d t}} = a (t) x (t), \quad x (0) = x _ {0}.\tag{3}
$$

## Stochastic Diferential Equations (SDE)

When we take the ODE (3) and assume that $a ( t )$ is not a deterministic parameter but rather a stochastic parameter, we get a stochastic diferential equation (SDE). The stochastic parameter $a ( t )$ is given as 

$$
a (t) = f (t) + h (t) \xi (t),\tag{4}
$$

where $\xi ( t )$ denotes a white noise process. 

Thus, we obtain 

$$
\frac {d X (t)}{d t} = f (t) X (t) + h (t) X (t) \xi (t).\tag{5}
$$

When we write (5) in the diferential form and use $d W ( t ) = \xi ( t ) d t$ , where dW(t) denotes diferential form of the Brownian motion,we obtain: 

$$
d X (t) = f (t) X (t) d t + h (t) X (t) d W (t).\tag{6}
$$

# Stochastic Diferential Equations (SDE)

In general an SDE is given as 

$$
d X (t, \omega) = f (t, X (t, \omega)) d t + g (t, X (t, \omega)) d W (t, \omega),\tag{7}
$$

where $\omega$ denotes that $X = X ( t , \omega )$ is a random variable and possesses the initial condition $X ( 0 , \omega ) ~ = ~ X _ { 0 }$ with probability one. As an example we have already encountered 

$$
d Y (t, \omega) = \mu (t) d t + \sigma (t) d W (t, \omega).
$$

Furthermore, $f ( t , X ( t , \omega ) ) \in \mathbb { R } , g ( t , X ( t , \omega ) ) \in \mathbb { R }$ , and $W ( t , \omega ) \in \mathbb { R }$ . Similar as in (2) we may write (7) as integral equation 

$$
X (t, \omega) = X _ {0} + \int_ {0} ^ {t} f (s, X (s, \omega)) d s + \int_ {0} ^ {t} g (s, X (s, \omega)) d W (s, \omega).\tag{8}
$$

## Stochastic Integrals

For the calculation of the stochastic integral $\begin{array} { r } { \int _ { 0 } ^ { T } g ( t , \omega ) d W ( t , \omega ) } \end{array}$ , we assume that $g ( t , \omega )$ is only changed at discrete time points $t _ { i } ( i = 1 , 2 , 3 , . . . , N - 1 )$ , where $0 = t _ { 0 } < t _ { 1 } < t _ { 2 } < . . . < t _ { N - 1 } < t _ { N } < T$ . We define the integral 

$$
S = \int_ {0} ^ {T} g (t, \omega) d W (t, \omega),\tag{9}
$$

as the Riemannßum 

$$
S _ {N} (\omega) = \sum_ {i = 1} ^ {N} g (t _ {i - 1}, \omega) \left(W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)\right).\tag{10}
$$

with $N  \infty$ 

## Stochastic Integrals

A random variable S is called the Itˆo integral of a stochastic process $g ( t , \omega )$ with respect to the Brownian motion $W ( t , \omega )$ on the interval $[ 0 , T ]$ if 

$$
\lim _ {N \to \infty} \mathsf {E} \Big [ \Big (S - \sum_ {i = 1} ^ {N} g (t _ {i - 1}, \omega) \Big (W (t _ {i}, \omega) - (W (t _ {i - 1}, \omega) \Big) \Big ] = 0,\tag{11}
$$

for each sequence of partitions $( t _ { 0 } , t _ { 1 } , \ldots , t _ { N } )$ of the interval $[ 0 , T ]$ such that $\operatorname* { m a x } _ { i } ( t _ { i } - t _ { i - 1 } ) \to 0$ . The limit in the above definition converges to the stochastic integral in the mean-square sense. Thus, the stochastic integral is a random variable, the samples of which depend on the individual realizations of the paths $W ( . , \omega )$ 

## Stochastic Integrals

The simplest possible example is $g ( t ) = c$ for all t. This is still a stochastic process, but a simple one. Taking the definition, we actually get 

$$
\begin{array}{r c l} \int_ {0} ^ {T} c d W (t, \omega) & = & c \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} \Big (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega) \Big) \\ & = & c \lim _ {N \to \infty} [ (W (t _ {1}, \omega) - W (t _ {0}, \omega)) + (W (t _ {2}, \omega) - W (t _ {1}, \omega)) + \ldots \\ & & + (W (t _ {N}, \omega) - W (t _ {N - 1}, \omega)) \\ & = & c (W (T, \omega) - W (0, \omega)), \end{array}
$$

where $W ( T , \omega )$ and $W ( 0 , \omega )$ are standard Gaussian random variables. With $W ( 0 , \omega ) = 0$ , the last result becomes 

$$
\int_ {0} ^ {T} c d W (t, \omega) = c W (T, \omega).
$$

## Stochastic Integrals

$$
\begin{array}{r l} & {\mathrm{Example:} g (t, \omega) = W (t, \omega) \quad \int_ {0} ^ {T} W (t, \omega) d W (t, \omega) =} \\ & {= \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} W (t _ {i - 1}, \omega) \Big (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega) \Big)} \\ & {= \lim _ {N \to \infty} \left[ \frac {1}{2} \sum_ {i = 1} ^ {N} (W ^ {2} (t _ {i}, \omega) - W ^ {2} (t _ {i - 1}, \omega)) - \frac {1}{2} \sum_ {i = 1} ^ {N} (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} \right]} \\ & {= - \frac {1}{2} \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} + \frac {1}{2} W ^ {2} (T, \omega),} \end{array} \tag {12}
$$

where we have used the following algebraic relationship $y ( x - y ) = y x - y ^ { 2 } +$ ${ \textstyle { \frac { 1 } { 2 } } } x ^ { 2 } - { \textstyle { \frac { 1 } { 2 } } } x ^ { 2 } = { \textstyle { \frac { 1 } { 2 } } } x ^ { 2 } - { \textstyle { \frac { 1 } { 2 } } } y ^ { 2 } - { \textstyle { \frac { 1 } { 2 } } } ( x - y ) ^ { 2 }$ 

## Stochastic Integrals

We take now a detailed look at :lim $\begin{array} { r } { { { \mathbf { \phi } } _ { N  \infty } } \sum _ { i = 1 } ^ { N } ( W ( t _ { i } , \omega ) - W ( t _ { i - 1 } , \omega ) ) ^ { 2 } } \end{array}$ 

$$
\begin{array}{r l r} \mathsf {E} [ \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} ] & = & \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} \mathsf {E} [ (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} ] \\ & = & \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} (t _ {i} - t _ {i - 1}) \\ & = & T \end{array}
$$

$$
\begin{array}{r l r} \mathsf {V a r} [ \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} ] & = & \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} \mathsf {V a r} [ (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} ] \\ & = & 2 \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} (t _ {i} - t _ {i - 1}) ^ {2}. \end{array}
$$

## Stochastic Integrals

By reducing the partition, the variance becomes zero, 

$$
\begin{array}{r l r} \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} (t _ {i} - t _ {i - 1}) ^ {2} & \leq & \max _ {i} (t _ {i} - t _ {i - 1}) \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} (t _ {i} - t _ {i - 1}) \\ & = & \max _ {i} (t _ {i} - t _ {i - 1}) T \\ & = & 0, \end{array}\tag{13}
$$

since $t _ { i - 1 } - t _ { i } \to 0$ . Since the expected value of $\begin{array} { r } { \sum _ { i = 1 } ^ { N } ( t _ { i } - t _ { i - 1 } ) ^ { 2 } } \end{array}$ is T and the variance becomes zero, we get 

$$
\sum_ {i = 1} ^ {N} (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} = T\tag{14}
$$

## Stochastic Integrals

The stochastic integral has the solution 

$$
\int_ {0} ^ {T} W (t, \omega) d W (t, \omega) = \frac {1}{2} W ^ {2} (T, \omega) - \frac {1}{2} T\tag{15}
$$

This is in contrast to our intuition from standard calculus. In the case of a deterministic integral $\begin{array} { r } { \int _ { 0 } ^ { T } x ( t ) d x ( t ) = \frac { 1 } { 2 } x ^ { 2 } ( t ) } \end{array}$ , whereas the Itˆo integral difers by the term $- { \frac { 1 } { 2 } } T$ — This example shows that the rules of diferentiation (in particular the chain rule) and integration need to be re-formulated in the stochastic calculus. 

## Stochastic Integrals

Properties of Itˆo Integrals. 

$$
E [ \int_ {0} ^ {T} g (t, \omega) d W (t, \omega) ] = 0.
$$

Proof: 

$$
\begin{array}{r c l} E [ \int_ {0} ^ {T} g (t, \omega) d W (t, \omega) ] & = & E [ \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} g (t _ {i - 1}, \omega) (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ] \\ & = & \lim _ {N \to \infty} \sum_ {i = 1} ^ {N} E [ g (t _ {i - 1}, \omega) ] E [ (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ] \\ & = & 0. \end{array}
$$

The expectation of stochastic integrals is zero. This is what we would expect anyway. 

## Stochastic Integrals

Properties of Itˆo Integrals. 

$$
\mathsf {V a r} \Big [ \int_ {0} ^ {T} g (t, \omega) d W (t, \omega) \Big ] = \int_ {0} ^ {T} E [ g ^ {2} (t, \omega) ] d t.\tag{16}
$$

Proof: 

$$
\begin{array}{r l r} \mathsf {V a r} \Big [ \int_ {0} ^ {T} g (t, \omega) d W (t, \omega) \Big ] & = & E \Big [ (\int_ {0} ^ {T} g (t, \omega) d W (t, \omega)) ^ {2} \Big ] \\ & = & E \Big [ \Big (\lim _ {N \to \infty} \sum_ {i = 1} ^ {N} g (t _ {i - 1}, \omega) \Big (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega) \Big) \Big) ^ {2} \Big ] \end{array}
$$

Stochastic Integrals 

$$
\begin{array}{r l} {=} & {\lim _ {N \to \infty} \sum_ {i = 1} ^ {N} \sum_ {j = 1} ^ {N} E [ g (t _ {i - 1}, \omega) g (t _ {j - 1}, \omega)} \\ & {(W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) (W (t _ {j}, \omega) - W (t _ {j - 1}, \omega)) ]} \\ {=} & {\lim _ {N \to \infty} \sum_ {i = 1} ^ {N} E [ g ^ {2} (t _ {i - 1}, \omega) ] E [ (W (t _ {i}, \omega) - W (t _ {i - 1}, \omega)) ^ {2} ]} \\ {=} & {\lim _ {N \to \infty} \sum_ {i = 1} ^ {N} E [ g ^ {2} (t _ {i - 1}, \omega) ] (t _ {i} - t _ {i - 1})} \\ {=} & {\int_ {0} ^ {T} E [ g ^ {2} (t, \omega) ] d t.} \end{array}\tag{17}
$$

# Stochastic Integrals

The calculation of the variance of the Itˆo Integrals shows two important properties: 

$$
\bullet \mathsf {E} \Big [ \Big (\int_ {0} ^ {T} g (t, \omega) d W (t, \omega) \Big) ^ {2} \Big ] = \int_ {0} ^ {T} \mathsf {E} \Big [ g ^ {2} (t, \omega) \Big ] d t
$$

• $\begin{array} { r } { \int _ { 0 } ^ { T } \mathsf { E } [ g ^ { 2 } ( t , \omega ) ] d t < \infty } \end{array}$ 

The second property is the condition of existence for Itˆo integrals. The next property is the linearity of Itˆo integrals: 

$$
\int_ {0} ^ {T} [ a _ {1} g _ {1} (t, \omega) + a _ {2} g _ {2} (t, \omega) ] d W (t, \omega)
$$

$$
= a _ {1} \int_ {0} ^ {T} g _ {1} (t, \omega) d W (t, \omega) + a _ {2} \int_ {0} ^ {T} g _ {2} (t, \omega) d W (t, \omega),\tag{18}
$$

for numbers $a _ { 1 } , a _ { 2 }$ and stochastic functions $g _ { 1 } ( t , \omega ) , g _ { 2 } ( t , \omega )$ 

## Itˆo’s lemma

As mentioned shown in the second example, the rules of classical calculus are not valid for stochastic integrals and diferential equations. It is the equivalent to the chain rule in classical calculus. The problem can be stated as follows: 

Given a stochastic diferential equation 

$$
d X (t) = f (t, X (t)) d t + g (t, X (t)) d W (t),\tag{19}
$$

and another process $Y ( t )$ which is a function of $X ( t )$ 

$$
Y (t) = \phi (t, X (t)),
$$

where the function $\phi ( t , X ( t ) )$ is continuously diferentiable in t and twice continuously diferentiable in X, find the stochastic diferential equation for the process $Y ( t )$ 

$$
d Y (t) = \tilde {f} (t, X (t)) d t + \tilde {g} (t, X (t)) d W (t).
$$

## Itˆo’s lemma

In the case when we assume that $g ( t , X ( t ) ) = 0$ , we know the result: the chain rule for standard calculus. The result is given by 

$$
d y (t) = (\phi_ {t} (t, x) + \phi_ {x} (t, x) f (t, x)) d t.\tag{20}
$$

In the case of stochastic problems, we reason as follows: The Taylor expansion of $\phi ( t , X ( t ) )$ yields 

$$
\begin{array}{r l r} {d Y (t)} & = & {\phi_ {t} (t, X) d t + \frac {1}{2} \phi_ {t t} (t, X) d t ^ {2} + \phi_ {x} (t, X) d X (t)} \\ & & {+ \frac {1}{2} \phi_ {x x} (t, X) (d X (t)) ^ {2} + \textsf {h . o . t .}} \end{array}\tag{21}
$$

## Itˆo’s lemma

We use (19) for $d X ( t )$ and get 

$$
\begin{array}{r c l} d Y (t) & = & \phi_ {t} (t, X) d t + \phi_ {x} (t, X) [ f (t, X (t)) d t + g (t, X (t)) d W (t) ] \\ & & + \phi_ {t t} (t, X) d t ^ {2} + \frac {1}{2} \phi_ {x x} (t, X) \left(f ^ {2} (t, X (t)) d t ^ {2} + g ^ {2} (t, X (t)) d W ^ {2} (t) \right. \\ & & \left. + 2 f (t, X (t)) g (t, X (t)) d t d W (t)\right) + \text {h.o.t.}. \end{array} \tag {22}
$$

The diferentials of higher order $( d t , d W )$ become fast zero, $d t ^ { 2 } \ \to \ 0$ and $d t d W ( t ) \to 0$ . The stochastic term $d W ^ { 2 } ( t )$ according to the rules of Brownian motion is given as 

$$
d W ^ {2} (t, \omega) = d t.\tag{23}
$$

## Itˆo’s lemma

Omitting higher order terms and using the properties of Brownian motion, we arrive at 

$$
\begin{array}{r c l} d Y (t) & = & \left[ \phi_ {t} (t, X) + \phi_ {x} (t, X) f (t, X (t)) + \frac {1}{2} \phi_ {x x} (t, X) g ^ {2} (t, X (t)) \right] d t \\ & & + \phi_ {x} (t, X) g (t, X (t)) d W (t). \end{array} \tag {2}\tag{24}
$$

Reordering the terms yields the scalar version of Itˆo’s Lemma: 

$$
{ d Y ( t ) } { = } { \tilde { f } ( t , X ( t ) ) d t + \tilde { g } ( t , X ( t ) ) d W ( t ) , }\tag{25}
$$

$$
\tilde {f} (t, X (t)) = \phi_ {t} (t, X) + \phi_ {x} (t, X) f (t, X (t))
$$

$$
+ \frac {1}{2} \phi_ {x x} (t, X) g ^ {2} (t, X (t)),\tag{26}
$$

$$
\tilde {g} (t, X (t)) = \phi_ {x} (t, X) g (t, X (t)).\tag{27}
$$

## Itˆo’s lemma

The term ${ \scriptstyle \frac { 1 } { 2 } } \phi _ { x x } ( t , X ) g ^ { 2 } ( t , X ( t ) )$ is often called the Itˆo corretion term, since this does not occur in the det. case. 

We apply Itˆos formula for the following problem: $\phi ( t , X ) ~ = ~ X ^ { 2 } \quad \quad \quad { }$ with the SDE $d X ( t ) = d W ( t )$ . From the SDE, we get $X ( t ) = W ( t )$ and calculate the partial derivatives of $\begin{array} { r } { \frac { \partial \phi ( t , X ) } { \partial X } = 2 X , \frac { \partial ^ { 2 } \phi ( t , X ) } { \partial X ^ { 2 } } = 2 } \end{array}$ , and $\begin{array} { r } { \frac { \partial \phi ( t , \boldsymbol { X } ) } { \partial t } = 0 } \end{array}$ . The Itˆo lemma yields 

$$
d (W ^ {2} (t)) = 1 d t + 2 W (t) d W (t).\tag{28}
$$

We rewrite the equation and use $W ( 0 ) = 0$ 

$$
{W ^ {2} (t)} = {1 t + 2 \int_ {0} ^ {t} W (t) d W (t),}
$$

$$
\int_ {0} ^ {t} W (t) d W (t) = \frac {1}{2} W ^ {2} (t) - \frac {1}{2} t.\tag{29}
$$

## Itˆo’s lemma

We now allow that the process $X ( t )$ is in $\mathbb { R } ^ { n }$ . We let $W ( t )$ be an m-dimensional standard Brownian motion and $f ( t , X ( t ) ) \in \mathbb { R } ^ { n }$ and $g ( t , X ( t ) ) \in \mathbb { R } ^ { n \times m }$ . Consider a scalar process $Y ( t )$ defined by $Y ( t ) = \phi ( t , X ( t ) )$ , where $\phi ( t , X )$ is a scalar function which is continuously diferentiable with respect to $t$ and twice continuously diferentiable with respect to $X$ . The Itˆo formula can be written in vector notation as follows: 

$$
{ d Y ( t ) } { = } { \tilde { f } ( t , X ( t ) ) d t + \tilde { g } ( t , X ( t ) ) d W ( t ) , }\tag{30}
$$

$$
\tilde {f} (t, X (t)) = \phi_ {t} (t, X (t)) + \phi_ {x} (t, X (t)) \cdot f (t, X (t))
$$

$$
+ \frac {1}{2} t r \Big (\phi_ {x x} (t, X (t)) g (t, X (t)) g ^ {T} (t, X (t))) \Big),\tag{31}
$$

$$
\tilde {g} (t, X (t)) = \phi_ {x} (t, X (t)) \cdot g (t, X (t)),\tag{32}
$$

where $" \mathrm { t r } "$ denotes the trace operator. 

## Itˆo’s lemma

Consider the following stochastic diferential equation: 

$$
d S (t) = \mu S (t) d t + \sigma S (t) d W (t),\tag{33}
$$

We want to find the SDE for the process Y related to S as follows: $Y ( t ) = \phi ( t , S ) =$ $\ln ( S ( t ) )$ . The partial derivatives are: $\begin{array} { r } { \frac { \partial \phi ( t , S ) } { \partial S } = \frac { 1 } { S } , \frac { \partial ^ { 2 } \phi ( t , S ) } { \partial S ^ { 2 } } = - \frac { 1 } { S ^ { 2 } } } \end{array}$ , and $\begin{array} { r } { \frac { \partial \phi ( t , S ) } { \partial t } = 0 } \end{array}$ Therefore, according to Itˆo we get, 

$$
\begin{array}{r l r} {d Y (t)} & = & {\left(\frac {\partial \phi (t , S)}{\partial t} + \frac {\partial \phi (t , S)}{\partial S} \mu S (t) + \frac {1}{2} \frac {\partial^ {2} \phi (t , S)}{\partial S ^ {2}} \sigma^ {2} S ^ {2} (t)\right) d t} \\ & & {+ \left(\frac {\partial \phi (t , S)}{\partial S} \sigma S (t)\right) d W (t),} \end{array}\tag{34}
$$

$$
{ d Y ( t ) } { = } { ( \mu - \frac { 1 } { 2 } \sigma ^ { 2 } ) d t + \sigma d W ( t ) . }\tag{35}
$$

## Itˆo’s lemma

Since the right hand side of (35) is independent of $Y ( t )$ , we are able to compute the stochastic integral: 

$$
{ Y ( t ) } { = } { Y _ { 0 } + \int _ { 0 } ^ { t } ( \mu - \frac { 1 } { 2 } \sigma ^ { 2 } ) d t + \int _ { 0 } ^ { t } \sigma d W , }\tag{36}
$$

$$
{ Y ( t ) } { = } { Y _ { 0 } + ( \mu - \frac { 1 } { 2 } \sigma ^ { 2 } ) t + \sigma W ( t ) . }\tag{37}
$$

Since $Y ( t ) = \ln S ( t )$ we have found a solution for $S ( t )$ 

$$
\ln (S (t)) = \ln (S (0)) + (\mu - \frac {1}{2} \sigma^ {2}) t + \sigma W (t),\tag{38}
$$

$$
{ S ( t ) } { = } { S ( 0 ) e ^ { ( \mu - \frac { 1 } { 2 } \sigma ^ { 2 } ) t + \sigma W ( t ) } , }\tag{39}
$$

where $W ( t )$ is a standard BM. 

## Itˆo’s lemma

Show for $U ( t ) = X _ { 1 } ( t ) X _ { 2 } ( t )$ with 

$$
\begin{array}{r l r} {d X _ {1} (t)} & = & {f _ {1} (t, X _ {1}) d t + g _ {1} (t, X _ {1}) d W (t),} \\ {d X _ {2} (t)} & = & {f _ {2} (t, X _ {2}) d t + g _ {2} (t, X _ {2}) d W (t),} \end{array}
$$

that following formula is valid: 

$$
d U (t) = d X _ {1} (t) X _ {2} (t) + X _ {1} (t) d X _ {2} (t) + g _ {1} (t, X _ {1}) g _ {2} (t, X _ {2}) d t\tag{40}
$$

We show that we obtain the same result as in the previous formula by apply Itˆo’s lemma. By (40) liefert 

$$
\begin{array}{r l r} {d U (t)} & = & {[ X _ {2} (t) f _ {1} (t, X _ {1}) + X _ {1} (t) f _ {2} (t, X _ {2}) + g _ {1} (t, X _ {1}) g _ {2} (t, X _ {2}) ] d t} \\ & & {+ [ X _ {2} (t) g _ {1} (t, X _ {1}) + X _ {1} (t) g _ {2} (t, X _ {2}) ] d W (t)} \end{array}
$$

## Itˆo’s lemma

The partial derivatives of U are : $\begin{array} { r } { \frac { \partial U } { \partial X } = ( X _ { 2 } ( t ) , X _ { 1 } ( t ) ) ^ { T } , \frac { \partial ^ { 2 } U } { \partial X ^ { 2 } } = \left[ \begin{array} { l l } { 0 } & { 1 } \\ { 1 } & { 0 } \end{array} \right] } \end{array}$ and $\begin{array} { r } { \frac { \partial U } { \partial t } = 0 . } \end{array}$ 

$$
\begin{array}{r c l} d U (t) & = & [ \frac {\partial U}{\partial t} + \frac {\partial U}{\partial X} [ f _ {1} (t, X _ {1}), f _ {2} (t, X _ {2}) ] ^ {T} \\ & & + \frac {1}{2} t r \Big (\frac {\partial^ {2} U}{\partial X ^ {2}} \left[ \begin{array}{c c} g _ {1} (t, X _ {1}) ^ {2} & g _ {1} (t, X _ {1}) g _ {2} (t, X _ {2}) \\ g _ {1} (t, X _ {1}) g _ {2} (t, X _ {2}) & g _ {2} (t, X _ {2}) ^ {2} \end{array} \right] \Big) ] d t \\ & & + \frac {\partial U}{\partial X} [ g _ {1} (t, X _ {1}), g _ {2} (t, X _ {2}) ] ^ {T} d W (t) \\ & = & [ X _ {2} (t) f _ {1} (t, X _ {1}) + X _ {1} (t) f _ {2} (t, X _ {2}) + g _ {1} (t, X _ {1}) g _ {2} (t, X _ {2}) ] d t \\ & & + [ X _ {2} (t) g _ {1} (t, X _ {1}) + X _ {1} (t) g _ {2} (t, X _ {2}) ] d W (t) \end{array}
$$

# Stochastic Diferential Equations (SDE)

We classify SDEs into two large groups, linear SDEs and non-linear SDEs. Furthermore, we distinguish between scalar linear and vector-valued linear SDEs. 

We start with the easy case, the scalar linear linear SDEs. An SDE 

$$
d X (t) = f (t, X (t)) d t + g (t, X (t)) d W (t),\tag{41}
$$

for a one-dimensional stochastic process $X ( t )$ is called a linear (scalar) SDE if and only if the functions $f ( t , X ( t ) )$ ) and $g ( t , X ( t ) )$ are afine functions of $X ( t ) \in \mathbb { R }$ and thus 

$$
\begin{array}{r c l} {f (t, X (t))} & = & {A (t) X (t) + a (t),} \\ {g (t, X (t))} & = & {\left[ B _ {1} (t) X (t) + b _ {1} (t), \dots , B _ {m} (t) X (t) + b _ {m} (t) \right],} \end{array}
$$

where $A ( t ) , a ( t ) \in \mathbb { R } , W ( t ) \in \mathbb { R } ^ { m }$ is an m-dimensional Brownian motion, and $B _ { i } ( t ) , b _ { i } ( t ) \in \mathbb { R } , i = 1 , \cdot \cdot \cdot , m$ . Hence, $\boldsymbol { f } ( t , \boldsymbol { X } ( t ) ) \in \mathbb { R } \mathrm { \sf ~ a n d ~ } \boldsymbol { g } ( t , \boldsymbol { X } ( t ) ) \in \mathbb { R } ^ { 1 \times m }$ 

## Stochastic Diferential Equations (SDE)

The linear SDE possesses the following solution 

$$
\begin{array}{r l r} {X (t)} & = & {\Phi (t) \Big (x _ {0} + \int_ {0} ^ {t} \Phi^ {- 1} (s) \Big [ a (s) - \sum_ {i = 1} ^ {m} B _ {i} (s) b _ {i} (s) \Big ] d s} \\ & & {+ \sum_ {i = 1} ^ {m} \int_ {0} ^ {t} \Phi^ {- 1} (s) b _ {i} (s) d W _ {i} (s) \Big),} \end{array}\tag{42}
$$

where we denote $\Phi ( t )$ as the fundamental matrix, which we obtain from 

$$
\Phi (t) = \exp \Big (\int_ {0} ^ {t} \Big [ A (s) - \sum_ {i = 1} ^ {m} \frac {B _ {i} ^ {2} (s)}{2} \Big ] d s + \sum_ {i = 1} ^ {m} \int_ {0} ^ {t} B _ {i} (s) d W _ {i} (s) \Big),\tag{43}
$$

The solution is similar to the solution of ODEs. 

## Stochastic Diferential Equations (SDE)

Let us assume that $W ( t ) \in \mathbb { R } , a ( t ) = 0 , b ( t ) = 0 , A ( t ) = A , B ( t ) = B$ . We want to compute the solution of the SDE 

$$
d X (t) = A X (t) d t + B X (t) d W (t), \quad X (t) = x _ {0},\tag{44}
$$

We can solve it using (42) and (43): 

$$
\Phi (t) = e ^ {(A - \frac {1}{2} B ^ {2}) t + B W (t)},\tag{45}
$$

and (42) is easy to calculate since 

$$
x (t) = \Phi (t) x _ {0} = x _ {0} e ^ {(A - \frac {1}{2} B ^ {2}) t + B W (t)}.\tag{46}
$$

## Stochastic Diferential Equations (SDE)

The expectation $m ( t ) = \mathsf E [ X ( t ) ]$ ]and the second moment $P ( t ) = \mathsf { E } [ X ^ { 2 } ( t ) ]$ for 

$$
d X (t) = (A (t) X (t) + a (t)) d t + \sum_ {i = 1} ^ {m} (B _ {i} (t) X (t) + b (t)) d W _ {i} (t).\tag{47}
$$

can be calculated by solving the following system of ODEs: 

(48) 

$$
\begin{array}{r c l} \dot {m} (t) & = & A (t) m (t) + a (t), m (0) = x _ {0}, \\ \dot {P} (t) & = & \left(2 A (t) + \sum_ {i = 1} ^ {m} B _ {i} ^ {2} (t)\right) P (t) + 2 m (t) \left(a (t) + \sum_ {i = 1} ^ {m} B _ {i} (t) b _ {i} (t)\right) \\ & & + \sum_ {i = 1} ^ {m} b _ {i} ^ {2} (t)), P (0) = x _ {0} ^ {2}. \end{array}\tag{49}
$$

## Stochastic Diferential Equations (SDE)

The ODE for the expectation is derived by applying the expectation operator on both sides of (42). 

$$
\begin{array}{r c l} \mathsf {E} [ d X (t) ] & = & \mathsf {E} [ (A (t) X (t) + a (t)) d t + \sum_ {i = 1} ^ {m} (B _ {i} (t) X (t) + b _ {i} (t)) d W _ {i} (t) ] \\ \underbrace {\mathsf {E} [ d X (t) ]} _ {d m (t)} & = & (A (t) \underbrace {\mathsf {E} [ X (t) ]} _ {= m (t)} + a (t)) d t \\ & & + \sum_ {i = 1} ^ {m} \mathsf {E} [ (B _ {i} (t) X (t) + b _ {i} (t)) ] \underbrace {\mathsf {E} [ d W _ {i} (t) ]} _ {= 0} \\ d m (t) & = & (A (t) m (t) + a (t)) d t. \end{array}\tag{50}
$$

## Stochastic Diferential Equations (SDE)

In order to compute the second moment, we need to derive the SDE for $Y ( t ) = X ^ { 2 } ( t )$ 

$$
\begin{array}{r c l} d Y (t) & = & \left[ 2 X (t) (A (t) X (t) + a (t)) + \sum_ {i = 1} ^ {m} \left(B _ {i} (t) X (t) + b _ {i} (t)\right) ^ {2} \right] d t \\ & & + 2 X (t) \sum_ {i = 1} ^ {m} \left(B _ {i} (t) X (t) + b _ {i} (t)\right) d W _ {i} (t) \\ d Y (t) & = & \left[ 2 A (t) X ^ {2} (t) + 2 X (t) a (t) + \sum_ {i = 1} ^ {m} \left(B _ {i} ^ {2} (t) X ^ {2} (t) + 2 B _ {i} (t) b _ {i} (t) X (t) \right. \right. \\ & & \left. \left. + b _ {i} ^ {2} (t)\right) \right] d t + 2 X (t) \sum_ {i = 1} ^ {m} \left(B _ {i} (t) X (t) + b _ {i} (t)\right) d W _ {i} (t) \end{array} \tag {51}
$$

## Stochastic Diferential Equations (SDE)

Furthermore, we apply the expectation operator to (52) and use $P ( t ) = \mathsf { E } [ X ^ { 2 } ( t ) ] =$ $\mathsf { E } [ Y ( t ) ]$ and $m ( t ) = \mathsf E [ X ( t ) ]$ ]. 

$$
\begin{array}{r l r} \mathsf {E} [ d Y (t) ] & = & {\Big [ 2 A (t) \mathsf {E} [ X ^ {2} (t) ] + 2 a (t) \mathsf {E} [ X (t) ] + \sum_ {i = 1} ^ {m} \Big (B _ {i} ^ {2} (t) \mathsf {E} [ X ^ {2} (t) ]} \\ & & {+ 2 B _ {i} (t) b _ {i} (t) \mathsf {E} [ X (t) ] + \left. b _ {i} ^ {2} (t)\right) \Big ] d t} \\ & & {+ \mathsf {E} \Big [ 2 X (t) \sum_ {i = 1} ^ {m} \Big (B _ {i} (t) X (t) + b _ {i} (t) \Big) d W _ {i} (t) \Big ]} \end{array}
$$

$$
\begin{array}{r l r} {d P (t)} & = & {\Big [ 2 A (t) P (t) + 2 a (t) m (t)} \\ & & {+ \sum_ {i = 1} ^ {m} \Big (B _ {i} ^ {2} (t) P (t) + 2 B _ {i} (t) b _ {i} (t) m (t) + b _ {i} ^ {2} (t) \Big) \Big ] d t} \end{array}
$$

## Stochastic Diferential Equations (SDE)

In the case that $B _ { i } ( t ) = 0 , ~ i = 1 , \ldots , m$ , we are able to directly compute the distribution. The scalar linear SDE 

$$
d X (t) = (A (t) X (t) + a (t)) d t + \sum_ {i = 1} ^ {m} b _ {i} (t) d W _ {i} (t),\tag{53}
$$

with $X ( 0 ) = x _ { 0 }$ is normaly distributed 

$P ( X ( t ) | x _ { 0 } ) \sim { \mathcal { N } } ( m ( t ) , V ( t ) )$ with expected value $m ( t )$ and variance $V ( t )$ , which are solutions of the following ODEs, 

$$
\dot {m} (t) = A (t) m (t) + a (t), m (0) = x _ {0},\tag{54}
$$

$$
\dot {V} (t) = 2 A (t) V (t) + \sum_ {i = 1} ^ {m} b _ {i} ^ {2} (t), V (0) = 0.\tag{55}
$$

## Stochastic Diferential Equations (SDE)

There are some specific scalar linear SDEs which are found to be quite useful in practice. The simplest case of SDE is where the drift and the difusion coeficients are independent of the information received over time 

$$
d S (t) = \mu d t + \sigma d W (t), S (0) = S _ {0}.\tag{56}
$$

This model has been used to simulate commodity prices, such as metals or agricultural products. 

The mean is $\mathsf E [ S ( t ) ] = \mu t + S _ { 0 }$ and the variance $\mathsf { V a r } [ S ( t ) ] = \sigma ^ { 2 } t . \ S ( t )$ possesses a behavior of fluctuations around the straight line $S _ { 0 } + \mu t$ .The process is normally distributed with the given mean and variance. 

## Stochastic Diferential Equations (SDE)

The standard model of stock prices is the geometric Brownian motion as given by 

$$
d S (t) = \mu S (t) d t + \sigma S (t) d W (t, \omega), S (0) = S _ {0}.
$$

The mean is given by $\mathsf E [ S ( t ) ] = S _ { 0 } e ^ { \mu t }$ and its variance by $\mathsf { V a r } [ S ( t ) ] = S _ { 0 } ^ { 2 } e ^ { 2 \mu t } ( e ^ { \sigma ^ { 2 } t } -$ 1). This model forms the starting point for the famous Black-Scholes formula for option pricing. The geometric Brownian motion has two main features which make it popular for stock 

The first property is that $S ( t ) > 0$ for all $t \in [ 0 , T ]$ and the second is that all returns are in scale with the current price. This process has a log-normal probability density function. 

## Stochastic Diferential Equations (SDE)

Another very popular class of SDEs are mean reverting linear SDEs. The model is obtained by 

$$
d S (t) = \kappa [ \mu - S (t) ] d t + \sigma d W (t, \omega), S (0) = S _ {0}.\tag{57}
$$

A special case of this SDE where $\mu ~ = ~ 0$ is called Ohrnstein-Uhlenbeck process. Equation (57) models a process which naturally falls back to its equilibrium level of $\mu .$ The expected price is $\mathsf E [ S ( t ) ] = \mu - ( \mu - S _ { 0 } ) e ^ { - \kappa t }$ and the variance is 

$$
\mathsf {V a r} [ S (t) ] = \frac {\sigma^ {2}}{2 \kappa} \Bigl (1 - e ^ {- 2 \kappa t} \Bigr).
$$

## Stochastic Diferential Equations (SDE)

In the long run, the following (unconditional) approximations are valid 

$$
\lim _ {t \to \infty} \mathsf {E} [ S (t) ] = \mu
$$

and 

$$
\lim _ {t \to \infty} \mathsf {V a r} [ S (t) ] = \frac {\sigma^ {2}}{2 \kappa}.
$$

This analysis shows that the process fluctuates around $\mu$ and has a variance of $\frac { \sigma ^ { 2 } } { 2 \kappa }$ which depends on the parameter $\kappa \cdot$ the higher $\kappa ,$ , the lower the variance. 

This is obvious since the higher κ, the faster the process reverts back to its mean value. 

This process is a stationary process which is normally distributed. 

## Stochastic Diferential Equations (SDE)

A popular extension is where the difusion term is in scale with the current value, i.e., the geometric mean reverting process: 

$$
d S (t) = \kappa [ \mu - S (t) ] d t + \sigma S (t) d W (t, \omega), S (0) = S _ {0}.
$$

In this model $S ( t ) \geq 0 , { \mathrm { i f ~ } } S _ { 0 } \geq 0 , \mu > 0$ , and $\kappa > 0$ 

The first mean reversion model(57) may produce negative values even for $\mu > 0$ 

Since the second mean-reversion model has always positive realizations, it is also called log-normal mean reversion. This type of model is used to model interest rate or volatilities. 

## Stochastic Diferential Equations (SDE)

In control engineering science, the most important (scalar) case is 

$$
d X (t) = \left(A (t) X (t) + C (t) u (t)\right) d t + \sum_ {i = 1} ^ {m} b _ {i} (t) d W _ {i}.\tag{58}
$$

In this equation, $X ( t )$ is normally distributed because the Brownian motion is just multiplied by time-dependent factors. 

When we compute an optimal control law for this SDE, the deterministic optimal control law (ignoring the Brownian motion) and the stochastic optimal control law are the same. 

This feature is called certainty equivalence. For this reason, the stochastics are often ignored in control engineering. 

## Stochastic Diferential Equations (SDE)

The logical extension of scalar SDEs is to allow $\ b X ( t ) \in \mathbb R ^ { n }$ to be a vector. The rest of this section proceeds in a similar fashion as for scalar linear SDEs. A stochastic vector diferential equation 

$$
d X (t) = f (t, X (t)) d t + g (t, X (t)) d W (t)
$$

with the initial condition $X ( 0 ) = x _ { 0 } \in \mathbb { R } ^ { n }$ for an n-dimensional stochastic process X(t) is called a linear SDE if the functions $f ( t , X ( t ) ) \in \mathbb { R } ^ { n }$ and $g ( t , X ( t ) ) \in \mathbb { R } ^ { n \times m }$ are afine functions of X(t) and thus 

$$
f (t, X (t)) = A (t) X (t) + a (t),
$$

$$
{g (t, X (t))} = {\left[ B _ {1} (t) X (t) + b _ {1} (t), \dots , B _ {m} (t) X (t) + b _ {m} (t) \right],}
$$

where $A ( t ) \in \mathbb { R } ^ { n \times n } , \ a ( t ) \in \mathbb { R } ^ { n } , \ W ( t ) \in \mathbb { R } ^ { m }$ is an m-dimensional Brownian motion, and $B _ { i } ( t ) \in \mathbb { R } ^ { n \times n } , \ b _ { i } ( t ) \in \mathbb { R } ^ { n }$ 

## Stochastic Diferential Equations (SDE)

Alternatively, the vector-valued linear SDE can be written as 

$$
d X (t) = (A (t) X (t) + a (t)) d t + \sum_ {i = 1} ^ {m} (B _ {i} (t) X (t) + b _ {i} (t)) d W _ {i} (t).\tag{59}
$$

A common extension of the above equation is the following form of a controlled stochastic diferential equation as given by 

$$
\begin{array}{r c l} d X (t) & = & (A (t) X (t) + C (t) u (t) + a (t)) d t \\ & & + \sum_ {i = 1} ^ {m} (B _ {i} (t) X (t) + D _ {i} (t) u (t) + b _ {i} (t)) d W _ {i}, \end{array}\tag{60}
$$

where $u ( t ) \in \mathbb { R } ^ { k } , C ( t ) \in \mathbb { R } ^ { n \times k } , D _ { i } ( t ) \in \mathbb { R } ^ { n \times k }$ 

## Stochastic Diferential Equations (SDE)

The linear SDE (59) has the following solution: 

$$
\begin{array}{r l r} {X (t)} & = & {\Phi (t) \Big (x _ {0} + \int_ {0} ^ {t} \Phi^ {- 1} (s) \Big [ a (s) - \sum_ {i = 1} ^ {m} B _ {i} (s) b _ {i} (s) \Big ] d s} \\ & & {+ \sum_ {i = 1} ^ {m} \int_ {0} ^ {t} \Phi^ {- 1} (s) b _ {i} (s) d W _ {i} (s) \Big),} \end{array}\tag{61}
$$

where the fundamental matrix $\Phi ( t ) \ \in \ \mathbb { R } ^ { n \times n }$ is the solution of the homogenous stochastic diferential equation. 

## Stochastic Diferential Equations (SDE)

The fundamental matrix $\Phi ( t ) \in \mathbb { R } ^ { n \times n }$ is the solution of the homogenous stochastic diferential equation: 

$$
d \Phi (t) = A (t) \Phi (t) d t + \sum_ {i = 1} ^ {m} B _ {i} (t) \Phi (t) d W _ {i} (t),\tag{62}
$$

with initial condition $\Phi ( { \boldsymbol { 0 } } ) = I , { \boldsymbol { I } } \in { \mathbb { R } } ^ { n \times n }$ e now prove that (61) and (62) are solutions of (59). We rewrite (61) as 

$$
{ X ( t ) } { = } { \Phi ( t ) \Big ( x _ { 0 } + \int _ { 0 } ^ { t } \Phi ^ { - 1 } ( t ) d Y ( t ) \Big ) }
$$

$$
{ d Y ( t ) } { = } { \left[ a ( t ) - \sum _ { i = 1 } ^ { m } B _ { i } ( t ) b _ { i } ( t ) \right] d t + \sum _ { i = 1 } ^ { m } b _ { i } ( t ) d W _ { i } ( t ) . }
$$

## Stochastic Diferential Equations (SDE)

$$
\begin{array}{r c l} {X (t)} & = & {\Phi (t) Z (t), \quad Z (t) = \left(x _ {0} + \int_ {0} ^ {t} \Phi^ {- 1} (t) d Y (t)\right)} \\ {d Z (t)} & = & {\Phi^ {- 1} (t) d Y (t)} \end{array}
$$

We use the Itˆo formula to calculate $X ( t ) = \Phi ( t ) Z ( t )$ 

$$
\begin{array}{r c l} {d X (t)} & = & {\Phi (t) d Z (t) + d \Phi (t) Z (t) + \sum_ {i = 1} ^ {m} B _ {i} (t) \Phi (t) \Phi (t) ^ {- 1} b _ {i} (t) d t} \\ & = & {d Y (t) + A (t) \Phi (t) Z (t) d t + \sum_ {i = 1} ^ {m} B _ {i} (t) \Phi (t) Z (t) d W _ {i} (t) + \sum_ {i = 1} ^ {m} B _ {i} (t) b _ {i} (t) d t} \end{array}
$$

## Stochastic Diferential Equations (SDE)

Noting that $Z ( t ) = \Phi ^ { - 1 } ( t ) X ( t )$ and using the SDE for $Y ( t )$ , we get 

$$
\begin{array}{r c l} d X (t) & = & d Y (t) + A (t) \Phi (t) Z (t) d t + \sum_ {i = 1} ^ {m} B _ {i} (t) \Phi (t) Z (t) d W _ {i} (t) + \sum_ {i = 1} ^ {m} B _ {i} (t) b _ {i} (t) d t \\ & = & \Big [ a (t) - \sum_ {i = 1} ^ {m} B _ {i} (t) b _ {i} (t) \Big ] d t + \sum_ {i = 1} ^ {m} b _ {i} (t) d W _ {i} (t) + A (t) X (t) d t \\ & & + \sum_ {i = 1} ^ {m} B _ {i} (t) X (t) d W _ {i} (t) + \sum_ {i = 1} ^ {m} B _ {i} (t) b _ {i} (t) d t \\ & = & [ a (t) + A (t) X (t) ] d t + \sum_ {i = 1} ^ {m} (B _ {i} (t) X (t) + b _ {i} (t)) d W _ {i} (t). \end{array}
$$

This completes the proof. 

## Stochastic Diferential Equations (SDE)

The expectation $m ( t ) = \mathsf { E } [ X ( t ) ] \in \mathbb { R } ^ { n }$ and the second moment matrix $P ( t ) =$ $\mathsf { E } [ X ( t ) X ^ { T } ( t ) ] \in \mathbb { R } ^ { n \times n }$ can be computed as follows: 

$$
\dot {m} (t) = A (t) m (t) + a (t), m (0) = x _ {0},\tag{63}
$$

$$
\begin{array}{r c l} \dot {P} (t) & = & A (t) P (t) + P (t) A ^ {T} (t) + a (t) m ^ {T} (t) + m (t) a ^ {T} (t) \\ & & + \sum_ {i = 1} ^ {m} [ B _ {i} (t) P (t) B _ {i} ^ {T} (t) + B _ {i} (t) m (t) b _ {i} ^ {T} (t) \\ & & + b _ {i} (t) m ^ {T} (t) B _ {i} ^ {T} (t) + b _ {i} (t) b _ {i} (t) ^ {T} ], P (0) = x _ {0} x _ {0} ^ {T}. \end{array}\tag{64}
$$

The covariance matrix for the system of linear SDEs is given by als 

$$
V (t) = \mathsf {V a r} \{x (t) \} = P (t) - m (t) m ^ {T} (t).\tag{65}
$$

## Stochastic Diferential Equations (SDE)

The special case 

$$
d X (t) = (A (t) X (t) + a (t)) d t + \sum_ {i = 1} ^ {m} b _ {i} (t) d W _ {i} (t)
$$

with the initial condition $X ( 0 ) = x _ { 0 } \in \mathbb { R } ^ { n }$ is normally distributed, i.e., 

$$
P (X (t) | x _ {0}) \sim \mathcal {N} (m (t), V (t))
$$

where 

$$
\begin{array}{r c l} \dot {m} (t) & = & A (t) m (t) + a (t) m (0) = x _ {0} \\ \dot {V} (t) & = & A (t) V (t) + V (t) A ^ {T} (t) + \sum_ {i = 1} ^ {m} b _ {i} b _ {i} ^ {T} (t) V (0) = 0. \end{array}
$$

## Stochastic Diferential Equations (SDE)

As first example of a linear vector valued SDE, we consider a two dimensional geometric Brownian motion: 

$$
d S _ {1} (t) = \mu_ {1} S _ {1} (t) d t + S _ {1} (t) \Big (\sigma_ {1 1} d W _ {1} (t) + \sigma_ {1 2} d W _ {2} (t) \Big),\tag{66}
$$

$$
d S _ {2} (t) = \mu_ {2} S _ {2} (t) d t + S _ {2} (t) \left(\sigma_ {2 1} d W _ {1} (t) + \sigma_ {2 2} d W _ {2} (t)\right).\tag{67}
$$

Written in matrix form $S = ( S _ { 1 } , S _ { 2 } ) ^ { T }$ , the same SDE is given as: 

$$
A (t) = \left( \begin{array}{c c} \mu_ {1} & 0 \\ 0 & \mu_ {1} \end{array} \right) a (t) = \binom{0}{0} B _ {1} (t) = \left( \begin{array}{c c} \sigma_ {1 1} & 0 \\ 0 & \sigma_ {2 1} \end{array} \right) B _ {2} (t) = \left( \begin{array}{c c} \sigma_ {1 2} & 0 \\ 0 & \sigma_ {2 2} \end{array} \right)
$$

Both processes $S _ { 1 } ( t )$ and $S _ { 2 } ( t )$ are correlated if $\sigma _ { 1 2 } = \sigma _ { 2 1 } \neq 0$ . This model can be easily extended to n processes. 

## Stochastic Diferential Equations (SDE)

The observed volatility for real existing price processes, such as stocks or bonds is itself a stochastic process. The following model describes this observation: 

$$
\begin{array}{r c l} {d P (t)} & = & {\mu d t + \sigma (t) d W _ {1} (t), P (0) = P _ {0},} \\ {d \sigma (t)} & = & {\kappa (\theta - \sigma (t)) d t + \sigma (t) \sigma_ {1} d W _ {2} (t), \sigma (0) = \sigma_ {0}.} \end{array}
$$

where $\theta$ is the average volatility, $\sigma _ { 1 }$ a volatility, and κ the mean reversion rate of the volatility process $\sigma ( t )$ . If this model is used for stock prices, the transformation $P ( t ) = \ln ( S ( t ) )$ is useful. The two Brownian motions $d W _ { 1 } ( t )$ and $d W _ { 2 } ( t )$ are correlated, hence corr $[ d W _ { 1 } ( t ) , d W _ { 2 } ( t ) ] = \rho$ . This model captures the behavior of real existing prices better and its distribution of returns shows “fatter tails”. 

## Stochastic Diferential Equations (SDE)

Die system (68) can be rewritten as linear SDE: 

$$
A (t) = \left( \begin{array}{c c} 0 & 0 \\ 0 & - \kappa \end{array} \right) a (t) = \binom{\mu}{\kappa \theta} B _ {1} (t) = \left( \begin{array}{c c} 0 & 1 \\ 0 & \sigma_ {1} \rho \end{array} \right)
$$

$$
B _ {2} (t) = \left( \begin{array}{c c} 0 & 0 \\ 0 & \sigma_ {1} \sqrt {1 - \rho^ {2}} \end{array} \right),
$$

wobei $x ( t ) = ( P ( t ) , \ \sigma ( t ) ) ^ { T }$ The system (68) has the property, that the variance of $P ( t )$ depends on the initial condition $\sigma _ { 0 }$ For the parameters $\mu = 0 . 1 , \kappa = 2$ $\theta = 0 . 2 , \sigma _ { 1 } = 0 . 5$ and $\rho = 0 . 5$ , we calculate the standard deviation of $P ( t )$ with $\sigma _ { 0 } ~ = ~ 0 . 1$ and alternatively with $\sigma _ { 0 } ~ = ~ 0 . 8$ . The expected value of $\sigma ( t )$ has the following evaluation over time $m ( t ) = \theta + ( \sigma _ { 0 } - \theta ) e ^ { - \kappa t }$ and thus the variance of $P ( t )$ depends on $\sigma _ { 0 }$ 

## Stochastic Diferential Equations (SDE)

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/b8900486-51b0-4310-b523-a538300c309a/3d82fad7fa0806dc384affed882a6582950ec7e68342a9c16d55e791edef3ed2.jpg)



Abbildung 1: Stand. dev. of $P ( t )$ for diferent initial conditions of $\sigma ( t )$


## Stochastic Diferential Equations (SDE)

In comparison with linear SDEs, nonlinear SDEs are less well understood. No general solution theory exists. And there are no explicit formulae for calculating the moments. In this section, we show some examples of nonlinear SDEs and their properties. 

In general, a scalar square root process can be written as 

$$
{ d X ( t ) } { = } { f ( t , X ( t ) ) d t + g ( t , X ( t ) ) d W ( t ) }
$$

with 

$$
{f (t, X (t))} = {A (t) X (t) + a (t)}
$$

$$
{g (t, X (t))} = {B (t) \sqrt {X (t)},}
$$

where $A ( t ) , a ( t )$ , and $B ( t )$ are real scalars. The nonlinear mean reverting SDEs difer from the linear scalar equations by their nonlinear difusion term. For this process, the distribution and moments can be calculated. 

## Stochastic Diferential Equations (SDE)

For a specific square root process with $A ( t ) = 0 , a ( t ) = 1$ and $B ( t ) = 2$ we are able to derive the analytical solution: The SDE 

$$
d X (t) = 1 d t + 2 \sqrt {X (t)} d W (t), X (0) = x _ {o},
$$

has the solution $X ( t ) = ( W ( t ) + x _ { 0 } ) ^ { 2 } \mathsf { W } \epsilon$ verify the solution using Itˆo formula. We use $\Phi ( t ) = X ( t ) = ( Y ( t ) + x _ { 0 } ) ^ { 2 }$ and $d Y ( t ) = d W ( t )$ . The partial derivatives are $\Phi _ { t } = 0 , \Phi _ { Y } = 2 ( Y ( t ) + x _ { 0 } )$ , and $\Phi _ { Y Y } = 2 $ . Thus 

$$
{d \Phi (t)} = {[ \Phi_ {t} + \Phi_ {Y} \cdot 0 + \frac {1}{2} \Phi_ {Y Y} \cdot 1 ] d t + \Phi_ {Y} \cdot 1 d W (t),}
$$

$$
{d \Phi (t)} = {1 d t + 2 (Y (t) + x _ {0}) d W (t), \Rightarrow d X (t) = 1 d t + 2 \sqrt {X (t)} d W (t),}
$$

since ${ \sqrt { X ( t ) } } = Y ( t ) + x _ { 0 }$ 

## Stochastic Diferential Equations (SDE)

Another widely used mean reversion model is obtained by 

$$
{ d S ( t ) } { = } { \kappa [ \mu - S ( t ) ] d t + \sigma \sqrt { S ( t ) } d W ( t ) , S ( 0 ) = S _ { 0 } . }\tag{68}
$$

This model is also known as the Cox-Ross-Ingersol processes.The process shows a less volatile behavior than its linear geometric counterpart and it has a non-central chi-square distribution. The process is often used to model short-term interest rates or stochastic volatility processes for stock prices. Another often used square root process is similar to the geometric Brownian motion, but with a square root difusion term instead of the linear difusion term. Its model is given by 

$$
d S (t) = \mu S (t) d t + \sigma \sqrt {S (t)} d W (t), S (0) = S _ {0}.\tag{69}
$$

# Stochastic Diferential Equations (SDE)

The expected value for (69) is $\mathsf E [ S ( t ) ] = S _ { 0 } e ^ { \mu t }$ and the variance is obtained by $\begin{array} { r } { \mathsf { V a r } [ S ( t ) ] = \frac { \sigma ^ { 2 } S _ { 0 } } { \mu } \Big ( e ^ { 2 \mu t } - e ^ { \mu t } \Big ) } \end{array}$ 

Another widely used mean reversion model is obtained by 

$$
d S (t) = \kappa S (t) [ \mu - \ln (S (t)) ] d t + S (t) \sigma d W (t).\tag{70}
$$

Using the transformation $P ( t ) = \ln ( S ( t ) )$ yields the linear mean reverting and normally distributed process $P ( t )$ 

$$
d P (t) = \kappa [ (\mu - \frac {\sigma^ {2}}{2 \kappa}) - P (t) ] d t + \sigma d W (t),\tag{71}
$$

Because of the transformation, $S ( t )$ is log-normally distributed. This model is used to model stock prices, stochastic volatilities, and electricity prices. Because $S ( t )$ is log-normally distributed, $S ( t )$ is always positive. 

## Stochastic Diferential Equations (SDE)

In this part, we introduce three major methods to compute solution of SDEs. 

• The first method is based on the Itˆo integral and has already been used for linear solutions. 

• We introduce numerical methods to compute path-wise solutions of SDEs. 

• The third method is based on partial diferential equations, where the problem of finding the probability density function of the solution is transformed into solving a partial diferential equation. 

## Stochastic Diferential Equations (SDE)

The stochastic process $X ( t )$ governed by the stochastic diferential equation 

$$
\begin{array}{r l r} {d X (t)} & = & {f (t, X (t)) d t + g (t, X (t)) d W (t)} \\ {X (0)} & = & {X _ {0}} \end{array}
$$

is explicitly described by the integral form 

$$
{X (t, \omega)} = {X _ {0} + \int_ {0} ^ {t} f (s, X (s)) d s + \int_ {0} ^ {t} g (s, X (s)) d W (s),}
$$

where the first integral is a path-wise Riemann integral and the second integral is an Itˆo integral. 

In this definition, it is assumed that the functions $f ( t , X ( t ) )$ and $g ( t , X ( t ) )$ are suficiently smooth in order to guarantee the existence of the solution $X ( t )$ 

# Stochastic Diferential Equations (SDE)

There are several ways of finding analytical solutions. One way is to guess a solution and use the Itˆo calculus to verify that it is a solution for the SDE under consideration. 

We assume that the following nonlinear SDE 

$$
d X (t) = d t + 2 \sqrt {X (t)} d W (t),
$$

has the solution 

$$
X (t) = (W (t) + \sqrt {X _ {0}}) ^ {2}.
$$

In order to verify this claim, we use the Itˆo calculus. We have $X ( t ) = \phi ( W )$ where $\phi ( W ) = ( W ( t ) + \sqrt { X _ { 0 } } ) ^ { 2 }$ , so that $\phi ^ { \prime } ( W ) = 2 ( W ( t ) + \sqrt { X _ { 0 } } )$ and $\phi ^ { \prime \prime } ( W ) = 2$ 

## Stochastic Diferential Equations (SDE)

Using Itˆo’s rule, we get 

$$
{ d X ( t ) } { = } { \widetilde { f } ( t , X ) d t + \widetilde { g } ( t , X ) d W ( t ) }
$$

$$
{\widetilde {f} (t, X)} = {\phi (W) ^ {\prime} 1 + \frac {1}{2} \phi^ {\prime \prime} (W) (2 \sqrt {X (t)}) ^ {2} = 1}
$$

$$
{\widetilde {g} (T, X)} = {\phi^ {\prime} (W) (2 \sqrt {X (t)}) = 2 (W (t) + \sqrt {X _ {0}}).}
$$

Since $X ( t ) = ( W ( t ) + \sqrt { X _ { 0 } } ) ^ { 2 }$ we know that $( W ( t ) + \sqrt { X _ { 0 } } ) = \sqrt { X ( t ) }$ and thus the Itˆo calculation generated the original SDE where we started at. 

## Stochastic Diferential Equations (SDE)

For some classes of SDEs, analytical formulas exist to find the solution, e.g. consider the following SDE: 

$$
d X (t) = f (t, X (t)) d t + \sigma (t) d W (t), X (0) = x _ {0}\tag{72}
$$

where $X ( t ) \in \mathbb { R } ^ { n } , \ f ( t , X ( t ) ) \ \in \ \mathbb { R } ^ { n }$ is an arbitrary function, $\sigma ( t ) \in \mathbb { R } ^ { n \times m }$ and $\boldsymbol { d W } ( t ) \in \mathbb { R } ^ { m }$ . This class of SDEs has the following general solution: 

$$
{ X ( t ) } { = } { Y ( t ) + F ( t ) }\tag{73}
$$

$$
{ d Y ( t ) } { = } { f ( t , Y ( t ) + F ( t ) ) d t , \ Y ( 0 ) = x _ { 0 } }\tag{74}
$$

$$
{ d F ( t ) } { = } { \sigma ( t ) d W ( t ) , } { F ( 0 ) = 0 . }\tag{75}
$$

The SDE for $F ( t )$ can be integrated, i.e. $\begin{array} { r } { F ( t ) = \int _ { 0 } ^ { t } \sigma ( s ) d W ( s ) } \end{array}$ . When $\sigma ( t ) = \sigma$ than $F ( t ) = \sigma W ( t )$ 

## Stochastic Diferential Equations (SDE)

Since $F ( t )$ is know,, we are able to solve for $Y ( t )$ in in function of $F ( t )$ Using Itˆo lemman, we show that $X ( t ) = Y ( t ) + F ( t )$ and this solves the SDE 

$$
\begin{array}{r c l} d X (t) & = & d Y (t) + d F (t) = f (t, Y (t) + F (t)) d t + \sigma (t) d W (t) \\ & = & f (t, X (t)) d t + \sigma (t) d W (t) \end{array}\tag{76}
$$

This solution is not very suprising, since $X ( t )$ is the sum of the process of $Y ( t )$ and the BM of $F ( t )$ 

## Stochastic Diferential Equations (SDE)

For another class of SDEs, exist an analytical formula for their solution: 

$$
d X (t) = f (t, X (t)) d t + c (t) X (t) d W (t), \quad X (0) = x _ {0},\tag{77}
$$

where $f ( t , X ( t ) ) \in \mathbb { R } , \ c ( t ) \in \mathbb { R }$ and $d W \in \mathbb { R }$ . DThe solution can be derived as follows: 

$$
X (t) = F ^ {- 1} (t) Y (t)\tag{78}
$$

$$
d F (t) = F (t) c ^ {2} (t) d t - F (t) c (t) d W (t), F (0) = 1\tag{79}
$$

$$
d Y (t) = F (t) f (t, F ^ {- 1} Y (t)) d t\tag{80}
$$

The proof is similar to the first case, sice the difusion is linear. 

## Stochastic Diferential Equations (SDE)

Calculate the analytical solution for 

$$
{ d X ( t ) } { = } { \frac { d t } { X ( t ) } + \alpha X ( t ) d W ( t ) , \; X ( 0 ) = x _ { 0 } . }
$$

$$
{ F ( t ) } { = } { e ^ { \frac { 1 } { 2 } \alpha ^ { 2 } t - \alpha W ( t ) } , d Y ( t ) = \frac { F ( t ) } { F ^ { - 1 } ( t ) Y } d t = \frac { F ^ { 2 } ( t ) } { Y } d t }
$$

$$
{d Y (t) Y (t)} = {F ^ {2} (t) d t, \frac {1}{2} Y ^ {2} (t) = \int_ {0} ^ {t} F ^ {2} (s) d s + C _ {0}}
$$

$$
{ Y ( t ) } { = } { \left( x _ { 0 } ^ { 2 } + 2 \int _ { 0 } ^ { t } e ^ { \alpha ^ { 2 } s - 2 \alpha W ( s ) } d s \right) ^ { \frac { 1 } { 2 } } }
$$

$$
{ X ( t ) } { = } { e ^ { - \frac { 1 } { 2 } \alpha ^ { 2 } t + \alpha W ( t ) } \Bigl ( x _ { 0 } ^ { 2 } + 2 \int _ { 0 } ^ { t } e ^ { \alpha ^ { 2 } s - 2 \alpha W ( s ) } d s \Bigr ) ^ { \frac { 1 } { 2 } } }
$$

## Stochastic Diferential Equations (SDE)

However, most SDEs, especially nonlinear SDEs, do not have analytical solutions so that one has to resort to numerical approximation schemes in order to simulate sample paths of solutions to the given equation. 

The simplest scheme is obtained by using a first-order approximation. This is called the Euler scheme 

$$
X (t _ {k}) = X (t _ {k - 1}) + f (t _ {k - 1}, X (t _ {k - 1})) \Delta t + g (t _ {k - 1}, X (t _ {k - 1})) \Delta W (t _ {k}).
$$

The Brownian motion term can be approximated as follows: 

$$
\Delta W (t _ {k}) = \epsilon (t _ {k}) \sqrt {\Delta t},
$$

where the $\epsilon ( . )$ is a discrete-time Gaussian white process with mean 0 and standard deviation 1. 