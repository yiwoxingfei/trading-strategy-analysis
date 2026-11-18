

<!-- === Source: MinerU_markdown_Introduction_to_Stochastic_Differential_Equations_for_Finance_1_2122706940055363599.md (Page 1) === -->

# Introduction to Stochastic Diferential Equations (SDEs) for Finance

Author: Andrew Papanicolaou ap1345@nyu.edu 

This work was partially supported by NSF grant DMS-0739195. 

## Contents

1 Financial Introduction 4
1.1 A Market in Discrete Time and Space . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
1.2 Equivalent Martingale Measure (EMM) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
1.3 Contingent Claims . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
1.4 Option Pricing Terminology . . . . . . . . . . . . . . . . . . . . . . . . 10
1.5 Completeness & Fundamental Theorems 10
2 Brownian Motion & Stochastic Calculus 12
2.1 Definition and Properties of Brownian Motion 12
2.2 The Itô Integral 14
2.3 Stochastic Differential Equations & Itô's Lemma 15
2.4 Multivariate Itô Lemma 19
2.5 The Feynman-Kac Formula 20
2.6 Girsanov Theorem 21
3 The Black-Scholes Theory 23
3.1 The Black-Scholes Model 23
3.2 Self-Financing Portfolio 24
3.3 The Black-Scholes Equation 25
3.4 Feynman-Kac, the EMM, & Heat Equations 25
3.5 The Black-Scholes Call Option Formula 27
3.6 Put-Call Parity and the Put Option Formula 30
3.7 Options on Futures and Stocks with Dividends 30
4 The Black-Scholes Greeks 34
4.1 The Delta Hedge 34
4.2 The Theta 35
4.3 The Gamma 38
4.4 The Vega 39
4.5 The Rho 41
4.6 Other Greeks 41 

5 Exotic Options 42
5.1 Asian Options . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 42
5.2 Exchange Options (Margrabe Formula) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 45
5.3 American Options and Optimality of Early Exercise 46
5.4 Bermuda Options 51
5.5 Free-Boundary Problem for the American Put 52
6 Implied Volatility & Local-Volatility Fits 54
6.1 Implied Volatility 54
6.2 Local Volatility Function 59
6.3 Fitting the Local Volatility Function 62
6.4 Surface Parameterizations 64
7 Stochastic Volatility 66
7.1 Hedging and Pricing 66
7.2 Monte Carlo Methods 71
7.3 Fourier Transform Methods 73
7.4 Call-Option Pricing 73
7.5 Heston Explicit Formula 76
7.6 The Merton Jump Diffusion 77
8 Stochastic Control 79
8.1 The Optimal Investment Problem 79
8.2 The Hamilton-Jacobi-Bellman (HJB) Equation 82
8.3 Merton's Optimal Investment Problem 83
8.4 Stochastic Returns 84
8.5 Stochastic Volatility 87
8.6 Indifference Pricing 89
Appendices 91
A Martingales and Stopping Times 93
A.1 Stopping Times 93
A.2 Local Martingales 94
B Some Notes on Fourier Transforms 96
B.1 Some Basic Properties 96
B.2 Regularity Strips 98
B.3 The Wave Equation 99
B.4 The Heat Equation 100
B.5 The Black-Scholes Equation 101 

## Chapter 1

## Financial Introduction

In this section we’ll discuss some of the basic ideas of option pricing. The main idea is replication, whereby a derivative security can be priced because it is shown to have the same cash flows as a portfolio of assets that already have a price-tag. Another word to describe such a notion of pricing is benchmarking, where to say that you’ve ‘benchmarked the security’ might mean that you’ve found a portfolio of other assets that do not replicate but have have some similarities to the derivative’s cash flows. 

The idea of finding a portfolio that is close in value to the derivative security is essentially the law of one price, which states that “In an eficient market, all identical goods must have only one price.” Indeed, we will assume that our markets are eficient, and in some cases we will assume that arbitrage has zero probability of occurring; these assumptions are routine and are generally not considered to be restrictive. 

The manner in which these notes can be considered ‘oversimplified’ is in the completeness of the resulting markets. In practice there are derivatives (e.g. insurance products) which cannot be hedged, and hence the market is incomplete. Both the discrete time-space market and the Black-Scholes market are simple enough for completeness to hold. In practice, reverse-engineering these models from real-life market data will require interpretation. 

## 1.1 A Market in Discrete Time and Space

Consider a very simple market where at time $t = 0$ it is known that there are only two possible states for the market at a later time $t = T$ . In between times $t = 0$ and $t = T$ there is no trading of any kind. This market is described by a probability space $\Omega = \{ \omega _ { 1 } , \omega _ { 2 } \}$ with probability measure P given by 

$$
p _ {1} = \mathbb {P} (\omega_ {1}) = \frac {2}{3}, \qquad p _ {2} = \mathbb {P} (\omega_ {2}) = \frac {1}{3}.
$$

The elementary events $\omega _ { 1 }$ and $\omega _ { 2 }$ are the two states of the market. The traded assets in this simple market are a bank account, a stock, and and a call option on the stock with exercise at $T$ and strike $K = 2 .$ . The market outcomes are shown in Table 1.1. 


Table 1.1: Assets in the Discrete Time-Space Market


<table><tr><td>time</td><td>t=0</td><td>t=T</td></tr><tr><td>bank account</td><td><eq>B_0 = 1</eq></td><td><eq>B_T = 1</eq> (interest rate <eq>r = 0</eq>)</td></tr><tr><td>stock</td><td><eq>S_0 = 2</eq></td><td><eq>S_T = \left\{ \begin{array}{ll} 3 &amp; \text{in } \omega_1 \\ 1 &amp; \text{in } \omega_2 \end{array} \right.</eq></td></tr><tr><td>call option, <eq>K = 2</eq></td><td><eq>C_0 = ?</eq></td><td><eq>C_T = \left\{ \begin{array}{ll} 1 &amp; \text{in } \omega_1 \\ 0 &amp; \text{in } \omega_2 \end{array} \right.</eq></td></tr></table>

The way to determine the price of the call option, $C _ { 0 }$ , is to replicate it with a portfolio of the stock and the bank account. Let $V _ { t }$ denote the value of such a portfolio at time $t ,$ so that, 

$$
\begin{array}{r c l} {V _ {0}} & = & {\alpha S _ {0} + \beta} \\ {V _ {T}} & = & {\alpha S _ {T} + \beta ,} \end{array}
$$

where α is $\#$ of shares and $\beta$ is $ in bank. The portfolio $V _ { t }$ will replicate the call option if we solve for $\alpha$ and $\beta$ so that $V _ { T } = C _ { T }$ for both $\omega _ { 1 }$ and $\omega _ { 2 }$ 

$$
\begin{array}{l} {3 \alpha + \beta = \alpha S _ {T} (\omega_ {1}) + \beta = C _ {T} (\omega_ {1}) = 1} \\ {\alpha + \beta = \alpha S _ {T} (\omega_ {1}) + \beta = C _ {T} (\omega_ {2}) = 0.} \end{array}
$$

This system has solution $\alpha = { \textstyle { \frac { 1 } { 2 } } } , \beta = - { \textstyle { \frac { 1 } { 2 } } }$ . Hence, by the law of one price, it must be that, 

$$
C _ {0} = V _ {0} = \frac {1}{2} S _ {0} - \frac {1}{2} = \frac {1}{2}.
$$

If $C _ { 0 } \neq V _ { 0 }$ , then there would be an arbitrage opportunity in the market. Arbitrage in a financial models means it is possible to purchase a portfolio for which there is a risk-less profit to be earned with positive probability. If such an opportunity is spotted then an investor could borrow an infinite amount of money and buy the arbitrage portfolio, giving him/her an infinite amount of wealth. Arbitrage (in this sense) does not make for a sound financial model, and in real life it is known that true arbitrage opportunities disappear very quickly by the eficiency of the markets. Therefore, almost every financial model assumes absolute eficiency of the market and ‘no-arbitrage’. There is also the concept of ‘No Free Lunch’, but in discrete time-space we do not have to worry about theses diferences. 

The notion of ‘no-arbitrage’ is defined as follows: 

Definition 1.1.1. Let wea $l t h _ { t }$ denote the wealth of an investor at time t. We say that the market has arbitrage if, 

$$
\begin{array}{l l} & \mathbb {P} (w e a l t h _ {T} > 0 | w e a l t h _ {0} = 0) > 0 \\ a n d & \mathbb {P} (w e a l t h _ {T} <   0 | w e a l t h _ {0} = 0) = 0 , \end{array}
$$

i.e. there is positive probability of a gain and zero probability of a loss. 

In our discrete time-space market, if $C _ { 0 } < V _ { 0 }$ then the arbitrage portfolio is one that buys the option, shorts the portfolio, and invest the diference in the bank. The risk-less payof of this portfolio is shown in Table 1.2. 


Table 1.2: Arbitrage Opportunity if Option Mispriced


<table><tr><td></td><td>t=0</td><td>t=T</td></tr><tr><td>buy option</td><td>-C0</td><td>max{ST-2,0}</td></tr><tr><td>sell portfolio</td><td>V0</td><td>-max{ST-2,0}</td></tr><tr><td>net:</td><td>V0-C0&gt;0</td><td>0</td></tr></table>

## 1.2 Equivalent Martingale Measure (EMM)

A common method for pricing an asset is to use a risk-neutral or an equivalent martingale measure (EMM). The EMM is convenient because all asset prices are simply an expectation of the payof.Two important questions are: what is the EMM? Is there more one? 

Definition 1.2.1. The probability measure $\mathbb { Q }$ is an EMM of P if $S _ { t }$ is a $\mathbb { Q } \mathrm { . }$ -martingale, that is 

$$
\mathbb {E} ^ {Q} S _ {T} = S _ {0}
$$

and $\mathbb { Q }$ is equivalent to $\mathbb { P } ,$ 

$$
\mathbb {P} (\omega) > 0 \Leftrightarrow \mathbb {Q} (\omega) > 0
$$

for all elementary events $\omega \in \Omega \ ( i t ^ { \prime } s$ more complicated when Ω is not made up of elementary events, but it’s basically the same idea). 

For our discrete time-space example market, we have 

• Under the original measure 

$$
\mathbb {E} S _ {T} = p _ {1} S _ {T} (\omega_ {1}) + p _ {2} S _ {T} (\omega_ {2}) = \frac {2}{3} 3 + \frac {1}{3} 1 = \frac {7}{3} > 2 = S _ {0}
$$

• Under an EMM $\mathbb { Q } ( \omega _ { 1 } ) = q _ { 1 }$ and $\mathbb { Q } ( \omega _ { 2 } ) = q _ { 2 }$ 2 

$$
\mathbb {E} ^ {Q} S _ {T} = q _ {1} 3 + (1 - q _ {1}) 1 = 2 = S _ {0}.
$$

Solution is $\begin{array} { r } { q _ { 1 } = \frac { 1 } { 2 } } \end{array}$ and $\begin{array} { r } { q _ { 2 } = 1 - q _ { 1 } = \frac { 1 } { 2 } } \end{array}$ 

Given the EMM, a replicable option is easily priced: 

$$
\mathbb {E} ^ {Q} C _ {T} = \mathbb {E} ^ {Q} V _ {T} = \mathbb {E} ^ {Q} [ \alpha S _ {T} + \beta ] = \alpha \mathbb {E} ^ {Q} S _ {T} + \beta = \alpha S _ {0} + \beta = V _ {0} = C _ {0},
$$

and so $C _ { 0 } = \mathbb { E } ^ { Q } \operatorname* { m a x } ( S _ { T } - K , 2 )$ 

## 1.3 Contingent Claims

A corporation is interested in purchasing a derivative product to provide specific cashflows for each of the elementary events that (they believe) the market can take. Let $\Omega = \{ \omega _ { 1 } , \omega _ { 2 } , \ldots , \omega _ { N } \}$ be these elementary events that can occur at time $t = T$ , and let the proposed derivative security be a function $C _ { t } ( \omega )$ such that, 

$$
C _ {T} (\omega_ {i}) = c _ {i} \quad \forall i \leq N,
$$

where each $c _ { i }$ is the corporations desired cash flow. The derivative product C is a contingent claim, because it pays a fixed amount for all events in the market. Below are some general examples of contingent claims: 

Example 1.3.1. European Call Option. At time T the holder of the option has the right to buy an asset at a pre-determined strike price K. This is a contingent claim that pays, 

$$
(S _ {T} (\omega) - K) ^ {+} = \max (S _ {T} (\omega) - K, 0),
$$

where $S _ { T }$ is some risk asset (e.g. a stock or bond). The payof on this call option is seen in Figure 1.1. 

Example 1.3.2. European Put Option. At time T the holder of the option has the right to sell an asset at a pre-determined strike price K. This is a contingent claim that pays, 

$$
(K - S _ {T} (\omega)) ^ {+} = \max (K - S _ {T} (\omega), 0).
$$

Figure 1.2 shows the payof for the put. 

Example 1.3.3. American Call/Put Option. At any time $t \leq T$ the holder of the option has the right to buy/sell an asset at a pre-determined strike price K. Exercise of this claim at time $t \leq T$ is contingent on the event $\mathcal { A } _ { t } = \{ \omega _ { i } \}$ it is optimal to exercise at time $t \}$ 

Example 1.3.4. Bermuda Call/Put Option. At either time $T / 2$ or time T, the holder of the option has the right to buy/sell an asset at a pre-determined strike price K. Similar to an American option except only one early strike time. 

Example 1.3.5. Asian Call Option. At time T the holder of the option has the right to buy the averaged asset at a pre-determined strike price $K$ 

$$
\left(\frac {1}{M} \sum_ {\ell = 1} ^ {M} S _ {t _ {\ell}} (\omega) - K\right) ^ {+},
$$

where $\begin{array} { r } { t _ { \ell } = \ell \frac { T } { M } } \end{array}$ for integer $M > 0$ 

Example 1.3.6. Exchange Option. At time T the holder of the option has the right to buy one asset at the price of another, 

$$
(S _ {T} ^ {1} (\omega) - S _ {T} ^ {2} (\omega)) ^ {+},
$$

where $S _ { t } ^ { 1 }$ is the price of an asset and $S _ { t } ^ { 2 }$ is the price of another. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/f2afe0d711bd5d46aea33b58a9113db5919856fb36f412c88619c9008ff370c3.jpg)



Figure 1.1: The payof on a European call option with strike $K = 5 0$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/9a135700fb52b74bddddbda6e9785cf1c08536f4ae4649cea6490b55ae7fa61e.jpg)



Figure 1.2: The payof on a European put option with strike $K = 5 0$


## 1.4 Option Pricing Terminology

The following is a list of terms commonly used in option pricing: 

• Long position, a portfolio is ‘long asset X’ if it has net positive holdings of contracts in asset X. 

• Short position, a portfolio is ‘short asset X’ if it has net negative holdings of contracts in asset X (i.e. has short sales of contracts). 

• Hedge, or ‘hedging portfolio’ is a portfolio that has minimal or possibly a floor on the losses it might obtain. 

• In-the-money (ITM), a derivative contract that would have positive payof if settlement based on today’s market prices (e.g. a call option with very low strike). 

• Out-of-the-money (OTM), a derivative contract that would be worthless if settlement based on today’s market prices (e.g. a call option with very high strike). 

• At-the-money (ATM), a derivative contract exactly at it’s breaking point between ITM and OTM. 

• Far-from-the-money, a derivative contract with very little chance of finishing ITM. 

• Underlying, the stock, bond, ETF, exchange rate, etc. on which a derivative contract is written. 

• Strike, The price upon which a call or put option is settled. 

• Maturity, the latest time at which a derivative contract can be settled. 

• Exercise, the event that the long party decides to use a derivative’s embedded option (e.g. using a call option to buy a share of stock at lower than market value). 

## 1.5 Completeness & Fundamental Theorems

The nice thing about the discrete time-space market is that any contingent claim can be replicated. In general, for $\Omega = \{ \omega _ { 1 } , \omega _ { 2 } , \dots , \omega _ { N } \}$ , and with N−1 risky-assets $( S ^ { 1 } , S ^ { 2 } , \dots , S ^ { N - 1 } )$ and a risk-free bank account (with $r = 0 )$ , replicating portfolio weights the contingent claim C can be found by solving, 

$$
\left( \begin{array}{c c c c c} 1 & S _ {T} ^ {1} (\omega_ {1}) & \ldots & \ldots & S _ {T} ^ {N - 1} (\omega_ {1}) \\ 1 & S _ {T} ^ {1} (\omega_ {2}) & \ldots & \ldots & S _ {T} ^ {N - 1} (\omega_ {2}) \\ \vdots & \vdots & \ddots & & \vdots \\ \vdots & \vdots & & \ddots & \vdots \\ 1 & S _ {T} ^ {1} (\omega_ {N}) & \ldots & \ldots & S _ {T} ^ {N - 1} (\omega_ {N}) \end{array} \right) \left( \begin{array}{c} \beta \\ \alpha_ {1} \\ \vdots \\ \vdots \\ \alpha_ {N - 1} \end{array} \right) = \left( \begin{array}{c} c _ {1} \\ c _ {2} \\ \vdots \\ \vdots \\ c _ {N} \end{array} \right)  ,
$$

which has a solution $( \beta , \alpha _ { 1 } , \ldots , \alpha _ { N - 1 } )$ provided that none of these assets are redundant (e.g., there does not exist a portfolio consisting of the first N − 2 assets and the banks account that replicated the $\bar { S } _ { T } ^ { N - 1 } )$ . This N-dimensional extension of the discrete timespace market serves to further exemplify the importance of replication in asset pricing, and should help to make clear the intentions of the following definition and theorems: 

Definition 1.5.1. A contingent claim is reachable if there is a hedging portfolio V such the $V _ { T } ( \omega ) = C ( \omega )$ for all ω, in which case we say that C can be replicated. If all contingent claims can be replicated, then we say the market is complete. 

Theorem 1.5.1. The 1st fundamental theorem of asset pricing states the market is arbitrage-free if and only if there exists an EMM. 

Theorem 1.5.2. The 2nd fundamental theorem of asset pricing states the market is arbitrage-free and complete if and only if there exists a unique EMM. 

One of the early works that proves these theorems is [Harrison and Pliska, 1981]. Another good article on the subject is [Schachermayer, 1992]. In summary, these fundamental theorems mean that derivative prices are the expectation under an EMM. 

# Brownian Motion & Stochastic Calculus

Continuous time financial models will often use Brownian motion to model the trajectory of asset prices. One can typically open the finance section of a newspaper and see a time series plot of an asset’s price history, and it might be possible that the daily movements of the asset resemble a random walk or a path taken by a Brownian motion. Such a connection between asset prices and Brownian motion was central to the formulas of [Black and Scholes, 1973] and [Merton, 1973], and have since led to a variety of models for pricing and hedging. The study of Brownian motion can be intense, but the main ideas are a simple definition and the application of Itˆo’s lemma. For further reading, see [Bj¨ork, 2000, Øksendal, 2003]. 

## 2.1 Definition and Properties of Brownian Motion

On the time interval [0, T], Brownian motion is a continuous stochastic process $( W _ { t } ) _ { t \leq T }$ such that 

1. $W _ { 0 } = 0 ,$ 

2. Independent Increments: for $0 \leq s ^ { \prime } < t ^ { \prime } \leq s < t \leq T , W _ { t } - W _ { s }$ is independent of $W _ { t ^ { \prime } } - W _ { s ^ { \prime } }$ 2 

3. Conditionally Gaussian: $W _ { t } - W _ { s } \sim { \mathcal { N } } ( 0 , t - s )$ , i.e. is normal with mean zero and variance $t - s$ 

There is a vast study of Brownian motion. We will instead use Brownian motion rather simply; the only other fact that is somewhat important is that Brownian motion is nowhere 

diferentiable, that is 

$$
\mathbb {P} \left(\frac {d}{d t} W _ {t} \text {   is   undefined   for   almost - everywhere   } t \in [ 0, T ]\right) = 1 ,
$$

although sometimes people write $\dot { W _ { t } }$ to denote a white noise process. It should also be pointed out that $W _ { t }$ is a martingale, 

$$
\mathbb {E} [ W _ {t} | (W _ {\tau}) _ {\tau \leq s} ] = W _ {s} \quad \forall s \leq t.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/b0993f3e33411abd73e2312fe75dac4dc5191c46075dd69222aec053763a9085.jpg)



Figure 2.1: A sample of 10 independent Brownian motions.


Simulation. There are any number of ways to simulate Brownian motion, but to understand why Brownian motion can be treated like a ‘random walk’, consider the process, 

$$
W _ {t _ {n}} ^ {N} = W _ {t _ {n - 1}} ^ {N} + \left\{ \begin{array}{c l} \sqrt {T / N} & \text { with   probability } 1 / 2 \\ - \sqrt {T / N} & \text { with   probability } 1 / 2 \end{array} \right.
$$

with $W _ { t _ { 0 } } = 0$ and $\begin{array} { r } { t _ { n } = n \frac { T } { N } } \end{array}$ for $n = 0 , 1 , 2 \ldots , N$ . Obviously $W _ { t _ { n } } ^ { N }$ has independent increments, and conditionally has the same mean and variance as Brownian motion. However it’s not conditional Gaussian. However, as $N \to \infty$ the probability law of $W _ { t _ { n } } ^ { N }$ converges to the probability law of Brownian motion, so this simple random walk is actually a good way to simulate Brownian motion if you take N large. However, one usually has a random number generator that can produce $W _ { t _ { n } } ^ { N }$ that also has conditionally Gaussian increments, and so it probably better to simulate Brownian motion this way. A sample of 10 independent Brownian Motions simulations are shown in Figure 2.1. 

## 2.2 The Itˆo Integral

Introductory calculus courses teach diferentiation first and integration second, which makes sense because diferentiation is generally a methodical procedure $( \mathrm { e . g . }$ , you use the chain rule) whereas finding an anti-derivative requires all kinds of change-of-variables, trigsubstitutions, and guess-work. The Itˆo calculus is derived and taught in the reverse order: first we need to understand the definition of an Itˆo (stochastic) integral, and then we can understand what it means for a stochastic process to have a diferential. 

The construction of the Itˆo integral begins with a backward Riemann sum. For some function $f : [ 0 , T ] \to \mathbb { R }$ (possibly random), non-anticipative of W, the Itˆo integral is defined as 

$$
\int_ {0} ^ {T} f (t) d W _ {t} = \lim _ {N \to 0} \sum_ {n = 0} ^ {N - 1} f (t _ {n}) (W _ {t _ {n + 1}} - W _ {t _ {n}}),\tag{2.1}
$$

where $\begin{array} { r } { t _ { n } = n \frac { T } { N } } \end{array}$ , with the limit holding in the strong sense. If E $\begin{array} { r } { \int _ { 0 } ^ { T } f ^ { 2 } ( t ) d t < \infty } \end{array}$ , then through an application of Fubini’s theorem, it can be shown that equation (2.1) is a martingale, 

$$
\mathbb {E} \left[ \int_ {0} ^ {T} f (t) d W _ {t} \Big | (W _ {\tau}) _ {\tau \leq s} \right] = \int_ {0} ^ {s} f (t) d W _ {t} \quad \forall s \leq T.
$$

Another important property of the stochastic integral is the Itˆo Isometry, 

Proposition 2.2.1. (Itˆo Isometry). For any functions $f , g$ (possibly random), nonanticipative of W, with E $\begin{array} { r } { \int _ { 0 } ^ { T } f ^ { 2 } ( t ) d t < \infty } \end{array}$ and E $\begin{array} { r } { \int _ { 0 } ^ { T } g ^ { 2 } ( t ) d t < \infty } \end{array}$ , then 

$$
\mathbb {E} \left(\int_ {0} ^ {T} f (t) d W _ {t}\right) \left(\int_ {0} ^ {T} g (t) d W _ {t}\right) = \mathbb {E} \int_ {0} ^ {T} f (t) g (t) d t.
$$

Some facts about the Itˆo integral: 

• One can look at Equation (2.1) and think about the stochastic integral as a sum of independent normal random variables with mean zero and variance $T / N$ 2 

$$
\sum_ {n = 0} ^ {N - 1} f (t _ {n}) \left(W _ {t _ {n + 1}} - W _ {t _ {n}}\right) \sim \mathcal {N} \left(0, \frac {T}{N} \sum f ^ {2} (t _ {n})\right).
$$

Therefore, one might suspect that $\begin{array} { r } { \int _ { 0 } ^ { T } f ( t ) d W _ { t } } \end{array}$ is normal distributed. 

• In fact, the Itˆo integral is normally distributed when f is a non-stochastic function, and its variance is given by te Itˆo isometry, 

$$
\int_ {0} ^ {T} f (t) d W _ {t} \sim \mathcal {N} \left(0, \int_ {0} ^ {T} f ^ {2} (t) d t\right).
$$

• The Itˆo integral is also defined for functions of another random variable. For instance, $f : \mathbb { R } \to \mathbb { R }$ and another random variable $X _ { t } ,$ the Itˆo integral is, 

$$
\int_ {0} ^ {T} f (X _ {t}) d W _ {t} = \lim _ {N \to \infty} \sum_ {n = 0} ^ {N - 1} f (X _ {t _ {n}}) (W _ {t _ {n + 1}} - W _ {t _ {n}}).
$$

The Itˆo isometry for this integral is, 

$$
\mathbb {E} \left(\int_ {0} ^ {T} f (X _ {t}) d W _ {t}\right) ^ {2} = \int_ {0} ^ {T} \mathbb {E} f ^ {2} (X _ {t}) d t,
$$

provided that X is non-anticipative of W. 

## 2.3 Stochastic Diferential Equations & Itˆo’s Lemma

With the stochastic integral defined, we can now start talking about diferentials. In applications the stochastic diferential is how we think about random process that evolve over time. For instance, the return on a portfolio or the evolution of a bond yield. The idea is not that various physical phenomena are Brownian motion, but that they are driven by a Brownian motion. 

Instead of a diferential equation, the integrands in Itˆo integrals satisfy stochastic differential equations (SDEs). For instance, 

$$
\begin{array}{r l} & {d S _ {t} = \mu S _ {t} d t + \sigma S _ {t} d W _ {t}} \\ & {d Y _ {t} = \kappa (\theta - Y _ {t}) d t + \gamma d W _ {t}} \\ & {d X _ {t} = a (X _ {t}) d t + b (X _ {t}) d W _ {t}} \end{array}
$$

geometric Brownian motion, 

an Ornstein-Uhlenbeck process, 

a general SDE. 

Essentially, the formulation of an SDE tells us the Itˆo integral representation. For instance, 

$$
d X _ {t} = a (X _ {t}) d t + b (X _ {t}) d W _ {t} \quad \Leftrightarrow \quad X _ {t} = X _ {0} + \int_ {0} ^ {t} a (X _ {s}) d s + \int_ {0} ^ {t} b (X _ {s}) d W _ {s}.
$$

Hence, any SDE that has no dt-terms is a martingale. For instance, if $d S _ { t } = r S _ { t } d t + \sigma S _ { t } d W _ { t }$ then $F _ { t } = e ^ { - r t } S _ { t }$ satisfies the SDE $d F _ { t } = \sigma F _ { t } d W _ { t }$ and is therefore a martingale. 

On any given day, mathematicians, physicists, and practitioners may or may not recall the conditions on functions a and b that provide a sound mathematical framework, but the safest thing to do is to work with coeficients that are known to provide existence and uniqueness of solutions to the SDE (see page 68 of [Øksendal, 2003]). 

Theorem 2.3.1. (Conditions for Existence and Uniqueness of Solutions to SDEs). For $0 < T < \infty$ , let $t \in [ 0 , T ]$ and consider the SDE 

$$
d X _ {t} = a (t, X _ {t}) d t + b (t, X _ {t}) d W _ {t},
$$

with initial condition $X _ { 0 } = x$ (x constant). Suficient conditions for existence and uniqueness of square-integrable solutions to this SDE (i.e. solutions such that E $\begin{array} { r } { \int _ { 0 } ^ { T } | X _ { t } | ^ { 2 } d t < \infty ) } \end{array}$ are linear growth 

$$
| a (t, x) | + | b (t, x) | \leq C (1 + | x |) \quad \forall x \in \mathbb {R} a n d \forall t \in [ 0, T ]
$$

for some finite constant $C > 0$ , and Lipschitz continuity 

$$
| a (t, x) - a (t, y) | + | b (t, x) - b (t, y) | \leq D | x - y | \quad \forall x, y \in \mathbb {R} a n d \forall t \in [ 0, T ]
$$

where $0 < D < \infty$ is the Lipschitz constant. 

From the statement of Theorem 2.3.1 it should be clear that these are not necessary conditions. For instance, the widely used square-root process 

$$
d X _ {t} = \kappa (\bar {X} - X _ {t}) d t + \gamma \sqrt {X _ {t}} d W _ {t}
$$

does not satisfy linear growth or Lipschitz continuity for x near zero, but there does exist a unique solution if $\gamma ^ { 2 } \leq 2 \bar { X } \kappa$ . In general, existence of solutions for SDEs not covered by Theorem 2.3.1 needs to be evaluated on a case-by-case basis. The rule of thumb is to stay within the bounds of the theorem, and only work with SDEs outside if you are certain that the solution exists (and is unique). 

Example 2.3.1 (Tanaka Equation). The canonical example to demonstrate non-uniqueness for non-Lipschitz coeficients is the Tanaka equation, 

$$
d X _ {t} = s g n (X _ {t}) d W _ {t},
$$

with $X _ { 0 } = 0$ , where $s g n ( x )$ is the sign function; $s g n ( x ) = 1 \ i f x > 0 , s g n ( x ) = - 1 \ i f x < 0$ and $s g n ( x ) = 0 \ i f \ x = 0$ . Consider another Brownian motion $\hat { W } _ { t }$ and define 

$$
\widetilde {W} _ {t} = \int_ {0} ^ {t} s g n (\hat {W} _ {s}) d \hat {W} _ {s},
$$

where it can be checked that $\widetilde { W _ { t } }$ is also a Brownian motion. We can also write 

$$
d \hat {W} _ {t} = s g n (\hat {W} _ {t}) d \widetilde {W} _ {t},
$$

which shows that $X _ { t } = \hat { W } _ { t }$ is a solution to the Tanaka equation. However, this is referred to as a weak solution, meaning that the driving Brownian motion was recovered after the solution X was given; a strong solution is a solution obtained when first the Brownian motion is given. Notice this weak solution is non-unique: take $Y _ { t } = - X _ { t }$ and look at the diferential, 

$$
d Y _ {t} = - d X _ {t} = - s g n (X _ {t}) d \widetilde {W} _ {t} = s g n (Y _ {t}) d \widetilde {W} _ {t}.
$$

Notice that $X _ { t } \equiv 0$ is also a solution. 

Given a stochastic diferential equation, Itˆo’s lemma tells us the diferential of any function on that process. Itˆo’s lemma can be thought of as the stochastic analogue to diferentiation, and is a fundamental tool in stochastic diferential equations: 

Lemma 2.3.1. (Itˆo’s Lemma). Consider the process $X _ { t }$ with SDE $d X _ { t } = a ( X _ { t } ) d t +$ $b ( X _ { t } ) d W _ { t }$ . For a function $f ( t , x )$ with at least one derivative in t and at least two derivatives in x, we have 

$$
d f (t, X _ {t}) = \left(\frac {\partial}{\partial t} + a (X _ {t}) \frac {\partial}{\partial x} + \frac {b ^ {2} (X _ {t})}{2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) f (t, X _ {t}) d t + b (X _ {t}) \frac {\partial}{\partial x} f (t, X _ {t}) d W _ {t}.\tag{2.2}
$$

Details on the Itˆo Lemma. The proof of (2.2) is fairly involved and has several details to check, but ultimately, Itˆo’s lemma is a Taylor expansion to the 2nd order term, e.g. 

$$
f (W _ {t}) \simeq f (W _ {t _ {0}}) + f ^ {\prime} (W _ {t _ {0}}) (W _ {t} - W _ {t _ {0}}) + \frac {1}{2} f ^ {\prime \prime} (W _ {t _ {0}}) (W _ {t} - W _ {t _ {0}}) ^ {2}
$$

for $0 < t - t _ { 0 } \ll 1$ , (i.e. t just slightly greater than $t _ { 0 } )$ . To get a sense of why higher order terms drop out, take $t _ { 0 } = 0$ and $t _ { n } = n t / N$ for some large $N _ { ; }$ , and use the Taylor expansion: 

$$
\begin{array}{r l} & f (W _ {t}) - f (W _ {0}) = \sum_ {n = 0} ^ {N - 1} f ^ {\prime} (W _ {t _ {n}}) (W _ {t _ {n + 1}} - W _ {t _ {n}}) + \frac {1}{2} \sum_ {n = 0} ^ {N - 1} f ^ {\prime \prime} (W _ {t _ {n}}) (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {2} \\ & \qquad + \frac {1}{6} \sum_ {n = 0} ^ {N - 1} f ^ {\prime \prime \prime} (W _ {t _ {n}}) (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {3} + \frac {1}{2 4} \sum_ {n = 0} ^ {N - 1} f ^ {\prime \prime \prime \prime} (\xi_ {n}) (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {4}, \end{array}
$$

where $\xi _ { n }$ is some (random) intermediate point to make the expansion exact. Now we use independent increments and the fact that 

$$
\mathbb {E} (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {k} = \left\{ \begin{array}{c l} \big (\frac {t}{N} \big) ^ {k / 2} (k - 1)!! & \text {if k even} \\ 0 & \text {if k odd}, \end{array} \right.
$$

from which is can be seem that the $f ^ { \prime }$ and $f ^ { \prime \prime }$ are are significant, 

$$
\mathbb {E} \left(\sum_ {n = 0} ^ {N - 1} f ^ {\prime} (W _ {t _ {n}}) (W _ {t _ {n + 1}} - W _ {t _ {n}})\right) ^ {2} = \frac {t}{N} \sum_ {n = 0} ^ {N - 1} \mathbb {E} | f ^ {\prime} (W _ {t _ {n}}) | ^ {2} = \mathcal {O} (1),
$$

$$
\mathbb {E} \sum_ {n = 0} ^ {N - 1} f ^ {\prime \prime} (W _ {t _ {n}}) (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {2} = \frac {t}{N} \sum_ {n = 0} ^ {N - 1} \mathbb {E} f ^ {\prime \prime} (W _ {t _ {n}}) = \mathcal {O} (1),
$$

and assuming there is some bound $M < \infty$ such that $| f ^ { \prime \prime \prime } | \le M$ and $| f ^ { \prime \prime \prime \prime } | \leq M$ , we see that the higher order terms are arbitrarily small, 

$$
\begin{array}{r l} & {\mathbb {E} \left| \sum_ {n = 0} ^ {N - 1} f ^ {\prime \prime \prime} (W _ {t _ {n}}) (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {3} \right| \leq M \sum_ {n = 0} ^ {N - 1} \mathbb {E} \left| W _ {t _ {n + 1}} - W _ {t _ {n}} \right| ^ {3}} \\ & {\qquad \leq M \sum_ {n = 0} ^ {N - 1} \sqrt {\mathbb {E} \left| W _ {t _ {n + 1}} - W _ {t _ {n}} \right| ^ {6}} = \mathcal {O} \left(\frac {1}{N ^ {1 / 2}}\right),} \\ & {\mathbb {E} \left| \sum_ {n = 0} ^ {N - 1} f ^ {\prime \prime \prime \prime} (\xi_ {n}) (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {4} \right| \leq M \sum_ {n = 0} ^ {N - 1} \mathbb {E} (W _ {t _ {n + 1}} - W _ {t _ {n}}) ^ {4} = \mathcal {O} \left(\frac {1}{N}\right),} \end{array}
$$

where we’ve used the Cauchy-Schwartz inequality, $\mathbb { E } | Z | ^ { 3 } \le \sqrt { \mathbb { E } | Z | ^ { 6 } }$ for some randomvariable $Z .$ 

The following are examples that should help to familiarize with the Itˆo lemma and solutions to SDEs: 

Example 2.3.2. An Ornstein-Uhlenbeck process $d X _ { t } = \kappa ( \theta - X _ { t } ) d t + \gamma d W _ { t }$ has solution 

$$
X _ {t} = \theta + (X _ {0} - \theta) e ^ {- \kappa t} + \gamma \int_ {0} ^ {t} e ^ {- \kappa (t - s)} d W _ {s}.
$$

This solution uses an integrating factor<sup>1</sup> of $e ^ { \kappa t }$ , 

$$
d X _ {t} + \kappa X _ {t} d t = \kappa \theta d t + \gamma d W _ {t}.
$$

Example 2.3.3. Apply Itˆo’s lemma to $X _ { t } = W _ { t } ^ { 2 }$ to get the SDE 

$$
d X _ {t} = d t + 2 W _ {t} d W _ {t}.
$$

Example 2.3.4. The canonical SDE in financial math, the geometric Brownian motion, $\begin{array} { r } { \frac { d S _ { t } } { S _ { t } } = \mu d t + \sigma d W _ { t } } \end{array}$ has solution 

$$
S _ {t} = S _ {0} e ^ {\left(\mu - \frac {1}{2} \sigma^ {2}\right) t + \sigma W _ {t}}
$$

which is always positive. Again, verify with Itˆo’s lemma. Also try Itˆo’s lemma on $\log ( S _ { t } )$ 

Example 2.3.5. Suppose $d Y _ { t } = ( \sigma ^ { 2 } Y _ { t } ^ { 3 } - a Y _ { t } ) d t + \sigma Y _ { t } ^ { 2 } d W _ { t }$ . Apply Itˆo’s lemma to $X _ { t } =$ $- 1 / Y _ { t }$ to get a simpler SDE for $X _ { t } ,$ 

$$
d X _ {t} = - a X _ {t} d t + \sigma d W _ {t}.
$$

Notice that $Y _ { t }$ ’s SDE doesn’t satisfy the criterion of Theorem 2.3.1, but though the change of variables we see that $Y _ { t }$ is really a function of $X _ { t }$ that is covered by the theorem. 

## 2.4 Multivariate Itˆo Lemma

Let $W _ { t } = ( W _ { t } ^ { 1 } , W _ { t } ^ { 2 } , \dots , W _ { t } ^ { n } )$ be an n-dimensional Brownian motion such that $\begin{array} { r } { \frac { 1 } { t } \mathbb { E } W _ { t } ^ { i } W _ { j } ^ { j } = } \end{array}$ $\mathbb { 1 } _ { [ i = j ] }$ . Now suppose that we also have a system of SDEs, $X _ { t } = ( X _ { t } ^ { 1 } , X _ { t } ^ { 2 } , \ldots , X _ { t } ^ { m } )$ (with m possibly not equal to n) such that 

$$
d X _ {t} ^ {i} = a _ {i} (X _ {t}) d t + \sum_ {j = 1} ^ {n} b _ {i j} (X _ {t}) d W _ {t} ^ {j} \quad \text { for   each } i \leq m
$$

where $\alpha _ { i } : \mathbb { R } ^ { m }  \mathbb { R }$ are the drift coeficients, and the difusion coeficients $b _ { i j } : \mathbb { R } ^ { m }  \mathbb { R }$ are such that $b _ { i j } = b _ { j i }$ and 

$$
\sum_ {i, j = 1} ^ {m} \sum_ {\ell = 1} ^ {n} b _ {i \ell} (x) b _ {j \ell} (x) v _ {i} v _ {j} > 0 \quad \forall v \in \mathbb {R} ^ {m} \text {   and   } \forall x \in \mathbb {R} ^ {m},
$$

i.e. for each $x \in \mathbb { R } ^ { m }$ the covariance matrix is positive definite. For some diferentiable function, there is a multivariate version of the Itˆo lemma. 

Lemma 2.4.1. (The Multivariate Itˆo Lemma). Let $f : \mathbb { R } ^ { + } \times \mathbb { R } ^ { m } \to \mathbb { R }$ with at least one derivative in the first argument and at least two derivatives in the remaining m arguments. The diferential of $f ( t , X _ { t } )$ is 

$$
d f (t, X _ {t}) = \left(\frac {\partial}{\partial t} + \sum_ {i = 1} ^ {m} \alpha_ {i} (X _ {t}) \frac {\partial}{\partial x _ {i}} + \frac {1}{2} \sum_ {i, j = 1} ^ {m} \mathbf {b} _ {i j} (X _ {t}) \frac {\partial^ {2}}{\partial x _ {i} \partial x _ {j}}\right) f (t, X _ {t}) d t
$$

$$
+ \sum_ {i = 1} ^ {m} \sum_ {\ell = 1} ^ {n} b _ {i \ell} (X _ {t}) \frac {\partial}{\partial x _ {i}} f (t, X _ {t}) d W _ {t} ^ {\ell}\tag{2.3}
$$

here $\begin{array} { r } { \mathbf { b } _ { i j } ( x ) = \sum _ { \ell = 1 } ^ { n } b _ { i \ell } ( x ) b _ { j \ell } ( x ) } \end{array}$ 

Equation (2.3) is essentially a 2nd-order Taylor expansion like the univariate case of equation (2.2). Of course, Theorem 2.3.1 still applies to to the system of SDEs (make sure $a _ { i }$ and $b _ { i j }$ have linear growth and are Lipschitz continuous for each i and $j )$ , and in the multidimensional case it is also important whether or not $n \geq m$ , and if so it is important that there is some constant c such that in $\mathrm { f } _ { x } \mathbf { b } ( x ) > c > 0$ . If there is not such constant $c > 0$ , then we are possibly dealing with a system that is degenerate and there could be (mathematically) technical problems. 

Correlated Brownian Motion. Sometimes the multivariate case is formulated with a correlation structure among the $W _ { t } ^ { i } \mathrm { { ^ , s } } ,$ , in which the Itˆo lemma of equation (2.3) will have extra correlation terms. Suppose there is correlation matrix, 

$$
\rho = \left( \begin{array}{c c c c c} 1 & \rho_ {1 2} & \rho_ {1 3} & \ldots & \rho_ {1 n} \\ \rho_ {2 1} & 1 & \rho_ {2 3} & \ldots & \rho_ {2 n} \\ \rho_ {3 1} & \rho_ {3 2} & 1 & \ldots & \rho_ {3 n} \\ \vdots & & & \ddots & \\ \rho_ {n 1} & \rho_ {n 2} & \rho_ {n 3} & \ldots & 1 \end{array} \right)
$$

where $\rho _ { i j } = \rho _ { j i }$ and such that $\begin{array} { r } { \frac { 1 } { t } \mathbb { E } W _ { t } ^ { i } W _ { t } ^ { j } = \rho _ { i j } } \end{array}$ for all $i , j \le n$ . Then equation (2.3) becomes 

$$
d f (t, X _ {t}) = \left(\frac {\partial}{\partial t} + \sum_ {i = 1} ^ {m} \alpha_ {i} (X _ {t}) \frac {\partial}{\partial x _ {i}} + \frac {1}{2} \sum_ {i, j = 1} ^ {m} \sum_ {\ell , k = 1} ^ {n} \rho_ {\ell k} b _ {i \ell} (X _ {t}) b _ {k j} (X _ {t}) \frac {\partial^ {2}}{\partial x _ {i} \partial x _ {j}}\right) f (t, X _ {t}) d t
$$

$$
+ \sum_ {i = 1} ^ {m} \sum_ {\ell = 1} ^ {n} b _ {i} (X _ {t}) \frac {\partial}{\partial x _ {i}} f (t, X _ {t}) d W _ {t} ^ {\ell}.
$$

Example 2.4.1. (Bivariate Example). Consider the case when $n = m = 2$ , with 

$$
\begin{array}{l} {d X _ {t} = a (X _ {t}) d x + b (X _ {t}) d W _ {t} ^ {1}} \\ {d Y _ {t} = \alpha (Y _ {t}) d t + \sigma (Y _ {t}) d W _ {t} ^ {2}} \end{array}
$$

and with $\begin{array} { r } { \frac { 1 } { t } \mathbb { E } W _ { t } ^ { 1 } W _ { t } ^ { 2 } = \rho } \end{array}$ . Then, 

$$
\begin{array}{l} d f (t, X _ {t}, Y _ {t}) = \frac {\partial}{\partial t} f (t, X _ {t}, Y _ {t}) d t \\ \qquad + \underbrace {\left(\frac {b ^ {2} (X _ {t})}{2} \frac {\partial^ {2}}{\partial x ^ {2}} + a (X _ {t}) \frac {\partial}{\partial x}\right) f (t , X _ {t} , Y _ {t}) d t + b (X _ {t}) \frac {\partial}{\partial x} f (t , X _ {t} , Y _ {t}) d W _ {t} ^ {1}} _ {X _ {t} \text {terms}} \\ \qquad + \underbrace {\left(\frac {\sigma^ {2} (Y _ {t})}{2} \frac {\partial^ {2}}{\partial y ^ {2}} + \alpha (Y _ {t}) \frac {\partial}{\partial y}\right) f (t , X _ {t} , Y _ {t}) d t + \sigma (Y _ {t}) \frac {\partial}{\partial y} f (t , X _ {t} , Y _ {t}) d W _ {t} ^ {2}} _ {Y _ {t} \text {terms}} \\ \qquad + \underbrace {\rho \sigma (X _ {t}) b (X _ {t}) \frac {\partial^ {2}}{\partial x \partial y} f (t , X _ {t} , Y _ {t}) d t} _ {\text {cross - term.}} \end{array}
$$

## 2.5 The Feynman-Kac Formula

If you one could identify the fundamental link between asset pricing and stochastic diferential equations, it would be the Feynman-Kac formula. The Feynman-Kac formula says the following: 

Proposition 2.5.1. (The Feynman-Kac Formula). Let the function $f ( x )$ be bounded, let $\psi ( x )$ be twice diferentiable with compact support<sup>2</sup> in $K \subset \mathbb { R }$ , and let the function $q ( x )$ is bounded below for all $x \in \mathbb { R }$ , and let $X _ { t }$ be given by the SDE 

$$
d X _ {t} = a (X _ {t}) d t + b (X _ {t}) d W _ {t}.\tag{2.4}
$$

• For $t \in [ 0 , T ]$ , the Feynman-Kac formula is 

$$
v (t, x) = \mathbb {E} \left[ \int_ {t} ^ {T} f (X _ {s}) e ^ {- \int_ {t} ^ {s} q (X _ {u}) d u} d s + e ^ {- \int_ {t} ^ {T} q (X _ {s}) d s} \psi (X _ {T}) \Big | X _ {t} = x \right]\tag{2.5}
$$

and is a solution to the following partial diferential equation (PDE): 

$$
\frac {\partial}{\partial t} v (t, x) + \left(\frac {b ^ {2} (x)}{2} \frac {\partial^ {2}}{\partial x ^ {2}} + a (x) \frac {\partial}{\partial x}\right) v (t, x) - q (x) v (t, x) + f (t, x) = 0\tag{2.6}
$$

$$
v (T, x) = \psi (x)\tag{2.7}
$$

${ \cal I } f \omega ( t , x )$ is a bounded solution to equations (2.6) and (2.7) for $x \in K$ , then $\omega ( t , x ) =$ $v ( t , x )$ 

The Feynman-Kac formula will be instrumental in pricing European derivatives in the coming sections. For now it is important to take note of how the SDE in (2.4) relates to the formula (2.5) and to the PDE of (2.6) and (2.7). It is also important to conceptualize how the Feynman-Kac formula might be extended to the multivariate case. In particular for scalar solutions of (2.6) and (2.7) that are expectations of a multivariate process $X _ { t } \in \mathbb { R } ^ { m }$ ， the key thing to realize is that x-derivatives in (2.6) are the same is the dt-terms in the Itˆo lemma. Hence, multivariate Feynman-kac can be deduced from the multivariate Itˆo lemma. 

## 2.6 Girsanov Theorem

Another important link between asset pricing and stochastic diferential equations is the Girsanov theorem, which provides a means for defining the equivalent martingale measure. 

For $T < \infty ,$ , consider a Brownian motion $( W _ { t } ) _ { t \leq T }$ , and consider another process $\theta _ { t }$ that does not anticipate future outcomes of the W (i.e. given the filtration $\mathcal { F } _ { t } ^ { W }$ generated by the history of W up to time $t , \ \theta _ { t }$ is adapted to $\mathcal { F } _ { t } ^ { W } )$ . The first feature to the Girsanov theorem is the Dolean-Dade exponent: 

$$
Z _ {t} \doteq \exp \left(- \frac {1}{2} \int_ {0} ^ {t} \theta_ {s} ^ {2} d s + \int_ {0} ^ {t} \theta_ {s} d W _ {s}\right)\tag{2.8}
$$

A suficient condition for the application of Girsanov theorem is the Novikov condition, 

$$
\mathbb {E} \exp \left(\frac {1}{2} \int_ {0} ^ {T} \theta_ {s} ^ {2} d s\right) <   \infty .
$$

Given the Novikov condition, the process $Z _ { t }$ is a martingale on [0, T] and a new probability measure is defined using the density 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} \Big | _ {t} = Z _ {t} \quad \forall t \leq T;\tag{2.9}
$$

in general $Z$ may not be a true martingale but only a local martingale (see Appendix A and [Harrison and Pliska, 1981]). The Girsanov Theorem is stated as follows: 

Theorem 2.6.1. (Girsanov Theorem). If $Z _ { t }$ is a true martingale on [0, T] then the process $\begin{array} { r } { \widetilde { W _ { t } } = W _ { t } - \int _ { 0 } ^ { t } \theta _ { s } d s } \end{array}$ is Brownian motion under the measure $\mathbb { Q }$ on [0, T]. 

Remark 1. The Novikov condition is only suficient and not necessary. There are other suficient conditions such as the Kazamaki condition, $\begin{array} { r } { \operatorname* { s u p } _ { \tau \in \mathcal { T } } \mathbb { E } e ^ { \frac { 1 } { 2 } \int _ { 0 } ^ { T \wedge \tau } \theta _ { s } d W _ { s } } < \infty } \end{array}$ where T is the set of finite stopping times. 

Remark 2. It is important to have $T < \infty$ . In fact, the Theorem does not hold for infinite time. 

Example 2.6.1. (EMM for Asset Prices of Geometric Brownian Motion). The important example for finance the (unique) EMM for the geometric Brownian. Let $S _ { t }$ be the price of an asset, 

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma d W _ {t},
$$

and let $r \geq 0$ be the risk-free rate of interest. For the exponential martingale 

$$
Z _ {t} = \exp \left(- \frac {t}{2} \left(\frac {r - \mu}{\sigma}\right) ^ {2} + \frac {r - \mu}{\sigma} W _ {t}\right),
$$

the process $\begin{array} { r } { W _ { t } ^ { Q } \doteq \frac { \mu - r } { \sigma } t + W _ { t } } \end{array}$ is Q-Brownian motion, and the price process satisfies, 

$$
\frac {d S _ {t}}{S _ {t}} = r d t + \sigma d W _ {t} ^ {Q}.
$$

Hence 

$$
S _ {t} = S _ {0} \exp \left(\left(r - \frac {1}{2} \sigma^ {2}\right) t + \sigma W _ {t} ^ {Q}\right)
$$

and $S _ { t } e ^ { - r t }$ is a Q-martingale. 

## Chapter 3

## The Black-Scholes Theory

This section builds a pricing theory around the assumptions of no-arbitrage with perfect liquidity and trades occurring in continuous time. The Black-Scholes model is a complete market, and there turns out to be a fairly general class of partial diferential equations (PDEs) that can price many contingent claims. The focus of Black-Scholes theory is often on European call and put options, but exotics such as the Asian and the exchange option are simple extensions of the basic formulae. The issues with American options are covered later in Section 5.3. 

## 3.1 The Black-Scholes Model

The Black-Scholes model assumes a market consisting of a single risky asset and a risk-free bank account. This market is given by the equations 

$$
\begin{array}{r c l l} \frac {d S _ {t}}{S _ {t}} & = & \mu d t + \sigma d W _ {t} & \mathrm{geometricBrownian-Motion} \\ d B _ {t} & = & r B _ {t} d t & \mathrm{non-stochastic} \end{array}
$$

where $W _ { t }$ is Brownian motion as described in Chapter 2 and the interpretation of the parameters is as follows: 

$\mu$ is the expected rate of return in the risk asset, 

σ > 0 is the volatility of the risky asset, 

$r \geq 0$ is the bank’s rate of interest. 

It turns out that this market is particularly well-suited for pricing options and other variations, as well as analyzing basic risks associated with the writing of such contracts. Even though this market is an oversimplification of real life, it is still remarkable how a such a parsimonious model is able to capture so much of the very essence of the risky behavior in the markets. In particular, the parameter σ will turn out to be a hugely important factor in secondary markets for options, swaps, etc. 

The default focus in these notes will be the European call option with strike K and maturity T, that is, a security that pays 

$$
(S _ {T} - K) ^ {+} \doteq \max (S _ {T} - K, 0),
$$

with strike and contract price agreed upon at some earlier time $t < T$ . In general, the price of any European derivative security with payof $\psi ( S _ { T } )$ (i.e. a derivative with payof determined by the terminal value of risky asset) will be a function of the current time and the current asset price, 

$$
C (t, S _ {t}) = \text {   price   of   derivative   security.   }
$$

The fact that the price can be written a function of t and $S _ { t }$ irrespective of $S \mathrm { { ^ { \circ } s } }$ history is due to the fact the model is Markov. Through an arbitrage argument we will arrive at a PDE for the pricing function C. Pricing equations for general non-European derivatives (such as the Asian option discussed in Section 5.1) are determined on a case-by-case basis. 

## 3.2 Self-Financing Portfolio

Let $V _ { t }$ denote the $-value of a portfolio with shares in the risk asset and the rest of it’s value in the risk-free bank account. At any time the portfolio can be written as 

$$
V _ {t} = \alpha_ {t} S _ {t} + \beta_ {t}
$$

where $\alpha _ { t }$ is the number of shares in $S _ { t }$ (could be any real number) and $\beta _ { t }$ is the $-amount in bank. The key characteristic that will be associated with V throughout these notes is the following condition: 

Definition 3.2.1. The portfolio $V _ { t }$ is self-financing if 

$$
d V _ {t} = \alpha_ {t} d S _ {t} + r \beta_ {t} d t
$$

with $\beta _ { t } = V _ { t } - \alpha _ { t } S _ { t }$ 

The self-financing condition is not entirely obvious at first, but it helps to think of one’s personal decision-making in a financial market. Usually, one chooses a portfolio allocation in stocks and bonds, and then allows a certain amount of change to occur in the market before adjusting their allocation. If you don’t remove any cash for consumption and you don’t inject any cash for added investment, then your portfolio is self-financing. Indeed, in discrete time the self-financing condition is 

$$
V _ {t _ {n + 1}} = V _ {t _ {n}} + \alpha_ {t _ {n}} (S _ {t _ {n + 1}} - S _ {t _ {n}}) + (e ^ {r \Delta t} - 1) \beta_ {t _ {n}}
$$

where $\Delta t = t _ { n + 1 } - t _ { n }$ . This becomes the condition described in Definition 3.2.1 as $\Delta t \searrow 0$ 

## 3.3 The Black-Scholes Equation

For general functions $f ( t , s )$ , the Itˆo lemma for the geometric Brownian motion process is 

$$
d f (t, S _ {t}) = \left(\frac {\partial}{\partial t} + \mu S _ {t} \frac {\partial}{\partial s} + \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}}\right) f (t, S _ {t}) d t + \sigma S _ {t} \frac {\partial}{\partial s} f (t, S _ {t}) d W _ {t}
$$

(recall equation (2.2) from Chapter 2). Hence, applying the Itˆo lemma to the price function $C ( t , S _ { t } )$ , the dynamics of the option and the self-financing portfolio are 

$$
{d C (t, S _ {t})} = {\left(\frac {\partial}{\partial t} + \mu S _ {t} \frac {\partial}{\partial s} + \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}}\right) C (t, S _ {t}) d t + \sigma S _ {t} \frac {\partial}{\partial s} C (t, S _ {t}) d W _ {t}}\tag{3.1}
$$

$$
{d V _ {t}} = {\alpha_ {t} d S _ {t} + r \beta_ {t} d t .}\tag{3.2}
$$

The idea is to find $\alpha _ { t }$ that can be known to us at time t (given our observed history of prices) so that $V _ { t }$ replicates $C ( t , S _ { t } )$ as closely as possible. Setting $\begin{array} { r } { \alpha _ { t } = \frac { \partial } { \partial s } C ( t , S _ { t } ) } \end{array}$ and $\beta _ { t } = V _ { t } - \alpha _ { t } S _ { t }$ , then buying the portfolio and shorting C gets a risk-less portfolio 

$$
d (V _ {t} - C (t, S _ {t})) = r \left(V _ {t} - S _ {t} \frac {\partial}{\partial s} C (t, S _ {t})\right) d t - \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}}\right) C (t, S _ {t}) d t
$$

and by arbitrage arguments, this must be equal to the risk-free rate, 

$$
= r (V _ {t} - C (t, S _ {t})) d t.
$$

Hence, we arrive at the Black-Scholes PDE 

$$
\left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} s ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + r s \frac {\partial}{\partial s} - r\right) C (t, s) = 0\tag{3.3}
$$

with $C ( T , s ) = \psi ( s )$ (recall we denote payof function for general European claim with function $\psi ( s ) )$ 

The power of the Black -Scholes PDE is that it replicates perfectly. Observe: if $V _ { 0 } =$ $C ( 0 , S _ { 0 } )$ , then 

$$
d (V _ {t} - C (t, S _ {t})) = 0 \quad \forall t \leq T,
$$

and so $V _ { T } = C ( T , S _ { T } ) = \psi ( S _ { T } )$ . In fact, it can be shown that any contingent claim (not just Europeans) is replicable under the Black-Scholes model. Hence, the market is complete. 

## 3.4 Feynman-Kac, the EMM, & Heat Equations

Feynman-Kac is a probabilistic formula for solving PDEs like (3.3). It also has financial meaning because it explicitly provides a unique equivalent martingale measure (EMM). Since we have assume no-arbitrage, the 1st Fundamental theorem of asset pricing (see Section 1) necessarily asserts the existence of an EMM. The structure of this probability measure is given to us by the Feynman-Kac formula: 

Proposition 3.4.1. (Feynman-Kac). The solution to the Black-Scholes PDE of (3.3) is the expectation 

$$
C (t, s) = e ^ {- r (T - t)} \mathbb {E} ^ {Q} [ \psi (S _ {T}) | S _ {t} = s ]
$$

where $\mathbb { E } ^ { Q }$ is an EMM under which $e ^ { r ( T - t ) } S _ { t }$ is a martingale, 

$$
d S _ {t} = r S _ {t} d t + \sigma S _ {t} d W _ {t} ^ {Q},
$$

with $\begin{array} { r } { W _ { t } ^ { Q } \doteq \frac { \mu - r } { \sigma } t + W _ { t } } \end{array}$ being Brownian motion under the EMM. 

Non-Smooth Payofs. For call options, the function $\psi$ is not twice diferentiable nor does it have compact support, so Proposition 3.4.1 is not a direct application of Feynman-Kac as stated in Proposition 2.5.1 of Chapter 2. There needs to be a further massaging of PDE to show that the formula holds for this special case. It is quite technical, but the end result is that Feynman-Kac applies to most payofs of financial assets for log-normal models. 

Uniqueness. The uniqueness of the EMM in Proposition 3.4.1 can be argued by using the uniqueness of solutions to (3.3). The conclusion that the EMM is unique and that the market is complete. 

Relationship with Heat Equation. The Black-Scholes PDE (3.3) is a type of heat equation from physics. The basic heat equation is 

$$
\frac {\partial}{\partial t} u (t, x) = \sigma^ {2} \frac {\partial^ {2}}{\partial x ^ {2}} u (t, x)
$$

with some initial condition $u | _ { t = 0 } = f .$ . Solutions to the heat equation are interpreted as the evolution of Brownian motion’s probability distribution. In the same manner that passage of time will coincide with the difusion of heat from a source, the heat equation can describe the difusion of possible trajectories of Brownian motion away from their common starting point of $W _ { 0 } = 0$ 

Equation (3.3) obviously has some extra term and an $\cdot _ { s } ,$ in front of the 2nd derivative, but a change of variables of $\tau = T - t$ and $x = \log ( s )$ leads to a representation of the solution as 

$$
\widetilde {C} (\tau , x) = C (T - \tau , e ^ {x})
$$

where $C$ solves the Black-Scholes PDE. Doing the calculus we arrive at a more basic PDE for $\widetilde { C }$ 

$$
\frac {\partial}{\partial \tau} \widetilde {C} (\tau , x) = \frac {\sigma^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} \widetilde {C} (\tau , x) + \left(b \frac {\partial}{\partial x} - r\right) \widetilde {C} (\tau , x)
$$

with initial condition $C ( 0 , x ) = \psi ( e ^ { x } )$ , and with $\begin{array} { r } { b = { \frac { 2 r - \sigma ^ { 2 } } { 2 } } } \end{array}$ . Hence Black-Scholes is a heat equation with drift $\textstyle b { \frac { \partial } { \partial x } } { \tilde { C } } ( \tau , x )$ , and decay $r \widetilde { C } ( \tau , x )$ 

## 3.5 The Black-Scholes Call Option Formula

Let $\psi ( s ) = ( s - K ) ^ { + }$ . From Feynman-Kac we have 

$$
C (t, s) = e ^ {- r (T - t)} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ]
$$

with $d S _ { t } = r S _ { t } d t + \sigma S _ { t } d W _ { t } ^ { Q }$ . Through a verification with Itˆo’s Lemma we can see that underlying’s value at time of maturity can be written as a log-normal random variable, 

$$
S _ {T} = S _ {t} \exp \left(\left(r - \frac {1}{2} \sigma^ {2}\right) (T - t) + \sigma (W _ {T} - W _ {t})\right).
$$

And so $\log ( S _ { T } / S _ { t } )$ is in fact normally distributed under the risk-neutral measure, 

$$
\log (S _ {T} / S _ {t}) \sim \mathcal {N} \left(\left(r - \frac {1}{2} \sigma^ {2}\right) (T - t), \sigma^ {2} (T - t)\right).
$$

Hence, we compute the expectation for $\psi ( s ) = ( s - K ) ^ { + }$ 2 

$$
\begin{array}{c} \mathbb {E} ^ {Q} \{(S _ {T} - K) ^ {+} | S _ {t} = s \} \\ = \underbrace {\frac {S _ {t}}{\sqrt {2 \pi \sigma^ {2} (T - t)}} \int_ {\log (K / S _ {t})} ^ {\infty} e ^ {x} e ^ {- \frac {1}{2} \left(x - \left(r - \frac {1}{2} \sigma^ {2}\right) (T - t)\right) ^ {2} / (\sigma^ {2} (T - t))} d x} _ {= (\dagger)} \\ - \underbrace {K \mathbb {Q} (\log (S _ {T} / S _ {t}) > \log (K / S _ {t}))} _ {= (\star)} \end{array}
$$

where $\mathbb { Q }$ is the risk-neutral probability measure. 

(†). First compute (†) (W.L.O.G. for $t = 0 )$ ): 

$$
\begin{array}{r l r} & & {(\dagger) = \frac {S _ {0}}{\sqrt {2 \pi \sigma^ {2} T}} \int_ {\log (K / S _ {0})} ^ {\infty} e ^ {x} e ^ {- \frac {1}{2} \left(\frac {x - (r - \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}}\right) ^ {2}} d x} \\ & & {= \frac {S _ {0}}{\sqrt {2 \pi \sigma^ {2} T}} \int_ {\log (K / S _ {0})} ^ {\infty} e ^ {- \frac {1}{2 \sigma^ {2} T} \left(- 2 x ^ {2} \sigma^ {2} T + x ^ {2} - 2 x (r -. 5 \sigma^ {2}) T + ((r -. 5 \sigma^ {2}) T) ^ {2}\right)} d x} \\ & & {= \frac {S _ {0}}{\sqrt {2 \pi \sigma^ {2} T}} \int_ {\log (K / S _ {0})} ^ {\infty} e ^ {- \frac {1}{2 \sigma^ {2} T} \left(x ^ {2} - 2 x (r +. 5 \sigma^ {2}) T + ((r -. 5 \sigma^ {2}) T) ^ {2}\right)} d x} \\ & & {= \frac {S _ {0} e ^ {r T}}{\sqrt {2 \pi \sigma^ {2} T}} \int_ {\log (K / S _ {0})} ^ {\infty} e ^ {- \frac {1}{2 \sigma^ {2} T} \left(x ^ {2} - (r +. 5 \sigma^ {2}) T\right) ^ {2}} d x} \end{array}
$$

change of variables $\begin{array} { r } { v = \frac { x - ( r + . 5 \sigma ^ { 2 } ) T } { \sigma \sqrt { T } } , d v = d x / ( \sigma \sqrt { T } ) } \end{array}$ , so that 

$$
\begin{array}{r l r} & & {(\dagger) = \frac {S _ {0} e ^ {r T}}{\sqrt {2 \pi}} \int_ {(\log (K / S _ {0}) - (r +. 5 \sigma^ {2}) T) / (\sigma \sqrt {T})} ^ {\infty} e ^ {\frac {1}{2} v ^ {2}} d v} \\ & & {= S _ {0} e ^ {r T} \left(1 - \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {(\log (K / S _ {0}) - (r +. 5 \sigma^ {2}) T) / (\sigma \sqrt {T})} e ^ {\frac {1}{2} v ^ {2}} d v\right)} \\ & & {= S _ {0} e ^ {r T} \left(1 - N (- d _ {1})\right)} \end{array}
$$

where $\begin{array} { r } { d _ { 1 } = \frac { \log ( S _ { 0 } / K ) + ( r + . 5 \sigma ^ { 2 } ) T } { \sigma \sqrt { T } } } \end{array}$ and $N ( \cdot )$ is the standard normal CDF. But the normal CDF has the property that $N ( - x ) = 1 - N ( x )$ , so 

$$
(\dagger) = S _ {0} e ^ {r T} N (d _ {1}).
$$

(?). Then, computing (?) is much simpler, 

$$
\begin{array}{c} (\star) = K \mathbb {Q} \left(\log (S _ {T} / S _ {0}) \geq \log (K / S _ {0})\right) \\ = K \mathbb {Q} \left(\frac {\log (S _ {T} / S _ {0}) - (r - . 5 \sigma^ {2}) T}{\sigma \sqrt {T}} \geq \frac {\log (K / S _ {0}) - (r - . 5 \sigma^ {2}) T}{\sigma \sqrt {T}}\right) \\ = K \left(1 - \mathbb {Q} \left(\frac {\log (S _ {T} / S _ {0}) - (r - . 5 \sigma^ {2}) T}{\sigma \sqrt {T}} \leq \frac {\log (K / S _ {0}) - (r - . 5 \sigma^ {2}) T}{\sigma \sqrt {T}}\right)\right) \\ = K \left(1 - N (- d _ {2})\right) = K N (d _ {2}) \end{array}
$$

where $\begin{array} { r } { d _ { 2 } = \frac { \log ( S _ { 0 } / K ) + ( r - . 5 \sigma ^ { 2 } ) T } { \sigma \cdot \sqrt { T } } = d _ { 1 } - \sigma \sqrt { T } } \end{array}$ . Hence, we have the Black-Scholes formula for a European Call Option, 

Proposition 3.5.1. (Black-Scholes Call Option Formula). The call option on $S _ { T }$ with strike K at time t with price $S _ { t }$ is given by 

$$
C (t, S _ {t}) = S _ {t} N (d _ {1}) - K e ^ {- r (T - t)} N (d _ {2})
$$

where $N ( \cdot )$ is the standard normal CDF and 

$$
\begin{array}{l} {d _ {1} = \frac {\log (S _ {t} / K) + (r + . 5 \sigma^ {2}) (T - t)}{\sigma \sqrt {T - t}}} \\ {d _ {2} = d _ {1} - \sigma \sqrt {T - t}.} \end{array}
$$

A plot of the Black-Scholes call option price with $K = 5 0 , r = . 0 2 , T = 3 / 1 2$ , and $\sigma = . 2$ with varying $S _ { 0 }$ is shown in Figure 3.1. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/83da90febf7bd92ea17dd6e4ccb2c319cc886a5733060c6a70116f9f77947ba6.jpg)



Figure 3.1: The Black-Scholes call price with $K = 5 0 , r = . 0 2 , T = 3 / 1 2 .$ and $\sigma = . 2 .$ Intrinsic value refers to the payof if exercised now, $( S _ { 0 } - K ) ^ { + }$


## 3.6 Put-Call Parity and the Put Option Formula

It is straight forward to verify the relationship 

$$
(S _ {T} - K) ^ {+} - (K - S _ {T}) ^ {+} = S _ {T} - K.\tag{3.4}
$$

Then applying the risk-neutral expectionan $e ^ { - r ( T - t ) } \mathbb { E } _ { t } ^ { Q }$ to both sides of (3.4) to get the put-call parity, 

$$
C (t, S _ {t}) - P (t, S _ {t}) = S _ {t} - K e ^ {- r (T - t)}\tag{3.5}
$$

where $C ( t , S _ { t } )$ is the price of a European call option and $\textstyle P ( t , S _ { t } )$ the price of a European put option with the same strike. From put-call parity we have 

$$
\begin{array}{c} P (t, s) = C (t, s) + K e ^ {- r (T - t)} - s \\ = - K e ^ {- r (T - t)} (N (d _ {2}) - 1) + s (N (d _ {1}) - 1) \\ = K e ^ {- r (T - t)} N (- d _ {2}) - s N (- d _ {1}), \end{array}
$$

because $1 - N ( x ) = N ( - x )$ for any $x \in \mathbb { R }$ 

Proposition 3.6.1. (Black-Scholes Put Option Formula). The put option on $S _ { T }$ with strike K at time t with price $S _ { t }$ is given by 

$$
P (t, S _ {t}) = K e ^ {- r (T - t)} N (- d _ {2}) - S _ {t} N (- d _ {1})
$$

where 

$$
\begin{array}{l} {d _ {1} = \frac {\log (S _ {t} / K) + (r + . 5 \sigma^ {2}) (T - t)}{\sigma \sqrt {T - t}}} \\ {d _ {2} = d _ {1} - \sigma \sqrt {T - t}.} \end{array}
$$

The Black-Scholes put option price for $K = 5 0 , r = . 0 2 , T = 3 / 1 2$ , and $\sigma = . 2$ and varying $S _ { 0 }$ is shown in Figure 3.2. 

## 3.7 Options on Futures and Stocks with Dividends

This section will explain how to compute European derivative prices on stocks with a continuously paying dividend rate, and on future prices. There is some technical issues with stocks paying dividends at a discrete times, but in the case of European options it is merely of matter of considering the future price. Dividends can be an issue in the Black-Scholes theory, particularly because they will determine whether or not Black-Scholes applies for American options (see Section 5.3). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/6f164cbb9069bc7723cc31ad013a875fe0be380c6672e2e81c1bf22735f52ef3.jpg)



Figure 3.2: The Black-Scholes put option price for $K = 5 0 , r = . 0 2 , T = 3 / 1 2 .$ , and $\sigma = . 2 .$ Intrinsic value refers to the payof if exercised now, $( K - S _ { 0 } ) ^ { + }$


Continuous Dividends. Suppose that a European option with payof $\psi ( S _ { T } )$ is being priced in a market with 

$$
\begin{array}{r c l} \frac {d S _ {t}}{S _ {t}} & = & (\mu - q) d t + \sigma d W _ {t} \\ d B _ {t} & = & r B _ {t} d t \end{array}
$$

where $q \geq 0$ is the dividend rate. Self-financing in this case has dynamics 

$$
d V _ {t} = \alpha_ {t} d S _ {t} + r (V _ {t} - \alpha_ {t} S _ {t}) d t + q \alpha_ {t} S _ {t} d t.
$$

The replicating strategy from the non-dividend case applies to obtain $\begin{array} { r } { \alpha _ { t } = \frac { \partial } { \partial s } C ( t , S _ { t } ) } \end{array}$ , but the arbitrage argument leads to a diferent equation, 

$$
\left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} s ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + (r - q) s \frac {\partial}{\partial s} - (r - q)\right) C (t, s) = q C (t, s)\tag{3.6}
$$

with $C ( T , s ) \ : = \ : \psi ( s )$ . Equation (3.6) is the Black-Scholes PDE with dividends, and is solved by 

$$
C (t, S _ {t}) = e ^ {- q (T - t)} C ^ {1} (t, S _ {t})
$$

where $C ^ { 1 } ( t , S _ { t } )$ solves the Black-Scholes equation of (3.3) with r replaced by $r - q$ . For example, a European call option on a stock with dividends: 

Proposition 3.7.1. (Call Option on Stock with Dividends). 

$$
C (t, S _ {t}) = S _ {t} e ^ {- q (T - t)} N (d _ {1}) - K e ^ {- r (T - t)} N (d _ {2})
$$

where 

$$
\begin{array}{l} {d _ {1} = \frac {\log (S _ {t} / K) + (r - q + . 5 \sigma^ {2}) (T - t)}{\sigma \sqrt {T - t}}} \\ {d _ {2} = d _ {1} - \sigma \sqrt {T - t}.} \end{array}
$$

Futures. Now we turn out attention to futures. Suppose that the spot price on a commodity is given by 

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma d W _ {t}.
$$

From arbitrage arguments we know that the future price on $S _ { T }$ is 

$$
F _ {t, T} \doteq S _ {t} e ^ {r (T - t)}
$$

with $F _ { T , T } = S _ { T }$ . However, $S _ { t } e ^ { r ( T - t ) }$ is a martingale under the EMM, and so $F _ { t , T }$ is also a martingale with 

$$
\frac {d F _ {t , T}}{F _ {t , T}} = \sigma d W _ {t} ^ {Q},
$$

and the price of a derivative in terms of $F _ { t , T }$ is $C ( t , F _ { t , T } ) = e ^ { - r ( T - t ) } \widetilde { C } ( t , F _ { t , T } )$ where $\widetilde { C }$ satisfies 

$$
\left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} x ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) \widetilde {C} (t, x) = 0\tag{3.7}
$$

with ${ \widetilde C } ( T , x ) = \psi ( x )$ . For example, the call option on the future: 

Proposition 3.7.2. (Call Option on Future). 

$$
C (t, F _ {t, T}) = e ^ {- r (T - t)} \left(F _ {t, T} N (d _ {1}) - K N (d _ {2})\right)
$$

where 

$$
\begin{array}{l} {d _ {1} = \frac {\log (F _ {t , T} / K) + . 5 \sigma^ {2} (T - t)}{\sigma \sqrt {T - t}}} \\ {d _ {2} = d _ {1} - \sigma \sqrt {T - t}.} \end{array}
$$

The Similarities. Futures contracts certainly have fundamental diferences from stocks paying dividends, and vice versa. But the Black-Scholes PDE for pricing options on futures is like that for a stock with dividend rate r. Alternatively, the future on a dividend paying stock is 

$$
F _ {t, T} = S _ {t} e ^ {(r - q) (T - t)}
$$

which is a non-dividend paying asset and can hence be priced using equation (3.7). 

Discrete-Time Dividends. This interpretation of dividend-paying stocks as futures is useful when dividends are paid at discrete times. Discrete time dividends are described as 

$$
\log (S _ {t} / S _ {0}) = \left(r - \frac {1}{2} \sigma^ {2}\right) t + \sigma W _ {t} ^ {Q} - \sum_ {i = 0} ^ {n (t)} \delta_ {i}
$$

where $\delta _ { i }$ is a proportional dividend rate, and $n ( t )$ is the number of dividends paid up to time t. The future price of dividend paying stock $S _ { T }$ is 

$$
F _ {t, T} = S _ {t} \exp \left(\left(r - \frac {1}{2} \sigma^ {2}\right) (T - t) - \sum_ {i = n (t) + 1} ^ {n (T)} \delta_ {i}\right).
$$

Call option on $F _ { T , T }$ can be priced with equation (3.7). 

## Chapter 4

# The Black-Scholes Greeks

The Greeks a set of letters labeling the quantities of risk associate with small changes in various inputs and model parameters. The Greeks have importance in risk management where hedging and risks are determined by how much/little of the Greeks are exposed on a portfolio. There are 5 main Greeks associated with the Black-Scholes, one of which has already been instrumental in setting up the hedging portfolio, namely the $\Delta$ . The other Greeks can be equally as important in determining the quality of a hedge. 

## 4.1 The Delta Hedge

Recall the derivation of the Black-Scholes PDE of equation (3.3) on page 25. In particular, recall the hedging allocation in the underlying was the first derivative. This is the Black-Scholes $\Delta$ 

$$
\Delta (t, s) \doteq \frac {\partial}{\partial s} C (t, s).
$$

In general, the hedge in the underlying what’s referred to when someone talks about being long, short or neutral in $\Delta$ . With continuos trading the hedging portfolio is a perfect replication because it continuously rebalances to remain ∆-neutral. $\mathrm { A }$ long position in $\Delta$ would be when the hedging portfolio holds the underlying in excess of the $\Delta$ (e.g. a covered call), and a short position in $\Delta$ would be a hedge with less (e.g. a naked call). 

For the European call and put options, the Black-Scholes $\Delta$ is 

$$
\begin{array}{r l} & {\Delta_ {c a l l} (t, s) = N (d _ {1})} \\ & {\Delta_ {p u t} (t, s) = - N (- d _ {1}) = \Delta_ {c a l l} (t, s) - 1} \end{array}
$$

which are obtained by diferentiating the formulas in Propositions 3.5.1 and 3.6.1, respectively. Plots of the $\Delta \mathrm { s }$ for varying s are shown in Figure 4.1. Notice that all the action in the ∆-hedge occurs when the underlying price is near the strike price. Intuitively, a call or put that is far money is eficiently hedged by either holding a share of the underling or simply holding the cash, and the risk is low because there very little probability of the underlying changing dramatically enough to efect your position. Hence, the $\Delta { \mathrm { - h e d g e } }$ is like a covered call/put when the derivative is far from the money. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/f2c43c8fdca94e1dbbbf59de907397bc214e5e7fbef4e51e265f12a333f10250.jpg)



Black Scholes Put ∆


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/78f0dedd51e267266758f2224ba6d9c82687edb8d865ecfb797d90031e3dace6.jpg)



Figure 4.1: Top: The Black-Scholes $\Delta$ for a European option with strike $K = 5 0$ , time to maturity $T = 3 / 1 2$ , interest rate $r = . 0 2$ , and volatility $\sigma = . 2$ . Bottom: The put option $\Delta .$


## 4.2 The Theta

The next Greek to discuss is the Θ, which measures the sensitivity to time. In particular, 

$$
\Theta (t, s) = \frac {\partial}{\partial t} C (t, s).
$$

The financial interpretation is that Θ measures the decay of the time value of the security. Intrinsic value of a security is fairly clear to understand: it is the value of the derivative at today’s price of the underlying. However, derivatives have an element of time value on top of the intrinsic value, and in cases where the intrinsic value is zero (e.g. an out-of-the-money option) the derivative’s entire cost is its time value. 

For option contracts, time value quantifies the cost to be paid for having the option to buy/sell, as opposed to taking a position that is long/short the underlying with no option involved. In most cases the time value is positive and decreases with time, hence $\Theta < 0 ,$ but there are contracts (such as far in-the-money put options) that have positive Θ. The $\Theta \mathrm { s }$ for European calls and puts are 

$$
\Theta_ {c a l l} (t, s) = - \frac {\sigma^ {2} S _ {t} ^ {2}}{2 \sqrt {T - t}} N ^ {\prime} (d _ {1}) - K e ^ {- r (T - t)} N (d _ {2})\tag{4.1}
$$

$$
\Theta_ {p u t} (t, s) = - \frac {\sigma^ {2} S _ {t} ^ {2}}{2 \sqrt {T - t}} N ^ {\prime} (d _ {1}) + K e ^ {- r (T - t)} N (- d _ {2})\tag{4.2}
$$

and are shown in Figure 4.2. To understand why a far in-the-money put option has positive Θ, look at Figure 4.3 and realize that the option price must with rise with time if it is below the intrinsic value. 


Black Scholes Call Θ


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/5685d153fbb579765a35e83937e4495d5b3486632ee2d859984c741617d34dc6.jpg)



Black Scholes Put Θ


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/bb29e21e0d61f8685f18da02ebcdb51a415e5b1acdda16eca4f38b9fdbef5b58.jpg)



Figure 4.2: Top: The Black-Scholes Θ for a European option with strike $K = 5 0$ , time to maturity $T = 3 / 1 2$ , interest rate $r = . 0 2$ , and volatility $\sigma = . 2$ . Bottom: The put option Θ.


In terms of hedging, a short position in a derivative is said to be short in $\Theta ,$ and a long position in the derivative is also long the Θ. Hence, a ∆-neutral hedge will exposed to Θ, and a decrease in Θ will benefit the short position because it means that the time value of the derivative decreases at a faster rate. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/d7f0e2c65397af06dfc914cdb143021465748d14f011357fc17ffb3c274b3e68.jpg)



Figure 4.3: The Black-Scholes price of a European put option with strike $K = 5 0$ , time to maturity $T = 5$ , interest rate $r = . 0 2$ , and volatility $\sigma = . 2$ . Notice if the price is low then the time value of exercise today is higher than the value of the option. This means that Θ of far in-the-money put options is positive.


## 4.3 The Gamma

The Γ of a security is the sensitivity of its ∆-hedge to changes in the underlying, and there a handful of ways in which the Γ explains hedging and risk management. In a nutshell, the Γ is the higher order sensitivity of the hedging portfolio, and is essentially a convexity term for higher order hedging. 

Let $\Delta t$ be the amount of time that goes by in between hedge adjustments. From Itˆo’s lemma we have the following approximations of the derivative dynamics and a self-financing portfolio: 

$$
\begin{array}{l} \Delta C _ {t} \simeq \left(\Theta_ {t} + \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \Gamma_ {t}\right) \Delta t + \Delta_ {t} \cdot \Delta S \\ \Delta V _ {t} \simeq \Delta_ {t} \cdot \Delta S _ {t} + r (V _ {t} - \Delta_ {t} \cdot S _ {t}) \Delta t \end{array}
$$

where $\Delta C _ { t } ~ = ~ C _ { t + \Delta t } - C _ { t }$ and $\Delta S _ { t } ~ = ~ S _ { t + \Delta t } - S _ { t }$ , and where $\Theta _ { t } , \ \Delta _ { t }$ and $\Gamma _ { t }$ are the derivative’s Greeks. Subtracting one from the other gets the (approximate) dynamics of a long position in the portfolio and short the derivative, 

$$
\Delta V _ {t} - \Delta C _ {t} \simeq \underbrace {r (V _ {t} - \Delta_ {t} \cdot S _ {t}) \Delta t} _ {\mathrm{earnedinbank}} + \underbrace {\left(- \Theta_ {t} - \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \Gamma_ {t}\right) \Delta t} _ {\mathrm{premiumoverrisk-free}}\tag{4.3}
$$

and so while the ∆-hedge replicates perfectly in continuous time, there will be error if this hedge is readjusted in discrete time. However, $- \Theta _ { t } - \frac { \sigma ^ { 2 } S _ { t } ^ { 2 } } { 2 } \Gamma _ { t } > 0$ corresponds to the premium over the risk-free rate earned by the hedging portfolio. Often times $\Gamma > 0$ and $\Theta < 0$ , and so the risk taken by rebalancing a $\Delta \cdot$ -hedge in discrete time is compensated with lower (more negative) Θ and lower Γ. 

For European call and put options, the Γ is 

$$
\Gamma (t, s) = \frac {N ^ {\prime} (d _ {1})}{S _ {t} \sigma \sqrt {T - t}}\tag{4.4}
$$

which proportional to the probability density function of log $( S _ { T } / S _ { t } )$ and is always positive for long positions. Furthermore, combining the Γ in (4.4) with equation (4.1) we find the premium of equation (4.3) is 

$$
- \Theta_ {c a l l} (t, s) - \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \Gamma (t, s) = K e ^ {- r (T - t)} N (d _ {2}) > 0,
$$

and so the ∆-hedge for a European call option earns a premium over the risk-free rate. However, the ∆-hedge of the put option has a negative premium 

$$
- \Theta_ {p u t} (t, s) - \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \Gamma (t, s) = - K e ^ {- r (T - t)} N (- d _ {2}) <   0,
$$

which means the portfolio that longs the put option and shorts the ∆-hedge will earn a return over the risk-free rate. 

If ∆-hedging is too risky then the Γ is used in higher order hedging, namely the $\Delta { - } \Gamma$ hedge. The idea is to consider a second derivative security $C ^ { \prime } ( t , s )$ with which to hedge. A hedge that is both ∆-neutral and Γ-neutral is found by solving the equations 

$$
\begin{array}{r l} & C (t, S _ {t}) = \alpha_ {t} S _ {t} + \beta_ {t} C ^ {\prime} (t, S _ {t}) + \eta_ {t} \\ & \Delta (t, S _ {t}) = \alpha_ {t} + \beta_ {t} \Delta^ {\prime} (t, S _ {t}) \\ & \Gamma (t, S _ {t}) = \beta_ {t} \Gamma^ {\prime} (t, S _ {t}) \end{array}
$$

where $\alpha _ { t }$ is the number of contracts in the underlying, $\beta _ { t }$ is number of contracts in $C ^ { \prime }$ , and $\eta _ { t }$ is the $-amount held in the risk-free bank account. This hedge is more expensive and will earn less premium over the risk-free rate, 

$$
\Delta V _ {t} - \Delta C _ {t} \simeq r \left(V _ {t} - \left(\Delta_ {t} - \Delta_ {t} ^ {\prime} \frac {\Gamma_ {t}}{\Gamma_ {t} ^ {\prime}}\right) S _ {t} - \frac {\Gamma}{\Gamma^ {\prime}} C _ {t} ^ {\prime}\right) \Delta t + \left(\frac {\Gamma_ {t}}{\Gamma_ {t} ^ {\prime}} \Theta_ {t} ^ {\prime} - \Theta_ {t}\right) \Delta t,
$$

with $\frac { \Gamma _ { t } } { \Gamma _ { t } ^ { \prime } } \Theta _ { t } ^ { \prime } - \Theta _ { t }$ being the premium over the risk-free rate. A plot of the Black-Scholes Γ is shown in Figure 4.4. 

## 4.4 The Vega

The Vega is the Greek to describe sensitivity to $\sigma .$ Of the 5 main Greeks it is the only one that corresponds to a latent parameter (although some could argue that the risk-free rate is also somewhat latent or abstract). Hence, not only is it important to have a good estimate of $\sigma ,$ it is also important to know if your hedging position is sensitive to estimation error. Indeed, volatility is a major question inn derivative pricing, and will be addressed in complete detail in Section 6. 

For the Black-Scholes call and puts, the Vega is 

$$
\frac {\partial}{\partial \sigma} C = S _ {t} N ^ {\prime} (d _ {1}) \sqrt {T - t}
$$

which is proportional to the Γ and to the probability density function of log $( S _ { T } / S _ { t } )$ (see Figure 4.4). There are some portfolios that are particularly sensitive Vega, for instance a straddle consisting of a call and put with the same strike K if K is near the money. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/9ce210396875a2dc32a31d77286f3d6f45c9842fad0b152d458867bb48c9f9d1.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/aed34830af99f4b581a3666093f6aa7f70d51b899ed51b4b99aa2c1d2ea5f774.jpg)



Figure 4.4: Top: The Black-Scholes $\begin{array} { r } { \Gamma = \frac { N ^ { \prime } ( d _ { 1 } ) } { S _ { t } \sigma \sqrt { T - t } } } \end{array}$ , proportional to the a Gaussian probability density function of $\log ( S _ { T } / S _ { t } )$


## 4.5 The Rho

The $\rho$ is the sensitivity of to changes in the risk-free rate 

$$
\rho = \frac {\partial}{\partial r} C.
$$

Of the 5 main Greeks it widely considered to be the least sensitive. For the Black-Scholes call and put options, the $\rho$ is 

$$
\begin{array}{r l} & {\rho_ {c a l l} = K (T - t) e ^ {- r (T - t)} N (d _ {2})} \\ & {\rho_ {p u t} = - K (T - t) e ^ {- r (T - t)} N (- d _ {2}).} \end{array}
$$

Notice that $\rho _ { c a l l } > 0$ because higher interest rates means risky assets should rise in price and hence it will be more likely that you will exercise. Similarly, $\rho _ { p u t } < 0$ because higher interest rates means it is less likely that you will exercise. 

## 4.6 Other Greeks

There are also other Greeks of interest in derivatives. Some of the are 

$\Lambda , \frac { \partial } { \partial S } C \times \frac { S } { C }$ , elasticity, or measure of leverage. 

• Vanna, $\frac { \partial ^ { 2 } } { \partial s \partial \sigma } C$ , The sensitivity of the $\Delta$ to changes in volatility. 

$\textstyle \mathrm { V o l g a } , \frac { \partial ^ { 2 } } { \partial \sigma ^ { 2 } } C$ , used for more elaborate volatility hedging. 

## Chapter 5

## Exotic Options

This section describes some of the better-known facts regarding a few exotic derivatives. The American and the Asian options are considered ‘path-dependent’ because the payof of the option will vary depending on the history of the price process, whereas exchange options and binary options are not path-dependent because the payof only depends on the asset price(s) are the terminal time. 

## 5.1 Asian Options

Asian option consider the average price of the underlying in the payof, 

$$
\psi_ {T} = \left(\frac {1}{T} \int_ {0} ^ {T} S _ {t} d t - K\right) ^ {+}.
$$

These options are path dependent because the path taken by the underlying is considered. The averaging in the Asian option makes it harder to manipulate the payof by driving the underlying’s price up or down when the option is close to maturity. 

Delta Hedge. In the Black-Scholes framework, the Asian option is a relatively simple extension of the hedging argument used to derive the Black-Scholes PDE. The trick is to consider an use an integrated field, 

$$
Z _ {t} = \frac {1}{T} \int_ {0} ^ {t} S _ {u} d u,
$$

and consider the price 

$$
C (t, s, z) = \text {   price   of   Asian   option   given   } S _ {t} = s \text {   and   } Z _ {t} = z.
$$

Let the underlying’s dynamics be 

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma d W _ {t}
$$

where $W _ { t }$ is a Brownian motion. From Itˆo’s lemma we have 

$$
d C (t, S _ {t}, Z _ {t}) = \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + \mu S _ {t} \frac {\partial}{\partial s} + \frac {S _ {t}}{T} \frac {\partial}{\partial z}\right) C (t, S _ {t}, Z _ {t}) d t + \sigma S _ {t} \frac {\partial}{\partial s} C (t, S _ {t}, Z _ {t}) d W _ {t} .
$$

On the other hand, we have a self-financing portfolio, 

$$
d V _ {t} = \alpha_ {t} d S _ {t} + r (V _ {t} - \alpha_ {t} S _ {t}) d t
$$

where $\alpha _ { t }$ is the number of contracts in $S _ { t }$ and $\left( V _ { t } - \alpha _ { t } S _ { t } \right)$ is the $-amount in the risk-free asset. Comparing the Itˆo lemma of the option to the self-financing portfolio, we see that a portfolio that is long $V _ { t }$ and short the Asian option will be risk-less if we have the ∆-hedge 

$$
\alpha_ {t} = \frac {\partial}{\partial s} C (t, S _ {t}, Z _ {t}).
$$

Furthermore, since the portfolio long $V _ { t }$ and short the option is risk-less, it must be that it earns at the risk-free rate. Hence, 

$$
d (V _ {t} - C (t, S _ {t}, Z _ {t})) = r \left(V _ {t} - S _ {t} \frac {\partial}{\partial s} C (t, S _ {t}, Z _ {t})\right) d t - \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} S _ {t} ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + \frac {S _ {t}}{T} \frac {\partial}{\partial z}\right) C (t, S _ {t}, Z _ {t}) d t
$$

$$
= r (V _ {t} - C (t, S _ {t}, Z _ {t})) d t.
$$

Hence, the price of the Asian option satisfies the following PDE, 

$$
\left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} s ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + s \frac {\partial}{\partial s} + \frac {s}{T} \frac {\partial}{\partial z} - r\right) C (t, s, z) = 0\tag{5.1}
$$

$$
C (t, s, z) \Big | _ {t = T} = (z - K) ^ {+}.\tag{5.2}
$$

Equations (5.1) and (5.2) can be solved with a Feynman-Kac formula, 

$$
C (t, s, z) = e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ (I _ {T} - K) ^ {+} \Big | S _ {t} = s, Z _ {t} = z \right]
$$

where $\mathbb { E } ^ { Q }$ is the expected value under the unique EMM $\mathbb { Q } ,$ and the asset price is $\begin{array} { r } { \frac { d S _ { t } } { S _ { t } } = } \end{array}$ $r d t + \sigma d W _ { t } ^ { Q }$ under $\mathbb { Q } .$ . We knew from Chapter 3 that this market was complete, so it shouldn’t come as a surprise that we were able to hedge perfectly the Asian option. 

PDE of Reduced Dimension. A useful formula is the dimension reduction of the Asian option price to a function of just time and one stochastic field. Define a new function 

$$
\phi (t, x) \doteq \mathbb {E} ^ {Q} \left[ \left(\frac {1}{T} \int_ {t} ^ {T} S _ {u} d u - x\right) ^ {+} \Big | S _ {t} = 1 \right].
$$

Then let $\mathcal { F } _ { t }$ denote the history of prices up time time t, and define the martingale 

$$
\begin{array}{c} M _ {t} \doteq \mathbb {E} ^ {Q} \left[ \left(\frac {1}{T} \int_ {0} ^ {T} S _ {u} d u - K\right) ^ {+} \Big | \mathcal {F} _ {t} \right] \\ = \mathbb {E} ^ {Q} \left[ \left(\frac {1}{T} \int_ {t} ^ {T} S _ {u} d u - \left(K - \frac {1}{T} \int_ {0} ^ {t} S _ {u} d u\right)\right) ^ {+} \Big | \mathcal {F} _ {t} \right] \\ = S _ {t} \mathbb {E} ^ {Q} \left[ \left(\frac {1}{T} \int_ {t} ^ {T} \frac {S _ {u}}{S _ {t}} d u - \frac {K - \frac {1}{T} \int_ {0} ^ {t} S _ {u} d u}{S _ {t}}\right) ^ {+} \Big | \mathcal {F} _ {t} \right] \\ = S _ {t} \phi (t, X _ {t}) \end{array}
$$

where $\begin{array} { r } { X _ { t } \doteq \frac { K - \frac { 1 } { T } \int _ { 0 } ^ { t } S _ { u } d u } { S _ { t } } } \end{array}$ . Applying the Itˆo lemma to $\xi _ { t } ,$ we have 

$$
d X _ {t} = - \frac {1}{T} d t + X _ {t} \left(- \sigma d W _ {t} ^ {Q} - r d t + \sigma^ {2} d t\right),
$$

and assuming that $\phi ( t , x )$ is twice diferentiable we apply the Itˆo lemma to $\phi ( t , X _ { t } )$ : 

$$
d \phi (t, X _ {t}) = \left(\frac {\partial}{\partial t} + \left(- \frac {1}{T} + X _ {t} (\sigma^ {2} - r)\right) \frac {\partial}{\partial x} + X _ {t} ^ {2} \sigma^ {2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) \phi (t, X _ {t}) d t - X _ {t} \sigma \frac {\partial}{\partial x} \phi (t, X _ {t}) d W _ {t} ^ {Q}.
$$

Then applying Itˆo’s lemma to $M _ { t }$ , we have 

$$
d M _ {t} = \phi (t, X _ {t}) d S _ {t} + S _ {t} d \phi (t, X _ {t}) + d S _ {t} \cdot d \phi (t, X _ {t})
$$

$$
= \phi (t, X _ {t}) \left(r S _ {t} d t + \sigma S _ {t} d W _ {t} ^ {Q}\right) + S _ {t} \left(\frac {\partial}{\partial t} + \left(- \frac {1}{T} + X _ {t} (\sigma^ {2} - r)\right) \frac {\partial}{\partial x} + X _ {t} ^ {2} \sigma^ {2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) \phi (t, X _ {t}) d t
$$

$$
- S _ {t} X _ {t} \sigma \frac {\partial}{\partial x} \phi (t, X _ {t}) d W _ {t} ^ {Q} - X _ {t} S _ {t} \sigma^ {2} \frac {\partial}{\partial x} \phi (t, X _ {t}) d t,
$$

and in order for $M _ { t }$ to be a martingale the dt terms must all cancel out. Therefore, we must have 

$$
r \phi (t, X _ {t}) + \left(\frac {\partial}{\partial t} - \left(\frac {1}{T} + r X _ {t}\right) \frac {\partial}{\partial x} + X _ {t} ^ {2} \sigma^ {2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) \phi (t, X _ {t}) = 0,
$$

which gives us the PDE of reduced dimension for a new function $\tilde { \phi } ( t , x ) \doteq e ^ { - r ( T - t ) } \phi ( t , x )$ 

$$
\left(\frac {\partial}{\partial t} - \left(\frac {1}{T} + r x\right) \frac {\partial}{\partial x} + x ^ {2} \sigma^ {2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) \tilde {\phi} (t, x) = 0\tag{5.3}
$$

$$
\tilde {\phi} (t, x) \Big | _ {t = T} = \max (- x, 0).\tag{5.4}
$$

The PDE of equations (5.3) and (5.4) is of reduced dimension and is solvable with a Feynman-Kac formula, 

$$
\widetilde {\phi} (t, x) = \mathbb {E} [ \max (- \widetilde {X} _ {T}, 0) | \widetilde {X} _ {t} = x ]
$$

with $\begin{array} { r } { d \widetilde { X } _ { t } = - \left( \frac { 1 } { T } + r \widetilde { X } _ { t } \right) d t + \sigma \widetilde { X } _ { t } d W _ { t } } \end{array}$ . Finally, the option price is 

$$
C (t, S _ {t}, Z _ {t}) = S _ {t} \cdot \widetilde {\phi} \left(t, \frac {K - Z _ {t}}{S _ {t}}\right) \quad \forall t \leq T.\tag{5.5}
$$

Equation (5.5) is the pricing formula of reduced dimension. 

## 5.2 Exchange Options (Margrabe Formula)

Consider two tradable assets, $S _ { t } ^ { 1 }$ and $S _ { t } ^ { 2 }$ . An exchange option with strike K has payof 

$$
\psi (S _ {T} ^ {1}, S _ {T} ^ {2}) = (S _ {T} ^ {1} - S _ {T} ^ {2} - K) ^ {+}
$$

which we price price under an EMM. In particular, for $K = 0$ we have 

$$
\begin{array}{r c l} {C (t, s _ {1}, s _ {2})} & = & {e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ (S _ {T} ^ {1} - S _ {T} ^ {2}) ^ {+} \Big | S _ {t} ^ {1} = s _ {1}, S _ {t} ^ {2} = s _ {2} \right]} \\ & = & {e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ S _ {T} ^ {2} \left(\frac {S _ {T} ^ {1}}{S _ {T} ^ {2}} - 1\right) ^ {+} \Big | S _ {t} ^ {1} = s _ {1}, S _ {t} ^ {2} = s _ {2} \right] .} \end{array}\tag{5.6}
$$

Options like this are found in forex markets and in commodities, the latter of which uses them to hedge risk in the risk between the retail price of a finished good verses the cost of manufacture. In electricity markets, the price of a megawatt hour of electricity needs to be hedged against the price of natural gas in what’s called the spark spread; in the soy market the cost of soy meal verses the cost of soy beans is called the crush spread; in the oil market the cost of refined oil products verses the cost of crude oil is called the crack spread. In commodities markets these options are called sometimes called spread options. The Margrabe formula prices spread/exchange options with $K = 0$ 

Suppose we have a double Black-Scholes model for the two assets, 

$$
\begin{array}{r c l} \frac {d S _ {t} ^ {1}}{S _ {t} ^ {1}} & = & r d t + \sigma_ {1} \left(\sqrt {1 - \rho^ {2}} d W _ {t} ^ {1} + \rho d W _ {t} ^ {2}\right) \\ \frac {d S _ {t} ^ {2}}{S _ {t} ^ {2}} & = & r d t + \sigma_ {2} d W _ {t} ^ {2} \end{array}
$$

where $W _ { t } ^ { 1 }$ and $W _ { t } ^ { 2 }$ are independent risk-neutral Brownian motions and $\rho \in ( - 1 , 1 )$ . Now we define ratio in (5.6) as 

$$
Y _ {t} \doteq \frac {S _ {t} ^ {1}}{S _ {t} ^ {2}},
$$

define an exponential martingale 

$$
Z _ {t} = \exp \left(- \frac {1}{2} \sigma_ {2} ^ {2} t + \sigma_ {2} W _ {t} ^ {2}\right),
$$

and notice that 

$$
C (t, s _ {1}, s _ {2}) = s _ {2} \mathbb {E} ^ {Q} [ Z _ {T} (Y _ {T} - 1) ^ {+} | S _ {t} ^ {1} = s _ {1}, S _ {t} ^ {2} = s _ {2} ].
$$

Recall the Girsanov Theorem from Chapter 2 and recognize that $Z _ { t }$ defines a new measure $\widetilde { \mathbb { P } } ^ { Q }$ under which $\widetilde { W } _ { t } \doteq W _ { t } ^ { 2 } - \sigma _ { 2 } t$ is Brownian motion, and under which $W _ { t } ^ { 1 }$ remains a Brownian motion independent of $\widetilde { W _ { t } }$ . Applying the Itˆo lemma to $Y _ { t }$ we get 

$$
d Y _ {t} = Y _ {t} (\sigma_ {2} ^ {2} - \sigma_ {2} \sigma_ {1} \rho) d t + Y _ {t} \sigma_ {1} \left(\sqrt {1 - \rho^ {2}} d W _ {t} ^ {1} + \rho d W _ {t} ^ {2}\right) - Y _ {t} \sigma_ {2} d W _ {t} ^ {2}
$$

$$
= Y _ {t} \sigma_ {1} \left(\sqrt {1 - \rho^ {2}} d W _ {t} ^ {1} + \rho d \widetilde {W} _ {t}\right) - Y _ {t} \sigma_ {2} d \widetilde {W} _ {t},
$$

and we can now write the option price under the new measure to get the Margrabe Formula: 

$$
C (t, s _ {1}, s _ {2}) = s _ {2} \widetilde {\mathbb {E}} ^ {Q} \left[ (Y _ {T} - 1) ^ {+} \Big | Y _ {t} = s _ {1} / s _ {2} \right]
$$

$$
= s _ {2} \widetilde {\mathbb {E}} ^ {Q} \left[ \left(\frac {s _ {1}}{s _ {2}} e ^ {- \frac {1}{2} \left(\sigma_ {1} ^ {2} + \sigma_ {2} ^ {2} - 2 \sigma_ {2} \sigma_ {1} \rho\right) (T - t) + \sigma_ {1} \left(\sqrt {1 - \rho^ {2}} (W _ {T} ^ {1} - W _ {t} ^ {2}) + \rho (\widetilde {W} _ {T} - \widetilde {W} _ {t})\right) - \sigma_ {2} (\widetilde {W} _ {T} - \widetilde {W} _ {t})} - 1\right) ^ {+} \Big | Y _ {t} = s _ {1} / s _ {2} \right]
$$

$$
= s _ {1} N (d _ {1}) - s _ {2} N (d _ {2})
$$

where $N ( \cdot )$ is the standard normal CDF function and 

$$
\begin{array}{l} d _ {1} = \frac {\log (s _ {1} / s _ {2}) + \frac {1}{2} \sigma^ {2} (T - t)}{\sigma \sqrt {T - t}} \\ d _ {2} = d _ {1} - \sigma \sqrt {T - t}, \end{array}
$$

where $\sigma ^ { 2 } = \sigma _ { 1 } ^ { 2 } + \sigma _ { 2 } ^ { 2 } - 2 \sigma _ { 2 } \sigma _ { 1 } \rho$ . Essentially, the Margrabe formula is the Black-Scholes call option price with $r = 0 , S _ { 0 } = s _ { 1 } , K = s _ { 2 }$ , and $\sigma ^ { 2 } = \sigma _ { 1 } ^ { 2 } + \sigma _ { 2 } ^ { 2 } - 2 \sigma _ { 2 } \sigma _ { 1 } \rho .$ 

## 5.3 American Options and Optimality of Early Exercise

Broadly speaking, options on index funds (such as S&P 500) are European, whereas options on individual stocks (such as Apple) are American. American options have the same features as their European counterparts, but with the additional option of early exercise. The option of early exercise can be equated with the option to wait and see, as the prices of these options is usually thought of the present value of the payof when exercised at an optimal time. For this reason the American options are consider path-dependent. Methods for pricing American options are quite involved, as there are no explicit solutions. Instead, pricing is done by working backward from the terminal condition on a binomial tree, or by solving a PDE with a free boundary. Pricing methods are not covered here; these notes focus on some fundamental facts about American options. 

The first thing to notice is that an American option is worth at least as much as a European. Hence, the prices are such that 

American Option = European Option + value of right to early exercise 

## ≥ European Option.

In particular, we will that an American put has positive value for the right to early exercise, and so does the American call when the underlying asset pays dividend. 

American Call Option. Let $C _ { t } ^ { A }$ denote the price of an American call option with strike K and maturity T. At any time $t \leq T$ we obviously must have $C _ { t } ^ { A } > S _ { t } - K$ , otherwise there is an arbitrage opportunity by buying the option and exercising immediately for a risk-less profit. Therefore, we can write 

$$
C _ {t} ^ {A} = \max \left(S _ {t} - K, C _ {t} ^ {c o n t}\right)
$$

where $C _ { t } ^ { c o n t }$ is the continuation value of the option at time $t ;$ at time $t \leq T$ the price is determined by whether or not it is optimal to exercise. Letting $C _ { t } ^ { E }$ denote the price of the European call, it is clear that the long party cannot lose anything by having the option to exercise early (provided they do so at a good time) and so 

$$
C _ {t} ^ {A} = \max \left(S _ {t} - K, C _ {t} ^ {c o n t}\right) \geq C _ {t} ^ {E}.
$$

Proposition 5.3.1. For an American call option on a non-dividend paying asset, it is never optimal to exercise early. Hence, American and European calls have the same price and 

$$
C _ {t} ^ {A} = C _ {t} ^ {c o n t} = C _ {t} ^ {E}.
$$

Proof. The proof follows from the European Put-Call parity and is simple. Early exercise is clearly not optimal if $S _ { t } < K$ . Now suppose that $S _ { t } > K$ . Letting $P ^ { E }$ denote the price of a European put option, we have 

$$
C _ {t} ^ {A} = \max \left(S _ {t} - K, C _ {t} ^ {c o n t}\right) \geq C _ {t} ^ {E} = P _ {t} ^ {E} + S _ {t} - K e ^ {- r (T - t)} > S _ {t} - K = \text { value   of   early   exercise },
$$

which proves the continuation value is worth more than early exercise, and the result follows. □ 

To illustrate this proposition consider the following scenario: Suppose you’re long an ITM American call, and you have a strong feeling that the asset price will go down and leave the option OTM. In this case you should not exercise but should short the asset and use the call to cover your short position. For example, suppose the asset is trading at $105, you’re long a 3 month American call with $K = \$ 100$ , and the risk-free rate is 5%. Now compare the following two strategies: 

1. Exercise the option and invest the proceeds: 

• Pay $K = \$ 100;$ sell the asset at $105. 

• Invest proceeds of $5 in bond. 

• In three months have $5.06. 

2. Short the asset, hold the option, and invest the proceeds: 

• Short the asset at $105. 

• Invest the proceeds of $105 in bond. 

• In three months have $106.32 in the bank; owe no more than $100 to cover your short position. 

From these two strategies it is clear that early exercise is sub-optimal, as the latter strategy has at least an edge of $1.32. Alternatively, one could simply sell the call, which will also be better than exercising early. 

The introduction of dividends changes things. In particular, early exercise can be optimal if the present value of the dividends is worth more than the interest earned on the strike and the time value of the option. We see this from the put-call parity 

$$
C _ {t} ^ {A} \geq C _ {t} ^ {E} = P _ {t} ^ {E} + S _ {t} - K e ^ {- r (T - t)} - P V _ {t} (D)
$$

where $P V _ { t } ( D )$ is the present value of dividends received during the life of the option. For European options, dividends can be expressed in terms of a yield, $\delta \geq 0$ , so that $P V _ { t } ( D ) = S _ { t } ( 1 - e ^ { - \delta ( T - t ) } )$ and 

$$
C _ {t} ^ {A} \geq C _ {t} ^ {E} = P _ {t} ^ {E} + S _ {t} e ^ {- \delta (T - t)} - K e ^ {- r (T - t)}.
$$

It may be optimal to exercise early if $C _ { t } ^ { E } < S _ { t } - K$ , which is possible in the presence of dividends as we can see in Figure 5.1. The intuition for this figure is that $P _ { t } ^ { E } \to 0$ as $S _ { t }  \infty$ , and that $C _ { t } ^ { E } \sim S _ { t } e ^ { - \delta ( T - t ) } - K e ^ { - r ( T - t ) } < S _ { t } - K$ for $S _ { t }$ big enough. This only proves that the option for early exercise has positive value, therefore implying that early exercise may be optimal at some point; it does not mean that one should exercise their American option right now. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/6532727047f878cc74aa0b09e9bcb6b3803e679773fee07c035f7e916c511447.jpg)



Figure 5.1: The Black-Scholes price of a European call option on a dividend paying asset, with $K = 5 0$ $T - t = 3 / 1 2 .$ $r = . 0 2$ $\sigma = . 2 .$ , and $\delta = . 0 5$ . Notice that early exercise exceeds the European price for high-enough price in the underlying.


Proposition 5.3.2. For an American call option on a dividend-paying asset, it may be optimal to exercise early. 

Proof. Let $\delta > 0$ be the dividend rate and assume $r > 0$ . From the put-call parity, 

$$
C _ {t} ^ {A} \geq C _ {t} ^ {E} = P _ {t} ^ {E} + S _ {t} e ^ {- \delta (T - t)} - K e ^ {- r (T - t)} = P _ {t} ^ {E} + e ^ {- r (T - t)} \left(e ^ {- (\delta - r) (T - t)} S _ {t} - K\right).
$$

Now suppose that $\delta , r , K$ and S are such that 

$$
C _ {t} ^ {E} <   S _ {t} - K.
$$

Clearly, $C _ { t } ^ { A } \geq S _ { t } - K$ , and so in this case we have strict inequality $C _ { t } ^ { A } > C _ { t } ^ { E }$ , which indicates the early exercise of the American option adds value, and hence early exercise can be optimal if done at the correct time. □ 

In practice, dividends are paid at discrete times, and early exercise of an American options should only occur immediately prior to the time of dividend payment. The intuition is similar to the non-dividend case: at non-dividend times it is optimal to wait; time value of strike amount in bank and the right to exercise are more valuable. 

American Put Option. Regardless of dividends, early exercise of an American put option may be optimal. To understand why, simply consider a portfolio consisting of an American put with strike $K > 0$ and a single contract in the underlying. If the underlying hits zero, then it is certainly optimal to exercise. In general, early exercise of a put option will be optimal if the price drops low enough to where the time value of the strike amount in the bank account is worth more than the option to wait on selling the asset plus the present value of any dividends that might be recieved. 

Proposition 5.3.3. Early exercise of an American put option may be optimal if $r > 0$ 

Proof. By contradiction. Suppose it is never optimal to exercise an American put. Then 

$$
P _ {t} ^ {A} = \max \left(K - S _ {t}, P _ {t} ^ {c o n t}\right) = P _ {t} ^ {c o n t} = P _ {t} ^ {E}
$$

where $P _ { t } ^ { c o n t }$ is the continuation value of the option and $P _ { t } ^ { E }$ is the price of a European put. Recall Figure 4.3 on page 37 of Section 4, where we see that 

$$
P _ {t} ^ {E} \to e ^ {- r (T - t)} K \qquad \mathrm{as} S _ {t} \searrow 0.
$$

If $r > 0$ there is a price $S _ { t } ^ { 0 } > 0$ such that $P _ { t } ^ { E } < K - S _ { t }$ for all $S _ { t } ~ < ~ S _ { t } ^ { 0 }$ , which is a contradiction. Hence, early exercise can be optimal. □ 

Proposition 5.3.3 is valid regardless of whether or not there are dividends, but the time value of dividends will counterbalance the time value of the cash received from exercise. If $r = 0$ , then the European put option is always greater or equal to its intrinsic value, which means 

$$
K - S _ {t} \leq P _ {t} ^ {E} \leq P _ {t} ^ {A} = \max \left(K - S _ {t}, P _ {t} ^ {c o n t}\right),
$$

with strict inequality between $K - S _ { t }$ and $P _ { t } ^ { E }$ if $S _ { t } > 0$ . Hence, if $\mathbb { P } ( S _ { t } > 0 ) = 1$ , then $\mathbb { P } ( P _ { t } ^ { A } = P _ { t } ^ { c o n t } ) = 1$ and early exercise is never optimal. Joke: Therefore, the Fed should drop interest rates if they are worried about rampant sell-ofs by option holders. 

To summarize, American options have three components beyond their intrinsic value, 

• value of option to early exercise (always positive impact on price), 

• time value of money (positive for calls, negative for puts), 

• dividends (negative for calls, positive for puts). 

The value of an American option over the price of a European option is essentially the value of early exercise. While the above results are model-free, the price (and the optimal exercise boundary) will be model-dependent. 

## 5.4 Bermuda Options

A Bermuda call option has two exercise times $T _ { 1 }$ and $T _ { 2 }$ with 

$$
0 <   T _ {1} <   T _ {2} <   \infty .
$$

At time $T _ { 1 }$ the holder of the option has the right to exercise a call with strike $K _ { 1 }$ , or to continue with the possibility to exercise at time $T _ { 2 }$ with exercise $K _ { 2 }$ . Hence, the risk-neutral price is 

$$
C ^ {B} (t) = \left\{ \begin{array}{l l} e ^ {- r (T _ {1} - t)} \mathbb {E} ^ {Q} \left[ \max (S _ {T _ {1}} - K _ {1}, C ^ {E} (T _ {1})) \Big | \mathcal {F} _ {t} \right] & \text { for } t \leq T _ {1} , \\ C ^ {E} (t) & \text { for } T _ {1} <   t \leq T _ {2} , \end{array} \right.
$$

where $C ^ { E } ( t )$ is price a European call option with strike $K _ { 2 }$ and maturity $T _ { 2 }$ . 

Consider the Black-Scholes model, 

$$
\frac {d S _ {t}}{S _ {t}} = (r - q) d t + \sigma d W _ {t} ^ {Q},
$$

where $q$ is the dividend rate. Recalling the Black-Scholes price for a call on a dividendpaying asset (see Section 3.7 of Chapter 3), the time- ${ \bf \nabla } \cdot { T _ { 1 } }$ payof for the Bermuda call option is 

$$
\psi (s) = \max \left(s - K _ {1}, s e ^ {- q (T _ {2} - T _ {1})} N (d _ {1}) - K e ^ {- r (T - t)} N (d _ {2})\right),
$$

where 

$$
\begin{array}{l} d _ {1} = \frac {\log (s / K _ {2}) + (r - q + . 5 \sigma^ {2}) (T _ {2} - T _ {1})}{\sigma \sqrt {T _ {2} - T _ {1}}} \\ d _ {2} = d _ {1} - \sigma \sqrt {T _ {2} - T _ {1}}. \end{array}
$$

It follows that for $t < T _ { 1 }$ that the Bermuda option price $C ^ { B } ( t , s )$ is given by the PDE 

$$
\begin{array}{r} \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} s ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + (r - q) s \frac {\partial}{\partial s} - r\right) C ^ {B} (t, s) = 0 \\ C ^ {B} (T _ {1}, s) = \psi (s). \end{array}
$$

When pricing the Bermuda option is intuitive to think about the appropriate early-exercise rule. We learned from Section 5.3 that it is never optimal to exercise at time $T _ { 1 } { \mathrm { ~ i f ~ } } q = 0$ However if $q > 0$ then we need to think of a rule for when to exercise. The rule turns out to be simple: find the optimal value $s ^ { e }$ such that at time $t = T _ { 1 }$ 1, 

$$
\begin{array}{l} \text {exercise if S_{T_{1}} \geq s^{e} ,} \\ \text {do not if S_{T_{1}} <  s^{e} .} \end{array}
$$

In the next subsection we consider the American put, where there will be a time-dependent exercise rule. 

## 5.5 Free-Boundary Problem for the American Put

Consider the Black-Scholes model, 

$$
\frac {d S _ {t}}{S _ {t}} = r d t + \sigma d W _ {t} ^ {Q},
$$

with $r > 0$ . In this case it may be optimal exercise early an American put. The price $P ^ { A }$ of the put is the solution to an optimization problem, 

$$
P ^ {A} (t, s) = \sup _ {\tau \geq t} \mathbb {E} ^ {Q} \left[ e ^ {- r (T \wedge \tau - t)} (K - S _ {\tau \wedge T}) ^ {+} \Big | S _ {t} = s \right],
$$

where the $\tau$ is the optional exercise time chosen by the holder, and $T \wedge \tau = \operatorname* { m i n } ( T , \tau )$ Define $\mathcal { L }$ to be the PDE operator, 

$$
\mathcal {L} = \frac {\partial}{\partial t} + \frac {\sigma^ {2} s ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + r s \frac {\partial}{\partial s} - r.
$$

If at time t it is optimal to continue then $\begin{array} { r } { \mathcal { L } P ^ { A } ( t , S _ { t } ) = 0 ; } \end{array}$ if it is optimal to exercise then $\mathcal { L } P ^ { A } ( t , S _ { t } ) = \mathcal { L } ( K - S _ { t } ) < 0$ and $\begin{array} { r } { \frac { \partial } { \partial s } P ^ { A } ( t , S _ { t } ) = - 1 } \end{array}$ . This is equivalent to finding the pair $( P ^ { A } , s ^ { e } )$ such that 

$$
\begin{array}{c} {\mathcal {L} P ^ {A} (t, s) = 0 \mathrm{for} t <   T \mathrm{and} s > s ^ {e} (t),} \\ {P ^ {A} (T, s) = (K - s) ^ {+}} \\ {\frac {\partial}{\partial s} P ^ {A} (t, s ^ {e} (t)) = - 1 \mathrm{for} t \leq T.} \end{array}
$$

This is the so-called free boundary problem, which refers to the fact that we need to solve for the boundary $s ^ { e } ( t )$ and the PDE’s solution $P ^ { A } ( t , s )$ . A straight-forward way to solve this PDE and to see the boundary is with a backward recursion on a binomial tree. 

# Implied Volatility & Local-Volatility Fits

A major point of discuss with Black-Scholes pricing is the role of volatility. The questions comes about when the Black-Scholes formula is inverted on the market’s option prices, which produces an interesting phenomenon known as the implied volatility smile, smirk, or skew. The implied volatility suggests that asset prices are more complex than geometric Brownian motion, and the Black-Scholes’ parameter σ needs to be dynamic. Local volatility models and stochastic volatility models are two well-known ways to address this issue; jump-difusion models and time-change jump models are also a popular choice of model. 

## 6.1 Implied Volatility

Implied volatility is the parameter estimate obtained by inverting the Black-Scholes model on market data. The interesting part is that European call and put options will return a diferent parameter for diferent strikes and maturity. Let $C ^ { B S } ( t , s , k , T , \sigma )$ be the Black-Scholes price of a call option with strike K and maturity T, and let $C _ { t } ^ { d a t a } ( K , T )$ be the price in the market. 

Definition 6.1.1. Implied Volatility is the quantity $\hat { \sigma } ( K , T ) > 0$ such that 

$$
C _ {t} ^ {d a t a} (K, T) = C ^ {B S} \left(t, S _ {t}, K, T, \hat {\sigma} (K, T)\right).
$$

Traders often quote option prices in implied volatility, probably because it is a ‘unit-less’ measure of risk. Typically, the implied smile/skew is plotted as a function of the option’s strike as shown in Figure 6.1. When plotting implied volatility, the term ‘Moneyness’ refers to how far the option is in-the-money (ITM) or out-of-the-money (OTM). Moneyness can also be interpreted as a unit-less measure, for instance the log-moneyness, 

$$
\mathrm{log-moneyess} = \log (K e ^ {- r (T - t)} / S _ {t}).
$$

Implied volatility is skewed to the left for many assets, but some assets (such as forex contracts) have a right skew (see Figure 6.2). The interpretation is the followoing: implied volatility smile/skew suggests that Black-Scholes is an oversimplification, and the left skew of equity options (such as the SPX ETF options) suggests there is ‘crash-o-phobia’ for long positions in the underlying, and long put options are an insurance item for which there is a premium in the market. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/daf4949a8b40414677efb42fd063d1a69c6363fa8163c1984dac5afcd4bd4132.jpg)



Figure 6.1: Implied Volatility Skew of SPX Index Options. On May 20th, 2010, the S&P 500 closed at 1072, so moneyness refers to something close to the intrinsic value.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/8c72e4d06ebcea2210778eae8a2cf609b29283ccd54e1d26a0a494e893ff39f7.jpg)



Figure 6.2: The implied volatility smile for options on the Euro/Yen currency exchange. Notice the skew is to the right.


Bounds on Implied Volatility. There are some bounds on implied volatility that can obtained from the Black-Scholes formula. 

Proposition 6.1.1. Changes in implied volatility have bounding inequalities 

$$
- \frac {e ^ {- r (T - t)} N (- d _ {2})}{S _ {t} \sqrt {T - t} N ^ {\prime} (d _ {1})} \leq \frac {\partial}{\partial K} \hat {\sigma} (K, T) \leq \frac {e ^ {- r (T - t)} N (d _ {2})}{S _ {t} \sqrt {T - t} N ^ {\prime} (d _ {1})}
$$

where $d _ { 1 }$ and $d _ { 2 }$ are given by the Black-Scholes formula and are functions $o f \hat { \sigma }$ 

The derivation of Proposition 6.1.1 is as follows: 

For the call option, 

$$
\frac {\partial}{\partial K} C _ {t} ^ {d a t a} (K) = C _ {k} ^ {B S _ {1}} (t, S _ {t}, K, T, \hat {\sigma} (K, T))
$$

$$
+ C _ {\sigma} ^ {B S} (t, S _ {t}, K, T, \hat {\sigma} (K, T)) \frac {\partial}{\partial K} \hat {\sigma} (K, T) \leq 0,
$$

hence 

$$
\begin{array}{c} \frac {\partial}{\partial K} \hat {\sigma} (K, T) \leq - \frac {C _ {k} ^ {B S _ {1}} (t , S _ {t} , K , T , \hat {\sigma} (K , T))}{C _ {\sigma} ^ {B S} (t , S _ {t} , K , T , \hat {\sigma} (K , T))} \\ = \frac {e ^ {- r (T - t)} N (d _ {2})}{S _ {t} \sqrt {T - t} N ^ {\prime} (d _ {1})}, \end{array}\tag{6.1}
$$

where it is straight forward to verify the K-derivative to be 

$$
C _ {k} ^ {B S _ {1}} = \frac {\partial}{\partial K} \left(S _ {t} N (d _ {1}) - K e ^ {- r (T - t)} N (d _ {2})\right) = - N (d _ {2}).
$$

The ratio in (6.1) has the Greek letter vega in the denominator, which causes it to blow-up when K is far-from-the-money, hence the estimate will be more useful for neat-the-money options (see Figure 6.3). A similar inequality is derived from the put option, 

$$
- \frac {e ^ {- r (T - t)} N (- d _ {2})}{S _ {t} \sqrt {T - t} N ^ {\prime} (d _ {1})} \leq \frac {\partial}{\partial K} \hat {\sigma} (K, T) .
$$

This growth bound is also shown in Figure 6.3. 

Another important bound on implied volatility is the moment formula for options with extreme strike. Let $x ( K ) = \log ( K e ^ { - r ( T - t ) } / S t )$ . There exists $x ^ { * } > 0$ such that 

$$
\hat {\sigma} (K, T) <   \sqrt {\frac {2}{T - t} | x (K) |}\tag{6.2}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/2292e78730335eb374d62a8a7f185dba653dff5fb717859fd3edb9831623e309.jpg)



Figure 6.3: The growth bound on an option with underlying price $S _ { t } = 5 0$ , time to maturity $T - t = 3 / 1 3$ , interest rate $r = 0$ , and implied volatility $\hat { \sigma } = . 2 .$ . For an ATM option, the bounds of proposition 6.1.1 show that derivative of implied volatility with respect to strike to be bounded by about 5%.


for all K s.t. $| x ( K ) | > x ^ { * }$ . The power of this estimate is that it provides a model-free bound on implied volatility. In other words, it extrapolates the implied volatility smile without assuming any particular structure of the probability distribution. The upper bound in (6.2) can be sharpened to the point where there is uncovered a relationship between implied volatility and the number of finite moments of the underlying $S _ { T }$ 

Proposition 6.1.2. (The Moment Formula for Large Strike). Let 

$$
\bar {p} = \sup \{p: \mathbb {E} ^ {Q} S _ {T} ^ {1 + p} <   \infty \},
$$

and let 

$$
\beta_ {R} = \limsup _ {K \to \infty} \frac {\hat {\sigma} ^ {2} (K , T)}{| x (K) | / T} .
$$

Then $\beta _ { R } \in [ 0 , 2 ]$ and 

$$
\bar {p} = \frac {1}{2 \beta_ {R}} + \frac {\beta_ {R}}{8} - \frac {1}{2},
$$

where $1 / 0 \dot { = } \infty$ . Equivalently, 

$$
\beta_ {R} = 2 - 4 (\sqrt {\bar {p} ^ {2} + \bar {p}} - \bar {p})
$$

where the right-hand side is taken to be zero when $\bar { p } = \infty$ 

There is also a moment formula for extremely small strikes and $\bar { q } = \operatorname* { s u p } \{ q : \mathbb { E } ^ { Q } S _ { T } ^ { - q } <$ $\infty \}$ . Both moment formulas are powerful because they are model-free, and because they say that tail behavior of the underlying can be characterized by implied volatility’s growth rate against log-moneyness. Indeed, an asset with heavy tails will have higher implied volatility, and so going long or short an option will have more risk, and hence these options will cost more. The important details of the moment formula(s) are in the original paper of Roger Lee [Lee, 2004]. 

## 6.2 Local Volatility Function

The idea the volatility is non-constant was first implemented in local volatility models. A local volatility model is a simple extension of Black-Scholes 

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma (t, S _ {t}) d W _ {t}
$$

where the function $\boldsymbol { \sigma } ( t , s )$ is chosen to fit the implied volatility smile. Dependence of σ on $S _ { t }$ does not efect completeness of market, so there is a pricing PDE that is try similar to the Black-Scholes and is derived in much the same way: 

$$
\left(\frac {\partial}{\partial t} + \frac {S _ {t} ^ {2} \sigma^ {2} (t , S _ {t})}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + r S _ {t} \frac {\partial}{\partial s} - r\right) C (t, S _ {t}) = 0\tag{6.3}
$$

with terminal condition $C | _ { t = T } = ( s - K ) ^ { + }$ . Hence, the Feynmann-Kac formula applies and we have 

$$
C (t, s) = e ^ {- r (T - t)} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ]
$$

where $\mathbb { E } ^ { Q }$ is a risk-neutral measure under which $\begin{array} { r } { \frac { d S _ { t } } { S _ { t } } = r d t + \sigma ( t , S _ { t } ) d W _ { t } ^ { Q } } \end{array}$ . Now, observe the following facts: 

1. The first derivative with respect to K is written with a CDF, 

$$
\begin{array}{r l} & {\frac {\partial}{\partial K} C (t, s) = e ^ {- r (T - t)} \frac {\partial}{\partial K} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ]} \\ & {\qquad = e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ \frac {\partial}{\partial K} (S _ {T} - K) ^ {+} \Big | S _ {t} = s \right]} \\ & {\qquad = - e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ \mathbb {1} _ {[ S _ {T} \geq K ]} \Big | S _ {t} = s \right]} \\ & {\qquad = - e ^ {- r (T - t)} \mathbb {Q} (S _ {T} > K | S _ {t} = s)} \\ & {\qquad = - e ^ {- r (T - t)} \left(1 - \mathbb {Q} (S _ {T} \leq K | S _ {t} = s)\right).} \end{array}
$$

2. The second derivative with respect to $K$ is a PDF, 

$$
\begin{array}{r l} & {\frac {\partial^ {2}}{\partial K ^ {2}} C (t, s) = e ^ {- r (T - t)} \frac {\partial^ {2}}{\partial K ^ {2}} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ]} \\ & {\qquad = - e ^ {- r (T - t)} \frac {\partial}{\partial K} \left(1 - \mathbb {Q} (S _ {T} \leq K | S _ {t} = s)\right)} \\ & {\qquad = e ^ {- r (T - t)} \frac {\partial}{\partial K} \mathbb {Q} (S _ {T} \leq K | S _ {t} = s),} \end{array}
$$

which is commonly referred to as the Breeden and Litzenberger formula. 

3. Finally, denote by $C ( t , s , k )$ all the list call options with strike $T$ and strikes k ranging from zero to infinity. For a fixed $K > 0$ , diferentiating with respect to $T$ and repeated application of integration-by-parts yields the following 

$$
\begin{array}{r l} & {\frac {\partial}{\partial T} C (t, s, K)} \\ & {= \frac {\partial}{\partial T} \left(e ^ {- r (T - t)} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ]\right)} \\ & {= - r e ^ {- r (T - t)} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ] + e ^ {- r (T - t)} \frac {\partial}{\partial T} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ]} \\ & {= - r e ^ {- r (T - t)} \mathbb {E} ^ {Q} \{(S _ {T} - K) ^ {+} | S _ {t} = s \}} \\ & {\quad + e ^ {- r (T - t)} \frac {\partial}{\partial T} \mathbb {E} ^ {Q} \left[ (s - K) ^ {+} + \int_ {t} ^ {T} \left(r S _ {u} \mathbb {1} _ {[ S _ {u} \geq K ]} + \frac {\sigma^ {2} (u , S _ {u}) S _ {u} ^ {2}}{2} \delta_ {K} (S _ {u})\right) d u \Big | S _ {t} = s \right]} \\ & {\quad + e ^ {- r (T - t)} \frac {\partial}{\partial T} \underbrace {\mathbb {E} ^ {Q} \left[ \int_ {t} ^ {T} \sigma (u , S _ {u}) S _ {u} \mathbb {1} _ {[ S _ {u} \geq K ]} d W _ {u} ^ {Q} \Big | S _ {t} = s \right]} _ {= 0}} \\ & {= - r e ^ {- r (T - t)} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ]} \\ & {\quad + e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ r S _ {T} \mathbb {1} _ {[ S _ {T} \geq K ]} + \frac {\sigma^ {2} (T , S _ {T}) S _ {T} ^ {2}}{2} \delta_ {K} (S _ {T}) \Big | S _ {t} = s \right]} \\ & {= r K e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ \mathbb {1} _ {[ S _ {T} \geq K ]} + \frac {\sigma^ {2} (T , S _ {T}) S _ {T} ^ {2}}{2} \delta_ {K} (S _ {T}) \Big | S _ {t} = s \right]} \\ & {= r K \int_ {0} ^ {\infty} \mathbb {1} _ {[ k \geq K ]} \frac {\partial^ {2}}{\partial k ^ {2}} C (t, s, k) d k + \int_ {0} ^ {\infty} \frac {\sigma^ {2} (T , k) k ^ {2}}{2} \delta_ {K} (k) \frac {\partial^ {2}}{\partial k ^ {2}} C (t, s, k) d k} \\ & {= - r K \frac {\partial}{\partial K} C (t, s, K) + \frac {\sigma^ {2} (T , K) K ^ {2}}{2} \frac {\partial^ {2}}{\partial K ^ {2}} C (t, s, K).} \end{array}
$$

The above steps 1 through 3 have derived what is known in financial literature as Dupire’s Equation: 

$$
\left(\frac {\partial}{\partial T} - \frac {K ^ {2} \sigma^ {2} (T , K)}{2} \frac {\partial^ {2}}{\partial K ^ {2}} + r K \frac {\partial}{\partial K}\right) C (t, s, K) = 0\tag{6.4}
$$

with initial condition $C ( t , s , K ) | _ { T = t } = ( s - K ) ^ { + }$ . From (6.4) we get the Dupire scheme for implied local volatility: 

$$
I ^ {2} (T, K) = 2 \frac {\left(\frac {\partial}{\partial T} + r K \frac {\partial}{\partial K}\right) C}{K ^ {2} \frac {\partial^ {2}}{\partial K ^ {2}} C}\tag{6.5}
$$

which can be fit to the market’s options data for various $T ^ { \prime } \varepsilon$ s and $K \mathrm { { s } }$ (see [Dupire, 1994]). This is called ‘calibration of the implied volatility surface’, although methods for calibrating local volatility can be quite complicated with numerical diferentiation schemes in T and $K$ , regularization constraints, etc (for more on fitting techniques see $[ \mathrm { A }$ chdou and Pironneau, 2005]). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/8a6505eef01e41de939db430bd63d0ebab6e592676552d23ef00388198b493ca.jpg)



Figure 6.4: Implied Volatility Surface


Shortcomings of Local Volatility. There are some shortcomings of local volatility, one of which is the time dependence or ‘little $t ^ { \prime }$ efects, which refers to changes in the calibrated surface with time. In other words, the volatility surface will change from day to day, a phenomenon that is inconsistent with $\Delta \cdot$ -hedging arguments for local volatility. 

## 6.3 Fitting the Local Volatility Function

Define the log moneyness $k = \log ( K / S _ { t } e ^ { r ( T - t ) } )$ , and the time-weighted implied volatility 

$$
\omega (T, k) = \hat {\sigma} ^ {2} \left(T, S _ {t} e ^ {r (T - t)} e ^ {k}\right) (T - t).
$$

It is straight forward to verify that the call-option price can be written with a dimensional version of Black-Scholes formula, 

$$
\begin{array}{r l} & C (t, s, K) = e ^ {- r (T - t)} \mathbb {E} ^ {Q} [ (S _ {T} - K) ^ {+} | S _ {t} = s ] \\ & \qquad = s C ^ {B S _ {1}} (\omega (T, k), k) \\ & \qquad = s (N (d _ {1}) - e ^ {k} N (d _ {2})) , \end{array}
$$

where $C ^ { B S _ { 1 } } ( \omega , \boldsymbol { k } )$ is the Black-Scholes call-option price $S _ { t } = 1$ , time to maturity $T - t = 1$ strike $e ^ { k }$ , interest rate $r = 0$ , initial asset price $S _ { t } = 1$ , and volatility ${ \sqrt { \omega } } ;$ the formula parameters are $d _ { 1 } = - k / \sqrt { \omega } + \sqrt { \omega } / 2$ and $d _ { 2 } = d _ { 1 } - \sqrt { \omega }$ . The dimensionless option price $C ^ { B S _ { 1 } } ( \omega , \boldsymbol { k } )$ takes only log moneyness and time-weight volatility, and then the market’s option price is proportional to the dimensionless price. 

Now, there are the following derivatives, 

$$
\begin{array}{c} \frac {1}{s} \frac {\partial}{\partial T} C (t, s, K) = C _ {k} ^ {B S _ {1}} (\omega (T, k), k) \frac {\partial k}{\partial T} + C _ {\omega} ^ {B S _ {1}} (\omega (T, k), k) \frac {\partial \omega (T , k)}{\partial T} \\ = - r C _ {k} ^ {B S _ {1}} (\omega (T, k), k) + C _ {\omega} ^ {B S _ {1}} (\omega (T, k), k)   (\omega_ {T} (T, k) - r \omega_ {k} (T, k)) \end{array}\tag{6.6}
$$

$$
\begin{array}{c} \frac {1}{s} \frac {\partial}{\partial K} C (t, s, K) = C _ {k} ^ {B S _ {1}} (\omega (T, k), k) \frac {\partial k}{\partial K} + C _ {\omega} ^ {B S _ {1}} (\omega (T, k), k) \frac {\partial \omega (T , k)}{\partial k} \frac {\partial k}{\partial K} \\ = \frac {1}{K} C _ {k} ^ {B S _ {1}} (\omega (T, k), k) + \frac {1}{K} C _ {\omega} ^ {B S} (\omega (T, k), k) \omega_ {k} (T, k) \end{array}\tag{6.7}
$$

$$
\begin{array}{c} \frac {1}{s} \frac {\partial^ {2}}{\partial K ^ {2}} C (t, s, K) = \frac {\partial^ {2}}{\partial k ^ {2}} C ^ {B S _ {1}} (\omega (T, k), k) \left(\frac {\partial k}{\partial K}\right) ^ {2} + \frac {\partial}{\partial k} C ^ {B S _ {1}} (\omega (T, k), k) \frac {\partial^ {2} k}{\partial K ^ {2}} \\ = \frac {1}{K ^ {2}} \left(\frac {\partial^ {2}}{\partial k ^ {2}} C ^ {B S} (\omega (T, k), k) - C _ {k} ^ {B S _ {1}} (\omega (T, k), k)\right). \end{array}\tag{6.8}
$$

Plugging (6.6), (6.7), and (6.8) into the implied local volatility function of (6.5) yields 

$$
\sigma^ {2} \left(t, S _ {t} e ^ {r (T - t)} e ^ {k}\right) = 2 \frac {C _ {\omega} ^ {B S _ {1}} (\omega (T , k) , k) \omega_ {T} (T , k)}{\frac {\partial^ {2}}{\partial k ^ {2}} C ^ {B S _ {1}} (\omega (T , k) , k) - \frac {\partial}{\partial k} C ^ {B S _ {1}} (\omega (T , k) , k)} .\tag{6.9}
$$

The denominator in (6.9) involves the following three derivatives: 

$$
C _ {\omega \omega} ^ {B S _ {1}} (\omega , k) = \left(- \frac {1}{8} - \frac {1}{2 \omega} + \frac {k ^ {2}}{2 \omega^ {2}}\right) C _ {\omega} ^ {B S _ {1}} (\omega , k)\tag{6.10}
$$

$$
C _ {\omega k} ^ {B S _ {1}} (\omega , k) = \left(\frac {1}{2} - \frac {k}{\omega}\right) C _ {\omega} ^ {B S _ {1}} (\omega , k)\tag{6.11}
$$

$$
C _ {k k} ^ {B S _ {1}} (\omega , k) - C _ {k} ^ {B S _ {1}} (\omega , k) = 2 C _ {\omega} ^ {B S _ {1}} (\omega , k).\tag{6.12}
$$

Using (6.10), (6.11) and (6.12), the denominator in (6.9) becomes 

$$
\begin{array}{l} \frac {\partial^ {2}}{\partial k ^ {2}} C ^ {B S _ {1}} (\omega (T, k), k) - \frac {\partial}{\partial k} C ^ {B S _ {1}} (\omega (T, k), k) \\ = C _ {\omega \omega} ^ {B S _ {1}} (\omega (T, k), k) (\omega_ {k} (T, k)) ^ {2} + C _ {\omega} ^ {B S _ {1}} (\omega (T, k), k) w _ {k k} (T, k) + 2 C _ {\omega k} ^ {B S _ {1}} (\omega (T, k), k) \omega_ {k} (T, k) \\ \quad + C _ {k k} ^ {B S _ {1}} (\omega (T, k), k) - C _ {\omega} ^ {B S _ {1}} (\omega (T, k), k) \omega_ {k} (T, k) - C _ {k} ^ {B S _ {1}} (\omega (T, k), k) \\ = \left\{\left(- \frac {1}{8} - \frac {1}{2 \omega} + \frac {k ^ {2}}{2 \omega^ {2}}\right) (\omega_ {k} (T, k)) ^ {2} + w _ {k k} (T, k) - \frac {2 k}{\omega} \omega_ {k} (T, k) + 2 \right\} C _ {\omega} ^ {B S _ {1}} (\omega (T, k), k)  , \end{array}
$$

which we then plug into (6.9) to get the following implied local volatility formula in terms of the implied volatility surface: 

$$
\begin{array}{l} \sigma^ {2} (T, K) \\ = \frac {\omega_ {T} (T , k)}{1 - \frac {k}{\omega (T , k)} \omega_ {k} (T , k) + \frac {1}{4} \left(- \frac {1}{4} - \frac {1}{\omega (T , k)} + \frac {k ^ {2}}{\omega^ {2} (T , k)}\right) (\omega_ {k} (T , k)) ^ {2} + \frac {1}{2} \omega_ {k k} (T , k)}. \end{array}\tag{6.13}
$$

## 6.4 Surface Parameterizations

Given the formula in (6.13), it remains to decide on a diferentiable model for $\omega ( T , k )$ . One approach is to find a parametric function $f ^ { \theta } ( T , k )$ to fit the implied volatility surface. If the function is once diferentiable in $T$ and twice in $k ,$ then the chain rule can be applied to obtain the derivatives in the (6.13). 

Let $\theta$ be a vector of parameters fit to the weighted surface, 

$$
\min _ {\theta} \sum_ {T, k} \left| f ^ {\theta} (T, k) - \omega (T, k) \right|,
$$

where $f ^ { \theta }$ is the parametric function. Given a fit $\theta ,$ , we need to check that 

• the fitted surface is a free from calendar-spread arbitrage, 

• and each time slice is free of butterfly arbitrage. 

Proposition 6.4.1. The fitted surface is free from calendar-spread arbitrage if 

$$
f _ {T} ^ {\theta} (T, k) \geq 0;
$$

in other words the slices of the weighted surface cannot intersect. 

To prevent butterfly arbitrage, efectively we need to ensure that the option price yields a probability density function, 

$$
\frac {d}{d K} \mathbb {P} ^ {Q} (S _ {T} \leq K | \mathcal {F} _ {t}) = e ^ {r (T - t)} \frac {\partial^ {2}}{\partial K ^ {2}} C (t, T, K).
$$

Using the parameterized surface, this density is 

$$
\begin{array}{r} e ^ {r (T - t)} \frac {\partial^ {2}}{\partial k ^ {2}} C (t, T, K) = s e ^ {r (T - t)} \frac {\partial^ {2}}{\partial k ^ {2}} C ^ {B S _ {1}} (f ^ {\theta} (T, k), k) \\ = \frac {g ^ {\theta} (k)}{\sqrt {2 \pi f ^ {\theta} (T , k)}} e ^ {- \frac {1}{2} d _ {2} ^ {2} (k; \theta)}, \end{array}
$$

where $d _ { 2 } ( k ; \theta ) = - k / \sqrt { f ^ { \theta } ( T , k ) } - \sqrt { f ^ { \theta } ( T , k ) } / 2$ , and 

$$
g ^ {\theta} (k) = \left(1 - \frac {k f _ {k} ^ {\theta} (T , k)}{2 f ^ {\theta} (T , k)}\right) ^ {2} - \frac {f _ {k} ^ {\theta} (T , k) ^ {2}}{4} \left(\frac {1}{f ^ {\theta} (T , k)} + \frac {1}{4}\right) + \frac {f _ {k k} ^ {\theta} (T , k)}{2} .\tag{6.14}
$$

Proposition 6.4.2. The fitted surface is free from butterfly arbitrage if and only if $\dot { g } ^ { \theta } ( k ) \geq$ 0 and lim $1 _ { k \to + \infty } d _ { 1 } ( k ; \theta ) = - \infty$ , where $d _ { 1 } ( k ; \theta ) = - k / \sqrt { f ^ { \theta } ( T , k ) } + \sqrt { f ^ { \theta } ( T , k ) } / 2$ 

Example 6.4.1 (The SVI Parameterization). One such model is the stochastic volatility inspired (SVI) parameterization of the implied-volatility surface. The SVI uses the parametric function 

$$
f ^ {\theta} (k) = a + b \left(\rho (k - m) + \sqrt {(k - m) ^ {2} + \xi^ {2}}\right)\tag{6.15}
$$

with parameters $\theta = ( a , b , \rho , m , \xi )$ fitted across k and T. Clearly, the SVI has $\begin{array} { r } { \frac { \partial } { \partial T } f ^ { \theta } ( k ) = 0 } \end{array}$ to avoid calendar-spread arbitrage (per Proposition $6 . 4 . 1 )$ and parameterizations can be found to avoid butterfly arbitrage per Proposition $6 . 4 . \mathcal { Q } .$ 

## Chapter 7

## Stochastic Volatility

Stochastic volatility is another popular way to fit the implied volatility smile. It has the advantage of assuming volatility brings another source of randomness, and this randomness can be hedge if it is also a Brownian motion. Furthermore, calibration of stochastic volatility models does have some robustness to the market’s daily changes. However, whereas local volatility models are generally calibrated to fit the implied volatility surface (i.e. to fit options of all maturities), stochastic volatility models have trouble fitting more than one maturity at a time. 

Consider the following stochastic volatility model, 

$$
{d S _ {t}} = {\mu S _ {t} d t + \sigma (X _ {t}) S _ {t} d W _ {t}}\tag{7.1}
$$

$$
{d X _ {t}} = {\alpha (X _ {t}) d t + \beta (X _ {t}) d B _ {t}}\tag{7.2}
$$

where $W _ { t }$ and $B _ { t }$ are Brownian motions with correlation $\rho \in ( - 1 , 1 )$ such that $\mathbb { E } [ d W _ { t } d B _ { t } ] =$ ρdt, $\sigma ( x ) > 0$ is the volatility function, and $X _ { t }$ is the volatility process and is usually meanreverting. An example of a mean-revering process is the square-root process, 

$$
d X _ {t} = \kappa (\bar {X} - X _ {t}) d t + \gamma \sqrt {X _ {t}} d B _ {t}.
$$

The square-root process is used in the Heston model (along with $\sigma ( x ) = \sqrt { x } )$ , and usually relies on what is known as the Feller condition $( \gamma ^ { 2 } \leq 2 \bar { X } \kappa )$ so that $X _ { t }$ never touches zero. 

## 7.1 Hedging and Pricing

Assuming that $\alpha$ and $\beta$ are ‘well-behaved’ functions, we define the diferential operator 

$$
\mathcal {L} \doteq \frac {\partial}{\partial t} + \frac {\sigma^ {2} (x) s ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + \mu s \frac {\partial}{\partial s} + \frac {\beta^ {2} (x)}{2} \frac {\partial^ {2}}{\partial x ^ {2}} + \alpha (x) \frac {\partial}{\partial x} + \rho \beta (x) \sigma (x) s \frac {\partial^ {2}}{\partial x \partial s};
$$

the interpretation of $\mathcal { L }$ is the following: $\begin{array} { r } { \frac { \sigma ^ { 2 } ( X _ { t } ) S _ { t } ^ { 2 } } { 2 } \frac { \partial ^ { 2 } } { \partial s ^ { 2 } } + \mu S _ { t } \frac { \partial } { \partial s } } \end{array}$ are the generator of $S _ { t } ;$ $\begin{array} { r l r } {  { \frac { \beta ^ { 2 } ( X _ { t } ) } { 2 } \frac { \partial ^ { 2 } } { \partial x ^ { 2 } } + \alpha ( X _ { t } ) \frac { \partial } { \partial x } } } \end{array}$ are the generator of $\begin{array} { r } { X _ { t } ; \rho \beta ( X _ { t } ) \sigma ( X _ { t } ) S _ { t } \frac { \partial ^ { 2 } } { \partial x \partial s } } \end{array}$ is the cross-term; and the remaining are the separate stochastic terms. We use when applying bi-variate Itˆo Lemma for the process in (7.1) and (7.2): 

For any twice diferentiable function $f ( t , s , x )$ , the Itˆo diferential is 

$$
d f (t, S _ {t}, X _ {t}) = \mathcal {L} f (t, S _ {t}, X _ {t}) d t + \sigma (X _ {t}) S _ {t} \frac {\partial}{\partial s} f (t, S _ {t}, X _ {t}) d W _ {t} + \beta (X _ {t}) \frac {\partial}{\partial x} f (t, S _ {t}, X _ {t}) d B _ {t}.\tag{7.3}
$$

The price $C ( t , s , x )$ is the price of claim $\psi ( s , x )$ paid at time $T$ given $S _ { t } ~ = ~ s$ and $X _ { t } = x$ . We hedge with a self-financing portfolio $V _ { t }$ consisting of risky-asset, the risk-free bank account, and a 2nd derivative $C ^ { \prime }$ that is settled at time $T ^ { \prime } > T$ . This method for hedging stochastic volatility is called the Hull-White method. 

The self-financing condition is 

$$
d V _ {t} = a _ {t} d S _ {t} + b _ {t} d C ^ {\prime} (t, S _ {t}, X _ {t}) + r (V _ {t} - a _ {t} S _ {t} - b _ {t} C ^ {\prime} (t, S _ {t}, X _ {t})) d t.
$$

Now, taking a long position in $V _ { t }$ and a short position in $C ( t , S _ { t } , X _ { t } )$ , we apply the bivariate Itˆo lemma of (7.3) to get the dynamics of this new portfolio: 

$$
d (V _ {t} - C (t, S _ {t}, X _ {t}))
$$

$$
= a _ {t} (\mu S _ {t} d t + \sigma (X _ {t}) S _ {t} d W _ {t})
$$

$$
+ b _ {t} \mathcal {L} C ^ {\prime} (t, S _ {t}, X _ {t}) d t + b _ {t} \sigma (X _ {t}) S _ {t} \frac {\partial}{\partial s} C ^ {\prime} (t, S _ {t}, X _ {t}) d W _ {t} + b _ {t} \beta (X _ {t}) \frac {\partial}{\partial x} C ^ {\prime} (t, S _ {t}, X _ {t}) d B _ {t}
$$

$$
\begin{array}{c} {+ r (V _ {t} - a _ {t} S _ {t} - b _ {t} C ^ {\prime} (t, S _ {t}, X _ {t})) d t} \\ {- \mathcal {L} C (t, S _ {t}, X _ {t}) d t - \sigma (X _ {t}) S _ {t} \frac {\partial}{\partial s} C (t, S _ {t}, X _ {t}) d W _ {t} - \beta (X _ {t}) \frac {\partial}{\partial x} C (t, S _ {t}, X _ {t}) d B _ {t}.} \end{array}
$$

We now choose $a _ { t }$ and $b _ { t }$ so that the $d W _ { t }$ and the $d B _ { t }$ terms vanish, which means that 

$$
\sigma (X _ {t}) S _ {t} \frac {\partial}{\partial s} C (t, S _ {t}, X _ {t}) = a _ {t} \sigma (X _ {t}) S _ {t} + b _ {t} \sigma (X _ {t}) S _ {t} \frac {\partial}{\partial s} C ^ {\prime} (t, S _ {t}, X _ {t})
$$

$$
\beta (X _ {t}) \frac {\partial}{\partial x} C (t, S _ {t}, X _ {t}) = b _ {t} \beta (X _ {t}) \frac {\partial}{\partial x} C ^ {\prime} (t, S _ {t}, X _ {t})
$$

or 

$$
b _ {t} = \frac {\frac {\partial}{\partial x} C (t , S _ {t} , X _ {t})}{\frac {\partial}{\partial x} C ^ {\prime} (t , S _ {t} , X _ {t})}\tag{7.4}
$$

$$
a _ {t} = \frac {\partial}{\partial s} C (t, S _ {t}, X _ {t}) - b _ {t} \frac {\partial}{\partial s} C ^ {\prime} (t, S _ {t}, X _ {t}).\tag{7.5}
$$

Plugging these solutions into the diferential, the $\alpha ( X _ { t } ) { \frac { \partial } { \partial x } }$ terms cancel, the $\mu S _ { t } \frac { \partial } { \partial s }$ terms cancel, and by the same arbitrage argument as Black-Scholes, it follows that $V _ { t } { - } C ( \bar { t } , S _ { t } , X _ { t } )$ must grow at the risk-free rate: 

$$
\begin{array}{l} d (V _ {t} - C _ {t} (t, S _ {t}, X _ {t})) \\ = a _ {t} \mu S _ {t} d t + b _ {t} \mathcal {L} C ^ {\prime} (t, S _ {t}, X _ {t}) d t + r (V _ {t} - a _ {t} S _ {t} - b _ {t} C ^ {\prime} (t, S _ {t}, X _ {t})) d t - \mathcal {L} C (t, S _ {t}, X _ {t}) d t \\ = r (V _ {t} - C (t, S _ {t}, X _ {t})) d t. \end{array}
$$

Inserting $a _ { t }$ and $b _ { t }$ from equations (7.4) and (7.5), and after some rearranging of terms (and dropping the dt’s), we get 

$$
\left(\mathcal {L} - (\mu - r) S _ {t} \frac {\partial}{\partial s} - r\right) C (t, S _ {t}, X _ {t}) = b _ {t} \left(\mathcal {L} - (\mu - r) S _ {t} \frac {\partial}{\partial s} - r\right) C ^ {\prime} (t, S _ {t}, X _ {t})
$$

and dividing both sides by $\textstyle { \frac { \partial } { \partial x } } C ( t , S _ { t } , X _ { t } )$ , we get 

$$
\frac {\left(\mathcal {L} - (\mu - r) S _ {t} \frac {\partial}{\partial s} - r\right) C (t , S _ {t} , X _ {t})}{\frac {\partial}{\partial x} C (t , S _ {t} , X _ {t})} = \frac {\left(\mathcal {L} - (\mu - r) S _ {t} \frac {\partial}{\partial s} - r\right) C ^ {\prime} (t , S _ {t} , X _ {t})}{\frac {\partial}{\partial x} C ^ {\prime} (t , S _ {t} , X _ {t})} \doteq R (t, s, x).
$$

The left-hand side of this equation does not depend on specifics of $C ^ { \prime } \ { \mathrm { ( e . g . } }$ . maturity and strikes), and the right-hand side does not depend on specifics of C. Therefore, there is a function $R ( t , s , x )$ that does not depend on parameters such as strike price and maturity, and it equates the two sides of the expression. We let R take the form 

$$
R (t, s, x) = - \alpha (x) + \beta (x) \Lambda (t, s, x)
$$

where 

$$
\Lambda (t, s, x) = \rho \frac {\mu - r}{\sigma (x)} + g (t, s, x) \sqrt {1 - \rho^ {2}},
$$

where $g$ is an arbitrary function. Hence, we arrive at the PDE for the price $C ( t , s , x )$ of a European Derivative with stochastic vol: 

Proposition 7.1.1. (Pricing PDE for Stochastic Volatility). Given the stochastic volatility model of equations (7.1) and (7.2), the price of a European claim with payof 

$\psi ( S _ { T } )$ satisfies 

$$
\begin{array}{r} \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} (x) s ^ {2}}{2} \frac {\partial^ {2}}{\partial s ^ {2}} + \rho \beta (x) \sigma (x) s \frac {\partial^ {2}}{\partial x \partial s} + \alpha (x) \frac {\partial}{\partial x} + \frac {\beta^ {2} (x)}{2} \frac {\partial^ {2}}{\partial x ^ {2}} + r s \frac {\partial}{\partial s} - r\right) C \\ = \beta (x) \Lambda (t, s, x) \frac {\partial}{\partial x} C \end{array}\tag{7.6}
$$

with ${ \cal C } \Big | _ { T } = \psi ( s , x )$ 

The PDE in (7.6) can be solved with Feynman-Kac, 

$$
C (t, s, x) = e ^ {- r (T - t)} \mathbb {E} ^ {Q} \{\psi (S _ {T}, X _ {T}) | S _ {t} = s, X _ {t} = x \}.
$$

which yields a description of an EMM, Q, under which the stochastic volatility model is 

$$
\begin{array}{r c l} \frac {d S _ {t}}{S _ {t}} & = & r d t + \sigma (X _ {t}) d W _ {t} ^ {Q} \\ d X _ {t} & = & (\alpha (X _ {t}) - \beta (X _ {t}) \Lambda (t, S _ {t}, X _ {t})) d t + \beta (X _ {t}) d B _ {t} ^ {Q} \end{array}
$$

where $\boldsymbol { W } _ { t } ^ { Q }$ and $B _ { t } ^ { Q }$ are Q-Brownian motions with the same correlation $\rho$ as before. The interpretation of $\Lambda ( t , s , x )$ is that it is the market price of volatility risk. 

One can think of a market as complete when there are as many non-redundant assets as there are sources of randomness. In this sense we have ‘completed’ this market with stochastic volatility by including the derivative $C ^ { \prime }$ among the traded assets. This has allowed us to replicate the European claim and obtain a unique no-arbitrage price that must be the solution to (7.6). 

Example 7.1.1. (The Heston Model). For the Heston model described earlier, the EMM $\mathbb { Q }$ is described by 

$$
d S _ {t} = r S _ {t} d t + \sqrt {X _ {t}} d W _ {t} ^ {Q}\tag{7.7}
$$

$$
d X _ {t} = \kappa (\bar {X} - X _ {t}) d t + \lambda X _ {t} d t + \gamma \sqrt {X _ {t}} d B _ {t} ^ {Q}\tag{7.8}
$$

where $\lambda X _ { t }$ is the assumed form of the volatility price of risk. This model can be re-written, 

$$
d X _ {t} = \tilde {\kappa} (\tilde {\bar {X}} - X _ {t}) d t + \gamma \sqrt {X _ {t}} d B _ {t} ^ {Q}
$$

where $\tilde { \kappa } = \kappa - \lambda$ and $\begin{array} { r } { \tilde { \bar { X } } = \frac { \kappa \bar { X } } { \kappa - \lambda } } \end{array}$ . It is important to have the Feller condition 

$$
\gamma^ {2} \leq 2 \tilde {\kappa} \tilde {\bar {X}}
$$

otherwise the PDE requires boundaries for the event $X _ { t } = 0$ . The process $X _ { t }$ is degenerate, but it is well-known that the Feller condition is the critical assumption for the application of Feynman-Kac. The fit of the Heston model to the implied volatility of market data is shown in Figure 7.1. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/9856f314b39bcff284d0bc9a4fb3d5844640c6265c3c772375e2b55d6f329a4e.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/110f68b6a94f1648ae38d463e7154846c963ee807342a2b2648a564190fcff6f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/5b480ce0-fef4-491d-ad85-e6f4522728f0/e1ad93fbdf064085e87dcb101249f9ef12b8ae8f03416d0298be635d8a251007.jpg)



Figure 7.1: The fit of the Heston model to implied volatility of market data on July 27 of 2012, with diferent maturities. Notice that the Heston model doesn’t fit very well to the options with shortest time to maturity.


## 7.2 Monte Carlo Methods

A slow but often reliable method for pricing derivatives is to approximate the risk-neutral expectation with independent samples. Essentially, sample paths of Brownian motion are obtained using a pseudo-random number generated, the realized derivative payof is computed for each sample, and then the average of these sample payofs is an approximation of the true average. For example, let $\ell = 1 , 2 , \ldots , N$ , let $S _ { T } ^ { ( \ell ) }$ be the index for an independent sample from $S _ { T } \mathrm { \ ' _ { s } }$ probability distribution. I $\mathrm { ~ f ~ } \mathbb { E } ^ { Q } S _ { T } ^ { 2 } < \infty$ , then by the law of large numbers we have 

$$
\frac {1}{N} \sum_ {\ell = 1} ^ {N} (S _ {T} ^ {(\ell)} - K) ^ {+} \stackrel {N \to \infty} {\longrightarrow} \mathbb {E} ^ {Q} (S _ {T} - K) ^ {+} .
$$

For stochastic diferential equations, the typical method is to generate samples that are approximately from the same distribution as the price. The basic idea is to use an Euler-Maruyama scheme, 

$$
\log \tilde {S} _ {t + \Delta t} ^ {(\ell)} = \log \tilde {S} _ {t} ^ {(\ell)} + \left(\mu - \frac {1}{2} \sigma^ {2}\right) \Delta t + \sigma (W _ {t + \Delta t} ^ {(\ell)} - W _ {t} ^ {(\ell)}) ,\tag{7.9}
$$

for some small $\Delta t > 0$ , with 

$$
W _ {t + \Delta t} ^ {(\ell)} - W _ {t} ^ {(\ell)} \sim i i d \mathcal {N} (0, \Delta t).
$$

This scheme is basically the discrete backward Riemann sum from which the Itˆo integral was derived (see Chapter 2). In the limit, the Monte-Carlo average will be with little-o of the true expectation, 

$$
\lim _ {N \to \infty} \frac {1}{N} \sum_ {\ell = 1} ^ {N} (\tilde {S} _ {T} ^ {(\ell)} - K) ^ {+} = \mathbb {E} ^ {Q} (S _ {T} - K) ^ {+} + o (\Delta t).
$$

The scheme in (7.9) can easily be adapted for a local volatility model, and can also be adapted to stochastic volatility models, but the latter will also need a scheme for generating the volatility process $X _ { t }$ 

Example 7.2.1. (The exponential OU model). Consider the stochastic volatility model 

$$
\begin{array}{l} \frac {d S _ {t}}{S _ {t}} = r d t + e ^ {X _ {t}} d W _ {t} ^ {Q} \\ d X _ {t} = \kappa (\bar {X} - X _ {t}) d t + \gamma d B _ {t} ^ {Q} \end{array}
$$

with correlation ρ between $\boldsymbol { W } _ { t } ^ { Q }$ and $B _ { t } ^ { Q }$ . The Euler-Maruyama scheme is 

$$
\log \tilde {S} _ {t + \Delta t} = \log \tilde {S} _ {t} + \left(r - \frac {1}{2} e ^ {2 \tilde {X} _ {t}}\right) \Delta t + e ^ {\tilde {X} _ {t}} \left(\rho (B _ {t + \Delta t} - B _ {t}) + \sqrt {1 - \rho^ {2}} (W _ {t + \Delta t} - W _ {t})\right)
$$

$$
\tilde {X} _ {t + \Delta t} = \tilde {X} _ {t} + \kappa (\bar {X} - \tilde {X} _ {t}) \Delta t + \gamma (B _ {t + \Delta t} - B _ {t})
$$

where $B _ { t + \Delta t } ^ { ( \ell ) } - B _ { t } ^ { ( \ell ) }$ and $W _ { t + \Delta t } ^ { ( \ell ) } - W _ { t } ^ { ( \ell ) }$ are increments of independent Brownian motions. 

Sometimes, there more clever methods of sampling need to be employed. For instance, the Heston model: 

Example 7.2.2. (Sampling the Heston Model). Recall the Heston model of $( 7 . 7 )$ and (7.8). A scheme similar to the one used in the previous example will not work for the Heston model because Euler-Maruyama, 

$$
\tilde {X} _ {t + \Delta t} = \tilde {X} _ {t} + \kappa (\bar {X} - \tilde {X} _ {t}) \Delta t + \gamma \sqrt {\tilde {X} _ {t}} (B _ {t + \Delta t} - B _ {t})
$$

will allow the volatility process to become negative. An alternative is to consider the Stratonovich-type diferential,<sup>1</sup> 

$$
d X _ {t} = \left(\kappa (\bar {X} - X _ {t}) - \frac {\gamma^ {2}}{2}\right) d t + \gamma \sqrt {X _ {t}} \circ d B _ {t}
$$

and then use an implicit Euler-Maruyama scheme 

$$
\tilde {X} _ {t + \Delta t} - \tilde {X} _ {t} = \left(\kappa (\bar {X} - \tilde {X} _ {t + \Delta t}) - \frac {\gamma^ {2}}{2}\right) \Delta t + \gamma \sqrt {\tilde {X} _ {t + \Delta t}} (B _ {t + \Delta t} - B _ {t}).
$$

which can be solved for $\sqrt { \tilde { X } _ { t + \Delta t } }$ using the quadratic equation. Notice that a condition for the discriminant to be real is the Feller condition that $\gamma ^ { 2 } \leq 2 \kappa \bar { X }$ 

In general, Monte Carlo methods are good because they can be used to price pretty much any type of derivative instrument, so long as the EMM is given. For instance, it is very easy to price an Asian option with Monte Carlo. Another advantages of Monte Carlo is that there is no need for an explicit solution to any kind of PDE; the methodology for pricing is to simply simulate and average. However, as mentioned above, this can be very slow, and so there is a need (particularly among practitioners) for faster ways to compute prices. 

Another important topic to remark on is importance sampling, which refers to simulations generated under an equivalent measure for which certain rare events are more common. For instance, suppose one wants to use Monte Carlo to price a call option with extreme strike. It will be a waste of time to generate samples from the EMM’s model if the overwhelming majority of them will finish out of the money. Instead, one can sample from another model that has more volatility, so that more samples finish in the money. Then, assign importance weights based on ratio of densities and take the average. See [Glasserman, 2004] for further reading on Monte Carlo methods in finance. 

<sup>1</sup>This refers to the Stratonovich-type integral that is the limit of forward Riemann sums, $\int f _ { s }$ ◦ $d B _ { s } ~ = ~$ lim<sub>N</sub> $\begin{array} { r } { \sum _ { n = 1 } ^ { N } f _ { t _ { n } } ( B _ { t _ { n } } - B _ { t _ { n - 1 } } ) } \end{array}$ . For the square-root process, the Itˆo lemma on $\sqrt { X _ { t } }$ is used to show that $\begin{array} { r l } { \gamma \int \sqrt { X _ { s } } d B _ { s } = \gamma \operatorname* { l i m } _ { n } \sum _ { n } \sqrt { X _ { t _ { n - 1 } } } \Delta B _ { t _ { n - 1 } } = - \gamma \operatorname* { l i m } _ { n } \sum _ { n } \left( \sqrt { X _ { t _ { n } } } - \sqrt { X _ { t _ { n - 1 } } } \right) \left( B _ { t _ { n } } - B _ { t _ { n - 1 } } \right) + \gamma \left( \sqrt { X _ { t _ { n - 1 } } } - \sqrt { X _ { t _ { n - 1 } } } \right) \left( B _ { t _ { n } } - B _ { t _ { n - 1 } } \right) . } \end{array}$ γ lim<sub>n</sub> $\begin{array} { r } { \sum _ { n } \sqrt { X _ { t _ { n } } } ( B _ { t _ { n } } - B _ { t _ { n - 1 } } ) = - \frac { \gamma ^ { 2 } } { 2 } \int d s + \gamma \int \sqrt { X _ { s } } \circ d B _ { s } } \end{array}$ 

## 7.3 Fourier Transform Methods

The most acclaimed way to compute a European option price is with the so-called Fourier transform methods. In particular, the class of afine models in [Dufie et al., 2000] have tractable pricing formulae because they have explicit expressions for their Fourier transforms. The essential ingredient to these methods is the characteristic function, 

$$
\phi_ {T} (u) \doteq \mathbb {E} ^ {Q} \exp (i u \log (S _ {T})) \quad \forall u \in \mathbb {C}, i = \sqrt {- 1},
$$

where $\mathbb { E } ^ { Q }$ now denotes expectation under an EMM. The function $\phi _ { T } ( u )$ is the Fourier transform of the log $S _ { T } \mathrm { \ ' _ { s } }$ distribution function, 

$$
\phi_ {T} (u) = \int_ {- \infty} ^ {\infty} e ^ {i u s} f (s) d s
$$

where $f ( s )$ is the density function for log $S _ { T }$ . The inverse Fourier transform is $f ( s ) = $ $\begin{array} { r } { { \frac { 1 } { 2 \pi } } \int _ { - \infty } ^ { \infty } e ^ { - i u s } \phi _ { T } ( u ) d u } \end{array}$ , which leads to the cumulative distribution function 

$$
F (s) - F (0) = \int_ {0} ^ {s} f (v) d v = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \frac {1 - e ^ {- i u s}}{i u} \phi_ {T} (u) d u.
$$

The crucial piece of information is the characteristic function, as any European claim can be priced provided there is also a Fourier transform for the payof function. Let $p _ { T }$ denote the density function on the risk-neutral distribution of $\log ( S _ { T } )$ and let $\widehat { \psi }$ denote the Fourier transform of the payof function. It is shown in [Lewis, 2000] that 

$$
\mathbb {E} ^ {Q} \psi (\log (S _ {T})) = \int_ {- \infty} ^ {\infty} \psi (s) f (s) d s = \int_ {- \infty} ^ {\infty} \frac {1}{2 \pi} \int_ {i z - \infty} ^ {i z + \infty} e ^ {- i u s} \widehat {\psi} (u) d u f (s) d s
$$

$$
= \frac {1}{2 \pi} \int_ {i z - \infty} ^ {i z + \infty} \widehat {\psi} (u) \int_ {- \infty} ^ {\infty} e ^ {- i u s} p _ {T} (s) d s d u = \frac {1}{2 \pi} \int_ {i z - \infty} ^ {i z + \infty} \widehat {\psi} (u) \phi_ {T} (- u) d u
$$

where the constant $z \in \mathbb { R }$ in the limit of integration is the appropriate strip of regularity for non-smooth payof functions (see Table 7.1). This usage of characteristic functions is far reaching, as the class of L´evy jump models are defined in terms of their characteristic function, or equivalently with the L´evy-Khintchine representation (for more on financial models with jumps see [Cont. and Tankov, 2003]). 

## 7.4 Call-Option Pricing

An important tool is the formula of Gil-Pelaez: 


Table 7.1: Fourier Transforms of Various Payofs, $\begin{array} { r } { \widehat { \psi } ( u ) = \int _ { - \infty } ^ { \infty } e ^ { i u s } \psi ( s ) d s } \end{array}$ and $\psi ( s ) = $ $\begin{array} { r } { \frac { 1 } { 2 \pi } \int _ { i z - \infty } ^ { i z + \infty } e ^ { - i u s } \widehat { \psi } ( u ) d u , z = \mathfrak { I } ( u ) } \end{array}$


<table><tr><td>asset</td><td><eq>\psi(s)</eq></td><td><eq>\widehat{\psi}(u)</eq></td><td>regularity strip</td></tr><tr><td>call</td><td><eq>(e^{s} - K)^{+}</eq></td><td><eq>-\frac{K^{iu+1}}{u^{2}-iu}</eq></td><td>z&gt;1</td></tr><tr><td>put</td><td><eq>(K - e^{s})^{+}</eq></td><td><eq>-\frac{K^{iu+1}}{u^{2}-iu}</eq></td><td>z&lt;0</td></tr><tr><td>covered call; cash secured put</td><td><eq>\min(e^{s}, K)</eq></td><td><eq>\frac{K^{iu+1}}{u^{2}-iu}</eq></td><td>0</td></tr><tr><td>cash or nothing call</td><td><eq>\mathbb{1}_{[e^{s} \geq K]}</eq></td><td><eq>-\frac{K^{iu}}{iu}</eq></td><td>z&gt;0</td></tr><tr><td>cash or nothing put</td><td><eq>\mathbb{1}_{[e^{s} \leq K]}</eq></td><td><eq>\frac{K^{iu}}{iu}</eq></td><td>z&lt;0</td></tr><tr><td>asset or nothing call</td><td><eq>e^{s}\mathbb{1}_{[e^{s} \geq K]}</eq></td><td><eq>-\frac{K^{iu+1}}{iu+1}</eq></td><td>z&gt;1</td></tr><tr><td>asset or nothing put</td><td><eq>e^{s}\mathbb{1}_{[e^{s} \leq K]}</eq></td><td><eq>\frac{K^{iu+1}}{iu+1}</eq></td><td>z&lt;0</td></tr><tr><td>Arrow-Debreu</td><td><eq>\delta(s - \log(K))</eq></td><td><eq>K^{iu}</eq></td><td>z∈R</td></tr></table>

Proposition 7.4.1 (Gil-Pelaez Inversion Theorem). The distribution function $F ( s )$ is given by 

$$
F (s) = \frac {1}{2} + \frac {1}{2 \pi} \int_ {0} ^ {\infty} \frac {e ^ {i u s} \phi_ {T} (- u) - e ^ {- i u s} \phi_ {T} (u)}{i u} d u,\tag{7.10}
$$

for all $s \in ( - \infty , \infty )$ 

Proof. First let’s prove an identity, 

$$
\operatorname{sign} (v - s) = \frac {2}{\pi} \int_ {0} ^ {\infty} \frac {\sin (u (v - s))}{u} d u = \left\{ \begin{array}{l l} - 1 & \text {if v <   s} \\ 0 & \text {if v = s} \\ 1 & \text {if v > s} \end{array} \right..
$$

This integral is shown using residue calculus: 

$$
\int_ {0} ^ {\infty} \frac {\sin (u)}{u} d u = \frac {1}{2} \int_ {- \infty} ^ {\infty} \frac {\sin (u)}{u} d u = \frac {1}{2} \lim _ {\epsilon \to 0} \lim _ {R \to 0} \mathrm{Im} \left(\int_ {- R} ^ {- \epsilon} \frac {e ^ {i z}}{z} d z + \int_ {\epsilon} ^ {R} \frac {e ^ {i z}}{z} d z\right) .
$$

A closed path can be constructed from −R to $R ,$ making a semi-circle of radius  around zero, and then from R back to −R on a semi-circle of radius R. Along this path the integral of $e ^ { i z } / z$ is zero, 

$$
\int_ {- R} ^ {- \epsilon} \frac {e ^ {i z}}{z} d z + \int_ {\epsilon} ^ {R} \frac {e ^ {i z}}{z} d z = - \int_ {C _ {\epsilon}} \frac {e ^ {i z}}{z} d z - \int_ {C _ {R}} \frac {e ^ {i z}}{z} d z = 0,
$$

where $C _ { \epsilon } = \{ \epsilon e ^ { i ( \theta - \pi ) } | 0 \le \theta \le \pi \}$ and $C _ { R } = \{ R e ^ { i \theta } | 0 \leq \theta \leq \pi \}$ . Now, 

$$
\begin{array}{r l} \left| \int_ {C _ {R}} \frac {e ^ {i z}}{z} d z \right| & = \frac {1}{R} \left| \int_ {0} ^ {\pi} \frac {e ^ {i R \cos (\theta) - R \sin (\theta)}}{e ^ {i \theta}} d \theta \right| \\ & \leq \frac {1}{R} \int_ {0} ^ {\pi} \left| \frac {e ^ {i R \cos (\theta) - R \sin (\theta)}}{e ^ {i \theta}} \right| d \theta \\ & = \frac {1}{R} \int_ {0} ^ {\pi} e ^ {- R \sin (\theta)} d \theta \\ & <   \frac {\pi}{R} \to 0 \qquad \text {as} R \to \infty , \end{array}
$$

and 

$$
\int_ {C _ {\epsilon}} \frac {e ^ {i z}}{z} d z = \int_ {\pi} ^ {0} \frac {1 + O (\epsilon)}{\epsilon e ^ {i \theta}} i \epsilon e ^ {i \theta} d \theta = - i \pi + O (\epsilon).
$$

Hence, 

$$
\int_ {0} ^ {\infty} \frac {\sin (u)}{u} d u = \frac {1}{2} \lim _ {\epsilon \to 0} \lim _ {R \to 0} \mathrm{Im} \left(\int_ {- R} ^ {- \epsilon} \frac {e ^ {i z}}{z} d z + \int_ {\epsilon} ^ {R} \frac {e ^ {i z}}{z} d z\right) = \frac {\pi}{2} .
$$

Now notice that 

$$
\begin{array}{l} \frac {1}{\pi} \int_ {0} ^ {\infty} \frac {e ^ {i u s} \phi_ {T} (- u) - e ^ {- i u s} \phi_ {T} (u)}{i u} d u = \frac {1}{\pi} \int_ {0} ^ {\infty} \int_ {- \infty} ^ {\infty} \frac {e ^ {- i u (v - s)} - e ^ {i u (v - s)}}{i u} d F (v) d u \\ \qquad = - \frac {2}{\pi} \int_ {0} ^ {\infty} \int_ {- \infty} ^ {\infty} \frac {\sin (u (v - s))}{u} d F (v) d u \\ \qquad = - \int_ {- \infty} ^ {\infty} d F (v) \frac {2}{\pi} \int_ {0} ^ {\infty} \frac {\sin (u (v - s))}{u} d u \\ \qquad = \int_ {- \infty} ^ {s} d F (v) - \int_ {s} ^ {\infty} d F (v) \\ \qquad = 2 F (s) - 1, \end{array}
$$

which proves (7.10). 

Notice that (7.10) can be further simplified to have 

$$
F (s) = \frac {1}{2} - \frac {1}{\pi} \int_ {0} ^ {\infty} \mathrm{Re} \left[ \frac {e ^ {- i u s} \phi_ {T} (u)}{i u} \right] d u ,
$$

which is used in pricing a European call option, as the risk-neutral probability of finishing in the money is 

$$
\Pi_ {2} = \mathbb {Q} (S _ {T} \geq K) = \frac {1}{2} + \frac {1}{\pi} \int_ {0} ^ {\infty} \mathrm{Re} \left[ \frac {e ^ {- i u \log (K)} \phi_ {T} (u)}{i u} \right] d u
$$

where $\mathbb { Q }$ denotes probability under the EMM. The ‘delta’ of the option is 

$$
\Pi_ {1} = \frac {e ^ {- r T}}{S _ {0}} \mathbb {E} ^ {Q} S _ {T} \mathbb {1} _ {[ S _ {T} \geq K ]} = \frac {e ^ {- r T}}{S _ {0}} \int_ {\log K} ^ {\infty} e ^ {s} f (s) d s ,
$$

but we can define a change of measure, 

$$
\frac {d \widetilde {\mathbb {Q}}}{d \mathbb {Q}} = \frac {e ^ {s _ {T}}}{\mathbb {E} ^ {Q} e ^ {s _ {T}}} = \frac {e ^ {s _ {T}}}{S _ {0} e ^ {r T}},
$$

where $s _ { T } =$ log $S _ { T }$ . Then, 

$$
\mathbb {E} ^ {\widetilde {Q}} e ^ {i u s _ {T}} = \frac {\mathbb {E} ^ {Q} e ^ {(1 + i u) s _ {T}}}{\mathbb {E} ^ {Q} e ^ {s _ {T}}} = \frac {\phi_ {T} (u - i)}{\phi_ {T} (- i)},
$$

and therefore we have the formula 

$$
\Pi_ {1} = \widetilde {\mathbb {Q}} (S _ {T} \geq K) = \frac {1}{2} + \frac {1}{\pi} \int_ {0} ^ {\infty} \mathrm{Re} \left[ \frac {e ^ {- i u \log (K)} \phi_ {T} (u - i)}{i u \phi_ {T} (- i)} \right] d u.
$$

Assuming no dividends, the value of a European call option with strike $K .$ , at time $t = 0$ is 

$$
C = S _ {0} \Pi_ {1} - K e ^ {- r T} \Pi_ {2}.\tag{7.11}
$$

The pricing formula of equation (7.11) is (in one way or another) interpreted as an inverse Fourier transform. Indeed, the method of Carr and Madan [Carr et al., 1999] shows that (7.11) can be well-approximated as a fast Fourier transform, which has the advantage of taking less time to compute than numerical integration, but it is also less accurate. Equation (7.11) has become an important piece of machinery in quantitative finance because it is (or is considered to be) an explicit solution to the pricing equation. In general the pricing formula of (7.11) applies to just about any situation where the characteristic function is given. 

## 7.5 Heston Explicit Formula

Finally, an important application of the Fourier pricing formula in (7.11) is to the Heston model. The call option formula for the Heston model from equations (7.7) and (7.8) has a well-known inverse Fourier transform (see [Gatheral, 2006]) with 

$$
\begin{array}{r l} & {\Pi_ {j} ^ {h e s t o n} = \frac {1}{2} + \frac {1}{\pi} \int_ {0} ^ {\infty} \mathrm{Re} \left[ \frac {e ^ {- i u \log (K)} \phi_ {T} ^ {j} (u)}{i u} \right] d u \qquad \mathrm{for} j = 1, 2,} \\ & {\phi_ {T} ^ {j} (u) = \exp {(A _ {j} (u) + B _ {j} (u) X _ {0} + i u (\log (S _ {0}) + r T))}} \\ & {A _ {j} (u) = \frac {\kappa \bar {X}}{\gamma^ {2}} \left((b _ {j} - \rho \gamma u i - d _ {j}) T - 2 \log {\left(\frac {1 - g _ {j} e ^ {- d _ {j} r}}{1 - g _ {j}}\right)}\right)} \\ & {B _ {j} (u) = \frac {b _ {j} - \rho \gamma u i - d _ {j}}{\gamma^ {2}} \left(\frac {1 - e ^ {- d _ {j} r}}{1 - g _ {j} e ^ {- d _ {j} r}}\right)} \\ & {\quad g _ {j} = \frac {b _ {j} - \rho \gamma u i - d _ {j}}{b _ {j} - \rho \gamma u i + d _ {j}}} \\ & {\quad d _ {j} = \sqrt {(\rho \gamma u i - b _ {j}) ^ {2} - \gamma^ {2} (2 c _ {j} u i - u ^ {2})}} \\ & {\quad c _ {1} = \frac {1}{2}, c _ {2} = - \frac {1}{2}, b _ {1} = \kappa - \rho \gamma , b _ {2} = \kappa ,} \end{array}
$$

which is applied for the Heston model the volatility price of risk absorbed into parameters κ and $\bar { X }$ . Warning: Use a well-made Gaussian quadrature function for numerical computation of the integrals for the Heston price; do not attempt to integrate with an evenly-spaced grid. 

## 7.6 The Merton Jump Difusion

Short time-to-maturity options are known to be well fit by the class of models where log-asset prices are L´evy processes. For instance, the Merton jump difusion, 

$$
\frac {d S _ {t}}{S _ {t}} = (r - \nu) d t + \sigma d W _ {t} + (e ^ {J _ {t}} - 1) d N _ {t}
$$

where $\sigma > 0 , \ N _ { t }$ is an independent Poisson process with parameter $\lambda \in ( 0 , \infty )$ , J<sub>t</sub> is a sequence of i.i.d. normal random variables with $J _ { t _ { i } } \sim { \cal N } ( \mu J , \sigma _ { J } ^ { 2 } )$ when $N _ { t _ { i } } - N _ { t _ { i } - } = 1$ , and $\nu = \lambda \left( e ^ { \mu _ { J } + \frac { \sigma _ { J } ^ { 2 } } { 2 } } - 1 \right)$ is a compensator to ensure the process is a discounted martingale. The log-price is 

$$
\begin{array}{c} \log (S _ {t} / S _ {0}) = \int_ {0} ^ {t} \left(r - \nu - \frac {\sigma^ {2}}{2}\right) d u + \sigma W _ {t} + \int_ {0} ^ {t} J _ {u} d N _ {u} \\ = \int_ {0} ^ {t} \left(r - \nu - \frac {\sigma^ {2}}{2}\right) d u + \sigma W _ {t} + \sum_ {n = 1} ^ {N _ {t}} J _ {n}. \end{array}
$$

For $S _ { 0 } = 1$ , the characteristic function is derived as follows, 

$$
\begin{array}{r l} & {\phi_ {T} (u) = \mathbb {E} \exp \left(i u \left(r - \nu - \frac {\sigma^ {2}}{2}\right) T + i u \sigma W _ {T} + i u \int_ {0} ^ {t} J _ {t} d N _ {t}\right)} \\ & {\qquad = \exp \left(i u \left(r - \nu - \frac {\sigma^ {2}}{2}\right) T - \frac {\sigma^ {2} u ^ {2}}{2} T + \lambda T \left(e ^ {i u \mu_ {J} - \frac {\sigma_ {J} ^ {2} u ^ {2}}{2}} - 1\right)\right).} \end{array}
$$

This is an example of a characteristic function that is known explicitly. In addition, it is particular example of the general L´evy-Khintchine representation, 

$$
\begin{array}{l} \mathbb {E} \exp (i u \log (S _ {T})) \\ = \exp \left(i u \left(r - \nu - \frac {\sigma^ {2}}{2}\right) T - \frac {\sigma^ {2} u ^ {2}}{2} T + T \int_ {\mathbb {R} \backslash \{0 \}} \left(e ^ {i u x} - 1 - i u x \mathbf {1} _ {| x | <   1}\right) \eta (d x)\right), \end{array}
$$

where $\eta$ is the intensity measure, satisfying $\begin{array} { r } { \int _ { \mathbb { R } \backslash \{ 0 \} } 1 \wedge x ^ { 2 } \eta ( d x ) < \infty } \end{array}$ . For more on the L´evy-Khintchine representation, see [Cont. and Tankov, 2003]. 

## Chapter 8

## Stochastic Control

This chapter takes techniques from stochastic control and applies them to portfolio management. The portfolio can be of varying type, two possibilites are a portfolio for investment of (personal) wealth, or a hedging portfolio with a short position in a derivative contract. The basic problem involves an investor with a self-financing wealth process and a concave utility function to quantify their risk aversion, from which their goal is to maximize their expected utility of terminal wealth and/or consumption. To exemplify the need for hedging obtained from optimal control, recall the price of volatility risk $\Lambda ( t , s , x )$ from Proposition 7.1.1 of Chapter 7. The pricing PDE for stochastic volatility depends on Λ, but incompleteness of the market means that Λ may not be uniquely specified. However, an expression can be obtained from the solution to an optimal control, hence writing Λ as a function of the investor’s risk aversion. This chapter will start by considering the basic problem of optimization of (personal) wealth, and later on will show how optimal control is used in hedging derivatives. 

## 8.1 The Optimal Investment Problem

Consider a standard geometric Brownian motion for the price of a risky asset, 

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma d W _ {t},\tag{8.1}
$$

where $\mu \in \mathbb { R } , \sigma > 0$ , and W is a Brownian motion under the statistical measure. There is also the risk-free bank account that pays interest at a rate $r \geq 0$ . At time $t \geq 0$ the investors has a portfolio value $X _ { t }$ with an allocation $\pi _ { t }$ in the risky asset and a consumption stream $c _ { t }$ . The dynamics of the portfolio are self-financing, 

$$
d X _ {t} = X _ {t} \left(r d t + \pi_ {t} \left(\frac {d S _ {t}}{S _ {t}} - r d t\right) - c _ {t} d t\right),\tag{8.2}
$$

where 

π<sub>t</sub> = proportion of wealth in the risky asset, 

$$
c _ {t} = \mathrm{rateofconsumption}.
$$

A natural constraint on consumption is $c _ { t } \geq 0$ for all $t \geq 0$ , and based on (8.2) a constraint of $X _ { t } ~ \geq ~ 0$ is enforced automatically. Here we have taken $X _ { t } ~ \geq ~ 0$ almost surely, but in general any finite lower bound on $X _ { t }$ is necessary to ensure no-arbitrage (i.e. $X _ { t } \geq - M >$ $- \infty$ almost with constant M finite), otherwise there could be doubling strateguies. The optimization problem is then formulated as 

$$
V (t, x) = \max _ {\pi , c \geq 0} \mathbb {E} \left[ \int_ {t} ^ {T} F (u, c _ {u}, X _ {u}) d u + U (X _ {T}) \Big | X _ {t} = x \right],\tag{8.3}
$$

where $F$ is a concave utility on consumption and wealth, $U$ is a concave utility on terminal wealth, and the admissible pairs $( \pi _ { t } , c _ { t } ) _ { t \geq 0 }$ are non-anticipating, adapted to $W$ , with $\begin{array} { r } { \int _ { 0 } ^ { T } | \pi _ { t } X _ { t } | ^ { 2 } d t < \infty } \end{array}$ almost surely. We refer to E $\begin{array} { r } { \left[ \int _ { t } ^ { T } F ( u , c _ { u } , X _ { u } ) d u + U ( X _ { T } ) \Big \vert X _ { t } = x \right] } \end{array}$ as the objective function, and refer to V as the optimal value function. 

Example 8.1.1 (Logarithmic utility). Suppose that $F = 0$ and $U ( x ) = \log ( x )$ . There is no utility of consumption, so the optimal is $c _ { t } = 0$ for all $t \geq 0$ . Now apply Itˆo’s lemma, 

$$
d \log (X _ {t}) = r d t + \pi_ {t} \left(\frac {d S _ {t}}{S _ {t}} - r d t\right) - \frac {\sigma^ {2} \pi_ {t} ^ {2}}{2} d t,
$$

and then taking expectations, 

$$
\mathbb {E} [ \log (X _ {T}) | X _ {t} = x ] = \log (x) + \mathbb {E} \left[ \int_ {t} ^ {T} \left(r + \pi_ {u} (\mu - r) - \frac {\sigma^ {2} \pi_ {u} ^ {2}}{2}\right) d u \Big | X _ {t} = x \right],
$$

where the right-hand side is concave in $\pi _ { t }$ . Hence, the optimal strategy is 

$$
\pi_ {t} = \frac {\mu - r}{\sigma^ {2}} \quad \forall t \in [ 0, T ],
$$

which is the Sharpe ratio divided by the volatility. The optimal value function is 

$$
V (t, x) = \max _ {\pi} \mathbb {E} [ \log (X _ {T}) | X _ {t} = x ] = \log \left(x e ^ {\left(r + \frac {(\mu - r) ^ {2}}{2 \sigma^ {2}}\right) (T - t)}\right),
$$

and using $U ^ { - 1 } ( v ) = e ^ { v }$ , we find the certainty equivalent, 

$$
X _ {t} ^ {c e} = e ^ {- r (T - t)} U ^ {- 1} \left(V (t, X _ {t})\right) = X _ {t} e ^ {\left(\frac {(\mu - r) ^ {2}}{2 \sigma^ {2}}\right) (T - t)},
$$

which is the risk-free rate plus $\frac { 1 } { 2 }$ times the Sharpe-ratio squared. 

Example 8.1.2 (Log-Utility of Consumption). Suppose that $F ( t , c _ { t } , X _ { t } ) = e ^ { - \beta t } \log ( c _ { t } X _ { t } )$ $U ( x ) = 0$ , and $T = \infty$ . The optimization problem is 

$$
\max _ {\pi , c \geq 0} \mathbb {E} \left[ \int_ {t} ^ {\infty} e ^ {- \beta (u - t)} \log (c _ {u} X _ {u}) d u \Big | X _ {t} = x \right] = V (x),
$$

which is constant in t. Now notice for any admissible $( \pi , c )$ on $[ t , t + \Delta t ]$ we have the dynamic programming principle, 

$$
V (X _ {t}) \geq e ^ {- \beta \Delta t} \mathbb {E} _ {t} V (X _ {t + \Delta t}) + \mathbb {E} _ {t} \int_ {t} ^ {t + \Delta t} e ^ {- \beta (u - t)} \log (c _ {u} X _ {u}) d u,
$$

with equality if and only $i f \left( \pi , c \right)$ is chosen optimally over $[ t , t + \Delta t ]$ , and hence 

$$
\begin{array}{l}\frac {\mathbb {E} _ {t} V (X _ {t + \Delta t}) - V (X _ {t})}{\Delta t}\\\leq \frac {1 - e ^ {- \beta \Delta t}}{\Delta t} \mathbb {E} _ {t} V (X _ {t + \Delta t}) - \frac {1}{\Delta t} \mathbb {E} _ {t} \int_ {t} ^ {t + \Delta t} e ^ {- \beta (u - t)} \log (c _ {u} X _ {u}) d u\\\rightarrow \beta V (X _ {t}) - \log (c _ {t} X _ {t}),\end{array}
$$

as $\Delta t \to 0$ . On the other hand, from Itˆo’s lemma we have 

$$
\begin{array}{r} d V (X _ {t}) = \left(\frac {\sigma^ {2} \pi_ {t} ^ {2} X _ {t} ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (X _ {t}) + (r + \pi_ {t} (\mu - r) - c _ {t}) X _ {t} \frac {\partial}{\partial x} V (X _ {t})\right) d t \\ + \sigma \pi_ {t} X _ {t} \frac {\partial}{\partial x} V (X _ {t}) d W _ {t}, \end{array}
$$

and assuming the Brownian term vanishes under expectations, we have 

$$
\begin{array}{r l}&{\frac {\mathbb {E} _ {t} V (X _ {t + \Delta t}) - V (X _ {t})}{\Delta t}}\\&{= \frac {1}{\Delta t} \mathbb {E} _ {t} \int_ {t} ^ {t + \Delta t} \left(\frac {\sigma^ {2} \pi_ {u} ^ {2} X _ {u} ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (X _ {u}) + (r + \pi_ {u} (\mu - r) - c _ {u}) X _ {u} \frac {\partial}{\partial x} V (X _ {u})\right) d u}\\&{\rightarrow \frac {\sigma^ {2} \pi_ {t} ^ {2} X _ {t} ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (X _ {t}) + (r + \pi_ {t} (\mu - r) - c _ {t}) X _ {t} \frac {\partial}{\partial x} V (X _ {t}),}\end{array}
$$

as $\Delta t \to 0$ . Hence, for all admissible pairs $( \pi , c )$ the value function $V ( x )$ satisifies 

$$
\frac {\sigma^ {2} \pi^ {2} x ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (x) + (r + \pi (\mu - r) - c) x \frac {\partial}{\partial x} V (x) - \beta V (x) + \log (c x) \leq 0,
$$

with equality if and only π and c are optimal, which leads to the equation 

$$
\max _ {\pi , c \geq 0} \left(\frac {\sigma^ {2} \pi^ {2} x ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (x) + (r + \pi (\mu - r) - c) x \frac {\partial}{\partial x} V (x) - \beta V (x) + \log (c x)\right) = 0.
$$

Let’s assume the ansatz 

$$
V (x) = a \log (x) + b.
$$

Then through first-order optimality conditions (i.e. by diferentiating with respect to π and setting equal to zero) we find the optimal 

$$
\pi (x) = - \frac {\mu - r}{\sigma^ {2} x} \frac {\frac {\partial}{\partial x} V (x)}{\frac {\partial^ {2}}{\partial x ^ {2}} V (x)} = \frac {\mu - r}{\sigma^ {2}}.
$$

Similarly, first-order optimality conditions for c yield 

$$
c (x) = \frac {1}{x \frac {\partial}{\partial x} V (x)} = \frac {1}{a}.
$$

Putting optimal $\pi _ { t }$ and $c _ { t }$ back into the equation for V along with the ansatz, we find 

$$
\log (x / a) - \beta (a \log (x) + b) + (a r - 1) + \frac {a}{2} \frac {(\mu - r) ^ {2}}{\sigma^ {2}} = 0,
$$

and comparing log(x) terms and non-x-dependent terms we find, 

$$
\begin{array}{l} {a = \frac {1}{\beta},} \\ {b = \frac {1}{2 \beta^ {2}} \frac {(\mu - r) ^ {2}}{\sigma^ {2}} + \frac {r}{\beta^ {2}} + \frac {1}{\beta} (\log (\beta) - 1).} \end{array}
$$

## 8.2 The Hamilton-Jacobi-Bellman (HJB) Equation

Example 8.1.1 is useful to get started and to get a sense for how an optimal control should look. Example 8.1.2 is more instructive because it shows us how (i) the function V inherits concavity from F and $U _ { : }$ , and (ii) how it also shows how to derive the PDE that V should satisfy. 

The derivation starts with the dynamic programming principle, 

$$
V (t, x) = \max _ {\pi , c \geq 0} \mathbb {E} \left[ \int_ {t} ^ {t + \Delta t} F (u, c _ {u}, X _ {u}) d u + V (t + \Delta t, X _ {t + \Delta t}) \Big | X _ {t} = x \right],
$$

where $\operatorname { m a x } _ { \pi , c }$ is taken over the interva $[ t , t + \Delta t ]$ . Applying Itˆo’s lemma to $V ( t , X _ { t } )$ , we find 

$$
\begin{array}{r l} & V (t + \Delta t, X _ {t + \Delta t}) \\ & = V (t, X _ {t}) + \int_ {t} ^ {t + \Delta t} \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} \pi_ {u} ^ {2} X _ {u} ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} + (r + \pi_ {u} (\mu - r) - c _ {u}) X _ {u} \frac {\partial}{\partial x}\right) V (u, X _ {u}) d u \\ & \qquad + \sigma \int_ {t} ^ {t + \Delta t} \pi_ {u} X _ {u} \frac {\partial}{\partial x} V (u, X _ {u}) d W _ {u}, \end{array}
$$

for any admissible $( \pi , c )$ over $[ t , t + \Delta t ]$ . Hence, for any $( \pi , c )$ on $[ t , t + \Delta t ]$ we have 

$$
\begin{array}{r l} & {\mathbb {E} \left[ \int_ {t} ^ {t + \Delta t} \left(F (u, c _ {u}, X _ {u}) + \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} \pi_ {u} ^ {2} X _ {u} ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} \right. \right. \right.} \\ & {\qquad \left. \left. + (r + \pi_ {u} (\mu - r) - c _ {u}) X _ {u} \frac {\partial}{\partial x}\right) V (u, X _ {u})\right) d u \Big | X _ {t} = x \Big ] \le 0 ,} \end{array}
$$

with equality if and only if an optimal $( \pi , c )$ is chosen. Hence, dividing by $\Delta t$ and taking the limt to zero, we obtain the so-called Hamilton-Jacobi-Bellman (HJB) equation: 

$$
\begin{array}{r} \max _ {\pi , c \geq 0} \left(F (t, c) + \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2} \pi^ {2} x ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} + (r + \pi (\mu - r) - c) x \frac {\partial}{\partial x}\right) V (t, x)\right) = 0 , \\ V (T, x) = U (x) \end{array}\tag{8.4}
$$

## 8.3 Merton’s Optimal Investment Problem

Let $F = 0$ and consider a power utility function, 

$$
U (x) = \frac {x ^ {1 - \gamma}}{1 - \gamma},
$$

where $\gamma > 0 , \gamma \neq 1$ is the risk aversion. The problem is to solve 

$$
V (t, x) = \max _ {\pi} \mathbb {E} [ U (X _ {T}) | X _ {t} = x ] ,
$$

The HJB equation for this problem is 

$$
\begin{array}{c} \left(\frac {\partial}{\partial t} + r x \frac {\partial}{\partial x}\right) V (t, x) + \max _ {\pi} \left(\frac {\sigma^ {2} \pi^ {2} x ^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (t, x) + \pi (\mu - r) x \frac {\partial}{\partial x} V (t, x)\right) = 0, \\ V (T, x) = U (x), \end{array}\tag{8.5}
$$

for which we find the optimal $\pi$ , 

$$
\pi_ {t} = - \frac {\mu - r}{x \sigma^ {2}} \frac {\frac {\partial}{\partial x} V (t , x)}{\frac {\partial^ {2}}{\partial x ^ {2}} V (t , x)}.
$$

Inserting the optimal $\pi _ { t }$ into (8.5) we obtain the nonlinear equation, 

$$
\left(\frac {\partial}{\partial t} + r x \frac {\partial}{\partial x}\right) V (t, x) - \frac {((\mu - r) \frac {\partial}{\partial x} V (t , x)) ^ {2}}{2 \sigma^ {2} \frac {\partial^ {2}}{\partial x ^ {2}} V (t , x)} = 0.\tag{8.6}
$$

Then using the ansatz $V ( t , x ) = g ( t ) U ( x )$ , we find 

$$
\frac {\partial}{\partial t} V (t, x) = g ^ {\prime} (t) U (x),
$$

$$
\frac {\partial}{\partial x} V (t, x) = \frac {1 - \gamma}{x} g (t) U (x),
$$

$$
\frac {\partial^ {2}}{\partial x ^ {2}} V (t, x) = - \frac {\gamma (1 - \gamma)}{x ^ {2}} g (t) U (x),
$$

and inserting in (8.6) we find an ODE for $g ,$ 

$$
g ^ {\prime} (t) + r (1 - \gamma) + \frac {(1 - \gamma) (\mu - r) ^ {2} g (t)}{2 \gamma \sigma^ {2}} = 0,
$$

with terminal condition $g ( T ) = 1$ . The solution is 

$$
g (t) = e ^ {(1 - \gamma) (T - t) \left(r + \frac {(\mu - r) ^ {2}}{2 \gamma \sigma^ {2}}\right)},
$$

and the optimal value function is 

$$
V (t, x) = U (x) g (t) = \frac {\left(x e ^ {(T - t) \left(r + \frac {(\mu - r) ^ {2}}{2 \gamma \sigma^ {2}}\right)}\right) ^ {1 - \gamma}}{1 - \gamma} = U \left(x e ^ {(T - t) \left(r + \frac {(\mu - r) ^ {2}}{2 \gamma \sigma^ {2}}\right)}\right) .
$$

and the certainty equivalent is 

$$
X _ {t} ^ {c e} = e ^ {- r (T - t)} U ^ {- 1} (v (t, X _ {t})) = X _ {t} e ^ {(T - t) \left(\frac {(\mu - r) ^ {2}}{2 \gamma \sigma^ {2}}\right)}.
$$

## 8.4 Stochastic Returns

Consider the model 

$$
{d S _ {t}} = {Y _ {t} S _ {t} d t + \sigma S _ {t} d W _ {t}}\tag{8.7}
$$

$$
d Y _ {t} = \kappa (\mu - Y _ {t}) d t + \beta d B _ {t},\tag{8.8}
$$

with $d W _ { t } d B _ { t } \ = \ \rho d t$ where $\rho \in ( - 1 , 1 )$ . The interpretation of $Y _ { t }$ could be any of the following: $Y _ { t }$ is a dividend yield with uncertainty (although somewhat of strange model because it can be negative), or $Y _ { t }$ is the return rate on a commodities or bond portfolio where there is a role yield due to contango or backwardation. 

Let’s assume the simple case $\mu = r = 0$ , for which the value function is 

$$
V (t, x, y) = \max _ {\pi} \mathbb {E} \left[ U (X _ {T}) \Big | X _ {t} = x, Y _ {t} = y \right],
$$

and has HJB equation 

$$
\begin{array}{r l} & {\left(\frac {\partial}{\partial t} + \frac {\beta^ {2}}{2} \frac {\partial^ {2}}{\partial y ^ {2}} - \kappa y \frac {\partial}{\partial y}\right) V (t, x, y)} \\ & {+ \max _ {\pi} \left(\frac {\sigma^ {2} x ^ {2} \pi^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (t, x, y) + \pi x y \frac {\partial}{\partial x} V (t, x, y) \right.} \\ & {\qquad \left. + \rho \pi x \beta \sigma \frac {\partial^ {2}}{\partial x \partial y} V (t, x, y)\right) = 0,} \\ & {\qquad \left. V (T, x, y) = U (x) \right.} \end{array}\tag{8.9}
$$

The first-order condition for π yields the optimal 

$$
\pi_ {t} = - \frac {x y \frac {\partial}{\partial x} V (t , x , y) + \rho \pi x \beta \sigma \frac {\partial^ {2}}{\partial x \partial y} V (t , x , y)}{\sigma^ {2} x ^ {2} \frac {\partial^ {2}}{\partial x ^ {2}} V (t , x , y)} .
$$

For the power utility 

$$
U (x) = \frac {x ^ {1 - \gamma}}{1 - \gamma},
$$

we have the ansatz $V ( t , x , y ) = U ( x ) g ( t , y )$ with 

$$
\begin{array}{r} \frac {\partial}{\partial t} V = \frac {\partial}{\partial t} g (t, y) U (x), \\ \frac {\partial}{\partial x} V = \frac {1 - \gamma}{x} g (t, y) U (x), \\ \frac {\partial^ {2}}{\partial x ^ {2}} V = - \frac {(1 - \gamma) \gamma}{x ^ {2}} g (t, y) U (x), \\ \frac {\partial^ {2}}{\partial x \partial y} V = \frac {1 - \gamma}{x} \frac {\partial}{\partial y} g (t, y) U (x), \end{array}
$$

all of which are inserted into equation (8.9) to get an equation for $g \colon$ 

$$
\begin{array}{r} \left(\frac {\partial}{\partial t} + \frac {\beta^ {2}}{2} \frac {\partial^ {2}}{\partial y ^ {2}} - \kappa y \frac {\partial}{\partial y}\right) g (t, y) + \frac {1 - \gamma}{2 \sigma^ {2} \gamma} \left(y + \frac {\rho \beta \sigma \frac {\partial}{\partial y} g (t , y)}{g (t , y)}\right) ^ {2} g (t, y) = 0, \\ g (T, y) = 1. \end{array}
$$

We now apply another ansatz $g ( t , y ) = e ^ { a ( t ) y ^ { 2 } + b ( t ) }$ , which when inserted into the equation for $g ( t , y )$ yields the following system: 

$$
y ^ {2}: a ^ {\prime} (t) = - 2 \beta^ {2} \left(1 + \frac {(1 - \gamma) \rho^ {2}}{\gamma}\right) a ^ {2} (t) - 2 \left(\frac {\rho \beta (1 - \gamma)}{\sigma \gamma} - \kappa\right) a (t) - \frac {1 - \gamma}{2 \sigma^ {2} \gamma},
$$

$$
1: b ^ {\prime} (t) = - \beta^ {2} a (t),
$$

with terminal conditions $a ( T ) = b ( T ) = 0$ . The solution $a ( t )$ can be written as a ratio, 

$$
a (t) = \frac {v ^ {\prime} (t)}{2 \beta^ {2} \left(1 + \frac {(1 - \gamma) \rho^ {2}}{\gamma}\right) v (t)},
$$

where $v ( t )$ is the solution to a 2nd-order ODE, 

$$
v ^ {\prime \prime} (t) + 2 \left(\frac {\rho \beta (1 - \gamma)}{\sigma \gamma} - \kappa\right) v ^ {\prime} (t) + \frac {(1 - \gamma) \beta^ {2}}{\sigma^ {2} \gamma} \left(1 + \frac {(1 - \gamma) \rho^ {2}}{\gamma}\right) v (t) = 0.
$$

The roots of this equation are 

$$
m _ {\pm} = - \left(\frac {\rho \beta (1 - \gamma)}{\sigma \gamma} - \kappa\right) \pm \sqrt {\kappa^ {2} - \frac {\beta (1 - \gamma)}{\sigma \gamma} \left(2 \kappa \rho + \frac {\beta}{\sigma}\right)},
$$

which gives the general solution 

$$
v (t) = C _ {1} e ^ {m _ {+} (T - t)} + C _ {2} e ^ {m _ {-} (T - t)}.
$$

It is not necessary to fully determine constants $C _ { 1 }$ and $C _ { 2 }$ because we are mainly interested in the ratio $\boldsymbol { v } ^ { \prime } ( t ) / \boldsymbol { v } ( t )$ 

Finite-Time Blowup. Complex valued $m _ { \pm }$ leads to finite-time blowup for the optimization problem. If the roots are complex then let $\begin{array} { r } { c = - \left( \frac { \rho \beta ( 1 - \gamma ) } { \sigma \gamma } - \kappa \right) } \end{array}$ and $d \digamma =$ $\begin{array} { r } { \frac { \beta ( 1 - \gamma ) } { \sigma \gamma } \left( 2 \kappa \rho + \frac { \beta } { \sigma } \right) - \kappa ^ { 2 } } \end{array}$ so that the general solution is 

$$
v (t) = e ^ {c (T - t)} \left(C _ {1} \cos (d (T - t)) + C _ {2} \sin (d (T - t))\right),
$$

and with $v ^ { \prime } ( T ) = - c C _ { 1 } - d C _ { 2 } = 0$ to satisfy the terminal condition $a ( T ) = 0$ , so that 

$$
v (t) = C _ {1} e ^ {c (T - t)} \left(\cos (d (T - t)) - \frac {c}{d} \sin (d (T - t))\right).
$$

The solution $a ( t )$ will blow at time $t ^ { * }$ such that $\begin{array} { r } { \cos ( d ( T - t ^ { * } ) ) - \frac { c } { d } \sin ( d ( T - t ^ { * } ) ) = 0 } \end{array}$ , that is tan $\begin{array} { r } { ( d ( T - t ^ { * } ) ) = \frac { d } { c } } \end{array}$ or 

$$
T - t ^ {*} = \frac {1}{d} \left(\pi \mathbb {1} _ {[ c \leq 0 ]} + \tan^ {- 1} \left(\frac {d}{c}\right)\right).
$$

## 8.5 Stochastic Volatility

Now let’s consider the same optimal terminal wealth problem as the Merton problem, with exponential utility 

$$
U (x) = - \frac {1}{\gamma} e ^ {- \gamma x} \quad \text { where } \gamma > 0,
$$

and in the incomplete market of stochastic volatility, 

$$
{d S _ {t}} = {\mu S _ {t} d t + \sigma (Y _ {t}) S _ {t} d W _ {t}}\tag{8.10}
$$

$$
{d Y _ {t}} = {\alpha (Y _ {t}) d t + \beta (Y _ {t}) d B _ {t},}\tag{8.11}
$$

where $d W _ { t } \cdot d B _ { t } = \rho d t$ . From (8.10) and (8.11), we have the wealth process, 

$$
d X _ {t} = r X _ {t} d t + \pi_ {t} \left(\frac {d S _ {t}}{S _ {t}} - r d t\right),
$$

no longer enforcing the non-negativity constraint. The optimization problem is 

$$
V (t, x, y) = \max _ {\pi} \mathbb {E} \left[ U (X _ {T}) \Big | X _ {t} = x, Y _ {t} = y \right],
$$

but the technique used in Example 8.1.1 does not apply because there is some local martingale behavior in the stochastic integrals. Instead, we arrive at the optimal solution using the HJB equation. The HJB equation is 

$$
\begin{array}{c} \left(\frac {\partial}{\partial t} + r x \frac {\partial}{\partial x} + \frac {\beta^ {2} (y)}{2} \frac {\partial^ {2}}{\partial y ^ {2}} + \alpha (y) \frac {\partial}{\partial y}\right) V (t, x, y) \\ + \max _ {\pi} \left(\frac {\sigma^ {2} (y) \pi^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} V (t, x, y) + \pi (\mu - r) \frac {\partial}{\partial x} V (t, x, y) \right. \\ \left. + \rho \pi \beta (y) \sigma (y) \frac {\partial^ {2}}{\partial x \partial y} V (t, x, y)\right) = 0 , \\ V (T, x) = U (x) \end{array}\tag{8.12}
$$

Using the ansatz $V ( t , x , y ) = U ( x e ^ { r ( T - t ) } ) g ( t , y )$ , we have 

$$
\frac {\partial}{\partial t} V = \gamma r x e ^ {r (T - t)} V + U (x e ^ {r (T - t)}) \frac {\partial}{\partial t} g (t, y),
$$

$$
\frac {\partial}{\partial x} V = - \gamma e ^ {r (T - t)} V,
$$

$$
\frac {\partial^ {2}}{\partial x ^ {2}} V = \gamma^ {2} e ^ {2 r (T - t)} V,
$$

$$
\frac {\partial^ {2}}{\partial x \partial y} V = - \gamma e ^ {r (T - t)} U (x e ^ {r (T - t)}) \frac {\partial}{\partial y} g (t, y),
$$

which we insert into (8.12) to find a PDE for $g ,$ 

$$
\begin{array}{c} \left(\frac {\partial}{\partial t} + \frac {\beta^ {2} (y)}{2} \frac {\partial^ {2}}{\partial y ^ {2}} + \alpha (y) \frac {\partial}{\partial y}\right) g (t, y) \\ + \min _ {\pi} \left(\frac {\gamma^ {2} e ^ {2 r (T - t)} \sigma^ {2} (y) \pi^ {2}}{2} g (t, y) - \gamma e ^ {r (T - t)} \pi \left((\mu - r) g (t, y) + \rho \beta (y) \sigma (y) \frac {\partial}{\partial y} g (t, y)\right)\right) = 0 , \end{array}\tag{8.13}
$$

$$
g (T, y) = 1,
$$

and the optimal strategy is 

$$
\pi_ {t} = e ^ {- r (T - t)} \left(\frac {\mu - r}{\gamma \sigma^ {2} (y)} + \rho \frac {\beta (y)}{\gamma \sigma (y)} \frac {\frac {\partial}{\partial y} g (t , y)}{g (t , y)}\right) .
$$

Inserting this optimal $\pi _ { t }$ into (8.13) yields the nonlinear equation 

$$
\left(\frac {\partial}{\partial t} + \frac {\beta^ {2} (y)}{2} \frac {\partial^ {2}}{\partial y ^ {2}} + \alpha (y) \frac {\partial}{\partial y}\right) g (t, y) - \frac {\sigma^ {2} (y)}{2} \left(\frac {\mu - r}{\sigma^ {2} (y)} + \rho \frac {\beta (y)}{\sigma (y)} \frac {\frac {\partial}{\partial y} g (t , y)}{g (t , y)}\right) ^ {2} g (t, y) = 0.\tag{8.14}
$$

This equation can be reduced to a linear PDE if we look for a function $\psi ( t , y )$ such that 

$$
g (t, y) = \psi (t, y) ^ {q},
$$

where $q$ is a parameter. Diferentiating yields, 

$$
\begin{array}{r l} & {\frac {\partial}{\partial t} g = \frac {q g}{\psi} \frac {\partial}{\partial t} \psi} \\ & {\frac {\partial}{\partial y} g = \frac {q g}{\psi} \frac {\partial}{\partial y} \psi} \\ & {\frac {\partial^ {2}}{\partial y ^ {2}} g = q g \left(\frac {1}{\psi} \frac {\partial^ {2}}{\partial y ^ {2}} \psi + \frac {q - 1}{\psi^ {2}} \left(\frac {\partial}{\partial y} \psi\right) ^ {2}\right),} \end{array}
$$

and then plugging into (8.14) with chosen parameter $q = 1 / ( 1 { + } \rho ^ { 2 } )$ yields a linear equation: 

$$
\left(\frac {\partial}{\partial t} + \frac {\beta^ {2} (y)}{2} \frac {\partial^ {2}}{\partial y ^ {2}} + \left(\alpha (y) - \rho \frac {(\mu - r) \beta (y)}{\sigma (y)}\right) \frac {\partial}{\partial y}\right) \psi (t, y) - \frac {(\mu - r) ^ {2}}{2 q \sigma^ {2} (y)} \psi (t, y) = 0.\tag{8.15}
$$

Example 8.5.1 (Fully Afine Heston Model). Consider a futures contract $F _ { t , T }$ with settlement date $T$ and stochastic volatility and returns, 

$$
\begin{array}{c} \frac {d F _ {t , T}}{F _ {t , T}} = \mu Y _ {t} d t + \sqrt {Y _ {t}} d W _ {t} \\ d Y _ {t} = \kappa (\bar {Y} - Y _ {t}) d t + \beta \sqrt {Y _ {t}} d B _ {t} \end{array}
$$

where $\beta ^ { 2 } \leq 2 \kappa \bar { Y }$ and $d W _ { t } d B _ { t } = \rho d t$ . The wealth process for futures trading is 

$$
d X _ {t} = r X _ {t} d t + \pi_ {t} \frac {d F _ {t , T}}{F _ {t , T}}.
$$

For $\begin{array} { r } { U ( x ) = - \frac { 1 } { \gamma } e ^ { - \gamma x } } \end{array}$ the optimal terminal expected utility is 

$$
V (t, x, y) = U (x e ^ {r (T - t)}) \psi (t, y) ^ {q},
$$

where $\psi ( t , y )$ is similar to a solution to equation (8.15), except the equation has no $r ,$ 

$$
\left(\frac {\partial}{\partial t} + \frac {\beta^ {2} y}{2} \frac {\partial^ {2}}{\partial y ^ {2}} + (\kappa (\bar {Y} - y) - \rho \mu \beta y) \frac {\partial}{\partial y}\right) \psi (t, y) - \frac {\mu^ {2} y}{2 q} \psi (t, y) = 0.
$$

It can be further shown that the solution to this equation is of the form 

$$
\psi (t, y) = e ^ {a (t) y + b (t)},
$$

with $a ( T ) = b ( T ) = 0$ , and where $a ( t )$ and $b ( t )$ satisfy ODEs, 

$$
\begin{array}{r} a ^ {\prime} (t) + \frac {\beta^ {2}}{2} a ^ {2} (t) - (\kappa + \rho \mu \beta) a (t) - \frac {\mu^ {2}}{2 q} = 0 \\ b ^ {\prime} (t) + \kappa \bar {Y} a (t) = 0, \end{array}
$$

both of which can be solved explicitly. 

## 8.6 Indiference Pricing

Stochastic control for terminal wealth can be implemented to find the the price of a call option under stochastic volatility, 

$$
V ^ {h} (t, x, y, s) = \max _ {\pi} \mathbb {E} \left[ U (X _ {T} - (S _ {T} - K) ^ {+}) \Big | X _ {t} = x, Y _ {t} = y, S _ {t} = s \right],
$$

where the investor now hedges a short position in a call option with strike K. Compared to the same investor’s value function that is not short the call 

$$
V ^ {0} (t, x, y) = \max _ {\pi} \mathbb {E} \left[ U (X _ {T}) \Big | X _ {t} = x, Y _ {t} = y \right],
$$

we look for the amount of cash $\$ 9$ such that the 

$$
V ^ {h} (t, x + p, y, s) = V ^ {0} (t, x, y).
$$

The extra cash makes the hedger utility indiferent to the short position. With exponential utility there is a separation of variables, 

$$
\begin{array}{r l} & V (t, x, y, s) = \max _ {\pi} \mathbb {E} \left[ - \frac {1}{\gamma} e ^ {- \gamma (X _ {T} - (S _ {T} - K) ^ {+})} \Big | X _ {t} = x, Y _ {t} = y, S _ {t} = s \right] \\ & \qquad = - \frac {1}{\gamma} e ^ {- \gamma x e ^ {r (T - t)}} \min _ {\pi} \mathbb {E} \left[ e ^ {- \gamma \left(\int_ {t} ^ {T} e ^ {r (T - u)} \pi_ {u} \left(\frac {d S _ {u}}{S _ {u}} - r d u\right) - (S _ {T} - K) ^ {+}\right)} \Big | Y _ {t} = y, S _ {t} = s \right] \\ & \qquad = U (x e ^ {r (T - t)}) g ^ {h} (t, y, s), \end{array}
$$

where we’ve used the diferential $\begin{array} { r } { d \left( e ^ { r ( T - t ) } X _ { t } \right) = e ^ { r ( T - t ) } \pi _ { t } \left( \frac { d S _ { t } } { S _ { t } } - r d t \right) } \end{array}$ . Hence we find a price $\$ 9$ such that $U \left( p e ^ { r ( T - t ) } \right) = g ( t , y ) / g ^ { h } ( t , y , s )$ , where $g ( t , y )$ is the solution from (8.13). 

Depending on the risk-aversion coeficient $\gamma _ { ; }$ , there will be diferent prices $\$ 9$ . This brings us back to the price of volatility risk $\Lambda ( t , s , x )$ from Proposition 7.1.1 of Chapter 7. Namely, investors with diferent risk aversion will have a diferent Λ for their martingale evaluation of the call option. 

If an indiference price is obtained then there is a solution to both optimization problems, and hence there is no-arbitrage and the range of prices for $c will be a no-arbitrage interval. For complete markets there will be a single price $c for all levels of risk aversion. 

Appendices 

# Appendix A

# Martingales and Stopping Times

Let $\mathcal { F } _ { t }$ denote a σ-algebra. A process $X _ { t }$ is an F<sub>t</sub>-martingale if and only if 

$$
\mathbb {E} _ {t} X _ {T} = X _ {t} \quad \forall t \leq T,
$$

where $\mathbb { E } _ { t } = \mathbb { E } [ { \mathbf { \mu } } \cdot { \mathbf { \mu } } | { \mathcal { F } } _ { t } ]$ . A process $X _ { t }$ is a submartingale if and only if 

$$
\mathbb {E} _ {t} X _ {T} \geq X _ {t} \quad \forall t \leq T,
$$

and a supermartingale if and only if 

$$
\mathbb {E} _ {t} X _ {T} \leq X _ {t} \quad \forall t \leq T.
$$

Note that true martingale is both a sub and supermartingale. 

## A.1 Stopping Times

In probability theory, a stopping time is a a stochastic time that is non-anticipative of the underlying process. For instance, for a stock price $S _ { t }$ a stopping time is the first time the price reaches a level M, 

$$
\tau = \inf \{t > 0 | S _ {t} \geq M \}.
$$

The non-anticipativeness of the stopping is important because there are some events that are seemingly similar but are not stopping times, for instance 

$$
\nu = \sup \{t > 0 | S _ {t} <   M \}
$$

is not a stopping time. 

Stopping times are useful when discussing martingales. For example, so-called stoppedprocesses inherit the sub or supermartingale property. Namely, $X _ { t \wedge \tau }$ is a sub or supermartingale of $X _ { t }$ is a sub or supermartingale, respectively. There is also the optional stopping theorem: 

Theorem A.1.1 (Optional Stopping Theorem). Let $X _ { t }$ be $a$ submartingale and let τ be a stopping time. $I f \ \tau < \infty \ a . s ,$ . and $X _ { t \wedge \tau }$ uniformly integrable, then $\mathbb { E } X _ { 0 } \leq \mathbb { E } X _ { \tau }$ with equality if $X _ { t }$ is a martingale. 

An example application of the optional stopping theorem is Gambler’s ruin: Let 

$$
\tau = \inf \left\{t > 0 \mid W _ {t} \notin (a, b) \right\},
$$

where $0 < b < \infty$ and $- \infty < a < 0$ . Then $\mathbb { P } ( \tau < \infty ) = 1$ and by optional stopping, 

$$
\begin{array}{l} 0 = W _ {0} = \mathbb {E} W _ {\tau} \\ \quad = a \mathbb {P} (W _ {\tau} = a) + b (1 - \mathbb {P} (W _ {\tau} = a)) \\ \quad = (a - b) \mathbb {P} (W _ {\tau} = a) + b, \end{array}
$$

which can be simplified to get 

$$
\mathbb {P} (W _ {\tau} = a) = \frac {b}{b - a}.
$$

## A.2 Local Martingales

First define a local martingale: 

Definition A.2.1 (Local Martingale). A process $X _ { t }$ is a local martingale if there exists a sequence of finite and increasing stopping times $\tau _ { n }$ such that $\mathbb { P } ( \tau _ { n } \to \infty \ a s \ n \to \infty ) = 1$ and $X _ { t \wedge \tau _ { n } }$ is a true martingale for any n. 

Some remarks are in order: 

Remark 3. In discrete time there are no local martingales; a martingale is a martingale. 

Remark 4. A true martingale $X _ { t }$ is a local martingale, and any bounded local martingale is in fact a true martingale. 

The Itˆo stochastic integral is in general a local martingale, not necessarily a true martingale. That is, 

$$
I _ {t} = \int_ {0} ^ {t} \sigma_ {u} d W _ {u},
$$

is only a local martingale, but there exists stopping times $\tau _ { n }$ such that 

$$
I _ {t \wedge \tau_ {n}} = \int_ {0} ^ {t \wedge \tau_ {n}} \sigma_ {u} d W _ {u},
$$

is a true martingale. For Itˆo integrals there is the following theorem for a suficient (but not necessary) condition for true martingales: 

Theorem A.2.1. The Itˆo integral $\textstyle \int _ { 0 } ^ { t } \sigma _ { u } d W _ { u }$ is a true martingale on [0, T] if 

$$
\mathbb {E} \int_ {0} ^ {T} \sigma_ {s} ^ {2} d s <   \infty ,
$$

i.e., the Itˆo isometry is finite. 

For the stochastic integral $\begin{array} { r } { I _ { t } = \int _ { 0 } ^ { t } \sigma _ { u } d W _ { u } } \end{array}$ we can define 

$$
\tau_ {n} = \inf \left\{t > 0 \middle | \int_ {0} ^ {t} \sigma_ {u} ^ {2} d s \geq n \right\} \wedge T,
$$

for which we have a bounded Itˆo isometry, and hence Theorem A.2.1 applies to make $I _ { t \wedge \tau _ { r } }$ a martingale on [0, T]. 

An example of a local martingale is the constant elasticity of volatility (CEV) model, 

$$
d S _ {t} = \sigma S _ {t} ^ {\alpha} d W _ {t},
$$

with $0 \leq \alpha \leq 2 ; S _ { t }$ is strictly a local martingale for $1 < \alpha \leq 2$ . For $\alpha = 2$ one can check using PDEs that the transition density is 

$$
p _ {t} (z | s) = \frac {s}{z ^ {3} \sqrt {2 \pi t \sigma^ {2}}} \left(e ^ {- \frac {\left(\frac {1}{z} - \frac {1}{s}\right) ^ {2}}{2 t \sigma^ {2}}} - e ^ {- \frac {\left(\frac {1}{z} + \frac {1}{s}\right) ^ {2}}{2 t \sigma^ {2}}}\right).
$$

One can check that $\mathbb { E } S _ { t } ^ { 4 } = \infty$ for all $t > 0$ so that Theorem A.2.1 does not apply, but to see that it is a strict local martingale one must also check that $\mathbb { E } _ { t } S _ { T } < S _ { t }$ for all $t < T$ 

## Appendix B

# Some Notes on Fourier Transforms

For a real-valued function $f ( x )$ with $\textstyle \int _ { - \infty } ^ { \infty } | f ( x ) | ^ { 2 } d x < \infty$ , Fourier transforms are defined as follows 

$$
\widehat {f} (u) = \int_ {- \infty} ^ {\infty} e ^ {i u x} f (x) d x\tag{B.1}
$$

$$
f (x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \widehat {f} (u) d u.\tag{B.2}
$$

The Fourier transforms in (B.1) and (B.2) are somewhat diferent from traditional definitions, which are 

$$
\begin{array}{l} \widehat {f} (u) = \int_ {- \infty} ^ {\infty} e ^ {- 2 \pi i u x} f (x) d x \\ f (x) = \int_ {- \infty} ^ {\infty} e ^ {2 \pi i u x} \widehat {f} (u) d u. \end{array}
$$

The reason we choose (B.1) in finance is because we work so much with probability theory, and as probabilists we like to have a Fourier transform of a density be equal to a characteristic function. However, nothing changes and we are able to carry out all the same calculations; the diference amounts merely to a change of variable inside the integrals. 

## B.1 Some Basic Properties

• Linearity: if $\psi ( s ) = a f ( s ) + b g ( s )$ , then 

$$
\widehat {\psi} (u) = a \widehat {f} (u) + b \widehat {g} (u).
$$

• Translation/Time Shifting: if $f ( s ) = \psi ( s - s _ { 0 } )$ , then 

$$
\widehat {f} (u) = e ^ {i u s _ {0}} \widehat {\psi} (u).
$$

• Convolution: for $\begin{array} { r } { f * g ( x ) = \int _ { - \infty } ^ { \infty } f ( y ) g ( x - y ) d y } \end{array}$ , 

$$
\begin{array}{l} \widehat {f * g} (u) = \int_ {- \infty} ^ {\infty} e ^ {i u x} \int_ {- \infty} ^ {\infty} f (y) g (x - y) d y d x \\ \qquad = \int_ {- \infty} ^ {\infty} e ^ {i u y} f (y) \int_ {- \infty} ^ {\infty} e ^ {i u (x - y)} g (x - y) d x d y \\ \qquad = \int_ {- \infty} ^ {\infty} e ^ {i u y} f (y) \widehat {g} (u) d y \\ \qquad = \widehat {f} (u) \widehat {g} (u). \end{array}
$$

• Reverse Convolution: 

$$
\begin{array}{l} \widehat {\widehat {f} * \widehat {g}} (x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \int_ {- \infty} ^ {\infty} \widehat {f} (v) \widehat {g} (u - v) d v d u \\ \qquad = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i v x} \widehat {f} (v) \int_ {- \infty} ^ {\infty} e ^ {- i (u - v) x} \widehat {g} (u - v) d u d v \\ \qquad = g (x) \int_ {- \infty} ^ {\infty} e ^ {- i v x} \widehat {f} (v) d v \\ \qquad = 2 \pi g (x) f (x). \end{array}
$$

An important concept to realize about Fourier is that functions $( e ^ { i u x } ) _ { u \in \mathbb { R } }$ can be thought of as orthonormal basis elements in a linear space. Similar to finite-dimensional vector spaces, we can write a function as a some inner products with the basis elements. Indeed, that is what we accomplish with the inverse Fourier transform; we can think of the integral as a sum, 

$$
f (x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \widehat {f} (u) d u \approx \frac {1}{2 \pi} \sum_ {n = 1} ^ {N} e ^ {- i u _ {n} x} \widehat {f} (u _ {n}),
$$

where $u _ { n }$ are discrete points $\mathbb { C }$ (this is a similar idea to Fast Fourier Transforms (FFT)). The basis elements are orthogonal in the sense that 

$$
\frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {i u x} e ^ {- i v x} d x = \delta_ {0} (u - v).
$$

Finally, it needs to be pointed out that the function $\delta _ { 0 }$ is something that defined under integrals, and is rather hard to formalize outside. For instance, in Parseval’s identity, we used $\delta _ { 0 }$ , but only inside the integral: 

Proposition B.1.1. For a real-valued function f(x) with $\textstyle \int _ { - \infty } ^ { \infty } | f ( x ) | ^ { 2 } d x < \infty$ 

$$
\int_ {- \infty} ^ {\infty} | f (x) | ^ {2} d s = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} | \widehat {f} (u) | ^ {2} d u.
$$

Proof. 

$$
\begin{array}{r l} & {\frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} | \widehat {f} (u) | ^ {2} d u = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \widehat {f} (u) \overline {{\widehat {f} (u)}} d u} \\ & {\qquad = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} e ^ {i u x} f (x) e ^ {- i u y} f (y) d x d y d u} \\ & {\qquad = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} f (x) f (y) \left(\int_ {- \infty} ^ {\infty} e ^ {i u x} e ^ {- i u y} d u\right) d x d y} \\ & {\qquad = \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} f (x) f (y) \delta_ {0} (y - x) d x d y} \\ & {\qquad = \int_ {- \infty} ^ {\infty} f (x) f (x) d x.} \end{array}
$$

## B.2 Regularity Strips

For some function $f : \mathbb { R } \to \mathbb { R }$ we modify (B.1) and (B.2) to accommodate non-integrability and/or non-diferentiability. We write 

$$
\begin{array}{l} \widehat {f} (u) = \int_ {- \infty} ^ {\infty} e ^ {i u x} f (x) d x \\ f (x) = \frac {1}{2 \pi} \int_ {i z - \infty} ^ {i z + \infty} e ^ {- i u x} \widehat {f} (u) d u. \end{array}
$$

where $z = \Im ( u )$ . The region of z values where the Fourier transform is defined is called the regularity strip. This comes in handy for functions like the European call and put payofs. 

Example B.2.1 (Call Option). For a call option, $f ( x ) = ( e ^ { s } - K ) ^ { + }$ . This function has $\begin{array} { r } { \int _ { \log K } ^ { \infty } | f ( s ) | ^ { 2 } d s = \infty } \end{array}$ and non-diferentiability at $s = \log ( K )$ . However, we can still write a Fourier transform: 

$$
\begin{array}{r l} & {\widehat {f} (u) = \int_ {- \infty} ^ {\infty} e ^ {i u s} (e ^ {s} - K) ^ {+} d s} \\ & {\quad = \int_ {\log K} ^ {\infty} e ^ {s + i u s} d s - K \int_ {\log K} ^ {\infty} e ^ {i u s} d s} \\ & {\quad = \frac {e ^ {s + i u s}}{1 + i u} \Big | _ {s = \log K} ^ {\infty} - \frac {K e ^ {i u s}}{i u} \Big | _ {s = \log K} ^ {\infty}.} \end{array}
$$

where the anti-derivative of $e ^ { i u s }$ and $e ^ { s + i u s }$ are the same as they are for real variables because the function is analytic in the complex plain. For $z = \mathbb { S } ( u ) > 1$ , the anti-derivative will be zero when evaluated at $s = \infty$ , will be infinite for $z < 1$ , and undefined for $z = 1$ Taking $z > 1$ , we have 

$$
\begin{array}{r l} & {\widehat {f} (u) = - \frac {e ^ {(1 + i u) \log (K)}}{1 + i u} + \frac {K e ^ {i u \log (K)}}{i u}} \\ & {\qquad = - \frac {\left(e ^ {\log (K)}\right) ^ {(1 + i u)}}{1 + i u} + \frac {K \left(e ^ {\log (K)}\right) ^ {i u}}{i u}} \\ & {\qquad = \frac {K ^ {1 + i u}}{i u - u ^ {2}},} \end{array}
$$

as shown in Table 7.1 of Chapter 7. 

Example B.2.2 (PutOption). For a put option, $f ( x ) = ( K - e ^ { s } ) ^ { + }$ . This function has $\begin{array} { r } { \int _ { \log K } ^ { \infty } | f ( s ) | ^ { 2 } d s < \dot { \infty } } \end{array}$ , like the put option is non-diferentiability at s = log(K). Repeating the steps from the previous example, it follows that the regularity strip is $z = \mathbb { S } ( u ) < 0$ (see Table 7.1 of Chapter 7). 

## B.3 The Wave Equation

Consider the wave (transport) equation, 

$$
\begin{array}{c} \frac {\partial}{\partial t} V (t, x) = a \frac {\partial}{\partial x} V (t, x) \\ V (0, x) = f (x). \end{array}
$$

The solution can be found with Fourier transforms: 

$$
\begin{array}{c} \left(\frac {\partial}{\partial t} - a \frac {\partial}{\partial x}\right) V (t, x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \left(\frac {\partial}{\partial t} - a \frac {\partial}{\partial x}\right) e ^ {- i u x} \widehat {V} (t, u) \\ = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \left(\frac {\partial}{\partial t} + a i u\right) \widehat {V} (t, u), \end{array}
$$

or simply 

$$
\begin{array}{c} \frac {\partial}{\partial t} \widehat {V} (t, u) = - a i u \widehat {V} (t, u), \\ \widehat {V} (0, u) = \widehat {f} (0). \end{array}
$$

The solution is 

$$
\widehat {V} (t, u) = e ^ {- a i u t} \widehat {f} (u),
$$

which we invert to obtain the solution to the wave equation, 

$$
\begin{array}{l} V (t, x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} e ^ {- a i u t} \widehat {f} (u) d u \\ \qquad = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u (x + a t)} \widehat {f} (u) d u \\ \qquad = f (x + a t). \end{array}
$$

The lines $x = c - a t$ are the characteristic lines so that for any c we have $v ( t , c - a t ) = f ( c )$ ; the initial information $f ( c )$ at point c is propagated along the characteristic line. 

## B.4 The Heat Equation

Consider the heat equation 

$$
\begin{array}{c} \frac {\partial}{\partial t} V (t, x) = \frac {1}{2} \Delta V (t, x) \\ V (0, x) = f (x), \end{array}
$$

where and $\textstyle \int _ { - \infty } ^ { \infty } | f ( x ) | ^ { 2 } d x < \infty$ . For scalar x we have $\begin{array} { r } { \Delta = \frac { \partial ^ { 2 } } { \partial x ^ { 2 } } } \end{array}$ , and the inverse Fourier transform yields an ODE under the integral sign, 

$$
\begin{array}{r l} & {\left(\frac {\partial}{\partial t} - \frac {1}{2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) V (t, x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \left(\frac {\partial}{\partial t} - \frac {1}{2} \frac {\partial^ {2}}{\partial x ^ {2}}\right) e ^ {- i u x} \widehat {V} (t, u) d u} \\ & {\qquad = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \left(\frac {\partial}{\partial t} + \frac {u ^ {2}}{2}\right) \widehat {V} (t, u) d u} \\ & {\qquad = 0,} \end{array}
$$

or simply, 

$$
\begin{array}{c} \frac {d}{d t} \widehat {V} (t, u) = - \frac {u ^ {2}}{2} \widehat {V} (t, u) \\ \widehat {V} (0, u) = \widehat {f} (u). \end{array}\tag{B.3}
$$

The solution to (B.3) is 

$$
\widehat {V} (t, u) = \widehat {f} (u) e ^ {- \frac {u ^ {2}}{2} t}.
$$

Applying the inverse Fourier transform yields the solution, 

$$
\begin{array}{r l} & V (t, x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \widehat {V} (t, u) d u \\ & \quad = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \widehat {f} (u) e ^ {- \frac {u ^ {2}}{2} t} d u \\ & \quad = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \left(\int_ {- \infty} ^ {\infty} e ^ {i u y} f (y) d y\right) e ^ {- \frac {u ^ {2}}{2} t} d u \\ & \quad = \frac {1}{\sqrt {2 \pi t}} \int_ {- \infty} ^ {\infty} f (y) \left(\sqrt {\frac {t}{2 \pi}} \int_ {- \infty} ^ {\infty} e ^ {i u (y - x)} e ^ {- \frac {u ^ {2}}{2} t} d u\right) d y \\ & \quad = \frac {1}{\sqrt {2 \pi t}} \int_ {- \infty} ^ {\infty} f (y) \left(\mathbb {E} e ^ {i \mathcal {Z} (y - x) / \sqrt {t}}\right) d y \qquad \mathrm{where} \mathcal {Z} \sim N (0, 1) \\ & \quad = \frac {1}{\sqrt {2 \pi t}} \int_ {- \infty} ^ {\infty} f (y) e ^ {- \frac {(y - x) ^ {2}}{2 t}} d y. \end{array}
$$

In fact, it can be seen as the expectation of a Brownian motion, 

$$
V (t, x) = \mathbb {E} f (x + W _ {t})
$$

where $W _ { t }$ is a Brownian motion. If $f ( x ) = \delta _ { 0 } ( x )$ , then the we have the fundamental solution, 

$$
\Phi (t, x) = \frac {1}{\sqrt {2 \pi t}} e ^ {- \frac {x ^ {2}}{2 t}},
$$

from which solutions for diferent initial conditions are convolutions, 

$$
V (t, x) = f * \Phi (t, x) = \int_ {- \infty} ^ {\infty} f (y) \Phi (t, x - y).
$$

## B.5 The Black-Scholes Equation

The Black-Scholes model is 

$$
\frac {d S _ {t}}{S _ {t}} = r d t + \sigma d W _ {t} ^ {Q}
$$

where $W ^ { Q }$ is a risk-neutral Brownian motion. Letting $X _ { t } ~ = ~ \log ( S _ { t } )$ the Black-Scholes equation is 

$$
\begin{array}{c} \left(\frac {\partial}{\partial t} + \frac {\sigma^ {2}}{2} \frac {\partial^ {2}}{\partial x ^ {2}} + \left(r - \frac {\sigma^ {2}}{2}\right) \frac {\partial}{\partial x} - r\right) V (t, x) = 0 \\ V (T, x) = \psi (x), \end{array}
$$

where $\psi ( X _ { T } )$ is the claim, e.g. a call option $\psi ( x ) = ( e ^ { x } - K ) ^ { + }$ . Using the same Fourier techniques as we did with the wave and heat equations, we have 

$$
\begin{array}{r} \left(\frac {\partial}{\partial t} - \frac {\sigma^ {2} u ^ {2}}{2} - i u \left(r - \frac {\sigma^ {2}}{2}\right) - r\right) \widehat {V} (t, u) = 0 \\ \widehat {V} (T, u) = \widehat {\psi} (u), \end{array}
$$

which has solution 

$$
\widehat {V} (t, u) = \widehat {\psi} (u) e ^ {- (T - t) \left(\frac {\sigma^ {2} u ^ {2}}{2} + i u \left(r - \frac {\sigma^ {2}}{2}\right) + r\right)}.
$$

Applying the inverse Fourier transform, we arrive at the risk-neutral pricing formula (i.e. Feynman-Kac), 

$$
\begin{array}{l} V (t, x) = \frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \widehat {V} (t, u) d u \\ \qquad = \frac {e ^ {- r (T - t)}}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \widehat {\psi} (u) e ^ {- (T - t) \left(\frac {\sigma^ {2} u ^ {2}}{2} + i u \left(r - \frac {\sigma^ {2}}{2}\right)\right)} d u \\ \qquad = \frac {e ^ {- r (T - t)}}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- i u x} \left(\int_ {- \infty} ^ {\infty} e ^ {i u y} \psi (y) d y\right) e ^ {- (T - t) \left(\frac {\sigma^ {2} u ^ {2}}{2} + i u \left(r - \frac {\sigma^ {2}}{2}\right)\right)} d u \\ \qquad = \frac {e ^ {- r (T - t)}}{2 \pi} \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} \psi (y) e ^ {i u \left(y - x - (T - t) \left(r - \frac {\sigma^ {2}}{2}\right)\right)} e ^ {- (T - t) \frac {\sigma^ {2} u ^ {2}}{2}} d u d y. \end{array}
$$

Take change of variable $\begin{array} { r } { y ^ { \prime } = y - x - \left( T - t \right) \left( r - \frac { \sigma ^ { 2 } } { 2 } \right) } \end{array}$ such that $d y ^ { \prime } = d y$ , then 

$$
\begin{array}{r l} & V (t, x) = \frac {e ^ {- r (T - t)}}{2 \pi} \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} \psi \left(y ^ {\prime} + x + (T - t) \left(r - \frac {\sigma^ {2}}{2}\right)\right) e ^ {i u y ^ {\prime}} e ^ {- (T - t) \frac {\sigma^ {2} u ^ {2}}{2}} d u d y ^ {\prime} \\ & \quad = \frac {e ^ {- r (T - t)}}{2 \pi} \int_ {- \infty} ^ {\infty} \psi \left(y ^ {\prime} + x + (T - t) \left(r - \frac {\sigma^ {2}}{2}\right)\right) \left(\int_ {- \infty} ^ {\infty} e ^ {i u y ^ {\prime}} e ^ {- (T - t) \frac {\sigma^ {2} u ^ {2}}{2}} d u\right) d y ^ {\prime} \\ & \quad = \frac {e ^ {- r (T - t)}}{\sqrt {2 \pi \sigma^ {2} (T - t)}} \int_ {- \infty} ^ {\infty} \psi \left(y ^ {\prime} + x + (T - t) \left(r - \frac {\sigma^ {2}}{2}\right)\right) \left(\mathbb {E} e ^ {i \frac {\mathcal {Z}}{\sigma \sqrt {T - t}} y ^ {\prime}}\right) d y ^ {\prime} \\ & \quad = \frac {e ^ {- r (T - t)}}{\sqrt {2 \pi \sigma^ {2} (T - t)}} \int_ {- \infty} ^ {\infty} \psi \left(y ^ {\prime} + x + (T - t) \left(r - \frac {\sigma^ {2}}{2}\right)\right) e ^ {- \frac {1}{2} \frac {(y ^ {\prime}) ^ {2}}{\sigma^ {2} (T - t)}} d y ^ {\prime} \\ & \quad = e ^ {- r (T - t)} \mathbb {E} ^ {Q} \psi \left(x + (T - t) \left(r - \frac {\sigma^ {2}}{2}\right) + \sigma (W _ {T} ^ {Q} - W _ {t} ^ {Q})\right) \\ & \quad = e ^ {- r (T - t)} \mathbb {E} ^ {Q} \left[ \psi (X _ {T}) | X _ {t} = x \right]. \end{array}
$$

## Bibliography



[Achdou and Pironneau, 2005] Achdou, Y. and Pironneau, O. (2005). Computational Methods for Option Pricing. SIAM Press. 





[Bj¨ork, 2000] Bj¨ork, T. (2000). Arbitrage Theory in Continuous Time. Oxford University Press, 2nd edition. 





[Black and Scholes, 1973] Black, F. and Scholes, M. (1973). The pricing of options and corporate liabilities. Journal of Political Economy, 81(3):637–54. 





[Carr et al., 1999] Carr, P., Madan, D., and Smith, R. (1999). Option valuation using the fast Fourier transform. Journal of Computational Finance, 2:61–73. 





[Cont. and Tankov, 2003] Cont., R. and Tankov, P. (2003). Financial modelling with Jump Processes. 





[Dufie et al., 2000] Dufie, D., Pan, J., and Singleton, K. (2000). Transform analysis and asset pricing for afine jump-difusions. Econometrica, 68:1343–1376. 





[Dupire, 1994] Dupire, B. (1994). Pricing with a smile. Risk, 7(1):18–20. 





[Gatheral, 2006] Gatheral, J. (2006). The Volatility Surface: A Practitioner’s Guide. Wiley. 





[Glasserman, 2004] Glasserman, P. (2004). Monte Carlo Methods in Financial Engineering. Springer. 





[Harrison and Pliska, 1981] Harrison, M. and Pliska, S. (1981). Martingales and stochastic integrals in the theory of continuous trading. Stochastic Processes and their Applications, (3):215–260. 





[Lee, 2004] Lee, R. W. (2004). The moment formula for implied volatility at extreme strikes. Mathematical Finance, 14(3):469–480. 





[Lewis, 2000] Lewis, A. L. (2000). Option Valuation under Stochastic Volatility with Mathematica Code. Finance Press. 





[Merton, 1973] Merton, R. (1973). On the pricing of corporate debt: the risk structure of interest rates. Technical report. 





[Øksendal, 2003] Øksendal, B. (2003). Stochastic diferential equations: an introduction with applications. Springer. 





[Schachermayer, 1992] Schachermayer, W. (1992). A Hilbert space proof of the fundamental theorem of asset pricing in finite discrete time. Insurance: Mathematics and Economics, 11(4):249– 257. 

