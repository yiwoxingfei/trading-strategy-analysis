

<!-- === Source: MinerU_markdown_High-frequency_trading_strategies1_1_2122707067558010894.md (Page 1) === -->

# High-frequency trading strategies

Michael Goldstein Babson College Babson Park, MA 02457-0310, USA goldstein@babson.edu 

Amy Kwan University of Sydney Sydney, NSW 2006, Australia amy.kwan@sydney.edu.au 

Richard Philip University of Sydney Sydney, NSW 2006, Australia richard.philip@sydney.edu.au 

Current version: December 8, 2016 

## Abstract

Using a unique, broker-level dataset, we document an important information channel driving high frequency trading strategies. High frequency traders (HFT) condition their strategies on order book depth imbalances, which are a strong predictor of future price movements. Examining the order book imbalance immediately before each order submission, cancelation and trade, we show HFT supply liquidity on the thick side of the order book and demand liquidity from the thin side. This strategic behavior is more pronounced during volatile periods and when trading speeds increase. However, by competing with non-HFT limit orders, HFT crowd out non-HFT limit orders. 

# High-frequency trading strategies

## Abstract

Using a unique, broker-level dataset, we document an important information channel driving high frequency trading strategies. High frequency traders (HFT) condition their strategies on order book depth imbalances, which are a strong predictor of future price movements. Examining the order book imbalance immediately before each order submission, cancelation and trade, we show HFT supply liquidity on the thick side of the order book and demand liquidity from the thin side. This strategic behavior is more pronounced during volatile periods and when trading speeds increase. However, by competing with non-HFT limit orders, HFT crowd out non-HFT limit orders. 

## 1.0 Introduction

High frequency traders (HFT) influence financial markets in many ways. For example, HFT reduces the bid-ask spread (Angel, Harris and Spatt, 2010; Jones, 2013; Harris, 2013; Hasbrouck and Saar, 2013; Brogaard, Hagstromer, Norden and Riordan, 2015; Malinova, Park and Riordan, 2016), increases price efficiency (Carrion, 2013; Brogaard, Hendershott and Riordan, 2014) and increases overall market depth (Hasbrouck and Saar, 2013). On the whole, HFT play a dominant role in providing liquidity (Hagstromer and Norden, 2013; Hasbrouck and Saar, 2013; Menkveld, 2013; Malinova, Park and Riordan, 2016, Conrad, Wahal and Xiang, 2015), but could also withdraw this liquidity during stressful periods (Kirilenko, Kyle, Samadi and Tuzun, 2016; Brogaard et al., 2016; van Kervel and Menkveld, 2016; Korajczk and Murphy, 2016). Similarly, other studies document that HFT can anticipate future order flow from other traders and predict future price movements (Brogaard, Hendershott and Riordan, 2014; Li, 2014; Hoffmann, 2014; Biais, Foucault and Moinas, 2015; Foucault, Hombert and Rosu, 2016; Hirschey, 2016; Rosu, 2016; Subrahmanyam and Zheng, 2016). While we understand much about how HFT affect financial markets, not much is known about the information channels that drive HFT behavior due to the proprietary nature of their business. 

In this study, we examine HFT order placement strategies and document one such information channel, namely the order book depth imbalance. Similar to previous studies, we provide strong evidence that order book imbalances predict short term future price movements. While all traders (i.e., HFT, institutions and retail) attempt to trade in the direction of the imbalance, we find HFT are better at taking advantage of information contained in the order book, especially at times when the market is volatile and when HFTs become faster. Specifically, HFTs trade in the direction of the order book imbalance and cancel or amend orders when the order book imbalance moves against them.<sup>1</sup> As a result, HFT on average, supply liquidity on the thick side of the order book and demand liquidity from the thin side. By competing with non-HFT limit orders on the thick side of the order book, we find evidence that HFT crowd out non-HFT limit orders from the order book. Our study exposes one important mechanism through which HFT anticipate future order flow and returns. 

For this investigation, we use a unique, broker-level dataset from the Australian Securities Exchange (ASX). Using this dataset, we reconstruct the full limit order book and measure the shape of the order book at the time of each order submission, cancelation, amendment, and trade. The dataset also classifies brokers into three trader types: proprietary HFT firms, institutions and retail. Our primary focus is on HFT trading behavior, relative to institutional and retail traders. Finally, the introduction of faster ITCH technology on the ASX provides a natural experiment for us to investigate the effects of increasing trading speeds. 

We find strong evidence that the shape of the limit order book contains information about future price movements. In particular, when the volume available on the best five prices on the bid (ask) side exceeds the volume available on the best five ask (bid) prices, we show that prices are more likely to rise (fall) in the short-term.<sup>2</sup> We also find that non-HFTs want to act like HFTs, but are less successful when the market indicates it is most important to do so. We demonstrate that all trader types attempt to trade in the direction of the price change predicted by the depth imbalance. Specifically, for all trader types, the percentage of buyer initiated trade volume increases as the depth available on the bid prices grows relative to the depth on the ask prices. However, when depth imbalances are very large (i.e., predicting the largest price changes), we find that HFTs are more successful at trading in the direction of the imbalance, relative to the other trader types. This finding is consistent with the HFT’s speed advantage, in that HFT monitor the limit order book more effectively than institutional and retail investors and react faster to large depth imbalances by submitting aggressive market orders. 

For passive limit orders, we find that HFTs are also better at using information contained in the limit order book. HFTs submit limit orders to the order book primarily when there is a small favorable depth imbalance. As the depth imbalance becomes more favorable, the resting limit order executes in the same direction as the imbalance. On the other hand, if the depth imbalance becomes less favourable, HFT are quick to cancel or amend their orders, reducing adverse selection costs. Together, these strategies mean that HFT supply liquidity to the thick side of the order book and demand liquidity from the thin side, which could exacerbate future depth imbalances. 

Next, we investigate HFT trading behavior around times of high stock volatility. We find HFT demand more liquidity when the market is volatile, in contrast to non-HFT. Further, for both aggressive and passive trades, we show that HFT are even more successful at trading in the direction of the order book during periods of high volatility, relative to non-HFT. In volatile markets, the HFTs use their speed advantage by strategically submitting market orders and cancelling limit orders. When markets are volatile, fast HFT are better able to use market orders to pick off stale limit orders from slower institutional and retail investors. Similarly, HFT use their speed advantage to cancel their own stale limit orders to reduce their adverse selection costs. These results imply that trading speed differentials are particularly advantageous during periods of high volatility. 

The introduction of ITCH in 2012 offers a natural experiment to investigate the effects of a speed change on HFT trading behavior. Using a difference-in-difference framework, we demonstrate that HFT are more successful at trading in the direction of the order book when they gain a larger speed advantage. However, one externality of HFT trading behavior is that there is a crowding out effect on non-HFT limit orders. We find that the probability of execution for institutional and retail limit orders submitted to the best bid and ask prices decreases when HFT gain a larger speed advantage. Further, conditioning limit order executions on the shape of the order book, we show that it is the probability of favourable executions (i.e. non-HFT limit order trading in the direction of the order book imbalance), which falls. While much is known about the effects of HFT, the literature is unclear on how HFTs trade to influence financial markets. While the theoretical literature predicts that fast traders can anticipate the order flow of slow traders (Biais, Foucault and Moinas, 2015; Li, 2014; Hoffmann, 2014; Rosu, 2016), the exact mechanism has not been previously documented in the theoretical or empirical literatures. Empirically, Hirschey (2016) documents that HFTs can anticipate order flow from other investors and Subrahmanyam and Zheng (2016) conclude that HFT manage their limit orders in anticipation of short-term price movements, but do not show how HFT predict future price movements. We demonstrate that the order book depth imbalance is one important mechanism through which HFT gain information on future price movements. Second, several studies find that HFT increase price efficiency. Brogaard, Hendershott and Riordan (2014) demonstrate that HFT buy in the direction of permanent price changes through liquidity demanding orders. Carrion (2013) shows that HFT incorporate information from order flow and market-wide returns more efficiently.<sup>3</sup> But how do they do so? We uncover the information channel through which HFT incorporates information into price. Specifically, we find that HFT increase price efficiency by trading in the direction of the order book imbalance, which is a strong predictor of future price movements. 

Third, our results have implications for studies on the market making role of HFT in equity markets, which find that HFT market making increases market depth (Hendershott, Jones and Menkveld, 2011; Hasbrouck and Saar, 2013; Brogaard, Hagstromer, Norden and Riordan, 2015). However, these findings are typically based on traditional measures of market depth, aggregated across both bid and ask prices. Aggregated measures of market depth do not capture the amount of depth available on the side of the limit order book where it is most needed. For example, a trader submitting a buy market order is more concerned about the depth available on the ask side of the limit order book, rather than aggregated depth over both bid and ask prices. Our results show that HFT on average supply depth on the thick side of the order book but demand depth from the thin side of the order book, i.e., they may add depth, but not on the side that is thin. Similarly, HFT cancel limit orders from the thin side of the order book, which face larger adverse selection costs. 

Finally, several studies in the literature examine HFT liquidity provision during stressful times. Brogaard et al. (2016) examine the stability of liquidity supply by high frequency traders, who do not have the obligation to supply liquidity during stressful periods. They find that HFTs supply liquidity to non-HFTs during extreme price moves in a single security but demand liquidity when several stocks experience simultaneous extreme price moves. However, their analysis focuses exclusively on the liquidity demanded and supplied through the Nasdaq exchange, which represents only 30-40% of all trading activity of the sample stocks. Thus, it is possible that HFT are supplying liquidity on Nasdaq while demanding liquidity from other trading venues. By analysing a mostly consolidated market, we provide further insights on HFT trading activity over the whole market. Unlike Brogaard et al. (2016), our results show that HFT are net demanders of liquidity and become even more aggressive at times of high market volatility. Further, we find that they demand more liquidity from the thin side of the order book, which could exacerbate future volatility.<sup>5</sup> 

In a related group of studies, van Kervel and Menkveld (2016) and Korajcyzk and Murphy (2016) study liquidity provision to institutional trades and show that HFTs initially trade ‘against the wind’ but eventually trade ‘with the wind’ as a large institutional trade progresses. By trading in the same direction as the institutional trader, HFTs increase the implementation shortfall of institutional orders. Our study reveals the mechanism through which HFT detect institutional orders. Specifically, we show that HFT can detect institutional demand through the order book depth imbalance and trade in the same direction of the imbalance before the predicted price rise. 

## 2.0 Institutional details

The Australian Securities Exchange (ASX) is the dominant stock exchange for Australian equities, with over 90% market share of on-market traded volume in 2012.<sup>6</sup> The ASX operates as a continuous limit order book between approximately 10:00 am and 4:00 pm, matching orders based on price and time priority, with a randomized open and a randomized close. Each stock opens with an opening auction at a random time between 10:00 and 10:10 am depending on the starting letter of their ASX code. Similarly, the closing price is determined via a closing price auction that takes place between 4:10 pm and 4:12 pm. While trading on the ASX has been anonymous since the removal of real-time broker identifiers in November 2005, the broker identification behind all executed trades is available to all market participants on a t+3 basis. 

On April 2, 2012, the ASX implemented ASX ITCH, which is an ultra-low latency protocol for accessing ASX market information available to all market participants for a monthly fee. ASX ITCH was designed to meet the requirements of speed sensitive traders and increased market information access speeds by up to seven times existing connections (ASX, 2013). Thus, the introduction of ASX ITCH is likely to create larger benefits for HFT, whose strategies rely on fast response times when new information arrives to the market. 

## 3.0 Data and variable construction

## 3.1 Data and sample selection

We obtain full order book and trade data for stocks in the S&P/ASX 100 index from the AusEquities database provided by the Securities Industry Research Centre of Asia Pacific.<sup>7</sup> The securities contained in our dataset are the most liquid and actively traded among HFT and institutional investors on the ASX. We analyze one year of order level data for the period January 1, 2012 to December 31, 2012, which incorporates the introduction of ITCH on April 2, 2012. To avoid the randomized open and close, we include only trades and orders entered between 10:10:00 and 16:00:00 to ensure that our sample is not contaminated by the opening and closing call auctions. We assume that all outstanding orders remaining in the limit order book at the end of the trading day are cancelled. 

Data from the ASX offer several advantages over other exchanges. For each order, the data contain the stock symbol, date and time of order entry to the millisecond level, order size and price, order identification number and an identifier for the submitting broker. In our dataset, broker identifiers are assigned into three trader categories: proprietary HFT firms (HFT), Institutions, and Retail.<sup>8</sup> We refer to orders originating from Institutions and Retail collectively as non-HFT. Additionally, we use the order identification number to trace subsequent amendments, executions or cancelation back to the original order entry, allowing for a full reconstruction of the limit order book and the tracking of the order and its queue position through time. We rely on the granularity of the data to compute the depth imbalance proxy for trading strategies. Furthermore, because we can replay the full order book, we do not have to rely on trade classification algorithms, such as Lee and Ready (1991),<sup>9</sup> to determine whether a trade is buyer or seller initiated. Following Upson, Johnson and McInish (2015), we aggregate all trade reports at the same price, in the same trade direction, from the same broker, and reported in the same millisecond timestamp into one marketable order. Finally, in comparison to U.S. and European equity markets, the ASX is less fragmented, operating as a virtual monopoly in Australian equities during our period with over 90% of the daily trading volume. 

[Insert Table 1] 

Table 1, Panel A reports the summary statistics for the 94 stocks, which appear in the S&P/ASX 100 index over the full sample period. Market capitalization is measured on January 3, 

2012, the first trading day in the sample, and is expressed in billions of AUD. All other variables are measured on a daily basis and averaged across the sample period. The average stock has a market capitalization of 13.52 AUD billion and volume weighted trade price of $11.67. The average daily dollar volume is 25.5 AUD million and the average number of trades is 2,176. Given that the minimum pricing increment on the ASX is $0.01 for stocks priced above $2.00, an average daily time-weighted quoted spread (Spread) of 1.04 cents indicates that many stocks in the sample are likely to be spread constrained.<sup>10</sup> 

Table 1, Panel B reports the summary statistics for HFT, Institutions and Retail. Consistent with the prior literature, we find that HFT monitor the limit order book more actively. Relative to Institutions and Retail, HFT have a higher percentage of order cancelations, and the median submission to cancel time is significantly lower for HFT. The average number of active and passive trades is approximately equal for HFT, whereas Institutions and Retail are predominantly limit order traders.<sup>11</sup> In the following sections, we investigate how HFT incorporate information contained in the order book to their trading strategies. 

## 3.2 Depth imbalance

Previous studies document a strong relationship between trade imbalances and future returns (Chordia, Roll and Subrahmanyam, 2002; Chordia and Subrahmanyam, 2004). Using more granular limit order book data, recent studies also find strong evidence that order imbalances between the buy and sell schedules of the limit order book are significantly related to future stock returns (Cao, Hansch and Wang, 2008; Cont, Kukanov and Stoikov, 2014). Cont, Kukanov and 

Stoikov (2014) show that high-frequency price changes are mainly driven by imbalances between supply and demand at the best bid and ask prices. Specifically, large buying (selling) pressure on the bid (ask) price predicts future price rises (falls). Further, Ranaldo (2004) examines how the state of the limit order book can affect a trader’s order submission strategy. We use the information contained in the state of the limit order book to proxy for strategic trading. 

To measure the shape of the limit order book at the time of order submission, we calculate depth imbalance (DI) as the difference between the volume available at the best bid and ask prices, as a proportion of the total volume available at the best bid and ask prices.<sup>12</sup> Specifically, for each order book event (i.e., submission, trade, amendment or cancelation) we determine: 

$$
D I _ {t} = \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i t}}
$$

where $\begin{array} { r } { \sum _ { i = 1 } ^ { n } V o l B i d _ { t } \ ( \sum _ { i = 1 } ^ { n } V o l A s k _ { t } ) } \end{array}$ is the volume available at the top n bid (ask) price levels immediately before the order book event, $t . ^ { 1 3 }$ For our main results, we calculate DI based on the volume available at the top five bid and ask prices (n = 5).<sup>14</sup> Our measure of DI is bounded between -1 and 1, where a value close to -1 (1) indicates that the depth available at the ask (bid) prices is much larger than the bid (ask) depth. 

For some tests, for which trade direction is not important, we multiply DI by an indicator for whether the order or trade is a buy or sell to remove the effects of trade direction. We refer to this directionally adjusted DI measure as Adjusted DI. When Adjusted DI is positive, the trade or order event occurs in the direction of the depth imbalance (e.g., a buy trade executes when the bid depth exceeds the ask depth). 

Table 1, Panel C summarizes the average Adjusted DI immediately before active trades, passive trades, order submissions, amendments and cancelations for each trader type. For active trades, we find that all traders trade in the direction of the imbalance, indicating that traders are more likely to submit a market buy (sell) order when the bid (ask) depth is much larger than the ask (bid) depth. 

Comparing the magnitude of Adjusted DI, HFT submit market orders when Adjusted DI is much larger (0.148) compared to 0.024 for both Institutions and Retail. Adjusted DI at the time of passive trades is 0.083, -0.030, and -0.012, for HFT, Institutions, and Retail, respectively. A negative Adjusted DI indicates that Institutions and Retail limit orders are picked off the thin side of the limit order book. In contrast, we find that HFT submit orders when there is a moderate Adjusted DI (Adjusted DI = 0.059) but cancel their limit orders when the order book moves against their resting limit orders, indicated by a lower Adjusted DI (0.017), which reduces the adverse selection costs of HFT. We formally investigate HFT trading strategies and their potential impact on non-HFT trading in the next section. 

## 4.0 Empirical Results

## 4.1 Depth imbalance, future stock prices and aggregate trading volumes

First, we need to establish the information content of order book depth imbalances for our sample stocks. To investigate whether depth imbalances contain information about the future stock price, we rank trades into deciles based on the depth imbalance immediately before the trade for each stock-day. For each transaction, we also calculate future returns by comparing the midpoint of the best bid and ask prices at the time of the trade with the bid-ask midpoint 10 trades in the future. Figure 1, Panel A presents the average future return for trades from each depth imbalance decile. We observe a strong positive relationship between the size and direction of the depth imbalance and future stock returns indicating that depth imbalances in the order book can predict future stock returns.<sup>15</sup> Specifically, when there are a lot of buyers in the order book, relative to the number of sellers, we observe a rise in future stock price. 

[Insert Figure 1] 

Next, we examine how the market responds to order book depth imbalances. For each depth imbalance decile, we calculate the percentage of total volume that is buyer or seller initiated. Given that depth imbalances predict future returns, we expect strategic traders to trade in the direction of the order book imbalance. Specifically, we expect more aggressive buying (i.e., more buyer initiated trades) when a large positive depth imbalance exists and more aggressive selling when there are large negative imbalances. Consistent with strategic trading, our full market results in Figure 1, Panel A confirm a strong positive (negative) relationship between the size of the depth imbalance and the percentage of buyer (seller) initiated trade volume. In the next section, we investigate whether some trader types trade more strategically than other traders based on order book depth imbalances. 

## 4.2 Depth imbalance and trading volumes by trader type

Our previous analysis show that in aggregate, traders buy aggressively when there is a large positive depth imbalance and sell aggressively when a large negative imbalance exists. To investigate whether the relation between depth imbalance and trading volumes differs by trader, for each trader type, we calculate the amount of buyer and seller initiated volumes as a percentage of total market volume. Figure 2, Panels A to C presents the results separately for HFT, Institutions, and Retail, respectively. Consistent with the full sample results from Figure 1, Panel A, we observe a general positive (negative) relationship between depth imbalance and aggressive buying (selling) for all trader types, indicating that all traders trade in the direction of the depth imbalance. 

[Insert Figure 2] 

Comparing between the panels, HFT are more successful than Institutions and Retail when depth imbalances are very positive or very negative. Figure 2, Panel A shows that HFT buy (sell) most aggressively when depth imbalance is the most positive (negative). For Institutions (Panel B) and Retail (Panel C), the percentage of buyer (seller) initiated trades increases with the size of the positive (negative) depth imbalance for moderate levels of imbalances. However, in the extremes (i.e., when depth imbalance is very positive or very negative), both Institutions and Retail are less successful at trading in the direction of the imbalance. 

To further assess whether HFT are more successful at trading on information contained in the depth imbalance, we calculate the executed volume imbalance for each DI decile. Specifically, for each trader type, we calculate the volume imbalance as: 

$$
V o l u m e i m b a l a n c e _ {j} = \frac {\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} - \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}{\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} + \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}
$$

where $\textstyle \sum _ { j = 1 } ^ { n }$ ݉݁ݑ݈݋ܸݕݑܤ $\scriptstyle j ( \sum _ { j = 1 } ^ { n } \sum _ { \ l } ^ { n } \sum _ { j = 1 } ^ { n }$ <sub>௝</sub>݉݁ݑ݈݋݈݈ܸܵ݁ ) is the total aggressive buying (selling) volume for depth imbalance decile, j. 

Figure 2, Panel D, shows the relation between Volume imbalance and a DI for our three trader types. Given the size of DI predicts future returns, a steeper slope indicates a trader is more focused on trading with the order book DI, ahead of future predicted price changes. Comparing the slopes for HFT, Institutions and Retail, our results show HFT Volume imbalance is most sensitive to an order book depth imbalance, indicating that HFT are most successful at buying aggressively before an expected price rise and selling aggressively before an expected price fall, as predicted by DI. 

In Table 2, we test whether a statistically significant difference in Volume imbalance exists between our trader types for each DI decile. When the average DI is the most negative (DI = - 0.375), the volume imbalance for HFT is -61.8%, while Volume imbalance for Institutions and Retail is only -16.8% and -6.2%, respectively. For the most positive DI decile (DI = 0.380), we observe positive volume imbalances for HFT (62.6%), Institutions (17.1%) and Retail (6.1%). Finally, when the order book is balanced, such that the bid depth is approximately equal to the ask depth, the difference in the Volume imbalance is less severe. For example, when DI is only 0.028 (decile 5), the volume imbalances range from 0% (Retail) to only 6.4% (HFT). 

Importantly, we find that HFT Volume imbalance is always significantly below the institutional and retail Volume imbalance when a negative depth imbalance exists (i.e., there is selling pressure in the limit order book). In contrast, when buying pressure exists in the limit order book, volume imbalances are significantly larger for HFT, relative to Institutions and Retail. This result indicates that HFT are more successful at buying when the order book is predicting a future price rise and selling before expected future price declines. Further, comparing between Institutions and Retail, we find that Institutions are more strategic than Retail in trading with the imbalance in 9 of the depth imbalance deciles. 

## [Insert Table 2]

Taken together, these results indicate that all broker types attempt to trade in the direction of a stock’s depth imbalance. However, HFT are more likely to trade on information contained in the depth imbalance than the other trader types, and the difference is even more severe at extreme levels of order book imbalances. One implication for our results is that HFT could be crowding out non-HFT limit orders, especially when large depth imbalances exist. 

In Table 3, we formally test the sensitivity of volume imbalances to depth imbalances for our trader types after controlling for trading volumes, stock and day fixed effects. Based on the volume imbalance for each broker and depth imbalance decile, we estimate the following regression: 

$$
\begin{array}{l} \text {Volume imbalance \%} = \beta_ {0} + \beta_ {1} I (H F T) \times D I + \beta_ {2} I (\text {Institutions}) \times D I + \beta_ {3} I (H F T) + \\ \beta_ {4} I (\text {Institutions}) + \beta_ {5} D I + \beta_ {6} \text {Volume} + \varepsilon \end{array} \tag {1}
$$

where ܫሺ ܨܪ ܶሻ and ܫሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ are indicator variables for HFT and institutional brokers. ܫܦ is the average depth imbalance for the trades in the depth imbalance decile and ܸ݋݈ݑ݉݁ is the natural log of the total traded volume in the decile. We also include controls for stock and day fixed effects. 

## [Insert Table 3]

Table 3, Column 1 presents the results for all trading days in the sample. The main variables of interest are the interaction terms between the trader type and DI. A positive and significant coefficient implies that a trader’s Volume imbalance is more sensitive to the level of DI in the order book. Consistent with our earlier results, we find that ܫሺ ܨܪ ܶሻ ൈ ܫܦ is positive and significant indicating that relative to the other broker categories, HFT are more likely to submit buyer initiated trades when DI is larger. In contrast, ܫሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ ൈ ܫܦ is insignificant and the coefficient on DI is negative and significant indicating that Retail and Institutions trade less on order book information than HFT. 

To investigate the effects of stock volatility on HFT trading behavior, for each stock we rank trading days into terciles based on the daily stock volatility.<sup>16</sup> Table 3, Columns 2 and 3, present the results separately for low and high volatility days, respectively. For both low and high volatility days, we find that HFT use more order book information in their trading strategies than Institutions and Retail.<sup>17</sup> Further, ܫሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ ൈ ܫܦ is negative and significant on high volatility days indicating that Institutions are less successful at trading in the direction of the expected future price movement when the market is highly volatile. 

It is possible that some smaller proprietary HFT firms trade through institutional brokers. While these HFT traders could influence trading imbalances based on the number of trades, it is much more difficult to change overall volume imbalances. To investigate this possibility, in Table 3, Columns 4-6, we replace the dependent variable from Equation (1) with trade imbalance, which is based on the number of buyer and seller initiated trades, rather than the volume of buyer and seller initiated trades. For HFT, our results are largely consistent with our findings based on volume imbalances. For Institutions, in contrast to our results based on volume imbalances, we also find that ܫሺܫ݊ ݐݏ ݅ ݐݑݐ ݅݋݊ݏሻ ൈ ܫܦ is positive and significant for all samples. This result reveals that institutional investors submit small trades that capture information contained in the order book while their large trades are less likely to execute in the direction of the imbalance. This result could be driven by small HFT firms executing their strategies through larger institutional brokers. 

So far, our results show that relative to non-HFT traders, HFT submit more buyer (seller) initiated orders when there are already low levels of liquidity available on the sell (buy) side of the order book. One implication of these results is that HFT strategies could exacerbate future order imbalances, especially when the market is volatile. 

## 4.3 Order submission strategies

In this section, we analyze how order submission strategies differ between our investor categories. Specifically, we measure the order book depth imbalance immediately before a trader submits, amends or cancels an order. For each stock, we estimate the daily average DI for each order book event: aggressive trade (i.e., market or marketable limit order), passive trade, order submission, amendment, and cancelation. 

As discussed earlier, to remove the effects of trade direction, we multiply DI by an indicator for whether the order or trade is a buy or sell so that purchases and sales can be interpreted together (Adjusted DI). An Adjusted DI value of 0 indicates that the order book is balanced and a high positive Adjusted DI value indicates a large depth imbalance in the direction of the order book event.<sup>18</sup> A negative Adjusted DI indicates that the order book is moving against the trader. Specifically, a negative Adjusted DI at the time of a buy trade indicates that a trader is buying when the ask depth exceeds the bid depth, before an expected future price fall. Thus, a strategic trader who uses information contained in the order book should execute trades when Adjusted DI is highly positive and cancel or amend orders when Adjusted DI is low or negative. We estimate the following regression: 

$$
\begin{array}{r} A d j u s t e d D I = \beta_ {0} + \beta_ {1} I (A g g r e s s i v e t r a d e) + \beta_ {2} I (P a s s i v e t r a d e) + \\ \beta_ {3} I (A m e n d) + \beta_ {4} I (C a n c e l) + \beta_ {5} V o l a t i l i t y + \beta_ {6} V o l u m e + \beta_ {7} P r i c e + \beta_ {8} S p r e a d + \varepsilon \end{array}\tag{2}
$$

where ܫሺܣ݃݃ݎ݁ ݏݏ ݅ݒ݁	 ݎݐ ܽ݀݁ሻ is an indicator variable equal to 1 for a market or marketable limit order and 0 otherwise. ܫሺܲܽ ݏݏ ݅ݒ݁	 ݎݐ ܽ݀݁ሻ is an indicator variable equal to 1 for a passive trade and 0 otherwise. ܫሺܣ݉݁݊݀ሻ is an indicator variable equal to 1 for an order amendment and 0 otherwise. ܫሺܥ݈ܽ݊ܿ݁ܽݐ݅݋݊ሻ is an indicator variable equal to 1 for an order cancelation and 0 otherwise. All stock control variables are measured at the daily level. Volatility is the standard deviation of 30- minute mid-quote returns, Volume is the daily dollar volume, Price is the value-weighted average price and Qspread is the time-weighted quoted spread. We also control for stock and day fixed effects. 

Consistent with our strategic trading hypothesis, we find that HFT trade aggressively when a large depth imbalance exists in the order book, and cancel or amend orders when the order book imbalance moves against them. Table 4, Column 1, shows that I(Aggressive trade) and I(Passive trade) is positive and significant indicating that on average, trades take place when the depth imbalance is larger than the depth imbalance at the time of a limit order submission, which is captured in the constant term. Comparing between aggressive and passive trades, we find HFTs submit market orders only when the order imbalance is highly favorable (p-value < 0.01). Further, we find that I(Amend) and I(Cancel) are negative and significant indicating HFT are quick to amend or cancel orders when the depth imbalance becomes less favorable to trade. In doing so, HFT remove stale limit orders before these orders can be picked off the order book by other traders. 

[Insert Table 4] 

We find institutions and retail investors are generally less strategic than HFT on trading on information contained in the limit order book. Similar to HFT, institutions submit aggressive orders when the depth imbalance is in the same direction (Table 4, Column 2). However, for their limit order strategies, I(Passive trade) is negative and significant while I(Amend) and I(Cancel) are both positive and significant. Together, these results indicate that institutions fail to cancel their resting limit orders when the depth imbalance moves in an unfavorable direction, meaning that their stale orders are more likely to be picked off the limit order book. 

For Retail, Table 4, Column 3 reveals that I(Passive trade) is negative and significant indicating that retail limit orders are also picked off the limit order book. Further, the negative and significant coefficient for I(Aggressive trade) suggests that retail investors are unable to strategically time their market orders. Taken together, these result shows that retail investors buy (either through passive or aggressive orders) before an expected fall in the stock price and sell before an expected price rise. 

In Table 4, Columns 4 to 6, we replace the dependent variable with Adjusted DI based on the depth available at the best bid and ask prices (i.e., 1 level of the order book). This test allows us to compare whether some traders are only trading on information contained in the top level of the order book. Comparing with Table 4, Columns 1 and 3, we find that for HFT, the coefficients are similar in sign and significance using either 5 levels or 1 level of order book information. One exception is I(Passive Trade), which is positive and significant when Adjusted DI is calculated using 5 levels of the order book but insignificant when the dependent variable is based on the top level of the order book. The insignificant coefficient on I(Passive trade) indicates that HFT use information contained in the order book, beyond the best bid and ask levels, in their order placement strategies. 

In Table 4, Column 5, the negative coefficients on I(Amend) and I(Cancel) show that Institutions are more likely to cancel and amend orders when the Adjusted DI for the top level of the order book is highly unfavorable. However, I(Passive trade) remains negative and significant, indicating that institutional limit orders are picked off the limit book. For Retail, the results in Column 6 are similar to the results reported earlier using 5 levels of the order book. One exception is I(Aggressive trade), which is now positive and significant, indicating that retail traders cross the spread when there is a large favourable depth imbalance based on the top level of the order book. 

Thus, when a retail investor wishes to buy (sell), and a large limit order queue exists on the best bid (ask) price, they are more likely to demand immediacy by submitting an aggressive market order. Overall, our results provide further support for the conclusion that HFT are more successful at monitoring the limit order book than other trader types. To avoid stale limit orders, HFT cancel or amend their resting limit orders when the order book depth imbalance moves in an unfavourable direction. 

To further investigate the order submission behavior of HFT, we use a multinomial logistic regression model to assess the probability of each order book event based on the prevailing market conditions in the limit order book. For each broker type, we estimate the following regression: 

$$
\begin{array}{c} \operatorname * {P r} (\text {OrderBookEvent}) = \beta_ {0} + \beta_ {1} \text {Adjusted DI} + + \beta_ {2} \text {Volatility} + \beta_ {3} \text {Volume} + \\ \beta_ {4} \text {Price} + \beta_ {5} \text {Spread} + \varepsilon \end{array} \tag {3}
$$

where OrderBookEvent is the dependent variable indicating one of five order book events: Aggressive trade, passive trade, limit order submission, amendment or cancelation. Adjusted DI, Volatility, Volume, Price and Spread are defined as in Equation (2). We estimate the model with limit order submission as the baseline category. 

[Insert Table 5] 

Table 5, Panel A presents the regression coefficients for HFT. Consistent with our expectations, we find that Adjusted DI is positive for aggressive trades. Thus, when Adjusted DI is large, HFT are more likely to submit a market (or marketable limit) order, than a less aggressive limit order. Similarly, Adjusted DI is positive for passive trades, meaning that limit order trade executions are more likely than a limit order submission when Adjusted DI is large. In contrast, Adjusted DI is negative for amendments and cancelations. When Adjusted DI is small, HFT are more likely to amend or cancel an order than to submit a limit order. These results are consistent with strategic HFT order placement strategies. HFT trade when there is a large favourable order book depth imbalance and cancel or amend their resting limit orders when the imbalance moves in an unfavourable direction. 

Table 5, Panels B and C show that Institutions and Retail are less strategic in their order placement strategies. While Institutions are more likely to submit aggressive market orders when the Adjusted DI is large, both Institutions and Retail are more likely to receive a limit order execution when Adjusted DI is lower, relative to Adjusted DI at the time of order submission. Consistent with our earlier findings, this result indicates that Institutions and Retail are less successful at monitoring the limit order book and are more likely to face picking-off risk due to stale orders resting in the book. 

## 4.4 Volatility and HFT strategies

In this section, we further investigate HFT trading behavior in times of high market volatility. We divide each trading day into 30 minute intervals and for each interval, measure its volatility by taking the natural log of the high price divided by the low price during the period. For each stock, we then rank the 30 minute intervals into 10 deciles based on its volatility. Decile 0 (9) contains the least (most) volatile periods. For each decile, we also determine the amount of aggressive volume and passive volume as a percentage of total market volume for each broker type. Figure 3, Panels A to C present the graphs of volatility against aggressive and passive volumes for HFT, Institutions, and Retail, respectively. 

[Figure 3] 

If HFT trade to decrease market volatility, we expect them to supply more passive volume in times of high market uncertainty. In contrast, Figure 3, Panel A shows that HFT aggressive volume increases while their passive volume decreases as the market becomes more volatile. For 

Institutions in Figure 3, Panel B, we observe a fall in both aggressive and passive volumes as volatility increases, which is consistent with Institutions withdrawing from the market in periods of high uncertainty. For Retail, with higher stock volatility, we observe a sharp decrease in aggressive volume (Figure 3, Panel C). Retail passive volume at first decreases and then increases when the market becomes more volatile. This trading pattern could indicate that stale retail limit orders are picked off the limit order book by aggressive HFT orders during volatile periods. 

We test the relationships observed in Figure 3 more formally using the following regression model, controlling for stock and day fixed effects: 

%	݉݁ݑ݈݋ݒ	݁ݒ݅ݏݏ݁ݎ݃݃ܣ 

$$
\begin{array}{l} = \beta_ {0} + \beta_ {1} I (H F T) \times I (\text {Low volatility}) + \beta_ {2} I (H F T) \times I (\text {High volatility}) \\ + \beta_ {3} I (\text {Institutions}) \times I (\text {Low volatility}) + \beta_ {4} I (\text {Institutions}) \\ \times I (\text {High volatility}) + \beta_ {5} I (\text {Low volatility}) + \beta_ {6} I (\text {High volatility}) \\ + \beta_ {7} I (H F T) + \beta_ {8} I (\text {Institutions}) + \beta_ {9} \text {Volatility} + \beta_ {1 0} \text {Volume} + \varepsilon \end{array}\tag{4}
$$

where the dependent variable, Aggressive volume %, is the aggressive volume as a percentage of total aggressive and passive volume for each broker type and volatility decile. I(HFT) and I(Institutions) are indicator variables for HFT and institutional brokers, respectively. I(Low volatility) (I(High volatility)) is an indicator variable equal to 1 for the lowest (highest) volatility decile, and 0 otherwise. For each volatility decile, Volatility is the natural log of the high price divided by the low price and Volume is the total number of shares traded. 

Consistent with our observations from Figure 3, Table 6, Column 1 shows that HFT Aggressive volume % is larger (smaller) when volatility is high (low). This finding is similar across both large stocks and small stocks in Columns 2 and 3. In Table 6, Columns 4 to 6, we replace the dependent variable with Aggressive Trade %. Again, we find HFT trade more aggressively in times of high market volatility, which could potentially exacerbate future volatility especially if HFT are taking liquidity from the thin side of the order book. 

[Insert Table 6] 

To test whether HFT are more strategic in times of market volatility, we investigate the relationship between Adjusted DI and stock volatility for each broker category. As discussed earlier, Adjusted DI measures a trader’s ability to condition their trades on information contained in the order book. Specifically, a positive Adjusted DI indicates that a trade executes in the direction of a favourable imbalance. Thus, Adjusted DI is more positive for traders better able to trade in the direction of the imbalance, or capture predicted future price movements based on the shape of the order book. For each market volatility decile, we calculate the average Adjusted DI for both the aggressive and passive trades in the decile. 

[Insert Figure 4] 

Figure 4, Panels A and B, present the average Adjusted DI for aggressive and passive trades, respectively. Comparing between the broker categories, we observe a large difference in trading behaviors. Notably, for both passive and aggressive trades, we observe a sharp increase in Adjusted DI for HFT as stock volatility increases. 

In contrast, for HFT and Institutions, Adjusted DI is relatively flat across the volatility deciles for their aggressive trades while for their passive trades, Adjusted DI decreases with rising market volatility. This finding supports our hypothesis that non-HFT limit orders are picked off the thin side of the order book, especially in times of high market uncertainty. When the market is volatile, limit orders from slower traders could potentially become stale, leaving more opportunities for faster, more sophisticated traders. 

We test the relationship between Adjusted DI and stock volatility more formally using a regression framework, after controlling for stock and day fixed effects. 

$$
\begin{array}{r l} A d j u s t e d D I = & \\ & = \beta_ {0} + \beta_ {1} I (H F T) \times I (L o w v o l a t i l i t y) + \beta_ {2} I (H F T) \times I (H i g h v o l a t i l i t y) \\ & + \beta_ {3} I (I n s t i t u t i o n s) \times I (L o w v o l a t i l i t y) + \beta_ {4} I (I n s t i t u t i o n s) \\ & \times I (H i g h v o l a t i l i t y) + \beta_ {5} I (L o w v o l a t i l i t y) + \beta_ {6} I (H i g h v o l a t i l i t y) \\ & + \beta_ {7} I (H F T) + \beta_ {8} I (I n s t i t u t i o n s) + \beta_ {9} V o l a t i l i t y + \beta_ {1 0} V o l u m e + \varepsilon \end{array}\tag{5}
$$

We estimate the regression separately for aggressive trades and passive trades. Table 7, Column 1 presents the results for aggressive trades based on the full sample of stocks. As expected, we find for HFT, Adjusted DI is larger when the market is more volatile, indicating that HFT are more strategic when uncertainty exists. The findings are consistent across both the large stock and small stock subsamples (Columns 2 and 3, respectively). While Institutions exhibit similar trading behaviors to HFT, the magnitudes of the coefficients are significantly lower. 

[Insert Table 7] 

Table 7, Columns 4 to 6 present the regression coefficients for passive trades. Consistent with our earlier results, we find that HFT are able to successfully implement limit order strategies, especially when the market is volatile. Relative to Retail passive orders, which is captured in the intercept coefficient, HFT passive orders execute with a larger Adjusted DI, when more stock volatility exists. This finding supports our hypothesis that HFT are more successful at monitoring their limit orders, in particular, when there is high stock volatility. In contrast, I(High volatility) is negative and significant across all stock samples indicating that retail limit orders are picked off more when the market is volatile. One further implication of our results is that HFT aggressively pick off stale orders from the thin side of the order book, which potentially exacerbates future stock volatility when the market is already highly volatile. 

## 4.5 Introduction of ITCH

Using a difference-in-difference framework, we exploit a natural experiment to investigate whether an increase in trading speed affects HFT behavior. On April 2, 2012, the ASX implemented ASX ITCH, which increased market information access speeds for a monthly subscription fee. While subscribing to ASX ITCH is voluntary, and the identity of subscribing brokers is confidential, it is reasonable to assume that traders who are most speed sensitive will be the first to subscribe to the faster data feed. To leave sufficient time for implementation, the pre-ITCH period is the one month period prior to April 2, 2012 (i.e., March 2, 2012 to March 30, 2012) and the post-ITCH period begins one week after the introduction of ITCH and ranges from April 9, 2012 to May 9, 2012. 

Given that HFT strategies are most likely to benefit from the faster trading speeds, we expect that HFT Volume imbalance is more sensitive to the level of DI after switching to ITCH. On the other hand, the gradient of the relationship between Volume imbalance and DI is less affected for Retail and Institutions, who are less speed sensitive. To empirically assess whether ITCH affects trading behavior, we use a difference-in-difference framework and re-estimate Equation (1) after including two interaction terms, I(Pre-ITCH) and I(Post-ITCH), which are indicator variables indicating whether the trading day is before or after the introduction of ITCH. The regression specification is now: 

ܾ݈݅݉ܽܽ݊ܿ݁	݉݁ݑ݈݋ܸ $\% = \beta _ { 0 }$ 

$$
\begin{array}{r l} & + I (P r e - I T C H) \times [ \beta_ {1} I (H F T) \times D I + \beta_ {2} I (I n s t i t u t i o n s) \times D I + \beta_ {3} D I ] \\ & + I (P o s t - I T C H) \times [ \beta_ {4} I (H F T) \times D I + \beta_ {5} I (I n s t i t u t i o n s) \times D I + \beta_ {6} D I ] \\ & + \beta_ {7} I (H F T) + \beta_ {8} I (I n s t i t u t i o n s) + \beta_ {9} V o l u m e + \varepsilon \end{array}\tag{6}
$$

Table 8, Columns 1 and 2, reports the two sets of coefficients $\{ \beta _ { 1 } , \beta _ { 2 } , \beta _ { 3 } \}$ and $\{ \beta _ { 4 } , \beta _ { 5 } , \beta _ { 6 } \}$ . The test of equality between $\beta _ { 1 }$ and $\beta _ { 4 } ( \mathrm { i . e . , } \beta _ { 4 } - \beta _ { 1 } = 0 )$ indicates whether HFT strategies capture more information contained in the order book depth imbalance after the implementation of ITCH. Similarly, the test of equality between $\beta _ { 2 }$ and $\beta _ { 5 }$ , and $\beta _ { 3 }$ and $\beta _ { 6 }$ tests whether institutional and retail strategies change as a result of ITCH, respectively. 

[Insert Table 8] 

Table 8, Columns 1 and 2 show that $\beta _ { 1 }$ and $\beta _ { 4 }$ are both positive and significant indicating that HFT buy when DI is positive and sell when DI is negative in both the pre- and post-ITCH periods. Importantly, the estimate of $\beta _ { 4 }$ is larger than $\beta _ { 1 }$ and the F-test in Column 3 shows that the difference is statistically significant at the 5% level. This result indicates that for HFT, the slope of Volume imbalance against DI is steeper in the post-ITCH period. As a group, HFT trade more strategically on information contained in the limit order book as their market information access speeds increase. In contrast, we cannot reject the null hypothesis that $\beta _ { 2 } = \beta _ { 5 }$ and $\beta _ { 3 } = \beta _ { 6 }$ Consistent with our expectations, we do not find evidence that non-HFT, who are less speed sensitive, trade more strategically after the adoption of ITCH. 

In Table 8, Columns 4 and 5, we replace the dependent variable with trade imbalance. Similar to our results based on volume imbalances, we find that HFT trade more strategically post-ITCH (F-test = 7.71). For Institutions, we also find that their trading is more sensitive to DI after the implementation of ITCH (F-test = 5.27). It is possible that some more speed sensitive institutional brokers also subscribed to ITCH to take advantage of the faster speeds. While it is difficult for an individual broker to influence average volume imbalances, we find that their number of buy and sell orders capture more information contained in order book depth imbalances after trading becomes faster. Based on trade imbalances, we find that Retail, who are less likely to compete on speed, trade less strategically post-ITCH. Specifically, we find that $\beta _ { 6 }$ is negative and significant in the post-ITCH period. 

So far, our results show that HFT are more successful at trading on information contained in the order book imbalance when their trading becomes faster. One implication for these results is that non-HFT traders could be crowded out of the order book as non-HFT trade in the same direction. We investigate whether HFT have a crowding out effect by measuring the probability of execution for HFT and non-HFT limit orders: 

$$
P (f i l l) = \frac {\sum T r a d e V o l u m e}{\sum S u b m i t V o l u m e}
$$

Where $\sum$ ܵݑܾ݉݅ݐܸ݋݈ݑ݉݁ is the total daily volume submitted to the top level of the limit order book and $\sum$ ܶݎܸܽ݀݁݋݈ݑ݉݁	is the total volume that is executed. We measure $P ( f i l l )$ on a daily basis for each broker category. We then estimate the following regression model: 

$$
\begin{array}{r l} & P (F i l l) = \beta_ {0} + \beta_ {1} I (N o n - H F T) \times I (P o s t - I T C H) + \beta_ {2} I (N o n - H F T) \\ & \qquad + \beta_ {3} I (P o s t - I T C H) + \beta_ {4} V o l a t i l i t y + \beta_ {5} V o l u m e + \beta_ {6} P r i c e + \beta_ {7} S p r e a d + \varepsilon_ {1}, \end{array}\tag{6}
$$

where I(Non-HFT) is an indicator variable equal to 1 for an institutional or retail broker, and 0 for an HFT broker and I(Post-ITCH) is an indicator variable equal to 1 for the post-ITCH period, and 0 for the pre-ITCH period. All other control variables are measured on a daily basis. Volatility is the standard deviation of 30-minute mid-quote returns, Volume is the daily dollar volume, Price is the value-weighted average price and Spread is the time-weighted quoted spread. We also control for stock and day fixed effects. 

## [Insert Table 9]

Our main variable of interest is $I ( N o n - H F T ) \times I ( P o s t - I T C H )$ . If HFT are crowding out non-HFT limit orders from the order book, we expect a negative coefficient for $I ( N o n - H F T ) \times I ( P o s t - I T C H )$ , indicating that the probability of a non-HFT order receiving execution decreases when HFT become faster. Consistent with our expectations, Table 8, Column 1 shows that the probability of limit order execution falls for non-HFT after the introduction of ITCH. In Table 9, Column 2, we separate non-HFT traders into Institutions and Retail. For both Institutions and Retail, we find the interaction term with I(Post-ITCH) is negative and significant, indicating that both Institutions and Retail are crowded out from the order book by HFT. 

From our earlier results, we show that a limit order trader benefits when an order executes with a lot of depth on the same side of the order book. On the other hand, if depth builds up on the opposite side of the order book, a limit order is likely to face adverse selection. In Table 9, Columns 3 to 6, we separate P(Fill) into favorable and unfavorable fills. We define a favourable fill as an order execution when the limit order rests on the side of the order book with more depth immediately prior to the trade. For example, if the limit order is sitting on the best bid price, a favourable fill occurs when there is more depth on the bid side of the order book, relative to the ask side. 

Our results show that the decrease in P(Fill) is driven by a fall in the volume of favorable executions. Comparing between Columns 3 and 5, we find that P(Favorable fill) falls for non-HFT while P(Unfavorable fill) remains unchanged after the implementation of ITCH. Separating non-HFT into Institutions and Retail in Columns 4 and 6, we document similar findings. Specifically, the interaction terms with I(Post-ITCH) is negative and significant in Column 4 and insignificant in Column 6. Thus, the likelihood of receiving a favourable limit order execution falls for both institutional and retail traders when HFT gain a speed advantage. Taken together, these results provide evidence that HFT are crowding out non-HFT limit orders from the order book, especially when trading becomes faster. 

## 5.0 Conclusion

The information channels through which HFT trade are relatively unknown. We present strong evidence of one such channel, which provides an explanation for many of the findings documented in the prior literature. We show that order book depth imbalances are strong predictors of future prices. HFT are highly sophisticated in monitoring order book imbalances, which allows them to trade ahead of these predicted price changes. At the same time, when the order book imbalance moves in an unfavourable direction, they are quick to cancel or amend orders that are at high risk of being picked off by other traders. 

HFT order placement strategies based on order book imbalances are particularly successful when the market is volatile. During times of high market volatility, the chance of an institutional or retail limit order becoming stale increases. We find that HFT trade more aggressively and are more successful at picking off stale orders from institutional and retail investors when the market is volatile. However, by demanding liquidity from the thin side of the order book, one consequence is that HFT could potentially exacerbate future limit order book imbalances. 

Using the introduction of ITCH as a natural experiment, we find that HFT become even better at acting on information contained in the order book when their trading becomes faster. However, by competing for favourable trade execution in the same direction as the buying or selling pressure, HFT have a crowding out effect on non-HFT limit orders, which potentially increases non-HFT limit order execution costs. 

Our results on HFT trading behavior have implications for market quality. Several studies show that HFT enhance market quality by improving the informational efficiency of stock prices (Carrion, 2013; Brogaard, Hendershott and Riordan, 2014). On the other hand, HFT could increase transaction costs when they trade in the same direction of the institutional order flow (van Kervel and Menkveld, 2016; Korajcyzk and Murphy, 2016). We show that HFT increase price efficiency by trading in the direction of the order book imbalance, which is a strong predictor of future price movements. However, HFT can also use the information contained in the order book imbalance to detect institutional buying or selling pressure. 

While earlier studies show that overall depth improves (Hasbrouck and Saar, 2013; Hendershott, Jones and Menkveld, 2011), when analysing directional depth, we show that HFT supply liquidity to the order book, but only to the side where there is a lot of existing depth. In contrast, we find that HFT demand liquidity from the thin side of the order book, which is more prominent in times of high market volatility. 

## References



Aitken, M., Chen, H. and Foley, S. (2016) The impact of fragmentation, exchange fees and liquidity provision on market quality. Journal of Empirical Finance, Forthcoming. 





Angel, J., Harris, L. and Spatt, C. 2010. Equity trading in the 21st century. Marshall School of Business Working Paper No. FBE 09-10. 





Biais, B., Foucault, T. and Moinas, S. (2015) Equilibrium fast trading. Journal of Financial Economics, 116, 292-313. 





Boehmer, E., Fong, K. and Wu, J. (2015) International evidence on algorithmic trading. SSRN Working Paper. 





Brogaard, J., Carrion, A., Moyaert, T., Riordan, R., Shkilko, A. and Sokolov, K. (2016) Highfrequency trading and extreme price movements. SSRN Working Paper. 





Brogaard, J., Hagströmer, B., Nordén, L. and Riordan, R. (2015) Trading fast and slow: Colocation and liquidity. Review of Financial Studies, 28, 3407-3443. 





Brogaard, J., Hendershott, T. and Riordan, R. (2014) High-frequency trading and price discovery. Review of Financial Studies, 27, 2267-2306. 





Cao, C., Hansch, O. and Wang, X. (2009) The information content of an open limit-order book. Journal of Futures Markets, 29, 16-41. 





Carrion, A. (2013) Very fast money: High-frequency trading on the Nasdaq. Journal of Financial Markets, 16, 680-711. 





Chaboud, A. P., Chiquoine, B., Hjalmarsson, E. and Vega, C. (2014) Rise of the machines: Algorithmic trading in the foreign exchange market. The Journal of Finance, 69, 2045- 2084. 





Chordia, T., Roll, R. and Subrahmanyam, A. (2002) Order imbalance, liquidity, and market returns. Journal of Financial Economics, 65, 111-130. 





Chordia, T. and Subrahmanyam, A. (2004) Order imbalance and individual stock returns: Theory and evidence. Journal of Financial Economics, 72, 485-518. 





Comerton-Forde, C. and Putniņš, T. J. (2015) Dark trading and price discovery. Journal of Financial Economics, 118, 70-92. 





Conrad, J., Wahal, S. and Xiang, J. (2015) High-frequency quoting, trading, and the efficiency of prices. Journal of Financial Economics, 116, 271-291. 





Cont, R., Kukanov, A. and Stoikov, S. (2014) The price impact of order book events. Journal of Financial Econometrics, 12, 47-88. 





Ellis, K., Michaely, R. and O'hara, M. (2000) The accuracy of trade classification rules: Evidence from nasdaq. Journal of Financial and Quantitative Analysis, 35, 529-551. 





Foucault, T., Hombert, J. and Roşu, I. (2016) News trading and speed. The Journal of Finance, 71, 335-382. 





Hagströmer, B. and Nordén, L. 2013. The diversity of high-frequency traders. Stockholm University Working Paper. 





Harris, L. (2013) What to do about high-frequency trading. Financial Analysts Journal, 69, 6-9. 





Hasbrouck, J. and Saar, G. (2013) Low-latency trading. Journal of Financial Markets, 16, 646- 679. 





Hendershott, T., Jones, C. M. and Menkveld, A. J. (2011) Does algorithmic trading improve liquidity? The Journal of Finance, 66, 1-33. 





Hirschey, N. (2016) Do high-frequency traders anticipate buying and selling pressure? SSRN Working Paper. 





Hoffmann, P. (2014) A dynamic limit order market with fast and slow traders. Journal of Financial Economics, 113, 156-169. 





Jones, C. 2013. What do we know about high-frequency trading? : Columbia Business School Research Paper No. 13-11. 





Kirilenko, A., Kyle, A., Samadi, M. and Tuzun, T. (2016) The flash crash: High frequency trading in an electronic market. Journal of Finance, Forthcoming. 





Korajczyk, R. and Murphy, D. (2016) High frequency market making to large institutional trades. SSRN Working Paper. 





Lee, C. M. C. and Ready, M. J. (1991) Inferring trade direction from intraday data. The Journal of Finance, 46, 733-746. 





Li, W. (2014) High frequency trading with speed hierarchies. University of Maryland Working Paper. 





Malinova, K., Park, A. and Riordan, R. 2016. Taxing high frequency market making: Who pays the bill? : University of Toronto Working Paper. 





Menkveld, A. J. (2013) High frequency trading and the new market makers. Journal of Financial Markets, 16, 712-740. 





Naes, R. and Skjeltorp, J. (2006) Order book characteristics and the volume-volatility relation: Empirical evidence from a limit order market. SSRN Working Paper. 





Ranaldo, A. (2004) Order aggressiveness in limit order book markets. Journal of Financial Markets, 7, 53-74. 





Rosu, I. (2016) Fast and slow informed trading. SSRN Working Paper. 





Subrahmanyam, A. and Zheng, H. (2016) Limit order placement by high-frequency traders. SSRN Working Paper. 





Van Kervel, V. (2015) Competition for order flow with fast and slow traders. Review of Financial Studies, 28, 2094-2127. 





Van Kervel, V. and Menkveld, A. J. (2016) High-frequency trading around large institutional orders. SSRN Working Paper. 



## Appendix 1

In this appendix, we investigate the information content of resting limit orders behind the best bid and offer prices. To determine the incremental information content of resting limit orders at levels 2 to 5 of the order book, we estimate a restricted model, which only contains the depth imbalance for the best bid and offer, and an unrestricted model, which contains the DI for the best bid and offer and for levels 2-5 of the limit order book. For each stock and day, we perform the following regressions: 

:model Restricted $R e t u r n = \beta _ { 0 } + \beta _ { 1 } D I _ { T o p L e v e l } + \varepsilon$ 

Unrestricted model: $R e t u r n = \beta _ { 0 } + \beta _ { 1 } D I _ { T o p L e v e l } + \beta _ { 2 } D I _ { L e v e l s 2 - 5 } + \varepsilon$ 

Return is calculated as the log of the difference between the bid-ask midpoint 10 trades in the future and the midpoint price just prior to the trade. DI is the depth imbalance immediately before the trade, which is calculated as the difference between the volumes available at the bid and ask prices as a proportion of the total volume available at the bid and ask prices. We calculate DI for the top level of the order book $( D I _ { T o p L e v e l } )$ as well as for levels 2 to 5 of the limit order book $( D I _ { L e v e l s 2 - 5 } )$ 

Table A1 summarizes the mean adjusted R-square for the restricted and unrestricted models. If $D I _ { L e v e l s 2 - 5 }$ adds incremental information about the future price movements, we expect a higher adjusted R-square for the unrestricted model, relative to the restricted model. For over 85% of our regressions, the F-test is significant at the 1% level, indicating that $D I _ { L e v e l s 2 - 5 }$ adds additional explanatory power. This result indicates that limit orders behind the best bid and offer also contains information on future stock returns. 

<table><tr><td rowspan="2"></td><td colspan="2">Adjusted R-square</td><td rowspan="2">% with F-test significant at 1%</td></tr><tr><td>Restricted model</td><td>Unrestricted model</td></tr><tr><td>Mean</td><td>12.02%</td><td>13.48%</td><td rowspan="2">85.64%</td></tr><tr><td>Median</td><td>10.96%</td><td>12.45%</td></tr></table>


Table A1. Adjusted R-square for restricted and unrestricted model.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/9339805bebbb767fb7a50284f233afaf64e74549d88418c59406fdd9c70e5bd0.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/986ab6ef4b531e79240ddfaeb57edbd316d1ce25bc0f1dfaf59f6b24f9790fd2.jpg)



Fig. 1. Fig. 1 shows the relationship between depth imbalance, returns (Panel A) and volumes (Panel B). Directional depth imbalance is calculated as the difference between the depths available at the five best bid and ask prices, scaled by total depth available at these price levels, immediately before each trade. For each stock day, we rank trades into 10 depth imbalance deciles. Trades with the most negative depth imbalances (i.e., ask depth > bid depth) are categorized as decile 0 and trades with the most positive depth imbalances (i.e., bid depth > ask depth) are in decile 9. In Panel A, we calculate returns by comparing the current midpoint of the best bid and ask prices with the midpoint price 10 trades in the future. In Panel B, the blue (red) dots represent the average percentage of buyer (seller) initiated volume, relative to total trade volume, for each depth imbalance decile.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/c53bb8d0f5935969aad9aef573db55f74a6185262b7361bf89c5793ad92805d3.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/8135693657f3f0b41e2e29c8ba6cc92b8676257922d130adf6724bfae765030d.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/0250a562b6612b25eefbc9d8c7b7f69d086c3a24e28b4f1d34a064d3c703ea35.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/7b7166e6d8734cad35ab745f0cb624ab45856ff595e65ac22407216c23bcd7e5.jpg)



Fig 2. Fig. 2 shows the relationship between depth imbalance and trading volumes for each broker category. Directional depth imbalance is calculated as the difference between the depths available at the five best bid and ask prices, scaled by total depth available at these price levels, immediately before each trade. For each stock day, we rank trades into 10 depth imbalance deciles. Trades with the most negative depth imbalances (i.e., ask depth > bid depth) are categorized as decile 0 and trades with the most positive depth imbalances (i.e., bid depth > ask depth) are in decile 9. Panels A-C present the results for HFT, Institutions, and Retail, respectively. The blue (red) dots represent the average percentage of buyer (seller) initiated volume, relative to total trade volume, for each depth imbalance decile and broker type. Panel D shows the volume imbalance (i.e., (Buys-Sells)/(Buys + Sells)) for each broker type and depth imbalance decile.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/01b5c0bef7aa705d2c0f87f6f83af66e70cce199f52389669e31a9ae36ce4088.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/f40f73ade2c4d19486786f4f6e3fbb661d22f92d27b08360aa9b03bdfed4dd2f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/126a7ce593aee2e1257e61bd9d524c45781093d9e3cdb4f394604b6091575273.jpg)



Fig. 3. Fig. 3 shows the relationship between volatility and trading volume for each broker category. Volatility is calculated as the log of ratio of the high to the low price over each 30 minute trading interval. Trading intervals are then ranked into volatility deciles. Panels A-C present the results for HFT, Institutions, and Retail, respectively. For each broker category, we calculate the percentage of aggressive (blue) and passive (red) trading volume, relative to total trading volume, for each volatility decile.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/00c93cb03bdad274e16e135cbe1342dc13fc0eee7df79908f69faca34b0bdfcf.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/3d715c9d-c421-4ea0-bbf3-e13ae260d112/7d1e2246e24a4ca7256a5f1baaaba9f62ab822b14a3eb0792c981b54c3c2cbc2.jpg)



Fig. 4. Fig. 4 shows the relationship between volatility and depth imbalance for each broker category. Volatility is calculated as the log of ratio of the high to the low price over each 30 minute trading interval. Trading intervals are then ranked into volatility deciles. For each broker category, we calculate the depth imbalance immediately before each aggressive (Panel A) or passive (Panel B) trade execution. Depth imbalance is calculated as the difference between the depths available at the five best bid and ask prices, scaled by total depth available at these price levels, immediately before each trade. We multiply depth imbalance by a buy or sell indicator so that buys and sells can be interpreted together. Depth imbalances are then averaged over each volatility decile by broker category.


## Table 1

Summary statistics 

Table 1, Panel A reports statistics for the 94 stocks that remain in the ASX 100 index for the period January 3, 2012 to December 31, 2012. Market capitalization is the stock’s market capitalization on January 3, 2012. Dollar volume is the average daily dollar volume in AUD. Number of trades is the average daily number of transactions. Price is the average trade price in AUD. Volatility is the difference between the log of the intraday high ask price and the log of the intraday low bid price. Spread is the time weighted average difference between the best bid and offer prices in AUD cents. The broker associated with each order book event is classified into three types: proprietary HFT (HFT), institutional (Institutions), or retail (Retail). Panel B reports the trading characteristics for each broker type. Panel C reports the average adjusted depth imbalance (Adjusted DI) for each trader type. For each order book event, Adjusted DI is calculated as: 

$$
A d j u s t e d D I _ {t} = q \times \frac {\sum_ {i = 1} ^ {5} V o l B i d _ {i t} - \sum_ {i = 1} ^ {5} V o l A s k _ {i t}}{\sum_ {i = 1} ^ {5} V o l B i d _ {i t} + \sum_ {i = 1} ^ {5} V o l A s k _ {i t}}
$$


where $\begin{array} { r } { \sum _ { i = 1 } ^ { 5 } V o l B i d _ { t } \ : ( \sum _ { i = 1 } ^ { 5 } V o l A s k _ { t } ) } \end{array}$ is the volume available at the top 5 bid (ask) price levels immediately before the order book event, t. q is an indicator variable equal to 1 for buys and -1 for sells.


<table><tr><td colspan="6">Panel A: Stock characteristics</td></tr><tr><td></td><td>Mean</td><td>Std.dev.</td><td>Q1</td><td>Median</td><td>Q3</td></tr><tr><td>Market capitalization (AUD billions)</td><td>13.52</td><td>22.77</td><td>2.844</td><td>10.00</td><td>114.8</td></tr><tr><td>Dollar volume (AUD millions)</td><td>25.54</td><td>43.67</td><td>5.179</td><td>10.51</td><td>23.44</td></tr><tr><td>Number of trades</td><td>2,176</td><td>1,718</td><td>1,088</td><td>1,633</td><td>2,614</td></tr><tr><td>Price (AUD)</td><td>11.67</td><td>13.18</td><td>3.052</td><td>6.431</td><td>15.05</td></tr><tr><td>Volatility (%)</td><td>2.026</td><td>1.215</td><td>1.280</td><td>1.756</td><td>2.443</td></tr><tr><td>Spread (cents)</td><td>1.037</td><td>0.369</td><td>0.956</td><td>1.014</td><td>1.119</td></tr></table>

<table><tr><td></td><td>HFT</td><td>Institutions</td><td>Retail</td></tr><tr><td colspan="4">Panel B: Trader characteristics</td></tr><tr><td>Average daily submissions</td><td>839.5</td><td>12,781</td><td>525.6</td></tr><tr><td>Average daily cancelations</td><td>375.9</td><td>4,309</td><td>58.79</td></tr><tr><td>Average daily trades (aggressive)</td><td>241.9</td><td>1,463</td><td>98.90</td></tr><tr><td>Average daily trades (passive)</td><td>279.4</td><td>3,529</td><td>167.7</td></tr><tr><td>Median trade size</td><td>1,681</td><td>926.5</td><td>2,187</td></tr><tr><td>Median submission to cancel time</td><td>128.7</td><td>246.8</td><td>3,034</td></tr></table>

<table><tr><td colspan="4">Panel C: Adjusted depth imbalance</td></tr><tr><td>Trades (aggressive)</td><td>0.148</td><td>0.024</td><td>0.024</td></tr><tr><td>Trades (passive)</td><td>0.083</td><td>-0.030</td><td>-0.012</td></tr><tr><td>Submissions</td><td>0.059</td><td>-0.005</td><td>0.030</td></tr><tr><td>Amendments</td><td>0.043</td><td>-0.003</td><td>0.014</td></tr><tr><td>Cancelations</td><td>0.017</td><td>0.003</td><td>0.027</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 2

V<sub>o</sub>l<sub>ume</sub> <sub>an</sub>d d<sub>ep</sub>th i<sub>m</sub>b<sub>a</sub>l<sub>ances</sub> b<sub>y</sub> t<sub>ra</sub>d<sub>er</sub> t<sub>ype</sub> 

Table 2 reports the volume imbalance for each depth imbalance (DI) decile by trader type For each stock we rank trades for each stock into DI deciles <sub>w</sub>hi<sub>c</sub>h i<sub>s ca</sub>l<sub>.</sub>F<sub>or every</sub> t<sub>ra</sub>d<sub>e</sub> DI i<sub>s ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub>d <sub>as :</sub> 

$$
D I _ {t} = \frac {\sum_ {i = 1} ^ {5} V o l B i d _ {i t} - \sum_ {i = 1} ^ {5} V o l A s k _ {i t}}{\sum_ {i = 1} ^ {5} V o l B i d _ {i t} + \sum_ {i = 1} ^ {5} V o l A s k _ {i t}}
$$

<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { i = 1 } ^ { 5 } V o l B i d _ { t } \left( \sum _ { i = 1 } ^ { 5 } V o l A s k _ { t } \right) } \end{array}$ is the volume available at the to 5 bid (ask) rice levels immediatel before the order book event t Then for each DI d<sub>ec</sub>il<sub>e we ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance as :</sub> 

$$
V o l u m e i m b a l a n c e _ {j} = \frac {\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} - \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}{\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} + \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}
$$


<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { j = 1 } ^ { n } B u y V o l u m e _ { j } ( \sum _ { j = 1 } ^ { n } } \end{array}$ ܵ݁ ݈ ݈ܸ݋ ݈ݑ݉݁<sub>௝</sub> ) is the total aggressive buying (selling) volume for depth imbalance decile<sub>,</sub> j<sub>.</sub> Column 2 reports the average DI C<sub>o</sub>l<sub>u</sub>mn<sub>s</sub> 3 -5 r<sub>epo</sub>rt th<sub>e ave</sub>r<sub>age</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> f<sub>o</sub>r HFT I<sub>ns</sub>tit<sub>u</sub>ti<sub>ons a</sub>nd R<sub>e</sub>t<sub>a</sub>il<sub>.</sub> C<sub>o</sub>l<sub>u</sub>mn<sub>s</sub> 6- 8 r<sub>epo</sub>rt th<sub>e</sub> diff<sub>e</sub>r<sub>e</sub>n<sub>ces</sub> in V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> m<sub>ea</sub>n<sub>s</sub> b<sub>e</sub>t<sub>wee</sub>n th<sub>e</sub> t<sub>ra</sub>d<sub>er</sub> t<sub>ypes as</sub> i<sub>n</sub>di<sub>ca</sub>t<sub>e</sub>d i<sub>n</sub> th<sub>e co</sub>l<sub>umn</sub> h<sub>ea</sub>di<sub>ngs</sub> b<sub>ase</sub>d <sub>on a</sub> t-t<sub>es</sub>t <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y</sub>


<table><tr><td>(1)Depth imbalance decile</td><td>(2)Depth imbalance</td><td>(3)HFT</td><td>(4)Institutions</td><td>(5)Retail</td><td colspan="2">(6)HFT vs. Institutions</td><td colspan="2">(7)HFT vs. Retail</td><td colspan="2">(8)Institutions vs. Retail</td></tr><tr><td>0 (most negative)</td><td>-0.375</td><td>-61.8</td><td>-16.8</td><td>-6.2</td><td>-44.9</td><td>***</td><td>-55.6</td><td>***</td><td>-55.6</td><td>***</td></tr><tr><td>1</td><td>-0.219</td><td>-46.8</td><td>-12.8</td><td>-7.4</td><td>-34.0</td><td>***</td><td>-39.5</td><td>***</td><td>-39.5</td><td>***</td></tr><tr><td>2</td><td>-0.141</td><td>-34.2</td><td>-8.6</td><td>-5.6</td><td>-25.6</td><td>***</td><td>-28.6</td><td>***</td><td>-28.6</td><td>***</td></tr><tr><td>3</td><td>-0.080</td><td>-21.3</td><td>-4.6</td><td>-4.1</td><td>-16.7</td><td>***</td><td>-17.2</td><td>***</td><td>-17.2</td><td></td></tr><tr><td>4</td><td>-0.025</td><td>-6.9</td><td>-1.0</td><td>-1.8</td><td>-5.9</td><td>***</td><td>-5.0</td><td>***</td><td>-5.0</td><td>*</td></tr><tr><td>5</td><td>0.028</td><td>6.4</td><td>2.8</td><td>0.0</td><td>3.5</td><td>***</td><td>6.3</td><td>***</td><td>6.3</td><td>***</td></tr><tr><td>6</td><td>0.084</td><td>20.2</td><td>6.0</td><td>1.3</td><td>14.3</td><td>***</td><td>18.9</td><td>***</td><td>18.9</td><td>***</td></tr><tr><td>7</td><td>0.146</td><td>33.3</td><td>9.8</td><td>3.7</td><td>23.5</td><td>***</td><td>29.6</td><td>***</td><td>29.6</td><td>***</td></tr><tr><td>8</td><td>0.225</td><td>47.1</td><td>14.2</td><td>4.4</td><td>32.9</td><td>***</td><td>42.7</td><td>***</td><td>42.7</td><td>***</td></tr><tr><td>9 (most positive)</td><td>0.380</td><td>62.6</td><td>17.1</td><td>6.1</td><td>45.5</td><td>***</td><td>56.5</td><td>***</td><td>56.5</td><td>***</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 3

R<sub>e</sub>l<sub>a</sub>ti<sub>on</sub> b<sub>e</sub>t<sub>ween</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance an</sub>d D<sub>ep</sub>th i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> 

T<sub>a</sub>bl<sub>e</sub> 3 <sub>repor</sub>t<sub>s</sub> th<sub>e</sub> <sub>regress</sub>i<sub>on</sub> <sub>o</sub>f V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> <sub>or</sub> T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> <sub>aga</sub>i<sub>ns</sub>t D<sub>ep</sub>th i<sub>m</sub>b<sub>a</sub>l<sub>ance .</sub> T<sub>ra</sub>d<sub>es</sub> <sub>are</sub> <sub>sor</sub>t<sub>e</sub>d i<sub>n</sub>t<sub>o</sub> d<sub>ec</sub>il<sub>es</sub> b<sub>ase</sub>d <sub>on</sub> th<sub>e</sub> <sub>s</sub>i<sub>ze</sub> <sub>o</sub>f th<sub>e</sub> d<sub>ep</sub>th imbalance (DI) immediately before the trade <sub>.</sub> For each DI decile and trader type we calculate Volume imbalance as : 

$$
V o l u m e i m b a l a n c e _ {j} = \frac {\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} - \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}{\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} + \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}
$$

<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { j = 1 } ^ { n } B u y V o l u m e _ { j } ( \sum _ { j = 1 } ^ { n } S e l l V o l u m e _ { j } ) } \end{array}$ is the total aggressive buying (selling) volume for depth imbalance decile j<sub>.</sub> For columns 1 -3 we estimate the f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near regress</sub>i<sub>on w</sub>hi<sub>c</sub>h i<sub>s</sub> b<sub>ase</sub>d <sub>on</sub> DI d<sub>ec</sub>il<sub>es :</sub> 

݅<sub>݉</sub>ܾ<sub>ܽ</sub>݈<sub>ܽ݊ܿ݁</sub>	<sub>݉݁ݑ</sub>݈<sub>݋</sub>ܸ $\begin{array} { r } { \vartheta _ { 0 } = \beta _ { 0 } + \beta _ { 1 } I ( H F T ) \times D I + \beta _ { 2 } I ( I n s t i t u t i o n s ) \times D I + \beta _ { 3 } I ( H F T ) + \beta _ { 4 } I ( I n s t i t u t i o n s ) + \beta _ { 5 } D I + \beta _ { 6 } V o l u m e + \varepsilon } \end{array}$ 


where I(HFT) and I(Institutions) are indicator variable for HFT and Institutions respectivel<sub>y.</sub> DI is the average depth imbalance for the decile and Volume is the <sub>na</sub>t<sub>ura</sub>l l<sub>og o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l <sub>s</sub>h<sub>are vo</sub>l<sub>ume</sub> t<sub>ra</sub>d<sub>e</sub>d i<sub>n</sub> th<sub>e</sub> d<sub>ec</sub>il<sub>e</sub> I<sub>n</sub> C<sub>o</sub>l<sub>umns</sub> 4-6 <sub>we rep</sub>l<sub>ace</sub> th<sub>e</sub> d<sub>epen</sub>d<sub>en</sub>t <sub>var</sub>i<sub>a</sub>bl<sub>e w</sub>ith T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance w</sub>hi<sub>c</sub>h i<sub>s ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub>d b<sub>ase</sub>d on the number rather than the volume of aggressive trades For each stock low (high) volatility days represent the lowest (highest) tercile of trading days based <sub>on s</sub>t<sub>oc</sub>k <sub>vo</sub>l<sub>a</sub>tilit<sub>y w</sub>h<sub>ere vo</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> hi<sub>g</sub>h <sub>as</sub>k <sub>pr</sub>i<sub>ce an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> l<sub>ow</sub> bid <sub>pr</sub>i<sub>ce</sub> All <sub>regress</sub>i<sub>ons</sub> <sub>con</sub>t<sub>ro</sub>l f<sub>or s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s</sub> W<sub>e repor</sub>t h<sub>e</sub>t<sub>eros</sub>k<sub>e</sub>d<sub>as</sub>ti<sub>c</sub>it<sub>y</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> i<sub>n paren</sub>th<sub>eses</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y</sub>


<table><tr><td></td><td colspan="3">Volume imbalance%</td><td colspan="3">Trade imbalance%</td></tr><tr><td></td><td>(1)All trading days</td><td>(2)Low volatility days</td><td>(3)High volatility days</td><td>(4)All trading days</td><td>(5)Low volatility days</td><td>(6)High volatility days</td></tr><tr><td>I(HFT) × DI</td><td>1.017***(0.04)</td><td>0.980***(0.04)</td><td>1.084***(0.04)</td><td>0.921***(0.03)</td><td>0.895***(0.04)</td><td>0.962***(0.03)</td></tr><tr><td>I(Institutions) × DI</td><td>-0.021(0.02)</td><td>0.006(0.02)</td><td>-0.036*(0.02)</td><td>0.080***(0.02)</td><td>0.081***(0.03)</td><td>0.088***(0.02)</td></tr><tr><td>I(HFT)</td><td>0.015(0.01)</td><td>0.024*(0.01)</td><td>0.009(0.01)</td><td>0.022*(0.01)</td><td>0.028**(0.01)</td><td>0.014(0.01)</td></tr><tr><td>I(Institutions)</td><td>0.018*(0.01)</td><td>0.024*(0.01)</td><td>0.016(0.01)</td><td>0.043***(0.01)</td><td>0.047***(0.01)</td><td>0.036***(0.01)</td></tr><tr><td>DI</td><td>-0.204***(0.03)</td><td>-0.183***(0.03)</td><td>-0.242***(0.03)</td><td>-0.138***(0.02)</td><td>-0.140***(0.03)</td><td>-0.129***(0.02)</td></tr><tr><td>Volume</td><td>0.011***(0.00)</td><td>0.007**(0.00)</td><td>0.008**(0.00)</td><td>0.010***(0.00)</td><td>0.006(0.00)</td><td>0.009**(0.00)</td></tr><tr><td>Constant</td><td>-0.288***(0.03)</td><td>-0.209***(0.04)</td><td>-0.242***(0.05)</td><td>-0.288***(0.03)</td><td>-0.292***(0.05)</td><td>-0.216***(0.05)</td></tr><tr><td>Obs.</td><td>503,990</td><td>150,376</td><td>166,644</td><td>503,990</td><td>150,376</td><td>166,644</td></tr><tr><td>Adj. R-square</td><td>0.183</td><td>0.175</td><td>0.198</td><td>0.254</td><td>0.242</td><td>0.283</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 4

Li<sub>m</sub>it <sub>or</sub>d<sub>er</sub> <sub>p</sub>l<sub>acemen</sub>t <sub>s</sub>t<sub>ra</sub>t<sub>eg</sub>i<sub>es</sub> 

Table 4 compares the Adjusted DI immediately before order book events for HFT Institutions and Retail The dependent variable is Adjusted DI which is the daily average Adjusted DI for each order book event and trader type 

$$
A d j u s t e d D I _ {t} = q \times \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i t}}
$$

<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { i = 1 } ^ { n } V o l B i d _ { t } \ ( \sum _ { i = 1 } ^ { n } V o l A s k _ { t } ) } \end{array}$ is the volume available at the top n bid (ask) price levels immediately before the order book event t<sub>.</sub> q is an indicator <sub>var</sub>i<sub>a</sub>bl<sub>e equa</sub>l t<sub>o</sub> 1 f<sub>or</sub> b<sub>uys an</sub>d - 1 f<sub>or se</sub>ll<sub>s</sub> W<sub>e presen</sub>t th<sub>e coe</sub>ffi<sub>c</sub>i<sub>en</sub>t <sub>es</sub>ti<sub>ma</sub>t<sub>es</sub> f<sub>or</sub> th<sub>e</sub> f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near regress</sub>i<sub>on:</sub> 

݁݀ݐݏݑ݆݀ܣ $D I = \beta _ { 0 } + \beta _ { 1 } I ( A g \varepsilon$ ݅ܿ݁ݎܲ<sub>଻</sub>ߚ	൅ ݉݁ݑ݈݋ܸ<sub>଺</sub>ߚ	൅ <sub>ݕ</sub>ݐ݈݅ ݅ݐ݈ܽ݋ܸ<sub>ହ</sub>ߚ	൅ ሻܽ݊ܿ݁ ݈ܥሺܫ<sub>ସ</sub>ߚ	൅ ሻ݉݁݊݀ܣሺܫ<sub>ଷ</sub>ߚ൅ ሻܽ݀݁ݎݐ	݁ݒ݅ݏݏܲܽሺܫ<sub>ଶ</sub>ߚ	൅ ሻܽ݀݁ݎݐ	݁ݒ݅ݏݏ݁ݎ $+ \beta _ { 8 } S p r e a d + \varepsilon$ 


where ܫ ሺ∙ሻ is an indicator variable e<sub>q</sub>ual to 1 for the order book event s<sub>p</sub>ecified in the <sub>p</sub>arentheses and 0 otherwise <sub>.</sub> All control variables are measured on a dail<sub>y</sub> b<sub>as</sub>i<sub>s</sub> V<sub>o</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>a</sub> hi<sub>g</sub>h <sub>as</sub>k <sub>pr</sub>i<sub>ce an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>a</sub> l<sub>ow</sub> bid <sub>pr</sub>i<sub>ce</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>s</sub> th<sub>e na</sub>t<sub>ura</sub>l l<sub>og o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l d<sub>a</sub>il<sub>y s</sub>h<sub>are vo</sub>l<sub>ume</sub> P<sub>r</sub>i<sub>ce</sub> i<sub>s</sub> th<sub>e average</sub> d<sub>a</sub>il<sub>y</sub> t<sub>ra</sub>d<sub>e pr</sub>i<sub>ce</sub> S<sub>prea</sub>d i<sub>s</sub> th<sub>e</sub> ti<sub>me we</sub>i<sub>g</sub>ht<sub>e</sub>d <sub>average</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> b<sub>es</sub>t bid <sub>an</sub>d <sub>o</sub>ff<sub>er pr</sub>i<sub>ces</sub> All <sub>regress</sub>i<sub>ons</sub> <sub>con</sub>t<sub>ro</sub>l f<sub>or s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s</sub> W<sub>e repor</sub>t h<sub>e</sub>t<sub>eros</sub>k<sub>e</sub>d<sub>as</sub>ti<sub>c</sub>it<sub>y</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> i<sub>n paren</sub>th<sub>eses</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y</sub>


<table><tr><td rowspan="2"></td><td colspan="3">Adjusted depth imbalance (5 levels)</td><td colspan="3">Adjusted depth imbalance (1 level)</td></tr><tr><td>(1)HFT</td><td>(2)Institutional</td><td>(3)Retail</td><td>(4)HFT</td><td>(5)Institutional</td><td>(6)Retail</td></tr><tr><td>I(Aggressive trade)</td><td>0.087***(0.00)</td><td>0.029***(0.00)</td><td>-0.006***(0.00)</td><td>0.330***(0.01)</td><td>0.221***(0.01)</td><td>0.059***(0.00)</td></tr><tr><td>I(Passive trade)</td><td>0.024***(0.00)</td><td>-0.026***(0.00)</td><td>-0.041***(0.00)</td><td>0.002(0.01)</td><td>-0.095***(0.00)</td><td>-0.077***(0.00)</td></tr><tr><td>I(Amend)</td><td>-0.014***(0.00)</td><td>0.001**(0.00)</td><td>-0.015***(0.00)</td><td>-0.026**(0.01)</td><td>-0.061***(0.00)</td><td>-0.030***(0.00)</td></tr><tr><td>I(Cancel)</td><td>-0.043***(0.00)</td><td>0.008***(0.00)</td><td>-0.003(0.00)</td><td>-0.278***(0.02)</td><td>-0.035***(0.00)</td><td>-0.018***(0.00)</td></tr><tr><td>Volatility</td><td>0.380***(0.10)</td><td>0.105**(0.04)</td><td>0.206**(0.08)</td><td>0.101(0.08)</td><td>0.070(0.04)</td><td>0.046(0.07)</td></tr><tr><td>Volume</td><td>-0.001(0.00)</td><td>0.004***(0.00)</td><td>-0.000(0.00)</td><td>0.001(0.00)</td><td>0.002*(0.00)</td><td>0.001(0.00)</td></tr><tr><td>Price</td><td>-0.007(0.01)</td><td>-0.006**(0.00)</td><td>0.001(0.01)</td><td>0.025(0.02)</td><td>-0.003(0.00)</td><td>-0.005(0.01)</td></tr><tr><td>Spread</td><td>3.871***(0.64)</td><td>0.545**(0.26)</td><td>-0.496(0.71)</td><td>1.753*(0.99)</td><td>-1.009***(0.27)</td><td>-0.483(0.58)</td></tr><tr><td>Constant</td><td>-0.004(0.04)</td><td>-0.071***(0.02)</td><td>0.040(0.03)</td><td>-0.025(0.05)</td><td>-0.025(0.02)</td><td>0.033(0.03)</td></tr><tr><td>Obs.</td><td>109,351</td><td>111,417</td><td>110,409</td><td>109,351</td><td>111,417</td><td>110,409</td></tr><tr><td>Adj. R-square</td><td>0.265</td><td>0.132</td><td>0.042</td><td>0.531</td><td>0.712</td><td>0.091</td></tr></table>

## Table 5

Multinomial logistic regressions for limit order placement strategies 

Table 5 assesses the probability of each order book event based on prevailing market conditions. We present the coefficient estimates for the following multinomial logistic regression: 

ߝ ൅ ݁ܽ݀ݎ݌ܵ<sub>ହ</sub>ߚ ൅ ݅ܿ݁ݎܲ<sub>ସ</sub>ߚ	൅ ݉݁ݑ݈݋ܸ<sub>ଷ</sub>ߚ	൅ ݕݐ݈݅݅ݐ݈ܽ݋ܸ<sub>ଶ</sub>ߚ	൅	൅ ܫܦ	݁݀ݐݏݑ݆݀ܣ<sub>ଵ</sub>ߚ	൅<sub>଴</sub>ߚ	ൌ ሻݐ݁݊ݒܧ݇݋݋ܤݎ݀݁ݎܱPrሺ 

here OrderBookEvent is the dependent variable indicating one of five order book events: Aggressive trade, passive trade, limit order submission, amendment or cancelation. Volatility is the difference between the log of the intraday high ask price and the log of the intraday low bid price. Volume is the natural log of the total daily share volume. Price is the average daily trade price. Spread is the time weighted average difference between the best bid and offer prices. The main independent variable is Adjusted DI, which is the daily average Adjusted DI for each order book event and trader type: 

$$
A d j u s t e d D I _ {t} = q \times \frac {\sum_ {i = 1} ^ {n} V o l B i d _ {i t} - \sum_ {i = 1} ^ {n} V o l A s k _ {i t}}{\sum_ {i = 1} ^ {n} V o l B i d _ {i t} + \sum_ {i = 1} ^ {n} V o l A s k _ {i t}}
$$


where $\begin{array} { r } { \sum _ { i = 1 } ^ { n } V o l B i d _ { t } \left( \sum _ { i = 1 } ^ { n } V o l A s k _ { t } \right) } \end{array}$ is the volume available at the top n bid (ask) price levels immediately before the order book event, t. q is an indicator variable equal to 1 for buys and -1 for sells. We estimate the model with limit order submission as the baseline category. Panels A to C present the results for HFT, Institutions and Retail, respectively. ***, ** and * indicate significance levels of 1%, 5% and 10%, respectively.


<table><tr><td></td><td>Aggressive Trade</td><td>Passive Trade</td><td>Amendment</td><td>Cancellation</td></tr><tr><td colspan="5">Panel A: HFT</td></tr><tr><td>Adjusted DI</td><td>8.062***(0.10)</td><td>2.435***(0.10)</td><td>-1.494***(0.10)</td><td>-3.757***(0.09)</td></tr><tr><td>Volatility</td><td>-9.492***(0.91)</td><td>-2.610***(0.85)</td><td>0.092(0.84)</td><td>3.607***(0.80)</td></tr><tr><td>Volume</td><td>0.225***(0.01)</td><td>0.042***(0.01)</td><td>0.069***(0.01)</td><td>-0.008(0.01)</td></tr><tr><td>Price</td><td>-0.293***(0.02)</td><td>-0.086***(0.02)</td><td>-0.030*(0.02)</td><td>0.106***(0.02)</td></tr><tr><td>Qspread</td><td>-18.047***(4.37)</td><td>-3.990(4.19)</td><td>4.127(4.38)</td><td>4.982(4.27)</td></tr><tr><td>Constant</td><td>-3.530***(0.18)</td><td>-0.605***(0.17)</td><td>-1.110***(0.17)</td><td>-0.049(0.16)</td></tr><tr><td>Obs.</td><td></td><td></td><td>109,351</td><td></td></tr><tr><td>Pseudo R-square</td><td></td><td></td><td>0.0496</td><td></td></tr><tr><td colspan="5">Panel B: Institutions</td></tr><tr><td>Adjusted DI</td><td>13.432***(0.22)</td><td>-10.111***(0.21)</td><td>0.681***(0.21)</td><td>3.897***(0.21)</td></tr><tr><td>Volatility</td><td>-0.816(0.85)</td><td>1.775**(0.81)</td><td>-0.069(0.83)</td><td>-0.334(0.83)</td></tr><tr><td>Volume</td><td>-0.006(0.01)</td><td>0.057***(0.01)</td><td>-0.002(0.01)</td><td>-0.010(0.01)</td></tr><tr><td>Price</td><td>0.071***(0.02)</td><td>-0.012(0.02)</td><td>0.002(0.02)</td><td>0.011(0.02)</td></tr><tr><td>Qspread</td><td>-17.359***(4.30)</td><td>-0.962(4.28)</td><td>-0.291(4.19)</td><td>-2.384(4.19)</td></tr><tr><td>Constant</td><td>0.053(0.17)</td><td>-1.093***(0.17)</td><td>0.039(0.16)</td><td>0.179(0.16)</td></tr><tr><td>Obs.</td><td></td><td></td><td>111,417</td><td></td></tr><tr><td>Pseudo R-square</td><td></td><td></td><td>0.0373</td><td></td></tr><tr><td></td><td colspan="4">Panel C: Retail</td></tr><tr><td>Adjusted DI</td><td>-0.502***(0.09)</td><td>-3.622***(0.09)</td><td>-1.320***(0.09)</td><td>-0.214**(0.09)</td></tr><tr><td>Volatility</td><td>-0.366(0.82)</td><td>1.144(0.82)</td><td>0.571(0.82)</td><td>0.399(0.82)</td></tr><tr><td>Volume</td><td>0.007(0.01)</td><td>0.005(0.01)</td><td>0.016(0.01)</td><td>0.008(0.01)</td></tr><tr><td>Price</td><td>0.015(0.02)</td><td>0.017(0.02)</td><td>0.008(0.02)</td><td>0.004(0.02)</td></tr><tr><td>Qspread</td><td>-1.798(4.16)</td><td>-2.801(4.22)</td><td>0.915(4.19)</td><td>0.513(4.17)</td></tr><tr><td>Constant</td><td>-0.092(0.16)</td><td>-0.071(0.16)</td><td>-0.302*(0.16)</td><td>-0.163(0.16)</td></tr><tr><td>Obs.</td><td></td><td></td><td>110,409</td><td></td></tr><tr><td>Pseudo R-square</td><td></td><td></td><td>0.0061</td><td></td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 6

R<sub>e</sub>l<sub>a</sub>ti<sub>on</sub> b<sub>e</sub>t<sub>ween</sub> A<sub>ggress</sub>i<sub>ve</sub> <sub>vo</sub>l<sub>ume</sub> % A<sub>ggress</sub>i<sub>ve</sub> t<sub>ra</sub>d<sub>e</sub> % <sub>an</sub>d <sub>s</sub>t<sub>oc</sub>k <sub>vo</sub>l<sub>a</sub>tilit<sub>y</sub> 

T<sub>a</sub>bl<sub>e</sub> 5 <sub>presen</sub>t<sub>s</sub> th<sub>e regress</sub>i<sub>on o</sub>f A<sub>ggress</sub>i<sub>ve vo</sub>l<sub>ume</sub> % <sub>or</sub> A<sub>ggress</sub>i<sub>ve</sub> t<sub>ra</sub>d<sub>e</sub> % <sub>aga</sub>i<sub>ns</sub>t <sub>vo</sub>l<sub>a</sub>tilit<sub>y</sub> Th<sub>e</sub> d<sub>epen</sub>d<sub>en</sub>t <sub>var</sub>i<sub>a</sub>bl<sub>e</sub> i<sub>s</sub> A<sub>ggress</sub>i<sub>ve vo</sub>l<sub>ume</sub> % <sub>w</sub>hi<sub>c</sub>h i<sub>s</sub> th<sub>e aggress</sub>i<sub>ve</sub> b<sub>uy</sub>i<sub>ng an</sub>d <sub>se</sub>lli<sub>ng vo</sub>l<sub>ume as a percen</sub>t<sub>age o</sub>f t<sub>o</sub>t<sub>a</sub>l <sub>aggress</sub>i<sub>ve an</sub>d <sub>pass</sub>i<sub>ve vo</sub>l<sub>ume</sub> f<sub>or eac</sub>h b<sub>ro</sub>k<sub>er</sub> t<sub>ype an</sub>d <sub>vo</sub>l<sub>a</sub>tilit<sub>y</sub> d<sub>ec</sub>il<sub>e .</sub> Th<sub>e resu</sub>lt<sub>s are</sub> b<sub>ase</sub>d <sub>on</sub> th<sub>e</sub> f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near regress</sub>i<sub>on w</sub>hi<sub>c</sub>h i<sub>s</sub> b<sub>ase</sub>d <sub>on</sub> 3 0-<sub>m</sub>i<sub>nu</sub>t<sub>e</sub> ti<sub>me</sub> i<sub>n</sub>t<sub>erva</sub>l<sub>s :</sub> 

%	݉݁ݑ݈݋ݒ	݁ݒ݅ݏݏ݁ݎ<sub>݃݃</sub>ܣ 

$$
\begin{array}{r l} & {= \beta_ {0} + \beta_ {1} I (H F T) \times I (L o w v o l a t i l i t y) + \beta_ {2} I (H F T) \times I (H i g h v o l a t i l i t y) + \beta_ {3} I (I n s t i t u t i o n s) \times I (L o w v o l a t i l i t y)} \\ & {+ \beta_ {4} I (I n s t i t u t i o n s) \times I (H i g h v o l a t i l i t y) + \beta_ {5} I (L o w v o l a t i l i t y) + \beta_ {6} I (H i g h v o l a t i l i t y) + \beta_ {7} I (H F T) + \beta_ {8} I (I n s t i t u t i o n s)} \\ & {+ \beta_ {9} V o l a t i l i t y + \beta_ {1 0} V o l u m e + \varepsilon} \end{array}
$$

F<sub>or eac</sub>h <sub>s</sub>t<sub>oc</sub>k <sub>we ran</sub>k th<sub>e</sub> 3 0 <sub>m</sub>i<sub>nu</sub>t<sub>e</sub> i<sub>n</sub>t<sub>erva</sub>l<sub>s</sub> i<sub>n</sub>t<sub>o vo</sub>l<sub>a</sub>tilit<sub>y</sub> d<sub>ec</sub>il<sub>es</sub> V<sub>o</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> hi<sub>g</sub>h<sub>es</sub>t b<sub>es</sub>t <sub>as</sub>k <sub>pr</sub>i<sub>ce an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> lowest best bid price during the 3 0 minute interval I(Low volatility) (I(High volatility)) is an indicator variable equal to 1 if the 3 0 minute interval is in the lowest (highest) decile based on stock volatilit<sub>y.</sub> I(HFT) and I(Institutions) are indicator variables equal to 1 for the trader t<sub>y</sub>pe specified in the parentheses and 0 otherwise <sub>.</sub> Volume is the natural log of the total daily share volume during the 3 0 minute interval<sub>.</sub> Large stocks (Small stocks) refer to stocks contained in the largest (smallest) tercile of all sample stocks based on market capitalization In Columns 4-6 we replace the dependent variable with Aggressive trade % which i<sub>s</sub> <sub>ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub>d b<sub>ase</sub>d <sub>on</sub> th<sub>e</sub> <sub>num</sub>b<sub>er</sub> <sub>ra</sub>th<sub>er</sub> th<sub>an</sub> th<sub>e</sub> <sub>vo</sub>l<sub>ume</sub> <sub>o</sub>f <sub>aggress</sub>i<sub>ve</sub> t<sub>ra</sub>d<sub>es .</sub> All <sub>regress</sub>i<sub>ons</sub> <sub>con</sub>t<sub>ro</sub>l f<sub>or</sub> <sub>s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s .</sub> W<sub>e</sub> <sub>repor</sub>t h<sub>e</sub>t<sub>eros</sub>k<sub>e</sub>d<sub>as</sub>ti<sub>c</sub>it<sub>y</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> i<sub>n paren</sub>th<sub>eses .</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d 1 0% res<sub>p</sub>ect<sup>i</sup>ve<sup>l</sup><sub>y.</sub> 

<table><tr><td rowspan="2"></td><td colspan="3">Aggressive volume %</td><td colspan="3">Aggressive trade %</td></tr><tr><td>(1)All stocks</td><td>(2)Large stocks</td><td>(3)Small stocks</td><td>(4)All stocks</td><td>(5)Large stocks</td><td>(6)Small stocks</td></tr><tr><td><eq>I(HFT) \times I(Low\ volatility)</eq></td><td>-4.058***(0.89)</td><td>-3.879***(1.38)</td><td>-4.376**(1.82)</td><td>-2.707***(0.96)</td><td>-4.521***(1.21)</td><td>-3.298*(1.84)</td></tr><tr><td><eq>I(HFT) \times I(High\ volatility)</eq></td><td>7.432***(0.62)</td><td>6.517***(0.91)</td><td>7.742***(1.58)</td><td>7.381***(0.87)</td><td>6.613***(1.19)</td><td>7.790***(1.94)</td></tr><tr><td><eq>I(Institutions) \times I(Low\ volatility)</eq></td><td>3.326***(0.81)</td><td>-0.763(0.83)</td><td>9.950***(1.54)</td><td>4.912***(0.78)</td><td>1.153(0.97)</td><td>8.360***(1.37)</td></tr><tr><td><eq>I(Institutions) \times I(High\ volatility)</eq></td><td>4.483***(0.52)</td><td>6.948***(0.51)</td><td>1.917(1.18)</td><td>2.223***(0.55)</td><td>5.015***(0.59)</td><td>-1.644*(0.87)</td></tr><tr><td><eq>I(Low\ volatility)</eq></td><td>-1.432**(0.60)</td><td>1.017(0.62)</td><td>-6.787***(1.17)</td><td>-2.378***(0.62)</td><td>0.363(0.65)</td><td>-5.427***(0.96)</td></tr><tr><td><eq>I(High\ volatility)</eq></td><td>-4.996***(0.37)</td><td>-6.205***(0.38)</td><td>-2.782***(0.92)</td><td>-3.254***(0.44)</td><td>-5.021***(0.57)</td><td>-0.493(0.72)</td></tr><tr><td><eq>I(HFT)</eq></td><td>13.677***(1.39)</td><td>10.162***(1.75)</td><td>14.839***(3.00)</td><td>16.521***(2.01)</td><td>13.366***(2.65)</td><td>16.784***(3.90)</td></tr><tr><td><eq>I(Institutions)</eq></td><td>-10.873***(0.72)</td><td>-12.163***(1.04)</td><td>-9.705***(1.65)</td><td>2.624**(1.15)</td><td>-5.138***(1.52)</td><td>10.603***(1.51)</td></tr><tr><td>Volatility</td><td>88.122***(20.72)</td><td>40.493(58.29)</td><td>53.509**(22.78)</td><td>131.281***(21.71)</td><td>111.875*(62.18)</td><td>116.592***(28.93)</td></tr><tr><td>Volume</td><td>-0.684***(0.08)</td><td>-0.880***(0.13)</td><td>-0.540***(0.15)</td><td>-0.615***(0.12)</td><td>-0.817***(0.18)</td><td>-0.265(0.20)</td></tr><tr><td>Constant</td><td>61.237***(1.23)</td><td>67.200***(2.54)</td><td>59.557***(2.11)</td><td>45.037***(1.76)</td><td>55.510***(2.96)</td><td>37.733***(2.18)</td></tr><tr><td>Obs.</td><td>449,556</td><td>175,152</td><td>118,303</td><td>449,556</td><td>175,152</td><td>118,303</td></tr><tr><td>Adj. R-square</td><td>0.241</td><td>0.239</td><td>0.207</td><td>0.200</td><td>0.245</td><td>0.162</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 7

Relation between Adjusted DI and stock volatility 

Table 5 presents the regression of Adjusted DI against volatility<sub>.</sub> The dependent variable is Adjusted DI<sub>,</sub> which is the average Adjusted DI for aggressive or passive trades during each 3 0 minute time interval as indicated in the table heading<sub>.</sub> For each trade Adjusted DI is calculated as : 

$$
A d j u s t e d D I _ {t} = q \times \frac {\sum_ {i = 1} ^ {5} V o l B i d _ {i t} - \sum_ {i = 1} ^ {5} V o l A s k _ {i t}}{\sum_ {i = 1} ^ {5} V o l B i d _ {i t} + \sum_ {i = 1} ^ {5} V o l A s k _ {i t}}
$$

<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { i = 1 } ^ { 5 } V o l B i d _ { t } \ ( \sum _ { i = 1 } ^ { 5 } V o l A s k _ { t } ) } \end{array}$ is the volume available at the top 5 bid (ask) price levels immediately before the trade t<sub>.</sub> The results are based on the f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near regress</sub>i<sub>on w</sub>hi<sub>c</sub>h i<sub>s</sub> b<sub>ase</sub>d <sub>on</sub> 3 0-<sub>m</sub>i<sub>nu</sub>t<sub>e</sub> ti<sub>me</sub> i<sub>n</sub>t<sub>erva</sub>l<sub>s :</sub> 

$$
\begin{array}{c} A d j u s t e d D I = \beta_ {0} + \beta_ {1} I (H F T) \times I (L o w v o l a t i l i t y) + \beta_ {2} I (H F T) \times I (H i g h v o l a t i l i t y) + \beta_ {3} I (I n s t i t u t i o n s) \times I (L o w v o l a t i l i t y) + \beta_ {4} I (I n s t i t u t i o n s) \\ \times I (H i g h v o l a t i l i t y) + \beta_ {5} I (L o w v o l a t i l i t y) + \beta_ {6} I (H i g h v o l a t i l i t y) + \beta_ {7} I (H F T) + \beta_ {8} I (I n s t i t u t i o n s) + \beta_ {9} V o l a t i l i t y + \beta_ {1 0} V o l u m e \\ + \varepsilon \end{array}
$$

F<sub>or eac</sub>h <sub>s</sub>t<sub>oc</sub>k <sub>we ran</sub>k th<sub>e</sub> 3 0 <sub>m</sub>i<sub>nu</sub>t<sub>e</sub> i<sub>n</sub>t<sub>erva</sub>l<sub>s</sub> i<sub>n</sub>t<sub>o vo</sub>l<sub>a</sub>tilit<sub>y</sub> d<sub>ec</sub>il<sub>es</sub> V<sub>o</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> hi<sub>g</sub>h<sub>es</sub>t b<sub>es</sub>t <sub>as</sub>k <sub>pr</sub>i<sub>ce an</sub>d th<sub>e</sub> l<sub>og o</sub>f th<sub>e</sub> lowest best bid price during the 3 0 minute interval I(Low volatility) (I(High volatility)) is an indicator variable equal to 1 if the 3 0 minute interval is in the lowest (highest) decile based on volatilit<sub>y</sub> I(HFT) and I(Institutions) are indicator variables equal to 1 for the trader t<sub>y</sub>pe specified in the parentheses and 0 otherwise Volume is the natural log of the total daily share volume during the 3 0 minute interval Large stocks (Small stocks) refer to stocks contained in the largest (smallest) tercile of all sample stocks based on market capitalization All regressions control for stock and day fixed effects We report heteroskedasticity-robust <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> i<sub>n paren</sub>th<sub>eses</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d $1 0 \% ,$ res<sub>p</sub>ect<sup>i</sup>ve<sup>l</sup><sub>y.</sub> 

<table><tr><td rowspan="2"></td><td colspan="3">Aggressive trades</td><td colspan="3">Passive trades</td></tr><tr><td>(1)All stocks</td><td>(2)Large stocks</td><td>(3)Small stocks</td><td>(4)All stocks</td><td>(5)Large stocks</td><td>(6)Small stocks</td></tr><tr><td><eq>I(HFT) \times I(Low\ volatility)</eq></td><td>-0.049***(0.00)</td><td>-0.035***(0.00)</td><td>-0.054***(0.01)</td><td>-0.055***(0.00)</td><td>-0.039***(0.00)</td><td>-0.064***(0.01)</td></tr><tr><td><eq>I(HFT) \times I(High\ volatility)</eq></td><td>0.065***(0.00)</td><td>0.064***(0.01)</td><td>0.074***(0.01)</td><td>0.080***(0.00)</td><td>0.068***(0.01)</td><td>0.092***(0.01)</td></tr><tr><td><eq>I(Institutions) \times I(Low\ volatility)</eq></td><td>-0.013***(0.00)</td><td>-0.006*(0.00)</td><td>-0.009(0.01)</td><td>-0.008**(0.00)</td><td>-0.008**(0.00)</td><td>-0.004(0.01)</td></tr><tr><td><eq>I(Institutions) \times I(High\ volatility)</eq></td><td>0.010***(0.00)</td><td>0.007**(0.00)</td><td>0.010**(0.00)</td><td>0.007***(0.00)</td><td>0.003(0.00)</td><td>0.005*(0.00)</td></tr><tr><td><eq>I(Low\ volatility)</eq></td><td>0.006*(0.00)</td><td>0.008**(0.00)</td><td>-0.000(0.01)</td><td>0.018***(0.00)</td><td>0.017***(0.00)</td><td>0.014(0.01)</td></tr><tr><td><eq>I(High\ volatility)</eq></td><td>-0.014***(0.00)</td><td>-0.017***(0.00)</td><td>-0.017***(0.00)</td><td>-0.024***(0.00)</td><td>-0.020***(0.00)</td><td>-0.026***(0.00)</td></tr><tr><td><eq>I(HFT)</eq></td><td>0.115***(0.00)</td><td>0.098***(0.01)</td><td>0.121***(0.01)</td><td>0.101***(0.01)</td><td>0.082***(0.01)</td><td>0.110***(0.01)</td></tr><tr><td><eq>I(Institutions)</eq></td><td>0.002(0.00)</td><td>0.007**(0.00)</td><td>0.003(0.01)</td><td>-0.022***(0.00)</td><td>-0.027***(0.00)</td><td>-0.019***(0.00)</td></tr><tr><td>Volatility</td><td>2.476***(0.27)</td><td>2.811***(0.51)</td><td>3.047***(0.40)</td><td>0.009(0.13)</td><td>0.097(0.14)</td><td>0.093(0.17)</td></tr><tr><td>Volume</td><td>-0.004***(0.00)</td><td>-0.003***(0.00)</td><td>-0.006***(0.00)</td><td>-0.002***(0.00)</td><td>-0.000(0.00)</td><td>-0.003***(0.00)</td></tr><tr><td>Constant</td><td>0.051***(0.01)</td><td>0.033***(0.01)</td><td>0.055***(0.02)</td><td>0.004(0.01)</td><td>-0.010(0.01)</td><td>0.043***(0.02)</td></tr><tr><td>Obs.</td><td>519904</td><td>189054</td><td>168110</td><td>519670</td><td>191623</td><td>174017</td></tr><tr><td>Adj. R-square</td><td>0.157</td><td>0.185</td><td>0.155</td><td>0.148</td><td>0.189</td><td>0.149</td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 8

R<sub>e</sub>l<sub>a</sub>ti<sub>on</sub> b<sub>e</sub>t<sub>ween</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> % <sub>an</sub>d DI b<sub>e</sub>f<sub>ore an</sub>d <sub>a</sub>ft<sub>er</sub> th<sub>e</sub> i<sub>mp</sub>l<sub>emen</sub>t<sub>a</sub>ti<sub>on o</sub>f ITCH 

T<sub>a</sub>bl<sub>e</sub> 7 <sub>repor</sub>t<sub>s</sub> th<sub>e regress</sub>i<sub>on o</sub>f V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> % <sub>or</sub> T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance</sub> % <sub>aga</sub>i<sub>ns</sub>t DI W<sub>e ana</sub>l<sub>yse</sub> t<sub>ra</sub>d<sub>e an</sub>d <sub>quo</sub>t<sub>e</sub> d<sub>a</sub>t<sub>a</sub> f<sub>or</sub> th<sub>e per</sub>i<sub>o</sub>d<sub>s</sub> M<sub>arc</sub>h 2 20 1 2 t<sub>o</sub> March 3 0 20 1 2 (pre-ITCH) and April 9 20 1 2 to May 9 20 1 2 (post-ITCH) Trades are sorted into deciles based on the size of the depth imbalance (DI) i<sub>mme</sub>di<sub>a</sub>t<sub>e</sub>l<sub>y</sub> b<sub>e</sub>f<sub>ore</sub> th<sub>e</sub> t<sub>ra</sub>d<sub>e .</sub> F<sub>or eac</sub>h DI d<sub>ec</sub>il<sub>e an</sub>d t<sub>ra</sub>d<sub>er</sub> t<sub>ype we ca</sub>l<sub>cu</sub>l<sub>a</sub>t<sub>e</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance as :</sub> 

$$
V o l u m e i m b a l a n c e _ {j} = \frac {\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} - \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}{\sum_ {j = 1} ^ {n} B u y V o l u m e _ {j} + \sum_ {i = 1} ^ {n} S e l l V o l u m e _ {j}}
$$

<sub>w</sub>h<sub>ere</sub> $\begin{array} { r } { \sum _ { j = 1 } ^ { n } B u y V o l u m e _ { j } ( \sum _ { j = 1 } ^ { n } S e l l V o l u m e _ { j } ) } \end{array}$ is the total aggressive buying (selling) volume for depth imbalance decile j<sub>.</sub> For columns $^ { 1 - 3 , }$ <sub>we</sub> <sub>es</sub>ti<sub>ma</sub>t<sub>e</sub> th<sub>e</sub> f<sub>o</sub>ll<sub>ow</sub>i<sub>ng</sub> li<sub>near</sub> <sub>regress</sub>i<sub>on</sub> <sub>w</sub>hi<sub>c</sub>h i<sub>s</sub> b<sub>ase</sub>d <sub>on</sub> DI d<sub>ec</sub>il<sub>es :</sub> 

$$
\begin{array}{l} V o l u m e i m b a l a n c e \% = \beta_ {0} \\ + I (P r e - I T C H) \times [ \beta_ {1} I (H F T) \times D I + \beta_ {2} I (I n s t i t u t i o n s) \times D I + \beta_ {3} D I ] \\ + I (P o s t - I T C H) \times [ \beta_ {4} I (H F T) \times D I + \beta_ {5} I (I n s t i t u t i o n s) \times D I + \beta_ {6} D I ] \\ + \beta_ {7} I (H F T) + \beta_ {8} I (I n s t i t u t i o n s) + \beta_ {9} V o l u m e + \varepsilon \end{array}
$$

I(Pre-ITCH) (I(Post-ITCH)) is an indicator variable equal to 1 if the trading da<sub>y</sub> falls in the pre-ITCH (post-ITCH) period and zero otherwise <sub>.</sub> I(HFT) and I(Institutions) are indicator variables equal to 1 for the trader t<sub>y</sub>pe specified in the parentheses and 0 otherwise Volume is the natural log of the total share volume traded in the decile For ease of comparison Column 1 reports the coefficients associated variables interacted with I(Pre-ITCH) and Column 2 presents the coefficients associated variables interacted with I(Post-ITCH) <sub>.</sub> We use a F-test to test for the equalit<sub>y</sub> of the coefficients interacted with DI<sub>.</sub> Column 3 presents th<sub>e</sub> F-t<sub>es</sub>t <sub>an</sub>d th<sub>e assoc</sub>i<sub>a</sub>t<sub>e</sub>d <sub>p</sub>-<sub>va</sub>l<sub>ue</sub> i<sub>n paren</sub>th<sub>eses</sub> I<sub>n</sub> C<sub>o</sub>l<sub>umns</sub> 4-6 <sub>we rep</sub>l<sub>ace</sub> th<sub>e</sub> d<sub>epen</sub>d<sub>en</sub>t <sub>var</sub>i<sub>a</sub>bl<sub>e w</sub>ith T<sub>ra</sub>d<sub>e</sub> i<sub>m</sub>b<sub>a</sub>l<sub>ance an</sub>d <sub>per</sub>f<sub>orm</sub> th<sub>e same ana</sub>l<sub>ys</sub>i<sub>s as</sub> th<sub>e prev</sub>i<sub>ous</sub> 3 <sub>co</sub>l<sub>umns .</sub> All <sub>regress</sub>i<sub>ons con</sub>t<sub>ro</sub>l f<sub>or s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> fi<sub>xe</sub>d <sub>e</sub>ff<sub>ec</sub>t<sub>s .</sub> W<sub>e repor</sub>t h<sub>e</sub>t<sub>eros</sub>k<sub>e</sub>d<sub>as</sub>ti<sub>c</sub>it<sub>y</sub>-<sub>ro</sub>b<sub>us</sub>t <sub>s</sub>t<sub>an</sub>d<sub>ar</sub>d <sub>errors</sub> d<sub>ou</sub>bl<sub>e c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> i<sub>n paren</sub>th<sub>eses .</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y.</sub> 

<table><tr><td rowspan="3"></td><td>(1)</td><td>(2)</td><td>(3)</td><td>(4)</td><td>(5)</td><td>(6)</td></tr><tr><td colspan="2">Volume imbalance %</td><td rowspan="2">F-Test</td><td colspan="2">Trade imbalance %</td><td rowspan="2">F-Test</td></tr><tr><td>Pre-ITCH</td><td>Post-ITCH</td><td>Pre-ITCH</td><td>Post-ITCH</td></tr><tr><td>I(HFT) × DI</td><td>0.942***(0.05)</td><td>1.064***(0.06)</td><td>5.350**(0.023)</td><td>0.938***(0.05)</td><td>1.066***(0.05)</td><td>7.71***(0.007)</td></tr><tr><td>I(Institutions) × DI</td><td>-0.030(0.04)</td><td>-0.038(0.04)</td><td>0.040(0.850)</td><td>0.017(0.04)</td><td>0.128***(0.04)</td><td>5.27**(0.024)</td></tr><tr><td>DI</td><td>-0.095**(0.05)</td><td>-0.118**(0.05)</td><td>0.480(0.490)</td><td>-0.028(0.04)</td><td>-0.121***(0.04)</td><td>6.36**(0.014)</td></tr><tr><td>I(HFT)</td><td></td><td>0.025(0.02)</td><td></td><td></td><td>0.026(0.02)</td><td></td></tr><tr><td>I(Institutions)</td><td></td><td>0.033**(0.02)</td><td></td><td></td><td>0.040**(0.02)</td><td></td></tr><tr><td>Volume</td><td></td><td>0.016***(0.00)</td><td></td><td></td><td>0.019***(0.01)</td><td></td></tr><tr><td>Constant</td><td></td><td>-0.373***(0.06)</td><td></td><td></td><td>-0.561***(0.07)</td><td></td></tr><tr><td>Obs.</td><td></td><td>80,666</td><td></td><td></td><td>80,666</td><td></td></tr><tr><td>Adj. R-square</td><td></td><td>0.186</td><td></td><td></td><td>0.278</td><td></td></tr></table>

## T<sub>a</sub>bl<sub>e</sub> 9

P<sub>ro</sub>b<sub>a</sub>bilit<sub>y</sub> <sub>o</sub>f li<sub>m</sub>it <sub>or</sub>d<sub>er</sub> <sub>execu</sub>ti<sub>ons</sub> b<sub>e</sub>f<sub>ore</sub> <sub>an</sub>d <sub>a</sub>ft<sub>er</sub> th<sub>e</sub> i<sub>mp</sub>l<sub>emen</sub>t<sub>a</sub>ti<sub>on</sub> <sub>o</sub>f ITCH 

T<sub>a</sub>bl<sub>e</sub> 8 <sub>ana</sub>l<sub>yzes</sub> th<sub>e proa</sub>b<sub>a</sub>bilit<sub>y o</sub>f li<sub>m</sub>it <sub>or</sub>d<sub>er execu</sub>ti<sub>ons</sub> f<sub>or</sub> HFT I<sub>ns</sub>tit<sub>u</sub>ti<sub>ons an</sub>d R<sub>e</sub>t<sub>a</sub>il b<sub>e</sub>f<sub>ore an</sub>d <sub>a</sub>ft<sub>er</sub> th<sub>e</sub> i<sub>mp</sub>l<sub>emen</sub>t<sub>a</sub>ti<sub>on o</sub>f ITCH W<sub>e ana</sub>l<sub>yse</sub> t<sub>ra</sub>d<sub>e</sub> and quote data for the periods March 2 20 1 2 to March 3 0 20 1 2 (pre-ITCH) and April 9 20 1 2 to May 9 20 1 2 (post-ITCH) The main dependent variable P(Fill) is calculated as 

$$
P (f i l l) = \frac {\sum T r a d e V o l u m e}{\sum S u b m i t V o l u m e}
$$

Where ∑ ܵݑܾ݉݅ݐܸ݋ ݈ݑ݉݁ is the total dail<sub>y</sub> volume submitted to the to<sub>p</sub> level of the limit order book and ∑ ܶݎܸܽ݀݁݋ ݈ݑ݉݁ is the total volume that is successfull<sub>y</sub> t<sub>ra</sub>d<sub>e</sub>d I<sub>n</sub> C<sub>o</sub>l<sub>umn</sub> 1 <sub>we es</sub>ti<sub>ma</sub>t<sub>e</sub> th<sub>e</sub> f<sub>o</sub>ll<sub>ow</sub>i<sub>ng regress</sub>i<sub>on</sub> 

ߝ൅݁ܽ݀ݎ<sub>݌</sub>ܵߚ൅݅ܿ݁ݎܲߚ൅݉݁ݑ݈݋ܸߚ൅<sub>ݕ</sub>ݐ݈݅݅ݐ݈ܽ݋ܸߚ൅ሻܪܥܶܫെݐݏ݋ܲሺܫߚ൅ሻܶܨܪെ݊݋ܰሺܫߚ൅ሻܪܥܶܫെݐݏ݋ܲሺܫൈሻܶܨܪെ݊݋ܰሺܫߚ൅ߚൌሻ݈݈݅ܨሺܲ where I(Non-HFT) is an indicator variable equal to 1 for Institutions and Retail and zero for HFT<sub>.</sub> I(Post-ITCH) is an indicator variable equal to 1 if the trading d<sub>ay</sub> f<sub>a</sub>ll<sub>s</sub> i<sub>n</sub> th<sub>e</sub> <sub>pos</sub>t-ITCH <sub>per</sub>i<sub>o</sub>d <sub>an</sub>d <sub>zero</sub> f<sub>or</sub> th<sub>e</sub> <sub>pre</sub>-ITCH <sub>per</sub>i<sub>o</sub>d<sub>.</sub> V<sub>o</sub>l<sub>a</sub>tilit<sub>y</sub> i<sub>s</sub> th<sub>e</sub> diff<sub>erence</sub> b<sub>e</sub>t<sub>ween</sub> th<sub>e</sub> l<sub>og</sub> <sub>o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> hi<sub>g</sub>h <sub>as</sub>k <sub>pr</sub>i<sub>ce</sub> <sub>an</sub>d th<sub>e</sub> l<sub>og</sub> <sub>o</sub>f th<sub>e</sub> i<sub>n</sub>t<sub>ra</sub>d<sub>ay</sub> l<sub>ow</sub> bid <sub>pr</sub>i<sub>ce</sub> V<sub>o</sub>l<sub>ume</sub> i<sub>s</sub> th<sub>e na</sub>t<sub>ura</sub>l l<sub>og o</sub>f th<sub>e</sub> t<sub>o</sub>t<sub>a</sub>l d<sub>a</sub>il<sub>y s</sub>h<sub>are vo</sub>l<sub>ume</sub> P<sub>r</sub>i<sub>ce</sub> i<sub>s</sub> th<sub>e average</sub> d<sub>a</sub>il<sub>y</sub> t<sub>ra</sub>d<sub>e pr</sub>i<sub>ce</sub> S<sub>prea</sub>d i<sub>s</sub> th<sub>e</sub> ti<sub>me we</sub>i<sub>g</sub>ht<sub>e</sub>d <sub>average</sub> difference between the best bid and offer prices <sub>.</sub> In Column 2 we replace I(Non-HFT) with I(Institutions) and I(Retail) which are indicator variables equal to 1 for the trader type specified in the parentheses and 0 otherwise<sub>.</sub> In Columns 3 and 4 (Columns 5 and 6) we replace the dependent variable with P(Favorable fill) (P( Unfavorable fill)) We define a favourable (unfavourable) fill as an order execution when the limit order rests on the side of the order book with more (less) depth immediately prior to the trade All regressions control for stock and day fixed effects We report heteroskedasticity-robust standard errors double <sub>c</sub>l<sub>us</sub>t<sub>ere</sub>d b<sub>y s</sub>t<sub>oc</sub>k <sub>an</sub>d d<sub>ay</sub> i<sub>n paren</sub>th<sub>eses</sub> <sup>* * * * *</sup> <sub>an</sub>d <sup>*</sup> i<sub>n</sub>di<sub>ca</sub>t<sub>e s</sub>i<sub>gn</sub>ifi<sub>cance</sub> l<sub>eve</sub>l<sub>s o</sub>f 1 % 5 % <sub>an</sub>d 1 0% <sub>respec</sub>ti<sub>ve</sub>l<sub>y</sub> 

<table><tr><td rowspan="2"></td><td colspan="2">P(Fill)</td><td colspan="2">P(Favorable fill)</td><td colspan="2">P(Unfavorable fill)</td></tr><tr><td>(1)</td><td>(2)</td><td>(3)</td><td>(4)</td><td>(4)</td><td>(5)</td></tr><tr><td>I(Non-HFT) × I(Post-ITCH)</td><td>-0.037***(0.01)</td><td></td><td>-0.040***(0.01)</td><td></td><td>-0.001(0.01)</td><td></td></tr><tr><td>I(Non-HFT)</td><td></td><td></td><td>-0.030*(0.02)</td><td></td><td>0.134***(0.01)</td><td></td></tr><tr><td>I(Institutions) × I(Post-ITCH)</td><td></td><td>-0.021**(0.01)</td><td></td><td>-0.029***(0.01)</td><td></td><td>0.008(0.00)</td></tr><tr><td>I(Institutions)</td><td></td><td>-0.069***(0.02)</td><td></td><td>-0.124***(0.02)</td><td></td><td>0.053***(0.01)</td></tr><tr><td>I(Retail) × I(Post-ITCH)</td><td></td><td>-0.057***(0.02)</td><td></td><td>-0.051***(0.01)</td><td></td><td>-0.009(0.01)</td></tr><tr><td>I(Retail)</td><td></td><td>0.301***(0.02)</td><td></td><td>0.078***(0.02)</td><td></td><td>0.226***(0.01)</td></tr><tr><td>I(Post-ITCH)</td><td>0.028*(0.02)</td><td>0.029*(0.02)</td><td>0.036**(0.02)</td><td>0.036**(0.02)</td><td>0.006(0.01)</td><td>0.008(0.01)</td></tr><tr><td>Volatility</td><td>0.087(0.17)</td><td>0.072(0.17)</td><td>0.054(0.16)</td><td>-0.090(0.16)</td><td>0.007(0.10)</td><td>-0.097(0.09)</td></tr><tr><td>Volume</td><td>0.071***(0.00)</td><td>0.069***(0.00)</td><td>0.039***(0.00)</td><td>0.036***(0.00)</td><td>0.028***(0.00)</td><td>0.026***(0.00)</td></tr><tr><td>Price</td><td>0.031(0.04)</td><td>0.033(0.04)</td><td>0.015(0.02)</td><td>0.009(0.02)</td><td>-0.006(0.01)</td><td>-0.014**(0.01)</td></tr><tr><td>Spread</td><td>-1.359(2.37)</td><td>-1.328(2.38)</td><td>-0.089(1.40)</td><td>-0.411(1.30)</td><td>-0.199(1.62)</td><td>-0.365(1.59)</td></tr><tr><td>Constant</td><td>-0.564***(0.08)</td><td>-0.534***(0.08)</td><td>-0.291***(0.06)</td><td>-0.231***(0.06)</td><td>-0.249***(0.04)</td><td>-0.205***(0.04)</td></tr><tr><td>Obs.</td><td>10646</td><td>10646</td><td>9718</td><td>9718</td><td>9574</td><td>9574</td></tr><tr><td>Adj. R-square</td><td>0.190</td><td>0.586</td><td>0.151</td><td>0.369</td><td>0.224</td><td>0.460</td></tr></table>