

<!-- === Source: MinerU_markdown_An_Introduction_to_the_Financial_Derivatives_1_2122707919320489996.md (Page 1) === -->

This chapter first deals with the two basic building blocks of financial derivatives: options and forwards (futures). Next, we introduce the more complicated class of derivatives known as swaps. The chapter concludes by showing that a complicated swap can be decomposed into a number of forwards and options. This decomposition is very practical. If one succeeds in pricing forwards and options, one can then reconstitute any swap and obtain its price. This chapter also introduces some formal notation that will be used throughout the book. 

Such an introduction requires a discussion of the logic behind asset pricing. In addition, at various points we provide examples that also require an understanding of formal asset pricing methods. All these necessitate a brief discussion of the securities under consideration. This introductory chapter has that aim. Readers can consult other books to obtain more background on derivatives. Hull (2000) is an excellent source for derivatives. Jarrow and Turnbull (1996) gives another approach. The more advanced books by Ingersoll (1987) and Duffie (1996) provide strong links to the underlying theory. The manual by Das (1994) provides a summary of the practical issues associated with derivative contracts. A comprehensive new source is Wilmott (1998). 

This book is an introduction to quantitative tools used in pricing financial derivatives. Hence, it is mainly about mathematics. It is a simple and heuristic introduction to mathematical concepts that have practical use in financial markets. 

## 1 Introduction

## Financial Derivatives

A Brief Introduction 

$^{2}$ There is a significant amount of trading on “notional” French government bonds in Paris. 

In these markets, one can borrow at risk-free rates (by collateralizing the underlying physical asset), buy and store the product, and insure it until the expiration date of any derivative contract. One can therefore easily build an alternative to holding a forward or futures contract on these commodities. For example, one can borrow at risk-free rates, buy a T-bond, and hold it until the delivery date of a futures contract on T-bonds. This is equivalent 

Some derivative instruments are written on products of cash-and-carry markets. Gold, silver, currencies, and T-bonds are some examples of cash-and-carry products. 

3.1 Cash-and-Carry Markets 

There is another method of classifying the underlying asset, which is important for our purposes. 

These underlying commodities are not financial assets. They are goods in kind. Hence, in most cases, they can be physically purchased and stored. 

4. Indexes: The S&P-500 and the FT-SE100 are two examples of stock indexes. The CRB commodity index is an index of commodity prices. Again, these are not “assets” themselves. But derivative contracts can be written on notional amounts and a position taken with respect to the direction of the underlying index. 

In this category, we can also include derivatives on bonds, notes, and T-bills, which are government debt instruments. They are promises by governments to make certain payments on set dates. By dealing with derivatives on bonds, notes and T-bills, one takes positions on the direction of various interest rates. In most cases, these derivative instruments are not notionals and can result in actual delivery of the underlying asset. 

3. Interest rates: In fact, interest rates are not assets. Hence, a notional asset needs to be devised so that one can take a position on the direction of future interest rates. Futures on Eurodollars is one example. 

sector for goods and services.
2. Currencies: These are liabilities of governments or, sometimes, banks.
They are not direct claims on real assets. 

Forwards and options are considered basic building blocks. Swaps and some other complicated structures are considered hybrid securities, which can eventually be decomposed into sets of basic forwards and options. We let $S_t$ denote the price of the relevant cash instrument, which we call 

3 Types of Derivatives 

Note in their valuation.
In the rest of this book, the symbols $F(t)$ and $F(S_{t}, t)$ will be used alter-
nately to denote the price of a derivative product written on the underlying
asset $S_{t}$ at time t. The financial derivative is sometimes assumed to yield
a payout $d_{t}$ . At other times, the payout is zero. T will always denote the
expiration date. 

Hence, at the time of the expiration of the derivative contract, denoted by $T$ , the price $F(T)$ of a derivative asset is completely determined by $S_T$ , the value of the "underlying asset." After that date, the security ceases to exist. This simple characteristic of derivative assets plays a very important role in their valuation. 

DEFINITION: A financial contract is a derivative security, or a contingent claim, if its value at expiration date T is determined exactly by the market price of the underlying cash instrument at time T (Ingersoll, 1987). 

In the words of practitioners, "Derivative securities are financial contracts that 'derive' their value from cash market instruments such as stocks, bonds, currencies and commodities."1 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/9edee3780367889e52961a0fe68bb2efb3bfe45c13d3fab85363aae1a5479940.jpg)


The payoff diagram for a simplified long position is shown in Figure 1. The contract is purchased for $F(t)$ at time $t$ . It is assumed that the contract expires at time $t + 1$ . The upward-sloping line indicates the profit or loss of the purchaser at expiration. The slope of the line is one. 

The expiration date of the contract and the forward price are written when the contract is entered into. If a forward purchase is made, the holder of such a contract is said to be long in the underlying asset. If at expiration the cash price is higher than the forward price, the long position makes a profit; otherwise there is a loss. 

DEFINITION: A forward contract is an obligation to buy (sell) an underlying asset at a specified forward price on a known date. 

Futures and forwards are linear instruments. This section will discuss forwards; their differences from futures will be briefly indicated at the end. 

4 Forwards and Futures 

contract. They both represent the same thing at time $T$ . So, in the case of gold futures, we can indeed say that the equality in (1) holds at expiration. At $t < T$ , $F(t)$ may not equal $S_t$ . Yet we can determine a function that ties $S_t$ to $F(t)$ . 

4 Forwards and Futures 

$^{3}$ However, as in the case of crude oil, the storage process may end up being very costly. Environmental and other effects make it very expensive to store crude oil. 

cash equivalent.
For example, the (exchange-traded) futures contract promising the delivery of 100 troy ounces of gold cannot have a value different from the actual market value of 100 troy ounces of gold on the expiration date of the 

$F(T) = S_T;$ 

The relationship between $F(t)$ , the price of the derivative, and $S_v$ , the value of the underlying asset, is known exactly (or deterministically), only at the expiration date $T$ . In the case of forwards or futures, we naturally expect 

3.3 Expiration Date 

sponding cash market may not yet exist.
The strategy of borrowing, buying, and storing the asset until some later
expiration date is not applicable to price-discovery markets. Under these
conditions, any information about the future supply and demand of the
underlying commodity cannot influence the corresponding cash price. Such
information can be discovered in the futures market, hence the terminology. 

The second type of underlying asset comes from price discovery mar-kets. Here, it is physically impossible to buy the underlying instrument for cash and store it until some future expiration date. Such goods either are too perishable to be stored or may not have a cash market at the time the derivative is trading. One example is a contract on spring wheat. When the futures contract for this commodity is traded in the exchange, the cor-sponding cash market may not yet exist. 

## 3.2 Price-Discovery Markets

gold, silver, crude oil, etc.
Pure cash-and-carry markets have one more property. Information about
future demand and supplies of the underlying instrument should not influ-
ence the "spread" between cash and futures (forward) prices. After all, this
spread will depend mostly on the level of risk-free interest rates, storage,
and insurance costs. Any relevant information concerning future supplies
and demands of the underlying instrument is expected to make the cash
price and the future price change by the same amount. 

to buying a futures contract and accepting the delivery of the underlying in- strument at expiration. One can construct similar examples with currencies, gold, silver, crude oil, etc. $^{2}$ 

CHAPTER·1 Financial Derivatives 

At time t, the only known “formula” concerning $C_{t}$ is the one that determines its value at the time of expiration denoted by T. In fact, 

The most desirable way of pricing a call option is to find a closed-form formula for $C_t$ that expresses the latter as a function of the underlying asset's price and the relevant parameters. 

## 5.1 Some Notation

However, the option may be traded infrequently. Then a trader may want to know the daily value of $C_{t}$ in order to evaluate its risks. Another trader may think that the market is mispricing the call option, and the extent of this mispricing may be of interest. Again, the arbitrage-free value of $C_{t}$ needs to be determined. 

There are several reasons that traders and investors may want to calculate the arbitrage-free price, $C_{t}$ , of a call option. Before the option is first written at time t, $C_{t}$ is not known. A trader may want to obtain some estimate of what this price will be if the option is written. If the option is an exchange-traded security, it will start trading and a market price will emerge. If the option trades over-the-counter, it may also trade heavily and a price can be observed. 

DEFINITION: A European-type call option on a security $S_{t}$ is the right to buy the security at a preset strike price K. This right may be exercised at the expiration date T of the option. The call option can be purchased for a price of $C_{t}$ dollars, called the premium, at time t < T. 

Forwards and futures obligate the contract holder to deliver or accept the delivery of the underlying instrument at expiration. Options, on the other hand, give the owner the right, but not the obligation, to purchase or sell an asset. 

Options constitute the second basic building block of asset pricing. In later chapters we often use pricing models for standard call options as a major example to introduce concepts of stochastic calculus. 

5 Options 

or loss during the day is recorded accordingly in the account of the contract holder. 

$^{4}$ Note that because the contract expires at $t+1$ , $S_{t+1}$ will equal $F(t+1)$ . 

custom-made and are issued over the securities.
Futures exchanges are cleared through exchange clearing houses, and
there is an intricate mechanism designed to reduce the default risk.
Finally, futures contracts are marked to market. That is, every day the
contract is settled and simultaneously a new contract is written. Any profit 

Futures and forwards are similar instruments. The major differences can be stated briefly as follows. 

circumstances.
Such payoff diagrams are useful in understanding the mechanics of derivative products. In this book we treat them briefly. The reader can consult Hull (1993) for an extensive discussion. 

If $S_{t+1}$ exceeds $F(t)$ , then the long position ends up with a profit. $^{4}$ Given that the line has unitary slope, the segment AB equals the vertical line BC. At time $t+1$ the gain or loss can be read directly as being the vertical distance between this “payoff” line and the horizontal axis.

Figure 2 displays the payoff diagram of a short position under similar 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/cf450d54b8febd73210133a5d1cd92e0783f0fdfb33679a2aef0f8561f587936.jpg)


Swaps and swoptions are among some of the most common types of derivatives. But this is not why we are interested in them. It turns out that one method for pricing swaps and swoptions is to decompose them into forwards and options. This illustrates the special role played by forwards and options as basic building blocks and justifies the special emphasis put on them in following chapters. 

Figure 4 displays the value of a call option at various times before expiration. Note that for t < T the value of the function can be represented by a smooth continuous curve. Only at expiration does the option value become a piecewise linear function with a kink at the strike price. 

Equation (6), which gives the relation between $S_T$ and $C_T$ , can be graphed easily. Figure 3 shows this relationship. Note that for $S_T \leq K$ , the $C_T$ is zero. For values of $S_T$ such that $K < S_T$ , the $C_T$ increases at the same rate as $S_T$ . Hence, for this range of values, the graph of Eq. (6) is a straight line with unitary slope. Options are nonlinear instruments. 

We can use a shorthand notation to express both of these possibilities by writing 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/d5c49c630b595fadcb209c5a2fdc40a1e655614090147c7c4803e24b5eed22a4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/1a67c3ac37e4503ffa450359890ef2cab7449aafb7ae0c0de0c3bd3b1a5e59e2.jpg)


the option will have some value. One should clearly exercise the option. One can buy the underlying security at price K and sell it at a higher price $S_{T}$ . Since there are no commissions or bid-ask spreads, the net profit will be $S_{T}-K$ . Market participants, being aware of this, will place a value of $S_{T}-K$ on the option, and we have 

then the option will have no value. The underlying asset can be purchased in the market for $S_{T}$ , and this is less than the strike price K. No option holder will exercise his or her right to buy the underlying asset at K. Thus, 

then at expiration, $C_T$ can assume only two possible values. If the option is expiring out-of-money, that is, if at expiration the option holder faces 

- if there are no commissions and/or fees, and
- if the bid-ask spreads on $S_{t}$ and $C_t$ are zero, 

Hull (2000) is an excellent source on derivatives that is unique in many ways. Practitioners use it as a manual; beginning graduate students utilize it as a textbook. It has a practical approach and is meticulously written. Jarrow and Turnbull (1996) is a welcome addition to books on derivatives. Duffie (1996) is an excellent source on dynamic asset pricing theory. However, it is not a source on the details of actual instruments traded in the markets. Yet, practitioners with a very strong math background may find it useful. Das (1994) is a useful reference on the practical aspects of derivative instruments. 

In this chapter, we have reviewed some basic derivative instruments. Our purpose was twofold: first, to give a brief treatment of the basic derivative securities so we can use them in examples; and second, to discuss some notation in derivative asset pricing, where one first develops pricing formulas for simple building blocks, such as options and forwards, and then decomposes more complicated structures into baskets of forwards and options. This way, pricing formulas for simpler structures can be used to value more complicated structured products. 

will secure lower rates and the swap dealer will can a nice.
It is always possible to decompose simple swap deals into a basket of simpler forward contracts. The basket will replicate the swap. The forwards can then be priced separately, and the corresponding value of the swap can be determined from these numbers. This decomposition into building blocks of forwards will significantly facilitate the valuation of the swap contract. 

This very basic interest rate swap consists of exchanges of interest payments. The counterparties borrow in sectors where they have an advantage and then exchange the interest payments. At the end both counterparties will secure lower rates and the swap dealer will earn a fee. 

$^{5}$ Other recent sources on practical applications of swaps are Dattatreya et al. (1994) and Kapner and Marshall (1992). 

fending bank.
5. Note that the initial sums, each being $1 million, are identical. Hence, they do not have to be exchanged. They are called notional principals. The interest payments are also in the same currency. Hence, the counter-parties exchange only the interest differentials. This concludes the interest rate swap. 

4. Counterparty B borrows $1 million at the floating rate. Interest payments will be received from counterparty A and will be repaid to the lending bank. 

then decides to exchange the interest payeeves.
3. Counterparty A borrows $1 million at a fixed rate. The interest pay-
ments will be received from counterparty B and paid back to the lending
bank 

1. Counterparty A needs a $1 million floating-rate loan. Counterparty B needs a $1 million fixed-rate loan. But because of market conditions and their relationships with various banks, B has a comparative advantage in borrowing at a floating rate. $^{6}$ 

In its simplest form, an interest rate swap between two counterparties and B is created as a result of the following steps: 

Decomposing a swap into its constituent components is a potent example of financial engineering and derivative asset pricing. It also illustrates the special role played by simple forwards and options. We discuss an interest rate swap in detail. Das (1994) can be consulted for more advanced swap structures. $^{5}$ 

6.1 A Simple Interest Rate Swap 

Even a brief summary of swap instruments is outside the scope of this book. As mentioned earlier, our intention is to provide a heuristic introduction of the mathematics behind derivative asset pricing, and not to discuss the derivative products themselves. We limit our discussion to a typical example that illustrates the main points. 

DEFINITION: A swap is the simultaneous selling and purchasing of cash flows involving various currencies, interest rates, and a number of other financial assets. 

In arbitrage opportunities of the second kind, a portfolio can ensure a negative net commitment today, while yielding nonnegative profits in the future. 

Arbitrage opportunities can arise in two different fashions. In the first way, one can make a series of investments with no current net commitment, yet expect to make a positive profit. For example, one can short-sell a stock and use the proceeds to buy call options written on the same security. In this portfolio, one finances a long position in call options with short positions in the underlying stock. If this is done properly, unpredictable movements in the short and long positions will cancel out, and the portfolio will be riskless. Once commissions and fees are deducted, such investment opportunities should not yield any excess profits. Otherwise, we say that there are arbitrage opportunities of the first kind. In arbitrage opportunities of the second kind, a portfolio can ensure a 

In its simplest form, arbitrage means taking simultaneous positions in different assets so that one guarantees a riskless profit higher than the riskless return given by U.S. Treasury bills. If such profits exist, we say that there is an arbitrage opportunity. 

All current methods of pricing derivative assets utilize the notion of arbitrage. In arbitrage pricing methods this utilization is direct. Asset prices are obtained from conditions that prechude arbitrage opportunities. In equilibrium pricing methods, lack of arbitrage opportunities is part of general equilibrium conditions. 

# A Primer on the Arbitrage Theorem

is the value of $F_{t}$ (b) Suppose the market starts quoting a price $F_{t} = 101$ for this contract. Form two arbitrage portfolios. 

(a) A trader writes a forward contract on the delivery of this stock. The delivery will be within 12 months and the price is $F_{t}$ . What 

4. An at-the-money call written on a stock with current price $S_{t} = 100$ trades at 3. The corresponding at-the-money put trades at 3.5. There are no transaction costs and the stock does not pay any dividends. Traders can borrow and lend at a rate of 5% per year and all markets are liquid. 

(c) Assuming that all the parameters of the problem remain the same, what would be the profit or loss of an arbitrage portfolio at expiration? 

(a) Obtain a formula for $F_t$ .
(b) Let the $F_t = 1500, r = 5\%, s = 100, c = 150$ and the spot price of wheat be $S_t = 1470$ . Is this $F_t$ arbitrage-free? How would you 

3. Let the arbitrage-free 3-month futures price for wheat be denoted by $F_{t}$ . Suppose it costs c$ to store 1 ton of wheat for 12 months and s$ per year to insure the same quantity. The (simple) interest rate applicable to traders of spot wheat is r%. Finally assume that the wheat has no convenience yield. 

lected FRAs in detail.
(c) Could you generate a synthetic swap using appropriate interest rate options? 

(a) Represent the cash flows generated by this swap on a graph.
(b) Create a synthetic equivalent of this swap using two Forward Rate Agreements (FRA) contracts. Describe the parameters of the se-

- The start date is in 12 months, the maturity is 24 months.
- Floating rate is 6 month USD Libor.
- The swap rate is $\kappa = 5\%$ . 

2. Consider a fixed-payer, plain vanilla, intercst rate swap paid in arrears with the following characteristics: 

(a) Plot the expiration payoff diagrams in each case.
(b) How would these diagrams look some time before expiration? 

- An investor buys one put with a strike price of $K_{1}$ and one call option at a strike price of $K_{2}$ with $K_{1} \leq K_{2}$ .
- An investor buys one put and writes one call with strike price $K_{1}$ , and buys one call and writes one put with strike price $K_{2}(K_{1} \leq K_{2})$ . 

CHAPTER·1 Financial Derivatives 

To proceed with the rest of this chapter, we need one more concept—a concept that, at the outset, may appear to be very abstract, yet has significant practical relevance. We let the vector W denote all possible states of the world, 

Here, $S_{1}(t)$ may be riskless borrowing or lending, $S_{2}(t)$ may denote a particular stock, $S_{3}(t)$ may be a call option written on this stock, $S_{4}(t)$ may represent the corresponding put option, and so on. The $t$ subscript in $S_{t}$ means that prices belong to time represented by the value of $t$ . In discrete time, securities prices can be expressed as $S_{0}, S_{1}, \ldots, S_{t}, S_{t+1}, \ldots$ . However, in continuous time, the $t$ subscript can assume any value between zero and infinity. We formally write this as 

The index t will represent time. Securities such as options, futures, forwards, and stocks will be represented by a vector of asset prices denoted by $S_{t}$ . This array groups all securities in financial markets under one symbol: 

ing of the notation is sometimes as important as an understanding of the underlying mathematical logic. 

$^{1}$ Note that devising such scenarios is not at all straightforward. For example, it is not clear that markets will have the necessary liquidity to secure no-arbitrage conditions if they are hit by some extreme shock. 

We begin with some formalism and start developing the notation that is an integral part of every mathematical approach. A correct understand-

2 Notation 

The mathematical environment provided by the no-arbitrage theorem is the major tool used to calculate such benchmark prices. 

Finally, arbitrage-free benchmark prices can be compared with prices observed in actual trading. Significant differences between observed and arbitrage-free values might indicate excess profit opportunities. This way arbitrage-free prices can be used to detect mispricings that may occur during short intervals. If the arbitrage-free price is above the observed price, the derivative is cheap. A long position may be called for. When the opposite occurs, the derivative instrument is overvalued.
The mathematical environment provided by the no-arbitrage theorem is 

A third example is marking to market of assets held in portfolios. A treasurer may want to know the current market value of a nonliquid asset for which no trades have been observed lately. Calculating the corresponding arbitrage-free price may provide a solution. 

A second example is from risk management. Often, risk managers would like to measure the risks associated with their portfolios by running some “worst case” scenarios. These simulations are repeated periodically. Each time some benchmark price needs to be utilized, given that what is in question is a hypothetical event that has not been observed. $^{1}$ 

One case may be when a derivatives house decides to engineer a new financial product. Because the product is new, the price at which it should be sold cannot be obtained by observing actual trading in financial markets. Under these conditions, calculating the arbitrage-free price will be very helpful in determining a market price for this product. 

In practice, arbitrage opportunities may exist. This, however, would not reduce our interest in “arbitrage-free” prices. In fact, determining arbitrage-free prices is at the center of valuing derivative assets. We can imagine at least four possible utilizations of arbitrage-free prices. 

We use these concepts to obtain a practical definition of a “fair price” for a financial asset. We say that the price of a security is at a “fair” level, or that the security is correctly priced, if there are no arbitrage opportunities of the first or second kind at those prices. Such arbitrage-free asset prices will be utilized as benchmarks. Deviations from these indicate opportunities for excess profits. 

2. An underlying asset, for example, a stock $S(t)$ . We assume that during the small interval $\Delta$ , $S(t)$ can assume one of only two possible values. This means a minimum of two states of the world. $S(t)$ is risky because its payoff is different in each of the two states. 

1. A risk-free asset such as a Treasury bill, whose gross return until next period is $(1+r\Delta)^{4}$ . This return is “risk-free,” in that it is constant regardless of the realized state of the world. 

We assume that time consists of “now” and a “next period” and that these two periods are separated by an interval of length $\Delta$ . Throughout this book $\Delta$ will represent a “small” but noninfinitesimal interval. We consider a case where the market participant is interested only in three assets: 

We use a simple model to explain most of the important results in pricing derivative assets. With this example, we first intend to illustrate the logic used in derivative asset pricing. Second, we hope to introduce the mathematical tools needed to carry out this logic in practical applications. The model is kept simple on purpose. A more general case is discussed at the end of the chapter. 

## 3 A Basic Example of Asset Pricing

A portfolio is a particular combination of assets in question. To form a portfolio, one needs to know the positions taken in each asset under consideration. The symbol $\theta_{i}$ represents the commitment with respect to the $i$ th asset. Identifying all $\{\theta_i; i = 1 \dots N\}$ specifies the portfolio. 

given state of the world.
If current prices of all assets are nonzero, then one can divide the ith row of D by the corresponding $S_{i}(t)$ and obtain the gross returns in different states of the world. The D will have a t subscript in the general case when payoffs depend on time. 

3 A Basic Example of Asset Pricing 

$^{2}$ To realize a capital gain, one must unwind the position. $^{3}$ Another example, besides dividend-paying stocks and coupon bonds, is investment in futures. The practice of “marking to market” leads to daily payouts to a contract holder. However, in the case of futures, these payouts may be negative or positive. 

There are two different ways one can visualize such a matrix. One can look at the matrix D as if each row represents payoffs to one unit of a given security in different states of the world. Conversely, one can look at D 

The first component is capital gains or losses. Asset values appreciate or depreciate. For an investor who is “long” in the asset, an appreciation leads to a capital gain and a depreciation leads to a capital loss. For somebody who is “short” in the asset, capital gains and losses will be reversed. $^{2}$ 

The states of the world $w_{i}$ matter because in different states of the world returns to securities would be different. We let $d_{ij}$ denote the number of units of account paid by one unit of security $i$ in state $j$ . These payoffs will have two components. 

## 2.3 Returns and Payoffs

It is not very difficult to visualize this concept. Suppose that from a trader's point of view, the only time of interest is the "next" instant. Clearly, securities prices may change, and we do not necessarily know how. Yet, in a small time interval, securities prices may have an "uptick" or a "downtick," or may not show any movement at all. Hence, we may act as if there are a total of three possible states of the world. 

In general, financial assets will have different values and give different payouts at different states of the world $w_{i}$ . It is assumed that there are a finite number $K$ of such possible states. 

$^{6}$ Note that if $1 + r > 1$ , we need to have $\psi_{1} + \psi_{2} < 1$ as well. This is obtained from the first row of the matrix equation. 

Thus, investors are willing to pay $\psi_{1}$ (current) units for an “insurance policy” that offers one unit of account in state 1 and nothing in state 2. Similarly, $\psi_{2}$ indicates how much investors would like to pay for an “insurance 

What do the constants $\psi_1, \psi_2$ represent? According to the second row of the representation implied by the arbitrage theorem, if a security pays 1 in state 1, and 0 in state 2, then 

The relationship in (10) is called a representation. It is not a relation that can be observed in reality. In fact, $S_{1}(t+1)$ and $S_{2}(t+1)$ are “possible” future values of the underlying asset. Only one of them—namely, the one that belongs to the state that is realized—will be observed. 

We are now ready to introduce a fundamental result in financial theory that can be used in calculating fair market values of derivative assets. But first we will simplify the notation even further. The amount of risk-free borrowing and lending is selected by the investor. Hence, we can always let 

3.1 A First Glance at the Arbitrage Theorem 

3 A Basic Example of Asset Pricing 

$^{5}$ In fact, we show later that a continuous-time Wiener process, or Brownian motion, can be approximated arbitrarily well by such two-state processes, as we let the $\Delta$ go toward zero. 

where r is the annual riskless rate of return. 

$\begin{array}{r}D_{t} = \left[ \begin{array}{lll}(1 + r\Delta)B(t) & (1 + r\Delta)B(t)\\ S_{1}(t + \Delta) & S_{2}(t + \Delta)\\ C_{1}(t + \Delta) & C_{2}(t + \Delta) \end{array} \right], \end{array}$ 

Payoffs will be grouped in a matrix $D_{t}$ , as discussed earlier. There are three assets, which means that matrix $D_{t}$ will have three rows. Also, there are two states of the world; the $D_{t}$ matrix will thus have two columns. The $B(t)$ is riskless borrowing or lending. Its payoff will be the same, regardless of the state of the world that applies in the “next instant.” The $S(t)$ is risky and its value may go either up to $S_{1}(t+\Delta)$ or down to $S_{2}(t+\Delta)$ . Finally, the market value of the call option $C(t)$ will change in line with movements in the underlying asset price $S(t)$ . Thus, $D_{t}$ will be given by: 

where $B(t)$ is riskless borrowing or lending, $S(t)$ is a stock, and $C(t)$ is the value of a call option written on this stock. The $t$ indicates the time for which these prices apply. 

The example is not altogether unrealistic. A trader operating in real (continuous) time may contemplate taking a (covered) position in a particular option. If the time interval under consideration is “small,” prices of these assets may not change by more than an up- or a downtick. Hence, the assumption of two states of the world may be a reasonable approximation. $^{5}$ We summarize this information in terms of the formal notation discussed earlier. Asset prices will form a vector $S_{t}$ of only three elements, 

This setup is fairly simple. There are three assets $(N = 3)$ , and two states of the world $(K = 2)$ . The first asset is risk-free borrowing and lending, the second is the underlying security, and the third is the option. 

3. A derivative asset, a call option with premium $C(t)$ and a strike price $C_{o}$ . The option expires “next” period. Given that the underlying asset has two possible values, the call option will assume two possible values as well. 

CHAPTER·2 A Primer on the Arbitrage Theorem 

But, we can replace $(1 + r)\psi_{i}, i = 1,2$ with the corresponding $\tilde{P}_i$ , $i = 1,2$ . This means that the two equations become 

Risk-adjusted probabilities exist if there are no arbitrage opportunities. In other words, if there are no “mispriced assets,” we are guaranteed to find positive constants $\{\psi_{1},\psi_{2}\}$ . Multiplying these by the riskless gross return $1+r$ guarantees the existence of $\{P_{1},P_{2}\}^{8}$ . 

Hence, $\tilde{P}_{i}$ 's are positive numbers, and they sum to one. As such, they can be interpreted as two probabilities associated with the two states under consideration. We say "interpreted" because the true probabilities that govern the occurrence of the two states of the world will in general be different from the $\tilde{P}_{1}$ and $\tilde{P}_{2}$ . These are defined by Equation (14) and provide no direct information concerning the true probabilities associated with the two states of the world. For this reason, $\{\tilde{P}_{1},\tilde{P}_{2}\}$ are called risk-adjusted synthetic probabilities. 

For the moment, let us put the first two questions aside and answer the third question: What types of practical results (if any) does one obtain from the existence of $\psi_{1}, \psi_{2}$ ? It turns out that the representation given by the arbitrage theorem is very important for practical asset pricing. 

- How does one obtain this theorem?
- What does the existence of $\psi_1, \psi_2$ have to do with no arbitrage?
- Why is this result relevant for asset pricing? 

policy" that pays 1 in state 2 and nothing in state 1. Clearly, by spending $\psi_{1} + \psi_{2}$ , one can guarantee 1 unit of account in the future, regardless of which state is realized. This is confirmed by the first row of representation (10). Consistent with this interpretation, $\psi_{i}, i = 1,2$ are called state prices. At this point there are several other issues that may not be clear. One can in fact ask the following questions: 

These equations are very convenient to use, and they internalize any risk premiums. Indeed, one does not need to calculate the risk premiums if one uses synthetic expectations. The corresponding discounting is done using the risk-free rate, which is easily observable. 

The importance of the no-arbitrage assumption in asset pricing should become clear at this point. If no-arbitrage implies the existence of positive constants such as $\psi_{1}, \psi_{2}$ , then we can always obtain from these constants the risk-adjusted probabilities $\bar{P}_{1}, \bar{P}_{2}$ and work with “synthetic” expectations that satisfy 

But this means that (true) expected returns from the risky assets equal risk-less return. This, however, is a contradiction, because in general risky assets will command a positive risk premium. If there is no such compensation for risk, no investor would hold them. Thus, for risky assets we generally have 

$^{10}$ We say “in general” because one can imagine risky assets that are negatively correlated with the “market.” Such assets may have negative risk premiums and are called “negative beta” assets. 

As long as the underlying probabilities are implicitly greater. With this interpretation of $\tilde{P}_1, \tilde{P}_2$ , the current prices of all assets under consideration become equal to their discounted expected payoffs. Further, the discounting is done using the risk-free rate, although the assets themselves are risky 

the risk-adjusted probabilities.
As such, the equalities in (21) and (22) do not represent “true” expected values. Yet as long as there is no arbitrage, these equalities are valid, and they can be used in practical calculations. We can use them in asset pricing, as long as the underlying probabilities are explicitly specified.
With this interpretation of B & F, the current prices of all assets under 

Now consider how these expressions can be interpreted. The expression on the right-hand side multiplies the term in the brackets by $1/(1+r)$ , which is a riskless one-period discount factor. On the other hand, the term inside the brackets can be interpreted as some sort of expected value. It is the sum of possible future values of $S(t)$ or $C(t)$ weighted by the “probabilities” $\tilde{P}_{1}, \tilde{P}_{2}$ . Hence, the terms in the brackets are expectations calculated using the risk-adjusted probabilities. 

$^{13}$ In probability theory, the phrase “under $\tilde{P}_{1}, \tilde{P}_{2}$ ” means “if one uses the probabilities $\tilde{P}_{1}$ and $\tilde{P}_{2}$ ” 

are the gross rates of return of $S(t)$ in states 1 and 2, respectively. The equalities (43) and (44) imply that if one uses $\tilde{P}_{1}, \tilde{P}_{2}$ in calculating the expected values, all assets would have the same expected return. According to this new result, “under $\tilde{P}_{1}, \tilde{P}_{2}$ ,” all expected returns equal the risk-free return $r^{13}$ . This is another widely used result in pricing financial assets. 

$$
\tilde {P} _ {1} \frac {S _ {1} (t + 1)}{S (t)} + \tilde {P} _ {2} \frac {S _ {2} (t + 1)}{S (t)} = (1 + r)
$$

Is the ratio: An interesting question that we investigate in the second half of this book is then the following. Suppose we divide the $S_{i}$ by some other asset's price, say $C_{i}$ ; would the new ratio, 

be a martingale with respect to some other probability, say $P^{*}$ ? The answer to this question is positive and is quite useful in pricing interest sensitive derivative instruments. Essentially, it gives us the flexibility to work with a more convenient probability by normalizing with an asset of our choice. But these issues have to wait until Chapter 17. 

was a martingale with respect to the risk-adjusted probability $\tilde{P}$ . Second, note that it is not the $S_{t}$ that is a martingale, but rather the $S_{t}$ divided, or normalized, by the $(1 + r)^{s}$ . The latter is the earnings of 1$ over s periods if invested and rolled-over in the risk-free investment. What is a martingale is the ratio. 

$^{12}$ There are other conditions that a martingale must satisfy. In later chapters, we discuss them in detail. In the meantime, we assume implicitly that these conditional expectations exist—that is, they are finite. 

It is important to realize that, in finance, the notion of martingale is always associated with two concepts. First, a martingale is always defined with respect to a certain probability. Hence, in Section 3.4 the discounted stock price, 

Here $S_{t+s}$ and r are the security price and risk-free return, respectively. $\tilde{P}$ is the risk-adjusted probability. According to this, utilization of risk-adjusted probabilities will convert all (discounted) asset prices into martingales. 

then $X_{t}$ is called a submartingale with respect to probability $Q$ . Here is why these concepts are fundamental. According to the discussion in the previous section, asset prices discounted by the risk-free rate will be submartingales under the true probabilities, but become martingales under the risk-adjusted probabilities. Thus, as long as we utilize the latter, the tools available to martingale theory become applicable, and "fair market values" of the assets under consideration can be obtained by exploiting the martingale equality 

This is the right time to introduce a concept that is at the foundation of pricing financial assets. We give a simple definition of the terms and leave technicalities for later chapters. 

If this was the case, then one could short the $S(t)$ and invest the proceeds in the risk-free investment to realize infinite gains. Again Equation (48) will not be satisfied with positive $\psi_1, \psi_2$ , because the right-hand side will always be positive under these conditions. Thus, we see that the existence of positive $\psi_1, \psi_2$ is closely tied to the condition 

We first divide the time interval $(T-t)$ into n smaller intervals, each of size $\Delta$ . We choose a “small” $\Delta$ , in the sense that the variations of $S_{t}$ during $\Delta$ can be approximated reasonably well by an up or down movement only. According to this, we hope that for small enough $\Delta$ the underlying asset price $S_{t}$ cannot wander too far from the currently observed price $S_{t}$ . Thus, we assume that during $\Delta$ the only possible changes in $S_{t}$ are an up movement by $\sigma\sqrt{\Delta}$ or a down movement by $-\sigma\sqrt{\Delta}$ : 

The same method of determining the unique arbitrage-free value of the call option would not work if there were more than two states of the world. For example, consider the system 

It turns out that in this particular case, the representation given by the arbitrage theorem is satisfied with positive and unique $\psi_{i}$ . This may not always be true. 

At this price, arbitrage profits do not exist. Note that, using the constants $\psi_1, \psi_2$ , we derived the arbitrage-free price $C = 9.09$ . In this sense, we used the arbitrage theorem as an asset-pricing tool. 

But now, instead of starting with an observed value of C, solve the first two equations for $\psi_{1}, \psi_{2}$ . These form a system of two equations in two unknowns. The unique solution gives 

Clearly, at the observed value for the call premium, C = 25, it is impossible to find $\psi_{1}, \psi_{2}$ that satisfies all three equations given by the arbitrage-free representation. Arbitrage opportunities therefore exist. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/d4226220a5e935b5cd27a81fcd83aef439569f7117fd16265f936783477886fb.jpg)


Hence, the procedure is to use the dynamics of $S_{i}$ to go forward and determine the expiration date values of the call option. Then, using the risk-adjusted probabilities and the boundary condition, one works backward with the lattice for the call option to determine the current value $C_{i}$ . It is the arbitrage theorem and the implied martingale equalities that make it possible to calculate the risk-adjusted probabilities $\bar{P}_{up}$ and $\bar{P}_{down}$ . 

Figure 2 shows the multiplicative lattice for the option price $C_t$ . The arbitrage-free values of $C_t$ are at this point indeterminate, except for the expiration "nodes." In fact, given the lattice for $S_t$ , we can determine the values of $C_t$ at the expiration using the boundary condition 

“ties” two (arbitrage-free) values of the call option at any time $t+\Delta$ to the (arbitrage-free) value of the option as of time t. The $P_{up}$ is known at this point. In order to make the equation usable, we need the two values $C_{t+\Delta}^{up}$ and $C_{t+\Delta}^{down}$ . Given these, we can calculate the value of the call option $C_{t}$ at time t. 

$^{15}$ In the second half of the book, we will relax the assumption that r is constant. But for now we maintain this assumption 

Once this is done, the $\tilde{P}_{up}$ can be used to calculate the current arbitrage-free value of the call option. In fact, the equation 

In this equation, $r$ , $S$ , $\sigma$ , and $\Delta$ are known. The first three are observed in the markets, while $\Delta$ is selected by us. Thus, the only unknown is the $\tilde{P}_{up}$ , which can be determined easily. $^{16}$ 

Suppose now that we are given the (constant) risk-free rate r for the period $\Delta$ . Can we determine the risk-adjusted probabilities? $^{15}$ We know from the arbitrage theorem that the risk-adjusted probabilities $\tilde{P}_{up}$ and $\tilde{P}_{down}$ must satisfy 

The dynamics described by Equation (65) represent a lattice or a binomial tree. Figure 1 displays these dynamics in the case of multiplicative up and down movements. 

Clearly, the size of the parameter $\sigma$ determines how far $S_{t + \Delta}$ can wander during a time interval of length $\Delta$ . For that reason it is called the volatility parameter. The $\sigma$ is known. Note that regardless of $\sigma$ , in smaller intervals, $S_{t}$ will change less. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/a7ea2245eed439b74f50a6e67f72ca74839859ce3c40ff1ce7e405fdbd1ab98f.jpg)


According to this last equation, we can state the following. If we were to let $\Delta$ go to zero and switch to continuous time, the drift term for $dS_{t}$ , which represents expected change in the underlying asset's price, will be given by $(r - d)S_{t}dt$ and the corresponding dynamics can be written as:17 

where $\tilde{P}$ is the risk-neutral probability, and where we ignored the time subscripts. Note that the first equation is now different from the case with no-dividends, but that the second equation is the same. According to this, each time an asset has some known percentage payout d during the period $\Delta$ , the risk-neutral discounting of the dividend paying asset has to be done using the factor $(1+d)/(1+r)$ instead of multiplying by $1/(1+r)$ only. It is also worth emphasizing that the discounting of the derivative itself did not change.
Now consider the following transformation: 

Inclusion of Section 3: Can we proceed the same way as in Section 3? The answer is positive. With minor modifications, we can apply the same steps and obtain two equations: 

$$
\left[ \begin{array}{c} B _ {t} \\ S _ {t} \\ C _ {t} \end{array} \right] = \left[ \begin{array}{c c} B _ {t + \Delta} ^ {u} & B _ {t + \Delta} ^ {d} \\ S _ {t + \Delta} ^ {u} + d _ {t} S _ {t + \Delta} ^ {u} & S _ {t + \Delta} ^ {d} + d _ {t} S _ {t + \Delta} ^ {d} \\ C _ {t + \Delta} ^ {u} & C _ {t + \Delta} ^ {d} \end{array} \right] \left[ \begin{array}{c} \psi_ {t} ^ {u} \\ \psi_ {t} ^ {d} \end{array} \right],
$$

The setup of Section 3 is first modified by adding a dividend equal to $d_{t}$ percent of $S_{t + \Delta}$ . Note two points. First, the dividends are not lump-sum, but are paid as a percentage of the price at time $t + \Delta$ . Second, the dividend payment rate has subscript $t$ instead of $t + \Delta$ . According to this, the $d_{t}$ is known as of time $t$ . Hence, it is not a random variable given the information set at $I_{t}$ . 

In this section we modify the simple two-state model introduced in this chapter to introduce two complications that are more often the case in practical situations. The first is the payment of interim payouts such as dividends and coupons. Many securities make such payments before the expiration date of the derivative under consideration. These payouts do change the pricing formulas in a simple, yet at first sight, counterintuitive fashion. The second complication is the case of foreign currency denominated assets. Here also the pricing formulas changes slightly. 

In this procedure Figure 1 gives an approximation of all the possible paths that $S_{t}$ may take during the period $T - t$ . The tree in Figure 2 gives an approximation of all possible paths that can be taken by the price of the call option written on $S_{t}$ . If $\Delta$ is small, then the lattices will be close approximations to the true paths that can be followed by $S_{t}$ and $C_{t}$ . 

$$
E ^ {\tilde {P}} \left[ \frac {e _ {t + \Delta}}{e _ {t}} \right] \cong 1 + (r - r ^ {f}) \Delta
$$

Again, note that the first equation is different but the second equation is the same. Thus, each time we deal with a foreign currency denominated asset that has payout $r^{f}$ during $\Delta$ , the risk-neutral discounting of the foreign asset has to be done using the factor $(1+r)/(1+r^{f})$ . Note the first-order approximation if $r^{f}$ is small: 

$$
C = \frac {1}{(1 + r)} \left[ C ^ {u} \tilde {p} ^ {u} + C ^ {d} \tilde {p} ^ {d} \right].
$$

$$
e = \frac {(1 + r ^ {f})}{(1 + r)} \left[ e ^ {u} \bar {P} ^ {u} + e ^ {d} \bar {P} ^ {d} \right]
$$

where the $C_{t}$ denotes a call option on price $e_{t}$ of one unit of foreign currency. The strike price is $K.^{18}$ We proceed in a similar fashion to the case of dividends and obtain the following pricing equations: $^{19}$ 

$$
\left[ \begin{array}{c} 1 \\ 1 \\ C _ {t} \end{array} \right] = \left[ \begin{array}{c c} (1 + r) & (1 + r) \\ \frac {e _ {t + \Delta} ^ {u}}{e _ {t}} (1 + r ^ {f}) & \frac {e _ {t + \Delta} ^ {d}}{e _ {t}} (1 + r f) \\ C _ {t + \Delta} ^ {u} & C _ {t + \Delta} ^ {d} \end{array} \right] \left[ \begin{array}{c} \psi_ {t} ^ {u} \\ \psi_ {t} ^ {d} \end{array} \right],
$$

These are slight modifications in the formulas, but in practice they may make a significant difference in pricing calculations. The case of foreign currencies below yields similar results. 

$$
E ^ {\tilde {p}} \left[ \frac {S _ {t + \Delta}}{S _ {t}} \right] = \frac {(1 + r \Delta)}{(1 + d \Delta)} \cong 1 + (r - d) \Delta
$$

Thus, we see that even though there is a divided payout made by the underlying stock, the risk-neutral expected return and the risk-free discounting remains the same for the call option written on this stock. Hence, in a risk-neutral world future returns to $C_{t}$ have to be discounted exactly by the same factor as in the case of no-dividends.
In other words: 

There is a second interesting point to be made with the introduction of payouts. Suppose now we try to go over similar steps using, this time, the equation for $C_t$ shown in (71): 

Third, we need to understand how to obtain risk-adjusted probabilities and how to determine the correct discounting factor. The Girsanov theorem states the conditions under which such risk-adjusted probabilities can be used. The theorem also gives the form of these probability distributions. 

Second, we need to handle the notion of “randomness” during such infinitesimal periods. Concepts such as probability, expectation, average value, and volatility during infinitesimal periods need to be carefully defined. This requires the study of the so-called stochastic calculus. We try to discuss the intuition behind the assumptions that lead to major results in stochastic calculus. 

The arbitrage theorem provides a powerful methodology for determining fair market values of financial assets in practice. The major steps of this methodology as applied to financial derivatives can be summarized as follows: 

(74) 

Using continuous-time models leads to a change in the way discounting is done. In fact, if t is continuous, then the discount factor for an interval of length $\Delta$ will be given by the exponential function 

where the symbol $dS_{t}$ represents an infinitesimal change in the price of the security, the $\mu_{t}S_{t}dt$ is the predicted movement during an infinitesimal interval $dt$ , and $\sigma_{t}S_{t}dW_{t}$ is an unpredictable, infinitesimal random shock. It is obvious that most of the concepts used in defining stochastic differential equations need to be developed step by step. 

(73) 

$dS_{i}=\mu_{i}S_{i}dt+\sigma_{i}S_{i}dW_{i},$ 

states of the world.
To capture such generalizations, we need to introduce stochastic differential equations. For example, as mentioned above increments in security prices $S_{i}$ may be modeled using 

1.2 States of the world
In continuous time, the values that an asset can assume are not limited to two. There may be uncountably many possibilities and a continuum of states of the world. 

This way, in addition to the “small” time interval $\Delta$ dealt with in this chapter, we can consider infinitesimal intervals denoted by the symbol dt. 

Up to this point we considered discrete time with $t = 1,2,3,\ldots$ . In continuous-time asset pricing models, this will change. We have to assume that $t$ is continuous: 

Up to this point, the setup has been very simple. In general, such simple examples cannot be used to price real-life financial assets. Let us briefly consider some generalizations that are needed to do so. 

7 Some Generalizations 

According to the last remark, if we were to let $\Delta$ go to zero and switch to SDE's, the drift terms for $dC_{t}$ will be given by $rC_{t}dt$ . But the drift term for the foreign currency denominated asset, $de_{t}$ , will now have to be $(r - rf)e_{t}dt$ . 

CHAPTER·2 A Primer on the Arbitrage Theorem 

1. If there are no arbitrage opportunities, then there exists a $\psi > 0$ such that 

According to this, the portfolio $\theta$ guarantees some positive return in all states, yet it costs nothing to purchase. Or it guarantees a nonnegative return while having a negative cost today. 

• We can now define an arbitrage portfolio:
DEFINITION: $\theta$ is an arbitrage portfolio, or simply an arbitrage, if either one of the following conditions is satisfied: 

$$
D ^ {\prime} \theta = \left[ \begin{array}{c c c} d _ {1 1} & \dots & d _ {N 1} \\ \vdots & \vdots & \vdots \\ d _ {1 K} & \dots & d _ {N K} \end{array} \right] \left[ \begin{array}{c} \theta_ {1} \\ \vdots \\ \theta_ {N} \end{array} \right].
$$

In dealer's terminology, $\theta$ gives the positions taken at a certain time. Multiplying the $\theta$ by $S_{t}$ , we obtain the value of portfolio $\theta$ : 

In this chapter, arbitrage theorem was treated in a simple way. Ingersoll (1987) provides a much more detailed treatment that is quite accessible, even to a beginner. Readers with a strong quantitative background may prefer Duffie (1996). The original article by Harrison and Kreps (1979) may also be consulted. Other related material can be found in Harrison and Pliska (1981). The first chapter in Musiela and Rutkowski (1997) is excellent and very easy to read after this chapter. 

## 9 References

a stochastic differential equation (SDP):
Needless to say, in order to attack these topics in turn, one must have some notion of the well-known concepts and results of “standard” calculus.
There are basically three: (1) the notion of derivative, (2) the notion of integral, and (3) the Taylor series expansion. 

(a) Arc the "current" prices of the three securities arbitrage-free?  
(b) If not, what type of arbitrage portfolio should one form?  
(c) Determine a set of arbitrage-free prices for securities A, B, and C (a) Find the risk-neutral martingale measure $P^{*}$ using the normalization by risk-free borrowing and lending.
(b) Calculate the value of the option under the risk-neutral martingale measure using 

The true probabilities of the two states are given by $\{P^u = .5, P^d = .5\}$ . The current price is $S_t = 280$ . The annual interest rate is constant at $r = 5\%$ . The time is discrete, with $\Delta = 3$ months. The option has a strike price of $K = 280$ and expires at time $t + \Delta$ . 

and that the $S_{i}$ is arbitrage-free. What is the value of $p$ ? Would a $p = 1/3$ bc consistent with arbitrage-free $S_{i}$ ? 

The 0 < p < 1 is a parameter.
• Volatility is 12% a year.
• The stock pays no dividends and the current stock price is 100. 

$\epsilon = \left\{ \begin{array}{ll} + 1 & \text{with probability } P \\ -1 & \text{with probability } 1 - P. \end{array} \right.$ 

6. Suppose you are given the following data:
• Risk-free yearly interest rate is $r = 6\%$ .
• The stock price follows: 

that replicates the option.
(b) Using the replicating portfolio price this call.
(c) Suppose you sell, over-the-counter, 100 such calls to your customers. How would you hedge this position? Be precise.
(d) Suppose the market price of this call is 5. How would you form an arbitrage portfolio? 

(a) Consider a European call option written on $S_{t}$ . The call has a strike price $K = 120$ and an expiration of 3 months. Using the $S_{t}$ and the risk-free borrowing and lending, $B_{t}$ , construct a portfolio that initiates the option 

It is hoped that the dynamic behavior of $S_{t}$ can be approximated reasonably well by a binomial process if one assumes observation intervals of length 1 month. 

- Current value = 102.
- Annual volatility = 30%.
- You are also given the spot rate $r = 5\%$ , which is known to be constant during the next 3 months. 

distribution?
(b) Calculate the four-step binomial trees for the $S_{t}$ and the $C_{t}$ .
(c) Calculate the arbitrage-free price $C_{o}$ of the option at time t = 0. 

(a) According to the data given above, what is the (approximate) annual volatility of $S_{i}$ if this process is known to have a log-normal trend? 

where $up$ and $down$ describe the two states of the world at each node. Assume that time is measured in months and that $t = 4$ is the expiration date for a European call option $C_t$ written on $S_t$ . The stock does not pay any dividends and its price is expected (by "market participants") to grow at an annual rate of $15\%$ . The risk-free interest rate $r$ is known to be constant at $5\%$ . 

$S_{i + \Delta}^{uP} = uS_{t}$ 

These up and down movements apply to one-month periods denoted by $\Delta = 1$ . We have the following dynamics for $S_{t}$ , 

4. A four-step binomial tree for the price of a stock $S_{f}$ is to be calculated using the up and down ticks given as follows: 

(a) Using the arbitrage theorem, write down a three-equation system with two states that gives the arbitrage-free values of $S_{t}$ and $C_{t}$ .  
(b) Now plot a two-step binomial tree for $S_{t}$ . Suppose at every node of the tree the markets are arbitrage-free. How many three-equation systems similar to the preceding case could then be 

3. Consider a stock $S_{t}$ and a plain vanilla, at-the-money, put option written on this stock. The option expires at time $t+\Delta$ , where $\Delta$ denotes a small interval. At time t, there are only two possible ways the $S_{t}$ can move. It can either go up to $S_{t+\Delta}^{u}$ , or go down to $S_{t+\Delta}^{d}$ . Also available to traders is risk-free borrowing and lending at annual rate r. 

(e) Suppose a put option with strike price K = 125 is written on C. The option expires in period 2. What is its arbitrage-free price? 

CHAPTER 2 A Primer on the Arbitrage Theorem 

In fact, sometimes there are no equivalent results in discrete time. In this sense stochastic calculus offers a wider variety of tools to the financial analyst. For example, continuous time permits infinitesimal adjustments in portfolio weights. This way, replicating “nonlinear” assets with “simple” portfolios becomes possible. In order to replicate an option, the underlying 

At the outset, stochastic calculus may appear too abstract to be of any use to a practitioner. This first impression is not correct. Continuous time finance is both simpler and richer. Once a market participant gets some practice, it is easier to work with continuous-time tools than their discrete-time equivalents. 

Stochastic calculus is an internally consistent set of operational rules that are different from the tools of “standard” calculus in some fundamental 

The mathematics of derivative assets assumes that time passes continuously. As a result, new information is revealed continuously, and decision-makers may face instantaneous changes in random news. Hence, technical tools for pricing derivative products require ways of handling random variables over infinitesimal time intervals. The mathematics of such random variables is known as stochastic calculus. 

# Calculus in Deterministic and Stochastic Environments

tree has 5 steps.
(b) What would be the implied u and d?
(c) What is the implied "up" probability?
(d) Determine the tree for the stock price $S_{i}$ .
(e) Determine the tree for the call premium $C_{i}$ . 

(a) Determine an appropriate time interval $\Delta$ , such that the binomial time has $5$ steps 

7. Using the data in the previous question, you are now asked to approximate the current value of a European call option on the stock $S_{r}$ . The option has a strike price of 100, and a maturity of 200 days. 

What do the p and $\epsilon$ represent under these conditions?
(d) Is it possible to determine the value of p? 

$\mu = r + \text{risk premium}$ 

(c) Now suppose $\mu$ is given by: 

If the sets A and B are themselves collections of functions, then f transforms a function into another function, and is called an operator. Most readers will be familiar with the standard notion of functions. Fewer readers may have had exposure to random functions. 

Suppose A and B are two sets, and let f be a rule which associates to every element x of A, exactly one element y in $B^{3}$ . Such a rule is called a function or a mapping. In mathematical analysis, functions are denoted by 

In this section we review the major concepts of standard (deterministic) calculus. Even if the reader is familiar with elementary concepts of standard calculus discussed here, it may still be worthwhile to go over the examples in this section. The examples are devised to highlight exactly those points at which standard calculus will fail to be a good approximation when underlying variables are stochastic. 

- We would like to calculate the response of one variable to a (random) change in another variable. That is, we would like to be able to differentiate various functions of interest.
- We would like to calculate sums of random increments that are of 

$^{1}$ Unless, of course, the underlying state space is itself discrete. This would be the case when the underlying asset price can assume only a finite number of possible values in the future. $^{2}$ A binomial random variable can assume one of the two possible values, and it may be significantly easier to work with than, say, a random variable that may assume any one of an uncountable number of possible values. 

These are some reasons behind developing a new calculus. Before doing this, however, a review of standard calculus will be helpful. After all, although the rules of stochastic calculus are different, the reasons for developing such rules are the same as in standard calculus: 

A more technical advantage of stochastic calculus is that a complicated random variable can have a very simple structure in continuous time, once the attention is focused on infinitesimal intervals. For example, if the time period under consideration is denoted by dt, and if dt is “infinitesimal,” then asset prices may safely be assumed to have two likely movements: uptick or downtick. 

## 1.2 Modeling Random Behavior

Non-periods, here, the E for any previous period. Also, numerical methods used in pricing securities are costly in terms of computer time. Hence, the pace of activity may make the analyst choose coarser or finer time intervals depending on the level of volatility. Such approximations can best be accomplished using random variables defined over continuous time. The tools of stochastic calculus will be needed to define these models. 

calculus.
For example, the relevant “time interval” may be different on different trading days. During some days an analyst may face more volatile markets, in others less. Changing volatility may require changing the basic “observa-
tion period,” i.e., the $\Delta$ of the previous chapter. 

It may be argued that the manner in which information flows in financial markets is more consistent with stochastic calculus than with “standard calculus.” 

asset and risk-free borrowing may be used. Such an exact replication will be impossible in discrete time. $^{1}$ 

$$
1 + 1 + \frac {1}{2 !} + \frac {1}{3 !} + \dots + \frac {1}{n !} + \dots
$$

stochastic processes. With stochastic processes, x will represent time, and we often limit our attention to the set $x \geq 0$ . Note this fundamental point. Randomness of a stochastic process is in terms of the trajectory as a whole, rather than a particular value at a specific point in time. In other words, the random drawing is done from a collection of trajectories. Choosing the state of the world, w, determines the complete trajectory. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/40cb447d94e50b2033361ef144faa6745759108f2cf14988d2ff8f8f62a137e9.jpg)


When $x$ represents time, we can interpret $f(x, w_1)$ and $f(x, w_2)$ as two different trajectories that depend on different states of the world. Hence, if $w$ represents the underlying randomness, the function $f(x, w)$ can be called a random function. Another name for random functions is where the notation $R \times W$ implies that one has to "plug in" to $f(\cdot)$ two variables, one from the set $W$ , and the other from $R$ . The function $f(x, w)$ has the following property: Given a $w \in W$ , the $f(\cdot, w)$ becomes a function of $x$ only. Thus, for different values of $w \in W$ we get different functions of $x$ . Two such cases are shown in Figure 1. $f(x, w_1)$ and $f(x, w_2)$ are two functions of $x$ that differ because the second element $w$ is different. 

once the value of x is given, we get the element y. Often y is assumed to be a real number. Now consider the following significant alteration.
There is a set W, where $w \in W$ denotes a state of the world. The function f depends on $x \in R$ and on $w \in W$ : 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/ac15291f906f114a073201183a788b506945261ccd0ad70b675aa3b09499c955.jpg)


It can be shown that $f(t)$ is not of bounded variation. $^{5}$ That this is the case is shown in Figure 2. Note that as $t \to 0$ , f becomes excessively “irregular.” The concept of bounded variation will play an important role in our discussions later. One reason is the following: asset prices in continuous 

Thus, functions of bounded variation are not excessively “irregular.” In fact, any “smooth” function will be of bounded variation. $^{4}$ 

where the maximum is taken over all possible partitions of the interval $[0, T]$ . In this sense, $V_0$ is the maximum of all possible variations in $f(\cdot)$ , and it is finite. $V_0$ is the total variation of $f$ on $[0, T]$ . Roughly speaking, $V_0$ measures the length of the trajectory followed by $f(\cdot)$ as $t$ goes from 0 to $T$ . 

Clearly, for each partition of the interval $[0, T]$ , we can form such a sum. Given that uncountably many partitions are possible, the sum can assume uncountably many values. If these sums are bounded from above, the function $f(\cdot)$ is said to be of bounded variation. Thus, bounded variation implies 

A practitioner may sometimes work with the logarithm of asset prices. Note that while y is always positive, there is no such restriction on x. Hence, the logarithm of an asset price may extend from minus to plus infinity. 

3.2.2 The Logarithmic Function
The logarithmic function is defined as the inverse of the exponential function. Given 

$^{6}$ The reader should not confuse the mathematical operation of differentiation or taking a derivative with the term “derivative securities” used in finance. $^{7}$ Time is one of the few deterministic variables one can imagine. 

For making the ratio independent of the size of $\Delta$ , one pays a price. The derivative is defined for infinitesimal intervals. For larger intervals, the derivative becomes an approximation that deteriorates as $\Delta$ gets larger and larger. 

Why is a limit being taken in (23)? In defining the derivative, the limit has a practical use. It is taken to make the ratio in (23) independent of the size of $\Delta$ , the time interval that passes. 

The variable x can represent any real-life phenomenon. Suppose it represents time. $^{7}$ Then $\Delta$ would correspond to a finite time interval. The $f(x)$ would be the value of y at time x, and the $f(x+\Delta)$ would represent the value of y at time $x+\Delta$ . Hence, the numerator in (23) is the change in y during a time interval $\Delta$ . The ratio itself becomes the rate of change in y during the same interval. For example, if y is the price of a certain as-set at time x, the ratio in (23) would represent the rate at which the price changes during an interval $\Delta$ . 

using the chain rate. The derivative is a rate of change. But it is a rate of change for infinitesimal movements. We give a formal definition first. 

their derivative is a way of calculating how one variable responds to a change in another variable. For example, given a change in the price of the underlying asset, we may want to know how the market value of an option written on it may move. These types of derivatives are usually taken using the chain rule. 

The notion of the derivative $^{6}$ can be looked at in (at least) two different ways. First, the derivative is a way of dealing with the “smoothness” of functions. It is a way of defining rates of change of variables under consideration. In particular, if trajectories of asset prices are “too irregular,” then their derivative with respect to time may not exist.
Second, the derivative is a way of calculating how one variable responds 

4 Convergence and Limit 

Are these definitions an equivalent:
We will answer these questions later. However, convergence is clearly a very important concept in approximating a quantity that does not easily lend itself to direct calculation. For example, we may want to define the notion of integral as the limit of a sequence. 

Very far non all $A$ even if $n \geqslant N$ . Secondly, since one can define different measures of "closeness," we should in principle be able to define convergence in different ways as well. Are these definitions all equivalent? 

In words, $x_{n}$ converges to $x^{*}$ if $x_{n}$ stays arbitrarily close to the point $x^{*}$ after a finite number of steps. Two important questions can be asked. Can we deal with convergence of $x_{n}$ if these were random variables instead of deterministic numbers? This question is relevant, since a random number $x_{n}$ can conceivably assume an extreme value and suddenly may fall very far from any $x^{*}$ even if $n > N$ . 

DEFINITION: We say that a sequence of real numbers $x_{n}$ converges to $x^{*} < \infty$ if for arbitrary $\epsilon > 0$ , there exists a $N < \infty$ such that 

of $x_{n}$ . The notion of convergence of a sequence has to do with the "eventual" value of $x_{n}$ as $n\to \infty$ . In the case where $x_{n}$ represents real numbers, we can state this more formally: 

where $x_{n}$ represents an object that changes as n is increased. This “object” can be a sequence of numbers, a sequence of functions, or a sequence of operations. The essential point is that we are observing successive versions of x. 

time will have some unpredictable part. No matter how finely we slice the time interval, they will still be partially unpredictable. But this means that trajectories of asset prices will have to be very irregular.
As will be seen later, continuous-time processes that we use to represent asset prices have trajectories with unbounded variation. 

$^{8}$ If x represents time, and if x is the “present,” then $f(x + \Delta)$ will belong to the “future.” However, $f(x), f_{x}$ , and $\Delta$ are all quantities that relate to the “present.” In this sense, they can be used for obtaining a crude “prediction” of $f(x + \Delta)$ in real time. This prediction requires having a numerical value for $f_{x}$ , the value of the derivative at the point x. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/7bd196a8e9690c59ea4ab0c235c94c30dabc5eac3032c23f91b9b65a8a018daa.jpg)


When we add the product $f_{x}\Delta$ to $f(x)$ we obtain the point C. This point can be taken as an approximation of B. Whether this will be a “good” or a “bad” approximation depends on the size of $\Delta$ and on the shape of the function $f(\cdot)$ . 

This equality means that the value assumed by $f(\cdot)$ at point $x + \Delta$ , can be approximated by the value of $f(\cdot)$ at point x, plus the derivative $f_{x}$ multiplied by $\Delta$ . Note that when one does not know the exact value of $f(x + \Delta)$ , the knowledge of $f(x)$ , $f_{x}$ , and $\Delta$ is sufficient to obtain an approximation. $^{8}$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/e4996283643f05b00f9c1d0edb4cf9c0957c17bfb74f93d306349ac747ed965c.jpg)


$^{9}$ As time passes, the expiration date of a contract comes closer, and even if the underlying asset's price remains constant, the price of the call option will fall. 

Hence, there is a chain effect. Time passes, new (small) events occur, the price of the underlying asset changes, and this affects the derivative asset's price. In standard calculus, the tool used to analyze these sorts of chain effects is known as the "chain rule." 

In pricing derivative securities, we face a somewhat different problem. The price of a derivative asset, e.g., a call option, will depend on the price of the underlying asset, and the price of the underlying asset depends on time. $^{9}$ 

The second use of the derivative is the chain rule. In the examples discussed earlier, $f(x)$ was a function of x, and x was assumed to represent time. The derivative was introduced as the response of a variable to a variation in time. 

likely to fail, but even a satisfactory definition of $f_{x}$ may not be obtained. Take, for example, the point $x_{0}$ . What is the rate of change of the function $f(x)$ at the point $x_{0}$ ? It is difficult to answer. Indeed, one can draw many tangents with differing slopes to $f(x)$ at that particular point. It appears that the function $f(x)$ is not differentiable. 

4.1.3 Example: High Variation
Consider Figure 7, where the function $f(x)$ is continuous, but exhibits extreme variations even in small intervals $\Delta$ . Here, not only is the prediction 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/d8cdfd47914d91ae0de8071f94a19e830f5ce042196e58650d99e3304a046113.jpg)


may end up being a very unsatisfactory approximation to the true $f(x+\Delta)$ . Clearly, the more “irregular” the function $f(\cdot)$ becomes, the more such approximations are likely to fail. Consider an extreme case in the next example. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/bd848186edf0896b5c51226ab912a42c502a09cabc2ebed3b332c7aa498d8fff.jpg)


which corresponds to the area shown in Figure 8. In order to calculate the Riemann integral, we partition the interval $[0,T]$ into $n$ disjoint subintervals 

4.3.1 The Riemann Integral
We are given a deterministic function $f(t)$ of time $t \in [0, T]$ . Suppose we are interested in integrating this function over an interval $[0, T]$ 

The general approach in defining integrals is, in a sense, obvious. One would begin with an approximation involving a countable number of objects, and then take some limit and move into uncountable objects. Given that different types of limits may be taken, the integral can be defined in various ways. In standard calculus the most common form is the Riemann integral. A somewhat more general integral defined similarly is the Riemann–Stieltjes integral. In this section we will review these definitions. 

4.3 The Integral
The integral is the mathematical tool used for calculating sums. In contrast to the $\Sigma$ operator, which is used for sums of a countable number of objects, integrals denote sums of uncountably infinite objects. Since it is not clear how one could “sum” objects that are not even countable, a formal definition of integral has to be derived. 

equivalent to the chain rule and that approximate the laws of motion of random variables in continuous time. The purpose of stochastic calculus is the same as that of standard calculus. The rules, though, are different. 

$^{19}$ Of course, there is always the question of whether the markets are correctly pricing the security at that instant. 

The answer to the first question is no. The chain rule formula given in (33) cannot be used in a continuous-time stochastic environment. In fact, by “stochastic calculus,” we mean a set of methods that yield the formulas 

In the example just given, $f(x)$ was a function of $x_{t}$ , and $x_{t}$ was a deterministic variable. There was no randomness associated with $x_{t}$ . What would happen if $x_{t}$ is random, or if the function $f(\cdot)$ depends on some random variable $z_{t}$ as well? In other words, 

valuable to changes in other variables.
Take the case of derivative asset prices. A trader observes the price of the underlying asset continuously and wants to know how the valuation of the complex derivative products written on this asset would change. If the derivative is an exchange-traded product, these changes can be observed from the markets directly. $^{10}$ However, if the derivative is a “structured” product, its valuation needs to be calculated in-house, using theoretical pricing models. These pricing models will use some tool such as the “chain rule” shown in (33). 

According to this, the chain rule is the product of two derivatives. First, the derivative of $f(g(t))$ is taken with respect to $g(t)$ . Second, the derivative of $g(t)$ is taken with respect to $t$ . The final effect of $t$ on $y_t$ is then equal to the product of these two expressions. 

Suppose in the example just given x was not itself the time, but a deterministic function of time, denoted by the symbol $t \geq 0$ : 

It turns out that a similar conclusion cannot be reached in stochastic environments. Suppose $f(W_{t})$ is a function of a random variable $W_{t}$ and that we are interested in calculating 

would the integral be different? To answer this question, consider Figure 10. Note that as the partitions get finer and finer, rectangles defined either way would eventually approximate the same area. Hence, at the limit, the approximation by rectangles would not give a different integral even when one uses different heights for defining the rectangles. 

under the curve were constructed in a particular way. To do this, we used the value of $f(t)$ evaluated at the midpoint of the intervals $t_i - t_{i-1}$ . Would the same approximation be valid if the rectangles were defined in a different fashion? For example, if one defined the rectangles either by 

A counterexample is shown in Figure 9. Here, the function $f(t)$ shows steep variations. If such variations do not smooth out as the base of the rectangles gets smaller, the approximation by rectangles may fail. We have one more comment that will be important in dealing with the Ito integral later in the text. The rectangles used to approximate the area 

rectangles will be available, and the area can be better approximated. Obviously, the condition that $f(t)$ should be smooth plays an important role during this process. In fact, a very "irregular" path followed by $f(t)$ may be much more difficult to approximate by this method. Using the terminology discussed before, in order for this method to work, the function $f(t)$ must be Riemann-integrable. 

In case the sum of the rectangles fails to approximate the area under the curve, we may be able to correct this by considering a finer partition. As the $|t_i - t_{i-1}|$ 's get smaller, the base of the rectangles will get smaller. More rectangles will be available, and the area can be better approximated. 

The term on the left-hand side of (37) involves adding the areas of $n$ rectangles constructed using $(t_i - t_{i-1})$ as the base and $f((t_i + t_{i-1})/2)$ as the height. Figure 8 displays this construction. Note that the small area $A$ is approximately equal to the area $B$ . This is especially true if the base of the rectangles is small and if the function $f(t)$ is smooth—that is, does not vary heavily in small intervals. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/cf530dc4b42cb7ac875bd99ae5141b08f0e0e6f97a636a161f32dde4b13ee942.jpg)


The answer to these questions is, in general, no. It turns out that in stochastic environments the functions to be integrated may vary too much for a straightforward extension of the Riemann integral to the stochastic case. A new definition of integral will be needed. 

However, before coming to such a conclusion, note that all the discussion thus far involved deterministic functions of time. Would the same definitions be valid in a stochastic environment? Can we use the same rectangles to approximate integrals in random environments? Would the choice of the rectangle make a difference? 

The Riemann-Stieltjes integral is useful when the integration is with respect to increments in $f(x)$ rather than the $x$ itself. Clearly, in dealing with financial derivatives, this is often the case. The price of the derivative asset depends on the underlying asset's price, which in turn depends on time. Hence, it may appear that the Riemann-Stieltjes integral is a more appropriate tool for dealing with derivative asset prices. 

This definition is not very different from that of the Riemann integral. In fact, similar approximating sums are used in both cases. If $x$ represents time $t$ , the Stieltjes integral over a partitioned interval, $[0, T]$ , is given by 

(Note that according to the notation used here, the derivative $f_{x}(x)$ is a function of $x$ as well.) Now suppose we want to integrate a function $h(x)$ with respect to $x$ : 

$^{11}$ Note that $(W_{t_{i}} - W_{t_{i-1}})$ and $W_{t_{i}}$ are correlated. 

4.3.2 The Stieltjes Integral
The Stieltjes integral is a different definition of the integral. Define the differential df as a small variation in the function $f(x)$ due to an infinitesimal variation in x: 

Finally, we would like to emphasize an important result. Note that when $f(\cdot)$ depends on a random variable, the resulting integral itself will be a random variable. In this sense, we will be dealing with random integrals. 

Information set.
On the other hand, the same conditional expectation of the term in (41) will, in general, be nonzero. $^{11}$ Clearly, in stochastic calculus, expressions that utilize different definitions of approximating rectangles may lead to different results. 

To see the reason behind this fundamental point, consider the case where $W_{t}$ is a martingale. Then the expectation of the term in (42), conditional on information at time $t_{t-1}$ , will vanish. This will be the case because, by definition, future increments of a martingale will be unrelated to the current information set. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/d855e60ee21915f744de402a80a14a667b078423ba2f747df4af2a1688669fc0.jpg)


where $h_{t}(t)$ and $f_{t}(t)$ are the derivatives of the corresponding functions with respect to time. They are themselves functions of time t.
In the notation of the Stieltjes integral, this transformation means that an expression that involves an integral 

The Riemann–Stieltjes approximating sums measure the area under the rectangle exactly, with no need to augment the number of approximating rectangles. 

(63) 

In other words, we take the total change in $S_{t}$ and multiply it by the partial derivative $f_{s}$ . We take the total change in time $dt$ and multiply it by the partial derivative $f_{t}$ . The total change in $f(\cdot)$ is the sum of these two products. According to this, total differentiation is calculated by splitting an observed change into different abstract components. 

Suppose we observe a small change in the price of a call option at time t. Let this total change be denoted by the differential $dC_{t}$ . How much of this variation is due to a change in the underlying asset's price? How much of the variation is the result of the expiration date getting nearer as time passes? Total differentiation is used to answer such questions.
Let $f(S_{t}, t)$ be a function of the two variables. Then the total differential is defined as 

Here $\partial S_{t}$ is an abstract increment in $S_{t}$ and does not imply a similar actual change in reality. In fact, the partial derivative $F_{s}$ is simply how much the function $F(\cdot)$ would have changed if we changed the $S_{t}$ by one unit. The $F_{s}$ is just a multiplier. 

in total differentiations.
Before dealing with total differentiation, we have one last comment on partial derivatives. Because the latter do not represent “observed” changes, there is no difference between their use in stochastic or deterministic environments. We do not have to develop a new theory of partial differentiation in stochastic environments.
To make this clearer consider the following example. 

price in financial markets. However, partial derivatives are very useful as in-
termediary tools. They are useful in taking a total change and then splitting
it into components that come from different sources, and they are useful
in total differentiations.
Before dealing with total differentiation we have one last comment on 

5 Partial Derivatives 

Because of this abstract nature of partial derivatives, this type of differentiation cannot be used directly in representing actual changes of asset 

Note that even though $S_{t}$ is a function of time, we are acting as if it does not change. Again, this shows the abstract character of the partial derivative. As $t$ changes, $S_{t}$ will change as well. But in taking partial derivatives, we behave as if it is a constant. 

would represent the (theoretical) effect of a change in the price of the underlying asset when time is kept fixed. This effect is an abstraction, because in practice one needs some time to pass before $S_{t}$ can change.
The partial derivative with respect to time variable can be defined similarly as 

Consider a call option. Time to expiration affects the price (premium) of the call in two different ways. First, as time passes, the expiration date will approach, and the remaining life of the option gets shorter. This lowers the premium. But at the same time, as time passes, the price of the underlying asset will change. This will also affect the premium. Hence, the price of a call is a function of two variables. It is more appropriate to write 

The stochastic version of this transformation is very useful in evaluating Ito integrals. In fact, imagine that $f(\cdot)$ is random while $h(\cdot)$ is (conditionally) a deterministic function of time. Then, using integration by parts, we can express stochastic integrals as a function of integrals with respect to a deterministic variable. In stochastic calculus, this important role will be played by Ito's formula. 

The convention in calculus is that, in general, terms of order $(dx)^{2}$ or higher are assumed to be negligible if x is a deterministic variable. $^{14}$ Thus, if we assume that x is deterministic, and let $(x - x_{0})$ be small, then we could use the first-order Taylor series approximation: 

This point is quite relevant for the later discussion of stochastic calculus. In fact, in order to prepare the groundwork for Ito's Lemma, we would like to consider a specific example. 

Under these conditions, we may want to drop some of the terms on the right-hand side of (64) if we can argue that they are negligible. To do this, we must adopt a “convention” for smallness and then eliminate all terms that are “negligible” according to this criterion. But when is a term small enough to be negligible? 

We are not going to elaborate on why the expansion in (64) is valid if $f(x)$ is continuous and smooth enough. Taylor series expansion is taken for granted. We will, however, discuss some of its implications. First, note that at this point the expression in (64) is not an approximation. The right-hand side involves an infinite series. Each element involves "simple" powers of $x$ only, but there are an infinite number of such elements. Because of this, Taylor series expansion is not very useful in practice. Yet, the expansion in (64) can be used to obtain useful approximations. Suppose we consider Equation (64) and only look at those $x$ near $x_0$ . That is, suppose 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/07faed6cedb5963c6f2473cb03b973ce7a00c705edd1c46fa5e9b5e71edc47f8.jpg)


This expression provides a second-order Taylor series expansion for the percentage rate of change in the value of a zero coupon bond as r changes 

Note that the difference between the first-order and second-order Taylor series approximations hinges on the size of the term $(t - t_0)^2$ . As $t$ nears $t_0$ , this terms becomes smaller. More importantly, it becomes smaller faster than the term $(t - t_0)$ . 

The right-hand side of this equation is a parabola that touches the exponential curve at point A. Because of the curvature of the parabola near $t_0$ , we expect this curve to be nearer the exponential function. Note that the difference between the first-order and second-order Taylor 

(76) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/3f9f86090120da5082be15005a14f5f6a941d4babe676258d3a5e02794ec8eef.jpg)


Figure 12 displays this approximation. The equation is represented by a convex curve that increases as $t \to T$ . The first-order Taylor series approximation is shown as a straight line tangent to the curve at point A. Note that as we go away from $t_0$ in either direction, the line becomes a worse approximation of the exponential curve. At $t$ near $t_0$ , on the other hand, the approximation is quite close. 

where the first term on the right-hand side is $B_{i}$ evaluated at $t = t_0$ . The second term on the right-hand side is the first derivative of $B_{i}$ with respect to $t$ , evaluated at $t_0$ , times the increment $t - t_0$ . 

We are interested in the Taylor series approximation of $B_{t}$ with respect to $t$ , assuming that $r, T$ remain constant. A first-order Taylor series expansion around $t = t_0$ will be given by 

This function begins at t = 0 with a value of $B_{0} = 100e^{-rT}$ . Then it increases at a constant percentage rate r. As $t \rightarrow T$ , the value of $B_{t}$ approaches 100. Hence, $B_{t}$ could be visualized as the value, as of time t, of 100 to be paid at time T. It is the present value of a default-free zero-coupon bond that matures at time T, and r is the corresponding continuously compounding yield to maturity. 

5.3.2 Example: Duration and Convexity
Consider the exponential function where t denotes time, T is fixed, r > 0, and $t \in [0, T]$ : 

Stochastic calculus is an attempt to perform similar operations when the underlying phenomena are continuous-time random processes. It turns out that in such an environment, the usual definitions of derivative, integral, and Taylor series approximations do not apply. In order to understand stochastic versions of such concepts, one first has to understand their deterministic equivalents. 

This chapter reviewed basic notions in calculus. Most of these concepts were elementary. While the notions of derivative, integral, and Taylor series may all be well known, it is important to review them for later purposes. 

(48) 

6 Conclusions 

(83) 

(82) 

The other important concept of the chapter was the notion of “smallness.” In particular, we need a convention to decide when an increment is small enough to be ignored. 

(85) 

Readers will recognize this as the valuation function for a zero-coupon bond. This example shows that the pricing functions for fixed income securities can be characterized as solutions of some appropriate differential equations. In stochastic settings, we will obtain more complex versions of this result. 

infinitesimally. The right-hand side measures the percentage rate of change in the bond price as r changes by $r - r_{0}$ , where $r_{0}$ can be interpreted as the current rate. We see two terms containing $r - r_{0}$ on the right-hand side. In financial markets the coefficient of the first term is called the modified duration. The second term is positive and has a coefficient of $1/2(T - t)^{2}$ . It represents the so-called convexity of the bond. Overall, the second-order Taylor series expansion of $B_{t}$ with respect to r shows that, as interest rates increase (decrease), the value of the bond decreases (increases). The “convexity” of the bond implies that the bigger these changes, the smaller their relative effects. 

the unknown element is a vector. Under appropriate conditions, the solution would be $x = A^{-1}b$ —i.e., the inverse of A multiplied by the vector b. 

solves the ODE in (77) in that plugging it into (79) satisfies the equality (77). Thus, an ordinary differential equation is first of all an equation. That is, it is an equality where there exist one or more unknowns that need to be determined. 

This expression states that $B_{t}$ is a quantity that varies with $t$ -i.e., changes in $B_{t}$ are a function of $t$ and of $B_{t}$ . The equation is called an ordinary differential equation. Here, the percentage variation in $B_{t}$ is proportional to some factor $r_{t}$ times $dt$ : 

The third major notion from standard calculus that we would like to review is the concept of an ordinary differential equation (ODE). For example, consider the expression 

This chapter provides examples of how to determine such pricing functions $F(S_t, t)$ for linear and nonlinear derivatives. These concepts are 

The second pricing method that utilizes arbitrage takes a somewhat more direct approach. One first constructs a risk-free portfolio, and then obtains a partial differential equation (PDE) that is implied by the lack of arbitrage opportunities. This PDE is either solved analytically or evaluated numerically. In either case, the problem of pricing derivatives is to find a function $F(S_{t}, t)$ that relates the price of the derivative product to $S_{p}$ , the price of the underlying asset, and possibly to some other market risk factors. When a closed-form formula is impossible to determine, one finds numerical ways to describe the dynamics of $F(S_{t}, t)$ . This chapter provides examples of how to $V_{t}$ is 

There exist specific ways to obtain such formulas. One method was discussed in Chapter 2. The notion of arbitrage can be used to determine a probability measure under which financial assets behave as martingales, once discounted properly. The tools of martingale arithmetic become available, and one can easily calculate arbitrage-free prices, by evaluating the implied expectations. This approach to pricing derivatives is called the method of equivalent martingale measures. 

There are some aspects of pricing derivative instruments that set them apart from the general theory of asset valuation. Under simplifying assumptions, one can express the arbitrage-free price of a derivative as a function of some “basic” securities, and then obtain a set of formulas that can be used to price the asset without having to consider any linkages to other financial markets or to the real side of the economy. 

## 1 Introduction

# Pricing Derivatives

Take the partials with respect to $x, y, z$ , respectively. 

$f(x,z,y) = \frac{x + y + z}{(1 + x)(1 + z)(1 + y)}$ 

10. Consider the following functions: 

(c) How do these sums approximate the true integral?
(d) Why? 

$\sum_{i=1}^{4} f(x_{i-1})(x_i - x_{i-1})$ . 

$\sum_{i=1}^{4} f(x_i)(x_i - x_{i-1})$ 

by choosing the $x_{i}$ numerically. Calculate the following sums: 

(b) Again, split the interval $[0,1]$ into 4 pieces, $x_0 = 0 < x_1 < x_2 < x_3 < x_4 = 1$ , $\begin{array}{r}f(x) = \left\{ \begin{array}{ll}x(\sin (\frac{\pi}{x})) & 0 < x \leq 1\\ 0 & x = 0. \end{array} \right. \end{array}$ 

9. Now consider the function $f(x)$ discussed in this chapter: 

(c) What are the differences between these two sums and do they approximate the true value of the integral? 

$^{4}$ Behind this statement there are assumptions, such as zero default risk of the forward contract. 

$^{3}$ Note the sense in which this is a derivative contract. Once the contract is signed, it becomes a separate security and can be traded on its own. To trade the forward contract, one need not have in possession any physical gold. In fact, such instruments can be derived from “notional” underlying assets that do not even exist concretely. Derivatives written on equity indices are one such class. 

The function $F(S_t, t)$ in (3) is linear in $S_t$ . Thus, forward contracts are called linear products. Later we will derive the Black-Scholes formula which 

Thus we used the possibility of exploiting any arbitrage opportunities and obtained an equality that expresses the price of a forward contract $F(S_{t}, t)$ as a function of $S_{t}$ , $t$ and other parameters. In fact, we determined a function $F(S_{t}, t)$ that gives the value of the forward contract at any time $t$ . Of the arguments in $F(S_{t}, t)$ , $S_{t}$ and $t$ are variables. They may change during the life of the contract. On the other hand, $c, r_{t}$ , and $T$ are parameters. It is assumed that they will remain constant during $T - t$ . The function $F(S_{t}, t)$ in (2) is linear in $g$ . Then $f_{t}$ is constant. 

$F(S_{t},t) = e^{r_{t}(T - t)}S_{t} + (T - t)c.$ 

Hence, the outcomes of the two sets of transactions are identical. $^{4}$ This means that they must cost the same; otherwise, there will be arbitrage opportunities. An astute player will enter two separate contracts, buying the cheaper gold and selling the expensive one simultaneously. Mathematically, this gives the equality 

The forward contract is another way of obtaining a unit of gold at time T. One signs a contract now for delivery of one unit of gold at time T, with the understanding that all payments will be made at expiration. 

This is one method of securing one unit of physical gold at time T. One borrows the necessary funds, buys the underlying commodity, and stores it until time T. 

where the first term is the principal and interest to be returned to the bank at time T, and the second represents total storage and insurance costs paid at time T. 

$e^{r_{i}(T - t)}S_{t} + (T - t)c,$ 

62 

Use an average $c$ Suppose one buys one unit of physical gold at time $t$ for $S_{t}$ dollars using funds borrowed at the continuously compounding risk-free rate $r_{t}$ . The $r_{t}$ is assumed to be fixed during the contract period. Let the insurance and storage costs per time unit be $c$ dollars and let them be paid at time $T$ . The total cost of holding this gold during a period of length $T - t$ will be given by 

of such a contract at time t in terms of the underlying parameters?³ We use an arbitrage argument. 

$^{1}$ The nonexistence of a closed-form formula does not necessarily imply the nonexistence of a pricing function. It may simply mean that we are not able to express the pricing function in terms of a simple formula. For example, all continuous and “smooth” functions can be expanded as an infinite Taylor series expansion. At the same time, truncating Taylor series in order to obtain a closed-form formula would in general lead to an approximation error. 

Hence, we have a contract that imposes an obligation on both counterparties—the one that delivers the gold, and the one that accepts the delivery. How can one determine a function $F(S_t, t)$ that gives the fair market value 

F dollars will be paid for one unit of gold.
• The contract is signed at time t, but no payment changes hands until time T. 

Consider the class of cash-and-carry goods. $^{2}$ Here we show how a pricing function $F(S_{t}, t)$ , where $S_{t}$ is the underlying asset, can be obtained for forward contracts. In particular, we consider a forward contract with the following provisions: 

to obtain an equation that governs the dynamics of $F(S_t, t)$ . In this section, we show examples of how to determine such $F(S_t, t)$ . The discussion is intended to introduce new mathematical tools and concepts that have common use in pricing derivative products. 

The unknown of a derivative pricing problem is a function $F(S_t, t)$ , where $S_t$ is the price of the underlying asset and $t$ is time. Ideally, the financial analyst will try to obtain a closed-form formula for $F(S_t, t)$ . The Black-Scholes formula that gives the price of a call option in terms of the underlying asset and some other relevant parameters is perhaps the best-known case. There are, however, many other examples, some considerably simpler. 

2 Pricing Functions 

clarified and an example of partial differential equation methods is given. This discussion provides some motivation for the fundamental tools of stochastic calculus that we introduce later. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/3d16cf019522129001229fb9e1fd3d87715fe1e45f69843c3edc3b978394a3ec.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/71218ff2a1b4e977eccd99bd2e64b2157c72d57e592f0077665dd2c997070430.jpg)


The part of this property can be made more explicit, consider Figure 1. To see how this property can be made more explicit, consider Figure 1. The lower part of this figure displays a payoff diagram for a short position in $S_{t}$ . A unit of the underlying asset, $S_{p}$ , is borrowed and sold at price $S$ . 

affecting the option's price. Hence, unpredictable movements in $S_{t}$ can be offset by opposite positions taken simultaneously in $C_{t}$ . This property imposes some conditions on the way $F(S_{t}, t)$ can change over time once the time path of $S_{t}$ is given. 

$^{5}$ The interest rate r is constant and, hence, is dropped as an argument of $F(\cdot)$ . 

$C_{t}=F(S_{t},t).$ The pricing function $F(S_{t},t)$ for options will have a fundamental property

Under simplifying conditions, the $S_{t}$ will be the only source of randomness. 

groundwork for further mathematical tools.
Suppose $C_{t}$ is a call option written on the stock $S_{t}$ . Let r be the constant risk-free rate. K is the strike price, and T, t < T, is the expiration date.
Then the price of the call option can be expressed as $^{5}$ 

Determining the pricing function $F(S_t, t)$ for nonlinear assets is not a easy as in the case of forward contracts. This will be done in later chapters. At this point, we only introduce an important property that the $F(S_t, t)$ should satisfy in the case of nonlinear products. This will prepare the groundwork for further mathematical tools. 

According to this, at expiration, the cash price of the underlying asset and the price of the forward contract will be equal. This is an example of a boundary condition. At the expiration date—i.e., at the boundary for time variable t—the pricing function $F(S_{t}, t)$ assumes a special value, $S_{T}$ . The boundary condition is known at time t, although the value that $S_{t}$ will assume at T is unknown. 

One question here is the presence of $r_t$ . In reality, this and $S_r$ are random variables, and one may ask if the use of a standard limit concept is valid. Ignoring this and applying the limit to the left-hand side of the expression in (3), we obtain 

2.1.1 Boundary Conditions
Here we have to mention briefly what a boundary condition is. Suppose we want to express formally the notion that the “expiration date gets nearer.” To do this, we use the concept of limits. We let 

provides a pricing function $F(S_t, t)$ for call options. This formula will be nonlinear in $S_t$ . Instruments that have optionlike characteristics are called nonlinear products. 

$^{6}$ It comes from the Black-Scholes formula that we prove later. $^{7}$ And of other possible parameters of the problem. 

The following by $r(\mathfrak{S},\mathfrak{r})$ : The following definition formalizes some of the concepts discussed in this section. 

where $g(t)$ is a completely predictable function of time $t^{7}$ . If we learn how to calculate such differentials, the equation above can be used in finding a closed-form formula for $F(S_{t}, t)$ . When such closed-form formulas do not exist, numerical methods can be used to trace the trajectories followed by $F(S_{t}, t)$ . The following definition formalizes some of the concepts discussed in 

Indicated by $\partial C_t$ . Clearly, if $dS_t$ is a small incremental change, then the $\partial C_t$ will be a very good approximation of the actual change $dC_t$ . As a result, the gain in the option position will (approximately) offset the loss in the short position. Such a portfolio will not move unpredictably. Thus, incremental movements in $F(S_t,t)$ and $S_t$ should be related by 

Now, suppose we are short by not one, but by $F_{s}$ units of the underlying stock. Then, as $S_{t}$ increases by $dS_{t}$ , the total loss on the short position will be $F_{s}dS_{t}$ . But according to Figure 1, this amount is very close to $dC_{t}$ . It is indicated by $\partial C_{t}$ . 

equal to $dS_{t}$ would lead to a net loss. But this reasoning suggests that with careful adjustments of positions, such losses could be eliminated. Consider the slope of the tangent to $F(S_{t}, t)$ at point A. This slope is given by 

However, we see a critical point. According to Figure 1, when $S_t$ increases by $dS_t$ , the price of the call option will increase only by $dC_t$ ; this latter change is smaller because the slope of the curve is less than one, i.e., 

Suppose, originally, the underlying asset's price is S. That is, initially we are at point A on the $F(S_{t}, t)$ curve. If the stock price increases by $dS_{t}$ , the short position will lose exactly the amount $dS_{t}$ . But the option position gains 

The first panel of Figure 1 displays the price $F(S_t, t)$ of a call option written on $S_t$ . At this point, we leave aside how the formula for $F(S_t, t)$ is obtained and graphed. $^6$ 

CHAPTER 4 Pricing Derivatives 

(14) 

The form of $F(x)$ is pinned down. However, the parameter $a$ is still unknown. It is found by using the so-called "boundary conditions." 

Thus, we are led to a problem where the unknown is a function. This argument shows that partial differential equations and their solutions are topics that need to be studied.
An example might be helpful at this point. 

3. Equation (11), called the total differential of $F(\cdot)$ , gives the change in derivative product's price in terms of changes in its determinants. Hence, one might think of an analyst who first obtains estimates of $dS_t$ and then uses the equation for the total differential to evaluate the $dF(S_t, t)$ . Equation (11) can be used once the partial derivatives $F_s, F_t$ are evaluated numerically. This, on the other hand, requires that the functional form of $F(S_t, t)$ be known. 

3 Application: Another Pricing Method 

1. Assume that an analyst observes the current price of a derivative product $F(S_{t}, t)$ and the underlying asset price $S_{t}$ in real time. Suppose the analyst would like to calculate the change in the derivative asset's price $dF(S_{t}, t)$ , given a change in the price of the underlying asset $dS_{t}$ .  
2. Here the notions that we introduced in Chapter 3 start to become useful. Remember that the concept of differentiation is a tool that one can use to approximate small changes in a function. In this particular case, we indeed have a function $F(\cdot)$ that depends on $S_{t}$ , $t$ . Thus, if we can use the standard calculus, we could write 

This book deals with the mathematics of derivative asset pricing. It is not a text on asset pricing per se. However, a discussion of general methods of pricing derivative assets is unavoidable. This is needed to illustrate the type of mathematics that we intend to discuss and to provide examples. We use the discussion of the previous section to summarize the pricing method that uses partial differential equations (PDEs). 

Clearly, the assumption of continuous time plays implicitly a fundamental role in asset pricing. In fact, we were able to replicate the movements in the option position by infinitesimally adjusting our short position in the underlying asset. The ability to make such infinitesimal adjustments in the portfolio clearly hinges on the assumption of continuous time and the absence of transaction costs. As shown earlier, with "large" increments, such approximations will deteriorate quickly. 

$^{10}$ This would make the expression a Taylor series approximation. $^{11}$ For that matter, it may not be true for the cross-product term, $(dS_{i}dt_{i})$ , either. $^{12}$ In infinitesimal intervals, we will see that the mean square limits of these terms are deterministic and proportional to dt. 

First, it is maintained that $(dS_{t})^{2}$ and $(dr_{t})^{2}$ are random during small intervals. $^{12}$ Thus, they have nonzero variances during dt. 

Now, dt is a small deterministic change in t. So to say that $(dt)^{2}$ , $(dt)^{3}$ , ... are “small” with respect to dt is an internally consistent statement. However, the same argument cannot be used for $(dS_{t})^{2}$ , and, possibly, for $(dt_{t})^{2.11}$ . 

depends on the assumption that the terms $(dt)^{2}$ , $(dS_{t})^{2}$ , and $(dr_{t})^{2}$ , and those of higher order, are “small” enough that they can be omitted from a multivariate Taylor series expansion. $^{10}$ Because of such an approximation, higher powers of the differentials $dS_{t}$ , dt, or $dr_{t}$ do not show up on the right-hand side of (23). 

we still do not know how arbitrage can be used to eliminate terms such as $d_{t}$ , $dF(t)$ , $dS_{t}$ , and $d r_{t}$ . We leave this aside for the time being. 

In standard calculus, variables under consideration are deterministic. Hence, to get a relation such as 

The answer to this question is no. It turns out that one needs a "new" calculus and a different formula when the variables under consideration are random processes. The following is a first look at some of these difficulties. 

## 4 The Problem

Remember that in the case of derivative products, one generally has some information about the form of $F(\cdot)$ at the expiration date. Such information can sometimes be used to determine the function $F(\cdot)$ explicitly, given a PDE. 

Note that the random event behind this bct is the same as in R. Now consider the following: 

2. Now place yourself exactly in the same setting as before, where the market quotes the above R. It just happens that you have a close friend who offers you the following separate bet, $R^{*}$ : 

You can take either side of the bet. Let the true probability of the incumbent winning be denoted by $p, 0 < p < 1$ . 

1. Suppose you can bet on an American presidential election in which one of the candidates is an incumbent. The market offers you the following payoffs R: 

valuation formulas. Cox and Rubinstein (1985) is a very good example. Finally, most of the valuation theory can be found in the excellent collection of papers in Merton (1990). There are also some recent sources that give a broad summary of valuation theory. Björk (1999), Nielsen (1999), and Kwok (1998) are three such books. 

Duffie (1996) is an excellent source on dynamic asset valuation. Ingersoll (1987) also provides a very good treatment. There are, however, several less complicated books to consider for an understanding of simple asset 

## 5 References

conditions, determine the parameters of the mathematical problems. This chapter also introduced the fundamental mathematical problems faced in continuous-time finance. Standard formulas from calculus are not applicable when the variables under consideration are continuous-time stochastic processes. Increments of these processes have nonzero variances. This will make the average “size” of the second-order terms such as $dS_{t}^{2}$ nonnegligible. 

If the notion of differential needs to be changed, then that notion of the integral should also be reformulated. In fact, in such a stochastic environment, we define differentials by using a new definition of integral. Otherwise, in continuous-time stochastic environments, a formal definition of derivative does not exist. 

This is an example of why we need to study “stochastic calculus.” We want to learn how to exploit the chain rule in a stochastic environment and understand what a differential means in such a setting. The example above shows that the resulting expressions would be different from the ones obtained in deterministic calculus. 

This poses a problem. On one hand, we want to use continuous-time random processes with nonzero variances during dt. So, we use positive numbers for the average values of $(dS_{t})^{2}$ and $(dr_{t})^{2}$ . But under these conditions, it would be inconsistent to call $(dS_{t})^{2}$ and $(dr_{t})^{2}$ “small” with respect to dt, and then equate them to zero, a step that can be taken if the variables in question are deterministic, as in the case of standard calculus.

Hence, in a stochastic environment with a continuous flow of randomness, we have to write the relevant total differentials as: 

$^{1}$ For example, prices can move up and down by some preset amounts. 

Derivative products are contracts written on underlying assets whose prices fluctuate randomly. A mathematical model of randomness is thus needed. 

## 2 Probability

The second purpose of this chapter is to introduce the binomial process, which plays an important role in derivative asset valuation. Pricing models for derivative assets are formulated in continuous time, but will be applied in discrete, “small” time intervals. Practical methods of asset pricing using “finite difference methods” or lattice methods fall within this category. Prices of underlying assets are assumed to be observed at time periods separated by small finite intervals of length $\Delta$ . In such small intervals, it is further assumed, prices can have only a limited number of possible movements. $^{1}$ These methods all rely on the idea that a continuous-time stochastic process representing the price of the underlying asset can be approximated arbitrarily well by a binomial process. This chapter introduces the mechanics of justifying such approximations. 

In this chapter, we review some basic notions in probability theory. Our first purpose here is to prepare the groundwork for a discussion of martingales and martingale-related tools. In doing this, we discuss properties of random variables and stochastic processes. A reader with a good background in probability theory may want to skip these sections. 

1 Introduction 

## Tools in Probability Theory

unknown value?
(c) What role would a statistician or econometrician play in making all these decisions? Why? 

(b) Is the value of the probability p important in selecting this portfolio? Do you care what the p is? Suppose you are given the R, but the payoff of $R^{*}$ when the incumbent wins is an unknown to be determined. Can the above portfolio help you determine this 

CHAPTER 4 Pricing Derivatives 

where B is the set made of all possible subsets of the real numbers R. In terms of the example just discussed, note that a “favorable harvest report” may contain several judgmental statements besides some accompanying numbers. Let X be the value of the numerical estimate provided by the USDA and let 100 be some minimum desirable harvest. Then mappings such as 

In general, there is no reason for a probability to be representable by a simple mathematical formula. However, some convenient and simple mathematical models are found to be acceptable approximations for representing probabilities associated with financial data. $^{2}$ 

Finally, note that in this particular example the $\Omega$ is the set of all possible reports that the USDA may make public. 

Depending on what is in the report, we can call it either favorable or unfavorable. This constitutes an example of an event. Note that there may be several $\omega$ 's that may lead us to call the harvest report "favorable." It is in this sense that events are collections of $\omega$ 's. Hence, we may want to know the probability of a "favorable report." 

Suppose the price of an exchange-traded commodity future during a given day depends only on a harvest report the U.S. Department of Agriculture (USDA) will make public during that day.
The specifics of the report written by the USDA are equivalent to an $\omega$ . 

The first of these conditions implies that probabilities of events are either zero or positive. The second says that the probabilities should sum to one. Here, note the notation $dP(A)$ . This is a measure theoretic notation and may be read as the incremental probability associated with an event $A$ . The triplet $\{\Omega, \mathfrak{S}, P\}$ is called a probability space. According to this, a point $\omega$ of $\Omega$ is chosen randomly. $P(A)$ , where $A \in \mathfrak{S}$ , represents the probability that the chosen point belongs to the set $A$ . 

In working with random variables, one first defines a probability space. That is, one explicitly lays out the framework where the notion of chance and the resulting probability can be defined without falling into some inconsistencies. 

This can be a bit surprising, given that many investors appear to be driven by "intuitive" notions of probabilities rather than by an axiomatic and formal probabilistic model. However, the discussion in Chapter 2 indicated that no matter what the "true" probabilities are, if there are no arbitrage opportunities, one can represent the fair market value of financial assets using probability measures constructed "synthetically." Hence, regardless of any subjective chances perceived by market participants, mathematical probability models have a natural use in pricing derivative products. 

Some elementary models of probability theory are especially well suited to pricing derivative assets. 

Consider the nonsymmetric density shown in Figure 2. If the mean is the center of gravity and standard deviation is a rough measure of the width of the distribution, then one would need another parameter to characterize the skewness of the distribution. Third moments are indeed informative about such asymmetries. 

In fact, all higher-order moments of normally distributed random variables can be expressed as functions of $\mu$ and $\sigma^{2}$ . In other words, given the first two moments, higher-order moments of normally distributed variables do not provide any additional information. 

A normally distributed random variable X would also have higher-order moments. For example, the centered third moment of any normally distributed random variable X will be given by 

Integrals of this formula determine the probabilities associated with various values that the random variable x can assume. Note that $f(x)$ depends on only two parameters, $\sigma^{2}$ and $\mu$ . Hence, the probabilities associated with a normally distributed random variable can be inferred if one has the sample estimates of these two moments. 

where the variance parameter $\sigma^2$ is the second moment around the mean and the parameter $\mu$ is the first moment. Figure 1 shows examples of normal distributions. 

## [f(x)=\frac{1}{\sqrt{2\pi\sigma^{2}}}e^{-\frac{1}{2\sigma^{2}}(x-\mu)^{2}},]

where $f(x)$ is the corresponding probability density function. $^{4}$ The variance $E[X - E[X]]^{2}$ is the second moment around the mean. The first moment of a random variable is the “center of gravity” of the distribution, while the second moment gives information about the way the distribution is spread out. The square root of the second moment is the standard deviation. It is a measure of the average deviation of observations from the mean. In financial markets, the standard deviation of a price change is called the volatility. For example, in the case of a normally distributed random variable X, the density function is given by the well-known formula $^{4}$ If the density does not exist, we replace $f(x)dx$ by $dF(x)$ . 

3.1 First Two Moments
The expected value $E[X]$ of a random variable X, with density $f(x)$ , is called the first moment. It is defined by 

There are different ways one can classify models of distribution functions. One classification uses the notion of "moments." Some random variables can be fully characterized by their first two moments. Others need higher-order moments for a full characterization. 

## 3 Moments

These examples are specially constructed so as to facilitate understanding of more complicated asset pricing methods to be discussed later. But first we need to review the notions of expectations and conditional expectations. 

It can be shown that under some technical conditions there always exists a distribution function $G(x)$ . However, whether this function $G(x)$ can be written as a convenient formula is a different question. It turns out that there are some well-known models where this is possible. We review three basic probability models that are frequently used in pricing derivative products. 

When the function $G(x)$ is smooth and has a derivative, we can define the density function of $X$ . This function is denoted by $g(x)$ and is obtained by $dG(x)$ . 

CHAPTER·5 Tools in Probability Theory (10) 

$^{5}$ An operator is a function that maps functions into functions. That is, it takes as input a function and produces as output another function. 

This is the probability that the x will fall in a small neighborhood of $x_{0}$ . The neighborhood is characterized by the “distance” dx. These quantities are shown in Figure 3. Note that although $f(x)$ is a nonlinear curve in this figure, for small dx it can be approximated reasonably well by a straight line. Then, the rectangle in Figure 3 would be 

First, the probability density functions need to be discussed further. If X is a random variable with density function $f(x)$ , and if $x_{0}$ is one possible value of this random variable, then for small dx, we have 

where $t_i$ , $i = 0,1,\ldots$ are times when the information set becomes available. In the mathematical analysis, such information sets are called an increasing sequence of sigma fields. When such information sets become available continuously, a different term is used, and the family $I_t$ satisfying (9) is called a filtration. 

In general, the information used by decision makers will increase as time passes. If we also assume that the decision maker never forgets past data, the information sets must be increasing over time: 

The operation of taking expectations of random variables is the formal equivalent of the heuristic notion of “forecasting.” To forecast a random variable, one utilizes some information denoted by the symbol $I_{i}$ . Expectations calculated using such information are called conditional expectations. The corresponding mathematical operation is the “conditional expectation operator.” $^{5}$ Since the information utilized could be, and in general is, different from one time to another, the conditional expectation operator is itself indexed by the time index. 

4 Conditional Expectations 

In other words, a casual observer is more likely to be “surprised” by extreme observations in the case of heavy-tailed random variables. 

But there is more to heavy-tailed distributions than that. In a normal distribution, most of the observations would naturally be occurring around the center. More importantly, the occurrence of extremes is gradual, in that the passage from ordinary, to large, and then to extreme observations occurs in a gradual fashion. In case of a heavy-tailed distribution, on the other hand, the passage from “ordinary” to extreme observations is more sudden. The middle tail region of the distribution contains relatively less weight than in the normal density. Compared to the normal density, one is likely to get “too many extreme observations.” 

3.2.1 Heavy Tails
What is the meaning of heavy tails?
A distribution that has heavier tails than the normal curve means a higher probability of extreme observations. But this point should be carefully made. Note that the normal density also has tails that extend to plus and minus infinities. Thus, a normally distributed random variable could also assume extreme values from time to time. However, in the case of a heavy-tailed distribution, these extreme observations have, relatively speaking, a higher frequency. 

In financial markets, a more important notion is the phenomenon of heavy tails. Figure 2 displays a symmetric density which has another characteristic that differentiates it from normal distributions. The tails of this distribution are heavier relative to the middle part of the tails. Such densities are called heavy-tailed and are fairly common with financial data. Again, one would need a parameter other than variance and the mean to characterize the heavy-tailed distributions. Fourth moments are used for that end. 

A nonsymmetric density (An F(5.3) distribution) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/1a49192954bfd46e26a33870e03ea1f13dd6c8d881c88d4310f448c81cb54c69.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/53100539df603a9711bf3e487ea462d0b3a272cdecae7d143bd9483660715b36.jpg)


⑤ 

Finally, if the conditioning information set $I_{t}$ is empty, then one obtains the “unconditional” expectation operator E. This means that E has properties similar to the conditional expectation operator. 

According to this, recursive application of conditional expectation operators always equals the conditional expectation with respect to the smaller information set: 

$E[E[|I_{t}||I_{o}] = E[|I_{0}],$ 

2. Suppose the most recent information set is $I_t$ , but one is interested in forecasting the expectation $E_{t + T}[S_{t + T + u}]$ , $T > 0, u > 0$ . That is, one would like to say something about the forecast of a possible forecast. Since the information set $I_{t + T}$ is unavailable at time $t$ , the conditional expectation $E_{t + T}[S_{t + T + u}]$ is unknown. In other words, $E_{t + T}[S_{t + T + u}]$ is itself a random variable. A property of conditional expectations is that the expectation of this future expectation equals the present forecast of $S_{t + T + u}$ : 

The t subscript in $E_{t}$ indicates that in the averaging operation one uses all information available up to time t.
The conditional expectation operator $E_{t}$ has the following properties. 

In this expression, the right-hand side should be read as follows: for a given t, the sum of all possible values that $S_{t}$ might assume are weighted by the corresponding probabilities $[f(S_{t}|I_{u})dS_{t}]$ and summed. The averaging is done by using probabilities conditional on $I_{u}$ . This way, any information that one has gets incorporated in the forecast. 

4 Conditional Expectations 

4.1.1 Conditional Expectation Operator
The second step in defining a conditional expectation is the “averaging” operator. In fact, every forecast is an average of possible future values. The values that the random variable can assume in the future are weighted by the probabilities associated with these values, and an average is obtained.
Hence, the operation of conditional expectation involves calculating a weighted sum. Since the possible outcomes are likely to be not only infinite, but also uncountably many, this sum is represented by an integral.
The conditional expectation (forecast) of some random variable S, given the information available at time u is given by 

Consider a simple example. The odds of a stock market crash will be an example of unconditional probability. The odds of a crash given that one has entered a severe recession can be represented by a conditional probability. In this particular case the information is the knowledge that a severe recession has begun. The use of such information may certainly lead to a revision of the (unconditional) probability of a crash. 

close to the probability that $x$ will fall within a small neighborhood of $x_0$ represented by the quantity $dx$ . If these probabilities are based on some information set $I_t$ , then $f(x)$ is called a conditional density. The dependence on $I_t$ is formally denoted by $f(x|I_t)$ . If the $f(x)$ is not based on any particular information, the $I_t$ term is dropped and the density is written as $f(x)$ . 

Finally, consider the following question. At the limit, the infinitesimal changes $dF(t)$ are still very erratic. Would the trajectories of $F(t)$ be of bounded variation? $^{7}$ The question is important, because otherwise, the Riemann-Stieltjes way of constructing integrals cannot be exploited and a new definition of integral would be needed. 

That is, beginning from an initial price $F(t_{0})$ , we obtain the price at time t by simply adding all subsequent infinitesimal changes. Clearly, in continuous time, there are an uncountable number of such infinitesimal changes—hence the use of integral notation. Also, at the limit, the notation for “small” incremental changes $\Delta F(t)$ is replaced by $dF(t)$ , which represents infinitesimal changes. 

come nearer, and second, $|a\sqrt{\Delta}|$ gets smaller. The $\Delta F(t)$ is the increment in the price process. What kind of a path is followed by $F(t)$ itself? First, note that if $F(t)$ represents the price of a derivative product at time $t$ , then it will equal the sum of all up- and downticks since $t_0$ . As $\Delta \to 0$ , $F(t)$ will be given by 

One important question is the following: what does a typical path followed by the $\Delta F(t)$ look like? Clearly, such a trajectory will be made of a sequence of $+a\sqrt{\Delta}$ and $-a\sqrt{\Delta}$ 's. If the probability of each of these outcomes is exactly equal to 1/2, then a realization of $\{\Delta F(t), t = t_0, t_0 + \Delta, \ldots\}$ will, as $\Delta$ gets smaller, converge to an extremely erratic trajectory that fluctuates between $+a\sqrt{\Delta}$ and $-a\sqrt{\Delta}$ . 

An important element of the discussion involving the binomial process $\Delta F(t)$ is that the two possible values assumed by each $\Delta F(t)$ depend on the parameter $\Delta$ . This dependence permits a discussion of the limiting behavior of the binomial process. We can ask a number of questions that will eventually relate to pricing derivative products. 

Note that these assumptions are somewhat artificial for actual markets. On a given trading day, even in markets with very high turnover, there are many time periods where $\Delta F(t)$ does not change. Or, in some special circumstances, it may change by more than an up or downtick. However, such complications will be dealt with later. For the time being, we consider the simpler case of binomial processes. 

5 Some Important Models 

At each time point a new $F(t)$ is observed. Each increment $\Delta F(t)$ will equal either $+a\sqrt{\Delta}$ or $-a\sqrt{\Delta}$ . If the $\Delta F(t)$ are independent of each other, the sequence of increments $\Delta F(t)$ will be called a binomial stochastic process, or simply a binomial process. $^{6}$ 

where $\Delta F(t)$ represents the change in the observed price during the “small” time interval $\Delta$ . 

The price $F(t)$ changes continuously over time, but the trader is assumed to have limited scope of attention and checks the market price every $\Delta$ seconds. We assume that $\Delta$ is a small time interval. More importantly, we assume that at any time $t$ there are two possibilities: 

Consider a trader who follows the price of an exchange-traded derivative asset $F(t)$ in real time, using a service such as Reuters, Telerate, or Bloomberg. 

5.1 Binomial Distribution in Financial Markets 

This section discusses some important models for random variables. These models are useful not only in theory, but also in practical applications of asset pricing. In this section we also extend the notion of a random variable to a random process. 

Beginning from $t_0 = 0$ , in the immediate futurc, $F(t)$ has only two possible values: 

Now consider the following experiment with the random variable $F(t)$ discussed in the previous section. We ask the computer to calculate many realizations of $F(t)$ . Then, beginning from the same initial point $F(0)$ , we plot these trajectories. 

These observations imply that for small intervals $\Delta$ , higher-order moments of a binomial random variable that assumes values proportional to $\sqrt{\Delta}$ can be ignored. 

As $\Delta \to 0$ , the fourth-order moment will become negligible. It is proportional to a power of $\Delta$ that goes to zero faster than the time interval itself. 

small $\Delta$ . This last point is also relevant for higher-order moments of the binomial process. Again assume that $p = .5$ for simplicity. Then the expected value is zero and the third moment will be given by to $\Delta^2$ will be approximately constant in infinitesimal time intervals. Figure 4 illustrates the difference between a variance proportional to $\Delta^2$ (the $45^{\circ}$ line) and one proportional to $\Delta^2$ . The latter becomes negligible for small $\Delta$ . 

In contrast, if $\Delta F(t)$ had instead fluctuated between, say, $+a\Delta$ and $-a\Delta$ the variance would be proportional to $\Delta^2$ . For "small" $\Delta$ , the value of $\Delta^2$ would be much smaller. When $\Delta \to 0$ , the variance would go to zero significantly faster. Under such conditions, it can be maintained without any contradiction that the variance of $\Delta F(t)$ is negligible, while $\Delta$ itself is not. Heuristically speaking, a random variable with a variance proportional 

and the expected value will equal 0 while the variance is given by $a^2\Delta$ . It is important to realize that the variance of the binomial process is proportional to $\Delta$ . As $\Delta$ approaches zero, a variance that is proportional to $\Delta$ will go toward zero with the same speed. This means that if we think of $\Delta$ as a small but nonnegligible quantity, then the variance will also be nonnegligible. 

process. Let $t$ be fixed. Then the expected value and the variance of $\Delta F(t)$ are defined as follows: 

Another important point is the following: the integral in (21) is taken with respect to a random process, and not with respect to a deterministic variable as is the case in standard calculus. Clearly, this integral is itself a random variable. Can such an integral be successfully defined? Can we use the Riemann-Stieltjes procedure of approximations by appropriate rectangles to construct an integral with respect to a random process? These questions lead to the Ito integral and will be answered in Chapter 9. 

(35) 

It is the notion of weak convergence that describes the way distributions of whole sequences of random variables converge. 

The corresponding distribution function does not have a closed-form formula. It can only be represented as an integral.
The convergence in distribution is illustrated in Figure 5. It is important for practical asset pricing to realize the meaning of this convergence in distribution. We observe a sequence of random variables indexed by n. $^{10}$ As n increases, the distribution function of the $n$ th random variable starts to resemble the normal distribution. $^{11}$ It is the option of $n$ . 

(34) 

Then, for fixed $\Delta$ and "large" $n$ , the distribution of $F(n\Delta)$ can be approximated by a normal distribution with mean 0 and variance $a^2 n\Delta$ . The approximating density function will be given by 

According to the central limit theorem, the distribution of $F(n\Delta)$ approaches the normal distribution as $n\Delta \to \infty$ . Assume that $p = .5$ and that 

Now, remember that at the origin $F(t)$ was binomial, but a little farther away the number of possible outcomes grew and it became multinomial. The probability distribution also changed accordingly. How does the form of the distribution change as $n \to \infty$ ? What would it look like at the limit? Questions such as these fall in the domain of "convergence of random variables." There are two different ways one can investigate this issue. The first approach is that of the central limit theorem. The second is called weak 

One question is what happens to the distribution of the random variable $F(n\Delta)$ as $n\to \infty$ and $\Delta$ remains fixed? A somewhat different question is what happens to the distribution of $F(n\Delta)$ as $\Delta \rightarrow 0$ while $n\Delta$ is fixed. Now, remember that at the origin $F(t)$ was binomial, but a little farther 

105 

in which $\Delta$ was constant and $n \rightarrow \infty$ , the time period under consideration increased indefinitely, and we looked at a limiting $F(t)$ projected toward a “distant” future. 

5 Some Important Models 

$^{8}$ In fact, this latter type of convergence is of interest to us. These types of experiments fall in the domain of weak convergence and give us an approximate distribution for a whole sequence of random variables observed during an interval. 

There are several other possibilities. In fact, we can consider the general case and try to find the total number of possible values $F(n\Delta)$ can take. Obviously, as $n \to \infty$ , $F(n\Delta)$ may take any of a possibly infinite number of values. A similar conclusion can be reached if $\Delta \to 0$ and $n \to \infty$ while the product $\Delta n$ remains constant. In this case, we are considering a fixed time interval and subdividing it into finer and finer partitions. For the case 

are two different sequences of price changes, each resulting in the same price at time $t = 5\Delta$ . 

That is, $F(2\Delta)$ may equal $F(0) + 2a\sqrt{\Delta}$ , $F(0) - 2a\sqrt{\Delta}$ , or $F(0)$ . Of these, the last outcome is most likely if there is a 50–50 chance of an uptick. Now consider possible values of $F(t)$ once some more time elapses. Several more combinations of upticks and downticks become possible. For example, by the time $t = 5\Delta$ , one possible but extreme outcome may be 

$F(2\Delta) = \left\{ \begin{array}{ll}F(0) + a\sqrt{\Delta} +a\sqrt{\Delta} & \text{with probability} p^{2}\\ F(0) - a\sqrt{\Delta} +a\sqrt{\Delta} & \text{with probability} 2p(1 - p)\\ F(0) - a\sqrt{\Delta} -a\sqrt{\Delta} & \text{with probability} (1 - p)^{2}. \end{array} \right.$ (28) 

But if we let some more time pass, and then look at $F(t)$ at, say, $t = 2\Delta$ , $F(t)$ will assume one of three possible values. More precisely, we have the following possibilities: 

(38) 

107 

Hence, during a small interval, there is a “high” probability that no jump will occur. Thus, the trajectory of a Poisson process will consist of a continuous path broken by occasional jumps. 

$^{12}$ Both of these assumptions can be altered. However, to keep the Poisson characteristic, the jump times need to be independent. 

where $\lambda$ is a positive constant called the intensity. Note the contrast with normal distribution. For a normally distributed variable, the probability of obtaining a value exactly equal to zero is nil. Yet with the Poisson distribution, if $\Delta$ is “small,” this probability is approximately 

(36) 

(37) 

This implies that the Gaussian model is useful when new information arriving during infinitesimal periods is itself infinitesimal. As illustrated for the binomial approximation, with $\Delta \rightarrow 0$ , the values assumed by $\Delta F(t)$ become smaller and smaller and the variance of new information given by 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/ade5bdf56a0ffbf4a720f3bde8a808d71f540b200f55d6604fd2c238a2327c5c.jpg)


Continuous-time versions of the normal distribution are very useful in asset pricing. Under some conditions, however, they may not be sufficient to approximate trajectories of asset prices observed in some financial markets. We may need a model for prices that show "jumps" as well. There were many examples of such "jumps" during the October 1987 crash of stock markets around the world. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/51ab651f0b423cc5d1a5ee5550f091c94022509deb6de372695d218ee9e56512.jpg)


How can we represent such phenomena?
The Poisson distribution is the second building block. A Poisson-distributed random process consists of jumps at unpredictable occurrence times $t_{i}, i = 1, 2, \ldots$ . The jump times are assumed to be independent of one another, and each jump is assumed to be of the same size. $^{12}$ Further, during a small time interval $\Delta$ , the probability of observing more than one jump is negligible. The total number of jumps observed up to time t is called a Poisson counting process and is denoted by $N_{t}$ .
For a Poisson process, the probability of a jump during a small interval $\Delta$ will be approximated by 

In dealing with continuous-time stochastic processes, we need two building blocks. One is the continuous-time equivalent of the normal distribution known as Brownian motion or, equivalently, as the Wiener process. As the discussion in the previous section indicates, trajectories of these processes are likely to be continuous. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/c7ba156314b53503e85f9d1c2b0e740db488ffaa1317354cf96be0cc9dd3391c.jpg)


(44) 

$^{14}$ We are not talking about the dependence of means or variances of $X_{t+1}$ only. The more distant past should not influence statements concerning the whole probabilistic behavior of a Markov process. 

$dr_{t} = \mu (r_{t}, t)dt + \sigma (r_{t}, t)dW_{t}$ . 

(43) 

These steps will be discussed in more detail when we develop the notion of stochastic differential equations in Chapter 11. There, letting $\Delta \to 0$ , we obtain a standard stochastic differential equation for $r_t$ and write it as 

(42) 

$\sigma (I_t,t) = \sigma (r_t,t).$ 

It turns out that if $r_{i}$ is a Markov process, and if $I_{i}$ contains only the current and past values of $r_{i}$ , then the conditional mean and variance will be functions of $r_{i}$ only and we can write: 

where the $\Delta W_{t}$ is some unpredictable random variable with variance $\Delta$ . Then, the $\sigma(I_t, t) \sqrt{\Delta}$ will be the standard deviation of interest rate increments. The first term on the right-hand side will represent expected change in interest rate movements, and the second term will represent the part that is unpredictable given $I_t$ . 

(41) 

How do these notions help a market practitioner?
Suppose the $X_{t}$ represents a variable such as instantaneous spot rate $r_{t}$ . Then, assuming that $r_{t}$ is Markov means that the (expected) future behavior of $r_{t+s}$ depends only on the latest observation and that a condition such as (40) will be valid. We can then proceed as follows.
We split changes in interest rates into expected and unexpected compo-

The assumption of Markovness has more than just theoretical relevance in asset pricing. In heuristic terms, and in discrete time $t = 1, 2, \ldots$ , a Markov process, $\{X_{t}\}$ , is a sequence of random variables such that knowledge of its past is totally irrelevant for any statement concerning the $X_{t+s}, 0 < s$ , given the last observed value, $x_{t}$ . In other words, any probability statement about some future $X_{t+s}, 0 < s$ , will depend only on the latest observation $x_{t}$ and on nothing observed earlier. $^{14}$ 

109 

6 Markov Processes and Their Relevance 

$^{13}$ It is quite important that the process one is modeling in finance is a Markov process. The Feynman-Kac theorem that we will see in later chapters will be valid only for such processes. Yet, it can be shown that short-term interest rate processes are, in general, not Markov. This imposes limitations on the numerical methods that can be applied for short rate processes. 

where $0 < s$ and $P(\cdot | I_i)$ is the probability conditional on the information set $I_i$ . 

DEFINITION: A discrete time process, $\{X_{1},\ldots,X_{i},\ldots\}$ , with joint probability distribution function, $F(x_{1},\ldots,x_{i})$ , is said to be a Markov process if the implied conditional probabilities satisfy 

In this section, we discuss in detail a class of stochastic processes that plays an important role in derivative asset pricing; namely, the Markov processes. Our discussion, which will be in discrete time, will try to motivate some important aspects of stochastic processes and will also clarify some notions that will be used later in dealing with continuous time models for interest rate derivatives. $^{13}$ as $t \to \infty$ . In case the index $t$ is continuous, one is dealing with uncountably many random variables and clearly the joint distribution function of such a process should be carefully “constructed” as will be illustrated for Wiener Process. 

Sequences of random variables $\{X_{t}\}$ indexed by an index $t$ , where $t$ is either discrete, $t = 0,1,\dots$ , or continuous, $t\in [0,\infty)$ , are called stochastic processes. A stochastic process is assumed to have a well-defined joint distribution function, 

The discussion thus far has dealt basically with random variables. Yet, this concept is too simple to be useful in finance, although, it does constitute a building block for more complex models. In finance, what we really need is a model of a sequence of random variables, and often those that are observed over continuous time. 

$P(\Delta N_{i} = n) = \frac{e^{-\lambda\Delta}(\lambda\Delta)^{n}}{n!},$ 

The probability that during a finite interval $\Delta$ there will be $n$ jumps is given by $^{16}$ Here the $W_{i}$ do not represent Wiener processes. They are any independent, identically distributed random variables with no dependence on a past. 

By itself, it does not satisfy the assumption of Markovness. Obviously, the reverse is also true. Any non-Markov process in a univariate world can be converted into a Markov process by increasing the 

Obviously, such an $r_t$ process cannot be Markov. For one, a forecast of the $r_{t+\Delta} - r_t$ would depend on $r_s, s < t$ in addition to the last observed $r_t$ . Hence, a univariate dynamic that assumes Markovian behavior for the short rate, $r_p$ , will not represent interest rate dynamics correctly, although the joint behavior or the short and long rates is Markov by assumption. 

In order to obtain a univariate model, consider the equation implied by the first row: 

Clearly, this is a special case. But, it is sufficient to make the point. We derive a univariate model for $r_t$ implied by the Markovian system in (45). This derivation is of interest itself, because the recursive method utilized here is a standard tool in solving difference equations in other contexts as 

to System (45), current short and long rates depend only on the latest observations of $r_t$ and $R_{t}^{16}$ . Clearly, this is a special case. But it is sufficient to make the next $W$ . 

$^{15}$ Also, if interest rates are not Markov, a very important correspondence between a class of partial differential equations (PDE) and a class of conditional expectations cannot be published. Monte Carlo methods cease to become equivalent to the PDE's commonly used the field of interest rate derivatives. 

where $W_{t + \Delta}^{1}, W_{t + \Delta}^{2}$ are two error terms independent of each other, and of the past $W_{s}^{1}, W_{s}^{2}, s \leq t$ . The $\{\beta_i; \alpha_i, \sigma_i\}$ are constant coefficients. According 

$\left[ \begin{array}{c}r_{t + \Delta}\\ R_{t + \Delta} \end{array} \right] = \left[ \begin{array}{c}\alpha_{1}r_{t} + \beta_{1}R_{t}\\ \alpha_{2}r_{t} + \beta_{2}R_{t} \end{array} \right] + \left[ \begin{array}{c}\sigma_{1}W_{t + \Delta}^{1}\\ \sigma_{2}W_{t + \Delta}^{2} \end{array} \right],$ 

short-rate based approach.
Suppose we have a bivariate process, $[r_{t}, R_{t}]$ , where the $r_{t}$ represents the “short” rate and the $R_{t}$ is the “long” rate. Suppose also that jointly the are Markov: 

The relevance of this can best be discussed in fixed-income. There (and elsewhere) a central concept is the yield curve. The so-called classical approach, attempts to model yield curve using a single interest rate process such as the $r_i$ discussed above. On the other hand, the more recent Health Jarrow-Merton (HJM) approach, consistent with Black-Scholes philosophy models it using $k$ separate forward rates, which are assumed to be Markov jointly. But as we will see below, the univariate dynamics of one element of a $k$ -dimensional Markov process will, in general, not be Markov. Hence Markovness can be maintained in HJM methodology, but may fail in short-rate based approach. 

6.2 The Vector Case 

But, if interest rates were not Markov, these steps cannot be followed, since the conditional mean and variance of the spot rate could potentially depend on observations other than the immediate past. $^{15}$ Hence, the assumption of Markovness appears to be quite relevant in pricing derivatives, at least in case of interest rate derivatives. 

With such a model, one can then proceed to parameterize the $\mu(r_t, t)$ and $\sigma(r_t, t)$ and hence obtain a model that captures the dynamics of interest rates. 

(57) 

But there is a fundamental difference. The sum $X_{n}$ now involves random processes. Hence, in taking a limit of (56), a new type of convergence criterion should be used. The standard definition of limit from calculus is not applicable.
Which (random) convergence criterion should be used? 

Note that $X_{n}$ is similar to a Riemann-Stieltjes sum. It is as if an inter-val $[t_0, T]$ is partitioned into $n$ subintervals and the $X_{n}$ is defined as an approximation to 

(56) 

Here $[S_{t_0 + (i + 1)\Delta} - S_{t_0 + i\Delta}]$ represents the increment in the asset price at time $t_0 + i\Delta$ . The observations begin at time $t_0$ and are recorded every $\Delta$ minutes. 

7.1.2 Example
Let $S_{i}$ be an asset price observed at equidistant time points: 

(54) 

This definition is a natural extension of the limiting operation used in standard calculus. It says that as n goes to infinity, the difference between the two random variables becomes negligibly small. In the case of mean square convergence, it was the variance that converged to zero. Now, it is the difference between $X_{n}$ and X. In the limit, the two random variables are almost the same. 

DEFINITION: A random variable $X_{n}$ converges to X almost surely (a.s.) if, for arbitrary $\delta > 0$ , 

7.1.1 Relevance of Mean Square Convergence
Mean square (m.s.) convergence is important because the Ito integral is defined as the mean square limit of a certain sum. If one uses other definitions of convergence, this limit may not exist.
We would like to discuss this important point further. Consider a more “natural” extension of the notion of limit used in standard calculus. 

will have a smaller and smaller variance as n goes to infinity.
Note that for finite n, the variance of $\epsilon_{n}$ may be small, but not necessary.
zero. This has an important implication. In doing numerical calculations
one may have to take such approximation errors into account explicitly
One way of doing this is to use the standard deviation of $\epsilon_{n}$ as an estimate 

DEFINITION: Let $X_0, X_1, \ldots, X_n, \ldots$ be a sequence of random variables. Then $X_n$ is said to converge to $X$ in mean square if 

criteria are used. The first is mean square convergence. This is a criterion utilized to define the Ito integral. The latter is utilized in characterizing stochastic differentials equations (SDEs). As a result, mean square convergence plays a fundamental role in numerical calculations involving SDEs. 

The notion of convergence has several uses in asset pricing. Some of these are theoretical, others practical. The binomial example of the previous section introduced the notion of convergence as a way of approximating a complicated random variable with a simpler model. As $\Delta \to 0$ , the approximation improved. In this section, we provide a more systematic treatment of these issues. Again, the discussion here should be considered a brief and heuristic introduction. 

dimensionality of the problem. This suggests that one can assume that forward rates are Markov, yet at the same time assuming Markovness for spot rates could, in general, be inaccurate. This point will play an important role in modeling interest-sensitive securities. Within the context of yield curve dynamics, this point suggests working with k-dimensional Markov processes rather than non-Markovian univariate models. 

(62) 

According to this, $X_{i}(t)$ is either 0 or 1, depending on the $t$ and on the value assumed by $\epsilon_{i}$ . 

7.2.2 An Example

Consider a time interval [0, 1] and let $t \in [0, 1]$ represent a particular time. $^{18}$ Suppose we are given n observations $\epsilon_{i}, i = 1, 2, \ldots, n$ drawn independently from the uniform distribution $U(0, 1)$ . $^{19}$ Next define the random variables $X_{i}(t), i = 1, \ldots, n$ by 

(60) 

Thus, instead of being concerned with the exact future value of $S_{T}$ , we need to calculate the expectation of some function $F(\cdot)$ of $S_{T}$ . Using the concept of weak convergence, an approximation $S_{T}^{n}$ of $S_{T}$ can be utilized. This may be desirable if $S_{T}^{n}$ is more convenient to work with than the actual random variable $S_{T}$ . For example, $S_{T}$ may be a continuous-time random process, whereas $S_{T}^{n}$ may be a random sequence defined over small intervals that depend on some parameter n. If the work is done on computers, $S_{T}^{n}$ will be easier to work with than $S_{T}$ . This idea was utilized earlier in obtaining a binomial approximation to a continuous normally distributed process. 

random price
For example, $F(S_{T}, T)$ may denote the random price of a derivative product at expiration time T. The derivative is written on the underlying asset $S_{T}$ . We know that if there are no arbitrage opportunities, then there exists a “risk-neutral” probability $\tilde{P}$ , such that, under some simplifying assumptions, the value of the derivative at time t is given by 

115 

Hence, in defining an Ito integral, values assumed by a random variable are of fundamental interest, and mean square convergence needs to be 

7 Convergence of Random Variables $^{17}$ The same result applies if, in addition, $S_{t}$ displays occasional jumps. 

7.2.1 Relevance of Weak Convergence
We are often interested in values assumed by a random variable as some parameter n goes to infinity. For example, to define an Ito integral, a random variable with a simple structure is first constructed. This random variable will depend on some parameter n. In the second step, one shows the as $n \rightarrow \infty$ , this simple variable converges to the Ito integral in the m-sense. 

According to this definition, a random variable $X_{n}$ converges to $X$ weak if functions of the two random variables have expectations that are close enough. Thus, $X_{n}$ and $X$ do not necessarily assume values that are very close, yet they are governed by arbitrarily close probabilities as $n \to \infty$ . 

where $f(\cdot)$ is any bounded, continuous, real-valued function; $E^{P_{n}}[f(X_{n})]$ is the expectation of a function of $X_{n}$ under probability distribution $P_{n}$ ; $E^{P}[f(X)]$ is the expectation of a function of X under probability distribution P. 

DEFINITION: Let $X_{n}$ be a random variable indexed by $n$ with probability distribution $P_{n}$ . We say that $X_{n}$ converges to $X$ weakly and 

In the case of weak convergence (the third kind of convergence), what is being approximated is not the value of a random variable $X_{n}$ , but the probability associated with a sequence $X_0, \ldots, X_n$ . Weak convergence is used in approximating the distribution function of families of random variables. 

The notion of m.s. convergence is used to find approximations to values assumed by random variables. As some parameter n goes to infinity, values assumed by some random variable $X_{n}$ can be approximated by values of some limiting random variable X. 

It turns out that if $S_{t}$ is a Wiener process, then $X_{n}$ will not converge almost surely, $^{17}$ but a mean square limit will exist. Hence, the type of approximation one uses will make a difference. This important point is taken up during the discussion of the Ito integral in later chapters. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/a0d9cd04879fe29525fc6d80f4f8b7528b1a5cbca4167dd0c6a364ace0552d22.jpg)


2. We let the random variable $X_{n}$ be a binomial process, 

(a) What are the marginal distributions of $X$ and $Y$ ?  
(b) Are $X$ and $Y$ independent?  
(c) Calculate $E[X]$ and $E[Y]$ .  
(d) Calculate the conditional distribution $P[X|Y = 1]$ .  
(e) Obtain the conditional expectation $E[X|Y = 1]$ and the conditional variance $Var[X|Y = 1]$ . 

1. You are given two discrete random variables X, Y that assume the possible values 0, 1 according to the following joint distribution: 

In the remainder of this book, we do not require any further results on probability than what is reviewed here. However, a financial market participant or a finance student will always benefit from a good understanding of the theory of stochastic processes. An excellent introduction is Ross (1993). Liptser and Shirayev (1977) is an excellent advanced introduction. Cinlar (1978) is another source for the intermediate level. The book by Brzezniak and Zastawniak (1999) is a good source for introductory stochastic processes. See also the new book by Ross (1999). 

Second, we discussed an important binomial process. This example was used to introduce the important notion of convergence of stochastic processes. The binomial example discussed here also happens to have practical implications, since it is very similar to the binomial tree-models routinely used in pricing financial assets. 

This chapter briefly reviewed some basic concepts of probability theory. We spent a minimal amount of time on the standard definitions of probability. However, we made a number of important points. First, we characterized normally distributed random variables and Poisson processes as two basic building blocks. 

## 8 Conclusions

Figure 6 displays this construction for n = 7. Note that $S_{n}(t)$ is a piecewise continuous function with jumps at $\epsilon_{i}$ . As $n \to \infty$ , the jump points become more frequent and the “oscillations” of $S_{n}(t)$ more pronounced. The sizes of the jumps, however, will diminish at the limit $n \to \infty$ , $S_{n}(t)$ will be very close to a normally distributed random variable for each t. Interestingly, the process will be continuous at the limit, the initial and the endpoints being identically equal to zero. $^{20}$ Clearly, what happens here is that as $n \to \infty$ , the $S_{n}(t)$ starts to behave more and more like a normally distributed process. For large n, we may find a limiting Gaussian process more convenient to work with than $S_{n}(t)$ . It should also be emphasized that in this example, as n increases, the number of points at which $S_{n}(t)$ changes will increase. In applications where we go from small discrete intervals toward continuous-time analysis, this would often be the case. 

is informal, since $dS_{i}$ is only a symbolic expression, as we will see in the definition of the Ito integral. 

$E[dS_{i}] = 0$ 

where $\Delta$ is a “small” interval, is well defined. Yet, writing 

$E[S_{t + \Delta} - S_t] = 0,$ 

To denote a small interval, we use the symbols h or $\Delta$ . An infinitesimal interval, on the other hand, is denoted by dt. In later chapters, we show that these notations are not equivalent. An operation such as 

We begin with a comment on notation. In this chapter, we use the notation $\Delta W_{t}$ or $\Delta S_{t}$ to represent “small” changes in $W_{t}$ or $S_{t}$ . Occasionally, we may also use their incremental versions $dW_{t}, dS_{t}$ , which represent stochastic changes during infinitesimal intervals. For the time being, the reader can interpret these differentials as “infinitesimal” stochastic changes observed over a continuous time axis. These concepts will be formally defined in Chapter 9. 

Martingales are one of the central tools in the modern theory of finance. In this chapter we introduce the basics of martingale theory. However, this theory is vast, and we only emphasize those aspects that are directly relevant to pricing financial derivatives. 

# Martingales and Martingale Representations

to show that 

(e) Calculate the mean and the variance of S. 

3. We say that $Z$ is exponentially distributed with parameter $\lambda > 0$ if the distribution function of $Z$ is given by: 

(a) Calculate the probabilities $P(X_4 > k)$ for $k = 0, 1, 2, 4$ and plot the distribution function.  
(b) Calculate the expected value and the variance of $X_n$ for $n = 3$ . 

$B_{i} = \left\{ \begin{array}{ll}1 & \text{with probability } p\\ 0 & \text{with probability } 1 - p. \end{array} \right.$ 

i.e., the best forecast of the change in $S_f$ over an arbitrary interval $u > 0$ is zero. In other words, the directions of the future movements in martin-gales are impossible to forecast. This is the fundamental characteristic of 

But $E_{t}[S_{t}]$ is a forecast of a random variable whose value is already “revealed” [since $S(t)$ is by definition $I_{t}$ -adapted]. Hence, it equals $S_{t}$ . If $S_{t}$ is a martingale, $E_{t}[S_{t + u}]$ would also equal $S_{t}$ . This gives 

According to this definition, martingales are random variables whose future variations are completely unpredictable given the current information set. For example, suppose $S_{t}$ is a martingale and consider the forecast of the change in $S_{t}$ over an interval of length u > 0: 

Here, all expectations $E[\cdot]$ , $E_{i}[\cdot]$ are assumed to be taken with respect to the probability $P$ . 

1. $S_{t}$ is known, given $I_{t}$ . ( $S_{t}$ is $I_{t}$ -adapted.)
2. Unconditional “forecasts” are finite: 

DEFINITION: We say that a process $\{S_t, t \in [0, \infty]\}$ is a martingale with respect to the family of information sets $I_t$ and with respect to the probability $P$ , if, for all $t > 0$ , 

is the formal way of denoting the forecast of a future value, $S_T$ of $S_t$ , using the information available as of time $t$ . $E_u[S_T]$ , $u < t$ , would denote the forecast of the same variable using a smaller information set as of or earlier than time $u$ . 

Using different information sets, one can conceivably generate different “forecasts” of a process $\{S_{t}\}$ . These forecasts are expressed using conditional expectations. In particular, 

$^{1}$ Depending on the problem at hand, the $I_{t}$ will represent different types of information. The most natural use of $I_{t}$ will be to represent the information one can obtain from the realized prices in financial markets up to time t. 

represent various time periods over a continuous time interval [0, T]. Not the way the initial value and the endpoint of the interval are handled in this notation. The symbol $t_0$ is assigned to the initial point, whereas $t_k$ the "new" symbol for T. In this notation, as $k \to \infty$ , and $(t_i - t_{i-1}) \to$ the interval [0, T] would be partitioned into finer and finer pieces. Now consider the random price process $S_t$ during the finite intervals [0, T]. At some particular time $t_i$ , the value of the price process will be $S_{t_i}$ . If the value of $S_t$ is included in the information set $I_t$ at each $t \geq 0$ , then it is said that $\{S_t, t \in [0, T]\}$ is adapted to $\{I_t, t \in [0, T]\}$ . That is, the value $S_t$ will be known, given the information set $I_t$ . We can now define continuous-time martingales. 

The set $\{I_t, t \in [0, T]\}$ is called a filtration. In discussing martingale theory (and throughout the rest of this book) we occasionally need to consider values assumed by some stochastic process at particular points in time. This is often accomplished by selecting sequence $\{t_i\}$ such that 

## $I_{s}\subseteq I_{t}\subseteq I_{T}\dots$

Suppose we observe a family of random variables indexed by time index $t$ . We assume that time is continuous and deal with continuous-time stochastic processes. Let the observed process be denoted by $\{S_t, t \in [0, \infty]\}$ . Let $\{I_t, t \in [0, \infty]\}$ represent a family of information sets that become continuously available to the decision maker as time passes. With $s < t < T$ , this family of information sets will satisfy 

## 2.1 Notation

Martingale theory classifies observed time series according to the way they "trend." A stochastic process behaves like a martingale if its trajectories display no discernible trends or periodicities. A process that, on the average increases is called a submartingale. The term supermartingale represents processes that, on the average, decline. This section gives formal definitions of these concepts. First, some notation. 

If this second methodology is selected to convert arbitrary processes into martingales, then the transformation is done using the Girsanov theorem. In 

(13) 

and the $e^{-r}S_{t}$ becomes a martingale. Probability distributions that convert equations such as (12) into equalities such as (13) are called equivalent martingale measures. They will be treated in Chapter 14. 

where $E_{t}^{P}[\cdot]$ is the conditional expectation calculated using a probability distribution P, we may try to find an “equivalent” probability $\hat{P}$ , such that the new expectations satisfy 

This methodology is equivalent to using the so-called representation results for martingales. In fact, Doob-Meyer decomposition implies that, under some general conditions, an arbitrary continuous-time process can be decomposed into a martingale and an increasing (or decreasing) process. Elimination of the latter leaves the martingale to work with. Doob-Meyer decomposition is handled in this chapter. 

The first method should be obvious. We can subtract an expected trend from $e^{-rt}S_{t}$ or $e^{-rt}B_{t}$ . This would make the deviations around the trend completely unpredictable. Hence, the “transformed” variables would be martingales. 

for stock prices, can be very useful in pricing derivative securities. One important question that we study in later chapters is how to obtain this conversion. There are in fact two ways of converting submartingales into martingales. 

(11) 

(10) 

It turns out that although most financial assets are not martingales, one can convert them into martingales. For example, one can find a probability distribution $\vec{P}$ such that bond or stock prices discounted by the risk-free rate become martingales. If this is done, equalities such as 

3 The Use of Martingales in Asset Pricing 

where $\mu$ is a positive rate of expected return. $^{3}$ A similar statement can be made about futures or options. For example, options have “time value,” and, as time passes, the price of European-style options will decline ceteris paribus. Such a process is a supermartingale. $^{4}$ 

Clearly, the price of a discount bond does not move like a martingale. Similarly, in general, a risky stock $S_{r}$ will have a positive expected return and will not be a martingale. For a small interval $\Delta_{r}$ , we can write 

According to the definition above, a process $S_{t}$ is a martingale if its future movements are completely unpredictable given a family of information sets. Now, we know that stock prices or bond prices are not completely unpredictable. The price of a discount bond is expected to increase over time. If general, the same is true for stock prices. They are expected to increase on the average. Hence, if $B_{t}$ represents the price of a discount bond maturing at time $T, t < T$ , 

## 3 The Use of Martingales in Asset Pricing

Before closing this section, we reemphasize a very important property of the definition of martingales. A martingale is always defined with respect to some information set, and with respect to some probability measure. If we change the information content and/or the probabilities associated with the process, the process under consideration may cease to be a martingale. The opposite is also true. Given a process $X_{t}$ that does not behave like a martingale, we may be able to modify the relevant probability measure $P_{t}$ and convert $X_{t}$ into a martingale. 

processes that behave as martingales. If the trajectories of a process display clearly recognizable long- or short-run “trends,” then the process is not a martingale. $^{2}$ 

Figure 2 displays an example of a right continuous martingale. Here, the trajectory is interrupted with occasional jumps.⁵ What makes the trajectory right continuous is the way jumps are modeled. At jump times $t_0$ , $t_1$ , $t_2$ , the martingale is continuous rightwards (but not leftwards.) 

As mentioned earlier, this equality implies that increments of a martingale should be totally unpredictable, no matter how small the time interval $\Delta$ is. But, since we are working with continuous time, we can indeed consider very small $\Delta$ 's. Martingales should then display very irregular trajectories. If fact, $X_{t}$ should not display any trends discernible by inspection, even during infinitesimally small time intervals $\Delta$ . If it did, it would become predictable. Such irregular trajectories can occur in two different ways. They can be continuous, or they can display jumps. The former leads to continuous martingales, whereas the latter are called right continuous martingales. Figure 1 displays an example of a continuous martingale. Note that the trajectories are continuous, in the sense that for $\Delta \to 0$ , 

$$
\Delta X _ {t} = X _ {t + \Delta} - X _ {t},
$$

where $\Delta > 0$ represents a small time interval. What type of trajectories would such an $X_{t}$ have in continuous time? To answer this question, first define the martingale difference $\Delta X_{t}$ , 

$$
E ^ {\tilde {P}} [ X _ {t + \Delta} | I _ {t} ] = X _ {t},
$$

asset pricing.
But this is not the only reason why martingales are useful tools. Martingale theory is very rich and provides a fertile environment for discussing stochastic variables in continuous time. In this section, we discuss these useful technical aspects of martingale theory. 

$$
E ^ {\tilde {P}} \left[ e ^ {- r u} S _ {t + u} | I _ {t} \right] = S _ {t},
$$

In the absence of arbitrage possibilities, market equilibrium suggests that we can find a synthetic probability distribution $\tilde{P}$ such that all property discounted asset prices $S_{t}$ behave as martingales: 

4 Relevance of Martingales in Stochastic Modeling 

financial asset pricing, this method is more promising than the Doob-Meyer decompositions. 

The properties of the trajectories of continuous square integrable martingales can be made more precise. Assume that $\{X_{i}\}$ represents a trajectory of a continuous square integrable martingale. Pick a time interval $[0,T]$ and consider the times $\{t_i\}$ : 

(In fact, $M_t$ will be a submartingale.) Hence, changing the underlying probabilities or the information set may alter martingale characteristics of a process. 

good news and the bad news are independently. Finally, during a small interval $\Delta$ , at most one instance of good news of one instance of bad news can occur, and the probability of this occurrence is the same for both types of news. Thus, the probabilities of incremental changes $\Delta N^{G}, \Delta N^{B}$ during $\Delta$ is assumed to be given approximately by 

good of bad. The $N_{t}^{G}$ and $N_{t}^{B}$ denote the total number of instances of “good” and “bad” news, respectively, until time t. We assume further that the way news arrives in financial markets is totally unrelated to past data, and that the “good” news and the “bad” news are independent. 

Note what this essentially means. If the continuous square integrable martingale is appropriate for modeling an asset price, one may as well assume normality for small increments of the price process. 

for all t > 0.
Such a process has finite variance and is called a continuous square integrable martingale. It is significant that one can represent all such martingales by running the Brownian motion at a modified time clock. [See Karatzas and Shreve (1991)]. In other words, the class of continuous square integrable martingales is very close to the Brownian motion. This suggests that the unpredictability of the changes and the absence of jumps are two properties of Brownian motion in continuous time.
Note: this essentially means. If the continuous square integrable 

This irregular behavior and the possibility of incorporating jumps in the trajectories is certainly desirable as a theoretical tool for representing asset prices, especially given the arbitrage theorem. But martingales have significance beyond this. In fact, suppose one is dealing with a continuous martingale $X_{i}$ that also has a finite second moment 

This means that $V^{4}$ will tend to zero. The same argument can be applied to all variations of order greater than two. 

As long as $V^{2}$ converges to a well-defined random variable, $^{7}$ the right-hand side of (39) will go to zero. The reason is the same as above. The $X_{i}$ is a continuous martingale and its increments get smaller as the partition of the interval $[0, T]$ becomes finer. Hence, as $t_{i} \to t_{i-1}$ for all i: 

Surprisingly, the opposite is true. As $[0,T]$ is partitioned into finer and finer subintervals, changes in $X_{t}$ get smaller. But, at the same time, the number of terms in the sum defining $V^{1}$ increases. It turns out that in the case of a continuous-time martingale, the second effect dominates and the $V^{1}$ goes toward infinity. The trajectories of continuous martingales have infinite variation, except for the case when the martingale is a constant. This can be shown heuristically as follows. We have 

$$
V ^ {2} <   \max _ {i} | X _ {t _ {i}} - X _ {t _ {i + 1}} | V ^ {1}.
$$

This is true because $X_{t}$ is after all a random process with nonzero variance. Now consider some properties of $V^{\perp}$ and $V^2$ . First, note that even though $X_{t}$ is a continuous martingalc, and $X_{t_{1}}$ approaches $X_{t_{1-1}}$ as the subinterval $[t_1, t_{i-1}]$ becomes smaller and smaller, this does not mean that $V^{\perp}$ also approaches zero. The reader may find this surprising. After all, $V^{\perp}$ is made of the sum of such incremental changes: 

some very important properties. We recall some relevant points. Remember that we want $X_{t}$ to be continuous and to have a nonzero variance. As mentioned earlier, this means two things. First, as the partitioning of the interval [0, T] gets finer and finer, "consecutive" $X_{t}$ 's get nearer and nearer, for any $\epsilon > 0$ 

Heuristically, $V^{1}$ can be interpreted as the length of the trajectory followed by $X_{i}$ during the interval [0, T]. The quadratic variation is given by 

Leaving aside formal aspects of defining such a process $X_{i}$ , here we ask a simple question: is $X_{i}$ a martingale? The process $X_{i}$ is the "accumulation" of infinitesimal increments over 

change in $X_{i}$ is denoted by $dX_{i}$ . Incremental changes in $X_{i}$ are assumed to be independent across time. Under these conditions, if $\Delta$ is a small interval, the increments $\Delta X_{i}$ during $\Delta$ will have a normal distribution with mean $\mu\Delta$ and variance $\sigma^2\Delta^8$ . This means 

Suppose $X_{t}$ represents a continuous process whose increments are normally distributed. Such a process is called a (generalized) Brownian motion. We observe a value of $X_{t}$ for each $t$ . At every instant, the infinitesimal 

These themes will reappear when we deal with the differentiation and integration operations in stochastic environments. A reader who remembers the definition of the Riemann-Stieltjes integral can already see that the same methodology cannot be used for integrals taken with respect to continuous square integrable martingales. This is the case since the Riemann-Stieltjes integral uses the equivalent of $V^1$ in deterministic calculus and considers finer and finer partitions of the interval under consideration. In stochastic environments such limits do not converge. Instead, stochastic calculus is forced to use $V^2$ . We will discuss this in detail later 

These properties have important implications. First, we see that $V^{1}$ is not a very useful quantity to use in the calculus of continuous square integrable martingales, whereas the $V^{2}$ can be used in a meaningful way. Secondly higher-order variations can be ignored if one is certain that the underlying process is a continuous martingale. 

• All higher-order variations will vanish in some probabilistic sense. A heuristic way of interpreting this is to say that higher-order variations do not contain much information beyond those in $V^{1}$ and $V^{2}$ . 

- The variation $V^1$ will converge to infinity in some probabilistic sense and the continuous martingale will behave very irregularly.
- The quadratic variation $V^2$ will converge to some well-defined random variable. This means that regardless of how irregular the trajectories are the martingale is square integrable and the sums of squares of the increments over small subperiods converge. This is possible because the square of a small number is even smaller. Hence, though the sum of increments is “too large” in some probabilistic sense, the sum of squared increments is not. 

For formal proofs of such arguments, the reader can consult Karatza and Shreve (1991). Here we summarize the three properties of the trajectories: 

The last equality follows because increments in $S_{t}$ are uncorrelated with current and past $S_{t}$ . As a result, the cross product terms drop. But this means that 

This is a sum to be received at time T and may be random if $r_{s}$ is stochastic. Here $B_{T}$ is assumed to be known.

Finally, consider the ratio $G_{T}/B_{T}$ , which is a relative price. In this ratio, we have a random variable that will be revealed at a fixed time T. As we get more information on the underlying asset, $S_{t}$ , successive conditional expectations of this ratio can be calculated until the $G_{T}/B_{T}$ is known exactly at time T. Let the successive conditional expectations of this ratio, calculated using different information sets, be denoted by $M_{t}$ . 

This result comes from the recursive property of conditional expectations, which we will see several times in later chapters. For any random variable Z, we can write: 

with respect to some probability $P$ . It turns out that the sequence of forecasts, $\{M_t\}$ , is a martingale. The is, for $0 < s$ : 

Intervals. Consider a random variable $Y_{T}$ with probability distribution $P$ . $Y_{T}$ will be revealed to us at some future date $T$ . Suppose we keep getting new information denoted by $I_{t}$ concerning $Y_{T}$ as time passes, $t, t + 1, \ldots, T$ , $1, T$ , such that: 

will be a martingale. Clearly, the $N_{i}^{*}$ also has increments that are unpre-dictable. It is a right-continuous martingale. Its variance is finite, and it's square integrable. 

We consider again the Poisson counting process $N_{t}$ discussed in the chapter. Clearly, $N_{t}$ will increase over time, since it is a counting process and the number of jumps will grow as time passes. Hence, $N_{t}$ cannot be martingale. It has a clear upward trend. Yet the compensated Poisson process denoted by $N_{t}^{*}$ , 

in order to make sure that $S_t$ is a martingale? Were not the increments of $X_t$ impossible to forecast anyway?
The answers to these questions have to do with the way one takes derivatives in stochastic environments. This is treated in later chapters. 

$^{12}$ Note the important assumption that k is finite. $^{13}$ For example, the trader may be interested in the length of the current uptrend or down-trend in asset prices. 

137 

Given that a typical object of interest is a sample path, or trajectory, of price changes, we first need to construct a set made of all possible paths. 

We observe $\Delta S_{t}$ at k distinct time points. $^{12}$ We begin with the notion of probability. The $\{p,(1-p)\}$ refers to the probability of a change in $S_{t}$ and is only a (marginal) probability distribution. What is of interest is the probability of a sequence of price changes. In other words, we would like to discuss probabilities associated with various “trajectories.” $^{13}$ Doing this requires constructing a probability space. 

(7) 

(78) 

the price of a financial asset $S_{t}$ . If the intervals between the times $t_{i-1}$ and $t_i$ are very small, and if the market is "liquid," the price of the asset is likely to exhibit at most one uptick or one downtick during a typical $t_i - t_{i-1}$ . We formalize this by saying that at each instant $t_i$ , there are only two possibilities for $S_{t_i}$ to change: 

One example provides a concrete discussion of a probability space and how one can assign probabilities to various trajectories associated with asset prices. 

The previous examples showed that it is possible to transform a wide variety of continuous-time processes into martingales by subtracting appropriate means.
In this section, we formalize these special cases and discuss the so-called 

that is, the $M_{t}$ will correctly price the zero-coupon bond. The mechanics of how $\vec{P}$ could be selected will be discussed in later chapters. But, already the idea that martingales are critical tools in dynamic assess pricing should become clear. It should also be clear that we can define several $M_{t}$ using different probabilities, and they will all be martingales (with respect to their particular probabilities). Yet, only one of these martingale will equal the arbitrary-free price of $B(t,T)$ . 

In the second half of this book we will see that, if the expectation calculated under a probability P, and if this probability is the real world probability, then $M_{t}$ will not, in general, equal the fair price $B(t, T)$ . But, if the probability used in calculating $M_{t}$ is selected judiciously as an arbitrage-free “equivalent” probability P, then 

the par value of the bond. Then, the $M_t$ is the conditional expectation of the discounted payoff maturity under the probability $P$ . It is also a martingale with respect to according to the discussion in the previous section. The intersecting question is whether we can take $M_t$ as the arbitrage-free price of the discount bond at time $t$ ? In other words, letting the $T$ -maturity default-free discount bond price be denoted by $B(t,T)$ , and assuming that $B(t,T)$ is arbitrage-free, can say that 

Suppose $r_t$ is stochastic and $G_T$ is the value at time $T$ of a default-free pure discount bond. If $T$ is the maturity date, then 

85 

(83) 

This probability is given by the binomial distribution. As $k \rightarrow \infty$ , this distribution converges to normal distribution. $^{15}$ 

$^{14}$ Addition of probabilities is permitted if the underlying events are mutually exclusive. In this particular case, different trajectories satisfy this condition by definition. $^{15}$ This is an example of weak convergence. 

Note that there are several possible trajectories that eventually result in the same value for $S_{t_{i}}$ . Adding the probabilities associated with all these combinations, we obtain 

(84) 

139 

that lead to the same $S_{i_k}^k$ . To be more precise, the highest possible value for $S_{i_k}$ is $S_{i_0} + k$ . This value will result if all incremental changes $\Delta S_i, i = 1, \dots, k$ are made of +1's. The probability of this outcome is 

Note that since a typical $S_{t_k}$ is made of the sum of $\Delta S_{t_k}$ 's, probabilities such as (81) can be used to obtain the probability distribution of the $S_{t_k}$ as well. In doing this we would simply add the probabilities of different trajectories that lead to the same $S_{t_k}^{14}$ . To be more precise, the highest possible value for $S_t$ is $S_t + k$ . This 

intermental change:
Up to this point, we have dealt with the sequence of changes in the asset price. Derivative securities are, in general, written on the price itself. For example, in the case of an option written on the S&P500, our interest is with the level of the index, not the change.
One can easily obtain the level of the asset price from subsequence and explore the property of generating probabilities. Another assumption that simplifies this task is the independence of successive price changes. This way, the probability of the whole trajectory can be obtained by simply multiplying the probabilities associated with each incremental change. 

It is worth repeating what enables us to do this. The finiteness of plays a role here, since with a finite number of possible trajectories the assignment of probabilities can be made one by one. Pricing derivatry products in financial markets often makes the assumption that $k$ is finit and exploits this property of generating probabilities. 

The probability of a trajectory that continuously declines during the first $k/2$ periods, then continuously increases until time $t_k$ , will also be the same. Since $k$ is finite, there are a finite number of possible trajectories in the sample space, and we can assign a probability to every one of the trajectories. 

Since $k$ is finite, given an initial point $S_{t_i}$ we can easily determine the trajectory followed by the asset price by adding incremental changes. This we can construct the set of all possible trajectories, i.e., the sample space. Next we define a probability associated with these trajectories. We the price changes are independent (and when $k$ is finite), doing this is each. The probability of a certain sequence is found by simply multiplying the probabilities of each price change. 

We assume again that time $t \in [0, T]$ is continuous. The value of a call option $C_t$ written on the underlying asset $S_t$ will be given by the function 

8.2.2 The Use of Doob Decomposition
The fact that we can take a process that is not a martingale and convert it into one may be quite useful in pricing financial assets. In this section we consider a simple example. 

8.2.1 The General Case
The decomposition of an upward-trending submartingale into a deterministic trend and a martingale component was done for a process observed at a finite number of points during a continuous interval. Can a similar decomposition be accomplished when we work with continuously observed processes? 

where $Z_{t_{k}}$ is a martingale. Hence, we decomposed a submartingale into two components. The first term on the right-hand side is an increasing deterministic variable. The second term is a martingale that has a value of $S_{\theta_{0}} + (1 - 2p)$ at time $t_{0}$ . The expression in (94) is a simple case of Doob-Meyer decomposition. $^{17}$ 

Consider the case where the probability of an uptick at any time $t_i$ somewhat greater than the probability of a downtick for a particular asset so that we expect a general upward trend in observed trajectories: 

8.1.1 Is $S_{t_{k}}$ a Martingale?
Is the $\{S_{t_{k}}\}$ defined in Eq. (82) a martingale with respect to the information set consisting of the increments in “past” price changes $\Delta S_{t_{k}}$ ?
Consider the expectations under the probabilities given in (86) 

(105) 

$$
E _ {t _ {0}} [ M _ {t _ {k}} ] = M _ {t _ {0}} + E _ {t _ {0}} \left[ \sum_ {i = 1} ^ {k} E _ {t _ {i - 1}} [ H _ {t _ {i - 1}} (Z _ {t _ {i}} - Z _ {t _ {i - 1}}) ] \right].
$$

option at time $^{2}$ .
However, this method of asset pricing is rarely pursued in practice. It is more convenient and significantly easier to convert asset prices into martingales, not by subtracting their drift, but instead by changing the underlying probability distribution P. 

We can use the results thus far to define a new martingale $M_{i}$ . Let $H_{i-1}$ be any random variable adapted to $I_{i,1}$ . Let $Z_i$ be any martingale with respect to $I_i$ and to some probability measure $P$ . Then the process defined by will also be a martingale with respect to $I_{t}$ . The idea behind this representation is not difficult to describe. $Z_{t}$ is a martingale and has unpredictable increments. The fact that $H_{t-1}$ is $I_{t-1}$ -adapted means $H_{t-1}$ are “constants” given $I_{t-1}$ . Then, increments in $Z_{t}$ will be uncorrelated with $H_{t-1}$ as well. Using these observations, we can calculate 

Then $e^{-n}C_t$ will be a martingale. But can we expect $e^{-n}S_t$ to be a martingale under the true probability. As discussed in Chapter 2, under the assumption that investors a risk-averse, for a typical risky security we have where the expectation is taken with respect to the distribution function that governs the price movements. Given this forecast, one may be tempted to ask if the fair market value $C_t$ will equal a properly discounted value of $E^p[\max [S_T - K,0] | I_t]$ . For example, suppose we use the (constant) risk-free interest rate $r$ discount $E^P[\max [S_T - K,0] | I_t]$ , to write 

According to this, if the underlying asset price is above the strike price $K$ , the option will be worth as much as this spread. If the underlying asset price is below $K$ , the option has zero value. At an earlier time $t, t < T$ , the exact value of $C_T$ is unknown. But can calculate a forecast of it using the information $I_t$ available at time $t$ . 

$^{21}$ As we will see later, the nonanticipative nature of the function $g(\cdot)$ implies that $g(C_{s})$ and $dM_{s}$ are uncorrelated. 

In this section, we show that this theorem is an abstract version of some very important market practices and that it suggests a general methodology for martingale methods in financial modeling. 

where the $D_{s}$ is known given the information set $I_{s}$ , the $g(\cdot)$ is a nonan-ticipative function of $C_{s}$ , and $M_{s}$ is a martingale given the information sets $\{I_{s}\}$ and the probability P.21 

(11) 

Doob-Meyer decomposition is a Martingale Representation Theorem. These types of results at the outset seem fairly innocuous. Given any submartingale $C_{t}$ , they say that we can decompose it into two components. One is a "known" trend given the information at time $t$ , the other is a martingale with respect to the same information set and the probability $P$ . This statement is equivalent, under some technical conditions, to the representation 

(110) 

$$
\alpha_ {t _ {0}} B _ {t _ {0}} + \beta_ {t _ {0}} S _ {t _ {0}} + \sum_ {j = 1} ^ {i - 1} [ \alpha_ {t _ {j}} [ B _ {t _ {j + 1}} - B _ {t _ {j}} ] + \beta_ {t _ {j}} [ S _ {t _ {j + 1}} - S _ {t _ {j}} ] ]
$$

where $i=1,2,\ldots,n$ . According to this strategy, the investor can sell his holdings at time for an amount equal to the left-hand side of the equation, and with all these proceeds purchase $\alpha_{i_{t}},\beta_{i_{t}}$ units of riskless and risky securities. In the sense his investment today is completely financed by his investment in previous period. 

securities at time $t_i$ . Suppose we now consider trading strategies that are self-financing. The are strategies where time $t_i$ investments are financed solely from the proceeds of time $t_{i-1}$ holdings. That is, they satisfy 

Let $\alpha_{t_{i-1}}$ and $\beta_{t_{i-1}}$ be the number of shares of riskless and risky curities held by the investor right before time $t_i$ trading begins. Clearly these random variables will be $I_{t_i}$ -adapted. $^{20}$ $\alpha_{t_0}$ and $\beta_{t_0}$ are the nonrandom initial holdings. Let $B_{t_i}$ and $S_t$ denote the prices of the riskless and risk securities at time $t_i$ . 

Stochastic integrals have interesting applications in financial theory. Of these applications is discussed in this section. We consider a decision maker who invests in both a riskless and a risk security at trading times $t_i$ : 

given the information at time $t$ : The question that we will investigate in the next few chapters is whether such an integral can be defined meaningfully. For example, can the Riemann-Stieltjes approximation scheme be used to define the stochastic integral in (108)? 

It turns out that $M_t$ defined this way is the first example of a stocktic integral. The question is whether we can obtain a similar result with $\sup_i [t_i - t_{i-1}]$ goes to zero. Using some analogy, can we obtain an expression such as 

$$
C _ {T} = C _ {t} + \sum_ {i = 1} ^ {n} D _ {t _ {i}} \Delta + \sum_ {i = 1} ^ {n} g (C _ {t _ {i}}) \Delta M _ {t _ {i}},
$$

(118) 

where the $\alpha_{t_{i}}, \beta_{t_{i}}$ are the “weights” of the replicating portfolio that en-
sure that its value matches the $C_{t_{i}}$ . Note that we know the terms on the
right-hand side, given the information at time $t_{i}$ . Hence, the $\{\alpha_{t_{i}}, \beta_{t_{i}}\}$ are
nonanticipative. We can now apply the martingale representation theorem
using this “hedge,” i.e., the replicating portfolio. 

We proceed in discrete time by letting $h > 0$ represent a small, finite terval and we subdivide the period $[t,T]$ into $n$ such intervals as in the previous section. The $C_t$ and $S_t$ represent the current price of a derivative security and the price of the underlying asset, respectively. The $C_t$ is unknown of the problem below. The $T$ is the expiration date. At expiration, the derivative will have a market value equal to its payoff, 

## 11 A Pricing Methodology

way of pricing derivative securities.
In the next section we do exactly that. First we show how a marting representation can be obtained for a derivative security's price $C_{r}$ . The we look at the implications of this representation and explain the notion of a self-financing portfolio. 

$$
E _ {t} ^ {p} \left[ \int_ {t} ^ {T} g \left(\frac {C _ {s}}{B _ {s}}\right) d M _ {s} \right] = 0,
$$

First, some motivation for what is described below. Suppose we would like to price a derivative security whose price denoted by $C_i$ . At expiration, its payoff is $C_T$ . We have seen in Chapter that a properly normalized $C_i$ can be combined with a martingale measure $\bar{P}$ to yield the pricing equation: 

It turns out that this equation can be obtained from (111). Note that Eq. (112), it is as if we are applying the conditional expectation operator $E_{t}^{p}[ \cdot ]$ to both sides of Eq. (111) after normalizing the $C_t$ by $B_t$ , and the letting 

The bracketed terms in (126) will not, in general, vanish under such an operation. But, at this point there are two tools available to us.
First, we can divide the $\{C_{v}, B_{v}, S_{i}\}$ in (126) by another arbitrage-free price, and write the martingale representation not for the actual prices, but instead for normalized prices. Such a normalization, if done judiciously, may 

Accordingly, at this point we cannot expect to apply an expectation operator $E_{i}^{P}[\cdot]$ , where $P$ is real-life probability, to Eq. (126) and hope to end up with something like 

The second bracketed term will be unknown given the information set $I_{t_i}$ , because it involves the price changes $\Delta S_{t_i}, \Delta B_{t_i}$ that occur after $t_i$ , and hence may contain new information not contained in $I_t$ . However, although unknown, these price changes are, in general, predictable. Thus we cannot expect the second term to play the role of $dM_t$ in the martingale representation theorem. The second bracketed term will, in general, have a nonzero drift and will fail to be a martingale. 

Consider the first bracketed term. Given the information set at time $t_{i+1}$ , every element of this bracket will be known. The $B_{t_{i+1}}, S_{t_{i+1}}$ are prices observed in the markets, and the $\Delta\alpha_t, \Delta\beta_t$ is the rebalancing of the replicating portfolio as described by the financial analyst. Hence, the first bracketed term has some similarities to the $D_t$ term in the martingale representation (111). 

Now consider the terms on the right-hand side of this expression. The $C_t$ is the unknown of the problem. We are, in fact, looking for a method to determine an arbitrage-free value for this term that satisfies the pricing Eq. (112). The two other terms in the brackets need to be discussed in detail. 

$$
C _ {T} = C _ {t} + \sum_ {i = 0} ^ {n} \left[ (\Delta \alpha_ {i}) B _ {t _ {i + 1}} + (\Delta \alpha_ {i}) S _ {t _ {i + 1}} \right]
$$

$$
+ \sum_ {i = 0} ^ {n} (\Delta \alpha_ {i}) S _ {t _ {i + 1}} + \sum_ {i = 0} ^ {n} \alpha_ {t _ {i}} (\Delta S _ {t _ {i}}).
$$

$$
\sum_ {i = 0} ^ {n} \Delta \left[ \alpha_ {i} S _ {i} \right] = \sum_ {i = 0} ^ {n} \left(\Delta \alpha_ {i}\right) S _ {i, i + 1} + \sum_ {i = 1} ^ {n} \alpha_ {i} \left(S _ {i}\right),
$$

$$
\sum_ {i = 0} ^ {n} \Delta [ \alpha_ {i} B _ {i} ] = \sum_ {i = 0} ^ {n} (\Delta \alpha_ {i}) B _ {i + 1} + \sum_ {i = 1} ^ {n} \alpha_ {i} (B _ {i})
$$

where the $\Delta$ represents the operation of taking first differences.
Now, recall that the “change” in a product, u.v., can be calculated using the “product rule”: 

the arbitrage-free value of the unknown $C_{i}$ . So, how do we eliminate this last bracketed term in Eq. (138)? We do this by choosing the $\{\alpha_{i_i},\beta_{i_i}\}$ so that 

$$
= \tilde {C} _ {i} + E _ {i} ^ {\tilde {p}} \left\{\sum_ {i = 0} ^ {n} \left[ (\Delta \alpha_ {t _ {i}}) \tilde {B} _ {t _ {i + 1}} + (\Delta \alpha_ {t _ {i}}) \tilde {S} _ {t _ {i + 1}} \right] \right\} + 0. \tag {137}
$$

$$
+ \sum_ {i = 0} ^ {n} \left[ \sum_ {i = 0} ^ {n} \alpha_ {i} (\Delta \tilde {S} _ {i}) \right]
$$

$$
E _ {t} ^ {P} \left[ \tilde {C} _ {T} \right] = \tilde {C} _ {t} + E _ {t} ^ {\tilde {P}} \left[ \sum_ {i = 0} ^ {n} \left[ (\Delta \alpha_ {i}) \tilde {B} _ {t - 1} + (\Delta \alpha_ {i}) \tilde {S} _ {t - 1} \right] \right]
$$

$$
\tilde {C} _ {T} = \bar {C} _ {t} + \sum_ {i = 1} ^ {n} \left[ (\Delta \alpha_ {i}) \bar {B} _ {t + 1} + (\Delta \alpha_ {i}) \bar {S} _ {t + 1} \right] + \sum_ {i = 1} ^ {n} \left[ \alpha_ {i} (\Delta \bar {S} _ {i}) \right],
$$

where the $\tilde{P}$ is the risk-neutral probability, obtained from state-prices as discussed in Chapter 2. Hence normalized $S_{i}$ also has zero mean under $\tilde{P}$ . We can now use the discrete time equivalent of this logic to eliminate the unwanted bracketed terms in (126). We start by writing 

where we substituted r for $dB_{r}/B_{r}$ . Remember from Chapter 2, that under the no-arbitrage condition, and with money market normalization, 

11.3 Normalization and Risk-Neutral Probability
In order to implement the steps discussed above, we first “normalize every asset by an appropriately chosen price. In this case, a convenient normalization is to divide by the corresponding value of $B_{i}$ and define ensure that any drift in the $C_{t}$ process is “compensated” by the drift of the normalizing variable. This may indeed be quite convenient given that we may want to discount the future payoff, $C_{T}$ , anyway.
Second, when we say that the second bracketed term is in general pro dictable, and hence, not a martingale, we say this with respect to the real-world probability. We can invoke the Girsanov theorem and switch probability distributions. In other words, we could work with risk-neutral probabilities. $^{23}$ We now show how these steps can be applied to Eq. (126). 

A reader willing to learn more about martingale arithmetic should consult the introductory book by Williams (1991). The book is very readable and provides details on the mechanics of all major martingale results using simple models. Revuz and Yor (1994) is an excellent advanced text on martingales. The survey by Shiryayev (1984) is an intermediate-level treatment that contains most of the recent results. For trading gains and stochastic integrals, the reader may consult Cox and Huang (1989). Dellacherie and Meyer (1980) is a comprehensive source on martingales. Musiela and Rutkowski (1997) is an excellent and comprehensive source on martingale methods in asset pricing. 

This is an important property of stochastic integrals. But it is also a restriction imposed on financial market participants by the way information flows in markets. Martingale methods are central in discussing such equalities. They are also essential for practitioners. 

$$
E _ {t} \left[ \int_ {t} ^ {t + T} \sigma_ {\nu} d W _ {u} \right] = 0.
$$

This equation has the same form as (108). If every incremental news is unpredictable, then the sum of incremental news should also be unpredictable (as of time t). But this means that $S_{t}$ should be a martingale, and we must have 

$$
S _ {t + T} = S _ {t} + \int_ {t} ^ {t + T} + _ {t} ^ {t} = I _ {+ t} ^ {n}.
$$

where $\sigma_{t}$ is volatility and $dW_{t}$ is an increment of Brownian motion. Note that volatility has a time subscript, and consequently changes over time. Also note that $dS_{t}$ has no predictable drift component. Over a longer period, such unpredictable information will accumulate. After an interval T, the asset price becomes 

Let $S_{t}$ be the price of an asset observed by a trader at time t. During infinitesimal periods, the trader receives new unpredictable information on $S_{t}$ . These are denoted by 

that will be useful in later chapters.
This chapter also introduced ways of obtaining martingales from processes that have positive (or negative) time trends.
We close this chapter with a discussion that illustrates why theoretic concepts introduced here are relevant to a practitioner. 

The third tool was the measure change. By calculating expectations using the risk-neutral probability, we made sure that the remaining unwanted terms in the martingale representation vanished. In fact, utilization of the risk-neutral measure had the effect of changing the expected trend of the $S_t$ process, and the normalization made sure that this new trend was eliminated by the growth in $B_t$ . As a result of all this, the normalized $C_t$ ends up having no trend at all and became a martingale. This gives the pricing Eq. (126), if one uses self-financing replicating portfolios. 

for all $i$ . That is, the time $t_{i+1}$ value of the portfolio chosen at time $t_i$ exactly sufficient to readjust the weights of the portfolio. Note that this le equation is written for the nonnormalized prices. This can be done because whatever the normalization we used, it will cancel out from both sides. 

Let $S_{t}$ be the price of a security, and let $F(S_{t}, t)$ denote the price of a derivative instrument written on $S_{t}$ . A stockbroker will be interested in knowing $dS_{t}$ , the next instant's incremental change in the security price. On the other hand, a derivatives desk needs $dF_{t}$ , the incremental change in the 

This section gives a heuristic comparison of differentiation in deterministic and stochastic environments. 

2 Motivation 

Constructing the SDE from scratch has a side benefit. This is one way we can get familiar with methods of continuous-time stochastic calculus. It may provide a bridge between discrete-time and continuous-time calculations, and several misconceptions may be eliminated this way. 

the adj and the diffusion coefficients, respectively. They are $t_{i}$ -adapted. Second, we study the properties of the innovation term $dW_{i}$ , which drives the system and is the source of the underlying randomness. We show that $W_{i}$ is a very irregular process and that its derivative does not exist in the sense of deterministic calculus. Hence, increments such as $dS_{i}$ or $dW_{i}$ have to be justified by some other means. 

where $dW_{t}$ is an innovation term representing unpredictable events that occur during the infinitesimal interval dt. The $a(S_{t}, t)$ and the $b(S_{t}, t)$ are the drift and the diffusion coefficients, respectively. They are $I_{t}$ -adapted. 

$dS_{t} = a(S_{t},t)dt + b(S_{t},t)dW_{t},$ 

More precisely, we first show under what conditions the behavior of a continuous-time process, $S_{t}$ , can be approximated using the dynamics described by the stochastic differential equation 

culties in defining stochastic differentiation equations (SDE) as well: This chapter treats differentiation in stochastic environments using the stochastic differential equations as the underlying model. We first construct the SDE from scratch, and then show the difficulties of importing the differentiation formulas directly from deterministic calculus. 

approximated reasonably well by a deterministic model. But, in the case of pricing derivative assets, the randomness of the underlying instrument is essential. After all, it is the desire to eliminate or take risk that leads to the existence of derivative assets. In deterministic environments, where everything can be fully predicted, there will be no risk. Consequently, there will be no need for financial derivative products. But if randomness is essential, how would one define differentiation in a stochastic environment? 

157 

2 Motivation 

where $f_{x}$ is the derivative of $f(x)$ with respect to x. We need similar concepts in stochastic environments as well. For example, given the variations in the price of an underlying asset $S_{p}$ , how would the price of, say, a call option written on S, react? In deterministic environments one would use “standard” rules of differentiation to investigate questions. But in pricing financial assets we deal with stochastic variables and the notion of risk plays a central role. Can similar formulas be used when the underlying variables are continuous-time stochastic processes? The notion of differentiation is closely linked to models of ordinary differential equations (ODE), where the effect of a change in a variable another set of variables can be modeled explicitly. In fact, (vector) differential equations are formal ways of modeling the dynamics of deterministic processes, and the existence of the derivative is necessary for doing this. Can differential equations be used in modeling the dynamics of assets as well? The first difficulty in doing this is because of the randomness of asset prices. The way heat is transferred in a metal rod may be 

## df = fx dx,

Differentiation in deterministic environments was reviewed in Chapter 2. The derivative of a function $f(x)$ with respect to $x$ gave us information about the rate at which $f(\cdot)$ would respond to a small change in $x$ , denote by $dx$ . This response was calculated as 

## 1 Introduction

# Differentiation in Stochastic Environments

$^{4}$ In the following, for notational simplicity, we omit the arguments of $f_{x}(x_{0})$ , $f_{\pi}(x_{0})$ , 

But read literally, this equality means that, “on the average,” the size of $(\Delta x)^{2}$ is nonzero. In other words, as soon as x becomes a random variable, treating $(\Delta x)^{2}$ as if it were zero will be equivalent to equating its variance 

Consider the second term $\frac{1}{2}f_{xx}(\Delta x)^{2}$ . If the variable x were deterministic, one could have said that the term $(\Delta x)^{2}$ is small. This could have been justified by keeping the size of $\Delta x$ nonnegligible, yet small enough that its square $(\Delta x)^{2}$ is negligible. In fact, if $\Delta x$ was small, the square of it would be even smaller and at some point would become negligible. However, in the present case, x is a random variable. So, changes in x will also be random. Suppose these changes have zero mean. Then a random variable is random, because it has a positive variance: 

On the right-hand side of this representation, $\Delta x$ represents a “small” change in the random variable x. Note that although this change is considered to be small, we do not want it to be so small that it becomes negligible. After all, our purpose is to evaluate the effect of a change in x on the $f(x)$ , and this cannot be done by considering negligible changes in x. Hence, in a potential approximation of the right-hand side, we would like to keep the term $f_{x}\Delta x$ . 

discussion of this important issue. Suppose $f(x)$ is a function of a random process $x^2$ . Now suppose we want to expand $f(x)$ around a known value of $x$ , say $x_0$ . A Taylor series 

Here, $f(x+h)-f(x)$ represents the change in the function as x changes by h. Hence, if x represents time, then the derivative is the rate at which $f(x)$ is changing during an infinitesimal interval. $^{1}$ In this case, time is a deterministic variable and one can use “standard” calculus. 

price of the derivative instrument written on $S_{i}$ . How can one calculate the $dF_{i}$ departing from some estimate of $dS_{i}$ ? What is of interest here is not how the underlying instrument changes, but, instead, how the financial derivative responds to change in the price of the underlying asset. In other words, a “chain rule” needs to be utilized. If the rules of standard calculus are applicable, a market participant can use the formula 

(18) 

$^{6}$ Remember that in probabilistic convergence we are interested in finding a random variable $X_{n}^{*}$ , to which a sequence or family of random variables $X_{n}$ converges. For “large” n, the limiting random variable $X_{n}^{*}$ can then be used as an approximation for $X_{n}$ , since often the limiting variable would be easier to handle than $X_{n}$ itself. 

$0 = t_{0} < t_{1} < \dots < t_{k} < \dots < t_{n} = T.$ 

We will consider a time interval $t \in [0, T]$ . Consider Figure 1. The $x$ axis, $[0, T]$ , is partitioned into $n$ intervals of equal length $h$ . In terms of the notation used in previous chapters, we consider intervals given by the partitions 

In order to understand the way differentiation can proceed in stochastic environments, the SDE will be “constructed” from scratch. The construction will proceed from discrete time to continuous time. We will consider a time interval $t \in [0, T]$ . 

The concept of differentiation deals with incremental changes in infinitesimal intervals. In applications to financial markets, changes in asset prices over incremental time periods are of interest. In addition, these changes are assumed to be random. Thus, in stochastic calculus, the concept of derivative has to use some type of probabilistic convergence. $^{6}$ 

One result of all this is the way differentiation is handled in deterministic and stochastic environments. For example, in the case of Eq. (14), we can try to divide both sides by $\Delta x$ and obtain the approximation 

Once $x$ becomes deterministic, we can assume that $(\Delta x)^2$ is negligible for small $\Delta x$ , and use 

$^{5}$ Some readers may remember the discussion involving variations of continuous-time martingales in Chapter 6. There, we showed that for continuous square integrable martingales, the first variation was infinite and the quadratic variation converged to a meaningful random variable, while the higher-order variations all vanished. Hence, if the x is a continuous square integrable martingale, the higher-order terms in $\Delta x$ can be set equal to zero in some approximate sense. 

A second possibility is to use, instead of $E[(\Delta x)^2]$ , some appropriate limit of the random variable $(\Delta x)^2$ as the time interval under consideration goes to zero. Such approximations were discussed in Chapter 4. It turns out that under some conditions, these two procedures would result in the same expression. In fact, if $h$ represents the time period during which the change $\Delta x$ is observed, and if $h$ is "small," under some conditions $\sigma^2 h$ may be close enough to $(\Delta x)^2$ in the mean square sense. Thus, we have two possible approximating equations, depending on whether $x$ is random or not. 

where the $(\Delta x)^{2}$ is replaced with its expectation. This is equivalent to replacing the term $\frac{1}{2}f_{xx}(\Delta x)^{2}$ with its “average” value as a method of approximation. In the second part of this book, we introduce tools that take exactly this direction. 

approximation must keep the second-order term.
On the other hand, note that while keeping the first- and second-order terms in $\Delta x$ on the right-hand side is required, one can still make a reasonable argument to drop the term that contains the third- and higher-order powers of $\Delta x$ . This would not cause any inconsistency if higher-order moments are negligible. $^{5}$ to zero. This amounts to approximating the random variable x by a non-random quantity and will defcat our purpose. After all, we are trying to find the effect of a random change in x on $f(x)$ . Hence, as long as x is random, the right-hand side of the Taylor series $^{2}$ If the information set is completely uninformative about the future movements in $S(t)$ , then this prediction will be zero. Under these conditions, $[S_{k}-S_{k-1}]$ will itself be the unpre-dictable component. 

What is the importance of random variables such as $\Delta W_{k}$ ? Consider a financial market participant. For this decision maker, the important information contained in asset prices is indeed $\Delta W_{k}$ . These unpredictable “news” occur continuously and can be observed “live” on all major networks such as Reuters or Bloomberg. Hence, “live” movements 

The latter is true because $E_{k-1}[\Delta W_k]$ equals zero and the $\Delta W_i, i = 1,\dots, k-1$ are known given $I_{k-1}$ . 

Here, the symbol $E_{k-1}[.]$ represents the expectation conditional on information available at the end of interval k-1. The $\Delta W_{k}$ is the part in $[S_{k}-S_{k-1}]$ that is totally unpredictable given the information available at the end of the $(k-1)$ th interval. The first term on the right-hand side represents actual change in the asset price $S(t)$ during the kth interval. The second term is the change that a market participant would have predicted given the information set $I_{k-1}$ . We call unpredictable components of new information “innovations.” Note the following properties of the innovation terms. 

Now pick a particular interval $k$ . As long as the corresponding expectations exist, we can always define a random variable $\Delta W_{k}$ in the following fashion: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/57aa1787a5235c904cc2617e04626da4132574b6ac5e065171f94677683c0f54.jpg)


(36) 

Now we are ready to discuss a very important property of $(\Delta W_{k})^{2}$ . The following proposition is at the center of stochastic calculus. 

According to this assumption, uncertainty of financial markets is not concentrated in some special periods. Whenever markets are open, there exists at least some volatility. This assumption rules out lotterylike uncertainty in financial markets. 

(3) 

$$
V _ {m a x} = \max _ {k} [ V _ {k}, k = 1, \dots , n ].
$$

(34) 

This assumption imposes an upper bound on the variance of cumulative errors and makes the volatility bounded from above. As the time axis is chopped into smaller and smaller intervals, more frequent trading is allowed. Such trading does not bring unbounded instability to the system. A large majority of market participants will agree with this assumption as well. After all, allowing for more frequent trading and having access to on-line screens does not lead to infinite volatility. For the third assumption, define 

## ASSUMPTION 2: NOLLIMUSSA

(33) 

and the variance of cumulative errors, V, will be positive. That is, more and more frequent observations of securities prices will not eliminate all the “risk.” Clearly, most financial market participants will accept such an assumption. Uncertainty of asset prices never vanishes even when one observes the markets during finer and finer time intervals. 

This assumption imposes a lower bound on the volatility of security prices. It says that when the period $[0, T]$ is divided into finer and finer sub-intervals, $^{9}$ 

where $A_{1}$ is independent of n. 

where the property that $\Delta W_{k}$ are uncorrelated across $k$ is used and the expectations of cross product terms are set equal to zero. We now introduce some assumptions, following Merton (1990). 

The innovation term $\Delta W_{k}$ represents an unpredictable change. $(\Delta W_{k})^{2}$ is in square. In deterministic environments, the concept of differentiation deals with terms such as $\Delta W_{k}$ , and squared changes are considered as negligible. Indeed, in deterministic calculus, terms such as $(\Delta W_{k})^{2}$ do not show up during the differentiation process. $^{8}$ On the other hand, in stochastic calculus one in general has to take into account the variation in the second-order terms. This section deals with a formal approximation of these terms. There are two ways of doing this. One is the method used in course on stochastic processes. The second is the one discussed in Merton (1990). We use Merton's approach because it permits a better understanding of the economics behind the assumptions that will be made along the way. Merton's approach is to study the characteristics of the information flow financial markets and to try to model this information flow in some prices 

in asset prices will be dominated by $\Delta W_{k}$ . This implies that to discuss differentiation in stochastic environments, one needs to study the properties $\Delta W_{k}$ . In particular, we intend to show that under some fairly acceptable assumptions, $\Delta W_{k}^{2}$ and its infinitesimal equivalent $dW_{i}^{2}$ cannot be considered as “negligible” in Taylor-style approximations. 

This term is a conditional expectation, or a forecast of a change in asset prices. The magnitude of this change depends on the latest information set and on the length of the time interval one is considering. Hence, $E_{k-1}[S_k - S_{k-1}]$ can be written as 

According to this, $S_{i}$ can be regarded as a random variable with log-normal distribution. We would like to work with the possible trajectories followed by this process. 

which says that the increments in $W_{t}$ have zero mean and a variance equal to $t - s$ . Thus, at $t$ the variance is equal to the time that elapsed since $W_{s}$ is observed. We also know that these Wiener increments are independent over time. 

1. We consider the random process $S_{t}$ , which plays a fundamental role in Black-Scholes analysis: 

The proof that, under the three assumptions, unpredictable errors will have a variance proportional to $h$ , is from Merton (1990). The chapter in Merton (1990) on the mathematics of continuous-time finance could at this point be useful to the reader. 

On the other hand, the difficulty of defining the differentials notwithstanding, we needed few assumptions to construct a SDE. In this sense, a stochastic differential equation is a fairly general representation that can be written down for a large class of stochastic processes. It is basically constructed by decomposing the change in a stochastic process into both a predictable part and an unpredictable part, and then making some assumptions about the smoothness of the predictable part. 

Differentiation in standard calculus cannot be extended in a straightforward fashion to stochastic derivatives, because in infinitesimal intervals the variance of random processes does not equal zero. Further, when the flow of new information obeys some fairly mild assumptions, continuous-time random processes become very erratic and time derivatives may not exist. In small intervals, $\Delta W_{k}$ dominates $h$ . As the latter becomes smaller, the ratio of $\Delta W_{k}$ to $h$ is likely to get larger in absolute value. A well-defined limit cannot be found. 

$^{12}$ Given $I_{k-1}$ , we are dealing with nonrandom quantities, and the derivatives in the Tap series expansion can be taken in a standard fashion. 

How can these terms be made more explicit?
It turns out that to do this we need to define the fundamental concept
the Ito integral. Only with the Ito integral can we formalize the notion
stochastic differentials such as $dS_{i}$ , dW, and hence give a solid interpretation
of the tools of stochastic differential equations. This, however, has to w
until Chapter 9. 

At several points in this chapter we had to discuss limits of random increments. The need to obtain formal definitions for incremental change such as $dS_{t}$ , $dW_{t}$ is evident. 

In later chapters, we let $h \rightarrow 0$ and obtain the infinitesimal version (57), which is the stochastic differential equation (SDE): 

Also, the convention in the literature dealing with ordinary stochastic differential equations is that any deterministic terms having powers of greater than one are small enough to be ignored. $^{13}$ Thus, as in standard calculus, we can let 

Here, $a(I_{k-1})$ is the first derivative of $A(I_{k-1}, h)$ with respect to $h$ evaluated at $h = 0$ . The $R(I_{k-1}, h)$ is the remainder of the Taylor series expansion. Now, if $h = 0$ , time will not pass and the predicted change in asset price will be zero. In other words, 

CHAPTER 7 Differentiation in Stochastic Environme 

What distinguishes rare events is the way their size and their probability of occurrence changes (or does not change) with the observation interval. 

We show that "rare events" have something to do with the discontinuity of observed price processes. This is not the same as turbulence. Increased variance or volatility can be accounted for by continuous-time stochastic processes. 

What makes an event “extreme” or “rare”? Is turbulence in financial markets the same as “rare events”? In this chapter we intend to clarify the probabilistic structure of rare events and contrast them with the behavior of Wiener processes. In particular, we discuss the types of events that a Wiener process is capable of characterizing. This discussion naturally leads to the characterization of rare events. 

At every instant of an ordinary trading day, there are three states of the world: prices may go up by one tick, decrease by one tick, or show no change. In fact, the price of a liquid instrument rarely changes by more than a minimum tick. Hence, pricing financial assets in continuous time may proceed quite realistically with just three states of the world, as long as one ignores “rare” events. Unfortunately, most markets for financial assets and derivative products may from time to time exhibit “extreme” behavior. These periods are exactly when we have the greatest need for accurate pricing. 

# The Wiener Process an Rare Events in Financial Markets

(g) Do you think the term in the previous question is a well-defined random variable? 

change as time passes?
(f) If $\Delta \rightarrow 0$ , what happens to the trajectories of the “random variable” 

for “small” 0 < Δ.
(d) Let $\Delta = .25$ . What does the term 

bers.
Plot the $W_{t}$ and $S_{t}$ . (You will obtain piecewise linear trajectory that will approximate the true trajectories.)
(b) Repeat the same exercise with a subdivision of [0, 1] into 8 into val. 

(a) Construct the $W_{t}$ and $S_{t}$ over the [0, 1] using these random numbers. 

$x \sim N(0, 25)$ . 

Let $\mu = .01, \sigma = .15$ and $t = 1$ . Subdivide the interval $[0,1]$ into subintervals and select 4 numbers randomly from: 

CHAPTER·7 Differentiation in Stochastic Environment 

By combining these two building blocks appropriately, one can generate a model that is suitable for a particular application. Before discussing rare and normal events, this section reviews these two building blocks. 

There are two basic building blocks in modeling continuous time asset prices. One is the Wiener process, or Brownian motion. This is a continuous stochastic process and can be used if markets are dominated by “ordinary” events while “extremes” occur only infrequently, according to the probabilities in the tail areas of a normal distribution. The second is the Poisson process which can be used for modeling systematic jumps caused by rare events. The Poisson process is discontinuous. 

## 2 Two Generic Models

On the other hand, if sporadic jumps are a systematic part of asset price changes, then value-at-risk calculations become more complicated. Attaching a probability to the amount one is likely to lose in extreme circumstances requires modeling the “rare event” process as well. 

During such an exercise it is very important to know if there exist rare events that cause prices to jump discontinuously. If such jumps are not likely, value-at-risk calculations can proceed using the normal distribution. Price changes can be modeled as outcomes of normally distributed random processes, and, under appropriate conditions, the value-at-risk will also be normally distributed. It would then be straightforward to attach a probability to the amount one can lose under some extreme price movement. 

The answer depends on how much “value” is at risk. There are several ways of calculating such value-at-risk measures, but they all try to measure changes in a portfolio’s value when some underlying asset price moves in some extreme fashion. 

As an example, consider recent issues in risk management. One issue is capital requirements. How much capital should a financial institution put aside to cover losses due to adverse movements in the market? 

The answers to these questions are in general affirmative. One has to use different formulas if asset prices exhibit jump discontinuities. This will indeed affect the pricing of financial assets. 

such a distinction is important—especially if the existence of rare events implies discontinuous paths for asset prices. But are there practical applications of such discontinuities? Would pricing financial assets proceed differently if rare events exist? 

$^{1}$ “The expected size” refers only to the absolute value of the change. Because surprises are, by definition, unpredictable, one knows nothing about the sign of these changes. $^{2}$ Or by a combination of the two. 

This chapter is focused on the distinction between rare and normal events. The reader may be easily convinced that, from a technical point, 

The first case corresponds to rare events, and the second to normal events. 

But remember how a “standard deviation” is obtained: one multiplies possible sizes with the corresponding probabilities. It is the product of two terms, the probability multiplied by the “size” of the event. A variance proportional to h can be obtained either by probabilities that depend on h while the size is independent, or by probabilities that are independent of h while the size is dependent. $^{2}$ 

## $E[\sigma_t\Delta W_i]^2 = \sigma_i^2 h,$

The previous chapter established one important result. Under some very mild assumptions, the surprise component of asset prices, $\sigma_{t}\Delta W_{t}$ , had a variance 

A rare event is different. By definition, it is supposed to occur infrequently. In continuous time, this means that as $h \rightarrow 0$ , its probability of occurrence goes to zero. Yet, its size may not shrink. A market crash such as the one in 1987 is “rare.” On a given day, during a very short period, there is negligible probability that one will observe such a crash. But when it occurs, its size may not be very different whether one looks at an interval of 10 minutes or an interval of a full trading day. 

On the other hand, because they are ordinary, even in a very small time interval h, their probability of occurrence is not zero. During small time intervals, there is always a nonzero probability that some “nonnoticeable” news will arrive. 

In particular, as the interval of observation, h, gets smaller, the size of normal events also gets smaller. This is, after all, what makes them "ordinary." In one month, several large price changes may be observed. In a week, fewer are encountered. Observing a number of large price jumps during a period of a few minutes is even less likely. Often, the events that occur during an "ordinary" minute are not worth much attention. This is the main characteristic of "normal" events. They become unimportant as $h \rightarrow 0$ . On the other hand, because they are not 

1. The process begins at zero, $B_{0}=0$ .
2. $B_{t}$ has stationary, independent increments. 

DEFINITION: A random process $B_{t}, t \in [0, T]$ , is a (standard) Brow-nian motion if: 

The Wiener process is the natural model for an asset price that has unpredictable increments but nevertheless moves over time continuously. Before we discuss this point, however, we need to clarify a possible confusion. 

DEFINITION: A Wiener process $W_{t}$ , relative to a family of information sets $\{I_t\}$ , is a stochastic process such that: 

$^{3}$ As n goes to infinity, the expression on the right-hand side will be a sum of a very large number of random variables that are independent of one another and that are all infinitesimal size. Under some conditions, the distribution of the sum will be approximate normal. This is typical of central limit theorems, or, in continuous time, of weak convergence 

One can also approach the Wiener process as a continuous square integrable martingale. In fact, suppose $W_{t}$ is a process that is continuous, has finite variance, $^{4}$ and has increments that are unpredictable given the family of information sets $\{I_{j}\}$ . $^{5}$ Then, according to a famous theorem by Levy, these properties are sufficient to guarantee that the increments in $W_{t}$ are normally distributed with mean zero and variance $\sigma^{2} dt$ . 

In this definition, a Wiener process is obtained as the limit, in some probabilistic sense, of a sum of independent, identically distributed random variables. The important point to note is that possible outcomes for these increments are functions of $h$ , the length of subintervals. As $h \to 0$ , changes in $W_i$ become smaller. With this approach, we see that the Wiener process will have a Gaussian (normal) distribution. 

will converge weakly to a Wiener process as n goes to infinity. Heuristically, this means that the Wiener process will be a good approximating model for the sum on the right-hand side, $^{3}$ 

In continuous time, "normal" events can be modeled using the Wiener process, or Brownian motion. A Wiener process is appropriate if the underlying random variable, say $W_t$ , can only change continuously. With a Wiener process, during a small time interval $h$ , one in general observes "small" changes in $W_t$ and this is consistent with the events being ordinary. There are several ways one can discuss a Wiener process. 

(12) 

(三)

This is heuristic because we do not know whether we can treat increments such as $dM_{i}$ as "objects" similar to standard random variables. To make the discussion precise, one must begin with a finite subdivision of the time interval, and then present some type of limiting argument. 

$E[dM_{i}]^{2} = \lambda dt.$ 

$E[dM_{t}]^{2} = 1^{2}\lambda dt + 0^{2}[1 - \lambda dt],$ 

$^{9}M_{t}$ is called a compensated Poisson process. The $\lambda t$ is referred to as the compensatory term. It “compensates” for the positive trend in $N_{t}$ and converts it into a “trendless” process $M_{t}$ . 

Second, the probability that $M_{t}$ will show a jump during a very small interval goes to zero. Heuristically, this means that the trajectories of $M_{t}$ are less irregular than the trajectories of $W_{t}$ , because the Poisson counting process is constant “most of the time.” Although $M_{t}$ displays discrete jumps, 

(10) 

Thus, although the trajectories of $M_{t}$ are discontinuous, the first and second moments of $M_{t}$ and $W_{t}$ have the same characterization. In particular, over small time intervals of length h, both processes have increments with variance proportional to $h^{10}$ . 

will be a discontinuous square integrable martingale. $^{9}$ It is interesting to note that 

The reader would recognize $N_{t}$ as the Poisson counting process. Assuming that the rate of occurrence of these events during $dt$ is $\lambda$ , the process defined as 

case of Brownian motion is that, this time, the size of Poisson outcomes does not depend on dt. Instead, the probabilities associated with the outcomes are functions of dt. As the observation period goes toward zero, the increments of Brownian motion become smaller $^{8}$ while the movements in $N_{t}$ remain of the same size. 

621 

$^{7}$ At this point, the use of $dN_{t}$ and dt instead of $\Delta N_{t}$ and h should be considered symbolic. In later chapters, it is hoped that the meaning of the notation $dN_{t}$ and dt will become clearer. 

Note that here we have increments in $N_{t}$ that can assume two possible values during an infinitesimal interval $dt$ . The critical difference from the 

The increments in $N_t$ can have only one of two possible values. Either they will equal zero, meaning that no new major event has occurred, or they will equal one, implying that some major event has occurred. Given that major events are "rare," increments in $N_t$ that have size 1 should also occur rarely. We use the symbol $dN_t$ to represent incremental changes in $N_t$ during an infinitesimal time period of length $dt$ . Consider the following characterization of the incremental changes in $N_t$ : 

Now consider a quite different type of random environment. Suppose $N_{t}$ represents the total number of extreme shocks that occur in a financial market until time t. Suppose these major events occur in an unpredictable fashion. 

This theorem is very explicit. We can use the terms Wiener process and Brownian motion interchangeably. Hence, no distinction will be made between these two concepts in the remaining chapters. 

THEOREM: Any Wiener process $W_{t}$ relative to a family $I_{t}$ is a Brownian motion process. 

These appear to be very important differences. In fact, the reader may think that $W_{i}$ is much more general than the Brownian motion, since no assumption is made about its distribution. 

This definition is, in many ways, similar to that of the Wiener process. There is, however, a crucial difference. $W_t$ was assumed to be a martingale, while no such statement is made about $B_t$ . Instead, it is posited that $B_t$ has a normal distribution. 

3. $B_{t}$ is continuous in t.
4. The increments $B_{t}-B_{s}$ have a normal distribution with mean zero and variance $|t-s|$ : 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/20347e2569c824f50bda61ca90f5332a1fb6e1e0228108ae7b6fa95b06d57eb5.jpg)


- The path shows occasional jumps, due to the Poisson component.
- Between jumps, the process is not constant; it fluctuates randomly. This is due to the Wiener component. 

Figure 2 displays a mixture of the Poisson and Wiener processes. First, a trajectory was drawn from the Poisson process. Next, the computer was asked to generate a trajectory from a standard Wiener process with variance h = .001. The two trajectories were added to each other. We see the following characteristics of this sample path: 

- The trajectory has a positive slope. (Hence, $N_{t}$ is not a martingale.)
- Changes occur in equal jumps of size 1.
- The trajectory is constant between these jumps.
- In this particular example, there are 14 jumps, which is very close to the mean. 

to generate a trajectory for the Poisson counting process $N_{t}, t \in [0,1]$ . This trajectory is displayed in Figure 1. We note the following characteristics of the Poisson paths: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/b45c4a7f45abcda21776e60fd45fd72c6cf8a58fcf17fd7bc7a335bea52d2810.jpg)


Indeed, it is true that, in general, the Riemann-Stieltjes definition may be applied to this latter integral. 

it will not have unbounded variation. $W_{i}$ , on the other hand, displays infinitesimal changes, but these changes are uncountably many. As a result, the variation becomes unbounded. Hence, it may be more difficult to define integrals such as $^{13}$ There are two reasons that we introduce this assumption. First, the distinction between rare and normal events will be much easier to introduce if the possibilities are finite. Second, actual asset pricing in financial markets often proceeds with either binomial or trinomial trees. In the case of binomial trees, the market participant assumes that, at any instant, there are only two possible moves for the price. With trinomial trees, possible moves are raised to three. Hence, in practical situations, the total number of possible states is selected as finite anyway. 

$^{11}$ Remember from Chapter 7 that in order to obtain the SDE in discrete intervals, we used several approximations. For small but noninfinitesimal $h_{i}$ , such equations hold in an approximate sense only. 

$\sigma_{k}\Delta W_{k} = \left\{ \begin{array}{ll}w_{1} & \text{with probability } p_{1}\\ w_{2} & \text{with probability } p_{2}\\ \vdots & \vdots \\ w_{m} & \text{with probability } p_{m}. \end{array} \right.$ 

ASSUMPTION 4: $\Delta W_{k}$ can assume only a finite number of possible values. The possible outcomes of $\Delta W_{k}$ and their corresponding probabilities are $^{13}$ 

where the $a(S_{k-1}, k)h$ is the drift component which determines how, on the average, the increment $S_{k} - S_{k-1}$ is expected to behave during the next interval. $\Delta W_{k}$ is the innovation term, determining the “surprise” component of asset prices. It was shown that, under some assumptions, the variance of the innovation term is proportional to h, the length of the interval. The term $\sigma(S_{k-1}, k)^{2}$ is the factor of proportionality. 

$S_{k} - S_{k-1} = a(S_{k-1}, k)h + \sigma(S_{k-1}, k)\Delta W_{k},\quad k = 1,2,\dots,n,\tag{13}$ 

A deeper analysis of normal vs rare events is best done by considering a stochastic differential equation in finite intervals. $^{11}$ Consider again the SDE that was introduced for discrete intervals of equal size h in Chapter 7: 

3 SDE in Discrete Intervals, Again 

single news item in determining the price or interest rate or currency derivatives is significantly smaller, although present. In the following sections, we characterize normal and rare events, and learn ways of modeling price series that are likely to exhibit occasional jumps. 

of the process. Several markets in derivatives exhibit jumps in prices. This is more often the case in commodities, where a single news item is more likely to carry important information for the underlying commodity. Reports on crop for example, are likely to cause jumps in futures on the same commodity. In the case of financial derivatives, this is less likely. The weight of 

What we need is a disturbance term that is capable of generating large events in extremely small intervals. In other words, we need a process that may exhibit jumps. Such a process will have outcomes that do not depend on h, and as h gets small, the size of the outcomes will not shrink.
Thus, “rare” events correspond to occasional jumps in the sample path. 

The problem with characterizing rare events using a Wiener process is the following. As $h$ goes to zero, the tails of the normal distribution carry less and less weight. At the limit, $h = 0$ , these tails have completely vanished. In fact, the whole distribution has concentrated on zero. This is to be expected because the Wiener process is continuous with probability one. As $h \to 0$ , the size of price changes represented by the Wiener process has to become smaller and smaller. In this sense, the Wiener process is not suitable for representing situations where, in an extremely short interval prices can move in some extreme fashion. 

price changes is normal.
A normal distribution has tails that extend to infinity. With small but nonzero h, there is a positive probability that a very large, unexpected price change will occur. Hence, with a nonzero h, the Wiener process seems to be perfectly capable of introducing “big” events in the stochastic differential equations. Why would we then need another discussion of “rare” or big events? 

Compared to events that occur in a routine fashion, a rare event is by definition something that has a "large" size. This classification seems obvious, but at a closer look, is not very easy to justify. Consider the Wiener process. A stochastic differential equation that is driven by a Wiener process amounts to assuming that in small intervals of length $h$ , unexpected price changes occur with a variance of $\sigma^2 h$ , where the $\sigma$ may depend on the available information as well. Further, the distribution of these unexpected price changes is normal. 

2.4 Back to Rare Events 

• The noise introduced by the Wiener process is much smaller than the jumps due to the Poisson process. This may change if we select a Wiener process with higher variance. Then, it could be very difficult to distinguish between Poisson jumps and noise caused by the Wiener component. 

CHAPTER 8 The Wiener Process and Rare Events 

$^{15}$ We show the potential dependence of $w_{i}$ , $p_{i}$ on the information that becomes available as time passes, by adding the k subscript to $\sigma_{k}$ . $^{16}$ In general, $c_{i}$ will depend on k as well. To keep notation simple, we eliminate the k subscript. 

where $r_i$ and $q_i$ are nonnegative constants. $\bar{w}_i$ and $\bar{p}_i$ are constants that may depend on $i$ or $k$ , but are independent of $h$ , the size of the observation interval. 

where $0 < c_{i}$ is some factor of proportionality. $^{16}$ Equation (18) says that all terms such as $p_{i}w_{i}^{2}$ are linear functions of h. Then, one can visualize the $p_{i}$ and the $w_{i}$ as two functions of h, whose product is proportional to h. That is, 

Now, the left-hand side of (17) is a sum of $m$ finite, nonnegative numbers. If the sum of such numbers is proportional to $h$ , and if each element is positive (or zero), then each term in the sum should also be proportional to $h$ or should equal zero. In other words, each $p_i w_i^2$ will be given by 

where the parameter m is the number of possible states. The left-hand side of Eq. (17) is simply the weighted average of squared deviations from the mean, which in this case is zero. The “weights” are probabilities associated with possible outcomes. $^{15}$ 

$^{14}$ Both $w_{i}$ and $p_{i}$ can very well be made to depend on the information set $I_{k}$ . However, this would add a k subscript to these variables and make the notation more cumbersome. The avoid this, we make $w_{i}$ and $p_{i}$ independent of k. 

events is eventually obtained. According to assumption 4, $\Delta W_{k}$ can assume only a finite number of values. In terms of $w_{i}$ and the corresponding probabilities, $p_{i}$ , we can explicitly write the variance as 

rameter given the information set $t_{k-1}$ . This result can be exploited further if we use assumption 4. In fact, a very explicit characterization of rare and normal events can be given this way, although the reader may find the notation a bit unpleasant. However, this is a small price to pay if a useful characterization of rare and normal events is eventually obtained. 

The remaining possibilities, $w_4$ , $w_5$ , ... are reserved for various types of special events that may occur rarely. For example, if the underlying security is a derivative written on grain futures, $w_4$ may be the effect of a major drought, the $w_5$ may be the effect of an unusually positive crop forecast, and so on. Clearly, if such possibilities refer to extreme price changes, and if they are rare, then they must lead to price changes greater than one tick. Otherwise, price changes are caused by normal events $w_1$ , $w_2$ , $w_3$ . This setup will be used in the next section to determine the probabilistic structure of any event. 

Although it is not clear which event will occur, the set of possible events is known by all agents. A typical $w_{i}$ represents a possible outcome of the innovation term $\sigma_{k}\Delta W_{k}$ , while $p_{i}$ denotes the associated probability. The parameter m is the total number of possible outcomes. It is an integer. $^{14}$ There are two types of $w_{i}$ . The first three represent “normal” outcomes. For example, $w_{1}$ may represent an uptick, $w_{2}$ may be a downtick, and the $w_{3}$ may represent “no change” in asset prices. In real time, these are certainly routine developments in financial markets. 

To interpret this, consider what happens when we select $r_{i}=1/2$ . First, we know that the $q_{i}$ must equal zero. $^{18}$ As a result, the functions that govern the size and the probability of the outcome $w_{i}$ become, respectively, 

To characterize rare and normal events we use the parameters $r_{i}$ and $q_{i}$ . Both of these parameters are nonnegative, $r_{i}$ governs how fast the size of the event goes to zero as the observation interval gets smaller, $q_{i}$ governs how fast the probability goes to zero as the observation interval decreases. It is, of course, possible that $r_{i}$ or $q_{i}$ vanish, although they cannot do so at the same time. $^{17}$ 

Figure 3 displays some choices for $h^r$ . Three examples are shown: the case when $r_i = 1$ (not allowed in this particular discussion), the case when $r_i = .5$ , and the case when $r_i = 1/3$ . In particular, we see that for small $h$ , $h^r > h$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/11ea01028f6e20228b4db76d1eafeb15075e9e358177ce5fe77bced6cb31b584.jpg)


The events $w_{i}$ that have a $r_{i}=0$ , $q_{i}=1$ are “rare” events, since, according to this equation, their probability vanishes as $h\to0$ . On the other hand, the size of the events will be given by 

This means that as the interval $h$ gets smaller, the $W_{i}$ starts to change at an infinite rate. Asset prices will behave continuously but erratically. (Here we assumed, without any loss of generality, that $\bar{w}_{i}$ was positive.) This concludes the discussion of trajectories that are generated by events of normal size. We now consider paths generated by rare events. 

proportional to $h^{1/2}$ . In other words, as time passes, the new events that affect prices will cause changes of the order $\sqrt{h}$ .
At any time t, the unexpected rate of change of prices can be written as are continuous. But they are not smooth.

First remember what smoothness means within the context of a deterministic function. Heuristically, a function will be “smooth” if it does not change abruptly. In other words, suppose we select a point $x_{0}$ where the function $f(x)$ is evaluated. $f(x)$ will be smooth at $x_{0}$ if for small h, the ratio depend on h. These outcomes are “small” but have a constant probability of occurrence as observation intervals get smaller. They are “ordinary.” Now suppose all possible outcomes for $\Delta W_{k}$ are of this type and have $r_{i} = .5$ . Then the sample paths of the resulting $W_{t}$ process will have a number of interesting properties. 

(52) 

One can be more specific. First, split the error term in two. It is clear from the previous discussion that changes in asset prices will be a mixture of normal events that occur in a continuous fashion, and of jumps that occur sporadically. We denote the first component by $\Delta W_{k}$ . The second component is denoted by the symbol $\Delta N_{k}$ . To make this more precise, assume that the event is a jump in asset prices of size 1. At any instant $k - 1$ , one has 

In the case of rare events, the defining factors are that the size of the event is not infinitesimal even when $h$ is, while its probability does become negligible with $h \to 0$ . Accordingly, the new innovation term should be able to represent (random) jumps that occur rarely in asset prices. Further, the model should be flexible enough to capture any potential variation of the probability of occurrence of such jumps. 

There is no need to adopt a different representation in order to take into account rare events. These also occur unexpectedly, and their variance is also proportional to $h$ , the time interval. In fact, the only difference from the case of a Wiener process occurs in the continuity of sample paths. Hence, the same SDE representation can be used with a simple modification. What is needed is a new model for the random, unpredictable errors $dW_{t}$ . 

that is predictable given the information at that time, and another that is unpredictable. In small intervals of length $h$ , we write events:
Consider what is needed. Our approach tries to represent asset prices by an equation that decomposes observed changes into two components: one 

## 5 A Model for Rare Events

Note that for such outcomes the corresponding probabilities also go to zero. Thus, these outcomes are not observed frequently. But given that their size will get smaller, they are not qualified as rare events. 

have $r_i$ and $q_i$ within these ranges? It turns out that for all $r_i, q_i$ within these ranges, the sample paths will be continuous but nonsmooth, just as in the case of a Wiener process. This is easy to see. As long as $0 < r_i < .5$ is satisfied, the size of $w_i$ will be a function of $h$ . As $h \to 0$ , $w_i$ will go to zero. In terms of size, they are not rare events. 

4.2.2 Further Comments
What can be said of the remaining values for $r_{i}$ and $q_{i}$ ? In other words, consider the ranges 

are not common. Clearly, if the random variable $\Delta W_{k}$ contains jumps, its sample paths will not be continuous. One would need a model other than the Wiener process to capture the behavior of such random shocks. 

On the other hand, if $q_i = 1$ , the probability of these jumps will depend on $h$ , and as the latter gets smaller, the probability of observing a jump will also go down. Hence, although the trajectory contains jumps, these jumps are not common. 

4.2.1 Sample Paths
Sample paths of an innovation term that contains rare events will be discontinuous. In fact, the sizes of those $w_{i}$ with $q_{i}=1$ do not depend on h. As h goes to zero, $\Delta W_{k}$ will from time to time assume values that do not get any smaller. The size of unexpected price changes will be independent of h. When such rare outcomes occur, $W_{i}$ will have a jump. 

where the independence of $\Delta W_{k}$ and $\Delta J_{k}$ is implicitly used. Now consider the magnitude of these moments when all events are of the “normal” type, having a size proportional to $h^{1/2}$ . That is, consider the case when all $q_{i}=0$ . 

The distinction between “normal” and “rare” events is important for one other reason.
Practical work with observed data proceeds either directly or indirectly by using appropriate “moments” of the underlying processes. In Chapter 5, we defined the term “moment” as representing various expectations of the underlying process. For example, the simple expected value $E[X_{i}]$ is the first moment. The variance "rare" events simultaneously. Finally, note that the jump component $dJ_{t}$ and the Wiener component $dW_{t}$ have to be statistically independent at every instant $t$ . As $h$ gets smaller, the size of "normal" events has to get smaller, while the size of rare events remains the same. Under these conditions the two types of events cannot be "related" to each other. Their instantaneous correlation must be zero. 

## $J_{t} = (N_{t} - \lambda t)$

The increments $\Delta J_{k}$ will have zero mean and will be unpredictable. Further, if we multiply the $J_{i}$ by a (time-dependent) constant, say, $\sigma_{2}(S_{k-1}, k)$ , the size of the jumps will be time-dependent. Hence, $\sigma_{2}(S_{k-1}, k)\Delta J_{k}$ is an appropriate candidate to represent unexpected jumps in asset prices.
This means that if the market for a financial instrument is affected by sporadic rare events, the stochastic differential equations can be written as 

In fact, the Poisson process is the only process that satisfies all these conditions simultaneously. It seems to be a good candidate for modeling jump discontinuities. We may, however, need two modifications. 

very close to 1. $^{20}$ 2. The information up to time t does not help to predict the occurrence (or the nonoccurrence) of the event in the next instant h.

3. The events occur at a constant rate $\lambda$ . 

This is the case because with rare events, the probabilities are proportional to $h$ , and the latter can be factored out. With $n > 2$ , higher-order moments are also of order $h$ . As we divide higher-order moments of $\Delta J_k$ by $h$ , they will not get any smaller as $h \to 0$ . Unlike Wiener processes, higher-order moments of $\Delta J_t$ cannot be ignored over infinitesimal time intervals. This means that if prices are affected by rare events, higher-order moments may provide useful information to market participants. 

where the $w_{i}$ do not depend on $h$ . As we divide the right-hand side of the last equation by $h$ , it will become independent of $h$ . Hence, variance cannot be considered negligible. Here, there is no difference from Wiener processes. 

parameters, one representing the first moment and the second representing the variance, will be sufficient to capture all the relevant information in price data for small “h.” The Wiener process is then a natural choice if there are no rare events. 

$^{22}$ When n is greater than 2, the exponent of h will be positive. 

verge to zero.
Consequently, for small h, higher-order moments of unpredictable price changes will not carry any useful information if the underlying events are all of the “normal” type. A probabilistic model that depends only on two 

with n > 2.
Here, when the events under consideration are of the normal type, raising the $w_{i}$ to a power of n will result in terms such as 

As we divide this by h, we obtain the average rate of variance. Clearly, the h will cancel out and the rate of variance remains constant as h gets smaller. This means that the variance does not become negligible as $h \rightarrow 0$ . In the case of “normal” events, the variance provides significant information about the underlying randomness even during an infinitesimal interval h. Now consider what happens with higher-order moments, 

gets larger as h gets smaller. We conclude that when the first moment is not equal to zero, it is “large” and cannot be ignored even in small intervals h. The same is true for the second moment. The variance of an unpredictable change in prices contains terms such as $w_{i}^{2}$ . When the $w_{i}$ are of normal type, their size is proportional to $h^{1/2}$ . Hence, the variance will be proportional to h: 

As we divide this by h, we obtain the average rate of unexpected changes in prices. Clearly, for small h the $\sqrt{h}$ is larger than h, and the expression (73) 

$^{23}$ These states are labeled as “up” and “down,” but in practice, both of the movements may be up, down, or one of them may stay the same. This choice of the terms should be regarded only as a symbolic way of naming the two states. Also, the parameters $u_{i}$ and $d_{i}$ may also depend on the $S_{i}$ observed at that node or even at earlier nodes. Here we adopt the simpler case of state-independent up and down movements. 

$S_{i+1} = \left\{ \begin{array}{ll}u_iS_i & \text{with probability } p_i\\ d_iS_i & \text{with probability } t - p_i. \end{array} \right.$ 

Suppose the $S_{i}$ has an instantaneous percentage trend represented by the parameter $\mu$ , and an instantaneous precentage volatility of $\sigma$ . For both cases considered below, we assume that $S_{i}$ evolves according to the following: 

In the first case, the sizes of $u_{i}$ and $d_{i}$ will be made to depend on the $\Delta$ , whereas the probabilities associated with them will be independent of $\Delta$ . In the second case, the reverse will be true. The $u_{i}$ and $d_{i}$ will be independent of $\Delta$ , while the probabilities of up and down states will depend on it. Clearly, the first will correspond to the case of “normal” events and will eventually be captured by variables driven by the Wiener process. The second will correspond to “rare events” and will lead to a Poisson type behavior. 

The binomial model implies that once it reaches a certain state or node, at every discrete point i, the immediate movement in $S_{i}$ will be limited to only two up and down states, which depend on two parameters denoted by $u_{i}$ and $d_{i}^{23}$ . 

This gives the discrete time points $\{t_i\}$ . We next model the values of $S_{i}$ at these specific time points, $t_{i}$ . For the sake of notational simplicity, we denote these by $S_{i}$ : 

to be “systematic” and “simple.” As usual, we divide the time interval of length T into n subintervals of equal length $\Delta$ such that: 

We are interested in discretizing the behavior of a continuous-time process $S_{t}$ , over time interval [0, T], $T < \infty$ . We also want this discretization 

the other that incorporates rate events.
First we need to review the standard binomial model for a financial asset price. We work with an underlying stock price $S_{f}$ , although a process such as instantaneous spot-rate $r_{t}$ could also be considered. 

In this section, we treat how the distinction between normal and rare events will exhibit itself in practical modeling of asset price dynamics. In particular, is this distinction only a theoretical curiosity, or can it be made more concrete by explicitly taking into account the above-mentioned discussion? The answer to the last question is yes. This is best seen within the class of binomial pricing models dealt with in Chapter 2. We discuss two binomial models, one being driven by a random term representing “normal” events, the other that incorporates “rare” events. 

## 8 Rare and Normal Events in Practice

events that occur rarely.
In small intervals, the random variable $W_{t}$ is described fully by the first-and second-order moments. Higher-order moments do not provide any additional information. Hence, assuming normality and letting $W_{t}$ be the Wiener process provides a good approximation for such events. 

where the first term on the right-hand side is the expected change in $S_{t}$ , and the second term in brackets is the surprise component, unpredictable given the information at time t. The stochastic differentials were not defined formally, so the discussion proceeded using “small” increments, $\Delta S_{k}$ and $\Delta W$ . 

for SDEs. We showed that the dynamics of an asset price can always be captured by a stochastic differential equation, 

for some integer, n > 1, which, in a sense, represents the accumulated changes in $S_{i}$ after n successive periods of length $\Delta$ has passed. 

In other words, instead of looking at the probability of one-step changes in $S_{i}$ as $i$ increases, we might be interested in looking at the behavior of ∞∞ 

There is another interesting question that we can ask: Leaving aside the one-step changes, how do the accumulated movements in $S_{i}$ behave as “time” passes? 

The discussion above dealt with possible ways of modeling the probability and the size of a discretized two-state process $S_{i}$ as a function of the discretization interval $\Delta$ . We were mainly interested in what happened to one-step movements in $S_{i}$ as $\Delta$ is made smaller and smaller. 

with $\Delta$ close to zero.
Clearly, this way of modeling the binomial parameters is more in line with the rare event characterization discussed earlier in this chapter. 

which, depending on $\Delta$ , is perhaps very close to one. This is the case because in small intervals: 

Consider the implications of this type of binomial behavior. As $\Delta$ , the time interval, is made smaller and smaller, the probability $p_{i}$ of the “up” state will approach zero, whereas the probability of the “down” state will approach one. This means that $S_{i}$ becomes less likely to exhibit “up” changes, $\hat{u}$ , as we consider smaller and smaller time intervals. As $\Delta \rightarrow 0$ , the $S_{i}$ will follow a stable path during a finite interval. Yet, even with very small $\Delta$ , there is a small probability that a “rare” event will occur because according to (80): 

where $0 < \lambda$ and $0 < \alpha$ are two parameters to be calibrated according to the “size” and probability of jumps that one is expecting in $S_{i}$ . The $\hat{u} \neq 1$ is also a positive constant. It represents the behavior of $S_{i}$ when there is a jump. $d_{i}$ is the case of no jump.
Figures for the implications of this type of calibration, where A and B 

Now we keep the same characterization of the binomial setup, except change the way $u_i$ , $d_i$ , and $p_i$ are modeled. In particular, we change the dependence on the time interval $\Delta$ . Thus, in place of Eqs. (74)-(76) we assume that the parameters of the 

Clearly, this way of parameterizing a binomial model is consistent with the notion that the events that drive the $S_{i}$ over various nodes of the tree are “normal.” These events occur frequently, even in small intervals, but their size is small. 

parameters $u_i, d_i$ , and $p_i$ as $\Delta$ goes to zero. From the definitions of these parameters we see that as $\Delta \to 0$ the $u_i, d_i$ go toward zero. Hence, with a parameterization such as in Eq. (73), the movements in $S_i$ become negligible over infinitesimal intervals. Yet, the probability of these moments go to 1/2, a constant: 

First, some comments. The parameters $u_{i}, d_{i}$ , and $p_{i}$ are chosen so that they are the same at every node $i$ . This is the case because on the right-hand side of Eqs. (74)-(76) there is no dependence on $S_{i}, i = 1, \dots, i$ . According to this, the dynamics of $S_{i}$ is discretized in a fashion that is homogeneous across time. Clearly, this need not be so, and more complex $u_{i}, d_{i}$ , or $p_{i}$ can be selected as long as the dependence on $\Delta$ is kept as modeled in (74)-(76). Thus, in this particular case we can even remove the $i$ subscript from 

For the case where $S_{i}$ is influenced only by “normal” events, the growth coefficients $u_{i}$ and $d_{i}$ can be chosen as: $^{24}$ 

For n trials, the variance of the n independent movements will be n times $p(1-p)$ , or $np(1-p)$ . 

$^{26}$ The expected value is easy to calculate. If we have n independent trials, each with a probability p of “up,” then the total number of expected “up” movements will be np. The $V_{\mathrm{art}}(Z)$ is slightly more complicated. The variance of Z for a single trial is: 

Replacing this and the values of u, d, p in both (91) and (92) we can get the asymptotic equivalents of the mean and the variance. In other words, with u, d, p, given in Eqs. (74)–(76), the first order approximation gives: 

$$
V a r \left[ \frac {S _ {i + n}}{S _ {i}} \right] = \left[ \log \frac {u}{d} \right] ^ {2} n p (1 - p).
$$

$$
E \left[ \frac {S _ {i + n}}{S _ {i}} \right] = \log \frac {u}{d} [ n p ] + n \log d
$$

$$
V a r \left[ \log \frac {S _ {i + n}}{S _ {i}} \right] = \left[ \log \frac {u}{d} \right] ^ {2} V a r [ Z ].
$$

With a linear equation we can calculate the mean and variance of the random variable $\log\frac{\xi_{i+n}}{5}$ easily: 

$^{25}$ The $u_{i}, d_{i}$ are multiplicative parameters. Taking the log converts a product into a sum, which is easier to analyze in asymptotic theory. Central limit theorems are formulated, in general, in terms of sums. 

As discussed in the previous paragraph, this last equation is now a linear function of the random variable Z. 

which depends on the way the main parameters of the binomial-tree are modeled. The discussion will proceed in terms of an integer-valued random variable Z, which represents the number of "up" movements observed between points i and $i + n$ . According to this, if beginning at point i, $S_{i}$ experiences only "up" movements, then Z = n. If only half of the movements are up, then Z = n/2, and so on. 

Hence, a market professional may be interested in the probabilistic behavior of the expiration point value $S_T$ as well as in its immediate change may be quite different than the $p_i$ that governs the immediate changes in $S_i$ . This is the case because in $n$ periods, the $S_i$ may assume many values different from just $u_i S_i$ or $d_i S_i$ . 

Clearly, the modeling of $S_{i}$ as a two-state process may be a reasonable approximation for the immediate future especially if the $\Delta$ is small, but may still leave the market practitioner in the dark if the trading or investment horizon is in a more distant future that occurs after $n$ steps of length $\Delta$ . For example, the interest of the market professional may be in the value of $S_{T}, t < T$ , at expiration, rather than the immediate $S_{i}$ , and the modeling of immediate one-step probabilities may not say much about this. 

The question is, what happens to the distribution of $X_{n}$ as the number of events go to infinity? There are two interesting cases, and the questions below relate to these. 

We can look at $X_{n}$ as the cumulated sum of a series of events that occur over time. The events are the individual $B_{i}$ . Note that there are two parameters of interest here. Namely, the p and the n. The first governs the probability of each “event” $B_{i}$ , whereas the second governs the number of events. 

The discussion characterizing rare events is covered in Merton (1990). The assumption that innovation terms have a finite number of possible values simplified the discussion significantly. A reader interested in the formal arguments justifying the statements made in this chapter can consider Bremaud (1979). Bremaud adopts a martingale approach to discuss the dynamics of point processes, which can be labeled as generalizations of Poisson processes. 

## 9 References

theorems?
It turns out that, in order for a properly scaled sum of independent random variables to converge to a normal distribution, each element of the sum must be asymptotically negligible. The condition for asymptotic negligibility is exactly the one that distinguishes normal events from rare events. Thus, with the choice of parameters for $u_{i}$ , $d_{i}$ , $p_{i}$ for rare events, the events are likely to be asymptotically nonnegligible, and, convergence will be toward a Poisson distribution. 

These are two examples of Central Limit Theorem, where the sum of a large number of random variables starts having a recognizable distribution. What causes this divergence between the applications of central limit 

That is, $[\log S_{i+n} - \log S_{i}]$ is approximately normally distributed. If, on the other hand, the parameterization in (78) and (79) that corresponds to rare events is adopted, then the distribution of $[\log S_{i+n} - \log S_{i}]$ will, as $\Delta \rightarrow 0$ , approximately be given by: 

$\left[\log S_{i + n} - \log S_i\right] \sim N(\mu (n\Delta), \sigma^2\Delta)$ . 

CHAPTER·8 The Wiener Process and Rare Events 

where the last term on the right-hand side is an integral with respect to increments in the Wiener process $W_{i}$ . 

Now, consider the SDE which represents dynamic behavior of some asset price $S_{i}$ : 

can be used to give meaning to $dX_{t}$ . In fact, at various earlier points, we made use of differentials such as $dS_{t}$ or $dW_{t}$ but never really discussed them in any precise fashion. The definition of the Ito integral will permit doing so. 

where future movements are expressed in terms of differentials $dX_{t}$ , dt, and $dW_{t}$ instead of derivatives such as $dX_{t}/dt$ . These differentials are defined using a new concept of integral. For example, as h gets smaller, the increments 

Yet, under some conditions, an integral can be obtained successfully. This permits replacing ordinary differential equations by stochastic differential equations 

sponding integral equation.
In stochastic calculus, application of the same agenda is not possible.
If unpredictable “news” arrives continuously, and if equations representing the dynamics of the phenomena under consideration are a function of such noise, a meaningful notion of derivative cannot be defined.
Yet under some conditions on internalism can be derived as it is 

205 

expansions. After taking into consideration any restrictions imposed by the theory under consideration, one gets the differential equation.
At the end of the agenda, the fundamental theorem of calculus is proved to show that there is a close correspondence between the notions of integral and derivative. In fact, integral denotes a sum of increments, while derivative denotes a rate of change. It seems natural to expect that if one adds changes $dX_{i}$ in a variable $X_{i}$ , with initial value $X_{0}=0$ , one would obtain the latest value of the variable: 

$^{1}$ If B = 0, the equation is said to be homogenous. When $y_{t}$ is independent of t, the system becomes autonomous. Otherwise, it is nonautonomous. $^{2}$ For example, the engineer may have in mind some desired future path for $X_{t}$ . Then the issue is to find the proper $\{y_{t}\}$ which will ensure that $X_{t}$ follows this path. 

The following agenda is used to obtain the ordinary differential equation. First, a notion of derivative is defined. It is shown that for most functions of interest denoted by $X_{i}$ , this derivative exists. Once existence is established, the agenda proceeds with approximating $dX_{i} / dt$ using Taylor series 

exogenous variable. A and B are parameters.
Ordinary differential equations are necessary tools for practical modeling. For example, an engineer may think that there is some variable y, that, together with the past values of $X_{t}$ , determines future changes in $X_{t}$ . This relationship is approximated by the differential equation, which can be utilized in various applications. $^{2}$ 

One source of practical interest in differentiation and integration operations is the need to obtain differential equations. Differential equations are used to describe the dynamics of physical phenomena. A simple linear differential equation will be of the form 

# Integration in Stochastic

## CHAPTER 9

The reader is cautioned against this. Understanding the definition of the Ito integral is important (at least) for two reasons. First, as mentioned earlier, a stochastic differential equation can be defined only in terms of the Ito integral. To understand the real meaning behind the SDEs, one has 

It may thus be difficult at this point to see the practical relevance of this concept from the point of view of, say, a trader. It may appear that defining the Ito integral is essentially a theoretical exercise, with no practical implications. A practitioner may be willing to accept that the Ito integral exists and prefer to proceed directly into using SDEs. 

In practice, the Ito integral is used less frequently than stochastic differential equations. Practitioners almost never use the Ito integral directly to calculate derivative asset prices. As will be discussed later, arbitrage-free prices are calculated either by using partial differential equation methods or by using martingale transformations. In neither of these cases is there a need to calculate any Ito integrals directly. 

Second, the $a(S_u,u),\sigma (S_u,u),u\in [t,t + h]$ were approximated by their value at $u = t$ .Both of these approximations require some smoothness conditions on $a(S_{u},u)$ and $\sigma (S_u,u)$ . All these imply that when we write 

reasons. First, the $E_{t}[S_{t + h} - S_{t}]$ was set equal to a first-order Taylor series approximation with respect to $h$ : 

$^{3}$ By the average rate of change we mean the standard deviation of $W_{t+k}-W_{t}$ divided by $h_{t}$ . In Chapter 6 it was shown that under fairly general assumptions, the standard deviations of unpredictable shocks were proportional to $h^{1/2}$ . 

This is the SDE representation in finite intervals that we often used in previous chapters. The representation is an approximation for at least two 

where h is some finite time interval.
From here, one can obtain the finite difference approximation that we used several times in Chapters 7 and 8. Indeed, if h is small, $a(S_{u}, u)$ and $\sigma(S_{u}, u)$ may not change very much during $u \in [t, t + h]$ , especially if they are smooth functions of $S_{u}$ and u. Then, we could rewrite this equation as: 

The interpretation of the integrals on the right-hand side of (6) is not immediate. As discussed in Chapters 5 through 7, increments in $W_t$ are too erratic during small intervals $h$ . The rate of change of the $W_t$ was, on the average, equal to $h^{-1/2}$ , and this became larger as $h$ became smaller. If these increments are too erratic, would not their sum be infinite? This chapter intends to show how this seemingly difficult problem can be solved. 

(21) 

Here, we have an integral of a function $g(x_t)$ taken with respect to $F(\cdot)$ . Similar notation occurs when we deal with expectations of random variables. For example, $F(\cdot)$ may represent the distribution function of a random variable $x_t$ , and we may want to calculate the expected value of some 

In the notation on the right-hand side, the integral is taken with respect to $F(\cdot)$ . Increments in $F(\cdot)$ are used to obtain the integral. We can complicate the latter notation further. For example, we may be interested in calculating the integral 

The integral on the left-hand side is taken with respect to $x_{t}$ , where $t$ varies from 0 to $T$ . Then, the value of $f(\cdot)$ at each $x_{t}$ is multiplied by the infinitesimal increment $dx_{t}$ . These (uncountably many) values are used to obtain the integral. This notation is in general preserved for the Ricmann integral. 

The integrals in (17) and (18) are summations of very erratic random variables, since two shocks that are $\epsilon > 0$ apart from each other, $dW_{t}$ and $dW_{t + \epsilon}$ , are still uncorrelated. The question that arises is whether the sum of such erratic terms can be meaningfully defined. After all, the sum of so many (uncountable) erratic elements can very well be unbounded. Consider again the way standard calculus defines the integral. 

to see why this is so. As seen earlier, increments in a Wiener process, $dW_t$ , represent random variables that are unpredictable, even in the immediate future. The value of the Wiener process at time $t$ , written as $W_t$ , is then a sum of an uncountable number of independent increments: 

dened using the no integral. This point is important from the point of view of pricing financial derivatives, since in practice one always does calculations using finite intervals. For example, "one day" is clearly not an infinitesimal interval, and the utilization of SDEs for such periods may require approximations. The precise form of these approximations will be obtained by taking into consideration the definition of Ito integral. 

to have some understanding of the Ito integral. Otherwise, errors can be made in applying SDEs to practical problems.
This brings us to the second reason why the Ito integral is relevant. Given that SDEs are defined for infinitesimal intervals, their use in finite intervals may require some approximations. In fact, the approximation in (14) may not be valid if h is not “small.” Then a new approximation will have to be defined using the Ito integral. 

$^{7}$ By considering intervals of equal length, the partition of $[0,T]$ can be made finer with $n\to\infty$ . Otherwise, the condition $\sup_{i}|t_{i}-t_{i-1}|\to0$ has to be used. 

$^{6}$ There are many different ways rectangles can approximate the area under a curve. One can pick the base of the rectangle the same way, but change the height of the rectangle to either $g(x_{i})$ or to $g(\frac{x_{i+1}+x_{i}}{2})$ . 

will exist and will be called the Riemann-Stieltjes integral. The reader should read this equality as a definition. The integral is defined as the limit of the sums on the right-hand side. $^{5}$ The sums $V_{n}$ are called Riemann sums. $^{6}$ 

$V_{n}$ is the sum of all such rectangles. If consecutive $t_{i}, i=0,\ldots,n$ are not very distant from each other—that is, if we have a fine partition of $[0,T]$ —this approximation may work reasonably well. In other words, if the function $g(\cdot)$ is integrable, then the limit 

$^{4}$ When the function $g(\cdot)$ is the square or the cube of $x_{t}$ , this integral will simply be second or third moment. 

which is the product of $g(x_{t_{i-1}})$ and $[F(x_{t_{i-1}}) - F(x_t)]$ . The first term represents $g(\cdot)$ evaluated at a point $x_{t_{i+1}}$ . The second term resembles the increments $dF(x_t)$ . Each element $g(x_{t_{i+1}})[F(x_{t_{i-1}}) - F(x_t)]$ can be visualized as a rectangle with base $[F(x_{t_{i-1}}) - F(x_t)]$ and height $g(x_{t_{i+1}})$ . 

The formal calculation using the Riemann-Stieltjes methodology is based on the familiar construction where the interval $[0, T]$ is partitioned into $n$ smaller intervals using the times 

The integral in (22) is quite different. The $t$ is constant, and it is $x$ , that goes from minus to plus infinity. The integral is not a random variable. For the case when there are no random variables in the picture, the Riemann-Stieltjes integral was defined as a limit of some infinite sum. The integral would exist as long as this limit was well defined. To highlight differences with Ito integral, we review Riemann-Stieltjes methodology once again 

Heuristically, in this integral, $x_{t}$ is varied from minus to plus infinity, and the corresponding values of $g(\cdot)$ are averaged using the increments in $dF(\cdot)$ . $dF(\cdot)$ in this case represents the probability associated with those values. Note the important difference between the integrals in (21) and (22). In the first case, it is the t that moves from 0 to T. The value of $x_{t}$ for a particular t is left unspecified. It could very well be a random variable. This would make the integral itself a random variable. 

$$
E \left[ \int_ {0} ^ {T} \sigma (S _ {t}, t) ^ {2} d t \right] <   \infty .
$$

$$
\lim _ {n \rightarrow \infty} E \left[ \sum_ {k = 1} ^ {n} \sigma (S _ {k - 1}, k) \left[ W _ {k} - W _ {k - 1} \right] - \int_ {0} ^ {T} \sigma (S _ {u}, u) d W _ {u} \right] ^ {2} = 0. \tag {37}
$$

$$
\int_ {0} ^ {T} a (S _ {u}, u) d u = \lim _ {n \to \infty} \sum_ {k = 1} ^ {n} [ a (S _ {k - 1}, k) h ].
$$

The first term on the right-hand side of (29) does not contain any random terms once information in time k becomes available. More importantly, the integral is taken with respect to increments in time h. By definition, time is a smooth function and has “finite variation.” This means that the same procedure used for the Riemann-Stieltjes case can be applied to define an integral such as $^{8}$ 

If $x_{i}$ is a Wiener process, the same approach cannot be used. First of all, the $V_{n}$ must be modified to 

$^{12}$ Equal-sized subintervals is a convenience. The same result can be shown with unequal $t_{t+1}-t_{i}$ as well. 

This situation can easily be seen in Figure 1, where we consider an arbitrary function of time $x_{i}$ and use a single rectangle to obtain the area under the curve. $^{13}$ 

$^{13}$ A single rectangle works because the function being integrated, $f(x_{i})$ , is just the 45-degree line, $f(x_{i}) = x_{i}$ . 

and let n go to infinity. The result is well known. The Riemann-Stieltjes integral of (42) with $x_{0}=0$ will be given by 

According to this definition, as the number of intervals goes to infinity and the length of each interval becomes infinitesimal, the finite sum will approach the random variable represented by the Ito integral. Clearly, the definition makes sense only if such a limiting random variable exists. The assumption that $\sigma(S_{k-1}, k)$ is nonanticipating turns out to be a fundamental condition for the existence of such a limit. $^{10}$ 

where, as usual, T = nh and for any i, $t_{i+1} - t_i = h$ . Second, one would define the sums 

The following example illustrates the utilization of mean square convergence in defining the Ito integral. In a second example, we show why the Ito integral cannot be defined "pathwise." 

To summarize, we see three major differences between deterministic and stochastic integrations. First, the notion of limit used in stochastic integration is different. Second, the Ito integral is defined for nonanticipative functions only. And third, while integrals in standard calculus are defined using the actual “paths” followed by functions, stochastic integrals are defined within stochastic equivalence. It is essentially these differences that make some rules of stochastic calculus different from standard calculus. 

must converge.
Given proper conditions, one can show that Ito sums converge and that the corresponding Ito integral exists. Yet it is, in general, not possible to explicitly calculate the mean square limit. This can be done only in some special cases. In this section, we consider an example where the mean square limit can be evaluated explicitly. $^{11}$ $^{10}$ One technical point is whether the limiting random variable, that is, the Ito integral depends on the choice of how one partitions the $[0,T]$ . It can be shown that the choice partition does not influence the value of the Ito integral. $^{11}$ This is in contrast to a proof where it is shown that the limit “exists.” 

where it is known that $x_{0}=0$ . If $x_{t}$ was a deterministic variable, one could calculate this integral using the finite sums defined in (24). To do this, one would first partition the interval $[0,T]$ into n smaller subintervals all of size h using 

$$
E \left[ \sum_ {i = 0} ^ {n - 1} \Delta x _ {t _ {i + 1}} ^ {2} - T \right] ^ {2}
$$

$$
E \left[ \sum_ {i = 0} ^ {n - 1} \Delta x _ {t _ {i + 1}} ^ {2} \right] = \sum_ {i = 0} ^ {n - 1} E [ \Delta x _ {t _ {i + 1}} ^ {2} ] = \sum_ {i = 0} ^ {n - 1} (t _ {i + 1} - t _ {i}), \tag {58}
$$

$$
E [ \sum_ {i = 0} ^ {n - 1} \Delta x _ {t - 1} ^ {2} ].
$$

$$
\lim _ {n \to \infty} E \left[ \sum_ {i = 0} ^ {n - 1} \Delta x _ {t + i} ^ {2} - Z \right] ^ {2} = 0.
$$

$$
V _ {n} = \frac {1}{2} \left[ x _ {T} ^ {2} - \sum_ {i = 0} ^ {n - 1} \Delta x _ {t + 1} ^ {2} \right].
$$

Now the first and second summations in (54) are the same except for the very first and last elements. Canceling similar terms, and noting that $x_{0}=0$ by definition, $^{14}$ 

$$
V _ {n} = \frac {1}{2} \left[ \sum_ {i = 0} ^ {n - 1} x _ {t - i} ^ {2} - \sum_ {i = 0} ^ {n - 1} x _ {t _ {i}} ^ {2} - \sum_ {i = 0} ^ {n - 1} \Delta x _ {t _ {i - 1}} ^ {2} \right].
$$

2.4.1 Explicit Calculation of Mean Square Limit
We intend to calculate the limiting random variable V step by step to clarify the meaning of the Ito integral as a mean square limit of a random sum. The first step is to manipulate the terms inside $V_{n}$ . We begin by noting that for any a and b we have 

$$
\lim _ {n \to \infty} \left[ \sum_ {i = 0} ^ {n - 1} x _ {i} \Delta x _ {i + 1} - V \right] ^ {2} = 0,
$$

integral that the integrators be nonanticipating.
Second, $V_{n}$ is now a random variable and simple limits cannot be taken.
In taking the limit of $V_{n}$ , one has to use a probabilistic approach. As mentioned earlier, the Ito integral uses the mean square limit.
Thus, we have to determine a limiting random variable V such that 

$$
\lim _ {n \to \infty} E \left[ \sum_ {i = 0} ^ {n - 1} \Delta x _ {t _ {i + 1}} ^ {2} - T \right] ^ {2} = 0.
$$

$$
E \left[ \sum_ {i = 0} ^ {n - 1} \Delta x _ {t _ {i + 1}} ^ {2} - T \right] ^ {2} = \sum_ {i = 0} ^ {n - 1} 3 (t _ {i + 1} - t _ {i}) ^ {2}
$$

is a sum of unpredictable disturbances that affect asset prices during an interval of length $\Delta$ . Now, if each increment is unpredictable given the information set at time t, the sum of these increments should also be un-predictable. This makes the integral shown in (82) a martingale difference: 

$$
E _ {s} \left[ \int_ {0} ^ {t} \sigma_ {u} d W _ {u} \right] = \int_ {0} ^ {s} \sigma_ {u} d W _ {u}, 0 <   s <   t.
$$

vHere we abuse the notation in writing $S(W_{t}) = S_{c}$ . But it simplifies the exposition. $^{18}$ For simplicity, we use one rectangle. In fact, much finer partitions of the interval $[t, t+\Delta]$ can be used. 

$$
E \left[ \left(\frac {W _ {i + \Delta} + W _ {i}}{2}\right) (W _ {i + \Delta} - W _ {i}) | W _ {i} \right] = E \left[ \frac {1}{2} (W _ {i + \Delta} ^ {2} - W _ {i} ^ {2}) | W _ {i} \right] \tag {99}
$$

Note that the term $\sigma S(W_{i})$ depends on $W_{i}$ indirectly, through $S_{i}$ . Now consider what happens when we try to approximate the second integral on the right-hand side using Riemann sums. One approximation used by Riemann sums uses the values of the Wiener process observed at “midpoints” of subintervals. This amounts to calculating first the terms 

This example is important for two reasons. First, we see the meaning of a pathwise integral. In calculating the integral pathwise, we did not use the probabilities associated with $\Delta S_{t_{i+1}}$ . The integral was calculated using the actual realization of the process. The Ito integral, on the other hand, is calculated using mean square convergence, and the integral is determined within stochastic equivalence. 

In stochastic calculus, one occasionally encounters the statement that stochastic integrals cannot be defined pathwise. What does this mean? Consider the binomial process $S_{t_{i-1}} - S_{t_i}, i = 1,2,\dots,n$ , measured over discrete intervals of length $\Delta$ during a period [0, T]: 

If such correlations are not zero, evaluating the Ito integral using Riemann sums will imply innovation disturbance terms with nonzero expectations: 

where, as usual $T = n\Delta$ . A typical path of this process will be a sequence of $+\sqrt{\Delta}$ and $-\sqrt{\Delta}$ following each other. For example, a typical realization may look like 

pathwise. This $V_{n}$ will converge, and the variation of the process $M_{t}$ will be finite with probability one. Under these conditions, we say that $V_{n}$ converges pathwise. 

conditions. Suppose a process $M_{t}$ is a martingale that exhibits finite jumps only and has no Wiener component. Trajectories of such an $M_{t}$ will exhibit occasional jumps, but otherwise will be very smooth. Then, one could define a $V_{n}$ , 

$$
E \left[ \int_ {0} ^ {t} f (W _ {u}, u) d W _ {u} \right] ^ {2} = E \left[ \int_ {0} ^ {t} f (W _ {u}, u) ^ {2} d u \right].
$$

Second, we see the importance of using nonanticipative functions as $f(\cdot)$ . In fact, because $f(\cdot)$ was able to "see the future," it anticipated the sign of $S_{t_{i+1}} - S_{t_i}$ . That made all the elements in the summation sign positive and led to an exploding $V_n$ as $n$ increased. 

4. In the above equation there are two integrals. Which integral is defined in the sense of Ito only? 

8 Exercises 

There are several excellent sources on the derivation of the Ito integral. Karatzas and Shreve (1991) and Revuz and Yor (1994) were already mentioned. Two additional sources that the reader may find a bit easier to read are Oksendal (1992) and Protter (1990). The former source could be a very good manual for quantitatively oriented practitioners and for beginning graduate students. It is well written and easy to understand. Technicalities are avoided as much as possible. 

convergence. Fortunately, in evaluating Ito integrals, the direct route of obtaining the mean square limit will rarely be used. Instead, Ito integrals can be evaluated in a more straightforward fashion using a result called Ito's Lemma. This will be discussed in the next chapter, where we will also discuss further examples of evaluating the Ito integral. 

We also discussed several examples and showed that the rules of integration are in general very different in stochastic environments, when compared with the deterministic case. This was the result of using mean square convergence. 

This chapter dealt with the definition of the Ito integral. From the point of view of a practitioner, there are two important points to keep in mind. First, the error terms in stochastic differential equations are defined in the sense of the Ito integral. Numerical calculations must obey the conditions set by this definition. Second, the stochastic differential equations routinely used in asset pricing are also defined in the sense of the Ito integral. 

The chain rule is quite similar to the total derivative. In classical calculus, the chain rule expresses the rate of change of a variable as a chain effect of some initial variation. In stochastic calculus, we know that operations such as $dF_{t}/dt$ , $dS_{t}/dt$ cannot be defined for continuous-time square integrable martingales, or Brownian motion. But a stochastic equivalent of the chain rule can be formulated in terms of absolute changes such as $dF_{t}$ , $dS_{t}$ , dt, and the Ito integral can be used to justify these terms. Thus, in stochastic calculus, the term “chain rule” will refer to the way stochastic differentials relate to one another. In other words, a stochastic version of total differentiation is developed. 

The total derivative is a more “realistic” notion. It is assumed that both time t and the underlying security price $S_{t}$ change, and then the total response of $F(S_{t}, t)$ is calculated. The result is the (stochastic) differential $dF_{t}$ . This is clearly a very useful quantity to the market participant. It represents the observed change in the price of the derivative asset during an interval dt. 

A classical example of the use of partial derivatives occurs in delta hedging. Suppose a market participant knows the functional form of $F(S_{t}, t)$ . Then, this mathematical formula can be differentiated only with respect to $S_{t}$ , in order to find the partial derivative $F_{s}$ . This $F_{s}$ is a measure of how much the derivative asset price will change per unit change in $S_{t}$ . In this sense, one does not have any of the difficulties encountered in defining a time derivative for Wiener processes. What is under investigation is not how $F(S_{t}, t)$ moves over time, but how $F(\cdot)$ responds to a “small” hypothetical change in $S_{t}$ , with time fixed. 

Various reasons.
The partial derivative has no direct real-life counterpart, but gives “multipliers” that can be used in evaluating responses of asset prices to observed changes in risk factors. For example, $F_{s}$ measures the response of $F(S_{t}, t)$ to a small change in $S_{t}$ only. As such, $F_{s}$ is a hypothetical concept, since the only way a continuous random variable $S_{t}$ can change is if some time passes. Hence, in reality, t has to change as well. Partial derivatives abstract from such questions. Because they are simple multipliers, there is no difference between the way stochastic and deterministic environments define partial derivatives. 

A financial market participant may be interested in these derivatives for various reasons. 

$\frac{dF(S_{t},t)}{dt} = F_{s}\frac{dS_{t}}{dt} +F_{t}\cdot$ 

In (2), $dF_{t}$ is used as a shorthand notation for $dF(S_{t}, t)$ . This should not be confused with $F_{t}$ , the partial of $F(\cdot)$ with respect to t. The third is the chain rule: 

2 Types of Derivatives 

The second is the total derivative dealing with differentials: 

Suppose we have a function $F(S_t, t)$ depending on two variables $S_t$ and $t$ , where $S_t$ itself varies with time $t$ . Further, assume that $S_t$ is a random process. 

2 Types of Derivatives 

We begin by discussing various types of derivatives. 

to be used in place of derivatives. Ito's rule provides an analytical formula that simplifies handling stochastic differentials and leads to explicit computations. It is the main topic of this chapter. 

As discussed earlier, in stochastic environments a formal notion of derivative does not exist. Shocks to asset prices are assumed to be unpredictable, and in continuous time they become “too erratic.” The resulting asset prices may be continuous, but they are not smooth. Stochastic differentials need to be used in place of derivatives. 

## 1 Introduction

## Ito's Lemma

$^{2}$ Incidentally, some readers may wonder if this “smoothness” does not contradict the extreme irregularity of $S_{i}$ . $F(\cdot)$ can be a smooth function of $S_{i}$ , and still be a very irregular stochastic process. Irregularity here is in the sense of how $F(\cdot)$ changes over time. It is not a statement about how $S_{i}$ relates to $F(\cdot)$ . 

The applicability of the Taylor series formula to a random environment is a deeper issue. First, it should be remembered that some of the terms in Taylor series are partial derivatives. With respect to these, one does not have any difficulty with differentiation in stochastic environments. Second, we have differentials such as $dS_{t}$ . Here, we do need an adjustment, which is in terms of the interpretation of the equality and not in the Taylor series expansion itself. The formula for Taylor series expansion will remain the 

where $X$ denotes the remainder. We apply this formula to $F(S_t, t)$ . At the outset, $F(\cdot)$ has to be a smooth function of $S_t^2$ . But there are two additional complications. First, the Taylor series formula in (9) is valid for a $f(x)$ which is a function of a single variable $x$ , while $F(S_t, t)$ depends on two variables, $S_t$ and $t$ . Second, the formula in (9) is valid for deterministic variables, while $S_t$ is a random process. Before using Taylor series, these complications must be addressed. The extension of a univariate Taylor series formula to two variables is straightforward. One adds the partials with respect to the second variable. 

We calculate Ito's formula in this setting, using the Taylor series. Re-call the Taylor series expansion of a smooth (i.e., infinitely differentiable) function $f(x)$ around some arbitrary point $x_0$ . 

using the mean square equivalence between the left- and right-hand side as $h \to 0$ . This notation will be preserved throughout this chapter. Also note that we shortened the notation for $a(S_{k-1}, k)$ to $a_k$ and for $\sigma(S_{k-1}, k)$ to $\sigma_k$ . 

233 

Let the random process $S_{t}$ be observed in continuous time. We again partition the time interval $[0,T]$ into $n$ equal pieces, each with length $h$ , and use the finite difference approximation. However, we write this as an equality 

as time passes, one obtains new information about $W_{t}$ and observes a new increment, $dS_{t}$ . This will also make $F(\cdot)$ change. The sum of these two effects is represented by the stochastic differential $dF(S_{t}, t)$ and is given by the stochastic equivalent of the chain rule. Let the random process $S_{t}$ be observed in continuous time. We again 

$^{1}$ Recall that such quantities are defined in terms of mean square convergence and within stochastic equivalence. 

The stochastic version of the chain rule is known as Ito's Lemma. Let $S_t$ be a continuous time process which depends on the Wiener process $W_t$ . Suppose we are given a function of $S_t$ , denoted by $F(S_t, t)$ , and suppose we would like to calculate the change in $F(\cdot)$ when $dt$ amount of time passes. Clearly, passing time would influence the $F(S_t, t)$ in two different ways. First, there is a direct influence through the $t$ variable in $F(S_t, t)$ . Second, 

This example suggests that when $r_{t}$ is random, we may be able to define the counterpart of total derivative, using the Ito integral, which gives a meaning to stochastic differentials such as $dr_{t}$ . This intuition is correct, and the result is Ito's formula. However, with stochastic $r_{t}$ , not only does the interpretation of $dr_{t}$ change, $^{1}$ but the formula will also be different. 

On the other hand, the total derivative relates to the actual occurrence of random events. In standard calculus, with nonrandom $r_t$ , the total derivative of this particular $F(\cdot)$ will be given by 

Note that these partials will be the same regardless of whether $r_{t}$ is deterministic or random. By taking these partial derivatives, we are simply calculating the rate of change of $F(\cdot)$ with respect to small hypothetical changes in $r_{t}$ or in t. 

We discuss a simple example before going into Ito's formula. The example will help clarify the mechanics of taking various derivatives. Let $F(r_t, t)$ be the price of a T-bill that matures at time $T$ , and let $r_t$ be a fixed, continuously compounding risk-free rate. Then 

This section discusses the convention used in determining which variables can be classified as “negligible” in stochastic calculus. In standard calculus, the Taylor series expansion of some function $f(S)$ around $S_{0}$ gives 

The first-order effects are the effects of time, represented by $F_{t}[h]$ , and the effects of change in the underlying asset's price, $F_{s,t}[a_k h + \sigma_k \Delta W_k]$ . In the latter we again see that changes in security prices have predictable and unpredictable components. Second-order effects are those changes that are represented, for the time being, by squared terms and by cross products. Higher-order terms are grouped in the remainder $R$ . 

In order to obtain a chain rule in stochastic environments, the terms on the right-hand side will be classified as negligible and nonnegligible. It will then be shown that in “small” time intervals, negligible terms can be dropped from the right-hand side and a chain rule formula obtained. In addition, as $h \rightarrow 0$ , a limiting argument can be used and a precise formula obtained in the mean square sense. This formula is known as Ito's Lemma.

The first step of this derivation is to separate the terms on the right-hand side. This requires an explicit criterion for deciding which terms are negligible. Afterward, one can consider the size of the terms on the right-hand side of (11) individually and decide which ones are to be dropped. 

What does this equation mean? On the left-hand side, $\Delta F(k)$ indicates the total change in $F(S_k,k)$ due to changing $k$ and $S_{k}$ . Hence, if $F(S_{k},k)$ is the price of a derivative security, on the left-hand side we have the change in the derivative asset's price during a short interval. This change is explained by the terms on the right-hand side. The first-order effects are the effects of time represented by $F[k]$ and 

This is equivalent to assuming that while in the Taylor series expansion (18), $\Delta S$ is small and noneligible, the terms involving $(\Delta S)^2$ , $(\Delta S)^3$ , ... are smaller and can be ignored as $\Delta S \to 0$ . Consequently, in the limit, the term $f_s dS$ is preserved, while all other terms are dropped. The result is the (total) differentiation formula (19). 

We can substitute the right-hand side of this for $\Delta S_{k}$ in the Taylor series expansion of (11): 

$$
F (S _ {k}, k) - F (S _ {k - 1}, k - 1) = \Delta F (k)
$$

where the partials $F_{s}, F_{ss}, F_{t}, F_{tt}, F_{st}$ are all evaluated at $S_{k-1}, k-1$ . R represents the remaining terms of the Taylor series expansion. Here we are keeping the $F_{t}, F_{st}, F_{tt}$ notation for convenience, although these partials are with respect to k.

Transpose $F(S_{k-1}, k-1)$ and relabel the increments in (11) as follows: 

First, fix $k$ . Given the information set $I_{k-1}$ , $S_{k-1}$ is a known number. Next, apply Taylor's formula to expand $F(S_k, k)$ around $S_{k-1}$ and $k - 1$ : 

same, but the meaning of the equality sign would change. The equality would have to be interpreted in the context of mean square convergence. We apply the Taylor series formula to $F(S_k, k)$ , $k = 1, 2, \ldots$ , where the $S_k$ is assumed to obey 

$^{3}$ Here, it should not be forgotten that the function $g(\Delta W_{k}, h)$ depends on powers of $\Delta W_{k}$ , and that these also determine whether the ratio in (23) becomes negligible as h gets smaller. Such is the case when we deal with cross-product terms of Taylor series expansions. 

The following discussion uses this convention in deciding which terms of a stochastic Taylor series expansion can be considered small. 

This convention amounts to comparing various terms with h. In particular, if the mean square limit of the function $g(\Delta W_{k}, h)$ is proportional to $h'$ with r > 1, it will go toward zero faster than h (i.e., the square of a small number is smaller than the number itself). On the other hand, if r < 1, then the mean square limit of $g(\Delta W_{k}, h)$ will be proportional to a larger power of h than h itself. $^{3}$ 

If this ratio vanishes (in the m.s. sense) as $h \to 0$ , then we consider $g(\Delta W_k, h)$ as negligible in small intervals. Otherwise, $g(\Delta W_k, h)$ is non-negligible. 

CONVENTION: Given a function $g(\Delta W_{k}, h)$ dependent on the increments of the Wiener process $W_{t}$ , and on the time increment, consider the ratio 

Given that the terms of size $h$ are of first order, and that these are by convention not small, the following rule will be used to distinguish negligible terms from nonnegligible ones. 

$\Delta S_{t}$ is random, its variance will be positive. But variance is the “size” of a typical $(\Delta S_{t})^{2}$ . Hence, on average, assuming that $(\Delta S_{t})^{2}$ is negligible will be equivalent to assuming that its variance is approximately zero—that $S_{t}$ is, approximately, not random. This is a contradiction, and it defeats the purpose of using SDEs in markets for derivative products. After all, the objective is to price risk, and risk is generated by unexpected news.

Hence, in contrast to deterministic environments, terms such as $(\Delta S_{k})^{2}$ cannot be ignored in stochastic differentiation. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/f7aa3559270ff8750ad6ec8fec79d49e748d2f151b8ab7714f4d20913061b11c.jpg)


Hence, terms involving $dS_{i}^{2}$ are likely to have sizes of order dt, which was considered as nonnegligible. If terms involving dt are preserved in Taylor approximations, the same must apply to squares of stochastic differentials. We further emphasize this important point. If $\Delta S_{i}$ is a random increment with mean zero, then $E[\Delta S_{i}]^{2}$ will be the variance of this increment. Since 

To see why such a convention makes sense, note that as $\Delta S$ gets smaller, terms such as $(\Delta S)^2$ , $(\Delta S)^3$ , ..., get small faster. This is shown in Figure 1, where the functions 

As long as the processes under consideration are continuous and do not display any jumps, terms involving cross products of $\Delta W_{k}$ and h would be negligible, according to the convention adopted earlier. 

The right-hand side of (35) depends on $\Delta W_{k}$ . As $h \rightarrow 0$ , $\Delta W_{k}$ goes to zero. In particular, $\Delta W_{k}$ becomes negligible, because as $h \rightarrow 0$ its variance $v_{k}^{2}h$ goes to zero. That is, $W_{k}$ does not change at the limit h = 0. This is another way of saying that the Wiener process has continuous sample paths. 

The terms in (24) involving cross products are also negligible in small intervals, under the assumption that the unpredictable components do not contain any "jumps." The argument rests on the continuity of the sample paths for $S_{i}$ . Consider the full probability of $S_{i}$ is a result of 10% of the total 

Thus, $\Delta W_k^2$ is a term that cannot be considered negligible, since by definition, we are dealing with stochastic $S_{k}$ , and the nonzero variance of $\Delta S_{k}$ implies: 

In this equation, the first term is "small." The numerator contains a power of $h$ greater than one, and the term is not random. The third term is also "small." It involves a cross product (sec next section). The second term, on the other hand, contains the random variable $(\Delta W_k)^2$ . This is the 

Here, the terms that contain $h$ or $\Delta S_k$ are clearly first-order increments that are not negligible. As $F_s[a_k h + \Delta W_k]$ or $F_t h$ are divided by $h$ , and $h$ is made smaller and smaller, these terms do not vanish. For example, the ratios 

5.1.1 Example 1
Consider a function of the standard Wiener process $W_{i}$ given by 

A discussion of some simple examples may be useful in getting familiar with the terms introduced by Ito's formula. 

We give some simple examples of these uses of Ito's Lemma. More substantial examples will be seen in later chapters when derivative asset pricing is discussed. 

The second use of Ito's Lemma is quite different. Ito's Lemma is useful in evaluating Ito integrals. This may be unexpected, because Ito's formula was introduced as a tool to deal with stochastic differentials. Under normal circumstances, one would not expect such a formula to be of much use in evaluating Ito integrals. Yet stochastic calculus is different. It is not like ordinary calculus, where integral and derivative are separately defined and then related by the fundamental theorem of calculus. As we pointed out earlier, the differential notation of stochastic calculus is a shorthand for stochastic integrals. Thus, it is not surprising that Ito's Lemma is useful for evaluating stochastic integrals. 

(39) 

If one has an exact formula for $F(S_{1}, t)$ , one can then take the partial derivatives explicitly and replace them in the foregoing formula to get the stochastic differential, $dF(S_{1}, t)$ . Later in this section, we give some examples of this use of Ito's Lemma. 

The first use of Ito's Lemma was just mentioned. The formula provides a tool for obtaining stochastic differentials for functions of random processes. For example, we may want to know what happens to the price of an option if the underlying asset's price changes. Letting $F(S_{t}, t)$ be the option price, and $S_{t}$ the underlying asset's price, we can write 

$^{4}$ With this we mean that the drift and diffusion parameters are not too irregular. Square integrability would satisfy this condition. For notational simplicity, we write $a(S_{t}, t)$ as $a_{t}$ and $\sigma(S_{t}, t)$ as $\sigma_{t}$ . 

there are underlying derivatives (e.g. Ito's formula is clearly a very useful tool to have in dealing with financial derivatives. The latter are contracts written on underlying assets. Using the Ito formula, we can determine the SDE for financial derivatives once we are given the SDE for the underlying asset. For a market participant who wants to price a derivative asset but is willing to take the behavior of the underlying asset's price as exogenous, Ito's formula is a necessary tool. 

Thus, the Ito formula can be seen as a vehicle that takes the SDE for $S_{i}^{2}$ and determines the SDE that corresponds to $F(S_{i}, t)$ . In fact, Eq. (37) is a stochastic differential equation for $F(S_{i}, t)$ . 

$$
d F _ {t} = \frac {\partial F}{\partial S _ {t}} d S _ {t} + \frac {\partial F}{\partial t} d t + \frac {1}{2} \frac {\partial^ {2} F}{\partial S _ {t} ^ {2}} \sigma_ {t} ^ {2} d t,
$$

## 4 The Ito Formula

All the terms in the remainder R contain powers of h and of $\Delta W_{k}$ greater than 2. According to the convention adopted earlier, if the unpredictable shocks are of “normal” type—i.e., there are no “rare events”—powers of $\Delta W_{k}$ greater than two will be negligible. In fact, it was shown in Chapter 8 that continuous martingales and Wiener processes have higher-order moments that are negligible as $h \rightarrow 0$ . 

In Chapter 9, this integral was evaluated directly by taking the mean square limit of some approximating sums. That evaluation used straightforward but lengthy calculations. We now exploit Ito's Lemma in evaluating the same integral in a few steps.
Define 

$$
F (W _ {t}, t) = \int_ {0} ^ {t} W _ {s} d W _ {s} + \frac {1}{2} \int_ {0} ^ {t} d s,
$$

$$
\int_ {0} ^ {t} w _ {s} d W _ {s} = \frac {1}{2} W _ {t} ^ {2} - \frac {1}{2} t,
$$

1. We guessed a form for the function $F(W_t, t)$ .
2. Ito's Lemma was used to obtain the SDE for $F(W_t, t)$ .
3. We applied the integral operator to both sides of this new SDE, and obtained an integral equation. This equation contained integrals that were simpler to evaluate than the original integral.
4. Rearranging the integral equation gave us the desired result. 

We now extend the Ito formula to a multivariate framework and give an example. For simplicity, we pick the bivariate case and hope that the reader can readily extend the formula to higher-order systems. 

The second generalization is more complex. One may argue that financial markets are affected by rare events, and that it is inappropriate to consider error terms made of Wiener processes only. One may want to add jump processes to the SDEs that drive asset prices. The corresponding Ito formula would clearly change. This is the second generalization that we discuss in this section. 

We can visualize two circumstances where this model may not apply. Under some conditions, the function $F(.)$ may depend on more than a single stochastic variable $S_t$ . Then a multivariate version of the Ito formula needs to be used. The extension is straightforward, but it is best to discuss it briefly. 

Ito's formula is seen as a way of obtaining the SDE for a function $F(S_t, t)$ , given the SDE for the underlying process $S_t$ . Such a tool is very useful when $F(S_t, t)$ is the price of a financial derivative and $S_t$ is the underlying asset. But the Ito formula introduced thus far may end up not being sufficiently general under some plausible circumstances that a practitioner may face in financial markets. 

This equality provides an expression where integrals with respect to Wiener processes or other continuous-time stochastic processes are expressed as a function of integrals with respect to time. It should be kept in mind that in (62) and (64), $F_s$ and $F_{sy}$ depend on $u$ as well. 

5.2.1 Another Example
Suppose we need to evaluate 

The technique is indirect but straightforward. The only difficulty is in guessing the exact form of the function $F(W_t, t)$ . This technique of using Ito's Lemma in evaluating integrals will be exploited in the next chapter. 

7.1.1 An Example from Financial Derivatives
Options written on bonds are among the most popular interest rate derivatives. In valuing these derivatives, the yield curve plays a fundamental role. One class of models of interest rate options assumes that the yield curve depends on two state variables, $r_{t}$ representing a short rate and $R_{t}$ representing a long rate. The price of the interest rate derivative will then be denoted by $F(r_{t}, R_{t}, t), t \in [0, T]$ .
These interest rates are assumed to follow the following SDEs: 

the existence of cross products such as $dW_{1}(t)dW_{2}(t)$ .⁸ Here we have the product of the increments of two independent Wiener processes. Over a finite interval $\Delta$ , we expect 

$^{6}$ There is a slight change in the notation dealing with the time variable t. $^{7}$ In the following equation we write the stochastic differentials without showing their dependence on t. 

where the squared differentials $[dS_{1}]^{2}$ , $[dS_{2}]^{2}$ and the cross-product term $dS_{1}dS_{2}$ need to be equated to their mean square limits. We already know that $dt^{2}$ and cross products such as $ddW_{1}(t)$ and $dtdW_{2}(t)$ are equal to zero in the mean square sense. This point was discussed in obtaining the univariate Ito's Lemma. The only novelty now is 

In this bivariate framework, $S_{1}(t), S_{2}(t)$ represent two stochastic processes that are influenced by the same Wiener components. Because the parameters $\sigma_{ij}(t)$ may differ across equations, error terms affecting the two equations may not be identical. Yet, because the $S_{1}(t), S_{2}(t)$ have common error components, they will in general be correlated, except for the special case when 

(84) 

where $\alpha_{t}$ is a drift coefficient of the continuous movements in $S_{t}$ . It is worth discussing one aspect of the jump process again. The process has two sources of randomness. The occurrence of a jump is a random 

Under these conditions, the drift coefficient $a_{t}$ can be seen as representing the sum of two separate drifts, one belonging to the Wiener continuous component, the other to the pure jumps in $S_{t}$ , 

where $N_{t}$ is a process that represents the sum of all jumps up to time t. More precisely, $\Delta N_{t}$ will have a value of $a_{i}$ if there was a jump during the h, and if the value of the jump was given by $a_{i}$ . The term $(\sum_{i=1}^{k}a_{i}p_{i})$ is the expected size of a jump, whereas $\lambda_{i}h$ represents, loosely speaking, the probability that a jump will occur. These are subtracted from $\Delta N_{t}$ to make $\Delta J_{t}$ unpredictable. 

$^{10}$ In the case of the standard Poisson process, all jumps have size 1. This step is thus redundant. 

(83) 

249 

We assume the following structure for the jumps. Between jumps, $J_{i}$ remains constant. At jump times $\tau_{j}, j = 1,2,\dots$ , it varies by some discrete and random amount. We assume that there are $k$ possible types of jumps, with sizes $\{a_i,i = 1,\dots ,k\}$ . The jumps occur at a rate $\lambda_{i}$ that may depend on the latest observed $S_{i}$ . Once a jump occurs, the jump type is selected randomly and independently. The probability that a jump of size $a_{i}$ will occur is given by $p_{i}^{10}$ . 

We need to make this assumption, since this term is part of the unpredictable innovation terms. This assumption is not restrictive, as any predictable part of the jumps may be included in the drift component $a$ . We assume the following structure for the jumps. Between jumps, $J$ . 

where $dW_{i}$ is a standard Wiener process. The new term $dJ_{i}$ represents possible unanticipated jumps. This jump component has zero mean during a finite interval h: 

Thus far, the underlying process $S_{i}$ was always assumed to be a function of random shocks representable by Wiener processes. This assumption may be too restrictive. There may be a jump component to random errors as well. In this section, we provide this extension of the Ito formula. 

7.1.2 Wealth
An investor buys $N_{i}(t)$ units of the ith asset at a price $P_{i}(t)$ . There are n assets, and both the $N_{i}(t)$ and $P_{i}(t)$ are continuous-time stochastic processes, potentially a function of the same random shocks.
The total value of the investment is given by the wealth $Y(t)$ at time t: 

The stochastic differential $dF_{t}$ would measure how the price of an interest rate derivative will change during a small interval dt, and given a small variation in the yield curve, the latter being caused by $dr_{t}$ and $dR_{t}$ . 

and long rates.
In valuing these interest rate options, one may want to know how the option price reacts to small changes in the yield curve, that is, to $dR_{t}$ and $dR_{t}$ . In other words, one needs the stochastic differential $dF_{t}$ . Here the multivariate form of the Ito formula must be used: $^{9}$ 

The market participant can select the parameters $\sigma_{ij}(t)$ so that the equations capture the correlation and volatility properties of the observed short and long rates. 

(a) Calculate $dS_{i}$ .
(b) What is the “expected rate of change” of $S_{i}$ ?
(c) If the exponential term in the definition of $S_{i}$ did not contain the $\frac{1}{2}\sigma^{2}t$ term, what would be the $dS_{i}$ ? What would then be the expected change in $S_{i}$ ? 

2. Supposc the $W_{it}$ , $i = 1,2$ are two Wiener processes. Use Ito's Lemma in obtaining appropriate stochastic differential equations for the following transformations. 

The sources recommended for Chapter 9 also apply here. Ito's Lemma and the Ito integral are two topics that are always treated together. One additional source the reader may appreciate is the book by Kushner (1995), which provides several examples of Ito's Lemma with jump processes. 

Finally, from a practical point of view, the reader should remember that standard formulas used in deterministic calculus give significantly different results than the Ito formula. In particular, if one uses standard formulas, this would amount to assuming that all processes under observation have zero infinitesimal volatility. This is not a pleasant assumption when one is trying to price risk using financial derivatives. 

Ito's Lemma is the central differentiation tool in stochastic calculus. There are a few basic things to remember. First, the formula helps to determine stochastic differentials for financial derivatives given movements in the underlying asset. Second, the formula is completely dependent on the definition of the Ito integral. This means that equalities should be interpreted within stochastic equivalence. 

That is, it is the value of S at an infinitesimal time before t. How would one calculate the $dJ_{F}$ in practice? One would first evaluate the expected change due to possible random jumps, which is the second term on the right-hand side of Eq. (86). To do this, one uses both the rate of possible jumps occurring during dt and the expected size of jump in $F(\cdot)$ caused by jumps in $S_{t}$ . If during that particular time a jump is observed, then the first term on the right-hand side is also included. Otherwise, the term will equal zero. 

event. But once the jump occurs, the size of the jump is also random. Moreover, the structure just given assumes that these two sources of randomness are independent of each other.
Under these conditions, the lto formula is given by were allowed to depend on $S_t$ and $t$ . Hence, these parameters are themselves random variables. The point is that given the information at time $t$ , they are observed by the market participant. Conditional on available information, they "become" constant. This is the consequence of the important assumption that these parameters are $I_t$ -adapted. At several points 

$dS_{t} = a(S_{t}, t)dt + \sigma(S_{t}, t)dW_{t},\quad t\in [0,\infty),$ 

The SDEs are utilized in pricing derivative assets because they give us a formal model of how an underlying asset's price changes over time. But it is also true that the formal derivation of SDEs is compatible with the way dealers behave in financial markets. In fact, on a given trading day, a trader continuously tries to forecast the price of an asset and record the "new events" as time passes. These events always contain some parts that are unpredictable until one observes the $dS_{t}$ . After that, they become known and become part of the new information set the trader possesses. This chapter considers some properties of stochastic differential equa than $aW_{t}$ : In stochastic calculus, this property of $W_{t}$ is formally summarized by saying that the Wiener process $W_{t}$ is adapted to the family of information sets $I_{t}$ . 

In these two equations the drift and the diffusion terms cannot be the same. The error terms that drive the SDEs are different, which makes $a^{*}(S_{i},t)$ different from $a(S_{i},t)$ . This example shows that the exact form of the SDE, and hence the definition of the error term $dW_{i}$ , always depends on the family of information sets $\{I_i,t\in [0,T]\}$ . If we had access to a different family of information sets, we would make different prediction errors, and the probabilistic behavior of the error terms would change. Given a different family of information sets $I_{i}^{*}$ , we may have to denote the errors by $dW_{i}^{*}$ instead of $dW_{i}$ . It may be that $dW_{i}^{*}$ has a smaller variance than $dW_{i}$ . 

$dS_{t} = a^{*}(S_{t},t)dt,$ 

variable perfectly, and $dW_{t}=0$ for all t. If we were to write this participant's SDE we would get random price into predictable and unpredictable components.

This brings us to another point. Given that the decomposition in Eq. (1) is done using the information set available at time t, then to the extent different players may have access to different sets of information, the SDE in (1) may also be different. For example, consider the following extreme case. Suppose a market participant has “inside information” and learns all the random events that influence price changes in advance. Under these (unrealistic) conditions, the diffusion term in (1) would be zero. Since the participant knows how $dS_{t}$ is going to change, he or she can predict this 

when $h$ is infinitesimal. We repeat some aspects of this derivation. First of all, no concept from financial markets or financial theory was used to obtain (1). The basic tools used were the Ito integral and the ability to split some increment in a random price into predictable and unpredictable components. This brings us to another point. Given that the decomposition in Eq. 

The concept of a stochastic differential equation (SDE) was introduced in Chapter 7. In Chapter 9 we used the Ito integral to formalize this concept. The notation 

Stochastic Differential Equations 

## The Dynamics of Derivative Prices

## CHAPTER II

The solution to this equation is a random process $S_{k}$ . We are interested in finding a sequence of random variables indexed by $k$ , such that the increments $\Delta S_{k}$ satisfy (7). Moreover, we would like to know the moments and the distribution function of a process $S_{k}$ that satisfies Eq. (7). At the outset, it is not clear that, given a particular $a(\cdot)$ and $\sigma(\cdot)$ , we could find a sequence of random numbers whose trajectories will satisfy the equality in (7) for all $k$ . 

3.1 What Does a Solution Mean?
First, consider the finite difference approximation in small, discrete intervals: 

A stochastic differential equation is by definition an equation. That is, it contains an unknown. This unknown is the stochastic process $S_{i}$ . The notion of a solution to an SDE is thus more complicated than it may seem at the outset. What we are searching for is not a number or vector of numbers. It is a random process whose trajectories and the probabilities associated with those trajectories need to be determined exactly. 

“Orthogonal” here implies “uncorrelated.” 

by the heavy line. This geometric derivation emphasizes once again that the trajectories of $S_{t}$ are likely to be very erratic when $h$ becomes infinitesimal. 

ascribe $S_{i}$ and (possession) on $h$ . What type of geometric behavior would such an SDE imply for $S_{i}$ ? An example is shown in Figure 1. We consider small but discrete intervals of length $h$ . We see that over time, the behavior of $S_{i}$ can be decomposed into two types of movements. First, there is an expected path during the interval. These are indicated by upward- or downward-sloping arrows. Then, at each $t_{k} = kh$ , there is a second movement orthogonal to the predicted changes. These are represented by vertical arrows. Sometimes they are negative; other times they are positive. The actual movement of $S_{i}$ over time is determined by the sum of these two components and is indicated by the heavy line. 

during the previous chapters, we made assumptions suggesting that these parameters should be well behaved.
It is customary to specify these “regularity conditions” each time an SDE is proposed as a model.
The $a(S_{t}, t)$ and $\sigma(S_{t}, t)$ parameters are assumed to satisfy the condi-

$^{3}$ As mentioned earlier, mathematicians call such information sets $\sigma$ -field or $\sigma$ -algebra. $^{4}$ Because of this martingale property, the Ito integrals that are in the background of SDEs can still be defined the same way. 

$^{2}$ As we see in Chapter 14, the two Wiener processes may imply different probability measures on $dS_{T}$ . 

The weak solution $\tilde{S}_t$ , on the other hand, is not calculated using the process that generates the information set $I_t$ . Instead, it is found along with some process $\tilde{W}_t$ . The process $\tilde{W}_t$ could generate some other information set $H_t$ . The corresponding $\tilde{S}_t$ will not necessarily be $I_t$ -adapted. But $\tilde{W}_t$ will still be a martingale with respect to histories $H_t^{4}$ . 

The strong solution then calculates an $S_{t}$ that satisfies Eq. (13) with $dW_{t}$ given. That is, in order to obtain the strong solution $S_{t}$ , we need to know the family $I_{t}$ . This means that the strong solution $S_{t}$ will be $I_{t}$ -adapted. 

Heuristically, the error process $dW_{t}$ symbolizes infinitesimal events that affect prices in a completely unpredictable fashion. The “history” generated by such infinitesimal events is the set of information that we have at time t. This we denoted by $I_{t}^{3}$ . 

This has to be made more precise because it re-emphasizes an important point made earlier—a point that needs to be clarified in order for the reader to understand the structure of continuous-time stochastic models. Consider the following SDE, where the diffusion term contains the exogenously given $dW_{i}$ : 

with zero mean and variance $dt$ ? Are these not the same object?

If looked at in terms of the form of distribution functions, this is a valid question. The density functions of $dW_t$ and $d\tilde{W}_t$ are given by the same formula. In this sense, there is no difference between the two random errors. The difference will be in the sequence of information sets that define $dW_t$ and $d\tilde{W}_t$ . Although the underlying densities may be the same, the two random processes could indeed represent very different real-life phenomena if they are measurable with respect to different information sets. 

argue that finding an $\tilde{S}_t$ and a $\bar{W}_t$ , such that the pair $\{\tilde{S}_t, \bar{W}_t\}$ satisfies this equation, is also a type of solution to the stochastic differential equation. In this type of solution, we are given the drift parameter $a(S_t, t)$ and the diffusion parameter $\sigma(S_t, t)$ . We then find the processes $\tilde{S}_t$ and $\bar{W}_t$ such that Eq. (8) is satisfied. This is in contrast to strong solutions where one does not solve for the $W_t$ , but considers it another given of the problem. Clearly there are some potentially confusing points here. First of all 

The idea of a weak solution can be explained as follows. Given that solving SDEs involves finding random variables that satisfy Eq. (8), one can 

where $\tilde{W}_i$ is a Wiener process whose distribution is determined simultaneously with $\bar{S}_i$ . According to this, for the weak solution of SDEs, the "givens" of the problems are only the drift and diffusion parameters, $a(\cdot)$ and $\sigma(\cdot)$ , respectively. 

The second solution concept is specific to stochastic differential equations. It is called the weak solution. In the weak solution, one determines the process $\tilde{S}_i$ . 

for all $t > 0$ . The solution determines the exact form of this dependence. When $W_t$ on the right-hand side of (8) is given exogenously and $S_t$ is then determined, we obtain the so-called strong solution of the SDE. This is similar to solutions of ordinary differential equations. 

Clearly, such a solution $S_{t}$ will depend on time t, and on the past and contemporaneous values of the random variable $W_{t}$ , as the underlying integral equation illustrates: 

The first type of solution to an SDE is similar to the case of ordinary differential equations. Given the drift and diffusion parameters and the random innovation term $dW_{t}$ , we determine a random process $S_{t}$ , paths of which satisfy the SDE: 

Because the solutions of SDEs are random processes, the nature of these solutions could be quite different when compared with ordinary differential equations. In fact, in stochastic calculus, there can be two types of solutions. 

More importantly, our purpose is to look for this solution when $h$ , the interval length, goes to zero. If a continuous time process $S_t$ satisfies the equation 

(16) 

Hence, the candidate solution satisfies the initial condition as well. We thus say that $X_{t}$ solves the ODE in (16). This method verified the solution using the concept of derivative. $^{6}$ where $a$ is a constant and $X_0$ is given. There is no random innovation term; this is not a stochastic differential equation. A candidate for the solution can be verified directly. For example, suppose it is suspected that the function 

If there is no differentiation theory of continuous stochastic processes, a similar approach cannot be utilized in verifying solutions of SDEs. In fact, if one uses the same differentiation methodology, assuming (mistakenly) that it holds in stochastic environments, and tries to "verify" solutions to SDEs by taking derivatives, one would get the wrong answer. As seen earlier, the rules of differentiation that hold for deterministic functions are not valid for functions of random variables. 

The process of verifying solutions to SDEs can best be understood if we start with a deterministic example. Consider the simple ordinary differential equation 

is a solution of (16). Then, the solution must satisfy two conditions. First, if we take the derivative of $X_{t}$ with respect to t, this derivative must equal a times the function itself. Second, when evaluated at t = 0, the function should give a value equal to $X_{0}$ , the initial point, which is assumed to be known. 

$^{6}$ Of course, the reader may wonder how the candidate solution was obtained to begin with. This topic belongs to texts on differential equations. Here, we just deal with models routinely used in finance. 

This approach verifies the solution using the corresponding integral equation rather than using the SDE directly. Why is this so? Note that according to the discussion up to this point, we do not have a theory of differentiation in stochastic environments. Hence, if we have a candidate for a solution of an SDE, we cannot take derivatives and see if the corresponding derivatives satisfy the SDE. Two alternative routes exist. 

is valid for all $t$ . In other words, the evolution of $S_t$ , starting from an initial point $S_0$ , is determined by the two integrals on the right-hand side. The solution process $S_t$ must be such that when these integrals are added together, they should yield the increment $S_t - S_0$ . This would verify the solution. 

The stochastic differential equation is, as mentioned earlier, an equation. This means that it contains an unknown that has to be solved for. In the case of SDEs, the “unknown” under consideration is a stochastic process. By solving an SDE, we mean determining a process $S_{t}$ such that the integral equation 

Note that this solution candidate is indeed a function of the parameters $a$ and $\sigma$ , of time $t$ , and of the random variable $W_t$ . Clearly, we are dealing with a strong solution, since $S_t$ depends on $W_t$ and is $I_t$ -adapted. How do we verify that this function is indeed a solution? 

$^{8}$ It is important to keep in mind that the SDE discussed above is a special case. In general, the strong solution $S_{i}$ shown in (23) will depend on the integrals of $a(S_{u}, u)$ , $\sigma(S_{u}, u)$ , and $dW_{u}$ . Hence, the dependence will be on the whole trajectory of $W_{r}$ . 

Instead, one should consider a candidate solution, and then, using Ito's Lemma, try to see if this candidate satisfies the SDE or the corresponding integral equation. In the example below, we consider this point in detail. 

Using deterministic differentiation formulas to check whether this $f(\cdot)$ satisfies the SDE in (22) means taking the derivatives of $S_t$ and $W_t$ with respect to $t$ . But these derivatives with respect to $t$ are not well defined. Hence, the solution cannot be verified by using the same methodology as in the deterministic case. 

with $X_{0}$ given, both sides of the equation contain terms in the unknown function $X_{t}$ . That is why the ODE is an equation. The solution of the equation is then a specific function that depends on the remaining parameters and known variables in the ODE. The parameters are $\{a, X_{0}\}$ , and the only known variable is the time t. Hence, the solution expresses the unknown function $X_{t}$ as a function of the known quantities: 

The idea behind the second method is to transform this nonlinear expression in $W_{i}$ into a linear one, and then take the expectations directly without having to use the density function of the Wiener process. The method is indirect, but fairly simple. First, denote the nonlinear random term in Eq. (35) by $Z_{i}$ . 

$$
E _ {i} [ e ^ {\sigma W _ {T}} ] = \int_ {- \infty} ^ {\infty} e ^ {\sigma W _ {T}} [ f (W _ {T} | W _ {i}) ] d W _ {T},
$$

where, for future reference, the expression is a nonlinear function of $W_{T}$ . Hence, the $S_{T}$ is a nonlinear function of $W_{T}$ as well. This means that in taking the expectation $E_{i}[S_{T}]$ , we cannot “move” the $E_{i}[\cdot]$ operator in front of the random term $W_{T}$ . 

This would make the current price equal to the expected price at time T discounted at a rate r. This martingale property is of interest because it can be exploited to calculate the current price $S_{r}$ . We now calculate $E_{r}[S_{T}]$ . The first step is to realize the following: 

Now, suppose $S_{T}$ is the price at some future time T > t. As of time t, this $S_{T}$ is unknown. But it can be predicted, and the best prediction will be given by the conditional expectation: 

which is the original SDE with $a$ equal to $\mu$ . It is interesting to note that the terms $\frac{1}{2}\sigma^2 dt$ are eliminated by the application of Ito's Lemma. If the rules of deterministic differentiation were used, these terms would not disappear in Eq. (32), and the function in (30) would not verify the SDE. In fact, if we had used ordinary calculus, total differentiation would instead give 

where the very last term on the right-hand side corresponds to the second-order term in Ito's Lemma. Canceling similar terms and replacing by $S_{t}$ , we obtain 

Hence, the drift and the diffusion coefficients depend on the information that becomes available at time t. However, this dependence is rather 

This suggests when such a stochastic differential equation is appropriate in practice. In particular, this SDE will be a good approximation if the behavior of the asset prices is stable over time, if the “trend” is linear and if the “variations” do not get any larger. Finally, it will be a good approximation if there do not appear to be systematic “jumps” in asset prices. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/f053fd1e4a19ff83678e88f9e0bbebdab848d2749dc8d15cad9589f8158f17a1.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/48a8b26045b237a4f99c81cde55da623476af67192ca5797ce7c8b5c03a02c70.jpg)


where the drift and diffusion coefficients are as in the case of Figure 3, but where the diffusion is now proportional to $\sqrt{S_t}$ instead of being proportional to $S_{t}$ . We select the initial point as $S_0 = 100$ . Clearly, the fluctuations in Figure 4 are more subdued than the ones in Figure 3, yet the sample paths have "similar" trends. 

As an example we provide, in Figure 4, the sample path obtained from the same $dW_{t}$ terms used to generate Figure 3. We consider the equation 

(72) 

Hence, the variance increases in a way proportional to the square of $S_{t}$ . In some practical cases, this may add too much variation to $S_{t}$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/e771e23ac655a250956ddb0d81f976250c8776cb2ba9bea7c5063d069cb0b64d.jpg)


But this says nothing about the assumption concerning the diffusion coefficient. Is a diffusion coefficient proportional to $S_{t}$ more realistic as well? To answer this, we note that the “variance” of an incremental change in $S_{t}$ between times $t_{k}$ and $t_{k-1}$ could be approximated by 

with the initial point $S_0 = 100$ . As can be seen from this graph, the $S_l$ is made of two components. First, there is an exponential trend that grows at $15\%$ . Second, there are random fluctuations around this trend. These variations increase over time because of higher prices. What is the empirical relevance of this model when compared with con-

This means that although the drift and the diffusion part of the increment in asset price changes, the drift and diffusion of percentage change in $S_{t}$ still has time invariant parameters. 

straightforward. The drift and the standard deviation change proportionally with $S_{t}$ . In fact, dividing both sides by $S_{t}$ , we obtain 

A much more general SDE can be obtained by making the drift and the diffusion parameters random. In the case of financial derivatives, this may 

All previous examples of SDEs consisted of modeling the drift and diffusion parameters of SDEs in some convenient fashion. The simplest case showed constant drift and diffusion. The most complicated case was the mean reverting process. 

This model can be used to represent asset prices that fluctuate around zero. The fluctuations can be in the form of excursions, which eventually revert to the long-run mean of zero. The parameter $\mu$ controls how long excursions away from this mean will take. The larger the $\mu$ , the faster the $S_{t}$ will go back toward the mean. 

where $\mu > 0$ . Here the drift depends on $S_{t}$ negatively through the parameter $\mu$ , and the diffusion term is of the constant parameter type. Obviously, this is a special case of “mean reverting SDE.” This model can be used to represent next priors that generate 

The trajectory is shown in Figure 5. Because the diffusion term does not depend on $S_{p}$ , in this particular case, the process may become negative. 

$^{11}$ This is often used to model interest rate dynamics. 

This implies a long-run mean of 5% and a volatility of 80% during a time interval of length 1. The $\lambda$ implies an adjustment of 50%. We then selected the length of finite subintervals as h = .001. According to this, during a time interval of length 1, we will observe 1000 $S_{t}$ 's. Random numbers with mean zero and variance .001 were obtained, and the sample path was generated by using the increments 

the two previous models.
The mean reverting process has a trend, but the deviations around this trend are not completely random. The process $S_{t}$ can take an excursion away from the long-run trend. It eventually reverts to that trend, but the excursion may take some time. The average length of these excursions is controlled by the parameter $\lambda > 0$ . As this parameter becomes smaller, the excursions take longer. Thus, asset prices may exhibit some predictable periodicities. This usually makes the model inconsistent with market efficiency. An example of a sample path of a mean reverting process is shown in 

Finally, another characteristic of this process is the meaning of the parameter $\sigma$ . Note that with this specification of the diffusion component, $\sigma$ cannot be interpreted as percentage volatility of $S_{r}$ . Markets, on the other hand, quote by convention the percentage volatility of underlying assets. 

with $S_{0}=1$ given.
Suppose a European call option with expiration T=1 and strike K=1.5 is written on this security. Assume that the risk-free interest rate is 3%. 

3. Consider the linear SDE that represents the dynamics of a security price: 

It is known that the annual percentage volatility is 0.15. The risk-free interest rate is constant at 5%. Also, as is the case in practice, the effect of dividends is eliminated in calculating this index. Your interest is confined to an 8-day period. You do not see any harm in dividing this horizon into four consecutive 2-day intervals denoted by $\Delta$ . 

In this chapter, we followed the treatment of Oksendal (1992), which has several other examples of SDEs. An applications-minded reader will also benefit from having access to the literature on the numerical solution of SDEs. The book by Kloeden, Platen, and Schurz (1994) is both very accessible and comprehensive. It may very well be said that the best way to understand SDEs is to work with their numerical solutions. 

## 7 References

This chapter introduced the notion of solutions for SDEs. We distinguished between two types of solutions. The strong solution is similar to the case of ordinary differential equations. The weak solution is novel. We did not discuss the weak solution in detail here. An important exam-

## 6 Conclusions

of the shocks to asset prices by. The $\alpha > 0$ is a parameter.
The market participant has to calculate predictions for asset prices and
for volatility. Using such layers of SDEs, one can obtain more complicated
models for representing real life, financial phenomena. On the other hand,
stochastic volatility adds additional diffusion components and possibly new
risks to be hedged. This may lead to models that are not “complete.” 

where the Wiener processes $W_{1t}$ , $W_{2t}$ may very well be dependent. Note what Eq. (80) says about the volatility. The volatility of the asset has a long-run mean of $\sigma_0$ . But at any time $t$ , the actual volatility may deviate from this long-run mean, the adjustment parameter being $\lambda$ . The increments $dW_{2t}$ are unpredictable shocks to volatility that are independent of the shocks to asset prices $S_t$ . The $\alpha > 0$ is a parameter. 

where the drift parameter is constant, while the diffusion parameter is assumed to change over time. More specifically, $\sigma_{t}$ is assumed to change according to another SDE, 

have some interesting applications, because it implies that the volatility may be considered not only time-varying, but also random given the $S_{t}$ . For example, consider the SDE for an asset price $S_{t}$ , 

First, we will briefly discuss the logic behind the method of pricing securities that leads to the use of PDEs. These results will be utilized in Chapter 13. 

Modern finance has developed two major methods of pricing derivative products. The first of these leads to the utilization of partial differential equations, which are the subject of this chapter. The second requires transforming underlying processes into martingales. This necessitates utilization of equivalent martingale measures, which is the topic of Chapter 14. In principle, both methods should give the same answer. However, depending on the problem at hand, one method may be more convenient or cheaper to use than the other. The mathematical tools behind these two pricing methods are, however, very different. 

These tools were not discussed for their own sake. Rather, they were discussed because of their usefulness in pricing various derivative instruments in financial markets. Far from being mere theoretical developments, these tools are practical methods that can be used by market professionals. In fact, because of some special characteristics of derivative products, abstract theoretical models in this area are much more amenable to practical applications than in other areas of finance. 

Thus far we have learned about major tools for modeling the dynamic behavior of a random process in continuous time, and how one can (and cannot) take derivatives and integrals under these circumstances. 

1 Introduction 

Partial Differential Equations 

# Pricing Derivative Products

## CHAPTER 12

(To generate any needed random variables you can toss a coin.) 

(c) Plot these two realizations.  
(d) How would these graphs look if $\Delta = .01$ ?  
(e) Now multiply the variance of $S_{t}$ by 3, let $dt = 1$ , and obtain a new realization for $S$ 

$\Delta W_{t} = \left\{ \begin{array}{ll} + \Delta & \text{with probability .5} \\ -\Delta & \text{with probability .5.} \end{array} \right.$ 

Suppose $dW_{t}$ is approximated by the following process: 

$dS_{t} = .05dt + .1dW_{t}$ 

4. Consider the SDE: 

(a) Using your computer, generate five normally distributed random variables with mean zero and variance $\sqrt{2}$ .  
(b) Obtain one simulated trajectory for the $S_{t}$ . Choose $\Delta t = .2$ .  
(c) Determine the value of the call at expiration.  
(d) Now repeat the same experiment with five uniformly distributed random numbers with appropriate mean and variances.  
(c) If we conducted the same experiment 1000 times would the calculated price differ significantly in two cases? Why?  
(f) Can we combine the two Monte Carlo samples and calculate the option price using 2000 paths? 

CHAPTER • 11 The Dynamics of Derivative Prices 

participant who selects the portfolio weights $\theta_{1},\theta_{2}$ . Second, the latter can always be set such that the $dP_{t}$ is independent of the innovation term $dW_{t}$ and hence is completely predictable. The reason is as follows. Given that $dF_{t}$ and $dS_{t}$ have the same unpredictable component, and given that $\theta_{1},\theta_{2}$ can be set as desired, one can always eliminate the $dW_{t}$ component from Eq. (4). To do this, consider again 

We first see that the SDE in (7) describing the dynamics of $df_{t}$ is driven by the same Wicner increment $dW_{t}$ that drives the $S_{r}$ . One should, in principle, be able to use one of these SDEs to eliminate the randomness in the other. In forming risk-free portfolios, this is in fact what is done. 

$$
d F _ {t} = \left[ F _ {s} a _ {t} + \frac {1}{2} F _ {\mathrm{ss}} \sigma_ {t} ^ {2} + F _ {t} \right] d t + F _ {s} \sigma_ {t} d W _ {t}.
$$

$$
d F _ {t} = F _ {t} d t + \frac {1}{2} F _ {\mathrm{ss}} \sigma_ {t} ^ {2} d t + F _ {s} d S _ {t}.
$$

Our main interest is in the price of the derivative product, and how this price changes. Thus, we begin by positing a model that determines the dynamics of the underlying asset $S_{t}$ , and from there we try to determine how $F(S_{t}, t)$ behaves. Accordingly, we assume that the stochastic differential $dS_{t}$ obeys the SDE 

[An important remark about notation. $dF_{t}$ should again be read as the total change in the derivative price $F(S_{t}, t)$ during an interval $dt$ . This should not be confused with $F_{t}$ , which we reserve for the partial derivative of $F(S_{t}, t)$ with respect to $t$ .] Our main interest is in the price of the derivative product, and how 

$^{1}$ Strictly speaking, this stochastic differential is correct only when the portfolio weights do not depend on $S_{\gamma}$ . Otherwise, there will be further terms on the right. This point will be quite relevant when we discuss the Black-Scholes framework below. 

In general, $\theta_{1},\theta_{2}$ will vary over time and hence will carry a time subscript as well. At this point we ignore such dependence. In this equation, both $dF_{t}$ and $dS_{t}$ are increments that have an unpredictable component due to the innovation term $dW_{t}$ in $dS_{t}$ . 

where $\theta_{1},\theta_{2}$ are the quantities of the derivative instrument and the underlying security purchased. They represent portfolio weights. The value of this portfolio changes as time $t$ passes because of changes in $F(S_t,t)$ and $S_t$ . Taking $\theta_{1},\theta_{2}$ as constant, we can write this change as 

Explanation: This function needs to be found. This suggests that if we have a law of motion for the $S_t$ process—i.e., if we have an equation describing the way $dS_t$ is determined—then we can use Ito's Lemma to obtain $dF_t$ . But this means that $dF_t$ and $dS_t$ would be increments that have the same source of underlying uncertainty, namely the innovation part in $dS_t$ . In other words, at least in the present example, we have two increments, $dF_t$ and $dS_t$ , that depend on one innovation term. Such dependence makes it possible to form risk-free portfolios in continuous time. 

The increments in this price will be denoted by $dF_t$ . At the outset, a market participant will not know the functional form of $F(S_t, t)$ at times other than expiration. This function needs to be found. 

This implies that at expiration, we know the exact form of the function $F(S_T, T)$ . We assume that the same relationship is true for times other than $T$ , and that the price of the derivative product can be written as 

Derivative instruments are contracts written on other securities, and these contracts have finite maturities. At the time of maturity denoted by T, the price $F_{T}$ of the derivative contract should depend solely on the value of the underlying security $S_{T}$ , the time T, and nothing else: 

This construction of a risk-free portfolio is heuristic. From a mathematical point of view, it is not satisfactory. In a formal approach, one should form self-financing portfolios using completeness of markets with respect to a class of trading strategies and using the implied "synthetic" equivalents of the assets under consideration. Jarrow (1996) is an excellent source on these concepts. Next section discusses this point in more detail. 

The reason this method “works” and eliminates the innovation term from Eq. (4) is that $F(\cdot)$ represents a price of a derivative instrument, and hence has the same inherent unpredictable component $dW_{i}$ as $S_{i}$ . Thus, by combining these two assets, it becomes possible to eliminate their common unpredictable movements. As a result, $P_{i}$ becomes a risk-free investment, since its future path will be known with certainty. 

According to this equation, if at expiration the stock price is below the strike price, $S_{T} - K$ will be negative and the call option will not be exercised. It will be worthless. Otherwise, the option will have a price equal to the differential between the stock and the strike price. 

We have an additional piece of information. The derivative product will have an expiration date T, and the relationship between the price of the underlying asset and that of the derivative asset will, in general, be known exactly at expiration. That is, we know at expiration that the price of the derivative product is given by 

$^{4}$ Note the role of dt. Some infinitesimal time must pass in order to earn interest or receive dividends. If no time passes, regardless of the level of interest rates r, the interest earnings will be zero. The same is true for dividend earnings. 

$^{2}$ Recall that this will be correct mathematically if $\theta_{1}, \theta_{2}$ do not depend on $S_{i}$ . $^{3}$ Note this important point: The value of $\theta_{2}$ set at $-F_{s}$ will vary over time. For nonlinear products such as options, or structures containing options, the $F_{s}$ will be a function of $S_{i}$ . This means that the risk-free portfolio method is not satisfactory mathematically, yet it will give the “correct” PDE. 

which will, in general, not be the case. In order to see this, note that differentiating the Black-Scholes PDE in (17) with respect to $S_{t}$ again, we can write 

where the third derivative of $F$ is there because we are applying Ito's Lemma to the $F$ already differentiated with respect to $S_t$ . After replacing the differential $dS_t$ , and arranging: 

Note that we now have a third term since the $F_{s}$ is dependent on $S_{t}$ , and, hence, is time dependent and stochastic. In general, this term will not vanish. In fact, we can use Ito's Lemma and calculate the $dF_{s}$ , which is a function of $S_{t}$ and $t$ . This is equivalent to taking the stochastic differential of the derivative's DELTA: 

This selection “works” in the sense that it eliminates the “unpredictable” random component and makes the portfolio risk-frec, but unfortunately it also violates the assumption that $\theta_{1}, \theta_{2}$ are constant. In fact, the $\theta_{2}$ is now dependent on $S_{t}$ because, in general, $F_{s}$ is a function of $S_{t}$ and t. Thus, first replacing the $\theta_{1}, \theta_{2}$ with their selected values, and then taking the differential should give a very different result.
Writing the dependence of $F_{s}$ on $S_{t}$ explicitly: 

If there are no boundary conditions, then finding price functions $F(S_t, t)$ that satisfy a given PDE will, in general, not be possible. Further, the fact that derivative products are known functions of the underlying asset at expiration will always yield a boundary condition to a market participant. 

In finance, boundary conditions play a similar role. They represent some contractual clauses of various derivative products. Depending on the product and the problem at hand, boundary conditions may change. The most obvious boundary values are initial or terminal values of derivative contracts. Often, finance theory tells us some plausible conditions that prices of derivative contracts must satisfy at maturity. For example, futures prices and cash prices cannot be (very) different at the delivery date. In the case of options, option prices must satisfy an equation such as (19). In case of a discount bond, the asset price equals 100 at maturity. 

Partial differential equations are obtained by combining various partial derivatives of a function and then setting the combination equal to zero. The boundary conditions are an integral part of such equations. In physics, boundary conditions are initial or terminal states of some physical phenomenon that evolves over time according to the PDE. In finance boundary conditions is similar to the phenomena 

Unlike the usual cases in algebra where equations are solved with respect to some variable or vector $x$ , the unknown in Eq. (29) is in the form of a function. It is not known what type of function $F(S_t, t)$ represents. What is known is that if one takes various partial derivatives of $F(S_t, t)$ and combines them by multiplying by coefficients $a_t$ , the result will equal zero. Also, at time $t = T$ , this function must equal the (known) $G(S_T, T)$ —i.e., it must satisfy the boundary condition.

Hence, in solving PDEs, one tries to find a function whose partial derivatives satisfy Eqs. (29) and (30). 

Since derivative securities are always “derived” from some underlying asset(s), the formation of such arbitrage-free portfolios is in general quite straightforward. On the other hand, the boundary conditions as well as the implied PDEs may get more complicated depending on the derivative product one is working with. But, overall, the method will center on the solution to a PDE. This concept should be discussed in detail. We discuss partial differential equations in several steps. 

In this section, we keep using $S_{i}$ instead of switching to a generic variable $X$ , as is usually done. 

$G(\cdot)$ being a known function. $^{5}$ The method of forming such risk-free portfolios in order to obtain arbitrage-free prices for derivative instruments will always lead to PDEs. 

We rewrite the partial differential equation (17) in a general form, using the shorthand notation $F(S_{i}, t) = F$ , 

## 4 Partial Differential Equations

Thus, in small intervals, the extra cost (gain) associated with the portfolio $P_{t}$ has zero expectation. It is as if, on the average, it is self-financing. But, it is interesting that this “average” is taken with respect to the synthetic risk-neutral measure and not with respect to real-life probability. See Musiela and Rutkowski (1997) for more details. 

$dW^{*} = (\sigma dW_{i} + (\mu - r)dt).$ 

The answer is in the additional term, $S_{i}^{2}F_{ss}(\sigma dW_{i} + (\mu - r))dt$ . This term has nonzero expectation under the true probability $P$ . But once we switch to a risk-free measure $\tilde{P}$ and define a new Wiener process $W_{i}^{*}$ under this probability, we can write: 

Although, formally speaking, the risk-frec portfolio method is not satisfactory and, in general, makes one work with portfolios that require infusions of cash or leave some capital gains, the method still gives us the correct PDE. How can we interpret this result? The answer is in the additional term. $S^2 F_{\alpha}(\sigma dW_+ + (u - r))dt$ . This term 

3.1 An Interpretation 

(38) 

Now, if in addition to (33) we are given some boundary conditions as well, then we can determine the $F(S_t, t)$ precisely. For example, suppose we know that at expiration time $t = 5$ (the boundary for $t$ ) we have 

We again see that $F(S_{t}, t)$ is a plane. But in this case it increases with respect to t, and decreases with respect to $S_{t}$ , the contours are again straight lines. 

The examples of $F(S_t, t)$ given in (36) and (37) are very different-looking functions. Yet they both solve the PDE in (32). This is because Eq. (32) does not contain sufficient information to allow the function $F(S_t, t)$ to be determined precisely. There are uncountably many functions $F(S_t, t)$ whose first partials with respect to $S_t$ and $t$ are equal. 

$F(S_{t},t)=-2S_{t}+2t-4,-10\leq t\leq10,-10\leq S_{t}\leq10.$ (37) 

(34) 

(35) 

Note that in this case $F_{s} = 3$ and $F_{t} = -3$ . Hence, this function satisfies the PDE in (32). This solution is a plane that increases with respect to $S_{t}$ , but decreases with respect to $t$ . 

straight lines with slope $\alpha$ .
Figures 1 and 2 show two examples of $F(S_{t}, t)$ that “solve” the PDE in (32). Figure 1 is the plot of the plane: 

Their sum will equal zero, and this is exactly what the PDE in (32) implies. The solution suggested by the function (33) is a plane in a three-dimensional space. If no boundary conditions are given, this is all we know. We would not be able to determine exactly which plane $F(S_t, t)$ would represent, since we would not be able to pinpoint the values of $\alpha, \beta$ given the information in (33). All we can say is the following: at $t = 0$ , $S_0 = 0$ the intercept will equal $\beta$ . For a fixed $S_t$ , the $F(S_t, t)$ has contours that are straight lines with slope $-\alpha$ . For fixed $t$ , the contours are straight lines with slope $\alpha$ . 

$\frac{\partial F}{\partial t} = -\alpha$ 

5 Classification of PDEs 

In a financial market, there is no compelling reason why such a relationship should exist between the two partial derivatives. But suppose (32) is nevertheless written down and a solution $F(S_t, t)$ is sought. What would this function $F(S_t, t)$ look like? 

According to this PDE, the negative of the partial of $F(\cdot)$ with respect to $t$ is equal to its partial with respect to $S_t$ . If $t$ were to represent time, and $S_t$ were to represent the price of the underlying security, then (32) would mean that the negative of the price change during a small time interval with $S_t$ fixed, equals the price change due to a small movement in the price of the underlying asset when $t$ is fixed. 

$F_{t} + F_{s} = 0, \quad 0 \leq S_{t}, \quad 0 \leq t \leq T.$ 

Consider the PDE for a function $F(S_{t}, t)$ : 

5.1 Example 1: Linear, First-Order PDE 

We encounter in finance are difficult to participate in PDEs. These examples have no direct relevance in finance. Yet they may help establish an intuitive understanding of what PDEs are, and why boundary conditions are important. 

be second-order. Thus far, these classifications are similar to the case of ordinary differential equations. The third type of classification is specific to PDEs. The latter can also be classified as elliptic, parabolic, or hyperbolic. The PDEs we encounter in finance are similar to parabolic PDEs. 

The second type of classification has to do with the order of differentiation. If all partial derivatives in the equation are first-order, then the PDE will also be first-order. If there are cross-partials, or second partials, then the PDE becomes second-order. For nonlinear financial derivatives such as options, or instruments containing options, the resulting PDE will always be second-order. 

One can classify PDEs in several different ways. First of all, PDEs can be linear or nonlinear. This refers to the coefficients applied to partial derivatives in the equation. If an equation is a linear combination of $F$ and its partial derivatives, it is called a linear PDE. $^{6}$ 

5 Classification of PDEs 

To see the role of boundary conditions and to consider some simple PDEs, we look at some examples. 

First note that we are again dealing with a linear PDE, since the partials in question are combined by using constant coefficients. Again, ignore the boundary conditions for the moment. We can try to guess a solution to (46). It is clear that the function $F(\cdot)$ has to be such that the second partials of $F(S_t, t)$ with respect to $S_t$ and $t$ are proportional with a factor of proportionality equal to .3. This relationship between $F_{ss}$ and $F_{tt}$ should be true at any $S_t$ and $t$ . What could this function be? 

is shown explicitly. Note that the other candidate for $F(S_{t}, t)$ shown in Figure 1 will not pass from this line at t = 5. Hence, it cannot be a solution. Also, when $F(S_{t}, t)$ is a plane, the terminal conditions with respect to t or $S_{t}$ will be straight lines. 

exactly pinpoint the function that solves the PDE. This is easy to see geometrically, since a boundary condition corresponds to first selecting the "endpoint" for $t$ (or $S_t$ ) and then obtaining the intersection of the plane with a surface orthogonal to the time axis and passing from that $t$ . In Figure 2, the boundary condition at $t = 5$ , 

5 Classification of PDEs 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/6bf1cec3f84b9f1f69365f746df2b2d94ecdbe211e331edb18fde1d8403d8547.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/974c5d9eeff2c72d033af50d0e81917dd75134b118b12e67b5dfbdb7100b85e2.jpg)


Here $A, B, C, D, E, F$ represent various constants. The equation is of the second degree, because the highest power of $x$ or of $y$ is a square. By choosing different values for $A, B, C, D, E, F$ , the locus of the equation can be in the form of an ellipse, a parabola, a hyperbola, or a circle. 

It turns out that frequently encountered graphs such as circles, ellipses, parabolas, or hyperbolas can all be represented by a second-degree equation. In this section we briefly review this aspect of analytical geometry, since it relates to the terminology concerning PDEs. 

$F(S_{t},t) = -10(S_{t} - 4)^{2} - 3(t - 2)^{2},\quad -10\leq t\leq 10, - 10\leq S_{t}\leq 10.$ (53) The surface has contours as ellipses. In terms of boundary conditions, we can pick $t = 10$ as the terminal value for $t$ and get a boundary condition that has the form of a parabola: 

This is a function that traces a parabola in the $F, t$ plane. Yct such a boundary condition is not sufficient to determine all the parameters $\alpha, \beta, S_0, t_0$ . One would need a second boundary condition, say, at $t = 0$ : 

In this chapter, we introduced the notion of a partial differential equation (PDE). These are functional equations, whose solutions are functions of the underlying variables. We briefly discussed various forms of PDEs and introduced the related terminology.
This chapter also showed that the relationship between financial derivatives and the underlying assets can be exploited to obtain PDEs that derivative asset prices must satisfy. 

Note that the contours of this function are parabolas. This $F(S_{t}, t)$ will have boundary conditions as parabolas with respect to $t$ , and as straight lines with respect to $S_{t}$ . Such an $F(S_{t}, t)$ is one of the solutions of the PDE 

7.1 Example: Parabolic PDE
Figure 4 gives the graph of the function $F(S_{t}, t)$ defined as $F(S_{t}, t) = -10(S_{t} - 4)^{2} - 3(t - 2).$ 

Clearly, $F(S_{1}, t)$ graphed in Figure 3 is a solution to a PDE that satisfies the condition of an elliptic PDE, since $a_{4} = 0$ and both $a_{3}$ and $a_{4}$ are of the same sign. As a result, the condition 

Example 2 suggests that the contours of $F(S_{t}, t)$ would in general be non-linear equations. In case of Example 2, they were ellipses. In fact, partial differential equations of the form 

The easiest way to see this is to note that B = 0 and either A = 0 or C = 0 satisfies the required condition. But, when this happens, the second-degree equation reduces to 

6.3 Parabola
The second-degree equation in (56) reduces to a parabola when we have $B^{2}-4AC=0$ . (72) 

(a) Is the single boundary condition sufficient for calculating a numerical approximation to $f(x,t)$ ?
(b) Impose additional boundary conditions of your choice on $f(0,t)$ and $f(12,t)$ .
(c) Choose grid sizes of $\Delta x = 3$ and $\Delta t = .25$ and calculate a numerical approximation to $f(x,t)$ under the boundary conditions you have imposed. 

(a) $f(x,z,y) = e^{[29a^2\pi^2 + \pi (3x + 2y + 4z)]}$ (b) $f(x,z,y) = 3x^{2} + 3y^{2} - 6z^{2} + x + y - 9z - 3$ 

where a is a constant.
According to the heat equation, first partial with respect to t is proportional to the sum of second partials with respect to the variables in the function. Do the following functions satisfy the heat equation? 

Most of our readers are interested in PDEs because, at one point, they will be applying them in practical derivative asset pricing. Thus, rather than books on the theory of PDEs, sources dealing with the numerical solution of PDEs will be more useful. In most cases, these sources contain a brief summary of the underlying theory as well. We recommend two books on PDEs. Smith (1985) is easy to read. Thomas (1995) is a more comprehensive and recent treatment. 

$a_{5}^{2}-4a_{3}a_{4},$ (5)
as zero. This means that leaving aside the presence of $S_{i}$ and $S_{i}^{2}$ , which are always positive, the Black-Scholes PDE is of the parabolic form. 

$^{1}$ Only one of the second partials, namely the one with respect to $S_{1}$ , is present in this PDE. Also, note that there is no constant term. Under these conditions, we can easily calculate the value of the expression from Chapter 12, 

To show that this function satisfies the Black–Scholes PDE and the corresponding boundary condition, we have to take the first and second partials of (6) with respect to $S_{f}$ , and plug these in (3) with the $F(S_{t}, t)$ and its partial with respect to t. The result should equal zero. As t approaches T, the function should equal (4). 

$$
F (S _ {t}, t) = S _ {t} N (d _ {1}) - K e ^ {- r (T - t)} N (d _ {2}),
$$

We occasionally write $\sigma_{t}$ to denote $\sigma S_{t}$ . Under these conditions the fundamental PDE of Black and Scholes and the associated boundary condition are given by 

and, more importantly, 

Now, suppose we consider the special SDE where 

In Chapter 12 we obtained the PDE that the price of a derivative written on the underlying asset $S_{i}$ must satisfy under some conditions. The underlying security did not pay a dividend, and the risk-free interest rate was assumed to be constant at $r$ . Now suppose we consider the special SDE where 

2 The Black-Scholes PDE 

Finally, we compare closed-form solutions for PDEs with numerical approaches. We conclude with an example of a numerical asset price calculation. 

Next, we complicate the original Black-Scholes framework by introducing a second factor. This leads to some major difficulties, which we will discuss briefly. 

One purpose of this is to have a geometric look at the function that solves the PDE obtained by Black and Scholes (1973). The geometry of the Black–Scholes formula helps with the understanding of PDEs. In particular, we show geometrically the implications of having a single random factor in pricing call options. 

In this chapter, we provide some examples of partial differential equation methods using derivative asset pricing. 

## The Black-Scholes PDE

The partial differential equation obtained by Black and Scholes is relevant under some specific assumptions. These are (1) the underlying asset is a stock, (2) the stock does not pay any dividends, (3) the derivative asset is a European style call option that cannot be exercised before the expiration date, (4) the risk-free rate is constant, and (5) there are no indivisibilities or transaction costs such as commissions and bid-ask spreads. 

3 PDEs in Asset Pricing 

The trajectory $C_0$ , $C_T$ is interesting from another angle as well. As time passes, $S_t$ will trace the trajectory shown on the $S_t \times t$ plane. Going vertically to the surface, we obtain the trajectory $C_0$ , $C_T$ . Note that there is a deterministic correspondence between the two trajectories. Given the trajectory of $S_t$ on the horizontal plane, there is only one trajectory for $F(S_t, t)$ to follow on the surface. This is the consequence of having the same randomness in $S_t$ and in $F(S_t, t)$ . 

The second contour is shown as $bb'$ and represents $F(S_t, t)$ when we fix $t$ at .4 and move $S_t$ from 60 to 140. It is interesting to see that as $t$ goes toward 1, this contour goes toward the limit shown as $cc'$ . The latter is the usual graph with a kink at $K$ , which shows the option payoff at expiration. We would like to emphasize a potentially confusing point using Figure 1. The Black-Scholes formula gives a surface, once we fix $K, r$ , and $\sigma$ . This surface will not move as random events occur and realized values of $dW_t$ become known. Realization of the Wiener increments would only cause random movements on the surface. One such example is the trajectory denoted by $C_0, C_T$ in Figure 8. Because the increments of the Wiener process are unpredictable, the movement of the stock price along the $t$ direction will proceed in "random steps." Over infinitesimal intervals these steps are also infinitesimal, yet still unpredictable. 

We display two types of contours on the surface. First, we fix $S_{t}$ at a particular level and vary $t$ . This gives lines such as $aa'$ , which show how the call price will change as $t$ goes from 0 to 1 when $S_{t}$ is fixed at 100. 

In Figure 1, we have a “horizontal surface” defined by the axes labeled $S_t$ and $T - t$ , where the latter represents “time to expiration.” These two axes form a plane. For example, point $A$ represents an underlying asset price of 130, and a “time to expiration” equal to .80. By going up vertically toward the surface we reach point $B$ , which is in fact the value of the Black–Scholes formula evaluated at $A$ : 

299 

3 PDEs in Asset Pricing 

$^{2}$ If T = 1 means “one year,” the interest rate and the volatility will be yearly rates. But T = 1 may very well mean six months, three months, or any time interval during which the financial instrument will exist. We merely used T = 1 as a normalization. Under such conditions, the interest rate or the volatility numbers must be adjusted to the relevant time period. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/c701364f99bed0d539e902dc9099e06e0682fe71f5fd720dc0d4c7508a685376.jpg)


To plot the Black–Scholes formula with these particular parameters, we must select a range for the two variables $S_{t}$ and t. We let $S_{t}$ range from 50 to 140, and let t range from 0 to 1. The resulting surface is shown in Figure 1. 

and substitute these in formula (6). These numbers imply a 6.5% risk-free borrowing cost, and an 80% volatility during the interval $t \in [0,1]$ . This type of volatility is high for most mature financial markets. But it makes the graphics easier to read. The life of the call option is normalized to 1, with T = 1 implying one year, and the initial time is set at $t_{0} = 0$ . Finally, the strike price is set at $100.^{2}$ 

2.1 A Geometric Look at the Black-Scholes Formula
We saw in Chapter 12 that functions $F(S_{t}, t)$ satisfying various PDEs could be represented in three-dimensional space. We can do the same for the Black-Scholes PDE. The solution of this PDE was given by (6). We would like to pick numerical values for the parameters K, r, $\sigma$ , T and represent this formula in the three-dimensional space $F \times S \times t$ .
We pick 

$^{3}$ These are also known as “knock-out” and “knock-in” options. $^{4}$ The lookback option is floating because the strike price is not fixed. 

A ladder option has several thresholds, such that if the underlying price reaches these thresholds, the return of the option is “locked in.” 

A fixed lookback call option, on the other hand, pays the difference (if positive) between a fixed strike price K and $S_{max}$ , where the latter is the maximum reached by the underlying asset price during the life of the option. These options have the characteristic that some positive payoff is guaranteed if the option is in the money during some time over its life. Hence, everything else being the same, they are more expensive. 

In the case of a floating lookback call option, the payoff is the difference $S_{T}-S_{min}$ , where $S_{min}$ is the minimum price of the underlying asset observed during the life of the option. $^{4}$ 

In the standard Black–Scholes case, the call option payoff is equal to $S_{T}-K$ , if the option expires in the money. In this payoff $S_{T}$ is the price of the underlying asset at expiration and K is the constant strike price. 

Suppose the derivative asset is an option with a possibly random expiration date. For example, there are some “down-and-out” and “up-and-out” options that are known as barrier derivatives. $^{3}$ Unlike “standard” options, the payoff of these instruments also depends on whether or not the spot price of the underlying asset crossed a certain barrier during the life of the option. If such a crossing has occurred, the payoff of the option changes. We briefly review some of these “exotic” options. 

In the previous section, a complication to the Black-Scholes framework was discussed. The PDE satisfied by the arbitrage-free price of the derivative asset did change as the assumptions concerning dividend payments changed. This section discusses another complication. 

4 Exotic Options 

There is now a constant term $\delta$ . Hence stocks paying dividends at a constant rate $\delta$ do not present a major problem. 

$dP_{t} + \delta dt = rP_{t}dt,$ 

The difference occurs in deciding how much this portfolio should appreciate in value. Before, the (completely predictable) capital gains were exactly equal to earnings of a risk-free investment. But now, the underlying stock pays a dividend that is predictable at a rate of $\delta$ . Hence, the capital gains plus the dividends received must equal the earnings of a risk-free portfolio: 

Up to this point there is no difference from the original Black-Scholes approach discussed in Chapter 12. The time path of the $P_{t}$ will again be completely predictable. 

If one is trying to price a call option, and if the option is written on a stock that pays dividends at a constant rate of $\delta$ units per time, the resulting PDE will change only slightly. 

In most applications of pricing, one or more of these assumptions will be violated. If so, in general, the Black-Scholes PDE will not apply and a new PDE should be found. One exception is the violation of assumption (3). If the option is American style, the PDE will remain the same.
The relevant PDEs under these more complicated circumstances fall into one of a few general classes of applications. We discuss a simple case next. 

$^{7}$ Often arithmetic averages are used, and the average can be computed on a daily, weekly, or monthly basis. 

The form of the PDE is the same, but the boundary is different. This will result in a different solution for $F(S_t, t, K_t)$ , as was discussed earlier. 

In deriving the relevant PDE, the main difference from the standard case is in the boundary conditions. As long as the underlying asset price is above the barrier $K_{t}$ during the life of the option, $t \in [0,T]$ , the same PDE as in the standard case prevails: 

Third, the derivative may be written on more than one asset. All these may lead to changes in the basic PDE that we derived in the Black-Scholes case. Not all examples can be discussed here. But consider the case of knock-out options. We discuss the case of a "down-and-out" call. Let the $K_{t}$ be the barrier at time $t$ . Let $S_{t}$ and $F(S_{t}, t, K_{t})$ , respectively, be the price of the underlying asset and the price of the knock-out option. If the $S_{t}$ reaches the $K_{t}$ during the life of the option, the option holder receives a rebate $R_{t}$ and the option suddenly expires. Otherwise, it is a standard European option. 

First, the expiration value of the option may depend on some event happening over the life of the option (e.g., it may be a function of the maximum of the underlying asset price). Clearly, these make the boundary conditions much more complicated than the Black–Scholes case. 

303 

• Average or Asian options are quite common and have payoffs depending on the average price of the underlying asset over the lifetime of the option. $^{7}$ 

$F(S_{1T}, S_{2T}, T) = \max[0, (S_{1T} - K_1), (S_{2T} - K_2)].$ 

where $\theta_{1},\theta_{2}$ are known portfolio weights. As a final example, one may have a dual strike call option: 

- Basket options, which are derivatives where the underlying asset is a basket of various financial instruments. Such baskets dampen the volatility of the individual securities. Basket options become more affordable in the case of emerging market derivatives.
- Multi-asset options have payoffs depending on the underlying price or more than one asset. For example, the payoff of such a call may be 

There are obviously many different ways one can structure an exode option. Some common cases include the following: 

Knock-out options are European options that expire immediately if, for example, the underlying asset price falls below a barrier during the life of the option. The option pays a rebate if the barrier is reached. Otherwise, it is a "standard" European option. Such an option is called "down-and-out." 

4.3 Trigger or Knock-in Options
A down-and-in option gives its holder a European option if the spot price falls below a barrier during the life of the option. If the barrier is not reached, the option expires with some rebate as a payoff. $^{5}$ 

$^{9}$ If a curve is smooth and continuous, it may, however, be expanded as an infinite Taylor series expansion. Yet Taylor series expansions are not closed-form formulas. They are representations of such $F(\cdot)$ . 

$^{8}$ On the other hand, if the curve is of a “special” type, one may be able to identify it as a simple polynomial and represent it with a formula. For example, the curve in Figure 3 looks like a parabola and has a simple closed-form representation as $F = a_{0} + a_{1}t + a_{2}t^{2}$ . 

Hence, a solution to a PDE may exist, but a closed-form expression for the formula may not. In fact, given that such formulas are very constrained in representing smooth surfaces in three (or higher) dimensions, this may often be the case rather than the exception. 

The solutions of PDEs in the simple Black-Scholes case are surfaces in the three dimensional space generated by $S_{t}, t$ and $F(S_{t}, t)$ . Given a smooth and continuous curve in three-dimensional space $F \times t \times S_{t}$ , the partial derivatives may be well defined and may satisfy a certain PDE, but the surface may not be representable by a compact formula. 

where $a_{i}, i = 1,2,3$ are constants, cannot represent this curve. In fact, for a general continuous and smooth function, such closed-form formulas will not exist. $^{8,9}$ 

in some arbitrary fashion, and there is no reason to expect that this curve can be represented by a compact formula involving a few terms in t. For example, an exponential formula 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/2d36a361ae9c5366ceb506edc80157532c47cc5d873f3f1b9be053a5306e3a80.jpg)


$F(t)$ shown in Figure 2. The way it is drawn, $F(t)$ is clearly continuous and smooth. So, in the region shown, $F(t)$ has derivatives with respect to time. But $F(t)$ was drawn 

Now, it is possible that one can find a continuous surface such that the partial derivatives do indeed satisfy the PDE. But it may still be impossible to represent this surface in terms of an easy and convenient formula as in the case of Black-Scholes. In other words, although a solution may exist, this solution may not be representable as a convenient function of $S_{r}$ and $t$ . We will discuss this by using an analogy. Consider the function of time $E(t)$ shown in Figure 2 

The first method is similar to the one used by Black and Scholes, which involves solving the PDE for a closed-form formula. It turns out that the PDEs describing the behavior of derivative prices cannot in every case be solved for closed forms. In general, either such PDEs are not easy to solve, or they do not have solutions that one can express as closed-form formulas. First, let us discuss the difference between closed forms and numerical solutions of a PDE. The function $F(S_{t}, t)$ solves a PDE if the appropriate partial derivatives satisfy an equality such as 

Once a trader obtains a PDE representing the behavior over time of a derivative price $F(S_{t}, t)$ there will be two ways to proceed in calculating this value in practice. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/637b5f317dd88653def1699e476913b282edb7601b229542debaf88e408e98d8.jpg)


To carry on this calculation, we need to change the partial differential equation to a difference equation by replacing all differentials by appro-

We let $F_{ij}$ denote the "dot" that represents the $i$ th value for $S_t$ and the $j$ th value for $t$ . These values for $S_t$ and $t$ will be selected from their respective axes and then "plugged in" to $F(S_t, t)$ . The result is written as $F_{ij}$ . 

(29) 

We want to approximate $F(S_{t}, t)$ at a finite number of points $F_{ij}$ . This is shown in Figure 4 for an arbitrary surface and in Figure 5 for the Black-Scholes surface. In either case, the dots represent the points at which $F(S_{t}, t)$ will be evaluated. The sizes of the grids $\Delta S$ and $\Delta t$ determine how “close” these dots will be on the surface. Obviously, the closer these dots are, the better the approximation of the surface. 

where $F_{ij}$ is the value at time $t_j$ if the price of the underlying asset is at $S_i$ . The limits of $i,j$ will be determined by the choice of $\Delta S$ , $\Delta t$ and of $S_{\min}, S_{\max}$ . 

$F_{ij} = F(S_i, t_j)$ , 

To illustrate the last step, let 

5. Assuming that for small but noninfinitesimal $\Delta S_{f}$ and $\Delta t$ the same PDE is valid, the values of $F(S_{t}, t)$ at the grid points should be determined. 

307 

5 Solving PDEs in Practice 

4. The boundary conditions must be determined. 

$S_{\min} \leq S_{t} \leq S_{\max}$ . 

is "small," can be decided by trial and error. 3. Next one has to decide on the range of possible values for $S_{r}$ . To be more precise, one selects, a priori, the minimum $S_{\min}$ and the maximum $S_{\max}$ as possible values of $S_{r}$ . These extreme values should be selected so that observed prices remain within the range price of the underlying security.
2. Time t is the second variable in $F(S_{t}, t)$ . Hence, a grid size for $\Delta t$ is needed as well. Needless to say, $\Delta t$ , $\Delta S$ must be “small.” How small 

1. A grid size for $\Delta S$ must be selected as a minimum increment in the 

To solve this PDE numerically, one assumes that the PDE is valid for finite increments in $S_{t}$ and t. Two “partitions” are needed. 

$-rF + F_{t} + rF_{s}S_{t} + \frac{1}{2} F_{ss}\sigma^{2}S_{t}^{2} = 0, 0 \leq S_{t}, 0 \leq t \leq T.$ (27) 

When a closed-form solution does not exist, a market participant is forced to obtain numerical solutions to PDEs. A numerical solution is like calculating the surface represented by $F(S_{t}, t)$ directly, without first obtaining a closed-form formula for $F(S_{t}, t)$ . Consider again the PDE obtained from the Black–Scholes framework: 

5.2 Numerical Solutions 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/58889fb2bab92d48945a9a91391548a2bea95e06d20669b4ee94de005cf85670.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/f600926de550ecda27d8e2ad19d87d3bd1cfe6e581534b219e45fcd4a985b488.jpg)


One important point was the geometry of the Black–Scholes surfaces. We saw that random trajectories for the underlying assets price led to random paths on this surface. This is shown in Figure 6. 

This chapter discussed some examples of PDEs faced in pricing derivative assets. We illustrated the difficulties of introducing a second random element in pricing call options. We also discussed some exotic derivatives and the way PDEs would change. 

(37) 

These give the boundary values for $F_{ij}$ . In Figure 5, these boundary regions are shown explicitly. Using these boundary values in Eq. (30), we can solve for the remaining unknown $F_{ij}$ . 

(36) 

In this case, $S_{\mathrm{min}}$ is an extremely low price. There is almost no chance that the option will expire in the money. The resulting call premium is close to zero.
- For $t = T$ , we know exactly that $^{10}$ We are ignoring i, j subscripts for notational convenience. As will be seen below, elements of this difference equation depend on i, j. For each i, j there exists one equation such as (30). 

5.2.1 Boundary Conditions
Now, some of the $F_{ij}$ are known because of endpoint conditions. For example, we always know the value of the option as a function of $S_{i}$ at expiration. For extreme values of $S_{i}$ , we can use some approximations that are valid in the limit. In particular: 

$$
\frac {\Delta^ {2} F}{\Delta S ^ {2}} \stackrel {\sim} {=} \left[ \frac {F _ {i + 1 , j} - F _ {i j}}{\Delta S} - \frac {F _ {i j} - F _ {i - 1 , j}}{\Delta S} \right] \frac {1}{\Delta S},
$$

$$
r S \frac {\Delta F}{\Delta S} \cong r S _ {j} \frac {F _ {i + 1 , j} - F _ {i j}}{\Delta S}.
$$

$$
r S \frac {\Delta F}{\Delta S} \cong r S _ {j} ^ {F _ {i j} - F _ {i - 1, j}} \frac {\Delta S}{\Delta S},
$$

$$
\frac {\Delta F}{\Delta t} \stackrel {<  } {=} \frac {F _ {i j} - F _ {i , j - 1}}{\Delta t}
$$

$$
\frac {\Delta F}{\Delta t} + r S \frac {\Delta F}{\Delta S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\Delta^ {2} F}{\Delta S ^ {2}} \simeq r F,
$$

priate differences. There are various methods of doing this, each with a different degree of accuracy. Here, we use the simplest method $^{10}$ 

Ingersoll (1987) provides several examples of PDEs from asset pricing. Our treatment of this topic is clearly intended to provide examples for a simple introduction to PDEs. An interested reader should consult other sources if information beyond a simple introduction is needed. One good introduction to PDEs is Betounes (1998). This book illustrates the basics using MAPLE. 

(a) Calculate the expected value of the increment $dZ(t)$ .  
(b) Is $Z_{t}$ a martingale?  
(c) Calculate $E[Z_{t}]$ . How would you change the definition of $X_{t}$ to make $Z_{t}$ a martingale?  
(d) How would $E[Z_{t}]$ then change? 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/3f43d7349afca0e9432953ae2b84222d13e5469c0dcd2f0bf64fa909cdf205d0.jpg)


This construction is shown in Figure 1. The probability in (5) is a “mass” represented (approximately) by a rectangle with basic $\Delta$ and height $f(\bar{z})$ . Visualized this way, probability corresponds to a “measure” that is associated with possible values of $z_{t}$ in small intervals. Probabilities are called measures because they are mappings from arbitrary sets to nonnegative real 

$$
\int_ {\bar {z} - \frac {1}{2} \Delta} ^ {\bar {z} + \frac {1}{2} \Delta} \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} z _ {i}} d z _ {i} \simeq \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} \bar {z} ^ {2}} \int_ {\bar {z} - \frac {1}{2} \Delta} ^ {\bar {z} + \frac {1}{2} \Delta} d z _ {i}
$$

Now, if the region around $\bar{z}$ is small, then $f(z_{t})$ will not change very much as $z_{t}$ varies from $\bar{z}-\frac{1}{2}\Delta$ to $\bar{z}+\frac{1}{2}\Delta$ . This means we can approximate $f(z_{t})$ by $f(\bar{z})$ during this interval and write the integral on the right-hand side of (3) as 

$$
P \left(\bar {z} - \frac {1}{2} \Delta <   z _ {t} <   \bar {z} + \frac {1}{2} \Delta\right) = \int_ {\bar {z} - \frac {1}{2} \Delta} ^ {\bar {z} + \frac {1}{2} \Delta} \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} z _ {t} ^ {2}} d z _ {t}.
$$

Suppose we are interested in the probability that $z_{t}$ falls near a specific value $\bar{z}$ . Then, this probability can be expressed by first choosing a small interval $\Delta > 0$ , and next by calculating the integral of the normal density over the region in question: 

The probability density $f(z_{t})$ of this random variable is given by the well-known expression 

1 Translations of Probabilities 

Consider a normally distributed random variable $z_{i}$ at a fixed time t, with zero mean and unit variance. Formally, 

1.1 Probability as "Measure" 

This chapter discusses these tools. We adopt a step-by-step approach. First we review some simple concepts and set the notation. As motivation, we show some simple examples of the way the Girsanov theorem is used. The full theorem is stated next. We follow this with a section dealing with the intuitive explanation of various concepts utilized in the theorem. Finally, the theorem is applied in examples of increasing complexity. Overall, few examples are provided from financial markets. The next chapter deals with that. The purpose of the present chapter is to clarify the notion of transforming underlying probability distributions. 

Recent methods of derivative asset pricing do not necessarily exploit PDEs implied by arbitrage-free portfolios. They rest on converting prices of such assets into martingales. This is done through transforming the underlying probability distributions using the tools provided by the Girsanov theorem. This approach is quite different from the method of PDEs. The tools involved exploit the existence of arbitrage-free portfolios indirectly, and hence are more difficult to visualize. A student of finance or economics is likely to be even less familiar with this new set of tools than with, say, the PDEs. 

## Pricing Derivative Products

Equivalent Martingale Measures 

## CHAPTER 14

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/3c489d94b59e57d45839d0ede399a6a6ef7bb6b1e8356c005f1b598b37bcdc08.jpg)


Modern methods for pricing derivative assets utilize a novel way of transforming the probability measure $dP$ so that the mean of a random process $z_t$ changes. The transformation permits treating an asset that carries a positive “risk premium” as if it were risk-free. This chapter deals with this complicated idea. 

$^{1}$ In this book we always assume that this density exists. In other settings, the density function of the underlying random variables may not exist. 

• We can leave the shape of the distribution the same, but move the density to a different location. Figure 2 illustrates a case where the normal density that was centered at 

Under these conditions, we can subject a probability distribution to two types of transformations: 

which can be seen as an “average” value of $z_{t}$ . Geometrically, this determines the center of the probability mass. The variance is another weighted average: 

This can be read as the probability that the random variable $z_{t}$ will fall within a small interval centered on $\bar{z}$ and of infinitesimal length $dz_{t}$ . The sum of all such probabilities will then be given by adding these $dP(\bar{z})$ for various values of $\bar{z}$ . Formally, this is expressed by the use of the integral 

numbers $R^{+}$ . For infinitesimal $\Delta$ , which we write as $dz_{i}$ , these measures are denoted by the symbol $dP(z_{i})$ , or simply dP when there is no confusion about the underlying random variable: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/f77fbf779d30ed917dd522e34030d076aca079a799550e1a608f2b1c4cacab24.jpg)


Now, suppose we would like to change the mean of Z using the method outlined earlier. More precisely, suppose we would like to calculate a new 

2.1.1 Example 1
In spite of the simplicity of this transformation, it is important for later discussions to look at a precise example.
Suppose the random variable Z is defined as follows. A die is rolled and the values of Z are set according to the rule 

The first and standard method for changing the mean of a random variable is used routinely in econometrics and statistics. One simply adds a constant $\mu$ to $z_{i}$ in order to obtain a new random variable $\tilde{z}_t = z_t + \mu.$ $^2$ . The $\tilde{z}_t$ defined this way will have a new mean. For example, if originally 

We discuss these methods in detail next. The discussion proceeds within the context of a single random variable, rather than a stochastic process. The more complicated case of a continuous-time process is treated in the section on the Girsanov theorem. 

Both operations lead to a change in the original mean, while preserving other characteristics of the original random variable. However, while the first method cannot, in general, be used in asset pricing, the second method becomes a very useful tool.
We discuss these methods in detail next. The discussion proceeds within 

Now, fix t and let $z_{t}$ be a univariate random variable. There are two ways: one can change the mean of $z_{t}$ . In the first case, we operate on the values assumed by $z_{t}$ . In the second, and counterintuitive, case, we leave the values assumed by $z_{t}$ unchanged, but instead operate on the probabilities associated with $z_{t}$ . 

in the case where $r_{t}$ and $\mu$ are small enough that the cross-product term can be ignored.
Under these conditions, $\mu$ is the risk premium for holding the asset for one period, and $\frac{1}{(1+r_{t})}$ is the risk-free discount factor. 

which says that the expected return of the risky asset must exceed the risk-free return approximately by $\mu$ : 

Lct $r_t$ be the rate of risk-free return. A typical risky asset $S_t$ must offer a rate of return $R_t$ greater than $r_t$ , since otherwise there will be no reason to hold it. This means that, using $E_{t}[\cdot]$ , the expectation operator conditional on information available as of time $t$ satisfies 

2.1.3 Example 3
The example is discussed in discrete time first. Let $S_{t}$ , $t = 1, 2, \ldots$ be the price of some financial asset that pays no dividends. The $S_{t}$ is observed over discrete times $t$ , $t + 1, \ldots$ . 

equivalent risk-free yield. This example is simple and does not illustrate why somebody might want to go through such a transformation of means to begin with. The next example is more illustrative in this respect. 

If $\mu$ is selected as $-\alpha$ , then such a transformation would eliminate the risk premium from $R_{t}$ . Note that in order to use this method for changing means, we need to know the risk premium $\alpha$ . Only under these conditions could we arrive at subtracting the "right" quantity from $R_{t}$ and obtain the equivalent risk-free yield. 

Then $R_{t}$ is a random variable with mean $r_t + \alpha$ . The first method to change the mean of $R_{t}$ is to add a constant and obtain a new random variable $\tilde{R}_{t} = R_{t} + \mu$ . This random variable will have the mean 

2.1.2 Example 2
We can illustrate this method for changing the means of random variables using a more relevant example from finance.
The yield of a triple-A-rated corporate bond $R_{t}$ with fixed t will have the expected value 

As can be seen from this transformation, in order to change the mean of Z, we operated on the values assumed by Z. Namely, we subtracted 1 from each possible value. The probabilities were not changed. 

Note that the new probabilities are designated by $\tilde{P}$ . Now calculate the mean under these new probabilities: 

The second way of changing the mean of a random variable is to leave the random variable “intact,” but transform the corresponding probability measure that governs $z_{i}$ . We introduce this method using a series of examples that get more and more complicated. At the end we provide the Girsanov theorem, which extends the method to continuous-time stochastic processes. The idea may be counterintuitive, but is in fact quite simple, as Example 1 will show. 

What would $E_t^p [-1]$ and $r_t$ represent in this particular case? $r_t$ will be the risk-free rate. The expectation operator would be given by the risk-neutral probabilities. By making these transformations, we would be eliminating the risk premium from $R_t$ : 

this can be very useful for calculating $S_{t}$ . In fact, one could exploit this equality by “forecasting” $S_{t+1}$ , using a model that describes the dynamics of $S_{t}$ , and then discounting the “average forecast” by the (known) $r_{t}$ . This would provide an estimate of $S_{t}$ . 

$$
E _ {t} ^ {\tilde {P}} \left[ \frac {1}{(1 + r _ {t})} S _ {t + 1} \right] = S _ {t},
$$

by calculating the expectation on the left-hand side. $^{3}$ But doing this requires a knowledge of the distribution of $R_{t}$ , which requires knowing the risk premium $\mu^{4}$ . Yet knowing the risk premium before knowing the fair market value $S_{t}$ is rare. Utilization of (29) will go nowhere in terms of calculating $S_{t}^{5}$ . 

Now consider the problem of a financial analyst who wants to obtain the fair market value of this asset today. That is, the analyst would like to calculate $S_{t}$ . One way to do this is to exploit the relation 

$$
[ d P (z _ {i}) ] [ \xi (z _ {i}) ] = \frac {1}{\sqrt {2 \pi}} e ^ {- \frac {1}{2} (z _ {i} ^ {2}) + \mu z _ {i} - \frac {1}{2} \mu^ {2}} d z _ {i}.
$$

$\xi(z_{t})=e^{z_{t}\mu-\frac{1}{2}\mu^{2}}.$ (43)
When we multiply $\xi(z_{t})$ by $dP(z_{t})$ , we obtain a new probability. This can be seen from the following: 

In this example, the state space is continuous, although we are still working with a single random variable, instead of a random process. Next, define the function 

We now discuss such probability transformations in more complex settings. The Girsanov theorem will be introduced using special cases with growing complexity. Then we provide the general theorem and discuss its assumptions and implications. 

The general method can be summarized as follows: (1) We have an expectation to calculate. (2) We transform the original probability measure so that the expectation becomes easier to calculate. (3) We calculate the expectation under the new probability. (4) Once the result is calculated and if desired, we transform this probability back to the original distribution. 

Accordingly, if we have to calculate an expectation, and if this expectation is easier to calculate with an equivalent measure, then it may be worth switching probabilities, although the new measure may not be the one that governs the true states of nature. After all, the purpose is not to make a statement about the odds of various states of nature. The purpose is to calculate a quantity in a convenient fashion. 

$^{7}$ Some readers may wonder how we found the new probabilities $\tilde{P}(Z)$ . In this particular case, it was easy. We considered the probabilities as unknowns and used three conditions to solve for them. The first condition is that the probabilities sum to one. The second is that the new mean is one. The third is that the variance equals 98/3. 

The probabilities so transformed are called "equivalent" because, as we will see in more detail later in this chapter, they assign positive probabilities to the same domains. Thus, although the two probability distributions are different, with appropriate transformations one can always recover one measure from the other. Since such recoveries are always possible, we may want to use the "convenient" distribution for our calculations, and then, if desired, switch back to the original distribution. 

Instead of using a random process:
The Girsanov theorem provides the general framework for transforming one probability measure into another “equivalent” measure in more complicated cases. The theorem covers the case of Brownian motion. Hence, the state space is continuous, and the transformations are extended to continuous-time stochastic processes. 

The examples just discussed were clearly simplified. First, we dealt with random variables that were allowed to assume a finite number of values—the state space was finite. Second, we dealt with a single random variable instead of using a random process. 

It is worth emphasizing that these new probabilities do not relate to the “true” odds of the experiment. The “true” probabilities associated with rolling the die are still given by the original numbers, P. The reader may have noticed the notation we adopted. In fact, we need to write the new expectation operator as $E^{P}[\cdot]$ , rather than $E[\cdot]$ . The probabilities used in calculating the averages are no longer the same as P, and the use of $E[\cdot]$ will be misleading. When this method is used, special care should be given to designating the probability distribution utilized in calculating expectations under consideration. $^{7}$ 

The variance has not changed. The transformation of probabilities shown in (38) accomplishes exactly what the first method did. Yet this second method operated on the probability measure $P(Z)$ , rather than on the values of Z itself. 

$E^{\tilde{P}}[Z]^2 = \frac{122}{429} [10 - 1]^2 +\frac{5}{33} [-1 - 1]^2 +\frac{22}{39} [-3 - 1]^2 = \frac{98}{3}. \tag{40}$ 

Suppose we want to change the means of $z_{1t}, z_{2t}$ from $\mu_1, \mu_2$ to zero, while leaving the variances unchanged. Can we accomplish this by transforming the probability $dP(z_{1t}, z_{2t})$ just as in the previous example, namely, by multiplying by a function $\xi(z_{1t}, z_{2t})$ ? 

This expression is the probability mass associated with a small rectangle $dz_{1t}dz_{2t}$ centered at a particular value for the pair $z_{1t}, z_{2t}$ . It gives the probability that $z_{1t}, z_{2t}$ will fall in that particular rectangle jointly. Hence the term joint density function. 

Finally, $\mu_{1},\mu_{2}$ are the means corresponding to $z_{1t}$ and $z_{2t}$ . The joint probability measure can be defined using 

The previous example showed how the mean of a normally distributed random variable could be changed by multiplying the corresponding probability measure by a function $\xi(z_{i})$ . The transformed measure was shown to be another probability that assigned a different mean to $z_{i}$ , although the variance remained the same. 

The next question is whether we can accomplish the same transformations if we are given a sequence of normally distributed random variables, $z_{1}, z_{2}, \ldots, z_{t}$ . 

Then $\tilde{Z}$ will have a zero mean.  
- Method 2: Using equivalent measures. Given a random variable $Z$ with probability $P$ , 

It turns out that by multiplying $dP(z_{i})$ by the function $\xi (z_{i})$ , and then switching to $\tilde{P}$ , we succeeded in changing the mean of $z_{i}$ . Note that in this particular case, the multiplication by $\xi (z_i)$ preserved the shape of the probability measure. In fact, (45) is still a bell-shaped, Gaussian curve with the same variance. But $P(z_{i})$ and $\tilde{P} (z_i)$ are different measures. They have different means and they assign different weights to intervals on the $z$ -axis. Under the measure $P(z_{i})$ , the random variable $z_{i}$ has mean zero, $E^P [z_i] = 0$ , and variance $E^P [\frac{z_i^2}{z_i}] = 1$ . However, under the new probability 

By simply reading from the density in (45), we see that $\tilde{P}(z_{t})$ is the probability associated with a normally distributed random variable mean $\mu$ and variance 1. 

This expression can be regarded as a derivative. It reads as if the “derivative” of the measure $\bar{P}$ with respect to P is given by $\xi(z_{t})$ . Such derivatives are called Radon–Nikodym derivatives, and $\xi(z_{t})$ can be regarded as the density of the probability measure $\bar{P}$ with respect to the measure P.

According to this, if the Radon–Nikodym derivative of $\bar{P}$ with respect to P exists, then we can use the resulting density $\xi(z_{t})$ to transform the mean of $z_{t}$ by leaving its variance structure unchanged. 

We will now discuss where this functional form comes from. In normal distributions, the parameter $\mu$ , which represents the mean, shows up only as an exponent of e. What is more, this exponent is in the form of a square: 

3.2.1 A Note
With future discussion in mind, we would like to emphasize one regularity that the reader may already have observed.
Think of $z_{i}$ as representing a vector of length k, or simply as a univariate random variable. In transforming the probability measures $P(z_{i})$ into $\tilde{P}(z_{i})$ , the function $\xi(z_{i})$ was utilized. This function had the following structure, 

underlying probabilities:
This example dealt with a bivariate random vector. Exactly the same transformation can be applied if instead we have a random sequence of k normally distributed random variables, $[z_{1}, z_{2}, \ldots, z_{k}]$ . Only the orders of the corresponding vectors and matrices in (53) need to be changed, with similar adjustments in (57). 

We recognize this as the bivariate normal probability distribution for a random vector $[z_{1t}, z_{2t}]$ with mean zero and variance-covariance matrix $\Omega$ . The multiplication by $\xi(z_{1t}, z_{2t})$ accomplished the stated objective. The nonzero mean of the bivariate vector was eliminated through a transformation of the underlying probabilities. 

Clearly, such a transformation is very useful for a financial market participant, because the risk premiums of asset prices can be “eliminated” while leaving the volatility structure intact. In the case of options, for example, the option price does not depend on the mean growth of the underlying asset price, whereas the volatility of the latter is a fundamental determinant. In such circumstances, transforming original probability distributions using $\xi(z_{t})$ would be very convenient.

In Figure 4, we show one example of this function $\xi(z_{t})$ . 

$\xi_{t}=e^{(\int_{0}^{t}X_{u}dW_{u}-\frac{1}{2}\int_{0}^{t}X_{u}^{2}d\omega)},\quad t\in[0,T],$ (76)
where $X_{t}$ is an $I_{t}$ -measurable process. $^{11}$ The $W_{t}$ is a Wiener process with probability distribution P.
We impose an additional condition on $X_{t}$ . $X_{t}$ should not vary “too much”. 

meaningfully, we need the probability mass in the denominator to be different from zero. To perform the inverse transformation, we need the numerator to be different from zero. But the numerator and the denominator are probabilities assigned to infinitesimal intervals dz. Hence, in order for the Radon-Nikodym derivative to exist, when P assigns a nonzero probability to dz, so must P, and vice versa. In other words: 

$^{10}$ Note that this is not a very serious restriction in the case of financial derivatives. Almost all financial derivatives have finite expiration dates. Often, the maturity of the derivative instrument is less than one year. 

will be changed.
2. In earlier examples, $\mu$ was time independent. Here, $X_{t}$ may depend on any random quantity, as long as this random quantity is known by time t. That is the meaning of making $X_{t}$ , $I_{t}$ -adapted. Hence, much more complicated drift transformations are allowed for.
3. The $\xi_{t}$ is a martingale with $E[\xi_{t}] = 1$ . 

In heuristic terms, this theorem states that if we are given a Wiener process $W_{t}$ , then, multiplying the probability distribution of this process by $\xi_{t}$ , we can obtain a new Wiener process $\tilde{W}_{t}$ with probability distribution $\tilde{P}$ . The two processes are related to each other through 

This means that $X_{i}$ cannot increase (or decrease) rapidly over time. Equation (77) is known as the Novikov condition.
In continuous time, the density $\xi_{i}$ has a “new” property that turns out to be very important. It turns out that if the Novikov condition is satisfied, then $\xi_{i}$ will be a square integrable martingale. We first show this explicitly.
Using Ito's Lemma, calculate the differential 

Then $\tilde{S}_t$ will be a martingale. One disadvantage of this transformation is that in order to obtain $\tilde{S}_t$ , one would need to know $\mu$ . But $\mu$ incorporates any risk premium that the risky stock return has. In general, such risk premiums are not known before one finds the fair market value of the asset. 

We give a heuristic example. Let $dS_{t}$ denote incremental changes in a stock price. Assume that these changes are driven by infinitesimal shocks that have a normal distribution, so that we can represent $S_{t}$ using the stochastic differential equation driven by the Wiener process $W_{t}$ . 

Next, consider the Wiener process $\tilde{W}_t$ . There is something counterintuitive about this process. It turns out that both $\tilde{W}_t$ and $W_t$ are standard Wiener processes. Thus, they do not have any drift. Yet they relate to each other by 

This determines the arbitrage-free dynamics of the postulated Stochastic Differential Equation.

• Second, the market practitioner needs to calibrate the SDEs volatility parameter(s). This nontrivial task is often based on the existence of liquid options, or caps/floors markers, that provide direct volatility quotes. But, even then calibration needs to be done carefully.

• Once the underlying synthetic probability and the dynamics are determined, the task reduces to one of calculating in (109) the expectation itself. This can be done either by calculating the implied closed-form solution, or by numerical evaluation of the expectation. In case of closed-form solution, one would “take” the integral, which gives the expectation $E^{P}[F(S_{T}, T)]$ : 

- First, the probability distribution $\tilde{P}$ needs to be selected. This is, in general, done indirectly by selecting the first- and second-order moments of the underlying processes, as implied by the fundamental theorem of finance. For example, in case the security does not have any payouts and there is no foreign currency involved, we let for a small $\Delta > 0$ : 

with known $F(\cdot)$ . A market practitioner would then need to take the following “straightforward” steps in order to price the derivative contract: 

The fact that the $D_{t}$ and the probability $\tilde{P}$ are known makes Eq. (109) a very useful analytical tool, because for all derivative assets there will exist an expiration time $T$ , such that the dependence of the derivative asset's price, $C_T$ , on $S_T$ is contractually specified. Hence, using $C_t = F(S_t, t)$ we can write: 

where t < T and the $D_{t}$ is a discount factor, known or random, depending on the normalization adopted. In case there are no foreign currencies or payouts, and in case savings account normalization is utilized, $D_{t}$ will be a function of the risk-free rate $r_{t}$ . If $r_{s} = r$ is constant, the $D_{t}$ will be known and will factor out of the expectation operator.
The fact that the $D_{t}$ and the probability $B_{r}$ are known across Eq. (100). 

The role played by the synthetic probabilities $\tilde{P}$ appears central to pricing of financial securities even at this level of discussion. According to the dis-cussion in Chapter 2, under the condition of no-arbitrage and in a discrete time setting, the “fair” price of any security that trades in liquid markets will be given by the martingale equality: 

But this is a probability measure associated with a normally distributed process with zero drift and diffusion $\sigma$ . That means we can write the increments of $S_{i}$ in terms of a new driving term $\tilde{W}_{i}$ : 

$E^{p}[S_{t+s}|S_{t}] = S_{t}.$ (103)
As usual, the superscript of the $E[\cdot|]$ operator represents the probability measure used to evaluate the expectation.
In order to perform this transformation, a $\xi(S_{t})$ function needs to be calculated. First recall that the density of $S_{t}$ is given by 

(117) 

That is, $\hat{S}_{t}$ will be obtained by multiplying the possible values $S_{T}^{i}$ by the true probabilities $p^{j}$ that correspond to the possible states. $^{15}$ Clearly, if one used the $\tilde{p}^{j}$ in place of $p^{j}$ , the resulting forecast where the $d\tilde{P}(S_{T})$ is the martingale probability associated with that particular infinitesimal variation in $S_{T}$ . The $S_{min}, S_{max}$ is the range of possible movements in $S_{T}$ .
In case of “Monte Carlo” evaluation, one would use the approxima-

As seen in Girsanov Theorem, there is an interesting way one can use martingales to generate probabilities. For example, assume that we define a random process $Z_{i}$ that assumes only nonnegative values. Suppose we select a random process Z that has the following properties: 

(119) 

$0 \leq Z_{t},$ (118) for all $t$ , under a probability $P$ . We show that such $Z$ can be very useful in generating new probabilities. Consider a set $A$ in the real line $R$ , and define its indicator function as $1_A$ : 

would be quite an inaccurate reflection of where $S_{t}$ would be within an interval $\Delta$ , because under $\tilde{P}$ the $S_{t}$ would grow at the (inaccurate) rate $r_{t}\Delta$ rather than the true expected growth $((r_t + \mu)\Delta)$ that incorporates the risk premium $\mu$ . Having misrepresented the possible growth in $S_{t}$ , the martingale probability $\tilde{P}$ could certainly not generate satisfactory forecasts. Yet, the $\tilde{P}$ is useful in the process of pricing. For forecasting exercises, a decision maker should clearly use the real-world probability and apply the operator $E^p[·]$ . 

(112) 

In also as important to, say, an econometrician: In general, not at all. Suppose the econometrician's objective is to obtain the best prediction of $S_T$ . Then, the use of $\bar{P}$ would yield miserable results. In order to see this, suppose the world at time $T$ has $M$ possible states. The "best" forecast of $S_T$ , denoted by $\hat{S}_t$ , will then be given by: 

where the $j = 1,\dots ,N$ is an index that represents trajectories of $S_T$ randomly selected from the arbitrage-free distribution $\vec{P}$ . This and similar procedures are called Monte Carlo methods. The law of large numbers guarantee that, if the randomness is correctly modeled in the selection of $S_T^j$ , and if the number of paths $N$ goes to infinity, the above average will converge to the true expectation. Hence, the approxima 

Hence, $e^{[\sigma W_{i}-\frac{1}{2}\sigma^{2}t]}$ is one convenient candidate to the nonnegative process $Z_{i}$ that we discussed in the previous section. It can be used to generate equivalent probabilities because it is positive and its expectation is equal to one. 

But the function under the integral sign is the density of a normally distributed random variable with mean $\sigma t$ and variance $\varepsilon$ . Consequently, when it is integrated from minus to plus infinity, we should obtain: 

$$
E ^ {p} [ Z _ {t} ] = \int_ {- \infty} ^ {\infty} e ^ {\sigma W _ {t} - \frac {1}{2} \sigma^ {2} t} \frac {1}{\sqrt {2} t} e ^ {- \frac {1}{2 t} w _ {t} ^ {2}} d W _ {t}.
$$

3. The long rate R and the short rate r are known to have a jointly normal distribution with variance–covariance matrix $\Sigma$ and mean $\mu$ . These moments are given by 

(d) Is the variance different under these probabilities? 

2. Assume that the return $R_{t}$ of a stock has the following log-normal distribution for fixed t: 

such that $\Delta y$ has mean .05.
(c) Has the variance changed?
(d) Now do the same transformation using a change in probabilities,
so that again the variance remains constant.
(e) Have the values of $\Delta x$ changed? 

(a) Calculate the mean and the variance of this random variable.  
(b) Change the mean of this random variable to .05 by subtracting an appropriate constant from $\Delta x$ . That is, calculate 

$\{\Delta x = 1, p(\Delta x = 1) = .3\},$ $\{\Delta x = -0.5, p(\Delta x = -0.5) = .2\},$ $\{\Delta x = .2, p(\Delta x = .2) = .5\}.$ 

1. Consider a random variable $\Delta x$ with the following values and the corresponding probabilities: 

Transforming stochastic processes into martingales through the use of the Gisanov theorem is a deeper topic in stochastic calculus. The source that provide the technical background of this method will all be at an advanced level. Karatzas and Shreve (1991) provides one of the more intuitive discussions. Liptser and Shiryayev (1977) is a comprehensive reference. 

## 9 References

- The transformation was done by switching the distribution of $S_t$ from $P$ to $\bar{P}$ . This was accomplished by using a new error term $\bar{W}_t$ .
- This new error term $\bar{W}_t$ still had the same variance.
- What distinguishes representation (108) from (94) is that the mean of $S_t$ is altered, while preserving the zero mean property of the error terms. This was accomplished by changing the distributions, rather than subtracting a constant from the underlying random variable.
- More importantly, in this example, the transformation was used to convert $S_t$ into a martingale. In financial models, one may want to apply the transformation to $e^{-r}S_t$ rather than $S_r$ . $e^{-r}S_t$ would represent the discounted value of the asset price, where the discount is done with respect to the (risk-free) rate $r$ . The $g(S_t)$ function has to be redefined in order to accomplish this. 

As conclusions, we review some of the important steps of transforming the $S_{i}$ into a martingale process. 

## 8 Conclusions

Note that, by switching to the probability $\tilde{P}$ , the term represented by $Z_{T}$ has simply “disappeared” and the expectation is easier to calculate. In the case of pricing exotic options, transformations that use this method turn out to be convenient ways of obtaining pricing formulas. Essentially, we see that expectations involving geometric processes will contain implicitly terms that can be represented by such $Z_{T}$ . It then immediately becomes possible to change measures using the trick discussed in this section. The resulting expectations may be easier to evaluate. 

The Girsanov theorem is applied explicitly in the second half of the chapter, where the correspondence between two approaches to asset pricing is also discussed. In particular, we show that converting (discounted) call 

The first major topic of this chapter is a step-by-step treatment of the martingale approach. We begin with the assumptions set by Black and Scholes and show how to convert the (discounted) asset prices into martingales. This is done by finding an equivalent martingale measure $\tilde{P}$ . This application does not use the Girsanov theorem directly. 

again, either analytically or numerically. 

1. The original Black-Scholes approach, where: (1) a riskless portfolio is formed, (2) a partial differential equation in $F(S_t, t)$ is obtained, and (3) the PDE is solved either directly or numerically.
2. The martingale methods, where one finds a "synthetic" probability $\tilde{P}$ under which $S_t$ becomes a martingale. One then calculates 

In this chapter, we show how the method of equivalent martingale measures can be applied. We use option pricing to do this. We know that there are two ways of calculating the arbitrage-free price of a European call option $C_t$ written on a stock $S_t$ that does not pay any dividends. 

1 Introduction 

Applications 

# Equivalent Martingale

## CHAPTER 15

(c) Plot the $\xi (R,r)$ and the new density. (d) Has the variance-covariance matrix of interest rate vector changed? 

$d\tilde{P} = \xi (R,r)f(R,r)dRdr.$ 

(a) Using Mathematica or Maple plot this joint density.
(b) Find a function $\xi(R,r)$ such that the interest rates have zero mean under the probability. 

The moment-generating function is a useful tool in statistics. If its kth derivative with respect to $\lambda$ is calculated and evaluated at $\lambda = 0$ , one finds the kth moment of the random variable in question.
For example, the first moment of $Y_{t}$ can be calculated by taking the derivative of (10) with respect to $\lambda$ : 

But the integral on the right-hand side of this expression is the area under the density of a normally distributed random variable. Hence, it sums to one. We obtain 

The exponent of the second exponential function can now be completed into a square. The terms that do not depend on $Y_{i}$ can be factored out. Doing this, we get 

$$
E [ e ^ {Y _ {t} \lambda} ] = \int_ {- \infty} ^ {\infty} e ^ {Y _ {t} \lambda} \frac {1}{\sqrt {2 \pi \sigma^ {2} t}} e ^ {- \frac {1}{2} \frac {(Y _ {t} - \mu) ^ {2}}{\sigma^ {2} t}} d Y _ {t},
$$

2.1.1 Calculation Using the distribution in (2), $E[e^{Y_{\lambda}}]$ can be calculated explicitly. Substituting from the definition in (4), we can write 

$^{1}Y_{t}$ is sometimes called a generalized Wicner process, because it obeys a normal distribution, has a nonzero mean, and has a variance not necessarily equal to one. $^{2}S_{0}$ may be random, as long as it is independent of $Y_{t}$ . 

where $\lambda$ is an arbitrary parameter. The explicit form of this moment-generating function is useful in asset pricing formulas. More importantly, the types of calculations one has to go over to obtain the moment-generating function illustrate some standard operations in stochastic calculus. The following section is useful in this respect as well. 

using the application:
First, some intermediate results need to be discussed. These results are important in their own right, since they occur routinely in asset pricing formulas. 

The method of equivalent martingale measures adopts a different way of obtaining the same formula. The derivation is tedious at points, but rests on straightforward mathematics and consequently is conceptually very simple. We will provide a step-by-step derivation of the Black-Scholes formula using this approach. 

The method of forming risk-free portfolios and using the resulting PDEs was discussed in Chapter 12, although a step-by-step derivation of the Black-Scholes formula was not provided there. 

prices into martingales is equivalent to forcing the $F(S_{1}, t)$ to satisfy a particular partial differential equation, which turns out to be the Black-Scholes PDE introduced earlier. We conclude that the PDE and the martingale approaches are closely related. 

$$
E \left[ \frac {S _ {t}}{S _ {u}} \mid S _ {u}, u <   t \right] = E [ e ^ {\Delta Y _ {t}} | S _ {u} ],
$$

Observed the asset price by:
Observed values of $S_{i}$ will occur according to the probabilities given by P. But this does not mean that a financial analyst would find this distribution most convenient to work with. In fact, according to the discussion in Chapter 14, one may be able to obtain an equivalent probability $\tilde{P}$ under which pricing assets becomes much easier. This will especially be the case if we work with probability measures that convert asset prices into martingales.
In this section we discuss an example of how to find such a probability measure 

as a result by itself. At several points later, we have to take expectations of geometric processes. The foregoing result is very convenient, in that it gives an explicit formula for expectations involving geometric processes. 

The parameter $\rho$ is now fixed in terms of the volatility $\sigma$ and the risk-free interest rate r. The important aspect of this choice for $\rho$ is that the exponential on the right-hand side of (38) will equal one, since with this value of $\rho$ , 

Now, assume that $S_{t}$ represents the value of an underlying asset at time $t$ , and let $S_{u}, u < t$ be a price observed at an earlier date $u$ . First of all, we know that because the asset $S_{t}$ is risky when discounted by the risk-free rate, it cannot be a martingale. In other words, under the true probability measure $P$ , we cannot have 

Note the second difference between the two SDEs. The SDE in (51) is driven by a new Wiener process $\tilde{W}_{i}$ , which has the distribution $\tilde{P}$ . This $\tilde{P}$ has nothing to do with the actual occurrence of various states of the world. The probability measure P determines that. On the other hand, $\tilde{P}$ is a very convenient measure to work with. Under this measure, (discounted) asset prices are martingales, and this is a very handy property to have in valuing derivative assets. Also, we know from finance theory that under appropriate conditions, the existence of such a “synthetic” probability $\tilde{P}$ under which asset prices are martingales is guaranteed if there is no arbitrage. 

This is an interesting result. The probability that makes $S_{t}$ a martingale, switches the drift parameter of the original SDE to the risk-free interest rate $r$ . The $\mu$ contained a risk premium that is in general not known before $S_{t}$ is calculated. The $r$ , on the other hand, is the risk-frec rate and is known by assumption. 

Here we emphasize, in passing, a critical step that may have gone unnoticed. By substituting $\bar{W}_{t}$ in place of $W_{t}$ , we are implicitly switching the underlying probability measures from P to $\bar{P}$ . This is the case because only under $\bar{P}$ will the error term in Eq. (48) be a standard Wiener process. If we continue to use P, the error terms $d\bar{W}_{t}$ will have a nonzero drift.
In Eq. (48), $\rho$ can now be replaced by its value 

The SDE under the martingale measure $\vec{P}$ is calculated in a similar fashion, but the drift coefficient is now different. To get this SDE, we simply 

1. a drift coefficient $(\mu + (1/2)\sigma^{2})S_{t}$ ,
2. a diffusion coefficient $\sigma S_{t}$ ,
3. and a driving Wiener process $W_{t}$ . 

To get the SDE satisfied by $S_{t}$ , we need to obtain the expression for stochastic differentials $dS_{t}$ . Because $S_{t}$ is a function of $Y_{t}$ , and because we have a SDE for the latter, Ito's Lemma can be used: 

The previous section discussed how to determine an equivalent martingale measure $\tilde{P}$ , when the “true” distribution of asset prices was governed by the probability measure P. It is instructive to compare the implied stochastic differential equations (SDE) under the two probability measures. $S_{t}$ was given by 

By determining a particular value for $\rho$ , we were able to find a probability distribution under which expectations of asset prices had the martingale property. This distribution is normal in this particular case, and its form is given by 

$$
d \breve {P} = \frac {1}{\sqrt {2 \pi \sigma^ {2} T}} e ^ {- \frac {1}{2 \sigma^ {2} T} (Y _ {T} - (r - \frac {1}{2} \sigma^ {2}) T) ^ {2}} d Y _ {T},
$$

- Let $t = 0$ and calculate the option price as of time zero.
- Accordingly, the current information set $I_t$ becomes $I_0$ . This way, instead of using conditional expectations, we can use the unconditional expectation operator $E^p[\cdot]$ . 

In order to derive the Black–Scholes formula, this expectation will be calculated explicitly. The derivation is straightforward, yet involves lengthy expressions. It is best to simplify the notation. We make the following simplifications: 

where $T > t$ is the expiration date of the call option. We know that at expiration, the option's payoff will be $S_T - K$ if $S_T > K$ . Otherwise, the call option expires with zero value. This permits one to write the boundary condition 

Let $S_{t}$ be an underlying asset, and $C_{t}$ the price of a European call option written on this asset. Assume the standard Black-Scholes framework, with no dividends, a constant risk-free rate, and no transaction costs. Our objective in this section is to derive the Black-Scholes formula directly by using the equivalent martingale measure $\tilde{P}$ . The basic relation is the martingale property that the $e^{-rt}C_t$ must satisfy 

In these expressions, T is the expiration date of the call option, r is the risk-free interest rate, K is the strike price, and $\sigma$ is the volatility. The function $N(x)$ is the probability that a standard normal random variable is less than x. For example, $N(d_{1})$ is given by 

$$
F (S _ {t}, t) = S _ {t} N (d _ {1}) - K e ^ {- r (T - t)} N (d _ {1} - \sigma \sqrt {T - t}),
$$

Under these conditions, the Black-Scholes formula can be obtained by solving the following PDE analytically: 

before the expiration date:
4. The price $S_{t}$ of the underlying security is a geometric Brownian motion with drift and diffusion terms proportional to $S_{t}$ .
5. Finally, there are no transaction costs, and assets are infinitely divisi-

We recall that the normal distribution has various symmetry properties. One of these states that with $f(x)$ standard normal density, we can write 

where the drift and the diffusion terms only depend on the observed underlying asset price $S_{t}$ . It is assumed that these coefficients satisfy the usual regularity conditions. $W_{t}$ is the usual Wiener process with probability measure P. 

5.1.1 Converting $e^{-r}S_{r}$ into a Martingale
We begin with the basic model that determines the dynamics of the underlying asset price $S_{r}$ . Suppose the underlying asset price follows the stochastic differential equation 

These conversions are done by a direct application of the Girsanov theorem. (The switching of probabilities from $P$ to $\bar{P}$ during the derivation of the Black-Scholes formula did not use the Girsanov theorem explicitly.) 

In order to show how the two approaches are related, we proceed in steps. In the first step, we show how $e^{-t}S_{t}$ can be converted into a martingale by switching the driving Wiener process, and the associated probability measure. In the second step, we do the same for the derivative asset $e^{-t}F(S_{t}, t)$ . 

Lemma is ascert.
In the following, Ito's Lemma will be applied to processes of the form $e^{-rt}F(S_t, t)$ . This requires that $F(\cdot)$ be twice differentiable with respect to $S_t$ , and once differentiable with respect to t. These assumptions will not be repeated in the following discussion. 

We show the correspondence between the PDE and martingale approaches in two stages. The first stage uses the symbolic form of Ito's Lemma. It is concise and intuitive, yet many important mathematical questions are not explicitly dealt with. The emphasis is put on the application of the Girsanov theorem. In the second stage, the integral form of Ito's Lemma is used. 

The discussion is a good opportunity to apply some of the more advanced mathematical tools introduced thus far. In particular, the discussion will be another example of the following: 

5 Comparing Martingale and PDE Approaches 

was zero.
The Black-Scholes formula can be obtained from either approach. One could either solve the fundamental PDE of Black and Scholes, or, as we did earlier, one could calculate the expectation $E^{\tilde{p}}[e^{-rT}F(S_{T},T)|I_{t}]$ explicitly using the equivalent measure P. In their original article, Black and Scholes chose the first path. The previous section derived the same formula using the martingale approach. This involved somewhat tedious manipulations, but was straightforward in terms of mathematical operations concerned.
Obviously, these two methods should be related in some way. In this section, we show the correspondence between the two approaches. 

The second method for pricing a derivative asset rested on the claim that we could find a probability measure $\tilde{P}$ such that under this probability, $e^{\pi F(S_{t},t)}$ becomes a martingale. This means that 

We have seen two contrasting approaches that can be used to calculate the fair market value of a derivative asset price. The first approach obtained the price of the derivative instrument by forming risk-free portfolios. In-finitesimal adjustments in portfolio weights and changes in the option price were used to replicate unexpected movements in the underlying asset, $S_{t}$ . This eliminated all the risk from the portfolio, at the same time imposing restrictions on the way $F(S_{t}, t)$ , $S_{t}$ and the risk-free asset could jointly move over time. The assumption that we could make infinitesimal changes in positions played an important role here and showed the advantage of continuous-time asset pricing models. 

## 5 Comparing Martingale and PDE Approaches

This gives the first part of the Black–Scholes formula and completes the derivation. We emphasize that during this derivation, no PDE was solved. 

According to the Girsanov theorem, if we define this SDE under the new probability $\tilde{P}$ , $\tilde{W}_t$ will be a standard Wiener process. In addition, $\tilde{P}$ will be a martingale measure if we equate the drift term to zero. This can be accomplished by picking the value of $dX_t$ as 

We assume that the integrability conditions required by the Girsanov theorem are satisfied by this $dX_{t}$ equaling the term in the brackets. This concludes the first step of our derivation. We now have a martingale measure $\bar{P}$ , a new Wiener process $\bar{W}_{t}$ , and the corresponding drift adjustment $X_{t}$ such that $e^{-\mu}S_{t}$ is a martingale and obcys the SDE 

5.1.2 Converting $e^{-\eta}F(S_t, t)$ into a Martingale
The derivation of the previous section gave the precise form of the process $X_t$ needed to apply the Girsanov theorem to derivative assets. To price a derivative asset, we need to show that $e^{-\eta}F(S_t, t)$ has the martingale property under $\tilde{P}$ . In this section, the Girsanov theorem will be used to do this. 

We go through similar steps. First we use the differential form of Ito's Lemma to obtain a stochastic differential equation for $e^{-t}F(S_t,t)$ , and then apply the Girsanov transformation to the driving Wiener process. Taking derivatives in a straightforward manner, we obtain 

$^{5}$ Here $rS_{i}dt$ is an incremental earning if $S_{i}$ dollars were kept in the risk-free asset, and $\mu_{i}dt$ is an actual expected earning on the asset during an infinitesimal period d. $^{6}$ This means, among other things, that the drift and diffusion parameters of the original system are well-behaved. 

$^{7}$ We know that if there are no arbitrage possibilities, the same $\tilde{P}$ will convert all asset prices into martingales. 

to the drift term. Note the subtle role played by this transformation. The $dX_{t}$ is defined such that the term $F_{s}\mu_{t}dt$ in Eq. (104) will be eliminated and will be replaced by $F_{s}rdt$ . 

This expression is identical to the fundamental PDE of Black and Scholes. With this choice of $dX_{t}$ , the derivative price discounted at the risk-free rate obeys the SDE 

But, in order for $e^{-t}F(S_{t},t)$ to be a martingale under the pair $\bar{W}_{t},\bar{P}$ , the drift term of this SDE must be zero. $^{7}$ This is the desired result: 

To do this we use the Girsanov theorem and find a new Wiener process and a new probability $\tilde{P}$ such that the discounted asset price becomes a martingale. The probability measure $\tilde{P}$ is called an equivalent martingale measure. This operation gives the drift adjustment term $X_{t}$ required by the Girsanov theorem. In the preceding derivation this was used twice, in (95) and in (106): 

Again, note the critical argument here. We know that the error term $d\tilde{W}$ , that drives Eq. (106) is a standard Wiener process only under the probability measure $\tilde{P}$ . Hence, $\tilde{P}$ becomes the relevant probability. The value of $dX$ , has already been derived in Eq. (97): 

In the martingale approach, we work with conditional expectations taken with respect to an equivalent martingale measure that converts all assets discounted by the risk-free rate into martingales. These expectations are very easy to conceptualize once the deep ideas involving the Girsanov theorem are understood. Also, in the case where the derivative asset is of the European type, these expectations provide an easy way of numerically obtaining arbitrage-free asset prices.
It was shown that the martingale approach implies the same PDEs utilized by the PDE methodology. The difference is that, in the martingale 

This chapter dealt with applications of the Girsanov theorem. We discussed several important technical points. In terms of broad conclusions, we retain the following. 

6 Conclusions 

(117) 

(116) 

a (trivial) martingale as well. But this is an integral taken with respect to time, and martingales are not supposed to have nonzero drift coefficients. Thus, the integral must equal zero. This gives the partial differential equation 

$$
\int_ {0} ^ {t} e ^ {- r u} \left[ - r F + F _ {t} + \frac {1}{2} F _ {s s} \sigma_ {u} ^ {2} + F _ {s} r S _ {u} \right] d u,
$$

is a martingale under $\hat{P}$ . But the derivative asset price discounted by $e^{-rt}$ is also a martingale. This makes the first integral on the right-hand side of (114), 

This is the Novikov condition of the Girsanov theorem and implies that the integral 

Note that we use $\bar{W}_{t}$ in place of $W_{t}$ , and consequently “replace” $\mu_{t}$ by r, the risk-free interest rate. 

$$
= F (S _ {0}, 0) + \int_ {0} ^ {t} e ^ {- r u} \left[ - r F + F _ {t} + \frac {1}{2} F _ {s s} \sigma_ {u} ^ {2} + F _ {s} r S _ {u} \right] d u
$$

The same analysis can be done using the integral form of Ito's Lemma. Without going over all the details, we repeat the basic steps. The value of a call option discounted by the risk-frec rate is represented as usual by $e^{-n}F(S_t,t)$ . Applying the integral form of Ito's Lemma, 

underentials. As emphasized several times earlier, the stochastic differentials under consideration are symbolic terms, which stand for integral equations in the background. The basic concept behind all SDEs is the Ito integral. We used stochastic differentials because they are convenient, and because the calculations already involved tedious equations. 

The relationship between the PDE and martingale approaches was discussed using the symbolic form of Ito's Lemma, which deals with stochastic differentials. 

Hence, into matrigation. Hence, the use of the same pair $\tilde{W}_t$ , $\tilde{P}$ in Girsanov transformations is a consequence of asset pricing theory. If arbitrage opportunities existed, we could not have done this. 

This step is related to equilibrium and arbitrage valuation of financial assets. It is in the domain of dynamic asset pricing theory. We briefly mention a rationale. As was discussed heuristically in Chapter 2, under proper conditions, arbitrage relations among asset prices will yield a unique martingale measure that will convert all asset prices, discounted by the risk-free rate, into martingales. 

formations. Here, we see this explicitly.
Finally, a third point. How do we know that the pair $\tilde{W}_{t}, \tilde{P}$ that converts $e^{-t}S_{t}$ into a martingale will also convert $e^{-t}F(S_{t}, t)$ into a martingale?
This question is important, because a function of a martingale need not itself be a martingale. 

In other words, the application of the Girsanov theorem amounts to transforming the drift term $\mu_{t}$ into $rS_{t}$ , the risk-free rate. Often, books on derivatives do this mechanically, by replacing all drift parameters with the risk-free rate. The Girsanov theorem is provided as the basis for such transformations. Here, we see this explicitly. 

2. In this exercise we work with the Black–Scholes setting applied to foreign currency denominated assets. We will see a different use of Gir-sanov theorem. [For more details see Musiela and Rutkowski (1997).]
Let r, f denote the domestic and the foreign risk-free rates. Let $S_{t}$ be the exchange rate, that is, the price of 1 unit of foreign currency in terms of domestic currency. Assume a geometric process for the dynamics of $S_{t}$ : 

Does this remind you of a well-known parity condition?
(b) Next, show that the value of the chooser option at time t is given by the same underlying asset. Let the $T$ be the expiration date, $S_{t}$ be the stock price, $K$ the strike price. If we buy the chooser option at time $t$ , we can choose between call or put with strike $K$ , written on $S_{t}$ . At time $t$ the value of the call is 

1. In this exercise we use the Girsanov theorem to price the chooser option. The chooser option is an exotic option that gives the holder the right to choose, at some future date, between a call and a put written on the same underlying asset. 

8 Exercises 

The section where we obtain the Black-Scholes formula follows the treatment of Ross (1993). Cox and Huang (1989) is an excellent summary of the main martingale results. The same is true, of course, of the treatment of Duffie (1996). 

7 References 

approach, the PDE is a consequence of risk-neutral asset pricing, whereas in the PDE method, one bcgins with the PDEs to obtain risk-free prices. 

$^{2}$ Morton (1973) was an early attempt to introduce stochastic interest rates. Yet, this was in a world where the underlying asset was again a stock. Such a complication can, by and large, still be handled by using classical tools. New tools start being more practical when the derivative is interest sensitive, in the sense that the payoff depends on the value and/or path followed by interest rates. 

In this chapter we briefly outline the basic ideas behind the new tools. The issues discussed in the following chapters are somewhat more advanced, 

This second part of the book discusses new tools required by such modifications and introduces the important new results applicable to term structure models. 

Finally, notice that Black-Scholes assumptions can be maintained as long as derivatives are short-dated, whereas the consideration of longer dated instruments may, by itself, be a sufficient reason for relaxing assumptions on constant interest rates and volatility. 

However, especially for interest rate derivatives, such an assumption can not be maintained. It is precisely the risk associated with the interest rate movements that makes these derivatives so popular. Introducing unpredictable Wiener components into risk-free interest rate models leads to some further complications in terms of mathematical tools. 

Second, it is obvious that risk-free interest rates are not constant. They are subject to unpredictable, infinitesimal shocks just like any other price. For some financial derivatives, such as options on stocks, the assumption of constant risk-free rate may be incorrect, but still is a reasonable approximation. 

These are serious restrictions for pricing a large majority of financial derivatives. $^{2}$ 

Recall that the examples discussed in previous chapters were by and large in line with the basic Black-Scholes assumptions. In particular, two aspects of Black-Scholes framework were always preserved. 

$^{1}$ Robustness of Black-Scholes assumptions is one reason why the formula continues to be very popular with market professionals. For example, one still obtains reasonably accurate prices when volatility is stochastic, or when interest rates move randomly. A comprehensive source on this aspect of Black-Scholes formula is El Karoui et al. (1998) 

These new instruments may be similar in some ways to the plain-vanilla derivatives already discussed. Yet, there are some nontrivial complications. More importantly, some new results have recently been obtained in dealing with interest-sensitive instruments and term structure of interest rates. These powerful results require a different set of quantitative tools in their 

The types of derivative securities traded in financial markets are much more complicated than such “plain vanilla” call or put options that may fit this simplified framework reasonably well. In fact, some of the assumptions used by Black-Scholes, although often quite robust, may fall significantly short in the case of interest-sensitive securities. $^{1}$ New assumptions introduced in their place require more complicated tools. 

The first part of this book dealt with an introduction to quantitative tools that are useful for Classical Black-Scholes approach, where underlying security $S_{i}$ was a nondividend-paying stock, the risk-free interest rate $r$ and the underlying volatility $\sigma$ were constant, the option was European, and where there were no transactions costs or indivisibilities. 

## 1 Introduction

# New Results and Tools for Interest-Sensitive Securities

$^{4}$ Libor is the London Interbank Offered Rate. It is an interbank rate asked by sellers of funds. It is obtained by polling selected banks in London and then averaging the quotes. Hence, depending on the selection of banks, there may be several Libor rates on the same maturity. The British Bankers Association calculates an “official” Libor that forms the basis of most of these Libor Instruments. 

$^{3}$ In the following, the reader will notice a slight change in notation. In particular, the time subscript will be denoted by $t_{i}$ . This is required by the new instruments. 

For example, forward loans for the period $[t_i, t_{i+1}]$ can be contacted at time $t$ , with an interest rate $F_t$ . The buyer of the forward will receive, as 

* Interest rate futures and forwards. Let $L_{i}$ represent the annualized simple interest rate on a loan that begins at time $t_i$ and ends at time $t_{i+1}$ . Suppose there are no bid-ask spreads or default risks involved. Then, at time $t_i$ , where $t < t_i < t_{i+1}$ , we can write futures and forward contracts on these “Libor rates,” $L_{i}^{4}$ . 

One of the most important classes of derivative instruments that violate the assumptions of Black-Scholes environment are derivatives written on interest-sensitive securities. 

3 Interest Rate Derivatives 

These mathematical tools are particularly useful in case of interest sensitive derivatives. Hence, before we proceed with the discussion of the tools, we need to discuss briefly some of these instruments. This is done in the following section. 

Stopping times are random variables whose outcomes are some particular points in time where a certain process is being "stopped." For example, an American-style call option can be exercised before the expiration date. Initially, such execution times are unknown. Hence, the execution date of an option can be regarded as a random variable. Stopping times provide the mathematical tools to incorporate in pricing the effects of such random variables. 

Finally, Chapter 22 discusses stopping times, which are essential in dealing with American style derivatives. This concept is introduced along with a certain algorithm called dynamic programming that is very important in its own right. In this chapter we also show the correspondence between using binomial trees for American-style securities and stopping times. We see that the pricing is based on applications of dynamic programming. 

process, a property which complicates the utilization of Feynman-Kac type correspondences. 

3 Interest Rate Derivatives 

simpler (of cheaper) numerical calculations. Some of the other concepts introduced in Chapter 21 are the generator of a stochastic process, Kolmogorov's backward equation, and the implications of the so-called Markov property. The latter is especially important for models of short rate, because the latter is shown not to behave as a Markov 

Chapter 20 is a discussion of the so-called classical PDE approach to fixed income. Chapter 21 deals with the recent tools that are utilized in pricing, hedging, and arbitraging interest rate sensitive securities. The first topic here consists of the fundamental relationship that exists between a class of conditional expectations of stochastic processes and some partial differential equations. Once this correspondence is established, financial market participants gain a very important tool with practical implications. This tool is related to the Feynman-Kac formula and it is dealt with in this chapter. Using this “correspondence,” one can work either with conditional expectations taken with respect to martingale measures, or with the corresponding PDEs. The analyst could take the direction which promises simpler (or cheaper) numerical calculations. 

Chapter 19 discusses classical PDE analysis for interest-sensitive securities. This approach can be regarded as an attempt to follow steps similar to those used with Black-Scholes PDE, and then obtaining PDEs satisfied by default-free zero-coupon bond prices and derivatives written on them. The main difficulty is to find ways of adjusting the drift of the short-rate process. Short-rate is not an asset, so this drift cannot be replaced with the risk-free spot rate, r, as in the case of Black-Scholes. A more complicated operation is needed. This leads to the introduction of the notion of a market price of interest rate risk. The corresponding PDEs will now incorporate this additional (unobserved) variable. 

The major topic of Chapter 18 is the foundations for modeling the term structure of interest rates. The definitions of a forward rate, spot rate, and term structure are given here formally. More important, Chapter 18 introduces the two broad approaches to modeling term structure of interest rates, namely, the classical and the Heath-Jarrow-Morton approach. Learning the differences between the assumptions, the basic philosophies, and the practical implementations that one can adopt in each case, is an important step for understanding the valuation of interest-sensitive instruments. 

Chapter 17 will reintroduce the simple two-state framework that motivated the first part of this book. But, in the new version of models used in Chapter 2, we will complicate the simple set-up by allowing for stochastic short rates and by considering interest-sensitive instruments. This way, we can motivate important concepts such as normalization and tools such as the forward measure. 

370 CHAPTER 16 Results and Tools for Interest-Sensitive Securities 

Otherwise, the holder receives nothing. That the caplet is equivalent to a call option on $L_{t_i}$ with a strike $R_{cap}$ is also seen in Figure 2. Here, if we view the caplet as a call with expiration date $t_{i+1}$ , written on the Libor rate $L_{t_j}$ , then it should be kept in mind that the settlement will be done at time $t_{i+1}$ , rather than at time $t_i$ . An interest rate floorlet, can similarly be shown to be equivalent to a call option with expiration $t_j$ , on a discount bond with maturity $t_{i+1}$ . 

This formulation is shown in Figure 2. At time $t_i$ the option expires. If the price of the bond is lower than $100 / (1 + R_{cup}\delta)$ , then the holder receives the difference: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/20a18da772024adad199ff80efb9c9e72801a4d0d2cfad9e6da2df5fbf8aab71.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/6f6ae499af255c26392672e2b8d507a6724937b361686a676bc2cfacbc385b27.jpg)


$^{5}$ For example, it is equal to the number of days during $[t_{1}, t_{1+}]$ divided by 365. 

where $L_{t_{i}}$ is the underlying Libor rate observed at time $t_{i}$ , the $\delta$ is the days adjustment, and the N is a notional amount to be decided at time t. The $R_{cap}$ is the cap rate which plays the role of a strike price. In a sense, a caplet will compensate the buyer for any increase in the future Libor rates beyond the level $R_{cap}$ . Thus, it is equivalent to a purpose with expiration date $t_{i}$ , written on a default-free discount bond with maturity date $t_{i+1}$ , with a strike price obtained from $R_{cap}$ . In particular, the strike price that applies to this option is the $100/(1 + R_{cap}\delta)$ , where $R_{cap}$ is the cap rate, and the $\delta$ is, as usual, the days adjustment. 

## $N\max \left[\delta (L_{t_i} - R_{cap}),0\right],$

Suppose $t$ denotes the present and let $t_0, t \leq t_0$ be the starting date of an interest rate cap. Let $t_n$ be the ending date of the cap for some fixed $n, t < t_0 < t_n$ . Let the $t_1, t_2, \ldots, t_{n-1}$ be reset dates. Then for every caplet that applies to the period $t_i, t_{i+1}$ , the buyer of the cap will receive, at time $t_{i+1}$ , the sum 

is also shown in Figure 1.
- Caps and floors. Caps and floors are among some of the most liquid interest rate derivatives. Caps can be used to hedge the risk of increasing interest rates. Floors do the same for decreasing rates. They are essentially baskets of options written on Libor rates. 

if it is negative. The FRA rate $F_{t}$ is selected so that the time $t$ price of the FRA contract equals zero. This situation is shown in Figure 1. In case of FRAs traded in actual markets, often the payment is made at the same time the $L_{t}$ is observed. Hence, it has to be discounted by $(1 + L_{t}, \delta)$ . This is also shown in Figure 1. 

## $N[F_t - L_{t_i}]\delta,$

if it is positive, or pays 

a loan, a certain sum N at time $t_{i}$ and will pay back at time $t_{i+1}$ the sum $N(1 + F_{t}\delta)$ , where the $\delta$ is the days adjustment factor. $^{5}$ • Forward rate agreements (FRA). Already discussed in Chapter 1, these instruments provide a more convenient way of hedging interest rate risk. Depending on the outcome of $F_{t} > L_{t}$ , or $F_{t} < L_{t}$ , the buyer of a FRA paid-in-arrears receives, at time $t_{i+1}$ , the sum 

372 CHAPTER • 16 Results and Tools for Interest-Sensitive Securities 

Payoff at $\left[(L_{\mathrm{tf}} - R_{\mathrm{cap}})\delta\right]$ 

Third, the payouts of the underlying security may be different for interest rate derivatives. For example, in case of mark-to-market adjustments the fact that spot rates are stochastic will, in general, make a difference in evaluating an arbitrage-free futures price compared to forward prices. This is the case because with mark-to-market adjustments the holder of the contracts makes/receives periodic payments that fluctuate as interest rates change. But these mark-to-market cash flows will also be discounted by stochastic discount factors that are affected by the same interest rate movements. The resulting futures prices may be different from the price of a forward contract that has no mark-to-market requirement. 

The second complication is that most interest rate derivatives may be American style and any explicit or implicit options may be exercised before their respective expiration date, if desired. 

Thus, the very first requirement is that we work with stochastic interest rates. But then, the resulting discount factors and the implied payoffs would be dependent on interest rates. Clearly this would make arbitrage-free pricing more complicated. 

The price of a bond $B_{t}$ depends on the stochastic behavior of the current and future spot rates in the economy. Hence, at the outset, two new assumptions are required. (1) Bond price $B_{t}$ must be a function of the current and future spot rates, and (2) the spot rate $r_{t}$ cannot be assumed constant, because this would amount to saying that $B_{t}$ would be completely predictable, which in turn would mean that the volatility of the underlying security is zero. Hence, there would be no demand for any call or put options written on the bond. 

Introducing interest rate derivatives leads to several complications. This is best seen by looking at bond options, and then comparing these with the Black-Scholes framework. 

These are some of the basic interest rate derivatives. The scope of this book prevents us from going into more exotic products. Instead, we now would like to summarize some key elements of these instruments and see what types of new tools would be required. 

rates $L_{i}$ : Swaptions. Swaptions are options written on swap contracts. Depending on maturity they are very liquid. At time t a practitioner may buy an option on a swap contract with strike price κ and notional amount N. 

- Bond options. A call option written on a bond gives its holder the right to buy a bond with price $B_{t}$ at the strike price $K$ . Since the price of a bond depends on the current and future spot rates, bond options will be sensitive to movements in $r_{t}$ or for that matter, to movements in Libor expires at time $t_{t+1}$ .

• Interest rate swaps. These instruments were also discussed in Chapter 1.

Plain vanilla interest rate swaps paid in-arrears involve an exchange of cash flows generated by a fixed pre-set swap rate $\kappa$ against cash flows generated by floating Libor rates $L_t$ . The cash flows are based on a notional amount $N$ and are settled at times $t_{t+1}$ . Clearly, a swap is a more complex form of a sequence of FRAs. The swap rate $\kappa$ is set so that the time $t$ price of the swap contract equals zero. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/2ae941e72dfc1b966cb27fc118ba649d39d50b32c7ed15065ce2b66540cb13b3.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/95d828157b3cfbd0bf6905f2325efb8f5917e19bdf729f038412c072fb1a193d.jpg)


The book of readings published by Risk, "Vasicck and Beyond," is highly recommended as an excellent collection of readings concerning interest rate 

6 References 

This chapter is simply a brief summary and cannot be considered an introduction to interest-sensitive securities. It has, however, the bare minimum necessary for understanding the tools discussed in the remaining chapters. 

5 Conclusions 

Some of these complications can be handled within a Black-Scholes framework by either making small modifications in the assumptions or by "tricking" them in some ingenious way. But the early exercise possibility of interest rate derivatives and stochastic interest rates are two modifications that have to be incorporated in derivative asset pricing using new mathematical tools. The following chapters are intended to do this. 

Last but not least, there is the modeling of volatilities. The volatility of a bond has to vary over time. After all, the bond matures at some specific date. Hence, these volatilities cannot be assumed constant as in the case of stocks. 

Note that in case of a classical Black-Scholes environment, modeling the risk-free dynamics of the underlying asset meant modeling a single SDE, where over-time arbitrage restrictions on a single variable had to be taken into account. But in the case of interest rates, the same over-time restrictions need to be modeled for k-variables. There is more. Now, arbitrage restrictions across variables need to be specified as well. 

Thus, in contrast to the Black-Scholes case for interest rates, one would deal with a vector of random processes that must obey complex interrelations due to arbitrage possibilities. The resulting k-dimensional dynamics are bound to be more complicated. 

Another complication is the coexistence of many interest rates. Note that within the simple Black-Scholes world, there is one underlying asset S. Yet within the fixed-income sector, there are many interest rates implied by different maturities. Moreover, these interest rates cannot follow very different dynamics from each other because they relate, after all, to similar instruments. 

4.2 Term Structure 

which is possible when $S_{t}$ is a traded asset. Fundamental theorem of finance would then imply this equality. Yet $r_t$ not being an "asset," a similar substitution is not valid. 

$r = (a\mu - \lambda_{i}\sigma)$ , 

And, it is not clear at the outset how $\lambda_{i}$ can be determined. This is a significant complication compared to the Black-Scholes substitution: 

$d\tau_{i} = (a(r_{i},t) - \lambda_{i}\sigma (r_{i},t))dt + \sigma (r_{i},t)d\vec{W}_{i}$ . 

The modifications of interest rate dynamics require: 

## $dW_{t} = d\tilde{W}_{t} - \lambda_{t}dt.$

the drift $a(r_{t}, t)$ has to be risk-adjusted by other means. This makes the practical application of Girsanov theorem much more complicated. In fact, the switch from $W_{t}$ to a new Wiener process, $\tilde{W}_{t}$ , defined under the risk-free measure $\tilde{P}$ , cannot be done in a straightforward way. Given the Girsanov correspondence between the two Wiener processes: 

and then replacing it with the risk-free rate, $r$ , is not a valid procedure anymore. In the dynamics of $r$ written as, 

Interest rates are not assets, they are more like “returns” on assets. This means that the arbitrage-free restriction that consists of removing the unknown drift, $\mu$ , of an asset price $S_{p}$ , in the dynamics: 

4.1 Drift Adjustment 

Similarly, if a bond makes coupon payments, the underlying security, $B_{t}$ , will also be different than a no-dividend paying stock, $S_{t}$ . These are some of the obvious modifications that are required to deal with interest rate derivatives. There are also some more technical implications that may not be as obvious at the outset. One of these was mentioned above. 

376 CHAPTER·16 Results and Tools for Interest-Sensitive Securities 

This chapter attempts to motivate these notions and introduces the new tools by using a simple discrete-state approach similar to the one utilized in Chapter 2. However, the model is extended in new directions so that these new tools and concepts can also be easily understood. By expanding 

Chapter 2 considered a model where lending and borrowing at a constant risk-free rate was one of the three possible ways of investing, the other two being stocks and options written on these stocks. Throughout Chapter 2 interest rates were assumed to be constant and a discussion of interest-sensitive financial derivatives was deliberately omitted. Yet, in financial markets a large majority of the instruments that trade are interest-sensitive products. These are used to hedge, to arbitrage the interest rate risk, and to speculate on it. Relaxing the assumption of constant interest rates is, thus, essential. As mentioned in Chapter 16, relaxing the assumption of constant interest rates and then introducing complex interest rate derivatives creates a need for new mathematical tools, most of which were discovered only lately. 

The motivation for the main tools in derivatives pricing was introduced in the simple model of Chapter 2. There we discussed a simple construction of synthetic (martingale) probabilities that played an essential role in the first part of this book. Because the setting was very simple, it was well-suited for motivating complex notions such as risk-neutral probabilities and the crucial role played by martingale tools. 

## 1 Introduction

Normalization and Random Interest Rates 

## CHAPTER 17

(c) A caplet
(d) A caplet
(e) Returns on 30-year German Bonds
(f) Volatility of Federal Funds rate
(g) An interest rate swap 

(a) 6-month Libor
(b) A 5-year Treasury bond
(c) A FRA contract 

2. Which one(s) of the following are assets traded in financial markets: 

was exactly 6 months ago.
(e) A swaption that expires in 6 months on a 2-year fixed payer swap with swap rate $\kappa = 6\%$ . 

(d) A fixed payer interest rate swap with swap rate $\kappa = 7.5\%$ . The swap has maturity 2 years and receives 6-month Libor. Start date 

contracted price is 89.5.
(c) A 3 by 6 FRA contract that pays the fixed 3-month rate, F, against fiber 

$L_{t}$ that is about to expire.
(b) A forward contract written on a default-free discount bond with maturity 2 years. The forward contract expires in 3 months. The 

(a) A caplet with cap rate $R_{cap} = 6.75\%$ written on 3-month Libor I that is about to evira 

1. Plot the payoff diagrams for the following instruments: 

7 Exercises 

378 CHAPTER·16 Results and Tools for Interest-Sensitive Securities derivatives and their pricing. The reader should also consult Hull (2000) and the extensive treatment in Rebonato (1998). 

where $\Delta$ is the time that elapses between the two time periods, the $u$ and the $d$ represent the two states under consideration, and the $\{\psi^u > 0, \psi^d > 0\}$ are state prices. The first row represents the payoffs of risk-free lending and borrowing, the second row represents the payoffs of the stock $S_t$ , and the third row represents payoffs of the option $C_t^2$ . 

$^{1}$ One can also ask the following question. Given that we want to convert asset prices into martingales by modifying the true probability distribution, is there a way we can choose that synthetic measure in some “best” way? 

this complex idea in a simple setting.
It is also the case that earlier chapters dealt with a very limited number of derivative instruments. Most discussion centered on plain vanilla options within the Black–Scholes environment. Occasionally, some forward contract 

This simple step, which appears at the outset inconsequential, turns out to be very important for the practical utilization of synthetic probabilities, or "measures," as a pricing tool in finance. In fact, we discover that choosing one measure over another equally "correct" probability can simplify the pricing effort dramatically. The second objective of this chapter is to explain this complex idea in a simple setting. $^{1}$ 

It turns out that once interest rates become stochastic, we have new ways of searching for synthetic probabilities, especially when we deal with interest-sensitive instruments. Although the general philosophy of the approach introduced in Chapter 2 remains the same, the mechanics change in a dramatic way. In fact, one can show that using different synthetic probabilities will be more practical for different classes of financial derivatives. Obviously, the final arbitrage-free price that one obtains will be identical in each case. After all, what matters is not the synthetic probability, but the underlying unique state-price vector. Yet some synthetic probabilities may be more practical than others. 

In order to start discussing the issue of normalization, we first let the short rate fluctuate randomly from one period to another and then try to see whether basic results obtained in Chapter 2 remain the same. Clearly, this makes the discussion directly applicable to interest-sensitive derivatives, given that pricing of such securities needs to assume stochastic interest rates. But this is not the main point. 

The first set of issues can be grouped under the concept of normalization. This is the technique of obtaining pricing equations for ratios of asset prices instead of prices themselves. A ratio has a numerator and a denominator. In a dynamic setting both of these change. The expected rate of change of each element may be unknown, but under some conditions, the expected rate of change of the ratio of the two, may be a known number. For example, the numerator and denominator of a deterministic ratio may grow at the same unknown rate. But the ratio itself will stay the same. Thus, if the numerators and denominators in pricing formulas are carefully selected, and if the Girsanov theorem is skillfully exploited, modeling of asset price dynamics can be greatly simplified. 

the simplified framework of Chapter 2, one can discuss at least three major additional results. 

CHAPTER·17 Arbitrage Theorem 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/8146f971aeddc195cb6e24a795e219a98eba51ab35e39988ac8718f43ca49496.jpg)


It turns out that a minimum of two time periods is necessary to factor in the effects of the random spot rate $r_{i}$ . The situation is shown in Figures 1 and 2. An investor who would like to lend his or her money between $t_{1}$ and $t_{2}$ does this at the risk-free rate contracted at time $t_{1}$ . Then, no matter which state occurs in the immediate future, his or her return is not risky, 

$\{\omega_{1} = down, down \quad \omega_{2} = down, up \quad \omega_{3} = up, up \quad \omega_{4} = up, down\}$ . 

We consider two periods described by dates $t_{1} < t_{2} < t_{3}$ , but keep the assumption of two possible states in each time period the same. Adding one more time period still increases the number of possibilities. This way, in looking at time $t_{3} = 1 + 2\Delta$ from time $t_{1} = 1$ there will be four possible states, $\{\omega_{i}, i = 1, \ldots, 4\}$ , describing the possible paths the prices can follow at time-nodes $\{t_{1}, t_{2}, t_{3}\}$ : 

## 2.1 The New Environment

In the next section we extend this framework in two ways. First, we add another time period so that the effects of random fluctuations in the spot rate can be taken into account. Second, we change the types of instruments considered and introduce interest-sensitive securities. 

Thus, the probability $\tilde{P}$ “modified” expected returns of the risky assets so that all expected returns became equal to the risk-free rate r. Hence, the term risk-neutral measure or probability. 

as if they come from a risk neutral work. There was a second important result that was obtained from these pricing equations. Rearranging (4) and (5), we get 

In $E_{t}$ : I to simplify the notation in this chapter. According to these pricing equations, expected future payoffs of the risky assets discounted by the risk-free rate give the current arbitrage-free price. It is in this sense that $\bar{P}_{u}, \bar{P}_{d}$ are “risk-neutral.” Even though market prices $S_{t}, C_{t}$ , contain risk premia, they are nevertheless obtained using the $\bar{P}_{u}, \bar{P}_{d}$ , as if they come from a risk-neutral world. 

where the $E^{\hat{p}}[\cdot]$ denotes, as usual, the (conditional) expectation operator that uses the probabilities $\tilde{P}^{u}, \tilde{P}^{d}$ . Note that we are omitting the t subscript in $E_{t}^{\hat{p}}[\cdot]$ to simplify the notation in this chapter. 

$$
= \frac {1}{(1 + r \Delta)} E ^ {\bar {r}} [ C _ {i + \Delta} ],
$$

$$
C _ {t} = C _ {t + \Delta} ^ {u} \frac {1}{(1 + r \Delta)} \frac {\tilde {p} ^ {u}}{1} + C _ {t + \Delta} ^ {d} \frac {1}{(1 + r \Delta)} \tilde {p} ^ {d}
$$

$$
= \frac {1}{(1 + r \Delta)} E ^ {\tilde {P}} [ S _ {t + \Delta} ]
$$

$$
S _ {t} = S _ {t + \Delta} ^ {u} \frac {1}{(1 + r \Delta)} \frac {\tilde {p} ^ {u}}{(\mathrm{I} + r \Delta)} + S _ {t + \Delta} ^ {d} \frac {1}{(1 + r \Delta)} \frac {\tilde {p} ^ {d}}{(\mathrm{I} + r \Delta)}
$$

$$
C _ {t} = C _ {t + \Delta} ^ {u} \psi^ {u} + C _ {t + \Delta} ^ {d} \psi^ {d}.
$$

$$
S _ {i} = S _ {i + \Delta} ^ {u} \psi^ {u} + S _ {i + \Delta} ^ {d} \psi^ {d}
$$

prices $\psi^u, \psi^u$ . Thus with $\tilde{P}^u, \tilde{P}^d$ we had two numbers that were positive and that summed to one. These satisfy the requirements of a probability distribution within this simple setting, and hence, we called the $\tilde{P}^u, \tilde{P}^d$ synthetic, or more precisely, risk-neutral probabilities. These probabilities, which said nothing about the real-world odds of the states $u, d$ , were called "risk-neutral" due to the following. 

$^{6}$ In this context, the liquidity of markets means that the assets can be instantaneously bought and sold at the quoted prices. 

$^{7}$ As defined in the previous chapter, Libor is the London Interbank Offered Rate, an interest rate at which banks can borrow money in London. Libor rates are used as benchmarks and Libor-based instruments form an important proportion of assets in bank balance sheets. 

extends arbitrage pricing to more interesting assets and, at the same time, gives us an easy way of showing why changing normalization is a useful tool for the financial market practitioner. In particular, within this framework we will be able to introduce the so-called forward measure and compare its properties with the risk-neutral measure seen earlier.

Hence, we assume that there are liquid markets for the following instruments $^{6}$ 

$^{5}$ This shows that the term “risk-free” investment is not entirely appropriate for a savings (or money market) account. The investment is risk-free in the sense that what will be received at the end of the contract is known. The contract has no “market” risk. Its price will not fluctuate during the contract period because the $r_{i}$ is constant. In addition, we assume that there is no default-risk either. So the payoff at the end of the contract period is constant. Yet, an investor who keeps his or her funds in the savings account will experience random fluctuations in the payoffs if this investment is rolled-over. 

$^{3}$ It is assumed that there is no default risk in this setting. 

The second modification that we introduce to Chapter 2 is in the selection of instruments. Instead of dealing with stocks and options written on these stocks, we consider interest-sensitive securities and forwards. This 

But as we add one more time period this changes. Looked at from time $t_{1}=1$ , the spot rate that the investor will be offered at time $t_{2}=1+\Delta$ will present some risks. By staying with this type of investment, the investor may end up lending his or her money either at a “high” rate of interest $r_{t_{2}}^{d}$ , or at a “lower” rate $r_{t_{2}}^{u}$ . Which of these spot rates will be available at $t_{2}$ is not known at time $t_{1}$ . Thus, with three time-nodes $t_{1}, t_{2}, t_{3}$ , the randomness of the “risk-free” rates will be an important factor, although with the one-period framework of Chapter 2 this randomness was not relevant. This situation was presented in Figure 1. For time-node $t_{2}$ we have two possible spot rates, $r_{t_{2}}^{u}$ and $r_{t_{2}}^{d}$ , and hence the value of $r_{t_{2}}$ is random. $^{5}$ 

because the payoff is known. $^{3}$ Regardless of the state up or down that may occur at $t_{2}$ , the investor will receive the same income $(1+r_{t},\Delta)$ . Because the riskless borrowing and lending yields the same return whether the up and down state occurs, in a model where there are two time-nodes, $t_{1}$ , $t_{2}$ , it will be as if the spot rate does not fluctuate. So the effect of any randomness in $r_{t}$ cannot be analyzed. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/42afe41f-1073-45b5-8111-5489c3317109/b6f72ae55cbef6244b2186bb4d5cb57feac05deaae1cb546ea7388610f91da4e.jpg)


This is the case, for example, for most forward Rate Agreements, traded in the market. But, because this type of settlement will involve a ratio of two random variables, they will introduce some further complications, called the FRA-adjustment. By assuming that the contract is settled at time $t_3$ we avoid such nonlinearities at this initial stage. In addition, most interest-rate derivatives settle in-arrears anyway. 

$^{8}$ Under some conditions the forward contracts may involve an immediate settlement at time $t_{2}$ . Then, the payment (receipt) will equal the present value of the difference, and will be given by 

tive security written on one or more of these assets. Finally, the $\{\psi^{ij}, i,j = u,d\}$ are the 4 state prices for time $t_3$ . They exist and they are positive if and only if there are no arbitrage opportunities. As 

The third and fourth rows of the matrix equation deal with the two bonds we included in the system. The $B_{t_1}^s$ and $B_{t_1}$ denote the time- $t_1$ arbitrage-free prices of the two zero-coupon bonds, the first maturing at time $t_3$ , the second at some future date $T$ , respectively. Note that the value of the short bond is constant and equal to one at $t_3$ because this happens to be the maturity date. On the other hand, the price of the long bond does not have this property. There are four possible values that $B_{t_3}$ can assume. The last row of the matrix equation represents the price, $C_{t_1}$ , of a deriva-

Next, consider the second row of this matrix equation. The $F_{t_1}$ is a forward rate contracted at time $t_1$ on the random Libor rate $L_{t_2}$ , which will be observed at time $t_2$ . Hence, we have here a Forward Rate Agreement. It turns out that FRAs have the arbitrage-free value zero at contract-time, because no up-front payment is required for signing these contracts. This explains the second element of the vector on the left-hand side. Also, according to this FRA contract, the difference between the known $F_{t_1}$ and the unknown $L_{t_3}$ will be paid (received) at time $t_3$ , and this explains the second row of the matrix. Clearly, there are four possibilities here. $^8$ 

The first row of this system describes what happens to an investment in the “risk-free” savings account. If one dollar is invested here, it will return a known $R_{t_{1}} = (1 + r_{t_{1}})$ at time $t_{2}$ and an unknown $R_{t_{2}} = (1 + r_{t_{2}})$ at time $t_{3}$ . Time $t_{3}$ return is random because, in contrast to $R_{t_{1}}$ , the $R_{t_{2}}$ is unknown at time $t_{1}$ . At time $t_{2}$ , there are two possibilities, and this is indicated by the superscripts u, d on the $R_{t_{2}}^{d}, R_{t_{2}}^{u}$ . This row is similar to the first row in Eq. (1), except here the elements are not constant. 

387 

where the right-hand side consists of the product of possible payoffs at time $t_{3}$ , multiplied by the states prices $\psi^{ij}$ . This matrix equation is similar to the one used in Chapter 2, yet, given the new complications, several comments are in order. 

2 A Model for New Instruments 

$$
\left[ \begin{array}{cc} 1 & \\ 0 & \\ B _ {t _ {1}} ^ {s} & \\ B _ {t _ {1}} ^ {s} & \\ C _ {t _ {1}} & \end{array} \right] = \left[ \begin{array}{cccc} R _ {t _ {1}} R _ {t _ {2}} ^ {u} & R _ {t _ {1}} R _ {t _ {2}} ^ {u} & R _ {t _ {1}} R _ {t _ {2}} ^ {d} & R _ {t _ {1}} R _ {t _ {2}} ^ {d} \\ (F _ {t _ {1}} - L _ {t _ {2}} ^ {u}) (F _ {t _ {1}} - L _ {t _ {2}} ^ {u}) & (F _ {t _ {1}} - L _ {t _ {2}} ^ {d}) & (F _ {t _ {1}} - L _ {t _ {2}} ^ {d}) & [ \psi^ {u u} ] \\ 1 & 1 & 1 & 1 \\ B _ {t _ {3}} ^ {u u} & B _ {t _ {3}} ^ {u d} & B _ {t _ {3}} ^ {d u} & B _ {t _ {3}} ^ {d d} \\ C _ {t _ {3}} ^ {u u} & C _ {t _ {3}} ^ {c u d} & C _ {t _ {3}} ^ {d u} & C _ {t _ {3}} ^ {d d} \end{array} \right]\left[ \begin{array}{c} \psi^ {u u} \\ \psi^ {u d} \\ \psi^ {d u} \\ \psi^ {d d} \end{array} \right],
$$

Now we can write the matrix equation implied by the Fundamental Theorem of Finance. Stacking the current prices of the five instruments discussed above in a $(5\times 1)$ vector on the left-hand side, we obtain the relation: 

Finally, we assume that all interest rates are expressed as rates over periods of length $\Delta$ . This way we do not need to multiply an “annual” rate $r_{t}$ by a factor of $\Delta$ to obtain corresponding returns. This is also intended to simplify the notation. Alternatively one can take $\Delta = 1$ as equaling one 

represent the price of the “long” bond at times $t_{1}$ and $t_{3}$ , respectively. We do not need to consider the price of the long bond for the interim period $t_{2}$ . Then, we set the notional amount of the FRA contract denoted by N equal to 1, because this parameter plays an inconsequential role in our model. 

$B_{t_1} = B(t_1,T)$ $B_{t_3} = B(t_3,T)$ 

which represents the price of the "short" bond at current period $t_1$ , and let the 

Although we will revert back to the original notation in later chapters, for the sake of simplifying the matrix equation discussed below, we simplify the notation for bonds as well. We let 

$\begin{array}{r}R_{t_1} = (1 + r_{t_1}\Delta)\\ R_{t_2} = (1 + r_{t_2}\Delta). \end{array}$ 

We now need to stack these assets and the corresponding payoffs in a matrix equation similar to the one used in Chapter 2. But, first we make some notational simplifications.
We define the gross risk-free returns for periods $t_{1}$ and $t_{2}$ as follows: 

CHAPTER·17 Arbitrage Theorem 

As mentioned earlier, under the risk-neutral measure $\tilde{P}$ , asset prices will have trends. Indeed, under $\tilde{P}$ , all expected returns are converted to $r$ and this means that they will drift upwards. Thus, the prices themselves will not be martingales under $\tilde{P}$ . But, by "normalizing" with risk-free lending, 

Nevertheless, the point to remember here is that the process of introducing the risk-neutral probabilities in the pricing equations resulted in the “normalization” of each state’s return by the corresponding return of risk-free lending. In fact, the substitution of $\tilde{P}^{u}$ for $\psi^{i}$ is equivalent to dividing every possible entry in the matrix Eq. (1) by the corresponding entry of the first row, which represents the payoff of the risk-free investment. 

$$
S _ {t} = \frac {1}{(1 + r \Delta)} \left[ S _ {t + \Delta} ^ {u} \tilde {P} ^ {u} + S _ {t + \Delta} ^ {d} \tilde {P} ^ {d} \right].
$$

Now, during this operation, when the $\tilde{P}^{i}$ arc substituted for the $\psi^{i}(1+r\Delta)$ , an extra factor is left in the denominator of each $S_{t+\Delta}^{i}$ term. This factor is $(1+r\Delta)$ , and represents the return of the risk-free investment in that particular state. But, recall that one-period-ahead risk-free return is constant, and hence this factor was successfully factored out to give: 

$$
S _ {t} = \frac {S _ {t + \Delta} ^ {u}}{(1 + r \Delta)} \tilde {p} ^ {u} + \frac {S _ {t + \Delta} ^ {d}}{(1 + r \Delta)} \tilde {p} ^ {d}.
$$

$$
S _ {t} = S _ {t + \Delta} ^ {\mu} \psi^ {\mu} \frac {(1 + r \Delta)}{(1 + r \Delta)} + S _ {t + \Delta} ^ {d} \psi^ {d} \frac {(1 + r \Delta)}{(1 + r \Delta)}
$$

Again we begin with a review of the framework in Chapter 2. Consider how the risk-neutral probabilities were obtained given the Fundamental Theorem of Finance. More precisely, take the equation for $S_{t}$ given by Equation (1) and earlier in Chapter 2: 

two periods and four states of the world is the smallest system in which the issue of normalization can be discussed. 

An alternative is to consider a two-period Libor. But this would require a three-period model which will lead to a much more complicated matrix equation than the one considered here. In this sense, the compromise of 

2.1.1 A Remark
In this chapter the $R_{t}$ and the $L_{t}$ denote the short rate and the Libor process, respectively. In principle, these two are different processes, with $L_{t}$ having a different maturity than the spot rate, which is by definition the rate on the shortest possible tenor. But, because we want to keep the instruments and the model at a minimum level of complication, we assume that the $L_{t}$ is the one-period Libor. This would make $R_{t}$ and $L_{t}$ the same, but even with this consideration all results of this chapter still hold. The chapter treats these as if they are different notationally because with longer maturity Libor rates this equivalence will disappear. Using different notation for $L_{t}$ and $R_{t}$ will help us better understand the Libor instruments and their relationship to spot rates in these more general cases. 

We can now consider the important issue of normalization that determines the choice of measure for the instruments under consideration. But first we need the following caveat. 

Finally, note a straightforward aspect of the model. Because one of the bonds matures at time $t_{3}$ , its payoff is known and is constant at that time. This simple point will have important implications for choosing a synthetic probability (martingale measure) that is more convenient for pricing the new assets introduced here. 

superscript indicating this dependence on the realized state at the $t_2$ . Second, note that the securities included in this model are quite different from those of Chapter 2. The forward contract and the bonds considered here are interest-sensitive instruments and the pricing of them is likely to be more delicate than the assets selected for the simpler model of Chapter 2. The same is true for the option $C_t$ . The option is written on interest-sensitive securities. 

Consider now how this setup differs from that of Chapter 2. First, in this matrix equation, the risks of investing in a “risk-free” savings account can be seen explicitly. The investment is risk-free only for one period. An investor may be certain about the payoff at time $t_{2}=t+\Delta$ , the immediate future. But, one period down the line, spot rates may yield a higher or lower return depending on the state of the world $\omega_{i,j}$ . Hence, in general terms, the current spot rate $r_{i}$ is known, but $r_{i+\Delta}$ is still random. It may be “low” (the up state), or “high” (the down state). Consequently, $R_{i_{2}}^{j}, j=u, d$ carries a superscript indicating this dependence on the realized state at time $t_{2}$ .
Second, note that the securities included in this model are quite different 

(20) 

$$
B _ {t _ {1}} = \frac {B _ {t _ {3}} ^ {u u}}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \frac {\tilde {p} ^ {u u}}{\tilde {P} ^ {u u}} + \frac {B _ {t _ {3}} ^ {u d}}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \frac {\tilde {p} ^ {u d}}{\tilde {P} ^ {u d}} + \frac {B _ {t _ {3}} ^ {d u}}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {d})} \frac {\tilde {p} ^ {d u}}{\tilde {P} ^ {d u}}
$$

$$
+ \frac {B _ {t _ {3}} ^ {d d}}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {d})} \tilde {p} ^ {d d}
$$

391 

$$
B (t, T) = E _ {t} ^ {\bar {P}} \left[ e ^ {- \int_ {t} ^ {T} r _ {u} d u} \right].
$$

This equation will be used extensively in later chapters. We now get similar pricing formulas for the long bond in system (6) by going over the same steps. The fourth row of (6) gives: 

(17) 

$$
B _ {t _ {1}} ^ {s} = E ^ {\tilde {p}} \left[ \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}})} \right],
$$

$$
B _ {t _ {1}} ^ {s} = \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \frac {\bar {p} u u}{+} + \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \frac {\bar {p} u d}{+} + \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {d})} \frac {\tilde {p} u d u}{+}
$$

$$
+ \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {d})} \tilde {P} ^ {d d},
$$

For example, the third row of the system gives the short bond's arbitrage-free price under the measure $\bar{P}$ : 

four states. Thus, proceeding in a way similar to Chapter 2, we can exploit the remaining equations of system (6) in order to obtain the corresponding martingale equalities. 

Clearly, as in Chapter 2, we can use the $\tilde{P}ii$ as if they are probabilities associated with the states-of-the-world, even though they do not have any probabilistic implications concerning the actual realization of any of the 

If there are no arbitrage opportunities, the state prices $\{\psi^i\}$ will be positive and we will have 

$$
1 = R _ {t _ {1}} R _ {t _ {2}} ^ {u} \psi^ {u u} + R _ {t _ {1}} R _ {t _ {2}} ^ {u} \psi^ {u d} + R _ {t _ {1}} R _ {t _ {2}} ^ {d} \psi^ {o u} + R _ {t _ {1}} R _ {t _ {2}} ^ {d} \psi^ {d d}, \tag {13}
$$

interest rate derivatives? The answer is no. Consider trying the same strategy in the new model shown in (6). Suppose we decide to determine the risk-neutral probabilities $\tilde{P}^{ij}$ by starting again with the first row of the system which corresponds to the savings account: 

the expected return (i.e., the trend) of the ratio becomes zero. In other words, the numerator and the denominator will “trend” upwards by the same expected drift r and the normalized variable becomes a martingale. It will have no discernible trend. 

$$
S _ {i} = \frac {1}{(1 + r \Delta)} E ^ {\vec {p}} [ S _ {t + \Delta} ].
$$

Note one additional characteristic of this normalization. The division by $(1 + r\Delta)$ amounts to discounting a future cash flow to present. But, in normalizing by risk-free lending, one first discounts, and then averages using the probability $\tilde{P}$ to get: 

$$
S _ {t} = E ^ {\bar {P}} \left[ \frac {S _ {t + \Delta}}{(1 + r \Delta)} \right].
$$

This expression yields a formula to determine the contractual rate $F_{t}$ using the risk-free probability P. But, unlike the case of option valuation with constant interest rates, we immediately see some undesirable properties of the representation. 

(31) 

$$
F _ {t _ {1}} E ^ {\tilde {P}} \left[ \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}})} \right] = E ^ {\tilde {P}} \left[ \frac {1}{(1 + r _ {t}) (1 + r _ {t _ {2}})} L _ {t _ {2}} \right].
$$

$$
F _ {t _ {1}} \left[ \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \frac {\tilde {p} ^ {u u}}{+} + \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \frac {\tilde {p} ^ {u d}}{+} + \frac {1}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {d})} \frac {\tilde {p} ^ {d u}}{+} \right]
$$

(28) 

(27) 

$$
0 = \frac {(F _ {t _ {1}} - L _ {t _ {2}} ^ {u})}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \tilde {\rho} ^ {u u} + \frac {(F _ {t _ {1}} - L _ {t _ {2}} ^ {u})}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {u})} \tilde {\rho} ^ {u d} + \frac {(F _ {t _ {1}} - L _ {t _ {2}} ^ {d})}{(1 + r _ {t _ {1}}) (1 + r _ {t _ {2}} ^ {d})} \tilde {\rho} ^ {d u}
$$

Now consider the details of how these probabilities were used in pricing the FRA contract. First, note that pricing the FRA means determining an $F_{t_{1}}$ such that the time $t_{1}$ value of the contract is zero. This is the case because all FRAs are traded at a price of zero and this we consider as the arbitrage-free price. The task is to determine the arbitrage-free $F_{t_{1}}$ implied by this price. From the second row of the system in (6) we have 

Thus, proceeding in a way similar to that in Chapter 2, and using the savings account to determine the $\tilde{P}$ , does lead to pricing formulas similar to the ones in (18) or (19). Yet, within the context of the instruments considered here, and with stochastic spot rates, the use of risk-neutral probabilities $\tilde{P}$ turns out to be less convenient and, at times, even inappropriate. It forces a market practitioner into handling unnecessary difficulties. The next section illustrates some of these. 

Here, $r_{t_{2}}$ is again a random variable. But so is $B_{t_{3}}$ , because the time $t_{3}$ is not a maturity date for this bond. For this reason, the equation in this form will not be very useful in practical pricing situations.

Finally, using the second and the fifth rows of (6) yields the pricing equations for the two Libor instruments, the FRA and the caplet derivative $C_{t}$ , respectively: 

This means that the $\pi^{ij}$ could be used as a new set of synthetic martingale probabilities. They yield a new set of martingale relationships. We call the $\pi^{ij}$ the forward measure. Before we consider the advantages of the forward measure, $\pi^{ij}$ , over the risk-neutral measure, $\tilde{P}$ , we make a few comments on the new normalization. 

$$
1 = \pi^ {u u} + \pi^ {u d} + \pi^ {d u} + \pi^ {d d},
$$

$$
1 = \frac {1}{B _ {t _ {1}} ^ {s}} \psi^ {u u} + \frac {1}{B _ {t _ {1}} ^ {s}} \psi^ {u d} + \frac {1}{B _ {t _ {1}} ^ {s}} \psi^ {d u} + \frac {1}{B _ {t _ {1}} ^ {s}} \psi^ {d d},
$$

$$
B _ {i _ {1}} ^ {s} = \psi^ {u u} + \psi^ {u d} + \psi^ {d u} + \psi^ {d d}.
$$

We now consider an alternative way of obtaining martingale probabilities. Within the same setup as in (6) and with the same $\psi^{\beta}$ , we can utilize the third equation to write: 

Clearly, using the money market account to define the probabilities $\tilde{P}_{i}$ as done in Eq. (24), creates complications which were not present in Chapter 2. Below we will see that a judicious choice of synthetic probabilities can get around these problems in a very convenient and elegant way. 

Again, if the $C_{t}$ is an interest-sensitive derivative, the same problems with $\vec{P}$ will be present. The random discount factor cannot be factored out of the expectation and the spot rate will in all likelihood be correlated with the option payoff $C_{t_{2}}$ if the latter is written on interest-sensitive securities. 

Proceeding in a similar fashion for the Libor derivative $C_t$ , we make the same argument. The pricing equation will be given by: 

eventually how the contract is settled. Clearly, this is not a very efficient way of calculating the arbitrage-free forward rate. In fact, one can dispense with the discounting altogether because both the $F_{t_1}$ and $L_{t_2}$ are measured in time $t_3$ dollars! 

corresponding expectations can be arduous with nonlinear expressions. A final comment. Note that, by definition, the $F_{t_1}$ is denominated in a currency value that will be settled in period $t_3$ . Now consider how the risk-neutral measure $\bar{P}$ operates in pricing Eq. (31). The pricing formula with $\bar{P}$ works by first discounting to present a value that belongs to time $t_3$ . Then, after taking the average via the expectation operator, the formula tries to reexpress this discounted term in time $t_3$ dollars, simply because that is eventually how the contract is settled. 

and stay inside the expectation.
Third, the pricing formula for the FRA in (31) is not linear. This property, although harmless at first sight, can be quite a damaging aspect of the use of risk-neutral measure. It creates major inconveniences for the market practitioner. In fact, when we try to determine the FRA rate $F_{t_{1}}$ or the price of the derivative $C_{t}$ , we now need to model two processes, namely the $r_{t}$ and $L_{t}$ , instead of one, the $L_{t}$ . Worse, these two processes are correlated with each other in some complicated way. The task of evaluating the corresponding expectations can be arduous with nonlinear expressions. A final comment Note that by definition, the $F_{t}$ is denominated in a independent? This will be a difficult assumption to maintain. Consider the second drawback of using the risk-neutral measure $\tilde{P}$ . As we noticed earlier, the spot-rate terms inside the expectations taken with respect to $\tilde{P}$ do not factor out. In contrast to the simple model of Chapter 2, where $r$ was constant across states, we now have an $r_2$ that depends on the state $u, d$ . Hence, the denominator terms in Eq. (31) are stochastic, and stay inside the expectation. 

Under this extreme assumption the forward rate becomes an unbiased estimator of the corresponding Libor process. But, in practice, can we really say that the short rates and the longer maturity Libor rates are statistically independent? This will be a difficult assumption to maintain. 

The only time this will be the case is when the $r_{i}$ and the $L_{i}$ are statistically independent. Then, the expectations can be taken separately: 

$E_{t}^{\pi}\left[E_{t+\Delta}^{\pi}[\cdot]\right]=E_{t}^{\pi}[\cdot],$ (48)

which says that the “best” forecasts of future forecasts, are simply the forecasts now. $^{10}$ $^{9}$ Thus $F_{t}$ is the FRA rate observed “now,” whereas the $F_{t+\Delta}$ is the FRA rate that will be observed within a short interval of time $\Delta$ . $^{10}$ Again, the “best” is used here in the sense of mean square error. 

with the $I_{t}$ being the information set available at time t. In this particular case, it consists of the current and past prices of all assets under consideration. 

Next, we recall the recursive property of conditional expectation operators that was used earlier: 

where the subscript of the $E_{t}^{\pi}[.]$ operator indicates that the expectation is now taken with respect to information available at time $t + \Delta$ . That is, 

Consider the following general case and revert back to using the $\Delta$ instead of the $t_i$ notation. Let the Libor rate for time $t + 2\Delta$ be given by $L_{t + 2\Delta}$ , the current forward rate be $F_{t}$ , and consider its future value $F_{t + \Delta}$ with $\Delta >0$ . We can utilize the measure $\pi$ and write: 

(45) 

Thus we obtained an important result. Although the $F_{t_1}$ is, in general, a biased estimator of $L_{t_2}$ , under the classical risk-neutral measure it becomes an unbiased estimator of $L_{t_2}$ under the new forward measure $\pi$ . Why is this relevant? How can it be used in practice? 

where the right-hand side is clearly the expectation of the Libor process $L_{2}$ evaluated using the new martingale probabilities $\pi^{ij}$ . This means that we now have: 

$0 = B_{t_1}^s\left[F_{t_1} - \left[L_{t_2}^u\pi^{uu} + L_{t_2}^u\pi^{ud} + L_{t_2}^d\pi^{du} + L_{t_2}^d\pi^{dd}\right]\right].$ (44) Note that here the $B_{t_1}^s$ has conveniently factored out because it is constant given the observed, arbitrage-free price $B_{t_1}^s$ . Canceling and rearranging: 

are in fact the corresponding elements of $\pi^{ij}$ , and that they sum to one, we obtain after factoring out the $F_{i_j}$ : 

Now consider evaluating the similar expectation under the measure $\pi$ . To do this, we take the second row in system (6) and multiply every element by the ratio $B_{t_1}^s / B_{t_1}^s$ , which obviously equals one: 

only measure $\pi$ instead of $F$ . We proceed in steps. First, recall that within the setup in this chapter, the use of the risk-neutral measure, $\bar{P}$ , leads to an equation where the $F_{t}$ is a biased estimator of the Libor process $L_{t}$ . In fact, we had 

Finally, note how normalization is done here. To introduce the probabilities in pricing equations, we multiply and divide each $\psi^{ij}$ by the $B_{i}^{s}$ . After relabeling the $\psi^{ij}/B_{i}^{s}$ as $\pi^{ij}$ , this amounts to multiplying, in the matrix Eq. (6), each asset price by the corresponding entry of the short bond $B_{i}^{s}$ . Hence, we say that we are “normalizing” by the $B_{i}^{s}$ . These and related issues will be discussed in more detail below. 

Second, note that we can define a new forward measure for every default-free zero-coupon bond with different maturity. Thus, it may be more appropriate to put a time subscript on the measure, say, $\pi_{T}$ , indicating the maturity, T, associated with that particular bond. Given a derivative written on interest-sensitive securities, it is clearly more appropriate to work with a forward measure that is obtained from a bond that matures at the same time that the derivative expires. 

First, to move from equations written in terms of state prices $\psi^{ij}$ , to those expressed in terms of $\pi$ , we need to multiply all state-dependent values by $B_{i_1}^s$ , which is a value determined at time $t_1$ . Hence, this term is independent of the states at future dates, and will not carry a state superscript. This means that it will factor out of expectations evaluated under $\pi$ . 

399 

In fact, any other asset can be chosen as the normalizing variable. Yet, the fact that $B_{t_1}^s$ matured at time $t_3$ made the time $t_3$ value of this bond constant. The convenience of the conditional expectations obtained under $\pi$ is the result of this very simple fact. It is this last property that makes the coefficients of the $u, d$ -dependent terms $L_{t_2}^{ij}$ or $C_{t_3}^{ij}$ constant relative to the information set available at time $t_1$ in equations such as (28). Because they were constants, these coefficients could be factored out of the expectation operators. This is an important result because it eliminated the need to calculate complex correlations between spot rates and future values of interest rate dependent prices. Also, due to this we avoided working with random discount factors. 

But the choice of normalization was important for another reason as well. Under carefully chosen normalization, forward rates such as $F_{t_1}$ become martingales, and were unbiased estimators for future values of spot rates such as $L_{t_2}$ . This implies that one can, heuristically speaking, replace the future value of a spot rate by the corresponding forward rates to find the current arbitrage-free price of various interest rate dependent securities. 

The procedure followed in the previous section chose a bond which matured at time $t = t_{3}$ in order to obtain a synthetic probability (measure) under which the martingale equalities turned out to be more convenient for pricing purposes. The choice of $B_{t_{1}}^{s}$ as the normalizing factor was dictated partly by this desire for convenience. 

According to this last equality, the conditional expectation of a function of $L_{t_{2}}$ is multiplied by the arbitrage-free price of the short bond. That is, the problem of modeling and calibrating a bivariate process has completely disappeared. Inside the expectation sign there is a single random variable $L_{t_{2}}$ . Here, we see the following convenient property of the new measure. The forward measure, $\pi$ , first calculates the expectation in time $t_{2}$ (i.e., forward) dollars and then does the discounting using an observed arbitrage-free price $B_{t_{1}}^{s}$ . In contrast, the risk-neutral measure first applies a random discount factor to a random payoff, and then does the averaging. Note that in proceeding this way, the risk-neutral measure misses the opportunity of using the discount factor implied by the markets, i.e., the $B_{t_{1}}^{s}$ , during the pricing process. Instead, the risk-neutral measure is trying to recalculate the discount factor from scratch, as if it is part of the pricing problem, leading to the complicated bivariate dynamics. We will see another example of this in the next section. 

As discussed earlier, in this pricing equation, the (random) spot rate $r_{t_2}$ is likely to be correlated with the (random) Libor rate $L_{t_1}$ , and hence the market practitioner will be forced to model and calibrate a bivariate process $r_t, L_t$ in order to price the caplet. Yet, using the forward measure in the last equation of system (6) gives 

beyond the lever X.
How should one price such an instrument? Consider the use of the classical risk-neutral measure $\tilde{P}$ . Using standard arguments and the risk-neutral probability $\tilde{P}$ , we have 

where $N$ is a notional amount that we set equal to one, the $K$ is the cap-rate selected at time $t_1$ , and the $L_{t_2}$ is the Libor rate realized at time $t_2$ . The payment is made in-arrears at time $t_3$ , and hence, provides the purchaser of the caplet some sort of insurance against increases in borrowing costs beyond the level $K$ . 

which says that the process $\{F_i\}$ is a martingale under the forward measure $\pi$ . As we will see later, this property of forward prices will be very convenient when pricing some interest rate sensitive instruments. A preliminary example of this can already be seen by looking at the similar conditional expectation for the derivative $C_i$ . 

and use the recursive property of conditional expectations to introduce an $E_{t+\Delta}^{\pi}$ operator at the “right place”: 

<!-- === Source: MinerU_markdown_An_Introduction_to_the_Financial_Derivatives_201_2122707919320489997.md (Page 201) === -->

401 

$C_{t} = E_{t}^{p}[e^{-f_{t}^{T}r_{t}d_{s}}\max [L_{T - \delta} - K,0]]$ (64) We also know that at time $T - \delta$ the $F_{T - \delta}$ will coincide with $L_{T - \delta}$ . So we may decide to use $F_{t}$ as the "underlying." After all, as time passes, 

$^{12}$ At any time, the forward rate for an immediate loan of tenor $\delta$ will be the same as the spot rate for that period. 

at time T. As mentioned earlier, this instrument will protect the buyer against increases in $L_{T-\delta}$ beyond the level K. Normally $0 < \delta < 1$ and in the above the right-hand side will be proportional to $\delta$ .
How does one price this caplet? Suppose we decide to use the risk-neutral probability $\tilde{P}$ . We know that the arbitrage-free price will be given by: 

2.5.2 A Caplet
As a second example to the power of the forward measure discussed above we consider pricing issues involving a caplet. Let $C_{t}$ be the current price of a caplet written on some Libor rate $L_{t}$ , with tenor $\delta$ and with cap rate K. Suppose the notional amount is N = 1 and that the caplet expires at time T. We let $\delta = 1$ , except for the notation on $L_{t}$ .
According to this, the buyer of the caplet will receive the payoff 

This is an equation that one can exploit conveniently to find the arbitrage-free value of $F_t$ . The critical point is to make sure that in calculating this average one uses the forward measure $\pi$ and not the risk-neutral probability $P$ . 

risk. Obviously, assuming deterministic spot rates would not be very appropriate here. But, if the assumption of deterministic $r_{t}$ is dropped, then the discount factor does not factor out and we cannot use Eq. (59) under $\tilde{P}$ . The forward measure can provide a convenient solution. Using the arbitrage-free price of the discount bond $B(t, T + \delta)$ , we can instead write the pricing equation under the forward measure: 

$^{11}$ Any margins that may be required are not cash exchanges, but are provided as a guarantee toward settlements in the future. 

That is, when spot rates are deterministic, the forward price is equal to the "best" forecast of the future $L_T$ under the risk-neutral measure $\bar{P}$ . Black-Scholes framework exploits the assumption of constant interest rates at various points in pricing stock options. But, the same assumption is not usable when one is dealing with interest-sensitive securities. The most important reason that such securities are traded is the need to hedge interest rate 

How can this price be zero given the formula in (56)? Because $F_{t}$ is chosen so that the right-hand side expectation vanishes. If the spot rates are assumed to be deterministic, this will be very easy to do. A value for $F_{t}$ can be easily obtained by factoring out the discount factor, 

$$
V _ {t} = E _ {t} ^ {\vec {p}} \left[ e ^ {- f _ {t} ^ {T + \delta} \tau_ {u} d u} (F _ {t} - L _ {T}) N \delta \right].
$$

2.5.1 The FRA Contract
Suppose we have a FRA contract that pays the sum $(F_{t}-L_{T})N$ , at some future date $T+\delta, t<T$ , where N is a notional amount and $F_{t}$ is the forward price of the random variable, $L_{T}$ . The $F_{t}$ is observed at contract-time t.
Because this is a cash flow that belongs to a future date, $T+\delta$ , the current value denoted by $V_{t}$ of the cash flow will be given by the “usual” martingale equality, where the future cash flow is discounted by using the risk-free rate $r_{s}, t \leq s \leq T + \delta$ . Under the risk-neutral measure we can 

We close this section by applying what was said in this chapter to two pricing examples in a continuous time setting. 

$$
\pi^ {i j} = \tilde {\pi} ^ {i j} \left[ \frac {B _ {t} ^ {i}}{B _ {t} ^ {s}} \right].
$$

This way one can go from one measure to another. Would such adjustments be any use to us in pricing interest rate sensitive securities? The answer is again yes. When we deal with an instrument that depends on more than one $L_{T}$ with different tenors T, we can first start with one forward measure, but then by taking the derivative with respect to the other, we can obtain the proper “correction terms” that need to be introduced. 

$$
\frac {\pi^ {i j}}{\tilde {\pi} ^ {i j}} = \left[ \frac {\frac {1}{B _ {t} ^ {s}}}{\frac {1}{B _ {t} ^ {i}}} \right],
$$

(67) 

$$
\tilde {\pi} ^ {i j} = \frac {1}{B _ {t}} \psi^ {i j}.
$$

We see from the above discussion that the fundamental variables are in fact the state prices $\{\psi^{ij}\}$ . When there are no arbitrage opportunities, these prices will exist, they will be positive and will be unique. Once this is determined, the financial analyst has a great deal of flexibility concerning the martingale measure that he or she can choose. The synthetic probability can be selected as the classical risk-neutral measure $\tilde{P}$ or the forward measure $\pi$ , depending on the instruments one is working with. Hence, the issue of which measure to work with becomes another tool for the analyst. In fact, as suggested by Girsanov theorem, one can go back and forth between various probabilities depending on the requirements of the pricing problem. In fact, consider a normalization with respect to $B_{t}^{s}$ and the corresponding measure $\pi$ that we just used. Clearly we could also have normalized with the longer maturity bond $B_{t}$ and obtained a new probability, say $\tilde{\pi}$ given by: 

2.5.3 Normalization as a Tool
Above we discussed the important implications of normalization and measure choice from the point of view of asset pricing, with particular emphasis on interest rate sensitive securities. Are there any implications for the mathematics of financial derivatives? 

will not be a matrigate. $^{14}$ A remaining difference is in the units used here. There is no need to discount the caplet payoff to the present if we use the forward rate dynamics. This is unlike the Black-Scholes environment where the stock price dynamics $dS_{t}$ are expressed in time t dollars. 

$^{15}$ It is important to realize that under a different normalization this particular forward rate will not be a martingale. 

There is no additional difficulty of determining an unknown drift. We can go ahead with a Black-Scholes type argument and price this caplet in a straightforward fashion. $^{14}$ where the $W_{t}^{\pi}$ is a Wiener process under $\pi$ . A very convenient property of this SDE is that the drift is equal to zero and the $F_{t}$ is an unbiased estimator of $L_{T - \delta}$ : 

determine.
Consider what happens to the forward rate dynamics if we use the forward measure $\pi$ instead. Under the forward measure obtained with $B(t, T)$ -normalization, the forward rate $F_{t}$ defined for time $T - \delta$ will be a martingale. $^{13}$ Hence we can write: 

this variable will eventually coincide with the future spot rate $L_{T-\delta}$ . This process is called the forward Libor process.
This suggests that we model log-normal forward rate dynamics with a Wiener process $W_{t}$ defined under the original probability P, where the $\mu^{*}$ is the new risk-adjusted drift implied by the Girsanov theorem. Under $\tilde{P}$ this drift is not known at the outset. So, unlike the Black-Scholes case where the drift of the underlying stock price is replaced by the known (and constant) spot rate $r$ , we now end up with a difficult unknown to determine. 

to determine the $C_{t}$ . If we proceed this way, the first step will be to switch to $\bar{P}$ , the risk-neutral probability. But this creates a problem. The $F_{t}$ is not a martingale under $\bar{P}$ . So, as we switch probabilities and use the Wiener process, $\bar{W}_{t}$ , defined under $\bar{P}$ , the forward rate dynamics will become 

3. Select ten standard, normal random numbers using Mathematica, Maple, or Matlab. Suppose interest rates follow the SDE: 

2. Suppose at time t = 0, you are given four default-free zero-coupon bond prices $P(t, T)$ with maturities from 1 to 4 years: 

The current spot rate is assumed to be 6%. 

$\mu = .01.$ 

15This is the case because the forward price, $F_{n}$ , itself belongs to the same forward date unlike, say, the $C_n$ , which is a value expressed in time $t$ dollars. 

• The annual drift is 

$d r_{i} = \mu r_{i} + \sigma r_{i} d W_{i}$ . 

5 Exercises 

The book by Musiela and Rutkowski (1997) is an excellent source for a reader with a strong quantitative background. Although it is much more demanding mathematically than the present text, the results are well worth the efforts. Another possible source is the last chapter in Pliska (1997). Pliska treats these notions in discrete time, but our treatment was also in discrete time. 

4 References 

martingale under $\pi_{T}$ .
• The forward prices that correspond to the same maturity become mar-
tingales themselves, without any need for normalization. $^{15}$ • The discount factors become deterministic and factor out of pricing
equations for derivatives with expiration date T. 

• The price of all assets considered here, once normalized by the arbitrage-free price of a zero-coupon bond of $B(t,T)$ , becomes a 

Some of the main results were the following. When we use the forward measure $\pi_T$ obtained from a default-free discount bond $B(t,T)$ , three things happen: 

In this chapter we introduced the notions of normalization and forward measure. These tools play an important role in pricing derivative securities in a convenient fashion. More than just theoretical concepts, they should be regarded as important tools in pricing assets in real world markets. They are especially useful for any derivative whose settlement is done at a future date, in future dollars. 

3 Conclusions 

# Modeling Term Structure and Related Concepts

## CHAPTER 19

CHAPTER $\cdot$ 17 Arbitrage Theorem 

(e) Can you use this result in calculating bond prices?
(f) In particular, how do we know that the interest rate dynamics displayed in the above SDE are arbitrage-free?
(g) What would happen to the above interest rate dynamics if we switched to risk-neutral measure $\hat{P}$ ?
(h) Suppose you are given a series of arbitrage-free bond prices. How can you exploit this within the above framework in obtaining the arbitrage-free dynamics for $r_{t}$ ? 

## 1 Introduction

The previous chapter was important because it discussed the Fundamental Theorem of Finance when interest-sensitive securities are included in the picture. We obtained new results. The issue of normalization, the use of forward measures within Libor instruments, and ways of handling the simultaneous existence of bonds with differing maturities was introduced using a simple model. Now it is time to take some steps backward and discuss the basic concepts in more detail before we utilize the results obtained in Chapter 17. 

In particular, we need to do two things. The new concepts from fixed income are much more fragile and somehow less intuitive than the straightforward notions used in the standard Black-Scholes world. These fixed income concepts need to be defined first, and carefully motivated second. Otherwise, some of the reasoning behind the well-known bond pricing formulas may be difficult to grasp. 

Next, at this point we need to introduce some important arbitrage relationships that are used repeatedly in pricing interest-sensitive securities. The next chapter will consider two fundamentally different methodologies used in pricing interest-sensitive securities. These are the so-called classical approach and the Heath-Jarrow-Morton approach, respectively. Our main purpose will be to show the basic reasoning behind these fundamentally different methodologies and highlight their similarities and differences. But 

$^{2}$ But, as we saw earlier, the spot rate itself can be a random variable and the investment may well have a market risk it rolled-over. 

The basic concepts defined in the previous section can be used to define three “curves” used routinely by market professionals. These are the yield curve, the discount curve, and the credit-spread curve. The so-called swap 

Note that the $F(t,T,U)$ has three time indices whereas discount bond prices each came with two indices. This suggests that to obtain a relation between forward rates and bond prices, we may have to use two different bonds, $B(t,T)$ and $B(t,U)$ , with maturities T and U, respectively. Between them, these two bond prices will have the same time indices $(t,T,U)$ . 

$_{e}^{F(t,TU)(U-T)}$ 

Next, we need to define a continuously compounded forward rate $F(t, T, U)$ . This concept represents the interest rate on a loan that begins at time T and matures at time U > T. The rate is contracted at time t, although cash transactions will take place at future dates T and U. The fact that the rate is continuously compounded implies that the actual interest calculation will be made using the exponential function. In fact, if one dollar is loaned at time T, the money returned at time U will be given by: 

It is the rate of return that corresponds to an investment of $B(t,T)$ dollars which returns one dollar after a period of length $[T-t]$ . Here, the use of an exponential function justifies the term continuously compounded. Note that there is a one-to-onc relationship between the bond price and the yield. Given one we know the other. They are also indexed by the same indices T and t. 

$B(t,T) = e^{...R(t,T)(T - t)}.$ 

The first new concept that we now define is the continuously compounded yield, $R(t,T)$ , of the discount bond, $B(t,T)$ . Given the current price of the bond $B(t,T)$ and with par value $1, the $R(t,T)$ is defined by the equation: 

will be represented by the symbol $B(t, T)$ . The $r_t$ will again denote the instantaneous spot rate on riskless borrowing. The spot rate is instantaneous in the sense that the loan is made at time $t$ and is repaid after an infinitesimal period $dt$ . The spot rate is also riskless in the sense that there is no default risk, and the return to this instantaneous investment is known with certainty. These two definitions were seen earlier. 

409 

$^{1}$ In practice, the shortest-term investment will earn an overnight interest rate. 

We begin with some definitions, some of which were introduced earlier. The price of a discount bond maturing at time $T$ observed at time $t < T$ . 

2 Main Concepts 

Thus, one way or another, the material in the present chapter should be regarded as a necessary background to discussing pricing of interest-sensitive securities. 

The second arbitrage relation is specific to fixed income. Fixed income markets provide many liquid instruments that are almost identical except for their maturity. For example, we have a spectrum of discount bonds that are differentiated only by their maturity. Similarly, we have forward rates of different maturities. It turns out that this multidimensional aspect of interest-sensitive instruments permits writing down complex arbitrage relations between a set of zero-coupon bonds and a set of forward rates. In fact, if we have a $k$ -dimensional vector of bond prices, we can relate this to a vector of forward rates using arbitrage arguments. These arbitrage relations form the basis of the Heath-Jarrow-Morton approach to pricing interest-sensitive securities. 

to do this we must first introduce a number of new arbitrage relations that exist between the spot rates, bond prices, and forward rates.
The first arbitrage relation that we need to study is the one between investment in very short-term savings accounts and bonds. Suppose both of these are default-free. How would the long-term bond prices relate to depositing money in a short-term savings account and then rolling this over continuously?¹ It is clear that when one buys a longer term bond, the commitment is for more than one night, or one month. During this “long” period, several risky events may occur, and these may affect the price of the bond adversely. Yet, the overnight investment will be mostly immune to the risky events because the investor’s money is returned the next “day,” and hence can be reinvested at a higher overnight rate. Thus, it appears that long-term bonds should pay a premium relative to overnight money, in order to be held by risk-averse investors. In the Black–Scholes world the switch to the risk-neutral measure eliminated these risk premia and gave us a pricing equation. Can the same be done with interest-sensitive securities and random spot rates? We will see that the answer is yes. In fact, the classical approach to pricing interest-sensitive securities exploits this particular arbitrage relation extensively. 

408 CHAPTER·18 Modeling Term Structure and Related Concepts 

Hence, for each risk class we obtain a different yield (discount) curve. The difference between these yield (discount) curves will indicate the credit spreads, the supplemental amount riskier credits have to pay to borrow money at the same maturity. The coexistence of different yield curves that represent different risk classes leads to the so-called credit-spread curve. 

DEFINITION: Given two yield curves $\{R(t,T),T\in [t,T^{max}]\}$ that correspond to default-free bonds and the $\{\tilde{R}_t^I,T\in [t,T^{max}]\}$ that 

2.1.3 The Credit Spread Curve Yield curves and the discount curves are obviously valid for bonds of a given risk class. When we look at the spectrum of bonds $\{B(t,T),T\in[t,T^{max}]\}$ , we implicitly assume that the default risk on these bonds is the same. Otherwise, the difference between yields would not just be due to differences in the corresponding maturities. 

The reason why this works is simple. The price $B(t, T_i)$ is simply the current arbitrage-free value of $1 to be paid at time $T_j$ . The discount is directly quoted by the market. Hence, the discount curve will play an essential role in the daily work of a market practitioner. 

The discount curve is more convenient to use in valuing general cash flows. In fact, let the $\{cf_{i_1},\ldots ,cf_{T_n}\}$ represent a general cash flow to be received at arbitrary times $T_{1} < T_{2} < \dots < T_{n} = T$ . The present value $CF_{i}$ of this general cash flow can be obtained by simply multiplying the amount to be received at time $T_{i}$ by the corresponding $B(t,T_i)$ . In fact, the discounted value can easily be obtained by using arbitrage-free zero- coupon bond prices with maturities falling to the corresponding $T_{i}$ . This present value is 

DEFINITION: The spectrum of default-free zero-coupon bond prices $\{B(t,T), T \in [t,T]\}$ , with a continuum of maturities that belong to the same risk class, is called the discount curve. 

2.1.2 The Discount Curve
In spite of the popularity of the term “yield curve,” most market applications instead use the discount curve. 

to the longest possible maturity $T = T^{max}$ , providing a continuous yield curve. According to this assumption, given an arbitrary $T < T^{max}$ , there will be no need to “interpolate” the corresponding yield because it will be directly observed in the markets. 

The yield curve is a correspondence between the yields of the bonds belonging to a certain risk class and their respective maturities. The definition of the yield curve given above is an extension of the yield curve notion used by practitioners. Observed yield curves provide the spec-trum of yields on, say, Treasuries, at a finite number of maturities. Here, we assume not only that time is continuous, but that at any time t, there is a continuum of pure discount bonds. An investor can always buy and sell a liquid T-maturity bond, for any value of $T < T^{max}$ . These maturities extend from the immediate tenor, 

DEFINITION: The spectrum of yields $\{R(t,T),T\in[t,T^{max}]\}$ is called the yield curve. 

Here, we have $0 < B(t,T) < 1$ as long as $t < T$ . Thus $\log [B(t,T)]$ will be a negative number, and hence the $R(t,T)$ will be positive. Now, assume that at time $t$ there exist zero-coupon bonds with a full spectrum of maturities $T \in [t,T^{\max}]$ , where $T^{\max}$ is the longest maturity available in the market. Let the price of these bonds be given by the set $\{B(t,T),T \in [t,T^{\max}]\}$ . For each $B(t,T)$ in this set we can use Eq. (4) and obtain the corresponding yield $R(t,T)$ . Then we have the following definition. 

$R(t,T) = \frac{\log(1) - \log B(t,T)}{T - t}$ 

where $B(t,T)$ is the arbitrage-free price of the T-maturity discount bond. Thus, to obtain the yield $R(t,T)$ of a bond, we first need to obtain its price. Then, Eq. (3) is used to get the continuously compounded yield: 

2.1.1 The Yield Curve
The yield curve is obtained from the relationship between the yield $R(t, T)$ , and the discount bond price $B(t, T)$ . We have: 

curve, which is perhaps the most widely used curve in fixed income markets, is omitted. This is due to the limited scope of this book. We do not consider instruments. We only deal with mathematical tools to study them. The forward curve which consists of a spectrum of interest rates on forward loans contracted for various future dates will be discussed later in the chapter. 

410 CHAPTER·18 Modeling Term Structure and Related Concepts 

changes, time will pass, new Wiener increments are drawn, random shock(s) affect the spot rate and the yield curve shifts. It is important to realize that as t increases by dt, the entire spectrum of yields will, in general, change. Thus, the dynamics of fixed income instruments are essentially the dynamics of a curve rather than the dynamics of a single stochastic process. The implied arbitrage restrictions will be much more complicated than the case of the Black-Scholes environment. After all, we need to make sure that the movements of an entire curve occurs in a fashion that rules out arbitrage. 

A second type of incremental change that we can contemplate is a variation in the time parameter t. The incremental change in the spectrum of yields $R(t, T)$ due to a change in time t, will involve random shocks. As 

Yield curves are generally classified as negatively sloped, positively sloped, and flat. They can also exhibit "humps." As the shape of the curve changes, the slope changes as well. It is important to realize that an incremental change in $T$ would not involve any unknown random shocks. It is an experiment involving bonds with different maturities at the same instant $t$ and, at time $t$ , every $R(t,T)$ is known. Also, because there are no Wiener increments involved in these movements, the derivative can be taken in standard fashion without having recourse to Ito's Lemma. 

This is simply the slope of the yield curve $\{R(t,T),T\in[t,T^{max}]\}$ . These quantities are shown in Figure 1. The $g(T)$ is the slope of the tangent to the continuous yield curve at maturity T. Figure 2 displays the corresponding situation with the discount curve. 

Before we deal with more substantial issues we also would like to discuss the comparison between a shift in the yield curve and a movement along it. Given a yield curve, $\{R(t,T),T\in[t,T^{max}]\}$ continuous in T, note that at time t, we can consider two different incremental changes. First, at any instant t, we can ask what happens to a particular $R(t,T)$ as T changes by a small amount denoted by dT. Here, we are modifying the maturity of a particular bond under consideration, namely the one that has maturity T, by dT. In other words, we are moving along the same yield curve. According to this, if the yield curve is continuous and “smooth,” we can obtain the derivative: 

## 2.2 Movements on the Yield Curve

Indeed, some practitioners prefer to work with a correspondence between the credit spread and the maturity, instead of dealing with the yield curve itself. The use of the credit spread curve will be more practical if the traded instruments are written on the spreads rather than the underlying interest rates. In this book, we omit a discussion of credit instruments and assume throughout that there is no default risk. Hence, there is only one risk class and there the default risk is assumed to be zero. 

correspond to bonds with a given default probability, the spectrum of the spreads, $\{s(t,T) = (\tilde{R}_i^T -R(t,T)),T\in [t,T^{max}]\}$ , is called the credit spread curve. 

412 CHAPTER·18 Modeling Term Structure and Related Concepts 

We utilize the methodology introduced in Chapter 17. We take the current bond price $B(t, T)$ and normalize by the current value of the savings account, which is $1. Next, we take the maturity value of the bond, which is $1, and normalize it by the value of the savings account. This value is equal 

When the instantaneous spot rate $r_{t}$ becomes stochastic, the pricing formula in (9) will have to change. Suppose $r_{t}$ represents the risk-free rate earned during the infinitesimal interval $[t, t + dt]$ . Thus, $r_{t}$ is known at t, but its future values fluctuate randomly as time passes. The Fundamental Theorem of Finance can be applied to obtain an arbitrage relation between $B(t, T)$ and the stochastic spot rates, $r_{t}, t \in [t, T]$ . We utilize the methodology introduced in Chapter 17. We take the cur-

Hence, this relationship is not a definition, or an assumption. It is a restriction imposed on bond prices and savings accounts by the requirement that there are no arbitrage opportunities. Notice that in obtaining this equation we did not use the Fundamental Theorem of Finance, but doing this would have given exactly the same result. $^{3}$ 

## 3.2 Stochastic Spot Rates

The only condition that would eliminate such arbitrage opportunities is when the “bond pricing equation” holds: 

The other possibility is $B(t, T) < e^{-r(T-t)}$ . Then at time $t$ , one would borrow $e^{-r(T-t)}$ dollars, and buy a bond at a price of $B(t, T)$ . When the maturity date arrives the net cash flow will again be zero. The +$1 received from the bond can be used to pay the loan off. But at time $t$ , there will be a net gain: 

Otherwise, there will be arbitrage opportunities. It is instructive to review the underlying arbitrage argument within this setting.
First, suppose $B(t,T) > e^{-r(T-t)}$ . Then, one can short the bond during the period $[t,T]$ , and invest $e^{-r(T-t)}$ of the proceeds to risk-free lending. At time T, the short (bond) position is worth -1. But the risk-free lending will return +1. Hence, at time T the net cash flow will be zero. But, at t the investor is still left with some cash in the pocket because 

Now, an investor who faces these instruments has the following choices. He or she can invest $e^{-r(T-t)}$ dollars in a risk-free savings account now, and at time T this will be worth $1. Or, the investor can buy the T-maturity discount bond and pay $B(t,T)$ dollars now. This investment will also return $1 at time T. Clearly we have two instruments, with no default risk, and with the same payoff at time T. There are no interim payouts either. If interest rates are constant and if there is no default risk, any bond that promises to pay one dollar at time T will have to have the same price as the initial investment of $e_t^{-r(T-t)}$ to risk-free lending. That is, we must have: 

Consider the rationale behind this formula. The r is the continuously compounded instantaneous interest rate. The function $e^{-r(T-t)}$ plays the role of a discount factor at time t. At t = T the exponential function equals 1, which is the same as the maturity value of the bond. At all other times, t < T, the exponential factor is less than 1. Hence, the right-hand side of Eq. (9) represents the present value of one time-T dollar, discounted to t at a constant, continuously compounded rate r. 

$r_{t}=r.$ (8)
Then, the price of a default-free pure discount bond paying $1 at time T will be given by: 

In this section we start discussing the first substantial issue of this chapter. We derive an equation that gives the arbitrage-free price of a default-free zero-coupon bond $B(t, T)$ , maturing at time T. We go in steps. We first begin with a simplified case where the instantaneous spot rate is constant, and then move to a stochastic risk-free rate. This way of proceeding makes it easier to understand the underlying arbitrage arguments. 

3 A Bond Pricing Equation 

Also, note that for stochastic differentials such as $dR(t,T)$ , Ito's Lemma needs to be used due to involved Wiener components. We are now ready to introduce a fundamental pricing equation that will be used throughout the second part of this book, namely, the bond pricing equation. 

given that all technical conditions are satisfied. Thus, as $\Delta \rightarrow 0$ we move from discrete-time discounting, toward continuous-time discounting with variable spot rates. As a result, discrete-time discount factors get replaced by the exponential function. Because interest rates are continuously changing, an integral has to be used in the exponent. Thus we obtain the continuous time bond pricing formula: 

We now show the heuristics of moving to continuous time in the present setting. As we move from three periods to an n-period setting, the formula (13) becomes: 

According to Eq. (13), the bond's price is equal to the discounted value of the payoff at maturity. The discount factor is random and an (conditional) expectation operator needs to be used. The expectation is taken with respect to the risk-neutral probability $\tilde{P}$ . We normalize the value of the bond at times t and $t + 3\Delta$ using the "risk-free" saving and borrowing.

As mentioned earlier, for time t we divide the bond price by 1, the amount invested in risk-free lending and borrowing. For time $t + 3\Delta$ we divide the value of the bond at maturity, which is 1, by the value of rolling the investment over at future spot rates $r_{t+\Delta}, r_{t+2\Delta}$ . The expectation is conditional on the information set available at time t. This information set contains the current value of $r_{t}$ . 

$^{4}$ Remember that conditional expectations provide the optimal forecasts in the sense of minimum mean square error given an information set $I_{t}$ . 

where $r_{t}$ is the known current spot rate on loans that begin at time t and end at time $t+\Delta$ , and $r_{t+\Delta}, r_{t+2\Delta}$ are unknown spot rates for the two future time periods. Unlike the case of continuous time, these are simple interest rates, and by market convention, are multiplied by $\Delta$ . 

3.2.1 Discrete Time
Consider the special case of a three-period bond in discrete time. If $\Delta$ represents some time interval less than one year and if t is the “present,” then the price of a three-period discount bond will be given by: 

We now discuss this formula using discrete intervals of size $0 < \Delta$ . This will show the passage to continuous time, and explain the mechanics of the bond pricing formula better. 

Second, there is the issue of which probability measure is used to calculate these expectations. One may think that with the class of Treasury bonds being risk-free assets, there is no risk premium to eliminate, and hence, there is no need to use the equivalent martingale measure. This is, in general, incorrect. As interest rates become stochastic, prices of Treasury bonds will contain “market risk.” They depend on the future behavior of spot rates and this behavior is stochastic. To eliminate the risk-premium associated with such risks, we need to use equivalent martingale measures in evaluating expressions as in (12). 

Some further comments about this formula are in order. First, the bond price formula given in (12) has another important implication. Bond prices depend on the whole spectrum of future short rates $r_{s}, t < s < T$ . In other words, we can look at it this way: the yield curve at time t contains all the relevant information concerning future short rates. $^{4}$ 

According to Chapter 17, this normalized bond price must be a martingalc under the risk-neutral measure $\tilde{P}$ . Thus, we must have 

According to this if, at time t, we invest the amount $B_{t}^{*}$ at a rate $r_{t}$ , and then at $t+\Delta$ roll this investment at a predetermined rate $F(t,t+\Delta,t+2\Delta)$ , we get a payoff of 1 at time $t+2\Delta$ . But this is exactly the same payoff given by the strategy of buying the bond $B(t,t+2\Delta)$ . Thus, if the credit risk involved in the two strategies is the same, we must have 

(25) 

$B(t,t + 2\Delta) = B_{t}^{*}$ 

$^{5}$ In the following expressions the reader may notice that the forward rates, say, $F(t,T,T+\Delta)$ , are multiplied by $\Delta$ . This is needed because the $F(\cdot)$ are assumed to be annual rates, whereas the $\Delta$ is supposedly a small arbitrary interval. By market convention, the forward interest earned during $\Delta$ is not $F(t,T,T+\Delta)$ , but $F(t,T,T+\Delta)$ times $\Delta$ . For example, if the annual forward rate is 6%, and if once year is made of 360 days, then a three-month loan will earn 6 times 1/4 percent. 

Finally, after recognizing that for period $t$ , $r_t$ is also the trivially defined forward rate $F(t,t,t+\Delta)\Delta$ , the $B_t^*$ becomes: $^6$ (24) 

Now this is an amount that belongs to time $t + \Delta$ . We need to discount the $B_{t+\Delta}^{*}$ to time t using the current spot rate. This gives the time t value of the forward loan, which we call $B_{t}^{*}$ : 

Now suppose liquid markets are available in forward loans and consider the following alternative investment at time t. We make a forward loan that begins at time $t + \Delta$ which pays an interest of $F(t, t + \Delta, t + 2\Delta)\Delta$ at $t + 2\Delta$ . Let the total amount loaned be such that, at time $t + 2\Delta$ we receive 1. Thus, the amount of the loan contracted for time $t + \Delta$ and denoted by $B_{t+\Delta}^{*}$ is: 

To motivate the discussion, we begin with two periods. If $\Delta$ represents a small but noninfinitesimal time interval, and if t is the “present,” then the price of a two-period bond will be given by $B(t,t+2\Delta)$ . This bond will yield a cash flow of 1 at maturity date $t+2\Delta$ . Thus, one pays $B(t,t+2\Delta)$ , at time t, and the investment pays off 1 at time $t+2\Delta$ . 

loan that begins at time $t$ and matures at time $c > t$ . As mentioned earlier, to derive a relationship between the $B(t,T)$ and $F(t,T,U)$ we need a second bond, $B(t,U)$ , that matures at time $U$ . This is easy to see. The $F(t,T,U)$ is a market price that incorporates time $t$ information concerning the (future) period between the times $T$ and $U$ . We expect the bond $B(t,T)$ to incorporate all relevant information up to time $T$ . The longer maturity bond $B(t,U)$ , on the other hand, is a price that will incorporate all information up to time $U$ . Hence, we should in principle be able to extract from $B(t,T)$ and $B(t,U)$ all necessary information concerning the $F(t,T,U)$ . As before, we obtain this relationship first in discrete time, using intervals of length $\Delta$ , and then take the continuous-time limit. 

In this section we obtain another arbitrage relation that shows how forward rates relate to bond prices. It turns out that this relationship plays a crucial role in the modern theory of fixed income. 

$$
R (t, T) = - \frac {\log E _ {t} ^ {\tilde {P}} \left[ e ^ {- f _ {t} ^ {T} r , d s} \right]}{T - t} = - \frac {\log e ^ {- r (T - t)}}{T - t}
$$

We see that the yield of a bond can (roughly) be visualized as some sort of average spot rate that is expected to prevail during the life of the bond. In fact, in the special case of a constant spot rate, 

We can also derive a relation between the yields $R(t, T)$ and the short rate $r_{t}$ . We can relate future short rates to the yield curve of time t using the two equations in (12) and (3). Equating the right-hand sides: 

That is, the instantaneous forward rate $F(t,T)$ is closely related to the derivative of the logarithm of the discount curve. 

$$
B (t, T + \Delta) = e ^ {- \int_ {t} ^ {T + \Delta} F (t, s) d s}.
$$

We can also go in the opposite direction and write $F(t,T,U)$ as a function of bond prices. We prefer to do this for the maturities T and $U = T + \Delta^{7}$ . Thus, consider two bonds, $B(t,T)$ and $B(t,T+\Delta)$ , whose maturities differ only by a small time interval $\Delta > 0$ . Then writing the formula (32) twice: 

we move from discrete time toward continuous-time discounting. As a result, two things happen. First, the discrete-time discount factors need to be replaced by the exponential function. Second, instead of discrete forward rates we need to use instantaneous forward rates. Because instantaneous forward rates may be different, an integral has to be used in the exponent. Again, note that there is no expectation operator in this equation because all $F(t,s)$ are quantities known at time $t$ . The formula: 

given that the recurring technical conditions are all satisfied. The $F(t,s)$ is now the instantaneous forward rate contracted at time $t$ , for a loan that begins at $s$ and ends after an infinitesimal time interval $ds$ . Thus, as $\Delta \to 0$ , which means that we can let $\Delta \rightarrow 0$ and increase the number of intervals to obtain the continuous version of the relation between instantaneous forward rates and bond prices, 

$\overline{[1+F(t,t,t+\Delta)\Delta]\cdots[1+F(t,t+(n-1)\Delta,t+n\Delta)\Delta]}$ (28)
Now use the approximation that when the $F(t,T,U)$ and $\Delta$ are small, one has 

What happens when this arbitrage relation does not hold? One would simply short sell the expensive investment and buy the cheaper one. The payments and receipts of two positions will cancel each other at time $t + 2\Delta$ , while leaving some profit at time $t$ . Hence, there will be an arbitrage opportunity. 

$B(t,t+2\Delta)=\overline{[1+F(t,t,t+\Delta)\Delta][1+F(t,t+\Delta,t+2\Delta)\Delta]}$ . (27)
Note that since all the quantities on the right-hand side of this equation are known at time t, there is no need to use any expectation operators in this formula. The relationship between the bond prices and the current forward rates is exact. 

To sum up, the first relation is simply a definition. It cannot be used for pricing. But the other two arc based on arbitrage principles and would hold in liquid and well-functioning markets. They form the basis of the two broad approaches to pricing interest-sensitive instruments. The so-called classical approach uses the second relation, whereas the recent Heath-Jarrow-Morton, HIM approach, uses the third. We will study these in the next chapter. 

This can also be used as a pricing equation, except that if we are given a $F(t,T,U)$ we will have one equation and two unknowns to determine here, namely the $B(t,T),B(t,U)$ . Thus, before we can use this as a pricing equation we need to know at least one of the $B(t,T),B(t,U)$ . The addition of other forward rates would not help much because each forward rate equation would come with an additional unknown bond price. $^{9}$ 

Thus, this second relationship is based on the no-arbitrage condition and as such is a pricing equation. That is, given a proper model for $r_{t}$ , it can be used to obtain the “correct” market price for the bond $B(t, T)$ . The third relationship was derived in the previous section. Using again an arbitrage argument we saw that the (arbitrage-free) prices of the bonds $B(t, T), B(t, U)$ with U > T, and continuously compounded forward rate $F(t, T, U)$ were related according to: 

The spot rate $r_{t}$ being random, we apply the (conditional) expectation operator under the risk-neutral measure $\hat{P}$ , to obtain the relation: 

once discounted by the instantaneous interest rate $r_t$ . The bond $B(t, T)$ paid $1 at maturity, and the discounted value of this was 

$^{8}$ Earlier in this section when discussing the discrete time case, $F(t,T,U)$ was used as a symbol for simple forward rates. In moving to continuous time, and switching to the use of the exponential function, the same symbol now denotes continuously compounded rates. A more appropriate way of proceeding would perhaps be to use different symbols for the two concepts. But the notation of this chapter is already too complicated. 

The second relationship was the result of applying the same principle that was used in the first part of the book to bond prices; namely, that the expectation under the risk-neutral measure $\tilde{P}$ of payoffs of a financial derivative would equal the current arbitrage-free price of the instrument, 

It is time to review what we have obtained so far. We have basically derived three relationships between the bond prices $B(t, T)$ , the bond yields $R(t, T)$ , the forward rates $F(t, T, U)$ , and the spot rates $r_t$ . The first relation was simply definitional. Given the bond price, we defined the continuously compounded yield to maturity $R(t, T)$ as: 

It is obvious from these arguments that the existence of $F(t, T)$ assumes that the discount curve, that is, the continuum of bond prices, is differentiable with respect to $T$ , the maturity date. Using Eq. (39) and assuming that some technical conditions are satisfied, we see that 

By going through a similar argument, we can derive a similar expression for the noninstantaneous, but continuously compounded forward rate $F(t, T, U):^{8}$ 

(a) Set up a $2 \times 4$ system with state prices $\psi^{ij}, i, j = u, d$ that gives the arbitrage-free prices of a savings account and of the bond B.
(b) Show how one can get risk-neutral probabilities, $\bar{P}$ , in this setting.
(c) Show that if one adopts a savings account normalization, the arbitrage-free price of the bond will be given by 

2. Consider a world with two time periods and two possible states at each time t = 0, 1, 2. There are only two assets to invest. One is risk-free borrowing and lending at the risk-frec rate $r_{i}, i = 0, 1$ . The other is to buy a two period bond with current price $B_{0}$ . The bond pays 1 at time t = 2 when it matures. 

(d) What happens to bond price volatility as maturity approaches? Is this expected?
(e) What happens to the drift coefficient as maturity approaches? Is this expected?
(f) Finally, what is the drift and diffusion parameter for a bond with very long maturity, $s \rightarrow \infty$ ? 

variance of spot rate as $s \rightarrow \infty$ ?
(c) Suppose the market price of interest rate risk is constant at $\lambda$ (i.e., the Girsanov transformation adjusts the drift by $\sigma\lambda$ ). Using the bond price function given in the text, show that the drift and diffusion parameters for a bond that matures at time s are given by 

$$
V a r [ r _ {s} | r _ {t} ] = \frac {\sigma^ {2}}{2 \alpha} \left(1 - e ^ {- 2 \alpha (s - t)}\right),
$$

The reader can consult this excellent book for discrete-time fixed income models, Jarrow (1996). Rebonato (1998) is one source that contains a good and comprehensive review of interest rate models, the other good source is the publication by Risk (1996). For a survey of recent issues, see Jegadeesh and Tuckman (2000). 

Second, one may go the other way around. If there are no reliable data on the discount curve $B(t,T)$ , one may first posit an appropriate arbitrage-free model for the spot rate $r_{t}$ , estimate it using historical data on interest rates, and then use Equation (1) in getting “fair” market prices for illiquid bonds and other interest-sensitive derivatives. Both of these will be called the classical approach to pricing interest rate derivatives. We will see that, one way or another, the classical approach is based on modeling the instantaneous interest rate $r_{t}$ , in the first case, by starting from a “reliable” set of bond prices $\{B(t,T)\}$ , and in the second case, from data available on $r_{t}$ process itself. 

can be exploited in (at least) two different ways by market practitioners. First, if an accurate and arbitrage-free discount curve $\{B(t,T)\}$ exists, one can use these in Equation (1), go “backwards,” and try to obtain an arbitrage-free model for the spot rate $r_{r}$ . One can then exploit the arbitrage-free characteristic of this spot-rate model to price interest rate derivatives other than bonds. 

2 The Classical Approach 

In this chapter we provide a discussion of these methods used by practitioners in pricing interest-sensitive securities. Given our limited scope, numerical issues and details of the pricing computations will be omitted. Interested readers can consult several excellent texts on these. Our focus is on the understanding of these two fundamentally different approaches. 

The Heath-Jarrow-Morton (HJM) approach, on the other hand, uses the second arbitrage condition and obtains arbitrage-free dynamics of $k$ -dimensional instantaneous forward rates $F(t,T)$ . It involves no drift modeling, but volatilities need to be calibrated. It is more general, and, usually, less practical to use in practice. The HJM approach does not need spot-rate modeling. Yet, it also demonstrates that the spot rate $r_t$ is in general not Markov. 

The so-called classical approach uses the first arbitrage relation and tries to extract from the $\{B(t,T)\}$ a risk-adjusted model for the spot rate $r_{t}$ . This will involve modeling the drift of the spot rate dynamics, as well as calibration to observed volatilities. An assumption on the Markovness of $r_{t}$ is used along the way. 

427 

$r_{i}$ , or for the instantaneous forward rates, will also be “risk-adjusted.” That is, they will be valid under the risk-neutral measure $\tilde{P}$ . 

2 The Classical Approach 

The market practice is to start with a set of bond prices $\{B(t,T)\}$ that can reasonably be argued to be arbitrage-free. Then either one of the above relations can be used to go “backwards” and determine a model for $r_{t}$ or for the set of forward rates $\{F(t,s),s\in[t,T]\}$ . Because the two relations above hold under no-arbitrage conditions, the model that one obtains for 

Obviously, both relations can be exploited to calculate arbitrage-free prices of interest-sensitive securities. 

$B(t,T) = e^{-\cdots f_{t}^{T}F(t,s)ds}$ . 

The second arbitrage relation of Chapter 18 was between instantaneous forward rates $F(t,T)$ and bond prices: 

which gave arbitrage-free prices of default-free discount bonds $B(t, T)$ under the risk-neutral measure $\bar{P}$ . This was a relation between spot rates $r_{t}$ and bond prices $B(t, T)$ that held only when there were no arbitrage possibilities. 

$B(t,T) = E_t^{\bar{p}}\left[e^{-j_T^T r_s ds}\right],$ 

Market practice in pricing interest-sensitive securities can proceed in two different ways depending on which of the two arbitrage relations developed in the previous chapter is taken as a starting point. In fact, Chapter 18 discussed in detail the bond pricing equation 

1 Introduction 

## CHAPTER 9

Suppose one obtains a reasonably accurate observation on the discount curve $\{B(t,u),t<u\leq T\}$ that one can assume to be arbitrage-free. Then, Equation (1) says that the same spot rate process $r_{s}$ must satisfy the following set of equations: $^{2}$ 

That is, the $r_{t}$ process is in fact constant at $r_{t}^{1}$ . Using this information, we can price interest-sensitive derivatives written on $r_{t}$ or on $B(t, T)$ . For example, a bond option will have an arbitrage-free price equal to zero because $r_{t}$ is constant. 

Now suppose we do not know what type of stochastic process $r_{t}$ follows in reality. In fact, suppose our purpose is to determine this process from observations on liquid bonds that trade in the market. In particular, suppose we observe the following discount curve: 

prices will be arbitrage-free.
However, note that if we had posited a nondeterministic model for $r_{t}$ , the application of the same procedure would be problematic. In fact, this would require knowing the drift of the spot rate process under the risk-neutral measure $\bar{P}$ . In the above, the $r_{t}$ was constant, and hence its drift under $\bar{P}$ was zero. 

(11) 

$^{4}$ The selection of $V_{i}$ as a Wiener process is already made. This also may not be appropriate because real-world spot-rate processes may contain jumps. 

$t_0 < t_1 < \ldots < t_m,$ 

$dr_{t} = \lambda (\theta_{t} - r_{t})dt + \sigma \sqrt{r_{t}} dW_{t}$ . (10) Here, for each time period $t$ , the parameter $\theta_{t}$ is allowed to assume a different known value. This augments the number of free parameters that one has in system (5). For example, in a discrete setting with: 

2.3.2 A Mean-Reverting Model
The geometric SDE may be inappropriate for describing the dynamics of the spot rate, but from the above arguments we learned something. First, an appropriate SDE should be selected for $r_{t}$ , and then the parameters of this model should be determined (calibrated) so that the spot-rate model “fits” the discount curve $\{B(t,T_{i})\}$ given by liquid markets. If this can be done, and if the observed discount bond prices $\{B(t,T_{i}), i=0,\ldots,n\}$ are arbitrage-free, then the resulting model for the spot-rate process $r_{t}$ would also be arbitrage-free. It could be used to price interest-sensitive derivatives.
Thus, one may ask if one can postulate a SDE more realistic than the geometric process discussed in the first example. In fact, consider the mean-reverting spot-rate process with variable “mean” $\theta_{t}$ and a square-root diffusion component: 

But how attractive is it to postulate such strong dependencies among the $n + 1$ bond prices that one observes in liquid markets? Obviously, the spot-rate process postulated in Equation (8) is quite inadequate for practical pricing purposes. Other models must be sought. 

This is no simple task. In fact, given the reasonably accurate observations on the bond prices, $\{B(t,T_{i}), i=0,\ldots,n\}$ , in (2)–(5) we have $n+1$ equations with known left-hand sides. But the free parameters of the interest rate model that we can choose arc only the $\mu$ and the $\sigma$ . Hence we have to satisfy a system of $n+1$ equations by choosing two unknowns. This is not going to be possible unless there are strong interdependencies among observed bond prices $\{B(t,T_{i}), i=0,\ldots,n\}$ , so that n-1 of these equations are in fact redundant. Then, the system would in fact reduce to two equations in two unknowns and a set of $\mu$ , $\sigma$ that fits the observed arbitrage-free discount curve $\{B(t,T)\}$ can be found. 

But putting these two difficulties aside, consider the problem mentioned above: namely, how to select the $\mu$ and $\sigma$ such that all the equations in the system in (5) are satisfied simultaneously? $^{4}$ This is no simple task. In fact, given the reasonably accurate observation 

be a complicated nonlinear function of the level of spot rate $r_{t}$ , rather than being just a constant. 

2 The Classical Approach 

$^{3}$ Note the implicit assumption here. The increment in the spot rate depends only on the current $r_{1}$ , and hence the spot rate has a Markovian character. As we see below, this will be a special case in fixed-income markets where arbitrage conditions are satisfied. 

There will immediately be some headaches. A spot rate process obeying this model would eventually go to plus or minus infinity depending on the sign of $\mu$ , as $t \to \infty$ . Also, the percentage volatility of the $r_t$ will be constant. Clearly, these do not seem to be ideal properties to represent the behavior of overnight rates observed in reality. First, interest rates do not have "trends." Second, in reality percentage interest rate volatility seems to $dr_{t} = \mu r_{i}dt + \sigma_{t}dW_{t}$ . (8) Hence we have postulated that in (7) the drift and the diffusion coefficients are given by: 

2.3.1 A Geometric SDE
To see that the system in (2)-(5) comes with "hidden" complications, suppose we select for the spot rate $r_t$ , a geometric SDE driven by a Wiener process under the $\tilde{P}$ : 

and second, one has to select the $a(r_{t}, t)$ , $b(r_{t}, t)$ and the probabilistic behavior of the driving process $V_{t}$ , such that the system of equations shown in (5) are satisfied. $^{3}$ We consider two examples. 

arbitrage-free bond prices. Let us discuss these equations. Given the martingale measure that defines the expectation operator $E_t^p [\cdot]$ , the right-hand sides of all these equations depend on the same spot rate process $r_t$ , albeit with different $T_i$ . The market will determine the left-hand side of these $n + 1$ equations. The problem faced by the practitioner is to determine one model for the interest rate process $r_t$ such that all these equations are satisfied simultaneously. How can we guarantee that the specific model selected for the $r_t$ will be consistent with these $n + 1$ set of equations? This is indeed no straightforward task. Let us illustrate some of the difficulties involved. In fact consider what this requires. First, one has to postulate a spot rate 

arc the $n + 1$ maturities at which we have reasonably accurate and arbitrage-free bond prices. 

But, the model would not be complete. In fact, we do not yet have an arbitrage-free model given the “second factor,” $R_{t}$ . Before we can proceed and calculate the price, we need to obtain a risk-adjusted SDE for $R_{T}$ as well. For these issues we refer the reader to Brennan and Schwarz (1979) and the related literature. It must be realized that the two processes $r_{t}$ and $R_{T}$ may have complex time-varying correlation properties and computationally the problem may get much more difficult than the case of a single factor. 

2.4.2 A Second Factor
Things can get somewhat more complicated if we want to price a derivative instrument that is sensitive to $r_{t}$ and, say, to $R_{t}$ , a long rate, which is not perfectly correlated with $r_{t}$ . Suppose the price of this new instrument is denoted by $C(r_{t}, R_{t}, t)$ . The expiration date is again T, and the expiration payoff is given by the known function $G(r_{T}, R_{T}, T)$ : 

This expectation can be evaluated using Monte Carlo methods; or it can be solved for a closed-form solution if one exists; or it can be converted into a PDE, as will be seen in Chapter 21; or it can be evaluated in a tree model. This will be possible because we would already have a dynamics for $r_t$ under the $\tilde{P}$ : 

2.4.1 A One-Factor Model
Suppose we want to price a derivative instrument that is sensitive to $r_{t}$ only. Its price is denoted by $C(r_{t}, t)$ . The expiration date is T and the expiration payoff is given by the known function $G(r_{T}, T)$ : 

where the drift $\tilde{a}(r,t)$ has a “tilde” because it is assumed to be adjusted for the interest rate risk and consequently the $W_{t}$ is a Wiener process under the risk-neutral measure $\bar{P}$ . We consider two cases. 

$^{7}$ We can mention at least three specific uses, but there are many others that we do not go into because of the limited scope of this book: (1) It may be that there is a traded instrument $C(r_{t}, t)$ that can be synthetically replicated using the traded bonds $B(t, T)$ . (2) The $C(r_{t}, t)$ may be a new instrument that does not yet trade. (3) There may be some suspicion that $C(r_{t}, t)$ is mispriced by the markets. Then, by using an arbitrage-free model for $r_{t}$ , one can calculate a “fair” price for the instrument and take proper hedging, arbitrage, or speculative positions. Or, one could simply use the price in investment banking operations. 

The parameters n and m need not be the same.
That is, we can calibrate the free parameters of the SDE shown in (10) so that the volatilities of $B(t,T)$ obtained from Equation (1) match the volatilities observed in liquid options markets on these bonds. 

$dr_{i} = \tilde{a} (r,t)dt + b(r_{i},t)dW_{i},$ 

To see the use of the spot-rate model, consider the following setup. A reliable term structure $\{B(t,T)\}$ is given and is exploited to extract the arbitrage-free model for $r_i$ ; 

How would this model be used? The answer to this question was briefly mentioned at the beginning of this chapter. The bond pricing equation is used to extract an arbitrage-free spot-rate model from the existing term structure because using this model one can then price other interest-sensitive securities and obtain arbitrage-free prices without having to look at the markets for these securities. 

Suppose one successfully completes the project to extract an arbitrage-free model for the spot rate $r_{t}$ from the pricing equation: 

Besides, unlike geometric processes, mean-reverting processes are known under the right conditions not to explode as $t \to \infty$ . Also, given infinitesimal steps, the $r_t$ process that will be generated by the mean-reverting model will not become negative given the diffusion component adopted here. 

This gives more flexibility in fitting the interest rate process to the observed discount curve, $\{B(t,T_{i}), i=0,\ldots,n\}$ . In fact, we can not only fit the $r_{t}$ process to bond prices, but fit it to bond volatilities as well. See Hull and White (1990) for example. 

Let $B(t, T)$ and $B(t, U)$ be two default-free zero-coupon bonds that are identical except for their maturity $U > T$ . Let $F(t, T, U)$ be the interest rate contracted at time $t$ on a default-free forward loan that starts at $T$ and ends at $U$ . Herc, $F(\cdot)$ is a percentage rate for period $U - T$ . Thus, no days 

The idea is based on the second arbitrage relation developed extensively in Chapter 18. As mentioned there, there are direct relations between discount bonds that are identical except for their maturity and forward rates. It is sufficient to review a simple case. 

This is indeed a complicated task of indirect accounting for a complex set of arbitrage relations between market prices. The Heath-Jarrow-Morton, or as known in the market, HIM, approach attacks these arbitrage restrictions directly by bringing the forward rates to the forefront. 

$dr_{i} = \tilde{a}(r_{i},t)dt + b(r_{i},t)dW_{i}$ . 

The classical approach to pricing interest-sensitive securities is an attempt to extract these arbitrage relations from the $B(t, T)$ and then summarize them within an arbitrage-free spot-rate model: 

The arbitrage restrictions that we have been studying are the result of common random processes that influence discount bonds that are identical except for their maturity. If the liquid bonds that determine the term structure $\{B(t,T)\}$ are all influenced by the same unpredictable Wiener process $W_{t}$ , the respective prices must somehow be related to each other as suggested by the pricing relation: 

## 3 The HJM Approach to Term Structure

This leads to the following question: Is there another approach that one can use, which will be more in line with the philosophy of Black-Scholes? The answer is yes and it is the Heath-Jarrow-Morton (HJM) Model. 

Thus, in this sense, the spot-rate modeling that forms the basis of the classical approach appears to be a fundamentally different methodology from the arbitrage-free pricing as seen until now. 

the unknown drift of the underlying process by the known spot rate. There was no need to model the drift term of the stock price process. The latter was simply replaced by the (constant) spot rate r. As a result, Black-Scholes approach reduced the problem to one of volatility modeling. The assumption of a geometric process for the underlying process $S_{t}$ simplified this further and percentage volatility was assumed to be constant. 

$^{8}$ In the following chapters we will have a different notation for the risk-adjusted drift. As we develop new concepts that we can use, we will be able to write the risk-adjusted drift as $a(r_{t}, t) - \lambda_{t}b(r_{t}, t)$ , where the $\lambda_{t}$ is the Girsanov drift adjustment, or, in this case, the market price of interest rate risk. 

is satisfied for every T.
This is quite different from the philosophy used in the Black-Scholes world discussed in the first part of this book. There, the arbitrage restrictions were directly and explicitly incorporated into the model by replacing 

Related to each other across mathematics. More importantly, if one pursues the classical approach, arbitrage restrictions will be incorporated into the model indirectly, through fitting to the initial yield curve. One first starts with a set of discount bond prices, or the corresponding yields and then one tries to find a model for $r_t$ that "fits" the observed term structure so that 

We see that the classical approach to pricing interest-sensitive securities amounts, essentially, to spot-rate modeling. We also see that this calibration effort is not trivial, especially when discount bond prices are not perfectly related to each other across maturities. 

2.5 Comparison with the Black-Scholes World 

that yields an arbitrage-free model because the probability used in this pricing equation is the P. Hence, arbitrage-free spot-rate modeling is more than just an estimation or calibration problem. It is also based on judicious choice of pricing models. $^{8}$ 

would not be called arbitrage free. Econometric methods yield estimates for the real-world parameters, and the model would be valid under the real-world probability P. The Wiener process $W_{t}^{*}$ can be directly estimated from the data as continuous-time regression residuals.
It is the backward extraction of the $r_{t}$ process using 

$d r_{i} = a(r,t)dt + \sigma (r_{i},t)d W_{i}^{*}$ 

2.4.3 The Importance of Calibration
It is important to understand the process by which one obtains the spot-rate model in (2.4.1). If one used only econometric methods and estimated a continuous-time drift $a(r_{t}, t)$ and diffusion $\sigma(r_{t}, t)$ , the resulting model written as 

For the next section adopt the notation $B_{t}=B(t,T)$ and assume that for a typical bond with maturity T we are given the following stochastic differential equation: 

(13) 

From the relationship between the default-free pure discount bond prices $B(t, T_{i}), T_{i} < T^{\max}$ , with maturity $T_{i}$ and forward rates $F(t, T)$ derived in Chapter 19, we have: 

Here, we can keep the $\Delta > 0$ fixed and consider the joint dynamics of the $B(t, T)$ . $B(t, T + \Delta)$ as t changes. The joint dynamics can be modeled with the risk-neutral measure, or depending on the instrument to be priced, with the forward measure introduced in Chapter 17. Proceeding this way leads to the so-called BGM models, after the work in Brace, Gatarek and Musiela (1996). The remaining part of this chapter will proceed along the lines of original HJM approach by using the instantaneous forward rate $F(t, T)$ . 

we can obtain an arbitrage restriction on the dynamics for continuously compounded instantaneous rates $F(t,T)$ , as will be done in the next section. But this is only one way HJM models can proceed. Another option is to use forward rates for discrete, noninfinitesimal periods. That is, we can use models that are based on the $F(t,T,U)$ . Letting $U = T + \Delta$ , we can model arbitrage-free dynamics using the relationship: 

where $F(t,s)$ is the rate on a forward loan that begins at time s and ends after an infinitesimal time period ds.
Writing the arbitrage relation as 

$^{9}$ Let us repeat the arbitrage condition using somewhat different language. The $B(t, U)$ is the present value of a sure dollar to be received at a later date U. Its inverse if the time U value of $1 that we have now. Dividing the inverse by $1 + F(t, T, U)$ brings a time U value to time T: 

Here we have several options because the arbitrage relation can be written in several different ways.
The original approach used by HJM is to model the continuously compounded instantaneous forward rates $F(t, T)$ —that is, use the relation 

Incorporated in the forward rate dynamics. In other words, if we decided to model the forward rates $F(t, T, U)$ instead of the spot rate $r_t$ , the arbitrage relations can be directly built into the forward rate dynamics similar to the case of Black-Scholes. The development of the HJM approach is based on this idea. Of course, in this framework we still have to calibrate the volatilities. Also, we need to select the exact forward rates that the pricing will be based on. 

We thus have two bonds with different maturities in a single expression that contains $F(t, T, U)$ . Now consider the joint dynamics of these variables. Because bonds are traded assets, in the corresponding SDEs we can replace the drift parameters by the risk-free rate $r_t$ . Thus, up to this point everything is identical to Black-Scholes derivation. But, note that according to the arbitrage relation above, the ratio of the two risk-neutral bond dynamics will be captured by the movements of a single forward rate $F(t, T, U)$ . In other words, once risk-neutral dynamics of the bonds are written, the SDE for the forward rate $F(t, T, U)$ will be determined. There will be no need to calibrate and/or estimate any additional drift coefficients, or for that matter to adjust these coefficients for risk. All these will automatically be incorporated in the forward rate dynamics. 

$[1 + F(t,T,U)] = \frac{B(t,T)}{B(t,U)}.$ 

In expressions like these, letting $\Delta \rightarrow 0$ means taking the (standard) derivative of $g(\cdot)$ with respect to x. Writing these terms in brackets separately and $\frac{g(x + \Delta) - g(x)}{\Delta}$ . 

Now, we can let $\Delta \rightarrow 0$ . This will give the dynamics of the instantaneous forward rate. To do this, note that the way expression (20) is written. On the right-hand side, we have two terms that are of the form: 

This is the final result of applying Ito's Lemma to (16). This equation gives the arbitrage-free dynamics of a forward rate on a loan that begins at time $T$ and ends $\Delta$ period later. 

It is important to realize that the first terms in drift of the SDEs for $B(t, T)$ and $B(T, T + \Delta)$ are the same because the dynamics under consideration are arbitrage-free. Under $\bar{P}$ , discount bonds with different maturities will have expected rates of returns that equal the risk-free rate $r_{i}$ . This is essentially the same argument used in switching to the (constant) risk-free rate r in the drift of the SDE for a stock price $S_{i}$ utilized in Black–Scholes derivation.

Now substitute the stochastic differentials (18) and (19) in the definition of $F(t, T, T + \Delta)$ given in (16) and cancel the common $r_{i}dt$ terms: 

Now apply Ito's Lemma to $d\log B(t,T + \Delta)$ and get the equivalent expression with $T$ replaced by $T + \Delta$ .${}^{12}$ 

Simplifying and then substituting from the SDE for the risk-adjusted bond dynamics in (15): 

$^{1}$ Here, applying Ito's Lemma means varying the t parameter. The reader may mistakenly think at this point that we are trying to take the limit as $\Delta \rightarrow 0$ . This will be done, but for the time being the $\Delta$ is kept constant. 

$^{10}$ A geometric SDE would have the diffusion parameter written as $\sigma B_{i}$ , with $\sigma$ constant. Here we have $\sigma(t, T, B_{i})$ depend on $B_{i}$ as well. Hence, percentage bond volatility is not constant here. 

$d[\log B(t,T)] = \frac{1}{B(t,T)} dB(t,T) - \frac{1}{2B(t,T)^2}\sigma (t,T,B_t)^2 B(t,T)^2 dt.$ (17) 

In all aspects, except for the arbitrary dynamics of forward rates, apply Ito's Lemma to the right-hand side of (16), and use the risk-adjusted drifts when ever needed. $^{11}$ Apply Ito's Lemma first to log $B(t, T)$ to get: 

where a noninfinitesimal interval $0 < \Delta$ is used to define the non-instantaneous forward rate, $F(t,T,T + \Delta)$ , for a loan that begins at time $T$ and ends at time $T + \Delta$ . This is done by considering two bonds that are identical in all aspects, except for their maturity, which are $\Delta$ apart. 

$F(t,T,T+\Delta)=\frac{\log B(t,T)-\log B(t,T+\Delta)}{(T+\Delta)-T},$ 

where $r_{t}$ is the risk-free instantaneous spot rate, and $W_{t}^{T}$ is the new Wiener process under the risk-neutral measure $\tilde{P}$ . That is, by switching from P to $\tilde{P}$ , we have eliminated the unknown drift in the bond dynamics. 

Now, bonds are traded assets. In a risk-neutral world with application of the Girsanov theorem, the drift coefficient can be modified as in the case of the Black-Scholes framework: 

where the $V_{t}^{T}$ is a Wiener process with respect to the real-world probability P. We need to emphasize three points concerning this SDE. First, the diffusion parameter is written in terms of percentage bond volatility, but is not necessarily of geometric form. $^{10}$ Second, the SDE is driven by a Wiener process indexed by T. This means that, in principle, every bond with different maturity is allowed to be influenced by some different shock. Later, we will see the single factor case where all the $V_{t}^{T}$ will be required to be the same. And third, note the new way we write the diffusion parameter. The $\sigma(t,T,B_{t})$ is explicitly made a function of the maturity T. This is needed in the derivation below, but will be abandoned in later chapters. 

441 

Further, note that in the HJM approach there is no need to model any short-rate process. In particular, an exact model for the spot rate $r_{t}$ is not needed. Yet, suppose there is a spot rate in the market. What would the SDEs obtained for the forward rates $F(t,T)$ imply for this spot rate? The question is relevant because the spot rate corresponds to the nearest infinitesimal forward loan, the one that starts at time t.
Thus, realizing that 

(23) 

$r_{t}=F(t,t)$ (25)
for all t, we can in fact derive an equation for the spot rate starting from the SDEs for forward rates. Before we start, we simplify the notation and 

(24) 

It is worth emphasizing that the risk-adjusted drift of instantaneous forward rates depends only on the volatility parameters. This is again similar to the Black-Scholes environment where there was no need to model the expected rate of return on the underlying stock, but modeling or calibrating the volatility was needed. It is in this sense that the HIM approach can be regarded as a true extension of the Black-Scholes methodology to fixed income sector. 

A reader may wonder how one would obtain these risk-adjusted parameters that are valid under the condition of no-arbitrage. Well, the previous section just established that under no-arbitrage, risk-adjusted drift can be replaced by: 

Hence, the previous section derived the exact no-arbitrage restrictions on the drift coefficient for instantaneous forward rate dynamics. This is similar to the Black-Scholes approach that was seen several times in the first part of the book. There, the drift term $\mu$ of the SDE for a stock price $S_{t}$ was replaced by the risk-free interest rate r under the condition that there were no-arbitrage possibilities. Here, the drift is replaced not by r, but by a somewhat more complicated term that depends on the volatilities of the bonds under consideration. But, in principle, the drift is determined by arbitrage arguments and will hold only under the condition that there are no-arbitrage possibilities between the forward loan markets and bond prices. Throughout this process no “forward rate modeling” was done. 

where the $a(F(t,T),t)$ and $b(F(t,T),t)$ are supposed to be the risk-adjusted drift and the diffusion parameters, and the $W_{t}$ is the risk-neutral probability. 

$dF(t,T) = a(F(t,T),t)dt + b(F(t,T),t)dW_t,$ 

The HIM approach is based on imposing the no-arbitrage restrictions directly on the forward rates. First, a relation between forward rates and bond prices is obtained using an arbitrage argument. Then arbitrage-free dynamics are written for $B(t,T)$ . Given the SDEs for bond prices, a SDE that an instantaneous forward rate should satisfy is obtained. To see the real meaning of this, suppose we postulate a general SDE for the instantaneous forward rate $F(t,T)$ : 

where the $\sigma(\cdot)$ are the bond price volatilities. We have several comments to make on this result. 

$\lim _{\Delta \to 0}\frac{1}{2\Delta} [\sigma (t,T + \Delta ,B(t,T + \Delta))^2 -\sigma (t,T,B(t,T))^2 ]$ 

The HJM approach exploited the arbitrage relation between forward rates and bond prices to impose restrictions on the dynamics of the instantaneous forward rates directly. By doing this it eliminated the need to model the expected rate of change of the spot rate. 

and would not be captured by a state variable. The difference between (29) and (32) will depend on interest rates observed before $t - \Delta$ . This would make the interest rate non-Markov in general.
Next we see an example. 

In fact, the new term in the equation for $r_{t}$ is more like a cross product. Hence, the similar term for an interest rate observed $\Delta$ period before the $r_{t}$ would be 

that, in general, will be a complex function of all past forward rate volatilities. In particular, this term is not simply an “accumulation” of past changes the way a typical drift or diffusion term would lead to 

Here, the forward rate in the first expectation is known at time t; hence it comes out of the expectation sign. The third expectation on the right-hand side is zero because it is taken with respect to a Wiener process. But the second term is in general positive and does not vanish. Hence we have: 

$\left[\{r_t^1\}, \{r_t^2\}, \dots, \{r_t^N\}\right]$ . 

Consider the following exercise. Select M standard normal random variables using some random number generator. Multiply each random number by $\sqrt{\Delta}$ . Start with a historical estimate of $\kappa$ and obtain the first Monte Carlo trajectory for $r_{t}^{1}$ starting with $r_{0}$ and using Equation (38) recursively. Repeat this N times to obtain N such spot-rate trajectories: 

Suppose we know that increments $[W_{t}-W_{t-\Delta}]$ are independent and are normally distributed with mean zero and variance $\Delta$ . Suppose we have also calibrated the volatility parameter $\sigma$ and the speed of mean reversion $\alpha$ . Hence, there is only one unknown parameter $\kappa$ . Finally, we also have the initial spot rate $r_{0}$ . 

where $\Delta$ is the discretization interval. The remaining part of the calibration exercise depends on the method adopted. We discuss some simple examples. 

$dr_{i} = \alpha (\kappa -r_{i})dt + \sigma dW_{i}$ 

to this term structure. How can this be done in practice? Several methods are open to us. They all start by positing a class of plausible spot-rate models and then continue by discretizing it. Thus, we can let $r_{t}$ follow the Vasicek model: 

$dr_{i} = a(r_{i},t)dt + b(r_{i},t)dW_{i}$ 

Suppose we are given an arbitrage-free family of n bond prices $B(t, T_{i})$ , $i = 1, \ldots, n$ . Suppose also that we decided to use the classical approach to price interest-sensitive securities. Assuming a one factor model, we first need to fit a risk-adjusted spot-rate model 

of the conceptual issues. Some simple examples of how an arbitrage-free spot-rate model can be obtained fall into this category. We discuss this briefly at the end of the chapter. 

445 

4 How to Fit $r_{t}$ to Initial Term Structure 

At several points in this chapter we discussed how a spot-rate model can be "fit" to an existing term structure known to be arbitrage-free. But, during this discussion, we never showed how this could be done in practice. This book tries to keep numerical issues to a minimum, but there are some cases where a discussion of practical pricing methods facilitates the understanding 

## 4 How to Fit $r_{i}$ to Initial Term Structure

The recent models that exploit the forward measure seem to be an answer to problems of instantaneous forward-rate modeling, and should be considered as a promising alternative. 

It is also true that there are significant resources invested in spot-rate models both financially and time-wise. There is, again, a great deal of familiarity with the spot-rate models, and it may be that they provide good approximations to arbitrage-free prices anyway.
The recent models that exploit the forward measure seem to be an an-

As discussed in Musiela and Rutkowski (1997), modeling the instantaneous spot rate has its own difficulties. When one imposes a Gaussian structure to SDEs that govern the dynamics of the $dF(t,T)$ and when one uses constant percentage volatilities, the processes under consideration explode in finite time. This is clearly not a very desirable property of a dynamic model. It can introduce major instabilities in the pricing effort. 

However, it appears that market practice still prefers the classical approach and continues to use spot-rate modeling one way or another. How can we explain this discrepancy? 

The HJM approach is clearly the more appropriate philosophy to adopt from the point of view of arbitrage-free pricing. It incorporates arbitrage restrictions directly into the model and is more flexible. 

3.6 Market Practice 

This point is important because current empirical work indicates that spot rate behavior in reality may fail to be Markovian. Hence, from this angle, the HJM approach provides an important flexibility to market practitioners. 

But the approach has other advantages as well. As was seen in earlier chapters, a $k$ -dimensional Markov process would in general yield non-Markov univariate models. Hence, within the HJM framework one could in principle impose Markovness on the behavior of a set of forward rates and in a multivariate sense this would be a reasonable approximation. Yet, in a univariate sense when we model the spot rate, the latter would still behave in a non-Markovian fashion. 

447 

This chapter has briefly summarized the two major approaches to pricing derivative securities that depend on interest rates. The classical approach was shown to be an effort in spot-rate modeling. The arbitrage restrictions were incorporated indirectly through a process of “fitting an initial curve.” The HIM approach on the other hand was an extension of the Black-Scholes formula to interest-sensitive securities. 

6 References 

$D(t,t)\equiv C(t,t,\kappa)$ . Then, we can minimize the distance between the closed-form solution and the observed arbitrage-free yield curve by choosing $\kappa$ in some optimal sense: 

and get a closed-form solution for the $B(t,T)$ , as will be discussed in the next chapter. Suppose this results in the function: 

The best source on these issues is Musiela and Rutkowski (1998). Of course, this source is quite technical, but we recommend that readers who are seriously interested in fixed-income sector put in the necessary effort and become more familiar with it. The excellent discrete time treatment, Jarrow (1996), should also be mentioned here. 

where the $r_{i}^{j}$ are the i'th element of the j'th tree trajectory and $N_{k}$ is the number of tree trajectories for a bond that matures after $T_{k}$ steps. These trajectories depend on the $u_{i}, d_{i}$ , and hence, these equations can be used to determine the latter. To do this we need to impose enough restrictions such that the total number of unknown parameters in the tree becomes equal to the number of equations. The tree parameters can then be obtained from these equations. The tree will fit the initial term structure exactly. An example to this way of proceeding is in Black, Derman, and Toy (1984). 

Given this restriction, the tree will be recombining and at every stage we will have i unknown parameters. The next task will be to determine these $u_{i}, d_{i}$ by using the equality: 

$u;d_{i}=1.$ 

Once we consider a binomial model for movements in $r_{i}$ we can choose the relevant parameters so that the tree trajectories “fit” the arbitrage-free term structure and the relevant volatilities. For example, we can assume that we have N arbitrage-free bond prices. Suppose we also know the volatilities $\sigma_{i}$ of each bond $B(t,T_{k})$ . Let the up and down movements in $r_{i}$ at stage i be denoted by $u_{i}, d_{i}$ , such that: 

The previous approach used a single parameter $\kappa$ to make calculated bond prices come as close as possible to an observed term structure. The fit was not perfect because the distance between the two term structures was not reduced to zero, although it was minimized. By adopting a general tree approach one can “improve” the fit.

Once we consider a binomial model for movements in r, we can choose 

This way we find a value for $\kappa$ such that the calculated term structure is as close as possible to the observed term structure. Once such a $\kappa$ is determined, the $r_{i}$ dynamics becomes (approximately) arbitrage-free, in the sense that using the model parameters, and this new $\kappa$ , one can obtain bond prices that come “closc” to the observed term structure. 

where M may be different for each bond, depending on the maturity. Now, because $\kappa$ was selected arbitrarily, the $\hat{B}(t,T_{i})$ will not be arbitrage-free. But, we also have the observed term structure, which is known to be arbitrage-free. So, we can try to adjust the $\kappa$ in a way to minimize the distance: 

Then calculate the prices by using the sample equivalent of the bond pricing formula: 

446 CHAPTER·19 Classical and HJM Approaches to Fixed Income 

(d) Given a default-free zero-coupon bond, $B_n$ , that matures at time $t = n$ , and all the forward rates $\{f_0, \ldots, f_{n-1}\}$ , obtain a formula that expresses $B_n$ as a function of $f_t$ . 

$\{f_0 = 8\%, f_1 = 9\%, f_2 = 10\%, f_3 = 18\%\}$ . 

We also have one-period forward rates $\{f_0, f_1, f_2, f_3\}$ , where each $f_i$ is the rate contracted at time $t = 0$ on a loan that begins at time $t = i$ and ends at time $t = i + 1$ . In other words, if a borrower borrows $N at time $t = i$ , he or she will pay back $N(1 + f_i)$ at time $t = i + 1$ . The spot rate is denoted by $r_i$ . By definition we have 

(a) Derive a univariate representation for the short rate $r_{t}$ .
(b) According to this representation, is $r_{t}$ a Markov process?
(c) Under what conditions, if any, would the univariate process $r_{t}$ be Markov? 

where the error term is jointly normal and serially uncorrelated. Suppose $r_{i}$ is a short rate, while $R_{i}$ is a long rate. 

such that $X_{i}$ is a first-order Markov?
(d) Can you write a continuous time equivalent of this system?
(e) Suppose short or long rates are individually non-Markov, possible that they are jointly so? 

1. Consider the equation below that gives interest rate dynamics in a setting where the time axis $[0, T]$ is subdivided into n equal intervals, each of length $\Delta$ : 

The r is the constant risk-free instantaneous spot rate, the $S_{i}$ is the price of a stock that paid no dividends, the F is the time t price of a European call option written on the stock. The K and the T are the strike price and the expiration date of the call, respectively. In Chapter 15 it was also 

$-rF + F_{t} + rS_{t}F_{s} + \frac{1}{2}\sigma^{2}S_{t}^{2}F_{ss} = 0,$ 

The reader is already familiar with various derivations of the Black-Scholes formula, one of which is the partial differential equations (PDE) method. In particular, Chapter 12 showed how risk-free borrowing and lending, the underlying instrument, and the corresponding options can be combined to obtain risk-free portfolios. Over time, these portfolios behaved in such a way that small random perturbations in the positions taken canceled each other, and the portfolio return became deterministic. As a result, with no default risk the portfolio had to yield the same return as the risk-free spot rate r, which was assumed to be constant. Otherwise, there would be arbitrary opportunities. The application of Ito's Lemma within this context resulted in the fundamental Black-Scholes PDE. The Black-Scholes PDE was of the form: 

# Classical PDE Analysis for Interest Rate Derivatives

(c) Would these assumptions be appropriate under the risk-neutral measure obtained using money market normalization? Explain.  
(d) How would the use of the forward measure that corresponds to each $L_{t}$ improve the situation?  
(e) In fact, can you obtain the forward measures for times $t = 1,2?$ (f) Price the call option for time $t = 2$ using the forward measure. 

(iii) We can use the Black formula to price the calls. 

(ii) Each $f_{i}$ is normally distributed with mean zero and constant 

(i) Each $f_{i}$ is a current observation on the future unknown value 

(a) How can you price such an option?
(b) Suppose we assume the following: 

where N is a notional amount that we set equal to one without loss of any generality. 

$C^i = N\max [L_i - K,0],$ 

4. Consider again the setup of Question 1. Suppose we want to price three European style call options written on one period (spot) Libor rates $L_{i}$ with i = 0, 1, 2, 3, as in the above case. Let these option prices be denoted by $C_{i}$ . Each option has the payoff: 

(g) Can we claim that all $f_{i}$ are normally distributed? Prove your answer. 

Can all $B_{i}$ be determined independently? (f) In the system above can all the $\{f_i\}$ be determined independently? 

$\left[ \begin{array}{cc}B_{1}\\ B_{2}\\ B_{3}\\ B_{4} \end{array} \right] = \left[ \begin{array}{cc}1 & 1\\ B_{2}^{u} & B_{2}^{d}\\ B_{3}^{u} & B_{3}^{d}\\ B_{4}^{u} & B_{4}^{d} \end{array} \right]\left[ \begin{array}{c}\psi_{1}\\ \psi_{2} \end{array} \right].$ 

CHAPTER • 19 Classical and HJM Approaches to Fixed Income
(e) Now consider the Fundamental Theorem of Finance as applied to the system: 

$^{2}$ The $r_{t}$ is more like a percentage return, a pure number. $^{3}$ Or in case of two-factor models, two independent Wiener processes. 

Yet, there are differences when compared with the case of stocks. In the classical Black-Scholes derivation, the spot rate was assumed to be constant. This assumption did not appear to be very severe. In the case of interest-sensitive securities, the assumption of a constant interest rate cannot be maintained. On the contrary, the randomness that drives the system comes from infinitesimal Wiener increments that affect instantaneous spot rate $r_{t}$ . But, this latter is not an asset price as mentioned earlier. The unknown drift of interest rate dynamics cannot be simply made equal to the risk-free rate by invoking arbitrage arguments. This introduces major complications in the derivation and numerical estimation of PDEs for interest rate derivatives. In fact, although the steps in the following derivation are mathematically straightforward, they are somewhat more convoluted than in the case of plain-vanilla call options written on stocks.

Finally, we should reiterate that the “classical” approach adopted here is heuristic just like the derivation of the Black-Scholes PDE. A techni-

The same idea can be extended to interest-sensitive securities. For example, except for their maturities, bonds are “similar” instruments. They are expected to be influenced by the similar infinitesimal random fluctuations. Hence, under some conditions, a portfolio formed using two (or more) bonds can be made risk-free if portfolio weights are chosen carefully. 

In this chapter we show that prices of interest rate derivatives will satisfy PDEs similar to the fundamental Black-Scholes PDE using the “classical steps.” But, this derivation will still be fundamentally different than the one followed in Chapter 12 because the underlying variable will now be the spot rate $r_{t}$ . Spot rate is not an asset price, in contrast to the $S_{t}$ which represented the price of a traded asset in the Black-Scholes world. $^{2}$ Obviously, the difficulties associated with spot-rate modeling will be present here also. The derivation of the fundamental PDE for interest-sensitive securities will follow steps similar to the classic paper by Vasicek (1977). The essential idea is to incorporate in the dynamics of the returns the arbitrage conditions implied by a single Wiener process $^{3}$ that determines the random movements observed in more than one asset. In the case of the Black-Scholes approach, we worked with two securities, the underlying stock and the call option written on it. An infinitesimal random movement in the price of the stock also affected the price of the option. Hence we had two prices driven essentially by the same source of randomness. These securities could be combined in a careful fashion with risk-free borrowing and lending so that the unpredictable random movements canceled each other and the resulting portfolio became “riskless.” 

$^{1}$ We remind the reader that risk-free portfolios are not self-financing, and as a result the method is not mathematically accurate in continuous time. Yet, one still obtains the “correct” PDE because the extra cash flow invested or withdrawn over time has an expected value of zero. This issue was discussed in Chapter 12 in more detail. We keep utilizing this heuristic method with the condition that the reader keeps in mind this important point. 

and a certain class of partial differential equations. In stochastic calculus, these topics come under the headings of “Generators for Ito Diffusions,” “Kolmogorov Backward Equation,” and more importantly, “Feynman-Kac formula.” Using these methods, given a conditional expectation such as in (4), we can directly obtain a PDE that corresponds to it and vice versa. Of course, this correspondence depends on some additional conditions concerning the underlying random variables, but is clearly a very convenient tool for the financial market practitioner. Yet, the discussion of these “modern” methods should wait until the next chapter. 

The second way of obtaining PDEs for interest-sensitive securities is by exploiting the martingale equalities and the so-called Feynman-Kac results directly. In fact, when we investigate the relationship between a certain class of expectations and PDEs, we are led to an interesting mathematical regularity. It turns out that there is a very close connection between a representation such as: 

These questions can be answered in two different ways. First, we can follow the same approach as in Chapter 12 and obtain a PDE for discount bond prices along the lines similar to the derivation of the Black-Scholes PDE. In particular, we can form a “risk-free” portfolio and equate its deterministic return to that of a risk-free instantaneous investment in a savings account. Application of Ito's Lemma should yield the desired PDE. $^{1}$ 

calculated with the risk-neutral probability $\tilde{P}$ .
Given that we are now dealing with derivatives written on interest-sensitive securities, we can now ask (at least) two questions: 

$F(S_{t},t) = E_{t}^{\bar{P}}\left[e^{-r(T - t)}F(S_{T},T)\right],$ 

452 CHAPTER • 20 Classical PDE Analysis for Interest Rate Derivatives mentioned that the solution of this PDE corresponded to the conditional expectation 

These steps justify the particular values chosen for the portfolio weights $\theta_{1}, \theta_{2}$ . These weights were selected so that the $dW_{i}$ term drops from the SDE of the portfolio P. This is similar to the derivation of the 

These increments do not have a Wiener component and are completely predictable. 

$$
- \theta_ {2} \left[ \mu (B ^ {2}, t) B ^ {2} d t + \sigma_ {2} (B ^ {2}, t) B ^ {2} d W _ {t} \right].
$$

$$
d \mathcal {P} = \theta_ {1} \left[ \mu (B ^ {1}, t) B ^ {1} d t + \sigma_ {1} (B ^ {1}, t) B ^ {1} d W _ {t} \right]
$$

$$
d \mathcal {P} = \theta_ {1} d B ^ {1} - \theta_ {2} d B ^ {2},
$$

where $\sigma_{i}, i = 1,2$ are the volatility parameters $\sigma_1(B^1,t),\sigma_2(B^2,t)$ of the two bonds as described in Equations (7) and (8). As time passes, this portfolio's value will change. Acting as if the portfolio weights are constant, the implied infinitesimal changes will be given by: 

$$
\theta_ {2} = \frac {\sigma_ {1}}{B ^ {2} (\sigma_ {2} - \sigma_ {1})} \mathcal {P},
$$

$$
\theta_ {1} = \frac {\sigma_ {2}}{B ^ {1} (\sigma_ {2} - \sigma_ {1})} \mathcal {G}
$$

To derive a PDE for a discount bond's price, we first need to form a risk-free portfolio $\mathcal{P}$ , made of the two bonds $B^{1}, B^{2}$ at time $t^{4}$ . In particular, without any loss of generality, it is assumed that $\theta_{1}$ units of $B^{1}$ are purchased, and $\theta_{2}$ units of $B^{2}$ are shorted, for a total portfolio value: 

probability $P$ . Note the critical restriction imposed on this spot-rate dynamics; the parameters $a(r_t, t), b(r_t, t)$ are assumed to depend only on the latest observation $r_t$ , so that previous $r_s, s < t$ do not affect the drift and volatility parameters. We already know from the previous chapter that this Markov property of $r_t$ will be violated in a general term-structure model. Still, the classical approach proceeds assuming that it is a reasonable approximation. 

where the drift $a(r_{t}, t)$ and the diffusion $b(r_{t}, t)$ parameters are assumed to be known. They are either estimated from historical data, or as in the practical approaches, calibrated using market prices. It is also worth emphasizing that the $W_{t}$ here is a Wiener process with respect to the real world probability $P$ . 

Note two points. First, the diffusion terms are a function of the same $W_{i}$ , but depend on different diffusion parameters $\sigma_{i}, i=1,2$ . Second, the volatility parameters are written in terms of percentage volatility, but the bond dynamics are not necessarily given by geometric processes because the drift and diffusion parameters are also allowed to depend on $B^{i}, i=1,2$ , and are not constant as would be required by a geometric SDE. Because we are adopting a “classical” approach we now need to posit an interest rate model. We let the dynamics of $r_{i}$ be given by: 

$$
d B ^ {1} = \mu (B ^ {1}, t) B ^ {1} d t + \sigma_ {1} (B ^ {1}, t) B ^ {1} d W _ {t},
$$

The first step is to set the framework. We assume that we are provided two SDEs describing the dynamics of two default-free discount bond prices, $B(t, T_1)$ and $B(t, T_2)$ , with maturities $T_1, T_2$ such that $T_1 < T_2$ . The bond prices are driven by the same Wiener process $W_t$ . To simplify the notation, in this section we ignore the time subscript $t$ and write: 

## 2 The Framework

cally correct derivation would incorporate in the argument the condition that the risk-free portfolios are also self-financing. As discussed earlier, the approach below may not yield self-financing portfolios. 

454 CHAPTER·20 Classical PDE Analysis for Interest Rate Derivatives 

$^{6}$ There will be arbitrage restrictions because we have assumed that all bond prices are driven by the same Wiener process $W_{c}$ . 

It turns out that the way to eliminate the “unknown” drift $\mu(B,t)$ from (26) is by using arbitrage arguments. Recall that in the case of Black-Scholes PDE, one simply “replaces” the $\mu(B,t)$ by the constant spot rate r. But in the present case this is not possible because we keep using the spot-rate drift $a(r_{t},t)$ in (26). If we replaced the $\mu(B,t)$ by $r_{t}$ , this would require adjusting the spot-rate drift $a(r_{t},t)$ in (26) to its risk-neutral 

Here we have two equations (25) and (26) that we can exploit in obtaining the PDE for bond prices. In fact, this last Equation (26) is already a PDE except for the fact that it contains the unknown $\mu(B,t)$ . Also, note that up to this point we did nothing that would incorporate the arbitrage restrictions that we must have in this system. $^{6}$ 

under the probability P. This means that we can equate the drift and diffusion coefficients. Setting the two diffusion coefficients in (23) and (24) equal to each other, we obtain: 

where again the $W_{t}$ is a Wiener process with respect to the real-world probability P. This SDE must be identical to the original equation that drives the bond price dynamics. Simplifying the notation, this SDE is: 

The third step of the PDE derivation for bond prices is to use the previous results in Ito's expansion for $B(t,T)$ . Remembering that $B(t,T)$ is also a function of $r_{t}$ , and applying Ito's rule: 

4 Derivation of the PDE 

This term is called the market price of interest rate risk. As can be seen from the derivation, it is in general a function of $r_t$ and $t$ . But in the following section we will simply write it as $\lambda_t$ while assuming that this dependence is kept in mind. Note again that $\lambda_t$ is independent of the bond maturity. It is worth mentioning that a similar market price of equity risk was present in the Black-Scholes framework but was not used explicitly. In contrast to the case of Black-Scholes PDE, with interest-sensitive securities we do have to use the $\lambda_t$ explicitly in deriving the PDEs here. 

That is, the risk premia offered by bonds of different maturities are equal, once normalized by the corresponding volatility parameter. Risk premia of per unit volatility are the same across bonds. Bonds with higher volatility pay proportionately higher risk-premia. $^{5}$ This result is not very unexpected because at the end, these bonds have the same source of risk given the common $dW_{i}$ factor. Obviously, if one of the bonds was a function of an additional and different Wiener process, say $W_{i}^{*}$ , then even under a no-arbitrage condition, risk premia per volatility unit could be different across bonds. Note, in passing, that these risk premia can very well be negative.

Now, during this derivation the maturities of the underlying bonds were selected arbitrarily. Thus, similar equalities should be true for all discount bonds as long as their dynamics are driven by the same Wiener process $W_{i}$ . This gives a term $\lambda(r_{i}, t)$ that is relevant to all bond prices, $B(t, T_{i})$ : 

This SDE does not contain a diffusion term and the dynamic behavior of $d\mathcal{P}$ is riskless. Hence, we can now use the standard argument and claim that this portfolio should not present any arbitrage opportunities and its deterministic return should equal the $r_t\mathcal{P}dt$ : 

Black-Scholes PDE. Indeed, replacing the $\theta_{t}$ , dividing and multiplying by $\mathcal{P}$ , and arranging the $d\mathcal{P}$ can be written as: 

A second fundamental point of the above derivation is the assumption of a single driving process $r_{t}$ . Remember that the dynamics of all bond prices were assumed to be driven by the same univariate Wiener process $W_{t}$ . Because the same Wiener process is present in the SDE for the spot rate $r_{t}$ , this assumption enabled us to obtain a convenient no-arbitrage condition that was a function of a single market price of risk $\lambda_{t}$ . Clearly, this may not be the case. Making a single stock price a function of a single random process, $W_{t}$ , may be an acceptable approximation; doing the same thing for a set of discount-free bonds ranging from very short to very long maturities may be more questionable. 

In case of the spot-rate approach to pricing interest-sensitive securities, the use of no-arbitrage conditions will again introduce the spot rate $r_{t}$ in the PDE. Yet, along with the $r_{t}$ , two new parameters enter, namely the spot-rate drift $a(r_{t}, t)$ and the $\lambda$ , market price of interest rate risk. These parameters need to be estimated or calibrated if the PDE is to be used in real-world pricing. As mentioned in the previous chapter, this is a departure from the practicality of the Black-Scholes approach, which required the modeling of volatilities only. But it is also a change in philosophy because, in a sense, a complete modeling of the $r_{t}$ process is now needed. 

However, notice a rather important difference. In the case of the Black-Scholes derivation, by using the no-arbitrage condition we succeeded in completely eliminating the need to model and calibrate the drift of the stock price process $S_{i}$ . In fact, in the Black-Scholes derivation, expected change in $S_{i}$ did not matter at all. The option price depended on the relevant volatilities only. 

The approach was to modify the drift of the bond dynamics using the market price of risk for $r_{t}$ . The reader should realize that letting 

The general strategy in deriving the PDE was similar to the case of Black-Scholes. The main difference arises from the fact that the driving process in the present case is not $S_{r}$ , the price of an asset, but is the spot rate $r_{i}$ , which is a pure number. Hence the no-arbitrage conditions have to be introduced in a different way than just making the unknown drift coefficient equal to the risk-free rate. 

We now summarize the major aspects of this derivation and compare it with the approach taken in the case of Black-Scholes PDE. 

The drift of this SDE is now adjusted for “interest rate risk.” Whenever the bond price drifts are switched from $\mu(\cdot)$ to $r_{t}$ , one needs to switch the spot-rate dynamics from $a(r_{t}, t)$ to $(a(r_{t}, t) - b(r_{t}, t)\lambda_{t})$ . 

drift of the spot-rate dynamics.
In fact, it is as if we are using the drift from the spot-rate dynamics, written under the risk-neutral measure $\tilde{P}$ . Invoking the Girsanov theorem for Equation (9) and switching from the Wiener process $W_{t}$ defined under P, to the Wiener process $\tilde{W}_{t}$ defined under $\tilde{P}$ , we obtain a new SDE for $r_{i}$ . 

If one had an interest rate model with known drift $a(r_{i}, t)$ and diffusion coefficient $b(r_{i}, t)$ , to use this PDE in practice, one would still need an estimate for the $\lambda_{i}$ . Otherwise the equation is not usable. Also, it is worth realizing that in this PDE the coefficient of $B_{i}$ is equivalent to a risk-adjusted drift of the spot-rate dynamics. 

This is a PDE for the price of a default-free pure discount bond $B(t, T)$ . The associated boundary condition is simpler than the case of Black-Scholes. The bond is default-free and at maturity is guaranteed to have a value of 1, regardless of the level of spot rates at that time: 

equivalent as well. But the $r_{t}$ is not the price of an asset and it is not clear how this adjustment can be done. This problem can be resolved by utilizing the market price of interest rate risk $\lambda_{t}$ .
In fact, Equation (20) gives the market price of risk $\lambda_{t}$ as: 

458 CHAPTER 20 Classical PDE Analysis for Interest Rate Derivatives 

where $W_{i}$ is a Wiener process under the real-world probability. Note that the volatility structure is restricted to be a constant absolute volatility denoted by b. Suppose further that the parameters $\alpha, \kappa, b$ , and $\lambda$ are known exactly. Then, the fundamental PDE for a typical $B(t, T)$ will reduce to: 

This bond pricing function will satisfy the boundary condition and the fundamental PDE. It is the usual discount at a constant instantaneous rate r. 

$a(t_{i},t),b(t_{i},t)$ and $s_t$ can be obtained. The analogy is with the fundamental PDE of Black-Scholes and the Black-Scholes formula. Given enough assumptions on the $S_{t}$ process and the constancy of the interest rates, one was able to solve that PDE to get the Black-Scholes formula. In the present framework, given enough assumptions about the interest rate process $r_t$ one can do the same for the bond price PDE. We discuss some simple examples. 

The fundamental PDE for bond prices can sometimes be solved for a closed-form solution. This way, an explicit formula that ties $B(t,T)$ to the maturity $T$ , the "current" spot rate $r_t$ , and the relevant parameters $a(r_t,t),b(r_t,t)$ and $\lambda_t$ can be obtained. 

## 5 Closed-Form Solutions of the PDE

Nevertheless, our purpose in this book is to display the relevant tools rather than obtaining satisfactory pricing methods for actual markets. The assumption of a single factor is useful to this end. $^{7}$ curve is shown in Figure 2 for the same set of initial spot rates. Note that the mean-reverting aspect of the interest rate SDE determines that the yield curve can have upward- or downward-sloping curves, as well as flat ones. This is because if the spot rate is $15\%$ currently, the model assumes that it will go back toward its mean $5\%$ as we consider the long bonds. Thus long bonds would automatically be priced by using rates on the average around $5\%$ , whereas short bonds will be priced by using short rates closer to $15\%$ . The case of a current short rate below the long-run mean is the reverse and gives an upward-sloping yield curve. Figure 3 shows the effect of changing the value of market price of risk $\lambda$ on the discount curve, assuming $r = 5\%$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a1ccff69-6b24-4389-b2f8-232fb22b064b/67683fd5bdffca233b52e3234e2f1180c3507569b1ffc78f8e7e8b215866fbbe.jpg)


The graph of the $\{B(t,T),T\in[0,T^{\max}]\}$ with $\{\lambda=-.10,b=.015,\alpha=.25,\kappa=.05\}$ at three different levels for the spot rate $r=.5\%$ , $r=5\%$ , $r=15\%$ are shown in Figure 1. Because these are discount bond prices, the short maturities have values close to 1, whereas longer maturities get progressively cheaper. 

Using these parameters, we can calculate the bond pricing function $B(t,T)$ that will depend on the initial interest rate $r$ and on the maturity parameter $T$ . This is the so-called "discount curve" discussed earlier. 

where the $\mu, \sigma$ are the unknown bond drift and volatility parameters. Then, we know that 

To apply the formula, we need the market price of interest rate risk. Assume that we have 

Further, suppose the absolute interest rate volatility is .015 during one year: 

5.2.1 Example
For example, consider an economy where the long-run mean of the spot rate is 5% and where the spot rate is pulled toward the long-run mean at a rate of .25. We thus have 

462 CHAPTER·20 Classical PDE Analysis for Interest Rate Derivatives 

where the $W_{t}$ is a Wiener process under the real-world probability and the $\sigma$ is a constant volatility. The initial spot rate $r_{0}$ is known to be 5%. 

The PDE solution for bond prices can be found in all major sources. The reader may, however, prefer to read first the original paper by Vasicek that can be found in “Vasicck and Beyond.” Two other good sources are Cox-Ingersoll-Ross (1985) and Hull and White (1990). 

This chapter dealt with the classical approach to deriving PDEs for interest-sensitive securities. We see that although the major steps are similar to the case of Black-Scholes, there are some major differences in terms of practical applications and the underlying philosophy between the two cases. The classical approach to pricing interest rate-sensitive securities rests on modeling the drifts of the underlying stochastic processes, whereas the Black-Scholes approach was one where only the volatilities needed to be modeled and calibrated. 

This PDE can again be solved for a closed-form bond-pricing equation. The resulting expression is somewhat more complex than the case of Va-sicek. It is given by 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a1ccff69-6b24-4389-b2f8-232fb22b064b/8c4044532143059e024fd585aa2ff27ce8a9e7fbf7d3c2d3320c74b2647ead5e.jpg)


$B_{r}(a(r_{t},t)-\lambda_{t}b(r_{t},t))+B_{t}+\frac{1}{2}B_{rr}b(r_{t},t)^{2}-r_{t}B=0,$ 

At other times, the pricing was discussed using PDE methods. For example, in the previous chapter, using the method of risk-free portfolios we derived the PDE that a default-free discount-bond price $B(t,T)$ must satisfy under the condition of no-arbitrage: 

$F(S_{t},t) = e^{-r(T - t)}E_{t}^{\bar{P}}[F(S_{T},T)].$ 

to price a derivative with expiration payoff $F(S_T, T)$ , written on $S_t$ . According to this, the conditional expectation under the risk-neutral measure, $\bar{P}$ , of future payoffs would equal the current arbitrage-free price $F(S_t, t)$ , once discounted by the random discount factor $e^{-f_t^t r_t ds}$ . When the $r_t$ was constant, as was the case under the Black-Scholes assumptions, this formula simplified to: 

Throughout this book we keep alternating between mathematical tools for two major pricing methods. Using the Fundamental Theorem of Finance and normalizing by the money market account, we often used the representation 

# Relating Conditional Expectations to PDEs

eters?
(g) What does the R represent? 

(f) Suppose $T \rightarrow \infty$ , what happens to the drift and diffusion param-

and its volatility?
(e) Is the risk premium, that is, the return, in excess of risk-free rate proportional to volatility? To market price of risk? Is this impor-

ket price of risk $\lambda$ ? (d) What is the relationship between the maturity of a discount bond 

and that the diffusion parameter equals: 

Now consider the following questions that deal with properties of discount bonds whose prices can be represented by this formula. 

where the $W_{t}$ is a Wiener process under the real-world probability. Under this spot rate model, the solution to the PDE that corresponds to a default-free pure discount bond $B(t,T)$ gives the closed-form bond pricing formula $B(t,T)$ : 

2. You are given the spot-rate model: 

der these conditions.
(c) Can you determine the solution to this PDE?
(d) What is the market price of interest rate risk? Can you interpret its sign? 

(a) What does this spot rate dynamics imply?
(b) Obtain a PDE for a default-free discount bond price $B(t, T)$ un-

466 CHAPTER·20 Classical PDE Analysis for Interest Rate Derivatives 

(10) 

$^{1}$ For example, in dealing with American-style derivatives, it will in general be more convenient to work with numerical PDE methods, instead of evaluating the conditional expectations through Monte Carlo. 

where $\beta > 0$ represents a constant instantaneous discount rate, $g(\cdot)$ is some continuous payout that depends on the value assumed by the random process $x_{i}, E_{i}^{P}[\cdot]$ is the expectation under the probability $P$ and conditional on the information set $I_{i}$ , both of which are left unspecified at this point. The process $x_{i}$ obeys the SDE: 

Our discussion will begin with a simple example that is not directly useful to a market participant. But this will facilitate the understanding of the derivations. Also, we gradually complicate these examples and show how the methods discussed here can be utilized in practical derivatives pricing as well. 

In this section we establish a correspondence between a class of conditional expectations and PDEs. Using simple examples, we illustrate that starting with a function defined via a certain class of conditional expectations, we can always obtain a corresponding PDE satisfied by this function, as long as some nontrivial conditions are satisfied. The main condition necessary for such a correspondence to exist is Markovness of the processes under consideration. 

## 2 From Conditional Expectations to PDEs

Alternatively, a market practitioner can be given a PDE that he or she does not know how to solve. If the conditional expectation in (8) is shown to be a solution for this PDE, then this may yield a convenient way of “solving” for $F(S_{t}, t)$ . Again, the correspondence will be very useful. In this chapter we discuss the mechanics of obtaining such correspondences and the tools that are associated with them. 

$F(S_{t}, t)$ . If one could establish a PDE that corresponds to such expectations, this could give a faster, more accurate, or simply a more practical numerical method for obtaining the fair market price $F(S_{t}, t)$ of a financial derivative written on $S_{t}^{1}$ . 

2 From Conditional Expectations to PDEs 

But these conditional expectations are not always easy to evaluate. The stochastic behavior of $r_t$ can make this a very complex task indeed. Often, there is no closed-form solution and numerical methods need to be used. Even when such expectations can be evaluated numerically, speed and accuracy considerations may necessitate alternative methods. Thus, it may be quite useful to have an alternative representation that avoids the (direct) evaluation of conditional expectations in calculating the arbitrage-free price $F(S_t, t)$ . In particular, if we can obtain a PDE that corresponds to the conditional expectations (1) or (2), we can use numerical schemes to calculate 

under the risk-neutral measure. As a result, such conditional expectations arise naturally in derivative pricing. This is especially the case for inter-est rate derivatives, where the spot rate cannot be assumed constant, and hence, the discount factors will have to be random. 

$$
F (S _ {t}, t) = E _ {t} ^ {\bar {p}} \left[ e ^ {- \int_ {t} ^ {T} \tau_ {s} d s} F (S _ {T}, T) \right],
$$

Thus, the pricing effort went back and forth between PDE approaches and approaches that used conditional expectations. Yet, both of these methods are supposed to give the same arbitrage-free price $F(S_t, t)$ . This suggests that there may be some deeper correspondence between conditional expectations, such as in (1) or (2), and the PDEs that are shown in (3) or (5), respectively. 

Similarly, under the Black-Scholes assumptions with constant spot rate r, we earlier obtained the fundamental Black-Scholes PDE for a call option with strike price K and expiration T, written on $S_{i}$ : 

$^{3}$ Here the $F(x_{0})$ is the value of $F(\cdot)$ observed at time t = 0. It is conditional on $x_{0}$ . The $F(x_{\Delta})$ , on the other hand, is the value that will be observed after a time interval of length $\Delta$ at $t = \Delta$ . It will be conditional on $x_{\Delta}$ . 

The third term, on the other hand, involves the expectation of a stochastic differential and hence requires the application of Ito's Lemma. First, we approximate using Taylor series and write: 

As the last step, we take the limit as $\Delta \to 0$ of each term on the left-hand side. The second term is, in fact, a standard derivative of $e^{\beta x}$ evaluated at $x = 0$ : 

$$
\frac {1}{\Delta} E _ {0} ^ {P} \left[ \int_ {o} ^ {\Delta} e ^ {- \beta s} g (x _ {s}) d s + (e ^ {- \beta \Delta} - 1) F (x _ {\Delta}) + [ F (x _ {\Delta}) - F (x _ {o}) ] \right] = 0. \tag {18}
$$

$$
E _ {0} ^ {P} \left[ \int_ {o} ^ {\Delta} e ^ {- \beta s} g (x _ {s}) d s + e ^ {- \beta \Delta} F (x _ {\Delta}) - F (x _ {o}) \right] = 0.
$$

Grouping all terms on the right-hand side and moving them inside the expectation operator we obtain: 

$$
E _ {0} ^ {P} \left[ \int_ {\Delta} ^ {\infty} e ^ {- \beta s} g (x _ {s}) d s \right] = E _ {0} ^ {P} \left[ e ^ {- \beta \Delta} F (x _ {\Delta}) \right].
$$

But we can recognize the term inside the inner brackets on the right-hand side as the $F(x_{\Delta})$ and write: $^{3}$ 

$$
E _ {0} ^ {P} \left[ \int_ {\Delta} ^ {\infty} e ^ {- \beta s} g (x _ {s}) d s \right] = E _ {0} ^ {P} \left[ e ^ {- \beta \Delta} E _ {\Delta} ^ {P} \left[ \int_ {\Delta} ^ {\infty} e ^ {- \beta (s - \Delta)} g (x _ {s}) d s \right] \right].
$$

The third step will apply the recursive property of conditional expectations. As seen earlier, when conditional expectations are nested, it is the expectation with respect to the smaller information set that matters. Thus, if we have $I_{i} \subseteq I_{s}$ , we can write: 

$$
\left. E _ {0} ^ {P} \left[ \int_ {\Delta} ^ {\infty} e ^ {- \beta s} g (x _ {s}) d s \right] = E _ {0} ^ {P} \left[ e ^ {- \beta \Delta} \int_ {\Delta} ^ {\infty} e ^ {- \beta (s - \Delta)} g (x _ {s}) d s \right]. \right. \tag {12}
$$

The second step involves some elementary transformations that are intended to introduce a future value of $F(\cdot)$ to the right-hand side of this expression. In fact, note that the second term in the brackets can be rewritten after multiplying and dividing by $e^{-\beta \Delta}$ as: 

$$
F (x _ {0}) = E _ {0} ^ {P} \left[ \int_ {0} ^ {\Delta} e ^ {- \beta s} g (x _ {s}) d s + \int_ {\Delta} ^ {\infty} e ^ {- \beta s} g (x _ {s}) d s \right].
$$

point is given by $t = 0$ . First, consider a small time interval $0 < \Delta$ and split the period $[0, \infty)$ in two. One being the immediate future, represented by the interval $[0, \Delta]$ , and the other represented by $[\Delta, \infty)$ , easily be introduced. We now obtain a PDE that corresponds to expectation (9) in several steps. These steps are general and can be applied to more complicated expectations than the one in (9). We proceed in a mechanical way, to illustrate the derivation. To simplify the notation we assume that the initial point is given by $t = 0$ . 

$x_{s}$ . The discount factor $0 < \beta$ is deterministic. Clearly, the cash flows of interest in financial markets will, in general, be discounted by random discount factors. This is especially the case for interest rate derivatives, but we will leave this aside at the moment. All we want to accomplish at this point is to obtain a PDE that “corresponds” to the expectation in (9). We intend to study in detail the steps that will lead to this PDE. Once we learn how to do this, random discount factors can easily be introduced. 

This $F(x_{i})$ can be interpreted as the expected value of some discounted future cash flow $g(x_{i})$ that depends on an $I_{s}$ -measurable random variable $x_{s}$ . The discount factor $0 < \beta$ is deterministic. 

Second, try to introduce the future price of the bond, $B(t + \Delta, T)$ , in this expression. In fact, the second exponential on the right-hand side can easily be recognized as $B(t + \Delta, T)$ once we use the recursive property of conditional expectations. Using 

(26) 

$$
B (t, T) = E _ {t} ^ {\tilde {p}} \left[ \left(e ^ {- f _ {t} ^ {s + \Delta} r _ {s} d s}\right) \left(e ^ {- f _ {t - \Delta} ^ {s} r _ {s} d s}\right) \right].
$$

(24) 

Thus, we again have a conditional expectation and a process that is driving it, just as in the previous case. This means that we can apply the same steps used there and obtain a PDE that corresponds to $B(t, T)$ . Yet, in the present case, this PDE may also have some practical use in pricing bonds. It can be solved numerically, or if a closed-form solution exists, analytically.
The same steps will be applied in a mechanical way, without discussing the details. First, split the interval $[t, T]$ into two parts to write: 

Here the expectation is taken with respect to the risk-neutral measure $\bar{P}$ and with respect to the conditioning set available at time $t$ , namely the $I_{t}$ . This is assumed to include the current observation on the spot rate $r_{t}$ . If $r_{t}$ is a Markov process $B(t,T)$ will depend only on the latest observation of $r_{t}$ . Because we are in the risk-neutral world, as dictated by the use of $\bar{P}$ , the $r_{t}$ will follow the dynamics given by the SDE: 

$$
B (t, T) = E _ {t} ^ {\tilde {P}} \left[ e ^ {- \int_ {t} ^ {T} \tau_ {s} d s} \right],
$$

rate $r_{t}$ is a Markov process and write the price of the bond with par value 1, using the familiar formula: 

$^{4}$ In fact, note that in obtaining the PDE we replaced the Wiener component of the x, with 

We now see a more relevant example to the correspondence between a class of conditional expectations and PDEs. In fact, we now apply the same derivation to obtain a PDE for default-free pure discount bond prices. Consider the price $B(t,T)$ of a default-free pure discount bond with maturity T in a no-arbitrage setting. Assume that the instantaneous spot 

future behavior of $x$ . These constraints are to be given. More precisely, the function $F(x_{0})$ is the result of an optimal forecast. This optimal forecast requires projecting ways in which $F(x_{i})$ may change over time. Expected changes in the random variable $x_{i}$ , deterministic changes in the time variable $t$ , payouts $g(x_{i})$ , and the second order Ito correction all cause various predictable changes in $F(\cdot)$ . The optimal pre-diction should take these changes into account. The PDE that corresponds to the conditional expectation operators are obtained in such a way that the expected value of the prediction error is set equal to zero, and its variance is minimized, once these predictable changes are taken into consideration. 

the following.
The PDE corresponds to the expectation of the “present value” of cash flow stream $\{g(x_{i})\}$ . If this present value $F(\cdot)$ is given by the conditional expectation shown above, then it cannot be an arbitrary function of $x_{o}$ and its behavior over time must satisfy some constraints due to the expected future behavior of x. These constraints lead to the PDE. 

where the $F_{x}, F_{xx}, F$ , and g are all functions of x.
One may wonder what causes this correspondence between the conditional expectation (9) and this PDE? After all, these two concepts seemed to be quite unrelated at the outset. A heuristic answer to this question is the following. 

$$
\lim _ {\Delta \to 0} \frac {1}{\Delta} E _ {0} ^ {p} \left[ F (x _ {\Delta}) - F (x _ {o}) \right] = F _ {x} \mu + \frac {1}{2} F _ {x x} \sigma^ {2},
$$

where $\mu$ is the drift of the random process $x$ that enters the formula as a result of applying the expectation operator to $(x_{\Delta} - x_{o})$ . Replacing the limits obtained in (19)-(22) in expression (18), we reach the desired PDE: 

$E_{i}^{\bar{p}}\left[\int_{t}^{T}e^{-j_{1}u_{y}d_{s}}g(x_{u})du\right]=\int_{t}^{T}B_{u}E_{i}^{\rho}[g(x_{u})du],$ (38) assuming that the necessary interchange of the operators is allowed. On the other hand, equation (38) can always be applied if we used the forward measure as discussed in Chapter 17. 

$^{7}$ Here we cannot directly apply the $E_{t}^{p}[.]$ operator to $D_{u}$ because the $g(r_{u})$ will be correlated with the $D_{u}$ . If such correlation did not exist, and if $g(\cdot)$ depended on an independent random variable, say $x_{u}$ only, then we could take expectations separately and simply multiply the payout by the corresponding discount bond price $B_{u}$ to discount it: 

Various instruments and interest rate derivatives, such as coupon bonds, financial futures that are marked to market, and index-linked derivatives fall into this category where the arbitrage-free price will be given by conditional expectations such as in (36). Thus the methods that were discussed in the last two sections can be applied to find the implied PDE if the process(es) that drive these expectations are Markov. The corresponding PDEs may be exploited for real-life pricing of these complex instruments. 

(36) 

This $F(\cdot)$ would represent the price of an instrument that makes interest rate dependent payments at times $u \in [t, T]$ , and hence needs to be evaluated using the random discount factor $D_u$ at each $u$ : 

$$
F (r _ {i}, t) = E _ {i} ^ {\tilde {p}} \left[ \int_ {t} ^ {T} \left(e ^ {- \int_ {t} ^ {u} r _ {i} d s}\right) g (r _ {u}) d u \right].
$$

Clearly, one can combine these two basic examples to obtain the PDE that corresponds to instruments that make spot-rate dependent payouts $g(r_{t})$ and that need to be discounted by random discount factors: 

We have seen in detail two cases where the existence of a certain type of conditional expectation led to a corresponding PDE. In the first case there was a random cash flow stream depending on an underlying process $x_{t}$ , but the discount rate was constant. In the second case, the instrument paid a single, fixed cash flow at maturity, yet the discount factor was random. 

$^{6}$ Unlike the previous example, here the $B(t,T)$ function depends on t as well as on $r_{t}$ . Hence there will be an additional $B_{t}$ term that did not exist before. 

This is a PDE that must be satisfied by an arbitrage-free price of a pure discount bond with no-default risk. In Chapter 20, the same PDE was obtained using the method of risk-free portfolios. 

Note that this introduces the increment $[B(t+\Delta,T)-B(t,T)]$ to the left-hand side. This will be used for applying Ito's Lemma.
Fourth, take the limit as $\Delta\rightarrow0$ of the first term in this equation: $^{5}$ 

where all symbols are as in (42) and (43). One can in fact obtain the same PDE as in (34) by departing from this conditional expectation and using exactly the same steps as before. The only major difference will be at the stage when one calculates the limit corresponding to (33). There, one would substitute the real-world drift $a(r_{t}, t)$ instead of the risk-adjusted drift. 

(45) 

The main focus of this chapter is the correspondence between PDEs and conditional expectations. But, in passing, it may be appropriate to discuss an application of equivalent martingale measures to bond pricing.
The preceding section considered two bond pricing formulas. One used the martingale measure $\bar{P}$ and gave the compact expression: 

Hence, within the present context, while using Ito's Lemma, whenever a drift substitution for $dr_t$ is needed we have to use $(a(r_t, t) - \lambda_f b(r_t, t))$ and not $a(r_t, t)$ . This was the case, for example, in obtaining the limit in (33). Will the nonadjusted drift ever be used? The question is interesting because it teaches us something about pricing approaches that use other than the risk-neutral measure; formulas that, in principle, should give the same answer, but may nevertheless not be very practical. In other words, the question will show the power of the martingale approach. 

Indeed, during the same derivation, instead of using the risk-adjusted drift, we can indeed use the original drift of the spot-rate process. But this requires that the conditional expectation under consideration be evaluated using the real-world probability P, instead of the risk-neutral probability. However, we know that an expression such as 

cannot hold in general if the $B(t, T)$ is arbitrage-free, and if the expectation is taken with respect to real-world probability P. If one insists on using the real-world probability then the formula for the arbitrage-free price will instead be given by: 

we take the expectation with respect to $\hat{P}$ , the risk-neutral probability. Given that the random process under consideration is $r_{i}$ , this choice of risk-neutral probability requires that we use the risk-adjusted drift for $r_{i}$ and write the corresponding SDE as 

2.4.1 The Importance of Markovness
The derivation used here in obtaining the PDE that corresponds to the class of conditional expectations is valid only if the underlying stochastic processes are Markov. It may be worthwhile to see exactly where this assumption of Markovness was used in the preceding discussion. 

general.
Hence, we see that the assumption of Markovness plays a central role in the choice of pricing methods that one uses for interest rate derivatives. 

These operations are valid only when the $r_t$ process is Markov. If this assumption is not true, then the conditional expectations that we considered would depend on more than just the $r_t$ . In fact, past spot rates $\{r_s, s < t\}$ would also be determining factors of the price of the instrument. In other words, the latter price could no longer be written as $F(t, r_t)$ , a function that depended on $r_t$ and $t$ only. The rest of the derivation would not follow in general. 

$$
E ^ {\bar {p}} \left[ \int_ {t} ^ {T} e ^ {- f _ {t} ^ {u} r _ {s} d s} g (x _ {u}) d u | I _ {t} \right] = E ^ {\bar {p}} \left[ \int_ {t} ^ {T} e ^ {- f _ {t} ^ {u} r _ {s} d s} g (x _ {u}) d u | r _ {t} \right] \tag {39}
$$

In this section we investigate going in the opposite direction. Suppose we are given a PDE satisfied by an asset price $F(S_t, t)$ . Can we go from there to conditional expectations as a possible solution class? We discuss this within a special case. We let the $F(W_t, t)$ be the price of a financial derivative that is written on the Wiener process $W_t$ defined with 

Up to this point we showed that if the underlying processes are Markov and if some technical conditions are satisfied, then the arbitrage-free prices characterized as conditional expectations with respect to some appropriate measure would satisfy a PDE. That is, given a class of conditional expectations, we obtain a corresponding PDE. 

Thus, in one case, the integral contains the $\lambda_{i}$ but not the SDE. In the other case, the $\lambda_{i}$ is in the SDE but does not show up in the integral. But in Monte Carlo pricing, the market participant has to use both the integral and the SDE. That is why the approach outlined here is still the "classical" approach and requires, one way or another, modeling underlying drifts. The HJM approach avoids this difficulty. 

The appearances are unfortunately deceiving in this particular case. Whether one uses (46) or (54), as long as one stays within the boundaries of the classical approach, Monte Carlo pricing of bonds or other interest-sensitive securities would necessitate a calibration of $\lambda_{t}$ . In the case of (54) this is obvious, the $\lambda_{t}$ is in the pricing formula. In the case of (50), some numerical estimate of the $\lambda_{t}$ will also be needed in generating random paths for the $r_t$ through the corresponding SDE under the martingale probability $\tilde{P}$ : 

Expressions (46) and (54) give two different characterizations for $B(t,T)$ . But the second formula, derived with respect to real-world probability, seems to be messier because it is a function of $\lambda_t$ , whereas characterization (50) does not contain this variable. Hence one may be tempted to conclude that if one is utilizing Monte Carlo approach to calculate bond prices, or the prices of related derivatives, the formula in (50) is the one that should be used. It does not require the knowledge of $\lambda_t$ . 

$^{8}$ In this particular case, $\lambda_{i}$ will be the market price of spot interest rate risk. 

tailed earlier.
Thus, the connection between the two characterizations of default-free pure discount bond prices becomes very simple once the Girsanov theorem is utilized. Of course, in the above derivation, we did not show that the term $\lambda_{i}$ is the market price for interest rate risk. But it is clearly a drift adjustment to the interest rate stochastic differential equation. 

$$
E _ {t} ^ {P} \left[ e ^ {- \int_ {t} ^ {T} r _ {s} d s} \right] = \int_ {\Omega} \left(e ^ {- \int_ {t} ^ {T} r _ {s} d s}\right) e ^ {\int_ {0} ^ {T} [ \lambda_ {s} d W _ {s} ^ {*} - \frac {1}{2} \lambda_ {s} ^ {2} d s ]} d P
$$

where the $\Omega$ is the relevant range at which future $r_t$ will take values. Now, use the equivalence between $\tilde{P}$ and $P$ shown in (48) to substitute for $d\tilde{P}$ in this equation: 

$$
E _ {t} ^ {\tilde {p}} \left[ e ^ {- f _ {t} ^ {T} r _ {s} d s} \right] = \int_ {\Omega} \left(e ^ {- f _ {t} ^ {I} r _ {s} d s}\right) d \tilde {P},
$$

$$
B (t, T) = E _ {t} ^ {\hat {p}} \left[ e ^ {- f _ {t} ^ {T} r _ {s} d s} \right].
$$

where $\lambda_{i}$ is an $I_{i}$ -measurable process. $^{8}$ We now show how to get pricing formula (47) starting from (46), assuming that all technical conditions of Girsanov theorem are satisfied.
Start with the bond pricing equation: 

Characterized and calculated. The question that we touch on briefly here is how to go from one bond price formula to the other. This provides a good example of the use of Girsanov theorem. First, we remind the reader that within the context of Chapter 15, two probabilities $\tilde{P}$ and $P$ are equivalent if they are related by which is a characterization of the price $F(W_{t}, t)$ as a conditional expectation of the boundary condition $G(W_{T})$ and the probability $\tilde{P}$ . This function is also the solution of the heat equation. In fact, beginning with a 

$$
E _ {i} ^ {\tilde {p}} \left[ \int_ {t} ^ {T} \frac {\partial F}{\partial t} \frac {d W _ {s}}{d W _ {s}} \right],
$$

To show that this is the case, we invoke an important property of Ito integrals with respect to Wiener processes. From Chapter 10 we know that if $h(W_t)$ is a nonanticipative function with respect to an information set $I_t$ , and with respect to the probability $P$ , then the expectation of integrals with respect to $W_t$ will vanish: 

$$
E _ {t} ^ {\tilde {P}} \left[ \int_ {t} ^ {T} \frac {\partial F}{\partial W} d W _ {s} \right] = 0.
$$

Thus, if we can show that the second expectation on the right-hand side is zero, then the (unknown) function $F(\cdot)$ can be determined by taking the expectation of the known function $G(\cdot)$ . But this requires that: 

Now, $F(W_{T}, T)$ is the value of $F(\cdot)$ at the boundary t = T, so we can replace it by the known function $G(W_{T})$ . Doing this and rearranging: 

$$
\int_ {t} ^ {t} \left[ F _ {t} + \frac {1}{2} F _ {W W} \right] d s = 0.
$$

$$
F (W _ {T}, T) - F (W _ {t}, t) = \int_ {t} ^ {T} \frac {\partial F}{\partial W} d W _ {s} + \int_ {t} ^ {T} \left[ F _ {t} + \frac {1}{2} F _ {w w} \right] d s. \tag {59}
$$

$$
= \left[ F _ {t} + \frac {1}{2} F _ {W W} \right] d t + F _ {w} d W _ {t},
$$

$$
d F = \left[ \frac {\partial F}{\partial t} + \frac {1}{2} \frac {\partial^ {2} F}{\partial W ^ {2}} \right] d t + \frac {\partial F}{\partial W} d W _ {t}
$$

respect to probability. The choice of a $W_t$ as the driving process may not seem to be very realistic but it can easily be generalized. Further, it permits the use of a known PDE called the heat equation in engineering literature. Suppose this price $F(W_t, t)$ of the derivative was known to satisfy the following PDE: 

$^{10}$ Every expectation represents an average. By definition, averages are smoother than particular values. 

Some readers may wonder how we can define a rate of change for $f(S_{t})$ , which indirectly is a function of a Wiener process. A rate of change is like a derivative and we have shown that Wiener processes are not differentiable. So, how can we justify the existence of an operator such as A, one may ask. The answer to this question is simple. A does not deal with the actual rate of change in $f(S_{t})$ . Instead, A represents an expected rate of change. Although the Wiener process may be too erratic and nondifferentiable, note that expected changes in $f(S_{t})$ will be a smoother function and, under some conditions, a limit can be defined. $^{10}$ 

Here the small case letter $s_t$ indicates an already observed value for $S_t$ . The numerator of the expression on the right-hand side measures expected change in $f(S_t)$ . As we divide this by $\Delta$ , the $A$ operator becomes a rate of change. In the theory of stochastic processes $A$ is called the generator of the Ito diffusion $S_t$ . 

We may wonder how $f(S_t)$ may move starting from the current state $s_t$ . We define an operator to represent this movement. We let the operator $A$ be defined as the expected rate of change for $f(S_t)$ as: 

That is, future movements in $S_{t}$ , given what we observed until time t, are likely to be the same as starting the process at time t. In other words, the observations on $S_{t}$ from the distant past do not help to improve forecasts, given the $S_{t}$ . 

$dS_{t}=a(S_{t})dt+\sigma(S_{t})dW_{t},\quad t\in[0,\infty).$ (70)
Let $f(\cdot)$ be any bounded function, and suppose that the information set $I_{t}$ contains all $S_{u}, u \leq t$ until time t. Then we say that $S_{t}$ satisfies the Markov Property if: 

4 Generators, Feynman-Kac Formula, and Other Tools 

$^{9}$ In almost all cases of interest where there are no jumps involved, the SDEs utilized in practice are either of geometric, or of mean reverting type. The latter is especially popular with interest rate derivatives because the short rate is widely believed to have a mean reverting character. Under these conditions, the drift and diffusion parameters would be a function of $S_{i}$ only. However, often dependence on time is allowed to match the initial term structure. 

where the $a(\cdot)$ and $\sigma(\cdot)$ are the drift and diffusion parameters. Processes that have this characteristic are called time-homogenous Ito diffusions. The results below apply to those processes whose instantaneous drift and diffusion are not dependent on t directly. Usual conditions apply to $a(\cdot)$ and $\sigma(\cdot)$ , in that they are not supposed to vary “too fast.” We can discuss two properties of Ito diffusions. 

We now assume that the drift and diffusion parameters depend on $S_{t}$ only. $^{9}$ The SDE can be written as: 

Given the importance of the issues discussed above, it is not very surprising that the theory of stochastic processes developed some systematic tools and concepts to facilitate the treatment of similar problems. Many of these tools simplify the notation and make the derivations mechanical. This is the case with the notion of a generator, which is the formal equivalent of obtaining limits such as in (33), and the Feynman-Kac theorem, which gives the probabilistic solution for a class of PDEs. We complete this chapter by formalizing these concepts utilized implicitly during the earlier discussion. 

4 Generators, Feynman-Kac Formula, and Other Tools 

PDE involving an unknown function $F(t, W_{t})$ , we determined the solution as an expectation of a known function with respect to a probability, with respect to which $W_{t}$ is a Wiener process. 

where the term $(\sigma_{i}\sigma_{t}^{T})^{ij}$ represents the ijth element of the matrix $(\sigma_{i}\sigma_{t}^{T})$ . The difference between the univariate case and this multivariate formula is the existence of cross-product terms. Otherwise, the extension is immediate. 

$$
d f (S _ {i}) = \left[ a _ {i} \frac {\partial f}{\partial S} + \frac {1}{2} \sigma_ {i} ^ {2} \frac {\partial^ {2} f}{\partial S ^ {2}} \right] d t + \sigma_ {i} \frac {\partial f}{\partial S} d W _ {i}.
$$

First note that A is an expected rate of change in the limit. That is, we consider the immediate future with an infinitesimal change of time. Then, it is obvious that such a change would relate directly to Ito's Lemma. In fact, in the present case where $S_{i}$ is a univariate stochastic process: 

Several interesting cases using this correspondence are found in Kushner (1995). This source also gives practical ways of calculating the implied PDEs. 

The correspondence between PDEs and some conditional expectations is very useful in practical asset pricing. Given an instrument with special characteristics, a market practitioner can use this correspondence and derive the implied PDEs. These can then be numerically evaluated. 

$$
\hat {f} (t, r _ {i}) = E _ {i} ^ {P} \left[ e ^ {- f _ {i} ^ {u} q (r _ {i}) d s} f (r _ {u}) \right],
$$

The Feynman–Kac formula is an extension of Kolmogorov's backward equation as well as being a formalization of the issues discussed earlier in this chapter. The formula provides a probabilistic solution $\hat{f}$ that corresponds to a given PDE. 

be satisfied. According to this result, the conditional density function of a (generalized) Wiener process satisfies Kolmogorov's backward equation. This PDE tells us how the probability associated with a particular value of $S_{t}$ will evolve as time passes, given the initial point $S_0$ . 

It turns out that the conditional density $p(S_t, S_0, t)$ is one such function $f$ . To see this, take the first partial derivative with respect to $t$ and the second partial with respect to $S_t$ and substitute in (89). The equation will be satisfied. 

This result means that $\hat{f}(S^{-},t)$ is a solution for the PDE in (81). Hence, Kolmogorov's backward equation is an example of the correspondence between an expectation of a stochastic process and PDEs seen earlier in this chapter. 

$^{1}$ Additional assumptions concerning no dividend payments and constant interest rates were also assumed to get a closed-form formula for $F(\cdot)$ . 

At expiration, a call option holder could for example be paid: 

$t < t_{1} < t_{2} < \dots < t_{N} = T.$ 

The second category of options, although not dealt with extensively in this book, were those that were classified as path-dependent. The price of these options at time t depended not only on the current $S_{t}$ , but possibly on some or on all other values of $S_{t}$ observed before time t as well. An option's payoff at expiration time T could depend, for example, on the average of the last N values observed at discrete times: 

Given the observed value of $S_{t}$ and the time t, the option price was determined by the function $F(\cdot)$ . Plain-vanilla European options, where the $S_{t}$ was a geometric process, fell into this category. $^{1}$ 

Options considered in this book can be divided into two categories. The first group was characterized using a pricing equation that depended on the current value of the underlying assets $S_{t}$ and on the time t. For example, the price of a plain-vanilla call option at time t was written as: 

1 Introduction 

# Stopping Times and American-Type Securities

## CHAPTER 22

where the expectation is conditional on the current $r_{t}$ which is assumed to be known. 

$B(t,T) = E_{i}^{P}\left[e^{-\int_{i}^{T}r_{s}ds}e^{\int_{i}^{T}|\lambda(r_{s},s)dW - \frac{1}{2}\lambda(r_{s},s)^{2}ds|}\right],$ (96) 

(a) Let $B(t, T)$ be the bond price. Calculate the $d(BV)$ .
(b) Use the PDE in (93) to get an expression for $dB(t, T)$ .
(c) Integrate this expression from t to T and take expectations with respect to martingale equality to obtain the bond pricing formula: 

where $\lambda_{5}$ is the market price of interest rate risk. 

$V(u) = e^{-\int_{t}^{u}r_{s}ds}e^{\int_{t}^{u}[\lambda (r_{s},s)dW_{s} - \frac{1}{2}\lambda (r_{s},s)^{2}ds]},$ 

$B(T,T) = 1.$ 

There are other reasons for studying stopping times. Optimal stopping times are in general obtained by using the so-called dynamic programming approach. Dynamic programming is a useful tool in its own right and should be learned whether one is interested in pricing derivatives or not. It just happens that the context of stopping times is a very natural setting for presenting the main ideas of dynamic programming. 

which means “do not exercise.” By doing these calculations faster or more accurately, one can reduce costs and capture arbitrage opportunities better. Hence, the properties of algorithms used to determine stopping times will be an important part of the pricing effort. 

There are properties of optimal stopping times that make some approaches more convenient than others when it comes to pricing. By learning these properties we can reduce the time it takes to calculate whether, at a certain time $t^*$ , an option should be exercised or not. Or, in terms of the $\theta$ , whether one has: 

Even if the notion of stopping times was limited to the class of American-style securities, it would still be necessary to study stopping times. It is true that most financial derivatives are American-style and stopping times are necessary to price them. But there is more to stopping times than just American-style derivatives. We need to study stopping times not just because they are theoretical notions useful in theoretical formulas, but also because there are some very specific numerical algorithms that one needs to use in determining dates of early exercise. That is, we study stopping times because of numerical considerations as well. 

## 2 Why Study Stopping Times?

Such $\theta$ 's are called stopping times. When the date to exercise is chosen in some optimal fashion, they are called optimal stopping times and play a crucial role in pricing American-style securities. 

This means that the discounted value of the expected payoff may be less than what one gains by simply exercising the option at time $\theta$ . From this it should be clear that with American-style securities, the decision to exercise the option is equivalent to finding such critical time periods $\theta$ . Note that under these conditions, the pricing formula for the option may depend on the procedure used to select the $\theta$ 's, as well as on the previously discussed variables. 

$^{2}$ In fact, no closed-form formula may exist. $^{3}$ We always assume that the interest rates and volatility are constant. 

$[S_{\theta} - K] > E^{\hat{p}}\left[e^{(T - \theta)r}\max [S_T - K,0]\big|I_\theta\right].$ 

In fact, at some critical time $\theta$ , the expectation under the martingale measure $\tilde{P}$ of the future payoff $\max[S_{I}-K,0]$ may be less than what one may get if one exercised the option and received $S_{\theta}-K$ . That is, with constant spot rates, we may have: 

Now consider an American-style option. These securities can be exercised at or before the expiration date $T$ . Once the investor buys an American-style option he or she will have an additional decision to make. The time to exercise the option must now be chosen. The investor cannot just sit and wait until expiration. At some critical time denoted by $\theta$ , where $\theta \in [0, T]$ , it may be more profitable to exercise the (call) option and realize the gain, 

$P_{t}$ is correctly postulated. Notice that for neither of these two categories of options the investor has to make another decision once the option is purchased. In both cases, one waits until expiration and exercises the right to buy if it is profitable to do so. Alternatively, the option holder can close the position and sell the option to somebody else. But no other decision has to be taken. Hence, no other variable enters the formula. $^{3}$ 

Clearly, this expression will look somewhat more complicated for time $t, t < T^2$ . Yet, pricing this sort of exotic option is not necessarily more difficult than the case of plain-vanilla exotic options. In fact, according to what was said, the payoff of this option occurs at expiration date $T$ , and in this sense the option is still European. The only complications are the additional $S_t$ terms that show up in the expression. Thus, although the option is path-dependent, and the payoff depends on how one gets to an expiration value of the underlying asset, a Monte Carlo-type approach can give a reasonable approximation to $C_t$ once the dynamics of $S_t$ is correctly postulated. 

Under these conditions the time T price of this call option could be written using: 

(15) 

(16) 

With American-type securities, $\tau$ is in general random. $^{4}$ Consider an American-style call option $F(S_{t}, t)$ written on the underlying security $S_{t}$ , where $S_{t}$ follows a SDE: 

How can the stopping times, $\tau$ , be utilized in practice?
The most obvious use of $\tau$ is to let it denote the exercise date of an option. With European securities, there was no randomness in exercise dates.
The security could only be exercised at expiration. Hence, we can write: 

$^{4}$ In some special cases it is never worth exercising the American-style option, and the corresponding $\tau$ will again equal T. 

(3) 

(14) 

In case of derivative securities in general, we have a finite expiration period. So the options will either be exercised at a finite time, or will expire unexercised. This means that the second requirement that $\tau$ be finite with probability one is always satisfied. 

been exercised or not. In other words, given $I_{t}$ , we can differentiate between the possibilities: 

must take this into account. Thus, we let $\tau$ represent the early exercise date. It is obvious that given the information set, $I_{\nu}$ , we will be able to tell whether the option has already of the contract.
Hence, we are dealing with a “random date,” which is of great importance from the point of view of pricing the asset. In fact, the right to exercise early may have some additional value and pricing an American security must take this into account.
There, we let c represent the early exercise date. It is obvious that given 

That is, the outcome of the random variable is a particular time period. Now consider an American-style option written on a bond. The option can be exercised at any time between the present $t = 0$ and the expiration date denoted by $T$ . The option holder will exercise this option if he or she thinks that it is better to do so, rather than waiting until the expiration date of the contract. 

Stopping times are special type random variables that assume as outcomes random time periods, t. For example, let $\tau$ be a stopping time. Then this means two things. First, that $\tau$ is random, and second, that the range of its possible values is $[0, T]$ for some T > 0. When an outcome is observed, it will be in the form: 

during which the option holder can either be used. From the point of view of the "optimal stopping" perspective, the complications created by Bermudan options are very similar to American-style securities. The same introductory discussion of stopping times and the related tools will be sufficient for American as well as for Bermudan options. Hence, in the remainder of this chapter we work only with American options when dealing with stopping times. 

American-type derivative securities contain implicit or explicit options, which can be exercised before the expiration date if desired. This causes significant complications both at a theoretical level where one has to characterize the fair-market value of the security, and at a practical level where one has to calculate this price. 

one has to calculate this price. Bermudan-style options are a mixture of American and European options. They can be exercised at some prespecified times other than the expiration date. Yet, they cannot be exercised at all times during $[0, T]$ . At the date of issue the security specifies some specific dates $t_{1} < t_{2} < \cdots < t_{n} = T$ during which the option holder can exercise his or her option. 

$$
S _ {i} ^ {\mu} = S _ {i - 1} e ^ {i (r - \delta) - \frac {1}{2} \sigma^ {2}) \Delta + r \sqrt {\Delta}},
$$

$$
S _ {i} ^ {d} = S _ {i - 1} e ^ {((\mathrm{r} \delta) - \frac {1}{4} \sigma^ {2}) \Delta - \sigma \sqrt {\Delta}}.
$$

That is, once the process reaches a point $S_{i-1}$ , the next stage is either up, $S_i^u$ , or down, $S_i^d$ , with a probability equal to $P(u)$ or $P(d)$ . With this choice of discretization parameters the discretized system converges to the geometric process as $\Delta \to 0$ . That is, the drift and the diffusion parameters would be the same and the $S_i$ would follow the same trajectory as dictated for $S_i$ in the SDE (19). Note that the up and down parameters $u, d$ are constant and are given by: 

$$
P (u) = \frac {1}{2} + \frac {(r - \delta) - \frac {1}{2} \sigma^ {2}}{2 \sigma} \sqrt {\Delta},
$$

$$
S _ {i} ^ {d} = S _ {i - 1} e ^ {- \sigma \sqrt {\Delta}}.
$$

We let the $C_{t}$ denote the price of an American-style call option, with strike K and expiration date T, T < t that is written on $S_{t}$ . Suppose we decide to price this call using a binomial tree approach.
The methodology was discussed earlier, but is summarized here for convenience. We first choose the grid parameter $\Delta$ and discretize the $S_{t}$ in a standard way: $^{6}$ 

where r is the constant instantaneous spot rate and the $0 < \delta$ is a known dividend rate. The $W_{i}$ is a Weiner process with respect to risk-neutral measure $\tilde{P}$ . 

We continue studying stopping times and the problem of optimal stopping using the simplified setting of a binomial model for pricing a plain-vanilla American-style call option. Yet, although the setting is “simple” and our main purpose is the understanding of tools related to stopping times, the actual pricing of American-style options often proceeds within frameworks similar to the one considered here. Thus, the discussion below is useful from the point of view of some simple numerical pricing calculations as well. 

Option holder decides to exercise the can option. Hence, at time $t$ , we can calculate a spectrum of possible prices $F(S_{\tau}, t, \tau)$ indexed by $\tau$ using the possible values for the stopping time $\tau$ . To find the correct price we then pick the supremum among all these $F(S_{\tau}, t, \tau)$ . 

$$
F (S _ {t}, t) ^ {*} = \sup _ {\tau \in \Phi_ {t, T}} \left[ E _ {t} ^ {\tilde {P}} \left[ e ^ {- \tau (\tau - i)} F (S _ {\tau}, t, \tau) \right] \right],
$$

$$
F (S _ {t}, t) = E _ {t} ^ {\bar {p}} \left[ e ^ {- r (T - t)} \max \{S _ {T} - K, 0 \} \right],
$$

The price of the derivative security can again be expressed using the equivalent martingale measure $\tilde{P}$ . But this time there is an additional complication. The security holder does not have to wait until time $T$ to exercise the option. He or she will exercise the option as soon as it is more profitable to do so than wait until expiration. In other words, if one has to wait until expiration, the asset will be worth 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a1ccff69-6b24-4389-b2f8-232fb22b064b/3b06ec38b2e32eefc794eb0f1215af466549fddb35a290081cc520b38a91ad7e.jpg)


Initially, we are at point $S_{o}$ at the middle point. Next time $n = 1$ with probability .5, $S_{1}$ will move either to the left, to $S_{o}$ , or with probability .5 

In case of American options, we have the right to exercise early. And early exercise will naturally depend on the value of $S_{i}$ at the point that we find ourselves. Now consider the way the process behaves on the set $E$ as represented by the horizontal line in Figure 2. 

Now, although binomial trees are normally visualized over time as in Figure 1, for stopping time problems, one gains additional insights when the tree is visualized as a function of the value assumed by $S_{i}$ . These values are represented on the horizontal line shown in Figure 2. The line is none other than the representation of the set $E$ . The figure is the same as in Figure 1, except we look at it "sideways" from right to left. 

$E = \{u^5 S_o, u^4 S_o, u^3 S_o, u^2 S_o, u S_o, S_o, dS_o, d^2 S_o, d^3 S_o, d^4 S_o, d^5 S_o\}$ . (30) 

Instead of looking at the tree over time as in Figure 1, consider now Figure 2, where on the horizontal axis we mark all possible values assumed by $S_{i}$ during the move from $n = 0$ to $n = 5$ , the expiration. During this period, $S_{i}$ , can assume eleven possible values. Denoting this set by $E$ and using the condition $ud = 1$ we obtain: 

The standard way of looking at binomial trees is as shown in Figure 1, which horizontally mimicks the behavior of $S_i$ over "time." For analyzing stopping times and understanding the complications introduced by interim decisions on "stopping" or "continuing," it is worthwhile to look at the same tree from a different angle, literally. This may be a bit inconvenient at the beginning, but it greatly facilitates the understanding of some mathematical tools associated with stopping times. 

## 5 A Simplified Setting

that $S_{i}$ can follow: The call option's price will depend on the trajectory followed by $S_{i}$ . For European options, this was discussed in earlier chapters. It turns out that for the American-style options, there is a completely different way of looking at the same tree and seeing the dependence between the $S_{i}$ and $C_{n}$ , the price of the call option. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a1ccff69-6b24-4389-b2f8-232fb22b064b/39dc5551c71dfc3d4f9a08959ebd02aa30d32a710cf98213acddb2dfc542f7bf.jpg)


That is, the tree is recombining. The likely paths followed by the discretized $S_{i}$ are shown in Figure 1. It is worthwhile to look at the structure of the tree. The horizontal movement represents the path taken by $S_{i}$ over "time." The process begins from the initial point $S_{0}$ and then ends up at one of the six expiration states. During the times $i = 1,\dots ,5$ the $S_{i}$ can follow several trajectories. In fact, altogether there are $2^{n}$ possible trajectories, where $n$ is the number of "stages" given by $n = T\Delta$ . In this particular case, this gives 32 possible trajectories that $S_{i}$ can follow. 

## Also, we have, as usual,

It turns out that to make this choice, the investor has to calculate if he or she is likely to early exercise in the future as well. This means that before reaching a decision today, the investor must evaluate the odds of making the same decision in the future. It is only after analyzing possible future gains from the option that a decision to continue can be made. But a decision about early exercise possibilities in the future depends on the same assessment of the more distant future, and so on. At the end, the 

$^{9}$ According to this setup, the $F(\cdot)$ is an objective function. If such $F(\cdot)$ is assumed to be bounded, all technical conditions will be satisfied for the following steps. In practice, pricing algorithms assume this boundedness implicitly. 

Second, we need to find a rule to determine the optimal stopping time $\tau^{*}$ such that: 

According to this, we choose the r so that when we stop optimally, in the sense that the value of the option now is maximized. $^{9}$ Thus, we need to do two things. First we need to obtain the variable: 

We now discuss a simple, yet important example in order to understand some deeper issues associated with stopping time problems, as the one above. Recall the following problem faced by the holder of an American-style call. At any instant during the life of the option, the option holder has the right to early exercise. Hence, at all $t \in [0, T]$ a decision should be made concerning whether to exercise early or not. But this decision is much more complicated than it looks. 

where $B(k, S_{k})$ will be an optimal exercise boundary that depends on the k and on the current (and possibly past) values of $S_{k}$ . This boundary is to be determined. $^{10}$ 

$^{10}$ Let us see how we can interpret expectations such as $E^{p}[S_{i}]$ . Here one random variable is the $\tau$ . Hence possible values of the function $S_{i}$ need to be multiplied by the probability that $\tau = k$ among other things. There are other considerations, because even with $\tau$ fixed $S_{i}$ will still be random. On the other hand, in expectations such as $E^{p}[S_{i}]$ one would multiply possible values of $S_{i}$ by the probability that $S_{i}$ will assume these values. 

$^{8}$ In the terminology of Markov chains the two end points are called absorbent. That is, once we get there, with probability one we stay there. 

What we think when we say, in $\tau$ , is a measure. Now, if we can determine a strategy to choose the $\tau$ then we may be able to obtain the probabilities associated with the random variable $\tau$ as well. But if such a strategy is not defined, then the properties of $\tau$ will not be known and the $C(\cdot)$ will not be a well-defined random variable. Thus the first task is to determine a strategy to choose the $\tau$ . How is this to be done? Consider the following criterion, where the conditional expectation op-

and the decision to stop will be a function of this history. According to this, the decision to exercise early does not depend on the knowledge of which states will occur after stage i. The “future” after i is still unknown. This is what we mean when we say $\tau$ is $I_{i}$ -measurable. 

Then, obviously this decision will be made by looking at the trajectory followed by $S_{i}$ until the stage i. That is, we will have the observations: 

In contrast, if we decide otherwise, and continue, then we will be in possession of a security that is valued at the price $C(S_i)$ . Let us now consider the way an optimal decision to stop can be made. We let the $\tau$ represent the random time period at which we decide to exercise the option before expiration. At the initial point $i = 0$ the $\tau$ is random because whether we stop or not depends on the random trajectory followed by $S_i$ . 

of a Munkov Chain at stage v.
Now, remember that we can at any stage "stop" the experiment if we desire to do so. If we do this, we receive the payoff: 

will move to the right, to $uS_o$ . Once there, it can either come back to $S_o$ , or move one step further to the right or to the left. Hence, at each point, the process can only move to adjacent states. The major exceptions are the two end points. Once the process gets there, it must stop by necessity because it takes exactly 5 time periods to get to those points and that is the expiration of the option. This means that $S_i$ can also represent the position of a Markov Chain at stage $i$ . 

CHAPTER • 22 Stopping Times and American-Type Securities 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a1ccff69-6b24-4389-b2f8-232fb22b064b/5f2f5f612594af614829c9803da0385f059289328d85a66a8f6ee0c25fb28d01.jpg)


The problem faced by the decision maker is the following. Successive values of $S_{i}$ are observed and the corresponding $F(a_{j})$ are revealed. The decision maker evaluates the payoff of stopping immediately, against the expected payoff of continuing and ending up with a better $F(a_{j})$ in the future. How should this decision maker act? We discuss the optimal decision using Figure 3. 

This situation is shown in Figure 3. The horizontal axis represents the set E. The arrows indicate the possible moves and the corresponding probabilities. Note that if the process reaches the two end points it stays there. We need to introduce one more component to discuss the optimal stopping decisions in this context. When the $S_{i}$ visits a state, say, $a_{j}$ in E, the decision maker is given an option to receive a payoff $F(a_{j})$ . If the decision maker accepts this payoff, then the game stops. If the payoff is not accepted, the game continues and the $S_{i}$ moves to adjacent states. In Figure 3, the payoff associated with each state $a_{j} \in E$ is shown as the vertical line at the corresponding point. 

This implies that the process $S_{i}$ cannot jump across states and that it has to move to an adjacent state. Finally, for the initial stage, we also have: 

The next stage in describing these types of models is to state explicitly the relevant transition probabilities. According to the description above, the transition probabilities are given 

assume either the value a or the value $a_{7}$ .
2. Second, the states $a_{1}$ and $a_{10}$ are absorbent. If the process reaches those states it will stay there with probability one. These states can be reached only at “expiration.” 

The initial value $S_{0}$ is known to be a. The process is observed starting with i=1, is Markovian, and behaves according to the following assumptions. 

the same notation:
Suppose we observe successive values of a random variable $S_{i}, i = 1, \ldots, n$ . We let n = 5 and assume that there are eleven possible values that $S_{i}$ can take. These are given by the ordered set E: 

The simple example below is expected to shed some light on these questions. The reader will notice that the way the example is set is similar to the binomial tree model discussed in the previous section. In fact, we use the same notation. 

periods until expiration.
How should such decisions be made? Are there some mechanical rules that will help the decision maker to decide on the early exercise or not? Finally how can we gain some insights into such interrelated complex decisions?
The decision is expected to check some light on these ones 

American-option holder is left with a complex decision that spans all time periods until expiration. 

CHAPTER·22 Stopping Times and American-Type Securities 

Thus, by substituting for “future” $V(\cdot)$ in (48), we can eventually get to $V(\cdot)$ 's that are known to us. Then, the $V(a_{5})$ can be evaluated.
So how can we take this into account in (48)? We do so by writing, instead of acting as we did in (46) and taking into account only the immediate future. In other words we want to substitute the $V(a_{4})$ and $V(a)$ in place of $F(a_{4})$ and $F(a)$ in (46). This is the case because the latter does not take into account the possibility of reaching the higher future payoffs and then stopping there, whereas the $V(a_{4})$ and $V(a)$ do. In other words the $V(a_{4})$ and $V(a)$ incorporate the idea that the decision will be made optimally in the future. This way of reasoning is very similar to pricing derivatives by going “backwards” in a binomial tree. When this is done it will be clear that we should continue at $a_{3}$ but stop at $a_{5}$ . Note that the expectation on the left-hand side of (51) is different from (46) since it is now conditional on the fact that we stop optimally. Hence, it is in fact $V(a_{5})$ . A final comment on the example. We should point out an interesting occurrence in Figure 3. The points at which we end up stopping are those 

Although the reasoning seems circular it really is not. The problem is set up in a way that there are some stages where calculation of the $V(a_{i})$ is immediate. For example, as we already know that we will stop when we reach $a_{1}$ or $a_{7}$ ; 

Note that this assumption assumes no discounting. Thus, before we can calculate $V(a_{5})$ we need to determine the $V(a_{4})$ and the $V(a)$ . But, there is the same problem with these. The $V(\cdot)$ that corresponds to future states seems to be unknown. 

$$
V (a _ {5}) = \max \left[ F (a _ {5}), \left[ \frac {1}{2} V (a _ {4}) + \frac {1}{2} V (a) \right] \right].
$$

Here the expected payoff if we stop is known. It is the $F(a_{5})$ . On the other hand, the expected payoff if we continue is unknown. It should be calculated by using the same notion as $V(a_{5})$ for future periods in an optimal fashion. In other words, we need to write: 

current payoff if we stop, or the expected payoff if we decide to continue, assuming that we continue in an optimal fashion. That is, we want: 

This is clearly worse than the 8 we can guarantee by stopping now. But there is an additional point. The game does not end at the next stage and looking only at the immediate future would ignore the expected payoff that would result if we reached the state $a_7$ . What we would like to do is to obtain an optimal payoff function denoted by, say, $V(a_5)$ that represents the greater of two payoffs; namely, the 

We are not going to do any better by continuing. Thus far, the decision to stop was not complicated at all. But now consider the two states $a_3$ and $a_5$ . Here the decisions will be more complicated. Both of these states have the following property. The payoff is a local maximum. If we continue after reaching them, we go to adjacent states and these states have lower payoffs. The decision maker will be worse off at least in the immediate future. But by not stopping, one is also keeping the possibility of reaching a payoff such as $F(a_7)$ or $F(a_5)$ open. So which one is better? Should one accept the local maxima such as $F(a_5)$ or $F(a_5)$ and stop, or should one continue at these points and expect to stop at a future date when there is a higher payoff? 

do better. We should not stop.
Another obvious decision occurs at state $a_{7}$ . This state is associated with the highest payoff ever, and we should clearly stop as soon as we reach it.
We are not going to do any better by continuing. 

states.
Next consider the state $a_{8}$ . Should we stop once we have $S_{i}=a_{8}$ , and accept the offered payoff $F(a_{8})$ ? The answer is, obviously, no (unless, of course, n=5 and we have to stop). It is clear that the next move of $S_{i}$ will be to either $a_{7}$ or to $a_{9}$ . As can be seen from Figure 3, either of these states has a payoff higher than $F(a_{8})$ . By continuing, we are guaranteed to do better. We should not stop. 

Note that at each stage we know where we are. In other words, we observe the current value of $S_{i}$ . But, we do not know the future outcomes, even though we do know the possibilities. Consider these possibilities. 

1. A player confronts the following situation. A coin will be tossed at every time $t, t = 1, 2, 3, \ldots, T$ and the player will get a total reward $W_t$ . He or she can either decide to stop or to continue to play. If he or she continues, a new coin will be tossed at time $t + 1$ , and so on. The question is, what is the best time to stop? We consider several cases. We begin with the double-or-nothing game. The total reward received at time $t = T$ is given by: 

There are three important topics in this chapter. First there is the issue of stopping times. The early exercise is an optimal stopping problem. We can recommend Dynkin et al. (1999). This treatment is classic but still very intuitive. A reader interested in learning more about classical stopping time problems can read the book by Shirayev (1978). The second major topic that we mentioned is dynamic programming although this was a side issue for us. There are many excellent texts dealing with dynamic programming. Finally there is the issue of numerical calculation of stopping times. Here the reader can go to references given in Broadie and Glasserman (1998). 

## 9 References

The chapter also introduced the notion of stopping times. This concept was useful in pricing American-style derivative products and in dynamic programming. We also illustrated the close relationship between binomial tree models and a certain class of Markov chains. 

This expression is called Dynkin's formula. It gives a convenient representation for the expectation of a function that depends on a stopping time. The operator A is as usual the generator. 

This property is clearly important in writing asset prices using equivalent martingale measures. The fact that the exercise date of a derivative is random does not preclude the use of equivalent martingale measures. With random $\tau$ , randomly stopped asset prices will still be martingales under the probability $P$ . 

We finish this chapter by looking at the role played by stopping times in the theory of martingales. It turns out that most of the results discussed in this book can be extended to stopping times. Below we simply give two such results without commenting extensively on them. 

times when the payoff from the state is on a boundary that we denote as the envelope in Figure 3. Thus, if a market practitioner is given this envelope, then the rule to pick optimal stopping times will be greatly simplified. All one has to do is to see whether the payoff is below the envelope or on it. One stops if the current payoff equals the value of the envelope at that point, and continues otherwise. Essentially, this is what is meant by Equation (37), which gives an optimal stopping rule. 

The environment imposes the following constraint on this policy maker: 

(b) How does this compare with $W_{T}$ ? Should the player then “stop”?
(c) But if the player never stops when he or she is in a winning streak,
how long would the player continue playing the game?
(d) What is the probability that $z_{t} = -1$ at some point?
(e) How do you explain this puzzle? 

$E[W_{T+1} \mid W_T = w_T^*] = 2^{T+1} \frac{T+1}{T+2}.$ 

(a) Show that the conditional expected reward as we just play one more time is: 

2. Consider the problem above again. Suppose we tossed a coin T times and the resulting $z_{t}$ were all +1. The reward will be: 

(d) What is the maximum value this reward can reach?
(e) Is there an optimal stopping rule? 

(b) What is the best time to stop this game?
(c) Suppose now we sweeten the reward at every stage and we multiply the $W_{T}$ by a number that increases and is greater than one.
In fact suppose the reward is now given by: 

(a) Can you calculate the expected reward at time T, $E[W_{T}]$ , given this information? 

where the $z_{t}$ is a binomial random variable: 

Dellacherie, C., and Meyer, P. Theorie des Maringales. Hermann, Paris, 1980. 

Das, S. Swap and Derivative Financing, Revised Edition. Probus, 1994.
Dattatreya, R. E., Venkatesh, R. S., and Venkatesh, V. E. Interest Rate and Currency Swors. Probus, Chicago, 1994. 

Cox, J., and Rubinstein, M. Options Markets. Prentice-Hall, New York, 1985.
Cox, J. C., Ingersoll, J. E., and Ross, S. "An Intertemporal Asset Pricing Model with 

Brennan, M. J., and Schwarz, E. S. "A Continuous Time Approach to Pricing of Bonds," Journal of Banking and Finance, 3, 135–155, 1979. 

Bremaud, P. Bremaud (1979) p. 181. Point Processes and Queues, Martingale Dy 

Brace, A., Gatarek, D. and Musiela, M. "The Market Model of Interest Rate Dy 

nal of Political Economy, 81, 637–654, 1973.
Black, E., Derman, E., and Troy, W. "A One-Factor Model of Interest Rates and Its Application to Treasury Bond Options," Financial Analysis Journal, 46, 33–39, 1990 

Bjork, T. Arbitrage Theory in Continuous Time. Oxford University Press, 1999.
Black, F., and Scholes, M. "The Pricing of Options and Corporate Liabilities," Jour-

Bhattacharya, S., and Constantinides, G. Theory of Valuation. Rowmand and Lit-

## BIBLIOGRAPHY

(d) Determine the value function $V_{t}$ that gives the optimal payoff for $t=1,2,3,4.$ (e) Plot the value function $V_{t}$ and interpret it. 

(a) What is the best choice of $k_{t}$ for period $t = 4$ ?  
(b) What is the best choice of $k_{t}$ for period $t = 3$ ?  
(c) From these, can you iterate and find the best choice of $k_{t}$ for 