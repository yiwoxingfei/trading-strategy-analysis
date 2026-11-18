

<!-- === Source: MinerU_markdown_Introduction_to_Computational_Finance_without_Agonizing_pain_1_2122707067558010899.md (Page 1) === -->

# An Introduction to Computational Finance Without Agonizing Pain

c Peter Forsyth 2007 

P.A. Forsyth<sup>∗</sup> 

February 12, 2007 

## Contents

1 The First Option Trade 3   
2 The Black-Scholes Equation 3   
2.1 Background . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3   
2.2 Definitions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4   
2.3 A Simple Example: The Two State Tree 4   
2.4 A hedging strategy 5   
2.5 Brownian Motion 5   
2.6 Geometric Brownian motion with drift 9   
2.6.1 Ito's Lemma 11   
2.6.2 Some uses of Ito's Lemma 12   
2.6.3 Some more uses of Ito's Lemma 12   
2.7 The Black-Scholes Analysis 14   
2.8 Hedging in Continuous Time 15   
2.9 The option price 16   
2.10 American early exercise 16   
3 The Risk Neutral World 17   
4 Monte Carlo Methods 19   
4.1 Monte Carlo Error Estimators 21   
4.2 Random Numbers and Monte Carlo 21   
4.3 The Box-Muller Algorithm 22   
4.3.1 An improved Box Muller 24   
4.4 Speeding up Monte Carlo 26   
4.5 Estimating the mean and variance 27   
4.6 Low Discrepancy Sequences 27   
4.7 Correlated Random Numbers 29 

4.8 Integration of Stochastic Differential Equations 30  
4.8.1 The Brownian Bridge 31  
4.8.2 Strong and Weak Convergence 32  
4.9 Matlab and Monte Carlo Simulation 35  

5 The Binomial Model 37  
5.1 A No-arbitrage Lattice 39  

6 More on Ito's Lemma 41  

7 Derivative Contracts on non-traded Assets and Real Options 44  
7.1 Derivative Contracts 44  
7.2 A Forward Contract 47  
7.2.1 Convenience Yield 48  
7.2.2 Volatility of Foward Prices 49  

8 Discrete Hedging 49  
8.1 Delta Hedging 49  
8.2 Gamma Hedging 52  
8.3 Vega Hedging 53  

9 Jump Diffusion 54  
9.1 The Poisson Process 55  
9.2 The Jump Diffusion Pricing Equation 56  
9.3 An Alternate Derivation of the Pricing Equation for Jump Diffusion 59  

10 Regime Switching 62  

11 Mean Variance Portfolio Optimization 64  
11.1 Special Cases 65  
11.2 The Portfolio Allocation Problem 66  
11.3 Adding a Risk-free asset 69  
11.4 Criticism 70  
11.5 Individual Securities 71  

12 Stocks for the Long Run? 74  

13 Further Reading 75  
13.1 General Interest 75  
13.2 More Background 77  
13.3 More Technical 77 “Men wanted for hazardous journey, small wages, bitter cold, long months of complete darkness, constant dangers, safe return doubtful. Honour and recognition in case of success.” Advertisement placed by Earnest Shackleton in 1914. He received 5000 replies. An example of extreme risk-seeking behaviour. Hedging with options is used to mitigate risk, and would not appeal to members of Shackleton’s expedition. 

## 1 The First Option Trade

Many people think that options and futures are recent inventions. However, options have a long history, going back to ancient Greece. 

As recorded by Aristotle in Politics, the fifth century BC philosopher Thales of Miletus took part in a sophisticated trading strategy. The main point of this trade was to confirm that philosophers could become rich if they so chose. This is perhaps the first rejoinder to the famous question “If you are so smart, why aren’t you rich?” which has dogged academics throughout the ages. 

Thales observed that the weather was very favourable to a good olive crop, which would result in a bumper harvest of olives. If there was an established Athens Board of Olives Exchange, Thales could have simply sold olive futures short (a surplus of olives would cause the price of olives to go down). Since the exchange did not exist, Thales put a deposit on all the olive presses surrounding Miletus. When the olive crop was harvested, demand for olive presses reached enormous proportions (olives were not a storable commodity). Thales then sublet the presses for a profit. Note that by placing a deposit on the presses, Thales was actually manufacturing an option on the olive crop, i.e. the most he could lose was his deposit. If had sold short olive futures, he would have been liable to an unlimited loss, in the event that the olive crop turned out bad, and the price of olives went up. In other words, he had an option on a future of a non-storable commodity. 

## 2 The Black-Scholes Equation

This is the basic PDE used in option pricing. We will derive this PDE for a simple case below. Things get much more complicated for real contracts. 

## 2.1 Background

Over the past few years derivative securities (options, futures, and forward contracts) have become essential tools for corporations and investors alike. Derivatives facilitate the transfer of financial risks. As such, they may be used to hedge risk exposures or to assume risks in the anticipation of profits. To take a simple yet instructive example, a gold mining firm is exposed to fluctuations in the price of gold. The firm could use a forward contract to fix the price of its future sales. This would protect the firm against a fall in the price of gold, but it would also sacrifice the upside potential from a gold price increase. This could be preserved by using options instead of a forward contract. 

Individual investors can also use derivatives as part of their investment strategies. This can be done through direct trading on financial exchanges. In addition, it is quite common for financial products to include some form of embedded derivative. Any insurance contract can be viewed as a put option. Consequently, any investment which provides some kind of protection actually includes an option feature. Standard examples include deposit insurance guarantees on savings accounts as well as the provision of being able to redeem a savings bond at par at any time. These types of embedded options are becoming increasingly common and increasingly complex. A prominent current example are investment guarantees being ofered by insurance companies (“segregated funds”) and mutual funds. In such contracts, the initial investment is guaranteed, and gains can be locked-in (reset) a fixed number of times per year at the option of the contract holder. This is actually a very complex put option, known as a shout option. How much should an investor be willing to pay for this insurance? Determining the fair market value of these sorts of contracts is a problem in option pricing. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/f042f679d04328c4a5d1a3297ef4ae4a252e3e5a16379354a600641818a635db.jpg)



Figure 2.1: A simple case where the stock value can either be $22 or $18, with a European call option, $K =$ $21.


## 2.2 Definitions

Let’s consider some simple European put/call options. At some time T in the future (the expiry or exercise date) the holder has the right, but not the obligation, to 

• Buy an asset at a prescribed price K (the exercise or strike price). This is a call option. 

• Sell the asset at a prescribed price K (the exercise or strike price). This is a put option. 

At expiry time $T ,$ we know with certainty what the value of the option is, in terms of the price of the underlying asset S, 

$$
\begin{array}{r l r} {\mathrm{Payoff}} & = & {\max (S - K, 0) \mathrm{foracall}} \\ {\mathrm{Payoff}} & = & {\max (K - S, 0) \mathrm{foraput}} \end{array}\tag{2.1}
$$

Note that the payof from an option is always non-negative, since the holder has a right but not an obligation. This contrasts with a forward contract, where the holder must buy or sell at a prescribed price. 

## 2.3 A Simple Example: The Two State Tree

This example is taken from Options, futures, and other derivatives, by John Hull. Suppose the value of a stock is currently $20. It is known that at the end of three months, the stock price will be either $22 or $18. We assume that the stock pays no dividends, and we would like to value a European call option to buy the stock in three months for $21. This option can have only two possible values in three months: if the stock price is $22, the option is worth $1, if the stock price is $18, the option is worth zero. This is illustrated in Figure 2.1. 

In order to price this option, we can set up an imaginary portfolio consisting of the option and the stock, in such a way that there is no uncertainty about the value of the portfolio at the end of three months. Since the portfolio has no risk, the return earned by this portfolio must be the risk-free rate. 

Consider a portfolio consisting of a long (positive) position of δ shares of stock, and short (negative) one call option. We will compute δ so that the portfolio is riskless. If the stock moves up to $22 or goes down to $18, then the value of the portfolio is 

$$
\begin{array}{r c l} \text {Value if stock goes up} & = & 2 2 \delta - 1 \\ \text {Value if stock goes down} & = & 1 8 \delta - 0 \end{array}\tag{2.2}
$$

So, if we choose δ = .25, then the value of the portfolio is 

$$
\begin{array}{r c l} \text {Value if stock goes up} & = & 2 2 \delta - 1 = 4. 5 0 \\ \text {Value if stock goes down} & = & 1 8 \delta - 0 = 4. 5 0 \end{array}\tag{2.3}
$$

So, regardless of whether the stock moves up or down, the value of the portfolio is $4.50. A risk-free portfolio must earn the risk free rate. Suppose the current risk-free rate is 12%, then the value of the portfolio today must be the present value of $4.50, or 

$$
4. 5 0 \times e ^ {-. 1 2 \times . 2 5} = 4. 3 6 7
$$

The value of the stock today is $20. Let the value of the option be V. The value of the portfolio is 

$$
\begin{array}{r c l}2 0 \times . 2 5 - V&=&4. 3 6 7\\\rightarrow&&V = . 6 3 3\end{array}
$$

## 2.4 A hedging strategy

So, if we sell the above option (we hold a short position in the option), then we can hedge this position in the following way. Today, we sell the option for $.633, borrow $4.367 from the bank at the risk free rate (this means that we have to pay the bank back $4.50 in three months), which gives us $5.00 in cash. Then, we buy .25 shares at $20.00 (the current price of the stock). In three months time, one of two things happens 

• The stock goes up to $22, our stock holding is now worth $5.50, we pay the option holder $1.00, which leaves us with $4.50, just enough to pay of the bank loan. 

• The stock goes down to $18.00. The call option is worthless. The value of the stock holding is now $4.50, which is just enough to pay of the bank loan. 

Consequently, in this simple situation, we see that the theoretical price of the option is the cost for the seller to set up portfolio, which will precisely pay of the option holder and any bank loans required to set up the hedge, at the expiry of the option. In other words, this is price which a hedger requires to ensure that there is always just enough money at the end to net out at zero gain or loss. If the market price of the option was higher than this value, the seller could sell at the higher price and lock in an instantaneous risk-free gain. Alternatively, if the market price of the option was lower than the theoretical, or fair market value, it would be possible to lock in a risk-free gain by selling the portfolio short. Any such arbitrage opportunities are rapidly exploited in the market, so that for most investors, we can assume that such opportunities are not possible (the no arbitrage condition), and therefore that the market price of the option should be the theoretical price. 

Note that this hedge works regardless of whether or not the stock goes up or down. Once we set up this hedge, we don’t have a care in the world. The value of the option is also independent of the probability that the stock goes up to $22 or down to $18. This is somewhat counterintuitive. 

## 2.5 Brownian Motion

Before we consider a model for stock price movements, let’s consider the idea of Brownian motion with drift. Suppose X is a random variable, and in time $t \to t + d t , X \to X + d X$ , where 

$$
d X = \alpha d t + \sigma d Z\tag{2.4}
$$

where αdt is the drift term, σ is the volatility, and dZ is a random term. The dZ term has the form 

$$
d Z = \phi \sqrt {d t}\tag{2.5}
$$

where $\phi$ is a random variable drawn from a normal distribution with mean zero and variance one $( \phi \sim N ( 0 , 1 )$ i.e. φ is normally distributed). 

If E is the expectation operator, then 

$$
E (\phi) = 0 \qquad E (\phi^ {2}) = 1.\tag{2.6}
$$

Now in a time interval $d t .$ , we have 

$$
\begin{array}{r c l} {E (d X)} & = & {E (\alpha d t) + E (\sigma d Z)} \\ & = & {\alpha d t,} \end{array}\tag{2.7}
$$

and the variance of $d X$ , denoted by $V a r ( d X )$ is 

$$
\begin{array}{r c l} {V a r (d X)} & = & {E ([ d X - E (d X) ] ^ {2})} \\ & = & {E ([ \sigma d Z ] ^ {2})} \\ & = & {\sigma^ {2} d t .} \end{array}\tag{2.8}
$$

Let’s look at a discrete model to understand this process more completely. Suppose that we have a discrete lattice of points. Let $X = X _ { 0 }$ at $t = 0$ Suppose that at $t = \Delta t$ ， 

$$
\begin{array}{r c l} X _ {0} & \to & X _ {0} + \Delta h    ; \quad \text {with probability p} \\ X _ {0} & \to & X _ {0} - \Delta h    ; \quad \text {with probability q} \end{array}\tag{2.9}
$$

where $p + q = 1$ . Assume that 

• X follows a Markov process, i.e. the probability distribution in the future depends only on where it is now. 

• The probability of an up or down move is independent of what happened in the past. 

• X can move only up or down $\Delta h .$ 

At any lattice point $X _ { 0 } + i \Delta h$ , the probability of an up move is $p ,$ and the probability of a down move is q. The probabilities of reaching any particular lattice point for the first three moves are shown in Figure 2.2. Each move takes place in the time interval $t \to { t + \Delta { t } }$ 

Let $\Delta X$ be the change in $X$ over the interval $t \to { t + \Delta { t } }$ . Then 

$$
\begin{array}{r c l} {E (\Delta X)} & = & {(p - q) \Delta h} \\ {E ([ \Delta X ] ^ {2})} & = & {p (\Delta h) ^ {2} + q (- \Delta h) ^ {2}} \\ & = & {(\Delta h) ^ {2},} \end{array}\tag{2.10}
$$

so that the variance of $\Delta X$ is (over $t \to { t + \Delta { t } } )$ 

$$
\begin{array}{r c l} {V a r (\Delta X)} & = & {E ([ \Delta X ] ^ {2}) - [ E (\Delta X) ] ^ {2}} \\ & = & {(\Delta h) ^ {2} - (p - q) ^ {2} (\Delta h) ^ {2}} \\ & = & {4 p q (\Delta h) ^ {2}.} \end{array}\tag{2.11}
$$

Now, suppose we consider the distribution of $X$ after n moves, so that $t = n \Delta t$ . The probability of $j$ up moves, and $( n - j )$ down moves $( P ( n , j ) )$ is 

$$
P (n, j) = \frac {n !}{j ! (n - j) !} p ^ {j} q ^ {n - j}\tag{2.12}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/c749d3ae1151ea9e0ab74badfdb217231abbbc116c1d1e7f4db06f2530c12646.jpg)



Figure 2.2: Probabilities of reaching the discrete lattice points for the first three moves.


which is just a binomial distribution. Now, if $X _ { n }$ is the value of X after n steps on the lattice, then 

$$
\begin{array}{r c l} {E (X _ {n} - X _ {0})} & = & {n E (\Delta X)} \\ {V a r (X _ {n} - X _ {0})} & = & {n V a r (\Delta X),} \end{array}\tag{2.13}
$$

which follows from the properties of a binomial distribution, (each up or down move is independent of previous moves). Consequently, from equations (2.10, 2.11, 2.13) we obtain 

$$
\begin{array}{r c l} E (X _ {n} - X _ {0}) & = & n (p - q) \Delta h \\ & = & \frac {t}{\Delta t} (p - q) \Delta h \\ V a r (X _ {n} - X _ {0}) & = & n 4 p q (\Delta h) ^ {2} \\ & = & \frac {t}{\Delta t} 4 p q (\Delta h) ^ {2} \end{array}\tag{2.14}
$$

Now, we would like to take the limit at $\Delta t \to 0$ in such a way that the mean and variance of X, after a finite time t is independent of $\Delta t .$ , and we would like to recover 

$$
\begin{array}{r c l} {d X} & = & {\alpha d t + \sigma d Z} \\ {E (d X)} & = & {\alpha d t} \\ {V a r (d X)} & = & {\sigma^ {2} d t} \end{array}\tag{2.15}
$$

as $\Delta t \to 0$ . Now, since $0 \leq p , q \leq 1$ , we need to choose ∆h = Const $\sqrt { \Delta t } .$ Otherwise, from equation (2.14) we get that $V a r ( X _ { n } - X _ { 0 } )$ is either 0 or infinite after a finite time. (Stock variances do not have either of these properties, so this is obviously not a very interesting case). 

Let’s choose $\Delta h = \sigma { \sqrt { \Delta t } }$ , which gives (from equation (2.14)) 

$$
\begin{array}{r c l} {E (X _ {n} - X _ {0})} & = & {(p - q) \frac {\sigma t}{\sqrt {\Delta t}}} \\ {V a r (X _ {n} - X _ {0})} & = & {t 4 p q \sigma^ {2}} \end{array}\tag{2.16}
$$

Now, for $E ( X _ { n } - X _ { 0 } )$ to be independent of $\Delta t$ as $\Delta t \to 0 .$ , we must have 

$$
(p - q) = C o n s t. \sqrt {\Delta t}\tag{2.17}
$$

If we choose 

$$
p - q = \frac {\alpha}{\sigma} \sqrt {\Delta t}\tag{2.18}
$$

we get 

$$
\begin{array}{r l r} {p} & {=} & {\frac {1}{2} [ 1 + \frac {\alpha}{\sigma} \sqrt {\Delta t} ]} \\ {q} & {=} & {\frac {1}{2} [ 1 - \frac {\alpha}{\sigma} \sqrt {\Delta t} ]} \end{array}\tag{2.19}
$$

Now, putting together equations (2.16-2.19) gives 

$$
\begin{array}{r c l} {E (X _ {n} - X _ {0})} & = & {\alpha t} \\ {V a r (X _ {n} - X _ {0})} & = & {t \sigma^ {2} (1 - \frac {\alpha^ {2}}{\sigma^ {2}} \Delta t)} \\ & = & {t \sigma^ {2} ; \Delta t \to 0 .} \end{array}\tag{2.20}
$$

Now, let’s imagine that $X ( t _ { n } ) - X ( t _ { 0 } ) = X _ { n } - X _ { 0 }$ is very small, so that $X _ { n } - X _ { 0 } \simeq d X$ and $t _ { n } - t _ { 0 } \simeq d t$ , so that equation (2.20) becomes 

$$
\begin{array}{r c l} {E (d X)} & = & {\alpha d t} \\ {V a r (d X)} & = & {\sigma^ {2} d t.} \end{array}\tag{2.21}
$$

which agrees with equations (2.7-2.8). Hence, in the limit as $\Delta t \to 0 .$ , we can interpret the random walk for X on the lattice (with these parameters) as the solution to the stochastic diferential equation (SDE) 

$$
\begin{array}{r c l} d X & = & \alpha d t + \sigma d Z \\ & & d Z = \phi \sqrt {d t}. \end{array}\tag{2.22}
$$

Consider the case where $\alpha = 0 , \sigma = 1$ , so that $d X = d Z = \simeq Z ( t _ { i } ) - Z ( t _ { i - 1 } ) = Z _ { i } - Z _ { i - 1 } = X _ { i } - X _ { i - 1 }$ Now we can write 

$$
\int_ {0} ^ {t} d Z = \lim _ {\Delta t \to 0} \sum_ {i} (Z _ {i + 1} - Z _ {i}) = (Z _ {n} - Z _ {0}).\tag{2.23}
$$

From equation (2.20) $( \alpha = 0 , \sigma = 1 )$ we have 

$$
\begin{array}{r l} {E (Z _ {n} - Z _ {0})} & {= 0} \\ {V a r (Z _ {n} - Z _ {0})} & {= t.} \end{array}\tag{2.24}
$$

Now, if n is large $( \Delta t  0 )$ , recall that the binomial distribution (2.12) tends to a normal distribution. From equation (2.24), we have that the mean of this distribution is zero, with variance t, so that 

$$
\begin{array}{r c l} (Z _ {n} - Z _ {0}) & \sim & N (0, t) \\ & = & \int_ {0} ^ {t} d Z. \end{array}
$$

(2.25) 

In other words, after a finite time $t , \int _ { 0 } ^ { t } d Z$ is normally distributed with mean zero and variance t (the limit of a binomial distribution is a normal distribution). 

Recall that have that $Z _ { i } - Z _ { i - 1 } = { \sqrt { \Delta t } }$ with probability p and $Z _ { i } - Z _ { i - 1 } = - \sqrt { \Delta t }$ with probability q. Note that $( Z _ { i } - Z _ { i - 1 } ) ^ { 2 } = \Delta t$ , with certainty, so that we can write 

$$
(Z _ {i} - Z _ {i - 1}) ^ {2} \simeq (d Z) ^ {2} = \Delta t.\tag{2.26}
$$

To summarize 

• We can interpret the SDE 

$$
\begin{array}{r c l} d X & = & \alpha d t + \sigma d Z \\ & & d Z = \phi \sqrt {d t}. \end{array}\tag{2.27}
$$

as the limit of a discrete random walk on a lattice as the timestep tends to zero. 

$V a r ( d Z ) = d t$ , otherwise, after any finite time, the $V a r ( X _ { n } - X _ { 0 } )$ is either zero or infinite. 

• We can integrate the term dZ to obtain 

$$
\begin{array}{r c l} \int_ {0} ^ {t} d Z & = & Z (t) - Z (0) \\ & \sim & N (0, t)  . \end{array}\tag{2.28}
$$

Going back to our lattice example, note that the total distance traveled over any finite interval of time becomes infinite, 

$$
E (| \Delta X |) = \Delta h\tag{2.29}
$$

so that the the total distance traveled in n steps is 

$$
\begin{array}{r c l} {n \Delta h} & = & {\frac {t}{\Delta t} \Delta h} \\ & = & {\frac {t \sigma}{\sqrt {\Delta t}}} \end{array}\tag{2.30}
$$

which goes to infinity as $\Delta t \to 0$ . Similarly, 

$$
{\frac {\Delta x}{\Delta t}} = {\pm \infty .}\tag{2.31}
$$

Consequently, Brownian motion is very jagged at every timescale. These paths are not diferentiable, i.e. $\textstyle { \frac { d x } { d t } }$ does not exist, so we cannot speak of 

$$
E (\frac {d x}{d t})\tag{2.32}
$$

but we can possibly define 

$$
\frac {E (d x)}{d t}.\tag{2.33}
$$

## 2.6 Geometric Brownian motion with drift

Of course, the actual path followed by stock is more complex than the simple situation described above. More realistically, we assume that the relative changes in stock prices (the returns) follow Brownian motion with drift. We suppose that in an infinitesimal time dt, the stock price S changes to $S + d S$ , where 

$$
\frac {d S}{S} = \mu d t + \sigma d Z\tag{2.34}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/95b244fb29280926aa2bd8e52de4d3fe3fb9bc1ac77adf62a564a6b71c34e5d3.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/dbe8284b8f53dd15a963fcf7eaa529c36836315062f1805b361ed0f45024eb7e.jpg)



Figure 2.3: Realizations of asset price following geometric Brownian motion. Left: low volatility case; right: high volatility case. Risk-free rate of return $r = . 0 5$


where $\mu$ is the drift rate, σ is the volatility, and dZ is the increment of a Wiener process, 

$$
{ d Z } { = } { \phi \sqrt { d t } }\tag{2.35}
$$

where $\phi \sim N ( 0 , 1 )$ . Equations (2.34) and (2.35) are called geometric Brownian motion with drift. So, superimposed on the upward (relative) drift is a (relative) random walk. The degree of randomness is given by the volatility σ. Figure 2.3 gives an illustration of ten realizations of this random process for two diferent values of the volatility. In this case, we assume that the drift rate $\mu$ equals the risk free rate. 

Note that 

$$
\begin{array}{r c l} E (d S) & = & E (\sigma S d Z + \mu S d t) \\ & = & \mu S d t \\ & & \text { since } E (d Z) = 0 \end{array}\tag{2.36}
$$

and that the variance of dS is 

$$
\begin{array}{r c l} {V a r [ d S ]} & = & {E (d S ^ {2}) - [ E (d S) ] ^ {2}} \\ & = & {E (\sigma^ {2} S ^ {2} d Z ^ {2})} \\ & = & {\sigma^ {2} S ^ {2} d t} \end{array}\tag{2.37}
$$

so that $\sigma$ is a measure of the degree of randomness of the stock price movement. 

Equation (2.34) is a stochastic diferential equation. The normal rules of calculus don’t apply, since for example 

$$
\begin{array}{r l r}\frac {d Z}{d t}&=&\phi \frac {1}{\sqrt {d t}}\\&&\rightarrow \infty \mathrm{as} d t \rightarrow 0.\end{array}
$$

The study of these sorts of equations uses results from stochastic calculus. However, for our purposes, we need only one result, which is Ito’s Lemma (see Derivatives: the theory and practice of financial engineering, by P. Wilmott). Suppose we have some function $G = G ( S , t )$ , where S follows the stochastic process equation (2.34), then, in small time increment dt, $G  G + d G$ , where 

$$
d G = \left(\mu S \frac {\partial G}{\partial S} + \frac {\sigma^ {2} S ^ {2}}{2} \frac {\partial^ {2} G}{\partial S ^ {2}} + \frac {\partial G}{\partial t}\right) d t + \sigma S \frac {\partial G}{\partial S} d Z\tag{2.38}
$$

An informal derivation of this result is given in the following section. 

## 2.6.1 Ito’s Lemma

We give an informal derivation of Ito’s lemma (2.38). Suppose we have a variable S which follows 

$$
d S = a (S, t) d t + b (S, t) d Z\tag{2.39}
$$

where dZ is the increment of a Weiner process. 

Now since 

$$
d Z ^ {2} = \phi^ {2} d t\tag{2.40}
$$

where φ is a random variable drawn from a normal distribution with mean zero and unit variance, we have that, if E is the expectation operator, then 

$$
E (\phi) = 0 \qquad E (\phi^ {2}) = 1\tag{2.41}
$$

so that the expected value of $d Z ^ { 2 }$ is 

$$
E (d Z ^ {2}) = d t\tag{2.42}
$$

Now, it can be shown (see Section 6) that in the limit as $d t \to 0$ , we have that $\phi ^ { 2 } d t$ becomes non-stochastic, so that with probability one 

$$
d Z ^ {2} \rightarrow d t \quad \mathrm{as} d t \rightarrow 0\tag{2.43}
$$

Now, suppose we have some function $G = G ( S , t )$ , then 

$$
d G = G _ {S} d S + G _ {t} d t + G _ {S S} \frac {d S ^ {2}}{2} + \dots\tag{2.44}
$$

Now (from (2.39) ) 

$$
\begin{array}{r c l} (d S) ^ {2} & = & (a d t + b d Z) ^ {2} \\ & = & a ^ {2} d t ^ {2} + a b d Z d t + b ^ {2} d Z ^ {2} \end{array}\tag{2.45}
$$

Since $d Z = O ( { \sqrt { d t } } )$ and $d Z ^ { 2 } \to d t$ , equation (2.45) becomes 

$$
(d S) ^ {2} = b ^ {2} d Z ^ {2} + O ((d t) ^ {3 / 2})\tag{2.46}
$$

or 

$$
(d S) ^ {2} \rightarrow b ^ {2} d t \text {as} d t \rightarrow 0\tag{2.47}
$$

Now, equations(2.39,2.44,2.47) give 

$$
\begin{array}{r c l} {d G} & = & {G _ {S} d S + G _ {t} d t + G _ {S S} \frac {d S ^ {2}}{2} + \dots} \\ & = & {G _ {S} (a d t + b d Z) + d t (G _ {t} + G _ {S S} \frac {b ^ {2}}{2})} \\ & = & {G _ {S} b d Z + (a G _ {S} + G _ {S S} \frac {b ^ {2}}{2} + G _ {t}) d t} \end{array}\tag{2.48}
$$

So, we have the result that if 

$$
d S = a (S, t) d t + b (S, t) d Z\tag{2.49}
$$

and if $G = G ( S , t )$ , then 

$$
d G = G _ {S} b d Z + (a G _ {S} + G _ {S S} \frac {b ^ {2}}{2} + G _ {t}) d t\tag{2.50}
$$

Equation (2.38) can be deduced by setting $a = \mu S$ and $b = \sigma S$ in equation (2.50). 

## 2.6.2 Some uses of Ito’s Lemma

Suppose we have 

$$
d S = \mu d t + \sigma d Z.\tag{2.51}
$$

If $\mu , \sigma = C o n s t .$ ., then this can be integrated (from $t = 0$ to $t = t )$ exactly to give 

$$
S (t) = S (0) + \mu t + \sigma (Z (t) - Z (0))\tag{2.52}
$$

and from equation (2.28) 

$$
Z (t) - Z (0) \sim N (0, t)\tag{2.53}
$$

Note that when we say that we solve a stochastic diferential equation exactly, this means that we have an expression for the distribution of $S ( T )$ 

Suppose instead we use the more usual geometric Brownian motion 

$$
d S = \mu S d t + \sigma S d Z\tag{2.54}
$$

Let $F ( S ) = \log S$ , and use Ito’s Lemma 

$$
\begin{array}{r c l} {d F} & = & {F _ {S} S \sigma d Z + (F _ {S} \mu S + F _ {S S} \frac {\sigma^ {2} S ^ {2}}{2} + F _ {t}) d t} \\ & = & {(\mu - \frac {\sigma^ {2}}{2}) d t + \sigma d Z ,} \end{array}\tag{2.55}
$$

so that we can integrate this to get 

$$
F (t) = F (0) + (\mu - \frac {\sigma^ {2}}{2}) t + \sigma (Z (t) - Z (0))\tag{2.56}
$$

or, since $S = e ^ { F }$ 2 

$$
S (t) = S (0) \exp [ (\mu - \frac {\sigma^ {2}}{2}) t + \sigma (Z (t) - Z (0)) ].\tag{2.57}
$$

Unfortunately, these cases are about the only situations where we can exactly integrate the SDE (constant $\sigma , \mu )$ 

## 2.6.3 Some more uses of Ito’s Lemma

We can often use Ito’s Lemma and some algebraic tricks to determine some properties of distributions. Let 

$$
d X = a (X, t) d t + b (X, t) d Z,\tag{2.58}
$$

then if $G = G ( X )$ , then 

$$
{ d G } { = } { \left[ a G _ { X } + G _ { t } + \frac { b ^ { 2 } } { 2 } G _ { X X } \right] d t + G _ { X } b d Z . }\tag{2.59}
$$

If $E [ X ] = { \bar { X } }$ , then $( b ( X , t )$ and $d Z$ are independent) 

$$
\begin{array}{r c l} E [ d X ] & = & d E [ S ] = d \bar {X} \\ & = & E [ a d t ] + E [ b ] E [ d Z ] \\ & = & E [ a d t ], \end{array}\tag{2.60}
$$

so that 

$$
\begin{array}{r c l} \frac {d \bar {X}}{d t} & = & E [ a ] = \bar {a} \\ \bar {X} = E \left[ \int_ {0} ^ {t} a d t \right]. \end{array}\tag{2.61}
$$

Let $\bar { G } = E [ ( X - \bar { X } ) ^ { 2 } ] = v a r ( X )$ , then 

$$
\begin{array}{r c l} d \bar {G} & = & E [ d G ] \\ & = & E [ 2 (X - \bar {X}) a - 2 (X - \bar {X}) \bar {a} + b ^ {2} ] d t + E [ 2 b (X - \bar {X}) ] E [ d Z ] \\ & = & E [ b ^ {2} d t ] + E [ 2 (X - \bar {X}) (a - \bar {a}) d t ], \end{array}\tag{2.62}
$$

which means that 

$$
\bar {G} = v a r (X) = E \left[ \int_ {0} ^ {t} b ^ {2} d t \right] + E \left[ \int_ {0} ^ {t} 2 (a - \bar {a}) (X - \bar {X}) d t \right].\tag{2.63}
$$

In a particular case, we can sometimes get more useful expressions. If 

$$
{ d S } { = } { \mu S ~ d t + \sigma S ~ d Z }\tag{2.64}
$$

with $\mu , \sigma$ constant, then 

$$
\begin{array}{r c l} E [ d S ] & = & d \bar {S} = E [ \mu S ] d t \\ & = & \mu \bar {S} d t, \end{array}\tag{2.65}
$$

so that 

$$
\begin{array}{r c l} {d \bar {S}} & = & {\mu \bar {S} d t} \\ {\bar {S}} & = & {S _ {0} e ^ {\mu t}.} \end{array}\tag{2.66}
$$

Now, let $G ( S ) = S ^ { 2 }$ , so that $E [ G ] = { \bar { G } } = E [ S ^ { 2 } ]$ , then (from Ito’s Lemma) 

$$
\begin{array}{r c l} {d \bar {G}} & = & {E [ 2 \mu S ^ {2} + \sigma^ {2} S ^ {2} ] d t + E [ 2 S ^ {2} \sigma ] E [ d Z ]} \\ & = & {E [ 2 \mu S ^ {2} + \sigma^ {2} S ^ {2} ] d t} \\ & = & {(2 \mu + \sigma^ {2}) \bar {G} d t,} \end{array}\tag{2.67}
$$

so that 

$$
\begin{array}{r c l} \bar {G} & = & \bar {G} _ {0} e ^ {(2 \mu + \sigma^ {2}) t} \\ & & E [ S ^ {2} ] = S _ {0} ^ {2} e ^ {(2 \mu + \sigma^ {2}) t}. \end{array}\tag{2.68}
$$

From equations (2.66) and (2.68) we then have 

$$
\begin{array}{r c l} v a r (S) & = & E [ S ^ {2} ] - (E [ S ]) ^ {2} \\ & = & E [ S ^ {2} ] - \bar {S} ^ {2} \\ & = & S _ {0} ^ {2} e ^ {2 \mu t} (e ^ {\sigma^ {2} t} - 1) \\ & = & \bar {S} ^ {2} (e ^ {\sigma^ {2} t} - 1). \end{array}\tag{2.69}
$$

One can use the same ideas to compute the skewness, $E [ ( S - { \bar { S } } ) ^ { 3 } ]$ . If $G ( S ) = S ^ { 3 }$ and $\bar { G } = E [ G ( S ) ] = E [ S ^ { 3 } ]$ ， then 

$$
\begin{array}{r c l} {d \bar {G}} & = & {E [ \mu S \cdot 3 S ^ {2} + \sigma^ {2} S ^ {2} / 2 \cdot 3 \cdot 2 S ] d t + E [ 3 S ^ {2} \sigma S ] E [ d Z ]} \\ & = & {E [ 3 \mu S ^ {3} + 3 \sigma^ {2} S ^ {3} ]} \\ & = & {3 (\mu + \sigma^ {2}) \bar {G},} \end{array}\tag{2.70}
$$

so that 

$$
\begin{array}{r c l} \bar {G} & = & E [ S ^ {3} ] \\ & = & S _ {0} ^ {3} e ^ {3 (\mu + \sigma^ {2}) t}. \end{array}\tag{2.71}
$$

We can then obtain the skewness from 

$$
\begin{array}{r c l} {E [ (S - \bar {S}) ^ {3} ]} & = & {E [ S ^ {3} - 2 S ^ {2} \bar {S} - 2 S \bar {S} ^ {2} + \bar {S} ^ {3} ]} \\ & = & {E [ S ^ {3} ] - 2 \bar {S} E [ S ^ {2} ] - \bar {S} ^ {3}.} \end{array}\tag{2.72}
$$

Equations (2.66, 2.68, 2.71) can then be substituted into equation (2.72) to get the desired result. 

## 2.7 The Black-Scholes Analysis

Assume 

• The stock price follows geometric Brownian motion, equation (2.34). 

• The risk-free rate of return is a constant r. 

• There are no arbitrage opportunities, i.e. all risk-free portfolios must earn the risk-free rate of return. 

• Short selling is permitted (i.e. we can own negative quantities of an asset). 

Suppose that we have an option whose value is given by $V = V ( S , t )$ . Construct an imaginary portfolio, consisting of one option, and a number of $( - ( \alpha ^ { h } ) )$ of the underlying asset. (If $( \alpha ^ { h } ) > 0$ , then we have sold the asset short, i.e. we have borrowed an asset, sold it, and are obligated to give it back at some future date). 

The value of this portfolio $P$ is 

$$
P = V - (\alpha^ {h}) S\tag{2.73}
$$

In a small time dt, $P  P + d P ,$ 

$$
d P = d V - (\alpha^ {h}) d S\tag{2.74}
$$

Note that in equation (2.74) we not included a term $( \alpha ^ { h } ) _ { S } S$ . This is actually a rather subtle point, since we shall see (later on) that $( \alpha ^ { h } )$ actually depends on S. However, if we think of a real situation, at any instant in time, we must choose $( \alpha ^ { h } )$ , and then we hold the portfolio while the asset moves randomly. So, equation (2.74) is actually the change in the value of the portfolio, not a diferential. If we were taking a true diferential then equation (2.74) would be 

$$
d P = d V - (\alpha^ {h}) d S - S d (\alpha^ {h})
$$

but we have to remember that $( \alpha ^ { h } )$ does not change over a small time interval, since we pick $( \alpha ^ { h } )$ , and then S changes randomly. We are not allowed to peek into the future, (otherwise, we could get rich without risk, which is not permitted by the no-arbitrage condition) and hence $( \alpha ^ { h } )$ is not allowed to contain any information about future asset price movements. The principle of no peeking into the future is why Ito stochastic calculus is used. Other forms of stochastic calculus are used in Physics applications (i.e. turbulent flow). 

Substituting equations (2.34) and (2.38) into equation (2.74) gives 

$$
d P = \sigma S \left(V _ {S} - (\alpha^ {h})\right) d Z + \left(\mu S V _ {S} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + V _ {t} - \mu (\alpha^ {h}) S\right) d t\tag{2.75}
$$

We can make this portfolio riskless over the time interval $d t ,$ , by choosing $( \alpha ^ { h } ) = V _ { S }$ in equation (2.75). This eliminates the dZ term in equation (2.75). (This is the analogue of our choice of the amount of stock in the riskless portfolio for the two state tree model.) So, letting 

$$
(\alpha^ {h}) = V _ {S}\tag{2.76}
$$

then substituting equation (2.76) into equation (2.75) gives 

$$
d P = \left(V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S}\right) d t\tag{2.77}
$$

Since $P$ is now risk-free in the interval $t  t + d t$ , then no-arbitrage says that 

$$
d P = r P d t\tag{2.78}
$$

Therefore, equations (2.77) and (2.78) give 

$$
r P d t = \left(V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S}\right) d t\tag{2.79}
$$

Since 

$$
P = V - (\alpha^ {h}) S = V - V _ {S} S\tag{2.80}
$$

then substituting equation (2.80) into equation (2.79) gives 

$$
V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + r S V _ {S} - r V = 0\tag{2.81}
$$

which is the Black-Scholes equation. Note the rather remarkable fact that equation (2.81) is independent of the drift rate µ. 

Equation (2.81) is solved backwards in time from the option expiry time $t = T$ to the present $t = 0$ 

## 2.8 Hedging in Continuous Time

We can construct a hedging strategy based on the solution to the above equation. Suppose we sell an option at price V at $t = 0$ . Then we carry out the following 

• We sell one option worth V . (This gives us V in cash initially). 

• We borrow $( S { \frac { \partial V } { \partial S } } - V )$ from the bank. 

• We buy $\frac { \partial V } { \partial S }$ shares at price S. 

At every instant in time, we adjust the amount of stock we own so that we always have $\frac { \partial V } { \partial S }$ shares. Note that this is a dynamic hedge, since we have to continually rebalance the portfolio. Cash will flow into and out of the bank account, in response to changes in S. If the amount in the bank is positive, we receive the risk free rate of return. If negative, then we borrow at the risk free rate. 

So, our hedging portfolio will be 

• Short one option worth V. 

• Long $\frac { \partial V } { \partial S }$ shares at price S. 

$V - S { \frac { \partial V } { \partial S } }$ cash in the bank account. 

At any instant in time (including the terminal time), this portfolio can be liquidated and any obligations implied by the short position in the option can be covered, at zero gain or loss, regardless of the value of S. Note that given the receipt of the cash for the option, this strategy is self-financing. 

## 2.9 The option price

So, we can see that the price of the option valued by the Black-Scholes equation is the market price of the option at any time. If the price was higher then the Black-Scholes price, we could construct the hedging portfolio, dynamically adjust the hedge, and end up with a positive amount at the end. Similarly, if the price was lower than the Black-Scholes price, we could short the hedging portfolio, and end up with a positive gain. By the no-arbitrage condition, this should not be possible. 

Note that we are not trying to predict the price movements of the underlying asset, which is a random process. The value of the option is based on a hedging strategy which is dynamic, and must be continuously rebalanced. The price is the cost of setting up the hedging portfolio. The Black-Scholes price is not the expected payof. 

The price given by the Black-Scholes price is not the value of the option to a speculator, who buys and holds the option. A speculator is making bets about the underlying drift rate of the stock (note that the drift rate does not appear in the Black-Scholes equation). For a speculator, the value of the option is given by an equation similar to the Black-Scholes equation, except that the drift rate appears. In this case, the price can be interpreted as the expected payof based on the guess for the drift rate. But this is art, not science! 

## 2.10 American early exercise

Actually, most options traded are American options, which have the feature that they can be exercised at any time. Consequently, an investor acting optimally, will always exercise the option if the value falls below the payof or exercise value. ${ \mathrm { S o } } ,$ the value of an American option is given by the solution to equation (2.81) with the additional constraint 

$$
V (S, t) \geq \left\{ \begin{array}{l l} \max (S - K, 0) & \text { for   a   call } \\ \max (K - S, 0) & \text { for   a   put } \end{array} \right.\tag{2.82}
$$

Note that since we are working backwards in time, we know what the option is worth in future, and therefore we can determine the optimal course of action. 

In order to write equation (2.81) in more conventional form, define $\tau = T - t ,$ , so that equation (2.81) becomes 

$$
\begin{array}{r c l} V _ {\tau} & = & \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + r S V _ {S} - r V \\ V (S, \tau = 0) & = & \left\{ \begin{array}{l l} \max (S - K, 0) & \text {for a call} \\ \max (K - S, 0) & \text {for a put} \end{array} \right. \\ V (0, \tau) & \to & V _ {\tau} = - r V \\ V (S = \infty , \tau) & \to & \left\{ \begin{array}{l l} \simeq S & \text {for a call} \\ \simeq 0 & \text {for a put} \end{array} \right. \end{array}\tag{2.83}
$$

If the option is American, then we also have the additional constraints 

$$
V (S, \tau) \geq \left\{ \begin{array}{l l} \max (S - K, 0) & \text { for   a   call } \\ \max (K - S, 0) & \text { for   a   put } \end{array} \right.\tag{2.84}
$$

Define the operator 

$$
L V \equiv V _ {\tau} - (\frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + r S V _ {S} - r V)\tag{2.85}
$$

and let $V ( S , 0 ) = V ^ { * }$ . More formally, the American option pricing problem can be stated as 

$$
\begin{array}{r c l} L V & \geq & 0 \\ V - V ^ {*} & \geq & 0 \\ (V - V ^ {*}) L V & = & 0 \end{array}\tag{2.86}
$$

## 3 The Risk Neutral World

Suppose instead of valuing an option using the above no-arbitrage argument, we wanted to know the expected value of the option. We can imagine that we are buying and holding the option, and not hedging. If we are considering the value of risky cash flows in the future, then these cash flows should be discounted at an appropriate discount rate, which we will call $\rho \ { \mathrm { ( i . e . } }$ . the riskier the cash flows, the higher $\rho )$ 

Consequently the value of an option today can be considered to the be the discounted future value. This is simply the old idea of net present value. Regard S today as known, and let $V ( S + d S , t + d t )$ be the value of the option at some future time $t + d t$ , which is uncertain, since $S$ evolves randomly. Thus 

$$
{ V ( S , t ) } { = } { \frac { 1 } { 1 + \rho d t } E ( V ( S + d S , t + d t ) ) }\tag{3.1}
$$

where $E ( . . . )$ is the expectation operator, i.e. the expected value of $V ( S + d S , t + d t )$ given that $V = V ( S , t )$ at $t = t .$ . We can rewrite equation (3.1) as (ignoring terms of $o ( d t )$ , where $o ( d t )$ represents terms that go to zero faster than dt ) 

$$
\rho d t V (S, t) = E (V (S, t) + d V) - V (S, t).\tag{3.2}
$$

Since we regard V as the expected value, so that $E [ V ( S , t ) ] = V ( S , t )$ , and then 

$$
E (V (S, t) + d V) - V (S, t) = E (d V),\tag{3.3}
$$

so that equation (3.2) becomes 

$$
\rho d t V (S, t) = E (d V).\tag{3.4}
$$

Assume that 

$$
\frac {d S}{S} = \mu d t + \sigma d Z.\tag{3.5}
$$

From Ito’s Lemma (2.38) we have that 

$$
{ d V } { = } { \left( V _ { t } + \frac { \sigma ^ { 2 } S ^ { 2 } } { 2 } V _ { S S } + \mu S V _ { S } \right) d t + \sigma S V _ { S } d Z . }\tag{3.6}
$$

Noting that 

$$
E (d Z) = 0\tag{3.7}
$$

then 

$$
E (d V) = \left(V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + \mu S V _ {S}\right) d t.\tag{3.8}
$$

Combining equations (3.4-3.8) gives 

$$
V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + \mu S V _ {S} - \rho V = 0.\tag{3.9}
$$

Equation (3.9) is the PDE for the expected value of an option. If we are not hedging, maybe this is the value that we are interested in, not the no-arbitrage value. However, if this is the case, we have to estimate the drift rate $\mu ,$ and the discount rate $\rho .$ Estimating the appropriate discount rate is always a thorny issue. 

Now, note the interesting fact, if we set $\rho = r$ and $\mu = r$ in equation (3.9) then we simply get the Black-Scholes equation (2.81). 

This means that the no-arbitrage price of an option is identical to the expected value if $\rho = r$ and $\mu = r .$ In other words, we can determine the no-arbitrage price by pretending we are living in a world where all assets drift at rate $r ,$ and all investments are discounted at rate r. This is the so-called risk neutral world. 

This result is the source of endless confusion. It is best to think of this as simply a mathematical fluke. This does not have any reality. Investors would be very stupid to think that the drift rate of risky investments is r. I’d rather just buy risk-free bonds in this case. There is in reality no such thing as a risk-neutral world. Nevertheless, this result is useful for determining the no-arbitrage value of an option using a Monte Carlo approach. Using this numerical method, we simply assume that 

$$
d S = r S d t + \sigma S d Z\tag{3.10}
$$

and simulate a large number of random paths. If we know the option payof as a function of $S$ at $t = T$ ， then we compute 

$$
V (S, 0) = e ^ {- r T} E _ {Q} (V (S, T))\tag{3.11}
$$

which should be the no-arbitrage value. 

Note the $E _ { Q }$ in the above equation. This makes it clear that we are taking the expectation in the risk neutral world (the expectation in the Q measure). This contrasts with the real-world expectation (the P measure). 

Suppose we want to know the expected value (in the real world) of an asset which pays $V ( S , t = T )$ at $t = T$ in the future. Then, the expected value (today) is given by solving 

$$
V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + \mu S V _ {S} = 0.\tag{3.12}
$$

where we have dropped the discounting term. In particular, suppose we are going to receive $V = S ( t = T )$ i.e. just the asset at $t = T$ . Assume that the solution to equation (3.12) is $V = C o n s t . ~ A ( t ) S$ , and we find that 

$$
V = C o n s t. S e ^ {\mu (T - t)}.\tag{3.13}
$$

Noting that we receive $V = S$ at $t = T$ means that 

$$
V = S e ^ {\mu (T - t)}.\tag{3.14}
$$

Today, we can acquire the asset for price $S ( t = 0 )$ . At $t = T$ , the asset is worth $S ( t = T )$ . Equation (3.14) then says that 

$$
{E [ V (S (t = 0), t = 0) ]} = {E [ S (t = 0) ] = S (t = 0) e ^ {\mu (T)}}\tag{3.15}
$$

In other words, if 

$$
d S = S \mu d t + S \sigma d Z\tag{3.16}
$$

then (setting t = T) 

$$
E [ S ] = S e ^ {\mu t}.\tag{3.17}
$$

Recall that the exact solution to equation (3.16) is (equation (2.57)) 

$$
S (t) = S (0) \exp [ (\mu - \frac {\sigma^ {2}}{2}) t + \sigma (Z (t) - Z (0)) ].\tag{3.18}
$$

So that we have just shown that $E [ S ] = S e ^ { \mu t }$ by using a simple PDE argument and Ito’s Lemma. Isn’t this easier than using brute force statistics? PDEs are much more elegant. 

## 4 Monte Carlo Methods

This brings us to the simplest numerical method for computing the no-arbitrage value of an option. Suppose that we assume that the underlying process is 

$$
\frac {d S}{S} = r d t + \sigma d Z\tag{4.1}
$$

then we can simulate a path forward in time, starting at some price today $S ^ { 0 }$ , using a forward Euler timestepping method $( S ^ { i } = S ( t _ { i } ) )$ 

$$
{S ^ {i + 1}} = {S ^ {i} + S ^ {i} (r \Delta t + \sigma \phi^ {i} \sqrt {\Delta t})}\tag{4.2}
$$

where $\Delta t$ is the finite timestep, and $\phi ^ { i }$ is a random number which is $N ( 0 , 1 )$ . Note that at each timestep, we generate a new random number. After N steps, with $T = N \Delta t$ , we have a single realized path. Given the payof function of the option, the value for this path would be 

$$
{ V a l u e } { = } { P a y o f f ( S ^ { N } ) . }\tag{4.3}
$$

For example, if the option was a European call, then 

$$
\begin{array}{r l r} {V a l u e} & = & {\max (S ^ {N} - K, 0)} \\ & & {K = \mathrm{StrikePrice}} \end{array}\tag{4.4}
$$

Suppose we run a series of trials, $m = 1 , . . . , M .$ , and denote the payof after the m<sup>0</sup>th trial as payoff(m). Then, the no-arbitrage value of the option is 

$$
\begin{array}{r c l} O p t i o n V a l u e & = & e ^ {- r T} E (p a y o f f) \\ & \simeq & e ^ {- r T} \frac {1}{M} \sum_ {m = 1} ^ {m = M} p a y o f f (m) . \end{array}\tag{4.5}
$$

Recall that these paths are not the real paths, but are the risk neutral paths. 

Now, we should remember that we are 

1. approximating the solution to the SDE by forward Euler, which has $O ( \Delta t )$ truncation error. 

2. approximating the expectation by the mean of many random paths. This Monte Carlo error is of size $O ( 1 / \sqrt { M } )$ , which is slowly converging. 

There are thus two sources of error in the Monte Carlo approach: timestepping error and sampling error. 

The slow rate of convergence of Monte Carlo methods makes these techniques unattractive except when the option is written on several (i.e. more than three) underlying assets. As well, since we are simulating forward in time, we cannot know at a given point in the forward path if it is optimal to exercise or hold an American style option. This is easy if we use a PDE method, since we solve the PDE backwards in time, so we always know the continuation value and hence can act optimally. However, if we have more than three factors, PDE methods become very expensive computationally. As well, if we want to determine the efects of discrete hedging, for example, a Monte Carlo approach is very easy to implement. 

The error in the Monte Carlo method is then 

$$
\begin{array}{r c l} {E r r o r} & = & {O \left(\max (\Delta t, \frac {1}{\sqrt {M}})\right)} \\ & & {\Delta t = \mathrm{timestep}} \\ & & {M = \mathrm{numberofMonteCarlopaths}} \end{array}\tag{4.6}
$$

Now, it doesn’t make sense to drive the Monte Carlo error down to zero if there is $O ( \Delta t )$ timestepping error. We should seek to balance the timestepping error and the sampling error. In order to make these two errors the same order, we should choose $\begin{array} { r } { M = O ( \frac { 1 } { ( \Delta t ) ^ { 2 } } ) } \end{array}$ . This makes the total error $O ( \Delta t )$ . We also have that 

$$
\begin{array}{r c l} \text {Complexity} & = & O \left(\frac {M}{\Delta t}\right) \\ & = & O \left(\frac {1}{(\Delta t) ^ {3}}\right) \\ \Delta t & = & O \left((\text {Complexity}) ^ {- 1 / 3}\right) \end{array}\tag{4.7}
$$

and hence 

$$
\text {   Error   } = O \left(\frac {1}{(\text {   Complexity }) ^ {1 / 3}}\right) .\tag{4.8}
$$

In practice, the convergence in terms of timestep error is often not done. People just pick a timestep, i.e. one day, and increase the number of Monte Carlo samples until they achieve convergence in terms of sampling error, and ignore the timestep error. Sometimes this gives bad results! 

Note that the exact solution to Geometric Brownian motion (2.57) has the property that the asset value S can never reach $S = 0 \mathrm { ~ i f ~ } S ( 0 ) > 0$ , in any finite time. However, due to the approximate nature of our Forward Euler method for solving the SDE, it is possible that a negative or zero $S ^ { i }$ can show up. We can do one of three things here, in this case 

• Cut back the timestep at this point in the simulation so that S is positive. 

• Set $S = 0$ and continue. In this case, S remains zero for the rest of this particular simulation. 

• Use Ito’s Lemma, and determine the SDE for log S, i.e. if $F = \log S$ , then, from equation (2.55), we obtain (with $\mu = r )$ 

$$
{ d F } { = } { ( r - \frac { \sigma ^ { 2 } } { 2 } ) d t + \sigma d Z , }\tag{4.9}
$$

so that now, if $F < 0$ , there is no problem, since $S = e ^ { F }$ , and if $F < 0$ , this just means that $S$ is very small. We can use this idea for any stochastic process where the variable should not go negative. 

Usually, most people set $S = 0$ and continue. As long as the timestep is not too large, this situation is probably due to an event of low probability, hence any errors incurred will not afect the expected value very much. If negative S values show up many times, this is a signal that the timestep is too large. 

In the case of simple Geometric Brownian motion, where $r , \sigma$ are constants, then the SDE can be solved exactly, and we can avoid timestepping errors (see Section 2.6.2). In this case 

$$
S (T) = S (0) \exp [ (r - \frac {\sigma^ {2}}{2}) T + \sigma \phi \sqrt {T} ]\tag{4.10}
$$

where $\phi \sim N ( 0 , 1 )$ . I’ll remind you that equation (4.10) is exact. For these simple cases, we should always use equation (4.10). Unfortunately, this does not work in more realistic situations. 

Monte Carlo is popular because 

• It is simple to code. Easily handles complex path dependence. 

• Easily handles multiple assets. 

The disadvantages of Monte Carlo methods are 

• It is dificult to apply this idea to problems involving optimal decision making (e.g. American options). 

• It is hard to compute the Greeks $( V _ { S } , V _ { S S } )$ , which are the hedging parameters, very accurately. 

• MC converges slowly. 

## 4.1 Monte Carlo Error Estimators

The sampling error can be estimated via a statistical approach. If the estimated mean of the sample is 

$$
\hat {\mu} = \frac {e ^ {- r T}}{M} \sum_ {m = 1} ^ {m = M} p a y o f f (m)\tag{4.11}
$$

and the standard deviation of the estimate is 

$$
\omega = \left(\frac {1}{M - 1} \sum_ {m = 1} ^ {m = M} (e ^ {- r T} p a y o f f (m) - \hat {\mu}) ^ {2}\right) ^ {1 / 2}\tag{4.12}
$$

then the 95% confidence interval for the actual value V of the option is 

$$
\hat {\mu} - \frac {1 . 9 6 \omega}{\sqrt {M}} <   V <   \hat {\mu} + \frac {1 . 9 6 \omega}{\sqrt {M}}\tag{4.13}
$$

Note that in order to reduce this error by a factor of 10, the number of simulations must be increased by 100. 

The timestep error can be estimated by running the problem with diferent size timesteps, comparing the solutions. 

## 4.2 Random Numbers and Monte Carlo

There are many good algorithms for generating random sequences which are uniformly distributed in [0, 1]. See for example, (Numerical Recipies in C++., Press et al, Cambridge University Press, 2002). As pointed out in this book, often the system supplied random number generators, such as rand in the standard C library, and the infamous RANDU IBM function, are extremely bad. The Matlab functions appear to be quite good. For more details, please look at (Park and Miller, ACM Transactions on Mathematical Software, 31 (1988) 1192-1201). Another good generator is described in (Matsumoto and Nishimura, “The Mersenne Twister: a 623 dimensionally equidistributed uniform pseudorandom number generator,” ACM Transactions on Modelling and Computer Simulation, 8 (1998) 3-30.) Code can be downloaded from the authors Web site. 

However, we need random numbers which are normally distributed on $[ - \infty , + \infty ]$ , with mean zero and variance one (N(0, 1)). 

Suppose we have uniformly distributed numbers on $[ 0 , 1 ]$ , i.e. the probability of obtaining a number between x and $x + d x$ is 

$$
\begin{array}{r c l} p (x) d x & = & d x ; 0 \leq x \leq 1 \\ & = & 0 ; \text { otherwise } \end{array}\tag{4.14}
$$

Let’s take a function of this random variable $y ( x )$ . How is $y ( x )$ distributed? Let $\hat { p } ( y )$ be the probability distribution of obtaining $y$ in $[ y , y + d y ]$ . Consequently, we must have (recall the law of transformation of probabilities) 

$$
{ p ( x ) | d x | } = { \hat { p } ( y ) | d y | }
$$

or 

$$
\hat {p} (y) = p (x) \left| \frac {d x}{d y} \right|.\tag{4.15}
$$

Suppose we want $\hat { p } ( y )$ to be normal, 

$$
\hat {p} (y) = \frac {e ^ {- y ^ {2} / 2}}{\sqrt {2 \pi}}.\tag{4.16}
$$

If we start with a uniform distribution, $p ( x ) = 1$ on $[ 0 , 1 ]$ , then from equations (4.15-4.16) we obtain 

$$
{\frac {d x}{d y}} = {\frac {e ^ {- y ^ {2} / 2}}{\sqrt {2 \pi}}}.\tag{4.17}
$$

Now, for $x \in [ 0 , 1 ]$ , we have that the probability of obtaining a number in $[ 0 , x ]$ is 

$$
\int_ {0} ^ {x} d x ^ {\prime} = x,\tag{4.18}
$$

but from equation (4.17) we have 

$$
d x ^ {\prime} = \frac {e ^ {- (y ^ {\prime}) ^ {2} / 2}}{\sqrt {2 \pi}} d y ^ {\prime}.\tag{4.19}
$$

$\mathrm { S o } .$ there exists a $y$ such that the probability of getting a $y ^ { \prime }$ in $[ - \infty , y ]$ is equal to the probability of getting $x ^ { \prime }$ in $[ 0 , x ]$ 2 

$$
\int_ {0} ^ {x} d x ^ {\prime} = \int_ {- \infty} ^ {y} \frac {e ^ {- (y ^ {\prime}) ^ {2} / 2}}{\sqrt {2 \pi}} d y ^ {\prime},\tag{4.20}
$$

or 

$$
{ x } { = } { \int _ { - \infty } ^ { y } \frac { e ^ { - ( y ^ { \prime } ) ^ { 2 } / 2 } } { \sqrt { 2 \pi } } d y ^ { \prime } ~ . }\tag{4.21}
$$

${ \mathrm { S o } } ,$ if we generate uniformly distributed numbers x on [0, 1], then to determine y which are $N ( 0 , 1 )$ , we do the following 

• Generate x 

• Find y such that 

$$
x = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {y} e ^ {- (y ^ {\prime}) ^ {2} / 2} d y ^ {\prime}.\tag{4.22}
$$

We can write this last step as 

$$
y = F (x)\tag{4.23}
$$

where $F ( x )$ is the inverse cumulative normal distribution. 

## 4.3 The Box-Muller Algorithm

Starting from random numbers which are uniformly distributed on $[ 0 , 1 ]$ , there is actually a simpler method for obtaining random numbers which are normally distributed. 

If $p ( x )$ is the probability of finding $x \in [ x , x + d x ]$ and if $y = y ( x )$ , and $\hat { p } ( y )$ is the probability of finding $y \in [ y , y + d y ]$ ], then, from equation (4.15) we have 

$$
{| p (x) d x |} = {| \hat {p} (y) d y |}\tag{4.24}
$$

or 

$$
\hat {p} (y) = p (x) \left| \frac {d x}{d y} \right|.\tag{4.25}
$$

Now, suppose we have two original random variables $x _ { 1 } , x _ { 2 }$ , and let $p ( x _ { i } , x _ { 2 } )$ be the probability of obtaining $( x _ { 1 } , x _ { 2 } )$ in $[ x _ { 1 } , x _ { 1 } + d x _ { 1 } ] \times [ x _ { 2 } , x _ { 2 } + d x _ { 2 } ]$ . Then, if 

$$
\begin{array}{r c l} {y _ {1}} & = & {y _ {1} (x _ {1}, x _ {2})} \\ {y _ {2}} & = & {y _ {2} (x _ {1}, x _ {2})} \end{array}\tag{4.26}
$$

and we have that 

$$
\hat {p} (y _ {1}, y _ {2}) = p (x _ {1}, x _ {2}) \left| \frac {\partial (x _ {1} , x _ {2})}{\partial (y _ {1} , y _ {2})} \right|\tag{4.27}
$$

where the Jacobian of the transformation is defined as 

$$
\frac {\partial (x _ {1} , x _ {2})}{\partial (y _ {1} , y _ {2})} = d e t \left| \begin{array}{c c} \frac {\partial x _ {1}}{\partial y _ {1}} & \frac {\partial x _ {1}}{\partial y _ {2}} \\ \frac {\partial x _ {2}}{\partial y _ {1}} & \frac {\partial x _ {2}}{\partial y _ {2}} \end{array} \right|\tag{4.28}
$$

Recall that the Jacobian of the transformation can be regarded as the scaling factor which transforms $d x _ { 1 } \ d x _ { 2 }$ to $d y _ { 1 } \ d y _ { 2 }$ , i.e. 

$$
d x _ {1} d x _ {2} = \left| \frac {\partial (x _ {1} , x _ {2})}{\partial (y _ {1} , y _ {2})} \right| d y _ {1} d y _ {2}.\tag{4.29}
$$

Now, suppose that we have $x _ { 1 } , x _ { 2 }$ uniformly distributed on $[ 0 , 1 ] \times [ 0 , 1 ]$ , i.e. 

$$
p (x _ {1}, x _ {2}) = U (x _ {1}) U (x _ {2})\tag{4.30}
$$

where 

$$
\begin{array}{r c l} U (x) & = & 1 \quad ; \quad 0 \leq x \leq 1 \\ & = & 0 \quad ; \quad \text { otherwise }  . \end{array}\tag{4.31}
$$

We denote this distribution as $x _ { 1 } \sim U [ 0 , 1 ]$ and $x _ { 2 } \sim U [ 0 , 1 ]$ 

If $p ( x _ { 1 } , x _ { 2 } )$ is given by equation (4.30), then we have from equation (4.27) that 

$$
\hat {p} (y _ {1}, y _ {2}) = \left| \frac {\partial (x _ {1} , x _ {2})}{\partial (y _ {1} , y _ {2})} \right|\tag{4.32}
$$

Now, we want to find a transformation $y _ { 1 } = y _ { 1 } ( x _ { 1 } , x _ { 2 } ) , y _ { 2 } = y _ { 2 } ( x _ { 1 } , x _ { 2 } )$ which results in normal distributions for $y _ { 1 } , y _ { 2 }$ . Consider 

$$
\begin{array}{r l r} {y _ {1}} & = & {\sqrt {- 2 \log x _ {1}} \cos 2 \pi x _ {2}} \\ {y _ {2}} & = & {\sqrt {- 2 \log x _ {1}} \sin 2 \pi x _ {2}} \end{array}\tag{4.33}
$$

or solving for $( x _ { 2 } , x _ { 2 } )$ 

$$
\begin{array}{r c l} x _ {1} & = & \exp \left(\frac {- 1}{2} (y _ {1} ^ {2} + y _ {2} ^ {2})\right) \\ x _ {2} & = & \frac {1}{2 \pi} \tan^ {- 1} \left[ \frac {y _ {2}}{y _ {1}} \right] . \end{array}\tag{4.34}
$$

After some tedious algebra, we can see that (using equation (4.34)) 

$$
{\left| \frac {\partial (x _ {1} , x _ {2})}{\partial (y _ {1} , y _ {2})} \right|} = {\frac {1}{\sqrt {2 \pi}} e ^ {- y _ {1} ^ {2} / 2} \frac {1}{\sqrt {2 \pi}} e ^ {- y _ {2} ^ {2} / 2}}\tag{4.35}
$$

Now, assuming that equation (4.30) holds, then from equations (4.32-4.35) we have 

$$
\hat {p} (y _ {1}, y _ {2}) = \frac {1}{\sqrt {2 \pi}} e ^ {- y _ {1} ^ {2} / 2} \frac {1}{\sqrt {2 \pi}} e ^ {- y _ {2} ^ {2} / 2}\tag{4.36}
$$

so that $( y _ { 1 } , y _ { 2 } )$ are independent, normally distributed random variables, with mean zero and variance one, or 

$$
y _ {1} \sim N (0, 1) \quad ; \quad y _ {2} \sim N (0, 1).\tag{4.37}
$$

This gives the following algorithm for generating normally distributed random numbers (given uniformly distributed numbers): 

## Box Muller Algorithm

Repeat
    Generate $u_{1} \sim U(0,1)$ , $u_{2} \sim U(0,1)$ $\theta = 2\pi u_{2}, \rho = \sqrt{-2 \log u_{1}}$ $z_{1} = \rho \cos \theta; z_{2} = \rho \sin \theta$ End Repeat 

(4.38) 

This has the efect that $Z _ { 1 } \sim N ( 0 , 1 )$ and $Z _ { 2 } \sim N ( 0 , 1 )$ 

Note that we generate two draws from a normal distribution on each pass through the loop. 

## 4.3.1 An improved Box Muller

The algorithm (4.38) can be expensive due to the trigonometric function evaluations. We can use the following method to avoid these evaluations. Let 

$$
\begin{array}{r l} {U _ {1} \sim U [ 0, 1 ]} & {; U _ {2} \sim U [ 0, 1 ]} \\ {V _ {1} = 2 U _ {1} - 1} & {; V _ {2} = 2 U _ {2} - 1} \end{array}\tag{4.39}
$$

which means that $( V _ { 1 } , V _ { 2 } )$ are uniformly distributed in $[ - 1 , 1 ] \times [ - 1 , 1 ]$ . Now, we carry out the following procedure 

## Rejection Method

Repeat
    If $(V_{1}^{2} + V_{2}^{2} < 1)$ Accept
    Else
    Reject
    Endif
End Repeat 

(4.40) 

which means that if we define $( V _ { 1 } , V _ { 2 } )$ as in equation (4.39), and then process the pairs $( V _ { 1 } , V _ { 2 } )$ using algorithm (4.40) we have that $( V _ { 1 } , V _ { 2 } )$ are uniformly distributed on the disk centered at the origin, with radius one, in the $( V _ { 1 } , V _ { 2 } )$ plane. This is denoted by 

$$
(V _ {1}, V _ {2}) \sim D (0, 1) .\tag{4.41}
$$

If $( V _ { 1 } , V _ { 2 } ) \sim D ( 0 , 1 )$ and $R ^ { 2 } = V _ { 1 } ^ { 2 } + V _ { 2 } ^ { 2 }$ , then the probability of finding R in $[ R , R + d R ]$ is 

$$
\begin{array}{r c l} {p (R) d R} & = & {\frac {2 \pi R d R}{\pi (1) ^ {2}}} \\ & = & {2 R d R.} \end{array}\tag{4.42}
$$

From the fundamental law of transformation of probabilities, we have that 

$$
\begin{array}{r c l} {p (R ^ {2}) d (R ^ {2})} & = & {p (R) d R} \\ & = & {2 R d R} \end{array}\tag{4.43}
$$

so that 

$$
\begin{array}{r l r} {p (R ^ {2})} & = & {\frac {2 R}{\frac {d (R ^ {2})}{d R}}} \\ & = & {1} \end{array}\tag{4.44}
$$

so that $R ^ { 2 }$ is uniformly distributed on $[ 0 , 1 ] , ( R ^ { 2 } \sim U [ 0 , 1 ] )$ . 

As well, if $\theta = \tan ^ { - 1 } ( V _ { 2 } / V _ { 1 } )$ , i.e. θ is the angle between a line from the origin to the point $( V _ { 1 } , V _ { 2 } )$ and the $V _ { 1 }$ axis, then $\theta \sim U [ 0 , 2 \pi ]$ . Note that 

$$
\begin{array}{r c l} \cos \theta & = & \frac {V _ {1}}{\sqrt {V _ {1} ^ {2} + V _ {2} ^ {2}}} \\ \sin \theta & = & \frac {V _ {2}}{\sqrt {V _ {1} ^ {2} + V _ {2} ^ {2}}}  . \end{array}\tag{4.45}
$$

Now in the original Box Muller algorithm (4.38), 

$$
\begin{array}{r l} \rho = \sqrt {- 2 \log U _ {1}} & ; U _ {1} \sim U [ 0, 1 ] \\ \theta = 2 \Pi U _ {2} & ; U _ {2} \sim U [ 0, 1 ], \end{array}\tag{4.46}
$$

but $\theta = \tan ^ { - 1 } ( V _ { 2 } / V _ { 1 } ) \sim U [ 0 , 2 \pi ]$ , and $R ^ { 2 } = U [ 0 , 1 ]$ . Therefore, if we let $W = R ^ { 2 }$ , then we can replace θ, ρ in algorithm (4.38) by 

$$
\begin{array}{r c l} \theta & = & \tan^ {- 1} \left(\frac {V _ {2}}{V _ {1}}\right) \\ \rho & = & \sqrt {- 2 \log W}. \end{array}\tag{4.47}
$$

Now, the last step in the Box Muller algorithm (4.38) is 

$$
\begin{array}{r c l} Z _ {1} & = & \rho \cos \theta \\ Z _ {2} & = & \rho \sin \theta , \end{array}\tag{4.48}
$$

but since $W = R ^ { 2 } = V _ { 1 } ^ { 2 } + V _ { 2 } ^ { 2 }$ , then cos $\theta = V _ { 1 } / R _ { : }$ sin $\theta = V _ { 2 } / R$ , so that 

$$
\begin{array}{r c l} Z _ {1} & = & \rho \frac {V _ {1}}{\sqrt {W}} \\ Z _ {2} & = & \rho \frac {V _ {2}}{\sqrt {W}}. \end{array}\tag{4.49}
$$

This leads to the following algorithm 

$$
\mathrm{PolarformofBoxMuller}
$$

Repeat Generate $U _ { 1 } \sim U [ 0 , 1 ] , U _ { 2 } \sim U [ 0 , 1 ]$ Let 

$$
\begin{array}{r c l} {V _ {1}} & = & {2 U _ {1} - 1} \\ {V _ {2}} & = & {2 U _ {2} - 1} \\ {W} & = & {V _ {1} ^ {2} + V _ {2} ^ {2}} \end{array}
$$

If( $W < 1 )$ then 

$$
\begin{array}{r l r} {Z _ {1}} & = & {V _ {1} \sqrt {- 2 \log W / W}} \\ {Z _ {2}} & = & {V _ {2} \sqrt {- 2 \log W / W}} \end{array}\tag{4.50}
$$

End If End Repeat 

Consequently, $( Z _ { 1 } , Z _ { 2 } )$ are independent (uncorrelated), and $Z _ { 1 } \sim N ( 0 , 1 )$ , and $Z _ { 2 } \sim N ( 0 , 1 )$ . Because of the rejection step (4.40), about $( 1 - \pi / 4 )$ of the random draws in $[ - 1 , + 1 ] \times [ - 1 , + 1 ]$ are rejected (about 21%), but this method is still generally more eficient than brute force Box Muller. 

## 4.4 Speeding up Monte Carlo

Monte Carlo methods are slow to converge, since the error is given by 

$$
\mathrm{Error} = O (\frac {1}{\sqrt {M}})
$$

where M is the number of samples. There are many methods which can be used to try to speed up convergence. These are usually termed Variance Reduction techniques. 

Perhaps the simplest idea is the Antithetic Variable method. Suppose we compute a random asset path 

$$
{S ^ {i + 1}} = {S ^ {i} \mu \Delta t + S ^ {i} \sigma \phi^ {i} \sqrt {\Delta t}}
$$

where $\phi ^ { i }$ are $N ( 0 , 1 )$ . We store all the $\phi ^ { i } , i = 1 , . . . ,$ for a given path. Call the estimate for the option price from this sample path $V ^ { + }$ . Then compute a second sample path where $( \phi ^ { i } ) ^ { \prime } = - \phi ^ { i } , i = 1 , . . . ,$ . Call this estimate $V ^ { - }$ . Then compute the average 

$$
\bar {V} = \frac {V ^ {+} + V ^ {-}}{2},
$$

and continue sampling in this way. Averaging over all the ${ \bar { V } } ,$ slightly faster convergence is obtained. Intuitively, we can see that this symmetrizes the random paths. 

Let $X ^ { + }$ be the option values obtained from all the $V ^ { + }$ simulations, and $X ^ { - }$ be the estimates obtained from all the $V ^ { - }$ simulations. Note that $V a r ( X ^ { + } ) = V a r ( X ^ { - } )$ (they have the same distribution). Then 

$$
\begin{array}{r c l} V a r (\frac {X ^ {+} + X ^ {-}}{2}) & = & \frac {1}{4} V a r (X ^ {+}) + \frac {1}{4} V a r (X ^ {-}) + \frac {1}{2} C o v (X ^ {+}, X ^ {-}) \\ & = & \frac {1}{2} V a r (X ^ {+}) + \frac {1}{2} C o v (X ^ {+}, X ^ {-}) \end{array}\tag{4.51}
$$

which will be smaller than $V a r ( X ^ { + } ) \mathrm { i f } \ C o v ( X ^ { + } , X ^ { - } )$ is nonpositive. Warning: this is not always the case. For example, if the payof is not a monotonic function of $S ,$ the results may actually be worse than crude Monte Carlo. For example, if the payof is a capped call 

$$
\begin{array}{r c l} \text { payoff } & = & \min (K _ {2}, \max (S - K _ {1}, 0)) \\ & & K _ {2} > K _ {1} \end{array}
$$

then the antithetic method performs poorly. 

Note that this method can be used to estimate the mean. In the MC error estimator (4.13), compute the standard deviation of the estimator as $\begin{array} { r } { \omega = \sqrt { V a r ( \frac { X ^ { + } + X ^ { - } } { 2 } ) } } \end{array}$ 

However, if we want to estimate the distribution of option prices (i.e. a probability distribution), then we should not average each $V ^ { + }$ and $V ^ { - }$ , since this changes the variance of the actual distribution. 

If we want to know the actual variance of the distribution (and not just the mean), then to compute the variance of the distribution, we should just use the estimates $V ^ { + }$ , and compute the estimate of the variance in the usual way. This should also be used if we want to plot a histogram of the distribution, or compute the Value at Risk. 

## 4.5 Estimating the mean and variance

An estimate of the mean ¯x and variance $s _ { M } ^ { 2 }$ of M numbers $x _ { 1 } , x _ { 2 } , . . . , x _ { M }$ is 

$$
{s _ {M} ^ {2}} = {\frac {1}{M - 1} \sum_ {i = 1} ^ {M} (x _ {i} - \bar {x}) ^ {2}}
$$

$$
{\bar {x}} = {\frac {1}{M} \sum_ {i = 1} ^ {M} x _ {i}}\tag{4.52}
$$

Alternatively, one can use 

$$
s _ {M} ^ {2} = \frac {1}{M - 1} \left(\sum_ {i = 1} ^ {M} x _ {i} ^ {2} - \frac {1}{M} \left(\sum_ {i = 1} ^ {M} x _ {i}\right) ^ {2}\right)\tag{4.53}
$$

which has the advantage that the estimate of the mean and standard deviation can be computed in one loop. In order to avoid roundof, the following method is suggested by Seydel (R. Seydel, Tools for Computational Finance, Springer, 2002). Set 

$$
\alpha_ {1} = x _ {1}; \beta_ {1} = 0\tag{4.54}
$$

then compute recursively 

$$
\begin{array}{r c l} \alpha_ {i} & = & \alpha_ {i - 1} + \frac {x _ {i} - \alpha_ {i - 1}}{i} \\ \beta_ {i} & = & \beta_ {i - 1} + \frac {(i - 1) (x _ {i} - \alpha_ {i - 1}) ^ {2}}{i} \end{array}\tag{4.55}
$$

so that 

$$
\begin{array}{r c l} \bar {x} & = & \alpha_ {M} \\ s _ {M} ^ {2} & = & \frac {\beta_ {M}}{M - 1} \end{array}\tag{4.56}
$$

## 4.6 Low Discrepancy Sequences

In a efort to get around the $\frac { 1 } { \sqrt { M } }$ , (M = number of samples) behaviour of Monte Carlo methods, quasi-Monte Carlo methods have been devised. 

These techniques use a deterministic sequence of numbers (low discrepancy sequences). The idea here is that a Monte Carlo method does not fill the sample space very evenly (after all, its random). A low discrepancy sequence tends to sample the space in a orderly fashion. If d is the dimension of the space, then the worst case error bound for an LDS method is 

$$
\mathrm{Error} = O \left(\frac {(\log M) ^ {d}}{M}\right)\tag{4.57}
$$

where M is the number of samples used. Clearly, if d is small, then this error bound is (at least asymptotically) better than Monte Carlo. 

LDS methods generate numbers on [0, 1]. We cannot use the Box-Muller method in this case to produce normally distributed numbers, since these numbers are deterministic. We have to invert the cumulative normal distribution in order to get the numbers distributed with mean zero and standard deviation one on $[ - \infty , + \infty ]$ . So, if $F ( x )$ is the inverse cumulative normal distribution, then 

$$
\begin{array}{r c l} {x _ {L D S}} & = & {\mathrm{uniformlydistributedon[0,1]}} \\ {y _ {L D S}} & = & {F (x _ {L D S}) \mathrm{is} N (0, 1) .} \end{array}\tag{4.58}
$$

Another problem has to do with the fact that if we are stepping through time, i.e. 

$$
\begin{array}{r c l} S ^ {n + 1} & = & S ^ {n} + S ^ {n} (r \Delta t + \phi \sigma \sqrt {\Delta t}) \\ & & \phi = N (0, 1) \end{array}\tag{4.59}
$$

with, say, N steps in total, then we need to think of this as a problem in N dimensional space. In other words, the $k - t h$ timestep is sampled from the $k - t h$ coordinate in this N dimensional space. We are trying to uniformly sample from this N dimensional space. 

Let ˆx be a vector of LDS numbers on [0, 1], in N dimensional space 

$$
\hat {x} = \left[ \begin{array}{c} x _ {1} \\ x _ {2} \\ | \\ x _ {N} \end{array} \right].\tag{4.60}
$$

${ \mathrm { S o } } ,$ an LDS algorithm would proceed as follows, for the $j ^ { \prime } t h$ trial 

• Generate ${ \hat { x } } ^ { j }$ (the $j ^ { \prime } t h$ LDS number in an N dimensional space). 

• Generate the normally distributed vector $\hat { y } ^ { j }$ by inverting the cumulative normal distribution for each component 

$$
\hat {y} ^ {j} = \left[ \begin{array}{c} F (x _ {1} ^ {j}) \\ F (x _ {2} ^ {j}) \\ | \\ F (x _ {N} ^ {j}) \end{array} \right]\tag{4.61}
$$

• Generate a complete sample path $k = 0 , . . . , N - 1$ 

$$
{S _ {j} ^ {k + 1}} = {S _ {j} ^ {k} + S _ {j} ^ {k} (r \Delta t + \hat {y} _ {k + 1} ^ {j} \sigma \sqrt {\Delta t})}\tag{4.62}
$$

• Compute the payof at $S = S _ { j } ^ { N }$ 

The option value is the average of these trials. 

There are a variety of LDS numbers: Halton, Sobol, Niederrieter, etc. Our tests seem to indicate that Sobol is the best. 

Note that the worst case error bound for the error is given by equation (4.57). If we use a reasonable number of timesteps, say 50 − 100, then, $d = 5 0 - 1 0 0$ , which gives a very bad error bound. For d large, the numerator in equation (4.57) dominates. The denominator only dominates when 

$$
M \simeq e ^ {d}\tag{4.63}
$$

which is a very large number of trials for $d \simeq 1 0 0$ . Fortunately, at least for path-dependent options, we have found that things are not quite this bad, and LDS seems to work if the number of timesteps is less than 100 − 200. However, once the dimensionality gets above a few hundred, convergence seems to slow down. 

## 4.7 Correlated Random Numbers

In many cases involving multiple assets, we would like to generate correlated, normally distributed random numbers. Suppose we have $i = 1 , . . . , d$ assets, and each asset follows the simulated path 

$$
{S _ {i} ^ {n + 1}} = {S _ {i} ^ {n} + S _ {i} ^ {n} (r \Delta t + \phi_ {i} ^ {n} \sigma_ {i} \sqrt {\Delta t})}\tag{4.64}
$$

where $\phi _ { i } ^ { n }$ is $N ( 0 , 1 )$ and 

$$
{E (\phi_ {i} ^ {n} \phi_ {j} ^ {n})} = {\rho_ {i j}}\tag{4.65}
$$

where $\rho _ { i j }$ is the correlation between asset i and asset $j .$ 

Now, it is easy to generate a set of d uncorrelated $N ( 0 , 1 )$ variables. Call these $\epsilon _ { 1 } , . . . , \epsilon _ { d } . \mathrm { ~ S o ~ }$ , how do we produce correlated numbers? Let 

$$
[ \Psi ] _ {i j} = \rho_ {i j}\tag{4.66}
$$

be the matrix of correlation coeficients. Assume that this matrix is SPD (if not, one of the random variables is a linear combination of the others, hence this is a degenerate case). Assuming Ψ is SPD, we can Cholesky factor $\Psi = L L ^ { t }$ , so that 

$$
\rho_ {i j} = \sum_ {k} L _ {i k} L _ {k j} ^ {t}\tag{4.67}
$$

Let $\bar { \phi }$ be the vector of correlated normally distributed random numbers (i.e. what we want to get), and let ¯ be the vector of uncorrelated $N ( 0 , 1 )$ numbers (i.e. what we are given). 

$$
\bar {\phi} = \left[ \begin{array}{c} \phi_ {1} \\ \phi_ {2} \\ | \\ \phi_ {d} \end{array} \right]; \bar {\epsilon} = \left[ \begin{array}{c} \epsilon_ {1} \\ \epsilon_ {2} \\ | \\ \epsilon_ {d} \end{array} \right]\tag{4.68}
$$

So, given ¯, we have 

$$
E (\epsilon_ {i} \epsilon_ {j}) = \delta_ {i j}
$$

where 

$$
\begin{array}{r c l} \delta_ {i j} & = & 0; \text {if} i \neq j \\ & = & 1; \text {if} i = j. \end{array}
$$

since the $\epsilon _ { i }$ are uncorrelated. Now, let 

$$
\phi_ {i} = \sum_ {j} L _ {i j} \epsilon_ {j}\tag{4.69}
$$

which gives 

$$
\begin{array}{r c l} \phi_ {i} \phi_ {k} & = & \sum_ {j} \sum_ {l} L _ {i j} L _ {k l} \epsilon_ {l} \epsilon_ {j} \\ & = & \sum_ {j} \sum_ {l} L _ {i j} \epsilon_ {l} \epsilon_ {j} L _ {l k} ^ {t}. \end{array}\tag{4.70}
$$

Now, 

$$
\begin{array}{r c l} E (\phi_ {i} \phi_ {k}) & = & E \left[ \sum_ {j} \sum_ {l} L _ {i j} \epsilon_ {l} \epsilon_ {j} L _ {l k} ^ {t} \right] \\ & = & \sum_ {j} \sum_ {l} L _ {i j} E (\epsilon_ {l} \epsilon_ {j}) L _ {l k} ^ {t} \\ & = & \sum_ {j} \sum_ {l} L _ {i j} \delta_ {l j} L _ {l k} ^ {t} \\ & = & \sum_ {l} L _ {i l} L _ {l k} ^ {t} \\ & = & \rho_ {i j} \end{array}\tag{4.71}
$$

So, in order to generate correlated $N ( 0 , 1 )$ numbers: 

• Factor the correlation matrix $\Psi = L L ^ { t }$ 

• Generate uncorrelated $N ( 0 , 1 )$ numbers $\epsilon _ { i }$ 

• Correlated numbers $\phi _ { i }$ are given from 

$$
\bar {\phi} = L \bar {\epsilon}
$$

## 4.8 Integration of Stochastic Diferential Equations

Up to now, we have been fairly slack about defining what we mean by convergence when we use forward Euler timestepping (4.2) to integrate 

$$
d S = \mu S d t + \sigma S d Z.\tag{4.72}
$$

The forward Euler algorithm is simply 

$$
S ^ {i + 1} = S ^ {i} + S ^ {i} (\mu h + \phi^ {i} \sqrt {h})\tag{4.73}
$$

where $h = \Delta t$ is the finite timestep. For a good overview of these methods, check out (“An algorithmic introduction to numerical simulation of stochastic diferential equations,” by D. Higham, SIAM Review vol. 43 (2001) 525-546). This article also has some good tips on solving SDEs using Matlab, in particular, taking full advantage of the vectorization of Matlab. Note that eliminating as many for loops as possible (i.e. computing all the MC realizations for each timestep in a vector) can reduce computation time by orders of magnitude. 

Before we start defining what we mean by convergence, let’s consider the following situation. Recall that 

$$
d Z = \phi \sqrt {d t}\tag{4.74}
$$

where $\phi$ is a random draw from a normal distribution with mean zero and variance one. Let’s imagine generating a set of $Z$ values at discrete times $t _ { i } .$ , e.g. $Z ( t _ { i } ) = Z _ { i }$ , by 

$$
{Z _ {i + 1}} = {Z _ {i} + \phi \sqrt {\Delta t}.}\tag{4.75}
$$

Now, these are all legitimate points along a Brownian motion path, since there is no timestepping error here, in view of equation (2.53). ${ \mathrm { S o } } ,$ this set of values $\{ Z _ { 0 } , Z _ { 1 } , . . . , \}$ are valid points along a Brownian path. Now, recall that the exact solution (for a given Brownian path) of equation (4.72) is given by equation (2.57) 

$$
S (T) = S (0) \exp [ (\mu - \frac {\sigma^ {2}}{2}) t + \sigma (Z (T) - Z (0)) ]\tag{4.76}
$$

where T is the stopping time of the simulation. 

Now if we integrate equation (4.72) using forward Euler, with the discrete timesteps $\Delta t = t _ { i + 1 } - t _ { i }$ , using the realization of the Brownian path $\{ Z _ { 0 } , Z _ { 1 } , . . . , \}$ , we will not get the exact solution (4.76). This is because even though the Brownian path points are exact, time discretization errors are introduced in equation (4.73). $\mathrm { S o } .$ how can we systematically study convergence of algorithm (4.73)? We can simply take smaller timesteps. However, we want to do this by filling in new Z values in the Brownian path, while keeping the old values (since these are perfectly legitimate values). Let $S ( T ) ^ { h }$ represent the forward Euler solution (4.73) for a fixed timestep h. Let $S ( T )$ be the exact solution (4.76). As $h  0$ , we would expect $S ( T ) ^ { h } \to { \dot { S } } ( T )$ , for a given path. 

## 4.8.1 The Brownian Bridge

So, given a set of valid $Z _ { k } ,$ , how do we refine this path, keeping the existing points along this path? In particular, suppose we have two points $Z _ { i } , Z _ { k }$ , at $( t _ { i } , t _ { k } )$ , and we would like to generate a point $Z _ { j }$ at $t _ { j } .$ with $t _ { i } < t _ { j } < t _ { k }$ . How should we pick $Z _ { j } ?$ What density function should we use when generating $Z _ { j } ,$ , given that $Z _ { k }$ is known? 

Let $x , y$ be two draws from a normal distribution with mean zero and variance one. Suppose we have the point $Z ( t _ { i } ) = Z _ { i }$ and we generate $Z ( t _ { j } ) = Z _ { j } , Z ( t _ { k } ) = Z _ { k }$ along the Wiener path, 

$$
{Z _ {j}} = {Z _ {i} + x \sqrt {t _ {j} - t _ {i}}}\tag{4.77}
$$

$$
{Z _ {k}} = {Z _ {j} + y \sqrt {t _ {k} - t _ {j}}}\tag{4.78}
$$

$$
Z _ {k} = Z _ {i} + x \sqrt {t _ {j} - t _ {i}} + y \sqrt {t _ {k} - t _ {j}}.\tag{4.79}
$$

So, given $( x , y )$ , and $Z _ { i } ,$ we can generate $Z _ { j } , Z _ { k }$ . Suppose on the other hand, we have $Z _ { i } .$ , and we generate $Z _ { k }$ directly using 

$$
{Z _ {k}} = {Z _ {i} + z \sqrt {t _ {k} - t _ {i}},}\tag{4.80}
$$

where z is $N ( 0 , 1 )$ . Then how do we generate $Z _ { j }$ using equation (4.77)? Since we are now specifying that we know $Z _ { k } .$ , this means that our method for generating $Z _ { j }$ is constrained. For example, given z, we must have that, from equations (4.79) and (4.80) 

$$
y = \frac {z \sqrt {t _ {k} - t _ {i}} - x \sqrt {t _ {j} - t _ {i}}}{\sqrt {t _ {k} - t _ {j}}}.\tag{4.81}
$$

Now the probability density of drawing the pair $( x , y )$ given z, denoted by $p ( x , y | z )$ is 

$$
p (x, y | z) = \frac {p (x) p (y)}{p (z)}\tag{4.82}
$$

where $p ( . . )$ is a standard normal distribution, and we have used the fact that successive increments of a Brownian process are uncorrelated. 

From equation (4.81), we can write $y = y ( x , z )$ , so that $p ( x , y | z ) = p ( x , y ( x , z ) | z )$ 

$$
\begin{array}{r c l} {p (x, y (x, z) | z)} & = & {\frac {p (x) p (y (x , z))}{p (z)}} \\ & = & {\frac {1}{\sqrt {2 \pi}} \exp \left[ - \frac {1}{2} (x ^ {2} + y ^ {2} - z ^ {2}) \right]} \end{array}\tag{4.83}
$$

or (after some algebra, using equation (4.81)) 

$$
\begin{array}{r c l} p (x | z) & = & \frac {1}{\sqrt {2 \pi}} \exp \left[ - \frac {1}{2} (x - \alpha z) ^ {2} / \beta^ {2} \right] \\ & & \alpha = \sqrt {\frac {t _ {j} - t _ {i}}{t _ {k} - t _ {i}}} \\ & & \beta = \sqrt {\frac {t _ {k} - t _ {j}}{t _ {k} - t _ {i}}} \end{array}\tag{4.84}
$$

so that x is normally distributed with mean αz and variance $\beta ^ { 2 }$ . Since 

$$
z = \frac {Z _ {k} - Z _ {i}}{\sqrt {t _ {k} - t _ {i}}}\tag{4.85}
$$

we have that x has mean 

$$
{ E ( x ) } { = } { \frac { \sqrt { t _ { j } - t _ { i } } } { t _ { k } - t _ { i } } ( Z _ { k } - Z _ { i } ) }\tag{4.86}
$$

and variance 

$$
E [ (x - E (x)) ^ {2} ] = \frac {t _ {k} - t _ {j}}{t _ {k} - t _ {i}}\tag{4.87}
$$

Now, let 

$$
{ x } { = } { \frac { \sqrt { t _ { j } - t _ { i } } } { t _ { k } - t _ { i } } ( Z _ { k } - Z _ { i } ) + \phi \sqrt { \frac { t _ { k } - t _ { j } } { t _ { k } - t _ { i } } } }\tag{4.88}
$$

where $\phi$ is $N ( 0 , 1 )$ . Clearly, x satisfies equations (4.86) and (4.88). Substituting equation (4.88) into (4.77) gives 

$$
{Z _ {j}} = {\left(\frac {t _ {k} - t _ {j}}{t _ {k} - t _ {i}}\right) Z _ {i} + \left(\frac {t _ {j} - t _ {i}}{t _ {k} - t _ {i}}\right) Z _ {k} + \phi \sqrt {\frac {(t _ {j} - t _ {i}) (t _ {k} - t _ {j})}{(t _ {k} - t _ {i})}}}\tag{4.89}
$$

where $\phi$ is $N ( 0 , 1 )$ . Equation (4.89) is known as the Brownian Bridge. 

Figure 4.1 shows diferent Brownian paths constructed for diferent timestep sizes. An initial coarse path is constructed, then the fine timestep path is constructed from the coarse path using a Brownian Bridge. By construction, the final timestep path will pass through the coarse timestep nodes. 

Figure 4.2 shows the asset paths integrated using the forward Euler algorithm (4.73) fed with the Brownian paths in Figure 4.1. In this case, note that the fine timestep path does not coincide with the coarse timestep nodes, due to the timestepping error. 

## 4.8.2 Strong and Weak Convergence

Since we are dealing with a probabilistic situation here, it is not obvious how to define convergence. Given a number of points along a Brownian path, we could imagine refining this path (using a Brownian Bridge), and then seeing if the solution converged to exact solution. For the model SDE (4.72), we could ask that 

$$
E \left[ | S (T) - S ^ {h} (T) | \right] \leq C o n s t. h ^ {\gamma}\tag{4.90}
$$

where the expectation in equation (4.90) is over many Brownian paths, and h is the timestep size. Note that $S ( T )$ is the exact solution along a particular Brownian path; the same path used to compute $S ^ { h } ( T )$ Criterion (4.90) is called strong convergence. A less strict criterion is 

$$
{| E [ S (T) ] - E [ S ^ {h} (T) ] |} \leq {C o n s t. h ^ {\gamma}}\tag{4.91}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/ba33ce3265add43ae1cad9ecadadd71f979ea9b50ef519719add4bf99988af4e.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/f6d8c8c7a64f297d0be1ac63599aedd2001c1542c3689c360ddf75c78a135daf.jpg)



Figure 4.1: Efect of adding more points to a Brownian path using a Brownian bridge. Note that the small timestep points match the coarse timestep points. Left: each coarse timestep is divided into 16 substeps. Right: each coarse timestep divided into $6 4$ substeps.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/0160d4b2f7e53ac24fee33def6e41154bc37ceb5897fe95a4a3193167ffb272b.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/fabf86075bc3d912664efe093b9abc4a7e427037eeb51119bf9cab4428b738fd.jpg)



Figure 4.2: Brownian paths shown in Figure 4.1 used to determine asset price paths using forward Euler timestepping (4.73). In this case, note that the asset paths for fine and coarse timestepping do not agree at the final time (due to the timestepping error). Eventually, for small enough timesteps, the final asset value will converge to the exact solution to the SDE. Left: each coarse timestep is divided into 16 substeps. Right: each coarse timestep divided into 64substeps.


<table><tr><td>T</td><td>.25</td></tr><tr><td>σ</td><td>.4</td></tr><tr><td>μ</td><td>.06</td></tr><tr><td>S0</td><td>100</td></tr></table>


Table 4.1: Data used in the convergence tests.


<table><tr><td>Timesteps</td><td>Strong Error (4.90)</td><td>Weak Error (4.91)</td></tr><tr><td>72</td><td>.0269</td><td>.00194</td></tr><tr><td>144</td><td>.0190</td><td>.00174</td></tr><tr><td>288</td><td>.0135</td><td>.00093</td></tr><tr><td>576</td><td>.0095</td><td>.00047</td></tr></table>


Table 4.2: Convergence results, 100,000 samples used. Data in Table $4 . 1 .$


It can be shown that using forward Euler results in weak convergence with $\gamma = 1$ , and strong convergence with $\gamma = . 5$ 

Table 4.1 shows some test data used to integrate the SDE (4.72) using method (4.73). A series of Brownian paths was constructed, beginning with a coarse timestep path. These paths were systematically refined using the Brownian Bridge construction. Table 4.2 shows results where the strong and weak convergence errors are estimated as 

$$
\mathrm{StrongError} = \frac {1}{N} \sum_ {i = 1} ^ {N} \left[ | S (T) _ {i} - S ^ {h} (T) _ {i} | \right]\tag{4.92}
$$

$$
\text { Weak   Error } = \left| \frac {1}{N} \sum_ {i = 1} ^ {N} [ S (T) _ {i} ] - \frac {1}{N} \sum_ {i = 1} ^ {N} \left[ S ^ {h} (T) _ {i} \right] \right|,\tag{4.93}
$$

where $S ^ { h } ( T ) _ { i }$ is the solution obtained by forward Euler timestepping along the $i ^ { \prime } t h$ Brownian path, and $S ( T ) _ { i }$ is the exact solution along this same path, and N is the number of samples. Note that for equation (4.72), we have the exact solution 

$$
\lim _ {N \to \infty} \frac {1}{N} \sum_ {i = 1} ^ {N} [ S (T) _ {i} ] = S _ {0} e ^ {\mu T}\tag{4.94}
$$

but we do not replace the approximate sampled value of the limit in equation (4.93) by the theoretical limit (4.94). If we use enough Monte Carlo samples, we could replace the approximate expression 

$$
\lim _ {N \to \infty} \frac {1}{N} \sum_ {i = 1} ^ {N} [ S (T) _ {i} ]
$$

by $S _ { 0 } e ^ { \mu T }$ , but for normal parameters, the Monte Carlo sampling error is much larger than the timestepping error, so we would have to use an enormous number of Monte Carlo samples. Estimating the weak error using equation (4.93) will measure the timestepping error, as opposed to the Monte Carlo sampling error. However, for normal parameters, even using equation (4.93) requires a large number of Monte Carlo samples in order to ensure that the error is dominated by the timestepping error. 

In Table 4.1, we can see that the ratio of the errors is about $\sqrt { 2 }$ for the strong error, and about two for the weak error. This is consistent with a convergence rate of $\gamma = . 5$ for strong convergence, and $\gamma = 1 . 0$ for weak convergence. 

## 4.9 Matlab and Monte Carlo Simulation

A straightforward implementation of Monte Carlo timestepping for solving the SDE 

$$
{ d S } { = } { \mu S ~ d t + \sigma S ~ d Z }\tag{4.95}
$$

in Matlab is shown in Algorithm (4.96). This code runs very slowly. 

```matlab
Slow.m

randn('state',100);
T = 1.00;    % expiry time
sigma = 0.25;    % volatility
mu = .10;    % P measure drift
S_init = 100;    % initial value
N_sim = 10000;    % number of simulations
N = 100;    % number of timesteps
delt = T/N;    % timestep

drift = mu*delt;
sigma_sqrt_delt = sigma*sqrt(delt);
S_new = zeros(N_sim,1);

for m=1:N_sim
S = S_init;
for i=1:N % timestep loop

S = S + S*( drift + sigma_sqrt_delt*randn(1,1) );

S = max(0.0, S );
% check to make sure that S_new cannot be < 0

end % timestep loop
S_new(m,1) = S;
end % simulation loop

n_bin = 200;
hist(S_new, n_bin);

stndrd_dev = std(S_new);
disp(sprintf('standard deviation: %.5g\n',stndrd_dev));

mean_S = mean(S_new);
disp(sprintf('mean: %.5g\n',stndrd_dev)); 
```

Alternatively, we can use Matlab’s vectorization capabilities to interchange the timestep loop and the simulation loop. The innermost simulation loop can be replaced by vector statements, as shown in Algorithm (4.97). This runs much faster. 

```matlab
Fast.m

randn('state',100);
%
T = 1.00;    % expiry time
sigma = 0.25;    % volatility
mu = .10;    % P measure drift
S_init = 100;    % initial value
N_sim = 10000;    % number of simulations
N = 100;    % number of timesteps
delt = T/N;    % timestep

drift = mu*delt;
sigma_sqrt_delt = sigma*sqrt(delt);

S_old = zeros(N_sim,1);
S_new = zeros(N_sim,1);

S_old(1:N_sim,1) = S_init;

for i=1:N % timestep loop

% now, for each timestep, generate info for
% all simulations

S_new(:,1) = S_old(:,1) +...
    S_old(:,1).*( drift + sigma_sqrt_delt*randn(N_sim,1) );

S_new(:,1) = max(0.0, S_new(:,1));
    % check to make sure that S_new cannot be < 0

S_old(:,1) = S_new(:,1);
%
% end of generation of all data for all simulations
% for this timestep

end % timestep loop

n_bin = 200;
hist(S_new, n_bin);

stndrd_dev = std(S_new);
disp(sprintf('standard deviation: %.5g\n', stndrd_dev));

mean_S = mean(S_new);
disp(sprintf('mean: %.5g\n', stndrd_dev)); 
```

## 5 The Binomial Model

We have seen that a problem with the Monte Carlo method is that it is dificult to use for valuing American style options. Recall that the holder of an American option can exercise the option at any time and receive the payof. In order to determine whether or not it is worthwhile to hold the option, we have to compare the value of continuing to hold the option (the continuation value) with the payof. If the continuation value is greater than the payof, then we hold; otherwise, we exercise. 

At any point in time, the continuation value depends on what happens in the future. Clearly, if we simulate forward in time, as in the Monte Carlo approach, we don’t know what happens in the future, and hence we don’t know how to act optimally. This is actually a dynamic programming problem. These sorts of problems are usually solved by proceeding from the end point backwards. We use the same idea here. We have to start from the terminal time and work backwards. 

Recall that we can determine the no-arbitrage value of an option by pretending we live in a risk-neutral world, where risky assets drift at r and are discounted at r. If we let $X = \log { S }$ then the risk neutral process for X is (from equation (2.55) ) 

$$
{ d X } { = } { ( r - \frac { \sigma ^ { 2 } } { 2 } ) d t + \sigma d Z . }\tag{5.1}
$$

Now, we can construct a discrete approximation to this random walk using the lattice discussed in Section 2.5. In fact, all we have to do is let let $\begin{array} { r } { \alpha = r - \frac { \sigma ^ { 2 } } { 2 } } \end{array}$ , so that equation (5.1) is formally identical to equation (2.4). In order to ensure that in the limit as $\Delta t \to 0$ , we get the process (5.1), we require that the sizes of the random jumps are $\Delta X = \sigma { \sqrt { \Delta t } }$ and that the probabilities of up $( p )$ and down $( q )$ moves are 

$$
\begin{array}{r c l} {p ^ {r}} & = & {\frac {1}{2} [ 1 + \frac {\alpha}{\sigma} \sqrt {\Delta t} ]} \\ & = & {\frac {1}{2} [ 1 + \left(\frac {r}{\sigma} - \frac {\sigma}{2}\right) \sqrt {\Delta t} ]} \\ {q ^ {r}} & = & {\frac {1}{2} [ 1 - \frac {\alpha}{\sigma} \sqrt {\Delta t} ]} \\ & = & {\frac {1}{2} [ 1 - \left(\frac {r}{\sigma} - \frac {\sigma}{2}\right) \sqrt {\Delta t} ],} \end{array}\tag{5.2}
$$

where we have denoted the risk neutral probabilities by $p ^ { r }$ and $q ^ { r }$ to distinguish them from the real probabilities $p , q .$ 

Now, we will switch to a more common notation. If we are at node $j ,$ timestep $n ,$ we will denote this node location by $X _ { j } ^ { n }$ . Recall that $X = \log { S }$ , so that in terms of asset price, this is $\bar { S } _ { i } ^ { n } = e ^ { X _ { j } ^ { n } }$ 

Now, consider that at node $( j , n )$ , the asset can move up with probability $p ^ { r }$ and down with probability $q ^ { r }$ . In other words 

$$
\begin{array}{l l l} S _ {j} ^ {n} & \to S _ {j + 1} ^ {n + 1} ; & \text {with probability p^{r}} \\ S _ {j} ^ {n} & \to S _ {j} ^ {n + 1} ; & \text {with probability q^{r}} \end{array}\tag{5.3}
$$

Now, since in Section 2.5 we showed that $\Delta X = \sigma { \sqrt { \Delta t } }$ , so that $( S = e ^ { X } )$ 

$$
\begin{array}{r l r} {S _ {j + 1} ^ {n + 1}} & = & {S _ {j} ^ {n} e ^ {\sigma \sqrt {\Delta t}}} \\ {S _ {j} ^ {n + 1}} & = & {S _ {j} ^ {n} e ^ {- \sigma \sqrt {\Delta t}}} \end{array}\tag{5.4}
$$

or 

$$
{S _ {j} ^ {n}} = {S _ {0} ^ {0} e ^ {(2 j - n) \sigma \sqrt {\Delta t}}; j = 0,.., n}\tag{5.5}
$$

$\mathrm { S o } .$ the first step in the process is to construct a tree of stock price values, as shown on Figure 5. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/986a16b35e80d78e5bc79c1a6860c240d7b57704331c6cc91633f8185395b37c.jpg)



Figure 5.1: Lattice of stock price values


Associated with each stock price on the lattice is the option value $V _ { j } ^ { n }$ . We first set the value of the option at $T = N \Delta t$ to the payof. For example, if we are valuing a put option, then 

$$
V _ {j} ^ {N} = \max (K - S _ {j} ^ {N}, 0); j = 0, \dots , N\tag{5.6}
$$

Then, we can use the risk neutral world idea to determine the no-arbitrage value of the option (it is the expected value in the risk neutral world). We can do this by working backward through the lattice. The value today is the discounted expected future value 

## European Lattice Algorithm

$$
\begin{array}{r c l} V _ {j} ^ {n} & = & e ^ {- r \Delta t} \left(p ^ {r} V _ {j + 1} ^ {n + 1} + q ^ {r} V _ {j} ^ {n + 1}\right) \\ & & n = N - 1,..., 0 \\ & & j = 0,..., n \end{array}\tag{5.7}
$$

Rolling back through the tree, we obtain the value at $S _ { 0 } ^ { 0 }$ today, which is $V _ { 0 } ^ { 0 }$ 

If the option is an American put, we can determine if it is optimal to hold or exercise, since we know the continuation value. In this case the rollback (5.7) becomes 

## American Lattice Algorithm

$$
\begin{array}{r c l} (V _ {j} ^ {n}) ^ {c} & = & e ^ {- r \Delta t} \left(p ^ {r} V _ {j + 1} ^ {n + 1} + q ^ {r} V _ {j} ^ {n + 1}\right) \\ V _ {j} ^ {n} & = & \max \left((V _ {j} ^ {n}) ^ {c}, \max (K - S _ {j} ^ {n}, 0)\right) \\ & & n = N - 1, \dots , 0 \\ & & j = 0, \dots , n \end{array}\tag{5.8}
$$

which is illustrated in Figure 5. 

The binomial lattice method has the following advantages 

• It is very easy to code for simple cases. 

• It is easy to explain to managers. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/c485c8370e48997062e8aaf6358171a328f677cde5be80481131ac7af4685d41.jpg)



Figure 5.2: Backward recursion step.


• American options are easy to handle. 

However, the binomial lattice method has the following disadvantages 

• Except for simple cases, coding becomes complex. For example, if we want to handle simple barrier options, things become nightmarish. 

• This method is algebraically identical to an explicit finite diference solution of the Black-Scholes equation. Consequently, convergence is at an $O ( \Delta t )$ rate. 

• The probabilities $p ^ { r } , q ^ { r }$ are not real probabilities, they are simply the coeficients in a particular discretization of a PDE. Regarding them as probabilities leads to much fuzzy thinking, and complex wrong-headed arguments. 

If we are going to solve the Black-Scholes PDE, we might as well do it right, and not fool around with lattices. 

## 5.1 A No-arbitrage Lattice

We can also derive the lattice method directly from the discrete lattice model in Section 2.5. Suppose we assume that 

$$
d S = \mu S d t + \sigma S d Z\tag{5.9}
$$

and letting $X = \log { S }$ , we have that 

$$
d X = (\mu - \frac {\sigma^ {2}}{2}) d t + \sigma d Z\tag{5.10}
$$

so that $\begin{array} { r } { \alpha = \mu - \frac { \sigma ^ { 2 } } { 2 } } \end{array}$ in equation (2.19). Now, let’s consider the usual hedging portfolio at $t = n \Delta t , S = S _ { j } ^ { n }$ 

$$
P _ {j} ^ {n} = V _ {j} ^ {n} - (\alpha^ {h}) S _ {j} ^ {n},\tag{5.11}
$$

where $V _ { j } ^ { n }$ is the value of the option at $t = n \Delta t , S = S _ { j } ^ { n } . \mathrm { \ A t \ } t = ( n + 1 ) \Delta t ,$ 

$$
\begin{array}{r c l}S _ {j} ^ {n}&\rightarrow&S _ {j + 1} ^ {n + 1}; \quad \text {with probability p}\\S _ {j} ^ {n}&\rightarrow&S _ {j} ^ {n + 1}; \quad \text {with probability q}\\&&S _ {j + 1} ^ {n + 1} = S _ {j} ^ {n} e ^ {\sigma \sqrt {\Delta t}}\\&&S _ {j} ^ {n + 1} = S _ {j} ^ {n} e ^ {- \sigma \sqrt {\Delta t}}\end{array}
$$

so that the value of the hedging portfolio at $t = n + 1$ is 

$$
{P _ {j + 1} ^ {n + 1}} = {V _ {j + 1} ^ {n + 1} - (\alpha^ {h}) S _ {j + 1} ^ {n + 1}; \mathrm{withprobability} p}\tag{5.12}
$$

$$
{P _ {j} ^ {n + 1}} = {V _ {j} ^ {n + 1} - (\alpha^ {h}) S _ {j} ^ {n + 1}; \mathrm{withprobability} q.}\tag{5.13}
$$

Now, as in Section 2.3, we can determine $( \alpha ^ { h } )$ so that the value of the hedging portfolio is independent of $p , q$ . We do this by requiring that 

$$
P _ {j + 1} ^ {n + 1} = P _ {j} ^ {n + 1}\tag{5.14}
$$

so that 

$$
V _ {j + 1} ^ {n + 1} - (\alpha^ {h}) S _ {j + 1} ^ {n + 1} = V _ {j} ^ {n + 1} - (\alpha^ {h}) S _ {j} ^ {n + 1}
$$

which gives 

$$
(\alpha^ {h}) = \frac {V _ {j + 1} ^ {n + 1} - V _ {j} ^ {n + 1}}{S _ {j + 1} ^ {n + 1} - S _ {j} ^ {n + 1}}.\tag{5.15}
$$

Since this portfolio is risk free, it must earn the risk free rate of return, so that 

$$
\begin{array}{r c l} P _ {j} ^ {n} & = & e ^ {- r \Delta t} P _ {j + 1} ^ {n + 1} \\ & = & e ^ {- r \Delta t} P _ {j} ^ {n + 1}. \end{array}\tag{5.16}
$$

Now, substitute for $P _ { j } ^ { n }$ from equation (5.11), with $P _ { j + 1 } ^ { n + 1 }$ from equation (5.13), and $( \alpha ^ { h } )$ from equation (5.15) gives 

$$
\begin{array}{r c l} {V _ {j} ^ {n}} & = & {e ^ {- r \Delta t} \left(p ^ {r *} V _ {j + 1} ^ {n + 1} + q ^ {r *} V _ {j} ^ {n + 1}\right)} \\ & & \\ & & {p ^ {r *} = \frac {e ^ {r \Delta t} - e ^ {- \sigma \sqrt {\Delta t}}}{e ^ {\sigma \sqrt {\Delta t}} - e ^ {- \sigma \sqrt {\Delta t}}}} \\ & & {q ^ {r *} = 1 - p ^ {r *}.} \end{array}\tag{5.17}
$$

Note that $p ^ { r * } , q ^ { r * }$ do not depend on the real drift rate $\mu ,$ which is expected. If we expand $p ^ { r * } , q ^ { r * }$ in a Taylor Series, and compare with the $p ^ { r } , q ^ { r }$ in equations (5.2), we can show that 

$$
\begin{array}{r c l} p ^ {r *} & = & p ^ {r} + O ((\Delta t) ^ {3 / 2}) \\ q ^ {r *} & = & q ^ {r} + O ((\Delta t) ^ {3 / 2}). \end{array}\tag{5.18}
$$

After a bit more work, one can show that the value of the option at $t = 0 , V _ { 0 } ^ { 0 }$ using either $p ^ { r * } , q ^ { r * }$ or $p ^ { r } , q ^ { r }$ is the same to $O ( \Delta t )$ , which is not surprising, since these methods can both be regarded as an explicit finite diference approximation to the Black-Scholes equation, having truncation error $O ( \Delta t )$ . The definition $p ^ { r * } , q ^ { r * }$ is the common definition in finance books, since the tree has no-arbitrage. 

What is the meaning of a no-arbitrage tree? If we are sitting at node $S _ { j } ^ { n }$ , and assuming that there are only two possible future states 

$$
\begin{array}{r c l r} S _ {j} ^ {n} & \to & S _ {j + 1} ^ {n + 1}    ; & \text {with probability p} \\ S _ {j} ^ {n} & \to & S _ {j} ^ {n + 1}    ; & \text {with probability q} \end{array}
$$

then using $( \alpha ^ { h } )$ from equation (5.15) guarantees that the hedging portfolio has the same value in both future states. 

But let’s be a bit more sensible here. Suppose we are hedging a portfolio of RIM stock. Let $\Delta t =$ one day. Suppose the price of RIM stocks is $10 today. Do we actually believe that tomorrow there are only two possible prices for Rim stock 

$$
\begin{array}{r c l} {S _ {u p}} & = & {1 0 e ^ {\sigma \sqrt {\Delta t}}} \\ {S _ {d o w n}} & = & {1 0 e ^ {- \sigma \sqrt {\Delta t}} ?} \end{array}\tag{5.19}
$$

Of course not. This is obviously a highly simplified model. The fact that there is no-arbitrage in the context of the simplified model does not really have a lot of relevance to the real-world situation. The best that can be said is that if the Black-Scholes model was perfect, then we have that the portfolio hedging ratios computed using either $p ^ { r } , q ^ { r }$ or $p ^ { r * } , q ^ { r * }$ are both correct to $O ( \Delta t )$ 

## 6 More on Ito’s Lemma

In Section 2.6.1, we mysteriously made the infamous comment 

...it can be shown that $d Z ^ { 2 } \to d t$ as $d t \to 0$ 

In this Section, we will give some justification this remark. For a lot more details here, we refer the reader to Stochastic Diferential Equations, by Bernt Oksendal, Springer, 1998. 

We have to go back here, and decide what the statement 

$$
{ d X } { = } { \alpha d t + c d Z }\tag{6.1}
$$

really means. The only sensible interpretation of this is 

$$
X (t) - X (0) = \int_ {0} ^ {t} \alpha (X (s), s) d s + \int_ {0} ^ {t} c (X (s), s) d Z (s).\tag{6.2}
$$

where we can interpret the integrals as the limit, as $\Delta t \to 0$ of a discrete sum. For example, 

$$
\begin{array}{r c l} \int_ {0} ^ {t} c (X (s), s) d Z (s) & = & \lim _ {\Delta t \to 0} \sum_ {j = 0} ^ {j = N - 1} c _ {j} \Delta Z _ {j} \\ & & c _ {j} = c (X (Z _ {j}), t _ {j}) \\ & & Z _ {j} = Z (t _ {j}) \\ & & \Delta Z _ {j} = Z (t _ {j + 1}) - Z (t _ {j}) \\ & & \Delta t = t _ {j + 1} - t _ {j} \\ & & N = t / (\Delta t) \end{array}\tag{6.3}
$$

In particular, in order to derive Ito’s Lemma, we have to decide what 

$$
\int_ {0} ^ {t} c (X (s), s) d Z (s) ^ {2}\tag{6.4}
$$

means. Replace the integral by a sum, 

$$
\int_ {0} ^ {t} c (X (s), s) d Z (s) ^ {2} = \lim _ {\Delta t \to 0} \sum_ {j = 0} ^ {j = N - 1} c (X _ {j}, t _ {j}) \Delta Z _ {j} ^ {2}.\tag{6.5}
$$

Note that we have evaluated the integral using the left hand end point of each subinterval (the no peeking into the future principle). 

From now on, we will use the notation 

$$
\sum_ {j} \equiv \sum_ {j = 0} ^ {j = N - 1}.\tag{6.6}
$$

Now, we claim that 

$$
\int_ {0} ^ {t} c (X (s), s) d Z ^ {2} (s) = \int_ {0} ^ {t} c (X (s), s) d s\tag{6.7}
$$

or 

$$
\lim _ {\Delta t \to 0} \left[ \sum_ {j} c _ {j} \Delta Z _ {j} ^ {2} \right] = \lim _ {\Delta t \to 0} \sum_ {j} c _ {j} \Delta t\tag{6.8}
$$

which is what we mean by equation (6.7). i.e. we can say that $d Z ^ { 2 } $ dt as $d t \to 0$ 

Now, let’s consider a finite $\Delta t .$ , and consider the expression 

$$
E \left[ \left(\sum_ {j} c _ {j} \Delta Z _ {j} ^ {2} - \sum_ {j} c _ {j} \Delta t\right) ^ {2} \right]\tag{6.9}
$$

If equation (6.9) tends to zero as $\Delta t \to 0$ , then we can say that (in the mean square limit) 

$$
\begin{array}{r l r} \lim _ {\Delta t \to 0} \left[ \sum_ {j} c _ {j} \Delta Z _ {j} ^ {2} \right] & = & \lim _ {\Delta t \to 0} \sum_ {j} c _ {j} \Delta t \\ & = & \int_ {0} ^ {t} c (X (s), s) d s \end{array}\tag{6.10}
$$

so that in this sense 

$$
\int_ {0} ^ {t} c (X, s) d Z ^ {2} = \int_ {0} ^ {t} c (X, s) d s\tag{6.11}
$$

and hence we can say that 

$$
d Z ^ {2} \rightarrow d t\tag{6.12}
$$

with probability one as $\Delta t  0$ 

Now, expanding equation (6.9) gives 

$$
E \left[ \left(\sum_ {j} c _ {j} \Delta Z _ {j} ^ {2} - \sum_ {j} c _ {j} \Delta t\right) ^ {2} \right] = \sum_ {i j} E \left[ c _ {j} (\Delta Z _ {j} ^ {2} - \Delta t) c _ {i} (\Delta Z _ {i} ^ {2} - \Delta t) \right].\tag{6.13}
$$

Now, note the following 

• The increments of Brownian motion are uncorrelated, i.e. $C o v [ \Delta Z _ { i } \Delta Z _ { j } ] = 0 , i \neq j$ , which means that Cov $\left[ \Delta Z _ { i } ^ { 2 } \Delta Z _ { j } ^ { 2 } \right] = 0$ , or $E \left[ ( \Delta Z _ { j } ^ { 2 } - \Delta t ) ( \Delta Z _ { i } ^ { 2 } - \Delta t ) \right] = 0 , i \neq j$ 

$c _ { i } = c ( t _ { i } , X ( Z _ { i } ) )$ , and $\Delta Z _ { i }$ are independent. 

It then follows that for $i < j$ 

$$
\begin{array}{r c l} {E \left[ c _ {j} (\Delta Z _ {j} ^ {2} - \Delta t) c _ {i} (\Delta Z _ {i} ^ {2} - \Delta t) \right]} & = & {E [ c _ {i} c _ {j} (\Delta Z _ {i} ^ {2} - \Delta t) ] E [ (\Delta Z _ {j} ^ {2} - \Delta t) ]} \\ & = & 0. \end{array}\tag{6.14}
$$

Similarly, if $i > j$ 

$$
\begin{array}{r c l} {E \left[ c _ {j} (\Delta Z _ {j} ^ {2} - \Delta t) c _ {i} (\Delta Z _ {i} ^ {2} - \Delta t) \right]} & = & {E [ c _ {i} c _ {j} (\Delta Z _ {j} ^ {2} - \Delta t) ] E [ (\Delta Z _ {i} ^ {2} - \Delta t) ]} \\ & = & 0. \end{array}
$$

(6.15) 

So that in all cases 

$$
{E \left[ c _ {j} (\Delta Z _ {j} ^ {2} - \Delta t) c _ {i} (\Delta Z _ {i} ^ {2} - \Delta t) \right]} = {\delta_ {i j} E \left[ c _ {i} ^ {2} (\Delta Z _ {i} ^ {2} - \Delta t) ^ {2} \right].}\tag{6.16}
$$

It also follows from the above properties that 

$$
{E [ c _ {j} ^ {2} (\Delta Z _ {j} ^ {2} - \Delta t) ^ {2} ]} = {E [ c _ {j} ^ {2} ] E [ (\Delta Z _ {j} ^ {2} - \Delta t) ^ {2} ]}\tag{6.17}
$$

since $c _ { j }$ and $( \Delta Z _ { i } ^ { 2 } - \Delta t )$ are independent. 

Using equations (6.16-6.17), then equation (6.13) becomes 

$$
\sum_ {i j} E \left[ c _ {j} (\Delta Z _ {j} ^ {2} - \Delta t) c _ {i} (\Delta Z _ {i} ^ {2} - \Delta t) \right] = \sum_ {i} E [ c _ {i} ^ {2} ] E \left[ (\Delta Z _ {i} ^ {2} - \Delta t) ^ {2} \right].\tag{6.18}
$$

Now, 

$$
\sum_ {i} E [ c _ {i} ^ {2} ] E \left[ (\Delta Z _ {i} ^ {2} - \Delta t) ^ {2} \right] = \sum_ {i} E [ c _ {i} ^ {2} ] \left(E \left[ \Delta Z _ {i} ^ {4} \right] - 2 \Delta t E \left[ \Delta Z _ {i} ^ {2} \right] + (\Delta t) ^ {2}\right).\tag{6.19}
$$

Recall that $( \Delta Z ) ^ { 2 }$ is $N ( 0 , \Delta t )$ ( normally distributed with mean zero and variance $\Delta t )$ so that 

$$
\begin{array}{r c l} {E \left[ (\Delta Z _ {i}) ^ {2} \right]} & = & {\Delta t} \\ {E \left[ (\Delta Z _ {i}) ^ {4} \right]} & = & {3 (\Delta t) ^ {2}} \end{array}\tag{6.20}
$$

so that equation (6.19) becomes 

$$
E \left[ \Delta Z _ {i} ^ {4} \right] - 2 \Delta t E \left[ \Delta Z _ {i} ^ {2} \right] + (\Delta t) ^ {2} = 2 (\Delta t) ^ {2}\tag{6.21}
$$

and 

$$
\begin{array}{r c l} \sum_ {i} E [ c _ {i} ^ {2} ] E [ (\Delta Z _ {i} ^ {2} - \Delta t) ^ {2} ] & = & 2 \sum_ {i} E [ c _ {i} ^ {2} ] (\Delta t) ^ {2} \\ & = & 2 \Delta t \left(\sum_ {i} E [ c _ {i} ^ {2} ] \Delta t\right) \\ & = & O (\Delta t) \end{array}\tag{6.22}
$$

so that we have 

$$
E \left[ \left(\sum c _ {j} \Delta Z _ {j} ^ {2} - \sum_ {j} c _ {j} \Delta t\right) ^ {2} \right] = O (\Delta t)\tag{6.23}
$$

or 

$$
\lim _ {\Delta t \to 0} E \left[ \left(\sum c _ {j} \Delta Z _ {j} ^ {2} - \int_ {0} ^ {t} c (s, X (s)) d s\right) ^ {2} \right] = 0\tag{6.24}
$$

so that in this sense we can write 

$$
d Z ^ {2} \rightarrow d t; d t \rightarrow 0.\tag{6.25}
$$

## 7 Derivative Contracts on non-traded Assets and Real Options

The hedging arguments used in previous sections use the underlying asset to construct a hedging portfolio. What if the underlying asset cannot be bought and sold, or is non-storable? If the underlying variable is an interest rate, we can’t store this. Or if the underlying asset is bandwidth, we can’t store this either. However, we can get around this using the following approach. 

## 7.1 Derivative Contracts

Let the underlying variable follow 

$$
d S = a (S, t) d t + b (S, t) d Z,\tag{7.1}
$$

and let $F = F ( S , t )$ , so that from Ito’s Lemma 

$$
{ d F } { = } { \left[ a F _ { S } + \frac { b ^ { 2 } } { 2 } F _ { S S } + F _ { t } \right] d t + b F _ { S } d Z , }\tag{7.2}
$$

or in shorter form 

$$
\begin{array}{r c l} {d F} & = & {\mu d t + \sigma^ {*} d Z} \\ & & {\mu = a F _ {S} + \frac {b ^ {2}}{2} F _ {S S} + F _ {t}} \\ & & {\sigma^ {*} = b F _ {S}.} \end{array}\tag{7.3}
$$

Now, instead of hedging with the underlying asset, we will hedge one contract with another. Suppose we have two contracts $F _ { 1 } , F _ { 2 }$ (they could have diferent maturities for example). Then 

$$
\begin{array}{r c l} d F _ {1} & = & \mu_ {1} d t + \sigma_ {1} ^ {*} d Z \\ d F _ {2} & = & \mu_ {2} d t + \sigma_ {2} ^ {*} d Z \\ & & \mu_ {i} = a (F _ {i}) _ {S} + \frac {b ^ {2}}{2} (F _ {i}) _ {S S} + (F _ {i}) _ {t} \\ & & \sigma_ {i} ^ {*} = b (F _ {i}) _ {S}; i = 1, 2. \end{array}\tag{7.4}
$$

Consider the portfolio Π 

$$
\Pi = n _ {1} F _ {1} + n _ {2} F _ {2}\tag{7.5}
$$

so that 

$$
\begin{array}{r c l} {d \Pi} & = & {n _ {1} d F _ {1} + n _ {2} d F _ {2}} \\ & = & {n _ {1} (\mu_ {1} d t + \sigma_ {1} ^ {*} d Z) + n _ {2} (\mu_ {2} d t + \sigma_ {2} ^ {*} d Z)} \\ & = & {(n _ {1} \mu_ {1} + n _ {2} \mu_ {2}) d t + (n _ {1} \sigma_ {1} ^ {*} + n _ {2} \sigma_ {2} ^ {*}) d Z.} \end{array}\tag{7.6}
$$

Now, to eliminate risk, choose 

$$
(n _ {1} \sigma_ {1} ^ {*} + n _ {2} \sigma_ {2} ^ {*}) = 0\tag{7.7}
$$

which means that Π is riskless, hence 

$$
d \Pi = r \Pi d t,\tag{7.8}
$$

so that, using equations (7.6-7.8), we obtain 

$$
(n _ {1} \mu_ {1} + n _ {2} \mu_ {2}) = r (n _ {1} F _ {1} + n _ {2} F _ {2}).\tag{7.9}
$$

Putting together equations (7.7) and (7.9) gives 

$$
\left[ \begin{array}{c c} \sigma_ {1} ^ {*} & \sigma_ {2} ^ {*} \\ \mu_ {1} - r F _ {1} & \mu_ {2} - r F _ {2} \end{array} \right] \left[ \begin{array}{l} n _ {1} \\ n _ {2} \end{array} \right] = \left[ \begin{array}{l} 0 \\ 0 \end{array} \right].\tag{7.10}
$$

Now, equation (7.10) only has a nonzero solution if the two rows of equation (7.10) are linearly dependent. In other words, there must be a $\lambda _ { S } = \lambda _ { S } ( S , t )$ (independent of the type of contract) such that 

$$
\begin{array}{r c l} \mu_ {1} - r F _ {1} & = & \lambda_ {S} \sigma_ {1} ^ {*} \\ \mu_ {2} - r F _ {2} & = & \lambda_ {S} \sigma_ {2} ^ {*}. \end{array}\tag{7.11}
$$

Dropping the subscripts, we obtain 

$$
{\frac {\mu - r F}{\sigma^ {*}}} = {\lambda_ {S}}\tag{7.12}
$$

Substituting $\mu , \sigma ^ { * }$ from equations (7.3) into equation (7.12) gives 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {S} b) F _ {S} - r F = 0.\tag{7.13}
$$

Equation (7.13) is the PDE satisfied by a derivative contract on any asset S. Note that it does not matter if we cannot trade $S .$ 

Suppose that $F _ { 2 } = S$ is a traded asset. Then we can hedge with S, and from equation (7.11) we have 

$$
\mu_ {2} - r S = \lambda_ {S} \sigma_ {2} ^ {*}\tag{7.14}
$$

and from equations (7.1) and (7.3) we have 

$$
\begin{array}{r c l} \sigma_ {2} ^ {*} & = & b \\ \mu_ {2} & = & a \end{array}\tag{7.15}
$$

and ${ \mathrm { s o } } ,$ using equations (7.11) and (7.15) , we have that 

$$
\lambda_ {S} = \frac {a - r S}{b}\tag{7.16}
$$

and equation (7.13) reduces to 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + r S F _ {S} - r F = 0.\tag{7.17}
$$

Suppose 

$$
\begin{array}{r c l} \mu & = & F \mu^ {\prime} \\ \sigma^ {*} & = & F \sigma^ {\prime} \end{array}\tag{7.18}
$$

so that we can write 

$$
{ d F } { = } { F \mu ^ { \prime } d t + F \sigma ^ { \prime } d Z }\tag{7.19}
$$

then using equation (7.18) in equation (7.12) gives 

$$
\mu^ {\prime} = r + \lambda_ {S} \sigma^ {\prime}\tag{7.20}
$$

which has the convenient interpretation that the expected return on holding (not hedging) the derivative contract $F$ is the risk-free rate plus extra compensation due to the riskiness of holding $F .$ The extra return is $\lambda _ { S } \sigma ^ { \prime }$ , where $\lambda _ { S }$ is the market price of risk of $S$ (which should be the same for all contracts depending on S) and $\sigma ^ { \prime }$ is the volatility of $F .$ . Note that the volatility and drift of $F$ are not the volatility and drift of the underlying asset $S .$ 

If we believe that the Capital Asset Pricing Model holds, then a simple minded idea is to estimate 

$$
\lambda_ {S} = \rho_ {S M} \lambda_ {M}\tag{7.21}
$$

where $\lambda _ { M }$ is the price of risk of the market portfolio, and $\rho _ { S M }$ is the correlation of returns between $S$ and the returns of the market portfolio. 

Another idea is the following. Suppose we can find some companies whose main source of business is based on $S .$ Let $q _ { i }$ be the price of this companies stock at $t = t _ { i }$ . The return of the stock over $t _ { i } - t _ { i - 1 }$ is 

$$
R _ {i} = \frac {q _ {i} - q _ {i - 1}}{q _ {i - 1}}.
$$

Let $R _ { i } ^ { M }$ be the return of the market portfolio (i.e. a broad index) over the same period. We compute $\beta$ as the best fit linear regression to 

$$
R _ {i} = \alpha + \beta R _ {i} ^ {M}
$$

which means that 

$$
\beta = \frac {C o v (R , R ^ {M})}{V a r (R ^ {M})}.\tag{7.22}
$$

Now, from CAPM we have that 

$$
E (R) = r + \beta \left[ E (R ^ {M}) - r \right]\tag{7.23}
$$

where $E ( . . . )$ is the expectation operator. We would like to determine the unlevered $\beta ,$ denoted by $\beta ^ { u }$ , which is the $\beta$ for an investment made using equity only. In other words, if the firm we used to compute the $\beta$ above has significant debt, its riskiness with respect to S is amplified. The unlevered $\beta$ can be computed b 

$$
\beta^ {u} = \frac {E}{E + (1 - T _ {c}) D} \beta\tag{7.24}
$$

where 

$$
\begin{array}{r c l} D & = & \text {long term debt} \\ E & = & \text {Total market capitalization} \\ T _ {c} & = & \text {Corporate Tax rate .} \end{array}\tag{7.25}
$$

$\mathrm { S o } ,$ now the expected return from a pure equity investment based on $S$ is 

$$
E (R ^ {u}) = r + \beta^ {u} \left[ E (R ^ {M}) - r \right].\tag{7.26}
$$

If we assume that $F$ in equation (7.19) is the company stock, then 

$$
\begin{array}{r c l} \mu^ {\prime} & = & E (R ^ {u}) \\ & = & r + \beta^ {u} [ E (R ^ {M}) - r ] \end{array}\tag{7.27}
$$

But equation (7.20) says that 

$$
\mu^ {\prime} = r + \lambda_ {S} \sigma^ {\prime}.\tag{7.28}
$$

Combining equations (7.27-7.27) gives 

$$
\lambda_ {S} \sigma^ {\prime} = \beta^ {u} [ E (R ^ {M}) - r ].\tag{7.29}
$$

Recall from equations (7.3) and (7.18) that 

$$
\begin{array}{r c l} \sigma^ {*} & = & F \sigma^ {\prime} \\ \sigma^ {*} & = & b F _ {S}, \end{array}
$$

or 

$$
\sigma^ {\prime} = \frac {b F _ {S}}{F}.\tag{7.30}
$$

Combining equations (7.29-7.30) gives 

$$
\lambda_ {S} = \frac {\beta^ {u} [ E (R ^ {M}) - r ]}{\frac {b F _ {S}}{F}}.\tag{7.31}
$$

In principle, we can now compute $\lambda _ { S }$ , since 

• The unleveraged $\beta ^ { u }$ is computed as described above. This can be done using market data for a specific firm, whose main business is based on $S _ { ; }$ and the firms balance sheet. 

$b ( S , t ) / S$ is the volatility rate of S (equation (7.1)). 

$\left[ E ( R ^ { M } ) - r \right]$ can be determined from historical data. For example, the expected return of the market index above the risk free rate is about 6% for the past 50 years of Canadian data. 

• The risk free rate r is simply the current T-bill rate. 

$F _ { S }$ can be estimated by computing a linear regression of the stock price of a firm which invests in S, and S. Now, this may have to be unlevered, to reduce the efect of debt. If we are going to now value the real option for a specific firm, we will have to make some assumption about how the firm will finance a new investment. If it is going to use pure equity, then we are done. If it is a mixture of debt and equity, we should relever the value of $F _ { S }$ . At this point, we need to talk to a Finance Professor to get this right. 

## 7.2 A Forward Contract

A forward contract is a special type of derivative contract. The holder of a forward contract agrees to buy or sell the underlying asset at some delivery price K in the future. K is determined so that the cost of entering into the forward contract is zero at its inception. 

The payof of a (long) forward contract expiring at $t = T$ is then 

$$
V (S, \tau = 0) = S (T) - K.\tag{7.32}
$$

Note that there is no optionality in a forward contract. 

The value of a forward contract is a contingent claim. and its value is given by equation (7.13) 

$$
V _ {t} + \frac {b ^ {2}}{2} V _ {S S} + (a - \lambda_ {S} b) V _ {S} - r V = 0.\tag{7.33}
$$

Now we can also use a simple no-arbitrage argument to express the value of a forward contract in terms of the original delivery price $K$ , (which is set at the inception of the contract) and the current forward price $f ( S , \tau )$ . Suppose we are long a forward contract with delivery price K. At some time $t > 0 , ( \tau < T )$ , the forward price is no longer K. Suppose the forward price is $f ( S , \tau )$ , then the payof of a long forward contract, entered into at (τ ) is 

$$
\text { Payoff } = S (T) - f (S (\tau), \tau) .
$$

Suppose we are long the forward contract struck at $t = 0$ with delivery price K. At some time $t > 0 .$ , we hedge this contract by going short a forward with the current delivery price $f ( S , \tau )$ (which costs us nothing to enter into). The payof of this portfolio is 

$$
S - K - (S - f) = f - K\tag{7.34}
$$

Since $f , K$ are known with certainty at $( S , \tau )$ , then the value of this portfolio today is 

$$
(f - K) e ^ {- r \tau}.\tag{7.35}
$$

But if we hold a forward contract today, we can always construct the above hedge at no cost. Therefore, 

$$
V (S, \tau) = (f - K) e ^ {- r \tau}.\tag{7.36}
$$

Substituting equation (7.36) into equation (7.33), and noting that $K$ is a constant, gives us the following PDE for the forward price (the delivery price which makes the forward contract worth zero at inception) 

$$
f _ {\tau} = \frac {b ^ {2}}{2} f _ {S S} + (a - \lambda_ {S} b) f _ {S}\tag{7.37}
$$

with terminal condition 

$$
f (S, \tau = 0) = S\tag{7.38}
$$

which can be interpreted as the fact that the forward price must equal the spot price at $t = T$ 

Suppose we can estimate $a , b$ in equation (7.37), and there are a set of forward prices available. We can then estimate $\lambda _ { S }$ by solving equation (7.37) and adjusting $\lambda _ { S }$ until we obtain a good fit for the observed forward prices. 

## 7.2.1 Convenience Yield

We can also write equation (7.37) as 

$$
f _ {t} + \frac {b ^ {2}}{2} f _ {S S} + (r - \delta) S f _ {S} = 0\tag{7.39}
$$

where $\delta$ is defined as 

$$
\delta = r - \frac {a - \lambda_ {S} b}{S}.\tag{7.40}
$$

In this case, we can interpret $\delta$ as the convenience yield for holding the asset. For example, there is a convenience to holding supplies of natural gas in reserve. 

## 7.2.2 Volatility of Foward Prices

From equation (7.37) we have that the forward price for a contract expiring at time $T ,$ , at current time $t ,$ spot price $S ( t )$ is given by 

$$
f (S, t) = E ^ {Q} [ S (T) ]\tag{7.41}
$$

where S follows the risk neutral process 

$$
d S = (a - \lambda_ {S} b) d t + b d Z.\tag{7.42}
$$

In other words. the forward price is the risk neutral expected spot price at expiry. 

Now, using Ito’s Lemma and assuming the risk neutral spot process (7.42) gives 

$$
{ d f } { = } { \left( f _ { t } + \frac { b ^ { 2 } } { 2 } f _ { S S } + ( a - \lambda _ { S } b ) f _ { S } \right) d t + f _ { S } b d Z . }\tag{7.43}
$$

But since $f$ satisfies equation (7.37), equation (7.43) becomes 

$$
\begin{array}{r c l} d f & = & f _ {S} b d Z \\ & = & \hat {\sigma} f d Z, \end{array}\tag{7.44}
$$

where the efective volatility of the foward price is 

$$
\hat {\sigma} = \frac {f _ {S} b}{f}.\tag{7.45}
$$

Note that from equation (7.44), the forward price has zero drift. 

## 8 Discrete Hedging

In practice, we cannot hedge at infinitesimal time intervals. In fact, we would like to hedge as infrequently as possible, since in real life, there are transaction costs (something which is ignored in the basic Black-Scholes equation, but which can be taken into account and results in a nonlinear PDE). 

## 8.1 Delta Hedging

Recall that the basic derivation of the Black-Scholes equation used a hedging portfolio where we hold $V _ { S }$ shares. In finance, $V _ { S }$ is called the option delta, hence this strategy is called delta hedging. 

As an example, consider the hedging portfolio $P ( t )$ which is composed of 

• A short position in an option $- V ( t )$ 

• Long $\alpha ( t ) ^ { h } { S } ( t )$ shares 

• An amount in a risk-free bank account $B ( t )$ 

Initially, we have 

$$
\begin{array}{r c l} P (0) = 0 & = & - V (0) + \alpha (0) ^ {h} S (0) + B (0) \\ & & \alpha = V _ {S} \\ & & B (0) = V (0) - \alpha (0) ^ {h} S (0) \end{array}
$$

The hedge is rebalanced at discrete times $t _ { i }$ . Defining 

$$
\begin{array}{r c l} \alpha_ {i} ^ {h} & = & V _ {S} (S _ {i}, t _ {i}) \\ V _ {i} & = & V (S _ {i}, t _ {i}) \end{array}
$$

then, we have to update the hedge by purchasing $\alpha _ { i } - \alpha _ { i - 1 }$ shares at $t = t _ { i }$ , so that updating our share position requires 

$$
S (t _ {i}) (\alpha_ {i} ^ {h} - \alpha_ {i - 1} ^ {h})
$$

in cash, which we borrow from the bank if $\textstyle \left( \alpha _ { i } ^ { h } - \alpha _ { i - 1 } ^ { h } \right) > 0 . { \mathrm { ~ I f ~ } } ( \alpha _ { i } ^ { h } - \alpha _ { i - 1 } ^ { h } ) < 0$ , then we sell some shares and deposit the proceeds in the bank account. If $\Delta t = t _ { i } - t _ { i - 1 }$ , then the bank account balance is updated by 

$$
B _ {i} = e ^ {r \Delta t} B _ {i - 1} - S _ {i} (\alpha_ {i} ^ {h} - \alpha_ {i - 1} ^ {h})
$$

At the instant after the rebalancing time $t _ { i } ,$ the value of the portfolio is 

$$
P (t _ {i}) = - V (t _ {i}) + \alpha (t _ {i}) ^ {h} S (t _ {i}) + B (t _ {i})
$$

Since we are hedging at discrete time intervals, the hedge is no longer risk free (it is risk free only in the limit as the hedging interval goes to zero). We can determine the distribution of profit and loss $( { \mathrm { ~ P } } \& { { \mathrm { ~ L } } } )$ by carrying out a Monte Carlo simulation. Suppose we have precomputed the values of $V _ { S }$ for all the likely $( S , t )$ values. Then, we simulate a series of random paths. For each random path, we determine the discounted relative hedging error 

$$
{ e r r o r } { = } { \frac { e ^ { - r T ^ { * } } P ( T ^ { * } ) } { V ( S _ { 0 } , t = 0 ) } }\tag{8.1}
$$

After computing many sample paths, we can plot a histogram of relative hedging error, i.e. fraction of Monte Carlo trials giving a hedging error between E and $E { + } \Delta E$ . We can compute the variance of this distribution, and also the value at risk (VAR). VAR is the worst case loss with a given probability. For example, a typical VAR number reported is the maximum loss that would occur 95% of the time. In other words, find the value of E along the x-axis such that the area under the histogram plot to the right of this point is .95× the total area. 

As an example, consider the case of an American put option, $T = . 2 5 , \sigma = . 3 , r = . 0 6 , K = S _ { 0 } = 1 0 0 .$ . At $t = 0 , S _ { 0 } = 1 0 0$ . Since there are discrete hedging errors, the results in this case will depend on the stock drift rate, which we set at $\mu = . 0 8$ . The initial value of the American put, obtained by solving the Black-Scholes linear complementarity problem, is $5.34. Figure 8.1 shows the results for no hedging, and hedging once a month. The x-axis in these plots shows the relative P & L of this portfolio (i.e. P & L divided by the Black-Scholes price), and the y-axis shows the relative frequency. 

$$
\mathrm {Relative P\ & L} = \frac {\mathrm {Actual P\ & L}}{\mathrm{Black-Scholesprice}}\tag{8.2}
$$

Note that the no-hedging strategy actually has a high probability of ending up with a profit (from the option writer’s point of view) since the drift rate of the stock is positive. In this case, the hedger does nothing, but simply pockets the option premium. Note the sudden jump in the relative frequency at relative $P \& L = 1$ . This is because the maximum the option writer stands to gain is the option premium, which we assume is the Black-Scholes value. The writer makes this premium for any path which ends up $S > K$ which is many paths, hence the sudden jump in probability. However, there is significant probability of a loss as well. Figure 8.1 also shows the relative frequency of the P&L of hedging once a month (only three times during the life of the option). 

In fact, there is a history of Ponzi-like hedge funds which simply write put options with essentially no hedging. In this case, these funds will perform very well for several years, since markets tend to drift up on average. However, then a sudden market drop occurs, and they will blow up. Blowing up is a technical term for losing all your capital and being forced to get a real job. However, usually the owners of these hedge funds walk away with large bonuses, and the shareholders take all the losses. 

Figure 8.2 shows the results for rebalancing the hedge once a week, and daily. We can see clearly here that the mean is zero, and variance is getting smaller as the hedging interval is reduced. In fact, one can show that the standard deviation of the hedge error should be proportional to $\sqrt { \Delta t }$ where $\Delta t$ is the hedge rebalance frequency. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/7d55a67135ee7a8da0c109db3d519a8704708bcb21163ba146a8e9b277a6f229.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/04e8655392dd92d21e598cfe21ea10ee7eea381e4e21eb74e0ddb0cf9527cca1.jpg)



Figure 8.1: Relative frequency (y-axis) versus relative P&L of delta hedging strategies. Left: no hedging, right: rebalance hedge once a month. American put, $T = . 2 5 , \sigma = . 3 , r = . 0 6 , \mu = . 0 8 , K = S _ { 0 } = 1 0 0$ . The relative P&L is computed by dividing the actual P&L by the Black-Scholes price


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/bc2ad560e6c3aad344c66a7f01afe3177be6989c76fe649ca38216ab4fd6e05c.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/7722cefd2f2523872bb3b1341112f42d22de38d23516697fa3d85201e26b84bf.jpg)



Figure 8.2: Relative frequency (y-axis) versus relative P&L of delta hedging strategies. Left: rebalance hedge once a week, right: rebalance hedge daily. American put, $T = . 2 5 , \sigma = . 3 , r = . 0 6 , \mu = . 0 8 , K = S _ { 0 } = 1 0 0$ The relative P&L is computed by dividing the actual P&L by the Black-Scholes price.


## 8.2 Gamma Hedging

In an attempt to account for some the errors in delta hedging at finite hedging intervals, we can try to use second derivative information. The second derivative of an option value $V _ { S S }$ is called the option gamma, hence this strategy is termed delta-gamma hedging. 

A gamma hedge consists of 

• A short option position $- V ( t )$ 

• Long $\alpha ^ { h } S ( t )$ shares 

• Long $\beta$ another derivative security I. 

• An amount in a risk-free bank account $B ( t )$ 

Now, recall that we consider $\alpha ^ { h } , \beta$ to be constant over the hedging interval (no peeking into the future), so we can regard these as constants (for the duration of the hedging interval). 

The hedge portfolio $P ( t )$ is then 

$$
P (t) = - V + \alpha^ {h} S + \beta I + B (t)
$$

Assuming that we buy and hold $\alpha ^ { h }$ shares and $\beta$ of the secondary instrument at the beginning of each hedging interval, then we require that 

$$
\begin{array}{r c l} \frac {\partial P}{\partial S} & = & - \frac {\partial V}{\partial S} + \alpha^ {h} + \beta \frac {\partial I}{\partial S} = 0 \\ \frac {\partial^ {2} P}{\partial S ^ {2}} & = & - \frac {\partial^ {2} V}{\partial S ^ {2}} + \beta \frac {\partial^ {2} I}{\partial S ^ {2}} = 0 \end{array}\tag{8.3}
$$

Note that 

• If $\beta = 0$ , then we get back the usual delta hedge. 

• In order for the gamma hedge to work, we need an instrument which has some gamma (the asset S has second derivative zero). Hence, traders often speak of being long (positive) or short (negative) gamma, and try to buy/sell things to get gamma neutral. 

So, at $t = 0$ we have 

$$
{ P ( 0 ) } { = } { 0 \Rightarrow B ( 0 ) = V ( 0 ) - \alpha _ { 0 } ^ { h } S _ { 0 } - \beta _ { 0 } I _ { 0 } }
$$

The amounts $\alpha _ { i } ^ { h } , \beta _ { i }$ are determined by requiring that equation (8.3) hold 

$$
\begin{array}{r c l} {- (V _ {S}) _ {i} + \alpha_ {i} ^ {h} + \beta_ {i} (I _ {S}) _ {i}} & = & 0 \\ {- (V _ {S S}) _ {i} + \beta_ {i} (I _ {S S}) _ {i}} & = & 0 \end{array}\tag{8.4}
$$

The bank account balance is then updated at each hedging time $t _ { i }$ by 

$$
{B _ {i}} = {e ^ {r \Delta t} B _ {i - 1} - S _ {i} (\alpha_ {i} ^ {h} - \alpha_ {i - 1} ^ {h}) - I _ {i} (\beta_ {i} - \beta_ {i - 1})}
$$

We will consider the same example as we used in the delta hedge example. For an additional instrument, we will use a European put option written on the same underlying with the same strike price and a maturity of $\mathrm { T } { = } . 5$ years. 

Figure 8.3 shows the results of gamma hedging, along with a comparison on delta hedging. In principle, gamma hedging produces a smaller variance with less frequent hedging. However, we are exposed to more model error in this case, since we need to be able to compute the second derivative of the theoretical price. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/d53a3bd8ddb9ab4bc754dfd13a5015b87ed623bb9064be0b378a8c7b31eb9083.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/58a36c803faf8e9d34a0bd2895850df24a3e80f13ca803cb38cca01a0a1b84c9.jpg)



Figure 8.3: Relative frequency (y-axis) versus relative P&L of gamma hedging strategies. Left: rebalance hedge once a week, right: rebalance hedge daily. Dotted lines show the delta hedge for comparison. American put, $T = . 2 5 , \sigma = . 3 , r = . 0 6 , \mu = . 0 8 , K = 1 0 0 , S _ { 0 } = 1 0 0$ . Secondary instrument: European put option, same strike, $T = . 5$ years. The relative P&L is computed by dividing the actual P&L by the Black-Scholes price.


## 8.3 Vega Hedging

The most important parameter in the option pricing is the volatility. What if we are not sure about the value of the volatility? It is possible to assume that the volatility itself is stochastic, i.e. 

$$
\begin{array}{r c l} {d S} & = & {\mu S d t + \sqrt {v} S d Z _ {1}} \\ {d v} & = & {\kappa (\theta - v) d t + \sigma_ {v} \sqrt {v} d Z _ {2}} \end{array}\tag{8.5}
$$

where $\mu$ is the expected growth rate of the stock price, $\sqrt { v }$ is its instantaneous volatili $\mathrm { \Delta [ y , }$ κ is a parameter controlling how fast v reverts to its mean level of $\theta , \sigma _ { v }$ is the “volatility of volatility” parameter, and $Z _ { 1 } , Z _ { 2 }$ are Wiener processes with correlation parameter $\rho .$ 

If we use the model in equation (8.5), the this will result in a two factor PDE to solve for the option price and the hedging parameters. Since there are two sources of risk $( d Z _ { 1 } , d Z _ { 2 } )$ , we will need to hedge with the underlying asset and another option (Heston, A closed form solution for options with stochastic volatility with applications to bond and currency options, Rev. Fin. Studies 6 (1993) 327-343). 

Another possibility is to assume that the volatility is uncertain, and to assume that 

$$
\sigma_ {m i n} \leq \sigma \leq \sigma_ {m a x},
$$

and to hedge based on a worst case (from the hedger’s point of view). This results in an uncertain volatility model (Avellaneda, Levy, Paris, Pricing and Hedging Derivative Securities in Markets with Uncertain Volatilities, Appl. Math. Fin. 2 (1995) 77-88). This is great if you can get someone to buy this option at this price, because the hedger is always guaranteed to end up with a non-negative balance in the hedging portfolio. But you may not be able to sell at this price, since the option price is expensive (after all, the price you get has to cover the worst case scenario). 

An alternative, much simpler, approach (and therefore popular in industry), is to construct a vega hedge. We assume that we know the volatility, and price the option in the usual way. Then, as with a gamma hedge, we construct a portfolio 

• A short option position $- V ( t )$ 

• Long $\alpha ^ { h } S ( t )$ shares 

• Long $\beta$ another derivative security I. 

• An amount in a risk-free bank account $B ( t )$ 

The hedge portfolio $P ( t )$ is then 

$$
P (t) = - V + \alpha^ {h} S + \beta I + B (t)
$$

Assuming that we buy and hold $\alpha ^ { h }$ shares and $\beta$ of the secondary instrument at the beginning of each hedging interval, then we require that 

$$
\begin{array}{r c l} \frac {\partial P}{\partial S} & = & - \frac {\partial V}{\partial S} + \alpha^ {h} + \beta \frac {\partial I}{\partial S} = 0 \\ \frac {\partial P}{\partial \sigma} & = & - \frac {\partial V}{\partial \sigma} + \beta \frac {\partial I}{\partial \sigma} = 0 \end{array}\tag{8.6}
$$

Note that if we assume that $\sigma$ is constant when pricing the option, yet do not assume $\sigma$ is constant when we hedge, this is somewhat inconsistent. Nevertheless, we can determine the derivatives in equation (8.6) numerically (solve the pricing equation for several diferent values of $\sigma ,$ and then finite diference the solutions). 

In practice, we would sell the option priced using our best estimate of σ (today). This is usually based on looking at the prices of traded options, and then backing out the volatility which gives back today’s traded option price (this is the implied volatility). Then as time goes on, the implied volatility will likely change. We use the current implied volatility to determine the current hedge parameters in equation (8.6). Since this implied volatility has likely changed since we last rebalanced the hedge, there is some error in the hedge. However, taking into account the change in the hedge portfolio through equations (8.6) should make up fo this error. This procedure is called delta-vega hedging. 

In fact, even if the underlying process is a stochastic volatility, the vega hedge computed using a constant volatility model works surprisingly well (Hull and White, The pricing of options on assets with stochastic volatilities, J. of Finance, 42 (1987) 281-300). 

## 9 Jump Difusion

Recall that if 

$$
d S = \mu S d t + \sigma S d Z\tag{9.1}
$$

then from Ito’s Lemma we have 

$$
{d [ \log S ]} = {\left[ \mu - \frac {\sigma^ {2}}{2} \right] d t + \sigma d Z.}\tag{9.2}
$$

Now, suppose that we observe asset prices at discrete times $t _ { i } .$ , i.e. $S ( t _ { i } ) = S _ { i }$ , with $\Delta t = t _ { i + 1 } - t _ { i }$ . Then from equation (9.2) we have 

$$
\begin{array}{r c l} \log S _ {i + 1} - \log S _ {i} & = & \log (\frac {S _ {i + 1}}{S _ {i}}) \\ & \simeq & [ \mu - \frac {\sigma^ {2}}{2} ] \Delta t + \sigma \phi \sqrt {\Delta t} \end{array}\tag{9.3}
$$

where $\phi$ is $N ( 0 , 1 )$ . Now, if $\Delta t$ is suficiently small, then $\Delta t$ is much smaller than $\sqrt { \Delta t } .$ , so that equation (9.3) can be approximated by 

$$
\begin{array}{r c l} \log (\frac {S _ {i + 1} - S _ {i} + S _ {i}}{S _ {i}}) & = & \log (1 + \frac {S _ {i + 1} - S _ {i}}{S _ {i}}) \\ & \simeq & \sigma \phi \sqrt {\Delta t}. \end{array}\tag{9.4}
$$

Define the return $R _ { i }$ in the period $t _ { i + 1 } - t _ { i }$ as 

$$
R _ {i} = \frac {S _ {i + 1} - S _ {i}}{S _ {i}}\tag{9.5}
$$

so that equation (9.4) becomes 

$$
\log (1 + R _ {i}) \simeq R _ {i} = \sigma \phi \sqrt {\Delta t}.
$$

Consequently, a plot of the discretely observed returns of S should be normally distributed, if the assumption (9.1) is true. In Figure 9.1 we can see a histogram of monthly returns from the S&P500 for the period 1982 − 2002. The histogram has been scaled to zero mean and unit standard deviation. A standard normal distribution is also shown. Note that for real data, there is a higher peak, and fatter tails than the normal distribution. This means that there is higher probability of zero return, or a large gain or loss compared to a normal distribution. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/99a0ad8d7252a4759e168d46ceaa095264f6d1f0ab5b74c4f880ddc4d960082e.jpg)



Figure 9.1: Probability density functions for the S&P 500 monthly returns 1982 − 2002, scaled to zero mean and unit standard deviation and the standardized Normal distribution.


As $\Delta t \to 0 .$ , Geometric Brownian Motion (equation (9.1)) assumes that the probability of a large return also tends to zero. The amplitude of the return is proportional to $\sqrt { \Delta t } .$ , so that the tails of the distribution become unimportant. 

But, in real life, we can sometimes see very large returns (positive or negative) in small time increments. It therefore appears that Geometric Brownian Motion (GBM) is missing something important. 

## 9.1 The Poisson Process

Consider a process where most of the time nothing happens (contrast this with Brownian motion, where some changes occur at any time scale we look at), but on rare occasions, a jump occurs. The jump size does not depend on the time interval, but the probability of the jump occurring does depend on the interval. 

More formally, consider the process dq where, in the interval $[ t , t + d t ]$ , 

$$
\begin{array}{r c l} d q & = & 1; \quad \text {with probability} \lambda d t \\ & = & 0; \quad \text {with probability} 1 - \lambda d t. \end{array}\tag{9.6}
$$

Note, once again, that size of the Poisson outcome does not depend on dt. Also, the probability of a jump occurring in $[ t , t + d t ]$ goes to zero as $d t \to 0 .$ in contrast to Brownian motion, where some movement always takes place (the probability of movement is constant as $d t \to 0 )$ , but the size of the movement tends to zero as $d t \to 0$ . For future reference, note that 

$$
\begin{array}{r c l} {E [ d q ]} & = & {\lambda d t \cdot 1 + (1 - \lambda d t) \cdot 0} \\ & = & {\lambda d t} \end{array}\tag{9.7}
$$

and 

$$
\begin{array}{r c l} V a r (d q) & = & E [ (d q - E [ d q ]) ^ {2} ] \\ & = & E [ (d q - \lambda d t) ^ {2} ] \\ & = & (1 - \lambda d t) ^ {2} \cdot \lambda d t + (0 - \lambda d t) ^ {2} \cdot (1 - \lambda d t) \\ & = & \lambda d t + O ((d t) ^ {2}). \end{array}\tag{9.8}
$$

Now, suppose we assume that, along with the usual GBM, occasionally the asset jumps, i.e. $S \to J S$ where J is the size of a (proportional) jump. We will restrict J to be non-negative. 

Suppose a jump occurs in $[ t , t + d t ]$ , with probability λdt. Let’s write this jump process as an SDE, i.e. 

$$
{[ d S ] _ {j u m p}} {= (J - 1) S d q}
$$

since, if a jump occurs 

$$
\begin{array}{r c l} {S _ {a f t e r j u m p}} & = & {S _ {b e f o r e j u m p} + [ d S ] _ {j u m p}} \\ & = & {S _ {b e f o r e j u m p} + (J - 1) S _ {b e f o r e j u m p}} \\ & = & {J S _ {b e f o r e j u m p}} \end{array}\tag{9.9}
$$

which is what we want to model. So, if we have a combination of GBM and a rare jump event, then 

$$
{ d S } { = } { \mu S ~ d t + \sigma S ~ d Z + ( J - 1 ) S ~ d q }\tag{9.10}
$$

Assume that the jump size has some known probability density $g ( J )$ , i.e. given that a jump occurs, then the probability of a jump in $[ J , J + d J ]$ is $g ( J )$ dJ, and 

$$
\int_ {- \infty} ^ {+ \infty} g (J) d J = \int_ {0} ^ {\infty} g (J) d J = 1\tag{9.11}
$$

since we assume that $g ( J ) = 0 { \mathrm { ~ i f ~ } } J < 0$ . For future reference, if $f = f ( J )$ , then the expected value of $f$ is 

$$
E [ f ] = \int_ {0} ^ {\infty} f (J) g (J) d J.\tag{9.12}
$$

The process (9.10) is basically geometric Brownian motion (a continuous process) with rare discontinuous jumps. Some example realizations of jump difusion paths are shown in Figure 9.2. 

Figure 9.3 shows the price followed by a listed drug company. Note the extreme price changes over very small periods of time. 

## 9.2 The Jump Difusion Pricing Equation

Now, form the usual hedging portfolio 

$$
P = V - \alpha S.\tag{9.13}
$$

Now, consider 

$$
{[ d P ] _ {t o t a l}} = {[ d P ] _ {B r o w n i a n} + [ d P ] _ {j u m p}}\tag{9.14}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/69ddfc906e02ad8c0ecc3d8225283ddf6673729c8162bd13e592d1cf8befb866.jpg)



Figure 9.2: Some realizations of a jump difusion process which follows equation (9.10).


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/65d3906cd30eea32e14ffc9d6090b50dbd27c82448789617496e289023812802.jpg)



Figure 9.3: Actual price of a drug company stock. Compare with simulation of a jump difusion in Figure 9.2.


where, from Ito’s Lemma 

$$
{[ d P ] _ {B r o w n i a n}} = {[ V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} ] d t + [ V _ {S} - \alpha S ] (\mu S d t + \sigma S d Z)}\tag{9.15}
$$

and, noting that the jump is of finite size, 

$$
{[ d P ] _ {j u m p}} = {[ V (J S, t) - V (S, t) ] d q - \alpha (J - 1) S d q.}\tag{9.16}
$$

If we hedge the Brownian motion risk, by setting $\alpha = V _ { S }$ , then equations (9.14-9.16) give us 

$$
{ d P } { = } { [ V _ { t } + \frac { \sigma ^ { 2 } S ^ { 2 } } { 2 } V _ { S S } ] d t + [ V ( J S , t ) - V ( S , t ) ] d q - V _ { S } ( J - 1 ) S ~ d q ~ . }\tag{9.17}
$$

So, we still have a random component $( d q )$ which we have not hedged away. Let’s take the expected value of this change in the portfolio, e.g. 

$$
{ E ( d P ) } { = } { [ V _ { t } + \frac { \sigma ^ { 2 } S ^ { 2 } } { 2 } V _ { S S } ] d t + E [ V ( J S , t ) - V ( S , t ) ] E [ d q ] - V _ { S } S E [ J - 1 ] E [ d q ] }\tag{9.18}
$$

where we have assumed that probability of the jump and the probability of the size of the jump are independent. Defining $E ( J - 1 ) = \kappa ,$ then we have that equation (9.18) becomes 

$$
{ E ( d P ) } { = } { [ V _ { t } + \frac { \sigma ^ { 2 } S ^ { 2 } } { 2 } V _ { S S } ] d t + E [ V ( J S , t ) - V ( S , t ) ] \lambda d t - V _ { S } S \kappa \lambda d t . }\tag{9.19}
$$

Now, we make a rather interesting assumption. Assume that an investor holds a diversified portfolio of these hedging portfolios, for many diferent stocks. If we make the rather dubious assumption that these jumps for diferent stocks are uncorrelated, then the variance of this portfolio of portfolios is small, hence there is little risk in this portfolio. Hence, the expected return should be 

$$
E [ d P ] = r P d t.\tag{9.20}
$$

Now, equating equations (9.19 and (9.20) gives 

$$
V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + V _ {S} [ r S - S \kappa \lambda ] - (r + \lambda) V + E [ V (J S, t) ] \lambda = 0.\tag{9.21}
$$

Using equation (9.12) in equation (9.21) gives 

$$
V _ {t} + \frac {\sigma^ {2} S ^ {2}}{2} V _ {S S} + V _ {S} [ r S - S \kappa \lambda ] - (r + \lambda) V + \lambda \int_ {0} ^ {\infty} g (J) V (J S, t) d J = 0.\tag{9.22}
$$

Equation (9.22) is a Partial Integral Diferential Equation (PIDE). 

A common assumption is to assume that $g ( J )$ is log normal, 

$$
g (J) = \frac {\exp \left(- \frac {(\log (J) - \hat {\mu}) ^ {2}}{2 \gamma^ {2}}\right)}{\sqrt {2 \pi} \gamma J}.\tag{9.23}
$$

where, some algebra shows that 

$$
E (J - 1) = \kappa = \exp (\hat {\mu} + \gamma^ {2} / 2) - 1.\tag{9.24}
$$

Now, what about our dubious assumption that jump risk was diversifiable? In practice, we can regard $\sigma , \hat { \mu } , \gamma , \lambda$ as parameters, and fit them to observed option prices. If we do this, (see L. Andersen and J. Andreasen, Jump-Difusion processes: Volatility smile fitting and numerical methods, Review of Derivatives Research (2002), vol 4, pages 231-262), then we find that σ is close to historical volatility, but that the fitted values of $\lambda , \hat { \mu }$ are at odds with the historical values. The fitted values seem to indicate that investors are pricing in larger more frequent jumps than has been historically observed. In other words, actual prices seem to indicate that investors do require some compensation for jump risk, which makes sense. In other words, these parameters contain a market price of risk. 

Consequently, our assumption about jump risk being diversifiable is not really a problem if we fit the jump parameters from market (as opposed to historical) data, since the market-fit parameters will contain some efect due to risk preferences of investors. 

One can be more rigorous about this if you assume some utility function for investors. See (Alan Lewis, Fear of jumps, Wilmott Magazine, December, 2002, pages 60-67) or (V. Naik, M. Lee, General equilibrium pricing of options on the market portfolio with discontinuous returns, The Review of Financial Studies, vol 3 (1990) pages 493-521.) 

## 9.3 An Alternate Derivation of the Pricing Equation for Jump Difusion

We will give a pure hedging argument in this section, in order to derive the PIDE for jump difusion. Initially, we suppose that there is only one possible jump size $J ,$ i.e. after a jump, $S  J S$ , where J is a known constant. Suppose 

$$
{ d S } { = } { a ( S , t ) d t + b ( S , t ) d Z + ( J - 1 ) S ~ d q , }\tag{9.25}
$$

where $d q$ is the Poisson process. Consider a contract on $S , F ( S , t )$ , then 

$$
d F = \left[ a F _ {S} + \frac {b ^ {2}}{2} F _ {S S} + F _ {t} \right] d t + b F _ {S} d Z + [ F (J S, t) - F (S, t) ] d q,\tag{9.26}
$$

or, in more compact notation 

$$
\begin{array}{r c l} {d F} & = & {\mu d t + \sigma^ {*} d Z + \Delta F d q} \\ & & {\mu = a F _ {S} + \frac {b ^ {2}}{2} F _ {S S} + F _ {t}} \\ & & {\sigma^ {*} = b F _ {S}} \\ & & {\Delta F = [ F (J S, t) - F (S, t) ] .} \end{array}\tag{9.27}
$$

Now, instead of hedging with the underlying asset, we will hedge one contract with another. Suppose we have three contracts $F _ { 1 } , F _ { 2 } , F _ { 3 }$ (they could have diferent maturities for example). 

Consider the portfolio Π 

$$
\Pi = n _ {1} F _ {1} + n _ {2} F _ {2} + n _ {3} F _ {3}\tag{9.28}
$$

so that 

$$
\begin{array}{r c l} d \Pi & = & n _ {1} d F _ {1} + n _ {2} d F _ {2} + n _ {3} d F _ {3} \\ & = & n _ {1} (\mu_ {1} d t + \sigma_ {1} ^ {*} d Z + \Delta F _ {1} d q) \\ & & + n _ {2} (\mu_ {2} d t + \sigma_ {2} ^ {*} d Z + \Delta F _ {2} d q) \\ & & + n _ {3} (\mu_ {3} d t + \sigma_ {3} ^ {*} d Z + \Delta F _ {3} d q) \\ & = & (n _ {1} \mu_ {1} + n _ {2} \mu_ {2} + n _ {3} \mu_ {3}) d t \\ & & + (n _ {1} \sigma_ {1} ^ {*} + n _ {2} \sigma_ {2} ^ {*} + n _ {3} \sigma_ {3} ^ {*}) d Z \\ & & + (n _ {1} \Delta F _ {1} + n _ {2} \Delta F _ {2} + n _ {3} \Delta F _ {3}) d q. \end{array}\tag{9.29}
$$

Eliminate the random terms by setting 

$$
\begin{array}{r c l} (n _ {1} \Delta F _ {1} + n _ {2} \Delta F _ {2} + n _ {3} \Delta F _ {3}) & = & 0 \\ (n _ {1} \sigma_ {1} ^ {*} + n _ {2} \sigma_ {2} ^ {*} + n _ {3} \sigma_ {3} ^ {*}) & = & 0. \end{array}\tag{9.30}
$$

This means that the portfolio is riskless, hence 

$$
d \Pi = r \Pi d t,\tag{9.31}
$$

hence (using equations (9.29-9.31)) 

$$
{(n _ {1} \mu_ {1} + n _ {2} \mu_ {2} + n _ {3} \mu_ {3})} = {(n _ {1} F _ {1} + n _ {2} F _ {2} + n _ {3} F _ {3}) r .}\tag{9.32}
$$

Putting together equations (9.30) and (9.32), we obtain 

$$
\left[ \begin{array}{c c c} \sigma_ {1} ^ {*} & \sigma_ {2} ^ {*} & \sigma_ {3} ^ {*} \\ \Delta F _ {1} & \Delta F _ {2} & \Delta F _ {3} \\ \mu_ {1} - r F _ {1} & \mu_ {2} - r F _ {2} & \mu_ {3} - r F _ {3} \end{array} \right] \left[ \begin{array}{l} n _ {1} \\ n _ {2} \\ n _ {3} \end{array} \right] = \left[ \begin{array}{l} 0 \\ 0 \\ 0 \end{array} \right].\tag{9.33}
$$

Equation (9.33) has a nonzero solution only if the rows are linearly dependent. There must be $\lambda _ { B } ( S , t ) , \lambda _ { J } ( S , t )$ such that 

$$
\begin{array}{r c l} {(\mu_ {1} - r F _ {1})} & = & {\lambda_ {B} \sigma_ {1} ^ {*} - \lambda_ {J} \Delta F _ {1}} \\ {(\mu_ {2} - r F _ {2})} & = & {\lambda_ {B} \sigma_ {2} ^ {*} - \lambda_ {J} \Delta F _ {2}} \\ {(\mu_ {3} - r F _ {3})} & = & {\lambda_ {B} \sigma_ {3} ^ {*} - \lambda_ {J} \Delta F _ {3}.} \end{array}\tag{9.34}
$$

(We will show later on that $\lambda _ { J } \geq 0$ to avoid arbitrage). Dropping subscripts, we have 

$$
(\mu - r F) = \lambda_ {B} \sigma^ {*} - \lambda_ {J} \Delta F\tag{9.35}
$$

and substituting the definitions of $\mu , \sigma ^ { * } , \Delta F$ , from equations (9.27), we obtain 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} b) F _ {S} - r F + \lambda_ {J} [ F (J S, t) - F (S, t) ] = 0.\tag{9.36}
$$

Note that $\lambda _ { J }$ will not be the real world intensity of the Poisson process, but J will be the real world jump size. 

In the event that, say, $F _ { 3 } = S$ is a traded asset, we note that in this case 

$$
\begin{array}{r c l} \sigma_ {3} ^ {*} & = & b \\ \mu_ {3} & = & a \\ \Delta F _ {3} & = & (J - 1) S. \end{array}\tag{9.37}
$$

From equation (9.34) we have that 

$$
\left(\mu_ {3} - r F _ {3}\right) = \lambda_ {B} \sigma_ {3} ^ {*} - \lambda_ {J} \Delta F _ {3},\tag{9.38}
$$

or, using equation (9.37), 

$$
a - \lambda_ {B} b = r S - \lambda_ {J} (J - 1) S.\tag{9.39}
$$

Substituting equation (9.39) into equation (9.36) gives 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + [ r - \lambda_ {J} (J - 1) ] S F _ {S} - r F + \lambda_ {J} [ F (J S, t) - F (S, t) ] = 0.\tag{9.40}
$$

Note that equation (9.36) is valid if the underlying asset cannot be used to hedge, while equation (9.40) is valid only if the underlying asset can be used as part of the hedging portfolio. 

Let $\tau = T - t .$ and set $a = 0 , b = 0 , r = 0$ in equation (9.36), giving 

$$
{F _ {\tau}} = {\lambda_ {J} [ F (J S, t) - F (S, t) ] .}\tag{9.41}
$$

Now, suppose that 

$$
\begin{array}{r c l} F (S, \tau = 0) & = & 0    ; \quad \text { if }   S \geq K \\ & = & 1    ; \quad \text { if }   S <   K    . \end{array}\tag{9.42}
$$

Now, consider the asset value $S ^ { * } > K$ , and let $J = K / ( 2 * S ^ { * } )$ . Imagine solving equation (9.41) to an infinitesimal time $\tau = \epsilon \ll 1$ . We will obtain the following value for $F .$ 

$$
F (S ^ {*}, \epsilon) \simeq \epsilon \lambda_ {J}.\tag{9.43}
$$

Since the payof is nonnegative, we must have $\lambda _ { J } \geq 0$ to avoid arbitrage. 

Now, suppose that there are a finite number of jump states, i.e. after a jump, the asset may jump to to any state $J _ { i } S$ 

$$
S \rightarrow J _ {i} S; i = 1, \dots , n.\tag{9.44}
$$

Repeating the above arguments, now using $n + 2$ hedging instruments in the hedging portfolio 

$$
\Pi = \sum_ {i = 1} ^ {i = n + 2} n _ {i} F _ {i}\tag{9.45}
$$

so that the difusion and jumps are hedged perfectly, we obtain the following PDE 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} b) F _ {S} - r F + \sum_ {i = 1} ^ {i = n} \lambda_ {J} ^ {i} [ F (J _ {i} S, t) - F (S, t) ] = 0.\tag{9.46}
$$

If we can use the underlying to hedge, then we get the analogue of equation (9.40) 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (r S - \sum_ {i = 1} ^ {i = n} \lambda_ {J} ^ {i} S (J _ {i} - 1)) F _ {S} - r F + \sum_ {i = 1} ^ {i = n} \lambda_ {J} ^ {i} [ F (J _ {i} S, t) - F (S, t) ] = 0.\tag{9.47}
$$

Now, let 

$$
{p (J _ {i})} = {\frac {\lambda_ {J} ^ {i}}{\sum_ {i = 1} ^ {i = n} \lambda_ {J} ^ {i}}}
$$

$$
\lambda^ {*} = \sum_ {i = 1} ^ {i = n} \lambda_ {J} ^ {i}\tag{9.48}
$$

then we can write equation (9.46) as 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} b) F _ {S} - r F + \lambda^ {*} \sum_ {i = 1} ^ {i = n} p (J _ {i}) [ F (J _ {i} S, t) - F (S, t) ] = 0.\tag{9.49}
$$

Note that since $\lambda _ { J } ^ { i } \ge 0 , p ( J _ { i } ) \ge 0$ , and $\lambda ^ { * } \geq 0 .$ 

Taking the limit as the number of jump states tends to infinity, then $p ( J )$ tends to a continuous distri bution, so that equation (9.49) becomes 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} b) F _ {S} - r F + \lambda^ {*} \int_ {0} ^ {\infty} p (J) [ F (J S, t) - F (S, t) ] d J = 0.\tag{9.50}
$$

It is convenient to rewrite equation (9.50) in a slightly diferent form. Suppose we redefine $\lambda _ { B }$ as follows 

$$
\lambda_ {B} = \lambda_ {B} ^ {\prime} + \lambda^ {*} \frac {E [ J - 1 ] S}{b}\tag{9.51}
$$

where 

$$
E [ J - 1 ] = \int_ {0} ^ {\infty} p (J) (J - 1) d J.\tag{9.52}
$$

Substituting equation (9.51) into equation (9.50) gives 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} ^ {\prime} b - \lambda^ {*} E [ J - 1 ] S) F _ {S} - r F + \lambda^ {*} \int_ {0} ^ {\infty} p (J) [ F (J S, t) - F (S, t) ] d J = 0.\tag{9.53}
$$

Note that in the case that $V _ { S S } = 0$ (which would normally be the case for $S \to \infty )$ , then equation (9.53) reduces to 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} b) F _ {S} - r F = 0,\tag{9.54}
$$

so that the term $\lambda ^ { * } E [ J - 1 ] S$ in the drift term cancels the integral term, leaving the equation independent of $\lambda ^ { * }$ . This is very convenient for applying numerical boundary conditions. The PIDE (9.53) can also be written as 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} ^ {\prime} b) F _ {S} - r F + \lambda^ {*} \int_ {0} ^ {\infty} p [ J ] [ F (J S, t) - F (S, t) - (J - 1) S F _ {S} ] d J = 0\tag{9.55}
$$

which is valid for infinite activity processes. 

In the case where we can hedge with the underlying asset $S ,$ we obtain 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (r - \lambda^ {*} E [ J - 1 ]) S F _ {S} - r F + \lambda^ {*} \int_ {0} ^ {\infty} p (J) [ F (J S, t) - F (S, t) ] d J = 0.\tag{9.56}
$$

Note that $\lambda ^ { * }$ and $p ( J )$ are not the real arrival rate and real jump size distributions, since they are based on hedging arguments which eliminate the risk. Consequently, $\lambda ^ { * } , p ( J )$ must be obtained by calibration to market data. 

## 10 Regime Switching

Of course, volatility is not constant in the real world. It is possible to combine jumps in the asset price with jumps in volatility and stochastic volatility. This leads to a two factor pricing PIDE for the option price. 

A simpler approach is to assume that the volatility jumps between a number of regimes or volatility states. Let the value of a contingent claim be given by $F ( \sigma , S , t )$ , where we have allowed the volatility σ to vary. Suppose 

$$
\begin{array}{r c l} {d S} & = & {a d t + b d Z + (J _ {S} - 1) S d q} \\ {d \sigma} & = & {(J _ {\sigma} - 1) \sigma d q ,} \end{array}\tag{10.1}
$$

where $d q$ is a Poisson process and $d Z$ is the increment of a Weiner process. Note that the same $d q$ drives the jump in $S$ and the jump in $\sigma .$ Following the same steps as in deriving equation (9.27) we obtain 

$$
\begin{array}{r c l} {d F} & = & {\mu d t + \sigma^ {*} d Z + \Delta F d q} \\ & & {\mu = a F _ {S} + \frac {b ^ {2}}{2} F _ {S S} + F _ {t}} \\ & & {\sigma^ {*} = b F _ {S}} \\ & & {\Delta F = [ F (J _ {\sigma} \sigma , J _ {S} S, t) - F (\sigma , S, t) ].} \end{array}\tag{10.2}
$$

We follow the same steps as in the derivation of the jump difusion PIDE in equations (9.29-9.36), i.e. we construct a hedge portfolio with three contracts $F _ { 1 } , F _ { 2 } , F _ { 3 }$ and we do not assume that we can trade in the underlying. Eliminating the random terms gives rise to the analogue of equation (9.33) and hence a solution exists only if one of the equations is a linear combination of the other equations, which results in 

$$
(\mu - r F) = \lambda_ {B} \sigma^ {*} - \lambda_ {J} \Delta F\tag{10.3}
$$

and substituting the definitions of $\sigma ^ { * } , \mu$ from equation (10.2) gives 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} b) F _ {S} - r F + \lambda_ {J} [ F (J _ {\sigma} \sigma , J _ {S} S, t) - F (\sigma , S, t) ] = 0.\tag{10.4}
$$

In the event that, say, $F _ { 3 } = S$ is a traded asset, we note that in this case 

$$
\begin{array}{r c l} \sigma_ {3} ^ {*} & = & b \\ \mu_ {3} & = & a \\ \Delta F _ {3} & = & (J _ {S} - 1) S. \end{array}\tag{10.5}
$$

Substituting equation (10.5) into equation (10.3) gives 

$$
a - \lambda_ {B} b = r S - \lambda_ {J} (J _ {S} - 1) S.\tag{10.6}
$$

Substituting equation (10.6) into equation (10.4) gives 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + [ r - \lambda_ {J} (J _ {S} - 1) ] S F _ {S} - r F + \lambda_ {J} [ F (J _ {\sigma} \sigma , J _ {S} S, t) - F (\sigma , S, t) ] = 0.\tag{10.7}
$$

Note that if $J _ { S } = 1$ (no jump in $S ,$ but a regime switch) then the term $\lambda _ { J } ( J _ { S } - 1 )$ disappears in the drift term. 

We can repeat the above arguments with jumps from a given regime with volatility σ to several possible regimes $J _ { \sigma } ^ { i } \sigma , i = 1 , \ldots , p$ . Each possible transition $\sigma \to J _ { \sigma } ^ { i } \sigma$ is driven by a Poisson process $d q ^ { i }$ . We assume that $d q ^ { i }$ and $d q ^ { j }$ are independent. In this case, we have 

$$
d S = a d t + b d Z + \sum_ {i = 1} ^ {i = p} (J _ {S} ^ {i} - 1) S d q ^ {i}
$$

$$
{d \sigma} = {\sum_ {i = 1} ^ {i = p} (J _ {\sigma} - 1) \sigma d q ^ {i},}\tag{10.8}
$$

Following the by now familiar steps, we obtain 

$$
F _ {t} + \frac {b ^ {2}}{2} F _ {S S} + (a - \lambda_ {B} b) F _ {S} - r F + \sum_ {i} \lambda_ {J} ^ {i} [ F (J _ {\sigma} ^ {i} \sigma , J _ {S} ^ {i} S, t) - F (\sigma , S, t) ] = 0.\tag{10.9}
$$

Note that in general $\lambda _ { J } ^ { i } = \lambda _ { J } ^ { i } ( \sigma , S ) , J _ { \sigma } ^ { i } = J _ { \sigma } ^ { i } ( \sigma , S ) , J _ { S } ^ { i } = J _ { S } ^ { i } ( \sigma , S )$ , and $\lambda _ { B } = \lambda _ { B } ( \sigma , S )$ . Now, suppose we have only a finite number of possible regimes $\sigma _ { k } , k = 1 , \dotsc , p .$ Let 

$$
\begin{array}{r c l} \lambda_ {B} ^ {k} (\sigma_ {k}, S) & = & \lambda_ {B} ^ {k} (S)) \\ F (\sigma_ {k}, S, t) & = & F ^ {k} (S, t) \\ \lambda_ {J} ^ {i} (\sigma_ {k}, S, t) & = & \lambda_ {J} ^ {k \to i} \\ J _ {\sigma} ^ {i} (\sigma_ {k}, S, t) & = & J _ {\sigma} ^ {k \to i} \\ J _ {S} ^ {i} (\sigma_ {k}, S, t) & = & J _ {S} ^ {k \to i}. \end{array}\tag{10.10}
$$

Rewriting equation (10.9) using equation (10.10) gives 

$$
F _ {t} ^ {k} + \frac {b _ {k} ^ {2}}{2} F _ {S S} ^ {k} + (a _ {k} - \lambda_ {B} ^ {k} b _ {k}) F _ {S} ^ {k} - r F ^ {k} + \sum_ {i} \lambda_ {J} ^ {k \rightarrow i} [ F ^ {i} (J _ {S} ^ {k \rightarrow i} S, t) - F ^ {k} (S, t) ] = 0.\tag{10.11}
$$

If we can hedge with the underlying, then the usual arguments give 

$$
a _ {k} - \lambda_ {B} ^ {k} b _ {k} = r S - \sum_ {i} \lambda_ {J} ^ {k \rightarrow i} (J _ {S} ^ {k \rightarrow i} - 1) S.\tag{10.12}
$$

Substituting equation (10.12) into equation (10.11) gives 

$$
F _ {t} ^ {k} + \frac {b _ {k} ^ {2}}{2} F _ {S S} ^ {k} + (r - \sum_ {i} \lambda_ {J} ^ {k \rightarrow i} (J _ {S} ^ {k \rightarrow i} - 1)) S F _ {S} ^ {k} - r F ^ {k} + \sum_ {i} \lambda_ {J} ^ {k \rightarrow i} [ F ^ {i} (J _ {S} ^ {k \rightarrow i} S, t) - F ^ {k} (S, t) ] = 0.\tag{10.13}
$$

If we have only a small number of regimes, we are efectively solving a small number of coupled 1-d PDEs. In principle, the $J _ { S } ^ { k \to i } , \sigma _ { k }$ are P measure parameters, while the $\lambda _ { J } ^ { k  i }$ is a $Q$ measure parameter. We can also determine the $\sigma _ { k } , \overset { \sim } { J _ { S } ^ { k \to i } } , \lambda _ { J } ^ { k \to i }$ by calibration to market prices. 

## 11 Mean Variance Portfolio Optimization

An introduction to Computational Finance would not be complete without some discussion of Portfolio Optimization. Consider a risky asset which follows Geometric Brownian Motion with drift 

$$
{\frac {d S}{S}} = {\mu d t + \sigma d Z ,}\tag{11.1}
$$

where as usual $d Z = \phi { \sqrt { d t } }$ and $\phi \sim N ( 0 , 1 )$ . Suppose we consider a fixed finite interval $\Delta t ,$ then we can write equation (11.1) as 

$$
\begin{array}{r c l} R & = & \mu^ {\prime} + \sigma^ {\prime} \phi \\ & & R = \frac {\Delta S}{S} \\ & & \mu^ {\prime} = \mu \Delta t \\ & & \sigma^ {\prime} = \sigma \sqrt {\Delta t}, \end{array}\tag{11.2}
$$

where R is the actual return on the asset in $[ t , t + \Delta t ] , \mu ^ { \prime }$ is the expected return on the asset in $[ t , t + \Delta t ]$ and $\sigma ^ { \prime }$ is the standard deviation of the return on the asset in $[ t , t + \Delta t ]$ 

Now consider a portfolio of N risky assets. Let $R ^ { i }$ be the return on asset i in $[ t , t + \Delta t ]$ , so that 

$$
{R ^ {i}} = {\mu_ {i} ^ {\prime} + \sigma_ {i} ^ {\prime} \phi_ {i}}\tag{11.3}
$$

Suppose that the correlation between asset i and asset j is given by $\rho _ { i j } = E [ \phi _ { i } \phi _ { j } ]$ . Suppose we buy $x _ { i }$ of each asset at t, to form the portfolio P 

$$
P = \sum_ {i = 1} ^ {i = N} x _ {i} S _ {i}.\tag{11.4}
$$

Then, over the interval $[ t , t + \Delta t ]$ 

$$
\begin{array}{r c l} P + \Delta P & = & \sum_ {i = 1} ^ {i = N} x _ {i} S _ {i} (1 + R ^ {i}) \\ \Delta P & = & \sum_ {i = 1} ^ {i = N} x _ {i} S _ {i} R ^ {i} \\ \frac {\Delta P}{P} & = & \sum_ {i = 1} ^ {i = N} w _ {i} R ^ {i} \\ & & w _ {i} = \frac {x _ {i} S _ {i}}{\sum_ {j = 1} ^ {j = N} x _ {j} S _ {j}} \end{array}\tag{11.5}
$$

In other words, we divide up our total wealth $\begin{array} { r } { W = \sum _ { i = 1 } ^ { i = N } x _ { i } S _ { i } } \end{array}$ into each asset with weight $w _ { i }$ . Note that $\begin{array} { r } { \sum _ { i = 1 } ^ { i = N } w _ { i } = 1 } \end{array}$ 

To summarize, given some initial wealth at t, we suppose that an investor allocates a fraction $w _ { i }$ of this wealth to each asset i. We assume that the total wealth is allocated to this risky portfolio $P ,$ so that 

$$
\begin{array}{r c l} \sum_ {i = 1} ^ {i = N} w _ {i} & = & 1 \\ P & = & \sum_ {i = 1} ^ {i = N} x _ {i} S _ {i} \\ R _ {p} = \frac {\Delta P}{P} & = & \sum_ {i = 1} ^ {i = N} w _ {i} R ^ {i}. \end{array}\tag{11.6}
$$

The expected return on this portfolio $\overline { { R _ { p } } }$ in $[ t , t + \Delta t ]$ is 

$$
\overline {{R _ {p}}} = \sum_ {i = 1} ^ {i = N} w _ {i} \mu_ {i} ^ {\prime},\tag{11.7}
$$

while the variance of $R _ { p }$ in $[ t , t + \Delta t ]$ is 

$$
{V a r (R _ {p})} = {\sum_ {i = 1} ^ {i = N} \sum_ {j = 1} ^ {j = N} w _ {i} w _ {j} \sigma_ {i} ^ {\prime} \sigma_ {j} ^ {\prime} \rho_ {i j}.}\tag{11.8}
$$

## 11.1 Special Cases

Suppose the assets all have zero correlation with one another, i.e. $\rho _ { i j } \equiv 0 , \forall i \neq j$ (of course $\rho _ { i i } = 1 )$ . Then equation (11.8) becomes 

$$
{V a r (R _ {p})} = {\sum_ {i = 1} ^ {i = N} (\sigma_ {i} ^ {\prime}) ^ {2} (w _ {i}) ^ {2}.}\tag{11.9}
$$

Now, suppose we equally weight all the assets in the portfolio, i.e. $w _ { i } = 1 / N , \forall i$ . Let $m a x _ { i } \sigma _ { i } ^ { \prime } = \sigma _ { m a x } ^ { \prime }$ , then 

$$
\begin{array}{r c l} V a r (R _ {p}) & = & \frac {1}{N ^ {2}} \sum_ {i = 1} ^ {i = N} (\sigma_ {i} ^ {\prime}) ^ {2} \\ & \leq & \frac {N (\sigma_ {m a x} ^ {\prime}) ^ {2}}{N ^ {2}} \\ & = & O \left(\frac {1}{N}\right), \end{array}\tag{11.10}
$$

so that in this special case, if we diversify over a large number of assets, the standard deviation of the portfolio tends to zero as $N \to \infty$ 

Consider another case: all assets are perfectly correlated, $\rho _ { i j } = 1 , \forall i , j$ . In this case 

$$
\begin{array}{r c l} V a r (R _ {p}) & = & \sum_ {i = 1} ^ {i = N} \sum_ {j = 1} ^ {j = N} w _ {i} w _ {j} \sigma_ {i} ^ {\prime} \sigma_ {j} ^ {\prime} \\ & = & \left[ \sum_ {j = 1} ^ {j = N} w _ {j} \sigma_ {j} ^ {\prime} \right] ^ {2} \end{array}\tag{11.11}
$$

so that if $s d ( R ) = \sqrt { V a r ( R ) }$ is the standard deviation of R, then, in this case 

$$
{s d (R _ {p})} = {\sum_ {j = 1} ^ {j = N} w _ {j} \sigma_ {j} ^ {\prime},}\tag{11.12}
$$

which means that in this case the standard deviation of the portfolio is simply the weighted average of the individual asset standard deviations. 

In general, we can expect that $0 < | \rho _ { i j } | < 1$ , so that the standard deviation of a portfolio of assets will be smaller than the weighted average of the individual asset standard deviation, but larger than zero. 

This means that diversification will be a good thing (as Martha Stewart would say) in terms of risk versus reward. In fact, a portfolio of as little as 10 − 20 stocks tends to reap most of the benefits of diversification. 

## 11.2 The Portfolio Allocation Problem

Diferent investors will choose diferent portfolios depending on how much risk they wish to take. However, all investors like to achieve the highest possible expected return for a given amount of risk. We are assuming that risk and standard deviation of portfolio return are synonymous. 

Let the covariance matrix C be defined as 

$$
[ C ] _ {i j} = C _ {i j} = \sigma_ {i} ^ {\prime} \sigma_ {j} ^ {\prime} \rho_ {i j}\tag{11.13}
$$

and define the vectors $\bar { \mu } = [ \mu _ { 1 } ^ { \prime } , \mu _ { 2 } ^ { \prime } , . . . , \mu _ { N } ^ { \prime } ] ^ { t } , \bar { w } = [ w _ { 1 } , w _ { 2 } , . . . , w _ { N } ] ^ { t }$ . In theory, the covariance matrix should be symmetric positive semi-definite. However, measurement errors may result in C having a negative eigenvalue, which should be fixed up somehow. 

The expected return on the portfolio is then 

$$
\overline {{R _ {p}}} = \bar {w} ^ {t} \bar {\mu},\tag{11.14}
$$

and the variance is 

$$
{V a r (R _ {p})} = {\bar {w} ^ {t} C \bar {w}.}\tag{11.15}
$$

We can think of portfolio allocation problem as the following. Let α represent the degree with which investors want to maximize return at the expense of assuming more risk. If $\alpha  0 .$ , then investors want to avoid as much risk as possible. On the other hand, if $\alpha  \infty$ , then investors seek only to maximize expected return, and don’t care about risk. The portfolio allocation problem is then (for given α) find ¯w which satisfies 

$$
\min _ {\bar {w}} \bar {w} ^ {t} C \bar {w} - \alpha \bar {w} ^ {t} \bar {\mu}\tag{11.16}
$$

subject to the constraints 

$$
\sum_ {i} w _ {i} = 1\tag{11.17}
$$

$$
L _ {i} \leq w _ {i} \leq U _ {i}; i = 1, \dots , N.\tag{11.18}
$$

Constraint (11.17) is simply equation (11.6), while constraints (11.18) may arise due to the nature of the portfolio. For example, most mutual funds can only hold long positions $( w _ { i } \geq 0 )$ , and they may also be prohibited from having a large position in any one asset $\left( \mathrm { e . g . } w _ { i } \leq . 2 0 \right)$ . Long-short hedge funds will not have these types of restrictions. For fixed $\alpha ,$ , equations (11.16-11.18) constitute a quadratic programming problem. 

Let 

$$
\begin{array}{r c l} s d (R _ {p}) & = & \text {standard deviation of R_{p}} \\ & = & \sqrt {\operatorname{Var} (R _ {p})} \end{array}\tag{11.19}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/7639d6b5cde0caa0492240c7a23916979e3996a76413767ec0f3fe8aa1bc40b1.jpg)



Figure 11.1: A typical eficient frontier. This curve shows, for each value of portfolio standard deviation $S D ( R _ { p } )$ , the maximum possible expected portfolio return $R _ { p }$ . Data in equation (11.20).


We can now trace out a curve on the $( s d ( R _ { p } ) , \overline { { R _ { p } } } )$ plane. We pick various values of $\alpha ,$ and then solve the quadratic programming problem (11.16-11.18). Figure 11.1 shows a typical curve, which is also known as the eficient frontier. The data used for this example is 

$$
\begin{array}{r l} \bar {\mu} = \left[ \begin{array}{l}. 1 5 \\ . 2 0 \\ . 0 8 \end{array} \right] & ; C = \left[ \begin{array}{c c c}. 2 0 & . 0 5 & -. 0 1 \\ . 0 5 & . 3 0 & . 0 1 5 \\ -. 0 1 & . 0 1 5 & . 1 \end{array} \right] \\ L = \left[ \begin{array}{l} 0 \\ 0 \\ 0 \end{array} \right] & ; U = \left[ \begin{array}{l} \infty \\ \infty \\ \infty \end{array} \right] \end{array}\tag{11.20}
$$

We have restricted this portfolio to be long only. For a given value of the standard deviation of the portfolio return $\left( s d ( R _ { p } ) \right)$ , then any point below the curve is not eficient, since there is another portfolio with the same risk (standard deviation) and higher expected return. Only points on the curve are eficient in this manner. In general, a linear combination of portfolios at two points along the eficient frontier will be feasible, i.e. satisfy the constraints. This feasible region will be convex along the eficient frontier. Another way of saying this is that a straight line joining any two points along the curve does not intersect the curve except at the given two points. Why is this the case? If this was not true, then the eficient frontier would not really be eficient. (see Portfolio Theory and Capital Markets, W. Sharpe, McGraw Hill, 1970, reprinted in 2000). 

Figure 11.2 shows results if we allow the portfolio to hold up to .25 short positions in each asset. In other words, the data is the same as in (11.20) except that 

$$
L = \left[ \begin{array}{l} -. 2 5 \\ -. 2 5 \\ -. 2 5 \end{array} \right].\tag{11.21}
$$

In general, long-short portfolios are more eficient than long-only portfolios. This is the advertised advantage of long-short hedge funds. 

Since the feasible region is convex, we can actually proceed in a diferent manner when constructing the eficient frontier. First of all, we can determine the maximum possible expected return $( \alpha = \infty$ in equation 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/f0cb60d7b74cde263ad55ecfcef3d507cedd1f38207ee90c4297ed8387335bbb.jpg)



Figure 11.2: Eficient frontier, comparing results for long-only portfolio (11.20) and a long-short portfolio (same data except that lower bound constraint is replaced by equation (11.21).


(11.16)), 

$$
\begin{array}{l} \min _ {\bar {w}} - \bar {w} ^ {t} \bar {\mu} \\ \sum_ {i} w _ {i} = 1 \\ L _ {i} \leq w _ {i} \leq U _ {i}; i = 1, \dots , N \end{array}\tag{11.22}
$$

which is simply a linear programming problem. If the solution weight vector to this problem is $( \bar { w } ) _ { m a x } ,$ , then the maximum possible expected return is $( \overline { { R _ { p } } } ) ^ { m a x } = \bar { w } _ { m a x } ^ { t } \bar { \mu }$ 

Then determine the portfolio with the smallest possible risk, $( \alpha = 0$ in equation (11.16) ) 

$$
\begin{array}{l} \min _ {\bar {w}} \bar {w} ^ {t} C \bar {w} \\ \sum_ {i} w _ {i} = 1 \\ L _ {i} \leq w _ {i} \leq U _ {i}; i = 1, \dots , N. \end{array}\tag{11.23}
$$

If the solution weight vector to this quadratic program is given by $\bar { w } _ { m i n } ,$ then the minimum possible portfolio return is $( \overline { { R _ { p } } } ) ^ { m i n } = \bar { w } _ { m i n } ^ { t } \bar { \mu }$ . We then divide up the range $[ ( \overline { { R _ { p } } } ) ^ { \dot { m } i n } , ( \overline { { R _ { p } } } ) ^ { m a x } ]$ into a large number of discrete portfolio returns $( \overline { { R _ { p } } } ) _ { k } ; k = 1 , . . . , N _ { p t s }$ . Let $e = [ 1 , 1 , . . . , 1 ] ^ { t }$ , and 

$$
A = \left[ \begin{array}{c} {\bar {\mu} ^ {t}} \\ {e ^ {t}} \end{array} \right]; B ^ {k} = \left[ \begin{array}{c} {(R _ {p}) _ {k}} \\ 1 \end{array} \right]\tag{11.24}
$$

then, for given $( \overline { { R _ { p } } } ) _ { k }$ we solve the quadratic program 

$$
\begin{array}{l} \min _ {\bar {w}} \bar {w} ^ {t} C \bar {w} \\ A \bar {w} = B ^ {k} \\ L _ {i} \leq w _ {i} \leq U _ {i}; i = 1, \dots , N, \end{array}\tag{11.25}
$$

with solution vector $( \bar { w } ) _ { k }$ and hence portfolio standard deviation $s d ( ( R _ { p } ) _ { k } ) = \sqrt { ( \bar { w } ) _ { k } ^ { t } C ( \bar { w } ) _ { k } }$ . This gives us a set of pairs $( s d ( ( R _ { p } ) _ { k } ) , ( \overline { { R _ { p } } } ) _ { k } ) , k = 1 , . . . , N _ { p t s }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/0bd16130ae2072b59ca2d868f66e1759e6c418e374f05669daacedbe7937f6e8.jpg)



Figure 11.3: The eficient frontier from Figure 11.1 (all risky assets), and the eficient frontier with the same assets as in Figure 11.1, except that we include a risk free asset. In this case, the eficient frontier becomes a straight line, shown as the capital market line.


## 11.3 Adding a Risk-free asset

Up to now, we have assumed that each asset is risky, i.e. $\sigma _ { i } ^ { \prime } > 0 , \forall i$ . However, what happens if we add a risk free asset to our portfolio? This risk-free asset must earn the risk free rate $r ^ { \prime } = r \Delta t .$ and its standard deviation is zero. The data for this case is (the risk-free asset is added to the end of the weight vector, with $r ^ { \prime } = . 0 3 )$ 

$$
\bar {\mu} = \left[ \begin{array}{l}. 1 5 \\ . 2 0 \\ . 0 8 \\ . 0 3 \end{array} \right]; C = \left[ \begin{array}{c c c c}. 2 0 & . 0 5 & -. 0 1 & 0. 0 \\ . 0 5 & . 3 0 & . 0 1 5 & 0. 0 \\ -. 0 1 & . 0 1 5 & . 1 & 0. 0 \\ 0. 0 & 0. 0 & 0. 0 & 0. 0 \end{array} \right]
$$

$$
L = \left[ \begin{array}{c} 0 \\ 0 \\ 0 \\ - \infty \end{array} \right]; U = \left[ \begin{array}{c} \infty \\ \infty \\ \infty \\ \infty \end{array} \right]\tag{11.26}
$$

where we have assumed that we can borrow any amount at the risk-free rate (a dubious assumption). 

If we compute the eficient frontier with a portfolio of risky assets and include one risk-free asset, we get the result labeled capital market line in Figure 11.3. In other words, in this case the eficient frontier is a straight line. Note that this straight line is always above the eficient frontier for the portfolio consisting of all risky assets (as in Figure 11.1). In fact, given the eficient frontier from Figure 11.1, we can construct the eficient frontier for a portfolio of the same risky assets plus a risk free asset in the following way. First of all, we start at the point $( 0 , r ^ { \prime } )$ in the $( s d ( R _ { p } ) , \overline { { R _ { p } } } )$ plane, corresponding to a portfolio which consists entirely of the risk free asset. We then draw a straight line passing through $( 0 , r ^ { \prime } )$ , which touches the all-risky-asset eficient frontier at a single point (the straight line is tangent the all-risky-asset eficient frontier). Let the portfolio weights at this single point be denoted by $\bar { w } _ { M }$ . The portfolio corresponding to the weights $\bar { w } _ { M }$ is termed the market portfolio. Let $( \overline { { { R _ { p } } } } ) _ { M } = \bar { w } _ { M } ^ { t } \bar { \mu }$ be the expected return on this market portfolio, with corresponding standard deviation $s d ( ( R _ { p } ) _ { M } )$ . Let $w _ { r }$ be the fraction invested in the risk free asset. Then, any point along the capital market line has 

$$
\begin{array}{r c l} \overline {{R _ {p}}} & = & w _ {r} r ^ {\prime} + (1 - w _ {r}) (\overline {{R _ {p}}}) _ {M} \\ s d (R _ {p}) & = & (1 - w _ {r}) s d ((R _ {p}) _ {M}). \end{array}\tag{11.27}
$$

If $w _ { r } \geq 0$ , then we are lending at the risk-free rate. If $w _ { r } < 0 .$ we are borrowing at the risk-free rate. 

Consequently, given a portfolio of risky assets, and a risk-free asset, then all investors should divide their assets between the risk-free asset and the market portfolio. Any other choice for the portfolio is not eficient. Note that the actual fraction selected for investment in the market portfolio depends on the risk preferences of the investor. 

The capital market line is so important, that the equation of this line is written as $\overline { { R _ { p } } } = r ^ { \prime } { + } \lambda _ { M } \ s d ( ( R _ { p } ) )$ where $\lambda _ { M }$ is the market price of risk. In other words, all diversified investors, at any particular point in time, should have diversified portfolios which plot along the capital market line. All portfolios should have the same Sharp ratio 

$$
\lambda_ {M} = \frac {\overline {{R _ {p}}} - r ^ {\prime}}{s d (R _ {p})}.\tag{11.28}
$$

## 11.4 Criticism

Is mean-variance portfolio optimization the solution to all our problems? Not exactly. We have assumed that $\mu ^ { \prime } , \sigma ^ { \prime }$ are independent of time. This is not likely. Even if these parameters are reasonably constant, they are dificult to estimate. In particular, $\mu ^ { \prime }$ is hard to determine if the time series of returns is not very long. Remember that for short time series, the noise term (Brownian motion) will dominate. If we have a long time series, we can get a better estimate for $\mu ^ { \prime } { \ : } _ { : }$ , but why do we think $\mu ^ { \prime }$ for a particular firm will be constant for long periods? Probably, stock analysts should be estimating $\mu ^ { \prime }$ from company balance sheets, sales data, etc. However, for the past few years, analysts have been too busy hyping stocks and going to lunch to do any real work. So, there will be lots of diferent estimates of $\mu ^ { \prime } , C$ , and hence many diferent optimal portfolios. 

In fact, some recent studies have suggested that if investors simply use the $1 / N$ rule, whereby initial wealth is allocated equally between N assets, that this does a pretty good job, assuming that there is uncertainty in the estimates of $\mu ^ { \prime } , C$ 

We have also assumed that risk is measured by standard deviation of portfolio return. Actually, if I am long an asset, I like it when the asset goes up, and I don’t like it when the asset goes down. In other words, volatility which makes the price increase is good. This suggests that perhaps it may be more appropriate to minimize downside risk only (assuming a long position). 

Perhaps one of the most useful ideas that come from mean-variance portfolio optimization is that diversified investors (at any point in time) expect that any optimal portfolio will produce a return 

$$
\begin{array}{r c l} \overline {{R _ {p}}} & = & r ^ {\prime} + \lambda_ {M} \sigma_ {p} ^ {\prime} \\ & & \overline {{R _ {p}}} = \text {Expected portfolio return} \\ & & r ^ {\prime} = \text {risk - free return in period} \Delta t \\ & & \lambda_ {M} = \text {market price of risk} \\ & & \sigma_ {p} ^ {\prime} = \text {Portfolio volatility}, \end{array}\tag{11.29}
$$

where diferent investors will choose portfolios with diferent $\sigma _ { p } ^ { \prime }$ (volatility), depending on their risk preferences, but $\lambda _ { M }$ is the same for all investors. Of course, we also have 

$$
{\overline {{R _ {M}}}} = {r ^ {\prime} + \lambda_ {M} \sigma_ {M} ^ {\prime}.}\tag{11.30}
$$

Note: there is a whole field called Behavioural Finance, whose adherents don’t think much of meanvariance portfolio optimization. 

Another recent approach is to compute the optimal portfolio weights using using many diferent perturbed input data sets. The input data (expected returns, and covariances) are determined by resampling, i.e. assuming that the observed values have some observational errors. In this way, we can get an some sort of optimal portfolio weights which have some efect of data errors incorporated in the result. This gives us an average eficient frontier, which, it is claimed, is less sensitive to data errors. 

## 11.5 Individual Securities

Equation (11.30) refers to an eficient portfolio. What is the relationship between risk and reward for individual securities? Consider the following portfolio: divide all wealth between the market portfolio, with weight $w _ { M }$ and security i, with weight $w _ { i }$ . By definition 

$$
w _ {M} + w _ {i} = 1,\tag{11.31}
$$

and we define 

$$
\begin{array}{r c l} \overline {{R ^ {M}}} & = & \mathrm{expectedreturnonthemarketportfolio} \\ \overline {{R ^ {i}}} & = & \mathrm{expectedreturnonasset} i \\ \sigma_ {M} ^ {\prime} & = & \mathrm{s.d.ofreturnonmarketportfolio} \\ \sigma_ {i} ^ {\prime} & = & \mathrm{s.d.ofreturnonasset} i \\ C _ {i, M} & = & \sigma_ {M} ^ {\prime} \sigma_ {i} ^ {\prime} \rho_ {i, M} \\ & = & \mathrm{Covariancebetween} i \mathrm{and} M \end{array}\tag{11.32}
$$

Now, the expected return on this portfolio is 

$$
\begin{array}{r c l} \overline {{R _ {p}}} = E [ R _ {p} ] & = & w _ {i} \overline {{R ^ {i}}} + w _ {M} \overline {{R ^ {M}}} \\ & = & w _ {i} R ^ {i} + (1 - w _ {i}) \overline {{R ^ {M}}} \end{array}\tag{11.33}
$$

and the variance is 

$$
\begin{array}{r c l} {V a r (R _ {p})} & = & {(\sigma_ {p} ^ {\prime}) ^ {2} = w _ {i} ^ {2} (\sigma_ {i} ^ {\prime}) ^ {2} + 2 w _ {i} w _ {M} C _ {i, M} + w _ {M} ^ {2} (\sigma_ {M} ^ {\prime}) ^ {2}} \\ & = & {w _ {i} ^ {2} (\sigma_ {i} ^ {\prime}) ^ {2} + 2 w _ {i} (1 - w _ {i}) C _ {i, M} + (1 - w _ {i}) ^ {2} (\sigma_ {M} ^ {\prime}) ^ {2}} \end{array}\tag{11.34}
$$

For a set of values $\{ w _ { i } \}$ , equations (11.33-11.34) will plot a curve in expected return-standard deviation plane $( \overline { { R _ { p } } } , \sigma _ { p } ^ { \prime } )$ (e.g. Figure 11.3). Let’s determine the slope of this curve when $w _ { i } \to 0$ , i.e. when this curve intersects the capital market line at the market portfolio. 

$$
\begin{array}{r c l} {2 (\sigma_ {p} ^ {\prime}) \frac {\partial (\sigma_ {p} ^ {\prime})}{\partial w _ {i}}} & = & {2 w _ {i} (\sigma_ {i} ^ {\prime}) ^ {2} + 2 (1 - 2 w _ {i}) C _ {i, M} + 2 (w _ {i} - 1) (\sigma_ {M} ^ {\prime}) ^ {2}} \\ & & \\ {\frac {\partial \overline {{R _ {p}}}}{\partial w _ {i}}} & = & {\overline {{R ^ {i}}} - \overline {{R ^ {M}}}.} \end{array}\tag{11.35}
$$

Now, 

$$
\begin{array}{r c l} \frac {\partial \overline {{R _ {p}}}}{\partial (\sigma_ {p} ^ {\prime})} & = & \frac {\frac {\partial \overline {{R _ {p}}}}{\partial w _ {i}}}{\frac {\partial (\sigma_ {p} ^ {\prime})}{\partial w _ {i}}} \\ & = & \frac {(\overline {{R ^ {i}}} - \overline {{R ^ {M}}}) (\sigma_ {p} ^ {\prime})}{w _ {i} (\sigma_ {i} ^ {\prime}) ^ {2} + (1 - 2 w _ {i}) C _ {i , M} + (w _ {i} - 1) (\sigma_ {M} ^ {\prime}) ^ {2}}. \end{array}\tag{11.36}
$$

Now, let $w _ { i } \to 0$ in equation (11.36), then we obtain 

$$
\frac {\partial \overline {{R _ {p}}}}{\partial (\sigma_ {p} ^ {\prime})} = \frac {(\overline {{R ^ {i}}} - \overline {{R ^ {M}}}) (\sigma_ {M} ^ {\prime})}{C _ {i , M} - (\sigma_ {M} ^ {\prime}) ^ {2}}\tag{11.37}
$$

But this curve should be tangent to the capital market line, equation (11.30) at the point where the capital market line touches the eficient frontier. If this curve is not tangent to the capital market line, then this implies that if we choose $w _ { i } = \pm \epsilon .$ , then the curve would be above the capital market line, which should not be possible (the capital market line is the most eficient possible portfolio). This assumes that positions with $w _ { i } < 0$ in asset i are possible. 

Assuming that the slope of the $\overline { { R _ { p } } }$ portfolio is tangent to the capital market line gives (from equations (11.30,11.37)) 

$$
{\frac {\overline {{R ^ {M}}} - r ^ {\prime}}{(\sigma_ {M} ^ {\prime})}} = {\frac {(\overline {{R ^ {i}}} - \overline {{R ^ {M}}}) (\sigma_ {M} ^ {\prime})}{C _ {i , M} - (\sigma_ {M} ^ {\prime}) ^ {2}}}\tag{11.38}
$$

or 

$$
\begin{array}{r l r} \overline {{R ^ {i}}} & = & r ^ {\prime} + \beta_ {i} (\overline {{R ^ {M}}} - r ^ {\prime}) \\ & & \beta_ {i} = \frac {C _ {i , M}}{(\sigma_ {M} ^ {\prime}) ^ {2}}. \end{array}\tag{11.39}
$$

The coeficient $\beta _ { i }$ in equation (11.39) has a nice intuitive definition. Suppose we have a time series of returns 

$$
\begin{array}{r l r} {(R ^ {i}) _ {k}} & = & {\mathrm{Returnonasseti,inperiodk}} \\ {(R ^ {M}) _ {k}} & = & {\mathrm{Returnonmarketportfolioinperiodk.}} \end{array}\tag{11.40}
$$

Typically, we assume that the market portfolio is a broad index, such as the TSX 300. Now, suppose we try to obtain a least squares fit to the above data, using the equation 

$$
R ^ {i} \simeq \alpha_ {i} + b _ {i} R ^ {M}.\tag{11.41}
$$

Carrying out the usual least squares analysis (e.g. do a linear regression of $R ^ { i }$ vs. $R ^ { M } )$ , we find that 

$$
b _ {i} = \frac {C _ {i , M}}{(\sigma_ {M} ^ {\prime}) ^ {2}}\tag{11.42}
$$

so that we can write 

$$
R ^ {i} \simeq \alpha_ {i} + \beta_ {i} R ^ {M}.\tag{11.43}
$$

This means that $\beta _ { i }$ is the slope of the best fit straight line to a $( ( R ^ { i } ) _ { k } , ( R ^ { M } ) _ { k } )$ scatter plot. An example is shown in Figure 11.4. Now, from equation (11.39) we have that 

$$
{\overline {{R ^ {i}}}} = {r ^ {\prime} + \beta_ {i} (\overline {{R ^ {M}}} - r ^ {\prime})}\tag{11.44}
$$

which is consistent with equation (11.43) if 

$$
\begin{array}{r c l} {R ^ {i}} & = & {\alpha_ {i} + \beta_ {i} R ^ {M} + \epsilon_ {i}} \\ & & {E [ \epsilon_ {i} ] = 0} \\ & & {\alpha_ {i} = r ^ {\prime} (1 - \beta_ {i})} \\ & & {E [ \epsilon_ {i}, R ^ {M} ] = 0 ,} \end{array}\tag{11.45}
$$

since 

$$
{E [ R ^ {i} ] = \overline {{R ^ {i}}}} = {\alpha_ {i} + \beta_ {i} \overline {{R ^ {M}}}.}\tag{11.46}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/425edd65a31762c23dba15c8db9c5e46724df11a52fe28262f4d3f9de7f33ed0.jpg)



Figure 11.4: Return on Rogers Wireless Communications versus return on TSE 300. Each point represents pairs of daily returns. The vertical axis measures the daily return on the stock and the horizontal axis that of the TSE300.


Equation (11.46) has the interpretation that the return on asset i can be decomposed into a drift component, a part which is correlated to the market portfolio (the broad index), and a random part uncorrelated with the index. Make the following assumptions 

$$
\begin{array}{r c l} {E [ \epsilon_ {i} \epsilon_ {j} ]} & = & {0 ; i \neq j} \\ & = & {e _ {i} ^ {2} ; i = j} \end{array}\tag{11.47}
$$

e.g. that returns on each each asset are correlated only through their correlation with the index. Consider once again a portfolio where the wealth is divided amongst $N$ assets, each asset receiving a fraction $w _ { i }$ of the initial wealth. In this case, the return on the portfolio is 

$$
\begin{array}{r c l} {R _ {p}} & = & {\sum_ {i = 1} ^ {i = N} w _ {i} R ^ {i}} \\ {\overline {{R _ {p}}}} & = & {\sum_ {i = 1} ^ {i = N} w _ {i} \alpha_ {i} + \overline {{R ^ {M}}} \sum_ {i = 1} ^ {i = N} w _ {i} \beta_ {i}} \end{array}\tag{11.48}
$$

and 

$$
\begin{array}{r c l} s. d. (R _ {p}) & = & \sqrt {(\sigma_ {M} ^ {\prime}) ^ {2} \sum_ {i = 1} ^ {i = N} \sum_ {j = 1} ^ {j = N} w _ {i} w _ {j} \beta_ {i} \beta_ {j} + \sum_ {i = 1} ^ {i = N} w _ {i} ^ {2} e _ {i} ^ {2}} \\ & = & \sqrt {(\sigma_ {M} ^ {\prime}) ^ {2} \left(\sum_ {i = 1} ^ {i = N} w _ {i} \beta_ {i}\right) ^ {2} + \sum_ {i = 1} ^ {i = N} w _ {i} ^ {2} e _ {i} ^ {2}} . \end{array}\tag{11.49}
$$

Now, if $w _ { i } = O ( 1 / N )$ , then 

$$
\sum_ {i = 1} ^ {i = N} w _ {i} ^ {2} e _ {i} ^ {2}\tag{11.50}
$$

is $O ( 1 / N )$ as N becomes large, hence equation (11.49) becomes 

$$
s. d. (R _ {p}) \simeq \sigma_ {M} ^ {\prime} \left| \sum_ {i = 1} ^ {i = N} w _ {i} \beta_ {i} \right|.\tag{11.51}
$$

Note that if we write 

$$
{\overline {{R ^ {i}}}} = {r ^ {\prime} + \lambda_ {i} \sigma_ {i} ^ {\prime}}\tag{11.52}
$$

then we also have that 

$$
{\overline {{R ^ {i}}}} = {r ^ {\prime} + \beta_ {i} (\overline {{R ^ {M}}} - r ^ {\prime})}\tag{11.53}
$$

so that the market price of risk of security i is 

$$
\lambda_ {i} = \frac {\beta_ {i} (\overline {{R ^ {M}}} - r ^ {\prime})}{\sigma_ {i} ^ {\prime}}\tag{11.54}
$$

which is useful in real options analysis. 

## 12 Stocks for the Long Run?

Conventional wisdom states that investment in a diversified portfolio of equities has a low risk for a long term investor. However, in a recent article (”Irrational Optimism,” Fin. Anal. J. E. Simson, P.Marsh, M. Staunton, vol 60 (January, 2004) 25-35) an extensive analysis of historical data of equity returns was carried out. Projecting this information forward, the authors conclude that the probability of a negative real return over a twenty year period, for a investor holding a diversified portfolio, is about 14 per cent. In fact, most individuals in defined contribution pension plans have poorly diversified portfolios. Making more realistic assumptions for defined contribution pension plans, the authors find that the probability of a negative real return over twenty years is about 25 per cent. 

Let’s see if we can explain why there is this common misconception about the riskiness of long term equity investing. Table 12.1 shows a typical table in a Mutual Fund advertisement. From this table, we are supposed to conclude that 

• Long term equity investment is not very risky, with an annualized compound return about 3% higher than the current yield on government bonds. 

• If S is the value of the mutual fund, and B is the value of the government bond, then 

$$
\begin{array}{r c l} B (T) & = & B (0) e ^ {r T} \\ & & r = . 0 3 \\ S (T) & \simeq & S (0) e ^ {\alpha T} \\ & & \alpha = . 0 6, \end{array}\tag{12.1}
$$

for T large, which gives 

$$
\begin{array}{r l r} \frac {\frac {S (T = 3 0)}{S (0)}}{\frac {B (T = 3 0)}{B (0)}} & = & e ^ {1. 8 -. 9} = e ^ {. 9} \simeq 2. 4 6, \end{array}\tag{12.2}
$$

indicating that you more than double your return by investing in equities compared to bonds (over the long term). 

A convenient way to measure the relative returns on these two investments (bonds and stocks) is to compare the total compound return 

$$
\begin{array}{r c l} \mathrm{Compoundreturn:stocks} & = & \log \left[ \frac {S (T)}{S (0)} \right] = \alpha T \\ \mathrm{Compoundreturn:bonds} & = & \log \left[ \frac {B (T)}{B (0)} \right] = r T, \end{array}\tag{12.3}
$$

<table><tr><td>1 year</td><td>2 years</td><td>5 years</td><td>10 years</td><td>20 years</td><td>30 years</td><td>30 year bond yield</td></tr><tr><td>-2%</td><td>-5%</td><td>10%</td><td>8%</td><td>7%</td><td>6%</td><td>3%</td></tr></table>


Table 12.1: Historical annualized compound return, XYZ Mutual Equity Funds. Also shown is the current yield on a long term government bond


or the annualized compound returns 

Annualized compound return: stocks $= \quad { \frac { 1 } { T } } \log \left[ { \frac { S ( T ) } { S ( 0 ) } } \right] = \alpha$ 

Annualized compound return: bonds $= \quad { \frac { 1 } { T } } \log \left[ { \frac { B ( T ) } { B ( 0 ) } } \right] = r$ 

(12.4) 

If we assume that the value of the equity portfolio S follows a Geometric Brownian Motion 

$$
d S = \mu S d t + \sigma S d Z\tag{12.5}
$$

then from equation (2.56) we have that 

$$
\log \left(\frac {S (T)}{S (0)}\right) \sim N ((\mu - \frac {\sigma^ {2}}{2}) T, \sigma^ {2} T),\tag{12.6}
$$

i.e. the compound return in is normally distributed with mean $( \mu - \frac { \sigma ^ { 2 } } { 2 } ) T$ and variance $\sigma ^ { 2 } T$ , so that the variance of the total compound return increases as T becomes large. 

Since $v a r ( a X ) = a ^ { 2 } v a r ( X )$ , it follows that 

$$
\frac {1}{T} \log \left(\frac {S (T)}{S (0)}\right) \sim N ((\mu - \frac {\sigma^ {2}}{2}), \sigma^ {2} / T),\tag{12.7}
$$

so that the the variance of the annualized return tends to zero at T becomes large. 

Of course, what we really care about is the total compound return (that’s how much we actually have at $t = T$ , relative to what we invested at $t = 0 )$ at the end of the investment horizon. This is why Table 12.1 is misleading. There is significent risk in equities, even over the long term (30 years would be long-term for most investors). 

Figure 12.1 shows the results of 100, 000 simulations of asset prices assuming that the asset follows equation (12.5), with $\mu = . 0 8 , \sigma = . 2$ . The investment horizon is 5 years. The results are given in terms of histograms of the annualized compound return (equation (12.4)) and the total compound return ((equation (12.3)). 

Figure 12.2 shows similar results for an investment horizon of 30 years. Note how the variance of the annualized return has decreased, while the variance of the total return has increased (verifying equations (12.6-12.7)). 

Assuming long term bonds yield 3%, this gives a total compound return over 30 years of .90, for bonds. Looking at the right hand panel of Figure 12.2 shows that there are many possible scenarios where the return on equities will be less than risk free bonds after 30 years. The number of scenarios with return less than risk free bonds is given by the area to the left of .9 in the histogram. 

## 13 Further Reading

## 13.1 General Interest

• Peter Bernstein, Capital Ideas: the improbable origins of modern Wall street, The Free Press, New York, 1992. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/afd579deeccc09c56f6e83c229d0919d2f3df97dcca2ad36abc8da792f7e9457.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/957ba0e774fe8446a34247a601bc20aca6afaf4a145b29963f89461d9edf51b1.jpg)



Figure 12.1: Histogram of distribution of returns $T = 5$ years. $\mu = . 0 8 , \sigma = . 2 ,$ 100, 000 simulations. Left: annualized return 1/T log[S(T)/S(0)]. Right: return $\log [ S ( T ) / S ( 0 ) ]$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/6ba7065ef7dc8e7beecd9117db1bf4caab5dbfdbf9d763e933e041c36243cee8.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/568b2077-c955-4582-82c0-8e5fc6d8f4d0/d4523f72e891292b4ef07bdcadcde6d578fbeff5b39488d1b8c0df73d2273bee.jpg)



Figure 12.2: Histogram of distribution of returns $T = 3 0$ years. µ = .08, σ = .2, 100, 000 simulations. Left: annualized return $1 / T \log [ S ( T ) / S ( 0 ) ]$ . Right: return $\log [ S ( T ) / S ( 0 ) ]$ 2


• Peter Bernstein, Against the Gods: the remarkable story of risk, John Wiley, New York, 1998, ISBN 0-471-29563-9. 

• Burton Malkeil, A random walk down Wall Street, W.W. Norton, New York, 1999, ISBN 0-393-32040-5. 

• N. Taleb, Fooled by Randomness, Texere, 2001, ISBN 1-58799-071-7. 

## 13.2 More Background

• A. Dixit and R. Pindyck, Investment under uncertainty, Princeton University Press, 1994. 

• John Hull, Options, futures and other derivatives, Prentice-Hall, 1997, ISBN 0-13-186479-3. 

• S. Ross, R. Westerfield, J. Jafe, Corporate Finance, McGraw-Hill Irwin, 2002, ISBN 0-07-283137-5. 

• W. Sharpe, Portfolio Theory and Capital Markets, Wiley, 1970, reprinted in 2000, ISBN 0-07-135320-8. (Still a classic). 

• Lenos Triegeorgis, Real Options: Managerial Flexibility and Strategy for Resource Allocation, MIT Press, 1996, ISBN 0-262-20102-X. 

## 13.3 More Technical

• P. Brandimarte, Numerical Methods in Finance: A Matlab Introduction, Wiley, 2002, ISBN 0-471- 39686-9. 

• Boyle, Broadie, Glassermman, Monte Carlo methods for security pricing, J. Econ. Dyn. Con., 21:1267- 1321 (1997) 

• P. Glasserman, Monte Carlo Methods in Financial Engineering, Springer (2004) ISBN 0-387-00451-3. 

• D. Higham, An Introduction to Financial Option Valuation, Cambridge (2004) ISBN 0-521-83884-3. 

• P. Jackel, Monte Carlo Methods in Finance, Wiley, 2002, ISBN 0-471-49741-X. 

• Y.K. Kwok, Mathematical Models of Finance, Springer Singapore, 1998, ISBN 981-3083-565. 

• S. Neftci, An Introduction to the Mathematics of Financial Derivatives, Academic Press (2000) ISBN 0-12-515392-9. 

• R. Seydel, Tools for Computational Finance, Springer, 2002, ISBN 3-540-43609-X. 

• D. Tavella and C. Randall, Pricing Financial Instruments: the Finite Diference Method, Wiley, 2000, ISBN 0-471-19760-2. 

• D. Tavella, Quantitative Methods in Derivatives Pricing: An Introduction to Computational Finance, Wiley (2002) ISBN 0-471-39447-5. 

• N. Taleb, Dynamic Hedging, Wiley, 1997, ISBN 0-471-15280-3. 

• P. Wilmott, S. Howison, J. Dewynne, The mathematics of financial derivatives: A student introduction, Cambridge, 1997, ISBN 0-521-49789-2. 

• Paul Wilmott, Paul Wilmott on Quantitative Finance, Wiley, 2000, ISBN 0-471-87438-8. 

pdflatex version 