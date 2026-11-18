

<!-- === Source: MinerU_markdown_Market_microstructure_and_market_liquidity_1_2122706850364366866.md (Page 1) === -->

# Market microstructure and market liquidity

Jun Muranaga and Tokiko Shimizu* 

Bank of Japan 

## Abstract

This paper explores the factors affecting market liquidity using a simulation model of an artificial market. We first survey definition of market liquidity and discuss the relationship between market liquidity and market efficiency or stability. We then consider a continuous auction market and discuss factors affecting market liquidity. Incorporating the discussion, we construct an artificial market model and conduct various simulations. We find that an increase in the ratio of market participants following short-term market price movements results in an increase in the number of trades and at the same time a decrease in the volume of accumulated order flows. When market participants become more risk-averse on average, market liquidity decreases. A precipitous decrease in market liquidity results when market participants lose confidence in their expectations on future prices. Changes in the sensitivities of traders to market information affect market liquidity, but various market liquidity indicators do not necessarily move in the same direction. These results suggest that change in market liquidity indicators may not always be consistent. 

## 1. Introduction

In this paper we review the factors which affect market liquidity and present a framework which measures such effects quantitatively. This framework enables us to clarify the logic behind recent market reforms and the introduction of rules (e.g. the introduction of electronic trading,<sup>1</sup> the development of disclosure of trade information for market participants,<sup>2</sup> and the prevalence of computerised bilateral transactions).<sup>3</sup> Market liquidity has long been implicitly assumed to exist when market participants evaluate the prices of financial products and manage their portfolios and when central banks implement monetary policy. Since the cost of losing market liquidity is large despite its implicit nature, the improvement and stability of market liquidity is not only important for market participants, but also serves as a way to enhance financial market stability. 

This paper is composed of two major parts: a survey of the concepts relating to the factors which affect market liquidity and verification by simulation. In the conceptual summary part, we first summarise the definition of market liquidity and the relationship between market liquidity and market efficiency or stability. Based on the summary, we consider the price discovery mechanism, in which potential trade needs are actually realised in the market as order flows and prices are discovered by matching such orders, and we clarify our direction toward simulation model construction. In the simulation, we assume a certain market structure and focus on the parameters which affect an individual market participant’s ordering decision, such as expectation of the asset price, confidence in such expectation, the extent of risk aversion, sensitivity to various kinds of market information. These parameters determine the realisation process of potential trade needs of market participants according to the market structure. Therefore, through the simulation we observe, as a mechanism in which market structure affects the state of market liquidity, how the above parameters affect market behaviour. Recently, simulation techniques have been widely used in the area of economics, and are useful in analysing an economic mechanism, which is an aggregate of complex individual behaviours. In our analysis, we do not deal with actual markets which trade specific goods such as foreign exchange, stocks, or government bonds, but assume a market in which hypothetical assets or securities are traded. Although some studies have dealt with the foreign exchange market<sup>4</sup> or analyses of government bond markets,<sup>5</sup> many studies have focused mainly on the New York Stock Exchange.<sup>6</sup> In our analysis, instead of recognising the difference between markets by the character of the goods traded, we regard the difference as a difference of market microstructure or trading rules, and try to capture their general effects on market liquidity. 

The composition of this paper is as follows. Section 2 defines market liquidity and Section 3 reviews the concepts relating to the mechanism of determining market liquidity. Section 4 will present a framework for both our model and the simulations, and we conduct the simulation analysis in Section 5. Section 6 concludes by describing some implications and areas for future research. 

## 2. Definition of market liquidity

## 2.1 Definition of market liquidity

Market liquidity has been defined in various ways according to the context in which it has been used. In retrospect, we can see that Keynes (1930) and Hicks (1962) chose “market liquidity” as a subject in economics, but the terminology they used consisted of phrases such as the “future volatility of market prices” or the “possibility of immediate execution of a transaction.” When discussing whether or not a market is liquid, Bagehot (1971) focused on factors such as the existence of adverse selection effects due to information asymmetry, the price impact of a trade, and the portion of trading cost which is set according to the pricing policy of the market maker. When market liquidity is discussed in market microstructure theory, it is often the case that more practical concepts are introduced, such as the “cost of changing positions (tightness),” the “trade size or thickness of the order book-profile (order book refers to a panel which provides traders with bid-ask prices and volume offered per price) required for changing prices (market depth),” and the “required period of time to recover from price fluctuation caused by a sudden shock or to reach a new equilibrium (market resiliency).” In defining the “liquid market” of finance theory, which is a premise for the option equation to hold, Black (1971) noted that this is a market in which a “bid-ask price is always quoted, its spread is small enough, and small trades can be immediately executed with minimal effect on price.” Grossman and Miller (1988) pointed out that we can measure the liquidity of a market by looking “the ability of executing trades under the current price quotes price– and time-wise.” 

We define a liquid market as a market where a large volume of trades can be immediately executed with minimum effect on price. In other words, the liquidity of the market can be recognised by how low the uncertainties of execution price are. In addition, we consider “market depth,” which absorbs the price changes accompanied by trade execution, as an important factor in explaining market liquidity. In determining “market depth,” we need to take into account the size of the trade needs, including potential needs, of a certain asset. 

Market liquidity is an important factor which affects market efficiency. Given that market liquidity is an indicator which represents market depth and shows the absorption power of risk premium on trading execution, the condition of market liquidity can be considered as one of the factors affecting the price discovery function. When we consider market efficiency in the context of a market’s price discovery function and the information content of price,<sup>10</sup> market liquidity can be regarded as a factor which affects market price uncertainties – uncertainties in the sense that market prices do not reveal all available information or in the sense that market price will temporarily diverge from the market-clearing equilibrium price – or price discovery function, and will, as a result, affect market efficiency. We can improve market efficiency by increasing market liquidity. Specifically, a decline of market price uncertainties accompanied by an increase in market liquidity will, through the decline of liquidity premiums such as the bid-ask spread and market impact, improve market efficiency, resulting in efficient fund and risk allocation. If one can clarify the mechanism by which market liquidity affects the price discovery process, it will provide a good reference in considering measures designed to improve market efficiency. 

Market liquidity is an important issue in maintaining financial system stability. The collapse of a system, or the emergence of systemic risk, will be caused by the market coming to a halt or by the loss of market participants’ faith in the market price discovery function. As tautological as it may sound, a halt in the endogenous market price discovery function depends on whether or not market participants who try to avoid the risk of market halt form a majority. Behaviour to avoid the risk of market halt such as the reduction of market exposure by closing positions is considered to materialise when market conditions including price levels and the speed of changes in the price level have exceeded specified limit values, and there will be various processes by which the system collapses. The processes include feedback effects caused by market participants’ responses and the synchronising effect between markets. Such boundary and collapse processes may differ between markets. The characteristics of boundary and collapse processes depend on market participants’ expectations of or confidence in the market itself, which are generated from market behaviour under normal conditions including a small degree of stress. Therefore, the maintenance of sufficient liquidity under normal conditions will autonomously improve market stability by expanding the market boundaries and improving the participants’ confidence in market sustainability. 

## 2.2 Static and dynamic aspects of market liquidity

Traditional measures of market liquidity include trade volume, or the number of trades, although the above definition of market liquidity suggests that any indicator which represents the extent of “uncertainty of trade execution price” would be an appropriate measure of market liquidity. Specifically, such indicators include the bid-ask spread, which is determined by taking into account the premium against price uncertainties, changes in bid-ask price at the moment of trade executions (market impact), and the period of time required to reach a new equilibrium after trade executions (market resiliency). In a market with no bid-ask spread or market impact, and quite a large market resiliency, the trade execution price will be identical to the market price at the time of trading, and there the market participants need not worry about price uncertainties in the execution of trades. Such a market is regarded as quite deep and highly liquid. 

Past studies of market liquidity have mainly focused on static aspects and have adopted indicators which show static market depth, such as turnover, bid-ask spread, as measures of market liquidity.<sup>12</sup> However, in order to examine how market liquidity affects the price discovery function in an actual market, not only should the static aspects of market liquidity be examined, but also the dynamic. In order to effectively capture supply and demand, we should take into account the dynamic measurement of market liquidity. Effective supply and demand refers to each market participant’s needs at a certain time which are not reflected in the observable order book-profile or order flows. The reasons why effective supply and demand do not necessarily surface include the existence of explicit trading costs such as taxes and transaction fees, and the uneven distribution of information among market participants. Implicitly existing effective supply and demand are revealed through the information about the price changes caused by trade execution itself, although there is another mechanism by which a decline in trading costs and the prevalence of information induce new effective supply and demand. 

Just as one cannot judge the depth of a well by throwing a stone into it, but must wait until the sound comes back, the potential depth of the market, i.e. effective supply and demand, is an indicator which can only be recognised dynamically. We need to observe dynamic indicators such as price changes upon execution (market impact),<sup>13</sup> the speed of convergence from one trade price to the next equilibrium price or bid-ask spread (market resiliency).<sup>14</sup> These dynamic indicators reflect the actual results of the executed transaction and the process by which information derived from such results is digested in the market. In discussing market liquidity under stress, it becomes essential to implement analyses which incorporate such dynamic aspects. We outline conceptual ways to measure these dynamic indicators in Appendix. 

In this paper, we focus on the following indicators to explore market liquidity conditions: probability of quote existence, trade frequency, price volatility, bid-ask spread, gross order book volume (buying order volume plus selling order volume), and net order book volume (buying order volume minus selling order volume). We also calculate the volatility of gross order book volume, and this indicator can be regarded as representing the ease with which the order book is restored to its original state after certain decrease in orders, that is, a proxy of market resiliency. The standard deviation of net order book volume represents bias of the market supply-demand. When the value increases, this suggests that large supply-demand bias is more likely to occur. 

## 3. Conceptual summary of the mechanism through which market microstructure affects market liquidity

One of the purposes of this study is to clarify conceptually the process by which actual market microstructure affects market liquidity. The process by which market microstructure affects price discovery in a market and market liquidity via changes in market participants’ behaviours is composed of two stages: (1) from when market participants hold potential trade needs based on their individual reasons to when they actually decide to place orders in the market (the micro stage), and (2) the stage in which such orders are accumulated in the market and trades are executed (the macro stage). In the following, we will summarise the mechanism through which market microstructure affects decision-making at the micro stage and price discovery at the macro stage. 


Figure 1. Price discovery process: Micro stage and macro stage


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/bf1803f6ac887f70d44bb8d84bca6813ec08fba2b4806140674ae3e6daf28ca9.jpg)


## 3.1 Decision-making process of market participants at the micro stage

There are various channels through which traders’ decision-making processes are influenced by the market microstructure.<sup>15</sup> If there is some institution or set of rules, such as an accounting rule and a tax system, which induce certain effects on the decision-making process of entering the market and placing trade orders, the market microstructure will alter effective supply and demand in the market and finally affect market liquidity. 

First of all, we consider the mechanism by which an economic agent decides to participate in a transaction in a specific market. Under certain budget constraints, the economic agent will decide to trade the goods. Such a decision to trade is based on his/her judgement that by executing the trade he/she will maximise his/her net benefit under his/her own budget constraint upon comparison of alternative behaviours.<sup>16</sup> Three factors which affect the decision-making at this point are the budget constraint of the economic agent ( B ), behavioural alternatives ( i ), and the expected returns and costs, including risk premiums $( \widetilde { R } _ { i } / \widetilde { C } _ { i } )$ ). 

$$
\begin{array}{l} \widetilde {R} / \widetilde {C} = \max _ {i = 1, \dots , n} \left(\widetilde {R} _ {i} / \widetilde {C} _ {i}\right) \\ B \geq \widetilde {C} \end{array}
$$

It is worth noting that there are numerous potential trade needs behind the actual trade orders explicitly placed in the market, and that whether such potential need are realised or not is determined not discontinuously but by the continuous cost-benefit function noted above. Therefore, in examining the issue of market liquidity, not only should the orders explicitly placed in the market be considered, but also the underlying trade needs, that is, effective supply and demand. 

Next we will consider how to quantify such costs and benefits. Cost components include: (1) the explicit trading cost $c _ { e }$ , such as brokerage fee and tax, and (2) the implicit trading cost $\tilde { c }$ , which is the difference between optimal trade price and actual execution price (expected price at the moment of decision-making).<sup>17</sup> Other than brokerage fee and tax, explicit trading cost includes all kinds of cost imposed on those who trade in the market. 18 

$$
C = c _ {e} + \widetilde {c}
$$

Implicit trading cost refers to the difference between the optimal trade price $( P _ { o } )$ and the expected value of the execution price $( \widetilde { P } _ { e } )$ . The optimal trading price $P _ { o }$ will be recognised in conjunction with the trade volume $( \nu _ { o } )$ , and in general the execution price $\widetilde { P } _ { e }$ is a function of $\nu _ { e }$ (the expected value of the execution volume). In determining the relationship between $\widetilde { P } _ { e }$ and $\nu _ { e } , ^ { 1 9 }$ the depth of the market should be taken into account and thus the relation will be affected by market liquidity expectations. 

$$
\widetilde {c} = \left| \widetilde {P} _ {e} \widetilde {v} _ {e} - P _ {o} v _ {o} \right|
$$

Among the determinants of implicit trading cost, optimal trade price $P _ { o }$ will be determined by a trader’s expectations concerning future prices and by institutional needs. In forming the expectation, a trader’s individual strategy for trading, for example chartist or fundamentalist, will have an effect, and in the case of informed traders, private information about future price changes will also be incorporated into the process. Institutional needs will reflect factors including preference among assets caused by accounting rules and the effects of investment regulations. 

The expected value of the actual execution price $( \widetilde P _ { e } ) .$ , another factor which determines the implicit trading cost, will be affected substantially, in the short run, by the market structure and trading rules, and, as in the case of the optimal trade price $P _ { o }$ , partially by an individual trader’s expectation of future price changes. For example, when we look at how implicit trading costs are determined in the Tokyo Stock Exchange system, traders will conjecture the $\widetilde { P } _ { e }$ for the two alternatives – market order and limit order – and select the one with lower cost. In the case of market order, $\widetilde { P } _ { e }$ is equal to the current market price $p _ { t }$ (best bid-ask).<sup>20</sup> On the other hand, when we consider $P _ { e }$ in the case of limit order, the ordered price itself $p _ { l }$ as well as the opportunity cost θ for the lag between order and execution should be taken into account. In calculating the opportunity cost, we need to incorporate trader’s expectations concerning future price changes.<sup>21</sup> Expectations of future price changes will also have an effect in calculating the optimal trade price $P _ { o }$ , and if we are to incorporate them into the expected execution price $P e$ , it should be noted that the effects of future changes in supply and demand of the market as a whole will also be incorporated. At this point, the availability of trade information such as order book information will affect individual traders’ decision-making. 

$$
\widetilde {P} _ {e} = b e s t \big (p _ {t}, p _ {l} \pm \theta \big)
$$

best( )⋅ here means that the lower price in case of a buying order and higher price in case of a selling order will be selected. 

With respect to the relationship between the difference in ordering methods and market liquidity, there have been many theoretical studies which showed that the number of limit orders affects the extent of market liquidity, or serves as an indicator of the state of market liquidity.<sup>22</sup> In those studies, limit orders are treated as a component of market supply and demand, and as a source of information for market makers. In addition, it was assumed that by observing limit orders, which are a type of option, one can learn about market participants’ judgements of market liquidity, i.e. trading incentives. 


If we are to summarise the decision-making process of an individual trader, it can be shown as follows:


<table><tr><td>Decision-making mechanism</td><td>Factors affecting the decision-making mechanism</td></tr><tr><td><eq>R/C = \max_{i=1 \to n} (R_i / C_i)</eq></td><td>choosing the market and asset which maximises his/her net benefit from economic activities</td></tr><tr><td><eq>B \geq C</eq></td><td>budget constraints</td></tr><tr><td><eq>C = c_e + \tilde{c}</eq></td><td><eq>c_e</eq>: brokerage fee, tax, settlement rules, and hedging devices, etc.</td></tr><tr><td><eq>\tilde{c} = \left| \tilde{P}_e \tilde{v}_e - P_o v_o \right|</eq></td><td><eq>P_o</eq>: expectations regarding future prices, accounting rules, investment regulations, etc.relation between <eq>\tilde{P}_e</eq> and <eq>\tilde{v}_e</eq>: expectations regarding future market liquidityrelationship between <eq>P_o</eq> and <eq>v_o</eq>: liquidity trader, informed trader, etc.</td></tr><tr><td><eq>\tilde{P}_e = best(p_t, p_l \pm \theta)</eq></td><td><eq>p_l \pm \theta</eq>: limit order, expectations regarding future prices, expectations regarding future demand and supply, etc.</td></tr><tr><td><eq>\tilde{P}_e = p_t</eq></td><td><eq>p_t</eq> market maker&#x27;s risk preference and information about stop-loss orders</td></tr></table>

## 3.2 Price discovery process at the macro stage

At the macro stage, a feedback mechanism will be generated: orders based on the decision-making process at the micro stage are placed in the market, prices are determined by the execution of such orders, and price information is in turn reflected in decision-making at the micro stage. There are some studies which have dealt with the effects of different execution systems – for example, a double auction system in which all orders are competitively matched or a market maker system in which orders are concentrated in and executed at the market maker’s place – on market liquidity.<sup>23</sup> What is important in any of these systems is how liquidity will be supplied to the market. During the process of individual orders being accumulated and market price being discovered, in particular, the different roles execution systems play in collecting and distributing information become quite important. Even in the same system, for example, market liquidity can either increase or decrease depending on the information distribution function of market makers. 

When placing an order according to the execution system structure, the macro structure has already been influenced by the micro decision-making. In addition, the information content incorporated at the point of the market maker’s quote presentation may be summarised as part of the process of forming macro information. What is important at the macro stage, therefore, is the mechanism by which feedback of information about execution results and orders is provided by the execution system as an input to market participant’s decision-making at the micro stage. The determinant of this mechanism is the extent of information sharing in the market, that is, market transparency. In an extreme case, when there are multiple market makers quoting independently in the market, there is no single common price in the market. In addition, even if the market shares the same information about the execution price, it may be the case that other information such as a market maker’s price quote at each point in time is presented only to a fraction of the participants, or, in contrast, all order information is disclosed as order book information. Furthermore, for effective supply and demand which are not explicitly revealed to the market in the form of orders, information may be revealed as stop-loss orders. 

The continuous double auction system and the market maker system are often deemed to be totally different, although the main difference between the two systems stems from the difference in the information collection and distribution mechanisms inherent in them. For example, the disappearance of best bid or ask price in the double auction system, which we often observe in individual stock markets, can be regarded as indicating the inadequacy of the information distribution function of the system in revealing information about current market price. As summarised during the discussion of the micro stage, what affects the decision-making process of an individual market participant is the information about the current state and future changes of prices and supply and demand conditions of the market obtained through the execution system. Therefore, from the viewpoint of the effects on the price discovery process, the most important issue will be what kind of information collection and distribution system the corresponding execution system employs, rather than the number of market makers in the market. There are three key pieces of information required for market participants’ decision-making, shown as the three axes in Figure 2: (1) information about executed trades (trade price, trade volume, etc.), (2) information about existing trade needs, (3) information about potential trade needs (effective supply and demand). Points which are further away from the origin suggest more sharing of information among market participants and an execution system will be illustrated as a solid or dotted triangle, as shown in the Figure, corresponding to its information collection and distribution mechanisms. 


Figure 2. Information distribution function of execution systems


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/6e0929e4060bf2816a78662572c01fda4dafd1ea5fccab9ac0bfadb04a973707.jpg)


## 4. Framework of analysis

In order to verify the decision-making mechanism of market liquidity summarised in Section 3 and to explore the possibility of quantitative analysis, we use a Monte Carlo simulation in our analysis. The reason for using this procedure is that when an analytical approach is adopted, it often results in solutions only being obtained in a relatively simple setting compared with that of actual market conditions. Since market microstructure theory, on which our analysis is based, formulates an individual trader’s behaviour at the micro level and aggregates the behaviour of many such traders to analyse market behaviour, a simulation approach becomes quite useful. By using a Monte Carlo simulation, which has developed rapidly in the field of finance theory, we can incorporate in our models traders who have complex decision-making functions or conditions and analyse the market behaviour patterns. 

Our model consists of two major parts. The first part models an individual trader’s decision-making and ordering, corresponding to the micro stage explained in Section 3. The second part models order flow aggregation in the trade execution system, which corresponds to the macro stage in Section 3. Parameters incorporated in the model are those that are unique to each market participant, such as (1) expected value of the asset, (2) confidence in the expected value, (3) the extent of risk aversion, and (4) sensitivity to feedback information obtained from the macro stage. Based on these parameters, a trader compares the benefit and cost (or risk) of each trade, selects a trade which maximises the net benefit, and places an order if the net benefit is consistent with the extent of risk aversion. Of the factors mentioned in Section 3 which affect trading behaviour, we assume explicit trading costs to be zero. We employ a continuous auction system which allows market orders and limit orders (during 

## 4.1 Simulation flow

The structure of our model is as follows: in a TSE-type market composed of N traders, we will conduct a simulation for M periods. In period t ( t =1, 2, ···, M ), all N traders can place an order once. Ordering rotation is randomly decided at each period, and each trader’s order will be executed based on the first-in rule, as in the TSE. The flow of the simulation is summarised in Figure 3. 

Figure 4 shows a rather detailed flow of the trader’s order decision process. Based on historical data such as price, order-book, and indication, a trader will forecast future market price and market liquidity (depth), take into account his/her own portfolio composition and risk preference, and make decisions about the order (order/not order, limit order/market order, order volume, and order price in the case of a limit order). All traders are uninformed about the true value of asset, and all market behaviour can be regarded as endogenous.<sup>25</sup> With respect to the trader’s trading strategy, we have prepared two types<sup>26</sup>: (1) one that captures the trend of price changes and aims to gain a short-term trading profit; and (2) one that conducts trading based on a long-term forecast of fundamentals and mean convergence. Each trader alters his/her trading strategy according to the performance of elements in the trading and market environment such as asset price and market depth. 

The format for accumulating market data is outlined in Figure 5. In period t , trader i places an order, the order is executed in the trade execution system, and market data will be produced as output: market data forms a matrix of N rows and 8 columns. In columns 1-4, the number of the trader whose limit/market order has been executed in the corresponding period (= period $t _ { i } )$ , the trade execution price, the trade volume, and the timing of the order will be entered, while in columns 5-8, the trader number whose limit order is remaining on the order book unexecuted, the buy/sell quote, the order volume, and the timing of the order will be entered according to price (from high to low) and time (first-in basis). 

The input (initial conditions) and the output (results) of the simulation are summarised as in Figure 6. 


Figure 3. Simulation flow


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/9808ce8dff0f86887704f461ed317aa33e2d44b8836c9fabf038de34a7483b36.jpg)



Figure 4. Order decision of a trader


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/f0f367ca3e87386b98d0d484cd2f28ce6674d458db8cebf5426358473bc870cd.jpg)



Figure 5. Market data for period $t _ { i }$ (order book information)


<table><tr><td></td><td>col. 1</td><td>col. 2</td><td>col. 3</td><td>col. 4</td><td>col. 5</td><td>col. 6</td><td>col. 7</td><td>col. 8</td></tr><tr><td>row 1</td><td>trader number</td><td>trade execution price</td><td>trade volume</td><td>timing of order</td><td>trader number</td><td>selling limit order</td><td>selling volume</td><td>timing of order</td></tr><tr><td>row 2</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td>row 3</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>trader number</td><td>buying limit order</td><td>buying volume</td><td>timing of order</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td></tr><tr><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td><td>.</td></tr></table>


Figure 6. Input/output of the simulation


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/ff2a724667f49c57ec18eac2fd2477849ec0d44eaee78c96ec417689af627fa6.jpg)


In our simulation, we classify the variables which imply market conditions as invisible variables and visible variables. The former cannot be observed in the actual market and include the trading patterns of market participants, traders’ expected values, confidence in such values, and risk preferences. The latter can be observed and include price indicators (market price, best-bid and best-ask prices), volume indicators (trading volume and order book profile), and information about order attributes. 

In the actual market, there is feedback by which current visible variables affect invisible variables from the next period onward. In particular, when the market is heading toward a ‘critical’ situation, decline in market liquidity, in addition to changes in price, will become an important factor representing the dynamics of an endogenous trading halt and resumption. For example, decline in market liquidity caused by a player’s exit from the market will induce an increase in transaction costs which will encourage other players to exit, and may thus result in a halt of market functioning. 

In the analysis, we observe the changes of market behaviour patterns brought about by altering the combination of parameters such as the composition of traders and the dispersion of traders’ expected values. Such analysis can be interpreted by observing what the effects would be when each trader’s invisible variables, such as the extent of risk aversion, change by the modification of market microstructure. In the actual market, market participants seem to change their behaviour based on visible variables, that is to say, invisible variables change dynamically. In our analysis, however, we provide constant figures for the invisible variables. And by analysing how changing patterns of visible variables differ when the constant figures change, we consider the relationship between these two groups of variables. 

## 4.2 A trader’s decision-making model

For our trade execution model we employ a continuous auction system patterned after that of the Tokyo Stock Exchange (TSE). There is no designated liquidity provider and market liquidity is only provided through trade orders from market participants. There are two types of traders in the market: “value 

traders” who place limit orders based on their expected values, and “momentum traders” who make market orders following short-term market trends.<sup>27</sup> The former maintain expected values of the asset based on information other than market data, and place limit orders according to differences between market prices and their expected values. The latter make market orders following short-term trends in market prices, and, as a result, they buy when market prices are rising and sell when market prices are falling.<sup>28</sup> In the following, we first look at the short-term price forecasting model, which both types of traders use, and explain the trading behaviour patterns of both value traders and momentum traders. 

## 4.2.1 Short-term price forecasting of the trader

In determining a trade order, a trader will make a short-term forecast of future market price based on historical market data.<sup>29</sup> The simplest pattern is shown in Figure 7. At period t , a trader monitors price movements during the period immediately before ( b ), measures the trend of mean price $\mu _ { h }$ and volatility $\sigma _ { h }$ , and based on this data, forecasts the market price (expected value $\mathrm { E } ( P _ { t + f } )$ and variance $\mathrm { V a r } ( P _ { t + f } ) )$ of the next trading opportunity, which is a period of f ahead. 


Figure 7. Price forecast of the trader


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/203f2d2fef9291b10200d60ee081218b8c778c14f83c31d8d6cb37bbae6b242a.jpg)



In addition to the simplest pattern in which the trader refers only to historical price information, we have also created a trader who considers volume information. Securities firms which are members of the TSE can obtain order-book information on their computer monitors. We assume that traders will incorporate such volume information in forming expectations of future market prices. Thus our model focuses on two indicators which can be obtained from the order-book information. The first indicator


is gross order volume, which is the sum of limit orders for selling and buying, and can be interpreted as a proxy of market depth. In general, the price risk caused by factors such as the impact of trading on market price will increase as gross order volume decreases, and will decrease as gross order volume increases. The second indicator is net order volume which shows the imbalance between limit orders for selling and buying. When selling orders exceed buying orders, we can interpret this as downward pressure on market prices, while buying orders exceeding selling orders can be interpreted as upward pressure on market prices. Let $V _ { g }$ be gross order volume (buying order volume plus selling order volume), $V _ { n }$ be net order volume (buying order volume minus selling order volume), and assume that traders who consider volume information will modify the market price trend and volatility as follows: 

(1) 

$$
\mu_ {h} ^ {\prime} = \mu_ {h} + \alpha \cdot V _ {n} / \overline {{V _ {g}}}\tag{2}
$$

$$
\sigma_ {h} ^ {\prime} = \sigma_ {h} \cdot \left(\frac {V _ {g}}{\overline {{V _ {g}}}}\right) ^ {- \beta}
$$

where $\mu _ { h } ^ { \prime }$ and $\boldsymbol { \sigma } _ { h } ^ { \prime }$ are obtained by revising the market price trend $( \mu _ { h } )$ and volatility $( \sigma _ { h } )$ without considering volume information. In addition, $\overline { { V } } _ { g }$ is the average of $V _ { g }$ obtained by monitoring $V _ { g }$ for the period immediately before ( b ). By using this value as a benchmark, traders will relatively compare the current and average state of market liquidity. α and $\beta$ are positive constants.<sup>30</sup> 

## 4.2.2 Trading behaviour of value traders

In addition to forecasting future short-term prices, value traders also maintain subjective information $\widetilde P$ about the fundamental value of an asset. We assume that the expected values of all traders in the market will, when aggregated, follow lognormal distribution with a standard deviation of $\sigma _ { V }$ . Each trader individually forms his/her expected value; its initial value is exogenously provided in our simulation, although this initial value does not represent an asset’s true value. The value trader will determine his/her order based on his/her expected value $\widetilde P$ and expectation distribution of the short-term price $P _ { t + f }$ . In placing limit orders, the order price (selling: $P _ { a s k }$ , buying: $P _ { b i d } )$ will be established to allow for maximised expected return $\mathbb { E } ( R \vert P _ { a s k } )$ or $\operatorname { E } ( R { \big | } P _ { b i d } )$ , which can be obtained by multiplying return of the order and the probability of being executed within the interval $\left[ t , t + f \right]$ prior to the next ordering opportunity. 

Selling limit order Maximum $\mathrm { E } ( R { \big | } P _ { a s k } ) { = } \mathrm { P r } ( P _ { t + f } \geq P _ { a s k } ) { \cdot } ( P _ { a s k } - \widetilde { P } )$ 

$$
\text {Buying   limit   order   Maximum } \mathrm{E} (R \mid P _ {b i d}) = \operatorname * {P r} (P _ {t + f} \leq P _ {b i d}) \cdot (\tilde {P} - P _ {b i d})
$$

Value traders will recognise their lack of confidence in their forecasts as the risk in submitting orders. When the expected return is substantially larger than the risk, the trader will place either a selling or buying order, which has a larger expected return. In our model, this lack of confidence is given as an expected dispersion (standard deviation) <sub>γ</sub> of the aggregate of each value trader’s expected values.<sup>31</sup> 

$$
\mathrm{E} (R \mid P _ {a s k}) > \mathrm{E} (R \mid P _ {b i d}) \text { and } \left. \frac {\mathrm{E} (R \mid P _ {a s k})}{\gamma} > A \right. \text { then   Selling   limit   order } (P _ {a s k})
$$

$$
\mathrm{E} (R \mid P _ {a s k}) <   \mathrm{E} (R \mid P _ {b i d}) \text {and} \left. \mathrm{E} (R \mid P _ {b i d}) / \gamma > A \text {then Buying limit order} (P _ {b i d}) \right.
$$

where A is a positive constant reflecting a trader’s risk aversion. 

## 4.2.3 Trading behaviour of momentum traders

Momentum traders are indifferent to the level of market prices and their trading is based on the trends and volatility of market prices. Namely, based on the short-term forecast by taking into account historical market data, they compare the expected earnings ratio with risks until the next trading opportunity, and, if the extent of their risk aversion allows, make selling market orders (when market prices are falling), or buying market orders (when market prices are rising). The order of the momentum trader is: 

$$
\mu_ {h} ^ {\prime} / \sigma_ {h} ^ {\prime} <   - B \quad \text { then } \quad \text { Selling   market   order }
$$

$$
\mu_ {h} ^ {\prime} / \sigma_ {h} ^ {\prime} > B \quad \text { then } \quad \text { Buying   market   order }
$$

where $\mu _ { h } ^ { \prime }$ and $\boldsymbol { \sigma } _ { h } ^ { \prime }$ are obtained from formulas (1) and (2) of Section 4.2.1, and B is a positive constant which reflects a trader’s risk aversion. 

## 5. Results of analysis

## 5.1 Basic design of simulation

Now we introduce the standard case of our simulation. We will set the parameters as follows: 

Number of traders: 60 

$$
\binom{\text { value traders:50 }}{\text { momentum traders:10 }}
$$

Market access frequency of the traders: 1/10 

Look-back periods of the traders ( b ): 10 

Forecasting periods of the traders ( f ): 10 

Mean of traders’ expected values $( \widetilde { P } ) { : 1 , 0 0 0 } \ : ( \mathrm { y e n } )$ 

Standard deviation of expected values $( \sigma _ { V } ) \colon 0 . 0 5$ 

Extent of risk aversion for value traders ( A ): 2 

Extent of risk aversion for momentum traders ( B ): 2 

Extent of order imbalance $( V _ { n } )$ being reflected through trends $( \mu _ { h } ) \colon 0$ 

Extent of gross order volume $( V _ { g } )$ ) being reflected through volatility $( \sigma _ { h } ) \colon 0 .$ 

In the following simulations (5.2–5.5), the standard cases are: 10 momentum traders (5.2), $\sigma _ { \nu } = \gamma = 0 . 0 5 ( 5 . 3 )$ , both types of traders’ extent of risk aversion = 2 (5.4), and $\alpha = \beta = 0$ (5.5). Observed indicators are as follows: 

Quote existence probability: 35% 

Trade frequency: 1.86 times per period 

Execution price volatility: 0.0135 

Mean price volatility: 0.0131 

Average spread: 0.0098 

Average of gross order volume: 43 

Volatility of gross order volume: 0.49 

Standard deviation of order imbalance / average of gross order volume: 0.69. 

## 5.2 Composition of traders

As indicated in the previous section, our model uses two types of traders: value traders and momentum traders. In a market composed of 50 traders, we will analyse the effects of market behaviour when the number of momentum traders increases.<sup>32</sup> Figure 8 summarises the features of the market data. We can see by various indicators that liquidity supply decreases as the proportion of value traders declines, and liquidity absorption increases as the proportion of momentum traders increases. 

We can see from Figures 8-1 and 8-2 that since orders on the book diminish as market orders from momentum traders increase, the number of cases in which quotes disappear would rise (probability of quote existence falls), while trade frequency would increase. However, there are diminishing, instead of linear, trends in both effects: when the number of momentum traders increases past a certain level (30 or 40 in our case), the probability of quote existence no longer falls, and trade frequency no longer increases. In Figure 8-1, when the number of momentum traders exceeds 30 and the probability of quote existence falls to a level of around 20%, a phase in which market orders buy up the selling order book to exhaust the orders, and a phase in which market orders sell down the buying order book to exhaust the orders, show up one after another. In addition, at the point when one phase shifts to another, quotes disappear, that is, no trading will be executed: it is unlikely to see further decline in the probability of quote existence or further increase in trade frequency. 

Next, when we see the volatility of execution price and mean quote during the simulation period (Figures 8-3 and 8-4) on the one hand, the volatility increases in the buying up/selling down process mentioned above when the number of momentum traders increases to 30. On the other hand, when the proportion of momentum traders exceeds a certain value, the probability of quote existence reaches its limit and thus trading becomes difficult to execute, or price is not discovered smoothly; as a result, the volatility of execution price and mean quote is contained. 

Figures 8-5 and 8-6 show the development of two liquidity indicators, average spread and average gross orders. During the process in which the number of momentum traders increases from zero to 20, orders on the order book are exhausted as market order increases, thereby spread increases and gross order book volume decreases. However, there seems to be a lower-limit to the decline in liquidity accompanied by the increase in the number of momentum traders. When the composition of momentum traders exceeds a certain level, trade frequency is contained, thus making a further liquidity decline difficult. 

Figure 8-7 displays volatility of gross order book volume. This indicator can be regarded as representing the ease with which the order book is restored to its original state after a certain decrease in orders. In essence, it is a proxy for market liquidity resiliency. An increase in the number of momentum traders will increase the resiliency of market liquidity to some extent, although this increasing effect will diminish and become constant because of the relative decrease in limit orders. 

Finally, Figure 8-8 shows the standard deviation of net order book volumes, which represents the bias of market supply-demand. When value increases, this suggests that a large supply-demand bias (either selling book or buying book exists) is more likely to occur; and when the value diminishes, it is more likely that the market will reach equilibrium. We can observe that when the composition of momentum traders exceeds a certain ratio, order imbalance is more likely to emerge. 

## 5.3 Dispersion of expectations on future prices and traders’ confidence

Value traders subjectively forecast the fundamental value of their own assets. At the same time, they assume a variance of the expectation distribution for the asset prices of all market participants. The variance is inversely proportional to the confidence in their expected value. In other words, the variance of expectation distribution decreases when traders are confident of their price forecasts, while variance tends to be large when traders are not so confident of their forecasts. As shown in 4.2, traders recognise magnitude of variance as a risk in placing orders 

Although expected values and the assumed variance of the expectation distribution change dynamically in an actual market, here we treat them as constant and analyse how the difference between their sizes affects market behaviour patterns. Figure 9 shows the development of each indicator when market participants’ expected variance and true variance, respectively, are changed. 

First we first look at the changes in the probability of quote existence and trade frequency (Figures 9-1 and 9-2). When the expected variance equals the true variance, namely on the 45 degree line (plain), both indicators move almost at constant levels (probability of quote existence=0.3, trade frequency=1.8). When the expected variance is less than the true variance, namely below the 45-degree plane, both indicators increase as the difference between expected and true variance increases (moves toward the other side of the plane). On the other hand, when the expected variance is larger than the true variance, namely above the 45-degree plane, both indicators decrease as the difference between expected and true variance increases (moves toward this side of the plane). This can be interpreted to mean that: when market participants underestimate actual risks in the market, trading becomes more active than when risk is correctly estimated; while when risks are overestimated, trading rapidly diminishes. 

Second, we look at changes in the volatility of execution price and mean value (Figures 9-3 and 9-4). The slope along the horizontal axis (expected variance) is almost flat regardless of the value of the true variance (which is depicted on the axis heading toward the back), while showing acclivity toward the back regardless of the values of expected variance. This suggests volatility falls as true variance declines. This implies the possibility that the magnitude of expected variance does not affect the price discovery mechanism, and the magnitude of price changes is determined by the actual dispersion of market participants’ expectations. 

A similar feature can be pointed out for the development of average spread (Figure 9-5). The slope toward the direction of the horizontal axis is flat regardless of the level of the true variance, while showing acclivity toward the back regardless of the magnitude of the expected variance. This implies the possibility that market liquidity measured by the average spread has been affected by the true variance instead of the expected variance, and that market liquidity declines as true variance increases. 

Figures 9-6 and 9-7 focused on the gross order book volume as an indicator of the depth of market liquidity. We can see that, as in the case of the probability of quote existence and trade frequency, the line of the story changes at the border of the 45-degree plane, where the expected variance equals the true variance. In the space below the 45-degree plane, where the true variance is larger than the expected variance, the gross volume of the order book increases as the difference between expected and true variance increases (moves toward the other side of the plane), while the volatility of the gross volume of the order book is almost constant. On the other hand, in the space above the 45-degree plane, where the expected variance is larger than the true variance, both the gross volume of the order book and its volatility decline as the difference between the expected variance and the true variance (moving toward this side of the plane) rapidly declines. This seems to imply the existence of a mechanism in which the depth of market liquidity increases when market participants underestimate the risk, while it declines rapidly along with resiliency when the risks are overestimated. 

## 5.4 Extent of the traders’ risk aversion

Figure 10 shows how the extent of traders’ risk aversion affects market conditions. Regardless of the extent of the momentum traders’ risk aversion, when the extent of value traders’ risk aversion falls (towards the back of the Figure), liquidity indicators such as the probability of quote existence, trade frequency, and order book profile (average $V _ { g } )$ (Figures 10-1, 10-2 and 10-6) rise, while price volatility (Figures 10-3 and 10-4) increases as the extent of the value traders’ risk aversion rises (toward the back of the Figure). The average spread (Figure 10-5) is not likely to be affected too much by the extent of risk aversion. Regarding market resiliency (Figure 10-7) and order imbalance (Figure 10-8), they both increase as the extent of the value traders’ risk aversion rises, while they tend to decrease once the risk aversion exceeds a certain magnitude (3 in this case). 

## 5.5 Sensitivity to order book information

In the TSE, member securities firms can monitor the order book through their private computer systems. The profile and size of the order book represent the imbalance of the orders or the magnitude of market impact, and can be interpreted as pressure (upward/downward) on future prices or volatility, which is the so-called liquidity risk or liquidity cost. Various ways to quantify such liquidity risk have been proposed, although no consensus has yet been formed. By using the simple model shown in $4 . 2 ,$ we will conduct a simulation which incorporates this market liquidity effect. In other words, the trader will forecast small (large) future price volatility if the gross order volume in the order-book is large (small), and a rise (fall) in future prices if the order volume is positive (negative). Market behaviour obtained by changing traders’ sensitivity to market liquidity indicators, namely α and $\beta$ , is shown in Figure 11. 

We can see that as sensitivity against order book information increases, the probability of quote existence and gross volume of the order book (average $V _ { g } )$ ) increases to as much as three times as before, and the order imbalance (Figure 11-8) substantially diminishes, suggesting an overall improvement in market liquidity. However, when viewed from indicators such as trade frequency, average spread, and market resiliency, market liquidity tends to decline as traders’ sensitivity to order book information increases (Figures 11-2, 11-5, and 11-7). 

## 6. Conclusions and further issues

Earlier part in this paper (Section 2), we defined ‘market liquidity,’ a concept widely recognised among market participants without explicit definition, and summarised its formation mechanism. In the latter part of this paper, we constructed an artificial market model consisting of hypothetical traders, characterised by various endogenous variables, such as the expected values and the extent of risk aversion, and a hypothetical execution system which matches orders from the traders, and conducted analyses based on a Monte Carlo simulation. Specifically, by giving constant values to traders’ expected values, confidence in their forecasts, and the extent of risk aversion, we observed the relationship between the size of such constant values and market behaviour. 

The results of the simulations can be summarised as follows: 

Effects of trading methods: If the proportion of traders who submit market orders based on short-term market price movements increases, market liquidity tends to decline. 

Effects of market participants’ confidence: If traders underestimate risk, trade becomes more active than when risks are correctly recognised, and market depth increases; on the other hand, if traders overestimate risk, trade rapidly becomes difficult, and market depth and market resiliency decline. However, market liquidity, indicated by price indicators such as price volatility and bid-ask spread, is determined by the actual dispersion of traders’ expectations regardless of the traders’ subjective confidence. 

Effects of the extent of traders’ risk aversion: market liquidity increases and price becomes less volatile as the degree of traders’ risk-aversion declines. 

Effects of traders’ sensitivity to order volume information: As sensitivity rises, probability of quote existence rises, gross order book volume increases, and supply-demand imbalance widens, suggesting improvements in market liquidity indicators such as trade frequency, average spread, and market resiliency, tend to decline. 

The results drawn in this paper from the simulation approach will differ depending on the structure of the model or initial conditions, and thus cannot be directly applicable to the actual market. However, by continuing our efforts to analyse, both conceptually and empirically, the relationship between market participants’ endogenous, invisible variables, such as confidence and the extent of risk aversion, and changing patterns of market behaviour, we may be able to collect more insights into market dynamics. 

## The following issues require further research:

We need to obtain deeper insights into how market participants’ decision-making is affected by feedback from market information on price and volume. By incorporating the feedback effects from market data (visible variables) to traders’ behaviour (invisible variables), we could replicate market dynamics more realistically.<sup>33</sup> 

We need to increase the sophistication of the model by incorporating some additional market structures into it. Specifically, by comparing the simulation results using the artificial market model and the results of the empirical analysis, based on high-frequency data, we could make the trader’s behaviour model more realistic, for example, closer to that of stock market participants on the TSE. 

In addition to the TSE type market, which employs a continuous auction system, the simulation approach used in our analysis also applies to a market with market makers, or to markets in which various execution systems co-exist. Structural factors such as tick-size, or the extent of information disclosure can also be incorporated into the model. In the future, we hope to quantitatively analyse the effects of these various market structures on market. 


Figure 8. Effects of the composition of traders


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/4fa20cf78ade68a8d51c8247acb86327687b6bd24bcd026d11497939f8a2eba0.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/bc3bb0be526306f283255b51774423101efee48d08d836117eb65e22386bd98a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/4a1dd4f026a718a928142e8e6bc8c6f84048a38593a81ac4978d03398486fea3.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/4b5e084d1e3e6c23b12da6bca2a5c08fc5fece4a10875ce506d56a44ce0e69a1.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/c2c222c8731c37d55e59a7c0ce8975a29c843807c06c7bb5be75ce2146b29611.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/e423a7eb0fcaf08a734bab4a587b450e26da5acc24d22ffd805e140b7adb39c5.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/2666a01bda9022bf15f4173b43a03d92e1e6ed22716de0d93006f5814fb13337.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/3dfb2ea2e4a4d7b3045e1b032f37f33975e690977e565f34cbcc3608d4c714ee.jpg)



Figure 9. Effects of dispersion of expectations on future prices and traders’ confidence


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/6f2dbded43d467493108128ceeb9ebdb89d405fcb98ace7025e80498653dff5a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/e43a06c345f384166e4eb35c9f55e70152167ef5d0d8fb076ad2711dc2bb967f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/c5cec605f0c9458ed54578fe80c29fcfcf95a678f552f57d19c5ee9ab19186ae.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/d868369762516eff48c537541fb4efb4d95a867c7a9f0ac46efa5b65f94c8f35.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/545419d0be57b97680bbc8c23f874bee3d2da9bc5396bf50eb7c1de3ff063e99.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/d1a6649594befc16f15d89d4b4ddce5b46193f54c4806993335658ab402a8a6b.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/b7b178b6560560197c9eea3a27844dab3f19fb21de5f78873fbc719aa2242e80.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/9cf54d554418ca7ab71802af9314bd98e961fe8d4b3041c03d60a88732b81f2f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/ca14e345c190d5791b2799d1c84565d248bae7ea5f3b6d2cc45661aaf88440a3.jpg)



Figure 10. Effects of the extent of traders’ risk aversion


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/df79165a5878e189297df5f38b844fc801e0a60af860fd04e644e6f87de1f8d2.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/3246f14911b554e4245f35017769e1fc951ab076b379c56ade741d7339b886b9.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/29687938b262abdd193964dbbc8d9efb3eecc150dd7be6243d62d5aa7d0856a1.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/efb5b5758bd28f2702dc8584eade4e60e5a414c7d0b969d7e3a5db9605b9292a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/34f6075fa4ab598716b6ff705254e89332c3f35ac95a30b8717738b95cb31184.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/acf43d222cc315ba475fa1b7ac4f6d2653be1330ad0d56d1ba4e1d70d3e6ab00.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/7d9adb7b3cbc9507b43b953640284ce49878edaa55acab7f8f881c0a5c4d161a.jpg)



Figure 11. Effects of sensitivity to order book information



Figure 11-1. Probability of quote existence


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/b4925bd0c24713391a78debf41bec1afbf5b9650268219d990e9ae9d46f19988.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/9750844e57858cc4554b080b006b7a8dc8d6284d33661fb512e01e8019ed632c.jpg)



Figure 11-3. Volatility of trade price


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/b53f3a7d19d588c7d459131c841022a9ec6033fb217bfb995944cec750b441ce.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/545f19625b7f87a5da64e6d5ccb447f478264cdc76b1cd069e7a80335c59593a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/7e5bcb9aa96d1e392935cfdca787dafc3336184a836aa61fa9524696cc05c063.jpg)



Figure 11-6. Average of gross orders


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/b9802c43761cefea80b72e1918ed5d65767bae4d5a5805f8ff56f8651820bec8.jpg)



Figure 11-7. Volatility of gross order book volume


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/6411201f374046f75da7e7b3fcc7e3396f36b6e792d5945cebd284aa49afdc84.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/24cd8fa7ce8669f5644350e8564facb8bc424182638852149fedc19c85c45ab0.jpg)


## Appendix

# Dynamic measurements of market liquidity

## A.1 Market impact

Market impact ( λ) provides information about the ability of the market to absorb trades as changes in price upon trade execution. λ is an indicator which shows to what extent the bid-ask spread will be widened upon execution of a trade.<sup>34</sup> λ includes two pieces of information: the volume of trade orders in a certain price range (gross order volume) and whether there are orders in each price range (price continuity or order book-profile). For the purpose of statistical analyses, we calculate λ standardised by gross order volume, which is denoted by $\bar { \lambda } . \bar { \lambda }$ will provide information about the order bookprofile which is independent of gross order volume (Figure A-1 shows how to measure). This indicator would be useful when we conduct a cross-sectional analysis, not an intertemporal analysis, on market impact. If the availability of current order book information improves, $\lambda \ ( \mathrm { o r } \ \bar { \lambda } )$ will be a more useful measure for forward-looking information of market liquidity. 

## A.2 Market resiliency

Another dynamic indicator of market liquidity is market resiliency (<sub>γ</sub> ). It provides information about potential trade needs (effective supply and demand) which are not explicitly placed in the market as an order. The definition of <sub>γ</sub> is yet to be fixed, although measuring an indicator which shows how the market autonomously restores its original state after a trade execution has added to the market may be a way to measure <sub>γ</sub> . In physics, the restoration speed of a coil, for example, is measured as an indicator of resiliency.<sup>35</sup> As an analogy, by measuring the widened bid-ask spread caused by trade executions and the period of time required for the spread to be restored the state immediately before the execution, we can calculate the speed of resiliency, and be able to recognise market resiliency. This method captures the process of trade needs, which were potential immediately before the trade execution, to materialise upon trade execution, and enable us to measure market liquidity which takes into account of potential trade needs. However, we should note that, in an actual market, <sub>γ</sub> may not be observable since new market orders, not limit orders which reduce the widened spread, could well be placed after the bid-ask spread been widened by a trade execution. How to take account of such market orders mingled during the observation period and bring the concept of market resiliency close to an observable indicator will be our future task. 


Figure A-1. Example of market impact $( \bar { \lambda } )$ calculation


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/069dfd71a0d1877087f2519166dbfbbbce01cf1d92d69d932a5ed9923f65ff73.jpg)



Figure A-2. Example of market resiliency ( <sub>γ</sub> ) calculation


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/58a4cc44-3ced-42ac-82ef-6e12769243b1/888f0ee9701b999b0706a1397a7e05cbb3d682feada47ac0979660cbeab39a7a.jpg)




Fukao, M 1988, “Kin-yuno kokusaikaga kawase-reitono hendou oyobi kokusai-shushini ataeru eikyonituite (in Japanese),” Kin-yu Kenkyu Vol.7, No. 4, Bank of Japan. 





Breedon, F and A Holland, 1997, “Electronic versus Open Outcry Markets: The Case of the Bund Futures Contract,” Bank of England. 





Brennan, M J, 1986, “Theory of Price Limits in Futures Markets,” Journal of Financial Economics Vol. 16. 





Brown, D P, and R H Jennings, 1989, “On Technical Analysis,” Review of Financial Studies Vol. 2. 





Brown, D P, and Z M Zhang, 1997, “Market Orders and Market Efficiency,” Journal of Finance Vol. 52, No. 1. 





Cohen, K S Maier, R Schwartz, and D Whitcomb, 1986, “Transactions Costs, Order Placement Strategy, and Existence of the Bid-Ask Spread,” Journal of Political Economy Vol. 89, 287-305. 





Easley, D, and M O’Hara, 1992, “Adverse Selection and Large Trade Volume: The Implications for Market Efficiency,” Journal of Financial and Quantitative Analysis Vol. 27, No. 2. 





Fleming, M, and E Remolona, 1999, “Price Formation and Liquidity in the U.S. Treasury Market: The Response to Public Information,” Journal of Finance, forthcoming. 





Gerety, M S, and J H Mulherin, 1992, “Trading Halts and Market Activity: An Analysis of Volume at the Open and the Close,” Journal of Finance Vol. 57, No. 5. 





Greenwald, B, and J Stein, 1988, “The Task Force Report: The Reasoning Behind the Recommendations”, Journal o Economic Perspectives Vol. 2, No. 3. 





Greenwald, B, and J Stein, 1991, “Transaction Risk, Market Crashes, and the Role of Circuit Breakers,” Journal of Business Vol. 64, No. 4. 





Harris, L, 1990, “Estimation of Stock Price Variances and Serial Covariances from Discrete Observations,” Journal of Financial and Quantitative Analysis Vol. 25, 291-306. 





Kyle, A S, 1985, “Continuous Auctions and Insider Trading,” Econometrica Vol. 53, 1315-1335. 





Lauterbach, B, and U Ben-Zion, 1993, “Stock Market Crashes and the Performance of Circuit Breakers: Empirical Evidence”, Journal of Finance Vol. 58, No. 5. 





Lyons, R, 1992, “Equilibrium Microstructure in the Foreign Exchange Market,” Working Paper, University of California at Berkley. 





Lyons, R, 1995, “Tests of Microstructural Hypotheses in the Foreign Exchange Market,” Journal of Financial Economics Vol. 39, No. 2&3. 





Muranaga, J, and T Shimizu, 1999, “Expectations and Market Microstructure when Liquidity is Lost,” mimeo. 





Presidential Task Force on Market Mechanism: Report, 1988. 





Proudman, J, 1995, “The Microstructure of the UK Gilt Market,” Bank of England Working Paper Series No. 38. 





Roll, R, 1988, “The International Crash of October 1987”, Financial Analysts Journal (September 1988). 





Subrahmanyam, A, 1994, “Circuit Breakers and Market Volatility: A Theoretical Perspective”, Journal of Finance Vol. 59, No. 1. 

