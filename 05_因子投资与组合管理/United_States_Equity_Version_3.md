

<!-- === Source: MinerU_markdown_United_States_Equity_Version_3_1_2122709305022066689.md (Page 1) === -->

United States Equity 

Version 3 (E3) 

BARRA makes no warranty, express or implied, regarding the United States Equity Risk Model or any results to be obtained from the use of the United States Equity Risk Model. BARRA EXPRESSLY DISCLAIMS ALL WARRANTIES, EXPRESS OR IMPLIED, REGARDING THE UNITED STATES EQUITY RISK MODEL, INCLUDING BUT NOT LIMITED TO ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE OR USE OR THEIR EQUIVALENTS UNDER THE LAWS OF ANY JURISDICTION. Although BARRA intends to obtain information and data from sources it considers to be reasonably reliable, the accuracy and completeness of such information and data are not guaranteed and BARRA will not be subject to liability for any errors or omissions therein. Accordingly, such information and data, the United States Equity Risk Model, and their output are not warranted to be free from error. BARRA does not warrant that the United States Equity Risk Model will be free from unauthorized hidden programs introduced into the United States Equity Risk Model without BARRA's knowledge. 

Copyright © BARRA, Inc. 1998. All rights reserved.
0111 O 02/98 

## Contents

About BARRA . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . A pioneer in risk management . . . . . . . . . . . . . . . . . . . . . . . 1   
Introduction. 3 In this handbook. 3 Further references 5 Books. 5   
Section I: Theory   
1. Why Risk is Important. 7 The goal of risk analysis. 8   
2. Defining Risk. 11 Some basic definitions. 11 Risk measurement 13 An example 13 Risk reduction through diversification 14 Drawbacks of simple risk calculations 16 Evolution of concepts 16   
3. Modeling and Forecasting Risk. 21 What are MFMs? 21 How do MFMs work? 21 Advantages of MFMs. 22 A simple MFM 23 Model mathematics 25 Risk prediction with MFMs 26 

4. Modern Portfolio Management and Risk 31
Portfolio management—two types 31
Passive management 31
Active management 32
Decomposing risk 34
Total Risk 34
Systematic-Residual Risk Decomposition 35
Active Risk Decomposition 36
Active Systematic-Active Residual Risk Decomposition 37
Summary of risk decomposition 38
Performance attribution 38
Summary 39

5. BARRA Multiple-Factor Modeling 41
Overview 41
Descriptor selection and testing 44
Descriptor standardization 44
Risk index formulation 45
Industry allocation 45
Factor return estimation 46
Covariance matrix calculation 46
Exponential weighting 47
Computing market volatility:
Extended GARCH models 48
Specific risk modeling 49
Overview 49
Methodology 50
Modeling the average level of specific risk 50
Modeling the relative level of specific risk 51
Estimating the scaling coefficients 52
Final specific risk forecast 52
Updating the model 52
Comparison of risk model features 53 

## Section II: US-E3 Model Details

6. Advantages of US-E3 Over US-E2 .... 55
Overview .... 55
Industries.... 56
Reclassification.... 56
Flexible industries.... 57
Increased size of the estimation universe.... 57
Risk indices.... 58
Size Nonlinearity factor.... 58
Leverage.... 58
Simpler volatility calculation.... 58
Elimination of US-E2's Labor Intensity and Foreign Income.... 59
Improved independence between risk indices.... 59
Risk forecasting.... 59
Improved GARCH model.... 59
Specific risk model.... 60
Model fit-related issues.... 60
Factor return estimation.... 60
Ongoing diagnostics.... 60
Scheduled refitting of model parameters.... 60
Asset class issues.... 61
REITs.... 61
Coming soon.... 61

7. The US-E3 Estimation Universe .... 63
Overview .... 63
Selection process .... 63
1. S&P 500 membership.... 64
2. Compustat data present.... 64
3. Capitalization.... 64
4. Minimum price.... 64
5. Industry fill-in.... 64
6. Grandfathering.... 65
Comparison with the US-E2 estimation universe.... 65 

8. US-E3 Risk Indices and Descriptors. 67
Differences between US-E2 and US-E3 risk indices. 67
General differences. 67
Specific differences. 67
Volatility. 67
Size. 68
Size Nonlinearity (US-E3). 68
Growth. 68
Financial Leverage (US-E2) and Leverage (US-E3). 69
Foreign Income (US-E2) and
Currency Sensitivity (US-E3). 69
Labor Intensity (US-E2). 69
US-E3 and US-E2 risk indices at a glance. 70
Risk index definitions. 74
1. Volatility. 74
2. Momentum. 74
3. Size. 74
4. Size Nonlinearity. 74
5. Trading Activity. 74
6. Growth. 75
7. Earnings Yield. 75
8. Value. 75
9. Earnings Variability. 75
10. Leverage. 75
11. Currency Sensitivity. 75
12. Dividend Yield. 75
13. Non-Estimation Universe Indicator. 76
Descriptor definitions. 76

9. US-E3 Industries. 77
Overview. 77
Industry classification scheme. 77
Mini-industries and industries. 77
Sectors. 78
Industry weights. 79
1. The valuation models. 79
2. Asset industry weights for each model. 79 

3. Final weights ..... 80
Historical assignment of industry and weights ..... 80
Ongoing assignment of industry and weights ..... 80
Industry evolution ..... 81
Sector mapping of US-E3 industries ..... 82

10. Factor Return Estimation ..... 85
Overview ..... 85
Estimation details ..... 85
GLS weights ..... 86
Factor returns for historic “newborn” industries ..... 86
The NONESTU factor return ..... 86
Testing ..... 87

11. Estimating the Factor Covariance Matrix in US-E3 ..... 89
Overview ..... 89

12. US-E3 Specific Risk Modeling ..... 91
Overview ..... 91

Appendix A: US-E3 Descriptor Definitions ..... 93
1. Volatility ..... 93
2. Momentum ..... 95
3. Size ..... 96
4. Size Nonlinearity ..... 96
5. Trading Activity ..... 96
6. Growth ..... 98
7. Earnings Yield ..... 100
8. Value ..... 101
9. Earnings Variability ..... 101
10. Leverage ..... 102
11. Currency Sensitivity ..... 103
12. Dividend Yield ..... 104
13. Non-Estimation Universe Indicator ..... 104 

Appendix B: US-E3 Industries, Mini-Industries, Example Companies, and Codes 105
Appendix C: US-E3 Frequency Distributions for Predicted Beta, Specific Risk, Risk Indices 115
Predicted beta. 115
Specific risk. 115
Risk indices. 116
Appendix D: US-E3 Risk Index Factor Returns 121
Glossary. 127
Index. 137
Contributors. 143 

## About BARRA

In recent years the investment management industry has adjusted to continuing changes—theoretical advances, technological developments, and market growth. To address these challenges, investment managers and financial institutions require the most advanced and powerful analytical tools available. 

## A pioneer in risk management

As the leading provider of global investment decision tools, BARRA has responded to these industry changes by providing quantitative products and services that are both flexible and efficient. Since our founding in 1975, BARRA has been a leader in modern financial research and techniques. 

Initially, our services focused on risk analysis in equity markets. Our U.S. Equity Model set a standard of accuracy that BARRA continues to follow. BARRA uses the best data available to develop econometric financial models. In turn, these models are the basis of software products designed to enhance portfolio performance through returns forecasting, risk analysis, portfolio construction, transaction cost analysis, and historical performance attribution. 

In 1979, BARRA expanded into the fixed income area with the release of U.S. bond valuation and risk models. In the mid-1980s we developed a global tactical asset allocation system: The BARRA World Markets Model $^{™}$ . More recently, the Total Plan Risk $^{™}$ approach was developed to provide multi-asset-class value-at-risk (VAR) analyses. 

BARRA now has offices around the world and products that cover most of the world's traded securities. By 1997, our clients comprised approximately 1,200 financial institutions worldwide managing over $7 trillion in assets. They rely on BARRA's investment technology and consulting services to strengthen their financial analysis and investment decision-making. 

## Introduction

## In this handbook

Section I: Theory contains a general discussion of equity risk and return, and the methods BARRA uses to model portfolio risk. Chapters 1 through 5 comprise this section. 

Chapter 1. Why Risk is Important gives an overview of why financial professionals should care about risk. 

Chapter 2. Defining Risk outlines the basic statistical concepts underlying risk analysis, and traces the history of equity risk theory. 

Chapter 3. Modeling and Forecasting Risk discusses the application of multiple-factor modeling (MFM) to the equity risk analysis problem. 

Chapter 4. Modern Portfolio Management and Risk relates the various types of active and passive equity management to the use of a risk model. 

Chapter 5. BARRA Multiple-Factor Modeling details the process of creating and maintaining a BARRA equity MFM. 

Section II: US-E3 Model Details discusses the construction of our third-generation U.S. equity risk model in depth. Chapters 6 through 12 and Appendices A through D comprise this section. 

Chapter 6. Advantages of US-E3 Over US-E2 summarizes the reasons for updating US-E2 and the particular advances made with US-E3 over US-E2. 

Chapter 7. The US-E3 Estimation Universe discusses the expansion of the US-E3 equity portfolio which is used to estimate the main parameters of the risk model. This was done to ensure a more accurate reflection of the investing activities of our clients. 

Chapter 8. US-E3 Risk Indices and Descriptors describes differences from the US-E2 treatment of these factors and improvements that have been made in this part of the model. 

Chapter 9. US-E3 Industries discusses the complete reclassification of the industry assignments and other enhancements intended to keep the model current over time. One of the least satisfactory aspects of US-E2 was the unchanging nature of the industry factor specification. 

Chapter 10. Factor Return Estimation contains a brief description of US-E3's particular implementation of this process. A more general discussion is contained in Chapter 5. 

Chapter 11. Estimating the Factor Covariance Matrix in US-E3 also briefly discusses only those aspects of this subject which are particular to US-E3, with a more general treatment detailed in Chapter 5. 

Chapter 12. US-E3 Specific Risk Modeling also briefly discusses only those aspects of this subject which are particular to US-E3, with a more general treatment detailed in Chapter 5. 

Appendix A: US-E3 Descriptor Definitions is the complete list of risk indices and their underlying data descriptors. 

Appendix B: US-E3 Industries, Mini-Industries, Example Companies, and Codes contains the complete list of industries, their constituent “mini-industries,” and selected example companies. 

Appendix C: US-E3 Frequency Distributions for Predicted Beta, Specific Risk, Risk Indices contains graphical depictions of the distribution of these model outputs. 

Appendix D: US-E3 Risk Index Factor Returns gives a full model history of the returns to the US-E3 risk indices. 

Finally, the Glossary and Index are useful resources for clarifying terminology and enhancing the handbook's usefulness. 

## Further references

BARRA has a comprehensive collection of articles and other materials describing the models and their applications. To learn more about the topics contained in this handbook, consult the following references or our extensive Publications Bibliography, which is available from BARRA offices and from our Web site at http://www.barra.com. 

## Books

Andrew Rudd and Henry K. Clasing, Modern Portfolio Theory: The Principles of Investment Management, Orinda, CA, Andrew Rudd, 1988. 

Richard C. Grinold and Ronald N. Kahn: Active Portfolio Management: Quantitative Theory and Applications, Probus Publishing, Chicago, IL, 1995. 

## 1. Why Risk is Important

Superior investment performance is the product of careful attention to four elements: 

■ forming reasonable return expectations 

■ controlling risk so that the pursuit of opportunities remains tempered by prudence 

■ controlling costs so that investment profits are not dissipated in excessive or inefficient trading 

■ controlling and monitoring the total investment process to maintain a consistent investment program 

These four elements are present in any investment management problem, be it a strategic asset allocation decision, an actively managed portfolio, or an index fund—managed bottom-up or top-down, via traditional or quantitative methods. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/715ef1f685952dcf5451cd8ff6e00a9cb22c57f47903c420766dd70c4bbe49c8.jpg)



Figure 1-1
The Performance Pyramid


In a simpler view, return and risk are the protagonist and antagonist of investing. According to an old adage, the tradeoff between return and risk is the tradeoff between eating well and sleeping well. Clearly, risk doesn't just matter to quants! 

Ignoring risk is hazardous to your portfolio. The optimal strategy ignoring risk places the entire portfolio in one stock. But no institutional investor follows this strategy. Hence risk considerations must impact every institutional portfolio. Unfortunately, they sometimes do not impact them enough. 

We need not look far to find examples of financial disasters that arose through lack of sufficient risk control. The debacles of Orange County, Barings Bank, and the Piper Jaffray Institutional Government Income Fund all testify to the dangers of ignoring or poorly understanding risk. 

But risk analysis is more than avoiding disasters—it can in fact enhance opportunities. Peter Bernstein has argued that a lack of understanding of risk holds back economic development. $^{1}$ Modern economic growth requires understanding risk. 

What are the expected returns to a new venture? What are the risks? Do the returns outweigh the risks? Can I hedge the risks? In modern economies, the future is not beyond management, not simply subject to the whims of many gods. In fact, the period which marked the development of probability and statistics (during and after the Renaissance) also marked a time of profound growth in trade, exploration, and wealth. The ideas of risk management enabled the modern economic world, according to Bernstein. Risk analysis enhanced opportunities. 

While Bernstein's argument may seem inspiring—though not of day-to-day relevance—in fact the goal of risk analysis is not to minimize risk but to properly weigh risk against return. Sometimes risk analysis leads to taking more risk. 

## The goal of risk analysis

Risk is important. It is a critical element of superior investment performance. Good risk analysis should provide not only a number—a quantification of risk—but insight, especially insight into the “Performance Pyramid.” 

We have illustrated superior performance as a three-dimensional object. A single risk number is only one-dimensional. So what do we mean by insight? 

Risk analysis should uncover not just overall risk, but the largest and smallest bets in the portfolio. Do the largest bets correspond to the highest expected returns? They should. If they do not, the portfolio isn't properly balancing return and risk. Are the bets too large or too small? What is the “worst case” scenario? How will the portfolio compare to its benchmark? 

Robust risk analysis can provide answers to all these questions as well as insight to all investors. In this volume we will discuss the history and current practice of equity risk modeling for single country markets. Other methods are used for different securities, such as bonds or currencies, and for different market structures, such as the global stock market. The underlying message is clear: The investor armed with superior methods of assessing and controlling risk possesses a significant competitive edge in modern capital markets. 

## 2. Defining Risk

## Some basic definitions

In an uncertain investment environment, investors bear risk. Risk is defined as the total dispersion or volatility of returns for a security or portfolio. Further, risk reflects uncertainty about the future. 

We will define risk as the standard deviation of the return. Risk is an abstract concept. An economist considers risk to be expressed in a person's preferences. What is perceived as risky for one individual may not be risky for another. $^{1}$ 

We need an operational and therefore universal and impersonal definition of risk. Institutional money managers are agents of pension fund trustees and other asset sponsors, who are themselves agents of the sponsoring organization and, ultimately, the beneficiaries of the fund. In that setting we cannot hope to have a personal view of risk. 

We need a symmetric view of risk. Institutional money managers are judged relative to a benchmark or relative to their peers. The money manager suffers as much if he does not hold a stock and it goes up as if he held a larger than average amount of the stock and it goes down. 

We need a flexible definition of risk. Our definition of risk should apply to individual stocks and to portfolios. We should be able to talk about realized risk in the past, and forecast risk over any future horizon. 

The definition of risk that meets these criteria of being universal, symmetric, and flexible is the standard deviation of return. $^{2,3}$ If $R_P$ is a portfolio's total return, then the portfolio's standard deviation of return is denoted by $\sigma_{P} \equiv Std\big[R_{P}\big]$ . A portfolio's excess return $r_{P}$ differs from the total return $R_{P}$ by a constant $R_{F}$ , so the risk of the excess return is equal to the risk of the total return. We will typically quote this risk, or standard deviation of return, on a percent per year basis. We will also occasionally refer to this quantity as volatility. $^{1}$ 

The rough interpretation of standard deviation is that the return will be within one standard deviation of its expected value two-thirds of the time and within two standard deviations nineteen times out of twenty. Figure 2-1 graphically illustrates this fact. 

Figure 2-1 

Risk: The Dispersion of Returns
The standard deviation is a statistical measure of dispersion around an expected value—in this case, zero. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/7da02454850ad7c3964e3994d6843ab6440e116eb9784e8bf09b916365fca67d.jpg)


## Risk measurement

A related risk measure is variance, the standard deviation squared. The formulae are: 

$$
S t d [ \tilde {r} ] = \sqrt {\operatorname{Var} [ \tilde {r} ]}\tag{EQ 2-1}
$$

$$
\operatorname{Var} \left[ \tilde {r} \right] = \mathrm{E} \left[ (\tilde {r} - \bar {r}) ^ {2} \right]\tag{EQ 2-2}
$$

where: 

$$
\tilde {r} = \mathrm{return},
$$

$\bar{r}$ = expected or mean return, 

$Std[x] = \text{standard deviation of } x,$ 

$Var[x] = \text{variance of } x, \text{ and}$ 

$$
\operatorname{E} [ x ] = \text { expected   value   of } x.
$$

The standard deviation is the more common risk indicator since it is measured in the same units as return. Of course, if the standard deviation is known, the variance can be easily computed and vice versa. Other measures, including value-at-risk and shortfall risk, can be easily computed from the standard deviation. 

## An example

The standard deviation has some interesting characteristics. In particular it does not have the portfolio property. The standard deviation of a stock portfolio is not the weighted average of the standard deviations of the component stocks. 

For example, suppose the correlation between the returns of Stocks 1 and 2 is $\rho_{12}$ . If we have a portfolio of 50% Stock 1 and 50% Stock 2, then: 

$$
\sigma_ {P} = \sqrt {\left(0 . 5 \cdot \sigma_ {1}\right) ^ {2} + \left(0 . 5 \cdot \sigma_ {2}\right) ^ {2} + 2 \cdot \left(0 . 5 \cdot \sigma_ {1}\right) \left(0 . 5 \cdot \sigma_ {2}\right) \cdot \rho_ {1 2}}\tag{EQ 2-3}
$$

$$
\text { and } \sigma_ {P} \leq 0. 5 \cdot \sigma_ {1} + 0. 5 \cdot \sigma_ {2}\tag{EQ 2-4}
$$

with such equality being maintained only if the two stocks are perfectly correlated ( $\rho_{12} = 1$ ). For risk, the whole is less than the sum of its parts. This is the key to portfolio diversification. 


Figure 2-2
Risk Reduction Benefits of Diversification:
A Two-Stock Example


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/55a0807d407966e4a8fb94ed18df7670f4a9a5986ef858d49c03becb6f5f173b.jpg)



Figure 2-2 shows a simple example. The risk of a portfolio made up from IBM and General Electric is plotted against the fraction of GE stock in the portfolio. The curved line represents the risk of the portfolio; the straight line represents the risk that we would obtain if the returns on IBM and GE were perfectly correlated. The risk of GE is 27.4% per year; the risk of IBM is 29.7% per year; and the two returns are 62.9% correlated. The difference between the two lines is an indication of the benefit of diversification in reducing risk.


## Risk reduction through diversification

We can see the power of diversification in another example. Given a portfolio of N stocks, each with risk $\sigma$ and uncorrelated returns, the risk of an equal-weighted portfolio of these stocks will be: 

$$
\sigma_ {P} = \frac {\sigma}{\sqrt {N}}\tag{EQ 2-5}
$$

Note that the average risk is $\sigma$ , while the portfolio risk is $\sigma/\sqrt{N}$ . 

For a more useful insight into diversification, assume now that the correlation between the returns of all pairs of stocks is equal to $\rho$ . Then the risk of an equally weighted portfolio is: 

$$
\sigma_ {P} = \sigma \cdot \sqrt {\frac {1 + \rho \cdot (N - 1)}{N}}\tag{EQ 2-6}
$$

In the limit that the portfolio contains a very large number of correlated stocks, this becomes: 

$$
\sigma_ {P} \Rightarrow \sigma \cdot \sqrt {\rho}\tag{EQ 2-7}
$$

To get a feel for this, consider the example of an equal-weighted portfolio of the 20 Major Market Index constituent stocks. In December 1992, these stocks had an average risk of 27.8%, while the equal-weighted portfolio has a risk of 20.4%. $^{1}$ Equation 2-6 then implies an average correlation between these stocks of 0.52. 

Risks don't add across stocks and risks don't add across time. However, variance will add across time if the returns in one interval of time are uncorrelated with the returns in other intervals of time. The assumption is that returns are uncorrelated from period to period. The correlation of returns across time (called autocorrelation) is close to zero for most asset classes. This means that variances will grow with the length of the forecast horizon and the risk will grow with the square root of the forecast horizon. Thus, a $5\%$ annual active risk is equivalent to a $2.5\%$ active risk over the first quarter or a $10\%$ active risk over four years. Notice that the variance over the quarter, year, and four-year horizon (6.25, 25, and 100) remains proportional to the length of the horizon. 

We use this relationship every time we “annualize” risk—i.e., standardize our risk numbers to an annual period. If we examine monthly returns to a stock and observe a monthly return standard deviation of $\sigma_{monthly}$ , we convert this to annual risk according to: 

$$
\sigma_ {a n n u a l} = \sqrt {1 2} \cdot \sigma_ {m o n t h l y}\tag{EQ 2-8}
$$

## Drawbacks of simple risk calculations

The mathematical calculation of risk using standard deviation of returns is therefore straightforward and can be extended to any number of securities. However, this approach suffers from several drawbacks: 

■ Estimating a robust covariance matrix of returns requires data for as many periods as we have securities to analyze. For large markets, such as the U.S. stock market, these long returns histories may simply not be available. 

■ Estimation error may occur in any one period due to spurious asset correlations that are unlikely to repeat in a systematic fashion. 

A simple covariance matrix of returns offers little in the way of economic analysis. In other words, it is largely a “black box” approach with little intuitive basis or forecastability. 

For all these reasons, financial economists have sought for many years to model investment risk in more nuanced ways. We will now turn to a brief history of these efforts. 

## Evolution of concepts

The development of equity risk concepts has evolved from the modest and unscientific guesswork of early investment theory to the quantitative analysis and technical sophistication of modern financial tools. 

Before the 1950s, there was no concept of systematic, or market-related, return. Return was a rise in the value of a stock and risk was a drop in the value of a stock. The investor's primary investment tools were intuition and insightful financial analysis. Portfolio selection was simply an act of assembling a group of “good” stocks. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/2bd708556b4302a3907d95041aee3625bb7706273b4f80e460fd2dba96376ba0.jpg)



Figure 2-3



Diversification and Risk
As a portfolio manager increases the number of stocks in a portfolio, residual—or non-market-related—risk is diversified. Market risk is undiversifiable.


Financial theorists became more scientific and statistical in the early 1950s. Harry Markowitz was the first to quantify risk (as standard deviation) and diversification. He showed precisely how the risk of the portfolio was less than the risk of its components. In the late 1950s, Breiman and Kelly derived mathematically the peril of ignoring risk. They showed that a strategy that explicitly accounted for risk outperformed all other strategies in the long run. $^{1}$ 

We now know how diversification affects risk exposures. It averages factor-related risk, such as industry exposures, and significantly reduces security-specific risk. However, diversification does not eliminate all risk because stocks tend to move up and down together with the market. Therefore, systematic, or market, risk cannot be eliminated by diversification. 

Figure 2-3 shows the balance between residual risk and market risk changing as the number of different stocks in a portfolio rises. At a certain portfolio size, all residual risk is effectively removed, leaving only market risk. 

As investment managers became more knowledgeable, there was a push to identify the conceptual basis underlying the concepts of risk, diversification, and returns. The Capital Asset Pricing Model (CAPM) was one approach that described the equilibrium relationship between return and systematic risk. William Sharpe earned the Nobel Prize in Economics for his development of the CAPM. 

Figure 2-4 

The Capital Asset Pricing Model
The Capital Asset Pricing Model asserts that the expected excess return on securities is proportional to their systematic risk coefficient, or beta. The market portfolio is characterized by a beta of unity. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/58dc1d84e3b0607a207958f2e6caf1aca0e5fd4fb11716b27a3ed409fe1aee18.jpg)


The central premise of CAPM is that, on average, investors are not compensated for taking on residual risk. CAPM asserts that the expected residual return is zero while the expected systematic return is greater than zero and linear (see Figure 2-4). 

The measure of portfolio exposure to systematic risk is called beta ( $\beta$ ). Beta is the relative volatility or sensitivity of a security or portfolio to market moves. More simply, beta is the numerical value of an asset's systematic risk. Returns, and hence risk premiums, for any stock or portfolio will be related to beta, the exposure to undiversifiable systematic risk. Equation 2-9 states this linear relationship. 

$$
\operatorname{E} \bigl [ \tilde {r} _ {i} \bigr ] - r _ {F} = \beta_ {i} \operatorname{E} \bigl [ \tilde {r} _ {M} - r _ {F} \bigr ]\tag{EQ 2-9}
$$

where: 

"Only undiversifiable risk should earn a premium."
William F. Sharpe, 1964
Capital Asset Pricing Model 

$$
\tilde {r} _ {i} = \mathrm{returnonasseti},
$$

$r_{F} =$ risk-free rate of return, 

$\tilde{r}_M =$ return on market portfolio, and 

$$
\beta_ {i} = \frac {\operatorname{Cov} \left[ \tilde {r} _ {i} , \tilde {r} _ {M} \right]}{\operatorname{Var} \left[ \tilde {r} _ {M} \right]}
$$

The CAPM is a model of return. Underlying it are equilibrium arguments and the view that the market is efficient because it is the portfolio that every investor on average owns. The CAPM does not require that residual returns be uncorrelated. But it did inspire Sharpe to suggest a one-factor risk model that does assume uncorrelated residual returns. This model has the advantage of simplicity. It is quite useful for back of the envelope calculations. But it ignores the risk that arises from common factor sources, such as industries, capitalization, and yield. 

By the 1970s, the investment community recognized that assets with similar characteristics tend to behave in similar ways. This notion is captured in the Arbitrage Pricing Theory (APT). APT asserts that security and portfolio expected returns are linearly related to the expected returns of an unknown number of underlying systematic factors. 

The focus of APT is on forecasting returns. Instead of equilibrium arguments, Ross and others used arbitrage arguments to assert that expected specific returns are zero, but expected common factor returns (including the market and other factors) need not be zero. Just like the CAPM, APT inspired a class of risk models: the multiple-factor model (MFM). The basic premise of an MFM is that many influences act on the volatility of a stock, and these influences are often common across many stocks. A properly constructed MFM is able to produce risk analyses with more accuracy and intuition than a simple covariance matrix of security returns or the CAPM. 

Multifactor models of security market returns can be divided into three types: macroeconomic, fundamental, and statistical factor models. Macroeconomic factor models use observable economic time series, such as inflation and interest rates, as measures of the pervasive shocks to security returns. Fundamental factor models use the returns to portfolios associated with observed security attributes such as dividend yield, the book-to-market ratio, and industry membership. Statistical factor models derive their factors from factor analysis of the covariance matrix of security returns. BARRA research has confirmed that of these three, fundamental factor models outperform the other two types in terms of explanatory power. $^{1}$ 

We now turn to a discussion of fundamental MFMs in more detail. 

"Since the factors can represent the components of return as seen by the financial analyst, the multiple-factor model is a natural representation of the real environment." Barr Rosenberg, 1974 Multiple Factor Models 

## 3. Modeling and Forecasting Risk

Through the years, theoretical approaches to investment analysis have become increasingly sophisticated. With more advanced concepts of risk and return, investment portfolio models have changed to reflect this growing complexity. The multiple-factor model (MFM) has evolved as a helpful tool for analyzing portfolio risk. 

## What are MFMs?

Multiple-factor models (MFMs) are formal statements about the relationships among security returns in a portfolio. The basic premise of MFMs is that similar stocks should display similar returns. This “similarity” is defined in terms of ratios, descriptors, and asset attributes which are based on market information, such as price and volume, or fundamental data derived from a company’s balance sheet and income statement. 

MFMs identify common factors and determine return sensitivity to these factors. The resulting risk model incorporates the weighted sum of common factor return and specific return. The risk profile will respond immediately to changes in fundamental information. 

## How do MFMs work?

We derive MFMs from securities patterns observed over time. The difficult steps are pinpointing these patterns and then identifying them with asset factors that investors can understand. Asset factors are characteristics related to securities price movements, such as industry membership, capitalization, and volatility. 

Once model factors are chosen and assigned to individual assets in the proper proportions, cross-sectional regressions are performed to determine the returns to each factor over the relevant time period. This allows the model to be responsive to market changes in a timely fashion. 

Risk calculation is the final step in constructing a sound and useful model. Variances, covariances, and correlations among factors are estimated and weighted. We then use these calculations to describe the risk exposure of a portfolio. 

Investors rely on risk exposure calculations to determine stock selection, portfolio construction, and other investment strategies. They base their decisions on information gleaned from MFM analysis as well as their risk preferences and other information they possess. 

## Advantages of MFMs

There are several advantages to using MFMs for security and portfolio analysis. 

■ MFMs offer a more thorough breakdown of risk and, therefore, a more complete analysis of risk exposure than other methods such as simple CAPM approaches. 

■ Because economic logic is used in their development, MFMs are not limited by purely historical analysis. 

■ MFMs are robust investment tools that can withstand outliers. 

■ As the economy and individual firms change, MFMs adapt to reflect changing asset characteristics. 

■ MFMs isolate the impact of individual factors, providing segmented analysis for better informed investment decisions. 

■ From an applications viewpoint, MFMs are realistic, tractable, and understandable to investors. 

■ Lastly, MFMs are flexible models allowing for a wide range of investor preferences and judgment. 

Of course, MFMs have their limitations. They predict much, but not all, of portfolio risk. In addition, a model does not offer stock recommendations; investors must make their own strategy choices. 

## A simple MFM

To illustrate the power of MFMs, let's begin with a simple example. 

Accurate characterization of portfolio risk requires an accurate estimate of the covariance matrix of security returns. A relatively simple way to estimate this covariance matrix is to use the history of security returns to compute each variance and covariance. This approach, however, suffers from two major drawbacks: 

■ Estimating a covariance matrix for, say, 3,000 stocks requires data for at least 3,000 periods. With monthly or weekly estimation horizons, such a long history may simply not exist. 

It is subject to estimation error: in any period, two stocks such as Weyerhaeuser and Ford may show very high correlation—higher than, say, GM and Ford. Our intuition suggests that the correlation between GM and Ford should be higher because they are in the same line of business. The simple method of estimating the covariance matrix does not capture our intuition. 

This intuition, however, points to an alternative method for estimating the covariance matrix. Our feeling that GM and Ford should be more highly correlated than Weyerhaeuser and Ford comes from Ford and GM being in the same industry. Taking this further, we can argue that firms with similar characteristics, such as their line of business, should have returns that behave similarly. For example, Weyerhaeuser, Ford, and GM will all have a common component in their returns because they would all be affected by news that affects the stock market as a whole. The effects of such news may be captured by a stock market component in each stock's return. This common component may be the (weighted) average return to all U.S. stocks. The degree to which each of the three stocks responds to this stock market component depends on the sensitivity of each stock to the stock market component. 

Additionally, we would expect GM and Ford to respond to news affecting the automobile industry, whereas we would expect Weyerhaeuser to respond to news affecting the forest and paper products industry. The effects of such news may be captured by the average returns of stocks in the auto industry and the forest and paper products industry. There are, however, events that affect one stock without affecting the others. For example, a defect in the brake system of GM cars, that forces a recall and replacement of the system, will likely have a negative impact on GM's stock price. This event, however, will most likely leave Weyerhaeuser and Ford stock prices unaltered. 

These arguments lead us to the following representation for returns: 

$$
\begin{array}{r} \tilde {r} _ {G M} = \mathrm{E} \big [ \tilde {r} _ {G M} \big ] + \beta_ {G M} \cdot \big [ \tilde {r} _ {M} - \mathrm{E} \big [ \tilde {r} _ {M} \big ] \big ] \\ + 1 \cdot \big [ \tilde {r} _ {A U T O} - \mathrm{E} \big [ \tilde {r} _ {A U T O} \big ] \big ] + 0 \cdot \big [ \tilde {r} _ {F P} - \mathrm{E} \big [ \tilde {r} _ {F P} \big ] \big ] + u _ {G M} \end{array}\tag{EQ 3-1}
$$

where: 

$$
{\tilde {r} _ {G M}} {= \mathrm {GM^ {\prime} s realized return},}
$$

$$
\tilde {r} _ {M} = \text { the   realized   average   stock   market   return },
$$

$\tilde{r}_{AUTO} =$ realized average return to automobile stocks, 

$\tilde{r}_{FP} =$ the realized average return to forest and paper products stocks, 

$\operatorname {E}[.] =$ expectations, 

$\beta_{GM} = \mathrm{GM's~sensitivity~to~stock~market~returns, and}$ 

$u_{GM}$ = the effect of GM specific news on GM returns. 

This equation simply states that GM's realized return consists of an expected component and an unexpected component. 

The unexpected component depends on any unexpected events that affect stock returns in general $\left[\tilde{r}_{M}-\mathrm{E}\left[\tilde{r}_{M}\right]\right]$ , any unexpected events that affect the auto industry $\left[\tilde{r}_{AUTO}-\mathrm{E}\left[\tilde{r}_{AUTO}\right]\right]$ , and any unexpected events that affect GM alone $(u_{GM})$ . Similar equations may be written for Ford and Weyerhaeuser. 

The sources of variation in GM's stock returns, thus, are variations in stock returns in general, variations in auto industry returns, and any variations that are specific to GM. Moreover, GM and Ford returns are likely to move together because both are exposed to stock market risk and auto industry risk. Weyerhaeuser and GM, and Weyerhaeuser and Ford, on the other hand, are likely to move together to a lesser degree because the only common component in their returns is the market return. Some additional correlation would arise, however, because auto and forest and paper products industry returns may exhibit some correlation. 

By beginning with our intuition about the sources of co-movement in security returns, we have made substantial progress in estimating the covariance matrix of security returns. What we need now is the covariance matrix of common sources in security returns, the variances of security specific returns, and estimates of the sensitivity of security returns to the common sources of variation in their returns. Because the common sources of risk are likely to be much fewer than the number of securities, we need to estimate a much smaller covariance matrix and hence a smaller history of returns is required. Moreover, because similar stocks are going to have larger sensitivities to similar common sources of risk, similar stocks will be more highly correlated than dissimilar stocks: our estimated correlation for GM and Ford will be larger than that for Ford and Weyerhaeuser. 

The decomposition of security returns into common and specific sources of return is, in fact, a multiple-factor model of security returns. We now turn to a generalized discussion of this process for many factors. 

## Model mathematics

MFMs build on single-factor models by including and describing the interrelationships among factors. For single-factor models, the equation that describes the excess rate of return is: 

$$
\tilde {r} _ {j} = X _ {j} \tilde {f} + \tilde {u} _ {j}\tag{EQ 3-2}
$$

where: 

$\tilde{r}_j =$ total excess return over the risk-free rate, 

$X_{j} =$ sensitivity of security $j$ to the factor, 

$\tilde{f} =$ rate of return on the factor, and 

$\tilde{u}_j = \text{nonfactor (specific) return on security } j$ . 

We can expand this model to include K factors. The total excess return equation for a multiple-factor model becomes: 

$$
\tilde {r} _ {j} = \sum_ {k = 1} ^ {K} X _ {j k} \tilde {f} _ {k} + \tilde {u} _ {j}\tag{EQ 3-3}
$$

where: 

$$
X _ {j k} = \text { risk   exposure   of   security } j \text { to   factor } k, \text { and }
$$

$$
\tilde {f} _ {k} = \text { rate   of   return   on   factor } k.
$$

Note that when K=1, the MFM equation reduces to the earlier single-factor version. For example, the CAPM is a single-factor model in which the “market” return is the only relevant factor. 

When a portfolio consists of only one security, Equation 3-3 describes its excess return. But most portfolios comprise many securities, each representing a proportion, or weight, of the total portfolio. When weights $h_{P1}, h_{P2}, \ldots, h_{PN}$ reflect the proportions of N securities in portfolio P, we express the excess return in the following equation: 

$$
\tilde {r} _ {P} = \sum_ {k = 1} ^ {K} X _ {P k} \tilde {f} _ {k} + \sum_ {j = 1} ^ {N} h _ {P j} \tilde {u} _ {j}\tag{EQ 3-4}
$$

where: 

$$
X _ {P k} = \sum_ {j = 1} ^ {N} h _ {P j} X _ {j k}
$$

This equation includes the risk from all sources and lays the groundwork for further MFM analysis. 

## Risk prediction with MFMs

Investors look at the variance of their total portfolios to provide a comprehensive assessment of risk. To calculate the variance of a portfolio, you need to calculate the covariances of all the constituent components. 

Without the framework of a multiple-factor model, estimating the covariance of each asset with every other asset is computationally burdensome and subject to significant estimation errors. For exam-

Figure 3-2 

ple, using an estimation universe of 1,400 assets, there are 980,700 covariances and variances to calculate (see Figure 3-1). 

$$
\begin{array}{c} \mathsf {V} (i, j) = \text {Covariance} [ r (\tilde {i}), r (\tilde {j}) ] \\ \text {where} \mathsf {V} (i, j) = \text {asset covariance matrix, and} \\ i, j = \text {individual stocks.} \\ \mathsf {V} = \left[ \begin{array}{c c c c} \mathsf {V} (1, 1) & \mathsf {V} (1, 2) & \ldots & \mathsf {V} (1, N) \\ \mathsf {V} (2, 1) & \mathsf {V} (2, 2) & \ldots & \mathsf {V} (2, N) \\ \mathsf {V} (3, 1) & \mathsf {V} (3, 2) & \ldots & \mathsf {V} (3, N) \\ \vdots & \vdots & & \vdots \\ \mathsf {V} (N, 1) & \mathsf {V} (N, 2) & \ldots & \mathsf {V} (N, N) \end{array} \right] \end{array}
$$

Asset Covariance Matrix
For N=1,400 assets, there are 980,700 covariances and variances to estimate. 

An MFM simplifies these calculations dramatically. This results from replacing individual company profiles with categories defined by common characteristics (factors). Since the specific risk is assumed to be uncorrelated among the assets, only the factor variances and covariances need to be calculated during model estimation (see Figure 3-2). 

$$
\widetilde {r} = X \widetilde {f} + \widetilde {u}
$$

$$
\begin{array}{r l} \text {where} & \widetilde {r} = \text {vector of excess returns}, \\ & X = \text {exposure matrix}, \\ & \widetilde {f} = \text {vector of factor returns, and} \\ & \widetilde {u} = \text {vector of specific returns}. \end{array}
$$

Factor Return Calculation
Using an MFM greatly simplifies the estimation process.
Figure 3-2 depicts the multiple-factor model in matrix terms. 

$$
\begin{array}{r l r} \left[ \begin{array}{l} \widetilde {\textbf {r}} (1) \\ \widetilde {\textbf {r}} (2) \\ \vdots \\ \widetilde {\textbf {r}} (N) \end{array} \right] & = & \left[ \begin{array}{l l l l} X (1, 1) & X (1, 2) & \dots & X (1, K) \\ X (2, 1) & X (2, 2) & \dots & X (2, K) \\ \vdots & \vdots & & \vdots \\ X (N, 1) & X (N, 2) & \dots & X (N, K) \end{array} \right] \left[ \begin{array}{l} \widetilde {\textbf {f}} (1) \\ \widetilde {\textbf {f}} (2) \\ \vdots \\ \widetilde {\textbf {f}} (K) \end{array} \right] + \left[ \begin{array}{l} \widetilde {\textbf {u}} (1) \\ \widetilde {\textbf {u}} (2) \\ \vdots \\ \widetilde {\textbf {u}} (N) \end{array} \right] \end{array}
$$

By using a multiple-factor model, we significantly reduce the number of calculations. For example, in the U.S. Equity Model (US-E3), 65 factors capture the risk characteristics of equities. This reduces the number of covariance and variance calculations to 2,145 (see Figure 3-3). Moreover, since there are fewer parameters to determine, they can be estimated with greater precision. 

Figure 3-3 

Factor Covariance Matrix
For K=65 factors, there are 2,145 covariances and variances to estimate. Quadrant I includes the covariances of risk indices with each other; quadrants II and III are mirror images of each other, showing the covariances of risk indices with industries; and quadrant IV includes covariances of industries with each other. 

$\begin{array}{c}\mathsf{F}(k,m) = \mathsf{Covariance}[\widetilde{f} (k),\widetilde{f} (m)]\\ \text{where}\quad \mathsf{F}(k,m) = \text{factor covariance matrix, and}\\ k,m = \text{common factors.} \end{array}$ $\mathsf{F} = \left[ \begin{array}{cccc:ccc}F(1,1) & \dots & F(1,13) &  & F(1,14) & \dots & F(1,65)\\ \vdots & I & \vdots &  & \vdots & II & \vdots \\ F(13,1) & \dots & F(13,13) &  & F(13,14) & \dots & F(13,65)\\ \hline  &  &  &  &  &  &  \\ F(14,1) & \dots & F(14,13) &  & F(14,14) & \dots & F(14,65)\\ \vdots & III & \vdots &  & \vdots & IV & \vdots \\ F(65,1) & \dots & F(65,13) &  & F(65,14) & \dots & F(65,65) \end{array} \right]$ 

We can easily derive the matrix algebra calculations that support and link the above diagrams by using an MFM. From Figure 3-2, we start with the MFM equation: 

$$
\tilde {r} _ {i} = X \tilde {f} + \tilde {u}\tag{EQ 3-5}
$$

where: 

$\tilde{r}_i =$ excess return on asset $i$ , 

X = exposure coefficient on the factor, 

$\tilde{f} =$ factor return, and 

$\tilde{u} =$ specific return. 

Substituting this relation in the basic equation, we find that: 

$$
\begin{array}{l} R i s k = V a r \Big (\tilde {r} _ {j} \Big) \\ = V a r \Big (X \tilde {f} + \tilde {u} \Big) \end{array}\tag{EQ 3-6}
$$

(EQ 3-7) 

Using the matrix algebra formula for variance, the risk equation becomes: 

$$
R i s k = X F X ^ {T} + \Delta\tag{EQ 3-8}
$$

where: 

X = exposure matrix of companies upon factors, 

F = covariance matrix of factors, 

$X^{T} =$ transpose of $X$ matrix, and 

$\Delta =$ diagonal matrix of specific risk variances. 

This is the basic equation that defines the matrix calculations used in risk analysis in the BARRA equity models. 

## 4. Modern Portfolio Management and Risk

In the previous chapters we observed that risk modeling is essential to successful portfolio management and that the standard deviation of returns is the best numerical risk measure. We also traced the evolution of risk concepts from portfolio standard deviation of security returns, through the CAPM and APT, to the current application of multiple-factor models (MFMs) in the portfolio management problem. In this chapter we will briefly explore the components of portfolio management and how BARRA MFMs can assist the manager at various points. In the next chapter a detailed description of BARRA MFMs will complete the theoretical portion of this handbook. 

## Portfolio management—two types

An equity portfolio manager must choose between two management methods: passive or active. BARRA MFMs are used to facilitate both methods. 

## Passive management

Passive management is an outgrowth of CAPM logic. In its broadest sense, passive management refers to any management strategy that does not rely on the possession of superior information. More specifically, disclosure of a passive investment strategy offers no competitive information that would undermine the strategy's validity. 

One type of passive management is indexing, tracking the performance of a particular index. An example is the “buy-and-hold” philosophy which exposes the portfolio only to systematic risk. The second form of passive management is constructing a portfolio to match prespecified attributes or constraints. The portfolio may be yield-biased with a selected beta or match an index within certain parameters. This is often called enhanced indexing. 

## Benchmark

A benchmark is the standard of comparison for investment performance and risk analysis. It is widely used to evaluate and track performance of investment managers. The benchmark is also known as the normal portfolio—that is, the asset basket a manager would hold in the absence of any judgmental information. It reflects the manager's particular style and biases. 

## Tracking Error

Tracking error is a measure of risk exposure. It is the annualized standard deviation of the difference between portfolio return and benchmark return. 

Because it provides a relative measure of risk exposure, tracking error is a useful evaluation tool, particularly for passive portfolios. Moreover, it offers relevant performance comparisons because the benchmark is selected based on portfolio characteristics and investor objectives. 

## Alpha

Alpha ( $\alpha$ ) generally refers to the expected exceptional return of a portfolio, factor, or individual asset. The use of alphas is a distinction of active management. They indicate that a manager believes a portion of expected return is attributable to particular factors. 

Historical alpha is the difference between actual performance and the performance of a diversified market portfolio with identical systematic risk over the same period. Judgmental, or predicted, alpha is the expected value of subsequent extraordinary return based on a return forecast. 

Passive management procedures are distinguished by the following attributes: 

■ They exclude any transactions in response to judgments about security valuations and the market as a whole. 

■ They contain relatively minimal residual risk with respect to the benchmark or index. 

■ They often involve industry or sector weighting. 

BARRA MFMs facilitate passive management by providing robust portfolio risk estimates versus passive benchmarks. The indexed portfolio can be readily compared with the benchmark to determine the magnitude of active risk (or tracking error) and its composition. Corrective action can be taken based on individual holding analysis which reveals those securities contributing the most active risk. Optimizing software can also be used to automate the rebalancing process. 

## Active management

Active management refers to investment strategies designed to increase return by using superior information. In other words, the active manager seeks to profit from information that would lose its value if all market participants interpreted it in the same way. If, for example, an investment manager observed that securities with certain characteristics performed better (or worse) than expected, the manager could hold a larger (or smaller) proportion of that security to increase the subsequent value of the portfolio. 

By following active management strategies, investors can add value to their portfolio if they predict returns better than the consensus expectations of the market. Information is obtained through ongoing research to forecast such things as yield curve changes, factor and industry returns, and transitory mispricing. At any given time, portfolio construction should reflect the tradeoff between risk and return—that is, any contribution to risk should be offset by the contribution to reward. 

There are several basic types of active investment strategies. They include market timing, sectoral emphasis, and stock selection. 

Market timing is the process of altering market risk exposure based on short-term forecasts in order to earn superior returns. The manager seeks to sell before the market goes down and buy before the 

Figure 4-1 

market goes up. However, this strategy increases the variability in the portfolio beta, inducing increased systematic risk through time. BARRA MFMs assist market timing by giving the investor a robust beta estimate for any portfolio and indicating the most efficient way to take on or reduce market risk, including the use of futures. 

The second type of active management is sectoral emphasis. Sectoral emphasis can be thought of as a combination of the other active strategies. It is both factor timing and a broad version of stock selection. The manager attempts to increase residual return through manipulating common factor exposures. For example, the manager can bet on an industry of high-yield stocks. Because several sectors can be emphasized at any given time, diversification is possible. BARRA MFMs possess detailed industry and risk index exposure information that can be utilized for any combination of sectoral tilts. 

Lastly, stock selection is a portfolio allocation strategy based on picking mispriced stocks. It uses security alphas to identify over- and undervalued stocks. The manager can then adjust the asset proportions in the portfolio to maximize specific return. These active holdings, in both positive and negative directions, increase residual risk and portfolio alpha. The primary objective of this strategy is to manage asset holdings so that any change in incremental risk is compensated by a comparable change in return. BARRA MFMs facilitate stock selection by extending the risk model down to the individual equity level. 

Figure 4-1 illustrates the typical prevalence of these various types of risk in a single stock, a small portfolio, and a multiple-portfolio situation. In each case, the manager's goal is to earn a superior return with minimum risk. The use of a multiple-factor model permits the manager to pursue these active management strategies with maximum precision. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/cd81ae4518cf36155ea53237ed4d6fbeda205b61de5099b1cd9add09e1de2b08.jpg)



Typical Individual Stock


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/f0d7aaa27914ce82a18e4a782a5d34ed9a9f918dde7d4d51956246d049da29cc.jpg)



Typical Institutional Portfolio with 50 stocks


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/688a7625f0a8b0133c25007f77fec4c246c9b0d487dd870c7167d923f7b81e9c.jpg)



Typical Sponsor Portfolio with Multiple Managers


□ Stock Selection
■ Sectoral Emphasis
■ Market Timing
□ Market 

Diversification and Risk
Market risk grows as a proportion of total risk as portfolio size increases. 

## Decomposing risk

BARRA's equity models isolate components of risk based on correlations across securities sharing similar characteristics. There are several ways to break down a portfolio's risk. BARRA uses any of four decompositions of risk, each reflecting a different perspective on portfolio management. These four decompositions are used in different ways by active and passive managers to provide insight and enhance performance. 

## Total Risk Decomposition


Figure 4-2
Total Risk Decomposition


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/7bd9b2269f9a7e5dfbb724b42171fc7b5e0465077acb54758335369d1b427b14.jpg)


The simplest risk decomposition, Total Risk (see Figure 4-2), is a basic breakdown into specific and common factor risk. There is no concept of a market, or systematic, portfolio. The risk is attributed purely to common factor and security-specific influences. 

Common factor risk is portfolio risk that arises from assets' exposures to common factors, such as capitalization and industries. 

Specific risk is unique to a particular company and thus is uncorrelated with the specific risk of other assets. For a portfolio, specific risk is the weighted sum of all the holdings' specific risk values. 

This risk decomposition is useful for managers who wish to minimize total risk, or for managers such as hedge funds which may be pursuing market-neutral or other long/short strategies. 

## Systematic-Residual Risk Decomposition

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/bc0a8f6256a57d3123d90c5a55cb10ecf9a3447734c4a709f918d0864c9c637f.jpg)



Systematic-Residual Risk Decomposition


This decomposition introduces the market into risk analysis (see Figure 4-3). This perspective partitions risk into the familiar categories of systematic (market) and residual risk. 

Systematic risk is the component of risk associated with the market portfolio. It is linked to the portfolio beta, which is the weighted average of the portfolio's asset betas. 

Residual risk is the component of risk uncorrelated with the market portfolio. It is further divided into specific and common factor sources. Residual risk can be diversified to a negligible level. 

This type of risk decomposition is the Capital Asset Pricing Model (CAPM) approach. With this approach, you can compare your managed portfolio against a broad-based market portfolio. A benchmark portfolio never comes into play. Risk is partitioned into residual and systematic components, and residual risk is further divided into specific and common factor sources. 

Figure 4-4
Active Risk Decomposition 

This risk decomposition would be most useful to market timers or other managers who “tilt” away from the market portfolio on an opportunistic basis. 


Active Risk Decomposition


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/cbc314b459500f4a3b7dd7e0e327119ca3a5d0d65f692c73cd5ea122485e5a99.jpg)


In this type of decomposition, the concepts of benchmark and active risk are superimposed on the common factor and specific risks itemized in Total Risk Decomposition (see Figure 4-4). 

◆ Benchmark risk is the risk associated with the benchmark portfolio. 

Active risk is the risk that arises from the manager's effort to outperform the benchmark. It is further divided into active specific and active common factor sources. Active risk is also known as tracking error. 

This perspective is most commonly used in analyzing index funds as well as traditionally managed active portfolios. 

In this type of decomposition, there is no concept of a market portfolio. The analysis concentrates solely on the managed portfolio against the benchmark that you select. However, for most managers, market risk is a component of active risk; these managers might 

prefer Active Systematic-Active Residual Risk decomposition, the fourth and last type. 

## Active Systematic-Active Residual Risk Decomposition

Finally, Active Systematic-Active Residual Risk decomposition (see Figure 4-5), the most complete perspective, expands the previous decomposition by including systematic sources of risk. Both this method and Active Risk are helpful in performance evaluation and analysis because they consider the benchmark portfolio, which reveals management style. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/99def208b04b9509a8922dff89c6d7af80a2df5579db1250b09e3ad0ae8016fd.jpg)



Figure 4-5



Active Systematic-Active Residual Risk Decomposition


This risk decomposition is useful for managers who overlay a market-timing strategy on their stock selection process and don't want market risk considerations to affect their analysis. 

## Summary of risk decomposition

These methods of risk decomposition represent compatible perspectives. Figure 4-6 shows how the four methods are different ways to slice the same pie—specific/common factor, systematic/residual, and benchmark/active. 


Figure 4-6
Risk Decomposition Overview


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/634abb6455fb216de57cef0d80a9cb61b1c8b89889de692cd3868aad4f4bbd8d.jpg)


## Performance attribution

Performance attribution completes the portfolio management process by applying the MFM to past portfolio activity. Performance attribution is the process of matching return with its sources. Return is attributed to common factors, market timing, and asset selection. Using benchmark comparisons to judge performance, the value of each investment decision can be determined. 

BARRA's performance attribution programs decompose return into its major components using any of the four methods of risk decomposition listed above. Performance can then be evaluated with respect to customized or industry-standard benchmark portfolios designed to compare managers with their own standards. 

## Summary

In this chapter we have outlined the general management approaches available to equity managers and discussed how BARRA MFMs can be utilized at various stages of the management process. In the next chapter we will describe in detail the process of building an MFM. 

## 5. BARRA Multiple-Factor Modeling

A BARRA equity risk model is the product of a thorough and exact-ing model estimation process. This section provides a brief overview of model estimation. 

## Overview

The creation of a comprehensive equity risk model is an extensive, detailed process of determining the factors that describe asset returns. Model estimation involves a series of intricate steps that is summarized in Figure 5-1. 

The first step in model estimation is acquiring and cleaning data. Both market information (such as price, dividend yield, or capitalization) and fundamental data (such as earnings, sales, or assets) are used. Special attention is paid to capital restructurings and other atypical events to provide for consistent cross-period comparisons. 

Descriptor selection follows. This involves choosing and standardizing variables which best capture the risk characteristics of the assets. To determine which descriptors partition risk in the most effective and efficient way, the descriptors are tested for statistical significance. Useful descriptors often significantly explain cross-sectional returns. 

Risk index formulation and assignment to securities is the fourth step. This process involves collecting descriptors into their most meaningful combinations. Though judgment plays a major role, a variety of techniques are used to evaluate different possibilities. For example, cluster analysis is one statistical tool used to assign descriptors to risk indices. 

Along with risk index exposures, industry allocations are determined for each security. In most BARRA models a single industry exposure is assigned, but multiple exposures for conglomerates are calculated in a few models, including the U.S. and Japan models. 

Next, through cross-sectional regressions, factor returns are calculated and used to estimate covariances between factors, generating the covariance matrix used to forecast risk. Exponential weighting of 

## Figure 5-1

Model Estimation Process 

1. Data acquisition and cleaning 

2. Descriptor selection and testing 

3. Descriptor standardization 

4. Risk index formulation 

5. Industry allocation 

6. Factor return estimation 

7. Covariance matrix calculation:
a. Exponential weighting
b. Market volatility: GARCH 

8. Specific risk forecasting 

9. Model updating 

data observations may be used if testing indicates it improves accuracy. This matrix may be further modified to utilize GARCH techniques. 

Specific returns are separated out at this stage and specific risk is forecast. This is the portion of total risk that is related solely to a particular stock and cannot be accounted for by common factors. The greater an asset's specific risk, the larger the proportion of return attributable to idiosyncratic, rather than common, factors. 

Lastly, the model undergoes final testing and updating. Risk forecasts are tested against alternative models. Tests compare ex ante forecasts with ex post realizations of beta, specific risk, and active risk. New information from company fundamental reports and market data is incorporated, and the covariance matrix is recalculated. 

Figure 5-2 summarizes these steps. 


Phase I: Factor Exposures


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/3c51d77bfc477e9352c8c52983ce19785766de12d91d6ede2eae5a616b8cefdf.jpg)



Figure 5-2


Data Flow for Model Estimation 

This figure depicts the model estimation process. The oval shapes mark the data flow throughout model estimation, while the rectangular shapes show manipulations of and additions to the data. 

## Descriptor selection and testing

Descriptor candidates are drawn from several sources. Market information, such as trading volume, stock prices, and dividends, is available daily. Fundamental company data—such as earnings, assets, and industry information—are derived from quarterly and annual financial statements. For some descriptors, market and fundamental information is combined. An example is the earnings to price ratio, which measures the relationship between the market's valuation of a firm and that firm's earnings. 

Descriptor selection is a largely qualitative process that is subjected to rigorous quantitative testing. First, preliminary descriptors are identified. Good descriptor candidates are individually meaningful; that is, they are based on generally accepted and well-understood asset attributes. Furthermore, they should divide the market into well-defined categories, providing full characterization of the portfolio's important risk features. BARRA has more than two decades of experience identifying important descriptors in equity markets worldwide. This experience informs every new model we build. 

Selected descriptors must have a sound theoretical justification for inclusion in the model. They must be useful in predicting risk and based on timely, accurate, and available data. In other words, each descriptor must add value to the model. If the testing process shows that they do not add predictive power, they are rejected. 

## Normalization

## Descriptor standardization

Normalization is the process of setting random variables to a uniform scale. Also called standardization, it is the process by which a constant (usually the mean) is subtracted from each number to shift all numbers uniformly. Then each number is divided by another constant (usually the standard deviation) to shift the variance. 

The risk indices are composed of descriptors designed to capture all the relevant risk characteristics of a company. The descriptors are first normalized; that is, they are standardized with respect to the estimation universe. This is done to allow combination of descriptors into meaningful risk factors, known as risk indices. The normalization process is summarized by the following relation: 

$$
\left[ \text { normalized   descriptor } \right] = \frac {\left[ \text { raw   descriptor } \right] - \left[ \text { mean } \right]}{\left[ \text { standard   deviation } \right]}
$$

## Risk index formulation

We regress asset returns against industries and descriptors, one descriptor at a time, after the normalization step. Each descriptor is tested for statistical significance. Based on the results of these calculations and tests, descriptors for the model are selected and assigned to risk indices. 

Risk index formulation is an iterative process. After the most significant descriptors are added to the model, remaining descriptors are subjected to stricter testing. At each stage of model estimation, a new descriptor is added only if it adds explanatory power to the model beyond that of industry factors and already-assigned descriptors. 

## Industry allocation

For most BARRA equity models, companies are allocated to single industries. For the U.S. and Japan, however, sufficient data exist to allocate to multiple industries. 

For the U.S. and Japan, industry exposures are allocated using industry segment data (i.e., operating earnings, assets, and sales). The model incorporates the relative importance of each variable in different industries. For example, the most important variable for oil companies would be assets; for retail store chains, sales; and for stable manufacturing companies, earnings. For any given multi-industry allocation, the weights will add up to 100%. 

Multiple industry allocation provides more accurate risk prediction and better describes market conditions and company activity. BARRA's multiple-industry model captures changes in a company's risk profile as soon as new business activity is reported to shareholders. Alternative approaches can require 60 months or more of data to recognize changes that result from market prices. 

## Factor return estimation

The previous steps have defined the exposures of each asset to the factors at the beginning of every period in the estimation window. The factor excess returns over the period are then obtained via a cross-sectional regression of asset excess returns on their associated factor exposures: 

$$
\tilde {r} _ {t} = X _ {t} \tilde {f} _ {t} + u _ {t}\tag{EQ 5-1}
$$

where: 

$$
\tilde {r} _ {t} = \text {excess returns to each asset}
$$

$X_{t} =$ exposure matrix of assets to factors 

$$
\tilde {f} _ {t} = \mathrm{factorreturnstobeestimated}
$$

$$
u _ {t} = \text { specific   returns }
$$

The resulting factor returns are robust estimates which can be used to calculate a factor covariance matrix to be used in the remaining model estimation steps. 

## Covariance matrix calculation

The simplest way to estimate the factor covariance matrix is to compute the sample covariances among the entire set of estimated factor returns. Implicit in this process is the assumption that we are modeling a stable process and, therefore, each point in time contains equally relevant information. 

There is evidence, however, that correlations among factor returns change. Moreover, a stable process implies a stable variance for a well-diversified portfolio with relatively stable exposures to the factors. There is considerable evidence that, in some markets, the volatility of market index portfolios changes. For example, periods of high volatility are often followed by periods of high volatility. The changing correlations among factor returns, and the changing volatility of market portfolios, belie the stability assumption underlying a simple covariance matrix. 

For certain models we relax the assumption of stability in two ways (see Table 5-1 at the end of this chapter for details). First, in computing the covariance among the factor returns, we assign more weight to recent observations relative to observations in the distant past. Second, we estimate a model for the volatility of a market index portfolio—for example, the S&P 500 in the U.S. and the TSE1 in Japan—and scale the factor covariance matrix so that it produces the same volatility forecast for the market portfolio as the model of market volatility. 

## Exponential weighting

Suppose that we think that observations that occurred 60 months ago should receive half the weight of the current observation. Denote by T the current period, and by t any period in the past, $t = 1, 2, 3, \ldots, T-1, T$ , and let $\delta = .5^{1/60}$ . If we assign a weight of $\delta^{T-t}$ to observation t, then an observation that occurred 60 months ago would get half the weight of the current observation, and one that occurred 120 months ago would get one-quarter the weight of the current observation. Thus, our weighting scheme would give exponentially declining weights to observations as they recede in the past. 

Our choice of sixty months was arbitrary in the above example. More generally, we give an observation that is HALF-LIFE months ago one-half the weight of the current observation. Then we let: 

$$
\delta = (. 5) ^ {\frac {1}{H A L F L I F E}}\tag{EQ 5-2}
$$

and assign a weight of: 

$$
w (t) = \delta^ {T - t}.\tag{EQ 5-3}
$$

The length of the HALF-LIFE controls how quickly the factor covariance matrix responds to recent changes in the market relationships between factors. Equal weighting of all observations corresponds to HALF-LIFE = $\infty$ . Too short a HALF-LIFE effectively “throws away” data at the beginning of the series. If the process is perfectly stable, this decreases the precision of the estimates. Our tests show that the best choice of HALF-LIFE varies from country to country. Hence, we use different values of HALF-LIFE for different single country models. 

## Computing market volatility: Extended GARCH models

There is considerable evidence that, in some markets, market volatility changes in a predictable manner. We find that returns that are large in absolute value cluster in time, or that volatility persists. Moreover, periods of above-normal returns are, on average, followed by lower volatility, relative to periods of below-normal returns. Finally, we find that actual asset return distributions exhibit a higher likelihood of extreme outcomes than is predicted by a normal distribution with a constant volatility. 

Variants of GARCH (Generalized Autoregressive Conditional Heteroskedasticity) models capture these empirical regularities by allowing volatility to increase following periods of high realized volatility, or below-normal returns, and allowing volatility to decrease following periods of low realized volatility, or above-normal returns. 

The following discussion lays out the general theory of extended GARCH modeling. Variants of this approach will be applied as appropriate to BARRA single country models over time. See Table 5-1 of this chapter for current coverage. 

Formally, denote by $\tilde{r}_{t}$ the market return at time t, and decompose it into its expected component, $\mathrm{E}\big(\tilde{r}_{t}\big)$ , and a surprise, $\varepsilon_{t}$ : 

$$
\tilde {r} _ {t} = \mathrm{E} (\tilde {r} _ {t}) + \varepsilon_ {t}\tag{EQ 5-4}
$$

The observed persistence in realized volatility indicates that the variance of the market return at t, $Var(\tilde{r}_{m})_{t}$ , can be modeled as: 

$$
V a r \big (\tilde {r} _ {m} \big) _ {t} = \omega + \alpha \varepsilon_ {t - 1} ^ {2} + \beta V a r \big (\tilde {r} _ {m} \big) _ {t - 1}\tag{EQ 5-5}
$$

This equation, which is referred to as a GARCH(1,1) model, says that current market volatility depends on recent realized volatility via $\varepsilon_{t-1}^2$ , and on recent forecasts of volatility via $Var(\tilde{r}_m)_{t-1}$ . If $\alpha$ and $\beta$ are positive, then this period's volatility increases with recent realized and forecast volatility. 

GARCH(1,1) models have been found to fit many financial time series. Nevertheless, they fail to capture relatively higher volatility following periods of below-normal returns. We can readily extend the GARCH(1,1) model to remedy this shortcoming by modeling market volatility as: 

$$
\operatorname{Var} \left(\tilde {r} _ {m}\right) _ {t} = \omega + \alpha \varepsilon_ {t - 1} ^ {2} + \beta \operatorname{Var} \left(\tilde {r} _ {m}\right) _ {t - 1} + \theta \varepsilon_ {t - 1}\tag{EQ 5-6}
$$

If $\theta$ is negative, then returns that are larger than expected are followed by periods of lower volatility, whereas returns that are smaller than expected are followed by higher volatility. 

Having satisfactorily fit a GARCH model to the volatility of a market proxy portfolio, it is used to scale the factor covariance matrix so that the matrix gives the same risk forecast for the market portfolio as the GARCH model. In implementing the scaling, however, we scale only the systematic part of the factor covariance matrix. 

## Specific risk modeling

## Overview

Referring to the basic factor model: 

$$
\tilde {r} _ {i} = \sum_ {k} X _ {i k} \tilde {f} _ {k} + \tilde {u} _ {i}\tag{EQ 5-7}
$$

The specific risk of asset i is the standard deviation of its specific return, $Std(\tilde{u}_{i})$ . The simplest way to estimate the specific risk matrix is to compute the historical variances of the specific returns. This, however, assumes that the specific return distribution is stable over time. Rather than use historical estimates, we model specific risk to capture fluctuations in the general level of specific risk and the relationship between specific risk and asset fundamental characteristics. 

An asset's specific risk is the product of the average level of specific risk that month across assets, and each asset's specific risk relative to the average level of specific risk. Moreover, our research has shown that the relative specific risk of an asset is related to the asset's fundamentals. Thus, developing an accurate specific risk model involves a model of the average level of specific risk across assets, and a model that relates each asset's relative specific risk to the asset's fundamental characteristics. 

## Methodology

Denote by $S_{t}$ the average level of specific risk across assets at time t, and by $V_{it}$ asset i's specific risk relative to the average. 

In equation form: 

$$
\operatorname{Std} \left(\tilde {u} _ {i t}\right) = S _ {t} \left(1 + V _ {i t}\right)\tag{EQ 5-8}
$$

where: 

$$
\operatorname{Std} \left(\tilde {u} _ {i t}\right) = \text { asset   specific   risk },
$$

$S_{t}$ = average level of specific risk at time t, and 

$V_{it}$ = asset i's specific risk relative to the average. 

We estimate a model for $S_{t}$ via time-series analysis, in which the average level of realized specific risk is related to its lagged values and to lagged market returns. Similarly, we estimate a model of relative specific risk by regressing realized relative specific risks of all firms, across all periods, on the firm fundamentals, which include the BARRA risk factors. 

## Modeling the average level of specific risk

We model the average level of specific risk via a time series model, where the average specific risk is related to its own lagged values, as well as to lagged market excess returns: 

$$
S _ {t} = \alpha + \sum_ {i = 1, k} \beta_ {i} S _ {t - i} + \beta_ {k + 1} r _ {m _ {t - 1}} + \varepsilon_ {t}\tag{EQ 5-9}
$$

where: 

$S_{t}$ = average specific risk at time t, 

$\alpha$ = expected level of average specific risk across assets, 

$\beta_{i}$ = sensitivity of average specific risk to lagged values, 

$S_{t - i} =$ lagged average specific risk, 

$\beta_{k+1}=$ sensitivity of average specific risk to market returns, 

$$
r _ {m _ {t - 1}} = \text {   market   return   at   time   } t \text {-} 1, \text {   and   }
$$

$\varepsilon_{t}$ = residual level of specific risk. 

This simple model captures mean reversion or trends and persistence in volatility, as well as lower average specific risk following market rises, and higher specific risk following market declines (provided $\beta_{k+1}$ is negative). We evaluate the performance of alternative weighting schemes by regressing realized average specific risk against predicted specific risk out of sample: 

$$
S _ {t} = a + b \S_ {t} + e _ {t}\tag{EQ 5-10}
$$

The results of these tests help us determine the appropriate coefficients in Equation 5-9. 

## Modeling the relative level of specific risk

To model the relative level of specific risk, we first identify factors that may account for the variation in specific risk among assets. These factors will vary depending on the country model and may include: 

■ Industry membership 

■ Risk index exposures 

Having identified these factors, we then estimate the relationship by performing the “pooled” cross-sectional regression: 

$$
V _ {i t} = \sum_ {k = 1, K} X _ {i k t} \gamma_ {k} + e _ {i t}\tag{EQ 5-11}
$$

where: 

$V_{it}$ = relative specific risk for asset i at time t, 

$$
t = 1 \text {   to   } T \text {   months, }
$$

i = 1 to N assets, 

$X_{ikt} = \text{the exposure of asset } i \text{ to factor } k \text{ at time } t, \text{ and}$ 

$\gamma_{k}$ = factor k's contribution to relative specific risk. 

In estimating this relationship, we mitigate the effects of outliers on the estimators by Windsorizing descriptors and risk indices. 

## Estimating the scaling coefficients

Average specific risk can vary widely over the full capitalization range of an equity market. To correct for this effect, scaling coefficients are used to adjust for any specific risk bias. To estimate the scaling coefficients, we divide the set of securities into capitalization deciles and, for each decile, we compute the bias in predicted specific risk from the previous steps. The scaling coefficients are then computed as a piece-wise linear function of an asset's relative capitalization in a manner that makes the average bias in predicted specific risk zero for each capitalization decile. 

## Final specific risk forecast

The above three components—average level of specific risk, relative level of specific risk, and decile scaling coefficients—are combined to produce the final asset specific risk forecast: 

$$
S t d (\varepsilon_ {i t}) = s c a l e _ {i t} \cdot \hat {S} _ {t} \cdot (1 + \hat {V} _ {i t})\tag{EQ 5-12}
$$

where: 

$\varepsilon_{it} =$ specific risk of asset $i$ at time $t$ , 

$scale_{it}=$ scale coefficient for the decile that asset i falls into at time t, 

$t$ = average level of specific risk across all assets, and 

$\hat{V}_{it}$ = relative level of specific risk for asset $i$ at time $t$ . 

## Updating the model

Model updating is a process whereby the most recent fundamental and market data are used to calculate individual stock exposures to the factors, to estimate the latest month's factor returns, and to recompute the covariance matrix. 

The latest data are collected and cleaned. Descriptor values for each company in the database are computed, along with risk index exposures and industry allocations. Next, a cross-sectional regression is run on the asset returns for the previous month. This generates factor returns which are used to update the covariance matrix. Finally, this updated information is distributed to users of BARRA's applications software. 

## Comparison of risk model features

Table 5-1 summarizes BARRA's single country equity models and the features of each as of January 1998. 

<table><tr><td>Country Model</td><td>Number of Industries</td><td>Number of Risk Indices</td><td>Industry Allocation Method: Multiple/Single</td><td>Exponential Smoothing Half-Life: Number of Months</td><td>GARCH: Yes/No</td></tr><tr><td>Australia (AUE2)</td><td>24</td><td>9</td><td>Single</td><td>90</td><td>No</td></tr><tr><td>Canada (CNE3)</td><td>40</td><td>11</td><td>Single</td><td>60</td><td>No</td></tr><tr><td>France (FRE3)</td><td>12</td><td>9</td><td>Single</td><td>48</td><td>No</td></tr><tr><td>Germany (GRE2)</td><td>17</td><td>10</td><td>Single</td><td>90</td><td>No</td></tr><tr><td>Germany—Trading Model (GRTM)</td><td>17</td><td>10</td><td>Single</td><td>90</td><td>Yes</td></tr><tr><td>Hong Kong (HKE1)</td><td>13</td><td>10</td><td>Single</td><td>48</td><td>No</td></tr><tr><td>Japan (JPE2)</td><td>40</td><td>12</td><td>Multiple</td><td>60</td><td>Yes</td></tr><tr><td>Korea (KRE1)</td><td>28</td><td>12</td><td>Single</td><td>24</td><td>No</td></tr><tr><td>Malaysia (MLE1)</td><td>14</td><td>10</td><td>Single</td><td>36</td><td>No</td></tr><tr><td>Netherlands (NLE1)</td><td>8</td><td>7</td><td>Single</td><td>60</td><td>No</td></tr><tr><td>New Zealand (NZE1)</td><td>6</td><td>5</td><td>Single</td><td>48</td><td>Yes</td></tr><tr><td>South Africa (SAE1)</td><td>23</td><td>11</td><td>Single</td><td>36</td><td>No</td></tr><tr><td>Sweden (SNE3)</td><td>20</td><td>10</td><td>Single</td><td>90</td><td>Yes</td></tr><tr><td>Switzerland (SWE2)</td><td>12</td><td>8</td><td>Single</td><td>90</td><td>No</td></tr><tr><td>Taiwan (TWE1)</td><td>25</td><td>10</td><td>Single</td><td>36</td><td>No</td></tr><tr><td>Thailand (THE1)</td><td>32</td><td>9</td><td>Single</td><td>36</td><td>No</td></tr><tr><td>U.K. (UKE5)</td><td>38</td><td>12</td><td>Single</td><td>90</td><td>No</td></tr><tr><td>U.K.—Trading Model (UKTM)</td><td>38</td><td>12</td><td>Single</td><td>90</td><td>Yes</td></tr><tr><td>U.S. (USE2)</td><td>55</td><td>13</td><td>Multiple</td><td>90</td><td>Yes</td></tr><tr><td>U.S. (USE3)</td><td>52</td><td>13</td><td>Multiple</td><td>90</td><td>Yes</td></tr><tr><td>U.S.—Small Cap (USSC)</td><td>42</td><td>11</td><td>Single</td><td>90</td><td>No</td></tr><tr><td>U.S.—Short-Term Risk (STRM)</td><td>55</td><td>3</td><td>Multiple</td><td>40 trading days</td><td>Yes</td></tr></table>

Table 5-1 BARRA Single Country Equity Risk Models $^{*}$ † 

## 6. Advantages of US-E3 Over US-E2

## Overview

The original BARRA product was a U.S. equity risk model, developed in 1975. Dubbed US-E1, it was superseded by a second-generation model, US-E2, in the early 1980s. US-E2 has served BARRA clients well over the last 18 years, but we identified a variety of deficiencies which made a significant upgrade desirable. The improvements that have been implemented in the U.S. Equity Model Version 3 (US-E3) cumulatively result in a demonstrably better model, both in terms of qualitative features and quantitative measures. 

Highlights of US-E3's advances over US-E2: 

■ complete industry reclassification 

■ flexible industries 

■ larger estimation universe 

■ addition of Size Nonlinearity risk index 

■ improved independence between risk indices 

■ improved specific risk model 

■ improved GARCH model 

■ calculation of REIT risk index exposures 

■ higher t-stats in general 

■ improved data quality assurance 

■ improved model diagnostics 

■ annual re-estimation of specific risk, GARCH, and descriptor weight parameters 

## Industries

## Reclassification

Experience from US-E2, client input, and the changing nature of the market led to a complete reconsideration of BARRA's industry classification. Once we decided upon a revised set of industries, we performed a company-by-company review of available tear sheets for all assets in the US-E2 estimation universe (the HICAP) by at least two people. Even if US-E2 and US-E3 industries mapped one-to-one or many-to-one, assets may have moved to other US-E3 industries if tear sheet review indicated they had been misclassified within US-E2. 

Here are some highlighted differences between US-E2 and US-E3 classification schemes: 

■ US-E3 does not have a Miscellaneous industry, as US-E2 does. All assets must now be assigned to specific industries. 

US-E2's five oil-related industries have been collapsed into three industries for US-E3, to reflect the massive changes in this segment since the early 1980s. 

■ US-E2's Services was a catchall industry. US-E3 has Information Services (more high-tech services) and Industrial Services (more low-tech types of industrial services). Also, software companies lumped into US-E2 Services are now in their own industry, Computer Software. 

■ US-E2's Aluminum, Coal & Uranium, and Iron & Steel have been combined into US-E3's Mining & Metals. 

■ US-E2's Forest Products and Paper are a single industry for US-E3. 

■ Photography is not a US-E3 industry. 

■ Containers is not a US-E3 industry. 

■ US-E3 has added the industries Entertainment, Semiconductors, Computer Software, Wireless Telecommunications, and Securities & Asset Management. 

■ US-E3 industries distinguish between Medical Providers & Services and Medical Products. 

## Flexible industries

This is a major advance in US-E3. BARRA risk models have historically had great difficulty adding or subtracting industries. US-E3 assigns industries to assets based on 82 mini-industries. This mini-industry classification has been performed historically for each asset from January 1975 to the present. This allows us to watch for an increase in assets in a given mini-industry. Once a minimum threshold has been reached, the mini-industry can be promoted to industry status if it appears appropriate. By “appropriate” we mean that either (a) there are statistical reasons for estimating the mini-industry separately; and/or (b) there is market/client differentiation which makes the mini-industry ripe for industry classification. Some element of judgment will be exercised here in consultation with our clients. 

We will also be monitoring the decline of assets within existing industries. Too few for too long will trigger an extinction of the industry. A situation similar to Coal & Uranium (which currently has no assets in the HICAP with this as primary industry) will not occur in US-E3. 

US-E3 performance analysis (as implemented in BARRA's Windows-based Aegis System) will be able to handle these rising and falling industries. Each industry will be assigned to one of 13 permanent economic sectors which will maintain continuity for all assets even as their industries change. 

## Increased size of the estimation universe

US-E3 has increased the size of its estimation universe by roughly 50%. This means that more of the midsize companies (those approximately 1,001–2,000 in capitalization rank) are participating in calculation of the factor returns. Since a greater number of BARRA clients are investing in such companies, this is a desirable feature. 

We extended the estimation universe only after we determined that (a) coverage of the descriptors used for risk index calculation would not deteriorate and (b) the factor returns would not change “too much” by the addition of lower-capitalization assets. 

## Risk indices

In general, US-E3 has pared down the total number of descriptors used for risk index construction. This has been done in order to reduce the number of descriptors used within each risk index so that only the most significant data are used and to remove overlaps which occurred in US-E2. 

## Size Nonlinearity factor

This is the most novel addition to the risk indices. Internal research has shown that US-E2, while doing a good job of risk forecasting of the top 500–750 capitalization assets, was systematically underpredicting risk for smaller capitalization assets. In other words, size has a nonlinear risk component. With the increase of the estimation universe to roughly the top 1,500 capitalization assets, this becomes even more of an issue. US-E3 uses a polynomial model to approximate this nonlinearity within the context of a linear model. The result is superior risk forecasts for assets and portfolios over the entire range of size-sorted portfolios. 

## Leverage

US-E3 calculates the Leverage exposure in the same fashion across all industries. US-E2 used (a) interest rate sensitivity for financial, utility, and railroad industries and (b) fundamental-based descriptors for all other industries. It is not a good idea to combine two different calculations under the same umbrella; for instance, there is no non-arbitrary way to normalize them. We also found that there was no need to treat this index differently for different industries; it did not capture any added nuances. 

## Simpler volatility calculation

US-E2 uses a three-tiered method of computing the Variability in Markets risk index (which is the counterpart of US-E3's Volatility). Different descriptors and weights were used within each of US-E2's tiers. The tiers are based on: assets with options, HICAP assets without options, and all other assets. Historically, assets have jumped tiers, which resulted in noticeable and non-intuitive changes in Variability in Markets exposures from month to month. 

US-E3 will not duplicate the three-tiered method of US-E2. Research during the development of US-E3 found no evidence to indicate that this “tiering” is necessary for providing accurate risk forecasts. Using a single set of core descriptors in addition to Option-Implied Standard Deviation (where appropriate), US-E3 achieves higher explanatory power than the US-E2 methodology. 

## Elimination of US-E2's Labor Intensity and Foreign Income

Although the motivation behind these risk indices is intuitive, coverage of data necessary for these risk indices is decidedly lower than for other risk indices. Since no substitute could be identified for Labor Intensity, we eliminated it. 

US-E3's Currency Sensitivity differs from US-E2's Foreign Income through the use of a regression technique to determine directly the effect of currency fluctuations on asset returns. This implied sensitivity to foreign operations avoids the need to find fundamental data describing this effect and was found in our testing to be robust. 

## Improved independence between risk indices

In US-E2 several risk indices shared the same descriptors. This resulted in a certain amount of unnecessary multicollinearity—most notably related to Growth, Yield, and Earnings/Price. US-E3 risk indices consist of separate sets of descriptors for each risk index. The model benefits from this through more precise factor returns estimates (smaller standard errors, higher t-stats) which results in more precise common factor covariance matrix estimation. 

## Risk forecasting

There are two sources of US-E3's improvement in risk forecasting: 

## Improved GARCH model

The extended GARCH(1,1) model provides for a more accurate risk forecast of overall market volatility. It responds appropriately to observed asymmetry in market volatility related to up market moves and down market moves. For additional details, see Chapter 5. BARRA Multiple-Factor Modeling. 

## Specific risk model

US-E3 builds its specific risk model based on two risk forecasts: market average specific risk and relative specific risk. US-E2 builds its model based only on relative specific risk. This will make US-E3's specific risk predictions more accurate. See Chapter 5. BARRA Multiple-Factor Modeling for details. 

## Model fit-related issues

## Factor return estimation

Even though the R-squared for the monthly factor return regressions are virtually the same for US-E2 and US-E3, the new industry classification and risk index modeling has resulted in more precise factor return estimates (which are reflected in increased t-statistics for the estimated factor returns). More precise factor return estimates provide better data for common factor risk forecasts. 

## Ongoing diagnostics

US-E3 will collect and save the set of information used in model-building each month as the model moves forward in time. This means BARRA can reassess modeling issues by simply examining this database, rather than having to redo historic estimations in the future. This makes it feasible to re-estimate model-related parameters (such as descriptor weights within risk indices and GARCH parameters) much faster. 

## Scheduled refitting of model parameters

US-E2 has always used the same weights for descriptors. The same is true for the parameters of the specific risk model. The US-E2 GARCH parameters have never been re-estimated. US-E3 will refit these models on a yearly or biyearly schedule. This will assure that the model responds to changes in the market. It will also provide an ongoing assessment of our modeling technique's true (live mode) out-of-sample performance. 

## Asset class issues

## REITs

Most of the REITs in US-E2 have "0" for all of their risk index exposures except LOCAP. US-E3 calculates risk index exposures for its REITs. US-E3 also does a better job of separating the property REITs from the mortgage REITs. 

## Coming soon

After the release of US-E3 we will conduct extensive research into the modeling of mutual funds, bonds, preferred stock, SPIDERs, ADRs, IPOs, and other asset classes. 

## 7. The US-E3 Estimation Universe

## Overview

The primary attribute determining an asset's inclusion in the US-E3 estimation universe is its capitalization. The top 1,500 assets by capitalization comprise the heart of the monthly estimation universe. Additional assets are added to ensure depth within industries. This has resulted in a final universe size of around 1,900, which will fluctuate from month to month. Only U.S. stocks with Compustat data are considered. Any asset which drops below the capitalization cut-off will be given a grace period of 18 months before it is dropped from the estimation universe. 

## Selection process

There are six considerations involved: 

1. S&P 500 membership 

2. Compustat data present 

3. Capitalization 

4. Industry fill-in 

5. Price 

6. Grandfathering 

The above considerations apply only to “plain vanilla” U.S. stocks. No REITs, ADRs, closed-end funds, etc. will be considered for inclusion in the estimation universe. The only possible exception here is in the case of S&P 500 membership. We will include any type of asset that is in the S&P 500, as long as we have assigned an industry to it. Considering only plain stocks for estimation universe membership ensures having the necessary industry assignments. 

## 1. S&P 500 membership

All assets in the S&P 500 will be included in the estimation universe, even if other rules discussed below are violated. The capitalization and price considerations that follow do not apply to these assets. 

## 2. Compustat data present

Since so many of the descriptors we need come from Compustat data, we do not want to select assets for our estimation universe when we know we will have to resort to replacement rules for all of the descriptors for those assets. Accordingly, we will use only assets that have annual Compustat data within at most 21 months from the model update. 

## 3. Capitalization

We will automatically include the top 1,500 stocks. No ADRs will be included unless they are part of the S&P 500. 

## 4. Minimum price

This will be applied only to assets that are selected for industry fill-in (described in the next step). No asset less than \$5.00 per share will be included unless it falls under 1. or 3. above. 

## 5. Industry fill-in

There should be at least 20 assets in each industry, if possible. After collecting the top 1,500 assets, we will determine which industries are thin. Each industry will be filled in, searching from the highest remaining capitalization assets in descending order, until there are 20 assets within the thin industries. It may not be possible to obtain all the assets we want. To avoid including companies that are too small, we will exclude from consideration any asset in the lowest 10% of capitalization. 

## 6. Grandfathering

Assets that are near the top 1,500 capitalization cutoff bounce in and out of the estimation universe from month to month. If this were allowed, their risk forecasts would bounce as well, since their Non-Estimation Universe (NONESTU) exposure would be changing. We will minimize this by allowing an 18-month grace period. If an asset was in the estimation universe by virtue of either 1., 3., or 5. above and drops out due to falling market capitalization, the asset will drop out of the estimation universe after 18 months unless it recovers to the cutoff during that time. This will minimize the associated jumps in risk forecasts. 

Even grandfathered assets must pass the minimum price condition and bottom 10th percentile in capitalization condition. 

This methodology requires keeping a time series database of assets that were part of the estimation universe based on contemporaneous considerations. 

## Comparison with the US-E2 estimation universe

In general, most of the US-E2 HICAP is included in US-E3's estimation universe. Differences between the two universes arise principally from the following: 

1. US-E3 takes the top 1,500 capitalization assets as its starting point. In US-E2, the HICAP takes the top 1,000 assets as its starting point. US-E3, therefore, is letting a larger number of assets participate in the estimation of industry and risk index factor returns. Studies addressing the effect of expanding the size of the estimation universe with respect to deterioration of coverage of descriptors and the resulting factor returns led to the selection of the number 1,500. 

2. The grandfathering and the monthly quest for industry depth have not been done in a consistent manner for US-E2. By following a rules-based process as described above, we will improve consistency. 

3. US-E2 has some very small assets in the HICAP. The bottom tenth percentile rule for US-E3 prevents this. 

## 8. US-E3 Risk Indices and Descriptors

## Differences between US-E2 and US-E3 risk indices

## General differences

In US-E2, there are a number of instances of the same descriptor appearing in more than one risk index. For example, descriptors relating earnings to price comprise part of the Growth risk index as well as the estimated Earnings-to-Price Ratio risk index, share turnover ratios appear in the Trading Activity risk index as well as the Variability in Markets risk index for some companies, and Dividend Yield is a separate risk index as well as a part of the Growth risk index. In some cases—for example, Yield and Growth—this leads to correlated exposures resulting in lower precision for the estimates of factor returns corresponding to these factors. To avoid highly correlated risk index exposures in US-E3, we decided to assign each descriptor to a single risk index. For most descriptors, the risk indices that they belonged to was fairly obvious; for the not-so-obvious cases, we assigned descriptors to risk indices based on a study we conducted. 

## Specific differences

Specific differences between US-E2 and US-E3 risk indices are as follows: 

## Volatility

In US-E2, this risk index has a three-tiered structure, with different ways of constructing this risk index for optioned stocks, other exchange-traded stocks, and thinly traded stocks. In US-E3, this risk index is constructed using a single rule for all stocks. For stocks that have options, option-implied standard deviation is computed using the Black-Scholes formula. For stocks without options, the option-implied standard deviation descriptor is treated as missing, and a replacement rule is used to estimate the descriptor value. 

## Size

In US-E2, the Size risk index is constructed using a weighted sum of the log of market capitalization and the log of total assets of the company. In contrast, US-E3 measures size exposure using simply the log of market capitalization. This measure of size exposure is consistent with the well-documented “size effect,” the term used by academics to refer to the strong linear relationship between average returns and log of market capitalization over many time periods. 

## Size Nonlinearity (US-E3)

This is a new risk index in US-E3 and does not appear in US-E2. The estimation universe in US-E3 consists of the top 1,500 stocks ranked by capitalization plus smaller companies chosen to ensure a reasonable number of companies in each industry. Our research showed that the linear relationship between the cross-section of returns and log of market capitalization is a good approximation for larger companies (especially in the top 500-750 range). For smaller companies, our research showed that there are some non-linearities in the relation between returns and log of market capitalization. The Size Nonlinearity risk index ensures that the US-E3 model does a good job of capturing the relationship between returns and size for all companies, not just the larger ones. 

## Growth

In US-E2, this risk index is a combination of historical earnings and asset growth, historical payout ratios, analyst-predicted growth, earnings-to-price, and dividend yield variables. The weights of each descriptor were based on a predictive model for five-year-ahead earnings growth. In US-E3, this risk index is a combination of historical earnings and asset growth, historical payout ratios, and analyst-predicted earnings growth. Earnings yield and dividend yield variables do not appear in the Growth risk index in US-E3. The weights of each descriptor are based on a predictive model for three-year-ahead sales growth. We estimated other predictive models for five-year-ahead sales growth and five-year-ahead earnings growth. The three-year sales growth model that we estimated provided the most intuitive set of weights, had the best in-sample fit, had good out-of-sample properties, and explained the cross-section of returns well. 

## Financial Leverage (US-E2) and Leverage (US-E3)

In US-E2, this risk index is constructed differently for companies in finance-related industries, railroads, and utilities. For companies in these industries, a market-based interest-rate-sensitivity measure is used to measure the exposure to the leverage factor. In contrast, US-E3 uses the same rule, based on the usual measures of book leverage, market leverage, etc., for all companies. Intuition suggests that the usual measures of leverage for companies in finance-related industries and utilities are likely to be very high, leading to clustering of such companies at the high end of the leverage spectrum. However, this intuition is not borne out by inspection of the data. In most cases, our research found that these companies have leverage values comparable with other companies, so the usual measures of leverage can be used as measures of exposure to the Leverage factor. 

## Foreign Income (US-E2) and Currency Sensitivity (US-E3)

In US-E2, this risk index is constructed as the proportion of operating income of a company that arises from non-domestic sources. Many companies do not report their operating income by geographic regions, so US-E2 uses replacement rules to fill in values for companies that do not report this information. Data coverage for this information has been a persistent problem for US-E2. In addition, US-E2 did not account for any currency hedging. To avoid these problems, US-E3 has adopted a different measure of non-domestic risk based on currency exchange rate returns. This measure is a regression-based sensitivity of asset returns to exchange rate returns, and was shown in our tests to be robust. 

## Labor Intensity (US-E2)

In US-E2, this risk index uses descriptors based on labor expenses, total assets, net plant and gross plant of a company. A large number of companies do not report labor expenses as a separate item in their financial statements. This leads to the use of a replacement rule for the descriptor based on labor expenses. A related issue is that over the history of the US-E2 model, the Labor Intensity risk index appears to be only marginally significant. We therefore decided to drop the Labor Intensity risk index in US-E3. 

## US-E3 and US-E2 risk indices at a glance

The table below displays US-E3 and US-E2 risk index information in a concise form. Each US-E3 risk index is paired with its most-closely-associated counterpart in US-E2, and a list of descriptors that make up each risk index is provided. US-E2 descriptors that appear with a strikethrough (for example, log of total assets) are those that are dropped from the corresponding US-E3 risk index. Such descriptors may still be a part of some other risk index in US-E3 or may have been dropped from the model. US-E3 descriptors that appear in a shaded box are new descriptors not present in US-E2. 

<table><tr><td>Descriptors in US-E3 Risk Index</td><td>US-E3 Risk Index</td><td>US-E2 Risk Index</td><td>Descriptors in US-E2 Risk Index</td></tr><tr><td>Beta times sigma</td><td>Volatility</td><td>Variability in MarketsNote: This is a three-tiered risk index in US-E2. The descriptors shown at right appear in at least one of the &quot;tiers.&quot;</td><td>Beta times sigma</td></tr><tr><td>Daily standard deviation</td><td></td><td></td><td>Daily standard deviation</td></tr><tr><td>High-low price</td><td></td><td></td><td>Log of stock price</td></tr><tr><td>Log of stock price</td><td></td><td></td><td>Cumulative range</td></tr><tr><td>Cumulative range</td><td></td><td></td><td>Serial dependence</td></tr><tr><td>Volume beta</td><td></td><td></td><td>Option-implied standard deviation</td></tr><tr><td>Serial dependence</td><td></td><td></td><td>Volume to variance</td></tr><tr><td>Option-implied standard deviation</td><td></td><td></td><td>Share turnover rate (annual)</td></tr><tr><td>Relative strengthHistorical alpha</td><td>Momentum</td><td>Success</td><td>Relative strengthHistorical alphaDividend cuts over the last five yearsRecent earnings changeAnalyst-predicted earnings growthGrowth in earnings per share</td></tr><tr><td>Log of market capitalization</td><td>Size</td><td>Size</td><td>Log of market capitalizationLog of total assetsIndicator of earnings history</td></tr><tr><td>Cube of log of market capitalization</td><td>Size Nonlinearity</td><td></td><td></td></tr></table>


Table 8-1 



US-E3 and US-E2 Risk Indices 


<table><tr><td>Descriptors in US-E3 Risk Index</td><td>US-E3 Risk Index</td><td>US-E2 Risk Index</td><td>Descriptors in US-E2 Risk Index</td></tr><tr><td>Share turnover rate (annual)</td><td>Trading Activity</td><td>Trading Activity</td><td>Share turnover rate (annual)</td></tr><tr><td>Share turnover rate (quarterly)</td><td></td><td></td><td>Share turnover rate (quarterly)</td></tr><tr><td>Share turnover rate (monthly)</td><td></td><td></td><td>Share turnover rate (five years)</td></tr><tr><td>Share turnover rate (five years)</td><td></td><td></td><td>Number of analysts</td></tr><tr><td>Indicator for forward split</td><td></td><td></td><td>Volume to variance</td></tr><tr><td>Volume to variance</td><td></td><td></td><td></td></tr><tr><td>Payout ratio over five years</td><td>Growth</td><td>Growth</td><td>Payout ratio over five years</td></tr><tr><td>Variability in capital structure</td><td></td><td></td><td>Variability in capital structure</td></tr><tr><td>Growth rate in total assets</td><td></td><td></td><td>Growth rate in total assets</td></tr><tr><td>Earnings growth rate over the last five years</td><td></td><td></td><td>Earnings growth rate over the last five years</td></tr><tr><td>Analyst-predicted earnings growth</td><td></td><td></td><td>Analyst-predicted earnings growth</td></tr><tr><td>Recent earnings change</td><td></td><td></td><td>Recent earnings change</td></tr><tr><td></td><td></td><td></td><td>Earnings-to-price ratio (five years)</td></tr><tr><td></td><td></td><td></td><td>Normalized earnings-to-price ratio</td></tr><tr><td></td><td></td><td></td><td>Dividend yield (five years)</td></tr><tr><td></td><td></td><td></td><td>Yield forecast</td></tr><tr><td></td><td></td><td></td><td>Indicator of zero yield</td></tr><tr><td></td><td></td><td></td><td>Earnings-to-price ratio</td></tr><tr><td></td><td></td><td></td><td>Analyst-predicted earnings-to-price ratio</td></tr><tr><td>Analyst-predicted earnings-to-price</td><td>Earnings Yield</td><td>Earnings-to-Price Ratio</td><td>Analyst-predicted earnings-to-price</td></tr></table>


Table 8-1 


US-E3 and US-E2 Risk Indices 

<table><tr><td>Descriptors in US-E3 Risk Index</td><td>US-E3 Risk Index</td><td>US-E2 Risk Index</td><td>Descriptors in US-E2 Risk Index</td></tr><tr><td>Trailing annual earnings-to-price</td><td></td><td></td><td>Earnings-to-price</td></tr><tr><td>Historical earnings-to-price</td><td></td><td></td><td>Historical earnings-to-price</td></tr><tr><td>Book-to-price ratio</td><td>Value</td><td>Book-to-Price Ratio</td><td>Book-to-price ratio</td></tr><tr><td>Variability in earnings</td><td>Earnings Variability</td><td>Earnings Variability</td><td>Variability in earnings</td></tr><tr><td>Variability in cash flows</td><td></td><td></td><td>Variability in cash flows</td></tr><tr><td>Extraordinary items in earnings</td><td></td><td></td><td>Extraordinary items in earnings</td></tr><tr><td>Standard deviation of analyst-predicted earnings-to-price</td><td></td><td></td><td>Standard deviation of analyst-predicted earnings-to-price</td></tr><tr><td></td><td></td><td></td><td>Earnings covariabilityConcentration</td></tr><tr><td>Market leverage</td><td>Leverage</td><td>Financial Leverage</td><td>Book leverage</td></tr><tr><td>Book leverage</td><td></td><td>Note: For finance-related industries, utilities, and railroads, this risk index is constructed using a measure of bond market sensitivity.</td><td>Debt to total assets</td></tr><tr><td>Debt to total assets</td><td></td><td></td><td>Uncovered fixed-charges</td></tr><tr><td></td><td></td><td></td><td>Bond market sensitivity</td></tr><tr><td>Senior debt rating</td><td></td><td></td><td></td></tr><tr><td>Exposure to foreign currencies</td><td>Currency Sensitivity</td><td></td><td></td></tr><tr><td></td><td></td><td>Foreign Income</td><td>Proportion of operating income from foreign-sources</td></tr><tr><td></td><td></td><td>Labor Income</td><td>Labor shareInflation-adjusted plant-to-equityNet plant-to-gross plant</td></tr><tr><td>Predicted dividend yield</td><td>Dividend Yield</td><td>Yield</td><td>Predicted dividend yield</td></tr><tr><td>Indicator for firms outside US-E3 estimation universe</td><td>Non-Estimation Universe Indicator</td><td>LOCAP Indicator</td><td>Indicator for firms outside US-E2 HICAP universe</td></tr></table>


Table 8-1 


US-E3 and US-E2 Risk Indices 

## Risk index definitions

## 1. Volatility

This risk index captures relative volatility using measures of both long-term historical volatility (such as historical residual standard deviation) and near-term volatility (such as high-low price ratio, daily standard deviation, and cumulative range over the last 12 months). Other proxies for volatility (log of stock price), corrections for thin trading (serial dependence), and changes in volatility (volume beta) are also included in this descriptor. 

## 2. Momentum

This risk index captures common variation in returns related to recent stock price behavior. Stocks that had positive excess returns in the recent past are grouped separately from those that displayed negative excess returns. 

## 3. Size

This risk index captures differences in stock returns due to differences in the market capitalization of companies. 

## 4. Size Nonlinearity

This risk index captures deviations from linearity in the relationship between returns and log of market capitalization. 

## 5. Trading Activity

This risk index measures the amount of relative trading in each stock. Stocks that are highly traded are likely to be those with greater institutional interest. Such stocks may display different returns behavior compared with those that are not widely held by institutions. 

## 6. Growth

This risk index uses historical growth and profitability measures to predict future earnings growth. 

## 7. Earnings Yield

This risk index combines current and historical earnings-to-price ratios with a measure of analyst-predicted earnings-to-price. Stocks with similar values of earnings yield behave in a similar fashion with respect to their returns. 

## 8. Value

This risk index distinguishes between value stocks and growth stocks using the ratio of book value of equity to market capitalization. 

## 9. Earnings Variability

This risk index measures the variability in earnings and cash flows using both historical measures and analyst predictions. 

## 10. Leverage

This risk index measures the financial leverage of a company. 

## 11. Currency Sensitivity

This risk index measures the sensitivity of a company's stock return to the return on a basket of foreign currencies. 

## 12. Dividend Yield

This risk index computes a measure of predicted dividend yield using the past history of dividends and the market price behavior of the stock. 

## 13. Non-Estimation Universe Indicator

This risk index flags companies outside the estimation universe. It allows the linear factor model to be extended to stocks outside the US-E3 estimation universe. 

## Descriptor definitions

See Appendix A for a full set of descriptor definitions. 

## 9. US-E3 Industries

## Overview

The industry component of the US-E3 model consists of two parts: 

■ the industry classification scheme (all new for US-E3) 

■ the industry weights for assets participating in multiple industries (essentially the same as US-E2) 

There are 52 industries in the US-E3 classification scheme. The set of industries used is the result of client input and extensive BARRA research. The industry classification scheme used by US-E2, although adequate in many respects, does not capture many relevant features of the current U.S. market. Notable examples are the absence of the software and cellular industries. US-E3 has been constructed to allow for an organic birth/death of industries as the market changes over time. 

As with US-E2, intra-asset industry weights are constructed based on valuation-type models using sales, assets, and operating income within industry segments. The Compustat segment data tapes provide the breakdown of these balance sheet items by SIC code. 

## Industry classification scheme

## Mini-industries and industries

After review of tear sheets for all assets in the US-E2 HICAP universe, other industry classification schemes, and in-house micro-industry analysis, we selected 82 mini-industries to begin the asset-by-asset reclassification. Classification of each asset at the mini-industry level has the following benefits: 

1. It provides historical information necessary to test and confirm that any mini-industry which could have been placed into one of two or more industries has been correctly positioned within the industry BARRA has selected. 

2. It is easy to count the growth of companies within mini-industries. Growth to a “critical mass” can serve as the trigger to consider upgrading a mini-industry to industry status. This vastly aids implementation of an organic classification of industries. 

3. Related to 1. and 2. above, we have the relevant information to decide if, given a critical mass of assets within a mini-industry, it is necessary to create a new industry. An example of this is Drugs and Biotechnology. Tests of risk forecasts indicate it is not necessary to separate Biotechnology from Drugs, so we have chosen not to do so for US-E3. 

Maintaining an ongoing mini-industry classification makes it a relatively simple task to revisit any of the above decisions, should it ever appear necessary. All new assets that appear in the future will be classified at the mini-industry level, and BARRA will be able to add any new mini-industries necessary, should we start seeing companies that do not seem to be appropriately described by our current set of 82. 

## Sectors

After the US-E3 industries were determined, we created a mapping of industries to 13 sectors. These mappings were based on intuition rather than a data-driven algorithm. For the most part, they should generate little controversy. We have performed tests to confirm that the underlying intuition is borne out by the data. The methodology used was to examine the principal components associated with the industries within each sector. The goal was to determine if the intra-sector industry factor returns “behaved differently” and therefore should not be regarded as being instances of the same sector. This analysis confirmed the current industry-to-sector groupings to be appropriate. 

It will be possible to do performance attribution based on sectors with future releases of our Performance products. The time invariance of sectors will make it possible for historical performance across US-E2 and US-E3 historical portfolios. It will also make future introduction of new industries or extinction of current industries simple from a performance point of view. The only requirement is that the sectors remain constant across time. The sectors are sufficiently broad in scope to permit this time invariance. 

## Industry weights

The methodology necessary to determine industry exposures for companies with more than one business activity is relatively unchanged from US-E2. Briefly, the process is as follows. First, Compustat segment data are used to build what can be regarded as three separate valuation models. Second, the results of each valuation model determine a set of weights, based on fundamental information. Third, the final industry weights are a weighted average of the three weighting schemes. Here is the process in more detail: 

## 1. The valuation models

$$
\operatorname{capt} _ {n} = \sum_ {i = 1} ^ {I} \text { fundamental } _ {k, n, i} \beta_ {k, i}
$$

where $fundamental_{k,n,i}$ refers to sales, assets, and operating income of asset n within each industry and $\beta_{k,i}$ is the sensitivity of the nth asset's capitalization to these attributes. 

Each of the above three valuation models produces a set of betas that explains the contribution of “$1.00 worth of sales/assets/operating income” to the capitalization of asset n. The estimation of the betas for each model is subject to various controls to prevent unreasonable values. 

## 2. Asset industry weights for each model

Use sales-based valuation as an example: 

$$
w _ {n, s a l e s, i} = \frac {\text { sales } _ {n , i} \beta_ {\text { sales } , i}}{\sum_ {i = 1} ^ {I} \text { sales } _ {n , i} \beta_ {\text { sales } , i}}
$$

for the sales-based weight of asset n in industry i. 

## 3. Final weights

We weight each measure into our final industry weights based on reasonable estimates from past model behavior. 

## Historical assignment of industry and weights

For the purpose of historical estimation, industry assignments from January 1973 to January 1998 were performed on an annual basis. We ran the industry weight program every April during this period (since most U.S. companies end their fiscal year December 31, the beginning of April is when the largest burst of new data would be available). This may result in a loss of timely change of industries for companies that had mergers/splits during the intra-year period. Client feedback should serve to highlight any such misclassifications. 

## Ongoing assignment of industry and weights

## There are three points of note:

1. The weighting program will be run quarterly instead of annually. Between quarterly running of the valuation model, the most recent sales, assets, and operating income betas will be used with the most recent available Compustat segment data. 

2. We will review the tear sheets of one-twelfth of the assets in the estimation universe each month. The mini-industry associated with each Compustat segment data will be confirmed or corrected. This will ensure that no misclassifications of assets are perpetuated for more than one year. It will also help determine when to remove/add industry exposures resulting from mergers/sell-offs. 

3. A well-defined industry override policy is in place. There are two types of overrides: 

## ■ Industry assignments

Clients are likely to be the source of these. It is quite likely that they know more about what certain companies do than what we can glean from tear sheets and SIC codes. We will assess the client information and make changes to the mini-industry/industry assignments as necessary. 

## ■ Weights of assets with multiple industry exposure

This often arises when clients disagree with the primary industry of a company. In addition to the weighting process described above—call this our fundamental-based weights—we will run a style-analysis-based weight program for all companies with multiple-industry exposure. If questions arise about the industry weights, the style-based weights can be compared with the fundamental weights. Without strong support from the style weights, BARRA will stick with the fundamental weights. Clients can be told of our confirming evidence. 

## Industry evolution

Over time it is reasonable to expect some current industries to disappear and new ones to arise within the U.S. market. This certainly happened over the life cycle of US-E2. Problems associated with the inflexibility of US-E2's industry classification were one of the primary motivating forces for US-E3. The 82 mini-industry classification allows for easy promotion of a current mini-industry to industry status (as well as the less likely recombination of mini-industries into a whole or partially new industry). As long as we have assets identified by their mini-industry, it is easy to keep count of how many of them there are, so once we achieve a critical mass of companies we can consider estimating their factor returns. This also gives us the ability to test to see whether mini-industries behave differently from other mini-industries within the same industry. New mini-industries can be added at any time. 

Examples of US-E3 industries that have “been born” since 1975 are: 

<table><tr><td>Industry</td><td>Starting Date</td></tr><tr><td>Medical Providers &amp; Services</td><td>October 1975</td></tr><tr><td>Securities &amp; Asset Management</td><td>April 1976</td></tr><tr><td>Entertainment</td><td>November 1980</td></tr><tr><td>Computer Software</td><td>August 1982</td></tr><tr><td>Wireless Telecommunications</td><td>June 1989</td></tr></table>

The starting date for each of the above industries was triggered by an increase in the number of companies whose primary industry was one of the above. The target goal was to have 20 or more assets within each industry. 

There are no US-E3 examples of industries that have died out during the January 1975 to current estimation period. 

## Sector mapping of US-E3 industries

Table 9-1 is an overview of the default sector assignments for US-E3. We have chosen 13 well-defined sectors in order to facilitate stable performance attribution and other model operations as the industry matrix evolves over time. For a more detailed listing of industries, mini-industries, and example companies, see Appendix B. 


US-E3 Industry


<table><tr><td>Sector</td><td>US-E3 Industry</td></tr><tr><td>Basic Materials</td><td>Mining &amp; MetalsGoldForest Products &amp; PaperChemicals</td></tr><tr><td>Energy</td><td>Energy Reserves &amp; ProductionOil RefiningOil Services</td></tr><tr><td>Consumer Noncyclicals</td><td>Food &amp; BeveragesAlcoholTobaccoHome ProductsGrocery Stores</td></tr><tr><td>Consumer Cyclicals</td><td>Consumer DurablesMotor Vehicles &amp; PartsApparel &amp; TextilesClothing StoresSpecialty RetailDepartment StoresConstruction &amp; Real Property</td></tr><tr><td>Consumer Services</td><td>PublishingMediaHotelsRestaurantsEntertainmentLeisure</td></tr><tr><td>Industrials</td><td>Environmental ServicesHeavy Electrical EquipmentHeavy MachineryIndustrial Parts</td></tr><tr><td>Utility</td><td>Electrical UtilitiesGas Utilities</td></tr><tr><td>Transport</td><td>RailroadsAirlinesTrucking, Shipping, Air Freight</td></tr><tr><td>Health Care</td><td>Medical Providers &amp; ServicesMedical ProductsDrugs</td></tr><tr><td>Technology</td><td>Electronic EquipmentSemiconductorsComputer Hardware &amp; Office EquipmentComputer SoftwareDefense &amp; Aerospace</td></tr><tr><td>Telecommunications</td><td>TelephonesWireless Telecommunications</td></tr></table>

Sector Mapping of US-E3 Industries 


Table 9-1



US-E3 Industry


<table><tr><td>Commercial Services</td><td>Information ServicesIndustrial Services</td></tr><tr><td>Financial</td><td>Life &amp; Health InsuranceProperty &amp; Casualty InsuranceBanksThriftsSecurities &amp; Asset ManagementFinancial Services</td></tr></table>

Sector Mapping of US-E3 Industries 

# 10. Factor Return Estimation

## Overview

US-E3 factor returns for industries and all risk indices except Non-Estimation Universe Indicator (NONESTU, formerly LOCAP, which fits the model to smaller assets) are computed using GLS regression over the US-E3 estimation universe. The NONESTU factor return is calculated separately, using the excess return residual to non-NONESTU common factor returns of U.S. assets outside of the estimation universe. The asset weights used for the GLS are $hsigma^{-2}$ , where hsigma is the residual volatility resulting from a simple CAPM regression over the last 60 months of asset returns. 

## Estimation details

The only screening of data used for computation of the factor returns is the following: 

■ Assets must have an industry assignment. This removes mutual funds, which had been put in the US-E2 Miscellaneous industry, and any assets which may not have been classified. 

■ Assets must have a non-missing capitalization. This is done to screen out “dead” assets that have slipped into the historical data. 

■ Assets must have non-missing hsigma. This is necessary since the asset regression weight is based on this. 

■ Monthly asset returns must fall within [S&P 500 return - 50%, S&P 500 return + 150%]. This provides protection against possible data errors that have slipped through as well as legitimate large returns that are best prevented from contributing to the factor return estimates. This extreme return screening applies to both the “regular” factor returns and the NONESTU factor. 

## GLS weights

The US-E3 estimation universe is used for the estimation of industry factor returns and all risk index factor returns except the NONESTU factor return. 

The regression weight for each asset is $hsigma^{-2}$ , truncated to the 99th percentile of all assets in the estimation universe. This is done to prevent an asset with an extraordinarily small hsigma from dominating the entire estimation universe. 

## Factor returns for historic "newborn" industries

Industries that organically were “born” during the January 1975 to current estimation period have no GLS computed factor returns since there were no assets exposed to them at the time of estimation. A complete time series of factor returns is required for covariance matrix calculation. In these cases we use the time series of GLS factor returns for the parent industry to fill in the January 1975 to starting date factor returns. For example, prior to June 1989 the factor return used in covariance calculation for Wireless Telecommunications will be the same as that which was calculated for Telephones. 

## The NONESTU factor return

The NONESTU factor return is calculated in the same fashion as the LOCAP factor return in US-E2. 

1. Start with all assets not in the US-E3 estimation universe. 

2. Remove all non-U.S. assets. 

3. Exclude all assets associated with extreme returns (see above for definition of “extreme”). 

4. Compute the specific return of the remaining assets, based on factor returns. 

The NONESTU factor return is the capitalization-weighted average of these specific returns. 

## Testing

Each month we collect performance statistics to allow ongoing monitoring of model performance. These statistics include model R-squared, t-statistics, standard errors associated with factor returns, and multicollinearity diagnostics. We test for differences of mini-industries within industries and perform an alternative “thin-industry-adjusted” regression, saving the same model statistics as the ordinary GLS regression. 

# 11. Estimating the Factor Covariance Matrix in US-E3

## Overview

We construct the US-E3 common factor covariance matrix using: 

■ exponential weighting of monthly factor returns with a 90-month half-life 

■ an extended GARCH (1,1) market volatility forecast to scale the systematic risk portion of the matrix. 

US-E2 follows the same methodology, but it uses a plain GARCH(1,1) forecast. See Chapter 5. BARRA Multiple-Factor Modeling for details. 

## 12.US-E3 Specific Risk Modeling

## Overview

Expect more fluctuating month-to-month specific risk forecasts in US-E3 than in US-E2. This effect will be more pronounced at active risk perspective. 

The specific risk model in US-E3 has two important differences from that in US-E2. First, US-E3 has a predictive model for the average level of specific risk. Our research shows that the average level of specific risk displays predictable variation from month to month. As US-E3 incorporates this predictability into its specific risk forecasts, it will be able to predict the average level of specific risk more accurately than US-E2. 

The second difference from US-E2 is that US-E3 scales specific risk numbers differently across different size deciles to ensure that forecasts are unbiased within each decile. In contrast, US-E2 uses a single scaling function for all deciles. The finer scaling function used by US-E3 is an improvement over US-E2 and will produce more accurate specific risk forecasts. 

These improvements bring our U.S. Equity Model's specific risk forecasting method to the same level as in our other single country equity models. Details are contained in Chapter 5. BARRA Multiple-Factor Modeling. 

# Appendix A: US-E3 Descriptor Definitions

This Appendix gives the detailed definitions of the descriptors which underlie the risk indices in US-E3. The method of combining these descriptors into risk indices is proprietary to BARRA. 

## 1. Volatility

## i) BTSG: Beta times sigma

This is computed as $\sqrt{\beta\sigma_{\varepsilon}}$ , where $\beta$ is the historical beta and $\sigma_{\varepsilon}$ is the historical residual standard deviation. If $\beta$ is negative, then the descriptor is set equal to zero. 

## ii) DASTD: Daily standard deviation

This is computed as: 

$$
\sqrt {N _ {\text { days }} \left[ \sum_ {t = 1} ^ {T} w _ {t} r _ {t} ^ {2} \right]}
$$

where $r_{t}$ is the return over day t, $w_{t}$ is the weight for day t, T is the number of days of historical returns data used to compute this descriptor (we set this to 65 days), and $N_{days}$ is the number of trading days in a month (we set this to 23). 

## iii) HILO: Ratio of high price to low price over the last month

This is calculated as: 

$$
\log \left(\frac {P _ {H}}{P _ {L}}\right)
$$

where $P_{H}$ and $P_{L}$ are the maximum price and minimum price attained over the last one month. 

## iv) LPRI: Log of stock price

This is the log of the stock price at the end of last month. 

## v) CMRA: Cumulative range

Let $Z_{t}$ be defined as follows: 

$$
Z _ {t} = \sum_ {s = 1} ^ {t} \log (1 + r _ {i, s}) - \sum_ {s = 1} ^ {t} \log (1 + r _ {f, s})
$$

where $r_{i,s}$ is the return on stock i in month s, and $r_{f,s}$ is the risk-free rate for month s. In other words, $Z_{t}$ is the cumulative return of the stock over the risk-free rate at the end of month t. Define $Z_{max}$ and $Z_{min}$ as the maximum and minimum values of $Z_{t}$ over the last 12 months. CMRA is computed as: 

$$
\log \left(\frac {1 + Z _ {\max}}{1 + Z _ {\min}}\right)
$$

vi) VOLBT: Sensitivity of changes in trading volume to changes in aggregate trading volume 

This may be estimated by the following regression: 

$$
\frac {\Delta V _ {i , t}}{N _ {i , t}} = a + b \frac {\Delta V _ {M , t}}{N _ {M , t}} + \xi_ {i, t}
$$

where $\Delta V_{i,t}$ is the change in share volume of stock i from week t-1 to week t, $N_{i,t}$ is the average number of shares outstanding for stock i at the beginning of week t-1 and week t, $\Delta V_{M,t}$ is the change in volume on the aggregate market from week t-1 to week t, and $N_{M,t}$ is the average number of shares outstanding for the aggregate market at the beginning of week t-1 and week t. 

## vii) SERDP: Serial dependence

This measure is designed to capture serial dependence in residuals from the market model regressions. It is computed as follows: 

$$
S E R D P = \frac {\frac {1}{T - 2} \sum_ {t = 3} ^ {T} \left(e _ {t} + e _ {t - 1} + e _ {t - 2}\right) ^ {2}}{\frac {1}{T - 2} \sum_ {t = 3} ^ {T} \left(e _ {t} ^ {2} + e _ {t - 1} ^ {2} + e _ {t - 2} ^ {2}\right)}
$$

where $e_{t}$ is the residual from the market model regression in month t, and T is the number of months over which this regression is run (typically, T = 60 months). 

## viii) OPSTD: Option-implied standard deviation

This descriptor is computed as the implied standard deviation from the Black-Scholes option pricing formula using the price on the closest to at-the-money call option that trades on the underlying stock. 

## 2. Momentum

## i) RSTR: Relative strength

This is computed as the cumulative excess return (using continuously compounded monthly returns) over the last 12 months—i.e., 

$$
R S T R = \sum_ {t = 1} ^ {T} \log (1 + r _ {i, t}) - \sum_ {t = 1} ^ {T} \log (1 + r _ {f, t})
$$

where $r_{i,t}$ is the arithmetic return of the stock in month i, and $r_{f,t}$ is the arithmetic risk-free rate for month i. This measure is usually computed over the last one year—i.e., T is set equal to 12 months. 

## ii) HALPHA: Historical alpha

This descriptor is equal to the alpha term (i.e., the intercept term) from a 60-month regression of the stock's excess returns on the S&P 500 excess returns. 

## 3. Size

## i) LNCAP: Log of market capitalization

This descriptor is computed as the log of the market capitalization of equity (price times number of shares outstanding) for the company. 

## 4. Size Nonlinearity

## i) LCAPCB: Cube of the log of market capitalization

This risk index is computed as the cube of the normalized log of market capitalization. 

## 5. Trading Activity

## i) STOA: Share turnover over the last year

STOA is the annualized share turnover rate using data from the last 12 months—i.e., it is equal to $V_{ann}/\overline{N}_{out}$ , where $V_{ann}$ is the total trading volume (in number of shares) over the last 12 months and $\overline{N}_{out}$ is the average number of shares outstanding over the previous 12 months (i.e., it is equal to the average value of the number of shares outstanding at the beginning of each month over the previous 12 months). 

## ii) STOQ: Share turnover over the last quarter

This is computed as the annualized share turnover rate using data from the most recent quarter. Let $V_{q}$ be the total trading volume (in number of shares) over the most recent quarter and let $\overline{N}_{out}$ be the average number of shares outstanding over the period (i.e., $\overline{N}_{out}$ is equal to the average value of the number of shares outstanding at the beginning of each month over the previous three months). Then, STOQ is computed as $4V_{q}/\overline{N}_{out}$ . 

## iii) STOM: Share turnover over the last month

This is computed as the share turnover rate using data from the most recent month—i.e., it is equal to the number of shares traded last month divided by the number of shares outstanding at the beginning of the month. 

## iv) STO5: Share turnover over the last five years

This is equal to the annualized share turnover rate using data from the last 60 months. In symbols, STOS is given by: 

$$
S T O 5 = \frac {1 2 \left[ \frac {1}{T} \sum_ {s = 1} ^ {T} V _ {s} \right]}{\overline {{N}} _ {\text { out }}}
$$

where $V_{s}$ is equal to the total trading volume in month s and $\overline{N}_{out}$ is the average number of shares outstanding over the last 60 months. 

## v) FSPLIT: Indicator for forward split

This descriptor is a 0-1 indicator variable to capture the occurrence of forward splits in the company's stock over the last two years. 

## vi) VLVR: Volume to variance

This measure is calculated as follows: 

$$
V L V R = \log \left(\frac {\frac {1 2}{T} \sum_ {s = 1} ^ {T} V _ {s} P _ {s}}{\sigma_ {\varepsilon}}\right)
$$

where $V_{s}$ equals the number of shares traded in month s, $P_{s}$ is the closing price of the stock at the end of month s, and $\sigma_{\varepsilon}$ is the estimated residual standard deviation. The sum in the numerator is computed over the last 12 months. 

## 6. Growth

## i) PAYO: Payout ratio over five years

This measure is computed as follows: 

$$
P A Y O = \frac {\frac {1}{T} \sum_ {t = 1} ^ {T} D _ {t}}{\frac {1}{T} \sum_ {t = 1} ^ {T} E _ {t}}
$$

where $D_{t}$ is the aggregate dividend paid out in year t and $E_{t}$ is the total earnings available for common shareholders in year t. This descriptor is computed using the last five years of data on dividends and earnings. 

## ii) VCAP: Variability in capital structure

This descriptor is measured as follows: 

$$
V C A P = \frac {\frac {1}{T - 1} \sum_ {t = 2} ^ {T} \left(\left| N _ {t - 1} - N _ {t} \right| P _ {t - 1} + \left| L D _ {t - 1} - L D _ {t} \right| + \left| P E _ {t} - P E _ {t - 1} \right|\right)}{C E _ {T} + L D _ {T} + P E _ {T}}
$$

where $N_{t-1}$ is the number of shares outstanding at the end of time t-1; $P_{t-1}$ is the price per share at the end of time t-1; $LD_{t-1}$ is the book value of long-term debt at the end of time period t-1; $PE_{t-1}$ is the book value of preferred equity at the end of time period t-1; and $CE_{T} + LD_{T} + PE_{T}$ are the book values of common equity, long-term debt, and preferred equity as of the most recent fiscal year. 

## iii) AGRO: Growth rate in total assets

To compute this descriptor, the following regression is run: 

$$
T A _ {i t} = a + b t + \zeta_ {i t}
$$

where $TA_{it}$ is the total assets of the company as of the end of year t, and the regression is run for the period =1,...,5. AGRO is computed as follows: 

$$
A G R O = \frac {b}{\frac {1}{T} \sum_ {t = 1} ^ {T} T A _ {i t}}
$$

where the denominator average is computed over all the data used in the regression. 

## iv) EGRO: Earnings growth rate over last five years

First, the following regression is run: 

$$
E P S _ {t} = a + b t + \zeta_ {t}
$$

where $EPS_{t}$ is the earnings per share for year t. This regression is run for the period $t=1,\ldots,5$ . EGRO is computed as follows: 

$$
E G R O = \frac {b}{\frac {1}{T} \sum_ {t = 1} ^ {T} E P S _ {t}}
$$

## v) EGIBS: Analyst-predicted earnings growth

This is computed as follows: 

$$
E G I B S = \frac {(E A R N - E P S)}{(E A R N + E P S) / 2}
$$

where EARN is a weighted average of the median earnings predictions by analysts for the current year and next year, and EPS is the sum of the four most recent quarterly earnings per share. 

## vi) DELE: Recent earnings change

This is a measure of recent earnings growth and is measured as follows: 

$$
D E L E = \frac {\left(E P S _ {t} - E P S _ {t - 1}\right)}{\left(E P S _ {t} + E P S _ {t - 1}\right) / 2}
$$

where $EPS_{t}$ is the earnings per share for the most recent year, and $EPS_{t-1}$ is the earnings per share for the previous year. We set this to missing if the denominator is non-positive. 

## 7. Earnings Yield

## i) EPIBS: Analyst-predicted earnings-to-price

This is computed as the weighted average of analysts' median predicted earnings for the current fiscal year and next fiscal year divided by the most recent price. 

## ii) ETOP: Trailing annual earnings-to-price

This is computed as the sum of the four most recent quarterly earnings per share divided by the most recent price. 

## iii) ETP5: Historical earnings-to-price

This is computed as follows: 

$$
E T P 5 = \frac {\frac {1}{T} \sum_ {t = 1} ^ {T} E P S _ {t}}{\frac {1}{T} \sum_ {t = 1} ^ {T} P _ {t}}
$$

where $EPS_{t}$ is equal to the earnings per share over year t, and $P_{t}$ is equal to the closing price per share at the end of year t. 

## 8. Value

## i) BTOP: Book-to-price ratio

This is the book value of common equity as of the most recent fiscal year end divided by the most recent value of the market capitalization of the equity. 

## 9. Earnings Variability

## i) VERN: Variability in earnings

This measure is computed as follows: 

$$
V E R N = \frac {\left(\frac {1}{T - 1} \sum_ {t = 1} ^ {T} \left(E _ {t} - \overline {{E}}\right) ^ {2}\right) ^ {\frac {1}{2}}}{\frac {1}{T} \sum_ {t = 1} ^ {T} E _ {t}}
$$

where $E_{t}$ is the earnings at time t ( $t=1,\ldots,5$ ) and $\overline{E}$ is the average earnings over the last five years. VERN is the coefficient of variation of earnings. 

## ii) VFLO: Variability in cash flows

This measure is computed as the coefficient of variation of cash flow using data over the last five years—i.e., it is computed in an identical manner to VERN, with cash flow being used in place of earnings. Cash flow is computed as earnings plus depreciation plus deferred taxes. 

## iii) EXTE: Extraordinary items in earnings

This is computed as follows: 

$$
E X T E = \frac {\frac {1}{T} \sum_ {t = 1} ^ {T} \left| E X _ {t} + N R I _ {t} \right|}{\frac {1}{T} \sum_ {t = 1} ^ {T} E _ {t}}
$$

where $EX_{t}$ is the value of extraordinary items and discontinued operations, $NRI_{t}$ is the value of non-operating income, and $E_{t}$ is the earnings available to common before extraordinary items. The descriptor uses data over the last five years. 

## iv) SPIBS: Standard deviation of analysts' prediction to price

This is computed as the weighted average of the standard deviation of IBES analysts' forecasts of the firm's earnings per share for the current fiscal year and next fiscal year divided by the most recent price. 

## 10. Leverage

## i) MLEV: Market leverage

This measure is computed as follows: 

$$
M L E V = \frac {M E _ {t} + P E _ {t} + L D _ {t}}{M E _ {t}}
$$

where $ME_{t}$ is the market value of common equity, $PE_{t}$ is the book value of preferred equity, and $LD_{t}$ is the book value of long-term debt. The value of preferred equity and long-term debt are as of the end of the most recent fiscal year. The market value of equity is computed using the most recent month's closing price of the stock. 

## ii) BLEV: Book leverage

This measure is computed as follows: 

$$
B L E V = \frac {C E Q _ {t} + P E _ {t} + L D _ {t}}{C E Q _ {t}}
$$

where $CEQ_{t}$ is the book value of common equity, $PE_{t}$ is the book value of preferred equity, and $LD_{t}$ is the book value of long-term debt. All values are as of the end of the most recent fiscal year. 

## iii) DTOA: Debt-to-assets ratio

This ratio is computed as follows: 

$$
D T O A = \frac {L D _ {t} + D C L _ {t}}{T A _ {t}}
$$

where $LD_{t}$ is the book value of long-term debt, $DCL_{t}$ is the value of debt in current liabilities, and $TA_{t}$ is the book value of total assets. All values are as of the end of the most recent fiscal year. 

## iv) SNRRT: Senior debt rating

This descriptor is constructed as a multi-level indicator variable of the debt rating of a company. 

## 11. Currency Sensitivity

## i) CURSENS: Exposure to foreign currencies

To construct this descriptor, the following regression is run: 

$$
r _ {i t} = \alpha_ {i} + \beta_ {i} r _ {m t} + \varepsilon_ {i t}
$$

where $r_{it}$ is the excess return on the stock and $r_{mt}$ is the excess return on the S&P 500 Index. Let $\varepsilon_{it}$ denote the residual returns from this regression. These residual returns are in turn regressed against the contemporaneous and lagged returns on a basket of foreign currencies, as follows: 

$$
\varepsilon_ {i t} = c _ {i} + \gamma_ {i 1} (F X) _ {t} + \gamma_ {i 2} (F X) _ {t - 1} + \gamma_ {i 3} (F X) _ {t - 2} + u _ {i t}
$$

where $\varepsilon_{it}$ is the residual return on stock i, $(FX)_{t}$ is the return on an index of foreign currencies over month t, $(FX)_{t-1}$ is the return on the same index of foreign currencies over month t-1, and $(FX)_{t-2}$ is the return on the same index over month t-2. The risk index is computed as the sum of the slope coefficients $\gamma_{i1}$ , $\gamma_{i2}$ , and $\gamma_{i3}$ —i.e., CURSENS = $\gamma_{i1} + \gamma_{i2} + \gamma_{i3}$ . 

## 12. Dividend Yield

## i) P_DYLD: Predicted dividend yield

This descriptor uses the last four quarterly dividends paid out by the company along with the returns on the company's stock and future dividend announcements made by the company to come up with a BARRA-predicted dividend yield. 

## 13. Non-Estimation Universe Indicator

## i) NONESTU: Indicator for firms outside US-E3 estimation universe

This is a 0-1 indicator variable: It is equal to 0 if the company is in the US-E3 estimation universe and equal to 1 if the company is outside the US-E3 estimation universe. 

# Appendix B: US-E3 Industries, Mini-Industries, Example Companies, and Codes

Below you will find definitions and example companies for the US-E3 industry definitions. US-E3 industry definitions consist of two types: (1) main industries and (2) mini-industries. Main industries and their codes are indicated by boldface type in the table on the following pages. Each main US-E3 industry is comprised of one or more mini-industries; if more than one, secondary mini-industries are listed beneath the main industry. For example, the Forest Products & Paper main industry consists of three mini-industries: Forest Products & Paper; Household Paper; and Office Paper. The mini-industry which dominates the main industry (in this example, Forest Products & Paper) will usually determine the name of the main industry. 

Mini-industries serve two purposes. Some are being watched to determine whether they will grow into main industries at some future date—e.g., Gaming and Biotechnology. Others have been classified separately to allow for future testing and confirmation that the clusters of mini-industries have been correctly aggregated into main industries. 

The industries are aggregated into sectors, which provide a coarser breakdown of business activities. Sectors can be used for display purposes in US-E3 but play no role in estimation. 

<table><tr><td>Sector</td><td>US-E3 Industry Definition</td><td>Code</td></tr><tr><td rowspan="7">Basic Materials</td><td>Mining &amp; MetalsAluminum, coal, iron and steel, stainless steel, steel castings, copper, beryllium, nickel, titanium, uranium. Metal and glass containers. Metal recycling. Does not include aluminum foil for households.Examples: Alcoa, Bethlehem Steel</td><td>MINING</td></tr><tr><td>GoldGold and silver.Example: Homestake Mining</td><td>GOLD</td></tr><tr><td>Forest Products &amp; PaperLumber, wood, paper, newsprint, paper and cardboard containers, paper machine clothing (e.g., conveyor belts).Example: Georgia Pacific</td><td>FOREST</td></tr><tr><td>Household PaperToilet paper, paper towels, tissues.Household paper wholesaling.Example: Kimberly-Clark</td><td>HSPAPER</td></tr><tr><td>Office PaperStationery, office paper supplies.Example: Nashua</td><td>OFPAPER</td></tr><tr><td>ChemicalsChemicals, paints, plastics, plastic containers, coatings, gases, adhesives, inks, fibers. Does not include household chemicals and plastics.Example: Dow Chemical</td><td>CHEM</td></tr><tr><td>FertilizersFertilizers, agricultural chemicals (pesticides).Example: Monsanto</td><td>FERT</td></tr><tr><td rowspan="3">Energy</td><td>Energy Reserves &amp; ProductionOil and gas exploration, reserves, and production.Example: Exxon</td><td>RESERVES</td></tr><tr><td>Oil RefiningOil refining and marketing.Example: Quaker State</td><td>OILREF</td></tr><tr><td>Gas PipelinesGas pipelines and distribution.Example: Williams Companies</td><td>GASPIPE</td></tr><tr><td>Energy (continued)</td><td>Oil ServicesOil drilling, oil platform operating, oil platform support services, drill bits, drilling tools.Examples: Parker Drilling, Schlumberger</td><td>OILSERV</td></tr><tr><td rowspan="6">Consumer Noncyclicals</td><td>Food &amp; BeveragesFood companies (processed food), raw agriculture products, beverage companies, soda bottling, flower-growing, veterinary services. Does not include fertilizer.Examples: Kellogg, Tyson Foods, Coca-Cola</td><td>FOODBEV</td></tr><tr><td>Food WholesaleFood distribution and wholesaling.Example: Fleming Companies</td><td>WHOLEFD</td></tr><tr><td>AlcoholBeer, wine, and spirits. Alcohol wholesaling.Example: Anheuser-Busch</td><td>ALCOHOL</td></tr><tr><td>TobaccoCigars, cigarettes, pipe tobacco, leaf tobacco dealers, chewing tobacco, tobacco distribution.Example: Philip Morris</td><td>TOBACCO</td></tr><tr><td>Home ProductsSoaps, housewares, cosmetics, personal care, skin care, beauty care, dental care, household chemicals, household plastics.Example: Procter &amp; Gamble</td><td>HOMEPROD</td></tr><tr><td>Grocery StoresGrocery stores.Example: Safeway</td><td>RETFOOD</td></tr><tr><td rowspan="2">Consumer Cyclicals</td><td>Consumer DurablesHome furniture, appliances, lawn mowers, snow blowers, televisions, floor coverings, non-textile home furnishings, luggage, cutlery, china. Consumer durable wholesaling.Examples: Maytag, Sunbeam, Black &amp; Decker</td><td>DURABLES</td></tr><tr><td>Office FurnitureOffice Furniture.Example: Hon Industries</td><td>OFFURN</td></tr><tr><td rowspan="11">Consumer Cyclicals (continued)</td><td>Motor Vehicles &amp; PartsCar and auto part manufacturing. Car batteries. Not auto part retailing.Examples: Ford, GM</td><td>CARS</td></tr><tr><td>Trucks Truck manufacturing. Not heavy equipment (e.g., cranes).Example: Navistar International Corp.</td><td>TRUCKS</td></tr><tr><td>Motor Homes Motor homes and trailers.Example: Winnebago</td><td>MOTORHM</td></tr><tr><td>Apparel, TextilesManufacturing of apparel, textiles, shoes, textile home furnishings (towels, sheets, etc.), processing of fibers for textiles, wholesale but not retail sale of apparel.Examples: Liz Claiborne, Nike</td><td>APPAREL</td></tr><tr><td>Clothing StoresSpecialty apparel retailers. Does not include fabric stores.Examples: Gap, Nordstrom</td><td>RETAPP</td></tr><tr><td>Specialty RetailSells one type of item or uses one concept (e.g., items under $10). Not apparel retailers. Includes retail auto supply stores, consumer electronics stores, fabric stores, catalog marketing, telemarketing, auctioneers.Examples: Home Depot, Circuit City</td><td>RETSPEC</td></tr><tr><td>Drug StoresExample: Longs Drugs</td><td>DRUGSTOR</td></tr><tr><td>Department StoresRetailers who sell widely diverse products, department stores.Examples: Dayton Hudson, Wal-Mart</td><td>RETDIV</td></tr><tr><td>Construction &amp; Real PropertyBuilding materials, residential lighting and fixtures, home builders, building managers, equity REITs. Wholesale construction materials.Example: Kaufman &amp; Broad</td><td>CONST</td></tr><tr><td>ConcreteConcrete and construction aggregatesExample: Lone Star Industries, Inc.</td><td>CONCRETE</td></tr><tr><td>Manufactured Housing and Mobile HomesExample: Skyline Corp.</td><td>MANHOUSE</td></tr><tr><td>Consumer Cyclicals (continued)</td><td>EngineeringEngineering and construction firms, industrial construction, plant construction.Example: Stone &amp; Webster</td><td>ENGNR</td></tr><tr><td rowspan="11">Consumer Services</td><td>PublishingNewspaper and magazine publishers, book publishers, greeting cards.Examples: Dow Jones, New York Times</td><td>PUB</td></tr><tr><td>Commercial PrintingCheck and business form printing.Example: R.R. Donnelley</td><td>PRINTING</td></tr><tr><td>MediaRadio and TV stations, cable TV stations.Not TV programming.Example: CBS</td><td>MEDIA</td></tr><tr><td>Satellite CommunicationsExample: COMSAT</td><td>SATELLTE</td></tr><tr><td>HotelsHotels and motels.Example: Hilton Hotels</td><td>HOTEL</td></tr><tr><td>GamingCasinos.Example: Caesars World</td><td>GAMING</td></tr><tr><td>RestaurantsExample: McDonald's</td><td>RESTRNT</td></tr><tr><td>EntertainmentMovies, TV programming, theaters, theme parks, cruises.Example: Disney</td><td>ENT</td></tr><tr><td>LeisureGolf clubs, boats, toys, photography, entertainment systems, bicycles, novelties, camps, recreational vehicle parks, jewelry.Example: Eastman Kodak</td><td>LEISURE</td></tr><tr><td>Gaming EquipmentExample: International Game</td><td>GAMEQUIP</td></tr><tr><td>MotorcyclesExample: Harley-Davidson</td><td>MCYCLE</td></tr><tr><td rowspan="7">Industrials</td><td>Environmental ServicesWaste management, hazardous materials disposal, cogeneration and independent power. Environmental consulting.Example: Browning-Ferris Industries (BFI)</td><td>ENSERV</td></tr><tr><td>Heavy Electrical EquipmentElectrical equipment, electric power generation equipment, cables, wire, insulation, connectors. Not electronics, batteries, elevators.Examples: GE, Westinghouse</td><td>ELECTRIC</td></tr><tr><td>Heavy MachineryTractors, cranes, fire trucks, sweeper machines.Example: Caterpillar</td><td>HMACHINE</td></tr><tr><td>Industrial PartsIndustrial manufacture of bearings, gears, pumps, equipment, batteries. Elevators.Examples: Applied Industrial Technologies, Inc., Timken</td><td>INDPARTS</td></tr><tr><td>Machine ToolsManufacturing of machine tools. Heavy industry machine tools.Example: Cincinnati Milacron</td><td>MTOOLS</td></tr><tr><td>Hand ToolsManufacturing of hand tools.Example: Snap-On Tools</td><td>HTOOLS</td></tr><tr><td>MachineryManufacturing of machinery, engines.Example: Briggs &amp; Stratton</td><td>MACHINE</td></tr><tr><td rowspan="3">Utilities</td><td>Electric UtilitiesExample: Pacific Gas &amp; Electric</td><td>ELECUTIL</td></tr><tr><td>Gas UtilitiesExample: Brooklyn Union Gas</td><td>GASWATER</td></tr><tr><td>Water UtilitiesExample: American Water Works</td><td>WATUTIL</td></tr><tr><td rowspan="2">Transport</td><td>RailroadsRailroads and rolling stock leasing.Example: Burlington Northern</td><td>RAILROAD</td></tr><tr><td>AirlinesAirlines and airport ground services. Not air freight.Examples: AMR, Delta</td><td>AIRLINE</td></tr><tr><td rowspan="2">Transport (continued)</td><td>Trucking, Shipping, Air FreightSea, land freight.Examples: CNF Transportation, Inc., Alexander &amp; Baldwin</td><td>FREIGHT</td></tr><tr><td>Air FreightExample: American Express</td><td>AIRFRGHT</td></tr><tr><td rowspan="6">Health Care</td><td>Medical Providers &amp; ServicesHospitals, nursing homes, surgical centers, HMOs, rehabilitation providers, laboratories, hospital pharmacy management, apartments with available nursing, cemetery and funeral homes, medical equipment rental.Example: Humana</td><td>MEDPROV</td></tr><tr><td>Medical ProductsHigh-tech and low-tech medical products.</td><td>MEDPROD</td></tr><tr><td>Medical TechnologyX-ray machines, ultrasound, CAT scan, angiographic products, implants, pace-makers.Examples: Advanced Technology, Boston Scientific</td><td>MEDTECH</td></tr><tr><td>Medical SuppliesBand-Aids, catheters, needles, knives, blood collection vials.Example: Kendall</td><td>MEDSUPP</td></tr><tr><td>DrugsDrug production via traditional chemical processes.Examples: Merck, Eli Lilly</td><td>DRUGS</td></tr><tr><td>BiotechnologyDrug production via DNA technology, monoclonal antibodies.Examples: Genentech, Amgen</td><td>BIOTECH</td></tr><tr><td rowspan="6">Technology</td><td>Electronic EquipmentAnalytical instruments, instrumentation, test and measurement electronics, high precision motors, electronic power supplies, electronic controls, circuit board manufacturing, antennas, electrical switches, circuit protectors, sensors, thermostats, security systems, membrane separation technology.Examples: Tektronix, Varian</td><td>MANHT</td></tr><tr><td>Communications EquipmentEquipment for digital switching, telecommunications, visual telecommunications, video transmission and broadcasting, voice and data networking, voice mail and electronic mail, and telephones; optical fiber manufacturing, paging equipment.Examples: Oak Industries, ADC Telecommunications</td><td>COMMEQP</td></tr><tr><td>SemiconductorsManufacture of semiconductors, chips, equipment for semiconductor manufacturing.Example: Intel</td><td>SEMICOND</td></tr><tr><td>Computer Hardware &amp; Office EquipmentComputers, disk and tape drives, network equipment, copiers, office machines, bar code scanners, credit card verification equipment, automatic toll collectors, and automatic teller machines.Example: IBM</td><td>COMPUTER</td></tr><tr><td>Computer SoftwareExample: Microsoft</td><td>SOFTWARE</td></tr><tr><td>Defense &amp; AerospaceManufacturing for defense, including aircraft, tanks, submarines, and supplies. Civil aeronautics, space exploration. Aircraft parts.Examples: Lockheed, Boeing, General Dynamics</td><td>DEFAERO</td></tr><tr><td rowspan="3">Telecommunications</td><td>TelephonesLong-distance companies.Example: AT&amp;T</td><td>PHONE</td></tr><tr><td>Local Phone CompaniesLocal phone companies and Baby Bells.Examples: NYNEX, Pacific Telesis</td><td>LOCPHONE</td></tr><tr><td>Wireless TelecommunicationsCellular phones and pagers.Examples: GTE Contel, Nextel Communications</td><td>CELLULAR</td></tr><tr><td rowspan="2">Commercial Services</td><td>Information ServicesAccount keeping, payroll processing, news feeds, user-searchable databases, research-based financial information, translation services, computer centers, market research, management consulting, advertising, electronic publishing. Travel agents.Examples: Automatic Data Processing, Dun &amp; Bradstreet</td><td>INFOSERV</td></tr><tr><td>Industrial ServicesJanitorial and housekeeping services, plumbing, pest control, employment agencies, office temps, uniform rental, truck and auto fleet management, relocation services, employee and student education, training, and testing; security services, industrial plant management, car and truck leasing. Auto repair.Example: Manpower Inc.</td><td>INDSERV</td></tr><tr><td rowspan="5">Financial</td><td>Life and Health InsuranceIncludes life insurance, annuities, health insurance, disability insurance. Not HMOs.Examples: Equitable, UNUM</td><td>LIFEINS</td></tr><tr><td>Property and Casualty InsuranceProperty insurance, casualty insurance, municipal bond insurance, title insurance, liability insurance, workers' compensation insurance. Not HMOs.Example: Allstate</td><td>OTHERINS</td></tr><tr><td>BanksLocal and regional banks.Example: BayBank</td><td>BANK</td></tr><tr><td>Money Center BanksExample: J.P. Morgan</td><td>MONCENTR</td></tr><tr><td>ThriftsExample: Dime Savings Bank</td><td>THRIFT</td></tr><tr><td rowspan="3">Financial (continued)</td><td>Securities &amp; Asset ManagementBrokers, mutual fund companies, asset management companies.Example: Merrill Lynch</td><td>SECASSET</td></tr><tr><td>Financial ServicesMortgage brokers, consumer loans, car loans, student loans, home loans, credit cards, tax preparation, loan agencies of the U.S. government; also credit card processing, check guarantee, loan guarantee and collection, wire transfer, mortgage REITs. Credit unions, pawnshops, patents.Example: FNMA</td><td>FINSERV</td></tr><tr><td>Insurance Services and BrokersInsurance reporting and consulting, insurance claims adjusting, insurance brokers.Example: Marsh &amp; McClennan</td><td>INSERVBR</td></tr></table>

Specific Risk 

# Appendix C: US-E3 Frequency Distributions for Predicted Beta, Specific Risk, Risk Indices

## Predicted beta

Predicted US-E3 beta frequency distribution of 1,941 estimation universe assets as of December 1997: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/26da146068772125baacdd52cfc674107e1027fc563db26d85418598fdd08ccb.jpg)


## Specific risk

Predicted US-E3 specific risk frequency distribution of 1,941 estimation universe assets as of December 1997: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/112e2c1e30ad3ec3ec58bf5971df1ee1ac4d247cb5a59adf993120db7478d659.jpg)


## Risk indices

US-E3 risk index frequency distributions of 1,941 estimation universe assets as of December 1997: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/cab95e42e37426f2f4b2432f9307559865992adddd3a40fd8cafdd16ca67f1ad.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/9ee259e01b063ee0440369f105d3514736c09fe42c35f4aa88c5b58175c7294f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/b08c101a1a89b1c198a1ca0ae2fe2587ec24090115b0c848dcdfe0a571b0a67a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/f8422d1e088031947c5add09bcf117e96507fa27a22a47bf954159f4bb224e13.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/c310e74a69b100de2fd601d3e22a98cd16f56cca956ef46f0fb037b1e1146075.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/38298b282d8bd2ca4e59e25a4466047b018538fbc19074efef534b72c398df8d.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/9f904f87d9c36d0bb890ee7c73cc780f37e860c0ad44d55ced771f0c23083d67.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/36a909e8d4b0857692c4451a25a363640e77d54f8363dd174cb68c2c7f57aaa5.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/f6529adde61be846c00a38941a9a9e9ce767b0123c9f832af3aa18a51ffefe91.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/c3a394e9d85df77a0ba9c593b38f01c629fba85fbeff0eba8b94adcfde02b81b.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/47f9e37a577b45f0e716faac381726d152912ed95a61aed374ccfd34cedd2763.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/7ea4c1c71058ef894cb4d22bb604d6edf2cbc3a9d976e6a12ce56b8ced5233b2.jpg)


## Appendix D: US-E3 Risk Index Factor Returns

The following pages display factor return charts for US-E3's risk indices over the period December 1974–December 1997. The single risk index return is the return that results from a regression of asset return against a single risk index and all industries. The multiple risk index return is the return that results from a regression of asset return against all risk indices and all industries. The single risk index return is the return that results from a naive model; it is shown here for comparison purposes only. The multiple risk index return is the "true" factor return; it is the return used to explain performance and to construct the factor covariance matrix. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/50e9326fdbf8a9374acc065122cd77063558d307cdfe36b0815ff83c7977e7af.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/fc4e85e1d387cc5b1f29b4d49bf5890a1b96294cb36ec4a5c5a34f70111d4ca1.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/86e4aa29631211a3486eec63c2f4244d8109677c108df4e7721b53fc3b21d53b.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/bb06450d40406ad3c03c25e551b41b2eec0085f9c47a252b493fb32f8f2a5b2f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/be9b4c85a233cec2b310a62adb558e97922dc13740ac20588235300e692861bc.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/2e605dfd483d2e2e169db403735c6f8620144668df9a235482e6b63bb1837c95.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/61b298791a3d531e8507389f0254bb10b57bf51196e33ca04d58b75385533bae.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/9af7741fd5dfd8fb5ed7b91b750616b12732483d00be318b4ffb3ba495125a99.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/423904d5707ec8038efd1f17145e483fa9542af0c4877193d63deb3994ab85b2.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/bb9b71cb077c0848d896222a4d967c1ccdaed7d0a112a4289655fbd9768ca6da.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/3788ea65d34bd0a34c783cdc7771f8ebf2e2c937f55d5ab338d9d65cd51a4aff.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/ec3d669a-e212-47c1-a18d-f42349d5055c/c782980b5f4197c4d6a3420f832e8241c1034c1dcfd91489b81b682384735176.jpg)


## Glossary

<table><tr><td>active management</td><td>The pursuit of investment returns in excess of a specified benchmark.</td></tr><tr><td>active return</td><td>Return relative to a benchmark. If a portfolio's return is 5%, and the benchmark's return is 3%, then the portfolio's active return is 2%.</td></tr><tr><td>active risk</td><td>The risk (annualized standard deviation) of the active return. Also called tracking error.</td></tr><tr><td>alpha</td><td>The expected residual return. Beyond the pages of this book, alpha is sometimes defined as the expected exceptional return and sometimes as the realized residual or exceptional return.</td></tr><tr><td>arbitrage</td><td>To profit because a set of cash flows has different prices in different markets.</td></tr><tr><td>Arbitrage Pricing Theory (APT)</td><td>Developed in the late 1970s, the theory which asserts that securities and portfolio returns are based on the expected returns attributable to an unknown number of underlying factors. APT provides a complementary alternative to its precursor, the Capital Asset Pricing Model.</td></tr><tr><td>benchmark</td><td>A reference portfolio for active management. The goal of the active manager is to exceed the benchmark return.</td></tr><tr><td>beta</td><td>The sensitivity of a portfolio (or asset) to a benchmark. For every 1% return to the benchmark, we expect a β·1% return to the portfolio.</td></tr><tr><td>beta, historical</td><td>Historical measure of the response of a company's return to the market return, ordinarily computed as the slope coefficient in a 60-month historical regression.</td></tr><tr><td>beta, predicted</td><td>Predicted systematic risk coefficients (predictive of subsequent response to market return) that are derived, in whole or in part, from the fundamental operating characteristics of a company. Also called fundamental beta.</td></tr><tr><td>breadth</td><td>The number of independent forecasts available per year. A stock picker forecasting returns to 100 stocks every quarter exhibits a breadth of 400, assuming each forecast is independent (based on separate information).</td></tr><tr><td>Capital Asset Pricing Model (CAPM)</td><td>The simplest version states that the expected excess return on securities will be exactly in proportion to their systematic risk coefficient, or beta. The CAPM implies that total return on any security is equal to the risk-free return, plus the security's beta, multiplied by the expected market excess return.</td></tr><tr><td>certainty equivalent return</td><td>The certain (zero risk) return an investor would trade for a given (larger) return with an associated risk. For example, a particular investor might trade an expected 3% active return with 4% risk for a certain active return of 1.4%.</td></tr><tr><td>characteristic portfolio</td><td>A portfolio which efficiently represents a particular asset characteristic. For a given characteristic, it is the minimum risk portfolio with portfolio characteristic equal to 1. For example, the characteristic portfolio of asset betas is the benchmark. It is the minimum risk beta = 1 portfolio.</td></tr><tr><td>coefficient of determination (<eq>R^2</eq>)</td><td>See R-squared.</td></tr><tr><td>common factor</td><td>An element of return that influences many assets. According to multiple-factor risk models, the common factors determine correlations between asset returns. Common factors include industries and risk indices.</td></tr><tr><td>constraint</td><td>In portfolio optimization, a limitation imposed upon the portfolio so that it will have desired characteristics.</td></tr><tr><td>correlationcovariance</td><td>A statistical term giving the strength of linear relationship between two random variables. It is a pure number, ranging from -1 to +1: +1 indicates a perfect positive linear relationship; -1 indicates a perfect negative linear relationship; 0 indicates no linear relationship. For jointly distributed random variables, correlation is often used as a measure of strength of relationship, but it fails when a nonlinear relationship is present.The tendency of different random investment returns to have similar outcomes, or to “covary.” When two uncertain outcomes are positively related, covariance is positive, and conversely, negatively related outcomes have negative covariances. The magnitude of covariance measures the strength of the common movement. For the special case of a return’s covariance with itself, the simplified name of variance is used. Covariance can be scaled to obtain the pure number, correlation, that measures the closeness of the relationship without its magnitude.</td></tr><tr><td>descriptor</td><td>A variable describing assets, used as an element of a risk index. For example, a volatility risk index, distinguishing high volatility assets from low volatility assets, could consist of several descriptors based on short-term volatility, long-term volatility, systematic and residual volatility, etc.</td></tr><tr><td>Dividend Discount Model (DDM)</td><td>A model of asset pricing based on discounting the future expected dividends.</td></tr><tr><td>dividend yield</td><td>The dividend per share divided by the price per share. Also known as the yield.</td></tr><tr><td>earnings yield</td><td>The earnings per share divided by the price per share.</td></tr><tr><td>efficient frontier</td><td>A set of portfolios, one for each level of expected return, with minimum risk. We sometimes distinguish different efficient frontiers based on additional constraints, e.g., the fully invested efficient frontier.</td></tr><tr><td>exceptional return</td><td>Residual return plus benchmark timing return. For a given asset with beta equal to 1, if its residual return is 2%, and the benchmark portfolio exceeds its consensus expected returns by 1%, then the asset’s exceptional return is 3%.</td></tr><tr><td>excess return</td><td>Return relative to the risk-free return. If an asset’s return is 3% and the risk-free return is 0.5%, then the asset’s excess return is 2.5%.</td></tr><tr><td>factor portfolio</td><td>The minimum risk portfolio with unit exposure to the factor and zero exposures to all other factors. The excess return to the factor portfolio is the factor return.</td></tr><tr><td>factor return</td><td>The return attributable to a particular common factor. We decompose asset returns into a common factor component, based on the asset's exposures to common factors times the factor returns, and a specific return.</td></tr><tr><td>information coefficient</td><td>The correlation of forecast return with their subsequent realizations. A measure of skill.</td></tr><tr><td>information ratio</td><td>The ratio of annualized expected residual return to residual risk. A central measurement for active management, value added is proportional to the square of the information ratio.</td></tr><tr><td>market</td><td>The portfolio of all assets. We typically replace this abstract construct with a more concrete benchmark portfolio.</td></tr><tr><td>modern portfolio theory (MPT)</td><td>The theory of portfolio optimization which accepts the risk/reward tradeoff for total portfolio return as the crucial criterion. Derived from Markowitz's pioneering application of statistical decision theory to portfolio problems, optimization techniques and related analysis are increasingly applied to investments.</td></tr><tr><td>multiple-factor model (MFM)</td><td>A specification for the return process for securities. This model states that the rate of return on any security is equal to the weighted sum of the rates of return on a set of common factors, plus the specific return on the security, where the weights measure the exposures (or sensitivity) of the security to the factor. These exposures are identified with microeconomic characteristics, or descriptors of the firms (see descriptor).Several simplifications of this model have been used historically. If there is only one factor, it becomes a single-factor model; if this one factor is identified with an index, it is called a single-index model; if the single-factor is identified with the market factor, it becomes the market model. Depending on the statistical specification, some of these could become a diagonal model, which simply indicates that the covariance matrix between security returns is (or can easily be transformed into) a diagonal matrix.</td></tr><tr><td>normal</td><td>A benchmark portfolio.</td></tr><tr><td>normalization</td><td>The process of transforming a random variable into another form with more desirable properties. One example is standardization in which a constant (usually the mean) is subtracted from each number to shift all numbers uniformly. Then each number is divided by another constant (usually the standard deviation) to shift the variance.</td></tr><tr><td>optimization</td><td>The best solution among all the solutions available for consideration. Constraints on the investment problem limit the region of solutions that are considered, and the objective function for the problem, by capturing the investor's goals correctly, providing a criterion for comparing solutions to find the better ones. The optimal solution is that solution among those admissible for consideration which has the highest value of the objective function. The first-order conditions for optimality express the tradeoffs between alternative portfolio characteristics to provide the optimum solution.</td></tr><tr><td>outlier</td><td>A data observation that is very different from other observations. It is often the result of an extremely rare event or a data error.</td></tr><tr><td>passive management</td><td>Managing a portfolio to match (not exceed) the return of a benchmark.</td></tr><tr><td>payout ratio</td><td>The ratio of dividends to earnings. The fraction of earnings paid out as dividends.</td></tr><tr><td>performance analysis</td><td>Evaluation of performance in relation to a standard or benchmark with the purpose of assessing manager skill.</td></tr><tr><td>performance attribution</td><td>The process of attributing portfolio returns to causes. Among the causes are the normal position for the portfolio, as established by the owner of funds or the manager, as well as various active strategies, including market timing, common factor exposure, and asset selection. Performance attribution serves an ancillary function to the prediction of future performance, in as much as it decomposes past performance into separate components that can be analyzed and compared with the claims of the manager.</td></tr><tr><td>R-squared</td><td>A statistic usually associated with regression analysis, where it describes the fraction of observed variation in data captured by the model. It varies between 0 and 1.</td></tr><tr><td>regression</td><td>A data analysis technique that optimally fits a model based on the squared differences between data points and model fitted points. Typically, regression chooses model coefficients to minimize the (possibly weighted) sum of these squared differences.</td></tr><tr><td>residual return</td><td>Return independent of the benchmark. The residual return is the return relative to beta times the benchmark return. To be exact, an asset's residual return equals its excess return minus beta times the benchmark excess return.</td></tr><tr><td>residual risk</td><td>The risk (annualized standard deviation) of the residual return.</td></tr><tr><td>risk</td><td>The uncertainty of investment outcomes. Technically, risk defines all uncertainty about the mean outcome, including both upside and downside possibilities. The more intuitive concept for risk measurement is the standard deviation of the distribution, a natural measure of spread. Variance, the square of the standard deviation, is used to compare independent elements of risk.</td></tr><tr><td>risk-free return</td><td>The return achievable with absolute certainty. In the U.S. market, short maturity Treasury bills exhibit effectively risk-free returns. The risk-free return is sometimes called the time premium, as distinct from the risk premium.</td></tr><tr><td>risk index</td><td>A common factor typically defined by some continuous measure, as opposed to a common industry membership factor defined as 0 or 1. Risk index factors include Volatility, Momentum, Size, and Value.</td></tr><tr><td>risk premium</td><td>The expected excess return to the benchmark.</td></tr><tr><td>score</td><td>A normalized asset return forecast. An average score is 0, with roughly two-thirds of the scores between -1 and 1. Only one-sixth of the scores lie above 1.</td></tr><tr><td>security market line</td><td>The linear relationship between asset returns and betas posited by the Capital Asset Pricing Model.</td></tr><tr><td>Sharpe ratio</td><td>The ratio of annualized excess returns to total risk.</td></tr><tr><td>significance(statistical significance)</td><td>A statistical term which measures the spread or variability of a probability distribution. The standard deviation is the square root of variance. Its intuitive meaning is best seen in a simple, symmetrical distribution, such as the normal distribution, where approximately two-thirds of all outcomes fall within ± 1 standard deviation of the mean, approximately 95 percent of all outcomes fall within ± 2 standard deviations, and approximately 99 percent of all outcomes fall within ± 2.5 standard deviations. The standard deviation of return—or, more properly, of the logarithm of return, which is approximately symmetrically distributed—is very widely used as a measure of risk for portfolio investments.</td></tr><tr><td>skill</td><td>The ability to accurately forecast returns. We measure skill using the information coefficient.</td></tr><tr><td>specific return</td><td>The part of the excess return not explained by common factors. The specific return is independent of (uncorrelated with) the common factors and the specific returns to other assets. It is also called the idiosyncratic return.</td></tr><tr><td>specific risk</td><td>The risk (annualized standard deviation) of the specific return.</td></tr><tr><td>standard error</td><td>The standard deviation of the error in an estimate. A measure of the statistical confidence in the estimate.</td></tr><tr><td>standardization</td><td>Standardization involves setting the zero point and scale of measurement for a variable. An example might be taken from temperature, where the centigrade scale is standardized by setting zero at the freezing point of water and establishing the scale (the centigrade degree) so that there are 100 units between the freezing point of water and the boiling point of water. Standardization for risk indices and descriptors in BARRA equity models sets the zero value at the capitalization-weighted mean of the companies in the universe and sets the unit scale equal to one cross-sectional standard deviation of that variable among the estimation universe.</td></tr><tr><td>systematic return</td><td>The part of the return dependent on the benchmark return. We can break excess returns into two components: systematic and residual. The systematic return is the beta times the benchmark excess return.</td></tr><tr><td>systematic risk</td><td>The risk (annualized standard deviation) of the systematic return.</td></tr><tr><td>t-statistic</td><td>The ratio of an estimate to its standard error. The t-statistic can help test the hypothesis that the estimate differs from zero. With some standard statistical assumptions, the probability that a variable with a true value of zero would exhibit a t-statistic greater than 2 in magnitude is less than 5%.</td></tr><tr><td>tracking error</td><td>See active risk.</td></tr><tr><td>transaction costs</td><td>The costs incurred for a portfolio when securities are changed for other securities. Transaction costs are deducted from the value of the portfolio directly, rather than paid as fees to the money manager. These costs arise from three sources: (1) commissions and taxes paid directly in cash; (2) the typical “dealer’s spread” (or one-half of this amount) earned by a dealer, if any, who acts as an intermediary between buyer and seller; and (3) the net advantage or disadvantage earned by giving or receiving accommodation to the person on the other side of the trade. The third component averages out to zero across all trades, but it may be positive or negative, depending on the extent to which a trader, acting urgently, moves the market against the selected strategy.</td></tr><tr><td>universe</td><td>The list of all assets eligible for consideration for inclusion in a portfolio. At any time, some assets in the universe may be temporarily ruled out because they are currently viewed as overvalued. However, the universe should contain all securities that might be considered for inclusion in the near term if their prices move to such an extent that they become undervalued.Universealso defines the normal position of a money manager, equating the normal holding with the capitalization-weighted average of the securities in the universe or followed list.</td></tr><tr><td>utility</td><td>A measure of the overall desirability or goodness of a person’s situation. In the theory of finance, utility is the desirability of a risky series of outcomes. The utility (or expected utility) of a set of risky outcomes is assumed to measure its goodness, so that a package with higher utility is always preferred to one with lower utility. In portfolio theory,utilityis almost always defined by a function of the mean and variance of portfolio outcomes, which is then called a mean/ variance utility function. The further assumption that the utility function is linear in its two arguments (mean and variance) results in a linear mean/variance utility function (LMVU).</td></tr></table>

## value added

## variance

The utility, or risk-adjusted return, generated by an investment strategy: the return minus a risk aversion constant times the variance. The value added depends on the performance of the manager and the preferences of the owner of the funds. 

A statistical term for the variability of a random variable about its mean. The variance is defined as the expected squared deviation of the random variable from its mean—that is, the average squared distance between the mean value and the actually observed value of the random variable. When a portfolio includes several independent elements of risk, the variance of the total arises as a summation of the variances of the separate components. 

A loosely-defined term for risk. Here we define volatility as the annualized standard deviation of return. 

See dividend yield. 

## Index

## A

Active management 32–33, 35–37
definition 127
strategies 32
Active management strategies
market timing 32
sectoral emphasis 32
stock selection 32
Active Portfolio Management: Quantitative Theory and Applications 5, 12
Active portfolios 36
Active return
definition 127
Active Risk 36
decomposition 36
definition 127
Active Risk Mode 36
Active Systematic-Active Residual Risk decomposition 37
Advantages of US-E3 Over US-E2 3, 55–61
Alpha 33
definition 32, 127
Alpha, historical
definition 32
Appendix A:
US-E3 Descriptor Definitions 93–104
Appendix B:
US-E3 Industries, Mini-Industries,
Example Companies, and Codes 105–114
Appendix C:
US-E3 Frequency Distributions for Predicted Beta, Specific Risk, Risk Indices 115–120
Appendix D:
US-E3 Risk Index Factor
Returns 121–125
APT: see Arbitrage Pricing Theory
Arbitrage
definition 127
Arbitrage Pricing Theory (APT) 19, 31
definition 127
Asset attributes 21
Asset class issues
future modeling 61
US-E2 and US-E3 61 

Asset covariance matrix 27
Asset industry weights for each model 79
Asset selection 33 

## B

BARRA
corporate history 1
multiple-factor models (MFMs) 31
risk models 1
Web site 5
BARRA equity risk models
industry allocation 45
model estimation 41–53
model estimation process 41
BARRA Multiple-Factor Modeling 3, 41–54
overview 41
BARRA single country equity models
features 53–54
table 54
BARRA Total Plan Risk™ 1
BARRA World Markets Model™ 1
Basic Materials 106
Benchmark 31, 32, 37, 44
definition 31, 127
Benchmark risk 36
Bernstein, Peter L. 8
Beta 18, 35
definition 127
Beta, fundamental 127
Beta, historical
definition 127
Beta, predicted
definition 127
Breadth
definition 128
Breiman, Leo 17 

## C

Capital Asset Pricing Model (CAPM) 17,
18, 19, 26, 31
definition 128
risk decomposition 35 

Capitalization
in US-E3 estimation universe 64
CAPM: see Capital Asset Pricing Model
Certainty equivalent return
definition 128
Characteristic portfolio
definition 128
Clasing, Henry K. 5
Codes, US-E3 industry
table 106–114
Coefficient of determination 128
Commercial Services 113
Common factor
definition 128
Common factor risk
definition 34
Common factors 21
Compustat 77, 79
Compustat data
in US-E3 estimation universe 64
Computing market volatility
extended GARCH models 48
Connor, Gregory 19
Constraint
definition 128
Consumer Cyclicals 107–109
Consumer Noncyclicals 107
Consumer Services 109
Correlation
definition 128
Costs, transaction
definition 134
Covariance 26, 27
definition 129
Covariance matrix 27
calculation 46
estimation 27
Cross-sectional regressions 41
Currency Sensitivity 59, 103, 119
factor returns 125
Currency Sensitivity risk index 69, 75 

## D

Decomposing risk 34–38
Decomposition of risk
overview 38
Defining Risk 3, 11–19
Descriptor
definition 129
definitions for US-E3 93–104
Currency Sensitivity 103 

Dividend Yield 104
Earnings Variability 101
Earnings Yield 100
Growth 98
Leverage 102
Momentum 95
Non-Estimation Universe
Indicator 104
Size 96
Size Nonlinearity 96
Trading Activity 96
Value 101
Volatility 93
selection 41
selection and testing 44
standardization 44
Descriptors 21, 45
US-E3 58–59, 67–76
Diagnostics, US-E3 60
Diagonal model 130
Diversification 17, 33
and risk 33, 17
risk reduction benefits of 14
Dividend Discount Model (DDM)
definition 129
Dividend Yield 67, 75, 104, 120
Dividend yield
definition 129 

## E

E1: see US-E1
E2: see US-E2
E3: see US-E3
Earnings Variability 75, 101, 119
factor returns 124
Earnings Yield 75, 100, 118
factor returns 124
Earnings yield
definition 129
Earnings-to-Price Ratio 67
Efficient frontier
definition 129
Energy 106–107
Enhanced indexing 31
Equations
multiple-factor model 28, 29
Equity risk and return, theory of 3
Equity risk models
model estimation process 41
Estimating the Factor Covariance Matrix in US-E3 4, 89 

Estimation universe
US-E3 57, 63–65
US-E3 compared with US-E2 65
Example companies
US-E3 industries 105–114
Exceptional return
definition 129
Excess return
definition 129
Exponential weighting 41, 47
Extended GARCH models
theory 48 

## F

Factor covariance matrix 28, 89
estimating 46
Factor portfolio
definition 129
Factor return 129
definition 130
Factor Return Estimation 4, 85–87
Factor return estimation 46, 60
details 85
for historic “newborn” industries 86
GLS weights 86
NONESTU 86
overview 85
testing 87
Factor returns 27, 41
for US-E3 risk indices 121–125
Currency Sensitivity 125
Earnings Variability 124
Earnings Yield 124
Growth 123
Leverage 125
Momentum 122
Size 122
Size Nonlinearity 123
Trading Activity 123
Value 124
Volatility 122
Yield 125
Factor, common
definition 128
Final weights 80
Financial 113–114
Financial Leverage (US-E2) 69
Foreign Income
eliminated in US-E3 59
Foreign Income (US-E2) 69 

Frequency distributions
Currency Sensitivity 119
Dividend Yield 120
Earnings Variability 119
Earnings Yield 118
Growth 118
Leverage 119
Momentum 116
predicted beta 115
risk indices 116–120
Size 117
Size Nonlinearity 117
specific risk 115
Trading Activity 117
Value 118
Volatility 116
Frontier, efficient
definition 129
Fundamental beta 127
Fundamental data 21
Fundamental factor models 19 

## G

GARCH 89
models 48–49, 59
techniques 42
theory 48
Glossary 127–135
GLS
regression 85
weights 86
Grandfathering
in US-E3 estimation universe 65
Grinold, Richard C. 5, 12
Growth 67, 68, 75, 98, 118
factor returns 123 

## H

Health Care 111
Hedge funds 35
HICAP 65
Historical alpha definition 32
Historical assignment, industry and weights 80
Historical beta definition 127 

## |

Idiosyncratic return 133
Index funds
    analyzing 36
Index, risk
    definition 132
Indexing
    enhanced 31
Industrials 110
Industries 45
    factor returns for historic “newborn” 86
    new in US-E3 56–57
    reclassification in US-E3 56–57
    table 83–84
    US-E2 4
    US-E3 77–83
Industries, sectors, and codes
    US-E3 105–114
Industries, US-E3
    example companies 106–114
Industries, flexible
    in US-E3 57
Industry allocation 41
    multiple industries 45
    single industry 45
Industry classification scheme 77–78
    mini-industries and industries 77–78
    sectors 78
Industry codes
    US-E3 105–114
Industry definitions 106–114
Industry evolution 81–82
Industry fill-in
    in US-E3 estimation universe 64
Industry weights 79–81
    asset industry weights for each model 79
    final weights 80
    historical assignment 80
    ongoing assignment 80
    the valuation models 79
Information coefficient
    definition 130
Information ratio
    definition 130
Introduction 3–5 

J
Japan Equity Risk Model
industry exposures 45 

## K

Kahn, Ronald N. 5, 11, 12 

## L

Labor Intensity (US-E2) 69
eliminated in US-E3 59
Leverage 58, 69, 75, 102, 119
factor returns 125
LOCAP 85
factor return, US-E2 86 

## M

Macroeconomic factor models 19
Management
active 127
passive
definition 131
Market
definition 130
Market data 41
Market model 130
Market timing 32, 37
Markowitz, Harry 17
MFM: see Multiple-factor model
Mini-industries and industries 77
Mini-industries, US-E3
table 106–114
Minimum price
in US-E3 estimation universe 64
Miscellaneous industry 85
Model
updating 52
Model estimation
BARRA equity risk models 41–53
data flow 43
process 41
Model features
comparison of BARRA single country
equity models 53–54
Model fit-related issues 60
Model parameters
refitting 60
Model performance
testing 87
Model testing 42
Model, diagonal 130
Model, market 130
Model, single-factor 130
Model, single-index 130
Modeling and Forecasting Risk 3, 21–29 

Models
    fundamental factor 19
    macroeconomic factor 19
    single-factor 25
    statistical factor 19
Modern Portfolio Management and Risk 3,
    31–39
Modern portfolio theory (MPT)
    definition 130
Modern Portfolio Theory:
    The Principles of Investment Management 5
Modes of risk 34–38
Momentum 74, 95, 116
    factor returns 122
Multiple risk index return 121
Multiple-factor model (MFM) 19, 31
    a simple MFM 23
    advantages 22
    BARRA 31–39
    definition 21, 130
    equations 28, 29
    limitations 22
    model mathematics 25
    risk prediction 26
    total excess return 26
mutual funds 85 

## N

Non-Estimation Universe Indicator
(NONESTU) 65, 76, 85, 104
factor return 86

NONESTU see Non-Estimation Universe
Indicator

Normal
definition 130

Normal portfolio
definition 31

Normalization
definition 44, 131
process summarized 44 

## 0

Optimization
definition 131
Option-implied standard deviation 59
Outlier
definition 131 

## P

Passive management 31–32, 34–35
attributes 32
characteristics 31
definition 31, 131
types 31
Payout ratio
definition 131
Performance 7
Performance analysis
definition 131
Performance attribution
BARRA programs 38
definition 38, 131
Performance Pyramid 7
Portfolio
benchmark 37
Portfolio allocation 33
Portfolio management
active 31
passive 31
types 31
Portfolio, characteristic
definition 128
Portfolio, factor
definition 129
Predicted beta 115
definition 127 

## R

References 5
Regression
definition 132
REIT 61
risk index exposures in US-E3 55
Residual return 33
definition 132
Residual risk 32, 35
definition 132
specific and common factor sources 35
Return
active 127
exceptional
definition 129
excess
definition 129
factor
definition 130
idiosyncratic 133
residual 33
definition 132 

risk-free
    definition 132
specific
    definition 133
systematic
    definition 133
Risk
Active 36
active 127
Active Systematic-Active Residual 37
and diversification 33
benchmark 36
common factor 34
decomposing 34–38
definition 11, 132
drawbacks of simple risk calculations 16
evolution of concepts 16
measurement 13
premium
    definition 132
reduction
    through diversification 14
residual 35
    definition 132
specific 34
    definition 133
systematic 35
    definition 133
Systematic-Residual 35
The Dispersion of Returns 12
Total 34
Risk analysis, goal of 8
Risk decomposition 34
Active 36
Active Risk 36
Active Systematic-Active Residual Risk 37
overview 38
Systematic-Residual Risk 35
Total Risk 34
Risk forecasting 59–60
GARCH model 59
Specific risk model 60
Risk index
definition 132
Risk index exposures 41
Risk index factor returns
Currency Sensitivity 125
Earnings Variability 124
Earnings Yield 124
Growth 123
Leverage 125
Momentum 122 

Size 122
Size Nonlinearity 123
Trading Activity 123
Value 124
Volatility 122
Yield 125
Risk index formulation 45
Risk index return
multiple 121
single 121
Risk indices
and descriptors in US-E3 58–59, 67–76
Currency Sensitivity 59, 69, 75, 119, 125
definition 44
definitions 74
differences between US-E2 and US-E3 67
Dividend Yield 67, 75, 120
Earnings Variability 75, 119, 124
Earnings Yield 75, 118, 124
Earnings-to-Price Ratio 67
factor returns 121–125
Foreign Income 59
frequency distributions 116–120
Growth 67, 68, 75, 118, 123
improved independence 59
Labor Intensity 59
Leverage 69, 75, 119, 125
Momentum 74, 116, 122
Non-Estimation Universe 65
Non-Estimation Universe Indicator 76
Size 68, 74, 117, 122
Size Nonlinearity 55, 68, 74, 117, 123
table, US-E3 and US-E2 71–73
Trading Activity 67, 74, 117, 123
US-E3 67
US-E3 and US-E2 at a glance
table 71–73
Value 75, 118, 124
Variability in Markets 67
Volatility 58, 67, 74, 116, 122
Yield 125
Risk measurement 13
Risk model features
comparison 53–54
Risk modes
Active Risk 36
Active Systematic-Active Residual Risk 37
Systematic-Residual Risk 35
Total Risk 34
Risk prediction with MFMs 26
Risk-free return
definition 132 

Rogers, Will 16
Rosenberg, Barr 19
Ross, Stephen A. 19
R-squared 128
definition 131
Rudd, Andrew 5 

## S

S&P 500
    assets in US-E3 estimation universe 64
Score
    definition 132
Section I: Theory 3, 7–54
Section II: US-E3 Model Details 3, 55–91
Sector mapping of US-E3 industries table 83–84
Sectoral emphasis 32, 33
Sectors 78
Sectors, US-E3
    table 106–114
    Basic Materials 106
    Commercial Services 113
    Consumer Cyclicals 107–109
    Consumer Noncyclicals 107
    Consumer Services 109
    Energy 106–107
    Financial 113–114
    Health Care 111
    Industrials 110
    Technology 112
    Telecommunications 113
    Transport 110–111
    Utilities 110
Security market line definition 132
Sharpe ratio definition 132
Sharpe, William 17, 18
Significance definition 133
Single risk index return 121
Single-factor model 130
Single-factor models 25 excess rate of return 25
Single-index model 130
Size 96, 117 factor returns 122
Size Nonlinearity 55, 58, 68, 74, 96, 117 factor returns 123
Skill definition 133 

Specific return
definition 133
Specific risk 34, 115
definition 42, 133
estimating the scaling coefficients 52
final forecast 52
modeling the average level 50
modeling the relative level 51
Specific risk model 60
differences between US-E3 and US-E2 91
Specific risk modeling
methodology 50
overview 49
US-E3 91
Standard Deviation
Option-Implied 59
Standard deviation 13
of return 11
Standard error
definition 133
Standardization 44
definition 133
Statistical factor models 19
Statistical significance
definition 133
Stefek, Dan 11
Stock selection 32, 33
Systematic return
definition 133
Systematic risk 35
definition 133
Systematic-Residual Risk
decomposition 35 

## T

Technology 112
Telecommunications 113
The US-E3 Estimation Universe 3, 63–65
Theory of equity risk and return 3
Total Plan Risk™ 1
Total return 37
Total Risk
decomposition 34
Tracking error 127, 134
definition 32
Trading Activity 67, 74, 96, 117
factor returns 123
Transaction costs
definition 134
Transport 110–111 

t-statistic
definition 134 

## U

U.S. Equity Risk Model 1
covariance and variance calculations 27
factors 27
industry exposures 45
Universe
definition 134
Universe, estimation
in US-E3 57
Updating the model 52
US-E1 55
US-E2 55
asset class issues 61
estimation universe 65
HICAP 77
industries 4, 56–57
LOCAP 86
Miscellaneous industry 85
risk indices 67
Financial Leverage 69
Foreign Income 69
Labor Intensity 69
table 71–73
US-E3
advances over E2 55–61
asset class issues 61
covariance and variance calculations 27
descriptors 58–59
diagnostics 60
estimating the factor covariance matrix 89
estimation universe 65
factor return estimation 60
factors 27
flexible industries 57
future modeling of asset classes 61
increased size of estimation universe 57
industry changes 56–57
Industry classification scheme 77–78
industry evolution 81–82
Industry weights 79–81
model details 3
model fit-related issues 60
model parameters, refitting of 60
new industries 56–57
reclassification of industries 56
risk forecasting 59–60
risk indices 67 

US-E3 and US-E2 risk indices
table 71–73
US-E3 Descriptor Definitions 4, 93–104
US-E3 Estimation Universe 63–65
US-E3 estimation universe
capitalization 64
Compustat data present 64
grandfathering 65
industry fill-in 64
minimum price 64
overview 63
S&P 500 membership 64
selection process 63
US-E3 frequency distributions
predicted beta 115
risk indices 116–120
Currency Sensitivity 119
Dividend Yield 120
Earnings Variability 119
Earnings Yield 118
Growth 118
Leverage 119
Momentum 116
Size 117
Size Nonlinearity 117
Trading Activity 117
Value 118
Volatility 116
specific risk 115
US-E3 Frequency Distributions for
Predicted Beta, Specific Risk,
Risk Indices 4, 115–120
US-E3 Industries 3, 77–84
US-E3 industries
overview 77
sector mapping 82
table 83–84
US-E3 Industries, Mini-Industries, Example
Companies, and Codes 4, 105–114
table 106–114
US-E3 industry definitions
table 106–114
US-E3 Risk Index Factor Returns 4, 121–125
US-E3 risk index factor returns
Currency Sensitivity 125
Earnings Variability 124
Earnings Yield 124
Growth 123
Leverage 125
Momentum 122
Size 122
Size Nonlinearity 123 

Trading Activity 123
Value 124
Volatility 122
Yield 125
US-E3 risk indices
    definitions 74
    table 71–73
US-E3 Risk Indices and Descriptors 3, 67–76
US-E3 specific risk model
    differences from US-E2 91
US-E3 Specific Risk Modeling 4, 91
Utilities 110
Utility
    definition 134 

## V

Valuation models 79
Value 101, 118
factor returns 124
Value added
definition 135
Value risk index 75
Variability in Markets 58, 67
Variance 13, 27, 29, 132
definition 135
Volatility 58, 67, 74, 93, 116
definition 135
factor returns 122 

## W

Web site, BARRA's 5
Weights
final 80
ongoing assignment, industry and weights 80
Why Risk is Important 3, 7–9
Windsorizing 52
World Markets Model™ 1 

## Y

Yield 129, 135
factor returns 125
Yield, earnings 129 

## Contributors

Editors 

Ronald N. Kahn 

Pamela Brougham 

Paul Green 

Consultants 

Ken Hui 

Tom Leimkuhler 

Scott Scheffler 

Aamir Sheikh 

Production Services 

Susan McIntosh 