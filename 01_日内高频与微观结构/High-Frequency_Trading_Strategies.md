

<!-- === Source: MinerU_markdown_High-Frequency_Trading_Strategies_1_2122707067558010893.md (Page 1) === -->

# High-frequency trading strategies*

Michael Goldstein 

Babson College 

Babson Park, MA 02457-0310, USA 

goldstein@babson.edu 

Amy Kwan 

University of Sydney 

Sydney, NSW 2006, Australia 

amy.kwan@sydney.edu.au 

Richard Philip 

University of Sydney 

Sydney, NSW 2006, Australia 

richard.philip@sydney.edu.au 

Current version: May 23, 2017 

*We thank Sean Anthonisz, Joseph Barbara, Kevin Crotty, Doug Foster, Sean Foley, Austin Gerig, Elmer Funke Kupper, Brad Katsuyama, Vincent van Kervel, Adrian Lee, Thomas McInish, Maureen O’Hara, Talis Putnins, Ryan Riordan, Kevin Roshak, Ioanid Rosu, Andriy Shkilko, Avanidhar Subrahmanyam, Kumar Venkataraman, Tina Viljoen, David Walsh, Bart Yueshen, and Marius Zoican, as well as conference and seminar participants at the Australasian Finance and Banking Conference, Auckland Finance Conference, Centre for International Finance and Regulation (CIFR) Market Microstructure Conference, Curtin University, European Financial Management Association Annual Meeting, Financial Management Association Annual Meeting, and the Financial Research Network (FIRN) Sydney Market Microstructure Meeting for helpful comments. We would also like to thank CIFR, which funded this research under CIFR grant T013, and the Securities Industry Research Centre of Asia-Pacifi (SIRCA) for providing the data used for part of this study. 

# High-frequency trading strategies

## Abstract

Examining the order book imbalance immediately before each order submission, cancelation and trade, we show high frequency traders (HFT) supply liquidity on the thick side of the order book and demand liquidity from the thin side. This strategic behavior is more pronounced during volatile periods and when trading speeds increase. However, by competing with non-HFT limit orders, HFT impose a welfare externality by crowding out slower non-HFT limit orders. Overall, we document an important information channel driving HFT behavior. 

## 1.0 Introduction

Financial markets are the aggregators of trading behaviors of many different types of agents. Traditionally, these agents were primarily retail and institutional investors, as well as dealers or market makers making a two-sided market. Over the past decade, the participation of high frequency traders (HFT) in the markets has notably increased, and become increasingly dominant players, influencing financial markets in many ways through their trading decisions. Some suggest that HFT trading reduce the bid-ask spread, increase price efficiency, and increase overall market depth, although these effects may vary with market conditions.<sup>1</sup> 

While these are ex post effects of HFT trading decisions, much less is known about what affects HFT trading decisions ex ante. Some suggest that HFT can anticipate future order flow from other traders and predict future price movements.<sup>2</sup> But how do they anticipate the future? What information do they use? Are they better at this during certain times than others? Is HFT behavior different than that of institutions and retail investors, and if so, how? Does HFT behavior have welfare effects on other market participants; if so, how, when, and to whom? While we understand much about how HFT affect financial markets, not much is known about the information channels that drive HFT behavior due to the proprietary nature of their business. 

To answer these questions, we examine HFT behavior and identify information that affects this behavior, and compare and contrast it with that of institutions and retail traders. Specifically, we examine HFT order placement strategies and document one such information channel, namely the order book depth imbalance, and show that HFT are better able to take advantage of this channel than non-HFT, particularly for large imbalances or times of high volatility. Similar to Cao, Hansch and Wang (2009) and Cont, Kukanov and Stoikov (2014), we provide strong evidence that order book imbalances predict short term future price movements. While we find that all traders (i.e., HFT, institutions and retail) attempt to capture information contained in the limit order book, we find HFT are better at taking advantage of this information, especially at times when the market is volatile and when HFT’s speed advantage increases.<sup>3</sup> Specifically, HFT executions (either due to market orders or the execution of previously submitted limit orders) occur in the direction of the order book imbalance (i.e., buy when the limit order book is deeper on the bid side than the ask side) and HFTs cancel or amend orders when the order book imbalance moves against them.<sup>4</sup> As a result, while it may be true that HFT add liquidity, they do not do so at times when it is most needed: HFT on average, supply liquidity on the thick side of the order book (where it is not needed) and demand liquidity from the thin side (where it is needed). By competing with non-HFT limit orders on the thick side of the order book, we find evidence that HFT limit order placement and trading behavior “crowd out” non-HFT limit order executions. Specifically, we find that HFT trading behavior results in a lower execution probability for non-HFTs when such execution would be beneficial for non-HFT. 

For this investigation, we use a unique, broker-level dataset from the Australian Securities Exchange (ASX). Using this dataset, we reconstruct the full limit order book and measure the shape of the order book at the time of each order submission, cancelation, amendment, and trade. The dataset also classifies brokers into three trader types: proprietary HFT firms, institutions and retail. Our primary focus is on HFT trading behavior, relative to institutional and retail traders. In addition, the introduction of faster ITCH technology on the ASX during our time period provides a natural experiment for us to investigate the effects of increasing trading speeds. 

We find strong evidence that the shape of the limit order book contains information about future price movements. In particular, when the depth available on the best five continuous prices on the bid (ask) side exceeds the volume available on the best five continuous ask (bid) prices, we show that prices are more likely to rise (fall) in the short-term.<sup>5</sup> We also find that non-HFTs want to act like HFTs, but are less successful precisely when the market indicates it is most important to do so. While Brogaard, Hendershott, and Riordan (2014) find that HFTs attempt to trade in the direction of the book, we demonstrate that all trader types attempt to trade in the direction of the price change predicted by the depth imbalance: for all trader types, the percentage of buyerinitiated trade volume increases as the depth available on the bid prices grows relative to the depth on the ask prices. We are also able to determine the conditions under which HFTs notably do better than non-HFTs, and find that the differential effects are non-linear: when depth imbalances are very large and therefore suggest that future price changes will be large, we find that HFTs are more successful at trading in the direction of the imbalance, relative to the other trader types.<sup>6</sup> Thus, HFT are most successful during market conditions when fast trading speeds offer the greatest advantages. This speed advantage has a welfare effect on the slower institutional and retail market participants. We find that over 40% of HFT profits arise from market order executions when the size of the order book imbalance at the time of trade is in the top decile of all order book imbalances. This finding suggests a large portion of HFT profits come from picking off stale limit orders from slower traders. While all traders attempt to trade in the direction of the imbalance, slower institutional and retail traders miss out on the most profitable trades. 

We use multinomial logistic regression to further investigate a trader’s order placement decisions. For passive limit orders, we find that HFTs are better at using information contained in the limit order book, relative to institutional and retail investors. HFTs submit limit orders to the order book primarily when there is a small favorable depth imbalance (i.e., slightly more depth on that side of the book). As the depth imbalance becomes more favorable (i.e., as one side of the book dominates the other), the resting limit order is left to execute in the same direction as the imbalance would imply, so, for example, a limit order is left on the bid side for large buy imbalance (bid depth exceeding ask depth). On the other hand, if the depth imbalance becomes less favorable, HFT are quick to cancel or amend their orders, reducing adverse selection costs. Together, these strategies mean that HFT supply liquidity to the thick side of the order book and demand liquidity from the thin side. 

Additionally, we show that large depth imbalances only persist in the order book for a fraction of a second and thus, speed is critical for a trader to capture this information. We document a U-shape pattern between aggressive HFT volumes and the limit order book depth imbalance. Notably, we find that HFT’s share of aggressive trading volume increases when particularly large positive or negative depth imbalances exists, consistent with the HFT’s speed advantage. Collectively, these results demonstrate that HFT monitor the limit order book more effectively than institutional and retail investors and react faster to changes in depth imbalances through their order placement strategies. 

We next investigate HFT trading behavior around times of high stock volatility. We find HFT demand more liquidity when the market is volatile. Further, for both aggressive and passive executions, we show that HFT are even more successful at trading in the direction of the order book during periods of high volatility.<sup>7</sup> When markets are volatile, fast HFT are better able to use market orders to pick off stale limit orders from slower institutional and retail investors. Similarly, HFT use their speed advantage to cancel their own stale limit orders to reduce their adverse selection costs. These results imply that trading speed differentials are particularly advantageous during periods of high volatility. 

The introduction of ITCH in 2012 offers a natural experiment to investigate the effects of a speed change on HFT trading behavior. Using a difference-in-difference framework, we demonstrate that HFT are more successful at trading in the direction of the order book when they gain a larger speed advantage. However, one externality of HFT trading behavior is that there is a negative welfare implications for non-HFT institutional and retail traders due to a “crowding out” effect on the execution of non-HFT limit orders. We find that the probability of execution for institutional and retail limit orders submitted to the best bid and ask prices decreases when HFT gain a larger speed advantage. Further, conditioning limit order executions on the shape of the order book, we show that it is the probability of favorable executions (i.e. non-HFT limit order trading in the direction of the order book imbalance), which falls. 

Overall, we uncover one information channel through which HFT incorporates information into price: by trading in the direction of the order book imbalance, which is a strong predictor of future price movements, and doing so better and faster than non-HFT participants. As a result, our findings provide an explanation for many previously reported empirical results. In particular, we find that HFT could help facilitate price efficiency by trading in the direction of the momentum and in doing so, incorporating information contained in the limit order book into the price formation process.<sup>8</sup> Second, our finding that HFT trade in the direction of the limit order book and reduce the limit order fill rate of institutional traders suggests how HFT may increase trading costs for institutional orders, which may explain how HFTs initially trade ‘against the wind’ but eventually trade ‘with the wind’ as a large institutional trade progresses, as in van Kervel and Menkveld (2016) and Korajcyzk and Murphy (2016). Specifically, we show that HFT can detect institutional demand through the order book depth imbalance and trade in the same direction of the imbalance before the predicted price rise, crowding out the institutional limit orders and ultimately increasing institutional implementation shortfall. 

Third, our findings on limit order strategies provide a mechanism for how limit orders contribute to price discovery (Brogaard, Hendershott and Riordan, 2016). HFT limit orders execute in the same direction of the imbalance and HFT cancel or amend their limit orders when depth on the opposite side of the resting limit order begins to build up. Thus, HFT limit buy orders in general trade before a predicted price rise and are canceled before a predicted price fall. 

Our results also have implications for studies on the market making role of HFT in equity markets. Some studies, such as Hendershott, Jones and Menkveld (2011), Hasbrouck and Saar, (2013), and Brogaard, Hagstromer, Norden and Riordan (2015), find that HFT market making increases market depth, but employ traditional measures of market depth, aggregated across both bid and ask prices.<sup>9</sup> However, aggregated measures of market depth do not capture the amount of depth available on the side of the limit order book where it is most needed or wanted, making welfare comments more difficult.<sup>10</sup> Whether depth increases are beneficial depends in part on whether depth is added on the side where it is needed; adding depth to the already thick side of a limit order book is likely of little benefit to the market and could disadvantage prior limit order submitters, while adding depth to the thin side of a market may add useful liquidity. Our results show that HFT on average supply depth on the thick side of the order book but demand depth from the thin side of the order book, i.e., they may add depth, but not on the side that is thin. Similarly, HFT cancel limit orders from the thin side of the order book, which face larger adverse selection costs. 

Finally, several studies in the literature examine HFT liquidity provision during stressful times. Brogaard et al. (2016) examine the stability of liquidity supply by high frequency traders, who do not have the obligation to supply liquidity during stressful periods. They find that HFTs supply liquidity to non-HFTs during extreme price moves in a single security but demand liquidity when several stocks experience simultaneous extreme price moves. However, their analysis focuses exclusively on the liquidity demanded and supplied through the Nasdaq exchange, which represents only 30-40% of all trading activity of the sample stocks. Thus, it is possible that HFT are supplying liquidity on Nasdaq while demanding liquidity from other trading venues. By analyzing a mostly consolidated market, we provide further insights on HFT trading activity over the whole market. Unlike Brogaard et al. (2016) which examined orders on a segment of a highly fragmented market with different maker/taker rebates, our results on a largely consolidated market with no maker/taker rebates shows that HFT are net demanders of liquidity and become even more aggressive at times of high volatility.<sup>11</sup> 

## 2.0 Data and variable construction

## 2.1 Data and sample selection

We obtain full order book and trade data for stocks in the S&P/ASX 100 index from the AusEquities database provided by the Securities Industry Research Centre of Asia Pacific.<sup>12</sup> The securities contained in our dataset are the most liquid and actively traded among HFT and institutional investors on the Australian Securities Exchange (ASX), the dominant stock exchange for Australian equities, with over 90% market share of on-market traded volume in 2012.<sup>13</sup> The ASX operates as a continuous limit order book between approximately 10:00 am and 4:00 pm, matching orders based on price and time priority, with a randomized open and a randomized close. 

We analyze six months of order level data for the period January 3, 2012 to June 30, 2012, which incorporates the introduction of ITCH on April 2, 2012.<sup>14</sup> To avoid the randomized open and close, we include only trades and orders entered between 10:10:00 and 16:00:00 to ensure that our sample is not contaminated by the opening and closing call auctions. We assume that all outstanding orders remaining in the limit order book at the end of the trading day are cancelled. 

For each order book event, the data contain the stock symbol, date and time of event to the millisecond level, order size and price, order identification number and an identifier for the submitting broker and event type, which consists of submit, trade, amend, or cancel. Additionally, we use the order identification number to trace subsequent amendments, executions or cancelation back to the original order entry, allowing for a full reconstruction of the limit order book and the tracking of the order and its queue position through time. 

Data from the ASX offer several advantages over other exchanges. In our dataset, broker identifiers are assigned into three trader categories: proprietary HFT firms (HFT), Institutions, and Retail.<sup>15</sup> We refer to orders originating from Institutions and Retail collectively as non-HFT. We rely on the granularity of the data to compute the depth imbalance proxy for trading strategies. Furthermore, because we can replay the full order book, we do not have to rely on trade classification algorithms, such as Lee and Ready (1991), to determine whether a trade is buyer or seller initiated.<sup>16</sup> Following Upson, Johnson and McInish (2015), we aggregate all trade reports at the same price, in the same trade direction, from the same broker, and reported in the same millisecond timestamp into one marketable order. Finally, in comparison to U.S. and European equity markets, the ASX is less fragmented, operating as a virtual monopoly in Australian equities during our period with over 90% of the daily trading volume, so our data comprises almost the entire market. 

## [Insert Table 1]

Table 1, Panel A reports the summary statistics for the 94 stocks, which appear in the S&P/ASX 100 index over the full sample period. Market capitalization is measured on January 3, 2012, the first trading day in the sample, and is expressed in billions of AUD. All other variables are measured on a daily basis and averaged across the sample period. The average stock has a market capitalization of 13.52 AUD billion and volume weighted trade price of $11.43. The average daily dollar volume is 27.8 AUD million and the average number of trades is 2,264. Given that the minimum pricing increment on the ASX is $0.01 for stocks priced above $2.00, an average daily time-weighted quoted spread (Spread) of 1.02 cents indicates that many stocks in the sample are likely to be spread constrained. 

Table 1, Panel B reports the summary statistics for all trader types, HFT, Institutions and Retail. Consistent with the prior literature, we find that HFT monitor the limit order book more actively. Relative to Institutions and Retail, HFT have a higher percentage of order cancelations, and the median submission to cancel time is significantly lower for HFT. The average number of active and passive executions is approximately equal for HFT, whereas Institutions and Retail are predominantly limit order traders.<sup>18</sup> In the following sections, we investigate how HFT incorporate information contained in the order book to their trading strategies. 

## 2.2 Depth imbalance

Previous work has established that imbalances are related to future price directions, and that imbalances can affect order submission strategies. Chordia, Roll and Subrahmanyam (2002) and Chordia and Subrahmanyam (2004) document a strong relationship between trade imbalances and future returns. Using more granular limit order book data, Cao, Hansch and Wang (2009) and Cont, Kukanov and Stoikov (2014) find strong evidence that order imbalances between the buy and sell schedules of the limit order book are significantly related to future stock returns. Cont, Kukanov and Stoikov (2014) show that price changes over short time intervals are mainly driven by imbalances between supply and demand at the best bid and ask prices. Specifically, large buying (selling) pressure on the bid (ask) price predicts future price rises (falls). Further, Ranaldo (2004) examines how the state of the limit order book can affect a trader’s order submission strategy. Based on these studies, we use the information contained in the state of the limit order book to proxy for strategic trading. 

To measure the shape of the limit order book prior to an order book event, we calculate depth imbalance (DI) as the difference between the volume available at the best bid and ask prices, as a proportion of the total volume available at the best bid and ask prices.<sup>19</sup> Specifically, for each order book event (i.e., submission, trade, amendment or cancelation) we determine: 

$$
D I _ {t} = \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}
$$

where $\begin{array} { r } { \sum _ { i = 1 } ^ { n } V o l B i d _ { i , t } \ ( \sum _ { i = 1 } ^ { n } V o l A s k _ { i , t } ) } \end{array}$ is the volume available at the top n bid (ask) price levels immediately before the order book event, t. (We compute DI immediately before the time of event to avoid capturing the volume of order book event itself; see Appendix 1 for a detailed example of the construction of DI.) For our main results, we calculate DI based on the volume available at the top five bid and ask prices (n = 5).<sup>20</sup> Our measure of DI is bounded between -1 and 1, where a value close to -1 (1) indicates that the depth available at the ask (bid) price levels is much larger than the bid (ask) depth available, so this measure could be interpreted as a relative buying interest index. 

For some tests, we multiply DI by an indicator for whether the order is a buy or sell to remove the effects of trade direction. We refer to this directionally adjusted DI measure as Adjusted DI. When Adjusted DI is positive, the trade or order event occurs in the direction of the depth imbalance (e.g., an active buy execution from a buy market order or a passive buy execution from a buy limit order executes when the bid depth exceeds the ask depth); when it is negative, the trade or order event occurs in the opposite direction of the depth imbalance (e.g., a buy market or limit order executes when the ask depth exceeds the bid depth). 

Table 1, Panel C summarizes the average Adjusted DI immediately before active executions, passive executions, order submissions, amendments and cancelations for each trader type.<sup>21</sup> For active executions, we find that all trader types (HFT, Institutions, and Retail) on average trade in the direction of the imbalance, indicating that traders are more likely to submit a market buy (sell) order when the bid (ask) depth is much larger than the ask (bid) depth. 

Comparing the magnitude of Adjusted DI, HFT submit market orders when Adjusted DI is much larger, 0.156, compared to 0.027 and 0.025 for Institutions and Retail, respectively. On the other hand, Adjusted DI at the time of passive executions is 0.083 for HFT, but is negative for Institutions, and Retail (-0.029, and -0.009, respectively). A negative Adjusted DI indicates that Institutions and Retail limit orders are picked off the thin side of the limit order book. We find that HFT submit limit orders when there is a moderate Adjusted DI (Adjusted DI = 0.063) but cancel their limit orders when the order book moves against their resting limit orders, indicated by a lower Adjusted DI (0.017), which reduces the adverse selection costs of HFT. In contrast, Retail traders both submit and cancel their orders in general in the same direction of the book at a much more moderate Adjusted DI (0.043 for submissions; 0.028 for cancels), and Institutions basically trade at a flat book, with their submissions very slightly on the opposite side (-0.004) and cancels very slightly on the same side (0.002). We investigate HFT trading strategies and their potential impact on non-HFT trading in the next section. 

## 3.0 Empirical Results

## 3.1 Depth imbalance, future stock prices and aggregate trading volumes

Before examining HFT trading behavior, we first establish the information content of order book depth imbalances. To investigate whether depth imbalances contain information about the future stock price, we start by ranking trades into deciles based on the depth imbalance immediately before the trade for each stock-day. For each transaction, we also calculate future returns by comparing the midpoint of the best bid and ask prices at the time of the trade with the bid-ask midpoint 10 trades in the future. Figure 1, Panel A presents the average future return for trades from each depth imbalance decile. We observe a strong positive relationship between the size and direction of the depth imbalance and future stock returns indicating that depth imbalances in the order book can predict future stock returns. <sup>22</sup> Specifically, as the number of buyers relative to sellers in the limit order book increase, the relative level of stock prices in the future also increase. 

## [Insert Figure 1]

Next, we examine how market participants respond to order book depth imbalances. For each depth imbalance decile, we calculate the percentage of total volume that is buyer or seller initiated. Given that depth imbalances predict future returns, we expect strategic traders to trade in the direction of the order book imbalance. Specifically, we expect more aggressive buying (i.e., more buyer initiated trades) when a large positive depth imbalance exists and more aggressive selling when there are large negative imbalances. Consistent with strategic trading, our full market results in Figure 1, Panel B confirm a strong positive (negative) relationship between the size of the depth imbalance and the percentage of buyer (seller) initiated trade volume. In the next section, we investigate whether some trader types trade more strategically than other traders based on order book depth imbalances. 

Table 2, Panel A, presents the associated depth imbalance levels and corresponding average volume of shares traded for each depth imbalance decile. We find that the market participants are more active when a large depth imbalance exists in the order book. The average number of shares traded is over 340,000 shares for each of the most extreme depth imbalance deciles (i.e., deciles 0 and 9) but approximately 270,000 shares when the order book is relatively balanced (i.e, deciles 4 and 5). This finding supports the theoretical prediction of Cespa and Vives (2017), who show that traders demand more liquidity when the market becomes less liquid. Interestingly, we find that HFT are more active in the extreme deciles while Institutions and Retail are more active when only a moderate depth imbalance exists. 

## [Insert Table 2]

## 3.2 Depth imbalance and volume imbalances by trader type

Our previous analysis shows that in aggregate, traders buy aggressively when there is a large positive depth imbalance and sell aggressively when a large negative depth imbalance exists. To investigate whether the relation between depth imbalance and trading volumes differs by trader, for each trader type, we calculate the amount of buyer and seller initiated volumes, in each decile, as a percentage of total market volume. Figure 2, Panels A to C presents the results separately for HFT, Institutions, and Retail, respectively. Consistent with the full sample results from Figure 1, Panel B, we observe a general positive (negative) relationship between depth imbalance and aggressive buying (selling) for all trader types, indicating that all traders trade in the direction of the depth imbalance. 

## [Insert Figure 2]

Comparing between the panels, HFT are more successful than Institutions and Retail when depth imbalances are very positive or very negative. Figure 2, Panel A shows that HFT buy (sell) most aggressively when depth imbalance is the most positive (negative). For Institutions (Panel B) and Retail (Panel C), the percentage of buyer (seller) initiated trades increases with the size of the positive (negative) depth imbalance for moderate levels of imbalances. However, in the extremes (i.e., when depth imbalance is very positive or very negative), both Institutions and Retail are less successful at trading in the direction of the imbalance. Retail, in particular, is less successful in trading in the direction of the depth imbalance when the imbalance is very positive (for buys) or very negative (for sells).<sup>23</sup> 

To further assess whether HFT are more successful at trading on information contained in the depth imbalance, for each stock day we calculate the executed volume imbalance that occurs at each DI decile, j, for each trader type, T. Specifically we calculate the volume imbalance as: 

$$
V o l u m e i m b a l a n c e _ {j} ^ {T} = \frac {\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} - \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}{\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} + \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}
$$

where $\begin{array} { r } { \sum _ { k = 1 } ^ { n } B u y V o l u m e _ { k , j } ^ { T } ( \sum _ { k = 1 } ^ { n } B u y V o l u m e _ { k , j } ^ { T } ) } \end{array}$ is the total aggressive buying (selling) volume, i.e., volume from the submission of market or marketable buy (sell) limit orders, for depth imbalance decile, j, initiated by trader type, T. 

Figure 2, Panel D, shows the relation between Volume imbalance and DI for our three trader types. Given that Figure 1, Panel A established that the size of DI predicts future returns, a steeper slope between Volume imbalance and DI indicates a trader is more focused on trading with the order book DI, ahead of future predicted price changes. Comparing the slopes for HFT, Institutions and Retail, our results show HFT Volume imbalance is most sensitive to an order book depth imbalance, indicating that HFT are most successful at buying aggressively before an expected price rise and selling aggressively before an expected price fall, as predicted by DI. 

In Table 2, Panel B we test whether a statistically significant difference in Volume imbalance exists between our trader types for each DI decile. When the average DI is the most negative (DI = -0.367; Depth imbalance decile 0), the volume imbalance for HFT is -61.4%, while Volume imbalance for Institutions and Retail is only -19.7% and -5.8%, respectively. For the most positive DI decile (DI = 0.382; Depth imbalance decile 9), we observe positive volume imbalances for HFT (61.7%), Institutions (19.3%) and Retail (7.0%). Finally, when the order book is balanced, such that the bid depth is approximately equal to the ask depth, the difference in the Volume imbalance is less severe. For example, when DI is only 0.035 (decile 5), the volume imbalances range from -1% (Retail) to only 6.1% (HFT), consistent with our finding in Table 2, Panel A that HFT aggressive market share % is lower when the order book is moderately flat. 

Importantly, we find that HFT Volume imbalance is always significantly below the institutional and retail Volume imbalance when a negative depth imbalance exists (i.e., there is selling pressure in the limit order book). In contrast, when buying pressure exists in the limit order book, volume imbalances are significantly larger for HFT, relative to Institutions and Retail. This result indicates that HFT are more successful at buying when the order book is predicting a future price rise and selling before expected future price declines. Further, comparing between Institutions and Retail, we find that Institutions are more strategic than Retail in trading with the imbalance in eight of the ten depth imbalance deciles. 

Brogaard, Hendershott and Riordan (2014) show that HFTs demand liquidity in the direction of the limit order book imbalance.<sup>24</sup> Our results show this behavior is not unique to HFT and that all broker types attempt to trade in the direction of a stock’s depth imbalance. However, HFT are more successful at trading on information contained in the depth imbalance than the other trader types, and the difference is even more severe at extreme levels of order book imbalances. We estimate the welfare effects of this behavior and find that HFT generate over 40% of their total profits through market order executions when the absolute size of the order book imbalance is in the most extreme decile. One implication for our results is that HFT could be crowding out non-HFT limit orders, especially when large depth imbalances exist. We formally test this hypothesis in Section 3.5. 

In Table 3, we formally test the sensitivity of volume imbalances to depth imbalances for our trader types after controlling for trading volumes, stock and day fixed effects. Using all stock day observations, we estimate the following regression: 

$$
\begin{array}{r l} {V o l u m e i m b a l a n c e _ {j} ^ {T} =} & {\beta_ {0} + \beta_ {1} I (H F T) ^ {T} \times D I _ {j} + \beta_ {2} I (I n s t i t u t i o n s) ^ {T} \times D I _ {j}} \\ & {+ \beta_ {3} I (H F T) ^ {T} + \beta_ {4} I (I n s t i t u t i o n s) ^ {T}} \\ & {+ \beta_ {5} D I _ {j} + \beta_ {6} V o l u m e _ {j} + \varepsilon_ {j} ^ {T}} \end{array}\tag{1}
$$

where $I ( H F T ) ^ { T } ( I ( I n s t i t u t i o n s ) ^ { T } )$ is 1 if trader type, T, is HFT (Institutions), and 0 otherwise. $D I _ { j }$ is the average depth imbalance for the trades in the depth imbalance decile, j, and ܸ݋݈ݑ݉݁ <sub>௝</sub> is the natural log of the total traded volume in the decile. We also include controls for stock and day fixed effects. 

$$
[ \text { Insert   Table   3 } ]
$$

Table 3, Column 1 presents the results for all trading days in the sample. The main variables of interest are the interaction terms between the trader type and DI. A positive and significant coefficient implies that a trader’s Volume imbalance is more sensitive to the level of DI in the order book. Consistent with our earlier results, we find that $I ( H F T ) \times D I$ is positive and significant indicating that relative to the other broker categories, HFT are more likely to submit buyer initiated trades when DI is larger. In contrast, ܫሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ ൈ ܫܦ is insignificant and the coefficient on DI is negative and significant indicating that Retail and Institutions trade less on order book information than HFT. 

To investigate the effects of stock volatility on HFT trading behavior, for each stock we rank trading days into terciles (low, medium, and high) based on the daily stock volatility.<sup>25</sup> Table 3, Columns 2 and 3, present the results separately for low and high volatility days, respectively. For both low and high volatility days, we find that HFT use more order book information in their trading strategies than Institutions and Retail.<sup>26</sup> Further, DI is negative and significant for all samples, indicating that Retail are less successful at trading in the direction of the expected future price movements. 

It is possible that some smaller proprietary HFT firms trade through institutional brokers. While it is difficult for these smaller HFT traders to change overall institutional volume imbalances, as shown in Table 3, Columns 1-3, these traders could influence trading imbalances based on the number of trades. To investigate this possibility, in Table 3, Columns 4-6, we replace the dependent variable from Equation (1) with trade imbalance, which is based on the number of buyer and seller initiated trades, rather than the volume of buyer and seller initiated trades. For HFT, our results are largely consistent with our findings based on volume imbalances. For Institutions, in contrast to our results based on volume imbalances, we also find that ܫሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ ൈ ܫܦ is positive and significant for the full sample (Column 4) and for the subsample of high volatility days (Column 6). This result reveals that small institutional investors behave like HFT and submit aggressive orders that capture information contained in the order book. In contrast, our volume results in columns 1-3 suggest that large trades from institutional investors are less likely to execute in the direction of the imbalance. This result could be driven by small HFT firms executing their strategies through larger institutional brokers, especially when the markets are highly volatile. Collectively, these results show that relative to non-HFT traders, HFT submit more buyer (seller) initiated orders when there are already low levels of liquidity available on the sell (buy) side of the order book. 

## 3.3 Order submission strategies

In this section, we analyze how order submission strategies differ between investor categories. Specifically, we measure the adjusted order book depth imbalance, Adjusted DI, immediately before a trader submits, amends or cancels an order. Since these orders include market orders and marketable limit orders, we are therefore also measuring Adjusted DI immediately before a trade execution takes place (i.e., when a market or marketable limit order is submitted or a limit order is executed against). We call each trade execution or the arrival of an order submission, amendment, or cancellation an order book “event”, as it will change the limit order book, either by causing an execution to occur or by otherwise adding to or altering the limit order book. 

These events are signed, in the sense that an event is classified as a “buy” if: 

1) a market or marketable limit order is submitted to remove volume from the ask side (“buy aggressive execution”), 

2) a limit order on the bid side is executed against by an incoming market or marketable limit order (“buy passive execution”), 

3) a limit order is submitted to the bid side (“buy submission”), or 

4) in the case of cancelations and amendments, volume is subtracted from the bid side (and so is a “buy cancelation” or “buy amendment”), and similarly for “sell” events. 

As discussed earlier, to remove the effects of trade direction, we multiply DI by an indicator for whether the order or trade is a buy or sell, resulting in the Adjusted DI measure, which allows purchases and sales to be interpreted together. An Adjusted DI value of 0 indicates that the order book is balanced, while a high positive Adjusted DI value indicates a large depth imbalance in the same direction as the order book event.<sup>27</sup> For example, a negative Adjusted DI at the time of a buy trade indicates that a trader is buying when the ask depth exceeds the bid depth. Since a larger ask depth, relative to the bid depth, is associated with an expected future price fall, a negative Adjusted DI at the time of a buy trade indicates that a trader is buying before an expected future price fall. Thus, a strategic trader who uses information contained in the order book should execute trades when Adjusted DI is highly positive and cancel or amend orders when Adjusted DI is low or negative. 

For each stock day, we estimate the daily average Adjusted DI for each trader type, T, and order book event, E, which we will refer to as ܣ݆݀ ݐݏݑ ݁݀	 ܫܦ <sub>ா</sub><sup>்</sup>. The order book events comprise of: aggressive executions (i.e., market or marketable limit order), passive executions, order submissions, amendments, and cancelations. Using all stock day observations, we estimate the following regression for each trader type: 

$$
\begin{array}{r l} A d j u s t e d D I _ {E} ^ {T} = & \beta_ {0} ^ {T} + \beta_ {1} ^ {T} I (A g g r e s s i v e e x e c u t i o n) _ {E} ^ {T} + \beta_ {2} ^ {T} I (P a s s i v e e x e c u t i o n) _ {E} ^ {T} \\ & + \beta_ {3} ^ {T} I (A m e n d) _ {E} ^ {T} + \beta_ {4} ^ {T} I (C a n c e l) _ {E} ^ {T} + \beta_ {5} ^ {T} V o l a t i l i t y \\ & + \beta_ {6} ^ {T} V o l u m e + \beta_ {7} ^ {T} P r i c e + \beta_ {8} ^ {T} S p r e a d + \varepsilon_ {E} ^ {T} \end{array} \tag {2}
$$

ሻ<sub>ா</sub>݊݋݅ݐݑ݁ܿݔ݁	݁ݒ݅ݏݏ݁ݎ݃݃ܣሺܫ where <sup>்</sup> is an indicator variable equal to 1 if the event, E, is a market or marketable limit order, and 0 otherwise. ܫሺܲܽ ݏݏ ݅ݒ݁	݁ݔ݁ܿ ݐݑ ݅݋݊ሻ<sub>ா</sub> ሻ<sub>ா</sub>݉݁݊݀ܣሺܫ <sup>்</sup>, <sup>்</sup>, and ܫሺܥ݈ܽ݊ܿ݁ሻ<sub>ா</sub><sup>்</sup> have a similar representation if the event is a passive execution, order amendment or order cancelation, respectively. Limit order submissions are captured in the constant term. All stock control variables are measured at the daily level. Volatility is the standard deviation of 30-minute mid-quote returns, Volume is the daily dollar volume, Price is the value-weighted average price and Spread is the time-weighted quoted spread. We also control for stock and day fixed effects. 

Consistent with our strategic trading hypothesis, we find that HFT trade aggressively when a large depth imbalance exists in the order book, and cancel or amend orders when the order book imbalance moves against them. Table 4, Column 1, shows that both I(Aggressive execution) at 0.091 and I(Passive execution) at 0.020 are positive and significant indicating that on average, trades take place when the depth imbalance is larger than the depth imbalance at the time of a limit order submission, which is captured in the constant term. The difference between the coefficients on the aggressive and passive executions is statistically different at the 1% level and suggest that HFTs submit market orders when the order imbalance is larger and suggests future prices will move in the direction of their trade, while their resting limit orders, which still execute under favorable order imbalances, do so when the order imbalance is smaller. Further, we find that I(Amend) and I(Cancel), (-0.018 and -0.046, respectively), are negative and significant, indicating HFT are quick to amend or cancel orders when the depth imbalance becomes less favorable to trade. In doing so, HFT remove stale limit orders before these orders can be picked off the order book by other traders. 

## [Insert Table 4]

We find institutions and retail investors are generally less strategic than HFT at trading on information contained in the limit order book. Similar to HFT, institutions submit aggressive orders, resulting in aggressive executions, when the depth imbalance is in the same direction (0.031; Table 4, Column 2). However, for their limit order strategies, the coefficient on I(Passive execution) at -0.025 is negative and significant while the coefficient on I(Cancel) at 0.007 is positive and significant, although notably smaller. Together, these results indicate that institutions fail to cancel their resting limit orders when the depth imbalance moves in an unfavorable direction, meaning that their stale orders are more likely to be picked off the limit order book.<sup>28</sup> 

For Retail, Table 4, Column 3 reveals that coefficient on I(Passive execution) at -0.051 is negative and significant indicating that retail limit orders are also picked off the limit order book. Further, the negative and significant coefficient for I(Aggressive execution) at -0.071 suggests that retail investors are also unable to strategically time their market orders. Taken together, these result shows that retail investors buy (either through passive or aggressive orders) before an expected fall in the stock price and sell before an expected price rise. 

In Table 4, Columns 4 to 6, we replace the dependent variable with Adjusted DI based on the depth available at the best bid and ask prices (i.e., 1 level of the order book). This test allows us to compare whether some traders are only trading on information contained in the top level of the order book. The results for the first level of the limit order book in columns 4 to 6 of Table 4 are broadly consistent with the previous results for the best five continuous limit order book levels in columns 1 to 3, with some minor differences. Specifically, comparing Table 4, Columns 1 and 4, we find that for HFT, the coefficients are similar in sign and significance using either 5 levels or 1 level of order book information. One exception is I(Passive execution), which for HFT is positive and significant when Adjusted DI is calculated using 5 levels of the order book but insignificant when the dependent variable is based on the top level of the order book. The insignificant coefficient on I(Passive execution) in column 4 but positive and significant in column 1 suggests that HFT use information contained in the order book, beyond the best bid and ask levels, when determining whether they should leave an order on the book when it is likely to be executed in the near term. The statistically significant coefficient on I(Cancel) in Column 4 of - 0.273 is large in absolute value and larger than the equivalent coefficient in column 1 (-0.046), suggesting that HFTs are more likely to cancel when the top of the book becomes unfavorable, which is consistent with the insignificant results for I(Passive execution) in that the passive executions can only happen if the order wasn’t previously cancelled (which would have already happened for large imbalances based on the large cancel coefficient). 

In Table 4, Column 5, the negative coefficients on I(Amend) of -0.058 and I(Cancel) of - 0.026 show that Institutions are more likely to cancel and amend orders when the Adjusted DI for the top level of the order book is unfavorable. However, I(Passive execution) remains negative and significant at -0.093, indicating that institutional limit orders are picked off the limit book. For Retail, the results in Column 6 are similar to the results reported earlier using 5 levels of the order book. One exception is I(Aggressive execution), which is now positive and significant, indicating that retail traders focus more on the top of the order book in their trading decisions and cross the spread when there is a large favorable depth imbalance based only on the best bid and ask volumes. 

Thus, when a retail investor wishes to buy (sell), and a large limit order queue exists on the best bid (ask) price, they are more likely to demand immediacy by submitting an aggressive market order and hitting the ask (bid) on the opposite side. Overall, our results provide further support for the conclusion that HFT are more successful at monitoring the limit order book, particularly past the best bid or ask, than other trader types. To avoid stale limit orders, HFT cancel or amend their resting limit orders when the order book depth imbalance moves in an unfavorable direction. 

To further investigate the order submission behavior of HFT, we use a multinomial logistic regression model to assess the probability of each order book event based on the prevailing market conditions in the limit order book. For each trader type, T, using all observations for each stock individually, we estimate the following regression controlling for stock and day fixed effects:<sup>29</sup> 

$$
\begin{array}{r l} {O r d e r B o o k E v e n t _ {E} ^ {T} =} & {\beta_ {0} ^ {T} + \beta_ {1} ^ {T} A d j u s t e d D I _ {E} ^ {T} + \beta_ {2} ^ {T} V o l a t i l i t y} \\ & {+ \beta_ {3} ^ {T} V o l u m e + \beta_ {4} ^ {T} P r i c e + \beta_ {5} ^ {T} S p r e a d + \varepsilon_ {E} ^ {T}} \end{array}\tag{3}
$$

݁݊ݒܧ݇݋݋ܤݎ݀݁ݎܱ where $t _ { E } ^ { T }$ is the dependent variable indicating one of five order book events, E: Aggressive execution, passive execution, limit order submission, amendment or cancelation. ݁݀ݐݏݑ݆݀ܣ $D I _ { E } ^ { T }$ , Volatility, Volume, Price and Spread are defined as in Equation (2). We estimate the model with limit order submission as the baseline category. 

$$
[ \text { Insert   Table } 5 ]
$$

Table 5, Panel A presents the regression coefficients for HFT. Consistent with our expectations, we find that Adjusted DI is positive for aggressive executions. Thus, when Adjusted 

DI is large, HFT are more likely to submit a market (or marketable limit) order, than a less aggressive limit order. Similarly, Adjusted DI is positive for passive executions, meaning that limit order trade executions are more likely than a limit order submission when Adjusted DI is large. In contrast, the coefficient on Adjusted DI is negative for amendments and cancelations. When Adjusted DI is lower, HFT are more likely to amend or cancel an order than to submit a limit order. These results are consistent with strategic HFT order placement strategies. HFT trade when there is a large favorable order book depth imbalance and cancel or amend their resting limit orders when the imbalance moves in an unfavorable direction. 

Table 5, Panels B and C show that Institutions and Retail are less strategic in their order placement strategies. While Institutions are more likely to submit aggressive market orders when the Adjusted DI is large, both Institutions and Retail are more likely to receive a limit order execution when Adjusted DI is lower (coefficients of -11.3 and -4.57, respectively), relative to Adjusted DI at the time of order submission. Consistent with our earlier findings, this result indicates that Institutions and Retail are less successful at monitoring the limit order book and are more likely to face picking-off risk due to stale orders resting in the book. 

So far, our findings indicate that HFT actively monitor the order book and thus, large depth imbalances, which are strong predictors of future price movements, should not persist in the order book for extended periods of time. Figure 3, Panel A shows the inverted U-shaped relationship between the size of an order book depth imbalance and the median time the limit order book remains within the depth imbalance decile.<sup>30</sup> We find that large imbalances (i.e., deciles 0 and 9) persist for a much shorter period of time than more balanced order books (i.e., deciles 4 and 5). Our results indicate that large buy (sell) imbalances remain for a median time of only 34 milliseconds (121 milliseconds), while an order book that is relatively balanced remains in the same decile for a median time of approximately 1.4 seconds, more than 40 times longer. Given the rapid changes in the state of the order book, it is likely that only HFT are able to participate effectively in the extreme depth imbalance deciles. Consistent with this intuition, Figure 3, Panel B show that HFT are more active in the extreme depth imbalance deciles, relative to when the order book is more balanced, resulting in a strong U-shaped pattern. In contrast, Institutions and Retail, who are less able to compete on speed, reduce their activity when large imbalances exist in the order book (Figure 3, Panels C and D), resulting in a strong inverted U-shaped pattern. 

[Insert Figure 3] 

## 3.4 Volatility and HFT strategies

In this section, we further investigate HFT trading behavior in times of high market volatility. We divide each trading day into 30 minute intervals and for each interval, measure its volatility by taking the natural log of the high price divided by the low price during the period. For each stock, we then rank the 30 minute intervals into 10 deciles based on its volatility. Decile 0 (9) contains the least (most) volatile periods. For each trader type, we also determine the amount of aggressive volume (i.e., due to market or marketable limit order submissions) and passive volume (i.e., limit order executions resulting from an incoming market or marketable limit order), as a percentage of their total volume, in each decile. Figure 4, Panels A to C present the graphs of volatility against aggressive and passive volumes for HFT, Institutions, and Retail, respectively. 

If HFT trade to decrease market volatility, we expect them to supply more passive volume in times of high market uncertainty. In contrast, Figure 4, Panel A shows that HFT aggressive volume increases while their passive volume decreases as the market becomes more volatile. For 

Institutions in Figure 4, Panel B, we observe a fall in aggressive volumes as volatility increases, which is consistent with Institutions withdrawing from the market in periods of high uncertainty. For Retail, with higher stock volatility, we observe a sharp decrease in aggressive volume (Figure 4, Panel C). For both Institutional and Retail, passive volume increases when the market becomes more volatile. This trading pattern could indicate that stale institutional and retail limit orders are picked off the limit order book by aggressive HFT orders during volatile periods and that retail and institutional brokers supply liquidity in times of need. 

We test the relationships observed in Figure 4 more formally using the following regression model, controlling for stock and day fixed effects: 

$$
A g g r e s s i v e v o l u m e \mathbb {\Phi} _ {I} ^ {T} = \beta_ {0} + \beta_ {1} V o l a t i l i t y _ {I} + \beta_ {1 0} V o l u m e _ {I} + \varepsilon\tag{4}
$$

݉݁ݑ݈݋ݒ	݁ݒ݅ݏݏ݁ݎ݃݃ܣ ,variable dependent the where $\% _ { I } ^ { T }$ ,	is the aggressive volume as a percentage of total aggressive and passive volume for each broker type, T, that is executed in the 30 minute interval, I. For each time interval, I, Volatility is the natural log of the high price divided by the low price and Volume is the total number of shares traded. We estimate Equation (4) separately for each trader type. 

Panel A of Table 6 shows that HFT Aggressive volume % increases with stock volatility (Column 1, coefficient of 447.6), consistent with our observations from Figure 4. This finding is similar across both large stocks and small stocks in Columns 2 and 3. In contrast, for institutional and retail traders in Table $^ { 6 , }$ Panels B and $\mathrm { C } ,$ we find that Aggressive volume % generally decreases when stock volatility increases (coefficients of -84.7 and -174.3, respectively). These results support Boehmer, Li and Saar (2016), who find that short-horizon directional HFT strategies are more active when a thin order book exists and markets are volatile. Taken together, our results show that HFT trade more aggressively in times of high market volatility. 

Our results contrast Brogaard et al. (2016), who find that HFTs supply liquidity during extreme price movements for a single stock, using a subsample of Nasdaq trades. One possible explanation for their findings is that HFT could be providing liquidity on Nasdaq while taking liquidity from other markets.<sup>31</sup> Our results further reveal that that it is important to investigate consolidated trading volumes when analyzing overall HFT behavior. 

[Insert Table 6] 

To test whether HFT are more strategic in times of market volatility, we investigate the relationship between Adjusted DI and stock volatility for each broker category. As discussed earlier, Adjusted DI measures a trader’s ability to condition their trades on information contained in the order book. Specifically, a positive Adjusted DI indicates that a trade executes in the direction of a favorable imbalance. Thus, Adjusted DI is more positive for traders better able to trade in the direction of the imbalance, or capture predicted future price movements based on the shape of the order book. For each market volatility decile, we calculate the average Adjusted DI for both the aggressive and passive executions in the decile. 

[Insert Figure 5] 

Figure 5, Panels A and B, present the average Adjusted DI for aggressive and passive executions, respectively. Comparing between the broker categories, we observe a large difference in trading behaviors. Notably, for both passive and aggressive executions, we observe a sharp increase in Adjusted DI for HFT as stock volatility increases. 

In contrast, for HFT and Institutions, Adjusted DI is relatively flat across the volatility deciles for their aggressive executions (Figure 5, Panel A) while for their passive executions (Figure 5, Panel B), Adjusted DI decreases with rising market volatility. This finding supports our hypothesis that non-HFT limit orders are picked off the thin side of the order book, especially in times of high market uncertainty. When the market is volatile, limit orders from slower traders could potentially become stale, leaving more opportunities for faster, more sophisticated traders. 

We test the relationship between Adjusted DI and stock volatility more formally using a regression framework, after controlling for stock and day fixed effects. 

$$
\begin{array}{r l} {A d j u s t e d D I _ {I} ^ {T} = \beta_ {0} + \beta_ {1} I (H F T) ^ {T} \times V o l a t i l i t y _ {I} + \beta_ {2} I (I n s t i t u t i o n s) ^ {T} \times V o l a t i l i t y _ {I}} \\ & {+ \beta_ {3} I (H F T) ^ {T} + \beta_ {4} I (I n s t i t u t i o n s) ^ {T} + \beta_ {5} V o l a t i l i t y _ {I} + \beta_ {6} V o l u m e _ {I} + \varepsilon_ {I},} \end{array}\tag{5}
$$

݁݀ݐݏݑ݆݀ܣ where $D I _ { I } ^ { T }$ is the average Adjusted DI for trades by trader T in the 30 minute interval, I. $I ( H F T ) ^ { T } ( I ( I n s t i t u t i o n s ) ^ { T } )$ is 1 if trader type, T, is HFT (Institutions) and 0 otherwise and $V o l a t i l i t y _ { I }$ and $V o l u m e _ { I }$ are defined as in Equation (4). 

We estimate the regression separately for aggressive and passive executions. Table 7, Column 1 presents the results for aggressive executions based on the full sample of stocks. As expected, we find for HFT, Adjusted DI is larger when the market is more volatile, indicating that HFT are more strategic when uncertainty exists. Comparing the results for large and small stocks (Table 7, Columns 2 and 3), we show that the relationship between Adjusted DI and volatility is driven by the large stock sample. This finding supports the notion that HFT are likely to benefit more from trading speed differentials when trading in larger, more liquid stocks, in which trading is typically faster. 

## [Insert Table 7]

Table 7, Columns 4 to 6 present the regression coefficients for passive executions. Consistent with our earlier results, we find that HFT are able to successfully implement limit order strategies, especially when the market is volatile. Relative to Retail passive orders, which is captured in the intercept coefficient, HFT passive orders execute with a larger Adjusted DI, when more stock volatility exists (the coefficient on ܫሺ ܨܪ ܶሻ ൈ ܸ݋݈ܽݐ݈݅݅ ݕݐ is 5.224). While Institutions exhibit similar trading behaviors to HFT, the magnitudes of the coefficients are significantly lower (the coefficient on ܫሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ ൈ ܸ݋݈ܽݐ݈݅݅ ݕݐ is 1.621). This finding supports our hypothesis that HFT are more successful at monitoring their limit orders, in particular, when there is high stock volatility. One further implication of our results is that HFT aggressively pick off stale orders from the thin side of the order book, particularly when the market is already highly volatile. 

## 3.5 Introduction of ITCH

Using a difference-in-difference framework, we exploit a natural experiment to investigate whether an increase in trading speed affects HFT behavior. On April 2, 2012, the ASX implemented ASX ITCH, which increased market information access speeds for a monthly subscription fee. While subscribing to ASX ITCH is voluntary, and the identity of subscribing brokers is confidential, it is reasonable to assume that traders who are most speed sensitive will be the first to subscribe to the faster data feed. To leave sufficient time for implementation, the pre-ITCH period is the one-month period prior to April 2, 2012 (i.e., March 2, 2012 to March 30, 2012) and the post-ITCH period begins one week after the introduction of ITCH and ranges from April 9, 2012 to May 9, 2012.<sup>32</sup> 

Given that HFT strategies are most likely to benefit from the faster trading speeds, we expect that HFT Volume imbalance is more sensitive to the level of DI after switching to ITCH. On the other hand, the slope of the relationship between Volume imbalance and DI is less affected for Retail and Institutions, who are less speed sensitive. To empirically assess whether ITCH affects trading behavior, we use a difference-in-difference framework and re-estimate Equation (1) after including two interaction terms, $I ( P r e )$ and I(Post), which are indicator variables indicating whether the observation occurs on a trading day before or after the introduction of ITCH. The regression specification is now: 

$$
\begin{array}{r l} V o l u m e i m b a l a n c e _ {j} ^ {T} = & \beta_ {0} + I (P r e) [ \beta_ {1} I (H F T) ^ {T} \times D I _ {j} + \beta_ {2} I (I n s t o) ^ {T} \times D I _ {j} + \beta_ {3} D I _ {j} ] \\ & + I (P o s t) [ \beta_ {4} I (H F T) ^ {T} \times D I _ {j} + \beta_ {5} I (I n s t o) ^ {T} \times D I _ {j} + \beta_ {6} D I _ {j} ] \\ & + \beta_ {7} I (H F T) ^ {T} + \beta_ {8} I (I n s t o) ^ {T} + \beta_ {9} V o l u m e _ {j} + \varepsilon_ {j} ^ {T} \end{array} \tag {6}
$$

We run the tests in Table 8 on buy volume imbalances and buy trade imbalances. Table 8, Columns 1 and 3, report the two sets of coefficients $\{ \beta _ { 1 } , \beta _ { 2 } , \beta _ { 3 } \}$ and $\{ \beta _ { 4 } , \beta _ { 5 } , \beta _ { 6 } \}$ . Table 8, Column 4 reports the test of equality between $\beta _ { 1 }$ and $\beta _ { 4 } \left( \mathrm { i . e . , } \beta _ { 4 } - \beta _ { 1 } = 0 \right)$ , which indicates whether HFT strategies capture more information contained in the order book depth imbalance after the implementation of ITCH. Similarly, Table 8, Column 4 also reports the test of equality between $\beta _ { 2 }$ and $\beta _ { 5 }$ , and $\beta _ { 3 }$ and $\beta _ { 6 }$ , which tests whether institutional and retail strategies change as a result of ITCH, respectively. Lastly, the coefficients for $\beta _ { 7 }$ and $\beta _ { 9 }$ and the intercept term are reported in Table 8, Column 2. 

[Insert Table 8] 

Table 8, Columns 1 and 3 show that $\beta _ { 1 }$ and $\beta _ { 4 }$ are both positive and significant (0.942 and 1.064, respectively) indicating that HFT buy when DI is positive and sell when DI is negative in both the pre- and post-ITCH periods. Importantly, the estimate of $\beta _ { 4 }$ is larger than $\beta _ { 1 }$ and the Ftest in Column 3 (F-test = 5.35) shows that the difference is statistically significant at the 5% level. This result indicates that for HFT, the slope of Buy Volume imbalance against DI is steeper in the post-ITCH period. As a group, HFT trade more strategically on information contained in the limit order book as their market information access speeds increase. In contrast, we cannot reject the null hypothesis that $\beta _ { 2 } = \beta _ { 5 }$ and $\beta _ { 3 } = \beta _ { 6 }$ . Consistent with our expectations, we do not find evidence that non-HFT, who are less speed sensitive, trade more strategically after the adoption of ITCH. 

In Table 8, Columns 4 to 6, we replace the dependent variable with buy trade imbalance. Similar to our results based on buy volume imbalances, we find that HFT trade more strategically post-ITCH (F-test = 7.71). For Institutions, we also find that their trading is more sensitive to DI after the implementation of ITCH (F-test = 5.27). Consistent with our earlier results, it is possible that some more speed sensitive institutional brokers also subscribed to ITCH, on behalf of their smaller HFT clients, to take advantage of the faster speeds. While it is difficult for a small HFT trader to influence average volume imbalances for the broker, we find that their number of buy and sell orders capture more information contained in order book depth imbalances after trading becomes faster. Based on trade imbalances, we find that Retail, who are less likely to compete on speed, trade less strategically post-ITCH. Specifically, we find that $\beta _ { 6 }$ is negative and significant at -0.121 in the post-ITCH period. 

So far, our results show that HFT are more successful at trading on information contained in the order book imbalance when their trading becomes faster. One implication for these results is that non-HFT traders could be crowded out of the order book as HFT compete to trade in the same direction as non-HFT. We investigate whether HFT have a crowding out effect by measuring the probability of execution for HFT and non-HFT limit orders. 

$$
P (F i l l) ^ {T} = \frac {\sum T r a d e V o l u m e ^ {T}}{\sum S u b m i t V o l u m e ^ {T}}
$$

݉݁<sup>்</sup>ݑ݈݋ܸݐܾ݉݅ݑܵ ∑ where is the total daily volume submitted to the top level of the limit order book by trader type, T, and $\sum$ ܶݎܸܽ݀݁݋݈ݑ݉݁<sup>்</sup> is the total volume of orders submitted to the top of the order book by trader type, T, which is executed. For each stock, we measure $P ( F i l l ) ^ { T }$ on a daily basis for each trader type. We then estimate the following regression model: 

$$
\begin{array}{r l} & P (F i l l) ^ {T} = \beta_ {0} + \beta_ {1} I (N o n - H F T) ^ {T} \times I (P o s t) \\ & \qquad + \beta_ {2} I (N o n - H F T) ^ {T} + \beta_ {3} I (P o s t) + \beta_ {4} V o l a t i l i t y \\ & \qquad + \beta_ {5} V o l u m e + \beta_ {6} P r i c e + \beta_ {7} S p r e a d + \varepsilon^ {T} \end{array}\tag{6}
$$

where $I ( N o n - H F T ) ^ { T }$ is an indicator variable equal to 1 if trader type T is an institutional or retail trader, and 0 for an HFT trader and I(Post) is an indicator variable equal to 1 for the post-ITCH period, and 0 for the pre-ITCH period. All other control variables are measured on a daily basis. Volatility is the standard deviation of 30-minute mid-quote returns, Volume is the daily dollar volume, Price is the value-weighted average price and Spread is the time-weighted quoted spread. We also control for stock and day fixed effects. 

[Insert Table 9] 

Our main variable of interest is $I ( N o n - H F T ) ^ { T } \times I ( P o s t )$ . If HFT are crowding out non-HFT limit orders from the order book, we expect a negative coefficient for $I ( N o n - H F T ) \times$ ܫሺܲ ݐݏ݋ ሻ, indicating that the probability of a non-HFT order receiving execution decreases when HFT become faster. Consistent with our expectations, Table 9, Column 1 shows that the probability of limit order execution falls for non-HFT after the introduction of ITCH (coefficient on $I ( n o n - H F T ) \times I ( P o s t )$ is -0.037. In Table 9, Column 2, we separate non-HFT traders into Institutions and Retail. For both Institutions and Retail, we find the interaction term with I(Post) is negative and significant (-0.021 and -0.058, respectively), indicating that both Institutions and Retail are crowded out from the order book by HFT. 

To further investigate the crowding out effect on non-HFT traders, in Table 9, Columns 3 to 6, we decompose P(Fill) into favorable and unfavorable fills. We define a favorable fill as an order execution when the limit order rests on the side of the order book with more depth immediately prior to the trade. From our earlier results, we show that a limit order trader benefits when an order executes with a lot of depth on the same side of the order book (i.e., favorable fill). On the other hand, if depth builds up on the opposite side of the order book, a limit order is likely to face adverse selection (i.e., unfavorable fill). 

Our results show that the decrease in P(Fill) is driven by a fall in the volume of favorable executions. Comparing between Columns 3 and 5, we find that P(Favorable fill) falls for non-HFT after the implementation of ITCH (I(Non-HFT)xI(Post) has a coefficient of -0.04) while P(Unfavorable fill) remains unchanged after the implementation of ITCH. Separating non-HFT into Institutions and Retail in Columns 4 and 6, we document similar findings. Specifically, the interaction terms with I(Post) is negative and significant at -0.029 and -0.051 for Institutions and Retail, respectively, in Column 4 and insignificant in Column 6. Thus, the likelihood of receiving a favorable limit order execution falls for both institutional and retail traders when HFT gain a speed advantage. Taken together, these results provide evidence that HFT are crowding out non-HFT limit orders from the order book, especially when trading becomes faster. These findings are consistent with Van Kervel and Menkveld (2016) and Korajczk and Murphy (2016), who report an increase in institutional trading costs increase when HFTs compete in the same direction with institutional orders. 

## 4.0 Conclusion

The information channels through which HFT trade are relatively unknown. We present strong evidence of one such channel, which provides an explanation for many of the findings documented in the prior literature. We show that order book depth imbalances are strong predictors of future prices. HFT are highly sophisticated in monitoring order book imbalances, which allows them to trade ahead of these predicted price changes. At the same time, when the order book imbalance moves in an unfavorable direction, they are quick to cancel or amend orders that are at high risk of being picked off by other traders. However, this strategic HFT behavior has potential negative welfare effects on slower traders. A strategy using fast market orders to pick of stale limit orders when the size of the order imbalance is in the largest size decile contributes over 40% to overall HFT trading revenues. 

HFT order placement strategies based on order book imbalances are particularly successful when the market is volatile. During times of high market volatility, the chance of an institutional or retail limit order becoming stale increases. We find that HFT trade more aggressively and are more successful at picking off stale orders from institutional and retail investors when the market is volatile. However, by demanding liquidity from the thin side of the order book, one consequence is that HFT could potentially exacerbate future limit order book imbalances. 

Using the introduction of ITCH as a natural experiment, we find that HFT become even better at acting on information contained in the order book when their trading becomes faster. However, by competing for favorable trade execution in the same direction as the buying or selling pressure, HFT have a crowding out effect on non-HFT limit orders, which potentially increases non-HFT limit order execution costs. 

Our results on HFT trading behavior have implications for market quality. Several studies show that HFT enhance market quality by improving the informational efficiency of stock prices (Carrion, 2013; Brogaard, Hendershott and Riordan, 2014; Brogaard, Hendershott and Riordan, 2016). On the other hand, HFT could increase transaction costs when they trade in the same direction of the institutional order flow (van Kervel and Menkveld, 2016; Korajcyzk and Murphy, 2016). We show that HFT increase price efficiency by trading in the direction of the order book imbalance, which is a strong predictor of future price movements. However, HFT can also use the information contained in the order book imbalance to detect institutional buying or selling pressure. 

While earlier studies show that overall depth improves (Hasbrouck and Saar, 2013; Hendershott, Jones and Menkveld, 2011), when analyzing directional depth, we show that HFT supply liquidity to the order book, but only to the side where there is a lot of existing depth. In contrast, we find that HFT demand liquidity from the thin side of the order book, which is more prominent in times of high market volatility. 

## References



Aitken, M., Chen, H. and Foley, S. (2017) The impact of fragmentation, exchange fees and liquidity provision on market quality. Journal of Empirical Finance, 41, 140-160. 





Angel, J., Harris, L. and Spatt, C. 2010. Equity trading in the 21st century. Marshall School of Business Working Paper No. FBE 09-10. 





Biais, B., Foucault, T. and Moinas, S. (2015) Equilibrium fast trading. Journal of Financial Economics, 116, 292-313. 





Boehmer, E., Fong, K. and Wu, J. (2015) International evidence on algorithmic trading. SSRN Working Paper. 





Boehmer, E., Li, D. and Saar, G. (2016) Correlated high-frequency trading. SSRN Working Paper. 





Brogaard, J., Carrion, A., Moyaert, T., Riordan, R., Shkilko, A. and Sokolov, K. (2017) Highfrequency trading and extreme price movements. Journal of Financial Economics, Forthcoming. 





Brogaard, J., Hagströmer, B., Nordén, L. and Riordan, R. (2015) Trading fast and slow: Colocation and liquidity. Review of Financial Studies, 28, 3407-3443. 





Brogaard, J., Hendershott, T. and Riordan, R. (2014) High-frequency trading and price discovery. Review of Financial Studies, 27, 2267-2306. 





Brogaard, J., Hendershott, T. and Riordan, R. (2016) Price discovery without trading: Evidence from limit orders. SSRN Working Paper. 





Cao, C., Hansch, O. and Wang, X. (2009) The information content of an open limit-order book. Journal of Futures Markets, 29, 16-41. 





Carrion, A. (2013) Very fast money: High-frequency trading on the Nasdaq. Journal of Financial Markets, 16, 680-711. 





Cespa, G. and Vives, X. 2017. High frequency trading and fragility. CESifo Working Paper Series No. 6279. 





Chaboud, A. P., Chiquoine, B., Hjalmarsson, E. and Vega, C. (2014) Rise of the machines: Algorithmic trading in the foreign exchange market. The Journal of Finance, 69, 2045- 2084. 





Chordia, T., Roll, R. and Subrahmanyam, A. (2002) Order imbalance, liquidity, and market returns. Journal of Financial Economics, 65, 111-130. 





Chordia, T. and Subrahmanyam, A. (2004) Order imbalance and individual stock returns: Theory and evidence. Journal of Financial Economics, 72, 485-518. 





Comerton-Forde, C. and Putniņš, T. J. (2015) Dark trading and price discovery. Journal of Financial Economics, 118, 70-92. 





Conrad, J., Wahal, S. and Xiang, J. (2015) High-frequency quoting, trading, and the efficiency of prices. Journal of Financial Economics, 116, 271-291. 





Cont, R., Kukanov, A. and Stoikov, S. (2014) The price impact of order book events. Journal of Financial Econometrics, 12, 47-88. 





Ellis, K., Michaely, R. and O'hara, M. (2000) The accuracy of trade classification rules: Evidence from nasdaq. Journal of Financial and Quantitative Analysis, 35, 529-551. 





Foucault, T., Hombert, J. and Roşu, I. (2016) News trading and speed. The Journal of Finance, 71, 335-382. 





Hagströmer, B. and Nordén, L. (2013) The diversity of high-frequency traders. Journal of Financial Markets, 16, 741-770. 





Harris, L. (2013) What to do about high-frequency trading. Financial Analysts Journal, 69, 6-9. 





Hasbrouck, J. and Saar, G. (2013) Low-latency trading. Journal of Financial Markets, 16, 646- 679. 





Hendershott, T., Jones, C. M. and Menkveld, A. J. (2011) Does algorithmic trading improve liquidity? The Journal of Finance, 66, 1-33. 





Hirschey, N. 2016. Do high-frequency traders anticipate buying and selling pressure? London Business School Working Paper. 





Hoffmann, P. (2014) A dynamic limit order market with fast and slow traders. Journal of Financial Economics, 113, 156-169. 





Jones, C. 2013. What do we know about high-frequency trading? Columbia Business School Research Paper No. 13-11. 





Kirilenko, A., Kyle, A., Samadi, M. and Tuzun, T. (2017) The flash crash: High frequency trading in an electronic market. Journal of Finance, Forthcoming. 





Korajczyk, R. and Murphy, D. (2016) High frequency market making to large institutional trades. SSRN Working Paper. 





Lee, C. M. C. and Ready, M. J. (1991) Inferring trade direction from intraday data. The Journal of Finance, 46, 733-746. 





Li, W. 2014. High frequency trading with speed hierarchies. University of Maryland Working Paper. 





Malinova, K. and Park, A. 2016. "Modern" market makers. University of Toronto Working Paper. 





Malinova, K., Park, A. and Riordan, R. 2016. Taxing high frequency market making: Who pays the bill? University of Toronto Working Paper. 





Menkveld, A. J. (2013) High frequency trading and the new market makers. Journal of Financial Markets, 16, 712-740. 





Naes, R. and Skjeltorp, J. (2006) Order book characteristics and the volume-volatility relation: Empirical evidence from a limit order market. Journal of Financial Markets, 9, 408-432. 





Ranaldo, A. (2004) Order aggressiveness in limit order book markets. Journal of Financial Markets, 7, 53-74. 





Rosu, I. 2016. Fast and slow informed trading. HEC Paris Research Paper No. FIN-2015-1123. 





Subrahmanyam, A. and Zheng, H. (2016) Limit order placement by high-frequency traders. Borsa Istanbul Review, 16, 185-209. 





Upson, J., Johnson, H. and Mcinish, T. H. (2015) Order versus trades on the consolidated tape. SSRN Working Paper. 





Van Kervel, V. (2015) Competition for order flow with fast and slow traders. Review of Financial Studies, 28, 2094-2127. 





Van Kervel, V. and Menkveld, A. J. (2016) High-frequency trading around large institutional orders. SSRN Working Paper. 





Yao, C. and Ye, M. (2016) Why trading speed matters: A tale of queue rationing under price controls. SSRN working paper. 





Ye, M. 2017. Who provides liquidity and when: An analysis of price vs. Speed competition on liquidity and welfare. University of Illinois at Urbana-Champaign Working Paper. 



![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/f005efa231ac28460179ee2164b92dbc48ccd0e0d36ebb91762f17cc31e017e8.jpg)


## Appendix 1

In this Appendix, we show examples of how DI is constructed. Figure A1 shows two stylized diagrams of the limit order book. In the first example, the bid depth exceeds the ask depth and in the second example, the ask depth exceeds the bid depth. In Table A1, we show the calculation for DI, which is defined as: 

$$
D I _ {t} = \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}
$$

where $\textstyle \sum _ { i = 1 } ^ { n } V o l B i d _ { i , t } \ : ( \sum _ { i = 1 } ^ { n } V o l A s k _ { i , t } )$ is the volume available at the top n bid (ask) price levels immediately before the order book event, t. 


Figure A1. Limit order book examples



Each black rectangle represents a limit buy order of 100 shares and each grey rectangle represents a limit sell order of 100 shares.



Table A1. Calculation of depth imbalance (DI) based on examples in Figure A1.


<table><tr><td></td><td>Example 1</td><td>Example 2</td></tr><tr><td>DI (5 levels, n = 5)</td><td><eq>\frac{1100-500}{1100+500} = 0.375</eq></td><td><eq>\frac{500-1100}{500+1100} = -0.375</eq></td></tr><tr><td>DI (1 level, n = 1)</td><td><eq>\frac{300-100}{300+100} = 0.5</eq></td><td><eq>\frac{100-300}{100+300} = -0.5</eq></td></tr></table>

## Appendix 2

In this Appendix, we investigate the information content of resting limit orders behind the best bid and offer prices. To determine the incremental information content of resting limit orders at levels 2 to 5 of the order book, we estimate a restricted model, which only contains the depth imbalance for the best bid and offer, and an unrestricted model, which contains the DI for the best bid and offer and for levels 2 to 5 of the limit order book. For each stock and day, we perform the following regressions: 

ߝ൅<sub>௟௘௩௢௣௅௘்</sub>ܫܦ<sub>ଵ</sub>ߚ	൅<sub>଴</sub>ߚ ൌ ݊ݎݑݐܴ݁ :model Restricted 

$$
\mathrm{Unrestrictedmodel:} R e t u r n = \beta_ {0} + \beta_ {1} D I _ {T o p L e v e l} + \beta_ {2} D I _ {L e v e l s 2 - 5} + \varepsilon
$$

Return is calculated as the log of the difference between the bid-ask midpoint 10 trades in the future and the midpoint price just prior to the trade. DI is the depth imbalance immediately before the trade, which is calculated as the difference between the volumes available at the bid and ask prices as a proportion of the total volume available at the bid and ask prices. We calculate DI for the top level of the order book $( D I _ { T o p L e v e l } )$ as well as for levels 2 to 5 of the limit order book $( D I _ { L e v e l s 2 - 5 } )$ 

Table A2 summarizes the adjusted R-square for the restricted and unrestricted models. If $D I _ { L e v e l s 2 - 5 }$ adds incremental information about the future price movements, we expect a higher adjusted R-square for the unrestricted model, relative to the restricted model. For over 85% of our regressions, the F-test is significant at the 1% level, indicating that $D I _ { L e v e l s 2 - 5 }$ adds additional explanatory power. This result indicates that limit orders behind the best bid and offer also contains information on future stock returns. 

<table><tr><td rowspan="2"></td><td colspan="2">Adjusted R-square</td><td rowspan="2">% with F-test significant at 1%</td></tr><tr><td>Restricted model</td><td>Unrestricted model</td></tr><tr><td>Mean</td><td>12.02%</td><td>13.48%</td><td rowspan="2">85.64%</td></tr><tr><td>Median</td><td>10.96%</td><td>12.45%</td></tr></table>


Table A2. Adjusted R-square for restricted and unrestricted model.


## Appendix 3

In this Appendix, we investigate whether HFT successfully use their order placement strategies to buy before future price rises and sell before future price falls. Specifically, for each active (i.e., market or marketable limit order) and passive execution, we calculate the price impact and realized spread as: 

$$
P r i c e I m p a c t = q _ {t} \times \frac {m _ {t + 1 0} - m _ {t}}{m _ {t}}
$$

$$
R e a l i z e d s p r e a d = q _ {t} \times \frac {p _ {t} - m _ {t + 1 0}}{m _ {t}}
$$

where $m _ { t }$ is the bid ask midpoint at the time when the current trade takes place, $m _ { t + 1 0 }$ is the bid ask midpoint in 10 trades’ time, and $p _ { t }$ is the trade price. Because each execution consists of both an active and passive side, we calculate the price impact and realized spread for both the active and passive parties to each trade. For active executions, the buy sell indicator, $q _ { t } ,$ equals 1 (-1) if the trade is buyer (seller) initiated. For passive executions, $q _ { t }$ equals 1 (-1) if the existing limit order is resting on the bid (ask) side of the limit order book. 

For active executions, we find that HFT outperform both institutional and retail market orders. The equally weighted average price impact for HFT is 7.38 basis points while the average price impact for institutional and retail is only 3.05 and 3.54 basis points, respectively. Consistent with this result, we also find that realized spreads for HFT active executions are larger than Institutions and Retail.<sup>33</sup> 

Importantly, our results show that HFT are able to successfully time their passive executions. On average HFTs earn 0.46 basis points per limit order execution, based on comparing the current bid-ask midpoint price with the bid-ask midpoint 10 trades into the future. This return increases to 1.04 basis points when we include the transaction price (i.e., a buy limit order transacts at the bid price, rather than at the bid-ask midpoint). In contrast, the price impact and realized spreads of institutional and retail limit orders are consistently negative, indicating that their orders are picked off the limit order book. Taken together, these results indicate that HFT have superior market timing abilities, relative to Institutions and Retail. 


Table A3. Price impact and realized spreads by trader type


<table><tr><td rowspan="2"></td><td colspan="2">Active executions (bps)</td><td colspan="2">Passive executions (bps)</td></tr><tr><td>Price impact</td><td>Realized spread</td><td>Price impact</td><td>Realized spread</td></tr><tr><td>HFT</td><td>7.383</td><td>-0.768</td><td>0.460</td><td>1.038</td></tr><tr><td>Institutions</td><td>3.049</td><td>-5.120</td><td>-2.665</td><td>-4.211</td></tr><tr><td>Retail</td><td>3.539</td><td>-6.114</td><td>-1.670</td><td>-20.76</td></tr><tr><td>HFT - Institutions</td><td>4.334 ***</td><td>4.352 ***</td><td>3.125 ***</td><td>5.249 ***</td></tr><tr><td>HFT - Retail</td><td>3.844 ***</td><td>5.346 ***</td><td>2.131 ***</td><td>21.80 ***</td></tr><tr><td>Institutions - Retail</td><td>-0.490 ***</td><td>0.995 ***</td><td>-0.995 ***</td><td>16.55 ***</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/4a050156e496eac7e3c9098c43f04075f7601277b6899b9ca1a7b547066e43b7.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/9a561a5c0b207cc76fd563d54c78f796154eca814702bc115f1fe7bb74603430.jpg)



Fig. 1. Fig. 1 shows the relationship between depth imbalance, returns (Panel A) and volumes (Panel B). Depth imbalance is calculated as the difference between the depths available at the five best bid and ask prices, scaled by total depth available at these price levels, immediately before each trade. For each stock day, we rank trades into 10 depth imbalance deciles. Trades with the most negative depth imbalances (i.e., bid depth << ask depth) are categorized as decile 0 and trades with the most positive depth imbalances (i.e., bid depth >> ask depth) are in decile 9. In Panel $\mathbf { A } ,$ we calculate returns by comparing the current midpoint of the best bid and ask prices with the midpoint price 10 trades in the future. In Panel B, the blue circles (red triangles) represent the average percentage of buyer (seller) initiated volume, relative to total trade volume, for each depth imbalance decile.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/14caeb67f36fbc9e39adf3d2a41d123fd8e040aeee462741215b8564d7aee136.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/427698b26d2e5234196a9e03d871cdf8f9d8ed8befdbc2ea2c2994d1569ebb15.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/d69da236a2a06778693b401c52897f4427ec4a4d56b62aa2b91439dca0745f7a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/9e5cf8e22efae3e3ce2cd9d5de7639101c20b4cafdd3529de7d44c088f9f9aa8.jpg)



Fig 2. Fig. 2 shows the relationship between depth imbalance and trading volumes for each broker category. Depth imbalance is calculated as the difference between the depths available at the five best bid and ask prices, scaled by total depth available at these price levels, immediately before each trade. For each stock day, we rank trades into 10 depth imbalance deciles. Trades with the most negative depth imbalances (i.e., bid depth << ask depth) are categorized as decile 0 and trades with the most positive depth imbalances (i.e., bid depth >> ask depth) are in decile 9. Panels A-C present the results for HFT, Institutions, and Retail, respectively. The blue circles (red triangles) represent the average percentage of buyer (seller) initiated volume, relative to total trade volume, for each depth imbalance decile and broker type. Panel D shows the volume imbalance (i.e., (Buys-Sells)/(Buys + Sells)) for each broker type and depth imbalance decile.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/debd50032d7afba180dd44b06fe5e1c57c9d1606892cefd4c3b90ef2862ea013.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/da916c303fc944ac49334eb32e2a2bd2dddd16b5d0c387f063e07a19210559d4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/4aa6827c7434c737b52f06e9718a5f80147c70b4cc3b7664701e0e88ce8ccd7d.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/d956bb2bf29961bccc1b68281f1eef7a49d91ecb2bee6348db8bcc82c6f8092d.jpg)



Fig. 3. Fig. 3 shows the relationship between depth imbalance and the median time the order book remains in each depth imbalance decile (Panel A) and market shares for HFT, Institutions and Retail (Panels B to D). In Panel A, we compute the depth imbalance for all order book events (submission, cancelation, amend, trade) and rank the depth imbalances into deciles. For all observations, we determine the time the order book remains within the same depth imbalance decile. Panel A plots the median time (seconds) the order book remains in each depth imbalance decile. For Panels B to D, we rank trades into 10 depth imbalance deciles for each stock day. Trades with the most negative depth imbalances (i.e., bid depth << ask depth) are categorized as decile 0 and trades with the most positive depth imbalances (i.e., bid depth >> ask depth) are in decile 9. Panels B to D plot the average daily market share per stock (based on aggressive orders) for each broker type and depth imbalance decile.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/e9c62fcf0ed9e5b1ab85b23e4fa4ce1cdfc9f7356076e0eae86c5ef4c9b87246.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/8bf604686f7ffcd131c7a44ea84b98356bc949dafd31330867272d402fdd89c4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/f1f47c59f5ffebb8938b01e1d3241fb7642e055194a74cefe6a721685a14c346.jpg)



Fig. 4. Fig. 4 shows the relationship between volatility and trading volume for each broker category. Volatility is calculated as the log of ratio of the high to the low price over each 30-minute trading interval. For each stock, trading intervals are then ranked into volatility deciles. Panels A-C present the results for HFT, Institutions, and Retail, respectively. For each broker category, we calculate the percentage of aggressive (blue circles) and passive (red triangles) trading volume, relative to total aggressive and passive trading volume, for each volatility decile.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/68e09d4fbfb6bcf7ed8e0651205cdc0a0e052c7408ec2b55968503423069a368.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/27e1016e-0aed-4a8f-aff9-f0fd082d36af/dbec6b1596f2225d002e9b2ec4282149a48e47064a12c4b527abd5b7fe832d34.jpg)



Fig. 5. Fig. 5 shows the relationship between volatility and adjusted depth imbalance for each broker category. Volatility is calculated as the log of ratio of the high to the low price over each 30-minute trading interval. Trading intervals are then ranked into volatility deciles. For each broker category, we calculate the depth imbalance immediately before each aggressive (Panel A) or passive (Panel B) trade execution. Depth imbalance is calculated as the difference between the depths available at the five best bid and ask prices, scaled by total depth available at these price levels, immediately before each trade. We multiply depth imbalance by a buy or sell indicator so that buys and sells can be interpreted together. Depth imbalances are then averaged over each volatility decile by broker category.


## Table 1

Summary statistics 

Table 1, Panel A reports statistics for the 94 stocks that remain in the ASX 100 index for the period January 3, 2012 to June 30, 2012. Market capitalization is the stock’s market capitalization on January 3, 2012. Dollar volume is the average daily dollar volume in AUD. Number of trades is the average daily number of transactions. Price is the average trade price in AUD. Volatility is the difference between the log of the intraday high ask price and the log of the intraday low bid price. Spread is the time weighted average difference between the best bid and offer prices in AUD cents. The broker associated with each order book event is classified into three types: proprietary HFT (HFT), institutional (Institutions), or retail (Retail). Panel B reports the trading characteristics for each broker type. Panel C reports the average adjusted depth imbalance (Adjusted DI) for each trader type. For each order book event, Adjusted DI is calculated as: 

$$
A d j u s t e d D I _ {t} = q _ {t} \times \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}
$$

where $\Sigma _ { i = 1 } ^ { 5 } V o l B i d _ { i , t } ( \Sigma _ { i = 1 } ^ { 5 } V o l A s k _ { i , t } )$ is the volume available at the top 5 bid (ask) price levels immediately before the order book event, $t . \ q _ { t }$ is an indicator variable equal to 1 for buys and -1 for sells. 


Panel A: Stock characteristics


<table><tr><td></td><td>Mean</td><td>Std.dev.</td><td>Q1</td><td>Median</td><td>Q3</td></tr><tr><td>Market capitalization (bil.)</td><td>13.52</td><td>22.77</td><td>2.844</td><td>10.00</td><td>114.8</td></tr><tr><td>Dollar volume (mil.)</td><td>27.80</td><td>47.72</td><td>5.295</td><td>10.99</td><td>25.60</td></tr><tr><td>Ntrades</td><td>2,264</td><td>1,838</td><td>1,112</td><td>1,659</td><td>2,701</td></tr><tr><td>Price (dollars)</td><td>11.43</td><td>12.81</td><td>2.954</td><td>5.974</td><td>14.86</td></tr><tr><td>Volatility</td><td>2.105</td><td>1.188</td><td>1.360</td><td>1.861</td><td>2.541</td></tr><tr><td>Spread (cents)</td><td>1.021</td><td>0.376</td><td>0.926</td><td>0.998</td><td>1.115</td></tr><tr><td></td><td>All</td><td>HFT</td><td colspan="2">Institutions</td><td>Retail</td></tr></table>


Panel B: Trader characteristics


<table><tr><td>Average daily submissions</td><td>5,556</td><td>1,025</td><td>15,185</td><td>440</td></tr><tr><td>Average daily cancelations</td><td>1,837</td><td>478</td><td>4,921</td><td>57</td></tr><tr><td>Average daily executions (active)</td><td>600</td><td>260</td><td>1,446</td><td>92</td></tr><tr><td>Average daily executions (passive)</td><td>1,427</td><td>319</td><td>3,796</td><td>162</td></tr><tr><td>Median submission to cancel time</td><td>413</td><td>188</td><td>233</td><td>3,200</td></tr></table>


Panel C: Adjusted depth imbalance


<table><tr><td>Executions (active)</td><td>0.069</td><td>0.156</td><td>0.027</td><td>0.025</td></tr><tr><td>Executions (passive)</td><td>0.015</td><td>0.083</td><td>-0.029</td><td>-0.009</td></tr><tr><td>Submissions</td><td>0.034</td><td>0.063</td><td>-0.004</td><td>0.043</td></tr><tr><td>Amendments</td><td>0.019</td><td>0.040</td><td>-0.003</td><td>0.023</td></tr><tr><td>Cancelations</td><td>0.016</td><td>0.017</td><td>0.002</td><td>0.028</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 2

M<sub>ar</sub>k<sub>e</sub>t <sub>s</sub>h<sub>ares</sub> <sub>vo</sub>l<sub>ume</sub> <sub>an</sub>d d<sub>ep</sub>th i<sub>m</sub>b<sub>a</sub>l<sub>ances</sub> b<sub>y</sub> t<sub>ra</sub>d<sub>er</sub> t<sub>ype</sub> 

Table 2 reports the market share (Panel A) and volume imbalance (Panel B) for each depth imbalance (DI) decile by trader type For each stock we rank t<sub>ra</sub>d<sub>es</sub> f<sub>or eac</sub>h <sub>s</sub>t<sub>oc</sub>k i<sub>n</sub>t<sub>o</sub> DI d<sub>ec</sub>il<sub>es .</sub> F<sub>or every</sub> t<sub>ra</sub>d<sub>e</sub> DI i<sub>s ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub>d <sub>as :</sub> 

$$
D I _ {t} = \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}
$$

<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { i = 1 } ^ { n } V o l B i d _ { i , t } \left( \sum _ { i = 1 } ^ { n } V o l A s k _ { i , t } \right. } \end{array}$ )is the volume available at the top 5 bid (ask) price levels immediately a trade t<sub>.</sub> Panel A reports the average total volume <sub>an</sub>d f<sub>or eac</sub>h t<sub>ra</sub>d<sub>er</sub> t<sub>ype</sub> th<sub>e aggress</sub>i<sub>ve mar</sub>k<sub>e</sub>t <sub>s</sub>h<sub>are percen</sub>t<sub>age across</sub> th<sub>e</sub> DI d<sub>ec</sub>il<sub>es .</sub> I<sub>n</sub> P<sub>ane</sub>l B f<sub>or eac</sub>h DI d<sub>ec</sub>il<sub>e we ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance as</sub> 

$$
V o l u m e i m b a l a n c e _ {j} ^ {T} = \frac {\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} - \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}{\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} + \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}
$$


<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { k = 1 } ^ { n } B u y V o l u m e _ { k , j } ^ { T } ( \sum _ { k = 1 } ^ { n } B u y V o l u m e _ { k , j } ^ { T } ) } \end{array}$ is the total aggressive buying (selling) volume for depth imbalance decile j We also use a t-test to test for th<sub>e</sub> diff<sub>erences</sub> i<sub>n</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance means</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> t<sub>ra</sub>d<sub>er</sub> t<sub>ypes .</sub> <sup>* * *</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>es a</sub> 1 % <sub>s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>.</sub>


<table><tr><td>Depth imbalance decile</td><td>Depth imbalance</td><td>Avg. total volume</td><td>HFT %</td><td>Institutions %</td><td>Retail %</td></tr><tr><td></td><td></td><td colspan="2">Panel A: Aggressive market share %</td><td></td><td></td></tr><tr><td>0 (most negative)</td><td>-0.367</td><td>349,745</td><td>14.62</td><td>77.62</td><td>7.76</td></tr><tr><td>1</td><td>-0.210</td><td>286,940</td><td>10.73</td><td>80.43</td><td>8.84</td></tr><tr><td>2</td><td>-0.132</td><td>279,059</td><td>9.27</td><td>81.37</td><td>9.36</td></tr><tr><td>3</td><td>-0.071</td><td>273,599</td><td>8.87</td><td>81.60</td><td>9.53</td></tr><tr><td>4</td><td>-0.017</td><td>268,912</td><td>8.52</td><td>81.81</td><td>9.66</td></tr><tr><td>5</td><td>0.035</td><td>270,881</td><td>8.38</td><td>81.81</td><td>9.81</td></tr><tr><td>6</td><td>0.090</td><td>278,228</td><td>8.68</td><td>81.63</td><td>9.70</td></tr><tr><td>7</td><td>0.150</td><td>277,294</td><td>9.30</td><td>81.14</td><td>9.56</td></tr><tr><td>8</td><td>0.228</td><td>296,959</td><td>10.68</td><td>80.49</td><td>8.83</td></tr><tr><td>9 (most positive)</td><td>0.382</td><td>346,089</td><td>14.67</td><td>77.77</td><td>7.57</td></tr></table>

<table><tr><td>Depth imbalance decile</td><td>HFT</td><td>Institutions</td><td>Retail</td><td colspan="2">HFT vs. Institutions</td><td colspan="2">HFT vs. Retail</td><td colspan="2">Institutions vs. Retail</td></tr><tr><td colspan="10">Panel B: Volume imbalance %</td></tr><tr><td>0 (most negative)</td><td>-61.4</td><td>-19.7</td><td>-5.8</td><td>-41.7</td><td>***</td><td>-55.6</td><td>***</td><td>-13.9</td><td>***</td></tr><tr><td>1</td><td>-47.3</td><td>-15.5</td><td>-8.3</td><td>-31.9</td><td>***</td><td>-39.1</td><td>***</td><td>-7.2</td><td>***</td></tr><tr><td>2</td><td>-35.0</td><td>-10.2</td><td>-6.6</td><td>-24.7</td><td>***</td><td>-28.4</td><td>***</td><td>-3.7</td><td>***</td></tr><tr><td>3</td><td>-21.9</td><td>-5.8</td><td>-4.8</td><td>-16.1</td><td>***</td><td>-17.1</td><td>***</td><td>-1.0</td><td></td></tr><tr><td>4</td><td>-7.4</td><td>-1.7</td><td>-2.3</td><td>-5.7</td><td>***</td><td>-5.1</td><td>***</td><td>0.6</td><td></td></tr><tr><td>5</td><td>6.1</td><td>2.6</td><td>-1.0</td><td>3.4</td><td>***</td><td>7.0</td><td>***</td><td>3.6</td><td>***</td></tr><tr><td>6</td><td>21.0</td><td>6.2</td><td>0.8</td><td>14.8</td><td>***</td><td>20.2</td><td>***</td><td>5.4</td><td>***</td></tr><tr><td>7</td><td>34.2</td><td>10.1</td><td>3.6</td><td>24.1</td><td>***</td><td>30.6</td><td>***</td><td>6.5</td><td>***</td></tr><tr><td>8</td><td>46.9</td><td>15.8</td><td>3.9</td><td>31.1</td><td>***</td><td>43.0</td><td>***</td><td>12.0</td><td>***</td></tr><tr><td>9 (most positive)</td><td>61.7</td><td>19.3</td><td>7.0</td><td>42.4</td><td>***</td><td>54.7</td><td>***</td><td>12.3</td><td>***</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 3

R<sub>e</sub>l<sub>a</sub>ti<sub>on</sub> b<sub>e</sub>t<sub>ween</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance an</sub>d D<sub>ep</sub>th i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> 

T<sub>a</sub>bl<sub>e</sub> 3 <sub>repor</sub>t<sub>s</sub> th<sub>e</sub> <sub>regress</sub>i<sub>on</sub> <sub>o</sub>f V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> <sub>or</sub> T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> <sub>aga</sub>i<sub>ns</sub>t D<sub>ep</sub>th i<sub>m</sub>b<sub>a</sub>l<sub>ance .</sub> T<sub>ra</sub>d<sub>es</sub> <sub>are</sub> <sub>sor</sub>t<sub>e</sub>d i<sub>n</sub>t<sub>o</sub> d<sub>ec</sub>il<sub>es</sub> b<sub>ase</sub>d <sub>on</sub> th<sub>e</sub> <sub>s</sub>i<sub>ze</sub> <sub>o</sub>f th<sub>e</sub> d<sub>ep</sub>th imbalance (DI) immediately before the trade <sub>.</sub> For each DI decile and trader type we calculate Volume imbalance as : 

$$
V o l u m e i m b a l a n c e _ {j} ^ {T} = \frac {\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} - \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}{\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} + \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}
$$

<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { k = 1 } ^ { n } B u y V o l u m e _ { k , j } ^ { T } ( \sum _ { k = 1 } ^ { n } B u y V o l u m e _ { k , j } ^ { T } ) \mathrm { i s } } \end{array}$ the total aggressive buying (selling) volume for depth imbalance decile j<sub>.</sub> For columns 1 -3 we estimate the f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near regress</sub>i<sub>on w</sub>hi<sub>c</sub>h i<sub>s</sub> b<sub>ase</sub>d <sub>on</sub> DI d<sub>ec</sub>il<sub>es :</sub> 

$$
V o l u m e i m b a l a n c e _ {j} ^ {T} = \beta_ {0} + \beta_ {1} I (H F T) ^ {T} \times D I _ {j} + \beta_ {2} I (I n s t i t u t i o n s) ^ {T} \times D I _ {j} + \beta_ {3} I (H F T) ^ {T} + \beta_ {4} I (I n s t i t u t i o n s) ^ {T} + \beta_ {5} D I _ {j} + \beta_ {6} V o l u m e _ {j} + \varepsilon_ {j} ^ {T}
$$


where ܫ ሺ ܨܪ ܶሻ <sup>்</sup> ሺܫ ሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ <sup>்</sup> ) is 1 if trader t<sub>yp</sub>e<sub>,</sub> T<sub>,</sub> is HFT (Institutions) and 0 otherwise <sub>.</sub> DI is the avera<sub>g</sub>e de<sub>p</sub>th imbalance for the decile and Volume is th<sub>e na</sub>t<sub>ura</sub>l l<sub>og o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l <sub>s</sub>h<sub>are vo</sub>l<sub>ume</sub> t<sub>ra</sub>d<sub>e</sub>d i<sub>n</sub> th<sub>e</sub> d<sub>ec</sub>il<sub>e .</sub> I<sub>n</sub> C<sub>o</sub>l<sub>umns</sub> 4-6 <sub>we rep</sub>l<sub>ace</sub> th<sub>e</sub> d<sub>epen</sub>d<sub>en</sub>t <sub>var</sub>i<sub>a</sub>bl<sub>e w</sub>ith T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance w</sub>hi<sub>c</sub>h i<sub>s ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub>d b<sub>ase</sub>d on the number rather than the volume of aggressive executions For each stock low (high) volatility days represent the lowest (highest) tercile of trading days b<sub>ase</sub>d <sub>on s</sub>t<sub>oc</sub>k <sub>vo</sub>l<sub>a</sub>tilit<sub>y w</sub>h<sub>ere vo</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> hi<sub>g</sub>h <sub>as</sub>k <sub>pr</sub>i<sub>ce an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> l<sub>ow</sub> bid <sub>pr</sub>i<sub>ce</sub> All <sub>regress</sub>i<sub>ons</sub> <sub>con</sub>t<sub>ro</sub>l f<sub>or</sub> <sub>s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s .</sub> H<sub>e</sub>t<sub>erosce</sub>d<sub>as</sub>ti<sub>c</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors</sub> <sub>are</sub> d<sub>ou</sub>bl<sub>e</sub> <sub>c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y</sub> <sub>s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> <sub>an</sub>d t-<sub>s</sub>t<sub>a</sub>ti<sub>s</sub>ti<sub>cs</sub> <sub>are</sub> <sub>repor</sub>t<sub>e</sub>d i<sub>n</sub> <sub>paren</sub>th<sub>eses .</sub> <sup>* * *</sup> <sub>,</sub> <sup>* *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e</sub> <sub>s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s</sub> <sub>o</sub>f 1 % <sub>,</sub> 5 % <sub>an</sub>d 1 0%<sub>,</sub> <sub>respec</sub>ti<sub>ve</sub>l<sub>y.</sub>


<table><tr><td></td><td colspan="3">Buy volume imbalance%</td><td colspan="3">Buy trade imbalance%</td></tr><tr><td></td><td>(1)All days</td><td>(2)Low volatilitydays</td><td>(3)High volatilitydays</td><td>(4)All days</td><td>(5)Low volatilitydays</td><td>(6)High volatilitydays</td></tr><tr><td>I(HFT) × DI</td><td>1.046***(25.95)</td><td>1.002***(19.73)</td><td>1.117***(28.90)</td><td>1.004***(24.58)</td><td>0.997***(18.78)</td><td>1.036***(26.18)</td></tr><tr><td>I(Institutions) × DI</td><td>0.025(0.91)</td><td>-0.008(-0.20)</td><td>0.040(1.33)</td><td>0.093***(3.37)</td><td>0.049(1.15)</td><td>0.129***(4.79)</td></tr><tr><td>I(HFT)</td><td>0.011(0.79)</td><td>0.025(1.24)</td><td>0.007(0.49)</td><td>0.022(1.52)</td><td>0.041**(2.17)</td><td>0.011(0.78)</td></tr><tr><td>I(Institutions)</td><td>0.016(1.26)</td><td>0.032*(1.81)</td><td>0.012(0.82)</td><td>0.037**(2.43)</td><td>0.053***(2.72)</td><td>0.025*(1.66)</td></tr><tr><td>DI</td><td>-0.175***(-5.22)</td><td>-0.116***(-2.65)</td><td>-0.227***(-5.81)</td><td>-0.100***(-4.10)</td><td>-0.077**(-1.99)</td><td>-0.124***(-4.77)</td></tr><tr><td>Volume</td><td>0.008**(2.37)</td><td>0.002(0.40)</td><td>0.006(1.30)</td><td>0.011***(3.44)</td><td>0.008*(1.66)</td><td>0.011*(1.89)</td></tr><tr><td>Constant</td><td>-0.241***(-6.45)</td><td>-0.160***(-2.76)</td><td>-0.220***(-4.23)</td><td>-0.303***(-7.29)</td><td>-0.404***(-6.17)</td><td>-0.231***(-3.48)</td></tr><tr><td>Obs.</td><td>245,382</td><td>64,203</td><td>93,143</td><td>245,382</td><td>64,203</td><td>93,143</td></tr><tr><td>Adj. R-square</td><td>0.186</td><td>0.186</td><td>0.201</td><td>0.275</td><td>0.274</td><td>0.302</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 4

Li<sub>m</sub>it <sub>or</sub>d<sub>er</sub> <sub>p</sub>l<sub>acemen</sub>t <sub>s</sub>t<sub>ra</sub>t<sub>eg</sub>i<sub>es</sub> 

Table 4 compares the Adjusted DI immediately before order book events for HFT Institutions and Retail The dependent variable is Adjusted DI which is the daily average Adjusted DI for each order book event and trader type : 

$$
A d j u s t e d D I _ {t} = q _ {t} \times \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}
$$

<sub>w</sub>h<sub>ere</sub> $\textstyle \sum _ { i = 1 } ^ { 5 } V o l B i d _ { i , t } \ : ( \sum _ { i = 1 } ^ { 5 } V o l A s k _ { i , t } )$ is the volume available at the top n bid (ask) price levels immediately before the order book event t q is an indicator <sub>var</sub>i<sub>a</sub>bl<sub>e equa</sub>l t<sub>o</sub> 1 f<sub>or</sub> b<sub>uys an</sub>d - 1 f<sub>or se</sub>ll<sub>s</sub> W<sub>e presen</sub>t th<sub>e coe</sub>ffi<sub>c</sub>i<sub>en</sub>t <sub>es</sub>ti<sub>ma</sub>t<sub>es</sub> f<sub>or</sub> th<sub>e</sub> f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near regress</sub>i<sub>on:</sub> 

$$
\begin{array}{r l} {A d j u s t e d D I _ {E} ^ {T} =} & {\beta_ {0} ^ {T} + \beta_ {1} ^ {T} I (A g g r e s s i v e e x e c u t i o n) _ {E} ^ {T} + \beta_ {2} ^ {T} I (P a s s i v e e x e c u t i o n) _ {E} ^ {T} + \beta_ {3} ^ {T} I (A m e n d) _ {E} ^ {T} + \beta_ {4} ^ {T} I (C a n c e l) _ {E} ^ {T} + \beta_ {5} ^ {T} V o l a t i l i t y + \beta_ {6} ^ {T} V o l u m e} \\ & {+ \beta_ {7} ^ {T} P r i c e + \beta_ {8} ^ {T} S p r e a d + \varepsilon_ {E} ^ {T}} \end{array}
$$

where ܫ ሺ∙ሻ is an indicator variable e<sub>q</sub>ual to 1 for the order book event s<sub>p</sub>ecified in the <sub>p</sub>arentheses and 0 otherwise All control variables are measured on a dail<sub>y</sub> b<sub>as</sub>i<sub>s .</sub> V<sub>o</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> hi<sub>g</sub>h <sub>as</sub>k <sub>pr</sub>i<sub>ce an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> l<sub>ow</sub> bid <sub>pr</sub>i<sub>ce .</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>s</sub> th<sub>e na</sub>t<sub>ura</sub>l l<sub>og o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l d<sub>a</sub>il<sub>y s</sub>h<sub>are vo</sub>l<sub>ume .</sub> P<sub>r</sub>i<sub>ce</sub> i<sub>s</sub> th<sub>e average</sub> d<sub>a</sub>il<sub>y</sub> t<sub>ra</sub>d<sub>e pr</sub>i<sub>ce .</sub> S<sub>prea</sub>d i<sub>s</sub> th<sub>e</sub> ti<sub>me we</sub>i<sub>g</sub>ht<sub>e</sub>d <sub>average</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> b<sub>es</sub>t bid <sub>an</sub>d <sub>o</sub>ff<sub>er pr</sub>i<sub>ces .</sub> All <sub>regress</sub>i<sub>ons</sub> <sub>con</sub>t<sub>ro</sub>l f<sub>or s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s</sub> H<sub>e</sub>t<sub>erosce</sub>d<sub>as</sub>ti<sub>c</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors are</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay an</sub>d t-<sub>s</sub>t<sub>a</sub>ti<sub>s</sub>ti<sub>cs are repor</sub>t<sub>e</sub>d i<sub>n paren</sub>th<sub>eses</sub> <sup>* * *</sup> <sub>,</sub> <sup>* *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e</sub> <sub>s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s</sub> <sub>o</sub>f 1 % <sub>,</sub> 5 % <sub>an</sub>d 1 0%<sub>,</sub> <sub>respec</sub>ti<sub>ve</sub>l<sub>y.</sub> 

<table><tr><td rowspan="2"></td><td colspan="3">Depth imbalance (5 levels)</td><td colspan="3">Depth imbalance (1 level)</td></tr><tr><td>(1)HFT</td><td>(2)Institutions</td><td>(3)Retail</td><td>(4)HFT</td><td>(5)Institutions</td><td>(6)Retail</td></tr><tr><td>I(Aggressive execution)</td><td>0.091***(21.98)</td><td>0.031***(13.72)</td><td>-0.017***(-8.36)</td><td>0.347***(21.74)</td><td>0.210***(31.55)</td><td>0.042***(8.54)</td></tr><tr><td>I(Passive execution)</td><td>0.020***(8.44)</td><td>-0.025***(-14.39)</td><td>-0.051***(-24.56)</td><td>0.008(1.04)</td><td>-0.093***(-32.04)</td><td>-0.087***(-34.08)</td></tr><tr><td>I(Amend)</td><td>-0.018***(-3.42)</td><td>0.001(1.54)</td><td>-0.018***(-7.85)</td><td>-0.036***(-2.96)</td><td>-0.058***(-40.61)</td><td>-0.032***(-7.45)</td></tr><tr><td>I(Cancel)</td><td>-0.046***(-10.16)</td><td>0.007***(7.78)</td><td>-0.014***(-5.57)</td><td>-0.273***(-10.78)</td><td>-0.026***(-9.57)</td><td>-0.031***(-8.75)</td></tr><tr><td>Volatility</td><td>0.252**(2.58)</td><td>0.171***(3.73)</td><td>0.025(0.34)</td><td>0.090(0.94)</td><td>0.049(0.91)</td><td>-0.014(-0.15)</td></tr><tr><td>Volume</td><td>0.003(1.49)</td><td>0.005***(4.94)</td><td>0.002(0.88)</td><td>-0.002(-0.46)</td><td>0.002**(1.99)</td><td>0.003(1.26)</td></tr><tr><td>Price</td><td>-0.022*(-1.86)</td><td>-0.006***(-3.25)</td><td>0.010(0.89)</td><td>0.007(0.46)</td><td>-0.011**(-2.08)</td><td>0.003(0.35)</td></tr><tr><td>Spread</td><td>5.158***(9.59)</td><td>0.456*(1.81)</td><td>-0.214(-0.21)</td><td>-0.232(-0.26)</td><td>-0.825*(-1.76)</td><td>-0.651(-0.98)</td></tr><tr><td>Constant</td><td>-0.040(-1.21)</td><td>-0.088***(-5.09)</td><td>0.007(0.22)</td><td>0.079*(1.73)</td><td>-0.022(-1.08)</td><td>0.005(0.14)</td></tr><tr><td>Obs.</td><td>53,858</td><td>55,320</td><td>54,688</td><td>53,858</td><td>55,320</td><td>54,688</td></tr><tr><td>Adj. R-square</td><td>0.332</td><td>0.147</td><td>0.045</td><td>0.543</td><td>0.696</td><td>0.081</td></tr></table>

## Table 5

Multinomial logistic regressions for limit order placement strategies 

Table 5 assesses the probability of each order book event based on prevailing market conditions. We present the coefficient estimates for the following multinomial logistic regression: 

$$
O r d e r B o o k E v e n t _ {E} ^ {T} = \beta_ {0} ^ {T} + \beta_ {1} ^ {T} A d j u s t e d D I _ {E} ^ {T} + \beta_ {2} ^ {T} V o l a t i l i t y + \beta_ {3} ^ {T} V o l u m e + \beta_ {4} ^ {T} P r i c e + \beta_ {5} ^ {T} S p r e a d + \varepsilon_ {E} ^ {T}
$$

<sub>ா</sub>ݐ݁݊ݒܧ݇݋݋ܤݎ݀݁ݎܱ where <sup>்</sup> is the dependent variable indicating one of five order book events, E,: Aggressive execution, passive execution, limit order submission, amendment or cancelation. We estimate the model with limit order submission as the baseline category. Volatility is the difference between the log of the intraday high ask price and the log of the intraday low bid price. Volume is the natural log of the total daily share volume. Price is the average daily trade price. Spread is the time weighted average difference between the best bid and offer prices. All regressions control for stock and day fixed effects. The main independent variable is Adjusted DI, which is the daily average Adjusted DI for each order book event and trader type: 

$$
A d j u s t e d D I _ {t} = q _ {t} \times \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}
$$

where $\begin{array} { r } { \sum _ { i = 1 } ^ { 5 } V o l B i d _ { i , t } \ : ( \sum _ { i = 1 } ^ { 5 } V o l A s k _ { i , t } ) } \end{array}$ is the volume available at the top n bid (ask) price levels immediately before the order book event, t. q is an indicator variable equal to 1 for buys and -1 for sells. Panels A to C present the results for HFT, Institutions and Retail, respectively. Robust standard errors are clustered by stock and t-statistics are reported in parentheses. ***, ** and * indicate significance levels of 1%, 5% and 10%, respectively. 

<table><tr><td></td><td>Aggressive executions</td><td>Passive executions</td><td>Amendment</td><td>Cancellation</td></tr><tr><td></td><td colspan="4">Panel A: HFT</td></tr><tr><td>Adjusted DI</td><td>10.498***(9.95)</td><td>2.574***(7.36)</td><td>-2.375***(-4.06)</td><td>-5.097***(-11.74)</td></tr><tr><td>Volatility</td><td>-0.472(-0.40)</td><td>-0.487*(-1.88)</td><td>1.110**(2.44)</td><td>2.232***(3.65)</td></tr><tr><td>Volume</td><td>0.005(0.17)</td><td>-0.004(-0.59)</td><td>0.031***(2.97)</td><td>0.051***(4.86)</td></tr><tr><td>Price</td><td>0.282*(1.78)</td><td>0.070**(2.05)</td><td>-0.046(-1.47)</td><td>-0.089***(-2.70)</td></tr><tr><td>Spread</td><td>-60.417***(-6.57)</td><td>-12.732***(-6.10)</td><td>15.991***(3.20)</td><td>22.956***(6.27)</td></tr><tr><td>Constant</td><td>-1.023**(-2.35)</td><td>0.018(0.18)</td><td>-0.634***(-4.23)</td><td>-1.019***(-6.49)</td></tr><tr><td>Obs.</td><td></td><td colspan="3">53,858</td></tr><tr><td>Pseudo R-square</td><td></td><td colspan="3">0.0673</td></tr></table>


Panel B: Institutions


<table><tr><td></td><td>Aggressive executions</td><td>Passive executions</td><td>Amendment</td><td>Cancellation</td></tr><tr><td>Adjusted DI</td><td>15.240***(8.21)</td><td>-11.297***(-7.74)</td><td>0.446(1.51)</td><td>3.572***(6.26)</td></tr><tr><td>Volatility</td><td>-1.024*(-1.69)</td><td>2.974***(4.45)</td><td>-0.078(-1.43)</td><td>-0.550***(-3.50)</td></tr><tr><td>Volume</td><td>-0.072***(-3.79)</td><td>0.067***(4.02)</td><td>-0.002(-1.49)</td><td>-0.018***(-3.67)</td></tr><tr><td>Price</td><td>0.114***(3.39)</td><td>-0.060**(-2.00)</td><td>0.003(1.43)</td><td>0.024***(3.00)</td></tr><tr><td>Spread</td><td>-15.403***(-3.09)</td><td>-1.647(-0.49)</td><td>-0.185(-1.10)</td><td>-1.984*(-1.84)</td></tr><tr><td>Constant</td><td>0.817***(3.13)</td><td>-1.319***(-4.82)</td><td>0.035(1.51)</td><td>0.256***(3.65)</td></tr><tr><td>Obs.</td><td></td><td colspan="3">55,320</td></tr><tr><td>Pseudo R-square</td><td></td><td colspan="3">0.0416</td></tr></table>

<table><tr><td rowspan="2"></td><td colspan="4">Panel C: Retail</td></tr><tr><td>Aggressive executions</td><td>Passive executions</td><td>Amendment</td><td>Cancellation</td></tr><tr><td>Adjusted DI</td><td>-1.459***(-7.52)</td><td>-4.565***(-14.41)</td><td>-1.579***(-5.95)</td><td>-1.202***(-4.89)</td></tr><tr><td>Volatility</td><td>-0.102(-0.86)</td><td>0.286(0.89)</td><td>0.269(1.07)</td><td>0.182(1.09)</td></tr><tr><td>Volume</td><td>0.004(1.07)</td><td>0.010(1.09)</td><td>0.034***(4.45)</td><td>0.009**(2.19)</td></tr><tr><td>Price</td><td>0.015(0.87)</td><td>0.044(0.87)</td><td>-0.041*(-1.66)</td><td>-0.023*(-1.69)</td></tr><tr><td>Spread</td><td>0.322(0.18)</td><td>-1.719(-0.41)</td><td>0.573(0.33)</td><td>1.385(0.78)</td></tr><tr><td>Constant</td><td>-0.025(-0.42)</td><td>-0.118(-0.84)</td><td>-0.532***(-4.48)</td><td>-0.146**(-2.03)</td></tr><tr><td>Obs.</td><td></td><td></td><td>54,688</td><td></td></tr><tr><td>Pseudo R-square</td><td></td><td></td><td>0.0077</td><td></td></tr></table>

## Table 6

Relation between Aggressive volume % and stock volatility 

Table 6 presents the regression of Aggressive volume % against volatility. The dependent variable is %	݉݁ݑ݈݋ݒ	݁ݒ݅ݏݏ݁ݎ݃݃ܣ <sup>்</sup>, which is the aggressive buying and selling volume of trader type, T, as a percentage of their total aggressive and passive volume executed in a 30 minute time interval, I. The results are based on the following linear regression: 

$$
A g g r e s s i v e v o l u m e \% _ {I} ^ {T} = \beta_ {0} + \beta_ {1} V o l a t i l i t y _ {I} + \beta_ {1 0} V o l u m e _ {I} + \varepsilon
$$

Volatility is the difference between the log of the highest best ask price and the log of the lowest best bid price during the 30 minute interval. Volume is the natural log of the total daily share volume during the 30 minute interval. Large stocks (Small stocks) refer to stocks contained in the largest (smallest) tercile of all sample stocks based on market capitalization. All regressions control for stock and day fixed effects. Panels A to C present the results for HFT, Institutions and Retail, respectively. Heteroscedastic-robust standard errors are double clustered by stock and day and t-statistics are reported in parentheses. ***, ** and * indicate significance levels of 1%, 5% and 10%, respectively. 

<table><tr><td></td><td>(1)All stocks</td><td>(2)Large stocks</td><td>(3)Small stocks</td></tr><tr><td colspan="4">Panel A: HFT</td></tr><tr><td>Volatility</td><td>447.573***(20.35)</td><td>211.525***(5.06)</td><td>453.829***(11.25)</td></tr><tr><td>Volume</td><td>0.504***(3.53)</td><td>0.368*(1.69)</td><td>1.698***(5.09)</td></tr><tr><td>Constant</td><td>40.377***(18.36)</td><td>42.203***(13.81)</td><td>23.657***(5.13)</td></tr><tr><td>Obs.</td><td>58,789</td><td>28,891</td><td>10,750</td></tr><tr><td>Adj. R-square</td><td>0.304</td><td>0.272</td><td>0.332</td></tr><tr><td colspan="4">Panel B: Institutions</td></tr><tr><td>Volatility</td><td>-84.866***(-15.77)</td><td>-10.890(-1.21)</td><td>-91.190***(-8.75)</td></tr><tr><td>Volume</td><td>-0.033(-1.23)</td><td>0.157***(4.17)</td><td>-0.409***(-7.06)</td></tr><tr><td>Constant</td><td>49.163***(119.37)</td><td>48.914***(84.32)</td><td>52.524***(62.17)</td></tr><tr><td>Obs.</td><td>95,102</td><td>34,025</td><td>28,243</td></tr><tr><td>Adj. R-square</td><td>0.118</td><td>0.143</td><td>0.122</td></tr><tr><td colspan="4">Panel C: Retail</td></tr><tr><td>Volatility</td><td>-174.323***(-7.14)</td><td>-663.288***(-13.31)</td><td>7.451(0.19)</td></tr><tr><td>Volume</td><td>-0.220(-1.43)</td><td>-0.916***(-3.62)</td><td>0.642**(2.20)</td></tr><tr><td>Constant</td><td>67.915***(27.96)</td><td>67.170***(18.38)</td><td>61.621***(14.20)</td></tr><tr><td>Obs.</td><td>61,640</td><td>27,154</td><td>14,913</td></tr><tr><td>Adj. R-square</td><td>0.053</td><td>0.074</td><td>0.065</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 7

Relation between Adjusted DI and stock volatility 

Table 7 presents the regression ofAdjusted DI against volatility<sub>.</sub> The dependent variable is ܣ ݆݀ ݐݏݑ ݁݀ $D I _ { I } ^ { T }$ which is the average Adjusted DI for aggressive or passive executions for each trader type T over a 3 0 minute interval I For each trade Adjusted DI is calculated as : 

$$
A d j u s t e d D I _ {t} = q _ {t} \times \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i , t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i , t}}
$$

<sub>w</sub>h<sub>ere</sub> $\textstyle \sum _ { i = 1 } ^ { 5 } V o l B i d _ { i , t } \ : ( \sum _ { i = 1 } ^ { 5 } V o l A s k _ { i , t } )$ is the volume available at the top 5 bid (ask) price levels immediately before the trade t The results are based on the f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near</sub> <sub>regress</sub>i<sub>on:</sub> 

$$
\begin{array}{r} A d j u s t e d D I _ {I} ^ {T} = \beta_ {0} + \beta_ {1} I (H F T) ^ {T} \times V o l a t i l i t y _ {I} + \beta_ {2} I (I n s t i t u t i o n s) ^ {T} \times V o l a t i l i t y _ {I} + \beta_ {3} I (H F T) ^ {T} + \beta_ {4} I (I n s t i t u t i o n s) ^ {T} + \beta_ {5} V o l a t i l i t y _ {I} \\ + \beta_ {6} V o l u m e _ {I} + \varepsilon \end{array}
$$

ܫ ሺ ܨܪ ܶሻ <sup>்</sup> ሺܫ ሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ <sup>்</sup>) is 1 if trader t<sub>yp</sub>e T is HFT (Institutions) and 0 otherwise Volatilit<sub>y</sub> is the difference between the lo<sub>g</sub> of the hi<sub>g</sub>hest best ask <sub>p</sub>rice <sub>an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> l<sub>owes</sub>t b<sub>es</sub>t bid <sub>pr</sub>i<sub>ce</sub> d<sub>ur</sub>i<sub>ng</sub> th<sub>e</sub> 3 0 <sub>m</sub>i<sub>nu</sub>t<sub>e</sub> i<sub>n</sub>t<sub>erva</sub>l V<sub>o</sub>l<sub>ume</sub> i<sub>s</sub> th<sub>e na</sub>t<sub>ura</sub>l l<sub>og o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l d<sub>a</sub>il<sub>y s</sub>h<sub>are vo</sub>l<sub>ume</sub> d<sub>ur</sub>i<sub>ng</sub> th<sub>e</sub> 3 0 <sub>m</sub>i<sub>nu</sub>t<sub>e</sub> i<sub>n</sub>t<sub>erva</sub>l Large stocks (Small stocks) refer to stocks contained in the largest (smallest) tercile of all sample stocks based on market capitalization All regressions control f<sub>or s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s .</sub> H<sub>e</sub>t<sub>erosce</sub>d<sub>as</sub>ti<sub>c</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors are</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay an</sub>d t-<sub>s</sub>t<sub>a</sub>ti<sub>s</sub>ti<sub>cs are repor</sub>t<sub>e</sub>d i<sub>n paren</sub>th<sub>eses .</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y</sub> 

<table><tr><td rowspan="2"></td><td colspan="3">Aggressive executions</td><td colspan="3">Passive executions</td></tr><tr><td>(1) All stocks</td><td>(2) Large stocks</td><td>(3) Small stocks</td><td>(4) All stocks</td><td>(5) Large stocks</td><td>(6) Small stocks</td></tr><tr><td rowspan="2">I(HFT) × Volatility</td><td>3.940***</td><td>5.012***</td><td>1.088</td><td>5.224***</td><td>5.473***</td><td>2.634*</td></tr><tr><td>(5.51)</td><td>(3.74)</td><td>(1.10)</td><td>(5.75)</td><td>(3.19)</td><td>(1.96)</td></tr><tr><td rowspan="2">I(Institutions) × Volatility</td><td>0.323</td><td>0.569</td><td>0.313</td><td>1.621***</td><td>2.361***</td><td>1.102***</td></tr><tr><td>(1.09)</td><td>(1.21)</td><td>(0.89)</td><td>(5.75)</td><td>(3.85)</td><td>(2.76)</td></tr><tr><td rowspan="2">I(HFT)</td><td>0.100***</td><td>0.080***</td><td>0.140***</td><td>0.068***</td><td>0.053***</td><td>0.103***</td></tr><tr><td>(15.63)</td><td>(11.92)</td><td>(9.43)</td><td>(6.95)</td><td>(5.10)</td><td>(3.95)</td></tr><tr><td rowspan="2">I(Institutions)</td><td>0.002</td><td>0.009**</td><td>-0.006</td><td>-0.036***</td><td>-0.040***</td><td>-0.030***</td></tr><tr><td>(0.55)</td><td>(2.25)</td><td>(-1.04)</td><td>(-11.23)</td><td>(-9.63)</td><td>(-6.70)</td></tr><tr><td rowspan="2">Volatility</td><td>1.753***</td><td>0.991**</td><td>2.440***</td><td>-2.521***</td><td>-3.134***</td><td>-1.526***</td></tr><tr><td>(6.22)</td><td>(1.98)</td><td>(6.64)</td><td>(-8.22)</td><td>(-4.32)</td><td>(-3.91)</td></tr><tr><td rowspan="2">Volume</td><td>-0.003***</td><td>-0.002**</td><td>-0.004**</td><td>-0.001*</td><td>-0.000</td><td>-0.003*</td></tr><tr><td>(-3.46)</td><td>(-2.04)</td><td>(-2.43)</td><td>(-1.90)</td><td>(-0.04)</td><td>(-1.79)</td></tr><tr><td rowspan="2">Constant</td><td>0.036***</td><td>0.034***</td><td>0.041**</td><td>0.017**</td><td>0.011</td><td>0.016</td></tr><tr><td>(4.58)</td><td>(2.96)</td><td>(2.56)</td><td>(2.31)</td><td>(0.69)</td><td>(0.97)</td></tr><tr><td>Obs.</td><td>253146</td><td>97567</td><td>80562</td><td>255094</td><td>99025</td><td>83576</td></tr><tr><td>Adj. R-square</td><td>0.178</td><td>0.207</td><td>0.173</td><td>0.157</td><td>0.197</td><td>0.138</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 8

R<sub>e</sub>l<sub>a</sub>ti<sub>on</sub> b<sub>e</sub>t<sub>ween</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance an</sub>d DI b<sub>e</sub>f<sub>ore an</sub>d <sub>a</sub>ft<sub>er</sub> th<sub>e</sub> i<sub>mp</sub>l<sub>emen</sub>t<sub>a</sub>ti<sub>on o</sub>f ITCH 

T<sub>a</sub>bl<sub>e</sub> 8 <sub>repor</sub>t<sub>s</sub> th<sub>e</sub> <sub>regress</sub>i<sub>on</sub> <sub>o</sub>f V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> <sub>or</sub> T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> <sub>aga</sub>i<sub>ns</sub>t DI<sub>.</sub> W<sub>e</sub> <sub>ana</sub>l<sub>yze</sub> t<sub>ra</sub>d<sub>e</sub> <sub>an</sub>d <sub>quo</sub>t<sub>e</sub> d<sub>a</sub>t<sub>a</sub> f<sub>or</sub> th<sub>e</sub> <sub>per</sub>i<sub>o</sub>d<sub>s</sub> M<sub>arc</sub>h 2 20 1 2 t<sub>o</sub> M<sub>arc</sub>h 3 0 20 1 2 (pre-ITCH) and April 9 20 1 2 to May 9 20 1 2 (post-ITCH) <sub>.</sub> For each stock trades are sorted into deciles based on the size of the depth imbalance (DI) i<sub>mme</sub>di<sub>a</sub>t<sub>e</sub>l<sub>y</sub> b<sub>e</sub>f<sub>ore</sub> th<sub>e</sub> t<sub>ra</sub>d<sub>e .</sub> F<sub>or eac</sub>h DI d<sub>ec</sub>il<sub>e an</sub>d t<sub>ra</sub>d<sub>er</sub> t<sub>ype we ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance as :</sub> 

$$
V o l u m e i m b a l a n c e _ {j} ^ {T} = \frac {\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} - \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}{\sum_ {k = 1} ^ {n} B u y V o l u m e _ {k , j} ^ {T} + \sum_ {k = 1} ^ {n} S e l l V o l u m e _ {k , j} ^ {T}}
$$

<sub>w</sub>h<sub>ere</sub> $\scriptstyle \sum _ { k = 1 } ^ { n }$ <sub>ݕ</sub>ݑܤ ܸ݋݈ݑ݉ $\scriptstyle { \sum _ { k , j } ^ { T } ( \sum _ { k = 1 } ^ { n } }$ ݕݑܤ<sub>ଵ</sub> $V o l u m e _ { k , j } ^ { T } )$ is the total aggressive buying (selling) volume for depth imbalance decile j<sub>.</sub> For columns 1 -3 we estimate th<sub>e</sub> f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near regress</sub>i<sub>on w</sub>hi<sub>c</sub>h i<sub>s</sub> b<sub>ase</sub>d <sub>on</sub> DI d<sub>ec</sub>il<sub>es :</sub> 

$$
\begin{array}{r l} & V o l u m e i m b a l a n c e _ {j} ^ {T} \\ & \quad = \beta_ {0} + I (P r e) [ \beta_ {1} I (H F T) ^ {T} \times D I _ {j} + \beta_ {2} I (I n s t o) ^ {T} \times D I _ {j} + \beta_ {3} D I _ {j} ] + I (P o s t) [ \beta_ {4} I (H F T) ^ {T} \times D I _ {j} + \beta_ {5} I (I n s t o) ^ {T} \times D I _ {j} + \beta_ {6} D I _ {j} ] \\ & \quad + \beta_ {7} I (H F T) ^ {T} + \beta_ {8} I (I n s t o) ^ {T} + \beta_ {9} V o l u m e _ {j} + \varepsilon_ {j} ^ {T} \end{array}
$$

I(Pre) (I(Post)) is an indicator variable e ual to 1 if the tradin da falls in the re-ITCH ( ost-ITCH) eriod and zero otherwise I(HFT) and I(Institutions) are i<sub>n</sub>di<sub>ca</sub>t<sub>or var</sub>i<sub>a</sub>bl<sub>es equa</sub>l t<sub>o</sub> 1 f<sub>or</sub> th<sub>e</sub> t<sub>ra</sub>d<sub>er</sub> t<sub>ype spec</sub>ifi<sub>e</sub>d i<sub>n</sub> th<sub>e paren</sub>th<sub>eses an</sub>d 0 <sub>o</sub>th<sub>erw</sub>i<sub>se .</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>s</sub> th<sub>e na</sub>t<sub>ura</sub>l l<sub>og o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l <sub>s</sub>h<sub>are vo</sub>l<sub>ume</sub> t<sub>ra</sub>d<sub>e</sub>d i<sub>n</sub> th<sub>e</sub> d<sub>ec</sub>il<sub>e</sub> F<sub>or ease o</sub>f <sub>compar</sub>i<sub>son</sub> C<sub>o</sub>l<sub>umn</sub> 1 <sub>repor</sub>t<sub>s</sub> th<sub>e coe</sub>ffi<sub>c</sub>i<sub>en</sub>t<sub>s assoc</sub>i<sub>a</sub>t<sub>e</sub>d <sub>var</sub>i<sub>a</sub>bl<sub>es</sub> i<sub>n</sub>t<sub>erac</sub>t<sub>e</sub>d <sub>w</sub>ith $I ( P r e ) ,$ C<sub>o</sub>l<sub>umn</sub> 2 <sub>resen</sub>t<sub>s</sub> th<sub>e coe</sub>ffi<sub>c</sub>i<sub>en</sub>t<sub>s</sub> f<sub>or</sub> th<sub>e con</sub>t<sub>ro</sub>l variables and Column 3 resents the coefficients associated variables interacted with I(Post) We use an F-test to test for the e ualit ofthe coefficients interacted <sub>w</sub>ith DI C<sub>o</sub>l<sub>umn</sub> 4 <sub>presen</sub>t<sub>s</sub> th<sub>e</sub> F-t<sub>es</sub>t <sub>an</sub>d th<sub>e assoc</sub>i<sub>a</sub>t<sub>e</sub>d <sub>p</sub>-<sub>va</sub>l<sub>ue</sub> i<sub>n paren</sub>th<sub>eses</sub> I<sub>n</sub> C<sub>o</sub>l<sub>umns</sub> 5 - 8 <sub>we rep</sub>l<sub>ace</sub> th<sub>e</sub> d<sub>epen</sub>d<sub>en</sub>t <sub>var</sub>i<sub>a</sub>bl<sub>e w</sub>ith T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance an</sub>d <sub>per</sub>f<sub>orm</sub> th<sub>e</sub> <sub>same</sub> <sub>ana</sub>l<sub>ys</sub>i<sub>s</sub> <sub>as</sub> th<sub>e</sub> <sub>prev</sub>i<sub>ous</sub> 4 <sub>co</sub>l<sub>umns .</sub> All <sub>regress</sub>i<sub>ons</sub> <sub>con</sub>t<sub>ro</sub>l f<sub>or</sub> <sub>s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s .</sub> H<sub>e</sub>t<sub>erosce</sub>d<sub>as</sub>ti<sub>c</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors</sub> <sub>are</sub> d<sub>ou</sub>bl<sub>e</sub> <sub>c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay an</sub>d t-<sub>s</sub>t<sub>a</sub>ti<sub>s</sub>ti<sub>cs are repor</sub>t<sub>e</sub>d i<sub>n paren</sub>th<sub>eses .</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5% <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y.</sub> 

<table><tr><td rowspan="3"></td><td colspan="2">(1)</td><td colspan="2">(2)</td><td colspan="2">(3)</td><td colspan="2">(4)</td><td colspan="2">(5)</td><td colspan="2">(6)</td><td colspan="2">(7)</td><td colspan="2">(8)</td></tr><tr><td colspan="6">Volume imbalance</td><td rowspan="2">F-Test</td><td colspan="7">Trade imbalance</td><td rowspan="2" colspan="2">F-Test</td></tr><tr><td colspan="3">Pre-ITCH</td><td colspan="3">Post-ITCH</td><td colspan="4">Pre-ITCH</td><td colspan="3">Post-ITCH</td></tr><tr><td>I(HFT) × DI</td><td><eq>\beta_1</eq></td><td>0.942***(18.43)</td><td></td><td><eq>\beta_4</eq></td><td>1.064***(18.79)</td><td></td><td>5.350**(0.023)</td><td><eq>\beta_1</eq></td><td>0.938***(17.24)</td><td></td><td></td><td><eq>\beta_4</eq></td><td>1.066***(22.25)</td><td></td><td>7.71***(0.007)</td><td></td></tr><tr><td>I(Institutional) × DI</td><td><eq>\beta_2</eq></td><td>-0.030(-0.79)</td><td></td><td><eq>\beta_5</eq></td><td>-0.038(-0.88)</td><td></td><td>0.040(0.850)</td><td><eq>\beta_2</eq></td><td>0.017(0.37)</td><td></td><td></td><td><eq>\beta_5</eq></td><td>0.128***(3.22)</td><td></td><td>5.27**(0.024)</td><td></td></tr><tr><td>Depth imbalance</td><td><eq>\beta_3</eq></td><td>-0.095**(-2.09)</td><td></td><td><eq>\beta_6</eq></td><td>-0.118**(-2.50)</td><td></td><td>0.480(0.490)</td><td><eq>\beta_3</eq></td><td>-0.028(-0.73)</td><td></td><td></td><td><eq>\beta_6</eq></td><td>-0.121***(-3.24)</td><td></td><td>6.36**(0.014)</td><td></td></tr><tr><td>I(HFT)</td><td></td><td></td><td><eq>\beta_7</eq></td><td>0.025(1.33)</td><td></td><td></td><td></td><td></td><td></td><td><eq>\beta_7</eq></td><td>0.026(1.49)</td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>I(Institutional)</td><td></td><td></td><td><eq>\beta_8</eq></td><td>0.033**(2.05)</td><td></td><td></td><td></td><td></td><td></td><td><eq>\beta_8</eq></td><td>0.040**(2.33)</td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>Volume</td><td></td><td></td><td><eq>\beta_9</eq></td><td>0.016***(3.36)</td><td></td><td></td><td></td><td></td><td></td><td><eq>\beta_9</eq></td><td>0.019***(3.44)</td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>Constant</td><td></td><td></td><td><eq>\beta_0</eq></td><td>-0.373***(-6.76)</td><td></td><td></td><td></td><td></td><td></td><td><eq>\beta_0</eq></td><td>-0.561***(-8.55)</td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>Obs.</td><td></td><td></td><td colspan="2">80,666</td><td></td><td></td><td></td><td></td><td></td><td></td><td colspan="2">80,666</td><td></td><td></td><td></td><td></td></tr><tr><td>Adj. R-square</td><td></td><td></td><td colspan="2">0.186</td><td></td><td></td><td></td><td></td><td></td><td></td><td colspan="2">0.278</td><td></td><td></td><td></td><td></td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 9

P<sub>ro</sub>b<sub>a</sub>bilit<sub>y</sub> <sub>o</sub>f li<sub>m</sub>it <sub>or</sub>d<sub>er</sub> <sub>execu</sub>ti<sub>ons</sub> b<sub>e</sub>f<sub>ore</sub> <sub>an</sub>d <sub>a</sub>ft<sub>er</sub> th<sub>e</sub> i<sub>mp</sub>l<sub>emen</sub>t<sub>a</sub>ti<sub>on</sub> <sub>o</sub>f ITCH 

T<sub>a</sub>bl<sub>e</sub> 9 <sub>ana</sub>l<sub>yzes</sub> th<sub>e</sub> <sub>pro</sub>b<sub>a</sub>bilit<sub>y</sub> <sub>o</sub>f li<sub>m</sub>it <sub>or</sub>d<sub>er</sub> <sub>execu</sub>ti<sub>ons</sub> f<sub>or</sub> HFT I<sub>ns</sub>tit<sub>u</sub>ti<sub>ons</sub> <sub>an</sub>d R<sub>e</sub>t<sub>a</sub>il b<sub>e</sub>f<sub>ore</sub> <sub>an</sub>d <sub>a</sub>ft<sub>er</sub> th<sub>e</sub> i<sub>mp</sub>l<sub>emen</sub>t<sub>a</sub>ti<sub>on</sub> <sub>o</sub>f ITCH<sub>.</sub> W<sub>e</sub> <sub>ana</sub>l<sub>yze</sub> t<sub>ra</sub>d<sub>e</sub> and quote data for the periods March 2 20 1 2 to March 3 0 20 1 2 (pre-ITCH) and April 9 20 1 2 to May 9 20 1 2 (post-ITCH) The main dependent variable $P ( F i l l ) ^ { T }$ i<sub>s ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub>d <sub>as :</sub> 

$$
P (F i l l) ^ {T} = \frac {\sum T r a d e V o l u m e ^ {T}}{\sum S u b m i t V o l u m e ^ {T}}
$$

where ∑ ܵݑܾ݉݅ݐܸ݋ ݈ݑ݉݁<sup>்</sup> is the total dail<sub>y</sub> volume submitted to the to<sub>p</sub> level ofthe limit order book and ∑ ܶݎܸܽ݀݁݋ ݈ݑ݉݁ <sup>்</sup> is the total volume that is successfull<sub>y</sub> t<sub>ra</sub>d<sub>e</sub>d f<sub>or</sub> t<sub>ra</sub>d<sub>er</sub> t<sub>ype</sub> T I<sub>n</sub> C<sub>o</sub>l<sub>umn</sub> 1 <sub>we es</sub>ti<sub>ma</sub>t<sub>e</sub> th<sub>e</sub> f<sub>o</sub>ll<sub>ow</sub>i<sub>ng regress</sub>i<sub>on:</sub> 

$$
P (F i l l) ^ {T} = \beta_ {0} + \beta_ {1} I (N o n - H F T) ^ {T} \times I (P o s t) + \beta_ {2} I (N o n - H F T) ^ {T} + \beta_ {3} I (P o s t) + \beta_ {4} V o l a t i l i t y + \beta_ {5} V o l u m e + \beta_ {6} P r i c e + \beta_ {7} S p r e a d + \varepsilon^ {T}
$$

<sub>w</sub>h<sub>ere</sub> $I ( N o n - H F T ) ^ { T }$ is an indicator variable equal to 1 for Institutions and Retail and zero for HFT I(Post) is an indicator variable equal to 1 if the trading d<sub>ay</sub> f<sub>a</sub>ll<sub>s</sub> i<sub>n</sub> th<sub>e pos</sub>t-ITCH <sub>per</sub>i<sub>o</sub>d <sub>an</sub>d <sub>zero</sub> f<sub>or</sub> th<sub>e pre</sub>-ITCH <sub>per</sub>i<sub>o</sub>d V<sub>o</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> hi<sub>g</sub>h <sub>as</sub>k <sub>pr</sub>i<sub>ce an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> l<sub>ow</sub> bid <sub>pr</sub>i<sub>ce .</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>s</sub> th<sub>e</sub> <sub>na</sub>t<sub>ura</sub>l l<sub>og</sub> <sub>o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l d<sub>a</sub>il<sub>y</sub> <sub>s</sub>h<sub>are</sub> <sub>vo</sub>l<sub>ume .</sub> P<sub>r</sub>i<sub>ce</sub> i<sub>s</sub> th<sub>e</sub> <sub>average</sub> d<sub>a</sub>il<sub>y</sub> t<sub>ra</sub>d<sub>e</sub> <sub>pr</sub>i<sub>ce .</sub> S<sub>prea</sub>d i<sub>s</sub> th<sub>e</sub> ti<sub>me</sub> <sub>we</sub>i<sub>g</sub>ht<sub>e</sub>d <sub>average</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> b<sub>es</sub>t bid <sub>an</sub>d <sub>o</sub>ff<sub>er r</sub>i<sub>ces</sub> I<sub>n</sub> C<sub>o</sub>l<sub>umn</sub> 2 <sub>we re</sub> l<sub>ace</sub> $I ( N o n - H F T ) ^ { T }$ with ܫ ሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ <sup>்</sup> and $I ( R e t a i l ) ^ { T }$ <sub>w</sub>hi<sub>c</sub>h <sub>are</sub> i<sub>n</sub>di<sub>ca</sub>t<sub>or var</sub>i<sub>a</sub>bl<sub>es</sub> equal to 1 for the trader type specified in the parentheses and zero otherwise <sub>.</sub> In Columns 3 and 4 (Columns 5 and 6) we replace the dependent variable with ܲ ሺܨܽ ݎ݋ݒ ܾܽ ݈݁ $f i l l ) ^ { T }$ (ܲ ሺܷ݂݊ܽ ݎ݋ݒ ܾ݈ܽ݁ $f i l l ) ^ { \bar { T } } )$ <sub>.</sub> We define a favorable (unfavorable) fill as an order execution when the limit order rests on the side of the order book with more (less) depth immediately prior to the trade <sub>.</sub> All regressions control for stock and day fixed effects <sub>.</sub> We report heteroskedastic-robust standard <sub>errors</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> i<sub>n paren</sub>th<sub>eses .</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5% <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y</sub> 

<table><tr><td rowspan="2"></td><td colspan="2">P(Fill)</td><td colspan="2">P(Favorable fill)</td><td colspan="2">P(Unfavorable fill)</td></tr><tr><td>(1)</td><td>(2)</td><td>(3)</td><td>(4)</td><td>(5)</td><td>(6)</td></tr><tr><td>I(Non-HFT) × I(Post)</td><td>-0.037***(-3.31)</td><td></td><td>-0.040***(-4.18)</td><td></td><td>-0.001(-0.13)</td><td></td></tr><tr><td>I(Non-HFT)</td><td>0.111***(5.95)</td><td></td><td>-0.030*(-1.80)</td><td></td><td>0.134***(22.11)</td><td></td></tr><tr><td>I(Institutions) × I(Post)</td><td></td><td>-0.021**(-2.04)</td><td></td><td>-0.029***(-3.03)</td><td></td><td>0.008(1.55)</td></tr><tr><td>I(Institutions)</td><td></td><td>-0.069***(-3.67)</td><td></td><td>-0.124***(-7.51)</td><td></td><td>0.053***(8.96)</td></tr><tr><td>I(Retail) × I(Post)</td><td></td><td>-0.058***(-3.77)</td><td></td><td>-0.051***(-4.23)</td><td></td><td>-0.009(-1.00)</td></tr><tr><td>I(Retail)</td><td></td><td>0.301***(15.87)</td><td></td><td>0.078***(4.52)</td><td></td><td>0.226***(29.49)</td></tr><tr><td>I(Post-ITCH)</td><td>0.006(0.39)</td><td>0.007(0.49)</td><td>0.036**(2.24)</td><td>0.036**(2.33)</td><td>0.006(0.57)</td><td>0.008(0.68)</td></tr><tr><td>Volatility</td><td>0.076(0.46)</td><td>0.062(0.36)</td><td>0.054(0.33)</td><td>-0.090(-0.56)</td><td>0.007(0.07)</td><td>-0.097(-1.04)</td></tr><tr><td>Volume</td><td>0.071***(17.62)</td><td>0.069***(17.64)</td><td>0.039***(11.72)</td><td>0.036***(10.89)</td><td>0.028***(10.88)</td><td>0.026***(10.02)</td></tr><tr><td>Price</td><td>0.030(0.77)</td><td>0.031(0.80)</td><td>0.015(0.81)</td><td>0.009(0.62)</td><td>-0.006(-0.78)</td><td>-0.014**(-2.01)</td></tr><tr><td>Spread</td><td>-1.334(-0.56)</td><td>-1.303(-0.55)</td><td>-0.089(-0.06)</td><td>-0.411(-0.32)</td><td>-0.199(-0.12)</td><td>-0.365(-0.23)</td></tr><tr><td>Constant</td><td>-0.559***(-6.85)</td><td>-0.529***(-6.61)</td><td>-0.291***(-4.81)</td><td>-0.231***(-3.85)</td><td>-0.249***(-5.73)</td><td>-0.205***(-4.67)</td></tr><tr><td>Obs.</td><td>10,646</td><td>10,646</td><td>9,718</td><td>9,718</td><td>9,574</td><td>9,574</td></tr><tr><td>Adj. R-square</td><td>0.188</td><td>0.586</td><td>0.151</td><td>0.369</td><td>0.224</td><td>0.460</td></tr></table>