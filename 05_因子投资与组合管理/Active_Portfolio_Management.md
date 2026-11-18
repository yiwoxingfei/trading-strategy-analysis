

<!-- === Source: MinerU_markdown_Active_Portfolio_Management_2121858659528060943.md (Page 1) === -->

## Active Portfolio Management By Richard C. Grinold and Ronald N. Kahn

Part I Foundations....2   
Chapter 1 Introduction....2   
Chapter 2 Consensus Expected Returns: The CAPM....3   
Chapter 3 Risk....3   
Chapter 4 Exceptional Return, Benchmarks, and Value Added....5   
Chapter 5 Residual Risk and Return: The Information Ratio....6   
Chapter 6 The Fundamental Law of Active Management....9   
Part II Expected Returns and Valuation....11   
Chapter 7 Expected Returns and the Arbitrage Pricing Theory....11   
Chapter 8 Valuation in Theory....13   
Chapter 9 Valuation in Practice....13   
Part III Implementation....14   
Chapter 10 Forecasting....14   
Chapter 11 Information Analysis....16   
Chapter 12 Portfolio Construction....18   
Chapter 13 Transactions Costs, Turnover, and Trading....22   
Chapter 14 Performance Analysis....24   
Chapter 15 Benchmark Timing....29   
Chapter 16 Summary....30 

# Active Portfolio Management

# By Richard C. Grinold and Ronald N. Kahn

## Part I Foundations

## Chapter 1 Introduction

I. A process for active investment management 

The process includes researching ideas, forecasting exceptional returns, constructing and implementing portfolios, and observing and refining their performance. 

II. Strategic overview 

1. Separating the risk forecasting problem from the return forecasting problem. 

2. Investors care about active risk and active return (relative to a benchmark). 

3. The relative perspective will focus us on the residual component of return: the return uncorrelated with the benchmark return. 

4. The information ratio is the ratio of the expected annual residual return to the annual volatility of the residual return. The information ratio defines the opportunities available to the active manager. The larger the information ratio, the larger the possibility for active management. 

5. Choosing investment opportunities depends on preferences. The preference point toward high residual return and low residual risk. We capture this in a mean/variance style through residual return minus a (quadratic) penalty on residual risk (a linear penalty on residual variance). We interpret this as “riskadjusted expected return” or “value added.” 

6. The highest value added achievable is proportional to the squared information ratio. The information ratio measures the active management opportunities, and the squared information ratio indicates our ability to add value. 

7. According to the fundamental law of active management, there are two sources of information ratio: 

IR = IC * BR 

Information coefficient: a measure of our level of skill, our ability to forecast each asset’s residual return. It is the correlation between the forecasts and the eventual returns. 

- Breadth: the number of times per year that we can use our skill. 

8. Return, risk, benchmarks, preferences, and information ratios constitute the foundations of active portfolio management. But the practice of active management requires something more: expected return forecasts different from the consensus. 

9. Active management is forecasting. Forecasting takes raw signals of asset returns and turns them into refined forecasts. This is a first step in active management implementation. The basic insight is the rule of thumb 

ALPHA = VOLATILITY*IC*SCORE 

that allows us to relate a standardized (zero mean and unit standard deviation) 

score to a forecast of residual return (an alpha). The volatility is the residual volatility. IC is the correlation between the scores and the returns. 

## Chapter 2 Consensus Expected Returns: The CAPM

1. The CAPM is about expected returns, not risk. 

2. There is a tendency for betas towards the mean. 

3. Forecasts of betas based on the fundamental attributes of the company, rather their returns over the past 60 or so months, turn out to be much better forecasts of future beta. 

4. Beta allows us to separate the excess returns of any portfolio into two uncorrelated components, a market return and a residual return. (no theory or assumption are needed to get this point) 

5. CAPM states that the expected residual return on all stocks and any portfolio is equal to zero. Expected excess returns will be proportional to the portfolio’s beta. 

6. Under CAPM, an individual whose portfolio differs from the market is playing a zero-sum game. The player has additional risk and no additional expected return. This logic leads to passive investing;, i.e., buy and hold the market portfolio. 

7. The ideas behind the CAPM help the active manager avoid the risk of market timing, and focus research on residual returns that have a consensus expectation of zero. 

8. The CAPM forecasts of expected return will be as good as the forecasts of beta. 

## Chapter 3 Risk

I. Introduction 

1. Risk is standard deviation of return. The cost of risk is proportional to variance. 

2. Investors care more about active and residual risk than total risk. 

3. Active risk depends primarily on the size of the active position and not the size of the benchmark position. 

II. Defining risk 

1. Variance will add across time if the returns in one interval are uncorrelated with the returns in other intervals of time. The autocorrelation is close to zero for most asset classes. Thus, variances will grow with the length of the forecast horizon and the risk will grow with the square root of the forecast horizon. 

2. Active risk = Std (active return) = Std(r<sub>P</sub> – r<sub>B</sub>) 

3. Residual risk of portfolio P relative to portfolio B is defined by 

$$
\omega_ {P} = \sqrt {\sigma_ {P} ^ {2} - \beta_ {P} ^ {2} \sigma_ {B} ^ {2}}
$$

Where, $\beta _ { P } = \frac { C o \nu ( r _ { P } , r _ { B } ) } { V a r ( r _ { B } ) }$ 

4. The cost of risk equates risk to an equivalent loss in expected return. This cost will be associated with either active or residual risk. 

## III. Structural Risk Models

$$
r _ {n} (t, t + 1) = \sum_ {k} \beta_ {n, k} (t) \bullet f _ {k} (t, t + 1) + u _ {n} (t)
$$

Where, r is excess return. Beta is the exposure of asset n to factor k. it is known at time t. 

## IV. Choosing the factors

1. All factors must be a priori factors. That is, even though the factor returns are uncertain, the factor exposures must be known a priori, i.e., at the beginning of the period. Three types of actors: 

2. Reponses to external influence: macro-factors. 

They suffer from two defects: 

The response coefficient has to be estimated through a regression analysis or some similar technique. Æ Error in variables problem. 

The estimate is based on behavior over a past period of approximately five years. It may not be an accurate description of the current situation. Æ These response coefficients can be nonstationary. 

## 3. Cross-sectional comparisons

These factors compare attributes of the stocks with no link to the remainder of the economy. These cross-sectional attributes can themselves be classified in two groups: fundamental and market. 

Fundamental attributes include ratios such as dividend yield and earnings yield, plus analysts’ forecasts of future earnings per share. 

Market attributes include volatility over a past period, momentum, option implied volatility, share turnover, etc. 

## 4. Statistical factors

principal component analysis, maximum likelihood analysis, expectations maximization analysis, using returns data only; 

We usually avoid statistical factors, because they are very difficult to interpret, and because the statistical estimation procedure is prone to discovering spurious correlation. These models also cannot capture factors whose exposures change over time. 

## 5. Three criteria: incisive, intuitive and interesting.

- Incisive factors distinguish returns. 

- Intuitive factors relate to interpretable and recognizable dimensions of the market. 

- Interesting factors explain some part of performance. 

6. Typical factors: 

Industries 

## Risk indices: measure the differing behavior of stocks across other, nonindustry dimensions, such as, volatility, momentum, size, liquidity, growth, value, earnings volatility and financial leverage.

Each broad index can have several descriptors. E.g. volatility measures might include recent daily return volatility, option implied volatility, recent price range, and beta. Though typically correlated, each descriptor captures one aspect of the risk index. We construct risk index exposures by weighting exposures of the descriptors within the risk index. 

7. Quantify exposures to descriptors and risk indices – standardize exposures! 

## Chapter 4 Exceptional Return, Benchmarks, and Value Added

I. Introduction 

1. Exceptional expected return is the difference between our forecasts and the consensus. 

2. Benchmark portfolios are a standard for the active manager. 

3. Active management value added is expected exceptional return less a penalty for active variance. 

4. Management of total risk and return is distinct from management of active risk and return. 

5. Benchmark timing decisions are distinct from stock selection decisions. 

II. Terminology 

1. Beta is the beta between portfolio and benchmark. 

2. Active position is the difference between the portfolio holdings and the benchmark holdings. 

$1 \mathrm { { p } _ { \mathrm { { A } } } = \mathrm { { h } _ { \mathrm { { P } } } - \mathrm { { h } _ { \mathrm { { B } } } } } }$ 

3. Active variance: 

$$
A V a r _ {P} ^ {2} = h _ {P A} ^ {T} \bullet V \bullet h _ {P A} = \sigma_ {P} ^ {2} + \sigma_ {B} ^ {2} - 2 \bullet \sigma_ {P, B} = \beta_ {P} ^ {2} \sigma_ {B} ^ {2} + V a r (r e s i d u a l r i s k)
$$

III. Components of Expected return $( \mathrm { R } _ { \mathrm { n } }$ is the total return on asset n) 

$\mathrm { E } ( \mathrm { R } _ { \mathrm { n } } ) = 1 + i _ { F } + \beta _ { \mathfrak { n } } \bullet \mu _ { B } + \beta _ { \mathfrak { n } } \bullet \Delta f _ { B } + \alpha _ { \mathfrak { n } }$ --- (4.1) 

- Time premium, $\mathrm { i } _ { \mathrm { F } } $ the compensation for time. 

Risk premium: ${ \mathrm { b e t a } } ^ { * } \mu .$ where μ is expected excess return on the benchmark, usually a very long-run average (50 years). 

Exceptional benchmark return: beta $^ { * } \Delta \mathrm { f } _ { \mathrm { B } } , \Delta \mathrm { f } _ { \mathrm { B } }$ is your measure of that difference between the expected excess return on the benchmark in the near future and the long-run expected excess return. 

- Alpha: expected residual return. 

Exceptional expected return: beta $\bf ^ { * } \Delta \Delta \Delta ^ { * } \Delta \bf { a l p h a } .$ : the first term measures benchmark timing; the second component measures stock selection. 

IV. Management of total risk and return 

1. Active management starts when the manager’s forecasts differ from the consensus. 

2. The forecast of expected excess return for portfolio p can be expressed as: $f _ { P } = \beta _ { P } \bullet f _ { B } + \alpha _ { P }$ ---- Same as (4.1) 

Where, $f _ { \mathrm { B } }$ is the forecast of expected excess return for the benchmark. These forecasts will differ from consensus forecasts to the extent that $f _ { \mathrm { B } }$ differs from the consensus estimate $\mu _ { B }$ , and alpha differs from zero. 

## 3. The total return – total risk tradeoff (too aggressive)

$U ( P ) = f _ { _ P } - \lambda _ { _ T } \bullet \sigma _ { _ P } ^ { 2 }$ , where f is the expected excess return and the second term is a penalty for risk. λ measures aversion to total risk. 

$$
\lambda_ {T} = \frac {\mu_ {B}}{2 \bullet \sigma_ {B} ^ {2}}
$$

$$
\beta_ {P} = \frac {f _ {B}}{2 \bullet \lambda_ {T} \bullet \sigma_ {B} ^ {2}} = 1 + \frac {\Delta f _ {B}}{\mu_ {B}} = 1 + \text { active   beta } (\beta_ {P A}), \text { which   is   the   ratio   of   our }
$$

forecast for benchmark exceptional return to the consensus expected excess return on the benchmark Æ we will argue that this expected utility criterion will lead to portfolios that are typically too aggressive for institutional investment managers. 

## V. Focus on value added

1. Expected utility objective Æ high residual risks. The root cause is our evenhanded treatment of benchmark and active risk. However, managers are much more adverse to the risk of deviation from the benchmark than they are adverse to the risk of the benchmark. 

2. A new objective that splits risk and return into three parts: 

Intrinsic, $f _ { B } - \lambda _ { T } \bullet \sigma _ { B } ^ { 2 }$ . This component arises from the risk and return of the benchmark. It is not under the manager’s control. λ is aversion to total risk. 

Timing, $\beta _ { P A } \bullet \Delta f _ { B } - \lambda _ { B T } \bullet \beta _ { P A } ^ { \quad 2 } \bullet \sigma _ { B } ^ { 2 }$ . This is the contribution from timing the benchmark. It is governed by the manager’s active beta. Risk aversion $\lambda _ { \mathrm { B T } }$ to the risk caused by benchmark timing. 

Residual, $\alpha _ { \scriptscriptstyle P } - \lambda _ { \scriptscriptstyle R } \bullet \omega _ { { \scriptscriptstyle P } } ^ { 2 }$ . This is due to the manager’s residual position. Here we have an aversion to the residual risk. 

- The last two parts of the objective measure the manager’s ability to add value: 

$$
\mathbf {V A} = \left(\beta_ {P A} \bullet \Delta f _ {B} - \lambda_ {B T} \bullet \beta_ {P A} ^ {2} \bullet \sigma_ {B} ^ {2}\right) + \left(\alpha_ {P} - \lambda_ {R} \bullet \omega_ {P} ^ {2}\right) -- - - (4. 1 5)
$$

The value added is a risk-adjusted expected return that ignores any contribution of the benchmark to risk and expected return. 

The new objective function splits the value added into value added by benchmark timing and value added by stock selection. 

## Chapter 5 Residual Risk and Return: The Information Ratio

I. Introduction: The information ratio measures achievement ex-post and connotes opportunity ex-ante. Here, we are concerned about the trade off between residual risk and alpha. When portfolio beta is equal to one, residual risk and active risk coincide. 

II. The definition of Alpha 

1. Look-forward (ex-ante), alpha is a forecast of residual return. Looking backward (ex-post), alpha is the average of the realized residual returns. 

2. $r _ { P } ( t ) = \alpha _ { P } + \beta _ { P } \bullet r _ { B } ( t ) + \varepsilon _ { P } ( t )$ --- (5.1) 

Where, $\mathbf { r } ^ { \bullet } \mathbf { s }$ are excess returns. The estimates of alpha and beta obtained from the regression are the realized or historical alpha and beta. The residual returns for portfolio P are: 

$\theta _ { P } ( t ) = \alpha _ { P } + \varepsilon _ { P } ( t )$ , where alpha is the average residual return and $\varepsilon ( \mathrm { t } )$ is the mean zero random component of residual return. 

3. Looking forward, alpha is a forecast of residual return. $ \alpha _ { n } = E ( \theta _ { n } )$ 

4. Alpha has the portfolio property since both residual returns and expectations have the portfolio property. 

$$
\alpha_ {P} = h _ {P} (1) \bullet \alpha_ {1} + h _ {P} (2) \bullet \alpha_ {2}
$$

5. By definition the benchmark portfolio will always have a residual return equal to zero; i.e. $\theta _ { \mathrm { B } } = 0$ with certainty. The alpha of the benchmark portfolio must be zero. Risk-free portfolio also has a zero residual return; so the alpha for cash is always equal to zero. Thus, any portfolio made up of mixture of the benchmark and cash will have a zero alpha. 

## III. Ex-post information ratio: A measure of achievement

1. An information ratio is a ratio of (annualized) residual return to (annualized) residual risk. 

2. A realized information ratio can (and frequently will) be negative. 

3. The ex-post information ratio is related to the t-statistic one obtains for the alpha in the regression (equation 5.1). If the data in the regression cover Y years, then the information ratio is approximately the alpha’s t-statistic divided by the square root of Y. 

## IV. Ex-ante information ratio: A measure of opportunity

1. The information ratio is the expected level of annual residual return per unit of annual residual risk. The more precise definition of the information ratio is the highest ratio of residual risk to residual standard deviation that the manager can obtain. 

2. Reasonable levels of ex-ante information ratios run from 0.5 to 1.0 

3. Given alpha and portfolio residual risk, ω, the information ratio for portfolio P is: $I R _ { _ P } = { \frac { \alpha _ { _ P } } { \omega _ { _ P } } }$ --- (5.5) 

4. Our personal “information ratio’ is maximum information ratio that we can attain over all portfolios: 

$$
I R = \operatorname{Max} \left\{I R _ {P} \mid P \right\}
$$

5. The information ratio is independent of the manager’s level of aggressiveness. But it does depend on the time horizon. Æ Information ratio increase with the square root of time. 

V. The Residual Frontier: The Manager’s Opportunity Set Æ the alpha versus residual risk (omega) tradeoffs. The residual frontier will describe the opportunities available to the active manager. The ex-ante information ratio determines the manager’s residual frontier. 

VI. The active management objective 

1. To Maximize the value added from residual return where value added is measured as: 

$V A [ P ] = \alpha _ { _ P } - \lambda _ { _ R } \bullet \omega _ { _ P } ^ { 2 }$ --(5.7) (ignoring benchmark timing here) 

Æ awards a credit for the expected residual return and a debit for residual risk. 

2. Value added is sometimes referred to as a certainty equivalent return. 

VII. Preferences meet opportunities: The information ratio describes the opportunities. The active manager should explore those opportunities and choose the portfolio that maximizes value added 

VIII. Aggressiveness, Opportunity, and residual risk aversion. 

1. Max 5.7, subject to 5.5 Æ the optimal level of residual risk must satisfy. $\omega ^ { * } = \frac { I R } { 2 \lambda }$ -- (5.9) Æ our desired level of residual risk will increase with our opportunities and decrease with our residual risk aversion. 

2. It is possible to use 5.9 to determine a reasonable level of residual risk aversion. 

$\lambda = \frac { I R } { 2 \omega }$ --- (5.10) 

## IX. Value added: risk-adjusted residual return

1. Combine 5.5, 5.7 and $5 . 9  V A ^ { ^ { * } } = V A [ \omega ^ { ^ { * } } ] = \frac { I R ^ { ^ { 2 } } } { 4 \lambda _ { _ R } } = \frac { \omega ^ { ^ { * } } \bullet I R } { 2 }$ Æ ability of the manager to add value increases as the square of the information ratio and decreases as the manager becomes more risk averse. 

X. The beta = 1 frontier 

How do our residual risk/return choices look in the total risk/total return picture? The portfolios we will select (in the absence of any benchmark timing) will lie along the beta = 1 frontier 

XI. Forecast alphas directly 

1. One way to get alpha is to start with expected returns and then go through the procedure described in chapter 4. 

2. Forecast alpha directly. 

Step 1: sort the assets into five bins: strong buy, buy, hold, sell and strong sell. Assign them respective alphas of 2%, 1%, 0%, -1% and -2% 

Step 2: find the benchmark average alpha. If it is zero, quit. 

Step 3: Modify the alphas by subtracting the benchmark average times the stock’s beta from the original alpha. 

These alphas will be benchmark-neutral. In the absence of constraints they should lead the manager to hold a portfolio with a beta of 1. More and more elaborate variations on this theme. For example, we could classify stocks into economic sectors and then sort them into strong buy, buy, hold, sell and strong sell bins. 

3. This example Æ first, we need not forecast alphas with laser-lie precision. The accuracy of a successful forecaster of alphas is apt to be fairly low. Any procedure that keeps the process simple and moving in the correct direction will probably compensate for losses in accuracy in the second and third decimal points. Second, although it may be difficult to forecast alphas correctly, it is not difficult to forecast alphas directly. 

## Chapter 6 The Fundamental Law of Active Management

I. The Fundament Law 

1. BR: the strategy’s breadth is defined as the number of independent forecasts of exceptional return we make per year and; 

2. IC: the manager’s information coefficient is measure of skill Æ the correlation of each forecast with the actual outcomes. We assume that IC is the same for all forecasts. 

3. The fundamental law – connects breadth and skill to the information ratio through the (approximately true) formula: 

$I R = I C \bullet { \sqrt { B R } }$ ---- (6.1) 

- The approximation ignores the benefits of reducing risk that our forecasts provide. For relatively low values of IC (below 0.1) this reduction in risk is extremely small. 

4. By 5.9 and $6 . 1  \ \omega ^ { * } = \frac { I R } { 2 \lambda } = \frac { I C ^ { \bullet } \sqrt { B R } } { 2 \lambda }$ 

- the desired level of aggressiveness will increase directly with the skill level and as the square root of the breadth. The breadth allows for diversification among the active bets so that overall level of aggressiveness, $\omega ^ { * }$ can increase. The skill increases the possibility of success; thus, we are willing to incur more risk since the gains appear to be larger. 

5. By 5.11 and $6 . 1  V A ^ { ^ { * } } = V A [ \omega ^ { ^ { * } } ] = \frac { I R ^ { ^ { 2 } } } { 4 \lambda _ { _ R } } = \frac { I C ^ { ^ { 2 } } \bullet B R } { 4 \lambda _ { _ R } }$ Æ value added by a strategy (the risk-adjusted return) will increase with the breadth and with the square of the skill level. 

6. The fundamental law is designed to give us insight into active management; it isn’t an operational tool. 

7. A manager needs to know the tradeoffs between increasing the breadth of the strategy, - by either covering more stocks or shortening the time horizons of the forecasts – and improving skill, IC. 

## II. Additivity - The fundamental law is additive in the square information ratio.

$$
I R ^ {2} = B R _ {1} \bullet I C _ {1} ^ {2} + B R _ {2} \bullet I C _ {2} ^ {2}
$$

- Can be applied to two different asset categories. 

- Can be applied to one asset category + market timing 

We can carry this notion to an international portfolio. The active return of an international portfolio comes from three main sources: active currency positions, active allocations across countries, and active allocations within country markets. 

The additivity holds across managers. In this case we have to assume that the allocation across the managers is the optimal. 

The law’s use in scaling alphas; i.e., making sure that forecasts of exceptional stock return are consistent with the manger’s information ratio. 

## III. Assumptions.

1. The forecasts should be independent. Æ Forecast #2 should not be based on a source of information that is correlated with the sources for forecast #1. 

In a situation where analysts provide recommendations on a firm-by-firm basis it is possible to check the level of dependence among these forecasts by first quantifying the recommendations and then regressing them against attributes of the firms. 

Analysts may like all the firms in a particular industry: their stock picks are actually a single industry be. 

All recommended stocks may have a high earnings yield: the analysts have made a single bet on earnings to price ratios. 

The same masking of dependence can occur over time. If you reassess your industry bets on the basis of new information each year, while rebalancing your portfolios monthly, you shouldn’t think that you make 12 industry bets per year: you just make the same bet 12 times. 

Suppose two sources of in have the same level of skill IC. If γ is the correlation between the two information sources, then the skill level of the combined sources, IC (com), will be: 

$$
I C (c o m) = I C \bullet \sqrt {\frac {2}{(1 + \gamma)}}
$$

2. The law is based on the assumption that each of the BR active bets has the same level of skill - In fact, the manager will have greater skills in one area than another. 

3. The strongest assumption behind the law is that the manager will accurately gauge the value of his information and build portfolios that use that information in an optimal way. 

IV. Tests: 

1. It is desirable to have some faith in the law’s ability to make reasonable predictions. When we impose institutional constraints limiting short sales, the realized information ratios drop slightly. 

V. You must play often and play well to win at the investment management game. 

## Part II Expected Returns and Valuation

## Chapter 7 Expected Returns and the Arbitrage Pricing Theory

I. Introduction 

1. The APT is a model of expected returns. 

The flexibility of the APT makes it inappropriate as a model for consensus expected returns, but an appropriate model for a manager’s expected returns. 

The APT is a source of information to the active manager. It should be flexible. If all active managers share the same information it would be worthless. 

2. We need to define a qualified model and find the correct set of factor forecasts. 

II. The easy part: finding a qualified model 

1. Among any group of N stocks there will be an efficient frontier for portfolios made up out of the N risky stocks. Portfolio Q (tangent portfolio) has the highest reward to risk ratio (Sharpe ratio). 

2. A factor model s qualified, if and only if portfolio Q is diversified with respect to that factor model. Diversified with respect to the factor model means that portfolio Q has minimum risk among all portfolios with the same factor exposures as portfolio Q. 

3. A frontier portfolio like Q should be highly diversified in the conventional sense of the world. Portfolio Q will contain all of the stocks, with no exceptionally large holdings. We want portfolio Q to be diversified with respect to the multiple-factor model. 

4. The BARRA model was constructed to help portfolio managers control risk, not to explain expected returns. 

However, it does attempt to capture those aspects of the market that cause some groups of stocks to behave differently than others. 

Well over 99% of the variance of highly diversified portfolios is captured by the factor component. 

5. Any factor model that is good at explaining the returns of a diversified portfolio should be (nearly) qualified as an APT model. 

The exact specification of the factor model may not be important in qualifying a model. What is important is that the model contains sufficient factors to capture movement in the important dimensions. 

## III. The Hard Part: Factor Forecasts

1. The simplest approach to forecasting factor returns is to calculate a history of factor returns and take their average. Æ We are implicitly assuming an element of stationarity in the market. The APT does not provide any guarantees here. However, there is hope. One of the non-APT reasons to focus on factors is the knowledge that the factor relationship is stable than the stock relationship. 

2. Most structure can be helpful in developing good forecasts. APT models can either be purely statistical or structural. The factors have some meaning in the structural model; they don’t in a purely statistical model. 

3. Factor forecasts are easier if there is some explicit link between the factors and our intuition. Æ suggests an opportunistic approach to building an APT model. 

4. We should take advantage of our conclusion that we can easily build qualified APT models. We should use factors that we have some ability to forecast. 

5. Factor forecasts are difficult. Structure should help. 

## IV. Applications: structural vs. statistical.

1. Structural model 1: given exposures, estimate factor returns: The BARRA model takes the factor exposures as given based on current characteristics of the stocks, such as their earnings yield and relative size. The factor returns are estimates. 

2. Structural model 2: given factor returns, estimate exposure: e.g. take the factor returns as the return on the value-weighted NYSE, gold, a government bond index, and a basket of foreign currencies. Set the exposure of each stock to the NYSE equal to 1. For the other factors, determine the past exposure of the stock to the factor returns by regressing the difference between the stock return and the NYSE return on the returns of the other factors. 

3. Structural model 3: combine structural models 1 and 2: start with some primitive factor definitions, estimate the stock’s factor exposure as in structural model 2, then attribute returns to the factors as in structural model 1. 

4. Statistical model 1: principal components analysis: 

Look at 50 stocks over 200 months. Calculate the 50 by 50 matrix of realized covariance between these stocks over the 200 months. 

- Do a principal component analysis of the covariance matrix. 

Typically, one will find that the first 20 components will explain 90% or more of the risk. Call these 20 principal component returns the factors. 

The analysis will tell us the exposures of the 50 stocks to the factors and give us the returns on those factors over the 200 months. 

- The factor returns will be uncorrelated. 

We can determine the exposures to the factors of stocks not included in the original group by regressing the returns of the new stocks on the returns to the factors. 

## 5. Statistical model 2: maximum likelihood factor analysis:

Look at 500 stocks over 60 months and 10 factors. Æ have $5 0 0 ^ { * } 6 0 = 3 0 0 0 0$ returns. There would be $5 0 0 ^ { * } 1 0 = 5 0 0 0$ exposures to estimate and $6 0 ^ { * } 1 0 = 6 0 0$ factor returns to estimate. 

## Chapter 8 Valuation in Theory

Active managers must believe their assessment of value is better than the market or consensus assessment. 

I. Risk adjusted expectations 

1. Introduce risk adjusted discount rate, by using CAPM or APT. And use usually expected cash flows in the nominator. Or, 

2. Introduce risk-adjusted expectations Æ risk-neutral pricing. 

$$
E ^ {*} [ c f (t) ] = E [ v (t) \bullet c f (t) ] = \sum_ {s} \pi (t, s) \bullet v (t, s) \bullet c f (t, s),
$$

Where v(t,s) is called ‘value multiples’, it is: 

- positive 

- with expected value one: $\mathrm { E } [ \mathrm { v ( t , s ) } ] = 1$ 

a function of the return to portfolio Q, and proportional to the total return on the portfolio S, the portfolio with minimum second moment of total return. 

3. The value multiples v(t,s) help define a new set of probabilities, $\pi * ( \mathrm { t } , \mathrm { s } ) = \pi$ $( \mathrm { t } , \mathrm { s } ) ^ { * } \mathrm { v } ( \mathrm { t } , \mathrm { s } ) .$ 

4. The role of covariance: 

$E ^ { ' } [ c f ( t ) ] = E [ \nu ( t ) ] + \mathrm { c o v } [ c f ( t ) , \nu ( t ) ] \to$ the covariance term will, in general, be negative. 

5. Value multiples modify the cash flows. The value multiples v(t,s) change the cash flows by amplifying some, if it>1, and reducing others, if v(t,s)<1. since ${ \displaystyle { \bf E } [ { \bf v ( t ) } ] = }$ 1, they are on average unbiased. 

II. Market-dependent valuation: both risk-free rate and the value multipliers, are marketdependent and not stock-dependent. 

E[R] = (1 + risk-free rate) – Cov(v, R) 

E*[R] = (1 + risk-free rate) = E[v*R] Æ expected excess return on all stocks is determined by their covariance with v. 

## Chapter 9 Valuation in Practice

I. Introduction 

1. The basic theory of corporate finance provides ground rules for acceptable valuation models. 

2. The standard model is Dividend Discount Model (DDM). DDMs are only as good as their growth forecasts. 

II. Modeling growth 

$$
1. \frac {d + p _ {1} - p _ {0}}{p _ {0}} = i _ {F} + r = \frac {d}{p _ {0}} + \xi = y,
$$

Where, r = the excess return 

ξ= the uncertain amount of capital appreciation. 

Let g = E(ξ) and f = E(r). Suppose the expected excess return f includes both consensus expected returns and alphas: $f _ { n } = \beta _ { n } \bullet f _ { B } + \alpha _ { n } $ 

$$
i _ {F} + \beta_ {n} \bullet f _ {B} + \alpha_ {n} = \frac {d _ {n}}{p _ {n}} + g _ {n} = y _ {n}
$$

$$
\rightarrow \alpha_ {n} = (\frac {d _ {n}}{p _ {n}} - i _ {F}) + (g _ {n} - \beta_ {n} \bullet f _ {B})\tag{9.19}
$$

Æ The most important insight we must keep in mind while using a DDM: The golden rule of DDM: g in, g out Æ each additional 1% of growth adds 1% to the alpha. The alphas that come out of the DDM are as good as (or as bad as) the growth estimates that go in. 

3. Implied growth rates: 

use 9.19, assume that the assets are fairly priced and determine the growth rates necessary to fairly price the assets: 

$$
- \quad g _ {n} ^ {*} = i _ {F} + \beta_ {n} \bullet f _ {B} - \frac {d _ {n}}{p _ {n}}
$$

The implied growth rate can identify companies priced with unrealistic growth prospects. 

## Part III Implementation

## Chapter 10 Forecasting

I. Introduction 

1. Active management is forecasting 

2. The unconditional or naïve forecast is the consensus expected return. The conditional or informed forecast is dependent on the info sources. Historical averages make poor unconditional forecasts. 

3. The refined forecast has the form volatility*IC*score. 

4. Forecasts of return have negligible effect on forecasts of risk. 

II. Naïve, raw, and refined forecasts 

1. The naïve forecast is the consensus expected return. It is the informationless forecast. The naïve forecast leads to the benchmark holdings. 

2. The raw forecast contains the active manager’s info in raw form: an earnings estimate, buy or sell recommendation, etc. It is not directly a forecast of exceptional return. 

3. The basic forecasting formula transforms raw forecasts into refined forecasts. 

$_ - E ( r \mid g ) = E ( r ) + C o \nu ( r , g ) \bullet V a r ^ { - 1 } ( g ) \bullet [ g - E ( g ) ]$ , where 

r = excess return vector (N assets); 

g = raw forecast vector (K forecasts) 

E(r) = naïve (consensus) forecast 

E(g) = expected forecast 

E(r|g) = informed expected return, conditional on g. 

## - Refined forecast = the change in expected return due to observing g:

$\phi = E ( r \mid g ) - E ( r ) = C o \nu ( r , g ) \bullet V a r ^ { - 1 } ( g ) \bullet [ g - E ( g ) ]$ , this is the exceptional return referred to in previous chapters. It can include both residual return forecasts and benchmark timing. And, given a benchmark portfolio B, the naïve (consensus) forecast is: $\operatorname { E } ( { \mathrm { r } } ) = \beta \bullet \mu _ { B }$ 

## III. Refining raw info: one asset and one forecast

1. Assume: $r = 1 . 5 + \theta _ { 1 } + \theta _ { 2 } + . . . + \theta _ { 8 1 }$ , where theta is binary: -1 or 1 with probability ½. They capture the uncertain component of the returns. Each theta has mean 0 and variance 1. 

2. Assume our forecast: $g = 2 + \theta _ { 1 } + \theta _ { 2 } + \theta _ { 3 } + \eta _ { 1 } + . . . + \eta _ { 1 3 }$ . The forecast is a combination of useful and useless info. Thetas are bits of signal and $\eta \mathrm { s }$ are bits of noise. Æ 

3. $I C = C o r r ( g , r ) = C o \nu ( r , g ) / [ s t d ( r ) s t d ( g ) ] = 3 / ( 9 ^ { * } 4 ) { = } 0 . 8 3 3 .$ 

4. $\phi = S T D ( r ) \bullet c o r r ( r , g ) \bullet \left[ { \frac { g - E ( g ) } { S T D ( g ) } } \right]$ , we call the last term as score or zscore. 

## IV. The forecasting rule of thumb

Refined forecast = Volatility * IC * Score 

## V. Refining forecasts: one asset and two forecasts

$\phi = S T D ( r ) \bullet I C _ { g } ^ { ^ { \ast } } \bullet z _ { g } + S T D ( r ) \bullet I C _ { g } ^ { ^ { \ast } } \bullet z _ { g } ,$ , where ICs take into account the correlation between the forecasts. 

- A good forecaster has an IC of 0.05, a great forecaster has an $\mathrm { I C } = 0 . 1$ , and a world class forecaster has an $\mathrm { I C } = 0 . 1 5$ . An IC higher than 0.2 usually signals a faulty backtest or imminent investigation for insider trading. 

## VI. Forecasting and risk.

1. Forecasts of returns have a negligible effect on forecasts of volatility and correlation. The little effect there is has nothing to do with the forecast and everything to do with the skill of the forecaster. Æ We can concentrate on the expected return part of the problem and not worry about the risk part. 

2. Let $\sigma _ { P R I O R }$ and $\sigma _ { P O S T }$ be estimates of volatility without forecast info and with forecast info. The formula relating these is: 

$\sigma _ { { _ { P O S T } } } = \sigma _ { { _ { P R I O R } } } \bullet \left[ 1 - I C ^ { 2 } \right] ^ { 1 / 2 }$ (it is derived from conditional variance formula). When IC is small, having info has very little effect on the volatility forecasts. 

## Chapter 11 Information Analysis

VII. Introduction 

1. Information analysis begins by transforming information into something concrete: investment portfolios. 

2. Information analysis is not concerned with the intuition or process used to generate stock recommendations, only with the recommendations themselves. 

3. Information analysis occurs in the investment process before backtesting. Information analysis looks at the unfettered value of signals. Backtesting looks not only at information content, but also at turnover, tradability, and transactions costs. Information analysis is a two-step process. 

Step 1 is to turn information into portfolios. 

Step 2 is to analyze the performance of those portfolios. 

## VIII. Information and active management

1. Active managers use information to predict the future exceptional return on a group of stocks. The emphasis is on predicting alpha, or residual return: beta adjusted return relative to a benchmark. 

2. So, when we talk about information in the context of active management, we are really talking about alpha predictors. Information analysis is an effort to find the signal-to-noise ratio. 

3. We can classify information along the following dimensions: 

- Primary or processed 

- Judgmental or impartial 

- Ordinal or cardinal 

- Historical, contemporary, or forecast 

## IX. Information analysis: step 1: information into portfolios.

1. As a general comment, the investment time period should match the information time period. Portfolios based quarterly information – information which changes quarterly and influences quarterly returns – should be regenerated each quarter. 

2. Here are six possibilities. Using book-to-price ratios as an example: 

Procedure 1: with buy and sell recommendations (rank stocks by b/p, put the top half on the buy list and the bottom half on the sell list) Æ we could equal (or value) weight the buy group and the sell group. 

Procedure 2: with scores (rank stocks into several groups) Æ we could build a portfolio for each score by equal (or value) weighting within each score category. 

Procedure 3: with straight alphas we could split the stocks into two groups: one group with higher than average alphas and one with lower than average alphas. Then we can weight the stocks in each group by how far their alpha exceeds (or lies below) the average. One way to generate alphas from b/p is to assume that they are linearly related to the b/p. So we can weight each asset in our buy and sell list by how far its b/p lies above or below the average. This is an elaboration of procedure 1. 

Procedure 4: with straight alphas we could rank the assets according to alpha, and then group the assets into quintiles and then equal (or value) weight within each groups. This is an elaboration of procedure 2 

Procedure 5: with any numerical score we can build a factor portfolio that bets on the prediction and does not make a market bet. The factor portfolio consists of a long portfolio and a short portfolio. The long and short portfolios have equal value and equal beta, but the long portfolio will have a unit bet on the prediction, relative to the short portfolio. Given these constraints, the long portfolio will tract the short portfolio as closely as possible. For b/p data, we can build long and short portfolios with equal value and beta, with the long portfolio exhibiting a b/p one standard deviation above that of the short portfolio, and designed so that the long portfolio will track the short portfolio as closely as possible. 

Procedure 6: with any numerical score we could build a factor portfolio, consisting of a long and a short portfolio, designed so that the long and short portfolios are matched on a set of pre-specified control variables. For example, we could make sure the long and short portfolios match on industry, sector, or smallcap stock exposures. This is a more elaborate form of procedure 5, where we only controlled for beta (as a measure of exposure to market risk). 

3. While procedure 5 and 6 are more elaborate, they are also more precise in isolating the information contained in the data. These procedures build portfolios based solely on new information in the data, controlling for other important factors in the market. We recommend Procedure 5 or 6 as the best approach for analyzing the information contained in any numerical scores. 

## X. Information analysis: step 2: performance evaluation

1. t-statistics, information ratio, and information coefficients Regress the excess portfolio returns against the excess benchmark returns: 

$$
r _ {P} (t) = \alpha_ {P} + \beta_ {P} \bullet r _ {B} (t) + \varepsilon_ {P} (t)
$$

2. The information ratio is the best single statistic to capture the potential for value added from active management. The t is the ratio of alpha to its standard error. The information ratio is the ratio of annual alpha to its annual risk. 

3. If we observe returns over a period of T years, the information ratio is approximately the t divided by the square root of the number of years of observations: 

$$
I R \approx \frac {t - s t a t}{\sqrt {T}}
$$

- the relationship becomes more exact as the number of observations increases. 

The t measures the statistical significance of the return; the information ratio captures the risk-reward tradeoff of the strategy and the manager’s value added. An information ratio of 0.5 observed over five years may be statistically more significantly than an information ratio of 0.5 observed over one year, but their value added will be equal. 

The distinction between t and information ratio arises because we define value added based on risk over a particular horizon, in this case one year. 

4. Information coefficient: in the context of information analysis, it is the correlation between our data and realized alpha. 

## XI. Advanced topics in performance analysis:

1. Portfolio turnover: given transaction costs, turnover will directly affect performance. Turnover becomes important as we move from information analysis to backtesting and development of investable strategies. 

2. The maximum information ratio should be achieved when the portfolio holding period matches the information horizon. We can also investigate the importance of controlling for other variables: industries, size, etc. We can construct portfolios with different controls, and analyze the performance in each case. 

XII. Four guidelines can help keep information analysis from turning into data mining: intuition, restraint, sensibility, and out-of-sample testing 

1. Intuition must guide the search for information before the backtest begins. Intuition should not be driven strictly by data. Ideally, it should arise from a general understanding of the forces governing investment returns and the economy as a whole. 

2. Restraint should govern the backtesting process. In principle, researchers should map out possible information variations of before the testing begins. 

3. Performance should be sensible. The information deserving most scrutiny is that which appears to perform too well. Only about 10% of observed realized information ratios lie above 1. 

4. Out-of-sample testing can serve as a quantitative check on data mining. 

## Chapter 12 Portfolio Construction

## I. Introduction

1. Implementation includes both portfolio construction and trading. This chapter will take a manager’s investment constraints (e.g., no short sales) as given and build the best possible portfolio subject to those limitations. It will assume the standard objective: maximizing active returns minus an active risk penalty. 

2. Portfolio construction requires several inputs: the current portfolio, alphas, covariance estimates, transactions costs estimates, and an active risk aversion. Of these inputs, we can measure only the current portfolio with near certainty. 

## II. Alphas and portfolio construction

1. We can always replace a very complicated portfolio construction procedure that leads to active holdings, $h _ { P A } ^ { * }$ , active risk, $\psi _ { P } ^ { * }$ , and an ex-ante information ratio, IR, by a direct, unconstrained mean-variance optimization using a modified set of alphas and the appropriate level of risk aversion (Here we are explicitly focusing portfolio construction on active return and active risk, instead of residual return and risk. Without benchmark timing these perspectives are identical). The 

modified alphas are: $\alpha ^ { \prime } = \left( \frac { I R } { \psi _ { P } ^ { * } } \right) \bullet V \bullet h _ { P A } ^ { * }$ 

and the appropriate active risk aversion is: $\lambda _ { _ A } ^ { ^ { \prime } } = \frac { I R } { 2 \bullet \psi _ { _ P } ^ { ^ { \ast } } }$ 

## III.Alpha analysis

Here are some procedures for refining alphas that can simplify the implementation procedure and explicitly link our refinement in the alphas to the desired properties of the resulting portfolios: 

1. Benchmark and cash neutral alphas. 

The first and simplest refinement is to make the alphas benchmark neutral. By definition, the benchmark portfolio has zero alpha, though the benchmark may experience exceptional return. Setting the benchmark alpha to zero insures that the alphas are benchmark neutral, and avoids benchmark timing. 

We may also want to make the alphas cash neutral; i.e., the alphas will not lead to any active cash position. It is possible to make the alphas both cash and benchmark neutral. 

- Table 12.1 and 12.2: the benchmark alpha is 1.6 basis points, subtracting $\beta _ { n } \bullet \alpha _ { B }$ from each modified alpha Æ the alpha of the benchmark = 0. 

<table><tr><td>Stock</td><td>Index weight</td><td>modified alpha</td><td>beta</td><td>weight*alpha</td><td>beta*benchmark alpha</td><td>modified alpha - beta*benchmark alpha</td><td>weight*new alpha</td></tr><tr><td>1</td><td>2.28%</td><td>-1.14%</td><td>1.21</td><td>-0.026%</td><td>0.019%</td><td>-1.16%</td><td>-0.026%</td></tr><tr><td>2</td><td>4.68%</td><td>0.30%</td><td>0.96</td><td>0.014%</td><td>0.015%</td><td>0.28%</td><td>0.013%</td></tr><tr><td>3</td><td>6.37%</td><td>0.11%</td><td>0.46</td><td>0.007%</td><td>0.007%</td><td>0.10%</td><td>0.007%</td></tr><tr><td>4</td><td>3.84%</td><td>-0.78%</td><td>0.96</td><td>-0.030%</td><td>0.015%</td><td>-0.80%</td><td>-0.031%</td></tr><tr><td>5</td><td>3.94%</td><td>0.60%</td><td>1.23</td><td>0.024%</td><td>0.019%</td><td>0.58%</td><td>0.023%</td></tr><tr><td>6</td><td>5.25%</td><td>0.22%</td><td>1.13</td><td>0.012%</td><td>0.018%</td><td>0.20%</td><td>0.011%</td></tr><tr><td>7</td><td>4.32%</td><td>-0.65%</td><td>1.09</td><td>-0.028%</td><td>0.017%</td><td>-0.67%</td><td>-0.029%</td></tr><tr><td>8</td><td>3.72%</td><td>0.14%</td><td>0.6</td><td>0.005%</td><td>0.009%</td><td>0.13%</td><td>0.005%</td></tr><tr><td>9</td><td>5.60%</td><td>-0.19%</td><td>0.46</td><td>-0.011%</td><td>0.007%</td><td>-0.20%</td><td>-0.011%</td></tr><tr><td>10</td><td>7.84%</td><td>-1.10%</td><td>1.3</td><td>-0.086%</td><td>0.020%</td><td>-1.12%</td><td>-0.088%</td></tr><tr><td>11</td><td>2.96%</td><td>-0.52%</td><td>0.9</td><td>-0.015%</td><td>0.014%</td><td>-0.53%</td><td>-0.016%</td></tr><tr><td>12</td><td>4.62%</td><td>-0.51%</td><td>0.64</td><td>-0.024%</td><td>0.010%</td><td>-0.52%</td><td>-0.024%</td></tr><tr><td>13</td><td>6.11%</td><td>0.01%</td><td>1.18</td><td>0.001%</td><td>0.019%</td><td>-0.01%</td><td>-0.001%</td></tr><tr><td>14</td><td>4.63%</td><td>0.66%</td><td>1.13</td><td>0.031%</td><td>0.018%</td><td>0.64%</td><td>0.030%</td></tr><tr><td>15</td><td>4.47%</td><td>0.14%</td><td>1.06</td><td>0.006%</td><td>0.017%</td><td>0.12%</td><td>0.006%</td></tr><tr><td>16</td><td>3.98%</td><td>0.20%</td><td>1.06</td><td>0.008%</td><td>0.017%</td><td>0.18%</td><td>0.007%</td></tr><tr><td>17</td><td>9.23%</td><td>0.91%</td><td>0.74</td><td>0.084%</td><td>0.012%</td><td>0.90%</td><td>0.083%</td></tr><tr><td>18</td><td>7.07%</td><td>0.12%</td><td>0.94</td><td>0.008%</td><td>0.015%</td><td>0.11%</td><td>0.007%</td></tr><tr><td>19</td><td>4.92%</td><td>0.44%</td><td>1</td><td>0.022%</td><td>0.016%</td><td>0.42%</td><td>0.021%</td></tr><tr><td>20</td><td>4.17%</td><td>0.35%</td><td>1.05</td><td>0.015%</td><td>0.016%</td><td>0.33%</td><td>0.014%</td></tr><tr><td colspan="4">Benchmark alpha=</td><td>0.016%</td><td></td><td></td><td></td></tr><tr><td colspan="7">new benchmark alpha=</td><td>0.001%</td></tr></table>

## 2. Scale the alphas

Alpha has a natural structure: Alpha = IC*volatility*score. We expect the information coefficient (IC) and residual risk (volatility) for a set of alphas to be approximately constant, with the score having mean zero and standard deviation one across the set. Hence, the alphas should have mean zero and standard deviation, or scale, equal to IC*volatility. 

3. Trim alpha outliers 

Closely examine all stocks with alphas greater in magnitude than, say, three times the scale of the alphas 

A detailed analysis may show that some of these alphas depend upon questionable data and should be ignored (set to zero), while others may appear genuine. Pull in these remaining genuine alphas to three times scale in magnitude. 

A more extreme approach to trimming alphas forces them into a normal distribution with benchmark alpha equal to zero and the required scale factor. Such approaches are extreme because they typically utilize only the ranking information in the alphas and ignore the size of the alphas. After such a transformation, you must recheck benchmark neutrality and scaling. 

## 4. Risk factor neutral alphas.

The multiple-factor approach to portfolio analysis separates return along several dimensions. A manager can identify each of those dimensions as either a source of risk or as a source of value added. By this definition, he does not have any ability to forecast the risk factors. He should neutralize his alphas against the risk factors. 

The neutralized alphas will only include info on the factors he can forecast, plus specific asset info. Once neutralized, the alphas of the risk factors will be zero. 

E.g., to make alphas industry neutral Æ calculate the (cap weighted) alpha for each industry. Then subtract the industry average alpha from each alpha in that industry. 

## IV. Transactions costs

1. When we consider only alphas and active risk in the portfolio construction process, we can offset any problem in setting the scale of the alphas by increasing or decreasing the active risk aversion. Find the correct tradeoff between alpha and active risk is a one-dimensional problem. Transaction costs make this a two-dimensional problem. 

2. We must amortize the transactions costs to compare them to the annual rate of gain from the alpha and the annual rate of loss from the active risk. The rate of amortization will depend on the anticipated holding period. The annualized transactions cost is the round-trip cost divided by the holding period in years. 

## V. Portfolio revisions

1. The returns themselves become noiser at shorter horizons. Rebalancing at very short horizons would involve frequent reactions to noise, not signal. But the transactions costs stay the same, whether we are reacting to signal or noise. 

2. We can capture the impact of new info, and decide whether to trade, by comparing the marginal contribution to value added for stock n, MCVAn, to the transactions costs. The marginal contribution to value added show how value added, as measure by risk-adjusted alpha, changes as the holding of the stock is increased with an offsetting decrease in the cash position. 

- As our holding in stock n increase, $\alpha _ { n }$ measures the effect on portfolio alpha. 

The change in value added also depends upon the marginal impact on active risk of adding more of stock n, MCARn, which measures the rate at which active risk changes as we add more of stock n. 

$$
M C V A _ {n} = \alpha_ {n} - 2 \bullet \lambda_ {A} \bullet \psi_ {P} \bullet M C A R _ {n}
$$

- Let $\mathrm { P C } _ { \mathrm { n } }$ be the purchase cost and $\mathrm { { S C } _ { n } }$ the sales cost for stock n. Then when $- S C { _ n } \leq M C V A { _ n } \leq P C { _ n }$ , we should not make a trade. $ \mathrm { a }$ band around the alpha for each stock 

$$
- 2 \bullet \lambda_ {A} \bullet \psi_ {P} \bullet M C A R _ {n} - S C _ {n} \leq \alpha_ {n} \leq P C + 2 \bullet \lambda_ {A} \bullet \psi_ {P} \bullet M C A R _ {n}
$$

VI. Techniques for portfolio construction: $\alpha _ { _ P } - \lambda _ { _ A } \bullet \psi _ { _ P } ^ { 2 } - T C$ 

1. Screens 

- Step1. Rank the stocks by alpha. 

- Step 2. Choose the first 50 stocks, say. 

- Step 3. Equal weight (or cap weight) the stocks. 

The screen is robust – it depends solely on raking. Wild estimates of positive or negative alphas will not alter the result. 

But screens ignore all info in the alphas apart from the rankings. They do not protect against biases in the alphas. If all of the utility stocks happen to be low in the alpha rankings, the portfolio will not include any utility stocks. 

2. Stratification – glorified screening. 

The key is splitting the list of followed stocks into categories. These categories are generally exclusive. E.g. 

- Step 1: classify stocks into ten economic sectors 

- Step 2: within each sector, classify stocks by size: big, medium, and small. 

Step 3: within each category (30), rank the stocks by alpha, place them into buy, hold and sell groups. Weight the stocks so that the portfolio’s weight in each category matches the benchmark’s weight in those categories. 

Stratification ignores some info and does not consider slightly overweighting one category and under-weighting another. Often, little substantive research underlies the selection of the categories, so risk control is rudimentary. 

## 3. Linear programming – space-age stratification

It characterizes stocks along dimensions of risk, e.g., industry, size, volatility, beta. 

It does not require that these dimensions distinctly and exclusively partition the stocks. We can characterize stocks along all of these dimensions. The linear program will then attempt to build portfolios that are reasonably close to the benchmark portfolio in all of the dimensions used for risk control. 

The linear program takes all of the info about alpha into account and controls risk by keeping the characteristics of the portfolio close to the characteristics of the benchmark. But, 

It has difficulty producing portfolios with a pre-specified number of stocks. Also, the risk-control characteristics should not work at cross purposes with the alphas. E.g., if the alphas tell you to shade the portfolio toward smaller stocks at some times and toward larger stocks at other times, you should not control risk on the size dimension. 

4. quadratic programming (QP) – the ultimate in portfolio construction 

It explicitly considers each of the three elements in our figure of merit: alpha, risk, and transactions costs. 

Since a QP is a glorified linear program, it can include all the constraints and limitations one finds in a linear program. 

However, the QP requires a great many more inputs than the other portfolio construction techniques. More inputs means more noise. 

VII. Summary: in the real world, alpha inputs are often unrealistic and biased. Covariances and transactions costs are measured imperfectly. The standard reaction is to compensate for flawed inputs by regulating the outputs of the portfolio construction process: placing limits on active stock positions, limiting turnover, and constraining holdings in certain categories of stocks to match the benchmark holdings. 

## Chapter 13 Transactions Costs, Turnover, and Trading

I. Introduction 

1. Transactions costs include commissions, the bid/ask spread, and market impact. 

Commissions are the charge per share paid to the broker for executing the trade. These tend to be the smallest component of the transactions costs and the easiest to measure. 

- The bid/ask spread is approximately the cost of trading one share of stock. 

Market impact is the cost of trading additional shares of stock. It is hard to measure because it is the cost of trading many shares relative to the cost of trading one share. Every trade alters the market. 

2. A strategic question – how we can reduce transactions costs while preserving as much of the strategy’s value added as possible. We can attack this in two ways: reducing transactions costs by reducing turnover while retaining as much as the value added as possible, and reducing transactions costs through optimal trading. 

3. Transactions costs increase with trade size and the desire for quick execution, which help identify the manager as an informed trader, and require increased inventory risk by the liquidity provider. 

4. Transactions costs are difficult to measure. 

5. Transactions costs lower value added, but you can often achieve at least 75% of the value added with only half the turnover. 

6. Trading is itself a portfolio optimization problem, distinct form the portfolio construction problem. Optimal trading can lower transactions costs, though at the expense of additional short-term risk. 

## II. Market microstructure

Several considerations determine what price the liquidity supplier will charge. 

1. The liquidity supplier would like to know why the manger is trading. He could only guess at the value of the manager’s info by the volume and urgency of the proposed trade. 

2. Inventory risk: When the liquidity supplier trades, his goal is to hold the inventory only until an opposing trade comes along. 

## III. Analyzing and estimating transactions costs

1. The theory of market microstructure says that transactions costs can depend on manager style, with trading speed mainly accounting for differences in manager style. Managers who trade more aggressively should experience higher transactions costs. 

2. Wayne Wagner (1993) finds that the most aggressive info trader was able to realize very large short-term returns, but they were offset by very large transactions costs. The slowest traders often even experienced negative short-term returns, but with small or even negative transactions costs. 

3. Estimation of expected transactions costs requires measurement and analysis of past transactions costs. The best place to start is with the manager’s past record of transactions, and the powerful ‘implementation short-fall’ approach to measuring the overall cost of trading. The idea is to compare the returns to a paper portfolio to the returns to the actual portfolio. Differences in returns to these two portfolios will arise due to commissions, the bid/ask spread, and market impact, as well as to the opportunity costs of trades which were never executed. E.g., some trades never execute because the trader keeps waiting for a good price while the stock keeps moving away from him. Wayne Wagner has estimated that such opportunity costs often dominate all transactions costs. 

4. Most services don’t use the implementation shortfall approach, because it involves considerable recordkeeping. They use more simple methods like comparing execution prices to the volume weighted average price (VWAP) over the day. Such as approach measures market impact extremely crudely and misses opportunity costs completely. 

5. The most difficult approach is to directly research market tick-by-tick data. Whatever the data analyzed, the goal is an estimate of expected transactions costs for each stock, based on manager style, for the possible range of trade volumes. 

6. The inventory risk model: 

Given a proposed trade of size, $\mathrm { V _ { t r a d e } }$ , the estimated time before an opposing trade appears to clear out the liquidity supplier’s net inventory in the stock is: 

$\tau _ { c l e a r } = \frac { V _ { t r a d e } } { V _ { d a i l y } } , \mathrm { V _ { d a i l y } }$ is the average daily volume in the stock. 

- Inventory risk: $\sigma _ { i n \nu e n t o r y } = \sigma \bullet \sqrt { \frac { \tau _ { c l e a r } } { 2 5 0 } }$ , where $\sigma$ is the stock’s annual volatility. 

- Last step assumes the liquidity supplier demands a return proportional to this inventory risk: $\frac { \Delta P } { P } = c \bullet \sigma _ { i n \nu e n t o r y }$ , where c is the risk/return tradeoff 

- Combine the above three equations together: 

Transactions costs = commissions + spread/price + $. c _ { t c } \sqrt { \frac { V _ { t r a d e } } { V _ { d a i l y } } }$ , where c includes the stock’s volatility, a risk/return tradeoff, and the conversion from annual to daily unit 

IV. Turnover, transactions costs, and value added 

1. $V A _ { P } = \alpha _ { P } - \lambda _ { A } \bullet \psi _ { P } ^ { 2 }$ , suppose the manager plans to move from portfolio I to portfolio Q. 

2. Purchase turnover: $T O _ { P } = \sum _ { n } M a x [ 0 , h _ { P , n } ^ { * } - h _ { P , n } ]$ 

3. sales turnover: $T O _ { s } = \sum _ { n } M a x [ 0 , h _ { P , n } - h _ { P , n } ^ { * } ]$ 

4. TO = min {TOp, TOs} 

5. A lower bound: $V A ( T O ) \geq V A _ { I } + \Delta V A _ { \varrho } [ 2 ( { \frac { T O } { T O _ { \varrho } } } ) - ( { \frac { T O } { T O _ { \varrho } } } ) ^ { 2 } ]$ 

6. You can achieve at least 75% of the incremental value added with 50% of the turnover. 

7. Transactions costs: Max: $\mathrm { V A p - T C ^ { * } T O _ { p }  }$ when TC = slope of value added/turnover frontier (VA over TO), Æ optimal. 

8. Implied transactions costs: we can fix the level of turnover at the required level, $\mathrm { T O } _ { \mathrm { R } }$ , and then find the slope, SLOPE(TO<sub>R</sub>), of the frontier at $\mathrm { T O } _ { \mathrm { R } } . $ implied transactions costs = the slope. 

9. Reasonable levels of round trip costs (2%) do not call for large amounts of turnover and that very low or high restrictions on turnover correspond to unrealistic levels of transactions costs. 

10. It is good news for the portfolio manager if the transactions costs differ. Differences in transactions costs further enhance our ability to discriminate – our ability to discriminate adds value. 

## Chapter 14 Performance Analysis

I. Introduction 

1. The goal of performance analysis is to distinguish skilled from unskilled investment mangers. Simple cross-sectional comparisons of returns can distinguish winners from losers. Time series analysis of the returns can start to separate skill from luck, by measuring return and risk. Time series analysis of returns and portfolio holdings can go the farthest toward analyzing where the manager has skill: what bets have paid off and what bets haven’t. The manager’s skill ex-post should lie along dimensions promised ex-ante. 

2. For owners of funds, some assumptions: 

- skillful active management is possible; 

- skill is an inherent quality that persists over time; 

- that statistically abnormal returns are a measure of skill; 

Skillful managers identified in one period will show up as skillful in the next period. 

3. For fund managers: performance analysis can be used to monitor and improve the investment process. Performance analysis can, ex-post, help the manager avoid two major pitfalls in implementing an active strategy. 

The first is incidental risk: managers may like growth stocks without being aware that growth stocks are concentrated in certain industry groups and concentrated in the group of stocks with higher volatility. 

The second pitfall is incremental decision making. A portfolio based on a sequence of individual asset decisions, each of them wise on the surface, can soon become much more risky than the portfolio manager intended. 

4. Portfolio based performance analysis is the most sophisticated approach to distinguishing skill and luck along many different dimensions. 

## II. Skill and Luck

1. Efficient markets hypothesis suggests that active managers have no skill. 

- Semi-strong form suggests active management skill is really insider trading. 

Week form rules out technical analysis as skilled active management, but would allow for skillful active management based on fundamental and economic analysis. 

2. Recent studies have shown that the average manager matches the benchmark net of fees, that top managers do have statistically significant skill, and that positive performance may persist. 

## III. Defining Returns

1. Compound total return: $R _ { P } ( 1 , T ) = \prod _ { t = 1 } ^ { t = T } R _ { P } ( t )$ 

2. Geometric average return: $( 1 + g _ { _ P } ) ^ { T } = \prod _ { t = 1 } ^ { t = T } R _ { _ P } ( t )$ 

3. Average log return: $z _ { P } = ( \frac { 1 } { T } ) \bullet \sum _ { t = 1 } ^ { t = T } \ln [ R ( t ) ]$ 

4. Arithmetic average return: $1 + a _ { _ P } = ( \frac { 1 } { T } ) \bullet \sum _ { t = 1 } ^ { t = T } R ( t )$ 

5. Geometric average return is compounded annually, while the average log return is compounded continuously. It is always true that $z _ { P } \le g _ { P } \le a _ { P }$ This does not necessarily say that one measure is better to use than the other. It does indicate that consistency is important to make sure we are not comparing apples and oranges. 

## IV. Cross-sectional Comparisons

Usually contain survivorship bias, which is increasingly severe the longer the horizon. 

It doesn’t adjust for risk. The top performer may have taken large risks and been lucky. 

## V. Returns-based performance analysis: basic

## 1. Returns regression:

Basic returns-based performance analysis according to Jensen (1986) involves regressing the time series of portfolio excess returns against benchmark excess returns (separates returns into systematic and residual components, and then analyzes the statistical significance of the residual component). 

$r _ { P } ( t ) = \alpha _ { P } + \beta _ { P } \bullet r _ { B } ( t ) + \varepsilon _ { P } ( t )$ 

- The regression divides the portfolio’s excess return into the benchmark component and the residual component. $\theta _ { P } ( t ) = \alpha _ { P } + \varepsilon _ { P } ( t )$ 

- The t-statistic is approximately: $t _ { r } = \left( \frac { \alpha _ { _ P } } { \omega _ { _ P } } \right) \bullet \sqrt { T }$ 

where $\alpha _ { P }$ and $\omega _ { P }$ are not annualized, and T is the number of observations (periods). The t measures where alpha differs significantly from zero. 

2. The t-statistic measures the statistical significance of the return and skill. The information ratio measures the ratio of annual return to risk, and relates to investment value added. The information ratio measures realized value added, whether statistically significant or not. 

3. The basic alternative to the Jensen approach is to compare Sharpe ratio for the portfolio and the benchmark. A portfolio with: 

$$
\frac {r _ {P}}{\sigma_ {P}} > \frac {r _ {B}}{\sigma_ {B}}
$$

- We can analyze the statistical significance of this relationship: Assuming that the standard errors in our estimates of the means returns $r _ { P }$ and $\overline { { r } } _ { B }$ dominate the errors in our estimates of $\sigma _ { P }$ and $\sigma _ { B }$ , the standard error of each Sharpe ratio is approximately : $1 / \sqrt { N }$ 

- Hence, a statistically significant (95% confidence level) demonstration of skill occurs when: 

$$
\left(\frac {\overline {{r}} _ {P}}{\sigma_ {P}} - \frac {\overline {{r}} _ {B}}{\sigma_ {B}}\right) > 2 \sqrt {\frac {2}{N}}
$$

- Dybvig and Ross (1985) have shown that superior performance according to Sharpe implies positive Jensen alphas, but that positive Jensen alphas do not imply positive performance according to Sharpe. 

VI. Returns-based performance analysis: advanced: 

1. Bayesian correlation: allows us to use our prior knowledge about the distribution of alphas and betas across managers. See Vasicek (1973). 

2. Heteroskedasticity 

3. Autocorrelation. 

4. Benchmark timing: one financially based refinement to the regression model is a benchmark timing component. The expanded model is: 

$$
r _ {P} (t) = \alpha_ {P} + \beta_ {P} \bullet r _ {B} (t) + \gamma_ {P} \bullet M a x \{0, r _ {B} (t) \} + \varepsilon_ {P} (t)
$$

- The model includes a “down-market” beta, $\beta _ { P }$ , and an “up-market” beta, $\beta _ { P } + \gamma _ { P }$ . If $\gamma _ { { } _ { P } }$ is significantly positive, then we say there is evidence of timing skill; benchmark exposure is significantly different in up and down cases. 

5. Value added: use the concept of value added and ideas from the theory of valuation (Chapter 8). 

6. Style analysis: attempts to extract as much information as possible out of the time series of portfolio returns without requiring the portfolio holdings. Like the factor model approach, style analysis assumes that portfolio returns have the form: 

$$
r _ {P} (t) = \sum_ {j = 1} ^ {J} h _ {P j} \bullet r _ {j} (t) + u _ {P} (t)
$$

- The $r _ { j } ( t )$ are returns to J “styles,” the $h _ { P j }$ measure the portfolio’s holdings of those styles, and $u _ { P } ( t )$ is the “selection return,” the portion of the return which style cannot explain. 

Style analysis attributes returns to several style classes and giving managers credit only for the remaining selection returns. 

Here the styles typically allocate portfolio returns along the dimensions of value versus growth, large versus small cap, domestic versus international, and equities versus bonds. 

- We estimate holdings $h _ { P j }$ via a quadratic program: 

Minimize 

$$
\operatorname{Var} u _ {P} (t)
$$

$$
\text { s.t. } \sum_ {j = 1} ^ {J} h _ {P j} = 1, \text { and } h _ {P j} > = 0 \text { for   all } j.
$$

Style analysis requires only the time series of portfolio returns, and the returns to a set of style indices. The result is a top-down attribution of the portfolio returns into style and selection. 

## VII. Portfolio-based performance analysis.

1. Portfolio-based performance analysis is a bottom-up approach, attributing returns into many components based on the ex-ante portfolio holdings and then giving managers credit for returns along many of these components. 

2. In contrast to returns-based performance analysis, performance-based analysis schemes can attribute returns to several components of possible manager skill. 

3. The analysis proceeds in two steps: performance attribution and performance analysis. 

## VIII. Performance attribution

1. Performance attribution looks at portfolio returns over a single period and attributes them to factors. The underlying principle is the multiple-factor model: 

$$
r _ {P} (t) = \sum_ {j = 1} ^ {J} x _ {P j} (t) \bullet b _ {j} (t) + u _ {P} (t)
$$

- Examining returns ex-post, we know the portfolio’s exposure, $x _ { P j } ( t )$ , at the beginning of the period, as well as the portfolio’s realized return, $r _ { P } ( t )$ , and the estimated factor returns over the period. 

- The return attributed to factor j is: $r _ { P j } ( t ) = x _ { P j } ( t ) \bullet b _ { j } ( t )$ . The portfolio’s specific return is $u _ { P } ( t )$ 

2. We are free to choose factors as described in Chapter 3, and in fact we typically run performance attribution using the same risk model factors. However, we are not in principle limited to the same factors in our risk model. We want to choose some factors for risk control and others as sources of return. The risk control factors are typically industry or market factors. 

3. In building risk models we always use ex-ante factors based on information known at the beginning of the period. For return attribution we could also consider ex-post factors based on information known only at the end of the period. 

4. Beyond the manager’s returns attributed to factors will remain the specific return to the portfolio. A manager’s ability to pick individual stocks, after controlling for the factors, will appear in this term. 

5. We can apply performance attribution to total, active returns, and even active residual return. For active returns, the analysis is exactly the same, but we work with active portfolio holdings and returns; 

$$
r _ {P A} (t) = \sum_ {j = 1} ^ {J} x _ {P A j} (t) \bullet b _ {j} (t) + u _ {P A} (t) \tag {14.17}
$$

- To break down active returns into systematic and residual Æ 

$x _ { { P A R } , j } = x _ { { P A } , j } - \beta _ { { P A } } \bullet x _ { { B } , j }$ , where we simply subtract the active beta times the benchmark’s exposure from the active exposure, and residual holdings similarly as: 

$h _ { { P A R } , n } = h _ { { P A } , n } - \beta _ { { P A } } \bullet h _ { { B } , n }$ , substituting these into 14.17 and remember that 

$u _ { P A } = \sum _ { n } h _ { P A , n } \bullet u _ { n }$ , we find: 

$$
r _ {P A} (t) = \beta_ {P A} \bullet r _ {B} (t) + \sum_ {j = 1} ^ {J} x _ {P A R, j} (t) \bullet b _ {j} (t) + u _ {P A R} (t) - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 1 4. 2 0
$$

## IX. Performance analysis

1. Performance analysis begins with the attributed returns each period and analyzes the statistical significance and value added of the attributed return series. This analysis relies on t-statistic and information ratio to determine statistical significance and value added. 

2. Consider the attribution defined in 14.20, with active returns separated into systematic $( \beta _ { P A } \bullet r _ { B } ( t ) )$ and residual, and active residual returns further attributed to common factors( $\sum _ { j = 1 } ^ { J } x _ { P A R , j } ( t ) \bullet b _ { j } ( t ) )$ and specific returns $( u _ { P A R } ( t ) )$ . 

## Chapter 15 Benchmark Timing

I. Defining benchmark timing 

1. Benchmark timing is an active management decision to vary the managed portfolio’s beta with respect to the benchmark. If we believe that the benchmark will do better than usual, then beta is increased. 

2. In its purest sense we should think of benchmark timing as choosing the correct mixture of the benchmark portfolio and cash. This type of benchmark timing is akin to buying or selling futures contracts on the benchmark. 

3. Benchmark timing is not asset allocation. Asset allocation focuses on aggregate asset classes rather than specific individual stocks, bonds, etc. 

4. The process of selecting a target asset allocation is called strategic asset allocation. The variation in asset allocation around that target is called tactical asset allocation. We only address tactical asset allocation here in that the principles for active management in one equity market also apply to tactical asset allocation. 

5. Since $I R _ { { \scriptscriptstyle B T } } = I C _ { { \scriptscriptstyle B T } } \sqrt { B R }$ , an independent benchmark timing forecast every quarter only leads to a breadth of 4. To generate a benchmark timing information ratio of 0.5 requires an information coefficient of 0.25! The fundamental law captures exactly why most institutional managers focus on stock selection. 

6. Stock selection strategies can diversify bets cross-sectionally across many stocks. Benchmark timing strategies can only diversify serially, through frequent bets per year. Significant benchmark timing value added can only arise with multiple bets per year. 

## II. Futures versus stocks

Benchmark timing is choosing an active beta. We can implement benchmark timing with futures. When the benchmark has no closely associated futures contract, the potential for adding value through benchmark timing is very small. 

## III. Value added

1. $V A [ \beta _ { { } _ { P A } } \mid \Delta f _ { { } _ { B } } ] = \beta _ { { } _ { P A } } \bullet \Delta f _ { { } _ { B } } - \lambda _ { { } _ { B T } } \bullet \beta _ { { } _ { P A } } { } ^ { 2 } \bullet \sigma _ { { } _ { B } } ^ { 2 }$ --(15.3) 

Where beta is the portfolio’s active beta with respect to the benchmark. This is the decision variable. 

- The optimal level of active beta is determined by FOC of the previous equation. 

$\beta _ { P A } ^ { * } = \frac { \Delta f _ { B } } { 2 \bullet \lambda _ { B T } \bullet \sigma _ { B } ^ { 2 } }$ -- (15.4) 

2. If we look at forecast deviation $\Delta f _ { B }$ directly, we can greatly simplify matters: 

$\mathbf { \nabla } - \Delta f _ { _ B } = \sigma _ { _ B } \bullet I C \bullet S$ ---(15.6) 

where 

- IC = information coefficient, the correlation between our forecasts and subsequent exceptional benchmark returns that is a measure of forecasting skill. 

- S = score, a normalized signal with mean zero and standard deviation equal to one over time. 

- With a correlation of IC =0.1, you would expect to be correct 55% of the time. 

## IV. Forecasting Frequency

1. The volatility of the benchmark over any period t will be: 

$$
- \sigma_ {B} (t) = \sigma_ {B} / \sqrt {T}
$$

- Period by period, the forecasting rule of thumb still applies: 

$$
\Delta f _ {B} (t) = \sigma_ {B} (t) \bullet I C \bullet S (t) = \left[ \frac {\sigma_ {B} \bullet I C \bullet S (t)}{\sqrt {T}} \right]
$$

since we ultimately keep score on an annual basis, we must analyze the annual value added generated by these higher frequency forecast. It is the sum of value added each period. Æ 

$$
V A = \sum_ {t = 1} ^ {T} \beta_ {P A} (t) \bullet \Delta f _ {B} (t) - \lambda_ {B T} \bullet \sum_ {t = 1} ^ {T} \beta_ {P A} ^ {2} (t) \bullet \sigma_ {B} ^ {2} (t)
$$

## Chapter 16 Summary

## I. What we have covered

The active management framework begins with a benchmark portfolio, and defines exceptional returns relative to that benchmark. Active managers seek exceptional returns, at the cost of assuming risk relative to matching the benchmark return. 

- We measure value added as the risk adjusted exceptional return. 

The key characteristic measuring a manager’s ability to add value is the information ratio, the amount of additional exceptional return he can generate for each additional unit of risk. The information ratio is both a figure of merit and a budget constraint. A manager’s ability to add value is constrained by his information ratio. 

Given this framework, portfolio theory connects exceptional return forecasts – return forecasts which differ from consensus expected returns – with portfolios that differ from the benchmark. If a manager’s forecasts agree with the consensus, he will hold the benchmark. To the extent that his information ratio is positive, the manager will hold a portfolio that differs from the consensus. 

- The fundamental law – high information ratio require both skill and breadth. 

## II. Themes

First, active management is a process. Active management begins with raw info, refines it into forecast, and then optimally and efficiently constructs portfolios balancing those forecasts of return against risk. 

Second, active management is forecasting, and a key to active manager performance is superior info. Most of this book describes the machinery for processing this superior info into portfolios. 

Thirdly, active managers should forecast as often as possible. Given the realities of active management, the best hope for a large information ratio is to develop a small edge and bet very often. In this search for breadth, we also advocate including multiple sources of info: the more the better. 

III. What’s left? – What this book ultimately can’t help with, is the search for superior info. 