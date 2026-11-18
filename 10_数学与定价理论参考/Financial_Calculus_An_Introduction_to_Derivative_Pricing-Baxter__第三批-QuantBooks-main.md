

<!-- === Source: MinerU_markdown_Financial_Calculus_An_Introduction_to_Derivative_Pricing-Baxter__第三批-QuantBooks-main_1_2122707855927779334.md (Page 1) === -->

## Financial Calculus

Vans Dus of Vom Ener 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/848bfe3a251173b014fe9489e4d1182231bfb844797c58324138c3ce8930840c.jpg)


## Financial calculus An introduction to derivative pricing

Martin Baxter 

Nomura International London 

Andrew Rennie 

Head of Debt Analytics, Merrill Lynch, Europe 

PUBLISHED BY THE PRESS SYNDICATE OF THE UNIVERSITY OF CAMBRIDGE
The Pitt Building, Trumpington Street, Cambridge, United Kingdom 

CAMBRIDGE UNIVERSITY PRESS
The Edinburgh Building, Cambridge CB2 2RU, UK
40 West 20th Street, New York, NY 10011-4211,
477 Williamstown Road, Port Melbourne, VIC 3207, Australia
Ruiz de Alarcón 13, 28014 Madrid, Spain
Dock House, The Waterfront, Cape Town 8001, South Africa 

http://www.cambridge.org 

© M.W. Baxter and A.J.O. Rennie 1996 

This book is in copyright. Subject to statutory exception and to the provisions of relevant collective licensing agreements, no reproduction of any part may take place without the written permission of Cambridge University Press. 

First published 1996
Reprinted with corrections 1997
Ninth printing 2003 

Printed in the United Kingdom at the University Press, Cambridge 

Typeset in Monotype Bembo by the authors using TEX 

A catalogue record for this book is available from the British Library 

ISBN 0 521 55289 3 hardback 

## Contents

Preface
The parable of the bookmaker
1
Chapter 1 Introduction
1.1 Expectation pricing
1.2 Arbitrage pricing
1.3 Expectation vs arbitrage
3
4
7
9
Chapter 2 Discrete processes
2.1 The binomial branch model
2.2 The binomial tree model
2.3 Binomial representation theorem
2.4 Overture to continuous models
10
10
17
28
41
Chapter 3 Continuous processes
3.1 Continuous processes
3.2 Stochastic calculus
3.3 Itô calculus
3.4 Change of measure – the C-M-G theorem
3.5 Martingale representation theorem
3.6 Construction strategies
3.7 Black–Scholes model
3.8 Black–Scholes in action
44
45
51
57
63
76
80
83
92 

## Contents

Chapter 4 Pricing market securities 99
4.1 Foreign exchange 99
4.2 Equities and dividends 106
4.3 Bonds 112
4.4 Market price of risk 116
4.5 Quantos 122
Chapter 5 Interest rates 128
5.1 The interest rate market 129
5.2 A simple model 135
5.3 Single-factor HJM 142
5.4 Short-rate models 149
5.5 Multi-factor HJM 158
5.6 Interest rate products 163
5.7 Multi-factor models 172
Chapter 6 Bigger models 178
6.1 General stock model 178
6.2 Log-normal models 181
6.3 Multiple stock models 183
6.4 Numeraires 189
6.5 Foreign currency interest-rate models 193
6.6 Arbitrage-free complete models 196
Appendices A1 Further reading 201
A2 Notation 205
A3 Answers to exercises 209
A4 Glossary of technical terms 216
Index 228 

# Preface

Notoriously, works of mathematical finance can be precise, and they can be comprehensible. Sadly, as Dr Johnson might have put it, the ones which are precise are not necessarily comprehensible, and those comprehensible are not necessarily precise. 

But both are needed. The mathematics of finance is not easy, and much market practice is based on a soft understanding of what is actually going on. This is usually enough for experienced practitioners to price existing contracts, but often insufficient for innovative new products. Novices, managers and regulators can be left to stumble around in literature which is ill suited to their need for a clear explanation of the basic principles. Such ‘seat of the pants’ practices are more suited to the pioneering days of an industry, rather than the mature $15 trillion market which the derivatives business has become. 

On the academic side, effort is too often expended on finding precise answers to the wrong questions. When working in isolation from the market, the temptation is to find analytic answers for their own sake with no reference to the concerns of practitioners. In particular, the importance of hedging both as a justification for the price and as an important end in itself is often underplayed. Scholars need to be aware of such financial issues, if only because some of the very best work has arisen in answering the questions of industry rather than academe. 

## Guide to the chapters

Chapter one is a brief warning, especially to beginners, that the expected worth of something is not a good guide to its price. That idea has to be shaken off and arbitrage pricing take its place. 

Chapter two develops the idea of hedging and pricing by arbitrage in the discrete-time setting of binary trees. The key probabilistic concepts of conditional expectation, martingales, change of measure, and representation are all introduced in this simple framework, accompanied by illustrative examples. 

Chapter three repeats all the work of its predecessor in the continuous-time setting. Brownian motion is brought out, as well as the Itô calculus needed to manipulate it, culminating in a derivation of the Black–Scholes formula. 

Chapter four runs through a variety of actual financial instruments, such as dividend paying equities, currencies and coupon paying bonds, and adapts the Black–Scholes approach to each in turn. A general pattern of the distinction between tradable and non-tradable quantities leads to the definition the market price of risk, as well as a warning not to take that name too seriously. A section on quanto products provides a showcase of examples. 

Chapter five is about the interest rate market. In spirit, a market of bonds is much like a market of stocks, but the richness of this market makes it more than just a special case of Black–Scholes. Market models are discussed with a joint short-rate/HJM approach, which lies within the general continuous framework set up in chapter three. One section details a few of the many possible interest rate contracts, including swaps, caps/floors and swaptions. This is a substantial chapter reflecting the depth of financial and technical knowledge that has to be introduced in an understandable way. The aim is to tell one basic story of the market, which all approaches can slot into. 

Chapter six concludes with some technical results about larger and more general models, including multiple stock n-factor models, stochastic numeraires, and foreign exchange interest-rate models. The running link between the existence of equivalent martingale measures and the ability to price and hedge is finally formalised. 

A short bibliography, complete answers to the (small) number of exercises, a full glossary of technical terms and an index are in the appendices. 

## How to read this book

The book can be read either sequentially as an unfolding story, or by random access to the self-contained sections. The occasional questions are to allow 

## Preface

practice of the requisite skills, and are never essential to the development of the material. 

A reader is not expected to have any particular prior body of knowledge, except for some (classical) differential calculus and experience with symbolic notation. Some basic probability definitions are contained in the glossary, whereas more advanced readers will find technical asides in the text from time to time. 

## Acknowledgements

We would like to thank David Tranah at CUP for politely never mentioning the number of deadlines we missed, as well as his much more invaluable positive assistance; the many readers in London, New York and various universities who have been subjected to writing far worse than anything remaining in the finished edition. Special thanks to Lorne Whiteway for his help and encouragement. 

Martin Baxter 

Andrew Rennie 

June 1996 

## The parable of the bookmaker

A bookmaker is taking bets on a two-horse race. Choosing to be scientific, he studies the form of both horses over various distances and goings as well as considering such factors as training, diet and choice of jockey. Eventually he correctly calculates that one horse has a 25% chance of winning, and the other a 75% chance. Accordingly the odds are set at 3–1 against and 3–1 on respectively. 

But there is a degree of popular sentiment reflected in the bets made, adding up to $5000 for the first and $10000 for the second. Were the second horse to win, the bookmaker would make a net profit of $1667, but if the first wins he suffers a loss of $5000. The expected value of his profit is 25% × (-$5000) + 75% × ($1667) = $0, or exactly even. In the long term, over a number of similar but independent races, the law of averages would allow the bookmaker to break even. Until the long term comes, there is a chance of making a large loss. 

Suppose however that he had set odds according to the money wagered – that is, not 3–1 but 2–1 against and 2–1 on respectively. Whichever horse wins, the bookmaker exactly breaks even. The outcome is irrelevant. 

In practice the bookmaker sells more than 100% of the race and the odds are shortened to allow for profit (see table). However, the same pattern emerges. Using the actual probabilities can lead to long-term gain but there is always the chance of a substantial short-term loss. For the bookmaker to earn a steady riskless income, he is best advised to assume the horses' probabilities are something different. That done, he is in the surprising position of being disinterested in the outcome of the race, his income being assured. 

## A note on odds

When a price is quoted in the form n-m against, such as 3-1 against, it means that a successful bet of $m will be rewarded with $n plus stake returned. The implied probability of victory (were the price fair) is m/(m+n). Usually the probability is less than half a chance so the first number is larger than the second. Otherwise, what one might write as 1-3 is often called odds of 3-1 on. 

<table><tr><td>Actual probability</td><td>25%</td><td>75%</td><td></td></tr><tr><td>Bets placed</td><td>$5000</td><td>$10000</td><td></td></tr><tr><td>1. Quoted odds</td><td>13–5 against</td><td>15–4 on</td><td></td></tr><tr><td>Implied probability</td><td>28%</td><td>79%</td><td>Total = 107%</td></tr><tr><td>Profit if horse wins</td><td>-$3000</td><td>$2333</td><td>Expected profit = $1000</td></tr><tr><td>2. Quoted odds</td><td>9–5 against</td><td>5–2 on</td><td></td></tr><tr><td>Implied probability</td><td>36%</td><td>71%</td><td>Total = 107%</td></tr><tr><td>Profit if horse wins</td><td>$1000</td><td>$1000</td><td>Expected profit = $1000</td></tr></table>

Allowing the bookmaker to make a profit, the odds change slightly. In the first case, the odds relate to the actual probabilities of a horse winning the race. In the second, the odds are derived from the amounts of money wagered. 

## Chapter 1 Introduction

Financial market instruments can be divided into two distinct species. There are the ‘underlying’ stocks: shares, bonds, commodities, foreign currencies; and their ‘derivatives’, claims that promise some payment or delivery in the future contingent on an underlying stock’s behaviour. Derivatives can reduce risk – by enabling a player to fix a price for a future transaction now, for example – or they can magnify it. A costless contract agreeing to pay off the difference between a stock and some agreed future price lets both sides ride the risk inherent in owning stock without needing the capital to buy it outright. 

In form, one species depends on the other – without the underlying (stock) there could be no future claims – but the connection between the two is sufficiently complex and uncertain for both to trade fiercely in the same market. The apparently random nature of stocks filters through to the claims – they appear random too. 

Yet mathematicians have known for a while that to be random is not necessarily to be without some internal structure – put crudely, things are often random in non-random ways. The study of probability and expectation shows one way of coping with randomness and this book will build on probabilistic foundations to find the strongest possible links between claims and their random underlying stocks. The current state of truth is, however, unfortunately complex and there are many false trails through this zoo of the new. Of these, one is particularly tempting. 

## Introduction

## 1.1 Expectation pricing

Consider playing the following game – someone tosses a coin and pays you one dollar for heads and nothing for tails. What price should you pay for this prize? If the coin is fair, then heads and tails are equally likely – about half the time you should win the dollar and the rest of the time you should receive nothing. Over enough plays, then, you expect to make about fifty cents a go. So paying more than fifty cents seems extravagant and less than fifty cents looks extravagant for the person offering the game. Fifty cents, then, seems about right. 

Fifty cents is also the expected profit from the game under a more formal, mathematical definition of expectation. A probabilistic analysis of the game would observe that although the outcome of each coin toss is essentially random, this is not inconsistent with a deeper non-random structure to the game. We could posit that there was a fixed measure of likelihood attached to the coin tossing, a probability of the coin landing heads or tails of $\frac{1}{2}$ . And along with a probability ascription comes the idea of expectation, in this discrete case, the total of each outcome's value weighted by its attached probability. The expected payoff in the game is $\frac{1}{2} \times 1 + \frac{1}{2} \times 0 = 0.50$ . 

This formal expectation can then be linked to a ‘price’ for the game via something like the following: 

## Kolmogorov's strong law of large numbers

Suppose we have a sequence of independent random numbers $X_{1}$ , $X_{2}$ , $X_{3}$ , and so on, all sampled from the same distribution, which has mean (expectation) $\mu$ , and we let $S_{n}$ be the arithmetical average of the sequence up to the $n$ th term, that is $S_{n} = (X_{1} + X_{2} + \ldots + X_{n}) / n$ . Then, with probability one, as $n$ gets larger the value of $S_{n}$ tends towards the mean $\mu$ of the distribution. 

If the arithmetical average of outcomes tends towards the mathematical expectation with certainty, then the average profit/loss per game tends towards the mathematical expectation less the price paid to play the game. If this difference is positive, then in the long run it is certain that you will end up in profit. And if it is negative, then you will approach an overall loss with certainty. In the short term of course, nothing can be guaranteed, but over time, expectation will out. Fifty cents is a fair price in this sense. 

## 1.1 Expectation pricing

But is it an enforceable price? Suppose someone offered you a play of the game for 40 cents in the dollar, but instead of allowing you a number of plays, gave you just one for an arbitrarily large payoff. The strong law lets you take advantage of them over repeated plays: 40 cents a dollar would then be financial suicide, but it does nothing if you are allowed just one play. Mortgaging your house, selling off all your belongings and taking out loans to the limit of your credit rating would not be a rational way to take advantage of this source of free money. 

So the ‘market’ in this game could trade away from an expectation justified price. Any price might actually be charged for the game in the short term, and the number of ‘buyers’ or ‘sellers’ happy with that price might have nothing to do with the mathematical expectation of the game’s outcome. But as a guide to a starting price for the game, a ball-park amount to charge, the strong law coupled with expectation seems to have something going for it. 

## Time value of money

We have ignored one important detail – the time value of money. Our analysis of the coin game was simplified by the payment for and the payoff from the game occurring at the same time. Suppose instead that the coin game took place at the end of a year, but payment to play had to be made at the beginning – in effect we had to find the value of the coin game's contingent payoff not as of the future date of play, but as of now. 

If we are in January, then one dollar in December is not worth one dollar now, but something less. Interest rates are the formal acknowledgement of this, and bonds are the market derived from this. We could assume the existence of a market for these future promises, the prices quoted for these bonds being structured, derivable from some interest rate. Specifically: 

## Time value of money

We assume that for any time T less than some time horizon $\tau$ , the value now of a dollar promised at time T is given by $\exp(-rT)$ for some constant r > 0. The rate r is then the continuously compounded interest rate for this period. 

## Introduction

The interest rate market doesn't have to be this simple; $r$ doesn't have to be constant. And indeed in real markets it isn't. But here we assume it is. We can derive a strong-law price for the game played at time $T$ . Paying 50 cents at time $T$ is the same as paying $50\exp(-rT)$ cents now. Why? Because the payment of 50 cents at time $T$ can be guaranteed by buying half a unit of the appropriate bond (that is, promise) now, for cost $50\exp(-rT)$ cents. Thus the strong-law price must be not 50 cents but $50\exp(-rT)$ cents. 

## Stocks, not coins

What about real stock prices in a real financial market? One widely accepted model holds that stock prices are log-normally distributed. As with the time value of money above, we should formalise this belief. 

## Stock model

We assume the existence of a random variable X, which is normally distributed with mean $\mu$ and standard deviation $\sigma$ , such that the change in the logarithm of the stock price over some time period T is given by X. That is 

$$
\log S _ {T} = \log S _ {0} + X, \quad \text {or} \quad S _ {T} = S _ {0} \exp (X).
$$

Suppose, now, that we have some claim on this stock, some contract that agrees to pay certain amounts of money in certain situations – just as the coin game did. The oldest and possibly most natural claim on a stock is the forward: two parties enter into a contract whereby one agrees to give the other the stock at some agreed point in the future in exchange for an amount agreed now. The stock is being sold forward. The ‘pricing question’ for the forward stock ‘game’ is: what amount should be written into the contract now to pay for the stock one year in the future? 

We can dress this up in formal notation - the stock price at time $T$ is given by $S_T$ , and the forward payment written into the contract is $K$ , thus the value of the contract at its expiry, that is when the stock transfer actually takes place, is $S_T - K$ . The time value of money tells us that the value of this claim as of now is $\exp(-rT)(S_T - K)$ . The strong law suggests that the expected value of this random amount, $\mathbb{E}\big(\exp(-rT)(S_T - K)\big)$ , should 

## 1.2 Arbitrage pricing

be zero. If it is positive or negative, then long-term use of that pricing should lead to one side's profit. Thus one apparently reasonable answer to the pricing question says K should be set so that $\mathbb{E}\big(\exp(-rT)(S_{T}-K)\big)=0$ , which happens when $K=\mathbb{E}(S_{T})$ . 

What is $\mathbb{E}(S_{T})$ ? We have assumed that $\log(S_{T}) - \log(S_{0})$ is normally distributed with mean $\mu$ and variance $\sigma^{2}$ – thus we want to find $\mathbb{E}\big(S_{0} \exp(X)\big)$ , where X is normally distributed with mean $\mu$ and standard deviation $\sigma$ . For that, we can use a result such as: 

## The law of the unconscious statistician

Given a real-valued random variable X with probability density function $f(x)$ then for any integrable real function h, the expectation of $h(X)$ is 

$$
\mathbb {E} \big (h (X) \big) = \int_ {- \infty} ^ {\infty} h (x) f (x) d x.
$$

Since X is normally distributed, the probability density function for X is 

$$
f (x) = \frac {1}{\sqrt {2 \pi \sigma^ {2}}} \exp \left(\frac {- (x - \mu) ^ {2}}{2 \sigma^ {2}}\right).
$$

Integration and the law of the unconscious statistician then tells us that the expected stock price at time T is $S_{0}\exp(\mu+\frac{1}{2}\sigma^{2})$ . This is the strong-law justified price for the forward contract; just as with the coin game, it can only be a suggestion as to the market's trading level. But the technique will clearly work for more than just forwards. Many claims are capable of translation into functional form, $h(X)$ , and the law of the unconscious statistician should be able to deliver an expected value for them. Discounting this expectation then gives a theoretical value which the strong law tempts us into linking with economic reality. 

## 1.2 Arbitrage pricing

So far, so plausible – but seductive though the strong law is, it is also completely useless. The price we have just determined for the forward could only be the market price by an unfortunate coincidence. With markets where the stock can be bought and sold freely and arbitrary positive and negative amounts of stock can be maintained without cost, trying to trade forward using the strong law would lead to disaster – in most cases there would be unlimited interest in selling forward to you at that price. 

Why does the strong law fail so badly with forwards? As mentioned above in the context of the coin game, the strong law cannot enforce a price, it only suggests. And in this case, another completely different mechanism does enforce a price. The fair price of the contract is $S_{0} \exp(rT)$ . It doesn't depend on the expected value of the stock, it doesn't even depend on the stock price having some particular distribution. Either counterparty to the contract can in fact construct the claim at the start of the contract period and then just wait patiently for expiry to exchange as appropriate. 

## Construction strategy

Consider the seller of the contract, obliged to deliver the stock at time T in exchange for some agreed amount. They could borrow $S_{0}$ now, buy the stock with it, put the stock in a drawer and just wait. When the contract expires, they have to pay back the loan – which if the continuously compounded rate is r means paying back $S_{0} \exp(rT)$ , but they have the stock ready to deliver. If they wrote less than $S_{0} \exp(rT)$ into the contract as the amount for forward payment, then they would lose money with certainty. 

So the forward price is bounded below by $S_{0}\exp(rT)$ . But of course, the buyer of the contract can run the scheme in reverse, thus writing more than $S_{0}\exp(rT)$ into the contract would guarantee them a loss. The forward price is bounded above by $S_{0}\exp(rT)$ as well. 

Thus there is an enforced price, not of $S_0 \exp(\mu + \frac{1}{2} \sigma^2)$ but $S_0 \exp(rT)$ . Any attempt to strike a different price and offer it into a market would inevitably lead to someone taking advantage of the free money available via the construction procedure. And unlike the coin game, mortgaging the house would now be a rational action. This type of market opportunism is old enough to be ennobled with a name - arbitrage. The price of $S_0 \exp(rT)$ is an arbitrage price - it is justified because any other price could lead to unlimited riskless profits for one party. The strong law wasn't wrong - if $S_0 \exp(\mu + \frac{1}{2} \sigma^2)$ is greater than $S_0 \exp(rT)$ , then a buyer of a forward contract expects to make money. (But then of course, if the stock is expected to grow faster than the riskless interest rate $r$ , so would buyers of the stock itself.) But the existence of an arbitrage price, however surprising, overrides the strong 

## 1.3 Expectation vs arbitrage

law. To put it simply, if there is an arbitrage price, any other price is too dangerous to quote. 

## 1.3 Expectation vs arbitrage

The strong law and expectation give the wrong price for forwards. But in a certain sense, the forward is a special case. The construction strategy – buying the stock and holding it – certainly wouldn't work for more complex claims. The standard call option which offers the buyer the right but not the obligation to receive the stock for some strike price agreed in advance certainly couldn't be constructed this way. If the stock price ends up above the strike, then the buyer would exercise the option and ask to receive the stock – having it salted away in a drawer would then be useful to the seller. But if the stock price ends up below the strike, the buyer will abandon the option and any stock owned by the seller would have incurred a pointless loss. 

Thus maybe a strong-law price would be appropriate for a call option, and until 1973, many people would have agreed. Almost everything appeared safe to price via expectation and the strong law, and only forwards and close relations seemed to have an arbitrage price. Since 1973, however, and the infamous Black–Scholes paper, just how wrong this is has slowly come out. Nowhere in this book will we use the strong law again. Just to muddy the waters, though, expectation will be used repeatedly, but it will be as a tool for risk-free construction. All derivatives can be built from the underlying – arbitrage lurks everywhere. 

# Chapter 2 Discrete processes

The goal of this book is to explore the limits of arbitrage. Bit by bit we will put together a mathematical framework strong enough to be a realistic model of the real financial markets and yet still structured enough to support construction techniques. We have a long way to go, though; it seems wise to start very small. 

## 2.1 The binomial branch model

Something random for the stock and something to represent the time-value of money. At the very least we need these two things – any model without them cannot begin to claim any relation to the real financial market. Consider, then, the simplest possible model with a stock and a bond. 

## The stock

Just one time-tick - we start at time $t = 0$ and end a short tick later at time $t = \delta t$ . We need something to represent the stock, and it had better have some unpredictability, some random component. So we suppose that only two things can happen to the stock in this time: an 'up' move or a 'down' move. With just two things allowed to happen, pictorially we have a branch (figure 2.1). 

Our randomness will have some structure - we will assign probabilities to the up and down move: probability $p$ to move up to node 3, and thus $1 - p$ 

## 2.1 The binomial branch model

to move down to node 2. The stock will have some value at the start (node 1 as labelled on the picture), call it $s_1$ . This value represents a price at which we can buy and sell the stock in unlimited amounts. We can then hold on to the stock across the time period until time $t = \delta t$ . Nothing happens to us in the intervening period by dint of holding on to the stock – there is no charge for holding positive or negative amounts – but at the end of the period it will have a new value. If it moves down, to node 2, then it will have value $s_2$ ; up, to node 3, value $s_3$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/ec05b9bd2386895dab6f0a1a8864d9b261771b565cc14b7071722a295502ae77.jpg)



Figure 2.1 The binomial branch


## The bond

We also need something to represent the time-value of money - a cash bond. There will be some continuously compounded interest rate $r$ that will hold for the period $t = 0$ to $t = \delta t -$ one dollar at time zero will grow to $ exp( $r \, \delta t$ ). We should be able to lend at that rate, and borrow - and in arbitrary size. To represent this, we introduce a cash bond $B$ which we can buy or sell at time zero for some price, say $B_0$ , and which will be worth a definite $B_0 \exp(r \, \delta t)$ a tick later. 

These two instruments are our financial world, and simple though it is it still has uncertainties for investors. Only one of the possible stock values might suit a particular player, their plans surviving or failing by the random outcome. Thus there could be a market for instruments dependent on the value the stock takes at the end of the tick-period. The investor's requirement for compensation based on the future value of the stock could be codified by a function $f$ mapping the two future possibilities, node 2 or node 3, to two rewards or penalties $f(2)$ and $f(3)$ . A forward contract, struck at $k$ , for example, could be codified as $f(2) = s_2 - k$ , $f(3) = s_3 - k$ . 

## Risk-free construction

The question can now be posed – exactly what class of functions f can be explicitly constructed via a suitable strategy? Clearly the forward can be – as in chapter one, we would buy the stock (cost: $s_{1}$ ), and sell off cash bonds to fund the purchase. At the end of the period, we would be able to hand over the stock and demand $s_{1}\exp(r\delta t)$ in exchange. The price k of the forward thus has to be $s_{1}\exp(r\delta t)$ exactly as we would have hoped – priced via arbitrage. 

But what about more complex $f$ ? Can we still find a construction strategy? Our first guess would be no. The stock takes one of two random values at the end of the tick-period and the value of the derivative would in general be different as well. The probabilities of each outcome for the derivative $f$ are known, thus we also know the expected value of $f$ at the end of the period as well: $(1 - p)f(2) + pf(3)$ , but we don't know its actual value in advance. 

## Bond-only strategy

All is not lost, though. Consider a portfolio of just the cash bond. The cash bond will grow by a factor of $\exp(r\delta t)$ across the period, thus buying discount bonds to the value of $\exp(-r\delta t)[(1-p)f(2)+pf(3)]$ at the start of the period will provide a value equal to $(1-p)f(2)+pf(3)$ at the end. Why would we choose this value as the target to aim for? Because it is the expected value of the derivative at the end of the period – formally: 

## Expectation for a branch

Let S be a binomial branch process with base value $s_{1}$ at time zero, down-value $s_{2}$ and up-value $s_{3}$ . Then the expectation of S at tick-time 1 under the probability of an up-move p is: 

$$
\mathbb {E} _ {p} (S _ {1}) = (1 - p) s _ {2} + p s _ {3}.
$$

Our claim $f$ on $S$ is just as much a random variable as $S_1$ is - we can meaningfully talk of its expectation. And thus we can meaningfully aim for the expectation of the claim, via the cash bonds. This strategy of construction would at the very least be expected to break even. And the value of the starting 

## 2.1 The binomial branch model

portfolio of cash bonds might be claimed to be a good predictor of the value of the derivative at the start of the period. The price we would predict for the derivative would be the discounted expectation of its value at the end. 

But of course this is just the strong law of chapter one all over again – just thinly disguised as construction. And exactly as before we are missing an element of coercion. We haven't explicitly constructed the two possible values the derivative can take: $f(2)$ and $f(3)$ ; we have simply aimed between them in a probabilistic sense and hoped for the best. 

And we already know that this best isn't good enough for forwards. For a stock that obeys a binomial branch process, its forward price is not suggested by the possible stock values $s_2$ and $s_3$ , but enforced by the interest rate $r$ implied by the cash bond $B$ : namely $s_1 \exp(r \delta t)$ . The discounted expectation of the claim doesn't work as a pricing tool. 

## Stocks and bonds together

But can we do any better? Another strategy might occur to us, we have after all two instruments which we can build into a portfolio to hold for the tick-period. We tried using the guaranteed growth of the cash bond as a device for producing a particular desired value, and we chose the expected value of the derivative as our target point. But we have another instrument tied more strongly to the behaviour of both the stock and the derivative than just the cash bond. Namely the stock itself. Suppose we attempted to guarantee not an amount known in advance which we hope will stand as a reasonable predictor for the value of the derivative, but the value of the derivative itself, whatever it might be. 

Consider a general portfolio $(\phi,\psi)$ , namely $\phi$ of the stock S (worth $\phi s_{1}$ ) and $\psi$ of the cash bond B (worth $\psi B_{0}$ ). If we were to buy this portfolio at time zero, it would cost $\phi s_{1} + \psi B_{0}$ . 

One tick later, though, it would be worth one of two possible values: 

$$
\begin{array}{l l} & \phi s _ {3} + \psi B _ {0} \exp (r   \delta t) \quad \text { after   an   `up' move, } \\ \text { and } & \phi s _ {2} + \psi B _ {0} \exp (r   \delta t) \quad \text { after   a   `down' move. } \end{array}
$$

This pair of equations should intrigue us - we have two equations, two possible claim values and two free variables $\phi$ and $\psi$ . We have two values $f(3)$ and $f(2)$ which we want to duplicate under the appropriate move of the stock, and we have two variables $\phi$ and $\psi$ which we can adjust. Thus the strategy can reduce to solving the following two simultaneous equations for $(\phi, \psi)$ : 

$$
\begin{array}{l} \phi s _ {3} + \psi B _ {0} \exp (r \delta t) = f (3), \\ \phi s _ {2} + \psi B _ {0} \exp (r \delta t) = f (2). \end{array}
$$

Except if perversely $s_2$ and $s_3$ are identical - in which case $S$ is a bond not a stock - we have the solutions: 

$$
\begin{array}{l} \phi = \frac {f (3) - f (2)}{s _ {3} - s _ {2}}, \\ \psi = B _ {0} ^ {- 1} \exp (- r \delta t) \left(f (3) - \frac {(f (3) - f (2)) s _ {3}}{s _ {3} - s _ {2}}\right). \end{array}
$$

What can we do with this algebraic result? If we bought this $(\phi,\psi)$ portfolio and held it, the equations guarantee that we achieve our goal – if the stock moves up, then the portfolio becomes worth $f(3)$ ; and if the stock moves down, the portfolio becomes worth $f(2)$ . We have synthesized the derivative. 

## The price is right

Our simple model allows a surprisingly prescient strategy. Any derivative f can be constructed from an appropriate portfolio of bond and stock. And constructed in advance. This must have some effect on the value of the claim, and of course it does – unlike the expectation derived value, this is enforceable in an ideal market as a rational price. Denote by V the value of buying the $(\phi,\psi)$ portfolio, namely $\phi s_{1} + \psi B_{0}$ , which is: 

$$
V = s _ {1} \left(\frac {f (3) - f (2)}{s _ {3} - s _ {2}}\right) + \exp (- r \delta t) \left(f (3) - \frac {(f (3) - f (2)) s _ {3}}{s _ {3} - s _ {2}}\right).
$$

Now consider some other market maker offering to buy or sell the derivative for a price P less than V. Anyone could buy the derivative from them in arbitrary quantity, and sell the $(\phi,\psi)$ portfolio to exactly match it. At the end of the tick-period the value of the derivative would exactly cancel the value of the portfolio, whatever the stock price was – thus this set of trades carries no risk. But the trades were carried out at a profit of V - P per unit of derivative/portfolio bought – by buying arbitrary amounts, anyone could 

## 2.1 The binomial branch model

make arbitrary risk-free profits. So P would not have been a rational price for the market maker to quote and the market would quickly have mobilised to take advantage of the ‘free’ money on offer in arbitrary quantity. 

Similarly if a market maker quoted the derivative at a price P greater than V, anyone could sell them it and buy the $(\phi,\psi)$ portfolio to lock in a risk-free profit of P-V per unit trade. Again the market would take advantage of the opportunity. 

Only by quoting a two-way price of V can the market maker avoid handing out risk-free profits to other players – hence V is the only rational price for the derivative at time zero, the start of the tick-period. Our model, though allowing randomness, lets arbitrage creep everywhere – the strong law can be banished completely. 

## Example - the whole story in one step

We have an interest-free bond and a stock, both initially priced at $1. At the end of the next time interval, the stock is worth either $2 or $0.50. What is the worth of a bet which pays $1 if the stock goes up? 

Solution. Let B denote the bond price, S the stock price, and X the payoff of the bet. The picture describes the situation: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/7248b4dfa2d147d943bc7a9ed050bd18653fb9f01b99c2bdd796696a1ea99bdc.jpg)



Figure 2.2 Pricing a bet


Buy a portfolio consisting of 2/3 of a unit of stock and a borrowing of 1/3 of a unit of bond. The cost of this portfolio at time zero is $\frac{2}{3} \times \$1 - \frac{1}{3} \times \$1 = \$0.33$ . But after an up-jump, this portfolio becomes worth $\frac{2}{3} \times \$2 - \frac{1}{3} \times \$1 = \$1$ . After a down-jump, it is worth $\frac{2}{3} \times \$0.5 - \frac{1}{3} \times \$1 = \$0$ . The portfolio exactly simulates the bet's payoff, so has to be worth exactly the same as the bet. It must be that the portfolio's initial value of \$0.33 is also the bet's initial value. 

## Expectation regained

A surprise still lurks. The strong-law approach may be useless in this model – leaving aside coincidence, expectation pricing involving the probabilities p and 1 - p leads to risk-free profits being available. But with an eye to rearranging the equations, we can define a simplifying variable: 

$$
q = \frac {s _ {1} \exp (r \delta t) - s _ {2}}{s _ {3} - s _ {2}}.
$$

What can we say about $q$ ? Without loss of generality, we can assume that $s_3$ is bigger than $s_2$ . Were $q$ to be less than or equal to 0, then $s_1 \exp(r \delta t) \leqslant s_2 < s_3$ . But $s_1 \exp(r \delta t)$ is the value that would be obtained by buying $s_1$ worth of the cash bond $B$ at the start of the tick-period. Thus the stock could be bought in arbitrary quantity, financed by selling the appropriate amount of cash bond and a guaranteed risk-free profit made. It is not unreasonable then to eliminate this possibility by fiat - specifying the structure of our market to avoid it. So for any market in which we have a stock which obeys a binomial branch process $S$ , we have $q > 0$ . 

Similarly were q to be greater than or equal to 1, then $s_{2} < s_{3} \leqslant s_{1} \exp(r \delta t) -$ and this time selling stock and buying cash bonds provides unlimited risk-free gains. Thus the structure of a rational market will force q into $(0,1)$ , the interval of points strictly between 0 and 1 – the same constraint we might demand for a probability. 

Now the surprise: when we rewrite the formula for the value V of the $(\phi,\psi)$ portfolio (try it) we get: 

$$
V = \exp (- r \delta t) ((1 - q) f (2) + q f (3)).
$$

Outrageous though it might seem, this is the expectation of the claim under q. This re-appearance of the expectation operator is unsettling. 

The price V is not the expected future value of the derivative (discounted suitably by the growth of the cash bond) – that would involve p in the above formula. Yet V is the discounted expectation with respect to some number q in $(0,1)$ . If we view the expectation operator as implying some information about the future – a strong-law average over many trials, for example – then V is not what we would unconsciously call the expected value. It sounds pedantic to say it, but V is an expectation, not an expected value. And it is easy enough to check that this expectation gives the correct strike for a forward contract: $s_{1} \exp(r \delta t)$ . 

## 2.2 The binomial tree model

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/2737ed24ae5e7b90f6f24b0411db743adc1d60741b22c1ca4042c9bef3c2e5d5.jpg)



Exercise 2.1 Show that a forward contract, struck at k, can be thought of as the payoff f, where $f(2) = s_{2} - k$ and $f(3) = s_{3} - k$ . Now verify, using the formula for V, that the correct strike price is indeed $s_{1} \exp(r \delta t)$ .


## 2.2 The binomial tree model

From branch to tree. Our single time step was simple to analyse, but it represents a bare minimum as a model. It had a random stock and a cash bond, but it only allowed the stock two possible values at the end of a single time period. Markets are not quite that straightforward. But if we could build the branch model up into something more sophisticated, then we could transfer its results into a larger, better model. This is the intention of this section – we shall build a tree out of branches, and see what survives. 

Our financial world will again be just two instruments – a discount bond B and a stock S. Unlimited amounts of either can be bought and sold without transaction costs, default risks, or bid-offer spreads. But now, instead of a single time-period, we will allow many, stringing the individual $\delta t s$ together. 

## The stock

Changes in the value of the stock S must be random – the market demands that – but the randomness can have structure. Our mini-stock from the binomial branch model allowed the stock to change to just two values at the end of the time period, and we shall keep that structure. But now, we will string these choices together into a tree. The very first time period, from t = 0 to $t = \delta t$ , will be just as before (a tree of branches starts with just one simple branch). If the value of S at time zero is $S_{0} = s_{1}$ , then the actual value one tick later is not known but the range of possibilities is $-S_{1}$ has only two possible values: $s_{2}$ and $s_{3}$ . 

Now, we must extend the branch idea in a natural fashion. One tick $\delta t$ later still, the stock again has two possibilities, but dependent on the value at tick-time 1; hence there are four possibilities. From $s_{2}$ , $S_{2}$ can be either $s_{4}$ or $s_{5}$ ; from $s_{3}$ , $S_{2}$ can be either $s_{6}$ or $s_{7}$ . 

As the picture suggests, at tick-time i, the stock can have one of $2^{i}$ possible values, though of course given the value at tick-time $(i - 1)$ , there are still only two admissible possibilities: from node j the process either goes down to node 2j or up to node $2j + 1$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/1aa1c4810b02a47bbcbc3203890d82d45bd6483f7cee78e08f938d06b36a7bd6.jpg)



Binary tree with numbered nodes



Figure 2.3



Stock price development


This tree arrangement gives us considerably more flexibility. A claim can now call on not just two possibilities, but any number. If we think that a thousand random possible values for a stock is a suitable level of complexity, then we merely have to set $\delta t$ small enough that we get ten or so layers of the tree in before the claim time t. We also have a richer allowed structure of probability. Each up/down choice will have an attached probability of it being made. From the standpoint of notation, we can represent this pair of probabilities (which must sum to 1) by just one of them (the up probability) $p_{j}$ , the probability of the stock achieving value $s_{2j+1}$ , given its previous value of $s_{j}$ . The probability of the stock moving down, and achieving value $s_{2j}$ , is then $1 - p_{j}$ . Again this is shown in the picture. 

## The cash bond

To go with our grown-up stock, we need a grown-up cash bond. In the simple branch model, the cash bond behaved entirely predictably; there was a known interest rate $r$ which applied across the period making the cash bond price increase by a factor of $\exp(r\delta t)$ . There is no reason to impose such a strict condition -- we don't have to have a constant interest rate known for the entire tree in advance but instead we could have a sequence of interest rates, $R_0, R_1, \ldots$ , each known at the start of the appropriate tick period. The 

## 2.2 The binomial tree model

value of the cash bond at time $n \delta t$ thus be $B_0 \exp(\sum_{i=0}^{n-1} R_i \delta t)$ . 

It is worth contrasting the cash bond and the stock. We have admitted the possibility of randomness in the cash bond's behaviour (though in fact we will not yet be particularly interested in its exact form). But compared to the stock it is a very different sort of randomness. The cash bond B has the same structure as the time value of money. The interest which must be paid or earned on cash can change over time, but the value of a cash holding at the next tick point is always known, because it depends only on the interest rate already known at the start of the period. 

But for simplicity's sake, we will now keep a constant interest rate $r$ applying everywhere in the tree, and in this case the price of the cash bond at time $n\delta t$ is $B_0\exp (rn\delta t)$ . 

## Trees are complex

At this stage, the binomial structure of the tree may seem rather arbitrary, or indeed unnecessarily simplistic. A tree is better than a single branch, but it still won't allow continuous fluid changes in stock and bond values. In fact, as we shall see, it more than suits our purpose. Our final goal, an understanding of the limitations (or lack of them) of risk-free construction when the underlying stocks take continuous values in continuous time, will draw directly and naturally on this starting point. And as $\delta t$ tends to zero, this model will in fact be more than capable of matching the models we have in mind. Perhaps more pertinently, before we abandon the tree as simplistic, we had better check that it hasn't become too complex for us to make any analytic progress at all. 

## Backwards induction

In fact most of the hard work has already been done when we examined the branch model. Extending the results and intuitions of section 2.1 to an entire binomial tree is surprisingly straightforward. The key idea is that of backwards induction – extending the construction portfolio back one tick at a time from the claim to the required starting place. 

Consider, then, a general claim for our stock S. When we examined a single branching of our tree, we had the function f dependent only on the node chosen at the end of a single tick period – here we can extend the idea of a claim to cover not only the value of S at the time the claim is exercised but also the history of S up until that point. 

The tree structure of the stock was not entirely arbitrary – it embodies a one-to-one relationship between a node and the history of the stock's path up to and including that node. No other history reaches that node; and trivially no other node is reached by that history. This is precisely that condition that allows us actually to associate a claim value with a particular end-node on our tree. We shall also insist on the finiteness of our tree. There must be some final tick-time at which the claim is fully determined. A condition not unreasonable in the real financial world. A general claim can be thought of as some function on the nodes at this claim time-horizon. 

## The two-step

We know that the expectation operator can be made to work for a single branch – here, then, we must wade through the algebra for two time-steps, three branches stuck together into a tree. If two time-steps work, then so will many. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/e48a9923ee193cb4eeb8f610b19c7c58dac0d67bf1f673bf89f9036ea3f07c59.jpg)



Figure 2.4 Double fork at time 0


Suppose that the interest rate over any branch is constant at rate r. Then there exists some set of suitable $q_{j}s$ such that the value of the derivative at node j at tick-time i, $f(j)$ , is 

$$
f (j) = e ^ {- r \delta t} \left(q _ {j} f (2 j + 1) + (1 - q _ {j}) f (2 j)\right).
$$

That is the discounted expectation under $q_{j}$ of the time- $(i+1)$ claim values $f(2j+1)$ and $f(2j)$ . So in our two-step tree (figure 2.4), the two forks from node 3 to nodes 6 and 7, and from node 2 to nodes 4 and 5, are both structurally identical to the simple one-step branch. This means that $f(3)$ comes from $f(6)$ and $f(7)$ via 

$$
f (3) = e ^ {- r \delta t} \bigl (q _ {3} f (7) + (1 - q _ {3}) f (6) \bigr),
$$

and similarly, $f(2)$ comes from $f(4)$ and $f(5)$ , with 

$$
f (2) = e ^ {- r \delta t} \bigl (q _ {2} f (5) + (1 - q _ {2}) f (4) \bigr).
$$

Here $q_{j}$ is the probability $(s_{j}\exp (r\delta t) - s_{2j}) / (s_{2j + 1} - s_{2j})$ , so for instance 

$$
q _ {2} = \frac {s _ {2} \exp (r \delta t) - s _ {4}}{s _ {5} - s _ {4}}, \quad \text { and } \quad q _ {3} = \frac {s _ {3} \exp (r \delta t) - s _ {6}}{s _ {7} - s _ {6}}.
$$

But now we have a value for the claim at time 1; it is worth $f(3)$ if the first jump was up, and $f(2)$ if it was down. But this initial fork from node 1 to nodes 2 and 3 also has the single branch structure. Its value at time zero must be 

$$
f (1) = e ^ {- r \delta t} \left(q _ {1} f (3) + \left(1 - q _ {1}\right) f (2)\right).
$$

Thus the value of the claim at time zero has the daunting looking expression formed by combining the three equations above, 

$$
\begin{array}{l} f (1) = e ^ {- 2 r \delta t} \Big (q _ {1} q _ {3} f (7) + q _ {1} (1 - q _ {3}) f (6) \\ \qquad + (1 - q _ {1}) q _ {2} f (5) + (1 - q _ {1}) (1 - q _ {2}) f (4) \Big). \end{array}
$$

We haven't formally defined expectation on our tree, but it is clear what it must be. 

## Path probabilities

The probability that the process follows a particular path through the tree is just the product of the probabilities of each branch taken. For example, in figure 2.4, the chance of going up twice is the product $q_{1}q_{3}$ , the chance of going up and then down is $q_{1}(1-q_{3})$ , and so on. 

This is a case of the more general slogan that when working with independent events, the probabilities multiply. 

## Expectation on a tree

The expectation of some claim on the final nodes of a tree is the sum over those nodes of the claim value weighted by the probabilities of paths reaching it. 

A two-step tree has four possible paths to the end. But each path carries two probabilities attached to it, one for the first time step and one for the second, thus the path-probability, the probability of following any particular path, must be the product of these. 

The expectation of a claim is then the total of the four outcomes each weighted by this path-probability. But examine the expression we have derived above - it is of course precisely the expectation of the claims $f(7), \ldots, f(4)$ , discounted by the appropriate interest-rate factor $e^{-2r\delta t}$ , under the probabilities $q_1q_3$ , $q_1(1 - q_3)$ , $(1 - q_1)q_2$ , $(1 - q_1)(1 - q_2)$ corresponding to the 'probability tree' $(q_1, q_2, q_3)$ . 

For claim pricing and expectation, a two-step tree is simply three branches. And so on. 

## The inductive step

Returning to our general tree over n periods, we start at its final layer. All nodes here have claim values and are in pairs, the ends of single branchings. Consider any one of these final branchings, from a node at time $(n - 1)$ to two nodes at time n. The results from section 2.1 provide a risk-free construction portfolio $(\phi, \psi)$ of stock and bond at the root of the branch that can generate the time n claim amount. (Both our grown-up stock and the cash bond are indistinguishable over a single branching from the stock and bond of the simple model.) 

Thus the nodes at time $(n-1)$ are all roots of branches that end on the claim layer and have arbitrage guaranteed values for the derivative attached – claim-values in their own right now insisted on not by the investor's contract (that only applies to the final layer) but by arbitrage considerations. Thus we can work back from enforced claims at the final layer to equally strongly enforced claim-values at the layer before. This is the inductive step – we have moved the claims on the final layer back one step. 

## The inductive result

By repeating the inductive step, we will sweep backwards through the tree. Each layer will fix the value of the derivative on the layer before, because each layer is only separated from the layer before by simple branches. What we have done is essentially a recursive filling in process. The investor filled in the nodes at the end of the tree with claims – we filled in the rest by constructing 

## 2.2 The binomial tree model

$(\phi,\psi)$ portfolios at each branching which guaranteed the correct outcome at the next step. 

We will reach the root of the entire tree with a single value. This is the time-zero value of the final derivative claim – why? Because just as for the single branch, there is a construction portfolio which, though it will change at each tick time, will inexorably lead us to the claim payoff required, whatever path the stock actually takes. 

We now have some idea of the complexity of the construction portfolios that will be required. Instead of a single amount of stock $\phi$ , we now have a whole number of them, one per node. And as fate casts the die and the stock jumps on the tree, so this amount will jump as well. Perverse though it may seem for a guaranteed construction procedure, the construction portfolios $(\phi_{i},\psi_{i})$ are also random, just like the stock. But there is a vital structural difference – they are known just in time to be useful, unlike the stock value they are known one-step in advance. 

Arbitrage has worked its way into the tree model as well. The fact that the tree is simply lots of branches was enough to banish the strong law here as well. All claims can be constructed from a stock and bond portfolio, and thus all claims have an arbitrage price. 

## Expectation again

The strong law may be useless, but what about expectation? We had no need of the probabilities $p_{j}$ , but the re-emergence of the expectation operator is not just a coincidence peculiar to the simplicities of the branch model. Yet again the expectation operator will appear with the correct result – just as the conclusion from the previous section was that with respect to a suitable ‘probability’, the expectation operator provided the correct local hedge, here we will see that the expectation operator with respect to some suitable set of ‘probabilities’ also provides the correct global structure for a hedge. 

## A worked example

We can give a concrete demonstration of how this works. The tree in Figure 2.5 is called recombinant as different branches can come back together, or recombine, at the same node. Such trees are computationally much easier to work with, as long as we remember that there is more than one path to the final nodes. The tree nodes are the stock prices, s, and at each node the process will go up with probability 3/4 and down with probability 1/4. (For simplicity, interest rates are zero.) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/b80f4dca431e741036922500de3cab8a958bb37c8a7ba8f73a6929283de29ef7.jpg)



Figure 2.5 A stock price on a recombinant tree


What is the value of an option to buy the stock for 100 at time 3? 

It is easy to fill in the value of the claim on the time 3 column. Reading from top to bottom, the claim has values then of 60, 20, 0 and 0. 

We shall now need our equations for the new probabilities q and the claim values f. As the interest rate r is zero, these equations are a little simpler. If we are about to move either ‘up’ or ‘down’, then the (risk-neutral) probability q is 

$$
q = \frac {s _ {\mathrm{now}} - s _ {\mathrm{down}}}{s _ {\mathrm{up}} - s _ {\mathrm{down}}}
$$

and the value of a claim, $f$ , now is 

$$
f _ {\text { now }} = q f _ {\text { up }} + (1 - q) f _ {\text { down }}.
$$

We calculate that the new q-probabilities are exactly 1/2 at each and every node. Now we can work out the value of the option at the penultimate time 2 by applying the up-down formulae to the final nodes in adjacent pairs. Figure 2.6 shows the result of the first two such calculations. 

We can complete filling in the nodes on level 2, and then repeat the process on level 1, and so on. At the end of this process we have the completed tree (figure 2.7). 

The price of the option at time zero is 15. We can trace through our hedge, using the formula that, at any current time, we should hedge 

$$
\phi = \frac {f _ {\mathrm{up}} - f _ {\mathrm{down}}}{s _ {\mathrm{up}} - s _ {\mathrm{down}}}
$$

units of stock. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/fa9be083942eb63da93cfff9e9f263ab055e54d31585384f406659baf718c8bb.jpg)



time: 0 time: 1 time: 2 time: 3


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/e920dad5839e060977a2b47a0460f56488aee8cc6ecbba4ce2f2c96b775e675d.jpg)



Figure 2.6 The option claims and claim-values at time 2


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/2bca24392ff715085c1c44d16138d24807aa48f1a080d8ebbc8842ac81568227.jpg)



Figure 2.7 The option claim tree


Time 0 We are given 15 for the option. We calculate $\phi$ as $(25 - 5) / (120 - 80) = 0.5$ . Buying 0.5 units of stock costs 50, so we need to borrow an additional 35. 

## Suppose the stock now goes up to 120

Time 1 The new $\phi$ is $(40 - 10) / (140 - 100) = 0.75$ , so we buy another 0.25 

units of stock at its new price, taking our total borrowing to 65. 

## Suppose the stock goes up again to 140

Time 2 The new $\phi$ is $(60 - 20) / (160 - 120) = 1$ , so we take our stock holding up to 1, making our debt now 100. 

## Finally suppose the stock goes down to 120

Time 3 The option will be in the money, and we are exactly placed to hand over one unit of stock and receive 100 in cash to cancel our debt. (In fact, the same would have happened if the stock had gone up to 160 instead.) 

The table below shows exactly how the various processes change over time. The portfolio strategies shown are those in force for the previous tick-period, for instance, $\phi_{1}$ units of stock are held during the interval from i=0 to i=1. The option value matches the worth of both the old and the new portfolios, for instance $V_{1}$ equals both $\phi_{1}S_{1}+\psi_{1}$ and $\phi_{2}S_{1}+\psi_{2}$ . 


Table 2.1 Option and portfolio development


<table><tr><td>Time i</td><td>Last Jump</td><td>Stock Price <eq>S_i</eq></td><td>Option Value <eq>V_i</eq></td><td>Stock Holding <eq>\phi_i</eq></td><td>Bond Holding <eq>\psi_i</eq></td></tr><tr><td>0</td><td>-</td><td>100</td><td>15</td><td>-</td><td>-</td></tr><tr><td>1</td><td>up</td><td>120</td><td>25</td><td>0.50</td><td>-35</td></tr><tr><td>2</td><td>up</td><td>140</td><td>40</td><td>0.75</td><td>-65</td></tr><tr><td>3</td><td>down</td><td>120</td><td>20</td><td>1.00</td><td>-100</td></tr></table>

This was the rosy scenario. What would have happened if the initial jump had been down? 

## Suppose the stock goes down to 80

Time 1 This time, the new $\phi$ is $(10 - 0) / (100 - 60) = 0.25$ . We sell half our stock holding and reduce our debt to 15. 

## Suppose now the stock goes up to 100

Time 2 The next hedge is $(20 - 0) / (120 - 80) = 0.50$ . We buy an extra 0.25 units of stock and our borrowing mounts to 40. 

## Suppose the stock goes down again to 80

Time 3 Our stock is now worth 40, exactly cancelling the debt. But the 

## 2.2 The binomial tree model

option is out of the money, so overall we have broken even. 


Table 2.2 Option and portfolio development along a different path


<table><tr><td>Time i</td><td>Last Jump</td><td>Stock Price <eq>S_i</eq></td><td>Option Value <eq>V_i</eq></td><td>Stock Holding <eq>\phi_i</eq></td><td>Bond Holding <eq>\psi_i</eq></td></tr><tr><td>0</td><td>-</td><td>100</td><td>15</td><td>-</td><td>-</td></tr><tr><td>1</td><td>down</td><td>80</td><td>5</td><td>0.50</td><td>-35</td></tr><tr><td>2</td><td>up</td><td>100</td><td>10</td><td>0.25</td><td>-15</td></tr><tr><td>3</td><td>down</td><td>80</td><td>0</td><td>0.50</td><td>-40</td></tr></table>

We note that all the process above $(S, V, \phi \text{ and } \psi)$ depend on the sequence of up-down jumps. In particular, $\phi$ and $\psi$ are random too, but depend only on the jumps made up to the time when you need to work them out. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/366b65b57f4ccc277d683fba1eb7b93c75bdea386d2b330157625ac826d29e69.jpg)


Exercise 2.2 Repeat the above calculations for a digital contract which pays off 100 if the stock ends higher than it started. 

The expectation result is still here. Under the probability q, the chances of each of the final nodes are (running from top to bottom) 1/8, 3/8, 3/8, and 1/8. The expectation of the claim is indeed 15 under these probabilities, but certainly not under the model probabilities of 3/4-up and 1/4-down. (That gives node probabilities of 27/64, 27/64, 9/64 and 1/64, and a claim expectation of 33.75.) 

## Conclusions

We can sum up. The tree structure ensured that any claim provides just one possible value for its implied derivative instrument at every node or else arbitrage intervened. Claim led to claim-value led to claim-value via backwards induction until the entire tree was filled in. Arbitrage spreads into every branch and thus across any tree. 

Something else happened as well - each branchlet carries its own probability $q_{j}$ under which fixing the value at the branchlet's root can be given by a local expectation operator with parameter $q_{j}$ . The cost of the local construction portfolio $(\phi_{j},\psi_{j})$ can be written as a discounted expectation. But a string of local construction portfolios is a global construction strategy guaranteeing a value. Thus the global discounted expectation operator gives the value of claims on a tree as well. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/d4325434bfbb6c7d835cb5c10a64b4402c44b2011fb0507c36b2862534621d9a.jpg)


## 2.3 Binomial representation theorem

The expectation operator is much more general and constructive an operator than its conventional probabilistic role suggests. We can raise the apparently coincidental finding that there exists some set of $q_{j}$ under which any derivative can be priced by a numerically trivial discounted expectation operation to the status of a theorem. Though it seems strangely formal here where we have the comfort of a pictured tree, when we move to continuous models we shall be glad of any guidance – in the continuous case intuition will often fail. And far from vanishing, the expectation result carries across to the continuous model with ease. 

It is in this spirit, then, that we derive the binomial representation theorem. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/586a460d38303278651cb1e43d48efb7914f90e339a0f722937b9ed8a6b56ac8.jpg)


## 2.3 Binomial representation theorem

## Illustrated definitions

We must start with some formal definitions of concepts we have, in many cases, already met informally. There are seven separate definitions and each will be illustrated by an example on the double forked tree with seven nodes (figure 2.8). 


Figure 2.8 Tree with node numbers Figure 2.9 Tree with price process


(i) We will call the set of possible stock values, one for each node of the tree, and their pattern of interconnections, a process S. One possible process S on our tree is shown in figure 2.9. The random variable $S_{i}$ denotes the value of the process at time i, for instance $S_{1}$ is either 60 or 120 depending on whether we are at node 2 or node 3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/f073f1cfb7e15c9e0c70883fc64ae23d46d578f5078171762b47fe2360caf228.jpg)



Figure 2.10a The measure $\mathbb{P}$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/b9c04c752dfeac045b467eda2d3c3829ca36578277d075b073508ca335243883.jpg)



Figure 2.10b The measure $\mathbb{Q}$


(ii) Separate from the process S, we will call the set of ‘probabilities’ $(p_{j})$ 

or $(q_{j})$ a measure P or Q on the tree. The measure describes how likely any up/down jump is at each node, represented by $p_{j}$ , the probability of moving upwards from node j. We could choose a simple measure P with all jumps equally likely (figure 2.10a) or a more complex measure like Q (shown in figure 2.10b). 

Notice that in our formal system, we have separated two components that would normally be seen as intimately connected parts of the same whole – the probability of an up-move, and where the up-move is to. They may not seem too different in character but the lesson of both the preceding sections is that this intuitive elision is unwise. We didn't need the real world measure $\mathbb{P}$ in order to find the measure which allowed risk-free construction. That measure was a function of $S$ and no function of $\mathbb{P}$ . The size and interrelation of up-moves affects the values of derivatives, the probabilities of achieving them does not. 

This separation of process and measure isn't artificial – it is fundamental to everything we have to do. Put crudely, the strong law failed precisely because it paid attention to both $S$ and $\mathbb{P}$ , not $S$ alone. 

(iii) A filtration $(\mathcal{F}_i)$ is the history of the stock up until tick-time $i$ on the tree. The filtration starts at time zero with $\mathcal{F}_0$ equal to the path consisting of the single node 1, that is $\mathcal{F}_0 = \{1\}$ . By time 1, the filtration will either be $\mathcal{F}_1 = \{1,2\}$ if the first jump was down, or $\mathcal{F}_1 = \{1,3\}$ if it was up. In full the filtration associated with each node is 


Table 2.3 The filtration process


<table><tr><td>node</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td></tr><tr><td>filtration</td><td>{1}</td><td>{1,2}</td><td>{1,3}</td><td>{1,2,4}</td><td>{1,2,5}</td><td>{1,3,6}</td><td>{1,3,7}</td></tr></table>

It thus corresponds to a particular node achieved at time i. Why? Because the binomial structure ensures it – check for yourself that there is only one path to any given node. The filtration fixes a history of choices, and thus fixes a node. To know where you are is the same as knowing the filtration (at least in non-recombinant trees). 

(iv) A claim $X$ on the tree is a function of the nodes at a claim time-horizon $T$ . Or equivalently it is a function of the filtration $\mathcal{F}_T$ , thanks to the 

## 2.3 Binomial representation theorem

one-to-one relationship between nodes and paths. For instance, the value of the process at time 2, $S_{2}$ , is a claim, as is the value of a call struck at 70 and the maximum price the stock attained along its path (table 2.4). 


Table 2.4 Some claims at time 2


<table><tr><td>time 2 node</td><td><eq>S_{2}</eq></td><td><eq>(S_{2}-70)^{+}</eq></td><td><eq>\max\{S_{0},S_{1},S_{2}\}</eq></td></tr><tr><td>7</td><td>180</td><td>110</td><td>180</td></tr><tr><td>6</td><td>80</td><td>10</td><td>120</td></tr><tr><td>5</td><td>72</td><td>2</td><td>80</td></tr><tr><td>4</td><td>36</td><td>0</td><td>80</td></tr></table>

The crucial difference between a claim and a process, is that the claim is only defined on the nodes at time T, while a process is defined at all times up to and including T. 


Table 2.5 Conditional expectation against filtration value


<table><tr><td>Expectation</td><td>Filtration value</td><td>Value</td></tr><tr><td><eq>\mathbb{E}_{\mathbb{P}}(S_2|\mathcal{F}_0)</eq></td><td>{1}</td><td><eq>(180 + 80 + 72 + 36)/4 = 92</eq></td></tr><tr><td rowspan="2"><eq>\mathbb{E}_{\mathbb{P}}(S_2|\mathcal{F}_1)</eq></td><td>{1,3}</td><td><eq>\frac{1}{2}(180 + 80) = 130</eq></td></tr><tr><td>{1,2}</td><td><eq>\frac{1}{2}(72 + 36) = 54</eq></td></tr><tr><td rowspan="4"><eq>\mathbb{E}_{\mathbb{P}}(S_2|\mathcal{F}_2)</eq></td><td>{1,3,7}</td><td>180</td></tr><tr><td>{1,3,6}</td><td>80</td></tr><tr><td>{1,2,5}</td><td>72</td></tr><tr><td>{1,2,4}</td><td>36</td></tr></table>

(v) The conditional expectation operator $\mathbb{E}_{\mathbb{Q}}(\cdot|\mathcal{F}_{i})$ extends our idea of expectation to two parameters – a measure Q and a history $F_{i}$ . The measure Q we might have guessed – it tells us which ‘probabilities’ to use in determining path-probability and thus the expectation. But so far we have only been interested in taking expectations along the whole of a path from time zero, and it is useful to take expectations from later starting points. The filtration serves this purpose. For a claim X, the quantity $\mathbb{E}_{\mathbb{Q}}(X|\mathcal{F}_{i})$ is the expectation of X along the latter portion of paths which have initial segment $F_{i}$ . We regard the node reached at time i as the new root of our tree, and take expectations of future claims from there. This conditional expectation has an enforced dependence on the value of the filtration $F_{i}$ , and so is itself a random variable. 

For each node at time i, $\mathbb{E}_{\mathbb{Q}}(X|\mathcal{F}_{i})$ is the expectation of X if we have already got to that node. As an example, we take P to be the measure in figure 2.10a and X to be the claim $S_{2}$ (table 2.5). 

Sensibly enough, starting at the root gives the same answer as the unconditioned expectation $\mathbb{E}_{\mathbb{P}}(S_{2})$ , whereas ‘starting’ at time 2 leaves no further time for development, so $\mathbb{E}_{\mathbb{P}}(S_{2}|\mathcal{F}_{2}) = S_{2}$ , for every possible value of the filtration $F_{2}$ . 

We could also see $\mathbb{E}_{\mathbb{P}}(X|\mathcal{F}_{i})$ as a process in i. In the case of $X = S_{2}$ , it is shown in figure 2.11. In this way we can convert a claim into a process, given a measure. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/3cc3aed088cadaf9415373c28bc0476a018ff69b18b8710ec540fbbaf0dd25a4.jpg)



Figure 2.11 Conditional expectation process $\mathbb{E}_{\mathbb{P}}(S_2|\mathcal{F}_i)$


(vi) A previsible process $\phi = \phi_i$ is a process on the same tree whose value at any given node at time-tick $i$ is dependent only on the history up to one time-tick earlier, $\mathcal{F}_{i-1}$ . What can we say about a previsible process? Given the one-to-one relationship between nodes and histories on our binary tree, it is certainly a binomial tree process in its own right, whose values are well defined at each node later than time zero. But compared to the main process $S$ , it is known one node in advance. It doesn't seem to notice branches until one time-step after they have happened. For instance a random bond price process $B_i$ would be previsible, as is the delayed price process $\phi_i = S_{i-1}, i \geqslant 1$ (figure 2.12). It is not always sensible to define the value that a previsible process has at time zero. 

## 2.3 Binomial representation theorem

Previsible processes will play the part of trading strategies, where we cannot tell in advance where prices are going to go. This is an essential feature of any model that excludes arbitrage (or insider trading). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/f41d5ad28d132b58e273ad46a3f2938c33e5e825c5e3da73c8343ac598a16dff.jpg)



Figure 2.12 The previsible process $S_{i-1}$


Our final definition is probably the most important of all – one question that we must surely ask soon is: what is the risk-free construction measure? Is it specific to the task in hand, or is it special in some other way as well? 

(vii) A process $S$ is a martingale with respect to a measure $\mathbb{P}$ and a filtration $(\mathcal{F}_i)$ if 

$$
\mathbb {E} _ {\mathbb {P}} (S _ {j} | \mathcal {F} _ {i}) = S _ {i}, \quad \text {   for   all   } i \leqslant j.
$$

This daunting expression needs expansion. Written out, for S to be a martingale with respect to a measure P, it means that the future expected value at time j of the process S under measure P (for of course our formal expectation demands a measure, it has no meaning without one) conditional on its history up until time i is merely the process' value at time i. 

Re-written again, that means the process S has no drift under P, no bias up or down in its value under the expectation operator $E_{P}$ . If the process has value 100 at some point, then its conditional expected value under P is 100 thereafter. 

Example (1). The process which constantly takes a fixed value is, rather trivially, a martingale with respect to all possible measures. 

Example (2). Our illustrative process S is actually a martingale under the measure Q given in figure 2.10b. For instance $\mathbb{E}_{\mathbb{Q}}(S_{1}|\mathcal{F}_{0})$ equals $\frac{1}{3} \times 120 + \frac{2}{3} \times 60 = 80$ , and 80 is indeed the value of $S_{0}$ . Slightly harder, $\mathbb{E}_{\mathbb{Q}}(S_{2}|\mathcal{F}_{1})$ equals $\frac{2}{5} \times 180 + \frac{3}{5} \times 80 = 120$ if the first jump was up, which matches the value $S_{1}$ takes if the first jump is up. The down-jump case and all the others need to be checked separately. 

Example (3). The conditional expectation process $N_{i} = \mathbb{E}_{\mathbb{P}}(S_{2}|\mathcal{F}_{i})$ is a P-martingale. Because of the nature of its definition we only need to check that $\mathbb{E}_{\mathbb{P}}(N_{1}|\mathcal{F}_{0})$ is equal to $N_{0}$ . As this is just $\frac{1}{2} \times 130 + \frac{1}{2} \times 54 = 92$ , it is immediate. 

The last example above is a particular example of a general result. 

## The conditional expectation process of a claim

For any claim $X$ , the process $\mathbb{E}_{\mathbb{P}}(X|\mathcal{F}_i)$ is always a $\mathbb{P}$ -martingale. 

To see this to be true, we need to use the fact that 

$$
\mathbb {E} _ {\mathbb {P}} \left(\mathbb {E} _ {\mathbb {P}} (X | \mathcal {F} _ {j}) \mid \mathcal {F} _ {i}\right) = \mathbb {E} _ {\mathbb {P}} (X | \mathcal {F} _ {i}), \quad i \leqslant j.
$$

In other words, that conditioning firstly on the history up to time j and then conditioning on the history up to an earlier time i is the same as just conditioning originally up to time i. This result is called the tower law. 

Given the tower law, an easy check of whether a process is a P-martingale or not is to compare the process $S_{i}$ itself with the conditional expectation process of its terminal value $\mathbb{E}_{\mathbb{P}}(S_{T}|\mathcal{F}_{i})$ . Only if these are identical is the process a P-martingale. 

We must also take the P dependence seriously. The process S is not a martingale on its own, it is a P-martingale, it is a martingale with respect to the measure P. And of course, exactly the same process can be a martingale with respect to one measure and not to another. For instance, our illustrative process S is not a P-martingale (because figure 2.9 and figure 2.11 are different), but it is a Q-martingale, where Q is given in figure 2.10b. Such a Q is called a martingale measure for S. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/54d06dc94c5ae93bb827028e63cb20734a215cc8c64938c44207081e8db966d1.jpg)


Exercise 2.3 Check that $\mathbb{E}_{\mathbb{Q}}(S_2|\mathcal{F}_i)$ is the same as $S_{i}$ , and so prove that $S$ is a $\mathbb{Q}$ -martingale. 

## 2.3 Binomial representation theorem

## Binomial representation theorem

We can now write down our theorem. 

## Binomial representation theorem

Suppose the measure Q is such that the binomial price process S is a Q-martingale. If N is any other Q-martingale, then there exists a previsible process $\phi$ such that 

$$
N _ {i} = N _ {0} + \sum_ {k = 1} ^ {i} \phi_ {k} \Delta S _ {k},
$$

where $\Delta S_{i} := S_{i} - S_{i-1}$ is the change in S from tick-time i - 1 to i, and $\phi_{i}$ is the value of $\phi$ at the appropriate node at tick-time i. 

We can get from $N_{0}$ to $N_{i}$ previsibly, with steps we know in advance. The proof is formal but straightforward – with the work we have put in already, this kind of manipulation should be second nature. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/803849b40ecbde7060dd6d749127ba2d82bde76f0ecbebacbe9903e0d02910d7.jpg)



Figure 2.13 The branch geometry (process S on left; process N on right)


Consider a single branching from a node at tick-time i - 1 to two nodes 'up' and 'down' at tick-time i. The structure of the tree ensures that the history $F_{i}$ has two choices beyond $F_{i-1}$ , corresponding to the up jump and down jumps respectively. The increments over the branch of the processes S and N are 

$$
\Delta S _ {i} = S _ {i} - S _ {i - 1} \quad \text { and } \quad \Delta N _ {i} = N _ {i} - N _ {i - 1}.
$$

The variability that these increments contain depends on the geometry of the branch itself (figure 2.13). 

There are only two places to go, so any random variable dependent on the branch is fully determined by its width size and a constant offset depending only on $F_{i-1}$ . So if we want to construct one random process out of another, it will in general be a construction based on a scaling (to match the widths) and a shift (to match the offsets). 

Consider then the scaling first. The size of the difference between the up and down jump values is $\delta s_{i} = s_{up} - s_{down}$ for S and $\delta n_{i} = n_{up} - n_{down}$ for N, both of these dependent only on the filtration $F_{i-1}$ . So we define $\phi_{i}$ to be the ratio of these branch widths, that is 

$$
\phi_ {i} = \frac {\delta n _ {i}}{\delta s _ {i}}.
$$

Now we can worry about the shift - the $N$ -increment $\Delta N_{i}$ must be given by the scaled increment $\phi_i\Delta S_i$ plus an offset $k$ , this $k$ again determined only by $\mathcal{F}_{i-1}$ . That is 

$$
\Delta N _ {i} = \phi_ {i} \Delta S _ {i} + k, \quad \text {   for   } \phi_ {i} \text {   and   } k \text {   known   by   } \mathcal {F} _ {i - 1}.
$$

But $S$ and $N$ are $\mathbb{Q}$ -martingales, that is $\mathbb{E}_{\mathbb{Q}}(\Delta N_i|\mathcal{F}_{i-1})$ and $\mathbb{E}_{\mathbb{Q}}(\Delta S_i|\mathcal{F}_{i-1})$ are both zero - the increments have zero expectation conditional on the history $\mathcal{F}_{i-1}$ . The scaling factor $\phi_i$ is previsible, that is known by time $i-1$ , so we also have $\mathbb{E}_{\mathbb{Q}}(\phi_i\Delta S_i|\mathcal{F}_{i-1}) = 0$ . Thus the offset $k$ must be zero as well $(0 = 0 + k)$ . 

So the general scale and shift reduces in the case where S and N are both Q-martingales to just a scaling 

$$
\Delta N _ {i} = \phi_ {i} \Delta S _ {i}.
$$

And of course induction ties all these increments together to give the result we want. 

## Financial application

We now have a theorem; but it is a formal theorem about binomial tree processes and measures. Nowhere in our proof do we consider portfolios of a stock and bond; nowhere do we consider arbitrage or market implications. We go through many of the same steps as we had to in section 2.2, but we haven't reached a financial conclusion. How then can we use the binomial representation theorem for pricing? 

## 2.3 Binomial representation theorem

In our binomial tree model for the market, the stock follows a binomial process S. And if there were a measure Q which made S a martingale, we could use the representation theorem to represent some other martingale $N_{i}$ in terms of the stock price. The previsible $\phi$ from the theorem could act as a construction strategy. At each point we could buy the appropriate $\phi_{i}$ of the stock and we would follow the gains and losses of the martingale $N_{i}$ . 

We would be able to match the martingale step for step, starting where it starts and finishing where it ends, wherever that might be. If the martingale ended in a claim, than that claim would have been synthesized. 

Two things stand in our way, though. Firstly we have a claim X, not a martingale. And though we would like to end up at the claim, the claim doesn't start or end anywhere. It isn't a process, it's a random variable. Secondly, we have not just a stock but a cash bond as well. X-ray vision or intuition would suggest that the $\phi_{i}$ of the binomial representation theorem is going to be a vital part of our formal construction strategy but, to use the notation of earlier, we need a $\psi_{i}$ as well. With each stock holding comes a bond holding. 

First things first. The claim X is a random variable but we have already seen one trick for turning random variables into processes. Given any measure Q, we can form the process 

$$
E _ {i} = \mathbb {E} _ {\mathbb {Q}} (X | \mathcal {F} _ {i}),
$$

by taking conditional expectations. Even better, as we have already observed, whatever measure Q we choose, $E_{i}$ is automatically a Q-martingale. Thus if we find Q, a measure under which $S_{i}$ is a Q-martingale, the appropriate $E_{i}$ is one as well. 

What about the cash bond? Ultimately we will simply have to grind through the algebra but a bit of intuition can guide us to what the answer might look like. The cash bond $B_i$ represents the growth of money – $1 today is not the same as $1 at time i, all things being equal. One dollar today is like $B_i$ dollars at time i. But we would like to be in a world without the growth of money – so we could simply factor it away. 

The bond process $B_{i}$ is previsible and positive. We can assume without loss of generality that $B_{0} = 1$ . 

(i) The process $B_{i}^{-1}$ is another previsible process, just like $B_{i}$ itself. Call this the discount process. 

(ii) Define $Z_{i} := B_{i}^{-1}S_{i}$ which is just as well a defined process as S itself and it subsists on the same binomial tree. Call this the discounted stock process. 

(iii) The value $B_T^{-1}X$ is also a claim and because of the simple mapping from $Z$ to $S$ it's as much a claim on $Z$ as $S$ . Call this the discounted claim. 

What, then, now? 

## Construction strategy

Let's try out the trick. With $\mathbb{Q}$ such that $Z$ is a $\mathbb{Q}$ -martingale and claim $X$ , there is a $\mathbb{Q}$ -martingale process produced from $B_T^{-1}X$ by taking conditional expectations, $E_i = \mathbb{E}_{\mathbb{Q}}(B_T^{-1}X|\mathcal{F}_i)$ . By the binomial representation theorem, there is a previsible process $\phi$ such that 

$$
E _ {i} = E _ {0} + \sum_ {k = 1} ^ {i} \phi_ {k} \Delta Z _ {k}.
$$

Now consider the following construction strategy: at tick-time i, buy the portfolio $\Pi_{i}$ consisting of: 

- $\phi_{i+1}$ units of the stock $S$ , 

- $\psi_{i+1} = (E_i - \phi_{i+1}B_i^{-1}S_i)$ units of the cash bond. 

At time zero, our starting point, $\Pi_{0}$ is worth $\phi_{1}S_{0} + \psi_{1}B_{0} = E_{0} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X) - it$ costs that much to create. There is also no difficulty in determining $\phi_{1}$ or $\psi_{1}$ as $\phi$ and $\psi$ are previsible. 

What about one tick later? We have held the portfolio safe across the period, but its constituents have changed in value: $\Pi_{0}$ is now worth 

$$
\phi_ {1} S _ {1} + \psi_ {1} B _ {1} = B _ {1} \big (E _ {0} + \phi_ {1} (B _ {1} ^ {- 1} S _ {1} - B _ {0} ^ {- 1} S _ {0}) \big),
$$

but $B_{1}^{-1}S_{1}-B_{0}^{-1}S_{0}=\Delta Z_{1}$ . Now we can use the binomial representation theorem to simplify the expression above: at time 1, $\Pi_{0}$ is worth $B_{1}E_{1}$ . 

We are at time 1, and the construction strategy demands that we buy a new portfolio $\Pi_{1}$ . But the portfolio $\Pi_{1}$ , which we need to create at time 1, costs precisely that amount above: $B_{1}E_{1}$ , whatever actually happened to S, that is whichever filtration $F_{1}$ actually obtains. 

Thus we can cash in our portfolio $\Pi_{0}$ to create $\Pi_{1}$ . And so on. At time i, portfolio $\Pi_{i}$ costs $B_{i}E_{i}$ to purchase, and it will change by time $(i+1)$ to be 

## 2.3 Binomial representation theorem

worth $B_{i+1}E_{i+1}$ , the cost of the next portfolio. Our construction strategy is what we might call self-financing. And at the end of our self-financing strategy, we end up with the worth of $\Pi_{T-1}$ at time T, which is $B_{T}B_{T}^{-1}X$ . That is X, the claim we require. 

## Arbitrage

The price of the claim $X$ is now obvious: it is $\mathbb{E}_{\mathbb{Q}}(B_T^{-1}X)$ – the expected value of the discounted claim, under the martingale measure $\mathbb{Q}$ for the discounted stock $Z$ . And it is an arbitrage price because any other price could be milked for free money by running the $(\phi_i, \psi_i)$ strategy the appropriate way round to duplicate the claim. We shouldn't be too surprised – we are simply repeating the argument of section 2.2 in formal guise. But our formal argument has won us an overview of the entire process and a couple of vital slogans: 

## The existence of self-financing strategies

The first slogan is that within the binomial tree model, we can produce a self-financing $(\phi_{i},\psi_{i})$ strategy which duplicates any claim. What do we mean exactly by self-financing? Let us define $V_{i}$ , the worth of the trading strategy at time i, to be the opening value of the portfolio $\Pi_{i}$ at time i, that is $V_{i}=\phi_{i+1}S_{i}+\psi_{i+1}B_{i}$ . Then a strategy is self-financing if the closing value of the portfolio $\Pi_{i-1}$ at time i is precisely equal to $V_{i}$ . In symbols, the ‘financing gap’ of cash that would otherwise have to be injected into the strategy, 

$$
D _ {i} = V _ {i} - \phi_ {i} S _ {i} - \psi_ {i} B _ {i},
$$

must be zero. 

Another way of representing this self-financing property comes from the changes of the strategy value process $\Delta V_{i} = V_{i} - V_{i-1}$ , 

$$
\Delta V _ {i} = \phi_ {i} \Delta S _ {i} + \psi_ {i} \Delta B _ {i} + D _ {i}.
$$

The gap $D_{i}$ at time i is zero if and only if the change in value of the strategy from time i - 1 to i is due only to changes in the stock and bond values alone. 

Formally: 

## Self-financing hedging strategies

Given a binomial tree model of a market with a stock S and bond B, then $(\phi_{i}, \psi_{i})$ is a self-financing strategy to construct a claim X if: 

(i) both $\phi$ and $\psi$ are previsible; 

(ii) the change in value $V$ of the portfolio defined by the strategy obeys the difference equation: 

$$
\Delta V _ {i} = \phi_ {i} \Delta S _ {i} + \psi_ {i} \Delta B _ {i}
$$

where $\Delta S_{i} := S_{i} - S_{i-1}$ is the change in S from tick-time i - 1 to i, and $\Delta B_{i} := B_{i} - B_{i-1}$ is the corresponding change in B; 

(iii) and $\phi_T S_T + \psi_T B_T$ is identically equal to the claim $X$ . 

## Expectation of the discounted claim under the martingale measure

The second of these slogans is that the price of any derivative within the binomial tree model is the expectation of the discounted claim under the measure Q which makes the discounted stock a martingale. 

## Option price formula (discrete case)

The value at tick-time i of a claim X maturing at date T is 

$$
B _ {i} \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} X \mid \mathcal {F} _ {i} \big).
$$

Why? Precisely because there is a self-financing strategy, justified by the binomial representation theorem, which requires that amount to start off and yields the claim without risk at T. 

## Uniqueness and existence of $\mathbb{Q}$

And in this discrete world, we can add almost as an afterthought that for any sensible stock process S, there will be a unique measure Q under which $B_{i}^{-1}S_{i}$ , the discounted stock, is a Q-martingale. 

## 2.4 Overture to continuous models

## Conclusions

We are now finished in the discrete world, we have the general theorem we require. Any claim on a stock implies a derivative instrument tied to the underlying stock value at any time by a construction strategy capable of providing arbitrage riches if any market player disobeyed it. That arbitrage-justified value is the expectation of the discounted claim, but expectation under just one special measure, the measure Q under which the discounted stock is a martingale. The real measure P which S follows is irrelevant. The construction strategy is self-financing and generates the claim whatever S does. 

## 2.4 Overture to continuous models

We can, in a heuristic way, look into the continuous world with our discrete techniques. Without being fully rigorous yet, we could believe that a continuous model can be approximated by a discrete time model with a very small intertick time. Indeed we can show that a natural discrete model with constant growth rate and noise approximates a log-normal distribution under both the original measure P and the martingale measure Q. It will even be possible to ‘derive’ the Black–Scholes option pricing formula, though its rigorous development must wait until the very end of the next chapter. 

## Model with constant stock growth and noise

The model is parameterised by the intertick time $\delta t$ . As that quantity gets smaller, the model should ever more closely approximate a continuous-time model. There are also three fixed and constant parameters: the noisiness $\sigma$ , the stock growth rate $\mu$ , and the riskless interest rate r. 

The cash bond $B_{t}$ has the simple form that $B_{t} = \exp(rt)$ , which does not depend on the interval size. 

The stock process follows the nodes of a recombinant tree, which moves from value s at some particular node along the next up/down branch to the new value 

$$
\left\{ \begin{array}{l l} s \exp \big (\mu   \delta t + \sigma \sqrt {\delta t} \big) & \text { if } \text { up }, \\ s \exp \big (\mu   \delta t - \sigma \sqrt {\delta t} \big) & \text { if } \text { down }. \end{array} \right.
$$

The jumps are all equally likely to be up as down, that is p = 1/2 everywhere. 

For a fixed time t, if we set n to be the number of ticks till time t, then $n = t/\delta t$ and 

$$
S _ {t} = S _ {0} \exp \left(\mu t + \sigma \sqrt {t} \left(\frac {2 X _ {n} - n}{\sqrt {n}}\right)\right),
$$

where $X_{n}$ is the total number of the n separate jumps which were up-jumps. The random variable $X_{n}$ has the binomial distribution with mean n/2 and variance n/4, so that $(2X_{n}-n)/\sqrt{n}$ has mean zero and variance one. By the central limit theorem, this distribution converges to that of a normal random variable with zero mean and unit variance. So as $\delta t$ gets smaller and n gets larger, the distribution of $S_{t}$ becomes log-normal, as $\log S_{t}$ is normally distributed with mean $\log S_{0}+\mu t$ and variance $\sigma^{2}t$ . 

## Under the martingale measure

This is what happens under the original measure P, but what goes on with Q? 

Following our formula the martingale measure probability q is 

$$
q = \frac {s \exp (r \delta t) - s _ {\mathrm{down}}}{s _ {\mathrm{up}} - s _ {\mathrm{down}}}.
$$

We can calculate that q is approximately equal to 

$$
q = \frac {1}{2} \left(1 - \sqrt {\delta t} \left(\frac {\mu + \frac {1}{2} \sigma^ {2} - r}{\sigma}\right)\right).
$$

So, under Q, $X_{n}$ is still binomially distributed, but now has mean nq and variance $nq(1-q)$ . 

Thus $(2X_{n}-n)/\sqrt{n}$ has mean $-\sqrt{t}(\mu+\frac{1}{2}\sigma^{2}-r)/\sigma$ and variance asymptotically approaching one. Again the central limit theorem gives the convergence of this to a normal random variable with the same mean and variance exactly one. The corresponding $S_{t}$ is still log-normally distributed with $\log S_{t}$ having mean $\log S_{0}+(r-\frac{1}{2}\sigma^{2})t$ and variance $\sigma^{2}t$ . This can be written 

$$
S _ {t} = S _ {0} \exp \left(\sigma \sqrt {t} Z + (r - \frac {1}{2} \sigma^ {2}) t\right),
$$

where Z is a normal $N(0,1)$ under Q. We have found the marginal distribution of $S_{t}$ under the martingale measure Q. 

## 2.4 Overture to continuous models

## Pricing a call option

If X is the call option maturing at date T, struck at k, with $X = (S_{T} - k)^{+}$ , then its worth at time zero is 

$$
\mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X\right) = \mathbb {E} _ {\mathbb {Q}} \left[ \left(S _ {0} \exp \left(\sigma \sqrt {T} Z - \frac {1}{2} \sigma^ {2} T\right) - k \exp (- r T)\right) ^ {+} \right].
$$

We will see in chapter three that this evaluates as 

$$
S _ {0} \Phi \left(\frac {\log \frac {S _ {0}}{k} + (r + \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}}\right) - k e ^ {- r T} \Phi \left(\frac {\log \frac {S _ {0}}{k} + (r - \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}}\right),
$$

where $\Phi$ is the normal distribution function $\Phi(x) = \mathbb{Q}(Z \leqslant x)$ . This is a preview of the Black–Scholes formula which we shall prove properly in the next chapter. 

# Chapter 3 Continuous processes

Stock prices are not trees. The discrete trees of the previous chapter are only an approximation to the way that prices actually move. In practice, a price can change at any instant, rather than just at some fixed tick-times when a portfolio can be calmly rebalanced. The binary choice of a single jump ‘up’ or ‘down’ only becomes subtle as the ticks get closer and closer, giving the tree more and ever-shorter branches. But such trees grow too complex and we stop being able to see the wood. 

We shall have to start from scratch in the continuous world. The discrete models will guide us – the intuitions gained there will be more than useful – but limiting arguments based on letting $\delta t$ tend to zero are too dangerous to be used rigorously. We will encounter a representation theorem which establishes the basis of risk-free construction and again it will be martingale measures that prime the expectation operator correctly. But processes and measures will be harder to separate intuitively – we will need a calculus to help us. And changes in measure will affect processes in surprising ways. We will no longer be able to proceed in full generality – we will concentrate on Brownian motion and its relatives. If there is one overarching principle to this chapter it is that Brownian motion is sophisticated enough to produce interesting models and simple enough to be tractable. Given the subtleties of working with continuous processes, a simple calculus based on Brownian motion will be more than enough for us. 

## 3.1 Continuous processes

## 3.1 Continuous processes

We want randomness. With our discrete stock price model we didn't have any old random process. We forcibly limited ourselves to a binomial tree. We started simply and hoped (with some justification) that complex enough market models could be built from such humble materials. The single binomial branching was the building block for our ‘realistic’ market. For the continuous world we need an analogous basis – something simple and yet a reasonable starting point for realism. 

What is a continuous process? Three small-scale principles guide us. Firstly, the value can change at any time and from moment to moment. Secondly, the actual values taken can be expressed in arbitrarily fine fractions – any real number can be taken as a value. And lastly the process changes continuously – the value cannot make instantaneous jumps. In other words, if the value changes from 1 to 1.05 it must have passed through, albeit quickly, all the values in between. 

At least as a starting point, we can insist that stock market indices or prices of individual securities behave this way. Even though they move in a ‘sharp-edged’ way, it isn’t too unrealistic to claim that they nonetheless display continuous process behaviour. 

And as far back as Bachelier in 1900, who analysed the motion of the Paris stock exchange, people have gone further and compared the prices to one particular continuous process – the process followed by a randomly moving gas particle, or Brownian motion (figure 3.2). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/04ad7f51d17eaa74173f6737bb1d3fc998a7780addf32178d15616bc802fc429.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/13327a097645c6495402c17e5d22be4337548af178a54882ecea3f9f74615933.jpg)



Figure 3.1 UK FTA index, 1963–92 Figure 3.2 Brownian motion


Locally the likeness can be striking – both display the same jaggedness, and the same similarity under scale changes – the jaggedness never smooths out as the magnification increases. But globally, the similarity fades – figure 3.1 doesn't look like figure 3.2. At an intuitive level, the global structure of the stock index is different. It grows, gets ‘noisier’ as time passes, and doesn’t go negative. Brownian motion can’t be the whole story. 

But we only want a basis – the single binomial branching didn't look promising right away. We shouldn't run ahead of ourselves. Brownian motion will prove a remarkably effective component to build continuous processes with – locally Brownian motion looks realistic. 

## Brownian motion

It was nearly a century after botanist Robert Brown first observed microscopic particles zigzagging under the continuous buffeting of a gas that the mathematical model for their movements was properly developed. The first step to the analysis of Brownian motion is to construct a special family of discrete binomial processes. 

The random walk $W_{n}(t)$ For $n$ a positive integer, define the binomial process $W_{n}(t)$ to have:
(i) $W_{n}(0) = 0$ ,
(ii) layer spacing $1/n$ ,
(iii) up and down jumps equal and of size $1/\sqrt{n}$ ,
(iv) measure $\mathbb{P}$ , given by up and down probabilities everywhere equal to $\frac{1}{2}$ . 

In other words, if $X_{1}, X_{2}, \ldots$ is a sequence of independent binomial random variables taking values +1 or -1 with equal probability, then the value of $W_{n}$ at the ith step is defined by: 

$$
W _ {n} \left(\frac {i}{n}\right) = W _ {n} \left(\frac {i - 1}{n}\right) + \frac {X _ {i}}{\sqrt {n}}, \quad \text {   for   all   } i \geqslant 1.
$$

The first two steps are shown in figure 3.3. What does $W_{n}$ look like as $n$ gets large? 

Instead of blowing out of control, the family portraits (figure 3.4) appear to be settling down towards something as n increases. The moves of size 

## 3.1 Continuous processes

$1/\sqrt{n}$ seem to force some kind of convergence. Can we make a formal statement? Consider for example, the distribution of $W_{n}$ at time 1: for a particular $W_{n}$ , there are $n+1$ possible values that it can take, ranging from $-\sqrt{n}$ to $\sqrt{n}$ . But the distribution always has zero mean and unit variance. (Because $W_{n}(1)$ is the sum of n IID random variables, each with zero mean and variance $1/n$ .) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/2abf9e03bdf230b50423781ad5db78a12e4e50a2a0571c5dc23230789c9d3ae8.jpg)



Figure 3.3 The first two steps of the random walk $W_{n}$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/55fa686928864cc1d1aa8ce03283e1ee6384a6e529e728ea7f7de825bb590809.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/45c0029e748ec4b504c459606efb00c0b1319613f55a3f17cd8d84fd5d368f3f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/728d7cf786f39bc89aca21d07c1239de7f91d452baa727fa9a63ed6fdd5f6690.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/c6b7580ca943817fc3c16272a9bd9f46e428a42083d2d01b41d448c332f478d2.jpg)



Figure 3.4 Random walks of 16, 64, 256 and 1024 steps respectively


Moreover the central limit theorem gives us a limit for these binomial distributions - as $n$ gets large, the distribution of $W_{n}(1)$ tends towards the unit normal $N(0,1)$ . In fact, the value of $W_{n}(t)$ is the same as 

$$
W _ {n} (t) = \sqrt {t} \left(\frac {\sum_ {i = 1} ^ {n t} X _ {i}}{\sqrt {n t}}\right).
$$

The distribution of the ratio in brackets tends, by the central limit theorem, to a normal $N(0,1)$ random variable. And so the distribution of $W_{n}(t)$ tends to a normal $N(0,t)$ . 

There is a formal unity underlying the family - all the marginal distributions tend towards the same underlying normal structure. 

And not just all the marginal distributions, but all the conditional marginal distributions as well. Each random walk $W_{n}$ has the property that its future movements away from a particular position are independent of where that position is (and indeed independent of its entire history of movements up to that time). Additionally such a future displacement $W_{n}(s+t)-W_{n}(s)$ is binomially distributed with zero mean and variance t. Thus again, the central limit theorem gives us a constant limiting structure, and all conditional marginals tend towards a normal distribution of the same mean and variance. 

The marginals converge, the conditional marginals converge, and the temptation is irresistible to say that the distributions of the processes converge too. And indeed they do, though this isn't the place to set up the careful formal framework to make sense of that statement. The distribution of $W_{n}$ converges, and it converges towards Brownian motion. 

Formally: 

## Brownian motion

The process $W = (W_{t}: t \geqslant 0)$ is a $\mathbb{P}$ -Brownian motion if and only if 

(i) $W_{t}$ is continuous, and $W_0 = 0$ , 

(ii) the value of $W_{t}$ is distributed, under $\mathbb{P}$ , as a normal random variable $N(0,t)$ , 

(iii) the increment $W_{s + t} - W_s$ is distributed as a normal $N(0,t)$ , under $\mathbb{P}$ , and is independent of $\mathcal{F}_s$ , the history of what the process did up to time $s$ . 

## 3.1 Continuous processes

These are both necessary and sufficient conditions for the process W to be Brownian motion. The last condition, though an exact echo of the behaviour of the discrete precursors $W_{n}(t)$ , is subtle. Many processes that have marginals $N(0,t)$ are not Brownian motion. In the continuous world, just as it was in the discrete, it is not just the marginals (conditional on the process' value at time zero) that count, but all the marginals conditional on all the histories $F_{s}$ . It will in fact be the daunting task of specifying all these that drives us to a Brownian calculus. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/1fee98c01c753dab4fec2629bdf8194ad89d9c0b1efbeacec718de2380c42949.jpg)


Exercise 3.1 If Z is a normal $N(0,1)$ , then the process $X_{t} = \sqrt{t}Z$ is continuous and is marginally distributed as a normal $N(0,t)$ . Is X a Brownian motion? 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/7883a6944d236205d7eef1e377215efcb512648bd4423829a4e6eac4e5d25aff.jpg)


Exercise 3.2 If $W_{t}$ and $\tilde{W}_{t}$ are two independent Brownian motions and $\rho$ is a constant between -1 and 1, then the process $X_{t} = \rho W_{t} + \sqrt{1 - \rho^{2}} \tilde{W}_{t}$ is continuous and has marginal distributions $N(0, t)$ . Is this X a Brownian motion? 

It is also worth noting just how odd Brownian motion really is. We won't stop to prove them, but here is a brief peek into the bestiary: 

- Although $W$ is continuous everywhere, it is (with probability one) differentiable nowhere. 

- Brownian motion will eventually hit any and every real value no matter how large, or how negative. It may be a million units above the axis, but it will (with probability one) be back down again to zero, by some later time. 

- Once Brownian motion hits a value, it immediately hits it again infinitely often, and then again from time to time in the future. 

- It doesn't matter what scale you examine Brownian motion on – it looks just the same. Brownian motion is a fractal. 

Brownian motion is often also called a Wiener process, and is a (one-dimensional) Gaussian process. 

## Brownian motion as stock model

We had our misgivings about Brownian motion as a global model for stock behaviour, but we don't have to use it on its own. Brownian motion wanders. It has mean zero, whereas the stock of a company normally grows at some rate – and historically we expect prices to rise if only because of inflation. But we can add in a drift artificially. For example the process $S_{t} = W_{t} + \mu t$ , for some constant $\mu$ reflecting nominal growth, is called Brownian motion with drift. 

And if it looks too noisy, or not noisy enough, we can scale the Brownian motion by some factor: for example, $S_{t} = \sigma W_{t} + \mu t$ , for a constant noise factor $\sigma$ . 

How are we doing? Consider the stock market data shown in figure 3.1. We could estimate $\sigma$ and $\mu$ for the best fit [in this case, $\sigma = 91.3$ and $\mu = 37.8$ ] and simulate a sample path. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/dc1eb0ddba0644e2764317155e22f9bb72450085b7b36a1718eedc74de8352fe.jpg)



Figure 3.5 Brownian motion plus drift


Not bad – the process has long-term upwards growth, as we want. But in this particular case, we have a glitch right away. The process went negative, which we may not want for the price of a stock of a limited liability company. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/d4fd343a98824040239c91f887630c19ce59c7c482a65ad352b72ae7dfa25e80.jpg)


Exercise 3.3 Show that, for all values of $\sigma$ ( $\sigma \neq 0$ ), $\mu$ , and $T > 0$ there is always a positive probability that $S_T$ is negative. (Hint: consider the marginal distribution of $S_T$ .) 

## 3.2 Stochastic calculus

We can though be more adventurous in shaping Brownian motion to our ends. Consider for example, taking the exponential of our process: 

$$
X _ {t} = \exp (\sigma W _ {t} + \mu t).
$$

Now we mirror the stock market's long-term exponential growth (and for good measure we start off quietly and get noisier). Again finding a best fit for $\sigma$ and $\mu$ [ $\sigma = 0.178$ and $\mu = 0.087$ , a 'noisiness' of $17.8\%$ and an annual drift of $8.7\%$ ] we can simulate a sample path (figure 3.6). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/3cc408256efe4fa630521b7d8c29a7ed93b0426df138928a3ea3ab510e0e4b2e.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/70a35c84b41bca1a746e4a38fb2908c7478970e99e3c228b35ff8587ec801d98.jpg)



This process is, not surprisingly, well known and it is usually called exponential Brownian motion with drift, or sometimes geometric Brownian motion with drift. It is not the only model for stocks – and indeed we will look at others later on – but it is simple and not that bad. (Could you tell which picture was which without the captions?) Brownian motion can prove an effective building block.


## 3.2 Stochastic calculus

Shaping Brownian motion with functions may be powerful, but it brings a dangerous complexity. Consider any smooth (differentiable) curve. Globally it can have almost any behaviour it likes, because the condition that it is differentiable does nothing to affect it at a large scale. Suppose we zoom in though, pinning down a small section under a microscope. In figure 3.7, we focus in on the point of a particular differentiable curve with x-co-ordinate of 1.7, increasing the magnification by a factor of about ten each time. 

Reading the graphs from left to right and line by line, each small box is expanded to form the frame for the next graph. As the process continues, the graph section becomes smoother and straighter, until eventually it is straight – it is a small straight line. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/e9ae9cb70c56a9b3655be9305bdb0860b93819fd9d20fe1aadb25c41e83a130c.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/c6fa7c9bbad4c465d201eff1b1fcd3a7ee9ec3ed900dc15eb10a71bf6af899be.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/462fd73e3d24054e239721f3a179871dfef14dd0b565e8c8858b82c593d9695a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/8e387f38a92e5b28e833be10914ef615ee93aa38e8524ce843642e19c8bebaf0.jpg)



Figure 3.7 Progressive magnification around the point 1.7


Differentiable functions, however strange their global behaviour, are at heart built from straight line segments. Newtonian calculus is the formal acknowledgement of this. 

With a Newtonian construction, we could decide to build up a family of nice functions by specifying how they are locally built up out of our building block, the straight line. We would write the change in value of a Newtonian function f over a time interval at t of infinitesimal length dt as 

$$
d f _ {t} = \mu_ {t} d t,
$$

where $\mu_{t}$ is our scaling function, the slope or drift of the magnified straight line at t. 

Then we could explore our universe of Newtonian functions. Consider, for example: 

(1) The equation $df_{t} = \mu dt$ , for some constant $\mu$ . What is $f$ ? That is, what does it look like? How does it behave globally? Could we draw it? If 

## 3.2 Stochastic calculus

we stick together straight line segments of slope $\mu$ , then intuitively we just produce a straight line of slope $\mu$ . If $f_{0}$ , for example, was equal to zero then we might guess (correctly) that $f_{t}$ could be written in more familiar notation as $f_{t} = \mu t$ . 

(2) The equation $df_{t} = t \, dt$ . Here we have a slope at time $t$ of value $t -$ what does this look like? Simple integration comes to the rescue. If $f_{0} = 0$ , then we could again pin down $f_{t}$ as $f_{t} = \frac{1}{2} t^{2}$ . The going was a bit harder here, but we managed it, and we can check it ourselves by differentiation: $f_{t}' = t$ as we require. 

What about uniqueness though? In the first example, our intuition dismissed the possibility of another solution, but what about here? The construction metaphor $(df_{t} = t dt$ tells us how to build $f_{t}$ , and thus given a starting place and a deterministic building plan we ought to produce just one possible $f_{t}$ suggests that $f_{t} = \frac{1}{2} t^{2}$ is the unique solution and indeed we can formalise this. 

## Uniqueness of Newtonian differentials

Two complementary forms of uniqueness operate here. 

- If $f_{t}$ and $\tilde{f}_{t}$ are two differentiable functions agreeing at 0 ( $f_{0} = \tilde{f}_{0}$ ) and they have identical drifts ( $df_{t} = d\tilde{f}_{t}$ ), then the processes are equal: $f_{t} = \tilde{f}_{t}$ for all $t$ . In other words, $f$ is unique given the drift $\mu_{t}$ (and $f_{0}$ ). 

- Secondly, given a differentiable function $f_{t}$ , there is only one drift function $\mu_{t}$ which satisfies $f_{t} = f_{0} + \int_{0}^{t} \mu_{s} ds$ (for all $t$ ). So $\mu$ is unique given $f$ . 

Instead of just giving the drift $\mu_{t}$ directly, we might have a problem where the drift itself depends on the current value of the function. Specifically, if the drift $\mu_{t}$ equals $\mu(f_{t}, t)$ , where $\mu(x, t)$ is a known function, then 

$$
d f _ {t} = \mu (f _ {t}, t) d t
$$

is called an ordinary differential equation (ODE). If there is a differentiable function f which satisfies it (with given $f_{0}$ ), it forms a solution. There are plenty of ODEs which have no solutions, and plenty more which do not have unique solutions. (The uniqueness of the solution to an ODE cannot be deduced just from the uniqueness of Newtonian differentials in the box.) 

(3) The equation $df_{t} = f_{t} dt$ . Now things are harder, as direct integration is not a route to the solution. We could guess - say $f_{t} = e^{t} -$ and then check by differentiation. This solution happens to be unique for $f_{0} = 1$ . 

(4) The equation $df_{t} = f_{t}t^{-2}dt$ . This is an example of a bad case, where solutions need neither exist nor be unique. Given $f_{0} = 0$ , there are an infinite number of solutions, namely $f_{t} = a\exp (-1 / t)$ for every possible value of an arbitrary constant $a$ . However, for $f_{0}\neq 0$ , there are no solutions at all. 

Perhaps our universe of Newtonian functions isn't so benign. It is clear that though ODEs are powerful construction tools, they are also dangerous ones. There are plenty of 'bad' ODEs which we haven't a clue how to explore. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/c9e38c681acbd6cf7b9b45a92f80ba12c43512fa6f6d12381ddb1735aaefb758.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/294b8c413be20b57fa6ccd5341e4a6411fc284febdeab9ac53a46d245f3d09f6.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/f279c27d714e7fcd981d0f3e42acd15f6ceb1e1328311b773c5050da37e24e32.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/f3112c8d5228066538f64d8627297b7f954bd5d1cb7108413ed8905f77c78d36.jpg)



Figure 3.8 ‘Zooming in’ on Brownian motion


## Stochastic differentials

And if it was bad for Newtonian differentials, consider a construction procedure based on Brownian motion. Zooming in on Brownian motion doesn't produce a straight line (figure 3.8) 

As before, each box is expanded by suitable horizontal and vertical scaling to frame the next graph. The self-similarity of Brownian motion means that 

## 3.2 Stochastic calculus

each new graph is also a Brownian motion, and just as noisy. 

But of course this self-similarity is ideal for a building block – we could build global Brownian motion out of lots of local Brownian motion segments. And we could build general random processes from small segments of Brownian motion (suitably scaled). If we built using straight line segments (suitably scaled) too, we could include Newtonian functions as well. 

A stochastic process X will have both a Newtonian term based on dt and a Brownian term, based on the infinitesimal increment of W which we will call $dW_{t}$ . The Brownian term of X can have a noise factor $\sigma_{t}$ , and so the infinitesimal change of $X_{t}$ is 

$$
d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t.
$$

As in the Newtonian case, the drift $\mu_{t}$ can depend on the time t. But it can also be random and depend on values that X (or indeed W) took up until t itself. And of course, so can the noisiness $\sigma_{t}$ . Such processes, like X and $\sigma$ , whose value at time t can depend on the history $F_{t}$ , but not the future, are called adapted to the filtration F of the Brownian motion W. 

We call $\sigma_{t}$ the volatility of the process X at time t and $\mu_{t}$ the drift of X at t. 

## Stochastic processes

What does our universe look like? As with Newtonian differentials, finding this out entails ‘integrating’ stochastic differentials in some way. We can, though, formally define what it is to be a (continuous) stochastic process. 

This definition of stochastic process (see box) is not universal, and in particular it excludes discontinuous cases such as Poisson processes. Nevertheless it will be quite adequate for all the models we will meet. 

The technical condition that $\sigma$ and $\mu$ must be F-previsible processes means that they are adapted to the filtration F, and that they may have some jump discontinuities. In terms of stochastic analysis, this defines stochastic processes to be semimartingales whose drift term is absolutely continuous. This class is closed under all the operations used later, and all the models considered will lie within it. 

And as it happens, we can provide a uniqueness result to mirror the classical setup. 

## Stochastic processes

A stochastic process X is a continuous process $(X_{t}: t \geqslant 0)$ such that $X_{t}$ can be written as 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \sigma_ {s} d W _ {s} + \int_ {0} ^ {t} \mu_ {s} d s,
$$

where $\sigma$ and $\mu$ are random F-previsible processes such that $\int_{0}^{t}(\sigma_{s}^{2}+|\mu_{s}|)ds$ is finite for all times t (with probability 1). The differential form of this equation can be written 

$$
d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t.
$$

## Uniqueness of volatility and drift

Two complementary forms of uniqueness operate here. 

- Firstly, if two processes $X_{t}$ and $\tilde{X}_{t}$ agree at time zero ( $X_{0} = \tilde{X}_{0}$ ) and they have identical volatility $\sigma_{t}$ and drift $\mu_{t}$ , then the processes are equal: $X_{t} = \tilde{X}_{t}$ for all $t$ . In other words, $X$ is unique given $\sigma_{t}$ and $\mu_{t}$ (and $X_{0}$ ). 

- Secondly, given the process $X$ , there is only one pair of volatility $\sigma_t$ and drift $\mu_t$ which satisfies $X_t = X_0 + \int_0^t \sigma_s dW_s + \int_0^t \mu_s ds$ (for all $t$ ). This uniqueness of $\sigma_t$ and $\mu_t$ given $X$ comes from the Doob-Meyer decomposition of semimartingales. 

In the special case when $\sigma$ and $\mu$ depend on W only through $X_{t}$ , such as $\sigma_{t} = \sigma(X_{t}, t)$ , where $\sigma(x, t)$ is some deterministic function, the equation 

$$
d X _ {t} = \sigma (X _ {t}, t) d W _ {t} + \mu (X _ {t}, t) d t
$$

is called a stochastic differential equation (SDE) for X. And it will generally be easier to write down the SDE (if it exists) for a particular X then it is to provide an explicit solution for the SDE. As in the Newtonian case (ODEs), an SDE need not have a solution, and if it does it might not be unique. Usage of the term SDE does tend to spread out from this strict definition to include the stochastic differentials of processes whose volatility and drift depends not only on $X_{t}$ and t, but also on other events in the history $F_{t}$ . 

## 3.3 Itô calculus

But can we recognise the world we have created, perhaps in terms of $W_{t}$ , the Brownian motion we have some handle on? 

Partially. In the simple case, where $\sigma$ and $\mu$ are both constants, meaning that X has constant volatility and drift, the SDE for X is 

$$
d X _ {t} = \sigma d W _ {t} + \mu d t.
$$

It isn't too hard to guess what the solution to this is: 

$$
X _ {t} = \sigma W _ {t} + \mu t,
$$

(assuming that $X_{0} = 0$ ). And our meagre understanding of $W_{t}$ and $dW_{t}$ at least gives us some confidence that the differential form of $\sigma W_{t}$ is $\sigma dW_{t}$ . As $\sigma$ and $\mu$ are independent of X, the uniqueness result could form a part of a proof that this is the only solution. 

But consider the only slightly more complex SDE (echoing the Newtonian ODE of example (3) above), 

$$
d X _ {t} = X _ {t} \left(\sigma d W _ {t} + \mu d t\right).
$$

We're at sea. 

## 3.3 Itô calculus

Intuitive integration doesn't carry us very far. We need tools to manipulate the differential equations, just as Newtonian calculus has the chain rule, product rule, integration by parts, and so on. 

How far could Newton carry us? Suppose we had some function $f$ of Brownian motion, say $f(W_t) = W_t^2$ . Could we use a simple chain rule to produce the stochastic differential $df_t$ ? Under Newtonian rules, $d(W_t^2)$ would be $2W_t dW_t$ , which doesn't look too implausible. But we should check via integration, because 

$$
\mathrm{if} \quad \int_ {0} ^ {t} d (W _ {s} ^ {2}) = 2 \int_ {0} ^ {t} W _ {s} d W _ {s}, \quad \mathrm{then} \quad W _ {t} ^ {2} = 2 \int_ {0} ^ {t} W _ {s} d W _ {s}.
$$

How can we tackle $\int_{0}^{t} W_{s} dW_{s}$ ? Consider dividing up the time interval $[0, t]$ into a partition $\{0, t/n, 2t/n, \ldots, (n-1)t/n, t\}$ for some n. Then we could approximate the integral with a summation over this partition, that is 

$$
2 \int_ {0} ^ {t} W _ {s} d W _ {s} \approx 2 \sum_ {i = 0} ^ {n - 1} W \left(\frac {i t}{n}\right) \left(W \left(\frac {(i + 1) t}{n}\right) - W \left(\frac {i t}{n}\right)\right).
$$

Now something begins to worry us. The difference term inside the brackets is just the increment of Brownian motion from one particular partition point to the next. By property (iii) of Brownian motion, that increment is independent of the Brownian motion up to that point, and in particular it is independent of the Brownian motion term $W(it/n)$ . Also the increment has zero mean, which means that so too must the product of the increment and $W(it/n)$ . So the summation consists of terms with zero mean, forcing it to have zero mean itself. 

But $W_{t}^{2}$ has mean $t$ , because of the variance structure of Brownian motion, so $2W_{t}dW_{t}$ cannot be the differential of $W_{t}^{2}$ , because its integral doesn't even have the right expectation. 

What went wrong? Consider a Taylor expansion of $f(W_{t})$ for some smooth f: 

$$
d f (W _ {t}) = f ^ {\prime} (W _ {t}) d W _ {t} + \frac {1}{2} f ^ {\prime \prime} (W _ {t}) (d W _ {t}) ^ {2} + \frac {1}{3 !} f ^ {\prime \prime \prime} (W _ {t}) (d W _ {t}) ^ {3} + \dots
$$

Over-familiar with Newtonian differentials, we assumed that $(dW_{t})^{2}$ and higher terms were zero. But as we have observed before, Brownian motion is odd. Take $(dW_{t})^{2}$ , given the same partitioning of $[0,t]$ we just used: $\{0,t/n,2t/n,\ldots,t\}$ . We can model the integral of $(dW_{t})^{2}$ by the (hopefully convergent) approximation 

$$
\int_ {0} ^ {t} \left(d W _ {t}\right) ^ {2} = \sum_ {i = 1} ^ {n} \left(W \left(\frac {t i}{n}\right) - W \left(\frac {t (i - 1)}{n}\right)\right) ^ {2}.
$$

But if we let $Z_{n,i}$ be 

$$
Z _ {n, i} = \frac {W \left(\frac {t i}{n}\right) - W \left(\frac {t (i - 1)}{n}\right)}{\sqrt {t / n}},
$$

then for each n, the sequence $Z_{n,1}, Z_{n,2}, \ldots$ is a set of IID normals $N(0,1)$ . (Because each increment $W\left(\frac{ti}{n}\right) - W\left(\frac{t(i-1)}{n}\right)$ is a normal $N(0, t/n)$ , independent of the ones before it, by Brownian motion fact (iii).) 

## 3.3 Itô calculus

We can rewrite our approximation for $\int(dW_{s})^{2}$ as 

$$
\int_ {0} ^ {t} (d W _ {s}) ^ {2} \approx t \sum_ {i = 1} ^ {n} \frac {Z _ {n , i} ^ {2}}{n}.
$$

By the weak law of large numbers (just like the strong law but only talking about the distribution of random variables), the distribution of the right-hand side summation converges towards the constant expectation of each $Z_{n,i}^{2}$ , namely 1. Thus $\int_{0}^{t}(dW_{s})^{2}=t$ , or in differential form $(dW_{t})^{2}=dt$ . 

We can't ignore $(dW_{t})^{2}$ ; it only looks second order because of the notation. What about $(dW_{t})^{3}$ and so on? It turns out that they are zero. (For example, $\mathbb{E}(|dW_{t}|^{3})$ has size $(dt)^{3/2}$ , which is negligible compared with $dt$ .) So Taylor gives us: 

$$
d f (W _ {t}) = f ^ {\prime} (W _ {t}) d W _ {t} + \frac {1}{2} f ^ {\prime \prime} (W _ {t}) d t + 0.
$$

The formal version of this surprising departure from Newtonian differentials is the deservedly famous Itô's formula (sometimes seen modestly as Itô's lemma). 

## Itô's formula

If X is a stochastic process, satisfying $dX_{t} = \sigma_{t} dW_{t} + \mu_{t} dt$ , and f is a deterministic twice continuously differentiable function, then $Y_{t} := f(X_{t})$ is also a stochastic process and is given by 

$$
d Y _ {t} = \left(\sigma_ {t} f ^ {\prime} (X _ {t})\right) d W _ {t} + \left(\mu_ {t} f ^ {\prime} (X _ {t}) + \frac {1}{2} \sigma_ {t} ^ {2} f ^ {\prime \prime} (X _ {t})\right) d t.
$$

Returning to our $W_{t}^{2}$ , we can apply Itô with $X = W$ and $f(x) = x^{2}$ and we have 

$$
d (W _ {t} ^ {2}) = 2 W _ {t} d W _ {t} + d t, \quad \mathrm{or} \quad W _ {t} ^ {2} = 2 \int_ {0} ^ {t} W _ {s} d W _ {s} + t,
$$

which at least has the right expectation. 

More generally, if X is still just the Brownian motion W, then $f(X)$ has differential 

$$
d f (W _ {t}) = f ^ {\prime} (W _ {t}) d W _ {t} + \frac {1}{2} f ^ {\prime \prime} (W _ {t}) d t,
$$

as hinted above. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/82d5cf97473978f98a400002f41aa389ad71f4e30951977207003eceb917a19d.jpg)


Exercise 3.4 If $X_{t} = \exp (W_{t})$ , then what is $dX_{t}$ ? 

## SDEs from processes

Itô's most immediate use is to generate SDEs from a functional expression for a process. Consider the exponential Brownian motion we set up in section 3.1: 

$$
X _ {t} = \exp (\sigma W _ {t} + \mu t).
$$

What SDE does X follow? We know we can handle the term inside the brackets but we have to take a stochastic differential of the exponential function as well. With the right formulation though, we can use Itô's formula. 

Suppose we took $Y_{t}$ to be the process $\sigma W_{t} + \mu t$ , and $f$ to be the exponential function $f(x) = e^{x}$ . Then $Y_{t}$ is simple enough that we can write down its differential immediately: $dY_{t} = \sigma dW_{t} + \mu dt$ . But of course the $X_{t}$ we want can be written as $X_{t} = f(Y_{t})$ , so one application of Itô's formula gives us 

$$
d X _ {t} = \sigma f ^ {\prime} (Y _ {t}) d W _ {t} + \left(\mu f ^ {\prime} (Y _ {t}) + \frac {1}{2} \sigma^ {2} f ^ {\prime \prime} (Y _ {t})\right) d t.
$$

The exponential function is particularly pleasant, as $f'(Y_t) = f''(Y_t) = f(Y_t) = X_t$ , so we can rewrite the differential as 

$$
d X _ {t} = X _ {t} \big (\sigma d W _ {t} + (\mu + \frac {1}{2} \sigma^ {2}) d t \big).
$$

Here, the variable $\sigma$ is sometimes called the log-volatility of the process, because it is the volatility of the process $\log X_{t}$ , and which is often abbreviated just to volatility notwithstanding that term's existing definition. We will also use the name log-drift for the drift $\mu$ of $\log X_{t}$ , which is different from the drift of $dX_{t}/X_{t}$ above. 

## Processes from SDEs

Much like differentiation (easy, but its inverse can be impossible), using Itô to convert processes to SDEs is relatively straightforward. And if that were all we ever wanted to do there would be few problems. But it isn't – one of the key needs we have is to go in the opposite direction and convert SDEs to processes. Or in other words, to solve them. 

In general we can't. Most stochastic differential equations are just too difficult to solve. But a few, rare examples can be, and just like some ODEs they depend on an inspired guess and then a proof that the proposed solution is an actual solution via Itô. Such a solution to an SDE is called a diffusion. 

Suppose we are asked to solve the SDE 

$$
d X _ {t} = \sigma X _ {t} d W _ {t}.
$$

We need an inspired guess - so we notice that the stochastic term $(\sigma X_{t}dW_{t})$ from this SDE is the same as the SDE we generated via Itô in the section above. Moreover, if we choose $\mu$ to be $-\frac{1}{2}\sigma^2$ , then the drift term in the SDE would match our SDE as well. We guess then that 

$$
X _ {t} = \exp (\sigma W _ {t} - \frac {1}{2} \sigma^ {2} t).
$$

What does Itô tell us? That $dX_{t}$ is indeed $\sigma X_{t} dW_{t}$ , which is what we wanted. So we have found one solution, and as it turns out, the only solution (up to constant multiples). Soluble SDEs are scarce, and this one is special enough to have a name: the Doléans exponential of Brownian motion. 

Let's go back then to the SDE we tripped over earlier: 

$$
d X _ {t} = X _ {t} \left(\sigma d W _ {t} + \mu d t\right).
$$

We could match both drift and volatility terms for this SDE and the SDE of $\exp(\sigma W_{t} + \nu t)$ if and only if we take $\nu$ to be $\mu - \frac{1}{2}\sigma^{2}$ . So that is our guess, that 

$$
X _ {t} = \exp \left(\sigma W _ {t} + \left(\mu - \frac {1}{2} \sigma^ {2}\right) t\right).
$$

And again Itô confirms our intuition. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/3b9a1f9f1d7345d06899f49f745d0852ef6b2e610d1381034cb86a0e4c99102b.jpg)


Exercise 3.5 What is the solution of $dX_{t}=X_{t}(\sigma dW_{t}+\mu_{t}dt)$ , for $\mu_{t}$ a general bounded integrable function of time? 

## The product rule

Another Newtonian law was the product rule, that $d(f_{t}g_{t}) = f_{t} dg_{t} + g_{t} df_{t}$ . In the stochastic world, there are two (seemingly) separate cases. 

In the more significant case, $X_{t}$ and $Y_{t}$ are adapted to the same Brownian motion W, in that 

$$
\begin{array}{r} d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t, \\ d Y _ {t} = \rho_ {t} d W _ {t} + \nu_ {t} d t. \end{array}
$$

By applying Itô's formula to $\frac{1}{2}\left((X_{t} + Y_{t})^{2} - X_{t}^{2} - Y_{t}^{2}\right) = X_{t}Y_{t}$ , we can see that 

$$
d (X _ {t} Y _ {t}) = X _ {t} d Y _ {t} + Y _ {t} d X _ {t} + \sigma_ {t} \rho_ {t} d t.
$$

The final term above is actually $dX_{t}dY_{t}$ (following from $(dW_{t})^{2}=dt$ ) and again marks the difference between Newtonian and Itô calculus. 

In the other case, $X_{t}$ and $Y_{t}$ are two stochastic processes adapted to two different and independent Brownian motions, such as 

$$
\begin{array}{r} d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t, \\ d Y _ {t} = \rho_ {t} d \tilde {W} _ {t} + \nu_ {t} d t, \end{array}
$$

where $\sigma_{t}$ and $\rho_{t}$ are the respective volatilities of X and Y, $\mu_{t}$ and $\nu_{t}$ are their drifts, and W and $\tilde{W}$ are two independent Brownian motions. Here 

$$
d (X _ {t} Y _ {t}) = X _ {t} d Y _ {t} + Y _ {t} d X _ {t},
$$

just as in the Newtonian case. 

At a deeper level these two stochastic cases can be reconciled by viewing $X_{t}$ and $Y_{t}$ as both adapted to the two-dimensional Brownian motion ( $W_{t}, \tilde{W}_{t}$ ), as will be explained in section 6.3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/b3ec2c7241ab970ec2702b8e11b1efdd330914a10790838ed8837d02ec4c81d9.jpg)


Exercise 3.6 Show that if $B_{t}$ is a zero-volatility process and $X_{t}$ is any stochastic process, then 

$$
d (B _ {t} X _ {t}) = B _ {t} d X _ {t} + X _ {t} d B _ {t}.
$$

## 3.4 Change of measure - the C-M-G theorem

## 3.4 Change of measure - the C-M-G theorem

Something remains hidden from us. One of the central themes of the previous chapter was the importance of separating process and measure. Yet we don't seem to mention measures in our stochastic differentials. We may have our basic tools for manipulating stochastic processes, but they are a manipulation of differentials of Brownian motion, not a manipulation of measure. We haven't actually ignored the importance of measure $-W_{t}$ is not strictly a Brownian motion per se, but a Brownian motion with respect to some measure $\mathbb{P}$ , a $\mathbb{P}$ -Brownian motion. And thus our stochastic differential formulation describes the behaviour of the process $X$ with respect to the measure $\mathbb{P}$ that makes the $W_{t}$ (or of course the $dW_{t}$ ) a Brownian motion. But the only tool we have seen so far gives us no clue how $W_{t}$ let alone $X_{t}$ changes as the measure changes. 

As it happens, Brownian motions change in easy and pleasant ways under changes in measure. And thus by extension through their differentials, so do stochastic processes. 

## Change of measure - the Radon-Nikodym derivative

To get some intuitive feel for the effects of a change of measure, we should go back for a while to discrete processes. Consider a simple two-step random walk: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/e494a8c6ff63debaf469f45e3e2031b6bcbe16b53f0a632bfdc192d5e8cd8a3b.jpg)



Figure 3.9 Two-step recombinant tree


To get from time 0 to time 2, we can follow four possible paths $\{0,1,2\}$ , $\{0,1,0\}$ , $\{0,-1,0\}$ and $\{0,-1,-2\}$ . Suppose we specified the probability of taking these paths: 


Table 3.1 Path probabilities


<table><tr><td>Path</td><td colspan="2">Probability</td></tr><tr><td>{0,1,2}</td><td><eq>p_1p_2</eq></td><td>=: <eq>\pi_1</eq></td></tr><tr><td>{0,1,0}</td><td><eq>p_1(1-p_2)</eq></td><td>=: <eq>\pi_2</eq></td></tr><tr><td>{0,-1,0}</td><td><eq>(1-p_1)p_3</eq></td><td>=: <eq>\pi_3</eq></td></tr><tr><td>{0,-1,-2}</td><td><eq>(1-p_1)(1-p_3)</eq></td><td>=: <eq>\pi_4</eq></td></tr></table>

We could view this mapping of paths to path probabilities as encoding the measure P. If we knew $\pi_{1}$ , $\pi_{2}$ , $\pi_{3}$ and $\pi_{4}$ , then (as long as all of them are strictly between 0 and 1) we know $p_{1}$ , $p_{2}$ and $p_{3}$ . Thus if we represent our process with a non-recombining tree, we can label each of the paths at the end with the $\pi$ -information encoding the measure. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/fb06bde8fd15aa8cb90ca695b58d5c72458dbcf339ed4f5e17a9d17142d6a477.jpg)



Figure 3.10 Tree with path probabilities marked


Now suppose we had a different measure Q with probabilities $q_{1}$ , $q_{2}$ and $q_{3}$ . Again we can code this up with path probabilities, say $\pi_{1}^{\prime}$ , $\pi_{2}^{\prime}$ , $\pi_{3}^{\prime}$ and $\pi_{4}^{\prime}$ . And again if each $\pi^{\prime}$ is strictly between 0 and 1, $\pi_{1}^{\prime}$ , $\pi_{2}^{\prime}$ , $\pi_{3}^{\prime}$ and $\pi_{4}^{\prime}$ uniquely decides Q. 

And with this encoding, there is a very natural way of encoding the differences between P and Q, giving some idea of how to distort P so as to produce Q. If we form the ratio $\pi_{i}^{\prime}/\pi_{i}$ for each path i, we write the mapping of paths to this ratio as $\frac{dQ}{dP}$ . This random variable (random because it depends on the path) is called the Radon–Nikodym derivative of Q with respect to P up to time 2. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/8fa83a8b183ad6154ce0e4d057d0b97390eb7514c8531a88b1753036a634f403.jpg)



Figure 3.11 Tree with Radon–Nikodym derivative marked


From $\frac{d\mathbb{Q}}{d\mathbb{P}}$ we can derive $\mathbb{Q}$ from $\mathbb{P}$ . How? If we have $\mathbb{P}$ , then we have $\pi_1, \pi_2, \ldots, \pi_4$ , and $\frac{d\mathbb{Q}}{d\mathbb{P}}$ gives us the ratios $\pi_i' / \pi_i$ , so we have $\pi_1', \pi_2', \ldots, \pi_4'$ . And thus $\mathbb{Q}$ . 

What about $p_i$ or $q_i$ being zero or one? Two things happen - firstly it can become impossible to back out the $p_i$ from the $\pi_i$ . Consider if $p_1$ is zero then both $\pi_1$ and $\pi_2$ are zero and so information about $p_2$ is lost. But then of course, the paths corresponding to $\pi_1$ and $\pi_2$ are both impossible (probability zero), so in some sense $p_2$ really isn't relevant. If we restrict ourselves to only providing $\pi_i$ for possible paths, then we can recover the corresponding $p$ 's. 

The second problem has a similar flavour but is more serious. Suppose one of the $p$ 's is zero, but none of the $q$ 's are. Then at least one $\pi_i$ will be zero when none of the $\pi_i'$ are. Not all the ratios $\pi_i' / \pi_i$ will be well defined, and thus $\frac{d\mathbb{Q}}{d\mathbb{P}}$ can't exist. We could suppress those paths which had path probability zero, but now we have lost something. Those paths may have been $\mathbb{P}$ -impossible but they are $\mathbb{Q}$ -possible. If we throw them away, then we have lost information about $\mathbb{Q}$ just where it is relevant -- paths which are $\mathbb{Q}$ -possible. Somehow we can't define $\frac{d\mathbb{Q}}{d\mathbb{P}}$ if $\mathbb{Q}$ allows something which $\mathbb{P}$ doesn't. And of course vice versa. 

This is important enough to formalise. 

## Equivalence

Two measures P and Q are equivalent if they operate on the same sample space and agree on what is possible. Formally, if A is any event in the sample space, 

$$
\mathbb {P} (A) > 0 \iff \mathbb {Q} (A) > 0.
$$

In other words, if A is possible under P then it is possible under Q, and if A is impossible under P then it is also impossible under Q. And vice versa. 

We can only meaningfully define $\frac{d\mathbb{Q}}{d\mathbb{P}}$ and $\frac{d\mathbb{P}}{d\mathbb{Q}}$ if $\mathbb{P}$ and $\mathbb{Q}$ are equivalent, and then only where paths are $\mathbb{P}$ -possible. But of course if paths are $\mathbb{P}$ -impossible then we know how $\mathbb{Q}$ acts on those paths - if $\mathbb{Q}$ is equivalent to $\mathbb{P}$ then they are $\mathbb{Q}$ -impossible as well. 

Thus two measures P and Q must be equivalent before they will have Radon–Nikodym derivatives $\frac{dQ}{dP}$ and $\frac{dP}{dQ}$ . 

## Expectation and $\frac{d\mathbb{Q}}{d\mathbb{P}}$

While we are still working with discrete processes, we should stock up on some facts about expectation and the Radon–Nikodym derivative. One of the reasons for defining it was the efficient coding it represented. Everything we needed to know about Q could be extracted from P and $\frac{dQ}{dP}$ . 

Consider then a claim X known by time 2 on our discrete two-step process. The claim X is a random variable, or in other words a mapping from paths to values – we can let $x_{i}$ denote the value the claim takes if path i is followed. So the expectation of X with respect to P is given by 

$$
\mathbb {E} _ {\mathbb {P}} (X) = \sum_ {i} \pi_ {i} x _ {i},
$$

where i ranges over all four possible paths. And the expectation of X with respect to Q is 

$$
\mathbb {E} _ {\mathbb {Q}} (X) = \sum_ {i} \pi_ {i} ^ {\prime} x _ {i} = \sum_ {i} \pi_ {i} \left(\frac {\pi_ {i} ^ {\prime}}{\pi_ {i}} x _ {i}\right) = \mathbb {E} _ {\mathbb {P}} \left(\frac {d \mathbb {Q}}{d \mathbb {P}} X\right).
$$

Just like $X$ , $\frac{d\mathbb{Q}}{d\mathbb{P}}$ is a random variable which we can take the expectation of. And the conversion from $\mathbb{Q}$ to $\mathbb{P}$ is pleasingly simple: $\mathbb{E}_{\mathbb{Q}}(X) = \mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}} X)$ . 

## 3.4 Change of measure - the C-M-G theorem

Attractive though this is, it represents just one simple case: $\frac{dQ}{dP}$ is defined with a particular time horizon in mind – the ends of the paths, in this case T = 2. We specified X at this time and we only wanted an unconditioned expectation. In formal terms, the result we derived was 

$$
\mathbb {E} _ {\mathbb {Q}} (X _ {T} \mid \mathcal {F} _ {0}) = \mathbb {E} _ {\mathbb {P}} \Big (\frac {d \mathbb {Q}}{d \mathbb {P}} X _ {T} \mid \mathcal {F} _ {0} \Big),
$$

where T is the time horizon for $\frac{dQ}{dP}$ and $X_{T}$ is known at time T. What about $\mathbb{E}_{\mathbb{Q}}(X_{t}|\mathcal{F}_{s})$ for t not equal to T and s not equal to zero? We need somehow to know $\frac{dQ}{dP}$ not just for the ends of paths but everywhere $-\frac{dQ}{dP}$ is a random variable, but we would like a process. 

## Radon-Nikodym process

We can do this by letting the time horizon vary, and setting $\zeta_t$ to be the Radon-Nikodym derivative taken up to the horizon $t$ . That is, $\zeta_t$ is the Radon-Nikodym derivative $\frac{d\mathbb{Q}}{d\mathbb{P}}$ but only following paths up to time $t$ , and only looking at the ratio of probabilities up to that time. For instance, at time 1, the possible paths are $\{0,1\}$ and $\{0,-1\}$ and the derivative $\zeta_1$ has values on them of $q_1/p_1$ and $(1-q_1)/(1-p_1)$ respectively. At time zero, the derivative process $\zeta_0$ is just 1, as the only 'path' is the point $\{0\}$ which has probability 1 under both $\mathbb{P}$ and $\mathbb{Q}$ . Concretely, we can fill in $\zeta_t$ on our tree in terms of the $p$ 's and $q$ 's (figure 3.12). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/67233a964b0175b0d926f8ccf9527ad77a3b05c75797b55048ab641f7e63c1df.jpg)



Figure 3.12 Tree with $\zeta_t$ process marked ( $\bar{p}_i = 1 - p_i$ , $\bar{q}_i = 1 - q_i$ )


In fact there is another expression for $\zeta_{t}$ as the conditional expectation of 

the T-horizon Radon–Nikodym derivative, 

$$
\zeta_ {t} = \mathbb {E} _ {\mathbb {P}} \left(\frac {d \mathbb {Q}}{d \mathbb {P}} \mid \mathcal {F} _ {t}\right),
$$

for every $t$ less than or equal to the horizon $T$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/6cc151a408c65889f48310c751f60461c30b712977df5de2cea19d8fd1369bca.jpg)


## Exercise 3.7 Prove that this equation holds for $t = 0,1,2$ .

We can see that the expectation with respect to P unpicks the $\frac{dQ}{dP}$ in just the right way. The process $\zeta_{t}$ represents just what we wanted – an idea of the amount of change of measure so far up to time t along the current path. If we wanted to know $\mathbb{E}_{\mathbb{Q}}(X_{t})$ it would be $\mathbb{E}_{\mathbb{P}}(\zeta_{t}X_{t})$ , where $X_{t}$ is a claim known at time t. If we want to know $\mathbb{E}_{\mathbb{Q}}(X_{t}|\mathcal{F}_{s})$ then we need the amount of change of measure from time s to time t – which is just $\zeta_{t}/\zeta_{s}$ . That is, the change up to time t with the change up to time s removed. In other words 

$$
\mathbb {E} _ {\mathbb {Q}} \big (X _ {t} \mid \mathcal {F} _ {s} \big) = \zeta_ {s} ^ {- 1} \mathbb {E} _ {\mathbb {P}} \big (\zeta_ {t} X _ {t} \mid \mathcal {F} _ {s} \big).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/2affeba37c3ea6f581e96a46c28e0faa6a08bcf0b15fd6a4838259a30af488df.jpg)


Exercise 3.8 Prove this on the tree. 

## Radon-Nikodym summary

Given P and Q equivalent measures and a time horizon T, we can define a random variable $\frac{dQ}{dP}$ defined on P-possible paths, taking positive real values, such that 

(i) $\mathbb{E}_{\mathbb{Q}}(X_{T})=\mathbb{E}_{\mathbb{P}}\left(\frac{d\mathbb{Q}}{d\mathbb{P}}X_{T}\right),$ 

for all claims $X_{T}$ knowable by time T. 

$$
\mathbb {E} _ {\mathbb {Q}} \left(X _ {t} \mid \mathcal {F} _ {s}\right) = \zeta_ {s} ^ {- 1} \mathbb {E} _ {\mathbb {P}} \left(\zeta_ {t} X _ {t} \mid \mathcal {F} _ {s}\right),
$$

where $\zeta_{t}$ is the process $\mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}}|\mathcal{F}_{t})$ . 

## 3.4 Change of measure - the C-M-G theorem

## Change of measure - the continuous Radon-Nikodym derivative

What now? To define a measure for Brownian motion it seems we have to be able to write down the likelihood of every possible path the process can take, ranging across not only a continuous-valued state space but also a continuous-valued time line. Standard probability theory gives some clue to the technology required, if we were content merely to represent the marginal distributions for the process at each time. Despite the continuous nature of the state space, we know that we can express likelihoods in terms of a probability density function. 

For example, the measure P on the real numbers, corresponding to a normal $N(0,1)$ random variable X, can be represented via the density $f_{\mathbb{P}}(x)$ , where 

$$
f _ {\mathbb {P}} (x) = \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} x ^ {2}}.
$$

In some loose sense, $f_{\mathbb{P}}(x)$ represents the relative likelihood of the event $\{X = x\}$ occurring. Or, less informally the probability that X lies between x and $x + dx$ is approximately $f_{\mathbb{P}}(x)dx$ . In exact terms, the probability that X takes a value in some subset A of the reals is 

$$
\mathbb {P} (X \in A) = \int_ {A} {\frac {1}{\sqrt {2 \pi}}} e ^ {- {\frac {1}{2}} x ^ {2}} d x.
$$

For example, the chance of $X$ being in the interval [0, 1] is the integral of the density over the interval, $\int_0^1 f_{\mathbb{P}}(x) dx$ , which has value 0.3413. 

But marginal distributions aren't enough - a single marginal distribution won't capture the nature of the process (we can see that clearly even on a discrete tree). Nor will all the marginal distributions for each time $t$ . We need nothing less than all the marginal distributions at each time $t$ conditional on every history $\mathcal{F}_s$ for all times $s < t$ . We need to capture the idea of a likelihood of a path in the continuous case, by means of some conceptual handle on a particular path specified for all times $t < T$ . 

One approach is to specify a path if not for all times before the horizon T, then at least for some arbitrarily large yet still finite set of times $\{t_{0}=0,t_{1},\ldots,t_{n-1},t_{n}=T\}$ . Consider then, the set of paths which go through the points $\{x_{1},\ldots,x_{n}\}$ at times $\{t_{1},\ldots,t_{n}\}$ . If there were just one time $t_{1}$ and one point $x_{1}$ , then we could write down the likelihood of such a path. We could use the probability density function of $W_{t_{1}}$ , $f_{\mathbb{P}}^{1}(x)$ , which is the density function of a normal $N(0, t_{1})$ , or 

$$
f _ {\mathbb {P}} ^ {1} (x) = \frac {1}{\sqrt {2 \pi t _ {1}}} \exp \left(- \frac {x ^ {2}}{2 t _ {1}}\right).
$$

And if we can do this for one time $t_{1}$ , then we can for finitely many $t_{i}$ . All we require is the joint likelihood function $f_{\mathbb{P}}^{n}(x_{1},\ldots,x_{n})$ for the process taking values $\{x_{1},\ldots,x_{n}\}$ at times $\{t_{1},\ldots,t_{n}\}$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/d303360e148491e1cec8070b5a9722391f93488e379c924b6f7238f3bc0fc48d.jpg)



Figure 3.13 Two Brownian motions agreeing on the set $\{t_1, t_2, t_3\}$


## Joint likelihood function for Brownian motion

If we take $t_0$ and $x_0$ to be zero, and write $\Delta x_i$ for $x_i - x_{i-1}$ and $\Delta t_i = t_i - t_{i-1}$ , then given the third condition of Brownian motion that increments $\Delta W_i = W(t_i) - W(t_{i-1})$ are mutually independent, we can write down 

$$
f _ {\mathbb {P}} ^ {n} \left(x _ {1}, \dots , x _ {n}\right) = \prod_ {i = 1} ^ {n} \frac {1}{\sqrt {2 \pi \Delta t _ {i}}} \exp \left(- \frac {\left(\Delta x _ {i}\right) ^ {2}}{2 \Delta t _ {i}}\right).
$$

So we can write down a likelihood function corresponding to the measure P for a process on a finite set of times. And in the continuous limit, we have a handle on the measure P for a continuous process. If A is some subset of $R^{n}$ , then the P-probability that the random n-vector $(W_{t_{1}},\ldots,W_{t_{n}})$ is in A is exactly the integral over A of the likelihood function $f_{P}^{n}$ . 

## 3.4 Change of measure - the C-M-G theorem

## Radon-Nikodym derivative - continuous version

Suppose P and Q are equivalent measures. Given a path $\omega$ , for every ordered time mesh $\{t_{1},\ldots,t_{n}\}$ (with $t_{n}=T$ ), we define $x_{i}$ to be $W_{t_{i}}(\omega)$ , and then the derivative $\frac{dQ}{dP}$ up to time T is defined to be the limit of the likelihood ratios 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} (\omega) = \lim _ {n \to \infty} \frac {f _ {\mathbb {Q}} ^ {n} (x _ {1} , \ldots , x _ {n})}{f _ {\mathbb {P}} ^ {n} (x _ {1} , \ldots , x _ {n})},
$$

as the mesh becomes dense in the interval $[0, T]$ . 

This continuous-time derivative $\frac{dQ}{dP}$ still satisfies the results that 

(i) 

$$
\mathbb {E} _ {\mathbb {Q}} (X _ {T}) = \mathbb {E} _ {\mathbb {P}} \Big (\frac {d \mathbb {Q}}{d \mathbb {P}} X _ {T} \Big),\tag{ii}
$$

$$
\mathbb {E} _ {\mathbb {Q}} \left(X _ {t} \mid \mathcal {F} _ {s}\right) = \zeta_ {s} ^ {- 1} \mathbb {E} _ {\mathbb {P}} \left(\zeta_ {t} X _ {t} \mid \mathcal {F} _ {s}\right), \quad s \leqslant t \leqslant T,
$$

where $\zeta_{t}$ is the process $\mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}}|\mathcal{F}_{t})$ , and $X_{t}$ is any process adapted to the history $F_{t}$ . 

Just as the measure P can be approached through a limiting time mesh, so can the Radon-Nikodym derivative $\frac{dQ}{dP}$ . The event of paths agreeing with $\omega$ on the mesh, $A = \{\omega' : W_{t_i}(\omega') = W_{t_i}(\omega), i = 1, \ldots, n\}$ , gets smaller and smaller till it is just the single point-set $\{\omega\}$ . The Radon-Nikodym derivative can be thought of as the limit 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} (\omega) = \lim _ {A \to \{\omega \}} \frac {\mathbb {Q} (A)}{\mathbb {P} (A)}.
$$

## Simple changes of measure - Brownian motion plus constant drift

We have the mechanics of change of measure but still no clue about what change of measure does in the continuous world. Suppose, for example, we had a P-Brownian motion $W_{t}$ . What does $W_{t}$ look like under an equivalent measure Q – is it still recognisably Brownian motion or something quite different? 

Foresight can provide one simple example. Consider $W_{t}$ a P-Brownian motion, then (out of nowhere) define Q to be a measure equivalent to P via 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = \exp \left(- \gamma W _ {T} - \frac {1}{2} \gamma^ {2} T\right),
$$

for some time horizon $T$ . What does $W_{t}$ look like with respect to $\mathbb{Q}$ ? 

One place to start, and it is just a start, is to look at the marginal of $W_{T}$ under Q. We need to find the likelihood function of $W_{T}$ with respect to Q, or something equivalent. One useful trick is to look at moment-generating functions: 

## Identifying normals

A random variable X is a normal $N(\mu, \sigma^{2})$ under a measure P if and only if 

$$
\mathbb {E} _ {\mathbb {P}} \bigl (\exp (\theta X) \bigr) = \exp \bigl (\theta \mu + \frac {1}{2} \theta^ {2} \sigma^ {2} \bigr), \quad \text {   for   all   real   } \theta .
$$

To calculate $\mathbb{E}_{\mathbb{Q}}\bigl(\exp (\theta W_T)\bigr)$ , we can use fact (i) of the Radon-Nikodym derivative summary, which tells us that it is the same as the $\mathbb{P}$ -expectation $\mathbb{E}_{\mathbb{P}}\bigl(\frac{d\mathbb{Q}}{d\mathbb{P}}\exp (\theta W_T)\bigr)$ . This equals 

$$
\mathbb {E} _ {\mathbb {P}} \left(\exp \left(- \gamma W _ {T} - \frac {1}{2} \gamma^ {2} T + \theta W _ {T}\right)\right) = \exp \left(- \frac {1}{2} \gamma^ {2} T + \frac {1}{2} (\theta - \gamma) ^ {2} T\right),
$$

because $W_{T}$ is a normal $N(0,T)$ with respect to $\mathbb{P}$ . 

Simplifying the algebra, we have 

$$
\mathbb {E} _ {\mathbb {Q}} \big (\exp (\theta W _ {T}) \big) = \exp (- \theta \gamma T + \frac {1}{2} \theta^ {2} T),
$$

which is the moment-generating function of a normal $N(-\gamma T, T)$ . Thus the marginal distribution of $W_{T}$ , under Q, is also a normal with variance T but with mean $-\gamma T$ . 

What about $W_{t}$ for t less than T? The marginal distribution of $W_{T}$ is what we would expect if $W_{t}$ under Q were a Brownian motion plus a constant drift $-\gamma$ . Of course, a lot of other process also have a marginal normal $N(-\gamma T, T)$ distribution at time T, but it would be an elegant result if the sole effect of changing from P to Q via $\frac{dQ}{dP} = \exp(-\gamma W_{T} - \frac{1}{2}\gamma^{2}T)$ were just to punch in a drift of $-\gamma$ . 

And so it is. The process $W_{t}$ is a Brownian motion with respect to P and Brownian motion with constant drift $-\gamma$ under Q. Using our two results about $\frac{dQ}{dP}$ , we can prove the three conditions for $\tilde{W}_{t}=W_{t}+\gamma t$ to be Q-Brownian motion: 

(i) $\tilde{W}_t$ is continuous and $\tilde{W}_0 = 0$ ; 

## 3.4 Change of measure - the C-M-G theorem

(ii) $\tilde{W}_t$ is a normal $N(0,t)$ under $\mathbb{Q}$ ; 

(iii) $\tilde{W}_{t+s} - \tilde{W}_s$ is a normal $N(0,t)$ independent of $\mathcal{F}_s$ . The first of these is true and (ii) and (iii) can be re-expressed as 

(ii)' $\mathbb{E}_{\mathbb{Q}}\bigl (\exp (\theta \tilde{W}_t)\bigr) = \exp (\frac{1}{2}\theta^2 t);$ 

(iii)' $\mathbb{E}_{\mathbb{Q}}\bigl (\exp \bigl (\theta (\tilde{W}_{t + s} - \tilde{W}_s)\bigr)\mid \mathcal{F}_s\bigr) = \exp (\frac{1}{2}\theta^2 t).$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/f2c729d8b44bdb14d722590cf940b129cd04258403eaf5b86acee87b48c59539.jpg)


Exercise 3.9 Show that (ii)' and (iii)' are equivalent to (ii) and (iii) respectively, and prove them using the change of measure process $\zeta_t = \mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}}|\mathcal{F}_t)$ . 

That both $W_{t}$ and $\tilde{W}_{t}$ are Brownian motion, albeit with respect to different measures, seems paradoxical. But switching from P to Q just changes the relative likelihood of a particular path being chosen. For example, W might follow a path which drifts downwards for a time at a rate of about $-\gamma$ . Although that path is P-unlikely, it is P-possible. Under Q, on the other hand, such a path is much more likely, and the chances are that is what we see. But it still could be just improbable Brownian motion behaviour. 

We can see this in the Radon–Nikodym derivative $\frac{dQ}{dP}$ which is large when $W_{T}$ is very negative, and small when $W_{T}$ is closer to zero or positive. This is just the consequence of the common sense thought that paths which end up negative are more likely under Q (Brownian motion plus downward drift) than they are under P (driftless Brownian motion). Correspondingly, paths which finish near or above zero are less likely under Q than P. 

## Cameron-Martin-Girsanov

So this one change of measure just changed a vanilla Brownian motion into one with drift – nothing else. And of course, drift is one of the elements of our stochastic differential form of processes. In fact all that measure changes on Brownian motion can do is to change the drift. All the processes that we are interested in are representable as instantaneous differentials made up of some amount of Brownian motion and some amount of drift. The mapping of stochastic differentials under P to stochastic differentials under Q is both natural and pleasing. 

This is what our theorem provides. 

## Cameron-Martin-Girsanov theorem

If $W_{t}$ is a $\mathbb{P}$ -Brownian motion and $\gamma_{t}$ is an $\mathcal{F}$ -previsible process satisfying the boundedness condition $\mathbb{E}_{\mathbb{P}} \exp\left(\frac{1}{2} \int_{0}^{T} \gamma_{t}^{2} dt\right) < \infty$ , then there exists a measure $\mathbb{Q}$ such that 

(i) $\mathbb{Q}$ is equivalent to $\mathbb{P}$ 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = \exp \left(- \int_ {0} ^ {T} \gamma_ {t} d W _ {t} - \frac {1}{2} \int_ {0} ^ {T} \gamma_ {t} ^ {2} d t\right)\tag{ii}
$$

(iii) $\tilde{W}_t = W_t + \int_0^t\gamma_s ds$ is a $\mathbb{Q}$ -Brownian motion. 

In other words, $W_{t}$ is a drifting Q-Brownian motion with drift $-\gamma_{t}$ at time t. 

Within constraints, if we want to turn a P-Brownian motion $W_{t}$ into a Brownian motion with some specified drift $-\gamma_{t}$ , then there's a Q which does it. 

Within limits, drift is measure and measure drift. 

Conversely to the theorem, 

## Cameron-Martin-Girsanov converse

If $W_{t}$ is a P-Brownian motion, and Q is a measure equivalent to P, then there exists an F-previsible process $\gamma_{t}$ such that 

$$
\tilde {W} _ {t} = W _ {t} + \int_ {0} ^ {t} \gamma_ {s} d s
$$

is a Q-Brownian motion. That is, $W_{t}$ plus drift $\gamma_{t}$ is Q-Brownian motion. Additionally the Radon–Nikodym derivative of Q with respect to P (at time T) is $\exp(-\int_{0}^{T}\gamma_{t}dW_{t}-\frac{1}{2}\int_{0}^{T}\gamma_{t}^{2}dt)$ . 

## C-M-G and stochastic differentials

The C-M-G theorem applies to Brownian motion, but all our processes are disguised Brownian motions at heart. Now we can see the rewards of our Brownian calculus instantly - C-M-G becomes a powerful tool for controlling the drift of any process. 

## 3.4 Change of measure - the C-M-G theorem

Suppose that X is a stochastic process with increment 

$$
d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t,
$$

where W is a P-Brownian motion. Suppose we want to find if there is a measure Q such that the drift of process X under Q is $\nu_{t} dt$ instead of $\mu_{t} dt$ . As a first step, dX can be rewritten as 

$$
d X _ {t} = \sigma_ {t} \left(d W _ {t} + \left(\frac {\mu_ {t} - \nu_ {t}}{\sigma_ {t}}\right) d t\right) + \nu_ {t} d t.
$$

If we set $\gamma_t$ to be $(\mu_t - \nu_t) / \sigma_t$ , and if $\gamma$ then satisfies the C-M-G growth condition $(\mathbb{E}_{\mathbb{P}} \exp(\frac{1}{2} \int_0^T \gamma_t^2 dt) < \infty)$ then indeed there is a new measure $\mathbb{Q}$ such that $\tilde{W}_t := W_t + \int_0^t (\mu_s - \nu_s) / \sigma_s ds$ is a $\mathbb{Q}$ -Brownian motion. 

But this means that the differential of X under Q is 

$$
d X _ {t} = \sigma_ {t} d \tilde {W} _ {t} + \nu_ {t} d t,
$$

where $\tilde{W}$ is a Q-Brownian motion – which gives X the drift $\nu_{t}$ we wanted. 

We can also set limits on the changes that changing to an equivalent measure can wreak on a process. Since the change of measure can only change the Brownian motion to a Brownian motion plus drift, the volatility of the process must remain the same. 

## Examples - changes of measure

1. Let $X_{t}$ be the drifting Brownian process $\sigma W_{t} + \mu t$ , where $W$ is a $\mathbb{P}$ -Brownian motion and $\sigma$ and $\mu$ are both constant. Then using $\mathbf{C - M - G}$ with $\gamma_{t} = \mu / \sigma$ , there exists an equivalent measure $\mathbb{Q}$ under which $\tilde{W}_{t} = W_{t} + (\mu / \sigma)t$ and $\tilde{W}$ is a $\mathbb{Q}$ -Brownian motion up to time $T$ . Then $X_{t} = \sigma \tilde{W}_{t}$ , which is (scaled) $\mathbb{Q}$ -Brownian motion. 

The measures also give rise to different expectations. For example, $\mathbb{E}_{\mathbb{P}}(X_{t}^{2})$ equals $\mu^{2}t^{2} + \sigma^{2}t$ , but $\mathbb{E}_{\mathbb{Q}}(X_{t}^{2}) = \sigma^{2}t$ . 

2. Let $X_{t}$ be the exponential Brownian motion with SDE 

$$
d X _ {t} = X _ {t} (\sigma d W _ {t} + \mu d t),
$$

where W is P-Brownian motion. Can we change measure so that X has the new SDE 

$$
d X _ {t} = X _ {t} (\sigma d W _ {t} + \nu d t),
$$

for some arbitrary constant drift $\nu$ ? 

Using C-M-G with $\gamma_{t}=(\mu-\nu)/\sigma$ , there is indeed a measure Q under which $\tilde{W}_{t}=W_{t}+(\mu-\nu)t/\sigma$ is a Q-Brownian motion. Then X does have the SDE 

$$
d X _ {t} = X _ {t} (\sigma d \tilde {W} _ {t} + \nu d t),
$$

where $\tilde{W}$ is a $\mathbb{Q}$ -Brownian motion. 

## 3.5 Martingale representation theorem

We can solve some SDEs with Itô; we can see how SDEs change as measure changes. But central to answering our pricing question in chapter two was the concept of a measure with respect to which the process was expected to stay the same, the martingale measure for our discrete trees. The price of derivatives turned out to be an expectation under this measure, and the construction of this expectation even showed us the trading strategy required to justify this price. And so it is here. 

First the description again: 

## Martingales

A stochastic process $M_t$ is a martingale with respect to a measure $\mathbb{P}$ if and only if 

$$
\mathbb {E} _ {\mathbb {P}} \big (| M _ {t} | \big) <   \infty , \quad \text { for   all } t \tag {i}
$$

$$
\mathbb {E} _ {\mathbb {P}} \big (M _ {t} \mid \mathcal {F} _ {s} \big) = M _ {s}, \quad \text {   for   all   } s \leqslant t. \tag {ii}
$$

The first condition is merely a technical sweetener, it is the second that carries the weight. A martingale measure is one which makes the expected future value conditional on its present value and past history merely its present value. It isn't expected to drift upwards or downwards. 

Some examples: 

(1) Trivially, the constant process $S_{t} = c$ (for all $t$ ) is a martingale with respect to any measure: $\mathbb{E}_{\mathbb{P}}(S_t|\mathcal{F}_s) = c = S_s$ , for all $s \leqslant t$ , and for any 

## 3.5 Martingale representation theorem

## measure P.

(2) Less trivially, $\mathbb{P}$ -Brownian motion is a $\mathbb{P}$ -martingale. Intuitively this makes sense - Brownian motion doesn't move consistently up or down, it's as likely to do either. But we should get into the habit of checking this formally: we need $\mathbb{E}_{\mathbb{P}}(W_t|\mathcal{F}_s) = W_s$ . Of course we have that the increment $W_{t} - W_{s}$ is independent of $\mathcal{F}_s$ and distributed as a normal $N(0,t - s)$ , so that $\mathbb{E}_{\mathbb{P}}(W_t - W_s|\mathcal{F}_s) = 0$ . This yields the result, as 

$$
\mathbb {E} _ {\mathbb {P}} (W _ {t} | \mathcal {F} _ {s}) = \mathbb {E} _ {\mathbb {P}} (W _ {s} | \mathcal {F} _ {s}) + \mathbb {E} _ {\mathbb {P}} (W _ {t} - W _ {s} | \mathcal {F} _ {s}) = W _ {s} + 0.
$$

(3) For any claim $X$ depending only on events up to time $T$ , the process $N_{t} = \mathbb{E}_{\mathbb{P}}(X|\mathcal{F}_t)$ is a $\mathbb{P}$ -martingale (assuming only the technical constraint $\mathbb{E}_{\mathbb{P}}(|X|) < \infty$ ). 

Example (3) is an elegant little trick for producing martingales - and as we shall see (and have already seen in chapter two) central to pricing derivatives. First why? Convince yourself that $N_{t} = \mathbb{E}_{\mathbb{P}}(X|\mathcal{F}_t)$ is a well-defined process - the first stage of the alchemy is the introduction of a time line into the random variable $X$ . Now for $N_{t}$ to be a $\mathbb{P}$ -martingale, we require $\mathbb{E}_{\mathbb{P}}(N_t|\mathcal{F}_s) = N_s$ , but for this we merely need to be satisfied that 

$$
\mathbb {E} _ {\mathbb {P}} \left(\mathbb {E} _ {\mathbb {P}} (X | \mathcal {F} _ {t}) \mid \mathcal {F} _ {s}\right) = \mathbb {E} _ {\mathbb {P}} \left(X \mid \mathcal {F} _ {s}\right).
$$

That is, that conditioning firstly on information up to time t and then on information up to time s is just the same as conditioning up to time s to begin with. This property of conditional expectation is the tower law. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/f8eee17c44c33e128d55eb144bf81e846a88333902db6fb1737e17d1682b9129.jpg)


Exercise 3.10 Show that the process $X_{t} = W_{t} + \gamma t$ , where $W_{t}$ is a $\mathbb{P}$ -Brownian motion, is a $\mathbb{P}$ -martingale if and only if $\gamma = 0$ . 

## Representation

In chapter two, we had a binomial representation theorem - if $M_t$ and $N_t$ are both $\mathbb{P}$ -martingales then they share more than just the name - locally they can only differ by a scaling, by the size of the opening of each particular branching. We could represent changes in $N_{t}$ by scaled changes in the other non-trivial P-martingale. Thus $N_{t}$ itself can be represented by the scaled sum of these changes. 

In the continuous world: 

## Martingale representation theorem

Suppose that $M_{t}$ is a Q-martingale process, whose volatility $\sigma_{t}$ satisfies the additional condition that it is (with probability one) always non-zero. Then if $N_{t}$ is any other Q-martingale, there exists an F-previsible process $\phi$ such that $\int_{0}^{T}\phi_{t}^{2}\sigma_{t}^{2}dt<\infty$ with probability one, and N can be written as 

$$
N _ {t} = N _ {0} + \int_ {0} ^ {t} \phi_ {s} d M _ {s}.
$$

Further $\phi$ is (essentially) unique. 

This is virtually identical to the earlier result, with summation replaced by an integral. As we are getting used to, the move to a continuous process extracts 'a formal technical penalty. In this case, the Q-martingale's volatility must be positive with probability 1 – but otherwise our chapter two result has carried across unchanged. If there is a measure Q under which $M_{t}$ is a Q-martingale, then any other Q-martingale can be represented in terms of $M_{t}$ . The process $\phi_{t}$ is simply the ratio of their respective volatilities. 

## Driftlessness

We need just one more tool. Thrown into the discussion of martingales was the intuitive description of a martingale as neither drifting up or drifting down. We have, though, a technical definition of drift via our stochastic differential formulation. An obvious question springs to mind: are stochastic processes with no drift term always martingales, and vice versa can martingales always be represented as just $\sigma_{t} dW_{t}$ for some F-previsible volatility process $\sigma_{t}$ ? 

Nearly. 

One way round we can do for ourselves with the martingale representation theorem. If a process $X_{t}$ is a P-martingale then with $W_{t}$ a P-Brownian motion, we have an F-previsible process $\phi_{t}$ such that 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \phi_ {s} d W _ {s}.
$$

## 3.5 Martingale representation theorem

This is just the integral form of the increment $dX_{t} = \phi_{t} dW_{t}$ , which has no drift term. 

The other way round is true (up to a technical constraint), but harder. For reference: 

## A collector's guide to martingales

If $X$ is a stochastic process with volatility $\sigma_t$ (that is $dX_t = \sigma_t dW_t + \mu_t dt$ ) which satisfies the technical condition $\mathbb{E}\left[(\int_0^T \sigma_s^2 ds)^{\frac{1}{2}}\right] < \infty$ , then 

$$
X \text {   is   a   martingale   } \iff X \text {   is   driftless   } (\mu_ {t} \equiv 0).
$$

If the technical condition fails, a driftless process may not be a martingale. Such processes are called local martingales. 

## Exponential martingales

The technical constraint can be tiresome. For example, take the (driftless) SDE for an exponential process $dX_{t} = \sigma_{t}X_{t}dW_{t}$ . The condition (in this case, $\mathbb{E}\left[\left(\int_{0}^{T}\sigma_{s}^{2}X_{s}^{2}ds\right)^{\frac{1}{2}}\right] < \infty$ ) is difficult to check, but for these specific exponential examples, a better (more practical) test is: 

## A collector's guide to exponential martingales

If $dX_{t} = \sigma_{t}X_{t}dW_{t}$ , for some $\mathcal{F}$ -previsible process $\sigma_{t}$ , then 

$$
\mathbb {E} \left(\exp \left(\frac {1}{2} \int_ {0} ^ {T} \sigma_ {s} ^ {2} d s\right)\right) <   \infty \Rightarrow X \text {   is   a   martingale. }
$$

We also note that the solution to the SDE is $X_{t} = X_{0}\exp \left(\int_{0}^{t}\sigma_{s}dW_{s} - \frac{1}{2}\int_{0}^{t}\sigma_{s}^{2}ds\right)$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/02b7d86bea2f6e94326042b4b40a3b9f3dc7bdd7ac5c481a72f392659a91b640.jpg)


Exercise 3.11 If $\sigma_{t}$ is a bounded function of both time and sample path, show that $dX_{t} = \sigma_{t}X_{t}dW_{t}$ is a $\mathbb{P}$ -martingale. 

# Continuous processes

## 3.6 Construction strategies

We have the mathematical tools – Itô, Cameron–Martin–Girsanov, and the martingale representation theorem – now we need some idea of how to hook them into a financial model. In the simplest models, Black–Scholes for example, we’ll have a market consisting of one random security and a riskless cash account bond; and with this comes the idea of a portfolio. 

## The portfolio $(\phi, \psi)$

A portfolio is a pair of processes $\phi_t$ and $\psi_t$ which describe respectively the number of units of security and of the bond which we hold at time $t$ . The processes can take positive or negative values (we'll allow unlimited short-selling of the stock or bond). The security component of the portfolio $\phi$ should be $\mathcal{F}$ -previsible: depending only on information up to time $t$ but not $t$ itself. 

There is an intuitive way to think about previsibility. If $\phi$ were left-continuous (that is, $\phi_{s}$ tends to $\phi_{t}$ as s tends upwards to t from below) then $\phi$ would be previsible. If $\phi$ were only right-continuous (that is, $\phi_{s}$ tends to $\phi_{t}$ only as s tends downwards to t from above), then $\phi$ need not be. 

## Self-financing strategies

With the idea of a portfolio comes the idea of a strategy. The description $(\phi_{t}, \psi_{t})$ is a dynamic strategy detailing the amount of each component to be held at each instant. And one particularly interesting set of strategies or portfolios are those that are financially self-contained or self-financing. 

A portfolio is self-financing if and only if the change in its value only depends on the change of the asset prices. In the discrete framework this was captured via a difference equation, and in the continuous case it is equivalent to an SDE. 

## What SDE?

With stock price $S_{t}$ and bond price $B_{t}$ , the value, $V_{t}$ , of a portfolio $(\phi_{t}, \psi_{t})$ at time t is given by $V_{t} = \phi_{t} S_{t} + \psi_{t} B_{t}$ . At the next time instant, two things happen: the old portfolio changes value because $S_{t}$ and $B_{t}$ have changed 

## 3.6 Construction strategies

price; and the old portfolio has to be adjusted to give a new portfolio as instructed by the trading strategy $(\phi,\psi)$ . If the cost of the adjustment is perfectly matched by the profits or losses made by the portfolio then no extra money is required from outside – the portfolio is self-financing. 

In our discrete language, we had the difference equation 

$$
\Delta V _ {i} = \phi_ {i} \Delta S _ {i} + \psi_ {i} \Delta B _ {i}.
$$

In continuous time, we get a stochastic differential equation: 

Self-financing property
If $(\phi_{t},\psi_{t})$ is a portfolio with stock price $S_{t}$ and bond price $B_{t}$ , then $(\phi_{t},\psi_{t})$ is self-financing $\Longleftrightarrow dV_{t} = \phi_{t} dS_{t} + \psi_{t} dB_{t}$ . 

Suppose the stock price $S_{t}$ is given by a simple Brownian motion $W_{t}$ (so $S_{t} = W_{t}$ for all t), and the bond price $B_{t}$ is constant ( $B_{t} = 1$ for all t). What kind of portfolios are self-financing? 

(1) Suppose $\phi_t = \psi_t = 1$ for all $t$ . If we hold a unit of stock and a unit of bond for all time without change, then the value of the portfolio $(V_t = W_t + 1)$ may fluctuate, but it will all be due to fluctuation of the stock. Intuitively, no extra money is needed to come in to uphold the $(\phi_t, \psi_t)$ strategy and none comes out - this $(\phi_t, \psi_t)$ portfolio ought to be self-financing. 

Checking this formally, $V_{t} = W_{t} + 1$ implies that $dV_{t} = dW_{t}$ which is the same as $\phi_{t} dS_{t} + \psi_{t} dB_{t}$ , as we required (remembering that $dB_{t} = 0$ ). 

(2) Suppose $\phi_t = 2W_t$ and $\psi_t = -t - W_t^2$ . Here $(\phi_t, \psi_t)$ is a portfolio, $\phi_t$ is previsible, and the value $V_t = \phi_t S_t + \psi_t B_t = W_t^2 - t$ . By Itô's formula, $dV_t = 2W_t dW_t$ which is identical to $\phi_t dS_t + \psi_t dB_t$ as required. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/4cbc8df42170e37b2b626707b14d8b3f02a77794394ec33fb1050002b8372988.jpg)


Exercise 3.12 Verify the Itô claim in (2) above (which also shows that $W_{t}^{2} - t$ is a martingale). 

Surprising though it seems: holding as many units of stock as twice its current price, though a rollercoaster strategy, is exactly offset by the stock profits and the changing bond holding of $-(t + W_{t}^{2})$ . The $(\phi_{t}, \psi_{t})$ strategy could (in a perfect market) be followed to our heart's content without further funding. 

The second example should convince us that being self-financing is not an automatic property of a portfolio. The Itô check worked, but it could easily have failed if $\psi_{t}$ had been different – the $(\phi_{t}, \psi_{t})$ strategy would have required injections or forced outflows of cash. Every time we claim a portfolio is self-financing we have to turn the handle on Itô's formula to check the SDE. 

## Trading strategies

Now we can define a replicating strategy for a claim: 

## Replicating strategy

Suppose we are in a market of a riskless bond B and a risky security S with volatility $\sigma_{t}$ , and a claim X on events up to time T. 

A replicating strategy for X is a self-financing portfolio $(\phi,\psi)$ such that $\int_{0}^{T}\sigma_{t}^{2}\phi_{t}^{2}dt<\infty$ and $V_{T}=\phi_{T}S_{T}+\psi_{T}B_{T}=X$ . 

Why should we care about replicating strategies? For the same reason as we wanted them in the discrete market models. The claim X gives the value of some derivative which we need to pay off at time T. We want a price if there is one, as of now, given a model for S and B. 

If there is a replicating strategy $(\phi_{t},\psi_{t})$ , then the price of X at time t must be $V_{t}=\phi_{t}S_{t}+\psi_{t}B_{t}$ . (And specifically, the price at time zero is $V_{0}=\phi_{0}S_{0}+\psi_{0}B_{0}$ .) If it were lower, a market player could buy one unit of the derivative at time t and sell $\phi_{t}$ units of S and $\psi_{t}$ units of B against it, continuing to be short $(\phi,\psi)$ until time T. Because $(\phi,\psi)$ is self-financing and the portfolio is worth X at time T guaranteed, the bought derivative and sold portfolio would safely cancel at time T, and no extra money is required between times t and T. The profit created by the mismatch at time t can be banked there and then without risk. And, as usual with arbitrage, one unit could have been many; no risk means no fear. 

## 3.7 Black-Scholes model

And of course if the derivative price had been higher than $V_{t}$ , then we could have sold the derivative and bought the self-financing $(\phi, \psi)$ to the same effect. Replicating strategies, if they exist, tie down the price of the claim X not just at payoff but everywhere. 

We can lay out a battle plan. We define a market model with a stock price process complex enough to satisfy our need for realism. Then, using whatever tools we have to hand we find replicating strategies for all useful claims X. And if we can, we can price derivatives in the model. The rest of the book consists of upping the stakes in complexity of models and of claims. 

## 3.7 Black-Scholes model

We need a model to cut our teeth on. We have the tools and we've seen the overall approach at the end of chapter two. So taking the stock model of section 3.1, we will use the Cameron–Martin–Girsanov theorem (section 3.4) to change it into a martingale, and then use the martingale representation theorem (section 3.5) to create a replicating strategy for each claim. Itô will oil the works. 

The model 

## Our first model - basic Black-Scholes

We will posit the existence of a deterministic r, $\mu$ and $\sigma$ such that the bond price $B_{t}$ and the stock price follow 

$$
\begin{array}{l} B _ {t} = \exp (r t), \\ S _ {t} = S _ {0} \exp (\sigma W _ {t} + \mu t), \end{array}
$$

where r is the riskless interest rate, $\sigma$ is the stock volatility and $\mu$ is the stock drift. There are no transaction costs and both instruments are freely and instantaneously tradable either long or short at the price quoted. 

We need a model for the behaviour of the stock - simple enough that we actually can find replicating strategies but not so simple that we can't bring ourselves to believe in it as a model of the real world. 

Following in Black and Scholes' footsteps, our market will consist of a riskless constant-interest rate cash bond and a risky tradable stock following an exponential Brownian motion. 

As we've seen in section 3.1, it is at least a plausible match to the real world. And as we shall see here, it is quite hard enough to start with. 

## Zero interest rates

If there's one parameter that throws up a smokescreen around a first run at an analysis of the Black–Scholes model, it's the interest rate $r$ . The problems it causes are more tedious than fatal – as we'll see soon, the tools we have are powerful enough to cope. But we'll temporarily simplify things, and set $r$ to be zero. 

So now we begin. For an arbitrary claim X, knowable by some horizon time T, we want to see if we can find a replicating strategy $(\phi_{t}, \psi_{t})$ . 

## Finding a replicating strategy

We shall follow a three-step process outlined in this box here. 

## Three steps to replication

(1) Find a measure $\mathbb{Q}$ under which $S_{t}$ is a martingale. 

(2) Form the process $E_{t} = \mathbb{E}_{\mathbb{Q}}(X|\mathcal{F}_t)$ . 

(3) Find a previsible process $\phi_t$ , such that $dE_t = \phi_t dS_t$ . 

The tools described earlier on will be essential to do this. We shall use the Cameron–Martin–Girsanov theorem (section 3.4) for the first step and the martingale representation theorem (section 3.5) for the third one. 

## Step one

For two different reasons - firstly we need to apply the Cameron-Martin-Girsanov theorem, and secondly we need to be able to tell if $S_{t}$ is a Q-martingale for a given Q - we want to find an SDE for $S_{t}$ . 

## 3.7 Black-Scholes model

The stock follows an exponential Brownian motion, $S_{t} = \exp(\sigma W_{t} + \mu t)$ , so the logarithm of the stock price, $Y_{t} = \log(S_{t})$ , follows a simple drifting Brownian motion $Y_{t} = \sigma W_{t} + \mu t$ . Thus the SDE for $Y_{t}$ is easy to write down: $dY_{t} = \sigma dW_{t} + \mu dt$ . But, of course, Itô makes it possible to write down the SDE for $S_{t} = \exp(Y_{t})$ as 

$$
d S _ {t} = \sigma S _ {t} d W _ {t} + (\mu + \frac {1}{2} \sigma^ {2}) S _ {t} d t.
$$

In order for $S_{t}$ to be a martingale, the first thing to do is to kill the drift in this SDE. If we let $\gamma_{t}$ be a process with constant value $\gamma = (\mu + \frac{1}{2}\sigma^{2})/\sigma$ , then the C-M-G theorem says that there is a measure Q such that $\tilde{W}_{t} = W_{t} + \gamma t$ is Q-Brownian motion. (The technical boundedness condition is satisfied because $\gamma_{t}$ is constant.) Substituting in, the SDE is now 

$$
d S _ {t} = \sigma S _ {t} d \tilde {W} _ {t}.
$$

No drift term, thus $S_{t}$ could be a Q-martingale. The exponential martingales box (section 3.5) contains a condition in terms of $\sigma$ for $S_{t}$ to be a martingale under Q. As $\sigma$ is constant, the condition holds which means that $S_{t}$ must be a Q-martingale. Consequently, Q is the martingale measure for $S_{t}$ . 

## Step two

Given Q, we can convert X into a process by forming $E_{t} = \mathbb{E}_{\mathbb{Q}}(X|\mathcal{F}_{t})$ . This is, as we have already discussed in example (3) of section 3.5, a Q-martingale. 

## Step three

Since there is a Q, under which both $E_{t}$ and $S_{t}$ are Q-martingales, we can invoke the martingale representation theorem. There exists a previsible process $\phi_{t}$ which constructs $E_{t} = \mathbb{E}_{\mathbb{Q}}(X|\mathcal{F}_{t})$ out of $S_{t}$ . (To use the theorem, we need to check that the volatility of $S_{t}$ is always positive, but this is true because the volatility is just $\sigma S_{t}$ , and both $\sigma$ and $S_{t}$ are always positive.) Formally: 

$$
E _ {t} = \mathbb {E} _ {\mathbb {Q}} (X | \mathcal {F} _ {t}) = \mathbb {E} _ {\mathbb {Q}} (X) + \int_ {0} ^ {t} \phi_ {s} d S _ {s},
$$

or, of course, $dE_{t} = \phi_{t} dS_{t}$ . So the martingale representation theorem tells us an important fact: given a Q that makes $S_{t}$ a Q-martingale with positive volatility, $dE_{t} = \phi_{t} dS_{t}$ for some $\phi_{t}$ . 

We need a replicating strategy $(\phi_{t}, \psi_{t})$ , and it's tempting to believe that we have got one half of it. So we should try it, setting $\psi_{t}$ to be the only thing it can be, given that we want the portfolio to be worth $E_{t}$ for all t. 

Replicating strategy 

Our strategy is to: 

• hold $\phi_{t}$ units of stock at time t and 

- hold $\psi_t = E_t - \phi_t S_t$ units of the bond at time $t$ . 

Is it self-financing? The value of the portfolio at time t is 

$$
V _ {t} = \phi_ {t} S _ {t} + \psi_ {t} B _ {t} = E _ {t},
$$

because the bond $B_{t}$ is constantly equal to 1. Thus $dV_{t}=dE_{t}$ , but of course $dE_{t}=\phi_{t}dS_{t}$ , from the martingale representation theorem. 

Since $dB_{t}$ is zero, we have the self-financing condition we want, namely $dV_{t} = \phi_{t} dS_{t} + \psi_{t} dB_{t}$ . 

Since the terminal value of the strategy $V_{T}$ is $E_{T} = X$ , we have a replicating strategy for X – which means there is an arbitrage price for X at all times. Specifically there is an arbitrage price for X at time zero – the value of the $(\phi_{t}, \psi_{t})$ portfolio at time zero, which makes the price $E_{0}$ , or $\mathbb{E}_{\mathbb{Q}}(X)$ . In other words, the price of the claim X is its expected value under the measure that makes the stock process $S_{t}$ a martingale. 

It is worth pausing to let a few surprises sink in. The first is just the fact that there are replicating strategies for arbitrary claims. The model that we have chosen isn't too unrealistic – it has the right kind of behaviour and a healthy degree of randomness. So we might expect to fail in our search for replicating strategies. It is after all particularly odd that despite the lack of knowledge about the claim's eventual value, we can nevertheless trade in the market in such a way that we always produce it. 

The second surprise, and just as important, is that the price of the derivative has such a simple expression – the expected value of the claim. It is the easiest thing to forget that this is not the expectation of the claim with respect to the real measure of $S_{t}$ , which is the measure that makes it an exponential Brownian motion with drift $\mu$ and volatility $\sigma$ . All that expectation could give us would be a long-term average of the claim's payout. And though that could be a useful thing to know in order to judge whether punting with the 

## 3.7 Black–Scholes model

derivative is worthwhile in the long run, it doesn't give a price. There is a replicating strategy and thus an arbitrage price for the claim. And arbitrage always wins out. 

The price happens to be an expectation, but not the expectation in a traditional statistics sense. It could only be the expectation if quite by chance the drift $\mu$ we believe in for the stock were exactly and precisely right to make $S_{t}$ a martingale in the first place ( $\mu = -\frac{1}{2}\sigma^{2}$ ). 

The third surprise is the simplicity of the process $S_{t}$ under its martingale measure. If we actually want to crank the handle and calculate derivative prices for a particular claim, we have to be able to calculate the expected value of the claim under the martingale measure Q. Since the claim depends on $S_{t}$ , this normally involves calculating the expected value, under Q, of some function of the values of $S_{t}$ up to t = T. If $S_{t}$ were an unpleasant process under Q, then this task could be unpleasant too. But $S_{t}$ is also an exponential Brownian motion under Q. If we solve the SDE, then 

$$
S _ {t} = \exp (\sigma \tilde {W} _ {t} - \frac {1}{2} \sigma^ {2} t),
$$

and we find that $S_{t}$ has the same constant volatility $\sigma$ and a new but also constant drift of $-\frac{1}{2}\sigma^{2}$ . So if we felt that $S_{t}$ was tractable under its original measure, it is also tractable under the martingale measure. 

## Non-zero interest rates

Now we can bring the interest rate $r$ back in again. What happens if $r$ is non-zero? We can't just ignore it. Suppose we did, and considered a forward contract with claim $S_T - k$ for some price $k$ . We already know that the $k$ which gives the forward contract a zero value at time zero is $k = S_0 e^{rT}$ . The arbitrage to produce this is easy to figure out. But our rule, when $r$ was zero, of simply taking the expected value of the claim under the martingale measure for $S_t$ cannot work. In fact, 

$$
\mathbb {E} _ {\mathbb {Q}} \left(S _ {T} - S _ {0} e ^ {r T}\right) = S _ {0} \left(1 - e ^ {r T}\right) \neq 0.
$$

Even discounting the claim won't help in this case. So our rule of finding a measure which makes $S_{t}$ into a martingale only holds true when $r$ is zero. When $r$ is not zero, the inexorable growth of cash gets in the way. 

So we take a guess. If the growth of cash is annoying, simply remove it by discounting everything. We call $B_{t}^{-1}$ the discount process, and form a discounted stock $Z_{t}=B_{t}^{-1}S_{t}$ and a discounted claim $B_{T}^{-1}X$ . 

In this discounted world, we could be forgiven for thinking that $r$ was zero again. So maybe our analysis will work again. Of course, this is all just heuristic justification, and the proof is only in the doing. If we can't find a replicating strategy then, attractive as our guess is, it is also wrong. 

Fortunately, we can. Focusing on our discounted stock process $Z_{t}$ , it is not too hard to write down an SDE 

$$
d Z _ {t} = Z _ {t} \big (\sigma d W _ {t} + \big (\mu - r + \frac {1}{2} \sigma^ {2} \big) d t \big).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/aa5b7bb00b29795a8b5f1fcd06dbbf416cddc514a5303a12244788faa60c66df.jpg)


Exercise 3.13 Prove it. 

## Step one

To make $Z_{t}$ into a martingale, we can invoke C-M-G just as before, only now to introduce a drift of $(\mu - r + \frac{1}{2}\sigma^{2})/\sigma$ to the underlying Brownian motion. So there exists (another) Q equivalent to the original measure P and a Q-Brownian motion $\tilde{W}_{t}$ such that 

$$
d Z _ {t} = \sigma Z _ {t} d \tilde {W} _ {t}.
$$

So $Z_{t}$ , under $\mathbb{Q}$ , is driftless and a martingale. 

## Step two

We need a process which hits the discounted claim and is also a Q-martingale. And, as before, conditional expectation provides it, namely by forming the process $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X \mid \mathcal{F}_{t})$ . 

## Step three

The discounted stock price $Z_{t}$ is a Q-martingale; and so is the conditional expectation process of the discounted claim $E_{t}$ . Thus the martingale representation theorem gives us a previsible $\phi_{t}$ such that $dE_{t} = \phi_{t} dZ_{t}$ . 

We want to hit the real claim with amounts of the real stock, but in our shadow discounted world we can hit the discounted claim by holding $\phi_{t}$ units of the discounted stock. So just as a guess, let us try $\phi_{t}$ out in the real world as well. 

## 3.7 Black-Scholes model

What about the bond holding? The bond holding in the discounted world is $\psi_{t}=E_{t}-\phi_{t}Z_{t}$ , so we can try that in the real world too. Some reassurance comes from the fact that at time T we will be holding $\phi_{T}$ units of the stock and $\psi_{T}$ units of the bond which will be worth $\phi_{T}S_{T}+\psi_{T}B_{T}=B_{T}E_{T}=X$ . 

So our replicating strategy is to 

• hold $\phi_{t}$ units of the stock at time t, and 

- hold $\psi_t = E_t - \phi_t Z_t$ units of the bond. 

Are we right? The value $V_{t}$ of the portfolio $(\phi_{t},\psi_{t})$ is given by $V_{t}=\phi_{t}S_{t}+\psi_{t}B_{t}=B_{t}E_{t}$ . Thus following exercise 3.6, we can write $dV_{t}$ as 

$$
d V _ {t} = B _ {t} d E _ {t} + E _ {t} d B _ {t}.
$$

But $dE_{t}$ is $\phi_{t}dZ_{t}$ (our fact from the martingale representation theorem), and so $dV_{t}=\phi_{t}B_{t}dZ_{t}+E_{t}dB_{t}$ . A bit of rearrangement tells us that $E_{t}=\phi_{t}Z_{t}+\psi_{t}$ , and thus 

$$
d V _ {t} = \phi_ {t} B _ {t} d Z _ {t} + (\phi_ {t} Z _ {t} + \psi_ {t}) d B _ {t} = \phi_ {t} (B _ {t} d Z _ {t} + Z _ {t} d B _ {t}) + \psi_ {t} d B _ {t}.
$$

But, from exercise 3.6 again, $d(B_{t}Z_{t}) = B_{t}dZ_{t} + Z_{t}dB_{t}$ , and since $S_{t} = B_{t}Z_{t}$ , we have 

$$
d V _ {t} = \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t}.
$$

That is, $(\phi_t,\psi_t)$ is self-financing. 

## Self-financing strategies

A portfolio strategy $(\phi_{t},\psi_{t})$ of holdings in a stock $S_{t}$ and a non-volatile cash bond $B_{t}$ has value $V_{t}=\phi_{t}S_{t}+\psi_{t}B_{t}$ and discounted value $E_{t}=\phi_{t}Z_{t}+\psi_{t}$ , where Z is the discounted stock process $Z_{t}=B_{t}^{-1}S_{t}$ . Then the strategy is self-financing if either 

$$
\begin{array}{l} d V _ {t} = \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t}, \\ d E _ {t} = \phi_ {t} d Z _ {t}. \end{array}
$$

or equivalently 

A strategy is self-financing if changes in its value are due only to changes in the assets' values, or equivalently if changes in its discounted value are due only to changes in the discounted values of the assets. 

Since we know that $V_{T} = X$ , then we have proved that $(\phi_{t}, \psi_{t})$ is a replicating strategy for X. Our guesses came good. 

## Summary

Suppose we have a Black–Scholes model for a continuously tradable stock and bond, that is assuming the existence of a constant r, $\mu$ and $\sigma$ such that their respective prices can be represented as $S_{t} = S_{0} \exp(\sigma W_{t} + \mu t)$ and $B_{t} = \exp(rt)$ . Then all integrable claims X, knowable by some time horizon T, have associated replicating strategies ( $\phi_{t}, \psi_{t}$ ). In addition, the arbitrage price of such a claim X is given by 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t} \big) = e ^ {- r (T - t)} \mathbb {E} _ {\mathbb {Q}} (X | \mathcal {F} _ {t}),
$$

where Q is the martingale measure for the discounted stock $B_{t}^{-1}S_{t}$ . 

The important measure Q is not the measure which makes the stock a martingale, but the measure that makes the discounted stock a martingale. And the arbitrage price of the claim is the expectation under Q of the discounted claim. 

So when interest rates are non-zero, what are the new rules? They are just discounted versions of the old rules: 

Three steps to replication (discounted case) 

(1) Find a measure $\mathbb{Q}$ under which the discounted stock price $Z_{t}$ is a martingale. 

(2) Form the process $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X \mid \mathcal{F}_{t})$ . 

(3) Find a previsible process $\phi_t$ , such that $dE_t = \phi_t dZ_t$ . 

## Call options

We should price something. Following Black and Scholes, we'll price a call option – the right but not the obligation to buy a unit of stock for a 

## 3.7 Black-Scholes model

predetermined amount at a particular exercise date, say T. If we let this predetermined amount be k (in financial terms, the strike of the option), then in formal notation, our claim is $\max(S_{T}-k,0)$ . Or in more convenient notation, $(S_{T}-k)^{+}$ . 

First we should find $V_{0}$ , the value of the replicating strategy (and thus the option) at time zero. Our formula tells us that this is given by 

$$
e ^ {- r T} \mathbb {E} _ {\mathbb {Q}} \big ((S _ {T} - k) ^ {+} \big),
$$

where $\mathbb{Q}$ is the martingale measure for $B_{t}^{-1}S_{t}$ . 

But how do we find this? The first thing to notice is the simplicity of the claim. The value $(S_{T}-k)^{+}$ only depends on the stock price at one point in time – namely the expiry time, T. So to find the expectation of this claim we need only find the marginal distribution of $S_{T}$ under Q. 

And to do that, we can look at the process for $S_{t}$ written in terms of the Q-Brownian motion $\tilde{W}_{t}$ . Since $d(\log S_{t}) = \sigma d\tilde{W}_{t} + (r - \frac{1}{2}\sigma^{2}) dt$ , if we denote the stock price at time zero, $S_{0}$ , by s, we have that $\log S_{t} = \log s + \sigma\tilde{W}_{t} + (r - \frac{1}{2}\sigma^{2}) t$ , and thus $S_{t} = s \exp\left(\sigma\tilde{W}_{t} + (r - \frac{1}{2}\sigma^{2}) t\right)$ . 

So the marginal distribution for $S_{T}$ is given by s times the exponential of a normal with mean $(r - \frac{1}{2}\sigma^{2})T$ and variance $\sigma^{2}T$ . Thus if we let Z be a normal $N(-\frac{1}{2}\sigma^{2}T, \sigma^{2}T)$ , we can write $S_{T}$ as $se^{(Z+rT)}$ and thus the claim as the expectation $e^{-rT}\mathbb{E}\big((se^{(Z+rT)} - k)^{+}\big)$ , which equals 

$$
\frac {1}{\sqrt {2 \pi \sigma^ {2} T}} \int_ {\log (k / s) - r T} ^ {\infty} (s e ^ {x} - k e ^ {- r T}) \exp \left(- \frac {(x + \frac {1}{2} \sigma^ {2} T) ^ {2}}{2 \sigma^ {2} T}\right) d x.
$$

This integral can be decomposed by a change of variables into a couple of standard cumulative normal integrals. If we use the notation $\Phi(x)$ to denote $(2\pi)^{-\frac{1}{2}}\int_{-\infty}^{x}\exp(-y^{2}/2)dy$ , the probability that a normal $N(0,1)$ has value less than x, then we can calculate that $V_{0}=V(s,T)$ , where 

## Black-Scholes formula

$$
V (s, T) = s \Phi \left(\frac {\log \frac {s}{k} + (r + \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}}\right) - k e ^ {- r T} \Phi \left(\frac {\log \frac {s}{k} + (r - \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}}\right).
$$

This is the Black–Scholes formula for pricing European call options. (Put options, the right to sell a unit of stock for k, can be priced as a call less a forward – put-call parity.) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/c194efba750b6735b4526d7e83d9b0cbc57aa91bd210caf3d68de635b0f8fec4.jpg)



Exercise 3.14 Find the change of variable and thus prove the Black–Scholes formula.


## 3.8 Black-Scholes in action

If a stock has a constant volatility of 18% and constant drift of 8%, with continuously compounded interest rates constant at 6%, what is the value of an option to buy the stock for $25 in two years time, given a current stock price of $20? 

The description fits the Black–Scholes conditions. Thus using s = 20, k = 25, σ = 0.18, r = 0.06, and t = 2, we can calculate $V_{0}$ as 1.221. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/267254b591b2f34a8c3654e8bcff1a0006f78ae252bec914cb368dcdef298704.jpg)


Exercise 3.15 What information about the drift was required? 

## Price dependence

For values of the current stock price s much smaller than the exercise price k, the value of the formula itself gets small, signifying that the option is out of the money and unlikely to recover in time. Conversely, for values of s much greater than k, the option loses most of its optionality, and becomes a forward. Correspondingly the option price is approximately $s - ke^{-rT}$ , which is the current value of a stock forward struck at price k for time T. 

## Time dependence

As the time to maturity T gets smaller, the chances of the price moving much more decreases and the option value gets closer and closer to the claim value taken at the current price, $(s - k)^{+}$ . 

For larger times, however, the option value gets larger. An option with almost infinite time to maturity would have value approaching s, as the cost now of price k is almost zero. It can be seen in figure 3.14 that as the time to expiration gets closer to zero, the curve gets closer to the option shape $(s - k)^{+}$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/30abbf4d3ef1499c958392424850e83dd8c41e33e9c355a78225c4e4222b9e70.jpg)



Figure 3.14 Option price against stock price for times 3, 1, and 0.3.
Exercise price k = $1, interest rate r = 0, volatility σ = 1.


## Volatility dependence

All else being equal, the option is worth more the more volatile the stock is. At one extreme, if $\sigma$ is very small, the option resembles a riskless bond and is just worth $(s - ke^{-rT})^{+}$ , which is the value of the corresponding forward if the option will be in the money and is zero otherwise. At the other extreme, if $\sigma$ is very large, the option is worth s. 

## American options

Sometimes an option has more optionality about it than just choosing between two alternatives at the maturity date. American options are the most well-known examples of such derivatives, giving the right to, say, purchase a unit of stock for a strike price k at any time up to and including the expiration date T, rather than only at that date. The buyer of the option then has to make decisions from moment to moment to decide when and if to call the option. 

The buyer of an American call has the choice when to stop, and that choice can only use price information up to the present moment. Such a (random) time is called a stopping time. Following a strategy which will result in exercising the option at the stopping time $\tau$ , the corresponding payoff is 

$$
(S _ {\tau} - k) ^ {+} \quad \text {   at   time   } \tau .
$$

If the option issuer knew in advance which stopping time the investor will 

use, the cost at time zero of hedging that payoff is 

$$
\mathbb {E} _ {\mathbb {Q}} \left(e ^ {- r \tau} (S _ {\tau} - k) ^ {+}\right).
$$

As we do not know which $\tau$ will be used, we have to prepare for the worst possible case, and charge the maximum value (maximised over all possible stopping strategies), 

$$
V _ {0} = \sup _ {\tau} \mathbb {E} _ {\mathbb {Q}} \left(e ^ {- r \tau} (S _ {\tau} - k) ^ {+}\right).
$$

## Pricing derivatives with optionality

In general, if the option purchaser has a set of options A, and receives a payoff $X_{a}$ at time T, after choosing a in A, then the option issuer should charge 

$$
V _ {0} = \sup _ {a \in A} \mathbb {E} _ {\mathbb {Q}} \left(e ^ {- r T} X _ {a}\right)
$$

for it. If the purchaser does not exercise the option optimally, then the issuer's hedge will produce a surplus by date T. 

## That hedge in full

Returning to the original European option, one thing that would be useful to know would be the actual replicating strategy required, that is, to actually find out how much stock would be required at each point of time to artificially construct the derivative. 

The amount of stock, $\phi_{t}$ , comes from the martingale representation theorem, but unfortunately, the theorem merely states that $\phi_{t}$ exists. However the martingale representation theorem, at heart, tells us that the reason that the discounted claim can be built from the discounted stock is that, being martingales under the same measure, one is locally just a scaled version of the other. The process $\phi_{t}$ is merely the ratio of volatilities. Thus, intuitively, if we looked at the ratio of the change in the value of the option caused by a move in the stock price and the change in the stock price used, this ought to be something like $\phi_{t}$ . And if we have a restricted enough claim where the only input required from the filtration for pricing the claim is the stock price at the current moment, and moreover that the functional relation implied by this between the value of the claim and the current stock price is 

## 3.8 Black-Scholes in action

smooth, then we could guess that the partial derivative of the option value with respect to the stock price is the $\phi_{t}$ we want. 

And so it is. For the often-encountered case where the claim depends only on the terminal value, the option value is a well-behaved function of the current stock price. Suppose the derivative X is a function of the terminal value of the stock price, so that $X = f(S_{T})$ for some function $f(s)$ . Then the following is true. 

## Terminal value pricing

If the derivative X equals $f(S_{T})$ , for some f, then in the value of the derivative at time t is equal to $V_{t} = V(S_{t}, t)$ , where $V(s, t)$ is given by the formula 

$$
V (s, t) = \exp (- r (T - t)) \mathbb {E} _ {\mathbb {Q}} \left(f \left(S _ {T}\right) \mid S _ {t} = s\right)
$$

And then the trading strategy is given by $\phi_t = \frac{\partial V}{\partial s}(S_t, t)$ . 

Why? Consider $dV_{t}$ , the infinitesimal change in the value of the option. Remembering that $dS_{t} = \sigma S_{t} d\tilde{W}_{t} + r S_{t} dt$ , then Itô gives us 

$$
d V _ {t} = d (V (S _ {t}, t)) = \left(\sigma S _ {t} \frac {\partial V}{\partial s}\right) d \tilde {W} _ {t} + \left(r S _ {t} \frac {\partial V}{\partial s} + \frac {1}{2} \sigma^ {2} S _ {t} ^ {2} \frac {\partial^ {2} V}{\partial s ^ {2}} + \frac {\partial V}{\partial t}\right) d t.
$$

But we also know that $dV_{t} = \phi_{t} dS_{t} + \psi_{t} dB_{t}$ , from the self-financing condition. And since $dB_{t} = rB_{t} dt$ we have 

$$
d V _ {t} = \left(\sigma S _ {t} \phi_ {t}\right) d \tilde {W} _ {t} + \left(r S _ {t} \phi_ {t} + r \psi_ {t} B _ {t}\right) d t.
$$

But SDE representations are unique - so the volatility terms must match, giving $\phi_t = \frac{\partial V}{\partial s}$ . The amount of stock in the replicating portfolio at any stage is the derivative of the option price with respect to the stock price. 

Using this substitution for $\phi_{t}$ and the fact that $V_{t}=S_{t}\phi_{t}+\psi_{t}B_{t}$ , we can also match the drift terms of the two SDEs to get a partial differential equation for V as 

$$
\frac {1}{2} \sigma^ {2} s ^ {2} \frac {\partial^ {2} V}{\partial s ^ {2}} + r s \frac {\partial V}{\partial s} - r V + \frac {\partial V}{\partial t} = 0.
$$

Notoriously, this PDE, coupled with the boundary condition that $V(s,T)$ must equal $f(s)$ , gives another way of solving the pricing equation. 

## Explicit Black-Scholes hedge

The call option is a terminal value claim, as described earlier, and so we can find an expression for the hedge itself. The amount of stock held is the derivative of the value function with respect to stock price. In symbols 

$$
\phi_ {t} = \frac {\partial V}{\partial s} (S _ {t}, T - t) = \Phi \left(\frac {\log \frac {S _ {t}}{k} + (r + \frac {1}{2} \sigma^ {2}) (T - t)}{\sigma \sqrt {T - t}}\right).
$$

Because $\phi$ is always between zero and one, we need only ever have a bounded long position in the stock. Also the value of the bond holding at any time is 

$$
B _ {t} \psi_ {t} = - k e ^ {- r (T - t)} \Phi \left(\frac {\log \frac {S _ {t}}{k} + (r - \frac {1}{2} \sigma^ {2}) (T - t)}{\sigma \sqrt {T - t}}\right),
$$

which, although always a borrowing, is bounded by the exercise price k. 

There are two possibilities as the time approaches maturity. If the option is out of the money, that is the stock price is less than the exercise price, then both the bond and the stock holding go to zero, reflecting the increasing worthlessness of the option. Alternatively, if the price stays above the exercise value, then the stock holding grows to one unit and the value of the bond to -k. This combination exactly balances the now certain demand for a unit of stock in return for cash amount k. 

## Example - hedging in continuous time

This can be seen operating in practice. Below are two possible realisations of a stock price which starts at $10. Both are exponential Brownian motions with volatility 20% and growth drift of 15%. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/1e989525308baac0b0b753fc3d0197bd3656ed5631143da5a5502b7a0615d7d9.jpg)



Figure 3.15a Stock price (A)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/22c71ab7b3ef85420c60cbab21ef8f9f87b2f54ac9022dc2d956feee805d14cf.jpg)



Figure 3.15b Stock price (B)


Let us price an option on this stock, to buy it at time T = 1 for the strike price of k = $12, assuming interest rates are 5%. We can calculate both the evolving worth of the option $V_{t}$ and the amount of stock to be held, $\phi_{t}$ , to hedge the contract. 

In the case (A), these processes are shown in figure 3.16. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/b47cbfb5e366552b7789f3e77915b3882ecd1f264622db2ba295821e7ae7a938.jpg)



Figure 3.16a Option value (A)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/901f8415a4a991405b12ffc41aebb76f1ffefc81b5792a3e411b5846c1380c8a.jpg)



Figure 3.16b Stock hedge (A)


As time progresses, the option becomes in the money and the option value moves like the stock price. Also the hedge gets closer and closer to one, signifying that the option will be exercised. 

In the case (B), these processes are shown in Figure 3.17. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/bd4ea1bf31ac5884b303b64dc9b312c5a5894fbe967ec15e5ef6467891767184.jpg)



Figure 3.17a Option value (B)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/55593062d237ea3deffcf60dca95649856dd844f7e7a91f29a0389e8123080e1.jpg)



Figure 3.17b Stock hedge (B)


This time the option is not exercised and both the value of it and the hedge go to zero over time. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/4b7bcaf4edbb021735d077fa4850a8623c79f14321fc976cd2598bcecec5e49d.jpg)


Exercise 3.16 A stock has current price $10 and moves as an exponential Brownian motion with upward drift of 15% a year (continuously compounded) and volatility of 20% a year. Current interest rates are constant at 5%. What is the value of an option on the stock for $12 in a year's time? 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/7aee29a86e10432c6fd3dfb0238d2840f44b2c02194895ce1eb30ef1607ad7c2.jpg)



Exercise 3.17 For the same stock, what is the value of a derivative which pays off $1 if the stock price is more than $10 in a year's time?


## Conclusions

Even with a respectable stochastic model for the stock, we can replicate any claim. Not something we had any right to expect. The replicating portfolio has a value given by the expected discounted claim, with respect to a measure which makes the discounted stock a martingale. Moreover, changing to the martingale measure has a remarkably simple effect on the process $S_{t}$ – only the drift changes, to another constant value. The stock remains an exponential Brownian motion; even the volatility $\sigma$ stays the same. 

These three surprises conspire to make the result look easier to get at than perhaps it really is. Something subtle and beautiful really is going on under all the formalism and the result only serves to obscure it. Before we push on, stop and admire the view. 

# Chapter 4 Pricing market securities

The Black–Scholes model we have seen so far has a simple mathematical side but it has an even simpler financial side. The asset we considered was a stock which could be held without additional cost or benefit and was freely tradable at the price quoted. Even leaving aside the issues of transaction costs and illiquidity, not much of the financial market is like that. Even vanilla products – foreign exchange, equities and bonds – don’t actually fit the simple asset class we devised. Foreign exchange involves two assets which pay interest, equities pay dividends, and bonds pay coupons. 

Just retreading the same mathematics for each of these will be enough to keep us busy. The sophistication we have to peddle now is financial. 

## 4.1 Foreign exchange

In the foreign exchange market, like the stock market, holding the basic asset, currency, is a risky business. The dollar value of, say, one pound sterling varies from moment to moment just as a US stock does. And with this risk comes demand for derivatives: claims based on the future value of one unit of currency in terms of another. 

## Forwards

Consider, though, a forward transaction: a dollar investor wanting to agree the cost in dollars of one pound at some future date T. As with stocks, the replicating strategy to guarantee the forward claim is static. We buy pounds now and sell dollars against them. But cash in both currencies attracts interest. And just as in the simple Black–Scholes model, our cash holding wasn't cash but a cash bond, so our cash holdings here will be cash bonds as well. 

Let's make things concrete. Suppose the constant dollar interest rate is $r$ , the sterling interest rate is $u$ , and $C_0$ dollars buy a pound now. Consider the following static replicating strategy. At time $t$ we 

- own $e^{-uT}$ units of sterling cash bonds, and 

- go short $C_0 e^{-uT}$ units of dollar cash bonds. 

At time zero the portfolio has nil value, and at time T the sterling holding will be one pound as required and the dollar short holding will be $C_{0}e^{(r-u)T}$ – the forward price we require. 

Contrast this with the stock forward price $S_{0}e^{rT}$ . We must be careful in extending our simple model to foreign exchange – both instruments now make payments. And that makes a difference. 

## Black-Scholes currency model

There are three instruments and processes to model – two local currency cash bonds and the exchange rate itself. Following the mathematical simplicity of Black–Scholes, our market will be: 

## Black-Scholes currency model

We let $B_{t}$ be the dollar cash bond, $D_{t}$ its sterling counterpart, and $C_{t}$ be the dollar worth of one pound. Then our model is 

Dollar bond 

$$
B _ {t} = e ^ {r t},
$$

Sterling bond 

$$
D _ {t} = e ^ {u t},
$$

Exchange rate 

$$
C _ {t} = C _ {0} \exp (\sigma W _ {t} + \mu t),
$$

for some $W_{t}$ a $\mathbb{P}$ -Brownian motion and constants $r, u, \sigma$ and $\mu$ . 

## 4.1 Foreign exchange

## The dollar investor

The underlying finance dictates that there are two tradables available to the dollar investor. One is uncomplicated – the dollar bond is straightforwardly a dollar tradable much as the cash bond was in the basic account of Black–Scholes. But the other is not. 

We would like to think of the stochastic process $C_t$ , the exchange rate, as a tradable but it isn't. The process $C_t$ represents the dollar value of one pound sterling, but sterling cash isn't a tradable instrument in our market. To hold cash naked would be to set up an arbitrage against the cash bond - to put it another way, the existence of the sterling cash bond $D_t$ sets an interest rate for sterling cash by arbitrage, and that rate is $u$ not zero. 

On the other hand, $D_{t}$ by itself isn't a dollar tradable either - it is the price of a tradable instrument, but it's a sterling price. 

Fortunately, the product of the two $S_{t} = C_{t}D_{t}$ is a dollar tradable. The dollar investor can hold sterling cash bonds, and the dollar value of the holding will be given by the translation of the sterling price $D_{t}$ into dollars, that is by multiplication by $C_{t}$ . 

Translation, then, yields two processes, $B_{t}$ and $S_{t}$ , which mirror the basic Black–Scholes set up. 

## Three steps to replication (foreign exchange)

(1) Find a measure $\mathbb{Q}$ under which the sterling bond discounted by the dollar bond $Z_{t} = B_{t}^{-1}S_{t} = B_{t}^{-1}C_{t}D_{t}$ is a martingale. 

(2) Form the process $E_{t} = \mathbb{E}_{\mathbb{Q}}\big(B_{T}^{-1}X\mid \mathcal{F}_{t}\big).$ 

(3) Find a previsible process $\phi_t$ , such that $dE_t = \phi_t dZ_t$ . 

## Step one

The dollar discounted worth of the sterling bond is 

$$
Z _ {t} = C _ {0} \exp (\sigma W _ {t} + (\mu + u - r) t).
$$

Can we make this into a martingale under some new measure Q? Only if $\tilde{W}_{t} = W_{t} + \sigma^{-1}(\mu + u - r + \frac{1}{2}\sigma^{2})t$ is a Q-Brownian motion, which is made possible as before by the Cameron–Martin–Girsanov theorem. Then, under Q 

$$
\begin{array}{l l} & Z _ {t} = C _ {0} \exp \left(\sigma \tilde {W} _ {t} - \frac {1}{2} \sigma^ {2} t\right), \\ \text { and   thus } & C _ {t} = C _ {0} \exp \left(\sigma \tilde {W} _ {t} + (r - u - \frac {1}{2} \sigma^ {2}) t\right). \end{array}
$$

## Step two

Given this Q, define the process $E_{t}$ to be the conditional expectation process $\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ , which as noted before is a Q-martingale. 

## Step three

The martingale representation theorem produces an $\mathcal{F}$ -previsible process $\phi_t$ linking $E_t$ with $Z_t$ , such that 

$$
E _ {t} = E _ {0} + \int_ {0} ^ {t} \phi_ {s} d Z _ {s}.
$$

Now where? We need a replicating strategy $(\phi_{t},\psi_{t})$ detailing holdings of our two dollar tradables $S_{t}$ and $B_{t}$ , so we try 

• holding $\phi_{t}$ units of sterling cash bond, and 

- holding $\psi_t = E_t - \phi_t Z_t$ units of dollar cash bond. 

The dollar value of the replicating portfolio at time t is $V_{t} = \phi_{t} S_{t} + \psi_{t} B_{t} = B_{t} E_{t}$ . This portfolio is only self-financing if changes in its value are only due to changes in the assets' prices, that is $dV_{t} = \phi_{t} dS_{t} + \psi_{t} dB_{t}$ , or as was shown to be equivalent in section 3.7, if $dE_{t} = \phi_{t} dZ_{t}$ – which is precisely what the martingale representation theorem guarantees. 

Since $V_{T} = B_{T}E_{T}$ , and $E_{T}$ is the discounted claim $B_{T}^{-1}X$ , we have a self-financing strategy $(\phi_{t}, \psi_{t})$ which replicates our arbitrary claim X. 

## Option price formula (foreign exchange)

All claims have arbitrage prices and those prices are given by the portfolio value 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right).
$$

where Q is the measure under which the discounted asset $Z_{t}$ is a martingale. 

## 4.1 Foreign exchange

## Example - forward contract

A sterling forward contract. At what price should we agree to trade sterling at a future date T? If we agree to buy a unit of sterling for an amount k of dollars, our payoff at time T is 

$$
X = C _ {T} - k.
$$

Its worth at time $t$ is $V_{t} = B_{t}\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ which is $e^{-r(T - t)}\mathbb{E}_{\mathbb{Q}}(C_T - k|\mathcal{F}_t)$ . So the forward price at time zero for purchasing sterling at time $T$ is $k = \mathbb{E}_{\mathbb{Q}}(C_T)$ or 

$$
F = \mathbb {E} _ {\mathbb {Q}} \left(C _ {0} \exp \left(\sigma \tilde {W} _ {T} + (r - u - \frac {1}{2} \sigma^ {2}) T\right)\right) = e ^ {(r - u) T} C _ {0}.
$$

That is, the current price for sterling discounted by a factor depending on the difference between the interest rates of the two currencies. With this strike, the contract's value at time t is 

$$
V _ {t} = e ^ {- u T} \left(e ^ {u t} C _ {t} - e ^ {r t} C _ {0}\right).
$$

The discounted portfolio value is $E_{t} = B_{t}^{-1}V_{t} = e^{-uT}Z_{t} - e^{-uT}C_{0}$ , thus $dE_{t} = e^{-uT}dZ_{t}$ , and so the required hedge $\phi_{t}$ is the constant $e^{-uT}$ , and $\psi_{t}$ is the constant $-e^{-uT}C_{0}$ . 

This confirms our earlier intuition. 

## Example - call option

A sterling call. Suppose we have a contract which allows us the option of buying a pound at time T in the future for the price of k dollars. The dollar payoff at time T is 

$$
X = (C _ {T} - k) ^ {+}.
$$

The value of the payoff at time t is $V_{t} = B_{t}\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ . Because $C_{T}$ is log-normally distributed we can evaluate this easily using a probabilistic result: 

## Log-normal call formula

If Z is a normal $N(0,1)$ random variable, and F, $\bar{\sigma}$ and k are constants, then 

$$
\mathbb {E} \left(\left(F \exp \left(\bar {\sigma} Z - \frac {1}{2} \bar {\sigma} ^ {2}\right) - k\right) ^ {+}\right) = F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \bar {\sigma} ^ {2}}{\bar {\sigma}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \bar {\sigma} ^ {2}}{\bar {\sigma}}\right).
$$

As the forward price $F$ is $\mathbb{E}_{\mathbb{Q}}(C_T)$ , the value of $C_T$ can be written in the form $F \exp(\bar{\sigma}Z - \frac{1}{2}\bar{\sigma}^2)$ , where $\bar{\sigma}^2$ is the variance of $\log C_T$ , namely $\sigma^2T$ , and $Z$ is a normal $N(0,1)$ under $\mathbb{Q}$ . 

The option price at time zero is then $\mathbb{E}\big(\big(F\exp(\bar{\sigma}Z-\frac{1}{2}\bar{\sigma}^{2})-k\big)^{+}\big)$ , which the theorem tells us is 

$$
V _ {0} = e ^ {- r T} \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) \right\}.
$$

The hedge is 

$$
\phi_ {t} = e ^ {- u T} \Phi \left(\frac {\log \frac {F _ {t}}{k} + \frac {1}{2} \sigma^ {2} (T - t)}{\sigma \sqrt {T - t}}\right),
$$

$$
\psi_ {t} = - k e ^ {- r T} \Phi \left(\frac {\log \frac {F _ {t}}{k} - \frac {1}{2} \sigma^ {2} (T - t)}{\sigma \sqrt {T - t}}\right),
$$

where $F_{t}$ is the forward sterling price at time $t$ , $F_{t} = e^{(r - u)(T - t)}C_{t}$ . 

## The sterling investor

A sterling investor sees things differently. Were we operating in pounds we would not be wanting dollar price processes of tradable instruments but sterling ones. The first of these is simply the sterling bond $D_{t} = e^{ut}$ , which will be our basic unit of account. There is also the inverse exchange rate process $C_{t}^{-1}$ – the worth in pounds of one dollar. This has the value 

$$
C _ {t} ^ {- 1} = C _ {0} ^ {- 1} \exp (- \sigma W _ {t} - \mu t),
$$

but it is not the sterling price of a tradable instrument, any more than $C_{t}$ was for the dollar investor. Our other actual sterling tradable price process is the sterling value of the dollar bond $C_{t}^{-1}B_{t}$ . 

With our two sterling tradable prices, $D_{t}$ and $C_{t}^{-1}B_{t}$ , we can follow again our three-step replication programme. The sterling discounted value of the dollar bond is 

$$
Y _ {t} = D _ {t} ^ {- 1} C _ {t} ^ {- 1} B _ {t} = C _ {0} ^ {- 1} \exp (- \sigma W _ {t} - (\mu + u - r) t).
$$

This discounted price process $Y_{t}$ will be a martingale under the new measure $\mathbb{Q}^{\mathcal{L}}$ , if 

$$
\tilde {W} _ {t} ^ {\mathcal {L}} = W _ {t} + \sigma^ {- 1} (\mu + u - r - \frac {1}{2} \sigma^ {2}) t
$$

## 4.1 Foreign exchange

is $\mathbb{Q}^{\mathcal{L}}$ -Brownian motion. Then hedging will be possible as before. 

## Option price formula (sterling investor)

The value to the sterling investor of a sterling payoff X at time T is 

$$
U _ {t} = D _ {t} \mathbb {E} _ {\mathbb {Q} \not \in} \big (D _ {T} ^ {- 1} X \mid \mathcal {F} _ {t} \big).
$$

where $Q^{L}$ is the measure under which the sterling discounted asset $Y_{t}$ is a martingale. 

## Change of numeraire

A worrying possibility now surfaces – the measures Q and $Q^{L}$ are different. Will the dollar and sterling investors disagree about the price of the same security? 

Suppose X is a dollar claim which pays off at time T. To the dollar investor, the claim is worth at time t 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right) \quad \text { dollars }.
$$

To the sterling investor, the claim pays off $C_{T}^{-1}X$ pounds, rather than X dollars, at time T, and its sterling worth at time t is 

$$
U _ {t} = D _ {t} \mathbb {E} _ {\mathbb {Q L}} \left(D _ {T} ^ {- 1} (C _ {T} ^ {- 1} X) \mid \mathcal {F} _ {t}\right) \quad \text { pounds }.
$$

Do these two prices agree? That is, is the dollar worth of the sterling valuation, $C_{t}U_{t}$ , the same as the original dollar valuation $V_{t}$ ? 

The $\mathbb{Q}^{\mathcal{L}}$ -Brownian motion $\tilde{W}_t^{\mathcal{L}}$ is equal to $\tilde{W}_t - \sigma t$ , so that by the converse of the Cameron-Martin-Girsanov theorem the Radon-Nikodym derivative of $\mathbb{Q}^{\mathcal{L}}$ with respect to $\mathbb{Q}$ (up to time $T$ ) must be 

$$
\frac {d \mathbb {Q} ^ {\mathcal {L}}}{d \mathbb {Q}} = \exp \left(\sigma \tilde {W} _ {T} - \frac {1}{2} \sigma^ {2} T\right).
$$

The Q-martingale associated with the Radon–Nikodym derivative, formed by conditional expectation is 

$$
\zeta_ {t} = \mathbb {E} _ {\mathbb {Q}} \left(\frac {d \mathbb {Q} ^ {\mathcal {L}}}{d \mathbb {Q}} \mid \mathcal {F} _ {t}\right) = \exp (\sigma \tilde {W} _ {t} - \frac {1}{2} \sigma^ {2} t).
$$

Note that $\zeta_{t}$ is (up to a constant) the dollar discounted worth of the sterling bond. Concretely, $C_{0}\zeta_{t}=Z_{t}=B_{t}^{-1}C_{t}D_{t}$ . Recall also (Radon–Nikodym fact (ii) of section 3.4) that for any random variable X which is known by time T, 

$$
\mathbb {E} _ {\mathbb {Q} \mathscr {L}} (X | \mathcal {F} _ {t}) = \zeta_ {t} ^ {- 1} \mathbb {E} _ {\mathbb {Q}} (\zeta_ {T} X | \mathcal {F} _ {t}).
$$

So the dollar worth of the sterling investor's valuation is 

$$
C _ {t} U _ {t} = C _ {t} D _ {t} \mathbb {E} _ {\mathbb {Q} \mathscr {L}} \left(D _ {T} ^ {- 1} C _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right) = C _ {t} D _ {t} \zeta_ {t} ^ {- 1} \mathbb {E} _ {\mathbb {Q}} \left(\zeta_ {T} D _ {T} ^ {- 1} C _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right),
$$

which is (substituting in the $\zeta_{t}$ expression) equal to 

$$
C _ {t} U _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right) = V _ {t}.
$$

Thus the payoff of X dollars at time T is worth the same to either investor at any time beforehand. Similar calculations show that the dollar and sterling investors' replicating strategies for X are identical. So they agree not only on the prices but also on the hedging strategy. 

The difference of martingale measures only reflected the different numeraires of the two investors rather than any fundamental disagreement over prices. Further details on the effect, or lack of it, of changing numeraires are in section 6.4. 

All investors, whatever their currency of account, will agree on the current value of a derivative or other security. 

## 4.2 Equities and dividends

An equity is a stock which makes periodic cash payments to the current holder. Our previous models treated a stock as a pure asset, but they can be modified to handle dividend payments. 

It is simplest to begin with a dividend which is paid continuously. 

## Equity model with continuous dividends

Let the stock price $S_{t}$ follow a Black–Scholes model, $S_{t} = S_{0} \exp(\sigma W_{t} + \mu t)$ and $B_{t}$ be a constant-rate cash bond $B_{t} = \exp(rt)$ . The dividend payment made in the time interval of length dt starting at time t is 

$$
\delta S _ {t} d t,
$$

where $\delta$ is a constant of proportionality. 

Just as with foreign exchange, our problem is that the process $S_{t}$ is not a tradable asset. If we buy the stock for $S_{0}$ , by the time we come to sell it at time t, what we bought is worth not just the price of the stock itself, namely $S_{t}$ , but also the total accumulated dividends, which under the model will depend on all the different values that the stock has taken up until time t. The process $S_{t}$ is no longer the value of the asset as a whole, because it is not enough. 

We need to translate $S_{t}$ somehow, and to find a new process as we did in foreign exchange, which involves $S_{t}$ but is a tradable. Consider the following simple portfolio strategy. The portfolio starts with one unit of stock, costing $S_{0}$ , and at every instant when the cash dividend is paid out, that cash is immediately used to buy a little more stock. That is, we are continuously reinvesting the dividends in the stock. The infinitesimal payout is $\delta S_{t} dt$ per unit of stock, which will purchase $\delta dt$ more units of stock. At time t, the number of stock units held by the portfolio will be $\exp(\delta t)$ , and the worth of the portfolio is 

$$
\tilde {S} _ {t} = S _ {0} \exp (\sigma W _ {t} + (\mu + \delta) t).
$$

Note how the structure of the model's assumptions made the translation straightforward. We assumed that the dividend payments were a constant proportion of the stock price. As a consequence it made it natural to construct the tradable by reinvesting in the stock. If we had assumed that the dividend stream was known in advance, independent of the stock price, then we would have reinvested in the cash bond (for an example of this see section 4.3 on bonds). Assumptions are all. 

## Replicating strategies - equities

Our definition of a portfolio of stock and bond $(\phi_{t},\psi_{t})$ can be rewritten as a portfolio of the reinvested stock and bond $(\tilde{\phi}_{t},\psi_{t})$ , where $\tilde{\phi}_{t}=e^{-\delta t}\phi_{t}$ , with value $V_{t}=\phi_{t}S_{t}+\psi_{t}B_{t}=\tilde{\phi}_{t}\tilde{S}_{t}+\psi_{t}B_{t}$ . The advantage of the new framework is that the self-financing equation retains the familiar form 

$$
d V _ {t} = \tilde {\phi} _ {t} d \tilde {S} _ {t} + \psi_ {t} d B _ {t},
$$

whereas in the plain stock/bond notation, this equation would need to be modified by the dividend cash stream, becoming $dV_{t} = \phi_{t} dS_{t} + \psi_{t} dB_{t} + \phi_{t} \delta S_{t} dt$ . That is, changes in the portfolio value are due both to trading profits and losses (the $dS_{t}$ and $dB_{t}$ terms) and also to dividend payments. 

Working now with our reinvested stock, as usual we want to make the discounted asset $\tilde{Z}_{t}=B_{t}^{-1}\tilde{S}_{t}$ into a martingale. Now $\tilde{Z}_{t}$ has SDE 

$$
d \tilde {Z} _ {t} = \tilde {Z} _ {t} \left(\sigma d W _ {t} + (\mu + \delta + \frac {1}{2} \sigma^ {2} - r) d t\right),
$$

so that we want a measure Q under which $\tilde{W}_{t}=W_{t}+\sigma^{-1}(\mu+\delta+\frac{1}{2}\sigma^{2}-r)t$ is Brownian motion. So under this martingale measure Q, $d\tilde{Z}_{t}=\sigma\tilde{Z}_{t}d\tilde{W}_{t}$ . To construct a strategy to hedge a claim X maturing at date T, again we follow the simple Black–Scholes model, and use the martingale representation theorem. That is, there exists a previsible process $\tilde{\phi}_{t}$ such that 

$$
E _ {t} = \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t} \big) = \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} X \big) + \int_ {0} ^ {t} \tilde {\phi} _ {s} d \tilde {Z} _ {s}.
$$

The trading strategy is to hold $\tilde{\phi}_{t}$ units of the translated asset $\tilde{S}_{t}$ and $\psi_{t}=E_{t}-\tilde{\phi}_{t}\tilde{Z}_{t}$ units of the cash bond. In terms of our original securities, this amounts to holding $\phi_{t}=e^{\delta t}\tilde{\phi}_{t}$ units of the stock $S_{t}$ and the same $\psi_{t}$ units of the bond $B_{t}$ . 

Thus, under the martingale measure 

$$
S _ {t} = S _ {0} \exp \left(\sigma \tilde {W} _ {t} + (r - \delta - \frac {1}{2} \sigma^ {2}) t\right),
$$

which is log-normally distributed. 

## 4.2 Equities and dividends

## Example - forward

An agreement to buy a unit of stock at time T for amount k has payoff 

$$
X = S _ {T} - k.
$$

Its worth at time t is 

$$
V _ {t} = \mathbb {E} _ {\mathbb {Q}} \left(e ^ {- r (T - t)} \left(S _ {T} - k\right) \mid \mathcal {F} _ {t}\right) = e ^ {- \delta (T - t)} S _ {t} - e ^ {- r (T - t)} k.
$$

The value of k which gives the contract initial nil value is the forward price of $S_{T}$ , 

$$
F = e ^ {(r - \delta) T} S _ {0}.
$$

The hedge is then to hold $\phi_{t}=e^{-\delta(T-t)}$ units of the stock and $\psi_{t}=-ke^{-rT}$ units of the bond at time t. Note the slightly surprising dynamic strategy for the forward. Instead of simply holding a certain amount of stock until T, we are continually buying more with the dividend income. Why? Again because of our assumption – if the dividend payments are a known proportion of the stochastic $S_{t}$ , we have no choice but to hide them in the stock itself. 

## Example - call option

A call struck at k, exercised at time T has payoff $X = (S_{T} - k)^{+}$ , and value at time zero of $V_{0} = \mathbb{E}_{\mathbb{Q}} \left( e^{-rT}(S_{T} - k)^{+} \right)$ , which equals 

$$
V _ {0} = e ^ {- r T} \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) \right\},
$$

where F is the forward price above $e^{(r-\delta)T}S_{0}$ . The hedge will be to hold $e^{-\delta(T-t)}\Phi(+)$ units of the stock and have a negative holding of $ke^{-rT}\Phi(-)$ units of the bond. (Here $\Phi(+)$ and $\Phi(-)$ refer respectively to the two $\Phi$ terms in the above equation.) 

Again the Black–Scholes call option formula re-emerges – if the martingale measure Q makes the process under study, $S_{t}$ , have a log-normal distribution, then the theorem in section 4.1 comes into play. Knowing the forward F and the term volatility $\sigma$ is enough to specify the price. 

## Example - guaranteed equity profits

A contract pays off according to gains of the UK FTSE stock index $S_{t}$ , with a guaranteed minimum payout and a maximum payout. More precisely, it is a five-year contract which pays out 90% times the ratio of the terminal and initial values of FTSE. Or it pays out 130% if otherwise it would be less, or 180% if otherwise it would be more. How much is this payout worth? 

Our data are 

$$
\mathrm{FTSE} \mathrm{drift} \quad \mu = 7
$$

$$
\text { FTSE   volatility } \quad \sigma = 15 \%
$$

$$
\text { FTSE   dividend   yield } \quad \delta = 4 \%
$$

$$
\text { UK   interest   rate } \quad r = 6.5 \%
$$

As FTSE is composed of 100 different stocks, their separate dividend payments will approximate a continuously paying stream. The claim X is 

$$
X = \min \left\{\max \{1. 3, 0. 9 S _ {T} \}, 1. 8 \right\},
$$

where T is 5 years and the initial FTSE value $S_{0}$ is 1. This claim can be rewritten as 

$$
X = 1. 3 + 0. 9 \left\{\left(S _ {T} - 1. 4 4 4\right) ^ {+} - \left(S _ {T} - 2\right) ^ {+} \right\}.
$$

That is, X is actually the difference of two FTSE calls (plus some cash). The forward price for $S_{T}$ is 

$$
F = e ^ {(r - \delta) T} S _ {0} = 1. 1 3 3.
$$

Using the above call price formula for dividend-paying stocks, we can value these calls (per unit) at 0.0422 and 0.0067 respectively. The worth of X at time zero is then 

$$
V _ {0} = 1. 3 e ^ {- r T} + 0. 9 (0. 0 4 2 2 - 0. 0 0 6 7) = 0. 9 7 1 2.
$$

Were we to have forgotten that the constituent stocks of FTSE pay dividends, but the dividends are not reflected in the index, we would incorrectly have valued the contract at 1.0183 – about 5% too high. 

## 4.2 Equities and dividends

## Periodic dividends

In practice, an individual stock pays dividends at regular intervals rather than continuously, but this presents no real problems for our basic model. Let us assume that the times of dividend payments $T_{1}, T_{2}, \ldots$ are known in advance, and at each time $T_{i}$ , the current holder of the equity receives a payment of a fraction $\delta$ of the current stock price. The stock price must also instantaneously decrease by the same amount – or else there would be an arbitrage opportunity. At any time $T = T_{i}$ , then, we can assume the dividend payout exactly equals the instantaneous decrease in the stock price. 

## Equity model with periodic dividends

At deterministic times $T_{1}, T_{2}, \ldots$ , the equity pays a dividend of a fraction $\delta$ of the stock price which was current just before the dividend is paid. The stock price process itself is modelled as 

$$
S _ {t} = S _ {0} (1 - \delta) ^ {n [ t ]} \exp (\sigma W _ {t} + \mu t),
$$

where $n[t] = \max\{i : T_i \leqslant t\}$ is the number of dividend payments made by time t. There is also a cash bond $B_t = \exp(rt)$ . 

We face two problems. The first is the familiar one that $S_{t}$ is not by itself the price of tradable asset. Translation, however, should provide a cure. The second is more serious. Away from the times $T_{i}, S_{t}$ has the usual SDE of $dS_{t} = S_{t}\left(\sigma dW_{t} + (\mu + \frac{1}{2}\sigma^{2})dt\right)$ , but at those times it has discontinuous jumps. Thus $S_{t}$ is discontinuous - it doesn't fit our definition of a stochastic process. Fortunately, translation cures this as well. 

Consider the following trading strategy. Starting with one unit of stock, every time the stock pays a dividend we reinvest the dividend by buying more stock. At time t, we will have $(1 - \delta)^{-n[t]}$ units of the stock, and the value of our portfolio will be $\tilde{S}_{t}$ , where 

$$
\tilde {S} _ {t} = (1 - \delta) ^ {- n [ t ]} S _ {t} = S _ {0} \exp (\sigma W _ {t} + \mu t).
$$

As before, $\tilde{S}_{t}$ is tradable but our arbitrage justified assumption that the dividend payments match the stock price jumps feeds through into making $\tilde{S}_{t}$ continuous as well. We are back in familiar territory. 

## Replicating strategy

Our trading strategy will then be $(\tilde{\phi}_{t},\psi_{t})$ , where $\tilde{\phi}_{t}$ is the number of units of $\tilde{S}_{t}$ we hold at time t, and $\psi_{t}$ is the amount of the cash bond $B_{t}$ . Such a strategy is equivalent to holding $\phi_{t}=(1-\delta)^{-n[t]}\tilde{\phi}_{t}$ units of the actual stock $S_{t}$ . 

The discounted value of the $(\tilde{\phi}_{t},\psi_{t})$ portfolio is $E_{t}=\tilde{\phi}_{t}\tilde{Z}_{t}+\psi_{t}$ , where $\tilde{Z}_{t}$ is the discounted value of the reinvested stock price $\tilde{Z}_{t}=B_{t}^{-1}\tilde{S}_{t}$ . The portfolio will be self-financing if $dE_{t}=\tilde{\phi}_{t}d\tilde{Z}_{t}$ . 

As before, we want to find a $\mathbb{Q}$ which makes $\tilde{Z}_t$ into a martingale. As $d\tilde{Z}_t = \tilde{Z}_t\big(\sigma dW_t + (\mu + \frac{1}{2}\sigma^2 - r)dt\big)$ , this will have no drift if $\tilde{W}_t = W_t + \sigma^{-1}(\mu + \frac{1}{2}\sigma^2 - r)t$ is $\mathbb{Q}$ -Brownian motion. Then $\tilde{Z}_t$ is also a $\mathbb{Q}$ -martingale. 

We can form the process $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ , where X is the option on the stock which we wish to hedge. 

Finally, the martingale representation theorem produces a hedging process $\tilde{\phi}_{t}$ and the corresponding $\psi_{t}$ can be set to be $E_{t}-\tilde{\phi}_{t}\tilde{Z}_{t}$ . So hedging is still possible in this case, and the value at time zero of the claim X is $\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X)$ . 

The stock price, under $\mathbb{Q}$ , is 

$$
S _ {t} = S _ {0} (1 - \delta) ^ {n [ t ]} e ^ {\sigma \tilde {W} _ {t} + (r - \frac {1}{2} \sigma^ {2}) t}.
$$

Since this is log-normal, with the forward price for $S_T$ equal to $F = S_0(1 - \delta)^{n[T]} e^{rT}$ , the Black-Scholes price for a call option struck at $k$ is equal to 

$$
V _ {0} = e ^ {- r T} \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) \right\}.
$$

## 4.3 Bonds

A pure discount bond is a security which pays off one unit at some future maturity time T. Were interest rates completely constant at rate r it would have present value at time t of $e^{-r(T-t)}$ . We might, however, want to consider the effect of interest rates being stochastic – much as they are in real markets. And with varying interest rates, uncertainty about their future values would cause a discount bond price to move randomly as well. 

## 4.3 Bonds

A full model of discount bonds, or for that matter coupon bonds, will have to wait for chapter five and term structure models. The interplay of interest rates of different maturities and the arbitrage minefield that models have to tiptoe through is not something we want to worry about in a simple Black–Scholes account. As a consequence we will try to take a schizophrenic attitude to interest rates. Bond prices will vary stochastically, but the short-term interest rate will be deterministic. In the real markets there is clearly a link, but then it can be argued that there are links between stock or foreign exchange prices and the cash bonds as well. Over short time horizons most practitioners ignore these links in all three markets. 

## Discount bonds

The Black–Scholes model for discount bonds is: 

## Discount bond model

We assume a cash bond $B_{t} = \exp(rt)$ for some positive constant r, and a discount bond $S_{t}$ whose price follows 

$$
S _ {t} = S _ {0} \exp (\sigma W _ {t} + \mu t),
$$

for all times t less than T, some time horizon T long before the maturity time $\tau$ of the bond. 

In formulation, this model is indistinguishable from the simple Black-Scholes model for stocks. Thus the forward price for purchasing the bond at time $T < \tau$ is 

$$
F = \mathbb {E} _ {\mathbb {Q}} (S _ {T}),
$$

where Q is the measure under which $e^{-rt}S_{t}$ is a martingale. Since $\sigma^{2}T$ is the variance, under Q, of $\log S_{T}$ ( $\sigma$ is the term volatility), then the price of a call on $S_{T}$ struck at k is 

$$
e ^ {- r T} \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) \right\}.
$$

We have to be careful, though, with our assumption that T is much before the maturity $\tau$ . Not only does the distinction between the deterministic cash bond and the stochastic discount bond get harder to maintain as T approaches $\tau$ , but for similar reasons it gets harder to justify a simple drift $\mu$ and a constant positive $\sigma$ . The bond promises one unit at time $\tau$ , thus its price at time $\tau$ must be $S_{\tau} = 1$ . In a good model, the drift and volatility will conspire to ensure this pull to par – and indeed this will happen in chapter five. Here if we let $T = \tau$ , we would have no such guarantee. 

## Bonds with coupons

Most market bonds do not just pay off one unit at maturity, but also pay off a series of smaller amounts c at various pre-determined times $T_{1}, T_{2}, \ldots, T_{n}$ before maturity. Such coupon payments may resemble dividend payments, but unlike the equity model, the amount of the coupon is known in advance. Here the schizophrenia extends to the treatment of coupons before and after the expiry date, T, of the option. The simplest model is to view coupons that occur before time T as coming under the regime of the deterministic cash bond, and coupons occurring after time T (including the redemption payment at maturity) as following a stochastic price process. 

## Coupon bond model

There is a simple cash bond $B_{t} = \exp(rt)$ , and a coupon bond which pays off an amount c at times $T_{1}, T_{2}, \ldots$ , up to a horizon $\tau$ . Denoting $I(t) = \min\{i : t < T_{i}\}$ to be the sequence number of the next coupon payment after time t, and j to be $I(T) - 1$ , the total number of payments before time T, then the price of the bond at time t is then 

$$
S _ {t} = \sum_ {i = I (t)} ^ {j} c e ^ {- r (T _ {i} - t)} + A \exp (\sigma W _ {t} + \mu t), \quad t <   T.
$$

Specifically, we model the first sort of coupon (payable at, for example, $T_{i} < T$ ) to be worth 

$$
c e ^ {- r (T _ {i} - t)} \quad \text {   at   time   } t (t <   T _ {i}),
$$

and for the sum of all the post-T payments to evolve as an exponential 

## 4.3 Bonds

Brownian motion 

$$
A \exp (\sigma W _ {t} + \mu t), \quad \text { for } t <   T,
$$

for constants $A, \sigma$ , and $\mu$ . 

Again $S_{t}$ is discontinuous at the coupon payment times, and again we can use a translation rather like the one used for equity dividends (section 4.2). But because the coupon payments are known in advance, this time we manufacture a continuous tradable asset by holding one unit of the coupon bond and investing all the coupon payments, as they occur, in the cash bond. The value of this asset is $\tilde{S}_{t}$ , where 

$$
\tilde {S} _ {t} = \sum_ {i = 1} ^ {j} c e ^ {- r (T _ {i} - t)} + A \exp (\sigma W _ {t} + \mu t).
$$

This is now a tradable asset with a continuous stochastic process. 

## Replicating strategy

We describe a portfolio as $(\tilde{\phi}_{t},\psi_{t})$ , where $\tilde{\phi}_{t}$ is the amount of the asset $\tilde{S}_{t}$ held at time t, and $\psi_{t}$ is the direct holding of the cash bond $B_{t}=e^{rt}$ . We let $V_{t}$ be the value of the portfolio, $V_{t}=\tilde{\phi}_{t}\tilde{S}_{t}+\psi_{t}B_{t}$ , and $E_{t}$ be its discounted value $E_{t}=\tilde{\phi}_{t}\tilde{Z}_{t}+\psi_{t}$ , where $\tilde{Z}_{t}$ is the discounted value of the asset $\tilde{S}_{t}$ . The portfolio is self-financing if $dE_{t}=\tilde{\phi}_{t}d\tilde{Z}_{t}$ . 

As usual, we want to make $\tilde{Z}_{t}$ into a martingale by changing measure. In fact $\tilde{Z}_{t}$ is just a constant cash sum of $\sum_{i=1}^{j}ce^{-rT_{i}}$ plus an exponential Brownian motion $A\exp\left(\sigma W_{t}+(\mu-r)t\right)$ . This will be a Q-martingale if $\tilde{W}_{t}=W_{t}+\sigma^{-1}(\mu+\frac{1}{2}\sigma^{2}-r)t$ is Q-Brownian motion. 

For an option X payable at time T, the process $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ can be represented as $dE_{t} = \tilde{\phi}_{t} d\tilde{Z}_{t}$ for some previsible process $\tilde{\phi}_{t}$ . We can set $\psi_{t}$ to be $E_{t} - \tilde{\phi}_{t}\tilde{Z}_{t}$ , so that $(\tilde{\phi}_{t}, \psi_{t})$ is a hedging strategy for X. The value of X at time zero must now be $\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X)$ . 

Under $\mathbb{Q}$ , the price of the bond at time $T$ is just 

$$
S _ {T} = A \exp \left(\sigma \tilde {W} _ {T} + (r - \frac {1}{2} \sigma^ {2}) T\right).
$$

This is log-normally distributed, so we can follow the call formula from section 4.1 to see that the forward price for $S_T$ is $F = Ae^{rT}$ and the value of a call on $S_T$ struck at $k$ is 

$$
e ^ {- r T} \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) \right\}.
$$

# Pricing market securities

## 4.4 Market price of risk

Now is the time to tie some loose ends together. The same pattern has been repeating through all the examples so far – the stochastic processes we have been using as models in this chapter have been tied to tradable quantities only indirectly. The foreign exchange process had to be converted from a non-tradable cash process to a tradable discount bond process. For equities, the model process had to have dividends recombined to make it tradable. And for bonds, the coupons had to be reinvested in the numeraire process. Underlying all this was a tradable/non-tradable distinction – we couldn't use the martingale representation theorem to replicate claims until we had something tradable to replicate with. But the distinction has so far been a common sense one – can we do any better? 

To some extent, yes. Some of the tradable/non-tradable distinction is going to have to be founded on goodwill. After all whether something can be traded or not in a free market is not a mathematical decision. But if we decide on a particular process $S_{t}$ representing something truly tradable and select an appropriate discounting process $B_{t}$ , then we can explore the market they create. 

## Martingales are tradables

Suppose that there is some measure Q under which the discounted tradable, $Z_{t} = B_{t}^{-1}S_{t}$ , is a Q-martingale, what can we say about another process $V_{t}$ adapted to the same filtration $F_{t}$ such that $E_{t} = B_{t}^{-1}V_{t}$ is also a Q-martingale? 

Firstly, the martingale representation theorem gives us that, as long as $Z_{t}$ has non-zero volatility, we can find an F-previsible process $\phi_{t}$ such that 

$$
d E _ {t} = \phi_ {t} d Z _ {t}.
$$

Taking our cue from all the examples so far, we could create a portfolio $(\phi_{t}, \psi_{t})$ where at time t we are 

- long $\phi_t$ of the tradable $S_t$ , 

- long $\psi_t = E_t - \phi_t Z_t$ of the tradable $B_t$ . 

Then as before we can show that $(\phi_{t},\psi_{t})$ is a self-financing strategy, that is changes in the value of the $(\phi_{t},\psi_{t})$ portfolio are explainable in terms of 

## 4.4 Market price of risk

changes in value of the tradable constituents alone. And the value of this portfolio at time t is always exactly $V_{t}$ . 

In other words we can make $V_{t}$ out of $S_{t}$ and $B_{t}$ . So it seems reasonable enough to ennoble $V_{t}$ with the title tradable as well. Being a Q-martingale after discounting is enough to ensure that it can be made costlessly from tradables – so it might as well be tradable itself. Of course all the derivatives that we have been constructing out of claims have this property $-\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ is always a Q-martingale. 

## Non-martingales are non-tradables

What about the other way round? Suppose $B_{t}^{-1}V_{t}$ was not a Q-martingale. Then from our definition of a martingale, there must be a positive probability at some times T and s that $\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}V_{T}|\mathcal{F}_{s}) \neq B_{s}^{-1}V_{s}$ . What would happen if $V_{t}$ were tradable and the market stumbled into this possible filtration? 

Suppose we define another process $U_{t}$ by simply setting $U_{t}$ to be the cost of replicating the claim $V_{T}$ , that is $U_{t} = B_{t} \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1} V_{T} | \mathcal{F}_{t})$ . Then the terminal value of $U_{T}$ will be equal to $V_{T}$ but at time s, $U_{s}$ and $V_{s}$ will be (possibly) different. As $B_{t}^{-1} U_{t}$ is a Q-martingale we can view $U_{t}$ as tradable by dint of being able to construct it from $S_{t}$ and $B_{t}$ . 

So we have two tradables, $U_{t}$ and $V_{t}$ , such that they are identical at time T but different at some earlier time s (with positive probability). We then have an arbitrage engine. If, say, $U_{s}$ were greater than $V_{s}$ , we could buy unlimited amounts of V and sell unlimited amounts of U collecting the cash up front. The V - U portfolio can be sold for nothing at time T, leaving just the (invested) cash as a guaranteed profit. And if $U_{s}$ were less than $V_{s}$ we would run the engine in reverse. 

Thus if $V_{t}$ were genuinely tradable, the market formed by $S_{t}$ , $B_{t}$ and $V_{t}$ would contain arbitrage opportunities – something we might want to dismiss by fiat. To avoid arbitrage engines, then, if $B_{t}^{-1}V_{t}$ were not a Q-martingale, it had better not be tradable. 

We have something akin to a definition then. Within an established (complete) market of tradable securities, there is a straightforward way of checking whether another process is a tradable security or not. It is tradable if its discounted price is a martingale under the martingale measure Q, and is not tradable if it isn't. 

# Pricing market securities

## Tradable securities

Given a numeraire $B_{t}$ and a tradable asset $S_{t}$ , a process $V_{t}$ represents a tradable asset if and only if its discounted value $B_{t}^{-1}V_{t}$ is actually a Q-martingale, where Q is the measure under which the discounted asset, $B_{t}^{-1}S_{t}$ , is a martingale. 

One way round, the process is just part of the 'linear span' of $S_{t}$ and $B_{t}$ ; the other way round, there is only room for two 'independent' tradables in a market defined by one-dimensional Brownian motion - any more and there can be arbitrage. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/b7e65a23e7e031cdca608f7c5b6e7138aa7e89d9d0fd68301d78db7e8f8b596e.jpg)


Exercise 4.1 If $S_{t}$ is a tradable Black-Scholes stock price under the martingale measure $\mathbb{Q}$ , $S_{t} = \exp\big(\sigma \tilde{W}_{t} + (r - \frac{1}{2}\sigma^{2})t\big)$ , with cash bond $B_{t} = \exp(rt)$ , show that 

(i) $X_{t} = S_{t}^{2}$ is non-tradable, 

(ii) $X_{t} = S_{t}^{-\alpha}$ , where $\alpha = 2r / \sigma^2$ , is tradable. 

## Tradables and the market price of risk

The market price of risk is best introduced through a slight modification of the simple Black–Scholes model. That model had stock price $S_{t} = S_{0} \exp(\sigma W_{t} + \mu t)$ , and SDE 

$$
d S _ {t} = S _ {t} \left(\sigma d W _ {t} + \left(\mu + \frac {1}{2} \sigma^ {2}\right) d t\right).
$$

We will find it convenient, however, to define price processes by means of their SDEs, typically 

$$
d S _ {t} = S _ {t} \left(\sigma d W _ {t} + \mu d t\right),
$$

which has solution $S_{t} = S_{0} \exp(\sigma W_{t} + (\mu - \frac{1}{2}\sigma^{2})t)$ . The only difference between these two approaches is the subtraction of $\frac{1}{2}\sigma^{2}$ from the drift, which can be thought of as just a change of notation. Both forms can be equally used to define such geometric Brownian motions, but the SDE formulation allows a greater general class of models to be more easily considered. 

Suppose then that we have a couple of tradable risky securities $S_{t}^{1}$ and $S_{t}^{2}$ , both in the same market – that is both are functions of the same Brownian motion $W_{t}$ , and both are defined via their SDEs, 

$$
d S _ {t} ^ {i} = S _ {t} ^ {i} (\sigma_ {i} d W _ {t} + \mu_ {i} d t), \quad i = 1, 2.
$$

## 4.4 Market price of risk

Following the discussion on tradables, we want the discounted prices of $S_{t}^{1}$ and $S_{t}^{2}$ to be martingales under the same measure Q. So assuming a simple numeraire $B_{t} = \exp(rt)$ , we have that 

$$
\tilde {W} _ {t} = W _ {t} + \left(\frac {\mu_ {i} - r}{\sigma_ {i}}\right) t
$$

must be a Q-Brownian motion for i equal to 1 and 2. But this can only happen if the two changes of drift are the same. That is if 

$$
\frac {\mu_ {1} - r}{\sigma_ {1}} = \frac {\mu_ {2} - r}{\sigma_ {2}}.
$$

In one of those coincidences that cause confusion, economists attach a meaning to this quantity – if we interpret $\mu$ as the growth rate of the tradable, r as the growth rate of the riskless bond and $\sigma$ as a measure of the risk of the asset, then 

$$
\gamma = \frac {\mu - r}{\sigma}
$$

is the rate of extra return (above the risk-free rate) per unit of risk. As such it is often called the market price of risk. 

Using this language then gives us a simple and compelling categorisation of tradables in terms of their SDEs – all tradables in a market should have the same market price of risk. 

## The general market price of risk

We can, in fact, generalise to more sophisticated one-factor models. Rigour will have to wait until section 6.1, but for now we can observe that a general stochastic price process $S_{t}$ will have SDE 

$$
d S _ {t} = S _ {t} (\sigma_ {t} d W _ {t} + \mu_ {t} d t),
$$

where $\sigma_{t}$ and $\mu_{t}$ are previsible processes. 

Then defining 

$$
\gamma_ {t} = \frac {\mu_ {t} - r}{\sigma_ {t}}
$$

gives a time and state dependent market price of risk. Despite this variation, the same as above will hold. All tradable securities must instantaneously have the same market price of risk. 

## The risk-neutral measure

It is worth reflecting on what we have done – we have provided justification that to be tradable in a market defined by a stock $S_{t}$ and a numeraire $B_{t}$ is to share, after discounting by $B_{t}$ , a martingale measure with $S_{t}$ . This translates naturally in SDE terms to sharing a market price of risk – the market price of risk is actually the drift change of the underlying Brownian motion given by Cameron–Martin–Girsanov. So we have a natural means for sorting through SDEs for tradables. 

We also have a natural explanation for the market terminology of Q as the risk-neutral measure. If we write the SDEs in terms of the Q-Brownian motion $\tilde{W}_{t}$ : 

$$
d S _ {t} = S _ {t} \left(\sigma_ {t} d \tilde {W} _ {t} + \tilde {\mu} _ {t} d t\right),
$$

then $S_{t}$ is tradable if and only if its market price of risk is zero. All tradables then have the same growth rate under Q as the cash bond, independent of their riskiness $\sigma_{t}$ – the measure Q is neutral with respect to risk. 

But we should not overstretch the economic analogy – within our one-factor market all tradables are instantaneously perfectly correlated. They share a market price of risk not for profound economic reasons or because investors behave with certain risk preferences but for the reason that to do otherwise would produce a non-martingale process with a consequent opportunity for arbitrage. The market price of risk is only a convenient algebraic form for the change of measure from P to Q, not a new argument for using it. 

## Non-tradable quantities

But convenient it is. Let's return to our underlying theme - dealing with non-tradable processes. With foreign exchange, equities and bonds we had a model for a process that had a fixed relationship to a tradable but was itself non-tradable. Concretely, we might have a non-tradable $X_{t}$ which is modelled with the stochastic differential 

$$
d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t,
$$

where $\sigma_{t}$ and $\mu_{t}$ are previsible processes and $W_{t}$ is $\mathbb{P}$ -Brownian motion. Here $\sigma_{t}$ and $\mu_{t}$ might be constants or constant multiples of $X_{t}$ , but they needn't be. 

We have $X_{t}$ non-tradable but a deterministic function of $X_{t}, Y_{t} = f(X_{t})$ , is tradable. Then by Itô's formula, $Y$ has differential increment 

$$
d Y _ {t} = \sigma_ {t} f ^ {\prime} (X _ {t}) d W _ {t} + \left(\mu_ {t} f ^ {\prime} (X _ {t}) + \frac {1}{2} \sigma_ {t} ^ {2} f ^ {\prime \prime} (X _ {t})\right) d t.
$$

## 4.4 Market price of risk

As $Y_{t}$ is tradable, we can write down the market price of risk for $Y_{t}$ immediately. Assuming the discount rate is constant at r, 

$$
\gamma_ {t} = \frac {\mu_ {t} f ^ {\prime} (X _ {t}) + \frac {1}{2} \sigma_ {t} ^ {2} f ^ {\prime \prime} (X _ {t}) - r f (X _ {t})}{\sigma_ {t} f ^ {\prime} (X _ {t})}.
$$

Since this market price of risk is simply the change of measure from $\mathbb{P}$ to $\mathbb{Q}$ , we can write down $X$ 's behaviour under $\mathbb{Q}$ as 

$$
d X _ {t} = \sigma_ {t} d \tilde {W} _ {t} + \frac {r f (X _ {t}) - \frac {1}{2} \sigma_ {t} ^ {2} f ^ {\prime \prime} (X _ {t})}{f ^ {\prime} (X _ {t})} d t.
$$

Thus if we have claims on $X_{t}$ , they can be priced via the normal expectation route, using this risk-neutral SDE for $X_{t}$ . 

## Examples

(i) If $X_{t}$ is the logarithm of a tradable asset, then $f$ is the exponential function $f(x) = e^{x}$ . In the simple case where $\sigma_{t} = \sigma$ and $\mu_{t} = \mu$ are constants (the basic Black-Scholes model), then the market price of risk for tradables is 

$$
\gamma_ {t} = \frac {\mu + \frac {1}{2} \sigma^ {2} - r}{\sigma},
$$

and the corresponding risk-neutral SDE for $X_{t}$ is 

$$
d X _ {t} = \sigma d \tilde {W} _ {t} + \left(r - \frac {1}{2} \sigma^ {2}\right) d t.
$$

## Time-dependent transforms

More generally, suppose interest rates follow the process $r_{t}$ , $X_{t}$ is non-tradable with stochastic differential 

$$
d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t,
$$

and Y is a tradable security which is a deterministic function of X and time, that is $Y_{t} = f(X_{t}, t)$ . Then under the martingale measure Q, X has differential 

$$
d X _ {t} = \sigma_ {t} d \tilde {W} _ {t} + \frac {r _ {t} f (X _ {t} , t) - \frac {1}{2} \sigma_ {t} ^ {2} f ^ {\prime \prime} (X _ {t} , t) - \partial_ {t} f (X _ {t} , t)}{f ^ {\prime} (X _ {t} , t)} d t,
$$

where $f'$ and $f''$ are derivatives of f with respect to x, and $\partial_{t}f$ is the derivative of f with respect to t. 

(ii) The price process $S_{t}$ pays dividends at rate $\delta S_{t}$ . Let $X_{t}$ be the process $S_{t}$ and assume that it follows the Black-Scholes model 

$$
d X _ {t} = X _ {t} (\sigma d W _ {t} + \mu d t).
$$

The asset $Y_{t} = \exp(\delta t)X_{t}$ made from instantaneously reinvesting the dividends back into the stock holding is a tradable asset. The function f is thus chosen to be $f(x, t) = xe^{\delta t}$ . The market price of risk for tradables is then 

$$
\gamma_ {t} = \frac {\mu X _ {t} e ^ {\delta t} + \delta X _ {t} e ^ {\delta t} - r X _ {t} e ^ {\delta t}}{\sigma X _ {t} e ^ {\delta t}} = \frac {\mu + \delta - r}{\sigma},
$$

and thus the risk-neutral SDE for $X_{t}$ becomes 

$$
d X _ {t} = X _ {t} \left(\sigma d \tilde {W} _ {t} + (r - \delta) d t\right).
$$

(iii) Foreign exchange, the ‘wrong way round’. Let $C_{t}$ be the dollar/mark exchange rate (worth in deutschmarks of one dollar), then the rate $C_{t}$ paid in dollars is non-tradable. (That is, if $C_{t}$ is equal to DM 1.45, the process worth 1.45 is not tradable.) However the process $1/C_{t}$ is tradable, or more strictly $e^{ut}/C_{t}$ is a dollar tradable asset if German interest rates are constant at rate u. If $X_{t}=C_{t}$ has SDE 

$$
d X _ {t} = X _ {t} (\sigma_ {t} d W _ {t} + \mu_ {t} d t),
$$

then the time-dependent transform of $f(x,t) = e^{ut} / x$ tells us that its risk-neutral SDE is 

$$
d X _ {t} = X _ {t} \left(\sigma_ {t} d \tilde {W} _ {t} + \left(\sigma_ {t} ^ {2} + u - r\right) d t\right).
$$

## 4.5 Quantos

British Petroleum, a UK company, has a sterling denominated stock price. But instead of thinking of that stock price just in pounds, we could also consider it as a pure number which could be denominated in any currency. 

## 4.5 Quantos

Contracts like this which pay off in the ‘wrong’ currency are quantos. For instance, if the current stock price were £5.20, we could have a derivative that paid this price in dollars, that is $5.20. This is not the same as the worth of the BP stock in dollars – that would depend on the exchange rate. What we have done is a purely formal change of units, whilst leaving the actual number unaltered. 

Quantos are best described with examples. Here are three: 

- a forward contract, namely receiving the BP stock price at time T as if it were in dollars in exchange for paying a pre-agreed dollar amount; 

- a digital contract which pays one dollar at time T if the then BP stock price is larger than some pre-agreed strike; 

- an option to receive the BP stock price less a strike price, in dollars. 

In each case, a simple derivative is given the added twist of paying off in a currency other than in which the underlying security is denominated. And our intuition should warn us that this act of switching currency is not a foreign exchange quibble but something more fundamental. The British Petroleum stock price in dollars is a meaningful concept, but it is not a traded security. The payoffs we describe involve a non-tradable quantity. 

Suppose we have a simple two-factor model. We have not actually met multi-factor models yet, but they are no more problematic than single-factor ones if we keep our head. Rigour can be found in the multiple stock models section (6.3). Our two random processes will be the stock price and the exchange rate, which will be driven by two independent Brownian motions $W_{1}(t)$ and $W_{2}(t)$ . 

For the construction, it is helpful to recall exercise 3.2: for $\rho$ lying between -1 and 1, then $\rho W_{1}(t) + \sqrt{1 - \rho^{2}} W_{2}(t)$ is also a Brownian motion, and it has correlation $\rho$ with the original Brownian motion $W_{1}(t)$ . This is a useful way to manufacture two Brownian motions which are correlated out of a pair which are independent. 

We suppose there exist the following constants: drifts $\mu$ and $\nu$ , positive volatilities $\sigma_{1}$ and $\sigma_{2}$ , and a correlation $\rho$ lying between -1 and 1. 

Given these constants, the quanto model is: 

## Quanto model

The sterling stock price $S_{t}$ and the value of one pound in dollars $C_{t}$ follow the processes 

$$
S _ {t} = S _ {0} \exp \left(\sigma_ {1} W _ {1} (t) + \mu t\right),
$$

$$
C _ {t} = C _ {0} \exp \left(\rho \sigma_ {2} W _ {1} (t) + \bar {\rho} \sigma_ {2} W _ {2} (t) + \nu t\right),
$$

where $\bar{\rho}$ is the orthogonal complement of $\rho$ , namely $\bar{\rho} = \sqrt{1 - \rho^{2}}$ . 

In addition there is a dollar cash bond $B_{t} = \exp(rt)$ and a sterling cash bond $D_{t} = \exp(ut)$ , for some positive constant interest rates r and u. 

Before we tease out the tradable instruments in dollars, note the covariance of $S_{t}$ and $C_{t}$ . If we write our model in vector form, the vector random variable ( $\log S_{t}, \log C_{t}$ ) is jointly-normally distributed with mean vector ( $\log S_{0} + \mu t, \log C_{0} + \nu t$ ) and covariance matrix 

$$
\left( \begin{array}{c c} \sigma_ {1} & 0 \\ \rho \sigma_ {2} & \bar {\rho} \sigma_ {2} \end{array} \right) \left( \begin{array}{c c} t & 0 \\ 0 & t \end{array} \right) \left( \begin{array}{c c} \sigma_ {1} & 0 \\ \rho \sigma_ {2} & \bar {\rho} \sigma_ {2} \end{array} \right) ^ {\top} = \left( \begin{array}{c c} \sigma_ {1} ^ {2} & \rho \sigma_ {1} \sigma_ {2} \\ \rho \sigma_ {1} \sigma_ {2} & \sigma_ {2} ^ {2} \end{array} \right) t.
$$

That is, we have ensured a constant volatility for $S_{t}$ of $\sigma_{1}$ , a constant volatility for $C_{t}$ of $\sigma_{2}$ and a correlation between them of $\rho$ . 

## Tradables

What are the dollar tradables? Following the intuition of the foreign exchange section (4.1), there are three: the dollar worth of the sterling bond, $C_{t}D_{t}$ ; the dollar worth of the stock, $C_{t}S_{t}$ ; and a dollar numeraire, the dollar cash bond $B_{t}$ . 

Writing down the first two of these tradables after discounting by the third, the numeraire, we have $Y_{t} = B_{t}^{-1}C_{t}D_{t}$ and $Z_{t} = B_{t}^{-1}C_{t}S_{t}$ respectively. Their SDEs are 

$$
\begin{array}{l} d Y _ {t} = Y _ {t} \big (\rho \sigma_ {2} d W _ {1} (t) + \bar {\rho} \sigma_ {2} d W _ {2} (t) + (\nu + \frac {1}{2} \sigma_ {2} ^ {2} + u - r) d t \big), \\ d Z _ {t} = Z _ {t} \big ((\sigma_ {1} + \rho \sigma_ {2}) d W _ {1} (t) + \bar {\rho} \sigma_ {2} d W _ {2} (t) \\ \qquad + (\mu + \nu + \frac {1}{2} \sigma_ {1} ^ {2} + \rho \sigma_ {1} \sigma_ {2} + \frac {1}{2} \sigma_ {2} ^ {2} - r) d t \big). \end{array}
$$

(This can be checked using the $n$ -factor Itô's formula of section 6.3.) 

## 4.5 Quantos

As in the market price of risk section, we know we want to find a change of measure to make these martingales, or equivalently a market price of risk that represents this change of drift. As there are two sources of risk, $W_{1}(t)$ and $W_{2}(t)$ , there will be two separate prices of risk. Respectively, $\gamma_{1}(t)$ will be the price of $W_{1}(t)$ -risk and $\gamma_{2}(t)$ will be the price of $W_{2}(t)$ -risk. In other words the market price of risk will be a vector $(\gamma_{1}(t),\gamma_{2}(t))$ . We want to choose these $\gamma$ so that the drift terms in $dY_{t}$ and $dZ_{t}$ vanish simultaneously. Not surprisingly this means solving a pair of simultaneous equations, or equivalently performing the matrix inversion 

$$
\binom{\gamma_ {1} (t)}{\gamma_ {2} (t)} = \left( \begin{array}{c c} \rho \sigma_ {2} & \bar {\rho} \sigma_ {2} \\ \sigma_ {1} + \rho \sigma_ {2} & \bar {\rho} \sigma_ {2} \end{array} \right) ^ {- 1} \binom{\nu + \frac {1}{2} \sigma_ {2} ^ {2} + u - r}{\mu + \nu + \frac {1}{2} \sigma_ {1} ^ {2} + \rho \sigma_ {1} \sigma_ {2} + \frac {1}{2} \sigma_ {2} ^ {2} - r}.
$$

This is a particular case of the more general result that the multi-dimensional market price of risk is 

$$
\gamma_ {t} = \Sigma^ {- 1} (\mu - r \mathbf {1}),
$$

where $\Sigma$ is the assets' volatility matrix, $\mu$ is their drift vector, and 1 is the constant vector $(1,\ldots,1)$ . More details are in section 6.3. 

Here then we have a market price of risk $\gamma_{t} = (\gamma_{1}(t),\gamma_{2}(t))$ , given by 

$$
\gamma_ {1} = \frac {\mu + \frac {1}{2} \sigma_ {1} ^ {2} + \rho \sigma_ {1} \sigma_ {2} - u}{\sigma_ {1}}, \quad \text { and } \quad \gamma_ {2} = \frac {\nu + \frac {1}{2} \sigma_ {2} ^ {2} + u - r - \rho \sigma_ {2} \gamma_ {1}}{\bar {\rho} \sigma_ {2}}.
$$

Thus under $\mathbb{Q}$ we can write the original processes $S_{t}$ and $C_t$ as 

$$
S _ {t} = S _ {0} \exp \bigl (\sigma_ {1} \tilde {W} _ {1} (t) + (u - \rho \sigma_ {1} \sigma_ {2} - \frac {1}{2} \sigma_ {1} ^ {2}) t \bigr),
$$

$$
C _ {t} = C _ {0} \exp \left(\rho \sigma_ {2} \tilde {W} _ {1} (t) + \bar {\rho} \sigma_ {2} \tilde {W} _ {2} (t) + (r - u - \frac {1}{2} \sigma_ {2} ^ {2}) t\right).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/a48d53f9308d0e02724b35efcda95320f910df33ec26a759d5eeef65c6709707.jpg)


Exercise 4.2 Verify that the measure Q which has Brownian motions $\tilde{W}_{i}(t)=W_{i}(t)+\int_{0}^{t}\gamma_{i}(s)ds(i=1,2)$ really is the martingale measure for $Y_{t}$ and $Z_{t}$ . 

Reassuringly the exchange rate process is as it was in section 4.1, given that $\rho \tilde{W}_1(t) + \bar{\rho} \tilde{W}_2(t)$ is another $\mathbb{Q}$ -Brownian motion (as was proved in exercise 3.2). 

But the stock price $S_{t}$ is different from what we expected. The drift has an extra term: $-\rho \sigma_{1} \sigma_{2}$ . For every value of $\rho$ (except one, namely $(u - r) / \sigma_{1} \sigma_{2}$ ) this stops the dollar-discounted stock price being a Q-martingale and thus prevents the price in dollars from being tradable. And that's precisely what our intuition warned us. There isn't a portfolio which is always worth a dollar amount numerically equal to the BP stock price. 

## Pricing

Since we have a measure Q, under which the dollar tradables are martingales, we can price up our quanto options. 

## Forward

To price the forward contract, it helps to re-express the stock price at date T as 

$$
S _ {T} = \exp (- \rho \sigma_ {1} \sigma_ {2} T) F \exp (\sigma_ {1} \sqrt {T} Z - \frac {1}{2} \sigma_ {1} ^ {2} T),
$$

where F is the local currency forward price of $S_{T}$ , $F = S_{0}e^{uT}$ , and Z is a normal $N(0,1)$ random variable under Q. 

Then the value of the forward at time zero in dollars is 

$$
V _ {0} = e ^ {- r T} \mathbb {E} _ {\mathbb {Q}} (S _ {T} - k) = e ^ {- r T} \left(\exp (- \rho \sigma_ {1} \sigma_ {2} T) F - k\right).
$$

For this to be on market, that is to have a value of zero, we must set k to be $F \exp(-\rho \sigma_{1} \sigma_{2} T)$ . This is not the same as the simple forward price F for sterling purchase. As $\sigma_{1}$ and $\sigma_{2}$ are both positive, it is clear that this quanto forward price is greater than the simple forward price if and only if the correlation between the stock and the exchange rate is negative. 

This actually makes some sense. Suppose we assumed that the quanto forward price was actually the same as the simple forward price F, then we could construct the following portfolio at time zero: by going 

- long $C_0 \exp((r - u)T)$ units of the quanto forward struck at $F$ , 

- short one unit of the simple sterling forward also struck at $F$ . 

If our assumption about the quanto forward price also being F were correct then this portfolio would be costless at time zero. At time T, this static replicating strategy would yield (in dollars) 

$$
C _ {0} \exp ((r - u) T) (S _ {T} - F) - C _ {T} (S _ {T} - F) = (C _ {0} \exp ((r - u) T) - C _ {T}) (S _ {T} - F).
$$

## 4.5 Quantos

Noting that $C_{0}\exp\left((r-u)T\right)$ is the forward FX rate for $C_{T}$ , consider the effect of negative correlation. If the stock price ends up above its forward and the FX rate is below its forward, then the value of this portfolio is positive. And if the stock price ends up below F and the FX rate is above its forward, then the value is also positive. 

Negative correlation makes these win-win situations more likely—perfect negative correlation makes them inevitable. If the quanto forward price really were $F$ under these circumstances it wouldn't be hard to construct an arbitrage. For negative $\rho$ the quanto forward must be greater than $F$ . 

## Digital

Our digital contract, $I(S_T > k)$ in dollars, has price $V_0 = e^{-rT}\mathbb{Q}(S_T > k)$ , or if we write $F_Q = F\exp (-\rho \sigma_1\sigma_2T)$ the quanto forward price, then 

$$
V _ {0} = e ^ {- r T} \Phi \left(\frac {\log \frac {F _ {Q}}{k} - \frac {1}{2} \sigma_ {1} ^ {2} T}{\sigma_ {1} \sqrt {T}}\right).
$$

Again the surprise of the $\exp(-\rho\sigma_{1}\sigma_{2}T)$ term. And in a ‘cleaner’ option. Surely the event of $S_{T}$ being greater than k is independent of whether the option is denominated in sterling or dollars. Indeed it is, but again replicating strategies, not expectation under P, price options. And replication involves the exchange rate, which is correlated with the stock price. 

## Call option

Finally, we can compute the option price of $e^{-rT}\mathbb{E}_{\mathbb{Q}}((S_T - k)^+)$ as 

$$
V _ {0} = e ^ {- r T} \left(F _ {Q} \Phi \left(\frac {\log \frac {F _ {Q}}{k} + \frac {1}{2} \sigma_ {1} ^ {2} T}{\sigma_ {1} \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F _ {Q}}{k} - \frac {1}{2} \sigma_ {1} ^ {2} T}{\sigma_ {1} \sqrt {T}}\right)\right).
$$

Perhaps not surprisingly for a log-normal model, this is just the original Black–Scholes formula with the quanto forward. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/006491a4bf7af092e5b41178733c99cf5b24390922e6602476a3b7817c2f543a.jpg)


Exercise 4.3 Suppose everything remains the same, except that the stock $S_{t}$ is the price in yen of NTT, a Japanese stock, $C_{t}$ is the dollar/yen exchange rate (the worth in yen of one dollar), and $\rho$ is their correlation. What is the one difference, between the sterling and yen cases, in the expression for the quanto forward price? 

# Chapter 5 Interest rates

Time is money. A dollar today is better than a dollar tomorrow. And a dollar tomorrow is better than a dollar next year. But just how much is that time worth – is every day worth the same or will the price of money change from time to time? 

The interest rate market is where the price of money is set – how much does it cost to have money tomorrow, money in a year, money in ten years? Previously we made the modelling assumption that the cost of money is constant, but this isn't actually so. The price of money over a term depends not only on the length of the term, but also on the moment-to-moment random fluctuations of the interest rate market. In this way, money behaves just like a stock with a noisy price driven by a Brownian motion. 

The uncertainty of the market opens up the possibility of derivative instruments based around the future value of money. Bonds, options on bonds, interest rate swaps, exotic contracts on the time value of different currencies, are all derived from basic interest-rate securities, just as stock options are derived from stocks in the market. In nominal cash terms, the market for such interest-rate derivatives far outstrips that for stock market products. Fortunately we shall still be able to calculate the prices of these contracts on exactly the same risk-free hedging basis as before. 

## 5.1 The interest rate market

## 5.1 The interest rate market

The most basic interest rate contract is an agreement to pay some money now in exchange for a promise of receiving a (usually) larger sum later. In general, the worth of such a contract will depend on factors other than just the time value of money, such as the credibility of the promisor and the perceived legality of the promise. Matters such as creditworthiness and the like are not our concern here, and it is for the bond market, not the interest rate market, to price them. We are solely concerned with the time value of money for default-free borrowing. 

This basic contract only requires two numbers to describe it – its length, or maturity, which records when we are to receive the later payment, and the ratio of the size of that payment to our initial payment. We can call the maturity date on which we are paid T, and the fraction of the final payment which is the initial, $P(0,T)$ . In other words, one dollar at time T can be bought at time zero for $P(0,T)$ dollars. 

## Discount bonds

But we can also regard the promise of a dollar as an asset, which will have some worth at time t before T. This asset is called a discount bond, and the price $P(0,T)$ is its price at time zero. But it can have a different price at any other time t up to maturity T, call it, say, $P(t,T)$ . This price $P(t,T)$ , the value at time t of receiving a dollar at time T, is a process in time – the price process of a tradable security. 

For any one maturity $T$ , the situation is much like the stock market in that here we have a tradable asset which has a stochastic price process. We feel we should be able to model its behaviour, and to price options on this $T$ -bond by trading in it to hedge them. (The only difference is the technical point that the bond evolves towards a known value - at time $T$ the bond is worth exactly one dollar, that is $P(T,T) = 1$ . Stocks don't do things like that, but it won't turn out to be a problem.) 

But we haven't got just one maturity. We could have written the contract for any one of the unlimited number of possible maturity dates. This matters because the bonds, although different, will be correlated. The ten-year bond, say, and the nine-year bond are going to move in very similar ways in the short term. Each bond cannot just be treated in isolation as if it were a stock. This is the real challenge of the interest rate market: the basic discount bonds are parameterised by two time indices, which determine both the start of the contract and its end. Bond prices are thus a function of two time variables, rather than just one, as stocks were. 

The bond price graph is actually a two-dimensional surface lying in three-dimensional space, which we can explore by taking two-dimensional graphical sections through it. Illustrated are sections along the lines t = 0 (figure 5.1) and T = 10 (figure 5.2). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/658b4be4740c4dc997903a4ca2628f29e2f91ade4bf68d98032338ce8ba22652.jpg)



Fig. 5.1 Bond prices now


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/ad5411489e25792d5818e722a10e26cc5bb931833c8a124058d4982dff2a3c0b.jpg)



Fig. 5.2 Price of 10-year bond vs time


Figure 5.1 is not the price process of an asset, but a graph of the current price of a whole spectrum of different assets (the bonds of different maturities). This reflects the current time value of money, quantifying exactly how much better it is to have cash now rather than later. Generally the more distant the payment maturity date, the less the current worth of the bond. Figure 5.2 is the price of one particular asset (the ten-year discount bond). Now instead of a smooth graph, we have a noisy stochastic process, up until it hits the value one at its maturity time. The start point of this graph is the end point of figure 5.1, being the common value $P(0,10)$ , or the worth now of receiving a dollar in ten years' time. 

## Yields

The picture in figure 5.1 is not particularly sensitive to what the market is doing. Other than saying now is better than later, it doesn't tell us very much on quick inspection. A more informative measure of the market is an indication of the implied average interest rate offered by a bond. If interest rates were constant at rate $r$ , the price of the $T$ -bond at time $t$ would be $e^{-r(T - t)}$ . In this particular case, $r$ can be recovered from the price $P(t,T)$ via the formula $r = -\log P(t,T) / (T - t)$ . 

## 5.1 The interest rate market

Interest rates are not constant, but that doesn't stop us viewing this translation as potentially useful. The rate we derive, $R(t,T)$ , is called the yield, and the mapping from price to yield is one-to-one for $t$ less than $T -$ no information is lost. 

## Yield

Given a discount bond price $P(t,T)$ at time t, the yield $R(t,T)$ is given by 

$$
R (t, T) = - \frac {\log P (t , T)}{T - t}.
$$

Thus for any given discount bond price curve, we can produce a yield curve; that is, a graph of $R(t,T)$ against T for some fixed t. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/bd7a81276e22cba8c83c2589747ef4448471b889ce71f22d35eac57c3cd67e8c.jpg)



Figure 5.3 Yield curve at $t = 0$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/9fa4b21b672168cb36da94aa4f85dcc1857d16c574bbd3271a79e58275a65c94.jpg)



Figure 5.4 Yield curve at $t = 4$


While the discount bond price curve contains exactly the same information as the yield curve, the translation is friendlier to the eye. Long dated bonds always have lower prices, so the downwards slope of the price curve is inevitable, thus redundant. Yield curves, on the other hand, can be increasing or decreasing functions of T, revealing the average return of bonds stripped of the crude effects of maturity – the term structure of the market. 

The difference in yields at different maturities reflects market beliefs about future interest rates. If there is a possibility that rates might be higher in the future, long-term loans will have to charge a higher rate than short-term ones. Typically the yield does increase with maturity, due to increased uncertainty about far-distant interest rates, but if current rates are high and expected to fall, the yield curve can become ‘inverted’ and long bond yields will be less than short bonds (figure 5.4). A good model should be able to cope with both these possibilities. 

## Instantaneous rate

But what is the price of money now? The yield curve gives us an idea of the rate of borrowing for each term length, but it would be convenient if we could summarise the current cost of borrowing in a single number. What we can do is look at the current rate for instantaneous borrowing. That is, borrowing which is paid back (nearly) instantly. If at time t we borrow over the period from t to $t + \Delta t$ , where $\Delta t$ is a small time increment, the rate we get is the yield $R(t, t + \Delta t)$ : 

$$
R (t, t + \Delta t) = - \frac {\log P (t , t + \Delta t)}{\Delta t}.
$$

For ever smaller time increments this value more closely approximates to $R(t,t)$ , which is the left-most point of the yield curve at time t. We call this value the instantaneous rate, or short rate, $r_{t}$ , which is given by both the expressions 

$$
\begin{array}{l} r _ {t} = R (t, t), \\ \text { and } \quad r _ {t} = - \frac {\partial}{\partial T} \log P (t, t). \end{array}
$$

The instantaneous rate is just a process in time, free of any other parameters. Figure 5.5 shows an example short rate over ten years, corresponding to the evolution of the 10-year bond in figure 5.2. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/f78dd9dfa55db4795d8cf08c44b21168b29e2496c9b9194f28e3b6830e17cbe4.jpg)



Figure 5.5 Instantaneous rate


We can sometimes see an interaction between the short rate and the bond prices if they are correlated. In one instance, bond prices might be lower 

## 5.1 The interest rate market

when the short rate is higher, which can be seen in this example around the 4 year and 8 year marks, when the short rate gets high and the bond price dips. Interestingly though, the high short rate at t = 4 even exceeds the increased yields on longer bonds, giving an inverted curve (figure 5.4). 

The instantaneous rate is not only an important process in the interest rate market, but many models are based exclusively on its behaviour, with all the other bonds extrapolated from it. 

## Forwards

The short-rate process, $r_{t}$ , is not a one-to-one mapping from the discount price curve $P(t,T)$ . The translation also entails a loss of information. Just giving $r_{t}$ with no extra prescription on how bond prices can move will not in general be enough to recover $P(t,T)$ . Yet the instantaneous rate is convenient to work with. What we require is a natural extension of $r_{t}$ which brings back the one-to-one mapping to the prices $P(t,T)$ and the yields $R(t,T)$ , yet still preserves the idea of instantaneity. 

Consider forward contracts, that is agreeing, at time t, to make a payment at a later date $T_{1}$ and receive a payment in return at an even later date $T_{2}$ . We are really just striking a forward on the $T_{2}$ -bond. But what forward price should we pay? 

There is a way of replicating this contract by, at time t, buying a $T_{2}$ -bond and selling a quantity, say k units, of the $T_{1}$ -bond. This deal has initial cost $P(t, T_{2}) - kP(t, T_{1})$ at time t, and will require us to make a payment of k at time $T_{1}$ , and will give us a payment of one dollar at time $T_{2}$ . To give the contract nil initial value, we must set k to be 

$$
k = \frac {P (t , T _ {2})}{P (t , T _ {1})}.
$$

This k must be, or face arbitrage, the forward price of purchasing the $T_{2}$ -bond at time $T_{1}$ . The corresponding (forward) yield is then 

$$
- \frac {\log P (t , T _ {2}) - \log P (t , T _ {1})}{T _ {2} - T _ {1}}.
$$

Were we to choose $T_{1}$ and $T_{2}$ very close together, say $T_{1} = T$ and $T_{2} = T + \Delta t$ , then as the increment $\Delta t$ became smaller this would converge to a forward rate for instantaneous borrowing, 

$$
f (t, T) = - \frac {\partial}{\partial T} \log P (t, T).
$$

This rate, called simply the forward rate, is the forward price of instantaneous borrowing at time T. As we might expect, the ‘forward’ rate for borrowing now, at time T = t, is exactly the current instantaneous rate, that is 

$$
f (t, t) = r _ {t}.
$$

But unlike $r_{t}$ , given the forward rates $f(t,T)$ we can recover the prices $P(t,T)$ and the yields $R(t,T)$ . The translation $f(t,T)$ for our particular example is shown in figure 5.6. 

Superficially, the forward rate curve resembles the bond yield curve (figure 5.3). Indeed the yield curve and the forward curve agree at their leftmost point, the instantaneous rate, but the other points of the two curves will generally be different. But the formula for $R(t,T)$ can be differentiated and rearranged to show that 

$$
f (t, T) = R (t, T) + (T - t) \frac {\partial R}{\partial T} (t, T).
$$

This tells us that the forward rate curve is higher than the yield curve, if the yield curve is increasing, and lower than it if the yield curve is inverted. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/5c148c0438157349d0c23533fc06a20a9c3dcb148cab414872df031e7ad0481f.jpg)



Figure 5.6 Forward rate curve at time t = 0


As a function of time rather than maturity the forward rate will not be so smooth, but will start with some initial value $f(0,T)$ and evolve as a stochastic process, finishing with the value $r_{T}$ at time T. 

## Summary

We have a market of default-free zero coupon discount bonds. The price at time t of the T-bond which pays off one dollar at time T is $P(t,T)$ . The average yield of the bond over its remaining lifetime is $R(t,T)$ , and the price now of instantaneous borrowing at time T is the forward rate $f(t,T)$ . The price of instantaneous spot borrowing is $r_{t}=R(t,t)=f(t,t)$ . 

Both of these associated families of rates, $R(t,T)$ and $f(t,T)$ , contain all the original price information which can be recovered. Explicitly 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/e2c3f7f2fd774ed196fbc01cbf1146a33bd2c891b42e51178514136fd9913734.jpg)


In other words, for modelling purposes we can choose to specify the behaviour of only any one of these three, and the other two will follow automatically. 

## 5.2 A simple model

A concrete example is illuminating. The secret of this chapter is that we can tackle interest rate models in exactly the same way as stock models. The Itô manipulations are harder but they are not significant for the story – just as in Black–Scholes, the real work is carried by the martingale representation theorem. In Black–Scholes, there were only two canonical tradables (the stock and the bond), but there are now an infinite number of underlying discount bonds. To pick just two of these tradables to work with would seem to favour that pair over the rest, but such worries will prove illusory. All the tradables will still turn out to be martingales under the risk-neutral measure, which itself is independent of the apparent ‘choice’ of instruments to work with. 

## Simple interest rate model

Given an initial T-integrable forward rate curve $f(0,T)$ , the forward curve evolves as: 

$$
d _ {t} f (t, T) = \sigma d W _ {t} + \alpha (t, T) d t,
$$

for some constant volatility $\sigma$ and drift $\alpha$ , a bounded deterministic function of time and maturity. 

We have set the market up not with an SDE for the price of any asset, but with the SDE for the forward rate. However as chapter four has shown, as long as we are an Itô step away from the price of something, this doesn't have to pose a problem. 

The forward rate itself is 

$$
f (t, T) = \sigma W _ {t} + f (0, T) + \int_ {0} ^ {t} \alpha (s, T) d s.
$$

Thus the forward rate is normally distributed. Moreover the forward rates at different maturities are perfectly correlated in their movements as the difference between any two of them, $f(t,T)-f(t,S)$ , is purely deterministic. There is only one source of randomness, the Brownian motion $W_{t}$ , and that is a process over time, not over maturity. 

## Tradable securities

Tradables may only be an Itô step away, but what are they? One is obvious – we want a numeraire. Though chapter six will show the choice of numeraire doesn't really matter, there is a canonical candidate – the cash bond formed by the instantaneous rate $r_{t}$ . That is, $B_{t}$ given by 

$$
d B _ {t} = r _ {t} B _ {t} d t, \qquad B _ {0} = 1.
$$

## 5.2 A simple model

Since $r_{t}$ is given by $f(t,t)$ , we can write down its integral equation easily enough as 

$$
r _ {t} = \sigma W _ {t} + f (0, t) + \int_ {0} ^ {t} \alpha (s, t) d s.
$$

[Technical trap: the SDE for $r_t$ is not just the SDE for $f(t, T)$ 'evaluated' at $T = t$ . Itô tells us it is actually $dr_t = d_t f(t, t) + \frac{\partial f}{\partial T}(t, t)$ .] Unlike the basic stock models, this rate is not constant but rather is a random process, and it is normally distributed, which admits the possibility of it being negative sometimes. Later we will show models which overcome this, but for the moment we'll pay this price for simplicity. Now for the cash bond, $B_t = \exp(\int_0^t r_s ds)$ , which has the slightly daunting expression 

$$
B _ {t} = \exp \left(\sigma \int_ {0} ^ {t} W _ {s} d s + \int_ {0} ^ {t} f (0, u) d u + \int_ {0} ^ {t} \int_ {s} ^ {t} \alpha (s, u) d u d s\right).
$$

This will be our tradable numeraire. 

What about another tradable? Here, as mentioned earlier, there's an embarrassment of tradables, but let's pick one. Fixing $T$ , we have the price of the $T$ -maturity bond $P(t,T)$ given by $P(t,T) = \exp(-\int_t^T f(t,u)du)$ or 

$$
P (t, T) = \exp - \left(\sigma (T - t) W _ {t} + \int_ {t} ^ {T} f (0, u) d u + \int_ {0} ^ {t} \int_ {t} ^ {T} \alpha (s, u) d u d s\right).
$$

## Replicating strategies

Suppose then we wanted to replicate some claim $X$ at a time horizon $S$ less than $T$ (so that the $T$ -maturity bond doesn't vanish on us). In chapters two, three and four we had a three-stage replicating strategy, so at least a first guess would be to follow it here as well: 

## Three steps to replication (interest-rate market)

(1) Find a measure $\mathbb{Q}$ under which the $T$ -bond discounted by the cash bond $Z_{t} = B_{t}^{-1}P(t,T)$ is a martingale. 

(2) Form the process $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{S}^{-1}X \mid \mathcal{F}_{t})$ . 

(3) Find a previsible process $\phi_t$ , such that $dE_t = \phi_t dZ_t$ . 

First we tackle the complicated-looking discounted bond price process $Z_{t}=B_{t}^{-1}P(t,T)$ : 

$$
Z _ {t} = \exp - \Big (\sigma (T - t) W _ {t} + \sigma \int_ {0} ^ {t} W _ {s} d s + \int_ {0} ^ {T} f (0, u) d u + \int_ {0} ^ {t} \int_ {s} ^ {T} \alpha (s, u) d u d s \Big).
$$

Noting that the $\sigma(T-t)W_t$ term's differential can be handled with the product rule and everything else inside the exponential is either constant or easy to differentiate, Itô gives us the SDE for $Z_t$ as 

$$
d Z _ {t} = Z _ {t} \left(- \sigma (T - t) d W _ {t} - \left(\int_ {t} ^ {T} \alpha (t, u) d u\right) d t + \frac {1}{2} \sigma^ {2} (T - t) ^ {2} d t\right).
$$

Now we are on familiar ground. Though we are used to the cash bond $B_{t}$ being deterministic, this (random) $B_{t}$ and the $T$ -bond price $P(t,T)$ are both adapted to the same Brownian motion, $W_{t}$ , and finding $Z_{t}$ doesn't pose any real problem. 

## Step one

We have an SDE for $Z_{t}$ and we want to see if we can find a change of measure drift $\gamma_{t}$ for the Brownian motion which makes $Z_{t}$ driftless. The candidate is clearly 

$$
\gamma_ {t} = - \frac {1}{2} \sigma (T - t) + \frac {1}{\sigma (T - t)} \int_ {t} ^ {T} \alpha (t, u) d u.
$$

And since it is bounded up to time S, the technical conditions of C-M-G are satisfied – our candidate passes and we have a measure Q, equivalent to P, such that $\tilde{W}_{t} = W_{t} + \int_{0}^{t} \gamma_{s} ds$ is a Q-Brownian motion. The SDE for the discounted price $Z_{t}$ now becomes 

$$
d Z _ {t} = - \sigma Z _ {t} (T - t) d \tilde {W} _ {t}.
$$

The process $Z_{t}$ has no drift, and because $\sigma(T - t)$ is bounded up to time S, $Z_{t}$ is a Q-martingale. 

## Step two

This gives us $E_{t}$ as the conditional $\mathbb{Q}$ -expectation of the discounted claim $B_{S}^{-1}X$ , namely 

$$
E _ {t} = \mathbb {E} _ {\mathbb {Q}} \big (B _ {S} ^ {- 1} X \mid \mathcal {F} _ {t} \big).
$$

But since $E_{t}$ is a Q-martingale just as $Z_{t}$ is, we take: 

## Step three

Using the martingale representation theorem to link them via an F-previsible process $\phi_{t}$ : 

$$
E _ {t} = \mathbb {E} _ {\mathbb {Q}} (B _ {S} ^ {- 1} X) + \int_ {0} ^ {t} \phi_ {s} d Z _ {s}.
$$

What is our trading strategy? At time t, 

• hold $\phi_t$ units of the $T$ -bond $P(t, T)$ 

- hold $\psi_t = E_t - \phi_t Z_t$ units of the cash bond $B_t$ . 

The undiscounted value of this portfolio at time t is 

$$
V _ {t} = \phi_ {t} P (t, T) + \psi_ {t} B _ {t} = B _ {t} E _ {t}.
$$

As before, it is also true that $dV_{t} = \phi_{t} d_{t} P(t, T) + \psi_{t} dB_{t}$ and thus this portfolio is self-financing. The strategy has an initial cost of $V_{0} = \mathbb{E}_{\mathbb{Q}}(B_{S}^{-1} X)$ and has a terminal value $V_{S} = X$ , which exactly hedges the claim. Arbitrage has won through. 

## Option price formula (interest rate)

The price of $X$ at time $t$ is 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \big (B _ {S} ^ {- 1} X \mid \mathcal {F} _ {t} \big).
$$

## No free lunches

So far, so good – even though the Itô work was harder, we have just another stock-type model. The chosen pair $B_{t}$ and $P(t,T)$ behaved like any of the tradables of chapter four. But something should worry us. We picked a particular bond, the T-maturity bond, and found a change of measure particular to that. Yet all claims which paid off at time S before T could be hedged, even those, for example, which are identical to bond of other maturities. 

So we have two ways of pricing the S-bond at time t, $P(t,S)$ . One direct from its SDE. And the other indirect, viewing $X = P(S,S) = 1$ as a claim to be hedged via the cash bond and the T-bond. 

There is no obvious reason why they should be the same given our original model. And yet the same they must be. If the hedge price were ever, say, less than $P(t, S)$ we would have an arbitrage engine capable of locking in unlimited profits. We don't want free lunches, so we should assume that the real world forbids them. That is we should impose on our real world model some suitable condition to make the various ways of getting at the price $P(t, S)$ agree. What condition? 

Consider the discounted process of the S-bond, $Y_{t} = B_{t}^{-1} P(t, S)$ . Reworking the Itô from before we have, as expected, 

$$
d Y _ {t} = Y _ {t} \left(- \sigma (S - t) d W _ {t} - \left(\int_ {t} ^ {S} \alpha (t, u) d u\right) d t + \frac {1}{2} \sigma^ {2} (S - t) ^ {2} d t\right).
$$

If we define $\gamma_t^S$ to be 

$$
\gamma_ {t} ^ {S} = - \frac {1}{2} \sigma (S - t) + \frac {1}{\sigma (S - t)} \int_ {t} ^ {S} \alpha (t, u) d u,
$$

then we have $dY_{t} = -\sigma Y_{t}(S-t)\left(dW_{t} + \gamma_{t}^{S} dt\right)$ , or in terms of the Q-Brownian motion we had before: 

$$
d Y _ {t} = - \sigma Y _ {t} (S - t) \left(d \tilde {W} _ {t} + \left(\gamma_ {t} ^ {S} - \gamma_ {t}\right) d t\right).
$$

This discounted process $Y_{t}$ must be a Q-martingale - it's tradable and, from the risk-free hedging construction, $Y_{t} = B_{t}^{-1}P(t,S) = \mathbb{E}_{\mathbb{Q}}(B_S^{-1}|\mathcal{F}_t)$ . So the drift term of the SDE above must be zero: $\gamma_t^S = \gamma_t$ . 

Here is the restriction we require - our arbitrary choice of $T$ must not have affected the process $\gamma_t$ . So $\gamma_t$ must be independent of $T$ , or in other words $\frac{\partial\gamma}{\partial T} = 0$ . 

Multiplying the formula for $\gamma_{t}$ by $\sigma(T-t)$ and differentiating with respect to T, we get: 

## Restriction on the drift

In an arbitrage-free market, the drift $\alpha(t,T)$ satisfies 

$$
\alpha (t, T) = \sigma^ {2} (T - t) + \sigma \gamma_ {t}.
$$

This equation is saying something we did not encounter, at this level, in the stock market. It says that there are restrictions on the drifts which the 

## 5.2 A simple model

forward rates can have if there is to be no arbitrage. The drift $\alpha(t,T)$ may have started off as a general deterministic function of both time and maturity, but now it is expressed as the sum of a particular function $(\sigma^{2}(T-t))$ and a process which has no maturity dependence at all $(\sigma\gamma_{t})$ . Most general functions cannot be written in this way. 

In another sense, this is actually familiar ground. We can think of the SDE for $P(t,T)$ under P as 

$$
d _ {t} P (t, T) = P (t, T) \left(- \sigma (T - t) d W _ {t} + \left(r _ {t} - \sigma (T - t) \gamma_ {t}\right) d t\right).
$$

Written this way, $\gamma_{t}$ stands revealed as the market price of risk (see section 4.4). We know that every security in the market has to have the same market price of risk, which explains why $\gamma_{t}$ does not depend on the maturity T chosen. 

Two things stand out. Firstly there is a measure Q which makes a martingale not just out of one discounted bond, but each and every discounted bond simultaneously. We worried about the embarrassment of bonds to choose, but we needn't have. There was only one Brownian motion and that is what matters. If we freeze time and look at just one t, the values of the bonds $P(t,T)$ are just deterministic transformations of each other. And if one bond can be brought into line by a change of measure then so can they all. 

If, that is, they are roughly in step in the first place. Our second point is that there is a price to pay for this success. If we write the original SDE for $f(t,T)$ in terms of the Q-Brownian motion, $\tilde{W}_{t}$ , we have: 

$$
d _ {t} f (t, T) = \sigma d \tilde {W} _ {t} + \sigma^ {2} (T - t) d t.
$$

As we expect from a Black–Scholes upbringing, the drift $\alpha(t,T)$ has vanished. But $\alpha(t,T)$ must be recoverable by a change of measure $\gamma_{t}$ which has no dependence on T. So we weren't free to pick $\alpha(t,T)$ as any function of t and T – we must, unlike Black–Scholes, have some structure to the original real world drift. 

But even if our success has brought slight complications, we have nonetheless succeeded. We have a model with stochastic interest rates which is still arbitrage-complete. All claims can be coherently hedged by the underlying bonds. Once more, replication provides the price. 

Bonds and rates in terms of the Q-Brownian motion $\tilde{W}_{t}$ . The bond prices, forward and short rates are given by: 

$$
P (t, T) = \exp - \left(\sigma (T - t) \tilde {W} _ {t} + \int_ {t} ^ {T} f (0, u) d u + \frac {1}{2} \sigma^ {2} T (T - t) t\right)
$$

$$
B _ {t} = \exp \left(\sigma \int_ {0} ^ {t} \tilde {W} _ {s} d s + \int_ {0} ^ {t} f (0, u) d u + \frac {1}{6} \sigma^ {2} t ^ {3}\right)
$$

$$
f (t, T) = \sigma \tilde {W} _ {t} + f (0, T) + \sigma^ {2} (T - \frac {1}{2} t) t,
$$

$$
r _ {t} = \sigma \tilde {W} _ {t} + f (0, t) + \frac {1}{2} \sigma^ {2} t ^ {2}.
$$

## 5.3 Single-factor HJM

From the particular to the general. We know the basic idea - all three descriptions of the yield curve, the prices $P(t,T)$ , the yields $R(t,T)$ and the forward rates $f(t,T)$ are equivalent, so we select one and specify its behaviour. Heath-Jarrow-Morton (HJM) is a powerful, technically rigorous interest-rate model based on the instantaneous forward rates $f(t,T)$ . 

## Single-factor HJM model

Given an initial forward rate curve $f(0, T)$ , the forward rate for each maturity T evolves as 

$$
f (t, T) = f (0, T) + \int_ {0} ^ {t} \sigma (s, T) d W _ {s} + \int_ {0} ^ {t} \alpha (s, T) d s, \quad 0 \leqslant t \leqslant T,
$$

or in differential form 

$$
d _ {t} f (t, T) = \sigma (t, T) d W _ {t} + \alpha (t, T) d t.
$$

The volatilities $\sigma(t,T)$ and the drifts $\alpha(t,T)$ can depend on the history of the Brownian motion $W_{t}$ and on the rates themselves up to time t. 

## 5.3 Single-factor HJM

For any fixed maturity T, the forward rate evolves according to its own volatility $\sigma(t,T)$ and its own drift $\alpha(t,T)$ . In section 5.5 we will allow the decoupling that comes when rates can move with less than perfect correlation, but here only a single process, a P-Brownian motion $W_{t}$ , will drive each and every rate. The incremental changes of all forward rates, and thus all yields and all bond prices are perfectly correlated. 

Our formal description is vague about the precise properties of the volatility and drift functions. The general HJM model posits very few overarching conditions on the $\sigma$ and $\alpha$ , but imposes piecemeal technical constraints from time to time. Collected, and simplified somewhat, these technical conditions are shown in the box. The first two conditions make sure that the forward rates $f(t,T)$ are well defined by their SDE. The last two conditions will be used for a Fubini-type result that the stochastic differential of the integral of $f(t,T)$ with respect to T is the integral of the stochastic differentials of f. Given these box conditions, the first three conditions of the HJM model (C1–C3 in their paper) are satisfied. 

## Single-factor HJM: conditions on the volatility and drift We assume that

- for each $T$ , the processes $\sigma(t, T)$ and $\alpha(t, T)$ are previsible and depend only on the history of the Brownian motion up to time $t$ , and are good integrators in the sense that $\int_{0}^{T} \sigma^{2}(t, T) dt$ and $\int_{0}^{T} |\alpha(t, T)| dt$ are finite; 

- the initial forward curve, $f(0,T)$ , is deterministic and satisfies the condition that $\int_0^T |f(0,u)|du < \infty$ ; 

- the drift $\alpha$ has finite integral $\int_0^T\int_0^u |\alpha (t,u)|dtdu;$ 

- the volatility $\sigma$ has finite expectation $\mathbb{E}\int_0^T\big|\int_0^u\sigma (t,u)dW_t\big|du.$ 

## Numeraire

As chapter six will show, the choice of numeraire is arbitrary - but algebraic convenience certainly points to a canonical choice. Our description of the forward rates $f(t,T)$ allows us to write down an integral equation for the instantaneous rate $r_t = f(t, t)$ (which need not be Markov), namely: 

$$
r _ {t} = f (0, t) + \int_ {0} ^ {t} \sigma (s, t) d W _ {s} + \int_ {0} ^ {t} \alpha (s, t) d s.
$$

The simplest cash product is then the account, or bond, formed by starting with one dollar at time zero and reinvesting continually at this rate. In other words, the bond B is a stochastic process satisfying the SDE 

$$
d B _ {t} = r _ {t} B _ {t} d t, \quad B _ {0} = 1, \quad \text { or } \quad B _ {t} = \exp \left(\int_ {0} ^ {t} r _ {s} d s\right).
$$

Integration then gives us 

$$
B _ {t} = \exp \left(\int_ {0} ^ {t} \left(\int_ {s} ^ {t} \sigma (s, u) d u\right) d W _ {s} + \int_ {0} ^ {t} f (0, u) d u + \int_ {0} ^ {t} \int_ {s} ^ {t} \alpha (s, u) d u d s\right).
$$

Here we used the last technical condition of the HJM box to say that the integrals of $\int_{0}^{t}\left(\int_{0}^{u}\sigma(s,u)dW_{s}\right)du$ can be interchanged to $\int_{0}^{t}\left(\int_{s}^{t}\sigma(s,u)du\right)dW_{s}$ . We have a numeraire. 

## Bond prices

We need tradable assets - and we have them, the bonds $P(t,T)$ . Since the forward rates $f(t,T)$ are a one-to-one transformation, the bond prices themselves are contained in the forward rate information as 

$$
P (t, T) = \exp \left(- \int_ {t} ^ {T} f (t, u) d u\right),
$$

which will be continuous in t and T. If we integrate the original equation for the forward rates $f(t,T)$ then we have the bond price $P(t,T)$ equal to 

$$
\exp - \left(\int_ {0} ^ {t} \left(\int_ {t} ^ {T} \sigma (s, u) d u\right) d W _ {s} + \int_ {t} ^ {T} f (0, u) d u + \int_ {0} ^ {t} \int_ {t} ^ {T} \alpha (s, u) d u d s\right)
$$

Reassuringly this expression, although awkward, has the right values at time zero (namely $\exp\left(-\int_{0}^{T}f(0,u)du\right)$ ) and time T (namely one). 

## 5.3 Single-factor HJM

## Discounted bonds

Let's fix one particular maturity $T$ to work with for the moment. As everywhere else, our attention focuses on the discounted asset price - that is, $Z(t,T) = B_t^{-1}P(t,T)$ . By combining the above expressions for the cash bond and the bond price itself, we get 

$$
Z (t, T) = \exp \left(\int_ {0} ^ {t} \Sigma (s, T) d W _ {s} - \int_ {0} ^ {T} f (0, u) d u - \int_ {0} ^ {t} \int_ {s} ^ {T} \alpha (s, u) d u d s\right),
$$

where $\Sigma(t, T)$ is just notation for the integral $-\int_{t}^{T} \sigma(t, u) du$ . Itô handle-turning then gives the SDE - 

$$
d _ {t} Z (t, T) = Z (t, T) \left(\Sigma (t, T) d W _ {t} + \left(\frac {1}{2} \Sigma^ {2} (t, T) - \int_ {t} ^ {T} \alpha (t, u) d u\right) d t\right),
$$

revealing the variable $\Sigma(t, T)$ to be the log-volatility of $P(t, T)$ . 

## Change of measure

In the usual way, we want to make the discounted bond into a martingale by changing measure. The change of measure drift (market price of risk) is 

$$
\gamma_ {t} = \frac {1}{2} \Sigma (t, T) - \frac {1}{\Sigma (t , T)} \int_ {t} ^ {T} \alpha (t, u) d u.
$$

We need the technical Cameron–Martin–Girsanov theorem condition that $E_{P} \exp \frac{1}{2} \int_{0}^{T} \gamma_{t}^{2} dt$ is finite. Then there will be a new measure Q equivalent to P, such that $\tilde{W}_{t} = W_{t} + \int_{0}^{t} \gamma_{s} ds$ is Q-Brownian motion. The SDE of the discounted bond under Q is then 

$$
d _ {t} Z (t, T) = Z (t, T) \Sigma (t, T) d \tilde {W} _ {t},
$$

which is driftless. For this to be a proper Q-martingale, it is sufficient that the exponential martingale condition $E_{Q} \exp \frac{1}{2} \int_{0}^{T} \Sigma^{2}(t, T) dt < \infty$ holds (see section 3.5). 

## Bond price SDE

Under this martingale measure, the bond price P now has the stochastic differential 

$$
d _ {t} P (t, T) = P (t, T) \left(\Sigma (t, T) d \tilde {W} _ {t} + r _ {t} d t\right).
$$

The concrete model of section 5.2 partially spoilt the surprise, but we have our Black–Scholes like result, even here with a general interest-rate model such as HJM. The behaviour of the price P under the martingale measure does not depend on the drift $\alpha$ , but only on the volatility $\Sigma$ (itself a function of $\sigma$ ). Just as the Black–Scholes stock model under Q had no dependence on the original stock drift $\mu$ . 

## Replicating strategies

We've jumped slightly ahead of ourselves, we have found the martingale measure and the process for $P(t,T)$ under it. But we ought to check that we can produce replicating strategies for claims. Suppose we have a claim $X$ which pays off at time $S$ . If we are going to hedge this with a discount bond maturing at date $T$ , our only restriction is that $S$ should come before $T$ – we cannot hedge a long-term product with a shorter-term instrument. (Unless we split the time-period up into shorter subsections, and roll over short-term bonds from section to section.) Suppose, for simplicity, we choose to use a bond with maturity $T$ larger than $S$ . 

As before, our second step to replication is to form the conditional Q-expectation of the discounted claim $B_{S}^{-1}X$ , rather than the raw claim X. That is, we define $E_{t}$ to be the Q-martingale 

$$
E _ {t} = \mathbb {E} _ {\mathbb {Q}} \big (B _ {S} ^ {- 1} X \mid \mathcal {F} _ {t} \big).
$$

For the martingale representation theorem to be used, we also need that the bond volatility $\Sigma(t,T)$ is never zero before T, in which case, we apply the representation theorem to the martingale $Z(t,T)$ and the discounted claim process $E_{t}$ . This gives us that 

$$
E _ {t} = E _ {0} + \int_ {0} ^ {t} \phi_ {s} d Z (s, T),
$$

for some $\mathcal{F}$ -previsible process $\phi$ . 

Our trading strategy will be a combination of both a holding in the T-bond and a holding in the cash bond $B_{t}$ . Specifically, we 

• hold $\phi_{t}$ units of the T-bond at time t, 

- hold $\psi_t := E_t - \phi_t Z(t, T)$ units of the cash bond at time $t$ . 

## 5.3 Single-factor HJM

The value of this portfolio at time t is 

$$
V _ {t} = B _ {t} E _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \big (B _ {S} ^ {- 1} X \big | \mathcal {F} _ {t} \big).
$$

The strategy $(\phi_{t},\psi_{t})$ will be self-financing if $dV_{t}=\phi_{t}d_{t}P(t,T)+\psi_{t}dB_{t}$ , or equivalently (as in section 3.7) if 

$$
d E _ {t} = \phi_ {t} d _ {t} Z (t, T).
$$

Which is ensured by the representation of $E_{t}$ in terms of $\phi_{t}$ . The portfolio $(\phi_{t},\psi_{t})$ is self-financing. Thus: 

Derivative pricing
If X is the payoff of a derivative maturing at time T, then its value at time t is $V_{t} = B_{t} \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X \mid \mathcal{F}_{t}) = \mathbb{E}_{\mathbb{Q}}\left(\exp(-\int_{t}^{T} r_{s} ds)X \mid \mathcal{F}_{t}\right).$ 

## Arbitrage-free market

But the S-bond is simply a claim of X = 1 maturing at time S. Thus its worth at time t must be $B_{t}\mathbb{E}_{\mathbb{Q}}(B_{S}^{-1}|\mathcal{F}_{t})$ . Or more fully, 

$$
P (t, S) = \mathbb {E} _ {\mathbb {Q}} \left(\exp \left(- \int_ {t} ^ {S} r _ {u} d u\right) \mid \mathcal {F} _ {t}\right), \quad t \leqslant S <   T.
$$

The martingale measure brings a pleasant simplicity. All bond prices are just the expectation under Q of the instantaneous rate discount from t to their maturity. 

What about the discounted S-bond, $Z(t,S)=B_{t}^{-1}P(t,S)$ ? This can now be written as 

$$
Z (t, S) = \mathbb {E} _ {\mathbb {Q}} \left(B _ {S} ^ {- 1} \mid \mathcal {F} _ {t}\right).
$$

Just as we saw in the simple example (section 5.2), all the other (discounted) bonds are now martingales under the same Q. Which means that their drifts under P are restricted by the need to be a simple change of measure away from a martingale. In other words, the market price of risk has to be the same for all bonds, or else there will be an arbitrage opportunity. 

So we have a restriction on the bonds' P-drifts. In particular, it must be the case that, for all maturities T, 

$$
\int_ {t} ^ {T} \alpha (t, u) d u = \frac {1}{2} \Sigma^ {2} (t, T) - \Sigma (t, T) \gamma_ {t}, \qquad t \leqslant T.
$$

Differentiating with respect to $T$ , we see that $\alpha(t, T) = -\sigma(t, T)\Sigma(t, T) + \sigma(t, T)\gamma_t$ , that is 

$$
\alpha (t, T) = \sigma (t, T) (\gamma_ {t} - \Sigma (t, T)).
$$

Exactly as in section 5.2, where $\sigma(t,T) = \sigma$ and $\Sigma(t,T) = -\sigma(T - t)$ , the real world drift $\alpha(t,T)$ cannot be too different from the risk-neutral value of $-\sigma(t,T)\Sigma(t,T)$ . 

Under this risk-neutral measure, the forward rate and the instantaneous rate are then, 

Forward and short rates under Q 

$$
\begin{array}{c} d _ {t} f (t, T) = \sigma (t, T) d \tilde {W} _ {t} - \sigma (t, T) \Sigma (t, T) d t, \\ r _ {t} = f (0, t) + \int_ {0} ^ {t} \sigma (s, t) d \tilde {W} _ {s} - \int_ {0} ^ {t} \sigma (s, t) \Sigma (s, t) d s. \end{array}
$$

Like the bond price itself, these expressions no longer depend on the drift at all, but are solely expressed in terms of the volatilities $\sigma$ and $\Sigma$ . 

## Model conditions

We have been accumulating technical conditions as we have swept through. They are summarised in the box below. 

The first condition is actually necessary and sufficient for there to be an equivalent measure under which every single discounted bond price is a martingale, which guarantees the absence of arbitrage. The second condition is equivalent to asserting that the change of measure is unique, which means that all risks can be hedged using the martingale representation theorem. The last two conditions are technical requirements for C-M-G to operate and to make sure that Z is a martingale under the new measure. 

Single-factor HJM: market completeness conditions
It is required that
• there exists an F-previsible process $\gamma_{t}$ , such that $\alpha(t,T)=\sigma(t,T)(\gamma_{t}-\Sigma(t,T))$ , for all $t\leqslant T$ ;
• the process $A_{t}=\Sigma(t,T)$ is non-zero for almost all $(t,\omega)$ , t<T, for every maturity T;
• the expectation $E\exp\frac{1}{2}\int_{0}^{T}\gamma_{t}^{2}dt$ is finite;
• and the expectation $E\exp\frac{1}{2}\int_{0}^{T}(\gamma_{t}-\Sigma(t,T))^{2}dt$ is finite. 

The importance of the first condition in this box is the constraint it places on the drift $\alpha(t,T)$ . As the process $\gamma_{t}$ is only a function of time and not of maturity, the drift is forced to take the value $-\sigma(t,T)\Sigma(t,T)$ modified only by the ‘one-dimensional’ displacement $\gamma_{t}\sigma(t,T)$ . Given that $\sigma(t,T)$ and $\Sigma(t,T)$ are determined by the forward rate volatilities, the only degree of freedom for the drift comes from the one-parameter $\gamma_{t}$ process. Unlike simple asset models, not all drift functions $\alpha(t,T)$ are allowable. 

## 5.4 Short-rate models

Short-rate models are popular in the market. In particular, they are often used to price derivatives which depend only on one underlying bond. They have evolved from various historical starting points – some emerging from discrete frameworks, others from equilibrium models – and are often presented in a simple hierarchy with no apparent connection to any overarching model. 

All however are HJM models, which is why we used this framework in the first place. And there is a mathematical transformation that makes these two alternative descriptions equivalent. Demonstrating that is the purpose of this section. 

A short-rate model posits a risk-neutral measure Q and a short-rate process $r_{t}$ . The model is that instantaneous borrowing can take place at rate $r_{t}$ for an infinitesimal period. Rolling up the periods gives rise to a cash bond process $B_{t} = \exp\left(\int_{0}^{t} r_{s} ds\right)$ , as in the HJM model. As with the equations at the end of section 5.3, the bond prices are given by 

$$
P (t, T) = \mathbb {E} _ {\mathbb {Q}} \left(\exp \left(- \int_ {t} ^ {T} r _ {s} d s\right) \mid \mathcal {F} _ {t}\right),
$$

and the value at time t of a claim X maturing at date T is 

$$
V _ {t} = \mathbb {E} _ {\mathbb {Q}} \left(\exp \left(- \int_ {t} ^ {T} r _ {s} d s\right) X \mid \mathcal {F} _ {t}\right).
$$

The paradigm of short-rate modelling is to work within a parameterised family of processes, which typically are Markovian. The parameters are chosen to best fit the market, and then the above expression for $V_{t}$ is calculated to price the claim X. 

## HJM in terms of the short rate

It is not immediately clear that this is an HJM model. To prove this requires choosing the forward volatility surface $\sigma(t,T)$ so that the resulting short rate from the HJM model is exactly the same as the original process $r_{t}$ . This is possible for any general short rate $r_{t}$ , but it's easiest to show in the special case where $r_{t}$ is a Markov process. 

Suppose that that $r_{t}$ is a Markov diffusion (though not necessarily time-homogeneous) with volatility $\rho(r_{t}, t)$ and drift $\nu(r_{t}, t)$ . That is 

$$
d r _ {t} = \rho (r _ {t}, t) d W _ {t} + \nu (r _ {t}, t) d t,
$$

where $\rho(x,t)$ and $\nu(x,t)$ are deterministic functions of space and time. 

Then $\int_t^T f(t,u)du = -\log P(t,T) = g(r_t,t,T)$ , where $g(x,t,T)$ is the deterministic function 

$$
g (x, t, T) = - \log \mathbb {E} _ {\mathbb {Q}} \left(\exp \left(- \int_ {t} ^ {T} r _ {s} d s\right) \mid r _ {t} = x\right).
$$

There is a theorem: 

## Short-rate model in HJM terms

The required volatility structure is 

$$
\sigma (t, T) = \rho (r _ {t}, t) \frac {\partial^ {2} g}{\partial x \partial T} (r _ {t}, t, T),
$$

$$
\text { and } \quad \Sigma (t, T) = - \rho (r _ {t}, t) \frac {\partial g}{\partial x} (r _ {t}, t, T).
$$

## 5.4 Short-rate models

We can see why this is so, by thinking of the forward rate $f(t,T)$ as $\frac{\partial g}{\partial T}(r_{t},t,T)$ , and using Itô to deduce that 

$$
d _ {t} f (t, T) = \frac {\partial^ {2} g}{\partial x \partial T} (\rho (r _ {t}, t) d W _ {t} + \nu (r _ {t}, t) d t) + \frac {\partial^ {2} g}{\partial t \partial T} d t + \frac {1}{2} \frac {\partial^ {3} g}{\partial x ^ {2} \partial T} \rho^ {2} (r _ {t}, t) d t.
$$

The volatility term must match $\sigma(t,T)$ , which gives us the result. In addition, the initial forward rate curve $f(0,T)$ is given by 

$$
f (0, T) = \frac {\partial g}{\partial T} (r _ {0}, 0, T).
$$

This volatility structure and initial curve then identifies an HJM model for this market with the same short rate under Q. 

## Short rate in terms of HJM

Conversely, it is also true that HJM models are short-rate models. The equation for the bond price in terms of $r_{t}$ holds (see near the end of section 5.3), with $r_{t}$ in terms of the HJM volatilities $\sigma(t,T)$ and $\Sigma(t,T)$ , given as 

$$
r _ {t} = f (0, t) + \int_ {0} ^ {t} \sigma (s, t) d W _ {s} - \int_ {0} ^ {t} \sigma (s, t) \Sigma (s, t) d s.
$$

This formula is not necessarily simple. 

## Ho and Lee

Now for the accepted hierarchy of short-rate models: starting with Ho and Lee. In its short-rate form, Ho and Lee gives the SDE for $r_{t}$ under Q, the martingale measure, as 

## Ho and Lee model

The short rate is driven by the SDE: 

$$
d r _ {t} = \sigma d W _ {t} + \theta_ {t} d t,
$$

for some $\theta_{t}$ deterministic and bounded, and $\sigma$ constant. 

The question we should immediately ask is, which HJM model corresponds to this? Following the mechanics from earlier, we find via Itô 

$$
g (x, t, T) = x (T - t) - \frac {1}{6} \sigma^ {2} (T - t) ^ {3} + \int_ {t} ^ {T} (T - s) \theta_ {s} d s.
$$

Thus $\sigma(t,T)$ , the HJM volatility surface, is simply $\sigma\frac{\partial^{2}g}{\partial x\partial T}=\sigma$ . Thus the volatility surface is constant, depending on neither time nor maturity. We can fully specify the HJM model under Q as 

## Ho and Lee model in HJM terms

with 

$$
\begin{array}{c} {d _ {t} f (t, T) = \sigma d W _ {t} + \sigma^ {2} (T - t) d t} \\ {f (0, T) = \frac {\partial g}{\partial T} (r _ {0}, 0, T) = r _ {0} - \frac {1}{2} \sigma^ {2} T ^ {2} + \int_ {0} ^ {T} \theta_ {s} d s.} \end{array}
$$

Equivalently, we can provide the evolution of the bond prices $P(t,T)$ under Q: 

$$
P (t, T) = \exp - \left(\sigma (T - t) W _ {t} + \int_ {t} ^ {T} f (0, u) d u + \frac {1}{2} \sigma^ {2} T (T - t) t\right).
$$

This model is the (general) single-factor model with constant volatility, and is actually the simple model of section 5.2. If used in the short-rate form, then $\sigma$ sets the volatility of all forward rates and $\theta_{t}$ allows matching to any initial forward curve via the identity $f(0,T)=r_{0}-\frac{1}{2}\sigma^{2}T^{2}+\int_{0}^{T}\theta_{s}ds$ . 

It is a simple model, and its simplicity tells against it – the forward rates and the short rate $r_{t}$ can go negative occasionally, and go to infinity in the long term. And not just of course under Q, but under any equivalent measure P as well. Many other models expend much effort just to avoid these pitfalls. 

But it is not that simple a model – the HJM formulation allows a description of how the real forward curve can move over time. Given any previsible process $\gamma_{t}$ , the forward rates can move as 

$$
\begin{array}{r} d _ {t} f (t, T) = \sigma d W _ {t} + (\sigma^ {2} (T - t) + \sigma \gamma_ {t}) d t, \\ \mathrm{with} \quad d r _ {t} = \sigma d W _ {t} + (\theta_ {t} + \sigma \gamma_ {t}) d t. \end{array}
$$

## 5.4 Short-rate models

So short rates can have a wide range of possible drifts under P the real world measure, not just the simple deterministic drift $\theta_{t}$ . The restriction with Ho and Lee lies not there but in the implication that $\sigma(t,T)=\sigma$ . 

Two extra things need mentioning. First, the bond price and the cash bond price are both log-normally distributed and thus the Black–Scholes formula can still hold (as hinted at in section 4.1, and shown in section 6.2). 

And second, there is a straightforward generalisation to a deterministic short-rate volatility 

$$
d r _ {t} = \sigma_ {t} d W _ {t} + \theta_ {t} d t,
$$

with a corresponding HJM formulation 

$$
d _ {t} f (t, T) = \sigma_ {t} d W _ {t} + \sigma_ {t} ^ {2} (T - t) d t,
$$

with the initial forward rate curve given by 

$$
f (0, T) = r _ {0} - \int_ {0} ^ {T} \sigma_ {s} ^ {2} (T - s) d s + \int_ {0} ^ {T} \theta_ {s} d s.
$$

The extra freedom here is to allow the volatility surface to depend on time, but not on maturity. For that we require something else... 

## Vasicek/Hull-White

Next in the accepted hierarchy is to allow the short rate's drift to depend on its current value. 

## Vasicek model

We model the short rate (under Q) as: 

$$
d r _ {t} = \sigma d W _ {t} + (\theta - \alpha r _ {t}) d t
$$

for some constant $\alpha, \theta$ and $\sigma$ . 

The SDE is composed of a Brownian part and a restoring drift which pushes it upwards when the process is below $\theta/\alpha$ and downwards when it is above. The magnitude of the drift is also proportional to the distance away from this mean. Such a process is called an Ornstein–Uhlenbeck or O-U process. 

We can use Itô's formula to check that the solution to this, starting r at $r_{0}$ , is 

$$
r _ {t} = \theta / \alpha + e ^ {- \alpha t} (r _ {0} - \theta / \alpha) + \sigma e ^ {- \alpha t} \int_ {0} ^ {t} e ^ {\alpha s} d W _ {s}.
$$

As it happens, $r_{t}$ can be rewritten in terms of a different Q-Brownian motion $\bar{W}$ as 

$$
r _ {t} = \theta / \alpha + e ^ {- \alpha t} (r _ {0} - \theta / \alpha) + \sigma e ^ {- \alpha t} \bar {W} \left(\frac {e ^ {2 \alpha t} - 1}{2 \alpha}\right),
$$

so that $r_t$ has a normal marginal distribution with mean $\theta / \alpha + \exp(-\alpha t) (r_0 - \theta / \alpha)$ and variance $\sigma^2 (1 - \exp(-2\alpha t)) / 2\alpha$ . As $t$ gets large, this converges to an equilibrium normal distribution of mean $\theta / \alpha$ and variance $\sigma^2 / 2\alpha$ . This does not mean that the process $r_t$ converges – it doesn't – only that its distribution converges. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/61081d581436aeca22a9404cdbebfc29478f40d9460477c3ecd4b356339f15d3.jpg)



Figure 5.7 An O-U process, with $\sigma = 2\theta = 2\alpha = 1$


What HJM model are we in? Again we can use Itô to find $g(x,t,T)$ , and thus $\sigma(t,T)$ and $f(0,T)$ . In this case 

Vasicek model in HJM terms 

$$
\begin{array}{l l} & \sigma (t, T) = \sigma \exp (- \alpha (T - t)), \\ \text {with} & f (0, T) = \theta / \alpha + e ^ {- \alpha T} (r _ {0} - \theta / \alpha) - \frac {\sigma^ {2}}{2 \alpha^ {2}} \big (1 - e ^ {- \alpha T} \big) ^ {2}. \end{array}
$$

Now we can see an advantage over Ho and Lee - where Ho and Lee failed to introduce a maturity dependence into the volatility surface, this model can. Thus this model is capable of calibration to a richer set of observed volatilities. Note how the volatility $\sigma(t,T)$ is derived from both the drift and volatility 

## 5.4 Short-rate models

of the short rate under $\mathbb{Q}$ . In order to describe an HJM model, we need two degrees of freedom for the volatility - one for time and one for maturity. The short rate description doesn't abandon the second degree of freedom; it encodes it in the relationship between its volatility $\rho(r_t, t)$ and its drift $\nu(r_t, t)$ . The drift of $r_t$ under $\mathbb{Q}$ is a vital part of the description. 

But only under Q. The Vasicek model, unlike Ho and Lee, may be mean reverting under Q, but both models are in fact capable of mean reversion under P. Some care has to be taken – the introduction of the extra parameter $\alpha$ does give Vasicek a richer set of allowable P-drifts than Ho and Lee, but this richness involves maturity. Simple time-dependent considerations will not in general prejudice one over the other. Because it is possible to find a change of measure $\gamma_{t}$ which gives mean reverting behaviour to Ho and Lee, Vasicek is not the inevitable choice if in the real world mean reversion is observed. In practice it will be the volatility of the entire curve, rather than the drift of the short rate that forces one over the other. 

As before there is a natural generalisation to 

$$
d r _ {t} = \sigma_ {t} d W _ {t} + (\theta_ {t} - \alpha_ {t} r _ {t}) d t
$$

where $\sigma_{t}$ , $\theta_{t}$ , and $\alpha_{t}$ are deterministic functions of time. As $r_{t}$ is still a Gaussian process with normal marginals, so $f(t,T)$ is Gaussian and the bond prices have log-normal marginals. In this case, the HJM volatility and initial forward curve are 

$$
\begin{array}{l} \sigma (t, T) = \sigma_ {t} \beta (t, T), \qquad \text {where} \quad \beta (t, T) = \exp \Bigl (- \int_ {t} ^ {T} \alpha_ {s} d s \Bigr), \qquad \text {and} \\ f (0, T) = r _ {0} \beta (0, T) + \int_ {0} ^ {T} \theta_ {s} \beta (s, T) d s - \int_ {0} ^ {T} \sigma_ {s} ^ {2} \beta (s, T) \left(\int_ {s} ^ {T} \beta (s, u) d u\right) d s. \end{array}
$$

The normality of the forward rates $f(t,T)$ is both good news and bad news. In its favour, it means that the bond prices $P(t,T)$ are log-normally distributed, so that the log-normal option pricing results of section 6.2 all hold. On the other hand, both the instantaneous rate and the forward rates can go negative from time to time. Depending on the parameters, this can happen more or less rarely – the next model rectifies this defect. 

## Cox-Ingersoll-Ross

The model is a mean-reverting process, which pushes away from zero to keep it positive (see box). 

## Cox-Ingersoll-Ross model

The instantaneous rate's SDE, under $\mathbb{Q}$ , is 

$$
d r _ {t} = \sigma_ {t} \sqrt {r _ {t}} d W _ {t} + (\theta_ {t} - \alpha_ {t} r _ {t}) d t,
$$

where $\sigma_{t}$ , $\theta_{t}$ and $\alpha_{t}$ are deterministic functions of time. 

The drift term is a restoring force which always points towards the current mean value of $\theta_{t}/\alpha_{t}$ . The volatility term is set up to get smaller as $r_{t}$ approaches zero, so allowing the drift $\theta_{t}$ to dominate and to stop $r_{t}$ from going below zero. 

As long as $\theta$ satisfies $\theta_t \geqslant \frac{1}{2}\sigma_t^2$ , then the process actually stays strictly positive. 

This process is called autoregressive. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/6c38200f1f3186dcd05a8a3026f96566489d038b9084e06f8fe90149f40ea341.jpg)



Figure 5.8 Autoregressive $\sigma = 1, \theta = 2, \alpha = 2$


It is difficult to find an explicit pathwise solution for $r_{t}$ , but we can solve a useful partial differential equation (PDE). Firstly define $B(t,T)$ to be the solution of the Riccati differential equation 

$$
\frac {\partial B}{\partial t} = \frac {1}{2} \sigma_ {t} ^ {2} B ^ {2} (t, T) + \alpha_ {t} B (t, T) - 1, \qquad B (T, T) = 0.
$$

## 5.4 Short-rate models

(In general, this equation has no analytic solution, but it has been well studied numerically.) Then the function $g(x,t,T)$ , which is $(-\log P(t,T)|r_{t}=x)$ can be written in terms of this solution $B(t,T)$ as 

$$
g (x, t, T) = x B (t, T) + \int_ {t} ^ {T} \theta_ {s} B (s, T) d s.
$$

Letting $D(t, T)$ be $\frac{\partial B}{\partial T}(t, T)$ , then the volatility structure can be expressed as 

## Cox-Ingersoll-Ross in HJM terms

$$
\sigma (t, T) = \sigma_ {t} \sqrt {r _ {t}} D (t, T),
$$

$$
\text { and } \quad \Sigma (t, T) = - \sigma_ {t} \sqrt {r _ {t}}   B (t, T),
$$

$$
\text { with } \quad f (0, T) = r _ {0} D (0, T) + \int_ {0} ^ {T} \theta_ {s} D (s, T)   d s.
$$

As usual, the bond price $P(t,T)$ has the form $P(t,T) = \exp - g(r_t,t,T)$ . 

## Black-Karasinski

Another way round the problem of keeping the short rate positive is to take exponentials. This model is an extension of the Black–Derman–Toy model and starts by taking $X_{t}$ to be the general O-U process of the Vasicek model. Explicitly: 

## Black-Karasinski model

The process $X_{t}$ is 

$$
d X _ {t} = \sigma_ {t} d W _ {t} + (\theta_ {t} - \alpha_ {t} X _ {t}) d t,
$$

where $\sigma_{t}$ , $\theta_{t}$ and $\alpha_{t}$ are deterministic functions of time. The instantaneous rate $r_{t}$ is then assumed to be 

$$
r _ {t} = \exp (X _ {t}).
$$

So the logarithm of the rate drifts towards the current mean of $\theta_{t}/\alpha_{t}$ . 

The rate itself also drifts towards a mean, and additionally is always positive. We also know that $X_{t}$ is normally distributed, so that $r_{t}$ is log-normal. However, $\int_{t}^{T} r_{s} ds$ is awkward to examine analytically. This model is still HJM consistent; that is, there is some volatility surface $\sigma(t, T)$ which generates a single-factor HJM model which has the same instantaneous rate as given above. 

## 5.5 Multi-factor HJM

The drawback of the single-factor model is that all the increments in the bond prices are perfectly correlated. For many applications, that assumption is too coarse, especially if we are trying to price something which depends on the difference of two points on the yield curve. 

A multi-factor model involves driving the various processes by a collection of independent Brownian motions. More details of such models are in section 6.3. In an n-factor model, we will have n Brownian motions to work with: $W_{1}(t), \ldots, W_{n}(t)$ . Correspondingly each T-bond forward rate process has a volatility $\sigma_{i}(t, T)$ for each Brownian factor $W_{i}(t)$ . This allows different bonds to depend on external ‘shocks’ in different ways, and to have strong correlations with some bonds and weaker correlations with others. The general form of the multi-factor HJM model is 

$$
f (t, T) = f (0, T) + \sum_ {i = 1} ^ {n} \int_ {0} ^ {t} \sigma_ {i} (s, T) d W _ {i} (s) + \int_ {0} ^ {t} \alpha (s, T) d s, \quad 0 \leqslant t \leqslant T,
$$

which is to say that the forward process starts with initial value $f(0,T)$ and is driven by various Brownian terms and a drift. From this, the total instantaneous square volatility of $f(t,T)$ , and the covariance of the increments of the two forward rates $f(t,T)$ and $f(t,S)$ are respectively 

$$
\sum_ {i = 1} ^ {n} \sigma_ {i} ^ {2} (t, T), \quad \text { and } \quad \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T) \sigma_ {i} (t, S).
$$

In the single-factor model, n is 1, and the correlation of the changes in the forward rates of the T-bond and S-bond is exactly one. 

The instantaneous rate $r_t = f(t, t)$ can be written, similarly to before as 

$$
r _ {t} = f (0, t) + \sum_ {i = 1} ^ {n} \int_ {0} ^ {t} \sigma_ {i} (s, t) d W _ {i} (s) + \int_ {0} ^ {t} \alpha (s, t) d s.
$$

The volatility and drift conditions are generalised to: 

## Multi-factor HJM: conditions on the volatilities and drift We assume that

- for each $T$ , the processes $\sigma_{i}(t,T)$ and $\alpha(t,T)$ are $\mathcal{F}$ -previsible and their integrals $\int_0^T \sigma_i^2(t,T) dt$ and $\int_0^T |\alpha(t,T)| dt$ are finite; 

- the initial forward curve, $f(0,T)$ , is deterministic and satisfies the condition that $\int_0^T |f(0,u)|du < \infty$ ; 

- the drift $\alpha$ has finite integral $\int_0^T\int_0^u |\alpha (t,u)|dtdu;$ 

- each volatility $\sigma_{i}$ has finite expectation $\mathbb{E}\int_{0}^{T}\left|\int_{0}^{u}\sigma_{i}(t,u)dW_{i}(t)\right|du$ . 

To make the discounted bond prices into martingales, we need a version of the Cameron–Martin–Girsanov theorem for higher dimensions (section 6.3). The conditions we need for this to work are shown in the two boxes, where $\Sigma_{i}(t,T)$ is the integral $-\int_{t}^{T}\sigma_{i}(t,u)du$ . 

## Multi-factor HJM: market completeness conditions (1) It is required that

- there exist previsible processes $\gamma_{i}(t)$ , for $1 \leqslant i \leqslant n$ , such that 

$$
\alpha (t, T) = \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T) \big (\gamma_ {i} (t) - \Sigma_ {i} (t, T) \big), \quad \text { for   all } t \leqslant T;
$$

• the expectation $E \exp \frac{1}{2} \sum_{i}^{n} \int_{0}^{T} \gamma_{i}^{2}(t) dt$ is finite; 

This is just as in the single-factor case, but with one difference. The drift is now allowed n ‘dimensions of freedom’ away from its risk-neutral value. That is, as a function of T, $\alpha(t,\cdot)$ is allowed to deviate by any linear combination of the functions $\sigma_{i}(t,\cdot)$ . This is still much less than the set of all possible functions, but it is larger than in the single-factor case. The second condition is the technical requirement of the C-M-G theorem for $\gamma_{i}(t)$ to be a drift under an equivalent change of measure. 

## Multi-factor HJM: market completeness conditions (2)

We also need that 

- the matrix $A_{t} = \left( \Sigma_{i}(t, T_{j}) \right)_{i,j=1}^{n}$ is non-singular for almost all $(t, \omega)$ , $t < T_{1}$ , for every set of maturities $T_{1} < T_{2} < \ldots < T_{n}$ ; 

• and the expectation $E \exp \frac{1}{2} \sum_{i}^{n} \int_{0}^{T} (\gamma_{i}(t) - \Sigma_{i}(t, T))^{2} dt$ is finite. 

The modification from the single-factor case here is that the volatility process $A_{t}$ which used to be required to be non-zero has been replaced by a volatility matrix process which has to be non-singular. The second condition ensures that the resulting driftless discounted bond price is in fact a martingale (a multi-dimensional equivalent of the collector's guide to exponential martingales). 

As before we find that the bond prices themselves have stochastic increments 

$$
\begin{array}{l} d _ {t} P (t, T) = P (t, T) \left(\sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) d W _ {i} (t) \dots \right. \\ \left. + \left(r _ {t} - \int_ {t} ^ {T} (\alpha (t, u) + \sum_ {i = 1} ^ {n} \sigma_ {i} (t, u) \Sigma_ {i} (t, u)) d u\right) d t\right), \end{array}
$$

where $\Sigma_{i}(t,T)$ is the integral $-\int_{t}^{T}\sigma_{i}(t,u)du$ . The discounted bond prices $Z(t,T) = B_{t}^{-1}P(t,T)$ satisfy 

$$
\begin{array}{l} d _ {t} Z (t, T) = Z (t, T) \left(\sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) d W _ {i} (t) \right. \\ \left. - \left(\int_ {t} ^ {T} (\alpha (t, u) + \sum_ {i} \sigma_ {i} (t, u) \Sigma_ {i} (t, u)) d u\right) d t\right). \end{array}
$$

The SDE for Z now becomes 

$$
d _ {t} Z (t, T) = Z (t, T) \sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) \left(d W _ {i} (t) + \gamma_ {i} (t) d t\right).
$$

Using the multi-dimensional C-M-G, we can find a measure Q equivalent to P, under which $\tilde{W}_{1},\ldots,\tilde{W}_{n}$ are independent Q-Brownian motions, where $\tilde{W}_{i}(t)=W_{i}(t)+\int_{0}^{t}\gamma_{i}(s)ds$ . So Z's SDE is (in Q-terms) 

$$
d _ {t} Z (t, T) = Z (t, T) \sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) d \tilde {W} _ {i} (t),
$$

and every $Z(t,T)$ is a $\mathbb{Q}$ -martingale in $t$ . 

Under this martingale measure, the bond price P and the forward rate f have the stochastic differentials 

Bond prices and forward rates under $\mathbb{Q}$ 

$$
d _ {t} P (t, T) = P (t, T) \left(\sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) d \tilde {W} _ {i} (t) + r _ {t} d t\right),
$$

$$
d _ {t} f (t, T) = \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T) d \tilde {W} _ {i} (t) - \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T) \Sigma_ {i} (t, T) d t.
$$

## Derivative pricing and hedging

The actual price of a derivative still has a familiar form: 

## Option price formula (HJM)

If X is the payoff of a derivative at time T, then its value at time t is 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right) = \mathbb {E} _ {\mathbb {Q}} \left(\exp \left(- \int_ {t} ^ {T} r _ {s} d s\right) X \mid \mathcal {F} _ {t}\right).
$$

We also need a multi-dimensional martingale representation theorem. Formally 

## Martingale representation theorem (n-factor)

Let $\tilde{W}$ be $n$ -dimensional $\mathbb{Q}$ -Brownian motion, and suppose that $M_t$ is an $n$ -dimensional $\mathbb{Q}$ -martingale process, $M_t = (M_1(t), \ldots, M_n(t))$ , which has volatility matrix $(\sigma_{ij}(t))$ , in that $dM_j(t) = \sum_i \sigma_{ij}(t) d\tilde{W}_i(t)$ , and the matrix satisfies the additional condition that (with probability one) it is always non-singular. Then if $N_t$ is any one-dimensional $\mathbb{Q}$ -martingale, there exists an $n$ -dimensional $\mathcal{F}$ -previsible process $\phi_t = (\phi_1(t), \ldots, \phi_n(t))$ such that $\int_0^T (\sum_j \sigma_{ij}(t) \phi_j(t))^2 dt < \infty$ , and the martingale $N$ can be written as 

$$
N _ {t} = N _ {0} + \sum_ {j = 1} ^ {n} \int_ {0} ^ {t} \phi_ {j} (s) d M _ {j} (s).
$$

Further $\phi$ is (essentially) unique. 

As a general rule, if we have an n-factor model, we need a trading portfolio of n separate instruments, as well as the cash bond, in order to hedge claims. An advantage of the HJM framework is that we are free to choose whichever n instruments we like, and the answer will always be the same. 

If we are going to hedge the claim X with discount bonds, we must still make sure that all their maturities are later than T. Suppose we choose to use bonds with maturities $T_{1}, T_{2}, \ldots, T_{n}$ all larger than T. 

A self-financing strategy $(\phi_{1}(t),\ldots,\phi_{n}(t),\psi_{t})$ will be the combination of both an n-vector of holdings in the bonds with maturities $T_{1},\ldots,T_{n}$ respectively, and a holding $\psi_{t}$ in the cash bond $B_{t}$ . The value of the portfolio at time t is 

$$
V _ {t} = \sum_ {j = 1} ^ {n} \phi_ {j} (t) P (t, T _ {j}) + \psi_ {t} B _ {t},
$$

and its discounted value $E_{t} = B_{t}^{-1}V_{t}$ is 

$$
E _ {t} = \sum_ {j = 1} ^ {n} \phi_ {j} (t) Z (t, T _ {j}) + \psi_ {t}.
$$

The self-financing equality for the strategy (as in section 6.4) is that 

$$
d E _ {t} = \sum_ {j = 1} ^ {n} \phi_ {j} (t) d _ {t} Z (t, T _ {j}).
$$

## 5.6 Interest rate products

We can now apply the representation theorem in the usual way to the martingale produced from the discounted claim, that is $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ . The part of the martingales $M_{j}(t)$ will be taken by the discounted bonds $Z(t,T_{j})$ . Their volatility matrix is given by $A_{t} = (\Sigma_{i}(t,T_{j}))_{i,j}$ , which is non-singular by the completeness conditions box. If we set $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ , then by the representation theorem, there is an n-vector of previsible processes $\phi_{t}$ such that 

$$
E _ {t} = \mathbb {E} _ {\mathbb {Q}} (B _ {T} ^ {- 1} X) + \sum_ {j = 1} ^ {n} \int_ {0} ^ {t} \phi_ {j} (s) d Z (s, T _ {j}).
$$

This immediately gives a self-financing strategy $\phi$ . We hold $\phi_{j}(t)$ units of the $T_{j}$ -bond at time t, and $\psi_{t}=E_{t}-\sum_{j}\phi_{j}(t)Z(t,T_{j})$ units of the cash bond. 

In the usual way, the portfolio costs an initial $\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X)$ and evolves to be worth exactly X by time T. 

## 5.6 Interest rate products

In recent years, there has been a great increase in the number of interest rate products available. Especially in the over-the-counter markets, contracts which not long ago would have been considered as exotics are now commonplace. We cannot hope to describe the hundreds and possibly thousands of traded claims, but we can sketch out the basic types within each area. 

## Forward contract

This is about the simplest product possible. We agree, at the current time t, to make a payment of an amount k at a future time $T_{1}$ , and in return to receive a dollar at the later time $T_{2}$ . What should the amount k be? 

According to the pricing formula (under whatever model we are in), the value of the claim now is 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} (B _ {T _ {2}} ^ {- 1} | \mathcal {F} _ {t}) - B _ {t} \mathbb {E} _ {\mathbb {Q}} (k B _ {T _ {1}} ^ {- 1} | \mathcal {F} _ {t}),
$$

under the martingale measure $\mathbb{Q}$ , where $B_{t}$ is the cash bond 

$$
B _ {t} = \exp \int_ {0} ^ {t} r _ {s} d s.
$$

Recalling that $B_{t}\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}|\mathcal{F}_{t})$ is just $P(t,T)$ , we see that 

$$
V _ {t} = P (t, T _ {2}) - k P (t, T _ {1}).
$$

For this contract to have null current net worth, we merely choose k at time t to be 

$$
k = \frac {P (t , T _ {2})}{P (t , T _ {1})}.
$$

This price makes sense, as saying that the forward yield from $T_{1}$ to $T_{2}$ is 

$$
- \frac {\log P (t , T _ {2}) - \log P (t , T _ {1})}{T _ {2} - T _ {1}}.
$$

For $T_{1}$ and $T_{2}$ very close together, this approximates to the instantaneous forward rate of borrowing 

$$
- \frac {\partial}{\partial T} \log P (t, T) = f (t, T).
$$

The price also gives us a clue to the hedging strategy. Suppose we were, at time t, to buy k units of the $T_{1}$ -bond and sell one unit of the $T_{2}$ -bond. The initial cost of that deal is zero, and the portfolio pays us k at time $T_{1}$ (matching the payment we have to make at that time) and exactly absorbs the dollar we receive at time $T_{2}$ . 

In this particular example, the answer is independent of our particular term structure model, as the hedging strategy is static. There are other important cases where this also happens. 

## Multiple payment contracts

Most interest rate products don't just make a single payment $X$ at time $T$ . Instead the contract specifies a sequence of payments $X_{i}$ made at a sequence of times $T_{i} (i = 1, \ldots, n)$ . Each payment $X_{i}$ may depend on price movements up to its payment time $T_{i}$ , and even on any previous payment. As long as we bear that in mind, this causes no serious problem, and indeed there are two different ways to keep things clear. 

- Divide and rule. We can treat each payment $X_{i}$ separately. On its own, it is just a claim at time $T_{i}$ , so its worth at time $t$ is 

$$
V _ {i} (t) = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T _ {i}} ^ {- 1} X _ {i} \mid \mathcal {F} _ {t}\right) = P (t, T _ {i}) \mathbb {E} _ {\mathbb {P} _ {T _ {i}}} (X | \mathcal {F} _ {t}),
$$

## 5.6 Interest rate products

where $P_{T_{i}}$ is the $T_{i}$ -forward measure (see section 6.4). This approach will always work, but the forward measure, if used, will have to be changed for each i. 

- Savings account. We could instead roll up the payments into savings as we get them, and keep them till the last payment date $T$ . That is, as each payment is made, we use it to buy a $T$ -bond (or invest it in the bank account process $B_t$ till time $T$ ). Then the payoff is a single payment at time $T$ of 

$$
X = \sum_ {i = 1} ^ {n} \frac {X _ {i}}{P (T _ {i} , T)}
$$

with worth at time t 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} X \big | \mathcal {F} _ {t} \big) = P (t, T) \mathbb {E} _ {\mathbb {P} _ {T}} (X | \mathcal {F} _ {t}).
$$

## Bonds with coupons

In practice, pure discount bonds with no coupon are not popular products. Especially at the long end. Instead, a bond may not only pay its principal back at maturity, but also make smaller regular coupon payments of a fixed amount c up until then. 

Suppose a bond makes n regular payments at (uncompounded) rate k at times $T_{i} = T_{0} + i\delta$ ( $i = 1, \ldots, n$ ) and also pays off a dollar at time $T_{n}$ . The amount of the actual coupon payment is $k\delta$ , where $\delta$ is the payment period. This income stream is equivalent to owning one $T_{n}$ -bond and $k\delta$ units of each $T_{i}$ -bond. The price of the coupon bond at time $T_{0}$ is 

$$
P (T _ {0}, T _ {n}) + k \delta \sum_ {i = 1} ^ {n} P (T _ {0}, T _ {i}).
$$

If we desire the bond to start with its face value, then the coupon rate should be 

$$
k = \frac {1 - P (T _ {0} , T _ {n})}{\delta \sum_ {i = 1} ^ {n} P (T _ {0} , T _ {i})}.
$$

## Floating rate bonds

A bond might also pay off a coupon which was not fixed, but depended on current interest rates. One interesting case is where the interest paid over an interval from time S to time T is the same as the yield of the T-bond bought at time S. 

Suppose a bond pays its dollar principal at time $T_{n}$ , and also payments at times $T_{i} = T_{0} + i\delta (i = 1, \ldots, n)$ of varying amounts. The amount of payment made at time $T_{i}$ is determined by the LIBOR rate set at time $T_{i-1}$ 

$$
L (T _ {i - 1}) = \frac {1}{\delta} \left(\frac {1}{P (T _ {i - 1} , T _ {i})} - 1\right).
$$

The actual payment made at time $T_{i}$ is $\delta L(T_{i-1}) = P(T_{i-1}, T_{i})^{-1} - 1$ , which is the amount of interest we would receive by buying a dollar's worth of the $T_{i}$ bond at time $T_{i-1}$ . 

The value to us now, at time $T_{0}$ , of the $T_{i}$ payment is 

$$
B _ {T _ {0}} \mathbb {E} _ {\mathbb {Q}} \big (B _ {T _ {i}} ^ {- 1} (P ^ {- 1} (T _ {i - 1}, T _ {i}) - 1) \mid \mathcal {F} _ {T _ {0}} \big).
$$

Because the conditional expectation $\mathbb{E}_{\mathbb{Q}}(B_{T_{i}}^{-1}|\mathcal{F}_{T_{i-1}})$ is $B_{T_{i-1}}^{-1}P(T_{i-1},T_{i})$ , and the bond price $P(T_{i-1},T_{i})$ is known with respect to the $F_{T_{i-1}}$ -information, we can divide it through both sides to get 

$$
\mathbb {E} _ {\mathbb {Q}} \left(B _ {T _ {i}} ^ {- 1} P ^ {- 1} (T _ {i - 1}, T _ {i}) \mid \mathcal {F} _ {T _ {i - 1}}\right) = B _ {T _ {i - 1}} ^ {- 1}.
$$

Using the tower law, we can rewrite the value of the $T_{i}$ payment as 

$$
B _ {T _ {0}} \mathbb {E} _ {\mathbb {Q}} \big (B _ {T _ {i - 1}} ^ {- 1} - B _ {T _ {i}} ^ {- 1} \big | \mathcal {F} _ {T _ {0}} \big),
$$

which is just $P(T_{0}, T_{i-1}) - P(T_{0}, T_{i})$ . This price also suggests the hedge of selling a $T_{i}$ -bond and buying a $T_{i-1}$ -bond. When the $T_{i-1}$ -bond matures, we buy $P^{-1}(T_{i-1}, T_{i})$ units of the $T_{i}$ -bond, and we are left with exactly the right payoff at time $T_{i}$ . 

The total value of the variable coupon bond is the sum of its components. That is, 

$$
V _ {0} = P (T _ {0}, T _ {n}) + \sum_ {i = 1} ^ {n} \left(P (T _ {0}, T _ {i - 1}) - P (T _ {0}, T _ {i})\right) = 1.
$$

## 5.6 Interest rate products

Surprisingly, the bond has a fixed price equal to the face value of its principal. Why this is so, is because the bond is equivalent to this simple sequence of trades: 

• take a dollar and buy $T_{1}$ -bonds with it 

- take the interest from the bonds at $T_{1}$ as a coupon, and buy some $T_{2}$ -bonds with the dollar principal 

- repeat until we are left with the dollar at time $T_{n}$ . 

This has exactly the same cash flows as the variable coupon bond, so the initial prices must match. 

## Swaps

This very popular contract simply exchanges a stream of varying payments for a stream of fixed amount payments (or vice versa). That is, we swap a floating interest rate for a fixed one. 

Typically, we might offer a contract where we receive a regular sequence of fixed amounts and at each payment date we pay an amount depending on prevailing interest rates. In practice, only the net difference is exchanged, as shown in figure 5.9: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/17b0d2612afafe417460e5fc16c296eb7bf806c6fd488dea8e28e72783489296.jpg)



Figure 5.9


A standard definition of the variable payment is that of the interest paid by a bond over the previous time period. If the payment dates are $T_{i} = T_{0} + i\delta$ ( $i = 1, \ldots, n$ ), then the ith payment will be determined by the $\delta$ -period 

LIBOR rate set at time $T_{i-1}$ . The payment made is 

$$
\delta L (T _ {i - 1}) = \frac {1}{P (T _ {i - 1} , T _ {i})} - 1.
$$

Suppose the swap pays at a fixed rate k at each time period. Then the swap looks like a portfolio which is long a fixed coupon bond and short a variable coupon bond. We know that the former is worth 

$$
P (T _ {0}, T _ {n}) + k \delta \sum_ {i = 1} ^ {n} P (T _ {0}, T _ {i}),
$$

and the latter costs a dollar. The fixed rate needed to give the swap initial null value is 

$$
k = \frac {1 - P (T _ {0} , T _ {n})}{\delta \sum_ {i = 1} ^ {n} P (T _ {0} , T _ {i})}.
$$

## Forward swaps

In a forward swap agreement, we have chosen to receive fixed payments at rate k, starting at time $T_{0}$ with payments at times $T_{i}=T_{0}+i\delta(i=1,\ldots,n)$ . The value of this swap at time $T_{0}$ will be 

$$
X = P (T _ {0}, T _ {n}) + k \delta \sum_ {i = 1} ^ {n} P (T _ {0}, T _ {i}) - 1.
$$

The present value of X at time t before $T_{0}$ is given by the formula: 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T _ {0}} ^ {- 1} X \mid \mathcal {F} _ {t}\right) = P (t, T _ {n}) + k \delta \sum_ {i = 1} ^ {n} P (t, T _ {i}) - P (t, T _ {0}).
$$

The fixed rate needed to give the forward swap initial null value at time t is 

$$
k = \frac {P (t , T _ {0}) - P (t , T _ {n})}{\delta \sum_ {i = 1} ^ {n} P (t , T _ {i})}.
$$

This rate k is the forward swap rate. An alternative formulation of this expression is 

$$
k = \frac {1 - F _ {t} (T _ {0} , T _ {n})}{\delta \sum_ {i = 1} ^ {n} F _ {t} (T _ {0} , T _ {i})},
$$

where $F_{t}(T_{0}, T_{i})$ is the forward price at time t for purchasing a $T_{i}$ -bond at time $T_{0}$ . That is $F_{t}(T_{0}, T_{i}) = P(t, T_{i}) / P(t, T_{0})$ . In this form the expression resembles the instantaneous swap rate. 

## 5.6 Interest rate products

## Bond options

Like a stock option, a bond option gives the right to buy a bond at a future date for a given price. An option on a T-bond, struck at k with exercise time t, has current worth 

$$
\mathbb {E} _ {\mathbb {Q}} \left(B _ {t} ^ {- 1} (P (t, T) - k) ^ {+}\right),
$$

where $\mathbb{Q}$ is the martingale measure. 

Under the Ho and Lee model, where the forward rates evolve as 

$$
d _ {t} f (t, T) = \sigma d W _ {t} + \sigma^ {2} (T - t) d t,
$$

the forward rates and the instantaneous short rate are normally distributed. This makes the T-bond and the discount bond log-normally distributed, so that we can price the option with the log-normal results of section 6.2. The option price is 

$$
V _ {0} = P (0, t) \left(F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \bar {\sigma} ^ {2} t}{\bar {\sigma} \sqrt {t}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \bar {\sigma} ^ {2} t}{\bar {\sigma} \sqrt {t}}\right)\right),
$$

where F is the current forward price for $P(t,T)$ , that is $F = P(0,T)/P(0,t)$ , and the term volatility $\bar{\sigma}$ is $\sigma(T-t)$ (that is, $\bar{\sigma}^{2}t$ is the log-variance of $P(t,T)$ ). Under the Vasicek model, which is the most general single-factor model with log-normal bond prices, this formula also holds with the same forward price, but a different $\bar{\sigma}$ depending on the deterministic processes $\sigma_{t}$ and $\phi_{t}$ in the model. 

Compare this with the price of an option on a stock S, with volatility $\sigma$ , struck at price k with exercise time t. It is worth 

$$
V _ {0} = e ^ {- r t} \left(F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} t}{\sigma \sqrt {t}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} t}{\sigma \sqrt {t}}\right)\right),
$$

where r is the constant interest rate and F is the current forward price of the stock, that is $F = e^{rt} S_{0}$ , and $\sigma$ is the (term) volatility of $S_{t}$ . 

We see that the bond option price formula merely changes the discount factor representing the value now of a dollar at time t. Under constant interest rates this was $e^{rt}$ , and under variable interest rates it is just the price of a t-bond $P(0,t)$ . Otherwise, as long as the other variables are expressed in terms of forward prices and term volatilities, the formula is the same. 

## Options on coupon bonds

Imagine a bond which pays coupons at rate k at the times $T_{i} = T_{0} + i\delta$ ( $i = 1, \ldots, n$ ) before redeeming a dollar at time $T_{n}$ . We can buy or sell the bond before time $T_{n}$ , transferring the ownership of future (but not past) coupons along with it. As we've seen before the value of this bond at time t is 

$$
C _ {t} = P (t, T _ {n}) + k \delta \sum_ {i = I (t)} ^ {n} P (t, T _ {i}),
$$

where $I(t) = \min\{i : t < T_i\}$ is the sequence number of the next coupon payment after time t. 

Suppose we have an option to buy the bond at time t for price K. In general it is not easy to value this option analytically. However, in the special case where we have a single-factor model with a Markovian short rate, we can price the option more easily using a trick of Jamshidian. 

Each bond price $P(t,T)$ can be seen as a deterministic function $P(t,T;r_{t})$ of time, maturity and the instantaneous rate. Additionally, this function will be decreasing in $r_{t}$ – as rates rise, prices fall. A portfolio which is long a number of bonds will have the same behaviour. So $C_{t}$ itself will be a function $C(t;r_{t})$ which is decreasing in $r_{t}$ . 

Thus there is some critical value $r^{*}$ of r such that $C(t;r^{*})$ is exactly K. Setting $K_{i}$ to be $P(t,T_{i};r^{*})$ , then $r^{*}$ is also critical for an option on the $T_{i}$ -bond struck at $K_{i}$ . This means that $C_{t}$ is larger than K if and only if any (and every) $P(t,T_{i})$ is larger than $K_{i}$ . And so 

$$
\left(C _ {t} - K\right) ^ {+} = \left(P (t, T _ {n}) - K _ {n}\right) ^ {+} + k \delta \sum_ {i = I (t)} ^ {n} \left(P (t, T _ {i}) - K _ {i}\right) ^ {+}.
$$

In other words, an option on this portfolio is a portfolio of options, and we can price each one using the zero-coupon bond option formula. 

## Caps and floors

Suppose we are borrowing at a floating rate and want to insure against interest payments going too high. If we make payments at times $T_{i} = T_{0} + i\delta$ ( $i = 1, \ldots, n$ ), then we pay at time $T_{i}$ the $\delta$ -period LIBOR rate set at time $T_{i-1}$ 

$$
L \left(T _ {i - 1}\right) = \frac {1}{\delta} \left(\frac {1}{P \left(T _ {i - 1} , T _ {i}\right)} - 1\right).
$$

## 5.6 Interest rate products

How much would it cost to ensure that this rate is never greater than some fixed rate k? The cap contract pays us the difference between the LIBOR and the cap rate 

$$
\delta \big (L (T _ {i - 1}) - k \big) ^ {+}
$$

at each time $T_{i}$ . An individual payment at a particular time $T_{i}$ is called a caplet, and if we can price caplets, we can price the cap. 

Now we can rewrite the caplet claim as 

$$
X = (1 + k \delta) P _ {i} ^ {- 1} \bigl (K - P _ {i} \bigr) ^ {+},
$$

where $P_{i}$ is $P(T_{i-1}, T_{i})$ and K is $(1 + k\delta)^{-1}$ . The value of the caplet at time t is $B_{t}\mathbb{E}_{\mathbb{Q}}(B_{T_{i}}^{-1}X|\mathcal{F}_{t})$ , which equals 

$$
(1 + k \delta) B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T _ {i - 1}} ^ {- 1} (K - P _ {i}) ^ {+} \mid \mathcal {F} _ {t}\right).
$$

This is just equal to the value of $(1 + k\delta)$ put options on the $T_{i}$ -bond, struck at K, exercised at $T_{i-1}$ . The option price formula (and put-call parity) will then price the caplet. 

A floor works similarly, but inversely, in that we receive a premium for agreeing to never pay less than rate k at each time $T_{i}$ . That is, we pay an extra amount 

$$
\delta \big (k - L (T _ {i - 1}) \big) ^ {+}
$$

at time $T_{i}$ . There is a floor-cap parity which says that the worth of a ‘floorlet’ less the cost of a caplet equals $(1 + k\delta)P(t, T_{i}) - P(t, T_{i-1})$ . Buying a floor and selling a cap at the same strike k is exactly equivalent to receiving fixed at rate k on a swap. 

## Swaptions

A swaption is an option to enter into a swap on a future date at a given rate. Suppose we have an option to receive fixed on a swap starting at date $T_{0}$ . The swap payment dates are $T_{i} = T_{0} + i\delta (i = 1, \ldots, n)$ , and the fixed swap rate is k. Then the worth of the option at time $T_{0}$ is 

$$
\left(P \left(T _ {0}, T _ {n}\right) + k \delta \sum_ {i = 1} ^ {n} P \left(T _ {0}, T _ {i}\right) - 1\right) ^ {+}.
$$

This is exactly the same as a call option, struck at 1, on a $T_{n}$ -bond which pays a coupon at rate k at each time $T_{i}$ . That is not entirely a coincidence as a swap is just a coupon bond less a floating bond (which always has par value). If you receive fixed on a swap, you have a long position in the bond market; a swap option looks like a bond option. 

## 5.7 Multi-factor models

If we want to price a product depending on a range of bonds, it makes more sense to use a multi-factor model. A simple case is given in Heath-Jarrow-Morton's original paper. It is an extension of Ho and Lee's model to two factors. 

## A two-factor model

Suppose the forward rates evolve as 

$$
d _ {t} f (t, T) = \sigma_ {1} d W _ {1} (t) + \sigma_ {2} e ^ {- \lambda (T - t)} d W _ {2} (t) + \alpha (t, T) d t,
$$

where $\sigma_{1}$ , $\sigma_{2}$ and $\lambda$ are constants, and $\alpha$ is a deterministic function of t and T. Here the $W_{1}$ Brownian motion provides ‘shocks’ which are felt equally by points of all maturities on the yield curve, whereas $W_{2}$ gives short-term shocks which have little effect on the long-term end of the curve. This model is HJM consistent, so we can read off information about it from that structure. The HJM completeness conditions reduce, in this case, to there being two F-previsible processes $\gamma_{1}(t)$ and $\gamma_{2}(t)$ such that the drift $\alpha$ is 

$$
\alpha (t, T) = \sigma_ {1} \gamma_ {1} (t) + \sigma_ {2} e ^ {- \lambda (T - t)} \gamma_ {2} (t) + \sigma_ {1} ^ {2} (T - t) + \frac {\sigma_ {2} ^ {2}}{\lambda} \big (1 - e ^ {- \lambda (T - t)} \big) e ^ {- \lambda (T - t)}.
$$

So the range of available drifts has two degrees of functional freedom away from the martingale measure drift. Under the martingale measure (that is $\gamma_{1} = \gamma_{2} = 0$ ), the forward rate is 

$$
f (t, T) = \sigma_ {1} W _ {1} (t) + \sigma_ {2} e ^ {- \lambda T} \int_ {0} ^ {t} e ^ {\lambda s} d W _ {2} (s) + f (0, T) + \int_ {0} ^ {t} \alpha (s, T) d s.
$$

Like Ho and Lee, this model has normally distributed forward rates – which does allow them to go negative. Nevertheless the model does have the advantages of technical tractability and an explicit option formula. We can deduce from the forward rate formula that $-\log P(t,T)=\int_{t}^{T}f(t,u)du$ is 

$$
\begin{array}{r l} & {\sigma_ {1} (T - t) W _ {1} (t) + \frac {\sigma_ {2}}{\lambda} \big (e ^ {- \lambda t} - e ^ {- \lambda T} \big) \int_ {0} ^ {t} e ^ {\lambda s} d W _ {2} (s)} \\ & {\qquad + \int_ {t} ^ {T} f (0, u) d u + \int_ {0} ^ {t} \int_ {t} ^ {T} \alpha (s, u) d u d s,} \end{array}
$$

and that the instantaneous interest rate is 

$$
r _ {t} = \sigma_ {1} W _ {1} (t) + \sigma_ {2} e ^ {- \lambda t} \int_ {0} ^ {t} e ^ {\lambda s} d W _ {2} (s) + f (0, t) + \int_ {0} ^ {t} \alpha (s, t) d s.
$$

This means that the instantaneous rate is made up of a Brownian motion and an independent mean-reverting (Ornstein-Uhlenbeck) process plus drift. However in a multi-factor setting, the short rate loses its dominant role as the carrier of all information about the bond prices. 

Setting $\bar{\sigma}^2 (t,T)$ to be the variance (term variance) of $\log P(t,T)$ , we have 

$$
\bar {\sigma} ^ {2} (t, T) = \sigma_ {1} ^ {2} (T - t) ^ {2} t + \left(\frac {\sigma_ {2}}{\lambda} \bigl (1 - e ^ {- \lambda (T - t)} \bigr)\right) ^ {2} \frac {1}{2 \lambda} \bigl (1 - e ^ {- 2 \lambda t} \bigr).
$$

The discounted bond, $B_{t} = \exp(\int_{0}^{t} r_{s} ds)$ , is also log-normally distributed, because we can deduce that the integral $\int_{0}^{t} r_{s} ds$ is normal from the expression for $r_{t}$ above. We can use the results of section 6.2, given the joint log-normality of the asset and discount bond prices. The value of an option on the T-bond, struck at k, exercised at time t is 

$$
V _ {0} = P (0, t) \left(F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \bar {\sigma} ^ {2} (t , T)}{\bar {\sigma} (t , T)}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \bar {\sigma} ^ {2} (t , T)}{\bar {\sigma} (t , T)}\right)\right),
$$

where $F$ is $P(0, T) / P(0, t)$ , the forward price of the $T$ -bond. This Black-Scholes type of formula allows us to price caps and floors as well as options on the discount $T$ -bonds. However, in the multi-factor setting, the trick we used before to price options on coupon-bearing bonds does not work, making it more involved to price them and the associated swaptions. 

## The general multi-factor normal model

We can actually generalise the two-factor model above to a general multifactor one which also has normal forward rates and an explicit Black-Scholes type option pricing formula. 

We take the instance of the completely general n-factor model, where each volatility surface $\sigma_{i}(t,T)$ can be written as a product 

$$
\sigma_ {i} (t, T) = x _ {i} (t) y _ {i} (T),
$$

where $x_{i}$ and $y_{i}$ are deterministic functions. The forward rates are then driven by 

$$
d _ {t} f (t, T) = \sum_ {i = 1} ^ {n} y _ {i} (T) x _ {i} (t) d W _ {i} (t) + \alpha (t, T) d t.
$$

Here the function $x_{i}$ determines the size at time $t$ of 'type $i$ shocks', and the function $y_{i}$ controls how the shock is felt at different maturities. In the single-factor case when $n = 1$ , this framework incorporates both the Ho and Lee model $(x(t) = \sigma, y(T) = 1)$ and the Vasicek model $(x(t) = \sigma_t \exp\left(\int_0^t \alpha_s ds\right), y(T) = \exp\left(-\int_0^T \alpha_s ds\right))$ . 

For the market to be complete, we need two conditions on the functions $\alpha$ and $y_{i}$ to hold. Firstly, there should be n F-previsible processes $\gamma_{1}, \ldots, \gamma_{n}$ , such that 

$$
\alpha (t, T) = \sum_ {i = 1} ^ {n} x _ {i} (t) y _ {i} (t) \left(\gamma_ {i} (t) + x _ {i} (t) Y _ {i} (t, T)\right),
$$

where $Y_{i}(t,T)=\int_{t}^{T}y_{i}(u)du$ . In other words, the drifts consistent with hedging span an n-dimensional function space around the martingale drift. Secondly the matrix $A_{t}=(a_{ij}(t))$ , where $a_{ij}(t)=Y_{j}(t,T_{i})$ should be non-singular for all $t<T_{1}$ , for every set of n maturities $T_{1}<\ldots<T_{n}$ . This condition is really just asserting that all the functions $y_{i}$ are different. It is satisfied, for instance, if each volatility $\sigma_{i}$ has the form 

$$
\sigma_ {i} (t, T) = \sigma_ {i} (t) \exp (- \lambda_ {i} (T - t)),
$$

where the $\sigma_{i}(t)$ are deterministic functions of time and the $\lambda_{i}$ are distinct constants. 

For the general volatility surface $\sigma_{i}(t,T)=x_{i}(t)y_{i}(T)$ , the short rate and the forward rates are normally distributed. Consequently the bond 

## 5.7 Multi-factor models

prices are log-normally distributed and a Black–Scholes type formula holds (see section 6.2). Let F be the forward price of the T-bond at time t, $F = P(0, T)/P(0, t)$ , and let $\sigma$ be the term volatility of the T-bond up to time t, that is $\sigma^{2}t$ is the variance of $\log P(t, T)$ , or 

$$
\sigma^ {2} = \frac {1}{t} \sum_ {i = 1} ^ {n} Y _ {i} ^ {2} (t, T) \int_ {0} ^ {t} x _ {i} ^ {2} (s) d s.
$$

Then the value at time zero of a call on the T-bond, struck at k, exercisable at time t is 

$$
V _ {0} = P (0, t) \left(F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} t}{\sigma \sqrt {t}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} t}{\sigma \sqrt {t}}\right)\right).
$$

## Brace-Gatarek-Musiela

The Brace–Gatarek–Musiela (BGM) model is a particular case of HJM which focuses on the $\delta$ -period LIBOR rates. We shall simplify their notation slightly and write 

$$
L (t, T) = \frac {1}{\delta} \left(\frac {P (t , T)}{P (t , T + \delta)} - 1\right).
$$

So $L(t, T)$ is the $\delta$ -period (forward) LIBOR rate for borrowing at a time $T$ . 

The general HJM model (of n factors) defined by the forward volatilities $\sigma_{i}(t,T)$ is restricted in the BGM setup to those $\sigma$ such that 

$$
\int_ {T} ^ {T + \delta} \sigma_ {i} (t, u) d u = \frac {\delta L (t , T)}{1 + \delta L (t , T)} \gamma_ {i} (t, T)
$$

holds for all t less than T. Here, $\gamma$ is some deterministic $R^{n}$ -valued function which is absolutely continuous with respect to T. 

Then it follows that, under the martingale measure $\mathbb{Q}$ , $L$ obeys the SDE 

$$
d _ {t} L (t, T) = L (t, T) \sum_ {i = 1} ^ {n} \gamma_ {i} (t, T) \left(d W _ {i} (t) + \left(\int_ {t} ^ {T + \delta} \sigma_ {i} (t, u) d u\right) d t\right).
$$

More interestingly, under the forward measure $P_{T+\delta}$ (see section 6.4), L obeys 

$$
d _ {t} L (t, T) = L (t, T) \sum_ {i = 1} ^ {n} \gamma_ {i} (t, T) d \tilde {W} _ {i} (t),
$$

where $\tilde{W}_{i}$ are $P_{T+\delta}$ -Brownian motions. Thus $L(t,T)$ , as a t-process, is not only a $P_{T+\delta}$ -martingale, but is also log-normal. We shall see later that this enables us to price caps and swaptions easily. 

To price, we only need to know the function $\gamma$ , rather than the whole volatility structure. While the $\gamma$ function represents the correlation at time $t$ between changes in the LIBOR rates at different forward dates $T$ , in practice $\gamma$ is calibrated by comparing the model's prices with the market. For instance, in their paper, Brace, Gatarek and Musiela fit a $\gamma$ function of the form 

$$
\gamma_ {i} (t, T) = f (t) \gamma_ {i} (T - t)
$$

by calibrating against known prices of caps and swaptions. 

Writing $L(T)$ for $L(T, T)$ , the instantaneous LIBOR rate, suppose we have a contract which pays off at a sequence of times $T_{i} = T_{0} + i\delta$ ( $i = 1, \ldots, n$ ). If the payment at time $T_{i+1}$ depends on the LIBOR rate set at time $T_{i}$ , for example if $X = f(L(T_{i}))$ , then the value of that payment at time t is 

$$
V _ {t} = P (t, T _ {i + 1}) \mathbb {E} _ {\mathbb {P} _ {T _ {i + 1}}} \left(f (L (T _ {i})) \mid \mathcal {F} _ {t}\right).
$$

The fact that $L(T_{i})$ is log-normally distributed under $P_{T_{i+1}}$ allows us to evaluate this expression for simple f. 

One such simple f is the caplet payoff $\delta\left(L(T_{i-1})-k\right)^{+}$ at time $T_{i}$ . In this case, the worth of the caplet at time t is $V_{t}$ , equal to 

$$
\delta P (t, T _ {i}) \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \zeta^ {2} (t , T _ {i - 1})}{\zeta (t , T _ {i - 1})}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \zeta^ {2} (t , T _ {i - 1})}{\zeta (t , T _ {i - 1})}\right) \right\},
$$

where $F$ is the forward LIBOR rate $L(t, T_{i-1})$ and $\zeta^2(t, T)$ is $\int_t^T |\gamma(s, T)|^2 ds$ , the variance of $\log L(T)$ given $\mathcal{F}_t$ . This valuation has the familiar Black-Scholes form because under the forward measure $\mathbb{P}_{T_i}$ , $L(T_{i-1})$ is log-normal and the calculation proceeds as usual. 

We can even (approximately) price swaptions. Consider the option to pay fixed at rate k and receive floating and at times $T_{i} = T_{0} + i\delta$ ( $i = 1, \ldots, n$ ). Let us set 

$$
\Gamma_ {i} ^ {2} = \int_ {t} ^ {T _ {0}} | \gamma (s, T _ {i - 1}) | ^ {2} d s,
$$

which is the variance of $\log L(T_{0}, T_{i-1})$ given $F_{t}$ under the forward measure $P_{T_{i}}$ . We also define 

$$
d _ {i} = \sum_ {j = 1} ^ {i} \frac {\delta L (t , T _ {j - 1})}{1 + \delta L (t , T _ {j - 1})} \Gamma_ {j} - \frac {1}{2} \Gamma_ {i},
$$

and $s_0$ to be the unique root of the equation 

$$
s: \sum_ {i = 1} ^ {n} (k \delta + I (i = n)) \left\{\prod_ {j = 1} ^ {i} \left(1 + \delta L (t, T _ {j - 1}) \exp (\Gamma_ {j} (s + d _ {j}))\right) \right\} ^ {- 1} = 1.
$$

Then an approximation to the value at time t of the above swaption is 

$$
V _ {t} = \delta \sum_ {i = 1} ^ {n} P (t, T _ {i}) \left\{L (t, T _ {i - 1}) \Phi \left(\frac {F _ {i} + \frac {1}{2} \Gamma_ {i} ^ {2}}{\Gamma_ {i}}\right) - k \Phi \left(\frac {F _ {i} - \frac {1}{2} \Gamma_ {i} ^ {2}}{\Gamma_ {i}}\right) \right\},
$$

where $F_{i} = -\Gamma_{i}(s_{0} + d_{i})$ 

## Chapter 6 Bigger models

The Black–Scholes stock model assumes that the stock drift and stock volatility are constant. It assumes that there is only a single stock in the market. And it assumes that the cash bond is deterministic with zero volatility. None of these assumptions is necessary. The subsequent sections tackle these restrictions one by one and show how a more general model can still price and hedge derivatives. Also we will reveal the underlying framework which governs all these models from behind the scenes. 

This is not to say that all models, no matter how complex or bizarre, will always give good prices. But if a model is driven by Brownian motions, and has no transaction costs, it is analysable in this framework. 

## 6.1 General stock model

We recall that the Black–Scholes model contained a bond and a stock $B_{t}$ and $S_{t}$ with SDEs 

$$
\begin{array}{r l} & d B _ {t} = r B _ {t} d t, \\ \text {and} & d S _ {t} = S _ {t} (\sigma d W _ {t} + \mu d t). \end{array}
$$

Here r is the constant interest rate, $\sigma$ is the constant stock volatility and $\mu$ is the constant stock drift, and we are using the SDE formulation discussed in section 4.4. The process W is P-Brownian motion. 

Our most general stochastic process can have variable drift and volatility. Not only can they vary with time, but they can depend on movements of the 

## 6.1 General stock model

stock itself (or equivalently, on movements of the Brownian motion W). We could replace the constant $\sigma$ by a function of the stock price $\sigma(S_{t})$ , or even a function of both the stock price and time $\sigma(S_{t}, t)$ . Even this is not fully general. (For instance the volatility at time t might depend on the maximum value achieved by the stock price up to time t.) We will replace $\sigma$ by a general F-previsible process $\sigma_{t}$ , and the constants r and $\mu$ by F-previsible processes $r_{t}$ and $\mu_{t}$ respectively. The new SDEs are now 

$$
\begin{array}{l l} & d B _ {t} = r _ {t} B _ {t}   d t, \\ \text { and } & d S _ {t} = S _ {t} (\sigma_ {t}   d W _ {t} + \mu_ {t}   d t). \end{array}
$$

These have solutions 

$$
\begin{array}{l} B _ {t} = \exp \left(\int_ {0} ^ {t} r _ {s} d s\right), \\ S _ {t} = S _ {0} \exp \left(\int_ {0} ^ {t} \sigma_ {s} d W _ {s} + \int_ {0} ^ {t} (\mu_ {s} - \frac {1}{2} \sigma_ {s} ^ {2}) d s\right). \end{array}
$$

[Technical note: the processes $\sigma_{t}$ , $r_{t}$ and $\mu_{t}$ cannot be fully general, as they must be integrable enough for these integrals to exist. Explicitly, we need that (with P-probability one), the integrals $\int_{0}^{T}\sigma_{t}^{2}dt$ , $\int_{0}^{T}|r_{t}|dt$ , and $\int_{0}^{T}|\mu_{t}|dt$ are finite.] 

## Change of measure

As before, we aim to make the discounted stock price $Z_{t} = B_{t}^{-1} S_{t}$ into a martingale. This is achieved by adding a drift $\gamma_{t}$ to W. That is, if $\tilde{W}_{t} = W_{t} + \int_{0}^{t} \gamma_{s} ds$ is Q-Brownian motion, then $Z_{t}$ has SDE 

$$
d Z _ {t} = Z _ {t} \left(\sigma_ {t} d \tilde {W} _ {t} + \left(\mu_ {t} - r _ {t} - \sigma_ {t} \gamma_ {t}\right) d t\right).
$$

And $Z$ is a $\mathbb{Q}$ -martingale if 

$$
\gamma_ {t} = \frac {\mu_ {t} - r _ {t}}{\sigma_ {t}},
$$

as was adumbrated in the market price of risk section (4.4). Now the market price of risk depends on the time t and the sample path up to that time. It will, however, continue to be independent of the instrument considered. It should also be checked, in any actual case, that $\gamma_{t}$ satisfies the C-M-G growth condition $\mathbb{E}_{\mathbb{P}}(\exp\frac{1}{2}\int_{0}^{T}\gamma_{t}^{2}dt)<\infty$ . 

Under $\mathbb{Q}$ , $Z$ has the SDE 

$$
d Z _ {t} = \sigma_ {t} Z _ {t} d \tilde {W} _ {t},
$$

so it is at least a local martingale because it is driftless. It should also be checked that Z is a proper martingale. For instance, it is enough that $\mathbb{E}_{\mathbb{Q}}(\exp\frac{1}{2}\int_{0}^{T}\sigma_{t}^{2}dt)$ is finite. 

## Replicating strategies

If X is the derivative to be priced, with maturity at time T, then the procedure is not much different from the basic Black–Scholes technique. 

We can form a Q-martingale $E_{t}$ through the conditional expectation process of the discounted claim, $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ . Then the martingale representation theorem (section 3.5) says that the martingale $E_{t}$ is the integral 

$$
E _ {t} = E _ {0} + \int_ {0} ^ {t} \phi_ {s} d Z _ {s},
$$

for some F-previsible process $\phi_{t}$ . (Note that we need $\sigma_{t}$ never to be zero.) Let us take $\phi_{t}$ to be our stock portfolio holding at time t. Then 

$$
d E _ {t} = \phi_ {t} d Z _ {t}.
$$

Setting the bond portfolio holding $\psi_{t}$ to be $\psi_{t}=E_{t}-\phi_{t}Z_{t}$ , then the value of the portfolio at time t is 

$$
V _ {t} = \phi_ {t} S _ {t} + \psi_ {t} B _ {t} = B _ {t} E _ {t}.
$$

It also follows (as in chapter three) that $(\phi,\psi)$ is self-financing in that the changes in the value $V_{t}$ are due only to changes in the assets' prices. That is 

$$
d V _ {t} = \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t}.
$$

So $(\phi,\psi)$ is a self-financing strategy with initial value $V_{0}=\mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X)$ and terminal value $V_{T}=X$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/5838cdd9771e63d1a10e3a247a9d73560179bfc4a610597fd3e7d6bb25680c9a.jpg)


## 6.2 Log-normal models

## Derivative pricing

Arbitrage arguments convince us that the only value for the derivative at time t is 

Derivative price 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right) = \mathbb {E} _ {\mathbb {Q}} \left(\exp \left(- \int_ {t} ^ {T} r _ {s} d s\right) X \mid \mathcal {F} _ {t}\right).
$$

In other words, the value at time t is the suitably discounted expectation of the derivative conditional on the history up to time t, under the measure which makes the discounted stock process a martingale – the risk-neutral measure. 

There is no general expression which will provide a more explicit answer for the option value $V_{t}$ . To make specific calculations, one needs to know the discount rate $r_{t}$ , the volatility of the stock $\sigma_{t}$ – though not its drift – and the derivative itself. 

## Implementation

In practice, if the model is much more complex than Black–Scholes, these expectations cannot be performed analytically. (The log-normal cases of section 6.2 will be notable exceptions.) Instead numerical methods must be used. 

If we can approximate the price $V_{t}$ at time t, then an approximation for $\phi_{t}$ or “ $dV_{t}/dS_{t}$ ” is the delta hedge 

$$
\phi_ {t} \approx \frac {\Delta V _ {t}}{\Delta S _ {t}},
$$

where $\Delta$ represents the change over a small time interval $(t, t + \Delta t)$ . 

## 6.2 Log-normal models

We have already seen that the Black–Scholes formula can be true, even if we are not working with the Black–Scholes model (as in section 4.1). The common feature of models where this happens is that the asset prices are log-normally distributed under the martingale measure Q. 

In the simple Black–Scholes model, the cash bond and the stock are modelled as 

$$
B _ {t} = e ^ {r t} \quad \text { and } \quad S _ {t} = S _ {0} \exp (\sigma W _ {t} + \mu t),
$$

where $r, \sigma$ and $\mu$ are constants and $W$ is $\mathbb{P}$ -Brownian motion. The forward price to purchase $F$ at time $T$ is 

$$
F = S _ {0} e ^ {r T}.
$$

And the value at time zero of an option to buy $S_{T}$ for a strike price of k is 

$$
V _ {0} = e ^ {- r T} \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right) \right\}.
$$

## Log-normal asset prices

When prices, under the martingale measure, are log-normal, there are great advantages. This holds for the Black–Scholes model itself, for some currency and equity models, and also for simple interest rate models. 

Explicitly, suppose the stock $S_{T}$ and the cash bond $B_{T}$ are known to be jointly log-normally distributed under the martingale measure Q. Let $\sigma_{1}^{2}T$ be the variance of $\log S_{T}$ , $\sigma_{2}^{2}T$ be the variance of $\log B_{T}^{-1}$ ( $\sigma_{1}$ and $\sigma_{2}$ are term volatilities), and let $\rho$ be their correlation. Then the forward price for purchasing S at time T is 

$$
F = \frac {\mathbb {E} _ {\mathbb {Q}} (B _ {T} ^ {- 1} S _ {T})}{\mathbb {E} _ {\mathbb {Q}} (B _ {T} ^ {- 1})}, \quad \text { or   equivalently } \quad F = \exp (\rho \sigma_ {1} \sigma_ {2} T) \mathbb {E} _ {\mathbb {Q}} (S _ {T}),
$$

and the price of a call on $S_{T}$ struck at k is the generalised Black–Scholes formula 

$$
V _ {0} = \mathbb {E} _ {\mathbb {Q}} (B _ {T} ^ {- 1}) \left\{F \Phi \left(\frac {\log \frac {F}{k} + \frac {1}{2} \sigma_ {1} ^ {2} T}{\sigma_ {1} \sqrt {T}}\right) - k \Phi \left(\frac {\log \frac {F}{k} - \frac {1}{2} \sigma_ {1} ^ {2} T}{\sigma_ {1} \sqrt {T}}\right) \right\}.
$$

We can see why these formulae are true. Write $S_T$ as 

$$
S _ {T} = A \exp \left(\alpha_ {1} Z - \frac {1}{2} \alpha_ {1} ^ {2}\right), \quad \text { with } \alpha_ {1} ^ {2} = \sigma_ {1} ^ {2} T,
$$

where A is the constant $\mathbb{E}_{\mathbb{Q}}(S_{T})$ and Z is a normal $N(0,1)$ random variable under Q. The discount factor $B_{T}^{-1}$ is log-normal with log-variance $\sigma_{2}^{2}T$ and its correlation with the stock log-price is $\rho$ . Setting $B$ to be its expectation $B = \mathbb{E}_{\mathbb{Q}}(B_T^{-1})$ , we get 

$$
B _ {T} ^ {- 1} = B \exp \bigl (\alpha_ {2} (\rho Z + \bar {\rho} W) - \frac {1}{2} \alpha_ {2} ^ {2} \bigr), \quad \text { with } \alpha_ {2} ^ {2} = \sigma_ {2} ^ {2} T,
$$

where $\bar{\rho} = \sqrt{1 - \rho^2}$ and $W$ is a normal $N(0,1)$ independent of $Z$ . 

The expected discounted stock price is then 

$$
\mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} S _ {T}\right) = A B \exp \left(\frac {1}{2} \left(\alpha_ {1} + \rho \alpha_ {2}\right) ^ {2} + \frac {1}{2} \bar {\rho} ^ {2} \alpha_ {2} ^ {2} - \frac {1}{2} \alpha_ {1} ^ {2} - \frac {1}{2} \alpha_ {2} ^ {2}\right) = A B \exp \left(\rho \alpha_ {1} \alpha_ {2}\right).
$$

So the forward price for $S_T$ is thus $F = A\exp (\rho \sigma_1\sigma_2T)$ . Re-expressing $S_T$ : 

$$
S _ {T} = F \exp (\alpha_ {1} Z - \frac {1}{2} \alpha_ {1} ^ {2} - \rho \alpha_ {1} \alpha_ {2}),
$$

gives us the call value 

$$
V _ {0} = \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} (S _ {T} - k) ^ {+} \big) = B \mathbb {E} _ {\mathbb {Q}} \big (e ^ {\rho \alpha_ {2} Z - \frac {1}{2} \rho^ {2} \alpha_ {2} ^ {2}} (S _ {T} - k) ^ {+} \big),
$$

which is also equal to 

$$
B \mathbb {E} _ {\mathbb {Q}} \left(F e ^ {(\alpha_ {1} + \rho \alpha_ {2}) Z - \frac {1}{2} (\alpha_ {1} + \rho \alpha_ {2}) ^ {2}} - k e ^ {\rho \alpha_ {2} Z - \frac {1}{2} \rho^ {2} \alpha_ {2} ^ {2}}; Z \geqslant - z\right),
$$

where z is the critical value $z = (\log \frac{F}{k} - \frac{1}{2}\alpha_{1}^{2} - \rho\alpha_{1}\alpha_{2})/\alpha_{1}$ . Using the probabilistic result that $\mathbb{E}(e^{yZ - \frac{1}{2}y^{2}}; Z \geqslant -z) = \Phi(y + z)$ , for any constants y and z, the result follows. [The notation $\mathbb{E}(X; A)$ denotes the expectation of the random variable X over the event A, or equivalently is $\mathbb{E}(XI_{A})$ , where $I_{A}$ is the indicator function of the event A.] 

## 6.3 Multiple stock models

Black–Scholes assumes a single stock in the market. In many cases, this assumption does little harm. If we write an option on, say, General Motors stock, having modelled its behaviour adequately, we are unaffected by the movements of other securities. However, more complex equity products, such as quantos, depend on the behaviour of at least two separate securities. Even more so in the bond market, where a swap's current value is affected by the movements of a large number of bonds of varying maturities. 

A good model of several securities must not only describe each one individually, but also represent the interaction and dependency between them. For instance, our quanto contract of section 4.5 was related to both the sterling/dollar exchange rate and an individual UK stock. These two processes have some degree of co-dependence. In particular, large movements in one may be linked with corresponding movements in the other. Such changes would suggest that the two securities are correlated. 

Stochastic processes adapted to n-dimensional Brownian motion
A stochastic process X is a continuous process $(X_{t}: t \geqslant 0)$ such that $X_{t}$ can be written as 

$$
X _ {t} = X _ {0} + \sum_ {i = 1} ^ {n} \int_ {0} ^ {t} \sigma_ {i} (s) d W _ {s} ^ {i} + \int_ {0} ^ {t} \mu_ {s} d s,
$$

where $\sigma_{1},\ldots,\sigma_{n}$ and $\mu$ are random F-previsible processes such that the integral $\int_{0}^{t}(\sum_{i}\sigma_{i}^{2}(s)+|\mu_{s}|)ds$ is finite for all times t (with probability 1). The differential form of this equation can be written 

$$
d X _ {t} = \sum_ {i = 1} ^ {n} \sigma_ {i} (t) d W _ {t} ^ {i} + \mu_ {t} d t.
$$

Multiple stocks can be driven by multiple Brownian motions. Instead of just one P-Brownian motion, we will have, in the n-factor case, n independent Brownian motions $W_{t}^{1},\ldots,W_{t}^{n}$ . That means that each $W_{t}^{i}$ behaves as a Brownian motion, and the behaviour of any one of them is completely uninfluenced by the movements of the others. Their filtration $F_{t}$ is now the total of all the histories of the n Brownian motions. In other words, $F_{T}$ is the history of the n-dimensional vector $(W_{t}^{1},\ldots,W_{t}^{n})$ up to time T. This leads to an enhanced definition of a stochastic process (see box). 

The drift term is unchanged from the original (one-factor) definition, but there is now a volatility process $\sigma_{i}(t)$ for each factor. We must remember that in a multi-factor setting volatility is no longer a scalar, but strictly is now a vector. The total volatility of the process X is $\sqrt{\sigma_{1}^{2}(t)+\ldots+\sigma_{n}^{2}(t)}$ . In 

## 6.3 Multiple stock models

other words, the variance of $dX_{t}$ is $\sum_{i}\sigma_{i}^{2}(t)dt$ , made up of the contribution $\sigma_{i}^{2}(t)dt$ from each Brownian motion component $W^{i}$ , the variances adding because the Brownian motion components are independent. 

There is also an $n$ -factor version of Itô's formula and the product rule. 

## Itô's formula (n-factor)

If X is a stochastic process, satisfying $dX_{t} = \sum_{i} \sigma_{i}(t) dW_{t}^{i} + \mu_{t} dt$ , and f is a deterministic twice continuously differentiable function, then $Y_{t} := f(X_{t})$ is also a stochastic process with stochastic increment 

$$
d Y _ {t} = \sum_ {i = 1} ^ {n} \left(\sigma_ {i} (t) f ^ {\prime} \left(X _ {t}\right)\right) d W _ {t} ^ {i} + \left(\mu_ {t} f ^ {\prime} \left(X _ {t}\right) + \frac {1}{2} \sum_ {i = 1} ^ {n} \sigma_ {i} ^ {2} (t) f ^ {\prime \prime} \left(X _ {t}\right)\right) d t.
$$

Again this is an analogue of the one-factor Itô formula, with the replication of the volatility terms for each additional Brownian factor. 

## Product rule (n-factor)

If X is a stochastic process satisfying $dX_{t} = \sum_{i} \sigma_{i}(t) dW_{t}^{i} + \mu_{t} dt$ , and Y is a stochastic process satisfying $dY_{t} = \sum_{i} \rho_{i}(t) dW_{t}^{i} + \nu_{t} dt$ , then $X_{t}Y_{t}$ is a stochastic process satisfying 

$$
d \left(X _ {t} Y _ {t}\right) = X _ {t} d Y _ {t} + Y _ {t} d X _ {t} + \left(\sum_ {i = 1} ^ {n} \sigma_ {i} (t) \rho_ {i} (t)\right) d t.
$$

This new version unifies the two apparently different cases of the product rule we encountered in section 3.3. If $X_{t}$ and $Y_{t}$ are both adapted to the same Brownian motion $W_{t}$ , then this rule agrees with the first case. If however $X_{t}$ and $Y_{t}$ are adapted to two independent Brownian motions, say $W_{t}^{1}$ and $W_{t}^{2}$ , then $X_{t}$ will have zero volatility with respect to $W^{2}$ , that is $\sigma_{2}(t)=0$ , and similarly $Y_{t}$ will have zero volatility with respect to $W^{1}$ , $\rho_{1}(t)=0$ . Thus the term $\sum\sigma_{i}(t)\rho_{i}(t)$ in the n-factor product rule will be identically zero, agreeing with the second case in section 3.3. 

The Cameron–Martin–Girsanov theorem continues to hold where W is n-dimensional Brownian motion and the drift $\gamma$ is an n-vector process for which $\mathbb{E}_{\mathbb{P}}\exp(\frac{1}{2}\int_{0}^{T}|\gamma_{t}|^{2}dt)$ is finite. 

## Cameron-Martin-Girsanov theorem (n-factor)

Let $W = (W^{1}, \ldots, W^{n})$ be $n$ -dimensional $\mathbb{P}$ -Brownian motion. Suppose that $\gamma_{t} = (\gamma_{t}^{1}, \ldots, \gamma_{t}^{n})$ is an $\mathcal{F}$ -previsible $n$ -vector process which satisfies the growth condition $\mathbb{E}_{\mathbb{P}} \exp\left(\frac{1}{2} \int_{0}^{T} |\gamma_{t}|^{2} dt\right) < \infty$ , and we set $\tilde{W}_{t}^{i} = W_{t}^{i} + \int_{0}^{t} \gamma_{s}^{i} ds$ . Then there is a new measure $\mathbb{Q}$ , equivalent to $\mathbb{P}$ up to time $T$ , such that $\tilde{W} := (\tilde{W}^{1}, \ldots, \tilde{W}^{n})$ is $n$ -dimensional $\mathbb{Q}$ -Brownian motion up to time $T$ . 

The Radon–Nikodym derivative of Q by P is 

$$
\frac {d \mathbb {Q}}{d \mathbb {P}} = \exp \left(- \sum_ {i = 1} ^ {n} \int_ {0} ^ {T} \gamma_ {t} ^ {i} d W _ {t} ^ {i} - \frac {1}{2} \int_ {0} ^ {T} | \gamma_ {t} | ^ {2} d t\right).
$$

There is also a converse to this theorem, exactly analogous to the one-factor converse. 

Finally, we recall from section 5.5 that there is an n-factor martingale representation theorem. With W as n-dimensional Q-Brownian motion, M as an n-dimensional Q-martingale with non-singular volatility matrix, and N any other one-dimensional Q-martingale, then there is an F-previsible n-vector process $\phi_{t} = (\phi_{t}^{1}, \ldots, \phi_{t}^{n})$ such that 

$$
N _ {t} = N _ {0} + \sum_ {j = 1} ^ {n} \int_ {0} ^ {t} \phi_ {s} ^ {j} d M _ {s} ^ {j}.
$$

## The general $n$ -factor model

We will see later that it is important that we have essentially as many basic securities (excluding the cash bond) as there are Brownian factors. Generally speaking, if there are more securities than factors there might be arbitrage, and if there are fewer we will not be able to hedge. The situation is not quite as simple as that (the bond market, for instance, has an unlimited number of different maturity bonds), but we shall start with the canonical case. 

Our model then, will contain a cash bond $B_{t}$ as usual, and n different market securities $S_{t}^{1},\ldots,S_{t}^{n}$ . Their SDEs are 

$$
d B _ {t} = r _ {t} B _ {t} d t,
$$

$$
d S _ {t} ^ {i} = S _ {t} ^ {i} \left(\sum_ {j = 1} ^ {n} \sigma_ {i j} (t) d W _ {t} ^ {j} + \mu_ {t} ^ {i} d t\right), \quad i = 1, \dots , n.
$$

## 6.3 Multiple stock models

Here $r_{t}$ is the instantaneous short-rate process, $\mu_{t}^{i}$ is the drift of the $i^{th}$ security, and $(\sigma_{ij})_{j=1}^{n}$ is its volatility vector. As each security has a volatility vector, the collection of n such vectors forms a volatility matrix $\Sigma_{t} = (\sigma_{ij}(t))_{i,j=1}^{n}$ of processes. In integral form, these securities are 

$$
\begin{array}{l} B _ {t} = \exp \left(\int_ {0} ^ {t} r _ {s} d s\right), \\ S _ {t} ^ {i} = S _ {0} ^ {i} \exp \left(\sum_ {j = 1} ^ {n} \int_ {0} ^ {t} \sigma_ {i j} (s) d W _ {s} ^ {j} + \int_ {0} ^ {t} \left(\mu_ {s} ^ {i} - \frac {1}{2} \sum_ {j = 1} ^ {n} \sigma_ {i j} ^ {2} (s)\right) d s\right). \end{array}
$$

## Change of measure

We now want to find a new measure Q, under which all the discounted stock prices are Q-martingales simultaneously. 

Suppose we add a drift $\gamma_t = (\gamma_t^1, \ldots, \gamma_t^n)$ to $W_t$ , so that 

$$
\tilde {W} _ {t} ^ {i} = W _ {t} ^ {i} + \int_ {0} ^ {t} \gamma_ {s} ^ {i} d s
$$

is Q-Brownian motion, by the n-factor C-M-G theorem. Then the discounted stock price $Z_{t}^{i}=B_{t}^{-1}S_{t}^{i}$ has SDE 

$$
d Z _ {t} ^ {i} = Z _ {t} ^ {i} \left(\sum_ {j = 1} ^ {n} \sigma_ {i j} (t) d \tilde {W} _ {t} ^ {j} + \left(\mu_ {t} ^ {i} - r _ {t} - \sum_ {j = 1} ^ {n} \sigma_ {i j} (t) \gamma_ {t} ^ {j}\right) d t\right).
$$

To make the drift term vanish for each i, we must have that 

$$
\sum_ {j = 1} ^ {n} \sigma_ {i j} (t) \gamma_ {t} ^ {j} = \mu_ {t} ^ {i} - r _ {t}, \quad \text {   for   all   } t, i = 1, \dots , n.
$$

In terms of vectors and matrices, this can be re-expressed as 

$$
\Sigma_ {t} \gamma_ {t} = \mu_ {t} - r _ {t} {\bf 1},
$$

where $\Sigma_{t}$ is the matrix $(\sigma_{ij}(t))$ and 1 is the constant vector $(1,1,\ldots,1)$ . This vector equation may or may not have a solution $\gamma_{t}$ for any particular t. Whether it does or not depends on the actual values of $\Sigma_{t}, \mu_{t}$ and $r_{t}$ . If, though, the matrix $\Sigma_t$ is invertible, then a unique such $\gamma_t$ must exist and be equal to 

$$
\gamma_ {t} = \Sigma_ {t} ^ {- 1} (\mu_ {t} - r _ {t} {\bf 1}).
$$

The one-factor market price of risk formula $\gamma_{t} = \sigma_{t}^{-1}(\mu_{t} - r_{t})$ is now just a special case. This means that if $\Sigma_{t}$ is invertible for every t and $\gamma_{t}$ satisfies the C-M-G condition $\mathbb{E}_{\mathbb{P}} \exp\left(\frac{1}{2} \int_{0}^{T} |\gamma_{t}|^{2} dt\right) < \infty$ , then there is a measure Q which makes the discounted stock prices into Q-martingales. (Or at least into Q-local martingales. We also need the integral condition that for each i, $\mathbb{E}_{\mathbb{Q}}(\exp \frac{1}{2} \sum_{j}^{n} \int_{0}^{T} \sigma_{ij}^{2}(t) dt) < \infty$ , for $Z^{i}$ to be a proper Q-martingale.) 

## Replicating strategies

Let X be a derivative maturing at time T, and let $E_{t}$ be the Q-martingale $E_{t} = \mathbb{E}_{\mathbb{Q}}(B_{T}^{-1}X|\mathcal{F}_{t})$ . If the matrix $\Sigma_{t}$ is always invertible, then the n-factor martingale representation theorem gives us a volatility vector process $\phi_{t} = (\phi_{t}^{1}, \ldots, \phi_{t}^{n})$ such that 

$$
E _ {t} = E _ {0} + \sum_ {j = 1} ^ {n} \int_ {0} ^ {t} \phi_ {s} ^ {j} d Z _ {s} ^ {j}.
$$

The invertibility of $\Sigma_{t}$ is essential at this stage. Our hedging strategy will be $(\phi_{t}^{1},\ldots,\phi_{t}^{n},\psi_{t})$ where $\phi_{t}^{i}$ is the holding of security i at time t and $\psi_{t}$ is the bond holding. As usual, the bond holding $\psi$ is 

$$
\psi_ {t} = E _ {t} - \sum_ {j = 1} ^ {n} \phi_ {t} ^ {j} Z _ {t} ^ {j},
$$

so that the value of the portfolio is $V_{t} = B_{t} E_{t}$ . The portfolio is self-financing, in that 

$$
d V _ {t} = \sum_ {j = 1} ^ {n} \phi_ {t} ^ {j} d S _ {t} ^ {j} + \psi_ {t} d B _ {t}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a890db8d-75eb-4910-8c81-6aa404e14264/d9edf1fa07bb20337f214552a632c70d3aef8ce857e050e26ea3925c7a34b435.jpg)


## 6.4 Numeraires

## 6.4 Numeraires

Although the numeraire is usually chosen to be a cash bond, it needn't be. In fact, not only can the numeraire have volatility, it can be any of the tradable instruments available. We have seen in the foreign exchange context that there can be a choice of which currency's cash bond to use. But no matter which numeraire is chosen, the price of the derivative will always be the same. It is because the choice of numeraire doesn't matter, that we usually pick the stolid cash bond. 

When we proved the self-financing condition in chapter three, we assumed that the numeraire had no volatility. This is not actually necessary. But we do have to check that the self-financing equations will still work. We want to show that 

## Self-financing strategies

A portfolio strategy $(\phi_{t},\psi_{t})$ of holdings in a stock $S_{t}$ and a possibly volatile cash bond $B_{t}$ has value $V_{t}=\phi_{t}S_{t}+\psi_{t}B_{t}$ and discounted value $E_{t}=\phi_{t}Z_{t}+\psi_{t}$ , where Z is the discounted stock process $Z_{t}=B_{t}^{-1}S_{t}$ . Then the strategy is self-financing if either 

$$
d V _ {t} = \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t}, \quad \text { or   equivalently } \quad d E _ {t} = \phi_ {t} d Z _ {t}.
$$

Recall the one-factor product rule 

$$
d (X Y) _ {t} = X _ {t} d Y _ {t} + Y _ {t} d X _ {t} + \sigma_ {t} \rho_ {t} d t,
$$

where X and Y are stochastic processes with stochastic differentials 

$$
\begin{array}{l} d X _ {t} = \sigma_ {t} d W _ {t} + \mu_ {t} d t, \\ d Y _ {t} = \rho_ {t} d W _ {t} + \nu_ {t} d t. \end{array}
$$

Suppose we have a strategy $(\phi,\psi)$ , with discounted value $E_{t}$ satisfying $dE_{t}=\phi_{t}dZ_{t}$ . We want to show that $(\phi,\psi)$ is self-financing. We do this with two applications of the product rule. Firstly 

$$
d V _ {t} = d \left(B _ {t} E _ {t}\right) = B _ {t} d E _ {t} + E _ {t} d B _ {t} + \sigma_ {t} \left(\phi_ {t} \rho_ {t}\right) d t,
$$

where $\sigma_{t}$ is the volatility of $B_{t}$ and $\rho_{t}$ is the volatility of $Z_{t}$ (and hence $\phi_{t}\rho_{t}$ is the volatility of $E_{t}$ ). We can use the substitutions $dE_{t} = \phi_{t} dZ_{t}$ and $E_{t} = \phi_{t} Z_{t} + \psi_{t}$ to rearrange the above expression into 

$$
d V _ {t} = \phi_ {t} (B _ {t} d Z _ {t} + Z _ {t} d B _ {t} + \sigma_ {t} \rho_ {t} d t) + \psi_ {t} d B _ {t}.
$$

The second use of the product rule says that the term in brackets above is equal to $d(BZ)_{t} = dS_{t}$ . The resulting equation is the self-financing equation. 

This also holds for n-factor models with multiple stocks. 

## Changing numeraires

Suppose we have a number of securities including some stocks $S_{t}^{1},\ldots,S_{t}^{n}$ and two others $B_{t}$ and $C_{t}$ either of which might be a numeraire. If we choose $B_{t}$ to be our numeraire, we need to find a measure Q (equivalent to the original measure) under which 

$$
B _ {t} ^ {- 1} S _ {t} ^ {i} \quad (i = 1, \dots , n) \quad \text { and } \quad B _ {t} ^ {- 1} C _ {t}
$$

are Q-martingales. Then the value at time t of a derivative payoff X at time T is 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right).
$$

Suppose however that we choose $C_{t}$ to be our numeraire instead. Then we would have a different measure $Q^{C}$ under which 

$$
C _ {t} ^ {- 1} S _ {t} ^ {i} \quad (i = 1, \dots , n) \qquad \text { and } \qquad C _ {t} ^ {- 1} B _ {t}
$$

are $\mathbb{Q}^C$ -martingales. We can actually find out what $\mathbb{Q}^C$ is, or at least what its Radon-Nikodym derivative with respect to $\mathbb{Q}$ is. We recall Radon-Nikodym fact (ii) from section 3.4, that for any process $X_t$ , 

$$
\zeta_ {s} \mathbb {E} _ {\mathbb {Q} ^ {C}} (X _ {t} \mid \mathcal {F} _ {s}) = \mathbb {E} _ {\mathbb {Q}} (\zeta_ {t} X _ {t} \mid \mathcal {F} _ {s}),
$$

where $\zeta_{t}$ is the change of measure process $\zeta_{t}=\mathbb{E}_{\mathbb{Q}}(\frac{d\mathbb{Q}^{C}}{d\mathbb{Q}}|\mathcal{F}_{t})$ . It follows from this that if $X_{t}$ happens to be a $Q^{C}$ -martingale, then 

$$
\zeta_ {s} X _ {s} = \mathbb {E} _ {\mathbb {Q}} \left(\zeta_ {t} X _ {t} \mid \mathcal {F} _ {s}\right),
$$

and so $\zeta_t X_t$ is a $\mathbb{Q}$ -martingale. 

## 6.4 Numeraires

The canonical $Q^{C}$ -martingales (including the constant martingale with value 1) are $1, C_{t}^{-1}B_{t}, C_{t}^{-1}S_{t}^{1}, \ldots, C_{t}^{-1}S_{t}^{n}$ and similarly the Q-martingales are $B_{t}^{-1}C_{t}, 1, B_{t}^{-1}S_{t}^{1}, \ldots, B_{t}^{-1}S_{t}^{n}$ . Each corresponding pair has a common ratio of $\zeta_{t} = B_{t}^{-1}C_{t}$ . Thus the Radon–Nikodym derivative of $Q^{C}$ with respect to Q is the ratio of the numeraire C to the numeraire B, 

$$
\frac {d \mathbb {Q} ^ {C}}{d \mathbb {Q}} = \frac {C _ {T}}{B _ {T}}.
$$

The price of a payoff X maturing at T under the $Q^{C}$ measure is 

$$
V _ {t} ^ {C} = C _ {t} \mathbb {E} _ {\mathbb {Q} ^ {C}} \left(C _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right).
$$

Using again the Radon–Nikodym result that $\mathbb{E}_{\mathbb{Q}^{C}}(X|\mathcal{F}_{t})=\zeta_{t}^{-1}\mathbb{E}_{\mathbb{Q}}(\zeta_{T}X|\mathcal{F}_{t})$ , then 

$$
V _ {t} ^ {C} = \zeta_ {t} ^ {- 1} C _ {t} \mathbb {E} _ {\mathbb {Q}} \big (\zeta_ {T} C _ {T} ^ {- 1} X \mid \mathcal {F} _ {t} \big) = B _ {t} \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t} \big).
$$

This is exactly the same as the price $V_{t}$ under Q, so the two agree, just as in the foreign exchange section (4.1), where the dollar and sterling investors agreed on all derivative prices. 

## Example - forward measures in the interest-rate market

In interest-rate models, it is often popular to use a bond maturing at date T (the T-bond with price $P(t,T)$ ) as the numeraire. The martingale measure for this numeraire is called the T-forward measure $P_{T}$ and makes the forward rate $f(t,T)$ a $P_{T}$ -martingale, as well as the $\delta$ -period LIBOR rate for borrowing up till time T. 

The new numeraire is the T-bond normalised to have unit value at time zero. If we call this numeraire $C_{t}$ , then $C_{t} = P(t, T)/P(0, T)$ . The forward measure $P_{T}$ thus has Radon–Nikodym derivative with respect to Q of 

$$
\frac {d \mathbb {P} _ {T}}{d \mathbb {Q}} = \frac {C _ {T}}{B _ {T}} = \frac {1}{P (0 , T) B _ {T}}.
$$

The associated $\mathbb{Q}$ -martingale is 

$$
\zeta_ {t} = \mathbb {E} _ {\mathbb {Q}} \left(\frac {d \mathbb {P} _ {T}}{d \mathbb {Q}} \mid \mathcal {F} _ {t}\right) = \frac {C _ {t}}{B _ {t}} = \frac {P (t , T)}{P (0 , T) B _ {t}}.
$$

Now the forward price set at time t for purchasing X at date T is its current value $V_{t}$ scaled up by the return on a T-bond, namely $F_{t} =$ 

<!-- === Source: MinerU_markdown_Financial_Calculus_An_Introduction_to_Derivative_Pricing-Baxter__第三批-QuantBooks-main_201_2122707583759396875.md (Page 201) === -->

$P^{-1}(t,T)B_{t}\mathbb{E}_{\mathbb{Q}}\big(B_{T}^{-1}X\mid \mathcal{F}_{t}\big)$ . Once more, by property (ii) of the Radon-Nikodym derivative, $F_{t}$ equals 

$$
F _ {t} = \mathbb {E} _ {\mathbb {P} _ {T}} (X | \mathcal {F} _ {t}),
$$

so is itself a $P_{T}$ -martingale. Calculating the forward price for X is now only a matter of taking its expectation under the forward measure. 

From the SDE for $P(t,T)$ , we find that $\zeta_t$ satisfies 

$$
d \zeta_ {t} = \zeta_ {t} \sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) d W _ {i} (t),
$$

where W is n-dimensional Q-Brownian motion, and $\Sigma_{i}(t,T)$ is the component of the volatility of $P(t,T)$ with respect to $W_{i}(t)$ . By the converse of the C-M-G theorem, we see that 

$$
\tilde {W} _ {i} (t) = W _ {i} (t) - \int_ {0} ^ {t} \Sigma_ {i} (s, T) d s
$$

is $\mathbb{P}_T$ -Brownian motion. 

This gives an alternative expression for pricing interest-rate derivatives. If X is a payoff at date T, then its value at time t is 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \big (B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t} \big) = P (t, T) \mathbb {E} _ {\mathbb {P} _ {T}} (X | \mathcal {F} _ {t}).
$$

So the value of X at time t is just the $P_{T}$ -expectation of X up to time t (the forward price of X) discounted by the $(T\text{-bond})$ time value of money up to date T. 

Also the forward rates $f(t, T)$ are the forward rates for $r_T$ , so that $f(t, T)$ is a $\mathbb{P}_T$ -martingale with 

$$
\begin{array}{c} f (t, T) = \mathbb {E} _ {\mathbb {P} _ {T}} (r _ {T} | \mathcal {F} _ {t}), \\ \text { and } \quad d _ {t} f (t, T) = \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T)   d \tilde {W} _ {i} (t). \end{array}
$$

Another forward measure martingale is the $\delta$ -period LIBOR rate 

$$
L _ {t} = \frac {1}{\delta} \left(\frac {P (t , T - \delta)}{P (t , T)} - 1\right).
$$

See chapter five (section 5.7) for more details. 

## 6.5 Foreign currency interest-rate models

## 6.5 Foreign currency interest-rate models

We have looked at foreign exchange (section 4.1). We have looked at the interest rate market (chapter five). But we have not yet studied an interest rate market of another currency. Now we will. 

For definiteness, we will imagine ourselves to be a dollar investor operating in both the dollar and sterling interest-rate markets. Our variables will be 

Table 6.1 Notation $P(t,T)$ : the dollar zero-coupon bond market prices $f(t,T)$ : the forward rate of dollar borrowing at date $T$ (is $-\frac{\partial}{\partial T} \log P(t,T)$ ) $\sigma(t,T)$ : the volatility of $f(t,T)$ $\alpha(t,T)$ : the drift of $f(t,T)$ $r_t$ : the dollar short rate (equal to $f(t,t)$ ) $B_t$ : the dollar cash bond (equal to $\exp \int_0^t r_s ds$ ) $Q(t,T)$ : the sterling zero-coupon bond market prices $g(t,T)$ : the forward rate of sterling borrowing at date $T$ (is $-\frac{\partial}{\partial T} \log Q(t,T)$ ) $\tau(t,T)$ : the volatility of $g(t,T)$ $\beta(t,T)$ : the drift of $g(t,T)$ $u_t$ : the sterling short rate (equal to $g(t,t)$ ) $D_t$ : the sterling cash bond (equal to $\exp \int_0^t u_s ds$ ) $C_t$ : the exchange rate value in dollars of one pound $\rho_t$ : the log-volatility of the exchange rate $\lambda_t$ : the drift coefficient of the exchange rate (the drift of $dC_t/C_t$ ). 

As in the HJM model, we will work in an n-factor model driven by the independent Brownian motions $W_{t}^{1},\ldots,W_{t}^{n}$ . Of course n might be one, but it needn't be, in which case, the volatilities $\sigma,\tau$ and $\rho$ are n-vectors $\sigma_{i}(t,T)$ , $\tau_{i}(t,T)$ and $\rho_{i}(t)$ ( $i=1,\ldots,n$ ). 

What we have here are two separate interest-rate markets (the dollar denominated and the sterling denominated), plus a currency market linking them. The multi-factor model approach is needed to reflect varying degrees of correlation between various securities in the three markets. 

The differentials of these processes are 

$$
\begin{array}{c} {d _ {t} f (t, T) = \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T) d W _ {t} ^ {i} + \alpha (t, T) d t,} \\ {d _ {t} g (t, T) = \sum_ {i = 1} ^ {n} \tau_ {i} (t, T) d W _ {t} ^ {i} + \beta (t, T) d t,} \\ {d C _ {t} = C _ {t} \left(\sum_ {i = 1} ^ {n} \rho_ {i} (t) d W _ {t} ^ {i} + \lambda_ {t} d t\right).} \end{array}
$$

Apart from the dollar cash bond $B_{t}$ , the dollar tradable securities in this market consist of the dollar-bonds $P(t,T)$ ; the dollar worth of the sterling bonds $C_{t}Q(t,T)$ ; and the dollar worth of the sterling cash bond $C_{t}D_{t}$ . Let us fix T, and let the dollar discounted value of these three securities be X, Y and Z respectively, where 

$$
\begin{array}{r l} & X _ {t} = B _ {t} ^ {- 1} P (t, T), \\ & Y _ {t} = B _ {t} ^ {- 1} C _ {t} Q (t, T), \\ & Z _ {t} = B _ {t} ^ {- 1} C _ {t} D _ {t}. \end{array}
$$

It will simplify later expressions to introduce the notation $\Sigma_{i}$ , $T_{i}$ and $\tilde{T}_{i}$ , where 

$$
\begin{array}{l} \Sigma_ {i} (t, T) = - \int_ {t} ^ {T} \sigma_ {i} (t, u) d u, \\ T _ {i} (t, T) = - \int_ {t} ^ {T} \tau_ {i} (t, u) d u, \\ \tilde {T} _ {i} (t, T) = T _ {i} (t, T) + \rho_ {i} (t). \end{array}
$$

Then $\Sigma_{i}(t,T)$ is the $W^{i}$ -volatility term of $P(t,T)$ , $T_{i}(t,T)$ is the same for $Q(t,T)$ , and $\tilde{T}_{i}(t,T)$ is the same for $C_{t}Q(t,T)$ . 

Our plan, much as ever, is to follow the three steps to replication. The first thing to do is to find a change of measure under which $X_{t}$ , $Y_{t}$ and $Z_{t}$ are all martingales. 

For any previsible $n$ -vector $\gamma = (\gamma_i(t))_{i=1}^n$ , there is a new measure $\mathbb{Q}$ and a $\mathbb{Q}$ -Brownian motion $\tilde{W} = (\tilde{W}_t^1, \ldots, \tilde{W}_t^n)$ , where $\tilde{W}_t^i = W_t^i + \int_0^t \gamma_i(s) ds$ . 

Then the SDEs of X, Y and Z with respect to Q are 

$$
d X _ {t} = X _ {t} \left(\sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) d \tilde {W} _ {t} ^ {i} + \left(\int_ {t} ^ {T} (\xi (t, u) - \alpha (t, u)) d u\right) d t\right)
$$

$$
d Y _ {t} = Y _ {t} \left(\sum_ {i = 1} ^ {n} \tilde {T} _ {i} (t, T) d \tilde {W} _ {t} ^ {i} + \left(\nu_ {t} + \int_ {t} ^ {T} (\eta (t, T) - \beta (t, u)) d u\right) d t\right)
$$

$$
d Z _ {t} = Z _ {t} \Bigl (\sum_ {i = 1} ^ {n} \rho_ {i} (t) d \tilde {W} _ {t} ^ {i} + \nu_ {t} d t \Bigr),
$$

where $\xi (t,T)$ , $\eta (t,T)$ and $\nu_{t}$ are defined to be 

$$
\xi (t, T) = \sum_ {i = 1} ^ {n} \sigma_ {i} (t, u) \left(\gamma_ {i} (t) - \Sigma_ {i} (t, u)\right),
$$

$$
\eta (t, T) = \sum_ {i = 1} ^ {n} \tau_ {i} (t, u) (\gamma_ {i} (t) - \tilde {T} _ {i} (t, u)),
$$

$$
\nu_ {t} = \lambda_ {t} - r _ {t} + u _ {t} - \sum_ {i} \rho_ {i} (t) \gamma_ {i} (t).
$$

Then there will be a martingale measure only if there is some choice of $\gamma$ which makes all of X, Y and Z driftless. This happens if 

$$
\alpha (t, T) = \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T) \left(\gamma_ {i} (t) - \Sigma_ {i} (t, T)\right),
$$

$$
\beta (t, T) = \sum_ {i = 1} ^ {n} \tau_ {i} (t, T) \left(\gamma_ {i} (t) - \tilde {T} _ {i} (t, T)\right),
$$

$$
\lambda_ {t} = r _ {t} - u _ {t} + \sum_ {i = 1} ^ {n} \rho_ {i} (t) \gamma_ {i} (t).
$$

Then under this $\mathbb{Q}$ measure 

$$
d _ {t} P (t, T) = P (t, T) \left(\sum_ {i = 1} ^ {n} \Sigma_ {i} (t, T) d \tilde {W} _ {t} ^ {i} + r _ {t} d t\right),
$$

$$
d _ {t} Q (t, T) = Q (t, T) \left(\sum_ {i = 1} ^ {n} T _ {i} (t, T) d \tilde {W} _ {t} ^ {i} + \left(u _ {t} - \sum_ {i = 1} ^ {n} \rho_ {i} (t) T _ {i} (t, T)\right) d t\right),
$$

$$
d C _ {t} = C _ {t} \left(\sum_ {i = 1} ^ {n} \rho_ {i} (t) d \tilde {W} _ {t} ^ {i} + (r _ {t} - u _ {t}) d t\right).
$$

As long as this measure Q is unique, we will be able to hedge. (And uniqueness will follow if the volatility vectors of any n of the dollar tradable securities make an invertible matrix.) A derivative X paid in dollars at date T will have value at time t 

$$
V _ {t} = B _ {t} \mathbb {E} _ {\mathbb {Q}} \left(B _ {T} ^ {- 1} X \mid \mathcal {F} _ {t}\right).
$$

## The sterling investor

The sterling investor is on the other side of the mirror. He works with a different martingale measure $\mathbb{Q}^{\mathcal{L}}$ . This reflects that his numeraire is the sterling cash bond $D_{t}$ rather than the dollar cash bond. The Radon–Nikodym derivative of $\mathbb{Q}^{\mathcal{L}}$ with respect to $\mathbb{Q}$ will be the ratio of the dollar worth of the sterling bond to the dollar numeraire. (Normalising $D_{0} = 1/C_{0}$ for convenience.) That is 

$$
\mathbb {E} _ {\mathbb {Q}} \left(\frac {d \mathbb {Q} ^ {\mathcal {L}}}{d \mathbb {Q}} \mid \mathcal {F} _ {t}\right) = \frac {C _ {t} D _ {t}}{B _ {t}} = Z _ {t}.
$$

As $Z_{t}$ has the SDE $dZ_{t} = Z_{t}\sum_{i}\rho_{i}(t)d\tilde{W}_{t}^{i}$ , the difference in drifts between the $\mathbb{Q}^{\mathcal{L}}$ -Brownian motion $\tilde{W}^{\mathcal{L}}$ and the $\mathbb{Q}$ -Brownian motion $\tilde{W}$ is just $\rho$ . That is 

$$
\tilde {W} _ {i} ^ {\mathcal {L}} (t) = \tilde {W} _ {t} ^ {i} - \int_ {0} ^ {t} \rho_ {i} (s) d s.
$$

To the sterling investor, the sterling bonds have SDE 

$$
d _ {t} Q (t, T) = Q (t, T) \left(\sum_ {i = 1} ^ {n} T _ {i} (t, T) d \tilde {W} _ {i} ^ {\mathcal {L}} (t) + u _ {t} d t\right),
$$

which is exactly the form that HJM leads us to expect. 

As explained in section 6.4, the sterling investor will agree with the dollar investor on prices of future payoffs. 

## 6.6 Arbitrage-free complete models

Time and again we have seen the same basic techniques used to price and hedge derivatives. Firstly, the C-M-G theorem is used to make the discounted price processes into martingales under a new measure. Then the 

## 6.6 Arbitrage-free complete models

martingale representation theorem gives a hedge for the derivative. The repeated recurrence of this program suggests that there might be a more general result underpinning it. And there is. 

Before stating this canonical theorem, it is worth carefully laying out some concepts we have already brushed up against. 

- arbitrage-free. A market is arbitrage-free if there is no way of making riskless profits. An arbitrage opportunity would be a (self-financing) trading strategy which started with zero value and terminated at some definite date T with a positive value. A market is arbitrage-free if there are absolutely no such arbitrage opportunities. 

- complete. A market is said to be complete if any possible derivative claim can be hedged by trading with a self-financing portfolio of securities. 

- equivalent martingale measure (EMM). Suppose we have a market of securities and a numeraire cash bond under a measure $\mathbb{P}$ . An EMM is a measure $\mathbb{Q}$ equivalent to $\mathbb{P}$ , under which the bond-discounted securities are all $\mathbb{Q}$ -martingales. This is just a more precise name for what we call the martingale measure. 

Already we have examples of the binomial trees and the continuous-time Black–Scholes model. Both of these are complete markets with an EMM. We have not found an arbitrage opportunity, but neither are we sure that one might not exist. 

In both the binomial tree and Black–Scholes models we found there was one and only one EMM, and we were able to hedge claims. Even more so in the multiple stock models (section 6.3). There we could find a market price of risk $\gamma_{t}$ but it (and so Q too) was only unique if the volatility matrix $\Sigma_{t}$ was invertible. And it was exactly that invertibility which lets us hedge. 

Arbitrage-free and completeness theorem (Harrison and Pliska) Suppose we have a market of securities and a numeraire bond. Then 

(1) the market is arbitrage-free if and only if there is at least one EMM $\mathbb{Q}$ ; and 

(2) in which case, the market is complete if and only if there is exactly one such EMM Q and no other. 

This simple yet powerful theorem makes sense of our experience. 

In the HJM bond-market model, these conditions were also visible. The model demands that the forward rate drift $\alpha(t,T)$ satisfied 

$$
\alpha (t, T) = \sum_ {i = 1} ^ {n} \sigma_ {i} (t, T) (\gamma_ {i} (t) - \Sigma_ {i} (t, T)),
$$

for some previsible processes $\gamma_{i}(t)$ . This ensures that there is an EMM Q, and $\gamma$ is the market price of risk. We now see that this is to make sure that the model is arbitrage-free. 

The other key HJM condition is that the volatility matrix 

$$
\left(\Sigma_ {i} (t, T _ {j})\right) _ {i, j = 1} ^ {n}
$$

is non-singular for all sequences of dates $T_{1} < \ldots < T_{n}$ , and for all t less than $T_{1}$ , which means there is only one viable price of risk in the market. This is sufficient (but actually slightly more than necessary) for the EMM to be unique, and consequently for the market to be complete. 

It is worth getting a feel of why this theorem works. Although the technical details and exact definitions are passed over, the structure of the following can be proved rigorously. 

## Martingales mean no arbitrage

A martingale is really the essence of a lack of arbitrage. The governing rule for a Q-martingale $M_{t}$ is that 

$$
\mathbb {E} _ {\mathbb {Q}} (M _ {t} | \mathcal {F} _ {s}) = M _ {s}.
$$

In other words, its future expectation, given the history up to time s, is just its current value at time s. The martingale is not ‘expected’ to be either higher or lower than its present value. An arbitrage opportunity, on the other hand, is a one-way bet which is certain to end up higher than it started. 

Suppose we have a potential arbitrage opportunity contained in the self-financing portfolio strategy $(\phi,\psi)$ . (Assuming for simplicity a two security market of stock $S_{t}$ and bond $B_{t}$ .) Then its value at time t is 

$$
V _ {t} = \phi_ {t} S _ {t} + \psi_ {t} B _ {t},
$$

## 6.6 Arbitrage-free complete models

and it satisfies the self-financing equation 

$$
d V _ {t} = \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t}.
$$

We can calculate the discounted value of the portfolio $E_{t}=B_{t}^{-1}V_{t}$ , and then 

$$
d E _ {t} = \phi_ {t} d Z _ {t},
$$

where $Z_{t}$ is the discounted stock price $B_{t}^{-1}S_{t}$ which is a Q-martingale. 

Suppose now that the strategy does start with zero value $(V_{0}=0)$ and finishes with a non-negative payoff $(V_{T}\geqslant0)$ . Can this really be an arbitrage opportunity? Crucially, $E_{t}$ is a Q-martingale because $Z_{t}$ is. And so 

$$
\mathbb {E} _ {\mathbb {Q}} (E _ {T}) = \mathbb {E} _ {\mathbb {Q}} (E _ {T} | \mathcal {F} _ {0}) = E _ {0} = V _ {0} = 0.
$$

But $V_{T} \geqslant 0$ and (because $B_{T}^{-1} > 0$ ) so is $E_{T} \geqslant 0$ . But the Q-expectation of $E_{T}$ is zero, so the only possible value that $E_{T}$ can take is zero too. 

From which it is clear that $V_{T}$ is zero as well. Any strategy can make no more than nothing from nothing. A martingale is essentially a ‘fair game’ and any strategy which involves only playing fair games cannot guarantee a profit. 

Or in our language, if an EMM exists, there are no arbitrage opportunities. 

## Hedging means unique prices

If we can hedge, then there can only be at most one EMM. 

To see this, suppose that we could hedge, but that there are two different EMMs $\mathbb{Q}$ and $\mathbb{Q}'$ . 

For any event A in the history $F_{T}$ , the digital-like claim which pays off the cash bond value at time T if A has happened has payoff $X = B_{T}I_{A}$ . (The indicator function $I_{A}$ takes the value 1 if the event A happens, and zero otherwise.) This is a valid derivative, so it must be hedgeable. (We assumed that we could hedge all claims.) So there must be a self-financing portfolio $(\phi, \psi)$ which hedges X, with value 

$$
V _ {t} = \phi_ {t} S _ {t} + \psi_ {t} B _ {t}.
$$

As usual the discounted claim $E_{t} = B_{t}^{-1} V_{t}$ satisfies 

$$
d E _ {t} = \phi_ {t} d Z _ {t},
$$

where $Z_{t}$ is the discounted stock price $B_{t}^{-1}S_{t}$ . Now $Z_{t}$ is both a Q-martingale and a Q'-martingale as both Q and Q' are EMMs. So also must $E_{t}$ be. And from that, we see 

$$
E _ {0} = \mathbb {E} _ {\mathbb {Q}} (E _ {T}) = \mathbb {E} _ {\mathbb {Q} ^ {\prime}} (E _ {T}).
$$

But $E_{T}$ is just the indicator function of the event A, $I_{A}$ , and so $E_{0} = \mathbb{Q}(A) = \mathbb{Q}'(A)$ . The two measures Q and $Q'$ which were trying to be different actually give the same likelihood for the event A. As A was completely general, the two measures agree completely, and thus $Q = Q'$ . If any two EMMs are identical, then there can only really be one EMM. 

## Harrison and Pliska

We have only proved each result in one direction. We showed that if there was an EMM there was no arbitrage, but did not show that if there is no arbitrage then there actually is an EMM. Also we proved that hedging can only happen with a unique EMM, but not that the uniqueness of the EMM forced hedging to be possible. 

The full and rigorous proofs of all these results in the discrete-time case are in the paper ‘Martingales and stochastic integrals in the theory of continuous trading’ by Michael Harrison and Stanley Pliska, in Stochastic Processes and their Applications (see appendix 1 for more details). For the continuous case and more advanced models, there has been other work, notably by Delbaen and Schachermayer. But the increasing technicality of this should not stand in the way of an appreciation of the remarkable insight of Harrison and Pliska. 

## Appendix 1 Further reading

The longer a list of books is, the fewer will actually be referred to. The lists below have been kept short, in the hope that in this case less choice is more. 

Probability and stochastic calculus books 

- A first course in probability, Sheldon Ross, Macmillan (4th edition 1994, 420 pages) 

- Probability and random processes, Geoffrey Grimmett and David Stirzaker, Oxford University Press (2nd edition 1992, 540 pages) 

- Probability with martingales, David Williams, Cambridge University Press (1991, 250 pages) 

- Continuous martingales and Brownian motion, Daniel Revuz and Mark Yor, Springer (2nd edition 1994, 550 pages) 

- Diffusions, Markov processes, and martingales: vol. 2 Itô calculus, Chris Rogers and David Williams, Wiley (1987, 475 pages) 

These books are arranged in increasing degrees of technicality and depth (with the last two being at an equivalent level) and contain the probabilistic material used in chapters one, two and three. Ross is an introduction to the basic (static) probabilistic ideas of events, likelihood, distribution and expectation. Grimmett and Stirzaker contain that material in their first half, as well as the development of random processes including some basic material on martingales and Brownian motion. 

Probability with martingales not only lays the groundwork for integration, (conditional) expectation and measures, but also is an excellent introduc-

## Appendices

tion to martingales themselves. There is also a chapter containing a simple representation theorem and a discrete-time version of Black–Scholes. 

Both Revuz and Yor, and Rogers and Williams provide a detailed technical coverage of stochastic calculus. They both contain all our tools; stochastic differentials, Itô's formula, Cameron–Martin–Girsanov change of measure, and the representation theorem. Although dense with material, a reader with background knowledge will find them invaluable and definitive on questions of stochastic analysis. 

## Financial books

- Options, futures, and other derivative securities, John Hull, Prentice-Hall (2nd edition 1993, 490 pages) 

- Dynamic asset pricing theory, Darrell Duffie, Princeton University Press (1992, 300 pages) 

- Option pricing: mathematical models and computation, Paul Wilmott, Jeff Dewynne and Sam Howison, Oxford Financial Press (1993, 450 pages) 

Hull is a popular book with practitioners, laying out the various real-world options contracts and markets before starting his analysis. A number of models are discussed, and numerical procedures for implementation are also included. The chapter-by-chapter bibliographies are another useful feature. 

Duffie is a much more mathematically rigorous text, but still accessible. He contains sections on equilibrium pricing and optimal portfolio selection as well as a treatment of continuous-time arbitrage-free pricing along the same lines as this book. For readers with mathematical backgrounds, it is a good read. 

Oxford Financial Press's volume comes at the subject purely from a differential equation framework without using stochastic techniques. Eventually, many pricing problems become differential equation problems, but unless a reader has experience in this area, it is not necessarily the best place to start from. 

## Chapter four: pricing market securities

Some notable journal papers include: 

- The pricing of options and corporate liabilities, F Black and M Scholes, Journal of Political Economy, 81 (1973), 637–654. 

- Theory of rational option pricing, R C Merton, Bell Journal of Economics and Management Science, 4 (1973), 141–183. 

- Foreign currency option values, M B Garman and S W Kohlhagen, Journal of International Money and Finance, 2 (1983), 231–237. 

- Options markets, J C Cox and M Rubinstein, Prentice-Hall (1985, 500 pages). 

- Two into one, M Rubinstein, RISK, (May 1991), p. 49. 

The Black–Scholes paper is now of historical interest, but it is still fascinating to see how the subject began, though the paper should be read for its insights, not the technical detail. At the time they were as concerned with pricing the stock of companies with outstanding liabilities (such as corporate bonds or warrants) as they were about options and derivatives. 

Merton provides a more rigorous treatment, contemporaneously with Black–Scholes, and makes extension to dividend-paying stocks and a barrier option. Garman and Kohlhagen described foreign exchange options, whilst Cox and Rubinstein contain some exotic option formulas, amongst much else. The Rubinstein paper from RISK is concerned with quantos and cross-currency options. 

## Chapter five: interest rates

In the interest-rate setting, Heath-Jarrow-Morton is as seminal as Black-Scholes. By focusing on forward rates and especially by giving a careful stochastic treatment, they produced the most general (finite) Brownian interest-rate model possible. Other models may claim differently, but they are just HJM with different notation. The paper itself repays reading and re-reading. 

- Bond pricing and the term structure of interest rates: a new methodology for contingent claims valuation, David Heath, Robert Jarrow and Andrew Morton, Econometrica, 60 (1992), 77–105. 

In addition to the HJM paper, notable papers on the various interest-rate market models include 

- Term structure movements and pricing interest rate contingent claims, T S Y Ho and S-B Lee, Journal of Finance, 41 (1986), 1011–1029. 

- An equilibrium characterization of the term structure, O A Vasicek, Journal of Finance, 5 (1977), 177–188. 

- Pricing interest rate derivative securities, J Hull and A White, The Review of Financial Studies, 3 (1990), 573–592. 

- A theory of the term structure of interest rates, J C Cox, J E Ingersoll and S A Ross, Econometrica, 53 (1985), 385–407. 

- Bond and option pricing when short rates are lognormal, F Black and P Karasinski, Financial Analysts Journal, (July–August 1991), 52–59. 

- The market model of interest rate dynamics, A Brace, D Gatarek and M Musiela, UNSW Preprint, Department of Statistics S95-2. 

- Which model for the term-structure of interest rates should one use?, L C G Rogers, in Mathematical Finance (ed. M H A Davis, D Duffie, et al.), IMA Volume 65, Springer-Verlag, 93–116. 

The last of these is a review paper of models and their properties, whilst the others describe separately all the major models considered in the chapter. 

## Chapter six: bigger models

- Martingales and stochastic integrals in the theory of continuous trading, Michael Harrison and Stanley Pliska, Stochastic Processes and their Applications, 11 (1981), 215–260. 

- The fundamental theorem of asset pricing, F Delbaen and W Schachermayer, Mathematische Annalen, 300 (1994), 463–520. 

- The valuation of options for alternative stochastic processes, J C Cox and S A Ross, Journal of Financial Economics, 3 (1976), 145–166. 

Harrison and Pliska made the next step forward by linking, in a general framework, the absence of arbitrage to the existence of a martingale measure, and showing that the ability to hedge depended on there only being one such measure. That this idea still underpins much of financial mathematics today is a demonstration of the importance of the paper. 

Delbaen and Schachermayer go over similar ground but in a much more technical way to deal with the particular problems of continuous-time processes, including discontinuous processes. Cox and Ross cover option pricing for models more general than Black–Scholes, including those paying dividends. 

## Appendix 2 Notation

Notation can be divided naturally into three parts: lower case (generally deterministic), upper case (generally random), and Greek. 

## Lower case

<table><tr><td>a</td><td>a (real) parameter</td></tr><tr><td>c</td><td>a constant; coupon rate</td></tr><tr><td><eq>\frac{d\mathbb{Q}}{d\mathbb{P}}</eq></td><td>Radon–Nikodym derivative of <eq>\mathbb{Q}</eq> with respect to <eq>\mathbb{P}</eq></td></tr><tr><td>dt</td><td>infinitesimal time increment</td></tr><tr><td><eq>dW_{t}</eq></td><td>infinitesimal Brownian increment</td></tr><tr><td>f</td><td>a function</td></tr><tr><td><eq>f_{\mathbb{P}}(x)</eq></td><td>probability density function of the law <eq>\mathbb{P}</eq></td></tr><tr><td><eq>f(t,T)</eq></td><td>bond forward rates</td></tr><tr><td>g</td><td>a function</td></tr><tr><td><eq>g(x,t,T)</eq></td><td>the function <eq>(-\log P(t,T) \mid r_{t}=x)</eq></td></tr><tr><td>i</td><td>an integer</td></tr><tr><td>j</td><td>an integer</td></tr><tr><td>k</td><td>contract strike/exercise price; an integer; an offset</td></tr><tr><td>n</td><td>an integer</td></tr><tr><td><eq>n[t]</eq></td><td>number of dividend payments made by time t</td></tr><tr><td><eq>p,p_{j}</eq></td><td>a probability</td></tr><tr><td><eq>q,q_{j}</eq></td><td>a probability</td></tr><tr><td>r</td><td>constant interest rate</td></tr><tr><td><eq>r_{t}</eq></td><td>variable interest rate process; instantaneous rate</td></tr></table>

## Appendices

s initial stock price, alternative time variable $s_{j}$ possible value for the discrete stock process
t time
u foreign currency interest rate; real variable
x a real variable; horizontal axis variable $x_{i}(t)$ time-dependent factor of volatility surface $y_{i}(T)$ maturity-dependent factor of volatility surface 

## Upper case

A an event; a constant $A_t$ HJM volatility matrix $B_i, B_t$ bond price process $B(t, T)$ solution of a Riccati equation $C_t$ foreign exchange rate; coupon bond price; numeraire $D_i$ financing gap $D_t$ foreign currency cash bond $D(t, T)$ solution of a Riccati equation
E expectation operator $E_P$ expectation under the measure P $E_t$ discounted portfolio value process
F forward price $F_s(t, T)$ forward price at time s for $P(t, T)$ $F_Q$ quanto forward price $\mathcal{F}_i$ history of discrete stock-price process up to tick-time i $\mathcal{F}_t$ history of Brownian motion up to time t $I_A$ indicator function of the event A $I(t)$ sequence number of next coupon payment
K option strike price $L(T)$ LIBOR rate $L(t, T)$ forward LIBOR rate $M_t$ a martingale $N_t$ a martingale
N the set of non-negative integers {0, 1, 2, ...} $N(\mu, \sigma^2)$ a normal random variable with mean $\mu$ and variance $\sigma^2$ P hypothetical discrete derivative price
P a probability measure $P_T$ forward measure 

<table><tr><td><eq>\alpha</eq></td><td>a real parameter</td></tr><tr><td><eq>\alpha(t,T)</eq></td><td>forward rate drift</td></tr><tr><td><eq>\beta(t,T)</eq></td><td>a function of two variables (Vasicek model)</td></tr><tr><td><eq>\gamma_t</eq></td><td>change of measure drift; market price of risk</td></tr><tr><td><eq>\gamma_i(t,T)</eq></td><td>BGM volatility surface</td></tr><tr><td><eq>\delta</eq></td><td>dividend yield; coupon payment interval</td></tr><tr><td><eq>\delta t</eq></td><td>a small time increment</td></tr><tr><td><eq>\delta s_i, \delta n_i</eq></td><td>branch widths</td></tr></table>

## Notation

<table><tr><td>P(t,T)</td><td>bond prices</td></tr><tr><td><eq>\mathbb{Q}</eq></td><td>a probability measure</td></tr><tr><td><eq>\mathbb{R}^{n}</eq></td><td>the n-dimensional real vector space</td></tr><tr><td>R(t,T)</td><td>bond yield surface</td></tr><tr><td>Si,St</td><td>stock price process</td></tr><tr><td><eq>\tilde{S}_{t}</eq></td><td>tradable asset price</td></tr><tr><td>St1...Stn</td><td>stock price processes</td></tr><tr><td>T</td><td>maturity/exercise time of a derivative</td></tr><tr><td>Ti</td><td>coupon payment times</td></tr><tr><td>Ut</td><td>foreign currency derivative value process</td></tr><tr><td>V</td><td>derivative value</td></tr><tr><td>Vt</td><td>derivative value process</td></tr><tr><td>V(s,T)</td><td>Black-Scholes option price</td></tr><tr><td>Wn(t)</td><td>random walk</td></tr><tr><td>Wt</td><td>Brownian motion</td></tr><tr><td><eq>\tilde{W}_{t}</eq></td><td>Brownian motion</td></tr><tr><td>Wt1,...,Wtn</td><td>independent Brownian motions</td></tr><tr><td>X</td><td>random variable; claim value of a derivative</td></tr><tr><td>Xi</td><td>sequence of random variables</td></tr><tr><td>Xt</td><td>a stochastic process</td></tr><tr><td>Yt</td><td>a stochastic process</td></tr><tr><td>Yi(t,T)</td><td>integral of yi over [t,T]</td></tr><tr><td>Z</td><td>a (normal) random variable</td></tr><tr><td>Zi,Zt</td><td>discounted stock-price process</td></tr><tr><td>Z(t,T)</td><td>discounted bond prices</td></tr><tr><td><eq>\tilde{Z}_{t}</eq></td><td>discounted tradable asset price</td></tr></table>

## Greek case

## Appendices

$\Delta S_{i}, \Delta V_{i}$ change in value across $\delta t$ of $S_{i}, V_{i}$ , etc $\zeta_{t}$ change of measure process $\theta$ a real variable $\theta_{t}$ deterministic drift function $\lambda$ a real parameter $\mu$ constant stock drift $\mu_{t}$ variable stock drift process $\nu_{t}$ stock drift process $\pi_{i}$ path probability $\Pi_{i}$ portfolio $\rho$ correlation $\bar{\rho}$ the orthogonal complement $\sqrt{1 - \rho^{2}}$ $\rho_{t}$ volatility process $\sigma$ constant stock volatility $\sigma_{1}, \sigma_{2}$ stock volatilities $\sigma_{t}$ variable stock volatility process $\sigma(t, T)$ forward rate volatility surface $\sigma_{i}(t, T)$ multi-factor forward rate volatility surface $\bar{\sigma}$ term volatility $\Sigma_{t}$ volatility matrix $\Sigma(t, T)$ bond price volatilities $\tau$ time horizon; maturity date; stopping time $\phi_{t}, \tilde{\phi}_{t}$ stock-holding strategy; representation theorem integrand $\Phi$ normal distribution function: $\Phi(x) = \mathbb{P}(N(0,1) \leqslant x)$ $\psi_{t}$ bond-holding trading strategy $\omega$ a sample path 

## Appendix 3 Answers to exercises

2.1 The value (at maturity) of the futures contract is the stock price less the exercise price. If the process moved to node 2, the stock price is $s_2$ , so the future's value is $f(2) = s_2 - k$ . The other node is similar. 

Then, recalling that $q$ is $(s_1 \exp(r \delta t) - s_2) / (s_3 - s_2)$ , 

$$
\begin{array}{l} V = \exp (- r \delta t) \big ((1 - q) (s _ {2} - k) + q (s _ {3} - k) \big) \\ = \exp (- r \delta t) \left(s _ {2} \frac {s _ {3} - s _ {1} e ^ {r \delta t}}{s _ {3} - s _ {2}} + s _ {3} \frac {s _ {1} e ^ {r \delta t} - s _ {2}}{s _ {3} - s _ {2}} - k\right). \end{array}
$$

This is equal to $e^{-r\delta t}(s_{1}e^{r\delta t}-k)$ , which can be simplified to give $V=s_{1}-ke^{-r\delta t}$ . The only strike price which gives zero present value to the future is $k=s_{1}\exp(r\delta t)$ . 


Table A.1 Option and portfolio development – in the money


<table><tr><td>Time i</td><td>Last Jump</td><td>Stock Price <eq>S_i</eq></td><td>Option Value <eq>V_i</eq></td><td>Stock Holding <eq>\phi_i</eq></td><td>Bond Holding <eq>\psi_i</eq></td></tr><tr><td>0</td><td>-</td><td>100</td><td>50</td><td>-</td><td>-</td></tr><tr><td>1</td><td>up</td><td>120</td><td>75</td><td>1.25</td><td>-75</td></tr><tr><td>2</td><td>up</td><td>140</td><td>100</td><td>1.25</td><td>-75</td></tr><tr><td>3</td><td>down</td><td>120</td><td>100</td><td>0.00</td><td>100</td></tr></table>

2.2 The progression, in the first scenario, of the stock price and hedging strategy is laid out in table A.1, and the option claim tree is shown in figure A.1. The corresponding table in the other case is table A.2. The price of the option at time 0 is 50. We can represent the hedging strategy $\phi$ with a tree up to time 2, each of whose nodes give the amount of stock which should be held from that time for the next period. The tree is given in figure A.2. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/010dbbc1-3ff0-413f-8785-575032e04439/d62edd94d94bd09c7d5c7a20fc0062c7f3262e4dd6381dd503a77fc49d79f219.jpg)



Figure A.1 The option claim tree for a digital payoff


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/010dbbc1-3ff0-413f-8785-575032e04439/0e258772a3d8e7d0b5a1d9b0c4f8cc7a33167f249749dffefef18a95903c8bbd.jpg)



Figure A.2 The hedging strategy tree



Table A.2 Option and portfolio development – out of the money


<table><tr><td>Time i</td><td>Last Jump</td><td>Stock Price <eq>S_i</eq></td><td>Option Value <eq>V_i</eq></td><td>Stock Holding <eq>\phi_i</eq></td><td>Bond Holding <eq>\psi_i</eq></td></tr><tr><td>0</td><td>-</td><td>100</td><td>50</td><td>-</td><td>-</td></tr><tr><td>1</td><td>down</td><td>80</td><td>25</td><td>1.25</td><td>-75</td></tr><tr><td>2</td><td>up</td><td>100</td><td>50</td><td>1.25</td><td>-75</td></tr><tr><td>3</td><td>down</td><td>80</td><td>0</td><td>2.50</td><td>-200</td></tr></table>

2.3 Table A.3 has the calculations which show that $E_{\mathbb{Q}}(S_{2}|\mathcal{F}_{i})$ is identical to $S_{i}$ . That $S_{i}$ is a Q-martingale is now immediate from the remarks following the tower law. 


Table A.3 Conditional expectation against filtration value


<table><tr><td>Expectation</td><td>Filtration</td><td>Value</td></tr><tr><td><eq>\mathbb{E}_{\mathbb{Q}}(S_2|\mathcal{F}_0)</eq></td><td><eq>\{1\}</eq></td><td><eq>\frac{1}{3} \cdot \frac{2}{5} \cdot 180 + \frac{1}{3} \cdot \frac{3}{5} \cdot 80 + \frac{2}{3} \cdot \frac{2}{3} \cdot 72 \dots + \frac{2}{3} \cdot \frac{1}{3} \cdot 36 = 80</eq></td></tr><tr><td rowspan="2"><eq>\mathbb{E}_{\mathbb{Q}}(S_2|\mathcal{F}_1)</eq></td><td><eq>\{1,3\}</eq></td><td><eq>\frac{2}{5} \cdot 180 + \frac{3}{5} \cdot 80 = 120</eq></td></tr><tr><td><eq>\{1,2\}</eq></td><td><eq>\frac{2}{3} \cdot 72 + \frac{1}{3} \cdot 36 = 60</eq></td></tr><tr><td rowspan="4"><eq>\mathbb{E}_{\mathbb{Q}}(S_2|\mathcal{F}_2)</eq></td><td><eq>\{1,3,7\}</eq></td><td>180</td></tr><tr><td><eq>\{1,3,6\}</eq></td><td>80</td></tr><tr><td><eq>\{1,2,5\}</eq></td><td>72</td></tr><tr><td><eq>\{1,2,4\}</eq></td><td>36</td></tr></table>

3.1 No. The increments are wrong (or equivalently the conditional distributions are wrong). The increment $X_{s+t} - X_s$ is a normal with variance $t - 2s(\sqrt{1 + t/s} - 1)$ , which is not t, and the increment is not independent of $X_s$ . 

3.2 Yes. The increment $X_{s+t}-X_{s}$ is the sum of a normal $N(0,t\rho^{2})$ and an independent normal $N\big(0,t(1-\rho^{2})\big)$ , which is equal to a normal $N(0,t)$ in total. The increment is certainly independent of both histories $(W_{u}:u\leqslant s)$ and $(\tilde{W}_{u}:u\leqslant s)$ , and hence also independent of the history $(X_{u}:u\leqslant s)$ . 

3.3 As $S_{T}$ is distributed as a normal random variable with mean $\mu T$ and variance $\sigma^{2}T$ , the probability that this is negative is the same as the probability that a normal $N(0,1)$ random variable is less than $-\mu\sqrt{T}/\sigma$ . This probability is positive. 

3.4 $dX_{t} = \exp (W_{t})dW_{t} + \frac{1}{2}\exp (W_{t})dt = X_{t}dW_{t} + \frac{1}{2} X_{t}dt.$ 

3.5 $X_{t} = X_{0}\exp (\sigma W_{t} + \int_{0}^{t}\mu_{s}ds - \frac{1}{2}\sigma^{2}t).$ 

3.6 We know that the processes can be written as $dB_{t} = \beta_{t}dt$ and $dX_{t} =$ 

## Appendices

$\sigma_t dW_t + \mu_t dt$ . Then 

$$
d (B _ {t} X _ {t}) = \frac {1}{2} d ((B _ {t} + X _ {t}) ^ {2} - B _ {t} ^ {2} - X _ {t} ^ {2}),
$$

which by Itô is equal to 

$$
(B _ {t} + X _ {t}) (d B _ {t} + d X _ {t}) + \frac {1}{2} \sigma_ {t} ^ {2} d t - B _ {t} d B _ {t} - X _ {t} d X _ {t} - \frac {1}{2} \sigma_ {t} ^ {2} d t.
$$

This itself simplifies to the desired answer. Alternatively, an application of the product rules gives an immediate solution. 

3.7 The formula will hold (by definition) for t = 2. At time t = 1, if the first jump was ‘up’, then $\frac{dQ}{dP}$ will be $q_{1}q_{2}/p_{1}p_{2}$ with P-probability $p_{2}$ , and $q_{1}\tilde{q}_{2}/p_{1}\tilde{p}_{2}$ with P-probability $\bar{p}_{2}$ . The (conditional) expectation is then $q_{1}q_{2}/p_{1} + q_{1}\bar{q}_{2}/p_{1} = q_{1}/p_{1}$ . This is exactly what $\zeta_{1}$ is, if the first jump were up. The case where the first jump is down is similar. 

At time $t = 0$ , $\mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}}|\mathcal{F}_0) = \mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}}) = \mathbb{E}_{\mathbb{Q}}(1) = 1$ . This matches $\zeta_0$ , as we desired. 

3.8 We have to prove the result for all $s$ and $t$ , such that $s \leqslant t$ , and for all possible $X_{t}$ . We note firstly that the $s = 0$ case follows immediately from the fact that $\mathbb{E}_{\mathbb{Q}}(X) = \mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}} X)$ , and that $\zeta_t$ is $\frac{d\mathbb{Q}}{d\mathbb{P}}$ at time $t$ . The $s = t$ case is also trivial, as both sides of the result are simply $X_{t}$ . So in fact, we need only check the case $s = 1, t = 2$ , for four cases of $X_{2}$ . Take the case where $X_{2}$ is the digital claim which only pays off 1 if the process goes up twice. If the first jump was down, then both sides of the result are zero, because $X_{2}$ and $\zeta_2X_2$ must both be zero. If the first jump was up, then the left-hand side is 

$$
\mathbb {E} _ {\mathbb {Q}} (X _ {2} | \mathcal {F} _ {1}) = q _ {2} (1) + \bar {q} _ {2} (0) = q _ {2}.
$$

The right-hand side is 

$$
\zeta_ {1} ^ {- 1} \mathbb {E} _ {\mathbb {P}} (\zeta_ {2} X _ {2} | \mathcal {F} _ {1}) = \frac {p _ {1}}{q _ {1}} \left(p _ {2} \left(\frac {q _ {1} q _ {2}}{p _ {1} p _ {2}} 1\right) + \bar {p} _ {2} (0)\right) = q _ {2}.
$$

Similarly, we can check the digital claims where $X_{2}$ pays off only after an up-down, a down-up, and a down-down. This completes the verification. 

3.9 The equivalence of (ii) and (ii)' is immediate from the boxed theorem about identifying normals. So too is the equivalence of (iii) and (iii)', as long as we note that the right-hand side of (iii)' is independent of the history $\mathcal{F}_s$ . 

We can also note that (ii)' is just a special case of (iii)' when $s = 0$ . So it is enough just to prove (iii)'. The left-hand side is 

$$
\begin{array}{r l} & {\mathbb {E} _ {\mathbb {Q}} \big (\exp \big (\theta (W _ {t + s} - W _ {s} + \gamma t) \big) \big | \mathcal {F} _ {s} \big)} \\ & {\qquad = \zeta_ {s} ^ {- 1} \mathbb {E} _ {\mathbb {P}} \big (\zeta_ {t + s} \exp \big (\theta (W _ {t + s} - W _ {s} + \gamma t) \big) \big | \mathcal {F} _ {s} \big).} \end{array}
$$

Here, $\zeta_t = \mathbb{E}_{\mathbb{P}}(\frac{d\mathbb{Q}}{d\mathbb{P}}|\mathcal{F}_t)$ . By property (iii) of the $\mathbb{P}$ -Brownian motion $W$ , $\frac{d\mathbb{Q}}{d\mathbb{P}} = \exp(-\gamma W_t - \frac{1}{2}\gamma^2 T) \exp(-\gamma(W_T - W_t))$ , where $W_T - W_t$ is a normal $N(0, T - t)$ independent of $\mathcal{F}_t$ , from which it follows that $\zeta_t = \exp(-\gamma W_t - \frac{1}{2}\gamma^2 T) \exp(\frac{1}{2}\gamma^2(T - t))$ , which is just 

$$
\zeta_ {t} = \exp (- \gamma W _ {t} - \frac {1}{2} \gamma^ {2} t).
$$

Thus the left-hand side of (iii)' becomes 

$$
\exp (\theta \gamma t - \frac {1}{2} \gamma^ {2} t) \mathbb {E} _ {\mathbb {P}} \left(\exp ((\theta - \gamma) (W _ {t + s} - W _ {s})) \mid \mathcal {F} _ {s}\right).
$$

Again using the fact that $W_{t+s}-W_{s}$ is a normal $N(0,t)$ independent of $F_{s}$ , the expectation part of the above is $\exp(\frac{1}{2}(\theta-\gamma)^{2}t)$ , which means that the whole expression actually is $\exp(\frac{1}{2}\theta^{2}t)$ , as desired. 

3.10 If $\gamma = 0$ , then $X_{t} = W_{t}$ , which we know is a martingale by example (2). If, however, $\gamma$ is not zero, then 

$$
\mathbb {E} (X _ {t} | \mathcal {F} _ {s}) = \mathbb {E} (W _ {t} | \mathcal {F} _ {s}) + \gamma t = W _ {s} + \gamma t = X _ {s} + \gamma (t - s).
$$

If $\gamma$ is not zero, then $X$ is not a martingale, because of the extra term $\gamma(t - s)$ above. 

3.11 The function $\sigma$ is bounded, in that there is a constant $K$ such that $|\sigma(t,\omega)| \leqslant K$ , for all $t \leqslant T$ , and for all $\omega$ in $\Omega$ . Then $\exp\left(\frac{1}{2} \int_0^T \sigma_s^2 ds\right)$ is bounded above by $\exp\left(\frac{1}{2} K^2 T\right)$ for all $\omega$ , so its expectation is also bounded by that constant. By the second collector's guide box, the local martingale $X$ must also be a martingale. 

## Appendices

3.12 To differentiate $V_{t} = W_{t}^{2} - t$ , we can treat the two terms $W_{t}^{2}$ and $-t$ separately. The first of these can be handled by applying Itô's formula to the case $f(x) = x^{2}$ , with $X_{t} = W_{t}$ . Then 

$$
d \big (f (W _ {t}) \big) = f ^ {\prime} (W _ {t}) d W _ {t} + \frac {1}{2} f ^ {\prime \prime} (W _ {t}) d t = 2 W _ {t} d W _ {t} + d t.
$$

Also $d(-t) = -dt$ , so we can deduce that $dV_{t} = 2W_{t}dW_{t}$ . In fact, $V_{t}$ is a proper martingale, because if we let $X$ be $(\int_0^T W_t^2 dt)^{\frac{1}{2}}$ , then it is enough to show (collector's guide) that $\mathbb{E}(X) < \infty$ . In fact 

$$
\left(\mathbb {E} (X)\right) ^ {2} \leqslant \mathbb {E} \bigl (X ^ {2} \bigr) = \int_ {0} ^ {T} \mathbb {E} \bigl (W _ {t} ^ {2} \bigr) d t = \frac {1}{2} T ^ {2}.
$$

3.13 If we let $L_{t}$ be the logarithm of $Z_{t}$ , then $L_{t} = \sigma W_{t} + (\mu - r)t$ , and so $dL_{t} = \sigma dW_{t} + (\mu - r)dt$ . The expression then follows from Itô. 

3.14 If we change variables in the integral to $v = -(x + \frac{1}{2}\sigma^2 T) / \sigma \sqrt{T}$ , then $V_0$ is 

$$
V _ {0} = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {a} \left(s e ^ {- \sigma \sqrt {T} v - \frac {1}{2} \sigma^ {2} T} - k e ^ {- r T}\right) e ^ {- \frac {1}{2} v ^ {2}} d v,
$$

where a is the constant $\left(\log\frac{s}{k}+(r-\frac{1}{2}\sigma^{2})T\right)/\sigma\sqrt{T}$ . By writing $\exp(-\sigma\sqrt{T}v-\frac{1}{2}\sigma^{2}T-\frac{1}{2}v^{2})$ as $\exp\left(-\frac{1}{2}(v+\sigma\sqrt{T})^{2}\right)$ , we can rewrite the integral as 

$$
V _ {0} = \frac {s}{\sqrt {2 \pi}} \int_ {- \infty} ^ {a + \sigma \sqrt {T}} e ^ {- \frac {1}{2} v ^ {2}} d v - \frac {k e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {a} e ^ {- \frac {1}{2} v ^ {2}} d v.
$$

This can then be evaluated as 

$$
V _ {0} = s \Phi (a + \sigma \sqrt {T}) - k e ^ {- r T} \Phi (a),
$$

which is the expression we sought. 

3.15 We needed to know that the drift was constant. So far, we can only cancel constant drifts with our three-step plan. Later (section 6.1) we will generalise this, but for the moment we need the drift to be constant, even if we are indifferent to which constant it is. 

3.16 Simply evaluate the Black-Scholes formula with $s = \$10$ , $k = \$12$ , $\mu = 0.15$ , $\sigma = 0.20$ , $r = 0.05$ and $T = 1$ . The option value is \$0.325. 

3.17 In this case X is $1 if $S_T > \$10$ , and is zero otherwise, where T is 1. Hence by the derivative pricing formula 

$$
V _ {0} = \mathbb {E} _ {\mathbb {Q}} (B _ {T} ^ {- 1} X) = e ^ {- r T} \mathbb {Q} (S _ {T} > 1 0) = e ^ {- r T} \Phi \left(\frac {r T - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}\right).
$$

This has the numerical value of $0.532. 

4.1 (i) Discounted, the asset is $Z_{t} = B_{t}^{-1}X_{t} = \exp \big(2\sigma \tilde{W}_{t} + (r - \sigma^{2})t\big)$ . Its SDE is $dZ_{t} = Z_{t}(2\sigma d\tilde{W}_{t} + (r + \sigma^{2})dt)$ , which has a non-vanishing drift term. So $Z_{t}$ is not a Q-martingale, and thus $X_{t}$ is not a tradable asset. (ii) In this case, the discounted asset is $Z_{t} = B_{t}^{-1}X_{t} = \exp \big(-\alpha \sigma \tilde{W}_{t} - \alpha rt\big)$ . Given that, $\alpha r = \frac{1}{2} (\alpha \sigma)^{2}$ , the SDE of $Z_{t}$ is $dZ_{t} = Z_{t}(-\alpha \sigma d\tilde{W}_{t})$ , which is a Q-martingale. So $X_{t}$ is tradable. 

4.2 Replace each $dW_{i}(t)$ by $d\tilde{W}_{i}(t)-\gamma_{i}(t)$ and substitute into the SDEs for $dY_{t}$ and $dZ_{t}$ and see that the drift terms vanish. 

4.3 The only difference between this example and the sterling case in the text is that the exchange rate is the other way round. Before we had the sterling/dollar rate (the worth of the local currency in domestic terms), and here we have the dollar/yen rate (the worth of the domestic currency in local terms). We should really be working with $C_{t}^{-1}$ instead of $C_{t}$ , but the only difference is that the sign of the correlation changes. Thus the forward price is $F_{0} = \exp(\rho\sigma_{1}\sigma_{2})F$ , and not $\exp(-\rho\sigma_{1}\sigma_{2})F$ , where F is the local currency forward $F = e^{uT}S_{0}$ . As exchange rates tend to quote the ‘big’ number, the sign of $\rho$ needed in any particular instance depends on the actual pair of currencies in question. 

## Appendix 4 Glossary of technical terms

Adapted a process which depends only on the current position and past movements of the driving processes. It is unable to see into the future 

American call option a call option which can be exercised at any time up to the option expiry date 

Arbitrage the making of a guaranteed risk-free profit with a trade or series of trades in the market 

Arbitrage free a market which has no opportunities for risk-free profit 

Arbitrage price the only price for a security that allows no arbitrage opportunity 

Autoregressive of a process, that it is mean-reverting 

Average the arithmetic mean of a sample 

Bank account process an account which is continuously compounded at the prevailing instantaneous rate, and behaves like the cash bond 

Binomial process a process on a binomial tree 

Binomial representation theorem a discrete-time version of the martingale representation theorem on the binomial tree 

Binomial tree a tree, each of whose nodes branches into two at the next stage 

Black-Scholes a stock market model with an analytic option pricing formula 

<table><tr><td>Bonds</td><td>interest bearing securities which can either make regular interest payments and/or a lump sum payment at maturity</td></tr><tr><td>Bond options</td><td>an option to buy or sell a bond at a future date</td></tr><tr><td>Brownian motion</td><td>the basic stochastic process formed by taking the limit of finer and finer random walks. It is a martingale, with zero drift and unit volatility, and is not Newtonian differentiable</td></tr><tr><td>Calculus</td><td>generally a formal system of calculation, in particular concerned with analysing behaviour in terms of infinitesimal changes of the variables.Newtonian calculus handles smooth functions, but not Brownian motion which requires the techniques of stochastic calculus.[From calculus (Lat.), a pebble used in an abacus]</td></tr><tr><td>Call option</td><td>the option to buy a security at/by a future date for a price specified now</td></tr><tr><td>Cameron-Martin-Girsanov theorem</td><td>a result which interprets equivalent change of measure as changing the drift of a Brownian motion</td></tr><tr><td>Cap</td><td>a contract which periodically pays the difference between current interest rate returns and a rate specified at the start, only if this difference is positive. A cap can be used to protect a borrower against floating interest rates being too high</td></tr><tr><td>Caplet</td><td>an individual cap payment at some instant</td></tr><tr><td>Cash bond</td><td>a liquid continuously compounded bond which appreciates at the instantaneous interest rate</td></tr><tr><td>Central limit theorem</td><td>a statistical result, which says that the average of a sample of IID random variables is asymptotically normally distributed</td></tr><tr><td>Change of measure</td><td>viewing the same stochastic process under a different set of likelihoods, changing the probabilities of various events occurring</td></tr><tr><td>Claim</td><td>a payment which will be made in the future according to a contract</td></tr><tr><td>Commodity</td><td>a real thing, such as gold, oil or frozen concentrated orange juice</td></tr><tr><td>Complete market</td><td>a market in which every claim is hedgable</td></tr></table>

## Appendices

<table><tr><td>Conditional distribution</td><td>the distribution of a random variable conditional on some information <eq>\mathcal{F}</eq>, such as <eq>\mathbb{P}(X \leqslant x|\mathcal{F})</eq></td></tr><tr><td>Conditional expectation</td><td>taking an expectation given some history as known. For instance the conditional expectation of the number of heads obtained in three tosses, given that the first toss was heads, is two; whereas the unconditioned expectation is only one and a half. Written <eq>\mathbb{E}(\cdot|\mathcal{F}_t)</eq>, for conditioning on the history of the process up to time <eq>t</eq></td></tr><tr><td>Contingent claim</td><td>a claim whose amount is determined by the behaviour of market securities up until the time it is paid</td></tr><tr><td>Continuous</td><td>a process or function which only changes by a small amount when its variable or parameter is altered infinitesimally</td></tr><tr><td>Continuous-time</td><td>a process which depends on a real-valued time parameter, allowing infinite divisibility of time</td></tr><tr><td>Continuously compounded</td><td>interest is compounded instantly, rather than annually or monthly, leading to exponential growth</td></tr><tr><td>Contract</td><td>an agreement under law between two principals, or counterparties</td></tr><tr><td>Correlation</td><td>a measure of the linear dependence of two random variables. If one variable gets larger as the other does, the correlation is positive, and negative if one gets larger as the other gets smaller. The limits of one and minus one correspond to exact dependence, whereas independent variables have zero correlation. Formally correlation is the covariance of the random variables divided by the square root of the product of their individual variances</td></tr><tr><td>Coupon</td><td>a periodic payment made by a bond</td></tr><tr><td>Covariance</td><td>a measure of the relationship of two random variables, the covariance is zero if the variables are independent (and vice versa in the case of jointly normal random variables). Formally the covariance of two variables is the expectation of their product less the product of their expectations</td></tr><tr><td>Cumulative normal integral</td><td>see normal distribution functionGlossary of technical terms</td></tr><tr><td>Currency</td><td>the monetary unit of a country or group of countries</td></tr><tr><td>Default free</td><td>there being no chance that the bond issuer will be unable to meet his financial undertakings (used theoretically)</td></tr><tr><td>Density</td><td>the probability density function <eq>f</eq> is the derivative (if it exists) of the distribution function of a continuous random variable. Intuitively, <eq>f(x) \, dx</eq> is the probability that <eq>X</eq> lies in the interval <eq>[x, x + dx]</eq>. The function <eq>f</eq> is non-negative, integrates to one, and can be used to calculate expectations, and so forth, as<eq>\mathbb{E}(X^2) = \int_{-\infty}^{\infty} x^2 f(x) \, dx</eq></td></tr><tr><td>Derivative</td><td>a security whose value is dependent on (derived from) existing underlying market securities. See also contingent claim</td></tr><tr><td>Difference equation</td><td>the discrete analogue of a differential equation. For example, to find the sequence <eq>(x_n)</eq> which obeys<eq>ax_{n+2} + bx_{n+1} + cx_n = d</eq></td></tr><tr><td>Diffusion</td><td>a stochastic process which is the solution to a SDE</td></tr><tr><td>Digital</td><td>a derivative which pays off a fixed amount if a given future event happens, and nothing otherwise</td></tr><tr><td>Discount</td><td>scaling a future reward or cost down to reflect the importance of now over later</td></tr><tr><td>Discount bond</td><td>a bond which promises to make a lump sum payment at a future date, but until then is worth less than its face value</td></tr><tr><td>Discrete</td><td>taking distinct, separated values; such as from the sets N or <eq>\{0, \delta t, 2\delta t, \ldots\}</eq></td></tr><tr><td>Distribution</td><td>of a random variable, the description of the likelihood of its every possible value</td></tr><tr><td>Distribution function</td><td>the (cumulative) distribution function <eq>F</eq> of a random variable is defined so that <eq>F(x)</eq> is the probability that the random variable is no larger than <eq>x</eq>. The</td></tr></table>

## Appendices

<table><tr><td>Distribution function (contd)</td><td>function F increases (weakly) from 0 to 1. If F is differentiable, then its derivative is the density</td></tr><tr><td>Dividends</td><td>regular but variable payments made by an equity</td></tr><tr><td>Doléans exponential</td><td>for a local martingale Mt, this is the solution of the SDE dXt = Xt dMt, which is another local martingale Xt = exp(Mt - 1/2 ∫0t(dMs)2)</td></tr><tr><td>Drift</td><td>the coefficient of the dt term of a stochastic process</td></tr><tr><td>Driftless</td><td>a process with constant zero drift</td></tr><tr><td>Equilibrium distribution</td><td>a distribution of a process which is stable under time evolution</td></tr><tr><td>Equities</td><td>stocks which make dividend payments</td></tr><tr><td>Equivalent martingale measure (EMM)</td><td>see martingale measure</td></tr><tr><td>Equivalent measures</td><td>two measures P and Q are equivalent if they agree on which events have zero probability</td></tr><tr><td>European call option</td><td>a call option which can be exercised or not only at the option exercise date. Compare with American call option</td></tr><tr><td>Exercise date</td><td>a set future date at which an option may be exercised or not</td></tr><tr><td>Exercise price</td><td>see strike price</td></tr><tr><td>Exotics</td><td>new derivative securities, which will quickly either become standard products or will sink without trace</td></tr><tr><td>Expectation</td><td>the mean of a random variable, which will be the limiting value of the average of an infinite number of identical trials. For a discrete and a continuous random variable (with density f) it is respectively</td></tr><tr><td></td><td>E(X) = ∑n∞n n P(X = n), E(X) = ∫∞-∞xf(x) dx</td></tr><tr><td>Exponential Brownian motion</td><td>a process which is the exponential of a drifting Brownian motion</td></tr><tr><td>Exponential martingales</td><td>the Doléans exponential of a martingale, which itself is a (local) martingale</td></tr><tr><td>Filtration</td><td>the history, <eq>(\mathcal{F}_t)_{t \geq 0}</eq>, of a process, where <eq>\mathcal{F}_t</eq> is the information about the path of the process up to time t</td></tr><tr><td>Fixed</td><td>of interest rates, that they are constant throughout the term of the contract</td></tr><tr><td>Floating</td><td>of interest rates, that they can move with the market over the term of the contract</td></tr><tr><td>Floor</td><td>a contract which periodically pays the difference between a rate specified at the start and current interest rate returns, only if this difference is positive. A floor can be used to protect a lender against floating interest rates being too low. See also cap</td></tr><tr><td>Floorlet</td><td>which is to floors as caplets are to caps</td></tr><tr><td>Foreign exchange</td><td>the market which prices one currency in terms of another</td></tr><tr><td>Forward</td><td>an agreement to buy or sell something at a future date for a set price, called the forward price</td></tr><tr><td>Forward rate</td><td>the forward price of instantaneous borrowing</td></tr><tr><td>Fractal</td><td>a geometrical shape which on a small-scale looks the same as the large-scale, only smaller. A straight line is a fractal of dimension one, and a Brownian motion path is a fractal of dimension 1.5</td></tr><tr><td>Future</td><td>a forward traded on an exchange</td></tr><tr><td>FX</td><td>abbreviation for foreign exchange</td></tr><tr><td>Gaussian process</td><td>a process, all of whose marginals are normally distributed, and all of whose joint distributions are jointly normal</td></tr><tr><td>Heath-Jarrow-Morton (HJM)</td><td>a model of the interest-rate market</td></tr><tr><td>Hedge</td><td>to protect a position against the risk of market movements</td></tr><tr><td>History</td><td>the information recording the path of a process</td></tr><tr><td>Identically distributed</td><td>of random variables, have the same probabilistic distribution</td></tr><tr><td>IID</td><td>abbreviation for Independent, Identically Distributed</td></tr></table>

## Appendices

<table><tr><td>Independent</td><td>of variables, none of which have any relation or influence on any of the others</td></tr><tr><td>Indicator function</td><td>a function of a set which is one when the argument lies in the set and zero when it is outside</td></tr><tr><td>Induction</td><td>a method of proof, involving the demonstration that the current case follows from the previous case, which itself then implies the next case, and so on</td></tr><tr><td>Instantaneous rate</td><td>the rate of interest paid on a very very short term loan</td></tr><tr><td>Instruments</td><td>tradable securities or contracts</td></tr><tr><td>Interest rate</td><td>the rate at which interest is paid</td></tr><tr><td>Interest rate market</td><td>the market which determines the time value of money</td></tr><tr><td>Itô's formula</td><td>a stochastic version of the ‘chain rule’ which expresses the volatility and drift of the function of a stochastic process in terms of the volatility and drift of the process itself and the derivatives of the function. If <eq>X_t</eq> has volatility <eq>\sigma_t</eq> and drift <eq>\mu_t</eq>, then <eq>Y_t = f(X_t)</eq> has volatility <eq>f'(X_t)\sigma_t</eq> and drift <eq>f'(X_t)\mu_t + \frac{1}{2}f''(t)\sigma_t^2</eq></td></tr><tr><td>Kolmogorov's strong law</td><td>see strong law</td></tr><tr><td>Law of the unconscious statistician</td><td>the result that if a random variable X has density f, then the expectation of h(X) is<eq>\mathbb{E}(h(X)) = \int_{-\infty}^{\infty} h(x)f(x) dx</eq></td></tr><tr><td>LIBOR</td><td>the London Inter-Bank Offer Rate. A daily set of interest rates for various currencies and maturities</td></tr><tr><td>Local martingale</td><td>a stochastic process which is driftless, but not necessarily a martingale</td></tr><tr><td>Log-drift</td><td>of a stochastic process <eq>X_t</eq>, the drift of log <eq>X_t</eq></td></tr><tr><td>Log-normal distribution</td><td>a random variable whose logarithm is normally distributed</td></tr><tr><td>Log-volatility</td><td>of <eq>X_t</eq> is the volatility of log <eq>X_t</eq>, or equivalently the volatility of <eq>dX_t/X_t</eq></td></tr><tr><td>Long</td><td>(of position) having a positive holding</td></tr><tr><td>Marginal</td><td>the marginal distribution of a process X at time t is the distribution of <eq>X_t</eq> considered as a random variable in isolation. Two processes may be different, yet have exactly the same marginal distributions</td></tr><tr><td>Market</td><td>a place for the exchanging of price information. Commonly situated in electronic space</td></tr><tr><td>Market maker</td><td>(in UK) a dealer who is obligated to quote and trade at two-way prices</td></tr><tr><td>Market price of risk</td><td>a standardised reward from risky investments in terms of extra growth rate</td></tr><tr><td>Markov</td><td>of a process, meaning that its future behaviour is independent of its past, conditional on the present</td></tr><tr><td>Martingale</td><td>a process whose expected future value, conditional on the past, is its current value. That is, <eq>\mathbb{E}(M_t|\mathcal{F}_s)</eq> equals <eq>M_s</eq> for every s less than t</td></tr><tr><td>Martingale measure</td><td>a measure under which a process is a martingale</td></tr><tr><td>Martingale representation theorem</td><td>a result which allows one martingale to be written as the integral of a previsible process with respect to another martingale</td></tr><tr><td>Maturity</td><td>the time at which a bond will repay its principal, or more generally the time at which any claim pays off</td></tr><tr><td>Mean</td><td>synonym for expectation</td></tr><tr><td>Mean reversion</td><td>the property of a process which ensures that it keeps returning to its long-term average</td></tr><tr><td>Measure</td><td>a collection of probabilities on the set of all possible outcomes, describing how likely each one is</td></tr><tr><td>Multi-factor</td><td>a market model which is driven by more than one Brownian motion</td></tr><tr><td>Newtonian calculus</td><td>classical differential and integral calculus, relating to smooth or differentiable functions</td></tr><tr><td>Newtonian function</td><td>a function which is smooth enough to have a classical (Newtonian) derivative</td></tr><tr><td>Node</td><td>a point on a tree where branches start and finish</td></tr><tr><td>Noise</td><td>a loose term for volatility</td></tr></table>

## Appendices

<table><tr><td>Normal distribution</td><td>a continuous distribution, parameterised by a mean <eq>\mu</eq> and variance <eq>\sigma^{2}</eq>, written <eq>N(\mu,\sigma^{2})</eq> with density</td></tr><tr><td></td><td><eq>f(x)=\frac{1}{\sqrt{2\pi\sigma^{2}}}\exp\left(-\frac{(x-\mu)^{2}}{2\sigma^{2}}\right)</eq></td></tr><tr><td>Normal distribution function</td><td>the distribution function of the normal random variable, written <eq>\Phi(x)=\mathbb{P}(N(0,1)\leqslant x)</eq></td></tr><tr><td>Numeraire</td><td>a basic security relative to which the value of other securities can be judged. Often the cash bond</td></tr><tr><td>ODE</td><td>abbreviation for Ordinary Differential Equation</td></tr><tr><td>Option</td><td>a contract which gives the right but not the obligation to do something at a future date</td></tr><tr><td>Ornstein-Uhlenbeck (O-U) process</td><td>a mean reverting stochastic process with SDE</td></tr><tr><td></td><td><eq>dX_{t}=\sigma dW_{t}+(\theta-\alpha X_{t})dt</eq></td></tr><tr><td>Over-the-counter</td><td>an agreement concluded directly between two parties, without the mediation of an exchange</td></tr><tr><td>Path probability</td><td>the probability of a tree process taking a particular path through the tree. The probability will be the product of the probabilities of the individual branches taken</td></tr><tr><td>Payoff</td><td>a payment</td></tr><tr><td>PDE</td><td>abbreviation for Partial Differential Equation</td></tr><tr><td>Poisson process</td><td>a type of random process with discontinuities</td></tr><tr><td>Portfolio</td><td>a collection of security holdings</td></tr><tr><td>Position</td><td>the amount of a security held, which can either be positive (a long position) or negative (a short position)</td></tr><tr><td>Previsible</td><td>a stochastic process which is adapted and is either continuous or left-continuous with right-limits or is a limit of such processes</td></tr><tr><td>Principal</td><td>the face value that a bond will pay back at maturity</td></tr><tr><td>Probability</td><td>the chance of an event occurring</td></tr><tr><td>Process</td><td>a sequence of random variables, parameterised by time</td></tr><tr><td>Product rule</td><td>a result giving the stochastic differential of the product of two stochastic processes</td></tr><tr><td>Put-call parity</td><td>the observation that the worth of a call less the price of a put struck at the same price is the current worth of a forward</td></tr><tr><td>Quantos</td><td>cross-currency contracts, derivatives which pay off in another currency</td></tr><tr><td>Radon-Nikodym derivative</td><td>of one measure with respect to another is the relative likelihood of each sample path under one measure compared with the other</td></tr><tr><td>Random variable</td><td>a function of a sample space</td></tr><tr><td>Random walk</td><td>a discrete Markov process made up of the sum of a number of independent steps. A simple symmetric random walk is N-valued and after each time step goes up one with probability <eq>\frac{1}{2}</eq> and down one with probability <eq>\frac{1}{2}</eq></td></tr><tr><td>Recombinant tree</td><td>a tree where branches can come together again</td></tr><tr><td>Replicating strategy</td><td>a self-financing portfolio trading strategy which hedges a claim precisely</td></tr><tr><td>Risk free</td><td>no chance of anything going wrong</td></tr><tr><td>Risk-neutral measure</td><td>a martingale measure</td></tr><tr><td>SDE</td><td>abbreviation for Stochastic Differential Equation</td></tr><tr><td>Security</td><td>a piece of paper representing a promise</td></tr><tr><td>Self-financing</td><td>a strategy which never needs to be topped up with extra cash nor can ever afford withdrawals</td></tr><tr><td>Semimartingale</td><td>a process which can be decomposed into a local martingale term and a drift term of finite variation</td></tr><tr><td>Share</td><td>(in UK) a stock or equity</td></tr><tr><td>Short</td><td>(of position) having a negative, or borrowed, holding</td></tr><tr><td>Short rate</td><td>see instantaneous rate</td></tr><tr><td>Single-factor</td><td>a market model which is driven by only one Brownian motion</td></tr></table>

## Appendices

<table><tr><td>Standard deviation</td><td>the square root of the variance</td></tr><tr><td>Stochastic</td><td>synonym for random</td></tr><tr><td>Stochastic calculus</td><td>a calculus for random processes, such as those involving Brownian motion terms</td></tr><tr><td>Stochastic process</td><td>a continuous process, which can be decomposed into a Brownian motion term and a drift term</td></tr><tr><td>Stock</td><td>a security representing partial ownership of a company</td></tr><tr><td>Stock market</td><td>a place for trading stocks</td></tr><tr><td>Strike price</td><td>the price at which an asset may be bought or sold under an option</td></tr><tr><td>Strong law</td><td>the result that the average of a sample of n IID random variables will converge to the mean of the distribution as n increases, given some technical conditions</td></tr><tr><td>Swaps</td><td>an agreement to make a series of fixed payments over time and receive a corresponding series of payments dependent on current interest rates, or vice versa</td></tr><tr><td>Swaption</td><td>an option to enter into a swap agreement at a future date</td></tr><tr><td>Taylor expansion</td><td>for Newtonian functions, the expression of the value of a function f near x in terms of the value of it and its derivatives at x, that is <eq>f(x+h) = f(x) + hf'(x) + \frac{1}{2}h^2f''(x) + \frac{1}{6}h^3f'''(x) \ldots</eq></td></tr><tr><td>Term structure</td><td>the relationship between the interest rates demanded on loans, and the length of the loans</td></tr><tr><td>Term variance</td><td>the variance of the logarithm of a security price over a time period, Var(<eq>\log(S_T/S_0)</eq>)</td></tr><tr><td>Term volatility</td><td>the effective (annualised) volatility of an asset over a time period. Explicitly, its square is the term variance divided by the length of the term:<eq>\bar{\sigma}^2 = \text{Var}(\log(S_T/S_0))/T</eq></td></tr><tr><td>Time value of money</td><td>the difference between cash now, and cash later which is subject to a discount</td></tr><tr><td>Tower law</td><td>the result that <eq>\mathbb{E}(\mathbb{E}(X|\mathcal{F}_t) \mid \mathcal{F}_s) = \mathbb{E}(X|\mathcal{F}_s)</eq>, for s &lt; t</td></tr><tr><td>Tradable</td><td>of an asset, that it can be traded either directly, or indirectly by trading a matching portfolio</td></tr><tr><td>Trading strategy</td><td>a continuous choice of portfolio, a choice which may depend on market movements</td></tr><tr><td>Transaction cost</td><td>a charge for buying or selling a security</td></tr><tr><td>Tree</td><td>a graph of nodes linked by branches which contains no closed loops or circuits</td></tr><tr><td>Underlying</td><td>a basic market security, such as stocks, bonds and currencies</td></tr><tr><td>Vanilla</td><td>of a product, the standard basic version</td></tr><tr><td>Variable coupon</td><td>periodic payments from a floating interest-rate contract</td></tr><tr><td>Variance</td><td>a measure of the uncertainty of a random variable. Formally, the expectation of its square less the square of its expectation, or equivalently the expected square of the difference between the random variable and its mean</td></tr><tr><td>Volatility</td><td>the amount of ‘noise’ or variability of a process, more precisely, the coefficient of the Brownian motion term of a stochastic process</td></tr><tr><td>Weak law</td><td>the result that the average of n IID random variables is increasingly less likely to be significantly different from the distribution mean as n increases</td></tr><tr><td>Wiener process</td><td>synonym for Brownian motion</td></tr><tr><td>With probability 1</td><td>of an event, having probability one of occurring. This is not quite the same as being guaranteed for sure, as, for example, a normal random variable can take the value zero, but with probability one it will not</td></tr><tr><td>Yield</td><td>the average interest rate offered by a bond</td></tr><tr><td>Yield curve</td><td>the graph of yield plotted against bond maturity</td></tr><tr><td>Zero coupon</td><td>a bond which does not make any payments until maturity</td></tr></table>

## Index

adapted processes, 55, 62
American options, 93
arbitrage, 8, 39, 41
    arbitrage price, 8, 86, 139
    arbitrage-free, 197
arbitrage pricing, 7–9
arbitrage-free complete models,
    196–200
autoregressive process, 156
Bachelier, 45
bank account process, see cash bond
binomial
    branch, 11
    branch model, 10–17
    distribution, 42
    process, 46
    tree, 19
    tree model, 17–28
binomial representation theorem,
    28–41, 77
Black–Derman–Toy model, 157
Black–Karasinski model, 157
Black–Scholes, 83–98
    currency model, 100 

formula, 43, 91, 182
hedge, 96
model, 83, 178
summary, 90
bond only strategy, 12
bond options, 169
bond prices, 144
bonds, 112–115
with coupons, 114, 165
Brace–Gatarek–Musiela model, 175
branch, 10
binomial branch process, 11
Brown, Robert, 46
Brownian motion, 44–46, 48, 49, 54
as stock model, 50
exponential with drift, 51
two-dimensional, 62
with drift, 50
calculus
Itô, 57–62
Newtonian, 52
stochastic, 51–57
call option, 9, 43, 90
American, 93 

European, 90
foreign exchange, 103
on bonds, 169
on coupon bonds, 115, 170
on dividend paying stocks, 109
on swaps, see swaptions
quanto, 123

Cameron–Martin–Girsanov theorem, 74, 75
n-factor, 159, 186, 187
and market price of risk, 120
converse, 74, 105, 192
use in foreign exchange, 102
use in HJM models, 138, 145
use in stock models, 83, 84, 179
caplet, 171, 176
caps, 170
cash bond, 11, 18, 37, 136, 144
foreign currency, 100
central limit theorem, 42, 47, 48
change of measure, 62–76, 145, 179, 187
claim, 3, 20, 30
coin-tossing game, 4, 5
collector's guide to
exponential martingales, 79
martingales, 79
commodity, 3
complete market, 197
completeness, 196–200
conditional expectation, 32
conditional marginal distribution, 48, 69
construction strategies, 79–83
contingent claim, see claim
continuous compounding, 5
continuous processes, 44–51 

correlation, 123, 126, 158, 176, 182, 193
coupon bonds, 114, 165
options on, 115, 170
coupons
fixed rate, 165
floating rate, 166
covariance, 124, 158
Cox–Ingersoll–Ross model, 156
cross-currency contracts, see quantos
cumulative normal integral, see normal distribution function
currency, see foreign exchange
default free, 129
delta hedge, 181
density, 7
derivative, 3, 12
derivative pricing, 181, 188
difference equation, 40, 80
diffusion, 61, 150
digital contract, 27, 123
discount bond, 112, 129
discount process, 37, 87
discounted
bond, 138, 145
claim, 38, 87, 90
expectation, 20, 28
stock, 38, 87, 90, 179
discrete model
conclusions, 41
continuous overture, 41–43
distribution function
normal, 43, 91
dividends, 106–112
continuous, 107
periodic, 111
dollar investor, 101 

Doléans exponential, 61
Doob-Meyer decomposition, 56
double fork, 20
drift, 52, 55, 83
HJM, 143, 158
HJM constraints on, 141, 148
uniqueness, 56
driftlessness, 78
equilibrium distribution, 154
equities, 106–112
guaranteed profits example, 110
equivalent martingale measure, 197–200
also, see martingale measure
equivalent measures, 66, 74
European call option, 90
examples
pricing on tree, 23
exercise date, 91
exercise price, see strike price
existence of martingale measure, 40
exotic contracts, 128, 163
expectation, 4, 9, 23
discounted claim, 40
for a branch, 12
on a tree, 21
operator, 31
pricing, 3–7, 16, 86
re-emergence, 23
regained, 16
vs arbitrage, 9
exponential Brownian motion, 60,
84, 85
with drift, 51
exponential martingale, 79, 85
filtration, 30, 48 

fixed rate, 165, 167, 168
floating rate, 166, 167
floorlet, 171
floors, 170
foreign exchange, 99–106, 122
interest rate models, 192–196
forward, 6, 11, 17
foreign exchange, 99, 103
interest rate, 133, 163
quanto, 123
use in option formula, 169, 182
forward measure, 165, 191
forward rate, 134–136, 142
bond price formula, 144
curve, 134
drift, 143, 158
under forward measure, 192
volatility, 143, 158
forward swaps, 168
fractal, 49
Fubini, 143
Gaussian process, 50
Harrison and Pliska, 197, 200
Heath–Jarrow–Morton, see HJM
hedge, 94, 145, 180, 188
Black–Scholes, 96
hedging strategy, see replicating strategy
history, 20, 30
HJM, 142, 158
conditions, 143, 148, 159
equivalence to short-rate, 150
multi-factor, 158–163
single-factor, 142–149
universality, 149 

Ho and Lee model, 151, 169, 172, 174 

Hull and White model, see Vasicek 

IID variables, 47, 58 

illustrated definitions, 29 

independence, 4, 21, 46, 48 

indicator function, 199 

induction, 19, 22
backwards, 19
inductive step, 22, 36
result, 22 

instantaneous rate, 132, 135, 136,
144
Markovian, 150 

instruments, 3, 11, 83, 100, 128 

interest rate, 18
foreign exchange model, 193
market, 128–135
multi-factor models, 172–177
products, 163–172
riskless, 83
short-rate models, 149–158
simple model, 135–142 

Itô calculus, 57–62 

Itô's formula, 59, 61, 81, 83
n-factor, 185 

Jamshidian, 170 

joint likelihood function, 70 

Kolmogorov's law of large numbers, see strong law 

law of the unconscious statistician, 7 

LIBOR rate, 166, 168, 170, 175–176 under forward measure, 191 

local martingales, 79 

log-drift, 60 log-normal
call formula, 103
distribution, 6
models, 181–183 

log-volatility, 60 

long position, 96, 168, 172 

marginal distribution, 48
conditional, 48, 69 

market maker, 14 

market price of risk, 115–122
definition, 119
in general models, 179, 188
in HJM models, 141, 145, 147 

Markov process, 144, 150 

martingale, 33, 76  
exponential, 79 

martingale measure, 34, 44, 76, 197
continuous model, 85, 87
discrete model, 34–39
existence and uniqueness, 40 

Martingale representation theorem, 78 

martingale representation theorem,
76–79, 94
n-factor, 161, 186, 188
and dividend payments, 108, 112
and tradable assets, 116
use in foreign exchange, 102
use in HJM, 139, 146
use in stock models, 83–85, 88,
180 

maturity, 129 

mean, see expectation 

mean reversion, 155 

measure, 30, 63 

multi-factor models, 172
HJM, 158 

normal models, 174 

multiple payment contracts, 164 

Newtonian calculus, 52 

Newtonian differentials, 51
uniqueness, 53 

Newtonian function, 52 

node, 10 

noise, 41, 50 

non-tradable quantity, 116–118, 120 

normal distribution function, 43, 91
identification, 72 

numeraires, 143, 188–192
changing, 190
with volatility, 189 

option, 9, 43, 90, 94 

ordinary differential equation, 53 

Ornstein-Uhlenbeck process, 173 

over-the-counter, 163 

partial differential equation, 95 

path probabilities, 21 

payoff, 4, 15, 103, 147 

Pliska, 197, 200 

Poisson process, 55 

portfolio, 80 

position, 96 

previsible process, 32, 56, 78, 80 

price is right, the, 14 

principal, 165–167 

probability, 4 

probability density function, 7 

process, 29
stochastic, 55 

product rule, 62, 138, 189  
n-factor, 185 

pull to par, 114 

put option, 91 

put-call parity, 91, 171 

quantos, 122–127, 183 

Radon–Nikodym derivative, 63–68,
73
changing numeraire, 105, 190–
192, 196
continuous time, 69, 71 

random variable, 7, 12, 32, 65 

random walk, 46 

recombinant tree, 23 

replicating strategy, 8, 12, 40
continuous model, 82, 86, 180
discrete model, 13, 22–23
foreign exchange, 102
HJM model, 137, 146, 164 

Riccati differential equation, 156 

risk-free construction, see replicating strategy 

risk-neutral measure, 120
also, see martingale measure 

SDE, 56 

self-financing, 39–40, 80, 180
equation, 81, 89, 162, 189
in HJM model, 139, 147 

semimartingale, 55, 56 

share, 3 

short position, 80, 82 

short rate, see instantaneous rate 

single-factor models
HJM, 142
short-rate models, 149 

standard deviation, 6 

sterling investor, 104 

stochastic n-factor process, 184 

## Index

calculus, 51–57
differential equation, 56
differentials, 54
process, 55
stock, 10, 17
stock model
n-factor model, 186
general model, 178–181
multiple stocks, 183–188
stocks and bonds together, 13
stocks not coins, 6
stopping time, 93
strike price, 9, 91, 96
strong law, 4, 5, 13, 15
misleading nature, 6–9, 16, 23, 30
weak law and, 59
swaps, 167, 171
forward, 168
options on, 171, 176
swaptions, 171, 176
Taylor expansion, 58
term structure, 131
term variance, 173
term volatility, 169, 175, 182
terminal value pricing, 95
three steps to replication, 84
discounted case, 90
foreign exchange, 101
interest rates, 137
time value of money, 5, 129
tower law, 34, 77, 166
tradable asset, 101, 116–118
trading strategy, 40, 81
transaction cost, 17, 83
tree, 17, 19
binomial, 17
complexity of, 19 

financial applications, 36
pricing conclusions, 27
recombinant, 23
strategy construction, 38
two-step, 20, 63
two-dimensional Brownian motion, 62
two-factor model, 172
two-step tree, 20, 63
underlying asset, 3
uniqueness of
martingale measure, 40
Newtonian differentials, 53
volatility and drift, 56
vanilla, 73, 99
variable coupon, 166, 168
variance, 42, 47, 58
Vasicek model, 153, 169, 174
view, admiring the, 98
volatility, 55, 83
HJM, 143, 158
term volatility, 169
uniqueness, 56
weak law, 59
whole story in one step, 15
Wiener process, 50
X-ray vision, 37
yield, 130, 135
yield curve, 131
inverted, 132, 133
zero coupon bond, 135
zoo of the new, 3 