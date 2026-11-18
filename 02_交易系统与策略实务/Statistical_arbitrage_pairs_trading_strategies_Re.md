

<!-- === Source: MinerU_markdown_Statistical_arbitrage_pairs_trading_strategies_Re_1_2122706224590991366.md (Page 1) === -->

Krauss, Christopher 

Working Paper 

# Statistical arbitrage pairs trading strategies: Review and outlook

IWQW Discussion Paper Series, No. 09/2015 

Provided in Cooperation with: 

Friedrich-Alexander University Erlangen-Nuremberg, Institute for Economics 

Suggested Citation: Krauss, Christopher (2015) : Statistical arbitrage pairs trading strategies: Review and outlook, IWQW Discussion Paper Series, No. 09/2015 

This Version is available at: http://hdl.handle.net/10419/116783 

## Standard-Nutzungsbedingungen:

Die Dokumente auf EconStor dürfen zu eigenen wissenschaftlichen Zwecken und zum Privatgebrauch gespeichert und kopiert werden. 

Sie dürfen die Dokumente nicht für öffentliche oder kommerzielle Zwecke vervielfältigen, öffentlich ausstellen, öffentlich zugänglich machen, vertreiben oder anderweitig nutzen. 

Sofern die Verfasser die Dokumente unter Open-Content-Lizenzen (insbesondere CC-Lizenzen) zur Verfügung gestellt haben sollten, gelten abweichend von diesen Nutzungsbedingungen die in der dort genannten Lizenz gewährten Nutzungsrechte. 

## Terms of use:

Documents in EconStor may be saved and copied for your personal and scholarly purposes. 

You are not to copy documents for public or commercial purposes, to exhibit the documents publicly, to make them publicly available on the internet, or to distribute or otherwise use the documents in public 

If the documents have been made available under an Open Content Licence (especially Creative Commons Licences), you may exercise further usage rights as specified in the indicated licence. 

Mitglied der Lmibniz Leibniz-Gemeinschaft 

IWQW 

Institut für Wirtschaftspolitik und Quantitative Wirtschaftsforschung 

Diskussionspapier Discussion Papers 

No. 09/2015 

# Statistical Arbitrage Pairs Trading Strategies: Review and Outlook

Christopher Krauss University of Erlangen-Nürnberg 

ISSN 1867-6707 

# Statistical Arbitrage Pairs Trading Strategies: Review and Outlook

Christopher Krauss Department of Statistics and Econometrics University of Erlangen-N¨urnberg, N¨urnberg 

Wednesday 26<sup>th</sup> August, 2015 

## Abstract

This survey reviews the growing literature on pairs trading frameworks, i.e., relative-value arbitrage strategies involving two or more securities. The available research is categorized into five groups: The distance approach uses nonparametric distance metrics to identify pairs trading opportunities. The cointegration approach relies on formal cointegration testing to unveil stationary spread time series. The time series approach focuses on finding optimal trading rules for mean-reverting spreads. The stochastic control approach aims at identifying optimal portfolio holdings in the legs of a pairs trade relative to other available securities. The category ”other approaches” contains further relevant pairs trading frameworks with only a limited set of supporting literature. Drawing from this large set of research consisting of more than 90 papers, an in-depth assessment of each approach is performed, ultimately revealing strengths and weaknesses relevant for further research and for implementation. 

Keywords: Statistical arbitrage, pairs trading, spread trading, relative-value arbitrage, meanreversion 

## 1. Introduction

According to Gatev et al. (2006), the concept of pairs trading is surprisingly simple and follows a two-step process. First, find two securities whose prices have moved together historically in a formation period. Second, monitor the spread between them in a subsequent trading period. If the prices diverge and the spread widens, short the winner and buy the loser. In case the two securities follow an equilibrium relationship, the spread will revert to its historical mean. Then, the positions are reversed and a profit can be made. The concept of univariate pairs trading can also be extended: In quasi-multivariate frameworks, one security is traded against a weighted portfolio of comoving securities. In fully multivariate frameworks, groups of stocks are traded against other groups of stocks. Terms of reference for such refined strategies are (quasi-)multivariate pairs trading, generalized pairs trading or statistical arbitrage. We further consider all these strategies under the umbrella term of ”statistical arbitrage pairs trading” (or short, ”pairs trading”), since it is the ancestor of more complex approaches (Vidyamurthy, 2004; Avellaneda and Lee, 2010). Clearly, pairs trading is closely related to other long-short anomalies, such as violations of the law of one price, lead-lag anomalies and return reversal anomalies. For a comprehensive overview of these and further long-short return phenomena, see Jacobs (2015). 

The most cited paper in the pairs trading domain has been published by Gatev et al. (2006), hereafter GGR. A simple yet compelling algorithm is tested on a large sample of U.S. equities, while rigorously controlling for data snooping bias. The strategy yields annualized excess returns of up to 11 percent at low exposure to systematic sources of risk. More importantly, profitability cannot be explained by previously documented reversal profits as in Jegadeesh (1990) and Lehmann (1990) or momentum profits as in Jegadeesh and Titman (1993). These unexplained excess returns elevate GGR’s pairs trading to one of the few capital market phenomena<sup>1</sup> that stood the test of $\mathrm { t i m e ^ { 2 } }$ as well as independent scrutiny by later authors, most notably Do and Faf (2010, 2012). 

Despite these findings, we have to recognize that academic research about pairs trading is still small compared to contrarian and momentum strategies.<sup>3</sup> However, interest has recently surged, and there is a growing base of conceptual pairs trading frameworks and empirical applications available across diferent asset classes. The prima facie simplicity of GGR’s strategy quickly evaporates in light of these recent developments. In total, we identify the following five streams of literature relevant to pairs trading research: 

• Distance approach: This approach represents the most intensively researched pairs trading framework. In the formation period, various distance metrics are leveraged to identify comoving securities. In the trading period, simple nonparametric threshold rules are used to trigger trading signals. The key assets of this strategy are its simplicity and its transparency, allowing for large scale empirical applications. The main findings establish distance pairs trading as profitable across diferent markets, asset classes and time frames. 

• Cointegration approach: Here, cointegration tests are applied to identify comoving securities in a formation period. In the trading period, simple algorithms are used to generate trading signals; the majority of them based on GGR’s threshold rule. The key benefit of these strategies is the econometrically more reliable equilibrium relationship of identified pairs. 

• Time series approach: In the time series approach, the formation period is generally ignored. All authors in this domain assume that a set of comoving securities has been established by prior analyses. Instead, they focus on the trading period and how optimized trading signals can be generated by diferent methods of time series analysis, i.e., by modeling the spread as a mean-reverting process. 

• Stochastic control approach: As in the time series approach, the formation period is ignored. This stream of literature aims at identifying the optimal portfolio holdings in the legs of a pairs trade compared to other available assets. Stochastic control theory is used to determine value and optimal policy functions for this portfolio problem. 

• Other approaches: This bucket contains further pairs trading frameworks with only a limited set of supporting literature and limited relation to previously mentioned approaches. Included in this category are the machine learning and combined forecasts approach, the copula approach, and the Principal Components Analysis (PCA) approach. 


Table 1 provides an overview of representative studies per approach, the data sample and the returns p.a., as stated in the respective paper.<sup>4</sup>


<table><tr><td>Approach</td><td>Representative studies</td><td>Sample</td><td>Return p.a.</td></tr><tr><td rowspan="2">Distance</td><td>Gatev et al. (2006)</td><td>U.S. CRSP 1962-2002</td><td>0.11</td></tr><tr><td>Do and Faff (2010)</td><td>U.S. CRSP 1962-2009</td><td>0.07</td></tr><tr><td rowspan="2">Cointegration</td><td>Vidyamurthy (2004)</td><td>-</td><td>-</td></tr><tr><td>Caldeira and Moura (2013)</td><td>Brazil 2005-2010</td><td>0.16</td></tr><tr><td rowspan="2">Time series</td><td>Elliott et al. (2005)</td><td>-</td><td>-</td></tr><tr><td>Cummins and Bucca (2012)</td><td>Energy futures 2003-2010</td><td>≥0.18</td></tr><tr><td rowspan="2">Stochastic control</td><td>Jurek and Yang (2007)</td><td>Selected stocks 1962-2004</td><td>0.28-0.43</td></tr><tr><td>Liu and Timmermann (2013)</td><td>Selected stocks 2006-2012</td><td>0.06-0.23</td></tr><tr><td rowspan="2">Others: ML, combined forecasts</td><td>Huck (2009)</td><td>U.S. S&amp;P 100 1992-2006</td><td>0.13-0.57</td></tr><tr><td>Huck (2010)</td><td>U.S. S&amp;P 100 1993-2006</td><td>0.16-0.38</td></tr><tr><td rowspan="2">Others: Copula</td><td>Liew and Wu (2013)</td><td>Selected stocks 2009-2012</td><td>-</td></tr><tr><td>Stander et al. (2013)</td><td>Selected stocks, SSFs 2007-2009</td><td>-</td></tr><tr><td>Others: PCA</td><td>Avellaneda and Lee (2010)</td><td>U.S. subset 1997-2007</td><td>-</td></tr></table>


Table 1: Overview pairs trading approaches


Considering the diversity of the above mentioned categories, the contribution of this survey is twofold: First, a comprehensive review of pairs trading literature is provided along the five approaches. Second, the most relevant contributions per category are discussed in detail. Drawing from a large set of literature consisting of more than 90 papers, an in-depth assessment of each approach is possible, ultimately revealing strengths and weaknesses relevant for further research and for implementation. The latter fact makes this survey relevant for researchers and practitioners alike. The remainder of this paper is organized as follows: Section 2 covers the distance approach and its various empirical applications. Section 3 reviews uni- and multivariate frameworks for the cointegration approach. Section 4 covers the time series approach and discusses diferent models aiming at the identification of optimal trading thresholds. Section 5 reviews the stochastic control approach and how to determine optimal portfolio holdings. Section 6 covers the remaining approaches. Finally, section 7 concludes and summarizes directions for further research. 

## 2. Distance approach

This section provides a comprehensive treatment of the distance approach. A concise overview with relevant studies, their data samples and objectives is provided in table 2. 

<table><tr><td>Study</td><td>Date</td><td>Sample</td><td>Objective</td></tr><tr><td>GGR</td><td>1999</td><td>U.S. CRSP 1962-1997</td><td rowspan="2">Baseline approach in U.S. equity markets: Pairs trading is profitable; returns are robust</td></tr><tr><td>GGR</td><td>2006</td><td>U.S. CRSP 1962-2002</td></tr><tr><td>DF</td><td>2010</td><td>U.S. CRSP 1962-2009</td><td rowspan="2">Expanding on GGR: Profitability is declining and not robust to transaction costs; improved formation based on industry, number of zero crossings</td></tr><tr><td>DF</td><td>2012</td><td>U.S. CRSP 1963-2009</td></tr><tr><td>CCL</td><td>2012</td><td>U.S. CRSP 1962-2002</td><td rowspan="3">Improvements: Quasi-multivariate pairs trading variants outperform univariate pairs trading; correlation-based formation outperforms SSD rule</td></tr><tr><td>P</td><td>2007</td><td>Brazil 2000-2006</td></tr><tr><td>P</td><td>2009</td><td>Brazil 2000-2006</td></tr><tr><td>ADS</td><td>2005</td><td>Taiwan 1994-2002</td><td rowspan="6">Sources of pairs trading profitability: Uninformed demand shocks, accounting events, common vs. idiosyncratic information, market frictions, etc.</td></tr><tr><td>PW</td><td>2007</td><td>U.S. subset 1981-2006</td></tr><tr><td>EGJ</td><td>2009</td><td>U.S. CRSP 1993-2006</td></tr><tr><td>JW</td><td>2013</td><td>Intl&#x27;; U.S. CRSP 1960-2008</td></tr><tr><td>J</td><td>2015</td><td>U.S. CRSP 1962-2008</td></tr><tr><td>JW</td><td>2015</td><td>Intl&#x27;; U.S. CRSP 1962-2008</td></tr><tr><td>H</td><td>2013</td><td>U.S. S&amp;P 500 2002-2009</td><td rowspan="2">Sensitivity of pairs trading profitability to duration of formation period and to volatility timing</td></tr><tr><td>H</td><td>2015</td><td>U.S.; Japan 2003-2013</td></tr><tr><td>N</td><td>2003</td><td>U.S. GovPX 1994-2000</td><td rowspan="2">High-frequency: Pairs trading profitability in the U.S. bond market and the U.K. equity market</td></tr><tr><td>BHO</td><td>2010</td><td>U.K. FTSE 100 2007-2007</td></tr><tr><td>BDZ</td><td>2009</td><td>Commodities 1990-2008</td><td rowspan="4">Further out-of-sample tests: Pairs trading profitability in the commodity markets, the Finnish market, the REIT sector, the U.K. equity market</td></tr><tr><td>BV</td><td>2012</td><td>Finland 1987-2008</td></tr><tr><td>MZ</td><td>2011</td><td>U.S. REITS 1987-2008</td></tr><tr><td>BH</td><td>2014</td><td>U.K. 1979-2012</td></tr></table>


Table 2: Distance approach


## 2.1 The baseline approach - Gatev, Goetzmann and Rouwenhorst

The distance approach has been introduced by the seminal paper of Gatev et al. (2006). Their study is performed on all liquid U.S. stocks from the CRSP daily files from 1962 to 2002. First, a cumulative total return index $P _ { i t }$ is constructed for each stock i and normalized to the first day of a 12 months formation period. Second, with n stocks under consideration, the sum of Euclidean squared distance (SSD) for the price time series<sup>5</sup> of $n ( n - 1 ) / 2$ possible combinations of pairs is calculated. The top 20 pairs with minimum historic distance metric are considered in a subsequent six months trading period. Prices are normalized again to the first day of the trading period. Trades are opened when the spread diverges by more than two historical standard deviations σ and closed upon mean reversion, at the end of the trading period, or upon delisting. The advantages of this methodology are relatively clear: As Do et al. (2006) point out, GGR’s ansatz is economic model-free, and as such not subject to model mis-specifications and mis-estimations. It is easy to implement, robust to data snooping and results in statistically significant risk-adjusted excess returns. The simple yet compelling methodology, applied to large sample over more than 40 years has definitely established pairs trading as a true capital market anomaly. However, there are also some areas of improvement: The choice of Euclidean squared distance for identifying pairs is analytically suboptimal. To elaborate on this fact, let us assume that a rational pairs trader has the objective of maximizing excess returns per pair, as in GGR’s paper. With constant initial invest, this amounts to maximizing profits per pair. The latter are the product of number of trades per pair and profit per trade. As such, a pairs trader aims for spreads exhibiting frequent and strong divergences from and subsequent convergences to equilibrium. In other words, the profitmaximizing rational investor seeks out pairs with the following characteristics: First, the spread should exhibit high variance and second, the spread should be strongly mean-reverting. These two attributes generate a high number of round-trip trades with high profits per trade. Let us now examine how GGR’s ranking logic relates to these requirements. 

Spread variance: $P _ { i t }$ and $P _ { j t }$ denote the normalized price time series of the securities i and $j$ of a pair and $\mathrm { V } ( . )$ the sample variance. As such, empirical spread variance $\mathrm { V } \left( P _ { i t } - P _ { j t } \right)$ can be expressed as follows: 

$$
\mathrm{V} \left(P _ {i t} - P _ {j t}\right) = \frac {1}{T} \sum_ {t = 1} ^ {T} \left(P _ {i t} - P _ {j t}\right) ^ {2} - \left(\frac {1}{T} \sum_ {t = 1} ^ {T} \left(P _ {i t} - P _ {j t}\right)\right) ^ {2}\tag{1}
$$

We can solve for the average sum of squared distances for the formation period: 

$$
\overline {{S S D _ {i j t}}} = \frac {1}{T} \sum_ {t = 1} ^ {T} (P _ {i t} - P _ {j t}) ^ {2} = \mathrm{V} (P _ {i t} - P _ {j t}) + \left(\frac {1}{T} \sum_ {t = 1} ^ {T} (P _ {i t} - P _ {j t})\right) ^ {2}\tag{2}
$$

First of all, it is trivial to see that an ”ideal pair” in the sense of GGR with zero squared distance has a spread of zero and thus produces no profits. The latter fact is indicative for a suboptimal selection metric, since we would expect the number one pair of the ranking to produce the highest profits. Next, let us consider pairs with low average SSD at the top of GGR’s ranking. Equation (2) shows that constraining for low SSD is the same as minimizing the sum of (i) spread variance and (ii) squared spread mean. Considering that the spread starts trading at zero due to normalization, we see that summand (ii) grows with the spread mean drifting away from its initial level. Conversely, summand (i) grows with increasing magnitude of deviations from this mean. It is hard to say which of these two summands dominates the minimization problem in an empirical application to security prices. However, table 2 of GGR’s results clearly shows decreasing spread volatility as we move up the ranking towards the top pairs. Thus, GGR’s selection metric is prone to form pairs with low spread variance, which ultimately limits profit potential and is in conflict with the objectives of a rational investor - at least from a purely analytic perspective. 

Mean reversion: GGR interpret the pairs price time series as cointegrated in the sense of Bossaerts (1988). However, Bossaerts develops a rigorous cointegration test based on canonical correlation analysis and applies it to industry and size-based portfolios. Conversely, GGR perform no cointegration testing on their identified pairs (Galenko et al., 2012). As such, the high correlation<sup>6</sup> may well be spurious, since high correlation is not related to a cointegration relationship (Alexander, 2001). It is unclear why the top pairs of the ranking are not truly tested for cointegration. This omission leads to pairs which are yet again not fully in line with the requirements of a rational investor. Spurious relationships based on an assumption of return parity are not meanreverting. The potential lack of an equilibrium relationship leads to higher divergence risks, such that opened pair trades may run in an unfavorable direction and have to be closed at a loss. Do and Faf (2010), using an extension of the GGR data and the same methodology, confirm that 32 percent of all identified pairs based on the distance metric actually do not converge. Huck (2015) shows in a later study that pairs selected based on cointegration relationships more frequently exhibit mean-reverting behavior compared to distance pairs, even if they do not necessarily converge until the end of the trading period (see share of non-convergent profitable trades in Huck (2015) table 3, p. 606). 

From this theoretical perspective, a better selection metric in line with the objectives of a rational investor could potentially be constructed as follows: First, pairs exhibiting the lowest drift in spread mean (summand(ii)) should be identified. Second, of these pairs, the ones with the highest spread variance (summand(i)) are retained and tested for cointegration while controlling the familywise error rate as in Cummins and Bucca (2012). This process selects cointegrated pairs with lower divergence risk and simultaneously assures more volatile spreads, resulting in higher profit opportunities. This theoretical assertion is confirmed in a recent comparison study of Huck and Afawubo (2015), showing that the volatility of the price spread of cointegrated pairs is almost twice as high as the volatility of the price spread of distance pairs. Nevertheless, this critique shall not detract from the fact that GGR’s large-scale empirical application of a simple yet compelling strategy has originally established pairs trading in the academic community. At that stage in time, the transparent nonparametric approach was required to capture the essence of this relative-value strategy. 

## 2.2 Expanding on the GGR sample

Do and Faf (2010, 2012) replicate GGR’s methodology on the U.S. CRSP stock universe, but extend the sample period by seven more years until 2009. They confirm a declining profitability in pairs trading, mainly due to an increasing share of nonconverging pairs. With the inclusion of trading costs, pairs trading according to GGR’s baseline methodology becomes largely unprofitable. Do and Faf then use refined selection criteria to improve pairs identification. First, they only allow for matching securities within the 48 Fama-French industries. This restriction has a potential to identify more meaningful pairs and to reduce spurious correlations, since companies are matched within the same sectors. However, there is also potential to miss out on inter-industry pairs trading opportunities, such as between customers and suppliers. For example, Cohen and Frazzini (2008) find substantial customer-supplier links in the U.S. stock market that allow for return predictability. Second, Do and Faf favor pairs with a high number of zero-crossings in the formation period. This indicator is used as a proxy for mean-reversion strength. It is not yet a cointegration test, as suggested earlier, but this heuristic already takes mean-reversion into account. The top portfolios incorporating industry restrictions, the number of zero-crossings as well as SSD in the selection algorithm are still slightly profitable, even after full consideration of transaction costs. However, the methodology of Do and Faf (2012) is more susceptible for data snooping, since they test a total of 29 diferent combinations of selection algorithms. Nevertheless, through independent scrutiny, these two studies have significantly contributed to corroborating GGR’s findings and to establishing pairs trading as capital market anomaly. 

## 2.3 From SSD to Pearson correlation and quasi-multivariate pairs trading

Chen et al. (2012) use the same data set and time frame as GGR, but they opt for Pearson correlation on return level for identifying pairs. In a five year formation period, pairwise return correlations are calculated, based on monthly return data for all stocks. Then, the authors construct a metric to quantify return divergence $D _ { i j t }$ of stock i from its comover $j \colon$ 

$$
D _ {i j t} = \beta (R _ {i t} - R _ {f}) - (R _ {j t} - R _ {f})\tag{3}
$$

Thereby, $\beta$ denotes the regression coeficient of stock i’s monthly return $R _ { i t }$ on its comover return $R _ { j t }$ and $R _ { f }$ is the risk free rate. Chen et al. consider two cases for the comover return $R _ { j t } { \mathrm { : } }$ : In the univariate case, it is the return of the most highly correlated partner for stock i. In the quasimultivariate case, it is the return of a comover portfolio, consisting of the equal weighted returns of the 50 most highly correlated partners for stock i. Subsequent to the formation period follows a one month trading period. All stocks are sorted in descending order based on their previous month’s return divergence and split into ten deciles. A dollar-neutral portfolio is constructed by longing decile 10 and shorting decile 1, and held for one month. Then, the process is repeated for the next month, with the prior five years as new formation period. 

The key question is how the correlation selection metric on return level difers from the SSD selection metric on price level. First, let us consider an expression for the sample variance of the spread return, defined as return on buy minus return on sell (Pole, 2008): 

$$
\mathrm{V} (R _ {i t} - R _ {j t}) = \mathrm{V} (R _ {i t}) + \mathrm{V} (R _ {j t}) - 2 r (R _ {i t}, R _ {j t}) \sqrt {\mathrm{V} (R _ {i t})} \sqrt {\mathrm{V} (R _ {i t})}\tag{4}
$$

We can immediately see from equation (4) that constraining for high return correlation $r ( R _ { i t } , R _ { j t } )$ leads to lower variance of spread returns. However, the returns $R _ { i t }$ and $R _ { j t }$ of the individual securities may still exhibit diferent variances. Let us now consider an analogous expression for the variance of the price spread under the constraint of low SSD. For simplicity’s sake, we assume that minimizing SSD leads to a minimization of price spread variance: 

$$
\begin{array}{r l} & {\mathrm{V} (P _ {i t} - P _ {j t}) = \mathrm{V} (P _ {i t}) + \mathrm{V} (P _ {j t}) - 2 r (P _ {i t}, P _ {j t}) \sqrt {\mathrm{V} (P _ {i t})} \sqrt {\mathrm{V} (P _ {i t})}} \\ & {\qquad \mathrm{s.t.:} \quad \mathrm{V} (P _ {i t} - P _ {j t}) \longrightarrow \min!} \end{array}\tag{5}
$$

Variance of the spread price in equation (5) reaches its minimum of zero, if the two stock prices are perfectly correlated and their price time series exhibit exactly the same variance. The minimum SSD criterion thus seeks out security prices exhibiting similar variance and high correlation. Clearly, this selection metric is stricter than simply demanding for high return correlation, as in Chen et al. For example, consider two securities with perfect return correlation, but one stock return is always twice that of the other (for example, due to very similar business models but diferent degrees of financial leverage, see Chen et al. (2012)). Return divergences between these two companies can successfully be captured in Chen et al.’s framework. In case their selection metric is meaningful and return divergences are reversed in the following month, a profit can be made. Conversely, the SSD metric would have missed out on this opportunity, since the price spread between these two stocks is clearly divergent. The second diference to GGR’s study stems from the higher information level contained in a diversified comover portfolio as opposed to single stocks. Return divergences from such a portfolio are more likely to be caused by idiosyncratic movements of stock i, and thus potentially reversible. A third diference lies in the trading method, which happens mechanically once a month for the top and bottom decile. As such, it is clear in advance how many pairs are traded and which amount of capital has to be allocated. For an equal-weighted portfolio, Chen et al. (2012) report average monthly raw returns of 1.70 percent, almost twice as high as those of GGR. The majority of this increase can be explained by the advantages of the comover portfolio. Reducing the number of stocks in the comover portfolio to one leads to a drop in returns by almost one third.<sup>7</sup> The rest of the edge versus the GGR methodology most likely stems from the higher flexibility of return correlation as pairs selection metric. Nonetheless, it needs to be pointed out that return correlation may be favorable to SSD from this empirical point of view, but it is also far from optimal. Two securities correlated on return level do not necessarily share an equilibrium relationship and there is no theoretical foundation that divergences need to be reversed. Actually, many of Chen et al.’s correlations may well be spurious. A better approach may be to look for cointegrated pairs, which is addressed in section 3. 

Perlin (2007, 2009) also test the advantages of quasi-multivariate pairs trading versus univariate pairs trading. Both studies concentrate on the 57 most liquid stocks in the Brazilian market from 2000 to 2006. Price time series are standardized by subtracting the mean and dividing by the standard deviation during a two year moving-window formation period. This transformation leads to the fact that minimum SSD and maximum Pearson correlation identify the same pairs, when applied to the price time series. The latter is easy to show, since the average SSD of two standardized price time series $P _ { i t }$ and $P _ { j t }$ can be expressed as follows: 

$$
\overline {{S S D _ {i j t}}} = \frac {1}{T} \sum_ {t = 1} ^ {T} (P _ {i t} - P _ {j t}) ^ {2} = \frac {1}{T} \sum_ {t = 1} ^ {T} (P _ {i t} ^ {2} - 2 P _ {i t} P _ {j t} + P _ {j t} ^ {2}) = \frac {1}{T} \sum_ {t = 1} ^ {T} (P _ {i t} ^ {2} - 2 r (P _ {i t}, P _ {j t}) + P _ {j t} ^ {2})\tag{6}
$$

where $r ( P _ { i t } , P _ { j t } )$ denotes the Pearson correlation coeficient of the standardized price time series. We directly see from equation (6) that maximizing correlation is equivalent to minimizing SSD. In the univariate context, Perlin (2007) matches stock i with stock $j ,$ , when the two standardized price time series exhibit maximum correlation. In the quasi-multivariate context, Perlin (2007) matches stock i with m = 5 stocks that show maximum correlation with stock i. In the next step, the standardized price time series $P _ { i t }$ of stock i is explained by a linear combination of the price time series $P _ { k t }$ of these five assets and an error term $\epsilon _ { i t }$ , as in the following equation: 

$$
P _ {i t} = \sum_ {k = 1} ^ {5} w _ {k} P _ {k t} + \epsilon_ {i t}\tag{7}
$$

The weights $w _ { k }$ are determined in three alternative approaches: Equal weighting, simple OLS and correlation weighting. Every ten days, these weights are re-estimated using the past two years of observations. A pairs trade is opened, if the spread between the two price time series exceeds a threshold value of k. The trade is closed, when the spread falls below k. In the univariate case, Perlin goes long the undervalued and short the overvalued security in equal dollar amounts. In the quasi-multivariate case, only the reference component of each pair is traded and not the synthetic asset, in order to avoid high transaction costs. Perlin (2007) reaches the same conclusion as Chen et al. (2012) at a later stage: Quasi-multivariate pairs trading results in higher and more robust annual excess returns than univariate pairs trading for a broad range of diferent threshold values. 

## 2.4 Explaining pairs trading profitability

Gatev et al. (2006) have shown that their excess returns of up to 11 percent per annum do not load on typical sources of systematic risk. Yet, risk-ajdusted excess returns of disjoint pairs portfolios exhibit high correlation. So, GGR hypothesize that these returns are a compensation for a yet undiscovered latent risk factor. Subsequent studies focus on trying to discover the sources of pairs trading profitability. 

Andrade et al. (2005) replicate GGR’s approach in the Taiwanese stock market from 1994 to 2004. First, they confirm GGR’s findings on their data set. Then, they link uninformed demand shocks with pairs trading risk and return characteristics. Andrade et al. find that the dominant factor behind spread divergence is uninformed buying, so that pairs returns exhibit strong correlation with uninformed demand shocks in the underlying securities. The authors conclude that pairs trading profits are a compensation for liquidity provision to uninformed buyers. 

Papadakis and Wysocki (2007) use GGR’s pairs trading rule on a subset of the U.S. equity market to analyze the impact of accounting events on pairs trading profitability between 1981 and 2006. Their key finding is that pairs trades are often opened around earnings announcements and analyst forecasts. Trades triggered after such events are significantly less profitable than those in non-event periods, which can be explained by investor underreaction. Incremental excess returns are earned by delaying the closures up to three weeks until after accounting events. This research suggests that drift in stock prices after such events is a significant factor afecting pairs trading profitability. However, Do and Faf (2010) could not replicate these results on the extended GGR sample, which casts doubt on the robustness of Papadakis and Wysocki’s findings. 

Engelberg et al. (2009) test a variant of the GGR algorithm on the CRSP U.S. stock universe from 1993 to 2006. They find that pairs trading profitability exponentially decreases over time and that this profitability is strongly related to events at the time of spread divergence. Idiosyncratic information and idiosyncratic liquidity shocks are unfavorable, since they have no impact on the paired firm and render spread divergences permanent. The combination of common information to both stocks with market frictions such as illiquidity is advantageous. It leads to the fact that the information is more quickly absorbed in the price of one stock of the pair and not the other. A lead-lag relationship between the pairs is the result, which can be profitably exploited. 

Chen et al. (2012) confirm that pairs trading profitability is partly driven by delays in information difusion across the two legs of a pair. Also, pairs trading profitability is highest in poorer information environments. Yet, contrary to Engelberg et al. (2009), they find no evidence that relates short-term liquidity provision to pairs trading profitability. If at all, their pairs trading returns are negatively related to the Pastor-Stambaugh Liquidity factor. Additionally, their strategy performs poorly during the financial crisis in 2008, a low liquidity environment with potential rewards for liquidity providing strategies. 

Jacobs and Weber (2013) test a variant of the GGR algorithm on a subset of the U.S. market 1960 to 2008 and several international markets in order to explore the sources of pairs trading profitability. They confirm that pairs trading returns are linked to diferent difusion speeds of common information across the two securities forming a pair. In particular, pairs are more likely to open on so-called high-divergence days, where investor attention is primarily focused on the market level instead of individual stocks, due to a high quantity of unexpected new information per day. High distraction leads to a slower difusion of common information, creating profitable lead-lag relationships. Hence, pairs opened on such days are more likely to converge and thus more profitable. Jacobs and Weber (2015) expand on this study on an even larger data base consisting of a comprehensive U.S. data set and 34 international markets. They find that pairs trading returns are a persistent phenomenon. The U.S. sample reveals that profitability is mainly afected by news events causing the spread to diverge, investor attention and limits to arbitrage. Jacobs (2015) tests 20 groups of long-short anomalies - one of them is a variant of GGR’s pairs trading strategy. The author finds pairs trading to be the top 5 anomaly on a large and representative sample of U.S. stocks, with abnormal returns exceeding 100 bps per month. The strategy barely loads on investo sentiment proxies, but seems to be related to limits to arbitrage. According to Jacobs, pairs trading is one of the few anomalies with higher alpha on the long leg - contrary to the findings of GGR. 

Huck has conducted two recent pairs trading studies, evaluating potential sources of profitability. Huck (2013) finds on a S&P 500 sample that GGR’s pairs trading returns are highly sensitive to the length of the formation period. Strong positive results are achieved with durations of 6, 18 and 

24 months. Surprisingly, there is a slump in abnormal returns for the 12 months formation periods chosen ad hoc by GGR. In a later study, Huck (2015) examines the impact of volatility timing on pairs trading strategies. On an international sample of S&P 500 and Nikkei 225 constituents, he finds that pairs trading returns cannot be further improved by timing volatility with the VIX index. 

## 2.5 High frequency applications

Nath (2003) is the first author to apply a pairs trading strategy to the entire secondary market of U.S. government debt in a high frequency setting. The data stem from GovPX and range from 1994 to 2000. Nath considers all liquid securities with at least ten quotes per trading day in a 40 days formation period. He standardizes the dirty prices of all securities and calculates the SSD between the two components of each pair. For all pairs, a record of the empirical distribution of the distance metric is kept. In the subsequent 40 days trading period, trades are entered when the squared distance reaches certain trigger levels around the median, defined as percentiles of the empirical distribution function. Trades are closed upon reversion to the median, at the end of the trading period, or if the stop loss percentiles are hit. As Nath points out, there is a major divergence risk involved in this strategy. Imagine a pair starting with low SSD at the beginning of the formation period, rising to higher levels until its end. This pair is clearly diverging, yet it would immediately open at the beginning of the trading period and - if it keeps diverging - lead to a substantial loss. This downside is less expressed in GGR’s strategy, since prices are re-normalized at the beginning of the trading period, and only pairs with low SSD are considered for trading. Hence, GGR’s algorithm is less susceptible for selecting pairs with strong divergence already during the formation period. However, despite this disadvantage, Nath’s strategies outperform their benchmarks in terms of Sharpe and Gain-Loss ratio. The returns are largely uncorrelated with the market. Unfortunately, exposure to systematic risk factors has not been evaluated. 

Bowen et al. (2010) examine GGR’s pairs trading strategy on the FTSE 100 constituents from Januar to December 2007, in a true high frequency setting using 60 minute return period intervals. The authors use 264 hour formation periods and subsequent 132 hour trading periods. At first, they find intraday pairs trading to be profitable with low exposure to systematic risk factors with excess returns of approximately 20 percent per annum. However, these results are extremely sensitive to transaction costs and speed of execution. Implementing transaction costs of 15 basis points and delaying execution by a 60 minute interval leads to full elimination of excess returns. 

## 2.6 Further out-of-sample testing of GGR’s strategy

GGR’s simple and appealing algorithm has been implemented on many international samples and across diferent asset classes: Bianchi et al. (2009) examine GGR’s strategy in commodity market futures from 1990 to 2008. They find statistically and economically significant excess returns with low exposure to systematic sources of risk. Mori and Ziobrowski (2011) test GGR’s trading rule for the U.S. stock market compared to the subset of the U.S. REIT<sup>8</sup> market 1987 to 2008. Over the entire sample period, REIT pairs produce higher profits at lower risk compared to common stocks. The superiority of REITs is mainly due to the high industry homogeneity within the REIT subsegment, leading to more stable pairs with clear, long-term relationships. However, this efect disappears after the year 2000, either due to structural changes in the REIT market or due to investor recognition of pairs trading opportunities in the REIT market. Broussard and Vaihekoski (2012) replicate GGR’s algorithm for the Finnish stock market 1987 to 2008. They confirm GGR’s results for their sample while highlighting potential implementation hurdles. Bowen and Hutchinson (2014) apply GGR’s strategy to the U.K. equity market 1979 to 2012. They find statistically significant risk-adjusted excess returns that do not load on systematic risk factors. However, contrary to Chen et al. (2012), pairs trading profitability can be partly explained by liquidity provision. 

## 3. Cointegration approach

In the cointegration approach, the degree of comovement between pairs is assessed by cointegration testing, e.g., with the Engle-Granger or the Johansen method. Table 3 provides an overview. 

<table><tr><td>Study</td><td>Date</td><td>Sample</td><td>Objective</td></tr><tr><td>V</td><td>2004</td><td>-</td><td>Most widely cited cointegration-based concept</td></tr><tr><td>LMG</td><td>2006</td><td>Selected stocks 2001-2002</td><td rowspan="3">Entry/exit signals: First, development of minimum profit bounds and then of optimal pre-set boundaries for cointegration-based pairs trading</td></tr><tr><td>PLG</td><td>2010</td><td>Selected stocks 2004-2005</td></tr><tr><td>P</td><td>2012</td><td>Selected applications</td></tr><tr><td>GP</td><td>1999</td><td>Crack spread 1983-1994</td><td rowspan="5">Futures spread trading: Cointegration-based trading of the crack spread, the WTI-Brent spread, the soy crush spread, the spark spread, the gold silver spread</td></tr><tr><td>DLE</td><td>2006c</td><td>Energy futures 1995-2004</td></tr><tr><td>S</td><td>1999</td><td>Soy crush spread 1985-1995</td></tr><tr><td>EL</td><td>2002</td><td>Spark spread 1996-2000</td></tr><tr><td>WC</td><td>1994</td><td>Gold-silver spread 1988-1992</td></tr><tr><td>HS</td><td>2003</td><td>64 Asian shares/ADRs 1991-2000</td><td rowspan="2">ADRs: Cointegration-based pairs trading strategies for ADRs and the local stocks</td></tr><tr><td>BR</td><td>2012</td><td>Selected stocks 2003-2009</td></tr><tr><td>DGLR</td><td>2010</td><td>EuroStoxx 50 2003/2009-2009</td><td rowspan="4">Common stocks: Cointegration-based pairs trading frameworks with applications to the European high frequency, the Brazilian and the Chinese markets; improved selection via Granger-causality</td></tr><tr><td>CM</td><td>2013</td><td>Brazil 2005-2012</td></tr><tr><td>GT</td><td>2011</td><td>Selected stocks 1997-2008</td></tr><tr><td>LCL</td><td>2014</td><td>38 Chinese stocks 2009-2013</td></tr><tr><td>HA</td><td>2015</td><td>U.S. S&amp;P 500 2000-2011</td><td rowspan="3">Comparison studies: Comparison of univariate pairs trading strategies - most notably distance vs. different variants of cointegration approach</td></tr><tr><td>B</td><td>2011</td><td>Australia ASX 1996-2010</td></tr><tr><td>BBS</td><td>2010</td><td>U.S. DJIA 1999-2008</td></tr><tr><td>DH</td><td>2005</td><td>EuroStoxx 50 1999-2003</td><td rowspan="4">Passive index tracking/enhanced indexation: Development of multivariate cointegration-based strategies for tracking indices or artificial benchmarks</td></tr><tr><td>A</td><td>1999</td><td>Intl&#x27; indexes 1990-1998</td></tr><tr><td>A</td><td>2001</td><td>U.S. S&amp;P 100 1995-2000</td></tr><tr><td>AD</td><td>2005</td><td>U.S. DJIA 1990-2003</td></tr><tr><td>GPP</td><td>2012</td><td>Intl&#x27; indexes 2003-2009</td><td rowspan="2">Cointegration-based multivariate statistical arbitrage approaches</td></tr><tr><td>B</td><td>2003</td><td>EuroStoxx 50 1998-2002</td></tr><tr><td>B</td><td>1999</td><td>U.K. FTSE 100 1997-1999</td><td>Multivariate statistical arbitrage approach based on cointegration and machine learning techniques</td></tr><tr><td>D</td><td>2011</td><td>U.S. Swap rates 1998-2005</td><td>Identification of sparse mean-reverting portfolios</td></tr><tr><td>K</td><td>2009</td><td>U.S. dual class firms 1980-2006</td><td rowspan="2">Fractional cointegration: Pairs trading approaches based on fractional cointegration</td></tr><tr><td>LC</td><td>2003</td><td>Gold-silver futures 1983-1995</td></tr><tr><td>PKLMG</td><td>2011</td><td>Selected securities 1999-2005</td><td rowspan="3">Bayesian approach: Development of Bayesian approaches for cointegration-based pairs trading</td></tr><tr><td>GHV</td><td>2011</td><td>Selected securities 2009-2009</td></tr><tr><td>GHLV</td><td>2014</td><td>U.S. DJIA 2009-2009</td></tr><tr><td>CYP</td><td>2011</td><td>Selected stocks 2005-2008</td><td>Cointegration-based pairs trading framework with logistic mixture AR equilibrium errors</td></tr></table>


Table 3: Cointegration approach


## 3.1 Univariate pairs trading

3.1.1 Development of a theoretical framework: Vidyamurthy (2004) provides the most cited work for this approach. He develops an univariate cointegration approach to pairs trading as a theoretical framework without empirical applications. The design is generally ad-hoc and for practitioners, yet with many relevant insights. The framework relies on three key steps: (1) Preselection of potentially cointegrated pairs, based on statistical or fundamental information. (2) Testing for tradability according to a proprietary approach. (3) Trading rule design with nonparametric methods. Along the entire process, Vidyamurthy does not perform rigorous cointegration testing, but instead opts for a practical approach. However, the guiding principle behind his framework is the idea of cointegrated pairs. For similar discussions of Vidyamurthy’s approach, see Do et al. (2006) and Puspaningrum (2012). 

Preselection: First, Vidyamurthy takes advantage of the common trends model (CTM) of Stock and Watson (1988) to decompose the log price $p _ { i t }$ of a security i in a nonstationary, common trends component $n _ { i t }$ and a stationary, idiosyncratic component $\epsilon _ { i t }$ . Along the same line, its return $r _ { i t }$ consists of a common trends return $r _ { i t } ^ { c }$ and a specific return $r _ { i t } ^ { s }$ . Now, consider a portfolio long one share of security i and short $\gamma$ shares of security $j$ . The portfolio price time series is the spread $m _ { i j t }$ between the two securities and the return time series its first diference $\Delta m _ { i j t }$ : 

$$
m _ {i j t} = p _ {i t} - \gamma p _ {j t} = n _ {i t} - \gamma n _ {j t} + \epsilon_ {i t} - \gamma \epsilon_ {j t}\tag{8}
$$

$$
\Delta m _ {i j t} = r _ {i j t} = r _ {i t} ^ {c} - \gamma r _ {j t} ^ {c} + r _ {i t} ^ {s} - \gamma r _ {j t} ^ {s}\tag{9}
$$

For this pair to be cointegrated, the common return components should be identical up to a scalar $\gamma ,$ the cointegration coeficient. Then, they cancel each other out and the spread time series is stationary. Vidyamurthy (2004) uses Arbitrage Pricing Theory (APT) of Ross (1976) to identify stocks with similar common return components. With APT in form of an orthogonal statistical factor model the return of stock i can be expressed as follows (Tsay, 2010) : 

$$
r _ {i t} - \mu_ {i} = \beta_ {i} ^ {\prime} f _ {t} + \epsilon_ {i t}\tag{10}
$$

Thereby, $\beta _ { i }$ denotes a $k \times 1$ vector of factor loadings for stock i, $\mathbf { \nabla } f _ { t }$ contains the $k \times 1$ factor returns and $\epsilon _ { i t }$ is the idiosyncratic error of $r _ { i t }$ . Note that Vidyamurthy either neglects the mean return $\mu _ { i }$ or implicitly assumes that returns are standardized. In the following, we shall opt for the latter, so that $\mu _ { i }$ equals to zero. Vidyamurthy asserts that if APT holds true for all time periods, then stocks i and $j$ form a cointegrated system in case their factor loadings $\beta _ { i }$ and $\beta _ { j }$ are identical up to a scalar $\gamma$ . As such, the portfolio returns can be expressed as follows: 

$$
r _ {i j t} = r _ {i t} - \gamma r _ {j t} = \beta_ {i} ^ {\prime} f _ {t} - \gamma \beta_ {j} ^ {\prime} f _ {t} + \epsilon_ {i t} - \gamma \epsilon_ {j t} = \epsilon_ {i t} - \gamma \epsilon_ {j t}\tag{11}
$$

When comparing equation (8) with (11), Vidyamurthy suggests that the common trend returns of the CTM correspond to the common factor returns of APT and the specific returns of the CTM correspond to the idiosyncratic returns of APT. According to Vidyamurthy’s model, equation (11) refers to a perfectly cointegrated pair, where common factor returns are identical up to a scalar and cancel each other out. Spoken in practical terms, a preselection of potentially cointegrated stocks can now be based on a measure of similarity of common factor returns. For this purpose, Vidyamurthy introduces a distance metric based on the absolute value of the Pearson correlation coeficient of the common factor returns and suggests to rank all possible combinations of pairs in descending order. Following this theory, the top pairs of the ranking have a higher probability of being cointegrated and thus of being suitable for trading. 

This framework is definitely hands-on and thus appealing from a practitioner’s perspective. However, Vidyamurthy’s descriptions are often informal and they leave wide space for interpretation. First, the unconventional combination of CTM and APT requires further scrutiny, especially regarding the assumption that APT holds true for all time periods. Second, Vidyamurthy provides no guidance on the selection of an adequate factor model. Avellaneda and Lee (2010) find that in the case of a statistical factor model, between 10 and 30 factors are required in the U.S. stock universe to explain a mere 50 percent of the variance of individual stock returns. In Vidyamurthy’s world, the unexplained other half would be interpreted as the idiosyncratic component of an asset’s returns - a quite high share. It is thus highly doubtful if this component truly corresponds to the stationary part in the common trends model and if any links to cointegration can be drawn. Nevertheless, Chen et al. (2012) empirically show that pairs trading based on common factor correlation exhibits much higher excess returns than pairs trading based on residual correlation. These findings may carefully be interpreted as empirical support for Vidyamurthy’s framework. Third, key parameter values are yet to be determined, such as the time frame to be considered for the preselection ranking or the minimum threshold values that indicate potentially cointegrated pairs. In summary, the preselection algorithm constitutes an appealing concept and it would be interesting to see how it actually fares on empirical data. 

Testing for tradability: In the next step, the log prices of the preselected pairs are regressed according to the following linear model: 

$$
p _ {i t} = \mu + \gamma p _ {j t} + \epsilon_ {i j t}\tag{12}
$$

Thereby, the intercept $\mu$ denotes the premium paid for holding stock i versus stock $j ,$ $\gamma$ is the coeficient of (quasi-)cointegration and $\epsilon _ { i j t }$ is the resulting spread time series. In a standard cointegration test such as the Engle-Granger approach in Engle and Granger (1987), we would test the residuals for stationarity with an adequate unit root test. However, Vidyamurthy prefers a less strict variant adapted to the primary objective of tradability testing. Key for a practitioner is not necessarily a cointegrated pair, but a spread with strong mean-reversion properties. A valid proxy for the latter is the zero-crossing frequency or its inverse, the time between two zero-crossings. Vidyamurthy suggests a bootstrap to estimate the standard errors for this average holding time of a pair. It may be an enhancement to consider a stationary bootstrap, following Politis and Romano (1994) in this time series context. Also, formal cointegration testing on the remaining suitable pairs with a high zero-crossing rate may further improve the suggested framework. 

Trading rule design: Vidyamurthy proposes a simple nonparametric approach in line with Gatev et al. (1999), meaning that a pairs trade is triggered when the spread deviates k standard deviations from its mean and closed upon mean-reversion. Whereas GGR fix the opening threshold at two standard deviations to avoid data snooping, Vidyamurthy develops an optimization routine to find the optimal trigger level k specific for each pair. At first, for each observation of the spread time series, the absolute value of the delta to the historical mean is calculated. Next, it is simply suggested to count the number of times each trigger level is exceeded. The total profit per threshold level is the number of occurrences times the delta to the mean. Whichever threshold level maximizes total profit is selected and assumed to be optimal. This assertion is clearly incorrect. 

The empirical distribution function Vidyamurthy proposes to evaluate here obviously loses the time ordering of the observations. Imagine the ”optimal” threshold level to be hit on the last day of trading. Clearly, the position is opened, but the profit equals to zero. A better approach would be to avoid optimization altogether as in GGR or to retain the time ordering by actually evaluating the trading profit for each trigger level. Of course, the latter is computationally more intensive, but at least the results are meaningful. 

In summary, Vidyamurthy proposes an appealing conceptual pairs trading framework from a practitioners point of view. It would be interesting to see how the idea of preselecting pairs based on similarity in common factor returns and evaluating tradability by counting the number of zerocrossings compares to the distance approach on actual market data. This is subject for further research. 

3.1.2 A deep-dive on the development of optimal trading thresholds: Lin et al. (2006) develop a minimum profit condition for a cointegrated pair of securities. They start with a pair of stocks that is cointegrated over the relevant time horizon in the following sense: 

$$
P _ {i t} + \gamma P _ {j t} = \epsilon_ {i j t}\tag{13}
$$

This regression is similar to equation (12), except that we use level prices here and that the intercept $\mu$ is neglected. The errors $\epsilon _ { i j t }$ are stationary and $\gamma$ is assumed to be less than zero on all occasions. Stock i is used for short positions and stock $j$ for long positions. Naturally, the price of $j$ at the opening of the trade is always lower than the price of i. For each n shares long of stock $j , n / | \gamma |$ shares of stock i are held short in one pair, i.e., the proportion of shares held is determined by the cointegrating relationship. When $t _ { o }$ denotes opening time and $t _ { c }$ closing time of a trade, and we use the relation from (13), the total profit per trade $T P _ { i j t _ { c } }$ amounts to: 

$$
T P _ {i j t _ {c}} = \frac {n}{\gamma} \left[ (\epsilon_ {i j t _ {c}} - P _ {i t _ {c}}) - (\epsilon_ {i j t _ {o}} - P _ {i t _ {o}}) \right] + \frac {n}{| \gamma |} [ P _ {i t _ {o}} - P _ {i t _ {c}} ] = \frac {n (\epsilon_ {i j t _ {o}} - \epsilon_ {i j t _ {c}})}{| \gamma |} > K\tag{14}
$$

If a trader sets the minimum required profit per trade to K and chooses the entry threshold $\epsilon _ { i j t _ { o } }$ and exit threshold $\epsilon _ { i j t _ { c } }$ , the number of shares n can be calculated according to (14). Lin et al. test this approach for diferent entry and exit thresholds in a simulation study and on one exemplary stock pair. The concept has several weaknesses. First, the minimum profit per trade is set in absolute terms, so the profitability scaled by initial investment can become quite low, which Lin et al. confirm in their application. Second, the simulation study lacks diversity: only one cointegration model is tested, from which 100 samples with 500 data points are drawn. It would be interesting to see how the trading rule performs in diferent cointegration settings and also in models that allow for the cointegration relationship to break. Third, the empirical application is limited to two stocks and a time frame of less than two years. Clearly, this is not representative. Fourth, as Vidyamurthy (2004) points out, total profit over a trading period is a function of the number of trades and the trading thresholds, i.e., the profit per trade. As such, optimizing the profit per trade usually does not optimize the total profit over the trading horizon, since a higher minimum profit per trade leads to a lower number of trades and vice versa. The latter point is addressed in a subsequent paper by Puspaningrum et al. (2010). They fit an $\mathrm { A R } ( 1 )$ process to the spread $\epsilon _ { i j t }$ of two cointegrated stocks and use an integral equation approach to numerically evaluate the estimated number of trades for any given trading threshold / minimum profit per trade. This approach allows for the optimization of total profit per trading period and constitutes an enhancement versus Lin et al. However, also the latter concept has not yet been empirically tested on a representative data set. 

3.1.3 Putting the frameworks to action - empirical applications: The first empirical applications of the univariate cointegration approach are found in the domain of futures markets under the keyword ”spread trading”. A representative study of this kind is by Girma and Paulson (1999). They focus on the ”crack spread”, i.e., the price diference between petroleum futures and futures on its refined end products, such as gasoline and heating oil from 1983 to 1994. Diferent variants of this spread are stationary according to the Augmented Dickey-Fuller (ADF) and the Phillips-Perron (PP) test statistics. Trades are entered when the spread deviates a multiple k of its cross-sectional standard deviation from its cross-sectional moving average, both calculated over n−days and all available contract months. Positions are closed when the spread returns to its own n−day moving average (not the cross-sectional one). Girma and Paulson (1999) test both 5 and 10-day moving averages and five diferent entry thresholds. The results are promising: After consideration of USD 100 transaction costs per full turn, the average annual return still exceeds 

15 percent<sup>9</sup>. This direction of research is promising, since there is a clear fundamental reason for the cointegration relationship between crude oil and its end products. Dunis et al. (2006c) and Cummins and Bucca (2012) confirm the profit potential for the crack spread in later years with diferent trading models. A comparable ansatz as in Girma and Paulson (1999) is followed by Simon (1999) and proves successful for the crush spread, i.e., the diference between soybean futures prices and its end products. Similarly, Emery and Liu (2002) analyze the spark spread, i.e., the diference between natural gas and electricity futures prices with positive results. However, in case of the gold-silver spread, Wahab and Cohn (1994) find trading to be unsuccessful. 

Hong and Susmel (2003) are the first authors to implement a rudimentary version of the cointegration approach to common stocks. They choose 64 American Depositary Receipts (ADRs) and the corresponding shares in the local markets from 1991 to 2000. Hong and Susmel assume these pairs to be cointegrated, but provide no test results in their paper. Also, they do not calculate the spread according to the cointegration relationship as in equation (12) or (13), but on a 1:1 basis in terms of share prices. Pairs trades are entered when the spread diverges more than a fixed threshold and reversed upon return to a equilibrium relationship. However, the exact threshold levels are not given in the text. Only ADRs may be shorted due to potential short selling restrictions in local markets. Despite the methodological weaknesses in terms of cointegration testing, the results are impressive with annualized returns of 33 percent.<sup>10</sup> However, Broumandi and Reuber (2012) note that these large returns may well be driven by an appreciation of local currencies, which casts doubt on the findings. 

Dunis et al. (2010) test the univariate cointegration approach in a daily and a high frequency setting on the constituents of the EuroStoxx 50 index. They restrict pairs formation to ten industry groups and come up with 176 possible pairs, which may or may not be cointegrated. The spread for each pair is calculated as follows: 

$$
\epsilon_ {i j t} = P _ {i t} - \gamma_ {t} P _ {j t}\tag{15}
$$

The time-varying parameter $\gamma _ { t }$ is estimated with the Kalman Filter, which performs best versus other estimation methods in this paper. Next, the spreads of all pairs are calculated with equation (15), standardized and then traded according to a simple standard deviation logic similar to GGR, after a waiting time of one period to avoid bid-ask bounce. However, if pairs formation simply relies on industry classification, the out-of-sample results are not very convincing. Therefore, Dunis et al. test the relationship between several in-sample indicators and out-of-sample information ratios with a nonparametric bootstrap. They find that in-sample t-statistics of the ADF test as part of the Engle-Granger cointegration test and the in-sample information ratio seem to have a certain predictive power for the out-of-sample information ratio. Hence, it is not surprising that they realize much better out-of-sample information ratios when they only trade the top five pairs preselected by one or both of these indicators. This approach is definitely appealing, and it should be tested on a larger data set so that more than the top five pairs can be selected for trading and their returns tested for statistical significance. Also, only the ADF test statistics have been used for constructing a ranking, but no cut-of points are defined. It would be interesting to see if test statistics above a critical value lead to an even higher out-of-sample performance. In subsequent analyses, it should be considered to include an intercept in equation (15). The authors neglect it with the following argument: ”Intuitively speaking, when the price of one share goes to 0, why would there be any threshold level under which the price of the second share cannot fall?” (Dunis et al., 2010, p. 9). This assertion is incorrect. According to Vidyamurthy (2004), the intercept can be interpreted as the premium paid of holding stock i versus stock $j .$ . For example, if stocks i and j are identical, but $j$ has twice the leverage ratio, it may well be the case that stock $j$ goes bankrupt in a situation of financial distress, whereas stock i survives. An intercept thus helps to better reflect the relationship between the two securities that form a pair. Finally, the study is missing any attempt to explain the returns by their loadings on standard risk factors as in GGR. 

Caldeira and Moura (2013) apply the univariate cointegration approach to the 50 most liquid stocks of the Brazilian stock index IBovespa. They define a spread equation similar to (12) and use the Engle-Granger two-step approach as well as the Johansen method at the five percent significance level to test for cointegration relationships for all 1225 combinations of pairs over a one year formation period. On average, they find 90 cointegrated pairs. Following Dunis et al. (2010), these pairs are ranked according to the in-sample Sharpe ratio. The top 20 pairs of this ranking are selected for a subsequent four months trading period. Positions are opened and closed based on a modified standard deviation rule similar to GGR. Caldeira and Moura (2013) show statistically significant excess returns after consideration of transaction costs that are robust to data snooping based on White’s reality check and Hansen’s SPA test. Also, the returns are significantly diferen when compared to the returns of randomized pairs trading according to a bootstrapping procedure. These results are definitely convincing for this emerging market. However, one key improvement for future studies in this area is the necessity to control for multiple comparison settings. Clearly, the Engle-Granger and the Johansen tests are not statistically independent when used on the same data set. On the contrary, in most cases they would probably lead to the same result. For simplicity’s sake, let us assume the latter fact were the case. Cointegration testing on 1225 pairs would thus produce 61 cointegrated pairs as false positives in expectation, at the five percent significance level the authors used. Even though this estimate is aggressive, Caldeira and Moura most likely have a significant share of false positives in their rankings. However, the subsequent heuristic of filtering the pairs by in-sample Sharpe ratio most likely improves tradability. Nevertheless, it would be an improvement to actively control for familywise error rate, for example as in Cummins and Bucca (2012). 

Gutierrez and Tse (2011) provide an appealing conceptual framework, that is unfortunately only applied to three stocks in the water utility sector. The authors first perform cointegration testing with the Engle-Granger and with the Johansen procedure. All three possible pairs are cointegrated according to both tests, so Gutierrez and Tse estimate their respective error correction models with OLS. Next, the Granger-leaders and Granger-followers of each pair are identified. When a classical pairs trading strategy similar to GGR is applied to these pairs, the key finding of the authors is that the majority of profitability stems from the Granger-follower, whereas the Granger-leader barely contributes. Even though the results are statistically not representative, the concept is appealing and deserves more rigorous testing on a larger sample. 

Finally, there is a set of further applications: Li et al. (2014) show that cointegration-based pairs trading is profitable in the Chinese AH-share markets. Baronyan et al. (2010) evaluate a set of 14 market-neutral trading strategies on the constituents of the Dow Jones Industrial Average. Similar to Gutierrez and Tse, they find improved performance in case Granger causality testing is taken into account. Huck and Afawubo (2015) also run a comparison study. They analyze the cointegration approach and the distance approach for the S&P 500 constituents and under varying parametrizations. After consideration of risk loadings and transaction costs, they find that the cointegration approach significantly outperforms the distance method. The latter fact corroborates the hypothesis that the cointegration approach identifies econometrically more sound equilibrium relationships. Bogomolov (2011) arrives at a similar conclusion for the Australian stock market. 

## 3.2 Multivariate cointegration approach

3.2.1 Passive index tracking and advanced indexation strategies: In the article of Dunis and Ho (2005), two objectives are pursued. First, the authors use cointegration relationships to construct index tracking portfolios for the EuroStoxx 50 index. More specifically, Dunis and Ho take diferent subsets (5, 10, 15 or 20 stocks) of the index constituents and estimate the joint cointegration vector for these constituents and the EuroStoxx 50 index. Then, they measure the tracking error return of this basket versus the index for diferent rebalancing frequencies. They find that the tracking baskets produce a positive tracking error, resulting in an outperformance versus the benchmark in terms of absolute returns and Sharpe ratio. Second, Dunis and Ho pursue an advanced indexation strategy. Such an approach is characterized by creating tracking baskets for artificial benchmarks. A synthetic ”plus” benchmark is constructed by adding uniformly distributed returns amounting to z percent p.a. to the daily returns of the EuroStoxx 50. Analogously, a ”minus” benchmark can be created. Next, the Johansen procedure is used to find adequate securities among the 50 index constituents to track these benchmarks. According to Dunis and Ho (2005), going long the ”plus” benchmark and short the ”minus” benchmark allows for a market neutral investment strategy with potential ”double alpha”. The authors find significant outperformance of their market neutral strategies compared to the EuroStoxx 50 index. Alexander (1999), Alexander (2001) and Alexander and Dimitriu (2005) develop very similar strategies to Dunis and Ho. However, all these enhanced indexation strategies have one key issue. Whereas the index tracking strategy relies on a ”natural” cointegration relationship between the index and its constituents, it is troubling to make such an assumption for the artificial benchmark. Alexander and Dimitriu (2005) also follow this approach, even though Alexander (1999) herself shows in a powerful example that when we add a miniscule daily incremental return to one of two cointegrated time series, this may break up the entire cointegration relationship (Alexander, 1999). 

3.2.2 Active statistical arbitrage strategies: In the previous section, tracking and enhanced indexation strategies have been discussed. These are passive or enhanced passive strategies, since they are closely tied to an underlying index as benchmark (Galenko et al., 2012). On the contrary, Galenko et al. (2012) develop an active statistical arbitrage strategy. They aim at developing an approach similar to that of GGR, but based on a multivariate cointegration framework. Whereas correlation reflects short-term linear dependence in returns, cointegration models long-term depen dencies in prices (Alexander, 2001). As such, compared to the distance methods from section $2 ,$ the approach of Galenko et al. (2012) has a higher potential of identifying true long-term equilibrium relationships between several assets. Their framework heavily relies on properties they develop for the return process $Z _ { t }$ of cointegrated assets. The latter is defined as weighted sum of asset returns $r _ { i t }$ , where the weighting scheme is according to the components of the cointegration vector $\gamma$ . The authors are able to show that this weighted return process is mean-reverting under certain conditions. A trading strategy capitalizing on this mean-reversion efect is shown to have positive expected profits. Empirical applications on several index exchange traded funds (ETFs) result in an outperformance compared to the benchmark. However, Galenko et al. (2012) perform extensive data mining exercises. First, they apply their strategy to daily and weekly data. Second, for each of these setups, they take a diferent duration of the formation period to estimate the cointegration vector. Finally, they test nine diferent lag parameters $p ,$ over which the return process is cumulated to a price time series. The latter fact is especially troublesome, considering that p should be infinity based on their theoretical trading model (Galenko et al., 2012, p. 94). It is thus unclear, why they also experiment with very short-term values for $p ,$ such as 5 days. Also, the excess returns are not tested for statistical significance. In conclusion, the study in this setup suggests an interesting and theoretically sound trading framework, but the empirical application is susceptible to data snooping. It would be interesting to see if the results are statistically significant on a larger sample and with a fixed set of parameter values chosen in accordance with their theories. 

## 3.3 Adjacent developments

Burgess (1999) surpasses the models presented so far in terms of complexity. In his thesis, he develops a holistic statistical arbitrage framework relying on a combination of cointegration and emerging techniques such as neural networks and genetic algorithms. In the first part of his work, he uses cointegration to construct time series having a significant predictable component. The second part uses neural networks in an attempt to forecast these predictable components, taking into account potential nonlinearities in the asset price dynamics. The third part is concerned with risk reduction through diversification and relies on a combination of portfolios, which are automatically selected with genetic algorithms. The framework of this dissertation is definitely appealing. Unfortunately, the empirical application is limited to FTSE 100 constituents and selected international stock indices. To our knowledge, no other author has followed this direction, most likely due to the high complexity and the ”black-box” character of neural networks and genetic algorithms. In later years, Burgess (2003) has published a simplified variant of his approach, solely relying on cointegration testing. D’Aspremont (2011) uses canonical correlation analysis to construct mean-reverting portfolios with a limited number of assets. Karakas (2009) applies fractional cointegration to dual class firms and Liu and Chou (2003) to gold and silver markets. Finally, Peters et al. (2011), Gatarek et al. (2011) and Gatarek et al. (2014) use Bayesian procedures for cointegration testing and apply them to a very limited set of securities. Finally, Cheng et al. (2011) develop a statistical arbitrage strategy with a cointegration model based on logistic mixture auto-regressive equilibrium errors. 

## 4. Time series approach

This section provides a comprehensive treatment of the time series approach. Its main objective is the modeling of mean-reversion with other time series methods than cointegration. A concise overview with relevant studies, their data samples and objectives is provided in table 4. 

## 4.1 Modeling the spread in state space

Elliott et al. (2005) are the most cited authors in this domain. They explicitly describe the spread with a mean-reverting Gaussian Markov chain, observed in Gaussian noise. The latter can be achieved with a state space model, consisting of a state and a measurement equation. We will briefly present Elliot et. al’s approach, starting with the state equation: It is assumed that the latent state variable $x _ { k }$ follows a mean-reverting process: 

<table><tr><td>Study</td><td>Date</td><td>Sample</td><td>Objective</td></tr><tr><td>EVM</td><td>2005</td><td>-</td><td>Modeling the spread in state space at the price level</td></tr><tr><td>DFH</td><td>2006</td><td>-</td><td>Modeling the spread in state space at the return level</td></tr><tr><td>TM</td><td>2011</td><td>Selected stocks 1980-2008</td><td>Modeling the spread in state space with a Bayesian approach</td></tr><tr><td>B</td><td>2010</td><td>-</td><td rowspan="5">Modeling the spread with OU processes; Development of optimal entry and exit thresholds; Selected empirical applications, also in high frequency settings</td></tr><tr><td>CB</td><td>2012</td><td>Energy futures 2003-2010</td></tr><tr><td>R</td><td>2007</td><td>-</td></tr><tr><td>K</td><td>2011</td><td>Korea KOSPI 2008-2010</td></tr><tr><td>ZL</td><td>2014</td><td>Selected stocks</td></tr><tr><td>BM</td><td>2009</td><td>DJ STOXX 600 2006-2007</td><td rowspan="4">Further time-series approaches for spread modeling: Markov regime-switching; profit model based on OU-process; nonparametric approach with renko and kagi; three regime TAR-GARCH</td></tr><tr><td>KRF</td><td>2010</td><td>Energy futures 2000-2008</td></tr><tr><td>B</td><td>2013</td><td>U.S.; Australia; 1996-2011</td></tr><tr><td>CCC</td><td>2014</td><td>U.S. DJIA 2006-2013</td></tr></table>


Table 4: Time series approach


$$
x _ {k + 1} - x _ {k} = (a - b x _ {k}) \tau + \sigma \sqrt {\tau} \epsilon_ {k + 1}\tag{16}
$$

Thereby, $a \in \mathcal { R } _ { 0 } ^ { + } , b > 0 , \sigma \geq 0$ and $\epsilon _ { k } \overset { i i d } { \sim } \mathcal { N } ( 0 , 1 )$ . Time $t _ { k } = k \tau$ for $k = 0 , 1 , 2 , \ldots$ . is discrete. This process reverts to its mean $\mu = a / b$ with mean-reversion strength b. It can also be written as: 

$$
x _ {k + 1} = A + B x _ {k} + C \epsilon_ {k + 1},\tag{17}
$$

where $A = a \tau$ ， $B = 1 - b \tau$ and $C = \sigma \sqrt { \tau }$ . In continuous time, it is possible to describe the state process with the well-known Ornstein-Uhlenbeck process: 

$$
\mathrm{d} x _ {t} = \rho (\mu - x _ {t}) \mathrm{d} t + \sigma \mathrm{d} W _ {t},\tag{18}
$$

where $\mathrm { d } { \boldsymbol { W } _ { t } }$ is a standard Brownian motion defined on some probability space. The parameter $\mu = a / b$ denotes the mean and $\rho = b$ describes the speed of mean-reversion. The second component to a state space model is the measurement equation: Here, the observed spread is defined as the sum of the state variable $x _ { k }$ and some Gaussian noise $\omega _ { t } \stackrel { i i d } { \sim } \mathcal { N } ( 0 , 1 )$ 

$$
y _ {k} = x _ {k} + D \omega_ {k}, \quad D > 0\tag{19}
$$

According to this model, a pairs trade is entered when $y _ { k } \ge \mu + c \left( \sigma / \sqrt { 2 \rho } \right)$ , or when $y _ { k } \le \mu - c \left( \sigma / \sqrt { 2 \rho } \right)$ . Thereby, c denotes a fixed parameter, for which Elliott et al. give no guidance on how to determine it. The position is reversed at time $T ,$ which denotes the first passage time result for the Ornstein-Uhlenbeck process. Following Do et al. (2006), this approach has three key advantages: First, the model is fully tractable, meaning that its parameters can be estimated using the Kalman Filter and the state space model. The estimator is based on maximum likelihood and thus optimal in terms of minimum mean squared error. There are well-known implementations at hand; Elliott et al. (2005) use the Shumway and Stofer version of the Expectation Maximization (EM) algorithm. Second, the continuous time model can be exploited for forecasting purposes. Critical questions about pairs trading such as the expected holding times and the expected returns can be explicitly answered, provided the fact that the spread really follows this rigid model. Third, the approach is fundamentally based on mean-reversion, which is key to pairs trading. However, Do et al. (2006) also criticize the model of Elliott et al. First, they remark that the spread process should be defined as the diference of log prices, not of level prices. Only then, the mean of the spread remains the same when the two stocks produce exactly the same returns (except when they trade at similar price points). This critique reflects the return perspective, but not the price perspective. Consider for example the cointegration regression in (12) with log prices and its counterpart with level prices. The log regression can be interpreted as follows: When the price of stock $j$ rises by one percent, the price of stock i rises by $\gamma$ percent. Thus, the corresponding log spread remains constant in case the number of stocks in the portfolio is in line with their cointegration vector. On the contrary, the level spread changes. The interpretation of the level regression is slightly diferent: When the price of stock $j$ rises by one infinitesimal unit, the price of stock i rises by $\gamma$ infinitesimal units. Thus, the corresponding level spread remains constant in case the number of stocks in the portfolio is in line with their cointegration vector. On the contrary, the log spread changes. As such, it is just a matter of perspective if log prices or level prices are to be preferred. However, as Puspaningrum (2012) remarks, it should be clear that a simple log transformation does not establish mean-reversion in the spread price time series. For this efect, a stock pair with an underlying equilibrium relationship needs to be identified. Second, Do et al. (2006) point out that this rigid model is only applicable to securities in return parity - a phenomenon which is rarely observed in practice. Exceptions are dual listed companies or cross-listings, limiting the applicability of this strategy to a small subset of securities. This assertion is basically valid, but variants of the concept have yet been applied to other securities in later years: For example, Avellaneda and Lee (2010) or D’Aspremont (2011) develop synthetic mean-reverting portfolios and the former authors successfully apply a variant of Elliott et al’s approach to their synthetic spread time series. The third relevant critique is provided by Cummins and Bucca (2012): A major limitation lies in the Gaussian nature of the OU-process, which is in conflict with the stylized facts of financial data. However, this disadvantage is largely compensated by the analytic simplicity associated with the OU-process. Thus, the work of Elliott et al. (2005) constitutes a valuable asset to pairs trading research and potentially a true improvement compared to nonparametric trading rules. 

Following the ansatz of Elliott et al. (2005), Do et al. (2006) develop a pairs trading approach that models mispricing at the return level, instead of the price level. Their proposed state space model can be briefly summarized as follows (Puspaningrum, 2012, p. 27): 

$$
x _ {k + 1} = A + B x _ {k} + C \epsilon_ {k + 1}\tag{20}
$$

$$
y _ {k} = x _ {k} + \Gamma U _ {k} + D \omega_ {k}\tag{21}
$$

This representation is very similar to equations (17) and (19) of Elliott et al. (2005). The first diference is that $y _ { k }$ is the observed spread defined as the diference of asset returns of the two stocks of a pair. The second adjustment consists of the loading matrix Γ and the variable $U _ { k }$ , which are exogenous inputs stemming from APT. Essentially, Do et al. use APT in a similar fashion as Vidyamurthy (2004) to generate a fundamental justification for their pairs trading framework. For further details, see (Do et al., 2006, p. 10 f). Similar to Elliott et al., the authors discuss diferent estimation procedures and also opt for the EM algorithm. Once all parameters are estimated, a long-short position is to be taken whenever the accumulated spread over a given time frame exceeds certain threshold values. However, these thresholds and the expected holding time are not further specified and have to be evaluated for a potential implementation. The same applies for the time frame over which they suggest to accumulate the residual spread to detect deviations from equilibrium. Here, it is insightful to draw parallels to Galenko et al. (2012), who also base their trading framework on return properties and an accumulated return time series: Galenko et al. in theory suggest an infinite time frame to accumulate returns. If the pairs of Do et al. were cointegrated in the sense of Galenko et al., this notion should also be applicable here. The authors finally demonstrate their model in a simulation study and in a small empirical application to a few selected securities. However, as Puspaningrum (2012) points out, they use a down-sized version of their model, which relies on the one factor CAPM instead of the multiple factor APT. Considering rising computing power, it should not pose a problem to apply the fully-fledged concept to a larger sample. It would be interesting to see how this appealing approach would fare in a large-scale empirical application - especially compared to Elliott et al. and Bertram (2010). 

Triantafyllopoulos and Montana (2011) also build on the model of Elliott et al. and enhance it in two key respects: First, they introduce time-dependency in the parameters of the model, which improves its flexibility. Second, the authors replace the EM algorithm with a Bayesian framework for parameter estimation. The latter is particularly useful for applications in high frequency settings due to faster convergence times. 

## 4.2 Applications of the Ornstein-Uhlenbeck process

Bertram (2010) develops a statistical arbitrage trading model for a spread $x _ { t }$ between two log price time series. The latter is assumed to follow a zero-mean, symmetric Ornstein-Uhlenbeck process: 

$$
\mathrm{d} x _ {t} = - \kappa x _ {t} \mathrm{d} t + \sigma \mathrm{d} W _ {t}\tag{22}
$$

Bertram now defines a trade cycle as follows: Let a be the threshold level to enter a trade and m the threshold level to exit a trade. Thereby, we assume that $a < m ,$ , so we $_ \mathrm { g o }$ long the spread at level a and reverse the positions at level m. The cycle time $\tau$ can be split up in two subperiods: 

$$
\mathcal {T} = \mathcal {T} _ {1} + \mathcal {T} _ {2},\tag{23}
$$

where $\mathcal { T } _ { 1 }$ is the time the process takes to transition from entry to exit and $\mathcal { T } _ { 2 }$ the time from exit to a subsequent entry. The times $\mathcal { T } _ { 1 }$ and $\mathcal { T } _ { 2 }$ are independent, due to the Markovian property of the OU-process. Considering relative transaction costs $^ { c , }$ the total log return per trade cycle can be defined as a function of the trigger thresholds and the transaction costs: $r ( a , m , c ) = m - a - c .$ Since the OU-process is stationary, this return is deterministic. In contrast, the associated cycle time is stochastic. With trade frequency following a renewal process, Bertram uses renewal theory to derive the following expressions for expected return and variance per unit time: 

$$
\mu (a, m, c) = \frac {r (a , m , c)}{\operatorname{E} (\mathcal {T})}
$$

$$
\sigma^ {2} (a, m, c) = \frac {r ^ {2} (a , m , c) \mathrm{VAR} (\mathcal {T})}{E ^ {3} (\mathcal {T})}\tag{24}
$$

(25) 

Next, Itˆo’s lemma is used to transform the OU-process to a dimensionless system in order to simplify the analysis. Leveraging first passage time theory about the OU process finally allows Bertram to derive analytic expressions for the expected trade length and its variance. With the help of these formulas, closed-form solutions for the expected return and the Sharpe ratio of the strategy are developed, both per unit time. Applying straightforward optimization routines to these equations results in optimal entry $a ^ { * }$ and exit thresholds $m ^ { * }$ , corresponding to maximum return or Sharpe ratio. As Bertram himself points out, the downside of this approach is once again the fact that a Gaussian OU-process is applied to non-Gaussian financial data. On the other hand, the upside lies in the availability of closed-form solutions. The latter allows for analytic investigations of the spread dynamics and for implementations in high frequency settings, which demand for computationally eficient solutions. Bertram empirically applies his strategy to a pair of dual-listed securities. Cummins and Bucca (2012) perform a large-scale implementation of this strategy to 861 energy futures spreads from 2003-2010. After rigorously controlling for data snooping bias following procedures of Romano and Wolf (2007) as well as Romano et al. (2010), they find that the daily returns of their top strategies amount to 0.07 to 0.55 percent. The corresponding Sharpe ratios are often larger than two. This study is striking evidence for the profit potential of Bertram’s approach. It is worth of further investigation. On the one hand, it could be conceptually enhanced by applying Bertram’s method to non-Gaussian processes, thus better reflecting the stylized facts of financial data. On the other hand, it would be interesting to see if the results of Cummins and Bucca (2012) can be replicated in other asset classes. 

Further discussions of the Ornstein-Uhlenbeck process in the context of pairs trading can be found in Rampertshammer (2007). Kim (2011) provides an empirical implementation in a high frequency setting in the Korean stock market. Zeng and Lee (2014) provide a recent extension of Bertram’s ansatz. 

## 4.3 Further concepts from time series analysis

The field of time series analysis is vast and equally numerous are the methods that could potentially be applied to develop trading systems for mean-reverting spreads. This section briefly names other relevant papers in this context. Bock and Mestel (2009) use a Markov switching model to develop a pairs trading system. Kanamura et al. (2010) derive a profit model for spread trading based on a mean-reverting process. They empirically apply their strategy to the energy futures market. Bogomolov (2013) develops an innovative nonparametric approach for pairs trading based on renko and kagi models. Chen et al. (2014) construct a pairs trading strategy with a three-regime threshold autoregressive model with GARCH efects. Building upon this complex structure they aim for capturing more stylized facts of financial market data. 

## 5. Stochastic control approach

This section provides a comprehensive treatment of the stochastic control approach. A concise overview with relevant studies, their data samples and objectives is provided in table 5. 

## 5.1 Modeling asset pricing dynamics with the Ornstein-Uhlenbeck process

Jurek and Yang (2007) provide the paper with the highest impact in this domain. In their setup, they allow non-myopic arbitrageurs to allocate their capital to a mean-reverting spread or to a riskfree asset. The former evolves according to an Ornstein-Uhlenbeck process and the latter is compounded continuously with the riskfree rate. Two scenarios for investor preferences are considered over a finite time horizon: constant relative risk aversion and the recursive Epstein-Zin utility function. Utilizing the asset price dynamics, Jurek and Yang develop the budget constraints and the wealth dynamics of the arbitrageurs’ assets. Applying stochastic control theory, the authors are able to derive the Hamilton-Jacobi-Bellmann (HJB) equation and subsequently find closed-form solutions for the value and policy functions for both scenarios. Their analytic solutions allow for the following contributions to the literature: First, the OU-process captures the uncertainties of an arbitrage opportunity in the form of horizon and divergence risk. This is a novelty compared to existing models in this domain, such as the Brownian Bridge. Second, the incorporation of diferent utility functions as opposed to log utility makes it possible to split the optimal policy function in two demand components: Myopic demand is a short-term component and exclusively oriented on the current magnitude of the mispricing. Conversely, intertemporal hedging demand addresses the investor’s need for a hedge against the risk stemming from the state variables. Jurek and Yang show that intertemporal hedging demand can explain a significant part of the allocation to the arbitrage opportunity. Third, arbitrageurs do not always perform arbitrage. In line with the numerical findings of Xiong (2001), Jurek and Yang analytically identify the boundaries of a ”stabilization region”, in which the arbitrageur trades against divergences of the spread. Outside of this region, he decreases his positions to avoid negative wealth efects. The authors apply their optimal investment policy in a simulation study and to a pair of stocks. In comparison to the simple threshold rule of GGR, the optimal strategy shows significant outperformance in terms of absolute returns and Sharpe ratios in case of highly mean-reverting spreads. The efect is less pronounced in case of slow mean-reversion and when estimation errors are assumed. Also, no market frictions are considered. In reality, Jurek and Yang’s daily rebalancing would result in substantial transaction costs compared to GGR’s relatively passive trading rule, which produces on average four trades every six months. It would thus be interesting to see how this strategy fares against GGR’s simple approach on a larger empirical data set and under full consideration of transaction costs. 

<table><tr><td>Study</td><td>Date</td><td>Sample</td><td>Objective</td></tr><tr><td>JY</td><td>2007</td><td>Selected stocks 1962-2006</td><td rowspan="4">OU-process: Derivation of the optimal strategy for a risky asset following an OU-process under various utilities</td></tr><tr><td>BB</td><td>2004</td><td>-</td></tr><tr><td>MPW</td><td>2008</td><td>-</td></tr><tr><td>KPB</td><td>2008</td><td>Selected stocks 2002-2008</td></tr><tr><td>ELT</td><td>2011</td><td>-</td><td rowspan="5">Optimal stopping theory: Derivation of the optimal closing of a pairs trade under different conditions (OU process; Lévy processes with jumps; opportunity costs, etc.)</td></tr><tr><td>LLW</td><td>2013</td><td>-</td></tr><tr><td>SZ</td><td>2013</td><td>Selected stocks 1992-2012</td></tr><tr><td>L</td><td>2014</td><td>-</td></tr><tr><td>KLNPTZ</td><td>2015</td><td>Selected stocks 2001-2012</td></tr><tr><td>LT</td><td>2013</td><td>Selected stocks 2006-2012</td><td rowspan="4">Cointegration: Derivation of the optimal strategy for two cointegrated risky assets under various utilities</td></tr><tr><td>TR</td><td>2013</td><td>Selected stocks 2011-2011</td></tr><tr><td>CW</td><td>2015</td><td>-</td></tr><tr><td>LX</td><td>2015</td><td>Selected stocks</td></tr></table>


Table 5: Stochastic control approach


Jurek and Yang provide the most comprehensive discussion of the stochastic control approach applied to an Ornstein-Uhlenbeck framework. Other relevant papers in this domain are as follows: Boguslavsky and Boguslavskaya (2004) develop the optimal investment strategy for a single risky asset following an OU-process for an arbitrageur under power utility. Mudchanatongsuk et al. (2008) also solve the stochastic control problem for pairs trading under power utility for terminal wealth. Their ansatz mostly difers in the assumed asset pricing dynamics, but the spread also relies on an OU-process. Kim et al. (2008) extend the stochastic control problem to multiple spreads and provide tractable solutions. The works of Ekstr¨om et al. (2011), Larsson et al. (2013), Song and Zhang (2013), Lindberg (2014) and Kuo et al. (2015) focus on how to optimally liquidate a pairs trade when incorporating stop-loss thresholds. 

## 5.2 Modeling asset pricing dynamics with error correction models

Liu and Timmermann (2013) build on the results of Jurek and Yang (2007). They also derive the optimal portfolio holdings for convergence trades under recurring and nonrecurring arbitrage opportunities for an investor with power utility over terminal wealth. Contrary to the existing literature, the authors use a cointegration framework for the asset price dynamics and they allow for non-delta-neutral investment positions in the two legs of a pairs trade. In their model, the market index $P _ { m t }$ evolves according to the following geometric random walk: 

$$
\frac {\mathrm{d} P _ {m t}}{P _ {m t}} = (r + \mu_ {m}) \mathrm{d} t + \sigma_ {m} \mathrm{d} B _ {t},\tag{26}
$$

with constant market risk premium $\mu _ { m }$ , constant market volatility $\sigma _ { m } ,$ , the riskfree asset $r$ and $B _ { t }$ as standard Brownian motion. Moreover, there exist two risky assets $P _ { 1 t }$ and $P _ { 2 t }$ with the following 

price dynamics: 

$$
\frac {\mathrm{d} P _ {1 t}}{P _ {1 t}} = (r + \beta \mu_ {m}) \mathrm{d} t + \beta \sigma_ {m} \mathrm{d} B _ {t} + \sigma \mathrm{d} Z _ {t} + b \mathrm{d} Z _ {1 t} - \lambda_ {1} x _ {t} \mathrm{d} t\tag{27}
$$

$$
\frac {\mathrm{d} P _ {2 t}}{P _ {2 t}} = (r + \beta \mu_ {m}) \mathrm{d} t + \beta \sigma_ {m} \mathrm{d} B _ {t} + \sigma \mathrm{d} Z _ {t} + b \mathrm{d} Z _ {2 t} + \lambda_ {2} x _ {t} \mathrm{d} t\tag{28}
$$

$$
x _ {t} = \ln (P _ {1 t}) - \ln (P _ {2 t})\tag{29}
$$

Thereby, $\lambda _ { i } , \beta , b ,$ and $\sigma$ are constants, and $Z _ { t } , \ Z _ { i t }$ are mutually independent standard Brownian motions for $i = 1 , 2$ , and $x _ { t }$ is the error term. Further, the sum of $\lambda _ { 1 }$ and $\lambda _ { 2 }$ is assumed to be greater zero, so that $x _ { t }$ is stationary and the log prices are cointegrated. The investor now has the choice of allocating his funds to the risky assets and to the market portfolio with shares $\phi _ { m } , \ \phi _ { 1 }$ and $\phi _ { 2 }$ , respectively. The authors follow Jurek and Yang and derive the HJB equation for an investor under power utility over terminal wealth. They find the value and optimal policy functions for this stochastic control problem, providing the optimal portfolio weights. By examining the arbitrage opportunity in this portfolio maximization context, the strategy not only incorporates the arbitrage opportunity, but also diversification benefits. This research design results in two new insights relevant for pairs trading: First, it can be optimal to hold both risky assets long (or short) at the same time, even if prices eventually converge. Second, it can also be optimal to only hold one of the two assets. This optimal investment policy is blatantly contrasting with standard deltaneutral long/short pairs trades, such as in GGR. Also, Jurek and Yang’s more enhanced work did not allow for non delta-neutral positionings. Liu and Timmermann empirically compare the optimal unconstrained with the delta neutral strategy on a set of Chinese banking stocks. Their findings are in line with their theories - the unconstrained strategy can result in economically significant gains over the standard arbitrage strategy. Regarding the optimal investment policy in a convergence trade, Liu and Timmermann thus currently provide the most advanced piece of research. A large-scale empirical application would be highly interesting. Since their model relies on daily rebalancing and thus produces high transaction costs, a comparison with a less active trading rule, such as in GGR’s paper, would provide new and relevant insights on how this model fares in light of actual market frictions. As a matter of fact, Lei and Xu (2015) expand on the methodology of Liu et al. and include transaction costs, thereby significantly afecting the optimal policy of the arbitrageur. Tourin and Yan (2013) and Chiu and Wong (2015) also develop optimal strategies for cointegrated risky assets. 

## 6. Other approaches

This section covers further pairs trading approaches. A concise overview with relevant studies, their data samples and objectives is provided in table 6. 

<table><tr><td>Study</td><td>Date</td><td>Sample</td><td>Objective</td></tr><tr><td>H</td><td>2010</td><td>U.S. S&amp;P 100 1992-2006</td><td>Multivariate pairs trading based on Elman</td></tr><tr><td>H</td><td>2009</td><td>U.S. S&amp;P 100 1993-2006</td><td>artificial neural networks and ELECTRE III</td></tr><tr><td>DLE</td><td>2006a</td><td>Crack spread 1995-2005</td><td>Pairs trading frameworks based on different</td></tr><tr><td>DLE</td><td>2008</td><td>Energy future spreads 1995-2005</td><td>machine learning techniques (artificial neural</td></tr><tr><td>TK</td><td>2006</td><td>Selected stocks 2005-2005</td><td>networks, higher order neural networks, re-</td></tr><tr><td>LC</td><td>2008</td><td>Australia ASX selection 2000-2002</td><td>current neural networks, genetic algorithms,</td></tr><tr><td>HHCCCL</td><td>2015</td><td>Selected stocks 2003-2012</td><td>support vector regression, etc.)</td></tr><tr><td>DLMK</td><td>2015</td><td>Corn/eth. crush spread 2005-2010</td><td></td></tr><tr><td>MP</td><td>2009</td><td>U.S. S&amp;P 500 EFT 2000-2007</td><td></td></tr><tr><td>LW</td><td>2013</td><td>Selected stocks 2009-2012</td><td>Copula based pairs trading frameworks</td></tr><tr><td>F</td><td>2008</td><td>Selected stocks 2007-2008</td><td></td></tr><tr><td>SMB</td><td>2013</td><td>Selected stocks, SSFs 2007-2009</td><td></td></tr><tr><td>AL</td><td>2010</td><td>U.S. subset 1997-2007</td><td>Multivariate pairs trading frameworks based</td></tr><tr><td>MTT</td><td>2009</td><td>U.S. S&amp;P 500 1997-2005</td><td>on PCA</td></tr></table>


Table 6: Other approaches


## 6.1 Machine learning and combined forecasts approach

Huck is the main author who has developed and published on this pairs trading methodology in Huck (2009) and Huck (2010), respectively. His framework is based on three steps: Forecasting, outranking and trading. In the forecasting step, a universe of n stocks is considered, so that $n \left( n - 1 \right) / 2$ combinations of pairs can be constructed. Huck uses Elman neural networks to generate one week ahead return forecasts $\hat { x } _ { | X _ { i , t } , X _ { j , t } } ^ { i , t + 1 }$ for each security i, conditional to the past returns of securities i and j, with $i , j \in [ 1 , . . . , n ]$ . Thus, in total, n − 1 return forecasts are generated per period for each security i. In the outranking step, Huck uses a Multi-Criteria Decision Method (MCDM) called ELECTRE III. This method ranks a set of alternatives according to a set of criteria. In this particular case, the n stocks represent the alternatives as well as the criteria. The performance $x _ { i j }$ of each stock i relative to criterion j can be calculated as follows: 

$$
x _ {i j} = \hat {x} _ {| X _ {i, t}, X _ {j, t}} ^ {i, t + 1} - \hat {x} _ {| X _ {i, t}, X _ {j, t}} ^ {j, t + 1}\tag{30}
$$

Thus, the performance is the anticipated spread, i.e., the diference in return forecasts of securities i and $j ,$ conditional to their past information. These performance values are collected in an antisymmetric $n \times n$ matrix. The rows correspond to the n alternatives and the columns to the n criteria. In each cell, we find the anticipated spread of stock i versus criterion $j .$ All criteria are equal-weighted. Next, Huck defines preference, indiference and veto thresholds to determine how performance diferences should be reflected in the ranking process. With ELECTRE III, an outranking of the pairs is created, so that undervalued stocks are at the top of the ranking and overvalued stocks at the bottom. Details about the methodology can be found in Huck’s work and the references therein. In the trading step, the top m stocks of the ranking are bought and the bottom m stocks are sold short. After a trading period of one week, the positions are closed, a new ranking is created and the process repeated. It is important to notice that Hucks’ pairs do not share any kind of equilibrium model. Instead, trading actions are simply triggered based on the position in the final ranking. An empirical application on the S&P 100 constituents from 1992 to 2006 produces impressive results: Buying the top 5 stocks and selling short the bottom 5 stocks of the ranking leads to a 54 percent forecasting accuracy and more than 0.8 percent weekly excess returns. However, these findings should be handled with care. First, Huck did not eliminate the survivorship bias from his database. Only stocks with initial quotations as of 1992 or later were excluded from his analysis. Conversely, an unbiased trading system should only consider those stocks for trading that were actually included in the S&P 100 prior to the trading week. Second, the value-add of the relatively complex MCDM needs further investigation. Normally, the key advantages of ELECTRE III are its fuzzy logic to account for uncertainties in the data and its ability to outrank alternatives across criteria denoted in diferent units. In the present application, all performance values are return diferences of the same dimension. A small increase in anticipated spread relative to one criteria is clearly better from an economic perspective. Thus, a rational investor would buy the stocks with the highest anticipated spreads and go short stocks with the lowest anticipated spreads. Hence, the ELECTRE III trading results should be compared to a simpler ranking algorithm to actually prove its superiority. Nevertheless, this equilibrium free approach constitutes a promising direction of further research, since it defines a completely new direction for pairs trading. 

There are further authors who apply machine learning techniques to pairs trading. The following is just a selection of relevant articles - most of them in an experimental setup and with limited applications to only a few selected securities: Dunis et al. (2006a) model the gasoline crack spread with artificial neural networks. Dunis et al. (2006b) apply recurrent and higher order networks to the soybean-oil crush spread and Dunis et al. (2008) to a portfolio of oil futures spreads. Thomaidis et al. (2006) propose an experimental statistical arbitrage system based on neural network GARCH models. Lin and Cao (2008) and Huang et al. (2015) use genetic algorithms for pairs mining and Dunis et al. (2015) develop pairs trading strategies for the corn/ethanol crush spread with diferent neural network types and genetic algorithms. Finally, Montana and Parrella (2009) use an ensemble of support vector regressions to develop a pairs trading strategy for the iShares S&P 500 ETF. 

## 6.2 Copula approach

The copula approach is extensively discussed in Ferreira (2008), Liew and Wu (2013) and Stander et al. (2013). In a formation period, pairs are built based on previously discussed correlation or cointegration criteria. Next, the log returns $r _ { i t }$ and $r _ { j t }$ are calculated for the two components i and $j$ of a pair. Then, the marginal distribution functions $F _ { i }$ and $F _ { j }$ for the return time series are estimated. Stander et al. (2013) discusses parametric and nonparametric approaches to obtain the marginal distributions, Ferreira (2008) and Liew and Wu (2013) opt for fitting parametric distribution functions. Applying probability integral transform by plugging the returns $r _ { i t }$ and $r _ { j t }$ into their own distribution functions creates two uniform variables $U = F _ { i } \left( r _ { i t } \right)$ and $V = F _ { j } \left( r _ { j t } \right)$ Now, we can identify an adequate copula function. Ferreira just uses one particular copula, whose parameters are estimated with a Canonical Maximum Likelihood method. Stander et al. rely on a set of 22 diferent Archimedean copulas and determine the best-fitting one with the Kolmogorov-Smirnov goodness-of-fit test. Liew and Wu start with five copulas most commonly used in financial applications and determine the best-fitting one by evaluating diferent information critera. The trading strategy is similar for all three papers and is described following Stander et al. and Liew and Wu. They take advantage of the best-fitted copula to calculate the conditional marginal distribution functions as first partial derivatives of the copula function $C ( u , v )$ 

$$
P (U \leq u | V = v) = \frac {\partial C (u , v)}{\partial v}; \quad P (V \leq v | U = u) = \frac {\partial C (u , v)}{\partial u}\tag{31}
$$

If the conditional probability is greater (less) than 0.5, a stock can be considered relatively overvalued (undervalued). The authors suggest to trade when the conditional probabilities are well in the tail regions of their conditional distribution functions, i.e. below their 5 percent and above their 95 percent confidence level. To be specific, stock i is bought and stock j is sold short when their transformed returns fall outside both confidence bands derived by $P \left( U \leq u | V = v \right) = 0 . 0 5$ and $P \left( V \leq v | U = u \right) = 0 . 9 5$ . Informally speaking, this corresponds to the extreme regions in the northwest quadrant of a scatter plot of U and V. Conversely, stock j is bought and stock i is sold short, when inverse conditions apply (extreme regions in the southwest quadrant). Stander et al. suggest to exit a trade as soon as it is profitable or after one week. Liew and Wu reverse their positions once the conditional probabilities cross the boundary of 0.5 again. Empirical applications of this strategy are very scarce, because all authors only use a few selected pairs to demonstrate their algorithm. However, the application of copulas to pairs trading research is promising. If the data were to follow a normal distribution, linear methods would fully capture the dependence structure. Stylized facts such as negative skewness and excess kurtosis are regularly observed. Copulas are an adequate way of modeling such complex dependence structures and thus have the potential to identify better trading opportunities. The key issue inherent to this approach is the complete loss of time structure of the data. When calibrating trading opportunities with the copula method, new returns are compared with confidence levels derived from all past returns of the formation period. Future research should thus aim for ways of better incorporating time structure in the copula approach. A first step could be to only consider residual returns after applying a GARCH filter to remove conditional heteroscedasticity from the return time series, see Hu (2006). Beyond that, Patton (2012) provides an excellent overview of copula models for economic time series. Especially the section about time-varying copula models contains many interesting techniques that could potentially enhance the copula approach to pairs trading. 

## 6.3 Principal components analysis approach

Avellaneda and Lee (2010) develop a statistical arbitrage strategy for the U.S. equity market and empirically apply it to stocks exceeding USD 1 billion in market capitalization at the time of trading. In their formation period, they use two alternative approaches to decompose stock returns into their systematic and idiosyncratic components. In the first approach, Avellaneda and Lee regress the returns $R _ { i }$ of each stock i on its corresponding sector ETF: 

$$
R _ {i} = \beta_ {i} F + \epsilon_ {i}\tag{32}
$$

Thereby, F stands for the returns of the corresponding sector ETF, so $\beta _ { i } F$ denotes the systematic component of the portfolio $( \beta _ { i }$ is the factor loading and F the factor return). Conversely, $\epsilon _ { i }$ represents the idiosyncratic component. In the second approach, a multi-factor model with m factors is considered: 

$$
R _ {i} = \sum_ {j = 1} ^ {m} \beta_ {i j} F _ {j} + \epsilon_ {i}\tag{33}
$$

Avellaneda and Lee use Principal Component Analysis to create m eigenportfolios in line with this statistical factor model. Next, they develop a relative-value model for equity valuation. Based on the multi-factor model above, it is assumed that stock returns satisfy the following diferential equation: 

$$
\frac {\mathrm{d} P _ {i t}}{P _ {i t}} = \mu_ {i} \mathrm{d} t + \sum_ {j = 1} ^ {m} \beta_ {i j} \frac {\mathrm{d} I _ {j t}}{I _ {j t}} + \mathrm{d} X _ {i t}\tag{34}
$$

Thereby, $\mu _ { i }$ represents stock price drift and the residual $X _ { i t }$ is assumed to follow an OU-process. These two components correspond to the idiosyncratic returns of stock i. The remaining summand represents the systematic returns, stemming from the corresponding sector ETF $( m = 1 )$ or from the statistical factor model $( m > 1 )$ . In the trading period, Avellaneda and Lee further consider the idiosyncratic returns of equation (34) and apply a trading model similar to Elliott et al. (2005), as discussed in section 4. The results are impressive with annualized Sharpe ratios of 1.44 from 1997 to 2007 for the PCA based strategies and 1.1 for the ETF based strategies. Going forward, the following improvements could be considered: First, the results are not robust to data mining, especially since Avellaneda and Lee experiment with diferent entry and exit thresholds for trading. 

An approach as in Cummins and Bucca (2012) is suggested. Second, as the authors point out, ”there are considerably more entries in the correlation matrix than data points” when performing PCA (Avellaneda and Lee, 2010, p. 764). Considering asymptotic PCA instead as suggested in Tsay (2010) could be an adequate solution. Third, it may be beneficial to use a cointegration framework instead of PCA. PCA delivers a limited set of series which can be used to approximate a much larger one, i.e., a small number of eigenportfolios is used to represent the systematic risk of the entire stock universe. Conversely, ”cointegration gives all possible stationary linear combinations of a set of random walks” (Alexander, 2001, p. 353). Since Avellaneda and Lee are aiming for stationary residuals, a cointegration framework is considered more appropriate. 

Montana et al. (2009) develop an adjacent approach for the S&P 500, relying on dimensionality reduction via PCA and flexible least squares. 

## 7. Conclusion

We have comprehensively reviewed literature closely related to the umbrella term of pairs trading, covering both univariate and multivariate strategies. Clustered by pairs trading approach, we can summarize our findings and suggestions for further research as follows. 

## 7.1 Distance approach

The distance approach relies on a simple algorithm that is easy to implement and robust to data snooping in its original implementation. The SSD has several deficiencies, leading to low variance spreads with limited profit potential and substantial divergence risk, caused by the lack of cointegration testing. Pearson correlation on return levels performs slightly better. Quasi-multivariate pairs trading leverages information from a whole portfolio of matching partners in one synthetic asset and generally outperforms the univariate version. Pairs trading profitability has low exposure to systematic factors of risk, declines over time and can partially be explained by information diffusion and market frictions, such as liquidity factors. There are applications to other asset classes (bonds, commodities) or time frames (daily data, high frequency data) and GGR’s initial findings are usually confirmed. 

Further research could aim at improving the selection metric to avoid the creation of minimum variance spreads without getting the benefit of increased mean-reversion strength. Especially a combination with the cointegration approach is promising: Ultimately, additional cointegration testing should lead to more stable pairs by filtering out spurious relationships. The chase for the common factor explaining pairs trading profitability could be implemented in a truly global setting, for example, along the lines of Asness et al. (2013) across multiple international markets and asset classes. The presented research leads to the conjecture that pairs trading return premia might be consistent across diverse markets with a strong common factor structure - just as it is the case for value-momentum trading (Asness et al., 2013). 

## 7.2 Cointegration approach

The frameworks presented in the cointegration approach are more diverse than in the distance approach, which mostly difered in terms of empirical implementation. We can summarize as follows: Cointegration constitutes a more rigorous framework for pairs trading compared to the distance approach due to the econometrically sound identification of equilibrium relationships. Vidyamurthy (2004) is the most cited author in this domain. He has proposed a set of heuristics instead of cointegration testing that have not yet been empirically applied. This would be an interesting area for further research. Lin et al. (2006) and Puspaningrum et al. (2010) develop improved trading rules specifically designed for cointegrated securities. Their concepts have the potential to improve trading results and yet need to be tested on a large data set. Existing empirical applications of the univariate frameworks are frequently limited to smaller groups of securities. In most cases, the specifics of multiple comparison problems are not considered, i.e., the cumulation of type I errors through repeated testing on the same data set and the resulting high number of false positives. A combination of Vidyamurthy’s preselection heuristics with adequate statistical procedures to control the familywise error rate as suggested in Cummins and Bucca (2012) would allow for large-scale empirical applications. The multivariate enhanced indexation strategies are highly susceptible for identifying spurious relationships. More appealing are the multivariate statistical arbitrage strategies. The approach of Galenko et al. (2012) leads to positive profits in expectation. A more diligent empirical application of their concept on a larger stock universe would most likely provide relevant new insights. 

## 7.3 Times series approach

Elliott et al. (2005) have introduced state space models and appropriate estimation algorithms to parametrically deal with mean-reverting spreads in pairs trading applications. Several authors have capitalized on their findings to further improve the methodology. Avellaneda and Lee (2010) successfully apply a variant of Eliott et al.’s approach to mean-reverting portfolios constructed from large sets of U.S. equities. This application clearly indicates that dynamic trading rules based on time series analysis can successfully be applied. Yet, this paper remains the only larger empirical application so far. Bertram (2010) presents an optimal statistical arbitrage trading rule for meanreverting portfolios. Initial empirical applications by Cummins and Bucca (2012) to the energy futures markets are highly promising. Also in this case, the strategy has not yet been deployed to other samples. Future research should especially bridge the gap between the distance/cointegration approach and the time series approach. The former focus on the identification of pairs and only apply simple trading rules, mostly on a standard deviation logic in the sense of GGR. The latter do not address the issue of actually finding matching pairs, but instead they develop complex trading systems aiming for improved profitability. Hence, combining strong pair selection algorithms with suitable trading strategies from the time series approach may lead to powerful empirical results. 

## 7.4 Stochastic control approach

The stochastic control approach is mainly focused on finding the optimal investment in the two legs of a pair when other assets are available. The model of Jurek and Yang (2007) shows clear improvement versus a standard threshold rule as in GGR. However, using a cointegration framework and allowing for flexible investment positions, Liu and Timmermann (2013) show that standard delta-neutral strategies may also be suboptimal relative to their unconstrained investment policy. The key direction for future research should be empirical implementation. A large-scale comparison of the these two strategies compared to GGR’s algorithm would show how these conceptual developments fare when facing actual market frictions and model mis-specifications. In the most extreme case, a three-staged combination is possible: Pairs can be selected with the cointegration approach, trading signals determined with an adequate time series approach and position sizing controlled with Jurek and Yang’s or Liu and Timmermann’s method. 

## 7.5 Other approaches

In this section, we have discussed other approaches to pairs trading. Huck (2009, 2010) have introduced a combined approach, building on artificial neural networks and multi-criteria decision methods. The results are impressive, but it is unclear if this is due to the combined forecasts or the MCDM. Especially the value-add of the latter is doubtful, since a rational investor would simply invest in the securities with the most favorable forecasts. Cutting the complexity and replacing the MCDM with a more transparent outranking system may even show improvements. Alternatively, a rigorous approach of ensemble learning as discussed in Mendes-Moreira et al. (2012) could be applied to better manage the bias-variance trade-of. Concretely, Huck does not perform ensemble pruning (i.e., no models are discarded) and it is unclear if ELECTRE III is the optimal mechanism for ensemble integration. In any case, despite the computational complexity, such studies should be conducted on a larger database to further improve the reliability of the results. Ferreira (2008), Stander et al. (2013) and Liew and Wu (2013) have successfully applied copulas in a pairs trading context. An open issue is the lack of empirical applications and the adequate treatment of time structure in financial data. Time dependence in marginal distributions could be accounted for with GARCH filters, time variance of the dependence structure by applying time-varying copula models. Avellaneda and Lee (2010) use PCA to create seemingly mean-reverting time-series, which they model as OU-processes similar to Elliott et al. (2005). Their empirical application is stateof-the-art, except for a rigorous control mechanism with respect to data mining. Methodological improvements should be focused on replacing standard PCA with more advanced methods, such as asymptotic PCA or a multivariate cointegration model. 

## References



Alexander, C. (1999). Optimal hedging using cointegration. Philosophical Transactions: Mathematical, Physical and Engineering Sciences, 357(1758):2039–2058. 





Alexander, C. (2001). Market models: A guide to financial data analysis. Wiley, Chichester, UK and New York, NY. 





Alexander, C. and Dimitriu, A. (2005). Indexing and statistical arbitrage. The Journal of Portfolio Management, 31(2):50–63. 





Andrade, S., Di Pietro, V., and Seasholes, M. (2005). Understanding the profitability of pairs trading. Working paper, UC Berkeley, Northwestern University. 





Asness, C. S., Moskowitz, T. J., and Pedersen, L. H. (2013). Value and momentum everywhere. Journal of Finance, 68(3):929–985. 





Avellaneda, M. and Lee, J.-H. (2010). Statistical arbitrage in the US equities market. Quantitative Finance, 10(7):761–782. 





Baronyan, S. R., Boduro˘glu, <sup>˙</sup>I. <sup>˙</sup>I., and S¸ener, E. (2010). Investigation of stochastic pairs trading strategies under diferent volatility regimes. The Manchester School, 78(s1):114–134. 





Bertram, W. K. (2010). Analytic solutions for optimal statistical arbitrage trading. Physica A: Statistical Mechanics and its Applications, 389(11):2234–2243. 





Bianchi, R., Drew, M., and Zhu, R. (2009). Pairs trading profits in commodity futures markets. In Proceedings of Asian Finance Association 2009 International Conference, pages 1–26. 





Bock, M. and Mestel, R. (2009). A regime-switching relative value arbitrage rule. In Operations Research Proceedings 2008, pages 9–14. Springer. 





Bogomolov, T. (2011). Pairs trading in the land down under. In Finance and Corporate Governance Conference. 





Bogomolov, T. (2013). Pairs trading based on statistical variability of the spread process. Quantitative Finance, 13(9):1411–1430. 





Boguslavsky, M. and Boguslavskaya, E. (2004). Arbitrage under power. Risk, 17(6):69–73. 





Bossaerts, P. (1988). Common nonstationary components of asset prices. Journal of Economic Dynamics and Control, 12(2-3):347–364. 





Bowen, D., Hutchinson, M. C., and O’Sullivan, N. (2010). High frequency equity pairs trading: transaction costs, speed of execution and patterns in returns. The Journal of Trading, 5(3):31–38. 





Bowen, D. A. and Hutchinson, M. C. (2014). Pairs trading in the UK equity market: Risk and return. The European Journal of Finance, 0(0):1–25. 





Broumandi, S. and Reuber, T. (2012). Statistical arbitrage and FX exposure with South American ADRs listed on the NYSE. Financial Assets and Investing, 3(2):5–18. 





Broussard, J. P. and Vaihekoski, M. (2012). Profitability of pairs trading strategy in an illiquid market with multiple share classes. Journal of International Financial Markets, Institutions and Money, 22(5):1188–1201. 





Burgess, A. N. (1999). A computational methodology for modelling the dynamics of statistical arbitrage. PhD thesis, University of London, London Business School. 





Burgess, A. N. (2003). Using cointegration to hedge and trade international equities. In Dunis, C. L., Laws, J., and Na¨ım, P., editors, Applied Quantitative Methods for Trading and Investment, pages 41–69. John Wiley & Sons, Ltd, Chichester, UK. 





Caldeira, J. F. and Moura, G. V. (2013). Selection of a portfolio of pairs based on cointegration: A statistical arbitrage strategy. Brazilian Review of Finance, 11(1):49–80. 





Chen, C. W. S., Chen, M., and Chen, S.-Y. (2014). Pairs trading via three-regime threshold autoregressive GARCH models. In Modeling Dependence in Econometrics, pages 127–140. Springer. 





Chen, H., Chen, S. J., and Li, F. (2012). Empirical investigation of an equity pairs trading strategy. SSRN Electronic Journal. 





Cheng, X., Yu, Philip L. H., and Li, W. K. (2011). Basket trading under co-integration with the logistic mixture autoregressive model. Quantitative Finance, 11(9):1407–1419. 





Chiu, M. C. and Wong, H. Y. (2015). Dynamic cointegrated pairs trading: Mean–variance timeconsistent strategies. Journal of Computational and Applied Mathematics, 290:516–534. 





Cohen, L. and Frazzini, A. (2008). Economic links and predictable returns. The Journal of Finance, 63(4):1977–2011. 





Cummins, M. and Bucca, A. (2012). Quantitative spread trading on crude oil and refined products markets. Quantitative Finance, 12(12):1857–1875. 





D’Aspremont, A. (2011). Identifying small mean-reverting portfolios. Quantitative Finance, 11(3):351–364. 





Do, B. and Faf, R. (2010). Does simple pairs trading still work? Financial Analysts Journal, 66(4):83–95. 





Do, B. and Faf, R. (2012). Are pairs trading profits robust to trading costs? Journal of Financial Research, 35(2):261–287. 





Do, B., Faf, R., and Hamza, K. (2006). A new approach to modeling and estimation for pairs trading. In Proceedings of 2006 Financial Management Association European Conference. 





Dunis, C. and Lequeux, P. (2010). Intraday data and hedging eficiency in interest spread trading. The European Journal of Finance, 6(4):332–352. 





Dunis, C. L., Giorgioni, G., Laws, J., and Rudy, J. (2010). Statistical arbitrage and high-frequency data with an application to Eurostoxx 50 equities. Working paper, Liverpool Business School. 





Dunis, C. L. and Ho, R. (2005). Cointegration portfolios of European equities for index tracking and market neutral strategies. Journal of Asset Management, 6(1):33–52. 





Dunis, C. L., Laws, J., and Evans, B. (2006a). Modelling and trading the gasoline crack spread: A non-linear story. Derivatives Use, Trading & Regulation, 12(1/2):126–145. 





Dunis, C. L., Laws, J., and Evans, B. (2006b). Modelling and trading the soybean-oil crush spread with recurrent and higher order networks: A comparative analysis. Neural Network World, 16(3):193. 





Dunis, C. L., Laws, J., and Evans, B. (2006c). Trading futures spreads: An application of correlation and threshold filters. Applied Financial Economics, 16(12):903–914. 





Dunis, C. L., Laws, J., and Evans, B. (2008). Trading futures spread portfolios: applications of higher order and recurrent networks. The European Journal of Finance, 14(6):503–521. 





Dunis, C. L., Laws, J., Middleton, P. W., and Karathanasopoulos, A. (2015). Trading and hedging the corn/ethanol crush spread using time-varying leverage and nonlinear models. The European Journal of Finance, 21(4):352–375. 





Ekstr¨om, E., Lindberg, C., and Tysk, J. (2011). Optimal liquidation of a pairs trade. In Advanced mathematical methods for finance, pages 247–255. Springer. 





Elliott, R. J., Van Der Hoek*, John, and Malcolm, W. P. (2005). Pairs trading. Quantitative Finance, 5(3):271–276. 





Emery, G. W. and Liu, Q. W. (2002). An analysis of the relationship between electricity and natural–gas futures prices. Journal of Futures Markets, 22(2):95–122. 





Engelberg, J., Gao, P., and Jagannathan, R. (2009). An anatomy of pairs trading: the role of idiosyncratic news, common information and liquidity. In Third Singapore International Conference on Finance. 





Engle, R. F. and Granger, C. W. J. (1987). Co-Integration and error correction: Representation, estimation, and testing. Econometrica, 55(2):251. 





Ferreira, L. (2008). New tools for spread trading. Futures: News, Analysis & Strategies for Futures, Options & Derivatives Traders, 37(12):38–41. 





Galenko, A., Popova, E., and Popova, I. (2012). Trading in the presence of cointegration. The Journal of Alternative Investments, 15(1):85–97. 





Gatarek, L. T., Hoogerheide, L. F., and van Dijk, H. K. (2014). Return and risk of pairs trading using a simulation-based Bayesian procedure for predicting stable ratios of stock prices. SSRN Electronic Journal. 





Gatarek, L. T., Hoogerheide, L. F., van Dijk, H. K., and Verbeek, M. (2011). A simulation-based Bayes’ procedure for robust prediction of pairs trading strategies. Tinbergen Institute Discussion Papers, pages 09–061. 





Gatev, E., Goetzmann, W. N., and Rouwenhorst, K. G. (1999). Pairs trading: Performance of a relative value arbitrage rule. Working paper, Yale School of Management’s International Center for Finance. 





Gatev, E., Goetzmann, W. N., and Rouwenhorst, K. G. (2006). Pairs trading: Performance of a relative-value arbitrage rule. Review of Financial Studies, 19(3):797–827. 





Girma, P. B. and Paulson, A. S. (1999). Risk arbitrage opportunities in petroleum futures spreads. Journal of Futures Markets, 19(8):931–955. 





Gutierrez, J. A. and Tse, Y. (2011). Illuminating the profitability of pairs trading: A test of the relative pricing eficiency of markets for water utility stocks. The Journal of Trading, 6(2):50–64. 





Hong, G. and Susmel, R. (2003). Pairs-trading in the Asian ADR market. Working paper, University of Houston. 





Hu, L. (2006). Dependence patterns across financial markets: A mixed copula approach. Applied Financial Economics, 16(10):717–729. 





Huang, C.-F., Hsu, C.-J., Chen, C.-C., Chang, B. R., and Li, C.-A. (2015). An intelligent model for pairs trading using genetic algorithms. Computational Intelligence and Neuroscience, 501:939606. 





Huck, N. (2009). Pairs selection and outranking: An application to the S&P 100 index. European Journal of Operational Research, 196(2):819–825. 





Huck, N. (2010). Pairs trading and outranking: The multi-step-ahead forecasting case. European Journal of Operational Research, 207(3):1702–1716. 





Huck, N. (2013). The high sensitivity of pairs trading returns. Applied Economics Letters, 20(14):1301–1304. 





Huck, N. (2015). Pairs trading: does volatility timing matter? Applied Economics, pages 1–18. 





Huck, N. and Afawubo, K. (2015). Pairs trading and selection methods: is cointegration superior? Applied Economics, 47(6):599–613. 





Jacobs, H. (2015). What explains the dynamics of 100 anomalies? Journal of Banking & Finance, 57:65–85. 





Jacobs, H. and Weber, M. (2013). Losing sight of the trees for the forest? Attention shifts and pairs trading. SSRN Electronic Journal. 





Jacobs, H. and Weber, M. (2015). On the determinants of pairs trading profitability. Journal of Financial Markets, 23:75–97. 





Jegadeesh, N. (1990). Evidence of predictable behavior of security returns. The Journal of Finance, 45(3):881. 





Jegadeesh, N. and Titman, S. (1993). Returns to buying winners and selling losers: Implications for stock market eficiency. The Journal of Finance, 48(1):65–91. 





Jurek, J. W. and Yang, H. (2007). Dynamic portfolio selection in arbitrage. Working paper, Harvard University. 





Kanamura, T., Rachev, S. T., and Fabozzi, F. J. (2010). A profit model for spread trading with an application to energy futures. The Journal of Trading, 5(1):48–62. 





Karakas, O. (2009). Mean reversion between diferent classes of shares in dual-class firms: Evidence and implications. Working paper, London Business School. 





Kim, K. (2011). Performance analysis of pairs trading strategy utilizing high frequency data with an application to KOSPI 100 equities. SSRN Electronic Journal. 





Kim, S.-J., Primbs, J., and Boyd, S. (2008). Dynamic spread trading. Working paper, Stanford University. 





Kuo, K., Luu, P., Nguyen, D., Perkerson, E., Thompson, K., and Zhang, Q. (2015). Pairs trading: An optimal selling rule. Mathematical Control and Related Fields, 5(3):489–499. 





Larsson, S., Lindberg, C., and Warfheimer, M. (2013). Optimal closing of a pair trade with a model containing jumps. Applications of Mathematics, 58(3):249–268. 





Lehmann, B. N. (1990). Fads, martingales, and market eficiency. The Quarterly Journal of Economics, 105(1):1. 





Lei, Y. and Xu, J. (2015). Costly arbitrage through pairs trading. Journal of Economic Dynamics and Control, 56:1–19. 





Li, M. L., Chui, C. M., and Li, C. Q. (2014). Is pairs trading profitable on China AH-share markets? Applied Economics Letters, 21(16):1116–1121. 





Liew, R. Q. and Wu, Y. (2013). Pairs trading: A copula approach. Journal of Derivatives & Hedge Funds, 19(1):12–30. 





Lin, L. and Cao, L. (2008). Mining in-depth patterns in stock market. International journal of intelligent systems technologies and applications, 4(3-4):225–238. 





Lin, Y.-X., McCrae, M., and Gulati, C. (2006). Loss protection in pairs trading through minimum profit bounds: A cointegration approach. Journal of Applied Mathematics and Decision Sciences, 2006(1):1–14. 





Lindberg, C. (2014). Pairs trading with opportunity cost. Journal of Applied Probability, 51(1):282– 286. 





Liu, J. and Timmermann, A. (2013). Optimal convergence trade strategies. Review of Financial Studies, 26(4):1048–1086. 





Liu, S.-M. and Chou, C.-H. (2003). Parities and Spread Trading in Gold and Silver Markets: A Fractional Cointegration Analysis. Applied Financial Economics, 13(12):899–911. 





Mendes-Moreira, J., Soares, C., Jorge, A. M., and Sousa, Jorge Freire De (2012). Ensemble approaches for regression. ACM Computing Surveys, 45(1):1–40. 





Montana, G. and Parrella, F. (2009). Data mining for algorithmic asset management. In Data Mining for Business Applications, pages 283–295. Springer. 





Montana, G., Triantafyllopoulos, K., and Tsagaris, T. (2009). Flexible least squares for temporal data mining and statistical arbitrage. Expert Systems with Applications, 36(2):2819–2830. 





Mori, M. and Ziobrowski, A. J. (2011). Performance of pairs trading strategy in the U.S. REIT market. Real Estate Economics, 39(3):409–428. 





Mudchanatongsuk, S., Primbs, J. A., and Wong, W. (2008). Optimal pairs trading: A stochastic control approach. In American Control Conference, 2008, pages 1035–1039. 





Nath, P. (2003). High frequency pairs trading with U.S. treasury securities: Risks and rewards for hedge funds. Working paper, London Business School. 





Papadakis, G. and Wysocki, P. (2007). Pairs trading and accounting information. Working paper, Boston University and MIT. 





Patton, A. J. (2012). A review of copula models for economic time series. Journal of Multivariate Analysis, 110:4–18. 





Perlin, M. S. (2007). M of a kind: A multivariate approach at pairs trading. Working paper, ICMA/Reading University. 





Perlin, M. S. (2009). Evaluation of pairs-trading strategy at the Brazilian financial market. Journal of Derivatives & Hedge Funds, 15(2):122–136. 





Peters, G. W., Kannan, B., Lasscock, B., Mellen, C., and Godsill, S. (2011). Bayesian cointegrated vector autoregression models incorporating alpha-stable noise for inter-day price movements via approximate Bayesian computation. Bayesian Analysis, 6(4):755–792. 





Pole, A. (2008). Statistical arbitrage: algorithmic trading insights and techniques. John Wiley & Sons, Hoboken, N.J. 





Politis, D. N. and Romano, J. P. (1994). The Stationary Bootstrap. Journal of the American Statistical Association, 89(428):1303–1313. 





Puspaningrum, H. (2012). Pairs trading using cointegration approach. PhD thesis, University of Wollongong. 





Puspaningrum, H., Lin, Y.-X., and Gulati, C. M. (2010). Finding the optimal pre-set boundaries for pairs trading strategy based on cointegration technique. Journal of Statistical Theory and Practice, 4(3):391–419. 





Rampertshammer, S. (2007). An Ornstein-Uhlenbeck framework for pairs trading. Working paper, University of Melbourne. 





Romano, J. P., Shaikh, A. M., and Wolf, M. (2010). Hypothesis testing in econometrics. Annual Review of Economics, 2(1):75–104. 





Romano, J. P. and Wolf, M. (2007). Control of generalized error rates in multiple testing. The Annals of Statistics, 35(4):1378–1408. 





Ross, S. A. (1976). The arbitrage theory of capital asset pricing. Journal of Economic Theory, 13(3):341–360. 





Shleifer, A. (2000). Ineficient markets: An introduction to behavioral finance. Oxford University Press, Oxford and New York. 





Simon, D. P. (1999). The soybean crush spread: Empirical evidence and trading strategies. Journal of Futures Markets, 19(3):271–289. 





Song, Q. and Zhang, Q. (2013). An optimal pairs-trading rule. Automatica, 49(10):3007–3014. 





Stander, Y., Marais, D., and Botha, I. (2013). Trading strategies with copulas. Journal of Economic and Financial Sciences, 6(1):83–107. 





Stock, J. H. and Watson, M. W. (1988). Testing for common trends. Journal of the American Statistical Association, 83(404):1097. 





Thomaidis, N. S., Kondakis, N., and Dounias, G. D. (2006). An intelligent statistical arbitrage trading system. In Advances in Artificial Intelligence, pages 596–599. Springer. 





Tourin, A. and Yan, R. (2013). Dynamic pairs trading using the stochastic control approach. Journal of Economic Dynamics and Control, 37(10):1972–1981. 





Triantafyllopoulos, K. and Montana, G. (2011). Dynamic modeling of mean-reverting spreads for statistical arbitrage. Computational Management Science, 8(1-2):23–49. 





Tsay, R. S. (2010). Analysis of financial time series. Wiley series in probability and statistics. John Wiley & Sons, Hoboken, N.J., 3rd edition. 





Vidyamurthy, G. (2004). Pairs trading: Quantitative methods and analysis. John Wiley & Sons, Hoboken, N.J. 





Wahab, M. and Cohn, R. (1994). The gold-silver spread: Integration, cointegration, predictability, and ex-ante arbitrage. Journal of Futures Markets, 14(6):709–756. 





Xiong, W. (2001). Convergence trading with wealth efects: an amplification mechanism in financial markets. Journal of Financial Economics, 62(2):247–292. 





Zeng, Z. and Lee, C.-G. (2014). Pairs trading: optimal thresholds and profitability. Quantitative Finance, 14(11):1881–1893. 



## Diskussionspapiere 2015 Discussion Papers 2015

01/2015 Seebauer, Michael: Does Direct Democracy Foster Efficient Policies? An Experimental Investigation of Costly Initiatives 

02/2015 Bünnings, Christian, Schmitz, Hendrik, Tauchmann, Harald and Ziebarth, Nicolas R.: How Health Plan Enrollees Value Prices Relative to Supplemental Benefits and Service Quality 

03/2015 Schnabel, Claus: United, yet apart? A note on persistent labour market differences between western and eastern Germany 

04/2015 Dieckmann, Anja, Fischbacher, Urs, Grimm, Veronika, Unfried, Matthias, Utikal, Verena and Valmasoni, Lorenzo: Trust and Beliefs among Europeans: Cross-Country Evidence on Perceptions and Behavior 

05/2015 Grimm, Veronika, Utikal, Verena and Valmasoni, Lorenzo: In-group favoritism and discrimination among multiple out-groups 

06/2015 Reichert, Arndt R., Tauchmann, Harald and Wübker, Ansgar: Weight Loss and Sexual Activity in Adult Obese Individuals: Establishing a Causal Link 

07/2015 Klein, Ingo, Mangold, Benedikt: Cumulative Paired ϕ-Entropy 

08/2015 Erbe, Katharina: Tax Planning of Married Couples in East and West Germany 

## Diskussionspapiere 2014 Discussion Papers 2014

01/2014 Rybizki, Lydia: Learning cost sensitive binary classification rules accounting for uncertain and unequal misclassification costs 

02/2014 Abbiati, Lorenzo, Antinyan, Armenak and Corazzini, Lucca: Are Taxes Beautiful? A Survey Experiment on Information, Tax Choice and Perceived Adequacy of the Tax Burden 

03/2014 Feicht, Robert, Grimm, Veronika and Seebauer, Michael: An Experimental Study of Corporate Social Responsibility through Charitable Giving in Bertrand Markets 

04/2014 Grimm, Veronika, Martin, Alexander, Weibelzahl, Martin and Zoettl, Gregor: Transmission and Generation Investment in Electricity Markets: The Effects of Market Splitting and Network Fee Regimes 

05/2014 Cygan-Rehm, Kamila and Riphahn, Regina: Teenage Pregnancies and Births in Germany: Patterns and Developments 

06/2014 Martin, Alexander and Weibelzahl, Martin: Where and when to Pray? - Optimal Mass Planning and Efficient Resource Allocation in the Church 

07/2014 Abraham, Martin, Lorek, Kerstin, Richter, Friedemann and Wrede, Matthias: Strictness of Tax Compliance Norms: A Factorial Survey on the Acceptance of Inheritance Tax Evasion in Germany 

08/2014 Hirsch, Boris, Oberfichtner, Michael and Schnabel Claus: The levelling effect of product market competition on gender wage discrimination 

09/1014 Mangold, Benedikt: Plausible Prior Estimation 

10/2014 Gehrke, Britta: Fiscal Rules and Unemployment 

11/2014 Gehrke, Britta and Yao, Fang: Phillips Curve Shocks and Real Exchange Rate Fluctuations: SVAR Evidence 

12/2014 Mäder, Miriam, Müller, Steffen, Riphahn, Regina and Schwientek, Caroline: Intergenerational transmission of unemployment - evidence for German sons 

13/2014 Casal, Sandro, Ploner, Matteo and Sproten, Alec N.: Fostering the Best Execution Regime. An Experiment about Pecuniary Sanctions and Accountability in Fiduciary Money Management 

14/2014 Lochner, Benjamin: Employment protection in dual labor markets - Any amplification of macroeconomic shocks? 

15/2014 Herrmann, Klaus, Teis, Stefan and Yu, Weijun: Components of Intraday Volatility and Their Prediction at Different Sampling Frequencies with Application to DAX and BUND Futures 

## Diskussionspapiere 2013 Discussion Papers 2013

01/2013 Wrede, Matthias: Rational choice of itemized deductions 

02/2013 Wrede, Matthias: Fair Inheritance Taxation in the Presence of Tax Planning 

03/2013 Tinkl, Fabian: Quasi-maximum likelihood estimation in generalized polynomial autoregressive conditional heteroscedasticity models 

04/2013 Cygan-Rehm, Kamila: Do Immigrants Follow Their Home Country’s Fertility Norms? 

05/2013 Ardelean, Vlad and Pleier, Thomas: Outliers & Predicting Time Series: A comparative study 

06/2013 Fackler, Daniel and Schnabel, Claus: Survival of spinoffs and other startups: First evidence for the private sector in Germany, 1976-2008 

07/2013 Schild, Christopher-Johannes: Do Female Mayors Make a Difference? Evidence from Bavaria 

08/2013 Brenzel, Hanna, Gartner, Hermann and Schnabel Claus: Wage posting or wage bargaining? Evidence from the employers’ side 

09/2013 Lechmann, Daniel S. and Schnabel Claus: Absence from work of the selfemployed: A comparison with paid employees 

10/2013 Bünnings, Ch. and Tauchmann, H.: Who Opts Out of the Statutory Health Insurance? A Discrete Time Hazard Model for Germany 

## Diskussionspapiere 2012 Discussion Papers 2012

01/2012 Wrede, Matthias: Wages, Rents, Unemployment, and the Quality of Life 

02/2012 Schild, Christopher-Johannes: Trust and Innovation Activity in European Regions - A Geographic Instrumental Variables Approach 

03/2012 Fischer, Matthias: A skew and leptokurtic distribution with polynomial tails and characterizing functions in closed form 

04/2012 Wrede, Matthias: Heterogeneous Skills and Homogeneous Land: Segmentation and Agglomeration 

05/2012 Ardelean, Vlad: Detecting Outliers in Time Series 

Diskussionspapiere 2011 Discussion Papers 2011 

01/2011 Klein, Ingo, Fischer, Matthias and Pleier, Thomas: Weighted Power Mean Copulas: Theory and Application 

02/2011 Kiss, David: The Impact of Peer Ability and Heterogeneity on Student Achievement: Evidence from a Natural Experiment 

03/2011 Zibrowius, Michael: Convergence or divergence? Immigrant wage assimilation patterns in Germany 

04/2011 Klein, Ingo and Christa, Florian: Families of Copulas closed under the Construction of Generalized Linear Means 

05/2011 Schnitzlein, Daniel: How important is the family? Evidence from sibling correlations in permanent earnings in the US, Germany and Denmark 

06/2011 Schnitzlein, Daniel: How important is cultural background for the level of intergenerational mobility? 

07/2011 Steffen Mueller: Teacher Experience and the Class Size Effect - Experimental Evidence 

08/2011 Klein, Ingo: Van Zwet Ordering for Fechner Asymmetry 

09/2011 Tinkl, Fabian and Reichert Katja: Dynamic copula-based Markov chains at work: Theory, testing and performance in modeling daily stock returns 

10/2011 Hirsch, Boris and Schnabel, Claus: Let’s Take Bargaining Models Seriously: The Decline in Union Power in Germany, 1992 – 2009 

11/2011 Lechmann, Daniel S.J. and Schnabel, Claus : Are the self-employed really jacks-of-all-trades? Testing the assumptions and implications of Lazear’s theory of entrepreneurship with German data 

12/2011 Wrede, Matthias: Unemployment, Commuting, and Search Intensity 

13/2011 Klein, Ingo: Van Zwet Ordering and the Ferreira-Steel Family of Skewed Distributions 

## Diskussionspapiere 2010 Discussion Papers 2010

01/2010 Mosthaf, Alexander, Schnabel, Claus and Stephani, Jens: Low-wage careers: Are there dead-end firms and dead-end jobs? 

02/2010 Schlüter, Stephan and Matt Davison: Pricing an European Gas Storage Facility using a Continuous-Time Spot Price Model with GARCH Diffusion 

03/2010 Fischer, Matthias, Gao, Yang and Herrmann, Klaus: Volatility Models with Innovations from New Maximum Entropy Densities at Work 

04/2010 Schlüter, Stephan and Deuschle, Carola: Using Wavelets for Time Series Forecasting – Does it Pay Off? 

05/2010 Feicht, Robert and Stummer, Wolfgang: Complete closed-form solution to a stochastic growth model and corresponding speed of economic recovery. 

06/2010 Hirsch, Boris and Schnabel, Claus: Women Move Differently: Job Separations and Gender. 

07/2010 Gartner, Hermann, Schank, Thorsten and Schnabel, Claus: Wage cyclicality under different regimes of industrial relations. 

08/2010 Tinkl, Fabian: A note on Hadamard differentiability and differentiability in quadratic mean. 

## Diskussionspapiere 2009 Discussion Papers 2009

01/2009 Addison, John T. and Claus Schnabel: Worker Directors: A German Product that Didn’t Export? 

02/2009 Uhde, André and Ulrich Heimeshoff: Consolidation in banking and financial stability in Europe: Empirical evidence 

03/2009 Gu, Yiquan and Tobias Wenzel: Product Variety, Price Elasticity of Demand and Fixed Cost in Spatial Models 

04/2009 Schlüter, Stephan: A Two-Factor Model for Electricity Prices with Dynamic Volatility 

05/2009 Schlüter, Stephan and Fischer, Matthias: A Tail Quantile Approximation Formula for the Student t and the Symmetric Generalized Hyperbolic Distribution 

06/2009 Ardelean, Vlad: The impacts of outliers on different estimators for GARCH processes: an empirical study 

07/2009 Herrmann, Klaus: Non-Extensitivity versus Informative Moments for Financial Models - A Unifying Framework and Empirical Results 

08/2009 Herr, Annika: Product differentiation and welfare in a mixed duopoly with regulated prices: The case of a public and a private hospital 

09/2009 Dewenter, Ralf, Haucap, Justus and Wenzel, Tobias: Indirect Network Effects with Two Salop Circles: The Example of the Music Industry 

10/2009 Stuehmeier, Torben and Wenzel, Tobias: Getting Beer During Commercials: Adverse Effects of Ad-Avoidance 

11/2009 Klein, Ingo, Köck, Christian and Tinkl, Fabian: Spatial-serial dependency in multivariate GARCH models and dynamic copulas: A simulation study 

12/2009 Schlüter, Stephan: Constructing a Quasilinear Moving Average Using the Scaling Function 

13/2009 Blien, Uwe, Dauth, Wolfgang, Schank, Thorsten and Schnabel, Claus: The institutional context of an “empirical law”: The wage curve under different regimes of collective bargaining 

14/2009 Mosthaf, Alexander, Schank, Thorsten and Schnabel, Claus: Low-wage employment versus unemployment: Which one provides better prospects for women? 

## Diskussionspapiere 2008 Discussion Papers 2008

01/2008 Grimm, Veronika and Gregor Zoettl: Strategic Capacity Choice under Uncertainty: The Impact of Market Structure on Investment and Welfare 

02/2008 Grimm, Veronika and Gregor Zoettl: Production under Uncertainty: A Characterization of Welfare Enhancing and Optimal Price Caps 

03/2008 Engelmann, Dirk and Veronika Grimm: Mechanisms for Efficient Voting with Private Information about Preferences 

04/2008 Schnabel, Claus and Joachim Wagner: The Aging of the Unions in West Germany, 1980-2006 

05/2008 Wenzel, Tobias: On the Incentives to Form Strategic Coalitions in ATM Markets 

06/2008 Herrmann, Klaus: Models for Time-varying Moments Using Maximum Entropy Applied to a Generalized Measure of Volatility 

07/2008 Klein, Ingo and Michael Grottke: On J.M. Keynes' “The Principal Averages and the Laws of Error which Lead to Them” - Refinement and Generalisation 