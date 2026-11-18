

<!-- === Source: MinerU_markdown_Introduction_1_2122709467580706822.md (Page 1) === -->

The purpose of this text is to provide an introduction to the mathematics utilized in the pricing models of derivative instruments. The text approaches the mathematics behind continuous-time finance informally. Examples are given and relevance to financial markets is provided. 

Pricing models for financial derivatives require, by their very nature, utilization of continuous-time stochastic processes. A good understanding of the tools of stochastic calculus and of some deep theorems in the theory of stochastic processes is necessary for practical asset valuation. 

This book is intended as background reading for modern asset pricing theory as outlined by Jarrow (1996), Hull (1999), Duffie (1996), Ingersoll (1987), Musiela and Rutkowski (1997), and other excellent sources. 

There are several excellent technical sources dealing with this mathematical theory. Karatzas and Shreve (1991), Karatzas and Shreve (1999), and Revuz and Yor (1994) are the first that come to mind. Others are discussed in the references. Yet even to a mathematically well-trained reader, these sources are not easy to follow. Sometimes, the material discussed has no direct applications in finance. At other times, the practical relevance of the assumptions is difficult to understand. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d60b277e-db62-4c98-a2e5-7064819da890/431e4e9f53cf897aaf87b1f684f748500395ac665f0508af0f8b5a4654a37b24.jpg)


Such an approach may be found imprecise by a technical reader. We simply hope that the informal treatment provides enough intuition about some of these difficult concepts to compensate for this shortcoming. Unfortunately, by providing a descriptive treatment of these concepts, it is difficult to emphasize technicalities. This would defeat the purpose of the book. Further, there are excellent sources at a technical level. What seems to be missing is a text that explains the assumptions and concepts behind 

We have the following plan for learning the mathematics of derivative products. 

Finally, derivative products have a property that makes them especially suitable for a mathematical approach. Despite their apparent complexity, derivative products are in fact extremely simple instruments. Often their value depends only on the underlying asset, some interest rates, and a few parameters to be calculated. It is significantly easier to model such an instrument mathematically $^{2}$ than, say, to model stocks. The latter are titles on private companies, and in general, hundreds of factors influence the performance of a company and, hence, of the stock itself. 

Trading became cheaper. The deregulation of the financial services that gathered steam during the 1980s was also an important factor here. Three major steps in the theoretical revolution led to the use of advanced mathematical methods that we discuss in this book: 

A might have occurred. As a result of these needs, new exchanges and marketplaces came into existence. Introduction of new products became easier and less costly. 

It is mainly the need to hedge interest-rate and currency risks that is at the origin of the recent prolific increase in markets for derivative products. This need was partially met by financial markets. New products were developed and offered, but the conceptual understanding of the structure, functioning, and pricing of these derivative products also played an important role. Because theoretical valuation models were directly applicable to these new products, financial intermediaries were able to “correctly” price and successfully market them. Without such a clear understanding of the conceptual framework, it is not evident to what extent a similar development might have occurred. 

a much higher priority.
During this time, interest rate controls were eliminated. This coincided with increases in the government budget deficits, which in turn led to large new issues of government debt in all industrialized nations. For this reason (among others), the need to eliminate the interest-rate risk became more urgent. Interest-rate derivatives became very popular. 

pages popular.
The past two decades saw the freeing of exchange and capital controls.
This made the exchange rates significantly more variable. In the meantime,
world trade grew significantly. This made the elimination of currency risk
a much higher priority. 

During the past two decades, some major developments have occurred in the theoretical understanding of how derivative asset prices are determined and how these prices move over time. There were also some recent institutional changes that indirectly made the methods discussed in the following pages popular 

## 2 New Developments

The text is directed toward a reader with some background in finance. A strong background in calculus or stochastic processes is not needed, although previous courses in these fields will certainly be helpful. One chapter will review some basic concepts in calculus, but it is best if the reader has already fulfilled some minimum calculus requirements. It is hoped that strong practitioners in financial markets, as well as beginning graduate students, will find the text useful. 

1 Audience 

these mathematical tools and then relates them to dynamic asset pricing theory. 

The text gives as many examples as possible. Some of these examples have relevance to financial markets; others simply illustrate the mathematical concept under study. 

The Feynman-Kac formula and its simpler versions give a correspondence between classes of partial differential equations and certain conditional expectations. These expectations are in the form of discounted future asset prices, where the discount rate is random. This correspondence is useful in pricing interest-rate derivatives. 

The Girsanov theorem permits changing means of random processes by varying the underlying probability distribution. The theorem is in the background of some of the most important pricing methods. 

Derivative asset valuation utilizes the notion of arbitrage to obtain partial differential equations (PDEs) that must be satisfied by the prices of these products. We present the mathematics of partial differential equations and their numerical estimation. 

3.6 Partial Differential Equations 

At this point, the notion of martingales and their uses in asset valuation should be introduced. Martingale measures and the way they are utilized in valuing asset prices are discussed with examples. 

In doing this, some familiarity with the new calculus needs to be developed. Hence, we go over some of the basic results and discuss some simple examples. 

All of these require an introductory discussion of Wiener processes from a practical point of view, which means learning the “economic assumptions” behind notions such as Wiener processes, stochastic calculus, and differential equations. 

## 3.3 Wiener and Poisson Processes

The arbitrage theorem, by itself, is sufficient to introduce some of the main mathematical concepts that we discuss later. In particular, the arbitrage theorem provides a mathematical framework and, more important, justifies the existence and utilization of risk-neutral probabilities. The latter are “synthetic” probabilities utilized in valuing assets. They make it possible to bypass issues related to risk premiums. 

3.2 Risk-Neutral Probabilities 

The meaning and the relevance of the arbitrage theorem will be introduced first. This is a major result of the theory of finance. Without a good understanding of the conditions under which arbitrage, and hence infinite profits, is ruled out, it would be difficult to motivate the mathematics that we intend to discuss. 

3.1 The Arbitrage Theorem 