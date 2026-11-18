

<!-- === Source: MinerU_markdown_Financial_Mathematics_1_2122707655893032961.md (Page 1) === -->

# KING’S COLLEGE LONDON DEPARTMENT OF MATHEMATICS

Financial Mathematics An Introduction to Derivatives Pricing 

Lane P. Hughston Christopher J. Hunter 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/e9ace21bf1404cdb565976fd1b9d561f521220c6d8bac03f2a6b6ded701e1267.jpg)


# Financial Mathematics An Introductory Guide

Lane P. Hughston<sup>1</sup> 

Department of Mathematics King’s College London The Strand, London WC2R 2LS, UK 

Christopher J. Hunter<sup>2</sup> 

NatWest Group 135 Bishopsgate, London Postal Code, UK 

and 

Department of Mathematics King’s College London The Strand, London WC2R 2LS, UK 

copyright c 2000 L.P. Hughston and C.J. Hunter 

## Preface

This book is intended as a guide to some elements of the mathematics of finance. Had we been a bit bolder it would have been entitled ‘Mathematics for Money Makers’ since it deals with derivatives, one of the most notorious ways to make (or lose) a lot of money. Our main goal in the book is to develop the basics of the theory of derivative pricing, as derived from the so-called ‘no arbitrage condition’. In doing so, we also introduce a number of mathematical tools that are of interest in their own right. At the end of it all, while you may not be a millionaire, you should understand how to avoid ‘breaking the bank’ with a few bad trades. In order to motivate the study of derivatives, we begin the book with a discussion of the financial markets, the instruments that are traded on them and how arbitrage opportunities can occur if derivatives are mispriced. We then arrive at a problem that inevitably arises when dealing with physical systems such as the financial markets: how to deal with the ‘flow of time’. There are two primary means of parametrizing time—the discrete time parameterization, where time advances in finite steps; and the continuous time parameterization, where time varies smoothly. We initially choose the former method, and develop a simple discrete time model for the movements of asset prices and their associated derivatives. It is based on an idealised Casino, where betting on the random outcome of a coin toss replaces the buying and selling of an asset. Once we have seen the basic ideas in this context, we then expand the model and interpret it in a language that brings out the analogy with a stock market. This is the binomial model for a stock market, where time is discrete and stock prices move in a random fashion. In the second half of the notes, we make the transition from discrete to continuous time models, and derive the famous Black-Scholes formula for option pricing, as well as a number of interesting extensions of this result. Throughout the book we emphasise the use of modern probabilistic methods and stress the novel financial ideas that arise alongside the mathematical innovations. Some more advanced topics are covered in the final sections— stocks which pay dividends, multi-asset models and one of the great simpli fications of derivative pricing, the Girsanov transformation. This book ia based on a series of lectures given by L.P. Hughston at King’s College London in 1997. The material in appendix D was provided by Professor R.F. Streater, whom we thank for numerous helpful observations on the structure and layout of the material in these notes. 

For lack of any better, yet still grammatically correct alternative, we will use ‘he’ and ‘his’ in a gender non-specific way. In a similar fashion, we will use ‘dollar’ in a currency non-specific way. 

L.P. Hughston and C.J. Hunter January 1999 

## Contents

1 Introduction 1
1.1 Financial Markets . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
1.1.1 Basic Assets . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
1.1.2 Derivatives . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
1.2 Uses of Derivatives . . . . . . . . . . . . . . . . . . 8
1.3 Derivative Payoff Functions .. 9
2 Arbitrage Pricing 13
2.1 Expectation Pricing .. 13
2.2 Arbitrage Pricing .. 14
2.3 Trading Strategies .. 17
2.4 Replication Strategy .. 20
2.5 Currency Swap .. 20
2.6 Summary .. 23
3 A Simple Casino 24
3.1 Rules of the Casino .. 24
3.2 Derivatives .. 25
3.3 No Arbitrage Argument .. 26
4 Probability Systems 29
4.1 Sample Space .. 29
4.2 Event Space .. 29
4.3 Probability Measure .. 31
4.4 Random Variables .. 32
5 Back to the Casino 35
5.1 The Casino as a Probability System .. 35
5.2 The Risk-Neutral Measure .. 35
5.3 A Non-Zero Interest Rate .. 37
6 The Binomial Model 41
6.1 Tree Models .. 41
6.2 Money Market Account .. 43
6.3 Derivatives .. 44
6.4 One-Period Replication Model .. 45
6.5 Risk-Neutral Probabilities .. 47 

7 Pricing in N-Period Tree Models 50   
8 Martingales and Conditional Expectation 54   
8.1 Stochastic Processes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .   
8.2 Filtration . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 54   
8.3 Adapted Process. 56   
8.4 Conditional Expectation. 56   
8.5 Martingales. 58   
8.6 Financial Interpretation. 58   
9 Binomial Lattice Model 60   
10 Relation to Binomial Model 63   
10.1 Limit of a Random Walk. 63   
10.2 Martingales associated with Random Walks. 64   
11 Continuous Time Models 68   
11.1 The Wiener Model. 68   
11.2 The Normal Distribution. 69   
12 Stochastic Calculus 76   
13 Arbitrage Argument 79   
13.1 Derivation of the No-Arbitrage Condition. 79   
13.2 Derivation of the Black-Scholes Equation. 83   
14 Replication Portfolios 86   
15 Solving the Black-Scholes Equation 89   
15.1 Solution of the Heat Equation. 90   
15.2 Reduction of the Black-Scholes Equation to the Heat Equation 92   
16 Call and Put Option Prices 97   
16.1 Call Option. 97   
16.2 Put Option. 101   
17 More Topics in Option Pricing 104   
17.1 Binary Options. 104   
17.2 'Greeks' and Hedging. 105 

17.3 Put-Call Parity . . . . . . . . . . . . . . . . . . . . . . . . . 107   
18 Continuous Dividend Model 109   
18.1 Modified Black-Scholes Equation . . . . . . . . . . . . . . . . . . 112   
18.2 Call and Put Option Prices . . . . . . . . . . . . . . . . . . 113   
19 Risk Neutral Valuation 115   
19.1 Single Asset Case . . . . . . . . . . . . . . . 115   
20 Girsanov Transformation 121   
20.1 Change of Drift . . . . . . . . . . . . 122   
21 Multiple Asset Models 126   
21.1 The Basic Model . . . . . . . . . . 126   
21.2 No Arbitrage and the Zero Volatility Portfolio 129   
21.3 Market Completeness . . . . . . . . 131   
22 Multiple Asset Models Continued 132   
22.1 Dividends 132   
22.2 Martingales and the Risk-Neutral Measure 133   
22.3 Derivatives 135   
A Glossary 137   
B Some useful formulae and definitions 140   
B.1 Definitions of a Normal Variable 140   
B.2 Moments of the Standard Normal Distribution 140   
B.3 Moments of a Normal Distribution 141   
B.4 Other Useful Integrals 141   
B.5 Ito's Lemma 141   
B.6 Geometric Brownian Motion 142   
B.7 Black-Scholes Formulae 142   
B.8 Bernoulli Distribution 143   
B.9 Binomial Distribution 143   
B.10 Central Limit Theorem 143   
C Solutions 145 

D Some Reminders of Probability Theory 194
D.1 Events, random variables and distributions ..... 194
D.2 Expectation, moments and generating functions ..... 195
D.3 Several random variables ..... 196
D.4 Conditional probability and expectation ..... 199
D.5 Filtrations and martingales ..... 204

E The Virtues and Vices of Options $^{1}$ 207

F KCL 1998 Exam 209
F.1 Question ..... 209
F.1.1 Solution ..... 210
F.2 Question ..... 212
F.2.1 Solution ..... 213
F.3 Question ..... 215
F.3.1 Solution ..... 216
F.4 Question ..... 218
F.4.1 Solution ..... 219
F.5 Question ..... 221
F.5.1 Solution ..... 222
F.6 Question ..... 223
F.6.1 Solution ..... 224

G Bibliography 225 

## 1 Introduction

The study of most sciences can be usefully divided into two distinct but interrelated branches, theory and experiment. For example, the body of knowledge that we conventionally label ‘physics’ consists of theoretical physics, where we develop mathematical models and theories to describe how nature behaves, and experimental physics, where we actually test and probe nature to see how it behaves. There is an important interplay between the two branches—for example, theory might develop a model which is then tested by experiment, or experiment might measure or discover a fact or feature of nature which must then be explained by theory. 

Finance is the science of the financial markets. Correspondingly, it has an important ‘theoretical’ side, called finance theory or mathematical finance, which entails both the development of the conceptual apparatus needed for an intellectually sound understanding of the behaviour of the financial markets, as well as the development of mathematical techniques and models useful in finance; and an ‘experimental’ side, which we might call practical or applied finance, that consists of the extensive range of trading techniques and risk management practices as they are actually carried out in the various financial markets, and applied by governments, corporations and individuals in their quest to improve their fortune and control their exposure to potentially adverse circumstances. 

In this book we ofer an introductory guide to mathematical finance, with particular emphasis on a topic of great interest and the source of numerous applications: namely, the pricing of derivatives. The mathematics needed for a proper understanding of this significant branch of theoretical and applied finance is both fascinating and important in its own right. Before we can begin building up the necessary mathematical tools for analysing derivatives, however, we need to know what derivatives are and what they are used for. But this requires some knowledge of the so-called ‘underlying assets’ on which these derivatives are based. So we begin this book by discussing the financial markets and the various instruments that are traded on them. Our intention here is not, of course, to make a comprehensive survey of these markets, but to sketch lightly the relevant notions and introduce some useful terminology. Unless otherwise stated, all dates in this section are from the year 1999, and all prices are the relevant markets’ closing values. If no date is given for a price, then it can be assumed to be January 11, 1999. 

## 1.1 Financial Markets

The global financial markets collectively comprise a massive industry spread over the entire world, with substantial volumes of buying and selling occurring in one market or another at one place or another at virtually any time. The dealing is mediated by traders who carry out trades on behalf of both their clients (institutional and individual investors) and their employers (investment banks and other financial institutions). This world-wide menagerie of traders, in the end, determines the prices of the available financial products, and is sometimes collectively referred to as the ‘market’. The most ‘elementary’ financial instruments bought and sold in financial markets can be described as basic assets. There are several common types. 

## 1.1.1 Basic Assets

A stock or share represents a part ownership of a company, typically on a limited liability basis (that is, if the company fails, then the shareholder’s loss is usually limited to his original investment). When the company is profitable, the owner of the stock benefits from time to time by receiving a dividend, which is typically a cash payment. The shareholder may also realize a profit or capital gain if the value of the stock increases. Ultimately, the share price is determined by the market according to the level of confidence of investors that the firm will be profitable, and hence pay further and perhaps higher dividends in the future. For example, the value of a Rolls-Royce share at the close of the London Stock Exchange on January 11 was 248.5p (pence), which was down 0.5p from the prior day’s closing value. In the previous 52 weeks the highest closing value was 309p, while the lowest was 176.5p. The company has declared a dividend of 6.15p per share for 1998 compared with 5.9p and 5.3p per share paid in the two years previous to that. 

A bond is, in efect, a loan made to a company or government by the bondholder, usually for a fixed period of time, for which the bond-holder receives a fee, known as interest. The interest rate charged is typically fixed at the time that the loan is made, but might be allowed to vary in time according to market levels and certain prescribed rules. The interest payments, which are typically made on an annual, semi-annual or quarterly basis, are called ‘coupon’ payments. If a 10-year bond with a ‘face-value’ of $1000 has a 6% annual coupon, that means that an interest rate payment of $60 is made every year for ten years, and then at the end of the ten year period the $1000 ‘principal’ is paid back to the bond-holder. Bonds are, in some respects, a more conservative investment than stocks, since they provide a more or less guaranteed or ‘fixed’ income. Hence the bond market is sometimes called the ‘fixed-income’ market. However, if the company or government issuing the bonds defaults, and cannot or will not pay back the loan, or part of the loan, then the bond-holder may lose his shirt. The likelihood that a borrower will default on any part of the loan is described by the credit quality of the borrower. There are several credit rating agencies, for example Standard & Poor’s (S&P) and Moody’s, which assign a rating to many companies and governments. The rating systems vary between the agencies, but given two ratings it is generally possible to decipher which one is better by following some simple rules—A’s are better than B’s, which are better than C’s, and so on; and more letters are better than less so, AAA is better than A. For example, on our fiducial date, January 11, a bond previously issued by Wal Mart, an American retail company that has an S&P credit rating of AA, with a maturity date of May 2002, a face-value of $100 and a coupon of $6.75 cost $105.02. By contrast, a Croatian government bond with a credit rating of BBB-, a maturity date of February 2002, a face-value of $100, and a coupon of $7.00 cost $93.21. Given the similar values of maturity and coupon, the diference in price between the bonds is due to the superior credit rating of Wal Mart (AA) over the Croatian government (BBB-). If the credit quality of the borrower declines, then the price of a bond issued by the borrower will also decline. Similarly, if interest rates generally rise, then bond prices will fall. In either case, the purchaser of a bond may find that it is worth less that what it was previously, despite the fixed income that it provides. 

Exercise 1.1 Why does the value of a bond drop if interest rates go up? Why does the value of a bond rise if credit quality improves? 

When money is put on deposit with a bank or other financial institution on an ‘overnight’ basis, i.e., where withdrawal on short notice is available, then the depositor is essentially making a very short term loan to the financial institution. The instantaneous (i.e., ‘overnight’) rate of interest paid on this loan is called a money market rate, or ‘short term interest rate’. Money market accounts can be very nearly ‘risk-free’, in the sense that depositors can get their money back on short notice, if required, and the balance in the account always goes up. As an example, a private client with an account balance of more than £1,000,000 in a money market account with the Royal Bank of Scotland would receive an interest rate of 6.1% per year. 

Exercise 1.2 Consider the money market account mentioned above. Suppose that the interest earned every month is added to the account at the end of the month. What is the actual annual interest rate that is earned? 

Exercise 1.3 Let $B _ { t }$ be the amount in a money market account at time t. Suppose that there is interest paid on the money in the account at a constant rate r, that is, in a short time period dt, the interest that is paid is $r B _ { t } d t$ Derive and solve the diferential equation for $B _ { t }$ 

Commodities are physical objects, typically natural resources or foods such as oil, gold, copper, cattle or wheat. There are often additional complications associated with commodities, for example, holding costs for the storage and insurance of goods and delivery costs to move them about. These costs are representative of the intricate details that can arise in practical finance. 

The concept of a domestic or foreign currency is, in reality, a fairly abstract idea, but certainly includes the conventional ‘money’ issued by the various countries of the world. The value of a currency, in units of other currencies, depends on a number of factors, such as interest rates in that country, the nation’s foreign trade surplus, the stability of the government, employment levels, inflation, and so on. The exchange rate for immediate delivery of a currency is called the spot exchange rate. This is the one kind of financial asset that almost everyone has had some experience with, and you will be familiar with the fact that the value (say in units of your own ‘domestic’ currency) of a unit of ‘foreign’ currency can go up or down. Sometimes these swings can be substantial, even over limited time horizons. Currencies are very actively traded on a large scale in international over-the-counter markets (that is, by telephone and electronic means). Some currency prices are quoted to several decimal points in the professional markets. For example, a typical ‘bid/ofer’ spread for the price of sterling in U.S. dollars might be 1.6558/1.6568. This means that the trader is willing to buy one pound for 1.6558 dollars, and is willing to sell one pound for 1.6568 dollars. Traders use fanciful nicknames for various rates, for example, the U.S. dollar/French franc rate is called ‘dollar/Paris’, while the Canadian dollar/Swiss franc rate is called ‘Candollar/Swiss’. The dollar/sterling rate is so important historically that it has a special name: ‘Cable’. 

## 1.1.2 Derivatives

In addition to the basic assets that we have just described, another important component of the financial markets are derivatives, which are in essence ‘sidebets’ based on the behaviour of the ‘underlying’ basic assets. A derivative can also be regarded as a kind of asset, the ownership of which entitles the holder to receive from the seller a cash payment or possibly a series of cash payments at some point in the future, depending in some pre-specified way on the behaviour of the underlying assets over the relevant time interval. In some instances, instead of a ‘cash’ payment another asset might be delivered instead. For example, a basic stock option allows the holder to purchase shares at some point in the future for a pre-specified price. 

Derivatives, unlike the underlying assets, are in many cases directly synthesized by investment banks and other financial institutions. They can either be ‘tailor-made’ and sold directly to a specific client, or, if they are general enough, they can be traded in a financial market, just like the underlying assets. The range of possible derivatives is essentially unlimited. However there are a number of standard examples and types of derivatives that one should be familiar with and which we shall mention briefly below. 

The most common types of derivatives are the so-called options. An option is a derivative with a specified payof function that can depend on the prices of one or more underlying assets. It will have specific dates when it can be exercised, that is, when the owner of the option can demand payment, based on the value of the payof function. However, you are never forced to ‘exercise the option’. Most options can only be exercised once, and have a fixed expiration date, after which the option is no longer valid. There are many diferent schemes for prescribing when an option can be exercised. The most common examples are the so-called European options, which can only be exercised on the expiration date, and American options, which can be exercised at any time up to the expiration date. In this book, we shall be concerned primarily with European derivatives, since they are mathematically much simpler, although the formalism that we build up is certainly capable of handling the American case as well. 

Exercise 1.4 What is the most money that you can lose by buying an option? Why? 

The two most common options are the call option, which gives the owner the right to buy a designated underlying asset at a set price (called the strike price), and the put option which allows the owner to sell the underlying asset at a given strike price. In London, organised derivatives trading takes place at the London International Financial Futures and Options Exchange (LIFFE). Among others, American call and put options on about 75 stocks U.K. stocks are traded at LIFFE. For example, a call option on Rolls-Royce with a strike of 240p and an expiry date of February 17, costs 19p per share, whereas a put with the same strike and maturity costs 9.5p per share (recall that the share price was 248.5p). In appendix E, an article from the May 2, 1885 Economist is reproduced. It contains a description of call and put options that has not really changed much in the intervening century. We shall give a fairly thorough treatment of the pricing of options in the sections that follow. Note that there are options not only on underlying assets, but also on other derivatives. For example, an option to enter into a swap is called a ‘swaption’ (swaps are defined below). 

An index is a number derived from a set of underlying assets (it generally is a weighted sum or average of the underlying asset prices). The most common underlying assets to use are stocks, but there are also indices based on bonds and commodities. As examples, The Financial Times-Stock Exchange 100 (FT-SE 100) index and the Dow Jones Industrial Average (DJIA) are indices that take their values from share prices on the London and New York exchanges respectively. 

How is the FT-SE 100 index calculated? Well, the calculation uses the 100 largest companies by market capitalisation (share price times the number of shares) on the London Stock Exchange. The index is simply the sum of the market capitalisations of the 100 firms divided by an overall normalising factor. This normalising factor was fixed at the inception of the index and is only altered to ensure continuity of the index when the market capitalisation of a firm used in the index calculation changes in a discontinuous way. This can happen when new shares are issued by the firm or when it is removed from the index calculation altogether and replaced by a new, larger firm. The value of the FT-SE 100 index on January 11 was 6085.00. 

In contrast, the DJIA was originally based on the unweighted average of 30 ‘industrial’ companies on the New York Stock Exchange that were chosen to span the manufacturing sector. Over the years two things have happened—the definition of industrial has been widened and the index now includes, for example, companies from the entertainment, financial and food industries, and weightings have been attached to the companies in order to keep the index continuous, just as in the case of the FT-SE 100. The value of the DJIA on January 11 was 9619.89. 

The advantage of an index is that it depends on a group of assets and hence describes a particular sector or cross-section of the market. This means that possible spurious fluctuations in individual asset prices that are specific to that asset, rather than to the set of all underlying assets, will have a decreased efect on the index. Two of the most common derivatives based on an index are call and put options. For example, four days before expiration, an American call option on the FTSE 100 index, with a strike of 6000, a payof of £10 per point, and a expiry date of January 15 cost £1,265 while the corresponding put cost £295 (recall that the index value on January 11 was 6085.00). A European call option with a strike of 6025 and the same expiry date cost £1,085, while the put cost £340. Clearly however, the underlying asset, the index, cannot be delivered, so instead a cash transfer is made for the diference between the index value and the strike price when the payof is positive. 

Exercise 1.5 How many pounds would you receive ifyou exercised the American call and put options on the FTSE? Why is this diferent from the market price of the option? 

A forward contract allows the investor to fix the price now for either sale or purchase of the underlying asset at a fixed time in the future. For example, one might contract to buy 100 shares of Rolls-Royce in 1 year’s time for a price of 250p per share. Forward contracts of various maturities are in principle possible for any underlying asset and can also be negotiated on indices. 

A swap is an agreement to exchange two underlying assets at some specified time in the future. For example, a currency swap might involve exchanging n pounds for m dollars in one year. 

As with any field of knowledge, there are many specialized terms that require explanation or definition. A position refers to the state of an investor or trader after either buying or selling an asset or derivative. If you have bought a financial instrument, then we say that you are long that instrument, or have taken a long position in it; whereas if you sell it, then you are short the instrument. Note that taking a short position means that you have actually sold something that you do not own, however, modulo certain rules and regulations, this is allowed by many exchanges. A portfolio is a combination of positions in many diferent instruments, variously long and short. A very simple derivative, such as a call or put option, is described as vanilla, while a more complicated one is refered to as an exotic derivative. 

## 1.2 Uses of Derivatives

Derivatives are used for a variety of purposes. They can be used to reduce risk by allowing the investor to hedge an investment or exposure, and hence function as a sort of insurance policy against adverse market movements. For example, if a firm needs a particular commodity, such as petroleum, on a regular basis, then they can guard against a rise in the price of oil by purchasing a call option. If the price of oil remains low, then the option is not exercised and the oil is bought at the current price in the market, while if the price rises above the strike, then the option is exercised to buy oil at a below-market value. Derivatives can also be used to gain extra leverage for specialized market speculation. In other words, if an investor has reason to believe that the market is going to move in a particular way, then a larger profit per dollar invested can be made by buying suitable derivatives, rather than the underlying asset. But similarly, if the investment decision is wrong, the investor runs the risk of making a correspondingly larger loss. 

Exercise 1.6 Can you think of an example where a company might have interest-rate risk? How about foreign exchange risk? 

So far we have talked about investors that buy derivatives, but there must likewise be financial institutions selling them. These sellers are generally investment banks, stock exchanges, and other large institutions. When selling a derivative, the issuer makes an initial gain up-front from the fee that they charge. They must then use the up-front money, possibly in conjunction with borrowing, to hedge the derivative that they have sold by buying other instruments in the market to form a hedging portfolio, in such a manner that, regardless of the way that the prices of the underlying assets change, they neither gain nor lose money. When the derivative expires, any payof due to its owner will be equal to the current value of the hedging portfolio, less any borrowings that have to be repaid. 

But how is the value of the initial payment to be calculated? What is the composition of the hedging portfolio? It is the principle of no arbitrage, which asserts that in well-developed financial markets it is impossible to make a risk-free profit from an initially empty portfolio, that is the key to derivative pricing. If arbitrage were possible, arbitrageurs would rush in to take advantage of it, and thereby alter the price so that inevitably no further arbitrage would be possible. A kind of market equilibrium is therefore established. By requiring that no arbitrage opportunities should arise between a derivative price and the prices of the corresponding underlying assets it is possible to arrive at a formula for the value of the derivative. This will yield a so-called ‘fair price’ for a derivative. In practice, a suitable commission has to be added to the fair price, otherwise the trader would not make a profit or even cover the execution costs associated with the creation of the derivative. 

## 1.3 Derivative Payof Functions

Before it is possible to price a derivative, however, we must understand its payof function—the amount of money that the owner of the derivative is entitled to receive (or must pay) at a given date or set of dates in the future, as a function of the values of one or more underlying assets at certain dates. If we consider European options, then the payof function depends only on the value of the underlying assets at the expiry date, $t = T$ 

For a call option with strike $K$ , the owner of the derivative only receives a payof if the final asset price $S _ { T }$ is greater than the strike price K, and then the payof is equal to the diference in the two prices. This can be expressed mathematically as 

$$
C _ {T} = \max [ S _ {T} - K, 0 ].\tag{1.1}
$$

Sometimes the more compact notation $[ x ] ^ { + } = \operatorname* { m a x } [ x , 0 ]$ is used. The payof of a call option is plotted as a function of the underlying asset price in figure 1.1. 

In the case of a put option, the payof is only non-zero if the asset price at expiration is less than the strike price. This is given by 

$$
P _ {T} = \max [ K - S _ {T}, 0 ].\tag{1.2}
$$

The payof function of the put option is plotted in figure 1.2 

The third example of a derivative that we want to consider here is the forward contract. A position in a forward contract difers from call and put options in that it can have a negative payof, that is, the investor can lose money by owning the derivative. This is because the forward contract is not an option; the investor is obliged to buy (or sell) the underlying asset at the strike price previously agreed, even if it is not advantageous for him to do so. The payof function is therefore the diference between the stock price $S _ { T }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/65f08bd55d5d86062a6315643a6a4df5ef2857973bf0dca91babffd70da27144.jpg)



Figure 1.1: The payof function of a call option with a strike of $100 as a function of the price of the underlying asset.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/3abed205f2c9453a84e52c39900669fef2ce286476512efed9e7029865b8d0b9.jpg)



Figure 1.2: The payof function of a put option with a strike of $100 as a function of the price of the underlying asset.


and the strike price K, that is, 

$$
F _ {T} = S _ {T} - K.\tag{1.3}
$$

This function is plotted in figure 1.3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/ed3812c41f883a73307a3be2e88942ff5d6c66d561a8f29a25d5e314fd123d99.jpg)



Figure 1.3: The payof function of a long position in a forward contract with a strike of $100 as a function of the price of the underlying asset.


Exercise 1.7 Suppose that a dealer sells a put option, instead of buying one. What is the payof function of the dealer’s position? Why might a dealer consider selling a put option? Can you find a combination of buying and selling calls and/or puts such that the resulting portfolio payof function is equal to the payof function for a long position in a forward contract with strike K? 

Exercise 1.8 Can you find a combination of long or short positions in calls and puts that will reproduce the following payof functions: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/3fbdccf732bd60f901d7cb8ccc266284e9a5814ea246649f6a7fb64d4a0b876f.jpg)



Figure 1.4: The payof function of an option for exercise 1.8. Can you decompose it into a combination of long and short calls and puts?


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/ae78295ffb3e105976f2b47ffe6964016351e9d7624d524733dc1f3f49dfac60.jpg)



Figure 1.5: The payof function of an option for exercise 1.8.


## 2 Arbitrage Pricing

As mentioned in the previous section, arbitrage—the ability to start with nothing and yet make a risk-free profit—is the key to understanding the mathematics of derivative pricing. In this section we will show how it can be used to determine a unique price for a derivative by using an example taken from the foreign exchange markets. 

Consider the exchange rate between U.S. dollars and U.K. pounds sterling. Let $S _ { t }$ be the price of one unit of sterling (i.e., one pound) in dollars at time t. For example, we might have $S _ { 0 } = \ S 1 . 6 0$ , which means that at time $0 ,$ it costs $1.60 to buy one pound. We say that $S _ { t }$ is the spot price for sterling at time t. We can contrast this with ${ \cal \tilde { S } } _ { t } ,$ the forward price, which is the price in dollars contracted today, that is at time $t = 0$ , for the purchase of one unit of asset (in our case one pound sterling) at time t in the future.<sup>3</sup> This means that we agree today to buy one pound sterling at time t for the price $\tilde { S } _ { t }$ , paying the amount $\tilde { S } _ { t }$ at time t on delivery of the sterling. The ‘tilde’ notation is used throughout the book as a reminder that $\tilde { S } _ { t }$ is a forward rather than spot price. We want to calculate the value of $\tilde { S } _ { t }$ which ensures that no arbitrage is possible. 

## 2.1 Expectation Pricing

One possible method for determining the forward price is expectation pricing. In this framework, we assume that $S _ { t }$ is a random variable, and set the forward price equal to the expected spot price at time t, 

$$
\tilde {S} _ {t} = E [ S _ {t} ].\tag{2.1}
$$

While at first glance this may seem reasonable, it is, unfortunately, not correct. This is because if the forward price is set by equation (2.1), then a clever arbitrageur can, by use of a crafty series of investments in the dollar and sterling money market accounts, make a risk-free profit. This is a situtation that, so the argument goes, would not be tolerated for long. You will have heard the old saying, “There ain’t no such thing as a free lunch”. 

We shall now demonstrate just how the arbitrageur is denied from dining at others’ expense. 

## 2.2 Arbitrage Pricing

Let $r$ and $\rho$ be the continuously compounded interest rates for dollars and pounds respectively. We assume here, for simplicity, that r and $\rho$ are constant. We can then let $D _ { t }$ and $P _ { t }$ denote the values respectively of the dollar and sterling bank accounts (money market accounts) at time t. As shown in exercise 1.3, the value of the dollar bank account at time t is 

$$
D _ {t} = D _ {0} e ^ {r t},\tag{2.2}
$$

while a similar relation holds for the sterling bank account, $P _ { t } = P _ { 0 } e ^ { \rho t }$ . Here $D _ { 0 }$ and $P _ { 0 }$ denote the initial number of dollars and pounds put on deposit. 

We now want to consider two diferent trading strategies for an initial investment of $n$ pounds that must be converted into dollars by time t. We would like the strategies to be deterministic, that is, they should not depend on any random variables, but instead must yield a definite result at time t. Since there are only two exchange rates that we know for sure, today’s rate $S _ { 0 }$ and the forward rate $\tilde { S } _ { t }$ , then there are only two times that we can exchange currencies without introducing some element of randomness—today, and at time t. Consider the two investment strategies described in figure 2.1. The ‘dollar investment strategy’ converts the initial n pound investment to dollars immediately, and has a final value of $n S _ { 0 } e ^ { r t }$ dollars. The ‘forward buying strategy’ takes the opposite tack and doesn’t convert the pounds to dollars until time t. This alternative route yields $n \tilde { S } _ { t } e ^ { \rho t }$ dollars. We then equate the results of the two investment strategies, that is, we have the relation 

$$
n \tilde {S} _ {t} e ^ {\rho t} = n S _ {0} e ^ {r t},\tag{2.3}
$$

which implies that 

$$
\tilde {S} _ {t} = S _ {0} e ^ {(r - \rho) t}.\tag{2.4}
$$

Thus, the forward price $\tilde { S } _ { t }$ is entirely determined by the interest rate $d i f -$ ferential $r \mathrm { ~ - ~ } \rho .$ and not, perhaps surprisingly, by the expected value of the spot rate $E [ S _ { t } ]$ . But why did we equate the results of the two investment strategies? The answer lies in the no arbitrage condition. 

Suppose that one could contract to sell sterling at a rate $F _ { t }$ , higher than $\tilde { S } _ { t }$ . Then, using the arbitrage strategy outlined in figure 2.2, an enterprising but penniless arbitrageur could start with no money but end up with $n ( F _ { t } -$ $\tilde { S } _ { t } ) e ^ { \rho t }$ dollars. Since $F _ { t } > \tilde { S } _ { t } .$ , by use of this fiendishly clever strategy a sure profit is generated without any initial investment and with absolutely no risk, that is, arbitrage occurs. In such a case, arbitrageurs will swoop in and take advantage of the situation, generating guaranteed profits for themselves, and essentially forcing traders to adjust their forward prices until at last the arbitrage opportunities disappear. In this way, the no arbitrage condition allows us to obtain a price for the forward contract. 

Dollar Investment Strategy:
1. Start with n pounds.
2. Exchange the n pounds for dollars at time 0, using the spot price $S_{0}$ . We now have $nS_{0}$ dollars, which we invest in a dollar bank account.
3. Sit back and relax.
4. At time t the investment is worth $nS_{0}e^{rt}$ dollars.

Forward Buying Strategy:
1. Start with n pounds and deposit them in the sterling bank account.
2. Contract to sell $ne^{\rho t}$ pounds for dollars at the forward exchange rate $\tilde{S}_{t}$ at time t. This is called a forward sale, since the contract is made at time 0 for a sale at time t.
3. At time t, the value of the sterling bank account will be $ne^{\rho t}$ pounds.
4. Convert the sterling to dollars at the contracted exchange rate $\tilde{S}_{t}$ (that is, execute the forward sale). The value of the dollar account is then $n\tilde{S}_{t}e^{\rho t}$ dollars. 


Figure 2.1: Two trading strategies which both begin with n pounds and 0 dollars, and end with 0 pounds and a fixed number of dollars. Arbitrage arguments tell us that the final number of dollars must be the same for both strategies.


Exercise 2.1 Show how an arbitrageur can make a sure profit with no risk if $F _ { t } < \tilde { S } _ { t }$ 

Arbitrage Strategy:
1. Start with nothing and borrow $nS_{0}$ dollars at the interest rate r. Immediately exchange these dollars at the spot rate $S_{0}$ for n pounds, which we deposit in the sterling bank account.
2. Still at time 0, contract to sell $ne^{\rho t}$ pounds forward at time t at the given ‘high’ forward exchange rate $F_{t} (> \tilde{S}_{t})$ .
3. At time t, the initial loan of $nS_{0}$ dollars now requires $nS_{0}e^{rt}$ dollars be repaid, while the sterling bank account has $ne^{\rho t}$ pounds in it.
4. Sell the pounds in the sterling bank account (taking advantage of the previous contracted agreement) at the price $F_{t}$ dollars per pound. This generates $nF_{t}e^{\rho t}$ dollars, so that after repaying the loan, the remaining number of dollars is $nF_{t}e^{\rho t}-nS_{0}e^{rt}=\quad ne^{\rho t}(F_{t}-S_{0}e^{(r-\rho)t})$ $=ne^{\rho t}(F_{t}-\tilde{S}_{t}).$ (2.5) 


Figure 2.2: A trading strategy which generates a guaranteed profit if the ofered forward price $F _ { t }$ is greater than the no arbitrage value $\tilde { S } _ { t }$


Exercise 2.2 Suppose that the initial exchange rate is $1.60, and that the interest rates are 10% and 8% (per annum) for dollars and pounds respectively. What is the exchange rate for a two-year forward purchase? 

Exercise 2.3 If the sterling interest rate is no longer time independent, but is instead given by a steadily changing rate according to the scheme $\rho ( t ) = a +$ bt, then what is the forward exchange rate? Suppose that the initial exchange rate is $1.60, the dollar interest rate is 10%, and the constant terms in sterling rate are 8% and 1% for a and b respectively. What is the exchange rate for (a) a two-year forward purchase, and (b) a four-year forward purchase? 

## 2.3 Trading Strategies

However, it still may not be clear why we had to equate the final values of the two trading strategies given in figure 2.1, since we ended up using a diferent trading strategy (that of figure 2.2) in order to prove that a forward price other than $\tilde { S } _ { t }$ would imply arbitrage. In order to understand the connection between the three trading strategies better, we should consider exactly what it is that we mean by a trading strategy—up to this point we have been slightly cavalier in our definitions and assumptions. For example, $D _ { t }$ does not tell you how much money that you have in the dollar bank account at time t, but rather it tells you how much a unit of the money market account is worth. It is easy to forget that the money market account is an underlying asset, just like a share in a company, and it can be bought and sold on the market. This is best illustrated with a simple example. Suppose that at time 0, the money market account is worth one dollar $( D _ { 0 } = 1 )$ . If I buy 100 units of it, then it will cost me 100 dollars. At time t, one unit of the money market account is worth $e ^ { r t }$ dollars, and since I have 100 units, my original investment is now worth $1 0 0 e ^ { r t }$ dollars. If I sell my units, then I receive this money and the value of my holdings in the money market becomes zero, but the money market account is still worth $D _ { t } = e ^ { r t }$ dollars per unit. 

From this example, it should be obvious that in addition to the value of a unit of the money market account $D _ { t }$ , we also need to introduce a second quantity $\phi _ { t }$ which tells you how much of the money market account that you own. The total value of your holding is then $\phi _ { t } D _ { t }$ , that is, it is the number of units of the money market account that you own, multiplied by the value of each unit. We will also need to introduce a quantity $\psi _ { t }$ which is equal to the number of units of the sterling money market account that you own. 

A trading strategy is then the pair or ‘portfolio’ $\left( \phi _ { t } , \psi _ { t } \right)$ which tells you how much of each asset that you own. ‘Buying’ an asset then corresponds to increasing the value of $\phi _ { t }$ or $\psi _ { t }$ , whereas ‘selling’ means decreasing the value. A negative value means that we are borrowing money, or have ‘sold short’ the asset. 

Look at figure 2.3. This is a graphical representation of the trading 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/5b99042635a71a8ee427d264f589561edb60d7a7fb5e5cdc1448cb47b758cffa.jpg)



Figure 2.3: The portfolio values for the dollar investment strategy (left) and the forward buying strategy (right).


strategies outlined in figure 2.1. The portfolios are discontinuous in time because money can be exchanged instantaneously. The times $0 ^ { - } , ~ 0 ^ { + }$ and $t ^ { - } , t ^ { + }$ represent left and right handed limits as time approaches 0 and t respectively. The steps 1,2,3 and 4 in figure 2.1 correspond to the time steps $0 ^ { - } , 0 ^ { + }$ , t− and $t ^ { + }$ . Similarly figure 2.4 is a realization of the arbitrage strategy described in figure 2.2. 

What mathematical operations can we perform on trading strategies? Well, suppose that $( \phi _ { t } , \psi _ { t } )$ is a trading strategy. Then what about its negative $\left( - \phi _ { t } , - \psi _ { t } \right)$ , is this also a trading strategy? Of course it is! It is the strategy which simply buys whenever the original strategy sells and sells whenever the original strategy buys. How about if we had two trading strategies $( \phi _ { t } , \psi _ { t } )$ and $( \phi _ { t } ^ { \prime } , \psi _ { t } ^ { \prime } )$ . Could we add them together to get a new strategy, $( \phi _ { t } + \phi _ { t } ^ { \prime } , \psi _ { t } +$ $\psi _ { t } ^ { \prime } ) \smash { \vdots }$ Again, the answer is yes! The new strategy simply performs all the buy and sell operations of the two original strategies. In terms of portfolio value plots, like those in figures 2.3 and 2.4, a negative trading strategy simply reverses the direction of all the arrows, while a sum of two strategies means that you combine all the arrows from both plots into a new one. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/5f0e35f324d5190f35b6f08b087a880e3d1ec1bfe7156305f3ddb3adcb50c797.jpg)



Figure 2.4: The portfolio values for the Arbitrage strategy.


We are now in a position to see exactly why we must equate the final values of the ‘dollar investment strategy’ and the ‘forward buying strategy’. Consider the trading strategy formed by adding the negative of the dollar investment strategy to the forward buying strategy. What does this look like? Well, at $0 ^ { - }$ the sterling holdings cancel and there are no dollar holdings, so we begin with nothing. Then at time $0 ^ { + }$ we have n pounds and $- n S _ { 0 }$ dollars. $\mathrm { A t } t ^ { - }$ , the sterling holdings are worth $n e ^ { \rho t }$ , while our dollar debt has mounted $\mathrm { t o } \mathrm { ~ - } n S _ { 0 } e ^ { r t }$ . Finally, at $t ^ { + }$ , we liquidate our sterling position and have a final dollar holding of $n \tilde { S } _ { t } e ^ { \rho t } - n S _ { 0 } e ^ { r t }$ . But since we began with nothing, in order to avoid arbitrage we must also end with nothing, and hence we must set $n \tilde { S } _ { t } e ^ { \rho t } - n S _ { 0 } e ^ { r t } = 0$ , which is the equivalent of equating the final values of the dollar investment strategy and the forward buying strategy. 

This new trading strategy outlined above is easiest to follow by simply subtracting the left hand side of figure 2.3 from the right hand side. You should then notice a remarkable similarity to the arbitrage strategy of figure 2.4, except that $F _ { t }$ is replaced by $\tilde { S } _ { t }$ . Thus, the arbitrage strategy is simply the forward buying strategy minus the dollar investment strategy. 

## 2.4 Replication Strategy

Any no arbitrage argument for pricing a derivative is ultimately based on a replication strategy, which is a trading strategy that uses market instruments to ‘replicate’ the initial and final positions required by the derivative. How does this work? Well, given two strategies with the same initial position, and guaranteed final positions, then these final positions must be equal. Otherwise, by going long the strategy with the higher final value and short the other we would generate an arbitrage. 

For example, suppose that we have a forward contract to buy one unit of sterling for a price ${ \ddot { S } } _ { t } .$ Then the cash flow is very simple: at time t we receive one unit of sterling and pay $\tilde { S } _ { t }$ dollars. This cash flow is shown in the left side of figure 2.5. Can we replicate this cash flow by using market instruments? Most certainly. Start with nothing, then borrow $S _ { 0 } e ^ { - \rho t }$ dollars from the bank and convert it into $e ^ { - \rho t }$ pounds. At time t we shall have the required one pound sterling, while the dollar position is short $S _ { 0 } e ^ { ( r - \rho ) t }$ dollars. This is shown on the right side of figure 2.5. Since the intial and final position of the derivative cash flow and replicating strategy are the same, and their final positions are both deterministic, then by our earlier arguments these final positions must be equal, so $\tilde { S } _ { t } = S _ { 0 } e ^ { ( r - \rho ) t }$ , as we have calculated several times before. Now let us consider a slightly more complicated example. 

## 2.5 Currency Swap

What we have done up to now is, given the current exchange rate and the interest rates in two currencies, to determine the no arbitrage value for the forward exchange rate at some time t in the future. However, suppose that we know what exchange rate we would like to pay in the future, and would like to agree on it now. This is a currency swap. Unlike the previous example it may involve an initial purchase price. But identical to the previous example, we can calculate the price of the derivative by replicating its cash flow. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/22a0715c5d9d5531e46598bbd82b3e520fadf7f00a43001e52e564e83d629e42.jpg)



Figure 2.5: The cash flow for a forward contract is shown on the left side. We can construct the replication strategy shown on the right such that it has the same initial and final positions as the derivative. This allows us to determine the forward price.


Suppose that we agree to swap nK dollars for n pounds at time t. What is the cash flow? Well, at time 0, we receive an initial cash payment of C dollars, which may be negative. This is the price paid by the dollar-purchaser for the swap. At time t, the currency swap occurs and we receive n pounds but must pay nK dollars to our counterparty. This cash flow is shown in figure 2.6. Can we artificially construct a trading strategy that has the same initial and final positions as the derivative? 

The first step in creating the replicating strategy is to start with C dollars and no sterling so that the initial positions are the same. Recall that C is the cost of the derivative (in dollars) that we are trying to calculate. If we convert $n S _ { 0 } e ^ { - \rho t }$ dollars into $n e ^ { - \rho t }$ pounds at time 0, then at time t this will produce the required sterling position of n pounds. The value at time 0<sup>+</sup> of the dollar account is $C - n S _ { 0 } e ^ { - \rho t }$ dollars, and hence at time t it will be worth $( C - n S _ { 0 } e ^ { - \rho t } ) e ^ { r t }$ dollars. What do we do next? Well, just as in the previous example, we set the value of the replicating position equal to that of the derivative. Anything would else allow arbitrage. Thus 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/f9b54da86f206b22b22bf03a96babeeb466b172469f566703eac8888f2dedc9f.jpg)



Figure 2.6: The cash-flow for a dollar-pound currency swap is shown on the left. The sterling-purchaser receives an initial amount C in dollars. This is the ‘cost’ of the swap. Then at time t, he receives n pounds and pays nK dollars to his counterparty. On the right is a replicating strategy which reproduces the swap cash-flow. Starting with C dollars, $n S _ { 0 } e ^ { - \bar { \rho } t }$ dollars are converted into pounds. At time t this will produce the required sterling position. We can then adjust the value of $C$ such that the dollar position is also equal to the required swap value, which therefore uniquely determines the cost of the swap.


$$
\left(C - n S _ {0} e ^ {- \rho t}\right) e ^ {r t} = - n K\tag{2.6}
$$

This allows us to solve for the purchase price $C _ { i }$ 

$$
\begin{array}{r c l} C & = & n e ^ {- r t} \left(S _ {0} e ^ {(r - \rho) t} - K\right) \\ & = & n e ^ {- r t} \left(\tilde {S} _ {t} - K\right) \end{array}\tag{2.7}
$$

Hence the price that the dollar-purchaser must pay for a currency swap where n pounds are exchanged for nK dollars is $n ( \tilde { S } _ { t } - K ) e ^ { - r t }$ dollars. The replication strategy is shown in the right side of figure 2.6. Note that the value of K that yields a zero price for the currency swap is the forward rate $\tilde { S } _ { t }$ . That is why there is no cost for either party to enter into a forward contract. 

## 2.6 Summary

The principle of no arbitrage may be the key to understanding derivative pricing, but what kind of law is it? It is clearly not a fundamental law of nature, and is not even always obeyed by the markets. In some ways it is similar to Darwin’s theory of natural selection. An institution that does not price by arbitrage arguments the derivatives that it sells will sufer relative to institutions that do. If the price is set too high, then competitors will undercut it; if the price is too low, then the institution will be liable to market uncertainty as a hedging portfolio cannot be properly constructed. In the competitive world of finance, such an institution would not last long. 

There is a crucial point to take away from this section, and to which we shall come back again and again in the course of this book. It is that the actual probabilities of what might happen to the exchange rate (or any other underlying asset) are not important. This is because the expectation of a random variable, such as the exchange rate, may give a good idea of what the exchange rate may be in the future, but it leaves too much to chance. What matters instead, is that we can create a trading strategy such that there is no uncertainty in the outcome. By creating a risk-free strategy that also replicates the derivative payof function, we can uniquely determine the no arbitrage price for the derivative. 

## 3 A Simple Casino

When it comes right down to it, putting money into the financial world can be a bit of a gamble. So there is really no better way to begin thinking about financial mathematics than by looking at betting in a Casino, which is every bit a gamble. To meet our sophisticated tastes, we will be betting in a deluxe Casino that allows not only standard wagers, but also ‘side-bets’ which we shall call derivative bets. Our Casino analogy will turn out to be a very simple, but highly efective, model for a stock market. After laying down the rules for gambling and investigating the nature of ‘ordinary’ bets, the goal will be to find a price for the derivative bets by use of the no arbitrage condition. 

## 3.1 Rules of the Casino

Suppose that we make our way into a Casino that allows gamblers to make bets on the outcome of a coin flip. While this is probably one of the simplest Casinos imaginable, we can make it a more interesting place by increasing the complexity of the bets that can be made on the result of the coin toss. 

At time $0 ,$ just before the coin toss, the initial stake for a bet is $S _ { 0 }$ dollars, which you pay to the Casino. The amount that you receive back from the Casino at time $t ,$ just after the coin toss, is $S _ { t }$ dollars, which for the ‘standard’ bet we define to be $U$ dollars $\mathrm { ( \dot { u } p ^ { \prime } ) }$ for heads and D dollars (‘down’) for tails. For example, we could take 

$$
S _ {0} = 2. 0 0, \quad U = 3. 0 0, \quad \text {and} \quad D = 1. 5 0.\tag{3.1}
$$

In this case, we place $2.00 on the the table, and if the outcome is heads we get $3.00 back, while if the outcome is tails, then we only get $1.50 back. In addition to this ‘standard’ bet, we can also make a short bet. This means that at time 0 the Casino pays you $S _ { 0 }$ dollars to enter the game, but then you have to pay the Casino $S _ { t }$ dollars at time $t ,$ so the actual amount that you have to pay depends on the outcome of the coin flip. Under this naming scheme, the standard bet is actually a long bet. Since we can place both long and short bets with the same initial stake, the roles of the Casino and player are symmetric in our simple model. In a real Casino this is not, of course, the case, and the rules of the various games are designed so that the Casino will on average make money. 

Since the Casino is trying to encourage gambling, it is willing to lend money at no charge. It will also hold your money for you, however no interest is earned. Thus, we can think of the Casino as having a money market account where the risk-free interest rate is zero. 

Exercise 3.1 Using a simple arbitrage argument, show why we must have $U > S _ { 0 } > D$ 

The Casino is a chaotic place, but the organisers and participants are known to be honest. That is, the rules of the Casino are always obeyed. We are not told whether the coin is ‘fair’ (50-50), nor is there any implication that it is. We suspect that it isn’t fair, and after watching play for a few hours and making use of the law of averages, we conclude that the relevant probabilities are 

$$
\operatorname{Prob} [ H ] = p \quad \text { and } \quad \operatorname{Prob} [ T ] = q,\tag{3.2}
$$

where H, T stand for heads and tails respectively, and $p + q = 1$ . We are also worried that these probablities may change over time. 

Clearly the expected payof from a standard bet is $E [ S _ { t } ] = p U + q D$ dollars. But there is no reason (a priori) to suppose that the initial stake satisfies $S _ { 0 } = E [ S _ { t } ]$ . This is the expectation hypothesis, which we saw in the previous section is generally wrong. If $S _ { 0 } < E [ S _ { t } ]$ , then anyone willing to play this game is risk-averse, that is, they expect some profit, on average, for taking risk. If $S _ { 0 } > E [ S _ { t } ]$ , then players, on average, pay to take risk (which is typical for a Casino), and are risk-preferring. If $S _ { 0 } = E [ S _ { t } ]$ , then the players are risk-neutral, since they expect to neither gain nor lose money if they play for a long time. 

## 3.2 Derivatives

A derivative is a kind of side-bet, with a prescribed payof that depends on the outcome of the coin flip. The Casino is happy to allow derivative bets by special arrangement. In a typical contract, a player pays an initial bet $f _ { 0 }$ at time 0, and then receives a payof of $f _ { t } ( S _ { t } )$ dollars at time $t ,$ where $f _ { t } ( S _ { t } )$ is a prescribed function of the random variable $S _ { t }$ . A derivative contract is defined by its payof function $f _ { t } ( S _ { t } )$ and its purchase price $f _ { 0 }$ . It is possible, in principle, for $f _ { 0 }$ to be negative, which by convention means that the Casino pays the player to enter into the contract. Note that $f _ { t } ( S _ { t } )$ can also, in principle, be negative, in which case the player has to pay the Casino at time t. 

For example, we can consider the important case of a call option, which has a payof function 

$$
f _ {t} (S _ {t}) = \max [ S _ {t} - K, 0 ],\tag{3.3}
$$

where K is a fixed number of dollars, known as the strike price, such that $U > K > D$ . By construction, the call option pays of only when $S _ { t } = U$ Note that many options, even if they are based on an underlying asset, do not necessarily involve the buying or selling of the underlying, but rather the cash diference between the asset value and the strike price is transferred if the terminal value of the asset exceeds the strike (assuming that the option is a call). In cases where the underlying is not transferrable, such as an option on a stock index, or the outcome of a coin flip, then a cash transfer is the only possibility. We could also consider a more complicated derivative, with a payof function such as 

$$
f _ {t} (S _ {t}) = \alpha S _ {t} ^ {3} + \beta S _ {t} ^ {2} + \gamma S _ {t} + \delta ,\tag{3.4}
$$

where $\alpha , \beta , \gamma , \delta$ are constants. The pricing of an exotic derivative, like this one, is computationally more dificult than for a vanilla one, such as the call option above, however, mathematically they are given by the same general formula. 

Now we need to determine the price $f _ { 0 }$ that someone should pay at time 0 to buy a derivative that pays of $f _ { t } ( S _ { t } )$ dollars at time t. A plausible guess is 

$$
\begin{array}{r c l} f _ {0} & = & E [ f _ {t} (S _ {t}) ] \\ & = & p f _ {t} (U) + q f _ {t} (D), \end{array}\tag{3.5}
$$

which represents the expected payof of the derivative, that is, the probability weighted average of the possible payofs. This guess is another typical example of the ‘expectation hypothesis’. As before, it is wrong. So how do we determine $f _ { 0 } { ? }$ Just like in the simple currency model of section 2, we want to use a no arbitrage condition to determine the correct price. 

## 3.3 No Arbitrage Argument

Suppose that instead of dealing directly with the Casino, the player instead goes through an intermediary known as the dealer or trader. Then, if the gambler purchases a derivative from the dealer, the dealer gets $f _ { 0 }$ dollars at time 0, and must pay $f _ { t } ( S _ { t } )$ dollars back to the player at time t. The dealer does not want to take any risk, and hence must hedge his derivative position by making a standard bet with the Casino, in a manner that we shall describe. Rather than making a full-sized bet, the stake for this standard bet is only $\delta S _ { 0 }$ . The idea is that the dealer will choose $\delta$ such that the total payof at time t is independent of the result of the coin flip, and hence a guaranteed amount. 

To calculate the required value of $\delta ,$ we note that at time t the dealer gets $\delta S _ { t }$ dollars from the Casino, but has to pay $f _ { t } ( S _ { t } )$ dollars to the player. So the dealer’s net payof at time t is $\delta S _ { t } - f _ { t } ( S _ { t } )$ dollars. Since the dealer wants this potentially random amount to be independent of the outcome of the coin flip, we need to force the two possible payofs to be the same, that is, we require that 

$$
\delta U - f _ {t} (U) = \delta D - f _ {t} (D).\tag{3.6}
$$

But, we can solve this for $\delta$ to get 

$$
\delta = \frac {f _ {t} (U) - f _ {t} (D)}{U - D}.\tag{3.7}
$$

This value of $\delta$ is called the hedge ratio. If the dealer makes a standard bet with the Casino in this quantity, that is, with initial stake $\delta S _ { 0 }$ dollars, then his obligation to the player (through the derivative) is ‘hedged’. 

## Exercise 3.2 Calculate the value of dealer’s payof for the hedged bet.

We can now apply the no arbitrage argument. Suppose that the dealer starts with nothing. At time 0 he sells the derivative to the player and receives $f _ { 0 }$ dollars, while at the same time he makes a basic bet with the Casino for $\delta S _ { 0 }$ dollars. After completing these two transactions the dealer will have $f _ { 0 } - \delta S _ { 0 }$ dollars left over, which is put into the bank account. At time $t ,$ after the coin toss, the dealer obtains the guaranteed amount $\delta S _ { t } - f ( S _ { t } )$ In addition, he has money in the bank account, although since it has not earned any interest it is still worth $f _ { 0 } - \delta S _ { 0 }$ dollars. Thus, the net value of the dealer’s position at time t is $f _ { 0 } - \delta S _ { 0 } + \delta S _ { t } - f _ { t } ( S _ { t } )$ dollars. But this is a risk-free amount, and since the dealer started with nothing, he must end with nothing, so 

$$
f _ {0} - \delta S _ {0} + \delta U - f _ {t} (U) = 0,\tag{3.8}
$$

or equivalently, 

$$
f _ {0} - \delta S _ {0} + \delta D - f _ {t} (D) = 0.\tag{3.9}
$$

This relation can be used to solve for the correct price $f _ { 0 }$ of the derivative. We get 

$$
\begin{array}{r c l} f _ {0} & = & f _ {t} (U) + \delta (S _ {0} - U) \\ & = & f _ {t} (U) + \frac {f _ {t} (U) - f _ {t} (D)}{U - D} (S _ {0} - U) \\ & = & \frac {f _ {t} (U) (U - D) + [ f _ {t} (U) - f _ {t} (D) ] (S _ {0} - U)}{U - D} \\ & = & \frac {f _ {t} (U) [ S _ {0} - D ] - f _ {t} (D) [ S _ {0} - U ]}{U - D} \\ & = & f _ {t} (U) \frac {S _ {0} - D}{U - D} + f _ {t} (D) \frac {U - S _ {0}}{U - D}. \end{array}\tag{3.10}
$$

Note that it was only possible to apply this argument because the dealer always gets the same payof from his hedged position, that is, it is independent of the actual outcome of the coin flip. 

The derivative price calculated in equation (3.10) can be summarised succintly by writing 

$$
f _ {0} = p ^ {*} f _ {t} (U) + q ^ {*} f _ {t} (D),\tag{3.11}
$$

where 

$$
p ^ {*} = \frac {S _ {0} - D}{U - D}, \quad \text { and } \quad q ^ {*} = \frac {U - S _ {0}}{U - D}.\tag{3.12}
$$

A quick calculation will confirm that $p ^ { * } , q ^ { * } > 0$ and $p ^ { * } + q ^ { * } = 1$ , which means that $f _ { 0 }$ can be interpreted as a kind of weighted average of the outcomes $f _ { t } ( U )$ and $f _ { t } ( D )$ , where the weights are given by the numbers $p ^ { * }$ and $q ^ { * }$ . 

Exercise 3.3 Show that an arbitrageur can make a sure profit if the derivative is priced other than at $f _ { 0 }$ . 

The price $f _ { 0 }$ does not depend in any way on the actual weighting of the coin as given by the probabilities $p , q$ . In fact, the price $f _ { 0 }$ is completely determined once we know the Casino rules, that is, the basic stake $S _ { 0 }$ , the payofs $U$ and $D _ { : }$ , and the derivative payof contract specification $f _ { t } ( S _ { t } )$ . This independence from ‘real’ or ‘physical’ probabilities is one of the ‘mysterious’ features of derivative pricing in general, as we shall see, that already applies very clearly in this somewhat simplistic, but nevertheless very important example. 

## 4 Probability Systems

Here we shall digress briefly to review some basic ideas in probability. We need to acquire an understanding of the diferent parts of a probability system and how they fit together. In order to make some sense of it all, we shall find it useful to think of a probability system as a physical experiment with a random outcome. To be more concrete, we shall use a specific example to guide us through the various definitions and what they signify. 

Suppose that we toss a coin three times and record the results in order. This is a very simple experiment, but note that we should not necessarily assume that the coin toss is fair, with an equally likely outcome for heads or tails. After all, life is rarely as fair as we would like it to be, and we need to be prepared for this. Joking aside, the reason for this chapter is to make it clear that there can, in principle, be many diferent probabilities associated with the same ‘physical experiment’. This will have an impact on how we price derivatives. 

## 4.1 Sample Space

The basic entity in a probability system is the sample space, usually denoted Ω, which is a set containing all the possible outcomes of the experiment. If we denote heads by H and tails by T, then there are 8 diferent possible outcomes of the coin-tossing experiment, and they define the sample space Ω as follows: 

$$
\Omega = \{H H H, H H T, H T H, H T T, T H H, T H T, T T H, T T T \}.\tag{4.1}
$$

We formalize the concept of a sample space in the following definition, 

Definition 4.1 The sample space $\Omega = \{ \omega _ { i } \} _ { i = 1 } ^ { N }$ is the set of all possible outcomes of the experiment. 

Note that we are assuming that the sample space is finite. This is applicable to the discrete time formalism that we are developing in our discussion of the Casino and the binomial model that follows on from this, but will have to be modified for the continuous time formalism that is to come later. 

## 4.2 Event Space

We are eventually going to want to talk about the probability of a specific ‘event’ occurring. Is the sample space, simply as given, adequate to allow us to discuss such a concept? Unfortunately, the answer is “not quite”. This is because we want to ask more than just, “What is the probability that the outcome of the coin toss is a specific element of the sample space, say $H T H ? $ We also want to ask, “What is the probability that the outcome of the coin toss belongs to a certain subset of the sample space, for example HTT, HTH ?”. We refer to subsets of Ω as events. For example, HTT, HTH is the event that the coin tosses result in either HTT or HTH. Thus, the question to ask is, “What is the probability that such-andsuch a specific event occurs?”. In order to be able to answer this, we need the concept of the set of all the events that we are interested in. This is called the event space, usually denoted Σ. 

What conditions should an event space satisfy? The most ‘basic’ event is Ω itself, that is, the event that one of the possible outcomes occurs. This event has probability one, that is, it always happens. It would thus make sense to require the event space to contain Ω. Likewise, we shall assume that the ‘null’ event , which occurs with probability zero, is also in the event space. Next, suppose that the events $A = \{ H T T , T H H \}$ and $B =$ HTH, HHH, HTT are elements of Σ. It is natural to be interested in the event that either A or B occurs. This is the union of the events, $A \cup B =$ HTT, THH, HTH, HHH . We would like Σ to be closed under the union of two of its elements. Finally, if the event $C = \{ H H H , H T H , H T T \}$ is an element of Σ, then the probability of it occurring is one minus the probability that the complementary event $\Omega - C = \{ H H T , T T T , T T H , T H T , T H H \}$ occurs. Hence if an event is in Σ, we would also like its complement to be in Σ. We can summarise the definition of the event space as follows. 

Definition 4.2 The event space $\Sigma$ is a set of subsets of the sample space Ω, satisfying the following conditions: 

1. $\Omega \in \Sigma$ 

2. $i f A , B \in \Sigma$ , then $A \cup B \in \Sigma$ 

3. if $A \in \Sigma$ , then $\Omega - A \in \Sigma$ 

Note that for our purposes, we can take Σ to be the power set (the set of all subsets) of Ω. The power set of our example system is perhaps just slightly too large to comfortably write out. It contains $2 ^ { 8 } = 2 5 6$ elements. 

Exercise 4.1 Show that the power set of Ω is a valid event space. Write down the power set generated by two coin tosses. 

Exercise 4.2 How about the set $\{ \varnothing , \Omega \} _ { \ast } ^ { \ell }$ Does it satisfy the definition of an event space? 

The system consisting of the sample space and the event space (Ω, Σ) might appropriately be called a ‘possibility system’, as opposed to a ‘probability system’ because all that it tells us are the possible outcomes of our experiment. It contains no information about how probable each event is. The so-called ‘probability’ measure is an additional ingredient, that must be specified in addition to the pair (Ω, Σ). 

## 4.3 Probability Measure

Now suppose that we want to assign a probability to each event in Σ. We can do this by means of a probability measure $P : \Sigma  [ 0 , 1 ]$ . For any event $A \in \Sigma , P [ A ]$ is the probability that the event A occurs. For example, if the coin is fair, then the probability of any event XY Z occurring (where X, Y , $Z$ can be either H or $T )$ is clearly $1 / 8$ . Sometimes, instead of writing $P [ A ]$ for the probability of event A, we write $\mathrm { P r o b } [ A ]$ to make the notation more explicit. 

Now, what conditions should we place on a probability measure? We have already constrained its values to lie between zero and one. Since the event Ω always occurs, its probability is one. Finally, if we have two disjoint sets, then the probability of their union occurring should be equal to the sum of the probabilities of the disjoint sets. For example, 

$$
\begin{array}{r c l} \text {Prob} [ \{H H H, T T T \} ] & = & \text {Prob} [ \{H H H \} ] + \text {Prob} [ \{T T T \} ] \\ & = & \frac {1}{4}. \end{array}\tag{4.2}
$$

Combining these constraints leads to the definition 

Definition 4.3 A probability measure P is a function $P : \Sigma  [ 0 , 1 ]$ satisfying 

1. $P [ \Omega ] = 1$ 

2. if $\sigma , \rho \in \Sigma$ and $\sigma \cap \rho = \emptyset$ , then $P [ \sigma \cup \rho ] = P [ \sigma ] + P [ \rho ]$ 

Taken together, the sample space, event space and probability measure form a so-called probability system, denoted $\mathcal { P } = ( \Omega , \Sigma , P )$ 

Exercise 4.3 Assume that Σ is the power set of Ω, and that Ω has a finite number of elements. Show that a probability measure is uniquely defined by its action on the single element sets of Σ. 

Exercise (4.3) demonstrates why we can sometimes get away with only talking about the sample space Ω and ignoring the more complicated event space Σ. For example, if $\Omega = \{ \omega _ { i } \} _ { i = 1 } ^ { N }$ is the sample space, then we call the set of numbers $\{ p _ { i } = P [ \omega _ { i } ] \} _ { i = 1 } ^ { N }$ the probabilities of Ω. Knowing the ‘probabilities’ of Ω is then equivalent to knowing the full probability measure $P ,$ , and so, as long as the sample space is finite, we can use either formulation when discussing a probability system $\mathcal { P } _ { \cdot }$ 

The key point to stress here is that we can in principle consider various probability measures on the same sample and event spaces (Ω, Σ). This turns out to be very useful in financial analysis. In our coin tossing example, we have already considered the probability measure P that we obtain if the coin that we are tossing is fair. However, we could also define a probability measure $Q : \Sigma  [ 0 , 1 ]$ that is based on an ‘unfair’ coin. Suppose that for the unfair coin we get heads with probability $1 / 3 { \mathrm { ; } }$ , and tails with probability $2 / 3$ . Then the probability measure is defined by the probabilities 

$$
\begin{array}{r c l} {Q (\{H H H \})} & = & {\frac {1}{2 7}} \\ {Q (\{H H T \})} & = & {q (\{H T H \}) = q (\{T H H \}) = \frac {2}{2 7}} \\ {Q (\{H T T \})} & = & {q (\{T T H \}) = q (\{T H T \}) = \frac {4}{2 7}} \\ {Q (\{T T T \})} & = & {\frac {8}{2 7}.} \end{array}\tag{4.3}
$$

Both measures are, in principle, valid to consider, so that when we are talking about probabilities related to the coin tossing, we must specify whether we are ‘in’ the probability system $\mathcal { P } = ( \Omega , \Sigma , P )$ , ‘in’ the probability system $\mathcal { Q } = ( \Omega , \Sigma , Q )$ , or possibly $ { \mathrm { \Omega } } _ { \mathrm { i n } }  { \mathrm { \Omega } } ,$ some other system based on another weighting of the coins. 

Exercise 4.4 What is the probability in the system that there are exactly two heads? What about in the system $\boldsymbol { \mathcal { Q } } \boldsymbol { \ell }$ 

## 4.4 Random Variables

The final concept that we want to think about is that of a ‘real-valued function’ X defined on the sample space Ω. Thus $X : \Omega  \Re$ assigns to each element $\omega _ { i }$ of $\Omega$ an element of $\Re ,$ that is, a real number. We call such a function a random variable. Even though the function is itself deterministic, that is, if we give X a definite input then we get a definite output, its argument $\omega _ { i }$ is the random outcome of our physical experiment and hence $X ( \omega _ { i } )$ is also random. For example, X could be the function that counts the numbers of heads, 

$$
\begin{array}{r c l} X (\{H H H \}) & = & 3 \\ X (\{H H T \}) & = & X (\{H T H \}) = X (\{T H H \}) = 2 \\ X (\{H T T \}) & = & X (\{T T H \}) = X (\{T H T \}) = 1 \\ X (\{T T T \}) & = & 0. \end{array}\tag{4.4}
$$

As a second example, X could be twice the diference between the number of heads and the number of tails; or as a third example X could be 1 for the element HHH and 0 for all the other elements of Ω. While these are all diferent functions, they do have one important thing in common: they are defined independently of any probability measure. That is, they depend on the ‘possibility system’ $( \Omega , \Sigma )$ , but not on a particular probability system (Ω, Σ, P). Thus we could change probability measures from $P$ to $Q .$ , and the values of X would be unafected. 

However, what would be afected by a change of probability measure is the probability that X would take on some given value. In particular the expectation of X, which is the probability weighted sum over the sample space of the possible values of the random variable, will depend on the probability measure that we are using. This is obvious from the formula for the expectation, 

$$
\begin{array}{r c l} E ^ {\mathcal {P}} [ X ] & = & \sum_ {i = 1} ^ {n} P (\{\omega_ {i} \}) X (\omega_ {i}) \\ & = & \sum_ {i = 1} ^ {n} p _ {i} X (\omega_ {i}), \end{array}\tag{4.5}
$$

which clearly depends in a crucial way on the probability measure. The notation $E ^ { \mathcal { P } } [ X ]$ is used to denote the expectation of the random variable X with respect to the probability system $\mathcal { P }$ . 

Going back to our example, suppose that we are in the ‘fair-coin’ probability system $\mathcal { P }$ . Then the expectation of the random variable X that returns the number of heads is 

$$
E ^ {\mathcal {P}} [ X ] = 1. 5,\tag{4.6}
$$

while in the unfair ‘weighted-coin’ system $\mathcal { Q } ,$ the expectation is 

$$
E ^ {\mathcal {Q}} [ X ] = 1.\tag{4.7}
$$

So we have explicitly verified that the expectation of a random variable depends on the probability system that we are using. If it is obvious which possibility system that we are ‘in’, then we will talk about expectation with respect to the relevant probability measure P, rather than with respect to the probability system $\mathcal { P } = ( \Omega , \Sigma , P )$ 

Exercise 4.5 Verify the expectation values calculated above in equations 4.6 and 4.7 . Calculate the expected values for the other two random variables described in the text for both  and $\mathcal { Q }$ 

## 5 Back to the Casino

In this chapter we want to look at two things relating to the Casino. First, we want to use the results of the previous chapter on probability systems to interpret the derivative pricing result of chapter 3, and second, we want to add in a non-zero interest rate. A non-zero interest rate afects the hedging of the bet because it means that we have to pay in order to borrow money to construct a hedged bet. This added cost must be added to the derivative price in order to ensure that no arbitrage is possible. 

## 5.1 The Casino as a Probability System

We begin by using the results of chapter 4 to describe the Casino as a probability system. The sample space Ω is simply the set of the two possible events, H, T . The event space is the power set of this, $\Sigma = \{ \emptyset , \{ H \} , \{ T \} , \Omega \}$ These two sets define the ‘possibility’ system, (Ω, Σ). The payof function $S _ { t }$ for a basic bet is a random variable defined on the possibility system, as is any arbitrary derivative payof function $f _ { t } ( S _ { t } )$ 

As shown in exercise 4.3, we can uniquely define a probability measure by its action on the sample space. We therefore can define the ‘physical’ probability measure P by 

$$
P [ \{H \} ] = p \quad \mathrm{and} \quad P [ \{T \} ] = q.\tag{5.1}
$$

What is it that this measure describes? Very simply it tells us the actual or physical probability of the coin toss being heads or tails. However, a key point of the derivative calculation was that the initial price of a derivative bet does not involve these physical probability values. That is why the expectation hypothesis fails. However, we can define a probability measure related to the derivative pricing formula. 

## 5.2 The Risk-Neutral Measure

Recall that in chapter 3 we found that the price of a derivative bet based on the ‘no arbitrage’ valuation is given by the formula 

$$
f _ {0} = p ^ {*} f _ {t} (U) + q ^ {*} f _ {t} (D),\tag{5.2}
$$

where 

$$
p ^ {*} = \frac {S _ {0} - D}{U - D} \quad \text { and } \quad q ^ {*} = \frac {U - S _ {0}}{U - D}.\tag{5.3}
$$

The first thing to note is that $p ^ { * }$ and $q ^ { * }$ satisfy $p ^ { * } , q ^ { * } \geq 0$ and $p ^ { * } + q ^ { * } = 1$ This means that we can define a probability measure $P ^ { * }$ by 

$$
P ^ {*} [ \{H \} ] = p ^ {*} \quad \text { and } \quad P ^ {*} [ \{T \} ] = q ^ {*},\tag{5.4}
$$

and hence a probability system $\mathcal { P } ^ { * } = ( \Omega , \Sigma , P ^ { * } )$ . When calculating expectations in the ${ \mathcal { P } } ^ { * }$ system we will abbreviate the notation by writing $E ^ { * }$ instead of $E ^ { \mathcal { P } ^ { \ast } }$ . Note that the probability measure $P ^ { * }$ has nothing to do with the ‘physical’ probability measure $P _ { - }$ 

Suppose that we take the expected value of the derivative payof function with respect to the ${ \mathcal { P } } ^ { * }$ probability system. This yields 

$$
\begin{array}{r c l} E ^ {*} [ f _ {t} (S _ {t}) ] & = & p ^ {*} f _ {t} (U) + q ^ {*} f _ {t} (D) \\ & = & f _ {0}. \end{array}\tag{5.5}
$$

In other words, the value of the derivative is given by the expectation of its payof function with respect to the new probability system ${ \mathcal { P } } ^ { * }$ 

Moreover, in the special case when the derivative payof function is simply the standard bet $f _ { t } ( S _ { t } ) = S _ { t }$ , we see that 

$$
\begin{array}{r c l} E ^ {*} [ f _ {t} (S _ {t}) ] & = & E ^ {*} [ S _ {t} ] \\ & = & p ^ {*} U + q ^ {*} D \\ & = & \frac {S _ {0} - D}{U - D} U + \frac {U - S _ {0}}{U - D} D \\ & = & S _ {0}. \end{array}\tag{5.6}
$$

We already know, of course, that the value of a derivative that pays of $S _ { t }$ dollars at time t is by definition $S _ { 0 }$ dollars. This is simply a statement of the Casino rule that the basic stake of $S _ { 0 }$ dollars pays of $S _ { t }$ dollars. But now we see that 

$$
S _ {0} = E ^ {*} [ S _ {t} ].\tag{5.7}
$$

In other words, the new probabilities $p ^ { * }$ and $q ^ { * }$ are precisely the ‘physical weightings’ that the coin must have if the stake $S _ { 0 }$ were equal to its expected value at time t. If this is the case then the expectation hypothesis actually gives the correct price for derivatives! 

We can interpret the ${ \mathcal { P } } ^ { * }$ probability system in terms of the amount of risk that a player is willing to take. If a player has no preference whether he (a) holds onto his initial stake of $S _ { 0 }$ dollars, or (b) bets it with an expected return of $E [ S _ { t } ]$ dollars, then the two strategies must have the same value to him, that is, $S _ { 0 } = E [ S _ { t } ]$ . Such players are called risk-neutral, or risk-indiferent and expect that if they play many times, they will neither gain nor lose money. For risk-neutral players to bet, the actual coin probabilities must be $p = p ^ { * }$ and $q = q ^ { * }$ . Thus, we call the probability measure $P ^ { * }$ the risk-neutral measure and the probability system $\mathcal { P } ^ { * } = ( \Omega , \Sigma , P ^ { * } )$ the risk-neutral system. 

In reality, we expect that players are either investors, who are by nature risk-averse, only playing if $S _ { 0 } < E [ S _ { t } ]$ , or gamblers, who are risk-preferring, and are willing to play if $S _ { 0 } > E [ S _ { t } ]$ (which corresponds to a risk-averse Casino). 

## 5.3 A Non-Zero Interest Rate

Suppose that the Casino bank begins to charge interest on borrowed money at a continuously compounded rate r. Similarly, it pays interest on deposits at the same rate. As in the foreign exchange example of chapter 2, the value of the interest rate will afect the derivative price. We therefore need to find the new value for the purchase price $f _ { 0 }$ of a derivative, again by using a no arbitrage argument. 

Consider the following scenario for a dealer who starts with nothing. At time 0 he sells a derivative with payof function $f _ { t } ( S _ { t } )$ to a gambler. He receives $f _ { 0 }$ dollars for selling the derivative and then hedges it by making a basic bet of $\delta S _ { 0 }$ dollars with the Casino. As in the zero interest rate case, the dealer wants his payout to be independent of the outcome of the coin toss, so he picks $\delta$ such that $\delta U - f _ { t } ( U ) = \delta D - f _ { t } ( D )$ . Solving this equation for the hedge ratio we find that is still given by equation (3.7) 

$$
\delta = \frac {f _ {t} (U) - f _ {t} (D)}{U - D},\tag{5.8}
$$

and therefore is not afected by the presence of a non-zero interest rate. However, the dealer’s basic bet is financed by borrowing $\delta S _ { 0 } - f _ { 0 }$ dollars from the bank at the interest rate r. Note that if $\delta S _ { 0 } - f _ { 0 }$ is negative, then the dealer deposits some money in the bank and gets it back with interest at time t. 

Now that we have described what happens before the coin toss, we need to turn our attention to what happens after it. The dealer gets $\delta S _ { t }$ dollars from the Casino for his basic bet, but has to pay $f _ { t } ( S _ { t } )$ dollars to the player as part of the derivative contract. By the construction of the hedged bet, this amount, $\delta S _ { t } - f _ { t } ( S _ { t } )$ dollars, is a guaranteed quantity. Furthermore, the amount that the dealer owes the Casino bank, $( \delta S _ { 0 } - f _ { 0 } ) e ^ { r t }$ dollars, is also a guaranteed quantity. Hence the dealer’s final position is risk-free. Since he starts with no money, a guaranteed profit would be an arbitrage. This implies that in an arbitrage-free Casino the dealer’s final position must be zero, 

$$
\delta S _ {t} - f _ {t} (S _ {t}) - (\delta S _ {0} - f _ {0}) e ^ {r t} = 0.\tag{5.9}
$$

If we substitute in for the hedge ratio $\delta$ from equation (5.8), then we can solve this equation for $f _ { 0 }$ to obtain 

$$
f _ {0} = e ^ {- r t} [ p ^ {*} f _ {t} (U) + q ^ {*} f _ {t} (D) ],\tag{5.10}
$$

where 

$$
p ^ {*} = \frac {S _ {0} e ^ {r t} - D}{U - D} \quad \mathrm{and} \quad q ^ {*} = \frac {U - S _ {0} e ^ {r t}}{U - D}.\tag{5.11}
$$

We can define the risk-neutral probability measure $P ^ { * }$ for the Casino with non-zero interest rates by setting the probabilities to be 

$$
P ^ {*} [ \{H \} ] = p ^ {*} \quad \text { and } \quad P ^ {*} [ \{T \} ] = q ^ {*}.\tag{5.12}
$$

The derivative price can therefore be written as 

$$
f _ {0} = e ^ {- r t} E ^ {*} [ f _ {t} (S _ {t}) ],\tag{5.13}
$$

where $E ^ { * } [ X ]$ is the expectation of a random variable X using the risk-neutral measure $P ^ { * }$ . This arbitrage argument difers from the zero interest rate case only in the fact that the dealer has to pay interest on the money borrowed to finance the initial hedged bet. The original argument and its values for $f _ { 0 } , p ^ { * }$ and $q ^ { * }$ are recovered if we set $r = 0$ in the above result. 

What is the significance of the factor $e ^ { - r t }$ in the derivative price? We can think of it as follows. If a sure sum of money $X _ { t }$ is to be delivered at time $t ,$ then its present value $X _ { 0 }$ is given by $X _ { 0 } = P _ { 0 t } X _ { t }$ , where $P _ { 0 t }$ is the discount factor. In general, we require that $0 \leq P _ { 0 t } \leq 1$ , and that $P _ { 0 t }$ is a decreasing function of t. For example, if r is a constant and $P _ { 0 t } = e ^ { - r t }$ , then we say that we have constant interest rates. The discount factor arises because of the time-value of money, which takes into account the fact that a fixed amount of money is worth more now than the same amount of money will be in the future. This is because the risk-free interest rate allows the value of an initial amount of money to grow in time. So the factor $e ^ { - r t }$ in the derivative price can be thought of as a discount factor that is applied because the derivative pays out at a time t in the future, rather than at $t = 0$ when it is purchased. 

## Exercise 5.1 Why must $P _ { 0 t }$ be a decreasing function of t?

As we shall see in the following sections, the formula $f _ { 0 } = e ^ { - r t } E ^ { * } [ f _ { t } ( S _ { t } ) ]$ is a good prototype for derivative pricing in general. In words, it says that the present value of a derivative is equal to the discounted value of the risk-neutral expectation of its payof. Note, once again, that to value the derivative we do not need to know the actual probabilities $p$ and $q$ for the results of the coin flip. 

We can verify the price for the special case of a derivative that pays of $f _ { t } ( S _ { t } ) = S _ { t }$ . We have 

$$
\begin{array}{r c l} f _ {0} & = & e ^ {- r t} E ^ {*} [ S _ {t} ] \\ & = & e ^ {- r t} (p ^ {*} U + q ^ {*} D) \\ & = & e ^ {- r t} \left(\frac {S _ {0} e ^ {r t} - D}{U - D} U + \frac {U - S _ {0} e ^ {r t}}{U - D} D\right) \\ & = & S _ {0}. \end{array}\tag{5.14}
$$

This shows that a derivative that has the same payofs as the basic bet also has the same initial price. 

Exercise 5.2 In the case where there is an interest rate r, show how an arbitrageur can still make a profit without risk if the dealer mispriced the derivative. 

Exercise 5.3 Suppose that the basic stake is $100, while the basic payofs are $105 and $95, for heads and tails respectively, and $e ^ { r t } = 1 . 0 1$ . The actual probabilities of heads and tails are $p = . 8$ and $q = . 2$ 

(a) Calculate the risk-neutral probabilities $p ^ { * }$ and $q ^ { * }$ . 

(b) Calculate the price of a derivative that pays of the value 5 for heads and nothing for tails. This is really a call option with a strike of $100. 

(c) What is the value of the hedge ratio δ? 

(d) Verify that the payof of a bet consisting of being long δ units of the basic bet, and short one derivative is independent of the coin toss. 

(e) What is the price of the derivative if the actual probabilities of heads and tails are $p = 0 . 3$ and $q = 0 . 7 \%$ 

Why do people gamble? Surely the answer must be that, despite losses on average in cash terms, there is an implicit benefit—that is, an intangible yield in the form of (say) pleasure, a fun evening out, interesting company, the thrill of living dangerously, satisfaction of an uncontrollable urge, or something along these lines. For fear of lapsing into a state of arm-chair psychology, let us not say more on this. The implicit benefit obtained in this way is formalised in the concept of a convenience yield. It is possible to price derivatives using a particular convenience yield but this method sufers from the fact that every player will have a diferent yield, and so no scheme that will satisfy every gambler is possible. The advantage of arbitrage pricing is that it is independent of the wishes or views of the players, and therefore can be uniquely defined. 

Summing up, we have seen here that the value of a derivative in the Casino is given by the discounted risk-neutral expectation of its payof function, $f _ { 0 } = e ^ { - r t } E ^ { * } [ f _ { t } ( S _ { t } ) ]$ , where $P ^ { * }$ is the unique system of probabilities such that $S _ { 0 } = e ^ { - r t } E ^ { * } [ S _ { t } ]$ These relations were derived by applying the no arbitrage condition to a hedged and hence risk-free bet. 

Exercise 5.4 Verify that the risk-neutral measure $P ^ { * }$ , defined by equation $\left( 5 . 1 1 \right)$ , is the unique probability measure that satisfies $S _ { 0 } = e ^ { - r t } E ^ { * } [ S _ { t } ]$ , that is, the basic bet is equal to its discounted expectation. 

## 6 The Binomial Model

We return once more to the Casino, but this time we give it a diferent interpretation: as a simple idealisation of a stock market. The ‘stake’ $S _ { 0 }$ at time 0 is now interpreted as the price of an asset. One can think of this as a ‘chip’ or ‘one share’. As a consequence of the ‘coin flip’, which represents a random movement in the stock price, the asset is worth either more $( S _ { 1 } = U )$ , or less $( S _ { 1 } = D )$ at $t = 1$ . Thus, we have a very elementary model for a ‘stock market’, in this case a ‘one-period’ market, since there is only one time step. In this chapter we shall expand this model and give the definition and construction of n-period markets before pricing derivatives in a one-period market. In the next chapter we turn our attention to the value of derivatives in an n-period market. The techniques that we introduce here, although very elementary in nature, have wide applications. 

## 6.1 Tree Models

In order to deal with a more complex system than the simple one-period market, we need to refine our current notation. Our convention will be to use a subscript for the time variable, and a superscript to indicate the state of the share price. Thus, initially the share price is $S _ { 0 }$ (there is only one state, so we don’t need a superscript). At time 1 we have two states, so we write $S _ { 1 } ^ { i }$ , where $i = 0 ,$ 1, as shown below: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/e4bfc88084b5a688b000e8d6883c7a4039fe23fb1e6e91aa52e94ac9ad2563cc.jpg)


(6.1) 

Now we suppose that at time 2 each of the states $S _ { 1 } ^ { i }$ can evolve to a pair of new states which we write as $S _ { 2 } ^ { i j }$ . The first index tells you which state you were in at time 1, while the second index tells you whether you have an up or down move following that, as illustrated in the following diagram: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/98cf7a8994fd0a0d5d1d3f8498be7040cf36fc46de8e68a13e962c70cc7ce233.jpg)


(6.2) 

The resulting system of prices is called a tree model. For simplicity, we shall consider trees which have two branches at each node, but in principle the idea can be extended to the situation where we have any number of branches at each node. We can display the system more compactly by suppressing the branches and writing, for example, 

$$
S _ {0} \longrightarrow S _ {1} ^ {i} \longrightarrow S _ {2} ^ {i j} \longrightarrow S _ {3} ^ {i j k},\tag{6.3}
$$

for a three-period model. Note that by simply changing the allowed range for the superscripts, this notation is general enough for any number of branches. 

We also need to introduce notation for the probabilities with which the various transitions occur. In compact form this is 

$$
S _ {0} \xrightarrow {p _ {0} ^ {i}} S _ {1} ^ {i} \xrightarrow {\hat {p} _ {1} ^ {i j}} S _ {2} ^ {i j} \xrightarrow {\hat {p} _ {2} ^ {i j k}} S _ {3} ^ {i j k}.\tag{6.4}
$$

Thus, $p _ { 0 } ^ { 1 }$ is the probability that $S _ { 0 }$ will drop to $S _ { 1 } ^ { 1 }$ . The corresponding tree representation is given explicitly as follows: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/d06ea55442eeadd53d7f20d48d0caf54dd7026883a7e2bd4695cb87b5e83d719.jpg)


(6.5) 

Note that $p _ { 0 } ^ { i }$ gives the probability that $S _ { 1 } = S _ { 1 } ^ { i }$ , while $\hat { p } _ { 1 } ^ { i j }$ is the conditional probability that $S _ { 2 } = S _ { 2 } ^ { i j }$ , given that $S _ { 1 } = S _ { 1 } ^ { i }$ . We will use a ‘hat’ throughout the book to denote conditional probabilities. The actual probability that $S _ { 2 } = S _ { 2 } ^ { i j } { \mathrm { \ i s \ } } p _ { 0 1 } ^ { i j } = p _ { 0 } ^ { i } { \hat { p } _ { 1 } ^ { i j } }$ . Since the total probability at any node must be one, we have $\begin{array} { r } { \sum _ { i } p _ { 0 } ^ { i } = 1 , \sum _ { j } \hat { p } _ { 1 } ^ { i j } = 1 , \sum _ { k } \hat { p } _ { 3 } ^ { i j k } = 1 } \end{array}$ , and so on. This notation means P<sub>that if we sum</sub> $\hat { p } ^ { i j }$ P P<sub>over j for any fixed value of</sub> $i ,$ then the result is one, with the analogous generalisation to the sum of conditional probabilities at later times. 

When convenient, we can drop the ‘time’ subscript from the share prices because the time is simply equal to the number of ‘state’ indices. This yields the less cluttered tree representation shown below: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/68b290bfacc9dc3e19d14cc6f1cb0230e99ee96ecf0e4509005826ea2e5ff22d.jpg)


(6.6) 


The corresponding compact notation is


$$
S \xrightarrow {p ^ {i}} S ^ {i} \xrightarrow {\hat {p} ^ {i j}} S ^ {i j} \xrightarrow {\hat {p} ^ {i j k}} S ^ {i j k}.\tag{6.7}
$$

## 6.2 Money Market Account

We have already considered the notion of borrowing in the Casino at a nonzero interest rate. Now we need to formalise this idea further by introducing the concept of a money market process that accumulates interest on a riskfree basis. Let $B _ { t }$ denote the value of the money market account at time t. For brevity, we shall sometimes refer to a unit in the money market account as a ‘bond’, hence the notation $B _ { t }$ , which might also be taken to stand for ‘bank account’. Assuming that the interest rate is deterministic, then the process is simply the linear tree: 

$$
B _ {0} \longrightarrow B _ {1} \longrightarrow B _ {2} \longrightarrow B _ {3}.\tag{6.8}
$$

If interest rates are constant, then, as we proved in exercise 1.3, the value of the money market account is 

$$
B _ {t} = B _ {0} e ^ {r t},\tag{6.9}
$$

where r is the interest rate ‘per period’, expressed on a continuously compounded basis. For example, if R is the annualised continuously compounded interest rate, and if time is counted in days, then $r = R / 3 6 5$ . We will not necessarily assume that interest rates are constant, but merely that they are positive, so $B _ { t + 1 } > B _ { t }$ that is, the bank account increases in value. 

Buying a unit of the money market account at time t for the price $B _ { t }$ is like ‘putting the amount $B _ { t }$ in the bank’. At time $t + 1$ it is worth a larger amount $B _ { t + 1 }$ . Selling a unit of the money market account for the price $B _ { t }$ at time t is like ‘borrowing the amount $B _ { t } { ' }$ from the bank. If you want to buy it back again at time $t + 1$ , that is, repay the loan, then you must pay $B _ { t + 1 }$ for it—principal plus interest. 

## 6.3 Derivatives

For a derivative we need to specify (a) the maturity date t, that is, the time when it pays of, and (b) the payof function $f .$ . It is convenient to think of the payof as being determined by the state of the market at the payof time, so $f = f _ { t } ( S _ { t } )$ . For example, a derivative that pays of at $t = 2$ will have a payof function $f ^ { i j } = f ( S ^ { i j } )$ . Specification of the payof function is part of the derivative contract, so the real problem is to determine the present value, or initial cost f of the derivative. Indeed, since a derivative itself can be viewed as an asset, we can express its time evolution in either the compact form, 

$$
f \longrightarrow f ^ {i} \longrightarrow f ^ {i j} \longrightarrow f ^ {i j k},\tag{6.10}
$$

or as the following tree: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/4b1630faf97edde5685370437521188d4f6bc0faba7fd4cf49dd74b3180c6ae0.jpg)


(6.11) 

In order to make the derivative calculations somewhat more tangible, it is worth considering some sample numerical exercises. A hypothetical share price process is given as follows: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/f4a8f08e04aaf0051db029c1062b2bb4786b33f16eac2a95a36f491ea58734d3.jpg)


(6.12) 

For the money market account, we will assume a flat rate of 1% per month, so the process can be represented by the diagram 

$$
1 0 0 \longrightarrow 1 0 1 \longrightarrow 1 0 2. 0 1,\tag{6.13}
$$

where each time step is one month. 

Exercise 6.1 In the given hypothetical two-period stock market what are the probabilities that (a) $S _ { 2 } = 1 0 2$ and (b) $\mathit { S } _ { 2 } > 9 5 ?$ 

Exercise 6.2 What is the value of r for the money market process given by equation (6.13), assuming that the interest is continuously compounded at an annualized rate $r ?$ 

Exercise 6.3 Using what you have learned in chapter 3, calculate the values of call options with a maturity of $t = 1$ and strike prices of $98 and $102. How much would similar derivative costs if you bought them at time 1 for exercise at time 2? Note that in this case you need to calculate two prices for each call option, one in the event that $S _ { 1 } = 1 0 5$ and one for the case when $S _ { 1 } = 9 5$ . Finally, how much would you be willing to pay at time 0 for the call options with a maturity of $t = 2 \ell$ 

## 6.4 One-Period Replication Model

We now want to price the derivative by using a no arbitrage argument. As in the case of the Casino analogy, the investor will buy a derivative from a trader, who will then take the proceeds of this sale and invest in the stock and money market so that the randomness in his stock and derivative positions cancel. By hedging in this way, the trader can obtain a guaranteed payof when the derivative expires, at which point he collects the proceeds from his stock and money market positions and pays the investor any money due on the derivative. By the no arbitrage condition, this guaranteed payout must be zero, since the trader started with nothing. If it were less than zero, the trader wouldn’t trade; whereas if it were more than zero, then the investor wouldn’t invest. 

To actually calculate the initial price of a derivative, we now need to turn these words into equations. Hence, suppose that we have a trader with no initial position and an investor that is flush with cash. At time 0 the investor buys a derivative with payof $f ^ { i }$ at $t = 1$ from the trader. The investor pays $f$ dollars, the value of the derivative at $t = 0$ , to the trader, who then uses the money to take a position in the stock S and the money market account B. Let $\beta$ be the number (possibly fractional, possibly negative) of units in the money market account that the trader buys, and $\delta$ the number of units in the stock S. Since this purchase is entirely funded by the money received from the sale of the derivative, we have 

$$
f = \beta B + \delta S.\tag{6.14}
$$

How does the trader choose the values of $\beta$ and $\delta ?$ Well, his position at time 1 is equal to the value of his stock and bond portfolio $\beta B ^ { i } + \delta S ^ { i }$ , minus the derivative payment $f ^ { i }$ that he must make to the investor, and most importantly, the trader would like this amount to be risk-free. By the no arbitrage condition, the value of this position must be zero, that is, 

$$
\beta B ^ {i} + \delta S ^ {i} - f ^ {i} = 0,\tag{6.15}
$$

or 

$$
f ^ {i} = \beta B ^ {i} + \delta S ^ {i}.\tag{6.16}
$$

Because the bond and stock portfolio exactly duplicates the payof function of the derivative, we call it a replicating strategy. The existence of a replicating strategy means that the derivative can be constructed from the underlying assets and hence an investor need never buy the derivative—he can do just as well by taking positions in stocks and bonds. In the real world, however, a derivative has lower transaction and maintenance costs and that is why investors will purchase them. 

Since equation (6.16) must hold independent of the ‘up’ or ‘down’ movement of the share price, we must have 

$$
f ^ {0} = \beta B _ {1} + \delta S ^ {0} \quad \mathrm{and} \quad f ^ {1} = \beta B _ {1} + \delta S ^ {1}.\tag{6.17}
$$

We can then solve these two equations for $\beta$ and $\delta _ { : }$ 

$$
\beta = \frac {f ^ {1} S ^ {0} - f ^ {0} S ^ {1}}{B _ {1} (S ^ {0} - S ^ {1})} \quad \text { and } \quad \delta = \frac {f ^ {0} - f ^ {1}}{S ^ {0} - S ^ {1}},\tag{6.18}
$$

where we have assumed that $S ^ { 0 } > S ^ { 1 }$ . Substituting these expressions back into equation (6.14) we obtain 

$$
f = \frac {f ^ {1} S ^ {0} - f ^ {0} S ^ {1}}{B _ {1} (S ^ {0} - S ^ {1})} B + \frac {f ^ {0} - f ^ {1}}{S ^ {0} - S ^ {1}} S,\tag{6.19}
$$

which completely determines the value of the derivative. Rearranging this expression, we get 

$$
f = \frac {S - S ^ {1} \frac {B}{B _ {1}}}{S ^ {0} - S ^ {1}} f ^ {0} + \frac {S ^ {0} \frac {B}{B _ {1}} - S}{S ^ {0} - S ^ {1}} f ^ {1},\tag{6.20}
$$

or alternatively 

$$
f = \frac {B}{B _ {1}} \left[ \frac {S \frac {B _ {1}}{B} - S ^ {1}}{S ^ {0} - S ^ {1}} f ^ {0} + \frac {S ^ {0} - S \frac {B _ {1}}{B}}{S ^ {0} - S ^ {1}} f ^ {1} \right].\tag{6.21}
$$

Exercise 6.4 Compare the derivative price equation (6.21) with the Casino price equation (5.13). Show that they are equivalent. 

## 6.5 Risk-Neutral Probabilities

As in the Casino example, we see that the derivative price, given by equation (6.21), is independent of the ‘physical’ probabilities $p ^ { i }$ . Instead of the physical probabilities, we want to define the risk-neutral probability measure $P ^ { * }$ generated by the probabilities 

$$
p _ {*} ^ {0} = \frac {\tilde {S} - S ^ {1}}{S ^ {0} - S ^ {1}} \quad \text {and} \quad p _ {*} ^ {1} = \frac {S ^ {0} - \tilde {S}}{S ^ {0} - S ^ {1}},\tag{6.22}
$$

where $\begin{array} { r } { \tilde { S } = \frac { B _ { 1 } } { B } S } \end{array}$ 

Exercise 6.5 Verify that the probabilities $p _ { * } ^ { 0 }$ and $p _ { * } ^ { 1 }$ do generate a valid probability measure. 

The initial price of the derivative can therefore be written as 

$$
\begin{array}{r c l} {f} & {=} & {\frac {B}{B _ {1}} [ p _ {*} ^ {0} f ^ {0} + p _ {*} ^ {1} f ^ {1} ]} \\ & {=} & {\frac {B}{B _ {1}} E ^ {*} [ f _ {1} ],} \end{array}\tag{6.23}
$$

where $f _ { 1 }$ is the random payof of either $f ^ { 0 }$ or $f ^ { 1 }$ at time 1 and $E ^ { * } [ - ]$ is the expectation with respect to the risk-neutral measure $P ^ { * }$ . Since B and $B _ { 1 }$ are deterministic, the derivative pricing formula (6.23) can be expressed in the form 

$$
{\frac {f}{B}} = E ^ {*} [ \frac {f _ {1}}{B _ {1}} ].\tag{6.24}
$$

In other words, the ratio $f / B$ of the present value of the derivative to the initial cost of the money market account is given by the risk neutral expectation of this ratio at $t = 1$ 

But in what sense is this new probability system ‘risk-neutral’ ? We need to verify that the probabilities $p _ { * } ^ { i }$ are indeed the probabilties that would apply in reality if investors were really ‘indiferent’, that is, neutral to risk. In this situation (risk indiference) investors would expect the same rate of return (average profitability per unit investment) on both (a) an investment in the stock market, and (b) an investment in a money market account. In equation form, this means that 

$$
\frac {E ^ {*} [ S _ {1} ]}{S _ {0}} = \frac {E ^ {*} [ B _ {1} ]}{B}.\tag{6.25}
$$

Note that $B _ { t }$ is actually deterministic, so $E ^ { * } [ B _ { 1 } ] = B _ { 1 }$ . After expanding $E ^ { * } [ S _ { 1 } ]$ in terms of the risk-neutral probabilities, we have 

$$
\frac {S ^ {0} p _ {*} ^ {0} + S ^ {1} p _ {*} ^ {1}}{S _ {0}} = \frac {B _ {1}}{B},\tag{6.26}
$$

where $p _ { * } ^ { 0 } + p _ { * } ^ { 1 } = 1$ . These relation imply, after a short calculation, that 

$$
p _ {*} ^ {0} = \frac {\tilde {S} - S ^ {1}}{S ^ {0} - S ^ {1}} \quad \text {and} \quad p _ {*} ^ {1} = \frac {S ^ {0} - \tilde {S}}{S ^ {0} - S ^ {1}},\tag{6.27}
$$

where 

$$
\tilde {S} = S \frac {B _ {1}}{B},\tag{6.28}
$$

which is the same result as equation (6.22). This verifies the interpretation of the probabilities $p _ { * } ^ { i }$ as risk-neutral. 

Exercise 6.6 Calculate the forward price at time 0 for the purchase at time 1 of one share. 

## 7 Pricing in N-Period Tree Models

Equation (6.21) completely determines the price of a derivative in a oneperiod market. So it is clearly time to expand our model and think about something a little more complicated! Consider a two-period market with a stock, a money market account, and a derivative. We know the values in the stock process, as illustrated in (6.6), and in the bond process, shown in (6.8). We also know the terminal values or payof of the derivative process $f ^ { i j }$ , that is, the final values of the tree (6.11). Our goal is to use a no arbitrage argument to compute the rest of the derivative process, including, in particular, its present value $f _ { 0 }$ , that is, today’s price. 

From the work that we have done on the one-period model, it should be clear that if we determine the possible values $f ^ { 0 }$ and $f ^ { 1 }$ of the derivative at time 1, then we can determine its value at time 0 by use of equation (6.24). Now consider the situation at time 1, and suppose that the outcome of the first period was an upward movement (‘heads’), so $S \to S ^ { 0 }$ . Then the stock has value $S ^ { 0 }$ , the bond has value $B _ { 1 }$ , and we must find the value $f ^ { 0 }$ of a derivative that pays of either $f ^ { 0 0 }$ or $f ^ { 0 1 }$ depending on whether $S ^ { 0 } \to S ^ { 0 0 }$ or $S ^ { 0 }  S ^ { 0 1 }$ . But clearly the problem now posed is formally identical to the original problem for a one-period derivative, as we can see from the relevant tree diagrams: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/92985deb498d54a9eb31a5d8cab92e3d737d9c8263e0c3f727f1aad908b497dd.jpg)


(7.1) 


We might call this realization an ‘inductive insight’. Since we can price derivatives in a one-period model using equation (6.21), we can determine the value of $f ^ { 0 }$ by simply using the same formula.


So, using equations (6.22) and (6.24) we can immediately write down the solution in the form 

$$
\frac {f ^ {0}}{B _ {1}} = \frac {f ^ {0 0} \hat {p} _ {*} ^ {0 0} + f ^ {0 1} \hat {p} _ {*} ^ {0 1}}{B _ {2}},\tag{7.2}
$$

where 

$$
\hat {p} _ {*} ^ {0 0} = \frac {\tilde {S} _ {1 2} ^ {0} - S ^ {0 1}}{S ^ {0 0} - S ^ {0 1}}, \quad \hat {p} _ {*} ^ {0 1} = \frac {S ^ {0 0} - \tilde {S} _ {1 2} ^ {0}}{S ^ {0 0} - S ^ {0 1}},\tag{7.3}
$$

and $\tilde { S } _ { 1 2 } ^ { 0 } = S ^ { 0 } B _ { 2 } / B _ { 1 }$ is the conditioned forward price made at time 1, when the stock has value $S ^ { 0 } \ \mathrm { ( ^ { \circ } u p ) } ^ { \prime }$ state) for delivery of a share at time 2. More generally, the random variable ${ \tilde { S } } _ { 1 2 }$ is is the forward price that will be made at time 1 for purchase of a share at time 2. It can take on two values, ${ \tilde { S } } _ { 1 2 } ^ { i }$ , $( i = 0 , 1 )$ depending on the actual value $S ^ { i }$ of the stock at time 1. 

Exercise 7.1 Use an arbitrage argument to show that if $S _ { 1 } = S _ { 1 } ^ { 0 }$ at time t = 1, then the value of the derivative must be $f ^ { 0 }$ , as given in equation (7.2). 

Similarly for $f ^ { 1 }$ , equations (6.22) and (6.24) tell us that 

$$
\frac {f ^ {1}}{B _ {1}} = \frac {f ^ {1 0} \hat {p} _ {*} ^ {1 0} + f ^ {1 1} \hat {p} _ {*} ^ {1 1}}{B _ {2}},\tag{7.4}
$$

where 

$$
p _ {*} ^ {1 0} = \frac {\tilde {S} _ {1 2} ^ {1} - S ^ {1 1}}{S ^ {1 0} - S ^ {1 1}}, \quad p _ {*} ^ {1 1} = \frac {S ^ {1 0} - \tilde {S} _ {1 2} ^ {1}}{S ^ {1 0} - S ^ {1 1}},\tag{7.5}
$$

and $\tilde { S } _ { 1 2 } ^ { 1 } = S ^ { 1 } B _ { 2 } / B _ { 1 }$ is the forward price made at time 1, when the stock has value $S ^ { 1 }$ , for delivery and payment at time 2. 

But now we know $f ^ { 0 }$ and $f ^ { 1 }$ . Thus, we can substitute these values back into equation (6.24) to obtain the initial price of the derivative, given by 

$$
\begin{array}{r c l} \frac {f}{B} & = & \frac {f ^ {0} p _ {*} ^ {0} + f ^ {1} p _ {*} ^ {1}}{B _ {1}} \\ & = & \frac {f ^ {0 0} p _ {*} ^ {0} \hat {p} _ {*} ^ {0 0} + f ^ {0 1} p _ {*} ^ {0} \hat {p} _ {*} ^ {0 1} + f ^ {1 0} p _ {*} ^ {1} \hat {p} _ {*} ^ {1 0} + f ^ {1 1} p _ {*} ^ {1} \hat {p} _ {*} ^ {1 1}}{B _ {2}} \\ & = & \frac {f ^ {0 0} p _ {*} ^ {0 0} + f ^ {0 1} p _ {*} ^ {0 1} + f ^ {1 0} p _ {*} ^ {1 0} + f ^ {1 1} p _ {*} ^ {1 1}}{B _ {2}}, \end{array}\tag{7.6}
$$

where we have used the fact that $p _ { * } ^ { i } \hat { p } _ { * } ^ { i j } = p _ { * } ^ { i j }$ is the risk-neutral probability that $S$ goes to $S ^ { i j }$ . Thus, we see that the final equation is an expectation in the risk-neutral measure, 

$$
\frac {f}{B} = E ^ {*} \left[ \frac {f _ {2}}{B _ {2}} \right],\tag{7.7}
$$

where $f _ { 2 }$ is the random payof of the derivative at time 2. 

The financial interpretation of this result is that the probabilities $p _ { * } ^ { i }$ and $\hat { p } _ { * } ^ { i j }$ yield the unique probability system such that the expected return from an investment in the money market account equals the expected return if the money were put in the stock market instead. Thus, 

$$
\frac {B _ {1}}{B _ {0}} = \frac {E ^ {*} [ S _ {1} ]}{S _ {0}} \quad \mathrm{and} \quad \frac {B _ {2}}{B _ {0}} = \frac {E ^ {*} [ S _ {2} ]}{S _ {0}}\tag{7.8}
$$

Exercise 7.2 Verify that the relations given in equation (7.8) hold. Do these conditions uniquely define a probability measure? 

Exercise 7.3 Calculate the risk-neutral probabilities for the numerical example illustrated in 6.12. Price the following derivatives: 

(a) $f ^ { i j } = S ^ { i j }$ , i.e., the derivative simply pays of the value of the stock. 

(b) A forward contract with a strike price of $100. 

(c) A European call option with a strike of $100. 

(d) A European put option with a strike of $100. 

(e) A call option that expires at t = 1 with a strike of $3 on a forward contract with a strike price of $100. 

(f) A derivative that pays out the diference if the share price falls below $97, summed over both time periods. That is, the payof function is max $[ 9 7 - S _ { 2 } , 0 ] + \operatorname* { m a x } [ 9 7 - S _ { 1 } , 0 ]$ dollars. This is a ‘path-dependent’ derivative because the final payout depends on the entire path that the share price takes, rather than just its final value. 

(g) A digital contract that pays out $10 if the share price is above $100. 

(h) Both a European and an American call option with strikes of $104. 

Exercise 7.4 Compute the entire system of risk-neutral probabilties $p _ { * } ^ { i }$ , $\hat { p } _ { * } ^ { i j }$ and $\hat { p } _ { * } ^ { i j k }$ for a three-period binomial model. 

So what have we learned about pricing in the tree model so far? We have shown that in a one-period market, a derivative is priced according to the rule 

$$
\frac {f _ {0}}{B _ {0}} = \frac {E ^ {*} [ f _ {1} ]}{B _ {1}},\tag{7.9}
$$

while in a two-period market we used this result inductively to deduce that 

$$
\frac {f _ {0}}{B _ {0}} = \frac {E ^ {*} [ f _ {2} ]}{B _ {2}}.\tag{7.10}
$$

Moreover, in an N-period binomial market model, a ‘backward induction’ argument can be made that the price of a derivative $f _ { 0 }$ at $t = 0$ with random payout $f _ { N }$ at $t = N$ is given by 

$$
\frac {f _ {0}}{B _ {0}} = \frac {E ^ {*} [ f _ {N} ]}{B _ {N}}\tag{7.11}
$$

where $B _ { N }$ is the value of the money market account at $t = N$ ， $f _ { N }$ is the random value of the derivative at time N, and $E ^ { * } [ - ]$ is the expectation in the risk-neutral measure determined by use of the one-period relation (6.22) at each node of the tree. 

Exercise 7.5 Verify equation (7.11) explicitly in the case of a three-period market. 

Exercise 7.6 Complete the backwards induction argument to prove equation (7.11). 

## 8 Martingales and Conditional Expectation

We are now at a point where we have an algorithm that can be used to evaluate the initial price of any derivative with a known payof function. Before proceeding further, we want to formalise some of the probabilistic concepts that we have been dealing with and which will reappear in the continuous time setting. Instead of the coin tosses considered in section 4 we will use the two-period tree model as the underlying ‘random’ experiment. The sample space is 

$$
\Omega = \{U U, U D, D D, D U \},\tag{8.1}
$$

where U indicates an ‘up’ movement in the stock market and D a ‘down’ one. We assume that the event space Σ is the power set of Ω. The share price $S _ { 2 }$ at time 2 is a random variable that takes the values $S ^ { i j }$ depending on the up and down movements in the markets. How about the share price $S _ { 1 }$ at an earlier time 1? It is also a random variable defined on the same sample space, but unlike $S _ { 2 }$ , it should not depend on the movements of the market after time 1. This means that $S _ { 1 } ( U U ) = S _ { 1 } ( U D )$ and $S _ { 1 } ( D D ) = S _ { 1 } ( D U )$ This discussion has illustrated the two concepts that we want to discuss next: stochastic processes and filtrations. 

## 8.1 Stochastic Processes

The share price process $S _ { i }$ that we have been dealing with so far is really a family of random variables indexed by a time parameter i. That is, there are three random variables $S _ { 0 } , S _ { 1 }$ and $S _ { 2 }$ defined on the sample space Ω. This is an example of a stochastic process. 

Definition 8.1 A stochastic process X is a sequence of random variables $\{ X _ { n } \} _ { n = 1 } ^ { K }$ defined on the sample space Ω. 

## 8.2 Filtration

Suppose that instead of being concerned with only the final outcome of the share price movements, we want to be able to describe the share price at any time before the final time. For example, we could evaluate the share price stochastic process $S _ { i }$ for each time i at the sample space element $U U { \mathrm { : } }$ $S _ { 0 } ( U U ) = S$ at time $0 , S _ { 1 } ( U U ) = S ^ { 0 }$ at time 1 and $S _ { 0 } ( U U ) = S ^ { 0 0 }$ at time 2. Note that at times before the final time, while the sample space is always the same, the elements of it that can be diferentiated from one another may not always be the same. For example, at time 0 it is impossible to tell any of the elements of the sample space apart, so the members of the set 

$$
F _ {0} = \{U U, U D, D U, D D \}\tag{8.2}
$$

all ‘appear’ the same. Similarly at time 1 it is possible to divide the sample space up into two distinguishable ‘partitions 

$$
F _ {1} ^ {0} = \{U U, U D \} \quad \mathrm{and} \quad F _ {1} ^ {1} = \{D U, D D \},\tag{8.3}
$$

depending on whether the initial movement in the market was ‘up’ or ‘down’. Finally at time 2, there are four diferent market states, that we can diferentiate between 

$$
F _ {2} ^ {0 0} = \{U U \}, \quad F _ {2} ^ {0 1} = \{U D \}, \quad F _ {2} ^ {1 0} = \{D U \}, \quad \text { and } \quad F _ {2} ^ {1 1} = \{D D \}.\tag{8.4}
$$

Each of these collection of sets $F _ { 0 } , \ F _ { 1 } ^ { i }$ and $F _ { 2 } ^ { i j }$ divides up or ‘partitions’ the sample space at the relevant time. We can formalise the definition of a partition. 

Definition 8.2 A partition $\{ F _ { i } \} _ { i = 1 } ^ { K }$ ofa set A is a family ofmutually disjoint subsets of A whose union is A. That is, for $i \neq j , F _ { i } \cap F _ { j } = \emptyset$ , and $\cup _ { i = 1 } ^ { K } F _ { i } =$ A. 

From our example we see that associated with the random movements of the market there is a natural sequence of partitions of the sample space in terms of $F _ { 0 } , \ F _ { 1 } ^ { i }$ and $F _ { 2 } ^ { i j }$ . We call such a sequence a filtration, which we formally define below. 

Definition 8.3 A filtration is a family $\{ \mathcal { F } _ { i } \} _ { i = 1 } ^ { K }$ of partitions of Ω. The notation that we use for an element of the filtration is $\mathcal { F } _ { i } = \{ F _ { j } ^ { ( i ) } \} _ { j = 1 } ^ { K _ { i } }$ , where the sets $F _ { j } ^ { ( i ) }$ are a partition of the sample space. An additional constraint that we require is that the partitions at later times respect the earlier partitions. That is, if $i < k$ , then every partition $F _ { i } ^ { ( l ) }$ at the earlier time is equal to the union of some set of partitions $\{ F _ { k } ^ { ( j _ { n } ) } \} _ { n = 1 } ^ { { \tilde { N _ { i , k } } } }$ at the later time. 

Thus the sets $F _ { i }$ that we have defined above are a valid filtration for the market sample space because at each time they partition the sample space, and because the partitions at later times respect the partitions at earlier times, for example, $F _ { 0 } = F _ { 1 } ^ { 0 } \cup F _ { 1 } ^ { 1 }$ . Using the concept of a filtration $\mathcal { F }$ allows us to define a ‘filtered possibility system $( \Omega , \Sigma , { \mathcal { F } } )$ and a ‘filtered probability system’ $( \Omega , \Sigma , { \mathcal { F } } , P )$ . It gives some sort of ‘time ordering’ to the possibility or probability system. 

## 8.3 Adapted Process

Suppose that we had a stochastic process X defined on the market possibility system such that $X _ { 1 } ( U U ) \ne X _ { 1 } ( U D )$ . This means that the process needs to know at time 1 what happens at time 2. We do not want this. Another way to look at it is that $X _ { 1 }$ is not constant on the partition $F ^ { 0 }$ defined by the filtration $\mathcal { F }$ . This leads to the following definition. 

Definition 8.4 A stochastic process X is adapted to a filtration  if at every ‘time $s t e p ' n$ , whenever ω and σ belong to the same partition $F _ { j } ^ { ( n ) }$ defined by the filtration then $X _ { n } ( \omega ) = X _ { n } ( \sigma )$ . That is, $X _ { n }$ is constant on each partition at time n. 

The share price process is clearly adapted to the filtration that we have defined for the market. The only stochastic processes that we will be interested in are adapted ones. 

## 8.4 Conditional Expectation

The conditional probability for an event A given an event B is the probability that A occurs when we alreay know that B occurs. It is equal to 

$$
P (A | B) = \frac {P (A \quad \mathrm{and} \quad B)}{P (B)}.\tag{8.5}
$$

In particular, we will be interested in the case when A is a single element set, and B is an element of a filtration, for example $P ( \{ \omega _ { i } \} | \{ F _ { k } ^ { ( j ) } \} )$ . More concretely, taking an example from the market system, 

$$
P (\{U U \} | \{U U, U D \}) = \hat {p} ^ {0 0},\tag{8.6}
$$

is the probability that we have two up movements, given that we know that the first market move was up. 

We can use the conditional probability to define the conditional expectation of a random variable 

$$
E [ X | \sigma ] = \sum_ {i = 1} ^ {N} X (\{\omega_ {i} \}) P (\{\omega_ {i} \} | \sigma).\tag{8.7}
$$

Again, drawing on the market system, we could consider 

$$
E [ S _ {2} | F ^ {0} ] = S ^ {0 0} \hat {p} _ {*} ^ {0 0} + S ^ {0 1} \hat {p} _ {*} ^ {0 1},\tag{8.8}
$$

which is the expected value of the share price at time 2, given that the initial market move was up. 

Define the stochastic process 

$$
Y _ {m} (\omega_ {i}) = E [ S _ {2} | F _ {k} ^ {(m)} ],\tag{8.9}
$$

where $\omega _ { i } \in \boldsymbol { F } _ { k } ^ { ( m ) }$ . That is, at time m we evaluate the conditional expectation of the share price at time 2 given the filtration at time m. For example, 

$$
Y _ {1} (\{U U \}) = E [ S _ {2} | F ^ {0} ],\tag{8.10}
$$

which was evaluated above. We will use the notation $Y _ { m } = E _ { m } [ S _ { 2 } ]$ to denote the conditional expectation of $S _ { 2 }$ given information up to time m. Note that since the filtration at time 0 is unable to distinguish between any elements, we have $E [ S _ { n } ] = E _ { 0 } [ S _ { n } ]$ 

Exercise 8.1 Verify that the stochastic process $Y _ { m }$ is adapted to the filtration $\mathcal { F }$ 

Recall that from the derivative pricing formulae we have 

$$
\frac {S _ {0}}{B _ {0}} = E _ {0} ^ {*} \left[ \frac {S _ {2}}{B _ {2}} \right] \quad \mathrm{and} \quad \frac {S _ {0}}{B _ {0}} = E _ {0} ^ {*} \left[ \frac {S _ {1}}{B _ {1}} \right],\tag{8.11}
$$

where we have inserted some suggestive zeros. By a simple calculation we could verify that 

$$
\frac {S _ {1}}{B _ {1}} = E _ {1} ^ {*} \left[ \frac {S _ {2}}{B _ {2}} \right].\tag{8.12}
$$

This is an important example of the next concept that we want to consdier—a martingale. 

## 8.5 Martingales

A stochastic process X is called a martingale (with respect to a filtered probability system $( \Omega , \Sigma , P , { \mathcal { F } } )$ , if it satisfies 

$$
X _ {m} = E _ {m} [ X _ {n} ] \quad \forall m \leq n \leq N.\tag{8.13}
$$

The standard definition of a martingale also requires that 

$$
E _ {m} [ | X _ {n} | ] <   \infty \quad \forall m \leq n \leq N,\tag{8.14}
$$

i.e., it exists for all valid m, n. However, this condition is automatically satisfied in our model. If a process is a martingale, then it means that its expected value at any later time is equal to its current value. 

## 8.6 Financial Interpretation

Let us go back and actually verify that the ratio of the stock to bond process is a martingale. In the case of a two-period market we have 

$$
\begin{array}{r c l} \frac {S ^ {0}}{B _ {1}} & = & \frac {\hat {p} _ {*} ^ {0 0} S ^ {0 0} + \hat {p} _ {*} ^ {0 1} S ^ {0 1}}{B _ {2}} \\ & = & E ^ {*} \left[ \frac {S _ {2}}{B _ {2}} | F ^ {0} \right] \end{array}\tag{8.15}
$$

and 

$$
\begin{array}{r c l} \frac {S ^ {1}}{B _ {1}} & = & \frac {\hat {p} _ {*} ^ {1 0} S ^ {1 0} + \hat {p} _ {*} ^ {1 1} S ^ {1 1}}{B _ {2}} \\ & = & E ^ {*} \left[ \frac {S _ {2}}{B _ {2}} | F ^ {1} \right], \end{array}\tag{8.16}
$$

which says that given that the system is in the state $S ^ { 0 }$ at time 1, the ratio of the stock to bond price can be expressed in terms of conditional probabilities $\hat { p } _ { * } ^ { 0 0 }$ and $\hat { p } _ { * } ^ { 0 1 }$ , and similarly for $S ^ { 1 } , \ \hat { p } _ { * } ^ { 1 0 }$ and $\hat { p } _ { * } ^ { 1 1 }$ . Writing this in terms of conditional expectation, we then obtain 

$$
\frac {S _ {1}}{B _ {1}} = E _ {1} ^ {*} \left[ \frac {S _ {2}}{B _ {2}} \right].\tag{8.17}
$$

In fact, using the one-period argument to derive the risk-netural probabilities we have for $n \leq N$ 

$$
\frac {S _ {n - 1}}{B _ {n - 1}} = E _ {n - 1} ^ {*} \left[ \frac {S _ {n}}{B _ {n}} \right],\tag{8.18}
$$

or, more generally, by induction we have 

$$
\frac {S _ {m}}{B _ {m}} = E _ {m} ^ {*} \left[ \frac {S _ {n}}{B _ {n}} \right]\tag{8.19}
$$

for $m \leq n$ 

## Exercise 8.2 Verify equation (8.19) for the three-period binomial model.

Thus, in the risk-neutral measure the ratio of the share price $S _ { n }$ to the money market account $B _ { n }$ is a martingale. This can be regarded as the definition of the risk-neutral measure. Alternatively, we say that the riskneutral probability measure $P ^ { * }$ is a martingale measure for the ratio $S _ { n } / B _ { n }$ 

The no arbitrage argument for derivative pricing, combined with a backwards induction, allows us to deduce, in the case of an N-period binomial model, that 

$$
\frac {f _ {m}}{B _ {m}} = E _ {m} ^ {*} \left[ \frac {f _ {n}}{B _ {n}} \right],\tag{8.20}
$$

for $0 \leq m \leq n \leq N$ . In other words: the ratio of the derivative price to the money market account is a martingale. In particular, if N is the payof date of the derivative, then 

$$
\frac {f _ {0}}{B _ {0}} = E ^ {*} \left[ \frac {f _ {N}}{B _ {N}} \right].\tag{8.21}
$$

So, once we show that the ratio of the derivative price to the money market account is a martingale in the risk-neutral measure, that is, equation (8.20) holds, then we can ‘price’ the derivative by use of (8.21). It will be a crucial relation when we come to pricing derivatives in the continuous time case. 

## 9 Binomial Lattice Model

The general kind of tree model that we have been discussing so far is sometimes called a ‘bushy tree’, since the number of branches gets large very quickly. At time n there are 2<sup>n</sup> states, which as n grows larger clearly makes the tree computationally unfeasible. A very useful special model is obtained, however, by letting the branches recombine to form a lattice of prices, and hence is called a ‘lattice model’ or ‘recombining tree’. At time $t = n$ the number of diferent states is only $n + 1$ which grows much more slowly than the $2 ^ { n }$ nodes of the ‘basic’ tree. 

At each node, the asset price can move either up in value, with probability $p ,$ by a multiplicative factor $u ,$ or down, with probability q, by a factor d. Index the nodes at each time by the number of ‘down’ moves that you need to reach it, for example, $S _ { 3 } ^ { 1 }$ is the node at time 3 with one ‘down’ and two ‘up’ movements. We can write the value of the $i ^ { \mathrm { t h } }$ node at time n as 

$$
S _ {n} ^ {i} = S _ {0} u ^ {n - i} d ^ {i}\tag{9.1}
$$

where $i = 0 , \ldots , n$ and the time index is now necessary. Thus, for example, $S _ { 2 } ^ { 0 } = S _ { 0 } u ^ { 2 } , S _ { 2 } ^ { 1 } = S _ { 0 } u d$ , and so on. A three-period recombining tree is shown below: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/fd7c8895b4674ea3c4edb0c1067dcbecfb946684e4f4c4e73d11dec513e99cfa.jpg)


(9.2) 

Suppose that at each node the actual probability of an up move is $p ,$ and a down move is $q .$ . Then, the probability of $S _ { n }$ taking on a specific value $S _ { n } ^ { i }$ is 

$$
\mathrm{Prob} [ S _ {n} = S _ {n} ^ {i} ] = C _ {i} ^ {n} p ^ {n - i} q ^ {i},\tag{9.3}
$$

where $C _ { i } ^ { n }$ is the standard binomial coeficient, given by 

$$
C _ {i} ^ {n} = \frac {n !}{i ! (n - i) !},\tag{9.4}
$$

e.g., $C _ { 2 } ^ { 3 } = 3 ! / ( 2 ! 1 ! ) = 3$ . The factor $C _ { i } ^ { n }$ is the number of diferent ways of arriving at the node $S _ { n } ^ { i }$ 

Exercise 9.1 Show that the number of diferent ways of arriving at the node $S _ { n } ^ { i }$ is $C _ { i } ^ { n }$ 

Recall that $C _ { i } ^ { n }$ is called the binomial coeficient because 

$$
(x + y) ^ {n} = \sum_ {i = 0} ^ {n} C _ {i} ^ {n} x ^ {n - i} y ^ {i}.\tag{9.5}
$$

Hence if we set $x = p$ and $y = q$ then using the fact that $p + q = 1$ , we see that 

$$
\sum_ {i = 0} ^ {n} C _ {i} ^ {n} p ^ {n - i} q ^ {i} = 1.\tag{9.6}
$$

This means that if we sum the probabilities (9.3) of each node at the $n ^ { \mathrm { t h } }$ time step, then we get one, as we should. 

However, in order to price derivatives, we know that we do not need to make any assumptions about the ‘physical’ probabilities, that is, the numbers $p$ and $q ,$ but instead, we must calculate the appropriate risk-neutral probabilities. For the bank account process, we assume for simplicity a constant interest rate of $r$ per period, continuously compounded, so $B _ { n } = B _ { 0 } e ^ { r n }$ Then, for risk-neutrality, we want 

$$
S _ {0} \frac {B _ {1}}{B _ {0}} = E ^ {*} [ S _ {1} ] = p _ {*} S _ {0} u + q _ {*} S _ {0} d\tag{9.7}
$$

at the first node. In fact, the probabilities are governed by essentially the same equation at each node. For example, at the node $S _ { 2 } ^ { 1 } = S _ { 0 } u d$ we want 

$$
\begin{array}{r c l} {S _ {0} u d \frac {B _ {3}}{B _ {2}}} & = & {E ^ {*} [ S _ {3} ]} \\ & = & {p _ {*} S _ {0} u ^ {2} d + q _ {*} S _ {0} u d ^ {2},} \end{array}\tag{9.8}
$$

but this reduces to the previous equation. The solution for $p _ { * } , q _ { * }$ is easily seen to be r r 

$$
p _ {*} = \frac {e ^ {r} - d}{u - d} \quad \mathrm{and} \quad q _ {*} = \frac {u - e ^ {r}}{u - d}.\tag{9.9}
$$

Exercise 9.2 Verify that equation (9.9) is consistent with the risk-neutral probabilities calculated in the general theory of tree models developed earlier. 

In the risk-neutral measure, the lattice is highly structured, which makes calculations easy. In particular, we can price derivatives. The risk-neutral probability of any state $S _ { n } ^ { i }$ is 

$$
\mathrm{Prob} ^ {*} [ S _ {n} = S _ {n} ^ {i} ] = C _ {i} ^ {n} p _ {*} ^ {n - 1} q _ {*} ^ {i},\tag{9.10}
$$

where Prob∗ denotes probability in the risk-neutral measure $P ^ { * }$ . Thus, suppose $f _ { 0 }$ is the price of a derivative (at time 0) with specified payof $f _ { n } ^ { i }$ at time $n$ in the $i ^ { \mathrm { t h } }$ state. Then, from our general theory of tree models, we know that 

$$
\frac {f _ {0}}{B _ {0}} = \frac {E ^ {*} [ f _ {n} ]}{B _ {n}},\tag{9.11}
$$

from which it follows that 

$$
f _ {0} = e ^ {- r n} \sum_ {i = 0} ^ {n} C _ {i} ^ {n} p _ {*} ^ {n - i} q _ {*} ^ {i} f _ {n} ^ {i}.\tag{9.12}
$$

This is the binomial derivative pricing formula which, together with its various generalizations, has many useful applications. In the case of a call option with strike $K ,$ for example, we would insert 

$$
\begin{array}{r c l} {f _ {n} ^ {i}} & = & {\max [ S _ {n} ^ {i} - K, 0 ]} \\ & = & {\max [ S _ {0} d ^ {i} u ^ {n - i} - K, 0 ]} \end{array}\tag{9.13}
$$

for the payof function $f _ { n } ^ { i }$ 

Exercise 9.3 For a three-period model with $S _ { 0 } = \ S 1 0 0 , p = 0 . 6 , r = 1 . 0 1$ 2 $u = 1 . 0 1$ and $d = 0 . 9 9$ , construct the lattice of stock prices and probabilities, calculate the risk-neutral probabilities for the lattice, and then price a call option with strike $100. 

## 10 Relation to Binomial Model

We shall now show how in a suitable limit the binomial lattice model of chapter 3 can give rise to the Wiener model for asset price movements. 

## 10.1 Limit of a Random Walk

Consider an n-period lattice. Recall that at any node of the lattice we have an ‘up’ and a ‘down’ branch, with probabilities $p$ and $q$ respectively, as shown below From an initial value of $S _ { 0 }$ , the asset price will increase to $S _ { 0 } u$ with probability $p ,$ or decrease to $S _ { 0 } d$ with probability $q .$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/2476e2847d6494186927f3411a81fecab17241392cf2d71039a6bd4badd4055b.jpg)


(10.1) 

Let $\delta t$ be the time-step to the. next node, and since there are n steps, the final time will be $t = n \delta t$ . Suppose moreover that the up and down factors are given explicitly by 

$$
u = e ^ {\tilde {\mu} \delta t + \sigma \sqrt {\delta t}} \quad \mathrm{and} \quad d = e ^ {\tilde {\mu} \delta t - \sigma \sqrt {\delta t}},\tag{10.2}
$$

where $\tilde { \mu }$ and $\sigma$ are constants. We shall assume that the actual probabilities $p$ and $q \ { \mathrm { ( i . e . } }$ , not the risk-neutral probabilities) are each $\begin{array} { l } { { \frac { 1 } { 2 } } } \end{array}$ . If we let $X _ { n }$ be the random variable equal to the number of $\mathrm { \dot { \cdot } u p } ^ { \mathrm { \prime } }$ movements after n steps, then the asset price $S _ { t }$ is 

$$
S _ {t} = S _ {0} u ^ {X _ {n}} d ^ {n - X _ {n}},\tag{10.3}
$$

where $n - X _ { n } .$ is the number of ‘down’ movements. Substituting in the values of u and d given above then yields 

$$
S _ {t} = S _ {0} \exp \left[ \tilde {\mu} t + \sigma \sqrt {t} \frac {2 X _ {n} - n}{\sqrt {n}}) \right].\tag{10.4}
$$

The random variable $X _ { n }$ has a binomial distribution, with mean ${ \frac { 1 } { 2 } } n$ and variance ${ \scriptstyle { \frac { 1 } { 4 } } } n$ . We can improve the notation here slightly by defining the new random variable 

$$
Z _ {n} \equiv \frac {2 X _ {n} - n}{\sqrt {n}},\tag{10.5}
$$

which has a binomial distribution with mean zero and variance one. Hence the asset price process is given by 

$$
S _ {t} = S _ {0} \exp \left[ \tilde {\mu} t + \sigma \sqrt {t} Z _ {n} \right].\tag{10.6}
$$

Next we use the central limit theorem, which says that if $A _ { 1 } , A _ { 2 } , . . .$ . are independent, identically distributed random variables with mean m and variance $V$ , and $X _ { n }$ is the sum $X _ { n } = A _ { 1 } + A _ { 2 } + \cdot \cdot \cdot A _ { n }$ , then the random variable $Z _ { n }$ defined by $Z _ { n } = ( X _ { n } - n m ) / \sqrt { n V } \to \mathrm { N } ( 0 , 1 )$ for large n. This tells us that in the limit of large $n , Z _ { n }$ converges to a normally distributed random variable with mean zero, and variance 1. Thus, it follows that 

$$
\lim _ {n \to \infty} S _ {t} = S _ {0} \exp [ \tilde {\mu} t + \sigma W _ {t} ]\tag{10.7}
$$

where $W _ { t }$ is a normally distributed random variable with mean zero and variance t. Then if we set $\tilde { \mu } = \textstyle \mu - { \frac { 1 } { 2 } } \sigma ^ { 2 }$ , the asset price process becomes 

$$
\lim _ {n \to \infty} S _ {t} = S _ {0} \exp [ \mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t ],\tag{10.8}
$$

and we are back to the Wiener model. Or so it appears. To show that we have recovered the model entirely, we still need to show that $W _ { t }$ is indeed the Wiener process—we know that it is normally distributed, but now we need to check that it has independent increments. This follows intuitively from the fact that the binomial process is defined as n independent measurements, and hence, by construction, has independent increments. When we take the large n limit, we are tempted to believe that this property is preserved, so (10.8) actually is the Wiener process. 

## 10.2 Martingales associated with Random Walks

This is, of course, a rather simplistic ‘derivation’ of the Wiener process, and does not yet fully exploit the technology that we developed for the binomial model. To proceed further, we begin by refining the binomial lattice model by consideration of a certain family of martingales that arise naturally in this context. 

Lemma 10.1 Suppose $Y _ { 1 } , Y _ { 2 } , . . .$ . are independent, identically distributed random variables with the property that the moment generating function, 

$$
M (\theta) = E [ e ^ {\theta Y _ {1}} ],\tag{10.9}
$$

exists (i.e., is finite) for some value of θ. Define a sequence of random variables by $Z _ { 0 } = 1$ , and 

$$
Z _ {n} = \frac {e ^ {\theta (Y _ {1} + Y _ {2} + \cdots + Y _ {n})}}{[ M (\theta) ] ^ {n}}.\tag{10.10}
$$

Then 

$$
E _ {n} [ Z _ {m} ] = Z _ {n}, \quad m \geq n\tag{10.11}
$$

where $E _ { n }$ is the conditional expectation given information up to time n (in this case, given $Y _ { 1 } , Y _ { 2 } , \ldots , Y _ { n } )$ 

Proof By definition, we have 

$$
E _ {n} [ Z _ {m} ] = E _ {n} \left[ \frac {e ^ {\theta (Y _ {1} + Y _ {2} + \cdots + Y _ {m})}}{[ M (\theta) ] ^ {m}} \right].\tag{10.12}
$$

Since the expectation is conditional, we know the values of $Y _ { 1 } , Y _ { 2 } , \dots , Y _ { n } .$ and hence can take them outside the expectation, so 

$$
E _ {n} [ Z _ {m} ] = \frac {e ^ {\theta (Y _ {1} + Y _ {2} + \cdots + Y _ {n})}}{[ M (\theta) ] ^ {n}} E \left[ \frac {e ^ {\theta (Y _ {n + 1} + Y _ {n + 2} + \cdots + Y _ {m})}}{[ M (\theta) ] ^ {m - n}} \right]\tag{10.13}
$$

But then since the $Y _ { i }$ ’s are independent and identically distributed, we can factor their expectation, which will then cancel with the factors of the moment generating function in the denominator, 

$$
E \left[ \frac {e ^ {\theta (Y _ {n + 1} + Y _ {n + 2} + \cdots + Y _ {m})}}{[ M (\theta) ] ^ {m - n}} \right] = \frac {E \left[ e ^ {\theta Y _ {n + 1}} \right] E \left[ e ^ {\theta Y _ {n + 2}} \right] \times \cdots \times E \left[ e ^ {\theta Y _ {m}} \right]}{[ M (\theta) ] ^ {m - n}} = 1.\tag{10.14}
$$

Hence, 

$$
E _ {n} [ Z _ {m} ] = \frac {e ^ {\theta (Y _ {1} + Y _ {2} + \cdots + Y _ {n})}}{[ M (\theta) ] ^ {n}} = Z _ {n}\tag{10.15}
$$

as desired. 

For example, if $Y _ { 1 }$ is normally distributed with mean m and variance $V ,$ it follows that 

$$
M (\theta) = E [ e ^ {\theta Y _ {1}} ] = e ^ {\theta m + \frac {1}{2} \theta^ {2} V},\tag{10.16}
$$

$$
Z _ {n} = e ^ {\theta (\tilde {Y} _ {1} + \tilde {Y} _ {2} + \dots \tilde {Y} _ {n}) - \frac {1}{2} n \theta^ {2} V}\tag{10.17}
$$

where ${ \tilde { Y } } _ { i } = Y _ { i } - m$ (i.e., remove the mean). But, this is clearly the product 

$$
Z _ {n} = e ^ {\theta \tilde {Y} _ {1} - \frac {1}{2} \theta^ {2} V} e ^ {\theta \tilde {Y} _ {2} - \frac {1}{2} \theta^ {2} V} \dots e ^ {\theta \tilde {Y} _ {n} - \frac {1}{2} \theta^ {2} V}\tag{10.18}
$$

which is given multiplicatively by a series of exponential martingales. 

Another example, which is the one we are particularly interested in here, is generated when $Y _ { i } = \pm 1$ , so $Y _ { 1 } + Y _ { 2 } + \cdots + Y _ { n }$ is the random variable corresponding to the $n ^ { \mathrm { t h } }$ step of a random walk. Then 

$$
M (\theta) = p e ^ {\theta} + q e ^ {- \theta}\tag{10.19}
$$

where $p , q$ are the probabilities respectively for $Y _ { i } = \pm 1$ , and thus we have 

$$
Z _ {n} = \frac {e ^ {\theta (Y _ {1} + Y _ {2} + \cdots + Y _ {n})}}{(p e ^ {\theta} + q e ^ {-} \theta) ^ {n}}\tag{10.20}
$$

Equivalently, we have 

$$
Z _ {n} = \frac {e ^ {\theta X _ {n}}}{(p e ^ {\theta} + q e ^ {-} \theta) ^ {n}}\tag{10.21}
$$

where $X _ { n } = Y _ { 1 } + Y _ { 2 } + \cdot \cdot \cdot + Y _ { n }$ is the random walk. We note that $E [ Y _ { i } ] = p - q$ Thus, $E [ X _ { n } ] = n ( p - q )$ , and we have ${ \tilde { X } } _ { n } = X _ { n } - n ( p - q )$ , where $E [ \ddot { X } _ { n } ] = 0$ Now suppose that we consider the case where $\textstyle p = q = { \frac { 1 } { 2 } }$ . Then we have 

$$
Z _ {n} = \frac {e ^ {\theta X _ {n}}}{[ \frac {1}{2} (e ^ {\theta} + e ^ {-} \theta) ] ^ {n}}\tag{10.22}
$$

and $E [ X _ { n } ] = 0$ . Now, suppose that we set 

$$
S _ {t} = S _ {0} e ^ {\mu t} \frac {e ^ {\sigma \sqrt {\delta t} X _ {n}}}{[ \frac {1}{2} (e ^ {\sigma \sqrt {\delta t}} + e ^ {- \sigma \sqrt {\delta t}}) ] ^ {n}},\tag{10.23}
$$

where $t = n \delta t$ . Then we can write 

$$
S _ {t} = S _ {0} e ^ {\mu t} \frac {e ^ {\sigma \sqrt {t} (X _ {n} / \sqrt {n}}}{[ \frac {1}{2} (e ^ {\sigma \sqrt {t} / \sqrt {n}} + e ^ {- \sigma \sqrt {t} / \sqrt {n}}) ] ^ {n}}.\tag{10.24}
$$

In the limit $n \to \infty$ , the numerator $X _ { n } / \sqrt { n }$ converges to an $N ( 0 , 1 )$ random variable, whereas for the denominator we have 

$$
\frac {1}{2} (e ^ {\sigma \sqrt {t} / \sqrt {n}} + e ^ {- \sigma \sqrt {t} / \sqrt {n}}) = 1 + \frac {\sigma^ {2} t}{2 n} + \mathcal {O} (n ^ {- 2}).\tag{10.25}
$$

So as $n \to \infty$ 

$$
\left[ \frac {1}{2} (e ^ {\sigma \sqrt {t} / \sqrt {n}} + e ^ {- \sigma \sqrt {t} / \sqrt {n}}) \right] ^ {n} \rightarrow e ^ {\frac {1}{2} \sigma^ {2} t}\tag{10.26}
$$

Thus, in the limit $n \longrightarrow \infty .$ , we find that $S _ { t }$ converges to 

$$
S _ {t} = S _ {0} e ^ {\mu t} e ^ {\sigma \sqrt {t} X - \frac {1}{2} \sigma^ {2} t},\tag{10.27}
$$

where X has an $N ( 0 , 1 )$ distribution, and hence $\sqrt { t } X$ has an $N ( 0 , t )$ distribution. This confirms in rather more detail the result that we deduced earlier. 

## 11 Continuous Time Models

The binomial model for asset price movements sufers from some defects, of which the most serious, from our point of view, is that in order for it to be realistic the model must have a very large number of time steps. While for a computer this presents less of a problem, actually evaluating the derivative using equation (7.11) becomes a labourious and time-consuming procedure. We can alleviate this to a certain extent, by moving from a discrete time model to one in which time is treated as a continuous variable. 

In this chapter we begin by our look at continuous time models of the financial markets by introducing an elementary ‘Wiener model’ for asset prices and exploring a few of its characteristics. 

## 11.1 The Wiener Model

The simplest continuous time model for an asset price is the basic log-normal or Wiener model. This model can be used to a reasonable approximation to fit actual asset movements over limited time periods. The asset price movements are driven both by a deterministic ‘trend’ or drift, and a random motion. The strength of the random component of the motion is called the volatility of the process. From actual asset price data, it is evident that, at least to a first approximation, the random motions are uncorrelated, that is, the market has no memory of its previous behaviour. More advanced models of the financial markets may take into account correlations between motions of the asset at one time and other, but little is really understood on this score. The Wiener model has the significant advantage over most other models in that it is simple enough that in many calculations we can obtain explicit ‘closed form’ results. 

However, we are not going to do anything with only words, so it is now time to write down some formulae. Analogous to the stochastic processes that we studied in the discrete time case, we can define a continuous time stochastic process as a family of random variables indexed by a continuous time parameter t. In the elementary Wiener model the asset price $S _ { t }$ is a stochastic process that evolves in time based on the following formula 

$$
S _ {t} = S _ {0} e ^ {\mu t} e ^ {\sigma W _ {t} - \frac {1}{2} \sigma^ {2} t}.\tag{11.1}
$$

Here $S _ { 0 } , \mu$ and $\sigma$ are constants: $S _ { 0 }$ is the initial stock price, $\mu$ is the drift and $\sigma$ is the volatility. The Wiener process $W _ { t }$ is the source of ‘randomness’ or ‘noise’ in the asset price movement. As we shall demonstrate in a later chapter it can be expressed as the limit of a lattice tree model. 

But what is the Wiener process $W _ { t }$ and what are its properties? Well, it is a stochastic process beginning at time 0 that satisfies 

1. The initial value is zero: $W _ { 0 } = 0$ 

2. At each time t, $W _ { t }$ is a normally distributed random variable with mean 0 and variance t. 

3. $W _ { t }$ has independent increments. That is, for $a < b < c < d ,$ the diference between the values of $W _ { t }$ at two times, such as $W _ { b } - W _ { a }$ and $W _ { d } - W _ { c } ,$ are independent random variables. 

If a stochastic process has these three properties, then we say that it is a Wiener process or, equivalently, it is a simple Brownian motion. The Wiener process is a very rich object of mathematical interest, with numerous important applications in finance. 

An example Wiener process is shown in figure 11.1. Note that at any time $W _ { t }$ has an equal likelihood of being positive or negative, but the spread (variance) increases over time. If we add to the Wiener process a constant deterministic drift of the form $\mu t$ then the resulting process will have a nonzero expectation value, as illustrated in figure 11.2. 

## 11.2 The Normal Distribution

Before we try and do too much with the Wiener process it is probably worth spending some time recalling some facts about the normal distribution. The probability distribution of a stochastic process at any particular time t is called the marginal distribution, so we say that a Wiener process has a ‘normal’ marginal distribution. We refer to any random variable that is normally distributed with mean m and variance $V$ as an $\mathrm { N } ( m , V )$ random variable. Hence if X is an $\mathrm { N } ( m , V )$ random variable we have 

$$
\operatorname{Prob} [ a <   X <   b ] = \frac {1}{\sqrt {2 \pi V}} \int_ {a} ^ {b} \exp \left[ - \frac {(x - m) ^ {2}}{2 V} \right] d x.\tag{11.2}
$$

Since the Wiener process $W _ { t }$ has an $\mathrm { N } ( 0 , t )$ marginal distribution, it is characterized by the following probability law: 

$$
\mathrm{Prob} [ a <   W _ {t} <   b ] = \frac {1}{\sqrt {2 \pi t}} \int_ {a} ^ {b} \exp \left[ - \frac {x ^ {2}}{2 t} \right] d x.\tag{11.3}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/6f71b626067d9f2b2352a60702f6b413070328730007ca0b59319545bdb235ea.jpg)



Figure 11.1: A Wiener process.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/71b4a80d0278b1b2d45451d4cb07fdfb02ef6250cf5bd4292f6bd7f7b48103db.jpg)



Figure 11.2: A Wiener process with an added drift term of 25% i.e. of the form W +.25t. The dashed line represents the contribution from the drift term. The underlying Wiener process is the same in both this figure and figure 11.1.


How about the diference between the Wiener process at two diferent times, $W _ { a + b } - W _ { b } ?$ In the definition of $W _ { t }$ we required that this be an independent random variable. In fact, it turns out to be a $\mathrm { N } ( 0 , b )$ random variable, which will be very important for some of our calculations. 

Exercise 11.1 Verify that $W _ { a + b } - W _ { a }$ is an $\mathrm { N } ( 0 , b )$ random variable. 

A useful formula to define is the cumulative normal distribution function $N ( x )$ 

$$
N (x) = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {x} \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi .\tag{11.4}
$$

Later, we will be able to express the price of call and put options in terms of $N ( x )$ . For now, we can use the cumulative distribution in order to describe a Wiener process $W _ { t }$ 

$$
\begin{array}{r c l} \mathrm{Prob} [ W _ {t} <   b ] & = & \frac {1}{\sqrt {2 \pi t}} \int_ {\xi = - \infty} ^ {\xi = b} e ^ {- \frac {\xi^ {2}}{2 t}} d \xi \\ & = & \frac {1}{\sqrt {2 \pi}} \int_ {\eta = - \infty} ^ {\eta = b / \sqrt {t}} e ^ {- \frac {1}{2} \eta^ {2}} d \eta \\ & = & N (b / \sqrt {t}) \end{array}\tag{11.5}
$$

where we made the substitution $\xi = \eta \sqrt { t }$ in going from the first to second line. 

We are now in a position where we can, at least heuristically, understand the drift $\mu$ and volatility $\sigma$ of the Wiener model for an asset price process, given by equation (11.1). In order to interpret the drift, we need the following result. 

Lemma 11.1 Let X be an $\mathrm { N } ( m , V )$ random variable. Then 

$$
E [ \exp (\alpha X) ] = \exp \left(\alpha m + \frac {1}{2} \alpha^ {2} V\right).\tag{11.6}
$$

Proof The density function $\rho _ { m , V } ( x )$ for an $N ( m , V )$ random variable is 

$$
\rho_ {m, V} (x) = \frac {1}{\sqrt {2 \pi V}} \exp \left(- \frac {(x - m) ^ {2}}{2 V}\right).\tag{11.7}
$$

Thus, the expected value is 

$$
E [ \exp (\alpha X) ] = \int_ {x = - \infty} ^ {x = \infty} {\frac {1}{\sqrt {2 \pi V}}} \exp \left[ \alpha x - \frac {(x - m) ^ {2}}{2 V} \right] d x\tag{11.8}
$$

A straightforward calculation that involves ‘completing the square’ then gives the desired result. 

An immediate corollary of this result is that 

$$
E [ \exp (\sigma W _ {t}) ] = \exp \left(\frac {1}{2} \sigma^ {2} t\right),\tag{11.9}
$$

from which we conclude that the expected value of the Wiener process is 

$$
\begin{array}{r c l} {E [ S _ {t} ]} & = & {E \left[ S _ {0} \exp \left(\mu t - \frac {1}{2} \sigma^ {2} t + \sigma W _ {t}\right) \right]} \\ & = & {S _ {0} \exp \left(\mu t - \frac {1}{2} \sigma^ {2} t\right) E \left[ \exp (\sigma W _ {t}) \right]} \\ & = & {S _ {0} \exp (\mu t).} \end{array}\tag{11.10}
$$

Since $E [ S _ { t } ] / S _ { 0 } = e ^ { \mu t }$ , we say that $\mu$ is the rate of return on an investment in the asset $S _ { t }$ with initial price $S _ { 0 }$ . Thus, the drift parameter controls the expected value of the asset price in the future. However, rather surprisingly, it will turn out that the call and put option prices that we will derive are independent of the value of the drift, that is, they do not depend on how we expect the asset price will move. 

The volatility, on the other hand, measures the ‘response’ of $S _ { t }$ to the movements in the Wiener process $W _ { t }$ . That is, the larger the volatility, the more randomness that is introduced into the model, as shown in figures 11.3 and 11.4. It is the volatility which will play the most important role in option pricing because it controls the randomness that we need to try and eliminate. 

## Exercise 11.2 Calculate the variance of the asset price process $S _ { t }$

Note that since the logarithm of the asset price is given by 

$$
\ln S _ {t} = \ln S _ {0} + (\mu - \frac {1}{2} \sigma^ {2}) t + \sigma W _ {t},\tag{11.11}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/a07302c350a6112acb1f276d763b9c96dd0af3d56cf4fb29302ef848e912c6d3.jpg)



Figure 11.3: A Wiener model asset price processes, driven by equation (11.1), with an initial price of $S _ { 0 } = \mathbb { S } 1 0 0$ , a drift of $\mu = 1$ and a volatility of $\sigma = 0 . 5$ . The dashed is line is the expected value $E [ S _ { t } ] = S _ { 0 } e ^ { \mu t }$


it follows that ln $S _ { t }$ is normally distributed with mean ln $S _ { 0 } + ( \mu - \textstyle { \frac { 1 } { 2 } } \sigma ^ { 2 } ) t$ and variance $\sigma ^ { 2 } t$ , which is why our basic model is sometimes called the log-normal model. This model is also sometimes called ‘geometric Brownian motion with drift’. 

Another useful property of Brownian motion is the fact that 

$$
E [ (W _ {t} - W _ {s}) ^ {2} ] = t - s,\tag{11.12}
$$

which as we shall demonstrate below, follows from the independent increments property. Using $W _ { 0 } = 0$ , we can write 

$$
W _ {t} = \left(W _ {t} - W _ {s}\right) + \left(W _ {s} - W _ {0}\right),\tag{11.13}
$$

and after squaring both sides we have 

$$
W _ {t} ^ {2} = (W _ {t} - W _ {s}) ^ {2} + (W _ {s} - W _ {0}) ^ {2} + 2 (W _ {t} - W _ {s}) (W _ {s} - W _ {0}).\tag{11.14}
$$

Taking expectations yields 

$$
E [ W _ {t} ^ {2} ] = E [ (W _ {t} - W _ {s}) ^ {2} ] + E [ W _ {s} ^ {2} ] + 0,\tag{11.15}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/245d24ae1d8155076cdc3feaf337f325eb5ba0b528af119c507a7ef6da4db0a9.jpg)



Figure 11.4: A Wiener model asset price processes, driven by equation (11.1), with an initial price of $S _ { 0 } = \mathbb { \ S } 1 0 0$ , a drift of $\mu = 1$ and a volatility of $\sigma = 1 . 0$ . This plot uses the same Wiener process as figure 11.3, but the volatility is twice as large here. You can see that the larger volatility causes the deviations from the expected value to be generally greater. The dashed is line is the expected value $E [ S _ { t } ] = S _ { 0 } e ^ { \hat { \mu } t }$


where we have used the fact that 

$$
\begin{array}{r c l} E [ (W _ {t} - W _ {s}) (W _ {s} - W _ {0}) ] & = & E [ W _ {t} - W _ {s} ] E [ W _ {s} - W _ {0} ] \\ & = & 0, \end{array}\tag{11.16}
$$

since the increments are independent and have zero mean. Returning to equation (11.15) we can evaluate the expectations to obtain 

$$
t = E [ (W _ {t} - W _ {s}) ^ {2} ] + s\tag{11.17}
$$

as desired. 

We could also take conditional expectations of equation (11.14), 

$$
\begin{array}{r c l} E _ {s} \left[ W _ {t} ^ {2} \right] & = & E _ {s} \left[ W _ {s} ^ {2} \right] + E _ {s} \left[ \left(W _ {t} - W _ {s}\right) ^ {2} \right] + 2 E _ {s} \left[ \left(W _ {t} - W _ {s}\right) \left(W _ {s} - W _ {0}\right) \right] \\ & = & W _ {s} ^ {2} + t - s + 0, \end{array} \tag {11}\tag{11.18}
$$

which implies that 

$$
E _ {s} [ W _ {t} ^ {2} - t ] = W _ {s} ^ {2} - s\tag{11.19}
$$

Note that this is the martingale property that we previously examined in the discrete time case. 

Exercise 11.3 Calculate $E [ X ^ { n } ]$ for X normally distributed with mean m and variance V for $n = 1 , 2 , 3 , 4$ 

Exercise 11.4 Calculate $\operatorname { E } [ e ^ { \alpha X } ]$ and $\mathrm { V a r } [ e ^ { \alpha X } ]$ for X as above. 

Exercise 11.5 Show that if $M _ { t } = e ^ { \alpha W _ { t } - \frac { 1 } { 2 } \alpha ^ { 2 } t }$ then 

$$
E _ {s} [ M _ {t} ] = M _ {s}.\tag{11.20}
$$

Exercise 11.6 Show that $M _ { t } = \cos ( \beta W _ { t } ) e ^ { \frac { 1 } { 2 } \beta ^ { 2 } t }$ satisfies 

$$
E _ {s} [ M _ {t} ] = M _ {s}.\tag{11.21}
$$

## 12 Stochastic Calculus

We are now in a position to begin considering trading in continuous time and to examine the situation where asset price motions are driven by a Wiener process rather than by a discrete time model. The idea is that at each instant we can look at the Wiener process $W _ { t }$ and study its change $d W _ { t }$ at that instant, which, intuitively can be thought of as moving slightly up or down with equal probability. 

For the asset price $S _ { t }$ we can hypothesize that the change in its value is given by a so-called ‘stochastic diferential equation’ of the form 

$$
\frac {d S _ {t}}{S _ {t}} = \mu_ {t} d t + \sigma_ {t} d W _ {t}.\tag{12.1}
$$

This says that the infinitesimal change $d S _ { t }$ in the asset price at time t, as a percentage of the value $S _ { t }$ , is given by a drift term $\mu _ { t } d t$ and a ‘fluctuation’ or small movement upwards or downwards given by $\sigma _ { t } d W _ { t }$ . We call $\mu _ { t }$ the drift at time $t ,$ and $\sigma _ { t }$ the volatility at time t. For elementary applications we take $\mu$ and $\sigma$ to be constant. This is often called the ‘Black-Scholes’ world. The solution of equation (12.1) is given by the Wiener model that we looked at in the previous chapter, 

$$
S _ {t} = S _ {0} e ^ {\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t},\tag{12.2}
$$

as we shall show later. 

Our first goal is to make sense of (12.1) mathematically, and to introduce the tools necessary to work with such expressions involving the Wiener process. This will enable us to see, for example, why (12.2) is the solution of (12.1). The main tool that we require is the so-called stochastic calculus or Ito calculus. Our approach will be to build this up in an intuitive way, and then to backtrack and attend to details and more precise definitions. 

A closely related idea to stochastic calculus is the stochastic integral. The integral of a process with respect to a Brownian motion is defined to be 

$$
\int_ {a} ^ {b} X _ {t} d W _ {t} = \lim _ {N \to \infty} \sum_ {i = 0} ^ {N} X _ {t _ {i}} (W _ {t _ {i + 1}} - W _ {t _ {i}}),\tag{12.3}
$$

where the $t _ { i }$ are some partition of the interval $[ a , b ]$ . The stochastic integral has a natural interpretation in terms of trading strategies. In particular, if 

$S _ { t }$ is an asset price, then a trading strategy $\phi _ { u }$ is a random process that says what the holding in the asset is at time u. Then 

$$
V _ {t} = V _ {0} + \int_ {0} ^ {t} \phi_ {u} d S _ {u}\tag{12.4}
$$

represents the value at time t of an investment portfolio based on holdings in the given asset, where $V _ { 0 }$ is the initial value of the portfolio, and $\phi _ { u }$ is the trading strategy. The term $\phi _ { u } d S _ { u }$ represents the infinitesimal gain (or loss) the portfolio makes at time u when the asset moves up (or down) by the amount $d S _ { u }$ . More fully, we can write 

$$
V _ {t} = V _ {0} + \int_ {0} ^ {t} \phi_ {u} S _ {u} \mu_ {u} d u + \int_ {0} ^ {t} \phi_ {u} S _ {u} \sigma_ {u} d W _ {u},\tag{12.5}
$$

where we have substituted the expression for $d S _ { u }$ in from equation (12.1). The trading strategy $\phi _ { u }$ can, in principle, be deterministic, but generally is itself also a random process, which depends on how events have played out so far. As in the discrete time case, we will be interested in deriving a hedging strategy that allows us to eliminate risk and generate a guaranteed return. 

The main tool that we require is Ito’s Lemma, which says that if the random process $X _ { t }$ satisfies 

$$
d X _ {t} = \mu_ {t} d t + \sigma_ {t} d W _ {t}\tag{12.6}
$$

and if $f ( X _ { t } )$ has continuous second derivatives as a function $f ( x )$ , then the process $f _ { t } = f ( X _ { t } )$ satisfies 

$$
d f (X _ {t}) = \frac {\partial f}{\partial X _ {t}} d X _ {t} + \frac {1}{2} \frac {\partial^ {2} f}{\partial X _ {t} ^ {2}} (d X _ {t}) ^ {2},\tag{12.7}
$$

where $( d X _ { t } ) ^ { 2 }$ is interpreted according to the rules 

$$
(d t) ^ {2} = 0, \quad d t d W _ {t} = 0, \quad \mathrm{and} \quad (d W _ {t}) ^ {2} = d t.\tag{12.8}
$$

Thus $( d X _ { t } ) ^ { 2 } = \sigma _ { t } ^ { 2 } d t$ , and we have 

$$
d f (X _ {t}) = \left(\mu_ {t} \frac {\partial f}{\partial X _ {t}} + \frac {1}{2} \sigma_ {t} ^ {2} \frac {\partial^ {2} f}{\partial X _ {t} ^ {2}}\right) d t + \sigma_ {t} \frac {\partial f}{\partial X _ {t}} d W _ {t}.\tag{12.9}
$$

This result has numerous applications. For example, suppose that $X _ { t }$ is a process that satisfies the stochastic diferential equation (12.6). What is the diferential of $f ( X _ { t } ) = \exp { X _ { t } ? }$ According to the Ito rule we have 

$$
\begin{array}{r c l} d e ^ {X _ {t}} & = & \left(\mu_ {t} \frac {\partial e ^ {X _ {t}}}{\partial X _ {t}} + \frac {1}{2} \sigma_ {t} ^ {2} \frac {\partial^ {2} e ^ {X _ {t}}}{\partial X _ {t} ^ {2}}\right) d t + \sigma_ {t} \frac {\partial e ^ {X _ {t}}}{\partial X _ {t}} d W _ {t}. \\ & = & e ^ {X _ {t}} \left[ (\mu_ {t} + \frac {1}{2} - s i g m a _ {t} ^ {2}) d t + \sigma_ {t} d W _ {t} \right] \end{array}\tag{12.10}
$$

Exercise 12.1 Use Ito’s lemma to show that equation (12.2) is a solution of (12.1) when $\mu$ and σ are constant. 

Exercise 12.2 Find the stochastic derivatives of the following processes 

$$
1. X _ {t} = W _ {t} ^ {2} - t
$$

$$
2. X _ {t} = W _ {t} ^ {3} - 3 t W _ {t}
$$

$$
3. X _ {t} = W _ {t} ^ {4} - 6 t W _ {t} ^ {2} + 3 t ^ {2}
$$

where $W _ { t }$ is $a$ Wiener process. What do these processes have in common $\ell$ 

Exercise 12.3 Use Ito’s lemma to show that if $Z _ { t } = X _ { t } Y _ { t }$ , then 

$$
d Z _ {t} = X _ {t} d Y _ {t} + Y _ {t} d X _ {t} + d X _ {t} d Y _ {t}\tag{12.11}
$$

Verify this in the case $X _ { t } = W _ { t }$ and $Y _ { t } = W _ { t } ^ { 2 }$ where $W _ { t }$ is the Wiener process. Hint: consider $( X _ { t } + Y _ { t } ) ^ { 2 } - X _ { t } ^ { 2 } - Y _ { t } ^ { 2 }$ 

Exercise 12.4 Use Ito’s lemma to show that for processes $X _ { t } , Y _ { t }$ we have 

$$
d \left(\frac {X}{Y}\right) = \frac {X}{Y} \left[ \frac {d X}{X} - \frac {d Y}{Y} + \frac {(d Y) ^ {2}}{Y ^ {2}} - \frac {d X d Y}{X Y} \right]\tag{12.12}
$$

## 13 Arbitrage Argument

It is now time to make a first attempt at deriving the Black-Scholes formula for the value of a call option. In fact, we shall derive the Black-Scholes partial diferential equation, which is valid for any derivative. However, it is only in specific simple cases, such as that of a call or put option with constant ‘market parameters’, where an explicit solution can be found. 

## 13.1 Derivation of the No-Arbitrage Condition

Consider a financial market that consists of one basic asset and a money market account. Suppose that the underlying asset has a stochastic price process $S _ { t }$ with dynamics 

$$
d S _ {t} = \mu_ {t} S _ {t} d t + \sigma_ {t} S _ {t} d W _ {t},\tag{13.1}
$$

where $\mu _ { t }$ is the drift and $\sigma _ { t }$ is the volatility. Later we shall specialize to the case where $\mu _ { t }$ and $\sigma _ { t }$ are constant, but for the moment we shall allow these processes to be fairly general, depending on the ‘history’ of $W _ { t }$ between 0 and t. The money market account or bond process $B _ { t }$ satisfies the stochastic diferential equation 

$$
d B _ {t} = r _ {t} B _ {t} d t,\tag{13.2}
$$

where $r _ { t }$ is the instantaneous risk-free interest rate or ‘short rate’. As in the case of the drift and volatility, for now we will only assume that the short rate is adapted to the Brownian motion $W _ { t }$ , but eventually we will take it to be constant. 

In addition to the underlying asset and the bond, we also have an option on $S _ { t } .$ , with price $C _ { t }$ at time t. In fact, for the moment we may suppose that $C _ { t }$ is a fairly general European-style derivative. It is therefore entirely specified by a maturity $T$ and a payof function $C _ { T }$ . Eventually we shall calculate the initial price for the payout 

$$
C (S _ {T}) = \max (S _ {T} - K, 0),\tag{13.3}
$$

that is, a call option. The payof function of a call option was illustrated in figure 1.1. 

What is the stochastic diferential equation satisfied by $C _ { t } ?$ We shall assume that $C _ { t }$ is ‘driven’ by the same randomness that afects $S _ { t }$ , that is, the Wiener process $W _ { t }$ . Hence the derivative price has the dynamics 

$$
d C _ {t} = \mu_ {t} ^ {C} C _ {t} d t + \sigma_ {t} ^ {C} C _ {t} d W _ {t},\tag{13.4}
$$

where $\mu _ { t } ^ { C }$ and $\sigma _ { t } ^ { C }$ are respectively the drift and volatility of the derivative price. Note that the stochastic process $C _ { t }$ does not really need to be a derivative at all! As remarked above, the only condition that we have actually required is that the random part of the ‘derivative’ motion is driven by the same Wiener process $W _ { t }$ that generates the randomness in the asset price process $S _ { t }$ . It turns out that the drifts and volatilities for any two processes that are driven by the same Brownian motion are not independent. That this result follows from an arbitrage argument should not be too surprising—by going long one process and short the other we can eliminate the common source of uncertainty and hence generate a guaranteed return. Any portfolio with a guaranteed return immediately implies that an arbitrage argument is waiting to happen. 

Suppose that an arbitrageur wants to make a risk-free profit (after all, who doesn’t?) by investing in the asset and derivative. Let $\phi _ { t }$ be the trading strategy for the underlying asset, that is, $\phi _ { t }$ tells us how much of the asset that we own at time t. It is the value of the trading strategy that will eventually be determined by the no arbitrage argument. 

A self-financing trading strategy is a trading strategy that has no external cash-flow. That is, any changes in the value of the portfolio are entirely due to changes in the value of the underlying assets and not due to money being put in or taken out of the portfolio in order to fund asset sales or purchases. For example, if we have a single asset with price process $S _ { t }$ and trading strategy $\phi _ { t }$ , then the portfolio value is $V _ { t } = \phi _ { t } S _ { t }$ and the change in the value of the portfolio over a short time interval $[ t , t + d t ]$ is $d V _ { t } = \phi _ { t } d S _ { t } + S _ { t } d \phi _ { t }$ The trading strategy is self-financing only if $S _ { t } d \phi _ { t } = 0$ because this is an external cash-flow, whereas $\phi _ { t } d S _ { t }$ is caused by a change in the value of the asset price. Consider the constant position $\phi _ { t }$ which buys one unit of stock at time 0 and then simply holds onto it. The portfolio value is $V _ { t } = \phi _ { t } S _ { t }$ and the change in the value of the portfolio is simply $d V _ { t } = \phi _ { t } d S _ { t }$ . Hence $\phi _ { t }$ is self-financing. A trading strategy that is not self-financing is $\phi _ { t } = t$ which continuously buys stock. The value of the portfolio is $V _ { t } = t S _ { t }$ , and hence the change in its value over a short time interval is $d V _ { t } = S _ { t } d t + t d S _ { t } ,$ which is not equal to $\phi _ { t } d S _ { t }$ . The amount $S _ { t } d t$ is an external cash-flow that must be added to the portfolio in order to fund the continual asset purchases. 

In the next chapter we will look at trading strategies which consist of positions in both an asset and a bond. In that case the value of a portfolio with a trading strategy $( \phi _ { t } , \psi _ { t } )$ is $V _ { t } = \phi _ { t } S _ { t } + \psi _ { t } B _ { t }$ . The change in a selffinancing strategy must be entirely due to the change in the asset and bond prices, that is $d V _ { t } = \phi _ { t } d S _ { t } + \psi _ { t } d B _ { t }$ . Unlike the single asset case, we no longer have to require that the change in the trading strategy vanishes, that is, we can buy and sell assets and bonds, but we do require that the additional terms that arise from these sales and purchases cancel each other in such a way that no external cash-flow is required. For example, if we want to increase our asset holdings $\phi _ { t }$ , then the money to fund this purchase must come from a correspondingly shorter position $\psi _ { t }$ in the bond. We can make the trading strategy $\phi _ { t } = t$ into a self-financing one by adding a bond position of 

$$
\psi_ {t} = - \int_ {0} ^ {t} \frac {S _ {u}}{B _ {u}} d u,\tag{13.5}
$$

which simply borrows the money from the bond market to pay for the purchases in the asset market, which means that $S _ { t } d \phi _ { t } + B _ { t } d \psi _ { t } = 0$ . Selffinancing strategies are very important for arbitrage arguments because we cannot require a portfolio that starts with no net position to end with similarly no net value if there is an external cash-flow which adds or subtracts money from the position. 

Now back to the arbitrage argument. As in our previous examples, the arbitrageur begins at time t with no money. He then buys one option for $C _ { t }$ dollars and assumes a short position in $\phi _ { t }$ units of the underlying asset. Note that we assume that the asset can be bought and sold in any quantity. Setting up this portfolio costs $V _ { t } = C _ { t } - \phi _ { t } S _ { t }$ dollars, which must be funded by a bank loan. Interest accumulates continuously on this loan at the rate $r _ { t } .$ , so that after a small time interval dt the arbitrageur owes an additional $r _ { t } V _ { t } d t$ dollars to the bank. 

But what is the value of $\phi _ { t }$ , that is, how much of the asset are we shorting? Just as in the discrete time case, the ‘arbitrage strategy’ $\phi _ { t }$ is chosen so that the risk or randomness in holding the option exactly cancels the risk in holding the asset. This is the only way to ensure the guaranteed return necessary for an arbitrage argument. So what is the return on the arbitrageur’s portfolio? Well, the value of his position at any time t is 

$$
V _ {t} = C _ {t} - \phi_ {t} S _ {t}.\tag{13.6}
$$

Assuming that we do not adjust the value of $\phi _ { t }$ , that is we neither buy nor sell any underlying assets, then the change in the value of the portfolio $V _ { t }$ over the short time interval $[ t , t + d t ]$ is 

$$
\begin{array}{r c l} {d V _ {t}} & = & {d C _ {t} - \phi_ {t} d S _ {t}} \\ & = & {C _ {t} (\mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t}) - \phi_ {t} S _ {t} (\mu_ {t} d t + \sigma_ {t} d W _ {t})} \\ & = & {(\mu_ {t} ^ {C} C _ {t} - \phi_ {t} \mu_ {t} S _ {t}) d t + (\sigma_ {t} ^ {C} C _ {t} - \phi_ {t} \sigma_ {t} S _ {t}) d W _ {t},} \end{array}\tag{13.7}
$$

where we have assumed that the asset and option prices obey equations (13.1) and (13.4) respectively. We can now fix $\phi _ { t }$ by setting the coeficient of $d W _ { t }$ to zero. This ensures that the arbitrageur’s asset and option portfolio ofers a definite rate of return over the small time interval $d t$ . Hence 

$$
\phi_ {t} = \frac {\sigma_ {t} ^ {C} C _ {t}}{\sigma_ {t} S _ {t}},\tag{13.8}
$$

and we call this value of $\phi _ { t }$ the arbitrage strategy. We can then calculate the change in the value of the position when the arbitrage strategy is used, 

$$
\begin{array}{r c l} {d V _ {t}} & = & {(\mu_ {t} ^ {C} C _ {t} - \phi_ {t} \mu_ {t} S _ {t}) d t} \\ & = & {\left(\mu_ {t} ^ {C} - \frac {\sigma_ {t} ^ {C} \mu_ {t}}{\sigma_ {t}}\right) C _ {t} d t.} \end{array}\tag{13.9}
$$

But the arbitrageur can make a risk-free profit if the drift in equation (13.9) yields a monetary gain greater than the interest payment $r _ { t } V _ { t } d t$ on the loan. This follows because at time $t + d t$ , the value of the arbitrageur’s asset and option portfolio is $V _ { t } + d V _ { t }$ , while the amount owed to the bank is $V _ { t } + r _ { t } V _ { t } d t$ Hence his net position is the risk-free amount $d V _ { t } - r _ { t } V _ { t } d t$ . Since he started with no money, the no arbitrage argument tells us that his final position must also be zero, and thus 

$$
d V _ {t} = r _ {t} V _ {t} d t.\tag{13.10}
$$

This implies that 

$$
\begin{array}{r c l} d V _ {t} & = & r _ {t} (C _ {t} - \phi_ {t} S _ {t}) d t \\ & = & r _ {t} \left(1 - \frac {\sigma_ {t} ^ {C}}{\sigma_ {t}}\right) C _ {t} d t, \end{array}\tag{13.11}
$$

where we have used the value of $V _ { t }$ from equation (13.6), and substituted in the arbitrage trading strategy $\phi _ { t }$ , as given by equation (13.8). 

Equating equations (13.9) and (13.11) we get 

$$
\mu_ {t} ^ {C} - \frac {\sigma_ {t} ^ {C} \mu_ {t}}{\sigma_ {t}} = r _ {t} \left(1 - \frac {\sigma_ {t} ^ {C}}{\sigma_ {t}}\right).\tag{13.12}
$$

After some rearrangement we obtain the formula 

$$
\frac {\mu_ {t} ^ {C} - r _ {t}}{\sigma_ {t} ^ {C}} = \frac {\mu_ {t} - r _ {t}}{\sigma_ {t}}.\tag{13.13}
$$

This is the general relation between $\mu _ { t } ^ { C } , \mu _ { t } , \sigma _ { t } ^ { C } , \sigma _ { t }$ and $r _ { t }$ that is required if there is to be no arbitrage between the option and the underlying. We therefore call this the no arbitrage condition. Note that we have made no specific assumptions about the form of the volatility, drift or short-rate processes, or even what kind of derivative that we are speaking of (except that its value, like that of $S _ { t }$ , should be determined by a knowledge of $W _ { t }$ between 0 and $t )$ , so that relation (13.13) is quite general. In fact, $C _ { t }$ does not even need to be a derivative, but rather it can be any price process that is driven by the same Brownian motion as $S _ { t }$ . In economic terms (13.13) says that the rate of return above the risk-free rate, per unit of risk, that is, volatility, has to be the same for any two processes governed by the same random motions. 

## 13.2 Derivation of the Black-Scholes Equation

To proceed further, we now assume that at each time t the derivative price $C _ { t }$ can be specified in terms of a function $C _ { t } = C ( S _ { t } , t )$ of just the asset price and time. This is true for a call option and many other standard types of derivatives. The big advantage of this assumption is that it allows us to apply Ito’s lemma to the derivative price, 

$$
\begin{array}{r c l} d C _ {t} & = & \frac {\partial C _ {t}}{\partial t} d t + \frac {\partial C _ {t}}{\partial S _ {t}} d S _ {t} + \frac {1}{2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} (d S _ {t}) ^ {2} \\ & = & \left(\frac {\partial C _ {t}}{\partial t} + \frac {\partial C _ {t}}{\partial S _ {t}} \mu_ {t} S _ {t} + \frac {1}{2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} S _ {t} ^ {2} \sigma_ {t} ^ {2}\right) d t + \frac {\partial C _ {t}}{\partial S _ {t}} S _ {t} \sigma_ {t} d W _ {t}. \end{array}\tag{13.14}
$$

Comparing the terms from this result with the coeficients of dt and $d W _ { t }$ in the original price process (13.4) 

$$
d C _ {t} = \mu_ {t} ^ {C} C _ {t} d t + \sigma_ {t} ^ {C} C _ {t} d t,\tag{13.15}
$$

we deduce that 

$$
\mu_ {t} ^ {C} C _ {t} = \frac {\partial C _ {t}}{\partial t} + \frac {\partial C _ {t}}{\partial S _ {t}} \mu_ {t} S _ {t} + \frac {1}{2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} S _ {t} ^ {2} \sigma_ {t} ^ {2},\tag{13.16}
$$

and 

$$
\sigma_ {t} ^ {C} C _ {t} = \frac {\partial C _ {t}}{\partial S _ {t}} S _ {t} \sigma_ {t}.\tag{13.17}
$$

If we then use these expressions to substitute for $\mu _ { t } ^ { C }$ and $\sigma _ { t } ^ { C }$ in the no arbitrage condition (13.13) obtained earlier, we get 

$$
\frac {\partial C}{\partial t} + \frac {\partial C}{\partial S _ {t}} \mu_ {t} S _ {t} + \frac {1}{2} \frac {\partial^ {2} C}{\partial S _ {t} ^ {2}} S _ {t} ^ {2} \sigma_ {t} ^ {2} - r _ {t} C = (\mu_ {t} - r _ {t}) \frac {\partial C}{\partial S _ {t}} S _ {t}.\tag{13.18}
$$

Note that the terms involving $\mu _ { t }$ on the right and left miraculously cancel, and we are left with the equation 

$$
\frac {\partial C}{\partial t} + \frac {1}{2} \frac {\partial^ {2} C}{\partial S ^ {2}} S _ {t} ^ {2} \sigma_ {t} ^ {2} = r _ {t} \left(C _ {t} - \frac {\partial C}{\partial S} S _ {t}\right).\tag{13.19}
$$

This is the famous Black-Scholes partial diferential equation for the price of a derivative. Note that it is independent of the drift of the asset price and both the drift and volatility of the derivative price. 

Exercise 13.1 We can also derive the Black-Scholes equation in the $f o l -$ lowing equivalent manner. Begin with nothing and take the position $V _ { t } ~ =$ $C _ { t } - \phi _ { t } S _ { t } - \psi _ { t } B _ { t }$ . Then use an arbitrage argument on the value of the portfolio at time $t + d t$ , where the stock and bond holdings are kept fixed over the time interval $[ t , t + d t ]$ 

To value a derivative we need to impose a ‘boundary condition’ on the diferential equation (13.19). This will take the form of a specification of the terminal pay-of function of the derivative. In the case of a call option, for example, we want 

$$
C _ {T} = \max (S _ {T} - K, 0).\tag{13.20}
$$

The idea is to solve for $C _ { t }$ as a function of $S _ { t }$ and t for values of t less than $T$ . In particular, we want the value of $C _ { 0 }$ , which is the initial price of the derivative. The solution of equation (13.19) for constant values of $\sigma _ { t } , \mu _ { t }$ , and $r _ { t } ,$ subject to the call option boundary condition, is given by 

$$
C (S _ {t}, t) = e ^ {- r (T - t)} [ S _ {t} e ^ {r (T - t)} N (h ^ {+}) - K N (h ^ {-}) ],\tag{13.21}
$$

where 

$$
h ^ {\pm} = \frac {\ln (S _ {t} e ^ {r (T - t)} / K) \pm \frac {1}{2} \sigma^ {2} (T - t)}{\sigma \sqrt {T - t}},\tag{13.22}
$$

and $N ( x )$ is the cumulative probability function for the $N ( 0 , 1 )$ normal distribution, 

$$
N (x) = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {x} e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{13.23}
$$

One can verify that (13.21) and (13.22) do indeed solve (13.19) for constant drift and volatilities, subject to the condition (13.20). This involves quite a bit of calculation. In fact, there is a quicker way of getting this result, by use of martingale arguments, which we shall look at later. This by-passes the need for solving the diferential equation (13.19). Nevertheless as a piece of elegant mathematics it is very instructive to see how (13.19) leads to (13.21). Form a numerical point of view, the partial diferential approach is the best way to obtain a price for an exotic derivative. 

Exercise 13.2 Calculate the price for a 6-month option with a strike of $115, if the initial cost of the asset is $100, the volatility is 20% per year and the risk-free interest rate is 5% per year. 

## 14 Replication Portfolios

We have seen that if an asset price $S _ { t }$ moves according to the process $d S _ { t } =$ $\mu _ { t } S _ { t } d t + \sigma _ { t } S _ { t } d W _ { t }$ , and if a derivative based on the asset moves according to the process $d C _ { t } = \mu _ { t } ^ { C } C _ { t } d t + \sigma _ { t } ^ { C } C _ { t } d W _ { t } ,$ , and if the money market account process $B _ { t }$ satisfies $d B _ { t } = r _ { t } B _ { t } d t$ , then to avoid arbitrage the relation $( \mu _ { t } ^ { C } - r _ { t } ) / \sigma _ { t } ^ { C } =$ ${ \left( { \mu _ { t } - r _ { t } } \right) } / { \sigma _ { t } }$ must hold. This ensures that if we hold a portfolio $V _ { t }$ that is long one derivative and short $\phi _ { t }$ units of the asset, and $\phi _ { t }$ is chosen so that the return on the position is riskless, that is $\phi _ { t } = \sigma _ { t } ^ { C } C _ { t } / \sigma _ { t } S _ { t }$ , then this riskless rate of return is equal to the risk-free short-rate $r _ { t }$ 

In this chapter we shall demonstrate a complementary result, namely that a position in the derivative can be replicated by a portfolio composed of holdings in both the underlying asset and the money market account. Recall that going long in the money market is equivalent to investing money at the rate $r _ { t }$ , while going short is the same as borrowing money at the same rate $r _ { t }$ 

So, how can we replicate the derivative? We begin by recalling that if we follow the arbitrage strategy $\phi _ { t }$ , then we obtain a fixed return on the position $V _ { t }$ , given by $d V _ { t } = r _ { t } V _ { t } d t$ . But this rate of return is equal to the rate of return obtained by an investment in the money market account, as required by the no arbitrage argument. So instead of buying the derivative and selling $\phi _ { t }$ units of the asset, that is taking the position $V _ { t } .$ , we could achieve the same efect by setting up a portfolio $\hat { V } _ { t }$ which simply invests $\psi _ { t }$ in the money market account. Since we want the portfolios to have the same value at time t, we clearly set 

$$
\psi_ {t} = V _ {t} / B _ {t}.\tag{14.1}
$$

If we hold our investment in the bond fixed, then the change in the value of this portfolio between time t and time $t + d t$ is 

$$
\begin{array}{r c l} {d \bar {V} _ {t}} & = & {\psi_ {t} d B _ {t}} \\ & = & {\psi_ {t} r _ {t} B _ {t} d t} \\ & = & {r _ {t} V _ {t} d t} \\ & = & {d V _ {t}.} \end{array}\tag{14.2}
$$

Thus, $\hat { V } _ { t }$ exactly replicates $V _ { t }$ and the two processes must therefore be equal. But this means that 

$$
\psi_ {t} B _ {t} = C _ {t} - \phi_ {t} S _ {t},\tag{14.3}
$$

and hence 

$$
C _ {t} = \psi_ {t} B _ {t} + \phi_ {t} S _ {t}.\tag{14.4}
$$

In essence what we have done is first calculated $\phi _ { t }$ using a no arbitrage argument, and then simply defined $\psi _ { t }$ by equation (14.4). 

Exercise 14.1 We want to show that the trading strategy $\left( \phi _ { t } , \psi _ { t } \right)$ defined by equations (13.8) and (14.4) is self-financing. 

(a) Begin by showing that 

$$
d \left(\frac {C _ {t}}{B _ {t}}\right) = \phi_ {t} d \left(\frac {S _ {t}}{B _ {t}}\right).\tag{14.5}
$$

We could, in $f a c t ,$ use this as a defintion of $\phi _ { t }$ . 

(b) Next, calculate the change in the bond position, $B _ { t } d \psi _ { t }$ 

(c) Finally, use these two results to verify that 

$$
d C _ {t} = \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t},\tag{14.6}
$$

which means that the trading strategy is indeed self-financing. 

This portfolio consisting of $\phi _ { t }$ units of the underlying asset and $\psi _ { t }$ units of the money market account is called the replication portfolio. Its importance can be seen by considering the risk associated with derivatives. Suppose that at time 0 an investment bank sells a derivative to a client at a price $C _ { 0 }$ Then at time $T$ it will have to pay the client $C _ { T }$ . This involves risk for the bank, since, depending on the value of $C _ { T }$ it might lose money. However, if the $C _ { 0 }$ from the sale of the option is immediately invested to synthesize a replication portfolio, then the value of the replication portfolio at time $T$ will automatically be $C _ { T }$ , which can be paid directly to the client. Thus, there is no risk that the bank will make a loss. Actually the bank cannot make a profit either, unless a price somewhat greater than $C _ { 0 }$ is actually charged for the derivative. 

So, why do we need derivatives at all, if we can replicate them with an appropriate portfolio? The reason is that the trading strategies $\phi _ { t }$ and $\psi _ { t }$ require continuous attention and re-adjustment which the client may wish to avoid, and indeed may not have the facility to carry out eficiently. 

The value of $\phi _ { t }$ in equation (13.8) is not very practical since it is defined in terms of two unknown volatilities $\sigma _ { t } ^ { C }$ and $\sigma _ { t }$ . A more useful expression can be obtained from equation (14.6), 

$$
\phi_ {t} = \frac {\partial C _ {t}}{\partial S _ {t}}.\tag{14.7}
$$

This tells you how much stock needs to be held at time t in order to replicate the ‘risky’ part of the motion of $C _ { t }$ . Intuitively, if the underlying asset moves by a small amount $\Delta S _ { t } .$ , then the first order change in the derivative price should be $( \Delta S _ { t } ) \partial C _ { t } / \partial S _ { t }$ . Hence if we are long one derivative and short $\phi _ { t }$ units of stock, then the two changes will cancel one another. The quantity $\phi _ { t }$ is generally called the ‘Delta’ of the derivative. 

What is the value of the bond position in our replicating portfolio? Substituting equation (14.7) into equation (14.4), which defines $\psi _ { t }$ , we see that 

$$
\psi_ {t} = \frac {1}{B _ {t}} \left(C _ {t} - \frac {\partial C _ {t}}{\partial S _ {t}} S _ {t}\right).\tag{14.8}
$$

This tells you how much money needs to be invested in the money market account when you are trying to replicate the derivative. 

## 15 Solving the Black-Scholes Equation

We now want to solve the Black-Scholes equation for a general ‘European’ payof, assuming that the drift, volatility, and interest rates are all constant. In this case the stochastic asset price process is 

$$
d S _ {t} = \mu S _ {t} d t + \sigma S _ {t} d W _ {t}.\tag{15.1}
$$

In exercise (12.1) we verified that the solution of this stochastic diferential equation is 

$$
S _ {t} = S _ {0} e ^ {\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t},\tag{15.2}
$$

where $S _ { 0 }$ is the initial price of the asset. If $C ( S _ { t } , t )$ is the value of a derivative at time t which expires at time $T ,$ , then in the previous two chapters we showed that for $0 \leq t \leq T$ it must satisfy the Black-Scholes partial diferential 

$$
\frac {\partial C _ {t}}{\partial t} + \frac {1}{2} \sigma_ {t} ^ {2} S _ {t} ^ {2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} = r \left(C _ {t} - \frac {\partial C _ {t}}{\partial S _ {t}} S _ {t}\right).\tag{15.3}
$$

Our goal is to solve this equation subject to the specification of a general payof function $C ( S _ { T } , T ) = f ( S _ { T } )$ at the expiry time T. In the event that the derivative is a call option with payof max $[ S _ { T } - K , 0 ]$ , then we can obtain a nice analytic formula for the initial price, known as the Black-Scholes formula. In the case of a more general derivative we shall demonstrate, just as in the discrete time case, that the initial price can be expressed as a discounted expectation of the payof function. 

To begin with, we note that the Black-Scholes equation (15.3) has a passing similarity to the more common heat equation 

$$
\frac {\partial A (x , \tau)}{\partial \tau} = \frac {1}{2} \sigma^ {2} \frac {\partial^ {2} A (x , \tau)}{\partial x ^ {2}}.\tag{15.4}
$$

In fact, by a series of transformations the Black-Scholes equation can be reduced to the heat equation. this means that we can solve for the derivative price by a two-step method. First, we show how to solve the heat equation (15.4) subject to a prescribed initial condition $A ( x , 0 ) = f ( x )$ . Second, we explicitly demonstrate the transformations needed to convert the Black-Scholes equation to the heat equation. By combining these two results we can write down the solution to the Black-Scholes equation for a derivative with an arbitrary European payof. 

## 15.1 Solution of the Heat Equation

Let $W _ { \tau }$ be a standard Brownian motion. If we consider a function $f ( x + W _ { \tau } )$ then from Ito’s lemma we see that 

$$
d f (x + W _ {\tau}) = \frac {\partial f (x + W _ {\tau})}{\partial W _ {\tau}} d W _ {\tau} + \frac {1}{2} \frac {\partial^ {2} f (x + W _ {\tau})}{\partial W _ {\tau} ^ {2}} d \tau .\tag{15.5}
$$

Note that we want to treat x as a parameter rather than a variable, and hence have ignored it in deriving the stochastic diferential equation. If we integrate this equation with respect to $\tau$ then we obtain 

$$
f (x + W _ {\tau}) = f (x) + \int_ {0} ^ {\tau} \frac {\partial f (x + W _ {s})}{\partial W _ {s}} d W _ {s} + \frac {1}{2} \int_ {0} ^ {\tau} \frac {\partial^ {2} f (x + W _ {s})}{\partial W _ {s} ^ {2}} d s,\tag{15.6}
$$

where we have used the fact that $W _ { 0 } = 0$ . We then notice that diferentiating $f ( x + W _ { \tau } )$ with respect to $W _ { \tau }$ is the same as diferentiating it with respect to x, that is 

$$
\frac {\partial f (x + W _ {\tau})}{\partial W _ {\tau}} = \frac {\partial f (x + W _ {\tau})}{\partial x} \quad \text {and} \quad \frac {\partial^ {2} f (x + W _ {\tau})}{\partial W _ {\tau} ^ {2}} = \frac {\partial^ {2} f (x + W _ {\tau})}{\partial x ^ {2}}.\tag{15.7}
$$

This is useful because we want to derive the heat equation, which involves derivatives with respect to a real quantity $x ,$ rather than a stochastic variable like $W _ { \tau }$ . Substituting these results into the equation for $f ( x + W _ { \tau } )$ we obtain 

$$
f (x + W _ {\tau}) = f (x) + \int_ {0} ^ {\tau} \frac {\partial f (x + W _ {s})}{\partial x} d W _ {s} + \frac {1}{2} \int_ {0} ^ {\tau} \frac {\partial^ {2} f (x + W _ {s})}{\partial x ^ {2}} d s.\tag{15.8}
$$

If we take an expectation on each side of this equation, then the stochastic integral vanishes, and we obtain 

$$
E [ f (x + W _ {\tau}) ] = f (x) + \frac {1}{2} \int_ {0} ^ {\tau} \frac {\partial^ {2} E [ f (x + W _ {s}) ]}{\partial x ^ {2}} d s.\tag{15.9}
$$

Exercise 15.1 By using the definition of a stochastic integral show that for any well-behaved function $g ( W _ { t } )$ 

$$
E \left[ \int_ {0} ^ {t} g (W _ {s}) d W _ {s} \right] = 0,\tag{15.10}
$$

and hence we are justified in discarding the expectation of the stochastic integral in equation (15.9). 

If we define the function 

$$
A (x, \tau) = E [ f (x + W _ {\tau}) ],\tag{15.11}
$$

then equation (15.9) becomes 

$$
A (x, \tau) = f (x) + \frac {1}{2} \int_ {0} ^ {\tau} \frac {\partial^ {2} A (x , s)}{\partial x ^ {2}} d s.\tag{15.12}
$$

Diferentiating with respect to $\tau _ { : }$ we see that $A ( x , \tau )$ satisfies the heat equation 

$$
\frac {\partial A (x , \tau)}{\partial \tau} = \frac {1}{2} \frac {\partial^ {2} A (x , \tau)}{\partial x ^ {2}}.\tag{15.13}
$$

Furthermore, if we evaluate $A ( x , \tau )$ at $\tau = 0$ we see that 

$$
\begin{array}{r c l} A (x, 0) & = & E [ f (x + W _ {0}) ] \\ & = & E [ f (x) ] \\ & = & f (x), \end{array}\tag{15.14}
$$

that is, $A ( x , \tau )$ satisfies the initial condition $A ( x , 0 ) = f ( x )$ . Thus, we now have a recipe for solving the heat equation subject to a given initial condition. Specifically, if $A ( x , \tau )$ satisfies the heat equation (15.13) and is subject to the initial condition $A ( x , 0 ) = f ( x )$ , then 

$$
\begin{array}{r c l} A (x, \tau) & = & E [ f (x + W _ {\tau}) ] \\ & = & \frac {1}{\sqrt {2 \pi \tau}} \int_ {- \infty} ^ {\infty} f (x + \xi) e ^ {- \frac {\xi^ {2}}{2 \tau}} d \xi . \end{array}\tag{15.15}
$$

Somewhat more generally, but by an identical argument, we find that 

$$
A (x, \tau) = E [ f (x + \sigma W _ {\tau}) ]\tag{15.16}
$$

satisfies the equation 

$$
\frac {\partial}{\partial \tau} A (x, \tau) = \frac {1}{2} \sigma^ {2} \frac {\partial^ {2}}{\partial x ^ {2}} A (x, \tau),\tag{15.17}
$$

subject to the initial condition $A ( x , 0 ) = f ( x )$ 

Exercise 15.2 Verify that $A ( x , \tau )$ as defined by equation (15.16) satisfies the partial diferential equation (15.17). 

For fixed $\tau ,$ the random variable $W _ { \tau }$ is normally distributed with mean 0 and variance τ . We can therefore rewrite the solution (15.16) as 

$$
A (x, \tau) = E [ f (x + \sigma \sqrt {\tau} Z) ],\tag{15.18}
$$

where $Z$ is a standard $N ( 0 , 1 )$ random variable. Explicitly writing out the expectation we have 

$$
A (x, \tau) = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} f (x + \sigma \sqrt {\tau} \xi) e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{15.19}
$$

Once we have transformed the Black-Scholes equation into the heat equation we will be able to use this result to calculate solutions of the Black-Scholes equation, and hence derivative prices. 

## 15.2 Reduction of the Black-Scholes Equation to the Heat Equation

Armed with this result we return to the Black-Scholes equation (15.3) and make a series of crafty transformations in order to reduce it to the heat equation (15.17). Proceed as follows: 

1. We need to reverse the direction of time, so that the terminal payout of the Black-Scholes equation becomes the initial condition for the heat equation. Set $C ( S , t ) = \alpha ( S , \tau )$ , where $\tau = T - t$ is a new time coordinate which still runs over the same interval $[ 0 , T ]$ as t, but in the opposite direction. The derivative expiry time $T$ is, of course, a constant. The time derivatives of $C ( S , t )$ and $\alpha ( S , \tau )$ are related by 

$$
\frac {\partial C}{\partial t} = - \frac {\partial \alpha}{\partial \tau},\tag{15.20}
$$

while all the other derivatives remain the same. Hence the Black-Scholes equation becomes 

$$
\frac {\partial \alpha}{\partial \tau} = \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} \alpha}{\partial S ^ {2}} + r S \frac {\partial \alpha}{\partial S} - r \alpha .\tag{15.21}
$$

This equation now has the ‘right’ sign for the time derivative, and has the initial condition 

$$
\begin{array}{r c l} \alpha (S _ {T}, 0) & = & C (S _ {T}, T) \\ & = & F (S _ {T}, T). \end{array}\tag{15.22}
$$

2. We now want to eliminate the rα term. We can do this by introducing a ‘discount factor’ e−<sup>rτ</sup> explicitly into the equation. Set $\alpha ( S , \tau ) = \beta ( S , \tau ) e ^ { - r \tau }$ The time derivative is then 

$$
\frac {\partial \alpha}{\partial \tau} = \left(\frac {\partial \beta}{\partial \tau} - r \beta\right) e ^ {- r \tau},\tag{15.23}
$$

and hence equation (15.21) can be written as 

$$
\frac {\partial \beta}{\partial \tau} = \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} \beta}{\partial S ^ {2}} + r S \frac {\partial \beta}{\partial S}.\tag{15.24}
$$

3. To proceed further, we want to write the equation in terms of the operator $S \mathrm { { } } \partial / \partial S$ . This can be easily accomplished by rearranging the second order term, 

$$
\frac {\partial \beta}{\partial \tau} = \frac {1}{2} \sigma^ {2} S \frac {\partial}{\partial S} \left(S \frac {\partial \beta}{\partial S}\right) + (r - \frac {1}{2} \sigma^ {2}) S \frac {\partial \beta}{\partial S}.\tag{15.25}
$$

4. We can simplify the operator $S \mathrm { { } } \partial / \partial S$ by defining the new variable $Y = \ln { S }$ , and noting that 

$$
S \frac {\partial}{\partial S} = \frac {\partial}{\partial Y}.\tag{15.26}
$$

If we then introduce the new function $\gamma ( Y , \tau ) \ : = \ : \beta ( S , \tau )$ , we see that the diferential equation (15.25) becomes 

$$
\frac {\partial \gamma}{\partial \tau} = \frac {1}{2} \sigma^ {2} \frac {\partial^ {2} \gamma}{\partial Y ^ {2}} + (r - \frac {1}{2} \sigma^ {2}) \frac {\partial \gamma}{\partial Y}.\tag{15.27}
$$

5. Finally, we need to get rid of the first order partial derivative. Define $X = Y + ( r - { \textstyle { \frac { 1 } { 2 } } } \sigma ^ { 2 } ) \tau$ , and set $A ( X , \tau ) = \gamma ( Y , \tau )$ . The partial derivative of $\gamma$ with respect to τ is then given by 

$$
\begin{array}{r c l} \frac {\partial \gamma}{\partial \tau} & = & \frac {\partial A}{\partial \tau} + \frac {\partial A}{\partial X} \frac {\partial X}{\partial \tau} \\ & = & \frac {\partial A}{\partial \tau} + \frac {\partial A}{\partial X} (r - \frac {1}{2} \sigma^ {2}). \end{array}\tag{15.28}
$$

However, since 

$$
\frac {\partial \gamma}{\partial Y} = \frac {\partial A}{\partial X}\tag{15.29}
$$

it follows that if we substitute (15.28) and (15.29) into equation (15.27) then the first order derivatives with respect to X cancel and we obtain 

$$
\frac {\partial A}{\partial \tau} = \frac {1}{2} \sigma^ {2} \frac {\partial^ {2} A}{\partial X ^ {2}},\tag{15.30}
$$

which is the heat equation at last! 

Now that we have shown that the Black-Scholes equation can be reduced by a series of transformations to the heat equation, we would like to solve for the derivative price $C ( S _ { t } , t )$ subject to the terminal condition 

$$
C (S _ {T}, T) = F (S _ {T}),\tag{15.31}
$$

where $F ( S _ { T } )$ is a prescribed function, that is, the payof function of the derivative. As noted earlier, $t = T$ corresponds to $\tau = 0$ , which is why the terminal payof function of the derivative is actually an initial condition for $A ( x , \tau )$ . If we follow through the various transformations made above, then we see that the relation between $C ( S _ { t } , t )$ and $A ( X , \tau )$ is 

$$
\begin{array}{r c l} {C (S _ {t}, t)} & = & {\alpha (S _ {t}, T - t)} \\ & = & {\beta (S _ {t}, T - t) e ^ {- r (T - t)}} \\ & = & {\gamma (\log S _ {t}, T - t) e ^ {- r (T - t)}} \\ & = & {A (\log S _ {t} + [ r - \sigma^ {2} / 2 ] [ T - t ], T - t) e ^ {- r (T - t)}.} \end{array}\tag{15.32}
$$

In particular the derivative payof function can be written as 

$$
\begin{array}{r c l} F (S _ {T}) & = & C (S _ {T}, T) \\ & = & A (\log S _ {T}, 0). \end{array}\tag{15.33}
$$

Hence the initial condition on $A ( x , \tau )$ at $\tau = 0$ is 

$$
A (x, 0) = F \left(e ^ {x}\right).\tag{15.34}
$$

For example, in the case of a call option we have 

$$
A (x, 0) = \max (e ^ {x} - K, 0).\tag{15.35}
$$

We can now appeal to our earlier formula (15.19) for the solution of the heat equation with the initial condition $A ( x , 0 ) = F ( e ^ { x } )$ 

$$
A (x, \tau) = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F (e ^ {x + \sigma \sqrt {\tau} \xi}) e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{15.36}
$$

Using this value of $A ( x , \tau )$ and the transformation (15.19) we can then write the derivative price as 

$$
\begin{array}{r c l} C (S _ {t}, t) & = & A (\log S _ {t} + [ r - \sigma^ {2} / 2 ] [ T - t ], T - t) e ^ {- r (T - t)} \\ & = & \frac {e ^ {- r (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F (S _ {t} e ^ {r (T - t) + \sigma \sqrt {\tau} \xi - \frac {1}{2} \sigma^ {2} \tau}) e ^ {- \frac {1}{2} \xi^ {2}} d \xi . \end{array}\tag{15.37}
$$

In particular, if we set $t = 0$ , then we obtain the initial price of the derivative 

$$
C _ {0} = \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F (S _ {0} e ^ {r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T}) e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{15.38}
$$

We see that the present value of the derivative depends on the expiry date $T$ , the initial asset price $S _ { 0 }$ , the volatility $\sigma .$ , the risk-free interest rate $r$ and the specification of the payof function $F ( S _ { T } )$ 

Note that, similar to the discrete case, we can write the derivative price in terms of an expectation 

$$
C _ {0} = e ^ {- r T} E ^ {*} [ F (S _ {T}) ],\tag{15.39}
$$

where 

$$
S _ {T} = S _ {0} e ^ {r T + \sigma W _ {T} ^ {*} - \frac {1}{2} \sigma^ {2} T}.\tag{15.40}
$$

$W _ { T } ^ { * }$ is a random variable that is normally distributed with mean zero and variance $T$ with respect to some new probability measure $P ^ { * }$ . This is the ‘risk-neutral’ measur $\mathrm { e , }$ just as in the discrete case. 

Before proceeding to the call and ut options, we can begin by pricing the ‘trivial’ derivative that simply delivers $S _ { T }$ at time $T _ { i }$ , that is, $F ( S _ { T } ) = S _ { T }$ The price of this derivative is 

$$
\begin{array}{r c l} {C _ {0}} & = & {e ^ {- r T} E ^ {*} [ F (S _ {T}) ]} \\ & = & {e ^ {- r T} E ^ {*} [ S _ {T} ]} \\ & = & {e ^ {- r T} E ^ {*} [ S _ {0} e ^ {r T + \sigma W _ {T} ^ {*} - \frac {1}{2} \sigma^ {2} T} ]} \\ & = & {S _ {0} e ^ {- \frac {1}{2} \sigma^ {2} T} E ^ {*} [ e ^ {\sigma W _ {T} ^ {*}} ].} \end{array}\tag{15.41}
$$

Using lemma 11.1 we can evaluate the expectation as 

$$
E ^ {*} [ e ^ {\sigma W _ {T} ^ {*}} ] = e ^ {\frac {1}{2} \sigma^ {2} T},\tag{15.42}
$$

and hence see that the derivative price is imply 

$$
C _ {0} = S _ {0},\tag{15.43}
$$

which is what we should expect. 

Exercise 15.3 Price a forward contract with strike K. This has a payof function $F ( S _ { T } ) = S _ { T } - K$ 

## 16 Call and Put Option Prices

Formula (15.38) is a great breakthrough. It says that by performing an integral we can price any European derivative with a payof function that depends only on the final asset price. Note that it does not allow us to calculate prices for either American exercise or path-dependent derivatives. However, there are still plenty of examples for us to consider. In this chapter we want to calculate the initial prices of the two of the most widely traded derivatives–call and put options. 

## 16.1 Call Option

Recall that the call option payof is 

$$
F (S _ {T}) = \max (S _ {T} - K, 0).\tag{16.1}
$$

Hence the initial price of the derivative is 

$$
\begin{array}{r c l} C _ {0} & = & \frac {e ^ {-} r T}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F \left(S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right]\right) \exp \left[ - \frac {1}{2} \xi^ {2} \right] \\ & = & \frac {e ^ {-} r T}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \max \left(S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K, 0\right) \\ & & \times \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi . \end{array}\tag{16.2}
$$

In order to evaluate the integral we need to remove the max function. This can easily be accomplished because it will be nonzero only when 

$$
S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K > 0,\tag{16.3}
$$

which is equivalent to 

$$
\exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] > K / S _ {0}.\tag{16.4}
$$

Taking logarithms of both sides we obtain 

$$
r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T > \log (K / S _ {0}).\tag{16.5}
$$

We then want to isolate the integration variable ξ. This will allow us to discover the integration region where the max function is nonzero. We find that 

$$
\xi > \frac {\log (K / S _ {0}) - (r T - \frac {1}{2} \sigma^ {2} T)}{\sigma \sqrt {T}}.\tag{16.6}
$$

If we define the critical value $\xi ^ { * }$ to be 

$$
\xi^ {*} = \frac {\log (K / S _ {0}) - (r T - \frac {1}{2} \sigma^ {2} T)}{\sigma \sqrt {T}},\tag{16.7}
$$

then the max function can be written as 

$$
\begin{array}{c} \max \left(S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K, 0\right) \\ = \left\{ \begin{array}{l l} S _ {0} e ^ {r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T} - K & \xi > \xi^ {*} \\ 0 & \xi <   \xi^ {*}. \end{array} \right. \end{array}\tag{16.8}
$$

Since the integrand vanishes for $\xi < \xi ^ { * }$ , we only need to integrate over the region where $\xi > \xi ^ { * }$ and the max function takes on a positive value. Hence the derivative price becomes 

$$
C _ {0} = \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} \left(S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K\right) \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi .\tag{16.9}
$$

This integral involves two terms, and it is easiest to evaluate them separately. If we define 

$$
\begin{array}{r c l} I _ {1} & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi \\ & = & \frac {1}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} S _ {0} \exp \left[ - \frac {1}{2} \xi^ {2} + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] \end{array}\tag{16.10}
$$

and 

$$
I _ {2} = - K \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi ,\tag{16.11}
$$

then the derivative price is simply the sum of the two integrals, $C _ { 0 } = I _ { 1 } + I _ { 2 }$ The second integral is easier, so we shall calculate it first. Before we do this, consider the following result 

$$
\begin{array}{r c l} \frac {1}{\sqrt {2 \pi}} \int_ {x} ^ {\infty} e ^ {- \frac {1}{2} \xi^ {2}} d \xi & = & \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {- x} e ^ {- \frac {1}{2} u ^ {2}} d u \\ & = & N (- x), \end{array}\tag{16.12}
$$

where we made the substitution $u = - \xi$ in the first line and $N ( x )$ is the standard normal cumulative probability density function, previously defined in equation (11.4). Using this result, we see that 

$$
\begin{array}{r c l} {I _ {2}} & = & {- K \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {- \xi^ {*}} e ^ {- \frac {1}{2} \xi^ {2}} d \xi} \\ & = & {- K e ^ {- r T} N (- \xi^ {*}).} \end{array}\tag{16.13}
$$

However, the standard way of writing the Black-Scholes formula is not in terms of $\xi ^ { * }$ , but rather in terms of two new constants $h ^ { + }$ and $h ^ { - }$ , defined to be 

$$
h ^ {\pm} = \frac {\log (\tilde {S} / K) \pm \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}},\tag{16.14}
$$

where $\tilde { S }$ is the forward price $S _ { 0 } e ^ { r T }$ . If we then rewrite $- \xi ^ { * }$ as 

$$
\begin{array}{r c l} - \xi^ {*} & = & - \frac {\log (K / S _ {0}) - (r T - \frac {1}{2} \sigma^ {2} T)}{\sigma \sqrt {T}} \\ & = & \frac {\log (S _ {0} / K) + r T - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}} \\ & = & \frac {\log (S _ {0} e ^ {r T} / K) - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}, \end{array}\tag{16.15}
$$

we see that 

$$
- \xi^ {*} = h ^ {-} \quad \text { and } \quad - \xi^ {*} + \sqrt {\sigma} T = h ^ {+}.\tag{16.16}
$$

Hence we can write the integral $I _ { 2 }$ as 

$$
I _ {2} = - e ^ {- r T} K N (h ^ {-}).\tag{16.17}
$$

We now want to calculate the slightly more complicated integral $I _ { 1 }$ . We begin by ‘completing the square’ in the exponential, 

$$
\begin{array}{r c l} {I _ {1}} & = & {\frac {1}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} S _ {0} \exp \left[ - \frac {1}{2} \xi^ {2} + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] d \xi} \\ & = & {\frac {S _ {0}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} \exp \left[ - \frac {1}{2} (\xi - \sigma \sqrt {T}) ^ {2} \right] d \xi .} \end{array}\tag{16.18}
$$

We then want to make a change of integration variable to $\eta = \xi - \sigma \sqrt { T }$ . In this case $d \xi = d \eta$ , and the lower limit of integration $\xi = \xi ^ { * }$ , becomes the new lower limit $\eta = \xi ^ { * } - \sigma \sqrt { T } = - h ^ { + }$ . Hence the integral becomes 

$$
I _ {1} = \frac {S _ {0}}{\sqrt {2 \pi}} \int_ {\eta = - h ^ {+}} ^ {\eta = \infty} e ^ {- \frac {1}{2} \eta^ {2}} d \eta .\tag{16.19}
$$

We can then use the result (C.237) to write the integral in terms of $N ( x )$ 

$$
I _ {1} = S _ {0} N (h ^ {+}).\tag{16.20}
$$

If we then sum the values of the integrals $I _ { 1 }$ and $I _ { 2 }$ we obtain 

$$
C _ {0} = e ^ {- r T} [ S _ {0} e ^ {r T} N (h ^ {+}) - K N (h ^ {-}) ],\tag{16.21}
$$

which is the famous Black-Scholes formula for the initial value of a call option. The price and payout function for a call option are plotted in figure 16.1. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/e3339f3382f747e475f775ab5de7464a1763fe21d149a1d8bbe66a3f018adf95.jpg)



Figure 16.1: This figure shows the price for a European call option as a function of the initial asset price $S _ { 0 } ,$ , for a maturity of $T = 1$ , an interest rate of $r = 0 . 0 5 .$ , a volatility of $\sigma = 0 . 2$ and a strike of $K = 1 0 0$ . The dashed line is the payof function for the option.


Exercise 16.1 Calculate and plot the following derivatives of the option price at time 0 

$$
\begin{array}{r l} & {(a) \Delta = \frac {\partial C _ {0}}{\partial S _ {0}}} \\ & {(b) \Gamma = \frac {\partial^ {2} C _ {0}}{\partial S _ {0} ^ {2}}} \\ & {(c) \mathcal {V} = \frac {\partial C _ {0}}{\partial \sigma}} \\ & {(d) \theta = - \frac {\partial C _ {0}}{\partial T}} \\ & {(e) \rho = \frac {\partial C _ {0}}{\partial r}} \end{array}
$$

## 16.2 Put Option

We recall that a European put option is a derivative that allows the holder to sell an asset at some time T in the future for a fixed strike price K. Hence the put option has a payof function 

$$
F (S _ {T}) = \max [ K - S _ {T}, 0 ].\tag{16.22}
$$

In other words, this is the net profit that would result if at maturity time $T$ the holder of the option buys a unit of stock for $S _ { T }$ dollars and then sells it for K dollars, according to the terms of the contract. Clearly the holder would only do this if $K > S _ { T }$ . If $K < S _ { T }$ then the option expires worthless. 

We can value the put option in an identical manner to how we dealt with the call option—by using the general formula (15.38). The initial price of the put option is therefore 

$$
\begin{array}{r c l} P _ {0} & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F \left(S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right]\right) \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \max \left(K - S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right], 0\right) \\ & & \times \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi . \end{array} \tag {16}\tag{16.23}
$$

As in the call option calculation, we first need to calculate the integration region on which the integrand is non-zero. This requires 

$$
K - S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] > 0,\tag{16.24}
$$

which implies that 

$$
K / S _ {0} > \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right].\tag{16.25}
$$

Taking logarithms we see that 

$$
\frac {\log (K / S _ {0}) - (r T - \frac {1}{2} \sigma^ {2} T)}{\sigma \sqrt {T}} > \xi .\tag{16.26}
$$

However, the left hand side of the inequality is simply the critical value $\xi ^ { * }$ defined in equation (C.232). Since the max function is only non-zero when the integration variable is less than the critical value $\xi ^ { * }$ , we can restrict the range of integration in equation (16.23) t $_ { 0 } \mathrm { ~ - \infty ~ } < \xi < \xi ^ { * }$ . Thus we can eliminate the max function from our expression for the price of the put option, 

$$
\begin{array}{r c l} {P _ {0}} & = & {\frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\xi^ {*}} \bigg (K - S _ {0} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] \bigg)} \\ & & {\times \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi .} \end{array}\tag{16.27}
$$

As before, we have two integrals to calculate, 

$$
I _ {1} = K \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\xi^ {*}} \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi ,\tag{16.28}
$$

and 

$$
\begin{array}{r c l} I _ {2} & = & - S _ {0} \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {\xi = - \infty} ^ {\xi = \xi^ {*}} \exp \left[ r T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi , \\ & = & - S _ {0} \frac {1}{\sqrt {2 \pi}} \int_ {\xi = - \infty} ^ {\xi = \xi^ {*}} \exp \left[ - \frac {1}{2} \xi^ {2} + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] d \xi , \end{array}\tag{16.29}
$$

where the put option price is the sum of the two, $P _ { 0 } = I _ { 1 } + I _ { 2 }$ . The integral $I _ { 1 }$ is trivial to evaluate, 

$$
I _ {1} = e ^ {- r T} K N (\xi^ {*}),\tag{16.30}
$$

or in terms of the constants $h ^ { \pm }$ defined in equation (C.239), 

$$
I _ {1} = e ^ {- r T} K N (- h ^ {-}).\tag{16.31}
$$

We can now evaluate the second integral by completing the square in the exponential, 

$$
\begin{array}{r c l} {I _ {2}} & = & {- S _ {0} \frac {1}{\sqrt {2 \pi}} \int_ {\xi = - \infty} ^ {\xi = \xi^ {*}} \exp \left[ - \frac {1}{2} \xi^ {2} + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] d \xi ,} \\ & = & {- \frac {S _ {0}}{\sqrt {2 \pi}} \int_ {\xi = - \infty} ^ {\xi = \xi^ {*}} \exp \left[ - \frac {1}{2} (\xi - \sigma \sqrt {T}) ^ {2} \right] d \xi .} \end{array}\tag{16.32}
$$

If we then change the integration variable to $\eta = \xi - \sigma \sqrt { T }$ , then the upper limit of integration $\xi = \xi ^ { * }$ , corresponds to $\eta = \xi ^ { * } - \sigma \sqrt { T } = - h ^ { + }$ , and we have 

$$
I _ {2} = - \frac {S _ {0}}{\sqrt {2 \pi}} \int_ {\eta = - \infty} ^ {\eta = - h ^ {+}} e ^ {- \frac {1}{2} \eta^ {2}} d \eta .\tag{16.33}
$$

This is may readily be expressed in terms of $N ( x )$ 2 

$$
I _ {2} = - S _ {0} N (- h ^ {+}).\tag{16.34}
$$

Summing the values of $I _ { 1 }$ and $I _ { 2 }$ yields 

$$
P _ {0} = e ^ {- r T} [ K N (- h ^ {-}) - S _ {0} e ^ {r T} N (- h ^ {+}) ],\tag{16.35}
$$

which is the Black-Scholes formula for the initial value of a put option. This is plotted in figure (16.2). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/af17031ed2e9666fcd23970c51acbe16dc3832a17e7bd9462859119d49e11e24.jpg)



Figure 16.2: This figure shows the price for a European put option as a function of the initial asset price $S _ { 0 }$ , for a maturity of $T = 1$ , an interest rate of $r = 0 . 0 5$ , a volatility of $\sigma = 0 . 2$ and a strike of $K = 1 0 0$ . The dashed line is the payof function for the option.


## 17 More Topics in Option Pricing

In this chapter we want to look at a few applications of the derivative pricing formula that we derived. We begin by considering European binary options, which are derivatives that pay of a constant amount only when the final asset price is above a fixed strike price—otherwise they pay nothing. We then discuss the partial derivatives of a portfolio, known as the Greeks, and see how they are used in hedging. Finally we look at put-call parity which relates the put and call option prices to the forward price of the asset. 

## 17.1 Binary Options

A derivative which pays of one dollar if the share price is above the strike price at maturity, and pays nothing otherwise is called a binary call option. If it pays of one dollar when the share price is below the strike and zero if it is above then this is called a binary put option. We can define the payof function in terms of the Heaviside function 

$$
H (x) = \left\{ \begin{array}{l l} 1 & x > 0 \\ 0 & x <   0 \end{array} \right..\tag{17.1}
$$

Hence the payof function for a binary call with strike K is $B C _ { T } ( S _ { T } ) ~ =$ $H ( S _ { T } - K )$ , while for a binary put with strike K it is $B P _ { T } ( S _ { T } ) = H ( K - S _ { T } )$ 

Suppose that we want to calculate the price for a binary call option. Using equation (15.38), we see that 

$$
\begin{array}{r c l} {B C _ {0}} & = & {e ^ {- r T} E ^ {*} [ B C _ {T} (S _ {T}) ]} \\ & = & {\frac {e ^ {- r T}}{\sqrt {2 \pi T}} \int_ {- \infty} ^ {\infty} H (S _ {T} - K) e ^ {- \xi^ {2} / 2 T} d \xi} \\ & = & {\frac {e ^ {- r T}}{\sqrt {2 \pi T}} \int_ {- \infty} ^ {\infty} H \left(S _ {0} \exp [ (r - \frac {1}{2} \sigma^ {2}) T + \sigma \xi ] - K\right) e ^ {- \xi^ {2} / 2 T} d \xi} \\ & = & {\frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} H \left(S _ {0} \exp [ (r - \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta ] - K\right) e ^ {- \eta^ {2} / 2} d \eta (1 7. 2)} \end{array}
$$

where we made the substitution $\eta = \xi / \sqrt { T }$ in the final integral. The Heaviside function is non-zero only when 

$$
S _ {0} \exp \left[ (r - \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta \right] > K.\tag{17.3}
$$

Taking logarithms and isolating η yields 

$$
\begin{array}{r c l} (r - \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta & > & - \log (S / K) \\ \eta & > & - \log (S / K) + (r - \frac {1}{2} \sigma^ {2}) T \sigma \sqrt {T} \\ \eta & > & - h ^ {-}. \end{array}\tag{17.4}
$$

Thus the integral simplifies to 

$$
\begin{array}{r c l} {B C _ {0}} & = & {\frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- h ^ {-}} ^ {\infty} e ^ {- \eta^ {2} / 2} d \eta} \\ & = & {e ^ {- r T} N (h ^ {-}) .} \end{array}\tag{17.5}
$$

Exercise 17.1 Calculate the value of the binary put option with payoffunction $H ( K - S _ { T } )$ 

## 17.2 ‘Greeks’ and Hedging

In chapter 15 we constructed a no arbitrage argument using a portfolio $V _ { t } ( S _ { t } )$ consisting of a long position in a derivative $C _ { t } ( S _ { t } )$ and a short position in $\phi _ { t }$ units of the asset $S _ { t }$ . Suppose that we consider the portfolio as a stochastic process. Then by Ito’s lemma the change in the value of the portfolio between times t and $t + d t$ is 

$$
d V _ {t} = \frac {\partial V _ {t}}{\partial t} d t + \frac {\partial V _ {t}}{\partial S _ {t}} d S _ {t} + \frac {1}{2} \frac {\partial^ {2} V _ {t}}{\partial S _ {t} ^ {2}} d S _ {t} ^ {2}.\tag{17.6}
$$

We were able to eliminate uncertainty in this value by setting 

$$
\frac {\partial V _ {t}}{\partial S _ {t}} = 0.\tag{17.7}
$$

A portfolio that satisfies this is known as Delta neutral or Delta hedged because $\frac { \partial V _ { t } } { \partial S _ { t } }$ is called the Delta of the portfolio. 

The Gamma of a portfolio is the second derivative of its value with respect to the asset price 

$$
\Gamma = \frac {\partial^ {2} V _ {t}}{\partial S _ {t} ^ {2}}.\tag{17.8}
$$

In order to construct the no arbitrage argument we do not need $\Gamma$ to vanish because it only contributes to the deterministic part of the portfolio return. 

However, the no arbitrage argument assumes that we are continuously able to rehedge our position such that $\Delta$ is always zero. In the context of our no arbitrage construction, this means that the share holding $\phi _ { t }$ must be continuously adjusted such that it is always equal to $- \partial C _ { t } / \partial S _ { t }$ . In order to do this we have to be continually buying or selling small amounts of the underlying asset. However, this is not realistic because there are transaction costs associated with each trade which make constant rehedging prohibitively expensive. So what really happens is that we start with a Delta neutral position which quickly becomes no longer Delta hedged as the share price moves around. We then rehedge our position, that is, make it Delta neutral again, from time to time to reduce the possibility of losing substantial sums of money. 

Is there any way that we can reduce the frequency with which we need to rehedge our position? Well, we have to adjust our holdings when the value of Delta becomes too large and sizeable losses can result from small movements in the underlying asset. If we set Gamma equal to zero, then Delta should remain small for asset prices near its current value, and hence we will need to rehedge less often. This is the rationale behind Gamma hedging. 

In order to Gamma hedge, assuming that we are also Delta hedging, our portfolio must consist of at least three instruments that depend on the same underlying asset. Suppose that we are short a derivative with price process $F _ { t } ( S _ { t } )$ . We can hedge this by taking a position in both the underlying $S _ { t }$ and a call option $C _ { t } ( S _ { t } )$ . The value of the portfolio is 

$$
V _ {t} = - F _ {t} + \phi_ {t} S _ {t} + \kappa_ {t} C _ {t}\tag{17.9}
$$

The Delta and Gamma of the portfolio are 

$$
\Delta = - \frac {\partial F _ {t}}{\partial S _ {t}} + \phi_ {t} + \kappa_ {t} \frac {\partial C _ {t}}{\partial S _ {t}} \quad \mathrm{and} \quad \Gamma = - \frac {\partial^ {2} F _ {t}}{\partial S _ {t} ^ {2}} + \kappa_ {t} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}}.\tag{17.10}
$$

We can set Γ to zero by choosing 

$$
\kappa_ {t} = \frac {\frac {\partial^ {2} F _ {t}}{\partial S _ {t} ^ {2}}}{\frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}}},\tag{17.11}
$$

which allows us to set $\Delta$ equal to zero if we take 

$$
\phi_ {t} = \frac {\partial F _ {t}}{\partial S _ {t}} - \frac {\frac {\partial^ {2} F _ {t}}{\partial S _ {t} ^ {2}}}{\frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}}} \frac {\partial C _ {t}}{\partial S _ {t}}.\tag{17.12}
$$

For example, we could Gamma hedge a short position in a binary call option by holding both the underlying asset and a call option on it. 

Exercise 17.2 Construct a Gamma hedged position for a portfolio which is short a binary call option with a strike price of $110 using the underlying asset which has a price of $100 and a call option with a strike price of $120. Assume that $r = 0 . 0 5 , \sigma = 0 . 2 0$ and that both options have a maturity of $T = 1 . 0$ 

Exercise 17.3 Can you Gamma hedge a short position in a call option with strike K by using the underlying and a call option of a diferent strike? Give a specific example. 

## 17.3 Put-Call Parity

There is an interesting and useful relationship between the value of a call option and the value of the corresponding put option, that is, the put option with the same maturity and strike price on the same underlying. Consider a position which is long the call and short the put. The payof function is 

$$
\begin{array}{r c l} {F (S _ {T})} & = & {C (S _ {T}) - P (S _ {T})} \\ & = & {\max [ S _ {T} - K, 0 ] - \max [ K - S _ {T}, 0 ]} \\ & = & {\max [ S _ {T} - K, 0 ] + \min [ S _ {T} - K, 0 ]} \\ & = & {S _ {T} - K.} \end{array}\tag{17.13}
$$

But this is simply the payof function for a forward contract with strike K. We have previously shown that the value of the forward contract is $S _ { 0 } \mathrm { ~ - ~ } K e ^ { - r T }$ . Hence the initial prices of the call and put portfolio must simply equal this value 

$$
C _ {0} - P _ {0} = S _ {0} - K e ^ {- r T}.\tag{17.14}
$$

This is the put-call parity relation. 

Exercise 17.4 Derive the put-call relation when $S _ { t }$ is the price of sterling in dollars and the interest rates are r and ρ for dollars and pounds respectively. 

We can also derive a put-call relation for the binary options. Consider a portfolio which is long both a put and call option with the same strike K and maturity T. The payof function is 

$$
\begin{array}{r c l} {F (S _ {T})} & = & {B C _ {T} (S _ {T}) + B P _ {T} (S _ {T})} \\ & = & {H (S _ {T} - K) + H (K - S _ {T})} \\ & = & 1. \end{array}\tag{17.15}
$$

Hence the payof is always one dollar. The initial price of a dollar is simply $e ^ { - r T }$ , and hence 

$$
B C _ {0} + B P _ {0} = e ^ {- r T}.\tag{17.16}
$$

Exercise 17.5 Using the Black-Scholes formulae for the put and call option prices verify the put-call relation. 

## 18 Continuous Dividend Model

There is a relatively simple but important adjustment that must be made to the Black-Scholes formula in order to take into account the fact that stocks pay dividends. These are typically relatively small payments made from time to time to the shareholders. The fact that dividends are paid to the owner of a stock means that the no arbitrage argument for pricing a derivative on the stock has to be modified. For simplicity, we shall assume that dividends are paid continuously over time at a rate $\delta _ { t } S _ { t }$ . In other words, the holder of the share at time t receives a dividend $\delta _ { t } S _ { t } d t$ in the time interval from t to $t + d t$ 

The situation is similar with a foreign currency. If $S _ { t }$ denotes the value of a foreign currency at time t, say, the price of one pound sterling in dollars, then the holder of that currency, assuming it is kept in a money market account, is paid interest on it. The amount of interest paid in the interval t to $t + d t$ is $\delta _ { t } S _ { t } d t$ , where $\delta _ { t }$ is the foreign interest rate. Note that in many circumstances interest really is paid on a continuous basis, whereas dividends are certainly not. If the underlying is taken to be a stock index, then the approximation of continuous dividends is more valid. 

We begin our work on the dividend model by calculating the cost of a forward contract to buy one share for K dollars at time $T$ , assuming that the dividend yield δ is constant. The initial cost of the contract is $F _ { 0 }$ dollars and the final payof is $F _ { T } ( S _ { T } ) = S _ { T } - K$ . We can replicate this payof by buying a portfolio which is long $e ^ { - \delta T }$ shares and short $K e ^ { - r T }$ bonds. The initial value of this position is 

$$
V _ {0} = S _ {0} e ^ {- \delta T} - K e ^ {- r T}\tag{18.1}
$$

We want to continuously reinvest the dividends back into shares. Thus the share holding $\psi _ { t }$ satisfies the diferential equation 

$$
d \psi_ {t} = \delta d t\tag{18.2}
$$

since we receive $\delta S _ { t } d t$ dollars in each small time interval and this can be used to buy δdt more shares, which each cost $S _ { t }$ . Hence the share holding is $\psi _ { t } = \psi _ { 0 } e ^ { \delta t }$ . Thus the final value of the portfolio is 

$$
V _ {T} = S _ {T} - K,\tag{18.3}
$$

which is the payof from the forward contract. Since the final payofs are the same, the initial values of the two positions must also be the same, and so 

$$
F _ {0} = S _ {0} e ^ {- \delta T} - K e ^ {- r T}.\tag{18.4}
$$

The forward price $\tilde { S }$ is the value of the strike price for which the initial cost of the forward contract is zero. It is easy to see that 

$$
\tilde {S} = S _ {0} e ^ {(r - \delta) T}.\tag{18.5}
$$

Exercise 18.1 What is the put-call relation for the constant dividend yield model? 

Now let us consider a local arbitrage argument that will eventually lead us to a generalisation of the Black-Scholes equation. Assume that the underlying asset price process is given by the usual stochastic diferential equation 

$$
\frac {d S _ {t}}{S _ {t}} = \mu_ {t} d t + \sigma_ {t} d W _ {t},\tag{18.6}
$$

where the drift $\mu _ { t }$ , the volatility $\sigma _ { t } ,$ the dividend rate (or foreign interest rate) $\delta _ { t }$ and the ‘domestic’ interest rate $r _ { t }$ are all ‘adapted’ to the Brownian motion $W _ { t }$ 

Suppose that we also have a derivative with price $C _ { t }$ at time t, with drift $\mu _ { t } ^ { C }$ , volatility $\sigma _ { t } ^ { C }$ and that it satisfies the dynamics 

$$
\frac {d C _ {t}}{C _ {t}} = \mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t}.\tag{18.7}
$$

Our goal is to discover the no-arbitrage relation between $S _ { t }$ and $C _ { t } .$ , which will take the form of a relation between $\mu _ { t } , \ \sigma _ { t } , \ \delta _ { t } , \ r _ { t } , \ \mu _ { t } ^ { C }$ and $\sigma _ { t } ^ { C }$ . Note that as in the previous case, $C _ { t }$ does not actually have to be a derivative of $S _ { t }$ , but merely must be driven by the same Brownian motion $W _ { t }$ . For the sake of symmetry, let us also suppose that the derivative pays a continuous dividend, at the rate $\delta _ { t } ^ { C }$ , which we also assume to be adapted to $W _ { t }$ . It might be thought that too many processes are being adapted to the same source Brownian motion. This defect will be cured later when we consider multiple assets and multiple sources of randomness. 

This time we shall present the arbitrage argument from the point of view of a ‘dealer’, who ‘sells’ the derivative to a client for the price $C _ { t } .$ , and wants to hedge his risk by buying $\phi _ { t }$ units of stock at price $S _ { t }$ . Thus, the dealer proceeds as follows: 

First, he borrows $\phi _ { t } S _ { t } - C _ { t }$ dollars from a bank, at the continuously compounded interest rate $r _ { t }$ 

Next, the derivative is sold to the client for $C _ { t }$ 

Finally, $\phi _ { t }$ units of stock are bought, for $\phi _ { t } S _ { t }$ dollars. 

The value of the dealer’s position (long the stock and short the derivative) is thus 

$$
V _ {t} = \phi_ {t} S _ {t} - C _ {t}.\tag{18.8}
$$

In other words, to ‘close down’ the position the dealer would have to sell $\phi _ { t }$ units of stock, and buy back the derivative, giving a total value $V _ { t } .$ , which might be negative. The change in the value of the position over the small time interval from t to $t + d t$ is given by 

$$
d V _ {t} = \phi_ {t} d S _ {t} - d C _ {t} + \delta \phi_ {t} S _ {t} d t - \delta^ {C} C _ {t} d t.\tag{18.9}
$$

The last two terms appear because the dealer has had to pay a small dividend $\delta _ { t } ^ { C } C _ { t } d t$ to the holder of the derivative, but at the same time gets a dividend $\delta _ { t } \phi _ { t } S _ { t } d t$ on the shares. Substituting in for $d S _ { t }$ and $d C _ { t }$ from the price processes for the stock and the derivative, we obtain 

$$
d V _ {t} = \phi_ {t} (\mu_ {t} S _ {t} d t + \sigma_ {t} S _ {t} d W _ {t}) + \phi_ {t} S _ {t} \delta d t - (\mu_ {t} ^ {C} C _ {t} d t + \sigma_ {t} ^ {C} C _ {t} d W _ {t}) - C _ {t} \delta_ {t} ^ {C} d t.\tag{18.10}
$$

More explicitly, gathering terms together we have 

$$
d V _ {t} = (\phi_ {t} \mu_ {t} S _ {t} + \phi_ {t} \delta_ {t} S _ {t} - \mu_ {t} ^ {C} C _ {t} - \delta_ {t} ^ {C} C _ {t}) d t + (\phi_ {t} \sigma_ {t} S _ {t} - \sigma_ {t} ^ {C} C _ {t}) d W _ {t}.\tag{18.11}
$$

To ensure a definite rate of return on the hedged position, the dealer must ensure that the coeficient of $d W _ { t }$ is made to vanish in this expression, so that the hedge ratio $\phi _ { t }$ is given by 

$$
\phi_ {t} = \frac {\sigma_ {t} ^ {C} C _ {t}}{\sigma_ {t} S _ {t}}.\tag{18.12}
$$

Note that the inclusion of dividends does not afect the formula for the hedge ratio, which agrees with the result calculated previously in equation (14.1). 

Thus the change in the hedged position $d V _ { t }$ , obtained by substituting the hedge ratio (18.12) into (18.11), is given by 

$$
d V _ {t} = [ (\mu_ {t} + \delta_ {t}) \frac {\sigma_ {t} ^ {C}}{\sigma_ {t}} - (\mu_ {t} ^ {C} + \delta_ {t} ^ {C}) ] C _ {t} d t,\tag{18.13}
$$

whereas the value $V _ { t } = \phi _ { t } S _ { t } - C _ { t }$ of the dealer’s position is 

$$
V _ {t} = \left(\frac {\sigma^ {C}}{\sigma} - 1\right) C _ {t}.\tag{18.14}
$$

For no arbitrage, the gains on the dealer’s risk-free position must be equal to the corresponding gains one would earn from a bank account with interest rate $r _ { t } .$ , so 

$$
d V _ {t} = r V _ {t} d t.\tag{18.15}
$$

It follows by substitution that 

$$
(\mu_ {t} + \delta_ {t}) \frac {\sigma_ {t} ^ {C}}{\sigma_ {t}} + (\mu_ {t} ^ {C} + \delta_ {t} ^ {C}) = r _ {t} \left(\frac {\sigma_ {t} ^ {C}}{\sigma_ {t}} - 1\right),\tag{18.16}
$$

which therefore implies 

$$
\frac {\mu_ {t} + \delta_ {t} - r _ {t}}{\sigma_ {t}} = \frac {\mu_ {t} ^ {C} + \delta_ {t} ^ {C} - r _ {t}}{\sigma_ {t} ^ {C}}.\tag{18.17}
$$

This is the no arbitrage relation in the presence of dividends. Or equivalently, if we interpret $S _ { t }$ as the price of a foreign currency (in units of domestic currency) then $\delta _ { t }$ has the interpretation of a foreign interest rate, and (18.17) is the no arbitrage condition for derivatives based on that currency. The financial interpretation of this relation is that the total excess return (‘capital’ gains plus dividends) above the risk-free interest rate, per unit of risk (volatility), is the same for both the underlying asset and the derivative, or more generally, for any two instruments driven by the same Brownian motion. 

## 18.1 Modified Black-Scholes Equation

Let us see what implications the inclusions of dividends has for the Black-Scholes equation. As in the previous derivation we assume that $C _ { t } = C ( S _ { t } , t )$ Ito’s lemma then implies that 

$$
\mu^ {C} = \frac {1}{C _ {t}} \left[ \frac {\partial C}{\partial t} + \mu S \frac {\partial C}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} C}{\partial S ^ {2}} \right],\tag{18.18}
$$

and 

$$
\sigma^ {C} = \frac {1}{C _ {t}} \left[ \sigma S \frac {\partial C}{\partial S} \right].\tag{18.19}
$$

Here, to simplify the notation slightly, we temporarily drop the time subscripts on the processes $\mu _ { t } , \sigma _ { t } , \delta _ { t } , r _ { t } , \mu _ { t } ^ { C } , \sigma _ { t } ^ { C }$ and $\delta _ { t } ^ { C }$ . As a consequence of the no-arbitrage relation (18.17) we have 

$$
(\mu + \delta - r) \frac {\sigma^ {C}}{\sigma} C _ {t} = (\mu^ {C} + \delta^ {C} - r) C _ {t},\tag{18.20}
$$

which follows by multiplying equation (18.17) by $\sigma ^ { C } C _ { t }$ . Substituting in the expressions for $\mu ^ { C }$ and $\sigma ^ { C }$ obtained above, we see therefore that 

$$
(\mu + \delta - r) S _ {t} \frac {\partial C}{\partial S} = \frac {\partial C}{\partial t} + \mu S \frac {\partial C}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} C}{\partial S ^ {2}} + (\delta^ {C} - r) C _ {t}.\tag{18.21}
$$

Note that once again the terms involving µ cancel, and we are left with 

$$
\frac {\partial C _ {t}}{\partial t} + \frac {1}{2} \sigma^ {2} S _ {t} ^ {2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} = (r - \delta^ {C}) C _ {t} - (r - \delta) S _ {t} \frac {\partial C _ {t}}{\partial S _ {t}}.\tag{18.22}
$$

This is the Black-Scholes equation as modified for the inclusion of dividends. 

Exercise 18.2 Using an argument similar to that in exercise 13.1 derive the modified Black-Scholes equation. 

## 18.2 Call and Put Option Prices

Now suppose that we specialize to the case when $\mu , ~ \sigma , ~ \delta , ~ r$ and $\delta ^ { C }$ are constant. Then by careful comparison with the transformations used earlier to convert the Black-Scholes equation to the heat equation, we find that the solutions are essentially the same as before, except that we use $F _ { t } = S _ { 0 } e ^ { ( r }$ −<sup>δ)t</sup> for the forward price, while the overall discount factor is $e ^ { - ( r - \delta ^ { C } ) t }$ . Thus the solution is 

$$
C _ {0} = \frac {e ^ {- (r - \delta^ {C}) T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F (S _ {0} e ^ {(r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T}) e ^ {- \frac {1}{2} \xi^ {2}} d \xi\tag{18.23}
$$

for a general European-style derivative with payof $F ( S _ { T } )$ at time $T .$ . Note that the presence of the continuous dividend $\delta ^ { \bar { C } }$ paid out on the derivative holding itself makes the value of $C _ { 0 }$ at time 0 greater than it would be otherwise, since, in addition to the final payof, the investor also gets all the dividends. 

Exercise 18.3 Show that (18.23) solves (18.22) with the required boundary conditions. 

For the Black-Scholes formula based on a dividend paying stock in the case of a basic call option, with no dividends paid on the option itself, we obtain 

$$
C _ {0} = e ^ {- r T} [ S _ {0} e ^ {(r - \delta) T} N (h ^ {+}) - K N (h ^ {-}) ],\tag{18.24}
$$

where 

$$
h ^ {\pm} = \frac {\ln (\tilde {S} _ {T} / K) \pm \frac {1}{2} \sigma^ {2} T)}{\sigma \sqrt {T}}.\tag{18.25}
$$

Here $\tilde { S } _ { T } = S _ { 0 } e ^ { ( r - \delta ) T }$ is the no arbitrage forward price for the dividend paying stock or interest paying foreign currency at time T. 

Exercise 18.4 Derive (18.24) from (18.23) in the case of a call option. 

Exercise 18.5 Calculate the initial cost of a binary call option. 

## 19 Risk Neutral Valuation

So far we have considered the situation where there are just two assets— the basic asset with price $S _ { t }$ , and the money market account with price $B _ { t }$ The ‘economy’ is driven by a single Brownian motion $W _ { t }$ . In this formalism a derivative is viewed as an additional ‘special’ asset with price $C _ { t }$ that is inserted into the economy, subject to a no arbitrage condition that relates its dynamics to those of the basic asset and the money market account. 

A more flexible approach is to introduce at the outset an economy based on a number of assets with prices $S _ { t } ^ { i } ( i = 1 , \dots , n )$ . These assets can include derivatives, but now the derivatives are not treated any diferently from the underlying assets on which they are based. Since there must be additional sources of randomness in the market, we want the entire system to be driven by a multi-dimensional Brownian motion $W _ { t } ^ { \alpha } ( \alpha = 1 , \ldots , N )$ . Typically, we want $n \geq N$ . This is a complicated area of research that we shall only touch only briefly in the final two chapters of the book. In order to prepare for this and develop the necessary mathematics, we shall first re-examine the single asset model using the ‘martingale’ method. 

## 19.1 Single Asset Case

Recall that the stochastic diferential equation for the share price in the single asset model is 

$$
\frac {d S _ {t}}{S _ {t}} = \mu_ {t} d t + \sigma_ {t} d W _ {t},\tag{19.1}
$$

where $\mu _ { t }$ and $\sigma _ { t }$ are adapted processes, that is, they depend only on the ‘history’ of the Brownian motion from time 0 to time t, and no other ‘source of randomness’. In the case where $\mu , \sigma$ are constant, the solution of (19.1) is given by 

$$
S _ {t} = S _ {0} \exp \left(\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t\right).\tag{19.2}
$$

How do we solve this equation? Perhaps the easiest way is to make the variable substitution $X _ { t } = \log S _ { t }$ . The stochastic diferential equation for $X _ { t }$ can then be calculated using Ito’s lemma, 

$$
\begin{array}{r c l} {d X _ {t}} & = & {\frac {\partial X _ {t}}{\partial S _ {t}} d S _ {t} + \frac {1}{2} \frac {\partial^ {2} X _ {t}}{\partial S _ {t} ^ {2}} d S _ {t} ^ {2}} \\ & = & {\frac {d S _ {t}}{S _ {t}} - \frac {1}{2} \frac {d S _ {t} ^ {2}}{S _ {t} ^ {2}}} \end{array}
$$

$$
{ = } { \mu _ { t } d t + \sigma _ { t } d W _ { t } - \frac { 1 } { 2 } \sigma _ { t } ^ { 2 } d t }\tag{19.3}
$$

In the case of constant coeficients $\mu$ and $\sigma$ we can integrate the equation to obtain 1 

$$
X _ {t} = X _ {0} + \mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t.\tag{19.4}
$$

But since $S _ { t } = e ^ { X _ { t } }$ , we see that 

$$
S _ {t} = S _ {0} \exp \left(\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t\right).\tag{19.5}
$$

We shall call this the Black-Scholes model for a single asset. 

However, suppose that we do not want to restrict ourselves to the constant coeficient case. We could still integrate equation (19.3) to obtain 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} \mu_ {s} d s + \int_ {0} ^ {t} \sigma_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \sigma_ {s} ^ {2} d s,\tag{19.6}
$$

which then yields the more general solution 

$$
S _ {t} = S _ {0} \exp \left[ \int_ {0} ^ {t} \mu_ {s} d s + \int_ {0} ^ {t} \sigma_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \sigma_ {s} ^ {2} d s \right].\tag{19.7}
$$

If $\mu$ and $\sigma$ are constant, then formula (19.7) reduces to (19.2). We shall call (19.7) the basic model for a single asset. 

Now that we have defined and solved for the asset price, we want to consider the money market account $B _ { t }$ . Its stochastic diferential equation is 

$$
\frac {d B _ {t}}{B _ {t}} = r _ {t} d t,\tag{19.8}
$$

where $r _ { t }$ is the short term interest rate. In the Black-Scholes model, where all the coeficients are constant, this has the solution 

$$
B _ {t} = B _ {0} e ^ {r t}.\tag{19.9}
$$

In the basic model we place no constraints on the interest rate, and hence have the more general solution 

$$
B _ {t} = B _ {0} \exp \left[ \int_ {0} ^ {t} r _ {s} d s \right].\tag{19.10}
$$

From now on we shall assume that $B _ { 0 } = 1$ 

We now want to introduce a new stochastic process that we shall call the risk premium or market price of risk process $\lambda _ { t } .$ and defined by the equation 

$$
\mu_ {t} = r _ {t} + \lambda_ {t} \sigma_ {t}.\tag{19.11}
$$

The risk premium is the ‘extra’ rate of return, above the short term rate, per unit of risk, as measured by the volatility. Then equation (19.1) can be written in the form 

$$
\frac {d S _ {t}}{S _ {t}} = (r _ {t} + \lambda_ {t} \sigma_ {t}) d t + \sigma_ {t} d W _ {t},\tag{19.12}
$$

or equivalently, 

$$
\frac {d S _ {t}}{S _ {t}} = r _ {t} d t + \sigma_ {t} (\lambda_ {t} d t + d W _ {t}).\tag{19.13}
$$

More specifically the asset price process (19.7) can be written as 

$$
\begin{array}{r c l} {S _ {t}} & = & {S _ {0} \exp \left[ \int_ {0} ^ {t} r _ {s} d s + \int_ {0} ^ {t} \sigma_ {s} (d W _ {s} + \lambda_ {s} d s) - \frac {1}{2} \int_ {0} ^ {t} \sigma_ {s} ^ {2} d s \right]} \\ {S _ {t}} & = & {S _ {0} B _ {t} \exp \left[ \int_ {0} ^ {t} \sigma_ {s} (d W _ {s} + \lambda_ {s} d s) - \frac {1}{2} \int_ {0} ^ {t} \sigma_ {s} ^ {2} d s \right],} \end{array}\tag{19.14}
$$

where we have substituted in the value of $B _ { t }$ from equation (19.10). Thus for the ratio $S _ { t } / B _ { t }$ we have 

$$
\frac {S _ {t}}{B _ {t}} = S _ {0} \exp \left[ \int_ {0} ^ {t} \sigma_ {s} (d W _ {s} + \lambda_ {s} d s) - \frac {1}{2} \int_ {0} ^ {t} \sigma_ {s} ^ {2} d s \right].\tag{19.15}
$$

Now suppose that we define the process $\rho _ { t }$ by 

$$
\rho_ {t} = \exp \left[ - \int_ {0} ^ {t} \lambda_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \lambda_ {s} ^ {2} d s \right].\tag{19.16}
$$

By use of Ito’s Lemma, is is straightforward to verify that the stochastic diferential of $\rho _ { t }$ is given by 

$$
d \rho_ {t} = - \rho_ {t} \lambda_ {t} d W _ {t},\tag{19.17}
$$

and hence is driftless, and thus $\rho _ { t }$ is a martingale. Now let us consider the product 

$$
\Pi_ {t} = \frac {\rho_ {t} S _ {t}}{B _ {t}}.\tag{19.18}
$$

This is given, in more explicit terms, by 

$$
\begin{array}{r c l} \Pi_ {t} & = & S _ {0} \exp \left[ - \int_ {0} ^ {t} \lambda_ {s} d W _ {s} - - \int_ {0} ^ {t} \lambda_ {s} ^ {2} d s \right] \\ & & \exp \left[ \int_ {0} ^ {t} \sigma_ {s} (d W _ {s} + \lambda_ {s} d s) - \frac {1}{2} \int_ {0} ^ {t} \sigma_ {s} ^ {2} d s \right] \\ & = & S _ {0} \exp \left[ \int_ {0} ^ {t} (\sigma_ {s} - \lambda_ {s}) d W _ {s} + \int_ {0} ^ {t} (- \frac {1}{2} \lambda_ {s} ^ {2} + \sigma_ {s} \lambda_ {s} - \frac {1}{2} \sigma_ {s} ^ {2}) d s \right] \\ & = & S _ {0} \exp \left[ \int_ {0} ^ {t} (\sigma_ {s} - \lambda_ {s}) d W _ {s} \right] \exp \left[ - \frac {1}{2} \int_ {0} ^ {t} (\lambda_ {s} - \sigma_ {s}) ^ {2} d s \right]. \end{array}\tag{19.19}
$$

The stochastic diferential of $\Pi _ { t }$ is thus given by 

$$
d \Pi_ {t} = (\sigma_ {t} - \lambda_ {t}) \Pi_ {t} d W _ {t},\tag{19.20}
$$

and since it is driftless, it follows that $\Pi _ { t }$ is also a martingale. 

Exercise 19.1 Show that if $X _ { t }$ is a stochastic process such that 

$$
d X _ {t} = f (X _ {t}, t) d W _ {t}\tag{19.21}
$$

then $X _ { t }$ is a martingale. 

The martingale property for $\Pi _ { t }$ can be written 

$$
E _ {s} \left[ \rho_ {t} \frac {S _ {t}}{B _ {t}} \right] = \rho_ {s} \frac {S _ {s}}{B _ {s}}\tag{19.22}
$$

Now for any random variable $Z _ { t } .$ , adapted to the history of $W _ { t }$ from $0$ to $t ,$ we can define a new probability measure $P ^ { * }$ with expectation 

$$
E _ {s} ^ {*} [ Z _ {t} ] \equiv \frac {E _ {s} [ \rho_ {t} Z _ {t} ]}{\rho_ {s}}.\tag{19.23}
$$

This is called a ‘change of measure’ and the idea is basic to finance. The positive martingale $\rho _ { t }$ defining the change of measure is called the density martingale. 

In the present situation the new measure is called the risk-neutral measure. The significance of $E _ { s } ^ { * }$ is that from (19.22) we have 

$$
E _ {s} ^ {*} \left[ \frac {S _ {t}}{B _ {t}} \right] = \frac {S _ {s}}{B _ {s}},\tag{19.24}
$$

which shows that the ratio $S _ { t } / B _ { t }$ is a martingale in this measure. 

This is completely analogous to the discrete time situation, in which the risk-neutral probabilities are those for which the ratio of the asset price to the money market account is a martingale. 

Now suppose that $C _ { t }$ is the price of a derivative based on $S _ { t } .$ , with payof $C _ { T }$ at time $T .$ where $C _ { T }$ is a random variable adapted to the history of the Brownian motion up to time $T .$ . Then for the process $C _ { t }$ we have the stochastic equation 

$$
\frac {d C _ {t}}{C _ {t}} = \mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t}.\tag{19.25}
$$

We have shown already that the no arbitrage condition is given by 

$$
\frac {\mu_ {t} ^ {C} - r _ {t}}{\sigma_ {t} ^ {C}} = \frac {\mu_ {t} - r _ {t}}{\sigma_ {t}},\tag{19.26}
$$

which, since $\lambda _ { t } = ( \mu _ { t } - r _ { t } ) / \sigma _ { t }$ , implies that 

$$
\mu_ {t} ^ {C} = r _ {t} + \lambda_ {t} \sigma_ {t} ^ {C},\tag{19.27}
$$

and thus 

$$
\frac {d C _ {t}}{C _ {t}} = r _ {t} d t + \sigma_ {t} ^ {C} (d W _ {t} + \lambda_ {t} d t).\tag{19.28}
$$

This is formally identical in structure to (19.13) so we can conclude that $\rho _ { t } C _ { t } / B _ { t }$ is a martingale, and hence 

$$
E _ {s} ^ {*} \left[ \frac {C _ {t}}{B _ {t}} \right] = \frac {C _ {s}}{B _ {s}}.\tag{19.29}
$$

That is to say, the process $C _ { t } / B _ { t }$ is a martingale in the risk-neutral measure. Thus, the initial value of the derivative is simply 

$$
E _ {0} ^ {*} \left[ \frac {C _ {T}}{B _ {T}} \right] = C _ {0}.\tag{19.30}
$$

Note that nothing in this derivation used the fact that $C _ { t }$ is a derivative based on the asset $S _ { t }$ . Hence it will hold for any financial instrument that is subject to the same Brownian motion as $S _ { t }$ . Thus, in the risk-neutral measure, the ratio of the price of any tradable asset to the price of the money market account is always a martingale. 

Exercise 19.2 What are the stochastic equations satisfied by 

$$
\frac {S _ {t}}{B _ {t}} \quad \mathrm{and} \quad \frac {\rho_ {t} S _ {t}}{B _ {t}}?\tag{19.31}
$$

Exercise 19.3 Show that 

$$
\rho_ {t} = 1 - \int_ {0} ^ {t} \lambda_ {s} \rho_ {s} d W _ {s}.\tag{19.32}
$$

Exercise 19.4 Suppose $\lambda$ is constant and $X _ { t } ~ = ~ W _ { t }$ . Find $E _ { s } ^ { * } [ W _ { t } ]$ and $E _ { s } ^ { * } [ W _ { t } ^ { 2 } ]$ 

Exercise 19.5 Show that $\Pi _ { t } ^ { C }$ is indeed a martingale under the measure $E _ { s } ^ { * }$ 

## 20 Girsanov Transformation

Now we shall attempt to interpret more clearly the meaning of the riskneutral measure. We have shown that if the asset $S _ { t }$ satisfies 

$$
\frac {d S _ {t}}{S _ {t}} = r _ {t} d t + \sigma_ {t} (d W _ {t} + \lambda_ {t} d t),\tag{20.1}
$$

where $r _ { t }$ is the short-term interest rate, $\sigma _ { t }$ is the volatility, and $\lambda _ { t }$ is the risk premium, all adapted, then 

$$
\Pi_ {t} = \rho_ {t} \frac {S _ {t}}{B _ {t}}\tag{20.2}
$$

is a martingale. Here 

$$
B _ {t} = \exp \left[ \int_ {0} ^ {t} r _ {s} d s \right]\tag{20.3}
$$

is the unit-initialised money market account and 

$$
\rho_ {t} = \exp \left[ - \int_ {0} ^ {t} \lambda_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \lambda_ {s} ^ {2} d s \right]\tag{20.4}
$$

is the change of measure density martingale. Thus, $E _ { s } [ \Pi _ { t } ] = \Pi _ { s }$ , and hence 

$$
E _ {s} ^ {*} \left[ \frac {S _ {t}}{B _ {t}} \right] = \frac {S _ {s}}{B _ {s}}\tag{20.5}
$$

Here $E _ { s } ^ { * }$ is the (conditional) risk-neutral expectation operator, defined by 

$$
E _ {s} ^ {*} [ X _ {t} ] = \frac {E _ {s} [ \rho_ {t} X _ {t} ]}{\rho_ {s}}\tag{20.6}
$$

for any random variable $X _ { t }$ adapted to the filtration of information available up to time t. 

If $C _ { t }$ is the value of a derivative based on the same information set, e.g. with a payof $C _ { T }$ that depends on $S _ { T }$ , then the process for $C _ { t }$ is, necessarily of the form 

$$
\frac {d C _ {t}}{C _ {t}} = r _ {t} d t + \sigma_ {t} ^ {C} (d W _ {t} + \lambda_ {t} d t),\tag{20.7}
$$

from which it follows that 

$$
\Pi_ {t} ^ {C} = \rho_ {t} \frac {C _ {t}}{B _ {t}}\tag{20.8}
$$

is also a martingale with repect to $E _ { s }$ , and hence $C _ { t } / B _ { t }$ is a martingale with respect to the risk-neutral expectation $E _ { s } ^ { * }$ 2 

$$
E _ {s} ^ {*} \left[ \frac {C _ {t}}{B _ {t}} \right] = \frac {C _ {s}}{B _ {s}}.\tag{20.9}
$$

Thus, for derivatives valuation we can write 

$$
C _ {0} = E _ {0} ^ {*} \left[ \frac {C _ {T}}{B _ {T}} \right].\tag{20.10}
$$

In particular, if $C _ { T } = F ( S _ { T } )$ , as in the case of a call option, then we have 

$$
C _ {0} = E _ {0} ^ {*} [ F (S _ {T}) / B _ {T} ]\tag{20.11}
$$

where the terminal value of the asset $S _ { T }$ is given by the random variable 

$$
S _ {T} = S _ {0} B _ {T} \exp \left[ \int_ {0} ^ {T} \sigma_ {s} (d W _ {S} + \lambda_ {s} d s) - \frac {1}{2} \int_ {0} ^ {T} \sigma_ {s} ^ {2} d s \right].\tag{20.12}
$$

## 20.1 Change of Drift

These formulae can all be simplified in an illuminating way by defining a new random process $W _ { t } ^ { * }$ 2 

$$
W _ {t} ^ {*} = W _ {t} + \int_ {0} ^ {t} \lambda_ {s} d s,\tag{20.13}
$$

which will turn out to be a Brownian motion with respect to the risk-neutral measure. The stochastic diferential of $W _ { t } ^ { * }$ is given by 

$$
d W _ {t} ^ {*} = d W _ {t} + \lambda_ {t} d t,\tag{20.14}
$$

and thus for the asset process (19.1) we can write 

$$
\frac {d S _ {t}}{S _ {t}} = r _ {t} d t + \sigma_ {t} d W _ {t} ^ {*},\tag{20.15}
$$

while for $C _ { t }$ we have 

$$
\frac {d C _ {t}}{C _ {t}} = r _ {t} d t + \sigma_ {t} ^ {C} d W _ {t} ^ {*}.\tag{20.16}
$$

Hence the final asset price (20.12) is given by 

$$
S _ {T} = S _ {0} B _ {T} \exp \left[ \int_ {0} ^ {T} \sigma_ {s} d W _ {S} ^ {*} - \frac {1}{2} \int_ {0} ^ {T} \sigma_ {s} ^ {2} \right] d s.\tag{20.17}
$$

Now we shall outline an important result, known as Girsanov’s theorem, which plays an important role in finance. We start with the process $W _ { t } ^ { * } =$ $\begin{array} { r } { W _ { t } + \int _ { 0 } ^ { t } \lambda _ { s } d s } \end{array}$ , which can be interpreted as a general Brownian motion with drift. We shall show that with respect to the new system of probabilities governed by the measure $E ^ { * }$ , the process $W _ { t } ^ { * }$ satsfies the axioms of standard Brownian motion. In other words, with respect to $E ^ { * }$ , the process $W _ { t } ^ { * }$ is normally distributed, has independent increments, and the variance of $W _ { t } ^ { * }$ is t. To derive this result we need the following useful lemmas. 

Lemma 20.1 A random variable X is normally distributed, with mean m and variance V , if and only if its characteristic function $\phi ( z ) ~ = ~ E [ e ^ { i z X } ]$ satisfies 

$$
E [ e ^ {i z X} ] = e ^ {i z m - \frac {1}{2} z ^ {2} V}.\tag{20.18}
$$

## Lemma 20.2

Two random variables X, Y are independent with respect to $E [ - ]$ if and only if their joint characteristic function factorises: 

$$
E [ e ^ {i z _ {1} X + i z _ {2} Y} ] = E [ e ^ {i z _ {1} X} ] E [ e ^ {i z _ {2} Y} ]\tag{20.19}
$$

We shall show first that with respect to $E ^ { * } [ - ]$ , the process $W _ { t } ^ { * }$ , as given by (20.13) is normally distributed, with mean zero and variance t. Consider first the density martingale $\rho _ { t }$ . Since $\rho _ { t }$ is a martingale with initial value unity, we have 

$$
E [ \rho_ {t} ] = E \left[ \exp \left(- \int_ {0} ^ {t} \lambda_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \lambda_ {s} ^ {2} d s\right) \right] = \rho_ {0} = 1.\tag{20.20}
$$

Now suppose that we replace $\lambda _ { s }$ with $\lambda _ { s } - i z$ , where z is a (real) parameter, and $i = \sqrt { - 1 }$ . Then one can use Ito’s lemma to verify that $d \rho _ { t }$ is still driftless, hence we still have a martingale, and thus 

$$
E \left[ \exp \left\{- \int_ {0} ^ {t} (\lambda_ {s} - i z) d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} (\lambda_ {s} - i z) ^ {2} d s \right\} \right] = 1.\tag{20.21}
$$

Expanding this expression we get 

$$
\begin{array}{l} E \left[ \exp \left\{- \int_ {0} ^ {t} \lambda_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \lambda_ {s} ^ {2} d s \right\} \right. \\ \times \left. \exp \left\{i z (\int_ {0} ^ {t} d W _ {s} + \int_ {0} ^ {t} \lambda_ {s} d s) \right\} \exp \left\{\frac {1}{2} \int_ {0} ^ {t} z ^ {2} d s \right\} \right] = 1, \end{array}\tag{20.22}
$$

which simplifies to the equation 

$$
E \left[ \rho_ {t} \exp \left\{i z (\int_ {0} ^ {t} d W _ {s} + \int_ {0} ^ {t} \lambda_ {s} d s) \right\} \right] = \exp \left\{- \frac {1}{2} \int_ {0} ^ {t} z ^ {2} d s \right\}\tag{20.23}
$$

or, equivalently, 

$$
E ^ {*} [ e ^ {i z W _ {t} ^ {*}} ] = e ^ {- \frac {1}{2} z ^ {2} t}.\tag{20.24}
$$

Hence by lemma 20.1, we see that $W _ { t } ^ { * }$ is indeed normally distributed with respect to the measure $E ^ { * }$ , with mean zero and variance t. 

In order to show that the process $W _ { t } ^ { * }$ has independent increments, we need the idea of the indicator function, $I _ { s } ( a , b )$ for an interval $[ a , b ]$ . We define 

$$
I _ {s} (a, b) = \left\{ \begin{array}{l l} 1 & \text { for } \quad a \leq s \leq b \\ 0 & \text { otherwise } \end{array} \right.\tag{20.25}
$$

Thus if $0 \leq a \leq b \leq t$ , then 

$$
\int_ {0} ^ {t} I _ {s} (a, b) d s = b - a.\tag{20.26}
$$

Now let us look at (20.20) again, this time making the substitution 

$$
\lambda_ {s} \rightarrow \lambda_ {s} - i z _ {1} I _ {s} (a, b) - i z _ {2} I _ {s} (c, d)\tag{20.27}
$$

where $z _ { 1 }$ and $z _ { 2 }$ are real parameters. Here we assume that $0 \leq a \leq b \leq c \leq$ $d \leq t .$ . Then we know that 

$$
E [ e ^ {X _ {t}} ] = 1,\tag{20.28}
$$

where 

$$
\begin{array}{r c l} X _ {t} & = & - \int_ {0} ^ {t} [ \lambda_ {s} - i z _ {1} I _ {s} (a, b) - i z _ {2} I _ {s} (c, d) ] d W _ {s} \\ & & - \frac {1}{2} \int_ {0} ^ {t} [ \lambda_ {s} - i z _ {1} I _ {s} (a, b) - i z _ {2} I _ {s} (c, d) ] ^ {2} d s. \end{array}\tag{20.29}
$$

after some simplification this expression reduces to 

$$
\begin{array}{r c l} X _ {t} & = & - \int_ {0} ^ {t} \lambda_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \lambda_ {s} ^ {2} d s + i z _ {1} \int_ {0} ^ {t} I _ {s} (a, b) [ d W _ {s} + \lambda_ {s} d s ] + \\ & & i z _ {2} \int_ {0} ^ {t} I _ {s} (c, d) [ d W _ {s} + \lambda_ {s} d s ] + \frac {1}{2} z _ {1} ^ {2} \int_ {0} ^ {t} I _ {s} (a, b) d s \\ & & + \frac {1}{2} z _ {1} ^ {2} \int_ {0} ^ {t} I _ {s} (a, b) d s. \end{array}\tag{20.30}
$$

Then we can evaluate the integrals involving the indicator functions to obtain 

$$
\begin{array}{r c l} X _ {t} & = & - \int_ {0} ^ {t} \lambda_ {s} d W _ {s} - \frac {1}{2} \int_ {0} ^ {t} \lambda_ {s} ^ {2} d s + i z _ {1} (\tilde {W} _ {b} - \tilde {W} _ {b}) + i z _ {2} (\tilde {W} _ {d} - \tilde {W} _ {c}) \\ & & + \frac {1}{2} z _ {1} ^ {2} (b - a) + \frac {1}{2} z _ {1} ^ {2} (b - a). \end{array} \tag {2}\tag{20.31}
$$

Substituting this back into (20.28), we get 

$$
\begin{array}{r c l} E \left[ \rho_ {t} \exp \left\{i z _ {1} (\tilde {W} _ {b} - \tilde {W} _ {a}) \right. \right. & \\ \left. + i z _ {2} (\tilde {W} _ {d} - \tilde {W} _ {c}) \right\} \biggr ] & = & \exp \left\{- \frac {1}{2} z _ {1} ^ {2} (b - a) \right\} \\ & & \times \exp \left\{- \frac {1}{2} z _ {1} ^ {2} (b - a) \right\}. \end{array}\tag{20.32}
$$

By lemma 20.2, this shows that with respect to the expectation $E ^ { * } [ - ] =$ $E [ \rho _ { t } - ]$ , the increments $W _ { b } ^ { * } - W _ { a } ^ { * }$ and $W _ { d } ^ { * } - W _ { c } ^ { * }$ are independent random variables, and each is normally distributed. 

Thus, we have shown that $W _ { s } ^ { * }$ is a Brownian motion with respect to the expectation $E ^ { * } [ - ]$ . That explains why the process (20.15) is called ‘risk neutral’ with respect to $E ^ { * } [ - ]$ 

Now suppose that we let r and $\sigma$ be constant. Then 

$$
S _ {T} = S _ {0} e ^ {r T + \sigma W _ {T} ^ {*} - \frac {1}{2} \sigma^ {2} T}\tag{20.33}
$$

and 

$$
\begin{array}{r c l} {C _ {0}} & = & {E ^ {*} [ \frac {C _ {T}}{B _ {T}} ]} \\ & = & {e ^ {- r T} E ^ {*} [ F (S _ {0} e ^ {r T + \sigma W _ {T} ^ {*} - \frac {1}{2} \sigma^ {2} T}) ],} \end{array}\tag{20.34}
$$

which is the formula we derived previously, by solving the Black-Scholes equation, for valuing general European derivatives. Note that $W _ { T } ^ { * }$ is normally distributed with respect to $E ^ { * }$ 

## 21 Multiple Asset Models

Until now we have considered a financial market that consists of a single basic asset together with a money market account and derivatives based on these two assets. This market is driven by a single source of randomness. Needless to say, for a more realistic financial market we have to consider a larger number of assets and more sources of randomness. So in this chapter, we analyse markets with both multiple assets and sources of uncertainty. For simplicity, we shall begin by assuming that these are non-dividend paying assets, but later we will extend our results to the case when continuous dividends are paid on shares, or equivalently, interest is paid on foreign currencies. 

## 21.1 The Basic Model

We want a market that has more than a single basic asset. Consider a situation where there are n assets, with prices $S _ { t } ^ { i } \ ( i = 1 , \ldots , n )$ . We also want a market where there is more than one source of uncertainty. So assume that the assets are driven by an N-dimensional Brownian motion $W _ { t } ^ { \alpha }$ $( \alpha = 1 , \ldots , N )$ . In order for everything to run smoothly we require $n \geq N$ Otherwise we are led to a so-called incomplete market situation. 

How are the movements of the n asset prices related? This can be formalised by introducing the idea of an instantaneous covariance matrix for the asset price dynamics. Let us proceed as follows. We assume the Brownian motions are independent, in the sense that the Ito rule is given by 

$$
d W _ {t} ^ {\alpha} d W _ {t} ^ {\beta} = \delta^ {\alpha \beta} d t,\tag{21.1}
$$

where $\delta ^ { \alpha \beta }$ is the identity matrix. Thus $d W ^ { 1 } d W ^ { 1 } = d t , d W ^ { 2 } d W ^ { 2 } = d t$ $d W ^ { 1 } d W ^ { 2 } = 0$ , and so on. As before, we also have $d W ^ { \alpha } d t = 0$ for all $\alpha$ Thus the multi-dimensional Ito rule is a straight-forward generalization of the one-dimensional case. 

Now that we have clarified the nature of the multi-dimensional Brownian motions, we can return to the asset price changes. The basic model for n asset prices is given by the following dynamics: 

$$
\frac {d S _ {t} ^ {i}}{S _ {t} ^ {i}} = \mu_ {t} ^ {i} d t + \sum_ {\alpha} \sigma_ {t} ^ {i \alpha} d W _ {t} ^ {\alpha}.\tag{21.2}
$$

Here $\mu _ { t } ^ { i }$ and $\sigma _ { t } ^ { i \alpha }$ are adapted processes, in the sense that they depend, in a general way, only on the history of the multi-dimensional Brownian motion 

$W _ { t } ^ { \alpha }$ from time 0 to time t. The $n \times N$ matrix $\sigma ^ { i \alpha }$ , for $i = 1 , \ldots , n$ and $\alpha = 1 , \ldots , N$ , is called the volatility matrix. It measures the sensitivity of asset number i to Brownian motion number $\alpha .$ . The processes $W _ { t } ^ { \alpha }$ can be thought of intuitively as representing ‘independent’ sources of randomness, or uncertainty, in the markets. 

Exercise 21.1 Consider a simple 2-dimensional Black-Scholes world, with asset price processes, 

$$
\begin{array}{r c l} {d S _ {t} ^ {1} / S _ {t} ^ {1}} & = & {\mu^ {1} d t + \sigma^ {1 1} d W _ {t} ^ {1} + \sigma^ {1 2} d W _ {t} ^ {2}} \\ {d S _ {t} ^ {2} / S _ {t} ^ {2}} & = & {\mu^ {2} d t + \sigma^ {2 1} d W _ {t} ^ {1} + \sigma^ {2 2} d W _ {t} ^ {2}} \end{array}\tag{21.3}
$$

where the vector $\mu ^ { i }$ and the matrix $\sigma ^ { i j }$ are both constant. Solve these equations for $S _ { t } ^ { 1 }$ and $S _ { t } ^ { 2 }$ . 

Now let us investigate the volatility matrix more closely. To this end, we consider the following product: 

$$
\begin{array}{r c l} \frac {d S ^ {i}}{S ^ {i}} \frac {d S ^ {j}}{S ^ {j}} & = & (\mu_ {t} ^ {i} d t + \sum_ {\alpha} \sigma_ {t} ^ {i \alpha} d W _ {t} ^ {\alpha}) (\mu_ {t} ^ {j} d t + \sum_ {\beta} \sigma_ {t} ^ {j \beta} d W _ {t} ^ {\beta}) \\ & = & \sum_ {\alpha} \sigma_ {t} ^ {i \alpha} d W _ {t} ^ {\alpha} \sum_ {\beta} \sigma_ {t} ^ {j \beta} d W _ {t} ^ {\beta} \\ & = & \sum_ {\alpha} \sum_ {\beta} \sigma_ {t} ^ {i \alpha} \sigma_ {t} ^ {j \beta} d W _ {t} ^ {\alpha} d W _ {t} ^ {\beta} \\ & = & \sum_ {\alpha} \sum_ {\beta} \sigma_ {t} ^ {i \alpha} \sigma_ {t} ^ {j \beta} \delta^ {\alpha \beta} d t \\ & = & \sum_ {\alpha} \sigma_ {t} ^ {i \alpha} \sigma_ {t} ^ {j \alpha} d t. \end{array}\tag{21.4}
$$

The matrix 

$$
C _ {t} ^ {i j} = \sum_ {\alpha} \sigma_ {t} ^ {i \alpha} \sigma_ {t} ^ {j \alpha}\tag{21.5}
$$

that arises here is called the instantaneous covariance matrix of the set of assets under consideration. 

Exercise 21.2 Calculate the instantaneous covariance matrix for the 2-dimensional Black-Scholes market given in exercise (21.1). 

In the case $i = j$ , we have 

$$
\left(\frac {d S ^ {i}}{S ^ {i}}\right) ^ {2} = C _ {t} ^ {i i},\tag{21.6}
$$

where 

$$
C _ {t} ^ {i i} = \sum_ {\alpha} (\sigma_ {t} ^ {i \alpha}) ^ {2}\tag{21.7}
$$

is the instantaneous variance (squared volatility) for the asset i. Note that in the case when there is only a single asset with $d S ^ { 1 } / S ^ { 1 } = \mu ^ { i } + \sigma ^ { 1 } d W ^ { 1 }$ , then $C _ { t } ^ { 1 1 } = ( \sigma ^ { 1 } ) ^ { 2 }$ , as expected. If we write 

$$
\sigma^ {i} = \sqrt {\sum_ {\alpha} \sigma^ {i \alpha} \sigma^ {i \alpha}}\tag{21.8}
$$

for the volatility of asset $i ,$ , then the matrix 

$$
\rho^ {i j} = \frac {C ^ {i j}}{\sigma^ {i} \sigma^ {j}}\tag{21.9}
$$

is called the instananeous correlation in the motion of asset i and asset $j$ . 

Exercise 21.3 Calculate the correlation matrix for the 2-dimensional Black-Scholes market. What are the volatilities of the two assets? 

We note that the covariance matrix $C ^ { i j }$ is non-negative in the sense that for any ‘vector’ of numbers $\theta ^ { i } \ ( i = 1 , \ldots n )$ we have 

$$
\sum_ {i j} C ^ {i j} \theta^ {i} \theta^ {j} \geq 0.\tag{21.10}
$$

This result can be given a financial interpretation. Suppose that we form a portfolio of assets, holding asset $S ^ { i }$ in the quantity $\phi ^ { i }$ . Thus $\phi ^ { i }$ is the number of shares one holds of asset $i ,$ which has price $S ^ { i }$ . The the total value of the portfolio is clearly $\Sigma _ { i } \phi ^ { i } S ^ { i }$ . Note that some of the $\phi ^ { i } \mathrm { \mathrm { : } } \mathrm { \Delta } \phi$ can be negative, in P<sub>the case of short positions. Now suppose we define</sub> 

$$
\theta^ {i} = \frac {\phi^ {i} S ^ {i}}{\sum_ {j} \phi^ {j} S ^ {j}}.\tag{21.11}
$$

Then $\theta ^ { i }$ is the percentage of the total value of the portfolio that is held in asset i. With this in mind, we can look at the change in the value of the portfolio as the market moves. If 

$$
V _ {t} = \sum_ {i} \phi^ {i} S _ {t} ^ {i}\tag{21.12}
$$

is the value of the portfolio at time t, then 

$$
d V = \sum_ {i} \phi^ {i} d S ^ {i},\tag{21.13}
$$

is the instantaneous change in the value of the portfolio, for the given holding defined by $\phi ^ { i }$ , when the asset price changes are given by $d S ^ { i }$ . Therefore, by the Ito rules we have 

$$
\begin{array}{r c l} (d V) ^ {2} & = & \sum_ {i j} \phi^ {i} \phi^ {j} d S ^ {i} d S ^ {j} \\ & = & \sum_ {i j} \phi^ {i} \phi^ {j} S ^ {i} S ^ {j} C ^ {i j} d t. \end{array}\tag{21.14}
$$

So, for the percentage change in the value of the portfolio, we have 

$$
\begin{array}{r c l} \left(\frac {d V}{V}\right) ^ {2} & = & \sum_ {i j} \frac {\phi^ {i} S ^ {i}}{V} \frac {\phi^ {j} S ^ {j}}{V} C ^ {i j} d t \\ & = & \sum_ {i j} \theta^ {i} \theta^ {j} C ^ {i j} d t, \end{array}\tag{21.15}
$$

where we have used the fact that $\theta ^ { i } = \phi ^ { i } S ^ { i } / V$ . Thus, $\textstyle \sum _ { i j } \theta ^ { i } \theta ^ { j } C ^ { i j }$ represents the instantaneous variance in the portfolio value at time t. But clearly the variance of the portfolio must be non-negative. Thus equation (21.10) can be interpreted as saying that the variance of any portfolio has to be nonnegative. These ideas can be developed further, and lead to the concepts of portfolio theory, which is an important branch of finance theory. 

## 21.2 No Arbitrage and the Zero Volatility Portfolio

Here, we shall consider one particular aspect of portfolio analysis that is of great significance to derivatives pricing. Suppose we consider the problem of choosing a portfolio weighting such that the portfolio has instantaneously zero volatility. Then, over the next short period, this portfolio would ofer a definite rate of return. By the no arbitrage condition, this rate of return would have to be the money market interest rate $r _ { t }$ 

We have seen from (21.15) that with a holding weight of $\theta ^ { i }$ in asset $i ,$ the portfolio variance vanishes if and only if 

$$
\sum_ {i j} \theta^ {i} \theta^ {j} C ^ {i j} = 0.\tag{21.16}
$$

But, we can express this sum in the form 

$$
\begin{array}{r c l} \sum_ {i j} \theta^ {i} \theta^ {j} C ^ {i j} & = & \sum_ {\alpha} \sum_ {i} \sum_ {j} \theta^ {i} \theta^ {j} \sigma^ {i \alpha} \sigma^ {j \alpha} \\ & = & \sum_ {\alpha} \xi^ {\alpha} \xi^ {\alpha}, \end{array}\tag{21.17}
$$

where $\begin{array} { r } { \xi ^ { \alpha } = \sum _ { i } \theta ^ { i } \sigma ^ { i \alpha } } \end{array}$ . Now, since (21.17) is given by a sum of squares, clearly P<sub>(21.16) holds if and only if</sub> $\xi ^ { \alpha } = 0$ for each value of α. In other words, the portfolio variance (risk) vanishes at time t if and only if $\theta ^ { i }$ is chosen so that 

$$
\sum_ {i} \theta^ {i} \sigma^ {i \alpha} = 0.\tag{21.18}
$$

Now let us return to the expression for the change in the portfolio value, (21.13), and note that 

$$
\begin{array}{r c l} \frac {d V}{V} & = & \frac {\sum_ {i} \phi^ {i} d S ^ {i}}{V} \\ & = & \frac {\sum_ {i} \phi^ {i} S ^ {i} (\mu^ {i} d t + \sum_ {\alpha} \sigma^ {i \alpha} d W ^ {\alpha})}{\sum_ {i} \phi^ {i} S ^ {i}} \\ & = & \sum_ {i} \theta^ {i} \mu^ {i} d t + \sum_ {\alpha} \left(\sum_ {i} \theta^ {i} \sigma^ {i \alpha}\right) d W ^ {\alpha}. \end{array}\tag{21.19}
$$

Clearly the volatility of the portfolio value V vanishes at time t if and only if the condition (21.18) holds at that time. 

We require that $\textstyle \sum _ { i } \theta ^ { i } \mu ^ { i } = r _ { t }$ if and only if $\theta ^ { i } \sigma ^ { i \alpha } = 0$ . In other words, we want the rate of return on the portfolio to be the short rate (i.e. the money market interest rate) if and only if the portfolio volatility vanishes. This implies that there must exist a set of numbers $\lambda ^ { \alpha } \left( \alpha = 1 , \ldots , N \right)$ such that 

$$
\sum_ {i} \theta^ {i} \mu^ {i} = r _ {t} + \sum_ {\alpha} \lambda^ {\alpha} \left(\sum_ {i} \theta^ {i} \sigma^ {i \alpha}\right).\tag{21.20}
$$

However, since $\textstyle \sum _ { i } \theta ^ { i } = 1$ , this relation can be written in the form 

$$
\sum_ {i} \theta^ {i} \mu^ {i} = \sum_ {i} \theta^ {i} r + \sum_ {i} \theta^ {i} (\sum_ {\alpha} \lambda^ {\alpha} \sigma^ {i \alpha}),\tag{21.21}
$$

which has to hold for any choice of $\theta ^ { i }$ . Hence it follows that 

$$
\mu^ {i} = r _ {t} + \sum_ {\alpha} \lambda^ {\alpha} \sigma^ {i \alpha}.\tag{21.22}
$$

This is the no arbitrage condition for n assets driven by N Brownian motions, when there are no dividends. 

Note that the ‘vector’ $\lambda ^ { \alpha }$ can be interpreted as the market risk premium for factor $\alpha .$ . In other words, $\lambda ^ { \alpha }$ is the excess rate $o f$ return, attributable to factor $\alpha ,$ per unit of volatility in that factor. 

For example, suppose that we have two assets, but just a single random factor $( i = 1 , 2 \alpha = 1 )$ Then, suppressing $\alpha _ { \mathrm { { ; } } }$ , we have 

$$
\mu^ {1} = r + \lambda \sigma^ {1} \quad \mathrm{and} \quad \mu^ {2} = r + \lambda \sigma^ {2}.\tag{21.23}
$$

Eliminating $\lambda ,$ we obtain 

$$
\frac {\mu^ {1} - r}{\sigma^ {1}} = \frac {\mu^ {2} - r}{\sigma^ {2}},\tag{21.24}
$$

which is equivalent to the no arbitrage condition that we derived earlier in connection with a share-price and an option. Thus we see that the two assets have a common risk premium, given by $\lambda .$ 

## 21.3 Market Completeness

Now let us consider the risk premium vector $\lambda ^ { \alpha }$ further. For no arbitrage, we know that (21.22) has to be satisfied. But if $\lambda ^ { \alpha }$ satisfies (21.22) is there any other vector, say $\bar { \lambda } ^ { \alpha }$ that also satisfies (21.22)? If so, then their diference, $\lambda ^ { \alpha } - \bar { \lambda } ^ { \alpha }$ would have to satisfy 

$$
\sum_ {\alpha} (\lambda^ {\alpha} - \bar {\lambda} ^ {\alpha}) \sigma^ {i \alpha} = 0.\tag{21.25}
$$

We say that a set of assets $S ^ { i } \ ( i = 1 , \ldots , n )$ , or market, is complete with respect to the Brownian motion $W _ { \alpha } ^ { t }$ if there exists no non-vanishing vector $\xi ^ { \alpha }$ such that $\begin{array} { r } { \sum _ { \alpha } \xi ^ { \alpha } \sigma ^ { i \alpha } = 0 } \end{array}$ . This market completeness condition is equivalent to a requirement that the matrix $\sigma ^ { i \alpha }$ should be of maximum rank (N). If the assets $S ^ { i }$ are complete, then any derivative adapted to $W _ { t } ^ { \alpha }$ , can be hedged with a portfolio of positions in these assets. 

## 22 Multiple Asset Models Continued

## 22.1 Dividends

Now let us consider the situation when dividends are paid in the multi-asset case. This leads to a simple modification of formula (21.22). In particular, suppose that there is a dividend (or interest) paid continuously at the rate $\delta _ { t } ^ { i }$ for asset i. This means that during the short interval dt, the holder of asset i receives a payment of $\delta ^ { i } S ^ { i } d t$ . Thus, if the portfolio has value $V = \textstyle \sum _ { i } \phi ^ { i } S ^ { i }$ 2 P<sub>then the total gain (or loss) to the holder over the interval dt is given by</sub> 

$$
R = d V + \sum_ {i} \phi^ {i} S ^ {i} \delta^ {i} d t,\tag{22.1}
$$

i.e., it is the change in value of the portfolio, plus all the dividends (or interest). In percentage terms, this is 

$$
\begin{array}{r c l} \frac {R}{V} & = & \frac {d V + \sum_ {i} \phi^ {i} S ^ {i} \delta^ {i} d t}{V} \\ & = & \frac {d V}{V} + \sum_ {i} \theta^ {i} \delta^ {i} d t, \end{array}\tag{22.2}
$$

since $\theta ^ { i } = \phi ^ { i } S ^ { i } / V$ . But, we calculated the percentage change in the portofolio value in (21.19), so 

$$
\frac {R}{V} = \sum_ {i} \theta^ {i} (\mu^ {i} + \delta^ {i}) d t + \sum_ {i \alpha} \theta^ {i} \sigma^ {i, \alpha} d W ^ {\alpha}.\tag{22.3}
$$

Thus, if we eliminate the randomness by applying condition (21.18), then the no arbitrage condition tells us that $\textstyle \sum _ { i } \theta ^ { i } ( \mu ^ { i } + \delta ^ { i } ) = r _ { t }$ when $\begin{array} { r } { \sum _ { i } \theta ^ { i } \sigma ^ { i \alpha } = 0 } \end{array}$ This implies that there must exist $\lambda ^ { \alpha }$ such that 

$$
\mu^ {i} + \delta^ {i} = r + \sum_ {\alpha} \lambda^ {\alpha} \sigma^ {i \alpha}.\tag{22.4}
$$

This is the general no arbitrage condition for n assets which pay continuous dividends (or interest). 

Now we can take formula (22.4) for the drift, and reinsert it into the asset dynamical equation to obtain 

$$
\frac {d S ^ {i}}{S ^ {i}} = (r - \delta^ {i}) d t + \sum_ {\alpha} \sigma^ {i \alpha} (d W ^ {\alpha} + \lambda^ {\alpha} d t).\tag{22.5}
$$

This is the general dynamical equation for n dividend paying assets under the condition of no arbitrage. We see that the only modification required is to subtract of the dividend rate (or foreign interest rate) from the ‘domestic interest rate r. 

## 22.2 Martingales and the Risk-Neutral Measure

We have seen, in the case of multiple assets with no dividends, that the noarbitrage requirement is equivalent to the condition (21.22) on the drift of the assets, 

$$
\mu^ {i} = r + \sum_ {\alpha} \lambda^ {\alpha} \sigma^ {i \alpha},\tag{22.6}
$$

where $r$ is the short rate of interest, $\lambda ^ { \alpha }$ is the market price of risk vector, and $\sigma ^ { i \alpha }$ is the volatility matrix. The no-arbitrage condition is both necessary and suficient for the existence of the market risk premium vector $\lambda ^ { \alpha }$ , which for each factor can be interpreted as the excess rate of return (above the short rate) per unit of volatility risk. If we substitute (21.22) into the asset price process (21.2), then we obtain 

$$
\frac {d S ^ {i}}{S ^ {i}} = r d t + \sum_ {\alpha} \sigma^ {i \alpha} (d W ^ {\alpha} + \lambda^ {\alpha} d t).\tag{22.7}
$$

Here, for convenience, we occasionally suppress the subscript t, writing $S ^ { i }$ for $S _ { t } ^ { i } \mathrm { \dag }$ ; but remember that all processes are adapted, i.e. they depend in a general way on the history of $W _ { s } ^ { \alpha }$ for $0 \leq s \leq t$ . In addition to the assets $S ^ { i }$ $( i = 1 , \ldots , n )$ we also have the money market account $B _ { t }$ . We want to assume market completeness, that is, that $\sigma ^ { i \alpha }$ has maximal rank $N ,$ the dimension of the Brownian motion). This ensures that the market-risk premium vector $\lambda ^ { \alpha }$ is unique. Also, it ensures that when $W _ { t } ^ { \alpha }$ moves at least one of the market prices $S ^ { i }$ moves. In that sense, market completeness implies that every move in $W _ { t } ^ { \alpha }$ implies some move in the prices $S ^ { i }$ , so that $W _ { t } ^ { \alpha }$ is ‘fully expressed’ in the given asset changes. Otherwise, the market is ‘incomplete’. 

Our next step is to form a multi-asset density martingale $\rho _ { t }$ , 

$$
\rho_ {t} = \exp \left[ - \int_ {0} ^ {t} \sum_ {\alpha} \lambda_ {s} ^ {\alpha} d W _ {s} ^ {\alpha} - \frac {1}{2} \int_ {0} ^ {t} \sum_ {\alpha} (\lambda_ {s} ^ {\alpha}) ^ {2} d s \right],\tag{22.8}
$$

where $\alpha = 1 , \ldots , N$ . This expression is, in fact, given by the product of the corresponding density martingales for the various components of $\lambda ^ { \alpha }$ . In 

other words, 

$$
\rho_ {t} = \prod_ {\alpha = 1} ^ {N} \rho_ {t} ^ {\alpha},\tag{22.9}
$$

where 

$$
\rho_ {t} ^ {\alpha} = \exp \left[ - \int_ {0} ^ {t} \lambda_ {s} ^ {\alpha} d W _ {s} ^ {\alpha} - \frac {1}{2} \int_ {0} ^ {t} (\lambda_ {s} ^ {\alpha}) ^ {2} d s \right].\tag{22.10}
$$

The following facts emerge: 

1. The process $\rho _ { t }$ is a martingale with respect to the measure defined by the expectation $E _ { s }$ 

2. For each value of $i ,$ , the ratio $\rho _ { t } S _ { t } ^ { i } / B _ { t }$ is a martingale with respect to the measure $E _ { s }$ 

3. If we define the risk-neutral measure $E _ { s } ^ { * }$ according to the scheme 

$$
E _ {s} ^ {*} [ X _ {t} ] = \frac {E _ {s} [ \rho_ {t} X _ {t} ]}{\rho_ {s}}\tag{22.11}
$$

for any adapted random variable $X _ { t }$ , then the process $W _ { t } ^ { * \alpha }$ defined by 

$$
W _ {t} ^ {* \alpha} = W _ {t} ^ {\alpha} + \int_ {0} ^ {t} \lambda_ {s} ^ {\alpha} d s\tag{22.12}
$$

is a standard N-dimensional Brownian motion with respect to $E _ { s } ^ { * }$ . That is, with respect to $E _ { s } ^ { * }$ , the process $W _ { t } ^ { * \alpha }$ is normally distributed for each value of $\alpha ,$ , with mean $0$ and variance $t ,$ has independent increments, and furthermore $W _ { t } ^ { * \alpha }$ and $W _ { t } ^ { * \beta }$ are independent for $\alpha \neq \beta$ 

These results can be established by analogy with the corresponding results in the single asset case. Thus, for the asset process we can write 

$$
\frac {d S ^ {i}}{S ^ {i}} = r _ {t} d t + \sum_ {\alpha} \sigma^ {i \alpha} d W _ {t} ^ {* \alpha},\tag{22.13}
$$

where $W _ { t } ^ { * \alpha }$ is a standard Brownian motion with respect to the risk-neutral measure. 

Moreover, since the ratio $\rho _ { t } S _ { t } ^ { i } / B _ { t }$ is a martingale, we have 

$$
\frac {\rho_ {s} S _ {s} ^ {i}}{B _ {s}} = E _ {s} \left[ \frac {\rho_ {t} S _ {t} ^ {i}}{B _ {t}} \right],\tag{22.14}
$$

and thus 

$$
\frac {S _ {s} ^ {i}}{B _ {s}} = \frac {E _ {s} \left[ \rho_ {t} (\frac {S _ {t} ^ {i}}{B _ {t}}) \right]}{\rho_ {s}},\tag{22.15}
$$

which by the definition of the risk-neutral measure gives 

$$
\frac {S _ {s} ^ {i}}{B _ {s}} = E _ {s} ^ {*} \left[ \frac {S _ {t} ^ {i}}{B _ {t}} \right].\tag{22.16}
$$

Thus, the absence of arbitrage ensures the existence of a unique risk-neutral measure such that the ratio of any asset price to the money market account is a martingale. This generalises the analogous result that we obtained in the single asset case. 

## 22.3 Derivatives

Now suppose that we have a derivative with payout $C _ { T }$ at time T. We assume that the payout is adapted to $W _ { s } ^ { \alpha }$ for $0 \leq s \leq T$ . For example, $C _ { T }$ can be a function of the values of the various assets $S _ { s } ^ { i }$ for various times between 0 and $T .$ . Let $C _ { t }$ denote the value of the derivative at time t. Then since the derivative is also an asset, we can use the martingale condition (22.16) to infer that C 

$$
\frac {C _ {t}}{B _ {t}} = E _ {t} ^ {*} \left[ \frac {C _ {T}}{B _ {T}} \right],\tag{22.17}
$$

or equivalently 

$$
C _ {t} = B _ {t} E _ {t} ^ {*} \left[ \frac {C _ {T}}{B _ {T}} \right].\tag{22.18}
$$

This gives us a formula for the price process of the derivative, and, in particular, allows us to compute its value today, $C _ { 0 }$ . Since the money market account $B _ { t }$ is given by 

$$
B _ {t} = \exp \{\int_ {0} ^ {t} r _ {s} d s \}\tag{22.19}
$$

it is worth noting that (22.18) can be written in the form 

$$
C _ {t} = E _ {t} ^ {*} \left[ \exp \{- \int_ {t} ^ {T} r _ {s} d s \} C _ {T} \right].\tag{22.20}
$$

Thus if $r _ { s }$ is non-random, or more generally if it is independent of the payof $C _ { T }$ , then (22.20) can be further simplified. 

Formula (22.20) is, of course, not the end of the story, but really is just the beginning. Given (22.20), we can compute the hedge ratios $\phi _ { t } ^ { i }$ needed in order to construct a portfolio in the $S _ { t } ^ { i } \mathrm { { ^ { s } } }$ and $B _ { t }$ to replicate the derivative. If $n > N$ , then the hedge portfolio can be constructed with some flexibility. 

In my end is my beginning. 

—T.S. Eliot, Four Quartets. 

## A Glossary

American option An option that can be exercised at any time up to the expiration date. 

arbitrage 

at the money A call or put option with a strike price equal to the current share price is said to be ‘at the money’. 

Call option A derivative that gives its owner the right to buy an asset at a fixed price, called the strike price. 

discount factor Something related to the time-value of money. 

European option An option that can only be exercised at a fixed expiration date. 

expectation The expectation of a discrete random variable X with probability distribution $p ( x _ { i } ) = \mathrm { P r o b } [ X = X _ { i } ]$ is 

$$
E [ X ] = \sum_ {i} x _ {i} p (x _ {i})
$$

It gives the ‘average’ value of X. The expectation of a continuous random variable X with probability density function $\rho ( x )$ is given by 

$$
E [ X ] = \int_ {- \infty} ^ {\infty} x p (x) d x
$$

in the money An option is said to be ‘in the money’ if it would have a positive payof if it were exercised immediately. 

interest rate The rate at which you pay interest. 

long position The position created by possession of an asset. 

## martingale

out of the money An option is said to be ‘out of the money’ if it would have have a negative payof if it were exercised immediately. 

probability density function Similarly, the probability density function $\rho ( x )$ of a continuous random variable X, if it exists, is a function $\rho ( x )$ such that 

$$
\mathrm{Prob} [ a \leq X \leq b ] = \int_ {a} ^ {b} \rho (x) d x
$$

put-call parity A relation holding between the values of call and put options with common strikes, in the absence of dividends. 

put option An option that gives the owner the right, but not the obligation, to sell an asset at a pre-specified price. 

random variable A random variable X is a function that maps each possible outcome from an experiment to a real number. 

risk-free Guaranteed, sure. 

sample space The sample space can be thought of as the set of all possible outcomes of an experiment or trial. The sample space is discrete if the elements of the sample space can be indexed by the integers (i.e., it is countable). 

short position A negative position in an asset; the position in an asset created when an asset is sold, but before the asset has been actually delivered; an American style derivative, whose payof is minus the value of the underlying asset at the time of exercise, and whose price today is equal to minus the value of the asset today. 

standard deviation The standard deviation $\sigma ( x )$ of a random variable X is defined by $\sigma ( X ) = [ V ( X ) ] ^ { 1 / 2 }$ , where $V ( x )$ is the variance. 

stock A part ownership of a company. 

strike price The amount of money needed to exercise an option, usually denoted K. 

time value of money The fact that money now is worth more than money in the future. 

underlying asset A stock or whatever on which a derivative is based. 

variance The variance of a random variable X, if it exists, is defined by 

$$
V [ X ] = E [ (X - E [ X ]) ^ {2} ] = E [ X ^ {2} ] - E [ X ] ^ {2}
$$

Wiener process Brownian motion with drift. 

## B Some useful formulae and definitions

## B.1 Definitions of a Normal Variable

The $\mathrm { N } ( m , V )$ probability density function is 

$$
\rho_ {m, V} (x) = \frac {1}{\sqrt {2 \pi V}} \exp \left[ - \frac {(x - m) ^ {2}}{2 V} \right].\tag{B.21}
$$

The cumulative normal function is defined to be 

$$
N (x) = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {x} \exp \left[ - \frac {\xi^ {2}}{2} \right] d x.\tag{B.22}
$$

## B.2 Moments of the Standard Normal Distribution For even moments,

$$
\frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} x ^ {2 n} \exp \left[ - \frac {x ^ {2}}{2} \right] d x = \frac {(2 n) !}{n ! 2 ^ {n}},\tag{B.23}
$$

while for odd moments, 

$$
{\frac {1}{\sqrt {2 \pi}}} \int_ {- \infty} ^ {\infty} x ^ {2 n + 1} \exp \left[ - \frac {x ^ {2}}{2} \right] d x = 0.\tag{B.24}
$$

The first few even moments are 

$$
{\frac {1}{\sqrt {2 \pi}}} \int_ {- \infty} ^ {\infty} \exp \left[ - \frac {x ^ {2}}{2} \right] d x = 1\tag{B.25}
$$

$$
{\frac {1}{\sqrt {2 \pi}}} \int_ {- \infty} ^ {\infty} x ^ {2} \exp \left[ - {\frac {x ^ {2}}{2}} \right] d x = 1\tag{B.26}
$$

$$
{\frac {1}{\sqrt {2 \pi}}} \int_ {- \infty} ^ {\infty} x ^ {4} \exp \left[ - \frac {x ^ {2}}{2} \right] d x = 3.\tag{B.27}
$$

## B.3 Moments of a Normal Distribution

$$
\frac {1}{\sqrt {2 \pi V}} \int_ {- \infty} ^ {\infty} x \exp \left[ - \frac {(x - m) ^ {2}}{2 V} \right] d x = m\tag{B.28}
$$

$$
{\frac {1}{\sqrt {2 \pi V}}} \int_ {- \infty} ^ {\infty} x ^ {2} \exp \left[ - \frac {(x - m) ^ {2}}{2 V} \right] d x = m ^ {2} + V\tag{B.29}
$$

$$
\frac {1}{\sqrt {2 \pi V}} \int_ {- \infty} ^ {\infty} x ^ {3} \exp \left[ - \frac {(x - m) ^ {2}}{2 V} \right] d x = m ^ {3} + 3 m V\tag{B.30}
$$

$$
\frac {1}{\sqrt {2 \pi V}} \int_ {- \infty} ^ {\infty} x ^ {4} \exp \left[ - \frac {(x - m) ^ {2}}{2 V} \right] d x = m ^ {4} + 6 V m ^ {2} + 3 V ^ {2}\tag{B.31}
$$

## B.4 Other Useful Integrals

For $a > 0$ 

$$
\frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \exp \left[ - \frac {a x ^ {2}}{2} + b x + c \right] = \frac {1}{\sqrt {a}} \exp \left[ \frac {b ^ {2}}{4 a} + c \right].\tag{B.32}
$$

$$
\int_ {0} ^ {\infty} e ^ {- \lambda x} d x = \lambda \quad \text { for } \quad \lambda > 0\tag{B.33}
$$

If X is an $N ( m , V )$ random variable, 

$$
E [ e ^ {\alpha X} ] = e ^ {\alpha m + \frac {1}{2} \alpha^ {2} V}.\tag{B.34}
$$

## B.5 Ito’s Lemma

If $X _ { t }$ satisfies 

$$
d X _ {t} = \mu_ {t} d t + \sigma_ {t} d W _ {t}\tag{B.35}
$$

and $F ( x )$ is a twice diferentiable function, then 

$$
d F (X _ {t}) = \frac {\partial F (X _ {t})}{\partial X _ {t}} d X _ {t} + \frac {1}{2} \frac {\partial^ {2} F (X _ {t})}{\partial X _ {t} ^ {2}} d X _ {t} ^ {2},\tag{B.36}
$$

where 

$$
d t ^ {2} = 0, \quad d t d W _ {t} = 0 \quad \mathrm{and} \quad d W _ {t} ^ {2} = d t.\tag{B.37}
$$

## B.6 Geometric Brownian Motion

$$
d S _ {t} = S _ {t} (\mu d t + \sigma d W _ {t})\tag{B.38}
$$

has solution 

$$
S _ {t} = S _ {0} \exp \left[ (\mu - \frac {1}{2} \sigma^ {2}) d t + \sigma W _ {t} \right].\tag{B.39}
$$

## B.7 Black-Scholes Formulae

The Black-Scholes equation for a derivative $C ( S _ { t } , t )$ is 

$$
\frac {\partial C}{\partial t} + \frac {1}{2} \frac {\partial^ {2} C}{\partial S _ {t} ^ {2}} S _ {t} ^ {2} \sigma^ {2} = r \left(C - \frac {\partial C}{\partial S _ {t}} S _ {t}\right).\tag{B.40}
$$

For a call option with payof function $C ( S _ { T } , T ) = \operatorname* { m a x } [ S _ { T } - K , 0 ]$ , it has solution 

$$
C _ {0} = e ^ {- r T} [ S _ {0} e ^ {r T} N (h ^ {+}) - K N (h ^ {-}) ].\tag{B.41}
$$

A put option with payof function $P ( S _ { T } , T ) = \operatorname* { m a x } [ K - S _ { T } , 0 ]$ , it has 

$$
P _ {0} = e ^ {- r T} [ K N (- h ^ {-}) - S _ {0} e ^ {r T} N (- h ^ {+}) ],\tag{B.42}
$$

where 

$$
h ^ {\pm} \equiv \frac {\ln (\frac {S _ {0} e ^ {r T}}{K}) \pm \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}.\tag{B.43}
$$

The payof for a call option with dividends is 

$$
C _ {0} = \frac {e ^ {- (r - \delta^ {C}) T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F (S _ {0} e ^ {(r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T}) e ^ {- \frac {1}{2} \xi^ {2}} d \xi\tag{B.44}
$$

For the Black-Scholes formula we then obtain, in the case of a call option (with no dividends paid on the option itself): 

$$
C _ {0} = e ^ {- r T} [ S _ {0} e ^ {(r - \delta) T} N (h ^ {+}) - K N (h ^ {-}) ],\tag{B.45}
$$

where 

$$
h ^ {\pm} = \frac {\ln (\frac {\tilde {S} _ {T}}{K}) \pm \frac {1}{2} \sigma^ {2} T)}{\sigma \sqrt {T}}.\tag{B.46}
$$

We still need to derive the formula in the case of a put option with dividends. Put-call parity says that 

$$
C _ {0} = S _ {0} - e ^ {- r T} K + P _ {0}.\tag{B.47}
$$

## B.8 Bernoulli Distribution

The simplest nontrivial discrete probability distribution is the Bernoulli distribution. There are only two points in the sample space $\Omega = \{ u , d \}$ . The probability distribution is then 

$$
\begin{array}{l} \operatorname{Prob} [ X = u ] = p \\ \operatorname{Prob} [ X = d ] = 1 - p \end{array}\tag{B.48}
$$

The expectation of the random variable X is $E [ X ] = p u + ( 1 - p ) d ;$ the variance is $V [ X ] = p ( 1 - p ) ( u - d ) ^ { 2 }$ 

## B.9 Binomial Distribution

This distribution is obtained by the consideration of n indepentant, identical Bernoulli trials. Let X be the random variable which counts the total number of u’s in n trials. We can obtain this by setting $u = 1 , d = 0$ , and summing over n independent Bernoulli trials $Y _ { i }$ . The binomial distribution is then given by 

$$
\operatorname{Prob} [ X = x ] = \left\{ \begin{array}{l l} \binom {n} {x} p ^ {x _ {i}} (1 - p) ^ {n - x _ {i}} & \text { for } x _ {i} = 0, 1, \ldots , n \\ 0 & \text { otherwise } \end{array} \right.\tag{B.49}
$$

The expectation of X is $E [ X ] = n p ;$ the variance of X is $V [ X ] = n p ( 1 - p )$ Here the combinatorial function $\left( { \begin{array} { l } { n } \\ { x } \end{array} } \right)$ , sometimes denoted $C _ { x } ^ { n }$ (‘n choose $x ^ { \prime } )$ is defined by 

$$
\binom{n}{x} = \frac {n !}{x ! (n - x) !}.\tag{B.50}
$$

## B.10 Central Limit Theorem

Let $X _ { i } \ ( i = 1 , \ldots , n )$ be a set of n independent, identically distributed random variables, each with mean m and variance V. Define 

$$
Z _ {n} = \frac {\sum_ {i = 1} ^ {n} (X _ {i} - m)}{\sqrt {n}}.\tag{B.51}
$$

Then the limit 

$$
Z = \lim _ {n \to \infty} Z _ {n}\tag{B.52}
$$

exists, and is normally distributed with mean 0 and variance V . Equivalently, we can assert that 

$$
\lim _ {n \to \infty} \operatorname{Prob} \left[ \sum_ {i = 1} ^ {n} (X _ {i} - m) <   \lambda \sqrt {\operatorname{Var} [ \sum_ {i = 1} ^ {n} (X _ {i} - m) ]} \right] = N (\lambda),\tag{B.53}
$$

where $N ( \lambda )$ is the normal distribution function. 

We can use the Central Limit Theorem to analyze the behaviour of the random variable $Z _ { n }$ in equation (B.51). We can rewrite $Z _ { n }$ in terms of the average ${ \bar { X } } _ { n }$ of n Bernoulli trials, 

$$
Z _ {n} = 2 \sqrt {n} (\bar {X} _ {n} - \frac {1}{2}),\tag{B.54}
$$

where 

$$
\bar {X} _ {n} = \frac {1}{n} \sum_ {i = 1} ^ {n} X _ {i}.\tag{B.55}
$$

Thus, by the Central Limit theorem $Z _ { n }$ approaches a normal distribution. Moreover, we can calculate the mean and variance of $\bar { X }$ as $E [ \bar { X } _ { n } ] = 1 / 2$ and $V [ \bar { X } _ { n } ] = n / 4$ , from which it follows that $E [ Z _ { n } ] = 0$ , and $V [ Z _ { n } ] = 1$ 

## C Solutions

## Section 1

1. Why do bond prices fall when the interest rate of the money market account rises? This is easiest to see by considering an example. Suppose that the initial value of the money market interest rate is $5 \%$ , and that at some time it increases to 6%. Before the interest rate rise, how much would you be willing to pay for a one-year bond with a notional of $100 and an annual interest rate of $7 \% 2$ This means that you pay an amount $B _ { 0 }$ for the bond now, and receive $107 dollars in one year’s time. We can determine $B _ { 0 }$ using arbitrage. 

Suppose that we start with nothing. In order to invest in the bond, we need to borrow $B _ { 0 }$ dollars from the money market account. Then in one year’s time, we receive $107 for the bond, but owe $B _ { 0 } e ^ { 0 . 0 5 }$ dollars for the loan. Since we started with nothing, we must end with nothing, and hence 

$$
1 0 7 - B _ {0} e ^ {0. 0 5} = 0\tag{C.1}
$$

which tells us that $B _ { 0 }$ is $1 0 7 e ^ { - . 0 5 } = 1 0 1 . 7 8$ dollars. This is how we can price bonds using arbitrage. 

Now suppose that we repeat the argument when the money market interest rate is 6% instead of 5%. The new price of the bond is $1 0 7 e ^ { - 0 . 0 6 } = 1 0 0 . 7 7$ dollars, which is less than the previous price. The price of the bond drops because the no arbitrage condition requires an investment in the bond to have the same return as an investment in the money market account. Because the interest rate on the bond is fixed, this is only possible if the bond price falls. 

Why does the value of a bond rise if the credit quality improves? This question is a little more dificult to quantify, since we have no exact mathematical way of describing loan default. However, suppose that we have two bonds which have the exact same characteristics, except that one is more likely to default than the other. Which are you willing to pay more for? Obviously the one which is less likely to default, that is, the one with the better credit rating. We now want to apply this argument to a single bond—but before and after an improvement in the credit quality. If the credit quality improves, and since all other properties of the bonds are the same, then by the above argument you should be willing to pay more for the bond after its credit rating has improved. This is why a bond price increases when credit quality improves. 

2. We want to calculate the efective continuously compound interest rate earned on an account which has an annual interest rate of $r = 6 . { \bar { 1 } } \%$ which is paid on a monthly compounded basis. Begin by assuming that we have $B _ { 0 }$ dollars in the bank. At the end of one month, the interest paid on this amount is $B _ { 0 } r / 1 2$ . That is, after one month, the amount that we have in the bank is 

$$
B _ {1} = B _ {0} (1 + r / 1 2).\tag{C.2}
$$

How about after the second month? Well, we earn an amount of interest equal to $B _ { 1 } r / 1 2$ , so 

$$
\begin{array}{r c l} B _ {2} & = & B _ {1} (1 + r / 1 2) \\ & = & B _ {0} (1 + r / 1 2) ^ {2}. \end{array}\tag{C.3}
$$

By induction, you should see that for $m \leq 1 2$ 2 

$$
B _ {m} = B _ {0} (1 + r / 1 2) ^ {m},\tag{C.4}
$$

and hence after a year 

$$
B _ {1 2} = B _ {0} (1 + r / 1 2) ^ {1 2}.\tag{C.5}
$$

What is the efective continuously compounded interest rate $\rho ?$ We can calculate this by noting that after one year, an initial investment of ${ \bf \dot { \boldsymbol B } } _ { 0 }$ dollars would be worth $\boldsymbol { B _ { 0 } e ^ { \rho } }$ dollars. Equating the two results we see that 

$$
B _ {0} (1 + r / 1 2) ^ {1 2} = B _ {0} e ^ {\rho},\tag{C.6}
$$

or 

$$
\begin{array}{r c l} \rho & = & 1 2 \log (1 + r / 1 2) \\ & = & 0. 0 6 0 8, \end{array}\tag{C.7}
$$

and hence the efective continuosly compounded rate is 6.08%. 

Note that if we divide the year up into n equal periods and repeat the above argument, then the amount of money in the bank account at the end of the year is 

$$
B _ {n} = B _ {0} (1 + r / n) ^ {n}.\tag{C.8}
$$

As we take n very large, we see that 

$$
\lim _ {n \to \infty} B _ {n} = B _ {0} e ^ {r},\tag{C.9}
$$

which is the continuously compounded limit. 

3. If we are paying interest into a money market account at a constant rate of r dollars per unit time, then the change $d B _ { t }$ in the amount of money in the bank account over the time interval $[ t , t + { \dot { d } } t ]$ is equal to the amount of interest paid, which is $r B _ { t } d t$ . Thus, the diferential equation is 

$$
\frac {d B _ {t}}{d t} = r B _ {t}.
$$

This has solution 

$$
B _ {t} = B _ {0} e ^ {r t}.
$$

This relation will be used throughout the book to describe the time evolution of a money market account. 

4. The most money that you can lose by buying an option is the purchase price that you paid for it. You never lose more because if the payof of the option is negative (the derivative is out of the money), then you simply do not ‘exercise your option’ and the option expires unused. This should be contrasted with a forward contract on an asset, which is a strict obligation – you must buy the asset at the strike price, whether it is beneficial to you or not. 

<table><tr><td>Option Type</td><td>Strike</td><td>Market Value</td><td>Intrinsic Value</td></tr><tr><td>American Call</td><td>6000</td><td>£1265</td><td>£850</td></tr><tr><td>American Put</td><td>6000</td><td>£295</td><td>£0</td></tr><tr><td>European Call</td><td>6025</td><td>£1085</td><td>£600</td></tr><tr><td>European Put</td><td>6025</td><td>£340</td><td>£0</td></tr></table>

5. For the call and put options specified in the text, the market and intrinsic (if the option were exercised immediately) values are given below. 

The market values are greater than the intrinsic values because they take into account the fact that the value of the index may achieve higher values before it expires, and hence pay out more than its current intrinsic value. The buyer of the option must pay for this potential gain, which is why the market value is larger than the intrinsic value. A reverse argument also may be applied, that the index may go down and the payof be less, however from a purely heuristic point of view, the total possible drop in the payof is less than the total possible gain in the payof (which is unlimited). 

6. A bank with a large number of fixed-rate loans or mortgages has a great deal of interest-rate risk. If the interest rate rises, then the bank will be receiving less than the market rate for its investments. In essence, it will be losing money. A company that sells products domestically, but buys supplies, for example timber, from a foreign nation, has a foreign-exchange risk. The price of timber will become more expensive if the foreign currency appreciates against the local currency, but the income from domestic sales is unafected. Thus, the company will efectively be losing money. 

7. Suppose a dealer sells a put with strike K. If the value of the stock $S _ { T }$ is lower than the strike when the put is exercised, then the dealer must pay the owner of the option this diference. If the value of the stock is higher than the strike price, then the dealer does not have to pay anything. Thus, the payof function is $\dot { \mathbf { \xi } } - \operatorname* { m a x } [ K - S _ { t } , 0 ] = \operatorname* { m i n } [ S _ { t } - K , 0 ]$ , which is shown in figure A.1. 

Consider a portfolio which is long a call with strike K, and short a put with the same strike. The payof function for this portfolio is 

$$
\begin{array}{r c l} {V _ {T}} & = & {\max [ S _ {T} - K, 0 ] + \min [ S _ {T} - K, 0 ]} \\ & = & {S _ {T} - K,} \end{array}\tag{C.10}
$$

which is the same as the payof for a forward contract. Graphically, you can see that by adding the payofs from figures 1.1 and C.1 you obtain the payof in figure 1.3. The fact that the payof for a basic call option is equal to the payof for a put option plus a forward contract is known as put-call parity. 

8. Figure 1.4 is known as a ‘call spread’. It can be reconstructed by buying a call struck at $50 and selling one struck at $100. In Figure 1.5 we have given an example of a ‘butterfly option’, which consists of a long position in a call with strike $50, a short position in two calls with strike $100 and another long position in a call with strike $150 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/2cdb0e1f9a97bcf92c3801b21e4e5a2922ef671f15c3cf2e1f63990c141b9c5c.jpg)



Figure C.1: The payof function of a short position in a put with a strike of $100 as a function of the price of the underlying asset.


## Section 2

1. We want to show that if a dealer ofers a forward rate of $F _ { t } < \tilde { S } _ { t }$ then an arbitrageur can make a sure profit. To this end, in figure C.2 an analogous trading strategy to the one given for the case $F _ { t } > \tilde { S } _ { t }$ is described. The strategy allows an arbitrageur to start with nothing, but to end with a guaranteed positive amount in a sterling bank account. The final value of the sterling bank account is greater than zero, which implies that an arbitrageur following this strategy can make a risk-free profit. 

2. We want to calculate the forward exchange rate for an initial rate of $1.60, and interest rates of $r = 1 0 \%$ and $\rho = 8 \%$ . From equation (2.4), we see that that the forward exchange rate is 

$$
\begin{array}{r c l} \tilde {S} _ {t} & = & (1. 6 0) \exp [ (0. 1 - 0. 0 8) 2 ] \\ & = & 1. 6 7. \end{array}\tag{C.12}
$$

3. We want to calculate the forward rate for a situation where the sterling interest rate follows the time dependent relation $\rho ( t ) = a + b t$ . However, we can proceed just as in the time independent case, and simply equate the results obtained by following the dollar investment and forward buying strategies of chapter 2. Starting with n units of sterling, the dollar investment route yields $n S _ { 0 }$ exp(rt) dollars, while the forward buying route has a final value of $n \tilde { S } _ { t } \exp ( a t + b t ^ { 2 } / 2 )$ dollars. Equating the two yields 

$$
\tilde {S} _ {t} = S _ {0} e ^ {(r - a) t - \frac {1}{2} b t ^ {2}}.\tag{C.13}
$$

Arbitrage Strategy II:
1. Borrow n units of sterling.
2. Convert the sterling at the spot rate $S_{0}$ into $nS_{0}$ dollars. Place these dollars into a dollar bank account, earning interest at the rate r. Contract to sell $nS_{0}e^{rt}$ dollars forward at time t at the rate $F_{t}$ (assumed $<\tilde{S}_{t}$ ).
3. At time t, the value of the dollar bank account is $nS_{0}e^{rt}$ , while the sterling position is $-ne^{\rho t}$ .
4. Sell $nS_{0}e^{rt}$ dollars at the contracted forward rate $F_{t}$ , which gives $nS_{0}e^{rt}/F_{t}$ pounds. After the arbitrageur repays the sterling loan, with interest, the balance in the sterling account is
 [ \frac{nS_{0}e^{rt}}{F_{t}}-ne^{\rho t}=\frac{ne^{\rho t}}{F_{t}}(S_{0}e^{(r-\rho)t}-F_{t}) ] 
 [ =\frac{ne^{\rho t}}{F_{t}}(\tilde{S}_{t}-F_{t}) ]  (C.11) 


Figure C.2: Arbitrage Strategy II


For a two-year forward purchase, we see that 

$$
\tilde {S} _ {2} = (1. 6 0) \exp [ (0. 1 - 0. 8) 2 - \frac {1}{2} 0. 0 1 2 ^ {2} ] = 1. 6 3
$$

Note that this is lower than the forward exchange rate of exercise 2.2. For the four-year forward purchase, the rate is 

$$
\tilde {S} _ {4} = (1. 6 0) \exp [ (0. 1 - 0. 8) 4 - \frac {1}{2} 0. 0 1 4 ^ {2} ] = 1. 6
$$

which is coincidentally the initial rate. 

## Section 3

1. We want to use a simple arbitrage argument to show that the basic stake $S _ { 0 }$ and the payof values U and D satisfy $U > S _ { 0 } > D$ Without loss of generality we can assume that $U > D . { \mathrm { ~ I f ~ } } U = D$ , then there is no point tossing the coin, and hence no point betting. If $S _ { 0 } \geq U$ , then by placing a short bet an arbitrageur could guarantee to not lose any money and to potentially make some, since the two possible payofs, $S _ { 0 } - U$ and $\check { S } _ { 0 } - D _ { \mathrm { \ell } }$ , are both non-negative. Similarly if $S _ { 0 } \le D$ , then the payofs from a standard bet, $U - S _ { 0 }$ and $D - { \breve { S } } _ { 0 }$ are both greater than or equal to zero, and hence the arbitrageur would not have anything to lose by betting. Thus, we must have $D < S _ { 0 } < U$ 

2. We want to calculate the dealer’s payof for the hedged bet. The payof is $\delta U - f _ { t } ( U )$ dollars, where 

$$
\delta = \frac {f _ {t} (U) - f _ {t} (D)}{U - D}\tag{C.14}
$$

and hence the payof is 

$$
\frac {f _ {t} (U) - f _ {t} (D)}{U - D} U - f _ {t} (U) = \frac {D f _ {t} (U) - U f _ {t} (D)}{U - D}\tag{C.15}
$$

dollars. 

3. Suppose that a derivative has payof function $f _ { t } ( S _ { t } )$ , and that the dealer makes a price of g dollars, which is assumed to be less than the arbitrage price of $f _ { 0 }$ dollars. Consider an arbitrageur that starts with empty pockets and borrows $g _ { 0 } - \delta S _ { 0 }$ dollars interest-free from the Casino, where δ is the hedge ratio given by equation (3.7), 

$$
\delta = \frac {f _ {t} (U) - f _ {t} (D)}{U - D}.
$$

The arbitrageur then buys the derivative from the dealer at price $g _ { 0 }$ , and makes a short bet with the casino, in the quantity $\delta S _ { 0 } , \mathrm { i . e }$ . the Casino pays the arbitrageur $\delta S _ { 0 }$ at $t = 0$ , and the arbitrageur must pay the Casino $\delta S _ { 1 }$ at time t. 

Thus, at time t the arbitrageur gets the certain amount $f _ { t } ( S _ { t } ) - \delta S _ { t }$ dollars, in other words, he gets $f _ { t } ( S _ { t } )$ dollars from dealer, but has to pay $\delta S _ { t }$ dollars to the Casino. However, the loan of $g _ { 0 } - \delta S _ { 0 }$ dollars must also be repaid. Thus the arbitrageur is left with 

$$
f _ {t} (S _ {t}) - \delta S _ {t} - (g _ {0} - \delta S _ {0})
$$

dollars. $\mathrm { B u t } ,$ recall that $f _ { 0 } = f _ { t } ( S _ { t } ) - \delta S _ { t } + \delta S _ { 0 }$ . So the arbitrageur is left with $f _ { 0 } - g _ { 0 }$ dollars, which is, by assumption, positive. Thus a sure profit with no risk has been made! Similarly if we took $g _ { 0 } > f _ { 0 }$ , then the arbitrageur could make a profit by taking a short hedged position. You should work out the details of this case as well. 

## Section 4

1. Let Ω be a sample space. We want to show that the power set ${ \mathcal { P } } ( \Omega )$ , which is the set of all subsets of Ω, is a valid event space. Since Ω is a subset of itself, $\Omega \in \mathcal { P } ( \Omega )$ If $A , B \in { \mathcal { P } } ( \Omega )$ , then they are subsets of Ω, that is $A , B \subset \Omega$ . But then $A \cup B \subset \Omega$ so $A \cup B \in { \dot { \mathcal { P } } } ( \Omega )$ ). Finally if $A \in \mathcal { P } ( \Omega )$ , then $A \subset \Omega$ , and since the complement of A in Ω is simply the set of elements of Ω that are not in $A , \Omega - A \subset \Omega$ . Hence $\Omega - A \in \mathcal { P } ( \Omega )$ . Thus the power set is a valid event space. 

We now want to write out the power set for a ‘possibility system’ that is based on the outcome of two coin tosses. Denoting ‘heads’ by H and ‘tails’ by T, the sample space can be written as $\{ H H , H T , T T , ^ { * } T H \}$ . The power set will have $2 ^ { 4 } = 1 6$ elements and is as follows: 

$$
\begin{array}{r c l} \Sigma & = & \Big \{\emptyset , \\ & & \{H H \}, \{H T \}, \{T T \}, \{T H \}, \\ & & \{H H, H T \}, \{H H, T T \}, \{H H, T H \}, \{H T, T T \}, \{H T, T H \}, \{T T, T H \}, \\ & & \{H H, H T, T T \}, \{H H, H T, T H \}, \{H H, T T, T H \}, \{H T, T T, T H \}, \\ & & \{H H, H T, T T, T H \} \Big \}. \end{array}
$$

2. We want to prove that given a sample space $\Omega ,$ the set $\Sigma = \{ \emptyset , \Omega \}$ is a valid event space. By definition, Σ satisfies $\Omega \in \Sigma$ . Since $\Omega \cup \emptyset = \Omega .$ , and these are the only two elements in $\Sigma .$ we see that Σ is closed under the union of its elements. Furthermore, since $\Omega - \emptyset = { \dot { \Omega } }$ and $\Omega - \Omega = \emptyset$ , we see that Σ is closed under complementation of its elements. Hence $\Sigma = \{ \emptyset , \Omega \}$ is a valid event space. However, it is not very useful, as the only events that it can diferentiate between are whether the experiment had an outcome or not. 

3. We want to show for a possibility system based on a finite sample space Ω and an event space $\Sigma$ equal to the power set of $\Omega ,$ , that any probability measure $P$ is uniquely defined by its values on the single element sets of the event space, that is, on the ‘probabilities’ of the sample space. Let $\Omega = \{ \omega _ { i } \} _ { i = 1 } ^ { N }$ , and let A be any element of $\Sigma .$ . But then A is simply a subset of Ω, and hence $A = \{ \omega _ { i _ { k } } \} _ { k = 1 } ^ { M }$ for some sequence $i _ { k }$ . We can then use the property that the probability of the union of disjoint sets is equal to the sum of the individual probabilities, that is, 

$$
\begin{array}{r c l} P (A) & = & P \left(\{\omega_ {i _ {k}} \} _ {k = 1} ^ {M}\right) \\ & = & \sum_ {k = 1} ^ {M} P \left(\{\omega_ {i _ {k}} \}\right) \\ & = & \sum_ {k = 1} ^ {M} p _ {i _ {k}}. \end{array}\tag{C.16}
$$

Thus we see that the probability of any set is simply the sum of the ‘probabilities’ of its individual elements. 

4. We want to calculate the probability, in the the possibility system (Ω, Σ) based on three coin tosses, that there are exactly two heads. This event is $A = \dot { \{ H H T , H T H , T H H \} }$ We have two probability systems in which to calculate the probability of A. Suppose that we are in the ‘equal probability’ system $( \Omega , \Sigma , P )$ . The probability of A is 

$$
\begin{array}{r c l} P (\{H H T, H T H, T H H \}) & = & P (\{H H T \}) + P (\{H T H \}) + P (\{T H H \}) \\ & = & \frac {3}{8}. \end{array} \tag {6}\tag{C.17}
$$

In the ‘weighted coin’ probability system (Ω, Σ, Q) we have 

$$
\begin{array}{r c l} Q (\{H H T, H T H, T H H \}) & = & Q (\{H H T \}) + Q (\{H T H \}) + Q (\{T H H \}) \\ & = & \frac {2}{9}. \end{array} \tag {6}\tag{C.18}
$$

5. We want to calculate the expectation of the random variable $X$ that returns the number of ‘heads’ in three coin tosses for both the ‘equal probability’ and ‘weighted coin’ probability measures $P$ and $Q .$ The values of $\dot { X }$ were written out in equation (4.4). For the probability measure ${ \bf \dot { \boldsymbol { P } } } .$ the expectation is 

$$
{E ^ {P} [ X ]} = {\frac {1}{8} X (\{H H H \}) + \frac {1}{8} X (\{H H T \}) + \frac {1}{8} X (\{H T H \}) + \frac {1}{8} X (\{T H H \}) +}
$$

$$
\begin{array}{l l} & \frac {1}{8} X (\{H T T \}) + \frac {1}{8} X (\{T T H \}) + \frac {1}{8} X (\{T H T \}) + \frac {1}{8} X (\{T T T \}) \\ = & \frac {1}{8} [ 3 + 2 + 2 + 2 + 1 + 1 + 1 + 0 ] \\ = & 1. 5, \end{array}\tag{C.19}
$$

while for the measure $Q ,$ we have 

$$
\begin{array}{r c l} E ^ {Q} [ X ] & = & \frac {1}{2 7} X (\{H H H \}) + \frac {2}{2 7} X (\{H H T \}) + \frac {2}{2 7} X (\{H T H \}) + \frac {2}{2 7} X (\{T H H \}) + \\ & & \frac {4}{2 7} X (\{H T T \}) + \frac {4}{2 7} X (\{T T H \}) + \frac {4}{2 7} X (\{T H T \}) + \frac {8}{2 7} X (\{T T T \} \\ & = & \frac {1}{2 7} [ 3 + 2 (2 + 2 + 2) + 4 (1 + 1 + 1) + 0 ] \\ & = & 1. \end{array} \tag {C.20}
$$

Let Y be the random variable which is equal to twice the number of ‘heads’ minus the number of ‘tails’. To simplify the calculation, let W be the random variable equal to the number of ‘tails’. Then $Y = 2 ( X - { \dot { W } } )$ . But, $X + W = 3 .$ so we see that 

$$
\begin{array}{r c l} Y & = & 2 [ X - (3 - X) ] \\ & = & 4 X - 6. \end{array}\tag{C.21}
$$

Using the result above for the expectation of $X ,$ , we can calculate the expectation of $Y$ , first in the probability measure $P$ 

$$
\begin{array}{r c l} E ^ {P} [ Y ] & = & E ^ {P} [ 4 X - 6 ] \\ & = & 4 E ^ {P} [ X ] - 6 \\ & = & 0, \end{array}\tag{C.22}
$$

and next in the measure $Q$ 

$$
\begin{array}{r c l} {E ^ {Q} [ Y ]} & = & {4 E ^ {Q} [ X ] - 6} \\ & = & {- 2.} \end{array}\tag{C.23}
$$

Let $Z$ be the random variable defined by 

$$
Z (\{A B C \}) = \left\{ \begin{array}{l l} 1 & A B C = H H H \\ 0 & \text { otherwise } \end{array} \right..
$$

In the ‘equal probability’ measure $P$ the expectation is 

$$
\begin{array}{r c l} E ^ {P} [ Z ] & = & P (\{H H H \}) Z (\{H H H \}) \\ & = & \frac {1}{8}, \end{array}\tag{C.24}
$$

while in the ‘weighted coin’ measure $Q$ 

$$
\begin{array}{r c l} {E ^ {Q} [ Z ]} & = & {Q (\{H H H \}) Z (\{H H H \})} \\ & = & {\frac {1}{2 7}.} \end{array}\tag{C.25}
$$

## Section 5

1. $P _ { 0 t }$ be a decreasing function of t because ... 

2. We want to show that if the dealer misprices a derivative and sells it for $g _ { 0 }$ dollars, which is less than the arbitrage value of $f _ { 0 }$ dollars, then an arbitrageur can make a sure profit. Suppose that the arbitrageur starts with nothing. Since the derivative is priced too low, he will buy it from the dealer for the price of $g _ { 0 }$ dollars and then hedge this derivative position by making a short bet with the Casino in the amount of $\bar { \delta S _ { 0 } }$ dollars, where δ is the hedge ratio (5.8). In order to fund this position, the arbitrageur must borrow $g _ { 0 } - \delta S _ { 0 }$ dollars from the bank at an interest rate r. Note that if $g _ { 0 } - \delta S _ { 0 }$ is negative then the arbitrageur is actually depositing money in the bank. At time $t ,$ the arbitrageur receives $f _ { t } ( S _ { t } )$ dollars from the dealer for the derivative and has to pay $\delta S _ { t }$ dollars to the Casino in order to cover his short bet. Furthermore, the loan, which is now worth $( g _ { 0 } - \delta S _ { 0 } ) e ^ { r t }$ dollars, must be repaid to the bank. Hence the net position of the arbitrageur after the coin toss is $f _ { t } ( S _ { t } ) - \delta S _ { t } - ( g _ { 0 } - \delta S _ { 0 } ) e ^ { r t }$ dollars. From equation (5.9) we see that $f _ { 0 } e ^ { r t } = f _ { t } ( S _ { t } ) - \delta S _ { t } + \delta S _ { 0 } e ^ { r t }$ , and hence the arbitrageur’s position is worth the guaranteed amount of 

$$
f _ {t} (S _ {t}) - \delta S _ {t} - (g _ {0} - \delta S _ {0}) e ^ {r t} = (f _ {0} - g _ {0}) e ^ {r t}\tag{C.26}
$$

dollars. Since $f _ { 0 } > g _ { 0 }$ the arbitrageur has made a sure profit, starting from nothing. If the derivative were over-priced, so $g _ { 0 } > f _ { 0 } ,$ , then the arbitrageur could construct a gambling portfolio which is short a derivative and long $\delta$ units of the basic bet to guarantee a profit. 

3. Suppose that the basic bet in the Casino is $100 and that it pays of $105 and $95 for heads and tails respectively, while the continuously compounded interest rate is $r t = \log 1 . 0 1$ 

(a) We want to calculate the risk-neutral probabilities. They are given by equation ??. Substituting in the values for $S _ { 0 } , U , D$ and $e ^ { r t }$ , we have 

$$
\begin{array}{r c l} p ^ {*} & = & \frac {(1 0 0) (1 . 0 1) - 9 5}{1 0 5 - 9 5} \\ & = & 0. 6, \end{array}\tag{C.27}
$$

and hence $q ^ { * } = 1 - p ^ { * } = 0 . 4$ 

(b) We now want to price a call option with a strike of $100. The payof function $f _ { t } ( S _ { t } )$ for this derivative, is 

$$
f _ {t} (U) = 5 \quad \text { and } \quad f _ {t} (D) = 0.
$$

Using the risk-neutral probabilities calculated above, and the pricing formula $f _ { 0 } = \smile e ^ { - r t } E ^ { * } [ f _ { t } ( S _ { t } ) ]$ , we see that the cost of the derivative is 

$$
\begin{array}{r c l} f _ {0} & = & \frac {1}{1 . 0 1} [ (0. 6) 5 + (0. 4) 0 ] \\ & = & 2. 9 7 \end{array}\tag{C.28}
$$

dollars. 

(c) The hedge ratio is given by equation (3.7). Substituting in the relevant values yields 

$$
\begin{array}{r c l} \delta & = & \frac {5 - 0}{1 0 5 - 9 5} \\ & = & 0. 5. \end{array}\tag{C.29}
$$

(d) We want to verify that the payof of a bet that is long $\delta$ units of the basic bet and short one derivative is independent of the outcome of the coin toss. $\mathrm { A t }$ time t the value of this hedged bet is $\delta S _ { t } - f _ { t } ( S _ { t } )$ . If the coin toss is heads, then the payof is 

$$
\begin{array}{r c l} \delta U - f _ {t} (U) & = & (0. 5) 1 0 5 - 5 \\ & = & 4 7. 5 0 \end{array}\tag{C.30}
$$

dollars, while if the coin flip is tails, then the result is 

$$
\begin{array}{r c l} \delta D - f _ {t} (D) & = & (0. 5) 9 5 - 0 \\ & = & 4 7. 5 0 \end{array}\tag{C.31}
$$

dollars. Thus the payof from the hedged bet is $47.50 and is independent of the outcome of the coin toss. 

(e) The cost of the derivative is independent of the ‘physical’ coin toss probabilties, p and $\smash { q , }$ and depends only on the risk-neutral probabilities $p ^ { * }$ and $q ^ { * }$ Hence even if we change the physical probabilities the cost of the derivative is still $2.97. 

4. We want to show that the risk-neutral probabilities $p ^ { * }$ and $q ^ { * }$ are uniquely defined by the requirement that $S _ { 0 } = e ^ { - r t } E ^ { * } [ S _ { t } ]$ . Suppose that we have diferent probabilities $\tilde { p }$ and $\tilde { q }$ that define a probability measure $\tilde { P }$ such that $S _ { 0 } = e ^ { - r t } \tilde { E } [ S _ { t } ]$ . Then 

$$
\begin{array}{r c l} {S _ {0}} & = & {e ^ {- r t} [ \tilde {p} U + \tilde {q} D ]} \\ & = & {e ^ {- r t} [ \tilde {p} (U - D) + D ].} \end{array}\tag{C.32}
$$

Solving for $\tilde { p } ,$ we obtain 

$$
\tilde {p} = \frac {S _ {0} e ^ {r t} - D}{U - D}.\tag{C.33}
$$

But, this is simply $p ^ { * } !$ Hence, the condition $S _ { 0 } = e ^ { - r t } \tilde { E } [ S _ { t } ]$ uniquely determines the risk-neutral probabilities. 

## Section 6

1. We want to calculate various probabilities for the numeric example illustrated in (6.12). The probability that $\mathit { \bar { S } } _ { 2 } ~ = ~ 1 0 2$ is simply the probability that we have an initial ‘up’ movement times the probability that this is followed by a ‘down’ movement, that is $p ^ { 0 } \hat { p } ^ { 0 1 }$ . Substituting in the numbers yields $0 . 5 \times \dot { 0 . 3 } = 0 . 1 5$ We can calculate the probability that $\breve { S } _ { 2 } > 9 5$ by noting that it is one minus the probability that $S _ { 2 } \leq \mathsf { \hat { 9 } } 5$ , which is equal to the probability that $S = 9 2$ . This is the probability of having two ‘down’ movements, which is given by $0 . 5 \times 0 . 3 = 0 . 1 5$ Hence the probability of $S _ { 2 }$ being greater than 95 is $1 - 0 . 1 5 = \mathrm { \dot { 0 } } . 8 5$ 

2. We want to calculate the annualised continuously compounded interest rate r for the bond process $\$ 100\to\ S 101 \to \ S 102.01$ where each time step is one month. At $t = 1 / 1 2$ , that is, after one month, a continuously compounded investment of $100 will be worth $\$ 100 e^ { r / 12 }$ . Equating this to the value of the bond process after one month $B _ { 1 } = \mathfrak { H } 1 0 1$ , we see that 

$$
\begin{array}{r c l} 1 0 0 e ^ {r / 1 2} & = & 1 0 1 \\ r / 1 2 & = & \log 1. 0 1 \\ r & = & 0. 1 1 9 4, \end{array}\tag{C.34}
$$

thus the interest rate is 11.94% per year. 

3. Using the numeric stock and bond processes given in (6.12) and (6.13), we want to calculate the price of two call options which have maturity at time 1 and strikes of $98 and $102 respectively. Before we can calculate any prices however, we need to determine the risk-neutral probabilities. Fortunately we have already done this—in exercise 5.3 we considered an identical system, albeit with only one-period, and obtained the risk neutral probabilities $p _ { * } ^ { 0 } = 0 . 6$ and $p _ { * } ^ { 1 } = 0 . 4$ . We can then price any derivative by using the discounted expectation of the payof in the risk-neutral probability system, 

$$
\begin{array}{r c l} f _ {0} & = & E ^ {*} [ f _ {1} ] B _ {0} / B _ {1} \\ & = & \frac {p _ {*} ^ {0} f ^ {0} + p _ {*} ^ {1} f ^ {1}}{B _ {1} / B _ {0}} \\ & = & \frac {0 . 6 f ^ {0} + 0 . 4 f ^ {1}}{1 . 0 1}. \end{array}\tag{C.35}
$$

For the call with a strike of $102, the payof in the event of an $^ { \circ } \mathrm { u p } ^ { \prime }$ movement is $f ^ { 0 } = \mathbb { \ S } 1 0 5 - \mathbb { \ S } 1 0 2 = \mathbb { \ S } 3$ , while for a ‘down’ movement $f ^ { 1 } = \$ 80$ . Subsituting this payof function into the pricing formula (C.35) we obtain $\dot { f } _ { 0 } = \mathfrak { H } 3 \times 0 . 6 / 1 . 0 1 = \check { \mathfrak { G } } 1 . 7 8$ If the strike is $98 then the payof function is $f ^ { 0 } = \$ 87$ and $f ^ { 1 } = \ S 0$ . Calculating the initial price of the derivative we find that it is $4.16. 

We want to calculate the value of the call options again, but this time we are buying them at time 1 with a maturity of time 2. Because there are two possible initial prices at time 1, $S ^ { 0 }$ and $S ^ { 1 }$ , we will need to calculate derivative prices for both cases. Begin by assuming that the first stock movement was $\mathrm { \dot { \cdot } u p } ^ { \mathrm { \prime } }$ , so that $S _ { 1 } = \mathbb { S } 1 0 5$ . But then the time step from $t = 1 \ \mathrm { t o } \ t = 2$ is a simple binomial tree, with an ‘up’ price of $108, and a ‘down’ price of $102. We can therefore calculate the risk-neutral probabilities using equation (5.11), and find that 

$$
\begin{array}{r c l} \hat {p} _ {*} ^ {0 0} & = & \frac {S ^ {0} B _ {2} / B _ {1} - S ^ {0 1}}{S ^ {0} - S ^ {1}} \\ & = & \frac {1 0 5 \times 1 . 0 1 - 1 0 2}{1 0 8 - 1 0 2} \\ & = & 0. 6 7 5, \end{array}\tag{C.36}
$$

and 

$$
\hat {p} _ {*} ^ {0 0} = \frac {S ^ {0 0} - S ^ {0} B _ {2} / B _ {1}}{S ^ {0} - S ^ {1}}
$$

$$
\begin{array}{r l} {=} & {\frac {1 0 8 - 1 0 5 \times 1 . 0 1}{1 0 8 - 1 0 2}} \\ {=} & {0. 3 2 5.} \end{array}\tag{C.37}
$$

We can now calculate the initial price $f ^ { 0 }$ of a derivative by using the discounted expectation of the payof in the risk-neutral system, 

$$
\begin{array}{r c l} f ^ {0} & = & \frac {\hat {p} _ {*} ^ {0 0} f ^ {0 0} + \hat {p} _ {*} ^ {0 1} f ^ {0 1}}{B _ {2} / B _ {1}} \\ & = & \frac {0 . 6 7 5 f ^ {0} + 0 . 3 2 5 f ^ {1}}{1 . 0 1}. \end{array}\tag{C.38}
$$

Recall that this formula assumes that the share price at time 1 is $S ^ { 0 }$ . If the share price is $S ^ { 1 }$ instead, then we will get a diferent formula. For the call option with a strike of $102, the payof function is $f ^ { 0 0 } = \$ 6$ and $f ^ { 0 1 } = \$ 0$ . We can substitute this into equation (C.38) to obtain a derivative price of $4.01. For the call with a strike of $98, the payof function is $f ^ { 0 0 } = \$ 10$ and $f ^ { 0 1 } = \$ 4$ . This yields an initial price of $7.97. 

An identical calculation can be carried out for the case when $S _ { 1 } = 9 5$ . In this case, the risk neutral probabilities are $\hat { p } _ { * } ^ { 1 0 } = 0 . 6 5 8$ and $\hat { p } _ { * } ^ { 1 1 } = 0 . 3 4 2$ . However, the payof functions for both call options are identically zero, and hence without further calculation we see that their initial prices will be zero. 

We now want to price the call options at time 0 when they have a maturity at time 2. This is equivalent to finding the value at time 0 of a derivative which pays of $f ^ { i }$ at time 1. Why? Because we can think of the following two investment strategies: (a) buy a call option at time 0 which pays of at time 2 and (b) buy a derivative at time 0 which pays $f _ { 1 }$ at time 1, and then use the proceeds of this payof to buy a call option which pays of at time 2. Since both strategies have the same payof they must have the same initial price, otherwise we could arbitrage by going long the cheaper strategy and shorting the more expensive one. By substituting the values calculated above for $f ^ { 0 }$ and $\bigcup f ^ { 1 }$ into the pricing formula (C.35) we can obtain the initial price of strategy (b), and hence of strategy (a) and the call option that we are interested in pricing. The price of the call option with strike $102 is 

$$
\begin{array}{rcl}f & = & \frac{0.6f^0 + 0.4f^1}{1.01}\\ & = & \frac{0.6\times\$4.01 + 0.4\times\$0}{1.01}\\ & = & \$2.38. \end{array}\tag{C.39}
$$

For the call option with a strike of 98, we can substitute in the derivative values $f ^ { 0 } = \$ 57 .97$ and $f ^ { 1 } = \$ 0$ to find the initial price of $4.73. 

4. We want to compare the Casino price equation (5.13), 

$$
f _ {0} = e ^ {- r t} \left(\frac {S _ {0} e ^ {r t} - D}{U - D} f _ {t} (U) + \frac {U - S _ {0} e ^ {r t}}{U - D} f _ {t} (D)\right),\tag{C.40}
$$

with the one-period derivative price of equation (6.21). If we make the substitutions $e ^ { r t } \to B _ { 1 } / \bar { B } , \stackrel { \cdot } { U } \to S ^ { 0 } , D \to \hat { S } ^ { 1 } , \ : f _ { t } ( U ) \ : \stackrel { \cdot } { \to } \ : f ^ { 0 }$ and $f _ { t } ( D ) \to f ^ { 1 }$ in the Casino price equation, then we obtain 

$$
f = \frac {B}{B _ {1}} \left[ \frac {S \frac {B _ {1}}{B} - S ^ {1}}{S ^ {0} - S ^ {1}} f ^ {0} + \frac {S ^ {0} - S \frac {B _ {1}}{B}}{S ^ {0} - S ^ {1}} f ^ {1} \right],\tag{C.41}
$$

which is exactly the one-period result. Hence the Casino and the binomial tree model price derivatives in the same way. 

5. We want to verify that the ‘probabilities’ introduced in equation (6.22), 

$$
p _ {*} ^ {0} = \frac {\tilde {S} - S ^ {1}}{S ^ {0} - S ^ {1}} \quad \mathrm{and} \quad p _ {*} ^ {1} = \frac {S ^ {0} - \tilde {S}}{S ^ {0} - S ^ {1}},\tag{C.42}
$$

where $\tilde { S } = S B _ { 1 } / B$ , generate a valid probability measure. We first note that 

$$
p _ {*} ^ {0} + p _ {*} ^ {1} = 1.\tag{C.43}
$$

We then need to show that the probabilities are both positive. We can do this by applying an arbitrage argument to the values of $\tilde { S } , S ^ { 0 }$ and $S ^ { 1 }$ . By assumption we take $S ^ { 1 } < S ^ { 0 }$ . Suppose that $\tilde { S } \le S ^ { 1 }$ . We can then form an arbitrage strategy by starting with nothing, and then going long on stocks and shorting the bonds. The initial holding of the portfolio is $\alpha S - B$ , where $\alpha = B / S$ so that the net value of the investment is zero. At time 1 the position is worth $\alpha S _ { 1 } - B _ { 1 }$ . The minimum value of this random amount occurs when $S _ { 1 } = S ^ { 1 }$ . We then see that 

$$
\begin{array}{r c l} \alpha S _ {1} - B _ {1} & \geq & \alpha S ^ {1} - B _ {1} \\ & \geq & \alpha (S ^ {1} - B _ {1} / \alpha) \\ & \geq & \alpha (S ^ {1} - \tilde {S}) \end{array}\tag{C.44}
$$

But, since $S ^ { 1 } \geq { \tilde { S } } ,$ we can never lose money by investing this way, and we will make some whenever $S _ { 1 } = S ^ { 0 }$ . Hence there is an arbitrage opportunity and to avoid it we must have $S ^ { 1 } < { \tilde { S } }$ . This tells us that $p _ { * } ^ { 0 } > 0 . \mathrm { ~ A ~ }$ similar argument can be used to demonstrate that $S ^ { 0 } > { \tilde { S } }$ , and hence that $p _ { * } ^ { 1 } > 0$ . Thus the risk-neutral probabilities do, in fact, constitute a geunine probability measure. 

6. We want to find the forward price at time 0 for the purchase of one share at time 1. We can do this by considering a forward contract, which is an agreement made at time 0 to purchase a unit of stock for a fixed price K. This is a derivative which pays of $f _ { 1 } \stackrel { \cdot } { = } S _ { 1 } - K$ (which may be negative) at time 1. The price of the forward contract is 

$$
\begin{array}{r c l} f _ {0} & = & \frac {B}{B _ {1}} \left[ p _ {*} ^ {0} (S ^ {0} - K) + p _ {*} ^ {1} (S ^ {1} - K) \right] \\ & = & \frac {B}{B _ {1}} [ p _ {*} ^ {0} S ^ {0} + p _ {*} ^ {1} S ^ {1} ] - [ p _ {*} ^ {0} + p _ {*} ^ {1} ] \frac {B}{B _ {1}} K \\ & = & \frac {B}{B _ {1}} E ^ {*} [ S _ {1} ] - \frac {B}{B _ {1}} K \end{array}\tag{C.45}
$$

But, by definition of the risk-neutral probability, the first term is simply the price of a derivative which pays of the stock value at $t = 1$ , which is therefore the initial price of the stock. Hence 

$$
f _ {0} = S _ {0} - \frac {B}{B _ {1}} K.\tag{C.46}
$$

This is the price of a forward contract to buy a unit of stock at time 1 for the fixed price $K .$ . The forward price of the stock $F ,$ is the value of $K$ such that the cost of the contract is zero. Thus, 

$$
F = S _ {0} \frac {B _ {1}}{B}.\tag{C.47}
$$

The correct forward price can also be obtained by an arbitrage argument. Suppose that an investor agrees at time 0 to purchase a stock at time t from a dealer for the price $\tilde { S } _ { t }$ . The dealer immediately buys a share at the going rate $S _ { 0 }$ , using money borrowed at a continuously compounded rate $r .$ At time $t ,$ the dealer receives $\tilde { S } _ { t }$ for the share, and uses it to repay the loan of $S _ { 0 } e ^ { r t }$ . The dealer’s net position is therefore $\tilde { S } _ { t } - S _ { 0 } e ^ { r t }$ , and because he started with nothing this must be zero. Hence $\tilde { S } _ { t } = S _ { 0 } e ^ { r t }$ 

## Section 7

1. In a two-period market, we want to show that if $S _ { 1 } = S _ { 1 } ^ { 0 }$ , then the value of the derivative at $t = 1$ must be $f ^ { 0 }$ as given in equation (7.2), 

$$
\frac {f ^ {0}}{B _ {1}} = \frac {f ^ {0 0} p _ {*} ^ {0 0} + f ^ {0 1} p _ {*} ^ {0 1}}{B _ {2}},
$$

where 

$$
p _ {*} ^ {0 0} = \frac {\tilde {S} _ {1 2} ^ {0} - S ^ {0 1}}{S ^ {0 0} - S ^ {0 1}},
$$

$p _ { * } ^ { 0 1 } = 1 - p ^ { 0 0 } ,$ <sup>∗</sup> , and $\begin{array} { r } { \tilde { S } _ { 1 2 } ^ { 0 } = S ^ { 0 } \frac { B _ { 2 } } { B _ { 1 } } } \end{array}$ (the forward price, made at time 1, for delivery at time 2, if at time 1 the stock is in the $S ^ { 0 }$ state). 

We do this by constructing a replicating portfolio, just as we did in the one-period case. At $t = \dot { 1 }$ , the dealer sells an investor a derivative which will pay out either $f ^ { 0 0 }$ or $f ^ { 0 1 }$ at time 2. The proceeds $f ^ { 0 }$ from this sale are used to construct a hedging portfolio in the stock and bond markets. The dealer buys $\beta _ { 1 }$ bonds at a price of $\bar { B _ { 1 } } \bar { }$ each and $\delta _ { 1 }$ shares at a price of $S ^ { 0 }$ each. Since the dealer’s initial position is zero, we have 

$$
f ^ {0} = \beta_ {1} B _ {1} + \delta_ {1} S _ {1} ^ {0}.\tag{C.48}
$$

At the next period we want the stock and bond investments to exactly replicate the derivative payof, so 

$$
f ^ {0 i} = \beta_ {1} B _ {2} + \delta_ {1} S _ {2} ^ {0 i}.\tag{C.49}
$$

Solving these two equations for $\beta _ { 1 }$ and $\delta _ { 1 }$ we get 

$$
\delta_ {1} = \frac {f ^ {0 0} - f ^ {0 1}}{S _ {2} ^ {0 0} - S _ {2} ^ {0 1}} \quad \text { and } \quad \beta_ {1} = \frac {f ^ {0 1} S _ {2} ^ {0 0} - f ^ {0 0} S _ {2} ^ {0 1}}{B _ {2} (S _ {2} ^ {0 0} - S _ {2} ^ {0 1})}.\tag{C.50}
$$

Plugging the values back into (C.48) we get 

$$
\frac {f ^ {0}}{B _ {1}} = \frac {1}{B _ {2}} \left[ \frac {S _ {1} ^ {0} \frac {B _ {2}}{B _ {1}} - S _ {2} ^ {0 1}}{S _ {2} ^ {0 0} - S _ {2} ^ {0 1}} f ^ {0 0} + \frac {S _ {2} ^ {0 0} - S _ {1} ^ {0} \frac {B _ {2}}{B _ {1}}}{S _ {2} ^ {0 0} - S _ {2} ^ {0 1}} f ^ {0 1} \right],
$$

which is the required result. 

Note, incidentally, that $\beta _ { 1 }$ and $\delta _ { 1 }$ are the ‘new’ hedge ratios that the dealer puts on at $t = 1$ . Strictly speaking, we should write $\beta _ { 1 } ^ { 0 } , \delta _ { 1 } ^ { 0 }$ to indicate that these are the hedge ratios at $t = 1$ for the ${ \bf \bar { \theta } }$ state (in the $S ^ { 1 }$ state, we would put on a diferent hedge). 

2. We want to show that the probability system generated by $p _ { * } ^ { i }$ and $p _ { * } ^ { i j }$ satisfies the relations (7.8), 

$$
\frac {B _ {1}}{B _ {0}} = \frac {E ^ {*} [ S _ {1} ]}{S _ {0}} \quad \text { and } \quad \frac {B _ {2}}{B _ {0}} = \frac {E ^ {*} [ S _ {2} ]}{S _ {0}}.\tag{C.51}
$$

The first equality is easy to verify, 

$$
\begin{array}{r c l} E ^ {*} [ S _ {1} ] & = & p _ {*} ^ {0} S ^ {0} + p _ {*} ^ {1} S ^ {1} \\ & = & \frac {\tilde {S} - S ^ {1}}{S ^ {0} - S ^ {1}} S ^ {0} - \frac {S ^ {0} - \tilde {S}}{S ^ {0} - S ^ {1}} S ^ {1} \\ & = & \tilde {S} \\ & = & S ^ {0} \frac {B _ {1}}{B _ {0}}. \end{array}\tag{C.52}
$$

In the two-period case, we have 

$$
E ^ {*} [ S _ {2} ] = p _ {*} ^ {0} \hat {p} _ {*} ^ {0 0} S _ {2} ^ {0 0} + p _ {*} ^ {0} \hat {p} _ {*} ^ {0 1} S _ {2} ^ {0 1} + p _ {*} ^ {1} \hat {p} _ {*} ^ {1 0} S _ {2} ^ {1 0} + p _ {*} ^ {1} \hat {p} _ {*} ^ {1 1} S _ {2} ^ {1 1}.\tag{C.53}
$$

Now consider the first two terms, 

$$
\begin{array}{r c l} \hat {p} _ {*} ^ {0 0} S _ {2} ^ {0 0} + \hat {p} _ {*} ^ {0 1} S _ {2} ^ {0 1} & = & \frac {\tilde {S} _ {1 2} ^ {0} - S _ {2} ^ {0 1}}{S _ {2} ^ {0 0} - S _ {2} ^ {0 1}} S _ {2} ^ {0 0} + \frac {S _ {2} ^ {0 0} - \tilde {S} _ {1 2} ^ {0}}{S _ {2} ^ {0 0} - S _ {2} ^ {0 1}} S _ {2} ^ {0 1} \\ & = & \tilde {S} _ {1 2} ^ {0}, \end{array}\tag{C.54}
$$

where $\begin{array} { r } { \tilde { S } _ { 1 2 } ^ { 0 } = S ^ { 0 } \frac { B _ { 2 } } { B _ { 1 } } } \end{array}$ . A similar relation holds for the next two terms, 

$$
\hat {p} _ {*} ^ {1 0} S _ {2} ^ {1 0} + \hat {p} _ {*} ^ {1 1} S _ {2} ^ {1 1} = \tilde {S} _ {1 2} ^ {1},\tag{C.55}
$$

where $\tilde { S } _ { 1 2 } ^ { 1 } = S ^ { 1 } B _ { 2 } / B _ { 1 }$ . Hence we see that 

$$
\begin{array}{r c l} E ^ {*} [ S _ {2} ] & = & [ p _ {*} ^ {0} S ^ {0} + p _ {*} ^ {1} S ^ {1} ] \frac {B _ {2}}{B _ {1}} \\ & = & \left[ S ^ {0} \frac {B _ {1}}{B _ {0}} \right] \frac {B _ {2}}{B _ {1}} \\ & = & S ^ {0} \frac {B _ {2}}{B _ {0}}, \end{array}\tag{C.56}
$$

where the second line follows from the previous argument. 

Do these two conditions uniquely define a probability measure? Consider the following two stock price processes: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/9accb8b9f9c1b1206db3d3ffaf8c86fb49af32f42685f5fab4fa0ebf80ed4566.jpg)


(C.57) 

and 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/a2b1b215cace590c854e6a3d870bd66ad264da226ef202e0bdf1bc7c8e55e778.jpg)


(C.58) 

Set the interest rate to zero. Then both these processes satisfy the relations (7.8), and hence they do not uniquely define a probability measure. 

3. In order to calculate the risk-neutral probabilities, we need the discounted stock prices, 

$$
\begin{array}{r c l} \tilde {S} _ {1 2} ^ {0} & = & S ^ {0} \frac {B _ {2}}{B _ {1}} = 1 0 6. 0 5 \\ \tilde {S} _ {1 2} ^ {1} & = & S ^ {1} \frac {B _ {2}}{B _ {1}} = 9 5. 9 5 \\ \tilde {S} _ {0 1} & = & S \frac {B _ {1}}{B _ {0}} = 1 0 1 \end{array}
$$

We can then calculate the probabilities 

$$
p _ {*} ^ {0 0} = \frac {\tilde {S} _ {1 2} ^ {0} - S ^ {0 1}}{S ^ {0 0} - S ^ {0 1}} = . 6 7 5,
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/6e242fb4b3c2fbe616890df3406f5570f1b8006480d940713c6f3f875bda3df5.jpg)



Figure C.3: The two-period Stock Market with risk-neutral probabilities.


etc., which gives the risk-neutral tree shown in figure C.3. Using this system, it is easy to calculate the price of any derivative from the formula 

$$
f = \frac {B}{B _ {2}} E ^ {*} [ f _ {2} ]
$$

We consider each of the derivatives in turn, expressing the payof as a vector of the form $( f ^ { 0 0 } , f ^ { 0 1 } , f ^ { 1 0 } , f ^ { 1 1 } )$ 

(a) If $f ^ { i j } = S ^ { i j }$ , then the payof vector is (108,102,98,92), and hence the derivative price is 

$$
f = \frac {1 0 0}{1 0 2 . 0 1} [. 6 (. 6 7 5 \times 1 0 8 +. 3 2 5 \times 1 0 2) +. 4 (. 6 5 8 3 \times 9 8 +. 3 4 1 6 \times 9 2) ] = 1 0 0,
$$

as expected. 

(b) If we take a future contract with a strike of 100, then the payof is (8,2,-2,-8), and the price is 1.97. 

(c) The European call option has payof (8,2,0,0) and costs 3.29. 

(d) The put option pays out (0,0,2,8) and has price 1.58. 

(e) In order to calculate the value of the call option, $f ,$ we need to know the value of the future at $t = 1 , \ \tilde { f } _ { 1 }$ . We can calculate this using the martingale property 

$$
\tilde {f} _ {1} = \frac {B _ {1}}{B _ {2}} E _ {1} ^ {*} [ \tilde {f} _ {2} ]
$$

which yields $\tilde { f } ^ { 0 } = 5 . 9 9$ and $\tilde { f } ^ { 1 } = - 4 . 0 1$ . Since the strike price is 3, the payof vector is $( f ^ { 0 } , f ^ { 1 } ) = ( 2 . 9 9 , 0 )$ . Hence, calculating the value of the option, we get 1.78. 

(f) The derivative has payof (0,0,2,7), and hence has price 1.45. 

(g) The digital payof is (10,10,0,0), and thus the value is 5.88. 

(h) A European call option has payout $( 4 , 0 , 0 , 0 )$ , and hence a price of 1.59. For the American option, we can price it by assuming that the investor always makes the best move possible. Thus, the payof vector is $( 4 , 1 . 0 1 , 0 , 0 )$ , corresponding to exercising the option at $t = 2 ,$ , and $t = 1$ for the first two cases. Note that if the option is exercised at $t = 1$ , then the payof can be invested in the money market account, and hence is worth 1.01, not 1 at $t = 2$ . Using this payof function, the American option is valued at 1.78. 

4. We want to calculate the risk-neutral probabilities for a three-period model. First of all let us define the forward prices that we are going to use: 

$$
\tilde {S} _ {0 1} = \frac {B _ {1}}{B _ {0}} S \quad \tilde {S} _ {1 2} ^ {i} = \frac {B _ {2}}{B _ {1}} S ^ {i} \quad \mathrm{and} \quad \tilde {S} _ {2 3} ^ {i j} = \frac {B _ {3}}{B _ {2}} S ^ {i j}.\tag{C.59}
$$

The probabilities at the first time step are 

$$
p _ {*} ^ {0} = \frac {\tilde {S} _ {0 1} - S ^ {1}}{S ^ {0} - S ^ {1}} \quad \mathrm{and} \quad p _ {*} ^ {1} = \frac {S ^ {0} - \tilde {S} _ {0 1}}{S ^ {0} - S ^ {1}}.\tag{C.60}
$$

At the second time setp, 

$$
\hat {p} _ {*} ^ {i 0} = \frac {\tilde {S} _ {1 2} ^ {i} - S ^ {i 1}}{S ^ {i 0} - S ^ {i 1}} \quad \mathrm{and} \quad p _ {*} ^ {i 1} = \frac {S ^ {i 0} - \tilde {S} _ {1 2} ^ {i}}{S ^ {i 0} - S ^ {i 1}}.\tag{C.61}
$$

At the third time step 

$$
\hat {p} _ {*} ^ {i j 0} = \frac {\tilde {S} _ {2 3} ^ {i j} - S ^ {i j 1}}{S ^ {i j 0} - S ^ {i j 1}} \quad \text {and} \quad p _ {*} ^ {i j 1} = \frac {S ^ {i j 0} - \tilde {S} _ {2 3} ^ {i j}}{S ^ {i j 0} - S ^ {i j 1}}.\tag{C.62}
$$

5. Suppose that at time 2 we are at a node $S ^ { i j }$ . Then by the one period approach we obtain the price of the derivative at the node as 

$$
f ^ {i j} = \frac {B _ {2}}{B _ {3}} (\hat {p} _ {*} ^ {i j 0} f ^ {i j 0} + \hat {p} _ {*} ^ {i j 1} f ^ {i j 1})\tag{C.63}
$$

Multiply by $p _ { * } ^ { i j }$ to remove the conditional probabilities from the right hand side, 

$$
p _ {*} ^ {i j} f ^ {i j} = \frac {B _ {2}}{B _ {3}} (p _ {*} ^ {i j 0} f ^ {i j 0} + p _ {*} ^ {i j 1} f ^ {i j 1})\tag{C.64}
$$

Sum over all possible values of i and $j .$ . This is simply taking the expectation of both sides, 

$$
E ^ {*} [ f _ {2} ] = \frac {B _ {2}}{B _ {3}} E ^ {*} [ f _ {3} ].\tag{C.65}
$$

We can then use our two-period result to write 

$$
f _ {0} = \frac {B _ {0}}{B _ {3}} E ^ {*} [ f _ {3} ].\tag{C.66}
$$

6. Consider the stock process at time $N - 1$ . We can write an arbitrary node as $S ^ { i _ { 1 } \cdots i _ { N - 1 } }$ , which will move to either $S ^ { i _ { 1 } \cdots i _ { N - 1 } 0 } \mathrm { o r } S ^ { i _ { 1 } \cdots i _ { N - 1 } 1 }$ . The bond process will move from $B _ { N - 1 }$ to $B _ { N }$ . The derivative will pay either $f ^ { i _ { 1 } \cdots i _ { N - 1 } 0 } \mathrm { o r } ^ { \mathbf { \bar { \alpha } } } f ^ { i _ { 1 } \cdots i _ { N - 1 } 1 }$ Using the standard one-period argument, we find that the value of the derivative at time $N - 1$ is 

$$
f ^ {i _ {1} \dots i _ {N - 1}} \frac {B _ {N}}{B _ {N - 1}} = \hat {p} ^ {i _ {1} \dots i _ {N - 1} 0} f ^ {1 _ {1} \dots i _ {N - 1} 0} + \hat {p} ^ {i _ {1} \dots i _ {N - 1} 1} f ^ {1 _ {1} \dots i _ {N - 1} 1}\tag{C.67}
$$

Multiply through by $p _ { * } ^ { i _ { 1 } \cdots i _ { N - 1 } }$ ， 

$$
p _ {*} ^ {i _ {1} \dots i _ {N - 1}} f ^ {i _ {1} \dots i _ {N - 1}} \frac {B _ {N}}{B _ {N - 1}} = p _ {*} ^ {i _ {1} \dots i _ {N - 1}} \hat {p} ^ {i _ {1} \dots i _ {N - 1} 0} f ^ {1 _ {1} \dots i _ {N - 1} 0} + p _ {*} ^ {i _ {1} \dots i _ {N - 1}} \hat {p} ^ {i _ {1} \dots i _ {N - 1} 1} f ^ {1 _ {1} \dots i _ {N - 1} 1}.\tag{C.68}
$$

But we can convert the conditional probabilities on the rigth hand side into unconditional probabilities 

$$
p _ {*} ^ {i _ {1} \dots i _ {N - 1}} f ^ {i _ {1} \dots i _ {N - 1}} \frac {B _ {N}}{B _ {N - 1}} = p ^ {i _ {1} \dots i _ {N - 1} 0} f ^ {1 _ {1} \dots i _ {N - 1} 0} + p ^ {i _ {1} \dots i _ {N - 1} 1} f ^ {1 _ {1} \dots i _ {N - 1} 1}.\tag{C.69}
$$

We then want to sum over all the possible values of $i _ { 1 } \cdots i _ { N - 1 }$ . This is equivalent to taking expectations of both sides, 

$$
E ^ {*} [ f _ {N - 1} ] \frac {B _ {N}}{B _ {N - 1}} = E ^ {*} [ f _ {N} ].\tag{C.70}
$$

By the induction hypothesis, 

$$
f _ {0} = E ^ {*} [ f _ {N - 1} ] \frac {B _ {0}}{B _ {N - 1}}\tag{C.71}
$$

and hence 

$$
f _ {0} = E ^ {*} [ f _ {N} ] \frac {B _ {0}}{B _ {N}}\tag{C.72}
$$

as desired. 

## Section 8

1. Working in a filtered probability system $( \Omega , \Sigma , P , { \mathcal { F } } )$ , we want to verify that the stochastic process 

$$
Y _ {m} (\omega_ {i}) = E [ S _ {n} | F _ {k} ^ {(m)} ],\tag{C.73}
$$

where $F _ { k } ^ { ( m ) }$ is the unique element of the filtration at time m that contains $\omega _ { i } ,$ is adapted to the filtration ${ \mathcal F } .$ . Note that we are being slightly more general by using $S _ { n }$ in the definition of $Y _ { m }$ instead of $S _ { 2 }$ . Recall that a process $\overset  { Y }$ is adapted, if at every time step m, $Y _ { m }$ has the same value for all the elements that are in the same set $F _ { k } ^ { ( m ) }$ of the partition of the sample space that is defined by the filtration element $\mathcal { F } _ { m }$ . So suppose $\omega _ { i }$ and $\omega _ { j }$ are both elements of $F _ { k } ^ { ( m ) }$ . Then by definiton, 

$$
Y _ {m} (\omega_ {i}) = E [ S _ {n} | F _ {k} ^ {(m)} ] \quad \text { and } \quad Y _ {m} (\omega_ {j}) = E [ S _ {n} | F _ {k} ^ {(m)} ],\tag{C.74}
$$

and hence Y is adapted to the filtration ${ \mathcal F } .$ 

2. We want to verify that the martingale condition 

$$
\frac {S _ {m}}{B _ {m}} = E ^ {*} \left[ \frac {S _ {n}}{B _ {n}} \right]\tag{C.75}
$$

holds for the three period binomial model. Since the expectation is with respect to the risk-neutral measure we need to calculate the relevant probabilities $\hat { p } _ { * } ^ { i } , \hat { p } _ { * } ^ { i j }$ and $\hat { p } _ { * } ^ { i j k }$ . Fortunately we have already done this in exercise 7.4. We begin by verifying the result for adjacent time steps. At the first time step we have 

$$
\begin{array}{r c l} E _ {0} \left[ \frac {S _ {1}}{B _ {1}} \right] & = & E \left[ \frac {S _ {1}}{B _ {1}} | F _ {0} \right] \\ & = & \frac {\hat {p} ^ {0} S ^ {0} + \hat {p} ^ {1} S ^ {1}}{B _ {1}} \\ & = & \frac {(\tilde {S} - S ^ {1}) S ^ {0} + (S ^ {0} - \tilde {S}) S ^ {1}}{B _ {1} (S ^ {0} - S ^ {1})} \\ & = & \frac {\tilde {S}}{B _ {1}} \\ & = & \frac {S}{B _ {0}}. \end{array}\tag{C.76}
$$

Between the first and second time steps, 

$$
\begin{array}{l l l} E _ {1} \left[ \frac {S _ {2}}{B _ {2}} \right] & = & E \left[ \frac {S _ {2}}{B _ {2}} | F ^ {i} \right] \\ & = & \frac {\hat {p} ^ {i 0} S ^ {i 0} + \hat {p} ^ {i 1} S ^ {i 1}}{B _ {2}} \\ & = & \frac {(\tilde {S} ^ {i} - S ^ {i 1}) S ^ {i 0} + (S ^ {i 0} - \tilde {S} ^ {i}) S ^ {i 1}}{B _ {2} (S ^ {i 0} - S ^ {i 1})} \\ & = & \frac {\tilde {S} ^ {i}}{B _ {2}} \\ & = & \frac {S ^ {i}}{B _ {1}}. \end{array}\tag{C.77}
$$

Finally, consider when we move from the second to third node, 

$$
\begin{array}{r c l} E _ {2} \left[ \frac {S _ {3}}{B _ {3}} \right] & = & E \left[ \frac {S _ {3}}{B _ {3}} | F ^ {i j} \right] \\ & = & \frac {\hat {p} ^ {i j 0} S ^ {i j 0} + \hat {p} ^ {i j 1} S ^ {i j 1}}{B _ {3}} \\ & = & \frac {(\tilde {S} ^ {i j} - S ^ {i j 1}) S ^ {i j 0} + (S ^ {i j 0} - \tilde {S} ^ {i j}) S ^ {i j 1}}{B _ {3} (S ^ {i j 0} - S ^ {i j 1})} \\ & = & \frac {\tilde {S} ^ {i j}}{B _ {3}} \\ & = & \frac {S ^ {i j}}{B _ {2}}. \end{array}\tag{C.78}
$$

We can verify the other cases by using a very important result: 

$$
E _ {i} [ X _ {n} ] = E _ {i} [ E _ {j} [ X _ {n} ].\tag{C.79}
$$

This is known as the tower law of conditional expectation. Rather than prove it, we will verify it for a specific example. Consider the random variable $E _ { 1 } [ S _ { 3 } ^ { \mathsf { ^ { - } } } ]$ , which is the expected value of the share price at time 3, given that we have information about what happened at time 1. Evaluate it at a particular element of the sample space, say $U D ^ { \dagger } { \dot { U } }$ 

$$
\begin{array}{r c l} E _ {1} [ S _ {3} ] (U D U) & = & E [ S _ {3} | F ^ {0} ] \\ & = & P (U U U | F ^ {0}) S ^ {0 0 0} + P (U U D | F ^ {0}) S ^ {0 0 1} \\ & & + P (U D U | F ^ {0}) S ^ {0 1 0} P (U D D | F ^ {0}) S ^ {0 1 1}. \end{array}\tag{C.80}
$$

Now consider the random variable $E _ { 1 } [ E _ { 2 } [ S _ { 3 } ] ]$ . We want to evaluate it at the same point and verify that we get the same result as above. Hence 

$$
\begin{array}{r c l} E _ {1} [ E _ {2} [ S _ {3} ] ] (U D U) & = & E [ E _ {2} [ S _ {3} ] | F ^ {0} ] \\ = & & P (U U U | F ^ {0}) E [ S _ {3} | F ^ {0 0} ] + P (U U D | F ^ {0}) E [ S _ {3} | F ^ {0 0} ] \\ & + & + P (U D U | F ^ {0}) E [ S _ {3} | F ^ {0 1} ] + P (U D D | F ^ {0}) E [ S _ {3} | F ^ {0 1} ] \\ = & & \{P (U U U | F ^ {0}) + P (U U D | F ^ {0}) \} \\ & \times & \{P (U U U | F ^ {0 0}) S ^ {0 0 0} + P (U U D | F ^ {0 0}) S ^ {0 0 1} \} \\ & + & \{P (U D U | F ^ {0}) + P (U D D | F ^ {0}) \} \\ & \times & \{P (U D U | F ^ {0 1}) S ^ {0 1 0} + P (U D D | F ^ {0 1}) S ^ {0 1 1} \}. \end{array} \tag {C}\tag{C.81}
$$

Collecting terms that have the same value of $S _ { 3 }$ , we have 

$$
\begin{array}{r c l} E _ {1} [ E _ {2} [ S _ {3} ] ] (U D U) & = & \{P (U U U | F ^ {0}) + P (U U D | F ^ {0}) \} P (U U U | F ^ {0 0}) S ^ {0 0 0} \\ & + & \{P (U U U | F ^ {0}) + P (U U D | F ^ {0}) \} P (U U D | F ^ {0 0}) S ^ {0 0 1} \\ & + & \{P (U D U | F ^ {0}) + P (U D D | F ^ {0}) \} P (U D U | F ^ {0 1}) S ^ {0 1 0} \\ & + & \{P (U D U | F ^ {0}) + P (U D D | F ^ {0}) \} P (U D D | F ^ {0 1}) S ^ {0 1} \text {(C.82)} \end{array}
$$

We then note that $P ( U U U | F ^ { 0 } ) + P ( U U D | F ^ { 0 } ) = P ( F ^ { 0 0 } | F ^ { 0 } )$ , and similarly $P ( U D U | F ^ { 0 } ) +$ $P ( U D D | F ^ { 0 } ) = P ( F ^ { 0 1 } | F ^ { 0 } )$ , so 

$$
\begin{array}{r c l} E _ {1} [ E _ {2} [ S _ {3} ] ] (U D U) & = & P (F ^ {0 0} | F ^ {0}) P (U U U | F ^ {0 0}) S ^ {0 0 0} \\ & + & P (F ^ {0 0} | F ^ {0}) P (U U D | F ^ {0 0}) S ^ {0 0 1} \\ & + & P (F ^ {0 1} | F ^ {0}) P (U D U | F ^ {0 1}) S ^ {0 1 0} \\ & + & P (F ^ {0 1} | F ^ {0}) P (U D D | F ^ {0 1}) S ^ {0 1 1}. \end{array}\tag{C.83}
$$

But then $P ( F ^ { 0 0 } | F ^ { 0 } ) P ( U U U | F ^ { 0 } ) = P ( U U U | F ^ { 0 } )$ , and so on, which simplifies our result to 

$$
\begin{array}{r c l} E _ {1} [ E _ {2} [ S _ {3} ] ] (U D U) & = & P (U U U | F ^ {0}) S ^ {0 0 0} + P (U U D | F ^ {0}) S ^ {0 0 1} \\ & + & P (U D U | F ^ {0}) S ^ {0 1 0} + P (U D D | F ^ {0}) S ^ {0 1 1} \\ & = & E _ {1} [ S _ {3} ] (U D U), \end{array}\tag{C.84}
$$

which is what we wanted to prove. 

We can then use the tower law to evaluate the other conditional expectations. For example, 

$$
E _ {0} \left[ \frac {S _ {2}}{B _ {2}} \right] = E _ {0} \left[ E _ {1} \left[ \frac {S _ {2}}{B _ {2}} \right] \right].\tag{C.85}
$$

But, we have already evaluated the single time-step conditional expectations, and hence 

$$
E _ {0} \left[ \frac {S _ {2}}{B _ {2}} \right] = E _ {0} \left[ \frac {S _ {1}}{B _ {1}} \right].\tag{C.86}
$$

Once again, we have already calculated this result, and so we see that 

$$
E _ {0} \left[ \frac {S _ {2}}{B _ {2}} \right] = \frac {S _ {0}}{B _ {0}}.\tag{C.87}
$$

Similarly we see that 

$$
\begin{array}{r c l} E _ {0} \left[ \frac {S _ {3}}{B _ {3}} \right] & = & E _ {0} \left[ E _ {2} \left[ \frac {S _ {3}}{B _ {3}} \right] \right] \\ & = & E _ {0} \left[ \frac {S _ {2}}{B _ {2}} \right] \\ & = & \frac {S _ {0}}{B _ {0}}. \end{array}\tag{C.88}
$$

Finally, we also have 

$$
\begin{array}{r c l} E _ {1} \left[ \frac {S _ {3}}{B _ {3}} \right] & = & E _ {1} \left[ E _ {2} \left[ \frac {S _ {3}}{B _ {3}} \right] \right] \\ & = & E _ {1} \left[ \frac {S _ {2}}{B _ {2}} \right] \\ & = & \frac {S _ {1}}{B _ {1}}. \end{array}\tag{C.89}
$$

## Section 9

1. We need to show that the number of ways of arriving at the node $S _ { i } ^ { n }$ is $C _ { i } ^ { n }$ . The node $S _ { i } ^ { n }$ is a combination of i ‘down’ movements and $n - i \cdot \mathrm { u p } ^ { \prime }$ movements. Hence we can view the problem as being the number of ways of placing i identical objects (the down movements) in $n$ ordered positions (the total number of time steps). The number of ways of placing n distinct objects in n locations is n!. However, this overcounts the number of ‘up’ movements by a factor of $( n - i ) !$ , since they are indistinguishable, and overcounts the ‘down’ movements by a factor $i ! .$ Hence the total number of distinct combinations is $n ! / [ i ! ( n - i ) ! ]$ , which is simply $C _ { i } ^ { n }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/11181fb9-8e49-4404-8b18-b8f89ef75afd/c1e20e4412b2dd0bdaad820ed9519796321fca207f91bda62769ab67a7f7586f.jpg)



Figure C.4: The share prices for the lattice model.


2. We want to verify that the risk-neutral probabilities for the binomial lattice are consistent with the risk-neutral probabilities derived earlier for the non-recombining tree, 

$$
p _ {*} ^ {0} = \frac {\tilde {S} - S ^ {1}}{S ^ {0} - S ^ {1}} \quad \mathrm{and} \quad p _ {*} ^ {1} = \frac {S ^ {0} - \tilde {S}}{S ^ {0} - S ^ {1}}.\tag{C.90}
$$

Setting $S ^ { 0 } = u S _ { 0 } , S ^ { 1 } = d S _ { 0 }$ and $\tilde { S } = e ^ { r } S _ { 0 }$ we see that 

$$
\begin{array}{r c l} {p _ {*} ^ {0}} & = & {\frac {e ^ {r} S _ {0} - d S _ {0}}{u S _ {0} - d S _ {0}}} \\ & = & {\frac {e ^ {r} - d}{u - d},} \end{array}\tag{C.91}
$$

(C.92) 

which is the probability $p _ { * }$ obtained for the lattice model. By conservation of probability we must also have $p _ { * } ^ { 1 } = q _ { * }$ 

3. Consider a market with $S _ { 0 } = \ S 1 0 0 , p = 0 . 6 , e ^ { r } = 1 . 0 1 , u = 1 . 0 5$ and $d = 0 . 9 5$ . The lattice of share prices is given in figure C.4. The risk neutral probability p can be calculated as 

$$
\begin{array}{r c l} p _ {*} & = & \frac {e ^ {r} - d}{u - d} \\ & = & \frac {1 . 0 1 - 0 . 9 5}{1 . 0 5 - 0 . 9 5} \\ & = & 0. 6. \end{array}\tag{C.93}
$$

We now want to price a call option with a strike of $100. The initial price $f _ { 0 }$ of any derivative is given by the binomial pricing formula 

$$
f _ {0} = e ^ {- r n} \sum_ {i = 0} ^ {n} C _ {i} ^ {n} p _ {*} ^ {n - i} q _ {*} ^ {i} f _ {n} ^ {i},\tag{C.94}
$$

where in the case of our call option the payof function $f _ { n } ^ { i } = S _ { n } ^ { i } - \mathbb { S } 1 0 0$ . Substituting in the share prices, we have 

$$
f _ {3} ^ {0} = 1 5. 7 6 \quad f _ {3} ^ {1} = 4. 7 4 \quad f _ {3} ^ {2} = 0 \quad \text { and } \quad f _ {3} ^ {3} = 0\tag{C.95}
$$

The pricing formula then yields an initial cost for the call option of 

$$
\begin{array}{r c l} f _ {0} & = & \frac {(1) (0 . 6) ^ {3} (0 . 4) ^ {0} (1 5 . 7 6) + (3) (0 . 6) ^ {2} (0 . 4) ^ {1} (4 . 7 4)}{(1 . 0 1) ^ {3}} \\ & = & 5. 2 9 \end{array}\tag{C.96}
$$

## Section 11

1. For now, we will assume that $W _ { a + b } - W _ { b }$ is normally distributed and merely calculate its mean and variance. The calculation of the expectation is trivial, 

$$
\begin{array}{r c l} E [ W _ {a + b} - W a ] & = & E [ W _ {a + b} ] - E [ W _ {a} ] \\ & = & 0, \end{array}\tag{C.97}
$$

where we have used the fact that the expectation of a Brownian motion $W _ { t }$ at any time t is 0. The variance calculation is slightly more complicated, but not much. We see that 

$$
\begin{array}{r c l} {E [ (W _ {a + b} - W _ {a}) ^ {2} ]} & = & {E [ W _ {a + b} ^ {2} - 2 W _ {a + b} W _ {a} + W _ {a} ^ {2} ]} \\ & = & {E [ W _ {a + b} ^ {2} ] - 2 E [ W _ {a + b} W _ {a} ] + E [ W _ {a} ^ {2} ]} \\ & = & {a + b - 2 E [ W _ {a + b} W _ {a} ] + a,} \end{array}\tag{C.98}
$$

where we took advantage of the fact that the variance of $W _ { t }$ is t. But what about the term $E [ W _ { a + b } W _ { a } ] ?$ The two random variables $W _ { a + b }$ and $W _ { a }$ are not independent, so we cannot factor the term into $E [ W _ { a + b } ] E [ W _ { a } ]$ . So how do we evaluate it? Well, we make use of a common trick for generating independent variables. Write $W _ { a + b } = ( W _ { a + b } - W _ { a } ) + W _ { a }$ . We then have 

$$
\begin{array}{r c l} E [ (W _ {a + b} - W _ {a}) ^ {2} ] & = & 2 a + b - 2 E [ \{(W _ {a + b} - W _ {a}) + W _ {a} \} W _ {a} ] \\ & = & 2 a + b - 2 E [ (W _ {a + b} - W _ {a}) W _ {a} ] \\ & & - 2 E [ W _ {a} ^ {2} ]. \end{array}\tag{C.99}
$$

But now we can make use of the fact that $\left( W _ { a + b } - W _ { a } \right)$ and $W _ { a }$ are independent random variables, and hence 

$$
\begin{array}{r c l} E [ (W _ {a + b} - W _ {a}) ^ {2} ] & = & 2 a + b - 2 E [ W _ {a + b} - W _ {a} ] E [ W _ {a} ] - 2 E [ W _ {a} ^ {2} ] \\ & = & 2 a + b - 0 - 2 a \\ & = & b. \end{array}\tag{C.100}
$$

Thus we see that $W _ { a + b } - W _ { a }$ has a mean of zero and a variance of b. 

2. We want to calculate the variance of the asset price process $S _ { t } .$ , which has a time evolution governed by equation (11.1), 

$$
S _ {t} = S _ {0} e ^ {\mu t - \frac {1}{2} \sigma^ {2} t + \sigma W _ {t}}.\tag{C.101}
$$

We already demonstrated in equation (11.10) that the expectation of the asset price is 

$$
E [ S _ {t} ] = S _ {0} e ^ {\mu t}.\tag{C.102}
$$

In order to obtain the variance, we first need to calculate the expectation of the square of the asset price, 

$$
\begin{array}{r c l} {E [ S _ {t} ^ {2} ]} & = & {E \left[ S _ {0} ^ {2} e ^ {2 \mu t - \sigma^ {2} t + 2 \sigma W _ {t}} \right]} \\ & = & {S _ {0} ^ {2} e ^ {2 \mu t - \sigma^ {2} t} E \left[ e ^ {2 \sigma W _ {t}} \right].} \end{array}\tag{C.103}
$$

Since $W _ { t }$ is an $\mathrm { N } ( 0 , t )$ random variable, we can use the result of lemma (11.1) to evaluate the expectation, 

$$
\begin{array}{r c l} {E [ S _ {t} ^ {2} ]} & = & {S _ {0} ^ {2} e ^ {2 \mu t - \sigma^ {2} t} e ^ {2 \sigma^ {2} t}} \\ & = & {S _ {0} ^ {2} e ^ {2 \mu t + \sigma^ {2} t}.} \end{array}\tag{C.104}
$$

Hence we can calculate the variance as 

$$
\begin{array}{r c l} {V [ S _ {t} ]} & = & {E [ S _ {t} ^ {2} ] - E [ S _ {t} ] ^ {2}} \\ & = & {S _ {0} ^ {2} e ^ {2 \mu t + \sigma^ {2} t} - S _ {0} ^ {2} e ^ {2 \mu t}} \\ & = & {S _ {0} ^ {2} e ^ {2 \mu t} (e ^ {\sigma^ {2} t} - 1).} \end{array}\tag{C.105}
$$

3. We want to calculate the first four moments for an $\mathrm { N } ( m , V )$ random variable. To begin with, we will calculate the first four moments of the ‘standard normal distribution’, $\mathrm { { N } } \dot { ( 0 , 1 ) }$ . Note that by symmetry any odd moments vanish. We can then calculate the zeroth moment (which must be 1 by conservation of probability) by using a well-known change of coordinates. We begin by considering the square of the integral, 

$$
\begin{array}{r c l} {I ^ {2}} & = & {\left[ \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} e ^ {- u ^ {2} / 2} d u \right] ^ {2}} \\ & = & {\frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} e ^ {- x ^ {2} / 2} d x \int_ {- \infty} ^ {\infty} e ^ {- y ^ {2} / 2} d y} \\ & = & {\frac {1}{2 \pi} \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} e ^ {- (x ^ {2} + y ^ {2}) / 2} d y d x} \end{array}\tag{C.106}
$$

We then want to change to polar coordinates r and $\theta$ 

$$
\begin{array}{r c l} {I ^ {2}} & = & {\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} \int_ {0} ^ {\infty} e ^ {- r ^ {2} / 2} r d r d \theta} \\ & = & {\int_ {0} ^ {\infty} e ^ {- r ^ {2} / 2} r d r} \end{array}\tag{C.107}
$$

Making the variable substitution $v = r ^ { 2 } / 2$ we obtain 

$$
\begin{array}{r c l} I ^ {2} & = & \int_ {0} ^ {\infty} e ^ {- v} d v \\ & = & 1, \end{array}\tag{C.108}
$$

so that I is indeed equal to 1. We can then obtain the other moments by using integration by parts. For example, 

$$
\begin{array}{r c l} \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} x ^ {2} e ^ {- x ^ {2} / 2} & = & \left. \frac {- x e ^ {- x ^ {2} / 2}}{\sqrt {2 \pi}} \right| _ {- \infty} ^ {\infty} + \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} e ^ {- x ^ {2} / 2} d x \\ & = & 1. \end{array}\tag{C.109}
$$

For the fourth moment, we have 

$$
\begin{array}{r c l} \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} x ^ {4} e ^ {- x ^ {2} / 2} & = & \frac {- x ^ {3} e ^ {- x ^ {2} / 2}}{\sqrt {2 \pi}} \bigg | _ {- \infty} ^ {\infty} + \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} 3 x ^ {2} e ^ {- x ^ {2} / 2} d x \\ & = & 3. \end{array}\tag{C.110}
$$

Using these results, we can then derive the moments for an $\mathrm { N } ( m , V )$ random variable, 

$$
E [ X ^ {n} ] = \frac {1}{\sqrt {2 \pi V}} \int_ {x = - \infty} ^ {x = \infty} x ^ {n} e ^ {- \frac {(x - m) ^ {2}}{2 V}} d x.
$$

Making the variable substitution $u = ( x - m ) / \sqrt { V }$ , we have 

$$
E [ X ^ {n} ] = \frac {1}{\sqrt {2 \pi}} \int_ {u = - \infty} ^ {u = \infty} (\sqrt {V} u + m) ^ {n} e ^ {- \frac {u ^ {2}}{2}} d u.
$$

Expanding the binomial term, 

$$
E [ X ^ {n} ] = \sum_ {k = 0} ^ {n} \left( \begin{array}{c c} n \\ k \end{array} \right) \frac {V ^ {k / 2} m ^ {n - k}}{\sqrt {2 \pi}} \int_ {u = - \infty} ^ {u = \infty} u ^ {k} e ^ {- \frac {u ^ {2}}{2}} d u.
$$

The integral is now in terms of the moments of an $\mathrm { { N } } ( 0 , 1 )$ variable, and hence we can find the values 

$$
E [ X ] = m\tag{C.111}
$$

$$
E [ X ^ {2} ] = m ^ {2} + V\tag{C.112}
$$

$$
{E [ X ^ {3} ]} = {m ^ {3} + 3 m V}\tag{C.113}
$$

$$
{E [ X ^ {4} ]} = {m ^ {4} + 6 m ^ {2} V + 3 V ^ {2}.}\tag{C.114}
$$

4. We want to calculate $E [ e ^ { \alpha X } ]$ and $V [ e ^ { \alpha X } ]$ for an $\mathrm { N } ( m , V )$ random variable X. We already calculated the expectation of $e ^ { \alpha \bar { X } }$ in lemma 11.1, 

$$
E [ e ^ {\alpha X} ] = e ^ {\alpha m + \frac {1}{2} \alpha^ {2} V}.\tag{C.115}
$$

In order to obtain the variance, we need to consider the expectation of $( e ^ { \alpha X } ) ^ { 2 } =$ $e ^ { 2 \alpha X }$ . This is easy to evaluate, again by using lemma 11.1, 

$$
E [ e ^ {2 \alpha X} ] = e ^ {2 \alpha m + 2 \alpha^ {2} V}.\tag{C.116}
$$

Hence the variance is 

$$
\begin{array}{r c l} V [ e ^ {\alpha X} ] & = & E [ e ^ {2 \alpha X} ] - E [ e ^ {\alpha X} ] ^ {2} \\ & = & e ^ {2 \alpha m + 2 \alpha^ {2} V} - e ^ {2 \alpha m + \alpha^ {2} V} \\ & = & e ^ {2 \alpha m + 2 \alpha^ {2} V} (1 - e ^ {- \alpha^ {2} V}). \end{array}\tag{C.117}
$$

5. We want to show that $M _ { t } ( W _ { t } ) = e ^ { \alpha W _ { t } - \frac { 1 } { 2 } \alpha ^ { 2 } t }$ is a martingale, that is, $E _ { s } [ M _ { t } ] = M _ { s }$ The simplest way to do this is to rewrite $M _ { t }$ in terms of random variables that are independent of the conditioning at time s. That is, write 

$$
M _ {t} = e ^ {\alpha (W _ {t} - W _ {s}) + \alpha W _ {s} - \frac {1}{2} \alpha^ {2} t},\tag{C.118}
$$

which is a function of the $\mathrm { N } ( 0 , t - s )$ random variable $( W _ { t } - W _ { s } )$ and the constant $W _ { s }$ . Note that $( W _ { t } \mathrm { ~ - ~ } W _ { s } )$ is independent of any conditioning at time s because of the independent increments property of Brownian motion, while $W _ { s }$ is fixed by the fact that we know what actually happens at time s—this is what a conditional expectation means. Thus we can calculate the conditional expectation of $M _ { t }$ by integrating (C.118) over the probability distribution for $\left( W _ { t } - \tilde { W } _ { s } \right)$ and treating $\check { W _ { s } }$ as a constant, 

$$
\begin{array}{r c l} E _ {s} [ M _ {t} ] & = & \int_ {- \infty} ^ {\infty} \exp \left[ \alpha x + \alpha W _ {s} - \frac {1}{2} \alpha^ {2} t \right] \frac {1}{\sqrt {2 \pi (t - s)}} \exp \left[ \frac {- x ^ {2}}{2 (t - s)} \right] d x \\ & = & \frac {1}{\sqrt {t - s}} \exp \left[ \alpha W _ {s} - \frac {1}{2} \alpha^ {2} t \right] \\ & & \times \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \exp \left[ - \frac {x ^ {2}}{2 (t - s)} + \alpha x \right] d x. \end{array} \tag {C}\tag{C.119}
$$

We then want to use the result, which is not dificult to prove, that 

$$
{\frac {1}{\sqrt {2 \pi}}} \int_ {- \infty} ^ {\infty} \exp \left[ - \frac {1}{2} a x ^ {2} + b x + c \right] d x = \frac {1}{\sqrt {a}} \exp \left[ \frac {b ^ {2}}{2 a} + c \right].\tag{C.120}
$$

In our case we have 

$$
a = \frac {1}{t - s}, \quad b = \alpha , \quad \mathrm{and} \quad c = 0,\tag{C.121}
$$

and hence 

$$
\begin{array}{r c l} E _ {s} [ M _ {t} ] & = & \frac {1}{\sqrt {t - s}} \exp \left[ \alpha W _ {s} - \frac {1}{2} \alpha^ {2} t \right] \sqrt {t - s} \exp \left[ - \frac {1}{2} \alpha^ {2} (t - s) \right] \\ & = & \exp \left[ \alpha W _ {s} - \frac {1}{2} \alpha^ {2} s \right] \\ & = & M _ {s}, \end{array}\tag{C.122}
$$

so $M _ { t }$ is a martingale. 

6. We want to show that $N _ { t } = \cos ( \beta W _ { t } ) e ^ { \frac { 1 } { 2 } \beta ^ { 2 } t }$ is a martingale, that is, $E _ { s } [ N _ { t } ] = N _ { s }$ Begin by rewriting $N _ { t }$ as the real part of a complex function, 

$$
\begin{array}{r c l} N _ {t} & = & \cos (\beta W _ {t}) e ^ {\frac {1}{2} \beta^ {2} t} \\ & = & \Re \exp \left[ i \beta W _ {t} + \frac {1}{2} \beta^ {2} t \right]. \end{array}\tag{C.123}
$$

If we then set $\beta = - i \alpha$ , we obtain 

$$
\begin{array}{r c l} N _ {t} & = & \Re \exp \left[ \alpha W _ {t} - \frac {1}{2} \alpha^ {2} t \right] \\ & = & \Re M _ {t}, \end{array}\tag{C.124}
$$

where we have substituted in the martingale process $M _ { t }$ considered in the previous question. Taking expectations then yields 

$$
\begin{array}{r c l} E _ {s} [ N _ {t} ] & = & E _ {s} [ \Re M _ {t} ] \\ & = & \Re E _ {s} [ M _ {t} ] \\ & = & \Re M _ {s} \\ & = & \Re \exp \left[ \alpha W _ {s} - \frac {1}{2} \alpha^ {2} s \right] \\ & = & \Re \exp \left[ i \beta W _ {s} + \frac {1}{2} \beta^ {2} s \right] \\ & = & \cos (\beta W _ {s}) \exp \left[ \frac {1}{2} \beta^ {2} s \right]. \end{array}\tag{C.125}
$$

Thus we see that the process $N _ { t }$ is indeed a martingale. 

## Section 12

1. We want to show that the Wiener model for an asset price process, with dynamics given by equation (11.1) 

$$
S _ {t} = S _ {0} \exp \left[ \left(\mu - \frac {1}{2} \sigma^ {2}\right) t + \sigma W _ {t} \right],\tag{C.126}
$$

satisfies the stochastic diferential equation (13.1), 

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma d W _ {t}.\tag{C.127}
$$

To do this we define the stochastic process 

$$
X _ {t} = \left(\mu - \frac {1}{2} \sigma^ {2}\right) t + \sigma W _ {t},\tag{C.128}
$$

which clearly satisfies the diferential equation 

$$
d X _ {t} = \left(\mu - \frac {1}{2} \sigma^ {2}\right) d t + \sigma d W _ {t}.\tag{C.129}
$$

Moreover, $\mathrm { i f }$ we square $d X _ { t }$ then we obtain 

$$
d X _ {t} ^ {2} = \sigma^ {2} d t,\tag{C.130}
$$

where we have applied the Ito calculus rules $d t ^ { 2 } = 0 , d t d W _ { t } = 0$ and $d W _ { t } ^ { 2 } = d t$ We can then consider the asset price process $S _ { t }$ as a function of a process for which we know the diferential equation, namely $X _ { t }$ . Using Ito’s lemma on the function $S _ { t } ( X _ { t } ) = S _ { 0 } e ^ { X _ { t } }$ we obtain 

$$
\begin{array}{r c l} d (S _ {t}) & = & S _ {0} d (e ^ {X _ {t}}) \\ & = & S _ {0} \left[ \frac {\partial e ^ {X _ {t}}}{\partial X _ {t}} d X _ {t} + \frac {1}{2} \frac {\partial^ {2} e ^ {X _ {t}}}{\partial X _ {t} ^ {2}} d X _ {t} ^ {2} \right] \\ & = & S _ {0} e ^ {X _ {t}} \left[ d X _ {t} + \frac {1}{2} d X _ {t} ^ {2} \right] \\ & = & S _ {t} \left[ \left(\mu - \frac {1}{2} \sigma^ {2}\right) d t + \sigma d W _ {t} + \frac {1}{2} \sigma^ {2} d t \right] \\ & = & S _ {t} [ \mu d t + \sigma d W _ {t} ]. \end{array}\tag{C.131}
$$

Thus the Wiener model asset price process $S _ { t }$ satisfies the desired diferential equation. 

2. In this exercise, we want to calculate the stochastic diferential equations for a number of stochastic processes $X _ { t }$ . We can do this by considering them as a function of both a Wiener process and time, that is $X _ { t } = \check { X _ { t } } ( W _ { t } , t )$ . Ito’s lemma then tells us that the stochastic diferential equation is 

$$
d X _ {t} = \frac {\partial X _ {t}}{\partial t} d t + \frac {\partial X _ {t}}{\partial W _ {t}} d W _ {t} + \frac {1}{2} \frac {\partial^ {2} X _ {t}}{\partial W _ {t} ^ {2}} d t,\tag{C.132}
$$

where we have set dW $\ T _ { t } ^ { 2 } = d t$ in the final term. Thus, 

(a) for the process $X _ { t } = W _ { t } ^ { 2 } - t ;$ 

$$
\begin{array}{r c l} d X _ {t} & = & - d t + 2 W _ {t} d W _ {t} + d t \\ & = & 2 W _ {t} d W _ {t}; \end{array}\tag{C.133}
$$

(b) for the process $X _ { t } = W _ { t } ^ { 3 } - 3 t W _ { t }$ ， 

$$
\begin{array}{r c l} {d W _ {t}} & = & {- 3 W _ {t} d t + (3 W _ {t} ^ {2} - 3 t) d W _ {t} + \frac {1}{2} 6 W _ {t} d t} \\ & = & {3 (W _ {t} ^ {2} - t) d W _ {t};} \end{array}\tag{C.134}
$$

(c) and for the process $X _ { t } = W _ { t } ^ { 4 } - 6 t W _ { t } ^ { 2 } + 3 t ^ { 2 }$ 

$$
\begin{array}{r c l} d X _ {t} & = & (- 6 W _ {t} ^ {2} + 6 t) d t + (4 W _ {t} ^ {3} - 1 2 t W _ {t}) d W _ {t} \\ & & + \frac {1}{2} (1 2 W _ {t} ^ {2} - 1 2 t) d t \\ & = & 4 (W _ {t} ^ {3} - 3 t W _ {t}) d W _ {t}. \end{array}\tag{C.135}
$$

3. We want to calculate the product rule $d ( X _ { t } Y _ { t } )$ for stochastic processes $X _ { t }$ and $Y _ { t } .$ Expanding the diferential as a Taylor series in $d X _ { t }$ and $d Y _ { t } ,$ and remembering to keep all terms up to the second order, we have 

$$
\begin{array}{r c l} {d (X _ {t} Y _ {t})} & = & {\frac {\partial (X _ {t} Y _ {t})}{\partial X _ {t}} d X _ {t} + \frac {\partial (X _ {t} Y _ {t})}{\partial Y _ {t}} d Y _ {t} + \frac {1}{2} \frac {\partial^ {2} (X _ {t} Y _ {t})}{\partial X _ {t} ^ {2}} d X _ {t} ^ {2}} \\ & & {+ \frac {1}{2} \frac {\partial^ {2} (X _ {t} Y _ {t})}{\partial Y _ {t} ^ {2}} d Y _ {t} ^ {2} + \frac {\partial^ {2} (X _ {t} Y _ {t})}{\partial X _ {t} \partial Y _ {t}} d X _ {t} d Y _ {t}} \\ & = & {Y _ {t} d X _ {t} + X _ {t} d Y _ {t} + d X _ {t} d Y _ {t}.} \end{array}\tag{C.136}
$$

4. We can calculate the division rule for stochastic diferentials $d ( X _ { t } / Y _ { t } )$ in a manner identical to that used for the product rule in the previous question, 

$$
\begin{array}{r c l} d (X _ {t} / Y _ {t}) & = & \frac {\partial (X _ {t} / Y _ {t})}{\partial X _ {t}} d X _ {t} + \frac {\partial (X _ {t} / Y _ {t})}{\partial Y _ {t}} d Y _ {t} + \frac {1}{2} \frac {\partial^ {2} (X _ {t} / Y _ {t})}{\partial X _ {t} ^ {2}} d X _ {t} ^ {2} \\ & & + \frac {1}{2} \frac {\partial^ {2} (X _ {t} / Y _ {t})}{\partial Y _ {t} ^ {2}} d Y _ {t} ^ {2} + \frac {\partial^ {2} (X _ {t} / Y _ {t})}{\partial X _ {t} \partial Y _ {t}} d X _ {t} d Y _ {t} \\ & = & \frac {1}{Y _ {t}} d X _ {t} - \frac {X _ {t}}{Y _ {t} ^ {2}} d Y _ {t} + \frac {X _ {t}}{Y _ {t} ^ {3}} d Y _ {t} ^ {2} - \frac {1}{Y _ {t} ^ {2}} d X _ {t} d Y _ {t} \\ & = & \frac {X _ {t}}{Y _ {t}} \left[ \frac {d X _ {t}}{X _ {t}} - \frac {d Y _ {t}}{Y _ {t}} + \frac {d Y _ {t} ^ {2}}{Y _ {t} ^ {2}} - \frac {d X _ {t} d Y _ {t}}{X _ {t} Y _ {t}} \right]. \end{array}\tag{C.137}
$$

## Section 13

1. Starting with nothing, if we take the position $V _ { t } = C _ { t } - \phi _ { t } S _ { t } - \psi _ { t } B _ { t }$ then since it has no net value, we can solve for the bond position $\psi _ { t }$ 

$$
\psi_ {t} = \frac {C _ {t}}{B _ {t}} - \phi_ {t} \frac {S _ {t}}{B _ {t}}.\tag{C.138}
$$

At time $t + d t$ the value of the portfolio has changed to 

$$
d V _ {t} = d C _ {t} - \phi_ {t} d S _ {t} - \psi_ {t} d B _ {t},\tag{C.139}
$$

where we have kept the stock and bond holdings fixed. Substituting in for the stochastic diferentials from equations (13.1), (13.2) and (13.4) we obtain 

$$
\begin{array}{r c l} d V _ {t} & = & \frac {\partial C _ {t}}{\partial t} d t + \frac {\partial C _ {t}}{\partial S _ {t}} d S _ {t} + \frac {1}{2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} d S _ {t} ^ {2} - \phi_ {t} d S _ {t} \\ & & - \left(\frac {C _ {t}}{B _ {t}} - \phi_ {t} \frac {S _ {t}}{B _ {t}}\right) r _ {t} B _ {t} d t. \end{array}\tag{C.140}
$$

Since $d S _ { t } ^ { 2 } = \sigma _ { t } ^ { 2 } S _ { t } ^ { 2 } d t$ , the only diferential that contains a random component is $d S _ { t }$ . Hence we can obtain a guaranteed return on our portfolio if we set the stock holding φ to be 

$$
\phi_ {t} = \frac {\partial C _ {t}}{\partial S _ {t}}.\tag{C.141}
$$

The fixed return is then 

$$
d V _ {t} = \left(\frac {\partial C _ {t}}{\partial t} + \frac {1}{2} \sigma_ {t} ^ {2} s _ {t} ^ {2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} - r _ {t} C _ {t} + r _ {t} S _ {t} \frac {\partial C _ {t}}{\partial S _ {t}}\right) d t.\tag{C.142}
$$

By the no arbitrage condition this must be zero, and hence we recover the Black-Scholes equation 

$$
\frac {\partial C _ {t}}{\partial t} + \frac {1}{2} \sigma_ {t} ^ {2} s _ {t} ^ {2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} - r _ {t} C _ {t} + r _ {t} S _ {t} \frac {\partial C _ {t}}{\partial S _ {t}} = 0.\tag{C.143}
$$

2. We want to value a call option for $T - t = 0 . 5 , K = 1 1 5 , S _ { t } = 1 0 0 \sigma = . 2$ and $r = 0 . 0 5$ . We find that 

$$
\begin{array}{r c l} h ^ {+} & = & - 0. 7 4 1 \\ h ^ {-} & = & - 0. 8 8 2 \\ N (h ^ {+}) & = & 0. 2 2 9 \\ N (h ^ {-}) & = & 0. 1 8 8 \end{array}\tag{C.144}
$$

and hence the call option price is $1.76. 

## Section 14

1. We want to verify that the trading strategy $( \phi _ { t } , \psi _ { t } )$ is self-financing. 

(a) We begin by calculating the stochastic diferential of the ratio of the derivative to the bond price, 

$$
\begin{array}{r c l} {d \left(\frac {C _ {t}}{B _ {t}}\right)} & = & {\frac {d C _ {t}}{B _ {t}} - \frac {C _ {t} d B _ {t}}{B _ {t} ^ {2}} - \frac {d C _ {t} d B _ {t}}{B _ {t} ^ {2}}} \\ & = & {\frac {C _ {t}}{B _ {t}} \left(\frac {d C _ {t}}{C _ {t}} - \frac {d B _ {t}}{B _ {t}}\right)} \\ & = & {\frac {C _ {t}}{B _ {t}} \left(\mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t} - r _ {t} d t\right).} \end{array}\tag{C.145}
$$

We then move on to the ratio of the asset to bond price, 

$$
\begin{array}{r c l} \phi_ {t} d \left(\frac {S _ {t}}{B _ {t}}\right) & = & \phi_ {t} \left(\frac {d S _ {t}}{B _ {t}} - \frac {S _ {t} d B _ {t}}{B _ {t} ^ {2}} - \frac {d C _ {t} d B _ {t}}{B _ {t} ^ {2}}\right) \\ & = & \frac {\sigma_ {t} ^ {C} C _ {t}}{\sigma_ {t} S _ {t}} \frac {S _ {t}}{B _ {t}} \left(\frac {d S _ {t}}{S _ {t}} - \frac {d B _ {t}}{B _ {t}}\right) \\ & = & \frac {\sigma_ {t} ^ {C} C _ {t}}{\sigma_ {t} B _ {t}} \left(\mu_ {t} d t + \sigma_ {t} d W _ {t} - r _ {t} d t\right). \end{array}\tag{C.146}
$$

Taking the diference between the two yields 

$$
\begin{array}{r c l} d \left(\frac {C _ {t}}{B _ {t}}\right) - \phi_ {t} d \left(\frac {S _ {t}}{B _ {t}}\right) & = & \frac {C _ {t}}{B _ {t}} \left[ \mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t} - r _ {t} d t \right. \\ & & \left. - \frac {\sigma_ {t} ^ {C}}{\sigma_ {t}} \left(\mu_ {t} d t + \sigma_ {t} d W _ {t} - r _ {t} d t\right) \right] \\ & = & \frac {C _ {t} \sigma_ {t} ^ {C}}{B _ {t}} \left[ \frac {\mu_ {t} ^ {C} - r _ {t}}{\sigma_ {t} ^ {C}} d t + d W _ {t} - \frac {\mu_ {t} - r _ {t}}{\sigma_ {t}} d t - d W _ {t} \right] \\ & = & \frac {C _ {t} \sigma_ {t} ^ {C}}{B _ {t}} \left[ \frac {\mu_ {t} ^ {C} - r _ {t}}{\sigma_ {t} ^ {C}} d t - \frac {\mu_ {t} - r _ {t}}{\sigma_ {t}} d t \right] \\ & = & 0. \end{array} \tag {C.14}\tag{C.147}
$$

(b) The equation $C _ { t } = \phi _ { t } S _ { t } + \psi _ { t } B _ { t }$ can be taken as the definition of $\psi _ { t }$ . Hence calculating the diferential, 

$$
\begin{array}{r c l} B _ {t} d \psi_ {t} & = & B _ {t} d \left(\frac {C _ {t}}{B _ {t}} - \phi_ {t} \frac {S _ {t}}{B _ {t}}\right) \\ & = & B _ {t} \left[ d \left(\frac {C _ {t}}{B _ {t}}\right) - \phi_ {t} d \left(\frac {S _ {t}}{B _ {t}}\right) - d \phi_ {t} \frac {S _ {t}}{B _ {t}} \right. \\ & & \left. - d \phi_ {t} d \left(\frac {S _ {t}}{B _ {t}}\right) \right] \end{array}\tag{C.148}
$$

Using the diferential rule for ratios of stochastic processes that we calculated in exercise 12.4, we obtain 

$$
B _ {t} d \psi_ {t} = - d \phi_ {t} S _ {t} - d \phi_ {t} d S _ {t} + d \phi_ {t} \frac {S _ {t} d B _ {t}}{B _ {t}} + d \phi_ {t} \frac {d S _ {t} d B _ {t}}{B _ {t}}\tag{C.149}
$$

We then notice that since $d B _ { t }$ is deterministic, that ${ \mathrm { i s } } ,$ it has only $d t$ terms and not $d W _ { t }$ terms, the product of $d B _ { t }$ with any other stochastic diferential is always zero. Hence we obtain 

$$
B _ {t} d \psi_ {t} = - d \phi_ {t} S _ {t} - d \phi_ {t} d S _ {t}.\tag{C.150}
$$

(c) Finally, if we take the diferential of $C _ { t }$ we obtain 

$$
d C _ {t} = \phi_ {t} d S _ {t} + d \phi_ {t} S _ {t} + d \phi_ {t} d S _ {t} + d \psi_ {t} B _ {t} + \psi_ {t} d B _ {t} + d \psi_ {t} d B _ {t}.\tag{C.151}
$$

We then want to set $d \psi _ { t } d B _ { t } = 0$ and substitute for $B _ { t } d \psi _ { t }$ from above, 

$$
\begin{array}{r c l} d C _ {t} & = & \phi_ {t} d S _ {t} + d \phi_ {t} S _ {t} + d \phi_ {t} d S _ {t} - d \phi_ {t} S _ {t} - d \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t} \\ & = & \phi_ {t} d S _ {t} + \psi_ {t} d B _ {t}. \end{array}\tag{C.152}
$$

Thus, we see that the trading strategy $( \phi _ { t } , \psi _ { t } )$ is, in fact, self-financing. 

## Section 15

1. We want to calculate the expectation of a stochastic integral 

$$
I = \int_ {0} ^ {t} g (W _ {s}) d W _ {s},\tag{C.153}
$$

where $g ( W _ { s } )$ is an arbitrary well-behaved function. Recall from equation (12.3) that the definition of the stochastic integral is 

$$
I = \lim _ {N \to \infty} \sum_ {i = 0} ^ {N} g (W _ {t _ {i}}) (W _ {t _ {i + 1}} - W _ {t _ {i}}),\tag{C.154}
$$

where the $t _ { i }$ are some partition of the interval [0, 1]. Taking expectations of this we have 

$$
E [ I ] = \lim _ {N \rightarrow \infty} \sum_ {i = 0} ^ {N} E \left[ g \left(W _ {t _ {i}}\right)\left(W _ {t _ {i + 1}} - W _ {t _ {i}}\right)\right].\tag{C.155}
$$

But by the independent increments property of Brownian motion, we know that $( W _ { t _ { i + 1 } } - W _ { t _ { i } } )$ and $W _ { t _ { i } }$ are independent random variables and hence we can factor their product in an expectation, that is, 

$$
E [ I ] = \lim _ {N \to \infty} \sum_ {i = 0} ^ {N} E [ g (W _ {t _ {i}}) ] E [ (W _ {t _ {i + 1}} - W _ {t _ {i}}) ].\tag{C.156}
$$

But the expected value of the diference of a Brownian motion at two diferent times is zero $E [ ( \mathbf { \tilde { W } } _ { t _ { i + 1 } } - W _ { t _ { i } } ) ] = 0$ and hence every term in the sum vanishes. Thus 

$$
E [ I ] = 0,\tag{C.157}
$$

which is what we set out to prove. 

2. We want to verify that the function 

$$
\begin{array}{r c l} A (x, \tau) & = & E [ f (x + \sigma W _ {\tau}) ] \\ & = & \frac {1}{\sqrt {2 \pi \tau}} \int_ {- \infty} ^ {\infty} f (x + \sigma \xi) \exp \left[ - \frac {\xi^ {2}}{2 \tau} \right] d \xi \end{array}\tag{C.158}
$$

is a solution of the heat equation 

$$
\frac {\partial A}{\partial \tau} = \frac {1}{2} \sigma^ {2} \frac {\partial^ {2} A}{\partial x ^ {2}}.\tag{C.159}
$$

In order to simplify the calculation, we define a new integration variable $\eta = x + \sigma \xi$ This has the efect of moving the x and τ dependence from f into the exponential, 

$$
A = \frac {1}{\sqrt {2 \pi \tau}} \int_ {- \infty} ^ {\infty} f (\eta) \exp \left[ - \frac {(\eta - x) ^ {2}}{2 \sigma^ {2} \tau} \right] d \eta .\tag{C.160}
$$

We now need to calculate the derivatives, 

$$
\begin{array}{r c l} \frac {\partial A}{\partial \tau} & = & - \frac {1}{2 \sqrt {2 \pi} \tau^ {3 / 2}} \int_ {- \infty} ^ {\infty} f (\eta) \exp \left[ - \frac {(\eta - x) ^ {2}}{2 \sigma^ {2} \tau} \right] d \eta \\ & & + \frac {1}{\sqrt {2 \pi \tau}} \int_ {- \infty} ^ {\infty} f (\eta) \frac {(\eta - x) ^ {2}}{2 \sigma^ {2} \tau^ {2}} \exp \left[ - \frac {(\eta - x) ^ {2}}{2 \sigma^ {2} \tau} \right] d \eta \end{array}\tag{C.161}
$$

and 

$$
\frac {\partial A}{\partial x} = \frac {1}{\sqrt {2 \pi \tau}} \int_ {- \infty} ^ {\infty} f (\eta) \frac {\eta - x}{\sigma^ {2} \tau} \exp \left[ - \frac {(\eta - x) ^ {2}}{2 \sigma^ {2} \tau} \right] d \eta\tag{C.162}
$$

which yields 

$$
\begin{array}{r l r} \frac {\partial^ {2} A}{\partial x ^ {2}} & = & \frac {1}{\sqrt {2 \pi \tau}} \int_ {- \infty} ^ {\infty} f (\eta) \frac {- 1}{\sigma^ {2} \tau} \exp \left[ - \frac {(\eta - x) ^ {2}}{2 \sigma^ {2} \tau} \right] d \eta \\ & + & \frac {1}{\sqrt {2 \pi \tau}} \int_ {- \infty} ^ {\infty} f (\eta) \frac {(\eta - x) ^ {2}}{\sigma^ {4} \tau^ {2}} \exp \left[ - \frac {(\eta - x) ^ {2}}{2 \sigma^ {2} \tau} \right] d \eta \end{array}\tag{C.163}
$$

from which the result follows. 

3. We want to price a forward contract with strike $K$ and maturity $T .$ . The payof function $F ( \hat { S _ { T } } ) = S _ { T } - K$ is simply the diference between the share price $S _ { T }$ at maturity and the strike price. Writing the derivative price in terms of an expectation we obtain 

$$
\begin{array}{r c l} {F _ {0}} & = & {e ^ {- r T} E ^ {*} [ F (S _ {T}) ]} \\ & = & {e ^ {- r T} E ^ {*} [ S _ {T} - K ]} \\ & = & {e ^ {- r T} E ^ {*} [ S _ {T} ] - e ^ {- r T} E ^ {*} [ K ].} \end{array}\tag{C.164}
$$

But in equation (15.43) we calculated the price of a derivative that simply pays of the share value at maturi ${ \mathrm { J } } ,$ and found that it was just the initial share price $S _ { 0 }$ This result allows us to evaluate the first term in equation (C.164). To evaluate the second term, we note that the expectation of a constant is simply its value. We then have 

$$
F _ {0} = S _ {0} - e ^ {- r T} K,\tag{C.165}
$$

which is the no arbitrage price for the derivative. The value of the strike K which zeros the initial cost of the derivative is $S _ { 0 } e ^ { r T }$ . This is called the forward price for the asset. 

## Section 16

1. In this question we want to calculate and plot the partial derivatives of the call option price with respect to various parameters. These quantities are useful when trying to create portfolios which are hedged against movements or estimation errors in the parameters. Recall the that price of a call option is 

$$
C _ {0} = S _ {0} N (h ^ {+}) - K e ^ {- r T} N (h ^ {-}).\tag{C.166}
$$

If we diferentiate this value with respect to an arbitrary parameter x we obtain 

$$
\begin{array}{r c l} \frac {\partial C _ {0}}{\partial x} & = & \frac {\partial}{\partial x} [ S _ {0} N (h ^ {+}) ] - \frac {\partial}{\partial x} [ K e ^ {- r T} N (h ^ {-}) ] \\ & = & \frac {\partial S _ {0}}{\partial x} N (h ^ {+}) - \frac {\partial (K e ^ {- r T})}{\partial x} N (h ^ {-}) \\ & & + S _ {0} \frac {\partial N (h ^ {+})}{\partial x} - K e ^ {- r T} \frac {\partial N (h ^ {-})}{\partial x}. \end{array}\tag{C.167}
$$

We can simplify the last two derivatives. Begin by using the chain rule for diferentiation, 

$$
\frac {\partial N (h ^ {\pm})}{\partial x} = \frac {1}{\sqrt {2 \pi}} \frac {\partial h ^ {\pm}}{\partial x} e ^ {- (h ^ {\pm}) ^ {2} / 2}.\tag{C.168}
$$

If we substitute in the values of $h ^ { \pm }$ , we see that 

$$
e ^ {- (h ^ {\pm}) ^ {2} / 2} = e ^ {- X} \left(\frac {S _ {0} e ^ {r T}}{K}\right) ^ {\mp 1 / 2},\tag{C.169}
$$

where 

$$
X = \frac {(\log \tilde {S} / K) ^ {2} + \frac {1}{4} \sigma^ {4} T ^ {2}}{2 \sigma^ {2} T}.\tag{C.170}
$$

Substituting this back into equation (C.167) we see that 

$$
\begin{array}{r c l} \frac {\partial C _ {0}}{\partial x} & = & \frac {\partial S _ {0}}{\partial x} N (h ^ {+}) - \frac {\partial K e ^ {- r T}}{\partial x} N (h ^ {-}) \\ & & + S _ {0} e ^ {- (h ^ {+}) ^ {2} / 2} \frac {\partial h ^ {+}}{\partial x} - K e ^ {- r T} e ^ {- (h ^ {-}) ^ {2} / 2} \frac {\partial h ^ {-}}{\partial x} \\ & = & \frac {\partial S _ {0}}{\partial x} N (h ^ {+}) - \frac {\partial K e ^ {- r T}}{\partial x} N (h ^ {-}) \\ & & + e ^ {- X} \left(\frac {S _ {0} K}{e ^ {r T}}\right) ^ {1 / 2} \frac {\partial h ^ {+}}{\partial x} - e ^ {- X} \left(\frac {S _ {0} K}{e ^ {r T}}\right) ^ {1 / 2} \frac {\partial h ^ {-}}{\partial x} \\ & = & \frac {\partial S _ {0}}{\partial x} N (h ^ {+}) - \frac {\partial K e ^ {- r T}}{\partial x} N (h ^ {-}) \\ & & + \frac {1}{\sqrt {2 \pi}} e ^ {- X} \left(\frac {S _ {0} K}{e ^ {r T}}\right) ^ {1 / 2} \frac {\partial (h ^ {+} - h ^ {-})}{\partial x} \end{array}\tag{C.171}
$$

But $h ^ { + } - h ^ { - } = \sigma \sqrt { T }$ and so we end up with the relatively simple formula 

$$
\begin{array}{r c l} \frac {\partial C _ {0}}{\partial x} & = & \frac {\partial S _ {0}}{\partial x} N (h ^ {+}) - \frac {\partial K e ^ {- r T}}{\partial x} N (h ^ {-}) \\ & & + \frac {1}{\sqrt {2 \pi}} e ^ {- X} \left(\frac {S _ {0} K}{e ^ {r T}}\right) ^ {1 / 2} \frac {\partial (\sigma \sqrt {T})}{\partial x}. \end{array}\tag{C.172}
$$

(a) The first quantity that we want to calculate is the change in the option price with respect to a change in the value fo the underlying asset price. We see that only the first term in equation (C.172) contributes and 

$$
\begin{array}{r c l} \Delta & = & \frac {\partial C _ {0}}{\partial S _ {0}} \\ & = & N (h ^ {+}). \end{array}\tag{C.173}
$$

(b) If we now take a second derivative of this, 

$$
\begin{array}{r c l} \Gamma & = & \frac {\partial^ {2} C _ {0}}{\partial S _ {0} ^ {2}} \\ & = & \frac {\partial N (h ^ {+})}{\partial S _ {0}} \\ & = & \frac {1}{\sqrt {2 \pi}} \frac {1}{\sigma \sqrt {T} S _ {0}} e ^ {- X} \left(\frac {S _ {0} e ^ {r T}}{K}\right) ^ {- 1 / 2} \end{array}\tag{C.174}
$$

(c) If we calculate the efect of varying the volatility, only the final term in (C.172) contributes, 

$$
\begin{array}{r c l} \mathcal {V} & = & \frac {\partial C _ {0}}{\partial \sigma} \\ & = & \frac {1}{\sqrt {2 \pi}} e ^ {- X} \left(\frac {S _ {0} K}{e ^ {r T}}\right) ^ {1 / 2} \sqrt {T}. \end{array}\tag{C.175}
$$

(d) Calculating the change in the derivative value as we change the time to expiry, we get contributions from the last two terms in (C.172), 

$$
\begin{array}{r c l} \theta & = & - \frac {\partial C _ {0}}{\partial T} \\ & = & - \frac {1}{\sqrt {2 \pi}} e ^ {- X} \left(\frac {S _ {0} K}{e ^ {r T}}\right) ^ {1 / 2} \frac {\sigma}{2 \sqrt {T}} - r K e ^ {- r T} N (h ^ {-}) \end{array}\tag{C.176}
$$

(e) Finally, if we vary the interest rate we obtain 

$$
\begin{array}{r c l} \rho & = & \frac {\partial C _ {0}}{\partial r} \\ & = & k T e ^ {- r T} N (h ^ {-}). \end{array}\tag{C.177}
$$

## Section 17

1. We want to calculate the initial value of a binary put option with a payof function $B P _ { T } ( S _ { T } ) = H ( K - S _ { T } )$ at time T. Using the derivative pricing equation (15.38), we see that 

$$
\begin{array}{r c l} B P _ {0} & = & e ^ {- r T} E ^ {*} [ B P _ {T} (S _ {T}) ] \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi T}} \int_ {- \infty} ^ {\infty} H (K - S _ {T}) e ^ {- \xi^ {2} / 2 T} d \xi \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi T}} \int_ {- \infty} ^ {\infty} H \left(K - S _ {0} \exp [ (r - \frac {1}{2} \sigma^ {2}) T + \sigma \xi ]\right) e ^ {- \xi^ {2} / 2 T} d \xi \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} H \left(K - S _ {0} \exp [ (r - \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta ]\right) \\ & & \times e ^ {- \eta^ {2} / 2} d \eta , \end{array}\tag{C.178}
$$

where we have made the substitution $\eta = \xi / \sqrt { T }$ in the final integral. The Heaviside function is non-zero only when 

$$
S _ {0} \exp \left[ (r - \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta \right] <   K.\tag{C.179}
$$

Taking logarithms and isolating η yields 

$$
\begin{array}{r c l} (r - \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta & <   & - \log (S / K) \\ \eta & <   & - \log (S / K) + (r - \frac {1}{2} \sigma^ {2}) T \sigma \sqrt {T} \\ \eta & <   & - h ^ {-}. \end{array}\tag{C.180}
$$

Thus the integral simplifies to 

$$
\begin{array}{r c l} {B P _ {0}} & = & {\frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {- h ^ {-}} e ^ {- \eta^ {2} / 2} d \eta} \\ & = & {e ^ {- r T} N (- h ^ {-}).} \end{array}\tag{C.181}
$$

We could have calculated this result by using the binary call option price, calculated in equation (C.250) 

$$
B C _ {0} = e ^ {- r T} N (h ^ {-}),\tag{C.182}
$$

and the put-call result of equation (17.16) 

$$
B C _ {0} + B P _ {0} = e ^ {- r T}.\tag{C.183}
$$

These two equations immediately tell us that 

$$
B P _ {0} = e ^ {- r T} [ 1 - N (h ^ {-}) ].\tag{C.184}
$$

If we then use the relation $N ( x ) + N ( - x ) = 1$ , we recover the formula calculated above, 

$$
B P _ {0} = e ^ {- r T} N (- h ^ {-}).\tag{C.185}
$$

2. Using positions in the underlying and call options, we want to construct a Gamma neutral portfolio which is short one binary call. If we hold φ shares and ψ call options, then the value of the portfolio is 

$$
V _ {0} = - B C _ {0} + \phi S _ {0} + \psi C _ {0}.\tag{C.186}
$$

Diferentiating with respect to the share price, we find that 

$$
\Delta = - \Delta_ {b c} + \phi + \psi \Delta_ {c}\tag{C.187}
$$

where $\Delta _ { b c }$ and $\Delta _ { c }$ are the Deltas of the binary call and call options respectively. Diferentiating again, we find the Gamma of the portfolio, 

$$
\Gamma = - \Gamma_ {b c} + \psi \Gamma_ {c}.\tag{C.188}
$$

Making the portfolio Gamma neutral, we can solve for the value of $\psi _ { ; }$ 

$$
\psi = \frac {\Gamma_ {b c}}{\Gamma_ {c}}.\tag{C.189}
$$

We can then make the portfolio Delta neutral, and hence obtain the value of $\phi ,$ 

$$
\phi = \Delta_ {b c} - \frac {\Gamma_ {b c}}{\Gamma_ {c}} \Delta_ {c}.\tag{C.190}
$$

In a previous exercise we determined the values of Delta and Gamma for the call option 

$$
\Delta_ {c} = N (h ^ {+}) \quad \mathrm{and} \quad \Gamma_ {c} = \frac {1}{\sigma \sqrt {T} S _ {0}} \frac {e ^ {- X}}{\sqrt {2 \pi}} \sqrt {\frac {K}{S _ {0} e ^ {r T}}},\tag{C.191}
$$

where 

$$
X = \frac {(\log \tilde {S} / K) ^ {2} + \frac {1}{4} \sigma^ {4} T ^ {2}}{2 \sigma^ {2} T}.\tag{C.192}
$$

Substituting in the numbers $K = 1 2 0 , S _ { 0 } = 1 0 0 , r = 0 . 0 5 , \sigma = . 2$ and $T = 1 . 0$ for the call option, we find that 

$$
\Delta_ {c} = 0. 2 8 7 1 9 2 \quad \mathrm{and} \quad \Gamma_ {c} = 0. 0 1 7 0 3 6 9.\tag{C.193}
$$

To calculate the Delta and Gamma for the binary call, we recall that the price is 

$$
B C _ {0} = e ^ {- r T} N (h ^ {-}).\tag{C.194}
$$

Diferentiating twice with respect to $S _ { 0 }$ we find that 

$$
\Delta_ {b c} = \frac {e ^ {- r t}}{\sqrt {2 \pi}} \frac {1}{\sigma \sqrt {T}} \frac {1}{\sqrt {K S _ {0} e ^ {r T}}} \quad \mathrm{and} \quad \Gamma_ {b c} = - \frac {\Delta_ {b}}{\sigma \sqrt {T} S _ {0}} h ^ {+}.\tag{C.195}
$$

Substituting in K = 110, S<sub>0</sub> = 100, r = 0.05, σ = .2 and $T = 1 . 0$ we find that 

$$
\Delta_ {b c} = 0. 0 1 7 9 8 9 1 \quad \mathrm{and} \quad \Gamma_ {b c} = 0. 0 0 0 1 1 3 8 2 7,\tag{C.196}
$$

which allows us to determine the share and call options holdings, 

$$
\phi = 0. 0 1 6 0 7 0 3 \quad \text { and } \quad \psi = 0. 0 0 6 6 8 1 1 9.\tag{C.197}
$$

3. We can Gamma hedge a short position in a call option with strike $K _ { 1 }$ by using a position in both the underlying asset and a call option with strike $K _ { 2 }$ . Besides the underlying asset, we could actually use any derivative based on the asset to Gamma hedge the call option, as long as the derivative has a non-zero Gamma itself. So we could, for example, hedge a call option with a strike of $100 by using the underlying and a call with a strike of $120. 

4. In order to derive the put-call relation when $S _ { t }$ is the price of sterling in dollars, we need to calculate the value of a forward contract with strike K. Suppose that a dealer agrees at time 0 to pay K dollars for 1 pound sterling at time $T ,$ , receiving an initial payment of $F _ { 0 }$ dollars for entering into the contract. How can he determine the arbitrage free value of $F _ { 0 } ?$ Well, he can replicate the dollar cash-flow by going short $K e ^ { - { \overset { \smile } { r } } T }$ dollars in the dollar money market account, where r is the dollar interest rate. This will be worth $- K$ dollars at time $T ,$ . Similarly by taking a long position of $e ^ { - \rho T }$ pounds in the sterling money market account, where $\rho$ is the sterling interest rate, we produce the 1 pound cash-flow at time $\overset { \vartriangle } { \boldsymbol { T } } .$ . The dollar value of the replicating portfolio is $S _ { 0 } e ^ { - \rho T } \overset { \cdot } { - } K e ^ { - r T }$ dollars, where $S _ { 0 }$ is the initial exchange rate. By the no arbitrage condition, the value of the forward contract must equal the calue of the replicating portfolio, and hence 

$$
F _ {0} = S _ {0} e ^ {- r T} - K e ^ {\rho T}.\tag{C.198}
$$

But the payof of portfolio with a long position in a call and a short position in a put, both with strike K and maturity $\stackrel { \smile } { T } ,$ has the same payof as a forward contract with the same strike and maturity. Hence the initial prices must also be the same, so 

$$
C _ {0} - P _ {0} = S _ {0} e ^ {- r T} - K e ^ {\rho T},\tag{C.199}
$$

which is the put-call relation for foreign exchange options. 

5. We can verify the put-call formula explicitly by using the Black-Scholes formula for the call and put option prices. Recall that the call option price is given by 

$$
C _ {0} = e ^ {- r T} [ S _ {0} e ^ {r T} N (h ^ {+}) - K N (h ^ {-}) ].\tag{C.200}
$$

But the cumulative normal density function satisfies $N ( x ) = 1 - N ( - x )$ . Hence 

$$
C _ {0} = e ^ {- r T} [ S _ {0} e ^ {r T} (1 - N (- h ^ {+})) - K (1 - N (- h ^ {-})) ],\tag{C.201}
$$

which can be written in the form 

$$
C _ {0} = S _ {0} - e ^ {- r T} K + e ^ {- r T} [ K N (- h ^ {-}) - S _ {0} e ^ {r T} N (- h ^ {+}) ].\tag{C.202}
$$

The last term in this expression is the value of a put option, as given in equation (16.35). Thus, we can write 

$$
C _ {0} = S _ {0} - e ^ {- r T} K + P _ {0}.\tag{C.203}
$$

## Section 18

1. To calculate the put-call relation for the constant dividend yield model we simply equate the value of a portfolio which is long a call and short a put with the value of a forward contract, where all three derivatives have the same strike K and the same maturity T. Hence 

$$
C _ {0} - P _ {0} = S _ {0} e ^ {- \delta T} - K e ^ {- r T}.\tag{C.204}
$$

2. We want to derive the Black-Scholes equation by using a no arbitrage argument on a hedged portfolio. Starting with nothing, if we take the position $V _ { t } = C _ { t } - \phi _ { t } S _ { t } - \psi _ { t } B _ { t }$ then since it has no net value, we can solve for the bond position ψ<sub>t</sub> 

$$
\psi_ {t} = \frac {C _ {t}}{B _ {t}} - \phi_ {t} \frac {S _ {t}}{B _ {t}}.\tag{C.205}
$$

At time $t + d t$ the value of the portfolio has changed to 

$$
d V _ {t} = d C _ {t} + \delta_ {t} ^ {C} C _ {t} d t - \phi_ {t} d S _ {t} - \phi_ {t} \delta_ {t} S _ {t} d t - \psi_ {t} d B _ {t},\tag{C.206}
$$

where we have kept the stock and bond holdings fixed, and included the dividend payments that we receive for holding the derivative, minus the dividend payments that we must make since we are short the stock. Substituting in for the stochastic diferentials from equations (13.1), (13.2) and (13.4) we obtain 

$$
\begin{array}{r c l} d V _ {t} & = & \frac {\partial C _ {t}}{\partial t} d t + \frac {\partial C _ {t}}{\partial S _ {t}} d S _ {t} + \frac {1}{2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} d S _ {t} ^ {2} - \phi_ {t} d S _ {t} \\ & & + (\delta_ {t} ^ {C} C _ {t} - \phi_ {t} \delta_ {t} S _ {t}) d t - \left(\frac {C _ {t}}{B _ {t}} - \phi_ {t} \frac {S _ {t}}{B _ {t}}\right) r _ {t} B _ {t} d t. \end{array}\tag{C.207}
$$

Since $d S _ { t } ^ { 2 } = \sigma _ { t } ^ { 2 } S _ { t } ^ { 2 } d t$ , the only diferential that contains a random component is $d S _ { t } .$ . Hence we can obtain a guaranteed return on our portfolio if we set the stock holding φ<sub>t</sub> to be 

$$
\phi_ {t} = \frac {\partial C _ {t}}{\partial S _ {t}}.\tag{C.208}
$$

The fixed return is then 

$$
d V _ {t} = \left(\frac {\partial C _ {t}}{\partial t} - \frac {1}{2} \sigma_ {t} ^ {2} s _ {t} ^ {2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} - (r _ {t} - \delta_ {t} ^ {C}) C _ {t} + (r _ {t} - \delta_ {t}) S _ {t} \frac {\partial C _ {t}}{\partial S _ {t}}\right) d t.\tag{C.209}
$$

By the no arbitrage condition this must be zero, and hence we recover the Black-Scholes equation 

$$
\frac {\partial C _ {t}}{\partial t} + \frac {1}{2} \sigma_ {t} ^ {2} S _ {t} ^ {2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} - (r _ {t} - \delta_ {t} ^ {C}) C _ {t} + (r _ {t} - \delta_ {t}) S _ {t} \frac {\partial C _ {t}}{\partial S _ {t}} = 0.\tag{C.210}
$$

3. We want to verify that the derivative price 

$$
C _ {t} = \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F (S _ {T}) e ^ {- \frac {1}{2} \xi^ {2}} d \xi\tag{C.211}
$$

where 

$$
S _ {T} = S _ {t} \exp \left[ (r - \delta - \frac {1}{2} \sigma^ {2}) (T - t) + \sigma \sqrt {T - t} \xi \right]\tag{C.212}
$$

satisfies the continuous dividend yield Black-Scholes equation 

$$
\frac {\partial C _ {t}}{\partial t} + \frac {1}{2} \sigma^ {2} S _ {t} ^ {2} \frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} + (r - \delta) S _ {t} \frac {\partial C _ {t}}{\partial S _ {t}} - (r - \delta^ {C}) C _ {t} = 0.\tag{C.213}
$$

Calculating the derivative with respect to the asset price using the chain rule, we have 

$$
\frac {\partial C _ {t}}{\partial S _ {t}} = \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \frac {\partial F (S _ {T})}{\partial S _ {T}} \frac {\partial S _ {T}}{\partial S _ {t}} e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{C.214}
$$

We see that 

$$
\frac {\partial S _ {T}}{\partial S _ {t}} = \frac {S _ {T}}{S _ {t}},\tag{C.215}
$$

and hence 

$$
\frac {\partial C _ {t}}{\partial S _ {t}} = \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \frac {\partial F (S _ {T})}{\partial S _ {T}} \frac {S _ {T}}{S _ {t}} e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{C.216}
$$

Calculating the second derivative, we obtain 

$$
\frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} = \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \frac {\partial^ {2} F (S _ {T})}{\partial S _ {T} ^ {2}} \frac {S _ {T} ^ {2}}{S _ {t} ^ {2}} e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{C.217}
$$

We then want to convert one diferentiation with respect to $S _ { T }$ into a derivative with respect to $\xi ,$ 

$$
\frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} = \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \frac {\partial^ {2} F (S _ {T})}{\partial \xi \partial S _ {T}} \frac {\partial \xi}{\partial S _ {T}} \frac {S _ {T} ^ {2}}{S _ {t} ^ {2}} e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{C.218}
$$

Inverting the relationship between $S _ { T }$ and $\xi ,$ we have 

$$
\xi = \frac {\log S _ {T} - \log S _ {t} + (r - \delta) (T - t) - \frac {1}{2} \sigma^ {2} (T - t)}{\sigma \sqrt {T - t}}\tag{C.219}
$$

and hence 

$$
\frac {\partial \xi}{\partial S _ {T}} = \frac {1}{S _ {T} \sigma \sqrt {T - t}}.\tag{C.220}
$$

Thus 

$$
\frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} = \frac {e ^ {- (r - \delta^ {\mathcal {C}}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \frac {\partial^ {2} F (S _ {T})}{\partial \xi \partial S _ {T}} \frac {1}{S _ {T} \sigma \sqrt {T - t}} \frac {S _ {T} ^ {2}}{S _ {t} ^ {2}} e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{C.221}
$$

We now want to integrate by parts to remove the derivative with respect to $\xi .$ The boundary terms at positive and negative infinity will vanish. Hence we are left with 

$$
\frac {\partial^ {2} C _ {t}}{\partial S _ {t} ^ {2}} = - \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi} S _ {t} ^ {2}} \int_ {- \infty} ^ {\infty} \frac {\partial F (S _ {T})}{\partial S _ {T}} \left[ S _ {T} - \frac {\xi S _ {T}}{\sigma \sqrt {T - t}} \right] e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{C.222}
$$

The derivative with respect to time is slightly more complicated, 

$$
\frac {\partial C _ {t}}{\partial t} = (r - \delta^ {C}) C _ {t} + \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \frac {\partial F (S _ {T})}{\partial S _ {T}} \frac {\partial S _ {T}}{\partial t} e ^ {- \frac {1}{2} \xi^ {2}} d \xi .\tag{C.223}
$$

We note that 

$$
\frac {\partial S _ {T}}{\partial t} = - S _ {T} \left[ (r - \delta - \frac {1}{2} \sigma^ {2} + \frac {\sigma \xi}{2 \sqrt {T - t}} \right].\tag{C.224}
$$

Substituting back in, we have 

$$
\begin{array}{r c l} \frac {\partial C _ {t}}{\partial t} & = & (r - \delta^ {C}) C _ {t} - \\ & & \frac {e ^ {- (r - \delta^ {C}) (T - t)}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \frac {\partial F (S _ {T})}{\partial S _ {T}} S _ {T} \left[ r - \delta - \frac {1}{2} \sigma^ {2} + \frac {\sigma \xi}{2 \sqrt {T - t}} \right] e ^ {- \frac {1}{2} \xi^ {2}} (\mathrm{d} \xi 2 5) \end{array}
$$

Combining all the terms we see that the equation is satisfied. 

4. Recall that the call option payof is 

$$
F (S _ {T}) = \max (S _ {T} - K, 0).\tag{C.226}
$$

Hence the initial price of the derivative is 

$$
\begin{array}{r c l} C _ {0} & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} F \left(S _ {0} \exp \left[ (r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right]\right) \exp \left[ - \frac {1}{2} \xi^ {2} \right] \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} \max \left(S _ {0} \exp \left[ (r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K, 0\right) \\ & & \times \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi . \end{array} \tag {C}\tag{C.227}
$$

In order to evaluate the integral we need to remove the max function. This can easily be accomplished because it will be nonzero only when 

$$
S _ {0} \exp \left[ (r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K > 0,\tag{C.228}
$$

which is equivalent to 

$$
\exp \left[ (r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] > K / S _ {0}.\tag{C.229}
$$

Taking logarithms of both sides we obtain 

$$
(r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T > \log (K / S _ {0}).\tag{C.230}
$$

We then want to isolate the integration variable $\xi .$ This will allow us to discover the integration region where the max function is nonzero. We find that 

$$
\xi > \frac {\log (K / S _ {0}) - (r - \delta - \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}}.\tag{C.231}
$$

If we define the critical value $\xi ^ { * }$ to be 

$$
\xi^ {*} = \frac {\log (K / S _ {0}) - (r - \delta - \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}},\tag{C.232}
$$

then the max function can be written as 

$$
\begin{array}{l} \max \left(S _ {0} \exp \left[ (r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K, 0\right) \\ = \left\{ \begin{array}{l l} S _ {0} e ^ {(r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T} - K & \xi > \xi^ {*} \\ 0 & \xi <   \xi^ {*}. \end{array} \right. \end{array}\tag{C.233}
$$

Since the integrand vanishes for $\xi < \xi ^ { * }$ , we only need to integrate ove r the region where $\xi > \xi ^ { * }$ and the max function takes on a positive value. Hence the derivative price becomes 

$$
C _ {0} = \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} \left(S _ {0} \exp \left[ (r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] - K\right) \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi .\tag{C.234}
$$

This integral involves two terms, and it is easiest to evaluate them separately. If we define 

$$
\begin{array}{r c l} I _ {1} & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} S _ {0} \exp \left[ (r - \delta) T + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi \\ & = & \frac {e ^ {- \delta T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} S _ {0} \exp \left[ - \frac {1}{2} \xi^ {2} + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] \end{array}\tag{C.235}
$$

and 

$$
I _ {2} = - K \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} \exp \left[ - \frac {1}{2} \xi^ {2} \right] d \xi ,\tag{C.236}
$$

then the derivative price is simply the sum of the two integrals, $C _ { 0 } = I _ { 1 } + I _ { 2 }$ . The second integral is easier, so we shall calculate it first. Before we do this, consider the following result 

$$
\begin{array}{r c l} \frac {1}{\sqrt {2 \pi}} \int_ {x} ^ {\infty} e ^ {- \frac {1}{2} \xi^ {2}} d \xi & = & \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {- x} e ^ {- \frac {1}{2} u ^ {2}} d u \\ & = & N (- x), \end{array}\tag{C.237}
$$

where we made the substitution $u = - \xi$ in the first line and $N ( x )$ is the standard normal cumulative probability density function, previously defined in equation (11.4). Using this result, we see that 

$$
\begin{array}{r c l} {I _ {2}} & = & {- K \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {- \xi^ {*}} e ^ {- \frac {1}{2} \xi^ {2}} d \xi} \\ & = & {- K e ^ {- r T} N (- \xi^ {*}).} \end{array}\tag{C.238}
$$

However, the standard way of writing the Black-Scholes formula is not in terms of $\xi ^ { * }$ , but rather in terms of two new constants $h ^ { + }$ and $h ^ { - }$ , defined to be 

$$
h ^ {\pm} = \frac {\log (\tilde {S} / K) \pm \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}},\tag{C.239}
$$

where $\tilde { S }$ is the forward price $S _ { 0 } e ^ { ( r - \delta ) T }$ . If we then rewrite $- \xi ^ { * }$ as 

$$
\begin{array}{r c l} - \xi^ {*} & = & - \frac {\log (K / S _ {0}) - ((r - \delta) T - \frac {1}{2} \sigma^ {2} T)}{\sigma \sqrt {T}} \\ & = & \frac {\log (S _ {0} / K) + (r - \delta) T - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}} \\ & = & \frac {\log (\tilde {S} / K) - \frac {1}{2} \sigma^ {2} T}{\sigma \sqrt {T}}, \end{array}\tag{C.240}
$$

we see that 

$$
- \xi^ {*} = h ^ {-} \quad \text { and } \quad - \xi^ {*} + \sqrt {\sigma} T = h ^ {+}.\tag{C.241}
$$

Hence we can write the integral $I _ { 2 }$ as 

$$
I _ {2} = - e ^ {- r T} K N (h ^ {-}).\tag{C.242}
$$

We now want to calculate the slightly more complicated integral $I _ { 1 }$ . We begin by ‘completing the square’ in the exponential, 

$$
\begin{array}{r c l} I _ {1} & = & \frac {e ^ {- \delta T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} S _ {0} \exp \left[ - \frac {1}{2} \xi^ {2} + \sigma \sqrt {T} \xi - \frac {1}{2} \sigma^ {2} T \right] d \xi \\ & = & \frac {S _ {0} e ^ {- \delta T}}{\sqrt {2 \pi}} \int_ {\xi^ {*}} ^ {\infty} \exp \left[ - \frac {1}{2} (\xi - \sigma \sqrt {T}) ^ {2} \right] d \xi . \end{array}\tag{C.243}
$$

We then want to make a change of integration variable to $\eta = \xi - \sigma \sqrt { T } .$ . In this case $d \xi = d \eta .$ , and the lower limit of integration $\xi = \xi ^ { * }$ , becomes the new lower limit $\overset { \cdot } { \eta } = \xi ^ { * } - \sigma \sqrt { T } = - h ^ { + }$ . Hence the integral becomes 

$$
I _ {1} = \frac {S _ {0} e ^ {- \delta T}}{\sqrt {2 \pi}} \int_ {\eta = - h ^ {+}} ^ {\eta = \infty} e ^ {- \frac {1}{2} \eta^ {2}} d \eta .\tag{C.244}
$$

We can then use the result (C.237) to write the integral in terms of $N ( x )$ 2 

$$
I _ {1} = S _ {0} e ^ {- \delta T} N (h ^ {+}).\tag{C.245}
$$

If we then sum the values of the integrals $I _ { 1 }$ and $I _ { 2 }$ we obtain 

$$
C _ {0} = e ^ {- r T} [ S _ {0} e ^ {(r - \delta) T} N (h ^ {+}) - K N (h ^ {-}) ].\tag{C.246}
$$

5. Suppose that we want to calculate the price for a binary call option. Using equation (15.38), we see that 

$$
\begin{array}{r c l} B C _ {0} & = & e ^ {- r T} E ^ {*} [ B C _ {T} (S _ {T}) ] \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi T}} \int_ {- \infty} ^ {\infty} H (S _ {T} - K) e ^ {- \xi^ {2} / 2 T} d \xi \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi T}} \int_ {- \infty} ^ {\infty} H (S _ {0} \exp [ (r - \delta - \frac {1}{2} \sigma^ {2}) T + \sigma \xi ] - K) \\ & & \times e ^ {- \xi^ {2} / 2 T} d \xi \\ & = & \frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- \infty} ^ {\infty} H (S _ {0} \exp [ (r - \delta - \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta ] - K) \\ & & \times e ^ {- \eta^ {2} / 2} d \eta , \end{array}\tag{C.247}
$$

where we made the substitution $\eta = \xi / \sqrt { T }$ in the final integral. The Heaviside function is non-zero only when 

$$
S _ {0} \exp \left[ (r - \delta \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta \right] > K.\tag{C.248}
$$

Taking logarithms and isolating η yields 

$$
\begin{array}{r c l} (r - \delta \frac {1}{2} \sigma^ {2}) T + \sigma \sqrt {T} \eta & > & - \log (S / K) \\ \eta & > & - \frac {\log (S / K) + (r - \delta \frac {1}{2} \sigma^ {2}) T}{\sigma \sqrt {T}} \\ \eta & > & - h ^ {-}. \end{array}\tag{C.249}
$$

Thus the integral simplifies to 

$$
\begin{array}{r c l} {B C _ {0}} & = & {\frac {e ^ {- r T}}{\sqrt {2 \pi}} \int_ {- h ^ {-}} ^ {\infty} e ^ {- \eta^ {2} / 2} d \eta} \\ & = & {e ^ {- r T} N (h ^ {-}) .} \end{array}\tag{C.250}
$$

## Section 19

1. Suppose that $X _ { t }$ is a stochastic process with dynamics 

$$
d X _ {t} = F (X _ {t}, t) d W _ {t}.\tag{C.251}
$$

We can integrate this equation to obtain an expression for $X _ { t }$ 

$$
X _ {t} = X _ {0} + \int_ {0} ^ {t} F (X _ {u}, u) d W _ {u}.\tag{C.252}
$$

To show that $X _ { t }$ is a martingale, we need to demonstrate that $E _ { s } [ X _ { t } ] = X _ { s }$ where ${ \cal E } _ { s } [ - ]$ is the expectation operator, conditioned upon knowing the values of $X _ { u }$ for $0 < u < s < t$ . If we take the condtional expectation of equation (C.252) then we obtain 

$$
\begin{array}{r c l} E _ {s} [ X _ {t} ] & = & E _ {s} \left[ X _ {0} + \int_ {0} ^ {t} F (W _ {u}, u) d W _ {u} \right] \\ & = & E _ {s} [ X _ {0} ] + E _ {s} \left[ \int_ {0} ^ {s} F (W _ {u}, u) d W _ {u} \right] \\ & & + E _ {s} \left[ \int_ {s} ^ {t} F (W _ {u}, u) d W _ {u} \right] \end{array}\tag{C.253}
$$

where we have split the integration up into an integral between 0 and s and an integral between s and t. By the definition of conditional expectation we know the values of $W _ { u }$ between 0 and s, and hence the integral between 0 and $s$ is ‘deterministic’ rather than ‘random’. Thus its expectation is simply the expectation of a deterministic function, which is simply equal to the value of the function, so 

$$
E [ _ {s} [ X _ {t} ] = X _ {0} + \int_ {0} ^ {s} F (W _ {u}, u) d W _ {u} + E _ {s} \left[ \int_ {s} ^ {t} F (W _ {u}, u) d W _ {u} \right].\tag{C.254}
$$

Using the definition of $\mathrm { a }$ stochastic integral, we then want to write the integral between s and t as a sum, 

$$
\begin{array}{r c l} E _ {s} [ X _ {t} ] & = & X _ {0} + \int_ {0} ^ {s} F (W _ {u}, u) d W _ {u} + E _ {s} \left[ \sum_ {i = 1} ^ {N} F \left(W _ {t _ {i}}, t _ {i}\right) \left(W _ {t _ {i + 1}} - W _ {t _ {i}}\right) \right] \\ & = & X _ {s} + \sum_ {i = 1} ^ {N} E _ {s} \left[ F \left(W _ {t _ {i}}, t _ {i}\right) \left(W _ {t _ {i + 1}} - W _ {t _ {i}}\right) \right] \end{array} \tag {C}\tag{C.255}
$$

But, by the independent increments property of Brownian motion, $( W _ { t _ { i + 1 } } - W _ { t _ { i } } )$ is an $\mathrm { N } ( 0 , t _ { i + 1 } - t _ { i } )$ random variable that is independent of $F ( W _ { t _ { i } } , t _ { i } )$ and hence we can factor the expectation, 

$$
E _ {s} [ X _ {t} ] = X _ {s} + \sum_ {i = 1} ^ {N} E _ {s} [ F (W _ {t _ {i}}, t _ {i}) ] E _ {s} [ (W _ {t _ {i + 1}} - W _ {t _ {i}}) ]\tag{C.256}
$$

Moreover, the independent increments property also implies that $( W _ { t _ { i + 1 } } - W _ { t _ { i } } )$ is independent of the value of $W _ { u }$ for $0 < u < s .$ , and hence it is not afected by the conditioning up to time $s .$ Therefore we can drop the conditioning on the expectation and we simply have 

$$
E _ {s} [ X _ {t} ] = X _ {s} + \sum_ {i = 1} ^ {N} E _ {s} [ F (W _ {t _ {i}}, t _ {i}) ] E [ (W _ {t _ {i + 1}} - W _ {t _ {i}}) ].\tag{C.257}
$$

But the expectation of $( W _ { t _ { i + 1 } } - W _ { t _ { i } } )$ is zero, and so the summation vanishes and we are left with 

$$
E _ {s} [ X _ {t} ] = X _ {s},\tag{C.258}
$$

which says that $X _ { t }$ is indeed a martingale. 

2. We want to calculate the stochastic diferential equations that are satisfied by $S _ { t } / B _ { t }$ and $\rho _ { t } S _ { t } / B _ { t }$ . Using the division rule for stochastic processes, we see that 

$$
d \left(\frac {S _ {t}}{B _ {t}}\right) = \frac {S _ {t}}{B _ {t}} \left[ \frac {d S _ {t}}{S _ {t}} - \frac {d B _ {t}}{B _ {t}} - \frac {d S _ {t}}{S _ {t}} \frac {d B _ {t}}{B _ {t}} \right].\tag{C.259}
$$

Recall that 

$$
\frac {d S _ {t}}{S _ {t}} = \mu_ {t} d t + \sigma_ {t} d t\tag{C.260}
$$

and 

$$
\frac {d B _ {t}}{B _ {t}} = r _ {t} d t.\tag{C.261}
$$

Subsituting in these values, we see that $d S _ { t } d B _ { t } = 0$ and 

$$
\begin{array}{r c l} d \left(\frac {S _ {t}}{B _ {t}}\right) & = & \frac {S _ {t}}{B _ {t}} \left[ (\mu_ {t} d t + \sigma_ {t} d W _ {t}) - r _ {t} d t \right] \\ & = & \frac {S _ {t}}{B _ {t}} \left[ (\mu_ {t} - r _ {t}) d t + \sigma_ {t} d W _ {t} \right]. \end{array}\tag{C.262}
$$

The second stochastic equation can then be calculated by using the product rule, 

$$
d \left(\frac {\rho_ {t} S _ {t}}{B _ {t}}\right) = \frac {\rho_ {t} S _ {t}}{B _ {t}} \left[ \frac {d (S _ {t} / B _ {t})}{S _ {t} / B _ {t}} + \frac {d \rho_ {t}}{\rho_ {t}} + \frac {d \rho_ {t}}{\rho_ {t}} \frac {d (S _ {t} / B _ {t})}{S _ {t} / B _ {t}} \right].\tag{C.263}
$$

We previously showed that 

$$
\frac {d \rho_ {t}}{\rho_ {t}} = - \lambda_ {t} d W _ {t},\tag{C.264}
$$

where $\lambda _ { t } = ( \mu _ { t } - r _ { t } ) / \sigma _ { t }$ . Using this expression, and the value of $d ( S _ { t } / B _ { t } )$ calculated above, we see that 

$$
\begin{array}{r c l} \frac {d \rho_ {t}}{\rho_ {t}} \frac {d (S _ {t} / B _ {t})}{S _ {t} / B _ {t}} & = & - \lambda_ {t} d W _ {t} [ (\mu_ {t} - r _ {t}) d t + \sigma_ {t} d W _ {t} ] \\ & = & - \lambda_ {t} \sigma_ {t} d t \\ & = & - (\mu_ {t} - r _ {t}) d t. \end{array}\tag{C.265}
$$

The diferential equation for $\rho _ { t } S _ { t } / B _ { t }$ then becomes 

$$
\begin{array}{r c l} d \left(\frac {\rho_ {t} S _ {t}}{B _ {t}}\right) & = & \frac {\rho_ {t} S _ {t}}{B _ {t}} \left[ (\mu_ {t} - r _ {t}) d t + \sigma_ {t} d W _ {t} - \lambda_ {t} d W _ {t} - (\mu_ {t} - r _ {t}) d t \right] \\ & = & (\sigma_ {t} - \lambda_ {t}) \frac {\rho_ {t} S _ {t}}{B _ {t}} d W _ {t}. \end{array}\tag{C.266}
$$

3. The stochastic diferential equation for $\rho _ { t }$ is 

$$
d \rho_ {t} = - \rho_ {t} \lambda_ {t} d W _ {t}.\tag{C.267}
$$

Integrating this, we obtain 

$$
\rho_ {t} = \rho_ {0} - \int_ {0} ^ {t} \rho_ {s} \lambda_ {s} d W _ {s}\tag{C.268}
$$

The initial value of $\rho _ { t }$ is 1, hence 

$$
\rho_ {t} = 1 - \int_ {0} ^ {t} \rho_ {s} \lambda_ {s} d W _ {s}.\tag{C.269}
$$

4. If $\lambda _ { t }$ is constant, then we can evaluate the integrals in the expression for $\rho _ { t }$ in order to obtain 

$$
\rho_ {t} = \exp \left[ - \lambda W _ {t} - \frac {1}{2} \lambda^ {2} t \right],\tag{C.270}
$$

which we can write as 

$$
\rho_ {t} = \rho_ {s} \exp \left[ - \lambda (W _ {t} - W _ {s}) - \frac {1}{2} \lambda^ {2} (t - s) \right].\tag{C.271}
$$

If we calculate the conditional expectation in the risk-neutral measure of $W _ { t } .$ , we see that 

$$
\begin{array}{r c l} E _ {s} ^ {*} [ W _ {t} ] & = & \frac {E _ {s} [ \rho_ {t} W _ {t} ]}{\rho_ {s}} \\ & = & E _ {s} \left[ \exp \left(- \lambda (W _ {t} - W _ {s}) - \frac {1}{2} \lambda^ {2} (t - s)\right) \right. \\ & & \times \left\{(W _ {t} - W _ {s}) + W _ {s} \right\}. \end{array}\tag{C.272}
$$

With respect to the conditioning up to time $s , W _ { s }$ is a constant, and $W _ { t } - W _ { s }$ is an independant $\mathrm { N } ( 0 , t - s )$ random variable. We can calculate the expectation more compactly by defining $\dot { \boldsymbol { X } } = \boldsymbol { W } _ { t } - \boldsymbol { W } _ { s }$ . Hence 

$$
\begin{array}{r c l} E _ {s} ^ {*} [ W _ {t} ] & = & E \left[ X \exp \left(- \lambda X - \frac {1}{2} \lambda^ {2} (t - s)\right) \right] \\ & & + W _ {s} E \left[ \exp \left(- \lambda X - \frac {1}{2} \lambda^ {2} (t - s)\right) \right]. \end{array}\tag{C.273}
$$

<!-- === Source: MinerU_markdown_Financial_Mathematics_201_2122707655893032962.md (Page 201) === -->

We can then calculate the two expectations individually, 

$$
\begin{array}{l} E \left[ X \exp \left(- \lambda X - \frac {1}{2} \lambda^ {2} (t - s)\right) \right] \\ = \frac {1}{\sqrt {2 \pi (t - s)}} \int_ {- \infty} ^ {\infty} x \exp \left(- \lambda x - \frac {1}{2} \lambda^ {2} (t - s)\right) \exp \left(- \frac {x ^ {2}}{2 (t - s)}\right) d x \\ = \frac {1}{\sqrt {2 \pi (t - s)}} \int_ {- \infty} ^ {\infty} x \exp \left(- \frac {[ x + \lambda (t - s) ] ^ {2}}{2 (t - s)}\right) d x \end{array} \tag {C.2}\tag{C.274}
$$

But this is simply the expectation of an $\operatorname { N } ( - \lambda ( t - s ) , ( t - s ) )$ random variable, which is $- \lambda ( t - s )$ . Following the same steps, we see that the second integral is $W _ { s }$ times the integral over the probability density function, which is 1. Thus 

$$
E _ {s} ^ {*} [ W _ {t} ] = - \lambda (t - s) + W _ {s}.\tag{C.275}
$$

The expectation of $W _ { t } ^ { 2 }$ can be calculated in an identical manner. 

5. We want to show that $\Pi _ { t } ^ { C } = \rho _ { t } C _ { t } / B _ { t }$ is a martingale under the measure $E .$ . We can do this by calculating the stochastic diferential and show that it does not have a drift term. Using both the product and division rules for stochastic diferentials, we see that 

$$
d \left(\frac {\rho_ {t} C _ {t}}{B _ {t}}\right) = \frac {\rho_ {t} C _ {t}}{B _ {t}} \left[ \frac {d \rho_ {t}}{\rho_ {t}} + \frac {d C _ {t}}{C _ {t}} + \frac {d \rho_ {t}}{\rho_ {t}} \frac {d C _ {t}}{C _ {t}} - \frac {d B _ {t}}{B _ {t}} \right].\tag{C.276}
$$

The diferential equation for $C _ { t }$ is 

$$
\frac {d C _ {t}}{C _ {t}} = \mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t},\tag{C.277}
$$

and if we substitute this expression, and the stochastic diferentials of $\rho _ { t }$ and $B _ { t }$ given above, into equation (C.276), then we obtain 

$$
d \left(\frac {\rho_ {t} C _ {t}}{B _ {t}}\right) = \frac {\rho_ {t} C _ {t}}{B _ {t}} \left[ - \lambda_ {t} d W _ {t} + (\mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t}) - \lambda_ {t} \sigma_ {t} ^ {C} d t - r _ {t} d t \right].\tag{C.278}
$$

But from the no arbitrage condition we can write $\lambda _ { t }$ as 

$$
\lambda_ {t} = \frac {\mu_ {t} ^ {C} - r _ {t}}{\sigma_ {t} ^ {C}},\tag{C.279}
$$

and hence 

$$
\begin{array}{r c l} d \left(\frac {\rho_ {t} C _ {t}}{B _ {t}}\right) & = & \frac {\rho_ {t} C _ {t}}{B _ {t}} \left[ - \lambda d W _ {t} + (\mu_ {t} ^ {C} d t + \sigma_ {t} ^ {C} d W _ {t}) - (\mu_ {t} ^ {C} - r _ {t}) d t - r _ {t} d t \right] \\ & = & (\sigma_ {t} ^ {C} - \lambda_ {t}) \frac {\rho_ {t} C _ {t}}{B _ {t}} d W _ {t}. \end{array} \tag {6}\tag{C.280}
$$

Thus $\Pi _ { t } ^ { C }$ is a martingale. 

## D Some Reminders of Probability Theory

(by R.F. Streater) 

## D.1 Events, random variables and distributions

An event A is a subset of a space (the sample space Ω); more exactly, A is a measurable subset. We are given the probability $p ( A )$ for all events $A \subseteq \Omega ;$ it is nonnegative, and $p ( \Omega ) = 1$ . We say that two events, $A \subseteq \Omega$ and $B \subseteq \Omega$ are independent if 

$$
p (A \cap B) = p (A) p (B).\tag{D.1}
$$

A random variable is a function $f : \Omega \to \mathbf { R } ;$ more exactly, it is a measurable function. We shall sometimes write r.v. for random variable. If $f$ takes discrete values $\{ x _ { 1 } . x _ { 2 } , . . . \}$ then we can define the distribution function of $f ,$ according to 

$$
p _ {f} (j) = \mathrm{Prob} \{f = x _ {j} \} = p \{\omega : f (\omega) = x _ {j} \}.\tag{D.2}
$$

If $f$ takes continuous values, then the probability that $f$ takes a particular real value might be zero; in that case we can define the cumulative distribution function 

$$
P _ {f} (x) = \operatorname{Prob} \{f \leq x \} = p \{\omega : - \infty <   f (\omega) \leq x \}.\tag{D.3}
$$

We say that a random variable $f$ “has a probability density” if its cumulative distribution is diferentiable; we then define its density to be 

$$
p _ {f} (x) := \frac {d P _ {f} (x)}{d x};\tag{D.4}
$$

and to first order in dx, 

$$
p _ {f} (x) d x = \operatorname{Prob} \{x \leq f \leq x + d x \}\tag{D.5}
$$

and 

$$
\mathrm{Prob} \{a \leq f \leq b \} = \int_ {a} ^ {b} p _ {f} (x) d x\tag{D.6}
$$

The cumulative distribution of the standard normal distribution is denoted $\operatorname { E r f } ( x )$ , or $N ( x )$ in this course. 

## D.2 Expectation, moments and generating functions

The expectation of the random variable $f ,$ defined abstractly by 

$$
E [ f ] := \int f (\omega) p (d \omega)\tag{D.7}
$$

in terms of the measure $p ,$ reduces when the space Ω is discrete, to 

$$
E [ f ] = \sum_ {\omega} f (\omega) p (\omega).\tag{D.8}
$$

Exercise D.1 Show that when $\Omega$ is discrete, the mean can be found in terms of the probability distribution $p _ { f }$ of f and the values $x _ { j }$ of f according to 

$$
E [ f ] = \sum_ {j} x _ {j} p _ {f} (j).\tag{D.9}
$$

In the continuous case, it can be shown that 

$$
E [ f ] = \int_ {- \infty} ^ {\infty} x p _ {f} (x) d x.\tag{D.10}
$$

The n-th moment, $m _ { n } ( f )$ of the r.v. $f ,$ is defined to be 

$$
m _ {n} (f) := E [ f ^ {n} ]\tag{D.11}
$$

which in the discrete case gives 

$$
m _ {n} = \sum_ {\omega} (f (\omega_ {j})) ^ {n} p (\omega) = \sum_ {j} x _ {j} ^ {n} p _ {f} (j);\tag{D.12}
$$

in the continuous case we get 

$$
m _ {n} = E [ f ^ {n} ] = \int_ {- \infty} ^ {\infty} x ^ {n} p _ {f} (x) d x.\tag{D.13}
$$

It is clear that $m _ { 1 } ( f )$ is the expectation of $f ;$ it is not hard to show 

Exercise D.2 The variance of $f _ { i }$ , defined by 

$$
V [ f ] := E [ (f - m _ {1}) ^ {2} ],\tag{D.14}
$$

is given by $V [ f ] = m _ { 2 } - m _ { 1 } ^ { 2 }$ 

The moment generating function is defined as 

$$
M (\theta) := \sum_ {n = 0} ^ {\infty} \frac {\theta^ {n}}{n !} m _ {n} = \sum_ {n} E [ f ^ {n} ] \theta^ {n} / n! = E [ e ^ {\theta f} ].\tag{D.15}
$$

This definition is only possible when the series converges, say for $| \theta |$ small. In that case, by Taylor’s theorem, M determines the moments: 

$$
m _ {n} = \left. \frac {d ^ {n} M}{d \theta^ {n}} \right| _ {\theta = 0}.\tag{D.16}
$$

It can be shown that M also determines the probability distribution of $f ;$ indeed, $m _ { n }$ is determined by $p _ { f } ( x )$ , according to eqs. (D.12,D.13); in the latter case, M is the Laplace transform of $p _ { f }$ : 

$$
M (\theta) = \int_ {- \infty} ^ {\infty} e ^ {\theta x} p _ {f} (x) d x;\tag{D.17}
$$

(if the integral converges); it follows that $p _ { f } ( x )$ is the inverse Laplace transform of M. 

Exercise D.3 Let f be $N ( m , V )$ ; that is, 

$$
p _ {f} (x) = \frac {1}{(2 \pi V) ^ {1 / 2}} \exp \{- \frac {(x - m) ^ {2}}{2 V} \};\tag{D.18}
$$

Show that m is the expectation (the first moment) and that V is the variance of $f$ . 

Exercise D.4 Find the n-th moments of a standard normal $r . v .$ , with distribution $N ( 0 , 1 )$ 

## D.3 Several random variables

In terms of the sample space, Ω, two random variables $f ,$ and ${ \mathit { g } } ,$ are just two functions on Ω. Given a probability on $\Omega$ , each will have its own distribution, $p _ { f }$ and $p _ { g }$ . In order to discuss the correlation between these, we should consider the joint distribution. In the case of r.v. with discrete values, $\{ x _ { j } \} , \{ y _ { k } \}$ , say, the joint distribution of $f$ and $g$ is defined as 

$$
p _ {f, g} (j, k) = \operatorname{Prob} \{\omega : f (\omega) = x _ {j} \text { and } g (\omega) = y _ {k} \}.\tag{D.19}
$$

We say that two r.v., f and $^ { g , }$ are independent if the pairs of events, A and B, of the form 

$$
A = \{\omega \in \Omega : a <   f (\omega) \leq b \}\tag{D.20}
$$

$$
B = \{\omega \in \Omega : c <   g (\omega) \leq d \}\tag{D.21}
$$

are independent for all real numbers $a , b , c , d ;$ see eq. (D.1). 

Exercise D.5 Show that if both f and g take discrete values, then they are independent if and only if 

$$
p _ {f, g} (j, k) = p _ {f} (j) p _ {g} (k), \text {   for   all   } j, k.\tag{D.22}
$$

If both f and g take continuous values, we can define the joint cumulative distribution function $P _ { f , g }$ to be 

$$
P _ {f, g} (x, y) := \operatorname{Prob} \{\omega \in \Omega : f (\omega) \leq x \text { and } g (\omega) \leq y \}.\tag{D.23}
$$

If $P _ { f , g }$ is diferentiable with respect to x and y, we say that f and g have a joint density function, which is defined to be 

$$
p _ {f, g} (x, y) := \frac {\partial^ {2} P _ {f , g}}{\partial x \partial y}.\tag{D.24}
$$

Then the probability that f lies between x and $x + d x$ , and simultaneously g lies between y and $y + d y$ , is, to second order 

$$
\operatorname{Prob} \{\omega \in \Omega : x \leq f (\omega) \leq x + d x \text {and} y \leq g (\omega) \leq y + d y \} = p _ {f, g} (x, y) d x d y.\tag{D.25}
$$

Again, f and g are independent if and only if 

$$
p _ {f, g} (x, y) = p _ {f} (x) p _ {g} (y) \quad \text {   for   all   } x, y.\tag{D.26}
$$

The correlation between f and g is defined as 

$$
\mathcal {C} (f, g) = E [ f g ] - E [ f ] E [ g ].\tag{D.27}
$$

Exercise D.6 If f and g have discrete values, and are independent, show that the correlation between them is zero. Show the same, if f and g have a joint density. 

It is not in general true that uncorrelated r.v. are independent. However, if $f$ and $g$ are jointly normal, then they are independent if and only if they are uncorrelated. We say that the r.v. f and $g$ are jointly normal if they have a joint density, and it is given by a function of the form 

$$
p _ {f, g} (x, y) = c o n s t. \exp \{- \alpha x ^ {2} + \beta x y - \gamma y ^ {2} + a x + b y \}.\tag{D.28}
$$

Here, $\alpha > 0 , \gamma > 0$ , and $\beta$ must be such that the quadratic expression tends to zero at infinity in all directions; a and b are any real numbers, and the constant is such that the total integral over $\mathbf { R } ^ { 2 }$ is unity. 

The joint $n , r$ moment of $f$ and $g$ is defined to be 

$$
m _ {n, r} = E [ f ^ {n} g ^ {r} ], n = 0, 1, 2 \dots ; r = 0, 1, 2, \dots .\tag{D.29}
$$

$\vdots$ From this we can define the joint moment generating function to be 

$$
M _ {f, g} (\theta_ {1}, \theta_ {2}) = \sum_ {n, r = 0} ^ {\infty} \theta_ {1} ^ {n} \theta_ {2} ^ {r} / (n! r!) m _ {n, r}.\tag{D.30}
$$

Exercise D.7 Suppose that f and g are independent, with either discrete values, or with a joint density. Show that 

$$
M _ {f, g} (\theta_ {1}, \theta_ {2}) = M _ {f} (\theta_ {1}) M _ {g} (\theta_ {2}) \quad \text {   for   all   } \quad \theta_ {1}, \theta_ {2}.\tag{D.31}
$$

Also, show the converse. 

Exercise D.8 Let f and g be independent, with either discrete value $o r$ a joint density. Show that the r.v $f + g$ has generating function $M _ { f + g }$ given by 

$$
M _ {f + g} (\theta) = M _ {f} (\theta) M _ {g} (\theta).\tag{D.32}
$$

Exercise D.9 Show that the joint moment generating function of the jointly normal r.v. f and g is the exponential of a quadratic function of $\theta _ { 1 }$ and $\theta _ { 2 } ,$ conversely, if the joint moment generating function is the exponential of a quadratic function of $\theta _ { 1 }$ and $\theta _ { 2 }$ , then the r.v. are jointly normal. 

Exercise D.10 Let S be the sum $f + g$ of jointly normal r.v f and $g ;$ show that S is normal. 

We can consider n random variables $f _ { 1 } , \ldots , f _ { n }$ , with joint probability density $p _ { 1 , \dots n } ( x _ { 1 } , \dots , x _ { n } )$ . This means that each $f _ { j }$ takes continuous values, and that 

$$
\begin{array}{r c l} \text {Prob} \{\omega \in \Omega : a _ {1} & \leq & f _ {1} (\omega) \leq b _ {1} \text {and} \ldots \text {and} a _ {n} \leq f _ {n} (\omega) \leq b _ {n} \} \\ & = & \int_ {a _ {1}} ^ {b _ {1}} \ldots \int_ {a _ {n}} ^ {b _ {n}} p _ {1 \ldots n} (x _ {1}, \ldots , x _ {n}) d x _ {1} \ldots d x _ {n}. \end{array}
$$

We say that $\{ f _ { k } \}$ are jointly normal if the density has the form 

$$
p (x _ {1}, \dots , x _ {n}) = c o n s t. \exp \{- \frac {1}{2} x. A. x ^ {T} + x. c ^ {T} \}\tag{D.33}
$$

for some positive definite $n \times n$ matrix $A$ , and some row vector $c = ( c _ { 1 } , \ldots , c _ { n } )$ Here we have written x as a $1 \times n$ row vector, and $x ^ { \overset { T } { \doublebarwedge } }$ is its transpose, the column vector. 

Exercise D.11 Let $f _ { k } , k = 1 , \dots , n$ be n jointly normal $r . v .$ Show that the joint moment generating function 

$$
M (\theta_ {1}, \dots , \theta_ {n}) := E [ e ^ {\theta_ {1} f _ {1} + \dots + \theta_ {n} f _ {n}} ]\tag{D.34}
$$

is the exponential of a quadratic expression in $\{ \theta _ { k } \}$ . [Hint: Show first that by a suitable choice of $\alpha _ { 1 } , \ldots , \alpha _ { n }$ we can change the variable of integration from $x _ { 1 } , \ldots x _ { n }$ to $y _ { 1 } = x _ { 1 } + \alpha _ { 1 } , \ldots , y _ { n } = x _ { n } + \alpha _ { n }$ , in such a way that the new density, as a function of $\left\{ y _ { k } \right\}$ , has the form 

$$
p (y) = c o n s t. \exp \{y. A. y ^ {T} \}.\tag{D.35}
$$

Then, write $\boldsymbol { A } = \boldsymbol { S } \boldsymbol { S } ^ { T }$ in terms of suitable matrices $S ,$ and change the variable of integration to $z = y S . \jmath$ 

## D.4 Conditional probability and expectation

Suppose that Ω is the sample space, and p a given probability on $\Omega ,$ so that $p ( A )$ is given for every event $A \subseteq \Omega$ . Suppose that we are told that the outcome $\omega$ lies in some subset B, but we are told no further information. Bayes said the probability that $\omega$ lies in the set $A \subseteq \Omega$ is modified by the information we have obtained; $p ( A )$ should be replaced by the conditional probability, given $B .$ , written $p ( A | B )$ , where 

$$
p (A | B) := p (A \cap B) / p (B).\tag{D.36}
$$

The definition requires that $p ( B ) \neq 0$ . Notice that $p ( A | B )$ is itself a probability on Ω; that is, for $A \subseteq \Omega$ , we have 

$$
p (A | B) \geq 0\tag{D.37}
$$

$$
p (\Omega | B) = 1\tag{D.38}
$$

$$
p (A _ {1} \cup A _ {2} | B) = p (A _ {1} | B) + p (A _ {2} | B) - p (A _ {1} \cap A _ {2} | B)\tag{D.39}
$$

By restricting, $p ( \omega | B )$ is a probability on B. 

If it happen that A and B are independent, then $p ( A \cap B ) = p ( A ) p ( B )$ and from eq. (D.36) we see that $p ( A | B ) \ = \ p ( B )$ . Thus in this case no information about A is contained in the occurrence of the event $B ,$ and it makes no diference to the probability of A whether we know $B$ or not. 

Another case of interest is when $A \subseteq B ;$ then $A \cap B = A$ , and we see: 

$$
p (A | B) = p (A) / p (B)\tag{D.40}
$$

which obviously gives 

$$
p (A) = p (A | B) p (B).\tag{D.41}
$$

This product structure does not express the independence of A and $B ;$ indeed, in this case A implies B, so they cannot be independent. 

We have in mind that Ω consists of the set of price histories from $t = 0 .$ and we are given the price at some later time, say $t = 1$ . This information, not available at $t = 0$ , increases our information and modifies the probability we assign to the remaining possibilities. Suppose that we have two timesteps, as in the figure: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/38cca223-57dc-4335-9bd7-1c3768e8bd36/d69137684e0e0a300b42a6a8d8a7f33aaaa8eefb44c9fab4e6fdde3b70be3147.jpg)


(D.42) 

The possible paths can be labelled by the symbols $\{ S ^ { 0 0 } , S ^ { 0 1 } , S ^ { 1 0 } , S ^ { 1 1 } \}$ as usual. Remember that there are four possible price histories, even if numerically $S ^ { 0 1 } = S ^ { 1 0 }$ , as in the binomial model. For this reason, we keep the symbols distinct. Thus, $\Omega = \{ 0 0 , 0 1 , 1 0 , 1 1 \}$ , and has four elements. Suppose we learn that at time $t = 1$ the price went up to $S ^ { 0 }$ , rather that going down to $S ^ { 1 }$ . Then only the paths $S ^ { 0 0 }$ and $S ^ { 0 1 }$ are possible. Thus, this information on the price at $t = 1$ means that the outcome must lie in the set $B = \{ 0 0 , 0 1 \}$ shown, and our new probabilities are 

$$
p (\{0 0 \} | S ^ {0}) = p ^ {0 0}, \qquad \mathrm{say}\tag{D.43}
$$

$$
p (\{0 1 \} | S ^ {0}) = p ^ {0 1}, \qquad \mathrm{say}.\tag{D.44}
$$

The two possible outcomes, 00 and 01 are subsets of $B ,$ the given event; the original probability, $p ,$ at $t = 0$ before we had any info, can then got from eq. (D.41), and is thus: 

$$
p (\omega = 0 0) = p (S ^ {0}) p (0 0 | S ^ {0}) = p ^ {0} p ^ {0 0}\tag{D.45}
$$

$$
p (\omega = 0 1) = p (S ^ {0}) p (0 1 | S ^ {0}) = p ^ {0} p ^ {0 1}.\tag{D.46}
$$

In the same way, if we knew that $S ^ { 1 }$ occurred at $t = 1$ we introduce the conditional probabilities 

$$
p (\{1 0 \} | S ^ {1}) = p ^ {1 0} \quad \text { say }\tag{D.47}
$$

$$
p (\{1 1 \} | S ^ {1}) = p ^ {1 1} \mathrm{say};\tag{D.48}
$$

then the original probabilities of 10 and 11 are given by eq. (D.41): 

$$
p (\omega = 1 0) = p (S ^ {1}) p (1 0 | S ^ {1}) = p ^ {1} p ^ {1 0}\tag{D.49}
$$

$$
p (\omega = 1 1) = p (S ^ {1}) p (1 1 | S ^ {1}) = p ^ {1} p ^ {1 1}.\tag{D.50}
$$

These are the formulae we used to find the probability of the prices at time $t = 2$ 

Consider now three steps of the time. If we are given that the pricehistory went through $S ^ { 0 }$ at time $t = 1$ , and were also told the step taken at time $t = 2$ , the later info must be compatible with that earlier. Thus the position at time $t = 2$ must be either 00 or 01. Say it is 00. Then the info at time $t = 1$ is summarised by saying that $\omega \in B$ in the figure below, and the info at time $t = 2$ further restricts the path to lies in the set $C \subseteq B$ . Then we see that $A \cap C = A \cap B \cap C$ , and so for any event A, 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/38cca223-57dc-4335-9bd7-1c3768e8bd36/82d8300f5138c84eb104865cff85c9a5c47bfe2440d28924ffe1fcc154e03360.jpg)


(D.51) 

$$
\begin{array}{r c l} p (A | C) & = & p (A \cap B \cap C) / p (C) = p (A \cap B \cap C)) / p (B) p (C | B) \\ & = & p (A \cap C | B) / p (C | B) = p ((A | B) | C) \end{array}\tag{D.52}
$$

The last expression, $p ( ( A | B ) | C )$ , is the conditioning of the (conditional) probability $p ( \bullet | B )$ , by the info $\omega ~ \in ~ C$ . We see from it that if $B = C$ $p ( ( A | B ) | B ) = p ( A | B )$ , so the giving of known info does not alter the probability. More generally, we see that we get the same result, $p ( A | C )$ , whether we feed the info in two steps, conditioning as we go, or just use the full info in one step. 

The conditional expectation $E [ f | B ]$ of a r.v. f, given $B _ { : }$ is just the expectation of $f$ using a conditional probability $p ( \omega | B )$ . Thus, in the discrete case, 

$$
E [ f | B ] = \sum_ {\omega} f (\omega) p (\omega | B) = \sum_ {j} x _ {j} \sum_ {\omega : f (\omega) = x _ {j}} p (\omega | B).\tag{D.53}
$$

The expression 

$$
p _ {f} (j | B) := \sum_ {\omega : f (\omega) = x _ {j}} p (\omega | B)\tag{D.54}
$$

is called the conditional probability distribution of $f ,$ given B. It enables us to compute all the conditional moments of $f$ . 

In the above example, we determined the set $B _ { ; }$ , on which we condition, by giving the value of the r.v. $S _ { 1 }$ , and we got the set $C$ by giving the values of the two r.v. $S _ { 1 }$ and $S _ { 2 }$ . More generally, we can condition a probability $p$ by giving the values of a collection of random variables $f _ { 1 } , \ldots , f _ { N }$ . Thus, in the discrete case, 

$$
p (\omega | f _ {1} = x _ {1}, f _ {2} = x _ {2}, \ldots , f _ {N} = x _ {N}) = \frac {p (\omega)}{\sum_ {\omega : f _ {1} (\omega) = x _ {1} \ldots f _ {N} (\omega) = x _ {N}} p (\omega)}\tag{D.55}
$$

if $\omega$ obeys the condition, and is zero otherwise. As before, we get the same result whether we use this definition, or condition $p$ in stages, using the info one bit at a time in any order. In the discrete case this is just limiting the sum on the r.h.s. of eq. (D.55) a bit at a time. 

In the continuous case, we talk of conditional density functions. If we have a joint probability density $p ( x _ { 1 } , x _ { 2 } , \ldots , x _ { n } )$ for n random variables $f _ { 1 } , \ldots , f _ { n } $ with continuous values, then a condition such as $f _ { 1 } = X _ { 1 }$ leads to the conditional density, which is obtained by putting $x _ { 1 } = X _ { 1 }$ in the joint density $p ,$ and dividing by a normalising factor: 

$$
p (x _ {2}, x _ {3}, \dots , x _ {n} | f _ {1} = X _ {1}) = \frac {p (X _ {1} , x _ {2} , \dots , x _ {n})}{\int p (X _ {1} , x _ {2} , \dots , x _ {n}) d x _ {2} d x _ {3} \dots d x _ {n}}.\tag{D.56}
$$

Similarly, we can condition on any subcollection of $f _ { 1 } , \ldots , f _ { n }$ 

The conditional expectation $E [ f | f _ { 1 } \ = \ X _ { 1 } , f _ { 2 } \ = \ X _ { 2 } , . . . , f _ { N } ]$ written $E [ f | \{ f _ { i } \} ]$ , is clearly a function of $X _ { 1 } , \ldots , X _ { n }$ . These must be possible values of these r.v.; that is, there must be a point $\omega \in { \Omega }$ such that $f _ { k } ( \omega ) = X _ { k }$ for $k = 1 \ldots N$ . As we vary ω, we get diferent conditionings. From this point of view, we can leave the values open, and consider the conditional expectation $E [ f | f _ { 1 } , \dots , f _ { _ { N } } ]$ as a function of $\omega .$ . That is, it is a random variable! $\mathrm { A s }$ we vary f too, we get diferent random variables for $E [ f | f _ { 1 } , \dots , f _ { _ { N } } ]$ . So, $E [ \bullet | \{ f _ { i } \} ]$ is an operator that takes the random variable $f$ to the random variable $E [ f | \{ f _ { i } \} ]$ . It is clear that the map $f \mapsto E [ f | \{ f _ { i } \} ]$ is linear in the variable $f ;$ it is also true that $E [ g | \{ f _ { i } \} ] = g$ , for all $g$ in the span of $\{ f _ { i } \}$ (exercise). We have seen that the giving of known info does not alter a probability already conditioned to it. This leads to the nice result that the conditional expectation relative to a given set of functions is a projection: applied twice to a random variable it gives the same result as applying it once (exercise). Moreover, applying it twice, once with a large amount of info, and then with a smaller amount, is the same as applying it with the smaller amount. This is because E is the projection onto the algebra generated by the functions listed in the conditions. In particular, the ordinary expectation can be thought of as $E [ f | 1 ]$ ], where 1 is the non-random function 1; clearly, $E [ f ]$ is the trivial function of $\omega$ . Thus 

Exercise D.12 Suppose that Ω is discrete, and that f and $f _ { 1 } , \ldots , f _ { n }$ are random variables on Ω. Show that for any probability $p ,$ we have 

$$
E [ E [ f | \{f _ {i} \} ] ] = E [ f ].\tag{D.57}
$$

## D.5 Filtrations and martingales

Most of this section will be new to you. 

The prices of various stocks, S, and of currencies, and gold, and of bonds, and other assets, become known to us, first at $t = 1$ , then at $t = 2$ , up to the present time, $t = t$ . It is clear that as t increases, we are in possession of an increasing amount of info. According to Bayes, we should condition our probability as we $\mathrm { g o }$ . We have seen that we do not in general know the actual probability that the share will go up, or down; but the correct price of a derivative has been seen to be expressible in terms of the risk-neutral probabilities, rather than the actual market probabilities. So we shall find it useful to develop the theory of conditioning for various probabilities on the sample space, any of which is to be modified by the info we have at any given time. 

Let us limit our info to the price of a single share, $S ,$ and consider the binomial model up to time $T .$ . Then the number of distinct price-histories is $2 ^ { T }$ . So $\Omega$ has $2 ^ { \hat { T } }$ points. Let $p$ be any probability on $\Omega$ . Suppose that at time $t ,$ with $t < T$ , we have the price-history of S up to time t. This means that we can calculate the actual value of any derivative stock option that depends only on the past values. Such a derivative will be a function $F$ of $S _ { 0 } , S _ { 1 } , \ldots , S _ { t }$ . And for such a function, the conditional expectation relative to $p ( \omega | S _ { 0 } , \ldots , S _ { t } )$ , using all the information, must be the actual value: 

$$
E [ F | S _ {0}, S _ {1}, \ldots , S _ {t} ] = F (S _ {0}, S _ {1}, \ldots , S _ {t}).\tag{D.58}
$$

Thus $E [ \bullet | S _ { 0 } , \ldots , S _ { t } ]$ leaves invariant not only the random variables $S _ { 0 } , \ldots , S _ { t }$ but all functions of these; this is because we have full information about all such functions. The set of all (measurable) functions of $S _ { 0 } , \ldots , S _ { t }$ is an $a l -$ gebra; that is, we can add and multiply such functions, and multiply them by real numbers, to get further functions in the set. These are all functions of $\omega .$ , since each r.v. $S _ { 0 } \ldots$ . is itself a function of $\omega .$ . Let us call this set $\mathcal { F } _ { t }$ Now, a function $F _ { 1 }$ say, of the variables $S _ { 0 } , \ldots , S _ { t - 1 }$ is also a function of $S _ { 0 } , \ldots , S _ { t - 1 } , S _ { t }$ , which happens not to depend on the last variable. So such a function is in $\mathcal { F } _ { t }$ . Thus we have that $\mathcal { F } _ { t - 1 } \subseteq \mathcal { F } _ { t }$ , and more generally, 

$$
\text { if   } s \leq t \text {   we   have   } \mathcal {F} _ {s} \subseteq \mathcal {F} _ {t}.\tag{D.59}
$$

This increasing family of function algebras, $\mathcal { F } _ { t }$ , is called the filtration generated by the process $S _ { t }$ . Sometimes it is more convenient to consider the indicator functions in the family. An indicator function is one that takes only two values, 0 or 1. The set on which it is equal to 1 is a subset of $\omega ,$ that is, an event, and knowing the value of this function (as we do by the time t) tells us whether this event has happened. Conversely, any function in $\mathcal { F } _ { t }$ can be written as a sum of indicator functions, with real coeficients. The information in the filtration can be regarded as a family of events whose occurence (or not) is known by the time t. This family of events is sometimes also called the filtration, and is denoted by $\mathcal { F } _ { t }$ as well. It is likewise an increasing family, as time increases. In either case, the conditional expectation of a random variable, $f$ given all the information up to time $t ,$ is denoted $E [ f | \mathcal { F } _ { t } ]$ 

## Martingales

Suppose that Ω is a sample space, and p a probability on $\Omega .$ . Let $\mathcal { F } _ { t }$ be the filtration generated by a process $S _ { t }$ . Let $X _ { t }$ be a process adapted to the filtration, that is, at any time $t \ X _ { t }$ is known if the price-history of $S _ { t }$ is known; this is nothing other than the condition that $X _ { t } ~ \in { \mathcal { F } } _ { t }$ for any t. Thus, $X _ { t }$ is some derivative based on the share price of $S _ { s }$ , involving only $s \leq t$ . We say that $X _ { t }$ is a martingale if it obeys 

$$
E [ X _ {t} | \mathcal {F} _ {s} ] = X _ {s}, \text {   for   all   } s \leq t.\tag{D.60}
$$

This says in a way that the present value of the derivative $X _ { s }$ is the expected value at any t in the future, given the known past history up to time s of the share $S$ on which the derivative is based. As an example of a martingale, let Y be any random variable. Then put $X _ { t } ~ = ~ E [ Y | \mathcal { F } _ { t } ]$ If $s \ \leq \ t$ , the family $\mathcal { F } _ { s }$ is smaller than the family $\mathcal { F } ^ { t }$ , (or the same); then we may use the principle that double conditioning, as given by eq. (D.57), gives the same as one conditioning onto the smaller algebra; indeed, eq. (D.57) is true whatever the initial probability was, so we may use it starting with the conditioned probability at time $s ;$ then we see that $X _ { t }$ is a martingale: 

$$
E [ X _ {t} | \mathcal {F} _ {s} ] = E [ E [ Y | \mathcal {F} _ {t} ] | \mathcal {F} _ {s} ] = E [ Y | \mathcal {F} _ {s} ] = X _ {s}.\tag{D.61}
$$

The martingale condition is a condition on the probability $p$ as well as on the process $X _ { t }$ . In our treatment of the pricing problem, in the binomial model, we saw that $S _ { t } / B _ { t }$ is $\mathrm { a }$ martingale, not relative to the (unknown) true probability of prices, but relative to the risk-free probability, $p _ { * }$ : 

$$
S _ {0} / B _ {0} = E ^ {*} [ S _ {1} / B _ {1} | S _ {0} ] = E ^ {*} [ S _ {2} / B _ {2} | S _ {0} ] = \dots\tag{D.62}
$$

In the model, all probabilities were conditional on the price $S _ { 0 }$ being given. But this is any starting time, so calling the starting time s instead of $0 ,$ shows that we have a martingale. In the same way, the pricing formula for any derivative at time $t ,$ in the binomial model, is a martingale, relative to the risk-free probabilitiy, $p _ { * }$ 

## E The Virtues and Vices of Options1

A rather marked feature in the Stock Exchange recently has been the revival of “option” dealing. In years gone by, a considerable amount of business was habitually transacted in “options,” especially in Consols, but more recently this species of speculation had dwindled down to very restricted dimensions. But at no period has it ever been as popular as it is on the continental bourses, and on the stock exchanges across the Atlantic. At Paris, and on all the German bourses, there is a vast amount of speculation constantly carried on by means of options, not separate from, but ancillary to direct operations for the rise or fall. In New York “options” or “privileges” are also a very favourite form of speculation, and that the means for indulging in it have been abundant, is evidenced by the fact that Mr Russell Sage, the well known associate of Mr Jay Gould, who was, until the collapse of May, 1884, one of the wealthiest and most powerful manipulators in Wall Street, has always been a great dealer in “stock privileges.” It is dificult to understand why options have so far not been acclimatised in England, but in view of their becoming more popular, it may be well to refer to their advantages and disadvantages from an outside standpoint. 

An “option” is the price paid for the right to demand or to deliver a certain amount of stock at a given price within a certain definite period. The prices given for this “option” may, of course, range infinitely, according to the supposed value of the elements of which it is composed. The right to demand a stock is termed the “call,” and the right to deliver it the “put.” For instance, one may pay to-day, say, 2 per cent for the “call” a month hence of 1,000l Russian 1873, which right may or may not be exercised. And a “put” would be exactly the converse of this. It is possible to buy the double privilege of both “put” and “call,” but the price asked is usually so heavy as to be practically prohibitive. Now, the idea of the speculator who dabbles a little in option is simply to buy the “put” or “call,” according to whether he thinks the market will fall or rise; whereas their real raison d’etre is something altogether diferent. They should always serve as a protection to other operations. For instance, a speculator becomes a “bear” of, say, 10,000l Russian 1873, and buys the “call” of the same amount of stock. If the price falls, as he anticipates, the profits which he realises are reduced by the amount paid for the “call.” On the other hand, if the stock rises, no matter how much, he can “call” the same amount of stock as that sold at presumably the same price, which liquidates the stock sold, leaving him only the premiums paid for the “call” out of pocket. It is, of course, evident that an “option” often afords protection not to one, but to a series of operations. Moreover, the holder of an “option,” using it this way, may finally find it to his advantage to close all operations for which it acted as protection, and using, say, the “call” in a direct manner, turn over from the “bear” side to the “bull” side of the market. An “option” used properly therefore afords ample scope for skilful speculation, while no loss can be incurred beyond the premium paid in the first instance. But when a speculator who dabbles a little in this sort of business just buys the “put” or “call,” and, as it is termed, “sits upon it,” he simply plays a losing game, for his operations for the fall or rise, which would be sufficiently weighted in the case of a purchase or sale by his own inexperience, and by the expenses of commission &c., are now burdened by the heavy prices paid for the option itself. In fact, the charges are probably multiplied ten fold against him. It is true that the loss is limited, but then the propect of a profit is reduced almost to the vanishing point. On the other hand, “options” capably used not only limit the loss, but ofer a fair chance of making a profit. They are, in fact, an excellent medium for clever, yet cautious operators. From what we have said, it will be seen that those who advise people to buy “options,” without taking any other measures, are simply considering their own interests, the more especially as the securities often recommended are those which are extremely unlikely to fluctuate to the extent of the given premium—the latter frequently remaining in the hands of the broker, or so-called “broker,” as something of a much more satisfactory nature than any commission. 

From the standpoint of business morality, two things may be adduced in connection with “options,” one for and one against. In the first place, they foster a form of speculation which already flourishes too abundantly. They do this not only directly, but also indirectly, as owing to the way in which they limit loss, they encourage people to speculate in stocks and shares who otherwise would be restrained, not so much by a positive prudence as by a negative timidity. But it is evident that one can be as efectually destroyed by a poison taken in regular and known quantities, as by a large draught taken heedlessly. It is only a question of time—both methods are equally certain. On the other hand, used by experienced speculators, “options” are generally great safeguards against unexpected and violent movements in prices, and hence in times like the present (speculation being a fact which must simply be acknowledged and dealt with) they are entitled to some commendation. As a matter of fact, speculation in stocks and shares at the present time is for most people gambling of an ultra-violent character, and is only tolerable when protected in the way described. 

## F KCL 1998 Exam

## F.1 Question

In one time-step of the binomial model, a share-price, initially (at time $t =$ 0) equal to $S _ { 0 }$ , moves up to $S _ { 1 } ^ { 0 }$ with probability $p ^ { 0 } > 0$ or down to $S _ { 1 } ^ { 1 }$ with probability $p ^ { 1 }$ . In the same time-interval, a unit in the money market increases from $B _ { 0 } = 1$ to $B _ { 1 }$ . A dealer contracts at time $t = 0$ to pay an investor $f ( S _ { 1 } ^ { i } ) \ ( i = 0 \ \mathrm { o r } \ i = 1 $ , whichever turns out) at time $t = 1$ , where $f$ is a specified function. The dealer hedges this derivative against the underlying, so that the outcome is not subject to risk, and so that no profit or loss is made on the deal. 

a) Show that the hedge ratio must be 

$$
\delta = \frac {f (S _ {1} ^ {0}) - f (S _ {1} ^ {1})}{S _ {1} ^ {0} - S _ {1} ^ {1}}.\tag{F.63}
$$

b) Show that the dealer must invest 

$$
\beta = \frac {f (S _ {1} ^ {1}) S _ {1} ^ {0} - f (S _ {1} ^ {0}) S _ {1} ^ {1}}{B _ {1} (S _ {1} ^ {0} - S _ {1} ^ {1})}\tag{F.64}
$$

in the money market. 

c) Show that the price of the option must be 

$$
f = f (S _ {1} ^ {0}) \frac {S _ {0} - S _ {1} ^ {1} / B _ {1}}{S _ {1} ^ {0} - S _ {1} ^ {1}} + f (S _ {1} ^ {1}) \frac {S _ {1} ^ {0} / B _ {1} - S _ {0}}{S _ {1} ^ {0} - S _ {1} ^ {1}}\tag{F.65}
$$

d) Use a no-arbitrage argument to show that $S _ { 0 } - S _ { 1 } ^ { 1 } / B _ { 1 } > 0$ 

## F.1.1 Solution

(a) The dealer must buy δ shares and invest $\beta$ in the money market, so that he has $\delta S _ { 0 } + \beta B _ { 0 }$ at time $t = 0$ and $\delta S _ { 1 } + \beta B _ { 1 }$ at time $t = 1$ . He has an obligation $f ( S _ { 1 } )$ at time $t = 1$ . The risky part of the dealers assets is 

$$
\delta S - f (S)
$$

The condition for no risk is that this take the same value whether $i = 0$ or $i = 1$ . This gives 

$$
\delta S _ {1} ^ {0} - f (S _ {1} ^ {0}) = \delta S _ {1} ^ {1} - f (S _ {1} ^ {1}).
$$

Solving, we get for the hedge ratio: 

$$
\delta = \frac {f (S _ {1} ^ {0}) - f (S _ {1} ^ {1})}{S _ {1} ^ {0} - S _ {1} ^ {1}}.
$$

b) 

Put this value in the formula for the dealer’s assets at time 1, which must cover the obligation $f ( S _ { 1 } )$ , we get, for $S _ { 1 } = S _ { 1 } ^ { 1 }$ say 

$$
f (S _ {1}) = \delta S _ {1} ^ {1} + \beta B _ {1}
$$

the value for $\beta \colon$ 

$$
\begin{array}{r c l} B _ {1} \beta & = & f (S _ {1} ^ {1}) - \frac {f (S _ {1} ^ {0}) - f (S _ {1} ^ {1})}{S _ {1} ^ {0} - S _ {1} ^ {1}} S _ {1} ^ {1} \\ & = & \frac {f (S _ {1} ^ {1}) S _ {1} ^ {0} - f (S _ {1} ^ {1}) S _ {1} ^ {1} - f (S _ {1} ^ {0}) S _ {1} ^ {1} + f (S _ {1} ^ {1}) S _ {1} ^ {1}}{S _ {1} ^ {0} - S _ {1} ^ {1}} \\ & = & \frac {f (S _ {1} ^ {1}) S _ {1} ^ {0} - f (S _ {1} ^ {0}) S _ {1} ^ {1}}{S ^ {0} - S ^ {1}} \end{array}
$$

Putting this in for the value of the derivative at time 0 gives 

$$
f _ {0} = \frac {f (S _ {1} ^ {1}) S _ {1} ^ {0} - f (S _ {1} ^ {0}) S _ {1} ^ {1}}{B _ {1} (S _ {1} ^ {0} - S _ {1} ^ {1})} + \frac {f (S _ {1} ^ {0}) - f (S _ {1} ^ {1})}{S _ {1} ^ {0} - S _ {1} ^ {1}} S _ {0},
$$

since $B _ { 0 } = 1$ . Rearranging, we get 

$$
f _ {0} = f (S _ {1} ^ {0}) \frac {S _ {0} - S _ {1} ^ {1} / B _ {1}}{S _ {1} ^ {0} - S _ {1} ^ {1}} + f (S _ {1} ^ {1}) \frac {S _ {1} ^ {0} / B _ {1} - S _ {0}}{S _ {1} ^ {0} - S _ {1} ^ {1}}.
$$

d) 

If $S _ { 0 } B _ { 1 } - S _ { 1 } ^ { 1 } \leq 0$ , then the lower of the two possible prices at time 1 is larger than the initial price plus interest. So the arbitrageur will buy the share at $t = 0$ for $S _ { 0 }$ , borrowing $S _ { 0 }$ to do this. His debt grows to $S _ { 0 } B _ { 1 }$ . He then sells his share at a price $S _ { 1 } ^ { 0 }$ or $S _ { 1 } ^ { 1 }$ , both $\geq$ than his debt. Since $p ^ { 0 } > 0$ , he has a non-zero chance to make money at no risk of a loss, and would therefore follow this course. 

## F.2 Question

Let $W _ { t }$ denote the Wiener process. 

a) State the Ito rules for the second-degree infinitesimals $( d t ) ^ { 2 }$ , (dt)(dW) and $( d W ) ^ { 2 }$ 

b) Show that $W _ { t }$ and $W _ { t } ^ { 2 } - t$ are martingales. 

[Hint: you may use without proof that 

$$
E [ X Y | \mathcal {F} ] = X E [ Y | \mathcal {F} ]\tag{F.66}
$$

if the collection of random variables $\mathcal { F }$ contains $X . ]$ 

c) Show that, if $\mu$ and $\sigma$ are constants, then 

$$
S _ {t} = S _ {0} e ^ {\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t}\tag{F.67}
$$

satisfies 

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma d W _ {t}\tag{F.68}
$$

and the initial condition, $S$ is equal to $S _ { 0 }$ at $t = 0$ 

## F.2.1 Solution

a) $( d t ) ^ { 2 } = 0 , ( d t ) ( d W ) = 0 , \mathrm { a n d } ( d W ) ^ { 2 } = d t .$ 

b) Let $0 \leq s \leq t$ . Then $W _ { t } = W _ { s } + W _ { ( s , t ) }$ , where 

$$
W _ {(s, t)} = \int_ {s} ^ {t} d W _ {u}
$$

is independent of $W _ { s }$ . Then 

$$
\begin{array}{r c l} E [ W _ {t} | W _ {\leq s} ] & = & E [ W _ {s} | W _ {\leq s} ] + E [ W _ {(s, t)} | W _ {\leq s} ] \\ & = & W _ {s} + E [ W _ {(s, t)} ] \end{array}
$$

since conditioning with independent info does not alter the mean. But $W _ { ( s , t ) }$ has mean zero, so 

$$
E [ W _ {t} | W _ {s} ] = W _ {s}. \square
$$

Also 

$$
\begin{array}{r c l} E [ W _ {t} ^ {2} | W _ {\leq s} ] & = & E [ (W _ {s} + W _ {(s, t)}) ^ {2} | W _ {\leq s} ] \\ & = & E [ W _ {s} ^ {2} | W _ {s} ] + 2 E [ W _ {s} W _ {(s, t)} | W _ {\leq s} ] + E [ W _ {(s, t)} ^ {2} | W _ {\leq s} ] \\ & = & W _ {s} ^ {2} + 2 W _ {s} E [ W _ {(s, t)} | W _ {\leq s} ] + E [ W _ {(s, t)} ^ {2} ] \\ & & \text {by given hint, and because W_{(s,t) is independent of W_{s}}} \\ & = & W _ {s} ^ {2} + 2 W _ {s} E [ W _ {(s, t)} ] + t - s \\ & & \text {since W_{(s,t) is independent of W_{\leq s} and is N(0,t - s)}} \\ & = & W _ {s} ^ {2} + t - s. \end{array}
$$

Hence 

$$
E [ W _ {t} ^ {2} - t | W _ {\leq s} ] = W _ {s} ^ {2} - s
$$

as required. 

c) By Ito’s formula, 

$$
d S _ {t} = \frac {\partial S}{\partial t} + \frac {\partial S}{\partial W} d W + \frac {1}{2} \frac {\partial^ {2} S}{\partial W ^ {2}} (d W) ^ {2}.
$$

We compute the terms entering here from the given function $S { \mathrm { : } }$ 

$$
\frac {\partial S}{\partial t} = S _ {0} (\mu - \frac {1}{2} \sigma^ {2}) e ^ {\mu t + \sigma W _ {t} - 1 / 2 \sigma^ {2} t} = (\mu - 1 / 2 \sigma^ {2}) S _ {t}
$$

$$
\frac {\partial S}{\partial W} = S _ {0} \sigma e ^ {\mu t + \sigma W _ {t} - 1 / 2 \sigma^ {2} t} = \sigma S _ {t}
$$

$$
\frac {\partial^ {2} S}{\partial W ^ {2}} = \sigma \frac {\partial S _ {t}}{\partial W} = \sigma^ {2} S _ {t}.
$$

Therefore 

$$
d S _ {t} = (\mu - 1 / 2 \sigma^ {2}) S _ {t} d t + \sigma S _ {t} d W _ {t} + 1 / 2 \sigma^ {2} S _ {t} d t
$$

$$
\frac {d S _ {t}}{S _ {t}} = \mu d t + \sigma d W _ {t}. \square .
$$

so 

## F.3 Question

Let $S _ { t }$ denote the price of a non-dividend-paying asset at time t, satisfying the stochastic equation 

$$
d S _ {t} = \mu S _ {t} d t + \sigma S _ {t} d W _ {t},
$$

where the drift $\mu$ and the volatility $\sigma$ are both assumed constant, and $W _ { t }$ is the Wiener process. Let $C _ { t }$ be the price of a derivative based on this asset, satisfying 

$$
d C _ {t} = \mu_ {t} ^ {C} C _ {t} d t + \sigma_ {t} ^ {C} C _ {t} W _ {t}.
$$

a) If at time t a trader is long $\phi _ { t }$ units of the asset, and short one unit of the derivative, what is the value of the trader’s position? Show that the position is risk-free if and only if 

$$
\phi_ {t} = \frac {\sigma_ {t} ^ {C} C _ {t}}{\sigma S _ {t}}.
$$

b) Assuming that the short-term interest rate has the constant value $r ,$ show that the principle of no arbitrage implies that 

$$
\frac {\mu_ {t} ^ {C} - r}{\sigma_ {t} ^ {C}} = \frac {\mu - r}{\sigma}.
$$

Comment briefly on the financial significance of this relation. 

c) Now assume that the derivative price can be expressed in the form $C _ { t } =$ $C ( S _ { t } , t )$ , where the function $C ( S , t )$ has continuous second derivatives. Use Ito’s lemma to show that 

$$
\begin{array}{r l r} {C _ {t} \mu_ {t} ^ {C}} & = & {\frac {\partial C}{\partial t} + \mu S \frac {\partial C}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} C}{\partial S ^ {2}}} \\ {\mathrm{and}} & {C _ {t} \sigma_ {t} ^ {C}} & = {\sigma S \frac {\partial C}{\partial S}.} \end{array}
$$

d) Show that the no arbitrage condition implies that $C ( S , t )$ satisfies 

$$
\frac {\partial C}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} C}{\partial S ^ {2}} = r \left(C - S \frac {\partial C}{\partial S}\right).
$$

What is the significance that the parameter $\mu$ does not appear in this relation? 

## F.3.1 Solution

a) The value of the trader’s position is $V _ { t } = \phi _ { t } S _ { t } - C _ { t }$ ; it is risk-free if and only if the coeficient of the randomness, $d W _ { t }$ is zero, during the small time-interval dt. The change in the value during dt is 

$$
d V _ {t} = \phi_ {t} d S _ {t} - d C _ {t} = \phi_ {t} (\mu S _ {t} d t + \sigma S _ {t} d W _ {t}) - (\mu_ {t} ^ {C} C _ {t} d t + \sigma_ {t} ^ {C} C _ {t} d W _ {t})
$$

since his position does not change; it is therefore risk-free if and only if 

$$
\phi_ {t} \sigma S _ {t} = \sigma_ {t} ^ {C} C _ {t}
$$

giving the result. 

b) The condition of no arbitrage means that the drift in the no-risk position must be the short-term interest-rate. Thus 

$$
\phi_ {t} \mu S _ {t} - \mu_ {t} ^ {C} C _ {t} = r V _ {t} = r (\phi S _ {t} - C _ {t})
$$

which, on substituting $\phi _ { t }$ gives 

$$
\sigma_ {t} ^ {C} C _ {t} \mu / \sigma - \mu_ {t} ^ {C} C _ {t} = r (\sigma_ {t} ^ {C} C _ {t} / \sigma - C _ {t}).
$$

Divide both sides by $C _ { t } ^ { C } \sigma _ { t } ^ { C }$ gives the result. It means that there exists a common risk-premium $\lambda = ( \mu - r ) / \sigma$ , the same for the asset and all derivatives of it. 

c) By Ito’s lemma, 

$$
d C _ {t} = \frac {\partial C}{\partial t} d t + \frac {\partial C}{\partial S} d S + \frac {1}{2} \frac {\partial^ {2} C}{\partial S ^ {2}} (d S) ^ {2}
$$

as the other second derivatives are zero by the Ito rules. The only non-zero term in $( d S ) ^ { 2 }$ is $\sigma ^ { 2 } S _ { t } ^ { 2 } ( d W _ { t } ) ^ { 2 } = \sigma ^ { 2 } S ^ { 2 } d t$ . Therefore 

$$
d C = \left(\frac {\partial C}{\partial t} + \frac {\partial C}{\partial S} \mu S + \frac {1}{2} \frac {\partial^ {2} C}{\partial S ^ {2}} \sigma^ {2} S ^ {2}\right) d t + \sigma S \frac {\partial C}{\partial S} d W _ {t}.
$$

We then prove c) by identifying $C _ { t } \mu _ { t } ^ { c }$ with the coeficient of dt and $C _ { t } \sigma _ { t } ^ { c }$ with the coeficient of $d W _ { t }$ 

d) b) tells us that 

$$
\mu_ {t} ^ {C} = r + \sigma_ {t} ^ {C} (\mu - r) / \sigma = r + (S / C) \frac {\partial C}{\partial S} (\mu - r), \mathrm{byc)}
$$

so substituting in c) we get 

$$
\mu^ {C} = C ^ {- 1} \left(\frac {\partial C}{\partial t} + \mu S \frac {\partial C}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} C}{\partial S ^ {2}}\right) = r + (S / C) \frac {\partial C}{\partial S} (\mu - r)
$$

and the result follows. This means that derivatives can be priced without knowing the rate of return on the asset. 

## F.4 Question

Let $S _ { t }$ be the price, in Sterling, of a foreign currency. The Sterling interest rate is $r ,$ and the foreign interest rate is $f _ { : }$ both assumed constant and expressed on a continuously compounded basis. 

a) Explain what is meant by the forward price of a foreign currency. 

b) At time $t = 0$ an investor purchases a derivative from a dealer which pays of $S _ { T } - K$ at time $t = T$ , where $K$ is a fixed amount of Sterling. The investor pays $C _ { 0 }$ for the derivative. Assuming that the dealer makes no profit or loss on the transaction, use a no arbitrage argument to show that $C _ { 0 } = 0$ if and only if $K = \tilde { S } _ { T }$ , where $\tilde { S } _ { T } = \check { S _ { 0 } } e ^ { ( r - \check { f } ) T }$ 

c) The price process for the foreign currency is given by 

$$
S _ {t} = S _ {0} e ^ {\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t}
$$

where $\mu$ and $\sigma$ are constants, and $W _ { t }$ is the standard Wiener process. Calculate the mean and variance of $S _ { T }$ . 

You can use the fact that 

$$
E \left[ e ^ {X} \right] = e ^ {M + \frac {1}{2} V}
$$

if the random variable X is normally distributed with mean $M$ and variance $V .$ 

d) Why would you expect the result for $E \left[ S _ { T } \right]$ to difer from $\tilde { S } _ { T }$ as defined in b) above? 

## F.4.1 Solution

a) The forward price in Sterling of a foreign currency is the price you pay, not due for payment till the forward time T, for one unit of foreign currency. 

b) Dealer may take no risks, and then ”no arbitrage” says that at time $T$ he must possess $A e ^ { r T }$ where A is his investment in the deal at $t = 0$ So if he makes no investment, he must break even at time $T$ . 

At $T = 0$ dealer receives $C _ { 0 }$ in Sterling. He must cover his obligation $S _ { T } - K$ at time $T _ { i }$ so he must now buy $S _ { 0 } e ^ { - f T }$ in foreign currency, which he can invest there. This grows to $( S _ { t } e ^ { - f T } ) e ^ { f t }$ at time t. He is left with $C _ { 0 } - S _ { 0 } e ^ { - f T }$ to invest in Sterling. This grows into $( C _ { 0 } - S _ { 0 } e ^ { - f T } ) e ^ { r t }$ at time t (all values in Sterling). At time $T$ his money-market assets are 

$$
(C _ {0} - S _ {0} e ^ {- f T}) e ^ {r T} + S _ {T} e ^ {- f T} e ^ {f T}
$$

and his obligation is $S _ { T } - K$ . To be equal: 

$$
(C _ {0} - S _ {0} e ^ {- f T}) e ^ {r T} + S _ {T} e ^ {- f T} e ^ {f T} = S _ {T} - K
$$

So $C _ { 0 } = 0$ if and only if 

$$
K = S _ {0} e ^ {(r - f) T}.
$$

c) σ $\cdot W _ { t }$ has mean 0 and variance $V = \sigma ^ { 2 } t$ , so from the given formula, 

$$
\begin{array}{r c l} {E \left[ S _ {t} \right]} & = & {E \left[ S _ {0} e ^ {\mu t + \sigma W _ {t} - \frac {1}{2} \sigma^ {2} t} \right]} \\ & = & {S _ {0} e ^ {\mu t - \frac {1}{2} \sigma^ {2} t} E \left[ e ^ {\sigma W _ {t}} \right]} \\ & = & {S _ {0} e ^ {\mu t - \frac {1}{2} \sigma^ {2} t} e ^ {0 t + \frac {1}{2} \sigma^ {2} t}} \end{array}
$$

so putting $t = T$ gives 

$$
E \left[ S _ {T} \right] = S _ {0} e ^ {\mu T}.
$$

For the variance we use Var $X ^ { = } E \left[ X ^ { 2 } \right] - \left( E [ X ] \right) ^ { 2 }$ , and that $2 \sigma W _ { T }$ has variance $4 \sigma ^ { 2 } T$ . Then 

$$
\begin{array}{r c l} {E \left[ S _ {T} ^ {2} \right]} & = & {E \left[ S _ {0} ^ {2} e ^ {2 \mu T - \sigma^ {2} T} e ^ {2 \sigma W _ {T}} \right]} \\ & = & {S _ {0} ^ {2} e ^ {2 \mu T} e ^ {- \sigma^ {2} T} e ^ {\frac {1}{2} 4 \sigma^ {2} T}.} \end{array}
$$

Hence 

$$
\mathrm{Var} S _ {T} = S _ {0} ^ {2} e ^ {2 \mu T} e ^ {\frac {3}{2} T \sigma^ {2}} - (E [ S _ {T} ]) ^ {2} = S _ {0} ^ {2} e ^ {2 \mu T} (e ^ {T \sigma^ {2}} - 1)
$$

d) The price is not risk free; also it depends on $\mu ,$ which the “no arbitrage” price never does. 

## F.5 Question

A call option on a foreign currency pays of $\mathrm { M a x } ( S _ { T } - K , 0 )$ at time $T _ { \ast }$ , where $S _ { t }$ is the price, in Sterling, of the foreign currency at time $t ,$ and K is the strike price of the option in Sterling. Assuming the Black-Scholes model, the present value $C _ { 0 }$ of a call option, in Sterling, can be written 

$$
C _ {0} = e ^ {- r T} \left[ S _ {0} e ^ {(r - f) T} N (h ^ {+}) - K N (h ^ {-}) \right],
$$

where $r$ is the Sterling interest rate, and $f$ is the foreign interest rate, both assumed constant and expressed on a continuously compounded basis. The normal cumulative distribution function $N ( x )$ is given by 

$$
N (x) = \frac {1}{\sqrt {(2 \pi)}} \int_ {- \infty} ^ {x} e ^ {- \frac {1}{2} \xi^ {2}} d \xi ,
$$

and the parameters $h ^ { \pm }$ are given by 

$$
h ^ {\pm} = \frac {\ln (\tilde {S} _ {T} / K) \pm \frac {1}{2} \sigma^ {2} T}{\sigma T ^ {1 / 2}},
$$

where $\sigma$ is the volatility and $\tilde { S } _ { T } = S _ { 0 } e ^ { ( r - f ) T }$ 

a) Explain briefly what is meant for a call option to be ‘in the money’, ‘at the money’ and ‘out of the money’. 

b) Show that if $S _ { 0 }$ is very large compared with K, then $C _ { 0 }$ is given approximately by 

$$
C _ {0} = S _ {0} e ^ {- f T} - K e ^ {- r t}.
$$

Comment on the financial significance of this result. 

c) Show that $N ( x ) + N ( - x ) = 1$ 

d) A currency option is said the be ‘at-the-money-forward’ when $K =$ $S _ { 0 } e ^ { ( r - f ) { \bar { T } } }$ ; show that the present value of an at-the-money-forward call option is given by 

$$
C _ {0} = S _ {0} e ^ {- f T} \left(2 N (\frac {1}{2} \sigma T ^ {1 / 2}) - 1\right).
$$

## F.5.1 Solution

a) ‘in the money’ means $S _ { 0 } > K$ ; ‘at the money’ means $S _ { 0 } = K ;$ ; ‘out of the money’ means $S _ { 0 } < K$ 

b) $S _ { 0 } \gg K$ implies that $\tilde { S } _ { T } \gg K$ , which implies that $l n ( \tilde { S } _ { T } / K ) \gg \sigma ^ { 2 } T$ and $\sigma T ^ { 1 / 2 } , \mathrm { s o } h ^ { \pm }$ is large, so $N ( h ^ { \pm } ) \approx 1$ . The $C _ { 0 }$ reduces to the ans. 

If the option is nearly certain to expire in the money, then the present value takes the simple given form, which can be written as the diference of the forward price of the currency minus the strike price, discounted back to the present. 

c) Put $\eta = - \xi$ in the integral for N. Then $d \xi = - d \eta .$ , so 

$$
N (- x) = (2 \pi) ^ {- 1 / 2} \int_ {\infty} ^ {x} e ^ {- \frac {1}{2} \eta^ {2}} (- d \eta) = (2 \pi) ^ {- 1 / 2} \int_ {x} ^ {\infty} e ^ {- \frac {1}{2} \eta^ {2}} d \eta .
$$

Adding to $N ( x )$ gives the full integral, = 1 as the probability is normalised. 

d) When $K \ = \ \tilde { S } _ { T }$ , we have ln $\left( \tilde { S } _ { T } / K \right) \ = \ 0 ;$ then $h ^ { \pm } ~ = ~ \pm \sigma T ^ { 1 / 2 }$ ; then $N ( h ^ { - } ) = 1 - N ( h ^ { + } )$ , and the formula gives 

$$
C _ {0} = e ^ {- r T} \left[ S _ {0} e ^ {(r - f) T} N (h ^ {+}) - S _ {0} e ^ {(r - f) T} \left(1 - N (h ^ {+})\right) \right] = S _ {0} e ^ {- f T} \left(2 N (h ^ {+}) - 1\right)
$$

which is the ans. 

## F.6 Question

Let $S _ { t }$ be the price of a non-dividend-paying asset at time t, where $t = 0$ is the present. Let $C ( S _ { 0 } , K , T )$ denote the value today of a standard call option on the asset, with strike K and maturity T. Let $P ( S _ { 0 } , K , T )$ denote the value of the corresponding standard put option. Assume that the continuously compounded rate of interest r is constant. 

a) What is the pay-of of the put option? Give two possible reasons why an investor might purchase a put option. 

b) Use a no-arbitrage argument to derive the put-call parity relation 

$$
C (S _ {0}, K, T) - P (S _ {0}, K, T) = S _ {0} - e ^ {- r T} K.
$$

c) Now assume the standard Black-Scholes model, according to which the value of the call option is given by 

$$
C (S _ {0}, K, T) = e ^ {- r T} \left[ S _ {0} e ^ {r T} N (h ^ {+}) - K N (h ^ {-}) \right],
$$

where $\begin{array} { r } { N ( x ) = \frac { 1 } { \sqrt { ( 2 \pi ) } } \int _ { - \infty } ^ { x } e ^ { - \frac { 1 } { 2 } \xi ^ { 2 } } d \xi } \end{array}$ is the $N ( 0 , 1 )$ cumulative distribution function, 

$$
\mathrm{and} h ^ {\pm} = \frac {\ln \left(S _ {0} e ^ {r T} / K\right) \pm \sigma^ {2} T}{\sigma T ^ {1 / 2}}, \mathrm{where} \sigma \mathrm{isconstant}.
$$

For what value of $S _ { 0 }$ does $N \left( h ^ { + } \right) = 1 / 2 ?$ 

Use the put-call parity relation and $N ( x ) + N ( - x ) = 1$ to prove that 

$$
P \left(S _ {0}, K, T\right) = e ^ {- r T} \left[ K N \left(- h ^ {-}\right) - S _ {0} e ^ {r T} N \left(- h ^ {+}\right) \right].
$$

## F.6.1 Solution

a) Payof for a put option is $\mathrm { M a x } ( K - S _ { T } , 0 )$ 

Reason for buying a put option is to speculate that the price will fall, and the option will magnify the profit in this case. Or, to pay a small premium to protect against falling price. 

b) Suppose first that $C - P - ( S _ { 0 } - e ^ { - r T } K ) = q > 0$ . The arbitrageur will then sell C and buy P, and buy the share at $S _ { 0 }$ . He then has $q - e ^ { - r T } K$ to invest in (or borrow from) the money market, which at time $T$ has grown to $q e ^ { r T } - K . \mathrm { ~ I f ~ } S _ { T } > K$ , P is void, but his client can buy the share (which he has) for K, which he uses to pay of the debt, leaving a profit of $q e ^ { r T }$ . If however, $S _ { T } < K$ , his client would not call, but he can sell his share for K using the put option, again leaving a profit of $q e ^ { r T }$ 

If $C - P - ( S _ { 0 } - e ^ { - r T } ) = - q < 0$ , he will buy $C$ and sell $P ,$ and sell $S _ { 0 }$ short. This leaves him $P - C + S _ { 0 } = q + e ^ { - r T } K$ invested until time $T ,$ , when it has grown to $q e ^ { r T } + K$ . If $S _ { T } > K$ his clients put-option will not be exercised; he uses his call option to buy a share for $K$ , to settle his short position on $S _ { 0 }$ , leaving him with a profit of $q e ^ { r T }$ . If however $S _ { T } < K$ , his call option is worthless, and his client will sell him a share for $K$ , which he uses to settle his short purchase. He still has $q e ^ { r T }$ profit. 

c) $N ( h ^ { + } ) = { \textstyle { \frac { 1 } { 2 } } } \ \mathrm { i f } \ h ^ { + } = 0$ , which means that 

$$
\ln \left(S _ {0} e ^ {r T} / K\right) = - \frac {1}{2} \sigma^ {2} T
$$

so 

$$
S _ {0} = e ^ {- r T} K e ^ {- \frac {1}{2} \sigma^ {2} T}.
$$

We have 

$$
\begin{array}{r c l} P & = & C - S _ {0} + e ^ {r T} K \\ & = & e ^ {- r T} \{S _ {0} e ^ {r T} N (h ^ {+}) - K N (h ^ {-}) \} - S _ {0} + e ^ {- r T} K \\ & = & S _ {0} (N (h ^ {+}) - 1) + e ^ {- r T} K (1 - N (h ^ {-})) \\ & = & e ^ {- r T} \{K N (- h ^ {-}) - e ^ {r T} S _ {0} N (- h ^ {+}) \}. \square \end{array}
$$

## G Bibliography

Here is a list of books that you might progress to next. While the ones that you choose may depend on your particular interests and tastes, they are all very useful in their own way, and to some extent complementary. 

1. M.W. Baxter and A.J.O. Rennie, Financial Calculus, Cambridge University Press (1996). 



2. J.C. Hull, Options, Futures, and Other Derivatives, Prentice-Hall (Third Edition, 1997). 



3. R. Jarrow and S. Turnbull, Derivative Securities, Southwestern Press (1997). 



4. B. Oksendal, Stochastic Diferential Equations, Springer-Verlag (Fifth Edition, 1998). 





5. P. Wilmott, Derivatives, Wiley (1998). 





The following is a chronological list of important papers that should be accesible if you have understood the material in this book. 





1. F. Black and M. Scholes, “The pricing of options and corporate liabilities”, Journal of Political Economy 81, 637 (1973). 





2. R.C. Merton, “Theory of rational option pricing”, Bell Journal of Economics and Management Science 4, 141 (1973). 





3. O.A. Vasicek, “An equilibrium characterization of the term structure”, Journal of Financial Economics 5, 177 (1977). 





4. J.C. Cox, S.A. Ross and M. Rubinstein, “Option Pricing: A Simplified Approach”, Journal of Financial Economics 7, 229 (1979). 





5. A. Bensoussan, “On the theory of option pricing”, Acta Applicandae Mathematicae 2, 139 (1984). 





6. D. Heath, R. Jarrow and A Morton, “Bond pricing and the term structure of interest rates: a new methodology”, Econometrica 60, 77 (1992). 





Here is a list of some relevant web sites: 



1. Dow Jones: www.dowjones.com 

2. Financial Times: www.ft.com 

3. Foreign Exchange: www.x-rates.com 

4. FTSE International: www.ftse.com 

5. London International Financial Futures and Options Exchange: www.life.com 

6. London Stock Exchange: www.londonstockex.co.uk 

7. NASDAQ: www.nasdaq.com 

8. New York Stock Exchange: www.nyse.com 