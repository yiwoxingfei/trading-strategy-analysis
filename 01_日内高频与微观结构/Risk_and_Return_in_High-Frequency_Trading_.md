

<!-- === Source: MinerU_markdown_Risk_and_Return_in_High-Frequency_Trading__1_2122706312759451666.md (Page 1) === -->

## Risk and Return in High-Frequency Trading

Matthew Baron, Cornell University 

Jonathan Brogaard, University of Washington 

Björn Hagströmer, Stockholm University 

Andrei Kirilenko, Imperial College London 

© 2017 by Baron et al. All rights reserved. Short sections of text, not to exceed two paragraphs, may be quoted without explicit permission provided that full credit, including © notice, is given to the source. 

# Risk and Return in High-Frequency Trading

Matthew Baron, Jonathan Brogaard, Björn Hagströmer and Andrei Kirilenko* 

## Abstract

We study performance and competition among high-frequency traders (HFTs). We construct measures of latency and find that differences in relative latency account for large differences in HFTs’ trading performance. HFTs that improve their latency rank due to colocation upgrades see improved trading performance. The stronger performance associated with speed comes through both the short-lived information channel and the risk management channel, and speed is useful for a variety of strategies including market making and cross-market arbitrage. We explore implications resulting from competition on relative latency and find support for various theoretical predictions. 

Traditional models of market making argue that competition among market intermediaries should decrease their profits and lead to lower trading costs for other investors (Ho and Stoll, 1983; Weston 2000). Several models of high-frequency trading (HFT) adopt this standard view.<sup>1</sup> Other theories offer a contrasting perspective, that competition based on relative (i.e., rank-order) latency makes the HFT industry different and leads to a distinct competitive environment. For example, Foucault, Kozhan and Tham (2015) and Foucault, Hombert and Roşu (2016) show how competition based on relative latency can reduce market quality by increasing adverse selection of non-HFT firms. Biais, Foucault and Moinas (2015) and Budish, Cramton and Shim. (2015) show in theory how it can lead to market concentration and inefficient overinvestment in speed. In these models, the fastest HFT firm responds first to profitable trading opportunities, capturing all the gains, while slower participants arrive marginally too late to trading opportunities to compete. As a result, small differences in trading speed are associated with large differences in trading revenues across firms. HFT revenues do not fall over time: regardless of how fast the market as a whole becomes, there is always at least one HFT firm with a relative speed advantage that can adversely select other traders. 

Motivated by the view that competition based on relative latency differs from competition of traditional market intermediaries, this paper tests whether relative latency can explain cross-sectional differences in HFT performance. To our knowledge, we are the first to present direct evidence that small differences in trading speed are associated with large differences in trading revenues. 

While HFTs benefit from the use of microwave transmission technologies (Shkilko and Sokolov, 2016) and colocation services (Brogaard, Hagströmer, Nordén and Riordan, 2015), it is unclear to what extent speed matters for trading performance and through which channels. For example, Brogaard et al. (2015) finds that not all HFTs choose faster colocation technology when offered, and we similarly find only about half of HFTs react to market events at time scales near the latency frontier. This suggests that many HFTs use computational power for other reasons, perhaps to better aggregate information from news feeds or order flow, and may not compete to be fastest. Despite these alternative possibilities, we find that the HFTs who are the fastest have better trading performance. We also find evidence supporting the importance of relative latency for trading performance and explore some of the predictions regarding market concentration. 

The theoretical literature has put forward a variety of channels through which HFTs may translate speed into profitability. For example, HFTs can use speed to enhance risk management, by avoiding adverse selection (Jovanovic and Menkveld, 2015) and improving inventory management (Aït-Sahalia and Saglam, 2014), or to trade on short-lived information (Foucault et al., 2016). We find evidence that firms with lower relative latency are better along both of these dimensions. The fastest firms earn a higher realized spread when trading passively, consistent with better risk management. They also have the highest price impact when trading with market orders, suggesting they are able to be the first to react to new information. Looking at crossmarket arbitrage, we also observe the fastest firms being more responsive to information on other exchanges. Thus, there is no one single dimension through which speed is beneficial. 

Our analysis uses proprietary transaction-level data with trader identifiers provided by the Swedish financial supervisory authority, Finansinspektionen. The data contain all trades of Swedish equities from January 2010 to December 2014 from all venues including regulated exchanges, multilateral trading facilities (MTFs), and dark pools. Given the high degree of fragmentation of volume in European equity trading, this cross-market coverage is an important feature to get the whole picture of trading. In addition, the five-year length of our data is important in allowing us to trace the “long-term” evolution of the HFT industry, at least relative to the rapid pace of innovation in the industry. 

We focus on the 25 largest Swedish stocks by market capitalization, as Hagströmer and Nordén (2013) show that HFT activity is mainly concentrated in these stocks. We classify highfrequency traders as those firms that self-describe as such through their membership in the European Principal Traders Association (FIA-EPTA; a lobby organization for principal trading firms formed in June 2011) and any other firm that, according to its own website, undertakes low-latency proprietary trading.<sup>2</sup> The 16 firms that we identify as HFTs all have international trading operations and none of them are headquartered in Sweden. Thus, it is unlikely that the findings reported in this paper are specific to the Swedish context.<sup>3</sup> 

We test the connection between HFT latency and trading performance. The main trading performance measure is Revenues, captured daily for each HFT firm as the net of purchases and sales, marking end-of-day positions to market.<sup>4</sup> We also include risk-adjusted performance measures, including returns, factor model alphas, and Sharpe ratios. We find that HFTs exhibit large, persistent cross-sectional differences in performance, with trading revenues disproportionally accumulating to a few firms. The results are robust to accounting for estimated exchange fees and liquidity rebates, which negligibly change the results. 

Our main measure of latency is the difference in time stamps from a passive trade to a subsequent aggressive trade by the same firm, in the same stock and at the same trading venue. This measure, which we call Decision Latency, aims to capture the reaction time involved in a deliberate decision to trade in reaction to a market event (its limit order being hit), which the HFT firm may view as informative. Specifically, for each HFT firm, we record the empirical latency distribution of all events where a passive trade is followed by an active trade by the same HFT firm in the same stock and at the same venue within one second. To capture the fastest possible reaction time for each HFT firm while also being robust to potential outliers, we use the 0.1% quantile of that distribution as the latency for each HFT firm.<sup>5</sup> As an example of a strategy our measure may capture, Clark-Joseph (2012) shows that HFTs use the execution of small test orders as a signal to trade on incoming order flow ahead of public order book feeds. Over our five-year sample period we show that the latency of the fastest HFTs falls substantially. 

We find that relative latency, not nominal latency, drives differences in performance across HFTs. Relative latency measures how fast a HFT firm is relative to other HFTs and is captured by ranking HFTs by their calculated latency measure. Nominal latency measures how fast a HFT firm is in absolute terms and is captured by the log of a HFT firm’s calculated Decision Latency. Our evidence is consistent with Biais et al. (2015) and Budish et al. (2015), who argue that competition on relative latency can lead to an inefficient and costly arms race. The discontinuous difference in payoffs provides strong incentives to become marginally faster than other HFTs through greater technological investment. Such competition on relative latency gives rise to a “positional externality” (Frank, 2005), since a firm that becomes faster increases the relative latency of its competitors, which can in turn lead to an inefficient over-investment in speed. 

We find that firms that are among the five fastest HFTs, and in particular the fastest single HFT firm, earn substantially higher revenues than other HFTs. It is not being fast that allows an HFT firm to capture trading opportunities, it is being faster than others, consistent with Biais et al. (2015) and Budish et al. (2015). Furthermore, we find that the fastest HFTs capture more trading opportunities and have higher risk-adjusted revenues, but they do not earn higher revenue margins per SEK traded. The differential finding suggests that on a per-trade basis, the fastest HFTs are no more accurate than other traders at processing and analyzing information (trade quality), but their latency advantage allows them to capture more trading opportunities (trade quantity) without taking on higher risk.<sup>6</sup> 

As a robustness check, we construct various alternative approaches to measuring HFT latency. For example, Queuing Latency, captures the race to be at the top of the order book, as motivated, for example, by theoretical work by Yueshen (2014) and empirical findings by Yao and Ye (2015). Specifically, following price changes that lead to an empty price level in the limit order book, we count how often a given HFT firm submits the first limit order and thus gets to the top of the queue. Importantly, Queuing Latency does not rely on time stamps, making it robust to potential time stamp noise, and it is potentially better at capturing latency of HFTs that do not use market orders. Nevertheless, we find qualitatively similar results as with our primary latency measure. 

To address possible endogeneity concerns, we present causal evidence from a quasiexperimental setting, studying two colocation upgrades on the NASDAQ OMX Stockholm exchange: the “Premium Colocation” upgrade first offered on March 14, 2011 and the “10G Colocation” upgrade first offered on September 17, 2012. These colocation upgrades lead some, but not all, HFTs to get faster.<sup>7</sup> We compare the change in trading performance for HFTs that become relatively faster to those that become relatively slower. We show, as before, that increases in relative speed lead to better trading performance. 

We then investigate through which channels relative latency benefits traders. Some theories view fast traders as using speed to trade on short-lived information, whether in reaction to news, order flow, or latency arbitrage (Cartea and Penalva 2012; Foucault et al., 2015; Foucault et al., 2016; Biais et al., 2015; and Roşu 2015). Other theories view speed as a way to avoid adverse selection and inventory costs (Jovanovic and Menkveld, 2015; Aït-Sahalia and Saglam, 2014; Hoffmann, 2014). Menkveld and Zoican (2015) posit that both these types can coexist in equilibrium. 

We examine the role of relative latency in both channels, both in the general setting as well as in a specific cross-market strategy. We proxy the short-lived information channel by the ability of a market order to predict price changes over the next 10 seconds, and the risk management channel by the ability of a passive order to capture a large realized spread. Relative latency is associated with better performance through both channels. As a specific strategy, we study cross-market arbitrage by examining HFTs’ equity trading following changes in the price of index futures. In the second after a change in the index futures price, the fastest HFTs are more likely than other HFTs to aggressively trade in individual equities in the direction of the futures price change. The fastest HFTs are also less likely to supply liquidity to equities trades in the direction of the futures price change, which is consistent with avoiding adverse selection. We thus conclude that relative latency is important for performance both in short-lived information trading and in risk management. 

Finally, we explore predictions regarding the effects of relative latency on market concentration. If the traditional view of market-making competition holds (Ho and Stoll, 1983; Weston 2000), we expect the alpha generated by HFTs and the concentration of revenues to disappear as the industry matures. Alternatively, if HFTs compete on relative latency, we do not expect increased competition to drive profit opportunities to zero. As argued by Budish et al. (2015), regardless of how fast the market as a whole becomes, there is always at least one firm with a relative speed advantage that can adversely select other traders. Additionally, rents remain concentrated among the fastest HFTs, as slower HFTs arrive marginally too late to trading opportunities to compete. 

Consistent with the predictions of the effects of competition on relative latency, we find that the HFT industry is concentrated among a few firms. In contrast to the traditional view that increased competition over time leads to lower profits, HFT concentration of trading revenues and trading volumes are high and non-declining over the five year sample, despite new HFT firm entry and a decline in overall HFT latency. We furthermore find that new HFT entrants are typically slower, earn lower trading revenues, and are more likely to exit, which likely reinforces concentration in the HFT industry.<sup>8</sup> 

## II. Data and Methodology

## A. Data

Our primary data source is the Transaction Reporting System (TRS), a proprietary data set provided to us by Finansinspektionen, the Swedish financial supervisory authority. According to the Markets in Financial Instruments Directive (MiFID), financial institutions in the European Union that are under the supervision of one of the national financial supervisory authorities must report all their transactions with financial instruments to TRS. 

The TRS data has two features that make it highly suitable for the analysis of revenues in equity trading. First, the scope of the reporting obligation spans transaction at all trading venues, including regulated exchanges, MTFs, and dark pools. This is important given the high degree of fragmentation of volume in European equity trading. Second, TRS contains identifiers (name, business identifier code, and address) for both the trading entity reporting the transaction and its counterparty. If the reporting entity undertakes the transaction as a broker for another financial institution, the identifiers for the client institution are reported too. The trader identifiers are necessary to identify HFTs and to analyze revenues in the cross-section of firms. Finally, the TRS data contains standard transaction-level variables such as date, time, venue, price, currency, quantity, and a buy/sell indicator. See Appendix Section A1 for information about the filtering procedures applied to the TRS data.<sup>9</sup> 

We restrict the sample to the constituents of the leading Swedish equity index, the OMX S30 in order to focus on the most liquid stocks where HFTs primarily operate (Hagströmer and Nordén, 2013). We exclude six stocks that are cross-listed in other currencies, because revenue calculations for such stocks would require transaction data for foreign exchange markets.<sup>10</sup> There is one index constituent change during the sample period. We include Kinnevik Investment AB (KINVb) after its inclusion in the index on July 1, 2014, and we include Scania AB (SCVb) up until May 16, 2014, when it ceased trading. The final sample has 25 stocks covering the period January 4, 2010 to December 30, 2014. 

We match the TRS transactions to transaction-level data available from the Thomson Reuters Tick History (TRTH) database. The TRTH database is accessed through the Securities Research Centre of Asia-Pacific (SIRCA). The purpose of the matching is twofold. First, whereas the TRS data has second-by-second time stamps, TRTH has time stamps at a microsecond granularity. Through the matching we can assign microsecond time stamps to the TRS data, which is important for our latency measurement. Second, TRTH also contains order book information recorded on a microsecond frequency synchronized to the transaction data. This enables us to assess the status of the order book just before each TRS transaction, which is necessary to measure, for instance, the effective spread and to determine whether the trade was initiated by the buyer or the seller, following Lee and Ready (1991).<sup>11</sup> 

## B. Trading Venues and Stock Characteristics

All the sample stocks have their primary listing at NASDAQ OMX Stockholm, which is open for continuous electronic limit order book trading from 9:00 am to 5:25 pm on weekdays. 

For details about the trading mechanism at NASDAQ OMX Stockholm, see Hagströmer and Nordén (2013). Other important trading venues by trading volume in our data are Chi-X, BATS, Turquoise (all based around London) and Burgundy (based in Stockholm). In February 2011, BATS and Chi-X merged at the corporate level, but they maintain separate trading venues throughout our sample period. Burgundy was acquired by Oslo Börs in 2012. All sample stocks are subject to mandatory central counterparty clearing. 

Table 1 reports descriptive statistics for the sample stocks. Market Capitalization at closing prices on December 31, 2014 ranges from 13,877 million SEK (henceforth MSEK) for SSABa to 475,595 MSEK for HMb, the equivalent of 1.78 to 60.91 billion USD, converted at the exchange rate of December 31, 2014. In the U.S. equities market, these stocks would be labeled as large or mid-cap stocks. 

## INSERT TABLE 1 ABOUT HERE

Daily Trading Volume refers to trading at NASDAQ OMX Stockholm only and is reported in MSEK. Daily Turnover is the Daily Trading Volume divided by Market Capitalization, expressed in percentage points. Tick Size is the average minimum price change. Quoted Spread is the average bid-ask spread prevailing just before each trade; and Effective Spread is the trade value-weighted average absolute difference between the trade price and the bid-ask midpoint. All spread measures are based on continuous trading at NASDAQ OMX Stockholm, expressed relative to the bid-ask spread midpoint, and presented in basis points. The Tick Size and the Quoted Spread are halved to be comparable to the Effective Spread. The Daily Turnover across stocks is 0.60% and the Quoted Spread and Effective Spread vary between 2 and 6 bps. The more liquid stocks in our sample have a turnover and spread similar to the US largecap stocks studied by Brogaard, Hendershott, and Riordan (2014). The Tick Size for many stocks is close to the Quoted Spread, indicating that market tightness is frequently bounded by the tick size. 

Finally, we report Volatility, the average 10-second squared basis point returns, calculated from bid-ask midpoints; and an index for the degree of volume fragmentation. The Fragmentation Index is defined as the inverse of a Herfindahl index of trading volumes across the five largest trading venues (BATS, Burgundy, Chi-X, NASDAQ OMX Stockholm, and Turquoise). The procedure implies that fragmentation is measured on a scale from one to the number of trading venues considered, which in our case is five.<sup>12</sup> Volatility ranges from 3 to 17 squared basis points, and the Fragmentation Index varies across stocks between 1.76 and 2.32. 

## C. HFT Identification

Previous studies classify HFTs according to observed trading behavior (as in Kirilenko, Kyle, Samadi and Tuzun, 2015) or using an exchange-defined classification (Brogaard et al., 2014). We define HFTs as those who self-describe as HFTs by including firms that are members of the FIA-EPTA or that according to their own website primarily undertake low-latency proprietary trading. The advantage of this approach over a classification based on observed trading behavior is that we can verify that HFTs have the characteristics usually associated with them: high trading volume, short investment horizons, and tight inventory management (Securities and Exchange Commission, 2010). 

To include an HFT firm, we also require it to trade at least 10 MSEK a day, about 1.05 million USD at the exchange rate on December 31, 2014, for at least 50 trading days of the 1,255 trading days in the sample. We find 25 firms who self-describe as HFTs, 16 of which satisfy the volume criteria and form our sample of HFTs. The firm-day requirement of 10 MSEK is imposed to avoid outliers in trading performance that can appear due to small volumes. The nine firms that self-describe as HFTs, but that do not satisfy the volume criteria together represent only 0.13% of the total HFT trading volume, and 0.85% of the firm-day observations.<sup>13</sup> 

## D. HFT Performance Measures

We study three dimensions of performance: quantity measures, risk-adjusted measures, and quality measures. The quantity performance dimension measures the ability to capture trading opportunities that are ex-ante expected to be profitable to the HFT firm, such as shortlived arbitrage events and the supply of liquidity to uninformed investors. The risk-adjusted performance dimension measures the ability to capture revenue while avoiding risky trades. The quality performance dimension measures the ability to capture revenues relative to trading volume. 

We capture quantity performance using Revenues and Trading Volume. Revenues is defined as the cumulative cash received from selling shares, minus the cash paid from buying shares, plus the value of any outstanding end-of-day inventory positions marked to the market price at close. We calculate Revenues for each HFT firm, each sample stock, and each trading day. Depending on the application we report Revenues for different frequencies of time, for individual HFT firms as well as across all firms in the industry, and for individual stocks or all stocks; however, all versions of Revenues are aggregates of the same panel of firm-stock-day observations. Trading Volume is the SEK volume traded, measured at the same frequency as Revenues. 

We assume zero beginning-of-day inventory positions as a way to overcome potential data errors. Even minor errors in inventory can accumulate over time, leading to large and persistent (unit root) errors if left uncorrected. Therefore, we zero beginning-of-day inventories so that any potential errors do not affect more than one day. This assumption is relatively innocuous because we show below that most HFTs usually end the day near a zero position anyway (see Table 2). In the Appendix Section A3, we compare our main method of calculating trading revenues with three alternative approaches, one of which relaxes the assumption of zero inventory at the start of the trading day and cumulates daily net inventory positions over the full sample. We conclude that alternative definitions of Revenues yield similar results. 

To capture risk-adjusted performance we measure Returns, factor model Alphas (one, three, or four factors), and the Sharpe Ratio. Through the use of risk-adjusted performance measures, we assess whether HFTs with higher revenues are simply taking on more risk. The view that fast traders can achieve high risk-adjusted performance is supported by both theoretical models and real-world evidence. Ait-Sahalia and Saglam (2014) show that fast market-makers are better at handle inventory risk, and Hoffman (2014) shows that fast traders are able to avoid adverse selection risk. In its IPO prospectus, Virtu, an HFT firm in our sample, states: “we had only one losing trading day during … a total of 1,238 trading days.” <sup>14</sup> 

Returns are calculated by dividing Revenues of each firm by the implied capitalization of the firm. The implied capitalization is calculated for each HFT firm as the maximum position in SEK that a firm’s portfolio takes over the five-year sample. HFTs’ inventories generally exhibit sharp, well-defined maximum and minimum total portfolio positions. We use the observed maximum position as an approximation of the maximum amount of capital that an HFT firm would need to execute its specific strategy in Swedish equities markets.<sup>15</sup> Returns can thus be viewed as the performance achieved relative the capital allocated to the trading operation. Returns are calculated at daily frequencies but throughout the paper are reported annualized. 

Factor model Alphas are computed for each HFT firm over the entire sample using the standard Fama-French model (Fama and French, 1993) and the Carhart (1997) momentum factor. The Fama-French and Carhart daily factors are constructed for Swedish equities according to the methodology from Fama and French (1993) and Ken French’s website, using the full sample of Swedish stocks traded on NASDAQ OMX Stockholm. Methodological details concerning the construction of these factors and validation exercises can be found in the Appendix Section A4. 

The annualized Sharpe Ratio for each HFT firm is calculated using daily observations as $\frac { \mu _ { i } - r _ { f } } { \sigma _ { i } } * \sqrt { 2 5 2 }$ , where $\mu _ { i }$ is the average daily return, $r _ { f }$ is the risk-free rate, and $\sigma _ { i }$ is the standard deviation of HFT firm i’s returns. Whereas Returns and factor model Alphas rely on the assumption that market capitalization can be proxied by the maximum inventory position of the trading firm, the Sharpe Ratio does not. To see this, note that if the risk-free rate can be neglected as it is nearly zero for much of the sample period, the Sharpe Ratio is equivalent to: $\frac { \mu ( R e v e n u e s ) _ { i } } { \sigma ( R e v e n u e s ) _ { i } } * \sqrt { 2 5 2 }$ . The equity capitalization is therefore irrelevant for calculating the Sharpe Ratio. 

We capture quality performance with the Revenues per MSEK Traded measure. The quality dimension of performance measures the ability to enter trades with a high revenue margin. Revenues per MSEK Traded is calculated daily as Revenues divided by Trading Volume. 

The performance measures do not account for trading fees and liquidity rebates. We show in Section III.C that an adjustment for estimated exchange fees and liquidity rebates does not change the conclusions of the paper. 

## E. HFT Latency

Generally, latency is the delay between a signal and a response, measured in units of time. Following Weller (2013), we define the signal as a passive execution for the HFT firm in question, and the response as a subsequent aggressive execution by the same firm. Examples of why HFTs would attempt to trade aggressively immediately after a passive execution include test orders described by Clark-Joseph (2012) and “scratch” trades described by Kirilenko et al. (2015). The HFT firm cannot control the timing of the passive trade but can only react to it. Our latency measure thus captures reactions to incoming order flow, not how fast an HFT firm can execute two successive trades. 

Specifically, for each firm in each month, we record all cases where a passive trade is followed by an aggressive trade by the same firm, in the same stock and at the same trading venue, within one second. The time-stamp difference between the two trades in each case forms an empirical distribution of response times. To capture the fastest possible reaction time, while also being robust to potential outliers, we define Decision Latency as the 0.1% quantile of the aforementioned distribution. <sup>16,</sup> <sup>17</sup> 

Decision Latency captures the following sequence of events. The starting point is when an HFT firm’s resting limit order is executed by an incoming market order. The matching engine processes and time stamps the trade. A confirmation message is then sent to the HFT firm. The firm processes the confirmation information and makes a decision on how to react, which may be in the form of an aggressive order. The end of the latency measure is marked by the time stamp assigned when the message for the market order is processed by the matching engine. 

By excluding cases where the two trades are recorded at different trading venues we avoid potential problems related to that time-stamps are not perfectly synchronized across venues. Additionally, we can test whether within-market Decision Latency also explains success at arbitrage across markets (see Section V). 

There are numerous signals that may trigger HFTs to react swiftly, including news events, order book gaps, and block orders. The inherent problem of signal-to-response latency measures is that HFTs employ different strategies and put different weights to different signals. We argue that it is likely that HFTs respond to signals affecting their own portfolio such as a passive execution. Our measure of Decision Latency, while not perfect, captures an important dimension of latency that varies across market participants. While we conjecture that the passive trade is the information triggering the subsequent aggressive trade, this cannot be confirmed. 

Also, the measure is less informative for HFTs that do not tend to follow passive executions with immediate aggressive executions.<sup>18</sup> However, these limitations should result in underestimating, not exacerbating, the role of speed in performance. Furthermore, in Section IV.C we show that our results are robust to two alternative measures of latency, Queuing Latency and Mean Latency. 

Figure 1 plots Decision Latency over the sample period 2010-2014. HFTs are grouped by their relative rank of latency per month; the categories are Top 1, Top 1-5, and all HFTs. Over the sample period latency decreases for HFTs in the top 5: for example, the latency of the Top 1 HFTs decreases from around 62 microseconds in 2010 to around 10 microseconds in 2014. The relative reduction in latency is much greater for Top 1-5 HFTs, who start out in 2010 with latencies of over 1,280 microseconds and converge in latency to the Top 1 HFT by 2014. In contrast, All HFTs, which disproportionately picks up the slower HFTs, remains relatively constant with an average latency of 25 milliseconds over the entire sample period. The finding that HFTs outside the Top 5 do not achieve lower latencies over time is consistent with the finding of Brogaard et al. (2015) that not all HFTs choose to be the fastest when given the opportunity to choose a faster colocation technology. 

## INSERT FIGURE 1 ABOUT HERE

The magnitude of latency recorded for the fastest HFTs in this paper is consistent with statements about the INET trading system used at NASDAQ OMX Stockholm. In marketing materials from 2012, NASDAQ states that their trading system delivers “sub-40 microsecond latency.”<sup>19</sup> At that time, our fastest measured latency is around 60 microseconds.<sup>20</sup> 

Figure 1 marks various technological upgrades: the introduction of INET in early 2010, a high-capacity trading system capable of handling over 1 million messages per second, and two colocation upgrades at NASDAQ OMX Stockholm in March 2011 and September 2012. The fact that Decision Latency decreases following the technology upgrades provide suggestive evidence that our latency measure indeed captures reaction time. While it is difficult to assess the impact of the 2010 INET upgrade since it comes at the start of the sample, the colocation upgrade of 2012 is followed by a decline in latency for the top 5 HFTs. The fact that latency falls subsequent to colocation upgrades is a valuable validation of our measure. In Section IV, we use the 2011 and 2012 colocation upgrades to provide evidence on a causal relation between relative latency and trading performance. 

## III. Characterizing HFT Performance

## A. HFT Performance in the Cross-Section

We document the risk and return characteristics of individual HFT firms. In Table 2 we report the cross-sectional distribution of HFT performance, latency, and other trading characteristics. For each variable, we retrieve the time-series average for each HFT firm, and then report the distributional statistics across firms. 

## INSERT TABLE 2 ABOUT HERE

The median HFT firm realizes an average daily Revenues of 6,990 SEK, or 56.5 SEK Revenues per MSEK Traded. It has a daily Trading Volume of 64 MSEK, an annualized Sharpe Ratio of 1.61, and a four-factor (Fama-French plus Carhart momentum) annualized Alpha of 9%. The Returns are also 9%, suggesting that exposure to well-documented risk factors is not particularly relevant for HFT firms.<sup>21</sup> 

We find considerable performance variation in the cross-section of HFTs. The crosssectional distributions are skewed towards a few high performers. For example, firms in the top 90<sup>th</sup> percentile generate Revenues of 61,354 SEK per day, compared with 6,990 for the median; a Sharpe Ratio of 11.1, compared with 1.61 at the median; Revenues per MSEK Traded of 472.2, compared with 56.5 at the median; and a four-factor annualized Alpha of 89%, compared with 9% at the median. 

HFTs are diverse in terms of other trading characteristics, too. Beyond performance, we report the distributions of End-of-Day Inventory Ratio (the end-of-day inventory divided by Trading Volume); Max. Intraday Inventory Ratio (the maximum intraday portfolio position divided by Trading Volume); Investment Horizon (the median holding time in seconds across all trades, calculated on a first-in-first-out basis); Aggressiveness Ratio (the market order volume in SEK divided by Trading Volume); and Decision Latency (in microseconds). Consistent with the characterization of HFTs in the Securities and Exchange Commission’s Concept Release on Equity Market Structure (2010) and with functional-based approaches for HFT classification (Kirilenko et al., 2015), most, though not all, HFTs tend to have low intraday and end-of-day inventories. HFTs vary in their Aggressiveness Ratio, with some nearly all active or passive and others mixed. The average aggressive ratio is 53%. Consistent with Figure 1 and the discussion above, there is also substantial variation in Decision Latency across HFTs, from 42 microsecond latency at the 10<sup>th</sup> percentile to 0.5 second latency at the $9 0 ^ { \mathrm { t h } }$ percentile, a finding we explore in Section IV. Notably, the 0.5 second latency for some HFTs to process information and react with a market order is slow for automated traders but still fast relative to human reaction time. 

## B. Comparison of Trading Revenues to Trading Profits Based on Public Filings

The data do not convey trading fees or other operational costs and so we are unable to directly calculate trading profits. However, regulatory filings of five major HFT firms (Virtu, 2011-2015; Knight Capital Group, 2013-2015; GETCO, 2009-2012; Flow Traders, 2012-2015; and Jump, 2010) allow a comparison of trading revenues and trading profits. A potential concern in our analysis of HFT performance is that firms with higher trading revenues may have higher fixed costs. That is, firms with higher trading revenue may also incur higher costs to produce better performance. If true, then trading revenues may not be a good proxy for firm profitability. We show that this is not likely the case. 

Table 3 reports trading revenue, trading costs, trading profit margins, and trading returns calculated from annual reports, IPO prospectuses, and SEC disclosures for five HFT firms for which public data is available.<sup>22</sup> Trading costs are broken down into several categories such as trading and clearing fees, data costs, financing costs, equipment and technical costs, all expressed as a percent of trading revenues. Trading costs also include depreciation and amortization. This serves as a control for investments that a firm may have undertaken in years preceding the public data coverage. 

## INSERT TABLE 3 ABOUT HERE

We make two observations. First, trading profit margins are high, ranging between 27.4% and 64.5% of trading revenue for all four firms. Approximately 40-80% of the HFT costs are per-trade fees: brokerage fees, exchange and clearance fees, and financing costs. The fixed (i.e. not per-trade) costs, including communications and data processing, equipment, administrative and technology costs, make up only 15-30% of the total costs. As a result, we conclude that fixed costs, which include costs related to technological investment and colocation services, are small relative to trading revenues, making it unlikely that firms with the highest trading revenues face higher investments costs that would substantially reduce their net profits. 

Second, as a percentage of trading revenues, the fixed costs do not vary substantially across firms, suggesting that revenues are not correlated with fixed costs in percentage terms. For example, in 2014, KCG had double the trading revenue of Virtu and five times the trading revenue of Flow Traders, but the total fixed costs as a percentage of trading revenue show no pattern (22.7% for KCG; 17.7% for Virtu; 27.2% for Flow Traders). There is also no clear time trend in fixed costs within each firm to suggest that higher trading revenues periods might be correlated with higher fixed costs. All else being equal, the stability of the fixed costs suggests that firms with higher trading revenues also have higher profits. As such, HFT revenue variation is likely a close proxy for variation in HFT profits. 

Table 3 reports trading returns. Trading returns are calculated in two ways based on different capitalization measures: trading revenue / (trading assets minus trading liabilities) and (trading revenue / book equity). From these public filings in which capitalization is directly observable, we find trading returns to range from 60% to almost 237%, depending on the firm. This suggests the returns computed in Section III.A are of a reasonable magnitude. 

## IV. The Role of Speed in Performance

Having documented the performance of HFTs, we now test our main hypothesis about speed and HFT trading revenues. While most theories in which HFTs earn profits posit that fast traders should have an advantage, other theories suggest that traders of different speed can specialize along other dimensions (Weller, 2013; Roşu, 2015). According to these models, a relatively slow market intermediary could compensate by providing deeper liquidity on the book or greater risk-bearing capacity, thus making similar profits as fast traders in equilibrium. Alternatively, some firms can simply be more skilled than others. For example, differences in technological capabilities can persist because technological expertise and trading strategies are closely guarded trade secrets, giving rise to barriers preventing the movement of human capital and technical knowledge across firms. 

## A. The Relation between Trading Performance and Latency

Motivated by the contrasting theories discussed in the introduction, we test whether latency, and especially relative latency, is associated with increased performance. 

We estimate the following regression model using ordinary least squares (OLS): 

$$
\begin{array}{r} P e r f o r m a n c e _ {i, t} = \alpha_ {t} + \beta_ {1} \log (D e c i s i o n L a t e n c y) _ {i, t} + \beta_ {2} \mathbf {1} _ {\mathrm{top1} i, t} + \beta_ {3} \mathbf {1} _ {\mathrm{top1-5} i, t} \\ + \gamma^ {\prime} c o n t r o l s _ {i, t} + \mathrm{month-FEs} + \epsilon_ {i, t}, \end{array}\tag{1}
$$

where ���������� $e _ { i , t }$ is one of the HFT performance measures Revenues, Returns, Sharpe Ratio, Revenues per MSEK Traded, or Trading Volume. All dependent variables are aggregated across stocks, venues, and days within the month to generate a firm-month panel on which Eqn. (1) is estimated. Specifically, Revenues and Trading Volume are averaged across trading days, and Returns and Revenues per MSEK Traded are calculated using the firm-month observations of Revenues and Trading Volume. The factor model Alphas are not included because they are nearly identical to Returns, as discussed in Section III.A. 

The independent variables $\mathbf { 1 } _ { \mathrm { t o p } 1 i , t }$ and $\mathbf { 1 } _ { \mathrm { t o p } 1 - 5 \ : i , t } .$ , are indicators for whether a given firm is ranked in the Top 1 or Top 1-5 by speed in a given month. Nominal latency is captured using Decision Latency, while the $\mathbf { 1 } _ { \mathrm { t o p } 1 i , t }$ and $\mathbf { 1 } _ { \mathrm { t o p } ~ 1 - 5 ~ i , t }$ indicators capture relative speed. Since Decision Latency can vary widely across firms, from the microsecond to the second level (see Table 2), the relationship between trading speed and trading revenues is best captured by taking logs. The indicator variables capture the potentially non-linear relationship between latency and performance: the fastest firms may perform substantially better than firms that are only slightly slower. 

The control variables account for other characteristics that may affect HFT performance, including measures of their risk-bearing capacity and strategies. These variables include the Endof-Day Inventory Ratio, Max. Intraday Inventory Ratio, Investment Horizon, and the Aggressiveness Ratio, which are defined in Section III.A and calculated on the monthly frequency for each HFT firm. Max. Intraday Inventory is used in the denominator to calculate Returns and is thus omitted when Returns is the dependent variable. 

The continuous independent variables, namely, log(Decision Latency) and the control variables, are normalized to be in units of standard deviations. Month fixed-effects absorb timevarying market conditions, including market trading volume and volatility. Following Petersen (2009) and Thompson (2011), standard errors are dually clustered by firm and month to account for correlations both across firms and over time. Table 4 reports coefficient estimates for various specifications of the model described in Eq. (1). 

## INSERT TABLE 4 ABOUT HERE

Our first result is that being fast is associated with increased revenue. The first specification sets all slope coefficients except that of nominal latency $( \beta _ { 1 } )$ equal to zero and shows a negative and statistically significant relation between Revenues and nominal latency. 

The second result is that the effect of relative latency on Revenues dominates that of nominal latency. This is seen in the second and third specifications, where the $\mathbf { 1 } _ { \mathrm { t o p } 1 i , t }$ and $\mathbf { 1 } _ { \mathrm { t o p } 1 - 5 \ : i , t }$ indicators of relative latency are included along with the nominal latency variable in the second specification, and along with control variables in the third specification. The lack of statistical significance and reduced economic magnitude for log(Decision Latency) suggest that relative speed matters more than nominal speed. Specifically, the estimates in Column 3 show that being among the five fastest HFTs (Top 1-5) predicts average daily trading revenues that are SEK 15,451 higher than the for the HFTs outside the top five. Being the fastest (Top 1) provides on average daily trading revenues of SEK 24,639 in addition to the revenues from being in the Top 1-5: the coefficient on the Top 1 dummy tests the difference in revenues between being Top 1 and Top 1-5, which is found to be statistically significant.<sup>23</sup> HFTs that are not among the five fastest in a given month have average daily revenues reflected by the intercept of SEK 10,894. These numbers imply that the revenues of the fastest HFT firm are around five times higher than those of the “slow” (non-Top 1-5) HFTs. 

Several of the control variables are related to trading revenues. For example, a one standard deviation increase in the Max. Intraday Inventory is associated with decreased daily Revenues of 21,008 SEK, suggesting that HFTs that have tighter inventory management perform better. Similarly, HFTs that are more aggressive earn somewhat higher trading revenues. 

The results for latency effects on risk-adjusted performance measures are similar to those for Revenues. The only difference between Returns and Revenues is that the former is expressed relative to the firm market capitalization. The results thus indicate that the HFT firm size does not drive the relation between Revenues and relative latency. Furthermore, we find that the Sharpe Ratio is higher for HFT firms with lower relative latency. This demonstrates that the relation between Revenues and relative latency is not driven by the risk of the trading strategies applied. 

To understand why relative latency is important, we next analyze whether it is primarily related to the trading revenues per trade (quality) or the number of trades (quantity). If HFTs use latency advantages to better obtain and aggregate information in order to predict future price changes we would expect the fastest HFTs to have the highest revenues per trade. However, according to Table 4, we find only a weak statistical association between Decision Latency and Revenues per MSEK Traded, and when the control variables are included the latency effects are not stable. Instead, we find a strong relationship between trading speed and Trading Volume. The results imply that faster HFTs are able to capture a larger trading quantity, but that trading speed is not an important determinant of trading quality. It appears that the fastest HFTs are no more accurate at processing new information per trade than other traders, but their latency advantage allows them to capture the most trading opportunities. This result supports the use of a measure of trade quantity, like Revenues, rather than a measure of trade quality, like Revenues per MSEK Traded, when evaluating HFT performance. 

The results presented in this section show that HFTs with relatively low latency are more successful in capturing trading opportunities and earning higher revenues. To alleviate concerns about a spurious relationship between speed and performance, in the next section we focus on a quasi-experimental setting where the trading speed changes for some firms but not for others. 

B. Evidence from two colocation upgrades 

To address the potential endogeneity concern that another variable correlated with HFT latency might be instead driving trading performance, we put forward evidence from a quasiexperimental setting studying two colocation upgrades that cause some HFTs to increase their relative speed. 

On March 14, 2011 and September 17, 2012, NASDAQ OMX Stockholm implemented optional upgrades to its colocation offerings (the “Premium Colocation” and “10G Colocation” upgrades, respectively). Members subscribing to the previously fastest colocation service were then offered to upgrade to an even faster connection. We study these events, which result in some HFTs improving their latency rank, and find evidence in support of a causal relation between relative latency and trading performance. 

The September 17, 2012 colocation upgrade has been previously studied by Brogaard et al. (2015), and background and institutional detail on this event can be found in that paper. In particular, they find that only about half of the affected members immediately subscribed to the new connection type. Likely as a result, we find that some, but not all, HFTs improve their latency shortly after the upgrade becomes available. 

Specifically, we measure Decision Latency before and after the event, and compare the change in trading performance for HFTs that become relatively faster through the colocation upgrade to HFTs that become relatively slower. Given that Decision Latency consists of firmmonth observations, we compare the latency of each firm the first full month before the colocation upgrade to the second full month after the event; for consistency, we measure the change in HFT performance for each firm over this same period. In measuring Decision Latency, we skip a month after the colocation upgrade because it seems that HFTs take time to adopt and exploit this new technology; we observe that the distribution across firms of Decision Latency decreases and fully reaches a stable equilibrium by the second month. However, it is important to note that the horizon for assessing performance does not matter: the difference-in-difference results are robust to looking at the change in HFT performance in a 2, 4, 8, or 12 week period before and after the upgrade. 

We find two HFT firms for the March 14, 2011 event and one HFT firm for the September 17, 2012 that improve their latency rank and refer to them as Faster. We compare that group to three HFT firmss for the March 14, 2011 event and one HFT firm for the September 17, 2012 event that decline in latency rank, which we refer to as Slower. All other HFTs who have unchanged relative latency – including some who get nominally, but not relatively, faster – are excluded from this analysis. 

Table 5 reports the trading performance measures for Faster and Slower HFTs, before and after the colocation upgrade event. The results suggest that the group of HFTs that improve their relative latency around the colocation upgrade (Faster) also improve their trading performance. This result holds for all five measures of trading performance. The HFTs in the Slower group also improve their Revenues and Revenues per MSEK Traded, but less so than the Faster group. The Slower group also has a lower Trading Volume after the event, suggesting that those HFTs capture fewer trading opportunities. As seen by the difference-in-difference estimate in the bottom line of Table 5, the Faster group improves relative to the Slower group in terms of all trading performance measures considered. For each performance measure, we test the null hypothesis that there is no difference in the before-after change between the Faster and Slower groups; the statistical significance of the difference-in-difference estimates is assessed with a ttest, where a p-value is computed under the null by taking the before-after changes in performance for each HFT firm as independent observations, pooling together the Faster and 

Slower groups. There are seven firms with changing relative latency, yielding six degrees of freedom. 

## INSERT TABLE 5 ABOUT HERE

The difference-in-difference estimates are large, positive, and often statistically significant due to the consistency and magnitude of the change, despite the small sample size. Notably, the relative improvement is statistically significant and much stronger for the quantity measures and risk-adjusted measures than for the quality measure Revenues per MSEK Traded, which is not statistically significant. The findings are thus consistent with the evidence presented in the previous section. 

Given the small sample of firms that get relatively faster or slower, the evidence presented in Table 5 should be seen as suggestive. Nevertheless, the results are consistent with the notion that improved relative latency leads to a boost in trading performance, in particular in terms of quantity performance measures. 

## C. Alternative Latency Measures

We acknowledge two potential concerns about the Decision Latency metric. First, measuring Decision Latency requires both limit and market orders, potentially discriminating against HFTs that do not mix order types. Second, the microsecond time stamps reported by TRTH are not assigned when the trading venue receives an order, but when the information about the order arrives at the TRTH servers. Variation in the delay within venue can potentially introduce time-stamp noise in the Decision Latency metric, though we expect it to be mitigated by two factors: first, time-series variation in the delay is presumably stronger over longer time periods than within milliseconds, over which Decision Latency is measured; and, second, variation across venues due to geographical distance does not influence Decision Latency, which only uses time stamps from within the same venue. 

Nevertheless, to address these concerns, we consider two alternative approaches to measuring HFT latency. We construct two additional latency measures, Queuing Latency and Mean Latency, and re-estimate the results of Table 4, which analyzes the connection between latency and various measures of HFT performance. The results are qualitatively unchanged. 

To mitigate the time stamp noise, we measure Mean Latency. We use the same distribution of latencies as for Decision Latency, but instead of calculating the 0.1% quantile, we define Mean Latency as the mean of all latencies that are shorter than one millisecond. By using a central moment rather than an extreme quantile, we expect the time-stamp noise to cancel out, relying on the central limit theorem. This approach comes at the cost of not picking the cases where HFTs operate at their very fastest speed. 

Our second alternative latency measure, Queuing Latency, circumvents both concerns described above. For this measure, we exploit price changes that lead to a gap in the limit order book. As modelled by Yueshen (2014), if the price change is viewed as temporary, fast traders rush in to capture the top-of-queue limit order position in the emerging gap. When the price changes and a new tick opens up, Queuing Latency measures how often each HFT firm submits the first limit order and thus gets to the top of the queue. A higher value corresponds to lower latency. Note that this measure does not use time stamps and, furthermore, that simply more trading or limit order submissions does not help one get to the top of the queue: given the brief window when a new tick opens up, the chances of a randomly submitted order ending up first is negligible. 

The measurement procedure for Queuing Latency involves the following three steps. First, we identify trades that consumes all available liquidity at a price level (gap-opening trades). Second, for each gap-opening trade we identify the next trade at the same price level as the gap-filling trade. We retain the passive counterparty of all gap-filling trades that: (i) are in the same direction as the corresponding gap-opening trades; (ii) occur within 10 seconds after the corresponding gap-opening trades; (iii) do not have the same broker as buyer and seller; (iv) do not have the same passive counterparty as the corresponding gap-opening trades.<sup>24</sup> 

We repeat the analysis in Table 4 for the two alternative measures of latency and report the findings in Table 6. As in Section IV.A, we use the alternative latency measures to rank HFTs by latency in each month and construct new Top 1 and Top 1-5 rank dummies. Note that in Panel A, which looks at Queuing Latency, we represent nominal latency with log(Queuing Latency + 1), so that we do not take the log of zero, which is the lowest possible value that Queuing Latency can attain. 

## INSERT TABLE 6 ABOUT HERE

Panel A reports the results for Queuing Latency. In Column 1, there is an association between nominal speed and trading performance. In contrast to Table 4, we expect a positive coefficient, since lower latency is represented by a higher value of Queuing Latency. In Columns 2 and 3, when the Top 1 and Top 1-5 rank dummies are added, the coefficient on nominal latency now becomes insignificantly different from zero, while the magnitudes of the estimates on the Top 1 and Top 1-5 rank dummies are large and significant. Thus, as before, relative latency is more important than nominal latency. Similar results can be seen for Returns, the Sharpe Ratio, and Trading Volume. However, as usual for the quality measure, Revenues per MSEK Traded, the results are small in magnitude and not significant. 

Panel B reports the results for Mean Latency and tells a similar story. The only main difference between Panel B and Table 4 is that the coefficient on the Top 1-5 rank dummy is generally statistically significant, but the one on Top 1 is not, although it is still generally positive and large in magnitude. So while being relatively fast according to this measure is still important, as reflected in the coefficient on the Top 1-5 dummy, Mean Latency may not be the best measure to capture the very fastest HFTs at their peak potential, when extreme low latencies are needed to outperform competitors. Nevertheless, as a central tendency and not an extreme value, Mean Latency is useful for assessing the robustness of our main measure, Decision Latency. 

## V. How does Latency Impact Performance?

The theoretical literature identifies two channels through which traders benefit from being fast: short-lived information and risk management. The benefit of low latency through short-lived information is explored by Foucault et al. (2016). They show that fast traders trade aggressively on news, picking off stale quotes. Furthermore, Biais et al. (2015) and Foucault et al. (2015) show that fast traders can benefit from a superior ability to react to cross-market arbitrage opportunities. Chaboud, Chiquoine, Hjalmarsson and Vega (2014) provide empirical evidence of fast traders pursuing cross-market arbitrage. The benefit of low latency in risk management is highlighted by Hoffmann (2014), who emphasizes that low latency allows liquidity providers to reduce their adverse selection costs, by revising stale quotes before they are picked off. Aït-Sahalia and Saglam (2014) add that fast traders can also benefit in terms of reduced inventory risk, which is supported empirically by Brogaard et al. (2015). 

In this section we investigate specifically how latency influences the two channels discussed above. We find that relative latency determines ability in both short-lived information trading and risk management. 

A. Short-Lived Information and Risk Management in General 

To capture trading on short-lived information, we measure active Price Impact as the basis point change in the bid-ask spread midpoint from just before a trade initiated by an HFT firm to ten seconds after. To capture risk management, we measure passive Realized Spread as the basis point difference between the transaction price and the bid-ask spread midpoint ten seconds after a trade where an HFT firm is the liquidity provider. Realized Spread captures the benefit of earning a wide bid-ask spread, as well as the ability to avoid supplying liquidity to trades with price impact. Each measure is calculated on a firm-stock-month frequency as the SEK-volume-weighted average across all trades of a given firm in each stock and each month. We interact both Realized Spread and Price Impact with a ±1 buy-sell indicator variable, such that a higher coefficient corresponds to better trading performance. As the analysis requires information on the bid-ask spread, we limit the measures to trades that can be matched to order book data, both contemporary to the trade and ten seconds later. 

We re-estimate Eq. (1) at the firm-stock-month level with Price Impact and Realized Spread as the dependent variables. Unlike in Table 4, we disaggregate by stock to control for stock-level characteristics, such as the Quoted Spread and Tick Size, which may affect Price Impact and Realized Spread. As before, the $\mathbf { 1 } _ { \mathrm { t o p } 1 i , t }$ and $\mathbf { 1 } _ { \mathrm { t o p } ~ 1 - 5 ~ i , t }$ are indicators that capture relative latency, whereas log(Decision Latency) captures nominal latency. The estimation is run with and without control variables. 

The control variables include both HFT firm characteristics and stock characteristics. The HFT firm characteristics are End-of-day Inventory, Max. Intraday Inventory, Investment Horizon, and Aggressiveness Ratio, defined as in Section III.A. Since these variables are firmcharacteristics, they are assigned the same value across stocks. The stock characteristics are measured on stock-month frequency and are defined as in Section II.B: Volatility, Fragmentation Index, Tick Size, and Quoted Spread. The Non-HFT Trading Volume is the daily sum of SEK trading volume in each stock that does not involve HFTs. All continuous independent variables are in units of standard deviations. Standard errors are dually clustered by firm-stock and month. The results are reported in Table 7. 

## INSERT TABLE 7 ABOUT HERE

As with HFT performance in general, we find for the specific channels that relative latency, not nominal latency, drives performance. The coefficients for the $\mathbf { 1 } _ { \mathrm { t o p } ~ 1 - 5 ~ i , t }$ relative latency dummy is statistically significant and economically meaningful for both the Price Impact and the Realized Spread. For example, being in the Top 1-5 by speed increases Price Impact by 0.645 bps, which can be related to the intercept of 3.96 bps. That means that the five fastest HFTs have 16% (0.645 / 3.96) higher price impact than other HFTs. In addition, the fastest HFT outperforms the price impact of other HFTs by another 0.34 basis points (0.34 / 3.96 = 9%). For the Realized Spread the Top 1-5 coefficient is 0.477 bps, whereas the intercept is insignificantly different from zero. This indicates that being among the fastest HFTs is important for being successful at the risk management required for passive trading. The results are robust to inclusion of the control variables. 

We conclude that relative latency is important both for improving trading on short-lived information and for risk management. This is consistent with theoretical models, such as 

Foucault et al. (2016) on active trading; and Hoffmann (2014) and Aït-Sahalia and Saglam (2014) on passive trading. 

## B. Short-Lived Information and Risk Management in Cross-Market Arbitrage

In a more controlled environment we re-examine both channels by focusing on crossmarket trading between the futures market and equities. Specifically, we test if faster HFTs are more likely than slower HFTs to actively trade in equities in quick response to “news” in the futures market, where “news” is defined to be a price change in the OMXS30 futures above a certain size. We also ask whether faster HFTs are less likely than slower HFTs to be adversely selected in a passive trade in equities markets in response to “news” in the futures market. The investigation is in line with the theoretical setup of active fast trading by Biais et al. (2015) and Foucault et al. (2015). 

We estimate the following probit regression, which in essence follows the setup of Hendershott and Riordan (2013) and Brogaard et al. (2015): 

$$
\operatorname * {P r} [ \text { Fast   HFT   Trades } ] = \Phi [ \beta \text { News } + \gamma^ {\prime} \text { controls } + \text { Stock   FEs } ].\tag{2}
$$

The unit of observation is a trade. To capture who is trading quickly in response to “news” in the futures market, we consider equity market trades in the 1-second interval subsequent to a “news” event in the futures market. We define Fast HFT as being either Top 1 or Top 1-5 of HFTs in terms of Decision Latency in each month; Slow HFT are those not among the top five. The dependent variable is 1 when a Fast HFT executes an equities trade in the subsequent 1-second and 0 if a Slow HFT does it. Thus, our results can be interpreted as the increased probability of a Fast HFT trading in equities relative to a Slow HFT, in response to “news” in the futures market. 

News is defined to be ±1 when the return on the OMXS30 futures during a one-second window preceding the stock trade is large, defined as when the absolute return exceeds the top decile among non-zero absolute returns of that month, and 0 otherwise. News takes the value +1 if the active party trades in direction of the news, and -1 if in the opposite direction. This design implies that News reflects any event that causes a large price change in the futures index. Note that all sample stocks are constituents of the index underlying the futures contract, making arbitrage activities between the two markets likely (Hasbrouck, 2003). 

We also control for the following variables, which may affect the probability of Fast HFTs doing cross-market arbitrage. Lagged Volatility is the average second-by-second squared return (multiplied by 1,000) over the previous ten seconds; Lagged Volume is the SEK trading volume (divided by 100,000) over the previous ten seconds; Quoted Spread is defined as before; and Depth at BBO is the average number of shares available at the best bid quote and the best offer quote (divided by 100,000), multiplied by the bid-ask spread midpoint. 

Estimates for active trading, the sample being all trades initiated through the submission of a market order by a HFT firm, are reported in Table 8, Panel A. Similarly, the estimates for passive trading, the sample being all trades where liquidity is provided by an HFT firm, are presented in Panel B. For computational tractability, regressions are run monthly for all month in 2010-2014. Similar to the Fama and Macbeth (1973) procedure, the monthly coefficients are averaged across months to produce the estimates reported in Table 8. To assess the economic magnitudes, we report marginal effects. The marginal effects show the increased probability of Fast HFTs to engage in a trade if the explanatory variable increases by one standard deviation, conditional on all other explanatory variables being at their unconditional means. 

## INSERT TABLE 8 ABOUT HERE

We find that the News coefficients are positive and statistically significant for active trading (Panel A). Based on the marginal effects, the fastest HFT firm (Top 1) is 0.6% more likely to actively trade in equities subsequent to “news” arrival in the futures market, relative a trader outside of the Top 5. The Top 1-5 HFTs show similar results. Overall, we conclude that faster HFTs are more likely to quickly submit market orders in response to changes in the futures index. This is consistent with fast active traders being better positioned to pursue cross-market arbitrage, as modeled by Biais et al. (2015) and Foucault et al. (2015). For passive trading, the News coefficients are negative (Panel B), indicating that fast HFTs are less likely to get caught in a passive equities trades that incur adverse selection costs to the liquidity provider. The result is not statistically significant for the Top 1 HFT firm, but is statistically significant at the 1% level for the Top 1-5 HFTs. This is in line with Foucault et al. (2015), who find that the probability of toxic arbitrage is related to the latency of arbitrageurs relative the latency of liquidity providers. 

## VI. Implications of Speed for the HFT Industry

Sections IV and V show that relative differences in latency can help explain the variation in HFT performance. If trading speed drives performance, why are HFT firms not competing away their trading revenues, either through new entry, higher trading volumes, or increased investment in speed and trading sophistication? 

According to the traditional view of market-making competition (Ho and Stoll, 1983; Weston 2000), the alpha generated by HFTs and the concentration of revenues should disappear as the industry matures. Alternatively, if HFTs compete on relative latency, then increased competition should not drive profit opportunities to zero. As argued by Budish et al. (2015), regardless of how fast the market as a whole becomes, there is always at least one firm with a relative speed advantage that can adversely select other traders. Additionally, rents remain concentrated among the fastest HFTs, as slower HFTs arrive marginally too late to trading opportunities to compete. 

We explore some of the prediction of relative latency regarding market concentration.<sup>25</sup> The HFT literature on competition on relative latency makes several predictions: persistence in performance, both at the firm-level and industry-wide level, high concentration of HFT revenues and trading volume, and difficulty of new entry. We examine each of these predictions and find evidence that all apply for the HFT industry. 

## A. Persistence in Firm-Level Performance

We first test for persistence at the firm-level. Large differences in HFT firm performance could potentially be driven by luck. For instance, in a model of identically skilled HFTs, all engaging in strategies with right-skewed distributions of performance, some will happen to outperform. Persistence shows that something other than luck drives a firm’s performance. 

There is an extant literature showing that performance for actively-managed mutual funds in period t generally does not predict performance in period t+1 (Carhart, 1997). However, there is evidence of persistence by some investors (Jagannathan, Malakhov, and Novikov, 2010, for hedge funds; and Kaplan and Schoar, 2004, for private equity). Nonetheless, the expectation for most types of investors and funds is little persistence in performance. 

To analyze persistence we regress various measures of performance (Revenues, Revenues per MSEK Traded, Returns, and the Sharpe Ratio) on their lagged values, on both the daily and monthly frequency (except for the Sharpe Ratio, which is available on the monthly frequency only). Measures of performance are standardized in the cross section. That is, on each day, firmlevel performance is centered on the mean and scaled by the standard deviation across firms. The standardization controls for potential time-variation in the mean and variance of returns. We also estimate persistence regressions with rank-order performance, ranking the relative performance of firms as 1, 2, 3, etc., for each measure of performance on each day or month. We estimate the following regression using OLS: 

$$
P e r f o r m a n c e _ {i, t} = \beta P e r f o r m a n c e _ {i, t - 1} + \epsilon_ {i, t},\tag{3}
$$

where $P e r f o r m a n c e _ { i , t }$ is defined as above. Results based on daily observations are reported in Table 9, Panel A, and those using monthly observations are reported in Panel B. Since each measure is standardized in the cross-section, the constant term in the regression model is mechanically zero. We refer to $\beta$ as the persistence coefficient, with $\beta = 1$ meaning perfect persistence and $\beta = 0$ meaning no persistence. Standard errors are dually clustered by firm and day in Panel A and by firm and month in Panel B. 

## INSERT TABLE 9 ABOUT HERE

We find that HFTs have statistically significant daily persistence coefficients of 0.235 for Revenues and 0.387 for Returns. On the monthly frequency, we find higher persistence coefficients: 0.631 for Revenues, 0.763 for the Sharpe Ratio, and 0.446 for Returns. Performance is more persistent at the monthly level, which is likely due to the higher idiosyncratic risk in daily observations. The rank order analysis shows similar persistence. Consistent with our earlier argument that Revenues per MSEK Traded may be a less relevant performance metric for HFTs, we find lower persistence in this measure. 

In summary, we find that the performance of HFTs is relatively stable over time, in terms of nominal performance as well as in terms of performance rankings. Firms that have done well in the past typically continue to outperform their competitors in the future. 

## B. Persistence in Industry-Wide Performance

Having found evidence of persistence in firm-level performance we examine overall performance of the HFT industry over our five year sample. Given that the HFT industry is relatively new, we may observe decreasing industry-wide performance if competition is increasing over time. However, in a market with competition on relative speed, performance may not change. Budish et al. (2015), for example, argue that if HFTs compete on relative latency, regardless of how fast the market as a whole becomes, there will always be a relatively fastest firm that can use its speed advantage to adversely slower traders, capturing a stable level of rents regardless of nominal speed differences. Furthermore, if competition on relative speed makes new entry difficult, as we show in Section VI.D, difficulty of new entry may keep aggregate HFT performance from declining. 

Consistent with these predictions, we find that the HFT industry-wide performance is relatively stable over the five-year sample. Table 10, Panel A, reports average daily statistics aggregated across all HFTs and all stocks and reported in half-year intervals. The statistics include Total Daily Revenues (Revenues summed across all HFTs), Average Daily Revenues (the Total Daily Revenues averaged across HFTs), Average Revenues per MSEK Traded (the ratio of Total Daily Revenues and Daily Trading Volume), and Daily Trading Volume (the Trading Volume summed across all HFTs and reported in MSEK). Time trends for Total Daily Revenues and Average Daily Revenues are also plotted in Figure 2, Panels A and B. 

## INSERT TABLE 10 ABOUT HERE INSERT FIGURE 2 ABOUT HERE

Our results show that Total Daily Revenues and Average Daily Revenues are relatively stable over the five-year period.<sup>26</sup> Interestingly, as shown in Figure 2, Panel B, Daily Trading Volume per Firm trends up while Average Revenues per MSEK Traded trends down, but the ratio of the two, HFT Revenues per Firm, is stable. One possible interpretation is that as HFTs are presumably competing more by increasing trading volume and pursuing ever-lower latencies, they are chasing the same number of profit opportunities, so the resulting HFT revenues per firm is the same. 

To formally test the movement of the trends, we estimate the following OLS regression on daily observations: 

$$
P e r f o r m a n c e _ {t} = \alpha + \beta (y e a r - 2 0 1 0) + \epsilon_ {t},\tag{4}
$$

where �����������<sub>�</sub> is one of the performance measures described above, and year is a continuous variable (e.g., year would take on the approximate value of 2014.25 on March 31, 2014). A positive (negative) coefficient on the (���� − 2010) variable corresponds to an increasing (decreasing) trend in the HFT industry-wide performance over the period 2010-2014. Newey-West standard errors with 30 day lags are used. The coefficient estimates are presented in Table 10, Panel B. 

The tests statistically confirm the aforementioned trends. However, there is statistical evidence that trading revenues are slightly increasing over the sample period: a yearly increase of 

22,682 SEK for Total Daily Revenues, relative to a baseline of 166,484 SEK in the first half of 2010. This increase is however not statistically significant in terms of Average Daily Revenues, which takes the number of HFTs in the industry into account. 

We also examine time trends in the cost of HFT activities for non-HFTs, which is defined as HFT Total Daily Revenues divided by Non-HFT Trading Volume, calculated on a daily basis. This measure captures the amount of revenue paid from non-HFTs to HFTs per SEK traded. The cost of HFT activities for non-HFTs is relatively small, varying between 0.113 and 0.426 bps, depending on the month, which is about the same order of magnitude as typical exchange fees (see Appendix Section A6). Whereas the exchange fees are direct costs incurred to exchange members and typically passed on to their clients, the cost of HFT activities is extracted indirectly through the trading process. Another way to put the cost of HFT activities into perspective is to compare it to the effective spread, which according to Table 1 is between 2 and 6 bps. That is, the cost of crossing the (half) bid-ask spread is more than ten times higher than the cost of HFT activities for non-HFTs. As seen in Figure 2, Panel C, and formally tested in the last column of Table 10, Panel B, there is a small upward time trend in the cost of HFT activities, starting from around 0.13 bps and increasing by about 0.06 on average per year. 

Thus, despite concerns that HFTs competing on relative latency might impose costs on non-HFTs, the average observed cost of HFT activities for non-HFTs is surprisingly small. 

## C. HFT Market Concentration over Time

We next turn to investigate HFT market concentration. While high concentration by itself need not signify lack of competition, there may be reasons why high concentration might be of concern in the context of HFTs. For example, a high concentration among market intermediaries could adversely affect market stability. For example, a dominant HFT firm that incurs a technical malfunction, suffers large capital losses, or suddenly withdraws its liquidity supply could lead to market fragility. 

We show that the HFT industry concentration remains high and relatively constant over the five-year sample. We calculate Herfindahl indices, a commonly used measure of concentration of market share or earnings within an industry, for both Revenues and Trading Volume. The Herfindahl Industry Concentration by Revenues is calculated as: 

$$
H e r f i n d a h l _ {i, t} = \sum_ {i = 1} ^ {N} \left[ \frac {R e v e n u e s _ {i , t}}{H F T R e v e n u e s _ {t}} \right] ^ {2},\tag{5}
$$

where N is the number of firms in month t that earn non-negative trading revenues, Revenues<sub>i,t</sub> is firm i’s total trading revenues in month t, and HFT Revenues<sub>t</sub> is the trading revenues summed across all HFT firms. Herfindahl Industry Concentration by Volumes is calculated using the same formula but considering Trading Volume instead of trading Revenues. A larger index implies a more concentrated industry: the index is at its minimum 1/N when all HFT firms have the same share of the industry and at its maximum of 1 when all activity is concentrated to one firm. 

As with the trading performance time trends, the Herfindahl indices are first calculated for each trading day, then averaged across trading days of each half-year block in the data set. Standard deviations are reported in parentheses. Results are reported in Table 10, Panel A, and graphed in Figure 2, Panel D. 

The Herfindahl industry concentration in terms of volume lies in the range from 0.186 to 0.304. In terms of revenues, the corresponding interval is from 0.275 to 0.354. As a reference, Van Ness, Van Ness, and Warr (2005) find that market makers have an average Herfindahl index in terms of trading volume on NASDAQ of 0.14, with a range of 0.037 to 0.439. 

We test for a time trend in industry concentration by estimating the following OLS regression: 

$$
C o n c e n t r a t i o n _ {t} = \alpha + \beta (y e a r - 2 0 1 0) + \epsilon_ {t},\tag{6}
$$

where year is a continuous variable and Concentration<sub>t</sub> is one of the concentration measures discussed above. The coefficient estimates are reported in Table 10, Panel B. 

We find no statistically significant time trend for revenues concentration. There is a statistically significant decrease in trading volume concentration, but it is not economically significant. The Herfindahl industry concentration by volume decreases by 0.009 per year from its starting value of 0.292 in the first-half of 2010. The overall conclusion with respect to industry concentration is however that it is relatively constant over the five years. 

## D. Entry and Exit

To investigate competition in the HFT industry, we examine the properties of firms that just entered the market. New entrants can potentially introduce competition and drive down both firm-level and industry-wide profits. However, frictions in labor markets may prevent the movement of human capital and technical knowledge to new HFTs. For instance, technological expertise and trading strategies are closely guarded trade secrets and employees often agree to non-compete and non-disclosure agreements, preventing them from simply starting new firms or moving to competitors. If new entrants cannot simply pay to acquire skill but require experience, then they may earn less and be less likely to survive in the market. 

To evaluate the importance of experience, we regress performance measures on indicator variables for the length of time an HFT firm has been active in a given stock, designating less than 1 month, 2 months or 3 months as indicators of new entry. 

We estimate the following regression model using OLS: 

$$
\begin{array}{c} \text {Performance} _ {i, j, t} = \beta_ {1} \mathbf {1} _ {\text {one - month} i, j, t} + \beta_ {2} \mathbf {1} _ {\text {two - month} i, j, t} + \beta_ {1} \mathbf {1} _ {\text {three - month} i, j, t} \\ + (\text {day x stock}) \text {-FEs} + \epsilon_ {i, j, t}, \end{array}\tag{7}
$$

where $P e r f o r m a n c e _ { i , j , t }$ can be Revenues, Revenues per MSEK Traded, or Returns, and is defined on a firm-stock-day frequency over the period 2010-2014. We exclude the observations in the first three months of the sample, since new entry during this period cannot be established. The notation $1 _ { o n e - m o n t h i , j , t }$ takes the value 1 if firm i began trading stock j in the last 30 calendar days, otherwise it takes the value $0 ;$ similarly, the $\ 1 _ { t w o - m o n t h } \ i , j , t$ dummy corresponds to beginning trading in stock $j$ in the last 31-60 days, and the $\ 1 _ { t h r e e - m o n t h \ i , j , t }$ dummy corresponds to the previous 61-90 days.<sup>27</sup> If new entrants are less competitive and perform worse than established firms, the coefficient on the one-month dummy should be negative, and, consistent with experience mattering, the two- and three-month dummy coefficients should also be negative though less so. The results are reported in Table 11. Standard errors are dually clustered by firm-stock and by month and are reported within parentheses. 

## INSERT TABLE 11 ABOUT HERE

Looking at Revenues, HFTs have statistically significant negative coefficients corresponding to the new entry dummies, with the negative value of -1,900 SEK for the 1-month dummy, -3,050 SEK for 2 months, and -780 SEK for 3 months. Returns are also significantly lower for new entrants in the first and second month. However, Revenues per MSEK Traded is statistically insignificant for all three time periods. The fact that the new firms have lower total trading revenues but no statistically significant difference in Revenues per MSEK Traded is consistent with HFTs competing on quantity, not quality, and new firms being less able to compete on capturing quantity. 

Additionally, we examine whether new entrants are more likely to exit the market by estimating the model described in Eq. (7) with the dummy $E x i t _ { i , j , t }$ as the dependent variable, which takes the value 1 on day t for firm i if that is the last day firm i trades stock j. In this analysis we exclude observations in December 2014, the last month of the analysis, as we are unable to determine market exit in that month. The model is estimated as a linear probability regression, and the results are in Table 11. 

We find that, on average, a new entrant in a stock has a higher probability of exit compared to more established HFTs. The effect is found in the one- and two-month indicator variables, both being statistically significant at the 1% level. The daily probability of exit is a statistically significant and economically large amount of 1.4% in the first month. The increased probability of exit is for each day, not the cumulative probability of exit at any future point, making the magnitude substantial. 

Why do new entrants typically perform worse than established firms? Given our previous findings on latency, we examine whether new entrants are slower than the incumbent HFTs. Repeating the analysis in Eq. (7) but replacing the dependent variable with the Decision Latency measure (expressed in milliseconds), we find statistically significant coefficients on the 1-month, 

2-month, and 3-month dummies of 44.36, 134.6, and 22.8 milliseconds.<sup>28</sup> The positive coefficients on the indicator variables show that new entrants are slower than established firms, which might in part explain their lower trading revenues. 

In summary, we find that new entrants tend to perform worse and are more likely to exit than established HFTs. This finding helps explain the continued concentration of revenues among a small subset of established firms: if new entrants tend to exit, then the concentration of revenues continues. A high and steady industry concentration combined with strong firm-level persistence of Revenues and Returns suggests that top performing incumbent HFTs maintain their position in the market. Together, the four measures of industry structure we examine point to high concentration, consistent with relative latency driving performance. 

## VII. Conclusion

We study the role of latency in the performance of HFT firms. We document a number of statistics consistent with superior investment performance by HFTs. There are large crosssectional differences in performance in the HFT industry, with trading revenues disproportionally accumulating to a few firms. The fastest firms tend to earn the largest trading revenues. While latency decreases substantially over our five-year sample period, we show that it is relative latency, not nominal latency, that helps explain the differences in performance across HFTs. 

Furthermore, we examine how speed may be used in specific HFT strategies. We find evidence that relative latency is important for success in trading on short-lived information, for risk management in liquidity provision, and for cross-market arbitrage. 

Finally, we explore implications of competition on relative latency regarding HFT concentration. If small differences in latency are important, then the HFT industry should be characterized by persistence in performance, high concentration, and difficulty of new entry. We find evidence that is consistent with these predictions. Firm trading performance is persistent, trading revenues are high and non-declining, as is HFT concentration, and new HFT entrants tend to be slower, underperform, and are more likely to exit. 

## References



Aït-Sahalia, Y. and M. Saglam, 2014, High-frequency traders: Taking advantage of speed, Working Paper. 





Biais, B., T. Foucault, and S. Moinas, 2015, Equilibrium fast trading, Journal of Financial Economics, 116 (2), 292-313. 





Boehmer, E., D. Li, and G. Saar, 2015, Correlated high-frequency trading, Working Paper. 





Bongaerts, D. and M. Van Achter, 2015, High-frequency trading and market stability, Working Paper. 





Breckenfelder, J., 2013, Competition between high-frequency traders, and market quality, Working Paper. 





Brogaard, J. and C. Garriott, 2015, High-frequency trading competition, Working Paper. 





Brogaard, J., B. Hagströmer, L. Nordén, and R. Riordan, 2015, Trading fast and slow: Colocation and liquidity, Review of Financial Studies, 28 (12), 3407-3443. 





Brogaard, J., T. Hendershott, and R. Riordan, 2014, High-frequency trading and price discovery, Review of Financial Studies, 27 (8), 2267-2306. 





Budish, E., P. Cramton, and J. Shim, 2015, The high-frequency trading arms race: Frequent batch auctions as a market design response, Quarterly Journal of Economics, 30 (1547), 1621. 





Carhart, M., 1997, On persistence in mutual fund performance, Journal of Finance, 52 (1), 57- 82. 





Cartea, A. and J. Penalva, 2012, Where is the value in high frequency trading?, Quarterly Journal of Finance, 2 (3), 1250014. 





Chaboud, A., B. Chiquoine, E. Hjalmarsson, and C. Vega, 2014, Rise of the machines: Algorithmic trading in the foreign exchange market, Journal of Finance, 69 (5), 2045- 2084. 





Chen, J., H. Hong, M. Huang, and J. Kubik, 2004, Does fund size erode mutual fund performance? The role of liquidity and organization, American Economic Review, 94 (5), 1276-1302. 





Clark-Joseph, A., 2013, Exploratory trading, Working Paper. 





Ellis, K., Michaely, R., & O'Hara, M. (2000). The accuracy of trade classification rules: Evidence from Nasdaq. Journal of Financial and Quantitative Analysis, 35(04), 529-551. 





Fama, E., and French, K., 1993, Common risk factors in the returns on stocks and bonds, Journal of Financial Economics, 33 (1), 3-56. 





Fama, E., and J. MacBeth, 1973, Risk, return, and equilibrium: Empirical tests, Journal of Political Economy, 81 (3), 607-636. 





Foucault, T., J. Hombert, and I. Roşu, 2016, News trading and speed, Journal of Finance, 71 (1) 335-382. 





Foucault, T., R. Kozhan, and W. Tham, 2015, Toxic arbitrage, Working Paper. 





Frank, R. H., 2005, Positional externalities cause large and preventable welfare losses, American Economic Review, 95 (2), 137-141. 





Geroski, P., R. Gilbert, and A. Jacquemin, 1990, Barriers to entry and strategic competition, Vol. 41, Taylor & Francis. 





Hagströmer, B. and L. Nordén, 2013, The diversity of high-frequency traders, Journal of Financial Markets, 16 (4), 741-770. 





Hagströmer, B., L. Nordén, and D. Zhang, 2014, How Aggressive Are High‐Frequency Traders?, Financial Review, 49 (2), 395-419. 





Hasbrouck, J., 2003, Intraday price formation in US equity index markets, Journal of Finance, 58 (6), 2375-2400. 





Hendershott, T., and R. Riordan, 2013, Algorithmic trading and the market for liquidity, Journal of Financial and Quantitative Analysis, 48 (4), 1001-1024. 





Ho, T. and H. Stoll, 1983, The dynamics of dealer markets under competition, Journal of Finance, 38 (4), 1053-1074. 





Hoffmann, P., 2014, A dynamic limit order market with fast and slow traders, Journal of Financial Economics, 113 (1), 156-169. 





Jagannathan, R., A. Malakhov, and D. Novikov, 2010, Do hot hands exist among hedge fund managers? An empirical evaluation, Journal of Finance, 65 (1), 217-255. 





Jovanovic, B. and A. Menkveld, 2015, Middlemen in limit-order markets, Working Paper. 





Kaplan, S. and A. Schoar, 2004. Private equity performance: returns, persistence, and capital flows, Journal of Finance, 60 (4), 1791-1823. 





Kirilenko, A., A. Kyle, M. Samadi, and T. Tuzun, 2015, The flash crash: The impact of high frequency trading on an electronic market, Working Paper. 





Lee, C. and M. Ready, 1991, Inferring trade direction from intraday data, Journal of Finance, 46 (2), 733-746. 





Menkveld, A. J. and M. Zoican, 2015, Need for speed? Low latency trading and adverse selection, Working Paper. 





Petersen, M., 2009, Estimating standard errors in finance panel data sets: Comparing approaches, Review of Financial Studies, 22 (1), 435-480. 





Roşu, I., 2015, Fast and Slow Informed Trading, Working Paper. 





Securities and Exchange Commission (U.S.), 2010, Concept release on equity market structure. 





Shkilko, A. and K. Sokolov, 2016, Every cloud has a silver lining: Fast trading, microwave connectivity and trading costs, Working Paper. 





Thompson, S., 2011, Simple formulas for standard errors that cluster by both firm and time, Journal of Financial Economics, 99 (1), 1-10. 





van Kervel, V. and A. J. Menkveld, 2015, High-frequency trading around large institutional orders, Working Paper. 





Van Ness, B., R. Van Ness, and R. Warr, 2005, The impact of market-maker concentration on adverse selection costs for NASDAQ stocks, Journal of Financial Research, 28 (3), 461- 485. 





Weller, B., 2013, Intermediation chains and specialization by speed: Evidence from commodity futures markets, Working Paper. 





Weston, J., 2000, Competition on the Nasdaq and the impact of recent market reforms, Journal of Finance, 55 (6), 2565-2598. 





Yao, C. and M. Ye, 2015, Why trading speed matters: a tale of queue rationing under price controls, Working Paper. 





Yueshen, B. Z., 2014, Queuing uncertainty in limit order market, Working Paper. 



## Figure 1: HFT Decision Latency over time

This figure plots Decision Latency (indicated on the vertical axis on a log scale) from January 2010 to December 2014. For each firm-month, Decision Latency is recorded as the 0.1% quantile of a distribution of latencies between a passive trade followed by an active trade at the same venue, in the same stock, within one second. HFT #1 is the Decision Latency of the fastest HFT firm in each month; HFTs #1-5 is the average Decision Latency of the 5 fastest HFTs in each month; and All HFTs is the average Decision Latency across all HFTs for which latency is lower than one second in the given month. The vertical bars indicate microstructure events at NASDAQ OMX Stockholm that are expected to be associated with changes in latency. The sample consists of 25 Swedish stocks. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/83a2737b-983b-43f5-be2c-da9c84185769/f7ada58e9615fdf3483888500fb72cf454216e5d239992fb9052e675b380056c.jpg)


## Figure 2: HFT revenues, cost of HFT activities, and industry concentration over time

This figure shows various time series trends. Panel A plots Total Daily Revenues, which is the average daily sum of Revenues (defined as in Table 2) across all HFT firms. Panel B plots Firm-Average Daily Revenues, which is the average Revenues across all HFT firms active on each given day. This variable is equivalent to SEK Trading Volume per Firm times Revenues per MSEK Traded, which are also plotted. Panel C plots the Cost of HFT Activities to Non-HFTs, calculated as HFT Total Daily Revenues divided by the total non-HFT trading volume (in SEK). Panel D plots two indexes of HFT Industry Concentration: Herfindahl indexes calculated on daily Revenues or with daily Trading Volumes, see Eq. (5). The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). The time series are reported on a biannual frequency. 


Panel A: Total Daily Revenues


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/83a2737b-983b-43f5-be2c-da9c84185769/49ef07e621aa2fa2caa944b0c893eaf5a00388f84cd7ef6fef1818e6b682ef61.jpg)



Panel B: Firm-Average Daily Revenues


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/83a2737b-983b-43f5-be2c-da9c84185769/ecaa56628c0d111ef80e135eb951a21a4f09f99039f3461f52447b3ee152ad53.jpg)



Panel C: Cost of HFT Activities to Non-HFTs


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/83a2737b-983b-43f5-be2c-da9c84185769/d04191a4d5060ecf963284126efb9a5ff209b66d8065642f65056ed0ec5aeecb.jpg)



Panel D: HFT Industry Concentration


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/83a2737b-983b-43f5-be2c-da9c84185769/48821210cee519b31e99685e37d2ff669b660d42e919e409ed864b77761d184b.jpg)


## Table 1: Stock characteristics

This table reports summary statistics of the 25 Swedish stocks in the sample. Market Capitalization is based on the closing price on December 31, 2014 (expressed in MSEK). All other statistics are calculated as averages across trading days in December 2014. Because SCVb is delisted in May 2014, the metrics for that stock are based on April 2014. Daily Trading Volume refers to trading at NASDAQ OMX Stockholm only and is reported in MSEK. Daily Turnover is the Daily Trading Volume divided by Market Capitalization, expressed in percentage points. Tick Size is the average minimum price change; Quoted Spread is the average bid-ask spread prevailing just before each trade; and Effective Spread is the trade value-weighted average absolute difference between the trade price and the bid-ask midpoint. All spread measures are based on continuous trading at NASDAQ OMX Stockholm, expressed relative to the bidask spread, and presented in basis points. The Tick Size and the Quoted Spread are halved to be comparable to the Effective Spread. Volatility is the average 10-second squared returns, calculated from bid-ask midpoints. The Fragmentation Index is the inverse of a Herfindahl index of trading volumes across the five largest trading venues (BATS, Burgundy, Chi-X, NASDAQ OMX Stockholm, and Turquoise); a higher value signifies greater fragmentation. The table is sorted by Market Capitalization. 

<table><tr><td>Stock Ticker</td><td>Market Cap. (MSEK)</td><td>Daily Trading Vol. (MSEK)</td><td>Daily Turnover (%)</td><td>Tick Size (bps)</td><td>Quoted Spread (bps)</td><td>Effective Spread (bps)</td><td>Volatility (sq. bps)</td><td>Fragmentation Index</td></tr><tr><td>HMb</td><td>475,595</td><td>1,358</td><td>0.29</td><td>1.57</td><td>2.06</td><td>2.26</td><td>2.94</td><td>2.11</td></tr><tr><td>SHBa</td><td>228,731</td><td>757</td><td>0.33</td><td>1.38</td><td>2.17</td><td>2.36</td><td>4.08</td><td>2.30</td></tr><tr><td>SWEDa</td><td>221,307</td><td>1,011</td><td>0.46</td><td>2.58</td><td>2.90</td><td>3.21</td><td>5.69</td><td>2.00</td></tr><tr><td>SEBa</td><td>216,025</td><td>771</td><td>0.36</td><td>2.67</td><td>3.19</td><td>3.30</td><td>5.20</td><td>1.93</td></tr><tr><td>ATCOa</td><td>183,324</td><td>839</td><td>0.46</td><td>2.32</td><td>3.04</td><td>3.23</td><td>5.12</td><td>2.29</td></tr><tr><td>ASSAb</td><td>145,878</td><td>529</td><td>0.36</td><td>1.23</td><td>2.36</td><td>2.51</td><td>3.52</td><td>2.28</td></tr><tr><td>VOLVb</td><td>136,816</td><td>1,099</td><td>0.80</td><td>2.98</td><td>3.24</td><td>3.34</td><td>5.71</td><td>1.91</td></tr><tr><td>INVEb</td><td>129,676</td><td>590</td><td>0.46</td><td>1.79</td><td>2.43</td><td>2.62</td><td>4.12</td><td>1.80</td></tr><tr><td>SCAb</td><td>104,559</td><td>632</td><td>0.60</td><td>2.91</td><td>3.42</td><td>3.59</td><td>5.13</td><td>2.13</td></tr><tr><td>SAND</td><td>95,835</td><td>798</td><td>0.83</td><td>3.27</td><td>3.67</td><td>3.74</td><td>6.55</td><td>2.12</td></tr><tr><td>SCVb</td><td>78,800</td><td>825</td><td>1.05</td><td>2.65</td><td>3.66</td><td>4.75</td><td>6.75</td><td>1.91</td></tr><tr><td>ATCOb</td><td>78,395</td><td>262</td><td>0.33</td><td>2.55</td><td>3.88</td><td>4.09</td><td>5.52</td><td>1.85</td></tr><tr><td>SKFb</td><td>68,879</td><td>684</td><td>0.99</td><td>3.14</td><td>3.63</td><td>3.85</td><td>6.07</td><td>2.24</td></tr><tr><td>ELUXb</td><td>68,807</td><td>471</td><td>0.68</td><td>2.24</td><td>3.16</td><td>3.29</td><td>5.05</td><td>2.31</td></tr><tr><td>SKAb</td><td>67,160</td><td>320</td><td>0.48</td><td>3.07</td><td>3.63</td><td>3.77</td><td>4.89</td><td>1.90</td></tr><tr><td>ALFA</td><td>62,205</td><td>463</td><td>0.75</td><td>3.42</td><td>4.06</td><td>4.10</td><td>6.04</td><td>2.05</td></tr><tr><td>KINVb</td><td>60,097</td><td>337</td><td>0.56</td><td>1.95</td><td>3.61</td><td>3.98</td><td>7.95</td><td>2.26</td></tr><tr><td>SWMA</td><td>49,082</td><td>337</td><td>0.69</td><td>2.04</td><td>3.10</td><td>3.32</td><td>4.38</td><td>2.24</td></tr><tr><td>TEL2b</td><td>40,403</td><td>334</td><td>0.83</td><td>2.64</td><td>3.21</td><td>3.51</td><td>5.97</td><td>2.12</td></tr><tr><td>GETIb</td><td>39,540</td><td>221</td><td>0.56</td><td>2.91</td><td>3.81</td><td>4.21</td><td>4.25</td><td>1.99</td></tr><tr><td>LUPE</td><td>34,964</td><td>586</td><td>1.68</td><td>4.08</td><td>5.65</td><td>5.68</td><td>16.53</td><td>1.91</td></tr><tr><td>BOL</td><td>34,326</td><td>538</td><td>1.57</td><td>4.05</td><td>4.87</td><td>4.90</td><td>7.88</td><td>2.06</td></tr><tr><td>SECUb</td><td>32,861</td><td>169</td><td>0.51</td><td>2.73</td><td>3.66</td><td>3.88</td><td>3.75</td><td>2.32</td></tr><tr><td>MTGb</td><td>15,369</td><td>155</td><td>1.01</td><td>2.05</td><td>4.07</td><td>4.77</td><td>7.46</td><td>2.17</td></tr><tr><td>SSABa</td><td>13,877</td><td>370</td><td>2.67</td><td>1.61</td><td>3.82</td><td>4.14</td><td>8.89</td><td>1.76</td></tr></table>

## Table 2: The cross-section of HFT performance

This table reports descriptive statistics on HFT performance and trading characteristics in the cross-section of HFT firms. The following variables underlying the statistics are first aggregated for each day over all stocks and venues and then averaged across time for each HFT; the resulting crosssectional distribution across HFT firms is then presented. Revenues is the average daily trading revenue for each HFT firm, calculated as cash received from selling shares, minus the cash paid from buying shares, plus the value of any outstanding positions at the end-of-day marked to the market price at close; Trading Volume is the average daily trading volume for each HFT firm, measured in MSEK; Revenues per MSEK Traded is daily Revenues divided by daily Trading Volume for each HFT firm; Returns is daily Revenues divided by the maximum intraday inventory position over the entire sample (used as a measure of capitalization) and reported in annualized terms; Sharpe Ratio is the average monthly ratio for each HFT firm, reported in annualized terms, of the average daily return divided by the standard deviation of daily returns; the 1-factor Alpha is the intercept estimated in a regression of daily HFT excess returns on the market return factor; the 3-factor Alpha is the intercept estimated in a regression of daily HFT excess returns on the Fama-French factors; the 4-factor Alpha is the intercept estimated in a regression of daily HFT excess returns on the Fama-French and Carhart momentum factors; End-of-Day Inventory Ratio is the absolute end-of-day SEK position (netted across stocks) divided by the Trading Volume; Max. Intraday Inventory Ratio is the maximum absolute intraday SEK inventory position divided by the daily Trading Volume; Investment Horizon is the median holding time in seconds across all trades, calculated on a first-in-first-out basis; Aggressiveness Ratio is the SEK volume traded using market orders divided by the Trading Volume; and Decision Latency is the 0.1% quantile of a distribution of latencies recorded in each firm-month where a passive trade is followed by an active trade at the same venue, in the same stock, within one second (measured in microseconds elapsed between the two trades of each event), averaged across months for each HFT firm. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). 

<table><tr><td></td><td>Mean</td><td>Std. Dev.</td><td>p10</td><td>p25</td><td>p50</td><td>p75</td><td>p90</td></tr><tr><td>Revenues (SEK)</td><td>18,181</td><td>29,519</td><td>-7,572</td><td>-487</td><td>6,990</td><td>31,968</td><td>61,354</td></tr><tr><td>Revenues per MSEK Traded</td><td>153.2</td><td>504.7</td><td>-257.9</td><td>-43.7</td><td>56.5</td><td>147.2</td><td>472.2</td></tr><tr><td>Returns</td><td>0.29</td><td>0.42</td><td>-0.09</td><td>0.01</td><td>0.09</td><td>0.51</td><td>0.89</td></tr><tr><td>Sharpe Ratio</td><td>4.16</td><td>6.58</td><td>-1.47</td><td>0.33</td><td>1.61</td><td>7.02</td><td>11.14</td></tr><tr><td>1-factor Alpha</td><td>0.29</td><td>0.43</td><td>-0.08</td><td>0.01</td><td>0.10</td><td>0.51</td><td>0.90</td></tr><tr><td>3-factor Alpha</td><td>0.29</td><td>0.43</td><td>-0.07</td><td>0.01</td><td>0.09</td><td>0.51</td><td>0.94</td></tr><tr><td>4-factor Alpha</td><td>0.29</td><td>0.43</td><td>-0.06</td><td>0.01</td><td>0.09</td><td>0.51</td><td>0.94</td></tr><tr><td>Trading Volume (MSEK)</td><td>272.0</td><td>378.1</td><td>4.2</td><td>7.4</td><td>63.7</td><td>507.7</td><td>909.2</td></tr><tr><td>End-of-Day Inventory Ratio</td><td>0.23</td><td>0.23</td><td>0.01</td><td>0.02</td><td>0.13</td><td>0.33</td><td>0.63</td></tr><tr><td>Max Intraday Inventory Ratio</td><td>0.28</td><td>0.25</td><td>0.03</td><td>0.07</td><td>0.18</td><td>0.41</td><td>0.70</td></tr><tr><td>Investment Horizon (seconds)</td><td>88.9</td><td>119.9</td><td>3.7</td><td>5.7</td><td>54.9</td><td>137.3</td><td>227.9</td></tr><tr><td>Aggressive Ratio</td><td>0.51</td><td>0.26</td><td>0.16</td><td>0.28</td><td>0.56</td><td>0.69</td><td>0.88</td></tr><tr><td>Decision Latency (microseconds)</td><td>86,859</td><td>168,632</td><td>42</td><td>209</td><td>22,522</td><td>48,472</td><td>508,869</td></tr></table>


(N = 16 firms) 


## Table 3: Trading revenues, costs, and profits from public filings

This table reports Trading Revenues, Trading Costs, Trading Profit Margins, and Trading Returns calculated from annual reports and IPO prospectuses for five high-frequency trading firms for which public data is available. Trading Costs are broken down into several categories, all expressed as a percent of trading revenues. Trading Profit Margin is calculated as (1 - Trading Costs), and Trading Returns are calculated two ways based on two capitalization measures: as Trading Revenues / (Trading Assets Minus Trading Liabilities) and as (Trading Revenues / Book Equity). All quantities are in million USD, except for the firm Flow Traders, which is in million EUR. 

<table><tr><td rowspan="2"></td><td colspan="5">Virtu</td><td colspan="3">KCG</td><td colspan="4">GETCO</td><td colspan="4">Flow Traders</td><td>Jump</td></tr><tr><td>2015</td><td>2014</td><td>2013</td><td>2012</td><td>2011</td><td>2015</td><td>2014</td><td>2013</td><td>2012*</td><td>2011</td><td>2010</td><td>2009</td><td>2015</td><td>2014</td><td>2013</td><td>2012</td><td>2010</td></tr><tr><td>Trading Revenues (in millions)</td><td>757.5</td><td>685.2</td><td>623.7</td><td>581.5</td><td>449.4</td><td>1,179.9</td><td>1,274.4</td><td>903.8</td><td>526.6</td><td>896.5</td><td>865.1</td><td>955.2</td><td>400.1</td><td>240.8</td><td>200.5</td><td>125.1</td><td>511.6</td></tr><tr><td>-- % of revenue from proprietary trading</td><td>95.1%</td><td>98.5%</td><td>98.4%</td><td>100%</td><td>100%</td><td>73.8%</td><td>68.5%</td><td>67.0%</td><td>89.9%</td><td>94.2%</td><td></td><td></td><td></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>Trading Costs (as % of Trading Revenue)</td><td>54.7%</td><td>60.0%</td><td>57.8%</td><td>72.6%</td><td>62.1%</td><td>51.3%</td><td>52.4%</td><td>59.0%</td><td>62.5%</td><td>48.5%</td><td>48.6%</td><td>40.4%</td><td>35.5%</td><td>41.6%</td><td>43.7%</td><td>47.5%</td><td></td></tr><tr><td>-- Brokerage, exchange and clearance fees</td><td>30.7%</td><td>33.7%</td><td>31.3%</td><td>34.5%</td><td>32.9%</td><td>22.5%</td><td>23.9%</td><td>27.3%</td><td>35.3%</td><td>32.2%</td><td>35.1%</td><td>32.1%</td><td>{ 14.2%</td><td>15.7%</td><td>15.8%</td><td>14.8%</td><td></td></tr><tr><td>-- Communication and data processing</td><td>9.0%</td><td>10.0%</td><td>10.4%</td><td>9.5%</td><td>10.3%</td><td>11.8%</td><td>11.8%</td><td>13.7%</td><td>17.2%</td><td>9.7%</td><td>7.1%</td><td>4.5%</td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>-- Equipment rentals, depreciation and amortization</td><td>4.4%</td><td>4.5%</td><td>4.0%</td><td>15.7%</td><td>11.1%</td><td>10.2%</td><td>10.4%</td><td>11.0%</td><td>9.1%</td><td>6.2%</td><td>6.2%</td><td>3.8%</td><td>1.6%</td><td>1.8%</td><td>1.9%</td><td>2.4%</td><td></td></tr><tr><td>-- Net interest &amp; dividends on securities paid (on credit lines, securities borrowing, etc.)</td><td>7.1%</td><td>8.6%</td><td>7.8%</td><td>7.1%</td><td>6.0%</td><td>6.1%</td><td>5.4%</td><td>6.5%</td><td>1.0%</td><td>0.3%</td><td>0.1%</td><td>0.0%</td><td>9.7%</td><td>12.5%</td><td>12.8%</td><td>12.3%</td><td></td></tr><tr><td>-- Other trading costs (administrative &amp; technical costs, other overhead, etc.)</td><td>3.4%</td><td>3.2%</td><td>4.4%</td><td>5.8%</td><td>1.8%</td><td>0.7%</td><td>0.8%</td><td>0.5%</td><td>0.0%</td><td>0.0%</td><td>0.0%</td><td>0.0%</td><td>10.1%</td><td>11.5%</td><td>13.3%</td><td>18.0%</td><td></td></tr><tr><td>Trading Profit Margin</td><td>45.3%</td><td>40.0%</td><td>42.2%</td><td>27.4%</td><td>37.9%</td><td>48.7%</td><td>47.6%</td><td>41.0%</td><td>37.5%</td><td>51.5%</td><td>51.4%</td><td>59.6%</td><td>64.5%</td><td>58.4%</td><td>56.3%</td><td>52.5%</td><td>52.3%***</td></tr><tr><td>Trading Revenue / (Trading Assets Minus Trading Liabilities)**</td><td>183%</td><td>228%</td><td>196%</td><td>184%</td><td></td><td>96%</td><td>96%</td><td>60%</td><td>62%</td><td></td><td></td><td></td><td>114%</td><td>118%</td><td>119%</td><td>103%</td><td>237%</td></tr><tr><td>Trading Revenue / (Book Equity)</td><td>136%</td><td>135%</td><td>138%</td><td>84%</td><td></td><td>82%</td><td>84%</td><td>60%</td><td>80%</td><td></td><td></td><td></td><td>162%</td><td>169%</td><td>146%</td><td>123%</td><td>222%</td></tr></table>

* Does not include any costs associated with the December 19, 2012 merger agreement with Knight, such as any costs related to the Knight August 1, 2012 incident ** Trading asset include cash and cash equivalents, financial instruments owned, receivables from broker-dealers and clearing organizations, and collateralized agreements. Trading liabilities include short-term borrowings, collateralized financing, financial instruments sold and not yet purchased, payables to broker-dealers and clearing organizations, and other accounts payable. 

*** Total profit margin 

## Table 4: Trading performance and latency

This table analyzes the relationship between trading performance and latency. It reports coefficients estimated from Eq. (1) for five performance measures as dependent variables: Revenues, Returns, Sharpe Ratio, Trading Volume, and Revenues per MSEK Traded (all defined as in Table 2). Revenue, Returns, Revenues per MSEK Traded, and Trading Volume are calculated at a daily level for each HFT firm aggregated across stocks and then averaged across trading days in each month to get firm-month observations; and the Sharpe Ratio is calculated as firm-month observations using the mean and standard deviation of daily observations of Revenues aggregated across stocks. We estimate OLS regressions with month fixed effects. The independent variables considered are as follows: log(Decision Latency) is the natural logarithm of Decision Latency (defined as in Table 2). Top 1 and Top 1-5 are indicator variables for whether a given firm is ranked among the top 1 or top 1-5 firms by Decision Latency in a given month. The End-of-Day Inventory Ratio, Max. Intraday Inventory Ratio, Investment Horizon, and the Aggressiveness Ratio are defined as in Table 2. All continuous independent variables are in units of standard deviations. We omit Max. Intraday Inventory Ratio as a control when estimating Returns as the dependent variable, because Max. Intraday Inventory ratio is used in the denominator to calculate returns. *, ** and *** correspond to statistical significance at the 10%, 5%, and 1%, respectively. Standard errors are dually clustered by firm and month and are reported in parentheses. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). 

<table><tr><td></td><td colspan="3">Revenues</td><td colspan="3">Returns</td><td colspan="3">Sharpe Ratio</td><td colspan="3">Trading Volume (x 10-6)</td><td colspan="3">Revenues per MSEK Traded</td></tr><tr><td rowspan="2">log(Decision Latency)</td><td>-14020***</td><td>-1063</td><td>9925</td><td>-.221***</td><td>-.059</td><td>-.00349</td><td>-4.38***</td><td>-1</td><td>2.03</td><td>-247***</td><td>-89.7</td><td>10.5</td><td>-19.4</td><td>-10.7</td><td>101**</td></tr><tr><td>(4311)</td><td>(6358)</td><td>(10481)</td><td>(.0483)</td><td>(.065)</td><td>(.0852)</td><td>(.632)</td><td>(1.2)</td><td>(1.46)</td><td>(43.7)</td><td>(59.1)</td><td>(74)</td><td>(57.5)</td><td>(69.1)</td><td>(40.4)</td></tr><tr><td rowspan="2">Top 1</td><td></td><td>29849*</td><td>24639**</td><td></td><td>.238*</td><td>.252*</td><td></td><td>3.77*</td><td>4.2*</td><td></td><td>326***</td><td>281***</td><td></td><td>6.99</td><td>57.6*</td></tr><tr><td></td><td>(15251)</td><td>(12249)</td><td></td><td>(.134)</td><td>(.142)</td><td></td><td>(2.21)</td><td>(2.29)</td><td></td><td>(97.9)</td><td>(104)</td><td></td><td>(51.7)</td><td>(32.8)</td></tr><tr><td rowspan="2">Top 1-5</td><td></td><td>24074**</td><td>15451*</td><td></td><td>.333**</td><td>.303**</td><td></td><td>7.29**</td><td>5.61**</td><td></td><td>301**</td><td>201**</td><td></td><td>19.4</td><td>44.1</td></tr><tr><td></td><td>(11619)</td><td>(8009)</td><td></td><td>(.155)</td><td>(.133)</td><td></td><td>(3.24)</td><td>(2.63)</td><td></td><td>(132)</td><td>(97.4)</td><td></td><td>(93.3)</td><td>(55.9)</td></tr><tr><td rowspan="2">End-of-Day Inv.</td><td></td><td></td><td>2921</td><td></td><td></td><td>.0839*</td><td></td><td></td><td>2***</td><td></td><td></td><td>-33.9**</td><td></td><td></td><td>326*</td></tr><tr><td></td><td></td><td>(3774)</td><td></td><td></td><td>(.0494)</td><td></td><td></td><td>(.74)</td><td></td><td></td><td>(15.9)</td><td></td><td></td><td>(168)</td></tr><tr><td rowspan="2">Max Intraday Inv.</td><td></td><td></td><td>-21008**</td><td></td><td></td><td>[omitted]</td><td></td><td></td><td>-3.74***</td><td></td><td></td><td>-183***</td><td></td><td></td><td>-76.3</td></tr><tr><td></td><td></td><td>(8579)</td><td></td><td></td><td></td><td></td><td></td><td>(1.23)</td><td></td><td></td><td>(65.3)</td><td></td><td></td><td>(127)</td></tr><tr><td rowspan="2">Investment Horizon</td><td></td><td></td><td>-5401</td><td></td><td></td><td>-.134***</td><td></td><td></td><td>-2.25***</td><td></td><td></td><td>-76.4</td><td></td><td></td><td>-73.3</td></tr><tr><td></td><td></td><td>(5994)</td><td></td><td></td><td>(.0404)</td><td></td><td></td><td>(.726)</td><td></td><td></td><td>(50.3)</td><td></td><td></td><td>(63.8)</td></tr><tr><td rowspan="2">Aggressive Ratio</td><td></td><td></td><td>5481</td><td></td><td></td><td>-.0212</td><td></td><td></td><td>-.779</td><td></td><td></td><td>41.7</td><td></td><td></td><td>-55.5</td></tr><tr><td></td><td></td><td>(3865)</td><td></td><td></td><td>(.0558)</td><td></td><td></td><td>(.823)</td><td></td><td></td><td>(28.8)</td><td></td><td></td><td>(65.8)</td></tr><tr><td rowspan="2">Constant</td><td>20278***</td><td>8466**</td><td>10894**</td><td>.254***</td><td>.104*</td><td>.107**</td><td>5.1***</td><td>1.94</td><td>2.26*</td><td>313***</td><td>169***</td><td>198***</td><td>35.2</td><td>27</td><td>7.91</td></tr><tr><td>(6973)</td><td>(4189)</td><td>(4885)</td><td>(.0579)</td><td>(.0587)</td><td>(.0513)</td><td>(1.26)</td><td>(1.23)</td><td>(1.23)</td><td>(75.9)</td><td>(57.8)</td><td>(56.3)</td><td>(57.3)</td><td>(80.2)</td><td>(10)</td></tr><tr><td>Month FEs</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr><tr><td>R-squared</td><td>0.123</td><td>0.168</td><td>0.263</td><td>0.198</td><td>0.233</td><td>0.269</td><td>0.207</td><td>0.254</td><td>0.361</td><td>0.294</td><td>0.362</td><td>0.454</td><td>0.080</td><td>0.080</td><td>0.148</td></tr><tr><td>N</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td></tr></table>

## Table 5: Relative latency and trading performance around colocation upgrades

This table examines the relationship between trading performance and latency around two colocation upgrades on March 14, 2011 and September 17, 2012. Specifically, it analyzes two groups of HFT firms that experience a change in their latency rank around each event: firms that improve their rank in terms of Decision Latency are in the Faster group, and firms that decline their rank are in the Slower group. The table then reports the change in average trading performance around the colocation events. The trading measures Revenue, Returns, Revenues per MSEK Traded, and Trading Volume are calculated at a daily level for each HFT and then averaged across trading days and HFTs for each period and group; and the Sharpe Ratio is calculated using the mean and standard deviation of daily observations of Revenues. The difference between the Before and After periods are reported for each group and each variable. The bottom row of the table reports the difference-in-difference estimate between groups. We test the null hypothesis that there is no difference in the before-after change between the Faster and Slower groups; the statistical significance of the difference-in-difference estimates is assessed with a t-test, where a p-value is computed under the null by taking the before-after changes in performance for each HFT firm as independent observations, pooling together the Faster and Slower groups (there are N = 7 firms with changing relative latency, yielding six degrees of freedom). 

<table><tr><td rowspan="2">HFT latency rank</td><td colspan="4">Revenues</td><td colspan="4">Returns</td><td colspan="4">Sharpe Ratio</td></tr><tr><td>Before</td><td>After</td><td>Diff.</td><td>(S.E.)</td><td>Before</td><td>After</td><td>Diff.</td><td>(S.E.)</td><td>Before</td><td>After</td><td>Diff.</td><td>(S.E.)</td></tr><tr><td>Faster</td><td>9,537</td><td>52,770</td><td>43,233</td><td>(14,841)</td><td>0.022</td><td>0.158</td><td>0.136</td><td>(0.055)</td><td>1.47</td><td>1.68</td><td>0.20</td><td>(0.46)</td></tr><tr><td>Slower</td><td>31,557</td><td>32,811</td><td>1,255</td><td>(2,608)</td><td>0.777</td><td>0.748</td><td>-0.030</td><td>(0.067)</td><td>5.50</td><td>4.70</td><td>-0.81</td><td>(0.99)</td></tr><tr><td>Diff-in-diff</td><td></td><td></td><td>41,978***</td><td>(6,533)</td><td></td><td></td><td>0.165**</td><td>(0.045)</td><td></td><td></td><td>1.01*</td><td>(0.50)</td></tr></table>

<table><tr><td rowspan="2">HFT latency rank</td><td colspan="4">Trading Volume (x 10-6)</td><td colspan="4">Revenues per MSEK Traded</td></tr><tr><td>Before</td><td>After</td><td>Diff.</td><td>(S.E.)</td><td>Before</td><td>After</td><td>Diff.</td><td>(S.E.)</td></tr><tr><td>Faster</td><td>415.9</td><td>537.4</td><td>121.5</td><td>(101.8)</td><td>-21.3</td><td>87.7</td><td>109.0</td><td>(33.9)</td></tr><tr><td>Slower</td><td>448.6</td><td>398.1</td><td>-50.5</td><td>(43.1)</td><td>207.3</td><td>282.2</td><td>74.9</td><td>(65.2)</td></tr><tr><td>Diff-in-diff</td><td></td><td></td><td>171.9**</td><td>(50.1)</td><td></td><td></td><td>34.1</td><td>(40)</td></tr></table>

## Table 6: Alternative latency measures

This table is similar to Table 4 but analyzes two alternative latency measures: Queuing Latency (Panel A), which counts the cases where an HFT firm captures the topof-queue position in a limit-order book gap; and Mean Latency (Panel B), the mean of a distribution of latencies in each firm-month where a passive trade is followed by an active trade at the same venue, in the same stock, within one millisecond. The construction of these alternative latency measures and their relationship to HFT strategies is discussed in Section IV.C. As in Table 4, the table reports coefficients estimated from Eq. (1) for five performance measures as dependent variables: Revenues, Returns, Sharpe Ratio, Trading Volume, and Revenues per MSEK Traded. We estimate OLS regressions with month fixed effects. In Panel A, log(Queuing Latency + 1) is the natural logarithm of Queuing Latency + 1, and, in Panel B, log(Mean Latency), is the natural logarithm of Mean Latency. Top 1 and Top 1-5 are indicator variables for whether a given firm is ranked among the top 1 or top 1-5 firms by the corresponding latency measure. All other independent variables are as in Table 4. *, ** and *** correspond to statistical significance at the 10%, 5%, and 1%, respectively. Standard errors are dually clustered by firm and month and reported in parentheses. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). 


Panel A: Queuing Latency and trading performance


<table><tr><td></td><td colspan="3">Revenues</td><td colspan="3">Returns</td><td colspan="3">Sharpe Ratio</td><td colspan="3">Trading Volume (x 10-6)</td><td colspan="3">Revenues per MSEK Traded</td></tr><tr><td rowspan="2">log(Queuing Latency + 1)</td><td>16761***</td><td>4150</td><td>-8265</td><td>.281***</td><td>.176***</td><td>.121*</td><td>5.43***</td><td>2.94***</td><td>-.283</td><td>288***</td><td>133**</td><td>34.8</td><td>32.9</td><td>38.1</td><td>-95</td></tr><tr><td>(4608)</td><td>(4907)</td><td>(11994)</td><td>(.0533)</td><td>(.0529)</td><td>(.0671)</td><td>(.72)</td><td>(1.12)</td><td>(1.43)</td><td>(39.6)</td><td>(56.7)</td><td>(102)</td><td>(58.6)</td><td>(77.1)</td><td>(62.1)</td></tr><tr><td rowspan="2">Top 1</td><td></td><td>50803***</td><td>51684***</td><td></td><td>.463**</td><td>.471**</td><td></td><td>11.9***</td><td>12.6***</td><td></td><td>601***</td><td>603***</td><td></td><td>-9.21</td><td>35.5</td></tr><tr><td></td><td>(18676)</td><td>(15865)</td><td></td><td>(.228)</td><td>(.218)</td><td></td><td>(2.4)</td><td>(2.13)</td><td></td><td>(126)</td><td>(119)</td><td></td><td>(75.9)</td><td>(75.6)</td></tr><tr><td rowspan="2">Top 1-5</td><td></td><td>13698*</td><td>9563</td><td></td><td>.102</td><td>.127</td><td></td><td>2.13</td><td>2.39</td><td></td><td>176*</td><td>128</td><td></td><td>-9.11</td><td>87.7</td></tr><tr><td></td><td>(7180)</td><td>(7400)</td><td></td><td>(.123)</td><td>(.136)</td><td></td><td>(1.74)</td><td>(1.88)</td><td></td><td>(99.9)</td><td>(87.4)</td><td></td><td>(125)</td><td>(66.2)</td></tr><tr><td rowspan="2">End-of-Day Inv.</td><td></td><td></td><td>2718</td><td></td><td></td><td>.0858*</td><td></td><td></td><td>1.95**</td><td></td><td></td><td>-32.5*</td><td></td><td></td><td>325*</td></tr><tr><td></td><td></td><td>(3742)</td><td></td><td></td><td>(.0508)</td><td></td><td></td><td>(.767)</td><td></td><td></td><td>(18.1)</td><td></td><td></td><td>(170)</td></tr><tr><td rowspan="2">Max Intraday Inv.</td><td></td><td></td><td>-19571**</td><td></td><td></td><td></td><td></td><td></td><td>-2.9**</td><td></td><td></td><td>-151**</td><td></td><td></td><td>-58.6</td></tr><tr><td></td><td></td><td>(8658)</td><td></td><td></td><td></td><td></td><td></td><td>(1.25)</td><td></td><td></td><td>(68.5)</td><td></td><td></td><td>(129)</td></tr><tr><td rowspan="2">Investment Horizon</td><td></td><td></td><td>-4950</td><td></td><td></td><td>-.0917***</td><td></td><td></td><td>-1.96**</td><td></td><td></td><td>-60.5</td><td></td><td></td><td>-72.8</td></tr><tr><td></td><td></td><td>(7114)</td><td></td><td></td><td>(.0333)</td><td></td><td></td><td>(.846)</td><td></td><td></td><td>(60.8)</td><td></td><td></td><td>(62.1)</td></tr><tr><td rowspan="2">Aggressive Ratio</td><td></td><td></td><td>6664</td><td></td><td></td><td>.00695</td><td></td><td></td><td>-.442</td><td></td><td></td><td>60.3*</td><td></td><td></td><td>-51.4</td></tr><tr><td></td><td></td><td>(4551)</td><td></td><td></td><td>(.0428)</td><td></td><td></td><td>(.617)</td><td></td><td></td><td>(33.9)</td><td></td><td></td><td>(65.8)</td></tr><tr><td rowspan="2">Constant</td><td>20223***</td><td>10893**</td><td>11153**</td><td>.252***</td><td>.176***</td><td>.16***</td><td>5.08***</td><td>3.32***</td><td>2.91**</td><td>313***</td><td>197***</td><td>203***</td><td>34.8</td><td>39.1</td><td>-7.21</td></tr><tr><td>(6685)</td><td>(5372)</td><td>(4814)</td><td>(.0509)</td><td>(.0557)</td><td>(.0496)</td><td>(1.13)</td><td>(1.28)</td><td>(1.19)</td><td>(72.2)</td><td>(67.7)</td><td>(58.2)</td><td>(56.6)</td><td>(96.2)</td><td>(45.5)</td></tr><tr><td>Month FEs</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr><tr><td>R-squared</td><td>0.152</td><td>0.213</td><td>0.302</td><td>0.267</td><td>0.300</td><td>0.323</td><td>0.285</td><td>0.357</td><td>0.429</td><td>0.377</td><td>0.474</td><td>0.547</td><td>0.080</td><td>0.080</td><td>0.146</td></tr><tr><td>N</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td></tr></table>


Panel B: Mean Latency and trading performance


<table><tr><td></td><td colspan="3">Revenues</td><td colspan="3">Returns</td><td colspan="3">Sharpe Ratio</td><td colspan="3">Trading Volume (x 10-6)</td><td colspan="3">Revenues per MSEK Traded</td></tr><tr><td rowspan="2">log(Mean Latency)</td><td>-10796***</td><td>3261</td><td>7350</td><td>-.14***</td><td>.00246</td><td>.0247</td><td>-3***</td><td>-.0674</td><td>1.06</td><td>-160***</td><td>-32.7</td><td>17.7</td><td>-5.42</td><td>22.9</td><td>50.3</td></tr><tr><td>(3456)</td><td>(6724)</td><td>(5858)</td><td>(.0523)</td><td>(.0918)</td><td>(.0913)</td><td>(.904)</td><td>(1.74)</td><td>(1.61)</td><td>(58.9)</td><td>(93.6)</td><td>(77.5)</td><td>(42.5)</td><td>(54)</td><td>(73.4)</td></tr><tr><td rowspan="2">Top 1</td><td></td><td>12076</td><td>19574</td><td></td><td>-.0658</td><td>.0144</td><td></td><td>-2.99</td><td>-.038</td><td></td><td>-220</td><td>-116</td><td></td><td>60.9</td><td>151</td></tr><tr><td></td><td>(26687)</td><td>(20144)</td><td></td><td>(.274)</td><td>(.263)</td><td></td><td>(4.63)</td><td>(4.02)</td><td></td><td>(216)</td><td>(148)</td><td></td><td>(93.1)</td><td>(142)</td></tr><tr><td rowspan="2">Top 1-5</td><td></td><td>33497***</td><td>13819</td><td></td><td>.433***</td><td>.301**</td><td></td><td>9.69***</td><td>4.69*</td><td></td><td>465***</td><td>216**</td><td></td><td>49.4</td><td>-40.7</td></tr><tr><td></td><td>(10315)</td><td>(10857)</td><td></td><td>(.148)</td><td>(.142)</td><td></td><td>(3)</td><td>(2.45)</td><td></td><td>(115)</td><td>(109)</td><td></td><td>(122)</td><td>(71.7)</td></tr><tr><td rowspan="2">End-of-Day Inv.</td><td></td><td></td><td>2352</td><td></td><td></td><td>.0737*</td><td></td><td></td><td>1.83**</td><td></td><td></td><td>-40.3**</td><td></td><td></td><td>322*</td></tr><tr><td></td><td></td><td>(3909)</td><td></td><td></td><td>(.0442)</td><td></td><td></td><td>(.746)</td><td></td><td></td><td>(17.5)</td><td></td><td></td><td>(167)</td></tr><tr><td rowspan="2">Max Intraday Inv.</td><td></td><td></td><td>-19668***</td><td></td><td></td><td></td><td></td><td></td><td>-3.65***</td><td></td><td></td><td>-217***</td><td></td><td></td><td>-52.1</td></tr><tr><td></td><td></td><td>(6100)</td><td></td><td></td><td></td><td></td><td></td><td>(.999)</td><td></td><td></td><td>(51.1)</td><td></td><td></td><td>(117)</td></tr><tr><td rowspan="2">Investment Horizon</td><td></td><td></td><td>-4960</td><td></td><td></td><td>-.171***</td><td></td><td></td><td>-2.19***</td><td></td><td></td><td>-82.3*</td><td></td><td></td><td>-69</td></tr><tr><td></td><td></td><td>(5628)</td><td></td><td></td><td>(.0469)</td><td></td><td></td><td>(.743)</td><td></td><td></td><td>(46.1)</td><td></td><td></td><td>(61.1)</td></tr><tr><td rowspan="2">Aggressive Ratio</td><td></td><td></td><td>6898**</td><td></td><td></td><td>-.0214</td><td></td><td></td><td>-.468</td><td></td><td></td><td>54.6**</td><td></td><td></td><td>-48.5</td></tr><tr><td></td><td></td><td>(3469)</td><td></td><td></td><td>(.0521)</td><td></td><td></td><td>(.764)</td><td></td><td></td><td>(25.3)</td><td></td><td></td><td>(61.5)</td></tr><tr><td rowspan="2">Constant</td><td>20554***</td><td>7620</td><td>12494</td><td>.258***</td><td>.109</td><td>.137**</td><td>5.19***</td><td>1.96</td><td>3.14**</td><td>319***</td><td>170*</td><td>230***</td><td>35.7</td><td>13.3</td><td>32.6</td></tr><tr><td>(7076)</td><td>(8590)</td><td>(8466)</td><td>(.0704)</td><td>(.0809)</td><td>(.0658)</td><td>(1.44)</td><td>(1.7)</td><td>(1.4)</td><td>(83.9)</td><td>(95.4)</td><td>(88.6)</td><td>(57.5)</td><td>(98.7)</td><td>(45)</td></tr><tr><td>Month FEs</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr><tr><td>R-squared</td><td>0.093</td><td>0.142</td><td>0.253</td><td>0.128</td><td>0.182</td><td>0.236</td><td>0.124</td><td>0.219</td><td>0.345</td><td>0.146</td><td>0.266</td><td>0.423</td><td>0.079</td><td>0.080</td><td>0.147</td></tr><tr><td>N</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td></tr></table>

## Table 7: Price impact, realized spread and latency

This table examines the relationship between Decision Latency and two dependent variables: active Price Impact and passive Realized Spread. Price Impact is the basis point change in spread midpoint from just before to ten seconds after a trade initiated by an HFT firm. Realized Spread is the basis point difference between the transaction price and the bid-ask spread midpoint ten seconds after a trade where an HFT firm was the liquidity provider. Top 1 and Top 1-5 are indicator variables for whether a given firm is ranked among the top 1 or top 1-5 firms by speed in a given month. Decision Latency, Average End-of-Day Inventory, Maximum Intraday Inventory, Investment Horizon, and the Aggressive Ratio are defined as in Table 2. We also control for the following stock-month-specific variables: Volatility, Fragmentation Index, Tick Size, Quoted Spread (all defined as in Table 1), and Non-HFT Trading Vol., which is the SEK trading volume recorded by non-HFT brokers. All continuous variables are in units of standard deviations. *, ** and *** correspond to p-values lower than 10%, 5%, and 1%, respectively. Standard errors are dually clustered by firm-stock and month and are reported in the parentheses. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014); stock-firm-month observations for which an HFT firm does not trade actively or passively are excluded. 

<table><tr><td></td><td colspan="2">Price Impact</td><td colspan="2">Realized Spread</td></tr><tr><td>log(Decision Latency)</td><td>-.318(.225)</td><td>-.494*(.212)</td><td>-.364***(.0982)</td><td>-.384***(.0958)</td></tr><tr><td>Top 1</td><td>.371*(.201)</td><td>.337*(.193)</td><td>.0214(.131)</td><td>.0599(.126)</td></tr><tr><td>Top 1-5</td><td>.73**(.362)</td><td>.645**(.315)</td><td>.448***(.136)</td><td>.477***(.118)</td></tr><tr><td>Avg. End-of-Day Inv.</td><td></td><td>.106(.158)</td><td></td><td>.00393(.0655)</td></tr><tr><td>Max. Intraday Inv.</td><td></td><td>.256(.216)</td><td></td><td>.0866(.0663)</td></tr><tr><td>Investment Horizon</td><td></td><td>-.158(.182)</td><td></td><td>-.0467(.0678)</td></tr><tr><td>Aggressiveness Ratio</td><td></td><td>.0103(.121)</td><td></td><td>-.0544(.0581)</td></tr><tr><td>Non-HFT Trading Vol.</td><td></td><td>-.100(.162)</td><td></td><td>.145**(.0618)</td></tr><tr><td>Volatility</td><td></td><td>-.226(.161)</td><td></td><td>-.462**(.217)</td></tr><tr><td>Fragmentation Index</td><td></td><td>-.162*(.0966)</td><td></td><td>-.0943*(.0538)</td></tr><tr><td>Tick Size</td><td></td><td>-.0469(.301)</td><td></td><td>-.265*(.136)</td></tr><tr><td>Quoted Spread</td><td></td><td>.890**(.379)</td><td></td><td>.623***(.163)</td></tr><tr><td>Constant</td><td>3.91***(.182)</td><td>3.96***(.22)</td><td>-.0958(.084)</td><td>-.108(.107)</td></tr><tr><td>(Month x Stock) FEs</td><td>Yes</td><td>No</td><td>Yes</td><td>No</td></tr><tr><td>R-squared</td><td>0.196</td><td>0.016</td><td>0.158</td><td>0.017</td></tr><tr><td>N</td><td>11449</td><td>11449</td><td>11269</td><td>11269</td></tr></table>

## Table 8: Cross-market arbitrage and latency

This table reports probit regression estimates corresponding to the probability of initiating a trade (Active Trading; Panel A) or supplying liquidity in a trade (Passive Trading; Panel B) in the equity markets in response to a change in the futures index price. The dependent variable is 1 when a Fast HFT firm performs the trade and 0 if a Slow HFT does it. In each month, Slow HFTs are those who are not among the top five HFTs in terms of trading speed. Fast HFTs are either the top 1 or top 1-5 HFTs in terms of trading speed. Trades included in the analysis are those performed by HFTs in the sample stocks. A news event is defined as when the absolute return on the OMXS30 futures during a one-second window preceding the stock trade is “large” (in the top decile for each month among non-zero absolute returns). The variable News is +1 if the active party trades in the direction of the news, -1 if the active party trades in the opposite direction of the news, and zero if there is no news event in the one-second window before the trade. We include the following control variables: Lagged Volatility, the average second-by-second squared return (multiplied by 1,000) over the previous ten seconds; Lagged Volume, the SEK Trading Volume (divided by 100,000) over the previous ten seconds; Quoted Spread, the difference between the best bid and offer quotes (multiplied by 10,000), divided by the midpoint quote; Depth at BBO, the average number of shares available at the best bid quote and the best offer quote (divided by 100,000), multiplied by the midpoint quote. Marginal effects are also reported. Regressions are estimated monthby-month from January 2010 to December 2014; reported coefficients and marginal effects are means across the sixty month, and standard errors are in parentheses. *, ** and *** correspond to p-values lower than 10%, 5%, and 1%, respectively. 


Panel A: Active Trading


<table><tr><td rowspan="2"></td><td colspan="2">“Fast” = Top 1 HFT</td><td colspan="2">“Fast” = Top 1-5 HFT</td></tr><tr><td>Probit(1=Fast HFT)</td><td>Marginal effects</td><td>Probit(1=Fast HFT)</td><td>Marginal effects</td></tr><tr><td>Constant</td><td>1.055***(0.31)</td><td></td><td>2.143***(0.17)</td><td></td></tr><tr><td>News</td><td>0.139***(0.04)</td><td>0.006</td><td>0.199***(0.03)</td><td>0.008</td></tr><tr><td>Lagged Volatility</td><td>-0.094(0.08)</td><td>0.000</td><td>-0.007***(0.00)</td><td>-0.001</td></tr><tr><td>Lagged Volume</td><td>-0.005***(0.00)</td><td>0.000</td><td>-0.004***(0.00)</td><td>0.000</td></tr><tr><td>Quoted Spread</td><td>-0.046***(0.01)</td><td>-0.004</td><td>-0.035***(0.00)</td><td>-0.001</td></tr><tr><td>Depth at BBO</td><td>0.013(0.03)</td><td>0.006</td><td>0.049***(0.02)</td><td>0.001</td></tr><tr><td>Stock FEs</td><td>Yes</td><td></td><td>Yes</td><td></td></tr><tr><td>Average N</td><td>109684</td><td></td><td>277044</td><td></td></tr><tr><td>Avg. psuedo-R2</td><td>0.209</td><td></td><td>0.169</td><td></td></tr></table>


Panel B: Passive Trading


<table><tr><td colspan="2">“Fast” = Top 1 HFT</td><td colspan="2">“Fast” = Top 1-5 HFT</td></tr><tr><td>Probit(1=Fast HFT)</td><td>Marginal effects</td><td>Probit(1=Fast HFT)</td><td>Marginal effects</td></tr><tr><td>0.551*(0.30)</td><td></td><td>1.646***(0.15)</td><td></td></tr><tr><td>0.001(0.03)</td><td>0.004</td><td>-0.097***(0.02)</td><td>-0.015</td></tr><tr><td>-0.116(0.12)</td><td>0.001</td><td>0.008***(0.00)</td><td>0.001</td></tr><tr><td>0.001(0.00)</td><td>0.000</td><td>0.000(0.00)</td><td>0.000</td></tr><tr><td>-0.024(0.02)</td><td>-0.002</td><td>-0.001(0.00)</td><td>0.000</td></tr><tr><td>-0.120**(0.05)</td><td>-0.009</td><td>-0.015(0.02)</td><td>-0.003</td></tr><tr><td>Yes</td><td></td><td>Yes</td><td></td></tr><tr><td>95268</td><td></td><td>258409</td><td></td></tr><tr><td>0.204</td><td></td><td>0.163</td><td></td></tr></table>

## Table 9: Persistence of HFT performance

This table analyzes persistence in HFTs’ performance on both a daily (Panel A) and a monthly (Panel B) frequency. The persistence coefficient reported in the table is the � estimated in the regression model given in Eq. (3), where Performance can be one of the following dependent variables calculated on a daily basis for each HFT firm: Revenues, Returns, Sharpe Ratio, and Revenues per MSEK Traded (all defined as in Table 2). For the monthly frequency, each of the performance measures defined on a daily frequency are first averaged across trading days within each month. The Sharpe Ratio is considered only for the monthly regressions and is based on mean and standard deviation of daily observations of Revenues. The variables are either in units of standard deviations for each day or month (in each time period, firm-level performance is centered on the mean and scaled by standard deviation across HFTs) or on the rank order of the HFTs (from 1 to 16 based on performance). *, ** and *** correspond to p-values lower than 10%, 5%, and 1%, respectively. Standard errors are dually clustered by firm and day (or month for Panel B) and are reported in parentheses. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). 


Panel A: Daily persistence


<table><tr><td rowspan="2"></td><td colspan="3">Standardized</td><td colspan="3">Rank order</td></tr><tr><td>Revenues</td><td>Returns</td><td>Revenues per MSEK Traded</td><td>Revenues</td><td>Returns</td><td>Revenues per MSEK Traded</td></tr><tr><td>Lag dependent variable</td><td>.235***(0.087)</td><td>.387***(0.085)</td><td>.023(0.020)</td><td>.234***(0.067)</td><td>.283***(0.064)</td><td>.029*(0.018)</td></tr><tr><td>R-squared</td><td>0.057</td><td>0.157</td><td>0.016</td><td>0.114</td><td>0.143</td><td>0.076</td></tr><tr><td>N</td><td>10642</td><td>10642</td><td>10642</td><td>10642</td><td>10642</td><td>10642</td></tr></table>


Panel B: Monthly persistence


<table><tr><td rowspan="2"></td><td colspan="4">Standardized</td><td colspan="4">Rank order</td></tr><tr><td>Revenues</td><td>Returns</td><td>Sharpe Ratio</td><td>Revenues per MSEK Traded</td><td>Revenues</td><td>Returns</td><td>Sharpe Ratio</td><td>Revenues per MSEK Traded</td></tr><tr><td>Lag dependent variable</td><td>.631***(0.113)</td><td>.446***(0.155)</td><td>.763***(0.062)</td><td>.106(0.083)</td><td>.464***(0.091)</td><td>.539***(0.094)</td><td>.196**(0.095)</td><td>.134**(0.063)</td></tr><tr><td>R-squared</td><td>0.401</td><td>0.222</td><td>0.584</td><td>0.060</td><td>0.252</td><td>0.325</td><td>0.091</td><td>0.069</td></tr><tr><td>N</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td></tr></table>

## Table 10: Long-run trends in HFT concentration and industry-wide performance

This table reports long-run trends in various variables related to the HFT industry. Total Daily Revenues (Average Daily Revenues) is Revenues summed (averaged) across all HFTs, reported in SEK; Average Revenues per MSEK Traded is daily Revenues per MSEK Traded aggregated across HFTs; Daily Trading Volume is the daily Trading Volume summed across HFTs; Cost of HFT Activities for Non-HFTs is HFT Revenues divided by non-HFT trading volume. The table also reports long-run trends in various variables measuring the HFT industry concentration in terms of revenues and volumes: specifically, the Herfindahl Concentration by Revenues or by Trading Volumes is calculated as in Eq. (5). All measures are calculated on a daily frequency and reported in Panel A as the average across the trading days of each half-year period. Standard errors are given in parentheses. Panel A also reports T, the number of trading days in each half-year period. Panel B reports estimates of regressions aimed at identifying time trends, specified for each variable observed at daily frequency. The regression specification is given in Eq. (4). An estimated � > 0 indicates an increasing trend in the dependent variable. *, ** and *** correspond to p-values lower than 10%, 5%, and 1%, respectively. In Panel B, Newey-West standard errors (using 30 day lags) are in parentheses. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). 


Panel A: Biannual averages


<table><tr><td></td><td>Total Daily Revenues (SEK)</td><td>Average Daily Revenues (SEK)</td><td>Average Revenues per MSEK Traded (SEK)</td><td>Daily Trading Volume (MSEK)</td><td>Cost of HFT Activities for Non-HFTs (bps)</td><td>Herfindahl Industry Conc. by Trading Volumes</td><td>Herfindahl Industry Conc. by Revenues</td><td>T (days)</td></tr><tr><td>2010:1</td><td>166,484(19439)</td><td>19,694(2256)</td><td>99.71(10.74)</td><td>1,626(57.03)</td><td>0.132(0.014)</td><td>0.292(0.059)</td><td>0.351(0.083)</td><td>124</td></tr><tr><td>2010:2</td><td>167,582(26100)</td><td>20,877(3257)</td><td>105.81(18.13)</td><td>1,589(65.69)</td><td>0.113(0.015)</td><td>0.304(0.04)</td><td>0.354(0.057)</td><td>130</td></tr><tr><td>2011:1</td><td>348,282(79005)</td><td>29,299(6577)</td><td>80.93(13.36)</td><td>4,512(148.62)</td><td>0.274(0.049)</td><td>0.282(0.025)</td><td>0.327(0.067)</td><td>124</td></tr><tr><td>2011:2</td><td>239,140(28225)</td><td>23,156(2668)</td><td>92.26(9.43)</td><td>2,536(80.15)</td><td>0.175(0.018)</td><td>0.225(0.032)</td><td>0.275(0.111)</td><td>130</td></tr><tr><td>2012:1</td><td>265,916(34121)</td><td>21,868(2879)</td><td>65.78(7.4)</td><td>4,167(88.5)</td><td>0.351(0.056)</td><td>0.199(0.044)</td><td>0.282(0.098)</td><td>123</td></tr><tr><td>2012:2</td><td>297,164(44538)</td><td>23,743(3490)</td><td>67.83(9.86)</td><td>4,287(108.34)</td><td>0.289(0.038)</td><td>0.216(0.026)</td><td>0.306(0.109)</td><td>127</td></tr><tr><td>2013:1</td><td>256,618(30104)</td><td>20,898(2375)</td><td>43.92(4.57)</td><td>5,665(108.73)</td><td>0.426(0.045)</td><td>0.206(0.02)</td><td>0.334(0.135)</td><td>122</td></tr><tr><td>2013:2</td><td>294,979(35315)</td><td>23,313(2756)</td><td>58.70(5.75)</td><td>5,487(129.71)</td><td>0.381(0.038)</td><td>0.186(0.03)</td><td>0.298(0.105)</td><td>128</td></tr><tr><td>2014:1</td><td>348,687(69728)</td><td>32,937(6069)</td><td>74.56(10.27)</td><td>4,280(144.08)</td><td>0.372(0.059)</td><td>0.269(0.024)</td><td>0.328(0.105)</td><td>121</td></tr><tr><td>2014:2</td><td>192,896(35573)</td><td>16,945(3244)</td><td>43.59(7.93)</td><td>4,888(153.5)</td><td>0.201(0.036)</td><td>0.290(0.016)</td><td>0.344(0.073)</td><td>129</td></tr></table>


Panel B: Time trend regressions


<table><tr><td></td><td>Total Daily Revenues (SEK)</td><td>Average Daily Revenues (SEK)</td><td>Average Revenues per MSEK Traded (SEK)</td><td>Daily Trading Volume (MSEK)</td><td>Cost of HFT Intermediation for Non-HFTs (bps)</td><td>Herfindahl Industry Conc. by Trading Volumes</td><td>Herfindahl Industry Conc. by Revenues</td></tr><tr><td rowspan="2">(year - 2010)</td><td>22682*</td><td>852.6</td><td>-11.61***</td><td>788.9***</td><td>.05635***</td><td>-.0092*</td><td>-.0022</td></tr><tr><td>(12130)</td><td>(1128)</td><td>(3.124)</td><td>(117.4)</td><td>(.01138)</td><td>(.0049)</td><td>(.0034)</td></tr><tr><td rowspan="2">Constant</td><td>199748***</td><td>21123***</td><td>103.4***</td><td>1867***</td><td>.1266***</td><td>.271***</td><td>.325***</td></tr><tr><td>(32304)</td><td>(3098)</td><td>(10.06)</td><td>(302.2)</td><td>(.02547)</td><td>(.0119)</td><td>(.0107)</td></tr><tr><td>R-squared</td><td>0.004</td><td>0.001</td><td>0.020</td><td>0.361</td><td>0.031</td><td>0.068</td><td>0.001</td></tr><tr><td>N</td><td>1255</td><td>1255</td><td>1255</td><td>1255</td><td>1255</td><td>1255</td><td>1255</td></tr></table>

## Table 11: HFT entry and exit analysis

This table analyzes the determinants of HFT entry and exit into stocks. The performance measures Revenues, Revenues per MSEK Traded, and Returns are defined as in Table 2 for each HFT firm, stock, and trading day. The table reports coefficient estimates from Eq. (7), estimated on a panel of firm-stock-day observations. The one-month dummy takes the value 1 if firm i began trading stock j in the last 30 days, otherwise 0; two- and three-month dummy variables are defined similarly. We exclude the observations in January 2010 as this is when we first observe any firm. In the fourth column, a linear probability regression is estimated using Eq. (7) but with the dummy $E x i t _ { i , t }$ as the dependent variable, which takes the value 1 on day t for firm i if that is the last day firm i trades. This regression excludes observations in December 2014, the last month of the analysis, since we cannot determine exits. In the fifth column, an OLS is estimated on a firm-stock-month panel using Eq. (7) but with Decision Latency as the dependent variable. (Since Decision Latency is a firm-month variable, it is assigned to be constant across stocks). *, ** and *** correspond to p-values lower than 10%, 5%, and 1%, respectively. Standard errors are dually clustered by firm-stock and month and are reported in the parentheses. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). 

<table><tr><td></td><td>Revenues (thous. SEK)</td><td>Revenues per MSEK Traded</td><td>Returns</td><td>Daily Probability of Exit (x 103)</td><td>Decision Latency (in milliseconds, monthly obs.)</td></tr><tr><td>One-month dummy</td><td>-1.90**(.93)</td><td>-97.46(209.7)</td><td>-.032**(.014)</td><td>1.455***(.420)</td><td>44.36*(26.73)</td></tr><tr><td>Two-month dummy</td><td>-3.05**(1.434)</td><td>-87.11(230.3)</td><td>-.033***(.011)</td><td>1.486***(.425)</td><td>134.6***(33.98)</td></tr><tr><td>Three-month dummy</td><td>-.78(1.35)</td><td>104.7(196.6)</td><td>-.018*(.010)</td><td>-.194(.477)</td><td>22.8**(11.19)</td></tr><tr><td>Constant</td><td>1.43***(.19)</td><td>76.64***(4.12)</td><td>.017***(.002)</td><td>.530***(.049)</td><td>14.87***(.89)</td></tr><tr><td>Day x Stock FEs</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>(Month x Stock FEs)</td></tr><tr><td>R-squared</td><td>0.101</td><td>0.129</td><td>0.147</td><td>0.154</td><td>0.432</td></tr><tr><td>N</td><td>241053</td><td>241053</td><td>241053</td><td>241053</td><td>11014</td></tr></table>

## Appendix

## A1. TRS data processing

This appendix presents a summary of our data processing. There are on average 8.56 million entries in each month of the TRS data. Post-processing, the number of observations is on average 6.16 million per month. 

## (a) Time stamp adjustment

The firms reporting to TRS operate in different time zones and the data base does not have a built in functionality to adjust the trade times to a common time zone. To adjust the time stamps we record in which hour the first and last exchange-transaction is executed at NASDAQ OMX Stockholm or at one of the MTFs for each firm in each day. All the exchanges open at 8 am (GMT) and close at 4:30 pm (GMT). We adjust the time stamps of firms that do not have their median first and last trades in sync with the opening hours. For example, for a firm with the median first trade hour in a month being 7 am and the median last trade hour being 3 pm, we adjust all transaction time stamps by +1 hour. 

## (b) Matching to TRTH data

TRS transactions are matched to TRTH transactions using information on stock, trading venue, date, time, price, buy/sell, and quantity. The time stamps of the two databases are allowed to differ by no more than one second. Where trader IDs are available in the TRTH data (for NASDAQ OMX Stockholm only), they are added to the matching criterion. TRTH trades are split into two transactions, one for the buyer and one for the seller. If there are several matches to one transaction, the transaction closest in time is considered to be the closest match. To the extent that there are multiple TRTH trades in the same second, same stock, at the same trading venue, with the same price and quantity, and with different subsecond time stamps, this approach may introduce noise in the time stamps. This potential problem applies only where trader IDs are unavailable in TRTH, and it is more likely at the most active trading venue, for example December 2014 at NASDAQ OMX Stockholm. For that subset, 6.5 % of all transactions have a potentially noisy sub-second time stamp. The time stamp noise due to this problem is however unlikely to influence the Decision Latency, see discussion in footnote 16. 

## (c) Firms

We analyze trading revenues at the corporation level rather than the branch or division level. Accordingly, we truncate BIC codes (11-letter identifiers of the financial institutions reporting to TRS) to the first four letters that are unique to each corporation. For various reasons, such as mergers and acquisitions, the same corporation may span several (truncated) BIC codes. For example, GETCO acquired Knight Trading in August 2013. We thus treat the (truncated) BIC codes GEEU (GETCO) and NITE (Knight Trading) as separate for the period preceding the merger and as one corporation for August 2013 onwards. 

## (d) Filtering of trades

We exclude transactions where the trade price is more than 5% lower than the official low price of the stock-day, or more than 5% higher than the official high price of the day. The official statistics do not consider OTC transactions, so prices outside the High-Low interval are possible, but deviations of more than 5% are considered erroneous. TRS transactions that are flagged as derivative-related either in TRS or in the TRTH entry that it is matched to are also excluded. 

Non-proprietary transactions frequently generate more than one entry in TRS. For example, if a broker buys 100 shares on behalf of a client, it may be reported as two transactions in TRS: one transaction where the reporting firm purchases 100 shares at the exchange, and one off-exchange transaction where the reporting firm sells 100 shares to its client.<sup>29</sup> As firms differ in how they report their transactions we need to process the data to make transactions comparable. 

For each transaction we seek to retain one representative TRS entry and to attach an entry of the end investor associated with that transaction. The end investor assignment is done differently depending on the type of trade. 

We define primary transaction as TRS entries where the counterparty of the trade is a clearing house or the same as the trading venue for the transaction or the owner of the trading venue (in the case of dark pools). The definition is motivated by the fact that all exchange transactions must be done through central counterparty (CCP) clearing. All other TRS entries are defined as secondary transactions. Of all TRS entries, 81.5% are considered primary transactions. 

(i) Primary transaction matched to a secondary transaction of the same firm 

To account for several entries reported for the same transaction, we match primary and secondary transactions by reporting firm, stock, price, quantity, date, and time. The time stamps are allowed to differ by no more than one second. The end investor of primary trades matched in this way is set to the client of the secondary trade, if available, and otherwise to the counterparty of the secondary trade. The matched secondary trades are then discarded. Of all primary transactions, 26 % are matched to a secondary transaction in this way. 

## (ii) Primary transaction matched to a secondary transaction of another firm

To account for the case that the same transaction is reported by both counterparties, we match the reporting firm of primary transactions to the counterparty of secondary transactions. The other matching criteria include stock, price, quantity, date, and time. As above, the time stamps are allowed to differ by no more than one second. The end investor of primary trades matched in this way is set to the client of the secondary trade, if available, and otherwise to the reporting firm of the secondary trade. The matched secondary trades are then discarded. Of all primary transactions, 12 % are matched to a secondary transaction in this way. 

(iii) Primary transaction that is not matched to a secondary transaction 

Primary transactions that are not matched to a secondary transaction are considered to be on behalf of a client if a client reference is available, and otherwise proprietary. For client (proprietary) trades, the end investor is set equal to the client reference (the reporting firm). 

## (iv) Secondary transaction that is not matched to a secondary transaction

Secondary transactions that are not matched to a primary transaction, are considered to be on behalf of a client if a client reference is available, and otherwise proprietary. For client (proprietary) trades, the end investor is set equal to the client reference (the reporting firm). 

## (v) Secondary transactions where the counterparty does not report to TRS

To capture firms that are not obliged to report to TRS, but that still trade our sample stocks, we look for firms that are reported as counterparties but that not show up as reporting firms. For all secondary transactions where such firms appear as counterparties, we create a new entry with the same properties but with opposite direction of trade and with counterparties reversed. This is a way to detect HFT firms that connect to the market through direct market access or sponsored access. Of all secondary transactions, 16 % are subject to this procedure. 

## A2. HFTs active at NASDAQ OMX Stockholm

Appendix Table 1 reports 19 firms identified as HFTs in the sample. Due to confidentiality requirements, we cannot report the full list of names of the 25 HFTs covered in the proprietary data set. However, in Appendix Table 1, we use public trading records to report the names of 19 HFTs who trade at NASDAQ OMX Stockholm as members. The HFTs not listed in Appendix Table 1 therefore trade only at other trading venues or as clients of other members at NASDAQ OMX Stockholm. 

## INSERT APPENDIX TABLE 1 ABOUT HERE

## A3. Comparison of HFT revenue calculation methods

We compare four methods of calculating trading revenues. As explained in the main text, adjustments are needed because small data errors in inventory can accumulate over time, leading to large and persistent (unit root) errors in computing position that can persist indefinitely throughout the sample if left uncorrected. However, this does not appear to be much of a concern in practice, as shown below (see Appendix Table 2). The four methods are as follows. No adjustment is calculated by cumulating daily inventory positions over the full sample. Method 1: Benchmark is the method used throughout the paper that zeros the end-of-day position daily for each HFT firm (equivalent to assuming that each firm liquidates any remaining end-of-day position at the daily closing price). Method 2: Intraday Revenues assumes a first-in-last-out inventory accounting. That is that any remaining end-ofday positions were never purchased in the first place. Method 3: Intraday Revenues Plus Revenues from Inventory Sold is similar to Method 2 but adds back in the revenues from closing end-of-day positions that are in opposite direction of previous day end-of-day inventory. That is, the end-of-day inventory is marked to market only if an offsetting position exists in the previous end-of-day inventory. 

Appendix Table 2 reports the firm cross-sectional distribution of HFT trading revenues using the four different methods for calculating trading revenues. It shows that inventory adjustments do not alter the main results of the paper in the sense that the mean, median, and distribution are roughly similar across the different methods. As a result, marking-to-market end-of-day inventory positions is relatively innocuous. 

## INSERT APPENDIX TABLE 2 ABOUT HERE

## A4. Construction of daily Fama-French plus momentum factors for Swedish equities

We construct daily Fama-French and momentum factors for Swedish equities. The dataset used to construct the factors (using the variables: daily total excess returns, shares outstanding, and quarterly book values) comes from Compustat Global and covers the period January 2010 to December 2014. We exclude stock-day observations in which the total market capitalization falls below 100 MSEK (about 10.5 million USD as of the exchange rate of December 2014). The four factors (excess market return, small minus large [SML], value minus growth [HML], winner minus loser [WML]) are constructed according to the specifications used to create U.S. factors, as specified on Kenneth French's website: the value-weighted portfolios consist of top-30%, middle 40%, and bottom-30% of stocks (by market capitalization, book to market, and past-12-month returns for SML, HML and WML, respectively) and are re-sorted every July 1 using data from the previous year’s performance. 

Appendix Table 3 reports summary statistics corresponding to these traded risk factors for Swedish equities. The statistics include the mean daily log excess return (annualized), its standard error, and the number of observations (i.e., the number of trading days), and are reported for each portfolio. The annualized excess returns on the four portfolios (market excess return, SMB, HML, WML) are 0.160, 0.176, 0.039, and 0.028, respectively, which are all positive, as expected. 

## INSERT APPENDIX TABLE 3 ABOUT HERE

## A5. Exchange fees, liquidity rebates, and their potential effect on trading performance

Appendix Table 4 reports exchange fees in 2014 for three stock exchanges (NASDAQ OMX Stockholm, BATS, and Chi-X) trading Swedish equities. Fees range from 0 to 0.325 bps over these selected venues. Exchange fees depend on the side of the trade: “maker” fees are less than “taker” fees (for example, 0.13 vs. 0.325 bps for NASDAQ OMX S30 stocks), and, at Chi-X, makers receive liquidity rebates (negative fees) of about 0.225 bps. For NASDAQ OMX Stockholm, we report the fees for S30 stocks, which are lower than for other stocks; all the stocks in our sample fall into this category. 

## INSERT APPENDIX TABLE 4 ABOUT HERE

While NASDAQ OMX Stockholm grants preferential prices for liquidity provision under its Liquidity Provider Scheme (LPS), BATS and Chi-X do not (a designated liquidity provider program exists but doesn’t have lower fees). Although BATS and Chi-X merged in November 2011, with technology integration complete by April 2012, the trading platforms continue to implement different pricing structures. 

Appendix Table 5 analyzes HFT performance after accounting for potential maker‐taker fees and liquidity rebates and shows that even accounting for the most conservative possible fees and/or rebates does not qualitatively change the results. 

## INSERT APPENDIX TABLE 5 ABOUT HERE

This table is similar to Table 2 but adjusts for potential maker-taker fees and liquidity rebates. Panel A reports trading revenues under the assumption of the maximum possible maker-taker fees on NASDAQ OMX Stockholm (0.325 bps taker fees; 0.125 bps maker fees), and Panel B uses the maximum possible on the Chi-X exchange, which features a liquidity rebate (0.30 bps taker fees; 0.225 bps liquidity rebate). 

Accounting for the most conservative possible fees and/or rebates does not qualitatively change the results. For example, though trading performance for the entire distribution is shifted down slightly, the sign of Revenues does not change for any HFT firm. We additionally confirm (not reported in the table) that the performance results are still positively skewed, with the same HFTs at the top strongly outperforming their competitors. 

A6. Trading performance and latency of the 5 fastest HFTs 

Appendix Table 6 is similar to Table 4 but breaks down the Top 1-5 dummy variables into individual dummy variables for the fastest HFTs: Top 1, Top 2, Top 3, Top 4, and Top 5. It shows that even among the top five HFTs the faster firm tends to perform better and that performance is monotonic in latency. 

## INSERT APPENDIX TABLE 6 ABOUT HERE

## Appendix Table 1: HFTs active at NASDAQ OMX Stockholm

This table shows a list of HFTs who according to public trading records are active at NASDAQ OMX Stockholm for at least one month of our sample period (January 2010 to December 2014). The list contains 19 of the 25 firms identified as HFTs in our sample. We can only show the public record for confidentiality reasons. HFTs that are not listed do not trade as members at NASDAQ OMX Stockholm, but may trade at other trading venues or as clients of other members at NASDAQ OMX Stockholm. The HFTs are presented in alphabetical order. 

<table><tr><td>Algoengineering</td></tr><tr><td>All Options International</td></tr><tr><td>Citadel Securities</td></tr><tr><td>Flow Traders</td></tr><tr><td>GETCOa</td></tr><tr><td>Hardcastle Trading</td></tr><tr><td>IMC Trading</td></tr><tr><td>International Algorithmic Trading (SSW Trading)</td></tr><tr><td>Knight Capitala</td></tr><tr><td>Madison Tylerb</td></tr><tr><td>MMX Trading</td></tr><tr><td>Optiver</td></tr><tr><td>Spire</td></tr><tr><td>Susquehanna Int. Sec.</td></tr><tr><td>Timber Hill</td></tr><tr><td>WEBB Traders</td></tr><tr><td>Virtu Financialb</td></tr><tr><td>Wolverine Trading UK</td></tr></table>


<sup>a</sup> Knight Capital merged with GETCO in July 2013 



(https://www.sec.gov/Archives/edgar/data/1569391/000119312513279128/d559202d8k12g3.htm) 


## Appendix Table 2: Comparison of HFT revenue calculation methods

This table reports the firm cross-sectional distribution of HFT trading revenues (as in Table 2) using four different methods for calculating trading revenues. No adjustments is calculated by cumulating daily inventory positions over the full sample; Method 1: Benchmark is the method used throughout the paper that zeros the end-of-day position daily for each HFT firm (equivalent to assuming that each firm liquidates any remaining end-of-day position at the daily closing price); Method 2: Intraday Revenues assumes that any remaining end-of-day positions were never purchased in the first place (assuming first-in-last-out inventory accounting); Method 3: Intraday Revenues Plus Revenues from Inventory Sold is similar to Method 2 but adds back in the revenues from closing end-of-day positions that are in opposite direction of previous day end-of-day inventory (that is, the end-of-day inventory is marked to market only if an offsetting position exists in the previous end-of-day inventory). 

<table><tr><td></td><td>mean</td><td>stdev</td><td>p10</td><td>p25</td><td>p50</td><td>p75</td><td>p90</td></tr><tr><td colspan="8">No adjustments</td></tr><tr><td>Revenues</td><td>20,824</td><td>25,149</td><td>-6,788</td><td>277</td><td>10,037</td><td>45,082</td><td>65,415</td></tr><tr><td>Sharpe Ratio</td><td>4.07</td><td>5.16</td><td>-0.76</td><td>0.80</td><td>2.81</td><td>6.04</td><td>10.89</td></tr><tr><td>Revenues per MSEK Traded</td><td>159.42</td><td>326.12</td><td>-201.36</td><td>27.00</td><td>59.05</td><td>217.77</td><td>443.20</td></tr><tr><td colspan="8">Method 1: Benchmark</td></tr><tr><td>Revenues</td><td>18,181</td><td>29,519</td><td>-7,572</td><td>-487</td><td>6,990</td><td>31,968</td><td>61,354</td></tr><tr><td>Sharpe Ratio</td><td>4.16</td><td>6.58</td><td>-1.47</td><td>0.33</td><td>1.61</td><td>7.02</td><td>11.14</td></tr><tr><td>Revenues per MSEK Traded</td><td>153.25</td><td>504.78</td><td>-257.94</td><td>-43.71</td><td>56.45</td><td>147.24</td><td>472.16</td></tr><tr><td colspan="8">Method 2: Intraday Revenues</td></tr><tr><td>Revenues</td><td>18,069</td><td>29,527</td><td>-7,554</td><td>-577</td><td>7,095</td><td>31,972</td><td>61,243</td></tr><tr><td>Sharpe Ratio</td><td>4.15</td><td>6.50</td><td>-1.47</td><td>0.33</td><td>1.61</td><td>7.01</td><td>11.14</td></tr><tr><td>Revenues per MSEK Traded</td><td>146.98</td><td>476.65</td><td>-255.17</td><td>-24.76</td><td>55.54</td><td>147.03</td><td>469.27</td></tr><tr><td colspan="8">Method 3: Intraday Revenues Plus Revenues from Inventory Sold</td></tr><tr><td>Revenues</td><td>21,128</td><td>25,451</td><td>-2,036</td><td>2,026</td><td>11,408</td><td>32,193</td><td>66,835</td></tr><tr><td>Sharpe Ratio</td><td>3.34</td><td>3.80</td><td>-0.09</td><td>0.75</td><td>1.93</td><td>4.90</td><td>9.37</td></tr><tr><td>Revenues per MSEK Traded</td><td>265.14</td><td>535.64</td><td>-200.68</td><td>9.13</td><td>88.62</td><td>367.66</td><td>1,160.62</td></tr></table>

## Appendix Table 3: Daily Fama-French plus momentum factors for Swedish equities

This table reports summary statistics corresponding to daily Fama-French plus momentum factors created for Swedish equities. The mean daily log excess return (annualized), its standard error, and the number of observations (i.e., number of normal trading days) are reported for each of the portfolios. The four factors are constructed according to the specifications used to create U.S. factors, as specified on Kenneth French's website: the value-weighted portfolios consist of top-30%, middle 40%, and bottom-30% of stocks and are re-sorted every July 1 using data from the previous year’s performance. The data (daily total excess returns, shares outstanding, and quarterly book values) come from Compustat Global and covers the period January 2010 to December 2014. 

<table><tr><td></td><td>Mean</td><td>S.E.</td><td>Daily observations</td></tr><tr><td>log market excess returns</td><td>0.160</td><td>0.083</td><td>1255</td></tr><tr><td>log large-cap returns</td><td>0.152</td><td>0.085</td><td>1255</td></tr><tr><td>log medium-cap returns</td><td>0.231</td><td>0.070</td><td>1255</td></tr><tr><td>log small-cap returns</td><td>0.347</td><td>0.063</td><td>1255</td></tr><tr><td>log SML returns</td><td>0.176</td><td>0.068</td><td>1255</td></tr><tr><td>log growth returns</td><td>0.161</td><td>0.088</td><td>1255</td></tr><tr><td>log neutral returns</td><td>0.143</td><td>0.084</td><td>1255</td></tr><tr><td>log value returns</td><td>0.206</td><td>0.090</td><td>1255</td></tr><tr><td>log HML returns</td><td>0.039</td><td>0.054</td><td>1255</td></tr><tr><td>log winner returns</td><td>0.171</td><td>0.095</td><td>1255</td></tr><tr><td>log neutral returns</td><td>0.155</td><td>0.084</td><td>1255</td></tr><tr><td>log loser returns</td><td>0.136</td><td>0.088</td><td>1255</td></tr><tr><td>log WML returns</td><td>0.028</td><td>0.065</td><td>1255</td></tr></table>

## Appendix Table 4: Exchange fees for three exchanges trading Swedish equities

This table reports exchange fees in 2014 for three stock exchanges (NASDAQ OMX Stockholm, BATS, and Chi-X) trading Swedish equities. Exchange fees depend on the side of the trade: “maker” fees are less than “taker” fees, and, at Chi-X, makers receive liquidity rebates (negative fees). NASDAQ OMX Stockholm fees are lower for S30 stocks; all the stocks in this study fall into this category. While NASDAQ OMX Stockholm grants preferential prices for liquidity provision under its Liquidity Provider Scheme (LPS), BATS and Chi-X do not (a designated liquidity provider program exists but it does not have lower fees). Although BATS and Chi-X merged in November 2011, with technology integration complete by April 2012, the trading platforms continue to implement different pricing structures. 

<table><tr><td></td><td>NASDAQ OMX Stockholm for S30 stocks</td><td>NASDAQ OMX Stockholm Liquidity Provider Scheme (LPS) for S30 stocks</td><td>BATS*</td><td>Chi-X*</td></tr><tr><td>Maker</td><td>0.125 bps</td><td>0 bps</td><td>0 bps</td><td>-0.15 to -0.225 bps**</td></tr><tr><td>Taker</td><td>0.325 bps</td><td>0.5 bps</td><td>0.15 bps</td><td>0.30 to 0.24 bps</td></tr></table>


* For non-hidden limit orders 



** The exact price within this range depends on volume. The lowest fees are given after total monthly trading volume exceeds 16 billion EUR. Negative values represent liquidity rebates. 


## Appendix Table 5: HFT performance after accounting for potential maker-taker fees

This table is similar to Table 2 but adjusts for potential maker-taker fees and liquidity rebates. Panel A reports trading revenues under the assumption of the maximum possible maker-taker fees on NASDAQ OMX Stockholm (0.325 bps taker fees; 0.125 bps maker fees), and Panel B uses the maximum possible on the Chi-X exchange, which features a liquidity rebate (0.30 bps taker fees; 0.225 bps liquidity rebate). 


Panel A: Using maker-taker fees on NASDAQ OMX Stockholm


<table><tr><td></td><td>Mean</td><td>Std.Dev.</td><td>p10</td><td>p25</td><td>p50</td><td>p75</td><td>p90</td></tr><tr><td>Revenues (SEK)</td><td>12,012</td><td>18,688</td><td>-2,228</td><td>-1,212</td><td>5,124</td><td>19,346</td><td>52,553</td></tr><tr><td>Revenues per MSEK Traded</td><td>31.87</td><td>207.36</td><td>-209.56</td><td>-39.64</td><td>34.68</td><td>66.04</td><td>330.17</td></tr><tr><td>Returns</td><td>0.22</td><td>0.33</td><td>-0.08</td><td>0.00</td><td>0.08</td><td>0.45</td><td>0.81</td></tr><tr><td>Sharpe Ratio</td><td>3.40</td><td>5.41</td><td>-1.50</td><td>0.00</td><td>1.66</td><td>6.20</td><td>10.49</td></tr><tr><td>1-factor Alpha</td><td>0.22</td><td>0.33</td><td>-0.07</td><td>0.00</td><td>0.08</td><td>0.45</td><td>0.82</td></tr><tr><td>3-factor Alpha</td><td>0.22</td><td>0.33</td><td>-0.06</td><td>0.01</td><td>0.08</td><td>0.45</td><td>0.80</td></tr><tr><td>4-factor Alpha</td><td>0.22</td><td>0.33</td><td>-0.06</td><td>0.01</td><td>0.08</td><td>0.45</td><td>0.80</td></tr></table>


(N = 16 firms) 



Panel B: Using taker fees & liquidity rebates on Chi-X


<table><tr><td></td><td>Mean</td><td>Std.Dev.</td><td>p10</td><td>p25</td><td>p50</td><td>p75</td><td>p90</td></tr><tr><td>Revenues (SEK)</td><td>17,525</td><td>24,207</td><td>-1,230</td><td>-327</td><td>5,252</td><td>36,366</td><td>56,420</td></tr><tr><td>Revenues per MSEK Traded</td><td>50.41</td><td>208.01</td><td>-198.67</td><td>-22.39</td><td>59.28</td><td>83.61</td><td>362.39</td></tr><tr><td>Returns</td><td>0.34</td><td>0.52</td><td>-0.08</td><td>0.01</td><td>0.08</td><td>0.48</td><td>1.11</td></tr><tr><td>Sharpe Ratio</td><td>4.74</td><td>7.61</td><td>-1.45</td><td>0.40</td><td>1.69</td><td>6.56</td><td>13.53</td></tr><tr><td>1-factor Alpha</td><td>0.34</td><td>0.53</td><td>-0.07</td><td>0.01</td><td>0.08</td><td>0.48</td><td>1.12</td></tr><tr><td>3-factor Alpha</td><td>0.34</td><td>0.54</td><td>-0.06</td><td>0.02</td><td>0.09</td><td>0.48</td><td>1.11</td></tr><tr><td>4-factor Alpha</td><td>0.34</td><td>0.54</td><td>-0.06</td><td>0.02</td><td>0.09</td><td>0.48</td><td>1.11</td></tr></table>


(N = 16 firms) 


## Appendix Table 6: Trading performance and latency of the 5 fastest HFTs

This table is similar to Table 4 but breaks down the Top 1-5 dummy variables into individual dummy variables for the fastest HFTs: Top 1, Top 2, Top 3, Top 4, and Top 5. As in Table 4, it reports coefficients estimated from Eq. (1) for five performance measures as dependent variables: Revenues, Returns, Sharpe Ratio, Trading Volume, and Revenues per MSEK Traded (all defined as in Table 2). We estimate OLS regressions with month fixed effects. The independent variables considered are as follows: log(Decision Latency) is the natural logarithm of Decision Latency (defined as in Table 2). Top 1, Top 2, Top 3, Top 4, and Top 5 are indicator variables for whether a given firm is ranked as the top 1, 2, 3, 4, or 5 firms by Decision Latency in a given month. The control variables, whose estimated coefficients are omitted to conserve space, are the same as in Table 4. All continuous independent variables are in units of standard deviations. *, ** and *** correspond to statistical significance at the 10%, 5%, and 1%, respectively. Standard errors are dually clustered by firm and month and are reported in the parentheses. The sample consists of 25 Swedish stocks and 60 months of trading (January 2010 to December 2014). 

<table><tr><td></td><td colspan="3">Revenues</td><td colspan="3">Returns</td><td colspan="3">Sharpe Ratio</td><td colspan="3">Trading Volume (x 10-6)</td><td colspan="3">Revenues per MSEK Traded</td></tr><tr><td rowspan="2">log(Decision Latency)</td><td>-14020***</td><td>1275</td><td>11334</td><td>-.221***</td><td>-.0297</td><td>.0174</td><td>-4.38***</td><td>-.395</td><td>2.34</td><td>-247***</td><td>-54.5</td><td>32.6</td><td>-19.4</td><td>-6.68</td><td>102**</td></tr><tr><td>(4311)</td><td>(6837)</td><td>(10708)</td><td>(.0483)</td><td>(.063)</td><td>(.0797)</td><td>(.632)</td><td>(1.34)</td><td>(1.5)</td><td>(43.7)</td><td>(64.7)</td><td>(77.8)</td><td>(57.5)</td><td>(69.3)</td><td>(40.6)</td></tr><tr><td rowspan="2">Top 1</td><td></td><td>58288***</td><td>44007***</td><td></td><td>.626***</td><td>.604***</td><td></td><td>12.2***</td><td>10.8***</td><td></td><td>693***</td><td>545***</td><td></td><td>33.9</td><td>106*</td></tr><tr><td></td><td>(15035)</td><td>(11886)</td><td></td><td>(.152)</td><td>(.166)</td><td></td><td>(3.63)</td><td>(3.7)</td><td></td><td>(160)</td><td>(145)</td><td></td><td>(103)</td><td>(57.4)</td></tr><tr><td rowspan="2">Top 2</td><td></td><td>40358***</td><td>29165***</td><td></td><td>.396***</td><td>.361***</td><td></td><td>9.01**</td><td>6.98**</td><td></td><td>496***</td><td>371***</td><td></td><td>26.7</td><td>56.3</td></tr><tr><td></td><td>(15163)</td><td>(10847)</td><td></td><td>(.15)</td><td>(.134)</td><td></td><td>(3.55)</td><td>(3.12)</td><td></td><td>(143)</td><td>(101)</td><td></td><td>(116)</td><td>(83.8)</td></tr><tr><td rowspan="2">Top 3</td><td></td><td>35262*</td><td>24967*</td><td></td><td>.575***</td><td>.534***</td><td></td><td>12.1**</td><td>9.91**</td><td></td><td>563**</td><td>446***</td><td></td><td>23.8</td><td>33.9</td></tr><tr><td></td><td>(21206)</td><td>(14052)</td><td></td><td>(.212)</td><td>(.19)</td><td></td><td>(5.17)</td><td>(4.22)</td><td></td><td>(232)</td><td>(169)</td><td></td><td>(98.2)</td><td>(63.2)</td></tr><tr><td rowspan="2">Top 4</td><td></td><td>23756**</td><td>16243**</td><td></td><td>.441**</td><td>.414**</td><td></td><td>8.89**</td><td>7.01**</td><td></td><td>249*</td><td>159</td><td></td><td>78.3</td><td>90.5***</td></tr><tr><td></td><td>(11854)</td><td>(7722)</td><td></td><td>(.21)</td><td>(.182)</td><td></td><td>(3.51)</td><td>(2.88)</td><td></td><td>(136)</td><td>(108)</td><td></td><td>(88)</td><td>(33.5)</td></tr><tr><td rowspan="2">Top 5</td><td></td><td>11588</td><td>5422</td><td></td><td>.106</td><td>.0955</td><td></td><td>2.92</td><td>2.21</td><td></td><td>117</td><td>48.6</td><td></td><td>-25.9</td><td>14.8</td></tr><tr><td></td><td>(7457)</td><td>(7618)</td><td></td><td>(.0952)</td><td>(.0838)</td><td></td><td>(1.8)</td><td>(1.62)</td><td></td><td>(87.5)</td><td>(79)</td><td></td><td>(102)</td><td>(73.7)</td></tr><tr><td rowspan="2">Constant</td><td>20278***</td><td>6993*</td><td>9568**</td><td>.254***</td><td>.0852</td><td>.0885*</td><td>5.1***</td><td>1.55</td><td>1.92</td><td>313***</td><td>147***</td><td>177***</td><td>35.2</td><td>24.4</td><td>6.17</td></tr><tr><td>(6973)</td><td>(3874)</td><td>(4393)</td><td>(.0579)</td><td>(.0564)</td><td>(.0463)</td><td>(1.26)</td><td>(1.28)</td><td>(1.21)</td><td>(75.9)</td><td>(55.8)</td><td>(52.4)</td><td>(57.3)</td><td>(82.2)</td><td>(11.9)</td></tr><tr><td>Controls</td><td>No</td><td>No</td><td>Yes</td><td>No</td><td>No</td><td>Yes</td><td>No</td><td>No</td><td>Yes</td><td>No</td><td>No</td><td>Yes</td><td>No</td><td>No</td><td>Yes</td></tr><tr><td>Month FEs</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td><td>Yes</td></tr><tr><td>R-squared</td><td>0.123</td><td>0.168</td><td>0.263</td><td>0.198</td><td>0.233</td><td>0.269</td><td>0.207</td><td>0.254</td><td>0.361</td><td>0.294</td><td>0.362</td><td>0.454</td><td>0.080</td><td>0.080</td><td>0.148</td></tr><tr><td>N</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td><td>737</td></tr></table>