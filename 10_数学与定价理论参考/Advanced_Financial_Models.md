

<!-- === Source: MinerU_markdown_Advanced_Financial_Models_1_2122707983329767440.md (Page 1) === -->

# Advanced Financial Models

Michael R. Tehranchi 

## Contents

1. Standing assumptions: complications we ignore 5  
2. Further modelling complications 8  
3. Prerequisite knowledge 10   
Chapter 1. Discrete-time models 11  
1. Measurability and conditional expectations 11  
2. The set-up 16  
3. The first fundamental theorem and martingales 19  
4. Local martingales 21  
5. Proof of the 1FTAP, easier direction 25  
6. Proof of harder direction of the 1FTAP 26  
7. Numéraires and equivalent martingale measures 30  
8. Special numéraires and equivalent martingale measures 35  
9. Contingent claim pricing and hedging 39  
10. Replication with calls and puts 47  
11. Call prices from moment generating functions 49  
12. Super-replication of American claims 51  
13. A dual approach to optimal stopping 54   
Chapter 2. Brownian motion and stochastic calculus 57  
1. Brownian motion 57  
2. Itô stochastic integration 59  
3. Itô's processes and quadratic variation 62  
4. Itô's formula 63  
5. Girsanov's theorem 65  
6. A martingale representation theorem 67   
Chapter 3. Continuous-time models 69  
1. The set-up 69  
2. Admissible strategies 69  
3. Arbitrage and local martingale deflators 72  
4. The structure of local martingale deflators 74  
5. Replication of European claims 76  
6. Risk-neutral measures 79  
7. The Black-Scholes model and formula 80  
8. Markovian markets: pricing and hedging by PDE 81  
9. Partial differential equations and conditional expectations 83  
10. Risk-neutral pricing and PDEs 86 

11. Beyond Black–Scholes 89
Chapter 4. Crashcourse on probability theory 95
1. Measures 95
2. Random variables 95
3. Expectations and variances 96
4. Special distributions 98
5. Conditional probability and expectation, independence 99
6. Probability inequalities 99
7. Characteristic functions 100
8. Fundamental probability results 100 

Financial mathematics as a subject is young (as compared to, say, number theory), but it is mature enough now that there has emerged some consensus on the notation, vocabulary and important results. These notes are an attempt to present many of the main ingredients of this theory, mainly concerning the pricing and hedging of derivative securities. 

But before launching into the story, we will begin by acknowledging some of the real-world complications that will not be discussed at length hereafter. 

## 1. Standing assumptions: complications we ignore

Unfortunately, actual financial markets are very complicated. Of course, in order to develop a systematic financial theory, it is prudent to concentrate on the essential features of these markets and ignore the less essential complications. Therefore, the theory that will be presented in these notes is concerned with the analysis of market models that have plenty of simplifying assumptions. 

That is not to say that these complications are not important. Indeed, there is active ongoing research attempting to remove these simplifying assumptions from the canonical theory. Below is a list of these assumptions. 

1.1. Dividends. The total stock of a publicly traded firm is divided into a fixed number N of shares. The owner of each share is then entitled to the fraction 1/N of the total profit of the firm.<sup>1</sup> A portion of the firm’s profit is usually reinvested by management, for instance by building new factories, but the rest of the profit is paid out to the shareholders. In particular, the owner of each share of stock will receive periodically a dividend payment. 

However, in this course, 

## we will usually assume that there are no dividend payments.

Actually, this assumption is not as terrible as it sounds. We will see see shortly how to adapt the theory developed for assets that pay no dividends to incorporate assets that have non-zero dividend payments. 

1.2. Tick size. Financial markets usually have a smallest increment of price, the tick. (The tick refers back to the days when prices were quoted on ticker tape.) Indeed, the tick size can vary from market to market, and even for assets traded in the same market. 

However, in this course, 

This is a convenient assumption for those who prefer continuous mathematics to discrete. It is usually a harmless assumption, unless the prices of interest are very close to zero. 

1.3. Transactions costs. Financial transactions are processed by a string of middle men, each of whom charge a fee for their services. Usually the fee is nearly proportional to the size of the transaction. 

However, in this course, 

we will assume that there are no transactions costs. 

This assumption is justified by by the fact that transactions costs are often very small relative to the size of typical transactions. But one must always remember that in some applications, it might not be wise to neglect these costs. 

1.4. Short-selling constraints. In the real world, it is actually possible for someone to sell an asset that he does not own. The essential mechanism is to borrow a share of that asset from a broker, and then immediately to sell it to the market. This procedure is called short selling. 

Brokers, however, place contraints on this behaviour. Indeed, they usually require collateral and charge a fee for their service. Furthemore, if the market price of the asset increases, or if the price of the collateral decreases, the broker may ask the short seller to put up even more collateral. 

However, in this course, 

we will assume that there are no short-selling constraints. 

Indeed, the theory of discrete-time trading is cleaner without additional assumptions on the sizes of trades. But we will see that to overcome some technical problems in the theory of continuous-time trading, it will be natural to restrict trading to what are called admissible strategies. 

1.5. Divisibility of assets. There is another real-world trading constraint of a rather technical nature. The smallest unit of stock is the share. A share cannot be further divided – it is generally impossible to buy half a share of a particular stock. 

However, in this course, 

we will assume that assets are infinitely divisible. 

1.6. Bid-ask spread. Real-world trading is asymmetrical since the price to buy a share is usually higher than the price to sell it. The reason is that are two diferent ways to buy or sell an asset listed on an exchange: the limit order and the market order. 

A limit buy order is an ofer to buy a certain number of shares of the asset at a certain price. A limit sell order is defined similarly. The collection of unfilled limit orders is called the limit order book. 

At any time, there is the highest price for which there is an order to buy the asset. This is called the bid price. The lowest price for which there is an order to sell is called the ask price. The bid/ask spread is the diference. Figure 1 illustrates the evolution of a hypothetical limit order book as various orders arrive and are filled. 

A market order are instructions to execute a transaction at the best available price. In particular, if the market order is to buy, then the lowest limit sell order is filled first. Therefore, for small market buy orders, the per share price paid is the ask price. Similarly, if a market sell order arrives, then the highest limit buy order is filled first, and hence the per share price received is the bid price. 

However, in this course, 

we will assume that there are no bid-ask spreads. 

This assumption is justified by the observation that in many markets, the spread is very small. However, in times of crisis, this assumption is not usually applicable, and hence the theory breaks down dramatically. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/a00066c50710d9dd72e129f8c2ff19a2a2b5129ee98511c19502e11946020302.jpg)



Old limit buy order is cancelled


Figure 1. Top left. The bid price is £8 and the ask is £11. Top right. A limit sell order for three shares at £11 arrives. Bottom left. A limit buy order for two shares at £8 is cancelled. Bottom right. A market order to buy five shares arrives. Note that four shares are sold at £11 and one at £12. After the transaction, the ask price is £12. 

1.7. Market depth. As described above, there are only a finite number of limit orders on the book at one time. If a large market buy order arrives, for instance, then the lowest limit sell order is filled first. But if the market order is bigger than the total shares available to buy at the ask price, then the limit orders at the next-to-lowest price are filled, and progresses up the book until the market order is finally filled. In this way, the ask price increases. 

The market depth is the number of shares available to buy or sell at the ask or bid price respectively. Equivalently, the depth of a market is a measure of the size of a market order necessary to move quoted prices. 

However, in this course, 

we will assume that there is infinite market depth. 

Equivalently, we will assume that investors are small relative to the limit order book, so they are price takers, not price makers. However, the most recent financial crisis shows that this assumption does not always approximate reality – just ask the traders at Lehman Brothers! 

## 2. Further modelling complications

Microeconomic models usually involve the interaction of hypothetical agents who are endowed with preferences over some set of economic variables. The observed outcome of the system is then described by an equilibrium in which the competing preferences of the various agents are balanced through some economic mechanism, such as trade. 

We will not deal much with such equilibrium models, but note here that equilibrium models make predictions about the structure of prices in a financial market (after we have made all of the simplifying assumptions listed above). In particular, in an equilibrium model, there cannot be an arbitrage. This will be explained in Chapter 1, but for the sake of this preface, we discuss some of the standard assumptions of equilibrium models and why they may fail in real life. 

2.1. The expected utility hypothesis. In many standard microeconomic models, agents have preferences over random variables. For instance, suppose that the agent is young now but is planning for retirement. The amount of money that the agent will have in his pension fund when he retires can be modelled as a random variable. Of course, the particular random variable depends on the investment policy the agent chooses now. 

The agent much choose his favourite investment strategy. Therefore, we must model his preferences over random variables. The expected utility hypothesis says that the agent prefers the random variable X to the random variable Y if and only if 

$$
\mathbb {E} [ U (X) ] > \mathbb {E} [ U (Y) ]
$$

where the function $U : \mathbb { R }  \mathbb { R }$ , called the agent’s utility function models the agents aversion risk. 

The expected utility hypothesis seems to have a certain intuitive appeal, and practically, it does make the modelling problem more tractable. Furthermore, von Neumann and Morgenstern showed that the expected utility hypothesis is equivalent to a sensible seeming axiomisation of preferences. 

2.2. The Allais paradox. The expected utility hypothesis can be tested, and it seems that real human beings do not always behave as though their preferences are consistent with it. Consider two games. 

Game A. You must choose between a payment of either X or Y pounds, where 

$$
X = \left\{ \begin{array}{l l} 1 0 1 & \text {with prob.} 0. 3 3 \\ 1 0 0 & \text {with prob.} 0. 6 6 \\ 0 & \text {with prob.} 0. 0 1 \end{array} \right. \quad \text {and} Y = 1 0 0 \text {with prob.} 1
$$

Game B. Again you must choose between a payment of either X or Y pounds, but now 

$$
X = \left\{ \begin{array}{l l} 1 0 0 & \text {with prob. 0.34} \\ 0 & \text {with prob. 0.66} \end{array} \right. \quad \text {and} Y = \left\{ \begin{array}{l l} 1 0 1 & \text {with prob. 0.33} \\ 0 & \text {with prob. 0.67} \end{array} \right.
$$

Apparently, in real experiments, a significant number of people prefer Y in both games. For these people, their preferences are not compatible with the expected utility hypothesis. To see why not, suppose for the sake of finding a contradiction that the agent has a utility function U. Then 

$$
\text { Game   A: } Y \text { preferred } \Leftrightarrow 0. 3 3 U (1 0 1) + 0. 6 6 U (1 0 0) + 0. 0 1 U (0) <   U (1 0 0)
$$

and 

$$
\text { Game   B: } Y \text { preferred } \Leftrightarrow 0. 3 4 U (1 0 0) + 0. 6 6 U (0) <   0. 3 3 U (1 0 1) + 0. 6 7 U (0)
$$

But the above inequalities cannot both hold true! 

2.3. The Ellsberg paradox. Underlying the expected utility hypothesis is assumption that economic agents are perfect statisticians. In reality, of course, when faced with a random outcome, there is risk associated with the realisation of the randomness, but also uncertainty in the unknown distribution of the randomness. Here is an example. 

Consider an urn with 30 balls, coloured red, yellow and black. You know that there are 10 red balls in the urn. However, you do not know the number of yellow balls or the number of black balls (but, of course, their sum to 20). 

A single ball is drawn from the urn. Consider two games: 

$$
X = \left\{ \begin{array}{l l} 1 0 0 & \text {if red} \\ 0 & \text {if yellow or black} \end{array} \right. \quad \text {and} Y = \left\{ \begin{array}{l l} 1 0 0 & \text {if yellow} \\ 0 & \text {if red or black} \end{array} \right.
$$

Game B. 

$$
X = \left\{ \begin{array}{l l} 1 0 0 & \text {if red or black} \\ 0 & \text {if yellow} \end{array} \right. \quad \text {and} Y = \left\{ \begin{array}{l l} 1 0 0 & \text {if yellow or black} \\ 0 & \text {if red} \end{array} \right.
$$

In experiments, people tend to prefer X in game A and Y in game B. This also contradicts the expected utility hypothesis. Suppose the agent estimates the probability of drawing yellow as p where $0 < p < 2 / 3$ 

Game A: X preferred 

$$
\Leftrightarrow \frac {1}{3} U (1 0 0) + \frac {2}{3} U (0) > p U (1 0 0) + (1 - p) U (0)
$$

and 

Game B: Y preferred 

$$
\Leftrightarrow (1 - p) U (1 0 0) + p U (0) <   \frac {2}{3} U (1 0 0) + \frac {1}{3} U (0)
$$

a contradiction! 

One way to avoid this paradox is to let the agent have preferences not only of risk but also uncertainty. For example, suppose that there is a probability models P consistent with the agent’s beliefs. An agent who is very averse uncertainty would prefer X to Y if and only if 

$$
\inf _ {\mathbb {P} \in \mathcal {P}} \mathbb {E} ^ {\mathbb {P}} [ U (X) ] > \inf _ {\mathbb {P} \in \mathcal {P}} \mathbb {E} ^ {\mathbb {P}} [ U (Y) ].
$$

This point of view is pursued in an area called robust finance, but we will not discuss it in these notes. 

## 3. Prerequisite knowledge

The emphasis of this course is on some of the mathematical aspects of financial market models. Very little is assumed of the reader’s knowledge of the workings of financial markets. However, some mathematical background is needed. 

Our starting point is the famous observation (sometimes attributed to Niels Bohr) that it is dificult to make predictions, especially about the future. Indeed, anyone with even a passing acquaintance with finance knows that most of us cannot predict with absolute certainty how the the price of an asset will fluctuate – otherwise we would be much richer! 

Therefore, the proper language to formulate the models that we will study is the language of probability theory. An attempt is made to keep this course self-contained, but you should be familiar with the basics of the theory, including knowing the definition and key properties of the following concepts: random variable, expected value, variance, conditional probability/expectation, independence, Gaussian (normal) distribution, etc. Familiarity with measure theoretical probability is helpful, though a crashcourse on probability theory is given in an appendix. 

Please send all comments and corrections (including small typos and major blunders) to me at m.tehranchi@statslab.cam.ac.uk. 

## CHAPTER 1

## Discrete-time models

We consider a market with n assets. The identity of the assets is not important as long as the standing assumptions (zero dividends, zero tick size, zero transaction costs, no short-selling constraints, infinite divisibility, zero bid-ask spread, infinite market depth) are fulfilled. We usually think of the assets as being stocks and bonds, but they also can be more exotic things like pork belly futures. 

We will use the notation $P _ { t } ^ { i }$ for the price of asset i at time t. In this section, the time index set is the non-negative integers, so the notation $t \geq 0$ should be interpreted as $t \in \{ 0 , 1 , 2 , \ldots \}$ 

## 1. Measurability and conditional expectations

A modelling assumption that we will use throughout is that the collection of prices $P =$ $( P _ { t } ^ { 1 } , \dots , P _ { t } ^ { n } ) _ { t \geq 0 }$ is an n-dimensional stochastic process adapted to a filtration $\mathbb { F } = ( \mathcal { F } _ { t } ) _ { t \geq 0 }$ We now briefly describe what this means. 

A stochastic process $( Z _ { t } ) _ { t \geq 0 }$ is just a collection of random variables (or vectors) indexed by the parameter t. In our case, the parameter is interpreted as time, either discrete or continuous. (Recall that when we speak of a random variable $Z$ , we secretly have a probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ in the background such that the map $Z : \Omega \to \mathbb { R }$ is F-measurable. See the crashcourse if this sounds unfamiliar to you.) 

We now formalise the concept of information being revealed as time marches forward. The correct notions are that of a filtration and adaptedness. 

Motivation. You are probably already familiar with the notion of the measurability of a set. Measurability is a hugely important (though technical) idea in the theory of Lebesgue integration: for instance, Vitali showed that it is impossible to define the Lebesgue measure of every subset of R. 

But on top of its technical importance, measurability has is a way to model information. Give an probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ , let G be some set of information. For the moment, we will be vague about what G is, but it intuitively should have the property that an event $A \in { \mathcal { F } }$ is ${ \mathcal { G } } .$ -measurable if 

$$
\mathbb {P} (A | \mathcal {G}) \in \{0, 1 \}.
$$

Note we have not yet defined the notation $\mathbb { P } ( A | \mathcal { G } )$ , but it should thought of as the probability of the event A given knowledge of the information set $\mathcal { G }$ 

For instance, consider the experiment of tossing a fair coin two times. We can model this experiment on the sample space $\Omega = \{ H H , H T , T H , T T \}$ . The set of all events is the set 

$$
\mathcal {F} = \{\emptyset , \{H H \}, \dots , \{H H, H T \}, \dots , \{H H, H T, T H \}, \dots , \{H H, H T, T H, T T \} \}
$$

of all $2 ^ { 4 } = 1 6$ subsets of $\Omega .$ . The probability measure is just the one that assigns $\mathbb { P } ( \{ \omega \} ) = 1 / 4$ equal probability to each elementary event. 

Suppose $\mathcal { G }$ is information revealed by the first toss of the coin. The set event 

$$
A = \{\text {   first   toss   is   heads   } \} = \{H H, H T \}
$$

is $\mathcal { G }$ -measurable, since for any sensible definition of the conditional probability we must have 

$$
\mathbb {P} (A | \mathcal {G}) = \left\{ \begin{array}{l l} 1 & \text {if the first toss is heads} \\ 0 & \text {if the first toss is tails.} \end{array} \right.
$$

On the other hand, the event 

$$
B = \{\text {   both   tosses   are   heads   } \} = \{H H \}
$$

is not ${ \mathcal { G } } .$ -measurable. Indeed, we must have 

$$
\mathbb {P} (B | \mathcal {G}) = \left\{ \begin{array}{c l} 1 / 2 & \text { if   the   first   toss   is   heads } \\ 0 & \text { if   the   first   toss   is   tails. } \end{array} \right.
$$

Now returning to the general case, rather than modelling the set $\mathcal { G }$ of information as a new mathematical structure, we simply identify $\mathcal { G }$ with the collection of all G-measurable events. Notice that, assuming that the conditional probability $\mathbb { P } ( \cdot | \mathcal { G } )$ somehow behaves like an unconditional probability, then $\mathcal { G }$ is a sigma-field. The lesson of all of this is that it makes sense to model information as a sub-sigma-field of the sigma-field of all events ${ \mathcal F } .$ . It remains to properly define the conditional probability and then check that it has the correct properties. 

We briefly recall some notions from probability. 

Definition. Given a probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ , let ${ \mathcal { G } } \subseteq { \mathcal { F } }$ be a sub-sigma-field of events. A random variable $X : \Omega  \mathbb { R }$ is measurable with respect to $\mathcal { G } \ ( $ ( or briefly, $\mathcal { G } _ { - }$ measurable) if and only if the event $\{ X \leq x \}$ is an element of $\mathcal { G }$ for all $x \in \mathbb { R }$ 

You know what that the conditional expectation of an integrable random variable X given a non-null event $G$ means 

$$
\mathbb {E} (X | G) = \frac {\mathbb {E} (X \mathbb {1} _ {G})}{\mathbb {P} (G)}
$$

The next theorem leads to a definition of conditional expectation given a sigma-field: 

Theorem (Existence and uniqueness of conditional expectations). Let X be an integrable random variable defined on the probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ , and let ${ \mathcal { G } } \subseteq { \mathcal { F } }$ be a sub-sigma-field of $\mathcal { F }$ . Then there exists an integrable G-measurable random variable Y such that 

$$
\mathbb {E} (\mathbb {1} _ {G} Y) = \mathbb {E} (\mathbb {1} _ {G} X)
$$

for all $G \in { \mathcal { G } }$ . Furthermore, if there exists another G-measurable random variable $Y ^ { \prime }$ such that $\mathbb { E } ( \mathbb { 1 } _ { G } Y ^ { \prime } ) = \mathbb { E } ( \mathbb { 1 } _ { G } X )$ for all $G \in { \mathcal { G } }$ , then $Y = Y ^ { \prime }$ almost surely. 

Definition. Let X be an integrable random variable and let ${ \mathcal { G } } \subseteq { \mathcal { F } }$ be a sigma-field. The conditional expectation of X given $\mathcal { G }$ , written $\mathbb { E } ( X | \mathcal { G } )$ , is a $\mathcal { G }$ -measurable random variable with the property that 

$$
\mathbb {E} \left[ \mathbb {1} _ {G} \mathbb {E} (X | \mathcal {G}) \right] = \mathbb {E} (\mathbb {1} _ {G} X)
$$

for all $G \in { \mathcal { G } }$ 

Example. (Sigma-field generated by a countable partition) Let X be a non-negative random variable defined on $( \Omega , \mathcal { F } , \mathbb { P } )$ . Let $G _ { 1 } , G _ { 2 } , . . .$ . be a sequence of disjoint events with $\mathbb { P } ( G _ { n } ) > 0$ for all n and $\textstyle \bigcup _ { n \in \mathbb { N } } G _ { n } = \Omega$ 

Let G be the smallest sigma-field containing $\left\{ G _ { 1 } , G _ { 2 } , \dots , \dots \right\}$ . That is, every element of $\mathcal { G }$ is of the form $\textstyle \bigcup _ { n \in I } G _ { n }$ where $I \subseteq \mathbb { N }$ . Then 

$$
\mathbb {E} (X | \mathcal {G}) (\omega) = \mathbb {E} (X | G _ {n}) = \frac {\mathbb {E} (X \mathbb {1} _ {G _ {n}})}{\mathbb {P} (G _ {n})} \text {   if   } \omega \in G _ {n}
$$

where the right-hand side denotes conditional expectation given the event $G _ { n }$ 

More concretely, suppose $\Omega = \{ H H , H T , T H , T T \}$ consists of two tosses of a fair coin, and let $\mathcal { G } = \{ \emptyset , \{ H H , H T \} , \{ T H , T T \} , \Omega \}$ be the sigma-field containing the information revealed by the first toss. Consider the random variable 

$$
X (\omega) = \left\{ \begin{array}{l l} a & \text {if} \omega = H H \\ b & \text {if} \omega = H T \\ c & \text {if} \omega = T H \\ d & \text {if} \omega = T T. \end{array} \right.
$$

Then 

$$
\mathbb {E} (X | \mathcal {G}) (\omega) = \left\{ \begin{array}{l l} (a + b) / 2 & \text {if} \omega \in \{H H, H T \} \\ (c + d) / 2 & \text {if} \omega \in \{T H, T T \} \end{array} \right.
$$

The important properties of conditional expectations are collected below: 

Theorem. Let all random variables appearing below be such that the relevant conditional expectations are defined, and let G be a sub-sigma-field of the sigma-field F of all events. 

• linearity: $\mathbb { E } ( a X + b Y | \mathcal { G } ) = a \mathbb { E } ( X | \mathcal { G } ) + b \mathbb { E } ( Y | \mathcal { G } )$ for all constants a and b 

• positivity: If $X \geq 0$ almost surely, then $\mathbb { E } ( X | \mathcal { G } ) \geq 0$ almost surely. 

• Jensen’s inequality: If f is convex, then $\mathbb { E } [ f ( X ) | { \mathcal { G } } ] \geq f [ \mathbb { E } ( X | { \mathcal { G } } ) ]$ 

• monotone convergence theorem: I $f 0 \leq X _ { n } \uparrow X \ a . s .$ then $\mathbb { E } ( X _ { n } | \mathcal { G } ) \uparrow \mathbb { E } ( X | \mathcal { G } ) \ a . s .$ 

• Fatou’s lemma: $I f X _ { n } \geq 0 \ a . s .$ . for all n, then E(lim $\operatorname { i n f } _ { n } X _ { n } | { \mathcal { G } } ) \leq$ lim in $\mathbb { f } _ { n } \mathbb { E } ( X _ { n } | \mathcal { G } )$ 

• dominated convergence theorem: If $\operatorname { s u p } _ { n } \left| X _ { n } \right|$ is integrable and $X _ { n }  X \ a . s .$ . then $\mathbb { E } ( X _ { n } | \mathcal { G } )  \mathbb { E } ( X | \mathcal { G } ) ~ a . s .$ 

$I f X$ is independent of G (the events $\{ X \leq x \}$ and G are independent for each $x \in \mathbb { R }$ and $G \in { \mathcal { G } } )$ then $\mathbb { E } ( X | { \mathcal { G } } ) = \mathbb { E } ( X )$ . In particular, $\mathbb { E } ( X | { \mathcal { G } } ) = \mathbb { E } ( X )$ if G is trivial. 

• ‘slot property’: If X is G-measurable, then $\mathbb { E } ( X Y | \mathcal { G } ) \stackrel { \cdot } { = } X \mathbb { E } ( Y | \mathcal { G } )$ . In particular, if X is G-measurable, then $\mathbb { E } ( X | { \mathcal { G } } ) = X$ 

• tower property or law of iterated expectations: $I f \mathcal { H } \subseteq \mathcal { G }$ then 

$$
\mathbb {E} [ \mathbb {E} (X | \mathcal {G}) | \mathcal {H} ] = \mathbb {E} [ \mathbb {E} (X | \mathcal {H}) | \mathcal {G} ] = \mathbb {E} (X | \mathcal {H})
$$

Definition. The conditional probability of an event $A \in { \mathcal { F } }$ given a sub-sigma-field G is defined by 

$$
\mathbb {P} (A | \mathcal {G}) = \mathbb {E} (\mathbb {1} _ {A} | \mathcal {G}).
$$

We now come full circle to show that the motivation for defining measurability is compatible with the definitions we have chosen: 

Proposition. $I f \mathbb { P } ( A | \mathcal { G } ) \in \{ 0 , 1 \}$ almost surely, then there exists a $\mathcal { G }$ -measurable event $A ^ { \prime }$ such that $\mathbb { P } ( A \backslash A ^ { \prime } ) = \dot { 0 } = \mathbb { P } ( \dot { A ^ { \prime } } \backslash A )$ 

Proof. Since the conditional probability takes values in {0, 1} there exists a ${ \mathcal { G } } .$ -measurable event A<sup>0</sup> such that 

$$
\mathbb {P} (A | \mathcal {G}) = \mathbb {1} _ {A ^ {\prime}}.
$$

Note that 

$$
\begin{array}{r l} \mathbb {P} (A) = & \mathbb {E} (\mathbb {1} _ {A}) \\ = & \mathbb {E} [ \mathbb {E} (\mathbb {1} _ {A} | \mathcal {G}) ] \qquad \text { tower } \\ = & \mathbb {E} [ \mathbb {1} _ {A ^ {\prime}} ] \\ = & \mathbb {P} (A ^ {\prime}) \end{array}
$$

and 

$$
\begin{array}{l l} \mathbb {P} (A \cap A ^ {\prime}) = \mathbb {E} (\mathbb {1} _ {A} \mathbb {1} _ {A ^ {\prime}}) \\ \qquad = \mathbb {E} [ \mathbb {E} (\mathbb {1} _ {A} \mathbb {1} _ {A ^ {\prime}} | \mathcal {G}) ] & \text {tower} \\ \qquad = \mathbb {E} [ \mathbb {1} _ {A ^ {\prime}} \mathbb {E} (\mathbb {1} _ {A} | \mathcal {G}) ] & \text {slot} \\ \qquad = \mathbb {E} [ \mathbb {1} _ {A ^ {\prime}} ^ {2} ] \\ \qquad = \mathbb {P} (A ^ {\prime}) \end{array}
$$

and hence 

$$
\mathbb {E} [ (\mathbb {1} _ {A} - \mathbb {1} _ {A ^ {\prime}}) ^ {2} ] = \mathbb {P} (A) + \mathbb {P} (A ^ {\prime}) - 2 \mathbb {P} (A \cap A ^ {\prime}) = 0.
$$

Continuing with the theme of measurability, we introduce a few more terms: 

Definition. A filtration $\mathbb { F } = ( \mathcal { F } _ { t } ) _ { t \geq 0 }$ on the probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ is a collection of sigma-fields such that $\mathcal { F } _ { s } \subseteq \mathcal { F } _ { t } \subseteq \mathcal { F }$ for all $0 \leq s \leq t$ 

Definition. A process $X = ( X _ { t } ) _ { t \geq 0 }$ is adapted to $\mathbb { F }$ if the random variable $X _ { t }$ is $\mathcal { F } _ { t ^ { - } }$ measurable for all $t \geq 0$ 

When discussing an adapted stochastic process but a filtration is not explicitly mentioned, then we are implicitly working with the natural filtration of the process. 

Definition. Given a stochastic process $X = ( X _ { t } ) _ { t \geq 0 }$ , the natural filtration of X, (or the filtration generated by X) is the smallest filtration for which X is adapted. That is, it is the filtration $( \mathcal { F } _ { t } ) _ { t \geq 0 }$ where 

$$
\mathcal {F} _ {t} = \sigma (X _ {s}, 0 \leq s \leq t).
$$

To gain some intuition about these definitions, consider this example. 

Example. Return to the experiment of tossing a fair coin two times. The flow of information is modelled by the following sigma-fields 

$$
\mathcal {F} _ {0} = \{\emptyset , \Omega \},
$$

$$
\bullet \mathcal {F} _ {1} = \{\emptyset , \{H H, H T \}, \{T H, T T \}, \Omega \},
$$

${ \mathcal { F } } _ { 2 } = { \mathcal { F } } .$ 

Now consider a stochastic process $( X _ { t } ) _ { t \in \{ 0 , 1 , 2 \} }$ that is adapted to the filtration $( \mathcal { F } _ { t } ) _ { t \in \{ 0 , 1 , 2 \} }$ Intuitively, the value of the random variable $X _ { t }$ is known once after t tosses of the coin. 

For instance, $X _ { 0 }$ must be a constant, 

$$
X _ {0} (\omega) = a \text {   for   all   } \omega \in \Omega ,
$$

since there is no information before the experiment. On the other hand, the random variable $X _ { 1 }$ must be of the form 

$$
X _ {1} (\omega) = \left\{ \begin{array}{l l} b & \text { if } \omega \in \{H H, H T \} \\ c & \text { if } \omega \in \{T H, T T \} \end{array} \right.
$$

since the only information known at time 1 is whether or not the first coin came up heads. Finally, $X _ { 2 }$ can be any function on $\Omega _ { ; }$ , that is, of the form 

$$
X _ {2} (\omega) = \left\{ \begin{array}{l l} d & \text {if} \omega = H H \\ e & \text {if} \omega = H T \\ f & \text {if} \omega = T H \\ g & \text {if} \omega = T T. \end{array} \right.
$$

Alternatively, on this particular filtered probability space, the adapted process $X$ can be visualised by the tree diagram: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/6904b2c02d24e520804b3cab7529491a9d4f0bdab22718b49d45eb5afe7e5850.jpg)


Notice that for all $t \in \{ 0 , 1 , 2 \}$ the event $\{ X _ { t } \leq x \}$ is in $\mathcal { F } _ { t }$ for every real x. 

For this course, it will be convenient to assume that there is no randomness at time 0. This can be made formal by assuming 

$$
\mathrm{thesigma-field} \mathcal {F} _ {0} \mathrm{istrivial}.
$$

This means that if A is an element $\mathcal { F } _ { 0 }$ then either $\mathbb { P } ( A ) = 0 { \mathrm { ~ o r ~ } } \mathbb { P } ( A ) = 1$ . In particular, every $\mathcal { F } _ { 0 } .$ -measurable random variable is almost surely constant. In the discrete-time theory, there nothing loss by further assuming ${ \mathcal { F } } _ { 0 } = \{ \emptyset , \Omega \}$ . However, it turns out that this further assumption is technically inconvenient in the continuous-time theory. 

Before continuing to the financial models, we list one final definition in this section. 

Definition. A discrete-time process $X = ( X _ { t } ) _ { t \geq 1 }$ is previsible (or predictable) if the random variable $X _ { t }$ is $\mathcal { F } _ { t - 1 }$ -measurable for all $t \geq 1$ 

Remark. Note that the time index set for a previsible process $( X _ { t } ) _ { t \geq 1 }$ is (usually) $\{ 1 , 2 , \ldots \}$ , not $\{ 0 , 1 , \ldots \}$ . In particular, $X _ { 0 }$ is not necessarily defined. 

Remark. In discrete time, a process $X$ is previsible if and only if the process $Y$ is adapted, where $X _ { t } = Y _ { t - 1 }$ . That is to say, the notion of previsibility can be dispensed with by simply changing notation. However, in continuous time, there is a more subtle diference between the notions of previsibility and adaptedness. Therefore, for the sake of a unified treatment of the discrete and continuous time cases, we keep it in. 

## 2. The set-up

Returning to our financial modelling, we assume that the market prices are given by a n-dimensional adapted process $P = ( P _ { t } ) _ { t > 0 }$ . For the moment, we assume that each asset may pay a dividend. Let $\delta _ { t } ^ { i }$ be the dividend paid for each share of asset i held at time t. We assume that $( \delta _ { t } ) _ { t \geq 1 }$ is an adapted process. Note that we start time at $t = 1$ for this process - the reason will be come clear shortly. Also, recall from the preface that for most of the rest of the course we will assume that $\delta _ { t } = 0$ almost surely for all $t \geq 1$ . But to be clear, we do not make that assumption now. 

To the market described by the adapted processes $P$ and $\delta ,$ we now introduce an investor. At time $t ,$ the investor comes into the market with an initial amount of money $X _ { t }$ . The investor receives some income $I _ { t }$ and consumes some amount $C _ { t }$ 

With the remaining money $X _ { t } + I _ { t } - C _ { t }$ , the investor buys a portfolio $H _ { t + t } \in \mathbb { R } ^ { n }$ of the assets, where the real number $H _ { t + 1 } ^ { i }$ denotes the number of shares held in asset $i . \ ( \mathrm { I f \ } H _ { t + 1 } ^ { i } > 0$ then the position is said to be long, and if $H _ { t + 1 } ^ { i } < 0$ then the position is said to be short.) 

There are two important accounting relationships between the variables. First, the budget constraint is 

$$
X _ {t} + I _ {t} - C _ {t} = H _ {t + 1} \cdot P _ {t},
$$

where we are using the notation 

$$
a \cdot b = \sum_ {i = 1} ^ {n} a ^ {i} b ^ {i}
$$

for the usual Euclidean inner (or dot) product in $\mathbb { R } ^ { n }$ . Second, at time $t + 1$ , the investor’s portfolio is worth $X _ { t + 1 } = H _ { t + 1 } \cdot ( P _ { t + t } + \delta _ { t + 1 } )$ 

Second, we have the accounting identity 

$$
X _ {t + 1} = H _ {t + 1} \cdot (P _ {t + 1} + \delta_ {t + 1})
$$

which says that the amount of money the investor has in the market at time $t + 1$ is equal to the sum of liquidation value of the assets and the accrued dividends. 

We will model the price process $P _ { \mathrm { : } }$ , the dividend process $\delta$ and external income process I as exogenously given adapted processes. We consider the investor’s initial wealth $X _ { 0 } = x$ as a given constraint, and the investor’s portfolio process $( H _ { t } ) _ { t \geq 1 }$ as her control. In order to eliminate clairvoyant investors, we insist that the control H is previsibile. 

Note that given x and $H$ , the investor’s wealth is 

$$
X _ {t} ^ {x, H} = \left\{ \begin{array}{l l} x & \text { if } t = 0 \\ H _ {t} \cdot (P _ {t} + \delta_ {t}) & \text { if } t \geq 1 \end{array} \right.
$$

and the consumption is then 

$$
C _ {t} ^ {x, H} = X _ {t} ^ {x, H} + I _ {t} - H _ {t + 1} \cdot P _ {t}.
$$

Now that we have our market model and we’ve introduced an investor into this market, our first challenge is to find out how to invest optimally. We consider one such optimal investment problem. The main motivation for studying this problem is to introduce the very important notion of a martingale deflator. 

Let $T > 0$ be some non-random time horizon and prefers a consumption stream $c =$ $( c _ { t } ) _ { 0 \leq t \leq T }$ to $c ^ { \prime } = ( c _ { t } ^ { \prime } ) _ { 0 \leq t \leq T }$ if and only if 

$$
\mathbb {E} [ U (c) ] > \mathbb {E} [ U (c ^ {\prime}) ]
$$

where $U : \mathbb { R } ^ { 1 + T }  \mathbb { R } \cup \{ - \infty \}$ is a given utility function. We will assume that $c _ { t } \mapsto$ $U ( c _ { 0 } , \ldots , c _ { T } )$ is strictly increasing for each t, modelling the assumption that the investor strictly prefers more to less. (Usually we also assume that $U$ is strictly concave, so that the investor is risk-averse, strictly preferring to consume the non-random quantity $\mathbb { E } ( c )$ to the random quantity $c ,$ for any non-constant random vector $c . )$ 

We suppose that investor’s initial wealth is x given. We also suppose that he will live exactly to age $T ,$ and since he derives no utility from wealth in the afterlife, chooses to consume his remaining wealth at time $T .$ Summing up, the investor faces the problem 

maximise E[U(c)] subject to $\left\{ \begin{array} { l l } { c _ { t } = C _ { t } ^ { x , H } \mathrm { ~ f o r ~ } 0 \leq t \leq T } \\ { c _ { T } = H _ { T } \cdot ( P _ { T } + \delta _ { T } ) + I _ { T } } \end{array} \right.$ 

With this problem in mind, we introduce an important definition: 

With this problem in mind, we introduce an important definition: 

Definition. An arbitrage is an n-dimensional previsible process H such that there exists a non-random time $T > 0$ with the properties, that the consumption stream 

$$
\begin{array}{l} c _ {0} = - H _ {1} \cdot P _ {0}, \\ c _ {t} = H _ {t} \cdot (P _ {t} + \delta_ {t}) - H _ {t + 1} \cdot P _ {t}, \text { for } 1 \leq t \leq T - 1, \\ c _ {T} = H _ {T} \cdot (P _ {T} + \delta_ {T}) \end{array}
$$

satisfies 

$c _ { t } \geq 0$ almost surely for all $0 \leq t \leq T$ 

$\mathbb { P } \left( c _ { t } > 0 \right.$ for some $0 \leq t \leq T ) > 0 .$ 

Note that if $H ^ { \mathrm { f } }$ is a feasible investment strategy for the above investment problem and if $H ^ { \mathrm { a } }$ is an arbitrage, then $H ^ { \mathrm { f } } + H ^ { \mathrm { a } }$ is also feasible (since it can be funded with same initial wealth $x )$ . However, the new strategy has strictly higher expected utility 

$$
\mathbb {E} [ U (c ^ {\mathrm{f}} + c ^ {\mathrm{a}}) ] > \mathbb {E} [ U (c ^ {\mathrm{f}}) ].
$$

Inductively, the strategy $H ^ { \mathrm { f } } + k H ^ { \mathrm { a } }$ is feasible for every $k \geq 0$ . In particular, if there is an arbitrage then there cannot be an optimal investment strategy to the utility maximisation problem. 

Aside. And why do we care about the existence of optimal investment strategies? To explain, we take a moment to ask where do prices come from? We consider a one-period model. Assume that that only happens at time 0, so we assign the terminal price vector 

$P _ { 1 } = 0$ . On the other hand, the vector of dividends $\delta _ { 1 }$ is unknown at time 0. It is possibly non-zero, but since its value is only revealed at time 1, we model it as a random vector. What determines the randomness? One could argue that all that matters is the beliefs of the market participants, not the underlying mechanism that causes the apparent randomness. So, we assume that there are $J$ investors, and each investor $j$ has a probability measure $\mathbb { P } _ { j }$ , where $j = 1 , \dots , J$ modelling the distribution of $\delta _ { 1 }$ . We also assume that each agent $j$ comes to the market with initial capital $x _ { j }$ . The market already has the n assets, with total supply of asset i given by $S ^ { i }$ and $S = ( S ^ { 1 } , \cdot \cdot \cdot , S ^ { n } )$ . The agents trade with each other until each arrive at an optimal allocation $H _ { j } ^ { * }$ and collectively determine an initial price $P _ { 0 } ^ { * }$ . To formalise this, we have the following definition: 

Definition. Given initial wealths $x _ { j }$ , utility functions $U _ { j }$ and probability measures $\mathbb { P } _ { j }$ for $j = 1 , \dots J$ which determine the distribution of the random vector $P _ { 1 }$ , let 

$$
H _ {j} (p) = \arg \max \{\mathbb {E} _ {j} [ U (c _ {0}, c _ {1}) ]: c _ {0} = x _ {j} - H \cdot p, c _ {1} = H \cdot \delta_ {1} \}
$$

be the optimal portfolio for agent i assuming the initial price is $P _ { 0 } = p$ . An equilibrium price $P _ { 0 } ^ { * }$ is a solution to the equation 

$$
\sum_ {j = 1} ^ {J} H _ {j} (P _ {0} ^ {*}) = S,
$$

where the notation $\mathbb { E } _ { j }$ denotes expectation with respect to $\mathbb { P } _ { j }$ . 

Note that the above condition says that for the equilibrium initial price $P _ { 0 } ^ { * }$ , the agents portfolios $H _ { j } ^ { * }$ solve their version of the optimal investment problem (*). A consequence of the previous proposition is the following motivating result: 

Proposition. If the market is in equilibrium then no agent can believe there is an arbitrage. 

Before proceeding, we consider a simple consequence of the assumption of no arbitrage in a market model. 

Proposition. Consider a market with $n = 1$ asset, and assume that $\delta _ { t } ~ \geq ~ 0$ almost surely for all $t \geq 1$ . If there exists a non-random $T > 0$ such that $P _ { T } \ge 0$ almost surely, then $P _ { t } \geq 0$ almost surely for all $0 \leq t \leq T$ 

Proof. Let $\tau = \operatorname* { i n f } \{ t \geq 0 : P _ { t } < 0 \}$ and let 

$$
H _ {t} = \mathbb {1} _ {\{\tau <   t \leq T \}}
$$

Note that H is previsible since for $1 \leq t \leq T$ we have 

$$
\{\tau <   t \} = \cup_ {s = 0} ^ {t - 1} \{P _ {s} <   0 \} \in \mathcal {F} _ {t - 1}.
$$

Hence $c _ { t } = - P _ { t } > 0$ on $\{ t = \tau < T \}$ and $c _ { T } = P _ { T } + \delta _ { T } \ge 0$ . Since there is no arbitrage, we must have $\mathbb { P } ( \tau < T ) = 0$ , or equivalently, $\mathbb { P } ( P _ { s } \ge 0$ for all $0 \leq s \leq T - 1 ) = 1$ as claimed.  

## 3. The first fundamental theorem and martingales

We have tried to argue above that it is natural to insist that our market model is free of arbitrage strategies. But how can we check that a given price process P is arbitrage free? The answer is contained in a famous theorem: 

Theorem (First fundamental theorem of asset pricing). A market model has no arbitrage if and only if there exists a martingale deflator. 

We spend the next few pages unpacking this theorem. First, we need a definition to get started: 

Definition. A martingale deflator is an adapted (real-valued) process $Y$ such that $Y _ { t } > 0$ for all $t \geq 0$ almost surely, and such that the n-dimensional process 

$$
M _ {t} = P _ {t} Y _ {t} + \sum_ {s = 1} ^ {t} \delta_ {s} Y _ {s}
$$

is a martingale. 

We now briefly review some bits of martingale theory. 

***** 

Now we come to one of the most important concepts in financial mathematics, the martingale. A martingale is simply an adapted stochastic process that is constant on average in the following sense: 

Definition. A martingale relative to a filtration $\mathbb { F }$ is an adapted stochastic process $M = ( M _ { t } ) _ { t \geq 0 }$ with the following properties: 

$\mathbb { E } ( | M _ { t } | ) < \infty$ for all $t \geq 0$ 

$\mathbb { E } ( M _ { t } | \mathcal { F } _ { s } ) = M _ { s }$ for all 0 ≤ s ≤ t. 

Remark. The above definition of martingale is the same both discrete- and continuoustime processes. However, if the time index set is discrete $\mathbb { T } = \mathbb { Z } _ { + }$ , it is an exercise to show that an integrable process M is a martingale only if $\mathbb { E } ( M _ { t + 1 } | \mathcal { F } _ { t } ) = M _ { t }$ for all $t \geq 0$ . That is, it is suficient to verify the conditional expectations of the process one period ahead. 

Below are some examples of martingales. 

Example. Let $\xi _ { 1 } , \xi _ { 2 } , \xi _ { 3 } , . . .$ . be independent integrable random variables such that $\mathbb { E } ( \xi _ { i } ) =$ 0 for all i. The process $( S _ { t } ) _ { t \geq 0 }$ given by $S _ { 0 } = 0$ and 

$$
S _ {t} = \xi_ {1} + \ldots + \xi_ {t}
$$

is a martingale relative to its natural filtration. Indeed, the random variable $S _ { t }$ is integrable since 

$$
\mathbb {E} (| S _ {t} |) \leq \mathbb {E} (| \xi_ {1} |) + \dots + \mathbb {E} (| \xi_ {t} |)
$$

by the triangular inequality and all the terms in this finite sum are finite by assumption. Also, 

$$
\begin{array}{r c l} \mathbb {E} (S _ {t + 1} | \mathcal {F} _ {t}) & = & \mathbb {E} (S _ {t} + \xi_ {t + 1} | \mathcal {F} _ {t}) \\ & = & \mathbb {E} (S _ {t} | \mathcal {F} _ {t}) + \mathbb {E} (\xi_ {t + 1} | \mathcal {F} _ {t}) \\ & = & S _ {t} + \mathbb {E} (\xi_ {t + 1}) = S _ {t}, \end{array}
$$

where the conditional expectation $\mathbb { E } ( \xi _ { t + 1 } | \mathcal { F } _ { t } )$ is replaced by the unconditional expectation $\mathbb { E } ( \xi _ { t + 1 } )$ by the assumption that $\xi _ { t + 1 }$ is independent of $\mathcal { F } _ { t } = \sigma ( S _ { 1 } , \ldots , S _ { t } ) = \sigma ( \xi _ { 1 } , \ldots , \xi _ { t } )$ 

Example. We now construct one of the most important examples of a martingale. Let X be an integrable random variable, and let 

$$
M _ {t} = \mathbb {E} (X | \mathcal {F} _ {t}).
$$

Then $M = ( M _ { t } ) _ { t \geq 0 }$ is a martingale. 

Integrability follows from the definition of conditional expectation. Now, for every $0 \leq$ $s \leq t$ we have 

$$
\begin{array}{r c l} \mathbb {E} (M _ {t} | \mathcal {F} _ {s}) & = & \mathbb {E} [ \mathbb {E} (X | \mathcal {F} _ {t}) | \mathcal {F} _ {s} ] \\ & = & \mathbb {E} (X | \mathcal {F} _ {s}) = M _ {s} \end{array}
$$

by the tower property. Notice that this example also works in continuous time. 

Sometimes we are given a process $( M _ { t } ) _ { 0 \leq t \leq T }$ where $T > 0$ is a fixed, non-random time horizon. To check that this process is a martingale, we need only check that 

$$
M _ {t} = \mathbb {E} (M _ {T} | \mathcal {F} _ {t}) \text {   for   all   } 0 \leq t \leq T,
$$

because this corresponds to the construction above with $X = M _ { T }$ 

This last example is theorem shows how to take one martingale and build another one. 

Proposition. Let M be a martingale and let K be a bounded predictable process. Then the process X defined by 

$$
X _ {t} = \sum_ {s = 1} ^ {t} K _ {s} (M _ {s} - M _ {s - 1})
$$

is a martingale. 

Proof. First, note $X _ { t }$ is F -measurable by construction. Also, by assumption, we have $\mathbb { E } ( | M _ { t } | ) < \infty$ for all t since M is a martingale and that there exist a constant $C > 0$ such that $| K _ { t } | \le C$ almost surely for all $t \geq 0$ . Hence 

$$
\begin{array}{r c l} \mathbb {E} (| X _ {t} |) & \leq & \sum_ {s = 1} ^ {t} \mathbb {E} (| K _ {s} | | M _ {s} - M _ {s - 1} |) \\ & \leq & \sum_ {s = 1} ^ {t} C [ \mathbb {E} (| M _ {s} |) + \mathbb {E} (| M _ {s - 1} |) ] <   \infty \end{array}
$$

Using the predictability of K and the slot property of conditional expectation, we have 

$$
\begin{array}{c} \mathbb {E} (X _ {t + 1} - X _ {t} | \mathcal {F} _ {t}) = \mathbb {E} (K _ {t + 1} (M _ {t + 1} - M _ {t}) | \mathcal {F} _ {t}) \\ = K _ {t + 1} \mathbb {E} (M _ {t + 1} - M _ {t} | \mathcal {F} _ {t}) \\ = 0 \end{array}
$$

implying the martingale property $\mathbb { E } ( X _ { t + 1 } | \mathcal { F } _ { t } ) = X _ { t }$ , since $X _ { t }$ is $\mathcal { F } _ { t } .$ -measurable.  

Remark. The martingale X above is often called a martingale transform or a discrete time stochastic integral. $\mathrm { A s }$ we will see, it is one of the key building blocks for the continuous time theory to come. 

## 4. Local martingales

It turns out that to prove the 1FTAP, even in the easy direction, we need a little more technology. 

With that introduction, we begin our study of local martingales. First we start with a definition. 

Definition. A stopping time for a filtration $( \mathcal { F } _ { t } ) _ { t \in \mathbb { T } }$ is a random variable $\tau$ taking values in $\mathbb { T } \cup \{ \infty \}$ such that the event $\{ \tau \leq t \}$ is F -measurable for all $t \in \mathbb { T }$ 

Example. Obviously, non-random times are stopping times. That is, if $\tau = t _ { 0 }$ for some fixed $t _ { 0 } \geq 0$ , then $\{ \tau \leq t \} = \Omega { \mathrm { ~ i f ~ } } t _ { 0 } \leq t$ and ∅ otherwise. 

Example. Here is a typical example of a stopping time. Let $( Y _ { t } ) _ { t \geq 0 }$ be a discrete-time adapted process and let A be a Borel set (for instance, an interval). Then the random variable 

$$
\tau = \inf \{t \geq 0: Y _ {t} \in A \}
$$

(with the usual convention that inf $\varnothing = + \infty )$ corresponding to the first time the process enters the set A is a stopping time. Indeed, 

$$
\{\tau \leq t \} = \bigcup_ {s = 0} ^ {t} \{Y _ {s} \in A \}
$$

is $\mathcal { F } _ { t }$ -measurable because each $\{ Y _ { s } \in A \}$ is $\mathcal { F } _ { s } { \mathrm { - m e a s u r a b l e } }$ by the adaptedness of $Y$ , and $\mathcal { F } _ { s } \subseteq \mathcal { F } _ { t }$ by the definition of filtration. 

Stopping times can be used to stop processes. 

Definition. For an adapted process X (in discrete or continuous<sup>1</sup> time) and a stopping time $\tau ,$ the process $X ^ { \tau }$ defined by $X _ { t } ^ { \tau } = X _ { t \wedge \tau }$ is said to be X stopped at $\tau .$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/09f1805b1f74568c14b63d13ae6564e7fd19df766707c59d52d72809e45a056a.jpg)



Stopping times interact well martingales: stopped martingales are still martingales.


Proposition. Let X be a discrete-time martingale and let τ be a stopping time. Then $X ^ { \tau }$ is a martingale. 

Remark. A version of this theorem also holds for continuous-time martingales with continuous sample paths. 

Proof. Note that 

$$
X _ {t} ^ {\tau} = X _ {0} + \sum_ {s = 1} ^ {t} \mathbb {1} _ {\{s \leq \tau \}} (X _ {s} - X _ {s - 1}).
$$

Since the event $\{ t \leq \tau \} = \{ \tau \leq t - 1 \} ^ { c }$ is $\mathcal { F } _ { t - 1 }$ -measurable by the definition of stopping time, the process $K _ { t } = \mathbb { 1 } _ { \{ t \leq \tau \} }$ is predictable. Since $X ^ { \tau }$ is the martingale transform of the bounded predictable process K with respect to the martingale $X$ , it is a martingale.  

The above result says that the martingale property is stable under stopping. We use this property as motivation for the following definition. 

Definition. A local martingale is an adapted process $X = ( X _ { t } ) _ { t \geq 0 }$ , in either discrete or continuous time, such that there exists an increasing sequence of stopping times $\left( \tau _ { N } \right)$ with $\tau _ { N }$ ↑ ∞ such that the stopped process $X ^ { \tau _ { N } }$ is a martingale for each $N$ 

Remark. Note that martingales are local martingales. Indeed, given a martingale X and any sequence of stopping times $\tau _ { N } \uparrow \infty$ , the stopped process $X ^ { \tau _ { N } }$ is a martingale. 

Remark. Note that the local martingale property is also stable under stopping. Indeed, let X be a local martingale and τ a stopping time. Then by definition, there exists a sequence of stopping times $\sigma _ { N }$ ↑ ∞ such that $X ^ { \sigma _ { N } }$ is a martingale. Hence $( X ^ { \sigma _ { N } } ) ^ { \tau } = X ^ { \sigma _ { N } \wedge \tau }$ is again a martingale since $\sigma _ { N } \wedge \tau$ is a stopping time. But note that $X ^ { \sigma _ { N } \wedge \tau } = ( X ^ { \tau } ) ^ { \sigma _ { N } }$ , implying that the sequence of stopping times $\sigma _ { N } \uparrow \infty$ is such that $( X ^ { \tau } ) ^ { \sigma _ { N } }$ is a martingale. This means $X ^ { \tau }$ is a local martingale. 

Theorem. Suppose M is a discrete-time local martingale and K is a predictable process. Let 

$$
X _ {t} = \sum_ {s = 1} ^ {t} K _ {s} (M _ {s} - M _ {s - 1})
$$

for $t \geq 1$ . Then X is a local martingale. 

Remark. This is the martingale transform as before, but now do not insist that K is bounded or that M is a true martingale. As a consequence, we cannot assert that X is a true martingale, merely a local martingale. The idea is that by localising, we can study the algebraic and measurability structure of the martingale transform without worrying about integrability issues. 

Proof. Since M is a local martingale by assumption, there exists a sequence of stopping times $( \tau _ { n } ) _ { r }$ with $\tau _ { n } \uparrow \infty \mathrm { a . s }$ . such that $M ^ { \tau _ { n } }$ is a martingale. 

Let $u _ { n } = \operatorname* { i n f } \{ t \geq 0 : | K _ { t + 1 } | > n \}$ with the convention inf $\varnothing = + \infty$ . Note that since K is predictable we have 

$$
\left\{u _ {n} \leq t - 1 \right\} ^ {c} = \left\{u _ {n} \geq t \right\} = \left\{\left| K _ {s} \right| \leq n \text {for all} 0 \leq s \leq t \right\} \in \mathcal {F} _ {t - 1}
$$

and hence that $u _ { n }$ is a stopping time with $u _ { n } \uparrow \infty . ^ { 2 }$ 

Finally, let $v _ { n } = \tau _ { n } \wedge u _ { n }$ . Note $v _ { n }$ ↑ ∞ and $v _ { n }$ is a stopping time since $\{ v _ { n } \leq t \} = \{ \tau _ { n } \leq$ $t \} \cup \{ u _ { n } \leq t \}$ 

Now $M ^ { v _ { n } } = ( M ^ { \tau _ { n } } ) ^ { u _ { n } }$ is a stopped martingale, and hence a martingale. Also $( K _ { t } \mathbb { 1 } _ { \{ t \leq v _ { n } \} } ) _ { t \geq 1 }$ is a predictable process, bounded by n. Writing 

$$
X _ {t} ^ {v _ {n}} = \sum_ {s = 1} ^ {t} K _ {s} \mathbb {1} _ {\{s \leq v _ {n} \}} (M _ {s} ^ {v _ {n}} - M _ {s - 1} ^ {v _ {n}})
$$

we see that the stopped process is the martingale transform of a bounded predictable process with respect to the martingale, and hence is a martingale.  

The next theorem gives a suficient condition that a local martingale is a true martingale. 

Theorem. Let X be a local martingale in either discrete or continuous time. Let $Y _ { t }$ be a process such that $| X _ { s } | \le Y _ { t }$ almost surely for all $0 \leq s \leq t$ . If $\mathbb { E } ( Y _ { t } ) < \infty$ for all $t \geq 0$ then X is a true martingale. 

Proof. Let $( \tau _ { N } ) _ { N }$ be a localising sequence of stopping times for X. Note that $X _ { t \wedge \tau _ { N } } $ $X _ { t } \ \mathrm { a . s }$ . since $\tau _ { N } \uparrow \infty$ . Furthermore, by assumption $| X _ { t \wedge \tau _ { N } } | \leq Y _ { t }$ which is integrable, so we may apply the conditional version of the dominated convergence theorem to conclude 

$$
\begin{array}{r l} & {\mathbb {E} (X _ {t} | \mathcal {F} _ {s}) = \mathbb {E} (\lim _ {N} X _ {t \wedge \tau_ {N}} | \mathcal {F} _ {s})} \\ & {\quad = \lim _ {N} \mathbb {E} (X _ {t \wedge \tau_ {N}} | \mathcal {F} _ {s})} \\ & {\quad = \lim _ {N} X _ {s \wedge \tau_ {N}}} \\ & {\quad = X _ {s}} \end{array}
$$

for $0 \leq s \leq t$ , where we have used the fact that the stopped process $( X _ { t \wedge \tau _ { N } } ) _ { t \geq 0 }$ is a martingale. 

The following corollary is useful: 

Corollary. Suppose X is a DISCRETE-TIME local martingale such that $\mathbb { E } ( | X _ { t } | ) < \infty$ for all $t \geq 0$ . Then X is a true martingale. 

Proof. Let $Y _ { t } = | X _ { 0 } | + \ldots + | X _ { t } |$ . The process Y is integrable by assumption and $| X _ { s } | \le Y _ { t }$ for all $0 \leq s \leq t$ . The conclusion follows from the previous theorem.  

In the absence of integrability, the next best property is non-negativity. First we need some definitions. 

Definition. A supermartingale relative to a filtration $( \mathcal { F } _ { t } ) _ { t \geq 0 }$ is an adapted stochastic process $( U _ { t } ) _ { t \geq 0 }$ with the following properties: 

$$
\begin{array}{r l} \{\sup _ {n} u _ {n} \geq t \} & = \cup_ {n} \{u _ {n} \geq t \} \\ & = \cup_ {n} \cap_ {s = 1} ^ {t} \{| K _ {s} | \leq n \} \\ & = \{\max _ {1 \leq s \leq t} | K _ {t} | <   \infty \} \end{array}
$$

$\mathbb { E } ( | U _ { t } | ) < \infty$ for all $t \geq 0$ 

$\mathbb { E } ( U _ { t } | \mathcal { F } _ { s } ) \le U _ { s }$ for all $0 \leq s \leq t$ 

A submartingale is an adapted process $( V _ { t } ) _ { t \geq 0 }$ with the following properties: 

$\mathbb { E } ( | V _ { t } | ) < \infty$ for all $t \geq 0$ 

$\mathbb { E } ( V _ { t } | \mathcal { F } _ { s } ) \ge V _ { s }$ for all $0 \leq s \leq t .$ 

Remark. Hence a supermartingale decreases on average, while a submartingale increases on average. A martingale is a stochastic process that is both a supermartingale and a submartingale. 

As in the case of the definition of martingale, to show that an adapted, integrable process U is a supermartingale in discrete time, it is enough to show that $\mathbb { E } ( U _ { t + 1 } | \mathcal { F } _ { t } ) \le U _ { t }$ for all $t \geq 0$ 

Theorem. Suppose X is a local martingale in either continuous or discrete time. If $X _ { t } \geq 0$ for all $t \geq 0$ , then X is a supermartingale. 

Proof. In the general case, let $( \tau _ { N } ) _ { N }$ be the localising sequence for X. First we show that $X _ { t }$ is integrable for each $t \geq 0$ . Fatou’s lemma yields 

$$
\begin{array}{l} \mathbb {E} (| X _ {t} |) = \mathbb {E} (X _ {t}) \\ \qquad = \mathbb {E} (\lim _ {N} X _ {t \wedge \tau_ {N}}) \\ \qquad \leq \operatorname * {l i m i n f} _ {N} \mathbb {E} (X _ {t \wedge \tau_ {N}}) \\ \qquad = X _ {0} <   \infty . \end{array}
$$

Now that we have established integrability, we can discuss conditional expectations. The conditional version of Fatou’s lemma yields 

$$
\begin{array}{l} \mathbb {E} (X _ {t} | \mathcal {F} _ {s}) = \mathbb {E} (\lim _ {N} X _ {t \wedge \tau_ {N}} | \mathcal {F} _ {s}) \\ \qquad \leq \operatorname * {l i m i n f} _ {N} \mathbb {E} (X _ {t \wedge \tau_ {N}} | \mathcal {F} _ {s}) \\ \qquad = \operatorname * {l i m i n f} _ {N} X _ {s \wedge \tau_ {N}} \\ \qquad = X _ {s} \end{array}
$$

for $0 \leq s \leq t ,$ as claimed. 

As before, discrete time local martingales are particularly nice: 

Corollary. If X is a DISCRETE-TIME local martingale such that $X _ { t } \geq 0 \ a . s .$ . for all $t \geq 0$ , then X is a martingale. 

Proof. By the above theorem, we have that $\mathbb { E } ( | X _ { t } | ) = \mathbb { E } ( X _ { t } ) \le X _ { 0 } < \infty$ . Since X is integrable, the previous corollary implies X is a martingale.  

Theorem. Suppose that 

$$
X _ {t} = X _ {0} + \sum_ {s = 1} ^ {t} K _ {s} (M _ {s} - M _ {s - 1})
$$

where K is predictable, X is a martingale and $X _ { 0 }$ is a constant. If $X _ { T } \geq 0 \ a . s .$ . for some non-random $T > 0$ , then $( X _ { t } ) _ { 0 \leq t \leq T }$ is a true martingale. 

Proof. Just as before, let $\tau _ { N } = \operatorname* { i n f } \{ t \geq 0 : | K _ { t + 1 } | > N \}$ . Note $X _ { s } \mathbb { 1 } _ { \{ t \leq \tau _ { N } \} }$ is integrable for all $0 \leq s \leq t$ , since M is integrable by definition of martingale, and $K _ { s }$ is bounded on $\{ t \leq \tau _ { N } \}$ . Hence we have 

$$
\begin{array}{l} 0 \leq \mathbb {E} [ X _ {T} \mathbb {1} _ {\{T \leq \tau_ {N} \}} | \mathcal {F} _ {T - 1} ] \\ = \mathbb {E} [ X _ {T - 1} \mathbb {1} _ {\{T \leq \tau_ {N} \}} + K _ {T} \mathbb {1} _ {\{T \leq \tau_ {N} \}} (M _ {T} - M _ {T - 1}) | \mathcal {F} _ {T - 1} ] \\ = X _ {T - 1} \mathbb {1} _ {\{T \leq \tau_ {N} \}} + K _ {T} \mathbb {1} _ {\{T \leq \tau_ {N} \}} \mathbb {E} [ M _ {T} - M _ {T - 1} | \mathcal {F} _ {T - 1} ] \\ = X _ {T - 1} \mathbb {1} _ {\{T \leq \tau_ {N} \}}. \end{array}
$$

Taking $N  \infty$ shows $X _ { T - 1 } \geq 0 \mathrm { ~ a . s . }$ ., induction shows that $X _ { t } ~ \geq ~ 0$ for all $0 \leq t \leq T$ Therefore $( X _ { t } ) _ { 0 \leq t \leq T }$ is a non-negative local martingale in discrete time and hence a true martingale.  

## 5. Proof of the 1FTAP, easier direction

Recall our framework. There exist n-dimensional price $( P _ { t } ) _ { t \geq 0 }$ and dividend $( \delta _ { t } ) _ { t \geq 1 }$ processes, adapted to a given filtration $( \mathcal { F } _ { t } ) _ { t \geq 0 }$ . A martingale deflator is a positive (real-valued) adapted process $( Y _ { t } ) _ { t \geq 0 }$ such that $Y P$ and Y δ are integrable and 

$$
\mathbb {E} [ Y _ {t + 1} (P _ {t + 1} + \delta_ {t + 1}) | \mathcal {F} _ {t} ] = Y _ {t} P _ {t} \text {   for   all   } t \geq 0.
$$

Our aim is to show that if there exists a martingale deflator, then there is no arbitrage. We first prove a useful lemma. 

Lemma. Given a real constant x and a n-dimensional previsible process $( H _ { t } ) _ { t \geq 1 }$ , let 

$$
\begin{array}{l} X _ {0} = x \\ X _ {t} = H _ {t} \cdot (P _ {t} + \delta_ {t}) f o r t \geq 1, \end{array}
$$

and 

$$
c _ {t} = X _ {t} - H _ {t + 1} \cdot P _ {t} \text { for } t \geq 0.
$$

Suppose there exists a martingale deflator Y . Set 

$$
Z _ {t} = X _ {t} Y _ {t} + \sum_ {s = 0} ^ {t - 1} c _ {s} Y _ {s}.
$$

Then M is a local martingale. Furthermore, if $c _ { t } \geq 0$ a.s for $0 \leq t \leq T - 1$ and $X _ { T } \geq 0$ a.s for some non-random $T > 0$ , then $( M _ { t } ) _ { 0 \leq t \leq T }$ is a martingale. 

Proof. Note that 

$$
\begin{array}{r l} & Z _ {t} - Z _ {t - 1} = X _ {t} Y _ {t} + Y _ {t - 1} (c _ {t - 1} - X _ {t - 1}) \\ & \qquad = H _ {t} \cdot [ Y _ {t} (P _ {t} + \delta_ {t}) - Y _ {t - 1} P _ {t - 1} ] \\ & \qquad = H _ {t} \cdot (M _ {t} - M _ {t - 1}) \end{array}
$$

where 

$$
M _ {t} = P _ {t} Y _ {t} + \sum_ {s = 1} ^ {t} \delta_ {s} Y _ {s}.
$$

Note that Z is martingale transform of the previsible process H with respect to the martingale M, and hence Z is a local martingale. 

Furthermore, if $Z _ { T } ~ \ge ~ 0 ~ \mathrm { a . s . }$ ., from the last theorem of the previous section, we have $( Z _ { t } ) _ { 0 \leq t \leq T }$ is a true martingale  

Proof of the 1FTAP, easier direction. Suppose that there is a martingale deflator Y . Let H be an n-dimensional previsible process and let $c _ { 0 } = - H _ { 1 } \cdot P _ { 0 }$ and 

$$
c _ {t} = H _ {t} \cdot (P _ {t} + \delta_ {t}) - H _ {t + 1} \cdot P _ {t} \text {   for   } t \geq 1.
$$

Suppose there is some non-random $T > 0$ such that $c _ { T } = H _ { T } \cdot \left( P _ { T } + \delta _ { T } \right)$ and $c _ { t } \geq 0$ almost surely for all $0 \leq t \leq T$ . To show that H is not an arbitrage, must show that $c _ { t } = 0$ almost surely for all $0 \leq t \leq T$ 

To this end, let 

$$
Z _ {T} = \sum_ {s = 0} ^ {T} c _ {s} Y _ {s}.
$$

Since $Y _ { s } > 0$ and $c _ { s } \geq 0$ for all $0 \leq s \leq T$ , we need only show that $Z _ { T } = 0$ almost surely. By the pigeon-hole principle, it is suficient to show 

$$
\mathbb {E} (Z _ {T}) = 0.
$$

To finish the proof, let 

$$
Z _ {t} = X _ {t} Y _ {t} + \sum_ {s = 0} ^ {t - 1} c _ {s} Y _ {s} \text { for } 0 \leq t \leq T
$$

where we have set $X _ { 0 } = 0$ and $X _ { t } = H _ { t } \cdot \left( P _ { t } + \delta _ { t } \right)$ for $1 \leq t \leq T$ . By the previous lemma, the process $( Z _ { t } ) _ { 0 \leq t \leq T }$ is a martingale. Since $Z _ { 0 } = 0$ , we are done.  

## 6. Proof of harder direction of the 1FTAP

In this section we will present elements of the proof of the first fundamental theorem of asset pricing. We will give a complete proof of the one-period case, and sketch the main steps to prove the full multi-period case. But first, we take a moment to reflect on the economic motivation. 

6.1. Motivation: Langrangian duality. Consider the investor’s utility maximisation problem to find an investment strategy H to 

$$
\text { maximise } \mathbb {E} [ U (c) ] \text { subject   to } \left\{ \begin{array}{l} c _ {0} = x - H _ {1} \cdot P _ {0}, \\ c _ {t} = H _ {t} \cdot (P _ {t} + \delta_ {t}) - H _ {t + 1} \cdot P _ {t} \text { for } 1 \leq t \leq T - 1 \\ c _ {T} = H _ {T} \cdot (P _ {T} + \delta_ {T}) \end{array} \right.
$$

where the utility function u is increasing in each argument. We have discussed previously that the existence of a maximiser implies that there does not exist an arbitrage. We now explain why the existence of a maximiser also points to the existence of a martingale deflator. 

As usual in a constrained optimisation problem, we apply the Lagrangian method. Recall that this involves replacing our given objective function with the so-called Lagrangian which encodes the constraints. In this case the Lagrangian is 

$$
\begin{array}{l} L (c, H, Y) = \mathbb {E} [ u (c _ {0}, \dots , c _ {T}) ] + Y _ {0} (x - c _ {0} - H _ {1} \cdot P _ {0}) \\ \qquad + \mathbb {E} \left[ \sum_ {t = 1} ^ {T - 1} Y _ {t} [ H _ {t} \cdot (P _ {t} + \delta_ {t}) - H _ {t + 1} \cdot P _ {t} - c _ {t} ] + Y _ {T} [ H _ {T} \cdot (P _ {T} + \delta_ {T}) - c _ {T} ] \right] \end{array}
$$

where the real-valued adapted process $( Y _ { t } ) _ { 0 \leq t \leq T }$ is the family of Lagrange multipliers. 

To identify the dual feasibility condition, we seek to find conditions on the Lagrange multiplier process $Y$ implied by the existence of a maximiser of the Lagrangian $L ( c , H , Y )$ over adapted c and previsible H. To this end, we rewrite the Lagrangian as 

$$
\begin{array}{l} L (c, H, Y) = \mathbb {E} \left[ u (c _ {0}, \ldots , c _ {T}) - \sum_ {t = 0} ^ {T} Y _ {t} c _ {t} \right] + x Y _ {0} \\ \qquad + \sum_ {t = 1} ^ {T} \mathbb {E} \{H _ {t} \cdot [ (P _ {t} + \delta_ {t}) Y _ {t} - P _ {t - 1} Y _ {t - 1} ] \}. \end{array}
$$

By formally diferentiating with respect to the t-th consumption variable, we find the maximised consumption $c ^ { * }$ satisfies 

$$
\mathbb {E} \left[ \frac {\partial u}{\partial c _ {t}} (c ^ {*}) | \mathcal {F} _ {t} \right] = Y _ {t}.
$$

Diferentiating with respect to $H _ { t }$ yields 

$$
\mathbb {E} [ (P _ {t} + \delta_ {t}) Y _ {t} | \mathcal {F} _ {t - 1} ] = P _ {t - 1} Y _ {t - 1}
$$

These two conditions suggest that $Y$ is an adapted, positive process such that the process 

$$
M _ {t} = Y _ {t} P _ {t} + \sum_ {s = 1} ^ {t} Y _ {s} \delta_ {s}
$$

is a martingale – i.e. Y is a martingale deflator. 

6.2. Proof when $T = 1$ . We now proceed to turn those fuzzy heuristics into a proper proof. We consider the one-period case. So our market data are the prices $P _ { 0 } , P _ { 1 }$ and the dividend $\delta _ { 1 }$ . Since our calculations only involve $P _ { 1 } + \delta _ { 1 }$ , but not the two terms separately, there is no loss just assuming $\delta _ { 1 } = 0$ 

We suppose that the market $( P _ { t } ) _ { t \in \{ 0 , 1 \} }$ has no arbitrage, so that for any vector $H \in \mathbb { R } ^ { n }$ that has the property that $H \cdot P _ { 0 } \leq \dot { 0 } \leq H \cdot P _ { 1 }$ almost surely, it must be the case that $H \cdot P _ { 0 } = 0 = H \cdot P _ { 1 }$ almost surely. We will show that, given any positive random variable $Z ,$ there exists a martingale deflator $Y _ { 0 } , Y _ { 1 }$ such that the product $Y _ { 1 } Z$ is bounded by a constant. This extra boundedness assumption is much stronger than what we need, but it comes for free from the proof and we will find it useful later in the course. 

Let 

$$
\zeta = \frac {e ^ {- \| P _ {1} \| ^ {2} / 2}}{1 + Z}.
$$

Define a function $F : \mathbb { R } ^ { n }  \mathbb { R }$ by 

$$
F (H) = e ^ {H \cdot P _ {0}} + \mathbb {E} [ e ^ {- H \cdot P _ {1}} \zeta ].
$$

The positive random variable $\zeta$ is introduced to ensure integrability. Indeed note that the integrand $e ^ { - H \cdot P _ { 1 } } \zeta \leq e ^ { \| H \| ^ { 2 } / 2 }$ is bounded for each choice of $H$ . In particular, the function $F$ is finite everywhere and (by the dominated convergence theorem) smooth. 

We will show that no investment-consumption arbitrage implies that the function $F$ has a minimiser $H ^ { * }$ . By the first order condition for a minimum, we have 

$$
0 = \nabla F (H ^ {*}) = e ^ {H ^ {*} \cdot P _ {0}} P _ {0} - \mathbb {E} [ e ^ {- H ^ {*} \cdot P _ {1}} \zeta P _ {t} ]
$$

and hence we may take 

$$
Y _ {0} = e ^ {H ^ {*} \cdot P _ {0}} \mathrm{and} Y _ {1} = e ^ {- H ^ {*} \cdot P _ {1}} \zeta .
$$

Note that $Y _ { 1 } Z < C$ for some constant $C > 0$ (which depends on $H ^ { * }$ in general). 

So let $( H _ { k } ) _ { k }$ be a sequence such that $F ( H _ { k } ) \to \operatorname* { i n f } _ { H } F ( H )$ . If $( H _ { k } ) _ { k }$ is bounded, we can pass to a convergent subsequence, by the Bolzano–Weierstrass theorem, such that $H _ { k } \to H ^ { * }$ $\mathrm { B y }$ the smoothness of $F$ we have 

$$
\inf _ {H} F (H) = \lim _ {k} F (H _ {k}) = F (\lim _ {k} H _ {k}) = F (H ^ {*})
$$

so $H ^ { * }$ is our desired minimiser. 

It remains to show that no arbitrage implies that there exists a bounded minimising sequence $( H _ { k } ) _ { k }$ . We show that if every minimising sequence $( H _ { k } ) _ { k }$ is unbounded, then there would be a contradiction. 

Now we arrive at a little technicality. Let 

$$
\mathcal {U} = \left\{u \in \mathbb {R} ^ {n}: u \cdot P _ {0} = 0 = u \cdot P _ {1} \text {a.s.} \right\} \subseteq \mathbb {R} ^ {n}
$$

and let 

$$
\mathcal {V} = \mathcal {U} ^ {\perp}.
$$

Notice that if $u \in \mathcal { U }$ and $v \in \mathcal V$ then $F ( u + v ) = F ( v )$ . Hence, by projecting a given minimising sequence onto the subspace V, it is suficient to consider minimising sequence $( H _ { k } ) _ { k }$ taking values in $\nu .$ 

So suppose, for the sake of finding a contradiction, that all minimising sequence $( H _ { k } ) _ { k }$ taking values in $\nu$ are unbounded. We can pass to a subsequence such that $\| H _ { k } \| \uparrow \infty$ . Now let 

$$
\hat {H} _ {k} = \frac {H _ {k}}{\| H _ {k} \|}.
$$

Note that $\| \hat { H } _ { k } \| = 1$ and that $\hat { H } _ { k } \in \mathcal { V }$ . Since $( { \hat { H } } _ { k } ) _ { k }$ is bounded, we can again pass to a convergent subsequence such that $\hat { H } _ { k } \  \ \hat { H }$ . Notice once more that $\| \hat { H } \| = 1$ and that $\hat { H } \in \nu$ 

We know that the sequence $F ( H _ { k } )$ is bounded (since it is convergent) but we also have 

$$
F (H _ {k}) = (e ^ {\hat {H} _ {k} \cdot P _ {0}}) ^ {\| H _ {k} \|} + \mathbb {E} [ (e ^ {- \hat {H} _ {k} \cdot P _ {1}}) ^ {\| H _ {k} \|} \zeta ]
$$

so we must conclude that $\hat { H } \cdot P _ { 0 } \leq 0 \leq \hat { H } \cdot P _ { 1 }$ a.s. (since otherwise the right-hand side would blow up). By no-arbitrage, we conclude that the candidate arbitrage $\hat { H }$ is not actually an arbitrage, so $\hat { H } \cdot P _ { 0 } = 0 = \hat { H } \cdot P _ { 1 }$ a.s. 

We have shown that $\hat { H }$ is in $\mathcal { U } .$ . But since $\hat { H }$ is also in $\mathcal { V } = \mathcal { U } ^ { \perp }$ , so we have $\hat { H } = 0$ . And, finally, this contradicts $\| { \hat { H } } \| = 1$  

6.3. Elements of the proof of the harder direction of the multi-period 1FTAP. We have already seen the one period case. The full multi-period proof is a little more dificult because of some technicalities involving measurability. 

We begin with two propositions that show that two of the existential-type results we needed in one-period proof have measurable versions. 

Proposition. Let $f : \mathbb { R } ^ { n } \times \Omega \to \mathbb { R }$ be such that $f ( x , \cdot )$ is measurable for all $x _ { i }$ and that $f ( \cdot , \omega )$ is continuous and has a unique minimiser $X ^ { \ast } ( \omega ) ~ f o r$ each $\omega$ . Then $X ^ { \ast }$ is measurable. 

Let us pause to think about what it means for the unique minimiser $x ^ { * } \in \mathbb { R } ^ { n }$ of a continuous function $g : \mathbb { R } ^ { n }  \mathbb { R }$ to be in a closed rectangle of the form $A = [ a _ { 1 } , b _ { 1 } ] \times \cdots \times$ $[ a _ { n } , b _ { n } ]$ 

First note that that for all $q \neq x ^ { * }$ , we have $g ( x ^ { * } ) < g ( q )$ . Let $Q \subset \mathbb { R } ^ { n }$ be countable and dense - for instance, let $Q$ be the set of points with rational coordinates. By the continuity of $g$ and the density of $Q { \mathrm { . } }$ , we have that for every $q \neq x ^ { * }$ , there exists a $p \in Q$ such that $g ( p ) < g ( q )$ 

Now if $x ^ { * } \in A$ , then for any $q \in A ^ { c } \cap Q$ , there exists a $p \in A \cap Q$ such that $g ( p ) < g ( q )$ since $q \neq x ^ { * }$ and $A \cap Q$ is dense in $A .$ 

Conversely, suppose that for any $q \in A ^ { c } \cap Q$ , there exists a $p \in A \cap Q$ such that $g ( p ) < g ( q )$ This means 

$$
\inf _ {x \in A \cap Q} g (x) \leq \inf _ {x \in A ^ {c} \cap Q} g (x).
$$

By the continuity of $g$ the above inequality implies 

$$
\inf _ {x \in A} g (x) = \inf _ {x \in A \cup A ^ {c}} g (x) = g (x ^ {*})
$$

and in particular, we have $x ^ { * } \in A$ since $A$ is closed. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/bce54bc69dda9dac9e25e431c8151cbb291ce7be344da1352145f5c87d54f212.jpg)


Proof. For any closed rectangle $A \subset \mathbb { R } ^ { n }$ we have 

$$
\{\omega : X ^ {*} (\omega) \in A \} = \bigcap_ {q \in A ^ {c} \cap Q} \bigcup_ {p \in A \cap Q} \{\omega : f (p, \omega) <   f (q, \omega) \}
$$

where $Q$ is a countable dense subset of $\mathbb { R } ^ { n }$ . Since the Borel sigma-field is generated by such rectangles, this implies the measurability of $X ^ { * }$  

We also need a useful measurable version of the Bolzano–Weierstrass theorem. 

Proposition. Let $( \xi _ { i } ) _ { i \geq 1 }$ be a sequence of measurable functions $\xi _ { i } : \Omega \to \mathbb { R } ^ { n }$ such that $\operatorname* { s u p } _ { i } \| \xi _ { i } ( \omega ) \| < \infty$ for all $\omega \in \Omega$ . Then there exists an increasing sequence of integer-valued measurable functions $I _ { j }$ and an $\mathbb { R } ^ { n }$ -valued measurable function $\xi ^ { * }$ such that 

$$
\xi_ {I _ {j} (\omega)} (\omega) \rightarrow \xi^ {*} (\omega) a s j \rightarrow \infty
$$

for all $\omega \in \Omega$ 

Proof. First we consider the $n = 1$ case. Let $\xi ^ { * } ( \omega ) = \operatorname* { l i m } \operatorname* { s u p } _ { i } \xi _ { i } ( \omega )$ . Note $\xi ^ { * }$ is finitevalued and measurable, and that for every $j > 0$ there exists an infinite number of i’s such that $\xi _ { i } ( \omega ) \ge \xi ^ { * } ( \omega ) - 1 / j$ . Now let 

$$
I _ {j} = \inf \{i \geq j: \xi_ {i} \geq \xi^ {*} - 1 / j \}.
$$

Since we have the representation of the event 

$$
\{I _ {j} \leq h \} = \cup_ {i = j} ^ {h} \{\xi_ {i} \geq \xi^ {*} - 1 / j \}
$$

for each $h \geq j$ , the function $I _ { j }$ is measurable and $\xi _ { I _ { i } } \to \xi ^ { * }$ as desired. 

Now we prove the claim for any dimension $n \geq 1$ by induction. Suppose that the claim is true for dimension $n = N$ . Let $( \xi _ { i } ) _ { i }$ be a sequence of measurable function valued in $\mathbb { R } ^ { N + 1 }$ such that sup $\lVert \xi _ { i } ( \omega ) \rVert < \infty$ . Writing $\xi _ { i } = ( \zeta _ { i } , \eta _ { i } )$ where $\zeta _ { i }$ takes values in $\mathbb { R } ^ { N }$ and $\eta _ { i }$ takes values in R, we have by assumption the existence of a measurable sequence $I _ { j }$ and a measurable $\zeta ^ { * }$ such that 

$$
\zeta_ {I _ {j}} \rightarrow \zeta^ {*}.
$$

Notice that $( \eta _ { I _ { j } ( \omega ) } ( \omega ) ) _ { j }$ is bounded for each $\omega ,$ , and hence by the $n = 1$ case, there exists an increasing measurable sequence $J _ { k }$ and a measurable $\eta ^ { * }$ such that $\eta _ { I _ { J _ { k } } } \to \eta ^ { * }$ . In particular, 

$$
\xi_ {I _ {J _ {k}}} \rightarrow (\zeta^ {*}, \eta^ {*}) = \xi^ {*}
$$

as desired. 

## 7. Num´eraires and equivalent martingale measures

For the previous sections, we have worked in considerable generality. We have allowed our assets to pay a dividend, and we have even allowed the prices and dividends to be negative. In this section, we will see the efect of adding more assumptions to our model. 

The first assumption that we will make from here on is that, unless otherwise indicated, there are no dividends: 

$$
\mathrm{Assumption:} \delta_ {t} = 0 \mathrm{almostsurelyforall} t \geq 1
$$

Removing dividends from the conversation simplifies things somewhat. For instance, in this case, a positive adapted process $Y$ is a martingale deflator if and only if the process $Y P$ is a martingale. It is sometimes useful (for example, for the example sheet) to introduce some vocabulary: 

Definition. In a market with no dividends, a pricing kernel (or stochastic discount factor or state price density) between times s and t, where $0 \leq s < t$ , is a positive $\mathcal { F } _ { t ^ { - } }$ measurable random variable $\rho _ { s , t }$ such that 

$$
P _ {s} = \mathbb {E} (\rho_ {s, t} P _ {t} | \mathcal {F} _ {s}).
$$

Let Y be a martingale deflator, so that $\mathbb { E } ( Y _ { t } P _ { t } | \mathcal { F } _ { s } ) = Y _ { s } P _ { s }$ for all $0 \leq s < t$ , and let $\rho _ { s , t } ~ = ~ Y _ { t } / Y _ { s }$ . If $\rho _ { s , t } P _ { t }$ is integrable, then $\rho _ { s , t }$ is a pricing kernel between times s and t. Conversely, suppose $\rho _ { s , s + 1 }$ is a pricing kernel between times s and $s + 1$ for $s \geq 0$ , and let $Y _ { t } = \rho _ { 0 , 1 } \cdot \cdot \cdot \cdot \rho _ { t - 1 , t }$ . Then assuming $Y P$ is integrable, then Y is a martingale deflator. 

Hopefully, after several sections where the theory is worked out in full generality, it is not too dificult to reincorporate dividends into the remaining bits of the course if desired. 

The point of this section is now to consider the efect of adding the further assumption that there exists a portfolio with a strictly positive price. 

Definition. A num´eraire portfolio is n-dimensional previsible process $\eta = ( \eta _ { t } ) _ { t \geq 0 }$ such that $\eta _ { t } \cdot P _ { t } > 0$ almost surely for each $t \geq 0$ , and satisfying the pure-investment self-financing condition 

$$
\left(\eta_ {t} - \eta_ {t + 1}\right) \cdot P _ {t} = 0.
$$

A num´eraire asset is an asset with a strictly positive price. 

Remark. If asset i is a num´eraire asset, then the constant portfolio η defined for all $t \geq 0$ by 

$$
\eta_ {t} ^ {j} = \left\{ \begin{array}{l l} 1 & \text {if j = i} \\ 0 & \text {otherwise} \end{array} \right.
$$

is a num´eraire portfolio. 

In the context of a market with a num´eraire, we consider a diferent type of arbitrage: 

Definition. A terminal consumption arbitrage is a n-dimensional previsible process H such that there exists a non-random $T > 0$ such that almost surely we have 

$$
\begin{array}{l} c _ {0} = - H _ {1} \cdot P _ {0} = 0 \\ c _ {t} = (H _ {t} - H _ {t + 1}) \cdot P _ {t} = 0 \text { for } 1 \leq t \leq T - 1 \\ c _ {T} = H _ {T} \cdot P _ {T} \geq 0 \end{array}
$$

and 

$$
\mathbb {P} (c _ {T} > 0) > 0.
$$

Note that our first definition of arbitrage allowed for consumption at intermediate times. Clearly, a terminal consumption arbitrage is an arbitrage according to our earlier definition. We now ask when does the existence of an arbitrage (possibly with intermediate consumption) imply the existence of a terminal consumption arbitrage. 

We come to the answer to our question: 

Proposition. Consider a market with a num´eraire η and let $N _ { t } = \eta _ { t } \cdot P _ { t }$ for $t \geq 0$ Let H be an investment-consumption strategy with consumption stream 

$$
\begin{array}{l} {c _ {0} = x - H _ {1} \cdot P _ {0}} \\ {c _ {t} = (H _ {t} - H _ {t + 1}) \cdot P _ {t},} \end{array}
$$

where x is the initial wealth. Let 

$$
K _ {t} = H _ {t} + \eta_ {t} \sum_ {s = 0} ^ {t - 1} \frac {c _ {s}}{N _ {s}}
$$

for $t \geq 1$ . Then K is a pure-investment strategy from the same initial wealth x. (That is, K be the strategy that consists of holding at time t the portfolio $H _ { t }$ but of instead of consuming the amount $c _ { t }$ , instead invest this money into the num´eraire portfolio.) 

In particular, H is an arbitrage if and only if K is a terminal consumption arbitrage. 

Proof. Note that 

$$
\begin{array}{r l} & {(K _ {t} - K _ {t + 1}) \cdot P _ {t} = (H _ {t} - H _ {t + 1}) \cdot P _ {t} - \eta_ {t + 1} \cdot P _ {t} \frac {c _ {t}}{N _ {t}}} \\ & {\qquad + (\eta_ {t} - \eta_ {t + 1}) \cdot P _ {t} \sum_ {s = 1} ^ {t - 1} \frac {c _ {s}}{N _ {s}}} \\ & {\qquad = 0} \end{array}
$$

so K is a pure investment strategy by the assumption that $\eta$ is pure-investment. Suppose $c _ { T } = H _ { T } \cdot P _ { T }$ for some non-random time T. Then 

$$
K _ {T} \cdot P _ {T} = N _ {T} \sum_ {s = 0} ^ {T} \frac {c _ {s}}{N _ {s}} \geq 0.
$$

The left-hand side is positive if and only if $c _ { t }$ is positive for some $0 \leq t \leq T$ 

Now we move to a definition that only makes sense in a market with a num´eraire. 

Definition. Let P be a market model defined on a probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ . The measure P is called the objective (or historical or statistical) measure for the model. 

Suppose that there exists a num´eraire portfolio $\eta$ and let $N = \eta \cdot P$ . An equivalent martingale measure relative to this num´eraire is any probability measure Q equivalent to $\mathbb { P }$ such that the discounted price processes 

$$
\left(\frac {P _ {t}}{N _ {t}}\right) _ {t \geq 0}
$$

is a martingale under $\mathbb { Q } .$ 

Remark. In many accounts of arbitrage theory, the concept of an equivalent martingale measure has taken centre stage. I believe that its importance has been overstressed. In particular, it is a num´eraire-dependent concept, unlike that of a martingale deflator. For instance, if there are two assets that both num´eraires (for example from the point of view of a British trader, both the euro and the US dollar are num´eraires) then one must be very careful to specify which one is the num´eraire. 

Before proceeding, it might be useful to recall some facts from probability theory. 

Definition. Let $( \Omega , { \mathcal { F } } )$ be a measurable space and let P and Q be two probability measures on $( \Omega , { \mathcal { F } } )$ . The measures $\mathbb { P }$ and $\mathbb { Q }$ are equivalent, written $\mathbb { P } \sim \mathbb { Q }$ , if 

$$
\{A \in \mathcal {F}: \mathbb {P} (A) = 1 \} = \{A \in \mathcal {F}: \mathbb {Q} (A) = 1 \}
$$

The above definition says that equivalent probability measures have the same almost sure events. Complementarily, equivalent probability measures have the same null sets: that is, $\mathbb { P } \sim \mathbb { Q }$ if 

$$
\{A \in \mathcal {F}: \mathbb {P} (A) = 0 \} = \{A \in \mathcal {F}: \mathbb {Q} (A) = 0 \}.
$$

It turns out that equivalent measures can be characterised by the following theorem. When there are more than one probability measure floating around, we use the notation $\mathbb { E } ^ { \mathbb { P } }$ to denote expected value with respect to $\mathbb { P } ,$ etc. 

Theorem (Radon–Nikodym theorem). The probability measure $\mathbb { Q }$ is equivalent to the probability measure $\mathbb { P }$ if and only if there exists a $\mathbb { P } { - } a . s$ . positive random variable Z such that 

$$
\mathbb {Q} (A) = \mathbb {E} ^ {\mathbb {P}} (Z \mathbb {1} _ {A})
$$

for each $A \in { \mathcal { F } }$ 

The random variable $Z$ is called the density, or the Radon–Nikodym derivative, of $\mathbb { Q }$ with respect to $\mathbb { P } _ { z }$ , and is often denoted 

$$
Z = \frac {d \mathbb {Q}}{d \mathbb {P}}.
$$

As a mnemonic device, note that the Radon–Nikodym derivative satisfies the identity 

$$
\mathbb {Q} (A) = \int_ {A} \frac {d \mathbb {Q}}{d \mathbb {P}} d \mathbb {P}.
$$

Also, note that $\mathbb { P }$ has a density with respect to $\mathbb { Q }$ given by 

$$
\frac {d \mathbb {P}}{d \mathbb {Q}} = \frac {1}{Z}.
$$

We only need the easy direction of the theorem, that the existence of a positive density implies equivalence, for this course. Here is a proof. The proof of the harder direction is omitted since we do not need it. 

Proof. Suppose $\mathbb { P } ( Z > 0 ) = 1$ and that $\mathbb { E } ^ { \mathbb { P } } ( Z ) = 1$ . Define a set function $\mathbb { Q }$ by 

$$
\mathbb {Q} (A) = \mathbb {E} ^ {\mathbb {P}} (Z \mathbb {1} _ {A}).
$$

Note that $\mathbb { Q }$ is countably additive by the monotone convergence theorem. Also, $\mathbb { Q } ( \Omega ) =$ $\mathbb { E } ^ { \mathbb { P } } ( Z ) = 1$ , so $\mathbb { Q }$ is a probability measure. If $\mathbb { P } ( A ) = 0$ , then the event $\left\{ \mathbb { 1 } _ { A } = 0 \right\}$ is P-almost sure and hence 

$$
\mathbb {Q} (A) = \mathbb {E} ^ {\mathbb {P}} (Z \mathbb {1} _ {A}) = 0.
$$

Conversely, if $\mathbb { Q } ( A ) = 0$ we can conclude that $\{ Z \mathbb { 1 } _ { A } = 0 \}$ is $\mathbb { P } \mathrm { - a . s }$ . by the pigeon-hole principle since $\{ Z \mathbb { 1 } _ { A } \geq 0 \}$ is $\mathbb { P } \mathrm { - a . s }$ . But since $\{ Z > 0 \}$ is $\mathbb { P } \mathrm { - a . s . }$ , we must conclude that $\left\{ \mathbb { 1 } _ { A } = 0 \right\}$ is $\mathbb { P } \mathrm { - a . s . }$ , i.e. $\mathbb { P } ( A ) = 0$ . Thus $\mathbb { Q }$ and $\mathbb { P }$ are equivalent.  

Example. Consider the sample space $\Omega = \{ 1 , 2 , 3 \}$ with the set $\mathcal { F }$ of events all subsets of Ω. Consider probability measures $\mathbb { P }$ and $\mathbb { Q }$ defined by 

$$
\bullet \mathbb {P} \{1 \} = \frac {1}{2}, \mathbb {P} \{2 \} = \frac {1}{2}, \text {   and   } \mathbb {P} \{3 \} = 0
$$

$$
\bullet \mathbb {Q} \{1 \} = \frac {1}{1 0 0 0}, \mathbb {Q} \{2 \} = \frac {9 9 9}{1 0 0 0}, \text { and } \mathbb {Q} \{3 \} = 0.
$$

Then $\mathbb { P }$ and $\mathbb { Q }$ are equivalent. We may take their density $\begin{array} { r } { Z = \frac { d \mathbb { Q } } { d \mathbb { P } } } \end{array}$ to be 

$$
Z (1) = \frac {1}{5 0 0}, Z (2) = \frac {9 9 9}{5 0 0}, Z (3) = 0.
$$

(Since both measures don’t ‘see’ the event {3}, we can let $Z ( 3 )$ be any value.) 

Now, returning to our financial model, we have a result that says, that in a market with a num´eraire, the notion of an equivalent martingale measure is morally the same as the notion of a martingale deflator. 

Proposition. Suppose the market has a num´eraire, and fix a non-random time horizon $T > 0$ . The market model $( P _ { t } ) _ { 0 \leq t \leq T }$ has an equivalent martingale measure relative to the num´eraire if and only if there is a martingale deflator. 

Proof. Let Y be a process such that $\left\{ Y _ { T } \ > \ 0 \right\}$ is $\mathbb { P } \mathrm { - a . s }$ . and such that $Y _ { T } P _ { T }$ is $\mathbb { P } _ { - }$ integrable. Define a new measure $\mathbb { Q }$ by the density 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = \frac {Y _ {T} N _ {T}}{\mathbb {E} ^ {\mathbb {P}} (Y _ {T} N _ {T})}.
$$

Our analysis turns on the Bayes formula 

$$
\mathbb {E} ^ {\mathbb {Q}} \left(\frac {P _ {T}}{N _ {T}} | \mathcal {F} _ {t}\right) = \frac {\mathbb {E} ^ {\mathbb {P}} (P _ {T} Y _ {T} | \mathcal {F} _ {t})}{\mathbb {E} ^ {\mathbb {P}} (N _ {T} Y _ {T} | \mathcal {F} _ {t})}
$$

Suppose Y is a martingale deflator. We have 

$$
\mathbb {E} ^ {\mathbb {P}} \left(P _ {T} Y _ {T} | \mathcal {F} _ {t}\right) = P _ {t} Y _ {t}.
$$

by definition. Also note that 

$$
Y _ {t} N _ {t} - Y _ {t - 1} N _ {t - 1} = \eta_ {t} \cdot (Y _ {t} P _ {t} - Y _ {t - 1} P _ {t - 1})
$$

and hence $Y N$ is a local martingale. However, since $Y N$ is non-negative, we know from last section that $Y N$ is a true martingale. In particular 

$$
\mathbb {E} ^ {\mathbb {P}} \left(N _ {T} Y _ {T} | \mathcal {F} _ {t}\right) = N _ {t} Y _ {t}.
$$

By the Bayes formula we have 

$$
\mathbb {E} ^ {\mathbb {Q}} \left(\frac {P _ {T}}{N _ {T}} | \mathcal {F} _ {t}\right) = \frac {P _ {t}}{N _ {t}}
$$

and hence $P / N$ is a $\mathbb { Q } \mathrm { . }$ -martingale, i.e. $\mathbb { Q }$ is an equivalent martingale measure. 

Conversely, suppose $\mathbb { Q }$ is an equivalent martingale measure. Let 

$$
Z _ {t} = \mathbb {E} ^ {\mathbb {P}} \left(\frac {d \mathbb {Q}}{d \mathbb {P}} | \mathcal {F} _ {t}\right).
$$

Note that $Z$ is a positive P-martingale. Let 

$$
Y _ {t} = Z _ {t} / N _ {t}.
$$

Since the random variable $P _ { T } / N _ { T }$ is Q-integrable by the definition of martingale, we can conclude that $P _ { T } Y _ { T }$ is P-integrable. Furthermore, the process Y is positive and satisfies 

$$
\begin{array}{r l} & {\mathbb {E} ^ {\mathbb {P}} (N _ {T} Y _ {T} | \mathcal {F} _ {t}) = \mathbb {E} ^ {\mathbb {P}} (Z _ {T} | \mathcal {F} _ {t})} \\ & {\qquad = Z _ {t}} \\ & {\qquad = N _ {t} Y _ {t}.} \end{array}
$$

Hence by the Bayes formula 

$$
\begin{array}{r l} & {\mathbb {E} ^ {\mathbb {P}} (P _ {T} Y _ {T} | \mathcal {F} _ {t}) = \mathbb {E} ^ {\mathbb {Q}} \left(\frac {P _ {T}}{N _ {T}} | \mathcal {F} _ {t}\right) \mathbb {E} ^ {\mathbb {P}} (N _ {T} Y _ {T} | \mathcal {F} _ {t})} \\ & {\qquad = \frac {P _ {t}}{N _ {t}} (N _ {t} Y _ {t})} \\ & {\qquad = P _ {t} Y _ {t}} \end{array}
$$

so that PY is a P-martingale and hence Y is a martingale deflator. 

Combining the two results of this section, we have the usual formulation of the first fundamental theorem of asset pricing: 

Theorem (First Fundamental Theorem of Asset Pricing when there is a num´eraire). Suppose the market has is a num´eraire, and fix a non-random time horizon $T > 0$ . The market model $( P _ { t } ) _ { 0 \leq t \leq T }$ has no terminal consumption arbitrage if and only if there exists an equivalent martingale measure relative to the num´eraire. 

## 8. Special num´eraires and equivalent martingale measures

In this section we consider two classes of num´eraire assets (and their respective equivalent martingale measures) that arise very frequently in applications. 

Definition. A (risk-free zero-coupon) bond is an asset such that there exists a nonrandom time $T > 0$ (called its maturity date) and such that its price at time T is a nonrandom positive constant (called its face value or principal value ). Unless otherwise specified, we shall assume that the face value of a bond is £1. We will denote the time t price of the bond of maturity T by $P _ { t } ^ { T }$ for $0 \leq t \leq T$ 

Proposition. Suppose the market contains a bond. If the market has no arbitrage, then the bond is a num´eraire. 

Proof. There are at least two ways to prove this. It is important to understand both methods. 

A ‘primal’ argument. The idea is that if the bond price drops to zero or less, then an investor could lock in a risk-less profit. In particular, if there is no arbitrage, the price must stay positive. 

In mathematical notation, let 

$$
\tau = \inf \{0 \leq t \leq T: P _ {t} ^ {T} \leq 0 \}.
$$

with the convention that $\tau = + \infty$ if $P _ { t } ^ { T } > 0$ for all $0 \leq t \leq T$ 

Note that τ is a stopping time. Consider predictable process $H _ { t } ~ = ~ \mathbb { 1 } _ { \{ \tau < t \leq T \} }$ This corresponds to a portfolio of buying the bond immediately after the price drops to zero or below and hold it until maturity. Note that 

$$
\begin{array}{r l} & c _ {0} = - H _ {1} ^ {T} P _ {0} ^ {T} = - \mathbb {1} _ {\{\tau = 0 \}} P _ {0} ^ {T} \geq 0 \\ & c _ {t} = (H _ {t} ^ {T} - H _ {t + 1} ^ {T}) P _ {t} ^ {T} = - \mathbb {1} _ {\{\tau = t \}} P _ {t} ^ {T} \geq 0 \text {for} 1 \leq t \leq T \\ & c _ {T} = \mathbb {1} _ {\{\tau <   T \}} P _ {T} ^ {T} \geq 0. \end{array}
$$

If there is no arbitrage, then $c _ { t } = 0 ~ \mathrm { a . s }$ . for all $0 \leq t \leq T$ . Hence $\tau = + \infty \ \mathrm { a . s }$ 

A ‘dual’ argument. Since there is no arbitrage, there exists a martingale deflator Y. Note $Y P ^ { T }$ is a martingale, and hence 

$$
P _ {t} ^ {T} = \frac {1}{Y _ {t}} \mathbb {E} (Y _ {T} | \mathcal {F} _ {t})
$$

since $P _ { T } ^ { T } = 1$ by definition. Since $Y _ { t } > 0 \ \mathrm { a . s }$ . for all $t \geq 0$ , the conclusion follows.  

Since we now know no arbitrage implies that bonds are num´eraires, we can discuss equivalent martingale measures: 

Definition. An equivalent martingale measure with respect to a bond of maturity $T > 0$ is called a T-forward measure. 

For an application of forward measures, we consider a forward contract: 

Definition. A forward initiated at time t with maturity date T is a contract where, at time t, no money is exchanged and at time T, an asset with price $S _ { T }$ is swapped for $F _ { t } ^ { T }$ units of money, where $F _ { t } ^ { T }$ is known at time t. The quantity $F _ { t } ^ { \bar { T } }$ is called the forward price of the asset. 

See the diagram for the timing of the payment streams in a forward contract. 

forward 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/bd4e3c4be5dbf4973f083f583fc6d4b2a5e3520ae643e61cb249ba0145a6b6a6.jpg)


Proposition. Consider a market model with a bond of maturity T and forward contract initiated at time t and maturing at time T. If the market has no arbitrage, then 

$$
F _ {t} ^ {T} = \mathbb {E} ^ {\mathbb {Q} ^ {T}} (S _ {T} | \mathcal {F} _ {t})
$$

where $\mathbb { Q } ^ { T }$ is a T-forward measure. 

Proof. Let $D _ { s }$ be the price of the forward contract at time $s ,$ for $t \le s \le T$ . Since there is no arbitrage, we have 

$$
D _ {t} = P _ {t} ^ {T} \mathbb {E} ^ {\mathbb {Q} ^ {T}} (D _ {T} | \mathcal {F} _ {t})
$$

Noting that $D _ { t } = 0$ and $D _ { T } = S _ { T } - F _ { t } ^ { T }$ , and that $F _ { t } ^ { T }$ is $\mathcal { F } _ { t }$ -measurable yields the result, upon rearrangement.  

We now suppose there is a whole family of bonds, indexed by their maturities. 

Definition. Consider a market with bonds of all maturities $T \in \{ 0 , 1 , 2 , . . . \}$ . The spot interest rate at time t is 

$$
r _ {t} = \frac {1}{P _ {t - 1} ^ {t}} - 1.
$$

The value of the bank account (or money market account) is given by $B _ { 0 } = 1$ and 

$$
B _ {t} = \prod_ {s = 1} ^ {t} (1 + r _ {s}) \text {   for   } t \geq 1.
$$

for all t. 

Remark. Note that the spot interest rate and bank account processes are previsible. 

The connection between bonds and the bank account is the following: 

Proposition. Suppose the arbitrage-free market model has bonds of all maturities. Then there exists a pure-investment (that is, no consumption) strategy η such that 

$$
B _ {t} = \eta_ {t} \cdot (P _ {t} ^ {0}, P _ {t} ^ {1}, P _ {t} ^ {2}, \ldots)
$$

for all $t \geq 0$ 

Proof. Let $\eta _ { t } = B _ { t } \delta ^ { t }$ , where $\delta ^ { t }$ is the portfolio of holding exactly one bond of maturity t. That is to say, η is the strategy of investing all of the accumulated wealth in the bond of maturity t during the interval $( t - 1 , t ]$ . Note that η is previsible and that 

$$
\begin{array}{r l} & {\eta_ {t + 1} \cdot (P _ {t} ^ {0}, P _ {t} ^ {1}, P _ {t} ^ {2}, \ldots) = B _ {t + 1} \delta^ {t + 1} \cdot (P _ {t} ^ {0}, P _ {t} ^ {1}, P _ {t} ^ {2}, \ldots)} \\ & {\qquad = B _ {t} (1 + r _ {t + 1}) P _ {t} ^ {t + 1}} \\ & {\qquad = B _ {t}} \\ & {\qquad = B _ {t} \delta^ {t} \cdot (P _ {t} ^ {0}, P _ {t} ^ {1}, P _ {t} ^ {2}, \ldots)} \\ & {\qquad = \eta_ {t} \cdot (P _ {t} ^ {0}, P _ {t} ^ {1}, P _ {t} ^ {2}, \ldots).} \end{array}
$$

Definition. An equivalent martingale measure with respect to the bank account is called a risk-neutral measure. 

Now we consider a natural application of a risk-neutral measure. 

Definition. A futures contract initiated at time t with maturity date $T$ is a contract where, at time $t ,$ no money is exchanged; at every time $t < u < T$ , the sum of $f _ { u } ^ { T }$ units of money is swapped for $f _ { u - 1 } ^ { T }$ units of money; and finally at time $T _ { \ast }$ the asset with price $S _ { T }$ is swapped for $\bar { f } _ { T - 1 } ^ { \bar { T } }$ units of money, where $\dot { f } _ { s } ^ { T }$ is known at time s for $t \le s \le T$ . The quantity $f _ { t } ^ { T }$ is called the futures price of the asset. 

A futures contract is essentially a portfolio of forward contracts of diferent maturities, with the payout of each forward dependent on the futures prices at the diferent times before maturity. See the diagram for the timing of the payment streams in a futures contract. 

futures 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/4452a2a00e68866b66c2d63b4d8fb8bb5be7caaf3014414afcd7fdab0aa9e2b8.jpg)


Proposition. Consider a market model with a bank account and futures contracts for maturity T initiated at each time u for $t \leq u < T$ . If the market has no arbitrage, then 

$$
f _ {t} ^ {T} = \mathbb {E} ^ {\mathbb {Q}} (S _ {T} | \mathcal {F} _ {t})
$$

where $\mathbb { Q }$ is a risk-neutral measure. 

Proof. By the 1FTAP says that a market with a dividend paying asset is free of arbitrage if and only if there exists a risk-neutral measure $\mathbb { Q }$ , i.e. a measure under which the process M defined by 

$$
M _ {t} = P _ {t} / B _ {t} + \sum_ {s = 1} ^ {t} \delta_ {s} / B _ {s}
$$

is a martingale. In our example, we set $\delta _ { u } = f _ { u } ^ { T } - f _ { u - 1 } ^ { T }$ and $P _ { u } = 0$ for $t \leq u \leq T$ , where $f _ { T } ^ { T } = S _ { T }$ 

Note 

$$
\begin{array}{c} 0 = \mathbb {E} ^ {\mathbb {Q}} [ M _ {u + 1} - M _ {u} | \mathcal {F} _ {u} ] = \mathbb {E} ^ {\mathbb {Q}} [ (f _ {u + 1} ^ {T} - f _ {u} ^ {T}) / B _ {u + 1} | \mathcal {F} _ {u} ] \\ = \left(\mathbb {E} ^ {\mathbb {Q}} [ f _ {u + 1} ^ {T} | \mathcal {F} _ {u} ] - f _ {u} ^ {T}\right) / B _ {u + 1} \end{array}
$$

by the $\mathcal { F } _ { u }$ -measurability of $B _ { u + 1 }$ . Hence $( f _ { u } ^ { T } ) _ { t \leq u \leq T }$ is a $\mathbb { Q } \mathrm { . }$ -martingale. 

Remark. Let $f _ { t } ^ { T }$ be the futures price of a stock at time t for maturity T. If $T \mapsto f _ { t } ^ { T }$ is non-decreasing, the market for that stock is said to be in contango at time t. And if $T \mapsto f _ { t } ^ { T }$ is non-increasing, the market is said to be in normal backwardation. 

Forward measures and risk-neutral measures are in general diferent. In particular, forward prices and futures prices usually disagree. But there is an important example where they agree: 

Proposition. Suppose that the spot interest rate process is not random. A probability measure is a T-forward measure if and only if it is risk-neutral. 

Proof. The fundamental result is that if B is a non-random process then 

$$
P _ {t} ^ {T} = \frac {B _ {t}}{B _ {T}}.
$$

This formula can be seen as an instance of the law of one price; see the first example sheet. But here is the quick dual argument: Since both $Y P ^ { T }$ and $Y B$ are martingales we have 

$$
\begin{array}{r l} & B _ {t} = \frac {1}{Y _ {t}} \mathbb {E} (B _ {T} Y _ {T} | \mathcal {F} _ {t}) \\ & \quad = \frac {B _ {T}}{Y _ {t}} \mathbb {E} (P _ {T} ^ {T} Y _ {T} | \mathcal {F} _ {t}) \\ & \quad = B _ {T} P _ {t} ^ {T}. \end{array}
$$

Now, since $B _ { T }$ is assumed to be a constant, the process $( S _ { t } / B _ { t } ) _ { 0 \leq t \leq T }$ is a martingale with respect to a certain measure if and only if $( S _ { t } / P _ { t } ^ { T } ) _ { 0 \leq t \leq T }$ is a martingale with respect to the same measure.  

## 9. Contingent claim pricing and hedging

The setting of this section is as follows. We find ourselves in a market with prices $( P _ { t } ) _ { t \geq 0 }$ A contingent claim is any cash payment where the size of the payment is contingent on the prices of other assets or any other variable<sup>3</sup> There are two major types of contingent claims that we will study in these notes: European and American. 

European: specified by a time horizon $T > 0$ and $\mathcal { F } _ { T }$ -measurable random variable $\xi _ { T }$ modelling the payout at the maturity date $T$ 

American: specified by a time horizon $T > 0$ and an adapted process $( \xi _ { t } ) _ { 0 \leq t \leq T }$ where $\xi _ { t }$ models the payout of the claim if the owner of the claim chooses to exercise at time t. 

We put ourselves in the shoes of an investment bank that would like to market a new contingent claim. The question are these: what is a ‘good’ initial price for this claim? How can the seller hedge against the liability of owing the buyer the payout of the claim? 

We first consider European options. 

Example (Forward contract). Given a market for a traded asset with prices $( S _ { t } ) _ { t \geq 0 }$ , a forward contract initiated at a fixed time t for maturity $T$ is a European claim with payout $\xi _ { T } = S _ { T } - F _ { t } ^ { T }$ , where $F _ { t } ^ { T }$ is the forward price at time t for maturity T. We have discussed this example in the previous section. 

Example (Call option). A European call option gives the owner of the option the right, but not the obligation, to buy a given stock at a fixed time $T$ (called the maturity date) at some fixed price K (called the strike). See the figure for the timing of the payments, where $C _ { t }$ is the price of the option at time t and $S _ { T }$ is the price of the stock at the maturity date T. There are two cases: If $K \geq S _ { T }$ , then the option is worthless to the owner since there 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/95cea83b74d5fdde90097c51ef86dc3b331f675306d30cf1cc4a1bf4f12477c7.jpg)


is no point paying a price above the market price for the underlying stock. On the other hand, if $K < S _ { T }$ , then the owner of the option can buy the stock for the price K from the counterparty and immediately sell the stock for the price $S _ { T }$ to the market, realising a profit of $S _ { T } - K$ . Hence, the payout of the call option is $\xi _ { T } = ( S _ { T } - K ) ^ { + }$ , where $a ^ { + } = \operatorname* { m a x } \{ a , 0 \}$ as usual. The ‘hockey-stick’ graph of the function $g ( x ) = ( x - K ) ^ { + }$ is below. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/2c01276ab83ce5b14e2438ef430aedb99c657b0863dd1a733c2b2a9547262add.jpg)


We will assume that the original market has no arbitrage, since otherwise it is dificult to formulate a reasonable answer to the pricing and hedging questions. Therefore, we will assume that there is at least one martingale deflator. 

Proposition. Consider an arbitrage-free market with prices $P .$ Introduce to this market a European contingent claim with maturity T and payout $\xi _ { T }$ . Suppose that for $t < T$ , the price of the claim at time t is $\xi _ { t }$ . If the augmented market with prices $( P _ { t } , \xi _ { t } ) _ { 0 \leq t \leq T }$ has no arbitrage, then 

$$
\underline {{\xi}} _ {t} \leq \xi_ {t} \leq \overline {{\xi_ {t}}} f o r a l l 0 \leq t \leq T
$$

where 

$$
\underline {{\xi}} _ {t} = \mathrm{ess} \inf \bigl \{\frac {1}{Y _ {t}} \mathbb {E} (Y _ {T} \xi_ {T} | \mathcal {F} _ {t}): Y \text {a martingale deflator for the original market} \bigr \}
$$

such that ξ<sub>T</sub>Y<sub>T</sub> is integrable 

and $\overline { { \xi } } _ { t }$ is defined similarly in terms of the essential supremum. 

Proof. This is just the 1FTAP. Indeed, if the augmented market there must be a martingale deflator for the augmented market. Such a martingale deflator is necessarily a martingale deflator for the original market. In particular, if $Y$ is a martingale deflator for the augmented market, then $\begin{array} { r } { \xi _ { t } = \frac { 1 } { Y _ { t } } \mathbb { E } ( Y _ { T } \xi _ { T } | \mathcal { F } _ { t } ) } \end{array}$ . That $\xi _ { t }$ is in the interval $[ \underline { { \xi } } _ { t } , \overline { { \xi } } _ { t } ]$ follows directly from the definition of essential infimum and supremum.  

Remark. We pause briefly to discuss the notions of essential supremum and essential infimum.. Given a collection of random variables $( X _ { k } ) _ { k \in K }$ indexed by an arbitrary (possibly uncountable) set $K$ , a random variable $Y$ is called the essential supremum of the collection, denoted 

$$
Y = \mathrm{ess} \sup _ {k \in K} X _ {k}
$$

if it satisfies 

$Y \geq X _ { k }$ almost surely for all $k \in K$ , and 

• if another random variable $Z$ is such that $Z \geq X _ { k }$ almost surely for all $k \in K$ , then $Z \geq Y$ almost surely. 

The essential infimum of the collection is defined similarly. The proof of the existence of the essential supremum of a family of random variables is on example sheet 2. 

Recall, that in contrast, the function $\hat { Y }$ defined by ${ \hat { Y } } ( \omega ) = \operatorname* { s u p } _ { k \in K } X _ { k } ( \omega )$ has the property that $\hat { Y } \geq X _ { k }$ for all $k \in K$ everywhere, and if $Z$ is another function such that $Z \geq X _ { k }$ for all $k \in K$ everywhere, then $Z \geq { \hat { Y } }$ everywhere. 

Here is an example to show that the ordinary notion of supremum is not the correct notion in certain probabilistic settings. Let the set of outcomes Ω be the interval $[ 0 , 1 ]$ , the set of events $\mathcal { F }$ be the Borel sigma-field and the probability measures $\mathbb { P }$ be the Lebesgue measure. Fix a subset $K \subseteq [ 0 , 1 ]$ and let $X _ { k } = \mathbb { 1 } _ { \{ k \} }$ . Note that $\hat { Y } = \operatorname* { s u p } _ { k } X _ { k } = \mathbb { 1 } _ { K }$ . There are a couple of reasons why $\hat { Y }$ is not very useful probabilistically. 

Firstly, note that $\hat { Y }$ is a measurable map from Ω to R if and only if K is a Borel set. Since K was arbitrary, it is not always the case that $\hat { Y }$ is a random variable. 

Secondly, even if $K$ is measurable and $\hat { Y }$ is a random variable, it is ‘too big’. Indeed, the smaller random variable $Y = 0$ has the property that $Y \geq X _ { k }$ almost surely for all $k \in K$ 

Returning to our application for bounding no-arbitrage prices, we don’t know a priori whether the set of martingale deflators is countable or not. So the ordinary supremum may not be measurable. Furthermore, we only care about almost sure inequality for each martingale deflator (not inequality simultaneously for all martingale deflators for every outcome<sup>4</sup>), the essential supremum and infimum appearing the statement of the result are appropriate. 

The above theorem says that the principle of no-arbitrage usually is not enough to uniquely price a contingent claim. At best, it gives an interval where the no-arbitrage price may lie. However, there is a special class of contingent claims that can be priced uniquely. 

Definition. A European contingent claim with payout $\xi _ { T }$ is replicable or attainable if there exists an initial wealth x and pure investment strategy H such that $X _ { T } ^ { x , H } = \xi _ { T }$ almost surely. (Recall that $X _ { 0 } = x , X _ { t } = H _ { t } \cdot P _ { t }$ for $t \geq 1$ and pure investment means $H _ { t + 1 } \cdot P _ { t } = X _ { t }$ for $t \geq 0$ 

One of the reasons to single out attainable claims is that there is an unambiguous way to price them according to the no-arbitrage principle: 

Theorem (Characterisation of attainable claims). Suppose that the market model with $n \textmd { - }$ dimensional price process P has no arbitrage. Let $\xi _ { T }$ be the payout of a European contingent claim with maturity date $T > 0$ . The following are equivalent: 

(1) The claim is atttainable. 

(2) There exists a unique process $( \xi _ { t } ) _ { 0 \leq t \leq T }$ such that the augmented market $( P , \xi )$ has no arbitrage. 

(3) There exists a number $\xi _ { 0 }$ such that $\mathbb { E } [ Y _ { T } \xi _ { T } ] = Y _ { 0 } \xi _ { 0 }$ for all martingale deflators $( o f$ the original market) such that $Y _ { T } \xi _ { T }$ is integrable. 

Proof. $( 1 ) \Rightarrow ( 2 )$ This is the law of one price from the first example sheet. Indeed, let $\xi _ { t }$ be the price of the claim and $X _ { t }$ be the price of the replicating portfolio at time t. Let $\tau$ be the first time $\xi _ { t } \neq X _ { t }$ . One the event $\{ \tau < T \}$ do the following: at time $\tau$ buy the cheaper one, sell the expensive one, and consume the diference; and at time $T$ unwind both positions for zero cost since $\xi _ { T } = X _ { T }$ by assumption. In notation, let $H$ be the replicating strategy and let consider the strategy $( \tilde { H } , h )$ in the augmented market given by 

$$
(\tilde {H} _ {t}, h _ {t}) = \mathbb {1} _ {\{\tau \leq t - 1 \}} (H _ {t}, - 1) \mathrm{sign} (\xi_ {\tau} - X _ {\tau}) \text {   for   } 1 \leq t \leq T
$$

and $\tilde { H } _ { T + 1 } = 0$ and $h _ { T + 1 } = 0$ . The corresponding consumption stream is 

$$
c _ {t} = \mathbb {1} _ {\{\tau = t \}} | X _ {t} - \xi_ {t} |
$$

This strategy would be an arbitrage unless $\mathbb { P } ( \tau < T ) = 0$ . Hence, no arbitrage in the augmented market implies $\xi _ { t } = X _ { t } \mathrm { ~ a . s ~ }$ . for all $0 \leq t \leq T$ and hence the price process is uniquely determined by the replicating strategy. 

(By the way, the same argument shows that if $X _ { T } ^ { x , H } = X _ { T } ^ { y , K }$ almost surely for possibly diferent strategies H and K initial wealths x and $y ,$ then $X _ { t } ^ { x , \hat { H } } = X _ { t } ^ { y , K }$ almost surely for all $0 \leq t \leq T$ . In particular, two replicating strategies of an attainable claim yield the same no arbitrage price.)  

Proof. $\left( 2 \right) \Rightarrow \left( 3 \right)$ Suppose that there is no arbitrage in the augmented market. Then there exists a martingale deflator Y for that market. In particular, this martingale deflator is a martingale deflator for the original market and also for the new asset. That is, $Y \xi$ is a martingale and in particular, $\mathbb { E } ( Y _ { T } \xi _ { T } ) = Y _ { 0 } \xi _ { 0 }$ . Now, assuming that the initial price $\xi _ { 0 }$ of the claim is uniquely identified yields the result.  

It remains to prove the implication $( 3 ) \Rightarrow ( 1 )$ . We will only prove the $T = 1$ version. Recall that in this setting, the martingale deflator: $Y _ { 0 } ~ > ~ 0 , Y _ { 1 } ~ > ~ 0$ almost surely and $\mathbb { E } ( Y _ { 1 } P _ { 1 } ) = Y _ { 0 } P _ { 0 }$ , can be replaced by the pricing kernel: $\rho > 0$ almost surely and $\mathbb { E } [ \rho P _ { 1 } ] = P _ { 0 }$ 2 by setting $\rho = Y _ { 1 } / Y _ { 0 }$ 

In what follows, we will assume that the one-period market with prices $P _ { 0 } , P _ { 1 }$ has no arbitrage. By the fundamental theorem of asset pricing, there exists a pricing kernel. But, given an arbitrary random variable $\xi _ { 1 }$ , one may worry whether there must exist a pricing kernel $\rho$ such that $\rho \xi _ { 1 }$ is integrable. Fortunately, it turns out that if there is no arbitrage, there does indeed exist at least one pricing kernel $\rho$ such that $\rho \xi _ { 1 }$ is integrable. <sup>5</sup> 

We will proceed by a series of lemmas. 

Lemma. Suppose that there exists a number $\xi _ { 0 }$ such that $\mathbb { E } ( \rho \xi _ { 1 } ) \ : < \ : \xi _ { 0 }$ for all pricing kernels such that $\rho \xi _ { 1 }$ is integrable. Then there exists a portfolio $H \in \mathbb { R } ^ { n }$ such that 

$$
H \cdot P _ {0} \leq \xi_ {0} a n d H \cdot P _ {1} \geq \xi_ {1} a. s.
$$

and there is positive probability that at least one of the above inequalities is strict. 

Proof. By assumption, there does not exist a pricing kernel for the augmented market $( P , \xi )$ . By the fundamental theorem of asset pricing, there exists an arbitrage in the augmented market, i.e. a portfolio $( \tilde { H } , h ) \in \mathbb { R } ^ { n + 1 }$ such that 

$$
\tilde {H} \cdot P _ {0} + h \xi_ {0} \leq 0 \text { and } \tilde {H} \cdot P _ {1} + h \xi_ {1} \geq 0 \text { a.s. }
$$

where there is positive probability that at least one of the above inequalities is strict. 

Let $\rho$ be a pricing kernel for the original market such that $\rho P _ { 1 }$ is integrable. Note that we have 

$$
\begin{array}{r l} & 0 \leq \mathbb {E} [ \rho (\tilde {H} \cdot P _ {1} + h \xi_ {1}) ] \\ & \quad = \tilde {H} \cdot P _ {0} + h \mathbb {E} (\rho \xi_ {1}) \\ & \quad \leq h [ \mathbb {E} (\rho \xi_ {1}) - \xi_ {0} ] \end{array}
$$

Since $\mathbb { E } ( \rho \xi _ { 1 } ) - \xi _ { 0 } < 0$ , we conclude that $h \leq 0 .$ 

We can rule out the case that $h = 0$ . For instance, if $h = 0$ we would have $\tilde { H }$ being an arbitrage in the original market - a contradiction.<sup>6</sup> We are left with $h < 0$ . This shows that $H = - \tilde { H } / h$ satisfies the conclusion of the lemma.  

Lemma. Suppose that there exists a number $\xi _ { 0 }$ such that $\mathbb { E } ( \rho \xi _ { 1 } ) \le \xi _ { 0 }$ for all pricing kernels such that $\rho \xi _ { 1 }$ is integrable. Then there exists a portfolio $H \in \mathbb { R } ^ { n }$ such that 

$$
H \cdot P _ {0} \leq \xi_ {0} a n d H \cdot P _ {1} \geq \xi_ {1} a. s.
$$

Proof. For all $k > 0$ , we have $\mathbb { E } ( \rho \xi _ { 1 } ) < \xi _ { 0 } + 1 / k$ and hence by the previous lemma there exists a portfolio $H _ { k } \in \mathbb { R } ^ { n }$ such that 

$$
H _ {k} \cdot P _ {0} \leq \xi_ {0} + 1 / k \mathrm{and} H _ {k} \cdot P _ {1} \geq \xi_ {1} \mathrm{a.s.}
$$

$$
F (h) = e ^ {h \cdot P _ {0}} + \mathbb {E} [ e ^ {- h \cdot P _ {1}} \zeta ]
$$

and chose the positive random variable such that $F$ was finite valued, and hence smooth. A good choice is We then showed that no arbitrage implied that there exists a minimiser $h ^ { * }$ of $F ,$ and hence 

$$
\rho = \frac {e ^ {- h ^ {*} \cdot P _ {1}}}{e ^ {h ^ {*} \cdot P _ {0}}} \zeta
$$

$\begin{array} { r l } { C a s e : } & { { } ( H _ { k } ) _ { k } } \end{array}$ is bounded. In this case, we can pass to a convergent subsequence such that $H _ { k } \to H ^ { * }$ . Note 

$$
H ^ {*} \cdot P _ {0} \leq \xi_ {0} \text { and } H ^ {*} \cdot P _ {1} \geq \xi_ {1} \text { a.s. }
$$

as desired. 

Case: $( H _ { k } ) _ { k }$ is unbounded. Recall from the proof of the 1FTAP the notation 

$$
\mathcal {U} = \left\{u \in \mathbb {R} ^ {n}: u \cdot P _ {0} = 0 = u \cdot P _ {1} \text { a   .   s   . } \right\}
$$

and 

$$
\mathcal {V} = \mathcal {U} ^ {\perp}.
$$

By projecting our given sequence onto V, we can assume that $H _ { k } \in \mathcal { V }$ for all k and that $( H _ { k } ) _ { k }$ is unbounded (otherwise, we are back to the previous case). We can pass to a subsequence such that $\| H _ { k } \| \to \infty$ and to a further subsequence such that $\hat { H } _ { k } = H _ { k } / \lVert H _ { k } \rVert$ converges to a non-zero<sup>7</sup> is limit $\hat { H } \in \nu$ . Now dividing the inequalities by $\| H _ { k } \|$ and taking the limit yields 

$$
\hat {H} \cdot P _ {0} \leq 0 \leq \hat {H} \cdot P _ {1} \mathrm{a.s.}
$$

By no arbitrage, we have $\hat { H } \cdot P _ { 0 } = 0 = \hat { H } \cdot P _ { 1 }$ a.s., or in other notation ${ \hat { H } } \in { \mathcal { U } } .$ . Since $\hat { H }$ is in V, we have $\hat { H } = 0$ , a contradiction. This shows that this second case is impossible.  

Proof of $( 3 ) \Rightarrow ( 1 )$ in one period. Suppose that there exists a number $\xi _ { 0 }$ such that $\mathbb { E } ( \rho \xi _ { 1 } ) = \xi _ { 0 }$ for all pricing kernels such that $\rho \xi _ { 1 }$ is integrable. Note that 

$$
\mathbb {E} (\rho \xi_ {1}) \leq \xi_ {0} \text { for   all } \rho
$$

so that there exists a portfolio $H ^ { + } \in \mathbb R ^ { n }$ such that 

$$
H ^ {+} \cdot P _ {0} \leq \xi_ {0} \mathrm{and} H ^ {+} \cdot P _ {1} \geq \xi_ {1} \mathrm{a.s.}
$$

Similarly, 

$$
\mathbb {E} [ \rho (- \xi_ {1}) ] \leq - \xi_ {0} \text {   for   all   } \rho
$$

so that there exists a portfolio $H ^ { - } \in \mathbb { R } ^ { n }$ such that 

$$
H ^ {-} \cdot P _ {0} \leq - \xi_ {0} \text { and } H ^ {-} \cdot P _ {1} \geq - \xi_ {1} \text { a.s. }
$$

Adding this together yields 

$$
\left(H ^ {+} + H ^ {-}\right) \cdot P _ {0} \leq 0 \leq \left(H ^ {+} + H ^ {-}\right) \cdot P _ {1} \text { a   .   s   . }
$$

By no arbitrage in the original market, we have 

$$
\left(H ^ {+} + H ^ {-}\right) \cdot P _ {0} = 0 = \left(H ^ {+} + H ^ {-}\right) \cdot P _ {1} \mathrm{a.s.}
$$

Hence the portfolios $H = H ^ { + }$ and $H = - H$ <sup>−</sup> satisfy the desired conclusion. 

Example. (Put-call parity formula) Suppose we start with a market with three assets with prices $( B _ { t } ^ { T } , S _ { t } , C _ { t } ) _ { 0 \leq t \leq T }$ The first asset is a bond with maturity date $T$ and unit principal value, so that in particular, $B _ { T } ^ { T } = 1$ almost surely. The next asset is a stock. The last asset is a call option on that stock with strike K and maturity $T _ { \ast }$ , so that $C _ { T } = ( S _ { T } - K ) ^ { + }$ Suppose that this market is free of arbitrage. 

Now we introduce another claim, called a put option. A put option gives the owner of the option the right, but not the obligation, to sell the stock for a fixed strike price at a fixed maturity date. If the strike is K and maturity date is $T _ { i }$ , then a similar argument as we used for the call option, the payout of a put option is $P _ { T } = ( K - S _ { T } ) ^ { + }$ 

It turns out that the put option is replicable in the market $( B ^ { T } , S , C )$ . Indeed, we have the identity 

$$
\begin{array}{r l} & P _ {T} = (K - S _ {T}) ^ {+} \\ & \quad = K - S _ {T} + (S _ {T} - K) ^ {+} \\ & \quad = (K, - 1, + 1) \cdot (B _ {T} ^ {T}, S _ {T}, C _ {T}). \end{array}
$$

Hence $H _ { t } = ( K , - 1 , + 1 )$ for all $1 \leq t \leq T$ is a replicating strategy. 

Now, suppose we want to assign prices $P _ { t }$ to the put for $0 \leq t < T$ . The above theorem says there is no arbitrage in the augmented market $( B ^ { T } , S , C , P )$ if and only if 

$$
\boxed {P _ {t} - C _ {t} = K B _ {t} ^ {T} - S _ {t}}
$$

This is the famous put-call parity formula. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/7d198df1be51e94fd78301e31de16d36002ad956265fa5b7f8de057151176d85.jpg)



Figure 1. A plot of $P _ { 0 } - C _ { 0 }$ versus K, where $t = 0$ corresponds to 23 October 2017 and and $t = T$ is 17 November 2017, and the underlying asset is the S&P 500 index with $S _ { 0 } = 2 , 5 7 3 . 8 2$ . The price of the calls and puts is taken to be the last traded price on the day (as opposed to the bid or ask price). All data is taken from https://uk.finance.yahoo.com.


Since attainable claims have unique no-arbitrage prices, we single out the markets for which every claim is attainable: 

Definition. A market is complete if and only if every European contingent claim is attainable. A market is incomplete otherwise. 

In discrete time models complete markets have a lot (probably too much) structure: 

Theorem. If the market model P with n assets is complete, then for each $t \geq 0$ the probability space Ω can be partitioned into no more than n<sup>t</sup> $\mathcal { F } _ { t }$ -measurable events of positive probability, and in particular, the n-dimensional random vector $P _ { t }$ takes values in a set of at most $n ^ { t }$ elements. 

Proof. We will proceed by induction. First suppose $A _ { 1 } , \ldots , A _ { k }$ are a collection of disjoint F<sub>t</sub>-measurable events with $\mathbb { P } ( A _ { i } ) > 0$ for all i. Claim: the set $\left\{ \mathbb { 1 } _ { A _ { 1 } } , \ldots , \mathbb { 1 } _ { A _ { k } } \right\}$ is linearly independent, and in particular, the dimension of the span of $\left\{ \mathbb { 1 } _ { A _ { 1 } } , \ldots , \mathbb { 1 } _ { A _ { k } } \right\}$ is exactly k. Indeed, we must show that if 

$$
a _ {1} \mathbb {1} _ {A _ {1}} + \dots a _ {k} \mathbb {1} _ {A _ {k}} = 0 \text { a.s. }
$$

for some constants $a _ { 1 } , \ldots , a _ { k }$ , then $a _ { 1 } = \cdots = a _ { k } = 0$ . To this end, note that if $i \neq j$ the sets $A _ { i }$ and $A _ { j }$ are disjoint and hence $\mathbb { 1 } _ { A _ { i } } \mathbb { 1 } _ { A _ { i } } = 0$ . By multiplying both sides of the equation by $\mathbb { 1 } _ { A _ { i } }$ we get $a _ { i } \mathbb { 1 } _ { A _ { i } } = 0$ . But since $\mathbb { P } ( A _ { i } ) \stackrel { \cdot } { > } 0$ it must be the case that $a _ { i } = 0$ , proving the claim. 

Since the market is complete, each of the $\mathbb { 1 } _ { A _ { i } }$ is replicable. Hence 

$$
\operatorname{span} \left\{\mathbb {1} _ {A _ {1}}, \dots , \mathbb {1} _ {A _ {k}} \right\} \subseteq \left\{H _ {t} \cdot P _ {t}: H _ {t} \text {   is   } \mathcal {F} _ {t - 1} \text {-meas. } \right\}
$$

Now let $B _ { 1 } , \ldots , B _ { N }$ be a maximal partition of Ω into disjoint $\mathcal { F } _ { t }$ -measurable sets of positive measure, where by the induction hypothesis $N \leq n ^ { t - 1 }$ . If a random vector $H _ { t }$ is $\mathcal { F } _ { t - 1 }$ -measurable, then it takes exactly one value on each of the $B _ { j } \mathrm { ^ { * } s }$ for a total of at most $N$ values $h _ { 1 } , \ldots , h _ { N }$ . Hence 

$$
\begin{array}{c} \{H _ {t} \cdot P _ {t}: H _ {t} \text {is} \mathcal {F} _ {t - 1} \text {-meas.} \} = \{h _ {1} \cdot P _ {t} \mathbb {1} _ {B _ {1}} + \ldots + h _ {N} \cdot P _ {t} \mathbb {1} _ {B _ {N}}: h _ {1}, \ldots , h _ {N} \in \mathbb {R} ^ {n} \} \\ = \operatorname{span} \{P _ {t} ^ {i} \mathbb {1} _ {B _ {j}}: 1 \leq i \leq n, 1 \leq j \leq N \} \end{array}
$$

and the dimension of the space above is at most $n N$ 

Therefore, we have shown $k \leq n N \leq n ^ { t }$ , completing the induction. 

We can characterise complete markets: 

Theorem (Second Fundamental Theorem of Asset Pricing). An arbitrage-free market model is complete if and only if there exists a unique martingale deflator Y such that $Y _ { 0 } = 1$ 

Proof. (‘if’ direction) Let Y and $Y ^ { \prime }$ be martingale deflators with $Y _ { 0 } = 1 = Y _ { 0 } ^ { \prime }$ . Suppose the market is complete, fix a non-random time $T > 0$ and consider the claim with payout $\xi _ { T } = Y _ { T } - Y _ { T } ^ { \prime }$ . By completeness, there exists $( x , H )$ such that $X _ { T } ^ { x , H } = \xi _ { T }$ . By completeness, every F -measurable random variable is bounded (since it can take at most $n ^ { T }$ diferent values) so both $Y _ { T } \xi _ { T }$ and $Y _ { T } ^ { \prime } \xi _ { T }$ are integrable. In particular, we have 

$$
\mathbb {E} [ Y _ {T} \xi_ {T} ] = x = \mathbb {E} [ Y _ {T} ^ {\prime} \xi_ {T} ].
$$

Subtracting the left and right side of the above equation yields $\mathbb { E } [ ( Y _ { T } - Y _ { T } ^ { \prime } ) ^ { 2 } ] = 0$ from which the uniqueness of the martingale deflator follows. 

(‘only if’ direction) Suppose there is a unique martingale deflator such that $Y _ { 0 } ~ = ~ 1$ Then for every contingent claim with payout $\xi _ { T }$ there exists a unique number $\xi _ { 0 }$ such that $\mathbb { E } ( Y _ { T } \xi _ { T } ) = \xi _ { 0 }$ for every (that is, the unique) martingale deflator. By the characterisation of attainability, we have $\xi _ { T }$ is attainable, as desired.  


This box summarises the fundamental theorems:


<table><tr><td>1FTAP:</td><td colspan="3">No arbitrage ⇔ Existence of martingale deflator</td></tr><tr><td>2FTAP:</td><td colspan="3">Completeness + No arb ⇔ Uniqueness of martingale deflator</td></tr></table>

Finally, we close this section with another useful consequence of completeness: 

Proposition. Suppose the arbitrage-free market model in complete. Then there exists a bank account. 

Proof. By completeness, bonds of all maturities can be replicated. Hence a bank account can be constructing by holding all the wealth during the period $( t - 1 , t ]$ in the bond with maturity t.  

## 10. Replication with calls and puts

We consider a market consisting of a bond, a stock with time-T price $S _ { T } ~ \ge ~ 0$ , and a family of European calls and puts with strikes in a finite set ${ \mathcal { K } } = \{ K _ { 1 } , \ldots , K _ { N } \} \subseteq ( 0 , \infty )$ all with maturity T. 

Theorem. Suppose g is piece-wise linear with kinks precisely at the points K. Then the European claim with time T payout $\xi _ { T } = g ( S _ { T } )$ can is attainable. 

Proof. Note that g is diferentiable everywhere except K. For every $a \not \in \mathcal { K }$ , note that the following identity holds 

$$
g (s) = g (a) + g ^ {\prime} (a) (s - a) + \sum_ {K \in \mathcal {K}, K <   a} \Delta_ {K} (K - s) ^ {+} + \sum_ {K \in \mathcal {K}, K > a} \Delta_ {K} (s - K) ^ {+}
$$

where $\Delta _ { K } = g ^ { \prime } ( K + ) - g ^ { \prime } ( K - )$ . Hence the replicating strategy is to hold $g ( a ) - a g ^ { \prime } ( a )$ shares of the bond, to hold $g ^ { \prime } ( a )$ shares of stock, and holding $\Delta _ { K }$ puts of strike $K < a$ and $\Delta _ { K }$ calls of strike $K > a$ for all $K \in \mathcal { K }$  

Remark. To prove the identity, note that 

$$
g (x) = g (0) + g ^ {\prime} (0) x + + \sum_ {K \in \mathcal {K}} \Delta_ {K} (x - K) ^ {+}
$$

for all $x \geq 0$ and 

$$
g ^ {\prime} (x) = g ^ {\prime} (0) + \sum_ {K \in \mathcal {K}, K <   x} \Delta_ {K}
$$

for $x \notin K$ , so that 

$$
\begin{array}{c} g (s) - g (a) - g ^ {\prime} (a) (s - a) = \sum_ {K \in \mathcal {K}} \Delta_ {K} [ (s - K) ^ {+} - (a - K) ^ {+} - (s - a) \mathbb {1} _ {\{K <   a \}} ] \\ = \sum_ {K \in \mathcal {K}, K <   a} \Delta_ {K} (K - s) ^ {+} + \sum_ {K \in \mathcal {K}, K > a} \Delta_ {K} (s - K) ^ {+}. \end{array}
$$

Remark. In fact, when $g$ is twice continuously diferentiable, the continuous analogue of the above identity holds 

$$
g (s) = g (a) + g ^ {\prime} (a) \left(S _ {1} - a\right) + \int_ {0} ^ {a} g ^ {\prime \prime} (K) (K - s) ^ {+} d K + \int_ {a} ^ {\infty} g ^ {\prime \prime} (K) (s - K) ^ {+} d K
$$

for any $a > 0$ . Note that the integrand of the first integral is zero unless min $\left\{ s , a \right\} \ \leq$ $K \leq a$ . Similarly, the integrand of the second integral is zero unless $a \le K \le \operatorname* { m a x } \{ s , a \}$ In particular, the ranges of both integrals are bounded intervals on which $g ^ { \prime \prime }$ is assumed continuous, so both integrals are ordinary Riemann integrals. 

(One way to prove this identity is to fix s and let $h ( a )$ equal the right-hand side. By the standard rules of calculus, we have $h ^ { \prime } ( a ) = 0$ and hence $h ( a )$ is a constant. To evaluate that constant, let $a = s$ and note that both integrals vanish since the ranges of integration have zero length.) 

Consider the case $g ( s ) = \log { s }$ . We have the identity 

$$
\log S _ {T} = \log a + \frac {S _ {T} - a}{a} - \int_ {0} ^ {a} \frac {(K - S _ {T}) ^ {+}}{K ^ {2}} d K - \int_ {a} ^ {\infty} \frac {(S _ {T} - K) ^ {+}}{K ^ {2}} d K.
$$

This formula is interpreted to mean that a claim with payout $\xi _ { T } = \log S _ { T }$ can be approximately replicated by trading in calls and puts over a large number of strikes. 

Although in reality there do not exist contingent claims with log payouts, market practitioners often think of this log contract as being traded since it can be manufactured (approximately) by calls and puts in a straight-forward manner. This line of thinking has lead to the introduction of variance swap contracts which we will consider in the chapter on continuous time models. 

The above result says that given enough call prices, it is possible to replicate any claim with payout of the form $g ( S _ { T } )$ , assuming $g$ is piece-wise linear (or at least to replicate approximately in the case where $g$ is smooth enough to be approximated by a piece-wise linear function). Assuming we know the initial prices of theses call, we can then calculate the initial cost of the approximate hedging portfolio. 

We now come to a simple result observed by Breeden and Litzenberger in 1978. Our setting is a market with prices $( P ^ { T } , S )$ where the first asset is a bond of maturity $T$ , let $\mathbb { Q } \sim \mathbb { P }$ be a T-forward measure, so that $\mathbb { E } ^ { \mathbb { Q } } ( S _ { T } ) = S _ { 0 } / P _ { 0 } ^ { T }$ . Let $C _ { T } ^ { T , K } = ( S _ { T } - K ) ^ { + }$ be the payout of a call with strike $K \geq 0$ , and let the initial prices be 

$$
C _ {0} ^ {T, K} = P _ {0} ^ {T} \mathbb {E} ^ {\mathbb {Q}} [ (S _ {T} - K) ^ {+} ].
$$

Then for any collection of strikes $\mathcal { K } = \{ K _ { 1 } , . . . , K _ { N } \}$ the augmented market with prices $( P ^ { T } , S , C ^ { T , K } ) _ { K \in \mathcal { K } }$ has no arbitrage by the easy direction of the first fundamental theorem, since $\mathbb { Q }$ is a forward measure for the augmented market. 

Note that the function $K \mapsto C _ { 0 } ^ { T , K }$ is convex and therefore has right- and left- derivatives at each point. The following gives meaning to these derivatives: 

Proposition (Breeden–Litzenberger formula). For any $K \geq 0$ we have 

$$
\mathbb {Q} (S _ {T} > K) = \frac {1}{P _ {0} ^ {T}} D _ {K} ^ {+} C _ {0} ^ {T, K}
$$

and 

$$
\mathbb {Q} (S _ {T} \geq K) = \frac {1}{P _ {0} ^ {T}} D _ {K} ^ {-} C _ {0} ^ {T, K}.
$$

If $K \mapsto C _ { 0 } ^ { T , K }$ is twice-diferentiable then the law of the random variable $S _ { T }$ has a density $f _ { S _ { T } }$ under $\mathbb { Q }$ given $b y$ 

$$
f _ {S _ {T}} (K) = \frac {1}{P _ {0} ^ {T}} D _ {K} ^ {2} C _ {0} ^ {T, K}.
$$

Proof. Note that 

$$
\begin{array}{r} D ^ {+} C _ {0} (K) = \lim _ {\varepsilon \downarrow 0} \frac {C _ {0} (K + \varepsilon) - C _ {0} (K)}{\varepsilon} \\ = - P _ {0} ^ {T} \lim _ {\varepsilon \downarrow 0} \mathbb {E} ^ {\mathbb {Q}} [ g _ {\varepsilon} (S _ {T} - K) ] \end{array}
$$

where 

$$
g _ {\varepsilon} (x) = \frac {x}{\varepsilon} \mathbb {1} _ {[ 0, \varepsilon)} + \mathbb {1} _ {[ \varepsilon , \infty)} (x).
$$

Note that $g _ { \varepsilon }$ is bounded and $g _ { \varepsilon } \to \mathbb { I } _ { ( 0 , \infty ) }$ pointwise, so the first formula is proven by by the dominated convergence theorem. The formula for the left-derivative is proven similarly. 

Finally, if $C _ { 0 }$ is twice-diferentiable the density is recovered by diferentiating once more with respect to K.  

## 11. Call prices from moment generating functions

Since a portfolio of calls and puts on a stock can essentially replicate any European contingent claim, it is important to have models where the call prices can be computed easily. Unfortunately, there are few models where there exists nice, elementary formulae for the call prices. However, there are many models (especially when we get to continuous time) where the moment generating functions can be computed explicitly, and we will now see that given the moment generating function we can compute call prices by integration: 

Consider a market model with a bond of maturity T, a stock with $S _ { T } \geq 0$ almost surely, and let Q be a fixed T-forward measure. Let 

$$
C _ {0} ^ {T, K} = P _ {0} ^ {T} \mathbb {E} ^ {\mathbb {Q}} [ (S _ {T} - K) ^ {+} ]
$$

for $K > 0$ , so that if $C _ { 0 } ^ { T , K }$ is the initial price of a call with strike $K$ , then the augmented market has no arbitrage. 

For complex θ in the vertical strip 

$$
\Theta = \{\theta = p + \mathrm{i} q: 0 \leq p \leq 1, q \in \mathbb {R} \}
$$

define the moment generating function of the log stock price by 

$$
M (\theta) = \mathbb {E} ^ {\mathbb {Q}} (e ^ {\theta \log S _ {T}} \mathbb {1} _ {\{S _ {T} > 0 \}}).
$$

Note that we have for $\theta = p + \mathrm { i } q \in \Theta$ 

$$
\begin{array}{r l} & {\mathbb {E} ^ {\mathbb {Q}} (| e ^ {\theta \log S _ {T}} \mathbb {1} _ {\{S _ {T} > 0 \}} |) = \mathbb {E} ^ {\mathbb {Q}} (S _ {T} ^ {p})} \\ & {\qquad \leq \mathbb {E} ^ {\mathbb {Q}} (S _ {T}) ^ {p}} \\ & {\qquad = \left(\frac {S _ {0}}{P _ {0} ^ {T}}\right) ^ {p} <   \infty} \end{array}
$$

by Jensen’s inequality, so the moment generating function is well-defined and finite-valued – indeed it is analytic on Θ but we do not use this fact below. The following result shows how to recover call prices from the moment generating function. 

Theorem. For any $0 < p < 1$ the identity 

$$
C _ {0} ^ {T, K} = S _ {0} - \frac {K ^ {1 - p} P _ {0} ^ {T}}{2 \pi} \int_ {- \infty} ^ {\infty} \frac {M (p + i x) e ^ {- \mathrm{i} x \log K}}{(x - \mathrm{i} p) (x + \mathrm{i} (1 - p))} d x
$$

holds. 

Essentially, we are inverting the moment generating function via a complex integral. Variants of this procedure are often called a Bromwich, Fourier or Mellin transform. To prove this formula, we begin with a lemma: 

Lemma. For any $0 < p < 1$ the identity 

$$
\frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \frac {e ^ {\mathrm{i} a x}}{(x - \mathrm{i} p) (x + \mathrm{i} (1 - p))} d x = \left\{ \begin{array}{l l} e ^ {- a p} & \text {if} a \geq 0 \\ e ^ {a (1 - p)} & \text {if} a <   0 \end{array} \right.
$$

holds. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/7d8bbcea75e57e982b8564eb36da9aa4d23df54ece963dd4cd966cc5bd452907.jpg)


Proof. This is a standard application of the Cauchy residue theorem. Consider the case $a \geq 0$ . Define the semi-circular contour 

$$
\Gamma_ {R} = \{x + \mathrm{i} 0: - R \leq x \leq R \} \cup \left\{R e ^ {\mathrm{i} \phi}: 0 \leq \phi \leq \pi \right\}
$$

in the upper half-plane. Cauchy’s theorem 

$$
\begin{array}{r} \int_ {\Gamma_ {R}} \frac {e ^ {\mathrm{i} a z}}{(z - \mathrm{i} p) (z + \mathrm{i} (1 - p))} d z = \mathrm{i} 2 \pi \frac {e ^ {\mathrm{i} a z}}{z + \mathrm{i} (1 - p)} \bigg | _ {z = \mathrm{i} p} \\ = 2 \pi e ^ {- a p} \end{array}
$$

since the integrand is meromorphic with a simple pole at $z = \mathrm { i } p$ inside the contour, and the contour integral is evaluated in the anticlockwise sense. 

On the other hand, 

$$
\int_ {\Gamma_ {R}} \frac {e ^ {\mathrm{i} a z}}{(z - \mathrm{i} p) (z + \mathrm{i} (1 - p))} d z = \int_ {- R} ^ {R} \frac {e ^ {\mathrm{i} a x}}{(x - \mathrm{i} p) (x + \mathrm{i} (1 - p))} d x + \int_ {0} ^ {\pi} \frac {\mathrm{i} R e ^ {- a R \sin \phi} e ^ {\mathrm{i} (a R \cos \phi + \phi)}}{(R e ^ {i \phi} - \mathrm{i} p) (R e ^ {\mathrm{i} \phi} + \mathrm{i} (1 - p))} d \phi
$$

and the second integral vanishes as $R \to \infty$ since $a \geq 0$ 

The case $a < 0$ is handled in exactly the same way; just integrate around a semi-circular contour in the lower half-plane enclosing the other pole at $- \mathrm { i } ( 1 - p )$  

Proof of theorem. From the lemma, we have the identity 

$$
\begin{array}{l} (S _ {T} - K) ^ {+} S _ {T} - S _ {T} \wedge K \\ = S _ {T} - \frac {K ^ {1 - p}}{2 \pi} \int_ {- \infty} ^ {\infty} \frac {e ^ {p \log S _ {T} + \mathrm{i} x \log (S _ {1} / K)} \mathbb {1} _ {\{S _ {T} > 0 \}}}{(x - \mathrm{i} p) (x + \mathrm{i} (1 - p))} d x. \end{array}
$$

Now multiply by $P _ { 0 } ^ { T }$ and compute expectations. The result follows upon interchanging expectation and integration on the right-hand side. This is justified by Fubini’s theorem since 

$$
\int_ {- \infty} ^ {\infty} \mathbb {E} ^ {\mathbb {Q}} \left| \frac {e ^ {p \log S _ {T} + \mathrm{i} x \log (S _ {1} / K)}}{(x - \mathrm{i} p) (x + \mathrm{i} (1 - p))} \right| d x = M (p) \int_ {- \infty} ^ {\infty} \frac {d x}{\sqrt {(x ^ {2} + p ^ {2}) (x ^ {2} + (1 - p) ^ {2})}} <   \infty
$$

## 12. Super-replication of American claims

We now discuss American claims. Here, things are quite diferent. The canonical example of an American claim is the American put option– a contract which gives the buyer the right (but not the obligation) to sell the underlying stock at a fixed strike price $K > 0$ at any time between time 0 and a fixed maturity date $T .$ Hence, the payout of the option is $( K - S _ { \tau } ) ^ { + }$ where $\tau \in \{ 0 , \ldots , T \}$ is a time chosen by the holder of the put to exercise the option. 

The payout of an American claim is specified by two ingredients: 

• a maturity date $T > 0$ 2 

• an adapted process $( \xi _ { t } ) _ { 0 \leq t \leq T }$ 

For instance, in the case of an American put, we may take $\xi _ { t } \ : = \ : ( K - S _ { t } ) ^ { + }$ . Unlike the European claim, the holder of an American claim can choose to exercise the option at any time $\tau$ before or at maturity. However, to rule out clairvoyance, we insist that $\tau$ is a stopping time. 

Now, if an American claim matures at $T > 0$ and is specified by the payout process $( \xi _ { t } ) _ { 0 \leq t \leq T }$ , then the actual payout of the claim is modelled by the random variable $\xi _ { \tau }$ , where τ is any stopping time for the filtration taking values in $\{ 0 , \ldots , T \}$ 

We can think of the American claim then as a family, indexed by the stopping time $\tau ,$ of European claims with payouts $\xi _ { \tau }$ . To simplify matters, we make the following assumption in this subsection: 

The market model $P = ( P _ { t } ) _ { 0 \leq t \leq T }$ is complete. 

Let $Y = ( Y _ { t } ) _ { 0 \leq t \leq T }$ be the unique martingale deflator such that $Y _ { 0 } = 1$ 

Intuitively, the seller of such a claim should at time 0 charge at least the amount 

$$
\sup _ {\tau \leq T} \mathbb {E} \left(Y _ {\tau} \xi_ {\tau}\right)
$$

to be sure that he can hedge the option, where the supremum is taken over the set of stopping times smaller than or equal to $T$ . Indeed, this is the case. 

Theorem. Suppose that the adapted process $( \xi _ { t } ) _ { 0 \le t \le T }$ specifies the payout ofan American claim maturing at $T > 0$ 

There exists a self-financing pure-investment trading strategy H such that 

• X<sub>t</sub> ≥ ξ<sub>t</sub> for all 0 ≤ t ≤ T, 

$X _ { \tau ^ { * } } = \xi _ { \tau ^ { * } } \ f o r$ some stopping time $\tau ^ { * }$ , and 

$\begin{array} { r } { X _ { 0 } = \operatorname* { s u p } _ { \tau \leq T } \mathbb E \left( Y _ { \tau } \xi _ { \tau } \right) } \end{array}$ 

where $X _ { t } = H _ { t } \cdot P _ { t } = H _ { t + 1 } \cdot P _ { t }$ 

Remark. The strategy H dominates the payout of the American claim at all times, but is conservative in the sense that it exactly replicates the optimally exercised claim. 

The rest of this subsection is dedicated to proving this theorem. 

***** 

We will need a result of general interest: 

Theorem (Doob decomposition theorem). Let U be a discrete-time supermartingale. Then there is a unique decomposition 

$$
U _ {t} = U _ {0} + M _ {t} - A _ {t}
$$

where M is a martingale and A is a predictable non-decreasing process with $M _ { 0 } = A _ { 0 } = 0$ 

Proof. Let $M _ { 0 } = 0 = A _ { 0 }$ and define 

$$
\begin{array}{r} M _ {t + 1} = M _ {t} + U _ {t + 1} - \mathbb {E} (U _ {t + 1} | \mathcal {F} _ {t}) \\ A _ {t + 1} = A _ {t} + U _ {t} - \mathbb {E} (U _ {t + 1} | \mathcal {F} _ {t}) \end{array}
$$

for $t \geq 0$ . Since U is assumed to be supermartingale, and hence integrable, the processes M and A are integrable. It is straightforward to check that M is a martingale, and since U is a supermartingale, that A is non-decreasing. Also by induction, we see that $A _ { t + 1 }$ is F -measurable. 

Summing up, 

$$
\begin{array}{c} M _ {t} - A _ {t} = M _ {0} - A _ {0} + \sum_ {s = 1} ^ {t} (M _ {s} - M _ {s - 1} - A _ {s} + A _ {s - 1}) \\ = \sum_ {s = 1} ^ {t} (U _ {s} - U _ {s - 1}) \\ = U _ {t} - U _ {0}. \end{array}
$$

To show uniqueness, assume that $U _ { t } = U _ { 0 } + M _ { t } - A _ { t } = U _ { 0 } + M _ { t } ^ { \prime } - A _ { t } ^ { \prime }$ . Then $M - M ^ { \prime }$ is a predictable discrete-time martingale, that is, a constant.  

Now we introduce the key concept in optimal stopping theory: 

Definition. Let $( Z _ { t } ) _ { 0 \leq t \leq T }$ be a given integrable adapted discrete-time process. Define an adapted process $( U _ { t } ) _ { 0 \leq t \leq T }$ by the recursion 

$$
U _ {T} = Z _ {T}
$$

$$
U _ {t} = \max \{Z _ {t}, \mathbb {E} (U _ {t + 1} | \mathcal {F} _ {t}) \} \mathrm{for} 0 \leq t \leq T - 1.
$$

The process $( U _ { t } ) _ { 0 \leq t \leq T }$ is called the Snell envelope of $( Z _ { t } ) _ { 0 \leq t \leq T }$ 

Remark. The Snell envelope clearly satisfies both 

$$
U _ {t} \geq Z _ {t} \text {   and   } U _ {t} \geq \mathbb {E} (U _ {t + 1} | \mathcal {F} _ {t})
$$

almost surely. Thus, another way to describe the Snell envelope of a process is to say it is the smallest supermartingale dominating that process. 

In our application Z will be the process $Y \xi _ { }$ , where $Y$ is the martingale deflator and $\xi$ is the process specifying the payout of the American claim. 

Theorem. Let $( Z _ { t } ) _ { 0 \leq t \leq T }$ be an integrable adapted process, let $( U _ { t } ) _ { 0 \leq t \leq T }$ be its Snell $e n \cdot$ velope with Doob decomposition $U _ { t } = U _ { 0 } + M _ { t } - A _ { t }$ . Let $A _ { T + 1 } = + \infty$ and 

$$
\tau^ {*} = \min \{t \in \{0, \dots , T \}: A _ {t + 1} > 0 \}.
$$

Then $\tau ^ { * }$ is a stopping time and 

$$
U _ {\tau^ {*}} = U _ {0} + M _ {\tau^ {*}} = Z _ {\tau^ {*}}.
$$

Proof. That $\tau ^ { * }$ is a stopping time follows from the fact that the non-decreasing process $( A _ { t } ) _ { 0 \leq t \leq T + 1 }$ is predictable. 

Now note that 

$$
\mathbb {E} (U _ {t + 1} | \mathcal {F} _ {t}) = \mathbb {E} (U _ {0} + M _ {t + 1} - A _ {t + 1} | \mathcal {F} _ {t}) = U _ {0} + M _ {t} - A _ {t + 1}
$$

since M is a martingale and A is predictable so that by the definition of Snell envelope 

$$
U _ {0} + M _ {t} - A _ {t} = \max \{Z _ {t}, U _ {0} + M _ {t} - A _ {t + 1} \}.
$$

Note that $A _ { \tau ^ { * } } = 0$ and hence 

$$
U _ {0} + M _ {\tau^ {*}} = \max \left\{Z _ {\tau^ {*}}, U _ {0} + M _ {\tau^ {*}} - A _ {\tau^ {*} + 1} \right\}.
$$

But since $A _ { \tau ^ { * } + 1 } > 0$ we must conclude 

$$
U _ {\tau^ {*}} = U _ {0} + M _ {\tau^ {*}} = Z _ {\tau^ {*}}.
$$

Theorem. Let $Z$ be an adapted integrable process and let U be its Snell envelope. Then 

$$
U _ {0} = \sup \{\mathbb {E} (Z _ {\tau}): s t o p p i n g t i m e 0 \leq \tau \leq T \}.
$$

Proof. Since U is a supermartingale, 

$$
U _ {0} \geq \mathbb {E} (U _ {\tau})
$$

for any stopping time $\tau$ by the optional sampling theorem. (See example sheet 1.) But since $U _ { t } \geq Z _ { t }$ by construction, 

$$
U _ {0} \geq \mathbb {E} (Z _ {\tau})
$$

for any stopping time $\tau .$ . But letting τ<sup>∗</sup> = min $\{ t \in \{ 0 , \ldots , T \} : A _ { t + 1 } > 0 \}$ where $U =$ $U _ { 0 } + M - A$ is the Doob decomposition of $U$ , we have 

$$
U _ {0} = U _ {0} + \mathbb {E} (M _ {\tau^ {*}}) = \mathbb {E} (Z _ {\tau^ {*}}).
$$

again by the optional sampling theorem and the previous result. 

Remark. By a similar argument, one can show that 

$$
U _ {t} = \operatorname{ess} \sup \{\mathbb {E} (Z _ {\tau} | \mathcal {F} _ {t}): \text {   stopping   time   } t \leq \tau \leq T \}.
$$

for all $0 \leq t \leq T$ . This formula allows us to define the Snell envelope for the infinite horizon case $T = \infty$ and also in the continuous time case. 

Definition. If Z is an integrable adapted process, a stopping time σ such that $\mathbb { E } ( Z _ { \sigma } ) =$ $\mathrm { s u p } _ { 0 \leq \tau \leq T } \mathbb { E } ( Z _ { \tau } )$ is called an optimal stopping time. Obviously the stopping time $\tau ^ { * }$ defined above is an optimal stopping time. Example sheet 2 shows how to find another one. 

***** 

Returning to finance, let $( \xi _ { t } ) _ { 0 \leq t \leq T }$ be the process specifying the payout of an American option, let $\breve { Y }$ the unique martingale deflator with $Y _ { 0 } = 0$ and let $( U _ { t } ) _ { 0 \leq t \leq T }$ be the Snell envelope of $Y \xi$ with Doob decomposition $U = U _ { 0 } + M - A$ 

We now will use the assumption that the market is complete: let H be strategy such that $H _ { T } \cdot P _ { T } = ( U _ { 0 } + M _ { T } ) / Y _ { T }$ . Setting $X _ { t } = H _ { t } \cdot P _ { t }$ note that $X Y$ is a martingale since it is a local martingale from before, and since the market is complete, it is also bounded. By the martingale property, we have 

$$
X _ {t} Y _ {t} = U _ {0} + M _ {t}
$$

for all $0 \leq t \leq T$ . In particular, 

$X _ { t } = ( U _ { 0 } + M _ { t } ) / Y _ { t } \geq U _ { t } / Y _ { t } \geq \xi _ { t }$ for all $0 \leq t \leq T$ 

$X _ { \tau ^ { * } } = ( U _ { 0 } + M _ { \tau ^ { * } } ) / Y _ { \tau ^ { * } } = U _ { \tau ^ { * } } / Y _ { \tau ^ { * } } = \xi _ { \tau ^ { * } }$ , and 

$\begin{array} { r } { X _ { 0 } = U _ { 0 } = \operatorname* { s u p } _ { \tau < T } \mathbb { E } ( Y _ { \tau } \xi _ { \tau } ) , } \end{array}$ 

completing the proof of the theorem. 

## 13. A dual approach to optimal stopping

The final result in discrete time is the following dual approach to optimal stopping: 

Theorem. Let $( Z _ { t } ) _ { 0 \leq t \leq T }$ be a discrete-time, integrable adapted process. Then 

$$
\sup _ {\tau \leq T} \mathbb {E} (Z _ {\tau}) = \inf _ {M} \mathbb {E} [ \max _ {0 \leq t \leq T} (Z _ {t} - M _ {t}) ]
$$

where the supremum on the left-hand side is taken over stopping times $\tau$ and the infimum on the right-hand side is taken over martingales M with $M _ { 0 } = 0$ 

Proof. Let M be a martingale with $M _ { 0 } = 0$ . By the optional stopping theorem we have 

$$
\begin{array}{c} \sup _ {\tau \leq T} \mathbb {E} (Z _ {\tau}) = \sup _ {\tau \leq T} \mathbb {E} (Z _ {\tau} - M _ {\tau}) \\ \leq \mathbb {E} [ \max _ {0 \leq t \leq T} (Z _ {t} - M _ {t}) ] \end{array}
$$

Since the inequality holds for any martingale M, it also holds when we take the infimum of the right-hand side over $M$ 

For the reverse inequality, let U be the Snell envelope of Z and let $U = U _ { 0 } + M ^ { * } - A$ be its Doob decomposition. Since $U _ { t } \leq Z _ { t }$ for all t we have 

$$
\begin{array}{l} \inf _ {M} \mathbb {E} [ \max _ {0 \leq t \leq T} (Z _ {t} - M _ {t}) ] \leq \mathbb {E} [ \max _ {0 \leq t \leq T} (Z _ {t} - M _ {t} ^ {*}) ] \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qend{array}
$$

$$
U _ {0} = \sup _ {\tau \leq T} \mathbb {E} (Z _ {\tau})
$$

The conclusion follows from the last section where we proved that 

## CHAPTER 2

## Brownian motion and stochastic calculus

Despite the elegance of discrete-time financial theory, there is at least one glaring problem: explicit computations are dificult. For instance, the fundamental theorems are stated in terms of state price densities, but it is very dificult to classify them except in a few simple examples. The continuous-time theory has the convenient feature that explicit formulae are easy to find–indeed, one of our first results will be the general formula for a state price density in a continuous-time market model. 

Before we can describe the continuous-time financial theory, we need to first learn about stochastic integration. Recall that in discrete time, the self-financing condition and budget constraint imply that for the wealth process X corresponding to a pure investment strategy H satisfies 

$$
X _ {t} Y _ {t} = X _ {0} Y _ {0} + \sum_ {s = 1} ^ {t} H _ {s} \cdot (Y _ {s} P _ {s} - Y _ {s - 1} P _ {s - 1})
$$

Recall that when Y is a martingale deflator, the process $M = Y P$ is a martingale and the process XY is a local martingale. 

The continuous time analogue ought to be something like 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} H _ {s} \cdot d M _ {s}
$$

What does the integral on the right mean? 

If we assume that the sample paths $t \mapsto M _ { t }$ are diferentiable, we could interpret the integral as the Lebesgue integral 

$$
\int_ {0} ^ {t} H _ {s} \cdot \frac {d M _ {s}}{d s} d s.
$$

Unfortunately, it turns out that life is not that simple. Now, a theorem of stochastic calculus says that a continuous martingale with everywhere diferentiable sample paths is necessarily constant. So if we insist that our price processes have diferentiable sample paths, we will have a very boring theory. 

This chapter is concerned with an integration theory where we use the martingale property, rather than the diferentiability of the sample paths, as the key ingredient. This theory is nice, and indeed something like the fundamental theorem of calculus holds. This means we can do explicit computations. 

The most basic example of a continuous martingale is Brownian motion: 

## 1. Brownian motion

In this section, we introduce one of the most fundamental continuous-time stochastic processes, Brownian motion. As hinted above, our primary interest in this process is that it will be the building block for all of the continuous-time market models studied in these lectures. 

Definition. A Brownian motion $W = ( W _ { t } ) _ { t \geq 0 }$ is a collection of random variables such that 

$W _ { 0 } ( \omega ) = 0$ for all $\omega \in \Omega$ 

• for all $0 \leq t _ { 0 } < t _ { 1 } < \ldots < t _ { n }$ the increments $W _ { t _ { i + 1 } } - W _ { t _ { i } }$ are independent, and the distribution of $W _ { t } - W _ { s }$ is $N ( 0 , | t - s | )$ , 

• the sample path $t \mapsto W _ { t } ( \omega )$ is continuous for all $\omega \in \Omega$ 

It is not clear that Brownian motion exists. That is, does there exist a probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ on which the uncountable collection of random variables $( W _ { t } ) _ { t \geq 0 }$ can be simultaneously defined in such a way that the above definition holds? The answer, of course, is yes, and the proof of this fact is due to Wiener in 1923. Therefore, the Brownian motion is also often called the Wiener process, especially in the U.S. 

Although the sample paths of Brownian motion are continuous, they are very irregular. Below is a computer simulation of a one-dimensional Brownian motion: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/3392e0474a236b7113044198ca051d2b7c33181feb0b0044cc4d28ae8fc85171.jpg)


It will often be useful to talk about a Brownian motion in the context of a filtered probability space: 

Definition. A Brownian motion in a filtration $( \mathcal { F } _ { t } ) _ { t \geq 0 } W = ( W _ { t } ) _ { t \geq 0 }$ is a Brownian such that $W _ { s }$ is $\mathcal { F } _ { s }$ -measurable and the increment $W _ { t } - W _ { s }$ is independent of $\mathcal { F } _ { s }$ for all $0 \leq s \leq t$ 

Remark. It is a little exercise in measure theory to show that a Brownian motion is automatically a Brownian motion in its natural filtration. 

Here are some useful properties of Brownian motion related to the martingale property: 

Proposition. Let W be a Brownian motion in a filtration F. Let $Q _ { t } = W _ { t } ^ { 2 } - t$ and $Z _ { t } = e ^ { \alpha W _ { t } - \alpha ^ { 2 } t / 2 }$ where $\alpha \in \mathbb { R }$ is constant. Then the process W, Q and Z are all martingales. 

Proof. Since $W _ { t }$ is $N ( 0 , t )$ , we have that $W _ { t } , Q _ { t }$ and $Z _ { t }$ are integrable. Also for $0 \leq s \leq t$ we have by the measurability of $W _ { s }$ and the independence of $W _ { t } - W _ { s }$ that 

$$
\begin{array}{r l} & {\mathbb {E} [ W _ {t} | \mathcal {F} _ {s} ] = \mathbb {E} [ W _ {t} - W _ {s} + W _ {s} | \mathcal {F} _ {s} ]} \\ & {\qquad = \mathbb {E} [ W _ {t} - W _ {s} ] + W _ {s}} \\ & {\qquad = W _ {s}.} \end{array}
$$

Note that 

$$
\mathbb {E} [ (W _ {t} - W _ {s}) W _ {s} | \mathcal {F} _ {s} ] = W _ {s} \mathbb {E} [ (W _ {t} - W _ {s}) | \mathcal {F} _ {s} ] = 0
$$

so 

$$
\begin{array}{r l} & {\mathbb {E} [ W _ {t} ^ {2} - t | \mathcal {F} _ {s} ] = \mathbb {E} [ (W _ {t} - W _ {s} + W _ {s}) ^ {2} | \mathcal {F} _ {s} ] - t} \\ & {\qquad = \mathbb {E} [ (W _ {t} - W _ {s}) ^ {2} ] + W _ {s} ^ {2} - t} \\ & {\qquad = W _ {s} ^ {2} - s} \end{array}
$$

and finally by the same idea... 

$$
\begin{array}{r l} & {\mathbb {E} [ Z _ {t} ] = Z _ {s} \mathbb {E} [ e ^ {\alpha (W _ {t} - W _ {s}) - \alpha^ {2} (t - s) / 2} | \mathcal {F} _ {s} ]} \\ & {\qquad = Z _ {s}.} \end{array}
$$

## 2. Itˆo stochastic integration

We now have suficient motivation to construct a stochastic integral with respect to a continuous local martingale. What follows is the briefest of sketches of the theory. There are now plenty of places to turn for a proper treatment of the subject. For instance, see the lecture notes on my webpage. 

For the record, we will assume henceforth that the filtration satisfies what are called the usual conditions of right-continuity $\begin{array} { r } { \mathcal { F } _ { t } = \bigcap _ { \epsilon > 0 } \mathcal { F } _ { t + \epsilon } } \end{array}$ and that $\mathcal { F } _ { 0 }$ contains all P-null events. These are technical assumptions that ensure the existence of stopping times with the right properties. 

## 2.1. Quadratic variation.

Theorem. Let M be a continuous local martingale. There exists a finite-valued nondecreasing adapted process A such that $A _ { 0 }$ and for all $t \geq 0$ we have 

$$
\sum_ {i = 1} ^ {n} (M _ {s _ {i} ^ {n}} - M _ {s _ {i - 1} ^ {n}}) ^ {2} \to A _ {t}
$$

where the convergence is in probability, and $s _ { i } ^ { n } = i t / n$ 

Definition. Given the continuous local martingale M, the non-decreasing process A is called the quadratic variation of M and is denoted $A = \langle M \rangle$ 

Theorem. The quadratic variation of a Brownian motion W is given by $\langle W \rangle _ { t } = t \ a . s .$ for all $t \geq 0$ 

Proof. By definition, the increments of Brownian motion are Gaussian random variables so that 

$$
\mathbb {E} [ (W _ {t} - W _ {s}) ^ {2} ] = t - s
$$

and 

$$
\operatorname{Var} \left[ \left(W _ {t} - W _ {s}\right) ^ {2} \right] = 2 (t - s) ^ {2}
$$

for every $0 \leq s \leq t$ . Fix t and n and let $s _ { i } = i t / n$ 

$$
\mathbb {E} \left[ \sum_ {i = 1} ^ {n} (W _ {s _ {i}} - W _ {s _ {i - 1}}) ^ {2} \right] = \sum_ {i = 1} ^ {n} (s _ {i} - s _ {i - 1}) = s _ {n} - s _ {0} = t
$$

and, by the independence of the increments of Brownian motion, 

$$
\mathrm{Var} \left[ \sum_ {i = 1} ^ {n} (W _ {s _ {i}} - W _ {s _ {i - 1}}) ^ {2} \right] = 2 \sum_ {i = 1} ^ {n} (s _ {i} - s _ {i - 1}) ^ {2} = 2 t ^ {2} / n.
$$

Chebychev’s inequality implies 

$$
\mathbb {P} \left(\left| \sum_ {i = 1} ^ {n} (W _ {s _ {i}} - W _ {s _ {i - 1}}) ^ {2} - t \right| \geq \epsilon\right) \leq \frac {2 t ^ {2}}{n \epsilon^ {2}} \to 0.
$$

Remark. For comparison, consider a continuously diferentiable function $f : [ 0 , 1 ] \to \mathbb { R }$ Recall that for such functions there exists a constant $C > 0$ such that $| f ( t ) - f ( s ) | \leq C | t - s |$ for all $s , t \in [ 0 , 1 ]$ . Hence we have 

$$
\begin{array}{c} \sum_ {i = 1} ^ {n} [ f (s _ {i}) - f (s _ {i - 1}) ] ^ {2} \leq \sum_ {i = 1} ^ {n} C ^ {2} t ^ {2} / n ^ {2} \\ = C ^ {2} t ^ {2} / n \to 0 \end{array}
$$

Since the quadratic variation of a Brownian motion is positive, we can conclude that the typical Brownian sample path is not a continuously diferentiable function of time. 

Definition. The previsible sigma-field P is the sigma-field on the product space $\mathbb { R } _ { + } \times \Omega$ generated by sets of the form $( s , t ] \times A$ where $0 \leq s < t$ and A is ${ \mathcal { F } } _ { s } .$ -measurable. 

A previsible process α is a map $\alpha : \mathbb { R } _ { + } \times \Omega \to \mathbb { R }$ that is P-measurable. Equivalently, a previsible process α is the $( t , \omega )$ pointwise limit of a sequence of simple processes $( \alpha ^ { n } ) _ { n }$ of the form 

$$
\alpha_ {t} ^ {n} (\omega) = \sum_ {i = 1} ^ {n} \mathbb {1} _ {(s _ {i - 1}, s _ {i} ]} (t) a _ {i} (\omega)
$$

where $a _ { i }$ is bounded and $\mathcal { F } _ { s _ { i - 1 } } .$ -measurable for some non-random $0 \leq s _ { 0 } < s _ { 1 } < . . . < s _ { n } < \infty$ 

Remark. A continuous adapted process is previsible. 

Theorem. Let M be a continuous local martingale, and let α be a previsible processes such that 

$$
\int_ {0} ^ {t} \alpha_ {s} ^ {2} d \langle M \rangle_ {s} <   \infty a. s. f o r a l l t \geq 0
$$

Then there exists a continuous local martingale X such that 

$$
\sum_ {i = 1} ^ {n} \alpha_ {s _ {i} ^ {n}} ^ {n} (M _ {s _ {i} ^ {n}} - M _ {s _ {i - 1} ^ {n}}) \rightarrow X _ {t}
$$

in a sense which we don’t make precise but involves a sequence of stopping times $\tau _ { n }$ localising M and a sequence of simple previsible processes $\alpha ^ { n }$ converging to α with respect to a certain norm. 

Definition. Given the continuous local martingale M be and the previsible process $\alpha ,$ the continuous local martingale X is called the stochastic integral of α with respect to M and is denoted 

$$
X _ {t} = \int_ {0} ^ {t} \alpha_ {s} d M _ {s}
$$

Remark. The inspired idea of the above definition of the integral is that it compensates for the roughness of a typical sample path of M by using instead the many cancellations that occur on average from the uncorrelated increments. 

Theorem. Let M, $M ^ { 1 }$ and $M ^ { 2 }$ be continuous local martingales and α, $\alpha ^ { 1 }$ and $\alpha ^ { 2 }$ previsible processes. Suppose the integrability conditions hold to ensure the existence of the following stochastic integrals. Then we have 

• R <sup>·</sup><sub>0</sub> α<sub>s</sub>dM<sub>s</sub> = R <sup>t</sup><sub>0</sub> α<sup>2</sup><sub>s</sub>dhMi<sub>s</sub>. 

$\begin{array} { r } { \int _ { 0 } ^ { t } ( c \alpha _ { s } ) d M _ { s } = \int _ { 0 } ^ { t } \alpha _ { s } d ( c M _ { s } ) = c \int _ { 0 } ^ { t } \alpha _ { s } d M _ { s } \ w h e r e \ c \in \mathbb { R } } \end{array}$ is a constant 

$$
\bullet \int_ {0} ^ {t} (\alpha_ {s} ^ {1} + \alpha_ {s} ^ {2}) d M _ {s} = \int_ {0} ^ {t} \alpha_ {s} ^ {1} d M _ {s} + \int_ {0} ^ {t} \alpha_ {s} ^ {2} d M _ {s}
$$

$$
\bullet \int_ {0} ^ {t} \alpha_ {s} d (M _ {s} ^ {1} + M _ {s} ^ {2}) = \int_ {0} ^ {t} \alpha_ {s} d M _ {s} ^ {1} + \int_ {0} ^ {t} \alpha_ {s} d M _ {s} ^ {2}
$$

$$
\bullet \int_ {0} ^ {t} \beta_ {s} d \left(\int_ {0} ^ {s} \alpha_ {u} d M _ {u}\right) = \int_ {0} ^ {t} (\beta_ {s} \alpha_ {s}) d M _ {s}
$$

We end this section with a criterion for knowing when a local martingale is a true martingale: 

Proposition. Let M be a continuous local martingale. $I f \operatorname { \mathbb { E } } ( \langle M \rangle _ { t } ) < \infty$ for all $t \geq 0$ then M is a martingale, and 

$$
\mathbb {E} (M _ {t} ^ {2}) = M _ {0} ^ {2} + \mathbb {E} (\langle M \rangle_ {t}).
$$

In particular if α is previsible and 

$$
\mathbb {E} \left(\int_ {0} ^ {t} \alpha_ {s} ^ {2} d s\right) <   \infty \text {   for   all   } t \geq 0
$$

then the stochastic integral $\begin{array} { r } { M _ { t } = \int _ { 0 } ^ { t } \alpha _ { s } d W _ { s } } \end{array}$ is a martingale (where W is a Brownian motion). 

Remark. Every left-continuous, adapted process is predictable. These are the examples to keep in mind, since they are the ones that come up most in application. 

## 3. Itˆo’s processes and quadratic variation

In the last section, we sketched very quickly the constructed of a stochastic integral with respect to a continuous local martingale. What makes the Itˆo stochastic integral useful is that there is a corresponding stochastic calculus. To describe it, we need a few more definitions. 

As before, let $( W _ { t } ) _ { t \geq 0 }$ be a scalar Brownian motion in a filtration $( \mathcal { F } _ { t } ) _ { t \geq 0 }$ satisfying our usual conditions. 

We can use our stochastic integration theory to define a useful class of stochastic process: 

Definition. An Itˆo process X is an adapted process of the form 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \alpha_ {s} d W _ {s} + \int_ {0} ^ {t} \beta_ {s} d s.
$$

where $X _ { 0 }$ is a fixed real number and $( \alpha _ { t } ) _ { t \geq 0 }$ and $( \beta _ { t } ) _ { t \geq 0 }$ be previsible real-valued processes such that 

$$
\int_ {0} ^ {t} \alpha_ {s} ^ {2} d s <   \infty \mathrm{and} \int_ {0} ^ {t} | \beta_ {s} | d s <   \infty
$$

almost surely for all $t \geq 0$ . For such an Itˆo process, we use the diferential notation 

$$
d X _ {t} = \alpha_ {t} d W _ {t} + \beta_ {t} d t
$$

or even 

$$
d X = \alpha d W + \beta d t
$$

as short hand for the integral notation. (The sample paths of the Brownian motion are nowhere diferentiable, so the notation $d W _ { t }$ is only formal, and can only be interpreted via the stochastic integration theory.) 

Note that the two integrals appearing the above definition have diferent meanings: the first as a stochastic integral and the second as a pathwise Lebesgue integral. 

We now introduce a notion which helps with computations involving Itˆo’s formula. 

Theorem. Let X be an Itˆo process as above. Then 

$$
\sum_ {i = 1} ^ {n} (X _ {s _ {i} ^ {n}} - X _ {s _ {i - 1} ^ {n}}) ^ {2} \rightarrow \int_ {0} ^ {t} \alpha_ {s} ^ {2} d s
$$

for each $t \geq 0$ , where the limit is in probability and $s _ { i } ^ { n } = i t / n$ 

Definition. The quadratic variation of the Itˆo process X with decomposition 

$$
d X _ {t} = \alpha_ {t} d W _ {t} + \beta_ {t} d t
$$

is given by 

$$
\langle X \rangle_ {t} = \int_ {0} ^ {t} \alpha_ {s} ^ {2} d s
$$

or in diferential notation 

$$
d \langle X \rangle_ {t} = \alpha_ {t} ^ {2} d t.
$$

## 4. Itˆo’s formula

We are now ready for the first version of Itˆo’s formula: 

Theorem (Itˆo’s formula, scalar version). Let X be an Itˆo process. $I f : \mathbb { R } $ R twice continuously diferentiable, then $f ( X )$ is an Itˆo process with 

$$
\boxed {d f (X _ {t}) = f ^ {\prime} (X _ {t}) d X _ {t} + \frac {1}{2} f ^ {\prime \prime} (X _ {t}) d \langle X \rangle_ {t}.}
$$

Or equivalently, if X is of the form 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \alpha_ {s} d W _ {s} + \int_ {0} ^ {t} \beta_ {s} d s.
$$

then 

$$
f (X _ {t}) = f (X _ {0}) + \int_ {0} ^ {t} f ^ {\prime} (X _ {s}) \alpha_ {s} d W _ {s} + \int_ {0} ^ {t} \left[ f ^ {\prime} (X _ {s}) \beta_ {s} + \frac {1}{2} f ^ {\prime \prime} (X _ {s}) \alpha_ {s} ^ {2} \right] d s.
$$

Let us highlight a diference between Itˆo and ordinary calculus, by noting the mysterious appearance of the $f ^ { \prime \prime }$ term in Itˆo’s formula. This term would not appear in the chain rule of ordinary calculus. But consider the example $f ( x ) = x ^ { 2 }$ so that 

$$
W _ {t} ^ {2} = 2 \int_ {0} ^ {t} W _ {s} d W _ {s} + t.
$$

Note that since 

$$
\mathbb {E} \left(\int_ {0} ^ {t} W _ {s} ^ {2} d s\right) = \int_ {0} ^ {t} s d s = t ^ {2} / 2 <   \infty ,
$$

the local martingale X given by 

$$
X _ {t} = \int_ {0} ^ {t} W _ {s} d W _ {s}
$$

is actually a true martingale. (Remember that we also verified, directly from the definition of Brownian motion, that the process $Q _ { t } = W _ { t } ^ { 2 } - t$ is a martingale.) 

Example. Consider the Itˆo process given by 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \alpha_ {s} W _ {s} + \int_ {0} ^ {t} \beta_ {s} d s
$$

for some predictable processes $\alpha , \beta$ . Letting 

$$
Y _ {t} = e ^ {X _ {t}},
$$

we would like to show that the process $( Y _ { t } ) _ { t \geq 0 }$ is an Itˆo process, and write down its decomposition in terms of ordinary and stochastic integrals. 

Let $f ( x ) = e ^ { x }$ . Then $f ^ { \prime } ( x ) = e ^ { x }$ and $f ^ { \prime \prime } ( x ) = e ^ { x }$ . Also, 

$$
d X _ {t} = \alpha_ {t} d W _ {t} + \beta_ {t} d t \quad \mathrm{and} \quad d \langle X \rangle_ {t} = \alpha_ {t} ^ {2} d t
$$

So Itˆo’s formula says: 

$$
\begin{array}{l} d f (X _ {t}) = f ^ {\prime} (X _ {t}) d X _ {t} + \frac {1}{2} f ^ {\prime \prime} (X _ {t}) d \langle X \rangle_ {t} \\ \Rightarrow d Y _ {t} = Y _ {t} [ (\beta_ {t} + \alpha_ {t} ^ {2} / 2) d t + \alpha_ {t} d W _ {t} ] \end{array}
$$

Note that 

Y is a local martingale $\Leftrightarrow \beta = - \alpha ^ { 2 } / 2$ 

Idea of proof of Ito’s formula. <sup>ˆ</sup> Fix a partition of $[ 0 , t ]$ . By telescoping a sum and consider the following second order Taylor approximation we have the following: 

$$
\begin{array}{r c l} f (X _ {t}) - f (X _ {0}) & = & \sum_ {i = 1} ^ {n} f (X _ {s _ {i}}) - f (X _ {s _ {i - 1}}) \\ & \approx & \sum_ {n = 1} ^ {N} f ^ {\prime} (X _ {s _ {i - 1}}) (X _ {s _ {i}} - X _ {s _ {i - 1}}) + \frac {1}{2} f ^ {\prime \prime} (X _ {s _ {i - 1}}) (X _ {s _ {i}} - X _ {s _ {i - 1}}) ^ {2} \\ & \approx & \int_ {0} ^ {t} f ^ {\prime} (X _ {s}) d X _ {s} + \int_ {0} ^ {t} \frac {1}{2} f ^ {\prime \prime} (X _ {s}) d \langle X \rangle_ {s}. \end{array}
$$

4.1. The multi-dimensional version. We now introduce the vector version of Itˆo’s formula. It is basically the same as before, but with worse notation. 

An n-dimensional Itˆo process $( X _ { t } ) _ { t \geq 0 }$ defined by 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \alpha_ {s} d W _ {s} + \int_ {0} ^ {t} \beta_ {s} d s,
$$

interpreted component-wise as 

$$
X _ {t} ^ {(i)} = X _ {0} ^ {(i)} + \int_ {0} ^ {t} \sum_ {k = 1} ^ {m} \alpha_ {s} ^ {(i, k)} d W _ {s} ^ {(k)} + \int_ {0} ^ {t} \beta_ {s} ^ {(i)} d s
$$

where $( W _ { t } ) _ { t \geq 0 }$ is an m-dimensional Brownian motion so that $W ^ { ( 1 ) } , \dots , W ^ { ( m ) }$ , are independent scalar Brownian motions, and the previsible process $( \alpha _ { t } ) _ { t \geq 0 }$ is valued in the space of $n \times m$ matrices, and the predictable process $( \beta _ { t } ) _ { t \geq 0 }$ is valued in $\mathbb { R } ^ { n }$ . We insist that 

$$
\int_ {0} ^ {t} \sum_ {i = 1} ^ {n} \sum_ {k = 1} ^ {m} (\alpha_ {s} ^ {(i, k)}) ^ {2} d s <   \infty \mathrm{and} \int_ {0} ^ {t} \sum_ {i = 1} ^ {n} | \beta_ {s} ^ {(i)} | d s <   \infty
$$

almost surely for all $t \geq 0$ so that all of the integrals are defined. The aim of this section is to give a formula for the Itˆo decomposition of $f ( t , X _ { t } )$ 

Now in the scalar case we needed a notion of quadratic variation $( d X _ { t } ) ^ { 2 } = d \langle X \rangle _ { t }$ . In the multi-dimensional case, we now introduce the notion of quadratic co-variation $( d X _ { t } ^ { ( i ) } ) ( d X _ { t } ^ { ( j ) } ) =$ $d \langle X ^ { ( i ) } , X ^ { ( j ) } \rangle _ { t }$ . 

Definition. The quadratic co-variation of $X ^ { ( i ) }$ and $X ^ { ( j ) }$ two Itˆo processes is defined by 

$$
\langle X ^ {(i)}, X ^ {(j)} \rangle_ {t} = \frac {1}{2} \big (\langle X ^ {(i)} + X ^ {(j)} \rangle_ {t} - \langle X ^ {(i)} \rangle_ {t} - \langle X ^ {(j)} \rangle_ {t} \big)
$$

Theorem. Let X be a multi-dimensional Itˆo process as above. Then 

$$
\begin{array}{c} \langle X ^ {(i)}, X ^ {(j)} \rangle_ {t} = \lim _ {n} \sum_ {k = 1} ^ {s} (X _ {s _ {k}} ^ {(i)} - X _ {s _ {k - 1}} ^ {(i)}) (X _ {s _ {k}} ^ {(j)} - X _ {s _ {k - 1}} ^ {(j)}) \\ = \int_ {0} ^ {t} \sum_ {k = 1} ^ {m} \alpha_ {s} ^ {(i, k)} \alpha_ {s} ^ {(j, k)} d s. \end{array}
$$

for each $t \geq 0$ , where $s _ { k } = k t / n$ and where the limit is in probability. 

The following multiplication table might help you remember how to compute quadratic co-variation, where W and $W ^ { \perp }$ denote independent Brownian motions: 

<table><tr><td>$ (dt)^{2} = 0 $</td><td>$ (dt)(dW_{t}) = 0 $</td></tr><tr><td>$ (dW_{t})^{2} = dt $</td><td>$ (dW_{t})(dW_{t}^{\perp}) = 0 $</td></tr></table>

Now we are ready for the statement of the theorem: 

Theorem (Itˆo’s formula, multi-dimensional version). Let $f : \mathbb { R } _ { + } \times \mathbb { R } ^ { n } \to \mathbb { R }$ where $( t , x ) \mapsto f ( t , x )$ be continuously diferentiable in the t variable and twice-continuously diferentiable in the x variable. Then 

$$
\boxed {d f (t, X _ {t}) = \frac {\partial f}{\partial t} (t, X _ {t}) d t + \sum_ {i = 1} ^ {n} \frac {\partial f}{\partial x _ {i}} (t, X _ {t}) d X _ {t} ^ {(i)} + \frac {1}{2} \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} \frac {\partial^ {2} f}{\partial x _ {i} \partial x _ {j}} (t, X _ {t}) d \langle X ^ {(i)}, X ^ {(j)} \rangle_ {t}}
$$

## 5. Girsanov’s theorem

As we have seen in discrete time, the economic notion of an arbitrage-free market model with a num´eraire is tied to the existence of an equivalent measure for which the asset prices, when discounted by a num´eraire, are martingales. 

Recall that an equivalent measures is related to a positive random variable via the Radon– Nikodym theorem. Indeed, let $( \Omega , \mathcal { F } , \mathbb { P } )$ be our probability space and let $\mathbb { Q }$ be equivalent to P. Then, by the Radon–Nikodym theorem there exists a density 

$$
Z = \frac {d \mathbb {Q}}{d \mathbb {P}}
$$

such that $Z > 0$ has unit P-expectation. Conversely, if $Z > 0$ and $\mathbb { E } ^ { \mathbb { P } } ( Z ) = 1$ , we can define an equivalent measure Q with density Z. 

Motivated by above discussion, we aim to understand how martingales arise within the context of the Itˆo stochastic integration theory. Consider the stochastic process $( Z _ { t } ) _ { t \geq 0 }$ given by 

$$
Z _ {t} = e ^ {- \frac {1}{2} \int_ {0} ^ {t} \| \alpha_ {s} \| ^ {2} d s + \int_ {0} ^ {t} \alpha_ {s} \cdot d W _ {s}}
$$

where $( W _ { t } ) _ { t \geq 0 }$ is a m-dimensional Brownian motion and $( \alpha _ { t } ) _ { t \geq 0 }$ is a m-dimensional predictable process with $\begin{array} { r } { \int _ { 0 } ^ { t } \| \alpha _ { s } \| ^ { 2 } d s < \infty \ \mathrm { a . s } } \end{array}$ . for all $t \geq 0$ 

This process is clearly positive. Furthermore, notice that by Itˆo’s formula we have 

$$
d Z _ {t} = Z _ {t} \alpha_ {t} \cdot d W _ {t}
$$

so that $( Z _ { t } ) _ { t \geq 0 }$ is a local martingale, as it is a stochastic integral with respect to a Brownian motion. 

Recall that since $Z$ is a positive local martingale, it is automatically a supermartingale. Hence, if 

$$
\mathbb {E} (Z _ {T}) = 1
$$

for some non-random $T > 0 ;$ , then $( Z _ { t } ) _ { 0 \leq t \leq T }$ is a true martingale. In this case, what happens to the Brownian motion when we change to an equivalent measure with density $Z _ { T } ?$ 

Theorem (Cameron–Martin–Girsanov Theorem). Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space on which a m-dimensional Brownian motion $( W _ { t } ) _ { t \geq 0 }$ is defined, and let $( \mathcal { F } _ { t } ) _ { t \geq 0 }$ be a filtration satisfying the usual conditions. Let 

$$
Z _ {t} = e ^ {- \frac {1}{2} \int_ {0} ^ {t} \| \alpha_ {s} \| ^ {2} d s + \int_ {0} ^ {t} \alpha_ {s} \cdot d W _ {s}}
$$

and suppose $( Z _ { t } ) _ { 0 \leq t \leq T }$ is a martingale. Define the equivalent measure $\mathbb { Q }$ on $( \Omega , { \mathcal { F } } _ { T } )$ by the density process 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = Z _ {T}.
$$

Then the m-dimensional process $( \hat { W } _ { t } ) _ { 0 \leq t \leq T }$ defined by 

$$
\hat {W} _ {t} = W _ {t} - \int_ {0} ^ {t} \alpha_ {s} d s
$$

is a Brownian motion on $( \Omega , \mathcal { F } _ { T } , \mathbb { Q } )$ 

Remark. This isn’t the appropriate place to prove Girsanov’s theorem, but here is a related result that is completely elementary: Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space, and let W be a random vector with the d-dimensional normal $N _ { d } ( 0 , I )$ distribution, where I is the $d \times d$ identity matrix. Fix a constant vector $\boldsymbol { \alpha } \in \mathbb { R } ^ { d }$ and define an equivalent measure $\mathbb { Q }$ on (Ω, F) by the density 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = e ^ {\alpha \cdot W - \| \alpha \| ^ {2} / 2}.
$$

Then the random vector $\hat { W } = W - \alpha$ has the $N _ { d } ( 0 , I )$ distribution under $\mathbb { Q } .$ 

To see why, let $f : \mathbb { R } ^ { d }  \mathbb { R }$ be bounded and measurable. The following computation proves the claim 

$$
\begin{array}{l} \mathbb {E} ^ {\mathbb {Q}} [ f (W) ] = \mathbb {E} ^ {\mathbb {P}} [ e ^ {\alpha \cdot W - \| \alpha \| ^ {2} / 2} f (W - \alpha) ] \\ \qquad = \int e ^ {\alpha \cdot w - \| \alpha \| ^ {2} / 2} f (w - \alpha) \frac {e ^ {- \| w \| ^ {2} / 2}}{(2 \pi) ^ {d / 2}} d w \\ \qquad = \int \frac {e ^ {- \| w - \alpha \| ^ {2} / 2}}{(2 \pi) ^ {d / 2}} f (w - \alpha) d w \\ \qquad = \int f (u) \frac {e ^ {- \| u \| ^ {2} / 2}}{(2 \pi) ^ {d / 2}} d u \\ \qquad = \mathbb {E} ^ {\mathbb {P}} [ f (W) ] \end{array}
$$

where the second to last line follows from the change of variables $u = w - \alpha$ 

Now, you may be asking yourself: When is the process $( Z _ { t } ) _ { t \geq 0 }$ not just a local martingale, but a true martingale? 

Theorem (Novikov’s criterion). If 

$$
\mathbb {E} \left(e ^ {+ \frac {1}{2} \int_ {0} ^ {T} \| \alpha_ {s} \| ^ {2} d s}\right) <   \infty
$$

then 

$$
\mathbb {E} \left(e ^ {- \frac {1}{2} \int_ {0} ^ {T} \| \alpha_ {s} \| ^ {2} d s + \int_ {0} ^ {T} \alpha_ {s} \cdot d W _ {s}}\right) = 1.
$$

## 6. A martingale representation theorem

In this section we will see that all continuous martingales are essentially stochastic integrals with respect to Brownian motion. This will have applications to our continuous-time financial models in the next chapter. 

Theorem (Itˆo’s Martingale Representation Theorem). Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space on which a m-dimensional Brownian motion $W ~ = ~ ( W _ { t } ) _ { t \geq 0 }$ is defined, and let the filtration $( \mathcal { F } _ { t } ) _ { t \geq 0 }$ be the filtration generated by W. 

Let $X = ( X _ { t } ) _ { t \geq 0 }$ be a continuous local martingale. Then there exists a unique predictable m-dimensional process $( \alpha _ { t } ) _ { t > 0 }$ such that $\textstyle \int _ { 0 } ^ { t } \| \alpha _ { s } \| ^ { 2 } d s < \infty$ almost surely for all $t \geq 0$ and 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \alpha_ {s} \cdot d W _ {s}.
$$

Furthermore, if $X _ { t } > 0$ for all $t \geq 0$ then there exists a predictable $\beta$ such that $\int _ { 0 } ^ { t } \| \beta _ { s } \| ^ { 2 } d s <$ ∞ and 

$$
X _ {t} = X _ {0} e ^ {- \frac {1}{2} \int_ {0} ^ {t} \| \beta_ {s} \| ^ {2} d s + \int_ {0} ^ {t} \beta_ {s} \cdot d W _ {s}}
$$

Proof of the second claim. Assuming that 

$$
d X _ {t} = \alpha_ {t} \cdot d W _ {t}
$$

and the positivity of X, apply Itˆo’s formula to get 

$$
d \log X _ {t} = \frac {\alpha_ {t}}{X _ {t}} \cdot d W _ {t} - \frac {\| \alpha_ {t} \| ^ {2}}{2 X _ {t} ^ {2}} d t
$$

so the conclusion follows with $\beta _ { t } = \alpha _ { t } / X _ { t }$ 

Remark. This isn’t the appropriate place to prove the martingale representation theorem, but here is an easy, related result: Let W be a simple, symmetric random walk, so that $\mathbb { P } ( W _ { t } - W _ { t - 1 } = \pm 1 | W _ { 0 } , \dots , W _ { t - 1 } ) = 1 / 2$ for all $t \geq 1$ . Suppose that the filtration is generated by W, then for every martingale M there exists a previsible process $( \theta _ { t } ) _ { t \geq 1 }$ such that 

$$
M _ {t} = M _ {0} + \sum_ {s = 1} ^ {t} \theta_ {s} (W _ {s} - W _ {s - 1}).
$$

To see why, note that since $M _ { t }$ is $\mathcal { F } _ { t } .$ -measurable for each t, there exists a function $f _ { t } : \{ 0 , 1 \} ^ { t } \to$ R such that 

$$
M _ {t} = f _ {t} (\zeta_ {1}, \dots , \zeta_ {t}).
$$

where $\zeta _ { s } = W _ { s } - W _ { s - 1 }$ . We will make use of the identity 

$$
f _ {t} (\zeta_ {1}, \dots , \zeta_ {t}) = \frac {1}{2} (\zeta_ {t} + 1) f _ {t} (\zeta_ {1}, \dots , \zeta_ {t - 1}, 1) + \frac {1}{2} (1 - \zeta_ {t}) f _ {t} (\zeta_ {1}, \dots , \zeta_ {t - 1}, - 1).
$$

Indeed, the martingale property implies 

$$
\begin{array}{l} M _ {t - 1} = \mathbb {E} (M _ {t} | \mathcal {F} _ {t - 1}) \\ \qquad = \frac {1}{2} f _ {t} (\zeta_ {1}, \ldots , \zeta_ {t - 1}, 1) + \frac {1}{2} f _ {t} (\zeta_ {1}, \ldots , \zeta_ {t - 1}, 0). \end{array}
$$

so that 

$$
M _ {t} - M _ {t - 1} = \frac {1}{2} [ f _ {t} (\zeta_ {1}, \dots , \zeta_ {t - 1}, 1) - f _ {t} (\zeta_ {1}, \dots , \zeta_ {t - 1}, - 1) ] \zeta_ {t}.
$$

The desired representation follows from identifying the $\mathscr { F } _ { t - 1 } { \mathrm { - m e a s u r a b l e } }$ random variable $\begin{array} { r } { \theta _ { t } = \frac 1 2 [ f _ { t } ( \zeta _ { 1 } , \dots , \zeta _ { t - 1 } , 1 ) - f _ { t } ( \zeta _ { 1 } , \dots , \zeta _ { t - 1 } , - 1 ) ] } \end{array}$ 

If this example has you thinking about the completeness of the binomial tree model, then you might not be surprised to learn that the martingale representation theorem plays a role in studying completeness in continuous time. 

We conclude this section with a useful result. It is not directly applicable to finance, but simplifies several arguments. 

Theorem (L´evy’s Characterisation of Brownian Motion). Let $( X _ { t } ) _ { t \geq 0 }$ be a continuous m-dimensional local martingale such that 

$$
\langle X ^ {(i)}, X ^ {(j)} \rangle_ {t} = \left\{ \begin{array}{l l} t & \text {   if   } i = j \\ 0 & \text {   if   } i \neq j. \end{array} \right.
$$

Then $( X _ { t } ) _ { t \geq 0 }$ is a standard m-dimensional Brownian motion. 

Proof. Fix a constant vector $\theta \in \mathbb { R } ^ { m }$ and let $\mathrm { i } = \sqrt { - 1 }$ . Consider 

$$
M _ {t} = e ^ {\mathrm{i} \theta \cdot X _ {t} + | \theta | ^ {2} t / 2}.
$$

By Itˆo’s formula, 

$$
\begin{array}{r c l} d M _ {t} & = & M _ {t} \left(\mathrm{i} \theta \cdot d X _ {t} + \frac {| \theta | ^ {2}}{2} d t\right) - \frac {1}{2} M _ {t} \sum_ {i = 1} ^ {m} \sum_ {j = 1} ^ {m} \theta^ {(i)} \theta^ {(j)} d \langle X ^ {(i)}, X ^ {(j)} \rangle_ {t} \\ & = & \mathrm{i} M _ {t} \theta \cdot d X _ {t} \end{array}
$$

and so $( M _ { t } ) _ { t \geq 0 }$ is a continuous local martingale, as it is the stochastic integral with respect to a continuous local martingale. On the other hand, since $| M _ { t } | = e ^ { | \theta | ^ { 2 } t / 2 }$ and hence $\mathbb { E } ( \operatorname* { s u p } _ { s \in [ 0 , t ] } | M _ { s } | ) < \infty$ the process $( M _ { t } ) _ { t \geq 0 }$ is a true martingale. Thus for all $0 \leq s \leq t$ we have 

$$
\mathbb {E} (M _ {t} | \mathcal {F} _ {s}) = M _ {s}
$$

which implies 

$$
\mathbb {E} \left(e ^ {i \theta \cdot \left(X _ {t} - X _ {s}\right)} \mid \mathcal {F} _ {s}\right) = e ^ {- | \theta | ^ {2} (t - s) / 2}.
$$

The above equation implies that the increment $X _ { t } - X _ { s }$ has the ${ N _ { m } } ( 0 , ( t - s ) I )$ distribution and is independent of $\mathcal { F } _ { s }$  

## CHAPTER 3

## Continuous-time models

We now return to the main theme of these lecture, models of financial markets. We now have the tools to discuss the continuous time case, at least when the asset prices are continuous processes. 

## 1. The set-up

As before, our market model consists of a n-dimensional stochastic processes $P =$ $( P _ { t } ^ { 1 } , \dots , P _ { t } ^ { n } ) _ { t \geq 0 }$ representing the asset prices. This process will be defined on a probability space $( \Omega , \mathcal { F } , \mathbb { P } )$ with a filtration $\mathbb { F } = ( \mathcal { F } _ { t } ) _ { t \geq 0 }$ satisfying the usual conditions. Furthermore, we will make the following assumption to make use of the Itˆo calculus developed in the previous chapter. 

Assumption. The stochastic process P is assumed to be is an Itˆo process adapted to F. 

Since continuous-time theory has enough complications, we will make the following simplification: 

Assumption. There exists a num´eraire asset. 

In particular, when we discuss arbitrage theory, there is no need to allow the possibility of intermediate consumption. 

As before, the investor’s controls consist of the n-dimensional process $H = ( H _ { t } ^ { 1 } , \dots , H _ { t } ^ { n } ) _ { t \geq 0 }$ where $H _ { t } ^ { i }$ and corresponds to the number of shares of asset i held at time t. We will assume that H is self-financing in the continuous time sense: 

Definition. A n-dimensional predictable process H such that H is P-integrable<sup>1</sup>is a self-financing (pure-investment) strategy if 

$$
d (H _ {t} \cdot P _ {t}) = H _ {t} \cdot d P _ {t}
$$

WARNING: THIS DEFINITION IS INCOMPLETE in the sense that it does not give rise to interesting arbitrage theory. The reason for the above warning is spelled out below. 

## 2. Admissible strategies

In order to make sense of the stochastic integral defining the wealth, we need to impose a technical integrability condition which holds automatically for continuous processes. 

However, in moving from discrete to continuous time, we have to be careful. We will now see that this condition isn’t strong enough to make our economic analysis interesting. 

Example. Consider a discrete-time market model with two assets $P = ( 1 , S )$ where S is a simple symmetric random walk: 

$$
S _ {t} = \xi_ {1} + \ldots + \xi_ {t}
$$

where the random variables $\xi _ { 1 } , \xi _ { 2 } , . . .$ . are independent and 

$$
\mathbb {P} (\xi_ {t} = 1) = \mathbb {P} (\xi_ {t} = - 1) = 1 / 2.
$$

Obviously this market has no arbitrage as $P$ is a martingale. Nevertheless, let’s explore how to approximate an arbitrage in some sense. Given a predictable process π, let 

$$
\phi_ {t} = \sum_ {s = 1} ^ {t - 1} (\pi_ {s + 1} - \pi_ {s}) S _ {s}
$$

Then the pair $( \phi , \pi )$ defines a self-financing pure investment strategy with associated wealth process 

$$
X _ {t} = \sum_ {s = 1} ^ {t} \pi_ {s} (S _ {s} - S _ {s - 1}).
$$

In particular, $X _ { 0 } = 0$ 

A simple strategy that resembles an arbitrage is constructed as follows: first define the stopping time 

$$
\sigma = \inf \{t \geq 0: S _ {t} > 0 \}.
$$

and consider the strategy with 

$$
\pi_ {t} = \mathbb {1} _ {\{t \leq \sigma \}}
$$

Note that the associated wealth process is $X _ { t } = S _ { t \wedge \sigma }$ . Since $\sigma < \infty \mathrm { a . s }$ ., the conclusion is that if you are willing to wait a while, investing in this strategy will result in an almost sure gain $X _ { \sigma } = 1$ . But the amount of time you have to wait is very long: one can show that $\mathbb { E } ( \sigma ) = + \infty$ 

One can improve upon the above idea by taking larger and larger bets, efectively ‘speeding up the clock’. Indeed, define the stopping time 

$$
\tau = \inf \{t \geq 0: \xi_ {t} = 1 \}
$$

and consider the strategy 

$$
\pi_ {t} = 2 ^ {t - 1} \mathbb {1} _ {\{t \leq \tau \}}.
$$

In this case, the associated wealth process is 

$$
X _ {t} = 1 - 2 ^ {t} \mathbb {1} _ {\{t \leq \tau - 1 \}}.
$$

This is the classical ‘martingale’ or doubling strategy. Note that $\mathbb { E } ( \tau ) = 2$ , so an investor following this strategy does not have to wait very long on average to realise the gain $X _ { \tau } = 1$ But although τ is small on average, it is not bounded, and hence this strategy does not qualify as an arbitrage. 

Example. A technical problem with continuous time models is that events that will happen eventually can be made to happen in bounded time by speeding up the clock. 

Consider the market with prices $P = ( 1 , W )$ where W is a Brownian motion. Given predictable process $( \pi _ { t } ) _ { t \in [ 0 , T ] }$ on non-random horizon $T > 0$ , such that 

$$
\int_ {0} ^ {T} \pi_ {s} ^ {2} d s <   \infty
$$

we can define 

$$
X _ {t} = \int_ {0} ^ {t} \pi_ {s} d W s
$$

and 

$$
\phi_ {t} = X _ {t} - \pi_ {t} W _ {t}
$$

for $0 \leq t \leq T$ . Note that the strategy ${ \cal H } = ( \phi , \pi )$ that $X _ { t } = H _ { t } \cdot P _ { t }$ is the wealth process and satisfies the self-financing condition 

$$
d X _ {t} = \pi_ {t} d W _ {t} = H _ {t} \cdot d P _ {t}
$$

with initial wealth $X _ { 0 } = 0$ 

We will now construct a process π such that $X _ { T } = K \ \mathrm { a . s }$ . where the constant $K > 0$ is arbitrary. 

Let $f : [ 0 , T ]  [ 0 , \infty ]$ be a strictly increasing, diferentiable function such that $f ( 0 ) = 0$ and $f ( T ) = \infty$ . In particular we assume that $f ^ { \prime } ( t ) > 0$ for t and there exists an inverse function $f ^ { - 1 } : [ 0 , \infty ]  [ 0 , T ]$ such that $f \circ f ^ { - 1 } ( u ) = u$ . For instance, to be explicit, we may take $\begin{array} { r } { f ( t ) = \frac { t } { T - t } } \end{array}$ and $\begin{array} { r } { f ^ { - 1 } ( u ) \stackrel { \cdot } { = } \frac { u T } { 1 + u } } \end{array}$ 

Now define $( Z _ { u } ) _ { u \ge 0 }$ by 

$$
Z _ {u} = \int_ {0} ^ {f ^ {- 1} (u)} \left(f ^ {\prime} (s)\right) ^ {1 / 2} d W _ {s}
$$

Note that Z is a local martingale in the filtration $( \mathcal F _ { f ^ { - 1 } ( u ) } ) _ { u \geq 0 }$ and that the quadratic variation is 

$$
\begin{array}{r c l} \langle Z \rangle_ {u} & = & \int_ {0} ^ {f ^ {- 1} (u)} f ^ {\prime} (s) d s \\ & = & f (f ^ {- 1} (u)) - f (0) \\ & = & u \end{array}
$$

so by L´evy’s characterisation $( Z _ { u } ) _ { u \ge 0 }$ is a Brownian motion. Define the stopping time $\tau$ by 

$$
\tau = \inf \{u \geq 0, Z _ {u} = K \}.
$$

Since $( Z _ { u } ) _ { u \ge 0 }$ is a Brownian motion, we have $\tau < \infty$ almost surely since $\mathrm { s u p } _ { u \geq 0 } Z _ { u } = \infty$ almost surely. 

Now let 

$$
\pi_ {t} = \left(f ^ {\prime} (t)\right) ^ {1 / 2} \mathbb {1} _ {\{t \leq f ^ {- 1} (\tau) \}}
$$

and note 

$$
\int_ {0} ^ {T} \pi_ {s} ^ {2} d s = \int_ {0} ^ {f ^ {- 1} (\tau)} f ^ {\prime} (s) d s = \tau <   \infty
$$

the stochastic integral defining X makes sense. The strange fact is that $( X _ { t } ) _ { t \in [ 0 , T ] }$ is a local martingale with $X _ { 0 } = 0$ , but $X _ { T } = Z _ { \tau } = K$ almost surely. 

We see that integrand $( \pi _ { s } ) _ { s \in [ 0 , T ] }$ roughly corresponds to an gambler starting at noon with £0, employing a doubling strategy (with borrowed money) at a quicker and quicker pace, until finally he gains £K almost surely before the clock strikes one o’clock. This situation is rather unrealistic, particularly since the gambler must go arbitrarily far into debt in order to secure the £K winning. Indeed, if such strategies were a good model for investor behaviour, we all could be much richer by just spending some time trading over the internet. 

The above discussion shows that the integrability necessary to define the stochastic integral is not really suficient for our needs. 

At this stage, there are several reasonable options. In this course we will insist that the investor’s portfolio always has non-negative value. 

Definition. A trading strategy H is admissible if 

$$
H _ {t} \cdot P _ {t} \geq 0 \mathrm{forall} t \geq 0 \mathrm{almostsurely}.
$$

Note that the doubling strategy is not admissible, since the investor now has only a finite credit line. However, a suicide strategy, that is, a doubling strategy in which the object is to lose a fixed amount K by time T, is admissible. 

## 3. Arbitrage and local martingale deflators

To see that our restriction to admissible strategies is reasonable, let’s now consider continuous-time arbitrage theory. 

Definition. An admissible strategy H is called an absolute arbitrage if there is a nonrandom time T such that 

$$
H _ {0} \cdot P _ {0} = 0 \leq H _ {T} \cdot P _ {T} \mathrm{a.s.}
$$

and 

$$
\mathbb {P} \left(H _ {T} \cdot P _ {T} > 0\right) > 0.
$$

An admissible strategy H is called an arbitrage relative to a strategy K if there is a nonrandom time T such that 

$$
H _ {0} \cdot P _ {0} = K _ {0} \cdot P _ {0},
$$

and 

$$
H _ {T} \cdot P _ {T} \geq K _ {T} \cdot P _ {T} \mathrm{a.s.}, \mathbb {P} (H _ {T} \cdot P _ {T} > K _ {T} \cdot P _ {T}) > 0.
$$

Remark. Note that if H is an absolute arbitrage and K is admissible, then the strategy $H + K$ is an arbitrage relative to K. On the other hand, if H is an arbitrage relative to K, then $H - K$ is an absolute arbitrage only if $H - K$ is admissible. In particular, an absolute arbitrage is an arbitrage relative the strategy $K = 0$ of holding no assets. 

In discrete time, the notions of absolute arbitrage and relative arbitrage are essentially equivalent since we did not have to worry about admissibility. In continuous time, we will soon find examples of the surprising fact that 

there exist continuous-time markets that have relative arbitrage but no absolute arbitrage. 

Such market models are sometimes considered models of price bubbles. 

The point of all of this is to warn you to be careful when making arbitrage arguments in continuous time, since reasonable people can disagree on what kind of strategies should be called arbitrages. 

As in the discrete-time theory, we now introduce martingale deflators. 

Definition. A (local) martingale deflator is a positive Itˆo process Y such that $Y P =$ $( Y _ { t } P _ { t } ) _ { t \geq 0 }$ is an n-dimensional (local) martingale. 

Our continuous-time version of the first fundamental theorem follows. Unfortunately, to get a clean statement of this result we need to up the technical ante. 

Theorem. Suppose there exists a local martingale deflator for the market model P. If K is a strategy such that the process K · P Y is a true martingale, then there is no arbitrage relative to K. In particular, there is no absolute arbitrage. 

The proof of this fact is based on an important lemma: 

Lemma. Suppose H is a self-financing pure investment strategy and let 

$$
X _ {t} = H _ {t} \cdot P _ {t} = X _ {0} + \int_ {0} ^ {t} H _ {s} \cdot d P _ {s}
$$

Then 

$$
d (X _ {t} Y _ {t}) = H _ {t} \cdot d (Y _ {t} P _ {t}).
$$

for any Itˆo process Y. In particular, if Y is a local martingale deflator and H is admissible then XY is a supermartingale. 

Proof of lemma. . First note 

$$
Y _ {t} d X _ {t} = Y _ {t} (H _ {t} \cdot d P _ {t})
$$

and 

$$
X _ {t} d Y _ {t} = H _ {t} \cdot P _ {t} d Y _ {t}.
$$

Finally, note that 

$$
d \langle X, Y \rangle_ {t} = (H _ {t} \cdot d P _ {t}) (d Y _ {t}) = \sum_ {i = 1} ^ {n} H _ {t} ^ {i} d \langle P ^ {i}, Y \rangle_ {t}.
$$

Putting this together with Itˆo’s formula yields 

$$
\begin{array}{l} d (X _ {t} Y _ {t}) = Y _ {t} d P _ {t} + X _ {t} d Y _ {t} + d \langle X, Y \rangle_ {t} \\ \qquad = \sum_ {i} H _ {t} ^ {i} (Y _ {t} d P _ {t} ^ {i} + P _ {t} ^ {i} d Y _ {t} + \langle Y, P ^ {i} \rangle_ {t}) \\ \qquad = H _ {t} \cdot d (Y _ {t} P _ {t}) \end{array}
$$

as claimed. Now if Y is a local martingale deflator, then $P Y$ is a local martingale. In particular the process XY can be expressed as the stochastic integral with respect to a continuous local martingale, and hence is itself a local martingale. Finally, if H is admissible, then XY is a non-negative local martingale. Non-negative local martingales are supermartingales by Fatou’s lemma.  

Proof that existence of a local martingale deflator implies no arbitrage. Let Y be a local martingale deflator, and let H and K be strategies such that 

$$
H _ {0} \cdot P _ {0} = K _ {0} \cdot P _ {0} \text { and } H _ {T} \cdot P _ {T} \geq K _ {T} \cdot P _ {T}.
$$

Furthermore, suppose that H is admissible and $K \cdot P Y$ is a martingale. We must show that $H _ { T } \cdot P _ { T } = K _ { T } \cdot P _ { T }$ 

By the above lemma and since Y is non-negative, the process $H { \cdot } P Y$ is a super-martingale. Hence 

$$
\begin{array}{l} K _ {0} \cdot P _ {0} Y _ {0} = H _ {0} \cdot P _ {0} Y _ {0} \\ \qquad \qquad \geq \mathbb {E} (H _ {T} \cdot P _ {T} Y _ {T}) \\ \qquad \qquad \geq \mathbb {E} (K _ {T} \cdot P _ {T} Y _ {T}) \\ \qquad = K _ {0} \cdot P _ {0} Y _ {0}. \end{array}
$$

This shows that $H _ { T } \cdot P _ { T } Y _ { T } = K _ { T } \cdot P _ { T } Y _ { T }$ . Since Y is strictly positive, the conclusion now follows.  

Remark. Note that the above theorem doesn’t say that no relative arbitrage implies the existence of a local martingale deflator. A weaker version notion of relative arbitrage, called ‘free-lunch-with-vanishing-risk,’ is needed to have the converse implication. See the recent book of Delbaen and Schachermayer The Mathematics of Arbitrage for an account of the modern theory. 

Remark. Here is an example of a market with a relative arbitrage and no absolute arbitrage. Fix $T > 0$ and let $( \pi _ { t } ) _ { 0 \leq t \leq T }$ be a predictable process such that $\textstyle \int _ { 0 } ^ { T } \pi _ { s } ^ { 2 } d s < \infty$ and let $\begin{array} { r } { S _ { t } = \int _ { 0 } ^ { t } \pi _ { s } d W _ { s } } \end{array}$ where $W$ is a Brownian motion. Suppose $S _ { t } \leq 1$ for all $t \leq T$ and $S _ { T } = 1$ almost surely. (See the previous section on doubling strategies for an explicit construction of such a process π.) 

Now consider the market with prices $P = ( 1 , S )$ . Note that P is a two-dimensional local martingale, hence there exists a martingale deflator – just set $Y _ { t } = 1$ for all t. Therefore, there is no absolute arbitrage. However, consider the strategy $K = ( 1 , - 1 )$ . Note that $K _ { t } \cdot P _ { t } = 1 - S _ { t } \geq 0$ so K is admissible. We will show that there exists an arbitrage relative to K. Indeed, let $H = ( 1 , 0 )$ . Note that $H _ { 0 } \cdot P _ { 0 } = 1 = K _ { 0 } \cdot P _ { 0 } = 1$ but ${ H _ { T } } \cdot { P _ { T } } = 1 > { K _ { T } } \cdot { P _ { T } } = 0$ 

The point of this example is that the asset with price S seems like a good deal - it costs nothing at time 0 but pays a positive amount at time 1. However, holding one share of the asset, corresponding to the strategy $( 0 , 1 ) = H - K$ is not admissible. 

## 4. The structure of local martingale deflators

In this section we will parametrise a fairly general Itˆo market with $n = d + 1$ assets. All assets in this market are num´eraires, and we use the notation $\boldsymbol { P } = \left( \boldsymbol { B } , \boldsymbol { S } \right)$ . We will assume the dynamics of the prices are given by the following equations 

$$
\begin{array}{l} d B _ {t} = B _ {t} r _ {t} d t \\ d S _ {t} ^ {i} = S _ {t} ^ {i} \left(\mu_ {t} ^ {i} d t + \sum_ {j = 1} ^ {m} \sigma_ {t} ^ {i j} d W _ {t} ^ {j}\right) \text { for } i = 1, \ldots , d \end{array}
$$

where the processes $r , \mu ^ { i } , \sigma ^ { i j }$ are predictable and suitably integrable, and the $W ^ { j }$ are independent Brownian motions. 

The first asset can be thought of as a bank account, and the random variable $r _ { t }$ is the spot interest rate at time t. The (random) ordinary diferential equation can be solved: 

$$
B _ {t} = B _ {0} e ^ {\int_ {0} ^ {t} r _ {s} d s}
$$

The d assets can be thought of as risky stocks. The random variable $\mu _ { t } ^ { i }$ is interpreted as the mean instantaneous return of asset $i ,$ while the spot volatility is $\textstyle \big ( \sum _ { j } ( \sigma _ { t } ^ { i j } ) ^ { 2 } \big ) ^ { 1 / 2 }$ . Note that Itˆo’s formula yields 

$$
S _ {t} ^ {i} = S _ {0} ^ {i} e ^ {\int_ {0} ^ {t} [ \mu_ {s} ^ {i} - \frac {1}{2} \sum_ {j} (\sigma_ {s} ^ {i j}) ^ {2} ] d s + \int_ {0} ^ {t} \sum_ {j} \sigma_ {s} ^ {i j} d W _ {s} ^ {j}}.
$$

We will use the notation 

$$
\mu_ {t} = \left( \begin{array}{c} \mu_ {t} ^ {1} \\ \vdots \\ \mu_ {t} ^ {d} \end{array} \right) \text {and} \sigma_ {t} = \left( \begin{array}{c c c} \sigma_ {t} ^ {1 1} & \dots & \sigma_ {t} ^ {1 m} \\ \vdots & \ddots & \vdots \\ \sigma_ {t} ^ {d 1} & \dots & \sigma_ {t} ^ {d m} \end{array} \right)
$$

for the $d \times 1$ vector of means and $d \times m$ matrix of volatilities, respectively. 

With this more explicit parametrisation, we can describe the structure of local martingale deflators: 

Theorem. Let λ be a predictable m-dimensional process such that $\begin{array} { r } { \int _ { 0 } ^ { t } \| \lambda _ { s } \| ^ { 2 } d s < \infty \ \mathrm { ~ } a . s , } \end{array}$ for all $t \geq 0$ and that 

$$
\sigma_ {t} \lambda_ {t} = \mu_ {t} - r _ {t} {\bf 1} f o r a l m o s t a l l (t, \omega)
$$

where $\mathbf { 1 } = ( 1 , \cdots , 1 ) ^ { \top }$ is the $d \times 1$ vector with the constant 1 in each component. 

$$
Y _ {t} = Y _ {0} e ^ {- \int_ {0} ^ {t} (r _ {s} + \| \lambda_ {s} \| ^ {2} / 2) d s - \int_ {0} ^ {t} \lambda_ {s} \cdot d W _ {s}}
$$

for a constant $Y _ { 0 } > 0 \textrm { - } o r$ in equivalent diferential form 

$$
d Y _ {t} = Y _ {t} (- r _ {t} d t - \lambda_ {t} \cdot d W _ {t}).
$$

Then $Y$ is a local martingale deflator. 

Furthermore, if the filtration is generated by the m-dimensional Brownian motion $W$ , all local martingale deflators have this form. 

Remark. The m-dimensional random vector $\lambda _ { t }$ appearing the theorem is a generalisation of the Sharpe ratio. The process $\lambda = ( \lambda _ { t } ) _ { t \geq 0 }$ is often called the market price of risk, for the local martingale deflator, since it measures in some sense the excess return of the stocks per unit of volatility. 

Proof. We need to show that Y B and Y S are local martingales. Note that by Itˆo’s formula 

$$
d (Y _ {t} B _ {t}) = - Y _ {t} B _ {t} \lambda_ {t} \cdot d W _ {t}
$$

so $Y B$ is a local martingale since it is the stochastic integral with respect to a Brownian motion W. 

Also, by Itˆo’s formula 

$$
\begin{array}{r} d (Y _ {t} S _ {t} ^ {i}) = Y _ {t} S _ {t} ^ {i} [ - r _ {t} + \mu_ {t} ^ {i} - (\sigma_ {t} \lambda_ {t}) ^ {i} ] + Y _ {t} S _ {t} ^ {i} (\sigma_ {t} ^ {i.} - \lambda_ {t}) \cdot d W _ {t} \\ = Y _ {t} S _ {t} ^ {i} (\sigma_ {t} ^ {i.} - \lambda_ {t}) \cdot d W _ {t} \end{array}
$$

where we have used the identity $\sigma _ { t } \lambda _ { t } = \mu _ { t } - r _ { t } \mathbf { 1 }$ to cancel the dt term. 

Conversely, if the filtration is generated by the Brownian motion, the martingale representation theorem says that all positive local martingales M are of the form 

$$
M _ {t} = M _ {0} e ^ {- \frac {1}{2} \int_ {0} ^ {t} \| \lambda_ {s} \| ^ {2} d s - \int_ {0} ^ {t} \lambda_ {s} \cdot d W _ {s}}
$$

for some predictable $\lambda ,$ or in diferential form 

$$
d M _ {t} = - M _ {t} \lambda_ {t} \cdot d W _ {t}.
$$

Hence, if $Y B = M$ is a positive local martingale then 

$$
d Y _ {t} = - Y _ {t} (r _ {t} d t + \lambda_ {t} \cdot d W _ {t})
$$

by Itˆo’s formula. Furthermore, if $Y S$ is a local martingale, then Itˆo’s formula shows that in order to cancel the drift we must have the identity $\sigma _ { t } \lambda _ { t } = \mu _ { t } - r _ { t } \mathbf { 1 }$  

## 5. Replication of European claims

As before, given a market model P we can introduce a contingent claim. Recall that a European contingent claim maturing at a time $T > 0$ is modelled as random variable $\xi _ { T }$ that is F<sub>T</sub>-measurable. We shall assume that there exists at least one martingale deflator, so that, in particular, there are no absolute arbitrages. 

First a simple result: 

Proposition. Suppose H is an admissible replication strategy for a European contingent claim with time T payout $\xi _ { T }$ , and let Y be a local martingale deflator. Then 

$$
H _ {t} \cdot P _ {t} \geq \frac {1}{Y _ {t}} \mathbb {E} (\xi_ {T} Y _ {T} | \mathcal {F} _ {t}).
$$

Proof. This is the same as the proof of that the existence of a local martingale deflator implies no arbitrage. 

$$
\begin{array}{c} \mathbb {E} (\xi_ {T} Y _ {T} | \mathcal {F} _ {t}) = \mathbb {E} (H _ {T} \cdot P _ {T} Y _ {T} | \mathcal {F} _ {t}) \\ \leq H _ {t} \cdot P _ {t} Y _ {t} \end{array}
$$

since $H \cdot P Y$ is a supermartingale. 

Now we will impose more structure, by assuming that the market model $\boldsymbol { P } = \left( \boldsymbol { B } , \boldsymbol { S } \right)$ has dynamics 

$$
d B _ {t} = B _ {t} r _ {t} d t
$$

$$
d S _ {t} ^ {i} = S _ {t} ^ {i} \left(\mu_ {t} ^ {i} d t + \sum_ {j = 1} ^ {m} \sigma_ {t} ^ {i j} d W _ {t} ^ {j}\right) \text {   for   } i = 1, \dots , d
$$

as before, or in vector notation, these equations can be written as 

$$
d S _ {t} = \mathrm{diag} (S _ {t}) (\mu_ {t} d t + \sigma_ {t} d W _ {t})
$$

where 

$$
\operatorname{diag} (s _ {1}, \ldots , s _ {d}) = \left( \begin{array}{c c c c} s _ {1} & 0 & \dots & 0 \\ 0 & s _ {2} & \ddots & 0 \\ \vdots & \ddots & \ddots & \vdots \\ 0 & 0 & \dots & s _ {d} \end{array} \right).
$$

We will work in the filtration generated by W, so that all state price densities Y are of the form 

$$
d Y _ {t} = Y _ {t} (- r _ {t} d t - \lambda_ {t} \cdot d W _ {t}).
$$

where 

$$
\sigma_ {t} \lambda_ {t} = \mu_ {t} - r _ {t} {\bf 1}.
$$

The following will serve as a version of the second fundamental theorem of asset pricing in continuous time. 

Theorem. Suppose the filtration is generated by W, and suppose $m = d$ and that the $d \times d$ matrix $\sigma _ { t }$ is invertible for all $( t , \omega )$ , so that in particular, there is a unique (up to scaling) martingale deflator Y of the form 

$$
d Y _ {t} = Y _ {t} (- r _ {t} d t - \lambda_ {t} \cdot d W _ {t}).
$$

where 

$$
\lambda_ {t} = \sigma_ {t} ^ {- 1} (\mu_ {t} - r _ {t} {\bf 1}).
$$

Let $\xi _ { T }$ be non-negative, $\mathcal { F } _ { T }$ -measurable and such that $\xi _ { T } Y _ { T }$ is integrable. Then there exists an admissible strategy H such that 

$$
H _ {t} \cdot P _ {t} = \frac {1}{Y _ {t}} \mathbb {E} (Y _ {T} \xi_ {T} | \mathcal {F} _ {t}).
$$

In particular, the strategy H replicates $\xi _ { T } = H _ { T } { \cdot } P _ { T }$ , and the initial cost $\mathbb { E } ( Y _ { T } \xi _ { T } ) / Y _ { 0 } = H _ { 0 } { \cdot } P _ { 0 }$ is the minimum cost among admissible replication strategies. 

Remark. Clearly, you could also replicate the claim with an admissible strategy by running a suicide strategy on top of the replication strategy H, but the initial cost of this strategy is more. On the other hand, if you didn’t care about admissibility, you could employ a doubling strategy to replicate the claim with strictly smaller initial cost. 

Proof. Let 

$$
M _ {t} = \mathbb {E} (Y _ {T} \xi_ {T} | \mathcal {F} _ {t}).
$$

Then M is a martingale, and since the filtration is generated by the Brownian motion W the martingale representation theorem tells us that there exists a d-dimensional predictable process α such that 

$$
d M _ {t} = \alpha_ {t} \cdot d W _ {t}.
$$

We will show that there exists an admissible self-financing strategy H such that $X _ { 0 } = M _ { 0 } / Y _ { 0 }$ and 

$$
d (X _ {t} Y _ {t}) = \alpha_ {t} \cdot d W _ {t}.
$$

where $X _ { t } ~ = ~ H _ { t } \cdot P _ { t }$ is the wealth process. This will show that $X _ { t } ~ { = } ~ M _ { t } / Y _ { t }$ , and hence $X _ { T } = \xi _ { T }$ as claimed. 

Now, let H be a self-financing strategy. By an Itˆo’s formula calculation, we have 

$$
d (X _ {t} Y _ {t}) = H _ {t} \cdot d (Y _ {t} P _ {t}).
$$

Write ${ \cal H } = ( \phi , \pi )$ , where $\phi$ is the number of shares of the bank account and $\pi ^ { i }$ is the number of shares of stock i. We need the following to hold 

$$
\phi_ {t} B _ {t} + \pi_ {t} \cdot S _ {t} = M _ {t} / Y _ {t}
$$

and 

$$
\phi_ {t} d (Y _ {t} B _ {t}) + \pi_ {t} \cdot d (Y _ {t} S _ {t}) = \alpha_ {t} \cdot d W _ {t}
$$

We can solve for $\phi$ in terms of $\pi { } .$ : 

$$
\phi_ {t} = \frac {1}{B _ {t}} \left(\frac {M _ {t}}{Y _ {t}} - \pi_ {t} \cdot S _ {t}\right).
$$

Finally, we know that 

$$
d (B _ {t} Y _ {t}) = - B _ {t} Y _ {t} \lambda_ {t} \cdot d W _ {t}
$$

and 

$$
d (S _ {t} ^ {i} Y _ {t}) = S _ {t} ^ {i} Y _ {t} (\sigma_ {t} ^ {i.} - \lambda_ {t}) \cdot d W _ {t}
$$

Plugging this in, yields 

$$
\pi_ {t} = \mathrm{diag} (S _ {t}) ^ {- 1} (\sigma_ {t} ^ {\top}) ^ {- 1} \frac {(M _ {t} \lambda_ {t} + \alpha_ {t})}{Y _ {t}}.
$$

To sum up, note that $\phi _ { t } B _ { t } + \pi _ { t } \cdot S _ { t } = M _ { t } / Y _ { t }$ and that 

$$
\phi_ {t} d B _ {t} + \pi_ {t} \cdot d S _ {t} = d \left(\frac {M _ {t}}{Y _ {t}}\right).
$$

This means ${ \cal H } = ( \phi , \pi )$ is a self-financing strategy and 

$$
H _ {t} \cdot P _ {t} = \frac {M _ {t}}{Y _ {t}} \text {   for   all   } 0 \leq t \leq T.
$$

It is admissible since $\xi _ { T } \ge 0$ and hence $M _ { t } \geq 0$ 

Now, given the existence of the replication strategy H, the minimality of the replication cost follows from the proposition at the beginning of this section since Y X is a true martingale (not just a supermartingale).  

If we consider the equation $\sigma _ { t } \lambda _ { t } = \mu _ { t } - r _ { t } \mathbf { 1 }$ where $\sigma _ { t }$ is an $d \times m$ matrix, one expects from the rules of linear algebra for there to be no solution if $m < d ,$ exactly one solution if $m = d .$ , and many solutions if $m > d .$ Of course, this is not a theorem, just a rule of thumb. Financially, the rule of thumb becomes: 

```txt
m < d ‘⇒’ The market has arbitrage.
m = d ‘⇒’ The market has no arbitrage and is complete.
m > d ‘⇒’ The market has no arbitrage and is incomplete. 
```

## 6. Risk-neutral measures

As before, we have $n = 1 + d$ asset withe prices $\boldsymbol { P } = \left( \boldsymbol { B } , \boldsymbol { S } \right)$ where 

$$
\begin{array}{r l} & {d B _ {t} = B _ {t} r _ {t} d t} \\ & {d S _ {t} = \mathrm{diag} (S _ {t}) (\mu_ {t} d t + \sigma_ {t} d W _ {t}).} \end{array}
$$

In this section we assume that there exists a local martingale deflator $Y$ 

Definition. A risk-neutral measure is an equivalent probability measure $\mathbb { Q }$ such that $S / B$ is a Q-local martingale. 

Note that $Y B$ is a local martingale by the definition of a martingale deflator. Assuming that $Y B$ is a true martingale, then we can construct a risk-neutral measure $\mathbb { Q }$ as we have done previously by fixing $T > 0$ and setting 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = \frac {B _ {T} Y _ {T}}{B _ {0} Y _ {0}}.
$$

Conversely, if $\mathbb { Q }$ is a risk-neutral measure, we have can construct a local martingale deflator Y by setting 

$$
Y _ {t} = \frac {1}{B _ {t}} \mathbb {E} \left(\frac {d \mathbb {Q}}{d \mathbb {P}} | \mathcal {F} _ {t}\right).
$$

Note that by this construction $Y B$ is a true martingale. This leads to the following result. It is just an application of our continuous time version of the 1FTAP: 

Proposition. Suppose there exists a risk-neutral measure, then there is no arbitrage relative to the bank account. 

Now let’s explore what the asset prices look like under a risk-neutral measure. 

Proposition. Let $\mathbb { Q }$ be a risk-neutral measure, and suppose that the filtration is generated $b y$ the Brownian motion. Then the asset prices have dynamics 

$$
\begin{array}{r l} & {d B _ {t} = B _ {t} r _ {t} d t} \\ & {d S _ {t} = \mathrm{diag} (S _ {t}) (r _ {t} {\bf 1} d t + \sigma_ {t} d \hat {W} _ {t}).} \end{array}
$$

where $\hat { W }$ is a Brownian motion under $\mathbb { Q }$ 

Proof. By the structure theorem for local martingale deflators we have that any martingale deflator $Y$ satisfies 

$$
\frac {Y _ {t} B _ {t}}{Y _ {0} B _ {0}} = e ^ {- \int_ {0} ^ {t} \| \lambda_ {s} \| ^ {2} d s - \int_ {0} ^ {t} \lambda_ {s} \cdot d W _ {s}}.
$$

where $\sigma _ { t } \lambda _ { t } = \mu _ { t } - r _ { t } \mathbf { 1 }$ 

Now if there exists a risk-neutral measure $\mathbb { Q } .$ then $Y B$ is a true martingale. Hence we may apply Girsanov’s theorem to conclude that the process $\hat { W }$ defined by 

$$
\hat {W} _ {t} = W _ {t} + \int_ {0} ^ {t} \lambda_ {s} d s
$$

is a Brownian motion under $\mathbb { Q } .$ . Note 

$$
\begin{array}{r l} & {d S _ {t} = \mathrm{diag} (S _ {t}) (\mu_ {t} d t + \sigma_ {t} d W _ {t})} \\ & {\qquad = \mathrm{diag} (S _ {t}) [ \mu_ {t} d t + \sigma_ {t} (d \hat {W} _ {t} - \lambda_ {t} d t) ]} \\ & {\qquad = \mathrm{diag} (S _ {t}) (r _ {t} \mathbf {1} d t + \sigma_ {t} d \hat {W} _ {t})} \end{array}
$$

as claimed. 

We finally connect risk-neutral measures to replication costs. This is just restatement of the version of the 2FTAP appearing the previous section: 

Proposition. Assume that there exists a risk-neutral measure $\mathbb { Q }$ , that the filtration is generated by W, and suppose $m = d$ and that the $d \times d$ matrix $\sigma _ { t }$ is invertible for all $( t , \omega )$ 

Let $\xi _ { T }$ be non-negative, $\mathcal { F } _ { T ^ { - } } m e a s u r a b l e$ and such that $\xi _ { T } / B _ { T }$ is $\mathbb { Q } \mathrm { . }$ -integrable. Then there exists an admissible strategy H that replicates the claim $\xi _ { T } = H _ { T } \cdot P _ { T }$ , and the initial cost $\mathbb { E } ^ { \mathbb { Q } } ( e ^ { - \int _ { 0 } ^ { T } r _ { s } d s } \xi _ { T } ) = H _ { 0 } \cdot P _ { 0 }$ is minimum among admissible replication strategies. 

## 7. The Black–Scholes model and formula

We will consider the simplest possible model of the type studied introduced above. Consider the case of a market with two assets. We will assume that all coeficients are constant, so the price dynamics are given by the pair of equations 

$$
\begin{array}{r c l} {d B _ {t}} & = & {B _ {t} r d t} \\ {d S _ {t}} & = & {S _ {t} (\mu d t + \sigma d W _ {t})} \end{array}
$$

for real constants $r , \mu , \sigma$ where $\sigma > 0$ . We will assume that the filtration is generate by the scalar Brownian motion $W$ . This is often called the Black–Scholes model. 

We are interested in finding the replication cost of a European contingent claim with payout $\xi _ { T } = g ( S _ { T } )$ , where g is a given function which we assume to be non-negative and suitably integrable. We know from before that the unique state price density with $Y _ { 0 } = 1$ is given by 

$$
Y _ {t} = e ^ {- (r + \lambda^ {2} / 2) t - \lambda W _ {t}}
$$

where $\lambda = ( \mu - r ) / \sigma$ 

Hence, from our existential result there is a trading strategy H which replicates the payout with time t cost 

$$
X _ {t} = \frac {1}{Y _ {t}} \mathbb {E} [ Y _ {T} g (S _ {T}) | \mathcal {F} _ {t} ].
$$

This is where we see the advantage of working with equivalent martingale measures rather than state price densities. Indeed, define the equivalent martingale measure Q by the density 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = e ^ {- \lambda^ {2} T / 2 - \lambda W _ {T}}
$$

and recall that by the Cameron–Martin–Girsanov theorem the process $\hat { W } _ { t } = W _ { t } + \lambda t$ is a Q-Brownian motion. 

The price of the stock can be written explicitly: 

$$
S _ {t} = S _ {0} e ^ {(\mu - \sigma^ {2} / 2) t + \sigma W _ {t}} = S _ {0} e ^ {(r - \sigma^ {2} / 2) t + \sigma \hat {W} _ {t}}
$$

and hence 

$$
\begin{array}{r l} & H _ {t} \cdot P _ {t} = e ^ {- r (T - t)} \mathbb {E} ^ {\mathbb {Q}} \left[ g \left(S _ {0} e ^ {(r - \sigma^ {2} / 2) T + \sigma \hat {W} _ {T}}\right) | \mathcal {F} _ {t} \right] \\ & \qquad = e ^ {- r (T - t)} \mathbb {E} ^ {\mathbb {Q}} \left[ g \left(S _ {t} e ^ {(r - \sigma^ {2} / 2) (T - t) + \sigma (\hat {W} _ {T} - \hat {W} _ {t})}\right) | \mathcal {F} _ {t} \right] \\ & \qquad = e ^ {- r (T - t)} \int_ {- \infty} ^ {\infty} g \left(S _ {t} e ^ {(r - \sigma^ {2} / 2) (T - t) + \sigma \sqrt {T - t} z}\right) \frac {e ^ {- z ^ {2} / 2}}{\sqrt {2 \pi}} d z. \end{array}
$$

A famous example is the case of the European call option where the payout function is of the form $g ( S ) = ( S - K ) ^ { + }$ . In this case, we have the the Nobel-prize-winning Black–Scholes formula: 

$$
\begin{array}{c} C _ {t} (T, K) = S _ {t} \Phi \left(- \frac {\log (K / S _ {t})}{\sigma \sqrt {T - t}} + (r / \sigma + \sigma / 2) \sqrt {T - t}\right) \\ - K e ^ {- r (T - t)} \Phi \left(- \frac {\log (K / S _ {t})}{\sigma \sqrt {T - t}} + (r / \sigma - \sigma / 2) \sqrt {T - t}\right) \end{array}
$$

where $\begin{array} { r } { \Phi ( x ) = \int _ { - \infty } ^ { x } \frac { 1 } { \sqrt { 2 \pi } } e ^ { - y ^ { 2 } / 2 } d y } \end{array}$ is the standard normal distribution function. (You are asked to derive this formula on Example Sheet 3.) 

We have argued that the martingale representation theorem asserts the existence of replicating strategy H, but unfortunately, it gives us no information about how to compute H. This problem will be tackled in the next section. 

## 8. Markovian markets: pricing and hedging by PDE

We now have a suficient condition that a contingent claim can be replicated. However, at this stage we can only assert the existence of a replicating strategy for a given claim, but we do not yet know how to actually compute it. This problem is the subject of this section. 

The first step is to pose a model for the asset prices $( B _ { t } , S _ { t } ) _ { t \geq 0 }$ . A good model should give a reasonable statistical fit to the actual market data. Furthermore, a useful model is one in which the prices and hedges of contingent claims can be computed reasonably easily. In this section, we will study models in which the asset prices are Markov processes. These models are useful in the above sense, though there seems to be some controversy over how well they fit actual market data. 

Now suppose that the $d + 1$ assets have Itˆo dynamics which can be expressed as 

$$
\begin{array}{r c l} d B _ {t} & = & B _ {t} r (t, S _ {t}) d t \\ d S _ {t} & = & \mathrm{diag} (S _ {t}) (\mu (t, S _ {t}) d t + \sigma (t, S _ {t}) d W _ {t}) \end{array}
$$

where the nonrandom functions $r : [ 0 , \infty ) \times \mathbb { R } ^ { d } \to \mathbb { R } , \mu : [ 0 , \infty ) \times \mathbb { R } ^ { d } \to \mathbb { R } ^ { d }$ and $\sigma$ : $[ 0 , \infty ) \times \mathbb { R } ^ { d } \to \mathbb { R } ^ { d \times m }$ are given. Notice that this is a special case of the set-up of the last section, as now (with an abuse notation) 

$$
r _ {t} (\omega) = r (t, S _ {t} (\omega)), \mu_ {t} (\omega) = \mu (t, S _ {t} (\omega)), \text { and } \sigma_ {t} (\omega) = \sigma (t, S _ {t} (\omega)).
$$

In this special situation, the asset prices $( S _ { t } ) _ { t \geq 0 }$ are a d-dimensional Markov process. 

The next theorem says how to find a replicating strategy for a contingent claim maturing at time T with payout 

$$
\xi_ {T} = g (S _ {T})
$$

for some non-random function $g : \mathbb { R } ^ { d }  [ 0 , \infty )$ 

Theorem. Suppose the function $V : [ 0 , T ] \times \mathbb { R } ^ { d }  [ 0 , \infty )$ satisfies the partial diferential equation 

$$
\frac {\partial V}{\partial t} + \sum_ {i = 1} ^ {d} r S ^ {i} \frac {\partial V}{\partial S ^ {i}} + \frac {1}{2} \sum_ {i = 1} ^ {d} \sum_ {j = 1} ^ {d} a _ {i, j} S ^ {i} S ^ {j} \frac {\partial^ {2} V}{\partial S ^ {i} \partial S ^ {j}} = r V
$$

$$
V (T, S) = g (S)
$$

where $a = \sigma \sigma ^ { \top }$ , and where all functions in the PDE are evaluated at the same point $( t , S ) \in$ $[ 0 , T ) \times \mathbb { R } ^ { d }$ 

Then there exists an-admissible strategy H such that $H _ { t } \cdot P _ { t } = V ( t , S _ { t } )$ . In particular, this strategy replicates the contingent claim with payout $g ( S _ { T } )$ 

Furthermore, if ${ \cal H } = ( \phi , \pi )$ then the strategy can be calculated as 

$$
\pi_ {t} = \operatorname{grad} V (t, S _ {t}) = \left(\frac {\partial V}{\partial S ^ {1}} (t, S _ {t}), \dots , \frac {\partial V}{\partial S ^ {d}} (t, S _ {t})\right).
$$

and 

$$
\phi_ {t} = \frac {V (t , S _ {t}) - \pi_ {t} \cdot S _ {t}}{B _ {t}}.
$$

The above theorem says that if the market model is Markovian, the price (i.e. replication cost) of a claim contingent on the future risky asset prices can be written as a deterministic function V of the current market prices. Furthermore, the pricing function V can be found by solving a certain linear parabolic partial diferential equation<sup>2</sup> with terminal data to match the payout of the claim. Solving this equation may be dificult to do by hand, but it can usually be done by computer if the dimension d is reasonably small. And most importantly for the banker selling such a contingent claim: the replicating portfolio $\pi _ { t }$ can be calculated as the gradient of the pricing function V with respect to the spatial variables, evaluated at time t and current price $S _ { t }$ 

Proof. By Itˆo’s formula we have 

$$
\begin{array}{l} d V (t, S _ {t}) = \frac {\partial V}{\partial t} d t + \sum_ {i} \frac {\partial V}{\partial S ^ {i}} d S _ {t} ^ {i} + \frac {1}{2} \sum_ {i, j} \frac {\partial^ {2} V}{\partial S ^ {i} \partial S ^ {j}} d \langle S ^ {i}, S ^ {j} \rangle_ {t} \\ = \left(\frac {\partial V}{\partial t} + \frac {1}{2} \sum_ {i, j} \frac {\partial^ {2} V}{\partial S ^ {i} \partial S ^ {j}} S ^ {i} S ^ {j} a ^ {i j}\right) d t + \sum_ {i} \frac {\partial V}{\partial S ^ {i}} d S _ {t} ^ {i} \\ = r \left(V - \sum_ {i} S ^ {i} \frac {\partial V}{\partial S ^ {i}}\right) d t + \sum_ {i} \frac {\partial V}{\partial S ^ {i}} d S _ {t} ^ {i} \end{array}
$$

where we have used the assumption that V solves a certain PDE to go from the second to third line above. 

Now letting φ and π be as in the statement of the theorem we have that 

$$
\begin{array}{c} {V (t, S _ {t}) = \phi_ {t} B _ {t} + \pi_ {t} \cdot S _ {t}} \\ {d V (t, S _ {t}) = \phi_ {t} d B _ {t} + \pi_ {t} \cdot d S _ {t}.} \end{array}
$$

Hence ${ \cal H } = ( \phi , \pi )$ is a self-financing strategy with associated wealth process $X _ { t } = V ( t , S _ { t } )$ as claimed. It is admissible since $V \geq 0$ by assumption.  

## 9. Partial diferential equations and conditional expectations

We have seen that there are two distinct ways to find a replication cost of a attainable contingent claim: by computing expectations or by solving a PDE. On the one hand, we have shown that the minimal replication cost is the expected value of the discounted payout under a risk-neutral measure. On the other hand, we have seen that if the payout is of the form $g ( S _ { T } )$ and the prices $( S _ { t } ) _ { 0 \leq t \leq T }$ satisfy a stochastic diferential equation (SDE), then a (not necessarily minimal) replication cost can be found by solving a partial diferential equation, and indeed, the replicating strategy is given by the gradient of the solution of the PDE. 

In this section we consider the connection between stochastic diferential equations and partial diferential equations. 

The main idea for this section is contained in this result: 

Theorem. Let the n-dimensional process Z satisfies the SDE 

$$
d Z _ {t} = b (Z _ {t}) d t + \sigma (Z _ {t}) d W _ {t}
$$

where W is a m-dimensional Brownian motion. Given function f and g, suppose $v : [ 0 , T ] \times$ $\mathbb { R } ^ { n } \to \mathbb { R } \ i s \ C ^ { 2 }$ , bounded and satisfies the PDE 

$$
\frac {\partial v}{\partial t} + \sum_ {i} b ^ {i} \frac {\partial v}{\partial z ^ {i}} + \frac {1}{2} \sum_ {i, j} a ^ {i j} \frac {\partial^ {2} v}{\partial z ^ {i} \partial z ^ {j}} = f V
$$

where 

$$
a ^ {i j} = \sum_ {k} \sigma^ {i k} \sigma^ {j k}
$$

with terminal condition 

$$
v (T, z) = g (z) \text {   for   all   } z \in \mathbb {R} ^ {n}.
$$

Let 

$$
M _ {t} = e ^ {- \int_ {0} ^ {t} f (Z _ {s}) d s} v (t, Z _ {t}) f o r 0 \leq t \leq T.
$$

Then M is a local martingale. If M is a true martingale (for instance, if M is bounded) then 

$$
v (t, z) = \mathbb {E} \left[ e ^ {- \int_ {t} ^ {T} f (X _ {s}) d s} g (Z _ {T}) | Z _ {t} = z \right].
$$

Proof. By Itˆo’s formula and the fact that v satisfies a certain PDE, we have 

$$
d M _ {t} = e ^ {- \int_ {0} ^ {t} f (Z _ {s}) d s} \sum_ {i j} \sigma^ {i j} \frac {\partial v}{\partial z ^ {i}} d W ^ {j}.
$$

Hence M is a local martingale. 

If M is true martingale, we have 

$$
M _ {t} = \mathbb {E} (M _ {T} | \mathcal {F} _ {t})
$$

and hence 

$$
v (t, Z _ {t}) = e ^ {\int_ {0} ^ {t} f (Z _ {s}) d s} \mathbb {E} \left[ e ^ {- \int_ {0} ^ {T} f (Z _ {s}) d s} g (Z _ {T}) | \mathcal {F} _ {t} \right].
$$

By applying slot property to move the exponential inside the expectation on the right-hand side, then computing the conditional expectation of both sides $Z _ { t }$ and applying the tower and finishes the argument. (Technical note: we have implicitly assumed that all random variables appearing in the conditional expectations are integrable.)  

There is a certain converse to this result. 

Theorem. Let the n-dimensional Markov process Z is a solution of the SDE 

$$
d Z _ {t} = b (Z _ {t}) d t + \sigma (Z _ {t}) d W _ {t}
$$

where b and σ are continuous and where W is a m-dimensional Brownian motion. Further, assume 

$$
\mathbb {P} (Z _ {t} \in A | Z _ {0} = z) > 0
$$

for any open set $A \subseteq \mathbb { R } ^ { n }$ and any starting point $z \in \mathbb { R } ^ { n }$ and any time $t > 0$ . Fix a nonrandom time horizon $T > 0$ and functions f and g and let 

$$
v (t, z) = \mathbb {E} \left[ e ^ {- \int_ {t} ^ {T} f (Z _ {s}) d s} g (Z _ {T}) | Z _ {t} = z \right],
$$

assuming suficient integrability that the conditional expectation is well-defined. If the function is v is twice-continuously diferentiable, then v satisfies the PDE 

$$
\frac {\partial v}{\partial t} + \sum_ {i} b ^ {i} \frac {\partial v}{\partial z ^ {i}} + \frac {1}{2} \sum_ {i, j} a ^ {i j} \frac {\partial^ {2} v}{\partial z ^ {i} \partial z ^ {j}} = f V
$$

where 

$$
a ^ {i j} = \sum_ {k} \sigma^ {i k} \sigma^ {j k}
$$

with terminal condition 

$$
v (T, z) = g (z) \text {   for   all   } z \in \mathbb {R} ^ {n}.
$$

Proof. By the Markov property 

$$
\begin{array}{r} v (t, Z _ {t}) = \mathbb {E} \left[ e ^ {- \int_ {t} ^ {T} f (Z _ {s}) d s} g (Z _ {T}) | Z _ {t} \right] \\ = \mathbb {E} \left[ e ^ {- \int_ {t} ^ {T} f (Z _ {s}) d s} g (Z _ {T}) | \mathcal {F} _ {t} \right] \end{array}
$$

where $( \mathcal { F } _ { t } ) _ { t \geq 0 }$ is the filtration generated by Z. Hence, the process M defined by 

$$
\begin{array}{r l} & M _ {t} = e ^ {- \int_ {0} ^ {t} f (Z _ {s}) d s} v (t, Z _ {t}) \\ & \qquad = \mathbb {E} \left[ e ^ {- \int_ {0} ^ {T} f (Z _ {s}) d s} g (X _ {T}) | \mathcal {F} _ {t} \right] \end{array}
$$

is a martingale. By assumption, the function v is twice-continuously diferentiable, so that Itˆo’s formula is applicable: 

$$
\begin{array}{l} {d M _ {t} = e ^ {- \int_ {0} ^ {t} f (X _ {s}) d s} \sum_ {i j} \sigma^ {i j} \frac {\partial v}{\partial z ^ {i}} d W ^ {j}} \\ {\qquad + e ^ {- \int_ {0} ^ {t} f (Z _ {s}) d s} \left(\frac {\partial v}{\partial t} + \sum_ {i} b ^ {i} \frac {\partial v}{\partial z ^ {i}} + \frac {1}{2} \sum_ {i, j} a ^ {i j} \frac {\partial^ {2} v}{\partial z ^ {i} \partial z ^ {j}} - f V\right) d t} \end{array}
$$

Since M is a martingale, the drift must vanish for almost every $( t , \omega )$ . And since v is $C ^ { 2 }$ and $Z$ can hit every open set arbitrarily quickly, we conclude that the drift vanishes identically.  

Remark. The partial diferential equation 

$$
\frac {\partial v}{\partial t} + \sum_ {i} b ^ {i} \frac {\partial v}{\partial z ^ {i}} + \frac {1}{2} \sum_ {i, j} a ^ {i j} \frac {\partial^ {2} v}{\partial z ^ {i} \partial z ^ {j}} = f V
$$

is called the Feynman–Kac PDE , whereas the equation 

$$
v (t, z) = \mathbb {E} \left[ e ^ {- \int_ {t} ^ {T} f (Z _ {s}) d s} g (Z _ {T}) | Z _ {t} = z \right]
$$

is called the Feynman–Kac formula . The above theorems say, roughly, that a function satisfies the Feynmann–Kac PDE if and only if it satisfies the Feynman–Kac formula. 

Example (Black–Scholes continued). Let’s return to the Black–Scholes model 

$$
\begin{array}{l} {d B _ {t} = B _ {t} r d t} \\ {d S _ {t} = S _ {t} (\mu d t + \sigma d W _ {t})} \end{array}
$$

with constant coeficients $r , \sigma , \mu .$ , with $\sigma > 0$ . If we would like to replicate a claim with payout $g ( S _ { T } )$ , the we know that we should solve the so-called Black–Scholes PDE 

$$
\boxed { \begin{array}{l} \frac {\partial V}{\partial t} + r S \frac {\partial V}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} V}{\partial S ^ {2}} = r V \\ V (T, S) = g (S) \end{array} }
$$

But how can we solve this PDE? By the Feynmann–Kac formula! 

$$
\begin{array}{r l} & V (t, S) = \mathbb {E} ^ {\mathbb {Q}} [ e ^ {- r (T - t)} g (S _ {T}) | S _ {t} = S ] \\ & \qquad = e ^ {- r (T - t)} \int_ {- \infty} ^ {\infty} g \left(S e ^ {(r - \sigma^ {2} / 2) (T - t) + \sigma \sqrt {T - t} z}\right) \frac {e ^ {- z ^ {2} / 2}}{\sqrt {2 \pi}} d z \end{array}
$$

where $\mathbb { Q }$ is the unique risk-neutral measure under which the process $\hat { W } _ { t } = W _ { t } + \lambda t$ is a Brownian motion, where $\lambda = ( \mu - r ) / \lambda$ . Note that 

$$
d S _ {t} = S _ {t} r d t + S _ {t} \sigma d \hat {W} _ {t}
$$

so the Feynmann–Kac PDE for the Markov process $S$ (when viewed on the risk-neutral measure) is exactly the Black–Scholes PDE. 

Now, let’s specialise to the case of the call option where $g ( S ) = ( S - K ) ^ { + }$ . From last section we have 

$$
\begin{array}{c} V (t, S) = S \Phi \left(- \frac {\log (K / S)}{\sigma \sqrt {T - t}} + (r / \sigma + \sigma / 2) \sqrt {T - t}\right) \\ - K e ^ {- r (T - t)} \Phi \left(- \frac {\log (K / S)}{\sigma \sqrt {T - t}} + (r / \sigma - \sigma / 2) \sqrt {T - t}\right). \end{array}
$$

The delta, i.e. the replicating portfolio, in this case is (by a miracle of algebra) 

$$
\frac {\partial V}{\partial S} (t, S) = \Phi \left(- \frac {\log (K / S)}{\sigma \sqrt {T - t}} + (r / \sigma + \sigma / 2) \sqrt {T - t}\right).
$$

Note that an agent attempting to replicate a call option using the Black–Scholes theory will always hold a fraction of shares of the underlying stock between 0 and 1. Also note that since the sensitivity of the portfolio to the price of the underlying, is given by the formula 

$$
\frac {\partial^ {2} V}{\partial S ^ {2}} (t, S) = \frac {1}{S \sigma \sqrt {T - t}} \phi \left(- \frac {\log (K / S)}{\sigma \sqrt {T - t}} + (r / \sigma + \sigma / 2) \sqrt {T - t}\right)
$$

where $\begin{array} { r } { \phi ( x ) = \frac { 1 } { \sqrt { 2 \pi } } e ^ { - x ^ { 2 } / 2 } } \end{array}$ . Since the gamma is always positive, the hedger will buy more shares of the underlying if the price goes up. 

## 10. Risk-neutral pricing and PDEs

In this section, we will build an arbitrage-free market model. By the fundamental theorem of asset pricing, a suficient condition for no-arbitrage is the existence of a risk-neutral measure. Rather than modelling everything under a real-world measure $\mathbb { P }$ and then ensuring that there exists a risk-neutral measure $\mathbb { Q } .$ we will simply assume that the measure $\mathbb { Q }$ exists and do all our modelling the on the probability space $( \Omega , \mathcal { F } , \mathbb { Q } )$ 

We specialise to a certain class of models called factor models. We assume there is a N-dimensional economic factor process $Z$ whose dynamics satisfy a stochastic diferential equation 

$$
d Z _ {t} = b (Z _ {t}) d t + \sigma (Z _ {t}) d W _ {t}
$$

where b takes values in $\mathbb { R } ^ { N }$ and $\sigma$ takes values in the $N \times m$ matrices, where $W$ is a Brownian motion in the risk-neutral measure $\mathbb { Q } .$ . (In previous section we had used the notation W for a Brownian motion under the real-world measure $\mathbb { P }$ and $\hat { W }$ for a Brownian motion under the risk-neutral measure Q. However, in this section, we do not model anything under P, hence we simplify things by dropping theˆfrom the notation.) 

We assume that the spot interest rate $r _ { t } ~ = ~ r ( Z _ { t } )$ is a deterministic function of the economic factor. The bank account evolves as 

$$
d B _ {t} = B _ {t} r _ {t} d t
$$

as usual. We build the prices of a second as follows. We consider a function V that iss twice-continuously diferentiablea and satisfies the PDE 

$$
\frac {\partial V}{\partial t} + \sum_ {i} b ^ {i} \frac {\partial V}{\partial z ^ {i}} + \frac {1}{2} \sum_ {i, j} a ^ {i j} \frac {\partial^ {2} V}{\partial z ^ {i} \partial z ^ {j}} = r V
$$

where 

$$
a ^ {i j} = \sum_ {k} \sigma^ {i k} \sigma^ {j k}.
$$

We then set $P _ { t } = V ( t , Z _ { t } )$ . By Itˆo’s formula, the discounted price $P _ { t } / B _ { t }$ is a local martingale, and hence there is no arbitrage relative to the bank account. 

We now give some examples of risk-neutral pricing in the context of interest rate and stochastic volatility. 

In the following interest rate models, we will set $N = 1$ and assume that the economic factor $Z _ { t }$ is the spot interest rate $r _ { t }$ . Our goal will be to price a zero-coupon bond. 

10.1. Vasicek model. In 1977, Vasicek proposed the following model for the short rate: 

$$
d r _ {t} = \lambda (\bar {r} - r _ {t}) d t + \gamma d W _ {t}
$$

for a parameter $\bar { r } > 0$ interpreted as a mean short rate, a mean-reversion parameter $\lambda > 0$ and a volatility parameter $\gamma > 0$ . This stochastic diferential equation can be solved explicitly to yield 

$$
r _ {t} = e ^ {- \lambda t} r _ {0} + (1 - e ^ {- \lambda t}) \bar {r} + \int_ {0} ^ {t} e ^ {- \lambda (t - s)} \gamma d W _ {s}.
$$

Note that the short interest rate in the Vasicek model follows an Ornstein–Uhlenbeck process, and in particular, that for each $t \geq 0$ the random variable $r _ { t }$ is Gaussian under the measure $\mathbb { Q }$ with 

$$
\mathbb {E} ^ {\mathbb {Q}} (r _ {t}) = e ^ {- \lambda t} r _ {0} + (1 - e ^ {- \lambda t}) \bar {r} \mathrm{and} \operatorname{Var} ^ {\mathbb {Q}} (r _ {t}) = \int_ {0} ^ {t} e ^ {- 2 \lambda (t - s)} \sigma^ {2} d s = \frac {\gamma^ {2}}{2 \lambda} (1 - e ^ {- 2 \lambda t}).
$$

Moreover, one can show that the process is ergodic and converges to the invariant distribution $\begin{array} { r } { N \left( \bar { r } , \frac { \gamma ^ { 2 } } { 2 \lambda } \right) } \end{array}$ . In particular, we have 

$$
\frac {1}{T} \int_ {0} ^ {T} r _ {s} d s \rightarrow \bar {r} \mathbb {Q} - \mathrm{almostsurely}.
$$

Please note, however, that in the present framework we can say absolutely nothing about the distribution of $r _ { t }$ for the objective measure $\mathbb { P } _ { \mathrm { : } }$ , unless we have a model for the market price of risk. 

Since the short rate $r _ { t }$ is Gaussian, the advantage of this type of model is that it is relatively easy to compute prices, for instance of bonds, explicitly. A disadvantage of this model is that there is a chance that $r _ { t } < 0$ for some time $t > 0$ . Recall that a normal random variable can take any real value, both positive and negative. However, for sensible parameter values, the Q-probability of the event $\{ r _ { t } < 0 \}$ is pretty small. 

We have learned from example sheet 3 that 

$$
\begin{array}{l} \int_ {0} ^ {T} r _ {t} d t = \int_ {0} ^ {T} [ e ^ {- \lambda t} r _ {0} + (1 - e ^ {- \lambda t}) \bar {r} ] d t + \int_ {0} ^ {T} \int_ {0} ^ {t} e ^ {- \lambda (t - s)} \gamma d W _ {s} d t \\ \qquad = \int_ {0} ^ {T} [ e ^ {- \lambda t} r _ {0} + (1 - e ^ {- \lambda t}) \bar {r} ] d t + \int_ {0} ^ {T} \left[ \int_ {s} ^ {T} e ^ {- \lambda (t - s)} d t \right] \gamma d W _ {s} \\ \qquad \sim N \left(\int_ {0} ^ {T} [ e ^ {- \lambda t} r _ {0} + (1 - e ^ {- \lambda t}) \bar {r} ] d t, \frac {\gamma^ {2}}{\lambda^ {2}} \int_ {0} ^ {T} (1 - e ^ {- \lambda t}) ^ {2} d t\right) \end{array}
$$

under $\mathbb { Q } .$ , so that, using the moment generating function of a Gaussian random variable we have that an initial zero-coupon price can be calculated via risk-neutral expectation: 

$$
\begin{array}{l} P _ {0} ^ {T} = \mathbb {E} ^ {\mathbb {Q}} [ e ^ {- \int_ {0} ^ {T} r _ {t} d t} ] \\ = \exp \left(- \int_ {0} ^ {T} \left[ e ^ {- \lambda t} r _ {0} + (1 - e ^ {- \lambda t}) \bar {r} - \frac {\gamma^ {2}}{2 \lambda^ {2}} (1 - e ^ {- \lambda t}) ^ {2} \right] d t\right). \end{array}
$$

The initial forward rates are given by 

$$
f _ {0} ^ {T} = - \frac {\partial}{\partial T} \log P _ {0} ^ {T} = e ^ {- \lambda t} r _ {0} + (1 - e ^ {- \lambda t}) \bar {r} - \frac {\gamma^ {2}}{2 \lambda^ {2}} (1 - e ^ {- \lambda t}) ^ {2}
$$

By the time-homogeneity of the Vasicek model, we can actually deduce the formula 

$$
\boxed {f _ {t} ^ {t + x} = r _ {t} e ^ {- \lambda x} + \bar {r} (1 - e ^ {- \lambda x}) - \frac {\gamma^ {2}}{2 \lambda^ {2}} (1 - e ^ {- \lambda x}) ^ {2}}
$$

This formula says that for the Vasicek model, the forward rates at time t are an afine function of the short rate at time t. (An afine function is of the form $g ( x ) = a x + b _ { \mathrm { ; } }$ , that is, its graph is a line.) 

We can also compute bond prices by solving a PDE. We save this calculation for the next model: 

10.2. Cox–Ingersoll-Ross model. In 1985, Cox, Ingersoll, and Ross proposed the following model for the short rate: 

$$
d r _ {t} = \lambda (\bar {r} - r _ {t}) + \gamma \sqrt {r _ {t}} d W _ {t}
$$

for a parameter $\bar { r } > 0$ interpreted as a mean short rate, a mean-reversion parameter $\lambda > 0$ and a volatility parameter $\gamma > 0$ . The process $( r _ { t } ) _ { t \geq 0 }$ satisfying the above stochastic diferential equation is often called a square-root difusion or CIR process, though this stochastic process was studied as early as 1951 by Feller. This process was also used by Heston to model the spot volatility process in an equity market. 

Although the CIR stochastic diferential equation cannot be solved explicitly, one can say quite a lot about this process. For instance, one can show that the process is ergodic and its invariant distribution is a gamma distribution with mean ¯r. 

An advantage of this model over the Vasicek model is that the short rate $r _ { t }$ is non-negative for all $t \geq 0$ . Furthermore, explicit formula are still available for the bond prices. 

We can also use the above theorem to compute bond prices. Indeed, fix $T > 0$ and consider the PDE 

$$
\begin{array}{l} \frac {\partial V}{\partial t} (t, r) + \lambda (\bar {r} - r) \frac {\partial V}{\partial r} (t, r) + \frac {1}{2} \gamma^ {2} r \frac {\partial^ {2} V}{\partial r ^ {2}} (t, r) = r V (t, r) \\ V (T, r) = 1. \end{array}
$$

We can make the log-afine ansatz 

$$
V (t, r) = e ^ {r R (T - t) + Q (T - t)}
$$

for some functions R and $Q$ which satisfy the boundary conditions $R ( 0 ) ~ = ~ Q ( 0 ) ~ = ~ 0$ Substituting this into the PDE yields 

$$
(- \dot {R} r - \dot {Q}) + \lambda (\bar {r} - r) R + \frac {\sigma^ {2}}{2} r R ^ {2} = r
$$

Matching coeficients of r yields 

$$
\begin{array}{r c l} \dot {R} & = & - \lambda R + \frac {\sigma^ {2}}{2} R ^ {2} - 1 \\ \dot {Q} & = & \lambda \bar {r} R. \end{array}
$$

The equation for R is a Riccati equation, whose solution is 

$$
\begin{array}{l} {R (\tau) = - \frac {2 (e ^ {\gamma \tau} - 1)}{(\gamma + \lambda) e ^ {\gamma \tau} + (\gamma - \lambda)}} \\ {Q (\tau) = \int_ {0} ^ {\tau} \lambda \bar {r} R (s) d s} \end{array}
$$

where $\gamma = \sqrt { \lambda ^ { 2 } + 2 \sigma ^ { 2 } }$ . The bond prices are too messy to write down, but the forward rates are given by 

$$
\boxed {f _ {t} ^ {t + x} = \frac {4 \gamma^ {2} e ^ {\gamma x}}{[ (\gamma + \lambda) e ^ {\gamma x} + (\gamma - \lambda) ] ^ {2}} r _ {t} + \frac {2 \lambda \bar {r} (e ^ {\gamma x} - 1)}{(\gamma + \lambda) e ^ {\gamma x} + (\gamma - \lambda)}.}
$$

In particular, the forward rates for the CIR model are again given by an afine function of the short rate. 

## 11. Beyond Black–Scholes

Recall that the Black–Scholes model predicts that the initial price (or more properly, the minimum initial cost of replicating) a European call option of maturity $T$ and strike $K$ is given by the formula 

$$
C _ {0} (T, K) = S _ {0} F (\sigma^ {2} T, K e ^ {- r T} / S _ {0})
$$

where $F$ is an explicit function (calculated in example sheet 3). What made the Black– Scholes formula so popular after its publication in 1973 is the fact that the right-hand-side depends only on five quantities: the option’s maturity time $T ,$ the option’s strike $K$ , the interest rate $r$ (assumed constant), the underlying stock’s initial price $S _ { 0 }$ at time $t ,$ and a volatility parameter $\sigma .$ Of these five numbers, only the volatility parameter is neither specified by the option contract nor quoted in the market. 

In reality we do not know $\sigma ;$ however we can observe the call prices. So one approach to find the volatility parameter is to observe the prices of calls from the market, and then try to work out which σ to put into the Black–Scholes formula to get the right price. 

This is called the implied volatility of the option: the unique number $\Sigma ( T , K ) = \sigma$ such that 

$$
C _ {0} ^ {\mathrm{obs}} (T, K) = S _ {0} F (\sigma^ {2} T, K e ^ {- r T} / S _ {0})
$$

If the market was still pricing call options by Black–Scholes formula, then there would exist one parameter σ such that $\Sigma ( T , K ) = \sigma$ for all $T$ and $K$ . However, in real-world markets, is is usually the case that the implied volatility surface $( T , K ) \mapsto \Sigma ( T , K )$ is not flat. 

Indeed, for fixed $T ,$ , the graph of the function $K \mapsto \Sigma ( T , K )$ often resembles a convex parabola<sup>3</sup> at least for strikes $K$ close to the money, i.e. such that $K e ^ { - r T } / S _ { 0 } \approx 1$ . That is why practitioners refer to the function $K \mapsto \Sigma ( T , K )$ as the implied volatility smile or smirk. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/36476aba-f178-4198-96a2-65dc827e6172/38c66fe418363f7daede7882730a25aa83148f0eb7d1bf71616e6a5b879136a8.jpg)



Figure 1. Implied volatility vs. log-moneyness $\log ( K e ^ { - r T } / S _ { 0 } )$ for E-mini S& P Mid-Cap 400 call options for maturity $T = 0 . 7$ years, downloaded from ftp: $/ / \tt f t p$ .cmegroup.com/pub/settle/stleqt on 12 July 2018


One could either conclude Black–Scholes model is the true model of the stock price and that the market is mispricing options, or that the Black–Scholes model does not quite match reality. The second approach is more prudent. Then, why even consider implied volatility? As Rebonato famously put it: 

Implied volatility is the wrong number to put into wrong formula to obtain the correct price. 

However, thanks to the enormous influence of the Black–Scholes theory, the implied volatility is now used as a common language to quote option prices. 

11.1. Heston model. In order to explain the observed implied volatility smile, we will then consider a stochastic volatility model. For this model, we will concentrate on the case where there is $d = 1$ stock. For simplicity, we will set the interest rate r to be a constant. It was introduced by Heston in 1993: 

$$
\begin{array}{r l} & {d B _ {t} = B _ {t} r d t} \\ & {d S _ {t} = S _ {t} (r d t + \sqrt {v _ {t}} d W _ {t} ^ {S})} \\ & {d v _ {t} = \lambda (\bar {v} - v _ {t}) d t + c \sqrt {v _ {t}} d W _ {t} ^ {v}} \end{array}
$$

Here $W ^ { S }$ and $W ^ { v }$ are assumed to be correlated Brownian motions in a fixed risk-neutral measure $\mathbb { Q } .$ with correlation $\rho .$ Correlated Brownian motions can be constructed, for instance, by letting $W ^ { v }$ and $W ^ { \perp }$ be independent Brownian motions and let 

$$
W _ {t} ^ {S} = \rho W _ {t} ^ {v} + \sqrt {1 - \rho^ {2}} W _ {t} ^ {\perp}.
$$

In this model the squared volatility v is a mean-reverting process , i.e. an ergodic Markov process, at least under Q. The interpretation of ¯v is the level of mean reversion, while λ is the speed of mean reversion. Note that the interest rate is constant r so that the risk-neutral measure Q is also a forward measure. 

Note that Heston’s model is special case of the general factor model we considered before, where the factor is $Z _ { t } = ( S _ { t } , v _ { t } )$ has dynamic parameters 

$$
b (S, v) = (r S, \lambda (\bar {v} - v))
$$

and 

$$
\sigma (S, v) = \left( \begin{array}{c c} S \sqrt {v} \rho & S \sqrt {v} \sqrt {1 - \rho^ {2}} \\ c \sqrt {v} & 0 \end{array} \right).
$$

The Heston PDE is then 

$$
\frac {\partial F}{\partial t} + r S \frac {\partial F}{\partial S} + \lambda (\bar {v} - v) \frac {\partial F}{\partial v} + \frac {1}{2} S ^ {2} v \frac {\partial^ {2} F}{\partial S ^ {2}} + S v \gamma \rho \frac {\partial^ {2} F}{\partial S \partial v} + \frac {1}{2} \gamma^ {2} v \frac {\partial^ {2} F}{\partial v ^ {2}} = r F.
$$

Note that $F ( t , S , v ) = S$ is a solution of the above PDE, so that the market with the bank account and stock has no arbitrage. 

We would like to compute call prices $\mathbb { E } [ e ^ { - r T } ( S _ { T } - K ) ^ { + } ]$ so we could try to solve Heston’s PDE with terminal condition 

$$
F (T, S, v) = (S - K) ^ {+}.
$$

While this PDE with boundary conditions can be solved numerically, it seems that no explicit solution is possible, unfortunately. 

However, recall that call prices can be calculated via a Fourier integral as long as the moment generating function of the log stock price is known under the forward measure. It turns out that in Heston’s model, we can compute the moment generating function reasonably explicitly. To do so, we need to solve Heston’s PDE with boundary condition 

$$
F (T, v, S; \theta) = S ^ {\theta}
$$

for $\theta \in \Theta = \{ p + \mathrm { i } q : 0 < p < 1 , q \in \mathbb { R } \} \subseteq \mathbb { C }$ . It turns out that this PDE can be solved explicitly. The trick is to make the ansatz 

$$
F (t, v, S; \theta) = S ^ {\theta} e ^ {R (T - t; \theta) v + Q (T - t; \theta)}.
$$

Note that the boundary condition force $R ( 0 ; \theta ) = Q ( 0 ; \theta ) = 0$ . The PDE becomes 

$$
- \dot {R} v - \dot {Q} + [ \theta r + (\theta^ {2} - \theta) v / 2 ] + [ \lambda \bar {v} + (\theta c \rho - \lambda) v ] R + \frac {1}{2} c ^ {2} v R ^ {2} = r,
$$

where the dot indicates diferentiation with respect to the time variable. Notice that the equation can be written in the form 

$$
\alpha (T - t; \theta) v + \beta (T - t; \theta) = 0.
$$

Now, the above equation should hold for all v so $\alpha ( T - t ; \theta ) = 0 = \beta ( T - t ; \theta )$ , i.e 

$$
\dot {R} = (\theta^ {2} - \theta) / 2 + (\theta c \rho - \lambda) R + \frac {1}{2} c ^ {2} R ^ {2}
$$

$$
\dot {Q} = (\theta - 1) r + \lambda \bar {v} R.
$$

The equation for $R$ is a Riccati equation which can be solved explicitly. In fact, we do not even have to make any tricky substitutions, separation of variables and partial fractions work well enough: 

$$
\begin{array}{r l} & {\dot {R} = \frac {1}{2} c ^ {2} (R - R _ {+}) (R - R _ {-})} \\ & {\Rightarrow \frac {\dot {R}}{(R - R _ {+}) (R - R _ {-})} = \frac {1}{2} c ^ {2}} \\ & {\Rightarrow \frac {1}{R _ {+} - R _ {-}} \left(\frac {1}{R - R _ {+}} - \frac {1}{R - R _ {-}}\right) \dot {R} = \frac {1}{2} c ^ {2}} \\ & {\Rightarrow \log \left(\frac {1 - R (\tau) / R _ {+}}{1 - R (\tau) / R _ {-}}\right) = \gamma \tau} \\ & {\Rightarrow R (\tau ; \theta) = (\theta^ {2} - \theta) \frac {e ^ {\gamma (\theta) \tau} - 1}{(\gamma (\theta) - \theta c \rho + \lambda) e ^ {\gamma (\theta) \tau} + (\gamma (\theta) + \theta c \rho - \lambda)}} \end{array}
$$

where $\gamma ( \theta ) = \sqrt { ( \lambda - \theta c \rho ) ^ { 2 } - ( \theta ^ { 2 } - \theta ) c ^ { 2 } }$ and $R _ { \pm } ( \theta ) = [ ( \lambda - \theta c \rho ) ^ { 2 } \pm \gamma ( \theta ) ] / c ^ { 2 }$ . And the second equation can be solved 

$$
\begin{array}{r l} & Q (\tau ; \theta) = \theta r \tau + \int_ {0} ^ {\tau} \lambda \bar {v} R (s; \theta) d s \\ & \qquad = \left(\theta r + \frac {(\theta^ {2} - \theta) \lambda \bar {v}}{\gamma (\theta) + \theta c \rho - \lambda}\right) \tau - \frac {2 \lambda \bar {v}}{c ^ {2}} \log \left(\frac {(\gamma (\theta) - \theta c \rho + \lambda) e ^ {\gamma (\theta) \tau} + (\gamma (\theta) + \theta c \rho - \lambda)}{2 \gamma (\theta)}\right) \end{array}
$$

It can be shown that for $\theta \in \Theta$ that 

$$
\mathbb {E} ^ {\mathbb {Q}} (e ^ {\theta \log S _ {T}}) = e ^ {r T + \theta \log S _ {0} + R (T; \theta) v _ {0} + Q (T; \theta)}.
$$

What is the point of this calculation? Although the formula for the moment generating function is hard to call beautiful, it is very explicit. In particular, given the set of model parameters $( v _ { 0 } , \lambda , \bar { v } , c )$ , the function can be evaluated very quickly on a computer, and hence the Bromwich integral for call prices can be computed numerically quickly. Hence, it is possible to calibrate the Heston model to market data in a reasonable amount of time. This is one of the main reasons for its popularity. 

11.2. Local volatility models. In the previous section we have considered a stochastic volatility model that can match observed call prices reasonably well. However, in this section we will see that it is possible to find a model that matches all observed call prices exactly: 

We consider a model given by 

$$
\begin{array}{r c l} {d B _ {t}} & = & {B _ {t} r d t} \\ {d S _ {t}} & = & {S _ {t} (r d t + \sigma (t, S _ {t}) d \hat {W} _ {t}).} \end{array}
$$

That is, the idea is replace the constant volatility parameter in Black–Scholes model with a local volatility function $\sigma : [ 0 , \infty ) \times ( 0 , \infty ) \to ( 0 , \infty )$ . We will assume that $\sigma$ is smooth and bounded from below and above. 

The next theorem in the present context is usually attributed to Dupire’s 1994 paper. 

Theorem. Suppose that 

$$
C _ {0} (T, K) = \mathbb {E} ^ {\mathbb {Q}} [ e ^ {- r T} (S _ {T} - K) ^ {+} ]
$$

Then 

$$
\frac {\partial C _ {0}}{\partial T} (T, K) + r K \frac {\partial C _ {0}}{\partial K} (T, K) = \frac {\sigma (T , K) ^ {2}}{2} K ^ {2} \frac {\partial^ {2} C _ {0}}{\partial K ^ {2}} (T, K).
$$

Remark. We have already seen a PDE for the replication cost of options in Markovian models. In that PDE, the solution $V ( t , S _ { t } )$ was the time-t value of a replication strategy for the given claim, and the derivatives were respect to the calendar time t and the current price of the underlying asset $S _ { t }$ . In contrast, Dupire’s PDE is for the initial replication cost of a call option, and the derivatives are with respect to the maturity date T and the strike K. 

Remark. The point of the above theorem is this: Suppose you believe that the stock price is generated by a local volatility model, but you do not know what the local volatility function is. If you can observe today’s call price surface $\{ C _ { 0 } ( T , K ) : T > 0 , K > 0 \}$ then you can solve for the local volatility in Dupire’s PDE to arrive at Dupire’s formula 

$$
\boxed {\sigma (T, K) = \left(\frac {2 [ \frac {\partial C _ {0}}{\partial T} (T , K) + r K \frac {\partial C _ {0}}{\partial K} (T , K) ]}{K ^ {2} \frac {\partial^ {2} C _ {0}}{\partial K ^ {2}} (T , K)}\right) ^ {1 / 2}.}
$$

Furthermore, assuming Dupire’s PDE has a unique solution (it will if $\sigma$ is smooth and bounded as assumed) then we have found a model that can reproduce the observed call prices. 

Sketch of proof of Dupire’s formula. To outline the argument, we proceed formally 

$$
\begin{array}{r c l} (S _ {T} - K) ^ {+} & = & (S _ {0} - K) ^ {+} + \int_ {0} ^ {T} \mathbb {1} _ {\{S _ {t} \geq K \}} d S _ {t} + \frac {1}{2} \int_ {0} ^ {T} \delta_ {K} (S _ {t}) d \langle S \rangle_ {t} \\ & = & (S _ {0} - K) ^ {+} + \int_ {0} ^ {T} \bigg (\mathbb {1} _ {\{S _ {t} \geq K \}} S _ {t} r + \frac {1}{2} \delta_ {K} (S _ {t}) S _ {t} ^ {2} \sigma (t, S _ {t}) ^ {2} \bigg)   d t \\ & & + \int_ {0} ^ {T} \mathbb {1} _ {\{S _ {t} \geq K \}} S _ {t} \sigma (t, S _ {t}) d \hat {W} _ {t} \end{array}
$$

where we have appealed to Itˆo’s formula<sup>4</sup> with $g ( x ) = ( x - K ) ^ { + } , g ^ { \prime } ( x ) = \mathbb { 1 } _ { [ K , \infty ) } ( x )$ , and $g ^ { \prime \prime } ( x ) = \delta _ { K } ( x )$ , the Dirac delta ‘function’. 

Now, by the assumption of smoothness and the bounds on the volatility function, the Q-law of the random variable $S _ { T }$ has a density function $f _ { T }$ . Computing expected values of both sides 

$$
e ^ {r T} C _ {0} (T, K) = (S _ {0} - K) ^ {+} + \int_ {0} ^ {T} \int_ {K} ^ {\infty} f _ {t} (y) y r d y d t + \frac {1}{2} \int_ {0} ^ {T} f _ {t} (K) K ^ {2} \sigma (t, K) ^ {2} d t\tag{1}
$$

and then diferentiating both sides with respect to $T$ yields 

$$
e ^ {r T} \left(\frac {\partial C _ {0}}{\partial T} (T, K) + r C _ {0} (T, K)\right) = \int_ {K} ^ {\infty} f _ {T} (y) y r d y + \frac {1}{2} f _ {T} (K) K ^ {2} \sigma (T, K) ^ {2}.
$$

Now we use the following the Breeden–Litzenberger identities 

$$
\begin{array}{c} {e ^ {r T} C _ {0} (T, K) = \int_ {K} ^ {\infty} f _ {T} (y) y d y - K \int_ {K} ^ {\infty} f _ {T} (y) d y} \\ {e ^ {r T} \frac {\partial C _ {0}}{\partial K} (T, K) = - \int_ {K} ^ {\infty} f _ {T} (y) d y} \\ {e ^ {r T} \frac {\partial^ {2} C _ {0}}{\partial K ^ {2}} (T, K) = f _ {T} (K)} \end{array}
$$

to finish the argument. 

## CHAPTER 4

## Crashcourse on probability theory

These notes are a list of many of the definitions and results of probability theory needed to follow the Advanced Financial Models course. Since they are free from any motivating exposition or examples, and since no proofs are given for any of the theorems, these notes should be used only as a reference. A table of notation is in the appendix. 

## 1. Measures

Definition. Let Ω be a set. A sigma-field on Ω is a non-empty set $\mathcal { F }$ of subsets of Ω such that 

(1) if $A \in { \mathcal { F } }$ then $A ^ { c } \in { \mathcal { F } }$ 2 

(2) if $A _ { 1 } , A _ { 2 } , \dotsc \in { \mathcal { F } }$ then $\textstyle \bigcup _ { i = 1 } ^ { \infty } A _ { i } \in { \mathcal { F } }$ 

The terms sigma-field and sigma-algebra are interchangeable. 

The Borel sigma-field B on R is the smallest sigma-field containing every open interval. More generally, if Ω is a topological space, for instance $\mathbb { R } ^ { n }$ , the Borel sigma-field on Ω is the smallest sigma-field containing every open set. 

Definition. Let Ω be a set and let $\mathcal { F }$ be a sigma-field on Ω. A measure $\mu$ on the measurable space $( \Omega , { \mathcal { F } } )$ is a $\mu : { \mathcal { F } }  [ 0 , \infty ]$ such that 

(1) $\mu ( \varnothing ) = 0$ 

(2) if $A _ { 1 } , A _ { 2 } , \dotsc \in { \mathcal { F } }$ are disjoint then $\textstyle \mu ( \bigcup _ { i = 1 } ^ { \infty } A _ { i } ) = \sum _ { i = 1 } ^ { \infty } \mu ( A _ { i } )$ 

Theorem. There exists a unique measure Leb on (R, B) such that 

$$
\operatorname{Leb} (a, b ] = b - a
$$

for every $b > a$ . This measure is called Lebesgue measure. 

Definition. A probability measure P on $( \Omega , { \mathcal { F } } )$ is a measure such that $\mathbb { P } ( \Omega ) = 1$ 

Let Ω be a set, $\mathcal { F }$ a sigma-field on Ω, and P a probability measure on $( \Omega , { \mathcal { F } } )$ . The triple $( \Omega , \mathcal { F } , \mathbb { P } )$ is called a probability space. 

The set Ω is called the sample space, and an element of Ω is called an outcome. A subset of Ω which is an element of $\mathcal { F }$ is called an event. 

Let $A \in { \mathcal { F } }$ be an event. $\operatorname { I f } \mathbb { P } ( A ) = 1$ then A is called an almost sure event, and if $\mathbb { P } ( A ) = 0$ then A is called a null event. The phrase ‘almost surely’ is often abbreviated a.s. A sigma-field is called trivial if each of its elements is either almost sure or null. 

## 2. Random variables

Definition. Let $( \Omega , \mathcal { F } , \mathbb { P } )$ be a probability space. A random variable is a function $X : \Omega $ R such that the set $\{ \omega \in \Omega : X ( \omega ) \leq t \}$ is an element of $\mathcal { F }$ for all $t \in \mathbb { R }$ 

Let A be a subset of R, and let X be a random variable. We use the notation $\{ X \in A \}$ to denote the set $\{ \omega \in \Omega : X ( \omega ) \in A \}$ . For instance, the event $\{ X \leq t \}$ denotes $\{ \omega \in \Omega$ $X ( \omega ) \leq t \}$ 

The distribution function of X is the function $F _ { X } : \mathbb { R } \to [ 0 , 1 ]$ defined by 

$$
F _ {X} (t) = \mathbb {P} (X \leq t)
$$

for all $t \in \mathbb { R }$ 

We also use the term random variable to refer to measurable functions X from Ω to more general spaces. In particular, we call a function $X : \Omega \to \mathbb { R } ^ { n }$ a random variable or random vector if $X ( \omega ) = ( X _ { 1 } ( \omega ) , \ldots , X _ { n } ( \omega ) )$ and $X _ { i }$ is a random variable for each $i \in \{ 1 , \ldots , n \}$ 

Definition. Let A be an event in Ω. The indicator function of the event A is the random variable $\mathbb { 1 } _ { A } : \Omega \to \{ 0 , 1 \}$ defined by 

$$
\mathbb {1} _ {A} (\omega) = \left\{ \begin{array}{l l} 1 & \text { if } \omega \in A \\ 0 & \text { if } \omega \in A ^ {c} \end{array} \right.
$$

for all $\omega \in \Omega$ 

## 3. Expectations and variances

Definition. Let X be a random variable on $( \Omega , \mathcal { F } , \mathbb { P } )$ . The expected value of X is denoted by $\mathbb { E } ( X )$ and is defined as follows 

• X is simple, i.e. takes only a finite number of values $x _ { 1 } , \ldots , x _ { n }$ 

$$
\mathbb {E} (X) = \sum_ {i = 1} ^ {n} x _ {i} \mathbb {P} (X = x _ {i}).
$$

$X \geq 0$ almost surely. 

$$
\mathbb {E} (X) = \sup \{\mathbb {E} (Y): Y \text {   simple   and   } 0 \leq Y \leq X \text { a.s. } \}
$$

Note that the expected value of a non-negative random variable may take the value ∞. 

• Either $\mathbb { E } ( X ^ { + } )$ or $\mathbb { E } ( X ^ { - } )$ is finite. 

$$
\mathbb {E} (X) = \mathbb {E} (X ^ {+}) - \mathbb {E} (X ^ {-})
$$

• X is vector valued and $\mathbb { E } ( | X | ) < \infty$ 

$$
\mathbb {E} [ (X _ {1}, \dots , X _ {d}) ] = (\mathbb {E} [ X _ {1} ], \dots , \mathbb {E} [ X _ {d} ])
$$

A random variable X is integrable if $\mathbb { E } ( | X | ) < \infty$ and is square-integrable if E $( X ^ { 2 } ) < \infty$ The terms expected value, expectation, and mean are interchangeable. 

The variance of an integrable random variable X, written $\operatorname { V a r } ( X )$ , is 

$$
\operatorname{Var} (X) = \mathbb {E} \{[ X - \mathbb {E} (X) ] ^ {2} \} = \mathbb {E} (X ^ {2}) - \mathbb {E} (X) ^ {2}.
$$

The covariance of square-integrable random variable X and Y , written $\operatorname { C o v } ( X , Y )$ , is 

$$
\operatorname{Cov} (X, Y) = \mathbb {E} \left\{\left[ X - \mathbb {E} (X) \right] \left[ Y - \mathbb {E} (Y) \right] \right\} = \mathbb {E} (X Y) - \mathbb {E} (X) \mathbb {E} (Y).
$$

If neither X or Y is almost surely constant, then their correlation, written $\rho ( X , Y )$ , is 

$$
\rho (X, Y) = \frac {\operatorname{Cov} (X , Y)}{\operatorname{Var} (X) ^ {1 / 2} \operatorname{Var} (Y) ^ {1 / 2}}.
$$

Random variables X and Y are called uncorrelated if Cov $( X , Y ) = 0$ 

Theorem. Let X and Y be integrable random variables. 

• linearity: $\mathbb { E } ( a X + b Y ) = a \mathbb { E } ( X ) + b \mathbb { E } ( Y )$ for constants $a , b .$ 

• positivity: Suppose $X \geq 0$ almost surely. Then $\mathbb { E } ( X ) \geq 0$ with equality if and only if $X = 0$ almost surely. 

Definition. For $p \geq 1$ , the space $L ^ { p }$ is the collection of random variables such that $\mathbb { E } ( | X | ^ { p } ) < \infty$ . The space $L ^ { \infty }$ is the collection of random variables which are bounded almost surely. 

Theorem (Jensen’s inequality). Let X be a random variable and $g : \mathbb { R }  \mathbb { R }$ be a convex function. Then 

$$
\mathbb {E} [ g (X) ] \geq g (\mathbb {E} [ X ])
$$

whenever the expectations exist. ${ \mathit { I f } } { \mathit { g } }$ is strictly convex, the above inequality is strict unless X is constant. 

Theorem (H¨older’s inequality). Let X and Y be random variables and let $p , q > 1$ with $\textstyle { \frac { 1 } { p } } + { \frac { 1 } { q } } = 1$ . If $X \in L ^ { p }$ and $Y \in L ^ { q }$ then 

$$
\mathbb {E} (X Y) \leq \mathbb {E} (| X | ^ {p}) ^ {1 / p} \mathbb {E} (| Y | ^ {q}) ^ {1 / q}
$$

with equality if and only if either $X = 0$ almost surely or X and Y have the same sign and $| Y | = a | X | ^ { p - 1 }$ almost surely for some constant $a \geq 0$ . The case when $p = q = 2$ is called the Cauchy–Schwarz inequality. 

Definition. A random variable X is called discrete if X takes values in a countable set; i.e. there is a countable set S such that $X \in S$ almost surely. If X is discrete, the function $p _ { X } : \mathbb { R } \to [ 0 , 1 ]$ defined by $p _ { X } ( t ) = \mathbb { P } ( X = t )$ is called the mass function of X. 

The random variable X is absolutely continuous (with respect to Lebesgue measure) if and only if there exists a function $f _ { X } : \mathbb { R } \to [ 0 , \infty )$ such that 

$$
\mathbb {P} (X \leq t) = \int_ {- \infty} ^ {t} f _ {X} (x) d x
$$

for all $t \in \mathbb { R }$ , in which case the function $f _ { X }$ is called the density function of $X$ 

If X is a random vector taking values in $\mathbb { R } ^ { n }$ , then the density of X, if it exists, is the function $f _ { X } : \mathbb { R } ^ { n } \to [ 0 , \infty )$ such that 

$$
\mathbb {P} (X \in A) = \int_ {A} f _ {X} (x) d x
$$

for all Borel subsets $A \subseteq \mathbb { R } ^ { n }$ 

Theorem. Let the function $g : \mathbb { R } \to \mathbb { R }$ be such that $g ( X )$ is integrable. 

If X is a discrete random variable with probability mass function $p _ { X }$ taking values in a countable set S then 

$$
\mathbb {E} (g (X)) = \sum_ {t \in S} g (t) p _ {X} (t).
$$

$I f X$ is an absolutely continuous random variable with density function $f _ { X }$ then 

$$
\mathbb {E} (g (X)) = \int_ {- \infty} ^ {\infty} g (x) f _ {X} (x) d x.
$$

More generally, if X is a random vector valued in $\mathbb { R } ^ { n }$ with density $f _ { X }$ and $g : \mathbb { R } ^ { n } $ R then 

$$
\mathbb {E} (g (X)) = \int_ {\mathbb {R} ^ {n}} g (x) f _ {X} (x) d x.
$$

## 4. Special distributions

Definition. Let X be a discrete random variable taking values in $\mathbb { Z } _ { + }$ with mass function p<sub>X</sub>. 

The random variable X is called 

• Bernoulli with parameter p if 

$$
p _ {X} (0) = 1 - p \text { and } p _ {X} (1) = p.
$$

where $0 < p < 1$ . Then $\mathbb { E } ( X ) = p$ and $\operatorname { V a r } ( X ) = p ( 1 - p )$ 

• binomial with parameters n and p, written $X \sim \operatorname { b i n } ( n , p )$ , if 

$$
p _ {X} (k) = \binom {n} {k} p ^ {k} (1 - p) ^ {n - k} \text {   for   all   } k \in \{0, 1, \ldots , n \}
$$

where $n \in \mathbb { N }$ and $0 < p < 1$ . Then $\mathbb { E } ( X ) = n p$ and $\operatorname { V a r } ( X ) = n p ( 1 - p )$ 

• Poisson with parameter λ if 

$$
p _ {X} (k) = \frac {\lambda^ {k}}{k !} e ^ {- \lambda} \text {   for   all   } k = 0, 1, 2, \ldots
$$

where $\lambda > 0$ . Then $\mathbb { E } ( X ) = \lambda$ 

• geometric with parameter p if 

$$
p _ {X} (k) = p (1 - p) ^ {k - 1} \text {   for   all   } k = 1, 2, 3, \ldots
$$

where $0 < p < 1$ . Then $\mathbb { E } ( X ) = 1 / p$ 

Definition. Let X be a continuous random variable with density function $f _ { X }$ The random variable X is called 

• uniform on the interval $( a , b )$ , written $X \sim \operatorname { u n i f } ( a , b )$ , if 

$$
f _ {X} (t) = \frac {1}{b - a} \text { for   all } a <   t <   b
$$

for some $a < b .$ Then $\textstyle \mathbb { E } ( X ) = { \frac { a + b } { 2 } }$ 

• normal or Gaussian with mean $\mu$ and variance $\sigma ^ { 2 }$ , written $X \sim N ( \mu , \sigma ^ { 2 } )$ , if 

$$
f _ {X} (t) = \frac {1}{\sqrt {2 \pi} \sigma} \exp \left(- \frac {(x - \mu) ^ {2}}{2 \sigma^ {2}}\right) \mathrm{forall} t \in \mathbb {R}
$$

for some $\mu \in \mathbb { R }$ and $\sigma ^ { 2 } > 0$ . Then $\mathbb { E } ( X ) = \mu$ and $\operatorname { V a r } ( X ) = \sigma ^ { 2 }$ 

• exponential with rate λ, if 

$$
f _ {X} (t) = \lambda e ^ {- \lambda t} \mathrm{forall} t \geq 0
$$

for some $\lambda > 0$ . Then $\mathbb { E } ( X ) = 1 / \lambda$ 

If X is a random vector valued in $\mathbb { R } ^ { n }$ with density 

$$
f _ {X} (x) = (2 \pi) ^ {- n / 2} \det (V) ^ {- 1 / 2} \exp \left(- \frac {1}{2} (x - \mu) \cdot V ^ {- 1} (x - \mu)\right)
$$

for a positive definite $n \times n$ matrix V and vector $\mu \in \mathbb { R } ^ { n }$ , then X is said to have the ndimensional normal (or Gaussian) distribution with mean $\mu$ and variance V, written $X \sim$ $N _ { n } ( \mu , V )$ . Then $\mathbb { E } ( X _ { i } ) = \mu _ { i }$ and $\operatorname { C o v } ( X _ { i } , X _ { j } ) = V _ { i j }$ 

## 5. Conditional probability and expectation, independence

Definition. Let B be an event with $\mathbb { P } ( B ) > 0$ . The conditional probability of an event A given B, written $\mathbb { P } ( A | B )$ , is 

$$
\mathbb {P} (A | B) = \frac {\mathbb {P} (A \cap B)}{\mathbb {P} (B)}.
$$

The conditional expectation of X given B, written $\mathbb { E } ( X | B )$ , is 

$$
\mathbb {E} (X | B) = \frac {\mathbb {E} (X \mathbb {1} _ {B})}{\mathbb {P} (B)}.
$$

Theorem (The law of total probability). Let $B _ { 1 } , B _ { 2 } , \ldots$ . be disjoint, non-null events such that $\textstyle \bigcup _ { i = 1 } ^ { \infty } B _ { i } = \Omega$ . Then 

$$
\mathbb {P} (A) = \sum_ {i = 1} ^ {\infty} \mathbb {P} (A | B _ {i}) \mathbb {P} (B _ {i})
$$

for all events A. 

Definition. Let $A _ { 1 } , A _ { 2 } , . . .$ . be events. If 

$$
\mathbb {P} (\bigcap_ {i \in I} A _ {i}) = \prod_ {i \in I} \mathbb {P} (A _ {i})
$$

for every finite subset $I \subset \mathbb { N }$ then the events are said to be independent. 

Random variables $X _ { 1 } , X _ { 2 } , \ldots$ . are called independent if the events $\{ X _ { 1 } \ \leq \ t _ { 1 } \} , \{ X _ { 2 } \ \leq$ $t _ { 2 } \} , \ldots$ . are independent. The phrase ‘independent and identically distributed’ is often abbreviated i.i.d. 

Theorem. If X and Y are independent and integrable, then 

$$
\mathbb {E} (X Y) = \mathbb {E} (X) \mathbb {E} (Y).
$$

## 6. Probability inequalities

Theorem (Markov’s inequality). Let X be a positive random variable. Then 

$$
\mathbb {P} (X \geq \epsilon) \leq \frac {\mathbb {E} (X)}{\epsilon}
$$

for all $\epsilon > 0$ 

Corollary (Chebychev’s inequality). Let X be a random variable with $\mathbb { E } ( X ) = \mu$ and $\operatorname { V a r } ( X ) = \sigma ^ { 2 }$ . Then 

$$
\mathbb {P} (| X - \mu | \geq \epsilon) \leq \frac {\sigma^ {2}}{\epsilon^ {2}}
$$

for all $\epsilon > 0$ 

## 7. Characteristic functions

Definition. The characteristic function of a real-valued random variable X is the function $\phi _ { X } : \mathbb { R } \overset { } {  } \mathbb { C }$ defined by 

$$
\phi_ {X} (t) = \mathbb {E} (e ^ {i t X})
$$

for all $t \in \mathbb { R }$ , where $i = \sqrt { - 1 }$ . More generally, if X is a random vector valued in $\mathbb { R } ^ { n }$ then $\phi _ { X } : \mathbb { R } ^ { n } \to \mathbb { C }$ defined by 

$$
\phi_ {X} (t) = \mathbb {E} (e ^ {i t \cdot X})
$$

is the characteristic function of X. 

Theorem (Uniqueness of characteristic functions). Let X and Y be real-valued random variables with distribution functions $F _ { X }$ and $F _ { Y }$ . Let $\phi _ { X }$ and $\phi _ { Y }$ be the characteristic functions of X and Y. Then 

$$
\phi_ {X} (t) = \phi_ {Y} (t) f o r a l l t \in \mathbb {R}
$$

if and only if 

$$
F _ {X} (t) = F _ {Y} (t) \text {   for   all   } t \in \mathbb {R}.
$$

## 8. Fundamental probability results

Definition (Modes of convergence). Let $X _ { 1 } , X _ { 2 } , . . .$ . and X be random variables. 

$X _ { n } \to X$ almost surely if $\mathbb { P } ( X _ { n } \to X ) = 1$ 

$X _ { n } \to X$ in L<sup>p</sup>, for $p \geq 1$ , if $\mathbb { E } | X | ^ { p } < \infty$ and $\mathbb { E } | X _ { n } - X | ^ { p }  0$ 

$X _ { n } \to X$ in probability if $\mathbb { P } ( | X _ { n } - X | > \epsilon )  0$ for all $\epsilon > 0$ 

• $X _ { n } \to X$ in distribution if $F _ { X _ { n } } ( t ) \to F _ { X } ( t )$ for all points $t \in \mathbb { R }$ of continuity of $F _ { X }$ 

Theorem. The following implications hold: 

$X _ { n } \to X$ almost surely or ⇒ X<sub>n</sub> → X in probability $\Rightarrow X _ { n } \to X$ in distribution $X _ { n } \to X$ in L<sup>p</sup>, p ≥ 1 

Furthermore, $i f r \geq p \geq 1$ then $X _ { n } \to X$ in $L _ { r } \Rightarrow X _ { n } \to X$ in L<sup>p</sup>. 

Definition. Let $A _ { 1 } , A _ { 2 } , . . .$ . be events. The term eventually is defined by 

$$
\left\{A _ {n} \text {   eventually } \right\} = \bigcup_ {N \in \mathbb {N}} \bigcap_ {n \geq N} A _ {n}
$$

and infinitely often by 

$$
\{A _ {n} \text {   infinitely   often } \} = \bigcap_ {N \in \mathbb {N}} \bigcup_ {n \geq N} A _ {n}.
$$

[The phrase ‘infinitely often’ is often abbreviated $i . o . ]$ 

Theorem (The first Borel–Cantelli lemma). Let $A _ { 1 } , A _ { 2 } , . . .$ . be a sequence of events. If 

$$
\sum_ {n = 1} ^ {\infty} \mathbb {P} (A _ {n}) <   \infty
$$

then $\mathbb { P } ( A _ { n }$ infinitely $o f t e n ) = 0$ 

Theorem (The second Borel-Cantelli lemma). Let $A _ { 1 } , A _ { 2 } , . . .$ . be a sequence of independent events. If 

$$
\sum_ {n = 1} ^ {\infty} \mathbb {P} (A _ {n}) = \infty
$$

then $\mathbb { P } ( A _ { n }$ infinitely $o f t e n ) = 1$ 

Theorem (Monotone convergence theorem). Let $X _ { 1 } , X _ { 2 } , . . .$ . be positive random variables with $X _ { n } \leq X _ { n + 1 }$ almost surely for all $n \geq 1$ , and let $X = \operatorname* { s u p } _ { n \in \mathbb { N } } X _ { n }$ . Then $X _ { n } \to X$ almost surely and 

$$
\mathbb {E} (X _ {n}) \to \mathbb {E} (X).
$$

Theorem (Fatou’s lemma). Let $X _ { 1 } , X _ { 2 } , . . .$ . be positive random variables. Then 

$$
\mathbb {E} (\operatorname * {l i m i n f} _ {n \uparrow \infty} X _ {n}) \leq \operatorname * {l i m i n f} _ {n \uparrow \infty} \mathbb {E} (X _ {n}).
$$

Theorem (Dominated convergence theorem). Let $X _ { 1 } , X _ { 2 } , . . .$ . and X be random variables such that $X _ { n } \to X$ almost surely. $I f \mathbb { E } ( \operatorname* { s u p } _ { n > 1 } | X _ { n } | ) < \infty$ then 

$$
\mathbb {E} (X _ {n}) \to \mathbb {E} (X).
$$

Theorem (A strong law of large numbers). Let $X _ { 1 } , X _ { 2 } , . . .$ . be independent and identically distributed integrable random variables with common mean $\mathbb { E } ( X _ { i } ) = \mu$ . Then 

$$
\frac {X _ {1} + \ldots + X _ {n}}{n} \rightarrow \mu \text {   almost   surely.   }
$$

Theorem (Central limit theorem). Let $X _ { 1 } , X _ { 2 } , . . .$ . be independent and identically distributed with $\mathbb { E } ( X _ { i } ) = \mu$ and $\mathrm { V a r } ( X _ { i } ) = \sigma ^ { 2 }$ for each $i = 1 , 2 , . . . ,$ and let 

$$
Z _ {n} = \frac {X _ {1} + \ldots + X _ {n} - n \mu}{\sigma \sqrt {n}}.
$$

Then $Z _ { n } \to Z$ in distribution, where $Z \sim N ( 0 , 1 )$ 

<table><tr><td><eq>\mathbb{R}</eq></td><td>the set of real numbers</td></tr><tr><td><eq>\mathbb{R}_{+}</eq></td><td>the set of non-negative real numbers <eq>[0, \infty)</eq></td></tr><tr><td><eq>\mathbb{N}</eq></td><td>the set of natural numbers <eq>\{1, 2, \ldots\}</eq></td></tr><tr><td><eq>\mathbb{C}</eq></td><td>the set of complex numbers</td></tr><tr><td><eq>\mathbb{Z}</eq></td><td>the set of integers <eq>\{\ldots, -2, -1, 0, 1, 2, \ldots\}</eq></td></tr><tr><td><eq>\mathbb{Z}_{+}</eq></td><td>the set of non-negative integers <eq>\{0, 1, 2, \ldots\}</eq></td></tr><tr><td><eq>A^{c}</eq></td><td>the complement of a set <eq>A</eq>, <eq>A^{c} = \{\omega \in \Omega, \omega \notin A\}</eq></td></tr><tr><td><eq>F_{X}</eq></td><td>the distribution function of a random variable <eq>X</eq></td></tr><tr><td><eq>p_{X}</eq></td><td>the mass function of a discrete random variable <eq>X</eq></td></tr><tr><td><eq>f_{X}</eq></td><td>the density function of an absolutely continuous random variable <eq>X</eq></td></tr><tr><td><eq>\phi_{X}</eq></td><td>the characteristic function of <eq>X</eq></td></tr><tr><td><eq>\mathbb{E}(X)</eq></td><td>the expected value of the random variable <eq>X</eq></td></tr><tr><td><eq>\text{Var}(X)</eq></td><td>the variance of <eq>X</eq></td></tr><tr><td><eq>\text{Cov}(X,Y)</eq></td><td>the covariance of <eq>X</eq> and <eq>Y</eq></td></tr><tr><td><eq>\mathbb{E}(X|B)</eq></td><td>the conditional expectation of <eq>X</eq> given the event <eq>B</eq></td></tr><tr><td><eq>a \wedge b</eq></td><td><eq>\min\{a, b\}</eq></td></tr><tr><td><eq>a \vee b</eq></td><td><eq>\max\{a, b\}</eq></td></tr><tr><td><eq>a^{+}</eq></td><td><eq>\max\{a, 0\}</eq></td></tr><tr><td><eq>\limsup_{n \uparrow \infty} x_{n}</eq></td><td>the limit superior of the sequence <eq>x_{1}, x_{2}, \ldots</eq></td></tr><tr><td><eq>\liminf_{n \uparrow \infty} x_{n}</eq></td><td>the limit inferior of the sequence <eq>x_{1}, x_{2}, \ldots</eq></td></tr><tr><td><eq>a \cdot b</eq></td><td>Euclidean inner (or dot) product in <eq>\mathbb{R}^{n}</eq>, <eq>a \cdot b = \sum_{i=1}^{n} a_{i} b_{i}</eq></td></tr><tr><td><eq>|a|</eq></td><td>Euclidean norm in <eq>\mathbb{R}^{n}</eq>, <eq>|a| = (a \cdot a)^{1/2}</eq></td></tr><tr><td><eq>X \sim \nu</eq></td><td>the random variable <eq>X</eq> is distributed as the probability measure <eq>\nu</eq></td></tr><tr><td><eq>\mathbb{1}_{A}</eq></td><td>the indicator function of the event <eq>A</eq></td></tr><tr><td><eq>N(\mu, \sigma^{2})</eq></td><td>the normal distribution with mean <eq>\mu</eq> and variance <eq>\sigma^{2}</eq></td></tr><tr><td><eq>N_{n}(\mu, V)</eq></td><td>the <eq>n</eq>-dimensional normal distribution with mean <eq>\mu \in \mathbb{R}^{n}</eq>and variance <eq>V \in \mathbb{R}^{n \times n}</eq></td></tr><tr><td><eq>\text{bin}(n, p)</eq></td><td>the binomial distribution with parameters <eq>n</eq> and <eq>p</eq></td></tr><tr><td><eq>\text{unif}(a, b)</eq></td><td>the uniform distribution on the interval <eq>(a, b)</eq></td></tr><tr><td><eq>L^{p}</eq></td><td>the set of random variables <eq>X</eq> with <eq>\mathbb{E}|X|^{p} &lt; \infty</eq></td></tr><tr><td colspan="2">TABLE 1. Notation</td></tr></table>